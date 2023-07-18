# Comparing `tmp/memory-efficient-attention-pytorch-0.1.4.tar.gz` & `tmp/memory-efficient-attention-pytorch-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "memory-efficient-attention-pytorch-0.1.4.tar", last modified: Sun Jul 16 16:09:42 2023, max compression
+gzip compressed data, was "memory-efficient-attention-pytorch-0.1.5.tar", last modified: Tue Jul 18 00:53:41 2023, max compression
```

## Comparing `memory-efficient-attention-pytorch-0.1.4.tar` & `memory-efficient-attention-pytorch-0.1.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:09:42.697715 memory-efficient-attention-pytorch-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-16 16:09:42.697715 memory-efficient-attention-pytorch-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:09:42.697715 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/autoregressive_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/cosine_sim_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7933 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/memory_efficient_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/memory_efficient_cosine_sim_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/reversible.py
--rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/transformer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:09:42.697715 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-16 16:09:42.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-16 16:09:42.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 16:09:42.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-16 16:09:42.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-16 16:09:42.000000 memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-16 16:09:42.697715 memory-efficient-attention-pytorch-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 16:09:42.697715 memory-efficient-attention-pytorch-0.1.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-16 16:09:30.000000 memory-efficient-attention-pytorch-0.1.4/tests/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:53:41.763570 memory-efficient-attention-pytorch-0.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-18 00:53:41.763570 memory-efficient-attention-pytorch-0.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:53:41.763570 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/autoregressive_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6976 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/cosine_sim_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7919 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/memory_efficient_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6356 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/memory_efficient_cosine_sim_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4725 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/reversible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/transformer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:53:41.763570 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-07-18 00:53:41.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-07-18 00:53:41.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 00:53:41.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 00:53:41.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-18 00:53:41.000000 memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-18 00:53:41.763570 memory-efficient-attention-pytorch-0.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 00:53:41.763570 memory-efficient-attention-pytorch-0.1.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     4544 2023-07-18 00:53:29.000000 memory-efficient-attention-pytorch-0.1.5/tests/test.py
```

### Comparing `memory-efficient-attention-pytorch-0.1.4/LICENSE` & `memory-efficient-attention-pytorch-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.4/PKG-INFO` & `memory-efficient-attention-pytorch-0.1.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memory-efficient-attention-pytorch
-Version: 0.1.4
+Version: 0.1.5
 Summary: Memory Efficient Attention - Pytorch
 Home-page: https://github.com/lucidrains/memory-efficient-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention-mechanism
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `memory-efficient-attention-pytorch-0.1.4/README.md` & `memory-efficient-attention-pytorch-0.1.5/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ## Memory Efficient Attention Pytorch (obsolete)
 
 Implementation of a memory efficient multi-head attention as proposed in the paper, <a href="https://arxiv.org/abs/2112.05682">Self-attention Does Not Need O(n²) Memory</a>. In addition, the module will take care of masking, causal masking, as well as cross attention.
 
-This repository also contains a <a href="https://github.com/lucidrains/memory-efficient-attention-pytorch/blob/main/memory_efficient_attention_pytorch/flash_attention.py">naive non-CUDA implementation</a> of the improvements made by <a href="https://tridao.me/">Tri Dao</a> with his <a href="https://github.com/HazyResearch/flash-attention">Flash Attention</a> paper, for educational purposes. It is a game changer for attention and building long-context transformers.
+This repository also contains a <a href="https://github.com/lucidrains/memory-efficient-attention-pytorch/blob/main/memory_efficient_attention_pytorch/flash_attention.py">naive non-CUDA implementation</a> of the improvements made by <a href="https://tridao.me/">Tri Dao</a> with his <a href="https://github.com/HazyResearch/flash-attention">Flash Attention 2</a> paper, for educational purposes. It is a game changer for attention and building long-context transformers.
 
 Update: from now on, you should just be using the <a href="https://pytorch.org/docs/master/generated/torch.nn.functional.scaled_dot_product_attention.html?highlight=scaled_dot_product#torch.nn.functional.scaled_dot_product_attention">`F.scaled_dot_product_attention`</a> function in Pytorch 2.0
 
 ## Install
 
 ```bash
 $ pip install memory-efficient-attention-pytorch
@@ -85,7 +85,15 @@
     title   = {FlashAttention: Fast and Memory-Efficient Exact Attention with IO-Awareness},
     author  = {Tri Dao and Daniel Y. Fu and Stefano Ermon and Atri Rudra and Christopher R'e},
     journal = {ArXiv},
     year    = {2022},
     volume  = {abs/2205.14135}
 }
 ```
+
+```bibtex
+@article{dao2023flashattention2,
+  title     = {Flash{A}ttention-2: Faster Attention with Better Parallelism and Work Partitioning,
+  author    = {Dao, Tri},
+  year      = {2023}
+}
+```
```

#### html2text {}

```diff
@@ -1,13 +1,13 @@
 ## Memory Efficient Attention Pytorch (obsolete) Implementation of a memory
 efficient multi-head attention as proposed in the paper, Self-attention_Does
 Not_Need_O(nÂ²)_Memory. In addition, the module will take care of masking,
 causal masking, as well as cross attention. This repository also contains a
 naive_non-CUDA_implementation of the improvements made by Tri_Dao with his
-Flash_Attention paper, for educational purposes. It is a game changer for
+Flash_Attention_2 paper, for educational purposes. It is a game changer for
 attention and building long-context transformers. Update: from now on, you
 should just be using the `F.scaled_dot_product_attention` function in Pytorch
 2.0 ## Install ```bash $ pip install memory-efficient-attention-pytorch ``` ##
 Usage For autoregressive language model ```python import torch from
 memory_efficient_attention_pytorch import Attention attn = Attention( dim =
 512, dim_head = 64, # dimension per head heads = 8, # number of attention heads
 causal = True, # autoregressive or not memory_efficient = True, # whether to
@@ -28,8 +28,11 @@
 Resolution}, author = {Ze Liu and Han Hu and Yutong Lin and Zhuliang Yao and
 Zhenda Xie and Yixuan Wei and Jia Ning and Yue Cao and Zheng Zhang and Li Dong
 and Furu Wei and Baining Guo}, year = {2021}, eprint = {2111.09883},
 archivePrefix = {arXiv}, primaryClass = {cs.CV} } ``` ```bibtex @article
 {Dao2022FlashAttentionFA, title = {FlashAttention: Fast and Memory-Efficient
 Exact Attention with IO-Awareness}, author = {Tri Dao and Daniel Y. Fu and
 Stefano Ermon and Atri Rudra and Christopher R'e}, journal = {ArXiv}, year =
-{2022}, volume = {abs/2205.14135} } ```
+{2022}, volume = {abs/2205.14135} } ``` ```bibtex @article
+{dao2023flashattention2, title = {Flash{A}ttention-2: Faster Attention with
+Better Parallelism and Work Partitioning, author = {Dao, Tri}, year = {2023} }
+```
```

### Comparing `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/autoregressive_wrapper.py` & `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/autoregressive_wrapper.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/cosine_sim_flash_attention.py` & `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/cosine_sim_flash_attention.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/flash_attention.py` & `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/flash_attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,19 +94,21 @@
                 exp_values = einsum('... i j, ... j d -> ... i d', exp_weights, vc)
 
                 exp_row_max_diff = torch.exp(row_maxes - new_row_maxes)
                 exp_block_row_max_diff = torch.exp(block_row_maxes - new_row_maxes)
 
                 new_row_sums = exp_row_max_diff * row_sums + exp_block_row_max_diff * block_row_sums
 
-                oc.mul_((row_sums / new_row_sums) * exp_row_max_diff).add_((exp_block_row_max_diff / new_row_sums) * exp_values)
+                oc.mul_(exp_row_max_diff).add_(exp_block_row_max_diff * exp_values)
 
                 row_maxes.copy_(new_row_maxes)
                 row_sums.copy_(new_row_sums)
 
+            oc.div_(row_sums)
+
         lse = all_row_sums.log() + all_row_maxes
 
         ctx.args = (causal, scale, mask, q_bucket_size, k_bucket_size)
         ctx.save_for_backward(q, k, v, o, lse)
 
         return o
```

### Comparing `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/memory_efficient_attention.py` & `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/memory_efficient_attention.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/memory_efficient_cosine_sim_attention.py` & `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/memory_efficient_cosine_sim_attention.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/reversible.py` & `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/reversible.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch/transformer.py` & `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch/transformer.py`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/PKG-INFO` & `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: memory-efficient-attention-pytorch
-Version: 0.1.4
+Version: 0.1.5
 Summary: Memory Efficient Attention - Pytorch
 Home-page: https://github.com/lucidrains/memory-efficient-attention-pytorch
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,attention-mechanism
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `memory-efficient-attention-pytorch-0.1.4/memory_efficient_attention_pytorch.egg-info/SOURCES.txt` & `memory-efficient-attention-pytorch-0.1.5/memory_efficient_attention_pytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `memory-efficient-attention-pytorch-0.1.4/setup.py` & `memory-efficient-attention-pytorch-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'memory-efficient-attention-pytorch',
   packages = find_packages(exclude=[]),
-  version = '0.1.4',
+  version = '0.1.5',
   license='MIT',
   description = 'Memory Efficient Attention - Pytorch',
   long_description_content_type = 'text/markdown',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   url = 'https://github.com/lucidrains/memory-efficient-attention-pytorch',
   keywords = [
@@ -26,10 +26,10 @@
     'pytest'
   ],
   classifiers=[
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Topic :: Scientific/Engineering :: Artificial Intelligence',
     'License :: OSI Approved :: MIT License',
-    'Programming Language :: Python :: 3.6',
+    'Programming Language :: Python :: 3.8',
   ],
 )
```

### Comparing `memory-efficient-attention-pytorch-0.1.4/tests/test.py` & `memory-efficient-attention-pytorch-0.1.5/tests/test.py`

 * *Files identical despite different names*

