# Comparing `tmp/venture-ai-0.9.7.tar.gz` & `tmp/venture-ai-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "venture-ai-0.9.7.tar", last modified: Sun Jul 16 18:43:59 2023, max compression
+gzip compressed data, was "venture-ai-0.9.8.tar", last modified: Tue Jul 18 18:08:02 2023, max compression
```

## Comparing `venture-ai-0.9.7.tar` & `venture-ai-0.9.8.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-16 18:43:59.105192 venture-ai-0.9.7/
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641       78 2023-07-16 18:38:40.000000 venture-ai-0.9.7/CHANGELOG.txt
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641    11357 2023-07-14 19:11:29.000000 venture-ai-0.9.7/LICENSE
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641       30 2020-10-02 05:54:43.000000 venture-ai-0.9.7/MANIFEST.in
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     9489 2023-07-16 18:43:59.104966 venture-ai-0.9.7/PKG-INFO
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641      302 2023-07-16 18:38:14.000000 venture-ai-0.9.7/main.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641      321 2023-07-14 20:30:33.000000 venture-ai-0.9.7/misc.txt
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641       41 2023-07-14 10:19:57.000000 venture-ai-0.9.7/requirements-dev.txt
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641       38 2023-07-16 18:43:59.105255 venture-ai-0.9.7/setup.cfg
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     1859 2023-07-16 18:38:43.000000 venture-ai-0.9.7/setup.py
-drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-16 18:43:59.098827 venture-ai-0.9.7/venture/
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641       31 2023-07-14 19:09:40.000000 venture-ai-0.9.7/venture/__init__.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641    10755 2023-07-16 18:35:52.000000 venture-ai-0.9.7/venture/app.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     2996 2023-07-16 17:48:22.000000 venture-ai-0.9.7/venture/casual_utils.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     2185 2023-07-16 17:48:06.000000 venture-ai-0.9.7/venture/config.py
-drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-16 18:43:59.100538 venture-ai-0.9.7/venture/logic/
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641      116 2023-07-15 09:50:06.000000 venture-ai-0.9.7/venture/logic/__init__.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     9508 2023-07-16 17:48:21.000000 venture-ai-0.9.7/venture/logic/cosmos_logic.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     6842 2023-07-16 17:14:20.000000 venture-ai-0.9.7/venture/logic/explore_logic.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     2464 2023-07-16 12:47:33.000000 venture-ai-0.9.7/venture/logic/function_name_logic.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     2474 2023-07-13 06:49:47.000000 venture-ai-0.9.7/venture/logic/interlink_logic.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     5357 2023-07-13 09:38:38.000000 venture-ai-0.9.7/venture/logic/json_fixer_logic.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     3110 2023-07-16 17:42:16.000000 venture-ai-0.9.7/venture/logic/loaders_logic.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     3640 2023-07-16 13:40:13.000000 venture-ai-0.9.7/venture/logic/model_selector_logic.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     1613 2023-07-13 08:22:16.000000 venture-ai-0.9.7/venture/logic/openai_logic.py
-drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-16 18:43:59.100861 venture-ai-0.9.7/venture/logic/retrieval_logic/
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641        0 2023-07-16 17:15:03.000000 venture-ai-0.9.7/venture/logic/retrieval_logic/__init__.py
-drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-16 18:43:59.101517 venture-ai-0.9.7/venture/logic/retrieval_logic/objects/
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641        0 2023-07-16 17:14:54.000000 venture-ai-0.9.7/venture/logic/retrieval_logic/objects/__init__.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641      269 2023-07-16 06:04:21.000000 venture-ai-0.9.7/venture/logic/retrieval_logic/objects/package_input.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641      152 2023-07-16 05:25:12.000000 venture-ai-0.9.7/venture/logic/retrieval_logic/objects/package_output.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641      242 2023-07-15 18:27:25.000000 venture-ai-0.9.7/venture/logic/retrieval_logic/objects/retrieval_output.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     9264 2023-07-16 13:40:13.000000 venture-ai-0.9.7/venture/logic/retrieval_logic/retrieval_logic.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     3928 2023-07-16 12:43:37.000000 venture-ai-0.9.7/venture/logic/token_count_logic.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     1062 2023-07-15 17:35:33.000000 venture-ai-0.9.7/venture/metadata.py
-drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-16 18:43:59.102948 venture-ai-0.9.7/venture/objects/
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641        0 2023-07-14 20:33:29.000000 venture-ai-0.9.7/venture/objects/__init__.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     2524 2023-07-13 08:31:40.000000 venture-ai-0.9.7/venture/objects/chat_gpt_output.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641      197 2023-06-30 06:27:50.000000 venture-ai-0.9.7/venture/objects/context_based_response_output.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641       94 2023-07-12 17:36:17.000000 venture-ai-0.9.7/venture/objects/file_type.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641      425 2023-07-12 05:59:32.000000 venture-ai-0.9.7/venture/objects/interlink_commander_details_output.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641      232 2023-07-03 17:43:11.000000 venture-ai-0.9.7/venture/objects/llm_output.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641      693 2023-07-16 09:06:31.000000 venture-ai-0.9.7/venture/objects/parse_result.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     1251 2023-07-14 05:34:39.000000 venture-ai-0.9.7/venture/objects/parsed_doc.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641      388 2023-07-16 05:42:39.000000 venture-ai-0.9.7/venture/objects/token_counts.py
-drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-16 18:43:59.103967 venture-ai-0.9.7/venture/prompts/
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641        0 2023-07-14 20:33:37.000000 venture-ai-0.9.7/venture/prompts/__init__.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     1223 2023-07-14 05:53:24.000000 venture-ai-0.9.7/venture/prompts/system_function_name.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     1603 2023-07-16 12:42:43.000000 venture-ai-0.9.7/venture/prompts/system_ownership.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     5459 2023-07-16 15:03:02.000000 venture-ai-0.9.7/venture/prompts/system_retrieval_caller.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     2234 2023-07-16 12:09:11.000000 venture-ai-0.9.7/venture/prompts/system_retrieval_verdict.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641      148 2023-07-07 11:57:16.000000 venture-ai-0.9.7/venture/prompts/system_summary.py
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     2624 2023-07-16 11:37:06.000000 venture-ai-0.9.7/venture/prompts/system_venture.py
-drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-16 18:43:59.104691 venture-ai-0.9.7/venture_ai.egg-info/
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     9489 2023-07-16 18:43:59.000000 venture-ai-0.9.7/venture_ai.egg-info/PKG-INFO
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641     1559 2023-07-16 18:43:59.000000 venture-ai-0.9.7/venture_ai.egg-info/SOURCES.txt
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641        1 2023-07-16 18:43:59.000000 venture-ai-0.9.7/venture_ai.egg-info/dependency_links.txt
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641       41 2023-07-16 18:43:59.000000 venture-ai-0.9.7/venture_ai.egg-info/requires.txt
--rw-r--r--   0 roy.sadaka (1831260692) 1720933641        8 2023-07-16 18:43:59.000000 venture-ai-0.9.7/venture_ai.egg-info/top_level.txt
+drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-18 18:08:02.260064 venture-ai-0.9.8/
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641      279 2023-07-18 18:05:04.000000 venture-ai-0.9.8/CHANGELOG.txt
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641    11357 2023-07-14 19:11:29.000000 venture-ai-0.9.8/LICENSE
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641       30 2020-10-02 05:54:43.000000 venture-ai-0.9.8/MANIFEST.in
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     9635 2023-07-18 18:08:02.259870 venture-ai-0.9.8/PKG-INFO
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641      351 2023-07-18 17:20:00.000000 venture-ai-0.9.8/main.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641      425 2023-07-16 18:47:32.000000 venture-ai-0.9.8/misc.txt
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641       41 2023-07-14 10:19:57.000000 venture-ai-0.9.8/requirements-dev.txt
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641       38 2023-07-18 18:08:02.260117 venture-ai-0.9.8/setup.cfg
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     1859 2023-07-18 18:05:20.000000 venture-ai-0.9.8/setup.py
+drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-18 18:08:02.254005 venture-ai-0.9.8/venture/
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641       31 2023-07-14 19:09:40.000000 venture-ai-0.9.8/venture/__init__.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641    10755 2023-07-16 18:35:52.000000 venture-ai-0.9.8/venture/app.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     2996 2023-07-16 17:48:22.000000 venture-ai-0.9.8/venture/casual_utils.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     2193 2023-07-18 17:52:19.000000 venture-ai-0.9.8/venture/config.py
+drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-18 18:08:02.255525 venture-ai-0.9.8/venture/logic/
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641      116 2023-07-15 09:50:06.000000 venture-ai-0.9.8/venture/logic/__init__.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     9508 2023-07-16 17:48:21.000000 venture-ai-0.9.8/venture/logic/cosmos_logic.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     6810 2023-07-18 17:50:45.000000 venture-ai-0.9.8/venture/logic/explore_logic.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     2464 2023-07-16 12:47:33.000000 venture-ai-0.9.8/venture/logic/function_name_logic.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     2474 2023-07-13 06:49:47.000000 venture-ai-0.9.8/venture/logic/interlink_logic.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     5357 2023-07-13 09:38:38.000000 venture-ai-0.9.8/venture/logic/json_fixer_logic.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     3110 2023-07-16 17:42:16.000000 venture-ai-0.9.8/venture/logic/loaders_logic.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     3448 2023-07-18 17:50:37.000000 venture-ai-0.9.8/venture/logic/model_selector_logic.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     1613 2023-07-13 08:22:16.000000 venture-ai-0.9.8/venture/logic/openai_logic.py
+drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-18 18:08:02.255838 venture-ai-0.9.8/venture/logic/retrieval_logic/
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641        0 2023-07-16 17:15:03.000000 venture-ai-0.9.8/venture/logic/retrieval_logic/__init__.py
+drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-18 18:08:02.256417 venture-ai-0.9.8/venture/logic/retrieval_logic/objects/
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641        0 2023-07-16 17:14:54.000000 venture-ai-0.9.8/venture/logic/retrieval_logic/objects/__init__.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641      269 2023-07-16 06:04:21.000000 venture-ai-0.9.8/venture/logic/retrieval_logic/objects/package_input.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641      152 2023-07-16 05:25:12.000000 venture-ai-0.9.8/venture/logic/retrieval_logic/objects/package_output.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641      242 2023-07-15 18:27:25.000000 venture-ai-0.9.8/venture/logic/retrieval_logic/objects/retrieval_output.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     9264 2023-07-16 13:40:13.000000 venture-ai-0.9.8/venture/logic/retrieval_logic/retrieval_logic.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     4037 2023-07-18 18:00:49.000000 venture-ai-0.9.8/venture/logic/token_count_logic.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     1062 2023-07-15 17:35:33.000000 venture-ai-0.9.8/venture/metadata.py
+drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-18 18:08:02.257723 venture-ai-0.9.8/venture/objects/
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641        0 2023-07-14 20:33:29.000000 venture-ai-0.9.8/venture/objects/__init__.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     2524 2023-07-13 08:31:40.000000 venture-ai-0.9.8/venture/objects/chat_gpt_output.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641      197 2023-06-30 06:27:50.000000 venture-ai-0.9.8/venture/objects/context_based_response_output.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641       94 2023-07-12 17:36:17.000000 venture-ai-0.9.8/venture/objects/file_type.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641      425 2023-07-12 05:59:32.000000 venture-ai-0.9.8/venture/objects/interlink_commander_details_output.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641      232 2023-07-03 17:43:11.000000 venture-ai-0.9.8/venture/objects/llm_output.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641      693 2023-07-16 09:06:31.000000 venture-ai-0.9.8/venture/objects/parse_result.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     1251 2023-07-14 05:34:39.000000 venture-ai-0.9.8/venture/objects/parsed_doc.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641      388 2023-07-16 05:42:39.000000 venture-ai-0.9.8/venture/objects/token_counts.py
+drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-18 18:08:02.258805 venture-ai-0.9.8/venture/prompts/
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641        0 2023-07-14 20:33:37.000000 venture-ai-0.9.8/venture/prompts/__init__.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     1223 2023-07-14 05:53:24.000000 venture-ai-0.9.8/venture/prompts/system_function_name.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     1603 2023-07-16 12:42:43.000000 venture-ai-0.9.8/venture/prompts/system_ownership.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     5459 2023-07-16 15:03:02.000000 venture-ai-0.9.8/venture/prompts/system_retrieval_caller.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     2234 2023-07-16 12:09:11.000000 venture-ai-0.9.8/venture/prompts/system_retrieval_verdict.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641      148 2023-07-07 11:57:16.000000 venture-ai-0.9.8/venture/prompts/system_summary.py
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     2624 2023-07-16 11:37:06.000000 venture-ai-0.9.8/venture/prompts/system_venture.py
+drwxr-xr-x   0 roy.sadaka (1831260692) 1720933641        0 2023-07-18 18:08:02.259621 venture-ai-0.9.8/venture_ai.egg-info/
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     9635 2023-07-18 18:08:02.000000 venture-ai-0.9.8/venture_ai.egg-info/PKG-INFO
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641     1559 2023-07-18 18:08:02.000000 venture-ai-0.9.8/venture_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641        1 2023-07-18 18:08:02.000000 venture-ai-0.9.8/venture_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641       41 2023-07-18 18:08:02.000000 venture-ai-0.9.8/venture_ai.egg-info/requires.txt
+-rw-r--r--   0 roy.sadaka (1831260692) 1720933641        8 2023-07-18 18:08:02.000000 venture-ai-0.9.8/venture_ai.egg-info/top_level.txt
```

### Comparing `venture-ai-0.9.7/LICENSE` & `venture-ai-0.9.8/LICENSE`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/PKG-INFO` & `venture-ai-0.9.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venture-ai
-Version: 0.9.7
+Version: 0.9.8
 Summary: A Fast, Flexible Trainer with Callbacks and Extensions for PyTorch
 Home-page: https://github.com/roysadaka/venture
 Author: Roy Sadaka
 Maintainer: lpd developers
 Maintainer-email: torch.lpd@gmail.com
 License: MIT Licences
 Keywords: ai,natural language processing,large language models,project exploration,chatbot,documentation exploration,reasoning based search,assistant,chatgpt,openai
@@ -53,14 +53,15 @@
 ```python
 from venture import Venture
 
 if __name__ == '__main__':
     v = Venture(openai_api_key='sk-...',  # OBTAINED FROM https://platform.openai.com/account/api-keys
                 captain_email='captain@spaceship.com',  # THE DEFAULT CONTACT IN INTERLINK TAB 
                 extra_role='You are an AI assistant for Venture Company.', # ANY INFO ABOUT YOUR SPECIFIC USE CASE
+                cosmos_path='/Users/captain/Documents/MyVenture/', # Optional, THE PATH TO STORE THE PARSED DOCUMENTS AND INTERNAL INDEXING
                 share=False) # FOR SHARING THE APP LINK OUTSIDE YOUR LOCAL NETWORK
     v.launch()
 ```
 
 After initiating the launch, ``Venture``, powered by Gradio, will generate a cosmic link that enables you to activate the application.  
 Effortlessly navigate to the bestowed link amidst the vastness of your web browser's galaxy.
 ```sh
@@ -76,24 +77,24 @@
 
 ---
 
 ## 💫 A Cosmic Journey
 In the celestial realm of the web app, ``Venture`` unveils its enchanting interface.  
 Prepare to embark on a cosmic journey through its three celestial tabs, each designed to guide you through the depths of your project documentation and beyond.
 
-1. 🧑‍🚀 Explore Tab: Unveil the Secrets of the Cosmos
+1. 🧑‍🚀 Explore Tab: Unveil the Secrets of the Cosmos  
     This ethereal tab serves as your portal to the wonders of project documentation.  
     In it, ``Venture`` eagerly awaits your inquiries and questions.  
     Discover the vast knowledge it holds or let its "Auto-Pilot" feature autonomously guide you to the precise documentation you seek.
 
-2. 🌟 Cosmos Tab: Forge New Stars in the Galaxy
+2. 🌟 Cosmos Tab: Forge New Stars in the Galaxy  
     In this celestial workshop, you possess the power to shape the very fabric of your cosmos.  
     Add new constellations of knowledge to the cosmic expanse or remove existing ones as you navigate through the possibilities of your documentation universe.
 
-3. 📡 Interlink Tab: Communication Across the Stars
+3. 📡 Interlink Tab: Communication Across the Stars  
     This celestial conduit bridges the gap between you and the support team, ensuring seamless communication amidst the cosmic expanse.  
     Should you encounter enigmatic anomalies or deem a documentation update necessary, harness the power of the Interlink Tab to connect with the support team, who will guide you through the celestial seas of knowledge.
 
 ---
```

### Comparing `venture-ai-0.9.7/setup.py` & `venture-ai-0.9.8/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
         'Programming Language :: Python :: 3.9',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Utilities'
     ]
 
 setup(
     name='venture-ai',
-    version='0.9.7',
+    version='0.9.8',
     description='A Fast, Flexible Trainer with Callbacks and Extensions for PyTorch',
     long_description_content_type='text/markdown',
     long_description=README_md,
     license='MIT Licences',
     url='https://github.com/roysadaka/venture',
     author='Roy Sadaka',
     maintainer='lpd developers',
```

### Comparing `venture-ai-0.9.7/venture/app.py` & `venture-ai-0.9.8/venture/app.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/casual_utils.py` & `venture-ai-0.9.8/venture/casual_utils.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/config.py` & `venture-ai-0.9.8/venture/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 class Config:
     # LOGIC
     MIN_TOKENS_TO_CONSIDER_DOC = 200
     MAX_TOKENS_TO_CONSIDER_DOC = 14_000
-    TOKEN_COUNT_MULTIPLIER = 1.1
+    FUNCTION_CALL_ADDED_TOKEN_COUNT = 11
     RESERVED_RETRIEVAL_TOKEN_COUNT = 500
     RESERVED_RESPONSE_TOKEN_COUNT = 1000
     SUMMARY_RESERVED_RESPONSE_TOKEN_COUNT = 1000
     OWNERSHIP_RESERVED_RESPONSE_TOKEN_COUNT = 200
     FUNCTION_NAME_RESERVED_RESPONSE_TOKEN_COUNT = 200
     ERROR_RESPONSE = "Apologies, there seems to be an unknown error.\nPlease try again or contact the devs."
     MODEL_NAME_TO_MAX_TOKENS = {'gpt-3.5-turbo-0613':4096, 'gpt-3.5-turbo-16k-0613':16384}
```

### Comparing `venture-ai-0.9.7/venture/logic/cosmos_logic.py` & `venture-ai-0.9.8/venture/logic/cosmos_logic.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/logic/explore_logic.py` & `venture-ai-0.9.8/venture/logic/explore_logic.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 def get_context_file_names_that_fit_in_window(metadata:Metadata, user_query:str, context_file_names_to_use:List[str]) -> List[str]:
     file_name_to_parsed_doc = metadata.file_name_to_parsed_doc
 
     max_token_count = max(Config.MODEL_NAME_TO_MAX_TOKENS.values())
 
     minimal_token_count = metadata.token_counts.explore_all_prompt_token_count + \
                             token_count_logic.count_tokens(user_query)
-    minimal_token_count = minimal_token_count * Config.TOKEN_COUNT_MULTIPLIER + Config.RESERVED_RESPONSE_TOKEN_COUNT
+    minimal_token_count = minimal_token_count + Config.RESERVED_RESPONSE_TOKEN_COUNT
     
     left_over_token_count = max_token_count - minimal_token_count
     result = []
     # WE CAN ASSUME AT LEAST 1 DOC WILL FIT
     for context_file_name_to_use in context_file_names_to_use:
         if left_over_token_count > file_name_to_parsed_doc[context_file_name_to_use].content_token_count:
             result.append(context_file_name_to_use)
```

### Comparing `venture-ai-0.9.7/venture/logic/function_name_logic.py` & `venture-ai-0.9.8/venture/logic/function_name_logic.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/logic/interlink_logic.py` & `venture-ai-0.9.8/venture/logic/interlink_logic.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/logic/json_fixer_logic.py` & `venture-ai-0.9.8/venture/logic/json_fixer_logic.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/logic/loaders_logic.py` & `venture-ai-0.9.8/venture/logic/loaders_logic.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/logic/model_selector_logic.py` & `venture-ai-0.9.8/venture/logic/model_selector_logic.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,54 +11,54 @@
         if token_count < max_tokens and max_tokens < lowest_model_token_count:
             lowest_model_name = model_name
             lowest_model_token_count = max_tokens
     return lowest_model_name
 
 def get_model_name_for_function_name_extract(metadata:Metadata, summary_token_count:int) -> str:
     token_count = metadata.token_counts.cosmos_function_name_all_prompt_count + summary_token_count
-    token_count = token_count * Config.TOKEN_COUNT_MULTIPLIER + Config.FUNCTION_NAME_RESERVED_RESPONSE_TOKEN_COUNT
+    token_count = token_count + Config.FUNCTION_NAME_RESERVED_RESPONSE_TOKEN_COUNT
     model_name = get_model_based_on_token_count(token_count)
     return model_name
 
 def get_model_name_for_ownership_extract(metadata:Metadata, processed_doc_token_count:int) -> str:
     token_count = metadata.token_counts.cosmos_system_ownership_all_prompt_count + processed_doc_token_count
-    token_count = token_count * Config.TOKEN_COUNT_MULTIPLIER + Config.OWNERSHIP_RESERVED_RESPONSE_TOKEN_COUNT
+    token_count = token_count + Config.OWNERSHIP_RESERVED_RESPONSE_TOKEN_COUNT
     model_name = get_model_based_on_token_count(token_count)
     return model_name
 
 def get_model_name_for_summary_extract(metadata:Metadata, processed_doc_token_count:int) -> str:
     token_count = metadata.token_counts.cosmos_system_summary_count + processed_doc_token_count
-    token_count = token_count * Config.TOKEN_COUNT_MULTIPLIER + Config.SUMMARY_RESERVED_RESPONSE_TOKEN_COUNT
+    token_count = token_count + Config.SUMMARY_RESERVED_RESPONSE_TOKEN_COUNT
     model_name = get_model_based_on_token_count(token_count)
     return model_name
 
 def get_model_name_for_retrieval_caller(metadata:Metadata, user_query:str, functions:List[object]) -> str:
     token_count =   metadata.token_counts.retrieval_caller_system_count + \
                     token_count_logic.count_tokens(user_query) + \
                     token_count_logic.count_tokens(Config.EXTRA_ROLE) + \
                     sum(metadata.token_counts.retrieval_function_name_to_count[f['name']] for f in functions)
-    token_count = token_count * Config.TOKEN_COUNT_MULTIPLIER + Config.RESERVED_RESPONSE_TOKEN_COUNT
+    token_count = token_count + Config.RESERVED_RESPONSE_TOKEN_COUNT
     model_name = get_model_based_on_token_count(token_count)
     return model_name
 
 
 def get_model_name_for_retrieval_verdict(metadata:Metadata, user_message:str) -> str:
     token_count =   metadata.token_counts.retrieval_verdict_system_count + \
                     token_count_logic.count_tokens(user_message) + \
                     token_count_logic.count_tokens(Config.EXTRA_ROLE)
     
-    token_count = token_count * Config.TOKEN_COUNT_MULTIPLIER + Config.RESERVED_RESPONSE_TOKEN_COUNT
+    token_count = token_count + Config.RESERVED_RESPONSE_TOKEN_COUNT
     model_name = get_model_based_on_token_count(token_count)
     return model_name
 
 def get_model_name_for_llm_response(metadata:Metadata, user_query:str, context_file_names_to_use:List[str]) -> str:
     file_name_to_parsed_doc = metadata.file_name_to_parsed_doc
 
     token_count =   metadata.token_counts.explore_all_prompt_token_count + \
                     token_count_logic.count_tokens(Config.EXTRA_ROLE) + \
                     sum(file_name_to_parsed_doc[file_name].content_token_count for file_name in context_file_names_to_use) + \
                     token_count_logic.count_tokens(user_query)
     
-    token_count = token_count * Config.TOKEN_COUNT_MULTIPLIER + Config.RESERVED_RESPONSE_TOKEN_COUNT
+    token_count = token_count + Config.RESERVED_RESPONSE_TOKEN_COUNT
     model_name = get_model_based_on_token_count(token_count)
     return model_name
```

### Comparing `venture-ai-0.9.7/venture/logic/openai_logic.py` & `venture-ai-0.9.8/venture/logic/openai_logic.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/logic/retrieval_logic/retrieval_logic.py` & `venture-ai-0.9.8/venture/logic/retrieval_logic/retrieval_logic.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/logic/token_count_logic.py` & `venture-ai-0.9.8/venture/logic/token_count_logic.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,30 +9,34 @@
 import tiktoken
 import json
 
 def count_tokens(text:str):
     tokenizer = tiktoken.get_encoding(Config.TOKENIZER_NAME)
     return len(tokenizer.encode(text))
 
+def function_call_count_tokens(f:object):
+    f_as_str = json.dumps(f)
+    return count_tokens(f_as_str) + Config.FUNCTION_CALL_ADDED_TOKEN_COUNT
+
 def get_explore_all_prompt_token_count():
     explore_functions = [system_venture.ANSWER_FOUND_HANDLER, system_venture.MISSING_ANSWER_HANDLER]
-    explore_functions_token_count = sum(count_tokens(json.dumps(f)) for f in explore_functions)
+    explore_functions_token_count = sum(function_call_count_tokens(f) for f in explore_functions)
     explore_all_prompt_token_count = explore_functions_token_count + count_tokens(system_venture.SYSTEM_MESSAGE) + count_tokens(system_venture.USER_MESSAGE)
     return explore_all_prompt_token_count
 
 def get_cosmos_function_name_all_prompt_token_count():
     cosmos_function_name_all_prompt_token_count = count_tokens(system_function_name.SYSTEM_MESSAGE) + \
                                     count_tokens(system_function_name.USER_MESSAGE_TEMPLATE) + \
-                                    count_tokens(json.dumps(system_function_name.FILE_NAME_HANDLER)) 
+                                    function_call_count_tokens(system_function_name.FILE_NAME_HANDLER) 
     return cosmos_function_name_all_prompt_token_count
 
 def get_cosmos_ownership_all_prompt_token_count():
     cosmos_ownership_all_prompt_token_count = count_tokens(system_ownership.SYSTEM_MESSAGE) + \
                                                 count_tokens(system_ownership.USER_MESSAGE) + \
-                                                count_tokens(json.dumps(system_ownership.OWNERSHIP_HANDLER)) 
+                                                function_call_count_tokens(system_ownership.OWNERSHIP_HANDLER) 
     return cosmos_ownership_all_prompt_token_count
 
 def get_system_token_counts():
     retrieval_caller_system_count = count_tokens(system_retrieval_caller.SYSTEM_MESSAGE) + count_tokens(system_retrieval_caller.USER_MESSAGE)
     retrieval_verdict_system_count = count_tokens(system_retrieval_verdict.SYSTEM_MESSAGE) + count_tokens(system_retrieval_verdict.USER_MESSAGE)
     explore_all_prompt_token_count = get_explore_all_prompt_token_count()
     cosmos_function_name_all_prompt_token_count = get_cosmos_function_name_all_prompt_token_count()
@@ -43,21 +47,21 @@
             explore_all_prompt_token_count, \
             cosmos_function_name_all_prompt_token_count, \
             cosmos_system_summary_token_count, \
             cosmos_ownership_all_prompt_token_count
 
 def get_cosmos_ownership_function_to_token_count():
     ownership_functions = [system_ownership.OWNERSHIP_HANDLER]
-    ownership_function_name_to_token_count = {f['name']:count_tokens(json.dumps(f)) for f in ownership_functions}
+    ownership_function_name_to_token_count = {f['name']:function_call_count_tokens(f) for f in ownership_functions}
     return ownership_function_name_to_token_count
 
 def get_retrieval_function_name_to_token_count(metadata:Metadata):
     function_name_to_file_name = metadata.function_name_to_file_name
     file_name_to_parsed_doc = metadata.file_name_to_parsed_doc
-    system_retrieval_caller.NON_TEMPLATE_FUNCTIONS
+
     # TOKEN COUNTS
-    retrieval_function_name_to_token_count = {f['name']:count_tokens(json.dumps(f)) for f in system_retrieval_caller.NON_TEMPLATE_FUNCTIONS}
-    template_token_count = count_tokens(json.dumps(system_retrieval_caller.TEMPLATE_TOPIC_HANDLER))
+    retrieval_function_name_to_token_count = {f['name']:function_call_count_tokens(f) for f in system_retrieval_caller.NON_TEMPLATE_FUNCTIONS}
+    template_token_count = function_call_count_tokens(system_retrieval_caller.TEMPLATE_TOPIC_HANDLER)
     for function_name, file_name in function_name_to_file_name.items():
         parsed_doc = file_name_to_parsed_doc[file_name]
         retrieval_function_name_to_token_count[function_name] = template_token_count + parsed_doc.summary_token_count
     return retrieval_function_name_to_token_count
```

### Comparing `venture-ai-0.9.7/venture/metadata.py` & `venture-ai-0.9.8/venture/metadata.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/objects/chat_gpt_output.py` & `venture-ai-0.9.8/venture/objects/chat_gpt_output.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/objects/parse_result.py` & `venture-ai-0.9.8/venture/objects/parse_result.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/objects/parsed_doc.py` & `venture-ai-0.9.8/venture/objects/parsed_doc.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/prompts/system_function_name.py` & `venture-ai-0.9.8/venture/prompts/system_function_name.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/prompts/system_ownership.py` & `venture-ai-0.9.8/venture/prompts/system_ownership.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/prompts/system_retrieval_caller.py` & `venture-ai-0.9.8/venture/prompts/system_retrieval_caller.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/prompts/system_retrieval_verdict.py` & `venture-ai-0.9.8/venture/prompts/system_retrieval_verdict.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture/prompts/system_venture.py` & `venture-ai-0.9.8/venture/prompts/system_venture.py`

 * *Files identical despite different names*

### Comparing `venture-ai-0.9.7/venture_ai.egg-info/PKG-INFO` & `venture-ai-0.9.8/venture_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: venture-ai
-Version: 0.9.7
+Version: 0.9.8
 Summary: A Fast, Flexible Trainer with Callbacks and Extensions for PyTorch
 Home-page: https://github.com/roysadaka/venture
 Author: Roy Sadaka
 Maintainer: lpd developers
 Maintainer-email: torch.lpd@gmail.com
 License: MIT Licences
 Keywords: ai,natural language processing,large language models,project exploration,chatbot,documentation exploration,reasoning based search,assistant,chatgpt,openai
@@ -53,14 +53,15 @@
 ```python
 from venture import Venture
 
 if __name__ == '__main__':
     v = Venture(openai_api_key='sk-...',  # OBTAINED FROM https://platform.openai.com/account/api-keys
                 captain_email='captain@spaceship.com',  # THE DEFAULT CONTACT IN INTERLINK TAB 
                 extra_role='You are an AI assistant for Venture Company.', # ANY INFO ABOUT YOUR SPECIFIC USE CASE
+                cosmos_path='/Users/captain/Documents/MyVenture/', # Optional, THE PATH TO STORE THE PARSED DOCUMENTS AND INTERNAL INDEXING
                 share=False) # FOR SHARING THE APP LINK OUTSIDE YOUR LOCAL NETWORK
     v.launch()
 ```
 
 After initiating the launch, ``Venture``, powered by Gradio, will generate a cosmic link that enables you to activate the application.  
 Effortlessly navigate to the bestowed link amidst the vastness of your web browser's galaxy.
 ```sh
@@ -76,24 +77,24 @@
 
 ---
 
 ## 💫 A Cosmic Journey
 In the celestial realm of the web app, ``Venture`` unveils its enchanting interface.  
 Prepare to embark on a cosmic journey through its three celestial tabs, each designed to guide you through the depths of your project documentation and beyond.
 
-1. 🧑‍🚀 Explore Tab: Unveil the Secrets of the Cosmos
+1. 🧑‍🚀 Explore Tab: Unveil the Secrets of the Cosmos  
     This ethereal tab serves as your portal to the wonders of project documentation.  
     In it, ``Venture`` eagerly awaits your inquiries and questions.  
     Discover the vast knowledge it holds or let its "Auto-Pilot" feature autonomously guide you to the precise documentation you seek.
 
-2. 🌟 Cosmos Tab: Forge New Stars in the Galaxy
+2. 🌟 Cosmos Tab: Forge New Stars in the Galaxy  
     In this celestial workshop, you possess the power to shape the very fabric of your cosmos.  
     Add new constellations of knowledge to the cosmic expanse or remove existing ones as you navigate through the possibilities of your documentation universe.
 
-3. 📡 Interlink Tab: Communication Across the Stars
+3. 📡 Interlink Tab: Communication Across the Stars  
     This celestial conduit bridges the gap between you and the support team, ensuring seamless communication amidst the cosmic expanse.  
     Should you encounter enigmatic anomalies or deem a documentation update necessary, harness the power of the Interlink Tab to connect with the support team, who will guide you through the celestial seas of knowledge.
 
 ---
```

### Comparing `venture-ai-0.9.7/venture_ai.egg-info/SOURCES.txt` & `venture-ai-0.9.8/venture_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

