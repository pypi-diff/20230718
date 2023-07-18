# Comparing `tmp/paper-qa-3.3.2.tar.gz` & `tmp/paper-qa-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-3.3.2.tar", last modified: Tue Jul 18 19:25:11 2023, max compression
+gzip compressed data, was "paper-qa-3.3.3.tar", last modified: Tue Jul 18 21:01:33 2023, max compression
```

## Comparing `paper-qa-3.3.2.tar` & `paper-qa-3.3.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:25:11.612240 paper-qa-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 19:24:26.000000 paper-qa-3.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-18 19:25:11.612240 paper-qa-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-18 19:24:26.000000 paper-qa-3.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:25:11.608240 paper-qa-3.3.2/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-18 19:25:11.000000 paper-qa-3.3.2/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-18 19:25:11.000000 paper-qa-3.3.2/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:25:11.000000 paper-qa-3.3.2/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-18 19:25:11.000000 paper-qa-3.3.2/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 19:25:11.000000 paper-qa-3.3.2/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:25:11.612240 paper-qa-3.3.2/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/chains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:25:11.612240 paper-qa-3.3.2/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    23494 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:25:11.612240 paper-qa-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-18 19:24:26.000000 paper-qa-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:25:11.612240 paper-qa-3.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    27622 2023-07-18 19:24:26.000000 paper-qa-3.3.2/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:01:33.657306 paper-qa-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 21:00:55.000000 paper-qa-3.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-18 21:01:33.653306 paper-qa-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-18 21:00:55.000000 paper-qa-3.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:01:33.649306 paper-qa-3.3.3/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-18 21:01:33.000000 paper-qa-3.3.3/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-18 21:01:33.000000 paper-qa-3.3.3/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 21:01:33.000000 paper-qa-3.3.3/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-18 21:01:33.000000 paper-qa-3.3.3/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 21:01:33.000000 paper-qa-3.3.3/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:01:33.653306 paper-qa-3.3.3/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:01:33.653306 paper-qa-3.3.3/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23494 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 21:00:55.000000 paper-qa-3.3.3/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 21:01:33.657306 paper-qa-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-18 21:00:55.000000 paper-qa-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:01:33.653306 paper-qa-3.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27622 2023-07-18 21:00:55.000000 paper-qa-3.3.3/tests/test_paperqa.py
```

### Comparing `paper-qa-3.3.2/LICENSE` & `paper-qa-3.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.2/PKG-INFO` & `paper-qa-3.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.3.2
+Version: 3.3.3
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.3.2/README.md` & `paper-qa-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.2/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.3.3/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.3.2
+Version: 3.3.3
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.3.2/paperqa/chains.py` & `paper-qa-3.3.3/paperqa/chains.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.2/paperqa/contrib/zotero.py` & `paper-qa-3.3.3/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.2/paperqa/docs.py` & `paper-qa-3.3.3/paperqa/docs.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.2/paperqa/prompts.py` & `paper-qa-3.3.3/paperqa/prompts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from datetime import datetime
-
 from langchain.prompts import PromptTemplate
 
 summary_prompt = PromptTemplate(
     input_variables=["text", "citation", "question", "summary_length"],
     template="Summarize the text below to help answer a question. "
     "Do not directly answer the question, instead summarize "
     "to give evidence to help answer the question. "
@@ -41,20 +39,15 @@
     "Choose papers that are relevant, from reputable sources, and timely "
     "(if the question requires timely information). \n\n"
     "Question: {question}\n\n"
     "{papers}\n\n"
     "Selected keys:",
 )
 
-
-def _get_datetime():
-    now = datetime.now()
-    return now.strftime("%m/%d/%Y")
-
-
+# We are unable to serialize with partial variables
+# so TODO: update year next year
 citation_prompt = PromptTemplate(
     input_variables=["text"],
-    template="Provide the citation for the following text in MLA Format. Today's date is {date}\n"
+    template="Provide the citation for the following text in MLA Format. The year is 2023\n"
     "{text}\n\n"
     "Citation:",
-    partial_variables={"date": _get_datetime},
 )
```

### Comparing `paper-qa-3.3.2/paperqa/readers.py` & `paper-qa-3.3.3/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.2/paperqa/types.py` & `paper-qa-3.3.3/paperqa/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from langchain.callbacks.base import BaseCallbackHandler
 from langchain.callbacks.manager import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
 )
 from langchain.prompts import PromptTemplate
-from pydantic import BaseModel, Field, validator
+from pydantic import BaseModel, validator
 
 from .prompts import citation_prompt, qa_prompt, select_paper_prompt, summary_prompt
 
 StrPath = Union[str, Path]
 DocKey = Any
 CBManager = Union[AsyncCallbackManagerForChainRun, CallbackManagerForChainRun]
 CallbackFactory = Callable[[str], Union[None, List[BaseCallbackHandler]]]
@@ -27,18 +27,18 @@
     text: str
     name: str
     doc: Doc
     embeddings: Optional[List[float]] = None
 
 
 class PromptCollection(BaseModel):
-    summary: PromptTemplate = Field(default_factory=lambda: summary_prompt)
-    qa: PromptTemplate = Field(default_factory=lambda: qa_prompt)
-    select: PromptTemplate = Field(default_factory=lambda: select_paper_prompt)
-    cite: PromptTemplate = Field(default_factory=lambda: citation_prompt)
+    summary: PromptTemplate = summary_prompt
+    qa: PromptTemplate = qa_prompt
+    select: PromptTemplate = select_paper_prompt
+    cite: PromptTemplate = citation_prompt
     pre: Optional[PromptTemplate] = None
     post: Optional[PromptTemplate] = None
 
     @validator("summary")
     def check_summary(cls, v: PromptTemplate) -> PromptTemplate:
         if not set(v.input_variables).issubset(set(summary_prompt.input_variables)):
             raise ValueError(
```

### Comparing `paper-qa-3.3.2/paperqa/utils.py` & `paper-qa-3.3.3/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.2/setup.py` & `paper-qa-3.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.2/tests/test_paperqa.py` & `paper-qa-3.3.3/tests/test_paperqa.py`

 * *Files identical despite different names*

