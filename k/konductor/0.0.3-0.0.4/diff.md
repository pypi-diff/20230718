# Comparing `tmp/konductor-0.0.3.tar.gz` & `tmp/konductor-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "konductor-0.0.3.tar", last modified: Sun May 21 04:53:33 2023, max compression
+gzip compressed data, was "konductor-0.0.4.tar", last modified: Tue Jul 18 05:07:11 2023, max compression
```

## Comparing `konductor-0.0.3.tar` & `konductor-0.0.4.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-21 04:53:24.000000 konductor-0.0.3/.dockerignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.805137 konductor-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-21 04:53:24.000000 konductor-0.0.3/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-21 04:53:24.000000 konductor-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-21 04:53:24.000000 konductor-0.0.3/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-21 04:53:24.000000 konductor-0.0.3/Dockerfile.pytorch
--rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-05-21 04:53:24.000000 konductor-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-05-21 04:53:33.817137 konductor-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-21 04:53:24.000000 konductor-0.0.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/docs/statistics.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/docs/trainer.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/docs/visualisation.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-21 04:53:24.000000 konductor-0.0.3/examples/kube-launch.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-21 04:53:24.000000 konductor-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 04:53:33.817137 konductor-0.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-21 04:53:24.000000 konductor-0.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.805137 konductor-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/src/konductor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/src/konductor/metadata/
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/src/konductor/metadata/checkpointer/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/checkpointer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/checkpointer/_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/checkpointer/_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/src/konductor/metadata/remotesync/
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/remotesync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/remotesync/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/remotesync/minio.py
--rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/remotesync/ssh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/metadata/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/statistics/perflogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/statistics/scalar_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     8378 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/metadata/statistics/statistic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/data/
--rw-r--r--   0 runner    (1001) docker     (123)     4324 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/data/_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/_pytorch/cityscapes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2899 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/_pytorch/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/_pytorch/mnist.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/data/_tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/_tensorflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/_tensorflow/dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/data/dali.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/init.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/losses/
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/losses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/losses/_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/losses/_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/losses/_pytorch/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/models/
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/models/_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/models/_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/models/_pytorch/encdec.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/models/_pytorch/torchvision.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/models/_tensorflow/
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/models/_tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)     1330 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/optimizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/optimizers/_pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/optimizers/_pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/optimizers/_pytorch/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/optimizers/_pytorch/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/optimizers/_pytorch/lamb.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/modules/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/modules/scheduler/_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.813137 konductor-0.0.3/src/konductor/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8715 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/trainer/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     4575 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/trainer/pbar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/trainer/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/trainer/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3806 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/trainer/trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/src/konductor/utilities/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/src/konductor/utilities/comm/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/utilities/comm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/utilities/comm/_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/utilities/comm/_tensorflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/utilities/metadata.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/utilities/onnx_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/src/konductor/webserver/
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/src/konductor/webserver/pages/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/pages/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/pages/experiment_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/pages/home.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/pages/simple_comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-21 04:53:24.000000 konductor-0.0.3/src/konductor/webserver/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.809137 konductor-0.0.3/src/konductor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-05-21 04:53:33.000000 konductor-0.0.3/src/konductor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-21 04:53:33.000000 konductor-0.0.3/src/konductor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 04:53:33.000000 konductor-0.0.3/src/konductor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-21 04:53:33.000000 konductor-0.0.3/src/konductor.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-21 04:53:33.000000 konductor-0.0.3/src/konductor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 04:53:33.000000 konductor-0.0.3/src/konductor.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/base.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/tests/config_init/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/config_init/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1143 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/config_init/test_pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/init_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/tests/remote/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/remote/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/remote/ssh_config
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/remote/test_remote.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/tests/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/statistics/test_checkpointer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/statistics/test_metamanager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/statistics/test_perflogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/statistics/test_statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/statistics/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/test_registry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/tests/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/trainer/test_pytorch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:33.817137 konductor-0.0.3/tests/webui/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/webui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-21 04:53:24.000000 konductor-0.0.3/tests/webui/test_tree.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.195876 konductor-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-18 05:07:02.000000 konductor-0.0.4/.dockerignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.179876 konductor-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.183876 konductor-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-18 05:07:02.000000 konductor-0.0.4/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-18 05:07:02.000000 konductor-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-07-18 05:07:02.000000 konductor-0.0.4/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-07-18 05:07:02.000000 konductor-0.0.4/Dockerfile.pytorch
+-rw-r--r--   0 runner    (1001) docker     (123)    11344 2023-07-18 05:07:02.000000 konductor-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-07-18 05:07:11.195876 konductor-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-07-18 05:07:02.000000 konductor-0.0.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.183876 konductor-0.0.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:02.000000 konductor-0.0.4/docs/statistics.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:02.000000 konductor-0.0.4/docs/trainer.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:02.000000 konductor-0.0.4/docs/visualisation.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.183876 konductor-0.0.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-18 05:07:02.000000 konductor-0.0.4/examples/kube-launch.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-18 05:07:02.000000 konductor-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 05:07:11.195876 konductor-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-18 05:07:02.000000 konductor-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.179876 konductor-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.183876 konductor-0.0.4/src/konductor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.187876 konductor-0.0.4/src/konductor/metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/metadata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.187876 konductor-0.0.4/src/konductor/metadata/checkpointer/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/metadata/checkpointer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/metadata/checkpointer/_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/metadata/checkpointer/_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5841 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/metadata/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.187876 konductor-0.0.4/src/konductor/metadata/remotesync/
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/metadata/remotesync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/metadata/remotesync/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5742 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/metadata/remotesync/minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10806 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/metadata/remotesync/ssh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.187876 konductor-0.0.4/src/konductor/metadata/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/metadata/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6447 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/metadata/statistics/perflogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/metadata/statistics/scalar_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8402 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/metadata/statistics/statistic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.187876 konductor-0.0.4/src/konductor/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.187876 konductor-0.0.4/src/konductor/modules/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.187876 konductor-0.0.4/src/konductor/modules/data/_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/data/_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/data/_pytorch/cityscapes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/data/_pytorch/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/data/_pytorch/mnist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.187876 konductor-0.0.4/src/konductor/modules/data/_tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/data/_tensorflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/data/_tensorflow/dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/data/dali.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3474 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/init.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.187876 konductor-0.0.4/src/konductor/modules/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/losses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.187876 konductor-0.0.4/src/konductor/modules/losses/_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/losses/_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/losses/_pytorch/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.191877 konductor-0.0.4/src/konductor/modules/models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.191877 konductor-0.0.4/src/konductor/modules/models/_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/models/_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1803 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/models/_pytorch/encdec.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/models/_pytorch/torchvision.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.191877 konductor-0.0.4/src/konductor/modules/models/_tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/models/_tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.191877 konductor-0.0.4/src/konductor/modules/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/optimizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.191877 konductor-0.0.4/src/konductor/modules/optimizers/_pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/optimizers/_pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/optimizers/_pytorch/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/optimizers/_pytorch/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5756 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/optimizers/_pytorch/lamb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3784 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.191877 konductor-0.0.4/src/konductor/modules/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/modules/scheduler/_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.191877 konductor-0.0.4/src/konductor/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8510 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/trainer/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/trainer/pbar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/trainer/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10251 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/trainer/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3803 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/trainer/trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.191877 konductor-0.0.4/src/konductor/utilities/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.191877 konductor-0.0.4/src/konductor/utilities/comm/
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/utilities/comm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8008 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/utilities/comm/_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3311 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/utilities/comm/_tensorflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/utilities/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/utilities/onnx_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.191877 konductor-0.0.4/src/konductor/webserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/webserver/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/webserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/webserver/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.191877 konductor-0.0.4/src/konductor/webserver/pages/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/webserver/pages/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4590 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/webserver/pages/experiment_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/webserver/pages/home.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/webserver/pages/simple_comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-07-18 05:07:02.000000 konductor-0.0.4/src/konductor/webserver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.187876 konductor-0.0.4/src/konductor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15612 2023-07-18 05:07:11.000000 konductor-0.0.4/src/konductor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-07-18 05:07:11.000000 konductor-0.0.4/src/konductor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 05:07:11.000000 konductor-0.0.4/src/konductor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-18 05:07:11.000000 konductor-0.0.4/src/konductor.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-18 05:07:11.000000 konductor-0.0.4/src/konductor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 05:07:11.000000 konductor-0.0.4/src/konductor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.195876 konductor-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/base.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.195876 konductor-0.0.4/tests/config_init/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/config_init/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1153 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/config_init/test_pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/init_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.195876 konductor-0.0.4/tests/remote/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/remote/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/remote/ssh_config
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/remote/test_remote.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.195876 konductor-0.0.4/tests/statistics/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/statistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/statistics/test_checkpointer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/statistics/test_metamanager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/statistics/test_perflogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/statistics/test_statistic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/statistics/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/test_registry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.195876 konductor-0.0.4/tests/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/trainer/test_pytorch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:11.195876 konductor-0.0.4/tests/webui/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/webui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-18 05:07:02.000000 konductor-0.0.4/tests/webui/test_tree.py
```

### Comparing `konductor-0.0.3/.dockerignore` & `konductor-0.0.4/.dockerignore`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/.github/workflows/publish-to-pypi.yml` & `konductor-0.0.4/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/.gitignore` & `konductor-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/Dockerfile.pytorch` & `konductor-0.0.4/Dockerfile.pytorch`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-FROM nvidia/cuda:12.0.1-devel-ubuntu22.04
+FROM nvidia/cuda:11.8.0-devel-ubuntu22.04
 
 # Basic Python Setup
 RUN apt update && apt install -y python3 python3-pip python3.10-venv git
 
 # Install Python Dependencies
 # Install PyTorch
 RUN pip3 install --index-url https://download.pytorch.org/whl/cu118 \
-    torch==2.0.0 torchvision==0.15.1 torchaudio==2.0.1 torchdata==0.6.0
+    torch==2.0.1 torchvision==0.15.2 torchaudio==2.0.2 torchdata==0.6.1
 
 # Install DALI
 RUN pip3 install --extra-index-url https://developer.download.nvidia.com/compute/redist \
-    nvidia-dali-cuda120==1.23.0
+    nvidia-dali-cuda110==1.27.0
 
 # Install other Python Packages
 RUN pip3 install \
     pyarrow==10.0.1 \
     paramiko==3.0.0 \
     minio==7.1.12 \
     pandas==1.3.5 \
```

### Comparing `konductor-0.0.3/LICENSE` & `konductor-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/PKG-INFO` & `konductor-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konductor
-Version: 0.0.3
+Version: 0.0.4
 Summary: Framework for training generic ml models
 Author-email: Bryce Ferenczi <frenzi@hotmail.com.au>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `konductor-0.0.3/README.rst` & `konductor-0.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/examples/kube-launch.yml` & `konductor-0.0.4/examples/kube-launch.yml`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/pyproject.toml` & `konductor-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/metadata/__init__.py` & `konductor-0.0.4/src/konductor/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/metadata/checkpointer/__init__.py` & `konductor-0.0.4/src/konductor/metadata/checkpointer/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/metadata/checkpointer/_pytorch.py` & `konductor-0.0.4/src/konductor/metadata/checkpointer/_pytorch.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/metadata/manager.py` & `konductor-0.0.4/src/konductor/metadata/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """
 
 """
 
 from datetime import datetime, timedelta
 from dataclasses import dataclass
-import os
 from pathlib import Path
 from typing import Any, Dict
 import subprocess
+from warnings import warn
+import os
 
 import yaml
 
 from .checkpointer import Checkpointer
 from .statistics.perflogger import PerfLogger
 from .remotesync import _RemoteSyncrhoniser
 from ..utilities import comm
@@ -84,14 +85,16 @@
         """Resume if available, pull from remote if necessary"""
         self._remote_resume()
         extras = self.checkpointer.resume()
         if extras is not None:
             self.epoch = extras["epoch"]
             self.iteration = extras["iteration"]
             self.perflog.set_iteration(self.iteration)
+        else:
+            warn("Unable to load epoch and iteration from checkpoint")
 
         return extras
 
     def _get_commit(self) -> str:
         try:
             git_hash = (
                 subprocess.check_output(
```

### Comparing `konductor-0.0.3/src/konductor/metadata/remotesync/__init__.py` & `konductor-0.0.4/src/konductor/metadata/remotesync/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/metadata/remotesync/_base.py` & `konductor-0.0.4/src/konductor/metadata/remotesync/_base.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/metadata/remotesync/minio.py` & `konductor-0.0.4/src/konductor/metadata/remotesync/minio.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/metadata/remotesync/ssh.py` & `konductor-0.0.4/src/konductor/metadata/remotesync/ssh.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/metadata/statistics/perflogger.py` & `konductor-0.0.4/src/konductor/metadata/statistics/perflogger.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/metadata/statistics/scalar_dict.py` & `konductor-0.0.4/src/konductor/metadata/statistics/scalar_dict.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/metadata/statistics/statistic.py` & `konductor-0.0.4/src/konductor/metadata/statistics/statistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     # How to sort each of the statistics in ascending order (worst to best)
     # i.e. if a smaller or larger value is better
     sort_fn: Dict[str, Callable[[float, float], bool]] = {}
 
     @classmethod
     def from_config(cls, buffer_length: int, writepath: Path, **kwargs):
-        return cls(buffer_length, writepath, **kwargs)
+        return cls(buffer_length=buffer_length, writepath=writepath, **kwargs)
 
     def __init__(
         self,
         buffer_length: int,
         writepath: Path,
         logger_name: str | None = None,
         reduce_batch: bool = True,
```

### Comparing `konductor-0.0.3/src/konductor/modules/__init__.py` & `konductor-0.0.4/src/konductor/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/modules/data/__init__.py` & `konductor-0.0.4/src/konductor/modules/data/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import abc
 import enum
 from dataclasses import dataclass, field
 import os
 from pathlib import Path
-from typing import Any, Dict, Sequence
+from typing import Any, Dict, List, Sequence
 
 from ..registry import Registry, BaseConfig
 from ..init import ModuleInitConfig, DatasetInitConfig, ExperimentInitConfig
 
 DATASET_REGISTRY = Registry("dataset")
 SAMPLER_REGISTRY = Registry("data_sampler")
 DATALOADER_REGISTRY = Registry("dataloder")
@@ -74,14 +74,15 @@
 
     dataset: DatasetConfig
     mode: Mode
     batch_size: int
     workers: int = 0
     shuffle: bool = False
     drop_last: bool = True
+    augmentations: List[ModuleInitConfig] = field(default_factory=lambda: [])
 
     @classmethod
     def from_config(cls, dataset: DatasetConfig, mode: Mode):
         match mode:
             case Mode.train:
                 loader_cfg = dataset.train_loader
             case Mode.val | Mode.test:
```

### Comparing `konductor-0.0.3/src/konductor/modules/data/_pytorch/cityscapes.py` & `konductor-0.0.4/src/konductor/modules/data/_pytorch/cityscapes.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/modules/data/_pytorch/dataloader.py` & `konductor-0.0.4/src/konductor/modules/data/_pytorch/dataloader.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,29 +1,33 @@
 from typing import Any, Callable, List, Type
-from warnings import warn
 from dataclasses import dataclass
 
 from ....utilities.comm import get_world_size, in_distributed_mode
-from .. import DataloaderConfig, DATALOADER_REGISTRY
+from .. import DataloaderConfig, DATALOADER_REGISTRY, Registry
 
 from torch.utils.data import (
     DataLoader,
     DistributedSampler,
     SequentialSampler,
     RandomSampler,
     Sampler,
     BatchSampler,
+    default_collate,
 )
 
+DATAPIPE_AUG = Registry("datapipe_augmentations")
+
 try:
+    from torchdata.datapipes.utils import pin_memory_fn
     from torchdata.datapipes.iter import IterableWrapper
     from torchdata.dataloader2 import DataLoader2
     from torchdata.dataloader2.reading_service import (
         MultiProcessingReadingService,
         DistributedReadingService,
+        SequentialReadingService,
     )
 except ImportError:
     print("torchdata unavailable")
 
 
 @dataclass
 @DATALOADER_REGISTRY.register_module("PYTORCH_V1")
@@ -72,24 +76,44 @@
 @DATALOADER_REGISTRY.register_module("PYTORCH_V2")
 class DataloaderV2Config(DataloaderConfig):
     """Uses DataPipe API
 
     :param DataloaderConfig: _description_
     """
 
+    pin_memory: bool = True
+
     def get_instance(self, *args, **kwargs):
         datapipe = IterableWrapper(self.dataset.get_instance(self.mode))
 
+        if self.shuffle:
+            datapipe = datapipe.shuffle()
+        if in_distributed_mode():
+            datapipe = datapipe.sharding_filter()
+
+        # if len(self.augmentations) > 0:
+        #     transforms = torch.nn.Sequential(
+        #         *list(DATAPIPE_AUG[aug.type](**aug.args) for aug in self.augmentations)
+        #     )
+        #     datapipe = datapipe.map(torch.jit.script(transforms))
+
+        for aug in self.augmentations:
+            datapipe = datapipe.map(DATAPIPE_AUG[aug.type](**aug.args))
+
+        datapipe = datapipe.batch(self.batch_size).map(default_collate)
+
+        if self.pin_memory:
+            datapipe = datapipe.map(pin_memory_fn)
+
         if self.workers > 0 and in_distributed_mode():
-            warn(
-                "Multiworker distributed is currently not supported"
-                "(waiting for torch2), defaulting to single worker"
+            rs = SequentialReadingService(
+                DistributedReadingService(),
+                MultiProcessingReadingService(num_workers=self.workers),
             )
-
-        if in_distributed_mode():
+        elif in_distributed_mode():
             rs = DistributedReadingService()
         elif self.workers > 0:
             rs = MultiProcessingReadingService(num_workers=self.workers)
         else:
             rs = None
 
         return DataLoader2(datapipe, reading_service=rs)
```

### Comparing `konductor-0.0.3/src/konductor/modules/data/dali.py` & `konductor-0.0.4/src/konductor/modules/data/dali.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,37 @@
 from dataclasses import dataclass
 
 import torch
 from nvidia.dali.plugin.pytorch import DALIGenericIterator
+from nvidia.dali.plugin.pytorch import LastBatchPolicy
 
-from . import DataloaderConfig, DATALOADER_REGISTRY, Mode
+from . import DataloaderConfig, DATALOADER_REGISTRY, Mode, Registry
 from ...utilities.comm import get_rank, get_world_size
 
+DALI_AUGMENTATIONS = Registry("DALI_AUGMENTATIONS")
+
 
 @dataclass
 @DATALOADER_REGISTRY.register_module("DALI")
 class DaliLoaderConfig(DataloaderConfig):
     def get_instance(self, *args):
         pipe_kwargs = {
             "shard_id": get_rank(),
             "num_shards": get_world_size(),
             "num_threads": max(self.workers, 1),
             "device_id": torch.cuda.current_device(),
             "batch_size": self.batch_size // get_world_size(),
+            "augmentations": self.augmentations,
         }
 
-        dali_pipe, out_map, reader_name = self.dataset.get_instance(
+        dali_pipe, out_map, reader_name, size = self.dataset.get_instance(
             mode=self.mode, random_shuffle=self.mode == Mode.train, **pipe_kwargs
         )
 
         return DALIGenericIterator(
-            dali_pipe, out_map, reader_name=reader_name, auto_reset=True
+            dali_pipe,
+            out_map,
+            reader_name=reader_name,
+            size=size,
+            auto_reset=True,
+            last_batch_policy=LastBatchPolicy.DROP,
         )
```

### Comparing `konductor-0.0.3/src/konductor/modules/init.py` & `konductor-0.0.4/src/konductor/modules/init.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,25 @@
     def from_yaml(cls, parsed_dict: Dict[str, Any]):
         dataset = ModuleInitConfig(parsed_dict["type"], parsed_dict["args"])
         if "loader" in parsed_dict:
             train_loader = val_loader = ModuleInitConfig(**parsed_dict["loader"])
         else:
             train_loader = ModuleInitConfig(**parsed_dict["train_loader"])
             val_loader = ModuleInitConfig(**parsed_dict["val_loader"])
+
+        # Transform augmentations to ModuleInitConfig
+        if "augmentations" in train_loader.args:
+            train_loader.args["augmentations"] = [
+                ModuleInitConfig(**aug) for aug in train_loader.args["augmentations"]
+            ]
+        if "augmentations" in val_loader.args:
+            val_loader.args["augmentations"] = [
+                ModuleInitConfig(**aug) for aug in val_loader.args["augmentations"]
+            ]
+
         return cls(dataset, train_loader, val_loader)
 
 
 @dataclass
 class ExperimentInitConfig:
     """
     Configuration for all the modules for training
```

### Comparing `konductor-0.0.3/src/konductor/modules/losses/__init__.py` & `konductor-0.0.4/src/konductor/modules/losses/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/modules/losses/_pytorch/base.py` & `konductor-0.0.4/src/konductor/modules/losses/_pytorch/base.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/modules/models/__init__.py` & `konductor-0.0.4/src/konductor/modules/models/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/modules/models/_pytorch/__init__.py` & `konductor-0.0.4/src/konductor/modules/models/_pytorch/__init__.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/modules/models/_pytorch/encdec.py` & `konductor-0.0.4/src/konductor/modules/models/_pytorch/encdec.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/modules/models/_pytorch/torchvision.py` & `konductor-0.0.4/src/konductor/modules/models/_pytorch/torchvision.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/modules/optimizers/__init__.py` & `konductor-0.0.4/src/konductor/modules/optimizers/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,35 @@
 import abc
+import inspect
 from dataclasses import dataclass
 from typing import Any
 
 from ..registry import Registry, BaseConfig
 from ..init import OptimizerInitConfig
 from ..scheduler import REGISTRY as SCHEDULER_REGISTRY, SchedulerConfig
 
 REGISTRY = Registry("optimizers")
 
 
 @dataclass
 class OptimizerConfig(BaseConfig):
     scheduler: SchedulerConfig
     lr: float
+    step_interval: int = 1
 
     @classmethod
     def from_config(cls, config: OptimizerInitConfig):
-        sched_cfg: SchedulerConfig = SCHEDULER_REGISTRY[
-            config.scheduler.type
-        ].from_config(config, **config.scheduler.args)
-        return cls(scheduler=sched_cfg, **config.args)
+        sched_cfg = SCHEDULER_REGISTRY[config.scheduler.type](**config.scheduler.args)
+        # TODO Maybe warn unused kwargs
+        filtered = {
+            k: v
+            for k, v in config.args.items()
+            if k in inspect.signature(cls).parameters
+        }
+        return cls(scheduler=sched_cfg, **filtered)
 
     @abc.abstractmethod
     def get_instance(self, model: Any) -> Any:
         raise NotImplementedError()
 
     def get_scheduler(self, optimizer: Any) -> Any:
         return self.scheduler.get_instance(optimizer)
```

### Comparing `konductor-0.0.3/src/konductor/modules/optimizers/_pytorch/base.py` & `konductor-0.0.4/src/konductor/modules/optimizers/_pytorch/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import itertools
 from typing import Any, Dict, Type, Iterator
 
 from torch import nn
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler, ReduceLROnPlateau
 
+from ...init import ModuleInitConfig
 from ...registry import Registry
 from ...optimizers import OptimizerConfig
 
 
 # Registry for custom parameter grouping functions
 PG_REGISTRY = Registry("param_group_fn")
 
@@ -60,25 +61,22 @@
     def _get_param_groups(model: nn.Module) -> Iterator[nn.Parameter]:
         return model.parameters()
 
     def _apply_extra(self, optim_cls: Type[Optimizer], model: nn.Module, **kwargs):
         optim_cls = self.maybe_add_gradient_clipping(optim_cls)
 
         if self.param_group_fn is not None:
-            pg_kwargs = dict(self.param_group_fn)  # make copy to modify
-            pg_fn = pg_kwargs.pop("type")
-            params = PG_REGISTRY[pg_fn](model, **pg_kwargs, **asdict(self))
+            pg = ModuleInitConfig(**self.param_group_fn)
+            params = PG_REGISTRY[pg.type](model, **pg.args, **asdict(self))
         else:
             params = model.parameters()
 
-        kwargs.update(**asdict(self))
-        for extra in ["scheduler", "gradient_clipping", "param_group_fn"]:
-            kwargs.pop(extra, None)
-
-        return optim_cls(params, **kwargs)
+        optim = self.init_auto_filter(optim_cls, params=params, **kwargs)
+        setattr(optim, "step_interval", self.step_interval)
+        return optim
 
     @abc.abstractmethod
     def get_instance(self, model: nn.Module) -> Optimizer:
         raise NotImplementedError()
 
     def get_scheduler(self, optimizer: Optimizer) -> _LRScheduler | ReduceLROnPlateau:
         return self.scheduler.get_instance(optimizer)
```

### Comparing `konductor-0.0.3/src/konductor/modules/optimizers/_pytorch/lamb.py` & `konductor-0.0.4/src/konductor/modules/optimizers/_pytorch/lamb.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/modules/registry.py` & `konductor-0.0.4/src/konductor/modules/registry.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 is that we can partially initialise and gather the relevant variables
 throughout the initialisation phase of the program. This allows for 
 circular dependices between classes such as the numebr of classes defined
 by a dataset can be used to configure the model 
 """
 
 import abc
-from dataclasses import dataclass
+from dataclasses import dataclass, asdict
 import inspect
 from logging import getLogger
 from typing import Any, Dict, Type
+from warnings import warn
 
 from .init import ExperimentInitConfig
 
 
 @dataclass
 class BaseConfig(metaclass=abc.ABCMeta):
     """
@@ -28,14 +29,27 @@
         """Run configuration stage of the module"""
         return cls(*args, **kwargs)
 
     @abc.abstractmethod
     def get_instance(self, *args, **kwargs) -> Any:
         """Get initialised module from configuration"""
 
+    def init_auto_filter(self, target, **kwargs) -> Dict[str, Any]:
+        """Make instance of target class with auto-filtered asdict(self) + kwargs"""
+        kwargs.update(asdict(self))
+        filtered = {
+            k: v for k, v in kwargs.items() if k in inspect.signature(target).parameters
+        }
+
+        diff = set(kwargs.keys()).difference(set(filtered.keys()))
+        if len(diff) > 0:
+            warn(f"Filtered unused arguments from {target.__name__}: {diff}")
+
+        return target(**filtered)
+
 
 class Registry:
     """
     Registry for modules to re-access by a given name.
     Names are case insensitive (all cast to lower).
     """
```

### Comparing `konductor-0.0.3/src/konductor/modules/scheduler/__init__.py` & `konductor-0.0.4/src/konductor/modules/scheduler/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,35 @@
 """
 Learning rate schedulers
 """
 from dataclasses import dataclass
-from typing import Any, NewType, Sequence
+from typing import Any, NewType
 
 from ..registry import Registry, BaseConfig
 from ..init import ModelInitConfig, ExperimentInitConfig
 
-SchedulerT = NewType("Scheduler", Sequence)
+SchedulerT = NewType("Scheduler", Any)
 OptimizerT = NewType("Optimizer", Any)
 
 REGISTRY = Registry("scheduler")
 
 
 @dataclass
 class SchedulerConfig(BaseConfig):
+    epoch_step: bool = True  # Scheduler is stepped at epoch, else at iteration
+
     @classmethod
     def from_config(cls, config: ExperimentInitConfig, *args, **kwargs):
         return super().from_config(config, *args, **kwargs)
 
-    def get_instance(self, optimizer: Any) -> SchedulerT:
-        raise NotImplementedError()
+    def get_instance(self, scheduler: SchedulerT, **kwargs):
+        """Add flag whether step is epoch based or iteration based"""
+        inst = self.init_auto_filter(scheduler, **kwargs)
+        setattr(inst, "epoch_step", self.epoch_step)
+        return inst
 
 
 try:
     import torch
 except ImportError:
     print("Unable to import torch, not using torch schedulers")
 else:
```

### Comparing `konductor-0.0.3/src/konductor/trainer/init.py` & `konductor-0.0.4/src/konductor/trainer/init.py`

 * *Files 5% similar despite different names*

```diff
@@ -146,22 +146,22 @@
     elif config_file is not None:
         with open(config_file, "r", encoding="utf-8") as conf_f:
             exp_cfg = yaml.safe_load(conf_f)
 
         train_hash = hash_from_config(exp_cfg)
         exp_path: Path = workspace / train_hash
 
-        if not exp_path.exists():
+        if not exp_path.exists() and comm.get_local_rank() == 0:
             print(f"Creating experiment directory {exp_path}")
             exp_path.mkdir(parents=True)
         else:
             print(f"Using experiment directory {exp_path}")
 
         # Ensure the experiment configuration exists in the target directory
-        if not (exp_path / "train_config.yml").exists():
+        if not (exp_path / "train_config.yml").exists() and comm.get_local_rank() == 0:
             with open(exp_path / "train_config.yml", "w", encoding="utf-8") as f:
                 yaml.safe_dump(exp_cfg, f)
 
     else:
         raise RuntimeError("Either --train_hash or --train_config are required")
 
     exp_cfg["work_dir"] = exp_path
@@ -264,21 +264,14 @@
     exp_config: ExperimentInitConfig,
     trainer_cls: Type[TrainerT],
     trainer_config: TrainerConfig,
     statistics: Dict[str, type[Statistic]],
     train_module_cls: Type[TrainerModules] = TrainerModules,
     perf_log_cfg_cls: Type[PerfLoggerConfig] = PerfLoggerConfig,
 ) -> TrainerT:
-    """Initialize training manager class + distributed setup"""
-    comm.initialize()  # Init distributed if required
-
-    # Making the big assumption that step interval is same for all optimizers
-    trainer_config.optimizer_interval = exp_config.model[0].optimizer.args.pop(
-        "step_interval", 1
-    )
-
+    """Initialize training manager class"""
     train_modules = init_training_modules(exp_config, train_module_cls)
     data_manager = init_data_manager(
         exp_config, train_modules, statistics, perf_log_cfg_cls
     )
 
     return trainer_cls(trainer_config, train_modules, data_manager)
```

### Comparing `konductor-0.0.3/src/konductor/trainer/pbar.py` & `konductor-0.0.4/src/konductor/trainer/pbar.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         f"{Fore.YELLOW}{Fore.RESET}{Fore.YELLOW}{Fore.RESET}"
         f"{Fore.GREEN}{Fore.YELLOW}{Fore.RED}{Fore.RESET}"
     )
 
     def __init__(
         self,
         total: int,
-        desc: str = "",
+        desc: str = "Running",
         ncols: int | None = None,
         frequency: float = 10,
         progress_style: List[str] | int | None = None,
     ) -> None:
         super().__init__()
         self.total = total
         self.ncols = ncols
@@ -106,15 +106,15 @@
                 start_str = f"{Fore.BLUE}{self._desc}: {Fore.GREEN}{self.n:0{n_digits}}{Fore.YELLOW}/{Fore.RED}{self.total}{Fore.RESET}"
             end_str = (
                 f"Elapsed: {Fore.YELLOW}{self.elapsed_str()}{Fore.RESET} "
                 f"Est: {Fore.YELLOW}{self.estimated_str()}{Fore.RESET}"
             )
 
             ncols = os.get_terminal_size().columns if self.ncols is None else self.ncols
-            print(" " * (ncols - 2), end="\r")  # Clear the terminal
+            print("\r" + " " * (ncols - 2), end="\r")  # Clear the terminal
             ncols -= len(start_str) + len(end_str) - self._fmt_len // 2
             done_bars = ncols * self.n // self.total
 
             bar_str = f"{Fore.GREEN}{'█'*done_bars}{Fore.YELLOW}{i}{Fore.RED}{'-'*(ncols - done_bars)}{Fore.RESET}"
 
             print(start_str, bar_str, end_str, end="\r")
```

### Comparing `konductor-0.0.3/src/konductor/trainer/profiler.py` & `konductor-0.0.4/src/konductor/trainer/profiler.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/trainer/pytorch.py` & `konductor-0.0.4/src/konductor/trainer/pytorch.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     amp: bool = False
     amp_kwargs: Dict[str, Any] | None = None
 
 
 def _amp_wrapper(func, amp_kwargs: Dict[str, Any] | None = None):
     if amp_kwargs is None:
         amp_kwargs = {"device_type": "cuda"}
-        print("Assuming cuda amp")
 
     def with_amp(*args, **kwargs):
         with autocast(**amp_kwargs):
             func(*args, **kwargs)
 
     return with_amp
 
@@ -109,15 +108,15 @@
         modules: PyTorchTrainerModules,
         data_manager: MetadataManager,
     ):
         # If AMP is enabled, wrap train and eval loops and add grad_scaler
         if config.amp:
             modules.grad_scaler = GradScaler()
             data_manager.checkpointer.add_checkpointable(
-                "grad_scaler", self.modules.grad_scaler
+                "grad_scaler", modules.grad_scaler
             )
             self._train = _amp_wrapper(self._train, config.amp_kwargs)
             self._validate = _amp_wrapper(self._validate, config.amp_kwargs)
 
         super().__init__(config, modules, data_manager)
 
         self.loss_monitor = config.loss_monitor
@@ -140,28 +139,51 @@
             self.loss_monitor(losses)
             all_loss = [
                 l
                 if self.modules.grad_scaler is None
                 else self.modules.grad_scaler.scale(l)
                 for l in losses.values()
             ]
-            all_loss = torch.stack(all_loss).sum() / self._config.optimizer_interval
+            all_loss = torch.stack(all_loss).sum()
             all_loss.backward()
 
+    def _maybe_step_scheduler(self, is_epoch: bool):
+        assert hasattr(self.modules.scheduler, "epoch_step"), (
+            "Scheduler needs 'epoch_step' attribute to "
+            "determine whether to step on iteration or epoch"
+        )
+        if self.modules.scheduler.epoch_step != is_epoch:
+            return
+
+        if isinstance(self.modules.scheduler, ReduceLROnPlateau):
+            if self.modules.scheduler.epoch_step == False:
+                self._logger.warn(
+                    "Reduce on plateau uses validation"
+                    "epoch loss for stepping by default"
+                )
+            self.modules.scheduler.step(self.data_manager.perflog.epoch_loss())
+        else:
+            self.modules.scheduler.step()
+
     def _maybe_step_optimiser(self, iter_: int) -> None:
         """Step optimizer if modulo the interval"""
+        assert hasattr(self.modules.optimizer, "step_interval"), (
+            "Optimizer needs 'step_interval' attribute to "
+            "determine the interval optimizer should be stepped"
+        )
         with record_function("optimizer"):
-            if iter_ % self._config.optimizer_interval == 0:
+            if iter_ % self.modules.optimizer.step_interval == 0:
                 if self.modules.grad_scaler is not None:
                     self.modules.grad_scaler.step(self.modules.optimizer)
                     self.modules.grad_scaler.update()
                 else:
                     self.modules.optimizer.step()
                 self.data_manager.iter_step()
                 self.modules.optimizer.zero_grad()
+                self._maybe_step_scheduler(is_epoch=False)
 
     @no_grad()
     def log_step(
         self,
         data: Dict[str, Tensor],
         preds: Dict[str, Tensor] | None,
         losses: Dict[str, Tensor] | None,
@@ -244,18 +266,15 @@
                 profiler.step()
                 if (
                     profiler.schedule(profiler.step_num)
                     == ProfilerAction.RECORD_AND_SAVE
                 ):
                     break
 
-        if isinstance(self.modules.scheduler, ReduceLROnPlateau):
-            self.modules.scheduler.step(self.data_manager.perflog.epoch_loss())
-        else:
-            self.modules.scheduler.step()
+        self._maybe_step_scheduler(is_epoch=True)
 
     def val_step(self, data) -> Tuple[Dict[str, Tensor] | None, Dict[str, Tensor]]:
         """
         Standard evaluation step, if you don't want to evaluate/track loss
         during evaluation, do not perform the calculation and return None
         in the loss part of the tuple.
         return:
```

### Comparing `konductor-0.0.3/src/konductor/trainer/trainer.py` & `konductor-0.0.4/src/konductor/trainer/trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 @dataclass
 class TrainerConfig:
     # Function to run for monitoring issues with the value
     # of the loss, does absolutely nothing by default
     loss_monitor: Callable[[Dict[str, Any]], None] = lambda x: None
 
     pbar: Callable | None = None  # Enable Console Progress
-    optimizer_interval: int = 1  # interval to call optimizer.step()
 
 
 class TrainingError(RuntimeError):
     """Exception raised by user in their training loop"""
 
 
 class BaseTrainer(ABC):
@@ -63,17 +62,19 @@
         extra = self.data_manager.resume()
         if extra is not None and "epoch" in extra:
             self._logger.info(f"Resuming from epoch {extra['epoch']}")
         else:
             self._logger.info(f"Unable to load checkpont, starting from scatch")
 
         if config.pbar is not None:
-            self._train = config.pbar(self._train, total=len(self.modules.trainloader))
+            self._train = config.pbar(
+                self._train, total=len(self.modules.trainloader), desc="Training"
+            )
             self._validate = config.pbar(
-                self._validate, total=len(self.modules.valloader)
+                self._validate, total=len(self.modules.valloader), desc="Validation"
             )
 
     def run_epoch(self) -> None:
         """Complete one epoch with training and validation epoch"""
         self._logger.info(f"Training epoch {self.data_manager.epoch}")
         self._train()
         self._logger.info(f"Validating epoch {self.data_manager.epoch}")
```

### Comparing `konductor-0.0.3/src/konductor/utilities/comm/_pytorch.py` & `konductor-0.0.4/src/konductor/utilities/comm/_pytorch.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/utilities/comm/_tensorflow.py` & `konductor-0.0.4/src/konductor/utilities/comm/_tensorflow.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/utilities/metadata.py` & `konductor-0.0.4/src/konductor/utilities/metadata.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/utilities/onnx_export.py` & `konductor-0.0.4/src/konductor/utilities/onnx_export.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/webserver/README.md` & `konductor-0.0.4/src/konductor/webserver/README.md`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/webserver/app.py` & `konductor-0.0.4/src/konductor/webserver/app.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/webserver/pages/experiment_summary.py` & `konductor-0.0.4/src/konductor/webserver/pages/experiment_summary.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/webserver/pages/simple_comparison.py` & `konductor-0.0.4/src/konductor/webserver/pages/simple_comparison.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor/webserver/utils.py` & `konductor-0.0.4/src/konductor/webserver/utils.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/src/konductor.egg-info/PKG-INFO` & `konductor-0.0.4/src/konductor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: konductor
-Version: 0.0.3
+Version: 0.0.4
 Summary: Framework for training generic ml models
 Author-email: Bryce Ferenczi <frenzi@hotmail.com.au>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `konductor-0.0.3/src/konductor.egg-info/SOURCES.txt` & `konductor-0.0.4/src/konductor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/tests/config_init/test_pytorch.py` & `konductor-0.0.4/tests/config_init/test_pytorch.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     return pgs
 
 
 def test_optim_param_groups(example_config: ExperimentInitConfig):
     lr_mult = 0.1
     example_config.model[0].optimizer.args["param_group_fn"] = {
         "type": "custom_pg",
-        "arg": lr_mult,
+        "args": {"arg": lr_mult},
     }
     _, optim, _ = get_training_model(example_config)
 
     pg1, pg2 = optim.param_groups
     assert np.allclose(pg1["lr"] / lr_mult, pg2["lr"])
```

### Comparing `konductor-0.0.3/tests/remote/test_remote.py` & `konductor-0.0.4/tests/remote/test_remote.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/tests/statistics/test_checkpointer.py` & `konductor-0.0.4/tests/statistics/test_checkpointer.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/tests/statistics/test_metamanager.py` & `konductor-0.0.4/tests/statistics/test_metamanager.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/tests/statistics/test_perflogger.py` & `konductor-0.0.4/tests/statistics/test_perflogger.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/tests/statistics/test_statistic.py` & `konductor-0.0.4/tests/statistics/test_statistic.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/tests/test_registry.py` & `konductor-0.0.4/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/tests/trainer/test_pytorch.py` & `konductor-0.0.4/tests/trainer/test_pytorch.py`

 * *Files identical despite different names*

### Comparing `konductor-0.0.3/tests/webui/test_tree.py` & `konductor-0.0.4/tests/webui/test_tree.py`

 * *Files identical despite different names*

