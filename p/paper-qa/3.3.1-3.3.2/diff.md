# Comparing `tmp/paper-qa-3.3.1.tar.gz` & `tmp/paper-qa-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paper-qa-3.3.1.tar", last modified: Sat Jul 15 05:00:01 2023, max compression
+gzip compressed data, was "paper-qa-3.3.2.tar", last modified: Tue Jul 18 19:25:11 2023, max compression
```

## Comparing `paper-qa-3.3.1.tar` & `paper-qa-3.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:00:01.616127 paper-qa-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-15 04:59:24.000000 paper-qa-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-15 05:00:01.616127 paper-qa-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-15 04:59:24.000000 paper-qa-3.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:00:01.612127 paper-qa-3.3.1/paper_qa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-15 05:00:01.000000 paper-qa-3.3.1/paper_qa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-15 05:00:01.000000 paper-qa-3.3.1/paper_qa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 05:00:01.000000 paper-qa-3.3.1/paper_qa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-15 05:00:01.000000 paper-qa-3.3.1/paper_qa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-15 05:00:01.000000 paper-qa-3.3.1/paper_qa.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:00:01.616127 paper-qa-3.3.1/paperqa/
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/chains.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:00:01.616127 paper-qa-3.3.1/paperqa/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/contrib/zotero.py
--rw-r--r--   0 runner    (1001) docker     (123)    23494 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/docs.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/paths.py
--rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/prompts.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3761 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-15 04:59:24.000000 paper-qa-3.3.1/paperqa/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 05:00:01.616127 paper-qa-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-15 04:59:24.000000 paper-qa-3.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 05:00:01.616127 paper-qa-3.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    27622 2023-07-15 04:59:25.000000 paper-qa-3.3.1/tests/test_paperqa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:25:11.612240 paper-qa-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 19:24:26.000000 paper-qa-3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-18 19:25:11.612240 paper-qa-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    17701 2023-07-18 19:24:26.000000 paper-qa-3.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:25:11.608240 paper-qa-3.3.2/paper_qa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 2023-07-18 19:25:11.000000 paper-qa-3.3.2/paper_qa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-18 19:25:11.000000 paper-qa-3.3.2/paper_qa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:25:11.000000 paper-qa-3.3.2/paper_qa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-07-18 19:25:11.000000 paper-qa-3.3.2/paper_qa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 19:25:11.000000 paper-qa-3.3.2/paper_qa.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:25:11.612240 paper-qa-3.3.2/paperqa/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/chains.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:25:11.612240 paper-qa-3.3.2/paperqa/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12316 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/contrib/zotero.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23494 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/docs.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/paths.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2234 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/prompts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3892 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 19:24:26.000000 paper-qa-3.3.2/paperqa/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:25:11.612240 paper-qa-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-18 19:24:26.000000 paper-qa-3.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:25:11.612240 paper-qa-3.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    27622 2023-07-18 19:24:26.000000 paper-qa-3.3.2/tests/test_paperqa.py
```

### Comparing `paper-qa-3.3.1/LICENSE` & `paper-qa-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.1/PKG-INFO` & `paper-qa-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.3.1
+Version: 3.3.2
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.3.1/README.md` & `paper-qa-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.1/paper_qa.egg-info/PKG-INFO` & `paper-qa-3.3.2/paper_qa.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paper-qa
-Version: 3.3.1
+Version: 3.3.2
 Summary: LLM Chain for answering questions from docs 
 Home-page: https://github.com/whitead/paper-qa
 Author: Andrew White
 Author-email: white.d.andrew@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `paper-qa-3.3.1/paperqa/chains.py` & `paper-qa-3.3.2/paperqa/chains.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.1/paperqa/contrib/zotero.py` & `paper-qa-3.3.2/paperqa/contrib/zotero.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.1/paperqa/docs.py` & `paper-qa-3.3.2/paperqa/docs.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.1/paperqa/prompts.py` & `paper-qa-3.3.2/paperqa/prompts.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.1/paperqa/readers.py` & `paper-qa-3.3.2/paperqa/readers.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.1/paperqa/types.py` & `paper-qa-3.3.2/paperqa/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from langchain.callbacks.base import BaseCallbackHandler
 from langchain.callbacks.manager import (
     AsyncCallbackManagerForChainRun,
     CallbackManagerForChainRun,
 )
 from langchain.prompts import PromptTemplate
-from pydantic import BaseModel, validator
+from pydantic import BaseModel, Field, validator
 
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
-    summary: PromptTemplate = summary_prompt
-    qa: PromptTemplate = qa_prompt
-    select: PromptTemplate = select_paper_prompt
-    cite: PromptTemplate = citation_prompt
+    summary: PromptTemplate = Field(default_factory=lambda: summary_prompt)
+    qa: PromptTemplate = Field(default_factory=lambda: qa_prompt)
+    select: PromptTemplate = Field(default_factory=lambda: select_paper_prompt)
+    cite: PromptTemplate = Field(default_factory=lambda: citation_prompt)
     pre: Optional[PromptTemplate] = None
     post: Optional[PromptTemplate] = None
 
     @validator("summary")
     def check_summary(cls, v: PromptTemplate) -> PromptTemplate:
         if not set(v.input_variables).issubset(set(summary_prompt.input_variables)):
             raise ValueError(
```

### Comparing `paper-qa-3.3.1/paperqa/utils.py` & `paper-qa-3.3.2/paperqa/utils.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.1/setup.py` & `paper-qa-3.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `paper-qa-3.3.1/tests/test_paperqa.py` & `paper-qa-3.3.2/tests/test_paperqa.py`

 * *Files identical despite different names*

