# Comparing `tmp/mct-quantizers-1.1.0.tar.gz` & `tmp/mct-quantizers-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mct-quantizers-1.1.0.tar", last modified: Wed Jun 14 12:12:13 2023, max compression
+gzip compressed data, was "mct-quantizers-1.2.0.tar", last modified: Tue Jul 18 14:17:52 2023, max compression
```

## Comparing `mct-quantizers-1.1.0.tar` & `mct-quantizers-1.2.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.699248 mct-quantizers-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-14 12:12:13.699248 mct-quantizers-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3525 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.687248 mct-quantizers-1.1.0/mct_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.691248 mct-quantizers-1.1.0/mct_quantizers/common/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3120 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/common/base_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2529 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/common/get_all_subclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/common/get_quantizers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/common/quant_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/common/quant_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.691248 mct-quantizers-1.1.0/mct_quantizers/keras/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6418 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    11711 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.695248 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.695248 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8082 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4012 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.695248 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3935 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     9612 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3318 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8559 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/keras/validation_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.695248 mct-quantizers-1.1.0/mct_quantizers/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/activation_quantization_holder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/load_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantize_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizer_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.699248 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.699248 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4197 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2761 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4678 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4693 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.699248 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
--rw-r--r--   0 runner    (1001) docker     (123)      697 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3683 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4824 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2980 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4765 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 12:12:13.687248 mct-quantizers-1.1.0/mct_quantizers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4559 2023-06-14 12:12:13.000000 mct-quantizers-1.1.0/mct_quantizers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-06-14 12:12:13.000000 mct-quantizers-1.1.0/mct_quantizers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 12:12:13.000000 mct-quantizers-1.1.0/mct_quantizers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-14 12:12:13.000000 mct-quantizers-1.1.0/mct_quantizers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-14 12:12:13.000000 mct-quantizers-1.1.0/mct_quantizers.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-06-14 12:12:13.699248 mct-quantizers-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-06-14 12:11:54.000000 mct-quantizers-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:52.477172 mct-quantizers-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-07-18 14:17:52.477172 mct-quantizers-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:52.469172 mct-quantizers-1.2.0/mct_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:52.473172 mct-quantizers-1.2.0/mct_quantizers/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3161 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/common/base_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2438 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1213 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/common/get_all_subclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2939 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/common/get_quantizers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/common/quant_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/common/quant_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:52.473172 mct-quantizers-1.2.0/mct_quantizers/keras/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3790 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11677 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:52.473172 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:52.473172 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8074 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2947 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4004 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2173 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:52.473172 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9604 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4269 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8558 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/keras/validation_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:52.473172 mct-quantizers-1.2.0/mct_quantizers/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3111 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/activation_quantization_holder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/load_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7924 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantize_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5929 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizer_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:52.473172 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:52.473172 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4223 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2787 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4704 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:52.477172 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      697 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3709 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4850 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4799 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:17:52.473172 mct-quantizers-1.2.0/mct_quantizers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4423 2023-07-18 14:17:52.000000 mct-quantizers-1.2.0/mct_quantizers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-18 14:17:52.000000 mct-quantizers-1.2.0/mct_quantizers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:17:52.000000 mct-quantizers-1.2.0/mct_quantizers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 14:17:52.000000 mct-quantizers-1.2.0/mct_quantizers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-18 14:17:52.000000 mct-quantizers-1.2.0/mct_quantizers.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-07-18 14:17:52.477172 mct-quantizers-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-18 14:17:33.000000 mct-quantizers-1.2.0/setup.py
```

### Comparing `mct-quantizers-1.1.0/LICENSE.md` & `mct-quantizers-1.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/PKG-INFO` & `mct-quantizers-1.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers
-Version: 1.1.0
+Version: 1.2.0
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel. 
         
@@ -33,15 +33,15 @@
         2. [Pytorch Quantizers](mct_quantizers/pytorch/quantizers)
         
         ### The mark_quantizer Decorator
         
         The [`@mark_quantizer`](mct_quantizers/common/base_inferable_quantizer.py) decorator is used to assign each quantizer with static properties that define its task compatibility. Each quantizer class should be decorated with this decorator, which defines the following properties:
          - [`QuantizationTarget`](mct_quantizers/common/base_inferable_quantizer.py): An Enum that indicates whether the quantizer is intended for weights or activations quantization.
          - [`QuantizationMethod`](mct_quantizers/common/quant_info.py): A list of quantization methods (Uniform, Symmetric, etc.).
-         - `quantizer_type`: An optional property that defines the type of the quantization technique. This is a helper property that allows the creation of advanced quantizers for specific tasks.
+         - `identifier`: A unique identifier for the quantizer class. This is a helper property that allows the creation of advanced quantizers for specific tasks.
          
         ## Getting Started
         
         This section provides a quick guide to getting started. We begin with the installation process, either via source code or the pip server. Then, we provide a short example of usage.
         
         ### Installation
         Please refer to the MCT install guide for installing the pip package or building from the source.
@@ -58,17 +58,16 @@
         pip install mct-quantizers-nightly
         ```
         
         ### Requirements
         
         To use MCT Quantizers, you need to have one of the supported frameworks, Tensorflow or PyTorch, installed.
         
-        For use with Tensorflow, please install the following packages:
-        [tensorflow](https://www.tensorflow.org/install), 
-        [tensorflow-model-optimization](https://www.tensorflow.org/model_optimization/guide/install)
+        For use with Tensorflow, please install the following package:
+        [tensorflow](https://www.tensorflow.org/install),
         
         For use with PyTorch, please install the following package:
         [torch](https://pytorch.org/)
         
         You can also use the [requirements](requirements.txt) file to set up your environment.
         
         ## License
```

### Comparing `mct-quantizers-1.1.0/README.md` & `mct-quantizers-1.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 2. [Pytorch Quantizers](mct_quantizers/pytorch/quantizers)
 
 ### The mark_quantizer Decorator
 
 The [`@mark_quantizer`](mct_quantizers/common/base_inferable_quantizer.py) decorator is used to assign each quantizer with static properties that define its task compatibility. Each quantizer class should be decorated with this decorator, which defines the following properties:
  - [`QuantizationTarget`](mct_quantizers/common/base_inferable_quantizer.py): An Enum that indicates whether the quantizer is intended for weights or activations quantization.
  - [`QuantizationMethod`](mct_quantizers/common/quant_info.py): A list of quantization methods (Uniform, Symmetric, etc.).
- - `quantizer_type`: An optional property that defines the type of the quantization technique. This is a helper property that allows the creation of advanced quantizers for specific tasks.
+ - `identifier`: A unique identifier for the quantizer class. This is a helper property that allows the creation of advanced quantizers for specific tasks.
  
 ## Getting Started
 
 This section provides a quick guide to getting started. We begin with the installation process, either via source code or the pip server. Then, we provide a short example of usage.
 
 ### Installation
 Please refer to the MCT install guide for installing the pip package or building from the source.
@@ -52,17 +52,16 @@
 pip install mct-quantizers-nightly
 ```
 
 ### Requirements
 
 To use MCT Quantizers, you need to have one of the supported frameworks, Tensorflow or PyTorch, installed.
 
-For use with Tensorflow, please install the following packages:
-[tensorflow](https://www.tensorflow.org/install), 
-[tensorflow-model-optimization](https://www.tensorflow.org/model_optimization/guide/install)
+For use with Tensorflow, please install the following package:
+[tensorflow](https://www.tensorflow.org/install),
 
 For use with PyTorch, please install the following package:
 [torch](https://pytorch.org/)
 
 You can also use the [requirements](requirements.txt) file to set up your environment.
 
 ## License
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/__init__.py` & `mct-quantizers-1.2.0/mct_quantizers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,8 +22,8 @@
 from mct_quantizers.pytorch.load_model import pytorch_load_quantized_model
 from mct_quantizers.pytorch.quantize_wrapper import PytorchQuantizationWrapper
 
 from mct_quantizers.common import constants
 from mct_quantizers.keras import quantizers as keras_quantizers
 from mct_quantizers.pytorch import quantizers as pytorch_quantizers
 
-__version__ = "1.1.0"
+__version__ = "1.2.0"
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/common/__init__.py` & `mct-quantizers-1.2.0/mct_quantizers/common/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/common/base_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/common/base_inferable_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,28 +19,32 @@
 
 
 class QuantizationTarget(Enum):
     Activation = "Activation"
     Weights = "Weights"
 
 
+class QuantizerID(Enum):
+    INFERABLE = "inferable_quantizer_id"
+
+
 def mark_quantizer(quantization_target: QuantizationTarget = None,
                    quantization_method: List[QuantizationMethod] = None,
-                   quantizer_type: Any = None):
+                   identifier: Any = None):
     """
     A function to be used as decoration for all inferable quantizers (which inherit from BaseInferableQuantizer).
     By decorating a class with this decoration, we can define required static properties of the quantizer.
 
     Args:
         quantization_target: QuantizationTarget value which indicates what is the target for quantization to
             use the quantizer for.
         quantization_method: A list of QuantizationMethod values to indicate all type of quantization methods that the
             quantizer supports.
-        quantizer_type: The type of the quantizer (quantization technique).
-            This can differ, depending on the purpose the quantizer is for.
+        identifier: A unique identifier for the quantizer class (either the quantization
+            type/technique or other unique ID).
 
     Returns: A function that decorates a class object.
 
     """
     def mark(quantizer_class_object: BaseInferableQuantizer):
         """
         Initializes the parameters for the decorator.
@@ -49,15 +53,15 @@
             quantizer_class_object: The class to be decorated.
 
         Returns: A decorated class.
 
         """
         quantizer_class_object.quantization_target = quantization_target
         quantizer_class_object.quantization_method = quantization_method
-        quantizer_class_object.quantizer_type = quantizer_type
+        quantizer_class_object.identifier = identifier
 
         return quantizer_class_object
 
     return mark
 
 
 class BaseInferableQuantizer:
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/common/constants.py` & `mct-quantizers-1.2.0/mct_quantizers/common/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,18 +15,17 @@
 
 import importlib.util
 
 
 ## Frameworks
 
 TENSORFLOW = 'tensorflow'
-PYTORCH = 'pytorch'
-FOUND_TF = importlib.util.find_spec(TENSORFLOW) is not None and importlib.util.find_spec(
-    "tensorflow_model_optimization") is not None
-FOUND_TORCH = importlib.util.find_spec("torch") is not None
+TORCH = 'torch'
+FOUND_TF = importlib.util.find_spec(TENSORFLOW) is not None
+FOUND_TORCH = importlib.util.find_spec(TORCH) is not None
 
 
 ## Quantization properties
 
 IS_WEIGHTS = "is_weights"
 IS_ACTIVATIONS = "is_activations"
 WEIGHTS_QUANTIZERS = "weights_quantizer"
@@ -43,15 +42,15 @@
 ENABLE_ACTIVATION_QUANTIZATION = 'enable_activation_quantization'
 
 
 ## Quantizers
 
 QUANTIZATION_TARGET = 'quantization_target'
 QUANTIZATION_METHOD = 'quantization_method'
-QUANTIZER_TYPE = 'quantizer_type'
+QUANTIZER_ID = 'identifier'
 
 # In KerasQuantizationWrapper and PytorchQuantizationWrapper multiple quantizers are kept
 ACTIVATION_QUANTIZERS = "activation_quantizers"
 # In ActivationQuantizationHolder only one quantizer is used thus a new attribute name is needed
 ACTIVATION_HOLDER_QUANTIZER = "activation_holder_quantizer"
 
 # Quantizer signature parameters:
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/common/get_all_subclasses.py` & `mct-quantizers-1.2.0/mct_quantizers/common/get_all_subclasses.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/common/get_quantizers.py` & `mct-quantizers-1.2.0/mct_quantizers/common/get_quantizers.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,16 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
-from mct_quantizers.common.base_inferable_quantizer import QuantizationTarget
-from mct_quantizers.common.constants import QUANTIZATION_TARGET, QUANTIZATION_METHOD
+from mct_quantizers.common.base_inferable_quantizer import QuantizationTarget, QuantizerID
+from mct_quantizers.common.constants import QUANTIZATION_TARGET, QUANTIZATION_METHOD, QUANTIZER_ID
 from mct_quantizers.common.get_all_subclasses import get_all_subclasses
 from mct_quantizers.common.quant_info import QuantizationMethod
 from mct_quantizers.logger import Logger
 
 
 def get_inferable_quantizer_class(quant_target: QuantizationTarget,
                                   quant_method: QuantizationMethod,
@@ -33,17 +33,19 @@
             quantizer supports.
         quantizer_base_class: A type of quantizer that the requested quantizer should inherit from.
 
     Returns: A class of a quantizer that inherits from the given quantizer_base_class.
 
     """
     qat_quantizer_classes = get_all_subclasses(quantizer_base_class)
+
     filtered_quantizers = list(filter(lambda q_class: getattr(q_class, QUANTIZATION_TARGET) == quant_target and
                                                       getattr(q_class, QUANTIZATION_METHOD) is not None and
-                                                      quant_method in getattr(q_class, QUANTIZATION_METHOD),
+                                                      quant_method in getattr(q_class, QUANTIZATION_METHOD) and
+                                                      getattr(q_class, QUANTIZER_ID) is QuantizerID.INFERABLE,
                                       qat_quantizer_classes))
 
     if len(filtered_quantizers) != 1:
         Logger.error(f"Found {len(filtered_quantizers)} quantizer for target {quant_target.value} "
                      f"that matches the requested quantization method {quant_method.name} "
                      f"but there should be exactly one."
                      f"The possible quantizers that were found are {filtered_quantizers}.")
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/common/quant_info.py` & `mct-quantizers-1.2.0/mct_quantizers/common/quant_info.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/common/quant_utils.py` & `mct-quantizers-1.2.0/mct_quantizers/common/quant_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/__init__.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/activation_quantization_holder.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/activation_quantization_holder.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,24 +9,23 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
-
 from mct_quantizers.common.base_inferable_quantizer import BaseInferableQuantizer
 from mct_quantizers.common.constants import ACTIVATION_HOLDER_QUANTIZER, FOUND_TF, TRAINING, STEPS
 from mct_quantizers.common.get_all_subclasses import get_all_subclasses
 from mct_quantizers.logger import Logger
 
 if FOUND_TF:
     import tensorflow as tf
-    from keras.utils import tf_inspect
-    from tensorflow_model_optimization.python.core.keras import utils
+    from tensorflow.python.util import tf_inspect
+    from tensorflow.python.keras.utils.control_flow_util import smart_cond
     from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
 
     keras = tf.keras
 
 
     def _make_quantizer_fn(quantizer, x, training):
         """Use currying to return True/False specialized fns to the cond."""
@@ -122,15 +121,15 @@
 
             """
             if training is None:
                 training = tf.keras.backend.learning_phase()
 
             activation_quantizer_args_spec = tf_inspect.getfullargspec(self.activation_holder_quantizer.__call__).args
             if TRAINING in activation_quantizer_args_spec:
-                return utils.smart_cond(
+                return smart_cond(
                     training,
                     _make_quantizer_fn(self.activation_holder_quantizer, inputs, True),
                     _make_quantizer_fn(self.activation_holder_quantizer, inputs, False))
 
             return self.activation_holder_quantizer(inputs)
 
         def convert_to_inferable_quantizers(self):
@@ -145,10 +144,10 @@
                 self.activation_holder_quantizer = self.activation_holder_quantizer.convert2inferable()
                 return self.from_config(self.get_config()) # return new layer with no weights. It assumes holder of inferable quantizers have no weights
 
 
 else:
     class KerasActivationQuantizationHolder:  # pragma: no cover
         def __init__(self, *args, **kwargs):
-            Logger.error('Installing tensorflow and tensorflow_model_optimization is mandatory '
+            Logger.error('Installing tensorflow is mandatory '
                          'when using ActivationQuantizationHolder. '
                          'Could not find Tensorflow package.')
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/load_model.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/load_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,10 +68,10 @@
             custom_objects: Additional custom objects
             compile: Boolean, whether to compile the model after loading.
             options: Optional `tf.saved_model.LoadOptions` object that specifies options for loading from SavedModel.
 
         Returns: A keras Model
 
         """
-        Logger.critical('Installing tensorflow and tensorflow_model_optimization is mandatory '
+        Logger.critical('Installing tensorflow is mandatory '
                         'when using keras_load_quantized_model. '
                         'Could not find Tensorflow package.')  # pragma: no cover
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/quantize_wrapper.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/quantize_wrapper.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,16 @@
 from mct_quantizers.common.constants import FOUND_TF, WEIGHTS_QUANTIZERS, STEPS, LAYER, TRAINING
 from mct_quantizers.logger import Logger
 from mct_quantizers.common.get_all_subclasses import get_all_subclasses
 
 if FOUND_TF:
     import tensorflow as tf
     from tensorflow.python.util import tf_inspect
-    from tensorflow_model_optimization.python.core.keras import utils
+    from tensorflow.python.keras.utils.control_flow_util import smart_cond
+
     from mct_quantizers.keras.quantizers import BaseKerasInferableQuantizer
 
     keras = tf.keras
 
     def _make_quantizer_fn(quantizer, x, training):
         """Use currying to return True/False specialized fns to the cond."""
 
@@ -196,15 +197,15 @@
 
             # Quantize all weights, and replace them in the underlying layer.
             quantized_weights = {}
             for name, unquantized_weight, quantizer in self._weights_vars:
 
                 weights_quantizer_args_spec = tf_inspect.getfullargspec(quantizer.__call__).args
                 if TRAINING in weights_quantizer_args_spec:
-                    quantized_weight = utils.smart_cond(
+                    quantized_weight = smart_cond(
                         training,
                         _make_quantizer_fn(quantizer, unquantized_weight, True),
                         _make_quantizer_fn(quantizer, unquantized_weight, False))
                     quantized_weights.update({name: quantized_weight})
                 else:
                     # Keras weights inferable quantizer
                     quantized_weight = quantizer(unquantized_weight)
@@ -279,10 +280,10 @@
             """
             Keras Quantization Wrapper takes a keras layer and quantizers and infer a quantized layer.
 
             Args:
                 layer: A keras layer.
                 weights_quantizers: A dictionary between a weight's name to its quantizer.
             """
-            Logger.critical('Installing tensorflow and tensorflow_model_optimization is mandatory '
+            Logger.critical('Installing tensorflow is mandatory '
                             'when using KerasQuantizationWrapper. '
                             'Could not find Tensorflow package.')  # pragma: no cover
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/quantizer_utils.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/__init__.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 # limitations under the License.
 # ==============================================================================
 import warnings
 from typing import List
 
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget, QuantizerID
 from mct_quantizers.common.constants import FOUND_TF, MULTIPLIER_N_BITS, EPS
 from mct_quantizers.common.quant_info import QuantizationMethod
 from mct_quantizers.logger import Logger
 
 
 if FOUND_TF:
     import tensorflow as tf
     from mct_quantizers.keras.quantizer_utils import lut_quantizer
     from mct_quantizers.keras.quantizers.base_keras_inferable_quantizer import BaseKerasInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Activation,
                     quantization_method=[QuantizationMethod.LUT_POT_QUANTIZER],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class ActivationLutPOTInferableQuantizer(BaseKerasInferableQuantizer):
         """
         Class for quantizing activations using lut power-of-two quantizer
         """
 
         def __init__(self,
                      num_bits: int,
@@ -150,10 +150,10 @@
                     'multiplier_n_bits': self.multiplier_n_bits,
                     'eps': self.eps}
 
 
 else:
     class ActivationLutPOTInferableQuantizer:  # pragma: no cover
         def __init__(self, *args, **kwargs):
-            Logger.error('Installing tensorflow and tensorflow_model_optimization is mandatory '
+            Logger.error('Installing tensorflow is mandatory '
                          'when using ActivationLutPOTInferableQuantizer. '
                          'Could not find Tensorflow package.')
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget, QuantizerID
 from mct_quantizers.common.constants import FOUND_TF
 from mct_quantizers.common.quant_info import QuantizationMethod
 from mct_quantizers.logger import Logger
 
 
 if FOUND_TF:
     from mct_quantizers.keras.quantizers.activation_inferable_quantizers.activation_symmetric_inferable_quantizer import \
         ActivationSymmetricInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Activation,
                     quantization_method=[QuantizationMethod.POWER_OF_TWO],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class ActivationPOTInferableQuantizer(ActivationSymmetricInferableQuantizer):
         """
         Class for quantizing activations using power-of-two quantizer
         """
 
         def __init__(self,
                      num_bits: int,
@@ -54,10 +54,10 @@
 
             is_threshold_pot = np.all([int(np.log2(x)) == np.log2(x) for x in np.asarray(self.threshold).flatten()])
             assert is_threshold_pot, f'Expected threshold to be power of 2 but is {self.threshold}'
 
 else:
     class ActivationPOTInferableQuantizer:  # pragma: no cover
         def __init__(self, *args, **kwargs):
-            Logger.error('Installing tensorflow and tensorflow_model_optimization is mandatory '
+            Logger.error('Installing tensorflow is mandatory '
                          'when using ActivationPOTInferableQuantizer. '
                          'Could not find Tensorflow package.')
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget, QuantizerID
 from mct_quantizers.common.constants import FOUND_TF
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 
 if FOUND_TF:
     import tensorflow as tf
     from mct_quantizers.keras.quantizers.activation_inferable_quantizers.activation_uniform_inferable_quantizer \
         import ActivationUniformInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Activation,
                     quantization_method=[QuantizationMethod.SYMMETRIC],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class ActivationSymmetricInferableQuantizer(ActivationUniformInferableQuantizer):
 
         """
         Class for quantizing activations using a symmetric quantizer
         """
 
         def __init__(self,
@@ -77,10 +77,10 @@
                     'signed': self.signed,
                     'threshold': self.threshold}
 
 
 else:
     class ActivationSymmetricInferableQuantizer:  # pragma: no cover
         def __init__(self, *args, **kwargs):
-            raise Exception('Installing tensorflow and tensorflow_model_optimization is mandatory '
+            raise Exception('Installing tensorflow is mandatory '
                             'when using ActivationSymmetricInferableQuantizer. '
                             'Could not find Tensorflow package.')
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget, QuantizerID
 from mct_quantizers.common.constants import FOUND_TF
 from mct_quantizers.common.quant_info import QuantizationMethod
 from mct_quantizers.common.quant_utils import adjust_range_to_include_zero
 from mct_quantizers.logger import Logger
 
 
 if FOUND_TF:
     import tensorflow as tf
     from mct_quantizers.keras.validation_functions import validate_uniform_min_max_ranges, validate_adjusted_min_max_ranges
     from mct_quantizers.keras.quantizers.base_keras_inferable_quantizer import BaseKerasInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Activation,
                     quantization_method=[QuantizationMethod.UNIFORM],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class ActivationUniformInferableQuantizer(BaseKerasInferableQuantizer):
         """
         Class for quantizing activations using an uniform quantizer
         """
 
         def __init__(self,
                      num_bits: int,
@@ -102,10 +102,10 @@
             return {'num_bits': self.num_bits,
                     'min_range': self.min_range,
                     'max_range': self.max_range}
 
 else:
     class ActivationUniformInferableQuantizer:  # pragma: no cover
         def __init__(self, *args, **kwargs):
-            Logger.error('Installing tensorflow and tensorflow_model_optimization is mandatory '
+            Logger.error('Installing tensorflow is mandatory '
                          'when using ActivationUniformInferableQuantizer. '
                          'Could not find Tensorflow package.')
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/base_keras_inferable_quantizer.py`

 * *Files 9% similar despite different names*

```diff
@@ -45,12 +45,12 @@
             Returns:
                 quantized tensor.
             """
             raise NotImplemented(f'{self.__class__.__name__} did not implement __call__')  # pragma: no cover
 else:
     class BaseKerasInferableQuantizer:  # pragma: no cover
         def __init__(self, *args, **kwargs):
-            raise Exception('Installing tensorflow and tensorflow_model_optimization is mandatory '
+            raise Exception('Installing tensorflow is mandatory '
                             'when using BaseKerasInferableQuantizer. '
                             'Could not find Tensorflow package.')
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,27 +12,27 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget, QuantizerID
 from mct_quantizers.common.constants import FOUND_TF, MULTIPLIER_N_BITS, EPS
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 
 if FOUND_TF:
     from mct_quantizers.keras.quantizers.weights_inferable_quantizers.weights_lut_symmetric_inferable_quantizer import \
         WeightsLUTSymmetricInferableQuantizer
 
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.LUT_POT_QUANTIZER],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class WeightsLUTPOTInferableQuantizer(WeightsLUTSymmetricInferableQuantizer):
         """
         Class for quantizing weights using a lut power-of-two quantizer
         """
 
         def __init__(self,
                      num_bits: int,
@@ -69,10 +69,10 @@
             is_threshold_pot = np.all([int(np.log2(x)) == np.log2(x) for x in self._np_threshold.flatten()])
             assert is_threshold_pot, f'Expected threshold to be power of 2 but is {self._np_threshold}'
 
 
 else:
     class WeightsLUTPOTInferableQuantizer:  # pragma: no cover
         def __init__(self, *args, **kwargs):
-            raise Exception('Installing tensorflow and tensorflow_model_optimization is mandatory '
+            raise Exception('Installing tensorflow is mandatory '
                             'when using WeightsLUTPOTInferableQuantizer. '
                             'Could not find Tensorflow package.')
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,28 +13,28 @@
 # limitations under the License.
 # ==============================================================================
 import warnings
 from typing import List
 
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import QuantizationTarget, mark_quantizer
+from mct_quantizers.common.base_inferable_quantizer import QuantizationTarget, mark_quantizer, QuantizerID
 from mct_quantizers.common.constants import FOUND_TF, MULTIPLIER_N_BITS, EPS
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 
 if FOUND_TF:
     import tensorflow as tf
     from mct_quantizers.keras.quantizer_utils import lut_quantizer
     from mct_quantizers.keras.quantizers.base_keras_inferable_quantizer import BaseKerasInferableQuantizer
 
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.LUT_SYM_QUANTIZER],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class WeightsLUTSymmetricInferableQuantizer(BaseKerasInferableQuantizer):
         """
         Class for quantizing weights using a lut symmetric quantizer
         """
 
         def __init__(self,
                      num_bits: int,
@@ -178,10 +178,10 @@
                     'input_rank': self.input_rank,
                     'multiplier_n_bits': self.multiplier_n_bits,
                     'eps': self.eps}
 
 else:
     class WeightsLUTSymmetricInferableQuantizer:  # pragma: no cover
         def __init__(self, *args, **kwargs):
-            raise Exception('Installing tensorflow and tensorflow_model_optimization is mandatory '
+            raise Exception('Installing tensorflow is mandatory '
                             'when using WeightsLUTSymmetricInferableQuantizer. '
                             'Could not find Tensorflow package.')
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import QuantizationTarget, mark_quantizer
+from mct_quantizers.common.base_inferable_quantizer import QuantizationTarget, mark_quantizer, QuantizerID
 from mct_quantizers.common.constants import FOUND_TF
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 
 if FOUND_TF:
     from mct_quantizers.keras.quantizers.weights_inferable_quantizers.weights_symmetric_inferable_quantizer import \
         WeightsSymmetricInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.POWER_OF_TWO],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class WeightsPOTInferableQuantizer(WeightsSymmetricInferableQuantizer):
         """
-        Class for quantizing weights using power-of-two quantizer
+        Class for quantizing weights using unsigned power-of-two quantizer.
         """
 
         def __init__(self,
                      num_bits: int,
                      threshold: List[float],
                      per_channel: bool,
                      channel_axis: int = None,
@@ -59,10 +59,10 @@
             is_threshold_pot = np.all([int(np.log2(x)) == np.log2(x) for x in self._np_threshold.flatten()])
             assert is_threshold_pot, f'Expected threshold to be power of 2 but is {self.threshold}'
 
 
 else:
     class WeightsPOTInferableQuantizer:  # pragma: no cover
         def __init__(self, *args, **kwargs):
-            raise Exception('Installing tensorflow and tensorflow_model_optimization is mandatory '
+            raise Exception('Installing tensorflow is mandatory '
                             'when using WeightsPOTInferableQuantizer. '
                             'Could not find Tensorflow package.')
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,29 +12,29 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget, QuantizerID
 from mct_quantizers.common.constants import FOUND_TF
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 
 if FOUND_TF:
     from mct_quantizers.keras.quantizers.weights_inferable_quantizers.weights_uniform_inferable_quantizer import \
         WeightsUniformInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.SYMMETRIC],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class WeightsSymmetricInferableQuantizer(WeightsUniformInferableQuantizer):
         """
-        Class for quantizing weights using a symmetric quantizer
+        Class for quantizing weights using unsigned symmetric quantizer.
         """
         def __init__(self,
                      num_bits: int,
                      threshold: List[float],
                      per_channel: bool,
                      channel_axis: int = None,
                      input_rank: int = None
@@ -78,10 +78,10 @@
                     'per_channel': self.per_channel,
                     'channel_axis': self.channel_axis,
                     'input_rank': self.input_rank}
 
 else:
     class WeightsSymmetricInferableQuantizer:  # pragma: no cover
         def __init__(self, *args, **kwargs):
-            raise Exception('Installing tensorflow and tensorflow_model_optimization is mandatory '
+            raise Exception('Installing tensorflow is mandatory '
                             'when using WeightsPOTInferableQuantizer. '
                             'Could not find Tensorflow package.')
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,32 +12,32 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 from typing import List
 
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import QuantizationTarget, mark_quantizer
+from mct_quantizers.common.base_inferable_quantizer import QuantizationTarget, mark_quantizer, QuantizerID
 from mct_quantizers.common.constants import FOUND_TF
 from mct_quantizers.common.quant_info import QuantizationMethod
 from mct_quantizers.common.quant_utils import adjust_range_to_include_zero
 
 
 if FOUND_TF:
     import tensorflow as tf
     from mct_quantizers.keras.quantizers.base_keras_inferable_quantizer import BaseKerasInferableQuantizer
     from mct_quantizers.keras.validation_functions import validate_uniform_min_max_ranges, \
         validate_adjusted_min_max_ranges
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.UNIFORM],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class WeightsUniformInferableQuantizer(BaseKerasInferableQuantizer):
         """
-        Class for quantizing weights using a uniform quantizer
+        Class for quantizing weights using unsigned uniform quantizer
         """
         def __init__(self,
                      num_bits: int,
                      min_range: List[float],
                      max_range: List[float],
                      per_channel: bool,
                      channel_axis: int = None,
@@ -157,10 +157,10 @@
                     'channel_axis': self.channel_axis,
                     'input_rank': self.input_rank}
 
 
 else:
     class WeightsUniformInferableQuantizer:  # pragma: no cover
         def __init__(self, *args, **kwargs):
-            raise Exception('Installing tensorflow and tensorflow_model_optimization is mandatory '
+            raise Exception('Installing tensorflow is mandatory '
                             'when using WeightsUniformInferableQuantizer. '
                             'Could not find Tensorflow package.')
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/keras/validation_functions.py` & `mct-quantizers-1.2.0/mct_quantizers/keras/validation_functions.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/logger.py` & `mct-quantizers-1.2.0/mct_quantizers/logger.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/__init__.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/activation_quantization_holder.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/activation_quantization_holder.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/load_model.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/load_model.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantize_wrapper.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantize_wrapper.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizer_utils.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizer_utils.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/__init__.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_lut_pot_inferable_quantizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,27 +10,27 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget, QuantizerID
 from mct_quantizers.common.constants import FOUND_TORCH, MULTIPLIER_N_BITS, EPS
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 
 if FOUND_TORCH:
     import torch
     from mct_quantizers.pytorch.quantizers.base_lut_symmetric_inferable_quantizer import BaseLUTSymmetricInferableQuantizer
     from mct_quantizers.pytorch.quantizer_utils import to_torch_tensor, get_working_device, lut_quantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Activation,
                     quantization_method=[QuantizationMethod.LUT_POT_QUANTIZER],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class ActivationLutPOTInferableQuantizer(BaseLUTSymmetricInferableQuantizer):
         """
         Class for quantizing activations using a lut power-of-two quantizer
         """
 
         def __init__(self,
                      num_bits: int,
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_pot_inferable_quantizer.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget, QuantizerID
 from mct_quantizers.common.constants import FOUND_TORCH
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 
 if FOUND_TORCH:
     from mct_quantizers.pytorch.quantizers.activation_inferable_quantizers.activation_symmetric_inferable_quantizer import \
         ActivationSymmetricInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Activation,
                     quantization_method=[QuantizationMethod.POWER_OF_TWO],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class ActivationPOTInferableQuantizer(ActivationSymmetricInferableQuantizer):
         """
         Class for quantizing activations using power-of-two quantizer
         """
 
         def __init__(self,
                      num_bits: int,
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_symmetric_inferable_quantizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget, QuantizerID
 from mct_quantizers.common.constants import FOUND_TORCH
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 
 if FOUND_TORCH:
     import torch
     from mct_quantizers.pytorch.quantizers.base_symmetric_inferable_quantizer import BaseSymmetricInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Activation,
                     quantization_method=[QuantizationMethod.SYMMETRIC],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class ActivationSymmetricInferableQuantizer(BaseSymmetricInferableQuantizer):
         """
         Class for quantizing activations using a symmetric quantizer
         """
 
         def __init__(self,
                      num_bits: int,
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/activation_inferable_quantizers/activation_uniform_inferable_quantizer.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,26 +10,26 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget, QuantizerID
 from mct_quantizers.common.constants import FOUND_TORCH
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 if FOUND_TORCH:
     import torch
     from mct_quantizers.pytorch.quantizers.base_uniform_inferable_quantizer import BaseUniformInferableQuantizer
 
 
     @mark_quantizer(quantization_target=QuantizationTarget.Activation,
                     quantization_method=[QuantizationMethod.UNIFORM],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class ActivationUniformInferableQuantizer(BaseUniformInferableQuantizer):
         """
         Class for quantizing activations using an uniform quantizer
         """
 
         def __init__(self,
                      num_bits: int,
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/base_lut_symmetric_inferable_quantizer.py`

 * *Files 5% similar despite different names*

```diff
@@ -11,25 +11,25 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 import warnings
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizerID
 from mct_quantizers.common.constants import FOUND_TORCH
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 
 if FOUND_TORCH:
     from mct_quantizers.pytorch.quantizers.base_pytorch_inferable_quantizer import BasePyTorchInferableQuantizer
 
     @mark_quantizer(quantization_target=None,
                     quantization_method=[QuantizationMethod.LUT_SYM_QUANTIZER],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class BaseLUTSymmetricInferableQuantizer(BasePyTorchInferableQuantizer):
 
         def __init__(self,
                      num_bits: int,
                      cluster_centers: np.ndarray,
                      threshold: np.ndarray,
                      signed: bool,
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/base_pytorch_inferable_quantizer.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/base_symmetric_inferable_quantizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizerID
 from mct_quantizers.common.constants import FOUND_TORCH
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 
 if FOUND_TORCH:
     from mct_quantizers.pytorch.quantizers.base_pytorch_inferable_quantizer import BasePyTorchInferableQuantizer
 
     @mark_quantizer(quantization_target=None,
                     quantization_method=[QuantizationMethod.SYMMETRIC],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class BaseSymmetricInferableQuantizer(BasePyTorchInferableQuantizer):
 
         def __init__(self,
                      num_bits: int,
                      threshold: np.ndarray,
                      signed: bool):
             """
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/base_uniform_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizerID
 from mct_quantizers.common.constants import FOUND_TORCH
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 
 if FOUND_TORCH:
     from mct_quantizers.pytorch.quantizers.base_pytorch_inferable_quantizer import BasePyTorchInferableQuantizer
 
     @mark_quantizer(quantization_target=None,
                     quantization_method=[QuantizationMethod.UNIFORM],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class BaseUniformInferableQuantizer(BasePyTorchInferableQuantizer):
 
         def __init__(self,
                      num_bits: int,
                      min_range: np.ndarray,
                      max_range: np.ndarray):
             """
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/__init__.py`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_pot_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget, QuantizerID
 from mct_quantizers.common.constants import FOUND_TORCH, MULTIPLIER_N_BITS, EPS
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 
 if FOUND_TORCH:
     from mct_quantizers.pytorch.quantizers.weights_inferable_quantizers.weights_lut_symmetric_inferable_quantizer import \
         WeightsLUTSymmetricInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.LUT_POT_QUANTIZER],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class WeightsLUTPOTInferableQuantizer(WeightsLUTSymmetricInferableQuantizer):
         """
         Class for quantizing weights using lut power-of-two quantizer
         """
 
         def __init__(self,
                      num_bits: int,
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_lut_symmetric_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,28 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget, QuantizerID
 from mct_quantizers.common.constants import FOUND_TORCH, MULTIPLIER_N_BITS, EPS
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 
 if FOUND_TORCH:
     import torch
     from mct_quantizers.pytorch.quantizer_utils import to_torch_tensor, get_working_device, lut_quantizer
     from mct_quantizers.pytorch.quantizers.base_lut_symmetric_inferable_quantizer import \
         BaseLUTSymmetricInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.LUT_SYM_QUANTIZER],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class WeightsLUTSymmetricInferableQuantizer(BaseLUTSymmetricInferableQuantizer):
         """
         Class for quantizing weights using a lut symmetric quantizer
         """
 
         def __init__(self,
                      num_bits: int,
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_pot_inferable_quantizer.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,29 +11,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget, QuantizerID
 from mct_quantizers.common.constants import FOUND_TORCH
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 
 if FOUND_TORCH:
     from mct_quantizers.pytorch.quantizers.weights_inferable_quantizers.weights_symmetric_inferable_quantizer import \
         WeightsSymmetricInferableQuantizer
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.POWER_OF_TWO],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class WeightsPOTInferableQuantizer(WeightsSymmetricInferableQuantizer):
         """
-        Class for quantizing weights using power-of-two quantizer
+        Class for quantizing weights using unsigned power-of-two quantizer.
         """
 
         def __init__(self,
                      num_bits: int,
                      threshold: np.ndarray,
                      per_channel: bool,
                      channel_axis: int = None
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_symmetric_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget, QuantizerID
 from mct_quantizers.common.constants import FOUND_TORCH
 from mct_quantizers.common.quant_info import QuantizationMethod
 
 
 if FOUND_TORCH:
     import torch
     from mct_quantizers.pytorch.quantizers.base_symmetric_inferable_quantizer import BaseSymmetricInferableQuantizer
     from mct_quantizers.pytorch.quantizer_utils import to_torch_tensor, get_working_device
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.SYMMETRIC],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class WeightsSymmetricInferableQuantizer(BaseSymmetricInferableQuantizer):
         """
-        Class for quantizing weights using a symmetric quantizer
+        Class for quantizing weights using unsigned symmetric quantizer.
         """
 
         def __init__(self,
                      num_bits: int,
                      threshold: np.ndarray,
                      per_channel: bool,
                      channel_axis: int = None
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py` & `mct-quantizers-1.2.0/mct_quantizers/pytorch/quantizers/weights_inferable_quantizers/weights_uniform_inferable_quantizer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,30 +11,30 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 # ==============================================================================
 
 import numpy as np
 
-from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget
+from mct_quantizers.common.base_inferable_quantizer import mark_quantizer, QuantizationTarget, QuantizerID
 from mct_quantizers.common.constants import FOUND_TORCH
 from mct_quantizers.common.quant_info import QuantizationMethod
 from mct_quantizers.logger import Logger
 
 if FOUND_TORCH:
     import torch
     from mct_quantizers.pytorch.quantizers.base_uniform_inferable_quantizer import BaseUniformInferableQuantizer
     from mct_quantizers.pytorch.quantizer_utils import fix_range_to_include_zero, get_working_device, to_torch_tensor
 
     @mark_quantizer(quantization_target=QuantizationTarget.Weights,
                     quantization_method=[QuantizationMethod.UNIFORM],
-                    quantizer_type=None)
+                    identifier=QuantizerID.INFERABLE)
     class WeightsUniformInferableQuantizer(BaseUniformInferableQuantizer):
         """
-        Class for quantizing weights using a uniform quantizer
+        Class for quantizing weights using unsigned uniform quantizer.
         """
 
         def __init__(self,
                      num_bits: int,
                      min_range: np.ndarray,
                      max_range: np.ndarray,
                      per_channel: bool,
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers.egg-info/PKG-INFO` & `mct-quantizers-1.2.0/mct_quantizers.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mct-quantizers
-Version: 1.1.0
+Version: 1.2.0
 Summary: Infrastructure for support neural networks compression
 Home-page: UNKNOWN
 License: UNKNOWN
 Description: # Model Compression Toolkit (MCT) Quantizers
         
         The MCT Quantizers library is an open-source library developed by researchers and engineers working at Sony Semiconductor Israel. 
         
@@ -33,15 +33,15 @@
         2. [Pytorch Quantizers](mct_quantizers/pytorch/quantizers)
         
         ### The mark_quantizer Decorator
         
         The [`@mark_quantizer`](mct_quantizers/common/base_inferable_quantizer.py) decorator is used to assign each quantizer with static properties that define its task compatibility. Each quantizer class should be decorated with this decorator, which defines the following properties:
          - [`QuantizationTarget`](mct_quantizers/common/base_inferable_quantizer.py): An Enum that indicates whether the quantizer is intended for weights or activations quantization.
          - [`QuantizationMethod`](mct_quantizers/common/quant_info.py): A list of quantization methods (Uniform, Symmetric, etc.).
-         - `quantizer_type`: An optional property that defines the type of the quantization technique. This is a helper property that allows the creation of advanced quantizers for specific tasks.
+         - `identifier`: A unique identifier for the quantizer class. This is a helper property that allows the creation of advanced quantizers for specific tasks.
          
         ## Getting Started
         
         This section provides a quick guide to getting started. We begin with the installation process, either via source code or the pip server. Then, we provide a short example of usage.
         
         ### Installation
         Please refer to the MCT install guide for installing the pip package or building from the source.
@@ -58,17 +58,16 @@
         pip install mct-quantizers-nightly
         ```
         
         ### Requirements
         
         To use MCT Quantizers, you need to have one of the supported frameworks, Tensorflow or PyTorch, installed.
         
-        For use with Tensorflow, please install the following packages:
-        [tensorflow](https://www.tensorflow.org/install), 
-        [tensorflow-model-optimization](https://www.tensorflow.org/model_optimization/guide/install)
+        For use with Tensorflow, please install the following package:
+        [tensorflow](https://www.tensorflow.org/install),
         
         For use with PyTorch, please install the following package:
         [torch](https://pytorch.org/)
         
         You can also use the [requirements](requirements.txt) file to set up your environment.
         
         ## License
```

### Comparing `mct-quantizers-1.1.0/mct_quantizers.egg-info/SOURCES.txt` & `mct-quantizers-1.2.0/mct_quantizers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mct-quantizers-1.1.0/setup.py` & `mct-quantizers-1.2.0/setup.py`

 * *Files identical despite different names*

