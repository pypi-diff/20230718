# Comparing `tmp/idoctorai-0.7.5.tar.gz` & `tmp/idoctorai-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idoctorai-0.7.5.tar", max compression
+gzip compressed data, was "idoctorai-0.7.6.tar", max compression
```

## Comparing `idoctorai-0.7.5.tar` & `idoctorai-0.7.6.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.7.5/LICENSE
--rw-r--r--   0        0        0    27932 2023-07-17 07:58:43.438913 idoctorai-0.7.5/pandasai/__init__.py
--rw-r--r--   0        0        0     1318 2023-07-07 01:08:43.311575 idoctorai-0.7.5/pandasai/constants.py
--rw-r--r--   0        0        0     1582 2023-07-07 01:01:47.982275 idoctorai-0.7.5/pandasai/exceptions.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.7.5/pandasai/helpers/__init__.py
--rw-r--r--   0        0        0     3940 2023-07-07 01:01:47.982275 idoctorai-0.7.5/pandasai/helpers/_optional.py
--rw-r--r--   0        0        0     5613 2023-07-07 01:01:47.983273 idoctorai-0.7.5/pandasai/helpers/anonymizer.py
--rw-r--r--   0        0        0     1812 2023-07-07 01:01:47.984270 idoctorai-0.7.5/pandasai/helpers/cache.py
--rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.7.5/pandasai/helpers/from_excel.py
--rw-r--r--   0        0        0     1542 2023-07-07 01:01:47.984270 idoctorai-0.7.5/pandasai/helpers/notebook.py
--rw-r--r--   0        0        0     3635 2023-07-17 07:57:55.760373 idoctorai-0.7.5/pandasai/helpers/save_chart.py
--rw-r--r--   0        0        0    10287 2023-07-07 01:01:47.985267 idoctorai-0.7.5/pandasai/helpers/shortcuts.py
--rw-r--r--   0        0        0     4643 2023-07-08 01:22:44.839806 idoctorai-0.7.5/pandasai/langchain/__init__.py
--rw-r--r--   0        0        0       68 2023-07-17 02:43:35.387669 idoctorai-0.7.5/pandasai/langchain/agents.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.7.5/pandasai/llm/__init__.py
--rw-r--r--   0        0        0     4466 2023-07-07 01:01:47.986265 idoctorai-0.7.5/pandasai/llm/azure_openai.py
--rw-r--r--   0        0        0    14051 2023-07-12 13:05:59.808678 idoctorai-0.7.5/pandasai/llm/base.py
--rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.7.5/pandasai/llm/fake.py
--rw-r--r--   0        0        0     1264 2023-07-07 01:01:47.986265 idoctorai-0.7.5/pandasai/llm/falcon.py
--rw-r--r--   0        0        0     4609 2023-07-07 01:01:47.986265 idoctorai-0.7.5/pandasai/llm/google_palm.py
--rw-r--r--   0        0        0      599 2023-07-07 01:01:47.987262 idoctorai-0.7.5/pandasai/llm/langchain.py
--rw-r--r--   0        0        0     4154 2023-07-07 14:00:39.632140 idoctorai-0.7.5/pandasai/llm/model.py
--rw-r--r--   0        0        0     1535 2023-07-07 01:01:47.988259 idoctorai-0.7.5/pandasai/llm/open_assistant.py
--rw-r--r--   0        0        0     3599 2023-07-07 14:00:39.633137 idoctorai-0.7.5/pandasai/llm/openai.py
--rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.7.5/pandasai/llm/starcoder.py
--rw-r--r--   0        0        0        0 2023-07-07 01:01:47.988259 idoctorai-0.7.5/pandasai/middlewares/__init__.py
--rw-r--r--   0        0        0      693 2023-07-07 01:01:47.988259 idoctorai-0.7.5/pandasai/middlewares/base.py
--rw-r--r--   0        0        0      986 2023-07-07 01:01:47.989256 idoctorai-0.7.5/pandasai/middlewares/charts.py
--rw-r--r--   0        0        0      678 2023-07-07 01:01:47.989256 idoctorai-0.7.5/pandasai/middlewares/streamlit.py
--rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.7.5/pandasai/prompts/__init__.py
--rw-r--r--   0        0        0      674 2023-07-07 01:01:47.990254 idoctorai-0.7.5/pandasai/prompts/base.py
--rw-r--r--   0        0        0     1349 2023-07-07 14:00:39.634134 idoctorai-0.7.5/pandasai/prompts/correct_error_prompt.py
--rw-r--r--   0        0        0     1125 2023-07-07 14:00:39.635132 idoctorai-0.7.5/pandasai/prompts/correct_multiples_prompt.py
--rw-r--r--   0        0        0     1295 2023-07-07 14:00:39.636130 idoctorai-0.7.5/pandasai/prompts/generate_python_code.py
--rw-r--r--   0        0        0      482 2023-07-07 01:01:47.990254 idoctorai-0.7.5/pandasai/prompts/generate_response.py
--rw-r--r--   0        0        0     1339 2023-07-07 14:00:39.637343 idoctorai-0.7.5/pandasai/prompts/multiple_dataframes.py
--rw-r--r--   0        0        0     2064 2023-07-17 03:29:32.558699 idoctorai-0.7.5/pyproject.toml
--rw-r--r--   0        0        0       96 2023-07-07 14:00:39.620963 idoctorai-0.7.5/README.md
--rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 idoctorai-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-31 07:10:59.339636 idoctorai-0.7.6/LICENSE
+-rw-r--r--   0        0        0    27947 2023-07-18 12:42:54.467639 idoctorai-0.7.6/pandasai/__init__.py
+-rw-r--r--   0        0        0     1318 2023-07-07 01:08:43.311575 idoctorai-0.7.6/pandasai/constants.py
+-rw-r--r--   0        0        0     1582 2023-07-07 01:01:47.982275 idoctorai-0.7.6/pandasai/exceptions.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.362575 idoctorai-0.7.6/pandasai/helpers/__init__.py
+-rw-r--r--   0        0        0     3940 2023-07-07 01:01:47.982275 idoctorai-0.7.6/pandasai/helpers/_optional.py
+-rw-r--r--   0        0        0     5613 2023-07-07 01:01:47.983273 idoctorai-0.7.6/pandasai/helpers/anonymizer.py
+-rw-r--r--   0        0        0     1812 2023-07-07 01:01:47.984270 idoctorai-0.7.6/pandasai/helpers/cache.py
+-rw-r--r--   0        0        0      590 2023-06-07 12:25:21.036958 idoctorai-0.7.6/pandasai/helpers/from_excel.py
+-rw-r--r--   0        0        0     1542 2023-07-07 01:01:47.984270 idoctorai-0.7.6/pandasai/helpers/notebook.py
+-rw-r--r--   0        0        0     3635 2023-07-17 07:57:55.760373 idoctorai-0.7.6/pandasai/helpers/save_chart.py
+-rw-r--r--   0        0        0    10287 2023-07-07 01:01:47.985267 idoctorai-0.7.6/pandasai/helpers/shortcuts.py
+-rw-r--r--   0        0        0     4643 2023-07-08 01:22:44.839806 idoctorai-0.7.6/pandasai/langchain/__init__.py
+-rw-r--r--   0        0        0       68 2023-07-17 02:43:35.387669 idoctorai-0.7.6/pandasai/langchain/agents.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.364569 idoctorai-0.7.6/pandasai/llm/__init__.py
+-rw-r--r--   0        0        0     4466 2023-07-07 01:01:47.986265 idoctorai-0.7.6/pandasai/llm/azure_openai.py
+-rw-r--r--   0        0        0    14051 2023-07-12 13:05:59.808678 idoctorai-0.7.6/pandasai/llm/base.py
+-rw-r--r--   0        0        0      566 2023-05-31 07:10:59.366593 idoctorai-0.7.6/pandasai/llm/fake.py
+-rw-r--r--   0        0        0     1264 2023-07-07 01:01:47.986265 idoctorai-0.7.6/pandasai/llm/falcon.py
+-rw-r--r--   0        0        0     4609 2023-07-07 01:01:47.986265 idoctorai-0.7.6/pandasai/llm/google_palm.py
+-rw-r--r--   0        0        0      599 2023-07-07 01:01:47.987262 idoctorai-0.7.6/pandasai/llm/langchain.py
+-rw-r--r--   0        0        0     4154 2023-07-07 14:00:39.632140 idoctorai-0.7.6/pandasai/llm/model.py
+-rw-r--r--   0        0        0     1535 2023-07-07 01:01:47.988259 idoctorai-0.7.6/pandasai/llm/open_assistant.py
+-rw-r--r--   0        0        0     3599 2023-07-07 14:00:39.633137 idoctorai-0.7.6/pandasai/llm/openai.py
+-rw-r--r--   0        0        0     1269 2023-05-31 07:10:59.368559 idoctorai-0.7.6/pandasai/llm/starcoder.py
+-rw-r--r--   0        0        0        0 2023-07-07 01:01:47.988259 idoctorai-0.7.6/pandasai/middlewares/__init__.py
+-rw-r--r--   0        0        0      693 2023-07-07 01:01:47.988259 idoctorai-0.7.6/pandasai/middlewares/base.py
+-rw-r--r--   0        0        0      986 2023-07-07 01:01:47.989256 idoctorai-0.7.6/pandasai/middlewares/charts.py
+-rw-r--r--   0        0        0      678 2023-07-07 01:01:47.989256 idoctorai-0.7.6/pandasai/middlewares/streamlit.py
+-rw-r--r--   0        0        0        0 2023-05-31 07:10:59.368559 idoctorai-0.7.6/pandasai/prompts/__init__.py
+-rw-r--r--   0        0        0      674 2023-07-07 01:01:47.990254 idoctorai-0.7.6/pandasai/prompts/base.py
+-rw-r--r--   0        0        0     1349 2023-07-07 14:00:39.634134 idoctorai-0.7.6/pandasai/prompts/correct_error_prompt.py
+-rw-r--r--   0        0        0     1125 2023-07-07 14:00:39.635132 idoctorai-0.7.6/pandasai/prompts/correct_multiples_prompt.py
+-rw-r--r--   0        0        0     1295 2023-07-07 14:00:39.636130 idoctorai-0.7.6/pandasai/prompts/generate_python_code.py
+-rw-r--r--   0        0        0      482 2023-07-07 01:01:47.990254 idoctorai-0.7.6/pandasai/prompts/generate_response.py
+-rw-r--r--   0        0        0     1339 2023-07-07 14:00:39.637343 idoctorai-0.7.6/pandasai/prompts/multiple_dataframes.py
+-rw-r--r--   0        0        0     2064 2023-07-18 12:43:18.585198 idoctorai-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0       96 2023-07-07 14:00:39.620963 idoctorai-0.7.6/README.md
+-rw-r--r--   0        0        0     1630 1970-01-01 00:00:00.000000 idoctorai-0.7.6/PKG-INFO
```

### Comparing `idoctorai-0.7.5/LICENSE` & `idoctorai-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/__init__.py` & `idoctorai-0.7.6/pandasai/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -630,15 +630,15 @@
                 error_returned=e,
                 question=self._original_instructions["question"],
                 df_head=self._original_instructions["df_head"],
                 num_rows=self._original_instructions["num_rows"],
                 num_columns=self._original_instructions["num_columns"],
             )
 
-        return self._llm.generate_code(error_correcting_instruction, "")
+        return self._llm.generate_code(error_correcting_instruction, "", self._history)
 
     def run_code(
         self,
         code: str,
         data_frame: pd.DataFrame,
         use_error_correction_framework: bool = True,
     ) -> str:
```

### Comparing `idoctorai-0.7.5/pandasai/constants.py` & `idoctorai-0.7.6/pandasai/constants.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/exceptions.py` & `idoctorai-0.7.6/pandasai/exceptions.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/helpers/_optional.py` & `idoctorai-0.7.6/pandasai/helpers/_optional.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/helpers/anonymizer.py` & `idoctorai-0.7.6/pandasai/helpers/anonymizer.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/helpers/cache.py` & `idoctorai-0.7.6/pandasai/helpers/cache.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/helpers/from_excel.py` & `idoctorai-0.7.6/pandasai/helpers/from_excel.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/helpers/notebook.py` & `idoctorai-0.7.6/pandasai/helpers/notebook.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/helpers/save_chart.py` & `idoctorai-0.7.6/pandasai/helpers/save_chart.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/helpers/shortcuts.py` & `idoctorai-0.7.6/pandasai/helpers/shortcuts.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/langchain/__init__.py` & `idoctorai-0.7.6/pandasai/langchain/__init__.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/llm/azure_openai.py` & `idoctorai-0.7.6/pandasai/llm/azure_openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/llm/base.py` & `idoctorai-0.7.6/pandasai/llm/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/llm/fake.py` & `idoctorai-0.7.6/pandasai/llm/fake.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/llm/falcon.py` & `idoctorai-0.7.6/pandasai/llm/falcon.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/llm/google_palm.py` & `idoctorai-0.7.6/pandasai/llm/google_palm.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/llm/langchain.py` & `idoctorai-0.7.6/pandasai/llm/langchain.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/llm/model.py` & `idoctorai-0.7.6/pandasai/llm/model.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/llm/open_assistant.py` & `idoctorai-0.7.6/pandasai/llm/open_assistant.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/llm/openai.py` & `idoctorai-0.7.6/pandasai/llm/openai.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/llm/starcoder.py` & `idoctorai-0.7.6/pandasai/llm/starcoder.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/middlewares/base.py` & `idoctorai-0.7.6/pandasai/middlewares/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/middlewares/charts.py` & `idoctorai-0.7.6/pandasai/middlewares/charts.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/middlewares/streamlit.py` & `idoctorai-0.7.6/pandasai/middlewares/streamlit.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/prompts/base.py` & `idoctorai-0.7.6/pandasai/prompts/base.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/prompts/correct_error_prompt.py` & `idoctorai-0.7.6/pandasai/prompts/correct_error_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/prompts/correct_multiples_prompt.py` & `idoctorai-0.7.6/pandasai/prompts/correct_multiples_prompt.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/prompts/generate_python_code.py` & `idoctorai-0.7.6/pandasai/prompts/generate_python_code.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pandasai/prompts/multiple_dataframes.py` & `idoctorai-0.7.6/pandasai/prompts/multiple_dataframes.py`

 * *Files identical despite different names*

### Comparing `idoctorai-0.7.5/pyproject.toml` & `idoctorai-0.7.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "idoctorai"
-version = "0.7.5"
+version = "0.7.6"
 description = "Idoctor AI is a Python library that integrates generative artificial intelligence capabilities into Pandas."
 authors = ["FH"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pandasai"}]
 
 [tool.poetry.dependencies]
```

### Comparing `idoctorai-0.7.5/PKG-INFO` & `idoctorai-0.7.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idoctorai
-Version: 0.7.5
+Version: 0.7.6
 Summary: Idoctor AI is a Python library that integrates generative artificial intelligence capabilities into Pandas.
 License: MIT
 Author: FH
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
```

