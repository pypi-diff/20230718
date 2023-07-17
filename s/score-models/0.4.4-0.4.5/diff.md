# Comparing `tmp/score_models-0.4.4.tar.gz` & `tmp/score_models-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "score_models-0.4.4.tar", last modified: Mon Jul 17 04:58:40 2023, max compression
+gzip compressed data, was "score_models-0.4.5.tar", last modified: Mon Jul 17 22:55:06 2023, max compression
```

## Comparing `score_models-0.4.4.tar` & `score_models-0.4.5.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 04:58:40.734296 score_models-0.4.4/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1081 2023-07-06 14:56:40.000000 score_models-0.4.4/LICENSE.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-07-17 04:58:40.734296 score_models-0.4.4/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5617 2023-07-13 16:06:46.000000 score_models-0.4.4/README.md
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       90 2023-07-06 13:52:30.000000 score_models-0.4.4/pyproject.toml
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 04:58:40.730296 score_models-0.4.4/score_models/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       94 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/__init__.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 04:58:40.730296 score_models-0.4.4/score_models/architectures/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/architectures/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4940 2023-07-13 23:11:59.000000 score_models-0.4.4/score_models/architectures/ddpm.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3557 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/architectures/mlp.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    15113 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/architectures/ncsnpp.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    20659 2023-07-17 04:41:11.000000 score_models-0.4.4/score_models/base.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2035 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/definitions.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 04:58:40.734296 score_models-0.4.4/score_models/layers/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      686 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3574 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/attention_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      601 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/combine.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2766 2023-03-05 17:43:23.000000 score_models-0.4.4/score_models/layers/conditional_batchnorm2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2279 2023-03-05 17:43:23.000000 score_models-0.4.4/score_models/layers/conditional_instancenorm2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2980 2023-03-05 17:43:23.000000 score_models-0.4.4/score_models/layers/conditional_instancenorm2d_plus.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2903 2023-03-05 17:43:23.000000 score_models-0.4.4/score_models/layers/conv1dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3120 2023-03-05 17:43:23.000000 score_models-0.4.4/score_models/layers/conv2dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3134 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/conv3dsame.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1111 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/conv_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3354 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/ddpm_resnet_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1950 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/downsample.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3543 2023-03-05 17:43:23.000000 score_models-0.4.4/score_models/layers/ncsn_resnet_block.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      611 2023-03-05 17:43:23.000000 score_models-0.4.4/score_models/layers/projection_embedding.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3232 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/resnet_block_biggan.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2447 2023-03-05 17:43:23.000000 score_models-0.4.4/score_models/layers/spectral_normalization.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      862 2023-03-05 17:43:23.000000 score_models-0.4.4/score_models/layers/squeeze_and_excitation.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2123 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/style_gan_conv.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1957 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/up_or_downsampling.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6493 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/up_or_downsampling1d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7626 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/up_or_downsampling2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7507 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/up_or_downsampling3d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1485 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/upfirdn1d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1720 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/upfirdn2d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2053 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/upfirdn3d.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1558 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/layers/upsample.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1647 2023-07-17 04:57:57.000000 score_models-0.4.4/score_models/score_model.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 04:58:40.734296 score_models-0.4.4/score_models/sde/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/sde/__init__.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1348 2023-07-13 23:11:59.000000 score_models-0.4.4/score_models/sde/sde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2110 2023-07-13 23:11:59.000000 score_models-0.4.4/score_models/sde/vesde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1577 2023-07-13 23:11:59.000000 score_models-0.4.4/score_models/sde/vpsde.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3101 2023-07-13 23:11:59.000000 score_models-0.4.4/score_models/sliced_score_matching.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3672 2023-07-06 13:52:30.000000 score_models-0.4.4/score_models/utils.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 04:58:40.730296 score_models-0.4.4/score_models.egg-info/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-07-17 04:58:40.000000 score_models-0.4.4/score_models.egg-info/PKG-INFO
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1764 2023-07-17 04:58:40.000000 score_models-0.4.4/score_models.egg-info/SOURCES.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-07-17 04:58:40.000000 score_models-0.4.4/score_models.egg-info/dependency_links.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       43 2023-07-17 04:58:40.000000 score_models-0.4.4/score_models.egg-info/requires.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       13 2023-07-17 04:58:40.000000 score_models-0.4.4/score_models.egg-info/top_level.txt
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-07-17 04:58:40.734296 score_models-0.4.4/setup.cfg
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      880 2023-07-17 04:58:24.000000 score_models-0.4.4/setup.py
-drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 04:58:40.734296 score_models-0.4.4/tests/
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1231 2023-07-06 13:52:30.000000 score_models-0.4.4/tests/test_architectures.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6839 2023-07-06 13:52:30.000000 score_models-0.4.4/tests/test_layers.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2361 2023-07-13 23:11:59.000000 score_models-0.4.4/tests/test_score_models.py
--rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2888 2023-07-13 23:11:59.000000 score_models-0.4.4/tests/test_training.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 22:55:06.790813 score_models-0.4.5/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1081 2023-07-06 14:56:40.000000 score_models-0.4.5/LICENSE.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-07-17 22:55:06.790813 score_models-0.4.5/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     5617 2023-07-13 16:06:46.000000 score_models-0.4.5/README.md
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       90 2023-07-06 13:52:30.000000 score_models-0.4.5/pyproject.toml
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 22:55:06.786813 score_models-0.4.5/score_models/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       94 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/__init__.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 22:55:06.786813 score_models-0.4.5/score_models/architectures/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/architectures/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     4940 2023-07-13 23:11:59.000000 score_models-0.4.5/score_models/architectures/ddpm.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3557 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/architectures/mlp.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    15113 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/architectures/ncsnpp.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)    20765 2023-07-17 22:53:49.000000 score_models-0.4.5/score_models/base.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2035 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/definitions.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 22:55:06.786813 score_models-0.4.5/score_models/layers/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      686 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3574 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/attention_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      601 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/combine.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2766 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/conditional_batchnorm2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2279 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/conditional_instancenorm2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2980 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/conditional_instancenorm2d_plus.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2903 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/conv1dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3120 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/conv2dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3134 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/conv3dsame.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1111 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/conv_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3354 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/ddpm_resnet_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1950 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/downsample.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3543 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/ncsn_resnet_block.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      611 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/projection_embedding.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3232 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/resnet_block_biggan.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2447 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/spectral_normalization.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      862 2023-03-05 17:43:23.000000 score_models-0.4.5/score_models/layers/squeeze_and_excitation.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2123 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/style_gan_conv.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1957 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/up_or_downsampling.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6493 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/up_or_downsampling1d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7626 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/up_or_downsampling2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     7507 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/up_or_downsampling3d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1485 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/upfirdn1d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1720 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/upfirdn2d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2053 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/upfirdn3d.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1558 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/layers/upsample.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1647 2023-07-17 04:57:57.000000 score_models-0.4.5/score_models/score_model.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 22:55:06.786813 score_models-0.4.5/score_models/sde/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       71 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/sde/__init__.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1348 2023-07-13 23:11:59.000000 score_models-0.4.5/score_models/sde/sde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2110 2023-07-13 23:11:59.000000 score_models-0.4.5/score_models/sde/vesde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1577 2023-07-13 23:11:59.000000 score_models-0.4.5/score_models/sde/vpsde.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3101 2023-07-17 18:30:38.000000 score_models-0.4.5/score_models/sliced_score_matching.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     3672 2023-07-06 13:52:30.000000 score_models-0.4.5/score_models/utils.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 22:55:06.786813 score_models-0.4.5/score_models.egg-info/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6233 2023-07-17 22:55:06.000000 score_models-0.4.5/score_models.egg-info/PKG-INFO
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1764 2023-07-17 22:55:06.000000 score_models-0.4.5/score_models.egg-info/SOURCES.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)        1 2023-07-17 22:55:06.000000 score_models-0.4.5/score_models.egg-info/dependency_links.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       43 2023-07-17 22:55:06.000000 score_models-0.4.5/score_models.egg-info/requires.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       13 2023-07-17 22:55:06.000000 score_models-0.4.5/score_models.egg-info/top_level.txt
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)       38 2023-07-17 22:55:06.790813 score_models-0.4.5/setup.cfg
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)      880 2023-07-17 22:54:35.000000 score_models-0.4.5/setup.py
+drwxrwxr-x   0 alexandre  (1001) alexandre  (1001)        0 2023-07-17 22:55:06.786813 score_models-0.4.5/tests/
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     1231 2023-07-06 13:52:30.000000 score_models-0.4.5/tests/test_architectures.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     6839 2023-07-06 13:52:30.000000 score_models-0.4.5/tests/test_layers.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2361 2023-07-13 23:11:59.000000 score_models-0.4.5/tests/test_score_models.py
+-rw-rw-r--   0 alexandre  (1001) alexandre  (1001)     2888 2023-07-13 23:11:59.000000 score_models-0.4.5/tests/test_training.py
```

### Comparing `score_models-0.4.4/LICENSE.txt` & `score_models-0.4.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/PKG-INFO` & `score_models-0.4.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: score_models
-Version: 0.4.4
+Version: 0.4.5
 Summary: A simple pytorch interface for score model and basic diffusion.
 Home-page: https://github.com/AlexandreAdam/torch_score_models
 Author: Alexandre Adam
 Author-email: alexandre.adam@umontreal.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `score_models-0.4.4/README.md` & `score_models-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/architectures/ddpm.py` & `score_models-0.4.5/score_models/architectures/ddpm.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/architectures/mlp.py` & `score_models-0.4.5/score_models/architectures/mlp.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/architectures/ncsnpp.py` & `score_models-0.4.5/score_models/architectures/ncsnpp.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/base.py` & `score_models-0.4.5/score_models/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     def __init__(self, model: Union[str, Module]=None, sde:SDE=None, checkpoints_directory=None, device=DEVICE, **hyperparameters):
         super().__init__()
         if model is None and checkpoints_directory is None:
             raise ValueError("Must provide one of 'model'i or 'checkpoints_directory'")
         if model is None or isinstance(model, str):
             model, hyperparams = load_architecture(checkpoints_directory, model=model, device=device, hyperparameters=hyperparameters)
             hyperparameters.update(hyperparams)
+        elif hasattr(model, "hyperparameters"):
+            hyperparameters.update(model.hyperparameters)
         if sde is None:
             if "sigma_min" in hyperparameters.keys():
                 hyperparameters["sde"] = "vesde"
             elif "beta_min" in hyperparameters.keys():
                 hyperparameters["sde"] = "vpsde"
             else:
                 raise KeyError("SDE parameters are missing, please specify `sigma_min` and `sigma_max`"
```

### Comparing `score_models-0.4.4/score_models/definitions.py` & `score_models-0.4.5/score_models/definitions.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/__init__.py` & `score_models-0.4.5/score_models/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/attention_block.py` & `score_models-0.4.5/score_models/layers/attention_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/combine.py` & `score_models-0.4.5/score_models/layers/combine.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/conditional_batchnorm2d.py` & `score_models-0.4.5/score_models/layers/conditional_batchnorm2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/conditional_instancenorm2d.py` & `score_models-0.4.5/score_models/layers/conditional_instancenorm2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/conditional_instancenorm2d_plus.py` & `score_models-0.4.5/score_models/layers/conditional_instancenorm2d_plus.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/conv1dsame.py` & `score_models-0.4.5/score_models/layers/conv1dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/conv2dsame.py` & `score_models-0.4.5/score_models/layers/conv2dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/conv3dsame.py` & `score_models-0.4.5/score_models/layers/conv3dsame.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/conv_layers.py` & `score_models-0.4.5/score_models/layers/conv_layers.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/ddpm_resnet_block.py` & `score_models-0.4.5/score_models/layers/ddpm_resnet_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/downsample.py` & `score_models-0.4.5/score_models/layers/downsample.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/ncsn_resnet_block.py` & `score_models-0.4.5/score_models/layers/ncsn_resnet_block.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/projection_embedding.py` & `score_models-0.4.5/score_models/layers/projection_embedding.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/resnet_block_biggan.py` & `score_models-0.4.5/score_models/layers/resnet_block_biggan.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/spectral_normalization.py` & `score_models-0.4.5/score_models/layers/spectral_normalization.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/squeeze_and_excitation.py` & `score_models-0.4.5/score_models/layers/squeeze_and_excitation.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/style_gan_conv.py` & `score_models-0.4.5/score_models/layers/style_gan_conv.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/up_or_downsampling.py` & `score_models-0.4.5/score_models/layers/up_or_downsampling.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/up_or_downsampling1d.py` & `score_models-0.4.5/score_models/layers/up_or_downsampling1d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/up_or_downsampling2d.py` & `score_models-0.4.5/score_models/layers/up_or_downsampling2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/up_or_downsampling3d.py` & `score_models-0.4.5/score_models/layers/up_or_downsampling3d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/upfirdn1d.py` & `score_models-0.4.5/score_models/layers/upfirdn1d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/upfirdn2d.py` & `score_models-0.4.5/score_models/layers/upfirdn2d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/upfirdn3d.py` & `score_models-0.4.5/score_models/layers/upfirdn3d.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/layers/upsample.py` & `score_models-0.4.5/score_models/layers/upsample.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/score_model.py` & `score_models-0.4.5/score_models/score_model.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/sde/sde.py` & `score_models-0.4.5/score_models/sde/sde.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/sde/vesde.py` & `score_models-0.4.5/score_models/sde/vesde.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/sde/vpsde.py` & `score_models-0.4.5/score_models/sde/vpsde.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/sliced_score_matching.py` & `score_models-0.4.5/score_models/sliced_score_matching.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models/utils.py` & `score_models-0.4.5/score_models/utils.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/score_models.egg-info/PKG-INFO` & `score_models-0.4.5/score_models.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: score-models
-Version: 0.4.4
+Version: 0.4.5
 Summary: A simple pytorch interface for score model and basic diffusion.
 Home-page: https://github.com/AlexandreAdam/torch_score_models
 Author: Alexandre Adam
 Author-email: alexandre.adam@umontreal.ca
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `score_models-0.4.4/score_models.egg-info/SOURCES.txt` & `score_models-0.4.5/score_models.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/setup.py` & `score_models-0.4.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the contents of the README file
 with open("long_description.rst", "r") as fh:
     long_description = fh.read()
 
 setup(
 	name="score_models",
-	version="0.4.4",
+	version="0.4.5",
     description="A simple pytorch interface for score model and basic diffusion.",
     long_description=long_description,
     author="Alexandre Adam",
     author_email="alexandre.adam@umontreal.ca",
     url="https://github.com/AlexandreAdam/torch_score_models",
     packages=find_packages(),
     install_requires=[
```

### Comparing `score_models-0.4.4/tests/test_architectures.py` & `score_models-0.4.5/tests/test_architectures.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/tests/test_layers.py` & `score_models-0.4.5/tests/test_layers.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/tests/test_score_models.py` & `score_models-0.4.5/tests/test_score_models.py`

 * *Files identical despite different names*

### Comparing `score_models-0.4.4/tests/test_training.py` & `score_models-0.4.5/tests/test_training.py`

 * *Files identical despite different names*

