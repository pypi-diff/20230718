# Comparing `tmp/xGPR-0.1.2.3.tar.gz` & `tmp/xGPR-0.1.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xGPR-0.1.2.3.tar", last modified: Tue Jun 27 18:22:59 2023, max compression
+gzip compressed data, was "xGPR-0.1.2.4.tar", last modified: Mon Jul 17 22:45:31 2023, max compression
```

## Comparing `xGPR-0.1.2.3.tar` & `xGPR-0.1.2.4.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.023565 xGPR-0.1.2.3/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1067 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/LICENSE
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-27 18:22:59.023565 xGPR-0.1.2.3/PKG-INFO
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1449 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/README.md
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       78 2023-06-21 00:02:39.000000 xGPR-0.1.2.3/pyproject.toml
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-27 18:22:59.023565 xGPR-0.1.2.3/setup.cfg
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8142 2023-05-25 13:16:01.000000 xGPR-0.1.2.3/setup.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.015565 xGPR-0.1.2.3/xGPR/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      105 2023-06-27 17:44:19.000000 xGPR-0.1.2.3/xGPR/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.015565 xGPR-0.1.2.3/xGPR/cg_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/cg_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2180 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/cg_toolkit/cg_linear_operators.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11182 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/cg_toolkit/cg_tools.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3515 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/cg_toolkit/cuda_cg_linear_operators.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.015565 xGPR-0.1.2.3/xGPR/constants/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/constants/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      533 2023-03-15 23:05:25.000000 xGPR-0.1.2.3/xGPR/constants/constants.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.015565 xGPR-0.1.2.3/xGPR/data_handling/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/data_handling/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4337 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/data_handling/data_handling_baseclass.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13191 2023-06-22 23:01:08.000000 xGPR-0.1.2.3/xGPR/data_handling/dataset_builder.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2233 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/data_handling/minibatch_data_handler.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8618 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/data_handling/offline_data_handling.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6843 2023-06-07 22:48:32.000000 xGPR-0.1.2.3/xGPR/data_handling/online_data_handling.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.015565 xGPR-0.1.2.3/xGPR/fitting_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/fitting_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4508 2023-03-15 23:05:25.000000 xGPR-0.1.2.3/xGPR/fitting_toolkit/ams_grad_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5010 2023-03-15 23:05:25.000000 xGPR-0.1.2.3/xGPR/fitting_toolkit/cg_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2523 2023-06-06 02:24:40.000000 xGPR-0.1.2.3/xGPR/fitting_toolkit/exact_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5306 2023-03-15 23:05:25.000000 xGPR-0.1.2.3/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8382 2023-03-15 23:05:25.000000 xGPR-0.1.2.3/xGPR/fitting_toolkit/sgd_fitting_toolkit.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.015565 xGPR-0.1.2.3/xGPR/kernels/
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.015565 xGPR-0.1.2.3/xGPR/kernels/ARD_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:25.000000 xGPR-0.1.2.3/xGPR/kernels/ARD_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13201 2023-06-19 15:11:57.000000 xGPR-0.1.2.3/xGPR/kernels/ARD_kernels/mini_ard.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      854 2023-06-16 16:46:38.000000 xGPR-0.1.2.3/xGPR/kernels/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.015565 xGPR-0.1.2.3/xGPR/kernels/basic_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/kernels/basic_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3507 2023-06-19 13:59:18.000000 xGPR-0.1.2.3/xGPR/kernels/basic_kernels/linear.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3206 2023-06-19 14:13:44.000000 xGPR-0.1.2.3/xGPR/kernels/basic_kernels/matern.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7009 2023-06-19 14:10:03.000000 xGPR-0.1.2.3/xGPR/kernels/basic_kernels/polynomial.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1951 2023-06-19 14:14:22.000000 xGPR-0.1.2.3/xGPR/kernels/basic_kernels/rbf.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11293 2023-06-19 15:12:56.000000 xGPR-0.1.2.3/xGPR/kernels/basic_kernels/rbf_linear.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8197 2023-06-19 15:13:21.000000 xGPR-0.1.2.3/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.015565 xGPR-0.1.2.3/xGPR/kernels/convolution_kernels/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/kernels/convolution_kernels/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8097 2023-06-17 22:46:55.000000 xGPR-0.1.2.3/xGPR/kernels/convolution_kernels/conv_feature_extractor.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10417 2023-06-19 15:13:46.000000 xGPR-0.1.2.3/xGPR/kernels/convolution_kernels/fht_conv1d.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7727 2023-06-19 15:14:09.000000 xGPR-0.1.2.3/xGPR/kernels/convolution_kernels/graph_arccos.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7287 2023-06-19 15:14:30.000000 xGPR-0.1.2.3/xGPR/kernels/convolution_kernels/graph_polysum.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7806 2023-06-19 15:16:23.000000 xGPR-0.1.2.3/xGPR/kernels/convolution_kernels/graph_rbf.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15507 2023-06-19 13:53:19.000000 xGPR-0.1.2.3/xGPR/kernels/kernel_baseclass.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6161 2023-05-25 01:08:01.000000 xGPR-0.1.2.3/xGPR/kernels/srht_compressor.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.015565 xGPR-0.1.2.3/xGPR/optimizers/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/optimizers/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10466 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/optimizers/bayes_grid_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3758 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/optimizers/crude_grid_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9640 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/optimizers/lb_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10478 2023-03-15 23:05:26.000000 xGPR-0.1.2.3/xGPR/optimizers/map_loss_bayes_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6649 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/optimizers/pure_bayes_optimizer.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.015565 xGPR-0.1.2.3/xGPR/preconditioners/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/preconditioners/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3902 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/preconditioners/cuda_rand_nys_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4647 2023-04-04 20:36:21.000000 xGPR-0.1.2.3/xGPR/preconditioners/inter_device_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14555 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/preconditioners/rand_nys_constructors.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3771 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/preconditioners/rand_nys_preconditioners.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4172 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/preconditioners/tuning_preconditioners.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.019565 xGPR-0.1.2.3/xGPR/random_feature_generation/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.019565 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.019565 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:46.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10516 2023-05-24 23:41:15.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1129 2023-05-24 23:00:09.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.019565 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:51.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10097 2023-05-25 14:51:51.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1195 2023-05-25 14:51:46.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4641 2023-05-25 14:51:48.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      477 2023-05-24 23:53:45.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    16445 2023-05-25 00:56:25.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1706 2023-05-25 00:56:23.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9824 2023-05-24 23:22:38.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    21805 2023-06-20 23:27:23.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12508 2023-06-19 14:41:23.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15398 2023-06-20 23:28:13.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      405 2023-05-24 23:56:48.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/cpu_rf_gen_module.pyx
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.019565 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:55.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    19216 2023-05-26 21:59:31.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2421 2023-05-24 22:21:14.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.019565 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:58.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    18137 2023-05-24 19:32:29.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1233 2023-05-24 19:21:47.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.019565 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/__init__.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.019565 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:06.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    17849 2023-05-24 17:21:51.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      581 2023-05-24 16:37:40.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4617 2023-05-24 13:45:05.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.019565 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:09.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7777 2023-05-25 15:07:21.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      491 2023-05-25 14:26:23.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5232 2023-05-24 15:25:35.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      698 2023-03-15 23:05:26.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3822 2023-05-24 17:21:33.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      259 2023-05-24 17:13:48.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11910 2023-05-24 17:59:42.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      742 2023-05-24 17:16:21.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6668 2023-05-24 16:38:48.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    23784 2023-06-20 23:29:00.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13335 2023-05-24 17:38:41.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15776 2023-06-20 23:30:00.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      410 2023-05-24 16:48:30.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/cuda_rf_gen_module.pyx
--rwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)      851 2023-05-25 15:21:39.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.019565 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:12.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12951 2023-05-24 17:22:09.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      895 2023-05-24 15:49:29.000000 xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    28012 2023-06-27 17:43:09.000000 xGPR-0.1.2.3/xGPR/regression_baseclass.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.019565 xGPR-0.1.2.3/xGPR/scoring_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.3/xGPR/scoring_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2944 2023-03-15 23:05:26.000000 xGPR-0.1.2.3/xGPR/scoring_toolkit/approximate_nmll_calcs.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3696 2023-03-15 23:05:26.000000 xGPR-0.1.2.3/xGPR/scoring_toolkit/cho_solvers.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5907 2023-06-20 17:26:24.000000 xGPR-0.1.2.3/xGPR/scoring_toolkit/exact_nmll_calcs.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6888 2023-03-15 23:05:26.000000 xGPR-0.1.2.3/xGPR/scoring_toolkit/nmll_gradient_tools.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3442 2023-03-15 23:05:26.000000 xGPR-0.1.2.3/xGPR/scoring_toolkit/probe_generators.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.019565 xGPR-0.1.2.3/xGPR/static_layers/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/static_layers/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9524 2023-06-17 22:48:21.000000 xGPR-0.1.2.3/xGPR/static_layers/fast_conv.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.023565 xGPR-0.1.2.3/xGPR/tuning_toolkit/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/tuning_toolkit/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8368 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4693 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/tuning_toolkit/direct_fitting_optimizer.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8221 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/tuning_toolkit/hparam_scoring.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.023565 xGPR-0.1.2.3/xGPR/visualization_tools/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:35:56.000000 xGPR-0.1.2.3/xGPR/visualization_tools/__init__.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7246 2023-02-19 16:15:17.000000 xGPR-0.1.2.3/xGPR/visualization_tools/kernel_xpca.py
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    54270 2023-06-16 17:55:48.000000 xGPR-0.1.2.3/xGPR/xGP_Regression.py
-drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-06-27 18:22:59.015565 xGPR-0.1.2.3/xGPR.egg-info/
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-06-27 18:22:58.000000 xGPR-0.1.2.3/xGPR.egg-info/PKG-INFO
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6971 2023-06-27 18:22:58.000000 xGPR-0.1.2.3/xGPR.egg-info/SOURCES.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        1 2023-06-27 18:22:58.000000 xGPR-0.1.2.3/xGPR.egg-info/dependency_links.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-06-27 18:22:58.000000 xGPR-0.1.2.3/xGPR.egg-info/requires.txt
--rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       39 2023-06-27 18:22:58.000000 xGPR-0.1.2.3/xGPR.egg-info/top_level.txt
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.640200 xGPR-0.1.2.4/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1067 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/LICENSE
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-07-17 22:45:31.640200 xGPR-0.1.2.4/PKG-INFO
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1449 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/README.md
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       78 2023-06-21 00:02:39.000000 xGPR-0.1.2.4/pyproject.toml
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-07-17 22:45:31.640200 xGPR-0.1.2.4/setup.cfg
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8142 2023-05-25 13:16:01.000000 xGPR-0.1.2.4/setup.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.372206 xGPR-0.1.2.4/xGPR/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      105 2023-07-17 22:42:25.000000 xGPR-0.1.2.4/xGPR/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.388205 xGPR-0.1.2.4/xGPR/cg_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/cg_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2180 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/cg_toolkit/cg_linear_operators.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11182 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/cg_toolkit/cg_tools.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3515 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/cg_toolkit/cuda_cg_linear_operators.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.388205 xGPR-0.1.2.4/xGPR/constants/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/constants/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      533 2023-03-15 23:05:25.000000 xGPR-0.1.2.4/xGPR/constants/constants.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.400205 xGPR-0.1.2.4/xGPR/data_handling/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/data_handling/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4337 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/data_handling/data_handling_baseclass.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13173 2023-07-17 22:27:06.000000 xGPR-0.1.2.4/xGPR/data_handling/dataset_builder.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2233 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/data_handling/minibatch_data_handler.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8618 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/data_handling/offline_data_handling.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6843 2023-06-07 22:48:32.000000 xGPR-0.1.2.4/xGPR/data_handling/online_data_handling.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.432204 xGPR-0.1.2.4/xGPR/fitting_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/fitting_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4508 2023-03-15 23:05:25.000000 xGPR-0.1.2.4/xGPR/fitting_toolkit/ams_grad_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5010 2023-03-15 23:05:25.000000 xGPR-0.1.2.4/xGPR/fitting_toolkit/cg_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2523 2023-06-06 02:24:40.000000 xGPR-0.1.2.4/xGPR/fitting_toolkit/exact_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5306 2023-03-15 23:05:25.000000 xGPR-0.1.2.4/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8382 2023-03-15 23:05:25.000000 xGPR-0.1.2.4/xGPR/fitting_toolkit/sgd_fitting_toolkit.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.452204 xGPR-0.1.2.4/xGPR/kernels/
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.468204 xGPR-0.1.2.4/xGPR/kernels/ARD_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:25.000000 xGPR-0.1.2.4/xGPR/kernels/ARD_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13201 2023-06-19 15:11:57.000000 xGPR-0.1.2.4/xGPR/kernels/ARD_kernels/mini_ard.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      854 2023-06-16 16:46:38.000000 xGPR-0.1.2.4/xGPR/kernels/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.516203 xGPR-0.1.2.4/xGPR/kernels/basic_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/kernels/basic_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3507 2023-06-19 13:59:18.000000 xGPR-0.1.2.4/xGPR/kernels/basic_kernels/linear.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3206 2023-06-19 14:13:44.000000 xGPR-0.1.2.4/xGPR/kernels/basic_kernels/matern.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7009 2023-06-19 14:10:03.000000 xGPR-0.1.2.4/xGPR/kernels/basic_kernels/polynomial.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1951 2023-06-19 14:14:22.000000 xGPR-0.1.2.4/xGPR/kernels/basic_kernels/rbf.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11293 2023-06-19 15:12:56.000000 xGPR-0.1.2.4/xGPR/kernels/basic_kernels/rbf_linear.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8197 2023-06-19 15:13:21.000000 xGPR-0.1.2.4/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.544202 xGPR-0.1.2.4/xGPR/kernels/convolution_kernels/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/kernels/convolution_kernels/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8097 2023-06-17 22:46:55.000000 xGPR-0.1.2.4/xGPR/kernels/convolution_kernels/conv_feature_extractor.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10642 2023-07-17 22:36:07.000000 xGPR-0.1.2.4/xGPR/kernels/convolution_kernels/fht_conv1d.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7727 2023-06-19 15:14:09.000000 xGPR-0.1.2.4/xGPR/kernels/convolution_kernels/graph_arccos.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7287 2023-06-19 15:14:30.000000 xGPR-0.1.2.4/xGPR/kernels/convolution_kernels/graph_polysum.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7806 2023-06-19 15:16:23.000000 xGPR-0.1.2.4/xGPR/kernels/convolution_kernels/graph_rbf.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15507 2023-06-19 13:53:19.000000 xGPR-0.1.2.4/xGPR/kernels/kernel_baseclass.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6161 2023-05-25 01:08:01.000000 xGPR-0.1.2.4/xGPR/kernels/srht_compressor.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.572201 xGPR-0.1.2.4/xGPR/optimizers/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/optimizers/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10466 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/optimizers/bayes_grid_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3758 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/optimizers/crude_grid_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9640 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/optimizers/lb_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10478 2023-03-15 23:05:26.000000 xGPR-0.1.2.4/xGPR/optimizers/map_loss_bayes_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6649 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/optimizers/pure_bayes_optimizer.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.596201 xGPR-0.1.2.4/xGPR/preconditioners/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/preconditioners/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3902 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/preconditioners/cuda_rand_nys_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4647 2023-04-04 20:36:21.000000 xGPR-0.1.2.4/xGPR/preconditioners/inter_device_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    14555 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/preconditioners/rand_nys_constructors.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3771 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/preconditioners/rand_nys_preconditioners.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4172 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/preconditioners/tuning_preconditioners.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.596201 xGPR-0.1.2.4/xGPR/random_feature_generation/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.600201 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.600201 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:46.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10516 2023-05-24 23:41:15.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1129 2023-05-24 23:00:09.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.604201 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:51.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    10097 2023-05-25 14:51:51.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1195 2023-05-25 14:51:46.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4641 2023-05-25 14:51:48.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      477 2023-05-24 23:53:45.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    16445 2023-05-25 00:56:25.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1706 2023-05-25 00:56:23.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9824 2023-05-24 23:22:38.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    21805 2023-06-20 23:27:23.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12508 2023-06-19 14:41:23.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15398 2023-06-20 23:28:13.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      405 2023-05-24 23:56:48.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/cpu_rf_gen_module.pyx
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.604201 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:55.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    19216 2023-05-26 21:59:31.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2421 2023-05-24 22:21:14.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.604201 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:27:58.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    18137 2023-05-24 19:32:29.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1233 2023-05-24 19:21:47.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.608201 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/__init__.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.608201 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:06.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    17849 2023-05-24 17:21:51.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      581 2023-05-24 16:37:40.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4617 2023-05-24 13:45:05.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.612201 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:09.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7777 2023-05-25 15:07:21.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      491 2023-05-25 14:26:23.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5232 2023-05-24 15:25:35.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      698 2023-03-15 23:05:26.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3822 2023-05-24 17:21:33.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      259 2023-05-24 17:13:48.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    11910 2023-05-24 17:59:42.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      742 2023-05-24 17:16:21.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6668 2023-05-24 16:38:48.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    23784 2023-06-20 23:29:00.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    13335 2023-05-24 17:38:41.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    15776 2023-06-20 23:30:00.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      410 2023-05-24 16:48:30.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/cuda_rf_gen_module.pyx
+-rwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)      851 2023-05-25 15:21:39.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.612201 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:28:12.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    12951 2023-05-24 17:22:09.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)      895 2023-05-24 15:49:29.000000 xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    28012 2023-06-27 17:43:09.000000 xGPR-0.1.2.4/xGPR/regression_baseclass.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.624200 xGPR-0.1.2.4/xGPR/scoring_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-03-15 23:05:26.000000 xGPR-0.1.2.4/xGPR/scoring_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     2944 2023-03-15 23:05:26.000000 xGPR-0.1.2.4/xGPR/scoring_toolkit/approximate_nmll_calcs.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3696 2023-03-15 23:05:26.000000 xGPR-0.1.2.4/xGPR/scoring_toolkit/cho_solvers.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     5907 2023-06-20 17:26:24.000000 xGPR-0.1.2.4/xGPR/scoring_toolkit/exact_nmll_calcs.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6888 2023-03-15 23:05:26.000000 xGPR-0.1.2.4/xGPR/scoring_toolkit/nmll_gradient_tools.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     3442 2023-03-15 23:05:26.000000 xGPR-0.1.2.4/xGPR/scoring_toolkit/probe_generators.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.624200 xGPR-0.1.2.4/xGPR/static_layers/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/static_layers/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     9524 2023-06-17 22:48:21.000000 xGPR-0.1.2.4/xGPR/static_layers/fast_conv.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.640200 xGPR-0.1.2.4/xGPR/tuning_toolkit/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/tuning_toolkit/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8368 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     4693 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/tuning_toolkit/direct_fitting_optimizer.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     8221 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/tuning_toolkit/hparam_scoring.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.640200 xGPR-0.1.2.4/xGPR/visualization_tools/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-04-14 20:35:56.000000 xGPR-0.1.2.4/xGPR/visualization_tools/__init__.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     7246 2023-02-19 16:15:17.000000 xGPR-0.1.2.4/xGPR/visualization_tools/kernel_xpca.py
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)    54270 2023-06-16 17:55:48.000000 xGPR-0.1.2.4/xGPR/xGP_Regression.py
+drwxrwxr-x   0 jlparkinson1  (1000) jlparkinson1  (1000)        0 2023-07-17 22:45:31.372206 xGPR-0.1.2.4/xGPR.egg-info/
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     1736 2023-07-17 22:45:31.000000 xGPR-0.1.2.4/xGPR.egg-info/PKG-INFO
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)     6971 2023-07-17 22:45:31.000000 xGPR-0.1.2.4/xGPR.egg-info/SOURCES.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)        1 2023-07-17 22:45:31.000000 xGPR-0.1.2.4/xGPR.egg-info/dependency_links.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       38 2023-07-17 22:45:31.000000 xGPR-0.1.2.4/xGPR.egg-info/requires.txt
+-rw-rw-r--   0 jlparkinson1  (1000) jlparkinson1  (1000)       39 2023-07-17 22:45:31.000000 xGPR-0.1.2.4/xGPR.egg-info/top_level.txt
```

### Comparing `xGPR-0.1.2.3/LICENSE` & `xGPR-0.1.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/PKG-INFO` & `xGPR-0.1.2.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xGPR
-Version: 0.1.2.3
+Version: 0.1.2.4
 Summary: Fast approximate Gaussian process regression
 Home-page: UNKNOWN
 Author: Jonathan Parkinson
 Author-email: jlparkinson1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xGPR-0.1.2.3/README.md` & `xGPR-0.1.2.4/README.md`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/setup.py` & `xGPR-0.1.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/cg_toolkit/cg_linear_operators.py` & `xGPR-0.1.2.4/xGPR/cg_toolkit/cg_linear_operators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/cg_toolkit/cg_tools.pyx` & `xGPR-0.1.2.4/xGPR/cg_toolkit/cg_tools.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/cg_toolkit/cuda_cg_linear_operators.py` & `xGPR-0.1.2.4/xGPR/cg_toolkit/cuda_cg_linear_operators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/constants/constants.py` & `xGPR-0.1.2.4/xGPR/constants/constants.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/data_handling/data_handling_baseclass.py` & `xGPR-0.1.2.4/xGPR/data_handling/data_handling_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/data_handling/dataset_builder.py` & `xGPR-0.1.2.4/xGPR/data_handling/dataset_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         raise ValueError("X and y must be numpy arrays!")
     if len(ydata.shape) != 1:
         raise ValueError("Y must be a 1d numpy array.")
     if xdata.dtype != "float64" or ydata.dtype != "float64":
         raise ValueError("Both x and y must be arrays of datatype np.float64.")
     if ydata.shape[0] != xdata.shape[0]:
         raise ValueError("Different number of datapoints in x and y.")
-    if np.sum(np.isnan(xdata)) > 0:
+    if np.isnan(xdata).any():
         raise ValueError("One or more elements in x is nan!")
     if np.max(xdata) > 1e15 or np.min(xdata) < -1e15:
         raise ValueError("Values > 1e15 or < -1e15 encountered. "
                     "Please rescale your data and check for np.inf.")
 
     dataset = OnlineDataset(xdata, ydata, chunk_size = chunk_size,
             normalize_y = normalize_y)
@@ -100,15 +100,15 @@
         raise ValueError("At least one datafile must be supplied.")
     xdim = [0,-1]
     if not skip_safety_checks:
         for xfile, yfile in zip(xlist, ylist):
             x_data = np.load(xfile)
             if x_data.shape[0] == 0:
                 raise ValueError(f"File {xfile} has no datapoints.")
-            if np.sum(np.isnan(x_data)) > 0:
+            if np.isnan(x_data).any():
                 raise ValueError(f"One or more elements in file {xfile} is nan.")
             if np.max(x_data) > 1e15 or np.min(x_data) < -1e15:
                 raise ValueError(f"One or more values in {xfile} is "
                         "> 1e15 or < -1e15. Please check for inf values "
                         "and / or rescale your data.")
             xdim[0] += x_data.shape[0]
             if xdim[1] == -1:
@@ -195,15 +195,15 @@
         raise ValueError("At least one datafile must be supplied.")
     xdim = [0,-1,-1]
     if not skip_safety_checks:
         for xfile, yfile in zip(xlist, ylist):
             x_data = np.load(xfile)
             if x_data.shape[0] == 0:
                 raise ValueError(f"File {xfile} has no datapoints.")
-            if np.sum(np.isnan(x_data)) > 0:
+            if np.isnan(x_data).any():
                 raise ValueError(f"One or more elements in file {xfile} is nan.")
             if np.max(x_data) > 1e15 or np.min(x_data) < -1e15:
                 raise ValueError(f"One or more values in {xfile} is "
                     "> 1e15 or < -1e15. Please check for inf values "
                     "and / or rescale your data.")
             xdim[0] += x_data.shape[0]
             yshape = _get_array_file_shape(yfile)
```

### Comparing `xGPR-0.1.2.3/xGPR/data_handling/minibatch_data_handler.py` & `xGPR-0.1.2.4/xGPR/data_handling/minibatch_data_handler.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/data_handling/offline_data_handling.py` & `xGPR-0.1.2.4/xGPR/data_handling/offline_data_handling.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/data_handling/online_data_handling.py` & `xGPR-0.1.2.4/xGPR/data_handling/online_data_handling.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/fitting_toolkit/ams_grad_toolkit.py` & `xGPR-0.1.2.4/xGPR/fitting_toolkit/ams_grad_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/fitting_toolkit/cg_fitting_toolkit.py` & `xGPR-0.1.2.4/xGPR/fitting_toolkit/cg_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/fitting_toolkit/exact_fitting_toolkit.py` & `xGPR-0.1.2.4/xGPR/fitting_toolkit/exact_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py` & `xGPR-0.1.2.4/xGPR/fitting_toolkit/lbfgs_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/fitting_toolkit/sgd_fitting_toolkit.py` & `xGPR-0.1.2.4/xGPR/fitting_toolkit/sgd_fitting_toolkit.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/kernels/ARD_kernels/mini_ard.py` & `xGPR-0.1.2.4/xGPR/kernels/ARD_kernels/mini_ard.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/kernels/__init__.py` & `xGPR-0.1.2.4/xGPR/kernels/__init__.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/kernels/basic_kernels/linear.py` & `xGPR-0.1.2.4/xGPR/kernels/basic_kernels/linear.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/kernels/basic_kernels/matern.py` & `xGPR-0.1.2.4/xGPR/kernels/basic_kernels/matern.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/kernels/basic_kernels/polynomial.py` & `xGPR-0.1.2.4/xGPR/kernels/basic_kernels/polynomial.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/kernels/basic_kernels/rbf.py` & `xGPR-0.1.2.4/xGPR/kernels/basic_kernels/rbf.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/kernels/basic_kernels/rbf_linear.py` & `xGPR-0.1.2.4/xGPR/kernels/basic_kernels/rbf_linear.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py` & `xGPR-0.1.2.4/xGPR/kernels/basic_kernels/sorf_kernel_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/kernels/convolution_kernels/conv_feature_extractor.py` & `xGPR-0.1.2.4/xGPR/kernels/convolution_kernels/conv_feature_extractor.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/kernels/convolution_kernels/fht_conv1d.py` & `xGPR-0.1.2.4/xGPR/kernels/convolution_kernels/fht_conv1d.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,17 +23,14 @@
     Attributes:
         hyperparams (np.ndarray): This kernel has three
             hyperparameters: lambda_ (noise), beta_ (amplitude)
             and sigma (inverse mismatch tolerance).
         conv_width (int): The width of the convolution kernel.
             This hyperparameter can be set based on experimentation
             or domain knowledge. Defaults to 9.
-        num_slides (int): The length of the (zero-padded) input data
-            minus conv_width + 1. The number of points that will
-            result from the convolution.
         dim2_no_padding (int): The size of the expected input data
             once reshaped for convolution, before zero padding.
         padded_dims (int): The size of the expected input data
             once reshaped for convolution, after zero-padding to
             be a power of 2.
         init_calc_freqsize (int): The number of times the transform
             will need to be performed to generate the requested number
@@ -91,15 +88,14 @@
         self.hyperparams = np.ones((3))
         rng = np.random.default_rng(random_seed)
         self.conv_width = kernel_spec_parms["conv_width"]
         if self.conv_width >= xdim[1]:
             raise ValueError("The conv_width for the convolution kernels must be "
                     "< the length of the time series / sequence.")
 
-        self.num_slides = xdim[1] - self.conv_width + 1
         self.dim2_no_padding = self.conv_width * xdim[2]
         self.padded_dims = 2**ceil(np.log2(max(self.dim2_no_padding, 2)))
         self.init_calc_freqsize = ceil(self.num_freqs / self.padded_dims) * \
                         self.padded_dims
         self.init_calc_featsize = 2 * self.init_calc_freqsize
         self.bounds = np.asarray([[1e-3,1e1], [0.2, 5], [1e-2, 1e2]])
 
@@ -151,24 +147,31 @@
         Returns:
             xtrans: A cupy or numpy array containing the generated features.
 
         Raises:
             ValueError: A value error is raised if the dimensionality of the
                 input does not meet validity criteria.
         """
+        #Because we are using stride_tricks, we need to run some additional
+        #checks on the input before doing anything else.
         if input_x.shape[1] <= self.conv_width:
             raise ValueError("Input X must have shape[1] >= the convolution "
                     "kernel width.")
         if len(input_x.shape) != 3:
             raise ValueError("Input X must be a 3d array.")
+        if input_x.shape[2] != self.xdim[2]:
+            raise ValueError("Unexpected input shape supplied.")
+
         xtrans = self.zero_arr((input_x.shape[0], self.num_rffs), self.out_type)
-        reshaped_x = self.zero_arr((input_x.shape[0], self.num_slides,
+
+        num_slides = input_x.shape[1] - self.conv_width + 1
+        reshaped_x = self.zero_arr((input_x.shape[0], num_slides,
                                 self.padded_dims), self.dtype)
         x_strided = self.stride_tricks(input_x, shape=(input_x.shape[0],
-                            self.num_slides, self.dim2_no_padding),
+                            num_slides, self.dim2_no_padding),
                             strides=(input_x.strides[0], input_x.shape[2] * input_x.strides[2],
                                 input_x.strides[2]))
         reshaped_x[:,:,:self.dim2_no_padding] = x_strided * self.hyperparams[2]
         self.conv_func(reshaped_x, self.radem_diag, xtrans, self.chi_arr, self.num_threads,
                 self.hyperparams[1], self.fit_intercept)
         return xtrans
 
@@ -197,19 +200,23 @@
                 output_x with respect to the kernel-specific hyperparameters.
         """
         if input_x.shape[1] <= self.conv_width:
             raise ValueError("Input X must have shape[1] >= the convolution "
                     "kernel width.")
         if len(input_x.shape) != 3:
             raise ValueError("Input X must be a 3d array.")
+        if input_x.shape[2] != self.xdim[2]:
+            raise ValueError("Unexpected input shape supplied.")
+
         output_x = self.zero_arr((input_x.shape[0], self.init_calc_featsize), self.out_type)
-        reshaped_x = self.zero_arr((input_x.shape[0], self.num_slides,
+        num_slides = input_x.shape[1] - self.conv_width + 1
+        reshaped_x = self.zero_arr((input_x.shape[0], num_slides,
                                 self.padded_dims), self.dtype)
         x_strided = self.stride_tricks(input_x, shape=(input_x.shape[0],
-                            self.num_slides, self.dim2_no_padding),
+                            num_slides, self.dim2_no_padding),
                             strides=(input_x.strides[0], input_x.shape[2] *
                                 input_x.strides[2], input_x.strides[2]))
         reshaped_x[:,:,:self.dim2_no_padding] = x_strided
         dz_dsigma = self.grad_func(reshaped_x, self.radem_diag,
                 output_x, self.chi_arr, self.num_threads, self.hyperparams[2],
                 self.hyperparams[1], self.fit_intercept)
```

### Comparing `xGPR-0.1.2.3/xGPR/kernels/convolution_kernels/graph_arccos.py` & `xGPR-0.1.2.4/xGPR/kernels/convolution_kernels/graph_arccos.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/kernels/convolution_kernels/graph_polysum.py` & `xGPR-0.1.2.4/xGPR/kernels/convolution_kernels/graph_polysum.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/kernels/convolution_kernels/graph_rbf.py` & `xGPR-0.1.2.4/xGPR/kernels/convolution_kernels/graph_rbf.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/kernels/kernel_baseclass.py` & `xGPR-0.1.2.4/xGPR/kernels/kernel_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/kernels/srht_compressor.py` & `xGPR-0.1.2.4/xGPR/kernels/srht_compressor.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/optimizers/bayes_grid_optimizer.py` & `xGPR-0.1.2.4/xGPR/optimizers/bayes_grid_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/optimizers/crude_grid_optimizer.py` & `xGPR-0.1.2.4/xGPR/optimizers/crude_grid_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/optimizers/lb_optimizer.py` & `xGPR-0.1.2.4/xGPR/optimizers/lb_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/optimizers/map_loss_bayes_optimizer.py` & `xGPR-0.1.2.4/xGPR/optimizers/map_loss_bayes_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/optimizers/pure_bayes_optimizer.py` & `xGPR-0.1.2.4/xGPR/optimizers/pure_bayes_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/preconditioners/cuda_rand_nys_preconditioners.py` & `xGPR-0.1.2.4/xGPR/preconditioners/cuda_rand_nys_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/preconditioners/inter_device_preconditioners.py` & `xGPR-0.1.2.4/xGPR/preconditioners/inter_device_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/preconditioners/rand_nys_constructors.py` & `xGPR-0.1.2.4/xGPR/preconditioners/rand_nys_constructors.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/preconditioners/rand_nys_preconditioners.py` & `xGPR-0.1.2.4/xGPR/preconditioners/rand_nys_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/preconditioners/tuning_preconditioners.py` & `xGPR-0.1.2.4/xGPR/preconditioners/tuning_preconditioners.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp` & `xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h` & `xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/basic_ops/transform_functions.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp` & `xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h` & `xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/arccos_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp` & `xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/conv1d_operations.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp` & `xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h` & `xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/convolution_ops/rbf_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx` & `xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/cpu_basic_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx` & `xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/cpu_convolution.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx` & `xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/cpu_polynomial.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx` & `xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/cpu_rbf_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp` & `xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h` & `xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/rbf_ops/rbf_ops.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp` & `xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.cpp`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h` & `xGPR-0.1.2.4/xGPR/random_feature_generation/cpu_rf_gen/shared_fht_functions/basic_array_operations.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/basic_array_operations.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/basic_ops/sharedmem.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/arccos_convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/ard_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/convolution_ops/rbf_convolution.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/cuda_basic_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/cuda_convolution.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/cuda_polynomial.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/cuda_rbf_operations.pyx`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/nvcc_compile.sh`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.cu`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h` & `xGPR-0.1.2.4/xGPR/random_feature_generation/gpu_rf_gen/rbf_ops/rbf_ops.h`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/regression_baseclass.py` & `xGPR-0.1.2.4/xGPR/regression_baseclass.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/scoring_toolkit/approximate_nmll_calcs.py` & `xGPR-0.1.2.4/xGPR/scoring_toolkit/approximate_nmll_calcs.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/scoring_toolkit/cho_solvers.py` & `xGPR-0.1.2.4/xGPR/scoring_toolkit/cho_solvers.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/scoring_toolkit/exact_nmll_calcs.py` & `xGPR-0.1.2.4/xGPR/scoring_toolkit/exact_nmll_calcs.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/scoring_toolkit/nmll_gradient_tools.py` & `xGPR-0.1.2.4/xGPR/scoring_toolkit/nmll_gradient_tools.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/scoring_toolkit/probe_generators.py` & `xGPR-0.1.2.4/xGPR/scoring_toolkit/probe_generators.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/static_layers/fast_conv.py` & `xGPR-0.1.2.4/xGPR/static_layers/fast_conv.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py` & `xGPR-0.1.2.4/xGPR/tuning_toolkit/bayesian_fitting_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/tuning_toolkit/direct_fitting_optimizer.py` & `xGPR-0.1.2.4/xGPR/tuning_toolkit/direct_fitting_optimizer.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/tuning_toolkit/hparam_scoring.py` & `xGPR-0.1.2.4/xGPR/tuning_toolkit/hparam_scoring.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/visualization_tools/kernel_xpca.py` & `xGPR-0.1.2.4/xGPR/visualization_tools/kernel_xpca.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR/xGP_Regression.py` & `xGPR-0.1.2.4/xGPR/xGP_Regression.py`

 * *Files identical despite different names*

### Comparing `xGPR-0.1.2.3/xGPR.egg-info/PKG-INFO` & `xGPR-0.1.2.4/xGPR.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xGPR
-Version: 0.1.2.3
+Version: 0.1.2.4
 Summary: Fast approximate Gaussian process regression
 Home-page: UNKNOWN
 Author: Jonathan Parkinson
 Author-email: jlparkinson1@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `xGPR-0.1.2.3/xGPR.egg-info/SOURCES.txt` & `xGPR-0.1.2.4/xGPR.egg-info/SOURCES.txt`

 * *Files identical despite different names*

