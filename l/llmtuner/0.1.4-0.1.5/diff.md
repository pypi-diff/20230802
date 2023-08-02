# Comparing `tmp/llmtuner-0.1.4.tar.gz` & `tmp/llmtuner-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llmtuner-0.1.4.tar", last modified: Tue Aug  1 04:14:57 2023, max compression
+gzip compressed data, was "llmtuner-0.1.5.tar", last modified: Wed Aug  2 08:15:47 2023, max compression
```

## Comparing `llmtuner-0.1.4.tar` & `llmtuner-0.1.5.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:57.470154 llmtuner-0.1.4/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-07-21 08:45:52.000000 llmtuner-0.1.4/LICENSE
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    15186 2023-08-01 04:14:57.470154 llmtuner-0.1.4/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    14586 2023-07-21 08:45:58.000000 llmtuner-0.1.4/README.md
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-07-21 08:45:58.000000 llmtuner-0.1.4/pyproject.toml
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-08-01 04:14:57.470154 llmtuner-0.1.4/setup.cfg
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2033 2023-07-21 08:45:58.000000 llmtuner-0.1.4/setup.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.326114 llmtuner-0.1.4/src/
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.346114 llmtuner-0.1.4/src/llmtuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       64 2023-08-01 04:05:57.000000 llmtuner-0.1.4/src/llmtuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.362115 llmtuner-0.1.4/src/llmtuner/api/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:05:52.000000 llmtuner-0.1.4/src/llmtuner/api/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4620 2023-08-01 04:05:52.000000 llmtuner-0.1.4/src/llmtuner/api/app.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2146 2023-08-01 04:05:52.000000 llmtuner-0.1.4/src/llmtuner/api/protocol.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.394116 llmtuner-0.1.4/src/llmtuner/chat/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-08-01 04:05:52.000000 llmtuner-0.1.4/src/llmtuner/chat/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4420 2023-08-01 04:05:52.000000 llmtuner-0.1.4/src/llmtuner/chat/stream_chat.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.510120 llmtuner-0.1.4/src/llmtuner/dsets/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      153 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/dsets/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4657 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/dsets/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     9418 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/dsets/preprocess.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      547 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/dsets/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.630125 llmtuner-0.1.4/src/llmtuner/extras/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3091 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/callbacks.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1735 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/constants.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      965 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/logging.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4262 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/misc.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1788 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/ploting.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2148 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/save_and_load.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6468 2023-08-01 04:05:53.000000 llmtuner-0.1.4/src/llmtuner/extras/template.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.746129 llmtuner-0.1.4/src/llmtuner/hparams/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      222 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/hparams/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5414 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/hparams/data_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3831 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/hparams/finetuning_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      374 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/hparams/general_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1973 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/hparams/generating_args.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3053 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/hparams/model_args.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.770130 llmtuner-0.1.4/src/llmtuner/tuner/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      241 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/__init__.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.926135 llmtuner-0.1.4/src/llmtuner/tuner/core/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/core/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3910 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/core/adapter.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     7060 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/core/loader.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     6910 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/core/parser.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4228 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/core/trainer.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.986137 llmtuner-0.1.4/src/llmtuner/tuner/ppo/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/ppo/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8287 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/ppo/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1719 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/ppo/utils.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3181 2023-08-01 04:05:54.000000 llmtuner-0.1.4/src/llmtuner/tuner/ppo/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:57.010138 llmtuner-0.1.4/src/llmtuner/tuner/pt/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/pt/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2595 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/pt/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:57.094141 llmtuner-0.1.4/src/llmtuner/tuner/rm/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/rm/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      802 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/rm/collator.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/rm/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2601 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/rm/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2854 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/rm/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:57.158143 llmtuner-0.1.4/src/llmtuner/tuner/sft/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/sft/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2225 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/sft/metric.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4595 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/sft/trainer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3975 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/tuner/sft/workflow.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:57.298148 llmtuner-0.1.4/src/llmtuner/webui/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     3089 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/webui/chat.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2564 2023-08-01 04:05:55.000000 llmtuner-0.1.4/src/llmtuner/webui/common.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:57.454153 llmtuner-0.1.4/src/llmtuner/webui/components/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      298 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/__init__.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1759 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/chatbot.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      677 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/data.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2617 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/eval.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      939 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/export.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1468 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/infer.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     5166 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/sft.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2123 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/components/top.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      387 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/css.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1603 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/interface.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    13920 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/locales.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     1261 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/manager.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     8162 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/runner.py
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     4279 2023-08-01 04:05:56.000000 llmtuner-0.1.4/src/llmtuner/webui/utils.py
-drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-01 04:14:56.350115 llmtuner-0.1.4/src/llmtuner.egg-info/
--rw-r--r--   0 zhengyw  (38105) domain users (10513)    15186 2023-08-01 04:14:55.000000 llmtuner-0.1.4/src/llmtuner.egg-info/PKG-INFO
--rw-r--r--   0 zhengyw  (38105) domain users (10513)     2274 2023-08-01 04:14:55.000000 llmtuner-0.1.4/src/llmtuner.egg-info/SOURCES.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-08-01 04:14:55.000000 llmtuner-0.1.4/src/llmtuner.egg-info/dependency_links.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)      215 2023-08-01 04:14:55.000000 llmtuner-0.1.4/src/llmtuner.egg-info/requires.txt
--rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-08-01 04:14:55.000000 llmtuner-0.1.4/src/llmtuner.egg-info/top_level.txt
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.293235 llmtuner-0.1.5/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    11524 2023-08-02 08:15:31.000000 llmtuner-0.1.5/LICENSE
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    16576 2023-08-02 08:15:47.293235 llmtuner-0.1.5/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    16008 2023-08-02 08:15:31.000000 llmtuner-0.1.5/README.md
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       87 2023-08-02 08:15:31.000000 llmtuner-0.1.5/pyproject.toml
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       38 2023-08-02 08:15:47.293235 llmtuner-0.1.5/setup.cfg
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2033 2023-08-02 08:15:31.000000 llmtuner-0.1.5/setup.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.109227 llmtuner-0.1.5/src/
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.117228 llmtuner-0.1.5/src/llmtuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       64 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.125228 llmtuner-0.1.5/src/llmtuner/api/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:27.000000 llmtuner-0.1.5/src/llmtuner/api/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4620 2023-08-02 08:15:27.000000 llmtuner-0.1.5/src/llmtuner/api/app.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2146 2023-08-02 08:15:27.000000 llmtuner-0.1.5/src/llmtuner/api/protocol.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.129228 llmtuner-0.1.5/src/llmtuner/chat/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-08-02 08:15:27.000000 llmtuner-0.1.5/src/llmtuner/chat/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4074 2023-08-02 08:15:27.000000 llmtuner-0.1.5/src/llmtuner/chat/stream_chat.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.165230 llmtuner-0.1.5/src/llmtuner/dsets/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      153 2023-08-02 08:15:27.000000 llmtuner-0.1.5/src/llmtuner/dsets/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4863 2023-08-02 08:15:27.000000 llmtuner-0.1.5/src/llmtuner/dsets/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     9288 2023-08-02 08:15:27.000000 llmtuner-0.1.5/src/llmtuner/dsets/preprocess.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      547 2023-08-02 08:15:27.000000 llmtuner-0.1.5/src/llmtuner/dsets/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.177230 llmtuner-0.1.5/src/llmtuner/extras/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:28.000000 llmtuner-0.1.5/src/llmtuner/extras/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3091 2023-08-02 08:15:27.000000 llmtuner-0.1.5/src/llmtuner/extras/callbacks.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1735 2023-08-02 08:15:27.000000 llmtuner-0.1.5/src/llmtuner/extras/constants.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      965 2023-08-02 08:15:27.000000 llmtuner-0.1.5/src/llmtuner/extras/logging.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5286 2023-08-02 08:15:27.000000 llmtuner-0.1.5/src/llmtuner/extras/misc.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1788 2023-08-02 08:15:28.000000 llmtuner-0.1.5/src/llmtuner/extras/ploting.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2148 2023-08-02 08:15:28.000000 llmtuner-0.1.5/src/llmtuner/extras/save_and_load.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7183 2023-08-02 08:15:28.000000 llmtuner-0.1.5/src/llmtuner/extras/template.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.189231 llmtuner-0.1.5/src/llmtuner/hparams/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      222 2023-08-02 08:15:28.000000 llmtuner-0.1.5/src/llmtuner/hparams/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5414 2023-08-02 08:15:28.000000 llmtuner-0.1.5/src/llmtuner/hparams/data_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3831 2023-08-02 08:15:28.000000 llmtuner-0.1.5/src/llmtuner/hparams/finetuning_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      374 2023-08-02 08:15:28.000000 llmtuner-0.1.5/src/llmtuner/hparams/general_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1973 2023-08-02 08:15:28.000000 llmtuner-0.1.5/src/llmtuner/hparams/generating_args.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3053 2023-08-02 08:15:28.000000 llmtuner-0.1.5/src/llmtuner/hparams/model_args.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.193231 llmtuner-0.1.5/src/llmtuner/tuner/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      241 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/__init__.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.201231 llmtuner-0.1.5/src/llmtuner/tuner/core/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      136 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/core/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3910 2023-08-02 08:15:28.000000 llmtuner-0.1.5/src/llmtuner/tuner/core/adapter.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     7060 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/core/loader.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     6910 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/core/parser.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4228 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/core/trainer.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.205231 llmtuner-0.1.5/src/llmtuner/tuner/ppo/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/ppo/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8287 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/ppo/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1719 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/ppo/utils.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3181 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/ppo/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.209231 llmtuner-0.1.5/src/llmtuner/tuner/pt/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/pt/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2595 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/pt/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.241233 llmtuner-0.1.5/src/llmtuner/tuner/rm/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       47 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/rm/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      802 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/rm/collator.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      273 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/rm/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2601 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/rm/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2854 2023-08-02 08:15:29.000000 llmtuner-0.1.5/src/llmtuner/tuner/rm/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.249233 llmtuner-0.1.5/src/llmtuner/tuner/sft/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)       49 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/tuner/sft/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2225 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/tuner/sft/metric.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4595 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/tuner/sft/trainer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3975 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/tuner/sft/workflow.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.261234 llmtuner-0.1.5/src/llmtuner/webui/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     3089 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/chat.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2564 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/common.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.289235 llmtuner-0.1.5/src/llmtuner/webui/components/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      298 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/components/__init__.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1759 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/components/chatbot.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      677 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/components/data.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2617 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/components/eval.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      939 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/components/export.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1468 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/components/infer.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     5166 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/components/sft.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2123 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/components/top.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      387 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/css.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1603 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/interface.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    13920 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/locales.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     1261 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/manager.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     8162 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/runner.py
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     4279 2023-08-02 08:15:30.000000 llmtuner-0.1.5/src/llmtuner/webui/utils.py
+drwxr-xr-x   0 zhengyw  (38105) domain users (10513)        0 2023-08-02 08:15:47.121228 llmtuner-0.1.5/src/llmtuner.egg-info/
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)    16576 2023-08-02 08:15:45.000000 llmtuner-0.1.5/src/llmtuner.egg-info/PKG-INFO
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)     2274 2023-08-02 08:15:46.000000 llmtuner-0.1.5/src/llmtuner.egg-info/SOURCES.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        1 2023-08-02 08:15:45.000000 llmtuner-0.1.5/src/llmtuner.egg-info/dependency_links.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)      215 2023-08-02 08:15:45.000000 llmtuner-0.1.5/src/llmtuner.egg-info/requires.txt
+-rw-r--r--   0 zhengyw  (38105) domain users (10513)        9 2023-08-02 08:15:45.000000 llmtuner-0.1.5/src/llmtuner.egg-info/top_level.txt
```

### Comparing `llmtuner-0.1.4/LICENSE` & `llmtuner-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/PKG-INFO` & `llmtuner-0.1.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.1.4
+Version: 0.1.5
 Summary: Easy-to-use fine-tuning framework using PEFT
 Home-page: https://github.com/hiyouga/LLaMA-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -28,35 +28,41 @@
 [![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Efficient-Tuning)](LICENSE)
 [![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Efficient-Tuning)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/commits/main)
 [![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/pulls)
 
 👋 Join our [WeChat](assets/wechat.jpg).
 
+\[ English | [中文](README_zh.md) \]
+
 ## Changelog
 
-[23/07/19] Now we support training the **LLaMA-2** models in this repo. Try `--model_name_or_path meta-llama/Llama-2-7b-hf` argument to use the LLaMA-2 model. Remember to use `--prompt_template llama2` argument when you are using the LLaMA-2-chat model.
+[23/07/31] Now we support dataset streaming. Try `--streaming` and `--max_steps 100` arguments to stream your dataset.
+
+[23/07/29] We release two instruction-tuned 13B models at Hugging Face. See these Hugging Face Repos ([LLaMA-2](https://huggingface.co/hiyouga/Llama-2-Chinese-13b-chat) / [Baichuan](https://huggingface.co/hiyouga/baichuan-13b-sft)) for details.
+
+[23/07/19] Now we support training the **LLaMA-2** models in this repo. Try `--model_name_or_path meta-llama/Llama-2-7b-hf` argument to use the LLaMA-2 model. Remember to use `--template llama2` argument when you are using the LLaMA-2-chat model.
 
 [23/07/18] Now we develop an all-in-one Web UI for training, evaluation and inference. Try `train_web.py` to fine-tune models in your Web browser. Thank [@KanadeSiina](https://github.com/KanadeSiina) and [@codemayq](https://github.com/codemayq) for their efforts in the development.
 
-[23/07/11] Now we support training the **Baichuan-13B** model in this repo. Please replace the Baichuan-13B model file with `tests/modeling_baichuan.py` and try `--model_name_or_path path_to_baichuan_model` and `--lora_target W_pack` arguments to train the Baichuan-13B model. Remember to use `--prompt_template baichuan` argument when you are using the Baichuan-13B-Chat model.
+[23/07/11] Now we support training the **Baichuan-13B** model in this repo. Try `--model_name_or_path baichuan-inc/Baichuan-13B-Base` and `--lora_target W_pack` arguments to train the Baichuan-13B model. Remember to use `--template baichuan` argument when you are using the Baichuan-13B-Chat model.
 
 [23/07/09] Now we release [FastEdit](https://github.com/hiyouga/FastEdit)⚡🩹, an easy-to-use package for editing the factual knowledge of large language models efficiently. Please follow [FastEdit](https://github.com/hiyouga/FastEdit) if you are interested.
 
-[23/07/07] Now we support training the **InternLM-7B** model in this repo. Try `--model_name_or_path internlm/internlm-7b` argument to use the InternLM model. Remember to use `--prompt_template intern` argument when you are using the InternLM-chat model.
+[23/07/07] Now we support training the **InternLM-7B** model in this repo. Try `--model_name_or_path internlm/internlm-7b` argument to use the InternLM model. Remember to use `--template intern` argument when you are using the InternLM-chat model.
 
 [23/07/05] Now we support training the **Falcon-7B/40B** models in this repo. Try `--model_name_or_path tiiuae/falcon-7b` and `--lora_target query_key_value` arguments to use the Falcon model.
 
 [23/06/29] We provide a **reproducible example** of training a chat model using instruction-following datasets, see this [Hugging Face Repo](https://huggingface.co/hiyouga/baichuan-7b-sft) for details.
 
 [23/06/22] Now we align the [demo API](src/api_demo.py) with the [OpenAI's](https://platform.openai.com/docs/api-reference/chat) format where you can insert the fine-tuned model in **arbitrary ChatGPT-based applications**.
 
 [23/06/15] Now we support training the **Baichuan-7B** model in this repo. Try `--model_name_or_path baichuan-inc/Baichuan-7B` and `--lora_target W_pack` arguments to use the Baichuan-7B model.
 
-[23/06/03] Now we support quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). Try `--quantization_bit 4/8` argument to work with quantized model. (experimental feature)
+[23/06/03] Now we support quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). Try `--quantization_bit 4/8` argument to work with quantized models.
 
 [23/05/31] Now we support training the **BLOOM & BLOOMZ** models in this repo. Try `--model_name_or_path bigscience/bloomz-7b1-mt` and `--lora_target query_key_value` arguments to use the BLOOMZ model.
 
 ## Supported Models
 
 - [LLaMA](https://github.com/facebookresearch/llama) (7B/13B/33B/65B)
 - [LLaMA-2](https://huggingface.co/meta-llama) (7B/13B/70B)
@@ -81,14 +87,18 @@
   - [LoRA](https://arxiv.org/abs/2106.09685)
   - [QLoRA](https://arxiv.org/abs/2305.14314)
 
 ## Provided Datasets
 
 - For pre-training:
   - [Wiki Demo (en)](data/wiki_demo.txt)
+  - [RefinedWeb (en)](https://huggingface.co/datasets/tiiuae/falcon-refinedweb)
+  - [StarCoder (en)](https://huggingface.co/datasets/bigcode/starcoderdata)
+  - [Wikipedia (en)](https://huggingface.co/datasets/olm/olm-wikipedia-20221220)
+  - [Wikipedia (zh)](https://huggingface.co/datasets/pleisto/wikipedia-cn-20230720-filtered)
 - For supervised fine-tuning:
   - [Stanford Alpaca (en)](https://github.com/tatsu-lab/stanford_alpaca)
   - [Stanford Alpaca (zh)](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
   - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
   - [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
   - [Self-cognition (zh)](data/self_cognition.json)
   - [ShareGPT (zh)](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT/tree/main/Chinese-instruction-collection)
@@ -97,14 +107,15 @@
   - [BELLE 2M (zh)](https://huggingface.co/datasets/BelleGroup/train_2M_CN)
   - [BELLE 1M (zh)](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
   - [BELLE 0.5M (zh)](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
   - [BELLE Dialogue 0.4M (zh)](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M)
   - [BELLE School Math 0.25M (zh)](https://huggingface.co/datasets/BelleGroup/school_math_0.25M)
   - [BELLE Multiturn Chat 0.8M (zh)](https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M)
   - [Firefly 1.1M (zh)](https://huggingface.co/datasets/YeungNLP/firefly-train-1.1M)
+  - [LIMA (en)](https://huggingface.co/datasets/GAIR/lima)
   - [CodeAlpaca 20k (en)](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k)
   - [Alpaca CoT (multilingual)](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT)
   - [Web QA (zh)](https://huggingface.co/datasets/suolyer/webqa)
   - [UltraChat (en)](https://github.com/thunlp/UltraChat)
   - [WebNovel (zh)](https://huggingface.co/datasets/zxbsmk/webnovel_cn)
 - For reward modelling:
   - [HH-RLHF (en)](https://huggingface.co/datasets/Anthropic/hh-rlhf)
@@ -126,52 +137,56 @@
 - 🤗Transformers, Datasets, Accelerate, PEFT and TRL
 - jieba, rouge-chinese and nltk (used at evaluation)
 - gradio and matplotlib (used in web_demo.py)
 - uvicorn, fastapi and sse-starlette (used in api_demo.py)
 
 And **powerful GPUs**!
 
-If you want to enable quantized LoRA (QLoRA) on the Windows platform, you should install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.1.
-
-```bash
-pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.39.1-py3-none-win_amd64.whl
-```
-
 ## Getting Started
 
 ### Data Preparation (optional)
 
 Please refer to `data/example_dataset` for checking the details about the format of dataset files. You can either use a single `.json` file or a [dataset loading script](https://huggingface.co/docs/datasets/dataset_script) with multiple files to create a custom dataset.
 
 Note: please update `data/dataset_info.json` to use your custom dataset. About the format of this file, please refer to `data/README.md`.
 
 ### Dependence Installation (optional)
 
 ```bash
+git lfs install
 git clone https://github.com/hiyouga/LLaMA-Efficient-Tuning.git
 conda create -n llama_etuning python=3.10
 conda activate llama_etuning
 cd LLaMA-Efficient-Tuning
 pip install -r requirements.txt
 ```
 
+If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you will be required to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.1.
+
+```bash
+pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.39.1-py3-none-win_amd64.whl
+```
+
 ### All-in-one Web UI
 
 ```bash
-python src/train_web.py
+CUDA_VISIBLE_DEVICES=0 python src/train_web.py
 ```
 
+Currently the web UI only supports training on **a single GPU**.
+
 ### (Continually) Pre-Training
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage pt \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset wiki_demo \
+    --template default \
     --finetuning_type lora \
     --output_dir path_to_pt_checkpoint \
     --overwrite_cache \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
     --logging_steps 10 \
@@ -186,37 +201,43 @@
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset alpaca_gpt4_en \
+    --template default \
     --finetuning_type lora \
     --output_dir path_to_sft_checkpoint \
     --overwrite_cache \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
     --logging_steps 10 \
     --save_steps 1000 \
     --learning_rate 5e-5 \
     --num_train_epochs 3.0 \
     --plot_loss \
     --fp16
 ```
 
+Remember to specify `--lora_target W_pack` if you are using Baichuan models.
+
 ### Reward Model Training
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage rm \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset comparison_gpt4_en \
+    --template default \
     --finetuning_type lora \
+    --resume_lora_training False \
+    --checkpoint_dir path_to_sft_checkpoint \
     --output_dir path_to_rm_checkpoint \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
     --logging_steps 10 \
     --save_steps 1000 \
     --learning_rate 1e-5 \
@@ -229,26 +250,27 @@
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage ppo \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset alpaca_gpt4_en \
+    --template default \
     --finetuning_type lora \
+    --resume_lora_training False \
     --checkpoint_dir path_to_sft_checkpoint \
     --reward_model path_to_rm_checkpoint \
     --output_dir path_to_ppo_checkpoint \
     --per_device_train_batch_size 2 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
     --logging_steps 10 \
     --save_steps 1000 \
     --learning_rate 1e-5 \
     --num_train_epochs 1.0 \
-    --resume_lora_training False \
     --plot_loss
 ```
 
 ### Distributed Training
 
 ```bash
 accelerate config # configure the environment
@@ -287,14 +309,15 @@
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
     --model_name_or_path path_to_your_model \
     --do_eval \
     --dataset alpaca_gpt4_en \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_eval_result \
     --per_device_eval_batch_size 8 \
     --max_samples 100 \
     --predict_with_generate
 ```
@@ -305,74 +328,83 @@
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
     --model_name_or_path path_to_your_model \
     --do_predict \
     --dataset alpaca_gpt4_en \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_predict_result \
     --per_device_eval_batch_size 8 \
     --max_samples 100 \
     --predict_with_generate
 ```
 
-If you want to predict the samples with empty responses, please kindly fill the `response` column with **dummy tokens** to ensure the sample will not be discarded throughout the preprocessing phase.
-
 ### API Demo
 
 ```bash
 python src/api_demo.py \
     --model_name_or_path path_to_your_model \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 Visit `http://localhost:8000/docs` for API documentation.
 
 ### CLI Demo
 
 ```bash
 python src/cli_demo.py \
     --model_name_or_path path_to_your_model \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Web Demo
 
 ```bash
 python src/web_demo.py \
     --model_name_or_path path_to_your_model \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Export model
 
 ```bash
 python src/export_model.py \
     --model_name_or_path path_to_your_model \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_export
 ```
 
+## TODO
+
+- [ ] Supporting flash attention ([torch](https://pytorch.org/docs/stable/generated/torch.nn.functional.scaled_dot_product_attention.html) / [xformers](https://github.com/facebookresearch/xformers) / [flashattn](https://github.com/Dao-AILab/flash-attention)).
+- [ ] Implementing multi-query attention for faster inference.
+- [ ] Supporting full-parameter RLHF training.
+
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
 Please follow the model licenses to use the corresponding model weights:
 
 - [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md)
 - [LLaMA-2](https://ai.meta.com/llama/license/)
 - [BLOOM](https://huggingface.co/spaces/bigscience/license)
 - [Falcon](LICENSE)
-- [baichuan](https://huggingface.co/baichuan-inc/baichuan-7B/resolve/main/baichuan-7B%20%E6%A8%A1%E5%9E%8B%E8%AE%B8%E5%8F%AF%E5%8D%8F%E8%AE%AE.pdf)
+- [Baichuan](https://huggingface.co/baichuan-inc/baichuan-7B/resolve/main/baichuan-7B%20%E6%A8%A1%E5%9E%8B%E8%AE%B8%E5%8F%AF%E5%8D%8F%E8%AE%AE.pdf)
 - [InternLM](https://github.com/InternLM/InternLM#open-source-license)
 
 ## Citation
 
 If this work is helpful, please kindly cite as:
 
 ```bibtex
```

### Comparing `llmtuner-0.1.4/README.md` & `llmtuner-0.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -4,35 +4,41 @@
 [![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Efficient-Tuning)](LICENSE)
 [![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Efficient-Tuning)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/commits/main)
 [![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/pulls)
 
 👋 Join our [WeChat](assets/wechat.jpg).
 
+\[ English | [中文](README_zh.md) \]
+
 ## Changelog
 
-[23/07/19] Now we support training the **LLaMA-2** models in this repo. Try `--model_name_or_path meta-llama/Llama-2-7b-hf` argument to use the LLaMA-2 model. Remember to use `--prompt_template llama2` argument when you are using the LLaMA-2-chat model.
+[23/07/31] Now we support dataset streaming. Try `--streaming` and `--max_steps 100` arguments to stream your dataset.
+
+[23/07/29] We release two instruction-tuned 13B models at Hugging Face. See these Hugging Face Repos ([LLaMA-2](https://huggingface.co/hiyouga/Llama-2-Chinese-13b-chat) / [Baichuan](https://huggingface.co/hiyouga/baichuan-13b-sft)) for details.
+
+[23/07/19] Now we support training the **LLaMA-2** models in this repo. Try `--model_name_or_path meta-llama/Llama-2-7b-hf` argument to use the LLaMA-2 model. Remember to use `--template llama2` argument when you are using the LLaMA-2-chat model.
 
 [23/07/18] Now we develop an all-in-one Web UI for training, evaluation and inference. Try `train_web.py` to fine-tune models in your Web browser. Thank [@KanadeSiina](https://github.com/KanadeSiina) and [@codemayq](https://github.com/codemayq) for their efforts in the development.
 
-[23/07/11] Now we support training the **Baichuan-13B** model in this repo. Please replace the Baichuan-13B model file with `tests/modeling_baichuan.py` and try `--model_name_or_path path_to_baichuan_model` and `--lora_target W_pack` arguments to train the Baichuan-13B model. Remember to use `--prompt_template baichuan` argument when you are using the Baichuan-13B-Chat model.
+[23/07/11] Now we support training the **Baichuan-13B** model in this repo. Try `--model_name_or_path baichuan-inc/Baichuan-13B-Base` and `--lora_target W_pack` arguments to train the Baichuan-13B model. Remember to use `--template baichuan` argument when you are using the Baichuan-13B-Chat model.
 
 [23/07/09] Now we release [FastEdit](https://github.com/hiyouga/FastEdit)⚡🩹, an easy-to-use package for editing the factual knowledge of large language models efficiently. Please follow [FastEdit](https://github.com/hiyouga/FastEdit) if you are interested.
 
-[23/07/07] Now we support training the **InternLM-7B** model in this repo. Try `--model_name_or_path internlm/internlm-7b` argument to use the InternLM model. Remember to use `--prompt_template intern` argument when you are using the InternLM-chat model.
+[23/07/07] Now we support training the **InternLM-7B** model in this repo. Try `--model_name_or_path internlm/internlm-7b` argument to use the InternLM model. Remember to use `--template intern` argument when you are using the InternLM-chat model.
 
 [23/07/05] Now we support training the **Falcon-7B/40B** models in this repo. Try `--model_name_or_path tiiuae/falcon-7b` and `--lora_target query_key_value` arguments to use the Falcon model.
 
 [23/06/29] We provide a **reproducible example** of training a chat model using instruction-following datasets, see this [Hugging Face Repo](https://huggingface.co/hiyouga/baichuan-7b-sft) for details.
 
 [23/06/22] Now we align the [demo API](src/api_demo.py) with the [OpenAI's](https://platform.openai.com/docs/api-reference/chat) format where you can insert the fine-tuned model in **arbitrary ChatGPT-based applications**.
 
 [23/06/15] Now we support training the **Baichuan-7B** model in this repo. Try `--model_name_or_path baichuan-inc/Baichuan-7B` and `--lora_target W_pack` arguments to use the Baichuan-7B model.
 
-[23/06/03] Now we support quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). Try `--quantization_bit 4/8` argument to work with quantized model. (experimental feature)
+[23/06/03] Now we support quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). Try `--quantization_bit 4/8` argument to work with quantized models.
 
 [23/05/31] Now we support training the **BLOOM & BLOOMZ** models in this repo. Try `--model_name_or_path bigscience/bloomz-7b1-mt` and `--lora_target query_key_value` arguments to use the BLOOMZ model.
 
 ## Supported Models
 
 - [LLaMA](https://github.com/facebookresearch/llama) (7B/13B/33B/65B)
 - [LLaMA-2](https://huggingface.co/meta-llama) (7B/13B/70B)
@@ -57,14 +63,18 @@
   - [LoRA](https://arxiv.org/abs/2106.09685)
   - [QLoRA](https://arxiv.org/abs/2305.14314)
 
 ## Provided Datasets
 
 - For pre-training:
   - [Wiki Demo (en)](data/wiki_demo.txt)
+  - [RefinedWeb (en)](https://huggingface.co/datasets/tiiuae/falcon-refinedweb)
+  - [StarCoder (en)](https://huggingface.co/datasets/bigcode/starcoderdata)
+  - [Wikipedia (en)](https://huggingface.co/datasets/olm/olm-wikipedia-20221220)
+  - [Wikipedia (zh)](https://huggingface.co/datasets/pleisto/wikipedia-cn-20230720-filtered)
 - For supervised fine-tuning:
   - [Stanford Alpaca (en)](https://github.com/tatsu-lab/stanford_alpaca)
   - [Stanford Alpaca (zh)](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
   - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
   - [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
   - [Self-cognition (zh)](data/self_cognition.json)
   - [ShareGPT (zh)](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT/tree/main/Chinese-instruction-collection)
@@ -73,14 +83,15 @@
   - [BELLE 2M (zh)](https://huggingface.co/datasets/BelleGroup/train_2M_CN)
   - [BELLE 1M (zh)](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
   - [BELLE 0.5M (zh)](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
   - [BELLE Dialogue 0.4M (zh)](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M)
   - [BELLE School Math 0.25M (zh)](https://huggingface.co/datasets/BelleGroup/school_math_0.25M)
   - [BELLE Multiturn Chat 0.8M (zh)](https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M)
   - [Firefly 1.1M (zh)](https://huggingface.co/datasets/YeungNLP/firefly-train-1.1M)
+  - [LIMA (en)](https://huggingface.co/datasets/GAIR/lima)
   - [CodeAlpaca 20k (en)](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k)
   - [Alpaca CoT (multilingual)](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT)
   - [Web QA (zh)](https://huggingface.co/datasets/suolyer/webqa)
   - [UltraChat (en)](https://github.com/thunlp/UltraChat)
   - [WebNovel (zh)](https://huggingface.co/datasets/zxbsmk/webnovel_cn)
 - For reward modelling:
   - [HH-RLHF (en)](https://huggingface.co/datasets/Anthropic/hh-rlhf)
@@ -102,52 +113,56 @@
 - 🤗Transformers, Datasets, Accelerate, PEFT and TRL
 - jieba, rouge-chinese and nltk (used at evaluation)
 - gradio and matplotlib (used in web_demo.py)
 - uvicorn, fastapi and sse-starlette (used in api_demo.py)
 
 And **powerful GPUs**!
 
-If you want to enable quantized LoRA (QLoRA) on the Windows platform, you should install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.1.
-
-```bash
-pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.39.1-py3-none-win_amd64.whl
-```
-
 ## Getting Started
 
 ### Data Preparation (optional)
 
 Please refer to `data/example_dataset` for checking the details about the format of dataset files. You can either use a single `.json` file or a [dataset loading script](https://huggingface.co/docs/datasets/dataset_script) with multiple files to create a custom dataset.
 
 Note: please update `data/dataset_info.json` to use your custom dataset. About the format of this file, please refer to `data/README.md`.
 
 ### Dependence Installation (optional)
 
 ```bash
+git lfs install
 git clone https://github.com/hiyouga/LLaMA-Efficient-Tuning.git
 conda create -n llama_etuning python=3.10
 conda activate llama_etuning
 cd LLaMA-Efficient-Tuning
 pip install -r requirements.txt
 ```
 
+If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you will be required to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.1.
+
+```bash
+pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.39.1-py3-none-win_amd64.whl
+```
+
 ### All-in-one Web UI
 
 ```bash
-python src/train_web.py
+CUDA_VISIBLE_DEVICES=0 python src/train_web.py
 ```
 
+Currently the web UI only supports training on **a single GPU**.
+
 ### (Continually) Pre-Training
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage pt \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset wiki_demo \
+    --template default \
     --finetuning_type lora \
     --output_dir path_to_pt_checkpoint \
     --overwrite_cache \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
     --logging_steps 10 \
@@ -162,37 +177,43 @@
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset alpaca_gpt4_en \
+    --template default \
     --finetuning_type lora \
     --output_dir path_to_sft_checkpoint \
     --overwrite_cache \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
     --logging_steps 10 \
     --save_steps 1000 \
     --learning_rate 5e-5 \
     --num_train_epochs 3.0 \
     --plot_loss \
     --fp16
 ```
 
+Remember to specify `--lora_target W_pack` if you are using Baichuan models.
+
 ### Reward Model Training
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage rm \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset comparison_gpt4_en \
+    --template default \
     --finetuning_type lora \
+    --resume_lora_training False \
+    --checkpoint_dir path_to_sft_checkpoint \
     --output_dir path_to_rm_checkpoint \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
     --logging_steps 10 \
     --save_steps 1000 \
     --learning_rate 1e-5 \
@@ -205,26 +226,27 @@
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage ppo \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset alpaca_gpt4_en \
+    --template default \
     --finetuning_type lora \
+    --resume_lora_training False \
     --checkpoint_dir path_to_sft_checkpoint \
     --reward_model path_to_rm_checkpoint \
     --output_dir path_to_ppo_checkpoint \
     --per_device_train_batch_size 2 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
     --logging_steps 10 \
     --save_steps 1000 \
     --learning_rate 1e-5 \
     --num_train_epochs 1.0 \
-    --resume_lora_training False \
     --plot_loss
 ```
 
 ### Distributed Training
 
 ```bash
 accelerate config # configure the environment
@@ -263,14 +285,15 @@
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
     --model_name_or_path path_to_your_model \
     --do_eval \
     --dataset alpaca_gpt4_en \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_eval_result \
     --per_device_eval_batch_size 8 \
     --max_samples 100 \
     --predict_with_generate
 ```
@@ -281,74 +304,83 @@
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
     --model_name_or_path path_to_your_model \
     --do_predict \
     --dataset alpaca_gpt4_en \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_predict_result \
     --per_device_eval_batch_size 8 \
     --max_samples 100 \
     --predict_with_generate
 ```
 
-If you want to predict the samples with empty responses, please kindly fill the `response` column with **dummy tokens** to ensure the sample will not be discarded throughout the preprocessing phase.
-
 ### API Demo
 
 ```bash
 python src/api_demo.py \
     --model_name_or_path path_to_your_model \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 Visit `http://localhost:8000/docs` for API documentation.
 
 ### CLI Demo
 
 ```bash
 python src/cli_demo.py \
     --model_name_or_path path_to_your_model \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Web Demo
 
 ```bash
 python src/web_demo.py \
     --model_name_or_path path_to_your_model \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Export model
 
 ```bash
 python src/export_model.py \
     --model_name_or_path path_to_your_model \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_export
 ```
 
+## TODO
+
+- [ ] Supporting flash attention ([torch](https://pytorch.org/docs/stable/generated/torch.nn.functional.scaled_dot_product_attention.html) / [xformers](https://github.com/facebookresearch/xformers) / [flashattn](https://github.com/Dao-AILab/flash-attention)).
+- [ ] Implementing multi-query attention for faster inference.
+- [ ] Supporting full-parameter RLHF training.
+
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
 Please follow the model licenses to use the corresponding model weights:
 
 - [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md)
 - [LLaMA-2](https://ai.meta.com/llama/license/)
 - [BLOOM](https://huggingface.co/spaces/bigscience/license)
 - [Falcon](LICENSE)
-- [baichuan](https://huggingface.co/baichuan-inc/baichuan-7B/resolve/main/baichuan-7B%20%E6%A8%A1%E5%9E%8B%E8%AE%B8%E5%8F%AF%E5%8D%8F%E8%AE%AE.pdf)
+- [Baichuan](https://huggingface.co/baichuan-inc/baichuan-7B/resolve/main/baichuan-7B%20%E6%A8%A1%E5%9E%8B%E8%AE%B8%E5%8F%AF%E5%8D%8F%E8%AE%AE.pdf)
 - [InternLM](https://github.com/InternLM/InternLM#open-source-license)
 
 ## Citation
 
 If this work is helpful, please kindly cite as:
 
 ```bibtex
```

### Comparing `llmtuner-0.1.4/setup.py` & `llmtuner-0.1.5/setup.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/api/app.py` & `llmtuner-0.1.5/src/llmtuner/api/app.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/api/protocol.py` & `llmtuner-0.1.5/src/llmtuner/api/protocol.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/chat/stream_chat.py` & `llmtuner-0.1.5/src/llmtuner/chat/stream_chat.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import torch
 from typing import TYPE_CHECKING, Any, Dict, Generator, List, Optional, Tuple
 from threading import Thread
 from transformers import TextIteratorStreamer
 
-from llmtuner.extras.misc import get_logits_processor
+from llmtuner.extras.misc import dispatch_model, get_logits_processor
 from llmtuner.extras.template import get_template
 from llmtuner.tuner import load_model_and_tokenizer
 
 if TYPE_CHECKING:
     from llmtuner.hparams import ModelArguments, DataArguments, FinetuningArguments, GeneratingArguments
 
 
@@ -17,23 +17,15 @@
         self,
         model_args: "ModelArguments",
         data_args: "DataArguments",
         finetuning_args: "FinetuningArguments",
         generating_args: "GeneratingArguments"
     ) -> None:
         self.model, self.tokenizer = load_model_and_tokenizer(model_args, finetuning_args)
-
-        if torch.cuda.device_count() > 1:
-            from accelerate import dispatch_model
-            from accelerate.utils import infer_auto_device_map, get_balanced_memory
-            device_map = infer_auto_device_map(self.model, max_memory=get_balanced_memory(self.model))
-            self.model = dispatch_model(self.model, device_map)
-        else:
-            self.model = self.model.cuda()
-
+        self.model = dispatch_model(self.model)
         self.template = get_template(data_args.template)
         self.source_prefix = data_args.source_prefix
         self.generating_args = generating_args
 
     def process_args(
         self,
         query: str,
```

### Comparing `llmtuner-0.1.4/src/llmtuner/dsets/loader.py` & `llmtuner-0.1.5/src/llmtuner/dsets/loader.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import hashlib
 from typing import TYPE_CHECKING, List, Optional
 
-from datasets import concatenate_datasets, interleave_datasets, load_dataset
+from datasets import Value, concatenate_datasets, interleave_datasets, load_dataset
 
 from llmtuner.extras.logging import get_logger
 
 if TYPE_CHECKING:
     from datasets import Dataset
     from llmtuner.hparams import ModelArguments, DataArguments
 
@@ -89,15 +89,19 @@
             dataset = dataset.select(range(max_samples_temp))
 
         for column_name in ["prompt", "query", "response", "history"]: # align datasets
             if getattr(dataset_attr, column_name) and getattr(dataset_attr, column_name) != column_name:
                 dataset = dataset.rename_column(getattr(dataset_attr, column_name), column_name)
 
         if dataset_attr.source_prefix: # add prefix
-            dataset = dataset.map(lambda _: {"prefix": dataset_attr.source_prefix})
+            features = None
+            if data_args.streaming:
+                features = dataset.features
+                features["prefix"] = Value(dtype="string", id=None)
+            dataset = dataset.map(lambda _: {"prefix": dataset_attr.source_prefix}, features=features)
 
         all_datasets.append(dataset)
 
     if len(data_args.dataset_list) == 1:
         return all_datasets[0]
     elif data_args.mix_strategy == "concat":
         if data_args.streaming:
```

### Comparing `llmtuner-0.1.4/src/llmtuner/dsets/preprocess.py` & `llmtuner-0.1.5/src/llmtuner/dsets/preprocess.py`

 * *Files 5% similar despite different names*

```diff
@@ -14,23 +14,23 @@
 def preprocess_dataset(
     dataset: "Dataset",
     tokenizer: "PreTrainedTokenizer",
     data_args: "DataArguments",
     training_args: "Seq2SeqTrainingArguments",
     stage: Literal["pt", "sft", "rm", "ppo"]
 ) -> "Dataset":
-    column_names = list(dataset.column_names or [])
+    column_names = list(dataset.column_names)
     template = get_template(data_args.template)
 
     def construct_example(examples: Dict[str, List[Any]]) -> Generator[Any, None, None]:
         for i in range(len(examples["prompt"])):
             query, response = examples["prompt"][i], examples["response"][i]
             query = query + "\n" + examples["query"][i] if "query" in examples and examples["query"][i] else query
-            history = history if "history" in examples and examples["history"][i] else []
-            prefix = prefix if "prefix" in examples and examples["prefix"][i] else ""
+            history = examples["history"][i] if "history" in examples else None
+            prefix = examples["prefix"][i] if "prefix" in examples else None
             yield query, response, history, prefix
 
     def preprocess_pretrain_dataset(examples: Dict[str, List[Any]]) -> Dict[str, Any]:
         # build grouped texts with format `<bos> X1 X2 X3 ...` (without <eos>)
         tokenized_examples = tokenizer(examples["prompt"], add_special_tokens=False)
         concatenated_examples = {k: list(chain(*tokenized_examples[k])) for k in tokenized_examples.keys()}
         total_length = len(concatenated_examples[list(concatenated_examples.keys())[0]])
@@ -139,23 +139,27 @@
     def print_unsupervised_dataset_example(example):
         print("input_ids:\n{}".format(example["input_ids"]))
         print("inputs:\n{}".format(tokenizer.decode(example["input_ids"], skip_special_tokens=False)))
 
     if stage == "pt":
         dataset = dataset.filter(lambda example: example["prompt"])
         preprocess_function = preprocess_pretrain_dataset
+        print_function = print_unsupervised_dataset_example
     elif stage == "sft" and not training_args.predict_with_generate:
         dataset = dataset.filter(lambda example: example["prompt"] and example["response"])
         preprocess_function = preprocess_supervised_dataset
+        print_function = print_supervised_dataset_example
     elif stage == "rm":
         dataset = dataset.filter(lambda example: example["prompt"] and len(example["response"]) > 1)
         preprocess_function = preprocess_pairwise_dataset
+        print_function = print_pairwise_dataset_example
     else:
         dataset = dataset.filter(lambda example: example["prompt"])
         preprocess_function = preprocess_unsupervised_dataset
+        print_function = print_unsupervised_dataset_example
 
     with training_args.main_process_first(desc="dataset map pre-processing"):
         kwargs = {}
         if not data_args.streaming:
             kwargs = dict(
                 num_proc=data_args.preprocessing_num_workers,
                 load_from_cache_file=not data_args.overwrite_cache,
@@ -168,17 +172,9 @@
             remove_columns=column_names,
             **kwargs
         )
 
         if data_args.streaming:
             dataset = dataset.shuffle(buffer_size=data_args.buffer_size)
 
-        if stage == "pt":
-            print_unsupervised_dataset_example(next(iter(dataset)))
-        elif stage == "sft":
-            print_supervised_dataset_example(next(iter(dataset)))
-        elif stage == "rm":
-            print_pairwise_dataset_example(next(iter(dataset)))
-        elif stage == "ppo":
-            print_unsupervised_dataset_example(next(iter(dataset)))
-
+        print_function(next(iter(dataset)))
         return dataset
```

### Comparing `llmtuner-0.1.4/src/llmtuner/dsets/utils.py` & `llmtuner-0.1.5/src/llmtuner/dsets/utils.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/extras/callbacks.py` & `llmtuner-0.1.5/src/llmtuner/extras/callbacks.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/extras/constants.py` & `llmtuner-0.1.5/src/llmtuner/extras/constants.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/extras/logging.py` & `llmtuner-0.1.5/src/llmtuner/extras/logging.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/extras/ploting.py` & `llmtuner-0.1.5/src/llmtuner/extras/ploting.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/extras/save_and_load.py` & `llmtuner-0.1.5/src/llmtuner/extras/save_and_load.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/extras/template.py` & `llmtuner-0.1.5/src/llmtuner/extras/template.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,26 +42,45 @@
         history: Optional[List[Tuple[str, str]]] = None,
         prefix: Optional[str] = ""
     ) -> List[Tuple[str, str]]:
         prefix = prefix or self.prefix # use prefix if provided
         prefix = prefix + self.sep if prefix else "" # add separator for non-empty prefix
         history = history if (history and self.use_history) else []
         history = history + [(query, "")]
-        convs = [
-            [(self.sep if turn_idx else prefix) + self.prompt.format(query=query_i), resp_i]
-            for turn_idx, (query_i, resp_i) in enumerate(history)
+        return [
+            [(self.sep if i else prefix) + self.prompt.format(query=q), r]
+            for i, (q, r) in enumerate(history)
+        ]
+
+
+@dataclass
+class Llama2Template(Template):
+
+    def _format_example(
+        self,
+        query: str,
+        history: Optional[List[Tuple[str, str]]] = None,
+        prefix: Optional[str] = ""
+    ) -> List[Tuple[str, str]]:
+        prefix = prefix or self.prefix # use prefix if provided
+        prefix = prefix if prefix.startswith("<<SYS>>") else "<<SYS>>\n{}\n<</SYS>>\n\n".format(prefix)
+        history = history if (history and self.use_history) else []
+        history = history + [(query, "")]
+        return [
+            [(self.sep if i else "") + self.prompt.format(query=(q if i else prefix + q)), r]
+            for i, (q, r) in enumerate(history)
         ]
-        return convs
 
 
 templates: Dict[str, Template] = {}
 
 
 def register_template(name: str, prefix: str, prompt: str, sep: str, use_history: bool) -> None:
-    templates[name] = Template(
+    template_class = Llama2Template if name == "llama2" else Template
+    templates[name] = template_class(
         prefix=prefix,
         prompt=prompt,
         sep=sep,
         use_history=use_history
     )
 
 
@@ -107,16 +126,16 @@
            "Always answer as helpfully as possible, while being safe.  "
            "Your answers should not include any harmful, unethical, "
            "racist, sexist, toxic, dangerous, or illegal content. "
            "Please ensure that your responses are socially unbiased and positive in nature.\n"
            "If a question does not make any sense, or is not factually coherent, "
            "explain why instead of answering something not correct. "
            "If you don't know the answer to a question, please don't share false information.\n<</SYS>>\n\n",
-    prompt=" [INST] {query} [/INST] ",
-    sep="",
+    prompt="[INST] {query} [/INST] ",
+    sep="<s>",
     use_history=True
 )
 
 
 r"""
 Supports: https://huggingface.co/tatsu-lab/alpaca-7b-wdiff
           https://github.com/ymcui/Chinese-LLaMA-Alpaca
```

### Comparing `llmtuner-0.1.4/src/llmtuner/hparams/data_args.py` & `llmtuner-0.1.5/src/llmtuner/hparams/data_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/hparams/finetuning_args.py` & `llmtuner-0.1.5/src/llmtuner/hparams/finetuning_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/hparams/generating_args.py` & `llmtuner-0.1.5/src/llmtuner/hparams/generating_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/hparams/model_args.py` & `llmtuner-0.1.5/src/llmtuner/hparams/model_args.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/tuner/core/adapter.py` & `llmtuner-0.1.5/src/llmtuner/tuner/core/adapter.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/tuner/core/loader.py` & `llmtuner-0.1.5/src/llmtuner/tuner/core/loader.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/tuner/core/parser.py` & `llmtuner-0.1.5/src/llmtuner/tuner/core/parser.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/tuner/core/trainer.py` & `llmtuner-0.1.5/src/llmtuner/tuner/core/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/tuner/ppo/trainer.py` & `llmtuner-0.1.5/src/llmtuner/tuner/ppo/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/tuner/ppo/utils.py` & `llmtuner-0.1.5/src/llmtuner/tuner/ppo/utils.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/tuner/ppo/workflow.py` & `llmtuner-0.1.5/src/llmtuner/tuner/ppo/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/tuner/pt/workflow.py` & `llmtuner-0.1.5/src/llmtuner/tuner/pt/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/tuner/rm/collator.py` & `llmtuner-0.1.5/src/llmtuner/tuner/rm/collator.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/tuner/rm/trainer.py` & `llmtuner-0.1.5/src/llmtuner/tuner/rm/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/tuner/rm/workflow.py` & `llmtuner-0.1.5/src/llmtuner/tuner/rm/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/tuner/sft/metric.py` & `llmtuner-0.1.5/src/llmtuner/tuner/sft/metric.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/tuner/sft/trainer.py` & `llmtuner-0.1.5/src/llmtuner/tuner/sft/trainer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/tuner/sft/workflow.py` & `llmtuner-0.1.5/src/llmtuner/tuner/sft/workflow.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/webui/chat.py` & `llmtuner-0.1.5/src/llmtuner/webui/chat.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/webui/common.py` & `llmtuner-0.1.5/src/llmtuner/webui/common.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/webui/components/chatbot.py` & `llmtuner-0.1.5/src/llmtuner/webui/components/chatbot.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/webui/components/data.py` & `llmtuner-0.1.5/src/llmtuner/webui/components/data.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/webui/components/eval.py` & `llmtuner-0.1.5/src/llmtuner/webui/components/eval.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/webui/components/export.py` & `llmtuner-0.1.5/src/llmtuner/webui/components/export.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/webui/components/infer.py` & `llmtuner-0.1.5/src/llmtuner/webui/components/infer.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/webui/components/sft.py` & `llmtuner-0.1.5/src/llmtuner/webui/components/sft.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/webui/components/top.py` & `llmtuner-0.1.5/src/llmtuner/webui/components/top.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/webui/interface.py` & `llmtuner-0.1.5/src/llmtuner/webui/interface.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/webui/locales.py` & `llmtuner-0.1.5/src/llmtuner/webui/locales.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/webui/manager.py` & `llmtuner-0.1.5/src/llmtuner/webui/manager.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/webui/runner.py` & `llmtuner-0.1.5/src/llmtuner/webui/runner.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner/webui/utils.py` & `llmtuner-0.1.5/src/llmtuner/webui/utils.py`

 * *Files identical despite different names*

### Comparing `llmtuner-0.1.4/src/llmtuner.egg-info/PKG-INFO` & `llmtuner-0.1.5/src/llmtuner.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: llmtuner
-Version: 0.1.4
+Version: 0.1.5
 Summary: Easy-to-use fine-tuning framework using PEFT
 Home-page: https://github.com/hiyouga/LLaMA-Efficient-Tuning
 Author: hiyouga
 Author-email: hiyouga@buaa.edu.cn
 License: Apache 2.0 License
 Keywords: LLaMA,BLOOM,Falcon,LLM,ChatGPT,transformer,pytorch,deep learning
 Classifier: Development Status :: 3 - Alpha
@@ -28,35 +28,41 @@
 [![GitHub Code License](https://img.shields.io/github/license/hiyouga/LLaMA-Efficient-Tuning)](LICENSE)
 [![GitHub last commit](https://img.shields.io/github/last-commit/hiyouga/LLaMA-Efficient-Tuning)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/commits/main)
 [![PyPI](https://img.shields.io/pypi/v/llmtuner)](https://pypi.org/project/llmtuner/)
 [![GitHub pull request](https://img.shields.io/badge/PRs-welcome-blue)](https://github.com/hiyouga/LLaMA-Efficient-Tuning/pulls)
 
 👋 Join our [WeChat](assets/wechat.jpg).
 
+\[ English | [中文](README_zh.md) \]
+
 ## Changelog
 
-[23/07/19] Now we support training the **LLaMA-2** models in this repo. Try `--model_name_or_path meta-llama/Llama-2-7b-hf` argument to use the LLaMA-2 model. Remember to use `--prompt_template llama2` argument when you are using the LLaMA-2-chat model.
+[23/07/31] Now we support dataset streaming. Try `--streaming` and `--max_steps 100` arguments to stream your dataset.
+
+[23/07/29] We release two instruction-tuned 13B models at Hugging Face. See these Hugging Face Repos ([LLaMA-2](https://huggingface.co/hiyouga/Llama-2-Chinese-13b-chat) / [Baichuan](https://huggingface.co/hiyouga/baichuan-13b-sft)) for details.
+
+[23/07/19] Now we support training the **LLaMA-2** models in this repo. Try `--model_name_or_path meta-llama/Llama-2-7b-hf` argument to use the LLaMA-2 model. Remember to use `--template llama2` argument when you are using the LLaMA-2-chat model.
 
 [23/07/18] Now we develop an all-in-one Web UI for training, evaluation and inference. Try `train_web.py` to fine-tune models in your Web browser. Thank [@KanadeSiina](https://github.com/KanadeSiina) and [@codemayq](https://github.com/codemayq) for their efforts in the development.
 
-[23/07/11] Now we support training the **Baichuan-13B** model in this repo. Please replace the Baichuan-13B model file with `tests/modeling_baichuan.py` and try `--model_name_or_path path_to_baichuan_model` and `--lora_target W_pack` arguments to train the Baichuan-13B model. Remember to use `--prompt_template baichuan` argument when you are using the Baichuan-13B-Chat model.
+[23/07/11] Now we support training the **Baichuan-13B** model in this repo. Try `--model_name_or_path baichuan-inc/Baichuan-13B-Base` and `--lora_target W_pack` arguments to train the Baichuan-13B model. Remember to use `--template baichuan` argument when you are using the Baichuan-13B-Chat model.
 
 [23/07/09] Now we release [FastEdit](https://github.com/hiyouga/FastEdit)⚡🩹, an easy-to-use package for editing the factual knowledge of large language models efficiently. Please follow [FastEdit](https://github.com/hiyouga/FastEdit) if you are interested.
 
-[23/07/07] Now we support training the **InternLM-7B** model in this repo. Try `--model_name_or_path internlm/internlm-7b` argument to use the InternLM model. Remember to use `--prompt_template intern` argument when you are using the InternLM-chat model.
+[23/07/07] Now we support training the **InternLM-7B** model in this repo. Try `--model_name_or_path internlm/internlm-7b` argument to use the InternLM model. Remember to use `--template intern` argument when you are using the InternLM-chat model.
 
 [23/07/05] Now we support training the **Falcon-7B/40B** models in this repo. Try `--model_name_or_path tiiuae/falcon-7b` and `--lora_target query_key_value` arguments to use the Falcon model.
 
 [23/06/29] We provide a **reproducible example** of training a chat model using instruction-following datasets, see this [Hugging Face Repo](https://huggingface.co/hiyouga/baichuan-7b-sft) for details.
 
 [23/06/22] Now we align the [demo API](src/api_demo.py) with the [OpenAI's](https://platform.openai.com/docs/api-reference/chat) format where you can insert the fine-tuned model in **arbitrary ChatGPT-based applications**.
 
 [23/06/15] Now we support training the **Baichuan-7B** model in this repo. Try `--model_name_or_path baichuan-inc/Baichuan-7B` and `--lora_target W_pack` arguments to use the Baichuan-7B model.
 
-[23/06/03] Now we support quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). Try `--quantization_bit 4/8` argument to work with quantized model. (experimental feature)
+[23/06/03] Now we support quantized training and inference (aka **[QLoRA](https://github.com/artidoro/qlora)**). Try `--quantization_bit 4/8` argument to work with quantized models.
 
 [23/05/31] Now we support training the **BLOOM & BLOOMZ** models in this repo. Try `--model_name_or_path bigscience/bloomz-7b1-mt` and `--lora_target query_key_value` arguments to use the BLOOMZ model.
 
 ## Supported Models
 
 - [LLaMA](https://github.com/facebookresearch/llama) (7B/13B/33B/65B)
 - [LLaMA-2](https://huggingface.co/meta-llama) (7B/13B/70B)
@@ -81,14 +87,18 @@
   - [LoRA](https://arxiv.org/abs/2106.09685)
   - [QLoRA](https://arxiv.org/abs/2305.14314)
 
 ## Provided Datasets
 
 - For pre-training:
   - [Wiki Demo (en)](data/wiki_demo.txt)
+  - [RefinedWeb (en)](https://huggingface.co/datasets/tiiuae/falcon-refinedweb)
+  - [StarCoder (en)](https://huggingface.co/datasets/bigcode/starcoderdata)
+  - [Wikipedia (en)](https://huggingface.co/datasets/olm/olm-wikipedia-20221220)
+  - [Wikipedia (zh)](https://huggingface.co/datasets/pleisto/wikipedia-cn-20230720-filtered)
 - For supervised fine-tuning:
   - [Stanford Alpaca (en)](https://github.com/tatsu-lab/stanford_alpaca)
   - [Stanford Alpaca (zh)](https://github.com/ymcui/Chinese-LLaMA-Alpaca)
   - [GPT-4 Generated Data (en&zh)](https://github.com/Instruction-Tuning-with-GPT-4/GPT-4-LLM)
   - [Open Assistant (multilingual)](https://huggingface.co/datasets/OpenAssistant/oasst1)
   - [Self-cognition (zh)](data/self_cognition.json)
   - [ShareGPT (zh)](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT/tree/main/Chinese-instruction-collection)
@@ -97,14 +107,15 @@
   - [BELLE 2M (zh)](https://huggingface.co/datasets/BelleGroup/train_2M_CN)
   - [BELLE 1M (zh)](https://huggingface.co/datasets/BelleGroup/train_1M_CN)
   - [BELLE 0.5M (zh)](https://huggingface.co/datasets/BelleGroup/train_0.5M_CN)
   - [BELLE Dialogue 0.4M (zh)](https://huggingface.co/datasets/BelleGroup/generated_chat_0.4M)
   - [BELLE School Math 0.25M (zh)](https://huggingface.co/datasets/BelleGroup/school_math_0.25M)
   - [BELLE Multiturn Chat 0.8M (zh)](https://huggingface.co/datasets/BelleGroup/multiturn_chat_0.8M)
   - [Firefly 1.1M (zh)](https://huggingface.co/datasets/YeungNLP/firefly-train-1.1M)
+  - [LIMA (en)](https://huggingface.co/datasets/GAIR/lima)
   - [CodeAlpaca 20k (en)](https://huggingface.co/datasets/sahil2801/CodeAlpaca-20k)
   - [Alpaca CoT (multilingual)](https://huggingface.co/datasets/QingyiSi/Alpaca-CoT)
   - [Web QA (zh)](https://huggingface.co/datasets/suolyer/webqa)
   - [UltraChat (en)](https://github.com/thunlp/UltraChat)
   - [WebNovel (zh)](https://huggingface.co/datasets/zxbsmk/webnovel_cn)
 - For reward modelling:
   - [HH-RLHF (en)](https://huggingface.co/datasets/Anthropic/hh-rlhf)
@@ -126,52 +137,56 @@
 - 🤗Transformers, Datasets, Accelerate, PEFT and TRL
 - jieba, rouge-chinese and nltk (used at evaluation)
 - gradio and matplotlib (used in web_demo.py)
 - uvicorn, fastapi and sse-starlette (used in api_demo.py)
 
 And **powerful GPUs**!
 
-If you want to enable quantized LoRA (QLoRA) on the Windows platform, you should install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.1.
-
-```bash
-pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.39.1-py3-none-win_amd64.whl
-```
-
 ## Getting Started
 
 ### Data Preparation (optional)
 
 Please refer to `data/example_dataset` for checking the details about the format of dataset files. You can either use a single `.json` file or a [dataset loading script](https://huggingface.co/docs/datasets/dataset_script) with multiple files to create a custom dataset.
 
 Note: please update `data/dataset_info.json` to use your custom dataset. About the format of this file, please refer to `data/README.md`.
 
 ### Dependence Installation (optional)
 
 ```bash
+git lfs install
 git clone https://github.com/hiyouga/LLaMA-Efficient-Tuning.git
 conda create -n llama_etuning python=3.10
 conda activate llama_etuning
 cd LLaMA-Efficient-Tuning
 pip install -r requirements.txt
 ```
 
+If you want to enable the quantized LoRA (QLoRA) on the Windows platform, you will be required to install a pre-built version of `bitsandbytes` library, which supports CUDA 11.1 to 12.1.
+
+```bash
+pip install https://github.com/jllllll/bitsandbytes-windows-webui/releases/download/wheels/bitsandbytes-0.39.1-py3-none-win_amd64.whl
+```
+
 ### All-in-one Web UI
 
 ```bash
-python src/train_web.py
+CUDA_VISIBLE_DEVICES=0 python src/train_web.py
 ```
 
+Currently the web UI only supports training on **a single GPU**.
+
 ### (Continually) Pre-Training
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage pt \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset wiki_demo \
+    --template default \
     --finetuning_type lora \
     --output_dir path_to_pt_checkpoint \
     --overwrite_cache \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
     --logging_steps 10 \
@@ -186,37 +201,43 @@
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset alpaca_gpt4_en \
+    --template default \
     --finetuning_type lora \
     --output_dir path_to_sft_checkpoint \
     --overwrite_cache \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
     --logging_steps 10 \
     --save_steps 1000 \
     --learning_rate 5e-5 \
     --num_train_epochs 3.0 \
     --plot_loss \
     --fp16
 ```
 
+Remember to specify `--lora_target W_pack` if you are using Baichuan models.
+
 ### Reward Model Training
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage rm \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset comparison_gpt4_en \
+    --template default \
     --finetuning_type lora \
+    --resume_lora_training False \
+    --checkpoint_dir path_to_sft_checkpoint \
     --output_dir path_to_rm_checkpoint \
     --per_device_train_batch_size 4 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
     --logging_steps 10 \
     --save_steps 1000 \
     --learning_rate 1e-5 \
@@ -229,26 +250,27 @@
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage ppo \
     --model_name_or_path path_to_your_model \
     --do_train \
     --dataset alpaca_gpt4_en \
+    --template default \
     --finetuning_type lora \
+    --resume_lora_training False \
     --checkpoint_dir path_to_sft_checkpoint \
     --reward_model path_to_rm_checkpoint \
     --output_dir path_to_ppo_checkpoint \
     --per_device_train_batch_size 2 \
     --gradient_accumulation_steps 4 \
     --lr_scheduler_type cosine \
     --logging_steps 10 \
     --save_steps 1000 \
     --learning_rate 1e-5 \
     --num_train_epochs 1.0 \
-    --resume_lora_training False \
     --plot_loss
 ```
 
 ### Distributed Training
 
 ```bash
 accelerate config # configure the environment
@@ -287,14 +309,15 @@
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
     --model_name_or_path path_to_your_model \
     --do_eval \
     --dataset alpaca_gpt4_en \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_eval_result \
     --per_device_eval_batch_size 8 \
     --max_samples 100 \
     --predict_with_generate
 ```
@@ -305,74 +328,83 @@
 
 ```bash
 CUDA_VISIBLE_DEVICES=0 python src/train_bash.py \
     --stage sft \
     --model_name_or_path path_to_your_model \
     --do_predict \
     --dataset alpaca_gpt4_en \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_predict_result \
     --per_device_eval_batch_size 8 \
     --max_samples 100 \
     --predict_with_generate
 ```
 
-If you want to predict the samples with empty responses, please kindly fill the `response` column with **dummy tokens** to ensure the sample will not be discarded throughout the preprocessing phase.
-
 ### API Demo
 
 ```bash
 python src/api_demo.py \
     --model_name_or_path path_to_your_model \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 Visit `http://localhost:8000/docs` for API documentation.
 
 ### CLI Demo
 
 ```bash
 python src/cli_demo.py \
     --model_name_or_path path_to_your_model \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Web Demo
 
 ```bash
 python src/web_demo.py \
     --model_name_or_path path_to_your_model \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint
 ```
 
 ### Export model
 
 ```bash
 python src/export_model.py \
     --model_name_or_path path_to_your_model \
+    --template default \
     --finetuning_type lora \
     --checkpoint_dir path_to_checkpoint \
     --output_dir path_to_export
 ```
 
+## TODO
+
+- [ ] Supporting flash attention ([torch](https://pytorch.org/docs/stable/generated/torch.nn.functional.scaled_dot_product_attention.html) / [xformers](https://github.com/facebookresearch/xformers) / [flashattn](https://github.com/Dao-AILab/flash-attention)).
+- [ ] Implementing multi-query attention for faster inference.
+- [ ] Supporting full-parameter RLHF training.
+
 ## License
 
 This repository is licensed under the [Apache-2.0 License](LICENSE).
 
 Please follow the model licenses to use the corresponding model weights:
 
 - [LLaMA](https://github.com/facebookresearch/llama/blob/main/MODEL_CARD.md)
 - [LLaMA-2](https://ai.meta.com/llama/license/)
 - [BLOOM](https://huggingface.co/spaces/bigscience/license)
 - [Falcon](LICENSE)
-- [baichuan](https://huggingface.co/baichuan-inc/baichuan-7B/resolve/main/baichuan-7B%20%E6%A8%A1%E5%9E%8B%E8%AE%B8%E5%8F%AF%E5%8D%8F%E8%AE%AE.pdf)
+- [Baichuan](https://huggingface.co/baichuan-inc/baichuan-7B/resolve/main/baichuan-7B%20%E6%A8%A1%E5%9E%8B%E8%AE%B8%E5%8F%AF%E5%8D%8F%E8%AE%AE.pdf)
 - [InternLM](https://github.com/InternLM/InternLM#open-source-license)
 
 ## Citation
 
 If this work is helpful, please kindly cite as:
 
 ```bibtex
```

### Comparing `llmtuner-0.1.4/src/llmtuner.egg-info/SOURCES.txt` & `llmtuner-0.1.5/src/llmtuner.egg-info/SOURCES.txt`

 * *Files identical despite different names*

