# Comparing `tmp/flash-attention-jax-0.3.0.tar.gz` & `tmp/flash-attention-jax-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flash-attention-jax-0.3.0.tar", last modified: Sun Jun 18 17:53:40 2023, max compression
+gzip compressed data, was "flash-attention-jax-0.3.1.tar", last modified: Tue Jul 18 02:45:07 2023, max compression
```

## Comparing `flash-attention-jax-0.3.0.tar` & `flash-attention-jax-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:53:40.365268 flash-attention-jax-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-18 17:53:40.365268 flash-attention-jax-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:53:40.365268 flash-attention-jax-0.3.0/flash_attention_jax/
--rw-r--r--   0 runner    (1001) docker     (123)      494 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/flash_attention_jax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/flash_attention_jax/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/flash_attention_jax/causal_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/flash_attention_jax/cosine_sim_flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     6715 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/flash_attention_jax/flash_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/flash_attention_jax/rabe_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/flash_attention_jax/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-18 17:53:40.365268 flash-attention-jax-0.3.0/flash_attention_jax.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-18 17:53:40.000000 flash-attention-jax-0.3.0/flash_attention_jax.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-18 17:53:40.000000 flash-attention-jax-0.3.0/flash_attention_jax.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-18 17:53:40.000000 flash-attention-jax-0.3.0/flash_attention_jax.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-18 17:53:40.000000 flash-attention-jax-0.3.0/flash_attention_jax.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-18 17:53:40.000000 flash-attention-jax-0.3.0/flash_attention_jax.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-18 17:53:40.365268 flash-attention-jax-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-06-18 17:53:27.000000 flash-attention-jax-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:45:07.548808 flash-attention-jax-0.3.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-18 02:44:56.000000 flash-attention-jax-0.3.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-18 02:45:07.548808 flash-attention-jax-0.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2647 2023-07-18 02:44:56.000000 flash-attention-jax-0.3.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:45:07.548808 flash-attention-jax-0.3.1/flash_attention_jax/
+-rw-r--r--   0 runner    (1001) docker     (123)      494 2023-07-18 02:44:56.000000 flash-attention-jax-0.3.1/flash_attention_jax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-18 02:44:56.000000 flash-attention-jax-0.3.1/flash_attention_jax/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7448 2023-07-18 02:44:56.000000 flash-attention-jax-0.3.1/flash_attention_jax/causal_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5822 2023-07-18 02:44:56.000000 flash-attention-jax-0.3.1/flash_attention_jax/cosine_sim_flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-18 02:44:56.000000 flash-attention-jax-0.3.1/flash_attention_jax/flash_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-18 02:44:56.000000 flash-attention-jax-0.3.1/flash_attention_jax/rabe_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1348 2023-07-18 02:44:56.000000 flash-attention-jax-0.3.1/flash_attention_jax/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 02:45:07.548808 flash-attention-jax-0.3.1/flash_attention_jax.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-07-18 02:45:07.000000 flash-attention-jax-0.3.1/flash_attention_jax.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-07-18 02:45:07.000000 flash-attention-jax-0.3.1/flash_attention_jax.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 02:45:07.000000 flash-attention-jax-0.3.1/flash_attention_jax.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 02:45:07.000000 flash-attention-jax-0.3.1/flash_attention_jax.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 02:45:07.000000 flash-attention-jax-0.3.1/flash_attention_jax.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 02:45:07.548808 flash-attention-jax-0.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-18 02:44:56.000000 flash-attention-jax-0.3.1/setup.py
```

### Comparing `flash-attention-jax-0.3.0/LICENSE` & `flash-attention-jax-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flash-attention-jax-0.3.0/PKG-INFO` & `flash-attention-jax-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flash-attention-jax
-Version: 0.3.0
+Version: 0.3.1
 Summary: Flash Attention - in Jax
 Home-page: https://github.com/lucidrains/flash-attention-jax
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,jax
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flash-attention-jax-0.3.0/README.md` & `flash-attention-jax-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `flash-attention-jax-0.3.0/flash_attention_jax/attention.py` & `flash-attention-jax-0.3.1/flash_attention_jax/attention.py`

 * *Files identical despite different names*

### Comparing `flash-attention-jax-0.3.0/flash_attention_jax/causal_flash_attention.py` & `flash-attention-jax-0.3.1/flash_attention_jax/causal_flash_attention.py`

 * *Files identical despite different names*

### Comparing `flash-attention-jax-0.3.0/flash_attention_jax/cosine_sim_flash_attention.py` & `flash-attention-jax-0.3.1/flash_attention_jax/cosine_sim_flash_attention.py`

 * *Files identical despite different names*

### Comparing `flash-attention-jax-0.3.0/flash_attention_jax/flash_attention.py` & `flash-attention-jax-0.3.1/flash_attention_jax/flash_attention.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,30 +34,28 @@
         attn_weights = einsum('i ... d, j ... d -> i ... j', q_scaled, k_chunk)
 
         key_mask_chunk = rearrange(key_mask_chunk, 'j b -> 1 b 1 j')
         attn_weights = jnp.where(key_mask_chunk, attn_weights, MASK_VALUE)
 
         block_row_max = jnp.max(attn_weights, axis = -1, keepdims = True)
 
-        exp_weights = jnp.exp(attn_weights - block_row_max)
+        new_row_max = jnp.maximum(block_row_max, row_max)
+        exp_weights = jnp.exp(attn_weights - new_row_max)
 
         exp_weights = jnp.where(key_mask_chunk, exp_weights, 0.)
         block_row_sum = jnp.sum(exp_weights, axis = -1, keepdims = True) + EPSILON
 
         exp_values = einsum('i ... j, j ... d -> i ... d', exp_weights, v_chunk)
 
-        new_row_max = jnp.maximum(block_row_max, row_max)
-
         exp_row_max_diff = jnp.exp(row_max - new_row_max)
-        exp_block_row_max_diff = jnp.exp(block_row_max - new_row_max)
 
-        new_row_sum = exp_row_max_diff * row_sum + exp_block_row_max_diff * block_row_sum
+        new_row_sum = exp_row_max_diff * row_sum + block_row_sum
 
         out = (row_sum / new_row_sum) * exp_row_max_diff * out + \
-              (exp_block_row_max_diff / new_row_sum) * exp_values
+              (1. / new_row_sum) * exp_values
 
         return (chunk_idx + k_chunk_sizes, out, new_row_sum, new_row_max), None
 
     out = jnp.zeros((q_len, batch, heads, dim))
     row_sum = jnp.zeros((q_len, batch, heads, 1))
     row_max = jnp.ones((q_len, batch, heads, 1)) * -1e6
```

### Comparing `flash-attention-jax-0.3.0/flash_attention_jax/rabe_attention.py` & `flash-attention-jax-0.3.1/flash_attention_jax/rabe_attention.py`

 * *Files identical despite different names*

### Comparing `flash-attention-jax-0.3.0/flash_attention_jax/utils.py` & `flash-attention-jax-0.3.1/flash_attention_jax/utils.py`

 * *Files identical despite different names*

### Comparing `flash-attention-jax-0.3.0/flash_attention_jax.egg-info/PKG-INFO` & `flash-attention-jax-0.3.1/flash_attention_jax.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flash-attention-jax
-Version: 0.3.0
+Version: 0.3.1
 Summary: Flash Attention - in Jax
 Home-page: https://github.com/lucidrains/flash-attention-jax
 Author: Phil Wang
 Author-email: lucidrains@gmail.com
 License: MIT
 Keywords: artificial intelligence,deep learning,transformers,attention mechanism,jax
 Classifier: Development Status :: 4 - Beta
```

### Comparing `flash-attention-jax-0.3.0/setup.py` & `flash-attention-jax-0.3.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
   name = 'flash-attention-jax',
   packages = find_packages(exclude=[]),
-  version = '0.3.0',
+  version = '0.3.1',
   license='MIT',
   description = 'Flash Attention - in Jax',
   author = 'Phil Wang',
   author_email = 'lucidrains@gmail.com',
   long_description_content_type = 'text/markdown',
   url = 'https://github.com/lucidrains/flash-attention-jax',
   keywords = [
```

