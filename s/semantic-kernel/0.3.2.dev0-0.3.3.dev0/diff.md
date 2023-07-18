# Comparing `tmp/semantic_kernel-0.3.2.dev0.tar.gz` & `tmp/semantic_kernel-0.3.3.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "semantic_kernel-0.3.2.dev0.tar", max compression
+gzip compressed data, was "semantic_kernel-0.3.3.dev0.tar", max compression
```

## Comparing `semantic_kernel-0.3.2.dev0.tar` & `semantic_kernel-0.3.3.dev0.tar`

### file list

```diff
@@ -1,96 +1,105 @@
--rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.000000 semantic_kernel-0.3.2.dev0/pip/README.md
--rw-r--r--   0        0        0     1040 2023-07-10 20:42:43.199828 semantic_kernel-0.3.2.dev0/pyproject.toml
--rw-r--r--   0        0        0     1301 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/__init__.py
--rw-r--r--   0        0        0      719 2023-05-25 17:48:21.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/__init__.py
--rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/ai_exception.py
--rw-r--r--   0        0        0     1792 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
--rw-r--r--   0        0        0     1235 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
--rw-r--r--   0        0        0     1405 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
--rw-r--r--   0        0        0      282 2023-04-30 18:57:02.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
--rw-r--r--   0        0        0      352 2023-04-30 18:57:02.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
--rw-r--r--   0        0        0     6161 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
--rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
--rw-r--r--   0        0        0      892 2023-04-30 18:57:02.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
--rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
--rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
--rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
--rw-r--r--   0        0        0     8467 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
--rw-r--r--   0        0        0     5504 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
--rw-r--r--   0        0        0     2723 2023-05-15 18:12:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
--rw-r--r--   0        0        0     1616 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
--rw-r--r--   0        0        0      182 2023-05-18 17:32:52.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
--rw-r--r--   0        0        0    15268 2023-06-08 17:22:29.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
--rw-r--r--   0        0        0     4402 2023-06-08 17:22:29.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/chroma/utils.py
--rw-r--r--   0        0        0      190 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/pinecone/__init__.py
--rw-r--r--   0        0        0    14867 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
--rw-r--r--   0        0        0     1154 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/pinecone/utils.py
--rw-r--r--   0        0        0    11295 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
--rw-r--r--   0        0        0      691 2023-05-19 18:06:11.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/__init__.py
--rw-r--r--   0        0        0     2510 2023-05-15 18:12:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
--rw-r--r--   0        0        0     2082 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/file_io_skill.py
--rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/http_skill.py
--rw-r--r--   0        0        0     3171 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/math_skill.py
--rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/text_memory_skill.py
--rw-r--r--   0        0        0     2413 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/text_skill.py
--rw-r--r--   0        0        0     7860 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/time_skill.py
--rw-r--r--   0        0        0      629 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/wait_skill.py
--rw-r--r--   0        0        0    27810 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/kernel.py
--rw-r--r--   0        0        0     1626 2023-04-30 18:57:02.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/kernel_exception.py
--rw-r--r--   0        0        0      160 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/__init__.py
--rw-r--r--   0        0        0     2544 2023-06-08 17:22:29.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/memory_query_result.py
--rw-r--r--   0        0        0     3708 2023-06-08 17:22:29.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/memory_record.py
--rw-r--r--   0        0        0     2014 2023-05-19 23:02:13.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/memory_store_base.py
--rw-r--r--   0        0        0     1272 2023-06-08 17:22:29.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/null_memory.py
--rw-r--r--   0        0        0     6354 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/semantic_text_memory.py
--rw-r--r--   0        0        0     1298 2023-06-08 17:22:29.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/semantic_text_memory_base.py
--rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/memory/volatile_memory_store.py
--rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/context_variables.py
--rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/delegate_handlers.py
--rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/delegate_inference.py
--rw-r--r--   0        0        0      638 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/delegate_types.py
--rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/sk_context.py
--rw-r--r--   0        0        0    16088 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/sk_function.py
--rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/sk_function_base.py
--rw-r--r--   0        0        0      158 2023-05-08 23:38:10.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/planning/__init__.py
--rw-r--r--   0        0        0     7538 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/planning/basic_planner.py
--rw-r--r--   0        0        0      396 2023-05-08 23:26:29.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/planning/plan.py
--rw-r--r--   0        0        0      932 2023-05-19 23:02:13.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/reliability/pass_through_without_retry.py
--rw-r--r--   0        0        0      694 2023-06-05 21:39:19.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/reliability/retry_mechanism_base.py
--rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
--rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/prompt_template.py
--rw-r--r--   0        0        0      506 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
--rw-r--r--   0        0        0     4525 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
--rw-r--r--   0        0        0      671 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
--rw-r--r--   0        0        0      322 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/__init__.py
--rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/function_view.py
--rw-r--r--   0        0        0     2199 2023-06-12 17:06:53.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/functions_view.py
--rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/parameter_view.py
--rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
--rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
--rw-r--r--   0        0        0      858 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
--rw-r--r--   0        0        0      837 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
--rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/skill_collection.py
--rw-r--r--   0        0        0      803 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/skill_collection_base.py
--rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/README.md
--rw-r--r--   0        0        0      830 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/block.py
--rw-r--r--   0        0        0      228 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/block_types.py
--rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/code_block.py
--rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
--rw-r--r--   0        0        0      276 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/symbols.py
--rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/text_block.py
--rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/val_block.py
--rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/var_block.py
--rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/code_tokenizer.py
--rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/prompt_template_engine.py
--rw-r--r--   0        0        0      532 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
--rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
--rw-r--r--   0        0        0      596 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
--rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/template_tokenizer.py
--rw-r--r--   0        0        0      473 2023-04-30 18:57:03.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/text/__init__.py
--rw-r--r--   0        0        0      667 2023-04-30 18:57:03.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/text/function_extension.py
--rw-r--r--   0        0        0     8440 2023-07-10 20:40:59.227169 semantic_kernel-0.3.2.dev0/semantic_kernel/text/text_chunker.py
--rw-r--r--   0        0        0      403 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/utils/null_logger.py
--rw-r--r--   0        0        0     2574 2023-07-06 22:13:35.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/utils/settings.py
--rw-r--r--   0        0        0      221 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/utils/static_property.py
--rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.000000 semantic_kernel-0.3.2.dev0/semantic_kernel/utils/validation.py
--rw-r--r--   0        0        0     1843 1970-01-01 00:00:00.000000 semantic_kernel-0.3.2.dev0/PKG-INFO
+-rw-r--r--   0        0        0     1186 2023-05-08 23:38:10.000000 semantic_kernel-0.3.3.dev0/pip/README.md
+-rw-r--r--   0        0        0     1322 2023-07-18 01:08:06.924816 semantic_kernel-0.3.3.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1375 2023-07-12 19:14:40.912511 semantic_kernel-0.3.3.dev0/semantic_kernel/__init__.py
+-rw-r--r--   0        0        0      719 2023-05-25 17:48:21.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/__init__.py
+-rw-r--r--   0        0        0     1647 2023-04-30 18:57:02.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/ai_exception.py
+-rw-r--r--   0        0        0     1792 2023-06-12 17:06:53.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py
+-rw-r--r--   0        0        0     1321 2023-07-14 16:57:26.312407 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/chat_request_settings.py
+-rw-r--r--   0        0        0     1484 2023-07-14 16:57:26.312942 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/complete_request_settings.py
+-rw-r--r--   0        0        0      282 2023-04-30 18:57:02.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/embeddings/embedding_generator_base.py
+-rw-r--r--   0        0        0      352 2023-04-30 18:57:02.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/hugging_face/__init__.py
+-rw-r--r--   0        0        0     6161 2023-06-12 17:06:53.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py
+-rw-r--r--   0        0        0     2317 2023-05-08 23:38:10.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py
+-rw-r--r--   0        0        0      892 2023-04-30 18:57:02.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py
+-rw-r--r--   0        0        0     2615 2023-05-15 18:12:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py
+-rw-r--r--   0        0        0     2607 2023-05-15 18:12:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py
+-rw-r--r--   0        0        0     2602 2023-05-15 18:12:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py
+-rw-r--r--   0        0        0     8903 2023-07-16 00:59:27.692753 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py
+-rw-r--r--   0        0        0     5788 2023-07-16 00:59:27.693316 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py
+-rw-r--r--   0        0        0     2723 2023-05-15 18:12:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py
+-rw-r--r--   0        0        0     1616 2023-06-12 17:06:53.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py
+-rw-r--r--   0        0        0      204 2023-07-16 07:20:48.222581 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/azure_search/__init__.py
+-rw-r--r--   0        0        0    16254 2023-07-16 07:20:48.223592 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/azure_search/azure_search_memory_store.py
+-rw-r--r--   0        0        0     8040 2023-07-16 07:20:48.224597 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/azure_search/utils.py
+-rw-r--r--   0        0        0      182 2023-05-18 17:32:52.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/chroma/__init__.py
+-rw-r--r--   0        0        0    15273 2023-07-16 00:58:37.999718 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py
+-rw-r--r--   0        0        0     4426 2023-07-16 00:58:38.000353 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/chroma/utils.py
+-rw-r--r--   0        0        0      190 2023-07-06 22:13:35.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/pinecone/__init__.py
+-rw-r--r--   0        0        0    14928 2023-07-12 19:14:40.913001 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py
+-rw-r--r--   0        0        0     1154 2023-07-06 22:13:35.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/pinecone/utils.py
+-rw-r--r--   0        0        0      190 2023-07-12 19:14:40.913420 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/postgres/__init__.py
+-rw-r--r--   0        0        0    20480 2023-07-12 19:14:40.913726 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/postgres/postgres_memory_store.py
+-rw-r--r--   0        0        0    11295 2023-06-12 17:06:53.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py
+-rw-r--r--   0        0        0      111 2023-07-17 21:15:24.598216 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/search_engine/__init__.py
+-rw-r--r--   0        0        0     2842 2023-07-17 21:15:24.598630 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/search_engine/bing_connector.py
+-rw-r--r--   0        0        0      173 2023-07-17 21:15:24.599030 semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/search_engine/connector.py
+-rw-r--r--   0        0        0      804 2023-07-17 21:15:24.599960 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/__init__.py
+-rw-r--r--   0        0        0     2510 2023-05-15 18:12:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/conversation_summary_skill.py
+-rw-r--r--   0        0        0     2131 2023-07-16 00:59:27.693756 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/file_io_skill.py
+-rw-r--r--   0        0        0     3754 2023-04-22 04:06:40.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/http_skill.py
+-rw-r--r--   0        0        0     3171 2023-07-06 22:13:35.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/math_skill.py
+-rw-r--r--   0        0        0     4641 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/text_memory_skill.py
+-rw-r--r--   0        0        0     2462 2023-07-16 00:59:27.694343 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/text_skill.py
+-rw-r--r--   0        0        0     7909 2023-07-16 00:59:27.694865 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/time_skill.py
+-rw-r--r--   0        0        0      678 2023-07-16 00:59:27.695359 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/wait_skill.py
+-rw-r--r--   0        0        0     1950 2023-07-17 21:15:24.600357 semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/web_search_engine_skill.py
+-rw-r--r--   0        0        0    32289 2023-07-17 21:15:24.601483 semantic_kernel-0.3.3.dev0/semantic_kernel/kernel.py
+-rw-r--r--   0        0        0     1726 2023-07-16 00:59:27.695868 semantic_kernel-0.3.3.dev0/semantic_kernel/kernel_exception.py
+-rw-r--r--   0        0        0      160 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/__init__.py
+-rw-r--r--   0        0        0     2544 2023-06-08 17:22:29.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/memory_query_result.py
+-rw-r--r--   0        0        0     3912 2023-07-12 19:14:40.914195 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/memory_record.py
+-rw-r--r--   0        0        0     2014 2023-05-19 23:02:13.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/memory_store_base.py
+-rw-r--r--   0        0        0     1272 2023-06-08 17:22:29.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/null_memory.py
+-rw-r--r--   0        0        0     6354 2023-07-16 00:42:59.250269 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/semantic_text_memory.py
+-rw-r--r--   0        0        0     1298 2023-06-08 17:22:29.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/semantic_text_memory_base.py
+-rw-r--r--   0        0        0    12032 2023-05-15 18:12:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/memory/volatile_memory_store.py
+-rw-r--r--   0        0        0     2361 2023-04-22 04:06:40.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/context_variables.py
+-rw-r--r--   0        0        0     5079 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/delegate_handlers.py
+-rw-r--r--   0        0        0     9005 2023-05-19 23:02:13.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/delegate_inference.py
+-rw-r--r--   0        0        0      638 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/delegate_types.py
+-rw-r--r--   0        0        0     7514 2023-04-14 00:52:05.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/sk_context.py
+-rw-r--r--   0        0        0    16088 2023-07-06 22:13:35.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/sk_function.py
+-rw-r--r--   0        0        0     6158 2023-04-30 18:57:02.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/sk_function_base.py
+-rw-r--r--   0        0        0      158 2023-05-08 23:38:10.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/planning/__init__.py
+-rw-r--r--   0        0        0     7538 2023-07-06 22:13:35.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/planning/basic_planner.py
+-rw-r--r--   0        0        0    15624 2023-07-16 00:59:27.696327 semantic_kernel-0.3.3.dev0/semantic_kernel/planning/plan.py
+-rw-r--r--   0        0        0      932 2023-05-19 23:02:13.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/reliability/pass_through_without_retry.py
+-rw-r--r--   0        0        0      694 2023-06-05 21:39:19.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/reliability/retry_mechanism_base.py
+-rw-r--r--   0        0        0     2101 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py
+-rw-r--r--   0        0        0     2332 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/prompt_template.py
+-rw-r--r--   0        0        0      506 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/prompt_template_base.py
+-rw-r--r--   0        0        0     4525 2023-06-12 17:06:53.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/prompt_template_config.py
+-rw-r--r--   0        0        0      671 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/semantic_function_config.py
+-rw-r--r--   0        0        0      322 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/__init__.py
+-rw-r--r--   0        0        0     2053 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/function_view.py
+-rw-r--r--   0        0        0     2199 2023-06-12 17:06:53.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/functions_view.py
+-rw-r--r--   0        0        0     1026 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/parameter_view.py
+-rw-r--r--   0        0        0     2104 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py
+-rw-r--r--   0        0        0     1345 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py
+-rw-r--r--   0        0        0      858 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py
+-rw-r--r--   0        0        0      837 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/sk_function_decorator.py
+-rw-r--r--   0        0        0     6056 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/skill_collection.py
+-rw-r--r--   0        0        0      803 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/skill_collection_base.py
+-rw-r--r--   0        0        0     1115 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/README.md
+-rw-r--r--   0        0        0      830 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/block.py
+-rw-r--r--   0        0        0      228 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/block_types.py
+-rw-r--r--   0        0        0     4577 2023-04-30 18:57:03.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/code_block.py
+-rw-r--r--   0        0        0     2653 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/function_id_block.py
+-rw-r--r--   0        0        0      276 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/symbols.py
+-rw-r--r--   0        0        0     1534 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/text_block.py
+-rw-r--r--   0        0        0     2274 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/val_block.py
+-rw-r--r--   0        0        0     2517 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/var_block.py
+-rw-r--r--   0        0        0     6535 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/code_tokenizer.py
+-rw-r--r--   0        0        0     6051 2023-04-14 00:51:57.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/prompt_template_engine.py
+-rw-r--r--   0        0        0      532 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/protocols/code_renderer.py
+-rw-r--r--   0        0        0     3043 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py
+-rw-r--r--   0        0        0      596 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/protocols/text_renderer.py
+-rw-r--r--   0        0        0     7637 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/template_tokenizer.py
+-rw-r--r--   0        0        0      473 2023-04-30 18:57:03.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/text/__init__.py
+-rw-r--r--   0        0        0      667 2023-04-30 18:57:03.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/text/function_extension.py
+-rw-r--r--   0        0        0     8568 2023-07-16 00:58:38.006510 semantic_kernel-0.3.3.dev0/semantic_kernel/text/text_chunker.py
+-rw-r--r--   0        0        0      403 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/utils/null_logger.py
+-rw-r--r--   0        0        0     2694 2023-07-12 19:14:40.915313 semantic_kernel-0.3.3.dev0/semantic_kernel/utils/settings.py
+-rw-r--r--   0        0        0      221 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/utils/static_property.py
+-rw-r--r--   0        0        0     2198 2023-04-13 23:12:46.000000 semantic_kernel-0.3.3.dev0/semantic_kernel/utils/validation.py
+-rw-r--r--   0        0        0     1843 1970-01-01 00:00:00.000000 semantic_kernel-0.3.3.dev0/PKG-INFO
```

### Comparing `semantic_kernel-0.3.2.dev0/pip/README.md` & `semantic_kernel-0.3.3.dev0/pip/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/pyproject.toml` & `semantic_kernel-0.3.3.dev0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "semantic-kernel"
-version = "0.3.2.dev"
+version = "0.3.3.dev"
 description = ""
 authors = ["Microsoft <SK-Support@microsoft.com>"]
 readme = "pip/README.md"
 packages = [{include = "semantic_kernel"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -24,23 +24,32 @@
 
 [tool.poetry.group.hugging_face.dependencies]
 transformers = "^4.28.1"
 sentence-transformers = "^2.2.2"
 torch = "2.0.0"
 
 [tool.poetry.group.chromadb.dependencies]
-chromadb = "^0.3.23"
-
+chromadb = "^0.3.29"
 
 [tool.poetry.group.weaviate.dependencies]
 weaviate-client = "^3.18.0"
 
 [tool.poetry.group.pinecone.dependencies]
 pinecone-client = "^2.2.2"
 
+[tool.poetry.group.postgres.dependencies]
+psycopg-pool = "^3.1.7"
+psycopg = "^3.1.9"
+psycopg-binary = "^3.1.9"
+
+[tool.poetry.group.azure_search.dependencies]
+azure-search-documents = {version = "11.4.0b6", allow-prereleases = true}
+azure-core = "^1.28.0"
+azure-identity = "^1.13.0"
+
 [tool.isort]
 profile = "black"
 
 [tool.ruff]
 select = ["E", "F", "I"]
 line-length = 120
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/__init__.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,21 +14,23 @@
     SemanticFunctionConfig,
 )
 from semantic_kernel.utils.null_logger import NullLogger
 from semantic_kernel.utils.settings import (
     azure_openai_settings_from_dot_env,
     openai_settings_from_dot_env,
     pinecone_settings_from_dot_env,
+    postgres_settings_from_dot_env,
 )
 
 __all__ = [
     "Kernel",
     "NullLogger",
     "openai_settings_from_dot_env",
     "azure_openai_settings_from_dot_env",
+    "postgres_settings_from_dot_env",
     "pinecone_settings_from_dot_env",
     "PromptTemplateConfig",
     "PromptTemplate",
     "ChatPromptTemplate",
     "SemanticFunctionConfig",
     "ContextVariables",
     "SKFunctionBase",
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/__init__.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/ai_exception.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/ai_exception.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/chat_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/chat_request_settings.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/complete_request_settings.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,37 +1,41 @@
 # Copyright (c) Microsoft. All rights reserved.
 
-from dataclasses import dataclass
-from typing import TYPE_CHECKING
+from dataclasses import dataclass, field
+from typing import TYPE_CHECKING, Dict, List
 
 if TYPE_CHECKING:
     from semantic_kernel.semantic_functions.prompt_template_config import (
         PromptTemplateConfig,
     )
 
 
 @dataclass
-class ChatRequestSettings:
+class CompleteRequestSettings:
     temperature: float = 0.0
     top_p: float = 1.0
     presence_penalty: float = 0.0
     frequency_penalty: float = 0.0
-    number_of_responses: int = 1
     max_tokens: int = 256
+    stop_sequences: List[str] = field(default_factory=list)
+    number_of_responses: int = 1
+    logprobs: int = 0
+    token_selection_biases: Dict[int, int] = field(default_factory=dict)
 
     def update_from_completion_config(
         self, completion_config: "PromptTemplateConfig.CompletionConfig"
     ):
         self.temperature = completion_config.temperature
         self.top_p = completion_config.top_p
         self.presence_penalty = completion_config.presence_penalty
         self.frequency_penalty = completion_config.frequency_penalty
-        self.number_of_responses = completion_config.number_of_responses
         self.max_tokens = completion_config.max_tokens
+        self.stop_sequences = completion_config.stop_sequences
+        self.number_of_responses = completion_config.number_of_responses
 
     @staticmethod
     def from_completion_config(
         completion_config: "PromptTemplateConfig.CompletionConfig",
-    ) -> "ChatRequestSettings":
-        settings = ChatRequestSettings()
+    ) -> "CompleteRequestSettings":
+        settings = CompleteRequestSettings()
         settings.update_from_completion_config(completion_config)
         return settings
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/complete_request_settings.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/chat_request_settings.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,38 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 from dataclasses import dataclass, field
-from typing import TYPE_CHECKING, List
+from typing import TYPE_CHECKING, Dict
 
 if TYPE_CHECKING:
     from semantic_kernel.semantic_functions.prompt_template_config import (
         PromptTemplateConfig,
     )
 
 
 @dataclass
-class CompleteRequestSettings:
+class ChatRequestSettings:
     temperature: float = 0.0
     top_p: float = 1.0
     presence_penalty: float = 0.0
     frequency_penalty: float = 0.0
-    max_tokens: int = 256
-    stop_sequences: List[str] = field(default_factory=list)
     number_of_responses: int = 1
-    logprobs: int = 0
+    max_tokens: int = 256
+    token_selection_biases: Dict[int, int] = field(default_factory=dict)
 
     def update_from_completion_config(
         self, completion_config: "PromptTemplateConfig.CompletionConfig"
     ):
         self.temperature = completion_config.temperature
         self.top_p = completion_config.top_p
         self.presence_penalty = completion_config.presence_penalty
         self.frequency_penalty = completion_config.frequency_penalty
-        self.max_tokens = completion_config.max_tokens
-        self.stop_sequences = completion_config.stop_sequences
         self.number_of_responses = completion_config.number_of_responses
+        self.max_tokens = completion_config.max_tokens
 
     @staticmethod
     def from_completion_config(
         completion_config: "PromptTemplateConfig.CompletionConfig",
-    ) -> "CompleteRequestSettings":
-        settings = CompleteRequestSettings()
+    ) -> "ChatRequestSettings":
+        settings = ChatRequestSettings()
         settings.update_from_completion_config(completion_config)
         return settings
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/hugging_face/services/hf_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/__init__.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_chat_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_completion.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/azure_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_chat_completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -104,14 +104,15 @@
         chat_settings = ChatRequestSettings(
             temperature=request_settings.temperature,
             top_p=request_settings.top_p,
             presence_penalty=request_settings.presence_penalty,
             frequency_penalty=request_settings.frequency_penalty,
             max_tokens=request_settings.max_tokens,
             number_of_responses=request_settings.number_of_responses,
+            token_selection_biases=request_settings.token_selection_biases,
         )
         response = await self._send_chat_request(
             prompt_to_message, chat_settings, False
         )
 
         if len(response.choices) == 1:
             return response.choices[0].message.content
@@ -125,14 +126,15 @@
         chat_settings = ChatRequestSettings(
             temperature=request_settings.temperature,
             top_p=request_settings.top_p,
             presence_penalty=request_settings.presence_penalty,
             frequency_penalty=request_settings.frequency_penalty,
             max_tokens=request_settings.max_tokens,
             number_of_responses=request_settings.number_of_responses,
+            token_selection_biases=request_settings.token_selection_biases,
         )
         response = await self._send_chat_request(prompt_to_message, chat_settings, True)
 
         # parse the completion text(s) and yield them
         async for chunk in response:
             text, index = _parse_choices(chunk)
             # if multiple responses are requested, keep track of them
@@ -204,14 +206,20 @@
                 temperature=request_settings.temperature,
                 top_p=request_settings.top_p,
                 presence_penalty=request_settings.presence_penalty,
                 frequency_penalty=request_settings.frequency_penalty,
                 max_tokens=request_settings.max_tokens,
                 n=request_settings.number_of_responses,
                 stream=stream,
+                logit_bias=(
+                    request_settings.token_selection_biases
+                    if request_settings.token_selection_biases is not None
+                    and len(request_settings.token_selection_biases) > 0
+                    else {}
+                ),
             )
         except Exception as ex:
             raise AIException(
                 AIException.ErrorCodes.ServiceError,
                 "OpenAI service failed to complete the chat",
                 ex,
             )
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_completion.py`

 * *Files 7% similar despite different names*

```diff
@@ -138,14 +138,20 @@
                 n=request_settings.number_of_responses,
                 stop=(
                     request_settings.stop_sequences
                     if request_settings.stop_sequences is not None
                     and len(request_settings.stop_sequences) > 0
                     else None
                 ),
+                logit_bias=(
+                    request_settings.token_selection_biases
+                    if request_settings.token_selection_biases is not None
+                    and len(request_settings.token_selection_biases) > 0
+                    else {}
+                ),
             )
         except Exception as ex:
             raise AIException(
                 AIException.ErrorCodes.ServiceError,
                 "OpenAI service failed to complete the prompt",
                 ex,
             )
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/open_ai/services/open_ai_text_embedding.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/ai/text_completion_client_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/chroma/chroma_memory_store.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,15 +157,15 @@
         collection = await self.get_collection_async(collection_name)
         if collection is None:
             raise Exception(f"Collection '{collection_name}' does not exist")
 
         record._key = record._id
         metadata = {
             "timestamp": record._timestamp or "",
-            "is_reference": record._is_reference,
+            "is_reference": str(record._is_reference),
             "external_source_name": record._external_source_name or "",
             "description": record._description or "",
             "additional_metadata": record._additional_metadata or "",
             "id": record._id or "",
         }
 
         collection.add(
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/chroma/utils.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/chroma/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     except IndexError:
         return []
 
     if with_embedding:
         memory_records = [
             (
                 MemoryRecord(
-                    is_reference=metadata["is_reference"],
+                    is_reference=(metadata["is_reference"] == "True"),
                     external_source_name=metadata["external_source_name"],
                     id=metadata["id"],
                     description=metadata["description"],
                     text=document,
                     embedding=embedding,
                     additional_metadata=metadata["additional_metadata"],
                     key=id,
@@ -58,15 +58,15 @@
                 results["metadatas"][0],
             )
         ]
     else:
         memory_records = [
             (
                 MemoryRecord(
-                    is_reference=metadata["is_reference"],
+                    is_reference=(metadata["is_reference"] == "True"),
                     external_source_name=metadata["external_source_name"],
                     id=metadata["id"],
                     description=metadata["description"],
                     text=document,
                     embedding=None,
                     additional_metadata=metadata["additional_metadata"],
                     key=id,
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/pinecone/pinecone_memory_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 MAX_QUERY_WITHOUT_METADATA_BATCH_SIZE = 10000
 MAX_QUERY_WITH_METADATA_BATCH_SIZE = 1000
 MAX_FETCH_BATCH_SIZE = 1000
 MAX_DELETE_BATCH_SIZE = 1000
 
 
 class PineconeMemoryStore(MemoryStoreBase):
+    """A memory store that uses Pinecone as the backend."""
+
     _logger: Logger
     _pinecone_api_key: str
     _pinecone_environment: str
     _default_dimensionality: int
 
     def __init__(
         self,
@@ -38,16 +40,16 @@
         logger: Optional[Logger] = None,
     ) -> None:
         """Initializes a new instance of the PineconeMemoryStore class.
 
         Arguments:
             pinecone_api_key {str} -- The Pinecone API key.
             pinecone_environment {str} -- The Pinecone environment.
-            logger {Optional[Logger]} -- The logger to use. (default: {None})
             default_dimensionality {int} -- The default dimensionality to use for new collections.
+            logger {Optional[Logger]} -- The logger to use. (default: {None})
         """
         if default_dimensionality > MAX_DIMENSIONALITY:
             raise ValueError(
                 f"Dimensionality of {default_dimensionality} exceeds "
                 + f"the maximum allowed value of {MAX_DIMENSIONALITY}."
             )
         self._pinecone_api_key = api_key
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/pinecone/utils.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/pinecone/utils.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/connectors/memory/weaviate/weaviate_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/__init__.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,17 +5,19 @@
 )
 from semantic_kernel.core_skills.file_io_skill import FileIOSkill
 from semantic_kernel.core_skills.http_skill import HttpSkill
 from semantic_kernel.core_skills.math_skill import MathSkill
 from semantic_kernel.core_skills.text_memory_skill import TextMemorySkill
 from semantic_kernel.core_skills.text_skill import TextSkill
 from semantic_kernel.core_skills.time_skill import TimeSkill
+from semantic_kernel.core_skills.web_search_engine_skill import WebSearchEngineSkill
 
 __all__ = [
     "TextMemorySkill",
     "TextSkill",
     "FileIOSkill",
     "TimeSkill",
     "HttpSkill",
     "ConversationSummarySkill",
     "MathSkill",
+    "WebSearchEngineSkill",
 ]
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/conversation_summary_skill.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/conversation_summary_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/file_io_skill.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/file_io_skill.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright (c) Microsoft. All rights reserved.
+
 import os
 
 import aiofiles
 
 from semantic_kernel.orchestration.sk_context import SKContext
 from semantic_kernel.skill_definition import sk_function, sk_function_context_parameter
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/http_skill.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/http_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/math_skill.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/math_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/text_memory_skill.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/text_memory_skill.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/text_skill.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/text_skill.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright (c) Microsoft. All rights reserved.
+
 from semantic_kernel.skill_definition import sk_function
 
 
 class TextSkill:
     """
     TextSkill provides a set of functions to manipulate strings.
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/time_skill.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/time_skill.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright (c) Microsoft. All rights reserved.
+
 import datetime
 
 from semantic_kernel.skill_definition import sk_function
 
 
 class TimeSkill:
     """
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/core_skills/wait_skill.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/core_skills/wait_skill.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# Copyright (c) Microsoft. All rights reserved.
+
 import asyncio
 
 from semantic_kernel.skill_definition import sk_function
 
 
 class WaitSkill:
     """
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/kernel.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/kernel.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (c) Microsoft. All rights reserved.
 
 import glob
 import importlib
 import inspect
 import os
 from logging import Logger
-from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, Union
+from typing import Any, Callable, Dict, List, Optional, Type, TypeVar, Union, cast
 from uuid import uuid4
 
 from semantic_kernel.connectors.ai.ai_exception import AIException
 from semantic_kernel.connectors.ai.chat_completion_client_base import (
     ChatCompletionClientBase,
 )
 from semantic_kernel.connectors.ai.chat_request_settings import ChatRequestSettings
@@ -31,14 +31,15 @@
 from semantic_kernel.orchestration.sk_context import SKContext
 from semantic_kernel.orchestration.sk_function import SKFunction
 from semantic_kernel.orchestration.sk_function_base import SKFunctionBase
 from semantic_kernel.reliability.pass_through_without_retry import (
     PassThroughWithoutRetry,
 )
 from semantic_kernel.reliability.retry_mechanism_base import RetryMechanismBase
+from semantic_kernel.semantic_functions.chat_prompt_template import ChatPromptTemplate
 from semantic_kernel.semantic_functions.prompt_template import PromptTemplate
 from semantic_kernel.semantic_functions.prompt_template_config import (
     PromptTemplateConfig,
 )
 from semantic_kernel.semantic_functions.semantic_function_config import (
     SemanticFunctionConfig,
 )
@@ -129,14 +130,118 @@
         function = self._create_semantic_function(
             skill_name, function_name, function_config
         )
         self._skill_collection.add_semantic_function(function)
 
         return function
 
+    async def run_stream_async(
+        self,
+        *functions: Any,
+        input_context: Optional[SKContext] = None,
+        input_vars: Optional[ContextVariables] = None,
+        input_str: Optional[str] = None,
+    ):
+        if len(functions) > 1:
+            pipeline_functions = functions[:-1]
+            stream_function = functions[-1]
+
+            # run pipeline functions
+            context = await self.run_async(
+                pipeline_functions, input_context, input_vars, input_str
+            )
+
+        elif len(functions) == 1:
+            stream_function = functions[0]
+            # if the user passed in a context, prioritize it, but merge with any other inputs
+            if input_context is not None:
+                context = input_context
+                if input_vars is not None:
+                    context._variables = input_vars.merge_or_overwrite(
+                        new_vars=context._variables, overwrite=False
+                    )
+
+                if input_str is not None:
+                    context._variables = ContextVariables(input_str).merge_or_overwrite(
+                        new_vars=context._variables, overwrite=False
+                    )
+
+            # if the user did not pass in a context, prioritize an input string,
+            # and merge that with input context variables
+            else:
+                if input_str is not None and input_vars is None:
+                    variables = ContextVariables(input_str)
+                elif input_str is None and input_vars is not None:
+                    variables = input_vars
+                elif input_str is not None and input_vars is not None:
+                    variables = ContextVariables(input_str)
+                    variables = variables.merge_or_overwrite(
+                        new_vars=input_vars, overwrite=False
+                    )
+                else:
+                    variables = ContextVariables()
+                context = SKContext(
+                    variables,
+                    self._memory,
+                    self._skill_collection.read_only_skill_collection,
+                    self._log,
+                )
+        else:
+            raise ValueError("No functions passed to run")
+
+        try:
+            client: ChatCompletionClientBase | TextCompletionClientBase
+            client = stream_function._ai_service
+
+            # Get the closure variables from function for finding function_config
+            closure_vars = stream_function._function.__closure__
+            for var in closure_vars:
+                if isinstance(var.cell_contents, SemanticFunctionConfig):
+                    function_config = var.cell_contents
+                    break
+
+            if function_config.has_chat_prompt:
+                as_chat_prompt = cast(
+                    ChatPromptTemplate, function_config.prompt_template
+                )
+
+                # Similar to non-chat, render prompt (which renders to a
+                # list of <role, content> messages)
+                completion = ""
+                messages = await as_chat_prompt.render_messages_async(context)
+                async for steam_message in client.complete_chat_stream_async(
+                    messages, stream_function._chat_request_settings
+                ):
+                    completion += steam_message
+                    yield steam_message
+
+                # Add the last message from the rendered chat prompt
+                # (which will be the user message) and the response
+                # from the model (the assistant message)
+                _, content = messages[-1]
+                as_chat_prompt.add_user_message(content)
+                as_chat_prompt.add_assistant_message(completion)
+
+                # Update context
+                context.variables.update(completion)
+
+            else:
+                completion = ""
+                prompt = await function_config.prompt_template.render_async(context)
+                async for stream_message in client.complete_stream_async(
+                    prompt, stream_function._ai_request_settings
+                ):
+                    completion += stream_message
+                    yield stream_message
+                context.variables.update(completion)
+
+        except Exception as e:
+            # TODO: "critical exceptions"
+            context.fail(str(e), e)
+
     async def run_async(
         self,
         *functions: Any,
         input_context: Optional[SKContext] = None,
         input_vars: Optional[ContextVariables] = None,
         input_str: Optional[str] = None,
     ) -> SKContext:
@@ -149,15 +254,16 @@
                 )
 
             if input_str is not None:
                 context._variables = ContextVariables(input_str).merge_or_overwrite(
                     new_vars=context._variables, overwrite=False
                 )
 
-        # if the user did not pass in a context, prioritize an input string, and merge that with input context variables
+        # if the user did not pass in a context, prioritize an input string,
+        # and merge that with input context variables
         else:
             if input_str is not None and input_vars is None:
                 variables = ContextVariables(input_str)
             elif input_str is None and input_vars is not None:
                 variables = input_vars
             elif input_str is not None and input_vars is not None:
                 variables = ContextVariables(input_str)
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/kernel_exception.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/kernel_exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,16 +20,18 @@
         InvalidFunctionType = 4
         # Invalid service configuration.
         InvalidServiceConfiguration = 5
         # Service not found.
         ServiceNotFound = 6
         # Skill collection not set.
         SkillCollectionNotSet = 7
+        # Represents an error that occurs when invoking a function.
+        FunctionInvokeError = 8
         # Ambiguous implementation.
-        AmbiguousImplementation = 8
+        AmbiguousImplementation = 9
 
     # The error code.
     _error_code: ErrorCodes
 
     def __init__(
         self,
         error_code: ErrorCodes,
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/memory/memory_query_result.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/memory/memory_query_result.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/memory/memory_record.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/memory/memory_record.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 # Copyright (c) Microsoft. All rights reserved.
 
+from datetime import datetime
 from typing import Optional
 
 from numpy import ndarray
 
 
 class MemoryRecord:
     _key: str
-    _timestamp: str
+    _timestamp: Optional[datetime]
     _is_reference: bool
     _external_source_name: Optional[str]
     _id: str
     _description: Optional[str]
     _text: Optional[str]
     _additional_metadata: Optional[str]
     _embedding: ndarray
@@ -22,15 +23,15 @@
         external_source_name: Optional[str],
         id: str,
         description: Optional[str],
         text: Optional[str],
         additional_metadata: Optional[str],
         embedding: Optional[ndarray],
         key: Optional[str] = None,
-        timestamp: Optional[str] = None,
+        timestamp: Optional[datetime] = None,
     ) -> None:
         """Initialize a new instance of MemoryRecord.
 
         Arguments:
             is_reference {bool} -- Whether the record is a reference record.
             external_source_name {Optional[str]} -- The name of the external source.
             id {str} -- A unique for the record.
@@ -89,29 +90,32 @@
     @staticmethod
     def local_record(
         id: str,
         text: str,
         description: Optional[str],
         additional_metadata: Optional[str],
         embedding: ndarray,
+        timestamp: Optional[datetime] = None,
     ) -> "MemoryRecord":
         """Create a local record.
 
         Arguments:
             id {str} -- A unique for the record.
             text {str} -- The text of the record.
             description {Optional[str]} -- The description of the record.
             additional_metadata {Optional[str]} -- Custom metadata for the record.
             embedding {ndarray} -- The embedding of the record.
+            timestamp {Optional[datetime]} -- The timestamp of the record.
 
         Returns:
             MemoryRecord -- The local record.
         """
         return MemoryRecord(
             is_reference=False,
             external_source_name=None,
             id=id,
             description=description,
             text=text,
             additional_metadata=additional_metadata,
+            timestamp=timestamp,
             embedding=embedding,
         )
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/memory/memory_store_base.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/memory/memory_store_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/memory/null_memory.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/memory/null_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/memory/semantic_text_memory.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/memory/semantic_text_memory.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/memory/semantic_text_memory_base.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/memory/semantic_text_memory_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/memory/volatile_memory_store.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/memory/volatile_memory_store.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/context_variables.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/context_variables.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/delegate_handlers.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/delegate_handlers.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/delegate_inference.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/delegate_inference.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/delegate_types.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/delegate_types.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/sk_context.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/sk_context.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/sk_function.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/sk_function.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/orchestration/sk_function_base.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/orchestration/sk_function_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/planning/basic_planner.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/planning/basic_planner.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/reliability/pass_through_without_retry.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/reliability/pass_through_without_retry.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/reliability/retry_mechanism_base.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/reliability/retry_mechanism_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/chat_prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/prompt_template.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/prompt_template.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/prompt_template_config.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/prompt_template_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/semantic_functions/semantic_function_config.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/semantic_functions/semantic_function_config.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/function_view.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/function_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/functions_view.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/functions_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/parameter_view.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/parameter_view.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/read_only_skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/sk_function_context_parameter_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/sk_function_decorator.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/sk_function_decorator.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/skill_collection.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/skill_collection.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/skill_definition/skill_collection_base.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/skill_definition/skill_collection_base.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/README.md` & `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/README.md`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/block.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/code_block.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/code_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/function_id_block.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/function_id_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/text_block.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/text_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/val_block.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/val_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/blocks/var_block.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/blocks/var_block.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/code_tokenizer.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/code_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/prompt_template_engine.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/prompt_template_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/protocols/code_renderer.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/protocols/code_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/protocols/prompt_templating_engine.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/protocols/text_renderer.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/protocols/text_renderer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/template_engine/template_tokenizer.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/template_engine/template_tokenizer.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/text/function_extension.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/text/function_extension.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/text/text_chunker.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/text/text_chunker.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,15 +120,15 @@
 
     return _split_text_paragraph(
         text=split_lines, max_tokens=max_tokens, token_counter=token_counter
     )
 
 
 def _split_text_paragraph(
-    text: List[str], max_tokens: int, token_counter: Callable
+    text: List[str], max_tokens: int, token_counter: Callable = _token_counter
 ) -> List[str]:
     """
     Split text into paragraphs.
     """
     if not text:
         return []
 
@@ -172,15 +172,18 @@
                 paragraphs[-2] = new_sec_last_para.strip()
                 paragraphs.pop()
 
     return paragraphs
 
 
 def _split_markdown_lines(
-    text: str, max_token_per_line: int, trim: bool, token_counter: Callable
+    text: str,
+    max_token_per_line: int,
+    trim: bool,
+    token_counter: Callable = _token_counter,
 ) -> List[str]:
     """
     Split markdown into lines.
     """
 
     return _split_str_lines(
         text=text,
@@ -188,15 +191,18 @@
         separators=MD_SPLIT_OPTIONS,
         trim=trim,
         token_counter=token_counter,
     )
 
 
 def _split_text_lines(
-    text: str, max_token_per_line: int, trim: bool, token_counter: Callable
+    text: str,
+    max_token_per_line: int,
+    trim: bool,
+    token_counter: Callable = _token_counter,
 ) -> List[str]:
     """
     Split text into lines.
     """
 
     return _split_str_lines(
         text=text,
@@ -208,15 +214,15 @@
 
 
 def _split_str_lines(
     text: str,
     max_tokens: int,
     separators: List[List[str]],
     trim: bool,
-    token_counter: Callable,
+    token_counter: Callable = _token_counter,
 ) -> List[str]:
     if not text:
         return []
 
     text = text.replace("\r\n", "\n")
     lines = []
     was_split = False
@@ -244,15 +250,15 @@
 
 
 def _split_str(
     text: str,
     max_tokens: int,
     separators: List[str],
     trim: bool,
-    token_counter: Callable,
+    token_counter: Callable = _token_counter,
 ) -> Tuple[List[str], bool]:
     """
     Split text into lines.
     """
     input_was_split = False
     if not text:
         return [], input_was_split
@@ -305,15 +311,15 @@
 
 
 def _split_list(
     text: List[str],
     max_tokens: int,
     separators: List[str],
     trim: bool,
-    token_counter: Callable,
+    token_counter: Callable = _token_counter,
 ) -> Tuple[List[str], bool]:
     """
     Split list of string into lines.
     """
     if not text:
         return [], False
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/utils/settings.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/utils/settings.py`

 * *Files 14% similar despite different names*

```diff
@@ -46,33 +46,40 @@
 
     assert api_key is not None, "Azure OpenAI API key not found in .env file"
     assert endpoint is not None, "Azure OpenAI endpoint not found in .env file"
 
     return deployment or "", api_key, endpoint
 
 
-def pinecone_settings_from_dot_env() -> Tuple[str, Optional[str]]:
+def postgres_settings_from_dot_env() -> str:
+    """Reads the Postgres connection string from the .env file.
+
+    Returns:
+        str: The Postgres connection string
     """
-    Reads the Pinecone API key and Environment from the .env file.
+    connection_string = None
+    config = dotenv_values(".env")
+    connection_string = config.get("POSTGRES_CONNECTION_STRING", None)
+
+    assert (
+        connection_string is not None
+    ), "Postgres connection string not found in .env file"
+
+    return connection_string
+
+
+def pinecone_settings_from_dot_env() -> Tuple[str, str]:
+    """Reads the Pinecone API key and Environment from the .env file.
+
     Returns:
         Tuple[str, str]: The Pinecone API key, the Pinecone Environment
     """
 
     api_key, environment = None, None
-    with open(".env", "r") as f:
-        lines = f.readlines()
-
-        for line in lines:
-            if line.startswith("PINECONE_API_KEY"):
-                parts = line.split("=")[1:]
-                api_key = "=".join(parts).strip().strip('"')
-                continue
-
-            if line.startswith("PINECONE_ENVIRONMENT"):
-                parts = line.split("=")[1:]
-                environment = "=".join(parts).strip().strip('"')
-                continue
+    config = dotenv_values(".env")
+    api_key = config.get("PINECONE_API_KEY", None)
+    environment = config.get("PINECONE_ENVIRONMENT", None)
 
     assert api_key is not None, "Pinecone API key not found in .env file"
     assert environment is not None, "Pinecone environment not found in .env file"
 
     return api_key, environment
```

### Comparing `semantic_kernel-0.3.2.dev0/semantic_kernel/utils/validation.py` & `semantic_kernel-0.3.3.dev0/semantic_kernel/utils/validation.py`

 * *Files identical despite different names*

### Comparing `semantic_kernel-0.3.2.dev0/PKG-INFO` & `semantic_kernel-0.3.3.dev0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: semantic-kernel
-Version: 0.3.2.dev0
+Version: 0.3.3.dev0
 Summary: 
 Author: Microsoft
 Author-email: SK-Support@microsoft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

