# Comparing `tmp/promptwatch-0.2.5.tar.gz` & `tmp/promptwatch-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promptwatch-0.2.5.tar", last modified: Fri Jul 14 21:46:30 2023, max compression
+gzip compressed data, was "promptwatch-0.2.6.tar", last modified: Tue Jul 18 16:08:39 2023, max compression
```

## Comparing `promptwatch-0.2.5.tar` & `promptwatch-0.2.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-14 21:46:30.647209 promptwatch-0.2.5/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-07-14 21:46:30.647000 promptwatch-0.2.5/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.2.5/README.md
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.2.5/pyproject.toml
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-07-14 21:46:30.647261 promptwatch-0.2.5/setup.cfg
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.2.5/setup.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-14 21:46:30.635634 promptwatch-0.2.5/src/
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-14 21:46:30.637903 promptwatch-0.2.5/src/promptwatch/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      442 2023-07-14 21:46:22.000000 promptwatch-0.2.5/src/promptwatch/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    16530 2023-05-31 21:34:19.000000 promptwatch-0.2.5/src/promptwatch/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     6257 2023-05-30 16:43:11.000000 promptwatch-0.2.5/src/promptwatch/client.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.2.5/src/promptwatch/constants.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     5282 2023-07-14 21:41:17.000000 promptwatch-0.2.5/src/promptwatch/data_model.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.2.5/src/promptwatch/decorators.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-14 21:46:30.642052 promptwatch-0.2.5/src/promptwatch/langchain/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.2.5/src/promptwatch/langchain/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    12414 2023-05-31 20:26:52.000000 promptwatch-0.2.5/src/promptwatch/langchain/caching.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    31317 2023-07-14 21:31:59.000000 promptwatch-0.2.5/src/promptwatch/langchain/langchain_support.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.2.5/src/promptwatch/langchain/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    18104 2023-06-15 22:09:53.000000 promptwatch-0.2.5/src/promptwatch/promptwatch_context.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-14 21:46:30.645444 promptwatch-0.2.5/src/promptwatch/unit_tests/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.2.5/src/promptwatch/unit_tests/__init__.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.2.5/src/promptwatch/unit_tests/evaluation.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.2.5/src/promptwatch/unit_tests/schema.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)    13645 2023-05-24 14:32:24.000000 promptwatch-0.2.5/src/promptwatch/unit_tests/unit_tests.py
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     2368 2023-06-17 16:42:18.000000 promptwatch-0.2.5/src/promptwatch/utils.py
-drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-14 21:46:30.640329 promptwatch-0.2.5/src/promptwatch.egg-info/
--rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-07-14 21:46:30.000000 promptwatch-0.2.5/src/promptwatch.egg-info/PKG-INFO
--rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-07-14 21:46:30.000000 promptwatch-0.2.5/src/promptwatch.egg-info/SOURCES.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-07-14 21:46:30.000000 promptwatch-0.2.5/src/promptwatch.egg-info/dependency_links.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.2.5/src/promptwatch.egg-info/not-zip-safe
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-07-14 21:46:30.000000 promptwatch-0.2.5/src/promptwatch.egg-info/requires.txt
--rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-07-14 21:46:30.000000 promptwatch-0.2.5/src/promptwatch.egg-info/top_level.txt
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-18 16:08:39.373280 promptwatch-0.2.6/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-07-18 16:08:39.373089 promptwatch-0.2.6/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3584 2023-05-19 10:25:10.000000 promptwatch-0.2.6/README.md
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      100 2023-04-17 11:00:59.000000 promptwatch-0.2.6/pyproject.toml
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       38 2023-07-18 16:08:39.373331 promptwatch-0.2.6/setup.cfg
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1198 2023-05-24 21:47:14.000000 promptwatch-0.2.6/setup.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-18 16:08:39.365479 promptwatch-0.2.6/src/
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-18 16:08:39.368685 promptwatch-0.2.6/src/promptwatch/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      442 2023-07-18 16:08:14.000000 promptwatch-0.2.6/src/promptwatch/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    16530 2023-05-31 21:34:19.000000 promptwatch-0.2.6/src/promptwatch/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     6257 2023-05-30 16:43:11.000000 promptwatch-0.2.6/src/promptwatch/client.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      260 2023-05-19 10:25:10.000000 promptwatch-0.2.6/src/promptwatch/constants.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     5281 2023-07-14 21:49:02.000000 promptwatch-0.2.6/src/promptwatch/data_model.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     1555 2023-05-23 20:20:02.000000 promptwatch-0.2.6/src/promptwatch/decorators.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-18 16:08:39.371101 promptwatch-0.2.6/src/promptwatch/langchain/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      219 2023-05-30 19:26:54.000000 promptwatch-0.2.6/src/promptwatch/langchain/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    12414 2023-05-31 20:26:52.000000 promptwatch-0.2.6/src/promptwatch/langchain/caching.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    31322 2023-07-18 10:38:03.000000 promptwatch-0.2.6/src/promptwatch/langchain/langchain_support.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     4270 2023-05-19 10:25:10.000000 promptwatch-0.2.6/src/promptwatch/langchain/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    18116 2023-07-18 10:44:42.000000 promptwatch-0.2.6/src/promptwatch/promptwatch_context.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-18 16:08:39.372450 promptwatch-0.2.6/src/promptwatch/unit_tests/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      162 2023-05-19 10:25:10.000000 promptwatch-0.2.6/src/promptwatch/unit_tests/__init__.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13513 2023-05-20 12:19:55.000000 promptwatch-0.2.6/src/promptwatch/unit_tests/evaluation.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2261 2023-05-19 10:25:10.000000 promptwatch-0.2.6/src/promptwatch/unit_tests/schema.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)    13645 2023-05-24 14:32:24.000000 promptwatch-0.2.6/src/promptwatch/unit_tests/unit_tests.py
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     2368 2023-06-17 16:42:18.000000 promptwatch-0.2.6/src/promptwatch/utils.py
+drwxr-xr-x   0 jurajbezdek   (501) staff       (20)        0 2023-07-18 16:08:39.369861 promptwatch-0.2.6/src/promptwatch.egg-info/
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)     3958 2023-07-18 16:08:39.000000 promptwatch-0.2.6/src/promptwatch.egg-info/PKG-INFO
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)      819 2023-07-18 16:08:39.000000 promptwatch-0.2.6/src/promptwatch.egg-info/SOURCES.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-07-18 16:08:39.000000 promptwatch-0.2.6/src/promptwatch.egg-info/dependency_links.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)        1 2023-04-17 11:10:06.000000 promptwatch-0.2.6/src/promptwatch.egg-info/not-zip-safe
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       33 2023-07-18 16:08:39.000000 promptwatch-0.2.6/src/promptwatch.egg-info/requires.txt
+-rw-r--r--   0 jurajbezdek   (501) staff       (20)       12 2023-07-18 16:08:39.000000 promptwatch-0.2.6/src/promptwatch.egg-info/top_level.txt
```

### Comparing `promptwatch-0.2.5/PKG-INFO` & `promptwatch-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.2.5
+Version: 0.2.6
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.2.5/README.md` & `promptwatch-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.5/setup.py` & `promptwatch-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.5/src/promptwatch/caching.py` & `promptwatch-0.2.6/src/promptwatch/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.5/src/promptwatch/client.py` & `promptwatch-0.2.6/src/promptwatch/client.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.5/src/promptwatch/data_model.py` & `promptwatch-0.2.6/src/promptwatch/data_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -162,15 +162,14 @@
     format:Optional[str]
     
 class ChatMessage(BaseModel):
     """ Explicit chat message used as a parameter value for chat history or template"""
     role:Optional[str]
     text:str
 
-
 class ChatMessagePromptTemplate(PromptTemplateDescription):
     role:Optional[str]
     
     
 class NamedPromptTemplateDescription(PromptTemplateDescription):
     template_name:str
     template_version:Optional[str]
```

### Comparing `promptwatch-0.2.5/src/promptwatch/decorators.py` & `promptwatch-0.2.6/src/promptwatch/decorators.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.5/src/promptwatch/langchain/caching.py` & `promptwatch-0.2.6/src/promptwatch/langchain/caching.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.5/src/promptwatch/langchain/langchain_support.py` & `promptwatch-0.2.6/src/promptwatch/langchain/langchain_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -302,21 +302,22 @@
     async def on_llm_error(
         self, error: Union[Exception, KeyboardInterrupt], **kwargs: Any
     ) -> Any:
         """Run when LLM errors."""
         self.prompt_watch._on_error(error, kwargs)
 
     
-    async def on_chain_start(
+    def on_chain_start(
         self, serialized: Dict[str, Any], inputs: Dict[str, Any], **kwargs: Any
     ) -> Any:
         """Run when chain starts running."""
         
-        if "LLM" in serialized.get("name","") or "LLM" in ".".join(serialized.get("id",[])) :
-            current_llm_chain = find_the_caller_in_the_stack(serialized["name"])
+        chain_name = serialized.get("name") or  serialized.get("id",[None])[-1]
+        if "LLM" in chain_name :
+            current_llm_chain = find_the_caller_in_the_stack(chain_name)
             self.prompt_watch.add_context(LLM_CHAIN_CONTEXT_KEY,current_llm_chain)
 
         self.try_get_retrieved_documents(inputs)
                   
 
 
         question = inputs.get("question")
```

### Comparing `promptwatch-0.2.5/src/promptwatch/langchain/unit_tests.py` & `promptwatch-0.2.6/src/promptwatch/langchain/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.5/src/promptwatch/promptwatch_context.py` & `promptwatch-0.2.6/src/promptwatch/promptwatch_context.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,39 +20,39 @@
 session_context = contextvars.ContextVar("promptwatch_context")
 
 class ContextTrackerSingleton(ABCMeta,type):
     """
     Singleton metaclass for ensuring only one instance of a class per thread
     """
 
-    #_thread_local = threading.local()
-    #_cross_thread_storage = {}
+    
+    _cross_thread_storage = {}
 
     def __call__(cls, *args, **kwargs)->PromptWatch:
         """Call method for the singleton metaclass."""
         prompt_watch_context = session_context.get(None)
         if not prompt_watch_context:
             prompt_watch_context = super(ContextTrackerSingleton, cls).__call__(*args, **kwargs)
             if not prompt_watch_context.session_id:
                 raise Exception("PromptWatch: Session ID was not initialized. Please report this as a bug.")
             session_context.set(prompt_watch_context)
             
-            # ContextTrackerSingleton._cross_thread_storage[prompt_watch_context.session_id] = prompt_watch_context
-            # ContextTrackerSingleton._thread_local._instance = prompt_watch_context
+            ContextTrackerSingleton._cross_thread_storage[prompt_watch_context.session_id] = prompt_watch_context
+            
        
         return prompt_watch_context
         
     def get_current(session_id:str=None)->PromptWatch:
         """ return the current instance
         for sync context session_id is not required
         for async context session_id is required, otherwise it the instance wont be found
         """
         prompt_watch_context =  session_context.get(None)
         if not prompt_watch_context:
-            return None
+            return ContextTrackerSingleton._cross_thread_storage.get(session_id)
         elif session_id and prompt_watch_context.session_id != session_id:
             raise Exception("PromptWatch: Session ID mismatch. Please report this as a bug.")
         else:
             return prompt_watch_context
 
     @classmethod
     def remove_active_instance(cls):
@@ -432,16 +432,17 @@
         self._flush_stack()
         if self.current_session.steps_count:
             self.client.finish_session(self.current_session)
         ContextTrackerSingleton.remove_active_instance()
         self.current_session=None
 
     def _on_error(self, error, kwargs):
-        self.current_activity.error=str(error)
-        if kwargs:
+        if self.current_activity:
+            self.current_activity.error=str(error)
+        if self.current_activity and kwargs:
             if not self.current_activity.metadata:
                 self.current_activity.metadata={}
             self.current_activity.metadata["error_kwargs"]=kwargs
         self.current_session.is_error=True
         self._close_current_activity()
 
     def _decode_tenant_from_api_key(self, api_key)->str:
```

### Comparing `promptwatch-0.2.5/src/promptwatch/unit_tests/evaluation.py` & `promptwatch-0.2.6/src/promptwatch/unit_tests/evaluation.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.5/src/promptwatch/unit_tests/schema.py` & `promptwatch-0.2.6/src/promptwatch/unit_tests/schema.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.5/src/promptwatch/unit_tests/unit_tests.py` & `promptwatch-0.2.6/src/promptwatch/unit_tests/unit_tests.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.5/src/promptwatch/utils.py` & `promptwatch-0.2.6/src/promptwatch/utils.py`

 * *Files identical despite different names*

### Comparing `promptwatch-0.2.5/src/promptwatch.egg-info/PKG-INFO` & `promptwatch-0.2.6/src/promptwatch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promptwatch
-Version: 0.2.5
+Version: 0.2.6
 Summary: promptwatch.io python client to trace langchain sessions
 Home-page: https://github.com/blip-solutions/promptwatch-client
 Author: Juraj Bezdek
 Author-email: juraj.bezdek@blip.solutions
 License: MIT License
 Keywords: promptwatch prompt monitoring
 Requires-Python: >=3.8
```

### Comparing `promptwatch-0.2.5/src/promptwatch.egg-info/SOURCES.txt` & `promptwatch-0.2.6/src/promptwatch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

