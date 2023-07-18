# Comparing `tmp/model_constructor-0.4.tar.gz` & `tmp/model_constructor-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_constructor-0.4.tar", last modified: Mon Jul 10 13:23:02 2023, max compression
+gzip compressed data, was "model_constructor-0.4.1.tar", last modified: Tue Jul 18 14:30:25 2023, max compression
```

## Comparing `model_constructor-0.4.tar` & `model_constructor-0.4.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-10 13:23:02.112471 model_constructor-0.4/
--rw-rw-r--   0 aya       (1000) aya       (1000)     2348 2021-12-22 07:36:39.000000 model_constructor-0.4/CONTRIBUTING.md
--rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2021-12-22 07:36:39.000000 model_constructor-0.4/LICENSE
--rw-rw-r--   0 aya       (1000) aya       (1000)      111 2021-12-22 07:36:39.000000 model_constructor-0.4/MANIFEST.in
--rw-rw-r--   0 aya       (1000) aya       (1000)    38242 2023-07-10 13:23:02.112471 model_constructor-0.4/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)    37725 2023-07-07 16:51:56.000000 model_constructor-0.4/README.md
--rw-rw-r--   0 aya       (1000) aya       (1000)      752 2022-08-02 08:52:12.000000 model_constructor-0.4/settings.ini
--rw-rw-r--   0 aya       (1000) aya       (1000)      690 2023-07-10 13:23:02.112471 model_constructor-0.4/setup.cfg
--rw-rw-r--   0 aya       (1000) aya       (1000)      597 2022-11-16 08:37:06.000000 model_constructor-0.4/setup.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-10 13:23:02.104471 model_constructor-0.4/src/
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-10 13:23:02.108471 model_constructor-0.4/src/model_constructor/
--rw-rw-r--   0 aya       (1000) aya       (1000)      124 2023-07-06 10:40:14.000000 model_constructor-0.4/src/model_constructor/__init__.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     4903 2023-07-06 10:40:14.000000 model_constructor-0.4/src/model_constructor/activations.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     8963 2023-07-10 12:49:31.000000 model_constructor-0.4/src/model_constructor/base_constructor.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     6144 2023-07-10 12:11:14.000000 model_constructor-0.4/src/model_constructor/blocks.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     5461 2023-07-10 12:47:21.000000 model_constructor-0.4/src/model_constructor/convmixer.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     4464 2023-07-10 13:06:56.000000 model_constructor-0.4/src/model_constructor/helpers.py
--rw-rw-r--   0 aya       (1000) aya       (1000)    10091 2023-07-10 12:44:50.000000 model_constructor-0.4/src/model_constructor/layers.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     7847 2023-07-10 12:49:20.000000 model_constructor-0.4/src/model_constructor/model_constructor.py
--rw-rw-r--   0 aya       (1000) aya       (1000)      364 2023-07-10 12:31:14.000000 model_constructor-0.4/src/model_constructor/mxresnet.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     9349 2023-07-10 12:50:04.000000 model_constructor-0.4/src/model_constructor/net.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     7220 2023-07-10 12:50:10.000000 model_constructor-0.4/src/model_constructor/twist.py
--rw-rw-r--   0 aya       (1000) aya       (1000)    11851 2023-07-10 12:45:33.000000 model_constructor-0.4/src/model_constructor/universal_blocks.py
--rw-rw-r--   0 aya       (1000) aya       (1000)       20 2023-07-10 13:11:31.000000 model_constructor-0.4/src/model_constructor/version.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1581 2023-07-10 12:35:45.000000 model_constructor-0.4/src/model_constructor/xresnet.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     6371 2023-07-10 12:35:59.000000 model_constructor-0.4/src/model_constructor/yaresnet.py
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-10 13:23:02.112471 model_constructor-0.4/src/model_constructor.egg-info/
--rw-rw-r--   0 aya       (1000) aya       (1000)    38242 2023-07-10 13:23:02.000000 model_constructor-0.4/src/model_constructor.egg-info/PKG-INFO
--rw-rw-r--   0 aya       (1000) aya       (1000)     1089 2023-07-10 13:23:02.000000 model_constructor-0.4/src/model_constructor.egg-info/SOURCES.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-07-10 13:23:02.000000 model_constructor-0.4/src/model_constructor.egg-info/dependency_links.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       67 2023-07-10 13:23:02.000000 model_constructor-0.4/src/model_constructor.egg-info/requires.txt
--rw-rw-r--   0 aya       (1000) aya       (1000)       18 2023-07-10 13:23:02.000000 model_constructor-0.4/src/model_constructor.egg-info/top_level.txt
-drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-10 13:23:02.112471 model_constructor-0.4/tests/
--rw-rw-r--   0 aya       (1000) aya       (1000)     3889 2022-12-21 15:06:47.000000 model_constructor-0.4/tests/test_Net.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1791 2023-07-06 10:40:14.000000 model_constructor-0.4/tests/test_blocks.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1840 2023-05-24 06:20:35.000000 model_constructor-0.4/tests/test_blocks_universal.py
--rw-rw-r--   0 aya       (1000) aya       (1000)      902 2022-12-21 15:06:47.000000 model_constructor-0.4/tests/test_convmixer.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     2668 2023-07-07 10:14:14.000000 model_constructor-0.4/tests/test_helpers.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     2870 2023-05-24 06:20:35.000000 model_constructor-0.4/tests/test_layers.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1669 2022-12-21 15:06:47.000000 model_constructor-0.4/tests/test_layers_depr.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     5040 2023-07-10 13:07:26.000000 model_constructor-0.4/tests/test_mc.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1325 2023-07-10 12:32:36.000000 model_constructor-0.4/tests/test_models.py
--rw-rw-r--   0 aya       (1000) aya       (1000)      995 2023-05-24 06:20:35.000000 model_constructor-0.4/tests/test_models_old.py
--rw-rw-r--   0 aya       (1000) aya       (1000)     1070 2023-07-10 12:33:17.000000 model_constructor-0.4/tests/test_models_universal_blocks.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-18 14:30:25.522948 model_constructor-0.4.1/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2348 2022-02-08 06:59:50.000000 model_constructor-0.4.1/CONTRIBUTING.md
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11357 2022-02-08 06:59:50.000000 model_constructor-0.4.1/LICENSE
+-rw-rw-r--   0 aya       (1000) aya       (1000)      111 2022-02-08 06:59:56.000000 model_constructor-0.4.1/MANIFEST.in
+-rw-rw-r--   0 aya       (1000) aya       (1000)    39217 2023-07-18 14:30:25.522948 model_constructor-0.4.1/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)    38698 2023-07-18 14:08:05.000000 model_constructor-0.4.1/README.md
+-rw-rw-r--   0 aya       (1000) aya       (1000)      752 2022-06-06 13:41:36.000000 model_constructor-0.4.1/settings.ini
+-rw-rw-r--   0 aya       (1000) aya       (1000)      690 2023-07-18 14:30:25.522948 model_constructor-0.4.1/setup.cfg
+-rw-rw-r--   0 aya       (1000) aya       (1000)      597 2022-11-16 08:39:29.000000 model_constructor-0.4.1/setup.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-18 14:30:25.514948 model_constructor-0.4.1/src/
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-18 14:30:25.518948 model_constructor-0.4.1/src/model_constructor/
+-rw-rw-r--   0 aya       (1000) aya       (1000)      124 2023-07-17 11:33:03.000000 model_constructor-0.4.1/src/model_constructor/__init__.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4903 2023-07-17 11:33:03.000000 model_constructor-0.4.1/src/model_constructor/activations.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     8963 2023-07-17 11:33:03.000000 model_constructor-0.4.1/src/model_constructor/base_constructor.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     6144 2023-07-17 11:33:03.000000 model_constructor-0.4.1/src/model_constructor/blocks.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     5461 2023-07-17 11:33:03.000000 model_constructor-0.4.1/src/model_constructor/convmixer.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     4886 2023-07-18 13:31:48.000000 model_constructor-0.4.1/src/model_constructor/helpers.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)    10091 2023-07-17 11:33:03.000000 model_constructor-0.4.1/src/model_constructor/layers.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     7847 2023-07-17 11:33:03.000000 model_constructor-0.4.1/src/model_constructor/model_constructor.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      364 2023-07-17 11:33:03.000000 model_constructor-0.4.1/src/model_constructor/mxresnet.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     9349 2023-02-27 16:35:27.000000 model_constructor-0.4.1/src/model_constructor/net.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     7220 2023-07-17 11:33:03.000000 model_constructor-0.4.1/src/model_constructor/twist.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)    11851 2023-07-17 11:33:03.000000 model_constructor-0.4.1/src/model_constructor/universal_blocks.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)       22 2023-07-18 14:20:32.000000 model_constructor-0.4.1/src/model_constructor/version.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1581 2023-07-17 11:33:03.000000 model_constructor-0.4.1/src/model_constructor/xresnet.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     6371 2023-07-17 11:33:03.000000 model_constructor-0.4.1/src/model_constructor/yaresnet.py
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-18 14:30:25.518948 model_constructor-0.4.1/src/model_constructor.egg-info/
+-rw-rw-r--   0 aya       (1000) aya       (1000)    39217 2023-07-18 14:30:25.000000 model_constructor-0.4.1/src/model_constructor.egg-info/PKG-INFO
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1089 2023-07-18 14:30:25.000000 model_constructor-0.4.1/src/model_constructor.egg-info/SOURCES.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)        1 2023-07-18 14:30:25.000000 model_constructor-0.4.1/src/model_constructor.egg-info/dependency_links.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       67 2023-07-18 14:30:25.000000 model_constructor-0.4.1/src/model_constructor.egg-info/requires.txt
+-rw-rw-r--   0 aya       (1000) aya       (1000)       18 2023-07-18 14:30:25.000000 model_constructor-0.4.1/src/model_constructor.egg-info/top_level.txt
+drwxrwxr-x   0 aya       (1000) aya       (1000)        0 2023-07-18 14:30:25.522948 model_constructor-0.4.1/tests/
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3889 2023-02-27 16:35:27.000000 model_constructor-0.4.1/tests/test_Net.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1791 2023-07-17 11:33:03.000000 model_constructor-0.4.1/tests/test_blocks.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1840 2023-02-27 16:35:27.000000 model_constructor-0.4.1/tests/test_blocks_universal.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      902 2023-02-27 16:35:27.000000 model_constructor-0.4.1/tests/test_convmixer.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     3121 2023-07-18 13:25:49.000000 model_constructor-0.4.1/tests/test_helpers.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     2870 2023-02-27 16:35:27.000000 model_constructor-0.4.1/tests/test_layers.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1669 2023-02-27 16:35:27.000000 model_constructor-0.4.1/tests/test_layers_depr.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     5040 2023-07-17 11:33:03.000000 model_constructor-0.4.1/tests/test_mc.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1325 2023-07-17 11:33:03.000000 model_constructor-0.4.1/tests/test_models.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)      995 2023-02-27 16:35:27.000000 model_constructor-0.4.1/tests/test_models_old.py
+-rw-rw-r--   0 aya       (1000) aya       (1000)     1070 2023-07-17 11:33:03.000000 model_constructor-0.4.1/tests/test_models_universal_blocks.py
```

### Comparing `model_constructor-0.4/CONTRIBUTING.md` & `model_constructor-0.4.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/LICENSE` & `model_constructor-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/PKG-INFO` & `model_constructor-0.4.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: model_constructor
-Version: 0.4
-Summary: Pytorch models constructor.
-Home-page: https://github.com/ayasyrev/model_constructor
-Author: Yasyrev Andrei
-Author-email: a.yasyrev@gmail.com
-License: apache2
-Keywords: pytorch models
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Provides-Extra: test
-License-File: LICENSE
-
 # model_constructor
 
 > Constructor to create pytorch model. 
 
 ## Install
 
 `pip install model-constructor`
@@ -64,34 +47,47 @@
 Check all parameters with `print_cfg` method:
 
 
 ```python
 mc.print_cfg()
 ```
 <details open> <summary>output</summary>  
-    <pre>ModelConstructor
-      in_chans: 3, num_classes: 1000
-      expansion: 1, groups: 1, dw: False, div_groups: None
-      act_fn: ReLU, sa: False, se: False
-      stem sizes: [64], stride on 0
-      body sizes [64, 128, 256, 512]
-      layers: [2, 2, 2, 2]
+    <pre>ModelConstructor(
+      in_chans=3
+      num_classes=1000
+      block='BasicBlock'
+      conv_layer='ConvBnAct'
+      block_sizes=[64, 128, 256, 512]
+      layers=[2, 2, 2, 2]
+      norm='BatchNorm2d'
+      act_fn='ReLU'
+      expansion=1
+      groups=1
+      bn_1st=True
+      zero_bn=True
+      stem_sizes=[64]
+      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
+      init_cnn='init_cnn'
+      make_stem='make_stem'
+      make_layer='make_layer'
+      make_body='make_body'
+      make_head='make_head')
     </pre>
 </details>
 
 Now we have model constructor, default setting as resnet18. And we can get model after call it.
 
 
 ```python
 
 model = mc()
 model
 ```
 <details> <summary>output</summary>  
-    </pre>ModelConstructor(
+    <pre>ModelConstructor(
       (stem): Sequential(
         (conv_1): ConvBnAct(
           (conv): Conv2d(3, 64, kernel_size=(7, 7), stride=(2, 2), padding=(3, 3), bias=False)
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): ReLU(inplace=True)
         )
         (stem_pool): MaxPool2d(kernel_size=3, stride=2, padding=1, dilation=1, ceil_mode=False)
@@ -274,23 +270,36 @@
 <details open> <summary>output</summary>  
     <pre>Changed fields:
     layers: [3, 4, 6, 3]
     expansion: 4
     </pre>
 </details>
 
+We can compare changed with defaults.
+
+
+```python
+mc.print_changed_fields(show_default=True)
+```
+<details open> <summary>output</summary>  
+    <pre>Changed fields:
+    layers: [3, 4, 6, 3] | [2, 2, 2, 2]
+    expansion: 4 | 1
+    </pre>
+</details>
+
 Now we can look at model parts - stem, body, head.  
 
 
 ```python
 
 mc.body
 ```
 <details> <summary>output</summary>  
-    </pre>Sequential(
+    <pre>Sequential(
       (l_0): Sequential(
         (bl_0): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
               (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
@@ -556,50 +565,58 @@
 cfg = ModelCfg(
     num_classes=10,
     act_fn=nn.Mish,
 )
 print(cfg)
 ```
 <details open> <summary>output</summary>  
-    <pre>in_chans=3 num_classes=10 block='BasicBlock' conv_layer='ConvBnAct' block_sizes=[64, 128, 256, 512] layers=[2, 2, 2, 2] norm='BatchNorm2d' act_fn='Mish' expansion=1 groups=1 bn_1st=True zero_bn=True stem_sizes=[64] stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
+    <pre>ModelCfg(
+      in_chans=3
+      num_classes=10
+      block='BasicBlock'
+      conv_layer='ConvBnAct'
+      block_sizes=[64, 128, 256, 512]
+      layers=[2, 2, 2, 2]
+      norm='BatchNorm2d'
+      act_fn='Mish'
+      expansion=1
+      groups=1
+      bn_1st=True
+      zero_bn=True
+      stem_sizes=[64]
+      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}")
     </pre>
 </details>
 
 When creating config or constructor we can use string annotation for nn.Modules - it useful when creating model from config files.
 
 
 ```python
 cfg = ModelCfg(
     num_classes=10,
     act_fn="nn.SELU",
 )
 print(cfg.act_fn)
 ```
 <details open> <summary>output</summary>  
-    <pre>class 'torch.nn.modules.activation.SELU'
-    </pre>
+    <pre>class 'torch.nn.modules.activation.SELU'</pre>
 </details>
 
 Now we can create constructor from config:
 
 
 ```python
 mc = ModelConstructor.from_cfg(cfg)
 mc
 ```
 <details open> <summary>output</summary>  
-    <pre>Deprecated. Pass se_module as se argument, se_reduction as arg to se.
-    Deprecated. Pass se_module as se argument, se_reduction as arg to se.
-    </pre>
-</details>
-<details open> <summary>output</summary>  
     <pre>ModelConstructor
       in_chans: 3, num_classes: 10
       expansion: 1, groups: 1, dw: False, div_groups: None
-      act_fn: ReLU, sa: <class 'model_constructor.layers.SimpleSelfAttention'>, se: SEModule
+      act_fn: SELU, sa: <class 'model_constructor.layers.SimpleSelfAttention'>, se: SEModule
       stem sizes: [64], stride on 0
       body sizes [64, 128, 256, 512]
       layers: [2, 2, 2, 2]</pre>
 </details>
 
 
 
@@ -678,15 +695,15 @@
 
 
 ```python
 
 mc()
 ```
 <details> <summary>output</summary>  
-    </pre>MxResNet(
+    <pre>MxResNet(
       act_fn: Mish, stem_sizes: [3, 32, 64, 64], make_stem: xresnet_stem
       (stem): Sequential(
         (conv_0): ConvBnAct(
           (conv): Conv2d(3, 3, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(3, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): Mish(inplace=True)
         )
@@ -905,30 +922,30 @@
 
 
 ```python
 
 mc.stem.conv_1
 ```
 <details> <summary>output</summary>  
-    </pre>ConvBnAct(
+    <pre>ConvBnAct(
       (conv): Conv2d(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
       (bn): BatchNorm2d(32, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
       (act_fn): Mish(inplace=True)
     )</pre>
 </details>
 
 
 
 
 ```python
 
 mc.body.l_0.bl_0
 ```
 <details> <summary>output</summary>  
-    </pre>BasicBlock(
+    <pre>BasicBlock(
       (convs): Sequential(
         (conv_0): ConvBnAct(
           (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): Mish(inplace=True)
         )
         (conv_1): ConvBnAct(
@@ -997,33 +1014,47 @@
 
 
 ```python
 
 mc.print_cfg()
 ```
 <details> <summary>output</summary>  
-    </pre>YaResNet
-      in_chans: 3, num_classes: 1000
-      expansion: 1, groups: 1, dw: False, div_groups: None
-      act_fn: ReLU, sa: False, se: False
-      stem sizes: [64], stride on 0
-      body sizes [64, 128, 256, 512]
-      layers: [2, 2, 2, 2]
+    <pre>ModelConstructor(
+      name='YaResNet'
+      in_chans=3
+      num_classes=1000
+      block='YaBasicBlock'
+      conv_layer='ConvBnAct'
+      block_sizes=[64, 128, 256, 512]
+      layers=[2, 2, 2, 2]
+      norm='BatchNorm2d'
+      act_fn='ReLU'
+      expansion=1
+      groups=1
+      bn_1st=True
+      zero_bn=True
+      stem_sizes=[64]
+      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
+      init_cnn='init_cnn'
+      make_stem='make_stem'
+      make_layer='make_layer'
+      make_body='make_body'
+      make_head='make_head')
     </pre>
 </details>
 
 Let see what we have.
 
 
 ```python
 
 mc.body.l_1.bl_0
 ```
 <details> <summary>output</summary>  
-    </pre>YaBasicBlock(
+    <pre>YaBasicBlock(
       (reduce): ConvBnAct(
         (conv): Conv2d(64, 64, kernel_size=(1, 1), stride=(2, 2), bias=False)
         (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
         (act_fn): ReLU(inplace=True)
       )
       (convs): Sequential(
         (conv_0): ConvBnAct(
@@ -1063,21 +1094,34 @@
 
 
 ```python
 mc = YaResnet34()
 mc.print_cfg()
 ```
 <details open> <summary>output</summary>  
-    <pre>YaResnet34
-      in_chans: 3, num_classes: 1000
-      expansion: 1, groups: 1, dw: False, div_groups: None
-      act_fn: ReLU, sa: False, se: False
-      stem sizes: [64], stride on 0
-      body sizes [64, 128, 256, 512]
-      layers: [3, 4, 6, 3]
+    <pre>YaResnet34(
+      in_chans=3
+      num_classes=1000
+      block='YaBasicBlock'
+      conv_layer='ConvBnAct'
+      block_sizes=[64, 128, 256, 512]
+      layers=[3, 4, 6, 3]
+      norm='BatchNorm2d'
+      act_fn='ReLU'
+      expansion=1
+      groups=1
+      bn_1st=True
+      zero_bn=True
+      stem_sizes=[64]
+      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
+      init_cnn='init_cnn'
+      make_stem='xresnet_stem'
+      make_layer='make_layer'
+      make_body='make_body'
+      make_head='make_head')
     </pre>
 </details>
 
 And `xResnet50` like model can be inherited from `YaResnet34`:
 
 
 ```python
```

### Comparing `model_constructor-0.4/README.md` & `model_constructor-0.4.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: model_constructor
+Version: 0.4.1
+Summary: Pytorch models constructor.
+Home-page: https://github.com/ayasyrev/model_constructor
+Author: Yasyrev Andrei
+Author-email: a.yasyrev@gmail.com
+License: apache2
+Keywords: pytorch models
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
 # model_constructor
 
 > Constructor to create pytorch model. 
 
 ## Install
 
 `pip install model-constructor`
@@ -47,34 +64,47 @@
 Check all parameters with `print_cfg` method:
 
 
 ```python
 mc.print_cfg()
 ```
 <details open> <summary>output</summary>  
-    <pre>ModelConstructor
-      in_chans: 3, num_classes: 1000
-      expansion: 1, groups: 1, dw: False, div_groups: None
-      act_fn: ReLU, sa: False, se: False
-      stem sizes: [64], stride on 0
-      body sizes [64, 128, 256, 512]
-      layers: [2, 2, 2, 2]
+    <pre>ModelConstructor(
+      in_chans=3
+      num_classes=1000
+      block='BasicBlock'
+      conv_layer='ConvBnAct'
+      block_sizes=[64, 128, 256, 512]
+      layers=[2, 2, 2, 2]
+      norm='BatchNorm2d'
+      act_fn='ReLU'
+      expansion=1
+      groups=1
+      bn_1st=True
+      zero_bn=True
+      stem_sizes=[64]
+      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
+      init_cnn='init_cnn'
+      make_stem='make_stem'
+      make_layer='make_layer'
+      make_body='make_body'
+      make_head='make_head')
     </pre>
 </details>
 
 Now we have model constructor, default setting as resnet18. And we can get model after call it.
 
 
 ```python
 
 model = mc()
 model
 ```
 <details> <summary>output</summary>  
-    </pre>ModelConstructor(
+    <pre>ModelConstructor(
       (stem): Sequential(
         (conv_1): ConvBnAct(
           (conv): Conv2d(3, 64, kernel_size=(7, 7), stride=(2, 2), padding=(3, 3), bias=False)
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): ReLU(inplace=True)
         )
         (stem_pool): MaxPool2d(kernel_size=3, stride=2, padding=1, dilation=1, ceil_mode=False)
@@ -257,23 +287,36 @@
 <details open> <summary>output</summary>  
     <pre>Changed fields:
     layers: [3, 4, 6, 3]
     expansion: 4
     </pre>
 </details>
 
+We can compare changed with defaults.
+
+
+```python
+mc.print_changed_fields(show_default=True)
+```
+<details open> <summary>output</summary>  
+    <pre>Changed fields:
+    layers: [3, 4, 6, 3] | [2, 2, 2, 2]
+    expansion: 4 | 1
+    </pre>
+</details>
+
 Now we can look at model parts - stem, body, head.  
 
 
 ```python
 
 mc.body
 ```
 <details> <summary>output</summary>  
-    </pre>Sequential(
+    <pre>Sequential(
       (l_0): Sequential(
         (bl_0): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
               (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
@@ -539,50 +582,58 @@
 cfg = ModelCfg(
     num_classes=10,
     act_fn=nn.Mish,
 )
 print(cfg)
 ```
 <details open> <summary>output</summary>  
-    <pre>in_chans=3 num_classes=10 block='BasicBlock' conv_layer='ConvBnAct' block_sizes=[64, 128, 256, 512] layers=[2, 2, 2, 2] norm='BatchNorm2d' act_fn='Mish' expansion=1 groups=1 bn_1st=True zero_bn=True stem_sizes=[64] stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
+    <pre>ModelCfg(
+      in_chans=3
+      num_classes=10
+      block='BasicBlock'
+      conv_layer='ConvBnAct'
+      block_sizes=[64, 128, 256, 512]
+      layers=[2, 2, 2, 2]
+      norm='BatchNorm2d'
+      act_fn='Mish'
+      expansion=1
+      groups=1
+      bn_1st=True
+      zero_bn=True
+      stem_sizes=[64]
+      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}")
     </pre>
 </details>
 
 When creating config or constructor we can use string annotation for nn.Modules - it useful when creating model from config files.
 
 
 ```python
 cfg = ModelCfg(
     num_classes=10,
     act_fn="nn.SELU",
 )
 print(cfg.act_fn)
 ```
 <details open> <summary>output</summary>  
-    <pre>class 'torch.nn.modules.activation.SELU'
-    </pre>
+    <pre>class 'torch.nn.modules.activation.SELU'</pre>
 </details>
 
 Now we can create constructor from config:
 
 
 ```python
 mc = ModelConstructor.from_cfg(cfg)
 mc
 ```
 <details open> <summary>output</summary>  
-    <pre>Deprecated. Pass se_module as se argument, se_reduction as arg to se.
-    Deprecated. Pass se_module as se argument, se_reduction as arg to se.
-    </pre>
-</details>
-<details open> <summary>output</summary>  
     <pre>ModelConstructor
       in_chans: 3, num_classes: 10
       expansion: 1, groups: 1, dw: False, div_groups: None
-      act_fn: ReLU, sa: <class 'model_constructor.layers.SimpleSelfAttention'>, se: SEModule
+      act_fn: SELU, sa: <class 'model_constructor.layers.SimpleSelfAttention'>, se: SEModule
       stem sizes: [64], stride on 0
       body sizes [64, 128, 256, 512]
       layers: [2, 2, 2, 2]</pre>
 </details>
 
 
 
@@ -661,15 +712,15 @@
 
 
 ```python
 
 mc()
 ```
 <details> <summary>output</summary>  
-    </pre>MxResNet(
+    <pre>MxResNet(
       act_fn: Mish, stem_sizes: [3, 32, 64, 64], make_stem: xresnet_stem
       (stem): Sequential(
         (conv_0): ConvBnAct(
           (conv): Conv2d(3, 3, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(3, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): Mish(inplace=True)
         )
@@ -888,30 +939,30 @@
 
 
 ```python
 
 mc.stem.conv_1
 ```
 <details> <summary>output</summary>  
-    </pre>ConvBnAct(
+    <pre>ConvBnAct(
       (conv): Conv2d(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
       (bn): BatchNorm2d(32, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
       (act_fn): Mish(inplace=True)
     )</pre>
 </details>
 
 
 
 
 ```python
 
 mc.body.l_0.bl_0
 ```
 <details> <summary>output</summary>  
-    </pre>BasicBlock(
+    <pre>BasicBlock(
       (convs): Sequential(
         (conv_0): ConvBnAct(
           (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): Mish(inplace=True)
         )
         (conv_1): ConvBnAct(
@@ -980,33 +1031,47 @@
 
 
 ```python
 
 mc.print_cfg()
 ```
 <details> <summary>output</summary>  
-    </pre>YaResNet
-      in_chans: 3, num_classes: 1000
-      expansion: 1, groups: 1, dw: False, div_groups: None
-      act_fn: ReLU, sa: False, se: False
-      stem sizes: [64], stride on 0
-      body sizes [64, 128, 256, 512]
-      layers: [2, 2, 2, 2]
+    <pre>ModelConstructor(
+      name='YaResNet'
+      in_chans=3
+      num_classes=1000
+      block='YaBasicBlock'
+      conv_layer='ConvBnAct'
+      block_sizes=[64, 128, 256, 512]
+      layers=[2, 2, 2, 2]
+      norm='BatchNorm2d'
+      act_fn='ReLU'
+      expansion=1
+      groups=1
+      bn_1st=True
+      zero_bn=True
+      stem_sizes=[64]
+      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
+      init_cnn='init_cnn'
+      make_stem='make_stem'
+      make_layer='make_layer'
+      make_body='make_body'
+      make_head='make_head')
     </pre>
 </details>
 
 Let see what we have.
 
 
 ```python
 
 mc.body.l_1.bl_0
 ```
 <details> <summary>output</summary>  
-    </pre>YaBasicBlock(
+    <pre>YaBasicBlock(
       (reduce): ConvBnAct(
         (conv): Conv2d(64, 64, kernel_size=(1, 1), stride=(2, 2), bias=False)
         (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
         (act_fn): ReLU(inplace=True)
       )
       (convs): Sequential(
         (conv_0): ConvBnAct(
@@ -1046,21 +1111,34 @@
 
 
 ```python
 mc = YaResnet34()
 mc.print_cfg()
 ```
 <details open> <summary>output</summary>  
-    <pre>YaResnet34
-      in_chans: 3, num_classes: 1000
-      expansion: 1, groups: 1, dw: False, div_groups: None
-      act_fn: ReLU, sa: False, se: False
-      stem sizes: [64], stride on 0
-      body sizes [64, 128, 256, 512]
-      layers: [3, 4, 6, 3]
+    <pre>YaResnet34(
+      in_chans=3
+      num_classes=1000
+      block='YaBasicBlock'
+      conv_layer='ConvBnAct'
+      block_sizes=[64, 128, 256, 512]
+      layers=[3, 4, 6, 3]
+      norm='BatchNorm2d'
+      act_fn='ReLU'
+      expansion=1
+      groups=1
+      bn_1st=True
+      zero_bn=True
+      stem_sizes=[64]
+      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
+      init_cnn='init_cnn'
+      make_stem='xresnet_stem'
+      make_layer='make_layer'
+      make_body='make_body'
+      make_head='make_head')
     </pre>
 </details>
 
 And `xResnet50` like model can be inherited from `YaResnet34`:
 
 
 ```python
```

### Comparing `model_constructor-0.4/settings.ini` & `model_constructor-0.4.1/settings.ini`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/setup.cfg` & `model_constructor-0.4.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/setup.py` & `model_constructor-0.4.1/setup.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/src/model_constructor/activations.py` & `model_constructor-0.4.1/src/model_constructor/activations.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/src/model_constructor/base_constructor.py` & `model_constructor-0.4.1/src/model_constructor/base_constructor.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/src/model_constructor/blocks.py` & `model_constructor-0.4.1/src/model_constructor/blocks.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/src/model_constructor/convmixer.py` & `model_constructor-0.4.1/src/model_constructor/convmixer.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/src/model_constructor/helpers.py` & `model_constructor-0.4.1/src/model_constructor/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -52,16 +52,16 @@
                 default_path = "torch.nn"
                 name = path_list[1]
             else:
                 default_path = path_list[0]
                 name = path_list[1]
     try:
         mod = importlib.import_module(default_path)
-    except ImportError:
-        raise ImportError(f"Module {default_path} not found")
+    except ImportError as exc:
+        raise ImportError(f"Module {default_path} not found") from exc
     if hasattr(mod, name):
         module = getattr(mod, name)
         if is_module(module):
             return module
         else:
             raise ImportError(f"Module {name} is not a nn.Module")
     else:
@@ -69,39 +69,47 @@
 
 
 class Cfg(BaseModel):
     """Base class for config."""
 
     name: Optional[str] = None
 
-    def _get_str_value(self, field: str) -> str:
-        value = getattr(self, field)
+    def _get_str(self, value: Any) -> str:
         if isinstance(value, type):
             value = value.__name__
         elif isinstance(value, partial):
             value = f"{value.func.__name__} {value.keywords}"
         elif callable(value):
             value = value.__name__
         return value
 
-    def __repr__(self) -> str:
+    def _get_str_value(self, field: str) -> str:
+        return self._get_str(getattr(self, field))
+
+    def _cfg_str(self) -> str:
         return f"{self.__repr_name__()}(\n  {self.__repr_str__(chr(10) + '  ')})"
 
+    def __repr__(self) -> str:
+        return self._cfg_str()
+
+    def __str__(self) -> str:
+        return self._cfg_str()
+
     def __repr_args__(self) -> List[Tuple[str, str]]:
         return [
             (field, str_value)
             for field in self.model_fields
             if (str_value := self._get_str_value(field))
         ]
 
     def __repr_set_fields__(self) -> List[str]:
         """Return list repr for fields set at init"""
         return [
             f"{field}: {self._get_str_value(field)}"
-            for field in self.model_fields_set  # pylint: disable=E1133
+            for field in self.model_fields_set  # pylint: disable=E1133:not-an-iterable
             if field != "name"
         ]
 
     def __repr_changed_fields__(self) -> List[str]:
         """Return list repr for changed fields"""
         return [
             f"{field}: {self._get_str_value(field)}"
@@ -110,33 +118,36 @@
         ]
 
     @property
     def changed_fields(self) -> Dict[str, Any]:
         # return "\n".join(self.__repr_changed_fields__())
         return {
             field: self._get_str_value(field)
-            for field in self.model_fields  # pylint: disable=E1133
-            if getattr(self, field) != self.model_fields[field].default
+            for field, value in self.model_fields.items()
+            if getattr(self, field) != value.default
         }
 
     def print_cfg(self) -> None:
         """Print full config"""
-        print(repr(self))
+        print(self._cfg_str())
 
     def print_set_fields(self) -> None:
         """Print fields changed at init."""
         set_fields = self.__repr_set_fields__()
         if set_fields:
             print("Set fields:")
             for field in set_fields:
                 print(field)
         else:
             print("Nothing changed")
 
-    def print_changed_fields(self) -> None:
+    def print_changed_fields(self, show_default: bool = False, separator: str = " | ") -> None:
         """Print fields changed at init."""
         if self.changed_fields:
+            default_value = ""
             print("Changed fields:")
             for field in self.changed_fields:
-                print(f"{field}: {self._get_str_value(field)}")
+                if show_default:
+                    default_value = f"{separator}{self._get_str(self.model_fields[field].default)}"
+                print(f"{field}: {self._get_str_value(field)}{default_value}")
         else:
             print("Nothing changed")
```

### Comparing `model_constructor-0.4/src/model_constructor/layers.py` & `model_constructor-0.4.1/src/model_constructor/layers.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/src/model_constructor/model_constructor.py` & `model_constructor-0.4.1/src/model_constructor/model_constructor.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/src/model_constructor/net.py` & `model_constructor-0.4.1/src/model_constructor/net.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/src/model_constructor/twist.py` & `model_constructor-0.4.1/src/model_constructor/twist.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/src/model_constructor/universal_blocks.py` & `model_constructor-0.4.1/src/model_constructor/universal_blocks.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/src/model_constructor/xresnet.py` & `model_constructor-0.4.1/src/model_constructor/xresnet.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/src/model_constructor/yaresnet.py` & `model_constructor-0.4.1/src/model_constructor/yaresnet.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/src/model_constructor.egg-info/PKG-INFO` & `model_constructor-0.4.1/src/model_constructor.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-constructor
-Version: 0.4
+Version: 0.4.1
 Summary: Pytorch models constructor.
 Home-page: https://github.com/ayasyrev/model_constructor
 Author: Yasyrev Andrei
 Author-email: a.yasyrev@gmail.com
 License: apache2
 Keywords: pytorch models
 Classifier: Programming Language :: Python :: 3
@@ -64,34 +64,47 @@
 Check all parameters with `print_cfg` method:
 
 
 ```python
 mc.print_cfg()
 ```
 <details open> <summary>output</summary>  
-    <pre>ModelConstructor
-      in_chans: 3, num_classes: 1000
-      expansion: 1, groups: 1, dw: False, div_groups: None
-      act_fn: ReLU, sa: False, se: False
-      stem sizes: [64], stride on 0
-      body sizes [64, 128, 256, 512]
-      layers: [2, 2, 2, 2]
+    <pre>ModelConstructor(
+      in_chans=3
+      num_classes=1000
+      block='BasicBlock'
+      conv_layer='ConvBnAct'
+      block_sizes=[64, 128, 256, 512]
+      layers=[2, 2, 2, 2]
+      norm='BatchNorm2d'
+      act_fn='ReLU'
+      expansion=1
+      groups=1
+      bn_1st=True
+      zero_bn=True
+      stem_sizes=[64]
+      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
+      init_cnn='init_cnn'
+      make_stem='make_stem'
+      make_layer='make_layer'
+      make_body='make_body'
+      make_head='make_head')
     </pre>
 </details>
 
 Now we have model constructor, default setting as resnet18. And we can get model after call it.
 
 
 ```python
 
 model = mc()
 model
 ```
 <details> <summary>output</summary>  
-    </pre>ModelConstructor(
+    <pre>ModelConstructor(
       (stem): Sequential(
         (conv_1): ConvBnAct(
           (conv): Conv2d(3, 64, kernel_size=(7, 7), stride=(2, 2), padding=(3, 3), bias=False)
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): ReLU(inplace=True)
         )
         (stem_pool): MaxPool2d(kernel_size=3, stride=2, padding=1, dilation=1, ceil_mode=False)
@@ -274,23 +287,36 @@
 <details open> <summary>output</summary>  
     <pre>Changed fields:
     layers: [3, 4, 6, 3]
     expansion: 4
     </pre>
 </details>
 
+We can compare changed with defaults.
+
+
+```python
+mc.print_changed_fields(show_default=True)
+```
+<details open> <summary>output</summary>  
+    <pre>Changed fields:
+    layers: [3, 4, 6, 3] | [2, 2, 2, 2]
+    expansion: 4 | 1
+    </pre>
+</details>
+
 Now we can look at model parts - stem, body, head.  
 
 
 ```python
 
 mc.body
 ```
 <details> <summary>output</summary>  
-    </pre>Sequential(
+    <pre>Sequential(
       (l_0): Sequential(
         (bl_0): BasicBlock(
           (convs): Sequential(
             (conv_0): ConvBnAct(
               (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
               (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
               (act_fn): ReLU(inplace=True)
@@ -556,50 +582,58 @@
 cfg = ModelCfg(
     num_classes=10,
     act_fn=nn.Mish,
 )
 print(cfg)
 ```
 <details open> <summary>output</summary>  
-    <pre>in_chans=3 num_classes=10 block='BasicBlock' conv_layer='ConvBnAct' block_sizes=[64, 128, 256, 512] layers=[2, 2, 2, 2] norm='BatchNorm2d' act_fn='Mish' expansion=1 groups=1 bn_1st=True zero_bn=True stem_sizes=[64] stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
+    <pre>ModelCfg(
+      in_chans=3
+      num_classes=10
+      block='BasicBlock'
+      conv_layer='ConvBnAct'
+      block_sizes=[64, 128, 256, 512]
+      layers=[2, 2, 2, 2]
+      norm='BatchNorm2d'
+      act_fn='Mish'
+      expansion=1
+      groups=1
+      bn_1st=True
+      zero_bn=True
+      stem_sizes=[64]
+      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}")
     </pre>
 </details>
 
 When creating config or constructor we can use string annotation for nn.Modules - it useful when creating model from config files.
 
 
 ```python
 cfg = ModelCfg(
     num_classes=10,
     act_fn="nn.SELU",
 )
 print(cfg.act_fn)
 ```
 <details open> <summary>output</summary>  
-    <pre>class 'torch.nn.modules.activation.SELU'
-    </pre>
+    <pre>class 'torch.nn.modules.activation.SELU'</pre>
 </details>
 
 Now we can create constructor from config:
 
 
 ```python
 mc = ModelConstructor.from_cfg(cfg)
 mc
 ```
 <details open> <summary>output</summary>  
-    <pre>Deprecated. Pass se_module as se argument, se_reduction as arg to se.
-    Deprecated. Pass se_module as se argument, se_reduction as arg to se.
-    </pre>
-</details>
-<details open> <summary>output</summary>  
     <pre>ModelConstructor
       in_chans: 3, num_classes: 10
       expansion: 1, groups: 1, dw: False, div_groups: None
-      act_fn: ReLU, sa: <class 'model_constructor.layers.SimpleSelfAttention'>, se: SEModule
+      act_fn: SELU, sa: <class 'model_constructor.layers.SimpleSelfAttention'>, se: SEModule
       stem sizes: [64], stride on 0
       body sizes [64, 128, 256, 512]
       layers: [2, 2, 2, 2]</pre>
 </details>
 
 
 
@@ -678,15 +712,15 @@
 
 
 ```python
 
 mc()
 ```
 <details> <summary>output</summary>  
-    </pre>MxResNet(
+    <pre>MxResNet(
       act_fn: Mish, stem_sizes: [3, 32, 64, 64], make_stem: xresnet_stem
       (stem): Sequential(
         (conv_0): ConvBnAct(
           (conv): Conv2d(3, 3, kernel_size=(3, 3), stride=(2, 2), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(3, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): Mish(inplace=True)
         )
@@ -905,30 +939,30 @@
 
 
 ```python
 
 mc.stem.conv_1
 ```
 <details> <summary>output</summary>  
-    </pre>ConvBnAct(
+    <pre>ConvBnAct(
       (conv): Conv2d(3, 32, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
       (bn): BatchNorm2d(32, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
       (act_fn): Mish(inplace=True)
     )</pre>
 </details>
 
 
 
 
 ```python
 
 mc.body.l_0.bl_0
 ```
 <details> <summary>output</summary>  
-    </pre>BasicBlock(
+    <pre>BasicBlock(
       (convs): Sequential(
         (conv_0): ConvBnAct(
           (conv): Conv2d(64, 64, kernel_size=(3, 3), stride=(1, 1), padding=(1, 1), bias=False)
           (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
           (act_fn): Mish(inplace=True)
         )
         (conv_1): ConvBnAct(
@@ -997,33 +1031,47 @@
 
 
 ```python
 
 mc.print_cfg()
 ```
 <details> <summary>output</summary>  
-    </pre>YaResNet
-      in_chans: 3, num_classes: 1000
-      expansion: 1, groups: 1, dw: False, div_groups: None
-      act_fn: ReLU, sa: False, se: False
-      stem sizes: [64], stride on 0
-      body sizes [64, 128, 256, 512]
-      layers: [2, 2, 2, 2]
+    <pre>ModelConstructor(
+      name='YaResNet'
+      in_chans=3
+      num_classes=1000
+      block='YaBasicBlock'
+      conv_layer='ConvBnAct'
+      block_sizes=[64, 128, 256, 512]
+      layers=[2, 2, 2, 2]
+      norm='BatchNorm2d'
+      act_fn='ReLU'
+      expansion=1
+      groups=1
+      bn_1st=True
+      zero_bn=True
+      stem_sizes=[64]
+      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
+      init_cnn='init_cnn'
+      make_stem='make_stem'
+      make_layer='make_layer'
+      make_body='make_body'
+      make_head='make_head')
     </pre>
 </details>
 
 Let see what we have.
 
 
 ```python
 
 mc.body.l_1.bl_0
 ```
 <details> <summary>output</summary>  
-    </pre>YaBasicBlock(
+    <pre>YaBasicBlock(
       (reduce): ConvBnAct(
         (conv): Conv2d(64, 64, kernel_size=(1, 1), stride=(2, 2), bias=False)
         (bn): BatchNorm2d(64, eps=1e-05, momentum=0.1, affine=True, track_running_stats=True)
         (act_fn): ReLU(inplace=True)
       )
       (convs): Sequential(
         (conv_0): ConvBnAct(
@@ -1063,21 +1111,34 @@
 
 
 ```python
 mc = YaResnet34()
 mc.print_cfg()
 ```
 <details open> <summary>output</summary>  
-    <pre>YaResnet34
-      in_chans: 3, num_classes: 1000
-      expansion: 1, groups: 1, dw: False, div_groups: None
-      act_fn: ReLU, sa: False, se: False
-      stem sizes: [64], stride on 0
-      body sizes [64, 128, 256, 512]
-      layers: [3, 4, 6, 3]
+    <pre>YaResnet34(
+      in_chans=3
+      num_classes=1000
+      block='YaBasicBlock'
+      conv_layer='ConvBnAct'
+      block_sizes=[64, 128, 256, 512]
+      layers=[3, 4, 6, 3]
+      norm='BatchNorm2d'
+      act_fn='ReLU'
+      expansion=1
+      groups=1
+      bn_1st=True
+      zero_bn=True
+      stem_sizes=[64]
+      stem_pool="MaxPool2d {'kernel_size': 3, 'stride': 2, 'padding': 1}"
+      init_cnn='init_cnn'
+      make_stem='xresnet_stem'
+      make_layer='make_layer'
+      make_body='make_body'
+      make_head='make_head')
     </pre>
 </details>
 
 And `xResnet50` like model can be inherited from `YaResnet34`:
 
 
 ```python
```

### Comparing `model_constructor-0.4/src/model_constructor.egg-info/SOURCES.txt` & `model_constructor-0.4.1/src/model_constructor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/tests/test_Net.py` & `model_constructor-0.4.1/tests/test_Net.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/tests/test_blocks.py` & `model_constructor-0.4.1/tests/test_blocks.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/tests/test_blocks_universal.py` & `model_constructor-0.4.1/tests/test_blocks_universal.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/tests/test_convmixer.py` & `model_constructor-0.4.1/tests/test_convmixer.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/tests/test_helpers.py` & `model_constructor-0.4.1/tests/test_helpers.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,44 +44,61 @@
     except ImportError as err:
         assert str(err) == "Module instantiate_module is not a nn.Module"
 
 
 def test_cfg_repr_print(capsys: CaptureFixture[str]):
     """test repr and print results"""
     cfg = Cfg()
-    repr_res = cfg.__repr__()
+    repr_res = repr(cfg)
     assert repr_res == "Cfg(\n  )"
     cfg.print_set_fields()
     out = capsys.readouterr().out
     assert out == "Nothing changed\n"
     cfg.name = "cfg_name"
-    repr_res = cfg.__repr__()
+    repr_res = repr(cfg)
     assert repr_res == "Cfg(\n  name='cfg_name')"
     cfg.print_cfg()
     out = capsys.readouterr().out
     assert out == "Cfg(\n  name='cfg_name')\n"
+
+    # print
+    print(cfg)
+    out = capsys.readouterr().out
+    assert out == "Cfg(\n  name='cfg_name')\n"
+
     # Set fields. default - name is not in changed
     cfg = Cfg2(name="cfg_name")
     cfg.print_set_fields()
     out = capsys.readouterr().out
     assert out == "Nothing changed\n"
-    assert "name" in cfg.model_fields_set
+    assert "name" in cfg.model_fields_set  # pylint: disable=E1135:unsupported-membership-test
     cfg = Cfg2(int_value=0)
     cfg.print_set_fields()
     out = capsys.readouterr().out
     assert out == "Set fields:\nint_value: 0\n"
+
     # Changed fields
     cfg = Cfg2(name="cfg_name")
     assert cfg.changed_fields == {"name": "cfg_name"}
     cfg.int_value = 1
     cfg.name = None
     assert cfg.changed_fields == {"int_value": 1}
+
     # print
     cfg.print_changed_fields()
     out = capsys.readouterr().out
     assert out == "Changed fields:\nint_value: 1\n"
+
+    cfg.print_changed_fields(show_default=True)
+    out = capsys.readouterr().out
+    assert out == "Changed fields:\nint_value: 1 | 10\n"
+
+    cfg.print_changed_fields(show_default=True, separator=" / ")
+    out = capsys.readouterr().out
+    assert out == "Changed fields:\nint_value: 1 / 10\n"
+
     # return to default
     cfg.int_value = 10
     assert not cfg.changed_fields
     cfg.print_changed_fields()
     out = capsys.readouterr().out
     assert out == "Nothing changed\n"
```

### Comparing `model_constructor-0.4/tests/test_layers.py` & `model_constructor-0.4.1/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/tests/test_layers_depr.py` & `model_constructor-0.4.1/tests/test_layers_depr.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/tests/test_mc.py` & `model_constructor-0.4.1/tests/test_mc.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/tests/test_models.py` & `model_constructor-0.4.1/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/tests/test_models_old.py` & `model_constructor-0.4.1/tests/test_models_old.py`

 * *Files identical despite different names*

### Comparing `model_constructor-0.4/tests/test_models_universal_blocks.py` & `model_constructor-0.4.1/tests/test_models_universal_blocks.py`

 * *Files identical despite different names*

