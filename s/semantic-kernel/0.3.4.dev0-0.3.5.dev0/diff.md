# Comparing `tmp/semantic_kernel-0.3.4.dev0.tar.gz` & `tmp/semantic_kernel-0.3.5.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.3.4.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.3.5.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.3.4.dev0.tar` & `semantic_kernel-0.3.5.dev0.tar`

### file list

```diff
@@ -1,107 +1,120 @@
--rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.000000 semantic_kernel-0.3.4.dev0/pip/README.md
--rw-r--r--   0        0        0     1412 2023-07-21 00:27:08.415513 semantic_kernel-0.3.4.dev0/pyproject.toml
--rw-r--r--   0        0        0     1375 2023-07-12 19:14:40.912511 semantic_kernel-0.3.4.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0      719 2023-05-25 17:48:21.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/ai_exception.py
--rw-r--r--   0        0        0     1792 2023-06-12 17:06:53.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1321 2023-07-14 16:57:26.312407 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1484 2023-07-14 16:57:26.312942 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-30 18:57:02.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      352 2023-04-30 18:57:02.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     6161 2023-06-12 17:06:53.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      892 2023-04-30 18:57:02.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     8903 2023-07-16 00:59:27.692753 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     5788 2023-07-16 00:59:27.693316 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2723 2023-05-15 18:12:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0     1616 2023-06-12 17:06:53.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      242 2023-07-21 00:24:52.991872 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
--rw-r--r--   0        0        0    15609 2023-07-21 00:24:52.992413 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
--rw-r--r--   0        0        0     8224 2023-07-21 00:24:52.992894 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
--rw-r--r--   0        0        0      182 2023-05-18 17:32:52.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    15260 2023-07-21 00:24:52.994825 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     4426 2023-07-16 00:58:38.000353 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0      133 2023-07-21 00:24:52.995551 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/milvus/__init__.py
--rw-r--r--   0        0        0    16859 2023-07-21 00:24:52.995917 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
--rw-r--r--   0        0        0      190 2023-07-06 22:13:35.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/pinecone/__init__.py
--rw-r--r--   0        0        0    14928 2023-07-12 19:14:40.913001 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
--rw-r--r--   0        0        0     1154 2023-07-06 22:13:35.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/pinecone/utils.py
--rw-r--r--   0        0        0      190 2023-07-12 19:14:40.913420 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/postgres/__init__.py
--rw-r--r--   0        0        0    20480 2023-07-12 19:14:40.913726 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
--rw-r--r--   0        0        0    11295 2023-06-12 17:06:53.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
--rw-r--r--   0        0        0      111 2023-07-17 21:15:24.598216 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/search_engine/__init__.py
--rw-r--r--   0        0        0     2842 2023-07-17 21:15:24.598630 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/search_engine/bing_connector.py
--rw-r--r--   0        0        0      173 2023-07-17 21:15:24.599030 semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/search_engine/connector.py
--rw-r--r--   0        0        0      804 2023-07-17 21:15:24.599960 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2510 2023-05-15 18:12:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
--rw-r--r--   0        0        0     2131 2023-07-16 00:59:27.693756 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/http_skill.py
--rw-r--r--   0        0        0     3171 2023-07-06 22:13:35.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/math_skill.py
--rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2462 2023-07-16 00:59:27.694343 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     7909 2023-07-16 00:59:27.694865 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0      678 2023-07-16 00:59:27.695359 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/wait_skill.py
--rw-r--r--   0        0        0     1950 2023-07-17 21:15:24.600357 semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/web_search_engine_skill.py
--rw-r--r--   0        0        0    32289 2023-07-17 21:15:24.601483 semantic_kernel-0.3.4.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     1726 2023-07-16 00:59:27.695868 semantic_kernel-0.3.4.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      160 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2544 2023-06-08 17:22:29.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     3912 2023-07-12 19:14:40.914195 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     2186 2023-07-21 00:24:52.996840 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1272 2023-06-08 17:22:29.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6354 2023-07-16 00:42:59.250269 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     1298 2023-06-08 17:22:29.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    16088 2023-07-06 22:13:35.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      158 2023-05-08 23:38:10.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/planning/__init__.py
--rw-r--r--   0        0        0     7538 2023-07-06 22:13:35.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/planning/basic_planner.py
--rw-r--r--   0        0        0    15624 2023-07-16 00:59:27.696327 semantic_kernel-0.3.4.dev0/semantic_kernel/planning/plan.py
--rw-r--r--   0        0        0      932 2023-05-19 23:02:13.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      694 2023-06-05 21:39:19.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     4525 2023-06-12 17:06:53.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     2199 2023-06-12 17:06:53.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      830 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      473 2023-04-30 18:57:03.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      667 2023-04-30 18:57:03.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     8568 2023-07-16 00:58:38.006510 semantic_kernel-0.3.4.dev0/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      403 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2694 2023-07-12 19:14:40.915313 semantic_kernel-0.3.4.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.000000 semantic_kernel-0.3.4.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     1843 1970-01-01 00:00:00.000000 semantic_kernel-0.3.4.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.000000 semantic_kernel-0.3.5.dev0/pip/README.md
+-rw-r--r--   0        0        0     1514 2023-08-02 21:24:55.086486 semantic_kernel-0.3.5.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1375 2023-07-12 19:14:40.912511 semantic_kernel-0.3.5.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0      719 2023-05-25 17:48:21.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/ai_exception.py
+-rw-r--r--   0        0        0     1792 2023-06-12 17:06:53.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1321 2023-07-14 16:57:26.312407 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1484 2023-07-14 16:57:26.312942 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-30 18:57:02.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      352 2023-04-30 18:57:02.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     6161 2023-06-12 17:06:53.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      892 2023-04-30 18:57:02.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     8903 2023-07-16 00:59:27.692753 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     5788 2023-07-16 00:59:27.693316 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     2723 2023-05-15 18:12:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1616 2023-06-12 17:06:53.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      242 2023-07-21 00:24:52.991872 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/__init__.py
+-rw-r--r--   0        0        0    15609 2023-07-21 00:24:52.992413 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py
+-rw-r--r--   0        0        0     8224 2023-07-21 00:24:52.992894 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py
+-rw-r--r--   0        0        0      182 2023-05-18 17:32:52.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    15093 2023-08-02 21:24:01.722277 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4426 2023-07-16 00:58:38.000353 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      133 2023-07-21 00:24:52.995551 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/milvus/__init__.py
+-rw-r--r--   0        0        0    16859 2023-07-21 00:24:52.995917 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py
+-rw-r--r--   0        0        0      190 2023-07-06 22:13:35.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0        0        0    14928 2023-07-12 19:14:40.913001 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0        0        0     1154 2023-07-06 22:13:35.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/pinecone/utils.py
+-rw-r--r--   0        0        0      190 2023-07-12 19:14:40.913420 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/postgres/__init__.py
+-rw-r--r--   0        0        0    20480 2023-07-12 19:14:40.913726 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
+-rw-r--r--   0        0        0      182 2023-08-02 21:24:01.723071 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/qdrant/__init__.py
+-rw-r--r--   0        0        0    11910 2023-08-02 21:24:01.723452 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/qdrant/qdrant_memory_store.py
+-rw-r--r--   0        0        0    11295 2023-06-12 17:06:53.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0      265 2023-08-02 21:24:01.724044 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/search_engine/__init__.py
+-rw-r--r--   0        0        0     2891 2023-08-02 21:24:01.724670 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/search_engine/bing_connector.py
+-rw-r--r--   0        0        0      254 2023-08-02 21:24:01.725238 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/search_engine/connector.py
+-rw-r--r--   0        0        0     3268 2023-08-02 21:24:01.725609 semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/search_engine/google_connector.py
+-rw-r--r--   0        0        0      804 2023-07-17 21:15:24.599960 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2510 2023-05-15 18:12:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
+-rw-r--r--   0        0        0     2131 2023-07-16 00:59:27.693756 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/http_skill.py
+-rw-r--r--   0        0        0     3172 2023-08-02 21:24:01.726389 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/math_skill.py
+-rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2462 2023-07-16 00:59:27.694343 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     7909 2023-07-16 00:59:27.694865 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0      678 2023-07-16 00:59:27.695359 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/wait_skill.py
+-rw-r--r--   0        0        0     1950 2023-07-17 21:15:24.600357 semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/web_search_engine_skill.py
+-rw-r--r--   0        0        0    32289 2023-07-17 21:15:24.601483 semantic_kernel-0.3.5.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     1726 2023-07-16 00:59:27.695868 semantic_kernel-0.3.5.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      160 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2544 2023-06-08 17:22:29.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     3912 2023-07-12 19:14:40.914195 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     7272 2023-08-02 21:24:01.726940 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1666 2023-08-02 21:24:01.727814 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6354 2023-07-16 00:42:59.250269 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     3418 2023-08-02 21:24:01.728381 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    16088 2023-07-06 22:13:35.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      408 2023-08-02 21:24:01.729218 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/__init__.py
+-rw-r--r--   0        0        0    12891 2023-08-02 21:24:01.729812 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/action_planner/action_planner.py
+-rw-r--r--   0        0        0      355 2023-08-02 21:24:01.730504 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/action_planner/skprompt.txt
+-rw-r--r--   0        0        0     7538 2023-07-06 22:13:35.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/basic_planner.py
+-rw-r--r--   0        0        0    16642 2023-08-02 21:24:01.731111 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/plan.py
+-rw-r--r--   0        0        0     1198 2023-08-02 21:24:01.731437 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/planning_exception.py
+-rw-r--r--   0        0        0      723 2023-08-02 21:24:01.732600 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/config.json
+-rw-r--r--   0        0        0     3005 2023-08-02 21:24:01.732891 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/Skills/SequentialPlanning/skprompt.txt
+-rw-r--r--   0        0        0      142 2023-08-02 21:24:01.733143 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/__init__.py
+-rw-r--r--   0        0        0     5761 2023-08-02 21:24:01.733497 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/sequential_planner.py
+-rw-r--r--   0        0        0     1147 2023-08-02 21:24:01.733879 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_config.py
+-rw-r--r--   0        0        0     8558 2023-08-02 21:24:01.734424 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_extensions.py
+-rw-r--r--   0        0        0     5515 2023-08-02 21:24:01.734840 semantic_kernel-0.3.5.dev0/semantic_kernel/planning/sequential_planner/sequential_planner_parser.py
+-rw-r--r--   0        0        0      932 2023-05-19 23:02:13.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      694 2023-06-05 21:39:19.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     4525 2023-06-12 17:06:53.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0      322 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     2199 2023-06-12 17:06:53.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      858 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      837 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      803 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      830 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      473 2023-04-30 18:57:03.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      667 2023-04-30 18:57:03.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     8568 2023-07-16 00:58:38.006510 semantic_kernel-0.3.5.dev0/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      403 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2694 2023-07-12 19:14:40.915313 semantic_kernel-0.3.5.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.000000 semantic_kernel-0.3.5.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     1843 1970-01-01 00:00:00.000000 semantic_kernel-0.3.5.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.3.4.dev0/pip/README.md` & `semantic_kernel-0.3.5.dev0/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/pyproject.toml` & `semantic_kernel-0.3.5.dev0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.3.4.dev"
+version = "0.3.5.dev"
 description = ""
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -12,25 +12,28 @@
 openai = "^0.27.0"
 aiofiles = "^23.1.0"
 python-dotenv = "1.0.0"
 regex = "^2023.6.3"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "3.3.3"
-black = {version = "23.3.0", allow-prereleases = true}
+black = {version = "23.7.0", allow-prereleases = true}
 ipykernel = "^6.21.1"
 pytest = "7.4.0"
-ruff = "0.0.278"
-pytest-asyncio = "0.21.0"
+ruff = "0.0.281"
+pytest-asyncio = "0.21.1"
 
 [tool.poetry.group.hugging_face.dependencies]
 transformers = "^4.28.1"
 sentence-transformers = "^2.2.2"
 torch = "2.0.0"
 
+[tool.poetry.group.qdrant.dependencies]
+qdrant-client = {version = "^1.3.2", python = ">=3.8,<3.12"}
+
 [tool.poetry.group.chromadb.dependencies]
 chromadb = "^0.4.0"
 
 [tool.poetry.group.milvus.dependencies]
 pymilvus = "^2.2.11"
 milvus = "^2.2.11"
```

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/__init__.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/ai_exception.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/chat_request_settings.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/chat_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/complete_request_settings.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/complete_request_settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/azure_cognitive_search_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/azure_cognitive_search/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,16 +123,14 @@
             collection_name {str} -- The name of the collection to delete.
 
         Returns:
             None
         """
         # Current version of ChromeDB reject camel case collection names.
         self._client.delete_collection(name=camel_to_snake(collection_name))
-        if self._persist_directory is not None:
-            self._client.persist()
 
     async def does_collection_exist_async(self, collection_name: str) -> bool:
         """Checks if a collection exists.
 
         Arguments:
             collection_name {str} -- The name of the collection to check.
 
@@ -171,17 +169,14 @@
         collection.add(
             metadatas=metadata,
             # by providing embeddings, we can skip the chroma's embedding function call
             embeddings=record.embedding.tolist(),
             documents=record._text,
             ids=record._key,
         )
-
-        if self._persist_directory is not None:
-            self._client.persist()
         return record._key
 
     async def upsert_batch_async(
         self, collection_name: str, records: List[MemoryRecord]
     ) -> List[str]:
         """Upserts a batch of records.
```

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/milvus/milvus_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/pinecone/utils.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/connectors/search_engine/bing_connector.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/connectors/search_engine/bing_connector.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright (c) Microsoft. All rights reserved.
+
 import urllib
 from logging import Logger
 from typing import List, Optional
 
 import aiohttp
 
 from semantic_kernel.connectors.search_engine.connector import ConnectorBase
```

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/__init__.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/conversation_summary_skill.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/conversation_summary_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/http_skill.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/http_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/math_skill.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/math_skill.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # Copyright (c) Microsoft. All rights reserved.
 
+
 from semantic_kernel.orchestration.sk_context import SKContext
 from semantic_kernel.skill_definition import sk_function, sk_function_context_parameter
 
 
 class MathSkill:
     """
     Description: MathSkill provides a set of functions to make Math calculations.
```

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/wait_skill.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/wait_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/core_skills/web_search_engine_skill.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/core_skills/web_search_engine_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/kernel.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/kernel_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/memory/memory_record.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/memory/null_memory.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,39 +11,44 @@
         self,
         collection: str,
         text: str,
         id: str,
         description: Optional[str] = None,
         additional_metadata: Optional[str] = None,
     ) -> None:
+        """Nullifies behavior of SemanticTextMemoryBase.save_information_async()"""
         return None
 
     async def save_reference_async(
         self,
         collection: str,
         text: str,
         external_id: str,
         external_source_name: str,
         description: Optional[str] = None,
         additional_metadata: Optional[str] = None,
     ) -> None:
+        """Nullifies behavior of SemanticTextMemoryBase.save_reference_async()"""
         return None
 
     async def get_async(
         self, collection: str, query: str
     ) -> Optional[MemoryQueryResult]:
+        """Nullifies behavior of SemanticTextMemoryBase.get_async()"""
         return None
 
     async def search_async(
         self,
         collection: str,
         query: str,
         limit: int = 1,
         min_relevance_score: float = 0.7,
     ) -> List[MemoryQueryResult]:
+        """Nullifies behavior of SemanticTextMemoryBase.search_async()"""
         return []
 
     async def get_collections_async(self) -> List[str]:
+        """Nullifies behavior of SemanticTextMemoryBase.get_collections_async()"""
         return []
 
 
 NullMemory.instance = NullMemory()  # type: ignore
```

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/planning/basic_planner.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/planning/basic_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/planning/plan.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/planning/plan.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import asyncio
 import re
 import threading
 from logging import Logger
-from typing import Any, Callable, List, Optional
+from typing import Any, Callable, List, Optional, Union
 
 from semantic_kernel import Kernel
 from semantic_kernel.connectors.ai import CompleteRequestSettings
 from semantic_kernel.connectors.ai.text_completion_client_base import (
     TextCompletionClientBase,
 )
 from semantic_kernel.kernel_exception import KernelException
@@ -16,14 +16,15 @@
 from semantic_kernel.orchestration.context_variables import ContextVariables
 from semantic_kernel.orchestration.sk_context import SKContext
 from semantic_kernel.orchestration.sk_function_base import SKFunctionBase
 from semantic_kernel.skill_definition.function_view import FunctionView
 from semantic_kernel.skill_definition.read_only_skill_collection_base import (
     ReadOnlySkillCollectionBase,
 )
+from semantic_kernel.utils.null_logger import NullLogger
 
 
 class Plan(SKFunctionBase):
     _state: ContextVariables
     _steps: List["Plan"]
     _function: SKFunctionBase
     _parameters: ContextVariables
@@ -108,42 +109,52 @@
         self._is_semantic = None
         self._function = None if function is None else function
         self._request_settings = None
 
         if function is not None:
             self.set_function(function)
 
+    @classmethod
+    def from_goal(cls, goal: str) -> "Plan":
+        return cls(description=goal, skill_name=cls.__name__)
+
+    @classmethod
+    def from_function(cls, function: SKFunctionBase) -> "Plan":
+        plan = cls()
+        plan.set_function(function)
+        return plan
+
     async def invoke_async(
         self,
         input: Optional[str] = None,
         context: Optional[SKContext] = None,
         settings: Optional[CompleteRequestSettings] = None,
         memory: Optional[SemanticTextMemoryBase] = None,
         logger: Optional[Logger] = None,
         # TODO: cancellation_token: CancellationToken,
     ) -> SKContext:
-        if input is not None:
+        if input is not None and input != "":
             self._state.update(input)
 
         if context is None:
             context = SKContext(
                 variables=self._state,
                 skill_collection=None,
                 memory=memory,
-                logger=logger,
+                logger=logger if logger is not None else NullLogger(),
             )
 
         if self._function is not None:
             result = await self._function.invoke_async(
                 context=context, settings=settings
             )
             if result.error_occurred:
                 result.log.error(
-                    msg="Something went wrong in plan step {0}.{1}:'{2}'".format(
-                        self._skill_name, self._name, context.last_error_description
+                    "Something went wrong in plan step {0}.{1}:'{2}'".format(
+                        self._skill_name, self._name, result.last_error_description
                     )
                 )
                 return result
             context.variables.update(result.result)
         else:
             # loop through steps until completion
             while self.has_next_step:
@@ -158,15 +169,15 @@
         self,
         input: Optional[str] = None,
         context: Optional[SKContext] = None,
         settings: Optional[CompleteRequestSettings] = None,
         memory: Optional[SemanticTextMemoryBase] = None,
         logger: Optional[Logger] = None,
     ) -> SKContext:
-        if input is not None:
+        if input is not None and input != "":
             self._state.update(input)
 
         if context is None:
             context = SKContext(
                 variables=self._state,
                 skill_collection=None,
                 memory=memory,
@@ -240,15 +251,15 @@
                 pass
         else:
             for step in plan.steps:
                 step = self.set_available_functions(step, context)
 
         return plan
 
-    def add_steps(self, steps: Optional[List[SKFunctionBase]]) -> None:
+    def add_steps(self, steps: Union[List["Plan"], List[SKFunctionBase]]) -> None:
         for step in steps:
             if type(step) is Plan:
                 self._steps.append(step)
             else:
                 new_step = Plan(
                     name=step.name,
                     skill_name=step.skill_name,
@@ -340,15 +351,15 @@
             result_string = self._state[Plan.DEFAULT_RESULT_KEY]
         else:
             result_string = str(self._state)
 
         context.variables.update(result_string)
 
         for item in self._steps[self._next_step_index - 1]._outputs:
-            if item in self._state:
+            if self._state.contains_key(item):
                 context.variables.set(item, self._state[item])
             else:
                 context.variables.set(item, result_string)
 
         return context
 
     def get_next_step_variables(
@@ -357,41 +368,43 @@
         # Priority for Input
         # - Parameters (expand from variables if needed)
         # - SKContext.Variables
         # - Plan.State
         # - Empty if sending to another plan
         # - Plan.Description
         input_string = ""
-        if step._parameters["input"] is not None:
-            input_string = self.expand_from_variables(
-                variables, step._parameters["input"]
-            )
-        elif variables["input"] is not None:
-            input_string = variables["input"]
-        elif self._state["input"] is not None:
-            input_string = self._state["input"]
+        step_input_exists, step_input_value = step._parameters.get("input")
+        variables_input_exists, variables_input_value = variables.get("input")
+        state_input_exists, state_input_value = self._state.get("input")
+        if step_input_exists and step_input_value != "":
+            input_string = self.expand_from_variables(variables, step_input_value)
+        elif variables_input_exists and variables_input_value != "":
+            input_string = variables_input_value
+        elif state_input_exists and state_input_value != "":
+            input_string = state_input_value
         elif len(step._steps) > 0:
             input_string = ""
-        elif self._description is not None:
+        elif self._description is not None and self._description != "":
             input_string = self._description
 
         step_variables = ContextVariables(input_string)
 
         # Priority for remaining stepVariables is:
         # - Function Parameters (pull from variables or state by a key value)
         # - Step Parameters (pull from variables or state by a key value)
+        # - All other variables. These are carried over in case the function wants access to the ambient content.
         function_params = step.describe()
         for param in function_params._parameters:
-            if param.name.lower == "input":
+            if param.name.lower() == variables._main_key.lower():
                 continue
-            if step_variables.contains_key(param.name):
+
+            if variables.contains_key(param.name):
                 step_variables.set(param.name, variables[param.name])
-            elif (
-                self._state.contains_key(param.name)
-                and self._state[param.name] is not None
+            elif self._state.contains_key(param.name) and (
+                self._state[param.name] is not None and self._state[param.name] != ""
             ):
                 step_variables.set(param.name, self._state[param.name])
 
         for param_var in step.parameters._variables:
             if step_variables.contains_key(param_var):
                 continue
 
@@ -401,22 +414,26 @@
             elif variables.contains_key(param_var):
                 step_variables.set(param_var, variables[param_var])
             elif self._state.contains_key(param_var):
                 step_variables.set(param_var, self._state[param_var])
             else:
                 step_variables.set(param_var, expanded_value)
 
+        for item in variables._variables:
+            if not step_variables.contains_key(item):
+                step_variables.set(item, variables[item])
+
         return step_variables
 
     def expand_from_variables(
         self, variables: ContextVariables, input_string: str
     ) -> str:
         result = input_string
         variables_regex = r"\$(?P<var>\w+)"
-        matches = re.findall(variables_regex, input_string)
+        matches = [m for m in re.finditer(variables_regex, input_string)]
         ordered_matches = sorted(
             matches, key=lambda m: len(m.group("var")), reverse=True
         )
 
         for match in ordered_matches:
             var_name = match.group("var")
             if variables.contains_key(var_name):
```

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/parameter_view.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/text/text_chunker.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/text/text_chunker.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/utils/settings.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.3.5.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.4.dev0/PKG-INFO` & `semantic_kernel-0.3.5.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.3.4.dev0
+Version: 0.3.5.dev0
 Summary: 
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

