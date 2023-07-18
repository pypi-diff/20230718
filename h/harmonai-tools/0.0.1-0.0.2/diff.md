# Comparing `tmp/harmonai-tools-0.0.1.tar.gz` & `tmp/harmonai-tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "harmonai-tools-0.0.1.tar", last modified: Thu Jul 13 19:49:02 2023, max compression
+gzip compressed data, was "harmonai-tools-0.0.2.tar", last modified: Tue Jul 18 06:06:43 2023, max compression
```

## Comparing `harmonai-tools-0.0.1.tar` & `harmonai-tools-0.0.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-13 19:49:02.000000 harmonai-tools-0.0.1/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1069 2023-06-19 21:12:07.000000 harmonai-tools-0.0.1/LICENSE
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-13 19:49:02.000000 harmonai-tools-0.0.1/PKG-INFO
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       68 2023-07-13 19:15:43.000000 harmonai-tools-0.0.1/README.md
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-13 19:49:02.000000 harmonai-tools-0.0.1/harmonai_tools/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.1/harmonai_tools/__init__.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-13 19:49:02.000000 harmonai-tools-0.0.1/harmonai_tools/data/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.1/harmonai_tools/data/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18238 2023-06-26 23:30:32.000000 harmonai-tools-0.0.1/harmonai_tools/data/dataset.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     2655 2023-06-19 21:12:07.000000 harmonai-tools-0.0.1/harmonai_tools/data/utils.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-13 19:49:02.000000 harmonai-tools-0.0.1/harmonai_tools/inference/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.1/harmonai_tools/inference/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     2931 2023-07-13 09:03:05.000000 harmonai-tools-0.0.1/harmonai_tools/inference/generation.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5195 2023-07-10 05:18:12.000000 harmonai-tools-0.0.1/harmonai_tools/inference/sampling.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-13 19:49:02.000000 harmonai-tools-0.0.1/harmonai_tools/interface/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-22 00:20:37.000000 harmonai-tools-0.0.1/harmonai_tools/interface/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4472 2023-07-10 05:25:04.000000 harmonai-tools-0.0.1/harmonai_tools/interface/gradio.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-13 19:49:02.000000 harmonai-tools-0.0.1/harmonai_tools/models/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       45 2023-06-19 21:12:07.000000 harmonai-tools-0.0.1/harmonai_tools/models/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    15254 2023-07-12 02:44:15.000000 harmonai-tools-0.0.1/harmonai_tools/models/autoencoders.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     6123 2023-06-22 21:58:42.000000 harmonai-tools-0.0.1/harmonai_tools/models/blocks.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5654 2023-07-12 03:17:02.000000 harmonai-tools-0.0.1/harmonai_tools/models/bottleneck.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    11713 2023-07-12 06:04:16.000000 harmonai-tools-0.0.1/harmonai_tools/models/conditioners.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    17273 2023-07-13 17:20:04.000000 harmonai-tools-0.0.1/harmonai_tools/models/diffusion.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     9412 2023-06-23 05:00:00.000000 harmonai-tools-0.0.1/harmonai_tools/models/discriminators.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4114 2023-07-12 03:20:54.000000 harmonai-tools-0.0.1/harmonai_tools/models/factory.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1506 2023-07-03 19:04:07.000000 harmonai-tools-0.0.1/harmonai_tools/models/pretransforms.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3240 2023-06-19 21:12:07.000000 harmonai-tools-0.0.1/harmonai_tools/models/wavelets.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-13 19:49:02.000000 harmonai-tools-0.0.1/harmonai_tools/training/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       91 2023-07-12 02:18:56.000000 harmonai-tools-0.0.1/harmonai_tools/training/__init__.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    11635 2023-07-12 03:28:38.000000 harmonai-tools-0.0.1/harmonai_tools/training/autoencoders.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18736 2023-07-11 18:15:31.000000 harmonai-tools-0.0.1/harmonai_tools/training/diffusion.py
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4457 2023-07-12 02:51:29.000000 harmonai-tools-0.0.1/harmonai_tools/training/factory.py
-drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-13 19:49:02.000000 harmonai-tools-0.0.1/harmonai_tools.egg-info/
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-13 19:49:02.000000 harmonai-tools-0.0.1/harmonai_tools.egg-info/PKG-INFO
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1041 2023-07-13 19:49:02.000000 harmonai-tools-0.0.1/harmonai_tools.egg-info/SOURCES.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        1 2023-07-13 19:49:02.000000 harmonai-tools-0.0.1/harmonai_tools.egg-info/dependency_links.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      418 2023-07-13 19:49:02.000000 harmonai-tools-0.0.1/harmonai_tools.egg-info/requires.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       15 2023-07-13 19:49:02.000000 harmonai-tools-0.0.1/harmonai_tools.egg-info/top_level.txt
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       80 2023-07-13 19:16:59.000000 harmonai-tools-0.0.1/pyproject.toml
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       38 2023-07-13 19:49:02.000000 harmonai-tools-0.0.1/setup.cfg
--rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1097 2023-07-13 19:48:20.000000 harmonai-tools-0.0.1/setup.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1069 2023-06-19 21:12:07.000000 harmonai-tools-0.0.2/LICENSE
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/PKG-INFO
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       68 2023-07-13 19:15:43.000000 harmonai-tools-0.0.2/README.md
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.2/harmonai_tools/__init__.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools/data/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.2/harmonai_tools/data/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18238 2023-06-26 23:30:32.000000 harmonai-tools-0.0.2/harmonai_tools/data/dataset.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     2655 2023-06-19 21:12:07.000000 harmonai-tools-0.0.2/harmonai_tools/data/utils.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools/inference/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-19 21:12:07.000000 harmonai-tools-0.0.2/harmonai_tools/inference/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     2931 2023-07-13 09:03:05.000000 harmonai-tools-0.0.2/harmonai_tools/inference/generation.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5195 2023-07-10 05:18:12.000000 harmonai-tools-0.0.2/harmonai_tools/inference/sampling.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools/interface/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        0 2023-06-22 00:20:37.000000 harmonai-tools-0.0.2/harmonai_tools/interface/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4472 2023-07-10 05:25:04.000000 harmonai-tools-0.0.2/harmonai_tools/interface/gradio.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools/models/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       45 2023-06-19 21:12:07.000000 harmonai-tools-0.0.2/harmonai_tools/models/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    15254 2023-07-12 02:44:15.000000 harmonai-tools-0.0.2/harmonai_tools/models/autoencoders.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     6123 2023-06-22 21:58:42.000000 harmonai-tools-0.0.2/harmonai_tools/models/blocks.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     5654 2023-07-12 03:17:02.000000 harmonai-tools-0.0.2/harmonai_tools/models/bottleneck.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    11828 2023-07-15 04:13:53.000000 harmonai-tools-0.0.2/harmonai_tools/models/conditioners.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    17998 2023-07-15 04:57:40.000000 harmonai-tools-0.0.2/harmonai_tools/models/diffusion.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     9412 2023-06-23 05:00:00.000000 harmonai-tools-0.0.2/harmonai_tools/models/discriminators.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4114 2023-07-12 03:20:54.000000 harmonai-tools-0.0.2/harmonai_tools/models/factory.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1506 2023-07-03 19:04:07.000000 harmonai-tools-0.0.2/harmonai_tools/models/pretransforms.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     3240 2023-06-19 21:12:07.000000 harmonai-tools-0.0.2/harmonai_tools/models/wavelets.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools/training/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       91 2023-07-12 02:18:56.000000 harmonai-tools-0.0.2/harmonai_tools/training/__init__.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    11635 2023-07-15 02:48:45.000000 harmonai-tools-0.0.2/harmonai_tools/training/autoencoders.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)    18736 2023-07-11 18:15:31.000000 harmonai-tools-0.0.2/harmonai_tools/training/diffusion.py
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     4457 2023-07-12 02:51:29.000000 harmonai-tools-0.0.2/harmonai_tools/training/factory.py
+drwxr-xr-x   0 fauno    (424401618) Domain Users (424400513)        0 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools.egg-info/
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      239 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools.egg-info/PKG-INFO
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1041 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)        1 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)      409 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools.egg-info/requires.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       15 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/harmonai_tools.egg-info/top_level.txt
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       80 2023-07-13 19:16:59.000000 harmonai-tools-0.0.2/pyproject.toml
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)       38 2023-07-18 06:06:43.000000 harmonai-tools-0.0.2/setup.cfg
+-rw-r--r--   0 fauno    (424401618) Domain Users (424400513)     1088 2023-07-18 06:06:26.000000 harmonai-tools-0.0.2/setup.py
```

### Comparing `harmonai-tools-0.0.1/LICENSE` & `harmonai-tools-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/harmonai_tools/data/dataset.py` & `harmonai-tools-0.0.2/harmonai_tools/data/dataset.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/harmonai_tools/data/utils.py` & `harmonai-tools-0.0.2/harmonai_tools/data/utils.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/harmonai_tools/inference/generation.py` & `harmonai-tools-0.0.2/harmonai_tools/inference/generation.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/harmonai_tools/inference/sampling.py` & `harmonai-tools-0.0.2/harmonai_tools/inference/sampling.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/harmonai_tools/interface/gradio.py` & `harmonai-tools-0.0.2/harmonai_tools/interface/gradio.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/harmonai_tools/models/autoencoders.py` & `harmonai-tools-0.0.2/harmonai_tools/models/autoencoders.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/harmonai_tools/models/blocks.py` & `harmonai-tools-0.0.2/harmonai_tools/models/blocks.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/harmonai_tools/models/bottleneck.py` & `harmonai-tools-0.0.2/harmonai_tools/models/bottleneck.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/harmonai_tools/models/conditioners.py` & `harmonai-tools-0.0.2/harmonai_tools/models/conditioners.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #Heavily influenced by https://github.com/facebookresearch/audiocraft/blob/main/audiocraft/modules/conditioners.py
 
 import torch
 import logging, warnings
 import typing as tp
 import gc
 
-from audio_diffusion_pytorch import NumberEmbedder
+from audio_diffusion_pytorch_fork import NumberEmbedder
 
 from torch import nn
 
 class Conditioner(nn.Module):
     def __init__(
             self,
             dim: int,
@@ -300,24 +300,30 @@
     Args:
         config: the conditioning config dictionary
         device: the device to put the conditioners on
     """
     conditioners = {}
     cond_dim = config["cond_dim"]
 
-    for conditioner_config in config["configs"]:
-        id = conditioner_config["id"]
+    for conditioner_info in config["configs"]:
+        id = conditioner_info["id"]
 
-        conditioner_type = conditioner_config["type"]
+        conditioner_type = conditioner_info["type"]
+
+        conditioner_config = {"output_dim": cond_dim}
+        
+        conditioner_config.update(conditioner_info["config"])
 
         if conditioner_type == "t5":
-            conditioners[id] = T5Conditioner(output_dim=cond_dim, **conditioner_config["config"])
+            conditioners[id] = T5Conditioner(**conditioner_config)
         elif conditioner_type == "clap_text":
-            conditioners[id] = CLAPTextConditioner(output_dim=cond_dim, **conditioner_config["config"])
+            conditioners[id] = CLAPTextConditioner(**conditioner_config)
         elif conditioner_type == "clap_audio":
-            conditioners[id] = CLAPAudioConditioner(output_dim=cond_dim, **conditioner_config["config"])
+            conditioners[id] = CLAPAudioConditioner(**conditioner_config)
         elif conditioner_type == "int":
-            conditioners[id] = IntConditioner(output_dim=cond_dim, **conditioner_config["config"])
+            conditioners[id] = IntConditioner(**conditioner_config)
+        elif conditioner_type == "number":
+            conditioners[id] = NumberConditioner(**conditioner_config)
         else:
             raise ValueError(f"Unknown conditioner type: {conditioner_type}")
 
     return MultiConditioner(conditioners)
```

### Comparing `harmonai-tools-0.0.1/harmonai_tools/models/diffusion.py` & `harmonai-tools-0.0.2/harmonai_tools/models/diffusion.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from .blocks import ResConvBlock, FourierFeatures, Upsample1d, Upsample1d_2, Downsample1d, Downsample1d_2, SelfAttention1d, SkipBlock, expand_to_planes
 from .factory import create_pretransform_from_config
 from .conditioners import MultiConditioner, create_multi_conditioner_from_conditioning_config
 from .pretransforms import Pretransform
 from ..inference.generation import generate_diffusion_cond
 
-from audio_diffusion_pytorch.modules import UNetCFG1d
+from audio_diffusion_pytorch_fork.modules import UNetCFG1d
 
 from time import time
 
 class Profiler:
 
     def __init__(self):
         self.ticks = [[time(), None]]
@@ -86,35 +86,48 @@
     def __init__(
             self, 
             model: ConditionedDiffusionModel,
             conditioner: MultiConditioner,
             io_channels = 2,
             pretransform: Pretransform = None,
             cross_attn_cond_ids: tp.List[str] = [],
+            global_cond_ids: tp.List[str] = [],
             ):
         super().__init__()
 
         self.model = model
         self.conditioner = conditioner
         self.io_channels = io_channels
         self.pretransform = pretransform
         self.cross_attn_cond_ids = cross_attn_cond_ids
+        self.global_cond_ids = global_cond_ids
 
     def get_conditioning_inputs(self, cond: tp.Dict[str, tp.Any]):
         cross_attention_input = None
+        cross_attention_masks = None
+        global_cond = None
 
         if len(self.cross_attn_cond_ids) > 0:
             # Concatenate all cross-attention inputs over the sequence dimension
             # Assumes that the cross-attention inputs are of shape (batch, seq, channels)
             cross_attention_input = torch.cat([cond[key][0] for key in self.cross_attn_cond_ids], dim=1)
             cross_attention_masks = torch.cat([cond[key][1] for key in self.cross_attn_cond_ids], dim=1)
 
+        if len(self.global_cond_ids) > 0:
+            # Concatenate all global conditioning inputs over the channel dimension
+            # Assumes that the global conditioning inputs are of shape (batch, channels)
+            global_cond = torch.cat([cond[key][0] for key in self.global_cond_ids], dim=-1)
+            if len(global_cond.shape) == 3:
+                global_cond = global_cond.squeeze(1)
+        
+
         return {
             "cross_attn_cond": cross_attention_input,
-            "cross_attn_masks": cross_attention_masks
+            "cross_attn_masks": cross_attention_masks,
+            "global_cond": global_cond
         }
 
     def forward(self, x: torch.Tensor, t: torch.Tensor, cond: tp.Dict[str, tp.Any], **kwargs):
         outputs = self.model(x, t, **self.get_conditioning_inputs(cond), **kwargs)
         return outputs
     
     def generate(self, *args, **kwargs):
@@ -474,19 +487,21 @@
 
     conditioning_config = model_config.get('conditioning', None)
     assert conditioning_config is not None, "Must specify conditioning config"
 
     conditioner = create_multi_conditioner_from_conditioning_config(conditioning_config)
 
     cross_attention_ids = diffusion_config.get('cross_attention_cond_ids', [])
+    global_cond_ids = diffusion_config.get('global_cond_ids', [])
 
     pretransform = model_config.get("pretransform", None)
     if pretransform is not None:
         pretransform = create_pretransform_from_config(pretransform)
 
     return ConditionedDiffusionModelWrapper(
         diffusion_model, 
         conditioner, 
         cross_attn_cond_ids=cross_attention_ids,
+        global_cond_ids=global_cond_ids,
         pretransform=pretransform, 
         io_channels=io_channels
     )
```

### Comparing `harmonai-tools-0.0.1/harmonai_tools/models/discriminators.py` & `harmonai-tools-0.0.2/harmonai_tools/models/discriminators.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/harmonai_tools/models/factory.py` & `harmonai-tools-0.0.2/harmonai_tools/models/factory.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/harmonai_tools/models/pretransforms.py` & `harmonai-tools-0.0.2/harmonai_tools/models/pretransforms.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/harmonai_tools/models/wavelets.py` & `harmonai-tools-0.0.2/harmonai_tools/models/wavelets.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/harmonai_tools/training/autoencoders.py` & `harmonai-tools-0.0.2/harmonai_tools/training/autoencoders.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
             l1_time_loss = l1_time_loss * self.loss_config['time']['weights']['l1']
 
             # Combine spectral loss, KL loss, time-domain loss, and adversarial loss
             loss = mrstft_loss + loss_adv + feature_matching_distance #+ l1_time_loss
 
             if isinstance(self.autoencoder.bottleneck, VAEBottleneck) or isinstance(self.autoencoder.bottleneck, DACRVQVAEBottleneck) or isinstance(self.autoencoder.bottleneck, RVQVAEBottleneck):
                 kl = encoder_info['kl']
-                kl_loss = 1e-4 * kl 
+                kl_loss = 1e-6 * kl 
                 loss = loss + kl_loss
 
             if isinstance(self.autoencoder.bottleneck, RVQBottleneck) or isinstance(self.autoencoder.bottleneck, RVQVAEBottleneck):
                 quantizer_loss = encoder_info['quantizer_loss']
                 loss = loss + quantizer_loss
                 
             if isinstance(self.autoencoder.bottleneck, DACRVQBottleneck) or isinstance(self.autoencoder.bottleneck, DACRVQVAEBottleneck):
```

### Comparing `harmonai-tools-0.0.1/harmonai_tools/training/diffusion.py` & `harmonai-tools-0.0.2/harmonai_tools/training/diffusion.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/harmonai_tools/training/factory.py` & `harmonai-tools-0.0.2/harmonai_tools/training/factory.py`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/harmonai_tools.egg-info/SOURCES.txt` & `harmonai-tools-0.0.2/harmonai_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `harmonai-tools-0.0.1/setup.py` & `harmonai-tools-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 
 setup(
     name='harmonai-tools',
-    version='0.0.1',
+    version='0.0.2',
     url='https://github.com/Harmonai-org/harmonai-tools.git',
     author='Harmonai',
     description='Training and inference tools for generative audio models from Harmonai',
     packages=find_packages(),  
     install_requires=[
         'aeiou',
         'alias-free-torch',
-        'audio-diffusion-pytorch-fork==0.0.101',
+        'audio-diffusion-pytorch-fork',
         'audio-metadata',
         'auraloss',
         'descript-audio-codec',
         'einops',
         'ema-pytorch',
         'encodec',
         'gradio',
```

