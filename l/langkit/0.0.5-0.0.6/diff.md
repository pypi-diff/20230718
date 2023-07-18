# Comparing `tmp/langkit-0.0.5.tar.gz` & `tmp/langkit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langkit-0.0.5.tar", max compression
+gzip compressed data, was "langkit-0.0.6.tar", max compression
```

## Comparing `langkit-0.0.5.tar` & `langkit-0.0.6.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0     3205 2023-07-04 20:10:20.545540 langkit-0.0.5/DESCRIPTION.md
--rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.5/LICENSE
--rw-r--r--   0        0        0      998 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/__init__.py
--rw-r--r--   0        0        0      596 2023-07-06 08:00:05.378422 langkit-0.0.5/langkit/all_metrics.py
--rw-r--r--   0        0        0     7915 2023-07-11 19:04:26.469567 langkit-0.0.5/langkit/callback_handler.py
--rw-r--r--   0        0        0      140 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/config/__init__.py
--rw-r--r--   0        0        0     1757 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/config/environment.py
--rw-r--r--   0        0        0     1260 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/docs/features/quality.md
--rw-r--r--   0        0        0     1801 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/docs/features/relevance.md
--rw-r--r--   0        0        0     1886 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/docs/features/security.md
--rw-r--r--   0        0        0     1364 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/docs/features/sentiment.md
--rw-r--r--   0        0        0    11682 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/docs/modules.md
--rw-r--r--   0        0        0    11230 2023-07-04 20:11:04.055540 langkit-0.0.5/langkit/examples/Batch_to_Whylabs.ipynb
--rw-r--r--   0        0        0     9718 2023-07-07 22:44:08.578422 langkit-0.0.5/langkit/examples/Intro_to_Langkit.ipynb
--rw-r--r--   0        0        0   262944 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/examples/LLM_to_WhyLabs.ipynb
--rw-r--r--   0        0        0    11770 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb
--rw-r--r--   0        0        0    21888 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/examples/Logging_Text.ipynb
--rw-r--r--   0        0        0     7126 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/examples/Sentiment_and_Toxicity.ipynb
--rw-r--r--   0        0        0    17842 2023-07-07 22:52:41.688422 langkit-0.0.5/langkit/examples/tutorials/Safeguarding_and_Monitoring_LLMs.ipynb
--rw-r--r--   0        0        0   109092 2023-07-07 22:52:41.698422 langkit-0.0.5/langkit/examples/tutorials/images/dashboard.png
--rw-r--r--   0        0        0   336393 2023-07-07 22:52:41.698422 langkit-0.0.5/langkit/examples/tutorials/images/safeguards_pipeline.png
--rw-r--r--   0        0        0     1362 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/injections.py
--rw-r--r--   0        0        0     2210 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/input_output.py
--rw-r--r--   0        0        0      297 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/light_metrics.py
--rw-r--r--   0        0        0      730 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/llm_metrics.py
--rw-r--r--   0        0        0       75 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/openai/__init__.py
--rw-r--r--   0        0        0     1167 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/openai/openai.py
--rw-r--r--   0        0        0     1741 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/openai_wrapper.py
--rw-r--r--   0        0        0      793 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/pattern_groups.json
--rw-r--r--   0        0        0     2938 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/regexes.py
--rw-r--r--   0        0        0      943 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/sentiment.py
--rw-r--r--   0        0        0      998 2023-07-11 19:04:26.469567 langkit-0.0.5/langkit/tests/__init__.py
--rw-r--r--   0        0        0     3970 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/tests/conftest.py
--rw-r--r--   0        0        0     4407 2023-07-11 19:04:26.469567 langkit-0.0.5/langkit/tests/test_callback_handler.py
--rw-r--r--   0        0        0     1078 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/tests/test_injections.py
--rw-r--r--   0        0        0     2308 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/tests/test_input_output.py
--rw-r--r--   0        0        0     2150 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/tests/test_patterns.py
--rw-r--r--   0        0        0     3658 2023-07-11 19:04:26.469567 langkit-0.0.5/langkit/tests/test_themes.py
--rw-r--r--   0        0        0      798 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/tests/test_toxicity.py
--rw-r--r--   0        0        0     3742 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/textstat.py
--rw-r--r--   0        0        0     8939 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/themes.json
--rw-r--r--   0        0        0      261 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/themes.json.txt
--rw-r--r--   0        0        0     4183 2023-07-11 19:04:26.469567 langkit-0.0.5/langkit/themes.py
--rw-r--r--   0        0        0      679 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/topics.py
--rw-r--r--   0        0        0     1305 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/toxicity.py
--rw-r--r--   0        0        0      144 2023-07-04 20:11:04.065540 langkit-0.0.5/langkit/transformer.py
--rw-r--r--   0        0        0     1159 2023-07-11 19:04:26.469567 langkit-0.0.5/langkit/whylogs/example_utils/guardrails_example_utils.py
--rw-r--r--   0        0        0     6609 2023-07-07 22:52:41.698422 langkit-0.0.5/langkit/whylogs/example_utils/guardrails_llm_schema.py
--rw-r--r--   0        0        0    30472 2023-07-04 20:11:04.075540 langkit-0.0.5/langkit/whylogs/reference_chats.json
--rw-r--r--   0        0        0      474 2023-07-04 20:11:04.075540 langkit-0.0.5/langkit/whylogs/rolling_logger.py
--rw-r--r--   0        0        0      993 2023-07-04 20:11:04.075540 langkit-0.0.5/langkit/whylogs/samples.py
--rw-r--r--   0        0        0      900 2023-07-11 19:04:26.469567 langkit-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 langkit-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     3205 2023-07-04 20:10:20.545540 langkit-0.0.6/DESCRIPTION.md
+-rw-r--r--   0        0        0    11357 2023-04-27 19:37:47.238351 langkit-0.0.6/LICENSE
+-rw-r--r--   0        0        0      998 2023-07-12 19:53:12.139567 langkit-0.0.6/langkit/__init__.py
+-rw-r--r--   0        0        0      596 2023-07-06 08:00:05.378422 langkit-0.0.6/langkit/all_metrics.py
+-rw-r--r--   0        0        0     7915 2023-07-12 20:36:17.619567 langkit-0.0.6/langkit/callback_handler.py
+-rw-r--r--   0        0        0      140 2023-07-04 20:11:04.055540 langkit-0.0.6/langkit/config/__init__.py
+-rw-r--r--   0        0        0     1757 2023-07-04 20:11:04.055540 langkit-0.0.6/langkit/config/environment.py
+-rw-r--r--   0        0        0     1260 2023-07-04 20:11:04.055540 langkit-0.0.6/langkit/docs/features/quality.md
+-rw-r--r--   0        0        0     1801 2023-07-04 20:11:04.055540 langkit-0.0.6/langkit/docs/features/relevance.md
+-rw-r--r--   0        0        0     1886 2023-07-04 20:11:04.055540 langkit-0.0.6/langkit/docs/features/security.md
+-rw-r--r--   0        0        0     1364 2023-07-04 20:11:04.055540 langkit-0.0.6/langkit/docs/features/sentiment.md
+-rw-r--r--   0        0        0    11682 2023-07-04 20:11:04.055540 langkit-0.0.6/langkit/docs/modules.md
+-rw-r--r--   0        0        0    11230 2023-07-04 20:11:04.055540 langkit-0.0.6/langkit/examples/Batch_to_Whylabs.ipynb
+-rw-r--r--   0        0        0     9709 2023-07-12 20:36:17.619567 langkit-0.0.6/langkit/examples/Intro_to_Langkit.ipynb
+-rw-r--r--   0        0        0   262944 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/examples/LLM_to_WhyLabs.ipynb
+-rw-r--r--   0        0        0    11770 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb
+-rw-r--r--   0        0        0    21888 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/examples/Logging_Text.ipynb
+-rw-r--r--   0        0        0     7126 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/examples/Sentiment_and_Toxicity.ipynb
+-rw-r--r--   0        0        0    17842 2023-07-07 22:52:41.688422 langkit-0.0.6/langkit/examples/tutorials/Safeguarding_and_Monitoring_LLMs.ipynb
+-rw-r--r--   0        0        0   109092 2023-07-07 22:52:41.698422 langkit-0.0.6/langkit/examples/tutorials/images/dashboard.png
+-rw-r--r--   0        0        0   336393 2023-07-07 22:52:41.698422 langkit-0.0.6/langkit/examples/tutorials/images/safeguards_pipeline.png
+-rw-r--r--   0        0        0     1362 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/injections.py
+-rw-r--r--   0        0        0     2210 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/input_output.py
+-rw-r--r--   0        0        0      297 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/light_metrics.py
+-rw-r--r--   0        0        0      730 2023-07-12 19:53:33.919567 langkit-0.0.6/langkit/llm_metrics.py
+-rw-r--r--   0        0        0       75 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/openai/__init__.py
+-rw-r--r--   0        0        0     1167 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/openai/openai.py
+-rw-r--r--   0        0        0     1741 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/openai_wrapper.py
+-rw-r--r--   0        0        0      793 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/pattern_groups.json
+-rw-r--r--   0        0        0     2938 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/regexes.py
+-rw-r--r--   0        0        0      943 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/sentiment.py
+-rw-r--r--   0        0        0      998 2023-07-12 20:36:17.619567 langkit-0.0.6/langkit/tests/__init__.py
+-rw-r--r--   0        0        0     3970 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/tests/conftest.py
+-rw-r--r--   0        0        0     4407 2023-07-12 20:36:17.619567 langkit-0.0.6/langkit/tests/test_callback_handler.py
+-rw-r--r--   0        0        0     1078 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/tests/test_injections.py
+-rw-r--r--   0        0        0     2308 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/tests/test_input_output.py
+-rw-r--r--   0        0        0     2150 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/tests/test_patterns.py
+-rw-r--r--   0        0        0     3658 2023-07-11 19:04:26.469567 langkit-0.0.6/langkit/tests/test_themes.py
+-rw-r--r--   0        0        0      798 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/tests/test_toxicity.py
+-rw-r--r--   0        0        0     3742 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/textstat.py
+-rw-r--r--   0        0        0     8939 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/themes.json
+-rw-r--r--   0        0        0      261 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/themes.json.txt
+-rw-r--r--   0        0        0     4183 2023-07-11 19:04:26.469567 langkit-0.0.6/langkit/themes.py
+-rw-r--r--   0        0        0      679 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/topics.py
+-rw-r--r--   0        0        0     1305 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/toxicity.py
+-rw-r--r--   0        0        0      144 2023-07-04 20:11:04.065540 langkit-0.0.6/langkit/transformer.py
+-rw-r--r--   0        0        0     1159 2023-07-12 20:36:17.619567 langkit-0.0.6/langkit/whylogs/example_utils/guardrails_example_utils.py
+-rw-r--r--   0        0        0     6609 2023-07-07 22:52:41.698422 langkit-0.0.6/langkit/whylogs/example_utils/guardrails_llm_schema.py
+-rw-r--r--   0        0        0    30472 2023-07-04 20:11:04.075540 langkit-0.0.6/langkit/whylogs/reference_chats.json
+-rw-r--r--   0        0        0      474 2023-07-04 20:11:04.075540 langkit-0.0.6/langkit/whylogs/rolling_logger.py
+-rw-r--r--   0        0        0      993 2023-07-04 20:11:04.075540 langkit-0.0.6/langkit/whylogs/samples.py
+-rw-r--r--   0        0        0      900 2023-07-12 20:36:17.619567 langkit-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4204 1970-01-01 00:00:00.000000 langkit-0.0.6/PKG-INFO
```

### Comparing `langkit-0.0.5/DESCRIPTION.md` & `langkit-0.0.6/DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/LICENSE` & `langkit-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/__init__.py` & `langkit-0.0.6/langkit/__init__.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/all_metrics.py` & `langkit-0.0.6/langkit/all_metrics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/callback_handler.py` & `langkit-0.0.6/langkit/callback_handler.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/config/environment.py` & `langkit-0.0.6/langkit/config/environment.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/docs/features/quality.md` & `langkit-0.0.6/langkit/docs/features/quality.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/docs/features/relevance.md` & `langkit-0.0.6/langkit/docs/features/relevance.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/docs/features/security.md` & `langkit-0.0.6/langkit/docs/features/security.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/docs/features/sentiment.md` & `langkit-0.0.6/langkit/docs/features/sentiment.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/docs/modules.md` & `langkit-0.0.6/langkit/docs/modules.md`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/examples/Batch_to_Whylabs.ipynb` & `langkit-0.0.6/langkit/examples/Batch_to_Whylabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/examples/Intro_to_Langkit.ipynb` & `langkit-0.0.6/langkit/examples/Intro_to_Langkit.ipynb`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982589285714285%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(1, '%pip install -U langkit[all]\\n')], delete: [1]}}}",*

 * * "'metadata'": "{'language_info': {'version': '3.8.10'}}"}*

```diff
@@ -32,15 +32,15 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "metadata": {},
             "outputs": [],
             "source": [
                 "# Note: you may need to restart the kernel to use updated packages.\n",
-                "%pip install 'langkit[all]==0.0.1' -q\n",
+                "%pip install -U langkit[all]\n",
                 "%pip install xformers ipywidgets -q\n"
             ]
         },
         {
             "attachments": {},
             "cell_type": "markdown",
             "metadata": {},
@@ -222,15 +222,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.11.2"
+            "version": "3.8.10"
         },
         "orig_nbformat": 4,
         "vscode": {
             "interpreter": {
                 "hash": "b0fa6594d8f4cbf19f97940f81e996739fb7646882a419484c72d19e05852a7e"
             }
         }
```

### Comparing `langkit-0.0.5/langkit/examples/LLM_to_WhyLabs.ipynb` & `langkit-0.0.6/langkit/examples/LLM_to_WhyLabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb` & `langkit-0.0.6/langkit/examples/Langchain_OpenAI_LLM_Monitoring_with_WhyLabs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/examples/Logging_Text.ipynb` & `langkit-0.0.6/langkit/examples/Logging_Text.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/examples/Sentiment_and_Toxicity.ipynb` & `langkit-0.0.6/langkit/examples/Sentiment_and_Toxicity.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/examples/tutorials/Safeguarding_and_Monitoring_LLMs.ipynb` & `langkit-0.0.6/langkit/examples/tutorials/Safeguarding_and_Monitoring_LLMs.ipynb`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/examples/tutorials/images/dashboard.png` & `langkit-0.0.6/langkit/examples/tutorials/images/dashboard.png`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/examples/tutorials/images/safeguards_pipeline.png` & `langkit-0.0.6/langkit/examples/tutorials/images/safeguards_pipeline.png`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/injections.py` & `langkit-0.0.6/langkit/injections.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/input_output.py` & `langkit-0.0.6/langkit/input_output.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/llm_metrics.py` & `langkit-0.0.6/langkit/llm_metrics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/openai/openai.py` & `langkit-0.0.6/langkit/openai/openai.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/openai_wrapper.py` & `langkit-0.0.6/langkit/openai_wrapper.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/pattern_groups.json` & `langkit-0.0.6/langkit/pattern_groups.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/regexes.py` & `langkit-0.0.6/langkit/regexes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/sentiment.py` & `langkit-0.0.6/langkit/sentiment.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/tests/__init__.py` & `langkit-0.0.6/langkit/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/tests/conftest.py` & `langkit-0.0.6/langkit/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/tests/test_callback_handler.py` & `langkit-0.0.6/langkit/tests/test_callback_handler.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/tests/test_injections.py` & `langkit-0.0.6/langkit/tests/test_injections.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/tests/test_input_output.py` & `langkit-0.0.6/langkit/tests/test_input_output.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/tests/test_patterns.py` & `langkit-0.0.6/langkit/tests/test_patterns.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/tests/test_themes.py` & `langkit-0.0.6/langkit/tests/test_themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/tests/test_toxicity.py` & `langkit-0.0.6/langkit/tests/test_toxicity.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/textstat.py` & `langkit-0.0.6/langkit/textstat.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/themes.json` & `langkit-0.0.6/langkit/themes.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/themes.py` & `langkit-0.0.6/langkit/themes.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/topics.py` & `langkit-0.0.6/langkit/topics.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/toxicity.py` & `langkit-0.0.6/langkit/toxicity.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/whylogs/example_utils/guardrails_example_utils.py` & `langkit-0.0.6/langkit/whylogs/example_utils/guardrails_example_utils.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/whylogs/example_utils/guardrails_llm_schema.py` & `langkit-0.0.6/langkit/whylogs/example_utils/guardrails_llm_schema.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/whylogs/reference_chats.json` & `langkit-0.0.6/langkit/whylogs/reference_chats.json`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/langkit/whylogs/samples.py` & `langkit-0.0.6/langkit/whylogs/samples.py`

 * *Files identical despite different names*

### Comparing `langkit-0.0.5/pyproject.toml` & `langkit-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [tool.poetry]
 name = "langkit"
-version = "0.0.5"
+version = "0.0.6"
 description = "A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs"
 authors = ["WhyLabs.ai <langkit@whylabs.ai>"]
 license = "Apache-2.0"
 readme = "DESCRIPTION.md"
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-whylogs = {version = "^1.2.1"}
+whylogs = {version = "^1.2.3"}
 textstat = "^0.7.3"
 pandas = "*"
 
 
 # optional dependencies
 torch = {version = "*", optional = true}
 datasets = {version ="^2.12.0", optional = true}
```

### Comparing `langkit-0.0.5/PKG-INFO` & `langkit-0.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langkit
-Version: 0.0.5
+Version: 0.0.6
 Summary: A collection of text metric udfs for whylogs profiling and monitoring in WhyLabs
 License: Apache-2.0
 Author: WhyLabs.ai
 Author-email: langkit@whylabs.ai
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -16,15 +16,15 @@
 Requires-Dist: datasets (>=2.12.0,<3.0.0) ; extra == "all"
 Requires-Dist: nltk (>=3.8.1,<4.0.0) ; extra == "all"
 Requires-Dist: openai (>=0.27.6,<0.28.0) ; extra == "all"
 Requires-Dist: pandas
 Requires-Dist: sentence-transformers (>=2.2.2,<3.0.0) ; extra == "all"
 Requires-Dist: textstat (>=0.7.3,<0.8.0)
 Requires-Dist: torch ; extra == "all"
-Requires-Dist: whylogs (>=1.2.1,<2.0.0)
+Requires-Dist: whylogs (>=1.2.3,<2.0.0)
 Description-Content-Type: text/markdown
 
 LangKit is an open-source text metrics toolkit for monitoring language models. It offers an array of methods for extracting relevant signals from the input and/or output text, which are compatible with the open-source data logging library [whylogs](https://whylogs.readthedocs.io/en/latest).
 
 > 💡 Want to experience LangKit? Go to this [notebook](https://github.com/whylabs/langkit/blob/main/langkit/examples/Intro_to_Langkit.ipynb)!
 
 ## Table of Contents 📖
```

