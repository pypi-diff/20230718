# Comparing `tmp/compel-2.0.0rc1.tar.gz` & `tmp/compel-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-3zkjqq6r/compel-2.0.0rc1.tar", last modified: Wed Jul 12 22:59:45 2023, max compression
+gzip compressed data, was "/Users/damian/2.current/stablediffusion/compel/dist/.tmp-cnb_kmek/compel-2.0.0rc2.tar", last modified: Fri Jul 14 09:35:16 2023, max compression
```

## Comparing `compel-2.0.0rc1.tar` & `compel-2.0.0rc2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-12 22:59:45.000000 compel-2.0.0rc1/
--rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-2.0.0rc1/LICENSE
--rw-r--r--   0 damian     (501) staff       (20)    11075 2023-07-12 22:59:45.000000 compel-2.0.0rc1/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)    10494 2023-07-04 22:01:43.000000 compel-2.0.0rc1/README.md
--rw-r--r--   0 damian     (501) staff       (20)      766 2023-07-12 22:59:12.000000 compel-2.0.0rc1/pyproject.toml
--rw-r--r--   0 damian     (501) staff       (20)       38 2023-07-12 22:59:45.000000 compel-2.0.0rc1/setup.cfg
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/compel/
--rw-r--r--   0 damian     (501) staff       (20)      175 2023-06-03 06:15:19.000000 compel-2.0.0rc1/src/compel/__init__.py
--rw-r--r--   0 damian     (501) staff       (20)    20003 2023-07-12 22:48:45.000000 compel-2.0.0rc1/src/compel/compel.py
--rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-2.0.0rc1/src/compel/conditioning_scheduler.py
--rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-2.0.0rc1/src/compel/cross_attention_control.py
--rw-r--r--   0 damian     (501) staff       (20)      653 2023-06-03 06:15:19.000000 compel-2.0.0rc1/src/compel/diffusers_textual_inversion_manager.py
--rw-r--r--   0 damian     (501) staff       (20)    30339 2023-07-12 22:57:28.000000 compel-2.0.0rc1/src/compel/embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    30771 2023-07-04 21:57:36.000000 compel-2.0.0rc1/src/compel/prompt_parser.py
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/compel.egg-info/
--rw-r--r--   0 damian     (501) staff       (20)    11075 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/compel.egg-info/PKG-INFO
--rw-r--r--   0 damian     (501) staff       (20)      512 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/compel.egg-info/SOURCES.txt
--rw-r--r--   0 damian     (501) staff       (20)        1 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/compel.egg-info/dependency_links.txt
--rw-r--r--   0 damian     (501) staff       (20)       56 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/compel.egg-info/requires.txt
--rw-r--r--   0 damian     (501) staff       (20)        7 2023-07-12 22:59:45.000000 compel-2.0.0rc1/src/compel.egg-info/top_level.txt
-drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-12 22:59:45.000000 compel-2.0.0rc1/test/
--rw-r--r--   0 damian     (501) staff       (20)    16457 2023-07-12 22:58:27.000000 compel-2.0.0rc1/test/test_compel.py
--rw-r--r--   0 damian     (501) staff       (20)    21072 2023-06-03 06:15:11.000000 compel-2.0.0rc1/test/test_embeddings_provider.py
--rw-r--r--   0 damian     (501) staff       (20)    47562 2023-06-03 06:55:54.000000 compel-2.0.0rc1/test/test_prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-14 09:35:16.000000 compel-2.0.0rc2/
+-rw-r--r--   0 damian     (501) staff       (20)     1064 2023-03-07 13:01:09.000000 compel-2.0.0rc2/LICENSE
+-rw-r--r--   0 damian     (501) staff       (20)    11075 2023-07-14 09:35:16.000000 compel-2.0.0rc2/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)    10494 2023-07-04 22:01:43.000000 compel-2.0.0rc2/README.md
+-rw-r--r--   0 damian     (501) staff       (20)      766 2023-07-14 09:33:35.000000 compel-2.0.0rc2/pyproject.toml
+-rw-r--r--   0 damian     (501) staff       (20)       38 2023-07-14 09:35:16.000000 compel-2.0.0rc2/setup.cfg
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/compel/
+-rw-r--r--   0 damian     (501) staff       (20)      175 2023-06-03 06:15:19.000000 compel-2.0.0rc2/src/compel/__init__.py
+-rw-r--r--   0 damian     (501) staff       (20)    20356 2023-07-14 09:32:50.000000 compel-2.0.0rc2/src/compel/compel.py
+-rw-r--r--   0 damian     (501) staff       (20)     1833 2023-03-15 21:38:57.000000 compel-2.0.0rc2/src/compel/conditioning_scheduler.py
+-rw-r--r--   0 damian     (501) staff       (20)     1581 2023-03-07 13:01:09.000000 compel-2.0.0rc2/src/compel/cross_attention_control.py
+-rw-r--r--   0 damian     (501) staff       (20)      653 2023-06-03 06:15:19.000000 compel-2.0.0rc2/src/compel/diffusers_textual_inversion_manager.py
+-rw-r--r--   0 damian     (501) staff       (20)    30339 2023-07-12 22:57:28.000000 compel-2.0.0rc2/src/compel/embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    30771 2023-07-04 21:57:36.000000 compel-2.0.0rc2/src/compel/prompt_parser.py
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/compel.egg-info/
+-rw-r--r--   0 damian     (501) staff       (20)    11075 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/compel.egg-info/PKG-INFO
+-rw-r--r--   0 damian     (501) staff       (20)      512 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/compel.egg-info/SOURCES.txt
+-rw-r--r--   0 damian     (501) staff       (20)        1 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/compel.egg-info/dependency_links.txt
+-rw-r--r--   0 damian     (501) staff       (20)       56 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/compel.egg-info/requires.txt
+-rw-r--r--   0 damian     (501) staff       (20)        7 2023-07-14 09:35:16.000000 compel-2.0.0rc2/src/compel.egg-info/top_level.txt
+drwxr-xr-x   0 damian     (501) staff       (20)        0 2023-07-14 09:35:16.000000 compel-2.0.0rc2/test/
+-rw-r--r--   0 damian     (501) staff       (20)    16457 2023-07-12 22:58:27.000000 compel-2.0.0rc2/test/test_compel.py
+-rw-r--r--   0 damian     (501) staff       (20)    21072 2023-06-03 06:15:11.000000 compel-2.0.0rc2/test/test_embeddings_provider.py
+-rw-r--r--   0 damian     (501) staff       (20)    47562 2023-06-03 06:55:54.000000 compel-2.0.0rc2/test/test_prompt_parser.py
```

### Comparing `compel-2.0.0rc1/LICENSE` & `compel-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc1/PKG-INFO` & `compel-2.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `compel-2.0.0rc1/README.md` & `compel-2.0.0rc2/README.md`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc1/pyproject.toml` & `compel-2.0.0rc2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "compel"
-version = "2.0.0-pre1"
+version = "2.0.0-pre2"
 authors = [
   { name="Damian Stewart", email="null@damianstewart.com" },
 ]
 description = "A prompting enhancement library for transformers-type text embedding systems."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `compel-2.0.0rc1/src/compel/compel.py` & `compel-2.0.0rc2/src/compel/compel.py`

 * *Files 1% similar despite different names*

```diff
@@ -201,59 +201,64 @@
                 cac_args = self._get_conditioning_for_cross_attention_control(prompt)
                 return cac_args.original_conditioning, { 'cross_attention_control': cac_args }
             else:
                 return self._get_conditioning_for_flattened_prompt(prompt), {}
 
         raise ValueError(f"unsupported prompt type: {type(prompt).__name__}")
 
-
-
-    def pad_conditioning_tensors_to_same_length(self, conditionings: List[torch.Tensor],
-                                                ) -> List[torch.Tensor]:
-        """
-        If `truncate_long_prompts` was set to False on initialization, or if your prompt includes a `.and()` operator,
-        conditioning tensors do not have a fixed length. This is a problem when using a negative and a positive prompt
-        to condition the diffusion process. This function pads any of the passed-in tensors, as necessary, to ensure
-        they all have the same length, returning the padded tensors in the same order they are passed.
-
-        Example:
-            ``` python
-            embeds = compel('("a cat playing in the forest", "an impressionist oil painting").and()')
-            negative_embeds = compel("ugly, deformed, distorted")
-            [embeds, negative_embeds] = compel.pad_conditioning_tensors_to_same_length([embeds, negative_embeds])
-            ```
-        """
+    @classmethod
+    def _pad_conditioning_tensors_to_same_length(cls, conditionings: List[torch.Tensor], emptystring_conditioning: torch.Tensor
+                                                 ) -> List[torch.Tensor]:
         c0_shape = conditionings[0].shape
         if not all([len(c.shape) == len(c0_shape) for c in conditionings]):
             raise ValueError("Conditioning tensors must all have either 2 dimensions (unbatched) or 3 dimensions (batched)")
 
         if len(c0_shape) == 2:
             # need to be unsqueezed
             conditionings = [c.unsqueeze(0) for c in conditionings]
             c0_shape = conditionings[0].shape
         if len(c0_shape) != 3:
             raise ValueError(f"All conditioning tensors must have the same number of dimensions (2 or 3)")
 
         if not all([c.shape[0] == c0_shape[0] and c.shape[2] == c0_shape[2] for c in conditionings]):
             raise ValueError(f"All conditioning tensors must have the same batch size ({c0_shape[0]}) and number of embeddings per token ({c0_shape[1]}")
 
+        empty_z = torch.cat([emptystring_conditioning] * c0_shape[0])
         max_token_count = max([c.shape[1] for c in conditionings])
         # if necessary, pad shorter tensors out with an emptystring tensor
-        emptystring_conditioning = self.build_conditioning_tensor("")
-        if type(emptystring_conditioning) is tuple:
-            # discard pooled
-            emptystring_conditioning = emptystring_conditioning[0]
-        empty_z = torch.cat([emptystring_conditioning] * c0_shape[0])
         for i, c in enumerate(conditionings):
             while c.shape[1] < max_token_count:
                 c = torch.cat([c, empty_z], dim=1)
                 conditionings[i] = c
         return conditionings
 
 
+    def pad_conditioning_tensors_to_same_length(self, conditionings: List[torch.Tensor],
+                                                ) -> List[torch.Tensor]:
+        """
+        If `truncate_long_prompts` was set to False on initialization, or if your prompt includes a `.and()` operator,
+        conditioning tensors do not have a fixed length. This is a problem when using a negative and a positive prompt
+        to condition the diffusion process. This function pads any of the passed-in tensors, as necessary, to ensure
+        they all have the same length, returning the padded tensors in the same order they are passed.
+
+        Example:
+            ``` python
+            embeds = compel('("a cat playing in the forest", "an impressionist oil painting").and()')
+            negative_embeds = compel("ugly, deformed, distorted")
+            [embeds, negative_embeds] = compel.pad_conditioning_tensors_to_same_length([embeds, negative_embeds])
+            ```
+        """
+        emptystring_conditioning = self.build_conditioning_tensor("")
+        if type(emptystring_conditioning) is tuple:
+            # discard pooled
+            emptystring_conditioning = emptystring_conditioning[0]
+        return type(self)._pad_conditioning_tensors_to_same_length(conditionings, emptystring_conditioning=emptystring_conditioning)
+
+
+
     def _get_conditioning_for_flattened_prompt(self,
                                                prompt: FlattenedPrompt,
                                                should_return_tokens: bool=False
                                                ) -> Union[torch.Tensor, Tuple[torch.Tensor, torch.Tensor]]:
         if type(prompt) is not FlattenedPrompt:
             raise ValueError(f"embeddings can only be made from FlattenedPrompts, got {type(prompt).__name__} instead")
         fragments = [x.text for x in prompt.children]
```

### Comparing `compel-2.0.0rc1/src/compel/conditioning_scheduler.py` & `compel-2.0.0rc2/src/compel/conditioning_scheduler.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc1/src/compel/cross_attention_control.py` & `compel-2.0.0rc2/src/compel/cross_attention_control.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc1/src/compel/diffusers_textual_inversion_manager.py` & `compel-2.0.0rc2/src/compel/diffusers_textual_inversion_manager.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc1/src/compel/embeddings_provider.py` & `compel-2.0.0rc2/src/compel/embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc1/src/compel/prompt_parser.py` & `compel-2.0.0rc2/src/compel/prompt_parser.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc1/src/compel.egg-info/PKG-INFO` & `compel-2.0.0rc2/src/compel.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: compel
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: A prompting enhancement library for transformers-type text embedding systems.
 Author-email: Damian Stewart <null@damianstewart.com>
 Project-URL: Homepage, https://github.com/damian0815/compel
 Project-URL: Bug Tracker, https://github.com/damian0815/compel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
```

### Comparing `compel-2.0.0rc1/src/compel.egg-info/SOURCES.txt` & `compel-2.0.0rc2/src/compel.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc1/test/test_compel.py` & `compel-2.0.0rc2/test/test_compel.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc1/test/test_embeddings_provider.py` & `compel-2.0.0rc2/test/test_embeddings_provider.py`

 * *Files identical despite different names*

### Comparing `compel-2.0.0rc1/test/test_prompt_parser.py` & `compel-2.0.0rc2/test/test_prompt_parser.py`

 * *Files identical despite different names*

