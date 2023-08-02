# Comparing `tmp/gentopia-0.0.1.tar.gz` & `tmp/gentopia-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gentopia-0.0.1.tar", last modified: Thu Jul 27 06:20:26 2023, max compression
+gzip compressed data, was "gentopia-0.0.2.tar", last modified: Tue Aug  1 23:57:35 2023, max compression
```

## Comparing `gentopia-0.0.1.tar` & `gentopia-0.0.2.tar`

### file list

```diff
@@ -1,161 +1,161 @@
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.580340 gentopia-0.0.1/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    11357 2023-06-10 13:57:28.000000 gentopia-0.0.1/LICENSE
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5708 2023-07-27 06:20:26.580340 gentopia-0.0.1/PKG-INFO
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5348 2023-07-27 05:14:23.000000 gentopia-0.0.1/README.md
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      970 2023-07-15 05:02:37.000000 gentopia-0.0.1/gentopia/__init__.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/agent/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       33 2023-07-03 16:27:20.000000 gentopia-0.0.1/gentopia/agent/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3490 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/agent/base_agent.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/agent/openai/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       42 2023-06-22 05:41:38.000000 gentopia-0.0.1/gentopia/agent/openai/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     9156 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/agent/openai/agent.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/agent/openai_memory/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       40 2023-07-10 23:23:40.000000 gentopia-0.0.1/gentopia/agent/openai_memory/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    10125 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/agent/openai_memory/agent.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1195 2023-07-15 14:57:36.000000 gentopia-0.0.1/gentopia/agent/openai_memory/load_memory.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1353 2023-07-27 03:24:25.000000 gentopia-0.0.1/gentopia/agent/plugin_manager.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/agent/react/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       30 2023-06-16 00:45:03.000000 gentopia-0.0.1/gentopia/agent/react/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     9794 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/agent/react/agent.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/agent/rewoo/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       30 2023-06-16 00:45:03.000000 gentopia-0.0.1/gentopia/agent/rewoo/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    14079 2023-07-27 03:25:32.000000 gentopia-0.0.1/gentopia/agent/rewoo/agent.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/agent/rewoo/nodes/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3270 2023-07-08 05:17:15.000000 gentopia-0.0.1/gentopia/agent/rewoo/nodes/Planner.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2677 2023-07-08 05:17:15.000000 gentopia-0.0.1/gentopia/agent/rewoo/nodes/Solver.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-06-13 13:12:30.000000 gentopia-0.0.1/gentopia/agent/rewoo/nodes/__init__.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/agent/vanilla/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       32 2023-06-16 00:45:03.000000 gentopia-0.0.1/gentopia/agent/vanilla/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5055 2023-07-15 14:57:36.000000 gentopia-0.0.1/gentopia/agent/vanilla/agent.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/assembler/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)       30 2023-07-06 14:53:35.000000 gentopia-0.0.1/gentopia/assembler/__init__.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     9849 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/assembler/agent_assembler.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     2637 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/assembler/config.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     4069 2023-07-15 14:57:36.000000 gentopia-0.0.1/gentopia/assembler/loader.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      671 2023-07-15 14:57:36.000000 gentopia-0.0.1/gentopia/assembler/task.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/llm/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      169 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/llm/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      771 2023-06-21 06:58:48.000000 gentopia-0.0.1/gentopia/llm/base_llm.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/llm/client/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      155 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/llm/client/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    10652 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/llm/client/huggingface.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    12848 2023-07-15 14:57:36.000000 gentopia-0.0.1/gentopia/llm/client/openai.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2347 2023-07-15 14:57:36.000000 gentopia-0.0.1/gentopia/llm/llm_info.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/llm/loaders/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      550 2023-06-20 04:55:33.000000 gentopia-0.0.1/gentopia/llm/loaders/airoboros.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      943 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/alpaca.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      943 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/baize.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      882 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/bloom.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      585 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/camel.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      519 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/falcon.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      732 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/flan_alpaca.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      951 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/guanaco.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      446 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/kullm.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      545 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/mpt.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      545 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/redpajama.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1019 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/replit.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      549 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/samantha_vicuna.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      647 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/stablelm.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      482 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/starchat.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      599 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/t5_vicuna.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      689 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/llm/loaders/vicuna.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      762 2023-06-20 04:55:33.000000 gentopia-0.0.1/gentopia/llm/test_llm.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1837 2023-07-08 05:17:15.000000 gentopia-0.0.1/gentopia/llm/wrap_llm.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/manager/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-20 04:55:33.000000 gentopia-0.0.1/gentopia/manager/__init__.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      853 2023-06-20 04:55:33.000000 gentopia-0.0.1/gentopia/manager/base_llm_manager.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/manager/llm_client/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-20 04:55:33.000000 gentopia-0.0.1/gentopia/manager/llm_client/__init__.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      559 2023-06-20 04:55:33.000000 gentopia-0.0.1/gentopia/manager/llm_client/base_llm_client.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1784 2023-06-20 04:55:33.000000 gentopia-0.0.1/gentopia/manager/llm_client/local_llm_client.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3418 2023-06-20 04:55:33.000000 gentopia-0.0.1/gentopia/manager/local_llm_manager.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      359 2023-06-20 04:55:33.000000 gentopia-0.0.1/gentopia/manager/server_info.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/memory/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-07-10 23:23:40.000000 gentopia-0.0.1/gentopia/memory/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     8872 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/memory/api.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1323 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/memory/base_memory.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      238 2023-07-10 23:23:40.000000 gentopia-0.0.1/gentopia/memory/document.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    17492 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/memory/embeddings.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5492 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/memory/serializable.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5236 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/memory/utils.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/memory/vectorstores/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:19:02.000000 gentopia-0.0.1/gentopia/memory/vectorstores/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    15210 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/memory/vectorstores/chroma.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    14915 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/memory/vectorstores/pinecone.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    29000 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/memory/vectorstores/vectorstore.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia/model/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       85 2023-07-03 16:27:20.000000 gentopia-0.0.1/gentopia/model/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1436 2023-07-10 23:23:40.000000 gentopia-0.0.1/gentopia/model/agent_model.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      715 2023-07-06 14:53:35.000000 gentopia-0.0.1/gentopia/model/completion_model.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1658 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/model/param_model.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.580340 gentopia-0.0.1/gentopia/output/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      967 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/output/__init__.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     6529 2023-07-15 14:57:33.000000 gentopia-0.0.1/gentopia/output/base_output.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     5513 2023-07-15 14:57:33.000000 gentopia-0.0.1/gentopia/output/console_output.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3383 2023-07-15 14:57:33.000000 gentopia-0.0.1/gentopia/output/print_output.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.580340 gentopia-0.0.1/gentopia/prompt/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      128 2023-07-27 03:40:32.000000 gentopia-0.0.1/gentopia/prompt/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1341 2023-07-27 05:33:19.000000 gentopia-0.0.1/gentopia/prompt/prompt_template.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      824 2023-07-27 03:40:32.000000 gentopia-0.0.1/gentopia/prompt/react.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3720 2023-07-27 03:40:32.000000 gentopia-0.0.1/gentopia/prompt/rewoo.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      198 2023-07-12 12:18:52.000000 gentopia-0.0.1/gentopia/prompt/tmp.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      286 2023-07-15 14:57:36.000000 gentopia-0.0.1/gentopia/prompt/vanilla.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.580340 gentopia-0.0.1/gentopia/resource/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-06-16 14:36:29.000000 gentopia-0.0.1/gentopia/resource/__init__.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.580340 gentopia-0.0.1/gentopia/tools/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1289 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/tools/__init__.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1665 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/tools/arxiv_search.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     9037 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/tools/basetool.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5998 2023-07-27 03:40:32.000000 gentopia-0.0.1/gentopia/tools/bing_search.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1488 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/tools/calculator.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1743 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/tools/code_interpreter.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1902 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/tools/file_operation.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      855 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/tools/google_search.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3542 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/tools/gradio.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.580340 gentopia-0.0.1/gentopia/tools/gradio_tools/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-07-01 23:00:56.000000 gentopia-0.0.1/gentopia/tools/gradio_tools/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2155 2023-07-12 12:18:52.000000 gentopia-0.0.1/gentopia/tools/gradio_tools/api.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.580340 gentopia-0.0.1/gentopia/tools/gradio_tools/tools/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1244 2023-07-12 12:18:52.000000 gentopia-0.0.1/gentopia/tools/gradio_tools/tools/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3514 2023-07-15 14:57:33.000000 gentopia-0.0.1/gentopia/tools/gradio_tools/tools/bark.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1074 2023-07-12 12:18:52.000000 gentopia-0.0.1/gentopia/tools/gradio_tools/tools/clip_interrogator.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1152 2023-07-12 12:18:52.000000 gentopia-0.0.1/gentopia/tools/gradio_tools/tools/document_qa.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3326 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/tools/gradio_tools/tools/gradio_tool.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1138 2023-07-12 12:18:52.000000 gentopia-0.0.1/gentopia/tools/gradio_tools/tools/image_captioning.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1187 2023-07-12 12:18:52.000000 gentopia-0.0.1/gentopia/tools/gradio_tools/tools/image_to_music.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1028 2023-07-12 12:18:52.000000 gentopia-0.0.1/gentopia/tools/gradio_tools/tools/prompt_generator.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2352 2023-07-12 12:18:52.000000 gentopia-0.0.1/gentopia/tools/gradio_tools/tools/sam_with_clip.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1371 2023-07-12 12:18:52.000000 gentopia-0.0.1/gentopia/tools/gradio_tools/tools/stable_diffusion.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1021 2023-07-12 12:18:52.000000 gentopia-0.0.1/gentopia/tools/gradio_tools/tools/text_to_video.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1037 2023-07-12 12:18:52.000000 gentopia-0.0.1/gentopia/tools/gradio_tools/tools/whisper.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1100 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/tools/search_doc.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     4952 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/tools/shell.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.580340 gentopia-0.0.1/gentopia/tools/utils/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)       23 2023-07-13 14:37:51.000000 gentopia-0.0.1/gentopia/tools/utils/__init__.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     2355 2023-07-13 14:37:51.000000 gentopia-0.0.1/gentopia/tools/utils/docstore.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.580340 gentopia-0.0.1/gentopia/tools/utils/document_loaders/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/tools/utils/document_loaders/__init__.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1639 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/tools/utils/document_loaders/base_loader.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      737 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/tools/utils/document_loaders/text_loader.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)    16131 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/tools/utils/document_loaders/text_splitter.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1579 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/tools/utils/vector_store.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     6101 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/tools/weather.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1298 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/tools/web_page.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     2316 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/tools/wikipedia.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1482 2023-07-27 03:27:55.000000 gentopia-0.0.1/gentopia/tools/wolfram_alpha.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.580340 gentopia-0.0.1/gentopia/utils/
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-24 07:59:31.000000 gentopia-0.0.1/gentopia/utils/__init__.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      688 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/utils/cost_helpers.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-24 07:59:31.000000 gentopia-0.0.1/gentopia/utils/display_utils.py
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      878 2023-07-23 00:45:38.000000 gentopia-0.0.1/gentopia/utils/text_helpers.py
--rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1690 2023-07-27 03:40:32.000000 gentopia-0.0.1/gentopia/utils/util.py
-drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:20:26.576340 gentopia-0.0.1/gentopia.egg-info/
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5708 2023-07-27 06:20:26.000000 gentopia-0.0.1/gentopia.egg-info/PKG-INFO
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     4390 2023-07-27 06:20:26.000000 gentopia-0.0.1/gentopia.egg-info/SOURCES.txt
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        1 2023-07-27 06:20:26.000000 gentopia-0.0.1/gentopia.egg-info/dependency_links.txt
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      276 2023-07-27 06:20:26.000000 gentopia-0.0.1/gentopia.egg-info/requires.txt
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        9 2023-07-27 06:20:26.000000 gentopia-0.0.1/gentopia.egg-info/top_level.txt
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       38 2023-07-27 06:20:26.580340 gentopia-0.0.1/setup.cfg
--rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1132 2023-07-27 05:54:56.000000 gentopia-0.0.1/setup.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.802369 gentopia-0.0.2/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1067 2023-07-29 06:32:27.000000 gentopia-0.0.2/LICENSE
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     7234 2023-08-01 23:57:35.802369 gentopia-0.0.2/PKG-INFO
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     6881 2023-08-01 23:57:15.000000 gentopia-0.0.2/README.md
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.786369 gentopia-0.0.2/gentopia/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      970 2023-07-15 05:02:37.000000 gentopia-0.0.2/gentopia/__init__.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.786369 gentopia-0.0.2/gentopia/agent/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       33 2023-07-03 16:27:20.000000 gentopia-0.0.2/gentopia/agent/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3490 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/agent/base_agent.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.786369 gentopia-0.0.2/gentopia/agent/openai/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       42 2023-06-22 05:41:38.000000 gentopia-0.0.2/gentopia/agent/openai/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     9156 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/agent/openai/agent.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.786369 gentopia-0.0.2/gentopia/agent/openai_memory/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       40 2023-07-10 23:23:40.000000 gentopia-0.0.2/gentopia/agent/openai_memory/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    10125 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/agent/openai_memory/agent.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1195 2023-07-15 14:57:36.000000 gentopia-0.0.2/gentopia/agent/openai_memory/load_memory.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1353 2023-07-27 03:24:25.000000 gentopia-0.0.2/gentopia/agent/plugin_manager.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.786369 gentopia-0.0.2/gentopia/agent/react/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       30 2023-06-16 00:45:03.000000 gentopia-0.0.2/gentopia/agent/react/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     9794 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/agent/react/agent.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.786369 gentopia-0.0.2/gentopia/agent/rewoo/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       30 2023-06-16 00:45:03.000000 gentopia-0.0.2/gentopia/agent/rewoo/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    14079 2023-07-27 03:25:32.000000 gentopia-0.0.2/gentopia/agent/rewoo/agent.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.790369 gentopia-0.0.2/gentopia/agent/rewoo/nodes/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3270 2023-07-08 05:17:15.000000 gentopia-0.0.2/gentopia/agent/rewoo/nodes/Planner.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2677 2023-07-08 05:17:15.000000 gentopia-0.0.2/gentopia/agent/rewoo/nodes/Solver.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-06-13 13:12:30.000000 gentopia-0.0.2/gentopia/agent/rewoo/nodes/__init__.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.790369 gentopia-0.0.2/gentopia/agent/vanilla/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       32 2023-06-16 00:45:03.000000 gentopia-0.0.2/gentopia/agent/vanilla/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5055 2023-07-15 14:57:36.000000 gentopia-0.0.2/gentopia/agent/vanilla/agent.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.790369 gentopia-0.0.2/gentopia/assembler/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)       30 2023-07-06 14:53:35.000000 gentopia-0.0.2/gentopia/assembler/__init__.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     9849 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/assembler/agent_assembler.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     2637 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/assembler/config.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     4069 2023-07-15 14:57:36.000000 gentopia-0.0.2/gentopia/assembler/loader.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      671 2023-07-15 14:57:36.000000 gentopia-0.0.2/gentopia/assembler/task.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.790369 gentopia-0.0.2/gentopia/llm/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      169 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/llm/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      771 2023-06-21 06:58:48.000000 gentopia-0.0.2/gentopia/llm/base_llm.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.790369 gentopia-0.0.2/gentopia/llm/client/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      155 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/llm/client/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    10652 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/llm/client/huggingface.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    12848 2023-07-15 14:57:36.000000 gentopia-0.0.2/gentopia/llm/client/openai.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2347 2023-07-15 14:57:36.000000 gentopia-0.0.2/gentopia/llm/llm_info.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.794369 gentopia-0.0.2/gentopia/llm/loaders/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      550 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/llm/loaders/airoboros.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      943 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/alpaca.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      943 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/baize.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      882 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/bloom.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      585 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/camel.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      519 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/falcon.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      732 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/flan_alpaca.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      951 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/guanaco.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      446 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/kullm.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      545 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/mpt.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      545 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/redpajama.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1019 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/replit.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      549 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/samantha_vicuna.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      647 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/stablelm.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      482 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/starchat.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      599 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/t5_vicuna.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      689 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/llm/loaders/vicuna.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      762 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/llm/test_llm.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1837 2023-07-08 05:17:15.000000 gentopia-0.0.2/gentopia/llm/wrap_llm.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.794369 gentopia-0.0.2/gentopia/manager/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/manager/__init__.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      853 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/manager/base_llm_manager.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.794369 gentopia-0.0.2/gentopia/manager/llm_client/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/manager/llm_client/__init__.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      559 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/manager/llm_client/base_llm_client.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1784 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/manager/llm_client/local_llm_client.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3418 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/manager/local_llm_manager.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      359 2023-06-20 04:55:33.000000 gentopia-0.0.2/gentopia/manager/server_info.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.794369 gentopia-0.0.2/gentopia/memory/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-07-10 23:23:40.000000 gentopia-0.0.2/gentopia/memory/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     8872 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/api.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1323 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/base_memory.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      238 2023-07-10 23:23:40.000000 gentopia-0.0.2/gentopia/memory/document.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    17492 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/embeddings.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5492 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/serializable.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5236 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/utils.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.794369 gentopia-0.0.2/gentopia/memory/vectorstores/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-07-27 06:32:36.000000 gentopia-0.0.2/gentopia/memory/vectorstores/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    15210 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/vectorstores/chroma.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    14915 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/vectorstores/pinecone.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)    29000 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/memory/vectorstores/vectorstore.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.794369 gentopia-0.0.2/gentopia/model/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       85 2023-07-03 16:27:20.000000 gentopia-0.0.2/gentopia/model/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1436 2023-07-10 23:23:40.000000 gentopia-0.0.2/gentopia/model/agent_model.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      715 2023-07-06 14:53:35.000000 gentopia-0.0.2/gentopia/model/completion_model.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1658 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/model/param_model.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.794369 gentopia-0.0.2/gentopia/output/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      967 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/output/__init__.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     6529 2023-07-15 14:57:33.000000 gentopia-0.0.2/gentopia/output/base_output.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     5513 2023-07-15 14:57:33.000000 gentopia-0.0.2/gentopia/output/console_output.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3383 2023-07-15 14:57:33.000000 gentopia-0.0.2/gentopia/output/print_output.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.798370 gentopia-0.0.2/gentopia/prompt/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      128 2023-07-27 03:40:32.000000 gentopia-0.0.2/gentopia/prompt/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1341 2023-07-27 05:33:19.000000 gentopia-0.0.2/gentopia/prompt/prompt_template.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      824 2023-07-27 03:40:32.000000 gentopia-0.0.2/gentopia/prompt/react.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3720 2023-07-27 03:40:32.000000 gentopia-0.0.2/gentopia/prompt/rewoo.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      198 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/prompt/tmp.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      286 2023-07-15 14:57:36.000000 gentopia-0.0.2/gentopia/prompt/vanilla.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.798370 gentopia-0.0.2/gentopia/resource/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-06-16 14:36:29.000000 gentopia-0.0.2/gentopia/resource/__init__.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.798370 gentopia-0.0.2/gentopia/tools/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1289 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/__init__.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1665 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/arxiv_search.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     9037 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/tools/basetool.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     5998 2023-07-27 03:40:32.000000 gentopia-0.0.2/gentopia/tools/bing_search.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1488 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/calculator.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1743 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/code_interpreter.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1902 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/file_operation.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      855 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/google_search.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     3542 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/gradio.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.798370 gentopia-0.0.2/gentopia/tools/gradio_tools/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        0 2023-07-01 23:00:56.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2155 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/api.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.798370 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1244 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3514 2023-07-15 14:57:33.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/bark.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1074 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/clip_interrogator.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1152 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/document_qa.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     3326 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/gradio_tool.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1138 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/image_captioning.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1187 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/image_to_music.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1028 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/prompt_generator.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     2352 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/sam_with_clip.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1371 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/stable_diffusion.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1021 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/text_to_video.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1037 2023-07-12 12:18:52.000000 gentopia-0.0.2/gentopia/tools/gradio_tools/tools/whisper.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1100 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/search_doc.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     4952 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/shell.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.798370 gentopia-0.0.2/gentopia/tools/utils/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)       23 2023-07-13 14:37:51.000000 gentopia-0.0.2/gentopia/tools/utils/__init__.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     2355 2023-07-13 14:37:51.000000 gentopia-0.0.2/gentopia/tools/utils/docstore.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.802369 gentopia-0.0.2/gentopia/tools/utils/document_loaders/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/tools/utils/document_loaders/__init__.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1639 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/tools/utils/document_loaders/base_loader.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)      737 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/tools/utils/document_loaders/text_loader.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)    16131 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/tools/utils/document_loaders/text_splitter.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1579 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/tools/utils/vector_store.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     6101 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/weather.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1298 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/web_page.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     2316 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/wikipedia.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1482 2023-07-27 03:27:55.000000 gentopia-0.0.2/gentopia/tools/wolfram_alpha.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.802369 gentopia-0.0.2/gentopia/utils/
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-24 07:59:31.000000 gentopia-0.0.2/gentopia/utils/__init__.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      688 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/utils/cost_helpers.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-06-24 07:59:31.000000 gentopia-0.0.2/gentopia/utils/display_utils.py
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      878 2023-07-23 00:45:38.000000 gentopia-0.0.2/gentopia/utils/text_helpers.py
+-rwxrwxr-x   0 billxbf   (1000) billxbf   (1000)     1690 2023-07-27 03:40:32.000000 gentopia-0.0.2/gentopia/utils/util.py
+drwxrwxr-x   0 billxbf   (1000) billxbf   (1000)        0 2023-08-01 23:57:35.786369 gentopia-0.0.2/gentopia.egg-info/
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     7234 2023-08-01 23:57:35.000000 gentopia-0.0.2/gentopia.egg-info/PKG-INFO
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     4390 2023-08-01 23:57:35.000000 gentopia-0.0.2/gentopia.egg-info/SOURCES.txt
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        1 2023-08-01 23:57:35.000000 gentopia-0.0.2/gentopia.egg-info/dependency_links.txt
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)      308 2023-08-01 23:57:35.000000 gentopia-0.0.2/gentopia.egg-info/requires.txt
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)        9 2023-08-01 23:57:35.000000 gentopia-0.0.2/gentopia.egg-info/top_level.txt
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)       38 2023-08-01 23:57:35.802369 gentopia-0.0.2/setup.cfg
+-rw-rw-r--   0 billxbf   (1000) billxbf   (1000)     1190 2023-08-01 23:56:55.000000 gentopia-0.0.2/setup.py
```

### Comparing `gentopia-0.0.1/PKG-INFO` & `gentopia-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,357 +1,453 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 6765 6e74  : 2.1.Name: gent
 00000020: 6f70 6961 0a56 6572 7369 6f6e 3a20 302e  opia.Version: 0.
-00000030: 302e 310a 5375 6d6d 6172 793a 2047 656e  0.1.Summary: Gen
+00000030: 302e 320a 5375 6d6d 6172 793a 2047 656e  0.2.Summary: Gen
 00000040: 746f 7069 6120 7072 6f76 6964 6573 2065  topia provides e
 00000050: 7874 656e 7369 7665 2075 7469 6c69 7469  xtensive utiliti
 00000060: 6573 2074 6f20 6173 7365 6d62 6c65 7320  es to assembles 
 00000070: 414c 4d20 6167 656e 7473 2064 7269 7665  ALM agents drive
 00000080: 6e20 6279 2063 6f6e 6669 6773 2e0a 486f  n by configs..Ho
 00000090: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
 000000a0: 2f67 6974 6875 622e 636f 6d2f 4765 6e74  /github.com/Gent
 000000b0: 6f70 6961 2d41 492f 4765 6e74 6f70 6961  opia-AI/Gentopia
 000000c0: 0a41 7574 686f 723a 2062 696c 6c78 6266  .Author: billxbf
 000000d0: 0a41 7574 686f 722d 656d 6169 6c3a 2062  .Author-email: b
 000000e0: 696c 6c78 6266 4067 6d61 696c 2e63 6f6d  illxbf@gmail.com
-000000f0: 0a4c 6963 656e 7365 3a20 4170 6163 6865  .License: Apache
-00000100: 2d32 2e30 206c 6963 656e 7365 0a44 6573  -2.0 license.Des
-00000110: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-00000120: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-00000130: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
-00000140: 7472 613a 2068 7567 6769 6e67 6661 6365  tra: huggingface
-00000150: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
-00000160: 4943 454e 5345 0a0a 2320 4765 6e74 6f70  ICENSE..# Gentop
-00000170: 6961 200a 2a54 6865 2043 6f6c 6c65 6374  ia .*The Collect
-00000180: 6976 6520 4772 6f77 7468 206f 6620 496e  ive Growth of In
-00000190: 7465 6c6c 6967 656e 7420 4167 656e 7473  telligent Agents
-000001a0: 2e2a 20f0 9fa6 99f0 9f8c 8e0a 0a47 656e  .* ..........Gen
-000001b0: 746f 7069 6120 6973 2061 206c 6967 6874  topia is a light
-000001c0: 7765 6967 6874 2061 6e64 2065 7874 656e  weight and exten
-000001d0: 7369 626c 6520 6672 616d 6577 6f72 6b20  sible framework 
-000001e0: 666f 7220 4c4c 4d2d 6472 6976 656e 2041  for LLM-driven A
-000001f0: 6765 6e74 7320 616e 6420 5b41 4c4d 5d28  gents and [ALM](
-00000200: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00000210: 672f 6162 732f 3233 3032 2e30 3738 3432  g/abs/2302.07842
-00000220: 2920 2072 6573 6561 7263 682e 2049 7420  )  research. It 
-00000230: 7072 6f76 6964 6573 206d 756c 7469 706c  provides multipl
-00000240: 6520 6573 7365 6e74 6961 6c20 636f 6d70  e essential comp
-00000250: 6f6e 656e 7473 2074 6f20 6275 696c 642c  onents to build,
-00000260: 2074 6573 7420 616e 6420 6576 616c 7561   test and evalua
-00000270: 7465 2061 6765 6e74 732e 2041 7420 6974  te agents. At it
-00000280: 7320 636f 7265 2c20 4765 6e74 6f70 6961  s core, Gentopia
-00000290: 2061 696d 7320 746f 2065 6d62 6f64 7920   aims to embody 
-000002a0: 6167 656e 7473 2077 6974 6820 7369 6e67  agents with sing
-000002b0: 6c65 2063 6f6e 6669 6720 6669 6c65 732c  le config files,
-000002c0: 2074 6875 7320 6d69 6e69 6d69 7a69 6e67   thus minimizing
-000002d0: 2079 6f75 7220 6566 666f 7274 2069 6e20   your effort in 
-000002e0: 6d61 696e 7461 696e 696e 672c 2074 756e  maintaining, tun
-000002f0: 696e 672c 2061 6e64 2073 6861 7269 6e67  ing, and sharing
-00000300: 2061 6765 6e74 732e 0a0a 4765 6e74 6f70   agents...Gentop
-00000310: 6961 206d 6169 6e74 6169 6e73 2061 6e20  ia maintains an 
-00000320: 6167 656e 7420 7a6f 6f20 5b47 656e 7450  agent zoo [GentP
-00000330: 6f6f 6c5d 2868 7474 7073 3a2f 2f67 6974  ool](https://git
-00000340: 6875 622e 636f 6d2f 4765 6e74 6f70 6961  hub.com/Gentopia
-00000350: 2d41 492f 4765 6e74 506f 6f6c 2920 746f  -AI/GentPool) to
-00000360: 2073 6861 7265 2070 7562 6c69 6320 6167   share public ag
-00000370: 656e 7473 2073 7065 6369 616c 697a 6564  ents specialized
-00000380: 2066 6f72 2064 6966 6665 7265 6e74 2074   for different t
-00000390: 6173 6b73 2e20 496e 2074 6869 7320 706c  asks. In this pl
-000003a0: 6174 666f 726d 2c20 796f 7520 636f 756c  atform, you coul
-000003b0: 6420 6561 7369 6c79 202a 696e 7465 7261  d easily *intera
-000003c0: 6374 2a20 7769 7468 206f 7468 6572 2061  ct* with other a
-000003d0: 6765 6e74 7320 6279 2063 6c6f 6e69 6e67  gents by cloning
-000003e0: 2c20 6869 6572 6172 6368 6963 616c 2070  , hierarchical p
-000003f0: 6c75 672d 696e 2c20 6f72 2073 6861 7269  lug-in, or shari
-00000400: 6e67 2065 6e76 6972 6f6e 6d65 6e74 2e20  ng environment. 
-00000410: 5765 2061 6c73 6f20 6275 696c 6420 6120  We also build a 
-00000420: 756e 6971 7565 2061 6765 6e74 205b 6265  unique agent [be
-00000430: 6e63 686d 6172 6b5d 2868 7474 7073 3a2f  nchmark](https:/
-00000440: 2f67 656e 746f 7069 612e 7265 6164 7468  /gentopia.readth
-00000450: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00000460: 7374 2f67 656e 7470 6f6f 6c2e 6874 6d6c  st/gentpool.html
-00000470: 2361 6765 6e74 2d65 7661 6c75 6174 696f  #agent-evaluatio
-00000480: 6e29 2066 6f72 2068 6f6c 6973 7469 6320  n) for holistic 
-00000490: 414c 4d20 6576 616c 7561 7469 6f6e 2e20  ALM evaluation. 
-000004a0: 0a0a 2323 204d 6f74 6976 6174 696f 6e20  ..## Motivation 
-000004b0: f09f a7a0 0a41 6765 6e74 2070 7261 6374  .....Agent pract
-000004c0: 6974 696f 6e65 7273 2073 7461 7274 2074  itioners start t
-000004d0: 6f20 7265 616c 697a 6520 7468 6520 6469  o realize the di
-000004e0: 6666 6963 756c 7479 2069 6e20 7475 6e69  fficulty in tuni
-000004f0: 6e67 2061 2022 7765 6c6c 2d72 6f75 6e64  ng a "well-round
-00000500: 6564 2220 6167 656e 7420 7769 7468 2074  ed" agent with t
-00000510: 6f6e 7320 6f66 2074 6f6f 6c73 206f 7220  ons of tools or 
-00000520: 696e 7374 7275 6374 696f 6e73 2069 6e20  instructions in 
-00000530: 7369 6e67 6c65 206c 6179 6572 2e0a 5265  single layer..Re
-00000540: 6365 6e74 2073 7475 6469 6573 206c 696b  cent studies lik
-00000550: 6520 5b54 696e 7953 746f 7269 6573 5d28  e [TinyStories](
-00000560: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00000570: 672f 6162 732f 3233 3031 2e31 3237 3236  g/abs/2301.12726
-00000580: 292c 205b 5370 6563 6961 6c69 7a69 6e67  ), [Specializing
-00000590: 2052 6561 736f 6e69 6e67 5d28 6874 7470   Reasoning](http
-000005a0: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
-000005b0: 732f 3233 3031 2e31 3237 3236 292c 205b  s/2301.12726), [
-000005c0: 4c65 7427 7320 5665 7269 6679 2053 6253  Let's Verify SbS
-000005d0: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
-000005e0: 6f72 672f 6162 732f 3233 3035 2e32 3030  org/abs/2305.200
-000005f0: 3530 292c 205b 5265 574f 4f5d 2868 7474  50), [ReWOO](htt
-00000600: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
-00000610: 6273 2f32 3330 352e 3138 3332 3329 2c20  bs/2305.18323), 
-00000620: 6574 632e 2061 6c73 6f20 706f 696e 7420  etc. also point 
-00000630: 7573 2074 6f77 6172 6473 2061 6e20 696e  us towards an in
-00000640: 7475 6974 6976 6520 7965 7420 756e 6465  tuitive yet unde
-00000650: 7276 616c 7565 6420 6469 7265 6374 696f  rvalued directio
-00000660: 6e20 f09f 9189 200a 0a60 6060 0a41 6e20  n .... ..```.An 
-00000670: 4c4c 4d20 6973 206d 6f72 6520 6361 7061  LLM is more capa
-00000680: 626c 6520 6966 2079 6f75 2063 7265 6174  ble if you creat
-00000690: 6520 6120 636f 6e74 6578 742f 6469 7374  e a context/dist
-000006a0: 7269 6275 7469 6f6e 2073 6869 6674 2073  ribution shift s
-000006b0: 7065 6369 616c 697a 6564 2074 6f20 736f  pecialized to so
-000006c0: 6d65 2074 6172 6765 7420 7461 736b 732e  me target tasks.
-000006d0: 0a60 6060 0a53 6164 6c79 2c20 7468 6572  .```.Sadly, ther
-000006e0: 6520 6973 206e 6f20 7369 6c76 6572 2062  e is no silver b
-000006f0: 756c 6c65 7420 666f 7220 6167 656e 7420  ullet for agent 
-00000700: 7370 6563 6961 6c69 7a61 7469 6f6e 2e20  specialization. 
-00000710: 466f 7220 6578 616d 706c 652c 2079 6f75  For example, you
-00000720: 2063 616e 200a 2d20 5369 6d70 6c79 2061   can .- Simply a
-00000730: 6464 2060 4c65 7427 7320 7468 696e 6b20  dd `Let's think 
-00000740: 7374 6570 2062 7920 7374 6570 2e60 2069  step by step.` i
-00000750: 6e20 796f 7572 202a 2a70 726f 6d70 742a  n your **prompt*
-00000760: 2a20 666f 7220 6d6f 7265 2061 6363 7572  * for more accur
-00000770: 6174 6520 4d61 7468 2051 412e 0a2d 2047  ate Math QA..- G
-00000780: 6976 6520 6120 2a2a 6665 772d 7368 6f74  ive a **few-shot
-00000790: 2a2a 2065 7865 6d70 6c61 7220 696e 2079  ** exemplar in y
-000007a0: 6f75 7220 7072 6f6d 7074 2074 6f20 6775  our prompt to gu
-000007b0: 6964 6520 6120 6265 7474 6572 2072 6561  ide a better rea
-000007c0: 736f 6e69 6e67 2074 7261 6a65 6374 6f72  soning trajector
-000007d0: 7920 666f 7220 6e6f 7665 6c20 706c 6f74  y for novel plot
-000007e0: 7469 6e67 2e0a 2d20 5375 7065 7276 6973  ting..- Supervis
-000007f0: 6520 2a2a 6669 6e65 2d74 756e 696e 672a  e **fine-tuning*
-00000800: 2a20 2853 4654 2920 796f 7572 2037 3042  * (SFT) your 70B
-00000810: 2060 6c6c 616d 6132 6020 6c69 6b65 205b   `llama2` like [
-00000820: 7468 6973 5d28 6874 7470 733a 2f2f 6172  this](https://ar
-00000830: 7869 762e 6f72 672f 6162 732f 3233 3035  xiv.org/abs/2305
-00000840: 2e32 3030 3530 2920 746f 206d 6174 6368  .20050) to match
-00000850: 2072 6561 736f 6e69 6e67 206f 6620 3137   reasoning of 17
-00000860: 3542 2047 5054 2d33 2e35 2e0a 2d20 5475  5B GPT-3.5..- Tu
-00000870: 6e65 2079 6f75 7220 6167 656e 7420 2a2a  ne your agent **
-00000880: 7061 7261 6469 676d 2a2a 206c 696b 6520  paradigm** like 
-00000890: 7468 6973 205b 6465 6d6f 5d28 6874 7470  this [demo](http
-000008a0: 733a 2f2f 7777 772e 796f 7574 7562 652e  s://www.youtube.
-000008b0: 636f 6d2f 7761 7463 683f 763d 6469 4a34  com/watch?v=diJ4
-000008c0: 4944 6154 345a 3429 2074 6f20 6561 7369  IDaT4Z4) to easi
-000008d0: 6c79 2068 616c 6620 7468 6520 6578 6563  ly half the exec
-000008e0: 7574 696f 6e20 7469 6d65 2066 6f72 2053  ution time for S
-000008f0: 6561 6368 2026 2053 756d 6d61 7269 7a65  each & Summarize
-00000900: 2e0a 2d20 416e 6420 6d6f 7265 202e 2e2e  ..- And more ...
-00000910: 0a0a 4973 6e27 7420 6974 2062 6561 7574  ..Isn't it beaut
-00000920: 6966 756c 2069 6620 6f6e 6520 7368 6172  iful if one shar
-00000930: 6573 2068 6973 2073 7065 6369 616c 697a  es his specializ
-00000940: 6564 2069 6e74 656c 6c69 6765 6e63 652c  ed intelligence,
-00000950: 2061 6c6c 6f77 696e 6720 6f74 6865 7273   allowing others
-00000960: 2074 6f20 7265 7072 6f64 7563 652c 2062   to reproduce, b
-00000970: 7569 6c64 206f 6e2c 206f 7220 696e 7465  uild on, or inte
-00000980: 7261 6374 2077 6974 6820 6974 2061 7420  ract with it at 
-00000990: 6561 7365 3f20 f09f a497 2054 6869 7320  ease? .... This 
-000009a0: 6265 6c69 6566 2069 6e73 7069 7265 7320  belief inspires 
-000009b0: 7573 2074 6f20 6275 696c 6420 4765 6e74  us to build Gent
-000009c0: 6f70 6961 2c20 0a2a 2a64 6573 6967 6e65  opia, .**designe
-000009d0: 6420 666f 7220 6167 656e 7420 2a73 7065  d for agent *spe
-000009e0: 6369 616c 697a 6174 696f 6e2c 2073 6861  cialization, sha
-000009f0: 7269 6e67 2c20 616e 6420 696e 7465 7261  ring, and intera
-00000a00: 6374 696f 6e2c 2a20 746f 2061 6368 6965  ction,* to achie
-00000a10: 7665 2063 6f6c 6c65 6374 6976 6520 6772  ve collective gr
-00000a20: 6f77 7468 2074 6f77 6172 6473 2067 7265  owth towards gre
-00000a30: 6174 6572 2069 6e74 656c 6c69 6765 6e63  ater intelligenc
-00000a40: 652a 2a2e 0a0a 2323 2043 6f72 6520 4665  e**...## Core Fe
-00000a50: 6174 7572 6573 20f0 9f92 a10a 0a2d 20e2  atures ......- .
-00000a60: 9a99 efb8 8f20 436f 6e66 6967 2d64 7269  ..... Config-dri
-00000a70: 7665 6e20 6167 656e 7420 6173 7365 6d62  ven agent assemb
-00000a80: 6c69 6e67 2061 6e64 2063 6861 742e 0a2d  ling and chat..-
-00000a90: 20f0 9f9a 8020 4c61 7267 6520 616d 6f75   .... Large amou
-00000aa0: 6e74 206f 6620 7072 6562 7569 6c74 2061  nt of prebuilt a
-00000ab0: 6765 6e74 2074 7970 6573 2c20 4c4c 4d20  gent types, LLM 
-00000ac0: 636c 6965 6e74 732c 2074 6f6f 6c73 2c20  clients, tools, 
-00000ad0: 6d65 6d6f 7279 2073 7973 7465 6d73 2c20  memory systems, 
-00000ae0: 616e 6420 6d6f 7265 2e0a 2d20 f09f aab6  and more..- ....
-00000af0: 204c 6967 6874 7765 6967 6874 2061 6e64   Lightweight and
-00000b00: 2068 6967 686c 7920 6578 7465 6e73 6962   highly extensib
-00000b10: 6c65 2069 6d70 6c65 6d65 6e74 6174 696f  le implementatio
-00000b20: 6e20 6f66 2065 7373 656e 7469 616c 2063  n of essential c
-00000b30: 6f6d 706f 6e65 6e74 732e 0a2d 20f0 9fa7  omponents..- ...
-00000b40: aa20 416c 6967 6e69 6e67 2077 6974 6820  . Aligning with 
-00000b50: 7374 6174 652d 6f66 2d74 6865 2d61 7274  state-of-the-art
-00000b60: 2041 4920 7265 7365 6172 6368 2e0a 2d20   AI research..- 
-00000b70: f09f a49d 2045 6e61 626c 696e 6720 6d75  .... Enabling mu
-00000b80: 6c74 692d 6167 656e 7420 696e 7465 7261  lti-agent intera
-00000b90: 6374 696f 6e73 2e0a 2d20 f09f a681 2055  ctions..- .... U
-00000ba0: 6e69 7175 6520 706c 6174 666f 726d 206f  nique platform o
-00000bb0: 6620 6167 656e 7420 7a6f 6f20 616e 6420  f agent zoo and 
-00000bc0: 6576 616c 2062 656e 6368 6d61 726b 2e0a  eval benchmark..
-00000bd0: 0a23 2320 5175 6963 6b20 5374 6172 7420  .## Quick Start 
-00000be0: f09f 9bab 0a60 6060 0a70 6970 2069 6e73  .....```.pip ins
-00000bf0: 7461 6c6c 2067 656e 746f 7069 610a 6060  tall gentopia.``
-00000c00: 600a 6f72 2069 6620 796f 7520 7761 6e74  `.or if you want
-00000c10: 2074 6f20 6275 696c 6420 7769 7468 206f   to build with o
-00000c20: 7065 6e20 4c4c 4d73 206c 6f63 616c 6c79  pen LLMs locally
-00000c30: 20f0 9f91 8920 6070 6970 2069 6e73 7461   .... `pip insta
-00000c40: 6c6c 2067 656e 746f 7069 615b 6875 6767  ll gentopia[hugg
-00000c50: 696e 6766 6163 655d 600a 0a46 6972 7374  ingface]`..First
-00000c60: 2074 696d 6520 746f 2047 656e 746f 7069   time to Gentopi
-00000c70: 613f 2047 7261 6220 6120 636f 6666 6565  a? Grab a coffee
-00000c80: 20e2 9895 2061 6e64 2074 616b 6520 7e20   ... and take ~ 
-00000c90: 3130 206d 696e 7320 746f 2063 6865 636b  10 mins to check
-00000ca0: 206f 7574 2074 6865 2066 6f6c 6c6f 7769   out the followi
-00000cb0: 6e67 206d 696e 642d 626c 6f77 696e 6720  ng mind-blowing 
-00000cc0: 6465 6d6f 7320 f09f 9180 20f0 9fa4 af0a  demos .... .....
-00000cd0: 0a3c 6469 7620 7374 796c 653d 2264 6973  .<div style="dis
-00000ce0: 706c 6179 3a20 666c 6578 3b20 6a75 7374  play: flex; just
-00000cf0: 6966 792d 636f 6e74 656e 743a 2073 7061  ify-content: spa
-00000d00: 6365 2d61 726f 756e 643b 223e 0a20 200a  ce-around;">.  .
-00000d10: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000d20: 2f77 7777 2e79 6f75 7475 6265 2e63 6f6d  /www.youtube.com
-00000d30: 2f77 6174 6368 3f76 3d37 645a 335a 7673  /watch?v=7dZ3Zvs
-00000d40: 4937 7377 2220 7461 7267 6574 3d22 5f62  I7sw" target="_b
-00000d50: 6c61 6e6b 223e 0a20 203c 696d 6720 7372  lank">.  <img sr
-00000d60: 633d 2268 7474 7073 3a2f 2f69 6d67 2e79  c="https://img.y
-00000d70: 6f75 7475 6265 2e63 6f6d 2f76 692f 3764  outube.com/vi/7d
-00000d80: 5a33 5a76 7349 3773 772f 6871 6465 6661  Z3ZvsI7sw/hqdefa
-00000d90: 756c 742e 6a70 6722 2061 6c74 3d22 5669  ult.jpg" alt="Vi
-00000da0: 6465 6f20 3122 2073 7479 6c65 3d22 7769  deo 1" style="wi
-00000db0: 6474 683a 3332 253b 223e 0a3c 2f61 3e0a  dth:32%;">.</a>.
-00000dc0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-00000dd0: 2f2f 7777 772e 796f 7574 7562 652e 636f  //www.youtube.co
-00000de0: 6d2f 7761 7463 683f 763d 5854 7376 3970  m/watch?v=XTsv9p
-00000df0: 6b36 414f 4122 2074 6172 6765 743d 225f  k6AOA" target="_
-00000e00: 626c 616e 6b22 3e0a 2020 3c69 6d67 2073  blank">.  <img s
-00000e10: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000e20: 796f 7574 7562 652e 636f 6d2f 7669 2f58  youtube.com/vi/X
-00000e30: 5473 7639 706b 3641 4f41 2f68 7164 6566  Tsv9pk6AOA/hqdef
-00000e40: 6175 6c74 2e6a 7067 2220 616c 743d 2256  ault.jpg" alt="V
-00000e50: 6964 656f 2032 2220 7374 796c 653d 2277  ideo 2" style="w
-00000e60: 6964 7468 3a33 3225 3b22 3e0a 3c2f 613e  idth:32%;">.</a>
-00000e70: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-00000e80: 3a2f 2f77 7777 2e79 6f75 7475 6265 2e63  ://www.youtube.c
-00000e90: 6f6d 2f77 6174 6368 3f76 3d64 694a 3449  om/watch?v=diJ4I
-00000ea0: 4461 5434 5a34 2220 7461 7267 6574 3d22  DaT4Z4" target="
-00000eb0: 5f62 6c61 6e6b 223e 0a20 203c 696d 6720  _blank">.  <img 
-00000ec0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000ed0: 2e79 6f75 7475 6265 2e63 6f6d 2f76 692f  .youtube.com/vi/
-00000ee0: 6469 4a34 4944 6154 345a 342f 6871 6465  diJ4IDaT4Z4/hqde
-00000ef0: 6661 756c 742e 6a70 6722 2061 6c74 3d22  fault.jpg" alt="
-00000f00: 5669 6465 6f20 3322 2073 7479 6c65 3d22  Video 3" style="
-00000f10: 7769 6474 683a 3332 253b 223e 0a3c 2f61  width:32%;">.</a
-00000f20: 3e0a 0a3c 2f64 6976 3e0a 0a28 4a75 6d70  >..</div>..(Jump
-00000f30: 2074 6f20 7468 6520 7468 6972 6420 6f6e   to the third on
-00000f40: 6520 6966 2079 6f75 206f 6e6c 7920 6861  e if you only ha
-00000f50: 7665 2033 206d 696e 7320 f09f a4ab 290a  ve 3 mins ....).
-00000f60: 0a23 2320 446f 6375 6d65 6e74 6174 696f  .## Documentatio
-00000f70: 6e20 f09f 9396 0a53 6565 205b 6865 7265  n .....See [here
-00000f80: 5d28 6874 7470 733a 2f2f 6765 6e74 6f70  ](https://gentop
-00000f90: 6961 2e72 6561 6474 6865 646f 6373 2e69  ia.readthedocs.i
-00000fa0: 6f2f 656e 2f6c 6174 6573 742f 696e 6465  o/en/latest/inde
-00000fb0: 782e 6874 6d6c 2920 666f 7220 6675 6c6c  x.html) for full
-00000fc0: 2064 6f63 756d 656e 7461 7469 6f6e 2e0a   documentation..
-00000fd0: 0af0 9f8c 9f20 4869 6768 6c69 6768 7420  ..... Highlight 
-00000fe0: 546f 7069 6373 200a 2d20 5b41 6765 6e74  Topics .- [Agent
-00000ff0: 2054 656d 706c 6174 6573 5d28 6874 7470   Templates](http
-00001000: 733a 2f2f 6765 6e74 6f70 6961 2e72 6561  s://gentopia.rea
-00001010: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00001020: 6174 6573 742f 7175 6963 6b5f 7374 6172  atest/quick_star
-00001030: 742e 6874 6d6c 2376 616e 696c 6c61 2d61  t.html#vanilla-a
-00001040: 6765 6e74 290a 2d20 5b48 6965 7261 7263  gent).- [Hierarc
-00001050: 6869 6361 6c20 4167 656e 7473 5d28 6874  hical Agents](ht
-00001060: 7470 733a 2f2f 6765 6e74 6f70 6961 2e72  tps://gentopia.r
-00001070: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00001080: 2f6c 6174 6573 742f 6167 656e 745f 636f  /latest/agent_co
-00001090: 6d70 6f6e 656e 7473 2e68 746d 6c23 6167  mponents.html#ag
-000010a0: 656e 742d 6173 2d70 6c75 6769 6e29 0a2d  ent-as-plugin).-
-000010b0: 205b 556e 6971 7565 2041 6765 6e74 2042   [Unique Agent B
-000010c0: 656e 6368 6d61 726b 5d28 6874 7470 733a  enchmark](https:
-000010d0: 2f2f 6765 6e74 6f70 6961 2e72 6561 6474  //gentopia.readt
-000010e0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-000010f0: 6573 742f 6765 6e74 706f 6f6c 2e68 746d  est/gentpool.htm
-00001100: 6c23 6167 656e 742d 6576 616c 7561 7469  l#agent-evaluati
-00001110: 6f6e 290a 2d20 5b4f 7065 6e20 4c4c 4d20  on).- [Open LLM 
-00001120: 5375 7070 6f72 7473 5d28 6874 7470 733a  Supports](https:
-00001130: 2f2f 6765 6e74 6f70 6961 2e72 6561 6474  //gentopia.readt
-00001140: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00001150: 6573 742f 6167 656e 745f 636f 6d70 6f6e  est/agent_compon
-00001160: 656e 7473 2e68 746d 6c23 6875 6767 696e  ents.html#huggin
-00001170: 6766 6163 652d 6f70 656e 2d6c 6c6d 7329  gface-open-llms)
-00001180: 0a2d 205b 4869 6768 2d50 6572 666f 726d  .- [High-Perform
-00001190: 616e 6365 204d 656d 6f72 795d 2868 7474  ance Memory](htt
-000011a0: 7073 3a2f 2f67 656e 746f 7069 612e 7265  ps://gentopia.re
-000011b0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-000011c0: 6c61 7465 7374 2f61 6765 6e74 5f63 6f6d  latest/agent_com
-000011d0: 706f 6e65 6e74 732e 6874 6d6c 236c 6f6e  ponents.html#lon
-000011e0: 672d 7368 6f72 742d 7465 726d 2d6d 656d  g-short-term-mem
-000011f0: 6f72 7929 0a0a 2323 2042 7569 6c64 2077  ory)..## Build w
-00001200: 6974 6820 7573 20f0 9f8c 8e0a 0a50 6172  ith us ......Par
-00001210: 7469 6369 7061 7465 2069 6e20 7468 6973  ticipate in this
-00001220: 2055 746f 7069 6120 6f66 2073 7570 6572   Utopia of super
-00001230: 696e 7465 6c6c 6967 656e 6365 2061 6e64  intelligence and
-00001240: 2068 656c 7020 6974 2067 726f 7773 2120   help it grows! 
-00001250: 4173 2061 2066 756c 6c79 206f 7065 6e2d  As a fully open-
-00001260: 736f 7572 6365 2070 726f 6a65 6374 2c20  source project, 
-00001270: 7765 2064 6576 656c 6f70 2075 6e64 6572  we develop under
-00001280: 2070 7562 6c69 6320 6164 7669 6365 2c20   public advice, 
-00001290: 6964 6561 732c 2061 6e64 2073 7570 6572  ideas, and super
-000012a0: 7669 7369 6f6e 2e20 4d65 616e 7768 696c  vision. Meanwhil
-000012b0: 652c 2068 6572 6520 6172 6520 7761 7973  e, here are ways
-000012c0: 2079 6f75 206d 6179 2063 6f6e 7472 6962   you may contrib
-000012d0: 7574 6520 746f 2047 656e 746f 7069 612e  ute to Gentopia.
-000012e0: 0a0a 2d20 f09f 909b 2050 6f73 7420 616e  ..- .... Post an
-000012f0: 205b 6973 7375 655d 2868 7474 7073 3a2f   [issue](https:/
-00001300: 2f67 6974 6875 622e 636f 6d2f 4765 6e74  /github.com/Gent
-00001310: 6f70 6961 2d41 492f 4765 6e74 6f70 6961  opia-AI/Gentopia
-00001320: 2f69 7373 7565 7329 2072 6571 7565 7374  /issues) request
-00001330: 696e 6720 6e65 6365 7373 6172 7920 6275  ing necessary bu
-00001340: 6720 6669 7865 732c 2061 6464 6974 696f  g fixes, additio
-00001350: 6e61 6c20 6665 6174 7572 6573 2c20 6f72  nal features, or
-00001360: 2072 6f61 646d 6170 2073 7567 6765 7374   roadmap suggest
-00001370: 696f 6e73 2e20 2843 6865 636b 2063 6c6f  ions. (Check clo
-00001380: 7365 6420 6f6e 6573 2066 6972 7374 290a  sed ones first).
-00001390: 2d20 f09f 8eaf 204f 7572 2064 6576 2074  - .... Our dev t
-000013a0: 6561 6d20 6d65 6574 7320 7765 656b 6c79  eam meets weekly
-000013b0: 2074 6f20 6772 6f6f 6d20 5b62 6163 6b6c   to groom [backl
-000013c0: 6f67 5d28 6874 7470 733a 2f2f 6769 7468  og](https://gith
-000013d0: 7562 2e63 6f6d 2f6f 7267 732f 4765 6e74  ub.com/orgs/Gent
-000013e0: 6f70 6961 2d41 492f 7072 6f6a 6563 7473  opia-AI/projects
-000013f0: 2f31 2920 696e 746f 2074 6963 6b65 7473  /1) into tickets
-00001400: 2e20 5768 696c 6520 7765 2077 6f72 6b20  . While we work 
-00001410: 6f6e 2074 6865 6d2c 2079 6f75 2063 616e  on them, you can
-00001420: 2070 6963 6b20 7570 206f 7468 6572 7320   pick up others 
-00001430: 616e 6420 6372 6561 7465 2061 205b 5075  and create a [Pu
-00001440: 6c6c 2052 6571 7565 7374 5d28 6874 7470  ll Request](http
-00001450: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f47  s://github.com/G
-00001460: 656e 746f 7069 612d 4149 2f47 656e 746f  entopia-AI/Gento
-00001470: 7069 612f 7075 6c6c 7329 2074 6f20 7265  pia/pulls) to re
-00001480: 7175 6573 7420 6120 6d65 7267 652e 2057  quest a merge. W
-00001490: 6520 616c 7761 7973 2077 656c 636f 6d65  e always welcome
-000014a0: 206e 6577 206d 656d 6265 7273 2069 6e20   new members in 
-000014b0: 7468 6973 2077 6179 2e0a 2d20 f09f a49d  this way..- ....
-000014c0: 2053 6861 7265 2079 6f75 7220 7370 6563   Share your spec
-000014d0: 6961 6c69 7a65 6420 6167 656e 7420 746f  ialized agent to
-000014e0: 205b 4765 6e74 506f 6f6c 5d28 6874 7470   [GentPool](http
-000014f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f47  s://github.com/G
-00001500: 656e 746f 7069 612d 4149 2f47 656e 7450  entopia-AI/GentP
-00001510: 6f6f 6c29 2120 4372 6561 7465 2061 6e20  ool)! Create an 
-00001520: 4167 656e 7420 5052 2028 5b65 7861 6d70  Agent PR ([examp
-00001530: 6c65 5d28 2929 2074 6f20 6d65 7267 6520  le]()) to merge 
-00001540: 796f 7572 2077 656c 6c2d 7475 6e65 6420  your well-tuned 
-00001550: 6167 656e 7420 696e 746f 2074 6865 2070  agent into the p
-00001560: 6f6f 6c2e 2054 6869 7320 616c 6c6f 7773  ool. This allows
-00001570: 206f 7468 6572 7320 746f 2075 7365 206f   others to use o
-00001580: 7220 6275 696c 6420 7570 6f6e 2079 6f75  r build upon you
-00001590: 7220 6167 656e 742e 200a 2d20 e2ad 9020  r agent. .- ... 
-000015a0: 4865 6c70 2075 7320 7370 7265 6164 2120  Help us spread! 
-000015b0: 4769 7665 2075 7320 6120 7374 6172 2c20  Give us a star, 
-000015c0: 666f 6c6c 6f77 2075 7320 6f6e 205b 5477  follow us on [Tw
-000015d0: 6974 7465 725d 2868 7474 7073 3a2f 2f74  itter](https://t
-000015e0: 7769 7474 6572 2e63 6f6d 2f47 656e 746f  witter.com/Gento
-000015f0: 7069 6141 4929 2c20 6a6f 696e 206f 7572  piaAI), join our
-00001600: 205b 4469 7363 6f72 645d 2868 7474 7073   [Discord](https
-00001610: 3a2f 2f64 6973 636f 7264 2e67 672f 4153  ://discord.gg/AS
-00001620: 5050 394d 5939 514b 292c 2061 6e64 2073  PP9MY9QK), and s
-00001630: 6861 7265 2077 6974 6820 796f 7572 2066  hare with your f
-00001640: 7269 656e 6473 2120 200a 0a0a            riends!  ...
+000000f0: 0a4c 6963 656e 7365 3a20 4d49 5420 6c69  .License: MIT li
+00000100: 6365 6e73 650a 4465 7363 7269 7074 696f  cense.Descriptio
+00000110: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+00000120: 7465 7874 2f6d 6172 6b64 6f77 6e0a 5072  text/markdown.Pr
+00000130: 6f76 6964 6573 2d45 7874 7261 3a20 6875  ovides-Extra: hu
+00000140: 6767 696e 6766 6163 650a 4c69 6365 6e73  ggingface.Licens
+00000150: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
+00000160: 0a23 2047 656e 746f 7069 6120 0af0 9f8c  .# Gentopia ....
+00000170: 8e20 2a43 6f6c 6c65 6374 6976 6520 4772  . *Collective Gr
+00000180: 6f77 7468 206f 6620 496e 7465 6c6c 6967  owth of Intellig
+00000190: 656e 7420 4167 656e 7473 2e2a 20f0 9fa6  ent Agents.* ...
+000001a0: 990a 0a0a 5b21 5b4c 6963 656e 7365 3a20  ....[![License: 
+000001b0: 4d49 545d 2868 7474 7073 3a2f 2f69 6d67  MIT](https://img
+000001c0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+000001d0: 652f 4c69 6365 6e73 652d 4d49 542d 7965  e/License-MIT-ye
+000001e0: 6c6c 6f77 2e73 7667 295d 2868 7474 7073  llow.svg)](https
+000001f0: 3a2f 2f6f 7065 6e73 6f75 7263 652e 6f72  ://opensource.or
+00000200: 672f 6c69 6365 6e73 6573 2f4d 4954 290a  g/licenses/MIT).
+00000210: 215b 5374 6174 6963 2042 6164 6765 5d28  ![Static Badge](
+00000220: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000230: 6c64 732e 696f 2f62 6164 6765 2f72 656c  lds.io/badge/rel
+00000240: 6561 7365 2d62 6574 612d 626c 7565 290a  ease-beta-blue).
+00000250: 5b21 5b53 7461 7469 6320 4261 6467 655d  [![Static Badge]
+00000260: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000270: 656c 6473 2e69 6f2f 6261 6467 652f 446f  elds.io/badge/Do
+00000280: 6375 6d65 6e74 6174 696f 6e2d 3841 3242  cumentation-8A2B
+00000290: 4532 295d 2868 7474 7073 3a2f 2f67 656e  E2)](https://gen
+000002a0: 746f 7069 612e 7265 6164 7468 6564 6f63  topia.readthedoc
+000002b0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f69  s.io/en/latest/i
+000002c0: 6e64 6578 2e68 746d 6c29 0a5b 215b 5374  ndex.html).[![St
+000002d0: 6174 6963 2042 6164 6765 5d28 6874 7470  atic Badge](http
+000002e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000002f0: 696f 2f62 6164 6765 2f47 656e 7450 6f6f  io/badge/GentPoo
+00000300: 6c2d 626c 7565 295d 2868 7474 7073 3a2f  l-blue)](https:/
+00000310: 2f67 6974 6875 622e 636f 6d2f 4765 6e74  /github.com/Gent
+00000320: 6f70 6961 2d41 492f 4765 6e74 506f 6f6c  opia-AI/GentPool
+00000330: 290a 5b21 5b53 7461 7469 6320 4261 6467  ).[![Static Badg
+00000340: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
+00000350: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000360: 6261 636b 6c6f 672d 6772 6579 295d 2868  backlog-grey)](h
+00000370: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000380: 6d2f 6f72 6773 2f47 656e 746f 7069 612d  m/orgs/Gentopia-
+00000390: 4149 2f70 726f 6a65 6374 732f 3129 0a5b  AI/projects/1).[
+000003a0: 215b 4f70 656e 2049 7373 7565 735d 2868  ![Open Issues](h
+000003b0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000003c0: 6473 2e69 6f2f 6769 7468 7562 2f69 7373  ds.io/github/iss
+000003d0: 7565 732d 7261 772f 4765 6e74 6f70 6961  ues-raw/Gentopia
+000003e0: 2d41 492f 4765 6e74 6f70 6961 295d 2868  -AI/Gentopia)](h
+000003f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000400: 6d2f 4765 6e74 6f70 6961 2d41 492f 4765  m/Gentopia-AI/Ge
+00000410: 6e74 6f70 6961 2f69 7373 7565 7329 0a5b  ntopia/issues).[
+00000420: 215b 4465 7065 6e64 656e 6379 2053 7461  ![Dependency Sta
+00000430: 7475 735d 2868 7474 7073 3a2f 2f69 6d67  tus](https://img
+00000440: 2e73 6869 656c 6473 2e69 6f2f 6c69 6272  .shields.io/libr
+00000450: 6172 6965 7369 6f2f 6769 7468 7562 2f47  ariesio/github/G
+00000460: 656e 746f 7069 612d 4149 2f47 656e 746f  entopia-AI/Gento
+00000470: 7069 6129 5d28 6874 7470 733a 2f2f 6c69  pia)](https://li
+00000480: 6272 6172 6965 732e 696f 2f67 6974 6875  braries.io/githu
+00000490: 622f 4765 6e74 6f70 6961 2d41 492f 4765  b/Gentopia-AI/Ge
+000004a0: 6e74 6f70 6961 290a 0a5b 215b 5477 6974  ntopia)..[![Twit
+000004b0: 7465 7220 466f 6c6c 6f77 5d28 6874 7470  ter Follow](http
+000004c0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000004d0: 696f 2f74 7769 7474 6572 2f66 6f6c 6c6f  io/twitter/follo
+000004e0: 772f 4765 6e74 6f70 6961 4149 295d 2868  w/GentopiaAI)](h
+000004f0: 7474 7073 3a2f 2f74 7769 7474 6572 2e63  ttps://twitter.c
+00000500: 6f6d 2f47 656e 746f 7069 6141 4929 0a5b  om/GentopiaAI).[
+00000510: 215b 5d28 6874 7470 733a 2f2f 6463 6261  ![](https://dcba
+00000520: 6467 652e 7665 7263 656c 2e61 7070 2f61  dge.vercel.app/a
+00000530: 7069 2f73 6572 7665 722f 4153 5050 394d  pi/server/ASPP9M
+00000540: 5939 514b 3f63 6f6d 7061 6374 3d74 7275  Y9QK?compact=tru
+00000550: 6526 7374 796c 653d 666c 6174 295d 2868  e&style=flat)](h
+00000560: 7474 7073 3a2f 2f64 6973 636f 7264 2e67  ttps://discord.g
+00000570: 672f 4153 5050 394d 5939 514b 290a 5b21  g/ASPP9MY9QK).[!
+00000580: 5b59 6f75 5475 6265 2043 6861 6e6e 656c  [YouTube Channel
+00000590: 2053 7562 7363 7269 6265 7273 5d28 6874   Subscribers](ht
+000005a0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000005b0: 732e 696f 2f79 6f75 7475 6265 2f63 6861  s.io/youtube/cha
+000005c0: 6e6e 656c 2f76 6965 7773 2f55 4339 5143  nnel/views/UC9QC
+000005d0: 6a63 7348 4a56 4b6a 4b5a 325a 6d72 7138  jcsHJVKjKZ2Zmrq8
+000005e0: 3376 4129 5d28 6874 7470 733a 2f2f 7777  3vA)](https://ww
+000005f0: 772e 796f 7574 7562 652e 636f 6d2f 6368  w.youtube.com/ch
+00000600: 616e 6e65 6c2f 5543 3951 436a 6373 484a  annel/UC9QCjcsHJ
+00000610: 564b 6a4b 5a32 5a6d 7271 3833 7641 290a  VKjKZ2Zmrq83vA).
+00000620: 5b21 5b47 6974 4875 6220 7374 6172 2063  [![GitHub star c
+00000630: 6861 7274 5d28 6874 7470 733a 2f2f 696d  hart](https://im
+00000640: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000650: 6875 622f 7374 6172 732f 4765 6e74 6f70  hub/stars/Gentop
+00000660: 6961 2d41 492f 4765 6e74 6f70 6961 3f73  ia-AI/Gentopia?s
+00000670: 7479 6c65 3d73 6f63 6961 6c29 5d28 6874  tyle=social)](ht
+00000680: 7470 733a 2f2f 7374 6172 2d68 6973 746f  tps://star-histo
+00000690: 7279 2e63 6f6d 2f47 656e 746f 7069 612d  ry.com/Gentopia-
+000006a0: 4149 2f47 656e 746f 7069 6129 0a0a 0a0a  AI/Gentopia)....
+000006b0: 0a47 656e 746f 7069 6120 6973 2061 206c  .Gentopia is a l
+000006c0: 6967 6874 7765 6967 6874 2061 6e64 2065  ightweight and e
+000006d0: 7874 656e 7369 626c 6520 6672 616d 6577  xtensible framew
+000006e0: 6f72 6b20 666f 7220 4c4c 4d2d 6472 6976  ork for LLM-driv
+000006f0: 656e 2041 6765 6e74 7320 616e 6420 5b41  en Agents and [A
+00000700: 4c4d 5d28 6874 7470 733a 2f2f 6172 7869  LM](https://arxi
+00000710: 762e 6f72 672f 6162 732f 3233 3032 2e30  v.org/abs/2302.0
+00000720: 3738 3432 2920 2072 6573 6561 7263 682e  7842)  research.
+00000730: 2049 7420 7072 6f76 6964 6573 2065 7373   It provides ess
+00000740: 656e 7469 616c 2063 6f6d 706f 6e65 6e74  ential component
+00000750: 7320 746f 2062 7569 6c64 2c20 7465 7374  s to build, test
+00000760: 2061 6e64 2065 7661 6c75 6174 6520 6167   and evaluate ag
+00000770: 656e 7473 2e20 4174 2069 7473 2063 6f72  ents. At its cor
+00000780: 652c 2047 656e 746f 7069 6120 6169 6d73  e, Gentopia aims
+00000790: 2074 6f20 6173 7365 6d62 6c65 2061 6e20   to assemble an 
+000007a0: 6167 656e 7420 7769 7468 2061 2073 696e  agent with a sin
+000007b0: 676c 6520 636f 6e66 6967 2c20 7468 7573  gle config, thus
+000007c0: 206d 696e 696d 697a 696e 6720 796f 7572   minimizing your
+000007d0: 2065 6666 6f72 7420 696e 2062 7569 6c64   effort in build
+000007e0: 696e 672c 2074 756e 696e 672c 2061 6e64  ing, tuning, and
+000007f0: 2073 6861 7269 6e67 2061 6765 6e74 732e   sharing agents.
+00000800: 200a 0a47 656e 746f 7069 6120 6d61 696e   ..Gentopia main
+00000810: 7461 696e 7320 616e 2061 6765 6e74 2070  tains an agent p
+00000820: 6c61 7466 6f72 6d20 5b47 656e 7450 6f6f  latform [GentPoo
+00000830: 6c5d 2868 7474 7073 3a2f 2f67 6974 6875  l](https://githu
+00000840: 622e 636f 6d2f 4765 6e74 6f70 6961 2d41  b.com/Gentopia-A
+00000850: 492f 4765 6e74 506f 6f6c 2920 746f 2073  I/GentPool) to s
+00000860: 6861 7265 2073 7065 6369 616c 697a 6564  hare specialized
+00000870: 2061 6765 6e74 732c 2077 6865 7265 2079   agents, where y
+00000880: 6f75 7220 6167 656e 7420 2a69 6e74 6572  our agent *inter
+00000890: 6163 7473 2a20 7769 7468 206f 7468 6572  acts* with other
+000008a0: 2061 6765 6e74 7320 6279 2063 6c6f 6e69   agents by cloni
+000008b0: 6e67 2c20 6869 6572 6172 6368 6963 616c  ng, hierarchical
+000008c0: 2070 6c75 672d 696e 2c20 6f72 2073 6861   plug-in, or sha
+000008d0: 7269 6e67 2065 6e76 6972 6f6e 6d65 6e74  ring environment
+000008e0: 2e20 5765 2070 726f 7669 6465 2061 2075  . We provide a u
+000008f0: 6e69 7175 6520 6167 656e 7420 5b62 656e  nique agent [ben
+00000900: 6368 6d61 726b 5d28 6874 7470 733a 2f2f  chmark](https://
+00000910: 6765 6e74 6f70 6961 2e72 6561 6474 6865  gentopia.readthe
+00000920: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00000930: 742f 6765 6e74 706f 6f6c 2e68 746d 6c23  t/gentpool.html#
+00000940: 6167 656e 742d 6576 616c 7561 7469 6f6e  agent-evaluation
+00000950: 2920 666f 7220 686f 6c69 7374 6963 2065  ) for holistic e
+00000960: 7661 6c75 6174 696f 6e2e 200a 0a23 2320  valuation. ..## 
+00000970: 4d6f 7469 7661 7469 6f6e 20f0 9fa7 a00a  Motivation .....
+00000980: 4167 656e 7420 7072 6163 7469 7469 6f6e  Agent practition
+00000990: 6572 7320 7374 6172 7420 746f 2072 6561  ers start to rea
+000009a0: 6c69 7a65 2074 6865 2064 6966 6669 6375  lize the difficu
+000009b0: 6c74 7920 696e 2074 756e 696e 6720 6120  lty in tuning a 
+000009c0: 2277 656c 6c2d 726f 756e 6465 6422 2061  "well-rounded" a
+000009d0: 6765 6e74 2077 6974 6820 746f 6e73 206f  gent with tons o
+000009e0: 6620 746f 6f6c 7320 6f72 2069 6e73 7472  f tools or instr
+000009f0: 7563 7469 6f6e 7320 696e 2061 2073 696e  uctions in a sin
+00000a00: 676c 6520 6c61 7965 722e 0a52 6563 656e  gle layer..Recen
+00000a10: 7420 7374 7564 6965 7320 6c69 6b65 205b  t studies like [
+00000a20: 5469 6e79 5374 6f72 6965 735d 2868 7474  TinyStories](htt
+00000a30: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
+00000a40: 6273 2f32 3330 312e 3132 3732 3629 2c20  bs/2301.12726), 
+00000a50: 5b53 7065 6369 616c 697a 696e 6720 5265  [Specializing Re
+00000a60: 6173 6f6e 696e 675d 2868 7474 7073 3a2f  asoning](https:/
+00000a70: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00000a80: 3330 312e 3132 3732 3629 2c20 5b4c 6574  301.12726), [Let
+00000a90: 2773 2056 6572 6966 7920 5362 535d 2868  's Verify SbS](h
+00000aa0: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
+00000ab0: 2f61 6273 2f32 3330 352e 3230 3035 3029  /abs/2305.20050)
+00000ac0: 2c20 5b52 6557 4f4f 5d28 6874 7470 733a  , [ReWOO](https:
+00000ad0: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
+00000ae0: 3233 3035 2e31 3833 3233 292c 2065 7463  2305.18323), etc
+00000af0: 2e20 616c 736f 2070 6f69 6e74 2075 7320  . also point us 
+00000b00: 746f 7761 7264 7320 616e 2069 6e74 7569  towards an intui
+00000b10: 7469 7665 2079 6574 2075 6e64 6572 7661  tive yet underva
+00000b20: 6c75 6564 2064 6972 6563 7469 6f6e 20f0  lued direction .
+00000b30: 9f91 8920 0a0a 6060 600a 416e 204c 4c4d  ... ..```.An LLM
+00000b40: 2069 7320 6d6f 7265 2063 6170 6162 6c65   is more capable
+00000b50: 2069 6620 796f 7520 6372 6561 7465 2061   if you create a
+00000b60: 2063 6f6e 7465 7874 2f64 6973 7472 6962   context/distrib
+00000b70: 7574 696f 6e20 7368 6966 7420 7370 6563  ution shift spec
+00000b80: 6961 6c69 7a65 6420 746f 2073 6f6d 6520  ialized to some 
+00000b90: 7461 7267 6574 2074 6173 6b73 2e0a 6060  target tasks..``
+00000ba0: 600a 5361 646c 792c 2074 6865 7265 2069  `.Sadly, there i
+00000bb0: 7320 6e6f 2073 696c 7665 7220 6275 6c6c  s no silver bull
+00000bc0: 6574 2066 6f72 2061 6765 6e74 2073 7065  et for agent spe
+00000bd0: 6369 616c 697a 6174 696f 6e2e 2046 6f72  cialization. For
+00000be0: 2065 7861 6d70 6c65 2c20 796f 7520 6361   example, you ca
+00000bf0: 6e20 0a2d 2053 696d 706c 7920 6164 6420  n .- Simply add 
+00000c00: 604c 6574 2773 2074 6869 6e6b 2073 7465  `Let's think ste
+00000c10: 7020 6279 2073 7465 702e 6020 696e 2079  p by step.` in y
+00000c20: 6f75 7220 2a2a 7072 6f6d 7074 2a2a 2066  our **prompt** f
+00000c30: 6f72 206d 6f72 6520 6163 6375 7261 7465  or more accurate
+00000c40: 204d 6174 6820 5141 2e0a 2d20 4769 7665   Math QA..- Give
+00000c50: 2061 202a 2a66 6577 2d73 686f 742a 2a20   a **few-shot** 
+00000c60: 6578 656d 706c 6172 2069 6e20 796f 7572  exemplar in your
+00000c70: 2070 726f 6d70 7420 746f 2067 7569 6465   prompt to guide
+00000c80: 2061 2062 6574 7465 7220 7265 6173 6f6e   a better reason
+00000c90: 696e 6720 7472 616a 6563 746f 7279 2066  ing trajectory f
+00000ca0: 6f72 206e 6f76 656c 2070 6c6f 7474 696e  or novel plottin
+00000cb0: 672e 0a2d 2053 7570 6572 7669 7365 202a  g..- Supervise *
+00000cc0: 2a66 696e 652d 7475 6e69 6e67 2a2a 2028  *fine-tuning** (
+00000cd0: 5346 5429 2079 6f75 7220 3730 4220 606c  SFT) your 70B `l
+00000ce0: 6c61 6d61 3260 206c 696b 6520 5b74 6869  lama2` like [thi
+00000cf0: 735d 2868 7474 7073 3a2f 2f61 7278 6976  s](https://arxiv
+00000d00: 2e6f 7267 2f61 6273 2f32 3330 352e 3230  .org/abs/2305.20
+00000d10: 3035 3029 2074 6f20 6d61 7463 6820 7265  050) to match re
+00000d20: 6173 6f6e 696e 6720 6f66 2031 3735 4220  asoning of 175B 
+00000d30: 4750 542d 332e 352e 0a2d 2054 756e 6520  GPT-3.5..- Tune 
+00000d40: 796f 7572 2061 6765 6e74 202a 2a70 6172  your agent **par
+00000d50: 6164 6967 6d2a 2a20 6c69 6b65 2074 6869  adigm** like thi
+00000d60: 7320 5b64 656d 6f5d 2868 7474 7073 3a2f  s [demo](https:/
+00000d70: 2f77 7777 2e79 6f75 7475 6265 2e63 6f6d  /www.youtube.com
+00000d80: 2f77 6174 6368 3f76 3d64 694a 3449 4461  /watch?v=diJ4IDa
+00000d90: 5434 5a34 2920 746f 2065 6173 696c 7920  T4Z4) to easily 
+00000da0: 6861 6c66 2074 6865 2065 7865 6375 7469  half the executi
+00000db0: 6f6e 2074 696d 6520 666f 7220 5365 6163  on time for Seac
+00000dc0: 6820 2620 5375 6d6d 6172 697a 652e 0a2d  h & Summarize..-
+00000dd0: 2041 6e64 206d 6f72 6520 2e2e 2e0a 0a49   And more .....I
+00000de0: 736e 2774 2069 7420 6265 6175 7469 6675  sn't it beautifu
+00000df0: 6c20 6966 206f 6e65 2073 6861 7265 7320  l if one shares 
+00000e00: 6869 7320 6566 666f 7274 2069 6e20 7370  his effort in sp
+00000e10: 6563 6961 6c69 7a65 6420 696e 7465 6c6c  ecialized intell
+00000e20: 6967 656e 6365 2c20 616c 6c6f 7769 6e67  igence, allowing
+00000e30: 206f 7468 6572 7320 746f 2072 6570 726f   others to repro
+00000e40: 6475 6365 2c20 6275 696c 6420 6f6e 2c20  duce, build on, 
+00000e50: 6f72 2069 6e74 6572 6163 7420 7769 7468  or interact with
+00000e60: 2069 743f 20f0 9fa4 9720 5468 6973 2062   it? .... This b
+00000e70: 656c 6965 6620 696e 7370 6972 6573 2075  elief inspires u
+00000e80: 7320 746f 2062 7569 6c64 2047 656e 746f  s to build Gento
+00000e90: 7069 612c 200a 2a2a 6465 7369 676e 6564  pia, .**designed
+00000ea0: 2066 6f72 2061 6765 6e74 202a 7370 6563   for agent *spec
+00000eb0: 6961 6c69 7a61 7469 6f6e 2c20 7368 6172  ialization, shar
+00000ec0: 696e 672c 2061 6e64 2069 6e74 6572 6163  ing, and interac
+00000ed0: 7469 6f6e 2c2a 2074 6f20 7374 6163 6b69  tion,* to stacki
+00000ee0: 6e67 6c79 2061 6368 6965 7665 2063 6f6c  ngly achieve col
+00000ef0: 6c65 6374 6976 6520 6772 6f77 7468 2074  lective growth t
+00000f00: 6f77 6172 6473 2067 7265 6174 6572 2069  owards greater i
+00000f10: 6e74 656c 6c69 6765 6e63 652e 2a2a 2e0a  ntelligence.**..
+00000f20: 0a23 2320 436f 7265 2046 6561 7475 7265  .## Core Feature
+00000f30: 7320 f09f 92a1 0a0a 2d20 e29a 99ef b88f  s ......- ......
+00000f40: 2043 6f6e 6669 672d 6472 6976 656e 2061   Config-driven a
+00000f50: 6765 6e74 2061 7373 656d 626c 696e 6720  gent assembling 
+00000f60: 616e 6420 6368 6174 2e0a 2d20 f09f 9a80  and chat..- ....
+00000f70: 204c 6172 6765 2061 6d6f 756e 7420 6f66   Large amount of
+00000f80: 2070 7265 6275 696c 7420 6167 656e 7420   prebuilt agent 
+00000f90: 7479 7065 732c 204c 4c4d 2063 6c69 656e  types, LLM clien
+00000fa0: 7473 2c20 746f 6f6c 732c 206d 656d 6f72  ts, tools, memor
+00000fb0: 7920 7379 7374 656d 732c 2061 6e64 206d  y systems, and m
+00000fc0: 6f72 652e 0a2d 20f0 9faa b620 4c69 6768  ore..- .... Ligh
+00000fd0: 7477 6569 6768 7420 616e 6420 6869 6768  tweight and high
+00000fe0: 6c79 2065 7874 656e 7369 626c 6520 696d  ly extensible im
+00000ff0: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
+00001000: 6573 7365 6e74 6961 6c20 636f 6d70 6f6e  essential compon
+00001010: 656e 7473 2e0a 2d20 f09f a7aa 2041 6c69  ents..- .... Ali
+00001020: 676e 696e 6720 7769 7468 2073 7461 7465  gning with state
+00001030: 2d6f 662d 7468 652d 6172 7420 4149 2072  -of-the-art AI r
+00001040: 6573 6561 7263 682e 0a2d 20f0 9fa4 9d20  esearch..- .... 
+00001050: 456e 6162 6c69 6e67 206d 756c 7469 2d61  Enabling multi-a
+00001060: 6765 6e74 2069 6e74 6572 6163 7469 6f6e  gent interaction
+00001070: 732e 0a2d 20f0 9fa6 8120 556e 6971 7565  s..- .... Unique
+00001080: 2070 6c61 7466 6f72 6d20 6f66 2061 6765   platform of age
+00001090: 6e74 207a 6f6f 2061 6e64 2065 7661 6c20  nt zoo and eval 
+000010a0: 6265 6e63 686d 6172 6b2e 0a0a 2323 2051  benchmark...## Q
+000010b0: 7569 636b 2053 7461 7274 20f0 9f8d 8f0a  uick Start .....
+000010c0: 6060 600a 636f 6e64 6120 6372 6561 7465  ```.conda create
+000010d0: 202d 2d6e 616d 6520 6765 6e74 656e 7620   --name gentenv 
+000010e0: 7079 7468 6f6e 3d33 2e31 300a 636f 6e64  python=3.10.cond
+000010f0: 6120 6163 7469 7661 7465 2067 656e 7465  a activate gente
+00001100: 6e76 0a70 6970 2069 6e73 7461 6c6c 2067  nv.pip install g
+00001110: 656e 746f 7069 610a 6060 600a 6f72 2069  entopia.```.or i
+00001120: 6620 796f 7520 7761 6e74 2074 6f20 6275  f you want to bu
+00001130: 696c 6420 7769 7468 206f 7065 6e20 4c4c  ild with open LL
+00001140: 4d73 206c 6f63 616c 6c79 20f0 9f91 8920  Ms locally .... 
+00001150: 6070 6970 2069 6e73 7461 6c6c 2067 656e  `pip install gen
+00001160: 746f 7069 615b 6875 6767 696e 6766 6163  topia[huggingfac
+00001170: 655d 600a 0a46 6972 7374 2074 696d 6520  e]`..First time 
+00001180: 746f 2047 656e 746f 7069 613f 2047 7261  to Gentopia? Gra
+00001190: 6220 6120 636f 6666 6565 20e2 9895 2061  b a coffee ... a
+000011a0: 6e64 200a 0a54 616b 6520 7e20 3820 6d69  nd ..Take ~ 8 mi
+000011b0: 6e73 2074 6f20 6368 6563 6b20 6f75 7420  ns to check out 
+000011c0: 7468 6520 666f 6c6c 6f77 696e 6720 6465  the following de
+000011d0: 6d6f 2074 7574 6f72 6961 6c73 205b 215b  mo tutorials [![
+000011e0: 596f 7554 7562 6520 4368 616e 6e65 6c20  YouTube Channel 
+000011f0: 5375 6273 6372 6962 6572 735d 2868 7474  Subscribers](htt
+00001200: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00001210: 2e69 6f2f 796f 7574 7562 652f 6368 616e  .io/youtube/chan
+00001220: 6e65 6c2f 7669 6577 732f 5543 3951 436a  nel/views/UC9QCj
+00001230: 6373 484a 564b 6a4b 5a32 5a6d 7271 3833  csHJVKjKZ2Zmrq83
+00001240: 7641 295d 2868 7474 7073 3a2f 2f77 7777  vA)](https://www
+00001250: 2e79 6f75 7475 6265 2e63 6f6d 2f63 6861  .youtube.com/cha
+00001260: 6e6e 656c 2f55 4339 5143 6a63 7348 4a56  nnel/UC9QCjcsHJV
+00001270: 4b6a 4b5a 325a 6d72 7138 3376 4129 200a  KjKZ2Zmrq83vA) .
+00001280: 0a3c 6469 7620 7374 796c 653d 2264 6973  .<div style="dis
+00001290: 706c 6179 3a20 666c 6578 3b20 6a75 7374  play: flex; just
+000012a0: 6966 792d 636f 6e74 656e 743a 2073 7061  ify-content: spa
+000012b0: 6365 2d61 726f 756e 643b 223e 0a20 200a  ce-around;">.  .
+000012c0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000012d0: 2f77 7777 2e79 6f75 7475 6265 2e63 6f6d  /www.youtube.com
+000012e0: 2f77 6174 6368 3f76 3d37 645a 335a 7673  /watch?v=7dZ3Zvs
+000012f0: 4937 7377 2220 7461 7267 6574 3d22 5f62  I7sw" target="_b
+00001300: 6c61 6e6b 223e 0a20 203c 696d 6720 7372  lank">.  <img sr
+00001310: 633d 2268 7474 7073 3a2f 2f69 6d67 2e79  c="https://img.y
+00001320: 6f75 7475 6265 2e63 6f6d 2f76 692f 3764  outube.com/vi/7d
+00001330: 5a33 5a76 7349 3773 772f 6871 6465 6661  Z3ZvsI7sw/hqdefa
+00001340: 756c 742e 6a70 6722 2061 6c74 3d22 5669  ult.jpg" alt="Vi
+00001350: 6465 6f20 3122 2073 7479 6c65 3d22 7769  deo 1" style="wi
+00001360: 6474 683a 3332 253b 223e 0a3c 2f61 3e0a  dth:32%;">.</a>.
+00001370: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00001380: 2f2f 7777 772e 796f 7574 7562 652e 636f  //www.youtube.co
+00001390: 6d2f 7761 7463 683f 763d 5854 7376 3970  m/watch?v=XTsv9p
+000013a0: 6b36 414f 4122 2074 6172 6765 743d 225f  k6AOA" target="_
+000013b0: 626c 616e 6b22 3e0a 2020 3c69 6d67 2073  blank">.  <img s
+000013c0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+000013d0: 796f 7574 7562 652e 636f 6d2f 7669 2f58  youtube.com/vi/X
+000013e0: 5473 7639 706b 3641 4f41 2f68 7164 6566  Tsv9pk6AOA/hqdef
+000013f0: 6175 6c74 2e6a 7067 2220 616c 743d 2256  ault.jpg" alt="V
+00001400: 6964 656f 2032 2220 7374 796c 653d 2277  ideo 2" style="w
+00001410: 6964 7468 3a33 3225 3b22 3e0a 3c2f 613e  idth:32%;">.</a>
+00001420: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+00001430: 3a2f 2f77 7777 2e79 6f75 7475 6265 2e63  ://www.youtube.c
+00001440: 6f6d 2f77 6174 6368 3f76 3d64 694a 3449  om/watch?v=diJ4I
+00001450: 4461 5434 5a34 2220 7461 7267 6574 3d22  DaT4Z4" target="
+00001460: 5f62 6c61 6e6b 223e 0a20 203c 696d 6720  _blank">.  <img 
+00001470: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00001480: 2e79 6f75 7475 6265 2e63 6f6d 2f76 692f  .youtube.com/vi/
+00001490: 6469 4a34 4944 6154 345a 342f 6871 6465  diJ4IDaT4Z4/hqde
+000014a0: 6661 756c 742e 6a70 6722 2061 6c74 3d22  fault.jpg" alt="
+000014b0: 5669 6465 6f20 3322 2073 7479 6c65 3d22  Video 3" style="
+000014c0: 7769 6474 683a 3332 253b 223e 0a3c 2f61  width:32%;">.</a
+000014d0: 3e0a 0a3c 2f64 6976 3e0a 0a4f 7220 6368  >..</div>..Or ch
+000014e0: 6563 6b20 6f75 7420 7468 6520 5b51 7569  eck out the [Qui
+000014f0: 636b 2053 7461 7274 5d28 6874 7470 733a  ck Start](https:
+00001500: 2f2f 6765 6e74 6f70 6961 2e72 6561 6474  //gentopia.readt
+00001510: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00001520: 6573 742f 7175 6963 6b5f 7374 6172 742e  est/quick_start.
+00001530: 6874 6d6c 2920 446f 632e 0a0a 2323 2044  html) Doc...## D
+00001540: 6f63 756d 656e 7461 7469 6f6e 20f0 9f93  ocumentation ...
+00001550: 960a 5365 6520 5b68 6572 655d 2868 7474  ..See [here](htt
+00001560: 7073 3a2f 2f67 656e 746f 7069 612e 7265  ps://gentopia.re
+00001570: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00001580: 6c61 7465 7374 2f69 6e64 6578 2e68 746d  latest/index.htm
+00001590: 6c29 2066 6f72 2066 756c 6c20 646f 6375  l) for full docu
+000015a0: 6d65 6e74 6174 696f 6e2e 0a0a f09f 8c9f  mentation.......
+000015b0: 2048 6967 686c 6967 6874 2054 6f70 6963   Highlight Topic
+000015c0: 7320 f09f 8c9f 200a 2d20 5bf0 9fa4 9620  s .... .- [.... 
+000015d0: 4167 656e 7420 5465 6d70 6c61 7465 735d  Agent Templates]
+000015e0: 2868 7474 7073 3a2f 2f67 656e 746f 7069  (https://gentopi
+000015f0: 612e 7265 6164 7468 6564 6f63 732e 696f  a.readthedocs.io
+00001600: 2f65 6e2f 6c61 7465 7374 2f71 7569 636b  /en/latest/quick
+00001610: 5f73 7461 7274 2e68 746d 6c23 7661 6e69  _start.html#vani
+00001620: 6c6c 612d 6167 656e 7429 0a2d 205b e29b  lla-agent).- [..
+00001630: b0ef b88f 2048 6965 7261 7263 6869 6361  .... Hierarchica
+00001640: 6c20 4167 656e 7473 5d28 6874 7470 733a  l Agents](https:
+00001650: 2f2f 6765 6e74 6f70 6961 2e72 6561 6474  //gentopia.readt
+00001660: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00001670: 6573 742f 6167 656e 745f 636f 6d70 6f6e  est/agent_compon
+00001680: 656e 7473 2e68 746d 6c23 6167 656e 742d  ents.html#agent-
+00001690: 6173 2d70 6c75 6769 6e29 0a2d 205b f09f  as-plugin).- [..
+000016a0: a587 2055 6e69 7175 6520 4167 656e 7420  .. Unique Agent 
+000016b0: 4265 6e63 686d 6172 6b5d 2868 7474 7073  Benchmark](https
+000016c0: 3a2f 2f67 656e 746f 7069 612e 7265 6164  ://gentopia.read
+000016d0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+000016e0: 7465 7374 2f67 656e 7470 6f6f 6c2e 6874  test/gentpool.ht
+000016f0: 6d6c 2361 6765 6e74 2d65 7661 6c75 6174  ml#agent-evaluat
+00001700: 696f 6e29 0a2d 205b f09f a699 204f 7065  ion).- [.... Ope
+00001710: 6e20 4c4c 4d20 5375 7070 6f72 7473 5d28  n LLM Supports](
+00001720: 6874 7470 733a 2f2f 6765 6e74 6f70 6961  https://gentopia
+00001730: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00001740: 656e 2f6c 6174 6573 742f 6167 656e 745f  en/latest/agent_
+00001750: 636f 6d70 6f6e 656e 7473 2e68 746d 6c23  components.html#
+00001760: 6875 6767 696e 6766 6163 652d 6f70 656e  huggingface-open
+00001770: 2d6c 6c6d 7329 0a2d 205b f09f a7a0 2048  -llms).- [.... H
+00001780: 6967 682d 5065 7266 6f72 6d61 6e63 6520  igh-Performance 
+00001790: 4d65 6d6f 7279 5d28 6874 7470 733a 2f2f  Memory](https://
+000017a0: 6765 6e74 6f70 6961 2e72 6561 6474 6865  gentopia.readthe
+000017b0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+000017c0: 742f 6167 656e 745f 636f 6d70 6f6e 656e  t/agent_componen
+000017d0: 7473 2e68 746d 6c23 6c6f 6e67 2d73 686f  ts.html#long-sho
+000017e0: 7274 2d74 6572 6d2d 6d65 6d6f 7279 290a  rt-term-memory).
+000017f0: 0a23 2320 4a6f 696e 2075 7321 20f0 9f8c  .## Join us! ...
+00001800: 8e0a 0a50 6172 7469 6369 7061 7465 2069  ...Participate i
+00001810: 6e20 7468 6973 2055 746f 7069 6120 6f66  n this Utopia of
+00001820: 2073 7570 6572 696e 7465 6c6c 6967 656e   superintelligen
+00001830: 6365 2061 6e64 2068 656c 7020 6974 2067  ce and help it g
+00001840: 726f 7773 2120 4173 2061 2066 756c 6c79  rows! As a fully
+00001850: 206f 7065 6e2d 736f 7572 6365 2070 726f   open-source pro
+00001860: 6a65 6374 2c20 7765 2064 6576 656c 6f70  ject, we develop
+00001870: 2075 6e64 6572 2070 7562 6c69 6320 6164   under public ad
+00001880: 7669 6365 2c20 6964 6561 732c 2061 6e64  vice, ideas, and
+00001890: 2073 7570 6572 7669 7369 6f6e 2e20 4d65   supervision. Me
+000018a0: 616e 7768 696c 652c 2068 6572 6520 6172  anwhile, here ar
+000018b0: 6520 7761 7973 2079 6f75 206d 6179 2063  e ways you may c
+000018c0: 6f6e 7472 6962 7574 6520 746f 2047 656e  ontribute to Gen
+000018d0: 746f 7069 612e 0a0a 2d20 f09f 909b 2050  topia...- .... P
+000018e0: 6f73 7420 616e 205b 6973 7375 655d 2868  ost an [issue](h
+000018f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001900: 6d2f 4765 6e74 6f70 6961 2d41 492f 4765  m/Gentopia-AI/Ge
+00001910: 6e74 6f70 6961 2f69 7373 7565 7329 2072  ntopia/issues) r
+00001920: 6571 7565 7374 696e 6720 6e65 6365 7373  equesting necess
+00001930: 6172 7920 6275 6720 6669 7865 732c 2061  ary bug fixes, a
+00001940: 6464 6974 696f 6e61 6c20 6665 6174 7572  dditional featur
+00001950: 6573 2c20 6f72 2072 6f61 646d 6170 2073  es, or roadmap s
+00001960: 7567 6765 7374 696f 6e73 2e20 2843 6865  uggestions. (Che
+00001970: 636b 2063 6c6f 7365 6420 6f6e 6573 2066  ck closed ones f
+00001980: 6972 7374 290a 2d20 f09f 8eaf 204f 7572  irst).- .... Our
+00001990: 2064 6576 2074 6561 6d20 6d65 6574 7320   dev team meets 
+000019a0: 7765 656b 6c79 2074 6f20 6772 6f6f 6d20  weekly to groom 
+000019b0: 5b62 6163 6b6c 6f67 5d28 6874 7470 733a  [backlog](https:
+000019c0: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 7267  //github.com/org
+000019d0: 732f 4765 6e74 6f70 6961 2d41 492f 7072  s/Gentopia-AI/pr
+000019e0: 6f6a 6563 7473 2f31 2920 696e 746f 2074  ojects/1) into t
+000019f0: 6963 6b65 7473 2e20 5768 696c 6520 7765  ickets. While we
+00001a00: 2077 6f72 6b20 6f6e 2074 6865 6d2c 2079   work on them, y
+00001a10: 6f75 2063 616e 2070 6963 6b20 7570 206f  ou can pick up o
+00001a20: 7468 6572 7320 616e 6420 6372 6561 7465  thers and create
+00001a30: 2061 205b 5075 6c6c 2052 6571 7565 7374   a [Pull Request
+00001a40: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001a50: 2e63 6f6d 2f47 656e 746f 7069 612d 4149  .com/Gentopia-AI
+00001a60: 2f47 656e 746f 7069 612f 7075 6c6c 7329  /Gentopia/pulls)
+00001a70: 2074 6f20 7265 7175 6573 7420 6120 6d65   to request a me
+00001a80: 7267 652e 2057 6520 616c 7761 7973 2077  rge. We always w
+00001a90: 656c 636f 6d65 206e 6577 206d 656d 6265  elcome new membe
+00001aa0: 7273 2069 6e20 7468 6973 2077 6179 2e0a  rs in this way..
+00001ab0: 2d20 f09f a49d 2053 6861 7265 2079 6f75  - .... Share you
+00001ac0: 7220 7370 6563 6961 6c69 7a65 6420 6167  r specialized ag
+00001ad0: 656e 7420 746f 205b 4765 6e74 506f 6f6c  ent to [GentPool
+00001ae0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001af0: 2e63 6f6d 2f47 656e 746f 7069 612d 4149  .com/Gentopia-AI
+00001b00: 2f47 656e 7450 6f6f 6c29 2120 4372 6561  /GentPool)! Crea
+00001b10: 7465 2061 6e20 4167 656e 7420 5052 2028  te an Agent PR (
+00001b20: 5b65 7861 6d70 6c65 5d28 2929 2074 6f20  [example]()) to 
+00001b30: 6d65 7267 6520 796f 7572 2077 656c 6c2d  merge your well-
+00001b40: 7475 6e65 6420 6167 656e 7420 696e 746f  tuned agent into
+00001b50: 2074 6865 2070 6f6f 6c2e 2054 6869 7320   the pool. This 
+00001b60: 616c 6c6f 7773 206f 7468 6572 7320 746f  allows others to
+00001b70: 2075 7365 206f 7220 6275 696c 6420 7570   use or build up
+00001b80: 6f6e 2079 6f75 7220 6167 656e 742e 200a  on your agent. .
+00001b90: 2d20 e2ad 9020 4865 6c70 2075 7320 7370  - ... Help us sp
+00001ba0: 7265 6164 2120 4769 7665 2075 7320 6120  read! Give us a 
+00001bb0: 7374 6172 2c20 666f 6c6c 6f77 2075 7320  star, follow us 
+00001bc0: 6f6e 205b 5477 6974 7465 725d 2868 7474  on [Twitter](htt
+00001bd0: 7073 3a2f 2f74 7769 7474 6572 2e63 6f6d  ps://twitter.com
+00001be0: 2f47 656e 746f 7069 6141 4929 2c20 6a6f  /GentopiaAI), jo
+00001bf0: 696e 206f 7572 205b 4469 7363 6f72 645d  in our [Discord]
+00001c00: 2868 7474 7073 3a2f 2f64 6973 636f 7264  (https://discord
+00001c10: 2e67 672f 4153 5050 394d 5939 514b 292c  .gg/ASPP9MY9QK),
+00001c20: 2061 6e64 2073 6861 7265 2077 6974 6820   and share with 
+00001c30: 796f 7572 2066 7269 656e 6473 2120 200a  your friends!  .
+00001c40: 0a0a                                     ..
```

### Comparing `gentopia-0.0.1/README.md` & `gentopia-0.0.2/gentopia.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,335 +1,453 @@
-00000000: 2320 4765 6e74 6f70 6961 200a 2a54 6865  # Gentopia .*The
-00000010: 2043 6f6c 6c65 6374 6976 6520 4772 6f77   Collective Grow
-00000020: 7468 206f 6620 496e 7465 6c6c 6967 656e  th of Intelligen
-00000030: 7420 4167 656e 7473 2e2a 20f0 9fa6 99f0  t Agents.* .....
-00000040: 9f8c 8e0a 0a47 656e 746f 7069 6120 6973  .....Gentopia is
-00000050: 2061 206c 6967 6874 7765 6967 6874 2061   a lightweight a
-00000060: 6e64 2065 7874 656e 7369 626c 6520 6672  nd extensible fr
-00000070: 616d 6577 6f72 6b20 666f 7220 4c4c 4d2d  amework for LLM-
-00000080: 6472 6976 656e 2041 6765 6e74 7320 616e  driven Agents an
-00000090: 6420 5b41 4c4d 5d28 6874 7470 733a 2f2f  d [ALM](https://
-000000a0: 6172 7869 762e 6f72 672f 6162 732f 3233  arxiv.org/abs/23
-000000b0: 3032 2e30 3738 3432 2920 2072 6573 6561  02.07842)  resea
-000000c0: 7263 682e 2049 7420 7072 6f76 6964 6573  rch. It provides
-000000d0: 206d 756c 7469 706c 6520 6573 7365 6e74   multiple essent
-000000e0: 6961 6c20 636f 6d70 6f6e 656e 7473 2074  ial components t
-000000f0: 6f20 6275 696c 642c 2074 6573 7420 616e  o build, test an
-00000100: 6420 6576 616c 7561 7465 2061 6765 6e74  d evaluate agent
-00000110: 732e 2041 7420 6974 7320 636f 7265 2c20  s. At its core, 
-00000120: 4765 6e74 6f70 6961 2061 696d 7320 746f  Gentopia aims to
-00000130: 2065 6d62 6f64 7920 6167 656e 7473 2077   embody agents w
-00000140: 6974 6820 7369 6e67 6c65 2063 6f6e 6669  ith single confi
-00000150: 6720 6669 6c65 732c 2074 6875 7320 6d69  g files, thus mi
-00000160: 6e69 6d69 7a69 6e67 2079 6f75 7220 6566  nimizing your ef
-00000170: 666f 7274 2069 6e20 6d61 696e 7461 696e  fort in maintain
-00000180: 696e 672c 2074 756e 696e 672c 2061 6e64  ing, tuning, and
-00000190: 2073 6861 7269 6e67 2061 6765 6e74 732e   sharing agents.
-000001a0: 0a0a 4765 6e74 6f70 6961 206d 6169 6e74  ..Gentopia maint
-000001b0: 6169 6e73 2061 6e20 6167 656e 7420 7a6f  ains an agent zo
-000001c0: 6f20 5b47 656e 7450 6f6f 6c5d 2868 7474  o [GentPool](htt
-000001d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
-000001e0: 4765 6e74 6f70 6961 2d41 492f 4765 6e74  Gentopia-AI/Gent
-000001f0: 506f 6f6c 2920 746f 2073 6861 7265 2070  Pool) to share p
-00000200: 7562 6c69 6320 6167 656e 7473 2073 7065  ublic agents spe
-00000210: 6369 616c 697a 6564 2066 6f72 2064 6966  cialized for dif
-00000220: 6665 7265 6e74 2074 6173 6b73 2e20 496e  ferent tasks. In
-00000230: 2074 6869 7320 706c 6174 666f 726d 2c20   this platform, 
-00000240: 796f 7520 636f 756c 6420 6561 7369 6c79  you could easily
-00000250: 202a 696e 7465 7261 6374 2a20 7769 7468   *interact* with
-00000260: 206f 7468 6572 2061 6765 6e74 7320 6279   other agents by
-00000270: 2063 6c6f 6e69 6e67 2c20 6869 6572 6172   cloning, hierar
-00000280: 6368 6963 616c 2070 6c75 672d 696e 2c20  chical plug-in, 
-00000290: 6f72 2073 6861 7269 6e67 2065 6e76 6972  or sharing envir
-000002a0: 6f6e 6d65 6e74 2e20 5765 2061 6c73 6f20  onment. We also 
-000002b0: 6275 696c 6420 6120 756e 6971 7565 2061  build a unique a
-000002c0: 6765 6e74 205b 6265 6e63 686d 6172 6b5d  gent [benchmark]
-000002d0: 2868 7474 7073 3a2f 2f67 656e 746f 7069  (https://gentopi
-000002e0: 612e 7265 6164 7468 6564 6f63 732e 696f  a.readthedocs.io
-000002f0: 2f65 6e2f 6c61 7465 7374 2f67 656e 7470  /en/latest/gentp
-00000300: 6f6f 6c2e 6874 6d6c 2361 6765 6e74 2d65  ool.html#agent-e
-00000310: 7661 6c75 6174 696f 6e29 2066 6f72 2068  valuation) for h
-00000320: 6f6c 6973 7469 6320 414c 4d20 6576 616c  olistic ALM eval
-00000330: 7561 7469 6f6e 2e20 0a0a 2323 204d 6f74  uation. ..## Mot
-00000340: 6976 6174 696f 6e20 f09f a7a0 0a41 6765  ivation .....Age
-00000350: 6e74 2070 7261 6374 6974 696f 6e65 7273  nt practitioners
-00000360: 2073 7461 7274 2074 6f20 7265 616c 697a   start to realiz
-00000370: 6520 7468 6520 6469 6666 6963 756c 7479  e the difficulty
-00000380: 2069 6e20 7475 6e69 6e67 2061 2022 7765   in tuning a "we
-00000390: 6c6c 2d72 6f75 6e64 6564 2220 6167 656e  ll-rounded" agen
-000003a0: 7420 7769 7468 2074 6f6e 7320 6f66 2074  t with tons of t
-000003b0: 6f6f 6c73 206f 7220 696e 7374 7275 6374  ools or instruct
-000003c0: 696f 6e73 2069 6e20 7369 6e67 6c65 206c  ions in single l
-000003d0: 6179 6572 2e0a 5265 6365 6e74 2073 7475  ayer..Recent stu
-000003e0: 6469 6573 206c 696b 6520 5b54 696e 7953  dies like [TinyS
-000003f0: 746f 7269 6573 5d28 6874 7470 733a 2f2f  tories](https://
-00000400: 6172 7869 762e 6f72 672f 6162 732f 3233  arxiv.org/abs/23
-00000410: 3031 2e31 3237 3236 292c 205b 5370 6563  01.12726), [Spec
-00000420: 6961 6c69 7a69 6e67 2052 6561 736f 6e69  ializing Reasoni
-00000430: 6e67 5d28 6874 7470 733a 2f2f 6172 7869  ng](https://arxi
-00000440: 762e 6f72 672f 6162 732f 3233 3031 2e31  v.org/abs/2301.1
-00000450: 3237 3236 292c 205b 4c65 7427 7320 5665  2726), [Let's Ve
-00000460: 7269 6679 2053 6253 5d28 6874 7470 733a  rify SbS](https:
-00000470: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
-00000480: 3233 3035 2e32 3030 3530 292c 205b 5265  2305.20050), [Re
-00000490: 574f 4f5d 2868 7474 7073 3a2f 2f61 7278  WOO](https://arx
-000004a0: 6976 2e6f 7267 2f61 6273 2f32 3330 352e  iv.org/abs/2305.
-000004b0: 3138 3332 3329 2c20 6574 632e 2061 6c73  18323), etc. als
-000004c0: 6f20 706f 696e 7420 7573 2074 6f77 6172  o point us towar
-000004d0: 6473 2061 6e20 696e 7475 6974 6976 6520  ds an intuitive 
-000004e0: 7965 7420 756e 6465 7276 616c 7565 6420  yet undervalued 
-000004f0: 6469 7265 6374 696f 6e20 f09f 9189 200a  direction .... .
-00000500: 0a60 6060 0a41 6e20 4c4c 4d20 6973 206d  .```.An LLM is m
-00000510: 6f72 6520 6361 7061 626c 6520 6966 2079  ore capable if y
-00000520: 6f75 2063 7265 6174 6520 6120 636f 6e74  ou create a cont
-00000530: 6578 742f 6469 7374 7269 6275 7469 6f6e  ext/distribution
-00000540: 2073 6869 6674 2073 7065 6369 616c 697a   shift specializ
-00000550: 6564 2074 6f20 736f 6d65 2074 6172 6765  ed to some targe
-00000560: 7420 7461 736b 732e 0a60 6060 0a53 6164  t tasks..```.Sad
-00000570: 6c79 2c20 7468 6572 6520 6973 206e 6f20  ly, there is no 
-00000580: 7369 6c76 6572 2062 756c 6c65 7420 666f  silver bullet fo
-00000590: 7220 6167 656e 7420 7370 6563 6961 6c69  r agent speciali
-000005a0: 7a61 7469 6f6e 2e20 466f 7220 6578 616d  zation. For exam
-000005b0: 706c 652c 2079 6f75 2063 616e 200a 2d20  ple, you can .- 
-000005c0: 5369 6d70 6c79 2061 6464 2060 4c65 7427  Simply add `Let'
-000005d0: 7320 7468 696e 6b20 7374 6570 2062 7920  s think step by 
-000005e0: 7374 6570 2e60 2069 6e20 796f 7572 202a  step.` in your *
-000005f0: 2a70 726f 6d70 742a 2a20 666f 7220 6d6f  *prompt** for mo
-00000600: 7265 2061 6363 7572 6174 6520 4d61 7468  re accurate Math
-00000610: 2051 412e 0a2d 2047 6976 6520 6120 2a2a   QA..- Give a **
-00000620: 6665 772d 7368 6f74 2a2a 2065 7865 6d70  few-shot** exemp
-00000630: 6c61 7220 696e 2079 6f75 7220 7072 6f6d  lar in your prom
-00000640: 7074 2074 6f20 6775 6964 6520 6120 6265  pt to guide a be
-00000650: 7474 6572 2072 6561 736f 6e69 6e67 2074  tter reasoning t
-00000660: 7261 6a65 6374 6f72 7920 666f 7220 6e6f  rajectory for no
-00000670: 7665 6c20 706c 6f74 7469 6e67 2e0a 2d20  vel plotting..- 
-00000680: 5375 7065 7276 6973 6520 2a2a 6669 6e65  Supervise **fine
-00000690: 2d74 756e 696e 672a 2a20 2853 4654 2920  -tuning** (SFT) 
-000006a0: 796f 7572 2037 3042 2060 6c6c 616d 6132  your 70B `llama2
-000006b0: 6020 6c69 6b65 205b 7468 6973 5d28 6874  ` like [this](ht
-000006c0: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
-000006d0: 6162 732f 3233 3035 2e32 3030 3530 2920  abs/2305.20050) 
-000006e0: 746f 206d 6174 6368 2072 6561 736f 6e69  to match reasoni
-000006f0: 6e67 206f 6620 3137 3542 2047 5054 2d33  ng of 175B GPT-3
-00000700: 2e35 2e0a 2d20 5475 6e65 2079 6f75 7220  .5..- Tune your 
-00000710: 6167 656e 7420 2a2a 7061 7261 6469 676d  agent **paradigm
-00000720: 2a2a 206c 696b 6520 7468 6973 205b 6465  ** like this [de
-00000730: 6d6f 5d28 6874 7470 733a 2f2f 7777 772e  mo](https://www.
-00000740: 796f 7574 7562 652e 636f 6d2f 7761 7463  youtube.com/watc
-00000750: 683f 763d 6469 4a34 4944 6154 345a 3429  h?v=diJ4IDaT4Z4)
-00000760: 2074 6f20 6561 7369 6c79 2068 616c 6620   to easily half 
-00000770: 7468 6520 6578 6563 7574 696f 6e20 7469  the execution ti
-00000780: 6d65 2066 6f72 2053 6561 6368 2026 2053  me for Seach & S
-00000790: 756d 6d61 7269 7a65 2e0a 2d20 416e 6420  ummarize..- And 
-000007a0: 6d6f 7265 202e 2e2e 0a0a 4973 6e27 7420  more .....Isn't 
-000007b0: 6974 2062 6561 7574 6966 756c 2069 6620  it beautiful if 
-000007c0: 6f6e 6520 7368 6172 6573 2068 6973 2073  one shares his s
-000007d0: 7065 6369 616c 697a 6564 2069 6e74 656c  pecialized intel
-000007e0: 6c69 6765 6e63 652c 2061 6c6c 6f77 696e  ligence, allowin
-000007f0: 6720 6f74 6865 7273 2074 6f20 7265 7072  g others to repr
-00000800: 6f64 7563 652c 2062 7569 6c64 206f 6e2c  oduce, build on,
-00000810: 206f 7220 696e 7465 7261 6374 2077 6974   or interact wit
-00000820: 6820 6974 2061 7420 6561 7365 3f20 f09f  h it at ease? ..
-00000830: a497 2054 6869 7320 6265 6c69 6566 2069  .. This belief i
-00000840: 6e73 7069 7265 7320 7573 2074 6f20 6275  nspires us to bu
-00000850: 696c 6420 4765 6e74 6f70 6961 2c20 0a2a  ild Gentopia, .*
-00000860: 2a64 6573 6967 6e65 6420 666f 7220 6167  *designed for ag
-00000870: 656e 7420 2a73 7065 6369 616c 697a 6174  ent *specializat
-00000880: 696f 6e2c 2073 6861 7269 6e67 2c20 616e  ion, sharing, an
-00000890: 6420 696e 7465 7261 6374 696f 6e2c 2a20  d interaction,* 
-000008a0: 746f 2061 6368 6965 7665 2063 6f6c 6c65  to achieve colle
-000008b0: 6374 6976 6520 6772 6f77 7468 2074 6f77  ctive growth tow
-000008c0: 6172 6473 2067 7265 6174 6572 2069 6e74  ards greater int
-000008d0: 656c 6c69 6765 6e63 652a 2a2e 0a0a 2323  elligence**...##
-000008e0: 2043 6f72 6520 4665 6174 7572 6573 20f0   Core Features .
-000008f0: 9f92 a10a 0a2d 20e2 9a99 efb8 8f20 436f  .....- ...... Co
-00000900: 6e66 6967 2d64 7269 7665 6e20 6167 656e  nfig-driven agen
-00000910: 7420 6173 7365 6d62 6c69 6e67 2061 6e64  t assembling and
-00000920: 2063 6861 742e 0a2d 20f0 9f9a 8020 4c61   chat..- .... La
-00000930: 7267 6520 616d 6f75 6e74 206f 6620 7072  rge amount of pr
-00000940: 6562 7569 6c74 2061 6765 6e74 2074 7970  ebuilt agent typ
-00000950: 6573 2c20 4c4c 4d20 636c 6965 6e74 732c  es, LLM clients,
-00000960: 2074 6f6f 6c73 2c20 6d65 6d6f 7279 2073   tools, memory s
-00000970: 7973 7465 6d73 2c20 616e 6420 6d6f 7265  ystems, and more
-00000980: 2e0a 2d20 f09f aab6 204c 6967 6874 7765  ..- .... Lightwe
-00000990: 6967 6874 2061 6e64 2068 6967 686c 7920  ight and highly 
-000009a0: 6578 7465 6e73 6962 6c65 2069 6d70 6c65  extensible imple
-000009b0: 6d65 6e74 6174 696f 6e20 6f66 2065 7373  mentation of ess
-000009c0: 656e 7469 616c 2063 6f6d 706f 6e65 6e74  ential component
-000009d0: 732e 0a2d 20f0 9fa7 aa20 416c 6967 6e69  s..- .... Aligni
-000009e0: 6e67 2077 6974 6820 7374 6174 652d 6f66  ng with state-of
-000009f0: 2d74 6865 2d61 7274 2041 4920 7265 7365  -the-art AI rese
-00000a00: 6172 6368 2e0a 2d20 f09f a49d 2045 6e61  arch..- .... Ena
-00000a10: 626c 696e 6720 6d75 6c74 692d 6167 656e  bling multi-agen
-00000a20: 7420 696e 7465 7261 6374 696f 6e73 2e0a  t interactions..
-00000a30: 2d20 f09f a681 2055 6e69 7175 6520 706c  - .... Unique pl
-00000a40: 6174 666f 726d 206f 6620 6167 656e 7420  atform of agent 
-00000a50: 7a6f 6f20 616e 6420 6576 616c 2062 656e  zoo and eval ben
-00000a60: 6368 6d61 726b 2e0a 0a23 2320 5175 6963  chmark...## Quic
-00000a70: 6b20 5374 6172 7420 f09f 9bab 0a60 6060  k Start .....```
-00000a80: 0a70 6970 2069 6e73 7461 6c6c 2067 656e  .pip install gen
-00000a90: 746f 7069 610a 6060 600a 6f72 2069 6620  topia.```.or if 
-00000aa0: 796f 7520 7761 6e74 2074 6f20 6275 696c  you want to buil
-00000ab0: 6420 7769 7468 206f 7065 6e20 4c4c 4d73  d with open LLMs
-00000ac0: 206c 6f63 616c 6c79 20f0 9f91 8920 6070   locally .... `p
-00000ad0: 6970 2069 6e73 7461 6c6c 2067 656e 746f  ip install gento
-00000ae0: 7069 615b 6875 6767 696e 6766 6163 655d  pia[huggingface]
-00000af0: 600a 0a46 6972 7374 2074 696d 6520 746f  `..First time to
-00000b00: 2047 656e 746f 7069 613f 2047 7261 6220   Gentopia? Grab 
-00000b10: 6120 636f 6666 6565 20e2 9895 2061 6e64  a coffee ... and
-00000b20: 2074 616b 6520 7e20 3130 206d 696e 7320   take ~ 10 mins 
-00000b30: 746f 2063 6865 636b 206f 7574 2074 6865  to check out the
-00000b40: 2066 6f6c 6c6f 7769 6e67 206d 696e 642d   following mind-
-00000b50: 626c 6f77 696e 6720 6465 6d6f 7320 f09f  blowing demos ..
-00000b60: 9180 20f0 9fa4 af0a 0a3c 6469 7620 7374  .. ......<div st
-00000b70: 796c 653d 2264 6973 706c 6179 3a20 666c  yle="display: fl
-00000b80: 6578 3b20 6a75 7374 6966 792d 636f 6e74  ex; justify-cont
-00000b90: 656e 743a 2073 7061 6365 2d61 726f 756e  ent: space-aroun
-00000ba0: 643b 223e 0a20 200a 3c61 2068 7265 663d  d;">.  .<a href=
-00000bb0: 2268 7474 7073 3a2f 2f77 7777 2e79 6f75  "https://www.you
-00000bc0: 7475 6265 2e63 6f6d 2f77 6174 6368 3f76  tube.com/watch?v
-00000bd0: 3d37 645a 335a 7673 4937 7377 2220 7461  =7dZ3ZvsI7sw" ta
-00000be0: 7267 6574 3d22 5f62 6c61 6e6b 223e 0a20  rget="_blank">. 
-00000bf0: 203c 696d 6720 7372 633d 2268 7474 7073   <img src="https
-00000c00: 3a2f 2f69 6d67 2e79 6f75 7475 6265 2e63  ://img.youtube.c
-00000c10: 6f6d 2f76 692f 3764 5a33 5a76 7349 3773  om/vi/7dZ3ZvsI7s
-00000c20: 772f 6871 6465 6661 756c 742e 6a70 6722  w/hqdefault.jpg"
-00000c30: 2061 6c74 3d22 5669 6465 6f20 3122 2073   alt="Video 1" s
-00000c40: 7479 6c65 3d22 7769 6474 683a 3332 253b  tyle="width:32%;
-00000c50: 223e 0a3c 2f61 3e0a 0a3c 6120 6872 6566  ">.</a>..<a href
-00000c60: 3d22 6874 7470 733a 2f2f 7777 772e 796f  ="https://www.yo
-00000c70: 7574 7562 652e 636f 6d2f 7761 7463 683f  utube.com/watch?
-00000c80: 763d 5854 7376 3970 6b36 414f 4122 2074  v=XTsv9pk6AOA" t
-00000c90: 6172 6765 743d 225f 626c 616e 6b22 3e0a  arget="_blank">.
-00000ca0: 2020 3c69 6d67 2073 7263 3d22 6874 7470    <img src="http
-00000cb0: 733a 2f2f 696d 672e 796f 7574 7562 652e  s://img.youtube.
-00000cc0: 636f 6d2f 7669 2f58 5473 7639 706b 3641  com/vi/XTsv9pk6A
-00000cd0: 4f41 2f68 7164 6566 6175 6c74 2e6a 7067  OA/hqdefault.jpg
-00000ce0: 2220 616c 743d 2256 6964 656f 2032 2220  " alt="Video 2" 
-00000cf0: 7374 796c 653d 2277 6964 7468 3a33 3225  style="width:32%
-00000d00: 3b22 3e0a 3c2f 613e 0a0a 3c61 2068 7265  ;">.</a>..<a hre
-00000d10: 663d 2268 7474 7073 3a2f 2f77 7777 2e79  f="https://www.y
-00000d20: 6f75 7475 6265 2e63 6f6d 2f77 6174 6368  outube.com/watch
-00000d30: 3f76 3d64 694a 3449 4461 5434 5a34 2220  ?v=diJ4IDaT4Z4" 
-00000d40: 7461 7267 6574 3d22 5f62 6c61 6e6b 223e  target="_blank">
-00000d50: 0a20 203c 696d 6720 7372 633d 2268 7474  .  <img src="htt
-00000d60: 7073 3a2f 2f69 6d67 2e79 6f75 7475 6265  ps://img.youtube
-00000d70: 2e63 6f6d 2f76 692f 6469 4a34 4944 6154  .com/vi/diJ4IDaT
-00000d80: 345a 342f 6871 6465 6661 756c 742e 6a70  4Z4/hqdefault.jp
-00000d90: 6722 2061 6c74 3d22 5669 6465 6f20 3322  g" alt="Video 3"
-00000da0: 2073 7479 6c65 3d22 7769 6474 683a 3332   style="width:32
-00000db0: 253b 223e 0a3c 2f61 3e0a 0a3c 2f64 6976  %;">.</a>..</div
-00000dc0: 3e0a 0a28 4a75 6d70 2074 6f20 7468 6520  >..(Jump to the 
-00000dd0: 7468 6972 6420 6f6e 6520 6966 2079 6f75  third one if you
-00000de0: 206f 6e6c 7920 6861 7665 2033 206d 696e   only have 3 min
-00000df0: 7320 f09f a4ab 290a 0a23 2320 446f 6375  s ....)..## Docu
-00000e00: 6d65 6e74 6174 696f 6e20 f09f 9396 0a53  mentation .....S
-00000e10: 6565 205b 6865 7265 5d28 6874 7470 733a  ee [here](https:
-00000e20: 2f2f 6765 6e74 6f70 6961 2e72 6561 6474  //gentopia.readt
-00000e30: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00000e40: 6573 742f 696e 6465 782e 6874 6d6c 2920  est/index.html) 
-00000e50: 666f 7220 6675 6c6c 2064 6f63 756d 656e  for full documen
-00000e60: 7461 7469 6f6e 2e0a 0af0 9f8c 9f20 4869  tation....... Hi
-00000e70: 6768 6c69 6768 7420 546f 7069 6373 200a  ghlight Topics .
-00000e80: 2d20 5b41 6765 6e74 2054 656d 706c 6174  - [Agent Templat
-00000e90: 6573 5d28 6874 7470 733a 2f2f 6765 6e74  es](https://gent
-00000ea0: 6f70 6961 2e72 6561 6474 6865 646f 6373  opia.readthedocs
-00000eb0: 2e69 6f2f 656e 2f6c 6174 6573 742f 7175  .io/en/latest/qu
-00000ec0: 6963 6b5f 7374 6172 742e 6874 6d6c 2376  ick_start.html#v
-00000ed0: 616e 696c 6c61 2d61 6765 6e74 290a 2d20  anilla-agent).- 
-00000ee0: 5b48 6965 7261 7263 6869 6361 6c20 4167  [Hierarchical Ag
-00000ef0: 656e 7473 5d28 6874 7470 733a 2f2f 6765  ents](https://ge
-00000f00: 6e74 6f70 6961 2e72 6561 6474 6865 646f  ntopia.readthedo
-00000f10: 6373 2e69 6f2f 656e 2f6c 6174 6573 742f  cs.io/en/latest/
-00000f20: 6167 656e 745f 636f 6d70 6f6e 656e 7473  agent_components
-00000f30: 2e68 746d 6c23 6167 656e 742d 6173 2d70  .html#agent-as-p
-00000f40: 6c75 6769 6e29 0a2d 205b 556e 6971 7565  lugin).- [Unique
-00000f50: 2041 6765 6e74 2042 656e 6368 6d61 726b   Agent Benchmark
-00000f60: 5d28 6874 7470 733a 2f2f 6765 6e74 6f70  ](https://gentop
-00000f70: 6961 2e72 6561 6474 6865 646f 6373 2e69  ia.readthedocs.i
-00000f80: 6f2f 656e 2f6c 6174 6573 742f 6765 6e74  o/en/latest/gent
-00000f90: 706f 6f6c 2e68 746d 6c23 6167 656e 742d  pool.html#agent-
-00000fa0: 6576 616c 7561 7469 6f6e 290a 2d20 5b4f  evaluation).- [O
-00000fb0: 7065 6e20 4c4c 4d20 5375 7070 6f72 7473  pen LLM Supports
-00000fc0: 5d28 6874 7470 733a 2f2f 6765 6e74 6f70  ](https://gentop
-00000fd0: 6961 2e72 6561 6474 6865 646f 6373 2e69  ia.readthedocs.i
-00000fe0: 6f2f 656e 2f6c 6174 6573 742f 6167 656e  o/en/latest/agen
-00000ff0: 745f 636f 6d70 6f6e 656e 7473 2e68 746d  t_components.htm
-00001000: 6c23 6875 6767 696e 6766 6163 652d 6f70  l#huggingface-op
-00001010: 656e 2d6c 6c6d 7329 0a2d 205b 4869 6768  en-llms).- [High
-00001020: 2d50 6572 666f 726d 616e 6365 204d 656d  -Performance Mem
-00001030: 6f72 795d 2868 7474 7073 3a2f 2f67 656e  ory](https://gen
-00001040: 746f 7069 612e 7265 6164 7468 6564 6f63  topia.readthedoc
-00001050: 732e 696f 2f65 6e2f 6c61 7465 7374 2f61  s.io/en/latest/a
-00001060: 6765 6e74 5f63 6f6d 706f 6e65 6e74 732e  gent_components.
-00001070: 6874 6d6c 236c 6f6e 672d 7368 6f72 742d  html#long-short-
-00001080: 7465 726d 2d6d 656d 6f72 7929 0a0a 2323  term-memory)..##
-00001090: 2042 7569 6c64 2077 6974 6820 7573 20f0   Build with us .
-000010a0: 9f8c 8e0a 0a50 6172 7469 6369 7061 7465  .....Participate
-000010b0: 2069 6e20 7468 6973 2055 746f 7069 6120   in this Utopia 
-000010c0: 6f66 2073 7570 6572 696e 7465 6c6c 6967  of superintellig
-000010d0: 656e 6365 2061 6e64 2068 656c 7020 6974  ence and help it
-000010e0: 2067 726f 7773 2120 4173 2061 2066 756c   grows! As a ful
-000010f0: 6c79 206f 7065 6e2d 736f 7572 6365 2070  ly open-source p
-00001100: 726f 6a65 6374 2c20 7765 2064 6576 656c  roject, we devel
-00001110: 6f70 2075 6e64 6572 2070 7562 6c69 6320  op under public 
-00001120: 6164 7669 6365 2c20 6964 6561 732c 2061  advice, ideas, a
-00001130: 6e64 2073 7570 6572 7669 7369 6f6e 2e20  nd supervision. 
-00001140: 4d65 616e 7768 696c 652c 2068 6572 6520  Meanwhile, here 
-00001150: 6172 6520 7761 7973 2079 6f75 206d 6179  are ways you may
-00001160: 2063 6f6e 7472 6962 7574 6520 746f 2047   contribute to G
-00001170: 656e 746f 7069 612e 0a0a 2d20 f09f 909b  entopia...- ....
-00001180: 2050 6f73 7420 616e 205b 6973 7375 655d   Post an [issue]
-00001190: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
-000011a0: 636f 6d2f 4765 6e74 6f70 6961 2d41 492f  com/Gentopia-AI/
-000011b0: 4765 6e74 6f70 6961 2f69 7373 7565 7329  Gentopia/issues)
-000011c0: 2072 6571 7565 7374 696e 6720 6e65 6365   requesting nece
-000011d0: 7373 6172 7920 6275 6720 6669 7865 732c  ssary bug fixes,
-000011e0: 2061 6464 6974 696f 6e61 6c20 6665 6174   additional feat
-000011f0: 7572 6573 2c20 6f72 2072 6f61 646d 6170  ures, or roadmap
-00001200: 2073 7567 6765 7374 696f 6e73 2e20 2843   suggestions. (C
-00001210: 6865 636b 2063 6c6f 7365 6420 6f6e 6573  heck closed ones
-00001220: 2066 6972 7374 290a 2d20 f09f 8eaf 204f   first).- .... O
-00001230: 7572 2064 6576 2074 6561 6d20 6d65 6574  ur dev team meet
-00001240: 7320 7765 656b 6c79 2074 6f20 6772 6f6f  s weekly to groo
-00001250: 6d20 5b62 6163 6b6c 6f67 5d28 6874 7470  m [backlog](http
-00001260: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f6f  s://github.com/o
-00001270: 7267 732f 4765 6e74 6f70 6961 2d41 492f  rgs/Gentopia-AI/
-00001280: 7072 6f6a 6563 7473 2f31 2920 696e 746f  projects/1) into
-00001290: 2074 6963 6b65 7473 2e20 5768 696c 6520   tickets. While 
-000012a0: 7765 2077 6f72 6b20 6f6e 2074 6865 6d2c  we work on them,
-000012b0: 2079 6f75 2063 616e 2070 6963 6b20 7570   you can pick up
-000012c0: 206f 7468 6572 7320 616e 6420 6372 6561   others and crea
-000012d0: 7465 2061 205b 5075 6c6c 2052 6571 7565  te a [Pull Reque
-000012e0: 7374 5d28 6874 7470 733a 2f2f 6769 7468  st](https://gith
-000012f0: 7562 2e63 6f6d 2f47 656e 746f 7069 612d  ub.com/Gentopia-
-00001300: 4149 2f47 656e 746f 7069 612f 7075 6c6c  AI/Gentopia/pull
-00001310: 7329 2074 6f20 7265 7175 6573 7420 6120  s) to request a 
-00001320: 6d65 7267 652e 2057 6520 616c 7761 7973  merge. We always
-00001330: 2077 656c 636f 6d65 206e 6577 206d 656d   welcome new mem
-00001340: 6265 7273 2069 6e20 7468 6973 2077 6179  bers in this way
-00001350: 2e0a 2d20 f09f a49d 2053 6861 7265 2079  ..- .... Share y
-00001360: 6f75 7220 7370 6563 6961 6c69 7a65 6420  our specialized 
-00001370: 6167 656e 7420 746f 205b 4765 6e74 506f  agent to [GentPo
-00001380: 6f6c 5d28 6874 7470 733a 2f2f 6769 7468  ol](https://gith
-00001390: 7562 2e63 6f6d 2f47 656e 746f 7069 612d  ub.com/Gentopia-
-000013a0: 4149 2f47 656e 7450 6f6f 6c29 2120 4372  AI/GentPool)! Cr
-000013b0: 6561 7465 2061 6e20 4167 656e 7420 5052  eate an Agent PR
-000013c0: 2028 5b65 7861 6d70 6c65 5d28 2929 2074   ([example]()) t
-000013d0: 6f20 6d65 7267 6520 796f 7572 2077 656c  o merge your wel
-000013e0: 6c2d 7475 6e65 6420 6167 656e 7420 696e  l-tuned agent in
-000013f0: 746f 2074 6865 2070 6f6f 6c2e 2054 6869  to the pool. Thi
-00001400: 7320 616c 6c6f 7773 206f 7468 6572 7320  s allows others 
-00001410: 746f 2075 7365 206f 7220 6275 696c 6420  to use or build 
-00001420: 7570 6f6e 2079 6f75 7220 6167 656e 742e  upon your agent.
-00001430: 200a 2d20 e2ad 9020 4865 6c70 2075 7320   .- ... Help us 
-00001440: 7370 7265 6164 2120 4769 7665 2075 7320  spread! Give us 
-00001450: 6120 7374 6172 2c20 666f 6c6c 6f77 2075  a star, follow u
-00001460: 7320 6f6e 205b 5477 6974 7465 725d 2868  s on [Twitter](h
-00001470: 7474 7073 3a2f 2f74 7769 7474 6572 2e63  ttps://twitter.c
-00001480: 6f6d 2f47 656e 746f 7069 6141 4929 2c20  om/GentopiaAI), 
-00001490: 6a6f 696e 206f 7572 205b 4469 7363 6f72  join our [Discor
-000014a0: 645d 2868 7474 7073 3a2f 2f64 6973 636f  d](https://disco
-000014b0: 7264 2e67 672f 4153 5050 394d 5939 514b  rd.gg/ASPP9MY9QK
-000014c0: 292c 2061 6e64 2073 6861 7265 2077 6974  ), and share wit
-000014d0: 6820 796f 7572 2066 7269 656e 6473 2120  h your friends! 
-000014e0: 200a 0a0a                                 ...
+00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
+00000010: 3a20 322e 310a 4e61 6d65 3a20 6765 6e74  : 2.1.Name: gent
+00000020: 6f70 6961 0a56 6572 7369 6f6e 3a20 302e  opia.Version: 0.
+00000030: 302e 320a 5375 6d6d 6172 793a 2047 656e  0.2.Summary: Gen
+00000040: 746f 7069 6120 7072 6f76 6964 6573 2065  topia provides e
+00000050: 7874 656e 7369 7665 2075 7469 6c69 7469  xtensive utiliti
+00000060: 6573 2074 6f20 6173 7365 6d62 6c65 7320  es to assembles 
+00000070: 414c 4d20 6167 656e 7473 2064 7269 7665  ALM agents drive
+00000080: 6e20 6279 2063 6f6e 6669 6773 2e0a 486f  n by configs..Ho
+00000090: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
+000000a0: 2f67 6974 6875 622e 636f 6d2f 4765 6e74  /github.com/Gent
+000000b0: 6f70 6961 2d41 492f 4765 6e74 6f70 6961  opia-AI/Gentopia
+000000c0: 0a41 7574 686f 723a 2062 696c 6c78 6266  .Author: billxbf
+000000d0: 0a41 7574 686f 722d 656d 6169 6c3a 2062  .Author-email: b
+000000e0: 696c 6c78 6266 4067 6d61 696c 2e63 6f6d  illxbf@gmail.com
+000000f0: 0a4c 6963 656e 7365 3a20 4d49 5420 6c69  .License: MIT li
+00000100: 6365 6e73 650a 4465 7363 7269 7074 696f  cense.Descriptio
+00000110: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
+00000120: 7465 7874 2f6d 6172 6b64 6f77 6e0a 5072  text/markdown.Pr
+00000130: 6f76 6964 6573 2d45 7874 7261 3a20 6875  ovides-Extra: hu
+00000140: 6767 696e 6766 6163 650a 4c69 6365 6e73  ggingface.Licens
+00000150: 652d 4669 6c65 3a20 4c49 4345 4e53 450a  e-File: LICENSE.
+00000160: 0a23 2047 656e 746f 7069 6120 0af0 9f8c  .# Gentopia ....
+00000170: 8e20 2a43 6f6c 6c65 6374 6976 6520 4772  . *Collective Gr
+00000180: 6f77 7468 206f 6620 496e 7465 6c6c 6967  owth of Intellig
+00000190: 656e 7420 4167 656e 7473 2e2a 20f0 9fa6  ent Agents.* ...
+000001a0: 990a 0a0a 5b21 5b4c 6963 656e 7365 3a20  ....[![License: 
+000001b0: 4d49 545d 2868 7474 7073 3a2f 2f69 6d67  MIT](https://img
+000001c0: 2e73 6869 656c 6473 2e69 6f2f 6261 6467  .shields.io/badg
+000001d0: 652f 4c69 6365 6e73 652d 4d49 542d 7965  e/License-MIT-ye
+000001e0: 6c6c 6f77 2e73 7667 295d 2868 7474 7073  llow.svg)](https
+000001f0: 3a2f 2f6f 7065 6e73 6f75 7263 652e 6f72  ://opensource.or
+00000200: 672f 6c69 6365 6e73 6573 2f4d 4954 290a  g/licenses/MIT).
+00000210: 215b 5374 6174 6963 2042 6164 6765 5d28  ![Static Badge](
+00000220: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000230: 6c64 732e 696f 2f62 6164 6765 2f72 656c  lds.io/badge/rel
+00000240: 6561 7365 2d62 6574 612d 626c 7565 290a  ease-beta-blue).
+00000250: 5b21 5b53 7461 7469 6320 4261 6467 655d  [![Static Badge]
+00000260: 2868 7474 7073 3a2f 2f69 6d67 2e73 6869  (https://img.shi
+00000270: 656c 6473 2e69 6f2f 6261 6467 652f 446f  elds.io/badge/Do
+00000280: 6375 6d65 6e74 6174 696f 6e2d 3841 3242  cumentation-8A2B
+00000290: 4532 295d 2868 7474 7073 3a2f 2f67 656e  E2)](https://gen
+000002a0: 746f 7069 612e 7265 6164 7468 6564 6f63  topia.readthedoc
+000002b0: 732e 696f 2f65 6e2f 6c61 7465 7374 2f69  s.io/en/latest/i
+000002c0: 6e64 6578 2e68 746d 6c29 0a5b 215b 5374  ndex.html).[![St
+000002d0: 6174 6963 2042 6164 6765 5d28 6874 7470  atic Badge](http
+000002e0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000002f0: 696f 2f62 6164 6765 2f47 656e 7450 6f6f  io/badge/GentPoo
+00000300: 6c2d 626c 7565 295d 2868 7474 7073 3a2f  l-blue)](https:/
+00000310: 2f67 6974 6875 622e 636f 6d2f 4765 6e74  /github.com/Gent
+00000320: 6f70 6961 2d41 492f 4765 6e74 506f 6f6c  opia-AI/GentPool
+00000330: 290a 5b21 5b53 7461 7469 6320 4261 6467  ).[![Static Badg
+00000340: 655d 2868 7474 7073 3a2f 2f69 6d67 2e73  e](https://img.s
+00000350: 6869 656c 6473 2e69 6f2f 6261 6467 652f  hields.io/badge/
+00000360: 6261 636b 6c6f 672d 6772 6579 295d 2868  backlog-grey)](h
+00000370: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000380: 6d2f 6f72 6773 2f47 656e 746f 7069 612d  m/orgs/Gentopia-
+00000390: 4149 2f70 726f 6a65 6374 732f 3129 0a5b  AI/projects/1).[
+000003a0: 215b 4f70 656e 2049 7373 7565 735d 2868  ![Open Issues](h
+000003b0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000003c0: 6473 2e69 6f2f 6769 7468 7562 2f69 7373  ds.io/github/iss
+000003d0: 7565 732d 7261 772f 4765 6e74 6f70 6961  ues-raw/Gentopia
+000003e0: 2d41 492f 4765 6e74 6f70 6961 295d 2868  -AI/Gentopia)](h
+000003f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000400: 6d2f 4765 6e74 6f70 6961 2d41 492f 4765  m/Gentopia-AI/Ge
+00000410: 6e74 6f70 6961 2f69 7373 7565 7329 0a5b  ntopia/issues).[
+00000420: 215b 4465 7065 6e64 656e 6379 2053 7461  ![Dependency Sta
+00000430: 7475 735d 2868 7474 7073 3a2f 2f69 6d67  tus](https://img
+00000440: 2e73 6869 656c 6473 2e69 6f2f 6c69 6272  .shields.io/libr
+00000450: 6172 6965 7369 6f2f 6769 7468 7562 2f47  ariesio/github/G
+00000460: 656e 746f 7069 612d 4149 2f47 656e 746f  entopia-AI/Gento
+00000470: 7069 6129 5d28 6874 7470 733a 2f2f 6c69  pia)](https://li
+00000480: 6272 6172 6965 732e 696f 2f67 6974 6875  braries.io/githu
+00000490: 622f 4765 6e74 6f70 6961 2d41 492f 4765  b/Gentopia-AI/Ge
+000004a0: 6e74 6f70 6961 290a 0a5b 215b 5477 6974  ntopia)..[![Twit
+000004b0: 7465 7220 466f 6c6c 6f77 5d28 6874 7470  ter Follow](http
+000004c0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000004d0: 696f 2f74 7769 7474 6572 2f66 6f6c 6c6f  io/twitter/follo
+000004e0: 772f 4765 6e74 6f70 6961 4149 295d 2868  w/GentopiaAI)](h
+000004f0: 7474 7073 3a2f 2f74 7769 7474 6572 2e63  ttps://twitter.c
+00000500: 6f6d 2f47 656e 746f 7069 6141 4929 0a5b  om/GentopiaAI).[
+00000510: 215b 5d28 6874 7470 733a 2f2f 6463 6261  ![](https://dcba
+00000520: 6467 652e 7665 7263 656c 2e61 7070 2f61  dge.vercel.app/a
+00000530: 7069 2f73 6572 7665 722f 4153 5050 394d  pi/server/ASPP9M
+00000540: 5939 514b 3f63 6f6d 7061 6374 3d74 7275  Y9QK?compact=tru
+00000550: 6526 7374 796c 653d 666c 6174 295d 2868  e&style=flat)](h
+00000560: 7474 7073 3a2f 2f64 6973 636f 7264 2e67  ttps://discord.g
+00000570: 672f 4153 5050 394d 5939 514b 290a 5b21  g/ASPP9MY9QK).[!
+00000580: 5b59 6f75 5475 6265 2043 6861 6e6e 656c  [YouTube Channel
+00000590: 2053 7562 7363 7269 6265 7273 5d28 6874   Subscribers](ht
+000005a0: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+000005b0: 732e 696f 2f79 6f75 7475 6265 2f63 6861  s.io/youtube/cha
+000005c0: 6e6e 656c 2f76 6965 7773 2f55 4339 5143  nnel/views/UC9QC
+000005d0: 6a63 7348 4a56 4b6a 4b5a 325a 6d72 7138  jcsHJVKjKZ2Zmrq8
+000005e0: 3376 4129 5d28 6874 7470 733a 2f2f 7777  3vA)](https://ww
+000005f0: 772e 796f 7574 7562 652e 636f 6d2f 6368  w.youtube.com/ch
+00000600: 616e 6e65 6c2f 5543 3951 436a 6373 484a  annel/UC9QCjcsHJ
+00000610: 564b 6a4b 5a32 5a6d 7271 3833 7641 290a  VKjKZ2Zmrq83vA).
+00000620: 5b21 5b47 6974 4875 6220 7374 6172 2063  [![GitHub star c
+00000630: 6861 7274 5d28 6874 7470 733a 2f2f 696d  hart](https://im
+00000640: 672e 7368 6965 6c64 732e 696f 2f67 6974  g.shields.io/git
+00000650: 6875 622f 7374 6172 732f 4765 6e74 6f70  hub/stars/Gentop
+00000660: 6961 2d41 492f 4765 6e74 6f70 6961 3f73  ia-AI/Gentopia?s
+00000670: 7479 6c65 3d73 6f63 6961 6c29 5d28 6874  tyle=social)](ht
+00000680: 7470 733a 2f2f 7374 6172 2d68 6973 746f  tps://star-histo
+00000690: 7279 2e63 6f6d 2f47 656e 746f 7069 612d  ry.com/Gentopia-
+000006a0: 4149 2f47 656e 746f 7069 6129 0a0a 0a0a  AI/Gentopia)....
+000006b0: 0a47 656e 746f 7069 6120 6973 2061 206c  .Gentopia is a l
+000006c0: 6967 6874 7765 6967 6874 2061 6e64 2065  ightweight and e
+000006d0: 7874 656e 7369 626c 6520 6672 616d 6577  xtensible framew
+000006e0: 6f72 6b20 666f 7220 4c4c 4d2d 6472 6976  ork for LLM-driv
+000006f0: 656e 2041 6765 6e74 7320 616e 6420 5b41  en Agents and [A
+00000700: 4c4d 5d28 6874 7470 733a 2f2f 6172 7869  LM](https://arxi
+00000710: 762e 6f72 672f 6162 732f 3233 3032 2e30  v.org/abs/2302.0
+00000720: 3738 3432 2920 2072 6573 6561 7263 682e  7842)  research.
+00000730: 2049 7420 7072 6f76 6964 6573 2065 7373   It provides ess
+00000740: 656e 7469 616c 2063 6f6d 706f 6e65 6e74  ential component
+00000750: 7320 746f 2062 7569 6c64 2c20 7465 7374  s to build, test
+00000760: 2061 6e64 2065 7661 6c75 6174 6520 6167   and evaluate ag
+00000770: 656e 7473 2e20 4174 2069 7473 2063 6f72  ents. At its cor
+00000780: 652c 2047 656e 746f 7069 6120 6169 6d73  e, Gentopia aims
+00000790: 2074 6f20 6173 7365 6d62 6c65 2061 6e20   to assemble an 
+000007a0: 6167 656e 7420 7769 7468 2061 2073 696e  agent with a sin
+000007b0: 676c 6520 636f 6e66 6967 2c20 7468 7573  gle config, thus
+000007c0: 206d 696e 696d 697a 696e 6720 796f 7572   minimizing your
+000007d0: 2065 6666 6f72 7420 696e 2062 7569 6c64   effort in build
+000007e0: 696e 672c 2074 756e 696e 672c 2061 6e64  ing, tuning, and
+000007f0: 2073 6861 7269 6e67 2061 6765 6e74 732e   sharing agents.
+00000800: 200a 0a47 656e 746f 7069 6120 6d61 696e   ..Gentopia main
+00000810: 7461 696e 7320 616e 2061 6765 6e74 2070  tains an agent p
+00000820: 6c61 7466 6f72 6d20 5b47 656e 7450 6f6f  latform [GentPoo
+00000830: 6c5d 2868 7474 7073 3a2f 2f67 6974 6875  l](https://githu
+00000840: 622e 636f 6d2f 4765 6e74 6f70 6961 2d41  b.com/Gentopia-A
+00000850: 492f 4765 6e74 506f 6f6c 2920 746f 2073  I/GentPool) to s
+00000860: 6861 7265 2073 7065 6369 616c 697a 6564  hare specialized
+00000870: 2061 6765 6e74 732c 2077 6865 7265 2079   agents, where y
+00000880: 6f75 7220 6167 656e 7420 2a69 6e74 6572  our agent *inter
+00000890: 6163 7473 2a20 7769 7468 206f 7468 6572  acts* with other
+000008a0: 2061 6765 6e74 7320 6279 2063 6c6f 6e69   agents by cloni
+000008b0: 6e67 2c20 6869 6572 6172 6368 6963 616c  ng, hierarchical
+000008c0: 2070 6c75 672d 696e 2c20 6f72 2073 6861   plug-in, or sha
+000008d0: 7269 6e67 2065 6e76 6972 6f6e 6d65 6e74  ring environment
+000008e0: 2e20 5765 2070 726f 7669 6465 2061 2075  . We provide a u
+000008f0: 6e69 7175 6520 6167 656e 7420 5b62 656e  nique agent [ben
+00000900: 6368 6d61 726b 5d28 6874 7470 733a 2f2f  chmark](https://
+00000910: 6765 6e74 6f70 6961 2e72 6561 6474 6865  gentopia.readthe
+00000920: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+00000930: 742f 6765 6e74 706f 6f6c 2e68 746d 6c23  t/gentpool.html#
+00000940: 6167 656e 742d 6576 616c 7561 7469 6f6e  agent-evaluation
+00000950: 2920 666f 7220 686f 6c69 7374 6963 2065  ) for holistic e
+00000960: 7661 6c75 6174 696f 6e2e 200a 0a23 2320  valuation. ..## 
+00000970: 4d6f 7469 7661 7469 6f6e 20f0 9fa7 a00a  Motivation .....
+00000980: 4167 656e 7420 7072 6163 7469 7469 6f6e  Agent practition
+00000990: 6572 7320 7374 6172 7420 746f 2072 6561  ers start to rea
+000009a0: 6c69 7a65 2074 6865 2064 6966 6669 6375  lize the difficu
+000009b0: 6c74 7920 696e 2074 756e 696e 6720 6120  lty in tuning a 
+000009c0: 2277 656c 6c2d 726f 756e 6465 6422 2061  "well-rounded" a
+000009d0: 6765 6e74 2077 6974 6820 746f 6e73 206f  gent with tons o
+000009e0: 6620 746f 6f6c 7320 6f72 2069 6e73 7472  f tools or instr
+000009f0: 7563 7469 6f6e 7320 696e 2061 2073 696e  uctions in a sin
+00000a00: 676c 6520 6c61 7965 722e 0a52 6563 656e  gle layer..Recen
+00000a10: 7420 7374 7564 6965 7320 6c69 6b65 205b  t studies like [
+00000a20: 5469 6e79 5374 6f72 6965 735d 2868 7474  TinyStories](htt
+00000a30: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
+00000a40: 6273 2f32 3330 312e 3132 3732 3629 2c20  bs/2301.12726), 
+00000a50: 5b53 7065 6369 616c 697a 696e 6720 5265  [Specializing Re
+00000a60: 6173 6f6e 696e 675d 2868 7474 7073 3a2f  asoning](https:/
+00000a70: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00000a80: 3330 312e 3132 3732 3629 2c20 5b4c 6574  301.12726), [Let
+00000a90: 2773 2056 6572 6966 7920 5362 535d 2868  's Verify SbS](h
+00000aa0: 7474 7073 3a2f 2f61 7278 6976 2e6f 7267  ttps://arxiv.org
+00000ab0: 2f61 6273 2f32 3330 352e 3230 3035 3029  /abs/2305.20050)
+00000ac0: 2c20 5b52 6557 4f4f 5d28 6874 7470 733a  , [ReWOO](https:
+00000ad0: 2f2f 6172 7869 762e 6f72 672f 6162 732f  //arxiv.org/abs/
+00000ae0: 3233 3035 2e31 3833 3233 292c 2065 7463  2305.18323), etc
+00000af0: 2e20 616c 736f 2070 6f69 6e74 2075 7320  . also point us 
+00000b00: 746f 7761 7264 7320 616e 2069 6e74 7569  towards an intui
+00000b10: 7469 7665 2079 6574 2075 6e64 6572 7661  tive yet underva
+00000b20: 6c75 6564 2064 6972 6563 7469 6f6e 20f0  lued direction .
+00000b30: 9f91 8920 0a0a 6060 600a 416e 204c 4c4d  ... ..```.An LLM
+00000b40: 2069 7320 6d6f 7265 2063 6170 6162 6c65   is more capable
+00000b50: 2069 6620 796f 7520 6372 6561 7465 2061   if you create a
+00000b60: 2063 6f6e 7465 7874 2f64 6973 7472 6962   context/distrib
+00000b70: 7574 696f 6e20 7368 6966 7420 7370 6563  ution shift spec
+00000b80: 6961 6c69 7a65 6420 746f 2073 6f6d 6520  ialized to some 
+00000b90: 7461 7267 6574 2074 6173 6b73 2e0a 6060  target tasks..``
+00000ba0: 600a 5361 646c 792c 2074 6865 7265 2069  `.Sadly, there i
+00000bb0: 7320 6e6f 2073 696c 7665 7220 6275 6c6c  s no silver bull
+00000bc0: 6574 2066 6f72 2061 6765 6e74 2073 7065  et for agent spe
+00000bd0: 6369 616c 697a 6174 696f 6e2e 2046 6f72  cialization. For
+00000be0: 2065 7861 6d70 6c65 2c20 796f 7520 6361   example, you ca
+00000bf0: 6e20 0a2d 2053 696d 706c 7920 6164 6420  n .- Simply add 
+00000c00: 604c 6574 2773 2074 6869 6e6b 2073 7465  `Let's think ste
+00000c10: 7020 6279 2073 7465 702e 6020 696e 2079  p by step.` in y
+00000c20: 6f75 7220 2a2a 7072 6f6d 7074 2a2a 2066  our **prompt** f
+00000c30: 6f72 206d 6f72 6520 6163 6375 7261 7465  or more accurate
+00000c40: 204d 6174 6820 5141 2e0a 2d20 4769 7665   Math QA..- Give
+00000c50: 2061 202a 2a66 6577 2d73 686f 742a 2a20   a **few-shot** 
+00000c60: 6578 656d 706c 6172 2069 6e20 796f 7572  exemplar in your
+00000c70: 2070 726f 6d70 7420 746f 2067 7569 6465   prompt to guide
+00000c80: 2061 2062 6574 7465 7220 7265 6173 6f6e   a better reason
+00000c90: 696e 6720 7472 616a 6563 746f 7279 2066  ing trajectory f
+00000ca0: 6f72 206e 6f76 656c 2070 6c6f 7474 696e  or novel plottin
+00000cb0: 672e 0a2d 2053 7570 6572 7669 7365 202a  g..- Supervise *
+00000cc0: 2a66 696e 652d 7475 6e69 6e67 2a2a 2028  *fine-tuning** (
+00000cd0: 5346 5429 2079 6f75 7220 3730 4220 606c  SFT) your 70B `l
+00000ce0: 6c61 6d61 3260 206c 696b 6520 5b74 6869  lama2` like [thi
+00000cf0: 735d 2868 7474 7073 3a2f 2f61 7278 6976  s](https://arxiv
+00000d00: 2e6f 7267 2f61 6273 2f32 3330 352e 3230  .org/abs/2305.20
+00000d10: 3035 3029 2074 6f20 6d61 7463 6820 7265  050) to match re
+00000d20: 6173 6f6e 696e 6720 6f66 2031 3735 4220  asoning of 175B 
+00000d30: 4750 542d 332e 352e 0a2d 2054 756e 6520  GPT-3.5..- Tune 
+00000d40: 796f 7572 2061 6765 6e74 202a 2a70 6172  your agent **par
+00000d50: 6164 6967 6d2a 2a20 6c69 6b65 2074 6869  adigm** like thi
+00000d60: 7320 5b64 656d 6f5d 2868 7474 7073 3a2f  s [demo](https:/
+00000d70: 2f77 7777 2e79 6f75 7475 6265 2e63 6f6d  /www.youtube.com
+00000d80: 2f77 6174 6368 3f76 3d64 694a 3449 4461  /watch?v=diJ4IDa
+00000d90: 5434 5a34 2920 746f 2065 6173 696c 7920  T4Z4) to easily 
+00000da0: 6861 6c66 2074 6865 2065 7865 6375 7469  half the executi
+00000db0: 6f6e 2074 696d 6520 666f 7220 5365 6163  on time for Seac
+00000dc0: 6820 2620 5375 6d6d 6172 697a 652e 0a2d  h & Summarize..-
+00000dd0: 2041 6e64 206d 6f72 6520 2e2e 2e0a 0a49   And more .....I
+00000de0: 736e 2774 2069 7420 6265 6175 7469 6675  sn't it beautifu
+00000df0: 6c20 6966 206f 6e65 2073 6861 7265 7320  l if one shares 
+00000e00: 6869 7320 6566 666f 7274 2069 6e20 7370  his effort in sp
+00000e10: 6563 6961 6c69 7a65 6420 696e 7465 6c6c  ecialized intell
+00000e20: 6967 656e 6365 2c20 616c 6c6f 7769 6e67  igence, allowing
+00000e30: 206f 7468 6572 7320 746f 2072 6570 726f   others to repro
+00000e40: 6475 6365 2c20 6275 696c 6420 6f6e 2c20  duce, build on, 
+00000e50: 6f72 2069 6e74 6572 6163 7420 7769 7468  or interact with
+00000e60: 2069 743f 20f0 9fa4 9720 5468 6973 2062   it? .... This b
+00000e70: 656c 6965 6620 696e 7370 6972 6573 2075  elief inspires u
+00000e80: 7320 746f 2062 7569 6c64 2047 656e 746f  s to build Gento
+00000e90: 7069 612c 200a 2a2a 6465 7369 676e 6564  pia, .**designed
+00000ea0: 2066 6f72 2061 6765 6e74 202a 7370 6563   for agent *spec
+00000eb0: 6961 6c69 7a61 7469 6f6e 2c20 7368 6172  ialization, shar
+00000ec0: 696e 672c 2061 6e64 2069 6e74 6572 6163  ing, and interac
+00000ed0: 7469 6f6e 2c2a 2074 6f20 7374 6163 6b69  tion,* to stacki
+00000ee0: 6e67 6c79 2061 6368 6965 7665 2063 6f6c  ngly achieve col
+00000ef0: 6c65 6374 6976 6520 6772 6f77 7468 2074  lective growth t
+00000f00: 6f77 6172 6473 2067 7265 6174 6572 2069  owards greater i
+00000f10: 6e74 656c 6c69 6765 6e63 652e 2a2a 2e0a  ntelligence.**..
+00000f20: 0a23 2320 436f 7265 2046 6561 7475 7265  .## Core Feature
+00000f30: 7320 f09f 92a1 0a0a 2d20 e29a 99ef b88f  s ......- ......
+00000f40: 2043 6f6e 6669 672d 6472 6976 656e 2061   Config-driven a
+00000f50: 6765 6e74 2061 7373 656d 626c 696e 6720  gent assembling 
+00000f60: 616e 6420 6368 6174 2e0a 2d20 f09f 9a80  and chat..- ....
+00000f70: 204c 6172 6765 2061 6d6f 756e 7420 6f66   Large amount of
+00000f80: 2070 7265 6275 696c 7420 6167 656e 7420   prebuilt agent 
+00000f90: 7479 7065 732c 204c 4c4d 2063 6c69 656e  types, LLM clien
+00000fa0: 7473 2c20 746f 6f6c 732c 206d 656d 6f72  ts, tools, memor
+00000fb0: 7920 7379 7374 656d 732c 2061 6e64 206d  y systems, and m
+00000fc0: 6f72 652e 0a2d 20f0 9faa b620 4c69 6768  ore..- .... Ligh
+00000fd0: 7477 6569 6768 7420 616e 6420 6869 6768  tweight and high
+00000fe0: 6c79 2065 7874 656e 7369 626c 6520 696d  ly extensible im
+00000ff0: 706c 656d 656e 7461 7469 6f6e 206f 6620  plementation of 
+00001000: 6573 7365 6e74 6961 6c20 636f 6d70 6f6e  essential compon
+00001010: 656e 7473 2e0a 2d20 f09f a7aa 2041 6c69  ents..- .... Ali
+00001020: 676e 696e 6720 7769 7468 2073 7461 7465  gning with state
+00001030: 2d6f 662d 7468 652d 6172 7420 4149 2072  -of-the-art AI r
+00001040: 6573 6561 7263 682e 0a2d 20f0 9fa4 9d20  esearch..- .... 
+00001050: 456e 6162 6c69 6e67 206d 756c 7469 2d61  Enabling multi-a
+00001060: 6765 6e74 2069 6e74 6572 6163 7469 6f6e  gent interaction
+00001070: 732e 0a2d 20f0 9fa6 8120 556e 6971 7565  s..- .... Unique
+00001080: 2070 6c61 7466 6f72 6d20 6f66 2061 6765   platform of age
+00001090: 6e74 207a 6f6f 2061 6e64 2065 7661 6c20  nt zoo and eval 
+000010a0: 6265 6e63 686d 6172 6b2e 0a0a 2323 2051  benchmark...## Q
+000010b0: 7569 636b 2053 7461 7274 20f0 9f8d 8f0a  uick Start .....
+000010c0: 6060 600a 636f 6e64 6120 6372 6561 7465  ```.conda create
+000010d0: 202d 2d6e 616d 6520 6765 6e74 656e 7620   --name gentenv 
+000010e0: 7079 7468 6f6e 3d33 2e31 300a 636f 6e64  python=3.10.cond
+000010f0: 6120 6163 7469 7661 7465 2067 656e 7465  a activate gente
+00001100: 6e76 0a70 6970 2069 6e73 7461 6c6c 2067  nv.pip install g
+00001110: 656e 746f 7069 610a 6060 600a 6f72 2069  entopia.```.or i
+00001120: 6620 796f 7520 7761 6e74 2074 6f20 6275  f you want to bu
+00001130: 696c 6420 7769 7468 206f 7065 6e20 4c4c  ild with open LL
+00001140: 4d73 206c 6f63 616c 6c79 20f0 9f91 8920  Ms locally .... 
+00001150: 6070 6970 2069 6e73 7461 6c6c 2067 656e  `pip install gen
+00001160: 746f 7069 615b 6875 6767 696e 6766 6163  topia[huggingfac
+00001170: 655d 600a 0a46 6972 7374 2074 696d 6520  e]`..First time 
+00001180: 746f 2047 656e 746f 7069 613f 2047 7261  to Gentopia? Gra
+00001190: 6220 6120 636f 6666 6565 20e2 9895 2061  b a coffee ... a
+000011a0: 6e64 200a 0a54 616b 6520 7e20 3820 6d69  nd ..Take ~ 8 mi
+000011b0: 6e73 2074 6f20 6368 6563 6b20 6f75 7420  ns to check out 
+000011c0: 7468 6520 666f 6c6c 6f77 696e 6720 6465  the following de
+000011d0: 6d6f 2074 7574 6f72 6961 6c73 205b 215b  mo tutorials [![
+000011e0: 596f 7554 7562 6520 4368 616e 6e65 6c20  YouTube Channel 
+000011f0: 5375 6273 6372 6962 6572 735d 2868 7474  Subscribers](htt
+00001200: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00001210: 2e69 6f2f 796f 7574 7562 652f 6368 616e  .io/youtube/chan
+00001220: 6e65 6c2f 7669 6577 732f 5543 3951 436a  nel/views/UC9QCj
+00001230: 6373 484a 564b 6a4b 5a32 5a6d 7271 3833  csHJVKjKZ2Zmrq83
+00001240: 7641 295d 2868 7474 7073 3a2f 2f77 7777  vA)](https://www
+00001250: 2e79 6f75 7475 6265 2e63 6f6d 2f63 6861  .youtube.com/cha
+00001260: 6e6e 656c 2f55 4339 5143 6a63 7348 4a56  nnel/UC9QCjcsHJV
+00001270: 4b6a 4b5a 325a 6d72 7138 3376 4129 200a  KjKZ2Zmrq83vA) .
+00001280: 0a3c 6469 7620 7374 796c 653d 2264 6973  .<div style="dis
+00001290: 706c 6179 3a20 666c 6578 3b20 6a75 7374  play: flex; just
+000012a0: 6966 792d 636f 6e74 656e 743a 2073 7061  ify-content: spa
+000012b0: 6365 2d61 726f 756e 643b 223e 0a20 200a  ce-around;">.  .
+000012c0: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+000012d0: 2f77 7777 2e79 6f75 7475 6265 2e63 6f6d  /www.youtube.com
+000012e0: 2f77 6174 6368 3f76 3d37 645a 335a 7673  /watch?v=7dZ3Zvs
+000012f0: 4937 7377 2220 7461 7267 6574 3d22 5f62  I7sw" target="_b
+00001300: 6c61 6e6b 223e 0a20 203c 696d 6720 7372  lank">.  <img sr
+00001310: 633d 2268 7474 7073 3a2f 2f69 6d67 2e79  c="https://img.y
+00001320: 6f75 7475 6265 2e63 6f6d 2f76 692f 3764  outube.com/vi/7d
+00001330: 5a33 5a76 7349 3773 772f 6871 6465 6661  Z3ZvsI7sw/hqdefa
+00001340: 756c 742e 6a70 6722 2061 6c74 3d22 5669  ult.jpg" alt="Vi
+00001350: 6465 6f20 3122 2073 7479 6c65 3d22 7769  deo 1" style="wi
+00001360: 6474 683a 3332 253b 223e 0a3c 2f61 3e0a  dth:32%;">.</a>.
+00001370: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+00001380: 2f2f 7777 772e 796f 7574 7562 652e 636f  //www.youtube.co
+00001390: 6d2f 7761 7463 683f 763d 5854 7376 3970  m/watch?v=XTsv9p
+000013a0: 6b36 414f 4122 2074 6172 6765 743d 225f  k6AOA" target="_
+000013b0: 626c 616e 6b22 3e0a 2020 3c69 6d67 2073  blank">.  <img s
+000013c0: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+000013d0: 796f 7574 7562 652e 636f 6d2f 7669 2f58  youtube.com/vi/X
+000013e0: 5473 7639 706b 3641 4f41 2f68 7164 6566  Tsv9pk6AOA/hqdef
+000013f0: 6175 6c74 2e6a 7067 2220 616c 743d 2256  ault.jpg" alt="V
+00001400: 6964 656f 2032 2220 7374 796c 653d 2277  ideo 2" style="w
+00001410: 6964 7468 3a33 3225 3b22 3e0a 3c2f 613e  idth:32%;">.</a>
+00001420: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
+00001430: 3a2f 2f77 7777 2e79 6f75 7475 6265 2e63  ://www.youtube.c
+00001440: 6f6d 2f77 6174 6368 3f76 3d64 694a 3449  om/watch?v=diJ4I
+00001450: 4461 5434 5a34 2220 7461 7267 6574 3d22  DaT4Z4" target="
+00001460: 5f62 6c61 6e6b 223e 0a20 203c 696d 6720  _blank">.  <img 
+00001470: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
+00001480: 2e79 6f75 7475 6265 2e63 6f6d 2f76 692f  .youtube.com/vi/
+00001490: 6469 4a34 4944 6154 345a 342f 6871 6465  diJ4IDaT4Z4/hqde
+000014a0: 6661 756c 742e 6a70 6722 2061 6c74 3d22  fault.jpg" alt="
+000014b0: 5669 6465 6f20 3322 2073 7479 6c65 3d22  Video 3" style="
+000014c0: 7769 6474 683a 3332 253b 223e 0a3c 2f61  width:32%;">.</a
+000014d0: 3e0a 0a3c 2f64 6976 3e0a 0a4f 7220 6368  >..</div>..Or ch
+000014e0: 6563 6b20 6f75 7420 7468 6520 5b51 7569  eck out the [Qui
+000014f0: 636b 2053 7461 7274 5d28 6874 7470 733a  ck Start](https:
+00001500: 2f2f 6765 6e74 6f70 6961 2e72 6561 6474  //gentopia.readt
+00001510: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00001520: 6573 742f 7175 6963 6b5f 7374 6172 742e  est/quick_start.
+00001530: 6874 6d6c 2920 446f 632e 0a0a 2323 2044  html) Doc...## D
+00001540: 6f63 756d 656e 7461 7469 6f6e 20f0 9f93  ocumentation ...
+00001550: 960a 5365 6520 5b68 6572 655d 2868 7474  ..See [here](htt
+00001560: 7073 3a2f 2f67 656e 746f 7069 612e 7265  ps://gentopia.re
+00001570: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
+00001580: 6c61 7465 7374 2f69 6e64 6578 2e68 746d  latest/index.htm
+00001590: 6c29 2066 6f72 2066 756c 6c20 646f 6375  l) for full docu
+000015a0: 6d65 6e74 6174 696f 6e2e 0a0a f09f 8c9f  mentation.......
+000015b0: 2048 6967 686c 6967 6874 2054 6f70 6963   Highlight Topic
+000015c0: 7320 f09f 8c9f 200a 2d20 5bf0 9fa4 9620  s .... .- [.... 
+000015d0: 4167 656e 7420 5465 6d70 6c61 7465 735d  Agent Templates]
+000015e0: 2868 7474 7073 3a2f 2f67 656e 746f 7069  (https://gentopi
+000015f0: 612e 7265 6164 7468 6564 6f63 732e 696f  a.readthedocs.io
+00001600: 2f65 6e2f 6c61 7465 7374 2f71 7569 636b  /en/latest/quick
+00001610: 5f73 7461 7274 2e68 746d 6c23 7661 6e69  _start.html#vani
+00001620: 6c6c 612d 6167 656e 7429 0a2d 205b e29b  lla-agent).- [..
+00001630: b0ef b88f 2048 6965 7261 7263 6869 6361  .... Hierarchica
+00001640: 6c20 4167 656e 7473 5d28 6874 7470 733a  l Agents](https:
+00001650: 2f2f 6765 6e74 6f70 6961 2e72 6561 6474  //gentopia.readt
+00001660: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00001670: 6573 742f 6167 656e 745f 636f 6d70 6f6e  est/agent_compon
+00001680: 656e 7473 2e68 746d 6c23 6167 656e 742d  ents.html#agent-
+00001690: 6173 2d70 6c75 6769 6e29 0a2d 205b f09f  as-plugin).- [..
+000016a0: a587 2055 6e69 7175 6520 4167 656e 7420  .. Unique Agent 
+000016b0: 4265 6e63 686d 6172 6b5d 2868 7474 7073  Benchmark](https
+000016c0: 3a2f 2f67 656e 746f 7069 612e 7265 6164  ://gentopia.read
+000016d0: 7468 6564 6f63 732e 696f 2f65 6e2f 6c61  thedocs.io/en/la
+000016e0: 7465 7374 2f67 656e 7470 6f6f 6c2e 6874  test/gentpool.ht
+000016f0: 6d6c 2361 6765 6e74 2d65 7661 6c75 6174  ml#agent-evaluat
+00001700: 696f 6e29 0a2d 205b f09f a699 204f 7065  ion).- [.... Ope
+00001710: 6e20 4c4c 4d20 5375 7070 6f72 7473 5d28  n LLM Supports](
+00001720: 6874 7470 733a 2f2f 6765 6e74 6f70 6961  https://gentopia
+00001730: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+00001740: 656e 2f6c 6174 6573 742f 6167 656e 745f  en/latest/agent_
+00001750: 636f 6d70 6f6e 656e 7473 2e68 746d 6c23  components.html#
+00001760: 6875 6767 696e 6766 6163 652d 6f70 656e  huggingface-open
+00001770: 2d6c 6c6d 7329 0a2d 205b f09f a7a0 2048  -llms).- [.... H
+00001780: 6967 682d 5065 7266 6f72 6d61 6e63 6520  igh-Performance 
+00001790: 4d65 6d6f 7279 5d28 6874 7470 733a 2f2f  Memory](https://
+000017a0: 6765 6e74 6f70 6961 2e72 6561 6474 6865  gentopia.readthe
+000017b0: 646f 6373 2e69 6f2f 656e 2f6c 6174 6573  docs.io/en/lates
+000017c0: 742f 6167 656e 745f 636f 6d70 6f6e 656e  t/agent_componen
+000017d0: 7473 2e68 746d 6c23 6c6f 6e67 2d73 686f  ts.html#long-sho
+000017e0: 7274 2d74 6572 6d2d 6d65 6d6f 7279 290a  rt-term-memory).
+000017f0: 0a23 2320 4a6f 696e 2075 7321 20f0 9f8c  .## Join us! ...
+00001800: 8e0a 0a50 6172 7469 6369 7061 7465 2069  ...Participate i
+00001810: 6e20 7468 6973 2055 746f 7069 6120 6f66  n this Utopia of
+00001820: 2073 7570 6572 696e 7465 6c6c 6967 656e   superintelligen
+00001830: 6365 2061 6e64 2068 656c 7020 6974 2067  ce and help it g
+00001840: 726f 7773 2120 4173 2061 2066 756c 6c79  rows! As a fully
+00001850: 206f 7065 6e2d 736f 7572 6365 2070 726f   open-source pro
+00001860: 6a65 6374 2c20 7765 2064 6576 656c 6f70  ject, we develop
+00001870: 2075 6e64 6572 2070 7562 6c69 6320 6164   under public ad
+00001880: 7669 6365 2c20 6964 6561 732c 2061 6e64  vice, ideas, and
+00001890: 2073 7570 6572 7669 7369 6f6e 2e20 4d65   supervision. Me
+000018a0: 616e 7768 696c 652c 2068 6572 6520 6172  anwhile, here ar
+000018b0: 6520 7761 7973 2079 6f75 206d 6179 2063  e ways you may c
+000018c0: 6f6e 7472 6962 7574 6520 746f 2047 656e  ontribute to Gen
+000018d0: 746f 7069 612e 0a0a 2d20 f09f 909b 2050  topia...- .... P
+000018e0: 6f73 7420 616e 205b 6973 7375 655d 2868  ost an [issue](h
+000018f0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00001900: 6d2f 4765 6e74 6f70 6961 2d41 492f 4765  m/Gentopia-AI/Ge
+00001910: 6e74 6f70 6961 2f69 7373 7565 7329 2072  ntopia/issues) r
+00001920: 6571 7565 7374 696e 6720 6e65 6365 7373  equesting necess
+00001930: 6172 7920 6275 6720 6669 7865 732c 2061  ary bug fixes, a
+00001940: 6464 6974 696f 6e61 6c20 6665 6174 7572  dditional featur
+00001950: 6573 2c20 6f72 2072 6f61 646d 6170 2073  es, or roadmap s
+00001960: 7567 6765 7374 696f 6e73 2e20 2843 6865  uggestions. (Che
+00001970: 636b 2063 6c6f 7365 6420 6f6e 6573 2066  ck closed ones f
+00001980: 6972 7374 290a 2d20 f09f 8eaf 204f 7572  irst).- .... Our
+00001990: 2064 6576 2074 6561 6d20 6d65 6574 7320   dev team meets 
+000019a0: 7765 656b 6c79 2074 6f20 6772 6f6f 6d20  weekly to groom 
+000019b0: 5b62 6163 6b6c 6f67 5d28 6874 7470 733a  [backlog](https:
+000019c0: 2f2f 6769 7468 7562 2e63 6f6d 2f6f 7267  //github.com/org
+000019d0: 732f 4765 6e74 6f70 6961 2d41 492f 7072  s/Gentopia-AI/pr
+000019e0: 6f6a 6563 7473 2f31 2920 696e 746f 2074  ojects/1) into t
+000019f0: 6963 6b65 7473 2e20 5768 696c 6520 7765  ickets. While we
+00001a00: 2077 6f72 6b20 6f6e 2074 6865 6d2c 2079   work on them, y
+00001a10: 6f75 2063 616e 2070 6963 6b20 7570 206f  ou can pick up o
+00001a20: 7468 6572 7320 616e 6420 6372 6561 7465  thers and create
+00001a30: 2061 205b 5075 6c6c 2052 6571 7565 7374   a [Pull Request
+00001a40: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001a50: 2e63 6f6d 2f47 656e 746f 7069 612d 4149  .com/Gentopia-AI
+00001a60: 2f47 656e 746f 7069 612f 7075 6c6c 7329  /Gentopia/pulls)
+00001a70: 2074 6f20 7265 7175 6573 7420 6120 6d65   to request a me
+00001a80: 7267 652e 2057 6520 616c 7761 7973 2077  rge. We always w
+00001a90: 656c 636f 6d65 206e 6577 206d 656d 6265  elcome new membe
+00001aa0: 7273 2069 6e20 7468 6973 2077 6179 2e0a  rs in this way..
+00001ab0: 2d20 f09f a49d 2053 6861 7265 2079 6f75  - .... Share you
+00001ac0: 7220 7370 6563 6961 6c69 7a65 6420 6167  r specialized ag
+00001ad0: 656e 7420 746f 205b 4765 6e74 506f 6f6c  ent to [GentPool
+00001ae0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+00001af0: 2e63 6f6d 2f47 656e 746f 7069 612d 4149  .com/Gentopia-AI
+00001b00: 2f47 656e 7450 6f6f 6c29 2120 4372 6561  /GentPool)! Crea
+00001b10: 7465 2061 6e20 4167 656e 7420 5052 2028  te an Agent PR (
+00001b20: 5b65 7861 6d70 6c65 5d28 2929 2074 6f20  [example]()) to 
+00001b30: 6d65 7267 6520 796f 7572 2077 656c 6c2d  merge your well-
+00001b40: 7475 6e65 6420 6167 656e 7420 696e 746f  tuned agent into
+00001b50: 2074 6865 2070 6f6f 6c2e 2054 6869 7320   the pool. This 
+00001b60: 616c 6c6f 7773 206f 7468 6572 7320 746f  allows others to
+00001b70: 2075 7365 206f 7220 6275 696c 6420 7570   use or build up
+00001b80: 6f6e 2079 6f75 7220 6167 656e 742e 200a  on your agent. .
+00001b90: 2d20 e2ad 9020 4865 6c70 2075 7320 7370  - ... Help us sp
+00001ba0: 7265 6164 2120 4769 7665 2075 7320 6120  read! Give us a 
+00001bb0: 7374 6172 2c20 666f 6c6c 6f77 2075 7320  star, follow us 
+00001bc0: 6f6e 205b 5477 6974 7465 725d 2868 7474  on [Twitter](htt
+00001bd0: 7073 3a2f 2f74 7769 7474 6572 2e63 6f6d  ps://twitter.com
+00001be0: 2f47 656e 746f 7069 6141 4929 2c20 6a6f  /GentopiaAI), jo
+00001bf0: 696e 206f 7572 205b 4469 7363 6f72 645d  in our [Discord]
+00001c00: 2868 7474 7073 3a2f 2f64 6973 636f 7264  (https://discord
+00001c10: 2e67 672f 4153 5050 394d 5939 514b 292c  .gg/ASPP9MY9QK),
+00001c20: 2061 6e64 2073 6861 7265 2077 6974 6820   and share with 
+00001c30: 796f 7572 2066 7269 656e 6473 2120 200a  your friends!  .
+00001c40: 0a0a                                     ..
```

### Comparing `gentopia-0.0.1/gentopia/__init__.py` & `gentopia-0.0.2/gentopia/__init__.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/agent/base_agent.py` & `gentopia-0.0.2/gentopia/agent/base_agent.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/agent/openai/agent.py` & `gentopia-0.0.2/gentopia/agent/openai/agent.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/agent/openai_memory/agent.py` & `gentopia-0.0.2/gentopia/agent/openai_memory/agent.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/agent/openai_memory/load_memory.py` & `gentopia-0.0.2/gentopia/agent/openai_memory/load_memory.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/agent/plugin_manager.py` & `gentopia-0.0.2/gentopia/agent/plugin_manager.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/agent/react/agent.py` & `gentopia-0.0.2/gentopia/agent/react/agent.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/agent/rewoo/agent.py` & `gentopia-0.0.2/gentopia/agent/rewoo/agent.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/agent/rewoo/nodes/Planner.py` & `gentopia-0.0.2/gentopia/agent/rewoo/nodes/Planner.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/agent/rewoo/nodes/Solver.py` & `gentopia-0.0.2/gentopia/agent/rewoo/nodes/Solver.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/agent/vanilla/agent.py` & `gentopia-0.0.2/gentopia/agent/vanilla/agent.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/assembler/agent_assembler.py` & `gentopia-0.0.2/gentopia/assembler/agent_assembler.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/assembler/config.py` & `gentopia-0.0.2/gentopia/assembler/config.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/assembler/loader.py` & `gentopia-0.0.2/gentopia/assembler/loader.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/assembler/task.py` & `gentopia-0.0.2/gentopia/assembler/task.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/base_llm.py` & `gentopia-0.0.2/gentopia/llm/base_llm.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/client/huggingface.py` & `gentopia-0.0.2/gentopia/llm/client/huggingface.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/client/openai.py` & `gentopia-0.0.2/gentopia/llm/client/openai.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/llm_info.py` & `gentopia-0.0.2/gentopia/llm/llm_info.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/loaders/airoboros.py` & `gentopia-0.0.2/gentopia/llm/loaders/airoboros.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/loaders/alpaca.py` & `gentopia-0.0.2/gentopia/llm/loaders/alpaca.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/loaders/baize.py` & `gentopia-0.0.2/gentopia/llm/loaders/baize.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/loaders/bloom.py` & `gentopia-0.0.2/gentopia/llm/loaders/bloom.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/loaders/camel.py` & `gentopia-0.0.2/gentopia/llm/loaders/camel.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/loaders/falcon.py` & `gentopia-0.0.2/gentopia/llm/loaders/falcon.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/loaders/flan_alpaca.py` & `gentopia-0.0.2/gentopia/llm/loaders/flan_alpaca.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/loaders/guanaco.py` & `gentopia-0.0.2/gentopia/llm/loaders/guanaco.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/loaders/mpt.py` & `gentopia-0.0.2/gentopia/llm/loaders/mpt.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/loaders/redpajama.py` & `gentopia-0.0.2/gentopia/llm/loaders/redpajama.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/loaders/replit.py` & `gentopia-0.0.2/gentopia/llm/loaders/replit.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/loaders/samantha_vicuna.py` & `gentopia-0.0.2/gentopia/llm/loaders/samantha_vicuna.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/loaders/stablelm.py` & `gentopia-0.0.2/gentopia/llm/loaders/stablelm.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/loaders/t5_vicuna.py` & `gentopia-0.0.2/gentopia/llm/loaders/t5_vicuna.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/loaders/vicuna.py` & `gentopia-0.0.2/gentopia/llm/loaders/vicuna.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/test_llm.py` & `gentopia-0.0.2/gentopia/llm/test_llm.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/llm/wrap_llm.py` & `gentopia-0.0.2/gentopia/llm/wrap_llm.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/manager/base_llm_manager.py` & `gentopia-0.0.2/gentopia/manager/base_llm_manager.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/manager/llm_client/base_llm_client.py` & `gentopia-0.0.2/gentopia/manager/llm_client/base_llm_client.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/manager/llm_client/local_llm_client.py` & `gentopia-0.0.2/gentopia/manager/llm_client/local_llm_client.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/manager/local_llm_manager.py` & `gentopia-0.0.2/gentopia/manager/local_llm_manager.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/memory/api.py` & `gentopia-0.0.2/gentopia/memory/api.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/memory/base_memory.py` & `gentopia-0.0.2/gentopia/memory/base_memory.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/memory/embeddings.py` & `gentopia-0.0.2/gentopia/memory/embeddings.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/memory/serializable.py` & `gentopia-0.0.2/gentopia/memory/serializable.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/memory/utils.py` & `gentopia-0.0.2/gentopia/memory/utils.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/memory/vectorstores/chroma.py` & `gentopia-0.0.2/gentopia/memory/vectorstores/chroma.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/memory/vectorstores/pinecone.py` & `gentopia-0.0.2/gentopia/memory/vectorstores/pinecone.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/memory/vectorstores/vectorstore.py` & `gentopia-0.0.2/gentopia/memory/vectorstores/vectorstore.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/model/agent_model.py` & `gentopia-0.0.2/gentopia/model/agent_model.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/model/completion_model.py` & `gentopia-0.0.2/gentopia/model/completion_model.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/model/param_model.py` & `gentopia-0.0.2/gentopia/model/param_model.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/output/__init__.py` & `gentopia-0.0.2/gentopia/output/__init__.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/output/base_output.py` & `gentopia-0.0.2/gentopia/output/base_output.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/output/console_output.py` & `gentopia-0.0.2/gentopia/output/console_output.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/output/print_output.py` & `gentopia-0.0.2/gentopia/output/print_output.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/prompt/prompt_template.py` & `gentopia-0.0.2/gentopia/prompt/prompt_template.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/prompt/react.py` & `gentopia-0.0.2/gentopia/prompt/react.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/prompt/rewoo.py` & `gentopia-0.0.2/gentopia/prompt/rewoo.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/__init__.py` & `gentopia-0.0.2/gentopia/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/arxiv_search.py` & `gentopia-0.0.2/gentopia/tools/arxiv_search.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/basetool.py` & `gentopia-0.0.2/gentopia/tools/basetool.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/bing_search.py` & `gentopia-0.0.2/gentopia/tools/bing_search.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/calculator.py` & `gentopia-0.0.2/gentopia/tools/calculator.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/code_interpreter.py` & `gentopia-0.0.2/gentopia/tools/code_interpreter.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/file_operation.py` & `gentopia-0.0.2/gentopia/tools/file_operation.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/google_search.py` & `gentopia-0.0.2/gentopia/tools/google_search.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/gradio.py` & `gentopia-0.0.2/gentopia/tools/gradio.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/gradio_tools/api.py` & `gentopia-0.0.2/gentopia/tools/gradio_tools/api.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/gradio_tools/tools/__init__.py` & `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/gradio_tools/tools/bark.py` & `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/bark.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/gradio_tools/tools/clip_interrogator.py` & `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/clip_interrogator.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/gradio_tools/tools/document_qa.py` & `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/document_qa.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/gradio_tools/tools/gradio_tool.py` & `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/gradio_tool.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/gradio_tools/tools/image_captioning.py` & `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/image_captioning.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/gradio_tools/tools/image_to_music.py` & `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/image_to_music.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/gradio_tools/tools/prompt_generator.py` & `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/prompt_generator.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/gradio_tools/tools/sam_with_clip.py` & `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/sam_with_clip.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/gradio_tools/tools/stable_diffusion.py` & `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/stable_diffusion.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/gradio_tools/tools/text_to_video.py` & `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/text_to_video.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/gradio_tools/tools/whisper.py` & `gentopia-0.0.2/gentopia/tools/gradio_tools/tools/whisper.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/search_doc.py` & `gentopia-0.0.2/gentopia/tools/search_doc.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/shell.py` & `gentopia-0.0.2/gentopia/tools/shell.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/utils/docstore.py` & `gentopia-0.0.2/gentopia/tools/utils/docstore.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/utils/document_loaders/base_loader.py` & `gentopia-0.0.2/gentopia/tools/utils/document_loaders/base_loader.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/utils/document_loaders/text_loader.py` & `gentopia-0.0.2/gentopia/tools/utils/document_loaders/text_loader.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/utils/document_loaders/text_splitter.py` & `gentopia-0.0.2/gentopia/tools/utils/document_loaders/text_splitter.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/utils/vector_store.py` & `gentopia-0.0.2/gentopia/tools/utils/vector_store.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/weather.py` & `gentopia-0.0.2/gentopia/tools/weather.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/web_page.py` & `gentopia-0.0.2/gentopia/tools/web_page.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/wikipedia.py` & `gentopia-0.0.2/gentopia/tools/wikipedia.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/tools/wolfram_alpha.py` & `gentopia-0.0.2/gentopia/tools/wolfram_alpha.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/utils/cost_helpers.py` & `gentopia-0.0.2/gentopia/utils/cost_helpers.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/utils/text_helpers.py` & `gentopia-0.0.2/gentopia/utils/text_helpers.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia/utils/util.py` & `gentopia-0.0.2/gentopia/utils/util.py`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/gentopia.egg-info/PKG-INFO` & `gentopia-0.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,357 +1,431 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310a 4e61 6d65 3a20 6765 6e74  : 2.1.Name: gent
-00000020: 6f70 6961 0a56 6572 7369 6f6e 3a20 302e  opia.Version: 0.
-00000030: 302e 310a 5375 6d6d 6172 793a 2047 656e  0.1.Summary: Gen
-00000040: 746f 7069 6120 7072 6f76 6964 6573 2065  topia provides e
-00000050: 7874 656e 7369 7665 2075 7469 6c69 7469  xtensive utiliti
-00000060: 6573 2074 6f20 6173 7365 6d62 6c65 7320  es to assembles 
-00000070: 414c 4d20 6167 656e 7473 2064 7269 7665  ALM agents drive
-00000080: 6e20 6279 2063 6f6e 6669 6773 2e0a 486f  n by configs..Ho
-00000090: 6d65 2d70 6167 653a 2068 7474 7073 3a2f  me-page: https:/
-000000a0: 2f67 6974 6875 622e 636f 6d2f 4765 6e74  /github.com/Gent
-000000b0: 6f70 6961 2d41 492f 4765 6e74 6f70 6961  opia-AI/Gentopia
-000000c0: 0a41 7574 686f 723a 2062 696c 6c78 6266  .Author: billxbf
-000000d0: 0a41 7574 686f 722d 656d 6169 6c3a 2062  .Author-email: b
-000000e0: 696c 6c78 6266 4067 6d61 696c 2e63 6f6d  illxbf@gmail.com
-000000f0: 0a4c 6963 656e 7365 3a20 4170 6163 6865  .License: Apache
-00000100: 2d32 2e30 206c 6963 656e 7365 0a44 6573  -2.0 license.Des
-00000110: 6372 6970 7469 6f6e 2d43 6f6e 7465 6e74  cription-Content
-00000120: 2d54 7970 653a 2074 6578 742f 6d61 726b  -Type: text/mark
-00000130: 646f 776e 0a50 726f 7669 6465 732d 4578  down.Provides-Ex
-00000140: 7472 613a 2068 7567 6769 6e67 6661 6365  tra: huggingface
-00000150: 0a4c 6963 656e 7365 2d46 696c 653a 204c  .License-File: L
-00000160: 4943 454e 5345 0a0a 2320 4765 6e74 6f70  ICENSE..# Gentop
-00000170: 6961 200a 2a54 6865 2043 6f6c 6c65 6374  ia .*The Collect
-00000180: 6976 6520 4772 6f77 7468 206f 6620 496e  ive Growth of In
-00000190: 7465 6c6c 6967 656e 7420 4167 656e 7473  telligent Agents
-000001a0: 2e2a 20f0 9fa6 99f0 9f8c 8e0a 0a47 656e  .* ..........Gen
-000001b0: 746f 7069 6120 6973 2061 206c 6967 6874  topia is a light
-000001c0: 7765 6967 6874 2061 6e64 2065 7874 656e  weight and exten
-000001d0: 7369 626c 6520 6672 616d 6577 6f72 6b20  sible framework 
-000001e0: 666f 7220 4c4c 4d2d 6472 6976 656e 2041  for LLM-driven A
-000001f0: 6765 6e74 7320 616e 6420 5b41 4c4d 5d28  gents and [ALM](
-00000200: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00000210: 672f 6162 732f 3233 3032 2e30 3738 3432  g/abs/2302.07842
-00000220: 2920 2072 6573 6561 7263 682e 2049 7420  )  research. It 
-00000230: 7072 6f76 6964 6573 206d 756c 7469 706c  provides multipl
-00000240: 6520 6573 7365 6e74 6961 6c20 636f 6d70  e essential comp
-00000250: 6f6e 656e 7473 2074 6f20 6275 696c 642c  onents to build,
-00000260: 2074 6573 7420 616e 6420 6576 616c 7561   test and evalua
-00000270: 7465 2061 6765 6e74 732e 2041 7420 6974  te agents. At it
-00000280: 7320 636f 7265 2c20 4765 6e74 6f70 6961  s core, Gentopia
-00000290: 2061 696d 7320 746f 2065 6d62 6f64 7920   aims to embody 
-000002a0: 6167 656e 7473 2077 6974 6820 7369 6e67  agents with sing
-000002b0: 6c65 2063 6f6e 6669 6720 6669 6c65 732c  le config files,
-000002c0: 2074 6875 7320 6d69 6e69 6d69 7a69 6e67   thus minimizing
-000002d0: 2079 6f75 7220 6566 666f 7274 2069 6e20   your effort in 
-000002e0: 6d61 696e 7461 696e 696e 672c 2074 756e  maintaining, tun
-000002f0: 696e 672c 2061 6e64 2073 6861 7269 6e67  ing, and sharing
-00000300: 2061 6765 6e74 732e 0a0a 4765 6e74 6f70   agents...Gentop
-00000310: 6961 206d 6169 6e74 6169 6e73 2061 6e20  ia maintains an 
-00000320: 6167 656e 7420 7a6f 6f20 5b47 656e 7450  agent zoo [GentP
-00000330: 6f6f 6c5d 2868 7474 7073 3a2f 2f67 6974  ool](https://git
-00000340: 6875 622e 636f 6d2f 4765 6e74 6f70 6961  hub.com/Gentopia
-00000350: 2d41 492f 4765 6e74 506f 6f6c 2920 746f  -AI/GentPool) to
-00000360: 2073 6861 7265 2070 7562 6c69 6320 6167   share public ag
-00000370: 656e 7473 2073 7065 6369 616c 697a 6564  ents specialized
-00000380: 2066 6f72 2064 6966 6665 7265 6e74 2074   for different t
-00000390: 6173 6b73 2e20 496e 2074 6869 7320 706c  asks. In this pl
-000003a0: 6174 666f 726d 2c20 796f 7520 636f 756c  atform, you coul
-000003b0: 6420 6561 7369 6c79 202a 696e 7465 7261  d easily *intera
-000003c0: 6374 2a20 7769 7468 206f 7468 6572 2061  ct* with other a
-000003d0: 6765 6e74 7320 6279 2063 6c6f 6e69 6e67  gents by cloning
-000003e0: 2c20 6869 6572 6172 6368 6963 616c 2070  , hierarchical p
-000003f0: 6c75 672d 696e 2c20 6f72 2073 6861 7269  lug-in, or shari
-00000400: 6e67 2065 6e76 6972 6f6e 6d65 6e74 2e20  ng environment. 
-00000410: 5765 2061 6c73 6f20 6275 696c 6420 6120  We also build a 
-00000420: 756e 6971 7565 2061 6765 6e74 205b 6265  unique agent [be
-00000430: 6e63 686d 6172 6b5d 2868 7474 7073 3a2f  nchmark](https:/
-00000440: 2f67 656e 746f 7069 612e 7265 6164 7468  /gentopia.readth
-00000450: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
-00000460: 7374 2f67 656e 7470 6f6f 6c2e 6874 6d6c  st/gentpool.html
-00000470: 2361 6765 6e74 2d65 7661 6c75 6174 696f  #agent-evaluatio
-00000480: 6e29 2066 6f72 2068 6f6c 6973 7469 6320  n) for holistic 
-00000490: 414c 4d20 6576 616c 7561 7469 6f6e 2e20  ALM evaluation. 
-000004a0: 0a0a 2323 204d 6f74 6976 6174 696f 6e20  ..## Motivation 
-000004b0: f09f a7a0 0a41 6765 6e74 2070 7261 6374  .....Agent pract
-000004c0: 6974 696f 6e65 7273 2073 7461 7274 2074  itioners start t
-000004d0: 6f20 7265 616c 697a 6520 7468 6520 6469  o realize the di
-000004e0: 6666 6963 756c 7479 2069 6e20 7475 6e69  fficulty in tuni
-000004f0: 6e67 2061 2022 7765 6c6c 2d72 6f75 6e64  ng a "well-round
-00000500: 6564 2220 6167 656e 7420 7769 7468 2074  ed" agent with t
-00000510: 6f6e 7320 6f66 2074 6f6f 6c73 206f 7220  ons of tools or 
-00000520: 696e 7374 7275 6374 696f 6e73 2069 6e20  instructions in 
-00000530: 7369 6e67 6c65 206c 6179 6572 2e0a 5265  single layer..Re
-00000540: 6365 6e74 2073 7475 6469 6573 206c 696b  cent studies lik
-00000550: 6520 5b54 696e 7953 746f 7269 6573 5d28  e [TinyStories](
-00000560: 6874 7470 733a 2f2f 6172 7869 762e 6f72  https://arxiv.or
-00000570: 672f 6162 732f 3233 3031 2e31 3237 3236  g/abs/2301.12726
-00000580: 292c 205b 5370 6563 6961 6c69 7a69 6e67  ), [Specializing
-00000590: 2052 6561 736f 6e69 6e67 5d28 6874 7470   Reasoning](http
-000005a0: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
-000005b0: 732f 3233 3031 2e31 3237 3236 292c 205b  s/2301.12726), [
-000005c0: 4c65 7427 7320 5665 7269 6679 2053 6253  Let's Verify SbS
-000005d0: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
-000005e0: 6f72 672f 6162 732f 3233 3035 2e32 3030  org/abs/2305.200
-000005f0: 3530 292c 205b 5265 574f 4f5d 2868 7474  50), [ReWOO](htt
-00000600: 7073 3a2f 2f61 7278 6976 2e6f 7267 2f61  ps://arxiv.org/a
-00000610: 6273 2f32 3330 352e 3138 3332 3329 2c20  bs/2305.18323), 
-00000620: 6574 632e 2061 6c73 6f20 706f 696e 7420  etc. also point 
-00000630: 7573 2074 6f77 6172 6473 2061 6e20 696e  us towards an in
-00000640: 7475 6974 6976 6520 7965 7420 756e 6465  tuitive yet unde
-00000650: 7276 616c 7565 6420 6469 7265 6374 696f  rvalued directio
-00000660: 6e20 f09f 9189 200a 0a60 6060 0a41 6e20  n .... ..```.An 
-00000670: 4c4c 4d20 6973 206d 6f72 6520 6361 7061  LLM is more capa
-00000680: 626c 6520 6966 2079 6f75 2063 7265 6174  ble if you creat
-00000690: 6520 6120 636f 6e74 6578 742f 6469 7374  e a context/dist
-000006a0: 7269 6275 7469 6f6e 2073 6869 6674 2073  ribution shift s
-000006b0: 7065 6369 616c 697a 6564 2074 6f20 736f  pecialized to so
-000006c0: 6d65 2074 6172 6765 7420 7461 736b 732e  me target tasks.
-000006d0: 0a60 6060 0a53 6164 6c79 2c20 7468 6572  .```.Sadly, ther
-000006e0: 6520 6973 206e 6f20 7369 6c76 6572 2062  e is no silver b
-000006f0: 756c 6c65 7420 666f 7220 6167 656e 7420  ullet for agent 
-00000700: 7370 6563 6961 6c69 7a61 7469 6f6e 2e20  specialization. 
-00000710: 466f 7220 6578 616d 706c 652c 2079 6f75  For example, you
-00000720: 2063 616e 200a 2d20 5369 6d70 6c79 2061   can .- Simply a
-00000730: 6464 2060 4c65 7427 7320 7468 696e 6b20  dd `Let's think 
-00000740: 7374 6570 2062 7920 7374 6570 2e60 2069  step by step.` i
-00000750: 6e20 796f 7572 202a 2a70 726f 6d70 742a  n your **prompt*
-00000760: 2a20 666f 7220 6d6f 7265 2061 6363 7572  * for more accur
-00000770: 6174 6520 4d61 7468 2051 412e 0a2d 2047  ate Math QA..- G
-00000780: 6976 6520 6120 2a2a 6665 772d 7368 6f74  ive a **few-shot
-00000790: 2a2a 2065 7865 6d70 6c61 7220 696e 2079  ** exemplar in y
-000007a0: 6f75 7220 7072 6f6d 7074 2074 6f20 6775  our prompt to gu
-000007b0: 6964 6520 6120 6265 7474 6572 2072 6561  ide a better rea
-000007c0: 736f 6e69 6e67 2074 7261 6a65 6374 6f72  soning trajector
-000007d0: 7920 666f 7220 6e6f 7665 6c20 706c 6f74  y for novel plot
-000007e0: 7469 6e67 2e0a 2d20 5375 7065 7276 6973  ting..- Supervis
-000007f0: 6520 2a2a 6669 6e65 2d74 756e 696e 672a  e **fine-tuning*
-00000800: 2a20 2853 4654 2920 796f 7572 2037 3042  * (SFT) your 70B
-00000810: 2060 6c6c 616d 6132 6020 6c69 6b65 205b   `llama2` like [
-00000820: 7468 6973 5d28 6874 7470 733a 2f2f 6172  this](https://ar
-00000830: 7869 762e 6f72 672f 6162 732f 3233 3035  xiv.org/abs/2305
-00000840: 2e32 3030 3530 2920 746f 206d 6174 6368  .20050) to match
-00000850: 2072 6561 736f 6e69 6e67 206f 6620 3137   reasoning of 17
-00000860: 3542 2047 5054 2d33 2e35 2e0a 2d20 5475  5B GPT-3.5..- Tu
-00000870: 6e65 2079 6f75 7220 6167 656e 7420 2a2a  ne your agent **
-00000880: 7061 7261 6469 676d 2a2a 206c 696b 6520  paradigm** like 
-00000890: 7468 6973 205b 6465 6d6f 5d28 6874 7470  this [demo](http
-000008a0: 733a 2f2f 7777 772e 796f 7574 7562 652e  s://www.youtube.
-000008b0: 636f 6d2f 7761 7463 683f 763d 6469 4a34  com/watch?v=diJ4
-000008c0: 4944 6154 345a 3429 2074 6f20 6561 7369  IDaT4Z4) to easi
-000008d0: 6c79 2068 616c 6620 7468 6520 6578 6563  ly half the exec
-000008e0: 7574 696f 6e20 7469 6d65 2066 6f72 2053  ution time for S
-000008f0: 6561 6368 2026 2053 756d 6d61 7269 7a65  each & Summarize
-00000900: 2e0a 2d20 416e 6420 6d6f 7265 202e 2e2e  ..- And more ...
-00000910: 0a0a 4973 6e27 7420 6974 2062 6561 7574  ..Isn't it beaut
-00000920: 6966 756c 2069 6620 6f6e 6520 7368 6172  iful if one shar
-00000930: 6573 2068 6973 2073 7065 6369 616c 697a  es his specializ
-00000940: 6564 2069 6e74 656c 6c69 6765 6e63 652c  ed intelligence,
-00000950: 2061 6c6c 6f77 696e 6720 6f74 6865 7273   allowing others
-00000960: 2074 6f20 7265 7072 6f64 7563 652c 2062   to reproduce, b
-00000970: 7569 6c64 206f 6e2c 206f 7220 696e 7465  uild on, or inte
-00000980: 7261 6374 2077 6974 6820 6974 2061 7420  ract with it at 
-00000990: 6561 7365 3f20 f09f a497 2054 6869 7320  ease? .... This 
-000009a0: 6265 6c69 6566 2069 6e73 7069 7265 7320  belief inspires 
-000009b0: 7573 2074 6f20 6275 696c 6420 4765 6e74  us to build Gent
-000009c0: 6f70 6961 2c20 0a2a 2a64 6573 6967 6e65  opia, .**designe
-000009d0: 6420 666f 7220 6167 656e 7420 2a73 7065  d for agent *spe
-000009e0: 6369 616c 697a 6174 696f 6e2c 2073 6861  cialization, sha
-000009f0: 7269 6e67 2c20 616e 6420 696e 7465 7261  ring, and intera
-00000a00: 6374 696f 6e2c 2a20 746f 2061 6368 6965  ction,* to achie
-00000a10: 7665 2063 6f6c 6c65 6374 6976 6520 6772  ve collective gr
-00000a20: 6f77 7468 2074 6f77 6172 6473 2067 7265  owth towards gre
-00000a30: 6174 6572 2069 6e74 656c 6c69 6765 6e63  ater intelligenc
-00000a40: 652a 2a2e 0a0a 2323 2043 6f72 6520 4665  e**...## Core Fe
-00000a50: 6174 7572 6573 20f0 9f92 a10a 0a2d 20e2  atures ......- .
-00000a60: 9a99 efb8 8f20 436f 6e66 6967 2d64 7269  ..... Config-dri
-00000a70: 7665 6e20 6167 656e 7420 6173 7365 6d62  ven agent assemb
-00000a80: 6c69 6e67 2061 6e64 2063 6861 742e 0a2d  ling and chat..-
-00000a90: 20f0 9f9a 8020 4c61 7267 6520 616d 6f75   .... Large amou
-00000aa0: 6e74 206f 6620 7072 6562 7569 6c74 2061  nt of prebuilt a
-00000ab0: 6765 6e74 2074 7970 6573 2c20 4c4c 4d20  gent types, LLM 
-00000ac0: 636c 6965 6e74 732c 2074 6f6f 6c73 2c20  clients, tools, 
-00000ad0: 6d65 6d6f 7279 2073 7973 7465 6d73 2c20  memory systems, 
-00000ae0: 616e 6420 6d6f 7265 2e0a 2d20 f09f aab6  and more..- ....
-00000af0: 204c 6967 6874 7765 6967 6874 2061 6e64   Lightweight and
-00000b00: 2068 6967 686c 7920 6578 7465 6e73 6962   highly extensib
-00000b10: 6c65 2069 6d70 6c65 6d65 6e74 6174 696f  le implementatio
-00000b20: 6e20 6f66 2065 7373 656e 7469 616c 2063  n of essential c
-00000b30: 6f6d 706f 6e65 6e74 732e 0a2d 20f0 9fa7  omponents..- ...
-00000b40: aa20 416c 6967 6e69 6e67 2077 6974 6820  . Aligning with 
-00000b50: 7374 6174 652d 6f66 2d74 6865 2d61 7274  state-of-the-art
-00000b60: 2041 4920 7265 7365 6172 6368 2e0a 2d20   AI research..- 
-00000b70: f09f a49d 2045 6e61 626c 696e 6720 6d75  .... Enabling mu
-00000b80: 6c74 692d 6167 656e 7420 696e 7465 7261  lti-agent intera
-00000b90: 6374 696f 6e73 2e0a 2d20 f09f a681 2055  ctions..- .... U
-00000ba0: 6e69 7175 6520 706c 6174 666f 726d 206f  nique platform o
-00000bb0: 6620 6167 656e 7420 7a6f 6f20 616e 6420  f agent zoo and 
-00000bc0: 6576 616c 2062 656e 6368 6d61 726b 2e0a  eval benchmark..
-00000bd0: 0a23 2320 5175 6963 6b20 5374 6172 7420  .## Quick Start 
-00000be0: f09f 9bab 0a60 6060 0a70 6970 2069 6e73  .....```.pip ins
-00000bf0: 7461 6c6c 2067 656e 746f 7069 610a 6060  tall gentopia.``
-00000c00: 600a 6f72 2069 6620 796f 7520 7761 6e74  `.or if you want
-00000c10: 2074 6f20 6275 696c 6420 7769 7468 206f   to build with o
-00000c20: 7065 6e20 4c4c 4d73 206c 6f63 616c 6c79  pen LLMs locally
-00000c30: 20f0 9f91 8920 6070 6970 2069 6e73 7461   .... `pip insta
-00000c40: 6c6c 2067 656e 746f 7069 615b 6875 6767  ll gentopia[hugg
-00000c50: 696e 6766 6163 655d 600a 0a46 6972 7374  ingface]`..First
-00000c60: 2074 696d 6520 746f 2047 656e 746f 7069   time to Gentopi
-00000c70: 613f 2047 7261 6220 6120 636f 6666 6565  a? Grab a coffee
-00000c80: 20e2 9895 2061 6e64 2074 616b 6520 7e20   ... and take ~ 
-00000c90: 3130 206d 696e 7320 746f 2063 6865 636b  10 mins to check
-00000ca0: 206f 7574 2074 6865 2066 6f6c 6c6f 7769   out the followi
-00000cb0: 6e67 206d 696e 642d 626c 6f77 696e 6720  ng mind-blowing 
-00000cc0: 6465 6d6f 7320 f09f 9180 20f0 9fa4 af0a  demos .... .....
-00000cd0: 0a3c 6469 7620 7374 796c 653d 2264 6973  .<div style="dis
-00000ce0: 706c 6179 3a20 666c 6578 3b20 6a75 7374  play: flex; just
-00000cf0: 6966 792d 636f 6e74 656e 743a 2073 7061  ify-content: spa
-00000d00: 6365 2d61 726f 756e 643b 223e 0a20 200a  ce-around;">.  .
-00000d10: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
-00000d20: 2f77 7777 2e79 6f75 7475 6265 2e63 6f6d  /www.youtube.com
-00000d30: 2f77 6174 6368 3f76 3d37 645a 335a 7673  /watch?v=7dZ3Zvs
-00000d40: 4937 7377 2220 7461 7267 6574 3d22 5f62  I7sw" target="_b
-00000d50: 6c61 6e6b 223e 0a20 203c 696d 6720 7372  lank">.  <img sr
-00000d60: 633d 2268 7474 7073 3a2f 2f69 6d67 2e79  c="https://img.y
-00000d70: 6f75 7475 6265 2e63 6f6d 2f76 692f 3764  outube.com/vi/7d
-00000d80: 5a33 5a76 7349 3773 772f 6871 6465 6661  Z3ZvsI7sw/hqdefa
-00000d90: 756c 742e 6a70 6722 2061 6c74 3d22 5669  ult.jpg" alt="Vi
-00000da0: 6465 6f20 3122 2073 7479 6c65 3d22 7769  deo 1" style="wi
-00000db0: 6474 683a 3332 253b 223e 0a3c 2f61 3e0a  dth:32%;">.</a>.
-00000dc0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
-00000dd0: 2f2f 7777 772e 796f 7574 7562 652e 636f  //www.youtube.co
-00000de0: 6d2f 7761 7463 683f 763d 5854 7376 3970  m/watch?v=XTsv9p
-00000df0: 6b36 414f 4122 2074 6172 6765 743d 225f  k6AOA" target="_
-00000e00: 626c 616e 6b22 3e0a 2020 3c69 6d67 2073  blank">.  <img s
-00000e10: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
-00000e20: 796f 7574 7562 652e 636f 6d2f 7669 2f58  youtube.com/vi/X
-00000e30: 5473 7639 706b 3641 4f41 2f68 7164 6566  Tsv9pk6AOA/hqdef
-00000e40: 6175 6c74 2e6a 7067 2220 616c 743d 2256  ault.jpg" alt="V
-00000e50: 6964 656f 2032 2220 7374 796c 653d 2277  ideo 2" style="w
-00000e60: 6964 7468 3a33 3225 3b22 3e0a 3c2f 613e  idth:32%;">.</a>
-00000e70: 0a0a 3c61 2068 7265 663d 2268 7474 7073  ..<a href="https
-00000e80: 3a2f 2f77 7777 2e79 6f75 7475 6265 2e63  ://www.youtube.c
-00000e90: 6f6d 2f77 6174 6368 3f76 3d64 694a 3449  om/watch?v=diJ4I
-00000ea0: 4461 5434 5a34 2220 7461 7267 6574 3d22  DaT4Z4" target="
-00000eb0: 5f62 6c61 6e6b 223e 0a20 203c 696d 6720  _blank">.  <img 
-00000ec0: 7372 633d 2268 7474 7073 3a2f 2f69 6d67  src="https://img
-00000ed0: 2e79 6f75 7475 6265 2e63 6f6d 2f76 692f  .youtube.com/vi/
-00000ee0: 6469 4a34 4944 6154 345a 342f 6871 6465  diJ4IDaT4Z4/hqde
-00000ef0: 6661 756c 742e 6a70 6722 2061 6c74 3d22  fault.jpg" alt="
-00000f00: 5669 6465 6f20 3322 2073 7479 6c65 3d22  Video 3" style="
-00000f10: 7769 6474 683a 3332 253b 223e 0a3c 2f61  width:32%;">.</a
-00000f20: 3e0a 0a3c 2f64 6976 3e0a 0a28 4a75 6d70  >..</div>..(Jump
-00000f30: 2074 6f20 7468 6520 7468 6972 6420 6f6e   to the third on
-00000f40: 6520 6966 2079 6f75 206f 6e6c 7920 6861  e if you only ha
-00000f50: 7665 2033 206d 696e 7320 f09f a4ab 290a  ve 3 mins ....).
-00000f60: 0a23 2320 446f 6375 6d65 6e74 6174 696f  .## Documentatio
-00000f70: 6e20 f09f 9396 0a53 6565 205b 6865 7265  n .....See [here
-00000f80: 5d28 6874 7470 733a 2f2f 6765 6e74 6f70  ](https://gentop
-00000f90: 6961 2e72 6561 6474 6865 646f 6373 2e69  ia.readthedocs.i
-00000fa0: 6f2f 656e 2f6c 6174 6573 742f 696e 6465  o/en/latest/inde
-00000fb0: 782e 6874 6d6c 2920 666f 7220 6675 6c6c  x.html) for full
-00000fc0: 2064 6f63 756d 656e 7461 7469 6f6e 2e0a   documentation..
-00000fd0: 0af0 9f8c 9f20 4869 6768 6c69 6768 7420  ..... Highlight 
-00000fe0: 546f 7069 6373 200a 2d20 5b41 6765 6e74  Topics .- [Agent
-00000ff0: 2054 656d 706c 6174 6573 5d28 6874 7470   Templates](http
-00001000: 733a 2f2f 6765 6e74 6f70 6961 2e72 6561  s://gentopia.rea
-00001010: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
-00001020: 6174 6573 742f 7175 6963 6b5f 7374 6172  atest/quick_star
-00001030: 742e 6874 6d6c 2376 616e 696c 6c61 2d61  t.html#vanilla-a
-00001040: 6765 6e74 290a 2d20 5b48 6965 7261 7263  gent).- [Hierarc
-00001050: 6869 6361 6c20 4167 656e 7473 5d28 6874  hical Agents](ht
-00001060: 7470 733a 2f2f 6765 6e74 6f70 6961 2e72  tps://gentopia.r
-00001070: 6561 6474 6865 646f 6373 2e69 6f2f 656e  eadthedocs.io/en
-00001080: 2f6c 6174 6573 742f 6167 656e 745f 636f  /latest/agent_co
-00001090: 6d70 6f6e 656e 7473 2e68 746d 6c23 6167  mponents.html#ag
-000010a0: 656e 742d 6173 2d70 6c75 6769 6e29 0a2d  ent-as-plugin).-
-000010b0: 205b 556e 6971 7565 2041 6765 6e74 2042   [Unique Agent B
-000010c0: 656e 6368 6d61 726b 5d28 6874 7470 733a  enchmark](https:
-000010d0: 2f2f 6765 6e74 6f70 6961 2e72 6561 6474  //gentopia.readt
-000010e0: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-000010f0: 6573 742f 6765 6e74 706f 6f6c 2e68 746d  est/gentpool.htm
-00001100: 6c23 6167 656e 742d 6576 616c 7561 7469  l#agent-evaluati
-00001110: 6f6e 290a 2d20 5b4f 7065 6e20 4c4c 4d20  on).- [Open LLM 
-00001120: 5375 7070 6f72 7473 5d28 6874 7470 733a  Supports](https:
-00001130: 2f2f 6765 6e74 6f70 6961 2e72 6561 6474  //gentopia.readt
-00001140: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
-00001150: 6573 742f 6167 656e 745f 636f 6d70 6f6e  est/agent_compon
-00001160: 656e 7473 2e68 746d 6c23 6875 6767 696e  ents.html#huggin
-00001170: 6766 6163 652d 6f70 656e 2d6c 6c6d 7329  gface-open-llms)
-00001180: 0a2d 205b 4869 6768 2d50 6572 666f 726d  .- [High-Perform
-00001190: 616e 6365 204d 656d 6f72 795d 2868 7474  ance Memory](htt
-000011a0: 7073 3a2f 2f67 656e 746f 7069 612e 7265  ps://gentopia.re
-000011b0: 6164 7468 6564 6f63 732e 696f 2f65 6e2f  adthedocs.io/en/
-000011c0: 6c61 7465 7374 2f61 6765 6e74 5f63 6f6d  latest/agent_com
-000011d0: 706f 6e65 6e74 732e 6874 6d6c 236c 6f6e  ponents.html#lon
-000011e0: 672d 7368 6f72 742d 7465 726d 2d6d 656d  g-short-term-mem
-000011f0: 6f72 7929 0a0a 2323 2042 7569 6c64 2077  ory)..## Build w
-00001200: 6974 6820 7573 20f0 9f8c 8e0a 0a50 6172  ith us ......Par
-00001210: 7469 6369 7061 7465 2069 6e20 7468 6973  ticipate in this
-00001220: 2055 746f 7069 6120 6f66 2073 7570 6572   Utopia of super
-00001230: 696e 7465 6c6c 6967 656e 6365 2061 6e64  intelligence and
-00001240: 2068 656c 7020 6974 2067 726f 7773 2120   help it grows! 
-00001250: 4173 2061 2066 756c 6c79 206f 7065 6e2d  As a fully open-
-00001260: 736f 7572 6365 2070 726f 6a65 6374 2c20  source project, 
-00001270: 7765 2064 6576 656c 6f70 2075 6e64 6572  we develop under
-00001280: 2070 7562 6c69 6320 6164 7669 6365 2c20   public advice, 
-00001290: 6964 6561 732c 2061 6e64 2073 7570 6572  ideas, and super
-000012a0: 7669 7369 6f6e 2e20 4d65 616e 7768 696c  vision. Meanwhil
-000012b0: 652c 2068 6572 6520 6172 6520 7761 7973  e, here are ways
-000012c0: 2079 6f75 206d 6179 2063 6f6e 7472 6962   you may contrib
-000012d0: 7574 6520 746f 2047 656e 746f 7069 612e  ute to Gentopia.
-000012e0: 0a0a 2d20 f09f 909b 2050 6f73 7420 616e  ..- .... Post an
-000012f0: 205b 6973 7375 655d 2868 7474 7073 3a2f   [issue](https:/
-00001300: 2f67 6974 6875 622e 636f 6d2f 4765 6e74  /github.com/Gent
-00001310: 6f70 6961 2d41 492f 4765 6e74 6f70 6961  opia-AI/Gentopia
-00001320: 2f69 7373 7565 7329 2072 6571 7565 7374  /issues) request
-00001330: 696e 6720 6e65 6365 7373 6172 7920 6275  ing necessary bu
-00001340: 6720 6669 7865 732c 2061 6464 6974 696f  g fixes, additio
-00001350: 6e61 6c20 6665 6174 7572 6573 2c20 6f72  nal features, or
-00001360: 2072 6f61 646d 6170 2073 7567 6765 7374   roadmap suggest
-00001370: 696f 6e73 2e20 2843 6865 636b 2063 6c6f  ions. (Check clo
-00001380: 7365 6420 6f6e 6573 2066 6972 7374 290a  sed ones first).
-00001390: 2d20 f09f 8eaf 204f 7572 2064 6576 2074  - .... Our dev t
-000013a0: 6561 6d20 6d65 6574 7320 7765 656b 6c79  eam meets weekly
-000013b0: 2074 6f20 6772 6f6f 6d20 5b62 6163 6b6c   to groom [backl
-000013c0: 6f67 5d28 6874 7470 733a 2f2f 6769 7468  og](https://gith
-000013d0: 7562 2e63 6f6d 2f6f 7267 732f 4765 6e74  ub.com/orgs/Gent
-000013e0: 6f70 6961 2d41 492f 7072 6f6a 6563 7473  opia-AI/projects
-000013f0: 2f31 2920 696e 746f 2074 6963 6b65 7473  /1) into tickets
-00001400: 2e20 5768 696c 6520 7765 2077 6f72 6b20  . While we work 
-00001410: 6f6e 2074 6865 6d2c 2079 6f75 2063 616e  on them, you can
-00001420: 2070 6963 6b20 7570 206f 7468 6572 7320   pick up others 
-00001430: 616e 6420 6372 6561 7465 2061 205b 5075  and create a [Pu
-00001440: 6c6c 2052 6571 7565 7374 5d28 6874 7470  ll Request](http
-00001450: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f47  s://github.com/G
-00001460: 656e 746f 7069 612d 4149 2f47 656e 746f  entopia-AI/Gento
-00001470: 7069 612f 7075 6c6c 7329 2074 6f20 7265  pia/pulls) to re
-00001480: 7175 6573 7420 6120 6d65 7267 652e 2057  quest a merge. W
-00001490: 6520 616c 7761 7973 2077 656c 636f 6d65  e always welcome
-000014a0: 206e 6577 206d 656d 6265 7273 2069 6e20   new members in 
-000014b0: 7468 6973 2077 6179 2e0a 2d20 f09f a49d  this way..- ....
-000014c0: 2053 6861 7265 2079 6f75 7220 7370 6563   Share your spec
-000014d0: 6961 6c69 7a65 6420 6167 656e 7420 746f  ialized agent to
-000014e0: 205b 4765 6e74 506f 6f6c 5d28 6874 7470   [GentPool](http
-000014f0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f47  s://github.com/G
-00001500: 656e 746f 7069 612d 4149 2f47 656e 7450  entopia-AI/GentP
-00001510: 6f6f 6c29 2120 4372 6561 7465 2061 6e20  ool)! Create an 
-00001520: 4167 656e 7420 5052 2028 5b65 7861 6d70  Agent PR ([examp
-00001530: 6c65 5d28 2929 2074 6f20 6d65 7267 6520  le]()) to merge 
-00001540: 796f 7572 2077 656c 6c2d 7475 6e65 6420  your well-tuned 
-00001550: 6167 656e 7420 696e 746f 2074 6865 2070  agent into the p
-00001560: 6f6f 6c2e 2054 6869 7320 616c 6c6f 7773  ool. This allows
-00001570: 206f 7468 6572 7320 746f 2075 7365 206f   others to use o
-00001580: 7220 6275 696c 6420 7570 6f6e 2079 6f75  r build upon you
-00001590: 7220 6167 656e 742e 200a 2d20 e2ad 9020  r agent. .- ... 
-000015a0: 4865 6c70 2075 7320 7370 7265 6164 2120  Help us spread! 
-000015b0: 4769 7665 2075 7320 6120 7374 6172 2c20  Give us a star, 
-000015c0: 666f 6c6c 6f77 2075 7320 6f6e 205b 5477  follow us on [Tw
-000015d0: 6974 7465 725d 2868 7474 7073 3a2f 2f74  itter](https://t
-000015e0: 7769 7474 6572 2e63 6f6d 2f47 656e 746f  witter.com/Gento
-000015f0: 7069 6141 4929 2c20 6a6f 696e 206f 7572  piaAI), join our
-00001600: 205b 4469 7363 6f72 645d 2868 7474 7073   [Discord](https
-00001610: 3a2f 2f64 6973 636f 7264 2e67 672f 4153  ://discord.gg/AS
-00001620: 5050 394d 5939 514b 292c 2061 6e64 2073  PP9MY9QK), and s
-00001630: 6861 7265 2077 6974 6820 796f 7572 2066  hare with your f
-00001640: 7269 656e 6473 2120 200a 0a0a            riends!  ...
+00000000: 2320 4765 6e74 6f70 6961 200a f09f 8c8e  # Gentopia .....
+00000010: 202a 436f 6c6c 6563 7469 7665 2047 726f   *Collective Gro
+00000020: 7774 6820 6f66 2049 6e74 656c 6c69 6765  wth of Intellige
+00000030: 6e74 2041 6765 6e74 732e 2a20 f09f a699  nt Agents.* ....
+00000040: 0a0a 0a5b 215b 4c69 6365 6e73 653a 204d  ...[![License: M
+00000050: 4954 5d28 6874 7470 733a 2f2f 696d 672e  IT](https://img.
+00000060: 7368 6965 6c64 732e 696f 2f62 6164 6765  shields.io/badge
+00000070: 2f4c 6963 656e 7365 2d4d 4954 2d79 656c  /License-MIT-yel
+00000080: 6c6f 772e 7376 6729 5d28 6874 7470 733a  low.svg)](https:
+00000090: 2f2f 6f70 656e 736f 7572 6365 2e6f 7267  //opensource.org
+000000a0: 2f6c 6963 656e 7365 732f 4d49 5429 0a21  /licenses/MIT).!
+000000b0: 5b53 7461 7469 6320 4261 6467 655d 2868  [Static Badge](h
+000000c0: 7474 7073 3a2f 2f69 6d67 2e73 6869 656c  ttps://img.shiel
+000000d0: 6473 2e69 6f2f 6261 6467 652f 7265 6c65  ds.io/badge/rele
+000000e0: 6173 652d 6265 7461 2d62 6c75 6529 0a5b  ase-beta-blue).[
+000000f0: 215b 5374 6174 6963 2042 6164 6765 5d28  ![Static Badge](
+00000100: 6874 7470 733a 2f2f 696d 672e 7368 6965  https://img.shie
+00000110: 6c64 732e 696f 2f62 6164 6765 2f44 6f63  lds.io/badge/Doc
+00000120: 756d 656e 7461 7469 6f6e 2d38 4132 4245  umentation-8A2BE
+00000130: 3229 5d28 6874 7470 733a 2f2f 6765 6e74  2)](https://gent
+00000140: 6f70 6961 2e72 6561 6474 6865 646f 6373  opia.readthedocs
+00000150: 2e69 6f2f 656e 2f6c 6174 6573 742f 696e  .io/en/latest/in
+00000160: 6465 782e 6874 6d6c 290a 5b21 5b53 7461  dex.html).[![Sta
+00000170: 7469 6320 4261 6467 655d 2868 7474 7073  tic Badge](https
+00000180: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000190: 6f2f 6261 6467 652f 4765 6e74 506f 6f6c  o/badge/GentPool
+000001a0: 2d62 6c75 6529 5d28 6874 7470 733a 2f2f  -blue)](https://
+000001b0: 6769 7468 7562 2e63 6f6d 2f47 656e 746f  github.com/Gento
+000001c0: 7069 612d 4149 2f47 656e 7450 6f6f 6c29  pia-AI/GentPool)
+000001d0: 0a5b 215b 5374 6174 6963 2042 6164 6765  .[![Static Badge
+000001e0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+000001f0: 6965 6c64 732e 696f 2f62 6164 6765 2f62  ields.io/badge/b
+00000200: 6163 6b6c 6f67 2d67 7265 7929 5d28 6874  acklog-grey)](ht
+00000210: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00000220: 2f6f 7267 732f 4765 6e74 6f70 6961 2d41  /orgs/Gentopia-A
+00000230: 492f 7072 6f6a 6563 7473 2f31 290a 5b21  I/projects/1).[!
+00000240: 5b4f 7065 6e20 4973 7375 6573 5d28 6874  [Open Issues](ht
+00000250: 7470 733a 2f2f 696d 672e 7368 6965 6c64  tps://img.shield
+00000260: 732e 696f 2f67 6974 6875 622f 6973 7375  s.io/github/issu
+00000270: 6573 2d72 6177 2f47 656e 746f 7069 612d  es-raw/Gentopia-
+00000280: 4149 2f47 656e 746f 7069 6129 5d28 6874  AI/Gentopia)](ht
+00000290: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000002a0: 2f47 656e 746f 7069 612d 4149 2f47 656e  /Gentopia-AI/Gen
+000002b0: 746f 7069 612f 6973 7375 6573 290a 5b21  topia/issues).[!
+000002c0: 5b44 6570 656e 6465 6e63 7920 5374 6174  [Dependency Stat
+000002d0: 7573 5d28 6874 7470 733a 2f2f 696d 672e  us](https://img.
+000002e0: 7368 6965 6c64 732e 696f 2f6c 6962 7261  shields.io/libra
+000002f0: 7269 6573 696f 2f67 6974 6875 622f 4765  riesio/github/Ge
+00000300: 6e74 6f70 6961 2d41 492f 4765 6e74 6f70  ntopia-AI/Gentop
+00000310: 6961 295d 2868 7474 7073 3a2f 2f6c 6962  ia)](https://lib
+00000320: 7261 7269 6573 2e69 6f2f 6769 7468 7562  raries.io/github
+00000330: 2f47 656e 746f 7069 612d 4149 2f47 656e  /Gentopia-AI/Gen
+00000340: 746f 7069 6129 0a0a 5b21 5b54 7769 7474  topia)..[![Twitt
+00000350: 6572 2046 6f6c 6c6f 775d 2868 7474 7073  er Follow](https
+00000360: 3a2f 2f69 6d67 2e73 6869 656c 6473 2e69  ://img.shields.i
+00000370: 6f2f 7477 6974 7465 722f 666f 6c6c 6f77  o/twitter/follow
+00000380: 2f47 656e 746f 7069 6141 4929 5d28 6874  /GentopiaAI)](ht
+00000390: 7470 733a 2f2f 7477 6974 7465 722e 636f  tps://twitter.co
+000003a0: 6d2f 4765 6e74 6f70 6961 4149 290a 5b21  m/GentopiaAI).[!
+000003b0: 5b5d 2868 7474 7073 3a2f 2f64 6362 6164  [](https://dcbad
+000003c0: 6765 2e76 6572 6365 6c2e 6170 702f 6170  ge.vercel.app/ap
+000003d0: 692f 7365 7276 6572 2f41 5350 5039 4d59  i/server/ASPP9MY
+000003e0: 3951 4b3f 636f 6d70 6163 743d 7472 7565  9QK?compact=true
+000003f0: 2673 7479 6c65 3d66 6c61 7429 5d28 6874  &style=flat)](ht
+00000400: 7470 733a 2f2f 6469 7363 6f72 642e 6767  tps://discord.gg
+00000410: 2f41 5350 5039 4d59 3951 4b29 0a5b 215b  /ASPP9MY9QK).[![
+00000420: 596f 7554 7562 6520 4368 616e 6e65 6c20  YouTube Channel 
+00000430: 5375 6273 6372 6962 6572 735d 2868 7474  Subscribers](htt
+00000440: 7073 3a2f 2f69 6d67 2e73 6869 656c 6473  ps://img.shields
+00000450: 2e69 6f2f 796f 7574 7562 652f 6368 616e  .io/youtube/chan
+00000460: 6e65 6c2f 7669 6577 732f 5543 3951 436a  nel/views/UC9QCj
+00000470: 6373 484a 564b 6a4b 5a32 5a6d 7271 3833  csHJVKjKZ2Zmrq83
+00000480: 7641 295d 2868 7474 7073 3a2f 2f77 7777  vA)](https://www
+00000490: 2e79 6f75 7475 6265 2e63 6f6d 2f63 6861  .youtube.com/cha
+000004a0: 6e6e 656c 2f55 4339 5143 6a63 7348 4a56  nnel/UC9QCjcsHJV
+000004b0: 4b6a 4b5a 325a 6d72 7138 3376 4129 0a5b  KjKZ2Zmrq83vA).[
+000004c0: 215b 4769 7448 7562 2073 7461 7220 6368  ![GitHub star ch
+000004d0: 6172 745d 2868 7474 7073 3a2f 2f69 6d67  art](https://img
+000004e0: 2e73 6869 656c 6473 2e69 6f2f 6769 7468  .shields.io/gith
+000004f0: 7562 2f73 7461 7273 2f47 656e 746f 7069  ub/stars/Gentopi
+00000500: 612d 4149 2f47 656e 746f 7069 613f 7374  a-AI/Gentopia?st
+00000510: 796c 653d 736f 6369 616c 295d 2868 7474  yle=social)](htt
+00000520: 7073 3a2f 2f73 7461 722d 6869 7374 6f72  ps://star-histor
+00000530: 792e 636f 6d2f 4765 6e74 6f70 6961 2d41  y.com/Gentopia-A
+00000540: 492f 4765 6e74 6f70 6961 290a 0a0a 0a0a  I/Gentopia).....
+00000550: 4765 6e74 6f70 6961 2069 7320 6120 6c69  Gentopia is a li
+00000560: 6768 7477 6569 6768 7420 616e 6420 6578  ghtweight and ex
+00000570: 7465 6e73 6962 6c65 2066 7261 6d65 776f  tensible framewo
+00000580: 726b 2066 6f72 204c 4c4d 2d64 7269 7665  rk for LLM-drive
+00000590: 6e20 4167 656e 7473 2061 6e64 205b 414c  n Agents and [AL
+000005a0: 4d5d 2868 7474 7073 3a2f 2f61 7278 6976  M](https://arxiv
+000005b0: 2e6f 7267 2f61 6273 2f32 3330 322e 3037  .org/abs/2302.07
+000005c0: 3834 3229 2020 7265 7365 6172 6368 2e20  842)  research. 
+000005d0: 4974 2070 726f 7669 6465 7320 6573 7365  It provides esse
+000005e0: 6e74 6961 6c20 636f 6d70 6f6e 656e 7473  ntial components
+000005f0: 2074 6f20 6275 696c 642c 2074 6573 7420   to build, test 
+00000600: 616e 6420 6576 616c 7561 7465 2061 6765  and evaluate age
+00000610: 6e74 732e 2041 7420 6974 7320 636f 7265  nts. At its core
+00000620: 2c20 4765 6e74 6f70 6961 2061 696d 7320  , Gentopia aims 
+00000630: 746f 2061 7373 656d 626c 6520 616e 2061  to assemble an a
+00000640: 6765 6e74 2077 6974 6820 6120 7369 6e67  gent with a sing
+00000650: 6c65 2063 6f6e 6669 672c 2074 6875 7320  le config, thus 
+00000660: 6d69 6e69 6d69 7a69 6e67 2079 6f75 7220  minimizing your 
+00000670: 6566 666f 7274 2069 6e20 6275 696c 6469  effort in buildi
+00000680: 6e67 2c20 7475 6e69 6e67 2c20 616e 6420  ng, tuning, and 
+00000690: 7368 6172 696e 6720 6167 656e 7473 2e20  sharing agents. 
+000006a0: 0a0a 4765 6e74 6f70 6961 206d 6169 6e74  ..Gentopia maint
+000006b0: 6169 6e73 2061 6e20 6167 656e 7420 706c  ains an agent pl
+000006c0: 6174 666f 726d 205b 4765 6e74 506f 6f6c  atform [GentPool
+000006d0: 5d28 6874 7470 733a 2f2f 6769 7468 7562  ](https://github
+000006e0: 2e63 6f6d 2f47 656e 746f 7069 612d 4149  .com/Gentopia-AI
+000006f0: 2f47 656e 7450 6f6f 6c29 2074 6f20 7368  /GentPool) to sh
+00000700: 6172 6520 7370 6563 6961 6c69 7a65 6420  are specialized 
+00000710: 6167 656e 7473 2c20 7768 6572 6520 796f  agents, where yo
+00000720: 7572 2061 6765 6e74 202a 696e 7465 7261  ur agent *intera
+00000730: 6374 732a 2077 6974 6820 6f74 6865 7220  cts* with other 
+00000740: 6167 656e 7473 2062 7920 636c 6f6e 696e  agents by clonin
+00000750: 672c 2068 6965 7261 7263 6869 6361 6c20  g, hierarchical 
+00000760: 706c 7567 2d69 6e2c 206f 7220 7368 6172  plug-in, or shar
+00000770: 696e 6720 656e 7669 726f 6e6d 656e 742e  ing environment.
+00000780: 2057 6520 7072 6f76 6964 6520 6120 756e   We provide a un
+00000790: 6971 7565 2061 6765 6e74 205b 6265 6e63  ique agent [benc
+000007a0: 686d 6172 6b5d 2868 7474 7073 3a2f 2f67  hmark](https://g
+000007b0: 656e 746f 7069 612e 7265 6164 7468 6564  entopia.readthed
+000007c0: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+000007d0: 2f67 656e 7470 6f6f 6c2e 6874 6d6c 2361  /gentpool.html#a
+000007e0: 6765 6e74 2d65 7661 6c75 6174 696f 6e29  gent-evaluation)
+000007f0: 2066 6f72 2068 6f6c 6973 7469 6320 6576   for holistic ev
+00000800: 616c 7561 7469 6f6e 2e20 0a0a 2323 204d  aluation. ..## M
+00000810: 6f74 6976 6174 696f 6e20 f09f a7a0 0a41  otivation .....A
+00000820: 6765 6e74 2070 7261 6374 6974 696f 6e65  gent practitione
+00000830: 7273 2073 7461 7274 2074 6f20 7265 616c  rs start to real
+00000840: 697a 6520 7468 6520 6469 6666 6963 756c  ize the difficul
+00000850: 7479 2069 6e20 7475 6e69 6e67 2061 2022  ty in tuning a "
+00000860: 7765 6c6c 2d72 6f75 6e64 6564 2220 6167  well-rounded" ag
+00000870: 656e 7420 7769 7468 2074 6f6e 7320 6f66  ent with tons of
+00000880: 2074 6f6f 6c73 206f 7220 696e 7374 7275   tools or instru
+00000890: 6374 696f 6e73 2069 6e20 6120 7369 6e67  ctions in a sing
+000008a0: 6c65 206c 6179 6572 2e0a 5265 6365 6e74  le layer..Recent
+000008b0: 2073 7475 6469 6573 206c 696b 6520 5b54   studies like [T
+000008c0: 696e 7953 746f 7269 6573 5d28 6874 7470  inyStories](http
+000008d0: 733a 2f2f 6172 7869 762e 6f72 672f 6162  s://arxiv.org/ab
+000008e0: 732f 3233 3031 2e31 3237 3236 292c 205b  s/2301.12726), [
+000008f0: 5370 6563 6961 6c69 7a69 6e67 2052 6561  Specializing Rea
+00000900: 736f 6e69 6e67 5d28 6874 7470 733a 2f2f  soning](https://
+00000910: 6172 7869 762e 6f72 672f 6162 732f 3233  arxiv.org/abs/23
+00000920: 3031 2e31 3237 3236 292c 205b 4c65 7427  01.12726), [Let'
+00000930: 7320 5665 7269 6679 2053 6253 5d28 6874  s Verify SbS](ht
+00000940: 7470 733a 2f2f 6172 7869 762e 6f72 672f  tps://arxiv.org/
+00000950: 6162 732f 3233 3035 2e32 3030 3530 292c  abs/2305.20050),
+00000960: 205b 5265 574f 4f5d 2868 7474 7073 3a2f   [ReWOO](https:/
+00000970: 2f61 7278 6976 2e6f 7267 2f61 6273 2f32  /arxiv.org/abs/2
+00000980: 3330 352e 3138 3332 3329 2c20 6574 632e  305.18323), etc.
+00000990: 2061 6c73 6f20 706f 696e 7420 7573 2074   also point us t
+000009a0: 6f77 6172 6473 2061 6e20 696e 7475 6974  owards an intuit
+000009b0: 6976 6520 7965 7420 756e 6465 7276 616c  ive yet underval
+000009c0: 7565 6420 6469 7265 6374 696f 6e20 f09f  ued direction ..
+000009d0: 9189 200a 0a60 6060 0a41 6e20 4c4c 4d20  .. ..```.An LLM 
+000009e0: 6973 206d 6f72 6520 6361 7061 626c 6520  is more capable 
+000009f0: 6966 2079 6f75 2063 7265 6174 6520 6120  if you create a 
+00000a00: 636f 6e74 6578 742f 6469 7374 7269 6275  context/distribu
+00000a10: 7469 6f6e 2073 6869 6674 2073 7065 6369  tion shift speci
+00000a20: 616c 697a 6564 2074 6f20 736f 6d65 2074  alized to some t
+00000a30: 6172 6765 7420 7461 736b 732e 0a60 6060  arget tasks..```
+00000a40: 0a53 6164 6c79 2c20 7468 6572 6520 6973  .Sadly, there is
+00000a50: 206e 6f20 7369 6c76 6572 2062 756c 6c65   no silver bulle
+00000a60: 7420 666f 7220 6167 656e 7420 7370 6563  t for agent spec
+00000a70: 6961 6c69 7a61 7469 6f6e 2e20 466f 7220  ialization. For 
+00000a80: 6578 616d 706c 652c 2079 6f75 2063 616e  example, you can
+00000a90: 200a 2d20 5369 6d70 6c79 2061 6464 2060   .- Simply add `
+00000aa0: 4c65 7427 7320 7468 696e 6b20 7374 6570  Let's think step
+00000ab0: 2062 7920 7374 6570 2e60 2069 6e20 796f   by step.` in yo
+00000ac0: 7572 202a 2a70 726f 6d70 742a 2a20 666f  ur **prompt** fo
+00000ad0: 7220 6d6f 7265 2061 6363 7572 6174 6520  r more accurate 
+00000ae0: 4d61 7468 2051 412e 0a2d 2047 6976 6520  Math QA..- Give 
+00000af0: 6120 2a2a 6665 772d 7368 6f74 2a2a 2065  a **few-shot** e
+00000b00: 7865 6d70 6c61 7220 696e 2079 6f75 7220  xemplar in your 
+00000b10: 7072 6f6d 7074 2074 6f20 6775 6964 6520  prompt to guide 
+00000b20: 6120 6265 7474 6572 2072 6561 736f 6e69  a better reasoni
+00000b30: 6e67 2074 7261 6a65 6374 6f72 7920 666f  ng trajectory fo
+00000b40: 7220 6e6f 7665 6c20 706c 6f74 7469 6e67  r novel plotting
+00000b50: 2e0a 2d20 5375 7065 7276 6973 6520 2a2a  ..- Supervise **
+00000b60: 6669 6e65 2d74 756e 696e 672a 2a20 2853  fine-tuning** (S
+00000b70: 4654 2920 796f 7572 2037 3042 2060 6c6c  FT) your 70B `ll
+00000b80: 616d 6132 6020 6c69 6b65 205b 7468 6973  ama2` like [this
+00000b90: 5d28 6874 7470 733a 2f2f 6172 7869 762e  ](https://arxiv.
+00000ba0: 6f72 672f 6162 732f 3233 3035 2e32 3030  org/abs/2305.200
+00000bb0: 3530 2920 746f 206d 6174 6368 2072 6561  50) to match rea
+00000bc0: 736f 6e69 6e67 206f 6620 3137 3542 2047  soning of 175B G
+00000bd0: 5054 2d33 2e35 2e0a 2d20 5475 6e65 2079  PT-3.5..- Tune y
+00000be0: 6f75 7220 6167 656e 7420 2a2a 7061 7261  our agent **para
+00000bf0: 6469 676d 2a2a 206c 696b 6520 7468 6973  digm** like this
+00000c00: 205b 6465 6d6f 5d28 6874 7470 733a 2f2f   [demo](https://
+00000c10: 7777 772e 796f 7574 7562 652e 636f 6d2f  www.youtube.com/
+00000c20: 7761 7463 683f 763d 6469 4a34 4944 6154  watch?v=diJ4IDaT
+00000c30: 345a 3429 2074 6f20 6561 7369 6c79 2068  4Z4) to easily h
+00000c40: 616c 6620 7468 6520 6578 6563 7574 696f  alf the executio
+00000c50: 6e20 7469 6d65 2066 6f72 2053 6561 6368  n time for Seach
+00000c60: 2026 2053 756d 6d61 7269 7a65 2e0a 2d20   & Summarize..- 
+00000c70: 416e 6420 6d6f 7265 202e 2e2e 0a0a 4973  And more .....Is
+00000c80: 6e27 7420 6974 2062 6561 7574 6966 756c  n't it beautiful
+00000c90: 2069 6620 6f6e 6520 7368 6172 6573 2068   if one shares h
+00000ca0: 6973 2065 6666 6f72 7420 696e 2073 7065  is effort in spe
+00000cb0: 6369 616c 697a 6564 2069 6e74 656c 6c69  cialized intelli
+00000cc0: 6765 6e63 652c 2061 6c6c 6f77 696e 6720  gence, allowing 
+00000cd0: 6f74 6865 7273 2074 6f20 7265 7072 6f64  others to reprod
+00000ce0: 7563 652c 2062 7569 6c64 206f 6e2c 206f  uce, build on, o
+00000cf0: 7220 696e 7465 7261 6374 2077 6974 6820  r interact with 
+00000d00: 6974 3f20 f09f a497 2054 6869 7320 6265  it? .... This be
+00000d10: 6c69 6566 2069 6e73 7069 7265 7320 7573  lief inspires us
+00000d20: 2074 6f20 6275 696c 6420 4765 6e74 6f70   to build Gentop
+00000d30: 6961 2c20 0a2a 2a64 6573 6967 6e65 6420  ia, .**designed 
+00000d40: 666f 7220 6167 656e 7420 2a73 7065 6369  for agent *speci
+00000d50: 616c 697a 6174 696f 6e2c 2073 6861 7269  alization, shari
+00000d60: 6e67 2c20 616e 6420 696e 7465 7261 6374  ng, and interact
+00000d70: 696f 6e2c 2a20 746f 2073 7461 636b 696e  ion,* to stackin
+00000d80: 676c 7920 6163 6869 6576 6520 636f 6c6c  gly achieve coll
+00000d90: 6563 7469 7665 2067 726f 7774 6820 746f  ective growth to
+00000da0: 7761 7264 7320 6772 6561 7465 7220 696e  wards greater in
+00000db0: 7465 6c6c 6967 656e 6365 2e2a 2a2e 0a0a  telligence.**...
+00000dc0: 2323 2043 6f72 6520 4665 6174 7572 6573  ## Core Features
+00000dd0: 20f0 9f92 a10a 0a2d 20e2 9a99 efb8 8f20   ......- ...... 
+00000de0: 436f 6e66 6967 2d64 7269 7665 6e20 6167  Config-driven ag
+00000df0: 656e 7420 6173 7365 6d62 6c69 6e67 2061  ent assembling a
+00000e00: 6e64 2063 6861 742e 0a2d 20f0 9f9a 8020  nd chat..- .... 
+00000e10: 4c61 7267 6520 616d 6f75 6e74 206f 6620  Large amount of 
+00000e20: 7072 6562 7569 6c74 2061 6765 6e74 2074  prebuilt agent t
+00000e30: 7970 6573 2c20 4c4c 4d20 636c 6965 6e74  ypes, LLM client
+00000e40: 732c 2074 6f6f 6c73 2c20 6d65 6d6f 7279  s, tools, memory
+00000e50: 2073 7973 7465 6d73 2c20 616e 6420 6d6f   systems, and mo
+00000e60: 7265 2e0a 2d20 f09f aab6 204c 6967 6874  re..- .... Light
+00000e70: 7765 6967 6874 2061 6e64 2068 6967 686c  weight and highl
+00000e80: 7920 6578 7465 6e73 6962 6c65 2069 6d70  y extensible imp
+00000e90: 6c65 6d65 6e74 6174 696f 6e20 6f66 2065  lementation of e
+00000ea0: 7373 656e 7469 616c 2063 6f6d 706f 6e65  ssential compone
+00000eb0: 6e74 732e 0a2d 20f0 9fa7 aa20 416c 6967  nts..- .... Alig
+00000ec0: 6e69 6e67 2077 6974 6820 7374 6174 652d  ning with state-
+00000ed0: 6f66 2d74 6865 2d61 7274 2041 4920 7265  of-the-art AI re
+00000ee0: 7365 6172 6368 2e0a 2d20 f09f a49d 2045  search..- .... E
+00000ef0: 6e61 626c 696e 6720 6d75 6c74 692d 6167  nabling multi-ag
+00000f00: 656e 7420 696e 7465 7261 6374 696f 6e73  ent interactions
+00000f10: 2e0a 2d20 f09f a681 2055 6e69 7175 6520  ..- .... Unique 
+00000f20: 706c 6174 666f 726d 206f 6620 6167 656e  platform of agen
+00000f30: 7420 7a6f 6f20 616e 6420 6576 616c 2062  t zoo and eval b
+00000f40: 656e 6368 6d61 726b 2e0a 0a23 2320 5175  enchmark...## Qu
+00000f50: 6963 6b20 5374 6172 7420 f09f 8d8f 0a60  ick Start .....`
+00000f60: 6060 0a63 6f6e 6461 2063 7265 6174 6520  ``.conda create 
+00000f70: 2d2d 6e61 6d65 2067 656e 7465 6e76 2070  --name gentenv p
+00000f80: 7974 686f 6e3d 332e 3130 0a63 6f6e 6461  ython=3.10.conda
+00000f90: 2061 6374 6976 6174 6520 6765 6e74 656e   activate genten
+00000fa0: 760a 7069 7020 696e 7374 616c 6c20 6765  v.pip install ge
+00000fb0: 6e74 6f70 6961 0a60 6060 0a6f 7220 6966  ntopia.```.or if
+00000fc0: 2079 6f75 2077 616e 7420 746f 2062 7569   you want to bui
+00000fd0: 6c64 2077 6974 6820 6f70 656e 204c 4c4d  ld with open LLM
+00000fe0: 7320 6c6f 6361 6c6c 7920 f09f 9189 2060  s locally .... `
+00000ff0: 7069 7020 696e 7374 616c 6c20 6765 6e74  pip install gent
+00001000: 6f70 6961 5b68 7567 6769 6e67 6661 6365  opia[huggingface
+00001010: 5d60 0a0a 4669 7273 7420 7469 6d65 2074  ]`..First time t
+00001020: 6f20 4765 6e74 6f70 6961 3f20 4772 6162  o Gentopia? Grab
+00001030: 2061 2063 6f66 6665 6520 e298 9520 616e   a coffee ... an
+00001040: 6420 0a0a 5461 6b65 207e 2038 206d 696e  d ..Take ~ 8 min
+00001050: 7320 746f 2063 6865 636b 206f 7574 2074  s to check out t
+00001060: 6865 2066 6f6c 6c6f 7769 6e67 2064 656d  he following dem
+00001070: 6f20 7475 746f 7269 616c 7320 5b21 5b59  o tutorials [![Y
+00001080: 6f75 5475 6265 2043 6861 6e6e 656c 2053  ouTube Channel S
+00001090: 7562 7363 7269 6265 7273 5d28 6874 7470  ubscribers](http
+000010a0: 733a 2f2f 696d 672e 7368 6965 6c64 732e  s://img.shields.
+000010b0: 696f 2f79 6f75 7475 6265 2f63 6861 6e6e  io/youtube/chann
+000010c0: 656c 2f76 6965 7773 2f55 4339 5143 6a63  el/views/UC9QCjc
+000010d0: 7348 4a56 4b6a 4b5a 325a 6d72 7138 3376  sHJVKjKZ2Zmrq83v
+000010e0: 4129 5d28 6874 7470 733a 2f2f 7777 772e  A)](https://www.
+000010f0: 796f 7574 7562 652e 636f 6d2f 6368 616e  youtube.com/chan
+00001100: 6e65 6c2f 5543 3951 436a 6373 484a 564b  nel/UC9QCjcsHJVK
+00001110: 6a4b 5a32 5a6d 7271 3833 7641 2920 0a0a  jKZ2Zmrq83vA) ..
+00001120: 3c64 6976 2073 7479 6c65 3d22 6469 7370  <div style="disp
+00001130: 6c61 793a 2066 6c65 783b 206a 7573 7469  lay: flex; justi
+00001140: 6679 2d63 6f6e 7465 6e74 3a20 7370 6163  fy-content: spac
+00001150: 652d 6172 6f75 6e64 3b22 3e0a 2020 0a3c  e-around;">.  .<
+00001160: 6120 6872 6566 3d22 6874 7470 733a 2f2f  a href="https://
+00001170: 7777 772e 796f 7574 7562 652e 636f 6d2f  www.youtube.com/
+00001180: 7761 7463 683f 763d 3764 5a33 5a76 7349  watch?v=7dZ3ZvsI
+00001190: 3773 7722 2074 6172 6765 743d 225f 626c  7sw" target="_bl
+000011a0: 616e 6b22 3e0a 2020 3c69 6d67 2073 7263  ank">.  <img src
+000011b0: 3d22 6874 7470 733a 2f2f 696d 672e 796f  ="https://img.yo
+000011c0: 7574 7562 652e 636f 6d2f 7669 2f37 645a  utube.com/vi/7dZ
+000011d0: 335a 7673 4937 7377 2f68 7164 6566 6175  3ZvsI7sw/hqdefau
+000011e0: 6c74 2e6a 7067 2220 616c 743d 2256 6964  lt.jpg" alt="Vid
+000011f0: 656f 2031 2220 7374 796c 653d 2277 6964  eo 1" style="wid
+00001200: 7468 3a33 3225 3b22 3e0a 3c2f 613e 0a0a  th:32%;">.</a>..
+00001210: 3c61 2068 7265 663d 2268 7474 7073 3a2f  <a href="https:/
+00001220: 2f77 7777 2e79 6f75 7475 6265 2e63 6f6d  /www.youtube.com
+00001230: 2f77 6174 6368 3f76 3d58 5473 7639 706b  /watch?v=XTsv9pk
+00001240: 3641 4f41 2220 7461 7267 6574 3d22 5f62  6AOA" target="_b
+00001250: 6c61 6e6b 223e 0a20 203c 696d 6720 7372  lank">.  <img sr
+00001260: 633d 2268 7474 7073 3a2f 2f69 6d67 2e79  c="https://img.y
+00001270: 6f75 7475 6265 2e63 6f6d 2f76 692f 5854  outube.com/vi/XT
+00001280: 7376 3970 6b36 414f 412f 6871 6465 6661  sv9pk6AOA/hqdefa
+00001290: 756c 742e 6a70 6722 2061 6c74 3d22 5669  ult.jpg" alt="Vi
+000012a0: 6465 6f20 3222 2073 7479 6c65 3d22 7769  deo 2" style="wi
+000012b0: 6474 683a 3332 253b 223e 0a3c 2f61 3e0a  dth:32%;">.</a>.
+000012c0: 0a3c 6120 6872 6566 3d22 6874 7470 733a  .<a href="https:
+000012d0: 2f2f 7777 772e 796f 7574 7562 652e 636f  //www.youtube.co
+000012e0: 6d2f 7761 7463 683f 763d 6469 4a34 4944  m/watch?v=diJ4ID
+000012f0: 6154 345a 3422 2074 6172 6765 743d 225f  aT4Z4" target="_
+00001300: 626c 616e 6b22 3e0a 2020 3c69 6d67 2073  blank">.  <img s
+00001310: 7263 3d22 6874 7470 733a 2f2f 696d 672e  rc="https://img.
+00001320: 796f 7574 7562 652e 636f 6d2f 7669 2f64  youtube.com/vi/d
+00001330: 694a 3449 4461 5434 5a34 2f68 7164 6566  iJ4IDaT4Z4/hqdef
+00001340: 6175 6c74 2e6a 7067 2220 616c 743d 2256  ault.jpg" alt="V
+00001350: 6964 656f 2033 2220 7374 796c 653d 2277  ideo 3" style="w
+00001360: 6964 7468 3a33 3225 3b22 3e0a 3c2f 613e  idth:32%;">.</a>
+00001370: 0a0a 3c2f 6469 763e 0a0a 4f72 2063 6865  ..</div>..Or che
+00001380: 636b 206f 7574 2074 6865 205b 5175 6963  ck out the [Quic
+00001390: 6b20 5374 6172 745d 2868 7474 7073 3a2f  k Start](https:/
+000013a0: 2f67 656e 746f 7069 612e 7265 6164 7468  /gentopia.readth
+000013b0: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+000013c0: 7374 2f71 7569 636b 5f73 7461 7274 2e68  st/quick_start.h
+000013d0: 746d 6c29 2044 6f63 2e0a 0a23 2320 446f  tml) Doc...## Do
+000013e0: 6375 6d65 6e74 6174 696f 6e20 f09f 9396  cumentation ....
+000013f0: 0a53 6565 205b 6865 7265 5d28 6874 7470  .See [here](http
+00001400: 733a 2f2f 6765 6e74 6f70 6961 2e72 6561  s://gentopia.rea
+00001410: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00001420: 6174 6573 742f 696e 6465 782e 6874 6d6c  atest/index.html
+00001430: 2920 666f 7220 6675 6c6c 2064 6f63 756d  ) for full docum
+00001440: 656e 7461 7469 6f6e 2e0a 0af0 9f8c 9f20  entation....... 
+00001450: 4869 6768 6c69 6768 7420 546f 7069 6373  Highlight Topics
+00001460: 20f0 9f8c 9f20 0a2d 205b f09f a496 2041   .... .- [.... A
+00001470: 6765 6e74 2054 656d 706c 6174 6573 5d28  gent Templates](
+00001480: 6874 7470 733a 2f2f 6765 6e74 6f70 6961  https://gentopia
+00001490: 2e72 6561 6474 6865 646f 6373 2e69 6f2f  .readthedocs.io/
+000014a0: 656e 2f6c 6174 6573 742f 7175 6963 6b5f  en/latest/quick_
+000014b0: 7374 6172 742e 6874 6d6c 2376 616e 696c  start.html#vanil
+000014c0: 6c61 2d61 6765 6e74 290a 2d20 5be2 9bb0  la-agent).- [...
+000014d0: efb8 8f20 4869 6572 6172 6368 6963 616c  ... Hierarchical
+000014e0: 2041 6765 6e74 735d 2868 7474 7073 3a2f   Agents](https:/
+000014f0: 2f67 656e 746f 7069 612e 7265 6164 7468  /gentopia.readth
+00001500: 6564 6f63 732e 696f 2f65 6e2f 6c61 7465  edocs.io/en/late
+00001510: 7374 2f61 6765 6e74 5f63 6f6d 706f 6e65  st/agent_compone
+00001520: 6e74 732e 6874 6d6c 2361 6765 6e74 2d61  nts.html#agent-a
+00001530: 732d 706c 7567 696e 290a 2d20 5bf0 9fa5  s-plugin).- [...
+00001540: 8720 556e 6971 7565 2041 6765 6e74 2042  . Unique Agent B
+00001550: 656e 6368 6d61 726b 5d28 6874 7470 733a  enchmark](https:
+00001560: 2f2f 6765 6e74 6f70 6961 2e72 6561 6474  //gentopia.readt
+00001570: 6865 646f 6373 2e69 6f2f 656e 2f6c 6174  hedocs.io/en/lat
+00001580: 6573 742f 6765 6e74 706f 6f6c 2e68 746d  est/gentpool.htm
+00001590: 6c23 6167 656e 742d 6576 616c 7561 7469  l#agent-evaluati
+000015a0: 6f6e 290a 2d20 5bf0 9fa6 9920 4f70 656e  on).- [.... Open
+000015b0: 204c 4c4d 2053 7570 706f 7274 735d 2868   LLM Supports](h
+000015c0: 7474 7073 3a2f 2f67 656e 746f 7069 612e  ttps://gentopia.
+000015d0: 7265 6164 7468 6564 6f63 732e 696f 2f65  readthedocs.io/e
+000015e0: 6e2f 6c61 7465 7374 2f61 6765 6e74 5f63  n/latest/agent_c
+000015f0: 6f6d 706f 6e65 6e74 732e 6874 6d6c 2368  omponents.html#h
+00001600: 7567 6769 6e67 6661 6365 2d6f 7065 6e2d  uggingface-open-
+00001610: 6c6c 6d73 290a 2d20 5bf0 9fa7 a020 4869  llms).- [.... Hi
+00001620: 6768 2d50 6572 666f 726d 616e 6365 204d  gh-Performance M
+00001630: 656d 6f72 795d 2868 7474 7073 3a2f 2f67  emory](https://g
+00001640: 656e 746f 7069 612e 7265 6164 7468 6564  entopia.readthed
+00001650: 6f63 732e 696f 2f65 6e2f 6c61 7465 7374  ocs.io/en/latest
+00001660: 2f61 6765 6e74 5f63 6f6d 706f 6e65 6e74  /agent_component
+00001670: 732e 6874 6d6c 236c 6f6e 672d 7368 6f72  s.html#long-shor
+00001680: 742d 7465 726d 2d6d 656d 6f72 7929 0a0a  t-term-memory)..
+00001690: 2323 204a 6f69 6e20 7573 2120 f09f 8c8e  ## Join us! ....
+000016a0: 0a0a 5061 7274 6963 6970 6174 6520 696e  ..Participate in
+000016b0: 2074 6869 7320 5574 6f70 6961 206f 6620   this Utopia of 
+000016c0: 7375 7065 7269 6e74 656c 6c69 6765 6e63  superintelligenc
+000016d0: 6520 616e 6420 6865 6c70 2069 7420 6772  e and help it gr
+000016e0: 6f77 7321 2041 7320 6120 6675 6c6c 7920  ows! As a fully 
+000016f0: 6f70 656e 2d73 6f75 7263 6520 7072 6f6a  open-source proj
+00001700: 6563 742c 2077 6520 6465 7665 6c6f 7020  ect, we develop 
+00001710: 756e 6465 7220 7075 626c 6963 2061 6476  under public adv
+00001720: 6963 652c 2069 6465 6173 2c20 616e 6420  ice, ideas, and 
+00001730: 7375 7065 7276 6973 696f 6e2e 204d 6561  supervision. Mea
+00001740: 6e77 6869 6c65 2c20 6865 7265 2061 7265  nwhile, here are
+00001750: 2077 6179 7320 796f 7520 6d61 7920 636f   ways you may co
+00001760: 6e74 7269 6275 7465 2074 6f20 4765 6e74  ntribute to Gent
+00001770: 6f70 6961 2e0a 0a2d 20f0 9f90 9b20 506f  opia...- .... Po
+00001780: 7374 2061 6e20 5b69 7373 7565 5d28 6874  st an [issue](ht
+00001790: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+000017a0: 2f47 656e 746f 7069 612d 4149 2f47 656e  /Gentopia-AI/Gen
+000017b0: 746f 7069 612f 6973 7375 6573 2920 7265  topia/issues) re
+000017c0: 7175 6573 7469 6e67 206e 6563 6573 7361  questing necessa
+000017d0: 7279 2062 7567 2066 6978 6573 2c20 6164  ry bug fixes, ad
+000017e0: 6469 7469 6f6e 616c 2066 6561 7475 7265  ditional feature
+000017f0: 732c 206f 7220 726f 6164 6d61 7020 7375  s, or roadmap su
+00001800: 6767 6573 7469 6f6e 732e 2028 4368 6563  ggestions. (Chec
+00001810: 6b20 636c 6f73 6564 206f 6e65 7320 6669  k closed ones fi
+00001820: 7273 7429 0a2d 20f0 9f8e af20 4f75 7220  rst).- .... Our 
+00001830: 6465 7620 7465 616d 206d 6565 7473 2077  dev team meets w
+00001840: 6565 6b6c 7920 746f 2067 726f 6f6d 205b  eekly to groom [
+00001850: 6261 636b 6c6f 675d 2868 7474 7073 3a2f  backlog](https:/
+00001860: 2f67 6974 6875 622e 636f 6d2f 6f72 6773  /github.com/orgs
+00001870: 2f47 656e 746f 7069 612d 4149 2f70 726f  /Gentopia-AI/pro
+00001880: 6a65 6374 732f 3129 2069 6e74 6f20 7469  jects/1) into ti
+00001890: 636b 6574 732e 2057 6869 6c65 2077 6520  ckets. While we 
+000018a0: 776f 726b 206f 6e20 7468 656d 2c20 796f  work on them, yo
+000018b0: 7520 6361 6e20 7069 636b 2075 7020 6f74  u can pick up ot
+000018c0: 6865 7273 2061 6e64 2063 7265 6174 6520  hers and create 
+000018d0: 6120 5b50 756c 6c20 5265 7175 6573 745d  a [Pull Request]
+000018e0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+000018f0: 636f 6d2f 4765 6e74 6f70 6961 2d41 492f  com/Gentopia-AI/
+00001900: 4765 6e74 6f70 6961 2f70 756c 6c73 2920  Gentopia/pulls) 
+00001910: 746f 2072 6571 7565 7374 2061 206d 6572  to request a mer
+00001920: 6765 2e20 5765 2061 6c77 6179 7320 7765  ge. We always we
+00001930: 6c63 6f6d 6520 6e65 7720 6d65 6d62 6572  lcome new member
+00001940: 7320 696e 2074 6869 7320 7761 792e 0a2d  s in this way..-
+00001950: 20f0 9fa4 9d20 5368 6172 6520 796f 7572   .... Share your
+00001960: 2073 7065 6369 616c 697a 6564 2061 6765   specialized age
+00001970: 6e74 2074 6f20 5b47 656e 7450 6f6f 6c5d  nt to [GentPool]
+00001980: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00001990: 636f 6d2f 4765 6e74 6f70 6961 2d41 492f  com/Gentopia-AI/
+000019a0: 4765 6e74 506f 6f6c 2921 2043 7265 6174  GentPool)! Creat
+000019b0: 6520 616e 2041 6765 6e74 2050 5220 285b  e an Agent PR ([
+000019c0: 6578 616d 706c 655d 2829 2920 746f 206d  example]()) to m
+000019d0: 6572 6765 2079 6f75 7220 7765 6c6c 2d74  erge your well-t
+000019e0: 756e 6564 2061 6765 6e74 2069 6e74 6f20  uned agent into 
+000019f0: 7468 6520 706f 6f6c 2e20 5468 6973 2061  the pool. This a
+00001a00: 6c6c 6f77 7320 6f74 6865 7273 2074 6f20  llows others to 
+00001a10: 7573 6520 6f72 2062 7569 6c64 2075 706f  use or build upo
+00001a20: 6e20 796f 7572 2061 6765 6e74 2e20 0a2d  n your agent. .-
+00001a30: 20e2 ad90 2048 656c 7020 7573 2073 7072   ... Help us spr
+00001a40: 6561 6421 2047 6976 6520 7573 2061 2073  ead! Give us a s
+00001a50: 7461 722c 2066 6f6c 6c6f 7720 7573 206f  tar, follow us o
+00001a60: 6e20 5b54 7769 7474 6572 5d28 6874 7470  n [Twitter](http
+00001a70: 733a 2f2f 7477 6974 7465 722e 636f 6d2f  s://twitter.com/
+00001a80: 4765 6e74 6f70 6961 4149 292c 206a 6f69  GentopiaAI), joi
+00001a90: 6e20 6f75 7220 5b44 6973 636f 7264 5d28  n our [Discord](
+00001aa0: 6874 7470 733a 2f2f 6469 7363 6f72 642e  https://discord.
+00001ab0: 6767 2f41 5350 5039 4d59 3951 4b29 2c20  gg/ASPP9MY9QK), 
+00001ac0: 616e 6420 7368 6172 6520 7769 7468 2079  and share with y
+00001ad0: 6f75 7220 6672 6965 6e64 7321 2020 0a0a  our friends!  ..
+00001ae0: 0a                                       .
```

### Comparing `gentopia-0.0.1/gentopia.egg-info/SOURCES.txt` & `gentopia-0.0.2/gentopia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gentopia-0.0.1/setup.py` & `gentopia-0.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gentopia',
-    version='0.0.1',
+    version='0.0.2',
     packages=find_packages(exclude=['llm', 'llm.*']),
     url='https://github.com/Gentopia-AI/Gentopia',
-    license='Apache-2.0 license',
+    license='MIT license',
     author='billxbf',
     author_email='billxbf@gmail.com',
     description='Gentopia provides extensive utilities to assembles ALM agents driven by configs.',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     extras_require={
             'huggingface': ['torch', 'transformers', 'optimum', 'peft'],
@@ -36,9 +36,12 @@
         'PyYAML',
         'requests',
         'setuptools',
         'uvicorn',
         'openai',
         'pexpect',
         'gradio_client',
+        'pinecone-client',
+        'chroma',
+        'chromadb',
     ],
 )
```

