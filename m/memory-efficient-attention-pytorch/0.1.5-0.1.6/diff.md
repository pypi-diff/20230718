# Comparing `tmp/memory-efficient-attention-pytorch-0.1.5.tar.gz` & `tmp/memory-efficient-attention-pytorch-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory-efficient-attention-pytorch-0.1.5.tar", last modified: Tue Jul 18 00:53:41 2023, max compression
+gzip compressed data, was "memory-efficient-attention-pytorch-0.1.6.tar", last modified: Tue Jul 18 02:42:46 2023, max compression
```

## Comparing `memory-efficient-attention-pytorch-0.1.5.tar` & `memory-efficient-attention-pytorch-0.1.6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:53:41.763570 memory-efficient-attention-pytorch-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-18 00:53:41.763570 memory-efficient-attention-pytorch-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:53:41.763570 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/cosine_sim_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/memory_efficient_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/memory_efficient_cosine_sim_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/reversible.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:53:41.763570 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-18 00:53:41.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-18 00:53:41.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 00:53:41.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 00:53:41.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-18 00:53:41.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-18 00:53:41.763570 memory-efficient-attention-pytorch-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:53:41.763570 memory-efficient-attention-pytorch-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:42:46.145041 memory-efficient-attention-pytorch-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-18 02:42:29.000000 memory-efficient-attention-pytorch-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-18 02:42:46.145041 memory-efficient-attention-pytorch-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-18 02:42:29.000000 memory-efficient-attention-pytorch-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:42:46.145041 memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-18 02:42:29.000000 memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-18 02:42:29.000000 memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-07-18 02:42:29.000000 memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/cosine_sim_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-07-18 02:42:29.000000 memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-18 02:42:29.000000 memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/memory_efficient_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-18 02:42:29.000000 memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/memory_efficient_cosine_sim_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-18 02:42:29.000000 memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/reversible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-18 02:42:29.000000 memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:42:46.145041 memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-18 02:42:46.000000 memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-18 02:42:46.000000 memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 02:42:46.000000 memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 02:42:46.000000 memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-18 02:42:46.000000 memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-18 02:42:46.145041 memory-efficient-attention-pytorch-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-18 02:42:29.000000 memory-efficient-attention-pytorch-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:42:46.145041 memory-efficient-attention-pytorch-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-18 02:42:29.000000 memory-efficient-attention-pytorch-0.1.6/tests/test.py
```

### Comparing `memory-efficient-attention-pytorch-0.1.5/LICENSE` & `memory-efficient-attention-pytorch-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.5/PKG-INFO` & `memory-efficient-attention-pytorch-0.1.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-efficient-attention-pytorch
-Version: 0.1.5
+Version: 0.1.6
 Summary: Memory Efficient Attention - Pytorch
 Home-page: https://github.com/lucidrains/memory-efficient-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention-mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `memory-efficient-attention-pytorch-0.1.5/README.md` & `memory-efficient-attention-pytorch-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/autoregressive_wrapper.py` & `memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/cosine_sim_flash_attention.py` & `memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/cosine_sim_flash_attention.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/flash_attention.py` & `memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/flash_attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from torch import nn, einsum
 from torch.autograd.function import Function
 
 from einops import rearrange
 
 # constants
 
-EPSILON = 1e-6
+EPSILON = 1e-10
 
 # helper functions
 
 def exists(val):
     return val is not None
 
 def default(val, d):
@@ -77,32 +77,30 @@
                     attn_weights.masked_fill_(~col_mask, max_neg_value)
 
                 if causal and q_start_index < (k_start_index + k_bucket_size - 1):
                     causal_mask = torch.ones((qc.shape[-2], kc.shape[-2]), dtype = torch.bool, device = device).triu(q_start_index - k_start_index + 1)
                     attn_weights.masked_fill_(causal_mask, max_neg_value)
 
                 block_row_maxes = attn_weights.amax(dim = -1, keepdims = True)
-                attn_weights -= block_row_maxes
-                exp_weights = torch.exp(attn_weights)
+                new_row_maxes = torch.maximum(block_row_maxes, row_maxes)
+
+                exp_weights = torch.exp(attn_weights - new_row_maxes)
 
                 if exists(col_mask):
                     exp_weights.masked_fill_(~col_mask, 0.)
 
                 block_row_sums = exp_weights.sum(dim = -1, keepdims = True).clamp(min = EPSILON)
 
-                new_row_maxes = torch.maximum(block_row_maxes, row_maxes)
-
                 exp_values = einsum('... i j, ... j d -> ... i d', exp_weights, vc)
 
                 exp_row_max_diff = torch.exp(row_maxes - new_row_maxes)
-                exp_block_row_max_diff = torch.exp(block_row_maxes - new_row_maxes)
 
-                new_row_sums = exp_row_max_diff * row_sums + exp_block_row_max_diff * block_row_sums
+                new_row_sums = exp_row_max_diff * row_sums + block_row_sums
 
-                oc.mul_(exp_row_max_diff).add_(exp_block_row_max_diff * exp_values)
+                oc.mul_(exp_row_max_diff).add_(exp_values)
 
                 row_maxes.copy_(new_row_maxes)
                 row_sums.copy_(new_row_sums)
 
             oc.div_(row_sums)
 
         lse = all_row_sums.log() + all_row_maxes
```

### Comparing `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/memory_efficient_attention.py` & `memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/memory_efficient_attention.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/memory_efficient_cosine_sim_attention.py` & `memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/memory_efficient_cosine_sim_attention.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/reversible.py` & `memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/reversible.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/transformer.py` & `memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch/transformer.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/PKG-INFO` & `memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: memory-efficient-attention-pytorch
-Version: 0.1.5
+Version: 0.1.6
 Summary: Memory Efficient Attention - Pytorch
 Home-page: https://github.com/lucidrains/memory-efficient-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention-mechanism
 Classifier: Development Status :: 4 - Beta
```

### Comparing `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/SOURCES.txt` & `memory-efficient-attention-pytorch-0.1.6/memory_efficient_attention_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.5/setup.py` & `memory-efficient-attention-pytorch-0.1.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'memory-efficient-attention-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.1.5',
+  version = '0.1.6',
   license='MIT',
   description = 'Memory Efficient Attention - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/memory-efficient-attention-pytorch',
   keywords = [
```

### Comparing `memory-efficient-attention-pytorch-0.1.5/tests/test.py` & `memory-efficient-attention-pytorch-0.1.6/tests/test.py`

 * *Files identical despite different names*

