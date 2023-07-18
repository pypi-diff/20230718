# Comparing `tmp/nnoir_onnx-1.1.0.tar.gz` & `tmp/nnoir_onnx-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nnoir_onnx-1.1.0.tar", max compression
+gzip compressed data, was "nnoir_onnx-1.2.0.tar", max compression
```

## Comparing `nnoir_onnx-1.1.0.tar` & `nnoir_onnx-1.2.0.tar`

### file list

```diff
@@ -1,50 +1,51 @@
--rw-r--r--   0        0        0     5340 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/README.md
--rw-r--r--   0        0        0      113 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/__init__.py
--rw-r--r--   0        0        0      148 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/_version.py
--rw-r--r--   0        0        0     1692 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/freeze.py
--rw-r--r--   0        0        0    18122 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/onnx.py
--rw-r--r--   0        0        0     1030 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/onnx2nnoir.py
--rw-r--r--   0        0        0     1149 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/__init__.py
--rw-r--r--   0        0        0      949 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/add.py
--rw-r--r--   0        0        0     2000 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/average_pool.py
--rw-r--r--   0        0        0     1123 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/batch_normalization.py
--rw-r--r--   0        0        0     1488 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/clip.py
--rw-r--r--   0        0        0      554 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/concat.py
--rw-r--r--   0        0        0     3146 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/conv.py
--rw-r--r--   0        0        0      269 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/cos.py
--rw-r--r--   0        0        0     1416 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/div.py
--rw-r--r--   0        0        0      426 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/dropout.py
--rw-r--r--   0        0        0      427 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/elu.py
--rw-r--r--   0        0        0      269 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/exp.py
--rw-r--r--   0        0        0      780 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/flatten.py
--rw-r--r--   0        0        0     1992 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/gemm.py
--rw-r--r--   0        0        0     1615 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/global_average_pool.py
--rw-r--r--   0        0        0      715 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/hard_swish.py
--rw-r--r--   0        0        0      441 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/leaky_relu.py
--rw-r--r--   0        0        0      922 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/lrn.py
--rw-r--r--   0        0        0    11515 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/lstm.py
--rw-r--r--   0        0        0      959 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/mat_mul.py
--rw-r--r--   0        0        0     2335 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/max_pool.py
--rw-r--r--   0        0        0      917 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/mul.py
--rw-r--r--   0        0        0     2338 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/pad.py
--rw-r--r--   0        0        0      633 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/prelu.py
--rw-r--r--   0        0        0     1095 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/reduce_mean.py
--rw-r--r--   0        0        0      927 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/reduce_sum.py
--rw-r--r--   0        0        0      272 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/relu.py
--rw-r--r--   0        0        0      363 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/reshape.py
--rw-r--r--   0        0        0     3343 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/resize.py
--rw-r--r--   0        0        0      281 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/sigmoid.py
--rw-r--r--   0        0        0      269 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/sin.py
--rw-r--r--   0        0        0      432 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/softmax.py
--rw-r--r--   0        0        0     3615 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/split.py
--rw-r--r--   0        0        0      960 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/squeeze.py
--rw-r--r--   0        0        0      730 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/sub.py
--rw-r--r--   0        0        0      404 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/sum.py
--rw-r--r--   0        0        0      269 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/tan.py
--rw-r--r--   0        0        0      272 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/tanh.py
--rw-r--r--   0        0        0      464 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/transpose.py
--rw-r--r--   0        0        0      498 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/unsqueeze.py
--rw-r--r--   0        0        0     1560 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/operators/utils.py
--rw-r--r--   0        0        0     1134 2023-03-06 03:13:50.200388 nnoir_onnx-1.1.0/nnoir_onnx/utils.py
--rw-r--r--   0        0        0     1350 2023-03-06 03:13:50.204388 nnoir_onnx-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     6459 1970-01-01 00:00:00.000000 nnoir_onnx-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     5426 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/README.md
+-rw-r--r--   0        0        0      113 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/__init__.py
+-rw-r--r--   0        0        0      148 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/_version.py
+-rw-r--r--   0        0        0     1692 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/freeze.py
+-rw-r--r--   0        0        0    18122 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/onnx.py
+-rw-r--r--   0        0        0     1030 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/onnx2nnoir.py
+-rw-r--r--   0        0        0     1189 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/__init__.py
+-rw-r--r--   0        0        0      949 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/add.py
+-rw-r--r--   0        0        0     2000 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/average_pool.py
+-rw-r--r--   0        0        0     1123 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/batch_normalization.py
+-rw-r--r--   0        0        0     1488 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/clip.py
+-rw-r--r--   0        0        0      554 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/concat.py
+-rw-r--r--   0        0        0     3146 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/conv.py
+-rw-r--r--   0        0        0      269 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/cos.py
+-rw-r--r--   0        0        0     1416 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/div.py
+-rw-r--r--   0        0        0      426 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/dropout.py
+-rw-r--r--   0        0        0      427 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/elu.py
+-rw-r--r--   0        0        0      269 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/exp.py
+-rw-r--r--   0        0        0      780 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/flatten.py
+-rw-r--r--   0        0        0     1992 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/gemm.py
+-rw-r--r--   0        0        0     1615 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/global_average_pool.py
+-rw-r--r--   0        0        0     1139 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/hard_sigmoid.py
+-rw-r--r--   0        0        0      715 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/hard_swish.py
+-rw-r--r--   0        0        0      441 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/leaky_relu.py
+-rw-r--r--   0        0        0      922 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/lrn.py
+-rw-r--r--   0        0        0    11515 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/lstm.py
+-rw-r--r--   0        0        0      959 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/mat_mul.py
+-rw-r--r--   0        0        0     2335 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/max_pool.py
+-rw-r--r--   0        0        0      917 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/mul.py
+-rw-r--r--   0        0        0     2338 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/pad.py
+-rw-r--r--   0        0        0      633 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/prelu.py
+-rw-r--r--   0        0        0     1095 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/reduce_mean.py
+-rw-r--r--   0        0        0      927 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/reduce_sum.py
+-rw-r--r--   0        0        0      272 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/relu.py
+-rw-r--r--   0        0        0      363 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/reshape.py
+-rw-r--r--   0        0        0     3343 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/resize.py
+-rw-r--r--   0        0        0      281 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/sigmoid.py
+-rw-r--r--   0        0        0      269 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/sin.py
+-rw-r--r--   0        0        0      432 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/softmax.py
+-rw-r--r--   0        0        0     3615 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/split.py
+-rw-r--r--   0        0        0      960 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/squeeze.py
+-rw-r--r--   0        0        0      730 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/sub.py
+-rw-r--r--   0        0        0      404 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/sum.py
+-rw-r--r--   0        0        0      269 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/tan.py
+-rw-r--r--   0        0        0      272 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/tanh.py
+-rw-r--r--   0        0        0      464 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/transpose.py
+-rw-r--r--   0        0        0      498 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/unsqueeze.py
+-rw-r--r--   0        0        0     1560 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/operators/utils.py
+-rw-r--r--   0        0        0     1134 2023-07-18 02:39:14.130149 nnoir_onnx-1.2.0/nnoir_onnx/utils.py
+-rw-r--r--   0        0        0     1350 2023-07-18 02:39:14.134149 nnoir_onnx-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     6545 1970-01-01 00:00:00.000000 nnoir_onnx-1.2.0/PKG-INFO
```

### Comparing `nnoir_onnx-1.1.0/README.md` & `nnoir_onnx-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -8,29 +8,29 @@
 ```
 pip install nnoir-onnx
 ```
 
 From [Dockerhub](https://hub.docker.com/repository/docker/idein/nnoir-tools):
 
 ```
-docker pull idein/nnoir-tools:20230306
+docker pull idein/nnoir-tools:20230718
 ```
 
 ## Example
 
 ~~~~bash
 wget https://www.cntk.ai/OnnxModels/mnist/opset_7/mnist.tar.gz
 tar xvzf mnist.tar.gz
 onnx2nnoir -o model.nnoir mnist/model.onnx
 ~~~~
 
 With docker:
 
 ```
-docker run --rm -it -u $UID:$GID -v $(pwd):/work idein/nnoir-tools:20230306 onnx2nnoir --graph_name "mobilenet" -o mobilenetv2-1.0.nnoir mobilenetv2-1.0.onnx
+docker run --rm -it -u $UID:$GID -v $(pwd):/work idein/nnoir-tools:20230718 onnx2nnoir --graph_name "mobilenet" -o mobilenetv2-1.0.nnoir mobilenetv2-1.0.onnx
 ```
 
 ## Supported ONNX Operators
 
 * [Add](https://github.com/onnx/onnx/blob/master/docs/Operators.md#Add)
 * [AveragePool](https://github.com/onnx/onnx/blob/master/docs/Operators.md#AveragePool)
 * [BatchNormalization](https://github.com/onnx/onnx/blob/master/docs/Operators.md#BatchNormalization)
@@ -52,14 +52,15 @@
 * [Elu](https://github.com/onnx/onnx/blob/master/docs/Operators.md#Elu)
 * [Exp](https://github.com/onnx/onnx/blob/master/docs/Operators.md#Exp)
 * [Flatten](https://github.com/onnx/onnx/blob/master/docs/Operators.md#Flatten)
 * [Gemm](https://github.com/onnx/onnx/blob/master/docs/Operators.md#Gemm)
     * `B` must be [Constant](https://github.com/onnx/onnx/blob/master/docs/Operators.md#Constant) value or have initializer value
     * `C` must be [Constant](https://github.com/onnx/onnx/blob/master/docs/Operators.md#Constant) value or have initializer value
 * [GlobalAveragePool](https://github.com/onnx/onnx/blob/master/docs/Operators.md#GlobalAveragePool)
+* [HardSigmoid](https://github.com/onnx/onnx/blob/main/docs/Operators.md#hardsigmoid)
 * [HardSwish](https://github.com/onnx/onnx/blob/main/docs/Operators.md#hardswish)
 * [LeakyRelu](https://github.com/onnx/onnx/blob/master/docs/Operators.md#LeakyRelu)
 * [LRN](https://github.com/onnx/onnx/blob/master/docs/Operators.md#LRN)
 * [LSTM](https://github.com/onnx/onnx/blob/master/docs/Operators.md#lstm)
     * only `seq_length == 1`
     * `direction` must be forward
     * Supported `activations` are below
```

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/freeze.py` & `nnoir_onnx-1.2.0/nnoir_onnx/freeze.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/onnx.py` & `nnoir_onnx-1.2.0/nnoir_onnx/onnx.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/onnx2nnoir.py` & `nnoir_onnx-1.2.0/nnoir_onnx/onnx2nnoir.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/__init__.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from .div import OpDiv
 from .dropout import OpDropout
 from .elu import OpElu
 from .exp import OpExp
 from .flatten import OpFlatten
 from .gemm import OpGemm
 from .global_average_pool import OpGlobalAveragePool
+from .hard_sigmoid import OpHardSigmoid
 from .hard_swish import OpHardSwish
 from .leaky_relu import OpLeakyRelu
 from .lrn import OpLRN
 from .lstm import OpLSTM
 from .mat_mul import OpMatMul
 from .max_pool import OpMaxPool
 from .mul import OpMul
```

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/add.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/add.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/average_pool.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/average_pool.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/batch_normalization.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/clip.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/clip.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/concat.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/concat.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/conv.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/conv.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/div.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/div.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/flatten.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/flatten.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/gemm.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/gemm.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/global_average_pool.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/global_average_pool.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/hard_swish.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/hard_swish.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/lrn.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/lrn.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/lstm.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/lstm.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/mat_mul.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/mat_mul.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/max_pool.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/max_pool.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/mul.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/mul.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/pad.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/pad.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/prelu.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/prelu.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/reduce_mean.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/reduce_mean.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/reduce_sum.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/reduce_sum.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/resize.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/resize.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/split.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/split.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/squeeze.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/squeeze.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/sub.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/sub.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/operators/utils.py` & `nnoir_onnx-1.2.0/nnoir_onnx/operators/utils.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/nnoir_onnx/utils.py` & `nnoir_onnx-1.2.0/nnoir_onnx/utils.py`

 * *Files identical despite different names*

### Comparing `nnoir_onnx-1.1.0/pyproject.toml` & `nnoir_onnx-1.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nnoir-onnx"
-version = "1.1.0"
+version = "1.2.0"
 description = "ONNX to NNOIR Converter"
 authors = ["Idein Inc."]
 license = "MIT"
 readme = "README.md"
 keywords = ["nnoir", "onnx", "machine learning"]
 repository = "https://github.com/Idein/nnoir/tree/master/nnoir-onnx"
 classifiers=[
```

### Comparing `nnoir_onnx-1.1.0/PKG-INFO` & `nnoir_onnx-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nnoir-onnx
-Version: 1.1.0
+Version: 1.2.0
 Summary: ONNX to NNOIR Converter
 Home-page: https://github.com/Idein/nnoir/tree/master/nnoir-onnx
 License: MIT
 Keywords: nnoir,onnx,machine learning
 Author: Idein Inc.
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -37,29 +37,29 @@
 ```
 pip install nnoir-onnx
 ```
 
 From [Dockerhub](https://hub.docker.com/repository/docker/idein/nnoir-tools):
 
 ```
-docker pull idein/nnoir-tools:20230306
+docker pull idein/nnoir-tools:20230718
 ```
 
 ## Example
 
 ~~~~bash
 wget https://www.cntk.ai/OnnxModels/mnist/opset_7/mnist.tar.gz
 tar xvzf mnist.tar.gz
 onnx2nnoir -o model.nnoir mnist/model.onnx
 ~~~~
 
 With docker:
 
 ```
-docker run --rm -it -u $UID:$GID -v $(pwd):/work idein/nnoir-tools:20230306 onnx2nnoir --graph_name "mobilenet" -o mobilenetv2-1.0.nnoir mobilenetv2-1.0.onnx
+docker run --rm -it -u $UID:$GID -v $(pwd):/work idein/nnoir-tools:20230718 onnx2nnoir --graph_name "mobilenet" -o mobilenetv2-1.0.nnoir mobilenetv2-1.0.onnx
 ```
 
 ## Supported ONNX Operators
 
 * [Add](https://github.com/onnx/onnx/blob/master/docs/Operators.md#Add)
 * [AveragePool](https://github.com/onnx/onnx/blob/master/docs/Operators.md#AveragePool)
 * [BatchNormalization](https://github.com/onnx/onnx/blob/master/docs/Operators.md#BatchNormalization)
@@ -81,14 +81,15 @@
 * [Elu](https://github.com/onnx/onnx/blob/master/docs/Operators.md#Elu)
 * [Exp](https://github.com/onnx/onnx/blob/master/docs/Operators.md#Exp)
 * [Flatten](https://github.com/onnx/onnx/blob/master/docs/Operators.md#Flatten)
 * [Gemm](https://github.com/onnx/onnx/blob/master/docs/Operators.md#Gemm)
     * `B` must be [Constant](https://github.com/onnx/onnx/blob/master/docs/Operators.md#Constant) value or have initializer value
     * `C` must be [Constant](https://github.com/onnx/onnx/blob/master/docs/Operators.md#Constant) value or have initializer value
 * [GlobalAveragePool](https://github.com/onnx/onnx/blob/master/docs/Operators.md#GlobalAveragePool)
+* [HardSigmoid](https://github.com/onnx/onnx/blob/main/docs/Operators.md#hardsigmoid)
 * [HardSwish](https://github.com/onnx/onnx/blob/main/docs/Operators.md#hardswish)
 * [LeakyRelu](https://github.com/onnx/onnx/blob/master/docs/Operators.md#LeakyRelu)
 * [LRN](https://github.com/onnx/onnx/blob/master/docs/Operators.md#LRN)
 * [LSTM](https://github.com/onnx/onnx/blob/master/docs/Operators.md#lstm)
     * only `seq_length == 1`
     * `direction` must be forward
     * Supported `activations` are below
```

