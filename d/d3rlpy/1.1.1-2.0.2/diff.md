# Comparing `tmp/d3rlpy-1.1.1.tar.gz` & `tmp/d3rlpy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/d3rlpy-1.1.1.tar", last modified: Fri Jun 24 11:15:47 2022, max compression
+gzip compressed data, was "d3rlpy-2.0.2.tar", last modified: Tue Jul 18 07:06:09 2023, max compression
```

## Comparing `d3rlpy-1.1.1.tar` & `d3rlpy-2.0.2.tar`

### file list

```diff
@@ -1,142 +1,138 @@
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      125 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/MANIFEST.in
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    13073 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/PKG-INFO
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    10164 2022-06-13 02:39:00.000000 d3rlpy-1.1.1/README.md
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      506 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       22 2022-06-24 11:03:36.000000 d3rlpy-1.1.1/d3rlpy/_version.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/algos/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2628 2022-04-10 06:53:01.000000 d3rlpy-1.1.1/d3rlpy/algos/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7536 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/awac.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    14072 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     8157 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/bc.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    17081 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/bcq.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12914 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/bear.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    10503 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/combo.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    14874 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/cql.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     9302 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/crr.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6885 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/ddpg.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7378 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/dqn.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7632 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/iql.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    10930 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/mopo.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4764 2022-04-10 06:54:31.000000 d3rlpy-1.1.1/d3rlpy/algos/nfq.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    14924 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/plas.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4032 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/random_policy.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    15636 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/sac.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     8015 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/td3.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7538 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/td3_plus_bc.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      478 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5290 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/awac_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7011 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7052 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/bc_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    11664 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/bcq_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    11605 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/bear_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3889 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/combo_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    10892 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/cql_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7085 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/crr_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     8191 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/ddpg_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5267 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/dqn_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5722 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/iql_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    10876 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/plas_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    14218 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/sac_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2858 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/td3_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2452 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/td3_plus_bc_impl.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2311 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/torch/utility.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3245 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/algos/utility.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3355 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/argument_utility.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    31916 2022-04-10 08:28:19.000000 d3rlpy-1.1.1/d3rlpy/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    10181 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/cli.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1225 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/constants.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1882 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/containers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      456 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/context.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/cpp/
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/cpp/include/
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/cpp/include/d3rlpy/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      465 2022-06-18 02:24:12.000000 d3rlpy-1.1.1/d3rlpy/cpp/include/d3rlpy/dataset.h
--rw-rw-r--   0 takuma    (1000) takuma    (1000)  1778593 2022-06-24 11:14:46.000000 d3rlpy-1.1.1/d3rlpy/dataset.cpp
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      604 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/dataset.pxd
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4542 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/dataset.pyi
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    42298 2022-06-18 02:10:08.000000 d3rlpy-1.1.1/d3rlpy/dataset.pyx
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    10968 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/datasets.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      677 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/decorators.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/dynamics/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      167 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/dynamics/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2218 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/dynamics/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5147 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/dynamics/probabilistic_ensemble_dynamics.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/dynamics/torch/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       93 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/dynamics/torch/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3122 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/dynamics/torch/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3782 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/dynamics/torch/probabilistic_ensemble_dynamics_impl.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/envs/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      114 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/envs/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12439 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/envs/wrappers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      781 2022-06-05 05:02:18.000000 d3rlpy-1.1.1/d3rlpy/gpu.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/iterators/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      192 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/iterators/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3321 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/iterators/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1195 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/iterators/random_iterator.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1437 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/iterators/round_iterator.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      394 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/itertools.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5392 2022-04-10 10:30:29.000000 d3rlpy-1.1.1/d3rlpy/logger.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/metrics/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      952 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/metrics/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3129 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/metrics/comparer.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    17618 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/metrics/scorer.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/models/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       48 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6661 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/builders.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    13752 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/encoders.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4577 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/optimizers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     9844 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/q_functions.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/models/torch/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2390 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/torch/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4185 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/torch/distributions.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     8046 2022-06-13 02:38:39.000000 d3rlpy-1.1.1/d3rlpy/models/torch/dynamics.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    10379 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/torch/encoders.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7351 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/torch/imitators.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      460 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/torch/parameters.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    11100 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/torch/policies.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2911 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     1445 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/base.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     6231 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/ensemble_q_function.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     9458 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/fqf_q_function.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7154 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/iqn_q_function.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3130 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/mean_q_function.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4980 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/qr_q_function.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2360 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/utility.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      831 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/models/torch/v_functions.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/online/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       33 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/online/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    10207 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/online/buffers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     4123 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/online/explorers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    12152 2022-04-10 08:29:50.000000 d3rlpy-1.1.1/d3rlpy/online/iterators.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      261 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/online/utility.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/ope/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       68 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/ope/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     8986 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/ope/fqe.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/ope/torch/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)        0 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/ope/torch/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     5887 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/ope/torch/fqe_impl.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/preprocessing/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)      784 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/preprocessing/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     7620 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/preprocessing/action_scalers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    15290 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/preprocessing/reward_scalers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    11721 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/preprocessing/scalers.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3659 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/preprocessing/stack.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)        0 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/py.typed
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    10397 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/torch_utility.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy/wrappers/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       18 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/wrappers/__init__.py
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     2288 2022-04-10 02:55:43.000000 d3rlpy-1.1.1/d3rlpy/wrappers/sb3.py
-drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy.egg-info/
--rw-rw-r--   0 takuma    (1000) takuma    (1000)    13073 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy.egg-info/PKG-INFO
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3324 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy.egg-info/SOURCES.txt
--rw-rw-r--   0 takuma    (1000) takuma    (1000)        1 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy.egg-info/dependency_links.txt
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       43 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy.egg-info/entry_points.txt
--rw-rw-r--   0 takuma    (1000) takuma    (1000)        1 2022-06-24 11:15:38.000000 d3rlpy-1.1.1/d3rlpy.egg-info/not-zip-safe
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       95 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy.egg-info/requires.txt
--rw-rw-r--   0 takuma    (1000) takuma    (1000)        7 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/d3rlpy.egg-info/top_level.txt
--rw-rw-r--   0 takuma    (1000) takuma    (1000)       38 2022-06-24 11:15:47.000000 d3rlpy-1.1.1/setup.cfg
--rw-rw-r--   0 takuma    (1000) takuma    (1000)     3080 2022-06-05 05:02:32.000000 d3rlpy-1.1.1/setup.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.424370 d3rlpy-2.0.2/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1068 2022-09-11 02:40:22.000000 d3rlpy-2.0.2/LICENSE
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      125 2022-09-11 02:40:22.000000 d3rlpy-2.0.2/MANIFEST.in
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12019 2023-07-18 07:06:09.424370 d3rlpy-2.0.2/PKG-INFO
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9254 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/README.md
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.420370 d3rlpy-2.0.2/d3rlpy/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      496 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       22 2023-07-18 07:05:48.000000 d3rlpy-2.0.2/d3rlpy/_version.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.420370 d3rlpy-2.0.2/d3rlpy/algos/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       75 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/__init__.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.420370 d3rlpy-2.0.2/d3rlpy/algos/qlearning/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      351 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5973 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/awac.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    32009 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/base.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6171 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/bc.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    14962 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/bcq.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    10883 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/bear.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12529 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/cql.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7331 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/crr.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5449 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/ddpg.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6647 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/dqn.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4001 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/explorers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6525 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/iql.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3697 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/nfq.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12022 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/plas.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4336 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/random_policy.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12811 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/sac.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6320 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/td3.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5837 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/td3_plus_bc.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.420370 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      323 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3267 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/awac_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4059 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/bc_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7013 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/bcq_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     8012 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/bear_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     8546 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/cql_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5466 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/crr_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4252 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/ddpg_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3014 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/dqn_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3549 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/iql_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5343 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/plas_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7320 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/sac_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1936 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/td3_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1546 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/td3_plus_bc_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1058 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/utility.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.420370 d3rlpy-2.0.2/d3rlpy/algos/transformer/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       78 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/transformer/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12680 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/transformer/base.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4813 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/transformer/decision_transformer.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4010 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/transformer/inputs.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.420370 d3rlpy-2.0.2/d3rlpy/algos/transformer/torch/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       41 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/transformer/torch/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2222 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/transformer/torch/decision_transformer_impl.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4456 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/algos/utility.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12802 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/base.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9991 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/cli.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1265 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/constants.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.420370 d3rlpy-2.0.2/d3rlpy/dataset/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      310 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/dataset/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3071 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/dataset/buffers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2032 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/dataset/compat.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    11090 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/dataset/components.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2577 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/dataset/episode_generator.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3264 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/dataset/io.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7410 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/dataset/mini_batch.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    15505 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/dataset/replay_buffer.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2941 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/dataset/trajectory_slicers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5413 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/dataset/transition_pickers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      286 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/dataset/types.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7796 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/dataset/utils.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12332 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/dataset/writers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    14906 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/datasets.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.420370 d3rlpy-2.0.2/d3rlpy/envs/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       47 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/envs/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      143 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/envs/utility.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    15039 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/envs/wrappers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1041 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/interface.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      443 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/itertools.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.420370 d3rlpy-2.0.2/d3rlpy/logging/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      134 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/logging/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2650 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/logging/file_adapter.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4169 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/logging/logger.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1050 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/logging/noop_adapter.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2457 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/logging/tensorboard_adapter.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2114 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/logging/utils.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.420370 d3rlpy-2.0.2/d3rlpy/metrics/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       49 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/metrics/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    18066 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/metrics/evaluators.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2965 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/metrics/utility.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.420370 d3rlpy-2.0.2/d3rlpy/models/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      101 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    10171 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/builders.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    10380 2023-07-18 06:51:00.000000 d3rlpy-2.0.2/d3rlpy/models/encoders.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5301 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/optimizers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6626 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/q_functions.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.424370 d3rlpy-2.0.2/d3rlpy/models/torch/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      210 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/torch/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4284 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/torch/distributions.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    11014 2023-07-18 07:05:05.000000 d3rlpy-2.0.2/d3rlpy/models/torch/encoders.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7803 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/torch/imitators.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      484 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/torch/parameters.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    11312 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/torch/policies.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.424370 d3rlpy-2.0.2/d3rlpy/models/torch/q_functions/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      198 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/torch/q_functions/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1574 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/torch/q_functions/base.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9237 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/torch/q_functions/ensemble_q_function.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9520 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/torch/q_functions/fqf_q_function.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     7216 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/torch/q_functions/iqn_q_function.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3194 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/torch/q_functions/mean_q_function.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     5040 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/torch/q_functions/qr_q_function.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     2552 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/torch/q_functions/utility.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12509 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/torch/transformers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      860 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/torch/v_functions.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      443 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/models/utility.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.424370 d3rlpy-2.0.2/d3rlpy/ope/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       19 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/ope/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     8378 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/ope/fqe.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.424370 d3rlpy-2.0.2/d3rlpy/ope/torch/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       24 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/ope/torch/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3436 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/ope/torch/fqe_impl.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.424370 d3rlpy-2.0.2/d3rlpy/preprocessing/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)      115 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/preprocessing/__init__.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     6533 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/preprocessing/action_scalers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3265 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/preprocessing/base.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    13692 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/preprocessing/observation_scalers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    15062 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/preprocessing/reward_scalers.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     4821 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/serializable_config.py
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     9874 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/d3rlpy/torch_utility.py
+drwxrwxr-x   0 takuma    (1000) takuma    (1000)        0 2023-07-18 07:06:09.420370 d3rlpy-2.0.2/d3rlpy.egg-info/
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)    12019 2023-07-18 07:06:09.000000 d3rlpy-2.0.2/d3rlpy.egg-info/PKG-INFO
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     3747 2023-07-18 07:06:09.000000 d3rlpy-2.0.2/d3rlpy.egg-info/SOURCES.txt
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)        1 2023-07-18 07:06:09.000000 d3rlpy-2.0.2/d3rlpy.egg-info/dependency_links.txt
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       43 2023-07-18 07:06:09.000000 d3rlpy-2.0.2/d3rlpy.egg-info/entry_points.txt
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       96 2023-07-18 07:06:09.000000 d3rlpy-2.0.2/d3rlpy.egg-info/requires.txt
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)        7 2023-07-18 07:06:09.000000 d3rlpy-2.0.2/d3rlpy.egg-info/top_level.txt
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)        1 2023-07-18 07:06:08.000000 d3rlpy-2.0.2/d3rlpy.egg-info/zip-safe
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)       38 2023-07-18 07:06:09.424370 d3rlpy-2.0.2/setup.cfg
+-rw-rw-r--   0 takuma    (1000) takuma    (1000)     1825 2023-07-18 06:25:45.000000 d3rlpy-2.0.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `d3rlpy-1.1.1/PKG-INFO` & `d3rlpy-2.0.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d3rlpy
-Version: 1.1.1
+Version: 2.0.2
 Summary: An offline deep reinforcement learning library
 Home-page: https://github.com/takuseno/d3rlpy
 Author: Takuma Seno
 Author-email: takuma.seno@gmail.com
 License: MIT License
 Description: <p align="center"><img align="center" width="300px" src="assets/logo.png"></p>
         
@@ -22,46 +22,44 @@
         
         ```py
         import d3rlpy
         
         dataset, env = d3rlpy.datasets.get_dataset("hopper-medium-v0")
         
         # prepare algorithm
-        sac = d3rlpy.algos.SAC()
+        sac = d3rlpy.algos.SACConfig().create(device="cuda:0")
         
         # train offline
         sac.fit(dataset, n_steps=1000000)
         
         # train online
         sac.fit_online(env, n_steps=1000000)
         
         # ready to control
         actions = sac.predict(x)
         ```
         
         - Documentation: https://d3rlpy.readthedocs.io
         - Paper: https://arxiv.org/abs/2111.03788
         
-        ## key features
+        ## Key features
         
         ### :zap: Most Practical RL Library Ever
         - **offline RL**: d3rlpy supports state-of-the-art offline RL algorithms. Offline RL is extremely powerful when the online interaction is not feasible during training (e.g. robotics, medical).
         - **online RL**: d3rlpy also supports conventional state-of-the-art online training algorithms without any compromising, which means that you can solve any kinds of RL problems only with `d3rlpy`.
-        - **advanced engineering**: d3rlpy is designed to implement the faster and efficient training algorithms. For example, you can train Atari environments with x4 less memory space and as fast as the fastest RL library.
         
         ### :beginner: User-friendly API
         - **zero-knowledge of DL library**: d3rlpy provides many state-of-the-art algorithms through intuitive APIs. You can become a RL engineer even without knowing how to use deep learning libraries.
         - **extensive documentation**: d3rlpy is fully documented and accompanied with tutorials and reproduction scripts of the original papers.
         
         ### :rocket: Beyond State-of-the-art
         - **distributional Q function**: d3rlpy is the first library that supports distributional Q functions in the all algorithms. The distributional Q function is known as the very powerful method to achieve the state-of-the-performance.
-        - **many tweek options**: d3rlpy is also the first to support N-step TD backup and ensemble value functions in the all algorithms, which lead you to the place no one ever reached yet.
         
         
-        ## installation
+        ## Installation
         d3rlpy supports Linux, macOS and Windows.
         
         ### PyPI (recommended)
         [![PyPI version](https://badge.fury.io/py/d3rlpy.svg)](https://badge.fury.io/py/d3rlpy)
         ![PyPI - Downloads](https://img.shields.io/pypi/dm/d3rlpy)
         ```
         $ pip install d3rlpy
@@ -76,15 +74,15 @@
         
         ### Docker
         ![Docker Pulls](https://img.shields.io/docker/pulls/takuseno/d3rlpy)
         ```
         $ docker run -it --gpus all --name d3rlpy takuseno/d3rlpy:latest bash
         ```
         
-        ## supported algorithms
+        ## Supported algorithms
         | algorithm | discrete control | continuous control | offline RL? |
         |:-|:-:|:-:|:-:|
         | Behavior Cloning (supervised learning) | :white_check_mark: | :white_check_mark: | |
         | [Neural Fitted Q Iteration (NFQ)](https://link.springer.com/chapter/10.1007/11564096_32) | :white_check_mark: | :no_entry: | :white_check_mark: |
         | [Deep Q-Network (DQN)](https://www.nature.com/articles/nature14236) | :white_check_mark: | :no_entry: | |
         | [Double DQN](https://arxiv.org/abs/1509.06461) | :white_check_mark: | :no_entry: | |
         | [Deep Deterministic Policy Gradients (DDPG)](https://arxiv.org/abs/1509.02971) | :no_entry: | :white_check_mark: | |
@@ -94,157 +92,141 @@
         | [Bootstrapping Error Accumulation Reduction (BEAR)](https://arxiv.org/abs/1906.00949) | :no_entry: | :white_check_mark: | :white_check_mark: |
         | [Conservative Q-Learning (CQL)](https://arxiv.org/abs/2006.04779) | :white_check_mark: | :white_check_mark: | :white_check_mark: |
         | [Advantage Weighted Actor-Critic (AWAC)](https://arxiv.org/abs/2006.09359) | :no_entry: | :white_check_mark: | :white_check_mark: |
         | [Critic Reguralized Regression (CRR)](https://arxiv.org/abs/2006.15134) | :no_entry: | :white_check_mark: | :white_check_mark: |
         | [Policy in Latent Action Space (PLAS)](https://arxiv.org/abs/2011.07213) | :no_entry: | :white_check_mark: | :white_check_mark: |
         | [TD3+BC](https://arxiv.org/abs/2106.06860) | :no_entry: | :white_check_mark: | :white_check_mark: |
         | [Implicit Q-Learning (IQL)](https://arxiv.org/abs/2110.06169) | :no_entry: | :white_check_mark: | :white_check_mark: |
+        | [Decision Transformer](https://arxiv.org/abs/2106.01345) | :construction: | :white_check_mark: | :white_check_mark: |
         
-        ## supported Q functions
+        ## Supported Q functions
         - [x] standard Q function
         - [x] [Quantile Regression](https://arxiv.org/abs/1710.10044)
         - [x] [Implicit Quantile Network](https://arxiv.org/abs/1806.06923)
         
-        ## experimental features
-        - Model-based Algorithms
-          - [Model-based Offline Policy Optimization (MOPO)](https://arxiv.org/abs/2005.13239)
-          - [Conservative Offline Model-Based Policy Optimization (COMBO)](https://arxiv.org/abs/2102.08363)
-        - Q-functions
-          - [Fully parametrized Quantile Function](https://arxiv.org/abs/1911.02140) (experimental)
-        
-        ## benchmark results
+        ## Benchmark results
         d3rlpy is benchmarked to ensure the implementation quality.
         The benchmark scripts are available [reproductions](https://github.com/takuseno/d3rlpy/tree/master/reproductions) directory.
         The benchmark results are available [d3rlpy-benchmarks](https://github.com/takuseno/d3rlpy-benchmarks) repository.
         
-        ## examples
+        ## Examples
         ### MuJoCo
         <p align="center"><img align="center" width="160px" src="assets/mujoco_hopper.gif"></p>
         
         ```py
         import d3rlpy
         
         # prepare dataset
         dataset, env = d3rlpy.datasets.get_d4rl('hopper-medium-v0')
         
         # prepare algorithm
-        cql = d3rlpy.algos.CQL(use_gpu=True)
+        cql = d3rlpy.algos.CQLConfig().create(device='cuda:0')
         
         # train
         cql.fit(
             dataset,
-            eval_episodes=dataset,
-            n_epochs=100,
-            scorers={
-                'environment': d3rlpy.metrics.evaluate_on_environment(env),
-                'td_error': d3rlpy.metrics.td_error_scorer,
-            },
+            n_steps=100000,
+            evaluators={"environment": d3rlpy.metrics.EnvironmentEvaluator(env)},
         )
         ```
         
         See more datasets at [d4rl](https://github.com/rail-berkeley/d4rl).
         
         ### Atari 2600
         <p align="center"><img align="center" width="160px" src="assets/breakout.gif"></p>
         
         ```py
         import d3rlpy
-        from sklearn.model_selection import train_test_split
-        
-        # prepare dataset
-        dataset, env = d3rlpy.datasets.get_atari('breakout-expert-v0')
         
-        # split dataset
-        train_episodes, test_episodes = train_test_split(dataset, test_size=0.1)
+        # prepare dataset (1% dataset)
+        dataset, env = d3rlpy.datasets.get_atari_transitions(
+            'breakout',
+            fraction=0.01,
+            num_stack=4,
+        )
         
         # prepare algorithm
-        cql = d3rlpy.algos.DiscreteCQL(
-            n_frames=4,
-            q_func_factory='qr',
-            scaler='pixel',
-            use_gpu=True,
-        )
+        cql = d3rlpy.algos.DiscreteCQLConfig(
+            observation_scaler=d3rlpy.preprocessing.PixelObservationScaler(),
+            reward_scaler=d3rlpy.preprocessing.ClipRewardScaler(-1.0, 1.0),
+        ).create(device='cuda:0')
         
         # start training
         cql.fit(
-            train_episodes,
-            eval_episodes=test_episodes,
-            n_epochs=100,
-            scorers={
-                'environment': d3rlpy.metrics.evaluate_on_environment(env),
-                'td_error': d3rlpy.metrics.td_error_scorer,
-            },
+            dataset,
+            n_steps=1000000,
+            evaluators={"environment": d3rlpy.metrics.EnvironmentEvaluator(env, epsilon=0.001)},
         )
         ```
         
         See more Atari datasets at [d4rl-atari](https://github.com/takuseno/d4rl-atari).
         
         
         ### Online Training
         ```py
         import d3rlpy
         import gym
         
         # prepare environment
-        env = gym.make('HopperBulletEnv-v0')
-        eval_env = gym.make('HopperBulletEnv-v0')
+        env = gym.make('Hopper-v3')
+        eval_env = gym.make('Hopper-v3')
         
         # prepare algorithm
-        sac = d3rlpy.algos.SAC(use_gpu=True)
+        sac = d3rlpy.algos.SACConfig().create(device='cuda:0')
         
         # prepare replay buffer
-        buffer = d3rlpy.online.buffers.ReplayBuffer(maxlen=1000000, env=env)
+        buffer = d3rlpy.dataset.create_fifo_replay_buffer(limit=1000000, env=env)
         
         # start training
         sac.fit_online(env, buffer, n_steps=1000000, eval_env=eval_env)
         ```
         
-        ## tutorials
+        ## Tutorials
         Try cartpole examples on Google Colaboratory!
         
         - offline RL tutorial: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/takuseno/d3rlpy/blob/master/tutorials/cartpole.ipynb)
         - online RL tutorial: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/takuseno/d3rlpy/blob/master/tutorials/online.ipynb)
         
         More tutorial documentations are available [here](https://d3rlpy.readthedocs.io/en/stable/tutorials/index.html).
         
-        ## contributions
+        ## Contributions
         Any kind of contribution to d3rlpy would be highly appreciated!
         Please check the [contribution guide](CONTRIBUTING.md).
         
-        The release planning can be checked at [milestones](https://github.com/takuseno/d3rlpy/milestones).
-        
-        ## community
+        ## Community
         | Channel | Link |
         |:-|:-|
-        | Chat | [Gitter](https://gitter.im/d3rlpy/d3rlpy) |
         | Issues | [GitHub Issues](https://github.com/takuseno/d3rlpy/issues) |
         
-        ## family projects
+        ## Family projects
         | Project | Description |
         |:-:|:-|
-        | [d4rl-pybullet](https://github.com/takuseno/d4rl-pybullet) | An offline RL datasets of PyBullet tasks |
         | [d4rl-atari](https://github.com/takuseno/d4rl-atari) | A d4rl-style library of Google's Atari 2600 datasets |
-        | [MINERVA](https://github.com/takuseno/minerva) | An out-of-the-box GUI tool for offline RL |
         
-        ## roadmap
+        ## Roadmap
         The roadmap to the future release is available in [ROADMAP.md](ROADMAP.md).
         
-        ## citation
+        ## Citation
         The paper is available [here](https://arxiv.org/abs/2111.03788).
         ```
-        @InProceedings{seno2021d3rlpy,
-          author = {Takuma Seno, Michita Imai},
-          title = {d3rlpy: An Offline Deep Reinforcement Library},
-          booktitle = {NeurIPS 2021 Offline Reinforcement Learning Workshop},
-          month = {December},
-          year = {2021}
+        @article{d3rlpy,
+          author  = {Takuma Seno and Michita Imai},
+          title   = {d3rlpy: An Offline Deep Reinforcement Learning Library},
+          journal = {Journal of Machine Learning Research},
+          year    = {2022},
+          volume  = {23},
+          number  = {315},
+          pages   = {1--20},
+          url     = {http://jmlr.org/papers/v23/22-0017.html}
         }
         ```
         
-        ## acknowledgement
+        ## Acknowledgement
+        This work started as a part of [Takuma Seno](https://github.com/takuseno)'s Ph.D project at Keio University in 2020.
+        
         This work is supported by Information-technology Promotion Agency, Japan
         (IPA), Exploratory IT Human Resources Project (MITOU Program) in the fiscal
         year 2020.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `d3rlpy-1.1.1/README.md` & `d3rlpy-2.0.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -14,46 +14,44 @@
 
 ```py
 import d3rlpy
 
 dataset, env = d3rlpy.datasets.get_dataset("hopper-medium-v0")
 
 # prepare algorithm
-sac = d3rlpy.algos.SAC()
+sac = d3rlpy.algos.SACConfig().create(device="cuda:0")
 
 # train offline
 sac.fit(dataset, n_steps=1000000)
 
 # train online
 sac.fit_online(env, n_steps=1000000)
 
 # ready to control
 actions = sac.predict(x)
 ```
 
 - Documentation: https://d3rlpy.readthedocs.io
 - Paper: https://arxiv.org/abs/2111.03788
 
-## key features
+## Key features
 
 ### :zap: Most Practical RL Library Ever
 - **offline RL**: d3rlpy supports state-of-the-art offline RL algorithms. Offline RL is extremely powerful when the online interaction is not feasible during training (e.g. robotics, medical).
 - **online RL**: d3rlpy also supports conventional state-of-the-art online training algorithms without any compromising, which means that you can solve any kinds of RL problems only with `d3rlpy`.
-- **advanced engineering**: d3rlpy is designed to implement the faster and efficient training algorithms. For example, you can train Atari environments with x4 less memory space and as fast as the fastest RL library.
 
 ### :beginner: User-friendly API
 - **zero-knowledge of DL library**: d3rlpy provides many state-of-the-art algorithms through intuitive APIs. You can become a RL engineer even without knowing how to use deep learning libraries.
 - **extensive documentation**: d3rlpy is fully documented and accompanied with tutorials and reproduction scripts of the original papers.
 
 ### :rocket: Beyond State-of-the-art
 - **distributional Q function**: d3rlpy is the first library that supports distributional Q functions in the all algorithms. The distributional Q function is known as the very powerful method to achieve the state-of-the-performance.
-- **many tweek options**: d3rlpy is also the first to support N-step TD backup and ensemble value functions in the all algorithms, which lead you to the place no one ever reached yet.
 
 
-## installation
+## Installation
 d3rlpy supports Linux, macOS and Windows.
 
 ### PyPI (recommended)
 [![PyPI version](https://badge.fury.io/py/d3rlpy.svg)](https://badge.fury.io/py/d3rlpy)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/d3rlpy)
 ```
 $ pip install d3rlpy
@@ -68,15 +66,15 @@
 
 ### Docker
 ![Docker Pulls](https://img.shields.io/docker/pulls/takuseno/d3rlpy)
 ```
 $ docker run -it --gpus all --name d3rlpy takuseno/d3rlpy:latest bash
 ```
 
-## supported algorithms
+## Supported algorithms
 | algorithm | discrete control | continuous control | offline RL? |
 |:-|:-:|:-:|:-:|
 | Behavior Cloning (supervised learning) | :white_check_mark: | :white_check_mark: | |
 | [Neural Fitted Q Iteration (NFQ)](https://link.springer.com/chapter/10.1007/11564096_32) | :white_check_mark: | :no_entry: | :white_check_mark: |
 | [Deep Q-Network (DQN)](https://www.nature.com/articles/nature14236) | :white_check_mark: | :no_entry: | |
 | [Double DQN](https://arxiv.org/abs/1509.06461) | :white_check_mark: | :no_entry: | |
 | [Deep Deterministic Policy Gradients (DDPG)](https://arxiv.org/abs/1509.02971) | :no_entry: | :white_check_mark: | |
@@ -86,153 +84,137 @@
 | [Bootstrapping Error Accumulation Reduction (BEAR)](https://arxiv.org/abs/1906.00949) | :no_entry: | :white_check_mark: | :white_check_mark: |
 | [Conservative Q-Learning (CQL)](https://arxiv.org/abs/2006.04779) | :white_check_mark: | :white_check_mark: | :white_check_mark: |
 | [Advantage Weighted Actor-Critic (AWAC)](https://arxiv.org/abs/2006.09359) | :no_entry: | :white_check_mark: | :white_check_mark: |
 | [Critic Reguralized Regression (CRR)](https://arxiv.org/abs/2006.15134) | :no_entry: | :white_check_mark: | :white_check_mark: |
 | [Policy in Latent Action Space (PLAS)](https://arxiv.org/abs/2011.07213) | :no_entry: | :white_check_mark: | :white_check_mark: |
 | [TD3+BC](https://arxiv.org/abs/2106.06860) | :no_entry: | :white_check_mark: | :white_check_mark: |
 | [Implicit Q-Learning (IQL)](https://arxiv.org/abs/2110.06169) | :no_entry: | :white_check_mark: | :white_check_mark: |
+| [Decision Transformer](https://arxiv.org/abs/2106.01345) | :construction: | :white_check_mark: | :white_check_mark: |
 
-## supported Q functions
+## Supported Q functions
 - [x] standard Q function
 - [x] [Quantile Regression](https://arxiv.org/abs/1710.10044)
 - [x] [Implicit Quantile Network](https://arxiv.org/abs/1806.06923)
 
-## experimental features
-- Model-based Algorithms
-  - [Model-based Offline Policy Optimization (MOPO)](https://arxiv.org/abs/2005.13239)
-  - [Conservative Offline Model-Based Policy Optimization (COMBO)](https://arxiv.org/abs/2102.08363)
-- Q-functions
-  - [Fully parametrized Quantile Function](https://arxiv.org/abs/1911.02140) (experimental)
-
-## benchmark results
+## Benchmark results
 d3rlpy is benchmarked to ensure the implementation quality.
 The benchmark scripts are available [reproductions](https://github.com/takuseno/d3rlpy/tree/master/reproductions) directory.
 The benchmark results are available [d3rlpy-benchmarks](https://github.com/takuseno/d3rlpy-benchmarks) repository.
 
-## examples
+## Examples
 ### MuJoCo
 <p align="center"><img align="center" width="160px" src="assets/mujoco_hopper.gif"></p>
 
 ```py
 import d3rlpy
 
 # prepare dataset
 dataset, env = d3rlpy.datasets.get_d4rl('hopper-medium-v0')
 
 # prepare algorithm
-cql = d3rlpy.algos.CQL(use_gpu=True)
+cql = d3rlpy.algos.CQLConfig().create(device='cuda:0')
 
 # train
 cql.fit(
     dataset,
-    eval_episodes=dataset,
-    n_epochs=100,
-    scorers={
-        'environment': d3rlpy.metrics.evaluate_on_environment(env),
-        'td_error': d3rlpy.metrics.td_error_scorer,
-    },
+    n_steps=100000,
+    evaluators={"environment": d3rlpy.metrics.EnvironmentEvaluator(env)},
 )
 ```
 
 See more datasets at [d4rl](https://github.com/rail-berkeley/d4rl).
 
 ### Atari 2600
 <p align="center"><img align="center" width="160px" src="assets/breakout.gif"></p>
 
 ```py
 import d3rlpy
-from sklearn.model_selection import train_test_split
-
-# prepare dataset
-dataset, env = d3rlpy.datasets.get_atari('breakout-expert-v0')
 
-# split dataset
-train_episodes, test_episodes = train_test_split(dataset, test_size=0.1)
+# prepare dataset (1% dataset)
+dataset, env = d3rlpy.datasets.get_atari_transitions(
+    'breakout',
+    fraction=0.01,
+    num_stack=4,
+)
 
 # prepare algorithm
-cql = d3rlpy.algos.DiscreteCQL(
-    n_frames=4,
-    q_func_factory='qr',
-    scaler='pixel',
-    use_gpu=True,
-)
+cql = d3rlpy.algos.DiscreteCQLConfig(
+    observation_scaler=d3rlpy.preprocessing.PixelObservationScaler(),
+    reward_scaler=d3rlpy.preprocessing.ClipRewardScaler(-1.0, 1.0),
+).create(device='cuda:0')
 
 # start training
 cql.fit(
-    train_episodes,
-    eval_episodes=test_episodes,
-    n_epochs=100,
-    scorers={
-        'environment': d3rlpy.metrics.evaluate_on_environment(env),
-        'td_error': d3rlpy.metrics.td_error_scorer,
-    },
+    dataset,
+    n_steps=1000000,
+    evaluators={"environment": d3rlpy.metrics.EnvironmentEvaluator(env, epsilon=0.001)},
 )
 ```
 
 See more Atari datasets at [d4rl-atari](https://github.com/takuseno/d4rl-atari).
 
 
 ### Online Training
 ```py
 import d3rlpy
 import gym
 
 # prepare environment
-env = gym.make('HopperBulletEnv-v0')
-eval_env = gym.make('HopperBulletEnv-v0')
+env = gym.make('Hopper-v3')
+eval_env = gym.make('Hopper-v3')
 
 # prepare algorithm
-sac = d3rlpy.algos.SAC(use_gpu=True)
+sac = d3rlpy.algos.SACConfig().create(device='cuda:0')
 
 # prepare replay buffer
-buffer = d3rlpy.online.buffers.ReplayBuffer(maxlen=1000000, env=env)
+buffer = d3rlpy.dataset.create_fifo_replay_buffer(limit=1000000, env=env)
 
 # start training
 sac.fit_online(env, buffer, n_steps=1000000, eval_env=eval_env)
 ```
 
-## tutorials
+## Tutorials
 Try cartpole examples on Google Colaboratory!
 
 - offline RL tutorial: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/takuseno/d3rlpy/blob/master/tutorials/cartpole.ipynb)
 - online RL tutorial: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/takuseno/d3rlpy/blob/master/tutorials/online.ipynb)
 
 More tutorial documentations are available [here](https://d3rlpy.readthedocs.io/en/stable/tutorials/index.html).
 
-## contributions
+## Contributions
 Any kind of contribution to d3rlpy would be highly appreciated!
 Please check the [contribution guide](CONTRIBUTING.md).
 
-The release planning can be checked at [milestones](https://github.com/takuseno/d3rlpy/milestones).
-
-## community
+## Community
 | Channel | Link |
 |:-|:-|
-| Chat | [Gitter](https://gitter.im/d3rlpy/d3rlpy) |
 | Issues | [GitHub Issues](https://github.com/takuseno/d3rlpy/issues) |
 
-## family projects
+## Family projects
 | Project | Description |
 |:-:|:-|
-| [d4rl-pybullet](https://github.com/takuseno/d4rl-pybullet) | An offline RL datasets of PyBullet tasks |
 | [d4rl-atari](https://github.com/takuseno/d4rl-atari) | A d4rl-style library of Google's Atari 2600 datasets |
-| [MINERVA](https://github.com/takuseno/minerva) | An out-of-the-box GUI tool for offline RL |
 
-## roadmap
+## Roadmap
 The roadmap to the future release is available in [ROADMAP.md](ROADMAP.md).
 
-## citation
+## Citation
 The paper is available [here](https://arxiv.org/abs/2111.03788).
 ```
-@InProceedings{seno2021d3rlpy,
-  author = {Takuma Seno, Michita Imai},
-  title = {d3rlpy: An Offline Deep Reinforcement Library},
-  booktitle = {NeurIPS 2021 Offline Reinforcement Learning Workshop},
-  month = {December},
-  year = {2021}
+@article{d3rlpy,
+  author  = {Takuma Seno and Michita Imai},
+  title   = {d3rlpy: An Offline Deep Reinforcement Learning Library},
+  journal = {Journal of Machine Learning Research},
+  year    = {2022},
+  volume  = {23},
+  number  = {315},
+  pages   = {1--20},
+  url     = {http://jmlr.org/papers/v23/22-0017.html}
 }
 ```
 
-## acknowledgement
+## Acknowledgement
+This work started as a part of [Takuma Seno](https://github.com/takuseno)'s Ph.D project at Keio University in 2020.
+
 This work is supported by Information-technology Promotion Agency, Japan
 (IPA), Exploratory IT Human Resources Project (MITOU Program) in the fiscal
 year 2020.
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/awac.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/crr.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,194 +1,200 @@
-from typing import Any, Dict, Optional, Sequence
+import dataclasses
+from typing import Dict
 
-from ..argument_utility import (
-    ActionScalerArg,
-    EncoderArg,
-    QFuncArg,
-    RewardScalerArg,
-    ScalerArg,
-    UseGPUArg,
-    check_encoder,
-    check_q_func,
-    check_use_gpu,
+from ...base import DeviceArg, LearnableConfig, register_learnable
+from ...constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
+from ...dataset import Shape
+from ...models.builders import (
+    create_continuous_q_function,
+    create_non_squashed_normal_policy,
 )
-from ..constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
-from ..dataset import TransitionMiniBatch
-from ..gpu import Device
-from ..models.encoders import EncoderFactory
-from ..models.optimizers import AdamFactory, OptimizerFactory
-from ..models.q_functions import QFunctionFactory
-from .base import AlgoBase
-from .torch.awac_impl import AWACImpl
-
-
-class AWAC(AlgoBase):
-    r"""Advantage Weighted Actor-Critic algorithm.
-
-    AWAC is a TD3-based actor-critic algorithm that enables efficient
-    fine-tuning where the policy is trained with offline datasets and is
-    deployed to online training.
+from ...models.encoders import EncoderFactory, make_encoder_field
+from ...models.optimizers import OptimizerFactory, make_optimizer_field
+from ...models.q_functions import QFunctionFactory, make_q_func_field
+from ...torch_utility import TorchMiniBatch
+from .base import QLearningAlgoBase
+from .torch.crr_impl import CRRImpl
+
+__all__ = ["CRRConfig", "CRR"]
+
+
+@dataclasses.dataclass()
+class CRRConfig(LearnableConfig):
+    r"""Config of Critic Reguralized Regression algorithm.
+
+    CRR is a simple offline RL method similar to AWAC.
 
     The policy is trained as a supervised regression.
 
     .. math::
 
         J(\phi) = \mathbb{E}_{s_t, a_t \sim D}
-            [\log \pi_\phi(a_t|s_t)
-                \exp(\frac{1}{\lambda} A^\pi (s_t, a_t))]
+            [\log \pi_\phi(a_t|s_t) f(Q_\theta, \pi_\phi, s_t, a_t)]
+
+    where :math:`f` is a filter function which has several options. The first
+    option is ``binary`` function.
+
+    .. math::
+
+        f := \mathbb{1} [A_\theta(s, a) > 0]
+
+    The other is ``exp`` function.
+
+    .. math::
+
+        f := \exp(A(s, a) / \beta)
+
+    The :math:`A(s, a)` is an average function which also has several options.
+    The first option is ``mean``.
+
+    .. math::
 
-    where :math:`A^\pi (s_t, a_t) = Q_\theta(s_t, a_t) -
-    Q_\theta(s_t, a'_t)` and :math:`a'_t \sim \pi_\phi(\cdot|s_t)`
+        A(s, a) = Q_\theta (s, a) - \frac{1}{m} \sum^m_j Q(s, a_j)
 
-    The key difference from AWR is that AWAC uses Q-function trained via TD
-    learning for the better sample-efficiency.
+    The other one is ``max``.
+
+    .. math::
+
+        A(s, a) = Q_\theta (s, a) - \max^m_j Q(s, a_j)
+
+    where :math:`a_j \sim \pi_\phi(s)`.
+
+    In evaluation, the action is determined by Critic Weighted Policy (CWP).
+    In CWP, the several actions are sampled from the policy function, and the
+    final action is re-sampled from the estimated action-value distribution.
 
     References:
-        * `Nair et al., Accelerating Online Reinforcement Learning with Offline
-          Datasets. <https://arxiv.org/abs/2006.09359>`_
+        * `Wang et al., Critic Reguralized Regression.
+          <https://arxiv.org/abs/2006.15134>`_
 
     Args:
-        actor_learning_rate (float): learning rate for policy function.
-        critic_learning_rate (float): learning rate for Q functions.
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        action_scaler (d3rlpy.preprocessing.ActionScaler): Action preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        actor_learning_rate (float): Learning rate for policy function.
+        critic_learning_rate (float): Learning rate for Q functions.
         actor_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the actor.
+            Optimizer factory for the actor.
         critic_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the critic.
-        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the actor.
-        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the critic.
-        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory or str):
+            Optimizer factory for the critic.
+        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the actor.
+        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the critic.
+        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory):
             Q function factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        tau (float): target network synchronization coefficiency.
-        lam (float): :math:`\lambda` for weight calculation.
-        n_action_samples (int): the number of sampled actions to calculate
-            :math:`A^\pi(s_t, a_t)`.
-        n_critics (int): the number of Q functions for ensemble.
-        update_actor_interval (int): interval to update policy function.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`
-        action_scaler (d3rlpy.preprocessing.ActionScaler or str):
-            action preprocessor. The available options are ``['min_max']``.
-        reward_scaler (d3rlpy.preprocessing.RewardScaler or str):
-            reward preprocessor. The available options are
-            ``['clip', 'min_max', 'standard']``.
-        impl (d3rlpy.algos.torch.awac_impl.AWACImpl): algorithm implementation.
-
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        beta (float): Temperature value defined as :math:`\beta` above.
+        n_action_samples (int): Number of sampled actions to calculate
+            :math:`A(s, a)` and for CWP.
+        advantage_type (str): Advantage function type. The available options
+            are ``['mean', 'max']``.
+        weight_type (str): Filter function type. The available options
+            are ``['binary', 'exp']``.
+        max_weight (float): Maximum weight for cross-entropy loss.
+        n_critics (int): Number of Q functions for ensemble.
+        target_update_type (str): Target update type. The available options are
+            ``['hard', 'soft']``.
+        tau (float): Target network synchronization coefficiency used with
+            ``soft`` target update.
+        update_actor_interval (int): Interval to update policy function used
+            with ``hard`` target update.
     """
+    actor_learning_rate: float = 3e-4
+    critic_learning_rate: float = 3e-4
+    actor_optim_factory: OptimizerFactory = make_optimizer_field()
+    critic_optim_factory: OptimizerFactory = make_optimizer_field()
+    actor_encoder_factory: EncoderFactory = make_encoder_field()
+    critic_encoder_factory: EncoderFactory = make_encoder_field()
+    q_func_factory: QFunctionFactory = make_q_func_field()
+    batch_size: int = 100
+    gamma: float = 0.99
+    beta: float = 1.0
+    n_action_samples: int = 4
+    advantage_type: str = "mean"
+    weight_type: str = "exp"
+    max_weight: float = 20.0
+    n_critics: int = 1
+    target_update_type: str = "hard"
+    tau: float = 5e-3
+    target_update_interval: int = 100
+    update_actor_interval: int = 1
+
+    def create(self, device: DeviceArg = False) -> "CRR":
+        return CRR(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "crr"
+
+
+class CRR(QLearningAlgoBase[CRRImpl, CRRConfig]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        policy = create_non_squashed_normal_policy(
+            observation_shape,
+            action_size,
+            self._config.actor_encoder_factory,
+            device=self._device,
+        )
+        q_func = create_continuous_q_function(
+            observation_shape,
+            action_size,
+            self._config.critic_encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
 
-    _actor_learning_rate: float
-    _critic_learning_rate: float
-    _actor_optim_factory: OptimizerFactory
-    _critic_optim_factory: OptimizerFactory
-    _actor_encoder_factory: EncoderFactory
-    _critic_encoder_factory: EncoderFactory
-    _q_func_factory: QFunctionFactory
-    _tau: float
-    _lam: float
-    _n_action_samples: int
-    _n_critics: int
-    _update_actor_interval: int
-    _use_gpu: Optional[Device]
-    _impl: Optional[AWACImpl]
-
-    def __init__(
-        self,
-        *,
-        actor_learning_rate: float = 3e-4,
-        critic_learning_rate: float = 3e-4,
-        actor_optim_factory: OptimizerFactory = AdamFactory(weight_decay=1e-4),
-        critic_optim_factory: OptimizerFactory = AdamFactory(),
-        actor_encoder_factory: EncoderArg = "default",
-        critic_encoder_factory: EncoderArg = "default",
-        q_func_factory: QFuncArg = "mean",
-        batch_size: int = 1024,
-        n_frames: int = 1,
-        n_steps: int = 1,
-        gamma: float = 0.99,
-        tau: float = 0.005,
-        lam: float = 1.0,
-        n_action_samples: int = 1,
-        n_critics: int = 2,
-        update_actor_interval: int = 1,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        action_scaler: ActionScalerArg = None,
-        reward_scaler: RewardScalerArg = None,
-        impl: Optional[AWACImpl] = None,
-        **kwargs: Any
-    ):
-        super().__init__(
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=n_steps,
-            gamma=gamma,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            reward_scaler=reward_scaler,
-            kwargs=kwargs,
+        actor_optim = self._config.actor_optim_factory.create(
+            policy.parameters(), lr=self._config.actor_learning_rate
+        )
+        critic_optim = self._config.critic_optim_factory.create(
+            q_func.parameters(), lr=self._config.critic_learning_rate
         )
-        self._actor_learning_rate = actor_learning_rate
-        self._critic_learning_rate = critic_learning_rate
-        self._actor_optim_factory = actor_optim_factory
-        self._critic_optim_factory = critic_optim_factory
-        self._actor_encoder_factory = check_encoder(actor_encoder_factory)
-        self._critic_encoder_factory = check_encoder(critic_encoder_factory)
-        self._q_func_factory = check_q_func(q_func_factory)
-        self._tau = tau
-        self._lam = lam
-        self._n_action_samples = n_action_samples
-        self._n_critics = n_critics
-        self._update_actor_interval = update_actor_interval
-        self._use_gpu = check_use_gpu(use_gpu)
-        self._impl = impl
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
-        self._impl = AWACImpl(
+        self._impl = CRRImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            actor_learning_rate=self._actor_learning_rate,
-            critic_learning_rate=self._critic_learning_rate,
-            actor_optim_factory=self._actor_optim_factory,
-            critic_optim_factory=self._critic_optim_factory,
-            actor_encoder_factory=self._actor_encoder_factory,
-            critic_encoder_factory=self._critic_encoder_factory,
-            q_func_factory=self._q_func_factory,
-            gamma=self._gamma,
-            tau=self._tau,
-            lam=self._lam,
-            n_action_samples=self._n_action_samples,
-            n_critics=self._n_critics,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            action_scaler=self._action_scaler,
-            reward_scaler=self._reward_scaler,
+            policy=policy,
+            q_func=q_func,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            gamma=self._config.gamma,
+            beta=self._config.beta,
+            n_action_samples=self._config.n_action_samples,
+            advantage_type=self._config.advantage_type,
+            weight_type=self._config.weight_type,
+            max_weight=self._config.max_weight,
+            tau=self._config.tau,
+            device=self._device,
         )
-        self._impl.build()
 
-    def _update(self, batch: TransitionMiniBatch) -> Dict[str, float]:
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
         assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
 
-        metrics = {}
-
         critic_loss = self._impl.update_critic(batch)
-        metrics.update({"critic_loss": critic_loss})
+        actor_loss = self._impl.update_actor(batch)
 
-        # delayed policy update
-        if self._grad_step % self._update_actor_interval == 0:
-            actor_loss, mean_std = self._impl.update_actor(batch)
-            metrics.update({"actor_loss": actor_loss, "mean_std": mean_std})
+        if self._config.target_update_type == "hard":
+            if self._grad_step % self._config.target_update_interval == 0:
+                self._impl.sync_critic_target()
+                self._impl.sync_actor_target()
+        elif self._config.target_update_type == "soft":
             self._impl.update_critic_target()
             self._impl.update_actor_target()
+        else:
+            raise ValueError(
+                f"invalid target_update_type: {self._config.target_update_type}"
+            )
 
-        return metrics
+        return {"critic_loss": critic_loss, "actor_loss": actor_loss}
 
     def get_action_type(self) -> ActionSpace:
         return ActionSpace.CONTINUOUS
+
+
+register_learnable(CRRConfig)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/bc.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/sac_impl.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,244 +1,236 @@
-from typing import Any, Dict, List, Optional, Sequence, Union
-
-import numpy as np
-
-from ..argument_utility import (
-    ActionScalerArg,
-    EncoderArg,
-    ScalerArg,
-    UseGPUArg,
-    check_encoder,
-    check_use_gpu,
+import copy
+import math
+from typing import Tuple
+
+import torch
+from torch.optim import Optimizer
+
+from ....dataset import Shape
+from ....models.torch import (
+    CategoricalPolicy,
+    EnsembleContinuousQFunction,
+    EnsembleDiscreteQFunction,
+    EnsembleQFunction,
+    Parameter,
+    Policy,
 )
-from ..constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
-from ..dataset import TransitionMiniBatch
-from ..gpu import Device
-from ..models.encoders import EncoderFactory
-from ..models.optimizers import AdamFactory, OptimizerFactory
-from .base import AlgoBase
-from .torch.bc_impl import BCBaseImpl, BCImpl, DiscreteBCImpl
+from ....torch_utility import TorchMiniBatch, hard_sync, train_api
+from ..base import QLearningAlgoImplBase
+from .ddpg_impl import DDPGBaseImpl
+from .utility import DiscreteQFunctionMixin
 
+__all__ = ["SACImpl", "DiscreteSACImpl"]
 
-class _BCBase(AlgoBase):
-    _learning_rate: float
-    _optim_factory: OptimizerFactory
-    _encoder_factory: EncoderFactory
-    _use_gpu: Optional[Device]
-    _impl: Optional[BCBaseImpl]
+
+class SACImpl(DDPGBaseImpl):
+    _log_temp: Parameter
+    _temp_optim: Optimizer
 
     def __init__(
         self,
-        *,
-        learning_rate: float = 1e-3,
-        optim_factory: OptimizerFactory = AdamFactory(),
-        encoder_factory: EncoderArg = "default",
-        batch_size: int = 100,
-        n_frames: int = 1,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        action_scaler: ActionScalerArg = None,
-        impl: Optional[BCBaseImpl] = None,
-        **kwargs: Any
+        observation_shape: Shape,
+        action_size: int,
+        policy: Policy,
+        q_func: EnsembleContinuousQFunction,
+        log_temp: Parameter,
+        actor_optim: Optimizer,
+        critic_optim: Optimizer,
+        temp_optim: Optimizer,
+        gamma: float,
+        tau: float,
+        device: str,
     ):
         super().__init__(
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=1,
-            gamma=1.0,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            kwargs=kwargs,
+            observation_shape=observation_shape,
+            action_size=action_size,
+            policy=policy,
+            q_func=q_func,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            gamma=gamma,
+            tau=tau,
+            device=device,
         )
-        self._learning_rate = learning_rate
-        self._optim_factory = optim_factory
-        self._encoder_factory = check_encoder(encoder_factory)
-        self._use_gpu = check_use_gpu(use_gpu)
-        self._impl = impl
-
-    def _update(self, batch: TransitionMiniBatch) -> Dict[str, float]:
-        assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
-        loss = self._impl.update_imitator(batch.observations, batch.actions)
-        return {"loss": loss}
-
-    def predict_value(
-        self,
-        x: Union[np.ndarray, List[Any]],
-        action: Union[np.ndarray, List[Any]],
-        with_std: bool = False,
-    ) -> np.ndarray:
-        """value prediction is not supported by BC algorithms."""
-        raise NotImplementedError("BC does not support value estimation.")
-
-    def sample_action(self, x: Union[np.ndarray, List[Any]]) -> None:
-        """sampling action is not supported by BC algorithm."""
-        raise NotImplementedError("BC does not support sampling action.")
-
-
-class BC(_BCBase):
-    r"""Behavior Cloning algorithm.
-
-    Behavior Cloning (BC) is to imitate actions in the dataset via a supervised
-    learning approach.
-    Since BC is only imitating action distributions, the performance will be
-    close to the mean of the dataset even though BC mostly works better than
-    online RL algorithms.
-
-    .. math::
-
-        L(\theta) = \mathbb{E}_{a_t, s_t \sim D}
-            [(a_t - \pi_\theta(s_t))^2]
-
-    Args:
-        learning_rate (float): learing rate.
-        optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory.
-        encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        policy_type (str): the policy type. The available options are
-            ``['deterministic', 'stochastic']``.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`.
-        action_scaler (d3rlpy.preprocessing.ActionScaler or str):
-            action scaler. The available options are ``['min_max']``.
-        impl (d3rlpy.algos.torch.bc_impl.BCImpl):
-            implemenation of the algorithm.
-
-    """
+        self._log_temp = log_temp
+        self._temp_optim = temp_optim
 
-    _policy_type: str
-    _impl: Optional[BCImpl]
+    def compute_actor_loss(self, batch: TorchMiniBatch) -> torch.Tensor:
+        action, log_prob = self._policy.sample_with_log_prob(batch.observations)
+        entropy = self._log_temp().exp() * log_prob
+        q_t = self._q_func(batch.observations, action, "min")
+        return (entropy - q_t).mean()
+
+    @train_api
+    def update_temp(self, batch: TorchMiniBatch) -> Tuple[float, float]:
+        self._temp_optim.zero_grad()
+
+        with torch.no_grad():
+            _, log_prob = self._policy.sample_with_log_prob(batch.observations)
+            targ_temp = log_prob - self._action_size
+
+        loss = -(self._log_temp().exp() * targ_temp).mean()
+
+        loss.backward()
+        self._temp_optim.step()
+
+        # current temperature value
+        cur_temp = self._log_temp().exp().cpu().detach().numpy()[0][0]
+
+        return float(loss.cpu().detach().numpy()), float(cur_temp)
+
+    def compute_target(self, batch: TorchMiniBatch) -> torch.Tensor:
+        with torch.no_grad():
+            action, log_prob = self._policy.sample_with_log_prob(
+                batch.next_observations
+            )
+            entropy = self._log_temp().exp() * log_prob
+            target = self._targ_q_func.compute_target(
+                batch.next_observations,
+                action,
+                reduction="min",
+            )
+            return target - entropy
+
+
+class DiscreteSACImpl(DiscreteQFunctionMixin, QLearningAlgoImplBase):
+    _policy: CategoricalPolicy
+    _q_func: EnsembleDiscreteQFunction
+    _targ_q_func: EnsembleDiscreteQFunction
+    _log_temp: Parameter
+    _actor_optim: Optimizer
+    _critic_optim: Optimizer
+    _temp_optim: Optimizer
 
     def __init__(
         self,
-        *,
-        learning_rate: float = 1e-3,
-        optim_factory: OptimizerFactory = AdamFactory(),
-        encoder_factory: EncoderArg = "default",
-        batch_size: int = 100,
-        n_frames: int = 1,
-        policy_type: str = "deterministic",
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        action_scaler: ActionScalerArg = None,
-        impl: Optional[BCBaseImpl] = None,
-        **kwargs: Any
+        observation_shape: Shape,
+        action_size: int,
+        q_func: EnsembleDiscreteQFunction,
+        policy: CategoricalPolicy,
+        log_temp: Parameter,
+        actor_optim: Optimizer,
+        critic_optim: Optimizer,
+        temp_optim: Optimizer,
+        gamma: float,
+        device: str,
     ):
         super().__init__(
-            learning_rate=learning_rate,
-            optim_factory=optim_factory,
-            encoder_factory=encoder_factory,
-            batch_size=batch_size,
-            n_frames=n_frames,
-            use_gpu=use_gpu,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            impl=impl,
-            **kwargs,
-        )
-        self._policy_type = policy_type
-
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
-        self._impl = BCImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            learning_rate=self._learning_rate,
-            optim_factory=self._optim_factory,
-            encoder_factory=self._encoder_factory,
-            policy_type=self._policy_type,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            action_scaler=self._action_scaler,
+            device=device,
         )
-        self._impl.build()
+        self._gamma = gamma
+        self._q_func = q_func
+        self._policy = policy
+        self._log_temp = log_temp
+        self._actor_optim = actor_optim
+        self._critic_optim = critic_optim
+        self._temp_optim = temp_optim
+        self._targ_q_func = copy.deepcopy(q_func)
+
+    @train_api
+    def update_critic(self, batch: TorchMiniBatch) -> float:
+        self._critic_optim.zero_grad()
+
+        q_tpn = self.compute_target(batch)
+        loss = self.compute_critic_loss(batch, q_tpn)
+
+        loss.backward()
+        self._critic_optim.step()
+
+        return float(loss.cpu().detach().numpy())
+
+    def compute_target(self, batch: TorchMiniBatch) -> torch.Tensor:
+        with torch.no_grad():
+            log_probs = self._policy.log_probs(batch.next_observations)
+            probs = log_probs.exp()
+            entropy = self._log_temp().exp() * log_probs
+            target = self._targ_q_func.compute_target(batch.next_observations)
+            keepdims = True
+            if target.dim() == 3:
+                entropy = entropy.unsqueeze(-1)
+                probs = probs.unsqueeze(-1)
+                keepdims = False
+            return (probs * (target - entropy)).sum(dim=1, keepdim=keepdims)
 
-    def get_action_type(self) -> ActionSpace:
-        return ActionSpace.CONTINUOUS
+    def compute_critic_loss(
+        self,
+        batch: TorchMiniBatch,
+        q_tpn: torch.Tensor,
+    ) -> torch.Tensor:
+        return self._q_func.compute_error(
+            observations=batch.observations,
+            actions=batch.actions.long(),
+            rewards=batch.rewards,
+            target=q_tpn,
+            terminals=batch.terminals,
+            gamma=self._gamma**batch.intervals,
+        )
 
+    @train_api
+    def update_actor(self, batch: TorchMiniBatch) -> float:
+        # Q function should be inference mode for stability
+        self._q_func.eval()
 
-class DiscreteBC(_BCBase):
-    r"""Behavior Cloning algorithm for discrete control.
+        self._actor_optim.zero_grad()
 
-    Behavior Cloning (BC) is to imitate actions in the dataset via a supervised
-    learning approach.
-    Since BC is only imitating action distributions, the performance will be
-    close to the mean of the dataset even though BC mostly works better than
-    online RL algorithms.
-
-    .. math::
-
-        L(\theta) = \mathbb{E}_{a_t, s_t \sim D}
-            [-\sum_a p(a|s_t) \log \pi_\theta(a|s_t)]
-
-    where :math:`p(a|s_t)` is implemented as a one-hot vector.
-
-    Args:
-        learning_rate (float): learing rate.
-        optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory.
-        encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        beta (float): reguralization factor.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`
-        impl (d3rlpy.algos.torch.bc_impl.DiscreteBCImpl):
-            implemenation of the algorithm.
+        loss = self.compute_actor_loss(batch)
 
-    """
+        loss.backward()
+        self._actor_optim.step()
 
-    _beta: float
-    _impl: Optional[DiscreteBCImpl]
+        return float(loss.cpu().detach().numpy())
 
-    def __init__(
-        self,
-        *,
-        learning_rate: float = 1e-3,
-        optim_factory: OptimizerFactory = AdamFactory(),
-        encoder_factory: EncoderArg = "default",
-        batch_size: int = 100,
-        n_frames: int = 1,
-        beta: float = 0.5,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        impl: Optional[DiscreteBCImpl] = None,
-        **kwargs: Any
-    ):
-        super().__init__(
-            learning_rate=learning_rate,
-            optim_factory=optim_factory,
-            encoder_factory=encoder_factory,
-            batch_size=batch_size,
-            n_frames=n_frames,
-            use_gpu=use_gpu,
-            scaler=scaler,
-            impl=impl,
-            **kwargs,
-        )
-        self._beta = beta
+    def compute_actor_loss(self, batch: TorchMiniBatch) -> torch.Tensor:
+        with torch.no_grad():
+            q_t = self._q_func(batch.observations, reduction="min")
+        log_probs = self._policy.log_probs(batch.observations)
+        probs = log_probs.exp()
+        entropy = self._log_temp().exp() * log_probs
+        return (probs * (entropy - q_t)).sum(dim=1).mean()
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
-        self._impl = DiscreteBCImpl(
-            observation_shape=observation_shape,
-            action_size=action_size,
-            learning_rate=self._learning_rate,
-            optim_factory=self._optim_factory,
-            encoder_factory=self._encoder_factory,
-            beta=self._beta,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-        )
-        self._impl.build()
+    @train_api
+    def update_temp(self, batch: TorchMiniBatch) -> Tuple[float, float]:
+        self._temp_optim.zero_grad()
+
+        with torch.no_grad():
+            log_probs = self._policy.log_probs(batch.observations)
+            probs = log_probs.exp()
+            expct_log_probs = (probs * log_probs).sum(dim=1, keepdim=True)
+            entropy_target = 0.98 * (-math.log(1 / self.action_size))
+            targ_temp = expct_log_probs + entropy_target
+
+        loss = -(self._log_temp().exp() * targ_temp).mean()
+
+        loss.backward()
+        self._temp_optim.step()
+
+        # current temperature value
+        cur_temp = self._log_temp().exp().cpu().detach().numpy()[0][0]
+
+        return float(loss.cpu().detach().numpy()), float(cur_temp)
+
+    def inner_predict_best_action(self, x: torch.Tensor) -> torch.Tensor:
+        return self._policy.best_action(x)
+
+    def inner_sample_action(self, x: torch.Tensor) -> torch.Tensor:
+        return self._policy.sample(x)
+
+    def update_target(self) -> None:
+        hard_sync(self._targ_q_func, self._q_func)
+
+    @property
+    def policy(self) -> Policy:
+        return self._policy
+
+    @property
+    def policy_optim(self) -> Optimizer:
+        return self._actor_optim
+
+    @property
+    def q_function(self) -> EnsembleQFunction:
+        return self._q_func
 
-    def get_action_type(self) -> ActionSpace:
-        return ActionSpace.DISCRETE
+    @property
+    def q_function_optim(self) -> Optimizer:
+        return self._critic_optim
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/bcq.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/bcq.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from typing import Any, Dict, List, Optional, Sequence, Union
+import dataclasses
+from typing import Dict
 
-import numpy as np
-
-from ..argument_utility import (
-    ActionScalerArg,
-    EncoderArg,
-    QFuncArg,
-    RewardScalerArg,
-    ScalerArg,
-    UseGPUArg,
-    check_encoder,
-    check_q_func,
-    check_use_gpu,
+from ...base import DeviceArg, LearnableConfig, register_learnable
+from ...constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
+from ...dataset import Shape
+from ...models.builders import (
+    create_conditional_vae,
+    create_continuous_q_function,
+    create_deterministic_residual_policy,
+    create_discrete_imitator,
+    create_discrete_q_function,
 )
-from ..constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
-from ..dataset import TransitionMiniBatch
-from ..gpu import Device
-from ..models.encoders import EncoderFactory
-from ..models.optimizers import AdamFactory, OptimizerFactory
-from ..models.q_functions import QFunctionFactory
-from .base import AlgoBase
+from ...models.encoders import EncoderFactory, make_encoder_field
+from ...models.optimizers import OptimizerFactory, make_optimizer_field
+from ...models.q_functions import QFunctionFactory, make_q_func_field
+from ...models.torch import DiscreteImitator, PixelEncoder
+from ...torch_utility import TorchMiniBatch
+from .base import QLearningAlgoBase
 from .torch.bcq_impl import BCQImpl, DiscreteBCQImpl
 
+__all__ = ["BCQConfig", "BCQ", "DiscreteBCQConfig", "DiscreteBCQ"]
+
 
-class BCQ(AlgoBase):
-    r"""Batch-Constrained Q-learning algorithm.
+@dataclasses.dataclass()
+class BCQConfig(LearnableConfig):
+    r"""Config of Batch-Constrained Q-learning algorithm.
 
     BCQ is the very first practical data-driven deep reinforcement learning
     lgorithm.
     The major difference from DDPG is that the policy function is represented
     as combination of conditional VAE and perturbation function in order to
     remedy extrapolation error emerging from target value estimation.
 
@@ -95,203 +95,163 @@
         the performance at production.
 
     References:
         * `Fujimoto et al., Off-Policy Deep Reinforcement Learning without
           Exploration. <https://arxiv.org/abs/1812.02900>`_
 
     Args:
-        actor_learning_rate (float): learning rate for policy function.
-        critic_learning_rate (float): learning rate for Q functions.
-        imitator_learning_rate (float): learning rate for Conditional VAE.
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        action_scaler (d3rlpy.preprocessing.ActionScaler): Action preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        actor_learning_rate (float): Learning rate for policy function.
+        critic_learning_rate (float): Learning rate for Q functions.
+        imitator_learning_rate (float): Learning rate for Conditional VAE.
         actor_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the actor.
+            Optimizer factory for the actor.
         critic_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the critic.
+            Optimizer factory for the critic.
         imitator_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the conditional VAE.
-        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the actor.
-        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the critic.
-        imitator_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the conditional VAE.
-        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory or str):
+            Optimizer factory for the conditional VAE.
+        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the actor.
+        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the critic.
+        imitator_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the conditional VAE.
+        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory):
             Q function factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        tau (float): target network synchronization coefficiency.
-        n_critics (int): the number of Q functions for ensemble.
-        update_actor_interval (int): interval to update policy function.
-        lam (float): weight factor for critic ensemble.
-        n_action_samples (int): the number of action samples to estimate
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        tau (float): Target network synchronization coefficiency.
+        n_critics (int): Number of Q functions for ensemble.
+        update_actor_interval (int): Interval to update policy function.
+        lam (float): Weight factor for critic ensemble.
+        n_action_samples (int): Number of action samples to estimate
             action-values.
-        action_flexibility (float): output scale of perturbation function
+        action_flexibility (float): Output scale of perturbation function
             represented as :math:`\Phi`.
-        rl_start_step (int): step to start to update policy function and Q
+        rl_start_step (int): Steps to start to update policy function and Q
             functions. If this is large, RL training would be more stabilized.
         beta (float): KL reguralization term for Conditional VAE.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`.
-        action_scaler (d3rlpy.preprocessing.ActionScaler or str):
-            action preprocessor. The available options are ``['min_max']``.
-        reward_scaler (d3rlpy.preprocessing.RewardScaler or str):
-            reward preprocessor. The available options are
-            ``['clip', 'min_max', 'standard']``.
-        impl (d3rlpy.algos.torch.bcq_impl.BCQImpl): algorithm implementation.
-
     """
+    actor_learning_rate: float = 1e-3
+    critic_learning_rate: float = 1e-3
+    imitator_learning_rate: float = 1e-3
+    actor_optim_factory: OptimizerFactory = make_optimizer_field()
+    critic_optim_factory: OptimizerFactory = make_optimizer_field()
+    imitator_optim_factory: OptimizerFactory = make_optimizer_field()
+    actor_encoder_factory: EncoderFactory = make_encoder_field()
+    critic_encoder_factory: EncoderFactory = make_encoder_field()
+    imitator_encoder_factory: EncoderFactory = make_encoder_field()
+    q_func_factory: QFunctionFactory = make_q_func_field()
+    batch_size: int = 100
+    gamma: float = 0.99
+    tau: float = 0.005
+    n_critics: int = 2
+    update_actor_interval: int = 1
+    lam: float = 0.75
+    n_action_samples: int = 100
+    action_flexibility: float = 0.05
+    rl_start_step: int = 0
+    beta: float = 0.5
+
+    def create(self, device: DeviceArg = False) -> "BCQ":
+        return BCQ(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "bcq"
+
+
+class BCQ(QLearningAlgoBase[BCQImpl, BCQConfig]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        policy = create_deterministic_residual_policy(
+            observation_shape,
+            action_size,
+            self._config.action_flexibility,
+            self._config.actor_encoder_factory,
+            device=self._device,
+        )
+        q_func = create_continuous_q_function(
+            observation_shape,
+            action_size,
+            self._config.critic_encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
+        imitator = create_conditional_vae(
+            observation_shape=observation_shape,
+            action_size=action_size,
+            latent_size=2 * action_size,
+            beta=self._config.beta,
+            min_logstd=-4.0,
+            max_logstd=15.0,
+            encoder_factory=self._config.imitator_encoder_factory,
+            device=self._device,
+        )
 
-    _actor_learning_rate: float
-    _critic_learning_rate: float
-    _imitator_learning_rate: float
-    _actor_optim_factory: OptimizerFactory
-    _critic_optim_factory: OptimizerFactory
-    _imitator_optim_factory: OptimizerFactory
-    _actor_encoder_factory: EncoderFactory
-    _critic_encoder_factory: EncoderFactory
-    _imitator_encoder_factory: EncoderFactory
-    _q_func_factory: QFunctionFactory
-    _tau: float
-    _n_critics: int
-    _update_actor_interval: int
-    _lam: float
-    _n_action_samples: int
-    _action_flexibility: float
-    _rl_start_step: int
-    _beta: float
-    _use_gpu: Optional[Device]
-    _impl: Optional[BCQImpl]
-
-    def __init__(
-        self,
-        *,
-        actor_learning_rate: float = 1e-3,
-        critic_learning_rate: float = 1e-3,
-        imitator_learning_rate: float = 1e-3,
-        actor_optim_factory: OptimizerFactory = AdamFactory(),
-        critic_optim_factory: OptimizerFactory = AdamFactory(),
-        imitator_optim_factory: OptimizerFactory = AdamFactory(),
-        actor_encoder_factory: EncoderArg = "default",
-        critic_encoder_factory: EncoderArg = "default",
-        imitator_encoder_factory: EncoderArg = "default",
-        q_func_factory: QFuncArg = "mean",
-        batch_size: int = 100,
-        n_frames: int = 1,
-        n_steps: int = 1,
-        gamma: float = 0.99,
-        tau: float = 0.005,
-        n_critics: int = 2,
-        update_actor_interval: int = 1,
-        lam: float = 0.75,
-        n_action_samples: int = 100,
-        action_flexibility: float = 0.05,
-        rl_start_step: int = 0,
-        beta: float = 0.5,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        action_scaler: ActionScalerArg = None,
-        reward_scaler: RewardScalerArg = None,
-        impl: Optional[BCQImpl] = None,
-        **kwargs: Any
-    ):
-        super().__init__(
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=n_steps,
-            gamma=gamma,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            reward_scaler=reward_scaler,
-            kwargs=kwargs,
+        actor_optim = self._config.actor_optim_factory.create(
+            policy.parameters(), lr=self._config.actor_learning_rate
+        )
+        critic_optim = self._config.critic_optim_factory.create(
+            q_func.parameters(), lr=self._config.critic_learning_rate
+        )
+        imitator_optim = self._config.imitator_optim_factory.create(
+            imitator.parameters(), lr=self._config.imitator_learning_rate
         )
-        self._actor_learning_rate = actor_learning_rate
-        self._critic_learning_rate = critic_learning_rate
-        self._imitator_learning_rate = imitator_learning_rate
-        self._actor_optim_factory = actor_optim_factory
-        self._critic_optim_factory = critic_optim_factory
-        self._imitator_optim_factory = imitator_optim_factory
-        self._actor_encoder_factory = check_encoder(actor_encoder_factory)
-        self._critic_encoder_factory = check_encoder(critic_encoder_factory)
-        self._imitator_encoder_factory = check_encoder(imitator_encoder_factory)
-        self._q_func_factory = check_q_func(q_func_factory)
-        self._tau = tau
-        self._n_critics = n_critics
-        self._update_actor_interval = update_actor_interval
-        self._lam = lam
-        self._n_action_samples = n_action_samples
-        self._action_flexibility = action_flexibility
-        self._rl_start_step = rl_start_step
-        self._beta = beta
-        self._use_gpu = check_use_gpu(use_gpu)
-        self._impl = impl
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
         self._impl = BCQImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            actor_learning_rate=self._actor_learning_rate,
-            critic_learning_rate=self._critic_learning_rate,
-            imitator_learning_rate=self._imitator_learning_rate,
-            actor_optim_factory=self._actor_optim_factory,
-            critic_optim_factory=self._critic_optim_factory,
-            imitator_optim_factory=self._imitator_optim_factory,
-            actor_encoder_factory=self._actor_encoder_factory,
-            critic_encoder_factory=self._critic_encoder_factory,
-            imitator_encoder_factory=self._imitator_encoder_factory,
-            q_func_factory=self._q_func_factory,
-            gamma=self._gamma,
-            tau=self._tau,
-            n_critics=self._n_critics,
-            lam=self._lam,
-            n_action_samples=self._n_action_samples,
-            action_flexibility=self._action_flexibility,
-            beta=self._beta,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            action_scaler=self._action_scaler,
-            reward_scaler=self._reward_scaler,
+            policy=policy,
+            q_func=q_func,
+            imitator=imitator,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            imitator_optim=imitator_optim,
+            gamma=self._config.gamma,
+            tau=self._config.tau,
+            lam=self._config.lam,
+            n_action_samples=self._config.n_action_samples,
+            action_flexibility=self._config.action_flexibility,
+            beta=self._config.beta,
+            device=self._device,
         )
-        self._impl.build()
 
-    def _update(self, batch: TransitionMiniBatch) -> Dict[str, float]:
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
         assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
 
         metrics = {}
 
         imitator_loss = self._impl.update_imitator(batch)
         metrics.update({"imitator_loss": imitator_loss})
 
-        if self._grad_step >= self._rl_start_step:
+        if self._grad_step >= self._config.rl_start_step:
             critic_loss = self._impl.update_critic(batch)
             metrics.update({"critic_loss": critic_loss})
 
-            if self._grad_step % self._update_actor_interval == 0:
+            if self._grad_step % self._config.update_actor_interval == 0:
                 actor_loss = self._impl.update_actor(batch)
                 metrics.update({"actor_loss": actor_loss})
                 self._impl.update_actor_target()
                 self._impl.update_critic_target()
 
         return metrics
 
-    def sample_action(self, x: Union[np.ndarray, List[Any]]) -> np.ndarray:
-        """BCQ does not support sampling action."""
-        raise NotImplementedError("BCQ does not support sampling action.")
-
     def get_action_type(self) -> ActionSpace:
         return ActionSpace.CONTINUOUS
 
 
-class DiscreteBCQ(AlgoBase):
-    r"""Discrete version of Batch-Constrained Q-learning algorithm.
+@dataclasses.dataclass()
+class DiscreteBCQConfig(LearnableConfig):
+    r"""Config of Discrete version of Batch-Constrained Q-learning algorithm.
 
     Discrete version takes theories from the continuous version, but the
     algorithm is much simpler than that.
     The imitation function :math:`G_\omega(a|s)` is trained as supervised
     learning just like Behavior Cloning.
 
     .. math::
@@ -322,117 +282,109 @@
     References:
         * `Fujimoto et al., Off-Policy Deep Reinforcement Learning without
           Exploration. <https://arxiv.org/abs/1812.02900>`_
         * `Fujimoto et al., Benchmarking Batch Deep Reinforcement Learning
           Algorithms. <https://arxiv.org/abs/1910.01708>`_
 
     Args:
-        learning_rate (float): learning rate.
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        learning_rate (float): Learning rate.
         optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory.
+            Optimizer factory.
         encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory.
+            Encoder factory.
         q_func_factory (d3rlpy.models.q_functions.QFunctionFactory or str):
             Q function factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        n_critics (int): the number of Q functions for ensemble.
-        action_flexibility (float): probability threshold represented as
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        n_critics (int): Number of Q functions for ensemble.
+        action_flexibility (float): Probability threshold represented as
             :math:`\tau`.
-        beta (float): reguralization term for imitation function.
-        target_update_interval (int): interval to update the target network.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`
-        reward_scaler (d3rlpy.preprocessing.RewardScaler or str):
-            reward preprocessor. The available options are
-            ``['clip', 'min_max', 'standard']``.
-        impl (d3rlpy.algos.torch.bcq_impl.DiscreteBCQImpl):
-            algorithm implementation.
-
+        beta (float): Reguralization term for imitation function.
+        target_update_interval (int): Interval to update the target network.
     """
+    learning_rate: float = 6.25e-5
+    optim_factory: OptimizerFactory = make_optimizer_field()
+    encoder_factory: EncoderFactory = make_encoder_field()
+    q_func_factory: QFunctionFactory = make_q_func_field()
+    batch_size: int = 32
+    gamma: float = 0.99
+    n_critics: int = 1
+    action_flexibility: float = 0.3
+    beta: float = 0.5
+    target_update_interval: int = 8000
+
+    def create(self, device: DeviceArg = False) -> "DiscreteBCQ":
+        return DiscreteBCQ(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "discrete_bcq"
+
+
+class DiscreteBCQ(QLearningAlgoBase[DiscreteBCQImpl, DiscreteBCQConfig]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        q_func = create_discrete_q_function(
+            observation_shape,
+            action_size,
+            self._config.encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
 
-    _learning_rate: float
-    _optim_factory: OptimizerFactory
-    _encoder_factory: EncoderFactory
-    _q_func_factory: QFunctionFactory
-    _n_critics: int
-    _action_flexibility: float
-    _beta: float
-    _target_update_interval: int
-    _use_gpu: Optional[Device]
-    _impl: Optional[DiscreteBCQImpl]
-
-    def __init__(
-        self,
-        *,
-        learning_rate: float = 6.25e-5,
-        optim_factory: OptimizerFactory = AdamFactory(),
-        encoder_factory: EncoderArg = "default",
-        q_func_factory: QFuncArg = "mean",
-        batch_size: int = 32,
-        n_frames: int = 1,
-        n_steps: int = 1,
-        gamma: float = 0.99,
-        n_critics: int = 1,
-        action_flexibility: float = 0.3,
-        beta: float = 0.5,
-        target_update_interval: int = 8000,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        reward_scaler: RewardScalerArg = None,
-        impl: Optional[DiscreteBCQImpl] = None,
-        **kwargs: Any
-    ):
-        super().__init__(
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=n_steps,
-            gamma=gamma,
-            scaler=scaler,
-            action_scaler=None,
-            reward_scaler=reward_scaler,
-            kwargs=kwargs,
+        # share convolutional layers if observation is pixel
+        if isinstance(q_func.q_funcs[0].encoder, PixelEncoder):
+            imitator = DiscreteImitator(
+                q_func.q_funcs[0].encoder, action_size, self._config.beta
+            )
+            imitator.to(self._device)
+        else:
+            imitator = create_discrete_imitator(
+                observation_shape,
+                action_size,
+                self._config.beta,
+                self._config.encoder_factory,
+                device=self._device,
+            )
+
+        # TODO: replace this with a cleaner way
+        # retrieve unique elements
+        q_func_params = list(q_func.parameters())
+        imitator_params = list(imitator.parameters())
+        unique_dict = {}
+        for param in q_func_params + imitator_params:
+            unique_dict[param] = param
+        unique_params = list(unique_dict.values())
+        optim = self._config.optim_factory.create(
+            unique_params, lr=self._config.learning_rate
         )
-        self._learning_rate = learning_rate
-        self._optim_factory = optim_factory
-        self._encoder_factory = check_encoder(encoder_factory)
-        self._q_func_factory = check_q_func(q_func_factory)
-        self._n_critics = n_critics
-        self._action_flexibility = action_flexibility
-        self._beta = beta
-        self._target_update_interval = target_update_interval
-        self._use_gpu = check_use_gpu(use_gpu)
-        self._impl = impl
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
         self._impl = DiscreteBCQImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            learning_rate=self._learning_rate,
-            optim_factory=self._optim_factory,
-            encoder_factory=self._encoder_factory,
-            q_func_factory=self._q_func_factory,
-            gamma=self._gamma,
-            n_critics=self._n_critics,
-            action_flexibility=self._action_flexibility,
-            beta=self._beta,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            reward_scaler=self._reward_scaler,
+            q_func=q_func,
+            imitator=imitator,
+            optim=optim,
+            gamma=self._config.gamma,
+            action_flexibility=self._config.action_flexibility,
+            beta=self._config.beta,
+            device=self._device,
         )
-        self._impl.build()
 
-    def _update(self, batch: TransitionMiniBatch) -> Dict[str, float]:
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
         assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
         loss = self._impl.update(batch)
-        if self._grad_step % self._target_update_interval == 0:
+        if self._grad_step % self._config.target_update_interval == 0:
             self._impl.update_target()
         return {"loss": loss}
 
     def get_action_type(self) -> ActionSpace:
         return ActionSpace.DISCRETE
+
+
+register_learnable(BCQConfig)
+register_learnable(DiscreteBCQConfig)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/bear.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/bear.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,32 +1,33 @@
-from typing import Any, Dict, Optional, Sequence
-
-from ..argument_utility import (
-    ActionScalerArg,
-    EncoderArg,
-    QFuncArg,
-    RewardScalerArg,
-    ScalerArg,
-    UseGPUArg,
-    check_encoder,
-    check_q_func,
-    check_use_gpu,
+import dataclasses
+import math
+from typing import Dict
+
+from ...base import DeviceArg, LearnableConfig, register_learnable
+from ...constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
+from ...dataset import Shape
+from ...models.builders import (
+    create_conditional_vae,
+    create_continuous_q_function,
+    create_parameter,
+    create_squashed_normal_policy,
 )
-from ..constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
-from ..dataset import TransitionMiniBatch
-from ..gpu import Device
-from ..models.encoders import EncoderFactory
-from ..models.optimizers import AdamFactory, OptimizerFactory
-from ..models.q_functions import QFunctionFactory
-from .base import AlgoBase
+from ...models.encoders import EncoderFactory, make_encoder_field
+from ...models.optimizers import OptimizerFactory, make_optimizer_field
+from ...models.q_functions import QFunctionFactory, make_q_func_field
+from ...torch_utility import TorchMiniBatch
+from .base import QLearningAlgoBase
 from .torch.bear_impl import BEARImpl
 
+__all__ = ["BEARConfig", "BEAR"]
+
 
-class BEAR(AlgoBase):
-    r"""Bootstrapping Error Accumulation Reduction algorithm.
+@dataclasses.dataclass()
+class BEARConfig(LearnableConfig):
+    r"""Config of Bootstrapping Error Accumulation Reduction algorithm.
 
     BEAR is a SAC-based data-driven deep reinforcement learning algorithm.
 
     BEAR constrains the support of the policy function within data distribution
     by minimizing Maximum Mean Discreptancy (MMD) between the policy function
     and the approximated beahvior policy function :math:`\pi_\beta(a|s)`
     which is optimized through L2 loss.
@@ -60,253 +61,212 @@
     :math:`\epsilon`.
 
     References:
         * `Kumar et al., Stabilizing Off-Policy Q-Learning via Bootstrapping
           Error Reduction. <https://arxiv.org/abs/1906.00949>`_
 
     Args:
-        actor_learning_rate (float): learning rate for policy function.
-        critic_learning_rate (float): learning rate for Q functions.
-        imitator_learning_rate (float): learning rate for behavior policy
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        action_scaler (d3rlpy.preprocessing.ActionScaler): Action preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        actor_learning_rate (float): Learning rate for policy function.
+        critic_learning_rate (float): Learning rate for Q functions.
+        imitator_learning_rate (float): Learning rate for behavior policy
             function.
-        temp_learning_rate (float): learning rate for temperature parameter.
-        alpha_learning_rate (float): learning rate for :math:`\alpha`.
+        temp_learning_rate (float): Learning rate for temperature parameter.
+        alpha_learning_rate (float): Learning rate for :math:`\alpha`.
         actor_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the actor.
+            Optimizer factory for the actor.
         critic_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the critic.
+            Optimizer factory for the critic.
         imitator_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the behavior policy.
+            Optimizer factory for the behavior policy.
         temp_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the temperature.
+            Optimizer factory for the temperature.
         alpha_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for :math:`\alpha`.
-        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the actor.
-        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the critic.
-        imitator_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the behavior policy.
-        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory or str):
+            Optimizer factory for :math:`\alpha`.
+        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the actor.
+        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the critic.
+        imitator_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the behavior policy.
+        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory):
             Q function factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        tau (float): target network synchronization coefficiency.
-        n_critics (int): the number of Q functions for ensemble.
-        initial_temperature (float): initial temperature value.
-        initial_alpha (float): initial :math:`\alpha` value.
-        alpha_threshold (float): threshold value described as
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        tau (float): Target network synchronization coefficiency.
+        n_critics (int): Number of Q functions for ensemble.
+        initial_temperature (float): Initial temperature value.
+        initial_alpha (float): Initial :math:`\alpha` value.
+        alpha_threshold (float): Threshold value described as
             :math:`\epsilon`.
-        lam (float): weight for critic ensemble.
-        n_action_samples (int): the number of action samples to compute the
+        lam (float): Weight for critic ensemble.
+        n_action_samples (int): Number of action samples to compute the
             best action.
-        n_target_samples (int): the number of action samples to compute
+        n_target_samples (int): Number of action samples to compute
             BCQ-like target value.
-        n_mmd_action_samples (int): the number of action samples to compute MMD.
+        n_mmd_action_samples (int): Number of action samples to compute MMD.
         mmd_kernel (str): MMD kernel function. The available options are
             ``['gaussian', 'laplacian']``.
         mmd_sigma (float): :math:`\sigma` for gaussian kernel in MMD
             calculation.
-        vae_kl_weight (float): constant weight to scale KL term for behavior
+        vae_kl_weight (float): Constant weight to scale KL term for behavior
             policy training.
-        warmup_steps (int): the number of steps to warmup the policy
+        warmup_steps (int): Number of steps to warmup the policy
             function.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device iD or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The avaiable options are `['pixel', 'min_max', 'standard']`.
-        action_scaler (d3rlpy.preprocessing.ActionScaler or str):
-            action preprocessor. The avaiable options are ``['min_max']``.
-        reward_scaler (d3rlpy.preprocessing.RewardScaler or str):
-            reward preprocessor. The available options are
-            ``['clip', 'min_max', 'standard']``.
-        impl (d3rlpy.algos.torch.bear_impl.BEARImpl): algorithm implementation.
-
     """
+    actor_learning_rate: float = 1e-4
+    critic_learning_rate: float = 3e-4
+    imitator_learning_rate: float = 3e-4
+    temp_learning_rate: float = 1e-4
+    alpha_learning_rate: float = 1e-3
+    actor_optim_factory: OptimizerFactory = make_optimizer_field()
+    critic_optim_factory: OptimizerFactory = make_optimizer_field()
+    imitator_optim_factory: OptimizerFactory = make_optimizer_field()
+    temp_optim_factory: OptimizerFactory = make_optimizer_field()
+    alpha_optim_factory: OptimizerFactory = make_optimizer_field()
+    actor_encoder_factory: EncoderFactory = make_encoder_field()
+    critic_encoder_factory: EncoderFactory = make_encoder_field()
+    imitator_encoder_factory: EncoderFactory = make_encoder_field()
+    q_func_factory: QFunctionFactory = make_q_func_field()
+    batch_size: int = 256
+    gamma: float = 0.99
+    tau: float = 0.005
+    n_critics: int = 2
+    initial_temperature: float = 1.0
+    initial_alpha: float = 1.0
+    alpha_threshold: float = 0.05
+    lam: float = 0.75
+    n_action_samples: int = 100
+    n_target_samples: int = 10
+    n_mmd_action_samples: int = 4
+    mmd_kernel: str = "laplacian"
+    mmd_sigma: float = 20.0
+    vae_kl_weight: float = 0.5
+    warmup_steps: int = 40000
+
+    def create(self, device: DeviceArg = False) -> "BEAR":
+        return BEAR(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "bear"
+
+
+class BEAR(QLearningAlgoBase[BEARImpl, BEARConfig]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        policy = create_squashed_normal_policy(
+            observation_shape,
+            action_size,
+            self._config.actor_encoder_factory,
+            device=self._device,
+        )
+        q_func = create_continuous_q_function(
+            observation_shape,
+            action_size,
+            self._config.critic_encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
+        imitator = create_conditional_vae(
+            observation_shape=observation_shape,
+            action_size=action_size,
+            latent_size=2 * action_size,
+            beta=self._config.vae_kl_weight,
+            min_logstd=-4.0,
+            max_logstd=15.0,
+            encoder_factory=self._config.imitator_encoder_factory,
+            device=self._device,
+        )
+        log_temp = create_parameter(
+            (1, 1),
+            math.log(self._config.initial_temperature),
+            device=self._device,
+        )
+        log_alpha = create_parameter(
+            (1, 1), math.log(self._config.initial_alpha), device=self._device
+        )
 
-    _actor_learning_rate: float
-    _critic_learning_rate: float
-    _imitator_learning_rate: float
-    _temp_learning_rate: float
-    _alpha_learning_rate: float
-    _actor_optim_factory: OptimizerFactory
-    _critic_optim_factory: OptimizerFactory
-    _imitator_optim_factory: OptimizerFactory
-    _temp_optim_factory: OptimizerFactory
-    _alpha_optim_factory: OptimizerFactory
-    _actor_encoder_factory: EncoderFactory
-    _critic_encoder_factory: EncoderFactory
-    _imitator_encoder_factory: EncoderFactory
-    _q_func_factory: QFunctionFactory
-    _tau: float
-    _n_critics: int
-    _initial_temperature: float
-    _initial_alpha: float
-    _alpha_threshold: float
-    _lam: float
-    _n_action_samples: int
-    _n_target_samples: int
-    _n_mmd_action_samples: int
-    _mmd_kernel: str
-    _mmd_sigma: float
-    _vae_kl_weight: float
-    _warmup_steps: int
-    _use_gpu: Optional[Device]
-    _impl: Optional[BEARImpl]
-
-    def __init__(
-        self,
-        *,
-        actor_learning_rate: float = 1e-4,
-        critic_learning_rate: float = 3e-4,
-        imitator_learning_rate: float = 3e-4,
-        temp_learning_rate: float = 1e-4,
-        alpha_learning_rate: float = 1e-3,
-        actor_optim_factory: OptimizerFactory = AdamFactory(),
-        critic_optim_factory: OptimizerFactory = AdamFactory(),
-        imitator_optim_factory: OptimizerFactory = AdamFactory(),
-        temp_optim_factory: OptimizerFactory = AdamFactory(),
-        alpha_optim_factory: OptimizerFactory = AdamFactory(),
-        actor_encoder_factory: EncoderArg = "default",
-        critic_encoder_factory: EncoderArg = "default",
-        imitator_encoder_factory: EncoderArg = "default",
-        q_func_factory: QFuncArg = "mean",
-        batch_size: int = 256,
-        n_frames: int = 1,
-        n_steps: int = 1,
-        gamma: float = 0.99,
-        tau: float = 0.005,
-        n_critics: int = 2,
-        initial_temperature: float = 1.0,
-        initial_alpha: float = 1.0,
-        alpha_threshold: float = 0.05,
-        lam: float = 0.75,
-        n_action_samples: int = 100,
-        n_target_samples: int = 10,
-        n_mmd_action_samples: int = 4,
-        mmd_kernel: str = "laplacian",
-        mmd_sigma: float = 20.0,
-        vae_kl_weight: float = 0.5,
-        warmup_steps: int = 40000,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        action_scaler: ActionScalerArg = None,
-        reward_scaler: RewardScalerArg = None,
-        impl: Optional[BEARImpl] = None,
-        **kwargs: Any
-    ):
-        super().__init__(
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=n_steps,
-            gamma=gamma,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            reward_scaler=reward_scaler,
-            kwargs=kwargs,
-        )
-        self._actor_learning_rate = actor_learning_rate
-        self._critic_learning_rate = critic_learning_rate
-        self._imitator_learning_rate = imitator_learning_rate
-        self._temp_learning_rate = temp_learning_rate
-        self._alpha_learning_rate = alpha_learning_rate
-        self._actor_optim_factory = actor_optim_factory
-        self._critic_optim_factory = critic_optim_factory
-        self._imitator_optim_factory = imitator_optim_factory
-        self._temp_optim_factory = temp_optim_factory
-        self._alpha_optim_factory = alpha_optim_factory
-        self._actor_encoder_factory = check_encoder(actor_encoder_factory)
-        self._critic_encoder_factory = check_encoder(critic_encoder_factory)
-        self._imitator_encoder_factory = check_encoder(imitator_encoder_factory)
-        self._q_func_factory = check_q_func(q_func_factory)
-        self._tau = tau
-        self._n_critics = n_critics
-        self._initial_temperature = initial_temperature
-        self._initial_alpha = initial_alpha
-        self._alpha_threshold = alpha_threshold
-        self._lam = lam
-        self._n_action_samples = n_action_samples
-        self._n_target_samples = n_target_samples
-        self._n_mmd_action_samples = n_mmd_action_samples
-        self._mmd_kernel = mmd_kernel
-        self._mmd_sigma = mmd_sigma
-        self._vae_kl_weight = vae_kl_weight
-        self._warmup_steps = warmup_steps
-        self._use_gpu = check_use_gpu(use_gpu)
-        self._impl = impl
+        actor_optim = self._config.actor_optim_factory.create(
+            policy.parameters(), lr=self._config.actor_learning_rate
+        )
+        critic_optim = self._config.critic_optim_factory.create(
+            q_func.parameters(), lr=self._config.critic_learning_rate
+        )
+        imitator_optim = self._config.imitator_optim_factory.create(
+            imitator.parameters(), lr=self._config.imitator_learning_rate
+        )
+        temp_optim = self._config.temp_optim_factory.create(
+            log_temp.parameters(), lr=self._config.temp_learning_rate
+        )
+        alpha_optim = self._config.alpha_optim_factory.create(
+            log_alpha.parameters(), lr=self._config.actor_learning_rate
+        )
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
         self._impl = BEARImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            actor_learning_rate=self._actor_learning_rate,
-            critic_learning_rate=self._critic_learning_rate,
-            imitator_learning_rate=self._imitator_learning_rate,
-            temp_learning_rate=self._temp_learning_rate,
-            alpha_learning_rate=self._alpha_learning_rate,
-            actor_optim_factory=self._actor_optim_factory,
-            critic_optim_factory=self._critic_optim_factory,
-            imitator_optim_factory=self._imitator_optim_factory,
-            temp_optim_factory=self._temp_optim_factory,
-            alpha_optim_factory=self._alpha_optim_factory,
-            actor_encoder_factory=self._actor_encoder_factory,
-            critic_encoder_factory=self._critic_encoder_factory,
-            imitator_encoder_factory=self._imitator_encoder_factory,
-            q_func_factory=self._q_func_factory,
-            gamma=self._gamma,
-            tau=self._tau,
-            n_critics=self._n_critics,
-            initial_temperature=self._initial_temperature,
-            initial_alpha=self._initial_alpha,
-            alpha_threshold=self._alpha_threshold,
-            lam=self._lam,
-            n_action_samples=self._n_action_samples,
-            n_target_samples=self._n_target_samples,
-            n_mmd_action_samples=self._n_mmd_action_samples,
-            mmd_kernel=self._mmd_kernel,
-            mmd_sigma=self._mmd_sigma,
-            vae_kl_weight=self._vae_kl_weight,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            action_scaler=self._action_scaler,
-            reward_scaler=self._reward_scaler,
+            policy=policy,
+            q_func=q_func,
+            imitator=imitator,
+            log_temp=log_temp,
+            log_alpha=log_alpha,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            imitator_optim=imitator_optim,
+            temp_optim=temp_optim,
+            alpha_optim=alpha_optim,
+            gamma=self._config.gamma,
+            tau=self._config.tau,
+            alpha_threshold=self._config.alpha_threshold,
+            lam=self._config.lam,
+            n_action_samples=self._config.n_action_samples,
+            n_target_samples=self._config.n_target_samples,
+            n_mmd_action_samples=self._config.n_mmd_action_samples,
+            mmd_kernel=self._config.mmd_kernel,
+            mmd_sigma=self._config.mmd_sigma,
+            vae_kl_weight=self._config.vae_kl_weight,
+            device=self._device,
         )
-        self._impl.build()
 
-    def _update(self, batch: TransitionMiniBatch) -> Dict[str, float]:
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
         assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
 
         metrics = {}
 
         imitator_loss = self._impl.update_imitator(batch)
         metrics.update({"imitator_loss": imitator_loss})
 
         # lagrangian parameter update for SAC temperature
-        if self._temp_learning_rate > 0:
+        if self._config.temp_learning_rate > 0:
             temp_loss, temp = self._impl.update_temp(batch)
             metrics.update({"temp_loss": temp_loss, "temp": temp})
 
         # lagrangian parameter update for MMD loss weight
-        if self._alpha_learning_rate > 0:
+        if self._config.alpha_learning_rate > 0:
             alpha_loss, alpha = self._impl.update_alpha(batch)
             metrics.update({"alpha_loss": alpha_loss, "alpha": alpha})
 
         critic_loss = self._impl.update_critic(batch)
         metrics.update({"critic_loss": critic_loss})
 
-        if self._grad_step < self._warmup_steps:
+        if self._grad_step < self._config.warmup_steps:
             actor_loss = self._impl.warmup_actor(batch)
         else:
             actor_loss = self._impl.update_actor(batch)
         metrics.update({"actor_loss": actor_loss})
 
         self._impl.update_actor_target()
         self._impl.update_critic_target()
 
         return metrics
 
     def get_action_type(self) -> ActionSpace:
         return ActionSpace.CONTINUOUS
+
+
+register_learnable(BEARConfig)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/cql.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/cql.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,33 +1,33 @@
-from typing import Any, Dict, Optional, Sequence
-
-from ..argument_utility import (
-    ActionScalerArg,
-    EncoderArg,
-    QFuncArg,
-    RewardScalerArg,
-    ScalerArg,
-    UseGPUArg,
-    check_encoder,
-    check_q_func,
-    check_use_gpu,
+import dataclasses
+import math
+from typing import Dict
+
+from ...base import DeviceArg, LearnableConfig, register_learnable
+from ...constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
+from ...dataset import Shape
+from ...models.builders import (
+    create_continuous_q_function,
+    create_discrete_q_function,
+    create_parameter,
+    create_squashed_normal_policy,
 )
-from ..constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
-from ..dataset import TransitionMiniBatch
-from ..gpu import Device
-from ..models.encoders import EncoderFactory
-from ..models.optimizers import AdamFactory, OptimizerFactory
-from ..models.q_functions import QFunctionFactory
-from .base import AlgoBase
-from .dqn import DoubleDQN
+from ...models.encoders import EncoderFactory, make_encoder_field
+from ...models.optimizers import OptimizerFactory, make_optimizer_field
+from ...models.q_functions import QFunctionFactory, make_q_func_field
+from ...torch_utility import TorchMiniBatch
+from .base import QLearningAlgoBase
 from .torch.cql_impl import CQLImpl, DiscreteCQLImpl
 
+__all__ = ["CQLConfig", "CQL", "DiscreteCQLConfig", "DiscreteCQL"]
+
 
-class CQL(AlgoBase):
-    r"""Conservative Q-Learning algorithm.
+@dataclasses.dataclass()
+class CQLConfig(LearnableConfig):
+    r"""Config of Conservative Q-Learning algorithm.
 
     CQL is a SAC-based data-driven deep reinforcement learning algorithm, which
     achieves state-of-the-art performance in offline RL problems.
 
     CQL mitigates overestimation error by minimizing action-values under the
     current policy and maximizing values under data distribution for
     underestimation issue.
@@ -62,191 +62,151 @@
     The rest of optimization is exactly same as :class:`d3rlpy.algos.SAC`.
 
     References:
         * `Kumar et al., Conservative Q-Learning for Offline Reinforcement
           Learning. <https://arxiv.org/abs/2006.04779>`_
 
     Args:
-        actor_learning_rate (float): learning rate for policy function.
-        critic_learning_rate (float): learning rate for Q functions.
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        action_scaler (d3rlpy.preprocessing.ActionScaler): Action preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        actor_learning_rate (float): Learning rate for policy function.
+        critic_learning_rate (float): Learning rate for Q functions.
         temp_learning_rate (float):
-            learning rate for temperature parameter of SAC.
-        alpha_learning_rate (float): learning rate for :math:`\alpha`.
+            Learning rate for temperature parameter of SAC.
+        alpha_learning_rate (float): Learning rate for :math:`\alpha`.
         actor_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the actor.
+            Optimizer factory for the actor.
         critic_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the critic.
+            Optimizer factory for the critic.
         temp_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the temperature.
+            Optimizer factory for the temperature.
         alpha_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for :math:`\alpha`.
-        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the actor.
-        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the critic.
-        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory or str):
+            Optimizer factory for :math:`\alpha`.
+        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the actor.
+        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the critic.
+        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory):
             Q function factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        tau (float): target network synchronization coefficiency.
-        n_critics (int): the number of Q functions for ensemble.
-        initial_temperature (float): initial temperature value.
-        initial_alpha (float): initial :math:`\alpha` value.
-        alpha_threshold (float): threshold value described as :math:`\tau`.
-        conservative_weight (float): constant weight to scale conservative loss.
-        n_action_samples (int): the number of sampled actions to compute
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        tau (float): Target network synchronization coefficiency.
+        n_critics (int): Number of Q functions for ensemble.
+        initial_temperature (float): Initial temperature value.
+        initial_alpha (float): Initial :math:`\alpha` value.
+        alpha_threshold (float): Threshold value described as :math:`\tau`.
+        conservative_weight (float): Constant weight to scale conservative loss.
+        n_action_samples (int): Number of sampled actions to compute
             :math:`\log{\sum_a \exp{Q(s, a)}}`.
-        soft_q_backup (bool): flag to use SAC-style backup.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`.
-        action_scaler (d3rlpy.preprocessing.ActionScaler or str):
-            action preprocessor. The available options are ``['min_max']``.
-        reward_scaler (d3rlpy.preprocessing.RewardScaler or str):
-            reward preprocessor. The available options are
-            ``['clip', 'min_max', 'standard']``.
-        impl (d3rlpy.algos.torch.cql_impl.CQLImpl): algorithm implementation.
-
+        soft_q_backup (bool): Flag to use SAC-style backup.
     """
+    actor_learning_rate: float = 1e-4
+    critic_learning_rate: float = 3e-4
+    temp_learning_rate: float = 1e-4
+    alpha_learning_rate: float = 1e-4
+    actor_optim_factory: OptimizerFactory = make_optimizer_field()
+    critic_optim_factory: OptimizerFactory = make_optimizer_field()
+    temp_optim_factory: OptimizerFactory = make_optimizer_field()
+    alpha_optim_factory: OptimizerFactory = make_optimizer_field()
+    actor_encoder_factory: EncoderFactory = make_encoder_field()
+    critic_encoder_factory: EncoderFactory = make_encoder_field()
+    q_func_factory: QFunctionFactory = make_q_func_field()
+    batch_size: int = 256
+    gamma: float = 0.99
+    tau: float = 0.005
+    n_critics: int = 2
+    initial_temperature: float = 1.0
+    initial_alpha: float = 1.0
+    alpha_threshold: float = 10.0
+    conservative_weight: float = 5.0
+    n_action_samples: int = 10
+    soft_q_backup: bool = False
+
+    def create(self, device: DeviceArg = False) -> "CQL":
+        return CQL(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "cql"
+
+
+class CQL(QLearningAlgoBase[CQLImpl, CQLConfig]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        policy = create_squashed_normal_policy(
+            observation_shape,
+            action_size,
+            self._config.actor_encoder_factory,
+            device=self._device,
+        )
+        q_func = create_continuous_q_function(
+            observation_shape,
+            action_size,
+            self._config.critic_encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
+        log_temp = create_parameter(
+            (1, 1),
+            math.log(self._config.initial_temperature),
+            device=self._device,
+        )
+        log_alpha = create_parameter(
+            (1, 1), math.log(self._config.initial_alpha), device=self._device
+        )
 
-    _actor_learning_rate: float
-    _critic_learning_rate: float
-    _temp_learning_rate: float
-    _alpha_learning_rate: float
-    _actor_optim_factory: OptimizerFactory
-    _critic_optim_factory: OptimizerFactory
-    _temp_optim_factory: OptimizerFactory
-    _alpha_optim_factory: OptimizerFactory
-    _actor_encoder_factory: EncoderFactory
-    _critic_encoder_factory: EncoderFactory
-    _q_func_factory: QFunctionFactory
-    _tau: float
-    _n_critics: int
-    _initial_temperature: float
-    _initial_alpha: float
-    _alpha_threshold: float
-    _conservative_weight: float
-    _n_action_samples: int
-    _soft_q_backup: bool
-    _use_gpu: Optional[Device]
-    _impl: Optional[CQLImpl]
-
-    def __init__(
-        self,
-        *,
-        actor_learning_rate: float = 1e-4,
-        critic_learning_rate: float = 3e-4,
-        temp_learning_rate: float = 1e-4,
-        alpha_learning_rate: float = 1e-4,
-        actor_optim_factory: OptimizerFactory = AdamFactory(),
-        critic_optim_factory: OptimizerFactory = AdamFactory(),
-        temp_optim_factory: OptimizerFactory = AdamFactory(),
-        alpha_optim_factory: OptimizerFactory = AdamFactory(),
-        actor_encoder_factory: EncoderArg = "default",
-        critic_encoder_factory: EncoderArg = "default",
-        q_func_factory: QFuncArg = "mean",
-        batch_size: int = 256,
-        n_frames: int = 1,
-        n_steps: int = 1,
-        gamma: float = 0.99,
-        tau: float = 0.005,
-        n_critics: int = 2,
-        initial_temperature: float = 1.0,
-        initial_alpha: float = 1.0,
-        alpha_threshold: float = 10.0,
-        conservative_weight: float = 5.0,
-        n_action_samples: int = 10,
-        soft_q_backup: bool = False,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        action_scaler: ActionScalerArg = None,
-        reward_scaler: RewardScalerArg = None,
-        impl: Optional[CQLImpl] = None,
-        **kwargs: Any,
-    ):
-        super().__init__(
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=n_steps,
-            gamma=gamma,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            reward_scaler=reward_scaler,
-            kwargs=kwargs,
-        )
-        self._actor_learning_rate = actor_learning_rate
-        self._critic_learning_rate = critic_learning_rate
-        self._temp_learning_rate = temp_learning_rate
-        self._alpha_learning_rate = alpha_learning_rate
-        self._actor_optim_factory = actor_optim_factory
-        self._critic_optim_factory = critic_optim_factory
-        self._temp_optim_factory = temp_optim_factory
-        self._alpha_optim_factory = alpha_optim_factory
-        self._actor_encoder_factory = check_encoder(actor_encoder_factory)
-        self._critic_encoder_factory = check_encoder(critic_encoder_factory)
-        self._q_func_factory = check_q_func(q_func_factory)
-        self._tau = tau
-        self._n_critics = n_critics
-        self._initial_temperature = initial_temperature
-        self._initial_alpha = initial_alpha
-        self._alpha_threshold = alpha_threshold
-        self._conservative_weight = conservative_weight
-        self._n_action_samples = n_action_samples
-        self._soft_q_backup = soft_q_backup
-        self._use_gpu = check_use_gpu(use_gpu)
-        self._impl = impl
+        actor_optim = self._config.actor_optim_factory.create(
+            policy.parameters(), lr=self._config.actor_learning_rate
+        )
+        critic_optim = self._config.critic_optim_factory.create(
+            q_func.parameters(), lr=self._config.critic_learning_rate
+        )
+        temp_optim = self._config.temp_optim_factory.create(
+            log_temp.parameters(), lr=self._config.temp_learning_rate
+        )
+        alpha_optim = self._config.alpha_optim_factory.create(
+            log_alpha.parameters(), lr=self._config.alpha_learning_rate
+        )
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
         self._impl = CQLImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            actor_learning_rate=self._actor_learning_rate,
-            critic_learning_rate=self._critic_learning_rate,
-            temp_learning_rate=self._temp_learning_rate,
-            alpha_learning_rate=self._alpha_learning_rate,
-            actor_optim_factory=self._actor_optim_factory,
-            critic_optim_factory=self._critic_optim_factory,
-            temp_optim_factory=self._temp_optim_factory,
-            alpha_optim_factory=self._alpha_optim_factory,
-            actor_encoder_factory=self._actor_encoder_factory,
-            critic_encoder_factory=self._critic_encoder_factory,
-            q_func_factory=self._q_func_factory,
-            gamma=self._gamma,
-            tau=self._tau,
-            n_critics=self._n_critics,
-            initial_temperature=self._initial_temperature,
-            initial_alpha=self._initial_alpha,
-            alpha_threshold=self._alpha_threshold,
-            conservative_weight=self._conservative_weight,
-            n_action_samples=self._n_action_samples,
-            soft_q_backup=self._soft_q_backup,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            action_scaler=self._action_scaler,
-            reward_scaler=self._reward_scaler,
+            policy=policy,
+            q_func=q_func,
+            log_temp=log_temp,
+            log_alpha=log_alpha,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            temp_optim=temp_optim,
+            alpha_optim=alpha_optim,
+            gamma=self._config.gamma,
+            tau=self._config.tau,
+            alpha_threshold=self._config.alpha_threshold,
+            conservative_weight=self._config.conservative_weight,
+            n_action_samples=self._config.n_action_samples,
+            soft_q_backup=self._config.soft_q_backup,
+            device=self._device,
         )
-        self._impl.build()
 
-    def _update(self, batch: TransitionMiniBatch) -> Dict[str, float]:
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
         assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
 
         metrics = {}
 
         # lagrangian parameter update for SAC temperature
-        if self._temp_learning_rate > 0:
+        if self._config.temp_learning_rate > 0:
             temp_loss, temp = self._impl.update_temp(batch)
             metrics.update({"temp_loss": temp_loss, "temp": temp})
 
         # lagrangian parameter update for conservative loss weight
-        if self._alpha_learning_rate > 0:
+        if self._config.alpha_learning_rate > 0:
             alpha_loss, alpha = self._impl.update_alpha(batch)
             metrics.update({"alpha_loss": alpha_loss, "alpha": alpha})
 
         critic_loss = self._impl.update_critic(batch)
         metrics.update({"critic_loss": critic_loss})
 
         actor_loss = self._impl.update_actor(batch)
@@ -257,16 +217,17 @@
 
         return metrics
 
     def get_action_type(self) -> ActionSpace:
         return ActionSpace.CONTINUOUS
 
 
-class DiscreteCQL(DoubleDQN):
-    r"""Discrete version of Conservative Q-Learning algorithm.
+@dataclasses.dataclass()
+class DiscreteCQLConfig(LearnableConfig):
+    r"""Config of Discrete version of Conservative Q-Learning algorithm.
 
     Discrete version of CQL is a DoubleDQN-based data-driven deep reinforcement
     learning algorithm (the original paper uses DQN), which achieves
     state-of-the-art performance in offline RL problems.
 
     CQL mitigates overestimation error by minimizing action-values under the
     current policy and maximizing values under data distribution for
@@ -280,94 +241,82 @@
             + L_{DoubleDQN}(\theta)
 
     References:
         * `Kumar et al., Conservative Q-Learning for Offline Reinforcement
           Learning. <https://arxiv.org/abs/2006.04779>`_
 
     Args:
-        learning_rate (float): learning rate.
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        learning_rate (float): Learning rate.
         optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory.
-        encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory.
-        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory or str):
+            Optimizer factory.
+        encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory.
+        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory):
             Q function factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        n_critics (int): the number of Q functions for ensemble.
-        target_update_interval (int): interval to synchronize the target
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        n_critics (int): Number of Q functions for ensemble.
+        target_update_interval (int): Interval to synchronize the target
             network.
-        alpha (float): the :math:`\alpha` value above.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`
-        reward_scaler (d3rlpy.preprocessing.RewardScaler or str):
-            reward preprocessor. The available options are
-            ``['clip', 'min_max', 'standard']``.
-        impl (d3rlpy.algos.torch.cql_impl.DiscreteCQLImpl):
-            algorithm implementation.
-
+        alpha (float): math:`\alpha` value above.
     """
+    learning_rate: float = 6.25e-5
+    optim_factory: OptimizerFactory = make_optimizer_field()
+    encoder_factory: EncoderFactory = make_encoder_field()
+    q_func_factory: QFunctionFactory = make_q_func_field()
+    batch_size: int = 32
+    gamma: float = 0.99
+    n_critics: int = 1
+    target_update_interval: int = 8000
+    alpha: float = 1.0
+
+    def create(self, device: DeviceArg = False) -> "DiscreteCQL":
+        return DiscreteCQL(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "discrete_cql"
+
+
+class DiscreteCQL(QLearningAlgoBase[DiscreteCQLImpl, DiscreteCQLConfig]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        q_func = create_discrete_q_function(
+            observation_shape,
+            action_size,
+            self._config.encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
 
-    _alpha: float
-    _impl: Optional[DiscreteCQLImpl]
-
-    def __init__(
-        self,
-        *,
-        learning_rate: float = 6.25e-5,
-        optim_factory: OptimizerFactory = AdamFactory(),
-        encoder_factory: EncoderArg = "default",
-        q_func_factory: QFuncArg = "mean",
-        batch_size: int = 32,
-        n_frames: int = 1,
-        n_steps: int = 1,
-        gamma: float = 0.99,
-        n_critics: int = 1,
-        target_update_interval: int = 8000,
-        alpha: float = 1.0,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        reward_scaler: RewardScalerArg = None,
-        impl: Optional[DiscreteCQLImpl] = None,
-        **kwargs: Any,
-    ):
-        super().__init__(
-            learning_rate=learning_rate,
-            optim_factory=optim_factory,
-            encoder_factory=encoder_factory,
-            q_func_factory=q_func_factory,
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=n_steps,
-            gamma=gamma,
-            n_critics=n_critics,
-            target_update_interval=target_update_interval,
-            use_gpu=use_gpu,
-            scaler=scaler,
-            reward_scaler=reward_scaler,
-            impl=impl,
-            **kwargs,
+        optim = self._config.optim_factory.create(
+            q_func.parameters(), lr=self._config.learning_rate
         )
-        self._alpha = alpha
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
         self._impl = DiscreteCQLImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            learning_rate=self._learning_rate,
-            optim_factory=self._optim_factory,
-            encoder_factory=self._encoder_factory,
-            q_func_factory=self._q_func_factory,
-            gamma=self._gamma,
-            n_critics=self._n_critics,
-            alpha=self._alpha,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            reward_scaler=self._reward_scaler,
+            q_func=q_func,
+            optim=optim,
+            gamma=self._config.gamma,
+            alpha=self._config.alpha,
+            device=self._device,
         )
-        self._impl.build()
+
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
+        assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
+        loss = self._impl.update(batch)
+        if self._grad_step % self._config.target_update_interval == 0:
+            self._impl.update_target()
+        return {"loss": loss}
+
+    def get_action_type(self) -> ActionSpace:
+        return ActionSpace.DISCRETE
+
+
+register_learnable(CQLConfig)
+register_learnable(DiscreteCQLConfig)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/crr.py` & `d3rlpy-2.0.2/d3rlpy/ope/fqe.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,247 +1,239 @@
-from typing import Any, Dict, Optional, Sequence
+import dataclasses
+from typing import Dict, Optional
 
-from ..argument_utility import (
-    ActionScalerArg,
-    EncoderArg,
-    QFuncArg,
-    RewardScalerArg,
-    ScalerArg,
-    UseGPUArg,
-    check_encoder,
-    check_q_func,
-    check_use_gpu,
+import numpy as np
+
+from ..algos.qlearning import QLearningAlgoBase, QLearningAlgoImplBase
+from ..base import DeviceArg, LearnableConfig, register_learnable
+from ..constants import (
+    ALGO_NOT_GIVEN_ERROR,
+    IMPL_NOT_INITIALIZED_ERROR,
+    ActionSpace,
+)
+from ..dataset import Observation, Shape
+from ..models.builders import (
+    create_continuous_q_function,
+    create_discrete_q_function,
 )
-from ..constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
-from ..dataset import TransitionMiniBatch
-from ..gpu import Device
-from ..models.encoders import EncoderFactory
-from ..models.optimizers import AdamFactory, OptimizerFactory
-from ..models.q_functions import QFunctionFactory
-from .base import AlgoBase
-from .torch.crr_impl import CRRImpl
+from ..models.encoders import EncoderFactory, make_encoder_field
+from ..models.optimizers import OptimizerFactory, make_optimizer_field
+from ..models.q_functions import QFunctionFactory, make_q_func_field
+from ..torch_utility import TorchMiniBatch, convert_to_torch
+from .torch.fqe_impl import DiscreteFQEImpl, FQEBaseImpl, FQEImpl
 
+__all__ = ["FQEConfig", "FQE", "DiscreteFQE"]
 
-class CRR(AlgoBase):
-    r"""Critic Reguralized Regression algorithm.
 
-    CRR is a simple offline RL method similar to AWAC.
+@dataclasses.dataclass()
+class FQEConfig(LearnableConfig):
+    r"""Config of Fitted Q Evaluation.
 
-    The policy is trained as a supervised regression.
+    FQE is an off-policy evaluation method that approximates a Q function
+    :math:`Q_\theta (s, a)` with the trained policy :math:`\pi_\phi(s)`.
 
     .. math::
 
-        J(\phi) = \mathbb{E}_{s_t, a_t \sim D}
-            [\log \pi_\phi(a_t|s_t) f(Q_\theta, \pi_\phi, s_t, a_t)]
+        L(\theta) = \mathbb{E}_{s_t, a_t, r_{t+1} s_{t+1} \sim D}
+            [(Q_\theta(s_t, a_t) - r_{t+1}
+                - \gamma Q_{\theta'}(s_{t+1}, \pi_\phi(s_{t+1})))^2]
 
-    where :math:`f` is a filter function which has several options. The first
-    option is ``binary`` function.
+    The trained Q function in FQE will estimate evaluation metrics more
+    accurately than learned Q function during training.
 
-    .. math::
+    References:
+        * `Le et al., Batch Policy Learning under Constraints.
+          <https://arxiv.org/abs/1903.08738>`_
 
-        f := \mathbb{1} [A_\theta(s, a) > 0]
+    Args:
+        algo (d3rlpy.algos.qlearning.base.QLearningAlgoBase):
+            Algorithm to evaluate.
+        learning_rate (float): Learning rate.
+        optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
+            Optimizer factory.
+        encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory.
+        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory):
+            Q function factory.
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        n_critics (int): Number of Q functions for ensemble.
+        target_update_interval (int): Interval to update the target network.
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        action_scaler (d3rlpy.preprocessing.ActionScaler): Action preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+    """
+    learning_rate: float = 1e-4
+    optim_factory: OptimizerFactory = make_optimizer_field()
+    encoder_factory: EncoderFactory = make_encoder_field()
+    q_func_factory: QFunctionFactory = make_q_func_field()
+    batch_size: int = 100
+    gamma: float = 0.99
+    n_critics: int = 1
+    target_update_interval: int = 100
+
+    def create(self, device: DeviceArg = False) -> "_FQEBase":
+        raise NotImplementedError(
+            "Config object must be directly given to constructor"
+        )
 
-    The other is ``exp`` function.
+    @staticmethod
+    def get_type() -> str:
+        return "fqe"
 
-    .. math::
 
-        f := \exp(A(s, a) / \beta)
+class _FQEBase(QLearningAlgoBase[FQEBaseImpl, FQEConfig]):
+    _algo: QLearningAlgoBase[QLearningAlgoImplBase, LearnableConfig]
+    _config: FQEConfig
+    _impl: Optional[FQEBaseImpl]
 
-    The :math:`A(s, a)` is an average function which also has several options.
-    The first option is ``mean``.
+    def __init__(
+        self,
+        algo: QLearningAlgoBase[QLearningAlgoImplBase, LearnableConfig],
+        config: FQEConfig,
+        device: DeviceArg = False,
+        impl: Optional[FQEBaseImpl] = None,
+    ):
+        super().__init__(config, device, impl)
+        self._algo = algo
 
-    .. math::
+    def save_policy(self, fname: str) -> None:
+        assert self._algo is not None, ALGO_NOT_GIVEN_ERROR
+        self._algo.save_policy(fname)
+
+    def predict(self, x: Observation) -> np.ndarray:
+        assert self._algo is not None, ALGO_NOT_GIVEN_ERROR
+        return self._algo.predict(x)
+
+    def sample_action(self, x: Observation) -> np.ndarray:
+        assert self._algo is not None, ALGO_NOT_GIVEN_ERROR
+        return self._algo.sample_action(x)
 
-        A(s, a) = Q_\theta (s, a) - \frac{1}{m} \sum^m_j Q(s, a_j)
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
+        assert self._algo is not None, ALGO_NOT_GIVEN_ERROR
+        assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
+        assert batch.numpy_batch
+        next_actions = self._algo.predict(batch.numpy_batch.next_observations)
+        loss = self._impl.update(
+            batch, convert_to_torch(next_actions, self._device)
+        )
+        if self._grad_step % self._config.target_update_interval == 0:
+            self._impl.update_target()
+        return {"loss": loss}
 
-    The other one is ``max``.
+    @property
+    def algo(self) -> QLearningAlgoBase[QLearningAlgoImplBase, LearnableConfig]:
+        return self._algo
 
-    .. math::
 
-        A(s, a) = Q_\theta (s, a) - \max^m_j Q(s, a_j)
+class FQE(_FQEBase):
+    r"""Fitted Q Evaluation.
+
+    FQE is an off-policy evaluation method that approximates a Q function
+    :math:`Q_\theta (s, a)` with the trained policy :math:`\pi_\phi(s)`.
+
+    .. math::
 
-    where :math:`a_j \sim \pi_\phi(s)`.
+        L(\theta) = \mathbb{E}_{s_t, a_t, r_{t+1} s_{t+1} \sim D}
+            [(Q_\theta(s_t, a_t) - r_{t+1}
+                - \gamma Q_{\theta'}(s_{t+1}, \pi_\phi(s_{t+1})))^2]
 
-    In evaluation, the action is determined by Critic Weighted Policy (CWP).
-    In CWP, the several actions are sampled from the policy function, and the
-    final action is re-sampled from the estimated action-value distribution.
+    The trained Q function in FQE will estimate evaluation metrics more
+    accurately than learned Q function during training.
 
     References:
-        * `Wang et al., Critic Reguralized Regression.
-          <https://arxiv.org/abs/2006.15134>`_
+        * `Le et al., Batch Policy Learning under Constraints.
+          <https://arxiv.org/abs/1903.08738>`_
 
     Args:
-        actor_learning_rate (float): learning rate for policy function.
-        critic_learning_rate (float): learning rate for Q functions.
-        actor_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the actor.
-        critic_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the critic.
-        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the actor.
-        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the critic.
-        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory or str):
-            Q function factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        beta (float): temperature value defined as :math:`\beta` above.
-        n_action_samples (int): the number of sampled actions to calculate
-            :math:`A(s, a)` and for CWP.
-        advantage_type (str): advantage function type. The available options
-            are ``['mean', 'max']``.
-        weight_type (str): filter function type. The available options
-            are ``['binary', 'exp']``.
-        max_weight (float): maximum weight for cross-entropy loss.
-        n_critics (int): the number of Q functions for ensemble.
-        target_update_type (str): target update type. The available options are
-            ``['hard', 'soft']``.
-        tau (float): target network synchronization coefficiency used with
-            ``soft`` target update.
-        update_actor_interval (int): interval to update policy function used
-            with ``hard`` target update.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`
-        action_scaler (d3rlpy.preprocessing.ActionScaler or str):
-            action preprocessor. The available options are ``['min_max']``.
-        reward_scaler (d3rlpy.preprocessing.RewardScaler or str):
-            reward preprocessor. The available options are
-            ``['clip', 'min_max', 'standard']``.
-        impl (d3rlpy.algos.torch.crr_impl.CRRImpl): algorithm implementation.
-
+        algo (d3rlpy.algos.base.AlgoBase): Algorithm to evaluate.
+        config (d3rlpy.ope.FQEConfig): FQE config.
+        device (bool, int or str):
+            Flag to use GPU, device ID or PyTorch device identifier.
+        impl (d3rlpy.metrics.ope.torch.FQEImpl): Algorithm implementation.
     """
 
-    _actor_learning_rate: float
-    _critic_learning_rate: float
-    _actor_optim_factory: OptimizerFactory
-    _critic_optim_factory: OptimizerFactory
-    _actor_encoder_factory: EncoderFactory
-    _critic_encoder_factory: EncoderFactory
-    _q_func_factory: QFunctionFactory
-    _beta: float
-    _n_action_samples: int
-    _advantage_type: str
-    _weight_type: str
-    _max_weight: float
-    _n_critics: int
-    _target_update_type: str
-    _tau: float
-    _target_update_interval: int
-    _update_actor_interval: int
-    _use_gpu: Optional[Device]
-    _impl: Optional[CRRImpl]
-
-    def __init__(
-        self,
-        *,
-        actor_learning_rate: float = 3e-4,
-        critic_learning_rate: float = 3e-4,
-        actor_optim_factory: OptimizerFactory = AdamFactory(),
-        critic_optim_factory: OptimizerFactory = AdamFactory(),
-        actor_encoder_factory: EncoderArg = "default",
-        critic_encoder_factory: EncoderArg = "default",
-        q_func_factory: QFuncArg = "mean",
-        batch_size: int = 100,
-        n_frames: int = 1,
-        n_steps: int = 1,
-        gamma: float = 0.99,
-        beta: float = 1.0,
-        n_action_samples: int = 4,
-        advantage_type: str = "mean",
-        weight_type: str = "exp",
-        max_weight: float = 20.0,
-        n_critics: int = 1,
-        target_update_type: str = "hard",
-        tau: float = 5e-3,
-        target_update_interval: int = 100,
-        update_actor_interval: int = 1,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        action_scaler: ActionScalerArg = None,
-        reward_scaler: RewardScalerArg = None,
-        impl: Optional[CRRImpl] = None,
-        **kwargs: Any,
-    ):
-        super().__init__(
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=n_steps,
-            gamma=gamma,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            reward_scaler=reward_scaler,
-            kwargs=kwargs,
-        )
-        self._actor_learning_rate = actor_learning_rate
-        self._critic_learning_rate = critic_learning_rate
-        self._actor_optim_factory = actor_optim_factory
-        self._critic_optim_factory = critic_optim_factory
-        self._actor_encoder_factory = check_encoder(actor_encoder_factory)
-        self._critic_encoder_factory = check_encoder(critic_encoder_factory)
-        self._q_func_factory = check_q_func(q_func_factory)
-        self._beta = beta
-        self._n_action_samples = n_action_samples
-        self._advantage_type = advantage_type
-        self._weight_type = weight_type
-        self._max_weight = max_weight
-        self._n_critics = n_critics
-        self._target_update_type = target_update_type
-        self._tau = tau
-        self._target_update_interval = target_update_interval
-        self._update_actor_interval = update_actor_interval
-        self._use_gpu = check_use_gpu(use_gpu)
-        self._impl = impl
-
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
     ) -> None:
-        self._impl = CRRImpl(
+        q_func = create_continuous_q_function(
+            observation_shape,
+            action_size,
+            self._config.encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
+        optim = self._config.optim_factory.create(
+            q_func.parameters(), lr=self._config.learning_rate
+        )
+        self._impl = FQEImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            actor_learning_rate=self._actor_learning_rate,
-            critic_learning_rate=self._critic_learning_rate,
-            actor_optim_factory=self._actor_optim_factory,
-            critic_optim_factory=self._critic_optim_factory,
-            actor_encoder_factory=self._actor_encoder_factory,
-            critic_encoder_factory=self._critic_encoder_factory,
-            q_func_factory=self._q_func_factory,
-            gamma=self._gamma,
-            beta=self._beta,
-            n_action_samples=self._n_action_samples,
-            advantage_type=self._advantage_type,
-            weight_type=self._weight_type,
-            max_weight=self._max_weight,
-            n_critics=self._n_critics,
-            tau=self._tau,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            action_scaler=self._action_scaler,
-            reward_scaler=self._reward_scaler,
+            q_func=q_func,
+            optim=optim,
+            gamma=self._config.gamma,
+            device=self._device,
         )
-        self._impl.build()
 
-    def _update(self, batch: TransitionMiniBatch) -> Dict[str, float]:
-        assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
+    def get_action_type(self) -> ActionSpace:
+        return ActionSpace.CONTINUOUS
 
-        critic_loss = self._impl.update_critic(batch)
-        actor_loss = self._impl.update_actor(batch)
 
-        if self._target_update_type == "hard":
-            if self._grad_step % self._target_update_interval == 0:
-                self._impl.sync_critic_target()
-                self._impl.sync_actor_target()
-        elif self._target_update_type == "soft":
-            self._impl.update_critic_target()
-            self._impl.update_actor_target()
-        else:
-            raise ValueError(
-                f"invalid target_update_type: {self._target_update_type}"
-            )
+class DiscreteFQE(_FQEBase):
+    r"""Fitted Q Evaluation for discrete action-space.
 
-        return {"critic_loss": critic_loss, "actor_loss": actor_loss}
+    FQE is an off-policy evaluation method that approximates a Q function
+    :math:`Q_\theta (s, a)` with the trained policy :math:`\pi_\phi(s)`.
+
+    .. math::
+
+        L(\theta) = \mathbb{E}_{s_t, a_t, r_{t+1} s_{t+1} \sim D}
+            [(Q_\theta(s_t, a_t) - r_{t+1}
+                - \gamma Q_{\theta'}(s_{t+1}, \pi_\phi(s_{t+1})))^2]
+
+    The trained Q function in FQE will estimate evaluation metrics more
+    accurately than learned Q function during training.
+
+    References:
+        * `Le et al., Batch Policy Learning under Constraints.
+          <https://arxiv.org/abs/1903.08738>`_
+
+    Args:
+        algo (d3rlpy.algos.qlearning.base.QLearningAlgoBase):
+            Algorithm to evaluate.
+        config (d3rlpy.ope.FQEConfig): FQE config.
+        device (bool, int or str):
+            Flag to use GPU, device ID or PyTorch device identifier.
+        impl (d3rlpy.metrics.ope.torch.DiscreteFQEImpl):
+            Algorithm implementation.
+    """
+
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        q_func = create_discrete_q_function(
+            observation_shape,
+            action_size,
+            self._config.encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
+        optim = self._config.optim_factory.create(
+            q_func.parameters(), lr=self._config.learning_rate
+        )
+        self._impl = DiscreteFQEImpl(
+            observation_shape=observation_shape,
+            action_size=action_size,
+            q_func=q_func,
+            optim=optim,
+            gamma=self._config.gamma,
+            device=self._device,
+        )
 
     def get_action_type(self) -> ActionSpace:
-        return ActionSpace.CONTINUOUS
+        return ActionSpace.DISCRETE
+
+
+register_learnable(FQEConfig)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/ddpg.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/bc.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,177 +1,185 @@
-from typing import Any, Dict, Optional, Sequence
+import dataclasses
+from typing import Dict, Generic, TypeVar
 
-from ..argument_utility import (
-    ActionScalerArg,
-    EncoderArg,
-    QFuncArg,
-    RewardScalerArg,
-    ScalerArg,
-    UseGPUArg,
-    check_encoder,
-    check_q_func,
-    check_use_gpu,
+from ...base import DeviceArg, LearnableConfig, register_learnable
+from ...constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
+from ...dataset import Shape
+from ...models.builders import (
+    create_deterministic_regressor,
+    create_discrete_imitator,
+    create_probablistic_regressor,
 )
-from ..constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
-from ..dataset import TransitionMiniBatch
-from ..gpu import Device
-from ..models.encoders import EncoderFactory
-from ..models.optimizers import AdamFactory, OptimizerFactory
-from ..models.q_functions import QFunctionFactory
-from .base import AlgoBase
-from .torch.ddpg_impl import DDPGImpl
+from ...models.encoders import EncoderFactory, make_encoder_field
+from ...models.optimizers import OptimizerFactory, make_optimizer_field
+from ...torch_utility import TorchMiniBatch
+from .base import QLearningAlgoBase
+from .torch.bc_impl import BCBaseImpl, BCImpl, DiscreteBCImpl
 
+__all__ = ["BCConfig", "BC", "DiscreteBCConfig", "DiscreteBC"]
 
-class DDPG(AlgoBase):
-    r"""Deep Deterministic Policy Gradients algorithm.
 
-    DDPG is an actor-critic algorithm that trains a Q function parametrized
-    with :math:`\theta` and a policy function parametrized with :math:`\phi`.
+TBCConfig = TypeVar("TBCConfig", bound="LearnableConfig")
+
+
+class _BCBase(Generic[TBCConfig], QLearningAlgoBase[BCBaseImpl, TBCConfig]):
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
+        assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
+        loss = self._impl.update_imitator(batch)
+        return {"loss": loss}
 
-    .. math::
 
-        L(\theta) = \mathbb{E}_{s_t,\, a_t,\, r_{t+1},\, s_{t+1} \sim D} \Big[(r_{t+1}
-            + \gamma Q_{\theta'}\big(s_{t+1}, \pi_{\phi'}(s_{t+1}))
-            - Q_\theta(s_t, a_t)\big)^2\Big]
+@dataclasses.dataclass()
+class BCConfig(LearnableConfig):
+    r"""Config of Behavior Cloning algorithm.
+
+    Behavior Cloning (BC) is to imitate actions in the dataset via a supervised
+    learning approach.
+    Since BC is only imitating action distributions, the performance will be
+    close to the mean of the dataset even though BC mostly works better than
+    online RL algorithms.
 
     .. math::
 
-        J(\phi) = \mathbb{E}_{s_t \sim D} \Big[Q_\theta\big(s_t, \pi_\phi(s_t)\big)\Big]
+        L(\theta) = \mathbb{E}_{a_t, s_t \sim D}
+            [(a_t - \pi_\theta(s_t))^2]
 
-    where :math:`\theta'` and :math:`\phi` are the target network parameters.
-    There target network parameters are updated every iteration.
+    Args:
+        learning_rate (float): Learing rate.
+        optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
+            Optimizer factory.
+        encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory.
+        batch_size (int): Mini-batch size.
+        policy_type (str): the policy type. Available options are
+            ``['deterministic', 'stochastic']``.
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        action_scaler (d3rlpy.preprocessing.ActionScaler): Action preprocessor.
+    """
+    batch_size: int = 100
+    learning_rate: float = 1e-3
+    policy_type: str = "deterministic"
+    optim_factory: OptimizerFactory = make_optimizer_field()
+    encoder_factory: EncoderFactory = make_encoder_field()
+
+    def create(self, device: DeviceArg = False) -> "BC":
+        return BC(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "bc"
+
+
+class BC(_BCBase[BCConfig]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        if self._config.policy_type == "deterministic":
+            imitator = create_deterministic_regressor(
+                observation_shape,
+                action_size,
+                self._config.encoder_factory,
+                device=self._device,
+            )
+        elif self._config.policy_type == "stochastic":
+            imitator = create_probablistic_regressor(
+                observation_shape,
+                action_size,
+                self._config.encoder_factory,
+                min_logstd=-4.0,
+                max_logstd=15.0,
+                device=self._device,
+            )
+        else:
+            raise ValueError(f"invalid policy_type: {self._config.policy_type}")
 
-    .. math::
+        optim = self._config.optim_factory.create(
+            imitator.parameters(), lr=self._config.learning_rate
+        )
 
-        \theta' \gets \tau \theta + (1 - \tau) \theta'
+        self._impl = BCImpl(
+            observation_shape=observation_shape,
+            action_size=action_size,
+            imitator=imitator,
+            optim=optim,
+            policy_type=self._config.policy_type,
+            device=self._device,
+        )
 
-        \phi' \gets \tau \phi + (1 - \tau) \phi'
+    def get_action_type(self) -> ActionSpace:
+        return ActionSpace.CONTINUOUS
 
-    References:
-        * `Silver et al., Deterministic policy gradient algorithms.
-          <http://proceedings.mlr.press/v32/silver14.html>`_
-        * `Lillicrap et al., Continuous control with deep reinforcement
-          learning. <https://arxiv.org/abs/1509.02971>`_
 
-    Args:
-        actor_learning_rate (float): learning rate for policy function.
-        critic_learning_rate (float): learning rate for Q function.
-        actor_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the actor.
-        critic_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the critic.
-        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the actor.
-        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the critic.
-        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory or str):
-            Q function factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        tau (float): target network synchronization coefficiency.
-        n_critics (int): the number of Q functions for ensemble.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`
-        action_scaler (d3rlpy.preprocessing.ActionScaler or str):
-            action preprocessor. The available options are ``['min_max']``.
-        reward_scaler (d3rlpy.preprocessing.RewardScaler or str):
-            reward preprocessor. The available options are
-            ``['clip', 'min_max', 'standard']``.
-        impl (d3rlpy.algos.torch.ddpg_impl.DDPGImpl): algorithm implementation.
+@dataclasses.dataclass()
+class DiscreteBCConfig(LearnableConfig):
+    r"""Config of Behavior Cloning algorithm for discrete control.
+
+    Behavior Cloning (BC) is to imitate actions in the dataset via a supervised
+    learning approach.
+    Since BC is only imitating action distributions, the performance will be
+    close to the mean of the dataset even though BC mostly works better than
+    online RL algorithms.
+
+    .. math::
+
+        L(\theta) = \mathbb{E}_{a_t, s_t \sim D}
+            [-\sum_a p(a|s_t) \log \pi_\theta(a|s_t)]
 
+    where :math:`p(a|s_t)` is implemented as a one-hot vector.
+
+    Args:
+        learning_rate (float): Learing rate.
+        optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
+            Optimizer factory.
+        encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory.
+        batch_size (int): Mini-batch size.
+        beta (float): Reguralization factor.
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
     """
+    batch_size: int = 100
+    learning_rate: float = 1e-3
+    optim_factory: OptimizerFactory = make_optimizer_field()
+    encoder_factory: EncoderFactory = make_encoder_field()
+    beta: float = 0.5
+
+    def create(self, device: DeviceArg = False) -> "DiscreteBC":
+        return DiscreteBC(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "discrete_bc"
+
+
+class DiscreteBC(_BCBase[DiscreteBCConfig]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        imitator = create_discrete_imitator(
+            observation_shape,
+            action_size,
+            self._config.beta,
+            self._config.encoder_factory,
+            device=self._device,
+        )
 
-    _actor_learning_rate: float
-    _critic_learning_rate: float
-    _actor_optim_factory: OptimizerFactory
-    _critic_optim_factory: OptimizerFactory
-    _actor_encoder_factory: EncoderFactory
-    _critic_encoder_factory: EncoderFactory
-    _q_func_factory: QFunctionFactory
-    _tau: float
-    _n_critics: int
-    _use_gpu: Optional[Device]
-    _impl: Optional[DDPGImpl]
-
-    def __init__(
-        self,
-        *,
-        actor_learning_rate: float = 3e-4,
-        critic_learning_rate: float = 3e-4,
-        actor_optim_factory: OptimizerFactory = AdamFactory(),
-        critic_optim_factory: OptimizerFactory = AdamFactory(),
-        actor_encoder_factory: EncoderArg = "default",
-        critic_encoder_factory: EncoderArg = "default",
-        q_func_factory: QFuncArg = "mean",
-        batch_size: int = 100,
-        n_frames: int = 1,
-        n_steps: int = 1,
-        gamma: float = 0.99,
-        tau: float = 0.005,
-        n_critics: int = 1,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        action_scaler: ActionScalerArg = None,
-        reward_scaler: RewardScalerArg = None,
-        impl: Optional[DDPGImpl] = None,
-        **kwargs: Any
-    ):
-        super().__init__(
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=n_steps,
-            gamma=gamma,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            reward_scaler=reward_scaler,
-            kwargs=kwargs,
+        optim = self._config.optim_factory.create(
+            imitator.parameters(), lr=self._config.learning_rate
         )
-        self._actor_learning_rate = actor_learning_rate
-        self._critic_learning_rate = critic_learning_rate
-        self._actor_optim_factory = actor_optim_factory
-        self._critic_optim_factory = critic_optim_factory
-        self._actor_encoder_factory = check_encoder(actor_encoder_factory)
-        self._critic_encoder_factory = check_encoder(critic_encoder_factory)
-        self._q_func_factory = check_q_func(q_func_factory)
-        self._tau = tau
-        self._n_critics = n_critics
-        self._use_gpu = check_use_gpu(use_gpu)
-        self._impl = impl
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
-        self._impl = DDPGImpl(
+        self._impl = DiscreteBCImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            actor_learning_rate=self._actor_learning_rate,
-            critic_learning_rate=self._critic_learning_rate,
-            actor_optim_factory=self._actor_optim_factory,
-            critic_optim_factory=self._critic_optim_factory,
-            actor_encoder_factory=self._actor_encoder_factory,
-            critic_encoder_factory=self._critic_encoder_factory,
-            q_func_factory=self._q_func_factory,
-            gamma=self._gamma,
-            tau=self._tau,
-            n_critics=self._n_critics,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            action_scaler=self._action_scaler,
-            reward_scaler=self._reward_scaler,
+            imitator=imitator,
+            optim=optim,
+            beta=self._config.beta,
+            device=self._device,
         )
-        self._impl.build()
 
-    def _update(self, batch: TransitionMiniBatch) -> Dict[str, float]:
-        assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
-        critic_loss = self._impl.update_critic(batch)
-        actor_loss = self._impl.update_actor(batch)
-        self._impl.update_critic_target()
-        self._impl.update_actor_target()
+    def get_action_type(self) -> ActionSpace:
+        return ActionSpace.DISCRETE
 
-        return {"critic_loss": critic_loss, "actor_loss": actor_loss}
 
-    def get_action_type(self) -> ActionSpace:
-        return ActionSpace.CONTINUOUS
+register_learnable(BCConfig)
+register_learnable(DiscreteBCConfig)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/dqn.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/dqn.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,146 +1,113 @@
-from typing import Any, Dict, Optional, Sequence
+import dataclasses
+from typing import Dict
 
-from ..argument_utility import (
-    EncoderArg,
-    QFuncArg,
-    RewardScalerArg,
-    ScalerArg,
-    UseGPUArg,
-    check_encoder,
-    check_q_func,
-    check_use_gpu,
-)
-from ..constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
-from ..dataset import TransitionMiniBatch
-from ..gpu import Device
-from ..models.encoders import EncoderFactory
-from ..models.optimizers import AdamFactory, OptimizerFactory
-from ..models.q_functions import QFunctionFactory
-from .base import AlgoBase
+from ...base import DeviceArg, LearnableConfig, register_learnable
+from ...constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
+from ...dataset import Shape
+from ...models.builders import create_discrete_q_function
+from ...models.encoders import EncoderFactory, make_encoder_field
+from ...models.optimizers import OptimizerFactory, make_optimizer_field
+from ...models.q_functions import QFunctionFactory, make_q_func_field
+from ...torch_utility import TorchMiniBatch
+from .base import QLearningAlgoBase
 from .torch.dqn_impl import DoubleDQNImpl, DQNImpl
 
+__all__ = ["DQNConfig", "DQN", "DoubleDQNConfig", "DoubleDQN"]
 
-class DQN(AlgoBase):
-    r"""Deep Q-Network algorithm.
+
+@dataclasses.dataclass()
+class DQNConfig(LearnableConfig):
+    r"""Config of Deep Q-Network algorithm.
 
     .. math::
 
         L(\theta) = \mathbb{E}_{s_t, a_t, r_{t+1}, s_{t+1} \sim D} [(r_{t+1}
             + \gamma \max_a Q_{\theta'}(s_{t+1}, a) - Q_\theta(s_t, a_t))^2]
 
     where :math:`\theta'` is the target network parameter. The target network
     parameter is synchronized every `target_update_interval` iterations.
 
     References:
         * `Mnih et al., Human-level control through deep reinforcement
           learning. <https://www.nature.com/articles/nature14236>`_
 
     Args:
-        learning_rate (float): learning rate.
-        optim_factory (d3rlpy.models.optimizers.OptimizerFactory or str):
-            optimizer factory.
-        encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory.
-        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory or str):
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        learning_rate (float): Learning rate.
+        optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
+            Optimizer factory.
+        encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory.
+        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory):
             Q function factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        n_critics (int): the number of Q functions for ensemble.
-        target_update_interval (int): interval to update the target network.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`
-        reward_scaler (d3rlpy.preprocessing.RewardScaler or str):
-            reward preprocessor. The available options are
-            ``['clip', 'min_max', 'standard']``.
-        impl (d3rlpy.algos.torch.dqn_impl.DQNImpl): algorithm implementation.
-
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        n_critics (int): Number of Q functions for ensemble.
+        target_update_interval (int): Interval to update the target network.
     """
+    batch_size: int = 32
+    learning_rate: float = 6.25e-5
+    optim_factory: OptimizerFactory = make_optimizer_field()
+    encoder_factory: EncoderFactory = make_encoder_field()
+    q_func_factory: QFunctionFactory = make_q_func_field()
+    gamma: float = 0.99
+    n_critics: int = 1
+    target_update_interval: int = 8000
+
+    def create(self, device: DeviceArg = False) -> "DQN":
+        return DQN(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "dqn"
+
+
+class DQN(QLearningAlgoBase[DQNImpl, DQNConfig]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        q_func = create_discrete_q_function(
+            observation_shape,
+            action_size,
+            self._config.encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
 
-    _learning_rate: float
-    _optim_factory: OptimizerFactory
-    _encoder_factory: EncoderFactory
-    _q_func_factory: QFunctionFactory
-    _n_critics: int
-    _target_update_interval: int
-    _use_gpu: Optional[Device]
-    _impl: Optional[DQNImpl]
-
-    def __init__(
-        self,
-        *,
-        learning_rate: float = 6.25e-5,
-        optim_factory: OptimizerFactory = AdamFactory(),
-        encoder_factory: EncoderArg = "default",
-        q_func_factory: QFuncArg = "mean",
-        batch_size: int = 32,
-        n_frames: int = 1,
-        n_steps: int = 1,
-        gamma: float = 0.99,
-        n_critics: int = 1,
-        target_update_interval: int = 8000,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        reward_scaler: RewardScalerArg = None,
-        impl: Optional[DQNImpl] = None,
-        **kwargs: Any,
-    ):
-        super().__init__(
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=n_steps,
-            gamma=gamma,
-            scaler=scaler,
-            reward_scaler=reward_scaler,
-            kwargs=kwargs,
-        )
-        self._learning_rate = learning_rate
-        self._optim_factory = optim_factory
-        self._encoder_factory = check_encoder(encoder_factory)
-        self._q_func_factory = check_q_func(q_func_factory)
-        self._n_critics = n_critics
-        self._target_update_interval = target_update_interval
-        self._use_gpu = check_use_gpu(use_gpu)
-        self._impl = impl
+        optim = self._config.optim_factory.create(
+            q_func.parameters(), lr=self._config.learning_rate
+        )
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
         self._impl = DQNImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            learning_rate=self._learning_rate,
-            optim_factory=self._optim_factory,
-            encoder_factory=self._encoder_factory,
-            q_func_factory=self._q_func_factory,
-            gamma=self._gamma,
-            n_critics=self._n_critics,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            reward_scaler=self._reward_scaler,
+            q_func=q_func,
+            optim=optim,
+            gamma=self._config.gamma,
+            device=self._device,
         )
-        self._impl.build()
 
-    def _update(self, batch: TransitionMiniBatch) -> Dict[str, float]:
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
         assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
         loss = self._impl.update(batch)
-        if self._grad_step % self._target_update_interval == 0:
+        if self._grad_step % self._config.target_update_interval == 0:
             self._impl.update_target()
         return {"loss": loss}
 
     def get_action_type(self) -> ActionSpace:
         return ActionSpace.DISCRETE
 
 
-class DoubleDQN(DQN):
-    r"""Double Deep Q-Network algorithm.
+@dataclasses.dataclass()
+class DoubleDQNConfig(DQNConfig):
+    r"""Config of Double Deep Q-Network algorithm.
 
     The difference from DQN is that the action is taken from the current Q
     function instead of the target Q function.
     This modification significantly decreases overestimation bias of TD
     learning.
 
     .. math::
@@ -153,49 +120,69 @@
     parameter is synchronized every `target_update_interval` iterations.
 
     References:
         * `Hasselt et al., Deep reinforcement learning with double Q-learning.
           <https://arxiv.org/abs/1509.06461>`_
 
     Args:
-        learning_rate (float): learning rate.
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        learning_rate (float): Learning rate.
         optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory.
-        encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory.
-        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory or str):
+            Optimizer factory.
+        encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory.
+        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory):
             Q function factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        n_critics (int): the number of Q functions.
-        target_update_interval (int): interval to synchronize the target
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        n_critics (int): Number of Q functions.
+        target_update_interval (int): Interval to synchronize the target
             network.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`
-        impl (d3rlpy.algos.torch.dqn_impl.DoubleDQNImpl):
-            algorithm implementation.
-
     """
+    batch_size: int = 32
+    learning_rate: float = 6.25e-5
+    optim_factory: OptimizerFactory = make_optimizer_field()
+    encoder_factory: EncoderFactory = make_encoder_field()
+    q_func_factory: QFunctionFactory = make_q_func_field()
+    gamma: float = 0.99
+    n_critics: int = 1
+    target_update_interval: int = 8000
+
+    def create(self, device: DeviceArg = False) -> "DoubleDQN":
+        return DoubleDQN(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "double_dqn"
 
-    _impl: Optional[DoubleDQNImpl]
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
+class DoubleDQN(DQN):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
     ) -> None:
+        q_func = create_discrete_q_function(
+            observation_shape,
+            action_size,
+            self._config.encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
+
+        optim = self._config.optim_factory.create(
+            q_func.parameters(), lr=self._config.learning_rate
+        )
+
         self._impl = DoubleDQNImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            learning_rate=self._learning_rate,
-            optim_factory=self._optim_factory,
-            encoder_factory=self._encoder_factory,
-            q_func_factory=self._q_func_factory,
-            gamma=self._gamma,
-            n_critics=self._n_critics,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            reward_scaler=self._reward_scaler,
+            q_func=q_func,
+            optim=optim,
+            gamma=self._config.gamma,
+            device=self._device,
         )
-        self._impl.build()
+
+
+register_learnable(DQNConfig)
+register_learnable(DoubleDQNConfig)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/iql.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/iql.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,30 @@
-from typing import Any, Dict, Optional, Sequence
+import dataclasses
+from typing import Dict
 
-from ..argument_utility import (
-    ActionScalerArg,
-    EncoderArg,
-    RewardScalerArg,
-    ScalerArg,
-    UseGPUArg,
-    check_encoder,
-    check_use_gpu,
+from ...base import DeviceArg, LearnableConfig, register_learnable
+from ...constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
+from ...dataset import Shape
+from ...models.builders import (
+    create_continuous_q_function,
+    create_non_squashed_normal_policy,
+    create_value_function,
 )
-from ..constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
-from ..dataset import TransitionMiniBatch
-from ..gpu import Device
-from ..models.encoders import EncoderFactory
-from ..models.optimizers import AdamFactory, OptimizerFactory
-from .base import AlgoBase
+from ...models.encoders import EncoderFactory, make_encoder_field
+from ...models.optimizers import OptimizerFactory, make_optimizer_field
+from ...models.q_functions import MeanQFunctionFactory
+from ...torch_utility import TorchMiniBatch
+from .base import QLearningAlgoBase
 from .torch.iql_impl import IQLImpl
 
+__all__ = ["IQLConfig", "IQL"]
 
-class IQL(AlgoBase):
+
+@dataclasses.dataclass()
+class IQLConfig(LearnableConfig):
     r"""Implicit Q-Learning algorithm.
 
     IQL is the offline RL algorithm that avoids ever querying values of unseen
     actions while still being able to perform multi-step dynamic programming
     updates.
 
     There are three functions to train in IQL. First the state-value function
@@ -36,15 +38,15 @@
     where :math:`L_2^\tau (u) = |\tau - \mathbb{1}(u < 0)|u^2`.
 
     The Q-function is trained with the state-value function to avoid query the
     actions.
 
     .. math::
 
-        L_Q(\theta) = \mathbb{E}_{(s, a, r, a') \sim D}
+        L_Q(\theta) = \mathbb{E}_{(s, a, r, s') \sim D}
             [(r + \gamma V_\psi(s') - Q_\theta(s, a))^2]
 
     Finally, the policy function is trained by using advantage weighted
     regression.
 
     .. math::
 
@@ -52,151 +54,129 @@
             [\exp(\beta (Q_\theta - V_\psi(s))) \log \pi_\phi(a|s)]
 
     References:
         * `Kostrikov et al., Offline Reinforcement Learning with Implicit
           Q-Learning. <https://arxiv.org/abs/2110.06169>`_
 
     Args:
-        actor_learning_rate (float): learning rate for policy function.
-        critic_learning_rate (float): learning rate for Q functions.
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        action_scaler (d3rlpy.preprocessing.ActionScaler): Action preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        actor_learning_rate (float): Learning rate for policy function.
+        critic_learning_rate (float): Learning rate for Q functions.
         actor_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the actor.
+            Optimizer factory for the actor.
         critic_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the critic.
-        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the actor.
-        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the critic.
-        value_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the value function.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        tau (float): target network synchronization coefficiency.
-        n_critics (int): the number of Q functions for ensemble.
-        expectile (float): the expectile value for value function training.
-        weight_temp (float): inverse temperature value represented as
+            Optimizer factory for the critic.
+        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the actor.
+        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the critic.
+        value_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the value function.
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        tau (float): Target network synchronization coefficiency.
+        n_critics (int): Number of Q functions for ensemble.
+        expectile (float): Expectile value for value function training.
+        weight_temp (float): Inverse temperature value represented as
             :math:`\beta`.
-        max_weight (float): the maximum advantage weight value to clip.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`.
-        action_scaler (d3rlpy.preprocessing.ActionScaler or str):
-            action preprocessor. The available options are ``['min_max']``.
-        reward_scaler (d3rlpy.preprocessing.RewardScaler or str):
-            reward preprocessor. The available options are
-            ``['clip', 'min_max', 'standard']``.
-        impl (d3rlpy.algos.torch.iql_impl.IQLImpl): algorithm implementation.
-
+        max_weight (float): Maximum advantage weight value to clip.
     """
+    actor_learning_rate: float = 3e-4
+    critic_learning_rate: float = 3e-4
+    actor_optim_factory: OptimizerFactory = make_optimizer_field()
+    critic_optim_factory: OptimizerFactory = make_optimizer_field()
+    actor_encoder_factory: EncoderFactory = make_encoder_field()
+    critic_encoder_factory: EncoderFactory = make_encoder_field()
+    value_encoder_factory: EncoderFactory = make_encoder_field()
+    batch_size: int = 256
+    gamma: float = 0.99
+    tau: float = 0.005
+    n_critics: int = 2
+    expectile: float = 0.7
+    weight_temp: float = 3.0
+    max_weight: float = 100.0
+
+    def create(self, device: DeviceArg = False) -> "IQL":
+        return IQL(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "iql"
+
+
+class IQL(QLearningAlgoBase[IQLImpl, IQLConfig]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        policy = create_non_squashed_normal_policy(
+            observation_shape,
+            action_size,
+            self._config.actor_encoder_factory,
+            min_logstd=-5.0,
+            max_logstd=2.0,
+            use_std_parameter=True,
+            device=self._device,
+        )
+        q_func = create_continuous_q_function(
+            observation_shape,
+            action_size,
+            self._config.critic_encoder_factory,
+            MeanQFunctionFactory(),
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
+        value_func = create_value_function(
+            observation_shape,
+            self._config.value_encoder_factory,
+            device=self._device,
+        )
 
-    _actor_learning_rate: float
-    _critic_learning_rate: float
-    _actor_optim_factory: OptimizerFactory
-    _critic_optim_factory: OptimizerFactory
-    _actor_encoder_factory: EncoderFactory
-    _critic_encoder_factory: EncoderFactory
-    _value_encoder_factory: EncoderFactory
-    _tau: float
-    _n_critics: int
-    _expectile: float
-    _weight_temp: float
-    _max_weight: float
-    _use_gpu: Optional[Device]
-    _impl: Optional[IQLImpl]
-
-    def __init__(
-        self,
-        *,
-        actor_learning_rate: float = 3e-4,
-        critic_learning_rate: float = 3e-4,
-        actor_optim_factory: OptimizerFactory = AdamFactory(),
-        critic_optim_factory: OptimizerFactory = AdamFactory(),
-        actor_encoder_factory: EncoderArg = "default",
-        critic_encoder_factory: EncoderArg = "default",
-        value_encoder_factory: EncoderArg = "default",
-        batch_size: int = 256,
-        n_frames: int = 1,
-        n_steps: int = 1,
-        gamma: float = 0.99,
-        tau: float = 0.005,
-        n_critics: int = 2,
-        expectile: float = 0.7,
-        weight_temp: float = 3.0,
-        max_weight: float = 100.0,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        action_scaler: ActionScalerArg = None,
-        reward_scaler: RewardScalerArg = None,
-        impl: Optional[IQLImpl] = None,
-        **kwargs: Any,
-    ):
-        super().__init__(
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=n_steps,
-            gamma=gamma,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            reward_scaler=reward_scaler,
-            kwargs=kwargs,
-        )
-        self._actor_learning_rate = actor_learning_rate
-        self._critic_learning_rate = critic_learning_rate
-        self._actor_optim_factory = actor_optim_factory
-        self._critic_optim_factory = critic_optim_factory
-        self._actor_encoder_factory = check_encoder(actor_encoder_factory)
-        self._critic_encoder_factory = check_encoder(critic_encoder_factory)
-        self._value_encoder_factory = check_encoder(value_encoder_factory)
-        self._tau = tau
-        self._n_critics = n_critics
-        self._expectile = expectile
-        self._weight_temp = weight_temp
-        self._max_weight = max_weight
-        self._use_gpu = check_use_gpu(use_gpu)
-        self._impl = impl
+        actor_optim = self._config.actor_optim_factory.create(
+            policy.parameters(), lr=self._config.actor_learning_rate
+        )
+        q_func_params = list(q_func.parameters())
+        v_func_params = list(value_func.parameters())
+        critic_optim = self._config.critic_optim_factory.create(
+            q_func_params + v_func_params, lr=self._config.critic_learning_rate
+        )
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
         self._impl = IQLImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            actor_learning_rate=self._actor_learning_rate,
-            critic_learning_rate=self._critic_learning_rate,
-            actor_optim_factory=self._actor_optim_factory,
-            critic_optim_factory=self._critic_optim_factory,
-            actor_encoder_factory=self._actor_encoder_factory,
-            critic_encoder_factory=self._critic_encoder_factory,
-            value_encoder_factory=self._value_encoder_factory,
-            gamma=self._gamma,
-            tau=self._tau,
-            n_critics=self._n_critics,
-            expectile=self._expectile,
-            weight_temp=self._weight_temp,
-            max_weight=self._max_weight,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            action_scaler=self._action_scaler,
-            reward_scaler=self._reward_scaler,
+            policy=policy,
+            q_func=q_func,
+            value_func=value_func,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            gamma=self._config.gamma,
+            tau=self._config.tau,
+            expectile=self._config.expectile,
+            weight_temp=self._config.weight_temp,
+            max_weight=self._config.max_weight,
+            device=self._device,
         )
-        self._impl.build()
 
-    def _update(self, batch: TransitionMiniBatch) -> Dict[str, float]:
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
         assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
 
         metrics = {}
 
-        critic_loss, value_loss = self._impl.update_critic(batch)
+        critic_loss, value_loss = self._impl.update_critic_and_state_value(
+            batch
+        )
         metrics.update({"critic_loss": critic_loss, "value_loss": value_loss})
 
         actor_loss = self._impl.update_actor(batch)
         metrics.update({"actor_loss": actor_loss})
 
         self._impl.update_critic_target()
 
         return metrics
 
     def get_action_type(self) -> ActionSpace:
         return ActionSpace.CONTINUOUS
+
+
+register_learnable(IQLConfig)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/nfq.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/awac.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,134 +1,160 @@
-from typing import Any, Dict, Optional, Sequence
+import dataclasses
+from typing import Dict
 
-from ..argument_utility import (
-    EncoderArg,
-    QFuncArg,
-    RewardScalerArg,
-    ScalerArg,
-    UseGPUArg,
-    check_encoder,
-    check_q_func,
-    check_use_gpu,
+from ...base import DeviceArg, LearnableConfig, register_learnable
+from ...constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
+from ...dataset import Shape
+from ...models.builders import (
+    create_continuous_q_function,
+    create_non_squashed_normal_policy,
 )
-from ..constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
-from ..dataset import TransitionMiniBatch
-from ..gpu import Device
-from ..models.encoders import EncoderFactory
-from ..models.optimizers import AdamFactory, OptimizerFactory
-from ..models.q_functions import QFunctionFactory
-from .base import AlgoBase
-from .torch.dqn_impl import DQNImpl
+from ...models.encoders import EncoderFactory, make_encoder_field
+from ...models.optimizers import OptimizerFactory, make_optimizer_field
+from ...models.q_functions import QFunctionFactory, make_q_func_field
+from ...torch_utility import TorchMiniBatch
+from .base import QLearningAlgoBase
+from .torch.awac_impl import AWACImpl
 
+__all__ = ["AWACConfig", "AWAC"]
 
-class NFQ(AlgoBase):
-    r"""Neural Fitted Q Iteration algorithm.
 
-    This NFQ implementation in d3rlpy is practically same as DQN, but excluding
-    the target network mechanism.
+@dataclasses.dataclass()
+class AWACConfig(LearnableConfig):
+    r"""Config of Advantage Weighted Actor-Critic algorithm.
+
+    AWAC is a TD3-based actor-critic algorithm that enables efficient
+    fine-tuning where the policy is trained with offline datasets and is
+    deployed to online training.
+
+    The policy is trained as a supervised regression.
 
     .. math::
 
-        L(\theta) = \mathbb{E}_{s_t, a_t, r_{t+1}, s_{t+1} \sim D} [(r_{t+1}
-            + \gamma \max_a Q_{\theta'}(s_{t+1}, a) - Q_\theta(s_t, a_t))^2]
+        J(\phi) = \mathbb{E}_{s_t, a_t \sim D}
+            [\log \pi_\phi(a_t|s_t)
+                \exp(\frac{1}{\lambda} A^\pi (s_t, a_t))]
 
-    where :math:`\theta'` is the target network parameter. The target network
-    parameter is synchronized every `target_update_interval` iterations.
+    where :math:`A^\pi (s_t, a_t) = Q_\theta(s_t, a_t) -
+    Q_\theta(s_t, a'_t)` and :math:`a'_t \sim \pi_\phi(\cdot|s_t)`
+
+    The key difference from AWR is that AWAC uses Q-function trained via TD
+    learning for the better sample-efficiency.
 
     References:
-        * `Riedmiller., Neural Fitted Q Iteration - first experiences with a
-          data efficient neural reinforcement learning method.
-          <https://link.springer.com/chapter/10.1007/11564096_32>`_
+        * `Nair et al., Accelerating Online Reinforcement Learning with Offline
+          Datasets. <https://arxiv.org/abs/2006.09359>`_
 
     Args:
-        learning_rate (float): learning rate.
-        optim_factory (d3rlpy.models.optimizers.OptimizerFactory or str):
-            optimizer factory.
-        encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory.
-        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory or str):
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        action_scaler (d3rlpy.preprocessing.ActionScaler): Action preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        actor_learning_rate (float): Learning rate for policy function.
+        critic_learning_rate (float): Learning rate for Q functions.
+        actor_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
+            Optimizer factory for the actor.
+        critic_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
+            Optimizer factory for the critic.
+        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the actor.
+        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the critic.
+        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory):
             Q function factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        n_critics (int): the number of Q functions for ensemble.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`
-        reward_scaler (d3rlpy.preprocessing.RewardScaler or str):
-            reward preprocessor. The available options are
-            ``['clip', 'min_max', 'standard']``.
-        impl (d3rlpy.algos.torch.dqn_impl.DQNImpl): algorithm implementation.
-
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        tau (float): Target network synchronization coefficiency.
+        lam (float): :math:`\lambda` for weight calculation.
+        n_action_samples (int): Number of sampled actions to calculate
+            :math:`A^\pi(s_t, a_t)`.
+        n_critics (int): Number of Q functions for ensemble.
+        update_actor_interval (int): Interval to update policy function.
     """
+    actor_learning_rate: float = 3e-4
+    critic_learning_rate: float = 3e-4
+    actor_optim_factory: OptimizerFactory = make_optimizer_field()
+    critic_optim_factory: OptimizerFactory = make_optimizer_field()
+    actor_encoder_factory: EncoderFactory = make_encoder_field()
+    critic_encoder_factory: EncoderFactory = make_encoder_field()
+    q_func_factory: QFunctionFactory = make_q_func_field()
+    batch_size: int = 1024
+    gamma: float = 0.99
+    tau: float = 0.005
+    lam: float = 1.0
+    n_action_samples: int = 1
+    n_critics: int = 2
+    update_actor_interval: int = 1
+
+    def create(self, device: DeviceArg = False) -> "AWAC":
+        return AWAC(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "awac"
+
+
+class AWAC(QLearningAlgoBase[AWACImpl, AWACConfig]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        policy = create_non_squashed_normal_policy(
+            observation_shape,
+            action_size,
+            self._config.actor_encoder_factory,
+            min_logstd=-6.0,
+            max_logstd=0.0,
+            use_std_parameter=True,
+            device=self._device,
+        )
+        q_func = create_continuous_q_function(
+            observation_shape,
+            action_size,
+            self._config.critic_encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
 
-    _learning_rate: float
-    _optim_factory: OptimizerFactory
-    _encoder_factory: EncoderFactory
-    _q_func_factory: QFunctionFactory
-    _n_critics: int
-    _use_gpu: Optional[Device]
-    _impl: Optional[DQNImpl]
-
-    def __init__(
-        self,
-        *,
-        learning_rate: float = 6.25e-5,
-        optim_factory: OptimizerFactory = AdamFactory(),
-        encoder_factory: EncoderArg = "default",
-        q_func_factory: QFuncArg = "mean",
-        batch_size: int = 32,
-        n_frames: int = 1,
-        n_steps: int = 1,
-        gamma: float = 0.99,
-        n_critics: int = 1,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        reward_scaler: RewardScalerArg = None,
-        impl: Optional[DQNImpl] = None,
-        **kwargs: Any,
-    ):
-        super().__init__(
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=n_steps,
-            gamma=gamma,
-            scaler=scaler,
-            reward_scaler=reward_scaler,
-            kwargs=kwargs,
+        actor_optim = self._config.actor_optim_factory.create(
+            policy.parameters(), lr=self._config.actor_learning_rate
+        )
+        critic_optim = self._config.critic_optim_factory.create(
+            q_func.parameters(), lr=self._config.critic_learning_rate
         )
-        self._learning_rate = learning_rate
-        self._optim_factory = optim_factory
-        self._encoder_factory = check_encoder(encoder_factory)
-        self._q_func_factory = check_q_func(q_func_factory)
-        self._n_critics = n_critics
-        self._use_gpu = check_use_gpu(use_gpu)
-        self._impl = impl
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
-        self._impl = DQNImpl(
+        self._impl = AWACImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            learning_rate=self._learning_rate,
-            optim_factory=self._optim_factory,
-            encoder_factory=self._encoder_factory,
-            q_func_factory=self._q_func_factory,
-            gamma=self._gamma,
-            n_critics=self._n_critics,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            reward_scaler=self._reward_scaler,
+            q_func=q_func,
+            policy=policy,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            gamma=self._config.gamma,
+            tau=self._config.tau,
+            lam=self._config.lam,
+            n_action_samples=self._config.n_action_samples,
+            device=self._device,
         )
-        self._impl.build()
 
-    def _update(self, batch: TransitionMiniBatch) -> Dict[str, float]:
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
         assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
-        loss = self._impl.update(batch)
-        self._impl.update_target()
-        return {"loss": float(loss)}
+
+        metrics = {}
+
+        critic_loss = self._impl.update_critic(batch)
+        metrics.update({"critic_loss": critic_loss})
+
+        # delayed policy update
+        if self._grad_step % self._config.update_actor_interval == 0:
+            actor_loss = self._impl.update_actor(batch)
+            metrics.update({"actor_loss": actor_loss})
+            self._impl.update_critic_target()
+            self._impl.update_actor_target()
+
+        return metrics
 
     def get_action_type(self) -> ActionSpace:
-        return ActionSpace.DISCRETE
+        return ActionSpace.CONTINUOUS
+
+
+register_learnable(AWACConfig)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/sac.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/sac.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,34 @@
-from typing import Any, Dict, Optional, Sequence
-
-from ..argument_utility import (
-    ActionScalerArg,
-    EncoderArg,
-    QFuncArg,
-    RewardScalerArg,
-    ScalerArg,
-    UseGPUArg,
-    check_encoder,
-    check_q_func,
-    check_use_gpu,
+import dataclasses
+import math
+from typing import Dict
+
+from ...base import DeviceArg, LearnableConfig, register_learnable
+from ...constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
+from ...dataset import Shape
+from ...models.builders import (
+    create_categorical_policy,
+    create_continuous_q_function,
+    create_discrete_q_function,
+    create_parameter,
+    create_squashed_normal_policy,
 )
-from ..constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
-from ..dataset import TransitionMiniBatch
-from ..gpu import Device
-from ..models.encoders import EncoderFactory
-from ..models.optimizers import AdamFactory, OptimizerFactory
-from ..models.q_functions import QFunctionFactory
-from .base import AlgoBase
+from ...models.encoders import EncoderFactory, make_encoder_field
+from ...models.optimizers import OptimizerFactory, make_optimizer_field
+from ...models.q_functions import QFunctionFactory, make_q_func_field
+from ...torch_utility import TorchMiniBatch
+from .base import QLearningAlgoBase
 from .torch.sac_impl import DiscreteSACImpl, SACImpl
 
+__all__ = ["SACConfig", "SAC", "DiscreteSACConfig", "DiscreteSAC"]
+
 
-class SAC(AlgoBase):
-    r"""Soft Actor-Critic algorithm.
+@dataclasses.dataclass()
+class SACConfig(LearnableConfig):
+    r"""Config Soft Actor-Critic algorithm.
 
     SAC is a DDPG-based maximum entropy RL algorithm, which produces
     state-of-the-art performance in online RL settings.
     SAC leverages twin Q functions proposed in TD3. Additionally,
     `delayed policy update` in TD3 is also implemented, which is not done in
     the paper.
 
@@ -61,148 +63,117 @@
         * `Haarnoja et al., Soft Actor-Critic: Off-Policy Maximum Entropy Deep
           Reinforcement Learning with a Stochastic Actor.
           <https://arxiv.org/abs/1801.01290>`_
         * `Haarnoja et al., Soft Actor-Critic Algorithms and Applications.
           <https://arxiv.org/abs/1812.05905>`_
 
     Args:
-        actor_learning_rate (float): learning rate for policy function.
-        critic_learning_rate (float): learning rate for Q functions.
-        temp_learning_rate (float): learning rate for temperature parameter.
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        action_scaler (d3rlpy.preprocessing.ActionScaler): Action preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        actor_learning_rate (float): Learning rate for policy function.
+        critic_learning_rate (float): Learning rate for Q functions.
+        temp_learning_rate (float): Learning rate for temperature parameter.
         actor_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the actor.
+            Optimizer factory for the actor.
         critic_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the critic.
+            Optimizer factory for the critic.
         temp_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the temperature.
-        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the actor.
-        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the critic.
-        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory or str):
+            Optimizer factory for the temperature.
+        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the actor.
+        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the critic.
+        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory):
             Q function factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        tau (float): target network synchronization coefficiency.
-        n_critics (int): the number of Q functions for ensemble.
-        initial_temperature (float): initial temperature value.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`.
-        action_scaler (d3rlpy.preprocessing.ActionScaler or str):
-            action preprocessor. The available options are ``['min_max']``.
-        reward_scaler (d3rlpy.preprocessing.RewardScaler or str):
-            reward preprocessor. The available options are
-            ``['clip', 'min_max', 'standard']``.
-        impl (d3rlpy.algos.torch.sac_impl.SACImpl): algorithm implementation.
-
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        tau (float): Target network synchronization coefficiency.
+        n_critics (int): Number of Q functions for ensemble.
+        initial_temperature (float): Initial temperature value.
     """
+    actor_learning_rate: float = 3e-4
+    critic_learning_rate: float = 3e-4
+    temp_learning_rate: float = 3e-4
+    actor_optim_factory: OptimizerFactory = make_optimizer_field()
+    critic_optim_factory: OptimizerFactory = make_optimizer_field()
+    temp_optim_factory: OptimizerFactory = make_optimizer_field()
+    actor_encoder_factory: EncoderFactory = make_encoder_field()
+    critic_encoder_factory: EncoderFactory = make_encoder_field()
+    q_func_factory: QFunctionFactory = make_q_func_field()
+    batch_size: int = 256
+    gamma: float = 0.99
+    tau: float = 0.005
+    n_critics: int = 2
+    initial_temperature: float = 1.0
+
+    def create(self, device: DeviceArg = False) -> "SAC":
+        return SAC(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "sac"
+
+
+class SAC(QLearningAlgoBase[SACImpl, SACConfig]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        policy = create_squashed_normal_policy(
+            observation_shape,
+            action_size,
+            self._config.actor_encoder_factory,
+            device=self._device,
+        )
+        q_func = create_continuous_q_function(
+            observation_shape,
+            action_size,
+            self._config.critic_encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
+        log_temp = create_parameter(
+            (1, 1),
+            math.log(self._config.initial_temperature),
+            device=self._device,
+        )
 
-    _actor_learning_rate: float
-    _critic_learning_rate: float
-    _temp_learning_rate: float
-    _actor_optim_factory: OptimizerFactory
-    _critic_optim_factory: OptimizerFactory
-    _temp_optim_factory: OptimizerFactory
-    _actor_encoder_factory: EncoderFactory
-    _critic_encoder_factory: EncoderFactory
-    _q_func_factory: QFunctionFactory
-    _tau: float
-    _n_critics: int
-    _initial_temperature: float
-    _use_gpu: Optional[Device]
-    _impl: Optional[SACImpl]
-
-    def __init__(
-        self,
-        *,
-        actor_learning_rate: float = 3e-4,
-        critic_learning_rate: float = 3e-4,
-        temp_learning_rate: float = 3e-4,
-        actor_optim_factory: OptimizerFactory = AdamFactory(),
-        critic_optim_factory: OptimizerFactory = AdamFactory(),
-        temp_optim_factory: OptimizerFactory = AdamFactory(),
-        actor_encoder_factory: EncoderArg = "default",
-        critic_encoder_factory: EncoderArg = "default",
-        q_func_factory: QFuncArg = "mean",
-        batch_size: int = 256,
-        n_frames: int = 1,
-        n_steps: int = 1,
-        gamma: float = 0.99,
-        tau: float = 0.005,
-        n_critics: int = 2,
-        initial_temperature: float = 1.0,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        action_scaler: ActionScalerArg = None,
-        reward_scaler: RewardScalerArg = None,
-        impl: Optional[SACImpl] = None,
-        **kwargs: Any
-    ):
-        super().__init__(
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=n_steps,
-            gamma=gamma,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            reward_scaler=reward_scaler,
-            kwargs=kwargs,
-        )
-        self._actor_learning_rate = actor_learning_rate
-        self._critic_learning_rate = critic_learning_rate
-        self._temp_learning_rate = temp_learning_rate
-        self._actor_optim_factory = actor_optim_factory
-        self._critic_optim_factory = critic_optim_factory
-        self._temp_optim_factory = temp_optim_factory
-        self._actor_encoder_factory = check_encoder(actor_encoder_factory)
-        self._critic_encoder_factory = check_encoder(critic_encoder_factory)
-        self._q_func_factory = check_q_func(q_func_factory)
-        self._tau = tau
-        self._n_critics = n_critics
-        self._initial_temperature = initial_temperature
-        self._use_gpu = check_use_gpu(use_gpu)
-        self._impl = impl
+        actor_optim = self._config.actor_optim_factory.create(
+            policy.parameters(), lr=self._config.actor_learning_rate
+        )
+        critic_optim = self._config.critic_optim_factory.create(
+            q_func.parameters(), lr=self._config.critic_learning_rate
+        )
+        temp_optim = self._config.temp_optim_factory.create(
+            log_temp.parameters(), lr=self._config.temp_learning_rate
+        )
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
         self._impl = SACImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            actor_learning_rate=self._actor_learning_rate,
-            critic_learning_rate=self._critic_learning_rate,
-            temp_learning_rate=self._temp_learning_rate,
-            actor_optim_factory=self._actor_optim_factory,
-            critic_optim_factory=self._critic_optim_factory,
-            temp_optim_factory=self._temp_optim_factory,
-            actor_encoder_factory=self._actor_encoder_factory,
-            critic_encoder_factory=self._critic_encoder_factory,
-            q_func_factory=self._q_func_factory,
-            gamma=self._gamma,
-            tau=self._tau,
-            n_critics=self._n_critics,
-            initial_temperature=self._initial_temperature,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            action_scaler=self._action_scaler,
-            reward_scaler=self._reward_scaler,
+            policy=policy,
+            q_func=q_func,
+            log_temp=log_temp,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            temp_optim=temp_optim,
+            gamma=self._config.gamma,
+            tau=self._config.tau,
+            device=self._device,
         )
-        self._impl.build()
 
-    def _update(self, batch: TransitionMiniBatch) -> Dict[str, float]:
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
         assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
 
         metrics = {}
 
         # lagrangian parameter update for SAC temperature
-        if self._temp_learning_rate > 0:
+        if self._config.temp_learning_rate > 0:
             temp_loss, temp = self._impl.update_temp(batch)
             metrics.update({"temp_loss": temp_loss, "temp": temp})
 
         critic_loss = self._impl.update_critic(batch)
         metrics.update({"critic_loss": critic_loss})
 
         actor_loss = self._impl.update_actor(batch)
@@ -213,16 +184,17 @@
 
         return metrics
 
     def get_action_type(self) -> ActionSpace:
         return ActionSpace.CONTINUOUS
 
 
-class DiscreteSAC(AlgoBase):
-    r"""Soft Actor-Critic algorithm for discrete action-space.
+@dataclasses.dataclass()
+class DiscreteSACConfig(LearnableConfig):
+    r"""Config of Soft Actor-Critic algorithm for discrete action-space.
 
     This discrete version of SAC is built based on continuous version of SAC
     with additional modifications.
 
     The target state-value is calculated as expectation of all action-values.
 
     .. math::
@@ -244,152 +216,127 @@
             [\pi_\phi(s_t)^T [\alpha \log(\pi_\phi(s_t)) - Q_\theta(s_t)]]
 
     References:
         * `Christodoulou, Soft Actor-Critic for Discrete Action Settings.
           <https://arxiv.org/abs/1910.07207>`_
 
     Args:
-        actor_learning_rate (float): learning rate for policy function.
-        critic_learning_rate (float): learning rate for Q functions.
-        temp_learning_rate (float): learning rate for temperature parameter.
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        actor_learning_rate (float): Learning rate for policy function.
+        critic_learning_rate (float): Learning rate for Q functions.
+        temp_learning_rate (float): Learning rate for temperature parameter.
         actor_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the actor.
+            Optimizer factory for the actor.
         critic_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the critic.
+            Optimizer factory for the critic.
         temp_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the temperature.
-        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the actor.
-        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the critic.
-        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory or str):
+            Optimizer factory for the temperature.
+        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the actor.
+        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the critic.
+        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory):
             Q function factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        n_critics (int): the number of Q functions for ensemble.
-        initial_temperature (float): initial temperature value.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`
-        reward_scaler (d3rlpy.preprocessing.RewardScaler or str):
-            reward preprocessor. The available options are
-            ``['clip', 'min_max', 'standard']``.
-        impl (d3rlpy.algos.torch.sac_impl.DiscreteSACImpl):
-            algorithm implementation.
-
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        n_critics (int): Number of Q functions for ensemble.
+        initial_temperature (float): Initial temperature value.
     """
+    actor_learning_rate: float = 3e-4
+    critic_learning_rate: float = 3e-4
+    temp_learning_rate: float = 3e-4
+    actor_optim_factory: OptimizerFactory = make_optimizer_field()
+    critic_optim_factory: OptimizerFactory = make_optimizer_field()
+    temp_optim_factory: OptimizerFactory = make_optimizer_field()
+    actor_encoder_factory: EncoderFactory = make_encoder_field()
+    critic_encoder_factory: EncoderFactory = make_encoder_field()
+    q_func_factory: QFunctionFactory = make_q_func_field()
+    batch_size: int = 64
+    gamma: float = 0.99
+    n_critics: int = 2
+    initial_temperature: float = 1.0
+    target_update_interval: int = 8000
+
+    def create(self, device: DeviceArg = False) -> "DiscreteSAC":
+        return DiscreteSAC(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "discrete_sac"
+
+
+class DiscreteSAC(QLearningAlgoBase[DiscreteSACImpl, DiscreteSACConfig]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        q_func = create_discrete_q_function(
+            observation_shape,
+            action_size,
+            self._config.critic_encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
+        policy = create_categorical_policy(
+            observation_shape,
+            action_size,
+            self._config.actor_encoder_factory,
+            device=self._device,
+        )
+        log_temp = create_parameter(
+            (1, 1),
+            math.log(self._config.initial_temperature),
+            device=self._device,
+        )
 
-    _actor_learning_rate: float
-    _critic_learning_rate: float
-    _temp_learning_rate: float
-    _actor_optim_factory: OptimizerFactory
-    _critic_optim_factory: OptimizerFactory
-    _temp_optim_factory: OptimizerFactory
-    _actor_encoder_factory: EncoderFactory
-    _critic_encoder_factory: EncoderFactory
-    _q_func_factory: QFunctionFactory
-    _n_critics: int
-    _initial_temperature: float
-    _target_update_interval: int
-    _use_gpu: Optional[Device]
-    _impl: Optional[DiscreteSACImpl]
-
-    def __init__(
-        self,
-        *,
-        actor_learning_rate: float = 3e-4,
-        critic_learning_rate: float = 3e-4,
-        temp_learning_rate: float = 3e-4,
-        actor_optim_factory: OptimizerFactory = AdamFactory(eps=1e-4),
-        critic_optim_factory: OptimizerFactory = AdamFactory(eps=1e-4),
-        temp_optim_factory: OptimizerFactory = AdamFactory(eps=1e-4),
-        actor_encoder_factory: EncoderArg = "default",
-        critic_encoder_factory: EncoderArg = "default",
-        q_func_factory: QFuncArg = "mean",
-        batch_size: int = 64,
-        n_frames: int = 1,
-        n_steps: int = 1,
-        gamma: float = 0.99,
-        n_critics: int = 2,
-        initial_temperature: float = 1.0,
-        target_update_interval: int = 8000,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        reward_scaler: RewardScalerArg = None,
-        impl: Optional[DiscreteSACImpl] = None,
-        **kwargs: Any
-    ):
-        super().__init__(
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=n_steps,
-            gamma=gamma,
-            scaler=scaler,
-            action_scaler=None,
-            reward_scaler=reward_scaler,
-            kwargs=kwargs,
-        )
-        self._actor_learning_rate = actor_learning_rate
-        self._critic_learning_rate = critic_learning_rate
-        self._temp_learning_rate = temp_learning_rate
-        self._actor_optim_factory = actor_optim_factory
-        self._critic_optim_factory = critic_optim_factory
-        self._temp_optim_factory = temp_optim_factory
-        self._actor_encoder_factory = check_encoder(actor_encoder_factory)
-        self._critic_encoder_factory = check_encoder(critic_encoder_factory)
-        self._q_func_factory = check_q_func(q_func_factory)
-        self._n_critics = n_critics
-        self._initial_temperature = initial_temperature
-        self._target_update_interval = target_update_interval
-        self._use_gpu = check_use_gpu(use_gpu)
-        self._impl = impl
+        critic_optim = self._config.critic_optim_factory.create(
+            q_func.parameters(), lr=self._config.critic_learning_rate
+        )
+        actor_optim = self._config.actor_optim_factory.create(
+            policy.parameters(), lr=self._config.actor_learning_rate
+        )
+        temp_optim = self._config.temp_optim_factory.create(
+            log_temp.parameters(), lr=self._config.temp_learning_rate
+        )
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
         self._impl = DiscreteSACImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            actor_learning_rate=self._actor_learning_rate,
-            critic_learning_rate=self._critic_learning_rate,
-            temp_learning_rate=self._temp_learning_rate,
-            actor_optim_factory=self._actor_optim_factory,
-            critic_optim_factory=self._critic_optim_factory,
-            temp_optim_factory=self._temp_optim_factory,
-            actor_encoder_factory=self._actor_encoder_factory,
-            critic_encoder_factory=self._critic_encoder_factory,
-            q_func_factory=self._q_func_factory,
-            gamma=self._gamma,
-            n_critics=self._n_critics,
-            initial_temperature=self._initial_temperature,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            reward_scaler=self._reward_scaler,
+            q_func=q_func,
+            policy=policy,
+            log_temp=log_temp,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            temp_optim=temp_optim,
+            gamma=self._config.gamma,
+            device=self._device,
         )
-        self._impl.build()
 
-    def _update(self, batch: TransitionMiniBatch) -> Dict[str, float]:
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
         assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
 
         metrics = {}
 
         # lagrangian parameter update for SAC temeprature
-        if self._temp_learning_rate > 0:
+        if self._config.temp_learning_rate > 0:
             temp_loss, temp = self._impl.update_temp(batch)
             metrics.update({"temp_loss": temp_loss, "temp": temp})
 
         critic_loss = self._impl.update_critic(batch)
         metrics.update({"critic_loss": critic_loss})
 
         actor_loss = self._impl.update_actor(batch)
         metrics.update({"actor_loss": actor_loss})
 
-        if self._grad_step % self._target_update_interval == 0:
+        if self._grad_step % self._config.target_update_interval == 0:
             self._impl.update_target()
 
         return metrics
 
     def get_action_type(self) -> ActionSpace:
         return ActionSpace.DISCRETE
+
+
+register_learnable(SACConfig)
+register_learnable(DiscreteSACConfig)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/td3.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/td3.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from typing import Any, Dict, Optional, Sequence
+import dataclasses
+from typing import Dict
 
-from ..argument_utility import (
-    ActionScalerArg,
-    EncoderArg,
-    QFuncArg,
-    RewardScalerArg,
-    ScalerArg,
-    UseGPUArg,
-    check_encoder,
-    check_q_func,
-    check_use_gpu,
+from ...base import DeviceArg, LearnableConfig, register_learnable
+from ...constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
+from ...dataset import Shape
+from ...models.builders import (
+    create_continuous_q_function,
+    create_deterministic_policy,
 )
-from ..constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
-from ..dataset import TransitionMiniBatch
-from ..gpu import Device
-from ..models.encoders import EncoderFactory
-from ..models.optimizers import AdamFactory, OptimizerFactory
-from ..models.q_functions import QFunctionFactory
-from .base import AlgoBase
+from ...models.encoders import EncoderFactory, make_encoder_field
+from ...models.optimizers import OptimizerFactory, make_optimizer_field
+from ...models.q_functions import QFunctionFactory, make_q_func_field
+from ...torch_utility import TorchMiniBatch
+from .base import QLearningAlgoBase
 from .torch.td3_impl import TD3Impl
 
+__all__ = ["TD3Config", "TD3"]
 
-class TD3(AlgoBase):
-    r"""Twin Delayed Deep Deterministic Policy Gradients algorithm.
+
+@dataclasses.dataclass()
+class TD3Config(LearnableConfig):
+    r"""Config of Twin Delayed Deep Deterministic Policy Gradients algorithm.
 
     TD3 is an improved DDPG-based algorithm.
     Major differences from DDPG are as follows.
 
     * TD3 has twin Q functions to reduce overestimation bias at TD learning.
       The number of Q functions can be designated by `n_critics`.
     * TD3 adds noise to target value estimation to avoid overfitting with the
@@ -49,152 +47,117 @@
     where :math:`\epsilon \sim clip (N(0, \sigma), -c, c)`
 
     References:
         * `Fujimoto et al., Addressing Function Approximation Error in
           Actor-Critic Methods. <https://arxiv.org/abs/1802.09477>`_
 
     Args:
-        actor_learning_rate (float): learning rate for a policy function.
-        critic_learning_rate (float): learning rate for Q functions.
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        action_scaler (d3rlpy.preprocessing.ActionScaler): Action preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        actor_learning_rate (float): Learning rate for a policy function.
+        critic_learning_rate (float): Learning rate for Q functions.
         actor_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the actor.
+            Optimizer factory for the actor.
         critic_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the critic.
-        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the actor.
-        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the critic.
-        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory or str):
+            Optimizer factory for the critic.
+        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the actor.
+        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the critic.
+        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory):
             Q function factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        tau (float): target network synchronization coefficiency.
-        n_critics (int): the number of Q functions for ensemble.
-        target_smoothing_sigma (float): standard deviation for target noise.
-        target_smoothing_clip (float): clipping range for target noise.
-        update_actor_interval (int): interval to update policy function
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        tau (float): Target network synchronization coefficiency.
+        n_critics (int): Number of Q functions for ensemble.
+        target_smoothing_sigma (float): Standard deviation for target noise.
+        target_smoothing_clip (float): Clipping range for target noise.
+        update_actor_interval (int): Interval to update policy function
             described as `delayed policy update` in the paper.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`.
-        action_scaler (d3rlpy.preprocessing.ActionScaler or str):
-            action preprocessor. The available options are ``['min_max']``.
-        reward_scaler (d3rlpy.preprocessing.RewardScaler or str):
-            reward preprocessor. The available options are
-            ``['clip', 'min_max', 'standard']``.
-        impl (d3rlpy.algos.torch.td3_impl.TD3Impl): algorithm implementation.
-
     """
+    actor_learning_rate: float = 3e-4
+    critic_learning_rate: float = 3e-4
+    actor_optim_factory: OptimizerFactory = make_optimizer_field()
+    critic_optim_factory: OptimizerFactory = make_optimizer_field()
+    actor_encoder_factory: EncoderFactory = make_encoder_field()
+    critic_encoder_factory: EncoderFactory = make_encoder_field()
+    q_func_factory: QFunctionFactory = make_q_func_field()
+    batch_size: int = 256
+    gamma: float = 0.99
+    tau: float = 0.005
+    n_critics: int = 2
+    target_smoothing_sigma: float = 0.2
+    target_smoothing_clip: float = 0.5
+    update_actor_interval: int = 2
+
+    def create(self, device: DeviceArg = False) -> "TD3":
+        return TD3(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "td3"
+
+
+class TD3(QLearningAlgoBase[TD3Impl, TD3Config]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        policy = create_deterministic_policy(
+            observation_shape,
+            action_size,
+            self._config.actor_encoder_factory,
+            device=self._device,
+        )
+        q_func = create_continuous_q_function(
+            observation_shape,
+            action_size,
+            self._config.critic_encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
 
-    _actor_learning_rate: float
-    _critic_learning_rate: float
-    _actor_optim_factory: OptimizerFactory
-    _critic_optim_factory: OptimizerFactory
-    _actor_encoder_factory: EncoderFactory
-    _critic_encoder_factory: EncoderFactory
-    _q_func_factory: QFunctionFactory
-    _tau: float
-    _n_critics: int
-    _target_smoothing_sigma: float
-    _target_smoothing_clip: float
-    _update_actor_interval: int
-    _use_gpu: Optional[Device]
-    _impl: Optional[TD3Impl]
-
-    def __init__(
-        self,
-        *,
-        actor_learning_rate: float = 3e-4,
-        critic_learning_rate: float = 3e-4,
-        actor_optim_factory: OptimizerFactory = AdamFactory(),
-        critic_optim_factory: OptimizerFactory = AdamFactory(),
-        actor_encoder_factory: EncoderArg = "default",
-        critic_encoder_factory: EncoderArg = "default",
-        q_func_factory: QFuncArg = "mean",
-        batch_size: int = 256,
-        n_frames: int = 1,
-        n_steps: int = 1,
-        gamma: float = 0.99,
-        tau: float = 0.005,
-        n_critics: int = 2,
-        target_smoothing_sigma: float = 0.2,
-        target_smoothing_clip: float = 0.5,
-        update_actor_interval: int = 2,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = None,
-        action_scaler: ActionScalerArg = None,
-        reward_scaler: RewardScalerArg = None,
-        impl: Optional[TD3Impl] = None,
-        **kwargs: Any
-    ):
-        super().__init__(
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=n_steps,
-            gamma=gamma,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            reward_scaler=reward_scaler,
-            kwargs=kwargs,
+        actor_optim = self._config.actor_optim_factory.create(
+            policy.parameters(), lr=self._config.actor_learning_rate
+        )
+        critic_optim = self._config.critic_optim_factory.create(
+            q_func.parameters(), lr=self._config.critic_learning_rate
         )
-        self._actor_learning_rate = actor_learning_rate
-        self._critic_learning_rate = critic_learning_rate
-        self._actor_optim_factory = actor_optim_factory
-        self._critic_optim_factory = critic_optim_factory
-        self._actor_encoder_factory = check_encoder(actor_encoder_factory)
-        self._critic_encoder_factory = check_encoder(critic_encoder_factory)
-        self._q_func_factory = check_q_func(q_func_factory)
-        self._tau = tau
-        self._n_critics = n_critics
-        self._target_smoothing_sigma = target_smoothing_sigma
-        self._target_smoothing_clip = target_smoothing_clip
-        self._update_actor_interval = update_actor_interval
-        self._use_gpu = check_use_gpu(use_gpu)
-        self._impl = impl
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
         self._impl = TD3Impl(
             observation_shape=observation_shape,
             action_size=action_size,
-            actor_learning_rate=self._actor_learning_rate,
-            critic_learning_rate=self._critic_learning_rate,
-            actor_optim_factory=self._actor_optim_factory,
-            critic_optim_factory=self._critic_optim_factory,
-            actor_encoder_factory=self._actor_encoder_factory,
-            critic_encoder_factory=self._critic_encoder_factory,
-            q_func_factory=self._q_func_factory,
-            gamma=self._gamma,
-            tau=self._tau,
-            n_critics=self._n_critics,
-            target_smoothing_sigma=self._target_smoothing_sigma,
-            target_smoothing_clip=self._target_smoothing_clip,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            action_scaler=self._action_scaler,
-            reward_scaler=self._reward_scaler,
+            policy=policy,
+            q_func=q_func,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            gamma=self._config.gamma,
+            tau=self._config.tau,
+            target_smoothing_sigma=self._config.target_smoothing_sigma,
+            target_smoothing_clip=self._config.target_smoothing_clip,
+            device=self._device,
         )
-        self._impl.build()
 
-    def _update(self, batch: TransitionMiniBatch) -> Dict[str, float]:
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
         assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
 
         metrics = {}
 
         critic_loss = self._impl.update_critic(batch)
         metrics.update({"critic_loss": critic_loss})
 
         # delayed policy update
-        if self._grad_step % self._update_actor_interval == 0:
+        if self._grad_step % self._config.update_actor_interval == 0:
             actor_loss = self._impl.update_actor(batch)
             metrics.update({"actor_loss": actor_loss})
             self._impl.update_critic_target()
             self._impl.update_actor_target()
 
         return metrics
 
     def get_action_type(self) -> ActionSpace:
         return ActionSpace.CONTINUOUS
+
+
+register_learnable(TD3Config)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/td3_plus_bc.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/td3_plus_bc.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-from typing import Any, Dict, Optional, Sequence
+import dataclasses
+from typing import Dict
 
-from ..argument_utility import (
-    ActionScalerArg,
-    EncoderArg,
-    QFuncArg,
-    RewardScalerArg,
-    ScalerArg,
-    UseGPUArg,
-    check_encoder,
-    check_q_func,
-    check_use_gpu,
+from ...base import DeviceArg, LearnableConfig, register_learnable
+from ...constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
+from ...dataset import Shape
+from ...models.builders import (
+    create_continuous_q_function,
+    create_deterministic_policy,
 )
-from ..constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
-from ..dataset import TransitionMiniBatch
-from ..gpu import Device
-from ..models.encoders import EncoderFactory
-from ..models.optimizers import AdamFactory, OptimizerFactory
-from ..models.q_functions import QFunctionFactory
-from .base import AlgoBase
+from ...models.encoders import EncoderFactory, make_encoder_field
+from ...models.optimizers import OptimizerFactory, make_optimizer_field
+from ...models.q_functions import QFunctionFactory, make_q_func_field
+from ...torch_utility import TorchMiniBatch
+from .base import QLearningAlgoBase
 from .torch.td3_plus_bc_impl import TD3PlusBCImpl
 
+__all__ = ["TD3PlusBCConfig", "TD3PlusBC"]
 
-class TD3PlusBC(AlgoBase):
-    r"""TD3+BC algorithm.
+
+@dataclasses.dataclass()
+class TD3PlusBCConfig(LearnableConfig):
+    r"""Config of TD3+BC algorithm.
 
     TD3+BC is an simple offline RL algorithm built on top of TD3.
     TD3+BC introduces BC-reguralized policy objective function.
 
     .. math::
 
         J(\phi) = \mathbb{E}_{s,a \sim D}
@@ -39,157 +37,120 @@
         \lambda = \frac{\alpha}{\frac{1}{N} \sum_(s_i, a_i) |Q(s_i, a_i)|}
 
     References:
         * `Fujimoto et al., A Minimalist Approach to Offline Reinforcement
           Learning. <https://arxiv.org/abs/2106.06860>`_
 
     Args:
-        actor_learning_rate (float): learning rate for a policy function.
-        critic_learning_rate (float): learning rate for Q functions.
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        action_scaler (d3rlpy.preprocessing.ActionScaler): Action preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        actor_learning_rate (float): Learning rate for a policy function.
+        critic_learning_rate (float): Learning rate for Q functions.
         actor_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the actor.
+            Optimizer factory for the actor.
         critic_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
-            optimizer factory for the critic.
-        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the actor.
-        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory or str):
-            encoder factory for the critic.
-        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory or str):
+            Optimizer factory for the critic.
+        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the actor.
+        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the critic.
+        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory):
             Q function factory.
-        batch_size (int): mini-batch size.
-        n_frames (int): the number of frames to stack for image observation.
-        n_steps (int): N-step TD calculation.
-        gamma (float): discount factor.
-        tau (float): target network synchronization coefficiency.
-        n_critics (int): the number of Q functions for ensemble.
-        target_smoothing_sigma (float): standard deviation for target noise.
-        target_smoothing_clip (float): clipping range for target noise.
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        tau (float): Target network synchronization coefficiency.
+        n_critics (int): Number of Q functions for ensemble.
+        target_smoothing_sigma (float): Standard deviation for target noise.
+        target_smoothing_clip (float): Clipping range for target noise.
         alpha (float): :math:`\alpha` value.
-        update_actor_interval (int): interval to update policy function
+        update_actor_interval (int): Interval to update policy function
             described as `delayed policy update` in the paper.
-        use_gpu (bool, int or d3rlpy.gpu.Device):
-            flag to use GPU, device ID or device.
-        scaler (d3rlpy.preprocessing.Scaler or str): preprocessor.
-            The available options are `['pixel', 'min_max', 'standard']`.
-        action_scaler (d3rlpy.preprocessing.ActionScaler or str):
-            action preprocessor. The available options are ``['min_max']``.
-        reward_scaler (d3rlpy.preprocessing.RewardScaler or str):
-            reward preprocessor. The available options are
-            ``['clip', 'min_max', 'standard']``.
-        impl (d3rlpy.algos.torch.td3_impl.TD3Impl): algorithm implementation.
-
     """
+    actor_learning_rate: float = 3e-4
+    critic_learning_rate: float = 3e-4
+    actor_optim_factory: OptimizerFactory = make_optimizer_field()
+    critic_optim_factory: OptimizerFactory = make_optimizer_field()
+    actor_encoder_factory: EncoderFactory = make_encoder_field()
+    critic_encoder_factory: EncoderFactory = make_encoder_field()
+    q_func_factory: QFunctionFactory = make_q_func_field()
+    batch_size: int = 256
+    gamma: float = 0.99
+    tau: float = 0.005
+    n_critics: int = 2
+    target_smoothing_sigma: float = 0.2
+    target_smoothing_clip: float = 0.5
+    alpha: float = 2.5
+    update_actor_interval: int = 2
+
+    def create(self, device: DeviceArg = False) -> "TD3PlusBC":
+        return TD3PlusBC(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "td3_plus_bc"
+
+
+class TD3PlusBC(QLearningAlgoBase[TD3PlusBCImpl, TD3PlusBCConfig]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        policy = create_deterministic_policy(
+            observation_shape,
+            action_size,
+            self._config.actor_encoder_factory,
+            device=self._device,
+        )
+        q_func = create_continuous_q_function(
+            observation_shape,
+            action_size,
+            self._config.critic_encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
 
-    _actor_learning_rate: float
-    _critic_learning_rate: float
-    _actor_optim_factory: OptimizerFactory
-    _critic_optim_factory: OptimizerFactory
-    _actor_encoder_factory: EncoderFactory
-    _critic_encoder_factory: EncoderFactory
-    _q_func_factory: QFunctionFactory
-    _tau: float
-    _n_critics: int
-    _target_smoothing_sigma: float
-    _target_smoothing_clip: float
-    _alpha: float
-    _update_actor_interval: int
-    _use_gpu: Optional[Device]
-    _impl: Optional[TD3PlusBCImpl]
-
-    def __init__(
-        self,
-        *,
-        actor_learning_rate: float = 3e-4,
-        critic_learning_rate: float = 3e-4,
-        actor_optim_factory: OptimizerFactory = AdamFactory(),
-        critic_optim_factory: OptimizerFactory = AdamFactory(),
-        actor_encoder_factory: EncoderArg = "default",
-        critic_encoder_factory: EncoderArg = "default",
-        q_func_factory: QFuncArg = "mean",
-        batch_size: int = 256,
-        n_frames: int = 1,
-        n_steps: int = 1,
-        gamma: float = 0.99,
-        tau: float = 0.005,
-        n_critics: int = 2,
-        target_smoothing_sigma: float = 0.2,
-        target_smoothing_clip: float = 0.5,
-        alpha: float = 2.5,
-        update_actor_interval: int = 2,
-        use_gpu: UseGPUArg = False,
-        scaler: ScalerArg = "standard",
-        action_scaler: ActionScalerArg = None,
-        reward_scaler: RewardScalerArg = None,
-        impl: Optional[TD3PlusBCImpl] = None,
-        **kwargs: Any
-    ):
-        super().__init__(
-            batch_size=batch_size,
-            n_frames=n_frames,
-            n_steps=n_steps,
-            gamma=gamma,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            reward_scaler=reward_scaler,
-            kwargs=kwargs,
+        actor_optim = self._config.actor_optim_factory.create(
+            policy.parameters(), lr=self._config.actor_learning_rate
+        )
+        critic_optim = self._config.critic_optim_factory.create(
+            q_func.parameters(), lr=self._config.critic_learning_rate
         )
-        self._actor_learning_rate = actor_learning_rate
-        self._critic_learning_rate = critic_learning_rate
-        self._actor_optim_factory = actor_optim_factory
-        self._critic_optim_factory = critic_optim_factory
-        self._actor_encoder_factory = check_encoder(actor_encoder_factory)
-        self._critic_encoder_factory = check_encoder(critic_encoder_factory)
-        self._q_func_factory = check_q_func(q_func_factory)
-        self._tau = tau
-        self._n_critics = n_critics
-        self._target_smoothing_sigma = target_smoothing_sigma
-        self._target_smoothing_clip = target_smoothing_clip
-        self._alpha = alpha
-        self._update_actor_interval = update_actor_interval
-        self._use_gpu = check_use_gpu(use_gpu)
-        self._impl = impl
 
-    def _create_impl(
-        self, observation_shape: Sequence[int], action_size: int
-    ) -> None:
         self._impl = TD3PlusBCImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            actor_learning_rate=self._actor_learning_rate,
-            critic_learning_rate=self._critic_learning_rate,
-            actor_optim_factory=self._actor_optim_factory,
-            critic_optim_factory=self._critic_optim_factory,
-            actor_encoder_factory=self._actor_encoder_factory,
-            critic_encoder_factory=self._critic_encoder_factory,
-            q_func_factory=self._q_func_factory,
-            gamma=self._gamma,
-            tau=self._tau,
-            n_critics=self._n_critics,
-            target_smoothing_sigma=self._target_smoothing_sigma,
-            target_smoothing_clip=self._target_smoothing_clip,
-            alpha=self._alpha,
-            use_gpu=self._use_gpu,
-            scaler=self._scaler,
-            action_scaler=self._action_scaler,
-            reward_scaler=self._reward_scaler,
+            policy=policy,
+            q_func=q_func,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            gamma=self._config.gamma,
+            tau=self._config.tau,
+            target_smoothing_sigma=self._config.target_smoothing_sigma,
+            target_smoothing_clip=self._config.target_smoothing_clip,
+            alpha=self._config.alpha,
+            device=self._device,
         )
-        self._impl.build()
 
-    def _update(self, batch: TransitionMiniBatch) -> Dict[str, float]:
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
         assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
 
         metrics = {}
 
         critic_loss = self._impl.update_critic(batch)
         metrics.update({"critic_loss": critic_loss})
 
         # delayed policy update
-        if self._grad_step % self._update_actor_interval == 0:
+        if self._grad_step % self._config.update_actor_interval == 0:
             actor_loss = self._impl.update_actor(batch)
             metrics.update({"actor_loss": actor_loss})
             self._impl.update_critic_target()
             self._impl.update_actor_target()
 
         return metrics
 
     def get_action_type(self) -> ActionSpace:
         return ActionSpace.CONTINUOUS
+
+
+register_learnable(TD3PlusBCConfig)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/torch/awac_impl.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/crr_impl.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,152 +1,155 @@
-from typing import Optional, Sequence, Tuple
-
-import numpy as np
 import torch
 import torch.nn.functional as F
+from torch.optim import Optimizer
 
-from ...gpu import Device
-from ...models.builders import create_non_squashed_normal_policy
-from ...models.encoders import EncoderFactory
-from ...models.optimizers import AdamFactory, OptimizerFactory
-from ...models.q_functions import QFunctionFactory
-from ...models.torch.policies import NonSquashedNormalPolicy
-from ...preprocessing import ActionScaler, RewardScaler, Scaler
-from ...torch_utility import TorchMiniBatch, torch_api, train_api
-from .sac_impl import SACImpl
+from ....dataset import Shape
+from ....models.torch import (
+    EnsembleContinuousQFunction,
+    NonSquashedNormalPolicy,
+)
+from ....torch_utility import TorchMiniBatch, hard_sync
+from .ddpg_impl import DDPGBaseImpl
 
+__all__ = ["CRRImpl"]
 
-class AWACImpl(SACImpl):
 
-    _policy: NonSquashedNormalPolicy
-    _lam: float
+class CRRImpl(DDPGBaseImpl):
+    _beta: float
     _n_action_samples: int
+    _advantage_type: str
+    _weight_type: str
+    _max_weight: float
+    _policy: NonSquashedNormalPolicy
+    _targ_policy: NonSquashedNormalPolicy
 
     def __init__(
         self,
-        observation_shape: Sequence[int],
+        observation_shape: Shape,
         action_size: int,
-        actor_learning_rate: float,
-        critic_learning_rate: float,
-        actor_optim_factory: OptimizerFactory,
-        critic_optim_factory: OptimizerFactory,
-        actor_encoder_factory: EncoderFactory,
-        critic_encoder_factory: EncoderFactory,
-        q_func_factory: QFunctionFactory,
+        policy: NonSquashedNormalPolicy,
+        q_func: EnsembleContinuousQFunction,
+        actor_optim: Optimizer,
+        critic_optim: Optimizer,
         gamma: float,
-        tau: float,
-        lam: float,
+        beta: float,
         n_action_samples: int,
-        n_critics: int,
-        use_gpu: Optional[Device],
-        scaler: Optional[Scaler],
-        action_scaler: Optional[ActionScaler],
-        reward_scaler: Optional[RewardScaler],
+        advantage_type: str,
+        weight_type: str,
+        max_weight: float,
+        tau: float,
+        device: str,
     ):
         super().__init__(
             observation_shape=observation_shape,
             action_size=action_size,
-            actor_learning_rate=actor_learning_rate,
-            critic_learning_rate=critic_learning_rate,
-            temp_learning_rate=0.0,
-            actor_optim_factory=actor_optim_factory,
-            critic_optim_factory=critic_optim_factory,
-            temp_optim_factory=AdamFactory(),
-            actor_encoder_factory=actor_encoder_factory,
-            critic_encoder_factory=critic_encoder_factory,
-            q_func_factory=q_func_factory,
+            policy=policy,
+            q_func=q_func,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
             gamma=gamma,
             tau=tau,
-            n_critics=n_critics,
-            initial_temperature=1e-20,
-            use_gpu=use_gpu,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            reward_scaler=reward_scaler,
+            device=device,
         )
-        self._lam = lam
+        self._beta = beta
         self._n_action_samples = n_action_samples
-
-    def _build_actor(self) -> None:
-        self._policy = create_non_squashed_normal_policy(
-            self._observation_shape,
-            self._action_size,
-            self._actor_encoder_factory,
-            min_logstd=-6.0,
-            max_logstd=0.0,
-            use_std_parameter=True,
-        )
-
-    @train_api
-    @torch_api()
-    def update_actor(
-        self, batch: TorchMiniBatch
-    ) -> Tuple[np.ndarray, np.ndarray]:
-        assert self._q_func is not None
-        assert self._policy is not None
-        assert self._actor_optim is not None
-
-        # Q function should be inference mode for stability
-        self._q_func.eval()
-
-        self._actor_optim.zero_grad()
-
-        loss = self.compute_actor_loss(batch)
-
-        loss.backward()
-        self._actor_optim.step()
-
-        # get current standard deviation for policy function for debug
-        mean_std = self._policy.get_logstd_parameter().exp().mean()
-
-        return loss.cpu().detach().numpy(), mean_std.cpu().detach().numpy()
+        self._advantage_type = advantage_type
+        self._weight_type = weight_type
+        self._max_weight = max_weight
 
     def compute_actor_loss(self, batch: TorchMiniBatch) -> torch.Tensor:
-        assert self._policy is not None
-
         # compute log probability
         dist = self._policy.dist(batch.observations)
         log_probs = dist.log_prob(batch.actions)
 
-        # compute exponential weight
-        weights = self._compute_weights(batch.observations, batch.actions)
+        weight = self._compute_weight(batch.observations, batch.actions)
 
-        return -(log_probs * weights).sum()
+        return -(log_probs * weight).mean()
 
-    def _compute_weights(
+    def _compute_weight(
+        self, obs_t: torch.Tensor, act_t: torch.Tensor
+    ) -> torch.Tensor:
+        advantages = self._compute_advantage(obs_t, act_t)
+        if self._weight_type == "binary":
+            return (advantages > 0.0).float()
+        elif self._weight_type == "exp":
+            return (advantages / self._beta).exp().clamp(0.0, self._max_weight)
+        raise ValueError(f"invalid weight type: {self._weight_type}.")
+
+    def _compute_advantage(
         self, obs_t: torch.Tensor, act_t: torch.Tensor
     ) -> torch.Tensor:
-        assert self._q_func is not None
-        assert self._policy is not None
         with torch.no_grad():
             batch_size = obs_t.shape[0]
 
-            # compute action-value
-            q_values = self._q_func(obs_t, act_t, "min")
-
-            # sample actions
-            # (batch_size * N, action_size)
+            # (batch_size, N, action)
             policy_actions = self._policy.sample_n(
                 obs_t, self._n_action_samples
             )
-            flat_actions = policy_actions.reshape(-1, self.action_size)
+            flat_actions = policy_actions.reshape(-1, self._action_size)
 
             # repeat observation
             # (batch_size, obs_size) -> (batch_size, 1, obs_size)
             reshaped_obs_t = obs_t.view(batch_size, 1, *obs_t.shape[1:])
             # (batch_sie, 1, obs_size) -> (batch_size, N, obs_size)
             repeated_obs_t = reshaped_obs_t.expand(
                 batch_size, self._n_action_samples, *obs_t.shape[1:]
             )
             # (batch_size, N, obs_size) -> (batch_size * N, obs_size)
             flat_obs_t = repeated_obs_t.reshape(-1, *obs_t.shape[1:])
 
-            # compute state-value
-            flat_v_values = self._q_func(flat_obs_t, flat_actions, "min")
-            reshaped_v_values = flat_v_values.view(obs_t.shape[0], -1, 1)
-            v_values = reshaped_v_values.mean(dim=1)
-
-            # compute normalized weight
-            adv_values = (q_values - v_values).view(-1)
-            weights = F.softmax(adv_values / self._lam, dim=0).view(-1, 1)
+            flat_values = self._q_func(flat_obs_t, flat_actions)
+            reshaped_values = flat_values.view(obs_t.shape[0], -1, 1)
+
+            if self._advantage_type == "mean":
+                values = reshaped_values.mean(dim=1)
+            elif self._advantage_type == "max":
+                values = reshaped_values.max(dim=1).values
+            else:
+                raise ValueError(
+                    f"invalid advantage type: {self._advantage_type}."
+                )
+
+            return self._q_func(obs_t, act_t) - values
+
+    def compute_target(self, batch: TorchMiniBatch) -> torch.Tensor:
+        with torch.no_grad():
+            action = self._targ_policy.sample(batch.next_observations)
+            return self._targ_q_func.compute_target(
+                batch.next_observations,
+                action.clamp(-1.0, 1.0),
+                reduction="min",
+            )
+
+    def inner_predict_best_action(self, x: torch.Tensor) -> torch.Tensor:
+        # compute CWP
+
+        actions = self._policy.onnx_safe_sample_n(x, self._n_action_samples)
+        # (batch_size, N, action_size) -> (batch_size * N, action_size)
+        flat_actions = actions.reshape(-1, self._action_size)
+
+        # repeat observation
+        # (batch_size, obs_size) -> (batch_size, 1, obs_size)
+        reshaped_obs_t = x.view(x.shape[0], 1, *x.shape[1:])
+        # (batch_size, 1, obs_size) -> (batch_size, N, obs_size)
+        repeated_obs_t = reshaped_obs_t.expand(
+            x.shape[0], self._n_action_samples, *x.shape[1:]
+        )
+        # (batch_size, N, obs_size) -> (batch_size * N, obs_size)
+        flat_obs_t = repeated_obs_t.reshape(-1, *x.shape[1:])
+
+        # (batch_size * N, 1)
+        flat_values = self._q_func(flat_obs_t, flat_actions)
+        # (batch_size * N, 1) -> (batch_size, N)
+        reshaped_values = flat_values.view(x.shape[0], -1)
+
+        # re-sampling
+        probs = F.softmax(reshaped_values, dim=1)
+        indices = torch.multinomial(probs, 1, replacement=True)
+
+        return actions[torch.arange(x.shape[0]), indices.view(-1)]
+
+    def sync_critic_target(self) -> None:
+        hard_sync(self._targ_q_func, self._q_func)
 
-        return weights * adv_values.numel()
+    def sync_actor_target(self) -> None:
+        hard_sync(self._targ_policy, self._policy)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/torch/bcq_impl.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/plas.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,322 +1,304 @@
-import math
-from typing import Optional, Sequence, cast
+import dataclasses
+from typing import Dict
 
-import numpy as np
-import torch
-from torch.optim import Optimizer
-
-from ...gpu import Device
+from ...base import DeviceArg, LearnableConfig, register_learnable
+from ...constants import IMPL_NOT_INITIALIZED_ERROR, ActionSpace
+from ...dataset import Shape
 from ...models.builders import (
     create_conditional_vae,
+    create_continuous_q_function,
+    create_deterministic_policy,
     create_deterministic_residual_policy,
-    create_discrete_imitator,
-)
-from ...models.encoders import EncoderFactory
-from ...models.optimizers import OptimizerFactory
-from ...models.q_functions import QFunctionFactory
-from ...models.torch import (
-    ConditionalVAE,
-    DeterministicResidualPolicy,
-    DiscreteImitator,
-    PixelEncoder,
-    compute_max_with_n_actions,
 )
-from ...preprocessing import ActionScaler, RewardScaler, Scaler
-from ...torch_utility import TorchMiniBatch, torch_api, train_api
-from .ddpg_impl import DDPGBaseImpl
-from .dqn_impl import DoubleDQNImpl
-
-
-class BCQImpl(DDPGBaseImpl):
-
-    _imitator_learning_rate: float
-    _imitator_optim_factory: OptimizerFactory
-    _imitator_encoder_factory: EncoderFactory
-    _lam: float
-    _n_action_samples: int
-    _action_flexibility: float
-    _beta: float
-    _policy: Optional[DeterministicResidualPolicy]
-    _targ_policy: Optional[DeterministicResidualPolicy]
-    _imitator: Optional[ConditionalVAE]
-    _imitator_optim: Optional[Optimizer]
-
-    def __init__(
-        self,
-        observation_shape: Sequence[int],
-        action_size: int,
-        actor_learning_rate: float,
-        critic_learning_rate: float,
-        imitator_learning_rate: float,
-        actor_optim_factory: OptimizerFactory,
-        critic_optim_factory: OptimizerFactory,
-        imitator_optim_factory: OptimizerFactory,
-        actor_encoder_factory: EncoderFactory,
-        critic_encoder_factory: EncoderFactory,
-        imitator_encoder_factory: EncoderFactory,
-        q_func_factory: QFunctionFactory,
-        gamma: float,
-        tau: float,
-        n_critics: int,
-        lam: float,
-        n_action_samples: int,
-        action_flexibility: float,
-        beta: float,
-        use_gpu: Optional[Device],
-        scaler: Optional[Scaler],
-        action_scaler: Optional[ActionScaler],
-        reward_scaler: Optional[RewardScaler],
-    ):
-        super().__init__(
+from ...models.encoders import EncoderFactory, make_encoder_field
+from ...models.optimizers import OptimizerFactory, make_optimizer_field
+from ...models.q_functions import QFunctionFactory, make_q_func_field
+from ...torch_utility import TorchMiniBatch
+from .base import QLearningAlgoBase
+from .torch.plas_impl import PLASImpl, PLASWithPerturbationImpl
+
+__all__ = [
+    "PLASConfig",
+    "PLAS",
+    "PLASWithPerturbationConfig",
+    "PLASWithPerturbation",
+]
+
+
+@dataclasses.dataclass()
+class PLASConfig(LearnableConfig):
+    r"""Config of Policy in Latent Action Space algorithm.
+
+    PLAS is an offline deep reinforcement learning algorithm whose policy
+    function is trained in latent space of Conditional VAE.
+    Unlike other algorithms, PLAS can achieve good performance by using
+    its less constrained policy function.
+
+    .. math::
+
+       a \sim p_\beta (a|s, z=\pi_\phi(s))
+
+    where :math:`\beta` is a parameter of the decoder in Conditional VAE.
+
+    References:
+        * `Zhou et al., PLAS: latent action space for offline reinforcement
+          learning. <https://arxiv.org/abs/2011.07213>`_
+
+    Args:
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        action_scaler (d3rlpy.preprocessing.ActionScaler): Action preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        actor_learning_rate (float): Learning rate for policy function.
+        critic_learning_rate (float): Learning rate for Q functions.
+        imitator_learning_rate (float): Learning rate for Conditional VAE.
+        actor_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
+            Optimizer factory for the actor.
+        critic_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
+            Optimizer factory for the critic.
+        imitator_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
+            Optimizer factory for the conditional VAE.
+        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the actor.
+        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the critic.
+        imitator_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the conditional VAE.
+        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory):
+            Q function factory.
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        tau (float): Target network synchronization coefficiency.
+        n_critics (int): Number of Q functions for ensemble.
+        update_actor_interval (int): Interval to update policy function.
+        lam (float): Weight factor for critic ensemble.
+        warmup_steps (int): Number of steps to warmup the VAE.
+        beta (float): KL reguralization term for Conditional VAE.
+    """
+    actor_learning_rate: float = 1e-4
+    critic_learning_rate: float = 1e-3
+    imitator_learning_rate: float = 1e-4
+    actor_optim_factory: OptimizerFactory = make_optimizer_field()
+    critic_optim_factory: OptimizerFactory = make_optimizer_field()
+    imitator_optim_factory: OptimizerFactory = make_optimizer_field()
+    actor_encoder_factory: EncoderFactory = make_encoder_field()
+    critic_encoder_factory: EncoderFactory = make_encoder_field()
+    imitator_encoder_factory: EncoderFactory = make_encoder_field()
+    q_func_factory: QFunctionFactory = make_q_func_field()
+    batch_size: int = 100
+    gamma: float = 0.99
+    tau: float = 0.005
+    n_critics: int = 2
+    update_actor_interval: int = 1
+    lam: float = 0.75
+    warmup_steps: int = 500000
+    beta: float = 0.5
+
+    def create(self, device: DeviceArg = False) -> "PLAS":
+        return PLAS(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "plas"
+
+
+class PLAS(QLearningAlgoBase[PLASImpl, PLASConfig]):
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        policy = create_deterministic_policy(
+            observation_shape,
+            2 * action_size,
+            self._config.actor_encoder_factory,
+            device=self._device,
+        )
+        q_func = create_continuous_q_function(
+            observation_shape,
+            action_size,
+            self._config.critic_encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
+        imitator = create_conditional_vae(
             observation_shape=observation_shape,
             action_size=action_size,
-            actor_learning_rate=actor_learning_rate,
-            critic_learning_rate=critic_learning_rate,
-            actor_optim_factory=actor_optim_factory,
-            critic_optim_factory=critic_optim_factory,
-            actor_encoder_factory=actor_encoder_factory,
-            critic_encoder_factory=critic_encoder_factory,
-            q_func_factory=q_func_factory,
-            gamma=gamma,
-            tau=tau,
-            n_critics=n_critics,
-            use_gpu=use_gpu,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            reward_scaler=reward_scaler,
-        )
-        self._imitator_learning_rate = imitator_learning_rate
-        self._imitator_optim_factory = imitator_optim_factory
-        self._imitator_encoder_factory = imitator_encoder_factory
-        self._n_critics = n_critics
-        self._lam = lam
-        self._n_action_samples = n_action_samples
-        self._action_flexibility = action_flexibility
-        self._beta = beta
-
-        # initialized in build
-        self._imitator = None
-        self._imitator_optim = None
-
-    def build(self) -> None:
-        self._build_imitator()
-        super().build()
-        # setup optimizer after the parameters move to GPU
-        self._build_imitator_optim()
-
-    def _build_actor(self) -> None:
-        self._policy = create_deterministic_residual_policy(
-            self._observation_shape,
-            self._action_size,
-            self._action_flexibility,
-            self._actor_encoder_factory,
-        )
-
-    def _build_imitator(self) -> None:
-        self._imitator = create_conditional_vae(
-            observation_shape=self._observation_shape,
-            action_size=self._action_size,
-            latent_size=2 * self._action_size,
-            beta=self._beta,
+            latent_size=2 * action_size,
+            beta=self._config.beta,
             min_logstd=-4.0,
             max_logstd=15.0,
-            encoder_factory=self._imitator_encoder_factory,
+            encoder_factory=self._config.imitator_encoder_factory,
+            device=self._device,
         )
 
-    def _build_imitator_optim(self) -> None:
-        assert self._imitator is not None
-        self._imitator_optim = self._imitator_optim_factory.create(
-            self._imitator.parameters(), lr=self._imitator_learning_rate
-        )
-
-    def compute_actor_loss(self, batch: TorchMiniBatch) -> torch.Tensor:
-        assert self._imitator is not None
-        assert self._policy is not None
-        assert self._q_func is not None
-        latent = torch.randn(
-            batch.observations.shape[0],
-            2 * self._action_size,
-            device=self._device,
+        actor_optim = self._config.actor_optim_factory.create(
+            policy.parameters(), lr=self._config.actor_learning_rate
+        )
+        critic_optim = self._config.critic_optim_factory.create(
+            q_func.parameters(), lr=self._config.critic_learning_rate
         )
-        clipped_latent = latent.clamp(-0.5, 0.5)
-        sampled_action = self._imitator.decode(
-            batch.observations, clipped_latent
-        )
-        action = self._policy(batch.observations, sampled_action)
-        return -self._q_func(batch.observations, action, "none")[0].mean()
-
-    @train_api
-    @torch_api()
-    def update_imitator(self, batch: TorchMiniBatch) -> np.ndarray:
-        assert self._imitator_optim is not None
-        assert self._imitator is not None
-
-        self._imitator_optim.zero_grad()
-
-        loss = self._imitator.compute_error(batch.observations, batch.actions)
-
-        loss.backward()
-        self._imitator_optim.step()
-
-        return loss.cpu().detach().numpy()
-
-    def _repeat_observation(self, x: torch.Tensor) -> torch.Tensor:
-        # (batch_size, *obs_shape) -> (batch_size, n, *obs_shape)
-        repeat_shape = (x.shape[0], self._n_action_samples, *x.shape[1:])
-        repeated_x = x.view(x.shape[0], 1, *x.shape[1:]).expand(repeat_shape)
-        return repeated_x
-
-    def _sample_repeated_action(
-        self, repeated_x: torch.Tensor, target: bool = False
-    ) -> torch.Tensor:
-        assert self._imitator is not None
-        assert self._policy is not None
-        assert self._targ_policy is not None
-        # TODO: this seems to be slow with image observation
-        flattened_x = repeated_x.reshape(-1, *self.observation_shape)
-        # sample latent variable
-        latent = torch.randn(
-            flattened_x.shape[0], 2 * self._action_size, device=self._device
-        )
-        clipped_latent = latent.clamp(-0.5, 0.5)
-        # sample action
-        sampled_action = self._imitator.decode(flattened_x, clipped_latent)
-        # add residual action
-        policy = self._targ_policy if target else self._policy
-        action = policy(flattened_x, sampled_action)
-        return action.view(-1, self._n_action_samples, self._action_size)
-
-    def _predict_value(
-        self,
-        repeated_x: torch.Tensor,
-        action: torch.Tensor,
-    ) -> torch.Tensor:
-        assert self._q_func is not None
-        # TODO: this seems to be slow with image observation
-        # (batch_size, n, *obs_shape) -> (batch_size * n, *obs_shape)
-        flattened_x = repeated_x.reshape(-1, *self.observation_shape)
-        # (batch_size, n, action_size) -> (batch_size * n, action_size)
-        flattend_action = action.view(-1, self.action_size)
-        # estimate values
-        return self._q_func(flattened_x, flattend_action, "none")
-
-    def _predict_best_action(self, x: torch.Tensor) -> torch.Tensor:
-        # TODO: this seems to be slow with image observation
-        repeated_x = self._repeat_observation(x)
-        action = self._sample_repeated_action(repeated_x)
-        values = self._predict_value(repeated_x, action)[0]
-        # pick the best (batch_size * n) -> (batch_size,)
-        index = values.view(-1, self._n_action_samples).argmax(dim=1)
-        return action[torch.arange(action.shape[0]), index]
-
-    def _sample_action(self, x: torch.Tensor) -> torch.Tensor:
-        raise NotImplementedError("BCQ does not support sampling action")
-
-    def compute_target(self, batch: TorchMiniBatch) -> torch.Tensor:
-        assert self._targ_q_func is not None
-        # TODO: this seems to be slow with image observation
-        with torch.no_grad():
-            repeated_x = self._repeat_observation(batch.next_observations)
-            actions = self._sample_repeated_action(repeated_x, True)
-
-            values = compute_max_with_n_actions(
-                batch.next_observations, actions, self._targ_q_func, self._lam
-            )
-
-            return values
-
-
-class DiscreteBCQImpl(DoubleDQNImpl):
-
-    _action_flexibility: float
-    _beta: float
-    _imitator: Optional[DiscreteImitator]
-
-    def __init__(
-        self,
-        observation_shape: Sequence[int],
-        action_size: int,
-        learning_rate: float,
-        optim_factory: OptimizerFactory,
-        encoder_factory: EncoderFactory,
-        q_func_factory: QFunctionFactory,
-        gamma: float,
-        n_critics: int,
-        action_flexibility: float,
-        beta: float,
-        use_gpu: Optional[Device],
-        scaler: Optional[Scaler],
-        reward_scaler: Optional[RewardScaler],
-    ):
-        super().__init__(
+        imitator_optim = self._config.critic_optim_factory.create(
+            imitator.parameters(), lr=self._config.imitator_learning_rate
+        )
+
+        self._impl = PLASImpl(
             observation_shape=observation_shape,
             action_size=action_size,
-            learning_rate=learning_rate,
-            optim_factory=optim_factory,
-            encoder_factory=encoder_factory,
-            q_func_factory=q_func_factory,
-            gamma=gamma,
-            n_critics=n_critics,
-            use_gpu=use_gpu,
-            scaler=scaler,
-            reward_scaler=reward_scaler,
-        )
-        self._action_flexibility = action_flexibility
-        self._beta = beta
-
-        # initialized in build
-        self._imitator = None
-
-    def _build_network(self) -> None:
-        super()._build_network()
-        assert self._q_func is not None
-        # share convolutional layers if observation is pixel
-        if isinstance(self._q_func.q_funcs[0].encoder, PixelEncoder):
-            self._imitator = DiscreteImitator(
-                self._q_func.q_funcs[0].encoder, self._action_size, self._beta
-            )
+            policy=policy,
+            q_func=q_func,
+            imitator=imitator,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            imitator_optim=imitator_optim,
+            gamma=self._config.gamma,
+            tau=self._config.tau,
+            lam=self._config.lam,
+            device=self._device,
+        )
+
+    def inner_update(self, batch: TorchMiniBatch) -> Dict[str, float]:
+        assert self._impl is not None, IMPL_NOT_INITIALIZED_ERROR
+
+        metrics = {}
+
+        if self._grad_step < self._config.warmup_steps:
+            imitator_loss = self._impl.update_imitator(batch)
+            metrics.update({"imitator_loss": imitator_loss})
         else:
-            self._imitator = create_discrete_imitator(
-                self._observation_shape,
-                self._action_size,
-                self._beta,
-                self._encoder_factory,
-            )
-
-    def _build_optim(self) -> None:
-        assert self._q_func is not None
-        assert self._imitator is not None
-        q_func_params = list(self._q_func.parameters())
-        imitator_params = list(self._imitator.parameters())
-
-        # TODO: replace this with a cleaner way
-        # retrieve unique elements
-        unique_dict = {}
-        for param in q_func_params + imitator_params:
-            unique_dict[param] = param
-        unique_params = list(unique_dict.values())
-
-        self._optim = self._optim_factory.create(
-            unique_params, lr=self._learning_rate
-        )
-
-    def compute_loss(
-        self, batch: TorchMiniBatch, q_tpn: torch.Tensor
-    ) -> torch.Tensor:
-        assert self._imitator is not None
-        loss = super().compute_loss(batch, q_tpn)
-        imitator_loss = self._imitator.compute_error(
-            batch.observations, batch.actions.long()
-        )
-        return loss + imitator_loss
-
-    def _predict_best_action(self, x: torch.Tensor) -> torch.Tensor:
-        assert self._imitator is not None
-        assert self._q_func is not None
-        log_probs = self._imitator(x)
-        ratio = log_probs - log_probs.max(dim=1, keepdim=True).values
-        mask = (ratio > math.log(self._action_flexibility)).float()
-        value = self._q_func(x)
-        normalized_value = value - value.min(dim=1, keepdim=True).values
-        action = (normalized_value * cast(torch.Tensor, mask)).argmax(dim=1)
-        return action
+            critic_loss = self._impl.update_critic(batch)
+            metrics.update({"critic_loss": critic_loss})
+            if self._grad_step % self._config.update_actor_interval == 0:
+                actor_loss = self._impl.update_actor(batch)
+                metrics.update({"actor_loss": actor_loss})
+                self._impl.update_actor_target()
+                self._impl.update_critic_target()
+
+        return metrics
+
+    def get_action_type(self) -> ActionSpace:
+        return ActionSpace.CONTINUOUS
+
+
+@dataclasses.dataclass()
+class PLASWithPerturbationConfig(PLASConfig):
+    r"""Config of Policy in Latent Action Space algorithm with perturbation
+    layer.
+
+    PLAS with perturbation layer enables PLAS to output out-of-distribution
+    action.
+
+    References:
+        * `Zhou et al., PLAS: latent action space for offline reinforcement
+          learning. <https://arxiv.org/abs/2011.07213>`_
+
+    Args:
+        observation_scaler (d3rlpy.preprocessing.ObservationScaler):
+            Observation preprocessor.
+        action_scaler (d3rlpy.preprocessing.ActionScaler): Action preprocessor.
+        reward_scaler (d3rlpy.preprocessing.RewardScaler): Reward preprocessor.
+        actor_learning_rate (float): Learning rate for policy function.
+        critic_learning_rate (float): Learning rate for Q functions.
+        imitator_learning_rate (float): Learning rate for Conditional VAE.
+        actor_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
+            Optimizer factory for the actor.
+        critic_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
+            Optimizer factory for the critic.
+        imitator_optim_factory (d3rlpy.models.optimizers.OptimizerFactory):
+            Optimizer factory for the conditional VAE.
+        actor_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the actor.
+        critic_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the critic.
+        imitator_encoder_factory (d3rlpy.models.encoders.EncoderFactory):
+            Encoder factory for the conditional VAE.
+        q_func_factory (d3rlpy.models.q_functions.QFunctionFactory):
+            Q function factory.
+        batch_size (int): Mini-batch size.
+        gamma (float): Discount factor.
+        tau (float): Target network synchronization coefficiency.
+        n_critics (int): Number of Q functions for ensemble.
+        update_actor_interval (int): Interval to update policy function.
+        lam (float): Weight factor for critic ensemble.
+        action_flexibility (float): Output scale of perturbation layer.
+        warmup_steps (int): Number of steps to warmup the VAE.
+        beta (float): KL reguralization term for Conditional VAE.
+    """
+    action_flexibility: float = 0.05
+
+    def create(self, device: DeviceArg = False) -> "PLASWithPerturbation":
+        return PLASWithPerturbation(self, device)
+
+    @staticmethod
+    def get_type() -> str:
+        return "plas_with_perturbation"
+
+
+class PLASWithPerturbation(PLAS):
+    _config: PLASWithPerturbationConfig
+
+    def inner_create_impl(
+        self, observation_shape: Shape, action_size: int
+    ) -> None:
+        policy = create_deterministic_policy(
+            observation_shape,
+            2 * action_size,
+            self._config.actor_encoder_factory,
+            device=self._device,
+        )
+        q_func = create_continuous_q_function(
+            observation_shape,
+            action_size,
+            self._config.critic_encoder_factory,
+            self._config.q_func_factory,
+            n_ensembles=self._config.n_critics,
+            device=self._device,
+        )
+        imitator = create_conditional_vae(
+            observation_shape=observation_shape,
+            action_size=action_size,
+            latent_size=2 * action_size,
+            beta=self._config.beta,
+            min_logstd=-4.0,
+            max_logstd=15.0,
+            encoder_factory=self._config.imitator_encoder_factory,
+            device=self._device,
+        )
+        perturbation = create_deterministic_residual_policy(
+            observation_shape=observation_shape,
+            action_size=action_size,
+            scale=self._config.action_flexibility,
+            encoder_factory=self._config.actor_encoder_factory,
+            device=self._device,
+        )
+
+        parameters = list(policy.parameters())
+        parameters += list(perturbation.parameters())
+        actor_optim = self._config.actor_optim_factory.create(
+            params=parameters, lr=self._config.actor_learning_rate
+        )
+        critic_optim = self._config.critic_optim_factory.create(
+            q_func.parameters(), lr=self._config.critic_learning_rate
+        )
+        imitator_optim = self._config.critic_optim_factory.create(
+            imitator.parameters(), lr=self._config.imitator_learning_rate
+        )
+
+        self._impl = PLASWithPerturbationImpl(
+            observation_shape=observation_shape,
+            action_size=action_size,
+            policy=policy,
+            q_func=q_func,
+            imitator=imitator,
+            perturbation=perturbation,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            imitator_optim=imitator_optim,
+            gamma=self._config.gamma,
+            tau=self._config.tau,
+            lam=self._config.lam,
+            device=self._device,
+        )
+
+
+register_learnable(PLASConfig)
+register_learnable(PLASWithPerturbationConfig)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/algos/torch/bear_impl.py` & `d3rlpy-2.0.2/d3rlpy/models/torch/encoders.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,329 +1,352 @@
-import math
-from typing import Optional, Sequence
+from abc import ABCMeta, abstractmethod
+from typing import List, Optional, Sequence
 
-import numpy as np
 import torch
-from torch.optim import Optimizer
+import torch.nn.functional as F
+from torch import nn
 
-from ...gpu import Device
-from ...models.builders import create_conditional_vae, create_parameter
-from ...models.encoders import EncoderFactory
-from ...models.optimizers import OptimizerFactory
-from ...models.q_functions import QFunctionFactory
-from ...models.torch import (
-    ConditionalVAE,
-    Parameter,
-    compute_max_with_n_actions_and_indices,
-)
-from ...preprocessing import ActionScaler, RewardScaler, Scaler
-from ...torch_utility import TorchMiniBatch, torch_api, train_api
-from .sac_impl import SACImpl
-
-
-def _gaussian_kernel(
-    x: torch.Tensor, y: torch.Tensor, sigma: float
-) -> torch.Tensor:
-    # x: (batch, n, 1, action), y: (batch, 1, n, action) -> (batch, n, n)
-    return (-((x - y) ** 2).sum(dim=3) / (2 * sigma)).exp()
-
-
-def _laplacian_kernel(
-    x: torch.Tensor, y: torch.Tensor, sigma: float
-) -> torch.Tensor:
-    # x: (batch, n, 1, action), y: (batch, 1, n, action) -> (batch, n, n)
-    return (-(x - y).abs().sum(dim=3) / (2 * sigma)).exp()
-
-
-class BEARImpl(SACImpl):
-
-    _imitator_learning_rate: float
-    _alpha_learning_rate: float
-    _imitator_optim_factory: OptimizerFactory
-    _alpha_optim_factory: OptimizerFactory
-    _imitator_encoder_factory: EncoderFactory
-    _initial_alpha: float
-    _alpha_threshold: float
-    _lam: float
-    _n_action_samples: int
-    _n_target_samples: int
-    _n_mmd_action_samples: int
-    _mmd_kernel: str
-    _mmd_sigma: float
-    _vae_kl_weight: float
-    _imitator: Optional[ConditionalVAE]
-    _imitator_optim: Optional[Optimizer]
-    _log_alpha: Optional[Parameter]
-    _alpha_optim: Optional[Optimizer]
+from ...itertools import last_flag
+
+__all__ = [
+    "Encoder",
+    "EncoderWithAction",
+    "PixelEncoder",
+    "PixelEncoderWithAction",
+    "VectorEncoder",
+    "VectorEncoderWithAction",
+]
+
+
+class Encoder(metaclass=ABCMeta):
+    @abstractmethod
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        pass
+
+    @abstractmethod
+    def get_feature_size(self) -> int:
+        pass
+
+    @property
+    @abstractmethod
+    def observation_shape(self) -> Sequence[int]:
+        pass
+
+    @abstractmethod
+    def __call__(self, x: torch.Tensor) -> torch.Tensor:
+        pass
+
+
+class EncoderWithAction(metaclass=ABCMeta):
+    @abstractmethod
+    def forward(self, x: torch.Tensor, action: torch.Tensor) -> torch.Tensor:
+        pass
+
+    @abstractmethod
+    def get_feature_size(self) -> int:
+        pass
+
+    @property
+    @abstractmethod
+    def action_size(self) -> int:
+        pass
+
+    @property
+    @abstractmethod
+    def observation_shape(self) -> Sequence[int]:
+        pass
+
+    @abstractmethod
+    def __call__(self, x: torch.Tensor, action: torch.Tensor) -> torch.Tensor:
+        pass
+
+
+class _PixelEncoder(nn.Module):  # type: ignore
+    _observation_shape: Sequence[int]
+    _feature_size: int
+    _use_batch_norm: bool
+    _dropout_rate: Optional[float]
+    _activation: nn.Module
+    _convs: nn.ModuleList
+    _conv_bns: nn.ModuleList
+    _fc: nn.Linear
+    _fc_bn: nn.BatchNorm1d
+    _dropouts: nn.ModuleList
+    _exclude_last_activation: bool
 
     def __init__(
         self,
         observation_shape: Sequence[int],
-        action_size: int,
-        actor_learning_rate: float,
-        critic_learning_rate: float,
-        imitator_learning_rate: float,
-        temp_learning_rate: float,
-        alpha_learning_rate: float,
-        actor_optim_factory: OptimizerFactory,
-        critic_optim_factory: OptimizerFactory,
-        imitator_optim_factory: OptimizerFactory,
-        temp_optim_factory: OptimizerFactory,
-        alpha_optim_factory: OptimizerFactory,
-        actor_encoder_factory: EncoderFactory,
-        critic_encoder_factory: EncoderFactory,
-        imitator_encoder_factory: EncoderFactory,
-        q_func_factory: QFunctionFactory,
-        gamma: float,
-        tau: float,
-        n_critics: int,
-        initial_temperature: float,
-        initial_alpha: float,
-        alpha_threshold: float,
-        lam: float,
-        n_action_samples: int,
-        n_target_samples: int,
-        n_mmd_action_samples: int,
-        mmd_kernel: str,
-        mmd_sigma: float,
-        vae_kl_weight: float,
-        use_gpu: Optional[Device],
-        scaler: Optional[Scaler],
-        action_scaler: Optional[ActionScaler],
-        reward_scaler: Optional[RewardScaler],
+        filters: Optional[List[List[int]]] = None,
+        feature_size: int = 512,
+        use_batch_norm: bool = False,
+        dropout_rate: Optional[float] = False,
+        activation: nn.Module = nn.ReLU(),
+        exclude_last_activation: bool = False,
     ):
-        super().__init__(
-            observation_shape=observation_shape,
-            action_size=action_size,
-            actor_learning_rate=actor_learning_rate,
-            critic_learning_rate=critic_learning_rate,
-            temp_learning_rate=temp_learning_rate,
-            actor_optim_factory=actor_optim_factory,
-            critic_optim_factory=critic_optim_factory,
-            temp_optim_factory=temp_optim_factory,
-            actor_encoder_factory=actor_encoder_factory,
-            critic_encoder_factory=critic_encoder_factory,
-            q_func_factory=q_func_factory,
-            gamma=gamma,
-            tau=tau,
-            n_critics=n_critics,
-            initial_temperature=initial_temperature,
-            use_gpu=use_gpu,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            reward_scaler=reward_scaler,
-        )
-        self._imitator_learning_rate = imitator_learning_rate
-        self._alpha_learning_rate = alpha_learning_rate
-        self._imitator_optim_factory = imitator_optim_factory
-        self._alpha_optim_factory = alpha_optim_factory
-        self._imitator_encoder_factory = imitator_encoder_factory
-        self._initial_alpha = initial_alpha
-        self._alpha_threshold = alpha_threshold
-        self._lam = lam
-        self._n_action_samples = n_action_samples
-        self._n_target_samples = n_target_samples
-        self._n_mmd_action_samples = n_mmd_action_samples
-        self._mmd_kernel = mmd_kernel
-        self._mmd_sigma = mmd_sigma
-        self._vae_kl_weight = vae_kl_weight
-
-        # initialized in build
-        self._imitator = None
-        self._imitator_optim = None
-        self._log_alpha = None
-        self._alpha_optim = None
-
-    def build(self) -> None:
-        self._build_imitator()
-        self._build_alpha()
-        super().build()
-        self._build_imitator_optim()
-        self._build_alpha_optim()
-
-    def _build_imitator(self) -> None:
-        self._imitator = create_conditional_vae(
-            observation_shape=self._observation_shape,
-            action_size=self._action_size,
-            latent_size=2 * self._action_size,
-            beta=self._vae_kl_weight,
-            min_logstd=-4.0,
-            max_logstd=15.0,
-            encoder_factory=self._imitator_encoder_factory,
-        )
-
-    def _build_imitator_optim(self) -> None:
-        assert self._imitator is not None
-        self._imitator_optim = self._imitator_optim_factory.create(
-            self._imitator.parameters(), lr=self._imitator_learning_rate
-        )
-
-    def _build_alpha(self) -> None:
-        initial_val = math.log(self._initial_alpha)
-        self._log_alpha = create_parameter((1, 1), initial_val)
-
-    def _build_alpha_optim(self) -> None:
-        assert self._log_alpha is not None
-        self._alpha_optim = self._alpha_optim_factory.create(
-            self._log_alpha.parameters(), lr=self._alpha_learning_rate
-        )
-
-    def compute_actor_loss(self, batch: TorchMiniBatch) -> torch.Tensor:
-        loss = super().compute_actor_loss(batch)
-        mmd_loss = self._compute_mmd_loss(batch.observations)
-        return loss + mmd_loss
-
-    @train_api
-    @torch_api()
-    def warmup_actor(self, batch: TorchMiniBatch) -> np.ndarray:
-        assert self._actor_optim is not None
-
-        self._actor_optim.zero_grad()
-
-        loss = self._compute_mmd_loss(batch.observations)
-
-        loss.backward()
-        self._actor_optim.step()
+        super().__init__()
 
-        return loss.cpu().detach().numpy()
-
-    def _compute_mmd_loss(self, obs_t: torch.Tensor) -> torch.Tensor:
-        assert self._log_alpha
-        mmd = self._compute_mmd(obs_t)
-        alpha = self._log_alpha().exp()
-        return (alpha * (mmd - self._alpha_threshold)).mean()
-
-    @train_api
-    @torch_api()
-    def update_imitator(self, batch: TorchMiniBatch) -> np.ndarray:
-        assert self._imitator_optim is not None
-
-        self._imitator_optim.zero_grad()
-
-        loss = self.compute_imitator_loss(batch)
-
-        loss.backward()
-
-        self._imitator_optim.step()
-
-        return loss.cpu().detach().numpy()
-
-    def compute_imitator_loss(self, batch: TorchMiniBatch) -> torch.Tensor:
-        assert self._imitator is not None
-        return self._imitator.compute_error(batch.observations, batch.actions)
-
-    @train_api
-    @torch_api()
-    def update_alpha(self, batch: TorchMiniBatch) -> np.ndarray:
-        assert self._alpha_optim is not None
-        assert self._log_alpha is not None
-
-        loss = -self._compute_mmd_loss(batch.observations)
-
-        self._alpha_optim.zero_grad()
-        loss.backward()
-        self._alpha_optim.step()
-
-        # clip for stability
-        self._log_alpha.data.clamp_(-5.0, 10.0)
+        # default architecture is based on Nature DQN paper.
+        if filters is None:
+            filters = [[32, 8, 4], [64, 4, 2], [64, 3, 1]]
+        if feature_size is None:
+            feature_size = 512
+
+        self._observation_shape = observation_shape
+        self._use_batch_norm = use_batch_norm
+        self._dropout_rate = dropout_rate
+        self._activation = activation
+        self._feature_size = feature_size
+        self._exclude_last_activation = exclude_last_activation
+
+        # convolutional layers
+        in_channels = [observation_shape[0]] + [f[0] for f in filters[:-1]]
+        self._convs = nn.ModuleList()
+        self._conv_bns = nn.ModuleList()
+        self._dropouts = nn.ModuleList()
+        for in_channel, f in zip(in_channels, filters):
+            out_channel, kernel_size, stride = f
+            conv = nn.Conv2d(
+                in_channel, out_channel, kernel_size=kernel_size, stride=stride
+            )
+            self._convs.append(conv)
 
-        cur_alpha = self._log_alpha().exp().cpu().detach().numpy()[0][0]
+            # use batch normalization layer
+            if use_batch_norm:
+                self._conv_bns.append(nn.BatchNorm2d(out_channel))
+
+            # use dropout layer
+            if dropout_rate is not None:
+                self._dropouts.append(nn.Dropout2d(dropout_rate))
+
+        # last dense layer
+        self._fc = nn.Linear(self._get_linear_input_size(), feature_size)
+        if use_batch_norm:
+            self._fc_bn = nn.BatchNorm1d(feature_size)
+        if dropout_rate is not None:
+            self._dropouts.append(nn.Dropout(dropout_rate))
 
-        return loss.cpu().detach().numpy(), cur_alpha
+    def _get_linear_input_size(self) -> int:
+        x = torch.rand((1,) + tuple(self._observation_shape))
+        with torch.no_grad():
+            return self._conv_encode(x).view(1, -1).shape[1]  # type: ignore
 
-    def _compute_mmd(self, x: torch.Tensor) -> torch.Tensor:
-        assert self._imitator is not None
-        assert self._policy is not None
+    def _get_last_conv_shape(self) -> Sequence[int]:
+        x = torch.rand((1,) + tuple(self._observation_shape))
         with torch.no_grad():
-            behavior_actions = self._imitator.sample_n_without_squash(
-                x, self._n_mmd_action_samples
-            )
-        policy_actions = self._policy.sample_n_without_squash(
-            x, self._n_mmd_action_samples
-        )
+            return self._conv_encode(x).shape  # type: ignore
 
-        if self._mmd_kernel == "gaussian":
-            kernel = _gaussian_kernel
-        elif self._mmd_kernel == "laplacian":
-            kernel = _laplacian_kernel
-        else:
-            raise ValueError(f"Invalid kernel type: {self._mmd_kernel}")
-
-        # (batch, n, action) -> (batch, n, 1, action)
-        behavior_actions = behavior_actions.reshape(
-            x.shape[0], -1, 1, self.action_size
-        )
-        policy_actions = policy_actions.reshape(
-            x.shape[0], -1, 1, self.action_size
-        )
-        # (batch, n, action) -> (batch, 1, n, action)
-        behavior_actions_T = behavior_actions.reshape(
-            x.shape[0], 1, -1, self.action_size
-        )
-        policy_actions_T = policy_actions.reshape(
-            x.shape[0], 1, -1, self.action_size
-        )
+    def _conv_encode(self, x: torch.Tensor) -> torch.Tensor:
+        h = x
+        for i, conv in enumerate(self._convs):
+            h = self._activation(conv(h))
+            if self._use_batch_norm:
+                h = self._conv_bns[i](h)
+            if self._dropout_rate is not None:
+                h = self._dropouts[i](h)
+        return h
+
+    def get_feature_size(self) -> int:
+        return self._feature_size
+
+    @property
+    def observation_shape(self) -> Sequence[int]:
+        return self._observation_shape
+
+
+class PixelEncoder(_PixelEncoder, Encoder):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        h = self._conv_encode(x)
+
+        h = self._fc(h.view(h.shape[0], -1))
+        if not self._exclude_last_activation:
+            h = self._activation(h)
+        if self._use_batch_norm:
+            h = self._fc_bn(h)
+        if self._dropout_rate is not None:
+            h = self._dropouts[-1](h)
+
+        return h
+
+
+class PixelEncoderWithAction(_PixelEncoder, EncoderWithAction):
+    _action_size: int
+    _discrete_action: bool
 
-        # 1 / N^2 \sum k(a_\pi, a_\pi)
-        inter_policy = kernel(policy_actions, policy_actions_T, self._mmd_sigma)
-        mmd = inter_policy.mean(dim=[1, 2])
-
-        # 1 / N^2 \sum k(a_\beta, a_\beta)
-        inter_data = kernel(
-            behavior_actions, behavior_actions_T, self._mmd_sigma
+    def __init__(
+        self,
+        observation_shape: Sequence[int],
+        action_size: int,
+        filters: Optional[List[List[int]]] = None,
+        feature_size: int = 512,
+        use_batch_norm: bool = False,
+        dropout_rate: Optional[float] = None,
+        discrete_action: bool = False,
+        activation: nn.Module = nn.ReLU(),
+        exclude_last_activation: bool = False,
+    ):
+        self._action_size = action_size
+        self._discrete_action = discrete_action
+        super().__init__(
+            observation_shape=observation_shape,
+            filters=filters,
+            feature_size=feature_size,
+            use_batch_norm=use_batch_norm,
+            dropout_rate=dropout_rate,
+            activation=activation,
+            exclude_last_activation=exclude_last_activation,
         )
-        mmd += inter_data.mean(dim=[1, 2])
 
-        # 2 / N^2 \sum k(a_\pi, a_\beta)
-        distance = kernel(policy_actions, behavior_actions_T, self._mmd_sigma)
-        mmd -= 2 * distance.mean(dim=[1, 2])
-
-        return (mmd + 1e-6).sqrt().view(-1, 1)
-
-    def compute_target(self, batch: TorchMiniBatch) -> torch.Tensor:
-        assert self._policy is not None
-        assert self._targ_q_func is not None
-        assert self._log_temp is not None
-        with torch.no_grad():
-            # BCQ-like target computation
-            actions, log_probs = self._policy.sample_n_with_log_prob(
-                batch.next_observations,
-                self._n_target_samples,
-            )
-            values, indices = compute_max_with_n_actions_and_indices(
-                batch.next_observations, actions, self._targ_q_func, self._lam
-            )
+    def _get_linear_input_size(self) -> int:
+        size = super()._get_linear_input_size()
+        return size + self._action_size
+
+    def forward(self, x: torch.Tensor, action: torch.Tensor) -> torch.Tensor:
+        h = self._conv_encode(x)
+
+        if self._discrete_action:
+            action = F.one_hot(
+                action.view(-1).long(), num_classes=self._action_size
+            ).float()
+
+        # cocat feature and action
+        h = self._fc(torch.cat([h.view(h.shape[0], -1), action], dim=1))
+        if not self._exclude_last_activation:
+            h = self._activation(h)
+        if self._use_batch_norm:
+            h = self._fc_bn(h)
+        if self._dropout_rate is not None:
+            h = self._dropouts[-1](h)
+
+        return h
+
+    @property
+    def action_size(self) -> int:
+        return self._action_size
+
+
+class _VectorEncoder(nn.Module):  # type: ignore
+    _observation_shape: Sequence[int]
+    _use_batch_norm: bool
+    _dropout_rate: Optional[float]
+    _use_dense: bool
+    _activation: nn.Module
+    _feature_size: int
+    _fcs: nn.ModuleList
+    _bns: nn.ModuleList
+    _dropouts: nn.ModuleList
+    _exclude_last_activation: bool
 
-            # (batch, n, 1) -> (batch, 1)
-            batch_size = batch.observations.shape[0]
-            max_log_prob = log_probs[torch.arange(batch_size), indices]
-
-            return values - self._log_temp().exp() * max_log_prob
-
-    def _predict_best_action(self, x: torch.Tensor) -> torch.Tensor:
-        assert self._policy is not None
-        assert self._q_func is not None
-        with torch.no_grad():
-            # (batch, n, action)
-            actions = self._policy.onnx_safe_sample_n(x, self._n_action_samples)
-            # (batch, n, action) -> (batch * n, action)
-            flat_actions = actions.reshape(-1, self._action_size)
-
-            # (batch, observation) -> (batch, 1, observation)
-            expanded_x = x.view(x.shape[0], 1, *x.shape[1:])
-            # (batch, 1, observation) -> (batch, n, observation)
-            repeated_x = expanded_x.expand(
-                x.shape[0], self._n_action_samples, *x.shape[1:]
-            )
-            # (batch, n, observation) -> (batch * n, observation)
-            flat_x = repeated_x.reshape(-1, *x.shape[1:])
+    def __init__(
+        self,
+        observation_shape: Sequence[int],
+        hidden_units: Optional[Sequence[int]] = None,
+        use_batch_norm: bool = False,
+        dropout_rate: Optional[float] = None,
+        use_dense: bool = False,
+        activation: nn.Module = nn.ReLU(),
+        exclude_last_activation: bool = False,
+    ):
+        super().__init__()
+        self._observation_shape = observation_shape
 
-            # (batch * n, 1)
-            flat_values = self._q_func(flat_x, flat_actions, "none")[0]
+        if hidden_units is None:
+            hidden_units = [256, 256]
 
-            # (batch, n)
-            values = flat_values.view(x.shape[0], self._n_action_samples)
+        self._use_batch_norm = use_batch_norm
+        self._dropout_rate = dropout_rate
+        self._feature_size = hidden_units[-1]
+        self._activation = activation
+        self._use_dense = use_dense
+        self._exclude_last_activation = exclude_last_activation
+
+        in_units = [observation_shape[0]] + list(hidden_units[:-1])
+        self._fcs = nn.ModuleList()
+        self._bns = nn.ModuleList()
+        self._dropouts = nn.ModuleList()
+        for i, (in_unit, out_unit) in enumerate(zip(in_units, hidden_units)):
+            if use_dense and i > 0:
+                in_unit += observation_shape[0]
+            self._fcs.append(nn.Linear(in_unit, out_unit))
+            if use_batch_norm:
+                self._bns.append(nn.BatchNorm1d(out_unit))
+            if dropout_rate is not None:
+                self._dropouts.append(nn.Dropout(dropout_rate))
+
+    def _fc_encode(self, x: torch.Tensor) -> torch.Tensor:
+        h = x
+        for is_last, (i, fc) in last_flag(enumerate(self._fcs)):
+            if self._use_dense and i > 0:
+                h = torch.cat([h, x], dim=1)
+            h = fc(h)
+            if not is_last or not self._exclude_last_activation:
+                h = self._activation(h)
+            if self._use_batch_norm:
+                h = self._bns[i](h)
+            if self._dropout_rate is not None:
+                h = self._dropouts[i](h)
+        return h
+
+    def get_feature_size(self) -> int:
+        return self._feature_size
+
+    @property
+    def observation_shape(self) -> Sequence[int]:
+        return self._observation_shape
+
+
+class VectorEncoder(_VectorEncoder, Encoder):
+    def forward(self, x: torch.Tensor) -> torch.Tensor:
+        h = self._fc_encode(x)
+        if self._use_batch_norm:
+            h = self._bns[-1](h)
+        if self._dropout_rate is not None:
+            h = self._dropouts[-1](h)
+        return h
+
+
+class VectorEncoderWithAction(_VectorEncoder, EncoderWithAction):
+    _action_size: int
+    _discrete_action: bool
 
-            # (batch, n) -> (batch,)
-            max_indices = torch.argmax(values, dim=1)
+    def __init__(
+        self,
+        observation_shape: Sequence[int],
+        action_size: int,
+        hidden_units: Optional[Sequence[int]] = None,
+        use_batch_norm: bool = False,
+        dropout_rate: Optional[float] = None,
+        use_dense: bool = False,
+        discrete_action: bool = False,
+        activation: nn.Module = nn.ReLU(),
+        exclude_last_activation: bool = False,
+    ):
+        self._action_size = action_size
+        self._discrete_action = discrete_action
+        concat_shape = (observation_shape[0] + action_size,)
+        super().__init__(
+            observation_shape=concat_shape,
+            hidden_units=hidden_units,
+            use_batch_norm=use_batch_norm,
+            use_dense=use_dense,
+            dropout_rate=dropout_rate,
+            activation=activation,
+            exclude_last_activation=exclude_last_activation,
+        )
+        self._observation_shape = observation_shape
 
-            return actions[torch.arange(x.shape[0]), max_indices]
+    def forward(self, x: torch.Tensor, action: torch.Tensor) -> torch.Tensor:
+        if self._discrete_action:
+            action = F.one_hot(
+                action.view(-1).long(), num_classes=self.action_size
+            ).float()
+        x = torch.cat([x, action], dim=1)
+        h = self._fc_encode(x)
+        if self._use_batch_norm:
+            h = self._bns[-1](h)
+        if self._dropout_rate is not None:
+            h = self._dropouts[-1](h)
+        return h
+
+    @property
+    def action_size(self) -> int:
+        return self._action_size
```

### Comparing `d3rlpy-1.1.1/d3rlpy/cli.py` & `d3rlpy-2.0.2/d3rlpy/cli.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,31 @@
 # pylint: disable=redefined-builtin,exec-used
+# type: ignore
 
 import glob
 import json
 import os
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Sequence, Tuple
 
 import click
 import gym
 import numpy as np
-from scipy.ndimage.filters import uniform_filter1d
 
-from . import algos
 from ._version import __version__
+from .algos import (
+    QLearningAlgoBase,
+    StatefulTransformerWrapper,
+    TransformerAlgoBase,
+)
+from .base import load_learnable
 from .envs import Monitor
-from .metrics.scorer import evaluate_on_environment
+from .metrics.utility import (
+    evaluate_qlearning_with_environment,
+    evaluate_transformer_with_environment,
+)
 
 if TYPE_CHECKING:
     import matplotlib.pyplot
 
 
 def print_stats(path: str) -> None:
     data = np.loadtxt(path, delimiter=",")
@@ -38,14 +46,24 @@
 
         sns.set()
     except ImportError:
         pass
     return plt
 
 
+def _compute_moving_average(values: np.ndarray, window: int) -> np.ndarray:
+    assert values.ndim == 1
+    results: List[float] = []
+    # average over past data
+    for i in range(values.shape[0]):
+        start = max(0, i - window)
+        results.append(float(np.mean(values[start : i + 1])))
+    return np.array(results)
+
+
 @click.group()
 def cli() -> None:
     print(f"d3rlpy command line interface (Version {__version__})")
 
 
 @cli.command(short_help="Show statistics of save metrics.")
 @click.argument("path")
@@ -89,15 +107,15 @@
             path
         ), "--labels must be provided as many as the number of paths"
 
     for i, p in enumerate(path):
         data = np.loadtxt(p, delimiter=",")
 
         # filter to smooth data
-        y_data = uniform_filter1d(data[:, 2], size=window)
+        y_data = _compute_moving_average(data[:, 2], window)
 
         # create label
         if label:
             _label = label[i]
         elif len(p.split(os.sep)) > 1:
             _label = "/".join(p.split(os.sep)[-2:])
         else:
@@ -190,116 +208,74 @@
     plt.tight_layout()
     if save:
         plt.savefig(save)
     else:
         plt.show()
 
 
-def _get_params_json_path(path: str) -> str:
-    dirname = os.path.dirname(path)
-    if not os.path.exists(os.path.join(dirname, "params.json")):
-        raise RuntimeError(
-            "params.json is not found in %s. Please specify"
-            "the path to params.json by --params-json."
-        )
-    return os.path.join(dirname, "params.json")
-
-
-@cli.command(short_help="Export saved model as inference model format.")
-@click.argument("path")
-@click.option(
-    "--format",
-    default="onnx",
-    show_default=True,
-    help="model format (torchscript, onnx).",
-)
-@click.option(
-    "--params-json", default=None, help="explicitly specify params.json."
+@cli.command(
+    short_help="Export saved model as inference model format (ONNX or TorchScript)."
 )
-@click.option("--out", default=None, help="output path.")
-def export(
-    path: str, format: str, params_json: Optional[str], out: Optional[str]
-) -> None:
-    # check format
-    if format not in ["onnx", "torchscript"]:
-        raise ValueError("Please specify onnx or torchscript.")
-
-    # find params.json
-    if params_json is None:
-        params_json = _get_params_json_path(path)
-
-    # load params
-    with open(params_json, "r") as f:
-        params = json.loads(f.read())
-
+@click.argument("model_path")
+@click.argument("output_path")
+def export(model_path: str, output_path: str) -> None:
     # load saved model
-    print(f"Loading {path}...")
-    algo = getattr(algos, params["algorithm"]).from_json(params_json)
-    algo.load_model(path)
-
-    if out is None:
-        ext = "onnx" if format == "onnx" else "torchscript"
-        export_name = os.path.splitext(os.path.basename(path))[0]
-        out = os.path.join(os.path.dirname(path), export_name + "." + ext)
+    print(f"Loading {model_path}...")
+    algo = load_learnable(model_path)
+    assert isinstance(
+        algo, QLearningAlgoBase
+    ), "Currently, only Q-learning algorithms are supported."
 
     # export inference model
-    print(f"Exporting to {out}...")
-    algo.save_policy(out, as_onnx=format == "onnx")
+    print(f"Exporting to {output_path}...")
+    algo.save_policy(output_path)
 
 
-def _exec_to_create_env(code: str) -> gym.Env:
+def _exec_to_create_env(code: str) -> gym.Env[Any, Any]:
     print(f"Executing '{code}'")
     variables: Dict[str, Any] = {}
     exec(code, globals(), variables)
     if "env" not in variables:
         raise RuntimeError("env must be defined in env_header.")
-    return variables["env"]
+    return variables["env"]  # type: ignore
 
 
 @cli.command(short_help="Record episodes with the saved model.")
 @click.argument("model_path")
 @click.option("--env-id", default=None, help="Gym environment id.")
 @click.option(
     "--env-header", default=None, help="one-liner to create environment."
 )
 @click.option("--out", default="videos", help="output directory path.")
 @click.option(
-    "--params-json", default=None, help="explicityly specify params.json."
-)
-@click.option(
     "--n-episodes", default=3, help="the number of episodes to record."
 )
 @click.option("--frame-rate", default=60, help="video frame rate.")
 @click.option("--record-rate", default=1, help="record frame rate.")
-@click.option("--epsilon", default=0.0, help="epsilon-greedy evaluation.")
+@click.option(
+    "--target-return",
+    default=None,
+    help="the target return for Decision Transformer variants.",
+)
 def record(
     model_path: str,
     env_id: Optional[str],
     env_header: Optional[str],
-    params_json: Optional[str],
     out: str,
     n_episodes: int,
     frame_rate: float,
     record_rate: int,
-    epsilon: float,
+    target_return: Optional[float],
 ) -> None:
-    if params_json is None:
-        params_json = _get_params_json_path(model_path)
-
-    # load params
-    with open(params_json, "r") as f:
-        params = json.loads(f.read())
-
     # load saved model
     print(f"Loading {model_path}...")
-    algo = getattr(algos, params["algorithm"]).from_json(params_json)
-    algo.load_model(model_path)
+    algo = load_learnable(model_path)
 
     # wrap environment with Monitor
-    env: gym.Env
+    env: gym.Env[Any, Any]
     if env_id is not None:
         env = gym.make(env_id)
     elif env_header is not None:
         env = _exec_to_create_env(env_header)
     else:
         raise ValueError("env_id or env_header must be provided.")
 
@@ -308,50 +284,68 @@
         out,
         video_callable=lambda ep: ep % 1 == 0,
         frame_rate=float(frame_rate),
         record_rate=int(record_rate),
     )
 
     # run episodes
-    evaluate_on_environment(wrapped_env, n_episodes, epsilon=epsilon)(algo)
+    if isinstance(algo, QLearningAlgoBase):
+        evaluate_qlearning_with_environment(
+            algo, wrapped_env, n_episodes, render=True
+        )
+    elif isinstance(algo, TransformerAlgoBase):
+        assert target_return is not None, "--target-return must be specified."
+        evaluate_transformer_with_environment(
+            StatefulTransformerWrapper(algo, float(target_return)),
+            wrapped_env,
+            n_episodes,
+            render=True,
+        )
+    else:
+        raise ValueError("invalid algo type.")
 
 
 @cli.command(short_help="Run evaluation episodes with rendering.")
 @click.argument("model_path")
 @click.option("--env-id", default=None, help="Gym environment id.")
 @click.option(
     "--env-header", default=None, help="one-liner to create environment."
 )
+@click.option("--n-episodes", default=3, help="the number of episodes to run.")
 @click.option(
-    "--params-json", default=None, help="explicityly specify params.json."
+    "--target-return",
+    default=None,
+    help="the target return for Decision Transformer variants.",
 )
-@click.option("--n-episodes", default=3, help="the number of episodes to run.")
 def play(
     model_path: str,
     env_id: Optional[str],
     env_header: Optional[str],
-    params_json: Optional[str],
     n_episodes: int,
+    target_return: Optional[float],
 ) -> None:
-    if params_json is None:
-        params_json = _get_params_json_path(model_path)
-
-    # load params
-    with open(params_json, "r") as f:
-        params = json.loads(f.read())
-
     # load saved model
     print(f"Loading {model_path}...")
-    algo = getattr(algos, params["algorithm"]).from_json(params_json)
-    algo.load_model(model_path)
+    algo = load_learnable(model_path)
 
     # wrap environment with Monitor
-    env: gym.Env
+    env: gym.Env[Any, Any]
     if env_id is not None:
         env = gym.make(env_id)
     elif env_header is not None:
         env = _exec_to_create_env(env_header)
     else:
         raise ValueError("env_id or env_header must be provided.")
 
     # run episodes
-    evaluate_on_environment(env, n_episodes, render=True)(algo)
+    if isinstance(algo, QLearningAlgoBase):
+        evaluate_qlearning_with_environment(algo, env, n_episodes, render=True)
+    elif isinstance(algo, TransformerAlgoBase):
+        assert target_return is not None, "--target-return must be specified."
+        evaluate_transformer_with_environment(
+            StatefulTransformerWrapper(algo, float(target_return)),
+            env,
+            n_episodes,
+            render=True,
+        )
+    else:
+        raise ValueError("invalid algo type.")
```

### Comparing `d3rlpy-1.1.1/d3rlpy/constants.py` & `d3rlpy-2.0.2/d3rlpy/constants.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from enum import Enum
 
 from ._version import __version__
 
+__all__ = [
+    "IMPL_NOT_INITIALIZED_ERROR",
+    "ALGO_NOT_GIVEN_ERROR",
+    "DISCRETE_ACTION_SPACE_MISMATCH_ERROR",
+    "CONTINUOUS_ACTION_SPACE_MISMATCH_ERROR",
+    "ActionSpace",
+]
+
 IMPL_NOT_INITIALIZED_ERROR = (
     "The neural network parameters are not "
     "initialized. Pleaes call build_with_dataset, "
     "build_with_env, or directly call fit or "
     "fit_online method."
 )
 
 ALGO_NOT_GIVEN_ERROR = (
     "The algorithm to evaluate is not given. Please give the trained algorithm"
     " to the argument."
 )
 
-DYNAMICS_NOT_GIVEN_ERROR = (
-    "The dynamics to generate transitions is not given. Please give the trained"
-    " dynamics to the argument."
-)
-
 DISCRETE_ACTION_SPACE_MISMATCH_ERROR = (
     "The action-space of the given dataset is not compatible with the"
     " algorithm. Please use discrete action-space algorithms. The algorithms"
     " list is available below.\n"
     f"https://d3rlpy.readthedocs.io/en/v{__version__}/references/algos.html"
 )
```

### Comparing `d3rlpy-1.1.1/d3rlpy/datasets.py` & `d3rlpy-2.0.2/d3rlpy/datasets.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,42 +1,74 @@
 # pylint: disable=unused-import,too-many-return-statements
 
 import os
 import random
 import re
-from typing import List, Tuple
+from typing import Any, Dict, Optional, Tuple
 from urllib import request
 
 import gym
 import numpy as np
+from gym.wrappers.time_limit import TimeLimit
 
-from .dataset import Episode, MDPDataset, Transition
-from .envs import ChannelFirst
+from .dataset import (
+    Episode,
+    EpisodeGenerator,
+    FrameStackTransitionPicker,
+    InfiniteBuffer,
+    MDPDataset,
+    ReplayBuffer,
+    TrajectorySlicerProtocol,
+    TransitionPickerProtocol,
+    create_infinite_replay_buffer,
+    load_v1,
+)
+from .envs import ChannelFirst, FrameStack
+
+__all__ = [
+    "DATA_DIRECTORY",
+    "DROPBOX_URL",
+    "CARTPOLE_URL",
+    "CARTPOLE_RANDOM_URL",
+    "PENDULUM_URL",
+    "PENDULUM_RANDOM_URL",
+    "get_cartpole",
+    "get_pendulum",
+    "get_atari",
+    "get_atari_transitions",
+    "get_d4rl",
+    "get_dataset",
+]
 
 DATA_DIRECTORY = "d3rlpy_data"
 DROPBOX_URL = "https://www.dropbox.com/s"
 CARTPOLE_URL = f"{DROPBOX_URL}/uep0lzlhxpi79pd/cartpole_v1.1.0.h5?dl=1"
 CARTPOLE_RANDOM_URL = f"{DROPBOX_URL}/4lgai7tgj84cbov/cartpole_random_v1.1.0.h5?dl=1"  # pylint: disable=line-too-long
 PENDULUM_URL = f"{DROPBOX_URL}/ukkucouzys0jkfs/pendulum_v1.1.0.h5?dl=1"
 PENDULUM_RANDOM_URL = f"{DROPBOX_URL}/hhbq9i6ako24kzz/pendulum_random_v1.1.0.h5?dl=1"  # pylint: disable=line-too-long
 
 
-def get_cartpole(dataset_type: str = "replay") -> Tuple[MDPDataset, gym.Env]:
+def get_cartpole(
+    dataset_type: str = "replay",
+    transition_picker: Optional[TransitionPickerProtocol] = None,
+    trajectory_slicer: Optional[TrajectorySlicerProtocol] = None,
+) -> Tuple[ReplayBuffer, gym.Env[np.ndarray, int]]:
     """Returns cartpole dataset and environment.
 
     The dataset is automatically downloaded to ``d3rlpy_data/cartpole.h5`` if
     it does not exist.
 
     Args:
         dataset_type: dataset type. Available options are
             ``['replay', 'random']``.
+        transition_picker: TransitionPickerProtocol object.
+        trajectory_slicer: TrajectorySlicerProtocol object.
 
     Returns:
-        tuple of :class:`d3rlpy.dataset.MDPDataset` and gym environment.
-
+        tuple of :class:`d3rlpy.dataset.ReplayBuffer` and gym environment.
     """
     if dataset_type == "replay":
         url = CARTPOLE_URL
         file_name = "cartpole_replay_v1.1.0.h5"
     elif dataset_type == "random":
         url = CARTPOLE_RANDOM_URL
         file_name = "cartpole_random_v1.1.0.h5"
@@ -48,35 +80,47 @@
     # download dataset
     if not os.path.exists(data_path):
         os.makedirs(DATA_DIRECTORY, exist_ok=True)
         print(f"Downloading cartpole.pkl into {data_path}...")
         request.urlretrieve(url, data_path)
 
     # load dataset
-    dataset = MDPDataset.load(data_path)
+    with open(data_path, "rb") as f:
+        episodes = load_v1(f)
+    dataset = ReplayBuffer(
+        InfiniteBuffer(),
+        episodes=episodes,
+        transition_picker=transition_picker,
+        trajectory_slicer=trajectory_slicer,
+    )
 
     # environment
-    env = gym.make("CartPole-v0")
+    env = gym.make("CartPole-v1")
 
     return dataset, env
 
 
-def get_pendulum(dataset_type: str = "replay") -> Tuple[MDPDataset, gym.Env]:
+def get_pendulum(
+    dataset_type: str = "replay",
+    transition_picker: Optional[TransitionPickerProtocol] = None,
+    trajectory_slicer: Optional[TrajectorySlicerProtocol] = None,
+) -> Tuple[ReplayBuffer, gym.Env[np.ndarray, np.ndarray]]:
     """Returns pendulum dataset and environment.
 
     The dataset is automatically downloaded to ``d3rlpy_data/pendulum.h5`` if
     it does not exist.
 
     Args:
         dataset_type: dataset type. Available options are
             ``['replay', 'random']``.
+        transition_picker: TransitionPickerProtocol object.
+        trajectory_slicer: TrajectorySlicerProtocol object.
 
     Returns:
-        tuple of :class:`d3rlpy.dataset.MDPDataset` and gym environment.
-
+        tuple of :class:`d3rlpy.dataset.ReplayBuffer` and gym environment.
     """
     if dataset_type == "replay":
         url = PENDULUM_URL
         file_name = "pendulum_replay_v1.1.0.h5"
     elif dataset_type == "random":
         url = PENDULUM_RANDOM_URL
         file_name = "pendulum_random_v1.1.0.h5"
@@ -87,23 +131,33 @@
 
     if not os.path.exists(data_path):
         os.makedirs(DATA_DIRECTORY, exist_ok=True)
         print(f"Donwloading pendulum.pkl into {data_path}...")
         request.urlretrieve(url, data_path)
 
     # load dataset
-    dataset = MDPDataset.load(data_path)
+    with open(data_path, "rb") as f:
+        episodes = load_v1(f)
+    dataset = ReplayBuffer(
+        InfiniteBuffer(),
+        episodes=episodes,
+        transition_picker=transition_picker,
+        trajectory_slicer=trajectory_slicer,
+    )
 
     # environment
-    env = gym.make("Pendulum-v0")
+    env = gym.make("Pendulum-v1")
 
     return dataset, env
 
 
-def get_atari(env_name: str) -> Tuple[MDPDataset, gym.Env]:
+def get_atari(
+    env_name: str,
+    num_stack: Optional[int] = None,
+) -> Tuple[ReplayBuffer, gym.Env[np.ndarray, int]]:
     """Returns atari dataset and envrironment.
 
     The dataset is provided through d4rl-atari. See more details including
     available dataset from its GitHub page.
 
     .. code-block:: python
 
@@ -112,35 +166,48 @@
         dataset, env = get_atari('breakout-mixed-v0')
 
     References:
         * https://github.com/takuseno/d4rl-atari
 
     Args:
         env_name: environment id of d4rl-atari dataset.
+        num_stack: the number of frames to stack (only applied to env).
 
     Returns:
-        tuple of :class:`d3rlpy.dataset.MDPDataset` and gym environment.
-
+        tuple of :class:`d3rlpy.dataset.ReplayBuffer` and gym environment.
     """
     try:
         import d4rl_atari  # type: ignore
 
-        env = ChannelFirst(gym.make(env_name))
-        dataset = MDPDataset(discrete_action=True, **env.get_dataset())
+        env = gym.make(env_name)
+        raw_dataset = env.get_dataset()  # type: ignore
+        episode_generator = EpisodeGenerator(**raw_dataset)
+        dataset = create_infinite_replay_buffer(
+            episodes=episode_generator(),
+            transition_picker=FrameStackTransitionPicker(num_stack or 1),
+            trajectory_slicer=None,
+        )
+        if num_stack:
+            env = FrameStack(env, num_stack=num_stack)
+        else:
+            env = ChannelFirst(env)
         return dataset, env
     except ImportError as e:
         raise ImportError(
             "d4rl-atari is not installed.\n"
             "pip install git+https://github.com/takuseno/d4rl-atari"
         ) from e
 
 
 def get_atari_transitions(
-    game_name: str, fraction: float = 0.01, index: int = 0
-) -> Tuple[List[Transition], gym.Env]:
+    game_name: str,
+    fraction: float = 0.01,
+    index: int = 0,
+    num_stack: Optional[int] = None,
+) -> Tuple[ReplayBuffer, gym.Env[np.ndarray, int]]:
     """Returns atari dataset as a list of Transition objects and envrironment.
 
     The dataset is provided through d4rl-atari.
     The difference from ``get_atari`` function is that this function will
     sample transitions from all epochs.
     This function is necessary for reproducing Atari experiments.
 
@@ -154,67 +221,86 @@
     References:
         * https://github.com/takuseno/d4rl-atari
 
     Args:
         game_name: Atari 2600 game name in lower_snake_case.
         fraction: fraction of sampled transitions.
         index: index to specify which trial to load.
+        num_stack: the number of frames to stack (only applied to env).
 
     Returns:
         tuple of a list of :class:`d3rlpy.dataset.Transition` and gym
         environment.
-
     """
     try:
         import d4rl_atari
 
         # each epoch consists of 1M steps
         num_transitions_per_epoch = int(1000000 * fraction)
 
-        transitions = []
+        copied_episodes = []
         for i in range(50):
             env = gym.make(
                 f"{game_name}-epoch-{i + 1}-v{index}", sticky_action=True
             )
-            dataset = MDPDataset(discrete_action=True, **env.get_dataset())
-            episodes = list(dataset.episodes)
+            raw_dataset = env.get_dataset()  # type: ignore
+            episode_generator = EpisodeGenerator(**raw_dataset)
+            episodes = list(episode_generator())
 
             # copy episode data to release memory of unused data
             random.shuffle(episodes)
             num_data = 0
-            copied_episodes = []
             for episode in episodes:
+                if num_data >= num_transitions_per_epoch:
+                    break
+
                 copied_episode = Episode(
-                    observation_shape=tuple(episode.get_observation_shape()),
-                    action_size=episode.get_action_size(),
-                    observations=episode.observations.copy(),
+                    observations=episode.observations.copy(),  # type: ignore
                     actions=episode.actions.copy(),
                     rewards=episode.rewards.copy(),
-                    terminal=episode.terminal,
+                    terminated=episode.terminated,
                 )
+
+                # trim episode
+                if num_data + copied_episode.size() > num_transitions_per_epoch:
+                    end = num_transitions_per_epoch - num_data
+                    copied_episode = Episode(
+                        observations=copied_episode.observations[:end],
+                        actions=copied_episode.actions[:end],
+                        rewards=copied_episode.rewards[:end],
+                        terminated=False,
+                    )
+
                 copied_episodes.append(copied_episode)
+                num_data += copied_episode.size()
 
-                num_data += len(copied_episode)
-                if num_data > num_transitions_per_epoch:
-                    break
+        dataset = ReplayBuffer(
+            InfiniteBuffer(),
+            episodes=copied_episodes,
+            transition_picker=FrameStackTransitionPicker(num_stack or 1),
+        )
 
-            transitions_per_epoch = []
-            for episode in copied_episodes:
-                transitions_per_epoch += episode.transitions
-            transitions += transitions_per_epoch[:num_transitions_per_epoch]
+        if num_stack:
+            env = FrameStack(env, num_stack=num_stack)
+        else:
+            env = ChannelFirst(env)
 
-        return transitions, ChannelFirst(env)
+        return dataset, env
     except ImportError as e:
         raise ImportError(
             "d4rl-atari is not installed.\n"
             "pip install git+https://github.com/takuseno/d4rl-atari"
         ) from e
 
 
-def get_d4rl(env_name: str) -> Tuple[MDPDataset, gym.Env]:
+def get_d4rl(
+    env_name: str,
+    transition_picker: Optional[TransitionPickerProtocol] = None,
+    trajectory_slicer: Optional[TrajectorySlicerProtocol] = None,
+) -> Tuple[ReplayBuffer, gym.Env[np.ndarray, np.ndarray]]:
     """Returns d4rl dataset and envrironment.
 
     The dataset is provided through d4rl.
 
     .. code-block:: python
 
         from d3rlpy.datasets import get_d4rl
@@ -224,41 +310,46 @@
     References:
         * `Fu et al., D4RL: Datasets for Deep Data-Driven Reinforcement
           Learning. <https://arxiv.org/abs/2004.07219>`_
         * https://github.com/rail-berkeley/d4rl
 
     Args:
         env_name: environment id of d4rl dataset.
+        transition_picker: TransitionPickerProtocol object.
+        trajectory_slicer: TrajectorySlicerProtocol object.
 
     Returns:
-        tuple of :class:`d3rlpy.dataset.MDPDataset` and gym environment.
-
+        tuple of :class:`d3rlpy.dataset.ReplayBuffer` and gym environment.
     """
     try:
         import d4rl  # type: ignore
 
         env = gym.make(env_name)
-        dataset = env.get_dataset()
+        raw_dataset: Dict[str, np.ndarray] = env.get_dataset()  # type: ignore
 
-        observations = dataset["observations"]
-        actions = dataset["actions"]
-        rewards = dataset["rewards"]
-        terminals = dataset["terminals"]
-        timeouts = dataset["timeouts"]
-        episode_terminals = np.logical_or(terminals, timeouts)
-
-        mdp_dataset = MDPDataset(
-            observations=np.array(observations, dtype=np.float32),
-            actions=np.array(actions, dtype=np.float32),
-            rewards=np.array(rewards, dtype=np.float32),
-            terminals=np.array(terminals, dtype=np.float32),
-            episode_terminals=np.array(episode_terminals, dtype=np.float32),
+        observations = raw_dataset["observations"]
+        actions = raw_dataset["actions"]
+        rewards = raw_dataset["rewards"]
+        terminals = raw_dataset["terminals"]
+        timeouts = raw_dataset["timeouts"]
+
+        dataset = MDPDataset(
+            observations=observations,
+            actions=actions,
+            rewards=rewards,
+            terminals=terminals,
+            timeouts=timeouts,
+            transition_picker=transition_picker,
+            trajectory_slicer=trajectory_slicer,
         )
 
-        return mdp_dataset, env
+        # wrapped by NormalizedBoxEnv that is incompatible with newer Gym
+        unwrapped_env: gym.Env[Any, Any] = env.env.env.env.wrapped_env  # type: ignore
+
+        return dataset, TimeLimit(unwrapped_env, max_episode_steps=1000)
     except ImportError as e:
         raise ImportError(
             "d4rl is not installed.\n"
             "pip install git+https://github.com/rail-berkeley/d4rl"
         ) from e
 
 
@@ -324,15 +415,19 @@
     "video-pinball",
     "wizard-of-wor",
     "yars-revenge",
     "zaxxon",
 ]
 
 
-def get_dataset(env_name: str) -> Tuple[MDPDataset, gym.Env]:
+def get_dataset(
+    env_name: str,
+    transition_picker: Optional[TransitionPickerProtocol] = None,
+    trajectory_slicer: Optional[TrajectorySlicerProtocol] = None,
+) -> Tuple[ReplayBuffer, gym.Env[Any, Any]]:
     """Returns dataset and envrironment by guessing from name.
 
     This function returns dataset by matching name with the following datasets.
 
     - cartpole-replay
     - cartpole-random
     - pendulum-replay
@@ -355,27 +450,50 @@
        dataset, env = d3rlpy.datasets.get_dataset('breakout-mixed-v0')
 
        # d4rl dataset
        dataset, env = d3rlpy.datasets.get_dataset('hopper-medium-v0')
 
     Args:
         env_name: environment id of the dataset.
+        transition_picker: TransitionPickerProtocol object.
+        trajectory_slicer: TrajectorySlicerProtocol object.
 
     Returns:
-        tuple of :class:`d3rlpy.dataset.MDPDataset` and gym environment.
-
+        tuple of :class:`d3rlpy.dataset.ReplayBuffer` and gym environment.
     """
     if env_name == "cartpole-replay":
-        return get_cartpole(dataset_type="replay")
+        return get_cartpole(
+            dataset_type="replay",
+            transition_picker=transition_picker,
+            trajectory_slicer=trajectory_slicer,
+        )
     elif env_name == "cartpole-random":
-        return get_cartpole(dataset_type="random")
+        return get_cartpole(
+            dataset_type="random",
+            transition_picker=transition_picker,
+            trajectory_slicer=trajectory_slicer,
+        )
     elif env_name == "pendulum-replay":
-        return get_pendulum(dataset_type="replay")
+        return get_pendulum(
+            dataset_type="replay",
+            transition_picker=transition_picker,
+            trajectory_slicer=trajectory_slicer,
+        )
     elif env_name == "pendulum-random":
-        return get_pendulum(dataset_type="random")
+        return get_pendulum(
+            dataset_type="random",
+            transition_picker=transition_picker,
+            trajectory_slicer=trajectory_slicer,
+        )
     elif re.match(r"^bullet-.+$", env_name):
-        return get_d4rl(env_name)
+        return get_d4rl(
+            env_name,
+            transition_picker=transition_picker,
+            trajectory_slicer=trajectory_slicer,
+        )
     elif re.match(r"hopper|halfcheetah|walker|ant", env_name):
-        return get_d4rl(env_name)
-    elif re.match(re.compile("|".join(ATARI_GAMES)), env_name):
-        return get_atari(env_name)
+        return get_d4rl(
+            env_name,
+            transition_picker=transition_picker,
+            trajectory_slicer=trajectory_slicer,
+        )
     raise ValueError(f"Unrecognized env_name: {env_name}.")
```

### Comparing `d3rlpy-1.1.1/d3rlpy/envs/wrappers.py` & `d3rlpy-2.0.2/d3rlpy/envs/wrappers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,54 @@
 import json
 import os
-from typing import Any, Callable, Dict, Optional, Tuple, Union
+from collections import deque
+from typing import Any, Callable, Deque, Dict, List, Optional, Tuple, TypeVar
 
 import gym
 import numpy as np
 
 try:
     import cv2  # this is used in AtariPreprocessing
 except ImportError:
     cv2 = None
 
 from gym.spaces import Box
-from gym.wrappers import TransformReward
+from gym.wrappers.transform_reward import TransformReward
 
+__all__ = [
+    "ChannelFirst",
+    "FrameStack",
+    "AtariPreprocessing",
+    "Atari",
+    "Monitor",
+]
 
-class ChannelFirst(gym.Wrapper):  # type: ignore
+_ObsType = TypeVar("_ObsType")
+_ActType = TypeVar("_ActType")
+
+
+class ChannelFirst(gym.Wrapper[_ObsType, _ActType]):
     """Channel-first wrapper for image observation environments.
 
     d3rlpy expects channel-first images since it's built with PyTorch.
     You can transform the observation shape with ``ChannelFirst`` wrapper.
 
     Args:
         env (gym.Env): gym environment.
-
     """
 
     observation_space: Box
 
-    def __init__(self, env: gym.Env):
+    def __init__(self, env: gym.Env[_ObsType, _ActType]):
         super().__init__(env)
         shape = self.observation_space.shape
         low = self.observation_space.low
         high = self.observation_space.high
         dtype = self.observation_space.dtype
+        assert dtype is not None
 
         if len(shape) == 3:
             self.observation_space = Box(
                 low=np.transpose(low, [2, 0, 1]),
                 high=np.transpose(high, [2, 0, 1]),
                 shape=(shape[2], shape[0], shape[1]),
                 dtype=dtype,
@@ -48,38 +60,91 @@
                 shape=(1, *shape),
                 dtype=dtype,
             )
         else:
             raise ValueError("image observation is only allowed.")
 
     def step(
-        self, action: Union[int, np.ndarray]
-    ) -> Tuple[np.ndarray, float, bool, Dict[str, Any]]:
-        observation, reward, terminal, info = self.env.step(action)
+        self, action: _ActType
+    ) -> Tuple[_ObsType, float, bool, bool, Dict[str, Any]]:
+        observation, reward, terminal, truncated, info = self.env.step(action)
         # make channel first observation
         if observation.ndim == 3:
             observation_T = np.transpose(observation, [2, 0, 1])
         else:
             observation_T = np.reshape(observation, (1, *observation.shape))
         assert observation_T.shape == self.observation_space.shape
-        return observation_T, reward, terminal, info
+        return observation_T, reward, terminal, truncated, info
 
-    def reset(self, **kwargs: Any) -> np.ndarray:
-        observation = self.env.reset(**kwargs)
+    def reset(self, **kwargs: Any) -> Tuple[_ObsType, Dict[str, Any]]:
+        observation, info = self.env.reset(**kwargs)
         # make channel first observation
         if observation.ndim == 3:
             observation_T = np.transpose(observation, [2, 0, 1])
         else:
             observation_T = np.reshape(observation, (1, *observation.shape))
         assert observation_T.shape == self.observation_space.shape
-        return observation_T
+        return observation_T, info
+
+
+class FrameStack(gym.Wrapper[np.ndarray, _ActType]):
+    """Observation wrapper that stacks the observations in a rolling manner.
+
+    This wrapper is implemented based on gym.wrappers.FrameStack. The
+    difference is that this wrapper returns stacked frames as numpy array.
+
+    Args:
+        env (gym.Env): gym environment.
+        num_stack (int): the number of frames to stack.
+    """
+
+    _num_stack: int
+    _frames: Deque[np.ndarray]
+
+    def __init__(self, env: gym.Env[np.ndarray, _ActType], num_stack: int):
+        super().__init__(env)
+        self._num_stack = num_stack
+        self._frames = deque(maxlen=num_stack)
+
+        low = np.repeat(
+            self.observation_space.low[np.newaxis, ...],  # type: ignore
+            num_stack,
+            axis=0,
+        )
+        high = np.repeat(
+            self.observation_space.high[np.newaxis, ...],  # type: ignore
+            num_stack,
+            axis=0,
+        )
+        self.observation_space = Box(
+            low=low,
+            high=high,
+            dtype=self.observation_space.dtype,  # type: ignore
+        )
+
+    def observation(self, observation: Any) -> np.ndarray:
+        return np.array(self._frames, dtype=self._frames[-1].dtype)
+
+    def step(
+        self, action: _ActType
+    ) -> Tuple[np.ndarray, float, bool, bool, Dict[str, Any]]:
+        observation, reward, terminated, truncated, info = self.env.step(action)
+        self._frames.append(observation)
+        return self.observation(None), reward, terminated, truncated, info
+
+    def reset(self, **kwargs: Any) -> Tuple[np.ndarray, Dict[str, Any]]:
+        obs, info = self.env.reset(**kwargs)
+        for _ in range(self._num_stack - 1):
+            self._frames.append(np.zeros_like(obs))
+        self._frames.append(obs)
+        return self.observation(None), info
 
 
 # https://github.com/openai/gym/blob/0.17.3/gym/wrappers/atari_preprocessing.py
-class AtariPreprocessing(gym.Wrapper):  # type: ignore
+class AtariPreprocessing(gym.Wrapper[np.ndarray, int]):
     r"""Atari 2600 preprocessings.
     This class follows the guidelines in
     Machado et al. (2018), "Revisiting the Arcade Learning Environment:
     Evaluation Protocols and Open Problems for General Agents".
     Specifically:
 
     * NoopReset: obtain initial state by taking random number of no-ops on
@@ -108,15 +173,15 @@
             is returned. It also limits memory optimization benefits of
             FrameStack Wrapper.
 
     """
 
     def __init__(
         self,
-        env: gym.Env,
+        env: gym.Env[np.ndarray, int],
         noop_max: int = 30,
         frame_skip: int = 4,
         screen_size: int = 84,
         terminal_on_life_loss: bool = False,
         grayscale_obs: bool = True,
         grayscale_newaxis: bool = False,
         scale_obs: bool = False,
@@ -132,36 +197,38 @@
         if frame_skip > 1:
             assert "NoFrameskip" in env.spec.id, (
                 "disable frame-skipping in"
                 " the original env. for more than one frame-skip as it will"
                 " be done by the wrapper"
             )
         self.noop_max = noop_max
-        assert env.unwrapped.get_action_meanings()[0] == "NOOP"
+        assert env.unwrapped.get_action_meanings()[0] == "NOOP"  # type: ignore
 
         self.frame_skip = frame_skip
         self.screen_size = screen_size
         self.terminal_on_life_loss = terminal_on_life_loss
         self.grayscale_obs = grayscale_obs
         self.grayscale_newaxis = grayscale_newaxis
         self.scale_obs = scale_obs
 
         # buffer of most recent two observations for max pooling
+        shape = env.observation_space.shape
+        assert shape is not None
         if grayscale_obs:
             self.obs_buffer = [
-                np.empty(env.observation_space.shape[:2], dtype=np.uint8),
-                np.empty(env.observation_space.shape[:2], dtype=np.uint8),
+                np.empty(shape[:2], dtype=np.uint8),
+                np.empty(shape[:2], dtype=np.uint8),
             ]
         else:
             self.obs_buffer = [
-                np.empty(env.observation_space.shape, dtype=np.uint8),
-                np.empty(env.observation_space.shape, dtype=np.uint8),
+                np.empty(shape, dtype=np.uint8),
+                np.empty(shape, dtype=np.uint8),
             ]
 
-        self.ale = env.unwrapped.ale
+        self.ale = env.unwrapped.ale  # type: ignore
         self.lives = 0
         self.game_over = True
 
         _low, _high, _obs_dtype = (
             (0, 255, np.uint8) if not scale_obs else (0, 1, np.float32)
         )
         _shape = (screen_size, screen_size, 1 if grayscale_obs else 3)
@@ -169,67 +236,67 @@
             _shape = _shape[:-1]  # type: ignore
         self.observation_space = Box(
             low=_low, high=_high, shape=_shape, dtype=_obs_dtype
         )
 
     def step(
         self, action: int
-    ) -> Tuple[np.ndarray, float, float, Dict[str, Any]]:
+    ) -> Tuple[np.ndarray, float, bool, bool, Dict[str, Any]]:
         R = 0.0
 
         for t in range(self.frame_skip):
-            _, reward, done, info = self.env.step(action)
+            _, reward, done, truncated, info = self.env.step(action)
             R += reward
             self.game_over = done
 
             if self.terminal_on_life_loss:
                 new_lives = self.ale.lives()
                 done = done or new_lives < self.lives
                 self.lives = new_lives
 
-            if done:
+            if done or truncated:
                 break
             if t == self.frame_skip - 2:
                 if self.grayscale_obs:
                     self.ale.getScreenGrayscale(self.obs_buffer[1])
                 else:
                     self.ale.getScreenRGB2(self.obs_buffer[1])
             elif t == self.frame_skip - 1:
                 if self.grayscale_obs:
                     self.ale.getScreenGrayscale(self.obs_buffer[0])
                 else:
                     self.ale.getScreenRGB2(self.obs_buffer[0])
 
-        return self._get_obs(), R, done, info
+        return self._get_obs(), R, done, truncated, info
 
-    def reset(self, **kwargs: Any) -> np.ndarray:
+    def reset(self, **kwargs: Any) -> Tuple[np.ndarray, Dict[str, Any]]:
         # this condition is not included in the original code
         if self.game_over:
-            self.env.reset(**kwargs)
+            _, info = self.env.reset(**kwargs)
         else:
             # NoopReset
-            self.env.step(0)
+            _, _, _, _, info = self.env.step(0)
 
         noops = (
-            self.env.unwrapped.np_random.randint(1, self.noop_max + 1)
+            self.env.unwrapped.np_random.integers(1, self.noop_max + 1)
             if self.noop_max > 0
             else 0
         )
         for _ in range(noops):
-            _, _, done, _ = self.env.step(0)
-            if done:
-                self.env.reset(**kwargs)
+            _, _, done, truncated, info = self.env.step(0)
+            if done or truncated:
+                _, info = self.env.reset(**kwargs)
 
         self.lives = self.ale.lives()
         if self.grayscale_obs:
             self.ale.getScreenGrayscale(self.obs_buffer[0])
         else:
             self.ale.getScreenRGB2(self.obs_buffer[0])
         self.obs_buffer[1].fill(0)
-        return self._get_obs()
+        return self._get_obs(), info
 
     def _get_obs(self) -> np.ndarray:
         if self.frame_skip > 1:  # more efficient in-place pooling
             np.maximum(
                 self.obs_buffer[0], self.obs_buffer[1], out=self.obs_buffer[0]
             )
         obs = cv2.resize(
@@ -244,100 +311,108 @@
             obs = np.asarray(obs, dtype=np.uint8)
 
         if self.grayscale_obs and self.grayscale_newaxis:
             obs = np.expand_dims(obs, axis=-1)  # Add a channel axis
         return obs
 
 
-class Atari(gym.Wrapper):  # type: ignore
+class Atari(gym.Wrapper[np.ndarray, int]):
     """Atari 2600 wrapper for experiments.
 
     Args:
         env (gym.Env): gym environment.
+        num_stack (int): the number of frames to stack.
         is_eval (bool): flag to enter evaluation mode.
-
     """
 
-    def __init__(self, env: gym.Env, is_eval: bool = False):
+    def __init__(
+        self,
+        env: gym.Env[np.ndarray, int],
+        num_stack: Optional[int] = None,
+        is_eval: bool = False,
+    ):
         env = AtariPreprocessing(env, terminal_on_life_loss=not is_eval)
         if not is_eval:
-            env = TransformReward(env, lambda r: np.clip(r, -1.0, 1.0))
-        super().__init__(ChannelFirst(env))
+            env = TransformReward(env, lambda r: float(np.clip(r, -1.0, 1.0)))
+        if num_stack:
+            env = FrameStack(env, num_stack)
+        else:
+            env = ChannelFirst(env)
+        super().__init__(env)
 
 
-class Monitor(gym.Wrapper):  # type: ignore
+class Monitor(gym.Wrapper[_ObsType, _ActType]):
     """gym.wrappers.Monitor-style Monitor wrapper.
 
     Args:
         env (gym.Env): gym environment.
         directory (str): directory to save.
         video_callable (callable): callable function that takes episode counter
             to control record frequency.
         force (bool): flag to allow existing directory.
         frame_rate (float): video frame rate.
         record_rate (int): images are record every ``record_rate`` frames.
-
     """
 
     _directory: str
     _video_callable: Callable[[int], bool]
     _frame_rate: float
     _record_rate: int
     _episode: int
     _episode_return: float
     _episode_step: int
-    _buffer: np.ndarray
+    _buffer: List[np.ndarray]
 
     def __init__(
         self,
-        env: gym.Env,
+        env: gym.Env[_ObsType, _ActType],
         directory: str,
         video_callable: Optional[Callable[[int], bool]] = None,
         force: bool = False,
         frame_rate: float = 30.0,
         record_rate: int = 1,
     ):
         super().__init__(env)
         # prepare directory
         if os.path.exists(directory) and not force:
             raise ValueError(f"{directory} already exists.")
         os.makedirs(directory, exist_ok=True)
         self._directory = directory
 
         if video_callable:
-            self._video_callable = video_callable  # type: ignore
+            self._video_callable = video_callable
         else:
-            self._video_callable = lambda ep: ep % 10 == 0  # type: ignore
+            self._video_callable = lambda ep: ep % 10 == 0
 
         self._frame_rate = frame_rate
         self._record_rate = record_rate
 
         self._episode = 0
         self._episode_return = 0.0
         self._episode_step = 0
         self._buffer = []
 
     def step(
-        self, action: Union[np.ndarray, int]
-    ) -> Tuple[np.ndarray, float, bool, Dict[str, Any]]:
-        obs, reward, done, info = super().step(action)
+        self, action: _ActType
+    ) -> Tuple[_ObsType, float, bool, bool, Dict[str, Any]]:
+        obs, reward, done, truncated, info = super().step(action)
 
-        if self._video_callable(self._episode):  # type: ignore
+        if self._video_callable(self._episode):
             # store rendering
             frame = cv2.cvtColor(super().render("rgb_array"), cv2.COLOR_BGR2RGB)
             self._buffer.append(frame)
             self._episode_step += 1
             self._episode_return += reward
             if done:
                 self._save_video()
                 self._save_stats()
 
-        return obs, reward, done, info
+        return obs, reward, done, truncated, info
 
-    def reset(self, **kwargs: Any) -> np.ndarray:
+    def reset(self, **kwargs: Any) -> Tuple[_ObsType, Dict[str, Any]]:
         self._episode += 1
         self._episode_return = 0.0
         self._episode_step = 0
         self._buffer = []
         return super().reset(**kwargs)
 
     def _save_video(self) -> None:
```

### Comparing `d3rlpy-1.1.1/d3rlpy/metrics/scorer.py` & `d3rlpy-2.0.2/d3rlpy/metrics/evaluators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,125 +1,131 @@
-from typing import Any, Callable, Iterator, List, Optional, Tuple, Union, cast
+from typing import Any, Iterator, Optional, Sequence, cast
 
 import gym
 import numpy as np
 from typing_extensions import Protocol
 
-from ..dataset import Episode, TransitionMiniBatch
-from ..preprocessing.reward_scalers import RewardScaler
-from ..preprocessing.stack import StackedObservation
+from ..dataset import (
+    EpisodeBase,
+    ReplayBuffer,
+    TransitionMiniBatch,
+    TransitionPickerProtocol,
+)
+from ..interface import QLearningAlgoProtocol
+from .utility import evaluate_qlearning_with_environment
+
+__all__ = [
+    "EvaluatorProtocol",
+    "make_batches",
+    "TDErrorEvaluator",
+    "DiscountedSumOfAdvantageEvaluator",
+    "AverageValueEstimationEvaluator",
+    "InitialStateValueEstimationEvaluator",
+    "SoftOPCEvaluator",
+    "ContinuousActionDiffEvaluator",
+    "DiscreteActionMatchEvaluator",
+    "CompareContinuousActionDiffEvaluator",
+    "CompareDiscreteActionMatchEvaluator",
+    "EnvironmentEvaluator",
+]
 
-WINDOW_SIZE = 1024
-
-
-class AlgoProtocol(Protocol):
-    def predict(self, x: Union[np.ndarray, List[Any]]) -> np.ndarray:
-        ...
-
-    def predict_value(
-        self,
-        x: Union[np.ndarray, List[Any]],
-        action: Union[np.ndarray, List[Any]],
-        with_std: bool = False,
-    ) -> Union[np.ndarray, Tuple[np.ndarray, np.ndarray]]:
-        ...
-
-    @property
-    def n_frames(self) -> int:
-        ...
 
-    @property
-    def gamma(self) -> float:
-        ...
-
-    @property
-    def reward_scaler(self) -> Optional[RewardScaler]:
-        ...
+WINDOW_SIZE = 1024
 
 
-class DynamicsProtocol(Protocol):
-    def predict(
+class EvaluatorProtocol(Protocol):
+    def __call__(
         self,
-        x: Union[np.ndarray, List[Any]],
-        action: Union[np.ndarray, List[Any]],
-        with_variance: bool = False,
-    ) -> Union[
-        Tuple[np.ndarray, np.ndarray], Tuple[np.ndarray, np.ndarray, np.ndarray]
-    ]:
-        ...
-
-    @property
-    def n_frames(self) -> int:
-        ...
-
-    @property
-    def reward_scaler(self) -> Optional[RewardScaler]:
-        ...
-
-
-def _make_batches(
-    episode: Episode, window_size: int, n_frames: int
+        algo: QLearningAlgoProtocol,
+        dataset: ReplayBuffer,
+    ) -> float:
+        """Computes metrics.
+
+        Args:
+            algo: Q-learning algorithm.
+            dataset: ReplayBuffer.
+
+        Returns:
+            Computed metrics.
+        """
+        raise NotImplementedError
+
+
+def make_batches(
+    episode: EpisodeBase,
+    window_size: int,
+    transition_picker: TransitionPickerProtocol,
 ) -> Iterator[TransitionMiniBatch]:
     n_batches = len(episode) // window_size
     if len(episode) % window_size != 0:
         n_batches += 1
     for i in range(n_batches):
         head_index = i * window_size
-        last_index = min(head_index + window_size, len(episode))
-        transitions = episode.transitions[head_index:last_index]
-        batch = TransitionMiniBatch(transitions, n_frames)
+        last_index = min(head_index + window_size, episode.transition_count)
+        transitions = [
+            transition_picker(episode, index)
+            for index in range(head_index, last_index)
+        ]
+        batch = TransitionMiniBatch.from_transitions(transitions)
         yield batch
 
 
-def td_error_scorer(algo: AlgoProtocol, episodes: List[Episode]) -> float:
+class TDErrorEvaluator(EvaluatorProtocol):
     r"""Returns average TD error.
 
     This metics suggests how Q functions overfit to training sets.
     If the TD error is large, the Q functions are overfitting.
 
     .. math::
 
         \mathbb{E}_{s_t, a_t, r_{t+1}, s_{t+1} \sim D}
             [(Q_\theta (s_t, a_t)
              - r_{t+1} - \gamma \max_a Q_\theta (s_{t+1}, a))^2]
 
     Args:
-        algo: algorithm.
-        episodes: list of episodes.
+        episodes: Optional evaluation episodes. If it's not given, dataset
+            used in training will be used.
+    """
+    _episodes: Optional[Sequence[EpisodeBase]]
 
-    Returns:
-        average TD error.
+    def __init__(self, episodes: Optional[Sequence[EpisodeBase]] = None):
+        self._episodes = episodes
 
-    """
-    total_errors = []
-    for episode in episodes:
-        for batch in _make_batches(episode, WINDOW_SIZE, algo.n_frames):
-            # estimate values for current observations
-            values = algo.predict_value(batch.observations, batch.actions)
-
-            # estimate values for next observations
-            next_actions = algo.predict(batch.next_observations)
-            next_values = algo.predict_value(
-                batch.next_observations, next_actions
-            )
-
-            # calculate td errors
-            mask = (1.0 - np.asarray(batch.terminals)).reshape(-1)
-            rewards = np.asarray(batch.rewards).reshape(-1)
-            if algo.reward_scaler:
-                rewards = algo.reward_scaler.transform_numpy(rewards)
-            y = rewards + algo.gamma * cast(np.ndarray, next_values) * mask
-            total_errors += ((values - y) ** 2).tolist()
-
-    return float(np.mean(total_errors))
-
-
-def discounted_sum_of_advantage_scorer(
-    algo: AlgoProtocol, episodes: List[Episode]
-) -> float:
+    def __call__(
+        self,
+        algo: QLearningAlgoProtocol,
+        dataset: ReplayBuffer,
+    ) -> float:
+        total_errors = []
+        episodes = self._episodes if self._episodes else dataset.episodes
+        for episode in episodes:
+            for batch in make_batches(
+                episode, WINDOW_SIZE, dataset.transition_picker
+            ):
+                # estimate values for current observations
+                values = algo.predict_value(batch.observations, batch.actions)
+
+                # estimate values for next observations
+                next_actions = algo.predict(batch.next_observations)
+                next_values = algo.predict_value(
+                    batch.next_observations, next_actions
+                )
+
+                # calculate td errors
+                mask = (1.0 - np.asarray(batch.terminals)).reshape(-1)
+                rewards = np.asarray(batch.rewards).reshape(-1)
+                if algo.reward_scaler:
+                    rewards = algo.reward_scaler.transform_numpy(rewards)
+                y = rewards + algo.gamma * cast(np.ndarray, next_values) * mask
+                total_errors += ((values - y) ** 2).tolist()
+
+        return float(np.mean(total_errors))
+
+
+class DiscountedSumOfAdvantageEvaluator(EvaluatorProtocol):
     r"""Returns average of discounted sum of advantage.
 
     This metrics suggests how the greedy-policy selects different actions in
     action-value space.
     If the sum of advantage is small, the policy selects actions with larger
     estimated action-values.
 
@@ -132,120 +138,98 @@
     - \mathbb{E}_{a \sim \pi} [Q_\theta (s_t, a)]`.
 
     References:
         * `Murphy., A generalization error for Q-Learning.
           <http://www.jmlr.org/papers/volume6/murphy05a/murphy05a.pdf>`_
 
     Args:
-        algo: algorithm.
-        episodes: list of episodes.
+        episodes: Optional evaluation episodes. If it's not given, dataset
+            used in training will be used.
+    """
+    _episodes: Optional[Sequence[EpisodeBase]]
 
-    Returns:
-        average of discounted sum of advantage.
+    def __init__(self, episodes: Optional[Sequence[EpisodeBase]] = None):
+        self._episodes = episodes
 
-    """
-    total_sums = []
-    for episode in episodes:
-        for batch in _make_batches(episode, WINDOW_SIZE, algo.n_frames):
-            # estimate values for dataset actions
-            dataset_values = algo.predict_value(
-                batch.observations, batch.actions
-            )
-            dataset_values = cast(np.ndarray, dataset_values)
-
-            # estimate values for the current policy
-            actions = algo.predict(batch.observations)
-            on_policy_values = algo.predict_value(batch.observations, actions)
-
-            # calculate advantages
-            advantages = (dataset_values - on_policy_values).tolist()
-
-            # calculate discounted sum of advantages
-            A = advantages[-1]
-            sum_advantages = [A]
-            for advantage in reversed(advantages[:-1]):
-                A = advantage + algo.gamma * A
-                sum_advantages.append(A)
-
-            total_sums += sum_advantages
-
-    # smaller is better
-    return float(np.mean(total_sums))
-
-
-def average_value_estimation_scorer(
-    algo: AlgoProtocol, episodes: List[Episode]
-) -> float:
+    def __call__(
+        self,
+        algo: QLearningAlgoProtocol,
+        dataset: ReplayBuffer,
+    ) -> float:
+        total_sums = []
+        episodes = self._episodes if self._episodes else dataset.episodes
+        for episode in episodes:
+            for batch in make_batches(
+                episode, WINDOW_SIZE, dataset.transition_picker
+            ):
+                # estimate values for dataset actions
+                dataset_values = algo.predict_value(
+                    batch.observations, batch.actions
+                )
+                dataset_values = cast(np.ndarray, dataset_values)
+
+                # estimate values for the current policy
+                actions = algo.predict(batch.observations)
+                on_policy_values = algo.predict_value(
+                    batch.observations, actions
+                )
+
+                # calculate advantages
+                advantages = (dataset_values - on_policy_values).tolist()
+
+                # calculate discounted sum of advantages
+                A = advantages[-1]
+                sum_advantages = [A]
+                for advantage in reversed(advantages[:-1]):
+                    A = advantage + algo.gamma * A
+                    sum_advantages.append(A)
+
+                total_sums += sum_advantages
+        # smaller is better
+        return float(np.mean(total_sums))
+
+
+class AverageValueEstimationEvaluator(EvaluatorProtocol):
     r"""Returns average value estimation.
 
     This metrics suggests the scale for estimation of Q functions.
     If average value estimation is too large, the Q functions overestimate
     action-values, which possibly makes training failed.
 
     .. math::
 
         \mathbb{E}_{s_t \sim D} [ \max_a Q_\theta (s_t, a)]
 
     Args:
-        algo: algorithm.
-        episodes: list of episodes.
-
-    Returns:
-        average value estimation.
-
+        episodes: Optional evaluation episodes. If it's not given, dataset
+            used in training will be used.
     """
-    total_values = []
-    for episode in episodes:
-        for batch in _make_batches(episode, WINDOW_SIZE, algo.n_frames):
-            actions = algo.predict(batch.observations)
-            values = algo.predict_value(batch.observations, actions)
-            total_values += cast(np.ndarray, values).tolist()
-    return float(np.mean(total_values))
-
-
-def value_estimation_std_scorer(
-    algo: AlgoProtocol, episodes: List[Episode]
-) -> float:
-    r"""Returns standard deviation of value estimation.
-
-    This metrics suggests how confident Q functions are for the given
-    episodes.
-    This metrics will be more accurate with `boostrap` enabled and the larger
-    `n_critics` at algorithm.
-    If standard deviation of value estimation is large, the Q functions are
-    overfitting to the training set.
-
-    .. math::
-
-        \mathbb{E}_{s_t \sim D, a \sim \text{argmax}_a Q_\theta(s_t, a)}
-            [Q_{\text{std}}(s_t, a)]
-
-    where :math:`Q_{\text{std}}(s, a)` is a standard deviation of action-value
-    estimation over ensemble functions.
-
-    Args:
-        algo: algorithm.
-        episodes: list of episodes.
+    _episodes: Optional[Sequence[EpisodeBase]]
 
-    Returns:
-        standard deviation.
+    def __init__(self, episodes: Optional[Sequence[EpisodeBase]] = None):
+        self._episodes = episodes
 
-    """
-    total_stds = []
-    for episode in episodes:
-        for batch in _make_batches(episode, WINDOW_SIZE, algo.n_frames):
-            actions = algo.predict(batch.observations)
-            _, stds = algo.predict_value(batch.observations, actions, True)
-            total_stds += stds.tolist()
-    return float(np.mean(total_stds))
+    def __call__(
+        self,
+        algo: QLearningAlgoProtocol,
+        dataset: ReplayBuffer,
+    ) -> float:
+        total_values = []
+        episodes = self._episodes if self._episodes else dataset.episodes
+        for episode in episodes:
+            for batch in make_batches(
+                episode, WINDOW_SIZE, dataset.transition_picker
+            ):
+                actions = algo.predict(batch.observations)
+                values = algo.predict_value(batch.observations, actions)
+                total_values += cast(np.ndarray, values).tolist()
+        return float(np.mean(total_values))
 
 
-def initial_state_value_estimation_scorer(
-    algo: AlgoProtocol, episodes: List[Episode]
-) -> float:
+class InitialStateValueEstimationEvaluator(EvaluatorProtocol):
     r"""Returns mean estimated action-values at the initial states.
 
     This metrics suggests how much return the trained policy would get from
     the initial states by deploying the policy to the states.
     If the estimated value is large, the trained policy is expected to get
     higher returns.
 
@@ -254,325 +238,309 @@
         \mathbb{E}_{s_0 \sim D} [Q(s_0, \pi(s_0))]
 
     References:
         * `Paine et al., Hyperparameter Selection for Offline Reinforcement
           Learning <https://arxiv.org/abs/2007.09055>`_
 
     Args:
-        algo: algorithm.
-        episodes: list of episodes.
+        episodes: Optional evaluation episodes. If it's not given, dataset
+            used in training will be used.
+    """
 
-    Returns:
-        mean action-value estimation at the initial states.
+    _episodes: Optional[Sequence[EpisodeBase]]
 
-    """
-    total_values = []
-    for episode in episodes:
-        for batch in _make_batches(episode, WINDOW_SIZE, algo.n_frames):
-            # estimate action-value in initial states
-            actions = algo.predict([batch.observations[0]])
-            values = algo.predict_value([batch.observations[0]], actions)
-            total_values.append(values[0])
-    return float(np.mean(total_values))
+    def __init__(self, episodes: Optional[Sequence[EpisodeBase]] = None):
+        self._episodes = episodes
+
+    def __call__(
+        self,
+        algo: QLearningAlgoProtocol,
+        dataset: ReplayBuffer,
+    ) -> float:
+        total_values = []
+        episodes = self._episodes if self._episodes else dataset.episodes
+        for episode in episodes:
+            for batch in make_batches(
+                episode, WINDOW_SIZE, dataset.transition_picker
+            ):
+                # estimate action-value in initial states
+                actions = algo.predict([batch.observations[0]])
+                values = algo.predict_value([batch.observations[0]], actions)
+                total_values.append(values[0])
+        return float(np.mean(total_values))
 
 
-def soft_opc_scorer(
-    return_threshold: float,
-) -> Callable[[AlgoProtocol, List[Episode]], float]:
+class SoftOPCEvaluator(EvaluatorProtocol):
     r"""Returns Soft Off-Policy Classification metrics.
 
-    This function returns scorer function, which is suitable to the standard
-    scikit-learn scorer function style.
     The metrics of the scorer funciton is evaluating gaps of action-value
     estimation between the success episodes and the all episodes.
     If the learned Q-function is optimal, action-values in success episodes
     are expected to be higher than the others.
     The success episode is defined as an episode with a return above the given
     threshold.
 
     .. math::
 
         \mathbb{E}_{s, a \sim D_{success}} [Q(s, a)]
             - \mathbb{E}_{s, a \sim D} [Q(s, a)]
 
-    .. code-block:: python
-
-        from d3rlpy.datasets import get_cartpole
-        from d3rlpy.algos import DQN
-        from d3rlpy.metrics.scorer import soft_opc_scorer
-        from sklearn.model_selection import train_test_split
-
-        dataset, _ = get_cartpole()
-        train_episodes, test_episodes = train_test_split(dataset, test_size=0.2)
-
-        scorer = soft_opc_scorer(return_threshold=180)
-
-        dqn = DQN()
-        dqn.fit(train_episodes,
-                eval_episodes=test_episodes,
-                scorers={'soft_opc': scorer})
-
     References:
         * `Irpan et al., Off-Policy Evaluation via Off-Policy Classification.
           <https://arxiv.org/abs/1906.01624>`_
 
     Args:
-        return_threshold: threshold of success episodes.
-
-    Returns:
-        scorer function.
-
+        return_threshold: Return threshold of success episodes.
+        episodes: Optional evaluation episodes. If it's not given, dataset
+            used in training will be used.
     """
+    _return_threshold: float
+    _episodes: Optional[Sequence[EpisodeBase]]
+
+    def __init__(
+        self,
+        return_threshold: float,
+        episodes: Optional[Sequence[EpisodeBase]] = None,
+    ):
+        self._return_threshold = return_threshold
+        self._episodes = episodes
 
-    def scorer(algo: AlgoProtocol, episodes: List[Episode]) -> float:
+    def __call__(
+        self,
+        algo: QLearningAlgoProtocol,
+        dataset: ReplayBuffer,
+    ) -> float:
         success_values = []
         all_values = []
+        episodes = self._episodes if self._episodes else dataset.episodes
         for episode in episodes:
-            is_success = episode.compute_return() >= return_threshold
-            for batch in _make_batches(episode, WINDOW_SIZE, algo.n_frames):
+            is_success = episode.compute_return() >= self._return_threshold
+            for batch in make_batches(
+                episode, WINDOW_SIZE, dataset.transition_picker
+            ):
                 values = algo.predict_value(batch.observations, batch.actions)
                 values = cast(np.ndarray, values)
                 all_values += values.reshape(-1).tolist()
                 if is_success:
                     success_values += values.reshape(-1).tolist()
         return float(np.mean(success_values) - np.mean(all_values))
 
-    return scorer
-
 
-def continuous_action_diff_scorer(
-    algo: AlgoProtocol, episodes: List[Episode]
-) -> float:
+class ContinuousActionDiffEvaluator(EvaluatorProtocol):
     r"""Returns squared difference of actions between algorithm and dataset.
 
     This metrics suggests how different the greedy-policy is from the given
     episodes in continuous action-space.
     If the given episodes are near-optimal, the small action difference would
     be better.
 
     .. math::
 
         \mathbb{E}_{s_t, a_t \sim D} [(a_t - \pi_\phi (s_t))^2]
 
     Args:
-        algo: algorithm.
-        episodes: list of episodes.
+        episodes: Optional evaluation episodes. If it's not given, dataset
+            used in training will be used.
+    """
+    _episodes: Optional[Sequence[EpisodeBase]]
 
-    Returns:
-        squared action difference.
+    def __init__(self, episodes: Optional[Sequence[EpisodeBase]] = None):
+        self._episodes = episodes
 
-    """
-    total_diffs = []
-    for episode in episodes:
-        for batch in _make_batches(episode, WINDOW_SIZE, algo.n_frames):
-            actions = algo.predict(batch.observations)
-            diff = ((batch.actions - actions) ** 2).sum(axis=1).tolist()
-            total_diffs += diff
-    return float(np.mean(total_diffs))
+    def __call__(
+        self,
+        algo: QLearningAlgoProtocol,
+        dataset: ReplayBuffer,
+    ) -> float:
+        total_diffs = []
+        episodes = self._episodes if self._episodes else dataset.episodes
+        for episode in episodes:
+            for batch in make_batches(
+                episode, WINDOW_SIZE, dataset.transition_picker
+            ):
+                actions = algo.predict(batch.observations)
+                diff = ((batch.actions - actions) ** 2).sum(axis=1).tolist()
+                total_diffs += diff
+        return float(np.mean(total_diffs))
 
 
-def discrete_action_match_scorer(
-    algo: AlgoProtocol, episodes: List[Episode]
-) -> float:
+class DiscreteActionMatchEvaluator(EvaluatorProtocol):
     r"""Returns percentage of identical actions between algorithm and dataset.
 
     This metrics suggests how different the greedy-policy is from the given
     episodes in discrete action-space.
     If the given episdoes are near-optimal, the large percentage would be
     better.
 
     .. math::
 
         \frac{1}{N} \sum^N \parallel
             \{a_t = \text{argmax}_a Q_\theta (s_t, a)\}
 
     Args:
-        algo: algorithm.
-        episodes: list of episodes.
-
-    Returns:
-        percentage of identical actions.
-
+        episodes: Optional evaluation episodes. If it's not given, dataset
+            used in training will be used.
     """
-    total_matches = []
-    for episode in episodes:
-        for batch in _make_batches(episode, WINDOW_SIZE, algo.n_frames):
-            actions = algo.predict(batch.observations)
-            match = (batch.actions.reshape(-1) == actions).tolist()
-            total_matches += match
-    return float(np.mean(total_matches))
-
+    _episodes: Optional[Sequence[EpisodeBase]]
 
-def evaluate_on_environment(
-    env: gym.Env, n_trials: int = 10, epsilon: float = 0.0, render: bool = False
-) -> Callable[..., float]:
-    """Returns scorer function of evaluation on environment.
+    def __init__(self, episodes: Optional[Sequence[EpisodeBase]] = None):
+        self._episodes = episodes
 
-    This function returns scorer function, which is suitable to the standard
-    scikit-learn scorer function style.
-    The metrics of the scorer function is ideal metrics to evaluate the
-    resulted policies.
-
-    .. code-block:: python
-
-        import gym
-
-        from d3rlpy.algos import DQN
-        from d3rlpy.metrics.scorer import evaluate_on_environment
-
-
-        env = gym.make('CartPole-v0')
-
-        scorer = evaluate_on_environment(env)
-
-        cql = CQL()
+    def __call__(
+        self,
+        algo: QLearningAlgoProtocol,
+        dataset: ReplayBuffer,
+    ) -> float:
+        total_matches = []
+        episodes = self._episodes if self._episodes else dataset.episodes
+        for episode in episodes:
+            for batch in make_batches(
+                episode, WINDOW_SIZE, dataset.transition_picker
+            ):
+                actions = algo.predict(batch.observations)
+                match = (batch.actions.reshape(-1) == actions).tolist()
+                total_matches += match
+        return float(np.mean(total_matches))
+
+
+class CompareContinuousActionDiffEvaluator(EvaluatorProtocol):
+    r"""Action difference between algorithms.
+
+    This metrics suggests how different the two algorithms are in continuous
+    action-space.
+    If the algorithm to compare with is near-optimal, the small action
+    difference would be better.
 
-        mean_episode_return = scorer(cql)
+    .. math::
 
+        \mathbb{E}_{s_t \sim D}
+            [(\pi_{\phi_1}(s_t) - \pi_{\phi_2}(s_t))^2]
 
     Args:
-        env: gym-styled environment.
-        n_trials: the number of trials.
-        epsilon: noise factor for epsilon-greedy policy.
-        render: flag to render environment.
-
-    Returns:
-        scoerer function.
-
-
+        base_algo: Target algorithm to comapre with.
+        episodes: Optional evaluation episodes. If it's not given, dataset
+            used in training will be used.
     """
+    _base_algo: QLearningAlgoProtocol
+    _episodes: Optional[Sequence[EpisodeBase]]
 
-    # for image observation
-    observation_shape = env.observation_space.shape
-    is_image = len(observation_shape) == 3
-
-    def scorer(algo: AlgoProtocol, *args: Any) -> float:
-        if is_image:
-            stacked_observation = StackedObservation(
-                observation_shape, algo.n_frames
-            )
-
-        episode_rewards = []
-        for _ in range(n_trials):
-            observation = env.reset()
-            episode_reward = 0.0
-
-            # frame stacking
-            if is_image:
-                stacked_observation.clear()
-                stacked_observation.append(observation)
-
-            while True:
-                # take action
-                if np.random.random() < epsilon:
-                    action = env.action_space.sample()
-                else:
-                    if is_image:
-                        action = algo.predict([stacked_observation.eval()])[0]
-                    else:
-                        action = algo.predict([observation])[0]
-
-                observation, reward, done, _ = env.step(action)
-                episode_reward += reward
-
-                if is_image:
-                    stacked_observation.append(observation)
-
-                if render:
-                    env.render()
-
-                if done:
-                    break
-            episode_rewards.append(episode_reward)
-        return float(np.mean(episode_rewards))
-
-    return scorer
-
-
-def dynamics_observation_prediction_error_scorer(
-    dynamics: DynamicsProtocol, episodes: List[Episode]
-) -> float:
-    r"""Returns MSE of observation prediction.
+    def __init__(
+        self,
+        base_algo: QLearningAlgoProtocol,
+        episodes: Optional[Sequence[EpisodeBase]] = None,
+    ):
+        self._base_algo = base_algo
+        self._episodes = episodes
 
-    This metrics suggests how dynamics model is generalized to test sets.
-    If the MSE is large, the dynamics model are overfitting.
+    def __call__(
+        self,
+        algo: QLearningAlgoProtocol,
+        dataset: ReplayBuffer,
+    ) -> float:
+        total_diffs = []
+        episodes = self._episodes if self._episodes else dataset.episodes
+        for episode in episodes:
+            # TODO: handle different n_frames
+            for batch in make_batches(
+                episode, WINDOW_SIZE, dataset.transition_picker
+            ):
+                base_actions = self._base_algo.predict(batch.observations)
+                actions = algo.predict(batch.observations)
+                diff = ((actions - base_actions) ** 2).sum(axis=1).tolist()
+                total_diffs += diff
+        return float(np.mean(total_diffs))
+
+
+class CompareDiscreteActionMatchEvaluator(EvaluatorProtocol):
+    r"""Action matches between algorithms.
+
+    This metrics suggests how different the two algorithms are in discrete
+    action-space.
+    If the algorithm to compare with is near-optimal, the small action
+    difference would be better.
 
     .. math::
 
-        \mathbb{E}_{s_t, a_t, s_{t+1} \sim D} [(s_{t+1} - s')^2]
-
-    where :math:`s' \sim T(s_t, a_t)`.
+        \mathbb{E}_{s_t \sim D} [\parallel
+            \{\text{argmax}_a Q_{\theta_1}(s_t, a)
+            = \text{argmax}_a Q_{\theta_2}(s_t, a)\}]
 
     Args:
-        dynamics: dynamics model.
-        episodes: list of episodes.
-
-    Returns:
-        mean squared error.
-
+        base_algo: Target algorithm to comapre with.
+        episodes: Optional evaluation episodes. If it's not given, dataset
+            used in training will be used.
     """
-    total_errors = []
-    for episode in episodes:
-        for batch in _make_batches(episode, WINDOW_SIZE, dynamics.n_frames):
-            pred = dynamics.predict(batch.observations, batch.actions)
-            errors = ((batch.next_observations - pred[0]) ** 2).sum(axis=1)
-            total_errors += errors.tolist()
-    return float(np.mean(total_errors))
-
-
-def dynamics_reward_prediction_error_scorer(
-    dynamics: DynamicsProtocol, episodes: List[Episode]
-) -> float:
-    r"""Returns MSE of reward prediction.
+    _base_algo: QLearningAlgoProtocol
+    _episodes: Optional[Sequence[EpisodeBase]]
 
-    This metrics suggests how dynamics model is generalized to test sets.
-    If the MSE is large, the dynamics model are overfitting.
+    def __init__(
+        self,
+        base_algo: QLearningAlgoProtocol,
+        episodes: Optional[Sequence[EpisodeBase]] = None,
+    ):
+        self._base_algo = base_algo
+        self._episodes = episodes
+
+    def __call__(
+        self, algo: QLearningAlgoProtocol, dataset: ReplayBuffer
+    ) -> float:
+        total_matches = []
+        episodes = self._episodes if self._episodes else dataset.episodes
+        for episode in episodes:
+            # TODO: handle different n_frames
+            for batch in make_batches(
+                episode, WINDOW_SIZE, dataset.transition_picker
+            ):
+                base_actions = self._base_algo.predict(batch.observations)
+                actions = algo.predict(batch.observations)
+                match = (base_actions == actions).tolist()
+                total_matches += match
+        return float(np.mean(total_matches))
+
+
+class EnvironmentEvaluator(EvaluatorProtocol):
+    r"""Action matches between algorithms.
+
+    This metrics suggests how different the two algorithms are in discrete
+    action-space.
+    If the algorithm to compare with is near-optimal, the small action
+    difference would be better.
 
     .. math::
 
-        \mathbb{E}_{s_t, a_t, r_{t+1} \sim D} [(r_{t+1} - r')^2]
-
-    where :math:`r' \sim T(s_t, a_t)`.
+        \mathbb{E}_{s_t \sim D} [\parallel
+            \{\text{argmax}_a Q_{\theta_1}(s_t, a)
+            = \text{argmax}_a Q_{\theta_2}(s_t, a)\}]
+
+    Args:
+        env: Gym environment.
+        n_trials: Number of episodes to evaluate.
+        epsilon: Probability of random action.
+        render: Flag to turn on rendering.
+    """
+    _env: gym.Env[Any, Any]
+    _n_trials: int
+    _epsilon: float
+    _render: bool
 
-    Args:
-        dynamics: dynamics model.
-        episodes: list of episodes.
-
-    Returns:
-        mean squared error.
-
-    """
-    total_errors = []
-    for episode in episodes:
-        for batch in _make_batches(episode, WINDOW_SIZE, dynamics.n_frames):
-            pred = dynamics.predict(batch.observations, batch.actions)
-            rewards = batch.rewards
-            if dynamics.reward_scaler:
-                rewards = dynamics.reward_scaler.transform_numpy(rewards)
-            errors = ((rewards - pred[1]) ** 2).reshape(-1)
-            total_errors += errors.tolist()
-    return float(np.mean(total_errors))
-
-
-def dynamics_prediction_variance_scorer(
-    dynamics: DynamicsProtocol, episodes: List[Episode]
-) -> float:
-    """Returns prediction variance of ensemble dynamics.
-
-    This metrics suggests how dynamics model is confident of test sets.
-    If the variance is large, the dynamics model has large uncertainty.
-
-    Args:
-        dynamics: dynamics model.
-        episodes: list of episodes.
-
-    Returns:
-        variance.
-
-    """
-    total_variances = []
-    for episode in episodes:
-        for batch in _make_batches(episode, WINDOW_SIZE, dynamics.n_frames):
-            pred = dynamics.predict(batch.observations, batch.actions, True)
-            pred = cast(Tuple[np.ndarray, np.ndarray, np.ndarray], pred)
-            total_variances += pred[2].tolist()
-    return float(np.mean(total_variances))
+    def __init__(
+        self,
+        env: gym.Env[Any, Any],
+        n_trials: int = 10,
+        epsilon: float = 0.0,
+        render: bool = False,
+    ):
+        self._env = env
+        self._n_trials = n_trials
+        self._epsilon = epsilon
+        self._render = render
+
+    def __call__(
+        self, algo: QLearningAlgoProtocol, dataset: ReplayBuffer
+    ) -> float:
+        return evaluate_qlearning_with_environment(
+            algo=algo,
+            env=self._env,
+            n_trials=self._n_trials,
+            epsilon=self._epsilon,
+            render=self._render,
+        )
```

### Comparing `d3rlpy-1.1.1/d3rlpy/models/optimizers.py` & `d3rlpy-2.0.2/d3rlpy/models/optimizers.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,112 +1,84 @@
-import copy
-from typing import Any, Dict, Iterable, Tuple, Type, Union, cast
+import dataclasses
+from typing import Iterable, Tuple
 
-from torch import nn, optim
-from torch.optim import SGD, Adam, Optimizer, RMSprop
+from torch import nn
+from torch.optim import SGD, Adam, AdamW, Optimizer, RMSprop
 
-from ..decorators import pretty_repr
+from ..serializable_config import DynamicConfig, generate_config_registration
 
+__all__ = [
+    "OptimizerFactory",
+    "SGDFactory",
+    "AdamFactory",
+    "AdamWFactory",
+    "RMSpropFactory",
+    "register_optimizer_factory",
+    "make_optimizer_field",
+]
 
-@pretty_repr
-class OptimizerFactory:
+
+@dataclasses.dataclass()
+class OptimizerFactory(DynamicConfig):
     """A factory class that creates an optimizer object in a lazy way.
 
     The optimizers in algorithms can be configured through this factory class.
-
-    .. code-block:: python
-
-        from torch.optim Adam
-        from d3rlpy.optimizers import OptimizerFactory
-        from d3rlpy.algos import DQN
-
-        factory = OptimizerFactory(Adam, eps=0.001)
-
-        dqn = DQN(optim_factory=factory)
-
-    Args:
-        optim_cls: An optimizer class.
-        kwargs: arbitrary keyword-arguments.
-
     """
 
-    _optim_cls: Type[Optimizer]
-    _optim_kwargs: Dict[str, Any]
-
-    def __init__(self, optim_cls: Union[Type[Optimizer], str], **kwargs: Any):
-        if isinstance(optim_cls, str):
-            self._optim_cls = cast(Type[Optimizer], getattr(optim, optim_cls))
-        else:
-            self._optim_cls = optim_cls
-        self._optim_kwargs = kwargs
-
     def create(self, params: Iterable[nn.Parameter], lr: float) -> Optimizer:
         """Returns an optimizer object.
 
         Args:
             params (list): a list of PyTorch parameters.
             lr (float): learning rate.
 
         Returns:
             torch.optim.Optimizer: an optimizer object.
-
         """
-        return self._optim_cls(params, lr=lr, **self._optim_kwargs)
-
-    def get_params(self, deep: bool = False) -> Dict[str, Any]:
-        """Returns optimizer parameters.
-
-        Args:
-            deep: flag to deeply copy the parameters.
-
-        Returns:
-            optimizer parameters.
-
-        """
-        if deep:
-            params = copy.deepcopy(self._optim_kwargs)
-        else:
-            params = self._optim_kwargs
-        return {"optim_cls": self._optim_cls.__name__, **params}
+        raise NotImplementedError
 
 
+@dataclasses.dataclass()
 class SGDFactory(OptimizerFactory):
     """An alias for SGD optimizer.
 
     .. code-block:: python
 
         from d3rlpy.optimizers import SGDFactory
 
         factory = SGDFactory(weight_decay=1e-4)
 
     Args:
         momentum: momentum factor.
         dampening: dampening for momentum.
         weight_decay: weight decay (L2 penalty).
         nesterov: flag to enable Nesterov momentum.
-
     """
 
-    def __init__(
-        self,
-        momentum: float = 0,
-        dampening: float = 0,
-        weight_decay: float = 0,
-        nesterov: bool = False,
-        **kwargs: Any
-    ):
-        super().__init__(
-            optim_cls=SGD,
-            momentum=momentum,
-            dampening=dampening,
-            weight_decay=weight_decay,
-            nesterov=nesterov,
+    momentum: float = 0.0
+    dampening: float = 0.0
+    weight_decay: float = 0.0
+    nesterov: bool = False
+
+    def create(self, params: Iterable[nn.Parameter], lr: float) -> SGD:
+        return SGD(
+            params,
+            lr=lr,
+            momentum=self.momentum,
+            dampening=self.dampening,
+            weight_decay=self.weight_decay,
+            nesterov=self.nesterov,
         )
 
+    @staticmethod
+    def get_type() -> str:
+        return "sgd"
 
+
+@dataclasses.dataclass()
 class AdamFactory(OptimizerFactory):
     """An alias for Adam optimizer.
 
     .. code-block:: python
 
         from d3rlpy.optimizers import AdamFactory
 
@@ -114,34 +86,75 @@
 
     Args:
         betas: coefficients used for computing running averages of
             gradient and its square.
         eps: term added to the denominator to improve numerical stability.
         weight_decay: weight decay (L2 penalty).
         amsgrad: flag to use the AMSGrad variant of this algorithm.
+    """
 
+    betas: Tuple[float, float] = (0.9, 0.999)
+    eps: float = 1e-8
+    weight_decay: float = 0
+    amsgrad: bool = False
+
+    def create(self, params: Iterable[nn.Parameter], lr: float) -> Adam:
+        return Adam(
+            params,
+            lr=lr,
+            betas=self.betas,
+            eps=self.eps,
+            weight_decay=self.weight_decay,
+            amsgrad=self.amsgrad,
+        )
+
+    @staticmethod
+    def get_type() -> str:
+        return "adam"
+
+
+@dataclasses.dataclass()
+class AdamWFactory(OptimizerFactory):
+    """An alias for AdamW optimizer.
+
+    .. code-block:: python
+
+        from d3rlpy.optimizers import AdamWFactory
+
+        factory = AdamWFactory(weight_decay=1e-4)
+
+    Args:
+        betas: coefficients used for computing running averages of
+            gradient and its square.
+        eps: term added to the denominator to improve numerical stability.
+        weight_decay: weight decay (L2 penalty).
+        amsgrad: flag to use the AMSGrad variant of this algorithm.
     """
 
-    def __init__(
-        self,
-        betas: Tuple[float, float] = (0.9, 0.999),
-        eps: float = 1e-8,
-        weight_decay: float = 0,
-        amsgrad: bool = False,
-        **kwargs: Any
-    ):
-        super().__init__(
-            optim_cls=Adam,
-            betas=betas,
-            eps=eps,
-            weight_decay=weight_decay,
-            amsgrad=amsgrad,
+    betas: Tuple[float, float] = (0.9, 0.999)
+    eps: float = 1e-8
+    weight_decay: float = 0
+    amsgrad: bool = False
+
+    def create(self, params: Iterable[nn.Parameter], lr: float) -> AdamW:
+        return AdamW(
+            params,
+            lr=lr,
+            betas=self.betas,
+            eps=self.eps,
+            weight_decay=self.weight_decay,
+            amsgrad=self.amsgrad,
         )
 
+    @staticmethod
+    def get_type() -> str:
+        return "adam_w"
+
 
+@dataclasses.dataclass()
 class RMSpropFactory(OptimizerFactory):
     """An alias for RMSprop optimizer.
 
     .. code-block:: python
 
         from d3rlpy.optimizers import RMSpropFactory
 
@@ -150,27 +163,40 @@
     Args:
         alpha: smoothing constant.
         eps: term added to the denominator to improve numerical stability.
         weight_decay: weight decay (L2 penalty).
         momentum: momentum factor.
         centered: flag to compute the centered RMSProp, the gradient is
             normalized by an estimation of its variance.
-
     """
 
-    def __init__(
-        self,
-        alpha: float = 0.95,
-        eps: float = 1e-2,
-        weight_decay: float = 0,
-        momentum: float = 0,
-        centered: bool = True,
-        **kwargs: Any
-    ):
-        super().__init__(
-            optim_cls=RMSprop,
-            alpha=alpha,
-            eps=eps,
-            weight_decay=weight_decay,
-            momentum=momentum,
-            centered=centered,
+    alpha: float = 0.95
+    eps: float = 1e-2
+    weight_decay: float = 0.0
+    momentum: float = 0.0
+    centered: bool = True
+
+    def create(self, params: Iterable[nn.Parameter], lr: float) -> RMSprop:
+        return RMSprop(
+            params,
+            lr=lr,
+            alpha=self.alpha,
+            eps=self.eps,
+            weight_decay=self.weight_decay,
+            momentum=self.momentum,
+            centered=self.centered,
         )
+
+    @staticmethod
+    def get_type() -> str:
+        return "rmsprop"
+
+
+register_optimizer_factory, make_optimizer_field = generate_config_registration(
+    OptimizerFactory, lambda: AdamFactory()
+)
+
+
+register_optimizer_factory(SGDFactory)
+register_optimizer_factory(AdamFactory)
+register_optimizer_factory(AdamWFactory)
+register_optimizer_factory(RMSpropFactory)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/models/torch/distributions.py` & `d3rlpy-2.0.2/d3rlpy/models/torch/distributions.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 from abc import ABCMeta, abstractmethod
 from typing import Optional, Tuple
 
 import torch
 import torch.nn.functional as F
 from torch.distributions import Normal
 
+__all__ = [
+    "Distribution",
+    "GaussianDistribution",
+    "SquashedGaussianDistribution",
+]
+
 
 class Distribution(metaclass=ABCMeta):
     @abstractmethod
     def sample(self) -> torch.Tensor:
         pass
 
     @abstractmethod
```

### Comparing `d3rlpy-1.1.1/d3rlpy/models/torch/imitators.py` & `d3rlpy-2.0.2/d3rlpy/models/torch/imitators.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 import torch.nn.functional as F
 from torch import nn
 from torch.distributions import Normal
 from torch.distributions.kl import kl_divergence
 
 from .encoders import Encoder, EncoderWithAction
 
+__all__ = [
+    "ConditionalVAE",
+    "Imitator",
+    "DiscreteImitator",
+    "DeterministicRegressor",
+    "ProbablisticRegressor",
+]
+
 
 class ConditionalVAE(nn.Module):  # type: ignore
     _encoder_encoder: EncoderWithAction
     _decoder_encoder: EncoderWithAction
     _beta: float
     _min_logstd: float
     _max_logstd: float
@@ -128,14 +136,19 @@
 
     @abstractmethod
     def compute_error(
         self, x: torch.Tensor, action: torch.Tensor
     ) -> torch.Tensor:
         pass
 
+    @property
+    @abstractmethod
+    def encoder(self) -> Encoder:
+        pass
+
 
 class DiscreteImitator(Imitator):
     _encoder: Encoder
     _beta: float
     _fc: nn.Linear
 
     def __init__(self, encoder: Encoder, action_size: int, beta: float):
@@ -158,14 +171,18 @@
     def compute_error(
         self, x: torch.Tensor, action: torch.Tensor
     ) -> torch.Tensor:
         log_probs, logits = self.compute_log_probs_with_logits(x)
         penalty = (logits**2).mean()
         return F.nll_loss(log_probs, action.view(-1)) + self._beta * penalty
 
+    @property
+    def encoder(self) -> Encoder:
+        return self._encoder
+
 
 class DeterministicRegressor(Imitator):
     _encoder: Encoder
     _fc: nn.Linear
 
     def __init__(self, encoder: Encoder, action_size: int):
         super().__init__()
@@ -178,14 +195,18 @@
         return torch.tanh(h)
 
     def compute_error(
         self, x: torch.Tensor, action: torch.Tensor
     ) -> torch.Tensor:
         return F.mse_loss(self.forward(x), action)
 
+    @property
+    def encoder(self) -> Encoder:
+        return self._encoder
+
 
 class ProbablisticRegressor(Imitator):
     _min_logstd: float
     _max_logstd: float
     _encoder: Encoder
     _mu: nn.Linear
     _logstd: nn.Linear
@@ -223,7 +244,11 @@
         return actions.transpose(0, 1)
 
     def compute_error(
         self, x: torch.Tensor, action: torch.Tensor
     ) -> torch.Tensor:
         dist = self.dist(x)
         return F.mse_loss(torch.tanh(dist.rsample()), action)
+
+    @property
+    def encoder(self) -> Encoder:
+        return self._encoder
```

### Comparing `d3rlpy-1.1.1/d3rlpy/models/torch/policies.py` & `d3rlpy-2.0.2/d3rlpy/models/torch/policies.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,14 +6,25 @@
 import torch.nn.functional as F
 from torch import nn
 from torch.distributions import Categorical
 
 from .distributions import GaussianDistribution, SquashedGaussianDistribution
 from .encoders import Encoder, EncoderWithAction
 
+__all__ = [
+    "squash_action",
+    "Policy",
+    "DeterministicPolicy",
+    "DeterministicResidualPolicy",
+    "NormalPolicy",
+    "SquashedNormalPolicy",
+    "NonSquashedNormalPolicy",
+    "CategoricalPolicy",
+]
+
 
 def squash_action(
     dist: torch.distributions.Distribution, raw_action: torch.Tensor
 ) -> Tuple[torch.Tensor, torch.Tensor]:
     squashed_action = torch.tanh(raw_action)
     jacob = 2 * (math.log(2) - raw_action - F.softplus(-2 * raw_action))
     log_prob = (dist.log_prob(raw_action) - jacob).sum(dim=-1, keepdims=True)
@@ -41,15 +52,14 @@
 
     @abstractmethod
     def best_action(self, x: torch.Tensor) -> torch.Tensor:
         pass
 
 
 class DeterministicPolicy(Policy):
-
     _encoder: Encoder
     _fc: nn.Linear
 
     def __init__(self, encoder: Encoder, action_size: int):
         super().__init__()
         self._encoder = encoder
         self._fc = nn.Linear(encoder.get_feature_size(), action_size)
@@ -76,15 +86,14 @@
         )
 
     def best_action(self, x: torch.Tensor) -> torch.Tensor:
         return self.forward(x)
 
 
 class DeterministicResidualPolicy(Policy):
-
     _encoder: EncoderWithAction
     _scale: float
     _fc: nn.Linear
 
     def __init__(self, encoder: EncoderWithAction, scale: float):
         super().__init__()
         self._scale = scale
@@ -121,15 +130,14 @@
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         raise NotImplementedError(
             "deterministic policy does not support sample_n"
         )
 
 
 class NormalPolicy(Policy):
-
     _encoder: Encoder
     _action_size: int
     _min_logstd: float
     _max_logstd: float
     _use_std_parameter: bool
     _mu: nn.Linear
     _logstd: Union[nn.Linear, nn.Parameter]
@@ -287,15 +295,14 @@
             max_logstd=max_logstd,
             use_std_parameter=use_std_parameter,
             squash_distribution=False,
         )
 
 
 class CategoricalPolicy(Policy):
-
     _encoder: Encoder
     _fc: nn.Linear
 
     def __init__(self, encoder: Encoder, action_size: int):
         super().__init__()
         self._encoder = encoder
         self._fc = nn.Linear(encoder.get_feature_size(), action_size)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/base.py` & `d3rlpy-2.0.2/d3rlpy/models/torch/q_functions/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 from abc import ABCMeta, abstractmethod
 from typing import Optional
 
 import torch
 
 from ..encoders import Encoder, EncoderWithAction
 
+__all__ = ["QFunction", "DiscreteQFunction", "ContinuousQFunction"]
+
 
 class QFunction(metaclass=ABCMeta):
     @abstractmethod
     def compute_error(
         self,
         observations: torch.Tensor,
         actions: torch.Tensor,
@@ -17,14 +19,15 @@
         terminals: torch.Tensor,
         gamma: float = 0.99,
         reduction: str = "mean",
     ) -> torch.Tensor:
         pass
 
     @property
+    @abstractmethod
     def action_size(self) -> int:
         pass
 
 
 class DiscreteQFunction(QFunction):
     @abstractmethod
     def forward(self, x: torch.Tensor) -> torch.Tensor:
@@ -36,14 +39,15 @@
     ) -> torch.Tensor:
         pass
 
     def __call__(self, x: torch.Tensor) -> torch.Tensor:
         return self.forward(x)
 
     @property
+    @abstractmethod
     def encoder(self) -> Encoder:
         pass
 
 
 class ContinuousQFunction(QFunction):
     @abstractmethod
     def forward(self, x: torch.Tensor, action: torch.Tensor) -> torch.Tensor:
@@ -55,9 +59,10 @@
     ) -> torch.Tensor:
         pass
 
     def __call__(self, x: torch.Tensor, action: torch.Tensor) -> torch.Tensor:
         return self.forward(x, action)
 
     @property
+    @abstractmethod
     def encoder(self) -> EncoderWithAction:
         pass
```

### Comparing `d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/ensemble_q_function.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/bcq_impl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,184 +1,201 @@
-from typing import List, Optional, Union, cast
+import math
+from typing import cast
 
 import torch
-from torch import nn
+from torch.optim import Optimizer
 
-from .base import ContinuousQFunction, DiscreteQFunction
-
-
-def _reduce_ensemble(
-    y: torch.Tensor, reduction: str = "min", dim: int = 0, lam: float = 0.75
-) -> torch.Tensor:
-    if reduction == "min":
-        return y.min(dim=dim).values
-    elif reduction == "max":
-        return y.max(dim=dim).values
-    elif reduction == "mean":
-        return y.mean(dim=dim)
-    elif reduction == "none":
-        return y
-    elif reduction == "mix":
-        max_values = y.max(dim=dim).values
-        min_values = y.min(dim=dim).values
-        return lam * min_values + (1.0 - lam) * max_values
-    raise ValueError
-
-
-def _gather_quantiles_by_indices(
-    y: torch.Tensor, indices: torch.Tensor
-) -> torch.Tensor:
-    # TODO: implement this in general case
-    if y.dim() == 3:
-        # (N, batch, n_quantiles) -> (batch, n_quantiles)
-        return y.transpose(0, 1)[torch.arange(y.shape[1]), indices]
-    elif y.dim() == 4:
-        # (N, batch, action, n_quantiles) -> (batch, action, N, n_quantiles)
-        transposed_y = y.transpose(0, 1).transpose(1, 2)
-        # (batch, action, N, n_quantiles) -> (batch * action, N, n_quantiles)
-        flat_y = transposed_y.reshape(-1, y.shape[0], y.shape[3])
-        head_indices = torch.arange(y.shape[1] * y.shape[2])
-        # (batch * action, N, n_quantiles) -> (batch * action, n_quantiles)
-        gathered_y = flat_y[head_indices, indices.view(-1)]
-        # (batch * action, n_quantiles) -> (batch, action, n_quantiles)
-        return gathered_y.view(y.shape[1], y.shape[2], -1)
-    raise ValueError
-
-
-def _reduce_quantile_ensemble(
-    y: torch.Tensor, reduction: str = "min", dim: int = 0, lam: float = 0.75
-) -> torch.Tensor:
-    # reduction beased on expectation
-    mean = y.mean(dim=-1)
-    if reduction == "min":
-        indices = mean.min(dim=dim).indices
-        return _gather_quantiles_by_indices(y, indices)
-    elif reduction == "max":
-        indices = mean.max(dim=dim).indices
-        return _gather_quantiles_by_indices(y, indices)
-    elif reduction == "none":
-        return y
-    elif reduction == "mix":
-        min_indices = mean.min(dim=dim).indices
-        max_indices = mean.max(dim=dim).indices
-        min_values = _gather_quantiles_by_indices(y, min_indices)
-        max_values = _gather_quantiles_by_indices(y, max_indices)
-        return lam * min_values + (1.0 - lam) * max_values
-    raise ValueError
-
-
-class EnsembleQFunction(nn.Module):  # type: ignore
-    _action_size: int
-    _q_funcs: nn.ModuleList
+from ....dataset import Shape
+from ....models.torch import (
+    ConditionalVAE,
+    DeterministicResidualPolicy,
+    DiscreteImitator,
+    EnsembleContinuousQFunction,
+    EnsembleDiscreteQFunction,
+    compute_max_with_n_actions,
+)
+from ....torch_utility import TorchMiniBatch, train_api
+from .ddpg_impl import DDPGBaseImpl
+from .dqn_impl import DoubleDQNImpl
+
+__all__ = ["BCQImpl", "DiscreteBCQImpl"]
+
+
+class BCQImpl(DDPGBaseImpl):
+    _lam: float
+    _n_action_samples: int
+    _action_flexibility: float
+    _beta: float
+    _policy: DeterministicResidualPolicy
+    _targ_policy: DeterministicResidualPolicy
+    _imitator: ConditionalVAE
+    _imitator_optim: Optimizer
 
     def __init__(
         self,
-        q_funcs: Union[List[DiscreteQFunction], List[ContinuousQFunction]],
+        observation_shape: Shape,
+        action_size: int,
+        policy: DeterministicResidualPolicy,
+        q_func: EnsembleContinuousQFunction,
+        imitator: ConditionalVAE,
+        actor_optim: Optimizer,
+        critic_optim: Optimizer,
+        imitator_optim: Optimizer,
+        gamma: float,
+        tau: float,
+        lam: float,
+        n_action_samples: int,
+        action_flexibility: float,
+        beta: float,
+        device: str,
     ):
-        super().__init__()
-        self._action_size = q_funcs[0].action_size
-        self._q_funcs = nn.ModuleList(q_funcs)
-
-    def compute_error(
-        self,
-        observations: torch.Tensor,
-        actions: torch.Tensor,
-        rewards: torch.Tensor,
-        target: torch.Tensor,
-        terminals: torch.Tensor,
-        gamma: float = 0.99,
-    ) -> torch.Tensor:
-        assert target.ndim == 2
+        super().__init__(
+            observation_shape=observation_shape,
+            action_size=action_size,
+            policy=policy,
+            q_func=q_func,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            gamma=gamma,
+            tau=tau,
+            device=device,
+        )
+        self._lam = lam
+        self._n_action_samples = n_action_samples
+        self._action_flexibility = action_flexibility
+        self._beta = beta
+        self._imitator = imitator
+        self._imitator_optim = imitator_optim
+
+    def compute_actor_loss(self, batch: TorchMiniBatch) -> torch.Tensor:
+        latent = torch.randn(
+            batch.observations.shape[0],
+            2 * self._action_size,
+            device=self._device,
+        )
+        clipped_latent = latent.clamp(-0.5, 0.5)
+        sampled_action = self._imitator.decode(
+            batch.observations, clipped_latent
+        )
+        action = self._policy(batch.observations, sampled_action)
+        return -self._q_func(batch.observations, action, "none")[0].mean()
 
-        td_sum = torch.tensor(
-            0.0, dtype=torch.float32, device=observations.device
+    @train_api
+    def update_imitator(self, batch: TorchMiniBatch) -> float:
+        self._imitator_optim.zero_grad()
+
+        loss = self._imitator.compute_error(batch.observations, batch.actions)
+
+        loss.backward()
+        self._imitator_optim.step()
+
+        return float(loss.cpu().detach().numpy())
+
+    def _repeat_observation(self, x: torch.Tensor) -> torch.Tensor:
+        # (batch_size, *obs_shape) -> (batch_size, n, *obs_shape)
+        repeat_shape = (x.shape[0], self._n_action_samples, *x.shape[1:])
+        repeated_x = x.view(x.shape[0], 1, *x.shape[1:]).expand(repeat_shape)
+        return repeated_x
+
+    def _sample_repeated_action(
+        self, repeated_x: torch.Tensor, target: bool = False
+    ) -> torch.Tensor:
+        # TODO: this seems to be slow with image observation
+        flattened_x = repeated_x.reshape(-1, *self.observation_shape)
+        # sample latent variable
+        latent = torch.randn(
+            flattened_x.shape[0], 2 * self._action_size, device=self._device
         )
-        for q_func in self._q_funcs:
-            loss = q_func.compute_error(
-                observations=observations,
-                actions=actions,
-                rewards=rewards,
-                target=target,
-                terminals=terminals,
-                gamma=gamma,
-                reduction="none",
-            )
-            td_sum += loss.mean()
-        return td_sum
+        clipped_latent = latent.clamp(-0.5, 0.5)
+        # sample action
+        sampled_action = self._imitator.decode(flattened_x, clipped_latent)
+        # add residual action
+        policy = self._targ_policy if target else self._policy
+        action = policy(flattened_x, sampled_action)
+        return action.view(-1, self._n_action_samples, self._action_size)
 
-    def _compute_target(
+    def _predict_value(
         self,
-        x: torch.Tensor,
-        action: Optional[torch.Tensor] = None,
-        reduction: str = "min",
-        lam: float = 0.75,
-    ) -> torch.Tensor:
-        values_list: List[torch.Tensor] = []
-        for q_func in self._q_funcs:
-            target = q_func.compute_target(x, action)
-            values_list.append(target.reshape(1, x.shape[0], -1))
-
-        values = torch.cat(values_list, dim=0)
-
-        if action is None:
-            # mean Q function
-            if values.shape[2] == self._action_size:
-                return _reduce_ensemble(values, reduction)
-            # distributional Q function
-            n_q_funcs = values.shape[0]
-            values = values.view(n_q_funcs, x.shape[0], self._action_size, -1)
-            return _reduce_quantile_ensemble(values, reduction)
-
-        if values.shape[2] == 1:
-            return _reduce_ensemble(values, reduction, lam=lam)
-
-        return _reduce_quantile_ensemble(values, reduction, lam=lam)
-
-    @property
-    def q_funcs(self) -> nn.ModuleList:
-        return self._q_funcs
-
-
-class EnsembleDiscreteQFunction(EnsembleQFunction):
-    def forward(self, x: torch.Tensor, reduction: str = "mean") -> torch.Tensor:
-        values = []
-        for q_func in self._q_funcs:
-            values.append(q_func(x).view(1, x.shape[0], self._action_size))
-        return _reduce_ensemble(torch.cat(values, dim=0), reduction)
-
-    def __call__(
-        self, x: torch.Tensor, reduction: str = "mean"
+        repeated_x: torch.Tensor,
+        action: torch.Tensor,
     ) -> torch.Tensor:
-        return cast(torch.Tensor, super().__call__(x, reduction))
+        # TODO: this seems to be slow with image observation
+        # (batch_size, n, *obs_shape) -> (batch_size * n, *obs_shape)
+        flattened_x = repeated_x.reshape(-1, *self.observation_shape)
+        # (batch_size, n, action_size) -> (batch_size * n, action_size)
+        flattend_action = action.view(-1, self.action_size)
+        # estimate values
+        return self._q_func(flattened_x, flattend_action, "none")
+
+    def inner_predict_best_action(self, x: torch.Tensor) -> torch.Tensor:
+        # TODO: this seems to be slow with image observation
+        repeated_x = self._repeat_observation(x)
+        action = self._sample_repeated_action(repeated_x)
+        values = self._predict_value(repeated_x, action)[0]
+        # pick the best (batch_size * n) -> (batch_size,)
+        index = values.view(-1, self._n_action_samples).argmax(dim=1)
+        return action[torch.arange(action.shape[0]), index]
+
+    def inner_sample_action(self, x: torch.Tensor) -> torch.Tensor:
+        return self.inner_predict_best_action(x)
+
+    def compute_target(self, batch: TorchMiniBatch) -> torch.Tensor:
+        # TODO: this seems to be slow with image observation
+        with torch.no_grad():
+            repeated_x = self._repeat_observation(batch.next_observations)
+            actions = self._sample_repeated_action(repeated_x, True)
 
-    def compute_target(
-        self,
-        x: torch.Tensor,
-        action: Optional[torch.Tensor] = None,
-        reduction: str = "min",
-        lam: float = 0.75,
-    ) -> torch.Tensor:
-        return self._compute_target(x, action, reduction, lam)
+            values = compute_max_with_n_actions(
+                batch.next_observations, actions, self._targ_q_func, self._lam
+            )
 
+            return values
 
-class EnsembleContinuousQFunction(EnsembleQFunction):
-    def forward(
-        self, x: torch.Tensor, action: torch.Tensor, reduction: str = "mean"
-    ) -> torch.Tensor:
-        values = []
-        for q_func in self._q_funcs:
-            values.append(q_func(x, action).view(1, x.shape[0], 1))
-        return _reduce_ensemble(torch.cat(values, dim=0), reduction)
 
-    def __call__(
-        self, x: torch.Tensor, action: torch.Tensor, reduction: str = "mean"
-    ) -> torch.Tensor:
-        return cast(torch.Tensor, super().__call__(x, action, reduction))
+class DiscreteBCQImpl(DoubleDQNImpl):
+    _action_flexibility: float
+    _beta: float
+    _imitator: DiscreteImitator
 
-    def compute_target(
+    def __init__(
         self,
-        x: torch.Tensor,
-        action: torch.Tensor,
-        reduction: str = "min",
-        lam: float = 0.75,
-    ) -> torch.Tensor:
-        return self._compute_target(x, action, reduction, lam)
+        observation_shape: Shape,
+        action_size: int,
+        q_func: EnsembleDiscreteQFunction,
+        imitator: DiscreteImitator,
+        optim: Optimizer,
+        gamma: float,
+        action_flexibility: float,
+        beta: float,
+        device: str,
+    ):
+        super().__init__(
+            observation_shape=observation_shape,
+            action_size=action_size,
+            q_func=q_func,
+            optim=optim,
+            gamma=gamma,
+            device=device,
+        )
+        self._action_flexibility = action_flexibility
+        self._beta = beta
+        self._imitator = imitator
+
+    def compute_loss(
+        self, batch: TorchMiniBatch, q_tpn: torch.Tensor
+    ) -> torch.Tensor:
+        loss = super().compute_loss(batch, q_tpn)
+        imitator_loss = self._imitator.compute_error(
+            batch.observations, batch.actions.long()
+        )
+        return loss + imitator_loss
+
+    def inner_predict_best_action(self, x: torch.Tensor) -> torch.Tensor:
+        log_probs = self._imitator(x)
+        ratio = log_probs - log_probs.max(dim=1, keepdim=True).values
+        mask = (ratio > math.log(self._action_flexibility)).float()
+        value = self._q_func(x)
+        # add a small constant value to deal with the case where the all
+        # actions except the min value are masked
+        normalized_value = value - value.min(dim=1, keepdim=True).values + 1e-5
+        action = (normalized_value * cast(torch.Tensor, mask)).argmax(dim=1)
+        return action
```

### Comparing `d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/fqf_q_function.py` & `d3rlpy-2.0.2/d3rlpy/models/torch/q_functions/fqf_q_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from .iqn_q_function import compute_iqn_feature
 from .utility import (
     compute_quantile_loss,
     compute_reduce,
     pick_quantile_value_by_action,
 )
 
+__all__ = ["DiscreteFQFQFunction", "ContinuousFQFQFunction"]
+
 
 def _make_taus(
     h: torch.Tensor,
     proposal: nn.Linear,
 ) -> Tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
     proposals = proposal(h.detach())
```

### Comparing `d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/iqn_q_function.py` & `d3rlpy-2.0.2/d3rlpy/models/torch/q_functions/iqn_q_function.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,16 @@
 from .base import ContinuousQFunction, DiscreteQFunction
 from .utility import (
     compute_quantile_loss,
     compute_reduce,
     pick_quantile_value_by_action,
 )
 
+__all__ = ["DiscreteIQNQFunction", "ContinuousIQNQFunction"]
+
 
 def _make_taus(
     h: torch.Tensor, n_quantiles: int, training: bool
 ) -> torch.Tensor:
     if training:
         taus = torch.rand(h.shape[0], n_quantiles, device=h.device)
     else:
```

### Comparing `d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/mean_q_function.py` & `d3rlpy-2.0.2/d3rlpy/models/torch/q_functions/mean_q_function.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 import torch.nn.functional as F
 from torch import nn
 
 from ..encoders import Encoder, EncoderWithAction
 from .base import ContinuousQFunction, DiscreteQFunction
 from .utility import compute_huber_loss, compute_reduce, pick_value_by_action
 
+__all__ = ["DiscreteMeanQFunction", "ContinuousMeanQFunction"]
+
 
 class DiscreteMeanQFunction(DiscreteQFunction, nn.Module):  # type: ignore
     _action_size: int
     _encoder: Encoder
     _fc: nn.Linear
 
     def __init__(self, encoder: Encoder, action_size: int):
```

### Comparing `d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/qr_q_function.py` & `d3rlpy-2.0.2/d3rlpy/models/torch/q_functions/qr_q_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from .base import ContinuousQFunction, DiscreteQFunction
 from .utility import (
     compute_quantile_loss,
     compute_reduce,
     pick_quantile_value_by_action,
 )
 
+__all__ = ["DiscreteQRQFunction", "ContinuousQRQFunction"]
+
 
 def _make_taus(h: torch.Tensor, n_quantiles: int) -> torch.Tensor:
     steps = torch.arange(n_quantiles, dtype=torch.float32, device=h.device)
     taus = ((steps + 1).float() / n_quantiles).view(1, -1)
     taus_dot = (steps.float() / n_quantiles).view(1, -1)
     return (taus + taus_dot) / 2.0
```

### Comparing `d3rlpy-1.1.1/d3rlpy/models/torch/q_functions/utility.py` & `d3rlpy-2.0.2/d3rlpy/models/torch/q_functions/utility.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,21 @@
 from typing import cast
 
 import torch
 import torch.nn.functional as F
 
+__all__ = [
+    "pick_value_by_action",
+    "pick_quantile_value_by_action",
+    "compute_huber_loss",
+    "compute_quantile_huber_loss",
+    "compute_quantile_loss",
+    "compute_reduce",
+]
+
 
 def pick_value_by_action(
     values: torch.Tensor, action: torch.Tensor, keepdim: bool = False
 ) -> torch.Tensor:
     assert values.ndim == 2
     action_size = values.shape[1]
     one_hot = F.one_hot(action.view(-1), num_classes=action_size)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/models/torch/v_functions.py` & `d3rlpy-2.0.2/d3rlpy/models/torch/v_functions.py`

 * *Files 25% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 import torch
 import torch.nn.functional as F
 from torch import nn
 
 from .encoders import Encoder
 
+__all__ = ["ValueFunction"]
+
 
 class ValueFunction(nn.Module):  # type: ignore
     _encoder: Encoder
     _fc: nn.Linear
 
     def __init__(self, encoder: Encoder):
         super().__init__()
```

### Comparing `d3rlpy-1.1.1/d3rlpy/online/explorers.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/explorers.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from abc import ABCMeta, abstractmethod
 from typing import Any, List, Optional, Union
 
 import numpy as np
 from typing_extensions import Protocol
 
-from ..preprocessing.action_scalers import ActionScaler, MinMaxActionScaler
+from ...preprocessing.action_scalers import ActionScaler, MinMaxActionScaler
+
+__all__ = [
+    "Explorer",
+    "ConstantEpsilonGreedy",
+    "LinearDecayEpsilonGreedy",
+    "NormalNoise",
+]
 
 
 class _ActionProtocol(Protocol):
     def predict(self, x: Union[np.ndarray, List[Any]]) -> np.ndarray:
         ...
 
-    def sample_action(self, x: Union[np.ndarray, List[Any]]) -> np.ndarray:
-        ...
-
     @property
     def action_size(self) -> Optional[int]:
         ...
 
     @property
     def action_scaler(self) -> Optional[ActionScaler]:
         ...
@@ -32,15 +36,14 @@
 
 
 class ConstantEpsilonGreedy(Explorer):
     """:math:`\\epsilon`-greedy explorer with constant :math:`\\epsilon`.
 
     Args:
         epsilon (float): the constant :math:`\\epsilon`.
-
     """
 
     _epsilon: float
 
     def __init__(self, epsilon: float):
         self._epsilon = epsilon
 
@@ -53,18 +56,17 @@
         return np.where(is_random, random_actions, greedy_actions)
 
 
 class LinearDecayEpsilonGreedy(Explorer):
     """:math:`\\epsilon`-greedy explorer with linear decay schedule.
 
     Args:
-        start_epsilon (float): the beginning :math:`\\epsilon`.
-        end_epsilon (float): the end :math:`\\epsilon`.
-        duration (int): the scheduling duration.
-
+        start_epsilon (float): Initial :math:`\\epsilon`.
+        end_epsilon (float): Final :math:`\\epsilon`.
+        duration (int): Scheduling duration.
     """
 
     _start_epsilon: float
     _end_epsilon: float
     _duration: int
 
     def __init__(
@@ -79,47 +81,44 @@
 
     def sample(
         self, algo: _ActionProtocol, x: np.ndarray, step: int
     ) -> np.ndarray:
         """Returns :math:`\\epsilon`-greedy action.
 
         Args:
-            algo: algorithm.
-            x: observation.
-            step: current environment step.
+            algo: Algorithm.
+            x: Observation.
+            step: Current environment step.
 
         Returns:
             :math:`\\epsilon`-greedy action.
-
         """
         greedy_actions = algo.predict(x)
         random_actions = np.random.randint(algo.action_size, size=x.shape[0])
         is_random = np.random.random(x.shape[0]) < self.compute_epsilon(step)
         return np.where(is_random, random_actions, greedy_actions)
 
     def compute_epsilon(self, step: int) -> float:
         """Returns decayed :math:`\\epsilon`.
 
         Returns:
             :math:`\\epsilon`.
-
         """
         if step >= self._duration:
             return self._end_epsilon
         base = self._start_epsilon - self._end_epsilon
         return base * (1.0 - step / self._duration) + self._end_epsilon
 
 
 class NormalNoise(Explorer):
     """Normal noise explorer.
 
     Args:
-        mean (float): mean.
-        std (float): standard deviation.
-
+        mean (float): Mean.
+        std (float): Standard deviation.
     """
 
     _mean: float
     _std: float
 
     def __init__(self, mean: float = 0.0, std: float = 0.1):
         self._mean = mean
@@ -127,29 +126,25 @@
 
     def sample(
         self, algo: _ActionProtocol, x: np.ndarray, step: int
     ) -> np.ndarray:
         """Returns action with noise injection.
 
         Args:
-            algo: algorithm.
-            x: observation.
+            algo: Algorithm.
+            x: Observation.
 
         Returns:
-            action with noise injection.
-
+            Action with noise injection.
         """
         action = algo.predict(x)
-        # FIXME: Scalar noise works better for some reason.
-        #        But this is different from paper.
-        noise = np.random.normal(self._mean, self._std)
+        noise = np.random.normal(self._mean, self._std, size=action.shape)
 
         if isinstance(algo.action_scaler, MinMaxActionScaler):
             # scale noise
-            params = algo.action_scaler.get_params()
-            minimum = params["minimum"]
-            maximum = params["maximum"]
+            minimum = algo.action_scaler.minimum
+            maximum = algo.action_scaler.maximum
         else:
             minimum = -1.0
             maximum = 1.0
 
         return np.clip(action + noise, minimum, maximum)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/ope/torch/fqe_impl.py` & `d3rlpy-2.0.2/d3rlpy/algos/qlearning/torch/plas_impl.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,202 +1,162 @@
 import copy
-from abc import abstractmethod
-from typing import Optional, Sequence
 
-import numpy as np
 import torch
 from torch.optim import Optimizer
 
-from ...algos.torch.base import TorchImplBase
-from ...algos.torch.utility import (
-    ContinuousQFunctionMixin,
-    DiscreteQFunctionMixin,
-)
-from ...gpu import Device
-from ...models.builders import (
-    create_continuous_q_function,
-    create_discrete_q_function,
-)
-from ...models.encoders import EncoderFactory
-from ...models.optimizers import OptimizerFactory
-from ...models.q_functions import QFunctionFactory
-from ...models.torch import (
+from ....dataset import Shape
+from ....models.torch import (
+    ConditionalVAE,
+    DeterministicPolicy,
+    DeterministicResidualPolicy,
     EnsembleContinuousQFunction,
-    EnsembleDiscreteQFunction,
-    EnsembleQFunction,
 )
-from ...preprocessing import ActionScaler, RewardScaler, Scaler
-from ...torch_utility import TorchMiniBatch, hard_sync, torch_api, train_api
+from ....torch_utility import TorchMiniBatch, soft_sync, train_api
+from .ddpg_impl import DDPGBaseImpl
 
+__all__ = ["PLASImpl", "PLASWithPerturbationImpl"]
 
-class FQEBaseImpl(TorchImplBase):
 
-    _learning_rate: float
-    _optim_factory: OptimizerFactory
-    _encoder_factory: EncoderFactory
-    _q_func_factory: QFunctionFactory
-    _gamma: float
-    _n_critics: int
-    _use_gpu: Optional[Device]
-    _q_func: Optional[EnsembleQFunction]
-    _targ_q_func: Optional[EnsembleQFunction]
-    _optim: Optional[Optimizer]
+class PLASImpl(DDPGBaseImpl):
+    _lam: float
+    _beta: float
+    _policy: DeterministicPolicy
+    _targ_policy: DeterministicPolicy
+    _imitator: ConditionalVAE
+    _imitator_optim: Optimizer
 
     def __init__(
         self,
-        observation_shape: Sequence[int],
+        observation_shape: Shape,
         action_size: int,
-        learning_rate: float,
-        optim_factory: OptimizerFactory,
-        encoder_factory: EncoderFactory,
-        q_func_factory: QFunctionFactory,
+        policy: DeterministicPolicy,
+        q_func: EnsembleContinuousQFunction,
+        imitator: ConditionalVAE,
+        actor_optim: Optimizer,
+        critic_optim: Optimizer,
+        imitator_optim: Optimizer,
         gamma: float,
-        n_critics: int,
-        use_gpu: Optional[Device],
-        scaler: Optional[Scaler],
-        action_scaler: Optional[ActionScaler],
-        reward_scaler: Optional[RewardScaler],
+        tau: float,
+        lam: float,
+        device: str,
     ):
         super().__init__(
             observation_shape=observation_shape,
             action_size=action_size,
-            scaler=scaler,
-            action_scaler=action_scaler,
-            reward_scaler=reward_scaler,
-        )
-        self._learning_rate = learning_rate
-        self._optim_factory = optim_factory
-        self._encoder_factory = encoder_factory
-        self._q_func_factory = q_func_factory
-        self._gamma = gamma
-        self._n_critics = n_critics
-        self._use_gpu = use_gpu
-
-        # initialized in build
-        self._q_func = None
-        self._targ_q_func = None
-        self._optim = None
-
-    def build(self) -> None:
-        self._build_network()
-
-        self._targ_q_func = copy.deepcopy(self._q_func)
-
-        if self._use_gpu:
-            self.to_gpu(self._use_gpu)
-        else:
-            self.to_cpu()
-
-        self._build_optim()
-
-    @abstractmethod
-    def _build_network(self) -> None:
-        pass
-
-    def _build_optim(self) -> None:
-        assert self._q_func is not None
-        self._optim = self._optim_factory.create(
-            self._q_func.parameters(), lr=self._learning_rate
-        )
+            policy=policy,
+            q_func=q_func,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            gamma=gamma,
+            tau=tau,
+            device=device,
+        )
+        self._lam = lam
+        self._imitator = imitator
+        self._imitator_optim = imitator_optim
 
     @train_api
-    @torch_api()
-    def update(
-        self, batch: TorchMiniBatch, next_actions: torch.Tensor
-    ) -> np.ndarray:
-        assert self._optim is not None
+    def update_imitator(self, batch: TorchMiniBatch) -> float:
+        self._imitator_optim.zero_grad()
 
-        q_tpn = self.compute_target(batch, next_actions)
-        loss = self.compute_loss(batch, q_tpn)
+        loss = self._imitator.compute_error(batch.observations, batch.actions)
 
-        self._optim.zero_grad()
         loss.backward()
-        self._optim.step()
+        self._imitator_optim.step()
 
-        return loss.cpu().detach().numpy()
+        return float(loss.cpu().detach().numpy())
 
-    def compute_loss(
-        self,
-        batch: TorchMiniBatch,
-        q_tpn: torch.Tensor,
-    ) -> torch.Tensor:
-        assert self._q_func is not None
-        return self._q_func.compute_error(
-            observations=batch.observations,
-            actions=batch.actions,
-            rewards=batch.rewards,
-            target=q_tpn,
-            terminals=batch.terminals,
-            gamma=self._gamma**batch.n_steps,
-        )
+    def compute_actor_loss(self, batch: TorchMiniBatch) -> torch.Tensor:
+        latent_actions = 2.0 * self._policy(batch.observations)
+        actions = self._imitator.decode(batch.observations, latent_actions)
+        return -self._q_func(batch.observations, actions, "none")[0].mean()
+
+    def inner_predict_best_action(self, x: torch.Tensor) -> torch.Tensor:
+        return self._imitator.decode(x, 2.0 * self._policy(x))
 
-    def compute_target(
-        self, batch: TorchMiniBatch, next_actions: torch.Tensor
-    ) -> torch.Tensor:
-        assert self._targ_q_func is not None
+    def inner_sample_action(self, x: torch.Tensor) -> torch.Tensor:
+        return self.inner_predict_best_action(x)
+
+    def compute_target(self, batch: TorchMiniBatch) -> torch.Tensor:
         with torch.no_grad():
+            latent_actions = 2.0 * self._targ_policy(batch.next_observations)
+            actions = self._imitator.decode(
+                batch.next_observations, latent_actions
+            )
             return self._targ_q_func.compute_target(
-                batch.next_observations, next_actions
+                batch.next_observations,
+                actions,
+                "mix",
+                self._lam,
             )
 
-    def update_target(self) -> None:
-        assert self._q_func is not None
-        assert self._targ_q_func is not None
-        hard_sync(self._targ_q_func, self._q_func)
-
-    def save_policy(self, fname: str) -> None:
-        raise NotImplementedError
-
-
-class FQEImpl(ContinuousQFunctionMixin, FQEBaseImpl):
-
-    _q_func: Optional[EnsembleContinuousQFunction]
-    _targ_q_func: Optional[EnsembleContinuousQFunction]
-
-    def _build_network(self) -> None:
-        self._q_func = create_continuous_q_function(
-            self._observation_shape,
-            self._action_size,
-            self._encoder_factory,
-            self._q_func_factory,
-            n_ensembles=self._n_critics,
-        )
 
+class PLASWithPerturbationImpl(PLASImpl):
+    _perturbation: DeterministicResidualPolicy
+    _targ_perturbation: DeterministicResidualPolicy
 
-class DiscreteFQEImpl(DiscreteQFunctionMixin, FQEBaseImpl):
-
-    _q_func: Optional[EnsembleDiscreteQFunction]
-    _targ_q_func: Optional[EnsembleDiscreteQFunction]
-
-    def _build_network(self) -> None:
-        self._q_func = create_discrete_q_function(
-            self._observation_shape,
-            self._action_size,
-            self._encoder_factory,
-            self._q_func_factory,
-            n_ensembles=self._n_critics,
-        )
-
-    def compute_loss(
+    def __init__(
         self,
-        batch: TorchMiniBatch,
-        q_tpn: torch.Tensor,
-    ) -> torch.Tensor:
-        assert self._q_func is not None
-        return self._q_func.compute_error(
-            observations=batch.observations,
-            actions=batch.actions.long(),
-            rewards=batch.rewards,
-            target=q_tpn,
-            terminals=batch.terminals,
-            gamma=self._gamma**batch.n_steps,
-        )
+        observation_shape: Shape,
+        action_size: int,
+        policy: DeterministicPolicy,
+        q_func: EnsembleContinuousQFunction,
+        imitator: ConditionalVAE,
+        perturbation: DeterministicResidualPolicy,
+        actor_optim: Optimizer,
+        critic_optim: Optimizer,
+        imitator_optim: Optimizer,
+        gamma: float,
+        tau: float,
+        lam: float,
+        device: str,
+    ):
+        super().__init__(
+            observation_shape=observation_shape,
+            action_size=action_size,
+            policy=policy,
+            q_func=q_func,
+            imitator=imitator,
+            actor_optim=actor_optim,
+            critic_optim=critic_optim,
+            imitator_optim=imitator_optim,
+            gamma=gamma,
+            tau=tau,
+            lam=lam,
+            device=device,
+        )
+        self._perturbation = perturbation
+        self._targ_perturbation = copy.deepcopy(perturbation)
+
+    def compute_actor_loss(self, batch: TorchMiniBatch) -> torch.Tensor:
+        latent_actions = 2.0 * self._policy(batch.observations)
+        actions = self._imitator.decode(batch.observations, latent_actions)
+        residual_actions = self._perturbation(batch.observations, actions)
+        q_value = self._q_func(batch.observations, residual_actions, "none")
+        return -q_value[0].mean()
+
+    def inner_predict_best_action(self, x: torch.Tensor) -> torch.Tensor:
+        action = self._imitator.decode(x, 2.0 * self._policy(x))
+        return self._perturbation(x, action)
+
+    def inner_sample_action(self, x: torch.Tensor) -> torch.Tensor:
+        return self.inner_predict_best_action(x)
 
-    def compute_target(
-        self, batch: TorchMiniBatch, next_actions: torch.Tensor
-    ) -> torch.Tensor:
-        assert self._targ_q_func is not None
+    def compute_target(self, batch: TorchMiniBatch) -> torch.Tensor:
         with torch.no_grad():
+            latent_actions = 2.0 * self._targ_policy(batch.next_observations)
+            actions = self._imitator.decode(
+                batch.next_observations, latent_actions
+            )
+            residual_actions = self._targ_perturbation(
+                batch.next_observations, actions
+            )
             return self._targ_q_func.compute_target(
                 batch.next_observations,
-                next_actions.long(),
+                residual_actions,
+                reduction="mix",
+                lam=self._lam,
             )
+
+    def update_actor_target(self) -> None:
+        super().update_actor_target()
+        soft_sync(self._targ_perturbation, self._perturbation, self._tau)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/preprocessing/action_scalers.py` & `d3rlpy-2.0.2/d3rlpy/preprocessing/action_scalers.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,262 +1,187 @@
-from typing import Any, ClassVar, Dict, List, Optional, Type
+import dataclasses
+from typing import Any, Optional, Sequence
 
 import gym
 import numpy as np
 import torch
 
-from ..dataset import MDPDataset, Transition
-from ..decorators import pretty_repr
+from ..dataset import (
+    EpisodeBase,
+    TrajectorySlicerProtocol,
+    TransitionPickerProtocol,
+)
+from ..serializable_config import (
+    generate_optional_config_generation,
+    make_optional_numpy_field,
+)
+from .base import Scaler, add_leading_dims, add_leading_dims_numpy
+
+__all__ = [
+    "ActionScaler",
+    "MinMaxActionScaler",
+    "register_action_scaler",
+    "make_action_scaler_field",
+]
 
 
-@pretty_repr
-class ActionScaler:
-    TYPE: ClassVar[str] = "none"
-
-    def fit(self, transitions: List[Transition]) -> None:
-        """Estimates scaling parameters from dataset.
-
-        Args:
-            transitions: a list of transition objects.
-
-        """
-        raise NotImplementedError
-
-    def fit_with_env(self, env: gym.Env) -> None:
-        """Gets scaling parameters from environment.
-
-        Args:
-            env: gym environment.
-
-        """
-        raise NotImplementedError
-
-    def transform(self, action: torch.Tensor) -> torch.Tensor:
-        """Returns processed action.
-
-        Args:
-            action: action vector.
-
-        Returns:
-            processed action.
-
-        """
-        raise NotImplementedError
-
-    def reverse_transform(self, action: torch.Tensor) -> torch.Tensor:
-        """Returns reversely transformed action.
-
-        Args:
-            action: action vector.
-
-        Returns:
-            reversely transformed action.
-
-        """
-        raise NotImplementedError
-
-    def reverse_transform_numpy(self, action: np.ndarray) -> np.ndarray:
-        """Returns reversely transformed action in numpy array.
-
-        Args:
-            action: action vector.
-
-        Returns:
-            reversely transformed action.
-
-        """
-        raise NotImplementedError
-
-    def get_type(self) -> str:
-        """Returns action scaler type.
-
-        Returns:
-            action scaler type.
-
-        """
-        return self.TYPE
-
-    def get_params(self, deep: bool = False) -> Dict[str, Any]:
-        """Returns action scaler params.
-
-        Args:
-            deep: flag to deepcopy parameters.
-
-        Returns:
-            action scaler parameters.
-
-        """
-        raise NotImplementedError
+class ActionScaler(Scaler):
+    pass
 
 
+@dataclasses.dataclass()
 class MinMaxActionScaler(ActionScaler):
     r"""Min-Max normalization action preprocessing.
 
     Actions will be normalized in range ``[-1.0, 1.0]``.
 
     .. math::
 
         a' = (a - \min{a}) / (\max{a} - \min{a}) * 2 - 1
 
     .. code-block:: python
 
-        from d3rlpy.dataset import MDPDataset
-        from d3rlpy.algos import CQL
-
-        dataset = MDPDataset(observations, actions, rewards, terminals)
-
-        # initialize algorithm with MinMaxActionScaler
-        cql = CQL(action_scaler='min_max')
-
-        # scaler is initialized from the given transitions
-        transitions = []
-        for episode in dataset.episodes:
-            transitions += episode.transitions
-        cql.fit(transitions)
-
-    You can also initialize with :class:`d3rlpy.dataset.MDPDataset` object or
-    manually.
-
-    .. code-block:: python
-
         from d3rlpy.preprocessing import MinMaxActionScaler
+        from d3rlpy.algos import CQLConfig
 
-        # initialize with dataset
-        scaler = MinMaxActionScaler(dataset)
+        # normalize based on datasets or environments
+        cql = CQLConfig(action_scaler=MinMaxActionScaler()).create()
 
-        # initialize manually
+        # manually initialize
         minimum = actions.min(axis=0)
         maximum = actions.max(axis=0)
         action_scaler = MinMaxActionScaler(minimum=minimum, maximum=maximum)
-
-        cql = CQL(action_scaler=action_scaler)
+        cql = CQLConfig(action_scaler=action_scaler).create()
 
     Args:
-        dataset (d3rlpy.dataset.MDPDataset): dataset object.
-        min (numpy.ndarray): minimum values at each entry.
-        max (numpy.ndarray): maximum values at each entry.
-
+        minimum (numpy.ndarray): Minimum values at each entry.
+        maximum (numpy.ndarray): Maximum values at each entry.
     """
+    minimum: Optional[np.ndarray] = make_optional_numpy_field()
+    maximum: Optional[np.ndarray] = make_optional_numpy_field()
 
-    TYPE: ClassVar[str] = "min_max"
-    _minimum: Optional[np.ndarray]
-    _maximum: Optional[np.ndarray]
+    def __post_init__(self) -> None:
+        if self.minimum is not None:
+            self.minimum = np.asarray(self.minimum)
+        if self.maximum is not None:
+            self.maximum = np.asarray(self.maximum)
+        self._torch_minimum: Optional[torch.Tensor] = None
+        self._torch_maximum: Optional[torch.Tensor] = None
 
-    def __init__(
+    def fit_with_transition_picker(
         self,
-        dataset: Optional[MDPDataset] = None,
-        maximum: Optional[np.ndarray] = None,
-        minimum: Optional[np.ndarray] = None,
-    ):
-        self._minimum = None
-        self._maximum = None
-        if dataset:
-            transitions = []
-            for episode in dataset.episodes:
-                transitions += episode.transitions
-            self.fit(transitions)
-        elif maximum is not None and minimum is not None:
-            self._minimum = np.asarray(minimum)
-            self._maximum = np.asarray(maximum)
-
-    def fit(self, transitions: List[Transition]) -> None:
-        if self._minimum is not None and self._maximum is not None:
-            return
+        episodes: Sequence[EpisodeBase],
+        transition_picker: TransitionPickerProtocol,
+    ) -> None:
+        assert not self.built
+        minimum = np.zeros(episodes[0].action_signature.shape[0])
+        maximum = np.zeros(episodes[0].action_signature.shape[0])
+        for i, episode in enumerate(episodes):
+            for j in range(episode.transition_count):
+                transition = transition_picker(episode, j)
+                if i == 0 and j == 0:
+                    minimum = transition.action
+                    maximum = transition.action
+                else:
+                    minimum = np.minimum(minimum, transition.action)
+                    maximum = np.maximum(maximum, transition.action)
+        self.minimum = minimum
+        self.maximum = maximum
 
-        for i, transition in enumerate(transitions):
-            action = np.asarray(transition.action)
+    def fit_with_trajectory_slicer(
+        self,
+        episodes: Sequence[EpisodeBase],
+        trajectory_slicer: TrajectorySlicerProtocol,
+    ) -> None:
+        assert not self.built
+        minimum = np.zeros(episodes[0].action_signature.shape[0])
+        maximum = np.zeros(episodes[0].action_signature.shape[0])
+        for i, episode in enumerate(episodes):
+            traj = trajectory_slicer(
+                episode, episode.size() - 1, episode.size()
+            )
+            actions = np.asarray(traj.actions)
+            min_action = np.min(actions, axis=0)
+            max_action = np.max(actions, axis=0)
             if i == 0:
-                minimum = action
-                maximum = action
+                minimum = min_action
+                maximum = max_action
             else:
-                minimum = np.minimum(minimum, action)
-                maximum = np.maximum(maximum, action)
-
-        self._minimum = minimum.reshape((1,) + minimum.shape)
-        self._maximum = maximum.reshape((1,) + maximum.shape)
-
-    def fit_with_env(self, env: gym.Env) -> None:
-        if self._minimum is not None and self._maximum is not None:
-            return
+                minimum = np.minimum(minimum, min_action)
+                maximum = np.maximum(maximum, max_action)
+        self.minimum = minimum
+        self.maximum = maximum
 
+    def fit_with_env(self, env: gym.Env[Any, Any]) -> None:
+        assert not self.built
         assert isinstance(env.action_space, gym.spaces.Box)
-        shape = env.action_space.shape
         low = np.asarray(env.action_space.low)
         high = np.asarray(env.action_space.high)
-        self._minimum = low.reshape((1,) + shape)
-        self._maximum = high.reshape((1,) + shape)
+        self.minimum = low
+        self.maximum = high
 
-    def transform(self, action: torch.Tensor) -> torch.Tensor:
-        assert self._minimum is not None and self._maximum is not None
-        minimum = torch.tensor(
-            self._minimum, dtype=torch.float32, device=action.device
-        )
-        maximum = torch.tensor(
-            self._maximum, dtype=torch.float32, device=action.device
+    def transform(self, x: torch.Tensor) -> torch.Tensor:
+        assert self.built
+        if self._torch_minimum is None or self._torch_maximum is None:
+            self._set_torch_value(x.device)
+        assert (
+            self._torch_minimum is not None and self._torch_maximum is not None
         )
+        minimum = add_leading_dims(self._torch_minimum, target=x)
+        maximum = add_leading_dims(self._torch_maximum, target=x)
         # transform action into [-1.0, 1.0]
-        return ((action - minimum) / (maximum - minimum)) * 2.0 - 1.0
+        return ((x - minimum) / (maximum - minimum)) * 2.0 - 1.0
 
-    def reverse_transform(self, action: torch.Tensor) -> torch.Tensor:
-        assert self._minimum is not None and self._maximum is not None
-        minimum = torch.tensor(
-            self._minimum, dtype=torch.float32, device=action.device
-        )
-        maximum = torch.tensor(
-            self._maximum, dtype=torch.float32, device=action.device
+    def reverse_transform(self, x: torch.Tensor) -> torch.Tensor:
+        assert self.built
+        if self._torch_minimum is None or self._torch_maximum is None:
+            self._set_torch_value(x.device)
+        assert (
+            self._torch_minimum is not None and self._torch_maximum is not None
         )
+        minimum = add_leading_dims(self._torch_minimum, target=x)
+        maximum = add_leading_dims(self._torch_maximum, target=x)
         # transform action from [-1.0, 1.0]
-        return ((maximum - minimum) * ((action + 1.0) / 2.0)) + minimum
-
-    def reverse_transform_numpy(self, action: np.ndarray) -> np.ndarray:
-        assert self._minimum is not None and self._maximum is not None
-        minimum, maximum = self._minimum, self._maximum
-        # transform action from [-1.0, 1.0]
-        return ((maximum - minimum) * ((action + 1.0) / 2.0)) + minimum
-
-    def get_params(self, deep: bool = False) -> Dict[str, Any]:
-        if self._minimum is not None:
-            minimum = self._minimum.copy() if deep else self._minimum
-        else:
-            minimum = None
-
-        if self._maximum is not None:
-            maximum = self._maximum.copy() if deep else self._maximum
-        else:
-            maximum = None
+        return ((maximum - minimum) * ((x + 1.0) / 2.0)) + minimum
 
-        return {"minimum": minimum, "maximum": maximum}
-
-
-ACTION_SCALER_LIST: Dict[str, Type[ActionScaler]] = {}
-
-
-def register_action_scaler(cls: Type[ActionScaler]) -> None:
-    """Registers action scaler class.
-
-    Args:
-        cls: action scaler class inheriting ``ActionScaler``.
-
-    """
-    is_registered = cls.TYPE in ACTION_SCALER_LIST
-    assert not is_registered, f"{cls.TYPE} seems to be already registered"
-    ACTION_SCALER_LIST[cls.TYPE] = cls
+    def transform_numpy(self, x: np.ndarray) -> np.ndarray:
+        assert self.built
+        assert self.maximum is not None and self.minimum is not None
+        minimum = add_leading_dims_numpy(self.minimum, target=x)
+        maximum = add_leading_dims_numpy(self.maximum, target=x)
+        # transform action into [-1.0, 1.0]
+        return ((x - minimum) / (maximum - minimum)) * 2.0 - 1.0
 
+    def reverse_transform_numpy(self, x: np.ndarray) -> np.ndarray:
+        assert self.built
+        assert self.maximum is not None and self.minimum is not None
+        minimum = add_leading_dims_numpy(self.minimum, target=x)
+        maximum = add_leading_dims_numpy(self.maximum, target=x)
+        # transform action from [-1.0, 1.0]
+        return ((maximum - minimum) * ((x + 1.0) / 2.0)) + minimum
 
-def create_action_scaler(name: str, **kwargs: Any) -> ActionScaler:
-    """Returns registered action scaler object.
+    def _set_torch_value(self, device: torch.device) -> None:
+        self._torch_minimum = torch.tensor(
+            self.minimum, dtype=torch.float32, device=device
+        )
+        self._torch_maximum = torch.tensor(
+            self.maximum, dtype=torch.float32, device=device
+        )
 
-    Args:
-        name: regsitered scaler type name.
-        kwargs: scaler arguments.
+    @staticmethod
+    def get_type() -> str:
+        return "min_max"
+
+    @property
+    def built(self) -> bool:
+        return self.minimum is not None and self.maximum is not None
 
-    Returns:
-        scaler object.
 
-    """
-    assert name in ACTION_SCALER_LIST, f"{name} seems not to be registered."
-    scaler = ACTION_SCALER_LIST[name](**kwargs)
-    assert isinstance(scaler, ActionScaler)
-    return scaler
+(
+    register_action_scaler,
+    make_action_scaler_field,
+) = generate_optional_config_generation(
+    ActionScaler  # type: ignore
+)
 
 
 register_action_scaler(MinMaxActionScaler)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/preprocessing/reward_scalers.py` & `d3rlpy-2.0.2/d3rlpy/preprocessing/reward_scalers.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,516 +1,501 @@
-from typing import Any, ClassVar, Dict, List, Optional, Type
+import dataclasses
+from typing import Any, Optional, Sequence
 
 import gym
 import numpy as np
 import torch
 
-from ..dataset import MDPDataset, Transition
-from ..decorators import pretty_repr
-from ..logger import LOG
-
-
-@pretty_repr
-class RewardScaler:
-
-    TYPE: ClassVar[str] = "none"
-
-    def fit(self, transitions: List[Transition]) -> None:
-        """Estimates scaling parameters from dataset.
-
-        Args:
-            transitions: list of transitions.
-
-        """
-        raise NotImplementedError
-
-    def fit_with_env(self, env: gym.Env) -> None:
-        """Gets scaling parameters from environment.
-
-        Note:
-            ``RewardScaler`` does not support fitting with environment.
-
-        Args:
-            env: gym environment.
-
-        """
-        raise NotImplementedError("Please initialize with dataset.")
-
-    def transform(self, reward: torch.Tensor) -> torch.Tensor:
-        """Returns processed rewards.
-
-        Args:
-            reward: reward.
-
-        Returns:
-            processed reward.
-
-        """
-        raise NotImplementedError
-
-    def reverse_transform(self, reward: torch.Tensor) -> torch.Tensor:
-        """Returns reversely processed rewards.
-
-        Args:
-            reward: reward.
-
-        Returns:
-            reversely processed reward.
-
-        """
-        raise NotImplementedError
-
-    def transform_numpy(self, reward: np.ndarray) -> np.ndarray:
-        """Returns transformed rewards in numpy array.
-
-        Args:
-            reward: reward.
-
-        Returns:
-            transformed reward.
-
-        """
-        raise NotImplementedError
-
-    def get_type(self) -> str:
-        """Returns a scaler type.
-
-        Returns:
-            scaler type.
-
-        """
-        return self.TYPE
-
-    def get_params(self, deep: bool = False) -> Dict[str, Any]:
-        """Returns scaling parameters.
-
-        Args:
-            deep: flag to deeply copy objects.
-
-        Returns:
-            scaler parameters.
-
-        """
-        raise NotImplementedError
+from ..dataset import (
+    EpisodeBase,
+    TrajectorySlicerProtocol,
+    TransitionPickerProtocol,
+)
+from ..serializable_config import generate_optional_config_generation
+from .base import Scaler
+
+__all__ = [
+    "RewardScaler",
+    "MultiplyRewardScaler",
+    "ClipRewardScaler",
+    "MinMaxRewardScaler",
+    "StandardRewardScaler",
+    "ReturnBasedRewardScaler",
+    "ConstantShiftRewardScaler",
+    "register_reward_scaler",
+    "make_reward_scaler_field",
+]
+
+
+class RewardScaler(Scaler):
+    def fit_with_env(self, env: gym.Env[Any, Any]) -> None:
+        pass
 
 
+@dataclasses.dataclass()
 class MultiplyRewardScaler(RewardScaler):
     r"""Multiplication reward preprocessing.
 
     This preprocessor multiplies rewards by a constant number.
 
     .. code-block:: python
 
         from d3rlpy.preprocessing import MultiplyRewardScaler
+        from d3rlpy.algos import CQLConfig
 
         # multiply rewards by 10
         reward_scaler = MultiplyRewardScaler(10.0)
-
-        cql = CQL(reward_scaler=reward_scaler)
+        cql = CQLConfig(reward_scaler=reward_scaler).create()
 
     Args:
-        multiplier (float): constant multiplication value.
-
+        multiplier (float): Constant multiplication value.
     """
+    multiplier: float = 1.0
 
-    TYPE: ClassVar[str] = "multiply"
-    _multiplier: Optional[float]
+    def fit_with_transition_picker(
+        self,
+        episodes: Sequence[EpisodeBase],
+        transition_picker: TransitionPickerProtocol,
+    ) -> None:
+        pass
+
+    def fit_with_trajectory_slicer(
+        self,
+        episodes: Sequence[EpisodeBase],
+        trajectory_slicer: TrajectorySlicerProtocol,
+    ) -> None:
+        pass
 
-    def __init__(self, multiplier: Optional[float] = None):
-        self._multiplier = multiplier
+    def transform(self, x: torch.Tensor) -> torch.Tensor:
+        return self.multiplier * x
 
-    def fit(self, transitions: List[Transition]) -> None:
-        if self._multiplier is None:
-            LOG.warning("Please initialize MultiplyRewardScaler manually.")
+    def reverse_transform(self, x: torch.Tensor) -> torch.Tensor:
+        return x / self.multiplier
 
-    def transform(self, reward: torch.Tensor) -> torch.Tensor:
-        return self._multiplier * reward
+    def transform_numpy(self, x: np.ndarray) -> np.ndarray:
+        return self.multiplier * x
 
-    def reverse_transform(self, reward: torch.Tensor) -> torch.Tensor:
-        return reward / self._multiplier
+    def reverse_transform_numpy(self, x: np.ndarray) -> np.ndarray:
+        return x / self.multiplier
 
-    def transform_numpy(self, reward: np.ndarray) -> np.ndarray:
-        return self._multiplier * reward
+    @staticmethod
+    def get_type() -> str:
+        return "multiply"
 
-    def get_params(self, deep: bool = False) -> Dict[str, Any]:
-        return {"multiplier": self._multiplier}
+    @property
+    def built(self) -> bool:
+        return True
 
 
+@dataclasses.dataclass()
 class ClipRewardScaler(RewardScaler):
     r"""Reward clipping preprocessing.
 
     .. code-block:: python
 
         from d3rlpy.preprocessing import ClipRewardScaler
+        from d3rlpy.algos import CQLConfig
 
         # clip rewards within [-1.0, 1.0]
         reward_scaler = ClipRewardScaler(low=-1.0, high=1.0)
-
-        cql = CQL(reward_scaler=reward_scaler)
+        cql = CQLConfig(reward_scaler=reward_scaler).create()
 
     Args:
-        low (float): minimum value to clip.
-        high (float): maximum value to clip.
-        multiplier (float): constant multiplication value.
-
+        low (Optional[float]): Minimum value to clip.
+        high (Optional[float]): Maximum value to clip.
+        multiplier (float): Constant multiplication value.
     """
+    low: Optional[float] = None
+    high: Optional[float] = None
+    multiplier: float = 1.0
 
-    TYPE: ClassVar[str] = "clip"
-    _low: Optional[float]
-    _high: Optional[float]
-    _multiplier: float
-
-    def __init__(
-        self,
-        low: Optional[float] = None,
-        high: Optional[float] = None,
-        multiplier: float = 1.0,
-    ):
-        self._low = low
-        self._high = high
-        self._multiplier = multiplier
-
-    def fit(self, transitions: List[Transition]) -> None:
-        if self._low is None and self._high is None:
-            LOG.warning("Please initialize ClipRewardScaler manually.")
-
-    def transform(self, reward: torch.Tensor) -> torch.Tensor:
-        return self._multiplier * reward.clamp(self._low, self._high)
-
-    def reverse_transform(self, reward: torch.Tensor) -> torch.Tensor:
-        return reward / self._multiplier
-
-    def transform_numpy(self, reward: np.ndarray) -> np.ndarray:
-        return self._multiplier * np.clip(reward, self._low, self._high)
-
-    def get_params(self, deep: bool = False) -> Dict[str, Any]:
-        return {
-            "low": self._low,
-            "high": self._high,
-            "multiplier": self._multiplier,
-        }
+    def fit_with_transition_picker(
+        self,
+        episodes: Sequence[EpisodeBase],
+        transition_picker: TransitionPickerProtocol,
+    ) -> None:
+        pass
 
+    def fit_with_trajectory_slicer(
+        self,
+        episodes: Sequence[EpisodeBase],
+        trajectory_slicer: TrajectorySlicerProtocol,
+    ) -> None:
+        pass
 
-class MinMaxRewardScaler(RewardScaler):
-    r"""Min-Max reward normalization preprocessing.
+    def transform(self, x: torch.Tensor) -> torch.Tensor:
+        return self.multiplier * x.clamp(self.low, self.high)
 
-    .. math::
+    def reverse_transform(self, x: torch.Tensor) -> torch.Tensor:
+        return x / self.multiplier
 
-        r' = (r - \min(r)) / (\max(r) - \min(r))
+    def transform_numpy(self, x: np.ndarray) -> np.ndarray:
+        return self.multiplier * np.clip(x, self.low, self.high)
 
-    .. code-block:: python
+    def reverse_transform_numpy(self, x: np.ndarray) -> np.ndarray:
+        return x / self.multiplier
+
+    @staticmethod
+    def get_type() -> str:
+        return "clip"
+
+    @property
+    def built(self) -> bool:
+        return True
 
-        from d3rlpy.algos import CQL
 
-        cql = CQL(reward_scaler="min_max")
+@dataclasses.dataclass()
+class MinMaxRewardScaler(RewardScaler):
+    r"""Min-Max reward normalization preprocessing.
+
+    Rewards will be normalized in range ``[0.0, 1.0]``.
 
-    You can also initialize with :class:`d3rlpy.dataset.MDPDataset` object or
-    manually.
+    .. math::
+
+        r' = (r - \min(r)) / (\max(r) - \min(r))
 
     .. code-block:: python
 
         from d3rlpy.preprocessing import MinMaxRewardScaler
+        from d3rlpy.algos import CQLConfig
 
-        # initialize with dataset
-        scaler = MinMaxRewardScaler(dataset)
+        # normalize based on datasets
+        cql = CQLConfig(reward_scaler=MinMaxRewardScaler()).create()
 
         # initialize manually
-        scaler = MinMaxRewardScaler(minimum=0.0, maximum=10.0)
-
-        cql = CQL(scaler=scaler)
+        reward_scaler = MinMaxRewardScaler(minimum=0.0, maximum=10.0)
+        cql = CQLConfig(reward_scaler=reward_scaler).create()
 
     Args:
-        dataset (d3rlpy.dataset.MDPDataset): dataset object.
-        minimum (float): minimum value.
-        maximum (float): maximum value.
-        multiplier (float): constant multiplication value.
-
+        minimum (float): Minimum value.
+        maximum (float): Maximum value.
+        multiplier (float): Constant multiplication value.
     """
-    TYPE: ClassVar[str] = "min_max"
-    _minimum: Optional[float]
-    _maximum: Optional[float]
-    _multiplier: float
-
-    def __init__(
-        self,
-        dataset: Optional[MDPDataset] = None,
-        minimum: Optional[float] = None,
-        maximum: Optional[float] = None,
-        multiplier: float = 1.0,
-    ):
-        self._minimum = None
-        self._maximum = None
-        self._multiplier = multiplier
-        if dataset:
-            transitions = []
-            for episode in dataset.episodes:
-                transitions += episode.transitions
-            self.fit(transitions)
-        elif minimum is not None and maximum is not None:
-            self._minimum = minimum
-            self._maximum = maximum
-
-    def fit(self, transitions: List[Transition]) -> None:
-        if self._minimum is not None and self._maximum is not None:
-            return
-
-        rewards = [transition.reward for transition in transitions]
-
-        self._minimum = float(np.min(rewards))
-        self._maximum = float(np.max(rewards))
-
-    def transform(self, reward: torch.Tensor) -> torch.Tensor:
-        assert self._minimum is not None and self._maximum is not None
-        base = self._maximum - self._minimum
-        return self._multiplier * (reward - self._minimum) / base
-
-    def reverse_transform(self, reward: torch.Tensor) -> torch.Tensor:
-        assert self._minimum is not None and self._maximum is not None
-        base = self._maximum - self._minimum
-        return reward * base / self._multiplier + self._minimum
-
-    def transform_numpy(self, reward: np.ndarray) -> np.ndarray:
-        assert self._minimum is not None and self._maximum is not None
-        base = self._maximum - self._minimum
-        return self._multiplier * (reward - self._minimum) / base
-
-    def get_params(self, deep: bool = False) -> Dict[str, Any]:
-        return {
-            "minimum": self._minimum,
-            "maximum": self._maximum,
-            "multiplier": self._multiplier,
-        }
+    minimum: Optional[float] = None
+    maximum: Optional[float] = None
+    multiplier: float = 1.0
+
+    def fit_with_transition_picker(
+        self,
+        episodes: Sequence[EpisodeBase],
+        transition_picker: TransitionPickerProtocol,
+    ) -> None:
+        assert not self.built
+        rewards = []
+        for episode in episodes:
+            for i in range(episode.transition_count):
+                transition = transition_picker(episode, i)
+                rewards.append(transition.reward)
+        self.minimum = float(np.min(rewards))
+        self.maximum = float(np.max(rewards))
+
+    def fit_with_trajectory_slicer(
+        self,
+        episodes: Sequence[EpisodeBase],
+        trajectory_slicer: TrajectorySlicerProtocol,
+    ) -> None:
+        assert not self.built
+        rewards = [
+            trajectory_slicer(
+                episode, episode.size() - 1, episode.size()
+            ).rewards
+            for episode in episodes
+        ]
+        self.minimum = float(np.min(rewards))
+        self.maximum = float(np.max(rewards))
+
+    def transform(self, x: torch.Tensor) -> torch.Tensor:
+        assert self.built
+        assert self.maximum is not None and self.minimum is not None
+        base = self.maximum - self.minimum
+        return self.multiplier * (x - self.minimum) / base
+
+    def reverse_transform(self, x: torch.Tensor) -> torch.Tensor:
+        assert self.built
+        assert self.maximum is not None and self.minimum is not None
+        base = self.maximum - self.minimum
+        return x * base / self.multiplier + self.minimum
+
+    def transform_numpy(self, x: np.ndarray) -> np.ndarray:
+        assert self.built
+        assert self.maximum is not None and self.minimum is not None
+        base = self.maximum - self.minimum
+        return self.multiplier * (x - self.minimum) / base
+
+    def reverse_transform_numpy(self, x: np.ndarray) -> np.ndarray:
+        assert self.built
+        assert self.maximum is not None and self.minimum is not None
+        base = self.maximum - self.minimum
+        return x * base / self.multiplier + self.minimum
+
+    @staticmethod
+    def get_type() -> str:
+        return "min_max"
+
+    @property
+    def built(self) -> bool:
+        return self.minimum is not None and self.maximum is not None
 
 
+@dataclasses.dataclass()
 class StandardRewardScaler(RewardScaler):
     r"""Reward standardization preprocessing.
 
     .. math::
 
         r' = (r - \mu) / \sigma
 
     .. code-block:: python
 
-        from d3rlpy.algos import CQL
-
-        cql = CQL(reward_scaler="standard")
-
-    You can also initialize with :class:`d3rlpy.dataset.MDPDataset` object or
-    manually.
-
-    .. code-block:: python
-
         from d3rlpy.preprocessing import StandardRewardScaler
+        from d3rlpy.algos import CQLConfig
 
-        # initialize with dataset
-        scaler = StandardRewardScaler(dataset)
+        # normalize based on datasets
+        cql = CQLConfig(reward_scaler=StandardRewardScaler()).create()
 
         # initialize manually
-        scaler = StandardRewardScaler(mean=0.0, std=1.0)
-
-        cql = CQL(scaler=scaler)
+        reward_scaler = StandardRewardScaler(mean=0.0, std=1.0)
+        cql = CQLConfig(reward_scaler=reward_scaler).create()
 
     Args:
-        dataset (d3rlpy.dataset.MDPDataset): dataset object.
-        mean (float): mean value.
-        std (float): standard deviation value.
-        eps (float): constant value to avoid zero-division.
-        multiplier (float): constant multiplication value
-
+        mean (float): Mean value.
+        std (float): Standard deviation value.
+        eps (float): Constant value to avoid zero-division.
+        multiplier (float): Constant multiplication value
     """
-    TYPE: ClassVar[str] = "standard"
-    _mean: Optional[float]
-    _std: Optional[float]
-    _eps: float
-    _multiplier: float
-
-    def __init__(
-        self,
-        dataset: Optional[MDPDataset] = None,
-        mean: Optional[float] = None,
-        std: Optional[float] = None,
-        eps: float = 1e-3,
-        multiplier: float = 1.0,
-    ):
-        self._mean = None
-        self._std = None
-        self._eps = eps
-        self._multiplier = multiplier
-        if dataset:
-            transitions = []
-            for episode in dataset.episodes:
-                transitions += episode.transitions
-            self.fit(transitions)
-        elif mean is not None and std is not None:
-            self._mean = mean
-            self._std = std
-
-    def fit(self, transitions: List[Transition]) -> None:
-        if self._mean is not None and self._std is not None:
-            return
-
-        rewards = [transition.reward for transition in transitions]
-
-        self._mean = float(np.mean(rewards))
-        self._std = float(np.std(rewards))
-
-    def transform(self, reward: torch.Tensor) -> torch.Tensor:
-        assert self._mean is not None and self._std is not None
-        nonzero_std = self._std + self._eps
-        return self._multiplier * (reward - self._mean) / nonzero_std
-
-    def reverse_transform(self, reward: torch.Tensor) -> torch.Tensor:
-        assert self._mean is not None and self._std is not None
-        return reward * (self._std + self._eps) / self._multiplier + self._mean
-
-    def transform_numpy(self, reward: np.ndarray) -> np.ndarray:
-        assert self._mean is not None and self._std is not None
-        nonzero_std = self._std + self._eps
-        return self._multiplier * (reward - self._mean) / nonzero_std
-
-    def get_params(self, deep: bool = False) -> Dict[str, Any]:
-        return {
-            "mean": self._mean,
-            "std": self._std,
-            "eps": self._eps,
-            "multiplier": self._multiplier,
-        }
+    mean: Optional[float] = None
+    std: Optional[float] = None
+    eps: float = 1e-3
+    multiplier: float = 1.0
+
+    def fit_with_transition_picker(
+        self,
+        episodes: Sequence[EpisodeBase],
+        transition_picker: TransitionPickerProtocol,
+    ) -> None:
+        assert not self.built
+        rewards = []
+        for episode in episodes:
+            for i in range(episode.transition_count):
+                transition = transition_picker(episode, i)
+                rewards.append(transition.reward)
+        self.mean = float(np.mean(rewards))
+        self.std = float(np.std(rewards))
+
+    def fit_with_trajectory_slicer(
+        self,
+        episodes: Sequence[EpisodeBase],
+        trajectory_slicer: TrajectorySlicerProtocol,
+    ) -> None:
+        assert not self.built
+        rewards = [
+            trajectory_slicer(
+                episode, episode.size() - 1, episode.size()
+            ).rewards
+            for episode in episodes
+        ]
+        self.mean = float(np.mean(rewards))
+        self.std = float(np.std(rewards))
+
+    def transform(self, x: torch.Tensor) -> torch.Tensor:
+        assert self.built
+        assert self.mean is not None and self.std is not None
+        nonzero_std = self.std + self.eps
+        return self.multiplier * (x - self.mean) / nonzero_std
+
+    def reverse_transform(self, x: torch.Tensor) -> torch.Tensor:
+        assert self.built
+        assert self.mean is not None and self.std is not None
+        return x * (self.std + self.eps) / self.multiplier + self.mean
+
+    def transform_numpy(self, x: np.ndarray) -> np.ndarray:
+        assert self.built
+        assert self.mean is not None and self.std is not None
+        nonzero_std = self.std + self.eps
+        return self.multiplier * (x - self.mean) / nonzero_std
+
+    def reverse_transform_numpy(self, x: np.ndarray) -> np.ndarray:
+        assert self.built
+        assert self.mean is not None and self.std is not None
+        return x * (self.std + self.eps) / self.multiplier + self.mean
+
+    @staticmethod
+    def get_type() -> str:
+        return "standard"
+
+    @property
+    def built(self) -> bool:
+        return self.mean is not None and self.std is not None
 
 
+@dataclasses.dataclass()
 class ReturnBasedRewardScaler(RewardScaler):
     r"""Reward normalization preprocessing based on return scale.
 
     .. math::
 
         r' = r / (R_{max} - R_{min})
 
     .. code-block:: python
 
-        from d3rlpy.algos import CQL
-
-        cql = CQL(reward_scaler="return")
-
-    You can also initialize with :class:`d3rlpy.dataset.MDPDataset` object or
-    manually.
-
-    .. code-block:: python
-
         from d3rlpy.preprocessing import ReturnBasedRewardScaler
+        from d3rlpy.algos import CQLConfig
 
-        # initialize with dataset
-        scaler = ReturnBasedRewardScaler(dataset)
+        # normalize based on datasets
+        cql = CQLConfig(reward_scaler=ReturnBasedRewardScaler()).create()
 
         # initialize manually
-        scaler = ReturnBasedRewardScaler(return_max=100.0, return_min=1.0)
-
-        cql = CQL(scaler=scaler)
+        reward_scaler = ReturnBasedRewardScaler(
+            return_max=100.0,
+            return_min=1.0,
+        )
+        cql = CQLConfig(reward_scaler=reward_scaler).create()
 
     References:
         * `Kostrikov et al., Offline Reinforcement Learning with Implicit
           Q-Learning. <https://arxiv.org/abs/2110.06169>`_
 
     Args:
-        dataset (d3rlpy.dataset.MDPDataset): dataset object.
-        return_max (float): the maximum return value.
-        return_min (float): standard deviation value.
-        multiplier (float): constant multiplication value
-
+        return_max (float): Maximum return value.
+        return_min (float): Standard deviation value.
+        multiplier (float): Constant multiplication value
     """
-    TYPE: ClassVar[str] = "return"
-    _return_max: Optional[float]
-    _return_min: Optional[float]
-    _multiplier: float
-
-    def __init__(
-        self,
-        dataset: Optional[MDPDataset] = None,
-        return_max: Optional[float] = None,
-        return_min: Optional[float] = None,
-        multiplier: float = 1.0,
-    ):
-        self._return_max = None
-        self._return_min = None
-        self._multiplier = multiplier
-        if dataset:
-            transitions = []
-            for episode in dataset.episodes:
-                transitions += episode.transitions
-            self.fit(transitions)
-        elif return_max is not None and return_min is not None:
-            self._return_max = return_max
-            self._return_min = return_min
-
-    def fit(self, transitions: List[Transition]) -> None:
-        if self._return_max is not None and self._return_min is not None:
-            return
-
-        # collect start states
-        start_transitions = set()
-        for transition in transitions:
-            # trace back to the start state
-            curr_transition = transition
-            while curr_transition.prev_transition:
-                curr_transition = curr_transition.prev_transition
-            start_transitions.add(curr_transition)
+    return_max: Optional[float] = None
+    return_min: Optional[float] = None
+    multiplier: float = 1.0
 
-        # accumulate all rewards
+    def fit_with_transition_picker(
+        self,
+        episodes: Sequence[EpisodeBase],
+        transition_picker: TransitionPickerProtocol,
+    ) -> None:
+        assert not self.built
+        returns = []
+        for episode in episodes:
+            rewards = []
+            for i in range(episode.transition_count):
+                transition = transition_picker(episode, i)
+                rewards.append(transition.reward)
+            returns.append(float(np.sum(rewards)))
+        self.return_max = float(np.max(returns))
+        self.return_min = float(np.min(returns))
+
+    def fit_with_trajectory_slicer(
+        self,
+        episodes: Sequence[EpisodeBase],
+        trajectory_slicer: TrajectorySlicerProtocol,
+    ) -> None:
+        assert not self.built
         returns = []
-        for start_transition in start_transitions:
-            ret = 0.0
-            curr_transition = start_transition
-            while True:
-                ret += curr_transition.reward
-                if curr_transition.next_transition is None:
-                    break
-                curr_transition = curr_transition.next_transition
-            returns.append(ret)
-
-        self._return_max = float(np.max(returns))
-        self._return_min = float(np.min(returns))
-
-    def transform(self, reward: torch.Tensor) -> torch.Tensor:
-        assert self._return_max is not None and self._return_min is not None
-        return self._multiplier * reward / (self._return_max - self._return_min)
-
-    def reverse_transform(self, reward: torch.Tensor) -> torch.Tensor:
-        assert self._return_max is not None and self._return_min is not None
-        return reward * (self._return_max + self._return_min) / self._multiplier
-
-    def transform_numpy(self, reward: np.ndarray) -> np.ndarray:
-        assert self._return_max is not None and self._return_min is not None
-        return self._multiplier * reward / (self._return_max - self._return_min)
-
-    def get_params(self, deep: bool = False) -> Dict[str, Any]:
-        return {
-            "return_max": self._return_max,
-            "return_min": self._return_min,
-            "multiplier": self._multiplier,
-        }
+        for episode in episodes:
+            traj = trajectory_slicer(
+                episode, episode.size() - 1, episode.size()
+            )
+            returns.append(float(np.sum(traj.rewards)))
+        self.return_max = float(np.max(returns))
+        self.return_min = float(np.min(returns))
+
+    def transform(self, x: torch.Tensor) -> torch.Tensor:
+        assert self.built
+        assert self.return_min is not None and self.return_max is not None
+        return self.multiplier * x / (self.return_max - self.return_min)
+
+    def reverse_transform(self, x: torch.Tensor) -> torch.Tensor:
+        assert self.built
+        assert self.return_min is not None and self.return_max is not None
+        return x * (self.return_max - self.return_min) / self.multiplier
+
+    def transform_numpy(self, x: np.ndarray) -> np.ndarray:
+        assert self.built
+        assert self.return_min is not None and self.return_max is not None
+        return self.multiplier * x / (self.return_max - self.return_min)
+
+    def reverse_transform_numpy(self, x: np.ndarray) -> np.ndarray:
+        assert self.built
+        assert self.return_min is not None and self.return_max is not None
+        return x * (self.return_max - self.return_min) / self.multiplier
+
+    @staticmethod
+    def get_type() -> str:
+        return "return"
+
+    @property
+    def built(self) -> bool:
+        return self.return_max is not None and self.return_min is not None
+
+
+@dataclasses.dataclass()
+class ConstantShiftRewardScaler(RewardScaler):
+    r"""Reward shift preprocessing.
 
+    .. math::
 
-REWARD_SCALER_LIST: Dict[str, Type[RewardScaler]] = {}
+        r' = r + c
 
+    You need to initialize manually.
 
-def register_reward_scaler(cls: Type[RewardScaler]) -> None:
-    """Registers reward scaler class.
+    .. code-block:: python
 
-    Args:
-        cls: scaler class inheriting ``RewardScaler``.
+        from d3rlpy.preprocessing import ConstantShiftRewardScaler
+        from d3rlpy.algos import CQLConfig
 
+        reward_scaler = ConstantShiftRewardScaler(shift=-1.0)
+        cql = CQLConfig(reward_scaler=reward_scaler).create()
+
+    References:
+        * `Kostrikov et al., Offline Reinforcement Learning with Implicit
+          Q-Learning. <https://arxiv.org/abs/2110.06169>`_
+
+    Args:
+        shift (float): Constant shift value
     """
-    is_registered = cls.TYPE in REWARD_SCALER_LIST
-    assert not is_registered, f"{cls.TYPE} seems to be already registered"
-    REWARD_SCALER_LIST[cls.TYPE] = cls
+    shift: float
 
+    def fit_with_transition_picker(
+        self,
+        episodes: Sequence[EpisodeBase],
+        transition_picker: TransitionPickerProtocol,
+    ) -> None:
+        pass
 
-def create_reward_scaler(name: str, **kwargs: Any) -> RewardScaler:
-    assert name in REWARD_SCALER_LIST, f"{name} seems not to be registered."
-    reward_scaler = REWARD_SCALER_LIST[name](**kwargs)
-    assert isinstance(reward_scaler, RewardScaler)
-    return reward_scaler
+    def fit_with_trajectory_slicer(
+        self,
+        episodes: Sequence[EpisodeBase],
+        trajectory_slicer: TrajectorySlicerProtocol,
+    ) -> None:
+        pass
+
+    def transform(self, x: torch.Tensor) -> torch.Tensor:
+        return self.shift + x
+
+    def reverse_transform(self, x: torch.Tensor) -> torch.Tensor:
+        return x - self.shift
+
+    def transform_numpy(self, x: np.ndarray) -> np.ndarray:
+        return self.shift + x
+
+    def reverse_transform_numpy(self, x: np.ndarray) -> np.ndarray:
+        return x - self.shift
+
+    @staticmethod
+    def get_type() -> str:
+        return "shift"
+
+    @property
+    def built(self) -> bool:
+        return True
+
+
+(
+    register_reward_scaler,
+    make_reward_scaler_field,
+) = generate_optional_config_generation(
+    RewardScaler  # type: ignore
+)
 
 
 register_reward_scaler(MultiplyRewardScaler)
 register_reward_scaler(ClipRewardScaler)
 register_reward_scaler(MinMaxRewardScaler)
 register_reward_scaler(StandardRewardScaler)
 register_reward_scaler(ReturnBasedRewardScaler)
+register_reward_scaler(ConstantShiftRewardScaler)
```

### Comparing `d3rlpy-1.1.1/d3rlpy/torch_utility.py` & `d3rlpy-2.0.2/d3rlpy/torch_utility.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,54 @@
 import collections
-from inspect import signature
-from typing import Any, Callable, Dict, List, Optional, Sequence, Union
+import dataclasses
+from typing import Any, Dict, List, Optional, Sequence, TypeVar, Union
 
 import numpy as np
 import torch
 from torch import nn
 from torch.optim import Optimizer
-from torch.utils.data._utils.collate import default_collate
-from typing_extensions import Protocol
 
-from .dataset import TransitionMiniBatch
-from .preprocessing import ActionScaler, RewardScaler, Scaler
+from .dataset import TrajectoryMiniBatch, TransitionMiniBatch
+from .preprocessing import ActionScaler, ObservationScaler, RewardScaler
 
-BLACK_LIST = [
+__all__ = [
+    "soft_sync",
+    "hard_sync",
+    "sync_optimizer_state",
+    "set_eval_mode",
+    "set_train_mode",
+    "to_cuda",
+    "to_cpu",
+    "to_device",
+    "freeze",
+    "unfreeze",
+    "get_state_dict",
+    "set_state_dict",
+    "reset_optimizer_states",
+    "map_location",
+    "TorchMiniBatch",
+    "TorchTrajectoryMiniBatch",
+    "convert_to_torch",
+    "convert_to_torch_recursively",
+    "eval_api",
+    "train_api",
+    "View",
+]
+
+
+IGNORE_LIST = [
     "policy",
     "q_function",
     "policy_optim",
     "q_function_optim",
 ]  # special properties
 
 
 def _get_attributes(obj: Any) -> List[str]:
-    return [key for key in dir(obj) if key not in BLACK_LIST]
+    return [key for key in dir(obj) if key not in IGNORE_LIST]
 
 
 def soft_sync(targ_model: nn.Module, model: nn.Module, tau: float) -> None:
     with torch.no_grad():
         params = model.parameters()
         targ_params = targ_model.parameters()
         for p, p_targ in zip(params, targ_params):
@@ -74,14 +97,21 @@
 def to_cpu(impl: Any) -> None:
     for key in _get_attributes(impl):
         module = getattr(impl, key)
         if isinstance(module, (torch.nn.Module, torch.nn.Parameter)):
             module.cpu()
 
 
+def to_device(impl: Any, device: str) -> None:
+    if device.startswith("cuda"):
+        to_cuda(impl, device)
+    else:
+        to_cpu(impl)
+
+
 def freeze(impl: Any) -> None:
     for key in _get_attributes(impl):
         module = getattr(impl, key)
         if isinstance(module, torch.nn.Module):
             for p in module.parameters():
                 p.requires_grad = False
 
@@ -121,206 +151,162 @@
     if "cuda" in device:
         return lambda storage, loc: storage.cuda(device)
     if "cpu" in device:
         return "cpu"
     raise ValueError(f"invalid device={device}")
 
 
-class _WithDeviceAndScalerProtocol(Protocol):
-    @property
-    def device(self) -> str:
-        ...
-
-    @property
-    def scaler(self) -> Optional[Scaler]:
-        ...
-
-    @property
-    def action_scaler(self) -> Optional[ActionScaler]:
-        ...
-
-    @property
-    def reward_scaler(self) -> Optional[RewardScaler]:
-        ...
-
-
-def _convert_to_torch(array: np.ndarray, device: str) -> torch.Tensor:
+def convert_to_torch(array: np.ndarray, device: str) -> torch.Tensor:
     dtype = torch.uint8 if array.dtype == np.uint8 else torch.float32
     tensor = torch.tensor(data=array, dtype=dtype, device=device)
     return tensor.float()
 
 
-class TorchMiniBatch:
+def convert_to_torch_recursively(
+    array: Union[np.ndarray, Sequence[np.ndarray]], device: str
+) -> Union[torch.Tensor, Sequence[torch.Tensor]]:
+    if isinstance(array, (list, tuple)):
+        return [convert_to_torch(data, device) for data in array]
+    elif isinstance(array, np.ndarray):
+        return convert_to_torch(array, device)
+    else:
+        raise ValueError(f"invalid array type: {type(array)}")
 
-    _observations: torch.Tensor
-    _actions: torch.Tensor
-    _rewards: torch.Tensor
-    _next_observations: torch.Tensor
-    _terminals: torch.Tensor
-    _n_steps: torch.Tensor
-    _device: str
 
-    def __init__(
-        self,
+@dataclasses.dataclass(frozen=True)
+class TorchMiniBatch:
+    observations: torch.Tensor
+    actions: torch.Tensor
+    rewards: torch.Tensor
+    next_observations: torch.Tensor
+    terminals: torch.Tensor
+    intervals: torch.Tensor
+    device: str
+    numpy_batch: Optional[TransitionMiniBatch] = None
+
+    @classmethod
+    def from_batch(
+        cls,
         batch: TransitionMiniBatch,
         device: str,
-        scaler: Optional[Scaler] = None,
+        observation_scaler: Optional[ObservationScaler] = None,
+        action_scaler: Optional[ActionScaler] = None,
+        reward_scaler: Optional[RewardScaler] = None,
+    ) -> "TorchMiniBatch":
+        # convert numpy array to torch tensor
+        observations = convert_to_torch_recursively(batch.observations, device)
+        actions = convert_to_torch(batch.actions, device)
+        rewards = convert_to_torch(batch.rewards, device)
+        next_observations = convert_to_torch_recursively(
+            batch.next_observations, device
+        )
+        terminals = convert_to_torch(batch.terminals, device)
+        intervals = convert_to_torch(batch.intervals, device)
+
+        # TODO: support tuple observation
+        assert isinstance(observations, torch.Tensor)
+        assert isinstance(next_observations, torch.Tensor)
+
+        # apply scaler
+        if observation_scaler:
+            observations = observation_scaler.transform(observations)
+            next_observations = observation_scaler.transform(next_observations)
+        if action_scaler:
+            actions = action_scaler.transform(actions)
+        if reward_scaler:
+            rewards = reward_scaler.transform(rewards)
+
+        return TorchMiniBatch(
+            observations=observations,
+            actions=actions,
+            rewards=rewards,
+            next_observations=next_observations,
+            terminals=terminals,
+            intervals=intervals,
+            device=device,
+            numpy_batch=batch,
+        )
+
+
+@dataclasses.dataclass(frozen=True)
+class TorchTrajectoryMiniBatch:
+    observations: torch.Tensor  # (B, L, ...)
+    actions: torch.Tensor  # (B, L, ...)
+    rewards: torch.Tensor  # (B, L, 1)
+    returns_to_go: torch.Tensor  # (B, L, 1)
+    terminals: torch.Tensor  # (B, L, 1)
+    timesteps: torch.Tensor  # (B, L, 1)
+    masks: torch.Tensor  # (B, L)
+    device: str
+    numpy_batch: Optional[TrajectoryMiniBatch] = None
+
+    @classmethod
+    def from_batch(
+        cls,
+        batch: TrajectoryMiniBatch,
+        device: str,
+        observation_scaler: Optional[ObservationScaler] = None,
         action_scaler: Optional[ActionScaler] = None,
         reward_scaler: Optional[RewardScaler] = None,
-    ):
+    ) -> "TorchTrajectoryMiniBatch":
         # convert numpy array to torch tensor
-        observations = _convert_to_torch(batch.observations, device)
-        actions = _convert_to_torch(batch.actions, device)
-        rewards = _convert_to_torch(batch.rewards, device)
-        next_observations = _convert_to_torch(batch.next_observations, device)
-        terminals = _convert_to_torch(batch.terminals, device)
-        n_steps = _convert_to_torch(batch.n_steps, device)
+        observations = convert_to_torch_recursively(batch.observations, device)
+        actions = convert_to_torch(batch.actions, device)
+        rewards = convert_to_torch(batch.rewards, device)
+        returns_to_go = convert_to_torch(batch.returns_to_go, device)
+        terminals = convert_to_torch(batch.terminals, device)
+        timesteps = convert_to_torch(batch.timesteps, device).long()
+        masks = convert_to_torch(batch.masks, device)
+
+        # TODO: support tuple observation
+        assert isinstance(observations, torch.Tensor)
 
         # apply scaler
-        if scaler:
-            observations = scaler.transform(observations)
-            next_observations = scaler.transform(next_observations)
+        if observation_scaler:
+            observations = observation_scaler.transform(observations)
         if action_scaler:
             actions = action_scaler.transform(actions)
         if reward_scaler:
             rewards = reward_scaler.transform(rewards)
+            # NOTE: some operations might be incompatible with returns
+            returns_to_go = reward_scaler.transform(returns_to_go)
 
-        self._observations = observations
-        self._actions = actions
-        self._rewards = rewards
-        self._next_observations = next_observations
-        self._terminals = terminals
-        self._n_steps = n_steps
-        self._device = device
-
-    @property
-    def observations(self) -> torch.Tensor:
-        return self._observations
-
-    @property
-    def actions(self) -> torch.Tensor:
-        return self._actions
-
-    @property
-    def rewards(self) -> torch.Tensor:
-        return self._rewards
-
-    @property
-    def next_observations(self) -> torch.Tensor:
-        return self._next_observations
-
-    @property
-    def terminals(self) -> torch.Tensor:
-        return self._terminals
-
-    @property
-    def n_steps(self) -> torch.Tensor:
-        return self._n_steps
-
-    @property
-    def device(self) -> str:
-        return self._device
-
-
-def torch_api(
-    scaler_targets: Optional[List[str]] = None,
-    action_scaler_targets: Optional[List[str]] = None,
-    reward_scaler_targets: Optional[List[str]] = None,
-) -> Callable[..., np.ndarray]:
-    def _torch_api(f: Callable[..., np.ndarray]) -> Callable[..., np.ndarray]:
-        # get argument names
-        sig = signature(f)
-        arg_keys = list(sig.parameters.keys())[1:]
-
-        def wrapper(
-            self: _WithDeviceAndScalerProtocol, *args: Any, **kwargs: Any
-        ) -> np.ndarray:
-            tensors: List[Union[torch.Tensor, TorchMiniBatch]] = []
-
-            # convert all args to torch.Tensor
-            for i, val in enumerate(args):
-                tensor: Union[torch.Tensor, TorchMiniBatch]
-                if isinstance(val, torch.Tensor):
-                    tensor = val
-                elif isinstance(val, list):
-                    tensor = default_collate(val)
-                    tensor = tensor.to(self.device)
-                elif isinstance(val, np.ndarray):
-                    if val.dtype == np.uint8:
-                        dtype = torch.uint8
-                    else:
-                        dtype = torch.float32
-                    tensor = torch.tensor(
-                        data=val,
-                        dtype=dtype,
-                        device=self.device,
-                    )
-                elif val is None:
-                    tensor = None
-                elif isinstance(val, TransitionMiniBatch):
-                    tensor = TorchMiniBatch(
-                        val,
-                        self.device,
-                        scaler=self.scaler,
-                        action_scaler=self.action_scaler,
-                        reward_scaler=self.reward_scaler,
-                    )
-                else:
-                    tensor = torch.tensor(
-                        data=val,
-                        dtype=torch.float32,
-                        device=self.device,
-                    )
-
-                if isinstance(tensor, torch.Tensor):
-                    # preprocess
-                    if self.scaler and scaler_targets:
-                        if arg_keys[i] in scaler_targets:
-                            tensor = self.scaler.transform(tensor)
-
-                    # preprocess action
-                    if self.action_scaler and action_scaler_targets:
-                        if arg_keys[i] in action_scaler_targets:
-                            tensor = self.action_scaler.transform(tensor)
-
-                    # preprocessing reward
-                    if self.reward_scaler and reward_scaler_targets:
-                        if arg_keys[i] in reward_scaler_targets:
-                            tensor = self.reward_scaler.transform(tensor)
-
-                    # make sure if the tensor is float32 type
-                    if tensor is not None and tensor.dtype != torch.float32:
-                        tensor = tensor.float()
-
-                tensors.append(tensor)
-            return f(self, *tensors, **kwargs)
+        return TorchTrajectoryMiniBatch(
+            observations=observations,
+            actions=actions,
+            rewards=rewards,
+            returns_to_go=returns_to_go,
+            terminals=terminals,
+            timesteps=timesteps,
+            masks=masks,
+            device=device,
+            numpy_batch=batch,
+        )
 
-        return wrapper
 
-    return _torch_api
+TCallable = TypeVar("TCallable")
 
 
-def eval_api(f: Callable[..., np.ndarray]) -> Callable[..., np.ndarray]:
-    def wrapper(self: Any, *args: Any, **kwargs: Any) -> np.ndarray:
+def eval_api(f: TCallable) -> TCallable:
+    def wrapper(self: Any, *args: Any, **kwargs: Any) -> Any:
         set_eval_mode(self)
-        return f(self, *args, **kwargs)
+        return f(self, *args, **kwargs)  # type: ignore
 
-    return wrapper
+    return wrapper  # type: ignore
 
 
-def train_api(f: Callable[..., np.ndarray]) -> Callable[..., np.ndarray]:
-    def wrapper(self: Any, *args: Any, **kwargs: Any) -> np.ndarray:
+def train_api(f: TCallable) -> TCallable:
+    def wrapper(self: Any, *args: Any, **kwargs: Any) -> Any:
         set_train_mode(self)
-        return f(self, *args, **kwargs)
+        return f(self, *args, **kwargs)  # type: ignore
 
-    return wrapper
+    return wrapper  # type: ignore
 
 
 class View(nn.Module):  # type: ignore
-
     _shape: Sequence[int]
 
     def __init__(self, shape: Sequence[int]):
         super().__init__()
         self._shape = shape
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:
```

### Comparing `d3rlpy-1.1.1/d3rlpy.egg-info/PKG-INFO` & `d3rlpy-2.0.2/d3rlpy.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: d3rlpy
-Version: 1.1.1
+Version: 2.0.2
 Summary: An offline deep reinforcement learning library
 Home-page: https://github.com/takuseno/d3rlpy
 Author: Takuma Seno
 Author-email: takuma.seno@gmail.com
 License: MIT License
 Description: <p align="center"><img align="center" width="300px" src="assets/logo.png"></p>
         
@@ -22,46 +22,44 @@
         
         ```py
         import d3rlpy
         
         dataset, env = d3rlpy.datasets.get_dataset("hopper-medium-v0")
         
         # prepare algorithm
-        sac = d3rlpy.algos.SAC()
+        sac = d3rlpy.algos.SACConfig().create(device="cuda:0")
         
         # train offline
         sac.fit(dataset, n_steps=1000000)
         
         # train online
         sac.fit_online(env, n_steps=1000000)
         
         # ready to control
         actions = sac.predict(x)
         ```
         
         - Documentation: https://d3rlpy.readthedocs.io
         - Paper: https://arxiv.org/abs/2111.03788
         
-        ## key features
+        ## Key features
         
         ### :zap: Most Practical RL Library Ever
         - **offline RL**: d3rlpy supports state-of-the-art offline RL algorithms. Offline RL is extremely powerful when the online interaction is not feasible during training (e.g. robotics, medical).
         - **online RL**: d3rlpy also supports conventional state-of-the-art online training algorithms without any compromising, which means that you can solve any kinds of RL problems only with `d3rlpy`.
-        - **advanced engineering**: d3rlpy is designed to implement the faster and efficient training algorithms. For example, you can train Atari environments with x4 less memory space and as fast as the fastest RL library.
         
         ### :beginner: User-friendly API
         - **zero-knowledge of DL library**: d3rlpy provides many state-of-the-art algorithms through intuitive APIs. You can become a RL engineer even without knowing how to use deep learning libraries.
         - **extensive documentation**: d3rlpy is fully documented and accompanied with tutorials and reproduction scripts of the original papers.
         
         ### :rocket: Beyond State-of-the-art
         - **distributional Q function**: d3rlpy is the first library that supports distributional Q functions in the all algorithms. The distributional Q function is known as the very powerful method to achieve the state-of-the-performance.
-        - **many tweek options**: d3rlpy is also the first to support N-step TD backup and ensemble value functions in the all algorithms, which lead you to the place no one ever reached yet.
         
         
-        ## installation
+        ## Installation
         d3rlpy supports Linux, macOS and Windows.
         
         ### PyPI (recommended)
         [![PyPI version](https://badge.fury.io/py/d3rlpy.svg)](https://badge.fury.io/py/d3rlpy)
         ![PyPI - Downloads](https://img.shields.io/pypi/dm/d3rlpy)
         ```
         $ pip install d3rlpy
@@ -76,15 +74,15 @@
         
         ### Docker
         ![Docker Pulls](https://img.shields.io/docker/pulls/takuseno/d3rlpy)
         ```
         $ docker run -it --gpus all --name d3rlpy takuseno/d3rlpy:latest bash
         ```
         
-        ## supported algorithms
+        ## Supported algorithms
         | algorithm | discrete control | continuous control | offline RL? |
         |:-|:-:|:-:|:-:|
         | Behavior Cloning (supervised learning) | :white_check_mark: | :white_check_mark: | |
         | [Neural Fitted Q Iteration (NFQ)](https://link.springer.com/chapter/10.1007/11564096_32) | :white_check_mark: | :no_entry: | :white_check_mark: |
         | [Deep Q-Network (DQN)](https://www.nature.com/articles/nature14236) | :white_check_mark: | :no_entry: | |
         | [Double DQN](https://arxiv.org/abs/1509.06461) | :white_check_mark: | :no_entry: | |
         | [Deep Deterministic Policy Gradients (DDPG)](https://arxiv.org/abs/1509.02971) | :no_entry: | :white_check_mark: | |
@@ -94,157 +92,141 @@
         | [Bootstrapping Error Accumulation Reduction (BEAR)](https://arxiv.org/abs/1906.00949) | :no_entry: | :white_check_mark: | :white_check_mark: |
         | [Conservative Q-Learning (CQL)](https://arxiv.org/abs/2006.04779) | :white_check_mark: | :white_check_mark: | :white_check_mark: |
         | [Advantage Weighted Actor-Critic (AWAC)](https://arxiv.org/abs/2006.09359) | :no_entry: | :white_check_mark: | :white_check_mark: |
         | [Critic Reguralized Regression (CRR)](https://arxiv.org/abs/2006.15134) | :no_entry: | :white_check_mark: | :white_check_mark: |
         | [Policy in Latent Action Space (PLAS)](https://arxiv.org/abs/2011.07213) | :no_entry: | :white_check_mark: | :white_check_mark: |
         | [TD3+BC](https://arxiv.org/abs/2106.06860) | :no_entry: | :white_check_mark: | :white_check_mark: |
         | [Implicit Q-Learning (IQL)](https://arxiv.org/abs/2110.06169) | :no_entry: | :white_check_mark: | :white_check_mark: |
+        | [Decision Transformer](https://arxiv.org/abs/2106.01345) | :construction: | :white_check_mark: | :white_check_mark: |
         
-        ## supported Q functions
+        ## Supported Q functions
         - [x] standard Q function
         - [x] [Quantile Regression](https://arxiv.org/abs/1710.10044)
         - [x] [Implicit Quantile Network](https://arxiv.org/abs/1806.06923)
         
-        ## experimental features
-        - Model-based Algorithms
-          - [Model-based Offline Policy Optimization (MOPO)](https://arxiv.org/abs/2005.13239)
-          - [Conservative Offline Model-Based Policy Optimization (COMBO)](https://arxiv.org/abs/2102.08363)
-        - Q-functions
-          - [Fully parametrized Quantile Function](https://arxiv.org/abs/1911.02140) (experimental)
-        
-        ## benchmark results
+        ## Benchmark results
         d3rlpy is benchmarked to ensure the implementation quality.
         The benchmark scripts are available [reproductions](https://github.com/takuseno/d3rlpy/tree/master/reproductions) directory.
         The benchmark results are available [d3rlpy-benchmarks](https://github.com/takuseno/d3rlpy-benchmarks) repository.
         
-        ## examples
+        ## Examples
         ### MuJoCo
         <p align="center"><img align="center" width="160px" src="assets/mujoco_hopper.gif"></p>
         
         ```py
         import d3rlpy
         
         # prepare dataset
         dataset, env = d3rlpy.datasets.get_d4rl('hopper-medium-v0')
         
         # prepare algorithm
-        cql = d3rlpy.algos.CQL(use_gpu=True)
+        cql = d3rlpy.algos.CQLConfig().create(device='cuda:0')
         
         # train
         cql.fit(
             dataset,
-            eval_episodes=dataset,
-            n_epochs=100,
-            scorers={
-                'environment': d3rlpy.metrics.evaluate_on_environment(env),
-                'td_error': d3rlpy.metrics.td_error_scorer,
-            },
+            n_steps=100000,
+            evaluators={"environment": d3rlpy.metrics.EnvironmentEvaluator(env)},
         )
         ```
         
         See more datasets at [d4rl](https://github.com/rail-berkeley/d4rl).
         
         ### Atari 2600
         <p align="center"><img align="center" width="160px" src="assets/breakout.gif"></p>
         
         ```py
         import d3rlpy
-        from sklearn.model_selection import train_test_split
-        
-        # prepare dataset
-        dataset, env = d3rlpy.datasets.get_atari('breakout-expert-v0')
         
-        # split dataset
-        train_episodes, test_episodes = train_test_split(dataset, test_size=0.1)
+        # prepare dataset (1% dataset)
+        dataset, env = d3rlpy.datasets.get_atari_transitions(
+            'breakout',
+            fraction=0.01,
+            num_stack=4,
+        )
         
         # prepare algorithm
-        cql = d3rlpy.algos.DiscreteCQL(
-            n_frames=4,
-            q_func_factory='qr',
-            scaler='pixel',
-            use_gpu=True,
-        )
+        cql = d3rlpy.algos.DiscreteCQLConfig(
+            observation_scaler=d3rlpy.preprocessing.PixelObservationScaler(),
+            reward_scaler=d3rlpy.preprocessing.ClipRewardScaler(-1.0, 1.0),
+        ).create(device='cuda:0')
         
         # start training
         cql.fit(
-            train_episodes,
-            eval_episodes=test_episodes,
-            n_epochs=100,
-            scorers={
-                'environment': d3rlpy.metrics.evaluate_on_environment(env),
-                'td_error': d3rlpy.metrics.td_error_scorer,
-            },
+            dataset,
+            n_steps=1000000,
+            evaluators={"environment": d3rlpy.metrics.EnvironmentEvaluator(env, epsilon=0.001)},
         )
         ```
         
         See more Atari datasets at [d4rl-atari](https://github.com/takuseno/d4rl-atari).
         
         
         ### Online Training
         ```py
         import d3rlpy
         import gym
         
         # prepare environment
-        env = gym.make('HopperBulletEnv-v0')
-        eval_env = gym.make('HopperBulletEnv-v0')
+        env = gym.make('Hopper-v3')
+        eval_env = gym.make('Hopper-v3')
         
         # prepare algorithm
-        sac = d3rlpy.algos.SAC(use_gpu=True)
+        sac = d3rlpy.algos.SACConfig().create(device='cuda:0')
         
         # prepare replay buffer
-        buffer = d3rlpy.online.buffers.ReplayBuffer(maxlen=1000000, env=env)
+        buffer = d3rlpy.dataset.create_fifo_replay_buffer(limit=1000000, env=env)
         
         # start training
         sac.fit_online(env, buffer, n_steps=1000000, eval_env=eval_env)
         ```
         
-        ## tutorials
+        ## Tutorials
         Try cartpole examples on Google Colaboratory!
         
         - offline RL tutorial: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/takuseno/d3rlpy/blob/master/tutorials/cartpole.ipynb)
         - online RL tutorial: [![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/github/takuseno/d3rlpy/blob/master/tutorials/online.ipynb)
         
         More tutorial documentations are available [here](https://d3rlpy.readthedocs.io/en/stable/tutorials/index.html).
         
-        ## contributions
+        ## Contributions
         Any kind of contribution to d3rlpy would be highly appreciated!
         Please check the [contribution guide](CONTRIBUTING.md).
         
-        The release planning can be checked at [milestones](https://github.com/takuseno/d3rlpy/milestones).
-        
-        ## community
+        ## Community
         | Channel | Link |
         |:-|:-|
-        | Chat | [Gitter](https://gitter.im/d3rlpy/d3rlpy) |
         | Issues | [GitHub Issues](https://github.com/takuseno/d3rlpy/issues) |
         
-        ## family projects
+        ## Family projects
         | Project | Description |
         |:-:|:-|
-        | [d4rl-pybullet](https://github.com/takuseno/d4rl-pybullet) | An offline RL datasets of PyBullet tasks |
         | [d4rl-atari](https://github.com/takuseno/d4rl-atari) | A d4rl-style library of Google's Atari 2600 datasets |
-        | [MINERVA](https://github.com/takuseno/minerva) | An out-of-the-box GUI tool for offline RL |
         
-        ## roadmap
+        ## Roadmap
         The roadmap to the future release is available in [ROADMAP.md](ROADMAP.md).
         
-        ## citation
+        ## Citation
         The paper is available [here](https://arxiv.org/abs/2111.03788).
         ```
-        @InProceedings{seno2021d3rlpy,
-          author = {Takuma Seno, Michita Imai},
-          title = {d3rlpy: An Offline Deep Reinforcement Library},
-          booktitle = {NeurIPS 2021 Offline Reinforcement Learning Workshop},
-          month = {December},
-          year = {2021}
+        @article{d3rlpy,
+          author  = {Takuma Seno and Michita Imai},
+          title   = {d3rlpy: An Offline Deep Reinforcement Learning Library},
+          journal = {Journal of Machine Learning Research},
+          year    = {2022},
+          volume  = {23},
+          number  = {315},
+          pages   = {1--20},
+          url     = {http://jmlr.org/papers/v23/22-0017.html}
         }
         ```
         
-        ## acknowledgement
+        ## Acknowledgement
+        This work started as a part of [Takuma Seno](https://github.com/takuseno)'s Ph.D project at Keio University in 2020.
+        
         This work is supported by Information-technology Promotion Agency, Japan
         (IPA), Exploratory IT Human Resources Project (MITOU Program) in the fiscal
         year 2020.
         
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

