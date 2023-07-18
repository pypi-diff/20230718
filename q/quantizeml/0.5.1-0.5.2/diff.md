# Comparing `tmp/quantizeml-0.5.1.tar.gz` & `tmp/quantizeml-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quantizeml-0.5.1.tar", last modified: Thu Jul  6 08:58:52 2023, max compression
+gzip compressed data, was "quantizeml-0.5.2.tar", last modified: Tue Jul 18 08:55:09 2023, max compression
```

## Comparing `quantizeml-0.5.1.tar` & `quantizeml-0.5.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:58:52.543598 quantizeml-0.5.1/
--rw-r--r--   0 root         (0) root         (0)    11358 2023-07-06 08:58:50.000000 quantizeml-0.5.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       16 2023-07-06 08:58:50.000000 quantizeml-0.5.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      477 2023-07-06 08:58:52.543598 quantizeml-0.5.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      168 2023-07-06 08:58:50.000000 quantizeml-0.5.1/README
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:58:52.539598 quantizeml-0.5.1/quantizeml/
--rw-r--r--   0 root         (0) root         (0)      122 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10463 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:58:52.539598 quantizeml-0.5.1/quantizeml/debugging/
--rw-r--r--   0 root         (0) root         (0)       26 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/debugging/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3824 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/debugging/assertions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:58:52.539598 quantizeml-0.5.1/quantizeml/layers/
--rw-r--r--   0 root         (0) root         (0)      524 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4193 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/activations.py
--rw-r--r--   0 root         (0) root         (0)     8671 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/attention.py
--rw-r--r--   0 root         (0) root         (0)     7897 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/batch_normalization.py
--rw-r--r--   0 root         (0) root         (0)    11090 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/convolution.py
--rw-r--r--   0 root         (0) root         (0)     2024 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/dense.py
--rw-r--r--   0 root         (0) root         (0)    10092 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/depthwise_convolution.py
--rw-r--r--   0 root         (0) root         (0)     1394 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/dropout.py
--rw-r--r--   0 root         (0) root         (0)    10692 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/layers_base.py
--rw-r--r--   0 root         (0) root         (0)     4798 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/multi_inbounds.py
--rw-r--r--   0 root         (0) root         (0)     8790 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/normalization.py
--rw-r--r--   0 root         (0) root         (0)     4182 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/output_observer.py
--rw-r--r--   0 root         (0) root         (0)     3815 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/pooling.py
--rw-r--r--   0 root         (0) root         (0)     3238 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/quantization_params.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:58:52.543598 quantizeml-0.5.1/quantizeml/layers/quantizers/
--rw-r--r--   0 root         (0) root         (0)      130 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/quantizers/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4012 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/quantizers/aligned_weight_quantizer.py
--rw-r--r--   0 root         (0) root         (0)     6326 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/quantizers/output_quantizer.py
--rw-r--r--   0 root         (0) root         (0)     4593 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/quantizers/quantizers.py
--rw-r--r--   0 root         (0) root         (0)     4412 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/quantizers/weight_quantizer.py
--rw-r--r--   0 root         (0) root         (0)     5576 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/recorders.py
--rw-r--r--   0 root         (0) root         (0)     2019 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/rescaling.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:58:52.543598 quantizeml-0.5.1/quantizeml/layers/reshaping/
--rw-r--r--   0 root         (0) root         (0)       69 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/reshaping/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2067 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/reshaping/flatten.py
--rw-r--r--   0 root         (0) root         (0)     2197 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/reshaping/permute.py
--rw-r--r--   0 root         (0) root         (0)     1992 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/reshaping/reshape.py
--rw-r--r--   0 root         (0) root         (0)     3478 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/separable_convolution.py
--rw-r--r--   0 root         (0) root         (0)     8801 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/shiftmax.py
--rw-r--r--   0 root         (0) root         (0)     7155 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/layers/vit.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:58:52.543598 quantizeml-0.5.1/quantizeml/models/
--rw-r--r--   0 root         (0) root         (0)      174 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11761 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/calibrate.py
--rw-r--r--   0 root         (0) root         (0)     4001 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/check_quantization.py
--rw-r--r--   0 root         (0) root         (0)    16664 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/quantize.py
--rw-r--r--   0 root         (0) root         (0)     1553 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/record.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:58:52.543598 quantizeml-0.5.1/quantizeml/models/transforms/
--rw-r--r--   0 root         (0) root         (0)      248 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/transforms/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7694 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/transforms/align_rescaling.py
--rw-r--r--   0 root         (0) root         (0)     9727 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/transforms/fold_batchnorms.py
--rw-r--r--   0 root         (0) root         (0)     7714 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/transforms/insert_layer.py
--rw-r--r--   0 root         (0) root         (0)     2938 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/transforms/invert_batchnorm_pooling.py
--rw-r--r--   0 root         (0) root         (0)     1668 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/transforms/relu_maxpool.py
--rw-r--r--   0 root         (0) root         (0)     6523 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/transforms/remove_zeropadding2d.py
--rw-r--r--   0 root         (0) root         (0)     6031 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/transforms/replace_lambda.py
--rw-r--r--   0 root         (0) root         (0)     1892 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/transforms/sanitize.py
--rw-r--r--   0 root         (0) root         (0)     7768 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/transforms/transforms_utils.py
--rw-r--r--   0 root         (0) root         (0)     3202 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/models/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:58:52.543598 quantizeml-0.5.1/quantizeml/tensors/
--rw-r--r--   0 root         (0) root         (0)       99 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/tensors/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22032 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/tensors/fixed_point.py
--rw-r--r--   0 root         (0) root         (0)     8281 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/tensors/qfloat.py
--rw-r--r--   0 root         (0) root         (0)     6012 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/tensors/qtensor.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:58:52.543598 quantizeml-0.5.1/quantizeml/tensors/tf_dispatch/
--rw-r--r--   0 root         (0) root         (0)       63 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/tensors/tf_dispatch/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10521 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/tensors/tf_dispatch/math.py
--rw-r--r--   0 root         (0) root         (0)    24855 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/tensors/tf_dispatch/nn.py
--rw-r--r--   0 root         (0) root         (0)    14430 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/tensors/tf_dispatch/reshaping.py
--rw-r--r--   0 root         (0) root         (0)      191 2023-07-06 08:58:50.000000 quantizeml-0.5.1/quantizeml/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-06 08:58:52.539598 quantizeml-0.5.1/quantizeml.egg-info/
--rw-r--r--   0 root         (0) root         (0)      477 2023-07-06 08:58:52.000000 quantizeml-0.5.1/quantizeml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2353 2023-07-06 08:58:52.000000 quantizeml-0.5.1/quantizeml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-06 08:58:52.000000 quantizeml-0.5.1/quantizeml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       51 2023-07-06 08:58:52.000000 quantizeml-0.5.1/quantizeml.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       33 2023-07-06 08:58:52.000000 quantizeml-0.5.1/quantizeml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-07-06 08:58:52.000000 quantizeml-0.5.1/quantizeml.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-06 08:58:52.543598 quantizeml-0.5.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1114 2023-07-06 08:58:50.000000 quantizeml-0.5.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 08:55:09.627832 quantizeml-0.5.2/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-07-18 08:55:03.000000 quantizeml-0.5.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       16 2023-07-18 08:55:03.000000 quantizeml-0.5.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      477 2023-07-18 08:55:09.627832 quantizeml-0.5.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      168 2023-07-18 08:55:03.000000 quantizeml-0.5.2/README
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 08:55:09.619832 quantizeml-0.5.2/quantizeml/
+-rw-r--r--   0 root         (0) root         (0)      122 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10463 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 08:55:09.619832 quantizeml-0.5.2/quantizeml/debugging/
+-rw-r--r--   0 root         (0) root         (0)       26 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/debugging/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3824 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/debugging/assertions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 08:55:09.623832 quantizeml-0.5.2/quantizeml/layers/
+-rw-r--r--   0 root         (0) root         (0)      524 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4193 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/activations.py
+-rw-r--r--   0 root         (0) root         (0)     8671 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/attention.py
+-rw-r--r--   0 root         (0) root         (0)     7897 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/batch_normalization.py
+-rw-r--r--   0 root         (0) root         (0)    11090 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/convolution.py
+-rw-r--r--   0 root         (0) root         (0)     2024 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/dense.py
+-rw-r--r--   0 root         (0) root         (0)    10092 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/depthwise_convolution.py
+-rw-r--r--   0 root         (0) root         (0)     1394 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/dropout.py
+-rw-r--r--   0 root         (0) root         (0)    10692 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/layers_base.py
+-rw-r--r--   0 root         (0) root         (0)     4798 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/multi_inbounds.py
+-rw-r--r--   0 root         (0) root         (0)     8790 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/normalization.py
+-rw-r--r--   0 root         (0) root         (0)     4182 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/output_observer.py
+-rw-r--r--   0 root         (0) root         (0)     3815 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/pooling.py
+-rw-r--r--   0 root         (0) root         (0)     3238 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/quantization_params.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 08:55:09.623832 quantizeml-0.5.2/quantizeml/layers/quantizers/
+-rw-r--r--   0 root         (0) root         (0)      130 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/quantizers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4012 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/quantizers/aligned_weight_quantizer.py
+-rw-r--r--   0 root         (0) root         (0)     6326 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/quantizers/output_quantizer.py
+-rw-r--r--   0 root         (0) root         (0)     4593 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/quantizers/quantizers.py
+-rw-r--r--   0 root         (0) root         (0)     4410 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/quantizers/weight_quantizer.py
+-rw-r--r--   0 root         (0) root         (0)     5576 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/recorders.py
+-rw-r--r--   0 root         (0) root         (0)     2019 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/rescaling.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 08:55:09.623832 quantizeml-0.5.2/quantizeml/layers/reshaping/
+-rw-r--r--   0 root         (0) root         (0)       69 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/reshaping/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/reshaping/flatten.py
+-rw-r--r--   0 root         (0) root         (0)     2197 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/reshaping/permute.py
+-rw-r--r--   0 root         (0) root         (0)     1992 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/reshaping/reshape.py
+-rw-r--r--   0 root         (0) root         (0)     3478 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/separable_convolution.py
+-rw-r--r--   0 root         (0) root         (0)     8801 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/shiftmax.py
+-rw-r--r--   0 root         (0) root         (0)     7155 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/layers/vit.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 08:55:09.623832 quantizeml-0.5.2/quantizeml/models/
+-rw-r--r--   0 root         (0) root         (0)      174 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11761 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/calibrate.py
+-rw-r--r--   0 root         (0) root         (0)     4001 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/check_quantization.py
+-rw-r--r--   0 root         (0) root         (0)    16664 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/quantize.py
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/record.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 08:55:09.627832 quantizeml-0.5.2/quantizeml/models/transforms/
+-rw-r--r--   0 root         (0) root         (0)      248 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/transforms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7694 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/transforms/align_rescaling.py
+-rw-r--r--   0 root         (0) root         (0)     9727 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/transforms/fold_batchnorms.py
+-rw-r--r--   0 root         (0) root         (0)     7714 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/transforms/insert_layer.py
+-rw-r--r--   0 root         (0) root         (0)     2938 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/transforms/invert_batchnorm_pooling.py
+-rw-r--r--   0 root         (0) root         (0)     1668 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/transforms/relu_maxpool.py
+-rw-r--r--   0 root         (0) root         (0)     6523 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/transforms/remove_zeropadding2d.py
+-rw-r--r--   0 root         (0) root         (0)     6031 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/transforms/replace_lambda.py
+-rw-r--r--   0 root         (0) root         (0)     1892 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/transforms/sanitize.py
+-rw-r--r--   0 root         (0) root         (0)     7768 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/transforms/transforms_utils.py
+-rw-r--r--   0 root         (0) root         (0)     3202 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/models/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 08:55:09.627832 quantizeml-0.5.2/quantizeml/tensors/
+-rw-r--r--   0 root         (0) root         (0)       99 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/tensors/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22032 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/tensors/fixed_point.py
+-rw-r--r--   0 root         (0) root         (0)     8281 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/tensors/qfloat.py
+-rw-r--r--   0 root         (0) root         (0)     6012 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/tensors/qtensor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 08:55:09.627832 quantizeml-0.5.2/quantizeml/tensors/tf_dispatch/
+-rw-r--r--   0 root         (0) root         (0)       63 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/tensors/tf_dispatch/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10521 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/tensors/tf_dispatch/math.py
+-rw-r--r--   0 root         (0) root         (0)    24855 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/tensors/tf_dispatch/nn.py
+-rw-r--r--   0 root         (0) root         (0)    14430 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/tensors/tf_dispatch/reshaping.py
+-rw-r--r--   0 root         (0) root         (0)      191 2023-07-18 08:55:03.000000 quantizeml-0.5.2/quantizeml/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 08:55:09.619832 quantizeml-0.5.2/quantizeml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      477 2023-07-18 08:55:09.000000 quantizeml-0.5.2/quantizeml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2353 2023-07-18 08:55:09.000000 quantizeml-0.5.2/quantizeml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 08:55:09.000000 quantizeml-0.5.2/quantizeml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       51 2023-07-18 08:55:09.000000 quantizeml-0.5.2/quantizeml.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       33 2023-07-18 08:55:09.000000 quantizeml-0.5.2/quantizeml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-07-18 08:55:09.000000 quantizeml-0.5.2/quantizeml.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 08:55:09.627832 quantizeml-0.5.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1114 2023-07-18 08:55:03.000000 quantizeml-0.5.2/setup.py
```

### Comparing `quantizeml-0.5.1/LICENSE` & `quantizeml-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/cli.py` & `quantizeml-0.5.2/quantizeml/cli.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/debugging/assertions.py` & `quantizeml-0.5.2/quantizeml/debugging/assertions.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/__init__.py` & `quantizeml-0.5.2/quantizeml/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/activations.py` & `quantizeml-0.5.2/quantizeml/layers/activations.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/attention.py` & `quantizeml-0.5.2/quantizeml/layers/attention.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/batch_normalization.py` & `quantizeml-0.5.2/quantizeml/layers/batch_normalization.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/convolution.py` & `quantizeml-0.5.2/quantizeml/layers/convolution.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/dense.py` & `quantizeml-0.5.2/quantizeml/layers/dense.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/depthwise_convolution.py` & `quantizeml-0.5.2/quantizeml/layers/depthwise_convolution.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/dropout.py` & `quantizeml-0.5.2/quantizeml/layers/dropout.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/layers_base.py` & `quantizeml-0.5.2/quantizeml/layers/layers_base.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/multi_inbounds.py` & `quantizeml-0.5.2/quantizeml/layers/multi_inbounds.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/normalization.py` & `quantizeml-0.5.2/quantizeml/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/output_observer.py` & `quantizeml-0.5.2/quantizeml/layers/output_observer.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/pooling.py` & `quantizeml-0.5.2/quantizeml/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/quantization_params.py` & `quantizeml-0.5.2/quantizeml/layers/quantization_params.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/quantizers/aligned_weight_quantizer.py` & `quantizeml-0.5.2/quantizeml/layers/quantizers/aligned_weight_quantizer.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/quantizers/output_quantizer.py` & `quantizeml-0.5.2/quantizeml/layers/quantizers/output_quantizer.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/quantizers/quantizers.py` & `quantizeml-0.5.2/quantizeml/layers/quantizers/quantizers.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/quantizers/weight_quantizer.py` & `quantizeml-0.5.2/quantizeml/layers/quantizers/weight_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         if isinstance(inputs, QTensor):
             raise ValueError(
                 f"{type(inputs)} input is not supported. WeightQuantizer only accepts float"
                 " inputs.")
 
         # Compute the quantization ranges from the inputs
         ranges = tf.math.reduce_max(tf.math.abs(inputs), self._axis)
-        if self._axis is not None and inputs.shape[-1] == 1 and len(inputs.shape) > 2:
+        if self.axis in [-2, 2] and inputs.shape[-1] == 1 and len(inputs.shape) > 2:
             # Expand the shape of the ranges so that it is broacastable on the inputs
             ranges = tf.expand_dims(ranges, -1)
         # Evaluate the scales to align on the optimal quantization ranges
         scales = QFloat.optimal_scales(ranges, self.value_bits)
         # Clip scales lower bound to avoid quantizing very tiny values. Minimum is defined
         # as 1e-6, enough value to be considered as zero.
         scales = tf.maximum(scales, 1e-6)
```

### Comparing `quantizeml-0.5.1/quantizeml/layers/recorders.py` & `quantizeml-0.5.2/quantizeml/layers/recorders.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/rescaling.py` & `quantizeml-0.5.2/quantizeml/layers/rescaling.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/reshaping/flatten.py` & `quantizeml-0.5.2/quantizeml/layers/reshaping/flatten.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/reshaping/permute.py` & `quantizeml-0.5.2/quantizeml/layers/reshaping/permute.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/reshaping/reshape.py` & `quantizeml-0.5.2/quantizeml/layers/reshaping/reshape.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/separable_convolution.py` & `quantizeml-0.5.2/quantizeml/layers/separable_convolution.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/shiftmax.py` & `quantizeml-0.5.2/quantizeml/layers/shiftmax.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/layers/vit.py` & `quantizeml-0.5.2/quantizeml/layers/vit.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/models/calibrate.py` & `quantizeml-0.5.2/quantizeml/models/calibrate.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/models/check_quantization.py` & `quantizeml-0.5.2/quantizeml/models/check_quantization.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/models/quantize.py` & `quantizeml-0.5.2/quantizeml/models/quantize.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/models/record.py` & `quantizeml-0.5.2/quantizeml/models/record.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/models/transforms/align_rescaling.py` & `quantizeml-0.5.2/quantizeml/models/transforms/align_rescaling.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/models/transforms/fold_batchnorms.py` & `quantizeml-0.5.2/quantizeml/models/transforms/fold_batchnorms.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/models/transforms/insert_layer.py` & `quantizeml-0.5.2/quantizeml/models/transforms/insert_layer.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/models/transforms/invert_batchnorm_pooling.py` & `quantizeml-0.5.2/quantizeml/models/transforms/invert_batchnorm_pooling.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/models/transforms/relu_maxpool.py` & `quantizeml-0.5.2/quantizeml/models/transforms/relu_maxpool.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/models/transforms/remove_zeropadding2d.py` & `quantizeml-0.5.2/quantizeml/models/transforms/remove_zeropadding2d.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/models/transforms/replace_lambda.py` & `quantizeml-0.5.2/quantizeml/models/transforms/replace_lambda.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/models/transforms/sanitize.py` & `quantizeml-0.5.2/quantizeml/models/transforms/sanitize.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/models/transforms/transforms_utils.py` & `quantizeml-0.5.2/quantizeml/models/transforms/transforms_utils.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/models/utils.py` & `quantizeml-0.5.2/quantizeml/models/utils.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/tensors/fixed_point.py` & `quantizeml-0.5.2/quantizeml/tensors/fixed_point.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/tensors/qfloat.py` & `quantizeml-0.5.2/quantizeml/tensors/qfloat.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/tensors/qtensor.py` & `quantizeml-0.5.2/quantizeml/tensors/qtensor.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/tensors/tf_dispatch/math.py` & `quantizeml-0.5.2/quantizeml/tensors/tf_dispatch/math.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/tensors/tf_dispatch/nn.py` & `quantizeml-0.5.2/quantizeml/tensors/tf_dispatch/nn.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml/tensors/tf_dispatch/reshaping.py` & `quantizeml-0.5.2/quantizeml/tensors/tf_dispatch/reshaping.py`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/quantizeml.egg-info/SOURCES.txt` & `quantizeml-0.5.2/quantizeml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `quantizeml-0.5.1/setup.py` & `quantizeml-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 # Read the contents of the README file
 directory = path.abspath(path.dirname(__file__))
 with open(path.join(directory, 'README'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='quantizeml',
-      version='0.5.1',
+      version='0.5.2',
       description='Base layers and quantization tools',
       long_description=long_description,
       long_description_content_type='text/markdown',
       author='David Corvoysier',
       author_email='dcorvoysier@brainchip.com',
       url='https://doc.brainchipinc.com',
       license='Apache 2.0',
```

