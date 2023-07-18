# Comparing `tmp/log10_io-0.1.0.tar.gz` & `tmp/log10_io-0.2.1.tar.gz`

## Comparing `log10_io-0.1.0.tar` & `log10_io-0.2.1.tar`

### file list

```diff
@@ -1,45 +1,47 @@
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 log10_io-0.1.0/requirements.txt
--rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 log10_io-0.1.0/setup.py
--rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.1.0/.github/workflows/release.yml
--rw-r--r--   0        0        0     2675 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/README.md
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/agents/biochemist.py
--rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/agents/code_optimizer.py
--rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/agents/coder.py
--rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/agents/cybersecurity_expert.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/agents/email_generator.py
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/agents/scrape_summarizer.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/agents/translator.py
--rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/evals/basic_eval.py
--rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/evals/compile.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/evals/fuzzy.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/evals/fuzzy_data.csv
--rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/evals/match_data.csv
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/logging/anthropic_completion.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/logging/chatcompletion.py
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/logging/chatcompletion_async_vs_sync.py
--rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/logging/completion.py
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/logging/completion_ada.py
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/logging/get_url.py
--rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/logging/langchain_babyagi.py
--rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/logging/langchain_multiple_tools.py
--rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/logging/langchain_qa.py
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/logging/langchain_simple_sequential.py
--rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/logging/langchain_sqlagent.py
--rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.1.0/examples/logging/multiple_sessions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.1.0/log10/__init__.py
--rw-r--r--   0        0        0     3923 2020-02-02 00:00:00.000000 log10_io-0.1.0/log10/anthropic.py
--rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.1.0/log10/bigquery.py
--rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 log10_io-0.1.0/log10/evals.py
--rw-r--r--   0        0        0     2822 2020-02-02 00:00:00.000000 log10_io-0.1.0/log10/llm.py
--rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 log10_io-0.1.0/log10/load.py
--rw-r--r--   0        0        0     2022 2020-02-02 00:00:00.000000 log10_io-0.1.0/log10/openai.py
--rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 log10_io-0.1.0/log10/tools.py
--rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 log10_io-0.1.0/log10/utils.py
--rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 log10_io-0.1.0/log10/agents/camel.py
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 log10_io-0.1.0/log10/agents/scrape_summarizer.py
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.1.0/log10/schemas/bigquery.json
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 log10_io-0.1.0/.gitignore
--rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.1.0/LICENSE
--rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 log10_io-0.1.0/README.md
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 log10_io-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 log10_io-0.2.1/requirements.txt
+-rw-r--r--   0        0        0      443 2020-02-02 00:00:00.000000 log10_io-0.2.1/setup.py
+-rw-r--r--   0        0        0     1045 2020-02-02 00:00:00.000000 log10_io-0.2.1/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2792 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/README.md
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/agents/biochemist.py
+-rw-r--r--   0        0        0     1896 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/agents/code_optimizer.py
+-rw-r--r--   0        0        0      972 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/agents/coder.py
+-rw-r--r--   0        0        0     1343 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/agents/cybersecurity_expert.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/agents/email_generator.py
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/agents/translator.py
+-rw-r--r--   0        0        0     1583 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/evals/basic_eval.py
+-rw-r--r--   0        0        0     1200 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/evals/compile.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/evals/fuzzy.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/evals/fuzzy_data.csv
+-rw-r--r--   0        0        0      520 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/evals/match_data.csv
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/logging/anthropic_completion.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/logging/chatcompletion.py
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/logging/chatcompletion_async_vs_sync.py
+-rw-r--r--   0        0        0      407 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/logging/completion.py
+-rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/logging/completion_ada.py
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/logging/get_url.py
+-rw-r--r--   0        0        0    10777 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/logging/langchain_babyagi.py
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/logging/langchain_model_logger.py
+-rw-r--r--   0        0        0      623 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/logging/langchain_multiple_tools.py
+-rw-r--r--   0        0        0     1162 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/logging/langchain_qa.py
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/logging/langchain_simple_sequential.py
+-rw-r--r--   0        0        0     2513 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/logging/langchain_sqlagent.py
+-rw-r--r--   0        0        0     1704 2020-02-02 00:00:00.000000 log10_io-0.2.1/examples/logging/multiple_sessions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 log10_io-0.2.1/log10/__init__.py
+-rw-r--r--   0        0        0     4005 2020-02-02 00:00:00.000000 log10_io-0.2.1/log10/anthropic.py
+-rw-r--r--   0        0        0     2594 2020-02-02 00:00:00.000000 log10_io-0.2.1/log10/bigquery.py
+-rw-r--r--   0        0        0     2684 2020-02-02 00:00:00.000000 log10_io-0.2.1/log10/evals.py
+-rw-r--r--   0        0        0     9293 2020-02-02 00:00:00.000000 log10_io-0.2.1/log10/langchain.py
+-rw-r--r--   0        0        0     6785 2020-02-02 00:00:00.000000 log10_io-0.2.1/log10/llm.py
+-rw-r--r--   0        0        0    13081 2020-02-02 00:00:00.000000 log10_io-0.2.1/log10/load.py
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 log10_io-0.2.1/log10/openai.py
+-rw-r--r--   0        0        0     2101 2020-02-02 00:00:00.000000 log10_io-0.2.1/log10/tools.py
+-rw-r--r--   0        0        0     1051 2020-02-02 00:00:00.000000 log10_io-0.2.1/log10/utils.py
+-rw-r--r--   0        0        0     9271 2020-02-02 00:00:00.000000 log10_io-0.2.1/log10/agents/camel.py
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 log10_io-0.2.1/log10/agents/scrape_summarizer.py
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 log10_io-0.2.1/log10/schemas/bigquery.json
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 log10_io-0.2.1/.gitignore
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 log10_io-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2715 2020-02-02 00:00:00.000000 log10_io-0.2.1/README.md
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 log10_io-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 log10_io-0.2.1/PKG-INFO
```

### Comparing `log10_io-0.1.0/.github/workflows/release.yml` & `log10_io-0.2.1/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/README.md` & `log10_io-0.2.1/examples/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -36,11 +36,12 @@
 
 - `langchain_babyagi.py` [Langchain's implementation](https://python.langchain.com/en/latest/use_cases/agents/baby_agi_with_agent.html) of [BabyAGI](https://babyagi.org/)
 - `langchain_multiple_tools.py` Langchain with multiple tools
 - `langchain_qa.py` Langchain + DocumentQA (also checkout Streamlit example [here](https://huggingface.co/spaces/arjunbansal/log10_langchain_qa_streamlit/blob/main/app.py))
 - `langchain_simple_sequential.py` Simplest Langchain example with 2 chains in sequence
 - `langchain_sqlagent.py` Langchain's SQLAgent for NLP2SQL
 - `multiple_sessions.py` Examples illustrating session scoping for Langchain + Log10
+- `langchain_model_logger.py` Example of OpenAI (chat and text completions) and Anthropic calls with a log10 logger.
 
 ### Anthropic
 
 - `anthropic_completion.py` Simple Anthropic completion example
```

### Comparing `log10_io-0.1.0/examples/agents/biochemist.py` & `log10_io-0.2.1/examples/agents/biochemist.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/agents/code_optimizer.py` & `log10_io-0.2.1/examples/agents/code_optimizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/agents/coder.py` & `log10_io-0.2.1/examples/agents/coder.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/agents/cybersecurity_expert.py` & `log10_io-0.2.1/examples/agents/cybersecurity_expert.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/agents/email_generator.py` & `log10_io-0.2.1/examples/agents/email_generator.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/agents/scrape_summarizer.py` & `log10_io-0.2.1/examples/agents/scrape_summarizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/agents/translator.py` & `log10_io-0.2.1/examples/agents/translator.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/evals/basic_eval.py` & `log10_io-0.2.1/examples/evals/basic_eval.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/evals/compile.py` & `log10_io-0.2.1/examples/evals/compile.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/evals/fuzzy.py` & `log10_io-0.2.1/examples/evals/fuzzy.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/evals/fuzzy_data.csv` & `log10_io-0.2.1/examples/evals/fuzzy_data.csv`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/evals/match_data.csv` & `log10_io-0.2.1/examples/evals/match_data.csv`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/logging/chatcompletion_async_vs_sync.py` & `log10_io-0.2.1/examples/logging/chatcompletion_async_vs_sync.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/logging/get_url.py` & `log10_io-0.2.1/examples/logging/get_url.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/logging/langchain_babyagi.py` & `log10_io-0.2.1/examples/logging/langchain_babyagi.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/logging/langchain_multiple_tools.py` & `log10_io-0.2.1/examples/logging/langchain_multiple_tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/logging/langchain_qa.py` & `log10_io-0.2.1/examples/logging/langchain_qa.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/logging/langchain_simple_sequential.py` & `log10_io-0.2.1/examples/logging/langchain_simple_sequential.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/logging/langchain_sqlagent.py` & `log10_io-0.2.1/examples/logging/langchain_sqlagent.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/examples/logging/multiple_sessions.py` & `log10_io-0.2.1/examples/logging/multiple_sessions.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/log10/anthropic.py` & `log10_io-0.2.1/log10/anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,19 @@
 
 import uuid
 
 import logging
 
 
 class Anthropic(LLM):
-    def __init__(self, hparams: dict = None, skip_initialization: bool = False):
+    def __init__(
+        self, hparams: dict = None, skip_initialization: bool = False, log10_config=None
+    ):
+        super().__init__(hparams, log10_config)
+
         if not skip_initialization:
             self.client = anthropic.Anthropic()
         self.hparams = hparams
 
         if "max_tokens_to_sample" not in self.hparams:
             self.hparams["max_tokens_to_sample"] = 1024
```

### Comparing `log10_io-0.1.0/log10/bigquery.py` & `log10_io-0.2.1/log10/bigquery.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/log10/evals.py` & `log10_io-0.2.1/log10/evals.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/log10/load.py` & `log10_io-0.2.1/log10/load.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/log10/openai.py` & `log10_io-0.2.1/log10/openai.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 from copy import deepcopy
+import time
 from typing import List
 import openai
 from log10.llm import LLM, ChatCompletion, Message, TextCompletion
 
 import logging
 
 # for exponential backoff
 import backoff
 from openai.error import RateLimitError, APIConnectionError
 import openai
 
 
 class OpenAI(LLM):
-    def __init__(self, hparams: dict = None):
-        self.hparams = hparams
+    def __init__(self, hparams: dict = None, log10_config=None):
+        super().__init__(hparams, log10_config)
 
     @backoff.on_exception(backoff.expo, (RateLimitError, APIConnectionError))
     def chat(self, messages: List[Message], hparams: dict = None) -> ChatCompletion:
         completion = openai.ChatCompletion.create(
             **self.chat_request(messages, hparams)
         )
 
@@ -37,20 +38,17 @@
             "messages": [message.to_dict() for message in messages],
             **merged_hparams,
         }
 
     @backoff.on_exception(backoff.expo, (RateLimitError, APIConnectionError))
     def text(self, prompt: str, hparams: dict = None) -> TextCompletion:
         request = self.text_request(prompt, hparams)
-        logging.info(f"sending request: {request}")
         completion = openai.Completion.create(**request)
-        logging.info(f"received response: {completion}")
         return TextCompletion(text=completion.choices[0].text, response=completion)
 
     def text_request(self, prompt: str, hparams: dict = None) -> dict:
         merged_hparams = deepcopy(self.hparams)
         if hparams:
             for hparam in hparams:
                 merged_hparams[hparam] = hparams[hparam]
         output = {"prompt": prompt, **merged_hparams}
-        logging.info(f"returning request {output}")
         return output
```

### Comparing `log10_io-0.1.0/log10/tools.py` & `log10_io-0.2.1/log10/tools.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/log10/utils.py` & `log10_io-0.2.1/log10/utils.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/log10/agents/camel.py` & `log10_io-0.2.1/log10/agents/camel.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/log10/agents/scrape_summarizer.py` & `log10_io-0.2.1/log10/agents/scrape_summarizer.py`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/log10/schemas/bigquery.json` & `log10_io-0.2.1/log10/schemas/bigquery.json`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/LICENSE` & `log10_io-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/README.md` & `log10_io-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `log10_io-0.1.0/pyproject.toml` & `log10_io-0.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "log10-io"
-version = "0.1.0"
+version = "0.2.1"
 authors = []
 license = "MIT"
 description = "Unified LLM data management"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `log10_io-0.1.0/PKG-INFO` & `log10_io-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log10-io
-Version: 0.1.0
+Version: 0.2.1
 Summary: Unified LLM data management
 Project-URL: Homepage, https://github.com/log10-io/log10
 Project-URL: Bug Tracker, https://github.com/log10-io/log10/issues
 License-Expression: MIT
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

