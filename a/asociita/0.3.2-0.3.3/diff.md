# Comparing `tmp/asociita-0.3.2.tar.gz` & `tmp/asociita-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "asociita-0.3.2.tar", max compression
+gzip compressed data, was "asociita-0.3.3.tar", max compression
```

## Comparing `asociita-0.3.2.tar` & `asociita-0.3.3.tar`

### file list

```diff
@@ -1,76 +1,78 @@
--rw-r--r--   0        0        0     1063 2023-05-29 08:30:33.477904 asociita-0.3.2/LICENSE
--rw-r--r--   0        0        0     2812 2023-05-29 08:30:33.477904 asociita-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-05-29 08:30:33.477904 asociita-0.3.2/asociita/__init__.py
--rw-r--r--   0        0        0     2725 2023-07-11 10:54:45.641955 asociita-0.3.2/asociita/components/archiver/__pycache__/archive_manager.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-07-11 10:54:39.082119 asociita-0.3.2/asociita/components/archiver/archive_manager.py
--rw-r--r--   0        0        0    10487 2023-06-28 14:35:28.652094 asociita-0.3.2/asociita/components/evaluator/__pycache__/evaluation_manager.cpython-310.pyc
--rw-r--r--   0        0        0     6307 2023-06-16 21:39:14.145401 asociita-0.3.2/asociita/components/evaluator/__pycache__/or_evaluator.cpython-310.pyc
--rw-r--r--   0        0        0    14784 2023-07-12 14:38:47.096029 asociita-0.3.2/asociita/components/evaluator/__pycache__/sample_evaluator.cpython-310.pyc
--rw-r--r--   0        0        0    15259 2023-06-22 18:08:42.554862 asociita-0.3.2/asociita/components/evaluator/evaluation_manager.py
--rw-r--r--   0        0        0    13324 2023-05-29 08:30:33.477904 asociita-0.3.2/asociita/components/evaluator/mr_evaluator.py
--rw-r--r--   0        0        0     9972 2023-06-16 21:38:55.086092 asociita-0.3.2/asociita/components/evaluator/or_evaluator.py
--rw-r--r--   0        0        0    18128 2023-07-04 14:39:59.993221 asociita-0.3.2/asociita/components/evaluator/sample_evaluator.py
--rw-r--r--   0        0        0     3999 2023-07-13 09:56:16.697717 asociita-0.3.2/asociita/components/nodes/__pycache__/federated_node.cpython-310.pyc
--rw-r--r--   0        0        0     4366 2023-07-13 09:56:12.917815 asociita-0.3.2/asociita/components/nodes/federated_node.py
--rw-r--r--   0        0        0     6319 2023-07-12 15:33:59.530733 asociita-0.3.2/asociita/components/orchestrator/__pycache__/evaluator_orchestrator.cpython-310.pyc
--rw-r--r--   0        0        0     5588 2023-07-13 09:26:40.219672 asociita-0.3.2/asociita/components/orchestrator/__pycache__/fedopt_orchestrator.cpython-310.pyc
--rw-r--r--   0        0        0     8999 2023-07-13 09:32:34.598465 asociita-0.3.2/asociita/components/orchestrator/__pycache__/generic_orchestrator.cpython-310.pyc
--rw-r--r--   0        0        0     8765 2023-07-13 09:24:20.995280 asociita-0.3.2/asociita/components/orchestrator/evaluator_orchestrator.py
--rw-r--r--   0        0        0     7373 2023-07-13 09:23:34.044495 asociita-0.3.2/asociita/components/orchestrator/fedopt_orchestrator.py
--rw-r--r--   0        0        0    11545 2023-07-13 09:32:16.910925 asociita-0.3.2/asociita/components/orchestrator/generic_orchestrator.py
--rw-r--r--   0        0        0     5098 2023-07-12 15:13:21.310949 asociita-0.3.2/asociita/components/settings/__pycache__/evaluator_settings.cpython-310.pyc
--rw-r--r--   0        0        0     4759 2023-07-12 14:39:39.170606 asociita-0.3.2/asociita/components/settings/__pycache__/fedopt_settings.cpython-310.pyc
--rw-r--r--   0        0        0     1663 2023-07-12 14:39:39.170606 asociita-0.3.2/asociita/components/settings/__pycache__/init_settings.cpython-310.pyc
--rw-r--r--   0        0        0    13715 2023-07-11 12:14:58.271395 asociita-0.3.2/asociita/components/settings/__pycache__/settings.cpython-310.pyc
--rw-r--r--   0        0        0     6901 2023-07-12 15:13:18.167030 asociita-0.3.2/asociita/components/settings/evaluator_settings.py
--rw-r--r--   0        0        0     5835 2023-07-12 14:39:37.466652 asociita-0.3.2/asociita/components/settings/fedopt_settings.py
--rw-r--r--   0        0        0     1931 2023-07-12 14:39:31.446817 asociita-0.3.2/asociita/components/settings/init_settings.py
--rw-r--r--   0        0        0    23141 2023-07-11 12:14:58.051401 asociita-0.3.2/asociita/components/settings/settings.py
--rw-r--r--   0        0        0     2465 2023-06-07 13:17:41.861780 asociita-0.3.2/asociita/datasets/__pycache__/fetch_data.cpython-310.pyc
--rw-r--r--   0        0        0     1997 2023-06-07 14:35:08.514819 asociita-0.3.2/asociita/datasets/__pycache__/load_cifar.cpython-310.pyc
--rw-r--r--   0        0        0     2034 2023-06-07 14:35:08.514819 asociita-0.3.2/asociita/datasets/__pycache__/load_fmnist.cpython-310.pyc
--rw-r--r--   0        0        0     2023 2023-06-07 14:35:08.314826 asociita-0.3.2/asociita/datasets/__pycache__/load_mnist.cpython-310.pyc
--rw-r--r--   0        0        0     1420 2023-06-07 14:35:08.514819 asociita-0.3.2/asociita/datasets/__pycache__/save_blueprint.cpython-310.pyc
--rw-r--r--   0        0        0     4844 2023-06-12 11:32:41.024825 asociita-0.3.2/asociita/datasets/__pycache__/shard_splits.cpython-310.pyc
--rw-r--r--   0        0        0     5554 2023-06-14 13:55:29.401627 asociita-0.3.2/asociita/datasets/__pycache__/shard_transformation.cpython-310.pyc
--rw-r--r--   0        0        0     3288 2023-06-07 13:08:30.716688 asociita-0.3.2/asociita/datasets/fetch_data.py
--rw-r--r--   0        0        0     3012 2023-06-07 14:34:09.128863 asociita-0.3.2/asociita/datasets/load_cifar.py
--rw-r--r--   0        0        0     2973 2023-06-07 14:34:21.476438 asociita-0.3.2/asociita/datasets/load_fmnist.py
--rw-r--r--   0        0        0     2955 2023-06-07 14:33:17.378645 asociita-0.3.2/asociita/datasets/load_mnist.py
--rw-r--r--   0        0        0     1314 2023-06-07 14:34:55.775257 asociita-0.3.2/asociita/datasets/save_blueprint.py
--rw-r--r--   0        0        0     6838 2023-06-09 14:54:11.498938 asociita-0.3.2/asociita/datasets/shard_splits.py
--rw-r--r--   0        0        0     5962 2023-06-14 13:53:33.877567 asociita-0.3.2/asociita/datasets/shard_transformation.py
--rw-r--r--   0        0        0      798 2023-06-05 13:07:28.160901 asociita-0.3.2/asociita/exceptions/__pycache__/evaluatorexception.cpython-310.pyc
--rw-r--r--   0        0        0      442 2023-06-16 12:12:22.850903 asociita-0.3.2/asociita/exceptions/__pycache__/modelexception.cpython-310.pyc
--rw-r--r--   0        0        0      990 2023-06-16 09:02:36.793602 asociita-0.3.2/asociita/exceptions/__pycache__/settingexception.cpython-310.pyc
--rw-r--r--   0        0        0      391 2023-06-05 10:23:46.853997 asociita-0.3.2/asociita/exceptions/evaluatorexception.py
--rw-r--r--   0        0        0       93 2023-06-16 11:49:20.285800 asociita-0.3.2/asociita/exceptions/modelexception.py
--rw-r--r--   0        0        0      420 2023-06-15 21:36:35.590719 asociita-0.3.2/asociita/exceptions/settingexception.py
--rw-r--r--   0        0        0     1139 2023-05-29 09:36:33.144103 asociita-0.3.2/asociita/models/pytorch/__pycache__/cifar10.cpython-310.pyc
--rw-r--r--   0        0        0    13786 2023-07-13 09:56:16.697717 asociita-0.3.2/asociita/models/pytorch/__pycache__/federated_model.cpython-310.pyc
--rw-r--r--   0        0        0      557 2023-06-01 15:37:30.741582 asociita-0.3.2/asociita/models/pytorch/__pycache__/fmnist.cpython-310.pyc
--rw-r--r--   0        0        0     4114 2023-06-14 08:05:54.914256 asociita-0.3.2/asociita/models/pytorch/__pycache__/mnist.cpython-310.pyc
--rw-r--r--   0        0        0      679 2023-05-29 08:30:33.481904 asociita-0.3.2/asociita/models/pytorch/cifar10.py
--rw-r--r--   0        0        0    17178 2023-07-13 09:54:08.141049 asociita-0.3.2/asociita/models/pytorch/federated_model.py
--rw-r--r--   0        0        0      288 2023-06-01 15:35:54.360809 asociita-0.3.2/asociita/models/pytorch/fmnist.py
--rw-r--r--   0        0        0     5260 2023-06-14 08:05:45.666579 asociita-0.3.2/asociita/models/pytorch/mnist.py
--rw-r--r--   0        0        0     6202 2023-06-26 13:45:06.401533 asociita-0.3.2/asociita/utils/__pycache__/computations.cpython-310.pyc
--rw-r--r--   0        0        0     1162 2023-05-29 09:36:33.148103 asociita-0.3.2/asociita/utils/__pycache__/custom_transformations.cpython-310.pyc
--rw-r--r--   0        0        0     1575 2023-06-22 17:32:18.144898 asociita-0.3.2/asociita/utils/__pycache__/debugger.cpython-310.pyc
--rw-r--r--   0        0        0     3695 2023-05-29 09:36:33.136103 asociita-0.3.2/asociita/utils/__pycache__/handlers.cpython-310.pyc
--rw-r--r--   0        0        0     2009 2023-06-23 10:59:17.491655 asociita-0.3.2/asociita/utils/__pycache__/helpers.cpython-310.pyc
--rw-r--r--   0        0        0     1079 2023-07-13 09:58:51.477702 asociita-0.3.2/asociita/utils/__pycache__/loggers.cpython-310.pyc
--rw-r--r--   0        0        0     4876 2023-06-26 09:06:30.509538 asociita-0.3.2/asociita/utils/__pycache__/optimizers.cpython-310.pyc
--rw-r--r--   0        0        0     4859 2023-06-05 13:07:02.649795 asociita-0.3.2/asociita/utils/__pycache__/orchestrations.cpython-310.pyc
--rw-r--r--   0        0        0     1282 2023-05-29 09:36:33.148103 asociita-0.3.2/asociita/utils/__pycache__/showcase.cpython-310.pyc
--rw-r--r--   0        0        0     5816 2023-06-26 13:44:42.626331 asociita-0.3.2/asociita/utils/computations.py
--rw-r--r--   0        0        0      613 2023-05-29 08:30:33.481904 asociita-0.3.2/asociita/utils/custom_transformations.py
--rw-r--r--   0        0        0     1388 2023-06-22 17:23:31.450734 asociita-0.3.2/asociita/utils/debugger.py
--rw-r--r--   0        0        0     4648 2023-05-29 08:30:33.481904 asociita-0.3.2/asociita/utils/handlers.py
--rw-r--r--   0        0        0     1312 2023-06-23 10:58:27.961327 asociita-0.3.2/asociita/utils/helpers.py
--rw-r--r--   0        0        0     1640 2023-07-13 09:58:47.289811 asociita-0.3.2/asociita/utils/loggers.py
--rw-r--r--   0        0        0     8064 2023-06-26 09:06:22.349796 asociita-0.3.2/asociita/utils/optimizers.py
--rw-r--r--   0        0        0     4526 2023-06-05 10:50:02.994008 asociita-0.3.2/asociita/utils/orchestrations.py
--rw-r--r--   0        0        0     1026 2023-05-29 08:30:33.481904 asociita-0.3.2/asociita/utils/showcase.py
--rw-r--r--   0        0        0      678 2023-07-13 10:06:11.350282 asociita-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 asociita-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-29 08:30:33.477904 asociita-0.3.3/LICENSE
+-rw-r--r--   0        0        0     2812 2023-05-29 08:30:33.477904 asociita-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-29 08:30:33.477904 asociita-0.3.3/asociita/__init__.py
+-rw-r--r--   0        0        0     2725 2023-07-11 10:54:45.641955 asociita-0.3.3/asociita/components/archiver/__pycache__/archive_manager.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-07-11 10:54:39.082119 asociita-0.3.3/asociita/components/archiver/archive_manager.py
+-rw-r--r--   0        0        0    11701 2023-07-17 19:25:35.652593 asociita-0.3.3/asociita/components/evaluator/__pycache__/evaluation_manager.cpython-310.pyc
+-rw-r--r--   0        0        0     4858 2023-07-17 19:25:35.652593 asociita-0.3.3/asociita/components/evaluator/__pycache__/lsaa_evaluator.cpython-310.pyc
+-rw-r--r--   0        0        0     6307 2023-06-16 21:39:14.145401 asociita-0.3.3/asociita/components/evaluator/__pycache__/or_evaluator.cpython-310.pyc
+-rw-r--r--   0        0        0    14893 2023-07-17 19:25:35.652593 asociita-0.3.3/asociita/components/evaluator/__pycache__/sample_evaluator.cpython-310.pyc
+-rw-r--r--   0        0        0    18742 2023-07-17 19:25:33.272652 asociita-0.3.3/asociita/components/evaluator/evaluation_manager.py
+-rw-r--r--   0        0        0     5561 2023-07-17 19:25:33.272652 asociita-0.3.3/asociita/components/evaluator/lsaa_evaluator.py
+-rw-r--r--   0        0        0    13324 2023-05-29 08:30:33.477904 asociita-0.3.3/asociita/components/evaluator/mr_evaluator.py
+-rw-r--r--   0        0        0     9972 2023-06-16 21:38:55.086092 asociita-0.3.3/asociita/components/evaluator/or_evaluator.py
+-rw-r--r--   0        0        0    18471 2023-07-17 19:25:33.272652 asociita-0.3.3/asociita/components/evaluator/sample_evaluator.py
+-rw-r--r--   0        0        0     3999 2023-07-17 16:29:11.910865 asociita-0.3.3/asociita/components/nodes/__pycache__/federated_node.cpython-310.pyc
+-rw-r--r--   0        0        0     4366 2023-07-16 13:33:46.445218 asociita-0.3.3/asociita/components/nodes/federated_node.py
+-rw-r--r--   0        0        0     6270 2023-07-17 19:03:11.725971 asociita-0.3.3/asociita/components/orchestrator/__pycache__/evaluator_orchestrator.cpython-310.pyc
+-rw-r--r--   0        0        0     5588 2023-07-13 09:26:40.219672 asociita-0.3.3/asociita/components/orchestrator/__pycache__/fedopt_orchestrator.cpython-310.pyc
+-rw-r--r--   0        0        0     8999 2023-07-17 16:29:11.446877 asociita-0.3.3/asociita/components/orchestrator/__pycache__/generic_orchestrator.cpython-310.pyc
+-rw-r--r--   0        0        0     8790 2023-07-17 19:03:05.726122 asociita-0.3.3/asociita/components/orchestrator/evaluator_orchestrator.py
+-rw-r--r--   0        0        0     7373 2023-07-13 09:23:34.044495 asociita-0.3.3/asociita/components/orchestrator/fedopt_orchestrator.py
+-rw-r--r--   0        0        0    11545 2023-07-16 13:33:46.445218 asociita-0.3.3/asociita/components/orchestrator/generic_orchestrator.py
+-rw-r--r--   0        0        0     5098 2023-07-12 15:13:21.310949 asociita-0.3.3/asociita/components/settings/__pycache__/evaluator_settings.cpython-310.pyc
+-rw-r--r--   0        0        0     4759 2023-07-12 14:39:39.170606 asociita-0.3.3/asociita/components/settings/__pycache__/fedopt_settings.cpython-310.pyc
+-rw-r--r--   0        0        0     1663 2023-07-12 14:39:39.170606 asociita-0.3.3/asociita/components/settings/__pycache__/init_settings.cpython-310.pyc
+-rw-r--r--   0        0        0    13715 2023-07-11 12:14:58.271395 asociita-0.3.3/asociita/components/settings/__pycache__/settings.cpython-310.pyc
+-rw-r--r--   0        0        0     6901 2023-07-12 15:13:18.167030 asociita-0.3.3/asociita/components/settings/evaluator_settings.py
+-rw-r--r--   0        0        0     5835 2023-07-12 14:39:37.466652 asociita-0.3.3/asociita/components/settings/fedopt_settings.py
+-rw-r--r--   0        0        0     1931 2023-07-12 14:39:31.446817 asociita-0.3.3/asociita/components/settings/init_settings.py
+-rw-r--r--   0        0        0    23141 2023-07-11 12:14:58.051401 asociita-0.3.3/asociita/components/settings/settings.py
+-rw-r--r--   0        0        0     2465 2023-06-07 13:17:41.861780 asociita-0.3.3/asociita/datasets/__pycache__/fetch_data.cpython-310.pyc
+-rw-r--r--   0        0        0     1997 2023-06-07 14:35:08.514819 asociita-0.3.3/asociita/datasets/__pycache__/load_cifar.cpython-310.pyc
+-rw-r--r--   0        0        0     2034 2023-06-07 14:35:08.514819 asociita-0.3.3/asociita/datasets/__pycache__/load_fmnist.cpython-310.pyc
+-rw-r--r--   0        0        0     2023 2023-06-07 14:35:08.314826 asociita-0.3.3/asociita/datasets/__pycache__/load_mnist.cpython-310.pyc
+-rw-r--r--   0        0        0     1420 2023-06-07 14:35:08.514819 asociita-0.3.3/asociita/datasets/__pycache__/save_blueprint.cpython-310.pyc
+-rw-r--r--   0        0        0     4844 2023-06-12 11:32:41.024825 asociita-0.3.3/asociita/datasets/__pycache__/shard_splits.cpython-310.pyc
+-rw-r--r--   0        0        0     5554 2023-06-14 13:55:29.401627 asociita-0.3.3/asociita/datasets/__pycache__/shard_transformation.cpython-310.pyc
+-rw-r--r--   0        0        0     3288 2023-06-07 13:08:30.716688 asociita-0.3.3/asociita/datasets/fetch_data.py
+-rw-r--r--   0        0        0     3012 2023-06-07 14:34:09.128863 asociita-0.3.3/asociita/datasets/load_cifar.py
+-rw-r--r--   0        0        0     2973 2023-06-07 14:34:21.476438 asociita-0.3.3/asociita/datasets/load_fmnist.py
+-rw-r--r--   0        0        0     2955 2023-06-07 14:33:17.378645 asociita-0.3.3/asociita/datasets/load_mnist.py
+-rw-r--r--   0        0        0     1314 2023-06-07 14:34:55.775257 asociita-0.3.3/asociita/datasets/save_blueprint.py
+-rw-r--r--   0        0        0     6838 2023-06-09 14:54:11.498938 asociita-0.3.3/asociita/datasets/shard_splits.py
+-rw-r--r--   0        0        0     5962 2023-06-14 13:53:33.877567 asociita-0.3.3/asociita/datasets/shard_transformation.py
+-rw-r--r--   0        0        0      798 2023-06-05 13:07:28.160901 asociita-0.3.3/asociita/exceptions/__pycache__/evaluatorexception.cpython-310.pyc
+-rw-r--r--   0        0        0      442 2023-06-16 12:12:22.850903 asociita-0.3.3/asociita/exceptions/__pycache__/modelexception.cpython-310.pyc
+-rw-r--r--   0        0        0      990 2023-06-16 09:02:36.793602 asociita-0.3.3/asociita/exceptions/__pycache__/settingexception.cpython-310.pyc
+-rw-r--r--   0        0        0      391 2023-06-05 10:23:46.853997 asociita-0.3.3/asociita/exceptions/evaluatorexception.py
+-rw-r--r--   0        0        0       93 2023-06-16 11:49:20.285800 asociita-0.3.3/asociita/exceptions/modelexception.py
+-rw-r--r--   0        0        0      420 2023-06-15 21:36:35.590719 asociita-0.3.3/asociita/exceptions/settingexception.py
+-rw-r--r--   0        0        0     1139 2023-05-29 09:36:33.144103 asociita-0.3.3/asociita/models/pytorch/__pycache__/cifar10.cpython-310.pyc
+-rw-r--r--   0        0        0    13786 2023-07-17 16:29:11.914865 asociita-0.3.3/asociita/models/pytorch/__pycache__/federated_model.cpython-310.pyc
+-rw-r--r--   0        0        0      557 2023-06-01 15:37:30.741582 asociita-0.3.3/asociita/models/pytorch/__pycache__/fmnist.cpython-310.pyc
+-rw-r--r--   0        0        0     4114 2023-06-14 08:05:54.914256 asociita-0.3.3/asociita/models/pytorch/__pycache__/mnist.cpython-310.pyc
+-rw-r--r--   0        0        0      679 2023-05-29 08:30:33.481904 asociita-0.3.3/asociita/models/pytorch/cifar10.py
+-rw-r--r--   0        0        0    17178 2023-07-16 13:33:46.449218 asociita-0.3.3/asociita/models/pytorch/federated_model.py
+-rw-r--r--   0        0        0      288 2023-06-01 15:35:54.360809 asociita-0.3.3/asociita/models/pytorch/fmnist.py
+-rw-r--r--   0        0        0     5260 2023-06-14 08:05:45.666579 asociita-0.3.3/asociita/models/pytorch/mnist.py
+-rw-r--r--   0        0        0     6202 2023-06-26 13:45:06.401533 asociita-0.3.3/asociita/utils/__pycache__/computations.cpython-310.pyc
+-rw-r--r--   0        0        0     1162 2023-05-29 09:36:33.148103 asociita-0.3.3/asociita/utils/__pycache__/custom_transformations.cpython-310.pyc
+-rw-r--r--   0        0        0     1575 2023-06-22 17:32:18.144898 asociita-0.3.3/asociita/utils/__pycache__/debugger.cpython-310.pyc
+-rw-r--r--   0        0        0     3695 2023-05-29 09:36:33.136103 asociita-0.3.3/asociita/utils/__pycache__/handlers.cpython-310.pyc
+-rw-r--r--   0        0        0     2009 2023-06-23 10:59:17.491655 asociita-0.3.3/asociita/utils/__pycache__/helpers.cpython-310.pyc
+-rw-r--r--   0        0        0     1079 2023-07-17 16:29:13.102835 asociita-0.3.3/asociita/utils/__pycache__/loggers.cpython-310.pyc
+-rw-r--r--   0        0        0     4876 2023-06-26 09:06:30.509538 asociita-0.3.3/asociita/utils/__pycache__/optimizers.cpython-310.pyc
+-rw-r--r--   0        0        0     4859 2023-06-05 13:07:02.649795 asociita-0.3.3/asociita/utils/__pycache__/orchestrations.cpython-310.pyc
+-rw-r--r--   0        0        0     1282 2023-05-29 09:36:33.148103 asociita-0.3.3/asociita/utils/__pycache__/showcase.cpython-310.pyc
+-rw-r--r--   0        0        0     5816 2023-06-26 13:44:42.626331 asociita-0.3.3/asociita/utils/computations.py
+-rw-r--r--   0        0        0      613 2023-05-29 08:30:33.481904 asociita-0.3.3/asociita/utils/custom_transformations.py
+-rw-r--r--   0        0        0     1388 2023-06-22 17:23:31.450734 asociita-0.3.3/asociita/utils/debugger.py
+-rw-r--r--   0        0        0     4648 2023-05-29 08:30:33.481904 asociita-0.3.3/asociita/utils/handlers.py
+-rw-r--r--   0        0        0     1312 2023-06-23 10:58:27.961327 asociita-0.3.3/asociita/utils/helpers.py
+-rw-r--r--   0        0        0     1640 2023-07-16 13:33:46.449218 asociita-0.3.3/asociita/utils/loggers.py
+-rw-r--r--   0        0        0     8064 2023-06-26 09:06:22.349796 asociita-0.3.3/asociita/utils/optimizers.py
+-rw-r--r--   0        0        0     4526 2023-06-05 10:50:02.994008 asociita-0.3.3/asociita/utils/orchestrations.py
+-rw-r--r--   0        0        0     1026 2023-05-29 08:30:33.481904 asociita-0.3.3/asociita/utils/showcase.py
+-rw-r--r--   0        0        0      678 2023-07-18 13:18:39.613274 asociita-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3765 1970-01-01 00:00:00.000000 asociita-0.3.3/PKG-INFO
```

### Comparing `asociita-0.3.2/LICENSE` & `asociita-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/README.md` & `asociita-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/archiver/__pycache__/archive_manager.cpython-310.pyc` & `asociita-0.3.3/asociita/components/archiver/__pycache__/archive_manager.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/archiver/archive_manager.py` & `asociita-0.3.3/asociita/components/archiver/archive_manager.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/evaluator/__pycache__/evaluation_manager.cpython-310.pyc` & `asociita-0.3.3/asociita/components/evaluator/__pycache__/evaluation_manager.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jun 22 18:08:42 2023 UTC, .py size: 15259 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 14% similar despite different names*

```diff
@@ -1,656 +1,732 @@
-00000000: 6f0d 0d0a 0000 0000 2a8e 9464 9b3b 0000  o.......*..d.;..
+00000000: 6f0d 0d0a 0000 0000 ad95 b564 3649 0000  o..........d6I..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0003 0000 0040 0000 0073 7e00 0000 6400  .....@...s~...d.
+00000020: 0003 0000 0040 0000 0073 8a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
-00000040: 6d03 5a03 0100 6400 6403 6c02 6d04 5a04  m.Z...d.d.l.m.Z.
-00000050: 0100 6400 6404 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
+00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
+00000050: 0100 6400 6404 6c04 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c07 6d08 5a08 0100 6400 6406 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 0100 6400 6407 6c0b 6d0c 5a0c  m.Z...d.d.l.m.Z.
-00000080: 0100 6400 6408 6c0d 5a0d 6400 6408 6c0e  ..d.d.l.Z.d.d.l.
-00000090: 5a0e 6400 6408 6c0f 5a0f 4700 6409 640a  Z.d.d.l.Z.G.d.d.
-000000a0: 8400 640a 8302 5a10 6408 5300 290b e900  ..d...Z.d.S.)...
-000000b0: 0000 0029 01da 0c4f 525f 4576 616c 7561  ...)...OR_Evalua
-000000c0: 746f 7229 01da 1053 616d 706c 655f 4576  tor)...Sample_Ev
-000000d0: 616c 7561 746f 7229 01da 1853 616d 706c  aluator)...Sampl
-000000e0: 655f 5368 6170 6c65 795f 4576 616c 7561  e_Shapley_Evalua
-000000f0: 746f 7229 01da 0e46 6564 6572 6174 6564  tor)...Federated
-00000100: 4d6f 6465 6c29 01da 1f53 616d 706c 655f  Model)...Sample_
-00000110: 4576 616c 7561 746f 725f 496e 6974 5f45  Evaluator_Init_E
-00000120: 7863 6570 7469 6f6e 2901 da0a 4f70 7469  xception)...Opti
-00000130: 6d69 7a65 7273 2901 da0b 4f72 6465 7265  mizers)...Ordere
-00000140: 6444 6963 744e 6300 0000 0000 0000 0000  dDictNc.........
-00000150: 0000 0000 0000 000b 0000 0040 0000 0073  ...........@...s
-00000160: 8600 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
-00000170: 0902 0902 641b 6403 6504 6404 6505 6405  ....d.d.e.d.e.d.
-00000180: 6506 6406 6507 6407 6402 660a 6408 6409  e.d.e.d.d.f.d.d.
-00000190: 8405 5a08 640a 6505 6602 640b 640c 8404  ..Z.d.e.f.d.d...
-000001a0: 5a09 640d 6505 6602 640e 640f 8404 5a0a  Z.d.e.f.d.d...Z.
-000001b0: 6410 650b 6602 6411 6412 8404 5a0c 6413  d.e.f.d.d...Z.d.
-000001c0: 650d 6414 6506 6415 6507 6606 6416 6417  e.d.e.d.e.f.d.d.
-000001d0: 8404 5a0e 0902 641c 6418 650f 6602 6419  ..Z...d.d.e.f.d.
-000001e0: 641a 8405 5a10 6402 5300 291d da12 4576  d...Z.d.S.)...Ev
-000001f0: 616c 7561 7469 6f6e 5f4d 616e 6167 6572  aluation_Manager
-00000200: 61bb 0200 0045 7661 6c75 6174 696f 6e20  a....Evaluation 
-00000210: 4d61 6e61 6765 7220 656e 6361 7073 756c  Manager encapsul
-00000220: 6174 6573 2074 6865 2077 686f 6c65 2070  ates the whole p
-00000230: 726f 6365 7373 206f 6620 6173 7365 7373  rocess of assess
-00000240: 696e 6720 7468 6520 6d61 7267 696e 616c  ing the marginal
-00000250: 0a20 2020 2063 6c69 656e 7473 2720 636f  .    clients' co
-00000260: 6e74 7269 6275 7469 6f6e 732c 2073 6f20  ntributions, so 
-00000270: 7468 6520 6f72 6368 6573 7472 6174 6f72  the orchestrator
-00000280: 2063 6f64 6520 6973 2066 7265 6520 6f66   code is free of
-00000290: 2061 6e79 2065 6e63 756d 6272 616e 6365   any encumbrance
-000002a0: 0a20 2020 2063 6f6e 6e65 6374 6564 2074  .    connected t
-000002b0: 6f20 6974 2e20 4576 616c 7561 7469 6f6e  o it. Evaluation
-000002c0: 204d 616e 6167 6572 206c 6966 652d 6379   Manager life-cy
-000002d0: 636c 6520 6973 2073 706c 6974 7465 6420  cle is splitted 
-000002e0: 696e 746f 2066 6f75 7220 6469 6666 6572  into four differ
-000002f0: 656e 740a 2020 2020 7374 6167 6573 3a20  ent.    stages: 
-00000300: 696e 6974 6961 6c69 7a61 7469 6f6e 2c20  initialization, 
-00000310: 7072 6573 6572 7661 7469 6f6e 2c20 7472  preservation, tr
-00000320: 6163 6b69 6e67 2061 6e64 2066 696e 616c  acking and final
-00000330: 697a 6174 696f 6e2e 2049 6e69 7469 616c  ization. Initial
-00000340: 697a 6174 696f 6e0a 2020 2020 7265 7175  ization.    requ
-00000350: 6972 6573 2061 2064 6963 7469 6f6e 6172  ires a dictionar
-00000360: 7920 636f 6e74 6169 6e69 6e67 2061 6c6c  y containing all
-00000370: 2074 6865 2072 656c 6576 616e 7420 7365   the relevant se
-00000380: 7474 696e 6773 2e20 5072 6573 6572 7661  ttings. Preserva
-00000390: 7469 6f6e 2073 686f 756c 640a 2020 2020  tion should.    
-000003a0: 6265 2063 616c 6c65 6420 6561 6368 2072  be called each r
-000003b0: 6f75 6e64 2062 6566 6f72 6520 7468 6520  ound before the 
-000003c0: 7472 6169 6e69 6e67 2063 6f6d 6d65 6e63  training commenc
-000003d0: 6573 2028 736f 2074 6865 2065 7661 6c75  es (so the evalu
-000003e0: 6174 696f 6e20 6d61 6e61 6765 720a 2020  ation manager.  
-000003f0: 2020 6861 7320 6c61 7374 2073 6574 206f    has last set o
-00000400: 6620 7765 6967 6874 7320 616e 6420 6d6f  f weights and mo
-00000410: 6d65 6e74 756d 2069 6e66 6f72 6d61 7469  mentum informati
-00000420: 6f6e 292e 2054 7261 636b 696e 6720 7368  on). Tracking sh
-00000430: 6f75 6c64 2062 6520 6361 6c6c 6564 2065  ould be called e
-00000440: 6163 680a 2020 2020 726f 756e 6420 746f  ach.    round to
-00000450: 2063 6f6d 7075 7465 2064 6966 6665 7265   compute differe
-00000460: 6e74 206d 6574 7269 6373 2e20 4669 6e61  nt metrics. Fina
-00000470: 6c69 7a61 7469 6f6e 2063 616e 2062 6520  lization can be 
-00000480: 6361 6c6c 6564 2061 7420 7468 6520 656e  called at the en
-00000490: 6420 6f66 2074 6865 0a20 2020 206c 6966  d of the.    lif
-000004a0: 652d 6379 636c 6520 746f 2070 7265 7365  e-cycle to prese
-000004b0: 7276 6520 7468 6520 7265 7375 6c74 732e  rve the results.
-000004c0: 4eda 0873 6574 7469 6e67 73da 056d 6f64  N..settings..mod
-000004d0: 656c da05 6e6f 6465 73da 0a69 7465 7261  el..nodes..itera
-000004e0: 7469 6f6e 73da 0672 6574 7572 6e63 0500  tions..returnc..
-000004f0: 0000 0000 0000 0000 0000 0600 0000 0a00  ................
-00000500: 0000 0300 0000 7302 0200 007c 017c 005f  ......s....|.|._
-00000510: 0064 017c 005f 0164 017c 005f 0264 017c  .d.|._.d.|._.d.|
-00000520: 005f 037c 037c 005f 0467 007c 005f 057c  ._.|.|._.g.|._.|
-00000530: 01a0 0664 02a1 0172 2264 037c 005f 077c  ...d...r"d.|._.|
-00000540: 006a 05a0 0864 04a1 0101 0074 0982 0164  .j...d.....t...d
-00000550: 057c 005f 077c 01a0 0664 06a1 0172 3564  .|._.|...d...r5d
-00000560: 037c 005f 0a7c 006a 05a0 0864 07a1 0101  .|._.|.j...d....
-00000570: 0074 0982 0164 057c 005f 0a7c 01a0 0664  .t...d.|._.|...d
-00000580: 08a1 0172 4764 037c 005f 0b7c 006a 05a0  ...rGd.|._.|.j..
-00000590: 0864 09a1 0101 006e 0364 057c 005f 0b7c  .d.....n.d.|._.|
-000005a0: 01a0 0664 0aa1 0172 5964 037c 005f 0c7c  ...d...rYd.|._.|
-000005b0: 006a 05a0 0864 0ba1 0101 006e 0364 057c  .j...d.....n.d.|
-000005c0: 005f 0c7c 0164 0c19 00a0 0664 0da1 0172  ._.|.d.....d...r
-000005d0: 6764 037c 005f 0d6e 0364 057c 005f 0d7c  gd.|._.n.d.|._.|
-000005e0: 0164 0c19 00a0 0664 0ea1 0172 7464 037c  .d.....d...rtd.|
-000005f0: 005f 0e7c 006a 0773 7a7c 006a 0a72 8174  ._.|.j.sz|.j.r.t
-00000600: 0f7c 017c 0264 0f8d 027c 005f 107c 006a  .|.|.d...|._.|.j
-00000610: 0b64 036b 0272 9e7a 0974 117c 0388 0064  .d.k.r.z.t.|...d
-00000620: 108d 027c 005f 1257 006e 0e04 0074 1379  ...|._.W.n...t.y
-00000630: 9d01 007d 0501 007a 0274 1482 0164 017d  ...}...z.t...d.}
-00000640: 057e 0577 0177 007c 006a 0c64 036b 0272  .~.w.w.|.j.d.k.r
-00000650: bb7a 0974 157c 0388 0064 108d 027c 005f  .z.t.|...d...|._
-00000660: 1657 006e 0e04 0074 1379 ba01 007d 0501  .W.n...t.y...}..
-00000670: 007a 0274 1482 0164 017d 057e 0577 0177  .z.t...d.}.~.w.w
-00000680: 007c 01a0 0664 11a1 0172 c67c 0164 1119  .|...d...r.|.d..
-00000690: 007c 005f 176e 0b87 0066 0164 1264 1384  .|._.n...f.d.d..
-000006a0: 087c 006a 0544 0083 017c 005f 177c 01a0  .|.j.D...|._.|..
-000006b0: 0664 14a1 0172 ea64 037c 005f 187c 01a0  .d...r.d.|._.|..
-000006c0: 0664 15a1 0172 e47c 0164 1619 007c 005f  .d...r.|.d...|._
-000006d0: 196e 0974 1aa0 1ba1 007c 005f 196e 0364  .n.t.....|._.n.d
-000006e0: 057c 005f 187c 01a0 0664 17a1 0172 f764  .|._.|...d...r.d
-000006f0: 057c 005f 1c64 0153 0064 037c 005f 1c7c  .|._.d.S.d.|._.|
-00000700: 0164 1819 007c 005f 1d64 0153 0029 1961  .d...|._.d.S.).a
-00000710: 3106 0000 4d61 6e61 6765 7320 7468 6520  1...Manages the 
-00000720: 7072 6f63 6573 7320 6f66 2065 7661 6c75  process of evalu
-00000730: 6174 696f 6e2e 2043 7265 6174 6573 2061  ation. Creates a
-00000740: 6e20 696e 7374 616e 6365 206f 6620 4576  n instance of Ev
-00000750: 616c 7561 7469 6f6e 5f4d 616e 6167 6572  aluation_Manager
-00000760: 200a 2020 2020 2020 2020 6f62 6a65 6374   .        object
-00000770: 2c20 7468 6174 2063 6f6e 7472 6f6c 7320  , that controls 
-00000780: 616c 6c20 7468 6520 696e 7374 616e 6365  all the instance
-00000790: 7320 7468 6174 2070 6572 666f 726d 2065  s that perform e
-000007a0: 7661 6c75 6174 696f 6e2e 2045 7661 6c75  valuation. Evalu
-000007b0: 6174 696f 6e0a 2020 2020 2020 2020 4d61  ation.        Ma
-000007c0: 6e61 6765 7220 6f70 6572 6174 6f72 6573  nager operatores
-000007d0: 206f 6e20 2766 6c61 6773 2720 7468 6174   on 'flags' that
-000007e0: 2061 7265 2072 6570 7265 7365 6e74 6564   are represented
-000007f0: 2061 7320 626f 6c65 616e 2061 7474 7269   as bolean attri
-00000800: 6275 7465 7320 6f66 2074 6865 0a20 2020  butes of the.   
-00000810: 2020 2020 2069 6e73 7461 6e63 6520 6f66       instance of
-00000820: 2074 6865 2043 6c61 7373 2e20 5468 6520   the Class. The 
-00000830: 7661 6c75 6520 6f66 2066 6c61 6773 2069  value of flags i
-00000840: 7320 6469 6374 6174 6564 2062 7920 7468  s dictated by th
-00000850: 6520 636f 7272 6573 706f 6e64 696e 6720  e corresponding 
-00000860: 7661 6c75 650a 2020 2020 2020 2020 7573  value.        us
-00000870: 6564 2069 6e20 7468 6520 7365 7474 696e  ed in the settin
-00000880: 6773 2e20 4769 7669 6e67 2061 6e20 6578  gs. Giving an ex
-00000890: 616d 706c 652c 2073 6574 7469 6e67 7320  ample, settings 
-000008a0: 5b2e 2e2e 5d5b 2749 4e5f 5341 4d50 4c45  [...]['IN_SAMPLE
-000008b0: 5f4c 4f4f 275d 2074 6f0a 2020 2020 2020  _LOO'] to.      
-000008c0: 2020 5472 7565 2077 696c 6c20 7472 6967    True will trig
-000008d0: 6765 7220 7468 6520 666c 6167 206f 6620  ger the flag of 
-000008e0: 7468 6520 696e 7374 616e 6365 2e20 5468  the instance. Th
-000008f0: 6973 206d 6561 6e73 2c20 7468 6174 2065  is means, that e
-00000900: 6163 6820 7469 6d65 2074 6865 206d 6574  ach time the met
-00000910: 686f 640a 2020 2020 2020 2020 4576 616c  hod.        Eval
-00000920: 7561 7469 6f6e 5f4d 616e 6167 6572 2829  uation_Manager()
-00000930: 2e74 7261 636b 5f72 6573 756c 7473 2069  .track_results i
-00000940: 7320 6361 6c6c 6564 2c20 4576 616c 7561  s called, Evalua
-00000950: 746f 7220 7769 6c6c 2074 7279 2074 6f20  tor will try to 
-00000960: 6361 6c63 756c 6174 650a 2020 2020 2020  calculate.      
-00000970: 2020 4c65 6176 652d 4f6e 652d 4f75 7420    Leave-One-Out 
-00000980: 7363 6f72 6520 666f 7220 6561 6368 2063  score for each c
-00000990: 6c69 656e 7420 696e 2074 6865 2073 616d  lient in the sam
-000009a0: 706c 652e 0a20 2020 2020 2020 200a 2020  ple..        .  
-000009b0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
-000009c0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
-000009d0: 2d2d 2d0a 2020 2020 2020 2020 7365 7474  ---.        sett
-000009e0: 696e 6773 3a20 6469 6374 0a20 2020 2020  ings: dict.     
-000009f0: 2020 2020 2020 2041 2064 6963 7469 6f6e         A diction
-00000a00: 6172 7920 636f 6e74 6169 6e69 6e67 2061  ary containing a
-00000a10: 6c6c 2074 6865 2072 656c 6576 616e 7420  ll the relevant 
-00000a20: 7365 7474 696e 6773 2066 6f72 2074 6865  settings for the
-00000a30: 2065 7661 6c75 6174 696f 6e5f 6d61 6e61   evaluation_mana
-00000a40: 6765 722e 0a20 2020 2020 2020 206d 6f64  ger..        mod
-00000a50: 656c 3a20 4665 6465 7261 7465 644d 6f64  el: FederatedMod
-00000a60: 656c 0a20 2020 2020 2020 2020 2020 2041  el.            A
-00000a70: 2069 6e69 7469 616c 697a 6564 2069 6e73   initialized ins
-00000a80: 7461 6e63 6520 6f66 2074 6865 2063 6c61  tance of the cla
-00000a90: 7373 2061 736f 6369 6974 612e 6d6f 6465  ss asociita.mode
-00000aa0: 6c73 2e70 7974 6f72 6368 2e66 6564 6572  ls.pytorch.feder
-00000ab0: 6174 6564 5f6d 6f64 656c 2e46 6564 6572  ated_model.Feder
-00000ac0: 6174 6564 4d6f 6465 6c0a 2020 2020 2020  atedModel.      
-00000ad0: 2020 2020 2020 5468 6973 2069 7320 6e65        This is ne
-00000ae0: 6365 7373 6172 7920 746f 2069 6e69 7469  cessary to initi
-00000af0: 616c 697a 6520 736f 6d65 2063 6f6e 7472  alize some contr
-00000b00: 6962 7574 696f 6e2d 6573 7469 6d61 7469  ibution-estimati
-00000b10: 6f6e 206f 626a 6563 7473 2e0a 2020 2020  on objects..    
-00000b20: 2020 2020 6e6f 6465 733a 206c 6973 742c      nodes: list,
-00000b30: 2064 6566 6175 6c74 2074 6f20 4e6f 6e65   default to None
-00000b40: 0a20 2020 2020 2020 2020 2020 2041 206c  .            A l
-00000b50: 6973 7420 636f 6e74 6169 6e69 6e67 2074  ist containing t
-00000b60: 6865 2069 6427 7320 6f66 2061 6c6c 2074  he id's of all t
-00000b70: 6865 2072 656c 6576 616e 7420 6e6f 6465  he relevant node
-00000b80: 732e 0a20 2020 2020 2020 2069 7465 7261  s..        itera
-00000b90: 7469 6f6e 733a 2069 6e74 2c20 6465 6661  tions: int, defa
-00000ba0: 756c 7420 746f 204e 6f6e 650a 2020 2020  ult to None.    
-00000bb0: 2020 2020 2020 2020 4e75 6d62 6572 206f          Number o
-00000bc0: 6620 6974 6572 6174 696f 6e73 2e0a 2020  f iterations..  
-00000bd0: 2020 2020 2020 0a20 2020 2020 2020 2052        .        R
-00000be0: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
-00000bf0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
-00000c00: 6f6e 650a 0a20 2020 2020 2020 2052 6574  one..        Ret
-00000c10: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-00000c20: 2d2d 2d2d 0a20 2020 2020 2020 2020 2020  ----.           
-00000c30: 204e 6f74 496d 706c 656d 656e 7465 6445   NotImplementedE
-00000c40: 7272 6f72 0a20 2020 2020 2020 2020 2020  rror.           
-00000c50: 2020 2020 2049 6620 7468 6520 666c 6167       If the flag
-00000c60: 2066 6f72 204f 6e65 2d52 6f75 6e64 2053   for One-Round S
-00000c70: 6861 706c 6579 2061 6e64 204f 6e65 2d52  hapley and One-R
-00000c80: 6f75 6e64 204c 4f4f 2069 7320 7365 7420  ound LOO is set 
-00000c90: 746f 2054 7275 652e 0a20 2020 2020 2020  to True..       
-00000ca0: 2020 2020 2053 616d 706c 655f 4576 616c       Sample_Eval
-00000cb0: 7561 746f 725f 496e 6974 5f45 7863 6570  uator_Init_Excep
-00000cc0: 7469 6f6e 0a20 2020 2020 2020 2020 2020  tion.           
-00000cd0: 2020 2020 2049 6620 7468 6520 4576 616c       If the Eval
-00000ce0: 7561 7469 6f6e 204d 616e 6167 6572 2069  uation Manager i
-00000cf0: 7320 756e 6162 6c65 2074 6f20 696e 6974  s unable to init
-00000d00: 6961 6c69 7a65 2061 6e20 696e 7374 616e  ialize an instan
-00000d10: 6365 206f 6620 7468 6520 0a20 2020 2020  ce of the .     
-00000d20: 2020 2020 2020 2020 2020 2053 616d 706c             Sampl
-00000d30: 6520 4576 616c 7561 746f 722e 0a20 2020  e Evaluator..   
-00000d40: 2020 2020 204e da0a 5368 6170 6c65 795f       N..Shapley_
-00000d50: 4f52 545a 0a73 6861 706c 6579 5f6f 7246  ORTZ.shapley_orF
-00000d60: da06 4c4f 4f5f 4f52 5a06 6c6f 6f5f 6f72  ..LOO_ORZ.loo_or
-00000d70: da0d 494e 5f53 414d 504c 455f 4c4f 4fda  ..IN_SAMPLE_LOO.
-00000d80: 0d69 6e5f 7361 6d70 6c65 5f6c 6f6f da0e  .in_sample_loo..
-00000d90: 494e 5f53 414d 504c 455f 5348 4150 da0e  IN_SAMPLE_SHAP..
-00000da0: 696e 5f73 616d 706c 655f 7368 6170 da13  in_sample_shap..
-00000db0: 7072 6573 6572 7665 5f65 7661 6c75 6174  preserve_evaluat
-00000dc0: 696f 6eda 1870 7265 7365 7276 655f 7061  ion..preserve_pa
-00000dd0: 7274 6961 6c5f 7265 7375 6c74 73da 1670  rtial_results..p
-00000de0: 7265 7365 7276 655f 6669 6e61 6c5f 7265  reserve_final_re
-00000df0: 7375 6c74 7329 0272 0a00 0000 720b 0000  sults).r....r...
-00000e00: 0029 0272 0c00 0000 720d 0000 00da 0973  .).r....r......s
-00000e10: 6368 6564 756c 6572 6301 0000 0000 0000  chedulerc.......
-00000e20: 0000 0000 0002 0000 0006 0000 0013 0000  ................
-00000e30: 0073 2000 0000 6900 7c00 5d0c 7d01 7c01  .s ...i.|.].}.|.
-00000e40: 6400 6401 8400 7400 8800 8301 4400 8301  d.d...t.....D...
-00000e50: 9302 7102 5300 2902 6301 0000 0000 0000  ..q.S.).c.......
-00000e60: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
-00000e70: 0073 1000 0000 6700 7c00 5d04 7d01 7c01  .s....g.|.].}.|.
-00000e80: 9102 7102 5300 a900 7219 0000 0029 02da  ..q.S...r....)..
-00000e90: 022e 30da 0969 7465 7261 7469 6f6e 7219  ..0..iterationr.
-00000ea0: 0000 0072 1900 0000 fa7f 2f68 6f6d 652f  ...r....../home/
-00000eb0: 6d7a 757a 6961 6b2f 736e 6170 2f73 6e61  mzuziak/snap/sna
-00000ec0: 7064 2d64 6573 6b74 6f70 2d69 6e74 6567  pd-desktop-integ
-00000ed0: 7261 7469 6f6e 2f38 332f 446f 6375 6d65  ration/83/Docume
-00000ee0: 6e74 732f 4173 6f63 6969 7461 2f61 736f  nts/Asociita/aso
-00000ef0: 6369 6974 612f 6173 6f63 6969 7461 2f63  ciita/asociita/c
-00000f00: 6f6d 706f 6e65 6e74 732f 6576 616c 7561  omponents/evalua
-00000f10: 746f 722f 6576 616c 7561 7469 6f6e 5f6d  tor/evaluation_m
-00000f20: 616e 6167 6572 2e70 79da 0a3c 6c69 7374  anager.py..<list
-00000f30: 636f 6d70 3e83 0000 0073 0200 0000 1000  comp>....s......
-00000f40: 7a3a 4576 616c 7561 7469 6f6e 5f4d 616e  z:Evaluation_Man
-00000f50: 6167 6572 2e5f 5f69 6e69 745f 5f2e 3c6c  ager.__init__.<l
-00000f60: 6f63 616c 733e 2e3c 6469 6374 636f 6d70  ocals>.<dictcomp
-00000f70: 3e2e 3c6c 6973 7463 6f6d 703e 2901 da05  >.<listcomp>)...
-00000f80: 7261 6e67 6529 0272 1a00 0000 da04 666c  range).r......fl
-00000f90: 6167 a901 720d 0000 0072 1900 0000 721c  ag..r....r....r.
-00000fa0: 0000 00da 0a3c 6469 6374 636f 6d70 3e83  .....<dictcomp>.
-00000fb0: 0000 0073 0200 0000 2000 7a2f 4576 616c  ...s.... .z/Eval
-00000fc0: 7561 7469 6f6e 5f4d 616e 6167 6572 2e5f  uation_Manager._
-00000fd0: 5f69 6e69 745f 5f2e 3c6c 6f63 616c 733e  _init__.<locals>
-00000fe0: 2e3c 6469 6374 636f 6d70 3eda 0a66 756c  .<dictcomp>..ful
-00000ff0: 6c5f 6465 6275 675a 0f64 6562 7567 5f66  l_debugZ.debug_f
-00001000: 696c 655f 7061 7468 da0f 6675 6c6c 5f64  ile_path..full_d
-00001010: 6562 7567 5f70 6174 685a 1764 6973 6162  ebug_pathZ.disab
-00001020: 6c65 5f6d 756c 7469 7072 6f63 6573 7369  le_multiprocessi
-00001030: 6e67 da11 6e75 6d62 6572 5f6f 665f 776f  ng..number_of_wo
-00001040: 726b 6572 7329 1e72 0a00 0000 da10 7072  rkers).r......pr
-00001050: 6576 696f 7573 5f63 5f6d 6f64 656c da0f  evious_c_model..
-00001060: 7570 6461 7465 645f 635f 6d6f 6465 6cda  updated_c_model.
-00001070: 1270 7265 7669 6f75 735f 6f70 7469 6d69  .previous_optimi
-00001080: 7a65 7272 0c00 0000 5a0e 636f 6d70 696c  zerr....Z.compil
-00001090: 6564 5f66 6c61 6773 da03 6765 74da 0c66  ed_flags..get..f
-000010a0: 6c61 675f 7368 6170 5f6f 72da 0661 7070  lag_shap_or..app
-000010b0: 656e 64da 134e 6f74 496d 706c 656d 656e  end..NotImplemen
-000010c0: 7465 6445 7272 6f72 da0b 666c 6167 5f6c  tedError..flag_l
-000010d0: 6f6f 5f6f 72da 1566 6c61 675f 7361 6d70  oo_or..flag_samp
-000010e0: 6c65 5f65 7661 6c75 6174 6f72 da17 666c  le_evaluator..fl
-000010f0: 6167 5f73 616d 706c 6573 685f 6576 616c  ag_samplesh_eval
-00001100: 7561 746f 7272 1600 0000 7217 0000 0072  uatorr....r....r
-00001110: 0200 0000 da0c 6f72 5f65 7661 6c75 6174  ......or_evaluat
-00001120: 6f72 7203 0000 00da 1073 616d 706c 655f  orr......sample_
-00001130: 6576 616c 7561 746f 72da 094e 616d 6545  evaluator..NameE
-00001140: 7272 6f72 7206 0000 0072 0400 0000 da12  rrorr....r......
-00001150: 7361 6d70 6c65 7368 5f65 7661 6c75 6174  samplesh_evaluat
-00001160: 6f72 7218 0000 0072 2200 0000 7223 0000  orr....r"...r#..
-00001170: 00da 026f 73da 0667 6574 6377 64da 066d  ...os..getcwd..m
-00001180: 756c 7469 7072 2400 0000 2906 da04 7365  ultipr$...)...se
-00001190: 6c66 720a 0000 0072 0b00 0000 720c 0000  lfr....r....r...
-000011a0: 0072 0d00 0000 da01 6572 1900 0000 7220  .r......er....r 
-000011b0: 0000 0072 1c00 0000 da08 5f5f 696e 6974  ...r......__init
-000011c0: 5f5f 1900 0000 7378 0000 0006 2706 0106  __....sx....'...
-000011d0: 0106 0106 0106 040a 0106 010c 0104 0106  ................
-000011e0: 020a 0206 010c 0104 0106 020a 0206 010e  ................
-000011f0: 0106 020a 0206 010e 0106 020e 0408 0106  ................
-00001200: 020e 0206 010c 0404 0102 0108 ff0a 0302  ................
-00001210: 0112 010e 0104 0108 8002 ff0a 0302 0112  ................
-00001220: 010e 0104 0108 8002 ff0a 040c 0116 020a  ................
-00001230: 0406 010a 010c 010c 0206 020a 030a 0106  ................
-00001240: 020e 017a 1b45 7661 6c75 6174 696f 6e5f  ...z.Evaluation_
-00001250: 4d61 6e61 6765 722e 5f5f 696e 6974 5f5f  Manager.__init__
-00001260: da0e 7072 6576 696f 7573 5f6d 6f64 656c  ..previous_model
-00001270: 6302 0000 0000 0000 0000 0000 0002 0000  c...............
-00001280: 0003 0000 0043 0000 00f3 1000 0000 7400  .....C........t.
-00001290: a001 7c01 a101 7c00 5f02 6401 5300 2902  ..|...|._.d.S.).
-000012a0: 6190 0100 0050 7265 7365 7276 6573 2074  a....Preserves t
-000012b0: 6865 206d 6f64 656c 2066 726f 6d20 7468  he model from th
-000012c0: 6520 7072 6576 696f 7573 2072 6f75 6e64  e previous round
-000012d0: 2062 7920 636f 7079 696e 6720 0a20 2020   by copying .   
-000012e0: 2020 2020 2069 7473 2073 7472 7563 7475       its structu
-000012f0: 7265 2061 6e64 2075 7369 6e67 2069 7420  re and using it 
-00001300: 6173 2061 6e20 6174 7472 6962 7574 6527  as an attribute'
-00001310: 7320 7661 6c75 652e 2053 686f 756c 640a  s value. Should.
-00001320: 2020 2020 2020 2020 6265 2063 616c 6c65          be calle
-00001330: 6420 6561 6368 2074 7261 696e 696e 6720  d each training 
-00001340: 726f 756e 6420 6265 666f 7265 2074 6865  round before the
-00001350: 2070 726f 7065 7220 7472 6169 6e69 6e67   proper training
-00001360: 0a20 2020 2020 2020 2063 6f6d 6d65 6e63  .        commenc
-00001370: 6573 2e0a 2020 2020 2020 2020 0a20 2020  es..        .   
-00001380: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
-00001390: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
-000013a0: 2d2d 0a20 2020 2020 2020 2070 7265 7669  --.        previ
-000013b0: 6f75 735f 6d6f 6465 6c3a 2046 6564 6572  ous_model: Feder
-000013c0: 6174 6564 4d6f 6465 6c0a 2020 2020 2020  atedModel.      
-000013d0: 2020 2020 2020 416e 2069 6e73 7461 6e63        An instanc
-000013e0: 6520 6f66 2074 6865 2046 6564 6572 6174  e of the Federat
-000013f0: 6564 4d6f 6465 6c20 6f62 6a65 6374 2e0a  edModel object..
-00001400: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-00001410: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-00001420: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
-00001430: 2020 2020 204e 2903 da04 636f 7079 da08       N)...copy..
-00001440: 6465 6570 636f 7079 7225 0000 0029 0272  deepcopyr%...).r
-00001450: 3600 0000 7239 0000 0072 1900 0000 7219  6...r9...r....r.
-00001460: 0000 0072 1c00 0000 da17 7072 6573 6572  ...r......preser
-00001470: 7665 5f70 7265 7669 6f75 735f 6d6f 6465  ve_previous_mode
-00001480: 6c98 0000 00f3 0200 0000 100f 7a2a 4576  l...........z*Ev
-00001490: 616c 7561 7469 6f6e 5f4d 616e 6167 6572  aluation_Manager
-000014a0: 2e70 7265 7365 7276 655f 7072 6576 696f  .preserve_previo
-000014b0: 7573 5f6d 6f64 656c da0d 7570 6461 7465  us_model..update
-000014c0: 645f 6d6f 6465 6c63 0200 0000 0000 0000  d_modelc........
-000014d0: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
-000014e0: 723a 0000 0029 0261 9a01 0000 5072 6573  r:...).a....Pres
-000014f0: 6572 7665 7320 7468 6520 7570 6461 7465  erves the update
-00001500: 6420 7665 7273 696f 6e20 6f66 2074 6865  d version of the
-00001510: 2063 656e 7472 616c 206d 6f64 656c 0a20   central model. 
-00001520: 2020 2020 2020 2062 7920 636f 7079 696e         by copyin
-00001530: 6720 6974 7320 7374 7275 6374 7572 6520  g its structure 
-00001540: 616e 6420 7573 696e 6720 6974 2061 7320  and using it as 
-00001550: 616e 2061 7474 7269 6275 7465 2773 2076  an attribute's v
-00001560: 616c 7565 2e20 0a20 2020 2020 2020 2053  alue. .        S
-00001570: 686f 756c 6420 6265 2063 616c 6c65 6420  hould be called 
-00001580: 6561 6368 2074 7261 696e 696e 6720 6166  each training af
-00001590: 7465 7220 7570 6461 7469 6e67 2074 6865  ter updating the
-000015a0: 2077 6569 6768 7473 0a20 2020 2020 2020   weights.       
-000015b0: 206f 6620 7468 6520 6365 6e74 7261 6c20   of the central 
-000015c0: 6d6f 6465 6c2e 0a20 2020 2020 2020 200a  model..        .
-000015d0: 2020 2020 2020 2020 5061 7261 6d65 7465          Paramete
-000015e0: 7273 0a20 2020 2020 2020 202d 2d2d 2d2d  rs.        -----
-000015f0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7570  -----.        up
-00001600: 6461 7465 645f 6d6f 6465 6c3a 2046 6564  dated_model: Fed
-00001610: 6572 6174 6564 4d6f 6465 6c0a 2020 2020  eratedModel.    
-00001620: 2020 2020 2020 2020 416e 2069 6e73 7461          An insta
-00001630: 6e63 6520 6f66 2074 6865 2046 6564 6572  nce of the Feder
-00001640: 6174 6564 4d6f 6465 6c20 6f62 6a65 6374  atedModel object
-00001650: 2e0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
-00001660: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
-00001670: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a20  -.        None. 
-00001680: 2020 2020 2020 4e29 0372 3b00 0000 723c        N).r;...r<
-00001690: 0000 0072 2600 0000 2902 7236 0000 0072  ...r&...).r6...r
-000016a0: 3f00 0000 7219 0000 0072 1900 0000 721c  ?...r....r....r.
-000016b0: 0000 00da 1670 7265 7365 7276 655f 7570  .....preserve_up
-000016c0: 6461 7465 645f 6d6f 6465 6caa 0000 0072  dated_model....r
-000016d0: 3e00 0000 7a29 4576 616c 7561 7469 6f6e  >...z)Evaluation
-000016e0: 5f4d 616e 6167 6572 2e70 7265 7365 7276  _Manager.preserv
-000016f0: 655f 7570 6461 7465 645f 6d6f 6465 6c72  e_updated_modelr
-00001700: 2700 0000 6302 0000 0000 0000 0000 0000  '...c...........
-00001710: 0002 0000 0003 0000 0043 0000 0072 3a00  .........C...r:.
-00001720: 0000 2902 6198 0100 0050 7265 7365 7276  ..).a....Preserv
-00001730: 6573 2074 6865 204f 7074 696d 697a 6572  es the Optimizer
-00001740: 2066 726f 6d20 7468 6520 7072 6576 696f   from the previo
-00001750: 7573 2072 6f75 6e64 2062 7920 636f 7079  us round by copy
-00001760: 696e 6720 0a20 2020 2020 2020 2069 7473  ing .        its
-00001770: 2073 7472 7563 7475 7265 2061 6e64 2075   structure and u
-00001780: 7369 6e67 2069 7420 6173 2061 6e20 6174  sing it as an at
-00001790: 7472 6962 7574 6527 7320 7661 6c75 652e  tribute's value.
-000017a0: 2053 686f 756c 640a 2020 2020 2020 2020   Should.        
-000017b0: 6265 2063 616c 6c65 6420 6561 6368 2074  be called each t
-000017c0: 7261 696e 696e 6720 726f 756e 6420 6265  raining round be
-000017d0: 666f 7265 2074 6865 2070 726f 7065 7220  fore the proper 
-000017e0: 7472 6169 6e69 6e67 0a20 2020 2020 2020  training.       
-000017f0: 2063 6f6d 6d65 6e63 6573 2e0a 2020 2020   commences..    
-00001800: 2020 2020 0a20 2020 2020 2020 2050 6172      .        Par
-00001810: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
-00001820: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
-00001830: 2020 2070 7265 7669 6f75 735f 6f70 7469     previous_opti
-00001840: 6d69 7a65 723a 204f 7074 696d 697a 6572  mizer: Optimizer
-00001850: 730a 2020 2020 2020 2020 2020 2020 416e  s.            An
-00001860: 2069 6e73 7461 6e63 6520 6f66 2074 6865   instance of the
-00001870: 2061 736f 6369 6974 612e 4f70 7469 6d69   asociita.Optimi
-00001880: 7a65 7273 2063 6c61 7373 2e0a 2020 2020  zers class..    
-00001890: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-000018a0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-000018b0: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
-000018c0: 204e 2903 723b 0000 0072 3c00 0000 7227   N).r;...r<...r'
-000018d0: 0000 0029 0272 3600 0000 7227 0000 0072  ...).r6...r'...r
-000018e0: 1900 0000 7219 0000 0072 1c00 0000 da1b  ....r....r......
-000018f0: 7072 6573 6572 7665 5f70 7265 7669 6f75  preserve_previou
-00001900: 735f 6f70 7469 6d69 7a65 72bb 0000 0072  s_optimizer....r
-00001910: 3e00 0000 7a2e 4576 616c 7561 7469 6f6e  >...z.Evaluation
-00001920: 5f4d 616e 6167 6572 2e70 7265 7365 7276  _Manager.preserv
-00001930: 655f 7072 6576 696f 7573 5f6f 7074 696d  e_previous_optim
-00001940: 697a 6572 da09 6772 6164 6965 6e74 73da  izer..gradients.
-00001950: 0f6e 6f64 6573 5f69 6e5f 7361 6d70 6c65  .nodes_in_sample
-00001960: 721b 0000 0063 0400 0000 0000 0000 0000  r....c..........
-00001970: 0000 0a00 0000 0900 0000 4300 0000 73bc  ..........C...s.
-00001980: 0100 007c 006a 0072 0b7c 006a 016a 027c  ...|.j.r.|.j.j.|
-00001990: 0164 018d 0101 006e 0a7c 006a 0372 157c  .d.....n.|.j.r.|
-000019a0: 006a 016a 047c 0164 018d 0101 007c 006a  .j.j.|.d.....|.j
-000019b0: 0572 2e7c 037c 006a 0664 0219 0076 0072  .r.|.|.j.d...v.r
-000019c0: 2e7c 006a 076a 087c 017c 027c 037c 006a  .|.j.j.|.|.|.|.j
-000019d0: 097c 006a 0a7c 006a 0b64 038d 0601 007c  .|.j.|.j.d.....|
-000019e0: 006a 0c72 d87c 037c 006a 0664 0419 0076  .j.r.|.|.j.d...v
-000019f0: 0072 da7c 006a 0d72 4d7c 006a 0e6a 0f7c  .r.|.j.rM|.j.j.|
-00001a00: 017c 027c 037c 006a 097c 006a 0b7c 006a  .|.|.|.j.|.j.|.j
-00001a10: 107c 006a 1164 058d 077d 046e 0f7c 006a  .|.j.d...}.n.|.j
-00001a20: 0e6a 127c 017c 027c 037c 006a 097c 006a  .j.|.|.|.|.j.|.j
-00001a30: 0b7c 006a 1064 068d 067d 047c 006a 1072  .|.j.d...}.|.j.r
-00001a40: dc7c 0364 076b 0272 a274 1374 146a 15a0  .|.d.k.r.t.t.j..
-00001a50: 167c 006a 1764 08a1 0264 0964 0a64 0b8d  .|.j.d...d.d.d..
-00001a60: 038f 287d 0567 0064 0ca2 017d 0674 18a0  ..(}.g.d...}.t..
-00001a70: 197c 05a1 017d 077c 07a0 1a7c 06a1 0101  .|...}.|...|....
-00001a80: 007c 04a0 1ba1 0044 005d 0c5c 027d 087d  .|.....D.].\.}.}
-00001a90: 097c 07a0 1a7c 087c 097c 0367 03a1 0101  .|...|.|.|.g....
-00001aa0: 0071 8357 0064 0d04 0004 0083 0301 0064  .q.W.d.........d
-00001ab0: 0d53 0031 0073 9b77 0101 0001 0001 0059  .S.1.s.w.......Y
-00001ac0: 0001 0064 0d53 0074 1374 146a 15a0 167c  ...d.S.t.t.j...|
-00001ad0: 006a 1764 08a1 0264 0964 0a64 0b8d 038f  .j.d...d.d.d....
-00001ae0: 1f7d 0574 18a0 197c 05a1 017d 077c 04a0  .}.t...|...}.|..
-00001af0: 1ba1 0044 005d 0c5c 027d 087d 097c 07a0  ...D.].\.}.}.|..
-00001b00: 1a7c 087c 097c 0367 03a1 0101 0071 b957  .|.|.|.g.....q.W
-00001b10: 0064 0d04 0004 0083 0301 0064 0d53 0031  .d.........d.S.1
-00001b20: 0073 d177 0101 0001 0001 0059 0001 0064  .s.w.......Y...d
-00001b30: 0d53 0064 0d53 0064 0d53 0064 0d53 0029  .S.d.S.d.S.d.S.)
-00001b40: 0e61 ad02 0000 4d65 7468 6f64 2075 7365  .a....Method use
-00001b50: 6420 746f 2074 7261 636b 5f72 6573 756c  d to track_resul
-00001b60: 7473 2061 6674 6572 2065 6163 6820 7472  ts after each tr
-00001b70: 6169 6e69 6e67 2072 6f75 6e64 2e0a 2020  aining round..  
-00001b80: 2020 2020 2020 4265 6361 7573 6520 7468        Because th
-00001b90: 6520 4f72 6368 6573 7472 6174 6f72 2061  e Orchestrator a
-00001ba0: 6273 7472 6163 7469 6f6e 2073 686f 756c  bstraction shoul
-00001bb0: 6420 6265 2066 7265 6520 6f66 2061 6e79  d be free of any
-00001bc0: 0a20 2020 2020 2020 2075 6e6e 6563 6573  .        unneces
-00001bd0: 7361 7279 2065 6e63 756d 6272 616e 6365  sary encumbrance
-00001be0: 2c20 7468 6520 4576 616c 7561 7469 6f6e  , the Evaluation
-00001bf0: 5f4d 616e 6167 6572 2e74 7261 636b 5f72  _Manager.track_r
-00001c00: 6573 756c 7473 2829 0a20 2020 2020 2020  esults().       
-00001c10: 2077 696c 6c20 7461 6b65 2063 6172 6520   will take care 
-00001c20: 6f66 2061 6e79 2072 6573 756c 7420 7072  of any result pr
-00001c30: 6573 6572 7661 7469 6f6e 2061 6e64 2073  eservation and s
-00001c40: 636f 7265 2063 616c 6375 6c61 7469 6f6e  core calculation
-00001c50: 2074 6861 7420 0a20 2020 2020 2020 206d   that .        m
-00001c60: 7573 7420 6265 2064 6f6e 6520 696e 206f  ust be done in o
-00001c70: 7264 6572 2074 6f20 6573 7461 626c 6973  rder to establis
-00001c80: 6820 7468 6520 7265 7375 6c74 732e 0a20  h the results.. 
-00001c90: 2020 2020 2020 200a 2020 2020 2020 2020         .        
-00001ca0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00001cb0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00001cc0: 2020 2020 2020 6772 6164 6965 6e74 733a        gradients:
-00001cd0: 204f 7264 6572 6564 4469 6374 0a20 2020   OrderedDict.   
-00001ce0: 2020 2020 2020 2020 2041 6e20 4f72 6465           An Orde
-00001cf0: 7265 6444 6963 7420 636f 6e74 6169 6e69  redDict containi
-00001d00: 6e67 2067 7261 6469 656e 7473 206f 6620  ng gradients of 
-00001d10: 7468 6520 7361 6d70 6c65 6420 6e6f 6465  the sampled node
-00001d20: 732e 0a20 2020 2020 2020 206e 6f64 6573  s..        nodes
-00001d30: 5f69 6e5f 7361 6d70 6c65 3a20 6c69 7374  _in_sample: list
-00001d40: 0a20 2020 2020 2020 2020 2020 2041 206c  .            A l
-00001d50: 6973 7420 636f 6e74 6169 6e69 6e67 2069  ist containing i
-00001d60: 6427 7320 6f66 2074 6865 206e 6f64 6573  d's of the nodes
-00001d70: 2074 6861 7420 7765 7265 2073 616d 706c   that were sampl
-00001d80: 6564 2e0a 2020 2020 2020 2020 6974 6572  ed..        iter
-00001d90: 6174 696f 6e3a 2069 6e74 0a20 2020 2020  ation: int.     
-00001da0: 2020 2020 2020 2054 6865 2063 7572 7265         The curre
-00001db0: 6e74 2069 7465 7261 7469 6f6e 2e0a 2020  nt iteration..  
-00001dc0: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
-00001dd0: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
-00001de0: 2020 2020 2020 4e6f 6e65 0a20 2020 2020        None.     
-00001df0: 2020 2029 0172 4200 0000 7212 0000 0029     ).rB...r....)
-00001e00: 0672 4200 0000 7243 0000 0072 1b00 0000  .rB...rC...r....
-00001e10: da09 6f70 7469 6d69 7a65 725a 0b66 696e  ..optimizerZ.fin
-00001e20: 616c 5f6d 6f64 656c 7239 0000 0072 1400  al_modelr9...r..
-00001e30: 0000 2907 7242 0000 0072 4300 0000 721b  ..).rB...rC...r.
-00001e40: 0000 0072 4400 0000 7239 0000 00da 1172  ...rD...r9.....r
-00001e50: 6574 7572 6e5f 636f 616c 6974 696f 6e73  eturn_coalitions
-00001e60: 7224 0000 0029 0672 4200 0000 7243 0000  r$...).rB...rC..
-00001e70: 0072 1b00 0000 7244 0000 0072 3900 0000  .r....rD...r9...
-00001e80: 7245 0000 0072 0100 0000 7a14 636f 6c5f  rE...r....z.col_
-00001e90: 7661 6c75 6573 5f64 6562 7567 2e63 7376  values_debug.csv
-00001ea0: 7a02 612b da00 a901 da07 6e65 776c 696e  z.a+......newlin
-00001eb0: 6529 03da 0963 6f61 6c69 7469 6f6e da05  e)...coalition..
-00001ec0: 7661 6c75 6572 1b00 0000 4e29 1c72 2900  valuer....N).r).
-00001ed0: 0000 722f 0000 005a 0d74 7261 636b 5f73  ..r/...Z.track_s
-00001ee0: 6861 706c 6579 722c 0000 005a 0974 7261  hapleyr,...Z.tra
-00001ef0: 636b 5f6c 6f6f 722d 0000 0072 1800 0000  ck_loor-...r....
-00001f00: 7230 0000 005a 0a75 7064 6174 655f 7073  r0...Z.update_ps
-00001f10: 6972 2700 0000 7226 0000 0072 2500 0000  ir'...r&...r%...
-00001f20: 722e 0000 0072 3500 0000 7232 0000 005a  r....r5...r2...Z
-00001f30: 1275 7064 6174 655f 7368 6170 5f6d 756c  .update_shap_mul
-00001f40: 7469 7072 2200 0000 7224 0000 005a 0b75  tipr"...r$...Z.u
-00001f50: 7064 6174 655f 7368 6170 da04 6f70 656e  pdate_shap..open
-00001f60: 7233 0000 00da 0470 6174 68da 046a 6f69  r3.....path..joi
-00001f70: 6e72 2300 0000 da03 6373 76da 0677 7269  nr#.....csv..wri
-00001f80: 7465 72da 0877 7269 7465 726f 77da 0569  ter..writerow..i
-00001f90: 7465 6d73 290a 7236 0000 0072 4200 0000  tems).r6...rB...
-00001fa0: 7243 0000 0072 1b00 0000 5a0c 6465 6275  rC...r....Z.debu
-00001fb0: 675f 7661 6c75 6573 da08 6373 765f 6669  g_values..csv_fi
-00001fc0: 6c65 da0b 6669 656c 645f 6e61 6d65 73da  le..field_names.
-00001fd0: 0a63 7376 5f77 7269 7465 72da 0363 6f6c  .csv_writer..col
-00001fe0: 724a 0000 0072 1900 0000 7219 0000 0072  rJ...r....r....r
-00001ff0: 1c00 0000 da0d 7472 6163 6b5f 7265 7375  ......track_resu
-00002000: 6c74 73cd 0000 0073 6400 0000 0618 1001  lts....sd.......
-00002010: 0601 0e01 0603 0e01 0801 0201 0201 0401  ................
-00002020: 0401 0401 06fb 0607 0e01 0601 0801 0201  ................
-00002030: 0201 0401 0401 0401 0401 08fa 0808 0201  ................
-00002040: 0201 0401 0401 0401 06fb 0608 0801 1c01  ................
-00002050: 0801 0a01 0a01 1001 1201 02ff 22fc 1c07  ............"...
-00002060: 0a01 1001 1201 02ff 22fe 04e4 0401 0412  ........".......
-00002070: 7a20 4576 616c 7561 7469 6f6e 5f4d 616e  z Evaluation_Man
-00002080: 6167 6572 2e74 7261 636b 5f72 6573 756c  ager.track_resul
-00002090: 7473 724c 0000 0063 0200 0000 0000 0000  tsrL...c........
-000020a0: 0000 0000 0f00 0000 0900 0000 4300 0000  ............C...
-000020b0: 73b4 0100 0069 0069 0064 019c 027d 027c  s....i.i.d...}.|
-000020c0: 006a 0072 0a74 0182 017c 006a 0272 0f74  .j.r.t...|.j.r.t
-000020d0: 0182 017c 006a 0372 257c 006a 04a0 05a1  ...|.j.r%|.j....
-000020e0: 005c 027d 037d 047c 037c 0264 0219 0064  .\.}.}.|.|.d...d
-000020f0: 033c 007c 047c 0264 0419 0064 053c 007c  .<.|.|.d...d.<.|
-00002100: 006a 0672 3b7c 006a 07a0 08a1 005c 027d  .j.r;|.j.....\.}
-00002110: 057d 067c 057c 0264 0219 0064 063c 007c  .}.|.|.d...d.<.|
-00002120: 067c 0264 0419 0064 073c 007c 006a 0964  .|.d...d.<.|.j.d
-00002130: 086b 0272 927c 0264 0219 00a0 0aa1 0044  .k.r.|.d.......D
-00002140: 005d 4b5c 027d 077d 0874 0b6a 0ca0 0d7c  .]K\.}.}.t.j...|
-00002150: 0174 0e7c 0783 0164 0917 00a1 027d 097c  .t.|...d.....}.|
-00002160: 006a 0f7d 0a7c 0aa0 1064 0aa1 0101 0074  .j.}.|...d.....t
-00002170: 117c 0964 0b64 0c64 0d8d 038f 257d 0b74  .|.d.d.d....%}.t
-00002180: 126a 137c 0b7c 0a64 0e8d 027d 0c7c 0ca0  .j.|.|.d...}.|..
-00002190: 14a1 0001 007c 08a0 0aa1 0044 005d 0d5c  .....|.....D.].\
-000021a0: 027d 0d7d 0e7c 0d7c 0e64 0a3c 007c 0ca0  .}.}.|.|.d.<.|..
-000021b0: 157c 0ea1 0101 0071 7457 0064 0f04 0004  .|.....qtW.d....
-000021c0: 0083 0301 006e 0831 0073 8c77 0101 0001  .....n.1.s.w....
-000021d0: 0001 0059 0001 0071 467c 006a 1664 086b  ...Y...qF|.j.d.k
-000021e0: 0272 d87c 0264 0419 00a0 0aa1 0044 005d  .r.|.d.......D.]
-000021f0: 3a5c 027d 077d 0874 0b6a 0ca0 0d7c 0174  :\.}.}.t.j...|.t
-00002200: 0e7c 0783 0164 0917 00a1 027d 097c 08a0  .|...d.....}.|..
-00002210: 17a1 007d 0a74 117c 0964 0b64 0c64 0d8d  ...}.t.|.d.d.d..
-00002220: 038f 187d 0b74 126a 137c 0b7c 0a64 0e8d  ...}.t.j.|.|.d..
-00002230: 027d 0c7c 0ca0 14a1 0001 007c 0ca0 157c  .}.|.......|...|
-00002240: 08a1 0101 0057 0064 0f04 0004 0083 0301  .....W.d........
-00002250: 006e 0831 0073 d277 0101 0001 0001 0059  .n.1.s.w.......Y
-00002260: 0001 0071 9d7c 0253 0029 1061 4a02 0000  ...q.|.S.).aJ...
-00002270: 4d65 7468 6f64 2075 7365 6420 746f 2066  Method used to f
-00002280: 696e 616c 697a 6520 7468 6520 7472 6163  inalize the trac
-00002290: 6b69 6e67 2061 7420 7468 6520 656e 6420  king at the end 
-000022a0: 6f66 2074 6865 2074 7261 696e 696e 672e  of the training.
-000022b0: 0a20 2020 2020 2020 2042 6563 6175 7365  .        Because
-000022c0: 2074 6865 204f 7263 6865 7374 7261 746f   the Orchestrato
-000022d0: 7220 6162 7374 7261 6374 696f 6e20 7368  r abstraction sh
-000022e0: 6f75 6c64 2062 6520 6672 6565 206f 6620  ould be free of 
-000022f0: 616e 790a 2020 2020 2020 2020 756e 6e65  any.        unne
-00002300: 6365 7373 6172 7920 656e 6375 6d62 7261  cessary encumbra
-00002310: 6e63 652c 2061 6c6c 2074 6865 206f 7074  nce, all the opt
-00002320: 696f 6e73 2063 6f6e 6669 6775 7269 6e67  ions configuring
-00002330: 2074 6865 2062 6568 6176 696f 7572 0a20   the behaviour. 
-00002340: 2020 2020 2020 206f 6620 7468 6520 6669         of the fi
-00002350: 6e61 6c69 7a65 5f74 7261 636b 696e 6720  nalize_tracking 
-00002360: 6d65 7468 6f64 2c20 7368 6f75 6c64 2062  method, should b
-00002370: 6520 7072 652d 636f 6e66 6967 7572 6564  e pre-configured
-00002380: 2061 7420 7468 6520 7374 6167 650a 2020   at the stage.  
-00002390: 2020 2020 2020 6f66 2074 6865 2045 7661        of the Eva
-000023a0: 6c75 6174 696f 6e5f 4d61 6e61 6765 7220  luation_Manager 
-000023b0: 696e 7374 616e 6365 2069 6e69 7469 616c  instance initial
-000023c0: 697a 6174 696f 6e2e 2020 0a20 2020 2020  ization.  .     
-000023d0: 2020 200a 2020 2020 2020 2020 5061 7261     .        Para
-000023e0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
-000023f0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
-00002400: 2020 7061 7468 3a20 7374 722c 2064 6566    path: str, def
-00002410: 6175 6c74 2074 6f20 4e6f 6e65 0a20 2020  ault to None.   
-00002420: 2020 2020 2020 2020 2061 2073 7472 696e           a strin
-00002430: 6720 6f72 2050 6174 682d 6c69 6b65 206f  g or Path-like o
-00002440: 626a 6563 7420 746f 2074 6865 2064 6972  bject to the dir
-00002450: 6563 746f 7279 2069 6e20 7768 6963 6820  ectory in which 
-00002460: 7265 7375 6c74 730a 2020 2020 2020 2020  results.        
-00002470: 2020 2020 7368 6f75 6c64 2062 6520 7361      should be sa
-00002480: 7665 642e 0a20 2020 2020 2020 2052 6574  ved..        Ret
-00002490: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
-000024a0: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
-000024b0: 650a 2020 2020 2020 2020 2902 da07 7061  e.        )...pa
-000024c0: 7274 6961 6cda 0466 756c 6c72 5700 0000  rtial..fullrW...
-000024d0: da0b 7061 7274 6961 6c5f 7073 6972 5800  ..partial_psirX.
-000024e0: 0000 da03 7073 69da 0c70 6172 7469 616c  ....psi..partial
-000024f0: 5f73 6861 70da 0473 6861 7054 7a04 2e63  _shap..shapTz..c
-00002500: 7376 721b 0000 007a 0277 2b72 4600 0000  svr....z.w+rF...
-00002510: 7247 0000 0029 01da 0a66 6965 6c64 6e61  rG...)...fieldna
-00002520: 6d65 734e 2918 7229 0000 0072 2b00 0000  mesN).r)...r+...
-00002530: 722c 0000 0072 2d00 0000 7230 0000 005a  r,...r-...r0...Z
-00002540: 1363 616c 6375 6c61 7465 5f66 696e 616c  .calculate_final
-00002550: 5f70 7369 722e 0000 0072 3200 0000 5a14  _psir....r2...Z.
-00002560: 6361 6c63 756c 6174 655f 6669 6e61 6c5f  calculate_final_
-00002570: 7368 6170 7216 0000 0072 5100 0000 7233  shapr....rQ...r3
-00002580: 0000 0072 4c00 0000 724d 0000 00da 0373  ...rL...rM.....s
-00002590: 7472 720c 0000 0072 2a00 0000 724b 0000  trr....r*...rK..
-000025a0: 0072 4e00 0000 da0a 4469 6374 5772 6974  .rN.....DictWrit
-000025b0: 6572 da0b 7772 6974 6568 6561 6465 7272  er..writeheaderr
-000025c0: 5000 0000 7217 0000 00da 046b 6579 7329  P...r......keys)
-000025d0: 0f72 3600 0000 724c 0000 00da 0772 6573  .r6...rL.....res
-000025e0: 756c 7473 7259 0000 0072 5a00 0000 725b  ultsrY...rZ...r[
-000025f0: 0000 0072 5c00 0000 da06 6d65 7472 6963  ...r\.....metric
-00002600: da06 7661 6c75 6573 5a06 735f 7061 7468  ..valuesZ.s_path
-00002610: 7253 0000 0072 5200 0000 7254 0000 0072  rS...rR...rT...r
-00002620: 1b00 0000 da03 726f 7772 1900 0000 7219  ......rowr....r.
-00002630: 0000 0072 1c00 0000 da11 6669 6e61 6c69  ...r......finali
-00002640: 7a65 5f74 7261 636b 696e 6715 0100 0073  ze_tracking....s
-00002650: 4c00 0000 0a11 0602 0401 0602 0401 0602  L...............
-00002660: 0e01 0c01 0c01 0602 0e01 0c01 0c01 0a02  ................
-00002670: 1401 1601 0601 0a01 1001 0e01 0801 1001  ................
-00002680: 0801 0c01 02fe 1cfd 0280 0a07 1401 1601  ................
-00002690: 0801 1001 0e01 0801 0c01 1cfd 0280 0404  ................
-000026a0: 7a24 4576 616c 7561 7469 6f6e 5f4d 616e  z$Evaluation_Man
-000026b0: 6167 6572 2e66 696e 616c 697a 655f 7472  ager.finalize_tr
-000026c0: 6163 6b69 6e67 2902 4e4e 2901 4e29 11da  acking).NN).N)..
-000026d0: 085f 5f6e 616d 655f 5fda 0a5f 5f6d 6f64  .__name__..__mod
-000026e0: 756c 655f 5fda 0c5f 5f71 7561 6c6e 616d  ule__..__qualnam
-000026f0: 655f 5fda 075f 5f64 6f63 5f5f da04 6469  e__..__doc__..di
-00002700: 6374 7205 0000 00da 046c 6973 74da 0369  ctr......list..i
-00002710: 6e74 7238 0000 0072 3d00 0000 7240 0000  ntr8...r=...r@..
-00002720: 0072 0700 0000 7241 0000 0072 0800 0000  .r....rA...r....
-00002730: 7256 0000 0072 5e00 0000 7266 0000 0072  rV...r^...rf...r
-00002740: 1900 0000 7219 0000 0072 1900 0000 721c  ....r....r....r.
-00002750: 0000 0072 0900 0000 0d00 0000 7346 0000  ...r........sF..
-00002760: 0008 0004 0102 0e02 0104 fc02 0102 ff02  ................
-00002770: 0202 fe02 0302 fd02 0402 fc02 040a fc02  ................
-00002780: 7f02 010a ff02 1202 010a ff02 1102 010a  ................
-00002790: ff02 1202 0102 ff02 0202 fe02 030a fd02  ................
-000027a0: 4904 ff02 010e ff72 0900 0000 2911 5a2a  I......r....).Z*
-000027b0: 6173 6f63 6969 7461 2e63 6f6d 706f 6e65  asociita.compone
-000027c0: 6e74 732e 6576 616c 7561 746f 722e 6f72  nts.evaluator.or
-000027d0: 5f65 7661 6c75 6174 6f72 7202 0000 005a  _evaluatorr....Z
-000027e0: 2e61 736f 6369 6974 612e 636f 6d70 6f6e  .asociita.compon
-000027f0: 656e 7473 2e65 7661 6c75 6174 6f72 2e73  ents.evaluator.s
-00002800: 616d 706c 655f 6576 616c 7561 746f 7272  ample_evaluatorr
-00002810: 0300 0000 7204 0000 00da 2761 736f 6369  ....r.....'asoci
-00002820: 6974 612e 6d6f 6465 6c73 2e70 7974 6f72  ita.models.pytor
-00002830: 6368 2e66 6564 6572 6174 6564 5f6d 6f64  ch.federated_mod
-00002840: 656c 7205 0000 005a 2661 736f 6369 6974  elr....Z&asociit
-00002850: 612e 6578 6365 7074 696f 6e73 2e65 7661  a.exceptions.eva
-00002860: 6c75 6174 6f72 6578 6365 7074 696f 6e72  luatorexceptionr
-00002870: 0600 0000 da19 6173 6f63 6969 7461 2e75  ......asociita.u
-00002880: 7469 6c73 2e6f 7074 696d 697a 6572 7372  tils.optimizersr
-00002890: 0700 0000 da0b 636f 6c6c 6563 7469 6f6e  ......collection
-000028a0: 7372 0800 0000 723b 0000 0072 3300 0000  sr....r;...r3...
-000028b0: 724e 0000 0072 0900 0000 7219 0000 0072  rN...r....r....r
-000028c0: 1900 0000 7219 0000 0072 1c00 0000 da08  ....r....r......
-000028d0: 3c6d 6f64 756c 653e 0100 0000 7316 0000  <module>....s...
-000028e0: 000c 000c 010c 010c 010c 010c 010c 0108  ................
-000028f0: 0108 0108 0112 03                        .......
+00000080: 0100 6400 6408 6c0d 6d0e 5a0e 0100 6400  ..d.d.l.m.Z...d.
+00000090: 6409 6c0f 5a0f 6400 6409 6c10 5a10 6400  d.l.Z.d.d.l.Z.d.
+000000a0: 6409 6c11 5a11 4700 640a 640b 8400 640b  d.l.Z.G.d.d...d.
+000000b0: 8302 5a12 6409 5300 290c e900 0000 0029  ..Z.d.S.)......)
+000000c0: 01da 0c4f 525f 4576 616c 7561 746f 7229  ...OR_Evaluator)
+000000d0: 01da 044c 5341 4129 01da 1053 616d 706c  ...LSAA)...Sampl
+000000e0: 655f 4576 616c 7561 746f 7229 01da 1853  e_Evaluator)...S
+000000f0: 616d 706c 655f 5368 6170 6c65 795f 4576  ample_Shapley_Ev
+00000100: 616c 7561 746f 7229 01da 0e46 6564 6572  aluator)...Feder
+00000110: 6174 6564 4d6f 6465 6c29 01da 1f53 616d  atedModel)...Sam
+00000120: 706c 655f 4576 616c 7561 746f 725f 496e  ple_Evaluator_In
+00000130: 6974 5f45 7863 6570 7469 6f6e 2901 da0a  it_Exception)...
+00000140: 4f70 7469 6d69 7a65 7273 2901 da0b 4f72  Optimizers)...Or
+00000150: 6465 7265 6444 6963 744e 6300 0000 0000  deredDictNc.....
+00000160: 0000 0000 0000 0000 0000 000b 0000 0040  ...............@
+00000170: 0000 0073 8600 0000 6500 5a01 6400 5a02  ...s....e.Z.d.Z.
+00000180: 6401 5a03 0902 0902 641b 6403 6504 6404  d.Z.....d.d.e.d.
+00000190: 6505 6405 6506 6406 6507 6407 6402 660a  e.d.e.d.e.d.d.f.
+000001a0: 6408 6409 8405 5a08 640a 6505 6602 640b  d.d...Z.d.e.f.d.
+000001b0: 640c 8404 5a09 640d 6505 6602 640e 640f  d...Z.d.e.f.d.d.
+000001c0: 8404 5a0a 6410 650b 6602 6411 6412 8404  ..Z.d.e.f.d.d...
+000001d0: 5a0c 6413 650d 6414 6506 6415 6507 6606  Z.d.e.d.e.d.e.f.
+000001e0: 6416 6417 8404 5a0e 0902 641c 6418 650f  d.d...Z...d.d.e.
+000001f0: 6602 6419 641a 8405 5a10 6402 5300 291d  f.d.d...Z.d.S.).
+00000200: da12 4576 616c 7561 7469 6f6e 5f4d 616e  ..Evaluation_Man
+00000210: 6167 6572 61bb 0200 0045 7661 6c75 6174  agera....Evaluat
+00000220: 696f 6e20 4d61 6e61 6765 7220 656e 6361  ion Manager enca
+00000230: 7073 756c 6174 6573 2074 6865 2077 686f  psulates the who
+00000240: 6c65 2070 726f 6365 7373 206f 6620 6173  le process of as
+00000250: 7365 7373 696e 6720 7468 6520 6d61 7267  sessing the marg
+00000260: 696e 616c 0a20 2020 2063 6c69 656e 7473  inal.    clients
+00000270: 2720 636f 6e74 7269 6275 7469 6f6e 732c  ' contributions,
+00000280: 2073 6f20 7468 6520 6f72 6368 6573 7472   so the orchestr
+00000290: 6174 6f72 2063 6f64 6520 6973 2066 7265  ator code is fre
+000002a0: 6520 6f66 2061 6e79 2065 6e63 756d 6272  e of any encumbr
+000002b0: 616e 6365 0a20 2020 2063 6f6e 6e65 6374  ance.    connect
+000002c0: 6564 2074 6f20 6974 2e20 4576 616c 7561  ed to it. Evalua
+000002d0: 7469 6f6e 204d 616e 6167 6572 206c 6966  tion Manager lif
+000002e0: 652d 6379 636c 6520 6973 2073 706c 6974  e-cycle is split
+000002f0: 7465 6420 696e 746f 2066 6f75 7220 6469  ted into four di
+00000300: 6666 6572 656e 740a 2020 2020 7374 6167  fferent.    stag
+00000310: 6573 3a20 696e 6974 6961 6c69 7a61 7469  es: initializati
+00000320: 6f6e 2c20 7072 6573 6572 7661 7469 6f6e  on, preservation
+00000330: 2c20 7472 6163 6b69 6e67 2061 6e64 2066  , tracking and f
+00000340: 696e 616c 697a 6174 696f 6e2e 2049 6e69  inalization. Ini
+00000350: 7469 616c 697a 6174 696f 6e0a 2020 2020  tialization.    
+00000360: 7265 7175 6972 6573 2061 2064 6963 7469  requires a dicti
+00000370: 6f6e 6172 7920 636f 6e74 6169 6e69 6e67  onary containing
+00000380: 2061 6c6c 2074 6865 2072 656c 6576 616e   all the relevan
+00000390: 7420 7365 7474 696e 6773 2e20 5072 6573  t settings. Pres
+000003a0: 6572 7661 7469 6f6e 2073 686f 756c 640a  ervation should.
+000003b0: 2020 2020 6265 2063 616c 6c65 6420 6561      be called ea
+000003c0: 6368 2072 6f75 6e64 2062 6566 6f72 6520  ch round before 
+000003d0: 7468 6520 7472 6169 6e69 6e67 2063 6f6d  the training com
+000003e0: 6d65 6e63 6573 2028 736f 2074 6865 2065  mences (so the e
+000003f0: 7661 6c75 6174 696f 6e20 6d61 6e61 6765  valuation manage
+00000400: 720a 2020 2020 6861 7320 6c61 7374 2073  r.    has last s
+00000410: 6574 206f 6620 7765 6967 6874 7320 616e  et of weights an
+00000420: 6420 6d6f 6d65 6e74 756d 2069 6e66 6f72  d momentum infor
+00000430: 6d61 7469 6f6e 292e 2054 7261 636b 696e  mation). Trackin
+00000440: 6720 7368 6f75 6c64 2062 6520 6361 6c6c  g should be call
+00000450: 6564 2065 6163 680a 2020 2020 726f 756e  ed each.    roun
+00000460: 6420 746f 2063 6f6d 7075 7465 2064 6966  d to compute dif
+00000470: 6665 7265 6e74 206d 6574 7269 6373 2e20  ferent metrics. 
+00000480: 4669 6e61 6c69 7a61 7469 6f6e 2063 616e  Finalization can
+00000490: 2062 6520 6361 6c6c 6564 2061 7420 7468   be called at th
+000004a0: 6520 656e 6420 6f66 2074 6865 0a20 2020  e end of the.   
+000004b0: 206c 6966 652d 6379 636c 6520 746f 2070   life-cycle to p
+000004c0: 7265 7365 7276 6520 7468 6520 7265 7375  reserve the resu
+000004d0: 6c74 732e 4eda 0873 6574 7469 6e67 73da  lts.N..settings.
+000004e0: 056d 6f64 656c da05 6e6f 6465 73da 0a69  .model..nodes..i
+000004f0: 7465 7261 7469 6f6e 73da 0672 6574 7572  terations..retur
+00000500: 6e63 0500 0000 0000 0000 0000 0000 0700  nc..............
+00000510: 0000 0a00 0000 0300 0000 7388 0200 007c  ..........s....|
+00000520: 017c 005f 0064 017c 005f 0164 017c 005f  .|._.d.|._.d.|._
+00000530: 0264 017c 005f 037c 037c 005f 0467 007c  .d.|._.|.|._.g.|
+00000540: 005f 057c 01a0 0664 02a1 0172 2264 037c  ._.|...d...r"d.|
+00000550: 005f 077c 006a 05a0 0864 04a1 0101 0074  ._.|.j...d.....t
+00000560: 0982 0164 057c 005f 077c 01a0 0664 06a1  ...d.|._.|...d..
+00000570: 0172 3564 037c 005f 0a7c 006a 05a0 0864  .r5d.|._.|.j...d
+00000580: 07a1 0101 0074 0982 0164 057c 005f 0a7c  .....t...d.|._.|
+00000590: 01a0 0664 08a1 0172 4764 037c 005f 0b7c  ...d...rGd.|._.|
+000005a0: 006a 05a0 0864 09a1 0101 006e 0364 057c  .j...d.....n.d.|
+000005b0: 005f 0b7c 01a0 0664 0aa1 0172 5964 037c  ._.|...d...rYd.|
+000005c0: 005f 0c7c 006a 05a0 0864 0ba1 0101 006e  ._.|.j...d.....n
+000005d0: 0364 057c 005f 0c7c 01a0 0664 0ca1 0172  .d.|._.|...d...r
+000005e0: 6b64 037c 005f 0d7c 006a 05a0 0864 0ca1  kd.|._.|.j...d..
+000005f0: 0101 006e 0364 057c 005f 0d7c 0164 0d19  ...n.d.|._.|.d..
+00000600: 00a0 0664 0ea1 0172 7964 037c 005f 0e6e  ...d...ryd.|._.n
+00000610: 0364 057c 005f 0e7c 0164 0d19 00a0 0664  .d.|._.|.d.....d
+00000620: 0fa1 0172 8664 037c 005f 0f7c 006a 0773  ...r.d.|._.|.j.s
+00000630: 8c7c 006a 0a72 9374 107c 017c 0264 108d  .|.j.r.t.|.|.d..
+00000640: 027c 005f 117c 006a 0b64 036b 0272 b07a  .|._.|.j.d.k.r.z
+00000650: 0974 127c 0388 0064 118d 027c 005f 1357  .t.|...d...|._.W
+00000660: 006e 0e04 0074 1479 af01 007d 0501 007a  .n...t.y...}...z
+00000670: 0274 1582 0164 017d 057e 0577 0177 007c  .t...d.}.~.w.w.|
+00000680: 006a 0c64 036b 0272 cd7a 0974 167c 0388  .j.d.k.r.z.t.|..
+00000690: 0064 118d 027c 005f 1757 006e 0e04 0074  .d...|._.W.n...t
+000006a0: 1479 cc01 007d 0501 007a 0274 1582 0164  .y...}...z.t...d
+000006b0: 017d 057e 0577 0177 007c 006a 0d64 036b  .}.~.w.w.|.j.d.k
+000006c0: 0272 fa7a 0e74 187c 0388 0064 118d 027c  .r.z.t.|...d...|
+000006d0: 005f 197c 0164 1219 007c 005f 1a57 006e  ._.|.d...|._.W.n
+000006e0: 1904 0074 1479 ed01 007d 0501 007a 0182  ...t.y...}...z..
+000006f0: 0064 017d 057e 0577 0104 0074 1b79 f901  .d.}.~.w...t.y..
+00000700: 007d 0601 007a 0182 0064 017d 067e 0677  .}...z...d.}.~.w
+00000710: 0177 007c 01a0 0664 13a1 0190 0172 067c  .w.|...d.....r.|
+00000720: 0164 1319 007c 005f 1c6e 0b87 0066 0164  .d...|._.n...f.d
+00000730: 1464 1584 087c 006a 0544 0083 017c 005f  .d...|.j.D...|._
+00000740: 1c7c 01a0 0664 16a1 0190 0172 2c64 037c  .|...d.....r,d.|
+00000750: 005f 1d7c 01a0 0664 17a1 0190 0172 267c  ._.|...d.....r&|
+00000760: 0164 1819 007c 005f 1e6e 0974 1fa0 20a1  .d...|._.n.t.. .
+00000770: 007c 005f 1e6e 0364 057c 005f 1d7c 01a0  .|._.n.d.|._.|..
+00000780: 0664 19a1 0190 0172 3a64 057c 005f 2164  .d.....r:d.|._!d
+00000790: 0153 0064 037c 005f 217c 0164 1a19 007c  .S.d.|._!|.d...|
+000007a0: 005f 2264 0153 0029 1b61 3106 0000 4d61  ._"d.S.).a1...Ma
+000007b0: 6e61 6765 7320 7468 6520 7072 6f63 6573  nages the proces
+000007c0: 7320 6f66 2065 7661 6c75 6174 696f 6e2e  s of evaluation.
+000007d0: 2043 7265 6174 6573 2061 6e20 696e 7374   Creates an inst
+000007e0: 616e 6365 206f 6620 4576 616c 7561 7469  ance of Evaluati
+000007f0: 6f6e 5f4d 616e 6167 6572 200a 2020 2020  on_Manager .    
+00000800: 2020 2020 6f62 6a65 6374 2c20 7468 6174      object, that
+00000810: 2063 6f6e 7472 6f6c 7320 616c 6c20 7468   controls all th
+00000820: 6520 696e 7374 616e 6365 7320 7468 6174  e instances that
+00000830: 2070 6572 666f 726d 2065 7661 6c75 6174   perform evaluat
+00000840: 696f 6e2e 2045 7661 6c75 6174 696f 6e0a  ion. Evaluation.
+00000850: 2020 2020 2020 2020 4d61 6e61 6765 7220          Manager 
+00000860: 6f70 6572 6174 6f72 6573 206f 6e20 2766  operatores on 'f
+00000870: 6c61 6773 2720 7468 6174 2061 7265 2072  lags' that are r
+00000880: 6570 7265 7365 6e74 6564 2061 7320 626f  epresented as bo
+00000890: 6c65 616e 2061 7474 7269 6275 7465 7320  lean attributes 
+000008a0: 6f66 2074 6865 0a20 2020 2020 2020 2069  of the.        i
+000008b0: 6e73 7461 6e63 6520 6f66 2074 6865 2043  nstance of the C
+000008c0: 6c61 7373 2e20 5468 6520 7661 6c75 6520  lass. The value 
+000008d0: 6f66 2066 6c61 6773 2069 7320 6469 6374  of flags is dict
+000008e0: 6174 6564 2062 7920 7468 6520 636f 7272  ated by the corr
+000008f0: 6573 706f 6e64 696e 6720 7661 6c75 650a  esponding value.
+00000900: 2020 2020 2020 2020 7573 6564 2069 6e20          used in 
+00000910: 7468 6520 7365 7474 696e 6773 2e20 4769  the settings. Gi
+00000920: 7669 6e67 2061 6e20 6578 616d 706c 652c  ving an example,
+00000930: 2073 6574 7469 6e67 7320 5b2e 2e2e 5d5b   settings [...][
+00000940: 2749 4e5f 5341 4d50 4c45 5f4c 4f4f 275d  'IN_SAMPLE_LOO']
+00000950: 2074 6f0a 2020 2020 2020 2020 5472 7565   to.        True
+00000960: 2077 696c 6c20 7472 6967 6765 7220 7468   will trigger th
+00000970: 6520 666c 6167 206f 6620 7468 6520 696e  e flag of the in
+00000980: 7374 616e 6365 2e20 5468 6973 206d 6561  stance. This mea
+00000990: 6e73 2c20 7468 6174 2065 6163 6820 7469  ns, that each ti
+000009a0: 6d65 2074 6865 206d 6574 686f 640a 2020  me the method.  
+000009b0: 2020 2020 2020 4576 616c 7561 7469 6f6e        Evaluation
+000009c0: 5f4d 616e 6167 6572 2829 2e74 7261 636b  _Manager().track
+000009d0: 5f72 6573 756c 7473 2069 7320 6361 6c6c  _results is call
+000009e0: 6564 2c20 4576 616c 7561 746f 7220 7769  ed, Evaluator wi
+000009f0: 6c6c 2074 7279 2074 6f20 6361 6c63 756c  ll try to calcul
+00000a00: 6174 650a 2020 2020 2020 2020 4c65 6176  ate.        Leav
+00000a10: 652d 4f6e 652d 4f75 7420 7363 6f72 6520  e-One-Out score 
+00000a20: 666f 7220 6561 6368 2063 6c69 656e 7420  for each client 
+00000a30: 696e 2074 6865 2073 616d 706c 652e 0a20  in the sample.. 
+00000a40: 2020 2020 2020 200a 2020 2020 2020 2020         .        
+00000a50: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00000a60: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00000a70: 2020 2020 2020 7365 7474 696e 6773 3a20        settings: 
+00000a80: 6469 6374 0a20 2020 2020 2020 2020 2020  dict.           
+00000a90: 2041 2064 6963 7469 6f6e 6172 7920 636f   A dictionary co
+00000aa0: 6e74 6169 6e69 6e67 2061 6c6c 2074 6865  ntaining all the
+00000ab0: 2072 656c 6576 616e 7420 7365 7474 696e   relevant settin
+00000ac0: 6773 2066 6f72 2074 6865 2065 7661 6c75  gs for the evalu
+00000ad0: 6174 696f 6e5f 6d61 6e61 6765 722e 0a20  ation_manager.. 
+00000ae0: 2020 2020 2020 206d 6f64 656c 3a20 4665         model: Fe
+00000af0: 6465 7261 7465 644d 6f64 656c 0a20 2020  deratedModel.   
+00000b00: 2020 2020 2020 2020 2041 2069 6e69 7469           A initi
+00000b10: 616c 697a 6564 2069 6e73 7461 6e63 6520  alized instance 
+00000b20: 6f66 2074 6865 2063 6c61 7373 2061 736f  of the class aso
+00000b30: 6369 6974 612e 6d6f 6465 6c73 2e70 7974  ciita.models.pyt
+00000b40: 6f72 6368 2e66 6564 6572 6174 6564 5f6d  orch.federated_m
+00000b50: 6f64 656c 2e46 6564 6572 6174 6564 4d6f  odel.FederatedMo
+00000b60: 6465 6c0a 2020 2020 2020 2020 2020 2020  del.            
+00000b70: 5468 6973 2069 7320 6e65 6365 7373 6172  This is necessar
+00000b80: 7920 746f 2069 6e69 7469 616c 697a 6520  y to initialize 
+00000b90: 736f 6d65 2063 6f6e 7472 6962 7574 696f  some contributio
+00000ba0: 6e2d 6573 7469 6d61 7469 6f6e 206f 626a  n-estimation obj
+00000bb0: 6563 7473 2e0a 2020 2020 2020 2020 6e6f  ects..        no
+00000bc0: 6465 733a 206c 6973 742c 2064 6566 6175  des: list, defau
+00000bd0: 6c74 2074 6f20 4e6f 6e65 0a20 2020 2020  lt to None.     
+00000be0: 2020 2020 2020 2041 206c 6973 7420 636f         A list co
+00000bf0: 6e74 6169 6e69 6e67 2074 6865 2069 6427  ntaining the id'
+00000c00: 7320 6f66 2061 6c6c 2074 6865 2072 656c  s of all the rel
+00000c10: 6576 616e 7420 6e6f 6465 732e 0a20 2020  evant nodes..   
+00000c20: 2020 2020 2069 7465 7261 7469 6f6e 733a       iterations:
+00000c30: 2069 6e74 2c20 6465 6661 756c 7420 746f   int, default to
+00000c40: 204e 6f6e 650a 2020 2020 2020 2020 2020   None.          
+00000c50: 2020 4e75 6d62 6572 206f 6620 6974 6572    Number of iter
+00000c60: 6174 696f 6e73 2e0a 2020 2020 2020 2020  ations..        
+00000c70: 0a20 2020 2020 2020 2052 6574 7572 6e73  .        Returns
+00000c80: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00000c90: 0a20 2020 2020 2020 204e 6f6e 650a 0a20  .        None.. 
+00000ca0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
+00000cb0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
+00000cc0: 2020 2020 2020 2020 2020 204e 6f74 496d             NotIm
+00000cd0: 706c 656d 656e 7465 6445 7272 6f72 0a20  plementedError. 
+00000ce0: 2020 2020 2020 2020 2020 2020 2020 2049                 I
+00000cf0: 6620 7468 6520 666c 6167 2066 6f72 204f  f the flag for O
+00000d00: 6e65 2d52 6f75 6e64 2053 6861 706c 6579  ne-Round Shapley
+00000d10: 2061 6e64 204f 6e65 2d52 6f75 6e64 204c   and One-Round L
+00000d20: 4f4f 2069 7320 7365 7420 746f 2054 7275  OO is set to Tru
+00000d30: 652e 0a20 2020 2020 2020 2020 2020 2053  e..            S
+00000d40: 616d 706c 655f 4576 616c 7561 746f 725f  ample_Evaluator_
+00000d50: 496e 6974 5f45 7863 6570 7469 6f6e 0a20  Init_Exception. 
+00000d60: 2020 2020 2020 2020 2020 2020 2020 2049                 I
+00000d70: 6620 7468 6520 4576 616c 7561 7469 6f6e  f the Evaluation
+00000d80: 204d 616e 6167 6572 2069 7320 756e 6162   Manager is unab
+00000d90: 6c65 2074 6f20 696e 6974 6961 6c69 7a65  le to initialize
+00000da0: 2061 6e20 696e 7374 616e 6365 206f 6620   an instance of 
+00000db0: 7468 6520 0a20 2020 2020 2020 2020 2020  the .           
+00000dc0: 2020 2020 2053 616d 706c 6520 4576 616c       Sample Eval
+00000dd0: 7561 746f 722e 0a20 2020 2020 2020 204e  uator..        N
+00000de0: da0a 5368 6170 6c65 795f 4f52 545a 0a73  ..Shapley_ORTZ.s
+00000df0: 6861 706c 6579 5f6f 7246 da06 4c4f 4f5f  hapley_orF..LOO_
+00000e00: 4f52 5a06 6c6f 6f5f 6f72 da0d 494e 5f53  ORZ.loo_or..IN_S
+00000e10: 414d 504c 455f 4c4f 4fda 0d69 6e5f 7361  AMPLE_LOO..in_sa
+00000e20: 6d70 6c65 5f6c 6f6f da0e 494e 5f53 414d  mple_loo..IN_SAM
+00000e30: 504c 455f 5348 4150 da0e 696e 5f73 616d  PLE_SHAP..in_sam
+00000e40: 706c 655f 7368 6170 7203 0000 00da 1370  ple_shapr......p
+00000e50: 7265 7365 7276 655f 6576 616c 7561 7469  reserve_evaluati
+00000e60: 6f6e da18 7072 6573 6572 7665 5f70 6172  on..preserve_par
+00000e70: 7469 616c 5f72 6573 756c 7473 da16 7072  tial_results..pr
+00000e80: 6573 6572 7665 5f66 696e 616c 5f72 6573  eserve_final_res
+00000e90: 756c 7473 2902 720b 0000 0072 0c00 0000  ults).r....r....
+00000ea0: 2902 720d 0000 0072 0e00 0000 da12 6c69  ).r....r......li
+00000eb0: 6e65 5f73 6561 7263 685f 6c65 6e67 7468  ne_search_length
+00000ec0: da09 7363 6865 6475 6c65 7263 0100 0000  ..schedulerc....
+00000ed0: 0000 0000 0000 0000 0200 0000 0600 0000  ................
+00000ee0: 1300 0000 7320 0000 0069 007c 005d 0c7d  ....s ...i.|.].}
+00000ef0: 017c 0164 0064 0184 0074 0088 0083 0144  .|.d.d...t.....D
+00000f00: 0083 0193 0271 0253 0029 0263 0100 0000  .....q.S.).c....
+00000f10: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00000f20: 5300 0000 7310 0000 0067 007c 005d 047d  S...s....g.|.].}
+00000f30: 017c 0191 0271 0253 00a9 0072 1b00 0000  .|...q.S...r....
+00000f40: 2902 da02 2e30 da09 6974 6572 6174 696f  )....0..iteratio
+00000f50: 6e72 1b00 0000 721b 0000 00fa 7f2f 686f  nr....r....../ho
+00000f60: 6d65 2f6d 7a75 7a69 616b 2f73 6e61 702f  me/mzuziak/snap/
+00000f70: 736e 6170 642d 6465 736b 746f 702d 696e  snapd-desktop-in
+00000f80: 7465 6772 6174 696f 6e2f 3833 2f44 6f63  tegration/83/Doc
+00000f90: 756d 656e 7473 2f41 736f 6369 6974 612f  uments/Asociita/
+00000fa0: 6173 6f63 6969 7461 2f61 736f 6369 6974  asociita/asociit
+00000fb0: 612f 636f 6d70 6f6e 656e 7473 2f65 7661  a/components/eva
+00000fc0: 6c75 6174 6f72 2f65 7661 6c75 6174 696f  luator/evaluatio
+00000fd0: 6e5f 6d61 6e61 6765 722e 7079 da0a 3c6c  n_manager.py..<l
+00000fe0: 6973 7463 6f6d 703e 9300 0000 7302 0000  istcomp>....s...
+00000ff0: 0010 007a 3a45 7661 6c75 6174 696f 6e5f  ...z:Evaluation_
+00001000: 4d61 6e61 6765 722e 5f5f 696e 6974 5f5f  Manager.__init__
+00001010: 2e3c 6c6f 6361 6c73 3e2e 3c64 6963 7463  .<locals>.<dictc
+00001020: 6f6d 703e 2e3c 6c69 7374 636f 6d70 3e29  omp>.<listcomp>)
+00001030: 01da 0572 616e 6765 2902 721c 0000 00da  ...range).r.....
+00001040: 0466 6c61 67a9 0172 0e00 0000 721b 0000  .flag..r....r...
+00001050: 0072 1e00 0000 da0a 3c64 6963 7463 6f6d  .r......<dictcom
+00001060: 703e 9300 0000 7302 0000 0020 007a 2f45  p>....s.... .z/E
+00001070: 7661 6c75 6174 696f 6e5f 4d61 6e61 6765  valuation_Manage
+00001080: 722e 5f5f 696e 6974 5f5f 2e3c 6c6f 6361  r.__init__.<loca
+00001090: 6c73 3e2e 3c64 6963 7463 6f6d 703e da0a  ls>.<dictcomp>..
+000010a0: 6675 6c6c 5f64 6562 7567 5a0f 6465 6275  full_debugZ.debu
+000010b0: 675f 6669 6c65 5f70 6174 68da 0f66 756c  g_file_path..ful
+000010c0: 6c5f 6465 6275 675f 7061 7468 5a17 6469  l_debug_pathZ.di
+000010d0: 7361 626c 655f 6d75 6c74 6970 726f 6365  sable_multiproce
+000010e0: 7373 696e 67da 116e 756d 6265 725f 6f66  ssing..number_of
+000010f0: 5f77 6f72 6b65 7273 2923 720b 0000 00da  _workers)#r.....
+00001100: 1070 7265 7669 6f75 735f 635f 6d6f 6465  .previous_c_mode
+00001110: 6cda 0f75 7064 6174 6564 5f63 5f6d 6f64  l..updated_c_mod
+00001120: 656c da12 7072 6576 696f 7573 5f6f 7074  el..previous_opt
+00001130: 696d 697a 6572 720d 0000 005a 0e63 6f6d  imizerr....Z.com
+00001140: 7069 6c65 645f 666c 6167 73da 0367 6574  piled_flags..get
+00001150: da0c 666c 6167 5f73 6861 705f 6f72 da06  ..flag_shap_or..
+00001160: 6170 7065 6e64 da13 4e6f 7449 6d70 6c65  append..NotImple
+00001170: 6d65 6e74 6564 4572 726f 72da 0b66 6c61  mentedError..fla
+00001180: 675f 6c6f 6f5f 6f72 da15 666c 6167 5f73  g_loo_or..flag_s
+00001190: 616d 706c 655f 6576 616c 7561 746f 72da  ample_evaluator.
+000011a0: 1766 6c61 675f 7361 6d70 6c65 7368 5f65  .flag_samplesh_e
+000011b0: 7661 6c75 6174 6f72 da13 666c 6167 5f6c  valuator..flag_l
+000011c0: 7361 615f 6576 616c 7561 746f 7272 1700  saa_evaluatorr..
+000011d0: 0000 7218 0000 0072 0200 0000 da0c 6f72  ..r....r......or
+000011e0: 5f65 7661 6c75 6174 6f72 7204 0000 00da  _evaluatorr.....
+000011f0: 1073 616d 706c 655f 6576 616c 7561 746f  .sample_evaluato
+00001200: 72da 094e 616d 6545 7272 6f72 7207 0000  r..NameErrorr...
+00001210: 0072 0500 0000 da12 7361 6d70 6c65 7368  .r......samplesh
+00001220: 5f65 7661 6c75 6174 6f72 7203 0000 00da  _evaluatorr.....
+00001230: 0e6c 7361 615f 6576 616c 7561 746f 72da  .lsaa_evaluator.
+00001240: 0d73 6561 7263 685f 6c65 6e67 7468 da08  .search_length..
+00001250: 4b65 7945 7272 6f72 721a 0000 0072 2400  KeyErrorr....r$.
+00001260: 0000 7225 0000 00da 026f 73da 0667 6574  ..r%.....os..get
+00001270: 6377 64da 066d 756c 7469 7072 2600 0000  cwd..multipr&...
+00001280: 2907 da04 7365 6c66 720b 0000 0072 0c00  )...selfr....r..
+00001290: 0000 720d 0000 0072 0e00 0000 da01 65da  ..r....r......e.
+000012a0: 016b 721b 0000 0072 2200 0000 721e 0000  .kr....r"...r...
+000012b0: 00da 085f 5f69 6e69 745f 5f1a 0000 0073  ...__init__....s
+000012c0: 9600 0000 0627 0601 0601 0601 0601 0604  .....'..........
+000012d0: 0a01 0601 0c01 0401 0602 0a02 0601 0c01  ................
+000012e0: 0401 0602 0a02 0601 0e01 0602 0a02 0601  ................
+000012f0: 0e01 0602 0a02 0601 0e01 0602 0e04 0801  ................
+00001300: 0602 0e02 0601 0c04 0401 0201 08ff 0a03  ................
+00001310: 0201 1201 0e01 0401 0880 02ff 0a03 0201  ................
+00001320: 1201 0e01 0401 0880 02ff 0a02 0201 0e01  ................
+00001330: 0e01 0e01 0201 0880 0e01 0201 0880 02ff  ................
+00001340: 0c05 0c01 1602 0c04 0601 0c01 0c01 0c02  ................
+00001350: 0602 0c03 0a01 0602 0e01 7a1b 4576 616c  ..........z.Eval
+00001360: 7561 7469 6f6e 5f4d 616e 6167 6572 2e5f  uation_Manager._
+00001370: 5f69 6e69 745f 5fda 0e70 7265 7669 6f75  _init__..previou
+00001380: 735f 6d6f 6465 6c63 0200 0000 0000 0000  s_modelc........
+00001390: 0000 0000 0200 0000 0300 0000 4300 0000  ............C...
+000013a0: f310 0000 0074 00a0 017c 01a1 017c 005f  .....t...|...|._
+000013b0: 0264 0153 0029 0261 9001 0000 5072 6573  .d.S.).a....Pres
+000013c0: 6572 7665 7320 7468 6520 6d6f 6465 6c20  erves the model 
+000013d0: 6672 6f6d 2074 6865 2070 7265 7669 6f75  from the previou
+000013e0: 7320 726f 756e 6420 6279 2063 6f70 7969  s round by copyi
+000013f0: 6e67 200a 2020 2020 2020 2020 6974 7320  ng .        its 
+00001400: 7374 7275 6374 7572 6520 616e 6420 7573  structure and us
+00001410: 696e 6720 6974 2061 7320 616e 2061 7474  ing it as an att
+00001420: 7269 6275 7465 2773 2076 616c 7565 2e20  ribute's value. 
+00001430: 5368 6f75 6c64 0a20 2020 2020 2020 2062  Should.        b
+00001440: 6520 6361 6c6c 6564 2065 6163 6820 7472  e called each tr
+00001450: 6169 6e69 6e67 2072 6f75 6e64 2062 6566  aining round bef
+00001460: 6f72 6520 7468 6520 7072 6f70 6572 2074  ore the proper t
+00001470: 7261 696e 696e 670a 2020 2020 2020 2020  raining.        
+00001480: 636f 6d6d 656e 6365 732e 0a20 2020 2020  commences..     
+00001490: 2020 200a 2020 2020 2020 2020 5061 7261     .        Para
+000014a0: 6d65 7465 7273 0a20 2020 2020 2020 202d  meters.        -
+000014b0: 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020 2020  ---------.      
+000014c0: 2020 7072 6576 696f 7573 5f6d 6f64 656c    previous_model
+000014d0: 3a20 4665 6465 7261 7465 644d 6f64 656c  : FederatedModel
+000014e0: 0a20 2020 2020 2020 2020 2020 2041 6e20  .            An 
+000014f0: 696e 7374 616e 6365 206f 6620 7468 6520  instance of the 
+00001500: 4665 6465 7261 7465 644d 6f64 656c 206f  FederatedModel o
+00001510: 626a 6563 742e 0a20 2020 2020 2020 2052  bject..        R
+00001520: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+00001530: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
+00001540: 6f6e 650a 2020 2020 2020 2020 4e29 03da  one.        N)..
+00001550: 0463 6f70 79da 0864 6565 7063 6f70 7972  .copy..deepcopyr
+00001560: 2700 0000 2902 723c 0000 0072 4000 0000  '...).r<...r@...
+00001570: 721b 0000 0072 1b00 0000 721e 0000 00da  r....r....r.....
+00001580: 1770 7265 7365 7276 655f 7072 6576 696f  .preserve_previo
+00001590: 7573 5f6d 6f64 656c a800 0000 f302 0000  us_model........
+000015a0: 0010 0f7a 2a45 7661 6c75 6174 696f 6e5f  ...z*Evaluation_
+000015b0: 4d61 6e61 6765 722e 7072 6573 6572 7665  Manager.preserve
+000015c0: 5f70 7265 7669 6f75 735f 6d6f 6465 6cda  _previous_model.
+000015d0: 0d75 7064 6174 6564 5f6d 6f64 656c 6302  .updated_modelc.
+000015e0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
+000015f0: 0000 0043 0000 0072 4100 0000 2902 619a  ...C...rA...).a.
+00001600: 0100 0050 7265 7365 7276 6573 2074 6865  ...Preserves the
+00001610: 2075 7064 6174 6564 2076 6572 7369 6f6e   updated version
+00001620: 206f 6620 7468 6520 6365 6e74 7261 6c20   of the central 
+00001630: 6d6f 6465 6c0a 2020 2020 2020 2020 6279  model.        by
+00001640: 2063 6f70 7969 6e67 2069 7473 2073 7472   copying its str
+00001650: 7563 7475 7265 2061 6e64 2075 7369 6e67  ucture and using
+00001660: 2069 7420 6173 2061 6e20 6174 7472 6962   it as an attrib
+00001670: 7574 6527 7320 7661 6c75 652e 200a 2020  ute's value. .  
+00001680: 2020 2020 2020 5368 6f75 6c64 2062 6520        Should be 
+00001690: 6361 6c6c 6564 2065 6163 6820 7472 6169  called each trai
+000016a0: 6e69 6e67 2061 6674 6572 2075 7064 6174  ning after updat
+000016b0: 696e 6720 7468 6520 7765 6967 6874 730a  ing the weights.
+000016c0: 2020 2020 2020 2020 6f66 2074 6865 2063          of the c
+000016d0: 656e 7472 616c 206d 6f64 656c 2e0a 2020  entral model..  
+000016e0: 2020 2020 2020 0a20 2020 2020 2020 2050        .        P
+000016f0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00001700: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00001710: 2020 2020 2075 7064 6174 6564 5f6d 6f64       updated_mod
+00001720: 656c 3a20 4665 6465 7261 7465 644d 6f64  el: FederatedMod
+00001730: 656c 0a20 2020 2020 2020 2020 2020 2041  el.            A
+00001740: 6e20 696e 7374 616e 6365 206f 6620 7468  n instance of th
+00001750: 6520 4665 6465 7261 7465 644d 6f64 656c  e FederatedModel
+00001760: 206f 626a 6563 742e 0a20 2020 2020 2020   object..       
+00001770: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+00001780: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+00001790: 204e 6f6e 650a 2020 2020 2020 204e 2903   None.       N).
+000017a0: 7242 0000 0072 4300 0000 7228 0000 0029  rB...rC...r(...)
+000017b0: 0272 3c00 0000 7246 0000 0072 1b00 0000  .r<...rF...r....
+000017c0: 721b 0000 0072 1e00 0000 da16 7072 6573  r....r......pres
+000017d0: 6572 7665 5f75 7064 6174 6564 5f6d 6f64  erve_updated_mod
+000017e0: 656c ba00 0000 7245 0000 007a 2945 7661  el....rE...z)Eva
+000017f0: 6c75 6174 696f 6e5f 4d61 6e61 6765 722e  luation_Manager.
+00001800: 7072 6573 6572 7665 5f75 7064 6174 6564  preserve_updated
+00001810: 5f6d 6f64 656c 7229 0000 0063 0200 0000  _modelr)...c....
+00001820: 0000 0000 0000 0000 0200 0000 0300 0000  ................
+00001830: 4300 0000 7241 0000 0029 0261 9801 0000  C...rA...).a....
+00001840: 5072 6573 6572 7665 7320 7468 6520 4f70  Preserves the Op
+00001850: 7469 6d69 7a65 7220 6672 6f6d 2074 6865  timizer from the
+00001860: 2070 7265 7669 6f75 7320 726f 756e 6420   previous round 
+00001870: 6279 2063 6f70 7969 6e67 200a 2020 2020  by copying .    
+00001880: 2020 2020 6974 7320 7374 7275 6374 7572      its structur
+00001890: 6520 616e 6420 7573 696e 6720 6974 2061  e and using it a
+000018a0: 7320 616e 2061 7474 7269 6275 7465 2773  s an attribute's
+000018b0: 2076 616c 7565 2e20 5368 6f75 6c64 0a20   value. Should. 
+000018c0: 2020 2020 2020 2062 6520 6361 6c6c 6564         be called
+000018d0: 2065 6163 6820 7472 6169 6e69 6e67 2072   each training r
+000018e0: 6f75 6e64 2062 6566 6f72 6520 7468 6520  ound before the 
+000018f0: 7072 6f70 6572 2074 7261 696e 696e 670a  proper training.
+00001900: 2020 2020 2020 2020 636f 6d6d 656e 6365          commence
+00001910: 732e 0a20 2020 2020 2020 200a 2020 2020  s..        .    
+00001920: 2020 2020 5061 7261 6d65 7465 7273 0a20      Parameters. 
+00001930: 2020 2020 2020 202d 2d2d 2d2d 2d2d 2d2d         ---------
+00001940: 2d0a 2020 2020 2020 2020 7072 6576 696f  -.        previo
+00001950: 7573 5f6f 7074 696d 697a 6572 3a20 4f70  us_optimizer: Op
+00001960: 7469 6d69 7a65 7273 0a20 2020 2020 2020  timizers.       
+00001970: 2020 2020 2041 6e20 696e 7374 616e 6365       An instance
+00001980: 206f 6620 7468 6520 6173 6f63 6969 7461   of the asociita
+00001990: 2e4f 7074 696d 697a 6572 7320 636c 6173  .Optimizers clas
+000019a0: 732e 0a20 2020 2020 2020 2052 6574 7572  s..        Retur
+000019b0: 6e73 0a20 2020 2020 2020 202d 2d2d 2d2d  ns.        -----
+000019c0: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
+000019d0: 2020 2020 2020 2020 4e29 0372 4200 0000          N).rB...
+000019e0: 7243 0000 0072 2900 0000 2902 723c 0000  rC...r)...).r<..
+000019f0: 0072 2900 0000 721b 0000 0072 1b00 0000  .r)...r....r....
+00001a00: 721e 0000 00da 1b70 7265 7365 7276 655f  r......preserve_
+00001a10: 7072 6576 696f 7573 5f6f 7074 696d 697a  previous_optimiz
+00001a20: 6572 cb00 0000 7245 0000 007a 2e45 7661  er....rE...z.Eva
+00001a30: 6c75 6174 696f 6e5f 4d61 6e61 6765 722e  luation_Manager.
+00001a40: 7072 6573 6572 7665 5f70 7265 7669 6f75  preserve_previou
+00001a50: 735f 6f70 7469 6d69 7a65 72da 0967 7261  s_optimizer..gra
+00001a60: 6469 656e 7473 da0f 6e6f 6465 735f 696e  dients..nodes_in
+00001a70: 5f73 616d 706c 6572 1d00 0000 6304 0000  _sampler....c...
+00001a80: 0000 0000 0000 0000 000a 0000 0009 0000  ................
+00001a90: 0043 0000 0073 ec03 0000 7c00 6a00 720b  .C...s....|.j.r.
+00001aa0: 7c00 6a01 6a02 7c01 6401 8d01 0100 6e0a  |.j.j.|.d.....n.
+00001ab0: 7c00 6a03 7215 7c00 6a01 6a04 7c01 6401  |.j.r.|.j.j.|.d.
+00001ac0: 8d01 0100 7c00 6a05 72a5 7c03 7c00 6a06  ....|.j.r.|.|.j.
+00001ad0: 6402 1900 7600 72a5 7c00 6a07 6a08 7c01  d...v.r.|.j.j.|.
+00001ae0: 7c02 7c03 7c00 6a09 7c00 6a0a 7c00 6a0b  |.|.|.j.|.j.|.j.
+00001af0: 6403 8d06 7d04 7c00 6a0c 72a5 7c03 6404  d...}.|.j.r.|.d.
+00001b00: 6b02 7272 740d 740e 6a0f a010 7c00 6a11  k.rrt.t.j...|.j.
+00001b10: 6405 a102 6406 6407 6408 8d03 8f27 7d05  d...d.d.d....'}.
+00001b20: 6700 6409 a201 7d06 7412 a013 7c05 a101  g.d...}.t...|...
+00001b30: 7d07 7c07 a014 7c06 a101 0100 7c04 a015  }.|...|.....|...
+00001b40: a100 4400 5d0c 5c02 7d08 7d09 7c07 a014  ..D.].\.}.}.|...
+00001b50: 7c08 7c09 7c03 6703 a101 0100 7155 5700  |.|.|.g.....qUW.
+00001b60: 640a 0400 0400 8303 0100 6e08 3100 736c  d.........n.1.sl
+00001b70: 7701 0100 0100 0100 5900 0100 6e33 740d  w.......Y...n3t.
+00001b80: 740e 6a0f a010 7c00 6a11 6405 a102 6406  t.j...|.j.d...d.
+00001b90: 6407 6408 8d03 8f1e 7d05 7412 a013 7c05  d.d.....}.t...|.
+00001ba0: a101 7d07 7c04 a015 a100 4400 5d0c 5c02  ..}.|.....D.].\.
+00001bb0: 7d08 7d09 7c07 a014 7c08 7c09 7c03 6703  }.}.|...|.|.|.g.
+00001bc0: a101 0100 7189 5700 640a 0400 0400 8303  ....q.W.d.......
+00001bd0: 0100 6e08 3100 73a0 7701 0100 0100 0100  ..n.1.s.w.......
+00001be0: 5900 0100 7c00 6a16 9001 7251 7c03 7c00  Y...|.j...rQ|.|.
+00001bf0: 6a06 640b 1900 7600 9001 7251 7c00 6a17  j.d...v...rQ|.j.
+00001c00: 72c6 7c00 6a18 6a19 7c01 7c02 7c03 7c00  r.|.j.j.|.|.|.|.
+00001c10: 6a09 7c00 6a0b 7c00 6a0c 7c00 6a1a 640c  j.|.j.|.j.|.j.d.
+00001c20: 8d07 7d04 6e0f 7c00 6a18 6a1b 7c01 7c02  ..}.n.|.j.j.|.|.
+00001c30: 7c03 7c00 6a09 7c00 6a0b 7c00 6a0c 640d  |.|.j.|.j.|.j.d.
+00001c40: 8d06 7d04 7c00 6a0c 9001 7251 7c03 6404  ..}.|.j...rQ|.d.
+00001c50: 6b02 9001 721c 740d 740e 6a0f a010 7c00  k...r.t.t.j...|.
+00001c60: 6a11 640e a102 6406 6407 6408 8d03 8f27  j.d...d.d.d....'
+00001c70: 7d05 6700 6409 a201 7d06 7412 a013 7c05  }.g.d...}.t...|.
+00001c80: a101 7d07 7c07 a014 7c06 a101 0100 7c04  ..}.|...|.....|.
+00001c90: a015 a100 4400 5d0c 5c02 7d08 7d09 7c07  ....D.].\.}.}.|.
+00001ca0: a014 7c08 7c09 7c03 6703 a101 0100 71fe  ..|.|.|.g.....q.
+00001cb0: 5700 640a 0400 0400 8303 0100 6e09 3100  W.d.........n.1.
+00001cc0: 9001 7316 7701 0100 0100 0100 5900 0100  ..s.w.......Y...
+00001cd0: 6e35 740d 740e 6a0f a010 7c00 6a11 640e  n5t.t.j...|.j.d.
+00001ce0: a102 6406 6407 6408 8d03 8f1f 7d05 7412  ..d.d.d.....}.t.
+00001cf0: a013 7c05 a101 7d07 7c04 a015 a100 4400  ..|...}.|.....D.
+00001d00: 5d0d 5c02 7d08 7d09 7c07 a014 7c08 7c09  ].\.}.}.|...|.|.
+00001d10: 7c03 6703 a101 0100 9001 7133 5700 640a  |.g.......q3W.d.
+00001d20: 0400 0400 8303 0100 6e09 3100 9001 734c  ........n.1...sL
+00001d30: 7701 0100 0100 0100 5900 0100 7c00 6a1c  w.......Y...|.j.
+00001d40: 9001 72f0 7c03 7c00 6a06 640f 1900 7600  ..r.|.|.j.d...v.
+00001d50: 9001 72f2 7c00 6a1d 6a1e 7c01 7c02 7c03  ..r.|.j.j.|.|.|.
+00001d60: 7c00 6a1f 7c00 6a09 7c00 6a0a 7c00 6a0b  |.j.|.j.|.j.|.j.
+00001d70: 6410 8d07 7d04 7c00 6a0c 9001 72f4 7c03  d...}.|.j...r.|.
+00001d80: 6404 6b02 9001 72b8 740d 740e 6a0f a010  d.k...r.t.t.j...
+00001d90: 7c00 6a11 6411 a102 6406 6407 6408 8d03  |.j.d...d.d.d...
+00001da0: 8f29 7d05 6700 6409 a201 7d06 7412 a013  .)}.g.d...}.t...
+00001db0: 7c05 a101 7d07 7c07 a014 7c06 a101 0100  |...}.|...|.....
+00001dc0: 7c04 a015 a100 4400 5d0d 5c02 7d08 7d09  |.....D.].\.}.}.
+00001dd0: 7c07 a014 7c08 7c09 7c03 6703 a101 0100  |...|.|.|.g.....
+00001de0: 9001 7197 5700 640a 0400 0400 8303 0100  ..q.W.d.........
+00001df0: 640a 5300 3100 9001 73b1 7701 0100 0100  d.S.1...s.w.....
+00001e00: 0100 5900 0100 640a 5300 740d 740e 6a0f  ..Y...d.S.t.t.j.
+00001e10: a010 7c00 6a11 6411 a102 6406 6407 6408  ..|.j.d...d.d.d.
+00001e20: 8d03 8f20 7d05 7412 a013 7c05 a101 7d07  ... }.t...|...}.
+00001e30: 7c04 a015 a100 4400 5d0d 5c02 7d08 7d09  |.....D.].\.}.}.
+00001e40: 7c07 a014 7c08 7c09 7c03 6703 a101 0100  |...|.|.|.g.....
+00001e50: 9001 71cf 5700 640a 0400 0400 8303 0100  ..q.W.d.........
+00001e60: 640a 5300 3100 9001 73e9 7701 0100 0100  d.S.1...s.w.....
+00001e70: 0100 5900 0100 640a 5300 640a 5300 640a  ..Y...d.S.d.S.d.
+00001e80: 5300 640a 5300 2912 61ad 0200 004d 6574  S.d.S.).a....Met
+00001e90: 686f 6420 7573 6564 2074 6f20 7472 6163  hod used to trac
+00001ea0: 6b5f 7265 7375 6c74 7320 6166 7465 7220  k_results after 
+00001eb0: 6561 6368 2074 7261 696e 696e 6720 726f  each training ro
+00001ec0: 756e 642e 0a20 2020 2020 2020 2042 6563  und..        Bec
+00001ed0: 6175 7365 2074 6865 204f 7263 6865 7374  ause the Orchest
+00001ee0: 7261 746f 7220 6162 7374 7261 6374 696f  rator abstractio
+00001ef0: 6e20 7368 6f75 6c64 2062 6520 6672 6565  n should be free
+00001f00: 206f 6620 616e 790a 2020 2020 2020 2020   of any.        
+00001f10: 756e 6e65 6365 7373 6172 7920 656e 6375  unnecessary encu
+00001f20: 6d62 7261 6e63 652c 2074 6865 2045 7661  mbrance, the Eva
+00001f30: 6c75 6174 696f 6e5f 4d61 6e61 6765 722e  luation_Manager.
+00001f40: 7472 6163 6b5f 7265 7375 6c74 7328 290a  track_results().
+00001f50: 2020 2020 2020 2020 7769 6c6c 2074 616b          will tak
+00001f60: 6520 6361 7265 206f 6620 616e 7920 7265  e care of any re
+00001f70: 7375 6c74 2070 7265 7365 7276 6174 696f  sult preservatio
+00001f80: 6e20 616e 6420 7363 6f72 6520 6361 6c63  n and score calc
+00001f90: 756c 6174 696f 6e20 7468 6174 200a 2020  ulation that .  
+00001fa0: 2020 2020 2020 6d75 7374 2062 6520 646f        must be do
+00001fb0: 6e65 2069 6e20 6f72 6465 7220 746f 2065  ne in order to e
+00001fc0: 7374 6162 6c69 7368 2074 6865 2072 6573  stablish the res
+00001fd0: 756c 7473 2e0a 2020 2020 2020 2020 0a20  ults..        . 
+00001fe0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00001ff0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00002000: 2d2d 2d2d 0a20 2020 2020 2020 2067 7261  ----.        gra
+00002010: 6469 656e 7473 3a20 4f72 6465 7265 6444  dients: OrderedD
+00002020: 6963 740a 2020 2020 2020 2020 2020 2020  ict.            
+00002030: 416e 204f 7264 6572 6564 4469 6374 2063  An OrderedDict c
+00002040: 6f6e 7461 696e 696e 6720 6772 6164 6965  ontaining gradie
+00002050: 6e74 7320 6f66 2074 6865 2073 616d 706c  nts of the sampl
+00002060: 6564 206e 6f64 6573 2e0a 2020 2020 2020  ed nodes..      
+00002070: 2020 6e6f 6465 735f 696e 5f73 616d 706c    nodes_in_sampl
+00002080: 653a 206c 6973 740a 2020 2020 2020 2020  e: list.        
+00002090: 2020 2020 4120 6c69 7374 2063 6f6e 7461      A list conta
+000020a0: 696e 696e 6720 6964 2773 206f 6620 7468  ining id's of th
+000020b0: 6520 6e6f 6465 7320 7468 6174 2077 6572  e nodes that wer
+000020c0: 6520 7361 6d70 6c65 642e 0a20 2020 2020  e sampled..     
+000020d0: 2020 2069 7465 7261 7469 6f6e 3a20 696e     iteration: in
+000020e0: 740a 2020 2020 2020 2020 2020 2020 5468  t.            Th
+000020f0: 6520 6375 7272 656e 7420 6974 6572 6174  e current iterat
+00002100: 696f 6e2e 0a20 2020 2020 2020 2052 6574  ion..        Ret
+00002110: 7572 6e73 0a20 2020 2020 2020 202d 2d2d  urns.        ---
+00002120: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+00002130: 650a 2020 2020 2020 2020 2901 7249 0000  e.        ).rI..
+00002140: 0072 1300 0000 2906 7249 0000 0072 4a00  .r....).rI...rJ.
+00002150: 0000 721d 0000 00da 096f 7074 696d 697a  ..r......optimiz
+00002160: 6572 da0b 6669 6e61 6c5f 6d6f 6465 6c72  er..final_modelr
+00002170: 4000 0000 7201 0000 007a 1863 6f6c 5f76  @...r....z.col_v
+00002180: 616c 7565 735f 6465 6275 675f 6c6f 6f2e  alues_debug_loo.
+00002190: 6373 767a 0261 2bda 00a9 01da 076e 6577  csvz.a+......new
+000021a0: 6c69 6e65 2903 da09 636f 616c 6974 696f  line)...coalitio
+000021b0: 6eda 0576 616c 7565 721d 0000 004e 7215  n..valuer....Nr.
+000021c0: 0000 0029 0772 4900 0000 724a 0000 0072  ...).rI...rJ...r
+000021d0: 1d00 0000 724b 0000 0072 4000 0000 da11  ....rK...r@.....
+000021e0: 7265 7475 726e 5f63 6f61 6c69 7469 6f6e  return_coalition
+000021f0: 7372 2600 0000 2906 7249 0000 0072 4a00  sr&...).rI...rJ.
+00002200: 0000 721d 0000 0072 4b00 0000 7240 0000  ..r....rK...r@..
+00002210: 0072 5200 0000 7a14 636f 6c5f 7661 6c75  .rR...z.col_valu
+00002220: 6573 5f64 6562 7567 2e63 7376 7203 0000  es_debug.csvr...
+00002230: 0029 0772 4900 0000 724a 0000 0072 1d00  .).rI...rJ...r..
+00002240: 0000 7237 0000 0072 4b00 0000 724c 0000  ..r7...rK...rL..
+00002250: 0072 4000 0000 7a19 636f 6c5f 7661 6c75  .r@...z.col_valu
+00002260: 6573 5f64 6562 7567 5f6c 7361 612e 6373  es_debug_lsaa.cs
+00002270: 7629 2072 2b00 0000 7232 0000 005a 0d74  v) r+...r2...Z.t
+00002280: 7261 636b 5f73 6861 706c 6579 722e 0000  rack_shapleyr...
+00002290: 005a 0974 7261 636b 5f6c 6f6f 722f 0000  .Z.track_loor/..
+000022a0: 0072 1a00 0000 7233 0000 005a 0a75 7064  .r....r3...Z.upd
+000022b0: 6174 655f 7073 6972 2900 0000 7228 0000  ate_psir)...r(..
+000022c0: 0072 2700 0000 7224 0000 00da 046f 7065  .r'...r$.....ope
+000022d0: 6e72 3900 0000 da04 7061 7468 da04 6a6f  nr9.....path..jo
+000022e0: 696e 7225 0000 00da 0363 7376 da06 7772  inr%.....csv..wr
+000022f0: 6974 6572 da08 7772 6974 6572 6f77 da05  iter..writerow..
+00002300: 6974 656d 7372 3000 0000 723b 0000 0072  itemsr0...r;...r
+00002310: 3500 0000 5a12 7570 6461 7465 5f73 6861  5...Z.update_sha
+00002320: 705f 6d75 6c74 6970 7226 0000 005a 0b75  p_multipr&...Z.u
+00002330: 7064 6174 655f 7368 6170 7231 0000 0072  pdate_shapr1...r
+00002340: 3600 0000 5a0b 7570 6461 7465 5f6c 7361  6...Z.update_lsa
+00002350: 6172 3700 0000 290a 723c 0000 0072 4900  ar7...).r<...rI.
+00002360: 0000 724a 0000 0072 1d00 0000 5a0c 6465  ..rJ...r....Z.de
+00002370: 6275 675f 7661 6c75 6573 da08 6373 765f  bug_values..csv_
+00002380: 6669 6c65 da0b 6669 656c 645f 6e61 6d65  file..field_name
+00002390: 73da 0a63 7376 5f77 7269 7465 72da 0363  s..csv_writer..c
+000023a0: 6f6c 7251 0000 0072 1b00 0000 721b 0000  olrQ...r....r...
+000023b0: 0072 1e00 0000 da0d 7472 6163 6b5f 7265  .r......track_re
+000023c0: 7375 6c74 73dd 0000 0073 bc00 0000 0618  sults....s......
+000023d0: 1001 0601 0e01 0603 0e01 0801 0201 0201  ................
+000023e0: 0401 0401 0401 06fb 0607 0801 1c01 0801  ................
+000023f0: 0a01 0a01 1001 1201 02ff 1cfc 0280 1c07  ................
+00002400: 0a01 1001 1201 02ff 1cfe 0806 1001 0601  ................
+00002410: 0801 0201 0201 0401 0401 0401 0401 08fa  ................
+00002420: 0808 0201 0201 0401 0401 0401 06fb 0808  ................
+00002430: 0a01 1c01 0801 0a01 0a01 1001 1201 02ff  ................
+00002440: 1efc 0280 1c07 0a01 1001 1401 02ff 1efe  ................
+00002450: 0806 1001 0801 0201 0201 0401 0401 0401  ................
+00002460: 0401 06fa 0809 0a01 1c01 0801 0a01 0a01  ................
+00002470: 1001 1401 02ff 24fc 1c07 0a01 1001 1401  ......$.........
+00002480: 02ff 24fe 04ec 0401 040a 7a20 4576 616c  ..$.......z Eval
+00002490: 7561 7469 6f6e 5f4d 616e 6167 6572 2e74  uation_Manager.t
+000024a0: 7261 636b 5f72 6573 756c 7473 7254 0000  rack_resultsrT..
+000024b0: 0063 0200 0000 0000 0000 0000 0000 1100  .c..............
+000024c0: 0000 0900 0000 4300 0000 73e0 0100 0069  ......C...s....i
+000024d0: 0069 0064 019c 027d 027c 006a 0072 0a74  .i.d...}.|.j.r.t
+000024e0: 0182 017c 006a 0272 0f74 0182 017c 006a  ...|.j.r.t...|.j
+000024f0: 0372 257c 006a 04a0 05a1 005c 027d 037d  .r%|.j.....\.}.}
+00002500: 047c 037c 0264 0219 0064 033c 007c 047c  .|.|.d...d.<.|.|
+00002510: 0264 0419 0064 053c 007c 006a 0672 3b7c  .d...d.<.|.j.r;|
+00002520: 006a 07a0 08a1 005c 027d 057d 067c 057c  .j.....\.}.}.|.|
+00002530: 0264 0219 0064 063c 007c 067c 0264 0419  .d...d.<.|.|.d..
+00002540: 0064 073c 007c 006a 0972 517c 006a 09a0  .d.<.|.j.rQ|.j..
+00002550: 0aa1 005c 027d 077d 087c 077c 0264 0219  ...\.}.}.|.|.d..
+00002560: 0064 083c 007c 087c 0264 0419 0064 093c  .d.<.|.|.d...d.<
+00002570: 007c 006a 0b64 0a6b 0272 a87c 0264 0219  .|.j.d.k.r.|.d..
+00002580: 00a0 0ca1 0044 005d 4b5c 027d 097d 0a74  .....D.]K\.}.}.t
+00002590: 0d6a 0ea0 0f7c 0174 107c 0983 0164 0b17  .j...|.t.|...d..
+000025a0: 00a1 027d 0b7c 006a 117d 0c7c 0ca0 1264  ...}.|.j.}.|...d
+000025b0: 0ca1 0101 0074 137c 0b64 0d64 0e64 0f8d  .....t.|.d.d.d..
+000025c0: 038f 257d 0d74 146a 157c 0d7c 0c64 108d  ..%}.t.j.|.|.d..
+000025d0: 027d 0e7c 0ea0 16a1 0001 007c 0aa0 0ca1  .}.|.......|....
+000025e0: 0044 005d 0d5c 027d 0f7d 107c 0f7c 1064  .D.].\.}.}.|.|.d
+000025f0: 0c3c 007c 0ea0 177c 10a1 0101 0071 8a57  .<.|...|.....q.W
+00002600: 0064 1104 0004 0083 0301 006e 0831 0073  .d.........n.1.s
+00002610: a277 0101 0001 0001 0059 0001 0071 5c7c  .w.......Y...q\|
+00002620: 006a 1864 0a6b 0272 ee7c 0264 0419 00a0  .j.d.k.r.|.d....
+00002630: 0ca1 0044 005d 3a5c 027d 097d 0a74 0d6a  ...D.]:\.}.}.t.j
+00002640: 0ea0 0f7c 0174 107c 0983 0164 0b17 00a1  ...|.t.|...d....
+00002650: 027d 0b7c 0aa0 19a1 007d 0c74 137c 0b64  .}.|.....}.t.|.d
+00002660: 0d64 0e64 0f8d 038f 187d 0d74 146a 157c  .d.d.....}.t.j.|
+00002670: 0d7c 0c64 108d 027d 0e7c 0ea0 16a1 0001  .|.d...}.|......
+00002680: 007c 0ea0 177c 0aa1 0101 0057 0064 1104  .|...|.....W.d..
+00002690: 0004 0083 0301 006e 0831 0073 e877 0101  .......n.1.s.w..
+000026a0: 0001 0001 0059 0001 0071 b37c 0253 0029  .....Y...q.|.S.)
+000026b0: 1261 4a02 0000 4d65 7468 6f64 2075 7365  .aJ...Method use
+000026c0: 6420 746f 2066 696e 616c 697a 6520 7468  d to finalize th
+000026d0: 6520 7472 6163 6b69 6e67 2061 7420 7468  e tracking at th
+000026e0: 6520 656e 6420 6f66 2074 6865 2074 7261  e end of the tra
+000026f0: 696e 696e 672e 0a20 2020 2020 2020 2042  ining..        B
+00002700: 6563 6175 7365 2074 6865 204f 7263 6865  ecause the Orche
+00002710: 7374 7261 746f 7220 6162 7374 7261 6374  strator abstract
+00002720: 696f 6e20 7368 6f75 6c64 2062 6520 6672  ion should be fr
+00002730: 6565 206f 6620 616e 790a 2020 2020 2020  ee of any.      
+00002740: 2020 756e 6e65 6365 7373 6172 7920 656e    unnecessary en
+00002750: 6375 6d62 7261 6e63 652c 2061 6c6c 2074  cumbrance, all t
+00002760: 6865 206f 7074 696f 6e73 2063 6f6e 6669  he options confi
+00002770: 6775 7269 6e67 2074 6865 2062 6568 6176  guring the behav
+00002780: 696f 7572 0a20 2020 2020 2020 206f 6620  iour.        of 
+00002790: 7468 6520 6669 6e61 6c69 7a65 5f74 7261  the finalize_tra
+000027a0: 636b 696e 6720 6d65 7468 6f64 2c20 7368  cking method, sh
+000027b0: 6f75 6c64 2062 6520 7072 652d 636f 6e66  ould be pre-conf
+000027c0: 6967 7572 6564 2061 7420 7468 6520 7374  igured at the st
+000027d0: 6167 650a 2020 2020 2020 2020 6f66 2074  age.        of t
+000027e0: 6865 2045 7661 6c75 6174 696f 6e5f 4d61  he Evaluation_Ma
+000027f0: 6e61 6765 7220 696e 7374 616e 6365 2069  nager instance i
+00002800: 6e69 7469 616c 697a 6174 696f 6e2e 2020  nitialization.  
+00002810: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
+00002820: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
+00002830: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
+00002840: 2020 2020 2020 2020 7061 7468 3a20 7374          path: st
+00002850: 722c 2064 6566 6175 6c74 2074 6f20 4e6f  r, default to No
+00002860: 6e65 0a20 2020 2020 2020 2020 2020 2061  ne.            a
+00002870: 2073 7472 696e 6720 6f72 2050 6174 682d   string or Path-
+00002880: 6c69 6b65 206f 626a 6563 7420 746f 2074  like object to t
+00002890: 6865 2064 6972 6563 746f 7279 2069 6e20  he directory in 
+000028a0: 7768 6963 6820 7265 7375 6c74 730a 2020  which results.  
+000028b0: 2020 2020 2020 2020 2020 7368 6f75 6c64            should
+000028c0: 2062 6520 7361 7665 642e 0a20 2020 2020   be saved..     
+000028d0: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+000028e0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+000028f0: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
+00002900: 2902 da07 7061 7274 6961 6cda 0466 756c  )...partial..ful
+00002910: 6c72 5f00 0000 da0b 7061 7274 6961 6c5f  lr_.....partial_
+00002920: 7073 6972 6000 0000 da03 7073 69da 0c70  psir`.....psi..p
+00002930: 6172 7469 616c 5f73 6861 70da 0473 6861  artial_shap..sha
+00002940: 70da 0c70 6172 7469 616c 5f6c 7361 61da  p..partial_lsaa.
+00002950: 046c 7361 6154 7a04 2e63 7376 721d 0000  .lsaaTz..csvr...
+00002960: 007a 0277 2b72 4d00 0000 724e 0000 0029  .z.w+rM...rN...)
+00002970: 01da 0a66 6965 6c64 6e61 6d65 734e 291a  ...fieldnamesN).
+00002980: 722b 0000 0072 2d00 0000 722e 0000 0072  r+...r-...r....r
+00002990: 2f00 0000 7233 0000 005a 1363 616c 6375  /...r3...Z.calcu
+000029a0: 6c61 7465 5f66 696e 616c 5f70 7369 7230  late_final_psir0
+000029b0: 0000 0072 3500 0000 5a14 6361 6c63 756c  ...r5...Z.calcul
+000029c0: 6174 655f 6669 6e61 6c5f 7368 6170 7236  ate_final_shapr6
+000029d0: 0000 005a 1463 616c 6375 6c61 7465 5f66  ...Z.calculate_f
+000029e0: 696e 616c 5f6c 7361 6172 1700 0000 7259  inal_lsaar....rY
+000029f0: 0000 0072 3900 0000 7254 0000 0072 5500  ...r9...rT...rU.
+00002a00: 0000 da03 7374 7272 0d00 0000 722c 0000  ....strr....r,..
+00002a10: 0072 5300 0000 7256 0000 00da 0a44 6963  .rS...rV.....Dic
+00002a20: 7457 7269 7465 72da 0b77 7269 7465 6865  tWriter..writehe
+00002a30: 6164 6572 7258 0000 0072 1800 0000 da04  aderrX...r......
+00002a40: 6b65 7973 2911 723c 0000 0072 5400 0000  keys).r<...rT...
+00002a50: da07 7265 7375 6c74 7372 6100 0000 7262  ..resultsra...rb
+00002a60: 0000 0072 6300 0000 7264 0000 0072 6500  ...rc...rd...re.
+00002a70: 0000 7266 0000 00da 066d 6574 7269 63da  ..rf.....metric.
+00002a80: 0676 616c 7565 735a 0673 5f70 6174 6872  .valuesZ.s_pathr
+00002a90: 5b00 0000 725a 0000 0072 5c00 0000 721d  [...rZ...r\...r.
+00002aa0: 0000 00da 0372 6f77 721b 0000 0072 1b00  .....rowr....r..
+00002ab0: 0000 721e 0000 00da 1166 696e 616c 697a  ..r......finaliz
+00002ac0: 655f 7472 6163 6b69 6e67 4f01 0000 7354  e_trackingO...sT
+00002ad0: 0000 000a 1106 0204 0106 0204 0106 020e  ................
+00002ae0: 010c 010c 0106 020e 010c 010c 0106 020e  ................
+00002af0: 010c 010c 010a 0214 0116 0106 010a 0110  ................
+00002b00: 010e 0108 0110 0108 010c 0102 fe1c fd02  ................
+00002b10: 800a 0714 0116 0108 0110 010e 0108 010c  ................
+00002b20: 011c fd02 8004 047a 2445 7661 6c75 6174  .......z$Evaluat
+00002b30: 696f 6e5f 4d61 6e61 6765 722e 6669 6e61  ion_Manager.fina
+00002b40: 6c69 7a65 5f74 7261 636b 696e 6729 024e  lize_tracking).N
+00002b50: 4e29 014e 2911 da08 5f5f 6e61 6d65 5f5f  N).N)...__name__
+00002b60: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00002b70: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+00002b80: 635f 5fda 0464 6963 7472 0600 0000 da04  c__..dictr......
+00002b90: 6c69 7374 da03 696e 7472 3f00 0000 7244  list..intr?...rD
+00002ba0: 0000 0072 4700 0000 7208 0000 0072 4800  ...rG...r....rH.
+00002bb0: 0000 7209 0000 0072 5e00 0000 7268 0000  ..r....r^...rh..
+00002bc0: 0072 7000 0000 721b 0000 0072 1b00 0000  .rp...r....r....
+00002bd0: 721b 0000 0072 1e00 0000 720a 0000 000e  r....r....r.....
+00002be0: 0000 0073 4800 0000 0800 0401 020e 0201  ...sH...........
+00002bf0: 04fc 0201 02ff 0202 02fe 0203 02fd 0204  ................
+00002c00: 02fc 0204 0afc 007f 020f 0201 0aff 0212  ................
+00002c10: 0201 0aff 0211 0201 0aff 0212 0201 02ff  ................
+00002c20: 0202 02fe 0203 0afd 0273 04ff 0201 0eff  .........s......
+00002c30: 720a 0000 0029 135a 2a61 736f 6369 6974  r....).Z*asociit
+00002c40: 612e 636f 6d70 6f6e 656e 7473 2e65 7661  a.components.eva
+00002c50: 6c75 6174 6f72 2e6f 725f 6576 616c 7561  luator.or_evalua
+00002c60: 746f 7272 0200 0000 5a2c 6173 6f63 6969  torr....Z,asocii
+00002c70: 7461 2e63 6f6d 706f 6e65 6e74 732e 6576  ta.components.ev
+00002c80: 616c 7561 746f 722e 6c73 6161 5f65 7661  aluator.lsaa_eva
+00002c90: 6c75 6174 6f72 7203 0000 005a 2e61 736f  luatorr....Z.aso
+00002ca0: 6369 6974 612e 636f 6d70 6f6e 656e 7473  ciita.components
+00002cb0: 2e65 7661 6c75 6174 6f72 2e73 616d 706c  .evaluator.sampl
+00002cc0: 655f 6576 616c 7561 746f 7272 0400 0000  e_evaluatorr....
+00002cd0: 7205 0000 00da 2761 736f 6369 6974 612e  r.....'asociita.
+00002ce0: 6d6f 6465 6c73 2e70 7974 6f72 6368 2e66  models.pytorch.f
+00002cf0: 6564 6572 6174 6564 5f6d 6f64 656c 7206  ederated_modelr.
+00002d00: 0000 005a 2661 736f 6369 6974 612e 6578  ...Z&asociita.ex
+00002d10: 6365 7074 696f 6e73 2e65 7661 6c75 6174  ceptions.evaluat
+00002d20: 6f72 6578 6365 7074 696f 6e72 0700 0000  orexceptionr....
+00002d30: da19 6173 6f63 6969 7461 2e75 7469 6c73  ..asociita.utils
+00002d40: 2e6f 7074 696d 697a 6572 7372 0800 0000  .optimizersr....
+00002d50: da0b 636f 6c6c 6563 7469 6f6e 7372 0900  ..collectionsr..
+00002d60: 0000 7242 0000 0072 3900 0000 7256 0000  ..rB...r9...rV..
+00002d70: 0072 0a00 0000 721b 0000 0072 1b00 0000  .r....r....r....
+00002d80: 721b 0000 0072 1e00 0000 da08 3c6d 6f64  r....r......<mod
+00002d90: 756c 653e 0100 0000 7318 0000 000c 000c  ule>....s.......
+00002da0: 010c 010c 010c 010c 010c 010c 0108 0108  ................
+00002db0: 0108 0112 03                             .....
```

### Comparing `asociita-0.3.2/asociita/components/evaluator/__pycache__/or_evaluator.cpython-310.pyc` & `asociita-0.3.3/asociita/components/evaluator/__pycache__/or_evaluator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/evaluator/__pycache__/sample_evaluator.cpython-310.pyc` & `asociita-0.3.3/asociita/components/evaluator/__pycache__/sample_evaluator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jul  4 14:39:59 2023 UTC, .py size: 18128 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3f2f a464 d046 0000  o.......?/.d.F..
+00000000: 6f0d 0d0a 0000 0000 ad95 b564 2748 0000  o..........d'H..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0007 0000 0040 0000 0073 c000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 5a04 6400  m.Z...d.d.l.Z.d.
 00000050: 6403 6c05 5a05 6400 6403 6c06 5a06 6400  d.l.Z.d.d.l.Z.d.
 00000060: 6404 6c07 6d08 5a08 6d09 5a09 0100 6400  d.l.m.Z.m.Z...d.
 00000070: 6405 6c0a 6d0b 5a0b 0100 6400 6406 6c0c  d.l.m.Z...d.d.l.
@@ -118,807 +118,814 @@
 00000750: 1600 0000 7217 0000 0072 1800 0000 5a0b  ....r....r....Z.
 00000760: 715f 6772 6164 6965 6e74 73da 0269 64da  q_gradients..id.
 00000770: 0467 7261 6472 0d00 0000 720d 0000 0072  .gradr....r....r
 00000780: 1100 0000 da10 7365 6c65 6374 5f67 7261  ......select_gra
 00000790: 6469 656e 7473 2100 0000 730c 0000 0004  dients!...s.....
 000007a0: 1310 0308 0108 0102 8004 0172 1c00 0000  ...........r....
 000007b0: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
-000007c0: 000c 0000 0040 0000 0073 6e00 0000 6500  .....@...sn...e.
+000007c0: 000f 0000 0040 0000 0073 7600 0000 6500  .....@...sv...e.
 000007d0: 5a01 6400 5a02 6401 5a03 6402 6504 6403  Z.d.Z.d.Z.d.e.d.
 000007e0: 6505 6404 6405 6606 6406 6407 8404 5a06  e.d.d.f.d.d...Z.
-000007f0: 6408 6507 6409 6504 640a 6508 640b 6505  d.e.d.e.d.e.d.e.
-00000800: 640c 6509 640d 6509 660c 640e 640f 8404  d.e.d.e.f.d.d...
-00000810: 5a0a 6404 650b 650c 6505 650c 8502 1900  Z.d.e.e.e.e.....
-00000820: 650c 6505 650d 8502 1900 6602 1900 6602  e.e.e.....f...f.
-00000830: 6410 6411 8404 5a0e 6405 5300 2912 da10  d.d...Z.d.S.)...
-00000840: 5361 6d70 6c65 5f45 7661 6c75 6174 6f72  Sample_Evaluator
-00000850: 6147 0100 0053 616d 706c 6520 6576 616c  aG...Sample eval
-00000860: 7561 746f 7220 6973 2075 7365 6420 746f  uator is used to
-00000870: 2065 7374 6162 6c69 7368 2074 6865 206d   establish the m
-00000880: 6172 6769 6e61 6c20 636f 6e74 7269 6275  arginal contribu
-00000890: 7469 6f6e 206f 6620 6561 6368 2073 616d  tion of each sam
-000008a0: 706c 6564 0a20 2020 2063 6c69 656e 7420  pled.    client 
-000008b0: 746f 2074 6865 2067 656e 6572 616c 2076  to the general v
-000008c0: 616c 7565 206f 6620 7468 6520 676c 6f62  alue of the glob
-000008d0: 616c 206d 6f64 656c 2e20 4261 7369 6320  al model. Basic 
-000008e0: 5361 6d70 6c65 2045 7661 6c75 6174 6f72  Sample Evaluator
-000008f0: 2069 7320 6162 6c65 2074 6f0a 2020 2020   is able to.    
-00000900: 6173 7365 7373 2074 6865 204c 6561 7665  assess the Leave
-00000910: 2d6f 6e65 2d6f 7574 2076 616c 7565 2066  -one-out value f
-00000920: 6f72 2065 7665 7279 2063 6c69 656e 7420  or every client 
-00000930: 696e 636c 7564 6564 2069 6e20 7468 6520  included in the 
-00000940: 7361 6d70 6c65 2e20 4974 2069 7320 616c  sample. It is al
-00000950: 736f 0a20 2020 2061 626c 6520 746f 2073  so.    able to s
-00000960: 756d 2074 6865 206d 6172 6769 6e61 6c20  um the marginal 
-00000970: 7661 6c75 6573 2074 6f20 6f62 6169 6e20  values to obain 
-00000980: 6120 6669 6e61 6c20 4c65 6176 652d 6f6e  a final Leave-on
-00000990: 652d 6f75 7420 7661 6c75 652e da05 6e6f  e-out value...no
-000009a0: 6465 73da 0a69 7465 7261 7469 6f6e 7372  des..iterationsr
-000009b0: 0c00 0000 4e63 0300 0000 0000 0000 0000  ....Nc..........
-000009c0: 0000 0300 0000 0300 0000 0300 0000 f32c  ...............,
-000009d0: 0000 0064 0164 0284 0088 0044 0083 017c  ...d.d.....D...|
-000009e0: 005f 0087 0066 0164 0364 0284 0874 017c  ._...f.d.d...t.|
-000009f0: 0283 0144 0083 017c 005f 0264 0453 0029  ...D...|._.d.S.)
-00000a00: 0561 af01 0000 436f 6e73 7472 7563 746f  .a....Constructo
-00000a10: 7220 666f 7220 7468 6520 5361 6d70 6c65  r for the Sample
-00000a20: 2045 7661 6c75 6174 6f72 2043 6c61 7373   Evaluator Class
-00000a30: 2e20 496e 6974 6961 6c69 7a65 7320 656d  . Initializes em
-00000a40: 7074 790a 2020 2020 2020 2020 6861 7368  pty.        hash
-00000a50: 2074 6162 6c65 7320 666f 7220 4c4f 4f20   tables for LOO 
-00000a60: 7661 6c75 6520 666f 7220 6561 6368 2069  value for each i
-00000a70: 7465 7261 7469 6f6e 2061 7320 7765 6c6c  teration as well
-00000a80: 2061 7320 6861 7368 2074 6162 6c65 0a20   as hash table. 
-00000a90: 2020 2020 2020 2066 6f72 2066 696e 616c         for final
-00000aa0: 204c 4f4f 2076 616c 7565 732e 0a20 2020   LOO values..   
-00000ab0: 2020 2020 200a 2020 2020 2020 2020 5061       .        Pa
-00000ac0: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-00000ad0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-00000ae0: 2020 2020 6e6f 6465 733a 206c 6973 740a      nodes: list.
-00000af0: 2020 2020 2020 2020 2020 2020 4120 6c69              A li
-00000b00: 7374 2063 6f6e 7461 696e 696e 6720 6964  st containing id
-00000b10: 7320 6f66 2061 6c6c 2074 6865 206e 6f64  s of all the nod
-00000b20: 6573 2065 6e67 6167 6564 2069 6e20 7468  es engaged in th
-00000b30: 6520 7472 6169 6e69 6e67 2e0a 2020 2020  e training..    
-00000b40: 2020 2020 6974 6572 6174 696f 6e73 3a20      iterations: 
-00000b50: 696e 740a 2020 2020 2020 2020 2020 2020  int.            
-00000b60: 4120 6e75 6d62 6572 206f 6620 7472 6169  A number of trai
-00000b70: 6e69 6e67 2069 7465 7261 7469 6f6e 730a  ning iterations.
-00000b80: 2020 2020 2020 2020 5265 7475 726e 730a          Returns.
-00000b90: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d0a          -------.
-00000ba0: 2020 2020 2020 2020 4e6f 6e65 0a20 2020          None.   
-00000bb0: 2020 2020 2063 0100 0000 0000 0000 0000       c..........
-00000bc0: 0000 0200 0000 0600 0000 5300 0000 f318  ..........S.....
-00000bd0: 0000 0069 007c 005d 087d 017c 0174 00a0  ...i.|.].}.|.t..
-00000be0: 0164 00a1 0193 0271 0253 00a9 0172 0100  .d.....q.S...r..
-00000bf0: 0000 a902 da02 6e70 da07 666c 6f61 7436  ......np..float6
-00000c00: 34a9 0272 0e00 0000 da04 6e6f 6465 720d  4..r......noder.
-00000c10: 0000 0072 0d00 0000 7211 0000 00da 0a3c  ...r....r......<
-00000c20: 6469 6374 636f 6d70 3e55 0000 00f3 0200  dictcomp>U......
-00000c30: 0000 1800 7a2d 5361 6d70 6c65 5f45 7661  ....z-Sample_Eva
-00000c40: 6c75 6174 6f72 2e5f 5f69 6e69 745f 5f2e  luator.__init__.
-00000c50: 3c6c 6f63 616c 733e 2e3c 6469 6374 636f  <locals>.<dictco
-00000c60: 6d70 3e63 0100 0000 0000 0000 0000 0000  mp>c............
-00000c70: 0200 0000 0500 0000 1300 0000 f31c 0000  ................
-00000c80: 0069 007c 005d 0a7d 017c 0164 0064 0184  .i.|.].}.|.d.d..
-00000c90: 0088 0044 0083 0193 0271 0253 0029 0263  ...D.....q.S.).c
-00000ca0: 0100 0000 0000 0000 0000 0000 0200 0000  ................
-00000cb0: 0600 0000 5300 0000 7221 0000 0072 2200  ....S...r!...r".
-00000cc0: 0000 7223 0000 0072 2600 0000 720d 0000  ..r#...r&...r...
-00000cd0: 0072 0d00 0000 7211 0000 0072 2800 0000  .r....r....r(...
-00000ce0: 5600 0000 7229 0000 007a 3853 616d 706c  V...r)...z8Sampl
-00000cf0: 655f 4576 616c 7561 746f 722e 5f5f 696e  e_Evaluator.__in
-00000d00: 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e 3c64  it__.<locals>.<d
-00000d10: 6963 7463 6f6d 703e 2e3c 6469 6374 636f  ictcomp>.<dictco
-00000d20: 6d70 3e72 0d00 0000 a902 720e 0000 00da  mp>r......r.....
-00000d30: 0572 6f75 6e64 a901 721e 0000 0072 0d00  .round..r....r..
-00000d40: 0000 7211 0000 0072 2800 0000 5600 0000  ..r....r(...V...
-00000d50: f302 0000 001c 004e 2903 da03 7073 6972  .......N)...psir
-00000d60: 1300 0000 da0b 7061 7274 6961 6c5f 7073  ......partial_ps
-00000d70: 69a9 03da 0473 656c 6672 1e00 0000 721f  i....selfr....r.
-00000d80: 0000 0072 0d00 0000 722d 0000 0072 1100  ...r....r-...r..
-00000d90: 0000 da08 5f5f 696e 6974 5f5f 4300 0000  ....__init__C...
-00000da0: 7304 0000 0010 121c 017a 1953 616d 706c  s........z.Sampl
-00000db0: 655f 4576 616c 7561 746f 722e 5f5f 696e  e_Evaluator.__in
-00000dc0: 6974 5f5f 7216 0000 00da 0f6e 6f64 6573  it__r......nodes
-00000dd0: 5f69 6e5f 7361 6d70 6c65 da09 6f70 7469  _in_sample..opti
-00000de0: 6d69 7a65 72da 0969 7465 7261 7469 6f6e  mizer..iteration
-00000df0: da0b 6669 6e61 6c5f 6d6f 6465 6cda 0e70  ..final_model..p
-00000e00: 7265 7669 6f75 735f 6d6f 6465 6c63 0700  revious_modelc..
-00000e10: 0000 0000 0000 0000 0000 1000 0000 0500  ................
-00000e20: 0000 4300 0000 7388 0000 007c 05a0 00a1  ..C...s....|....
-00000e30: 0064 0119 007d 077c 0244 005d 397d 087c  .d...}.|.D.]9}.|
-00000e40: 086a 017d 0974 02a0 037c 01a1 017d 0a7c  .j.}.t...|...}.|
-00000e50: 0a7c 093d 0074 02a0 037c 03a1 017d 0b74  .|.=.t...|...}.t
-00000e60: 02a0 037c 06a1 017d 0c74 04a0 057c 0aa1  ...|...}.t...|..
-00000e70: 017d 0d7c 0b6a 067c 0ca0 07a1 007c 0d64  .}.|.j.|.....|.d
-00000e80: 028d 027d 0e7c 0ca0 087c 0ea1 0101 007c  ...}.|...|.....|
-00000e90: 0ca0 00a1 0064 0119 007d 0f7c 077c 0f18  .....d...}.|.|..
-00000ea0: 007c 006a 097c 0419 007c 093c 0071 0864  .|.j.|...|.<.q.d
-00000eb0: 0353 0029 0461 c603 0000 4d65 7468 6f64  .S.).a....Method
-00000ec0: 2075 7365 6420 746f 2074 7261 636b 5f72   used to track_r
-00000ed0: 6573 756c 7473 2061 6674 6572 2065 6163  esults after eac
-00000ee0: 6820 7472 6169 6e69 6e67 2072 6f75 6e64  h training round
-00000ef0: 2e0a 2020 2020 2020 2020 4769 7665 6e20  ..        Given 
-00000f00: 7468 6520 6772 6169 646e 6574 732c 2069  the graidnets, i
-00000f10: 6473 206f 6620 7468 6520 6e6f 6465 7320  ds of the nodes 
-00000f20: 696e 636c 7564 6564 2069 6e20 7361 6d70  included in samp
-00000f30: 6c65 2c0a 2020 2020 2020 2020 6c61 7374  le,.        last
-00000f40: 2076 6572 7369 6f6e 206f 6620 7468 6520   version of the 
-00000f50: 6f70 7469 6d69 7a65 722c 2070 7265 7669  optimizer, previ
-00000f60: 6f75 7320 7665 7273 696f 6e20 6f66 2074  ous version of t
-00000f70: 6865 206d 6f64 656c 0a20 2020 2020 2020  he model.       
-00000f80: 2061 6e64 2074 6865 2075 7064 6174 6564   and the updated
-00000f90: 2076 6572 7369 6f6e 206f 6620 7468 6520   version of the 
-00000fa0: 6d6f 6465 6c2c 2069 7420 6361 6c63 756c  model, it calcul
-00000fb0: 6174 6573 2076 616c 7565 7320 6f66 0a20  ates values of. 
-00000fc0: 2020 2020 2020 2061 6c6c 2074 6865 206d         all the m
-00000fd0: 6172 6769 6e61 6c20 636f 6e74 7269 6275  arginal contribu
-00000fe0: 7469 6f6e 7320 7573 696e 6720 4c65 6176  tions using Leav
-00000ff0: 652d 6f6e 652d 6f75 7420 6d65 7468 6f64  e-one-out method
-00001000: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00001010: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00001020: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00001030: 0a20 2020 2020 2020 2067 7261 6469 656e  .        gradien
-00001040: 7473 3a20 4f72 6465 7265 6444 6963 740a  ts: OrderedDict.
-00001050: 2020 2020 2020 2020 2020 2020 416e 204f              An O
-00001060: 7264 6572 6564 4469 6374 2063 6f6e 7461  rderedDict conta
-00001070: 696e 696e 6720 6772 6164 6965 6e74 7320  ining gradients 
-00001080: 6f66 2074 6865 2073 616d 706c 6564 206e  of the sampled n
-00001090: 6f64 6573 2e0a 2020 2020 2020 2020 6e6f  odes..        no
-000010a0: 6465 735f 696e 5f73 616d 706c 653a 206c  des_in_sample: l
-000010b0: 6973 740a 2020 2020 2020 2020 2020 2020  ist.            
-000010c0: 4120 6c69 7374 2063 6f6e 7461 696e 696e  A list containin
-000010d0: 6720 6964 2773 206f 6620 7468 6520 6e6f  g id's of the no
-000010e0: 6465 7320 7468 6174 2077 6572 6520 7361  des that were sa
-000010f0: 6d70 6c65 642e 0a20 2020 2020 2020 2070  mpled..        p
-00001100: 7265 7669 6f75 735f 6f70 7469 6d69 7a65  revious_optimize
-00001110: 723a 204f 7074 696d 697a 6572 730a 2020  r: Optimizers.  
-00001120: 2020 2020 2020 2020 2020 416e 2069 6e73            An ins
-00001130: 7461 6e63 6520 6f66 2074 6865 2061 736f  tance of the aso
-00001140: 6369 6974 612e 4f70 7469 6d69 7a65 7273  ciita.Optimizers
-00001150: 2063 6c61 7373 2e0a 2020 2020 2020 2020   class..        
-00001160: 6974 6572 6174 696f 6e3a 2069 6e74 0a20  iteration: int. 
-00001170: 2020 2020 2020 2020 2020 2054 6865 2063             The c
-00001180: 7572 7265 6e74 2069 7465 7261 7469 6f6e  urrent iteration
-00001190: 2e0a 2020 2020 2020 2020 7072 6576 696f  ..        previo
-000011a0: 7573 5f6d 6f64 656c 3a20 4665 6465 7261  us_model: Federa
-000011b0: 7465 644d 6f64 656c 0a20 2020 2020 2020  tedModel.       
-000011c0: 2020 2020 2041 6e20 696e 7374 616e 6365       An instance
-000011d0: 206f 6620 7468 6520 4665 6465 7261 7465   of the Federate
-000011e0: 644d 6f64 656c 206f 626a 6563 742e 0a20  dModel object.. 
-000011f0: 2020 2020 2020 2075 7064 6174 6564 5f6d         updated_m
-00001200: 6f64 656c 3a20 4665 6465 7261 7465 644d  odel: FederatedM
-00001210: 6f64 656c 0a20 2020 2020 2020 2020 2020  odel.           
-00001220: 2041 6e20 696e 7374 616e 6365 206f 6620   An instance of 
-00001230: 7468 6520 4665 6465 7261 7465 644d 6f64  the FederatedMod
-00001240: 656c 206f 626a 6563 742e 0a20 2020 2020  el object..     
-00001250: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
-00001260: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
-00001270: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
-00001280: e901 0000 00a9 02da 0777 6569 6768 7473  .........weights
-00001290: da05 6465 6c74 614e 290a da0e 6576 616c  ..deltaN)...eval
-000012a0: 7561 7465 5f6d 6f64 656c da07 6e6f 6465  uate_model..node
-000012b0: 5f69 64da 0463 6f70 79da 0864 6565 7063  _id..copy..deepc
-000012c0: 6f70 7972 0200 0000 da0f 636f 6d70 7574  opyr......comput
-000012d0: 655f 6176 6572 6167 65da 0c66 6564 5f6f  e_average..fed_o
-000012e0: 7074 696d 697a 65da 0b67 6574 5f77 6569  ptimize..get_wei
-000012f0: 6768 7473 da0e 7570 6461 7465 5f77 6569  ghts..update_wei
-00001300: 6768 7473 7230 0000 0029 1072 3200 0000  ghtsr0...).r2...
-00001310: 7216 0000 0072 3400 0000 7235 0000 0072  r....r4...r5...r
-00001320: 3600 0000 7237 0000 0072 3800 0000 5a11  6...r7...r8...Z.
-00001330: 6669 6e61 6c5f 6d6f 6465 6c5f 7363 6f72  final_model_scor
-00001340: 6572 2700 0000 723e 0000 005a 126d 6172  er'...r>...Z.mar
-00001350: 6769 6e61 6c5f 6772 6164 6965 6e74 735a  ginal_gradientsZ
-00001360: 0e6d 6172 6769 6e61 6c5f 6f70 7469 6d5a  .marginal_optimZ
-00001370: 0e6d 6172 6769 6e61 6c5f 6d6f 6465 6c5a  .marginal_modelZ
-00001380: 116d 6172 6769 6e61 6c5f 6772 6164 5f61  .marginal_grad_a
-00001390: 7667 5a10 6d61 7267 696e 616c 5f77 6569  vgZ.marginal_wei
-000013a0: 6768 7473 5a14 6d61 7267 696e 616c 5f6d  ghtsZ.marginal_m
-000013b0: 6f64 656c 5f73 636f 7265 720d 0000 0072  odel_scorer....r
-000013c0: 0d00 0000 7211 0000 00da 0a75 7064 6174  ....r......updat
-000013d0: 655f 7073 6959 0000 0073 1e00 0000 0c21  e_psiY...s.....!
-000013e0: 0802 0601 0a03 0601 0a02 0a03 0a01 0a01  ................
-000013f0: 0201 06ff 0a02 0c01 1401 04f0 7a1b 5361  ............z.Sa
-00001400: 6d70 6c65 5f45 7661 6c75 6174 6f72 2e75  mple_Evaluator.u
-00001410: 7064 6174 655f 7073 6963 0100 0000 0000  pdate_psic......
-00001420: 0000 0000 0000 0400 0000 0800 0000 4300  ..............C.
-00001430: 0000 f346 0000 007c 006a 00a0 01a1 0044  ...F...|.j.....D
-00001440: 005d 177d 017c 01a0 02a1 0044 005d 105c  .].}.|.....D.].\
-00001450: 027d 027d 037c 006a 037c 0205 0019 0074  .}.}.|.j.|.....t
-00001460: 04a0 057c 03a1 0137 0003 003c 0071 0b71  ...|...7...<.q.q
-00001470: 057c 006a 007c 006a 0366 0253 0029 0161  .|.j.|.j.f.S.).a
-00001480: 0401 0000 4d65 7468 6f64 2075 7365 6420  ....Method used 
-00001490: 746f 2073 756d 2075 7020 616c 6c20 7468  to sum up all th
-000014a0: 6520 7061 7274 6961 6c20 4c4f 4f20 7363  e partial LOO sc
-000014b0: 6f72 6573 2074 6f20 6f62 7461 696e 0a20  ores to obtain. 
-000014c0: 2020 2020 2020 2061 2066 696e 616c 204c         a final L
-000014d0: 4f4f 2073 636f 7265 2066 6f72 2065 6163  OO score for eac
-000014e0: 6820 636c 6965 6e74 2e0a 2020 2020 2020  h client..      
-000014f0: 2020 0a20 2020 2020 2020 2050 6172 616d    .        Param
-00001500: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00001510: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00001520: 204e 6f6e 650a 2020 2020 2020 2020 0a20   None.        . 
-00001530: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-00001540: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00001550: 2020 2020 2020 2074 7570 6c65 5b64 6963         tuple[dic
-00001560: 745b 696e 743a 2064 6963 745d 2c20 6469  t[int: dict], di
-00001570: 6374 5b69 6e74 3a20 666c 6f61 745d 5d0a  ct[int: float]].
-00001580: 2020 2020 2020 2020 2906 7230 0000 00da          ).r0....
-00001590: 0676 616c 7565 7372 1900 0000 722f 0000  .valuesr....r/..
-000015a0: 0072 2400 0000 7225 0000 00a9 0472 3200  .r$...r%.....r2.
-000015b0: 0000 5a11 6974 6572 6174 696f 6e5f 7265  ..Z.iteration_re
-000015c0: 7375 6c74 7372 2700 0000 da05 7661 6c75  sultsr'.....valu
-000015d0: 6572 0d00 0000 720d 0000 0072 1100 0000  er....r....r....
-000015e0: da13 6361 6c63 756c 6174 655f 6669 6e61  ..calculate_fina
-000015f0: 6c5f 7073 698f 0000 0073 0a00 0000 0e0d  l_psi....s......
-00001600: 1001 1a01 02ff 0c02 7a24 5361 6d70 6c65  ........z$Sample
-00001610: 5f45 7661 6c75 6174 6f72 2e63 616c 6375  _Evaluator.calcu
-00001620: 6c61 7465 5f66 696e 616c 5f70 7369 290f  late_final_psi).
-00001630: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
-00001640: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
-00001650: 6d65 5f5f da07 5f5f 646f 635f 5fda 046c  me__..__doc__..l
-00001660: 6973 74da 0369 6e74 7233 0000 0072 0700  ist..intr3...r..
-00001670: 0000 7209 0000 0072 0600 0000 7245 0000  ..r....r....rE..
-00001680: 00da 0574 7570 6c65 da04 6469 6374 da05  ...tuple..dict..
-00001690: 666c 6f61 7472 4a00 0000 720d 0000 0072  floatrJ...r....r
-000016a0: 0d00 0000 720d 0000 0072 1100 0000 721d  ....r....r....r.
-000016b0: 0000 003d 0000 0073 2e00 0000 0800 0401  ...=...s........
-000016c0: 0205 0201 02ff 0202 02fe 0202 0afe 0216  ................
-000016d0: 0201 02ff 0202 02fe 0203 02fd 0204 02fc  ................
-000016e0: 0205 02fb 0206 0afa 2a36 721d 0000 0063  ........*6r....c
-000016f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001700: 0f00 0000 4000 0000 73a6 0000 0065 005a  ....@...s....e.Z
-00001710: 0164 005a 0264 015a 0364 0265 0464 0365  .d.Z.d.Z.d.e.d.e
-00001720: 0564 0464 0566 0664 0664 0784 045a 0609  .d.d.f.d.d...Z..
-00001730: 0864 1b64 0965 0764 0a65 0464 0b65 0864  .d.d.e.d.e.d.e.d
-00001740: 0c65 0564 0d65 0964 0e65 0a66 0c64 0f64  .e.d.e.d.e.f.d.d
-00001750: 1084 055a 0b09 1109 0864 1c64 0965 0764  ...Z.....d.d.e.d
-00001760: 0a65 0464 0b65 0864 0c65 0564 0d65 0964  .e.d.e.d.e.d.e.d
-00001770: 1265 0564 0e65 0a66 0e64 1364 1484 055a  .e.d.e.f.d.d...Z
-00001780: 0c64 1565 0464 0965 0764 0b65 0864 1665  .d.e.d.e.d.e.d.e
-00001790: 0964 0465 0d65 0465 0e66 0219 0066 0a64  .d.e.e.e.f...f.d
-000017a0: 1764 1884 045a 0f64 1964 1a84 005a 1064  .d...Z.d.d...Z.d
-000017b0: 0553 0029 1dda 1853 616d 706c 655f 5368  .S.)...Sample_Sh
-000017c0: 6170 6c65 795f 4576 616c 7561 746f 7261  apley_Evaluatora
-000017d0: 7101 0000 5361 6d70 6c65 2065 7661 6c75  q...Sample evalu
-000017e0: 6174 6f72 2069 7320 7573 6564 2074 6f20  ator is used to 
-000017f0: 6573 7461 626c 6973 6820 7468 6520 6d61  establish the ma
-00001800: 7267 696e 616c 2063 6f6e 7472 6962 7574  rginal contribut
-00001810: 696f 6e20 6f66 2065 6163 6820 7361 6d70  ion of each samp
-00001820: 6c65 640a 2020 2020 636c 6965 6e74 2074  led.    client t
-00001830: 6f20 7468 6520 6765 6e65 7261 6c20 7661  o the general va
-00001840: 6c75 6520 6f66 2074 6865 2067 6c6f 6261  lue of the globa
-00001850: 6c20 6d6f 6465 6c20 7573 696e 6720 5368  l model using Sh
-00001860: 6170 6c65 7920 5661 6c75 6520 6173 2061  apley Value as a
-00001870: 206d 6574 686f 6420 6f66 0a20 2020 2061   method of.    a
-00001880: 7373 6573 6d65 6e74 2e20 5368 6170 6c65  ssesment. Shaple
-00001890: 7920 5361 6d70 6c65 2045 7661 6c75 6174  y Sample Evaluat
-000018a0: 6f72 2069 7320 6162 6c65 2074 6f20 6173  or is able to as
-000018b0: 7365 7373 2074 6865 2053 6861 706c 6579  sess the Shapley
-000018c0: 2076 616c 7565 2066 6f72 2065 7665 7279   value for every
-000018d0: 200a 2020 2020 636c 6965 6e74 2069 6e63   .    client inc
-000018e0: 6c75 6465 6420 696e 2074 6865 2073 616d  luded in the sam
-000018f0: 706c 652e 2049 7420 6973 2061 6c73 6f20  ple. It is also 
-00001900: 6162 6c65 2074 6f20 7375 6d20 7468 6520  able to sum the 
-00001910: 6d61 7267 696e 616c 2076 616c 7565 7320  marginal values 
-00001920: 746f 206f 6261 696e 200a 2020 2020 6120  to obain .    a 
-00001930: 6669 6e61 6c20 5368 6170 6c65 7920 7661  final Shapley va
-00001940: 6c75 6573 2e72 1e00 0000 721f 0000 0072  lues.r....r....r
-00001950: 0c00 0000 4e63 0300 0000 0000 0000 0000  ....Nc..........
-00001960: 0000 0300 0000 0300 0000 0300 0000 7220  ..............r 
-00001970: 0000 0029 0561 bf01 0000 436f 6e73 7472  ...).a....Constr
-00001980: 7563 746f 7220 666f 7220 7468 6520 5368  uctor for the Sh
-00001990: 6170 6c65 7920 5361 6d70 6c65 2045 7661  apley Sample Eva
-000019a0: 6c75 6174 6f72 2043 6c61 7373 2e20 496e  luator Class. In
-000019b0: 6974 6961 6c69 7a65 7320 656d 7074 790a  itializes empty.
-000019c0: 2020 2020 2020 2020 6861 7368 2074 6162          hash tab
-000019d0: 6c65 7320 666f 7220 5368 6170 6c65 7920  les for Shapley 
-000019e0: 7661 6c75 6520 666f 7220 6561 6368 2069  value for each i
-000019f0: 7465 7261 7469 6f6e 2061 7320 7765 6c6c  teration as well
-00001a00: 2061 7320 6861 7368 2074 6162 6c65 0a20   as hash table. 
-00001a10: 2020 2020 2020 2066 6f72 2066 696e 616c         for final
-00001a20: 2053 6861 706c 6579 2076 616c 7565 732e   Shapley values.
-00001a30: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00001a40: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00001a50: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-00001a60: 2020 2020 2020 2020 6e6f 6465 733a 206c          nodes: l
-00001a70: 6973 740a 2020 2020 2020 2020 2020 2020  ist.            
-00001a80: 4120 6c69 7374 2063 6f6e 7461 696e 696e  A list containin
-00001a90: 6720 6964 7320 6f66 2061 6c6c 2074 6865  g ids of all the
-00001aa0: 206e 6f64 6573 2065 6e67 6167 6564 2069   nodes engaged i
-00001ab0: 6e20 7468 6520 7472 6169 6e69 6e67 2e0a  n the training..
-00001ac0: 2020 2020 2020 2020 6974 6572 6174 696f          iteratio
-00001ad0: 6e73 3a20 696e 740a 2020 2020 2020 2020  ns: int.        
-00001ae0: 2020 2020 4120 6e75 6d62 6572 206f 6620      A number of 
-00001af0: 7472 6169 6e69 6e67 2069 7465 7261 7469  training iterati
-00001b00: 6f6e 730a 2020 2020 2020 2020 5265 7475  ons.        Retu
-00001b10: 726e 730a 2020 2020 2020 2020 2d2d 2d2d  rns.        ----
-00001b20: 2d2d 2d0a 2020 2020 2020 2020 4e6f 6e65  ---.        None
-00001b30: 0a20 2020 2020 2020 2063 0100 0000 0000  .        c......
-00001b40: 0000 0000 0000 0200 0000 0600 0000 5300  ..............S.
-00001b50: 0000 7221 0000 0072 2200 0000 7223 0000  ..r!...r"...r#..
-00001b60: 0072 2600 0000 720d 0000 0072 0d00 0000  .r&...r....r....
-00001b70: 7211 0000 0072 2800 0000 ba00 0000 7229  r....r(.......r)
-00001b80: 0000 007a 3553 616d 706c 655f 5368 6170  ...z5Sample_Shap
-00001b90: 6c65 795f 4576 616c 7561 746f 722e 5f5f  ley_Evaluator.__
-00001ba0: 696e 6974 5f5f 2e3c 6c6f 6361 6c73 3e2e  init__.<locals>.
-00001bb0: 3c64 6963 7463 6f6d 703e 6301 0000 0000  <dictcomp>c.....
-00001bc0: 0000 0000 0000 0002 0000 0005 0000 0013  ................
-00001bd0: 0000 0072 2a00 0000 2902 6301 0000 0000  ...r*...).c.....
-00001be0: 0000 0000 0000 0002 0000 0006 0000 0053  ...............S
-00001bf0: 0000 0072 2100 0000 7222 0000 0072 2300  ...r!...r"...r#.
-00001c00: 0000 7226 0000 0072 0d00 0000 720d 0000  ..r&...r....r...
-00001c10: 0072 1100 0000 7228 0000 00bb 0000 0072  .r....r(.......r
-00001c20: 2900 0000 7a40 5361 6d70 6c65 5f53 6861  )...z@Sample_Sha
-00001c30: 706c 6579 5f45 7661 6c75 6174 6f72 2e5f  pley_Evaluator._
-00001c40: 5f69 6e69 745f 5f2e 3c6c 6f63 616c 733e  _init__.<locals>
-00001c50: 2e3c 6469 6374 636f 6d70 3e2e 3c64 6963  .<dictcomp>.<dic
-00001c60: 7463 6f6d 703e 720d 0000 0072 2b00 0000  tcomp>r....r+...
-00001c70: 722d 0000 0072 0d00 0000 7211 0000 0072  r-...r....r....r
-00001c80: 2800 0000 bb00 0000 722e 0000 004e 2903  (.......r....N).
-00001c90: da07 7368 6170 6c65 7972 1300 0000 da0f  ..shapleyr......
-00001ca0: 7061 7274 6961 6c5f 7368 6170 6c65 7972  partial_shapleyr
-00001cb0: 3100 0000 720d 0000 0072 2d00 0000 7211  1...r....r-...r.
-00001cc0: 0000 0072 3300 0000 a900 0000 7304 0000  ...r3.......s...
-00001cd0: 0010 111c 017a 2153 616d 706c 655f 5368  .....z!Sample_Sh
-00001ce0: 6170 6c65 795f 4576 616c 7561 746f 722e  apley_Evaluator.
-00001cf0: 5f5f 696e 6974 5f5f 5472 1600 0000 7234  __init__Tr....r4
-00001d00: 0000 0072 3500 0000 7236 0000 0072 3800  ...r5...r6...r8.
-00001d10: 0000 da11 7265 7475 726e 5f63 6f61 6c69  ....return_coali
-00001d20: 7469 6f6e 7363 0700 0000 0000 0000 0000  tionsc..........
-00001d30: 0000 1f00 0000 0800 0000 4300 0000 73f2  ..........C...s.
-00001d40: 0100 0064 017d 0764 0274 007c 0283 0113  ...d.}.d.t.|....
-00001d50: 0064 0118 007d 0869 007d 0964 0364 0484  .d...}.i.}.d.d..
-00001d60: 007c 0244 0083 017d 0274 016a 027c 0264  .|.D...}.t.j.|.d
-00001d70: 0564 068d 027d 0a7c 0244 005d da7d 0b64  .d...}.|.D.].}.d
-00001d80: 077d 0c74 016a 037c 0a7c 0b64 088d 027d  .}.t.j.|.|.d...}
-00001d90: 0d7c 0da0 04a1 0044 005d b77d 0e74 0574  .|.....D.].}.t.t
-00001da0: 067c 0e83 0183 017d 0f74 0574 067c 0e7c  .|.....}.t.t.|.|
-00001db0: 0b66 0117 0083 0183 017d 107c 09a0 077c  .f.......}.|...|
-00001dc0: 0fa1 0172 467c 097c 0f19 007d 116e 3d74  ...rF|.|...}.n=t
-00001dd0: 087c 079b 0064 097c 089b 0064 0a7c 0f9b  .|...d.|...d.|..
-00001de0: 009d 0583 0101 0074 097c 017c 0f64 0b8d  .......t.|.|.d..
-00001df0: 027d 1274 0aa0 0b7c 03a1 017d 1374 0aa0  .}.t...|...}.t..
-00001e00: 0b7c 05a1 017d 1474 0ca0 0d7c 12a1 017d  .|...}.t...|...}
-00001e10: 157c 136a 0e7c 14a0 0fa1 007c 1564 0c8d  .|.j.|.....|.d..
-00001e20: 027d 167c 14a0 107c 16a1 0101 007c 14a0  .}.|...|.....|..
-00001e30: 11a1 0064 0119 007d 117c 117c 097c 0f3c  ...d...}.|.|.|.<
-00001e40: 007c 0764 0137 007d 077c 09a0 077c 10a1  .|.d.7.}.|...|..
-00001e50: 0172 8d7c 097c 1019 007d 176e 3d74 087c  .r.|.|...}.n=t.|
-00001e60: 079b 0064 097c 089b 0064 0a7c 109b 009d  ...d.|...d.|....
-00001e70: 0583 0101 0074 097c 017c 1064 0b8d 027d  .....t.|.|.d...}
-00001e80: 1874 0aa0 0b7c 03a1 017d 1974 0aa0 0b7c  .t...|...}.t...|
-00001e90: 05a1 017d 1a74 0ca0 0d7c 18a1 017d 1b7c  ...}.t...|...}.|
-00001ea0: 196a 0e7c 1aa0 0fa1 007c 1b64 0c8d 027d  .j.|.....|.d...}
-00001eb0: 1c7c 1aa0 107c 1ca1 0101 007c 1aa0 11a1  .|...|.....|....
-00001ec0: 0064 0119 007d 177c 177c 097c 103c 007c  .d...}.|.|.|.<.|
-00001ed0: 0764 0137 007d 0774 12a0 1374 007c 0283  .d.7.}.t...t.|..
-00001ee0: 0164 0118 0074 007c 0f83 01a1 027d 1d64  .d...t.|.....}.d
-00001ef0: 017c 1d1b 007d 1e7c 0c7c 1e7c 177c 1118  .|...}.|.|.|.|..
-00001f00: 0014 0037 007d 0c71 2b7c 0c74 007c 0283  ...7.}.q+|.t.|..
-00001f10: 011b 007c 006a 147c 0419 007c 0b3c 007c  ...|.j.|...|.<.|
-00001f20: 0664 056b 0272 f67c 0902 0001 0053 0071  .d.k.r.|.....S.q
-00001f30: 1c64 0d53 0029 0e61 4204 0000 4d65 7468  .d.S.).aB...Meth
-00001f40: 6f64 2075 7365 6420 746f 2074 7261 636b  od used to track
-00001f50: 5f72 6573 756c 7473 2061 6674 6572 2065  _results after e
-00001f60: 6163 6820 7472 6169 6e69 6e67 2072 6f75  ach training rou
-00001f70: 6e64 2e0a 2020 2020 2020 2020 4769 7665  nd..        Give
-00001f80: 6e20 7468 6520 6772 6169 646e 6574 732c  n the graidnets,
-00001f90: 2069 6473 206f 6620 7468 6520 6e6f 6465   ids of the node
-00001fa0: 7320 696e 636c 7564 6564 2069 6e20 7361  s included in sa
-00001fb0: 6d70 6c65 2c0a 2020 2020 2020 2020 6c61  mple,.        la
-00001fc0: 7374 2076 6572 7369 6f6e 206f 6620 7468  st version of th
-00001fd0: 6520 6f70 7469 6d69 7a65 722c 2070 7265  e optimizer, pre
-00001fe0: 7669 6f75 7320 7665 7273 696f 6e20 6f66  vious version of
-00001ff0: 2074 6865 206d 6f64 656c 0a20 2020 2020   the model.     
-00002000: 2020 2061 6e64 2074 6865 2075 7064 6174     and the updat
-00002010: 6564 2076 6572 7369 6f6e 206f 6620 7468  ed version of th
-00002020: 6520 6d6f 6465 6c2c 2069 7420 6361 6c63  e model, it calc
-00002030: 756c 6174 6573 2076 616c 7565 7320 6f66  ulates values of
-00002040: 0a20 2020 2020 2020 2061 6c6c 2074 6865  .        all the
-00002050: 206d 6172 6769 6e61 6c20 636f 6e74 7269   marginal contri
-00002060: 6275 7469 6f6e 7320 7573 696e 6720 5368  butions using Sh
-00002070: 6170 6c65 7920 7661 6c75 652e 0a20 2020  apley value..   
-00002080: 2020 2020 200a 2020 2020 2020 2020 5061       .        Pa
-00002090: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
-000020a0: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
-000020b0: 2020 2020 6772 6164 6965 6e74 733a 204f      gradients: O
-000020c0: 7264 6572 6564 4469 6374 0a20 2020 2020  rderedDict.     
-000020d0: 2020 2020 2020 2041 6e20 4f72 6465 7265         An Ordere
-000020e0: 6444 6963 7420 636f 6e74 6169 6e69 6e67  dDict containing
-000020f0: 2067 7261 6469 656e 7473 206f 6620 7468   gradients of th
-00002100: 6520 7361 6d70 6c65 6420 6e6f 6465 732e  e sampled nodes.
-00002110: 0a20 2020 2020 2020 206e 6f64 6573 5f69  .        nodes_i
-00002120: 6e5f 7361 6d70 6c65 3a20 6c69 7374 0a20  n_sample: list. 
-00002130: 2020 2020 2020 2020 2020 2041 206c 6973             A lis
-00002140: 7420 636f 6e74 6169 6e69 6e67 2069 6427  t containing id'
-00002150: 7320 6f66 2074 6865 206e 6f64 6573 2074  s of the nodes t
-00002160: 6861 7420 7765 7265 2073 616d 706c 6564  hat were sampled
-00002170: 2e0a 2020 2020 2020 2020 7072 6576 696f  ..        previo
-00002180: 7573 5f6f 7074 696d 697a 6572 3a20 4f70  us_optimizer: Op
-00002190: 7469 6d69 7a65 7273 0a20 2020 2020 2020  timizers.       
-000021a0: 2020 2020 2041 6e20 696e 7374 616e 6365       An instance
-000021b0: 206f 6620 7468 6520 6173 6f63 6969 7461   of the asociita
-000021c0: 2e4f 7074 696d 697a 6572 7320 636c 6173  .Optimizers clas
-000021d0: 732e 0a20 2020 2020 2020 2069 7465 7261  s..        itera
-000021e0: 7469 6f6e 3a20 696e 740a 2020 2020 2020  tion: int.      
-000021f0: 2020 2020 2020 5468 6520 6375 7272 656e        The curren
-00002200: 7420 6974 6572 6174 696f 6e2e 0a20 2020  t iteration..   
-00002210: 2020 2020 2070 7265 7669 6f75 735f 6d6f       previous_mo
-00002220: 6465 6c3a 2046 6564 6572 6174 6564 4d6f  del: FederatedMo
-00002230: 6465 6c0a 2020 2020 2020 2020 2020 2020  del.            
-00002240: 416e 2069 6e73 7461 6e63 6520 6f66 2074  An instance of t
-00002250: 6865 2046 6564 6572 6174 6564 4d6f 6465  he FederatedMode
-00002260: 6c20 6f62 6a65 6374 2e0a 2020 2020 2020  l object..      
-00002270: 2020 7570 6461 7465 645f 6d6f 6465 6c3a    updated_model:
-00002280: 2046 6564 6572 6174 6564 4d6f 6465 6c0a   FederatedModel.
-00002290: 2020 2020 2020 2020 2020 2020 416e 2069              An i
-000022a0: 6e73 7461 6e63 6520 6f66 2074 6865 2046  nstance of the F
-000022b0: 6564 6572 6174 6564 4d6f 6465 6c20 6f62  ederatedModel ob
-000022c0: 6a65 6374 2e0a 2020 2020 2020 2020 7265  ject..        re
-000022d0: 7475 726e 5f63 6f61 6c69 7469 6f6e 733a  turn_coalitions:
-000022e0: 2062 6f6f 6c2c 2064 6566 6175 6c74 2074   bool, default t
-000022f0: 6f20 5472 7565 0a20 2020 2020 2020 2020  o True.         
-00002300: 2020 2049 6620 7365 7420 746f 2054 7275     If set to Tru
-00002310: 652c 206d 6574 686f 6420 7769 6c6c 2072  e, method will r
-00002320: 6574 7572 6e20 7661 6c75 652d 6d61 7070  eturn value-mapp
-00002330: 696e 6720 666f 7220 6576 6572 7920 636f  ing for every co
-00002340: 616c 6974 696f 6e2e 0a20 2020 2020 2020  alition..       
-00002350: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
-00002360: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
-00002370: 204e 6f6e 650a 2020 2020 2020 2020 7239   None.        r9
-00002380: 0000 00e9 0200 0000 6301 0000 0000 0000  ........c.......
-00002390: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
-000023a0: 00f3 1200 0000 6700 7c00 5d05 7d01 7c01  ......g.|.].}.|.
-000023b0: 6a00 9102 7102 5300 720d 0000 00a9 0172  j...q.S.r......r
-000023c0: 3e00 0000 7226 0000 0072 0d00 0000 720d  >...r&...r....r.
-000023d0: 0000 0072 1100 0000 da0a 3c6c 6973 7463  ...r......<listc
-000023e0: 6f6d 703e e800 0000 f302 0000 0012 007a  omp>...........z
-000023f0: 3853 616d 706c 655f 5368 6170 6c65 795f  8Sample_Shapley_
-00002400: 4576 616c 7561 746f 722e 7570 6461 7465  Evaluator.update
-00002410: 5f73 6861 702e 3c6c 6f63 616c 733e 2e3c  _shap.<locals>.<
-00002420: 6c69 7374 636f 6d70 3e54 a901 da0b 7265  listcomp>T....re
-00002430: 7475 726e 5f64 6963 74e7 0000 0000 0000  turn_dict.......
-00002440: 0000 a902 da0a 636f 616c 6974 696f 6e73  ......coalitions
-00002450: da0d 7365 6172 6368 6564 5f6e 6f64 657a  ..searched_nodez
-00002460: 0420 6f66 207a 203a 2066 6f72 6d69 6e67  . of z : forming
-00002470: 2061 6e64 2065 7661 6c75 6174 696e 6720   and evaluating 
-00002480: 7375 6273 6574 20a9 0272 1600 0000 7217  subset ..r....r.
-00002490: 0000 0072 3a00 0000 4e29 1572 1400 0000  ...r:...N).r....
-000024a0: 7203 0000 00da 0d66 6f72 6d5f 7375 7065  r......form_supe
-000024b0: 7273 6574 da0e 7365 6c65 6374 5f73 7562  rset..select_sub
-000024c0: 7365 7473 da04 6b65 7973 7251 0000 00da  sets..keysrQ....
-000024d0: 0673 6f72 7465 64da 0367 6574 da05 7072  .sorted..get..pr
-000024e0: 696e 7472 1c00 0000 723f 0000 0072 4000  intr....r?...r@.
-000024f0: 0000 7202 0000 0072 4100 0000 7242 0000  ..r....rA...rB..
-00002500: 0072 4300 0000 7244 0000 00da 0e71 7569  .rC...rD.....qui
-00002510: 636b 5f65 7661 6c75 6174 65da 046d 6174  ck_evaluate..mat
-00002520: 68da 0463 6f6d 6272 5600 0000 291f 7232  h..combrV...).r2
-00002530: 0000 0072 1600 0000 7234 0000 0072 3500  ...r....r4...r5.
-00002540: 0000 7236 0000 0072 3800 0000 7257 0000  ..r6...r8...rW..
-00002550: 00da 116f 7065 7261 7469 6f6e 5f63 6f75  ...operation_cou
-00002560: 6e74 6572 da14 6e75 6d62 6572 5f6f 665f  nter..number_of_
-00002570: 6f70 6572 6174 696f 6e73 da0f 7265 636f  operations..reco
-00002580: 7264 6564 5f76 616c 7565 73da 0873 7570  rded_values..sup
-00002590: 6572 7365 7472 2700 0000 da04 7368 6170  ersetr'.....shap
-000025a0: da01 53da 0173 da06 735f 776f 5f69 da05  ..S..s..s_wo_i..
-000025b0: 735f 775f 695a 0c73 5f77 6f5f 695f 7363  s_w_iZ.s_wo_i_sc
-000025c0: 6f72 655a 1073 5f77 6f5f 695f 6772 6164  oreZ.s_wo_i_grad
-000025d0: 6965 6e74 735a 0c73 5f77 6f5f 695f 6f70  ientsZ.s_wo_i_op
-000025e0: 7469 6d5a 0c73 5f77 6f5f 695f 6d6f 6465  timZ.s_wo_i_mode
-000025f0: 6c5a 0f73 5f77 6f5f 695f 6772 6164 5f61  lZ.s_wo_i_grad_a
-00002600: 7667 5a0e 735f 776f 5f69 5f77 6569 6768  vgZ.s_wo_i_weigh
-00002610: 7473 5a0b 735f 775f 695f 7363 6f72 655a  tsZ.s_w_i_scoreZ
-00002620: 0f73 5f77 5f69 5f67 7261 6469 656e 7473  .s_w_i_gradients
-00002630: 5a0b 735f 775f 695f 6f70 7469 6d5a 0b73  Z.s_w_i_optimZ.s
-00002640: 5f77 5f69 5f6d 6f64 656c 5a0e 735f 775f  _w_i_modelZ.s_w_
-00002650: 695f 6772 6164 5f61 7667 5a0d 735f 775f  i_grad_avgZ.s_w_
-00002660: 695f 7765 6967 6874 73da 0a73 616d 706c  i_weights..sampl
-00002670: 655f 706f 73da 0764 6976 6973 6f72 720d  e_pos..divisorr.
-00002680: 0000 0072 0d00 0000 7211 0000 00da 0b75  ...r....r......u
-00002690: 7064 6174 655f 7368 6170 be00 0000 7356  pdate_shap....sV
-000026a0: 0000 0004 2310 0104 030e 030e 0208 0304  ....#...........
-000026b0: 010e 020c 010c 0112 010a 030a 0118 020c  ................
-000026c0: 010a 010a 010a 0112 010a 010c 0108 0108  ................
-000026d0: 010a 030a 0118 020c 010a 010a 010a 0112  ................
-000026e0: 010a 010c 0108 0108 0118 0208 0212 0116  ................
-000026f0: 0108 0208 0102 ff04 d47a 2453 616d 706c  .........z$Sampl
-00002700: 655f 5368 6170 6c65 795f 4576 616c 7561  e_Shapley_Evalua
-00002710: 746f 722e 7570 6461 7465 5f73 6861 70e9  tor.update_shap.
-00002720: 1e00 0000 da11 6e75 6d62 6572 5f6f 665f  ......number_of_
-00002730: 776f 726b 6572 7363 0800 0000 0000 0000  workersc........
-00002740: 0000 0000 1b00 0000 0800 0000 0300 0000  ................
-00002750: 73ac 0100 0069 007d 0864 0164 0284 007c  s....i.}.d.d...|
-00002760: 0244 0083 017d 0274 006a 017c 0264 0364  .D...}.t.j.|.d.d
-00002770: 048d 027d 0964 057d 0a64 0674 027c 0283  ...}.d.}.d.t.|..
-00002780: 0113 0064 0718 007d 0b74 027c 0983 017c  ...d...}.t.|...|
-00002790: 066b 0072 2474 027c 0983 017d 0674 037c  .k.r$t.|...}.t.|
-000027a0: 097c 0664 088d 027d 0c74 047c 0683 018f  .|.d...}.t.|....
-000027b0: 3e89 027c 0c44 005d 337d 0d87 0087 0187  >..|.D.]3}......
-000027c0: 0287 0387 0466 0564 0964 0284 087c 0d44  .....f.d.d...|.D
-000027d0: 0083 017d 0e7c 0e44 005d 107d 0f7c 0fa0  ...}.|.D.].}.|..
-000027e0: 05a1 005c 027d 107d 117c 117c 0874 0674  ...\.}.}.|.|.t.t
-000027f0: 077c 1083 0183 013c 0071 427c 0a74 027c  .|.....<.qB|.t.|
-00002800: 0d83 0137 007d 0a74 0864 0a7c 0a9b 0064  ...7.}.t.d.|...d
-00002810: 0b7c 0b9b 0064 0c9d 0583 0101 0071 3157  .|...d.......q1W
-00002820: 0064 0d04 0004 0083 0301 006e 0831 0073  .d.........n.1.s
-00002830: 6f77 0101 0001 0001 0059 0001 0074 0864  ow.......Y...t.d
-00002840: 0e83 0101 007c 0244 005d 537d 1264 0f7d  .....|.D.]S}.d.}
-00002850: 1374 006a 097c 097c 1264 108d 027d 147c  .t.j.|.|.d...}.|
-00002860: 1444 005d 387d 1574 0674 077c 1583 0183  .D.]8}.t.t.|....
-00002870: 017d 1674 0aa0 0b7c 15a1 017d 177c 17a0  .}.t...|...}.|..
-00002880: 0c7c 12a1 0101 0074 0674 077c 1783 0183  .|.....t.t.|....
-00002890: 017d 1874 0da0 0e74 027c 0283 0164 0718  .}.t...t.|...d..
-000028a0: 0074 027c 1683 01a1 027d 1974 0f64 077c  .t.|.....}.t.d.|
-000028b0: 191b 0083 017d 1a7c 1374 0f7c 1a7c 087c  .....}.|.t.|.|.|
-000028c0: 1819 007c 087c 1619 0018 0014 0083 0137  ...|.|.........7
-000028d0: 007d 1371 8774 0f7c 1374 027c 0283 011b  .}.q.t.|.t.|....
-000028e0: 0083 0188 046a 107c 0419 007c 123c 0071  .....j.|...|.<.q
-000028f0: 7a7c 0764 116b 0272 d47c 0853 0064 0d53  z|.d.k.r.|.S.d.S
-00002900: 0029 1261 4905 0000 4d65 7468 6f64 2075  .).aI...Method u
-00002910: 7365 6420 746f 2074 7261 636b 5f72 6573  sed to track_res
-00002920: 756c 7473 2061 6674 6572 2065 6163 6820  ults after each 
-00002930: 7472 6169 6e69 6e67 2072 6f75 6e64 2e0a  training round..
-00002940: 2020 2020 2020 2020 5570 6461 7465 5f73          Update_s
-00002950: 6861 705f 6d75 6c74 6970 2069 7320 6120  hap_multip is a 
-00002960: 6465 6661 756c 7420 6d65 7468 6f64 2075  default method u
-00002970: 7365 6420 746f 2063 616c 6375 6c61 7465  sed to calculate
-00002980: 0a20 2020 2020 2020 2053 6861 706c 6579  .        Shapley
-00002990: 2072 6f75 6e64 2c20 6173 2069 7420 7573   round, as it us
-000029a0: 6573 2061 206e 756d 6265 7220 6f66 2077  es a number of w
-000029b0: 6f72 6b65 7273 2074 6f20 636f 6d70 6c65  orkers to comple
-000029c0: 7465 2061 2074 6173 6b2e 0a20 2020 200a  te a task..    .
-000029d0: 2020 2020 2020 2020 4769 7665 6e20 7468          Given th
-000029e0: 6520 6772 6169 646e 6574 732c 2069 6473  e graidnets, ids
-000029f0: 206f 6620 7468 6520 6e6f 6465 7320 696e   of the nodes in
-00002a00: 636c 7564 6564 2069 6e20 7361 6d70 6c65  cluded in sample
-00002a10: 2c0a 2020 2020 2020 2020 6c61 7374 2076  ,.        last v
-00002a20: 6572 7369 6f6e 206f 6620 7468 6520 6f70  ersion of the op
-00002a30: 7469 6d69 7a65 722c 2070 7265 7669 6f75  timizer, previou
-00002a40: 7320 7665 7273 696f 6e20 6f66 2074 6865  s version of the
-00002a50: 206d 6f64 656c 0a20 2020 2020 2020 2061   model.        a
-00002a60: 6e64 2074 6865 2075 7064 6174 6564 2076  nd the updated v
-00002a70: 6572 7369 6f6e 206f 6620 7468 6520 6d6f  ersion of the mo
-00002a80: 6465 6c2c 2069 7420 6361 6c63 756c 6174  del, it calculat
-00002a90: 6573 2076 616c 7565 7320 6f66 0a20 2020  es values of.   
-00002aa0: 2020 2020 2061 6c6c 2074 6865 206d 6172       all the mar
-00002ab0: 6769 6e61 6c20 636f 6e74 7269 6275 7469  ginal contributi
-00002ac0: 6f6e 7320 7573 696e 6720 5368 6170 6c65  ons using Shaple
-00002ad0: 7920 7661 6c75 652e 0a20 2020 2020 2020  y value..       
-00002ae0: 200a 2020 2020 2020 2020 5061 7261 6d65   .        Parame
-00002af0: 7465 7273 0a20 2020 2020 2020 202d 2d2d  ters.        ---
-00002b00: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
-00002b10: 6772 6164 6965 6e74 733a 204f 7264 6572  gradients: Order
-00002b20: 6564 4469 6374 0a20 2020 2020 2020 2020  edDict.         
-00002b30: 2020 2041 6e20 4f72 6465 7265 6444 6963     An OrderedDic
-00002b40: 7420 636f 6e74 6169 6e69 6e67 2067 7261  t containing gra
-00002b50: 6469 656e 7473 206f 6620 7468 6520 7361  dients of the sa
-00002b60: 6d70 6c65 6420 6e6f 6465 732e 0a20 2020  mpled nodes..   
-00002b70: 2020 2020 206e 6f64 6573 5f69 6e5f 7361       nodes_in_sa
-00002b80: 6d70 6c65 3a20 6c69 7374 0a20 2020 2020  mple: list.     
-00002b90: 2020 2020 2020 2041 206c 6973 7420 636f         A list co
-00002ba0: 6e74 6169 6e69 6e67 2069 6427 7320 6f66  ntaining id's of
-00002bb0: 2074 6865 206e 6f64 6573 2074 6861 7420   the nodes that 
-00002bc0: 7765 7265 2073 616d 706c 6564 2e0a 2020  were sampled..  
-00002bd0: 2020 2020 2020 7072 6576 696f 7573 5f6f        previous_o
-00002be0: 7074 696d 697a 6572 3a20 4f70 7469 6d69  ptimizer: Optimi
-00002bf0: 7a65 7273 0a20 2020 2020 2020 2020 2020  zers.           
-00002c00: 2041 6e20 696e 7374 616e 6365 206f 6620   An instance of 
-00002c10: 7468 6520 6173 6f63 6969 7461 2e4f 7074  the asociita.Opt
-00002c20: 696d 697a 6572 7320 636c 6173 732e 0a20  imizers class.. 
-00002c30: 2020 2020 2020 2069 7465 7261 7469 6f6e         iteration
-00002c40: 3a20 696e 740a 2020 2020 2020 2020 2020  : int.          
-00002c50: 2020 5468 6520 6375 7272 656e 7420 6974    The current it
-00002c60: 6572 6174 696f 6e2e 0a20 2020 2020 2020  eration..       
-00002c70: 2070 7265 7669 6f75 735f 6d6f 6465 6c3a   previous_model:
-00002c80: 2046 6564 6572 6174 6564 4d6f 6465 6c0a   FederatedModel.
-00002c90: 2020 2020 2020 2020 2020 2020 416e 2069              An i
-00002ca0: 6e73 7461 6e63 6520 6f66 2074 6865 2046  nstance of the F
-00002cb0: 6564 6572 6174 6564 4d6f 6465 6c20 6f62  ederatedModel ob
-00002cc0: 6a65 6374 2e0a 2020 2020 2020 2020 7570  ject..        up
-00002cd0: 6461 7465 645f 6d6f 6465 6c3a 2046 6564  dated_model: Fed
-00002ce0: 6572 6174 6564 4d6f 6465 6c0a 2020 2020  eratedModel.    
-00002cf0: 2020 2020 2020 2020 416e 2069 6e73 7461          An insta
-00002d00: 6e63 6520 6f66 2074 6865 2046 6564 6572  nce of the Feder
-00002d10: 6174 6564 4d6f 6465 6c20 6f62 6a65 6374  atedModel object
-00002d20: 2e0a 2020 2020 2020 2020 6e75 6d62 6572  ..        number
-00002d30: 5f6f 665f 776f 726b 6572 733a 2069 6e74  _of_workers: int
-00002d40: 2c20 6465 6661 756c 7420 746f 2035 300a  , default to 50.
-00002d50: 2020 2020 2020 2020 2020 2020 4120 6e75              A nu
-00002d60: 6d62 6572 206f 6620 776f 726b 6572 7320  mber of workers 
-00002d70: 7468 6174 2077 696c 6c20 7369 6d75 6c74  that will simult
-00002d80: 616e 656f 7573 6c79 2077 6f72 6b20 6f6e  aneously work on
-00002d90: 2061 2074 6173 6b2e 0a20 2020 2020 2020   a task..       
-00002da0: 2072 6574 7572 6e5f 636f 616c 6974 696f   return_coalitio
-00002db0: 6e73 3a20 626f 6f6c 2c20 6465 6661 756c  ns: bool, defaul
-00002dc0: 7420 746f 2054 7275 650a 2020 2020 2020  t to True.      
-00002dd0: 2020 2020 2020 4966 2073 6574 2074 6f20        If set to 
-00002de0: 5472 7565 2c20 6d65 7468 6f64 2077 696c  True, method wil
-00002df0: 6c20 7265 7475 726e 2076 616c 7565 2d6d  l return value-m
-00002e00: 6170 7069 6e67 2066 6f72 2065 7665 7279  apping for every
-00002e10: 2063 6f61 6c69 7469 6f6e 2e0a 2020 2020   coalition..    
-00002e20: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
-00002e30: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
-00002e40: 2020 2020 4e6f 6e65 0a20 2020 2020 2020      None.       
-00002e50: 2063 0100 0000 0000 0000 0000 0000 0200   c..............
-00002e60: 0000 0300 0000 5300 0000 7259 0000 0072  ......S...rY...r
-00002e70: 0d00 0000 725a 0000 0072 2600 0000 720d  ....rZ...r&...r.
-00002e80: 0000 0072 0d00 0000 7211 0000 0072 5b00  ...r....r....r[.
-00002e90: 0000 4501 0000 725c 0000 007a 3f53 616d  ..E...r\...z?Sam
-00002ea0: 706c 655f 5368 6170 6c65 795f 4576 616c  ple_Shapley_Eval
-00002eb0: 7561 746f 722e 7570 6461 7465 5f73 6861  uator.update_sha
-00002ec0: 705f 6d75 6c74 6970 2e3c 6c6f 6361 6c73  p_multip.<locals
-00002ed0: 3e2e 3c6c 6973 7463 6f6d 703e 4672 5d00  >.<listcomp>Fr].
-00002ee0: 0000 7201 0000 0072 5800 0000 7239 0000  ..r....rX...r9..
-00002ef0: 0072 1000 0000 6301 0000 0000 0000 0000  .r....c.........
-00002f00: 0000 0002 0000 000b 0000 0013 0000 0073  ...............s
-00002f10: 3400 0000 6700 7c00 5d16 7d01 8802 a000  4...g.|.].}.....
-00002f20: 8804 6a01 7c01 7402 a003 8800 a101 7402  ..j.|.t.......t.
-00002f30: a003 8801 a101 7402 a003 8803 a101 6604  ......t.......f.
-00002f40: a102 9102 7102 5300 720d 0000 0029 04da  ....q.S.r....)..
-00002f50: 0b61 7070 6c79 5f61 7379 6e63 da0f 6573  .apply_async..es
-00002f60: 7461 626c 6973 685f 7661 6c75 6572 3f00  tablish_valuer?.
-00002f70: 0000 7240 0000 0029 0272 0e00 0000 da09  ..r@...).r......
-00002f80: 636f 616c 6974 696f 6ea9 0572 1600 0000  coalition..r....
-00002f90: 7235 0000 00da 0470 6f6f 6c72 3800 0000  r5.....poolr8...
-00002fa0: 7232 0000 0072 0d00 0000 7211 0000 0072  r2...r....r....r
-00002fb0: 5b00 0000 4f01 0000 730e 0000 0006 0002  [...O...s.......
-00002fc0: 030a fd08 0108 0108 010a fd7a 0a43 6f6d  ...........z.Com
-00002fd0: 706c 6574 6564 207a 0820 6f75 7420 6f66  pleted z. out of
-00002fe0: 207a 0b20 6f70 6572 6174 696f 6e73 4e7a   z. operationsNz
-00002ff0: 5f46 696e 6973 6865 6420 6576 616c 7561  _Finished evalua
-00003000: 7469 6e67 2061 6c6c 206f 6620 7468 6520  ting all of the 
-00003010: 636f 616c 6974 696f 6e73 2e20 436f 6d6d  coalitions. Comm
-00003020: 656e 6369 6e67 2063 616c 6375 6c61 7469  encing calculati
-00003030: 6f6e 206f 6620 696e 6469 7669 6475 616c  on of individual
-00003040: 2053 6861 706c 6579 2076 616c 7565 732e   Shapley values.
-00003050: 725f 0000 0072 6000 0000 5429 1172 0300  r_...r`...T).r..
-00003060: 0000 7264 0000 0072 1400 0000 7215 0000  ..rd...r....r...
-00003070: 0072 0400 0000 7268 0000 0072 5100 0000  .r....rh...rQ...
-00003080: 7267 0000 0072 6900 0000 7265 0000 0072  rg...ri...re...r
-00003090: 3f00 0000 7240 0000 00da 0661 7070 656e  ?...r@.....appen
-000030a0: 6472 6b00 0000 726c 0000 0072 5300 0000  drk...rl...rS...
-000030b0: 7256 0000 0029 1b72 3200 0000 7216 0000  rV...).r2...r...
-000030c0: 0072 3400 0000 7235 0000 0072 3600 0000  .r4...r5...r6...
-000030d0: 7238 0000 0072 7a00 0000 7257 0000 005a  r8...rz...rW...Z
-000030e0: 1163 6f61 6c69 7469 6f6e 5f72 6573 756c  .coalition_resul
-000030f0: 7473 7270 0000 0072 6d00 0000 726e 0000  tsrp...rm...rn..
-00003100: 00da 0763 6875 6e6b 6564 da05 6368 756e  ...chunked..chun
-00003110: 6bda 0772 6573 756c 7473 da06 7265 7375  k..results..resu
-00003120: 6c74 727d 0000 00da 0573 636f 7265 7227  ltr}.....scorer'
-00003130: 0000 0072 7100 0000 7272 0000 0072 7300  ...rq...rr...rs.
-00003140: 0000 7274 0000 005a 0673 5f63 6f70 7972  ..rt...Z.s_copyr
-00003150: 7500 0000 7276 0000 0072 7700 0000 720d  u...rv...rw...r.
-00003160: 0000 0072 7e00 0000 7211 0000 00da 1275  ...r~...r......u
-00003170: 7064 6174 655f 7368 6170 5f6d 756c 7469  pdate_shap_multi
-00003180: 701d 0100 0073 4800 0000 0427 0e01 0e01  p....sH....'....
-00003190: 0402 1001 0c01 0801 0c01 0a01 0801 1201  ................
-000031a0: 0203 06fd 0804 0c01 1201 0c01 1801 02f7  ................
-000031b0: 1cff 080b 0801 0401 0e01 0801 0c01 0a01  ................
-000031c0: 0a01 0c01 1801 0c01 1e01 1c02 0802 0401  ................
-000031d0: 04ff 7a2b 5361 6d70 6c65 5f53 6861 706c  ..z+Sample_Shapl
-000031e0: 6579 5f45 7661 6c75 6174 6f72 2e75 7064  ey_Evaluator.upd
-000031f0: 6174 655f 7368 6170 5f6d 756c 7469 7072  ate_shap_multipr
-00003200: 7d00 0000 da05 6d6f 6465 6c63 0500 0000  }.....modelc....
-00003210: 0000 0000 0000 0000 0800 0000 0400 0000  ................
-00003220: 4300 0000 7346 0000 0074 007c 027c 0164  C...sF...t.|.|.d
-00003230: 018d 027d 0274 01a0 027c 02a1 017d 057c  ...}.t...|...}.|
-00003240: 036a 037c 04a0 04a1 007c 0564 028d 027d  .j.|.....|.d...}
-00003250: 067c 04a0 057c 06a1 0101 007c 04a0 06a1  .|...|.....|....
-00003260: 0064 0319 007d 077c 017c 0766 0253 0029  .d...}.|.|.f.S.)
-00003270: 0461 9702 0000 4865 6c70 6572 206d 6574  .a....Helper met
-00003280: 686f 6420 7573 6564 2074 6f20 6573 7461  hod used to esta
-00003290: 626c 6973 6820 6120 7661 6c75 6520 6f66  blish a value of
-000032a0: 2061 2070 6172 7469 6375 6c61 7220 636f   a particular co
-000032b0: 616c 6974 696f 6e2e 0a20 2020 2020 2020  alition..       
-000032c0: 2043 616c 6c65 6420 6173 796e 6368 726f   Called asynchro
-000032d0: 6e6f 7573 6c79 2069 6e20 6d75 6c74 6970  nously in multip
-000032e0: 726f 6365 7373 6564 2076 6572 7369 6f6e  rocessed version
-000032f0: 206f 6620 7468 6520 7365 6c66 2e75 7064   of the self.upd
-00003300: 6174 655f 7368 6170 5f6d 756c 7469 7028  ate_shap_multip(
-00003310: 290a 2020 2020 2020 2020 6d65 7468 6f64  ).        method
-00003320: 2e0a 2020 2020 2020 2020 0a20 2020 2020  ..        .     
-00003330: 2020 2050 6172 616d 6574 6572 730a 2020     Parameters.  
-00003340: 2020 2020 2020 2d2d 2d2d 2d2d 2d2d 2d2d        ----------
-00003350: 0a20 2020 2020 2020 204e 6f6e 650a 2020  .        None.  
-00003360: 2020 2020 2020 6772 6164 6965 6e74 733a        gradients:
-00003370: 204f 7264 6572 6564 4469 6374 0a20 2020   OrderedDict.   
-00003380: 2020 2020 2020 2020 2041 6e20 4f72 6465           An Orde
-00003390: 7265 6444 6963 7420 636f 6e74 6169 6e69  redDict containi
-000033a0: 6e67 2067 7261 6469 656e 7473 206f 6620  ng gradients of 
-000033b0: 7468 6520 7361 6d70 6c65 6420 6e6f 6465  the sampled node
-000033c0: 732e 0a20 2020 2020 2020 2063 6f61 6c69  s..        coali
-000033d0: 7469 6f6e 3a20 6c69 7374 0a20 2020 2020  tion: list.     
-000033e0: 2020 2020 2020 2041 206c 6973 7420 636f         A list co
-000033f0: 6e74 6169 6e69 6e67 2069 6427 7320 6f66  ntaining id's of
-00003400: 2074 6865 206e 6f64 6573 2074 6861 7420   the nodes that 
-00003410: 7765 7265 2073 616d 706c 6564 2e0a 2020  were sampled..  
-00003420: 2020 2020 2020 6f70 7469 6d69 7a65 723a        optimizer:
-00003430: 204f 7074 696d 697a 6572 730a 2020 2020   Optimizers.    
-00003440: 2020 2020 2020 2020 416e 2069 6e73 7461          An insta
-00003450: 6e63 6520 6f66 2074 6865 2061 736f 6369  nce of the asoci
-00003460: 6974 612e 4f70 7469 6d69 7a65 7273 2063  ita.Optimizers c
-00003470: 6c61 7373 2e0a 2020 2020 2020 2020 6d6f  lass..        mo
-00003480: 6465 6c3a 2046 6564 6572 6174 6564 4d6f  del: FederatedMo
-00003490: 6465 6c0a 2020 2020 2020 2020 2020 2020  del.            
-000034a0: 416e 2069 6e73 7461 6e63 6520 6f66 2074  An instance of t
-000034b0: 6865 2046 6564 6572 6174 6564 4d6f 6465  he FederatedMode
-000034c0: 6c20 6f62 6a65 6374 2e0a 2020 2020 2020  l object..      
-000034d0: 2020 5265 7475 726e 730a 2020 2020 2020    Returns.      
-000034e0: 2020 2d2d 2d2d 2d2d 2d0a 2020 2020 2020    -------.      
-000034f0: 2020 7475 706c 655b 6c69 7374 2c20 666c    tuple[list, fl
-00003500: 6f61 745d 0a20 2020 2020 2020 2072 6300  oat].        rc.
-00003510: 0000 723a 0000 0072 3900 0000 2907 721c  ..r:...r9...).r.
-00003520: 0000 0072 0200 0000 7241 0000 0072 4200  ...r....rA...rB.
-00003530: 0000 7243 0000 0072 4400 0000 726a 0000  ..rC...rD...rj..
-00003540: 0029 0872 3200 0000 727d 0000 0072 1600  .).r2...r}...r..
-00003550: 0000 7235 0000 0072 8700 0000 da08 6772  ..r5...r......gr
-00003560: 6164 5f61 7667 723b 0000 0072 8500 0000  ad_avgr;...r....
-00003570: 720d 0000 0072 0d00 0000 7211 0000 0072  r....r....r....r
-00003580: 7c00 0000 6b01 0000 7310 0000 0004 1802  |...k...s.......
-00003590: 0106 ff0a 0212 010a 010c 0108 017a 2853  .............z(S
-000035a0: 616d 706c 655f 5368 6170 6c65 795f 4576  ample_Shapley_Ev
-000035b0: 616c 7561 746f 722e 6573 7461 626c 6973  aluator.establis
-000035c0: 685f 7661 6c75 6563 0100 0000 0000 0000  h_valuec........
-000035d0: 0000 0000 0400 0000 0800 0000 4300 0000  ............C...
-000035e0: 7246 0000 0029 0161 0c01 0000 4d65 7468  rF...).a....Meth
-000035f0: 6f64 2075 7365 6420 746f 2073 756d 2075  od used to sum u
-00003600: 7020 616c 6c20 7468 6520 7061 7274 6961  p all the partia
-00003610: 6c20 5368 6170 6c65 7920 7661 6c75 6573  l Shapley values
-00003620: 2074 6f20 6f62 7461 696e 0a20 2020 2020   to obtain.     
-00003630: 2020 2061 2066 696e 616c 2053 6861 706c     a final Shapl
-00003640: 6579 2073 636f 7265 2066 6f72 2065 6163  ey score for eac
-00003650: 6820 636c 6965 6e74 2e0a 2020 2020 2020  h client..      
-00003660: 2020 0a20 2020 2020 2020 2050 6172 616d    .        Param
-00003670: 6574 6572 730a 2020 2020 2020 2020 2d2d  eters.        --
-00003680: 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020 2020  --------.       
-00003690: 204e 6f6e 650a 2020 2020 2020 2020 0a20   None.        . 
-000036a0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-000036b0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-000036c0: 2020 2020 2020 2074 7570 6c65 5b64 6963         tuple[dic
-000036d0: 745b 696e 743a 2064 6963 745d 2c20 6469  t[int: dict], di
-000036e0: 6374 5b69 6e74 3a20 666c 6f61 745d 5d0a  ct[int: float]].
-000036f0: 2020 2020 2020 2020 2906 7256 0000 0072          ).rV...r
-00003700: 4700 0000 7219 0000 0072 5500 0000 7224  G...r....rU...r$
-00003710: 0000 0072 2500 0000 7248 0000 0072 0d00  ...r%...rH...r..
-00003720: 0000 720d 0000 0072 1100 0000 da14 6361  ..r....r......ca
-00003730: 6c63 756c 6174 655f 6669 6e61 6c5f 7368  lculate_final_sh
-00003740: 6170 8c01 0000 730a 0000 000e 0c10 011a  ap....s.........
-00003750: 0102 ff0c 027a 2d53 616d 706c 655f 5368  .....z-Sample_Sh
-00003760: 6170 6c65 795f 4576 616c 7561 746f 722e  apley_Evaluator.
-00003770: 6361 6c63 756c 6174 655f 6669 6e61 6c5f  calculate_final_
-00003780: 7368 6170 2901 5429 0272 7900 0000 5429  shap).T).ry...T)
-00003790: 1172 4b00 0000 724c 0000 0072 4d00 0000  .rK...rL...rM...
-000037a0: 724e 0000 0072 4f00 0000 7250 0000 0072  rN...rO...rP...r
-000037b0: 3300 0000 7207 0000 0072 0900 0000 7206  3...r....r....r.
-000037c0: 0000 00da 0462 6f6f 6c72 7800 0000 7286  .....boolrx...r.
-000037d0: 0000 0072 5100 0000 7253 0000 0072 7c00  ...rQ...rS...r|.
-000037e0: 0000 7289 0000 0072 0d00 0000 720d 0000  ..r....r....r...
-000037f0: 0072 0d00 0000 7211 0000 0072 5400 0000  .r....r....rT...
-00003800: a200 0000 7368 0000 0008 0004 0102 0602  ....sh..........
-00003810: 0102 ff02 0202 fe02 020a fe02 1b04 fa02  ................
-00003820: 0102 ff02 0202 fe02 0302 fd02 0402 fc02  ................
-00003830: 0502 fb02 060a fa02 6502 0104 f902 0102  ........e.......
-00003840: ff02 0202 fe02 0302 fd02 0402 fc02 0502  ................
-00003850: fb02 0602 fa02 070a f902 4e02 0102 ff02  ..........N.....
-00003860: 0202 fe02 0302 fd02 0402 fc0a 040a fc0c  ................
-00003870: 2172 5400 0000 2901 4629 1ada 1b61 736f  !rT...).F)...aso
-00003880: 6369 6974 612e 7574 696c 732e 636f 6d70  ciita.utils.comp
-00003890: 7574 6174 696f 6e73 7202 0000 0072 0300  utationsr....r..
-000038a0: 0000 da05 6e75 6d70 7972 2400 0000 723f  ....numpyr$...r?
-000038b0: 0000 0072 6b00 0000 da0f 6d75 6c74 6970  ...rk.....multip
-000038c0: 726f 6365 7373 696e 6772 0400 0000 7205  rocessingr....r.
-000038d0: 0000 00da 2761 736f 6369 6974 612e 6d6f  ....'asociita.mo
-000038e0: 6465 6c73 2e70 7974 6f72 6368 2e66 6564  dels.pytorch.fed
-000038f0: 6572 6174 6564 5f6d 6f64 656c 7206 0000  erated_modelr...
-00003900: 00da 0b63 6f6c 6c65 6374 696f 6e73 7207  ...collectionsr.
-00003910: 0000 00da 105f 636f 6c6c 6563 7469 6f6e  ....._collection
-00003920: 735f 6162 6372 0800 0000 da19 6173 6f63  s_abcr......asoc
-00003930: 6969 7461 2e75 7469 6c73 2e6f 7074 696d  iita.utils.optim
-00003940: 697a 6572 7372 0900 0000 da04 6974 6572  izersr......iter
-00003950: 7250 0000 0072 1500 0000 724f 0000 0072  rP...r....rO...r
-00003960: 8a00 0000 721c 0000 0072 1d00 0000 7254  ....r....r....rT
-00003970: 0000 0072 0d00 0000 720d 0000 0072 0d00  ...r....r....r..
-00003980: 0000 7211 0000 00da 083c 6d6f 6475 6c65  ..r......<module
-00003990: 3e01 0000 0073 2600 0000 0c00 0c01 0801  >....s&.........
-000039a0: 0801 0801 1001 0c01 0c01 0c01 0c01 1603  ................
-000039b0: 0216 08fe 0201 02ff 0202 0afe 0e1c 1265  ...............e
+000007f0: 0908 6414 6409 6507 640a 6504 640b 6508  ..d.d.e.d.e.d.e.
+00000800: 640c 6505 640d 6509 640e 6509 640f 650a  d.e.d.e.d.e.d.e.
+00000810: 660e 6410 6411 8405 5a0b 6404 650c 650d  f.d.d...Z.d.e.e.
+00000820: 6505 650d 8502 1900 650d 6505 650e 8502  e.e.....e.e.e...
+00000830: 1900 6602 1900 6602 6412 6413 8404 5a0f  ..f...f.d.d...Z.
+00000840: 6405 5300 2915 da10 5361 6d70 6c65 5f45  d.S.)...Sample_E
+00000850: 7661 6c75 6174 6f72 6147 0100 0053 616d  valuatoraG...Sam
+00000860: 706c 6520 6576 616c 7561 746f 7220 6973  ple evaluator is
+00000870: 2075 7365 6420 746f 2065 7374 6162 6c69   used to establi
+00000880: 7368 2074 6865 206d 6172 6769 6e61 6c20  sh the marginal 
+00000890: 636f 6e74 7269 6275 7469 6f6e 206f 6620  contribution of 
+000008a0: 6561 6368 2073 616d 706c 6564 0a20 2020  each sampled.   
+000008b0: 2063 6c69 656e 7420 746f 2074 6865 2067   client to the g
+000008c0: 656e 6572 616c 2076 616c 7565 206f 6620  eneral value of 
+000008d0: 7468 6520 676c 6f62 616c 206d 6f64 656c  the global model
+000008e0: 2e20 4261 7369 6320 5361 6d70 6c65 2045  . Basic Sample E
+000008f0: 7661 6c75 6174 6f72 2069 7320 6162 6c65  valuator is able
+00000900: 2074 6f0a 2020 2020 6173 7365 7373 2074   to.    assess t
+00000910: 6865 204c 6561 7665 2d6f 6e65 2d6f 7574  he Leave-one-out
+00000920: 2076 616c 7565 2066 6f72 2065 7665 7279   value for every
+00000930: 2063 6c69 656e 7420 696e 636c 7564 6564   client included
+00000940: 2069 6e20 7468 6520 7361 6d70 6c65 2e20   in the sample. 
+00000950: 4974 2069 7320 616c 736f 0a20 2020 2061  It is also.    a
+00000960: 626c 6520 746f 2073 756d 2074 6865 206d  ble to sum the m
+00000970: 6172 6769 6e61 6c20 7661 6c75 6573 2074  arginal values t
+00000980: 6f20 6f62 6169 6e20 6120 6669 6e61 6c20  o obain a final 
+00000990: 4c65 6176 652d 6f6e 652d 6f75 7420 7661  Leave-one-out va
+000009a0: 6c75 652e da05 6e6f 6465 73da 0a69 7465  lue...nodes..ite
+000009b0: 7261 7469 6f6e 7372 0c00 0000 4e63 0300  rationsr....Nc..
+000009c0: 0000 0000 0000 0000 0000 0300 0000 0300  ................
+000009d0: 0000 0300 0000 f32c 0000 0064 0164 0284  .......,...d.d..
+000009e0: 0088 0044 0083 017c 005f 0087 0066 0164  ...D...|._...f.d
+000009f0: 0364 0284 0874 017c 0283 0144 0083 017c  .d...t.|...D...|
+00000a00: 005f 0264 0453 0029 0561 af01 0000 436f  ._.d.S.).a....Co
+00000a10: 6e73 7472 7563 746f 7220 666f 7220 7468  nstructor for th
+00000a20: 6520 5361 6d70 6c65 2045 7661 6c75 6174  e Sample Evaluat
+00000a30: 6f72 2043 6c61 7373 2e20 496e 6974 6961  or Class. Initia
+00000a40: 6c69 7a65 7320 656d 7074 790a 2020 2020  lizes empty.    
+00000a50: 2020 2020 6861 7368 2074 6162 6c65 7320      hash tables 
+00000a60: 666f 7220 4c4f 4f20 7661 6c75 6520 666f  for LOO value fo
+00000a70: 7220 6561 6368 2069 7465 7261 7469 6f6e  r each iteration
+00000a80: 2061 7320 7765 6c6c 2061 7320 6861 7368   as well as hash
+00000a90: 2074 6162 6c65 0a20 2020 2020 2020 2066   table.        f
+00000aa0: 6f72 2066 696e 616c 204c 4f4f 2076 616c  or final LOO val
+00000ab0: 7565 732e 0a20 2020 2020 2020 200a 2020  ues..        .  
+00000ac0: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00000ad0: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00000ae0: 2d2d 2d0a 2020 2020 2020 2020 6e6f 6465  ---.        node
+00000af0: 733a 206c 6973 740a 2020 2020 2020 2020  s: list.        
+00000b00: 2020 2020 4120 6c69 7374 2063 6f6e 7461      A list conta
+00000b10: 696e 696e 6720 6964 7320 6f66 2061 6c6c  ining ids of all
+00000b20: 2074 6865 206e 6f64 6573 2065 6e67 6167   the nodes engag
+00000b30: 6564 2069 6e20 7468 6520 7472 6169 6e69  ed in the traini
+00000b40: 6e67 2e0a 2020 2020 2020 2020 6974 6572  ng..        iter
+00000b50: 6174 696f 6e73 3a20 696e 740a 2020 2020  ations: int.    
+00000b60: 2020 2020 2020 2020 4120 6e75 6d62 6572          A number
+00000b70: 206f 6620 7472 6169 6e69 6e67 2069 7465   of training ite
+00000b80: 7261 7469 6f6e 730a 2020 2020 2020 2020  rations.        
+00000b90: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+00000ba0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00000bb0: 4e6f 6e65 0a20 2020 2020 2020 2063 0100  None.        c..
+00000bc0: 0000 0000 0000 0000 0000 0200 0000 0600  ................
+00000bd0: 0000 5300 0000 f318 0000 0069 007c 005d  ..S........i.|.]
+00000be0: 087d 017c 0174 00a0 0164 00a1 0193 0271  .}.|.t...d.....q
+00000bf0: 0253 00a9 0172 0100 0000 a902 da02 6e70  .S...r........np
+00000c00: da07 666c 6f61 7436 34a9 0272 0e00 0000  ..float64..r....
+00000c10: da04 6e6f 6465 720d 0000 0072 0d00 0000  ..noder....r....
+00000c20: 7211 0000 00da 0a3c 6469 6374 636f 6d70  r......<dictcomp
+00000c30: 3e55 0000 00f3 0200 0000 1800 7a2d 5361  >U..........z-Sa
+00000c40: 6d70 6c65 5f45 7661 6c75 6174 6f72 2e5f  mple_Evaluator._
+00000c50: 5f69 6e69 745f 5f2e 3c6c 6f63 616c 733e  _init__.<locals>
+00000c60: 2e3c 6469 6374 636f 6d70 3e63 0100 0000  .<dictcomp>c....
+00000c70: 0000 0000 0000 0000 0200 0000 0500 0000  ................
+00000c80: 1300 0000 f31c 0000 0069 007c 005d 0a7d  .........i.|.].}
+00000c90: 017c 0164 0064 0184 0088 0044 0083 0193  .|.d.d.....D....
+00000ca0: 0271 0253 0029 0263 0100 0000 0000 0000  .q.S.).c........
+00000cb0: 0000 0000 0200 0000 0600 0000 5300 0000  ............S...
+00000cc0: 7221 0000 0072 2200 0000 7223 0000 0072  r!...r"...r#...r
+00000cd0: 2600 0000 720d 0000 0072 0d00 0000 7211  &...r....r....r.
+00000ce0: 0000 0072 2800 0000 5600 0000 7229 0000  ...r(...V...r)..
+00000cf0: 007a 3853 616d 706c 655f 4576 616c 7561  .z8Sample_Evalua
+00000d00: 746f 722e 5f5f 696e 6974 5f5f 2e3c 6c6f  tor.__init__.<lo
+00000d10: 6361 6c73 3e2e 3c64 6963 7463 6f6d 703e  cals>.<dictcomp>
+00000d20: 2e3c 6469 6374 636f 6d70 3e72 0d00 0000  .<dictcomp>r....
+00000d30: a902 720e 0000 00da 0572 6f75 6e64 a901  ..r......round..
+00000d40: 721e 0000 0072 0d00 0000 7211 0000 0072  r....r....r....r
+00000d50: 2800 0000 5600 0000 f302 0000 001c 004e  (...V..........N
+00000d60: 2903 da03 7073 6972 1300 0000 da0b 7061  )...psir......pa
+00000d70: 7274 6961 6c5f 7073 69a9 03da 0473 656c  rtial_psi....sel
+00000d80: 6672 1e00 0000 721f 0000 0072 0d00 0000  fr....r....r....
+00000d90: 722d 0000 0072 1100 0000 da08 5f5f 696e  r-...r......__in
+00000da0: 6974 5f5f 4300 0000 7304 0000 0010 121c  it__C...s.......
+00000db0: 017a 1953 616d 706c 655f 4576 616c 7561  .z.Sample_Evalua
+00000dc0: 746f 722e 5f5f 696e 6974 5f5f 5472 1600  tor.__init__Tr..
+00000dd0: 0000 da0f 6e6f 6465 735f 696e 5f73 616d  ....nodes_in_sam
+00000de0: 706c 65da 096f 7074 696d 697a 6572 da09  ple..optimizer..
+00000df0: 6974 6572 6174 696f 6eda 0b66 696e 616c  iteration..final
+00000e00: 5f6d 6f64 656c da0e 7072 6576 696f 7573  _model..previous
+00000e10: 5f6d 6f64 656c da11 7265 7475 726e 5f63  _model..return_c
+00000e20: 6f61 6c69 7469 6f6e 7363 0800 0000 0000  oalitionsc......
+00000e30: 0000 0000 0000 1200 0000 0600 0000 4300  ..............C.
+00000e40: 0000 73b8 0000 0069 007d 087c 05a0 00a1  ..s....i.}.|....
+00000e50: 0064 0119 007d 097c 097c 0874 017c 01a0  .d...}.|.|.t.|..
+00000e60: 02a1 0083 013c 007c 0244 005d 417d 0a7c  .....<.|.D.]A}.|
+00000e70: 0a6a 037d 0b74 04a0 057c 01a1 017d 0c7c  .j.}.t...|...}.|
+00000e80: 0c7c 0b3d 0074 04a0 057c 03a1 017d 0d74  .|.=.t...|...}.t
+00000e90: 04a0 057c 06a1 017d 0e74 06a0 077c 0ca1  ...|...}.t...|..
+00000ea0: 017d 0f7c 0d6a 087c 0ea0 09a1 007c 0f64  .}.|.j.|.....|.d
+00000eb0: 028d 027d 107c 0ea0 0a7c 10a1 0101 007c  ...}.|...|.....|
+00000ec0: 0ea0 00a1 0064 0119 007d 117c 097c 1118  .....d...}.|.|..
+00000ed0: 007c 006a 0b7c 0419 007c 0b3c 007c 117c  .|.j.|...|.<.|.|
+00000ee0: 0874 017c 0ca0 02a1 0083 013c 0071 127c  .t.|.......<.q.|
+00000ef0: 0764 036b 0272 5a7c 0853 0064 0453 0029  .d.k.rZ|.S.d.S.)
+00000f00: 0561 c603 0000 4d65 7468 6f64 2075 7365  .a....Method use
+00000f10: 6420 746f 2074 7261 636b 5f72 6573 756c  d to track_resul
+00000f20: 7473 2061 6674 6572 2065 6163 6820 7472  ts after each tr
+00000f30: 6169 6e69 6e67 2072 6f75 6e64 2e0a 2020  aining round..  
+00000f40: 2020 2020 2020 4769 7665 6e20 7468 6520        Given the 
+00000f50: 6772 6169 646e 6574 732c 2069 6473 206f  graidnets, ids o
+00000f60: 6620 7468 6520 6e6f 6465 7320 696e 636c  f the nodes incl
+00000f70: 7564 6564 2069 6e20 7361 6d70 6c65 2c0a  uded in sample,.
+00000f80: 2020 2020 2020 2020 6c61 7374 2076 6572          last ver
+00000f90: 7369 6f6e 206f 6620 7468 6520 6f70 7469  sion of the opti
+00000fa0: 6d69 7a65 722c 2070 7265 7669 6f75 7320  mizer, previous 
+00000fb0: 7665 7273 696f 6e20 6f66 2074 6865 206d  version of the m
+00000fc0: 6f64 656c 0a20 2020 2020 2020 2061 6e64  odel.        and
+00000fd0: 2074 6865 2075 7064 6174 6564 2076 6572   the updated ver
+00000fe0: 7369 6f6e 206f 6620 7468 6520 6d6f 6465  sion of the mode
+00000ff0: 6c2c 2069 7420 6361 6c63 756c 6174 6573  l, it calculates
+00001000: 2076 616c 7565 7320 6f66 0a20 2020 2020   values of.     
+00001010: 2020 2061 6c6c 2074 6865 206d 6172 6769     all the margi
+00001020: 6e61 6c20 636f 6e74 7269 6275 7469 6f6e  nal contribution
+00001030: 7320 7573 696e 6720 4c65 6176 652d 6f6e  s using Leave-on
+00001040: 652d 6f75 7420 6d65 7468 6f64 2e0a 2020  e-out method..  
+00001050: 2020 2020 2020 0a20 2020 2020 2020 2050        .        P
+00001060: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+00001070: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+00001080: 2020 2020 2067 7261 6469 656e 7473 3a20       gradients: 
+00001090: 4f72 6465 7265 6444 6963 740a 2020 2020  OrderedDict.    
+000010a0: 2020 2020 2020 2020 416e 204f 7264 6572          An Order
+000010b0: 6564 4469 6374 2063 6f6e 7461 696e 696e  edDict containin
+000010c0: 6720 6772 6164 6965 6e74 7320 6f66 2074  g gradients of t
+000010d0: 6865 2073 616d 706c 6564 206e 6f64 6573  he sampled nodes
+000010e0: 2e0a 2020 2020 2020 2020 6e6f 6465 735f  ..        nodes_
+000010f0: 696e 5f73 616d 706c 653a 206c 6973 740a  in_sample: list.
+00001100: 2020 2020 2020 2020 2020 2020 4120 6c69              A li
+00001110: 7374 2063 6f6e 7461 696e 696e 6720 6964  st containing id
+00001120: 2773 206f 6620 7468 6520 6e6f 6465 7320  's of the nodes 
+00001130: 7468 6174 2077 6572 6520 7361 6d70 6c65  that were sample
+00001140: 642e 0a20 2020 2020 2020 2070 7265 7669  d..        previ
+00001150: 6f75 735f 6f70 7469 6d69 7a65 723a 204f  ous_optimizer: O
+00001160: 7074 696d 697a 6572 730a 2020 2020 2020  ptimizers.      
+00001170: 2020 2020 2020 416e 2069 6e73 7461 6e63        An instanc
+00001180: 6520 6f66 2074 6865 2061 736f 6369 6974  e of the asociit
+00001190: 612e 4f70 7469 6d69 7a65 7273 2063 6c61  a.Optimizers cla
+000011a0: 7373 2e0a 2020 2020 2020 2020 6974 6572  ss..        iter
+000011b0: 6174 696f 6e3a 2069 6e74 0a20 2020 2020  ation: int.     
+000011c0: 2020 2020 2020 2054 6865 2063 7572 7265         The curre
+000011d0: 6e74 2069 7465 7261 7469 6f6e 2e0a 2020  nt iteration..  
+000011e0: 2020 2020 2020 7072 6576 696f 7573 5f6d        previous_m
+000011f0: 6f64 656c 3a20 4665 6465 7261 7465 644d  odel: FederatedM
+00001200: 6f64 656c 0a20 2020 2020 2020 2020 2020  odel.           
+00001210: 2041 6e20 696e 7374 616e 6365 206f 6620   An instance of 
+00001220: 7468 6520 4665 6465 7261 7465 644d 6f64  the FederatedMod
+00001230: 656c 206f 626a 6563 742e 0a20 2020 2020  el object..     
+00001240: 2020 2075 7064 6174 6564 5f6d 6f64 656c     updated_model
+00001250: 3a20 4665 6465 7261 7465 644d 6f64 656c  : FederatedModel
+00001260: 0a20 2020 2020 2020 2020 2020 2041 6e20  .            An 
+00001270: 696e 7374 616e 6365 206f 6620 7468 6520  instance of the 
+00001280: 4665 6465 7261 7465 644d 6f64 656c 206f  FederatedModel o
+00001290: 626a 6563 742e 0a20 2020 2020 2020 2052  bject..        R
+000012a0: 6574 7572 6e73 0a20 2020 2020 2020 202d  eturns.        -
+000012b0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 204e  ------.        N
+000012c0: 6f6e 650a 2020 2020 2020 2020 e901 0000  one.        ....
+000012d0: 00a9 02da 0777 6569 6768 7473 da05 6465  .....weights..de
+000012e0: 6c74 6154 4e29 0cda 0e65 7661 6c75 6174  ltaTN)...evaluat
+000012f0: 655f 6d6f 6465 6cda 0574 7570 6c65 da04  e_model..tuple..
+00001300: 6b65 7973 da07 6e6f 6465 5f69 64da 0463  keys..node_id..c
+00001310: 6f70 79da 0864 6565 7063 6f70 7972 0200  opy..deepcopyr..
+00001320: 0000 da0f 636f 6d70 7574 655f 6176 6572  ....compute_aver
+00001330: 6167 65da 0c66 6564 5f6f 7074 696d 697a  age..fed_optimiz
+00001340: 65da 0b67 6574 5f77 6569 6768 7473 da0e  e..get_weights..
+00001350: 7570 6461 7465 5f77 6569 6768 7473 7230  update_weightsr0
+00001360: 0000 0029 1272 3200 0000 7216 0000 0072  ...).r2...r....r
+00001370: 3400 0000 7235 0000 0072 3600 0000 7237  4...r5...r6...r7
+00001380: 0000 0072 3800 0000 7239 0000 00da 0f72  ...r8...r9.....r
+00001390: 6563 6f72 6465 645f 7661 6c75 6573 5a11  ecorded_valuesZ.
+000013a0: 6669 6e61 6c5f 6d6f 6465 6c5f 7363 6f72  final_model_scor
+000013b0: 6572 2700 0000 7241 0000 00da 126d 6172  er'...rA.....mar
+000013c0: 6769 6e61 6c5f 6772 6164 6965 6e74 73da  ginal_gradients.
+000013d0: 0e6d 6172 6769 6e61 6c5f 6f70 7469 6dda  .marginal_optim.
+000013e0: 0e6d 6172 6769 6e61 6c5f 6d6f 6465 6cda  .marginal_model.
+000013f0: 116d 6172 6769 6e61 6c5f 6772 6164 5f61  .marginal_grad_a
+00001400: 7667 da10 6d61 7267 696e 616c 5f77 6569  vg..marginal_wei
+00001410: 6768 7473 da14 6d61 7267 696e 616c 5f6d  ghts..marginal_m
+00001420: 6f64 656c 5f73 636f 7265 720d 0000 0072  odel_scorer....r
+00001430: 0d00 0000 7211 0000 00da 0a75 7064 6174  ....r......updat
+00001440: 655f 7073 6959 0000 0073 2800 0000 0421  e_psiY...s(....!
+00001450: 0c03 1002 0802 0601 0a03 0601 0a02 0a03  ................
+00001460: 0a01 0a01 0201 06ff 0a02 0c01 1201 1202  ................
+00001470: 0802 0401 04ff 7a1b 5361 6d70 6c65 5f45  ......z.Sample_E
+00001480: 7661 6c75 6174 6f72 2e75 7064 6174 655f  valuator.update_
+00001490: 7073 6963 0100 0000 0000 0000 0000 0000  psic............
+000014a0: 0400 0000 0800 0000 4300 0000 f346 0000  ........C....F..
+000014b0: 007c 006a 00a0 01a1 0044 005d 177d 017c  .|.j.....D.].}.|
+000014c0: 01a0 02a1 0044 005d 105c 027d 027d 037c  .....D.].\.}.}.|
+000014d0: 006a 037c 0205 0019 0074 04a0 057c 03a1  .j.|.....t...|..
+000014e0: 0137 0003 003c 0071 0b71 057c 006a 007c  .7...<.q.q.|.j.|
+000014f0: 006a 0366 0253 0029 0161 0401 0000 4d65  .j.f.S.).a....Me
+00001500: 7468 6f64 2075 7365 6420 746f 2073 756d  thod used to sum
+00001510: 2075 7020 616c 6c20 7468 6520 7061 7274   up all the part
+00001520: 6961 6c20 4c4f 4f20 7363 6f72 6573 2074  ial LOO scores t
+00001530: 6f20 6f62 7461 696e 0a20 2020 2020 2020  o obtain.       
+00001540: 2061 2066 696e 616c 204c 4f4f 2073 636f   a final LOO sco
+00001550: 7265 2066 6f72 2065 6163 6820 636c 6965  re for each clie
+00001560: 6e74 2e0a 2020 2020 2020 2020 0a20 2020  nt..        .   
+00001570: 2020 2020 2050 6172 616d 6574 6572 730a       Parameters.
+00001580: 2020 2020 2020 2020 2d2d 2d2d 2d2d 2d2d          --------
+00001590: 2d2d 0a20 2020 2020 2020 204e 6f6e 650a  --.        None.
+000015a0: 2020 2020 2020 2020 0a20 2020 2020 2020          .       
+000015b0: 2052 6574 7572 6e73 0a20 2020 2020 2020   Returns.       
+000015c0: 202d 2d2d 2d2d 2d2d 0a20 2020 2020 2020   -------.       
+000015d0: 2074 7570 6c65 5b64 6963 745b 696e 743a   tuple[dict[int:
+000015e0: 2064 6963 745d 2c20 6469 6374 5b69 6e74   dict], dict[int
+000015f0: 3a20 666c 6f61 745d 5d0a 2020 2020 2020  : float]].      
+00001600: 2020 2906 7230 0000 00da 0676 616c 7565    ).r0.....value
+00001610: 7372 1900 0000 722f 0000 0072 2400 0000  sr....r/...r$...
+00001620: 7225 0000 00a9 0472 3200 0000 da11 6974  r%.....r2.....it
+00001630: 6572 6174 696f 6e5f 7265 7375 6c74 7372  eration_resultsr
+00001640: 2700 0000 da05 7661 6c75 6572 0d00 0000  '.....valuer....
+00001650: 720d 0000 0072 1100 0000 da13 6361 6c63  r....r......calc
+00001660: 756c 6174 655f 6669 6e61 6c5f 7073 6999  ulate_final_psi.
+00001670: 0000 0073 0a00 0000 0e0d 1001 1a01 02ff  ...s............
+00001680: 0c02 7a24 5361 6d70 6c65 5f45 7661 6c75  ..z$Sample_Evalu
+00001690: 6174 6f72 2e63 616c 6375 6c61 7465 5f66  ator.calculate_f
+000016a0: 696e 616c 5f70 7369 a901 5429 10da 085f  inal_psi..T)..._
+000016b0: 5f6e 616d 655f 5fda 0a5f 5f6d 6f64 756c  _name__..__modul
+000016c0: 655f 5fda 0c5f 5f71 7561 6c6e 616d 655f  e__..__qualname_
+000016d0: 5fda 075f 5f64 6f63 5f5f da04 6c69 7374  _..__doc__..list
+000016e0: da03 696e 7472 3300 0000 7207 0000 0072  ..intr3...r....r
+000016f0: 0900 0000 7206 0000 00da 0462 6f6f 6c72  ....r......boolr
+00001700: 4f00 0000 723f 0000 00da 0464 6963 74da  O...r?.....dict.
+00001710: 0566 6c6f 6174 7255 0000 0072 0d00 0000  .floatrU...r....
+00001720: 720d 0000 0072 0d00 0000 7211 0000 0072  r....r....r....r
+00001730: 1d00 0000 3d00 0000 7334 0000 0008 0004  ....=...s4......
+00001740: 0102 0502 0102 ff02 0202 fe02 020a fe02  ................
+00001750: 1d04 f902 0102 ff02 0202 fe02 0302 fd02  ................
+00001760: 0402 fc02 0502 fb02 0602 fa02 070a f92a  ...............*
+00001770: 4072 1d00 0000 6300 0000 0000 0000 0000  @r....c.........
+00001780: 0000 0000 0000 000f 0000 0040 0000 0073  ...........@...s
+00001790: a600 0000 6500 5a01 6400 5a02 6401 5a03  ....e.Z.d.Z.d.Z.
+000017a0: 6402 6504 6403 6505 6404 6405 6606 6406  d.e.d.e.d.d.f.d.
+000017b0: 6407 8404 5a06 0908 641b 6409 6507 640a  d...Z...d.d.e.d.
+000017c0: 6504 640b 6508 640c 6505 640d 6509 640e  e.d.e.d.e.d.e.d.
+000017d0: 650a 660c 640f 6410 8405 5a0b 0911 0908  e.f.d.d...Z.....
+000017e0: 641c 6409 6507 640a 6504 640b 6508 640c  d.d.e.d.e.d.e.d.
+000017f0: 6505 640d 6509 6412 6505 640e 650a 660e  e.d.e.d.e.d.e.f.
+00001800: 6413 6414 8405 5a0c 6415 6504 6409 6507  d.d...Z.d.e.d.e.
+00001810: 640b 6508 6416 6509 6404 650d 6504 650e  d.e.d.e.d.e.e.e.
+00001820: 6602 1900 660a 6417 6418 8404 5a0f 6419  f...f.d.d...Z.d.
+00001830: 641a 8400 5a10 6405 5300 291d da18 5361  d...Z.d.S.)...Sa
+00001840: 6d70 6c65 5f53 6861 706c 6579 5f45 7661  mple_Shapley_Eva
+00001850: 6c75 6174 6f72 6171 0100 0053 616d 706c  luatoraq...Sampl
+00001860: 6520 6576 616c 7561 746f 7220 6973 2075  e evaluator is u
+00001870: 7365 6420 746f 2065 7374 6162 6c69 7368  sed to establish
+00001880: 2074 6865 206d 6172 6769 6e61 6c20 636f   the marginal co
+00001890: 6e74 7269 6275 7469 6f6e 206f 6620 6561  ntribution of ea
+000018a0: 6368 2073 616d 706c 6564 0a20 2020 2063  ch sampled.    c
+000018b0: 6c69 656e 7420 746f 2074 6865 2067 656e  lient to the gen
+000018c0: 6572 616c 2076 616c 7565 206f 6620 7468  eral value of th
+000018d0: 6520 676c 6f62 616c 206d 6f64 656c 2075  e global model u
+000018e0: 7369 6e67 2053 6861 706c 6579 2056 616c  sing Shapley Val
+000018f0: 7565 2061 7320 6120 6d65 7468 6f64 206f  ue as a method o
+00001900: 660a 2020 2020 6173 7365 736d 656e 742e  f.    assesment.
+00001910: 2053 6861 706c 6579 2053 616d 706c 6520   Shapley Sample 
+00001920: 4576 616c 7561 746f 7220 6973 2061 626c  Evaluator is abl
+00001930: 6520 746f 2061 7373 6573 7320 7468 6520  e to assess the 
+00001940: 5368 6170 6c65 7920 7661 6c75 6520 666f  Shapley value fo
+00001950: 7220 6576 6572 7920 0a20 2020 2063 6c69  r every .    cli
+00001960: 656e 7420 696e 636c 7564 6564 2069 6e20  ent included in 
+00001970: 7468 6520 7361 6d70 6c65 2e20 4974 2069  the sample. It i
+00001980: 7320 616c 736f 2061 626c 6520 746f 2073  s also able to s
+00001990: 756d 2074 6865 206d 6172 6769 6e61 6c20  um the marginal 
+000019a0: 7661 6c75 6573 2074 6f20 6f62 6169 6e20  values to obain 
+000019b0: 0a20 2020 2061 2066 696e 616c 2053 6861  .    a final Sha
+000019c0: 706c 6579 2076 616c 7565 732e 721e 0000  pley values.r...
+000019d0: 0072 1f00 0000 720c 0000 004e 6303 0000  .r....r....Nc...
+000019e0: 0000 0000 0000 0000 0003 0000 0003 0000  ................
+000019f0: 0003 0000 0072 2000 0000 2905 61bf 0100  .....r ...).a...
+00001a00: 0043 6f6e 7374 7275 6374 6f72 2066 6f72  .Constructor for
+00001a10: 2074 6865 2053 6861 706c 6579 2053 616d   the Shapley Sam
+00001a20: 706c 6520 4576 616c 7561 746f 7220 436c  ple Evaluator Cl
+00001a30: 6173 732e 2049 6e69 7469 616c 697a 6573  ass. Initializes
+00001a40: 2065 6d70 7479 0a20 2020 2020 2020 2068   empty.        h
+00001a50: 6173 6820 7461 626c 6573 2066 6f72 2053  ash tables for S
+00001a60: 6861 706c 6579 2076 616c 7565 2066 6f72  hapley value for
+00001a70: 2065 6163 6820 6974 6572 6174 696f 6e20   each iteration 
+00001a80: 6173 2077 656c 6c20 6173 2068 6173 6820  as well as hash 
+00001a90: 7461 626c 650a 2020 2020 2020 2020 666f  table.        fo
+00001aa0: 7220 6669 6e61 6c20 5368 6170 6c65 7920  r final Shapley 
+00001ab0: 7661 6c75 6573 2e0a 2020 2020 2020 2020  values..        
+00001ac0: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
+00001ad0: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
+00001ae0: 2d2d 2d2d 2d2d 0a20 2020 2020 2020 206e  ------.        n
+00001af0: 6f64 6573 3a20 6c69 7374 0a20 2020 2020  odes: list.     
+00001b00: 2020 2020 2020 2041 206c 6973 7420 636f         A list co
+00001b10: 6e74 6169 6e69 6e67 2069 6473 206f 6620  ntaining ids of 
+00001b20: 616c 6c20 7468 6520 6e6f 6465 7320 656e  all the nodes en
+00001b30: 6761 6765 6420 696e 2074 6865 2074 7261  gaged in the tra
+00001b40: 696e 696e 672e 0a20 2020 2020 2020 2069  ining..        i
+00001b50: 7465 7261 7469 6f6e 733a 2069 6e74 0a20  terations: int. 
+00001b60: 2020 2020 2020 2020 2020 2041 206e 756d             A num
+00001b70: 6265 7220 6f66 2074 7261 696e 696e 6720  ber of training 
+00001b80: 6974 6572 6174 696f 6e73 0a20 2020 2020  iterations.     
+00001b90: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00001ba0: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00001bb0: 2020 204e 6f6e 650a 2020 2020 2020 2020     None.        
+00001bc0: 6301 0000 0000 0000 0000 0000 0002 0000  c...............
+00001bd0: 0006 0000 0053 0000 0072 2100 0000 7222  .....S...r!...r"
+00001be0: 0000 0072 2300 0000 7226 0000 0072 0d00  ...r#...r&...r..
+00001bf0: 0000 720d 0000 0072 1100 0000 7228 0000  ..r....r....r(..
+00001c00: 00c4 0000 0072 2900 0000 7a35 5361 6d70  .....r)...z5Samp
+00001c10: 6c65 5f53 6861 706c 6579 5f45 7661 6c75  le_Shapley_Evalu
+00001c20: 6174 6f72 2e5f 5f69 6e69 745f 5f2e 3c6c  ator.__init__.<l
+00001c30: 6f63 616c 733e 2e3c 6469 6374 636f 6d70  ocals>.<dictcomp
+00001c40: 3e63 0100 0000 0000 0000 0000 0000 0200  >c..............
+00001c50: 0000 0500 0000 1300 0000 722a 0000 0029  ..........r*...)
+00001c60: 0263 0100 0000 0000 0000 0000 0000 0200  .c..............
+00001c70: 0000 0600 0000 5300 0000 7221 0000 0072  ......S...r!...r
+00001c80: 2200 0000 7223 0000 0072 2600 0000 720d  "...r#...r&...r.
+00001c90: 0000 0072 0d00 0000 7211 0000 0072 2800  ...r....r....r(.
+00001ca0: 0000 c500 0000 7229 0000 007a 4053 616d  ......r)...z@Sam
+00001cb0: 706c 655f 5368 6170 6c65 795f 4576 616c  ple_Shapley_Eval
+00001cc0: 7561 746f 722e 5f5f 696e 6974 5f5f 2e3c  uator.__init__.<
+00001cd0: 6c6f 6361 6c73 3e2e 3c64 6963 7463 6f6d  locals>.<dictcom
+00001ce0: 703e 2e3c 6469 6374 636f 6d70 3e72 0d00  p>.<dictcomp>r..
+00001cf0: 0000 722b 0000 0072 2d00 0000 720d 0000  ..r+...r-...r...
+00001d00: 0072 1100 0000 7228 0000 00c5 0000 0072  .r....r(.......r
+00001d10: 2e00 0000 4e29 03da 0773 6861 706c 6579  ....N)...shapley
+00001d20: 7213 0000 00da 0f70 6172 7469 616c 5f73  r......partial_s
+00001d30: 6861 706c 6579 7231 0000 0072 0d00 0000  hapleyr1...r....
+00001d40: 722d 0000 0072 1100 0000 7233 0000 00b3  r-...r....r3....
+00001d50: 0000 0073 0400 0000 1011 1c01 7a21 5361  ...s........z!Sa
+00001d60: 6d70 6c65 5f53 6861 706c 6579 5f45 7661  mple_Shapley_Eva
+00001d70: 6c75 6174 6f72 2e5f 5f69 6e69 745f 5f54  luator.__init__T
+00001d80: 7216 0000 0072 3400 0000 7235 0000 0072  r....r4...r5...r
+00001d90: 3600 0000 7238 0000 0072 3900 0000 6307  6...r8...r9...c.
+00001da0: 0000 0000 0000 0000 0000 001f 0000 0008  ................
+00001db0: 0000 0043 0000 0073 f201 0000 6401 7d07  ...C...s....d.}.
+00001dc0: 6402 7400 7c02 8301 1300 6401 1800 7d08  d.t.|.....d...}.
+00001dd0: 6900 7d09 6403 6404 8400 7c02 4400 8301  i.}.d.d...|.D...
+00001de0: 7d02 7401 6a02 7c02 6405 6406 8d02 7d0a  }.t.j.|.d.d...}.
+00001df0: 7c02 4400 5dda 7d0b 6407 7d0c 7401 6a03  |.D.].}.d.}.t.j.
+00001e00: 7c0a 7c0b 6408 8d02 7d0d 7c0d a004 a100  |.|.d...}.|.....
+00001e10: 4400 5db7 7d0e 7405 7406 7c0e 8301 8301  D.].}.t.t.|.....
+00001e20: 7d0f 7405 7406 7c0e 7c0b 6601 1700 8301  }.t.t.|.|.f.....
+00001e30: 8301 7d10 7c09 a007 7c0f a101 7246 7c09  ..}.|...|...rF|.
+00001e40: 7c0f 1900 7d11 6e3d 7408 7c07 9b00 6409  |...}.n=t.|...d.
+00001e50: 7c08 9b00 640a 7c0f 9b00 9d05 8301 0100  |...d.|.........
+00001e60: 7409 7c01 7c0f 640b 8d02 7d12 740a a00b  t.|.|.d...}.t...
+00001e70: 7c03 a101 7d13 740a a00b 7c05 a101 7d14  |...}.t...|...}.
+00001e80: 740c a00d 7c12 a101 7d15 7c13 6a0e 7c14  t...|...}.|.j.|.
+00001e90: a00f a100 7c15 640c 8d02 7d16 7c14 a010  ....|.d...}.|...
+00001ea0: 7c16 a101 0100 7c14 a011 a100 6401 1900  |.....|.....d...
+00001eb0: 7d11 7c11 7c09 7c0f 3c00 7c07 6401 3700  }.|.|.|.<.|.d.7.
+00001ec0: 7d07 7c09 a007 7c10 a101 728d 7c09 7c10  }.|...|...r.|.|.
+00001ed0: 1900 7d17 6e3d 7408 7c07 9b00 6409 7c08  ..}.n=t.|...d.|.
+00001ee0: 9b00 640a 7c10 9b00 9d05 8301 0100 7409  ..d.|.........t.
+00001ef0: 7c01 7c10 640b 8d02 7d18 740a a00b 7c03  |.|.d...}.t...|.
+00001f00: a101 7d19 740a a00b 7c05 a101 7d1a 740c  ..}.t...|...}.t.
+00001f10: a00d 7c18 a101 7d1b 7c19 6a0e 7c1a a00f  ..|...}.|.j.|...
+00001f20: a100 7c1b 640c 8d02 7d1c 7c1a a010 7c1c  ..|.d...}.|...|.
+00001f30: a101 0100 7c1a a011 a100 6401 1900 7d17  ....|.....d...}.
+00001f40: 7c17 7c09 7c10 3c00 7c07 6401 3700 7d07  |.|.|.<.|.d.7.}.
+00001f50: 7412 a013 7400 7c02 8301 6401 1800 7400  t...t.|...d...t.
+00001f60: 7c0f 8301 a102 7d1d 6401 7c1d 1b00 7d1e  |.....}.d.|...}.
+00001f70: 7c0c 7c1e 7c17 7c11 1800 1400 3700 7d0c  |.|.|.|.....7.}.
+00001f80: 712b 7c0c 7400 7c02 8301 1b00 7c00 6a14  q+|.t.|.....|.j.
+00001f90: 7c04 1900 7c0b 3c00 7c06 6405 6b02 72f6  |...|.<.|.d.k.r.
+00001fa0: 7c09 0200 0100 5300 711c 640d 5300 290e  |.....S.q.d.S.).
+00001fb0: 6142 0400 004d 6574 686f 6420 7573 6564  aB...Method used
+00001fc0: 2074 6f20 7472 6163 6b5f 7265 7375 6c74   to track_result
+00001fd0: 7320 6166 7465 7220 6561 6368 2074 7261  s after each tra
+00001fe0: 696e 696e 6720 726f 756e 642e 0a20 2020  ining round..   
+00001ff0: 2020 2020 2047 6976 656e 2074 6865 2067       Given the g
+00002000: 7261 6964 6e65 7473 2c20 6964 7320 6f66  raidnets, ids of
+00002010: 2074 6865 206e 6f64 6573 2069 6e63 6c75   the nodes inclu
+00002020: 6465 6420 696e 2073 616d 706c 652c 0a20  ded in sample,. 
+00002030: 2020 2020 2020 206c 6173 7420 7665 7273         last vers
+00002040: 696f 6e20 6f66 2074 6865 206f 7074 696d  ion of the optim
+00002050: 697a 6572 2c20 7072 6576 696f 7573 2076  izer, previous v
+00002060: 6572 7369 6f6e 206f 6620 7468 6520 6d6f  ersion of the mo
+00002070: 6465 6c0a 2020 2020 2020 2020 616e 6420  del.        and 
+00002080: 7468 6520 7570 6461 7465 6420 7665 7273  the updated vers
+00002090: 696f 6e20 6f66 2074 6865 206d 6f64 656c  ion of the model
+000020a0: 2c20 6974 2063 616c 6375 6c61 7465 7320  , it calculates 
+000020b0: 7661 6c75 6573 206f 660a 2020 2020 2020  values of.      
+000020c0: 2020 616c 6c20 7468 6520 6d61 7267 696e    all the margin
+000020d0: 616c 2063 6f6e 7472 6962 7574 696f 6e73  al contributions
+000020e0: 2075 7369 6e67 2053 6861 706c 6579 2076   using Shapley v
+000020f0: 616c 7565 2e0a 2020 2020 2020 2020 0a20  alue..        . 
+00002100: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+00002110: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+00002120: 2d2d 2d2d 0a20 2020 2020 2020 2067 7261  ----.        gra
+00002130: 6469 656e 7473 3a20 4f72 6465 7265 6444  dients: OrderedD
+00002140: 6963 740a 2020 2020 2020 2020 2020 2020  ict.            
+00002150: 416e 204f 7264 6572 6564 4469 6374 2063  An OrderedDict c
+00002160: 6f6e 7461 696e 696e 6720 6772 6164 6965  ontaining gradie
+00002170: 6e74 7320 6f66 2074 6865 2073 616d 706c  nts of the sampl
+00002180: 6564 206e 6f64 6573 2e0a 2020 2020 2020  ed nodes..      
+00002190: 2020 6e6f 6465 735f 696e 5f73 616d 706c    nodes_in_sampl
+000021a0: 653a 206c 6973 740a 2020 2020 2020 2020  e: list.        
+000021b0: 2020 2020 4120 6c69 7374 2063 6f6e 7461      A list conta
+000021c0: 696e 696e 6720 6964 2773 206f 6620 7468  ining id's of th
+000021d0: 6520 6e6f 6465 7320 7468 6174 2077 6572  e nodes that wer
+000021e0: 6520 7361 6d70 6c65 642e 0a20 2020 2020  e sampled..     
+000021f0: 2020 2070 7265 7669 6f75 735f 6f70 7469     previous_opti
+00002200: 6d69 7a65 723a 204f 7074 696d 697a 6572  mizer: Optimizer
+00002210: 730a 2020 2020 2020 2020 2020 2020 416e  s.            An
+00002220: 2069 6e73 7461 6e63 6520 6f66 2074 6865   instance of the
+00002230: 2061 736f 6369 6974 612e 4f70 7469 6d69   asociita.Optimi
+00002240: 7a65 7273 2063 6c61 7373 2e0a 2020 2020  zers class..    
+00002250: 2020 2020 6974 6572 6174 696f 6e3a 2069      iteration: i
+00002260: 6e74 0a20 2020 2020 2020 2020 2020 2054  nt.            T
+00002270: 6865 2063 7572 7265 6e74 2069 7465 7261  he current itera
+00002280: 7469 6f6e 2e0a 2020 2020 2020 2020 7072  tion..        pr
+00002290: 6576 696f 7573 5f6d 6f64 656c 3a20 4665  evious_model: Fe
+000022a0: 6465 7261 7465 644d 6f64 656c 0a20 2020  deratedModel.   
+000022b0: 2020 2020 2020 2020 2041 6e20 696e 7374           An inst
+000022c0: 616e 6365 206f 6620 7468 6520 4665 6465  ance of the Fede
+000022d0: 7261 7465 644d 6f64 656c 206f 626a 6563  ratedModel objec
+000022e0: 742e 0a20 2020 2020 2020 2075 7064 6174  t..        updat
+000022f0: 6564 5f6d 6f64 656c 3a20 4665 6465 7261  ed_model: Federa
+00002300: 7465 644d 6f64 656c 0a20 2020 2020 2020  tedModel.       
+00002310: 2020 2020 2041 6e20 696e 7374 616e 6365       An instance
+00002320: 206f 6620 7468 6520 4665 6465 7261 7465   of the Federate
+00002330: 644d 6f64 656c 206f 626a 6563 742e 0a20  dModel object.. 
+00002340: 2020 2020 2020 2072 6574 7572 6e5f 636f         return_co
+00002350: 616c 6974 696f 6e73 3a20 626f 6f6c 2c20  alitions: bool, 
+00002360: 6465 6661 756c 7420 746f 2054 7275 650a  default to True.
+00002370: 2020 2020 2020 2020 2020 2020 4966 2073              If s
+00002380: 6574 2074 6f20 5472 7565 2c20 6d65 7468  et to True, meth
+00002390: 6f64 2077 696c 6c20 7265 7475 726e 2076  od will return v
+000023a0: 616c 7565 2d6d 6170 7069 6e67 2066 6f72  alue-mapping for
+000023b0: 2065 7665 7279 2063 6f61 6c69 7469 6f6e   every coalition
+000023c0: 2e0a 2020 2020 2020 2020 5265 7475 726e  ..        Return
+000023d0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+000023e0: 2d0a 2020 2020 2020 2020 4e6f 6e65 0a20  -.        None. 
+000023f0: 2020 2020 2020 2072 3a00 0000 e902 0000         r:.......
+00002400: 0063 0100 0000 0000 0000 0000 0000 0200  .c..............
+00002410: 0000 0300 0000 5300 0000 f312 0000 0067  ......S........g
+00002420: 007c 005d 057d 017c 016a 0091 0271 0253  .|.].}.|.j...q.S
+00002430: 0072 0d00 0000 a901 7241 0000 0072 2600  .r......rA...r&.
+00002440: 0000 720d 0000 0072 0d00 0000 7211 0000  ..r....r....r...
+00002450: 00da 0a3c 6c69 7374 636f 6d70 3ef2 0000  ...<listcomp>...
+00002460: 00f3 0200 0000 1200 7a38 5361 6d70 6c65  ........z8Sample
+00002470: 5f53 6861 706c 6579 5f45 7661 6c75 6174  _Shapley_Evaluat
+00002480: 6f72 2e75 7064 6174 655f 7368 6170 2e3c  or.update_shap.<
+00002490: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
+000024a0: 703e 54a9 01da 0b72 6574 7572 6e5f 6469  p>T....return_di
+000024b0: 6374 e700 0000 0000 0000 00a9 02da 0a63  ct.............c
+000024c0: 6f61 6c69 7469 6f6e 73da 0d73 6561 7263  oalitions..searc
+000024d0: 6865 645f 6e6f 6465 7a04 206f 6620 7a20  hed_nodez. of z 
+000024e0: 3a20 666f 726d 696e 6720 616e 6420 6576  : forming and ev
+000024f0: 616c 7561 7469 6e67 2073 7562 7365 7420  aluating subset 
+00002500: a902 7216 0000 0072 1700 0000 723b 0000  ..r....r....r;..
+00002510: 004e 2915 7214 0000 0072 0300 0000 da0d  .N).r....r......
+00002520: 666f 726d 5f73 7570 6572 7365 74da 0e73  form_superset..s
+00002530: 656c 6563 745f 7375 6273 6574 7372 4000  elect_subsetsr@.
+00002540: 0000 723f 0000 00da 0673 6f72 7465 64da  ..r?.....sorted.
+00002550: 0367 6574 da05 7072 696e 7472 1c00 0000  .get..printr....
+00002560: 7242 0000 0072 4300 0000 7202 0000 0072  rB...rC...r....r
+00002570: 4400 0000 7245 0000 0072 4600 0000 7247  D...rE...rF...rG
+00002580: 0000 00da 0e71 7569 636b 5f65 7661 6c75  .....quick_evalu
+00002590: 6174 65da 046d 6174 68da 0463 6f6d 6272  ate..math..combr
+000025a0: 6200 0000 291f 7232 0000 0072 1600 0000  b...).r2...r....
+000025b0: 7234 0000 0072 3500 0000 7236 0000 0072  r4...r5...r6...r
+000025c0: 3800 0000 7239 0000 00da 116f 7065 7261  8...r9.....opera
+000025d0: 7469 6f6e 5f63 6f75 6e74 6572 da14 6e75  tion_counter..nu
+000025e0: 6d62 6572 5f6f 665f 6f70 6572 6174 696f  mber_of_operatio
+000025f0: 6e73 7248 0000 00da 0873 7570 6572 7365  nsrH.....superse
+00002600: 7472 2700 0000 da04 7368 6170 da01 53da  tr'.....shap..S.
+00002610: 0173 da06 735f 776f 5f69 da05 735f 775f  .s..s_wo_i..s_w_
+00002620: 695a 0c73 5f77 6f5f 695f 7363 6f72 655a  iZ.s_wo_i_scoreZ
+00002630: 1073 5f77 6f5f 695f 6772 6164 6965 6e74  .s_wo_i_gradient
+00002640: 735a 0c73 5f77 6f5f 695f 6f70 7469 6d5a  sZ.s_wo_i_optimZ
+00002650: 0c73 5f77 6f5f 695f 6d6f 6465 6c5a 0f73  .s_wo_i_modelZ.s
+00002660: 5f77 6f5f 695f 6772 6164 5f61 7667 5a0e  _wo_i_grad_avgZ.
+00002670: 735f 776f 5f69 5f77 6569 6768 7473 5a0b  s_wo_i_weightsZ.
+00002680: 735f 775f 695f 7363 6f72 655a 0f73 5f77  s_w_i_scoreZ.s_w
+00002690: 5f69 5f67 7261 6469 656e 7473 5a0b 735f  _i_gradientsZ.s_
+000026a0: 775f 695f 6f70 7469 6d5a 0b73 5f77 5f69  w_i_optimZ.s_w_i
+000026b0: 5f6d 6f64 656c 5a0e 735f 775f 695f 6772  _modelZ.s_w_i_gr
+000026c0: 6164 5f61 7667 5a0d 735f 775f 695f 7765  ad_avgZ.s_w_i_we
+000026d0: 6967 6874 73da 0a73 616d 706c 655f 706f  ights..sample_po
+000026e0: 73da 0764 6976 6973 6f72 720d 0000 0072  s..divisorr....r
+000026f0: 0d00 0000 7211 0000 00da 0b75 7064 6174  ....r......updat
+00002700: 655f 7368 6170 c800 0000 7356 0000 0004  e_shap....sV....
+00002710: 2310 0104 030e 030e 0208 0304 010e 020c  #...............
+00002720: 010c 0112 010a 030a 0118 020c 010a 010a  ................
+00002730: 010a 0112 010a 010c 0108 0108 010a 030a  ................
+00002740: 0118 020c 010a 010a 010a 0112 010a 010c  ................
+00002750: 0108 0108 0118 0208 0212 0116 0108 0208  ................
+00002760: 0102 ff04 d47a 2453 616d 706c 655f 5368  .....z$Sample_Sh
+00002770: 6170 6c65 795f 4576 616c 7561 746f 722e  apley_Evaluator.
+00002780: 7570 6461 7465 5f73 6861 70e9 1e00 0000  update_shap.....
+00002790: da11 6e75 6d62 6572 5f6f 665f 776f 726b  ..number_of_work
+000027a0: 6572 7363 0800 0000 0000 0000 0000 0000  ersc............
+000027b0: 1b00 0000 0800 0000 0300 0000 73ac 0100  ............s...
+000027c0: 0069 007d 0864 0164 0284 007c 0244 0083  .i.}.d.d...|.D..
+000027d0: 017d 0274 006a 017c 0264 0364 048d 027d  .}.t.j.|.d.d...}
+000027e0: 0964 057d 0a64 0674 027c 0283 0113 0064  .d.}.d.t.|.....d
+000027f0: 0718 007d 0b74 027c 0983 017c 066b 0072  ...}.t.|...|.k.r
+00002800: 2474 027c 0983 017d 0674 037c 097c 0664  $t.|...}.t.|.|.d
+00002810: 088d 027d 0c74 047c 0683 018f 3e89 027c  ...}.t.|....>..|
+00002820: 0c44 005d 337d 0d87 0087 0187 0287 0387  .D.]3}..........
+00002830: 0466 0564 0964 0284 087c 0d44 0083 017d  .f.d.d...|.D...}
+00002840: 0e7c 0e44 005d 107d 0f7c 0fa0 05a1 005c  .|.D.].}.|.....\
+00002850: 027d 107d 117c 117c 0874 0674 077c 1083  .}.}.|.|.t.t.|..
+00002860: 0183 013c 0071 427c 0a74 027c 0d83 0137  ...<.qB|.t.|...7
+00002870: 007d 0a74 0864 0a7c 0a9b 0064 0b7c 0b9b  .}.t.d.|...d.|..
+00002880: 0064 0c9d 0583 0101 0071 3157 0064 0d04  .d.......q1W.d..
+00002890: 0004 0083 0301 006e 0831 0073 6f77 0101  .......n.1.sow..
+000028a0: 0001 0001 0059 0001 0074 0864 0e83 0101  .....Y...t.d....
+000028b0: 007c 0244 005d 537d 1264 0f7d 1374 006a  .|.D.]S}.d.}.t.j
+000028c0: 097c 097c 1264 108d 027d 147c 1444 005d  .|.|.d...}.|.D.]
+000028d0: 387d 1574 0674 077c 1583 0183 017d 1674  8}.t.t.|.....}.t
+000028e0: 0aa0 0b7c 15a1 017d 177c 17a0 0c7c 12a1  ...|...}.|...|..
+000028f0: 0101 0074 0674 077c 1783 0183 017d 1874  ...t.t.|.....}.t
+00002900: 0da0 0e74 027c 0283 0164 0718 0074 027c  ...t.|...d...t.|
+00002910: 1683 01a1 027d 1974 0f64 077c 191b 0083  .....}.t.d.|....
+00002920: 017d 1a7c 1374 0f7c 1a7c 087c 1819 007c  .}.|.t.|.|.|...|
+00002930: 087c 1619 0018 0014 0083 0137 007d 1371  .|.........7.}.q
+00002940: 8774 0f7c 1374 027c 0283 011b 0083 0188  .t.|.t.|........
+00002950: 046a 107c 0419 007c 123c 0071 7a7c 0764  .j.|...|.<.qz|.d
+00002960: 116b 0272 d47c 0853 0064 0d53 0029 1261  .k.r.|.S.d.S.).a
+00002970: 4905 0000 4d65 7468 6f64 2075 7365 6420  I...Method used 
+00002980: 746f 2074 7261 636b 5f72 6573 756c 7473  to track_results
+00002990: 2061 6674 6572 2065 6163 6820 7472 6169   after each trai
+000029a0: 6e69 6e67 2072 6f75 6e64 2e0a 2020 2020  ning round..    
+000029b0: 2020 2020 5570 6461 7465 5f73 6861 705f      Update_shap_
+000029c0: 6d75 6c74 6970 2069 7320 6120 6465 6661  multip is a defa
+000029d0: 756c 7420 6d65 7468 6f64 2075 7365 6420  ult method used 
+000029e0: 746f 2063 616c 6375 6c61 7465 0a20 2020  to calculate.   
+000029f0: 2020 2020 2053 6861 706c 6579 2072 6f75       Shapley rou
+00002a00: 6e64 2c20 6173 2069 7420 7573 6573 2061  nd, as it uses a
+00002a10: 206e 756d 6265 7220 6f66 2077 6f72 6b65   number of worke
+00002a20: 7273 2074 6f20 636f 6d70 6c65 7465 2061  rs to complete a
+00002a30: 2074 6173 6b2e 0a20 2020 200a 2020 2020   task..    .    
+00002a40: 2020 2020 4769 7665 6e20 7468 6520 6772      Given the gr
+00002a50: 6169 646e 6574 732c 2069 6473 206f 6620  aidnets, ids of 
+00002a60: 7468 6520 6e6f 6465 7320 696e 636c 7564  the nodes includ
+00002a70: 6564 2069 6e20 7361 6d70 6c65 2c0a 2020  ed in sample,.  
+00002a80: 2020 2020 2020 6c61 7374 2076 6572 7369        last versi
+00002a90: 6f6e 206f 6620 7468 6520 6f70 7469 6d69  on of the optimi
+00002aa0: 7a65 722c 2070 7265 7669 6f75 7320 7665  zer, previous ve
+00002ab0: 7273 696f 6e20 6f66 2074 6865 206d 6f64  rsion of the mod
+00002ac0: 656c 0a20 2020 2020 2020 2061 6e64 2074  el.        and t
+00002ad0: 6865 2075 7064 6174 6564 2076 6572 7369  he updated versi
+00002ae0: 6f6e 206f 6620 7468 6520 6d6f 6465 6c2c  on of the model,
+00002af0: 2069 7420 6361 6c63 756c 6174 6573 2076   it calculates v
+00002b00: 616c 7565 7320 6f66 0a20 2020 2020 2020  alues of.       
+00002b10: 2061 6c6c 2074 6865 206d 6172 6769 6e61   all the margina
+00002b20: 6c20 636f 6e74 7269 6275 7469 6f6e 7320  l contributions 
+00002b30: 7573 696e 6720 5368 6170 6c65 7920 7661  using Shapley va
+00002b40: 6c75 652e 0a20 2020 2020 2020 200a 2020  lue..        .  
+00002b50: 2020 2020 2020 5061 7261 6d65 7465 7273        Parameters
+00002b60: 0a20 2020 2020 2020 202d 2d2d 2d2d 2d2d  .        -------
+00002b70: 2d2d 2d0a 2020 2020 2020 2020 6772 6164  ---.        grad
+00002b80: 6965 6e74 733a 204f 7264 6572 6564 4469  ients: OrderedDi
+00002b90: 6374 0a20 2020 2020 2020 2020 2020 2041  ct.            A
+00002ba0: 6e20 4f72 6465 7265 6444 6963 7420 636f  n OrderedDict co
+00002bb0: 6e74 6169 6e69 6e67 2067 7261 6469 656e  ntaining gradien
+00002bc0: 7473 206f 6620 7468 6520 7361 6d70 6c65  ts of the sample
+00002bd0: 6420 6e6f 6465 732e 0a20 2020 2020 2020  d nodes..       
+00002be0: 206e 6f64 6573 5f69 6e5f 7361 6d70 6c65   nodes_in_sample
+00002bf0: 3a20 6c69 7374 0a20 2020 2020 2020 2020  : list.         
+00002c00: 2020 2041 206c 6973 7420 636f 6e74 6169     A list contai
+00002c10: 6e69 6e67 2069 6427 7320 6f66 2074 6865  ning id's of the
+00002c20: 206e 6f64 6573 2074 6861 7420 7765 7265   nodes that were
+00002c30: 2073 616d 706c 6564 2e0a 2020 2020 2020   sampled..      
+00002c40: 2020 7072 6576 696f 7573 5f6f 7074 696d    previous_optim
+00002c50: 697a 6572 3a20 4f70 7469 6d69 7a65 7273  izer: Optimizers
+00002c60: 0a20 2020 2020 2020 2020 2020 2041 6e20  .            An 
+00002c70: 696e 7374 616e 6365 206f 6620 7468 6520  instance of the 
+00002c80: 6173 6f63 6969 7461 2e4f 7074 696d 697a  asociita.Optimiz
+00002c90: 6572 7320 636c 6173 732e 0a20 2020 2020  ers class..     
+00002ca0: 2020 2069 7465 7261 7469 6f6e 3a20 696e     iteration: in
+00002cb0: 740a 2020 2020 2020 2020 2020 2020 5468  t.            Th
+00002cc0: 6520 6375 7272 656e 7420 6974 6572 6174  e current iterat
+00002cd0: 696f 6e2e 0a20 2020 2020 2020 2070 7265  ion..        pre
+00002ce0: 7669 6f75 735f 6d6f 6465 6c3a 2046 6564  vious_model: Fed
+00002cf0: 6572 6174 6564 4d6f 6465 6c0a 2020 2020  eratedModel.    
+00002d00: 2020 2020 2020 2020 416e 2069 6e73 7461          An insta
+00002d10: 6e63 6520 6f66 2074 6865 2046 6564 6572  nce of the Feder
+00002d20: 6174 6564 4d6f 6465 6c20 6f62 6a65 6374  atedModel object
+00002d30: 2e0a 2020 2020 2020 2020 7570 6461 7465  ..        update
+00002d40: 645f 6d6f 6465 6c3a 2046 6564 6572 6174  d_model: Federat
+00002d50: 6564 4d6f 6465 6c0a 2020 2020 2020 2020  edModel.        
+00002d60: 2020 2020 416e 2069 6e73 7461 6e63 6520      An instance 
+00002d70: 6f66 2074 6865 2046 6564 6572 6174 6564  of the Federated
+00002d80: 4d6f 6465 6c20 6f62 6a65 6374 2e0a 2020  Model object..  
+00002d90: 2020 2020 2020 6e75 6d62 6572 5f6f 665f        number_of_
+00002da0: 776f 726b 6572 733a 2069 6e74 2c20 6465  workers: int, de
+00002db0: 6661 756c 7420 746f 2035 300a 2020 2020  fault to 50.    
+00002dc0: 2020 2020 2020 2020 4120 6e75 6d62 6572          A number
+00002dd0: 206f 6620 776f 726b 6572 7320 7468 6174   of workers that
+00002de0: 2077 696c 6c20 7369 6d75 6c74 616e 656f   will simultaneo
+00002df0: 7573 6c79 2077 6f72 6b20 6f6e 2061 2074  usly work on a t
+00002e00: 6173 6b2e 0a20 2020 2020 2020 2072 6574  ask..        ret
+00002e10: 7572 6e5f 636f 616c 6974 696f 6e73 3a20  urn_coalitions: 
+00002e20: 626f 6f6c 2c20 6465 6661 756c 7420 746f  bool, default to
+00002e30: 2054 7275 650a 2020 2020 2020 2020 2020   True.          
+00002e40: 2020 4966 2073 6574 2074 6f20 5472 7565    If set to True
+00002e50: 2c20 6d65 7468 6f64 2077 696c 6c20 7265  , method will re
+00002e60: 7475 726e 2076 616c 7565 2d6d 6170 7069  turn value-mappi
+00002e70: 6e67 2066 6f72 2065 7665 7279 2063 6f61  ng for every coa
+00002e80: 6c69 7469 6f6e 2e0a 2020 2020 2020 2020  lition..        
+00002e90: 5265 7475 726e 730a 2020 2020 2020 2020  Returns.        
+00002ea0: 2d2d 2d2d 2d2d 2d0a 2020 2020 2020 2020  -------.        
+00002eb0: 4e6f 6e65 0a20 2020 2020 2020 2063 0100  None.        c..
+00002ec0: 0000 0000 0000 0000 0000 0200 0000 0300  ................
+00002ed0: 0000 5300 0000 7264 0000 0072 0d00 0000  ..S...rd...r....
+00002ee0: 7265 0000 0072 2600 0000 720d 0000 0072  re...r&...r....r
+00002ef0: 0d00 0000 7211 0000 0072 6600 0000 4f01  ....r....rf...O.
+00002f00: 0000 7267 0000 007a 3f53 616d 706c 655f  ..rg...z?Sample_
+00002f10: 5368 6170 6c65 795f 4576 616c 7561 746f  Shapley_Evaluato
+00002f20: 722e 7570 6461 7465 5f73 6861 705f 6d75  r.update_shap_mu
+00002f30: 6c74 6970 2e3c 6c6f 6361 6c73 3e2e 3c6c  ltip.<locals>.<l
+00002f40: 6973 7463 6f6d 703e 4672 6800 0000 7201  istcomp>Frh...r.
+00002f50: 0000 0072 6300 0000 723a 0000 0072 1000  ...rc...r:...r..
+00002f60: 0000 6301 0000 0000 0000 0000 0000 0002  ..c.............
+00002f70: 0000 000b 0000 0013 0000 0073 3400 0000  ...........s4...
+00002f80: 6700 7c00 5d16 7d01 8802 a000 8804 6a01  g.|.].}.......j.
+00002f90: 7c01 7402 a003 8800 a101 7402 a003 8801  |.t.......t.....
+00002fa0: a101 7402 a003 8803 a101 6604 a102 9102  ..t.......f.....
+00002fb0: 7102 5300 720d 0000 0029 04da 0b61 7070  q.S.r....)...app
+00002fc0: 6c79 5f61 7379 6e63 da0f 6573 7461 626c  ly_async..establ
+00002fd0: 6973 685f 7661 6c75 6572 4200 0000 7243  ish_valuerB...rC
+00002fe0: 0000 0029 0272 0e00 0000 da09 636f 616c  ...).r......coal
+00002ff0: 6974 696f 6ea9 0572 1600 0000 7235 0000  ition..r....r5..
+00003000: 00da 0470 6f6f 6c72 3800 0000 7232 0000  ...poolr8...r2..
+00003010: 0072 0d00 0000 7211 0000 0072 6600 0000  .r....r....rf...
+00003020: 5901 0000 730e 0000 0006 0002 030a fd08  Y...s...........
+00003030: 0108 0108 010a fd7a 0a43 6f6d 706c 6574  .......z.Complet
+00003040: 6564 207a 0820 6f75 7420 6f66 207a 0b20  ed z. out of z. 
+00003050: 6f70 6572 6174 696f 6e73 4e7a 5f46 696e  operationsNz_Fin
+00003060: 6973 6865 6420 6576 616c 7561 7469 6e67  ished evaluating
+00003070: 2061 6c6c 206f 6620 7468 6520 636f 616c   all of the coal
+00003080: 6974 696f 6e73 2e20 436f 6d6d 656e 6369  itions. Commenci
+00003090: 6e67 2063 616c 6375 6c61 7469 6f6e 206f  ng calculation o
+000030a0: 6620 696e 6469 7669 6475 616c 2053 6861  f individual Sha
+000030b0: 706c 6579 2076 616c 7565 732e 726a 0000  pley values.rj..
+000030c0: 0072 6b00 0000 5429 1172 0300 0000 726f  .rk...T).r....ro
+000030d0: 0000 0072 1400 0000 7215 0000 0072 0400  ...r....r....r..
+000030e0: 0000 7272 0000 0072 3f00 0000 7271 0000  ..rr...r?...rq..
+000030f0: 0072 7300 0000 7270 0000 0072 4200 0000  .rs...rp...rB...
+00003100: 7243 0000 00da 0661 7070 656e 6472 7500  rC.....appendru.
+00003110: 0000 7276 0000 0072 5f00 0000 7262 0000  ..rv...r_...rb..
+00003120: 0029 1b72 3200 0000 7216 0000 0072 3400  .).r2...r....r4.
+00003130: 0000 7235 0000 0072 3600 0000 7238 0000  ..r5...r6...r8..
+00003140: 0072 8300 0000 7239 0000 005a 1163 6f61  .r....r9...Z.coa
+00003150: 6c69 7469 6f6e 5f72 6573 756c 7473 7279  lition_resultsry
+00003160: 0000 0072 7700 0000 7278 0000 00da 0763  ...rw...rx.....c
+00003170: 6875 6e6b 6564 da05 6368 756e 6bda 0772  hunked..chunk..r
+00003180: 6573 756c 7473 da06 7265 7375 6c74 7286  esults..resultr.
+00003190: 0000 00da 0573 636f 7265 7227 0000 0072  .....scorer'...r
+000031a0: 7a00 0000 727b 0000 0072 7c00 0000 727d  z...r{...r|...r}
+000031b0: 0000 005a 0673 5f63 6f70 7972 7e00 0000  ...Z.s_copyr~...
+000031c0: 727f 0000 0072 8000 0000 720d 0000 0072  r....r....r....r
+000031d0: 8700 0000 7211 0000 00da 1275 7064 6174  ....r......updat
+000031e0: 655f 7368 6170 5f6d 756c 7469 7027 0100  e_shap_multip'..
+000031f0: 0073 4800 0000 0427 0e01 0e01 0402 1001  .sH....'........
+00003200: 0c01 0801 0c01 0a01 0801 1201 0203 06fd  ................
+00003210: 0804 0c01 1201 0c01 1801 02f7 1cff 080b  ................
+00003220: 0801 0401 0e01 0801 0c01 0a01 0a01 0c01  ................
+00003230: 1801 0c01 1e01 1c02 0802 0401 04ff 7a2b  ..............z+
+00003240: 5361 6d70 6c65 5f53 6861 706c 6579 5f45  Sample_Shapley_E
+00003250: 7661 6c75 6174 6f72 2e75 7064 6174 655f  valuator.update_
+00003260: 7368 6170 5f6d 756c 7469 7072 8600 0000  shap_multipr....
+00003270: da05 6d6f 6465 6c63 0500 0000 0000 0000  ..modelc........
+00003280: 0000 0000 0800 0000 0400 0000 4300 0000  ............C...
+00003290: 7346 0000 0074 007c 027c 0164 018d 027d  sF...t.|.|.d...}
+000032a0: 0274 01a0 027c 02a1 017d 057c 036a 037c  .t...|...}.|.j.|
+000032b0: 04a0 04a1 007c 0564 028d 027d 067c 04a0  .....|.d...}.|..
+000032c0: 057c 06a1 0101 007c 04a0 06a1 0064 0319  .|.....|.....d..
+000032d0: 007d 077c 017c 0766 0253 0029 0461 9702  .}.|.|.f.S.).a..
+000032e0: 0000 4865 6c70 6572 206d 6574 686f 6420  ..Helper method 
+000032f0: 7573 6564 2074 6f20 6573 7461 626c 6973  used to establis
+00003300: 6820 6120 7661 6c75 6520 6f66 2061 2070  h a value of a p
+00003310: 6172 7469 6375 6c61 7220 636f 616c 6974  articular coalit
+00003320: 696f 6e2e 0a20 2020 2020 2020 2043 616c  ion..        Cal
+00003330: 6c65 6420 6173 796e 6368 726f 6e6f 7573  led asynchronous
+00003340: 6c79 2069 6e20 6d75 6c74 6970 726f 6365  ly in multiproce
+00003350: 7373 6564 2076 6572 7369 6f6e 206f 6620  ssed version of 
+00003360: 7468 6520 7365 6c66 2e75 7064 6174 655f  the self.update_
+00003370: 7368 6170 5f6d 756c 7469 7028 290a 2020  shap_multip().  
+00003380: 2020 2020 2020 6d65 7468 6f64 2e0a 2020        method..  
+00003390: 2020 2020 2020 0a20 2020 2020 2020 2050        .        P
+000033a0: 6172 616d 6574 6572 730a 2020 2020 2020  arameters.      
+000033b0: 2020 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020    ----------.   
+000033c0: 2020 2020 204e 6f6e 650a 2020 2020 2020       None.      
+000033d0: 2020 6772 6164 6965 6e74 733a 204f 7264    gradients: Ord
+000033e0: 6572 6564 4469 6374 0a20 2020 2020 2020  eredDict.       
+000033f0: 2020 2020 2041 6e20 4f72 6465 7265 6444       An OrderedD
+00003400: 6963 7420 636f 6e74 6169 6e69 6e67 2067  ict containing g
+00003410: 7261 6469 656e 7473 206f 6620 7468 6520  radients of the 
+00003420: 7361 6d70 6c65 6420 6e6f 6465 732e 0a20  sampled nodes.. 
+00003430: 2020 2020 2020 2063 6f61 6c69 7469 6f6e         coalition
+00003440: 3a20 6c69 7374 0a20 2020 2020 2020 2020  : list.         
+00003450: 2020 2041 206c 6973 7420 636f 6e74 6169     A list contai
+00003460: 6e69 6e67 2069 6427 7320 6f66 2074 6865  ning id's of the
+00003470: 206e 6f64 6573 2074 6861 7420 7765 7265   nodes that were
+00003480: 2073 616d 706c 6564 2e0a 2020 2020 2020   sampled..      
+00003490: 2020 6f70 7469 6d69 7a65 723a 204f 7074    optimizer: Opt
+000034a0: 696d 697a 6572 730a 2020 2020 2020 2020  imizers.        
+000034b0: 2020 2020 416e 2069 6e73 7461 6e63 6520      An instance 
+000034c0: 6f66 2074 6865 2061 736f 6369 6974 612e  of the asociita.
+000034d0: 4f70 7469 6d69 7a65 7273 2063 6c61 7373  Optimizers class
+000034e0: 2e0a 2020 2020 2020 2020 6d6f 6465 6c3a  ..        model:
+000034f0: 2046 6564 6572 6174 6564 4d6f 6465 6c0a   FederatedModel.
+00003500: 2020 2020 2020 2020 2020 2020 416e 2069              An i
+00003510: 6e73 7461 6e63 6520 6f66 2074 6865 2046  nstance of the F
+00003520: 6564 6572 6174 6564 4d6f 6465 6c20 6f62  ederatedModel ob
+00003530: 6a65 6374 2e0a 2020 2020 2020 2020 5265  ject..        Re
+00003540: 7475 726e 730a 2020 2020 2020 2020 2d2d  turns.        --
+00003550: 2d2d 2d2d 2d0a 2020 2020 2020 2020 7475  -----.        tu
+00003560: 706c 655b 6c69 7374 2c20 666c 6f61 745d  ple[list, float]
+00003570: 0a20 2020 2020 2020 2072 6e00 0000 723b  .        rn...r;
+00003580: 0000 0072 3a00 0000 2907 721c 0000 0072  ...r:...).r....r
+00003590: 0200 0000 7244 0000 0072 4500 0000 7246  ....rD...rE...rF
+000035a0: 0000 0072 4700 0000 7274 0000 0029 0872  ...rG...rt...).r
+000035b0: 3200 0000 7286 0000 0072 1600 0000 7235  2...r....r....r5
+000035c0: 0000 0072 9000 0000 da08 6772 6164 5f61  ...r......grad_a
+000035d0: 7667 723c 0000 0072 8e00 0000 720d 0000  vgr<...r....r...
+000035e0: 0072 0d00 0000 7211 0000 0072 8500 0000  .r....r....r....
+000035f0: 7501 0000 7310 0000 0004 1802 0106 ff0a  u...s...........
+00003600: 0212 010a 010c 0108 017a 2853 616d 706c  .........z(Sampl
+00003610: 655f 5368 6170 6c65 795f 4576 616c 7561  e_Shapley_Evalua
+00003620: 746f 722e 6573 7461 626c 6973 685f 7661  tor.establish_va
+00003630: 6c75 6563 0100 0000 0000 0000 0000 0000  luec............
+00003640: 0400 0000 0800 0000 4300 0000 7250 0000  ........C...rP..
+00003650: 0029 0161 0c01 0000 4d65 7468 6f64 2075  .).a....Method u
+00003660: 7365 6420 746f 2073 756d 2075 7020 616c  sed to sum up al
+00003670: 6c20 7468 6520 7061 7274 6961 6c20 5368  l the partial Sh
+00003680: 6170 6c65 7920 7661 6c75 6573 2074 6f20  apley values to 
+00003690: 6f62 7461 696e 0a20 2020 2020 2020 2061  obtain.        a
+000036a0: 2066 696e 616c 2053 6861 706c 6579 2073   final Shapley s
+000036b0: 636f 7265 2066 6f72 2065 6163 6820 636c  core for each cl
+000036c0: 6965 6e74 2e0a 2020 2020 2020 2020 0a20  ient..        . 
+000036d0: 2020 2020 2020 2050 6172 616d 6574 6572         Parameter
+000036e0: 730a 2020 2020 2020 2020 2d2d 2d2d 2d2d  s.        ------
+000036f0: 2d2d 2d2d 0a20 2020 2020 2020 204e 6f6e  ----.        Non
+00003700: 650a 2020 2020 2020 2020 0a20 2020 2020  e.        .     
+00003710: 2020 2052 6574 7572 6e73 0a20 2020 2020     Returns.     
+00003720: 2020 202d 2d2d 2d2d 2d2d 0a20 2020 2020     -------.     
+00003730: 2020 2074 7570 6c65 5b64 6963 745b 696e     tuple[dict[in
+00003740: 743a 2064 6963 745d 2c20 6469 6374 5b69  t: dict], dict[i
+00003750: 6e74 3a20 666c 6f61 745d 5d0a 2020 2020  nt: float]].    
+00003760: 2020 2020 2906 7262 0000 0072 5100 0000      ).rb...rQ...
+00003770: 7219 0000 0072 6100 0000 7224 0000 0072  r....ra...r$...r
+00003780: 2500 0000 7252 0000 0072 0d00 0000 720d  %...rR...r....r.
+00003790: 0000 0072 1100 0000 da14 6361 6c63 756c  ...r......calcul
+000037a0: 6174 655f 6669 6e61 6c5f 7368 6170 9601  ate_final_shap..
+000037b0: 0000 730a 0000 000e 0c10 011a 0102 ff0c  ..s.............
+000037c0: 027a 2d53 616d 706c 655f 5368 6170 6c65  .z-Sample_Shaple
+000037d0: 795f 4576 616c 7561 746f 722e 6361 6c63  y_Evaluator.calc
+000037e0: 756c 6174 655f 6669 6e61 6c5f 7368 6170  ulate_final_shap
+000037f0: 7256 0000 0029 0272 8200 0000 5429 1172  rV...).r....T).r
+00003800: 5700 0000 7258 0000 0072 5900 0000 725a  W...rX...rY...rZ
+00003810: 0000 0072 5b00 0000 725c 0000 0072 3300  ...r[...r\...r3.
+00003820: 0000 7207 0000 0072 0900 0000 7206 0000  ..r....r....r...
+00003830: 0072 5d00 0000 7281 0000 0072 8f00 0000  .r]...r....r....
+00003840: 723f 0000 0072 5f00 0000 7285 0000 0072  r?...r_...r....r
+00003850: 9200 0000 720d 0000 0072 0d00 0000 720d  ....r....r....r.
+00003860: 0000 0072 1100 0000 7260 0000 00ac 0000  ...r....r`......
+00003870: 0073 6800 0000 0800 0401 0206 0201 02ff  .sh.............
+00003880: 0202 02fe 0202 0afe 021b 04fa 0201 02ff  ................
+00003890: 0202 02fe 0203 02fd 0204 02fc 0205 02fb  ................
+000038a0: 0206 0afa 0265 0201 04f9 0201 02ff 0202  .....e..........
+000038b0: 02fe 0203 02fd 0204 02fc 0205 02fb 0206  ................
+000038c0: 02fa 0207 0af9 024e 0201 02ff 0202 02fe  .......N........
+000038d0: 0203 02fd 0204 02fc 0a04 0afc 0c21 7260  .............!r`
+000038e0: 0000 0029 0146 291a da1b 6173 6f63 6969  ...).F)...asocii
+000038f0: 7461 2e75 7469 6c73 2e63 6f6d 7075 7461  ta.utils.computa
+00003900: 7469 6f6e 7372 0200 0000 7203 0000 00da  tionsr....r.....
+00003910: 056e 756d 7079 7224 0000 0072 4200 0000  .numpyr$...rB...
+00003920: 7275 0000 00da 0f6d 756c 7469 7072 6f63  ru.....multiproc
+00003930: 6573 7369 6e67 7204 0000 0072 0500 0000  essingr....r....
+00003940: da27 6173 6f63 6969 7461 2e6d 6f64 656c  .'asociita.model
+00003950: 732e 7079 746f 7263 682e 6665 6465 7261  s.pytorch.federa
+00003960: 7465 645f 6d6f 6465 6c72 0600 0000 da0b  ted_modelr......
+00003970: 636f 6c6c 6563 7469 6f6e 7372 0700 0000  collectionsr....
+00003980: da10 5f63 6f6c 6c65 6374 696f 6e73 5f61  .._collections_a
+00003990: 6263 7208 0000 00da 1961 736f 6369 6974  bcr......asociit
+000039a0: 612e 7574 696c 732e 6f70 7469 6d69 7a65  a.utils.optimize
+000039b0: 7273 7209 0000 00da 0469 7465 7272 5c00  rsr......iterr\.
+000039c0: 0000 7215 0000 0072 5b00 0000 725d 0000  ..r....r[...r]..
+000039d0: 0072 1c00 0000 721d 0000 0072 6000 0000  .r....r....r`...
+000039e0: 720d 0000 0072 0d00 0000 720d 0000 0072  r....r....r....r
+000039f0: 1100 0000 da08 3c6d 6f64 756c 653e 0100  ......<module>..
+00003a00: 0000 7326 0000 000c 000c 0108 0108 0108  ..s&............
+00003a10: 0110 010c 010c 010c 010c 0116 0302 1608  ................
+00003a20: fe02 0102 ff02 020a fe0e 1c12 6f         ............o
```

### Comparing `asociita-0.3.2/asociita/components/evaluator/evaluation_manager.py` & `asociita-0.3.3/asociita/components/evaluator/evaluation_manager.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from asociita.components.evaluator.or_evaluator import OR_Evaluator
+from asociita.components.evaluator.lsaa_evaluator import LSAA
 from asociita.components.evaluator.sample_evaluator import Sample_Evaluator
 from asociita.components.evaluator.sample_evaluator import Sample_Shapley_Evaluator
 from asociita.models.pytorch.federated_model import FederatedModel
 from asociita.exceptions.evaluatorexception import Sample_Evaluator_Init_Exception
 from asociita.utils.optimizers import Optimizers
 from collections import OrderedDict
 import copy
@@ -91,14 +92,20 @@
             self.flag_sample_evaluator = False
         # Flag: Shapley-InSample Method
         if settings.get("IN_SAMPLE_SHAP"):
             self.flag_samplesh_evaluator = True
             self.compiled_flags.append('in_sample_shap')
         else:
             self.flag_samplesh_evaluator = False
+        # Flag: LSAA
+        if settings.get("LSAA"):
+            self.flag_lsaa_evaluator = True
+            self.compiled_flags.append('LSAA')
+        else:
+            self.flag_lsaa_evaluator = False
         
         # Sets up a flag for each available method of score preservation
         # Flag: Preservation of partial results (for In-Sample Methods)
         if settings['preserve_evaluation'].get("preserve_partial_results"):
             self.preserve_partial_results = True
         else:
             self.preserve_partial_results = False
@@ -119,15 +126,24 @@
                 raise Sample_Evaluator_Init_Exception
         # Initialization: Shapley-InSample Method
         if self.flag_samplesh_evaluator == True:
             try:
                 self.samplesh_evaluator = Sample_Shapley_Evaluator(nodes = nodes, iterations=iterations)
             except NameError as e:
                 raise Sample_Evaluator_Init_Exception
-        
+        if self.flag_lsaa_evaluator == True:
+            try:
+                self.lsaa_evaluator = LSAA(nodes = nodes, iterations = iterations)
+                self.search_length = settings['line_search_length']
+            except NameError as e:
+                raise #TODO: Custom error
+            except KeyError as k:
+                raise #TODO: Lacking configuration error
+
+
         # Sets up the scheduler
         if settings.get("scheduler"):
             self.scheduler = settings['scheduler']
         else:
             self.scheduler = {flag: [iteration for iteration in range(iterations)] for flag in self.compiled_flags}
         
         # Auxiliary
@@ -230,20 +246,35 @@
             self.or_evaluator.track_shapley(gradients=gradients)
         elif self.flag_loo_or: # This is called ONLY when we don't calculate Shapley, but we calculate LOO
             self.or_evaluator.track_loo(gradients=gradients)
         
         # LOO-InSample Method
         if self.flag_sample_evaluator:
             if iteration in self.scheduler['in_sample_loo']: # Checks scheduler
-                self.sample_evaluator.update_psi(gradients = gradients,
+                debug_values = self.sample_evaluator.update_psi(gradients = gradients,
                                             nodes_in_sample = nodes_in_sample,
                                             iteration = iteration,
                                             optimizer = self.previous_optimizer,
                                             final_model = self.updated_c_model,
                                             previous_model= self.previous_c_model)
+                # Preserving debug values (if enabled)
+                if self.full_debug:
+                    if iteration == 0:
+                        with open(os.path.join(self.full_debug_path, 'col_values_debug_loo.csv'), 'a+', newline='') as csv_file:
+                            field_names = ['coalition', 'value', 'iteration']
+                            csv_writer = csv.writer(csv_file)
+                            csv_writer.writerow(field_names)
+                            for col, value in debug_values.items():
+                                csv_writer.writerow([col, value, iteration])
+                    else:
+                        with open(os.path.join(self.full_debug_path, 'col_values_debug_loo.csv'), 'a+', newline='') as csv_file:
+                            csv_writer = csv.writer(csv_file)
+                            for col, value in debug_values.items():
+                                csv_writer.writerow([col, value, iteration])
+
         # Shapley-InSample Method
         if self.flag_samplesh_evaluator:
             if iteration in self.scheduler['in_sample_shap']: # Checks scheduler
                 if self.multip:
                     debug_values = self.samplesh_evaluator.update_shap_multip(gradients = gradients,
                                                                nodes_in_sample = nodes_in_sample,
                                                                iteration = iteration,
@@ -269,14 +300,41 @@
                             for col, value in debug_values.items():
                                 csv_writer.writerow([col, value, iteration])
                     else:
                         with open(os.path.join(self.full_debug_path, 'col_values_debug.csv'), 'a+', newline='') as csv_file:
                             csv_writer = csv.writer(csv_file)
                             for col, value in debug_values.items():
                                 csv_writer.writerow([col, value, iteration])
+    
+        #LSAA Method
+        if self.flag_lsaa_evaluator:
+            if iteration in self.scheduler['LSAA']: # Checks scheduler
+                debug_values = self.lsaa_evaluator.update_lsaa(gradients = gradients,
+                                    nodes_in_sample = nodes_in_sample,
+                                    iteration = iteration,
+                                    search_length = self.search_length,
+                                    optimizer = self.previous_optimizer,
+                                    final_model = self.updated_c_model,
+                                    previous_model = self.previous_c_model)
+            
+                            # Preserving debug values (if enabled)
+                if self.full_debug:
+                    if iteration == 0:
+                        with open(os.path.join(self.full_debug_path, 'col_values_debug_lsaa.csv'), 'a+', newline='') as csv_file:
+                            field_names = ['coalition', 'value', 'iteration']
+                            csv_writer = csv.writer(csv_file)
+                            csv_writer.writerow(field_names)
+                            for col, value in debug_values.items():
+                                csv_writer.writerow([col, value, iteration])
+                    else:
+                        with open(os.path.join(self.full_debug_path, 'col_values_debug_lsaa.csv'), 'a+', newline='') as csv_file:
+                            csv_writer = csv.writer(csv_file)
+                            for col, value in debug_values.items():
+                                csv_writer.writerow([col, value, iteration])
+
 
     def finalize_tracking(self,
                           path: str = None):
         """Method used to finalize the tracking at the end of the training.
         Because the Orchestrator abstraction should be free of any
         unnecessary encumbrance, all the options configuring the behaviour
         of the finalize_tracking method, should be pre-configured at the stage
@@ -305,14 +363,19 @@
             results['full']['psi'] = psi
         
         if self.flag_samplesh_evaluator:
             partial_shap, shap = self.samplesh_evaluator.calculate_final_shap()
             results['partial']['partial_shap'] = partial_shap
             results['full']['shap'] = shap
         
+        if self.lsaa_evaluator:
+            partial_lsaa, lsaa = self.lsaa_evaluator.calculate_final_lsaa()
+            results['partial']['partial_lsaa'] = partial_lsaa
+            results['full']['lsaa'] = lsaa
+        
         if self.preserve_partial_results == True:
             for metric, values in results['partial'].items():
                 s_path = os.path.join(path, (str(metric) + '.csv'))
                 field_names = self.nodes
                 field_names.append('iteration') # Field names == nodes id's (keys)
                 with open(s_path, 'w+', newline='') as csv_file:
                     csv_writer = csv.DictWriter(csv_file, fieldnames=field_names)
```

### Comparing `asociita-0.3.2/asociita/components/evaluator/mr_evaluator.py` & `asociita-0.3.3/asociita/components/evaluator/mr_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/evaluator/or_evaluator.py` & `asociita-0.3.3/asociita/components/evaluator/or_evaluator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/evaluator/sample_evaluator.py` & `asociita-0.3.3/asociita/components/evaluator/sample_evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,16 @@
 
     def update_psi(self,
                    gradients: OrderedDict,
                    nodes_in_sample: list,
                    optimizer: Optimizers,
                    iteration: int,
                    final_model: FederatedModel,
-                   previous_model: FederatedModel):
+                   previous_model: FederatedModel,
+                   return_coalitions: bool = True):
         """Method used to track_results after each training round.
         Given the graidnets, ids of the nodes included in sample,
         last version of the optimizer, previous version of the model
         and the updated version of the model, it calculates values of
         all the marginal contributions using Leave-one-out method.
         
         Parameters
@@ -114,17 +115,21 @@
         updated_model: FederatedModel
             An instance of the FederatedModel object.
         Returns
         -------
         None
         """
 
+        recorded_values = {}
+
         # Evaluating the performance of the final model.
         final_model_score = final_model.evaluate_model()[1]
         
+        recorded_values[tuple(gradients.keys())] = final_model_score
+        
         for node in nodes_in_sample:
             node_id = node.node_id
             
             # Deleting gradients of node i from the sample.
             marginal_gradients = copy.deepcopy(gradients)
             del marginal_gradients[node_id] 
             # Cloning the last optimizer
@@ -134,14 +139,19 @@
             marginal_model = copy.deepcopy(previous_model)
             marginal_grad_avg = Aggregators.compute_average(marginal_gradients) # AGGREGATING FUNCTION -> CHANGE IF NEEDED
             marginal_weights = marginal_optim.fed_optimize(weights=marginal_model.get_weights(),
                                                            delta=marginal_grad_avg)
             marginal_model.update_weights(marginal_weights)
             marginal_model_score = marginal_model.evaluate_model()[1]
             self.partial_psi[iteration][node_id] = final_model_score - marginal_model_score
+            
+            recorded_values[tuple(marginal_gradients.keys())] = marginal_model_score
+            
+        if return_coalitions == True:
+            return recorded_values
 
 
     def calculate_final_psi(self) -> tuple[dict[int: dict], dict[int: float]]:
         """Method used to sum up all the partial LOO scores to obtain
         a final LOO score for each client.
         
         Parameters
```

### Comparing `asociita-0.3.2/asociita/components/nodes/__pycache__/federated_node.cpython-310.pyc` & `asociita-0.3.3/asociita/components/nodes/__pycache__/federated_node.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 13 09:56:12 2023 UTC, .py size: 4366 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 3cca af64 0e11 0000  o.......<..d....
+00000000: 6f0d 0d0a 0000 0000 baf1 b364 0e11 0000  o..........d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 4a00 0000 6400  .....@...sJ...d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c04 6d05 5a05  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c06 6d07 5a07 0100 6507  ..d.d.l.m.Z...e.
 00000060: a008 a100 5a08 4700 6405 6406 8400 6406  ....Z.G.d.d...d.
 00000070: 8302 5a09 6407 5300 2908 e900 0000 0029  ..Z.d.S.)......)
```

### Comparing `asociita-0.3.2/asociita/components/nodes/federated_node.py` & `asociita-0.3.3/asociita/components/nodes/federated_node.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/orchestrator/__pycache__/evaluator_orchestrator.cpython-310.pyc` & `asociita-0.3.3/asociita/components/orchestrator/__pycache__/evaluator_orchestrator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Wed Jul 12 15:33:37 2023 UTC, .py size: 8893 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,395 +1,392 @@
-00000000: 6f0d 0d0a 0000 0000 d1c7 ae64 bd22 0000  o..........d."..
+00000000: 6f0d 0d0a 0000 0000 6990 b564 5622 0000  o.......i..dV"..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
-00000020: 0004 0000 0040 0000 0073 dc00 0000 6400  .....@...s....d.
+00000020: 0004 0000 0040 0000 0073 d400 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 6d04 5a04 6d05 5a05 0100 6400  m.Z.m.Z.m.Z...d.
 00000050: 6403 6c06 6d07 5a07 0100 6400 6404 6c08  d.l.m.Z...d.d.l.
 00000060: 6d09 5a09 0100 6400 6402 6c02 6d03 5a03  m.Z...d.d.l.m.Z.
 00000070: 6d04 5a04 6d05 5a05 0100 6400 6405 6c0a  m.Z.m.Z...d.d.l.
 00000080: 6d0b 5a0b 0100 6400 6406 6c0c 6d0d 5a0d  m.Z...d.d.l.m.Z.
 00000090: 0100 6400 6407 6c0e 6d0f 5a0f 0100 6400  ..d.d.l.m.Z...d.
 000000a0: 6408 6c10 6d11 5a11 0100 6400 6409 6c12  d.l.m.Z...d.d.l.
 000000b0: 6d13 5a13 0100 6400 640a 6c14 5a14 6400  m.Z...d.d.l.Z.d.
 000000c0: 640a 6c15 5a15 6400 640b 6c16 6d17 5a17  d.l.Z.d.d.l.m.Z.
-000000d0: 6d18 5a18 0100 6509 a019 a100 5a19 6400  m.Z...e.....Z.d.
-000000e0: 640c 6c16 6d1a 5a1a 0100 651a 640d 640e  d.l.m.Z...e.d.d.
-000000f0: 640f 8d02 0100 4700 6410 6411 8400 6411  d.....G.d.d...d.
-00000100: 6501 8303 5a1b 640a 5300 2912 e900 0000  e...Z.d.S.).....
-00000110: 0029 01da 0c4f 7263 6865 7374 7261 746f  .)...Orchestrato
-00000120: 7229 03da 0c63 7265 6174 655f 6e6f 6465  r)...create_node
-00000130: 73da 0c73 616d 706c 655f 6e6f 6465 73da  s..sample_nodes.
-00000140: 0b74 7261 696e 5f6e 6f64 6573 2901 da0b  .train_nodes)...
-00000150: 4167 6772 6567 6174 6f72 7329 01da 074c  Aggregators)...L
-00000160: 6f67 6765 7273 2901 da0a 4f70 7469 6d69  oggers)...Optimi
-00000170: 7a65 7273 2901 da12 4576 616c 7561 7469  zers)...Evaluati
-00000180: 6f6e 5f4d 616e 6167 6572 2901 da0f 4172  on_Manager)...Ar
-00000190: 6368 6976 655f 4d61 6e61 6765 7229 01da  chive_Manager)..
-000001a0: 0853 6574 7469 6e67 7329 01da 0748 656c  .Settings)...Hel
-000001b0: 7065 7273 4e29 02da 0450 6f6f 6cda 074d  persN)...Pool..M
-000001c0: 616e 6167 6572 2901 da10 7365 745f 7374  anager)...set_st
-000001d0: 6172 745f 6d65 7468 6f64 5a05 7370 6177  art_methodZ.spaw
-000001e0: 6e54 2901 5a05 666f 7263 6563 0000 0000  nT).Z.forcec....
-000001f0: 0000 0000 0000 0000 0000 0000 0400 0000  ................
-00000200: 0000 0000 734c 0000 0065 005a 0164 005a  ....sL...e.Z.d.Z
-00000210: 0264 015a 0364 0265 0464 0364 0466 0487  .d.Z.d.e.d.d.f..
-00000220: 0066 0164 0564 0684 0c5a 0564 0765 0665  .f.d.d...Z.d.e.e
-00000230: 076a 086a 0965 076a 086a 0966 0219 0064  .j.j.e.j.j.f...d
-00000240: 0364 0466 0464 0864 0984 045a 0a87 0004  .d.f.d.d...Z....
-00000250: 005a 0b53 0029 0ada 1645 7661 6c75 6174  .Z.S.)...Evaluat
-00000260: 6f72 5f4f 7263 6865 7374 7261 746f 7261  or_Orchestratora
-00000270: 1102 0000 4f72 6368 6573 7472 6174 6f72  ....Orchestrator
-00000280: 2069 7320 6120 6365 6e74 7261 6c20 6f62   is a central ob
-00000290: 6a65 6374 206e 6563 6573 7361 7279 2066  ject necessary f
-000002a0: 6f72 2070 6572 666f 726d 696e 6720 7468  or performing th
-000002b0: 6520 7369 6d75 6c61 7469 6f6e 2e0a 2020  e simulation..  
-000002c0: 2020 2020 2020 4974 2063 6f6e 6e65 6374        It connect
-000002d0: 7320 7468 6520 6e6f 6465 732c 206d 6169  s the nodes, mai
-000002e0: 6e74 6169 6e20 7468 6520 6b6e 6f77 6c65  ntain the knowle
-000002f0: 6467 6520 6162 6f75 7420 7468 6569 7220  dge about their 
-00000300: 7374 6174 6520 616e 6420 6d61 6e61 6765  state and manage
-00000310: 7320 7468 650a 2020 2020 2020 2020 6d75  s the.        mu
-00000320: 6c74 6974 6872 6561 6420 706f 6f6c 2e20  ltithread pool. 
-00000330: 4576 616c 7561 746f 7220 6f72 6368 6573  Evaluator orches
-00000340: 7472 6174 6f72 2069 7320 6120 6368 696c  trator is a chil
-00000350: 6420 636c 6173 7320 6f66 2074 6865 2047  d class of the G
-00000360: 656e 6572 6963 204f 7263 6865 7374 7261  eneric Orchestra
-00000370: 746f 722e 0a20 2020 2020 2020 2055 6e6c  tor..        Unl
-00000380: 696b 6520 6974 7320 7061 7265 6e74 2c20  ike its parent, 
-00000390: 4576 616c 7561 746f 7220 7065 7266 6f72  Evaluator perfor
-000003a0: 6d73 2061 2074 7261 696e 696e 6720 7573  ms a training us
-000003b0: 696e 6720 4665 6465 7261 7465 6420 4f70  ing Federated Op
-000003c0: 7469 6d69 7a61 7469 6f6e 0a20 2020 2020  timization.     
-000003d0: 2020 202d 2070 7365 7564 6f2d 6772 6164     - pseudo-grad
-000003e0: 6965 6e74 7320 6672 6f6d 2074 6865 206d  ients from the m
-000003f0: 6f64 656c 7320 616e 6420 6d6f 6d65 6e74  odels and moment
-00000400: 756d 2e20 4164 6469 7469 6f6e 616c 6c79  um. Additionally
-00000410: 2c20 4576 616c 7561 746f 7220 4f72 6368  , Evaluator Orch
-00000420: 6573 7472 6174 6f72 0a20 2020 2020 2020  estrator.       
-00000430: 2069 7320 6162 6c65 2074 6f20 6173 7365   is able to asse
-00000440: 7373 2063 6c69 656e 7473 206d 6172 6769  ss clients margi
-00000450: 6e61 6c20 636f 6e74 7269 6275 7469 6f6e  nal contribution
-00000460: 2077 6974 6820 7468 6520 6865 6c70 206f   with the help o
-00000470: 6620 4576 616c 7561 7469 6f6e 204d 616e  f Evaluation Man
-00000480: 6167 6572 2eda 0873 6574 7469 6e67 73da  ager...settings.
-00000490: 0672 6574 7572 6e4e 6302 0000 0000 0000  .returnNc.......
-000004a0: 0000 0000 0002 0000 0003 0000 0003 0000  ................
-000004b0: 0073 1000 0000 7400 8300 a001 7c01 a101  .s....t.....|...
-000004c0: 0100 6401 5300 2902 610c 0300 004f 7263  ..d.S.).a....Orc
-000004d0: 6865 7374 7261 746f 7220 6973 2069 6e69  hestrator is ini
-000004e0: 7469 616c 697a 6564 2062 7920 7061 7373  tialized by pass
-000004f0: 696e 6720 616e 2069 6e73 7461 6e63 650a  ing an instance.
-00000500: 2020 2020 2020 2020 6f66 2074 6865 2053          of the S
-00000510: 6574 7469 6e67 7320 6f62 6a65 6374 2e20  ettings object. 
-00000520: 5365 7474 696e 6773 206f 626a 6563 7420  Settings object 
-00000530: 636f 6e74 6169 6e73 2061 6c6c 2074 6865  contains all the
-00000540: 2072 656c 6576 616e 7420 636f 6e66 6967   relevant config
-00000550: 7572 6174 696f 6e61 6c0a 2020 2020 2020  urational.      
-00000560: 2020 7365 7474 696e 6773 2074 6861 7420    settings that 
-00000570: 616e 2069 6e73 7461 6e63 6520 6f66 2074  an instance of t
-00000580: 6865 204f 7263 6865 7374 7261 746f 7220  he Orchestrator 
-00000590: 6f62 6a65 6374 206d 6179 206e 6565 6420  object may need 
-000005a0: 746f 2063 6f6d 706c 6574 6520 7468 6520  to complete the 
-000005b0: 7369 6d75 6c61 7469 6f6e 2e0a 2020 2020  simulation..    
-000005c0: 2020 2020 4576 616c 7561 746f 7220 4f72      Evaluator Or
-000005d0: 6368 6573 7472 6174 6f72 2061 6464 6974  chestrator addit
-000005e0: 696f 6e61 6c79 2072 6571 7569 7265 7320  ionaly requires 
-000005f0: 6120 636f 6e66 6967 7572 6174 696f 6e73  a configurations
-00000600: 2070 6173 7365 6420 746f 2074 6865 204f   passed to the O
-00000610: 7074 696d 697a 6572 200a 2020 2020 2020  ptimizer .      
-00000620: 2020 616e 6420 4576 616c 7561 746f 7220    and Evaluator 
-00000630: 4d61 6e61 6765 7220 7570 6f6e 2069 7473  Manager upon its
-00000640: 2069 6e69 7469 616c 697a 6174 696f 6e2e   initialization.
-00000650: 0a20 2020 2020 2020 200a 2020 2020 2020  .        .      
-00000660: 2020 5061 7261 6d65 7465 7273 0a20 2020    Parameters.   
-00000670: 2020 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a       ----------.
-00000680: 2020 2020 2020 2020 7365 7474 696e 6773          settings
-00000690: 3a20 5365 7474 696e 6773 200a 2020 2020  : Settings .    
-000006a0: 2020 2020 2020 2020 416e 2069 6e73 7461          An insta
-000006b0: 6e63 6520 6f66 2074 6865 2053 6574 7469  nce of the Setti
-000006c0: 6e67 7320 6f62 6a65 6374 2063 6f74 6169  ngs object cotai
-000006d0: 6e69 6e67 2061 6c6c 2074 6865 2073 6574  ning all the set
-000006e0: 7469 6e67 7320 6f66 2074 6865 206f 7263  tings of the orc
-000006f0: 6865 7374 7261 746f 722e 0a20 2020 2020  hestrator..     
-00000700: 2020 2020 2020 2054 6865 2045 7661 6c75         The Evalu
-00000710: 6174 6f72 204f 7263 6865 7374 7261 746f  ator Orchestrato
-00000720: 7220 6164 6469 7469 6f6e 616c 7920 7265  r additionaly re
-00000730: 7175 6972 6573 2074 6865 2070 6173 7365  quires the passe
-00000740: 6420 6f62 6a65 6374 2074 6f20 636f 6e74  d object to cont
-00000750: 6169 6e20 6120 0a20 2020 2020 2020 2020  ain a .         
-00000760: 2020 2063 6f6e 6669 6775 7261 7469 6f6e     configuration
-00000770: 2066 6f72 2074 6865 204f 7074 696d 697a   for the Optimiz
-00000780: 6572 2061 6e64 2074 6865 2045 7661 6c75  er and the Evalu
-00000790: 6174 696f 6e20 4d61 6e61 6765 722e 0a20  ation Manager.. 
-000007a0: 2020 2020 2020 0a20 2020 2020 2020 5265        .       Re
-000007b0: 7475 726e 730a 2020 2020 2020 202d 2d2d  turns.       ---
-000007c0: 2d2d 2d2d 0a20 2020 2020 2020 4e6f 6e65  ----.       None
-000007d0: 0a20 2020 2020 2020 204e 2902 da05 7375  .        N)...su
-000007e0: 7065 72da 085f 5f69 6e69 745f 5f29 02da  per..__init__)..
-000007f0: 0473 656c 6672 1100 0000 a901 da09 5f5f  .selfr........__
-00000800: 636c 6173 735f 5fa9 00fa 862f 686f 6d65  class__..../home
-00000810: 2f6d 7a75 7a69 616b 2f73 6e61 702f 736e  /mzuziak/snap/sn
-00000820: 6170 642d 6465 736b 746f 702d 696e 7465  apd-desktop-inte
-00000830: 6772 6174 696f 6e2f 3833 2f44 6f63 756d  gration/83/Docum
-00000840: 656e 7473 2f41 736f 6369 6974 612f 6173  ents/Asociita/as
-00000850: 6f63 6969 7461 2f61 736f 6369 6974 612f  ociita/asociita/
-00000860: 636f 6d70 6f6e 656e 7473 2f6f 7263 6865  components/orche
-00000870: 7374 7261 746f 722f 6576 616c 7561 746f  strator/evaluato
-00000880: 725f 6f72 6368 6573 7472 6174 6f72 2e70  r_orchestrator.p
-00000890: 7972 1400 0000 1e00 0000 7302 0000 0010  yr........s.....
-000008a0: 127a 1f45 7661 6c75 6174 6f72 5f4f 7263  .z.Evaluator_Orc
-000008b0: 6865 7374 7261 746f 722e 5f5f 696e 6974  hestrator.__init
-000008c0: 5f5f da0a 6e6f 6465 735f 6461 7461 6302  __..nodes_datac.
-000008d0: 0000 0000 0000 0000 0000 0019 0000 000a  ................
-000008e0: 0000 0003 0000 0073 8202 0000 7c00 6a00  .......s....|.j.
-000008f0: 6a01 7d02 7c00 6a00 6a02 7d03 7c00 6a00  j.}.|.j.j.}.|.j.
-00000900: 6a03 7d04 6401 6402 8400 7404 7c03 8301  j.}.d.d...t.|...
-00000910: 4400 8301 7d05 7c00 6a00 6a05 7d06 7c00  D...}.|.j.j.}.|.
-00000920: 6a00 6a06 6403 6b02 7227 7407 7c00 6a00  j.j.d.k.r't.|.j.
-00000930: 6a08 7409 6404 8d02 7d07 7c00 6a00 6a0a  j.t.d...}.|.j.j.
-00000940: 7d08 740b 7c00 6a0c a00d a100 7c08 6405  }.t.|.j.....|.d.
-00000950: 8d02 7d09 740e 7c00 6a00 6a0f 7c00 6a0c  ..}.t.|.j.j.|.j.
-00000960: 7c05 7c02 6406 8d04 7d0a 7410 7c05 7c00  |.|.d...}.t.|.|.
-00000970: 6a00 6a11 8302 7d0b 7c00 6a12 7c03 7c00  j.j...}.|.j.|.|.
-00000980: 6a13 6407 8d02 7d0c 7c00 6a14 7c0b 7c0c  j.d...}.|.j.|.|.
-00000990: 7c01 6408 8d03 7d0b 7404 7c02 8301 4400  |.d...}.t.|...D.
-000009a0: 5dd8 7d0d 7409 a015 6409 7c0d 9b00 9d02  ].}.t...d.|.....
-000009b0: a101 0100 6900 7d0e 7c0a 6a16 7c00 6a0c  ....i.}.|.j.|.j.
-000009c0: 640a 8d01 0100 7c0a 6a17 7c09 640b 8d01  d.....|.j.|.d...
-000009d0: 0100 7418 7c0b 7c06 7409 640c 8d03 7d0f  ..t.|.|.t.d...}.
-000009e0: 7c00 6a19 72b8 741a 6a1b 7c0f 7c00 6a1c  |.j.r.t.j.|.|.j.
-000009f0: 640d 8d02 4400 5d31 7d10 741d 7c06 8301  d...D.]1}.t.|...
-00000a00: 8f23 8900 8700 6601 640e 6402 8408 7c10  .#....f.d.d...|.
-00000a10: 4400 8301 7d11 7c11 4400 5d0f 7d12 7c12  D...}.|.D.].}.|.
-00000a20: a01e a100 5c02 7d13 7d14 741f a020 7c14  ....\.}.}.t.. |.
-00000a30: a101 7c0e 7c13 3c00 7197 5700 640f 0400  ..|.|.<.q.W.d...
-00000a40: 0400 8303 0100 6e08 3100 73b1 7701 0100  ......n.1.s.w...
-00000a50: 0100 0100 5900 0100 7185 6e2f 741d 7c06  ....Y...q.n/t.|.
-00000a60: 8301 8f23 8900 8700 6601 6410 6402 8408  ...#....f.d.d...
-00000a70: 7c0f 4400 8301 7d11 7c11 4400 5d0f 7d12  |.D...}.|.D.].}.
-00000a80: 7c12 a01e a100 5c02 7d13 7d15 741f a020  |.....\.}.}.t.. 
-00000a90: 7c15 a101 7c0e 7c13 3c00 71c8 5700 640f  |...|.|.<.q.W.d.
-00000aa0: 0400 0400 8303 0100 6e08 3100 73e2 7701  ........n.1.s.w.
-00000ab0: 0100 0100 0100 5900 0100 7421 a022 7c0e  ......Y...t!."|.
-00000ac0: a101 7d16 7c09 6a23 7c00 6a0c a00d a100  ..}.|.j#|.j.....
-00000ad0: 7c16 6411 8d02 7d17 7c0a 6a24 7c00 6a0c  |.d...}.|.j$|.j.
-00000ae0: 6412 8d01 0100 7c0a 6a25 7c0e 7c0f 7c0d  d.....|.j%|.|.|.
-00000af0: 6413 8d03 0100 7c00 6a0c a026 7c17 a101  d.....|.j..&|...
-00000b00: 0100 7c0b 4400 5d09 7d18 7c18 6a27 a026  ..|.D.].}.|.j'.&
-00000b10: 7c17 a101 0100 9001 710d 7c00 6a00 6a06  |.......q.|.j.j.
-00000b20: 6403 6b02 9001 7227 7c07 6a28 7c0d 7c00  d.k...r'|.j(|.|.
-00000b30: 6a0c 7c0b 6414 8d03 0100 7c00 6a29 6403  j.|.d.....|.j)d.
-00000b40: 6b02 9001 7232 742a 7c0d 6415 8d01 0100  k...r2t*|.d.....
-00000b50: 715a 7c0a 6a2b 7c07 6a2c 6416 8d01 7d11  qZ|.j+|.j,d...}.
-00000b60: 7409 a02d 6417 a101 0100 6418 5300 2919  t..-d.....d.S.).
-00000b70: 61b6 0300 0022 5065 7266 6f72 6d73 2061  a...."Performs a
-00000b80: 2066 756c 6c20 6665 6465 7261 7465 6420   full federated 
-00000b90: 7472 6169 6e69 6e67 2061 6363 6f72 6469  training accordi
-00000ba0: 6e67 2074 6f20 7468 6520 696e 6974 6961  ng to the initia
-00000bb0: 6c69 7a65 640a 2020 2020 2020 2020 7365  lized.        se
-00000bc0: 7474 696e 6773 2e20 5468 6520 7472 6169  ttings. The trai
-00000bd0: 6e5f 7072 6f74 6f63 6f6c 206f 6620 7468  n_protocol of th
-00000be0: 6520 6f72 6368 6573 7472 6174 6f72 2e65  e orchestrator.e
-00000bf0: 7661 6c75 6174 6f72 5f6f 7263 6865 7374  valuator_orchest
-00000c00: 7261 746f 720a 2020 2020 2020 2020 666f  rator.        fo
-00000c10: 6c6c 6f77 7320 6120 706f 7075 6c61 7220  llows a popular 
-00000c20: 4665 6441 7667 2067 656e 6572 616c 6973  FedAvg generalis
-00000c30: 6174 696f 6e2c 2046 6564 4f70 742e 2049  ation, FedOpt. I
-00000c40: 6e73 7465 6164 206f 6620 7765 6967 6874  nstead of weight
-00000c50: 7320 6672 6f6d 2065 6163 680a 2020 2020  s from each.    
-00000c60: 2020 2020 636c 6965 6e74 732c 2069 7420      clients, it 
-00000c70: 6167 6772 6567 6174 6573 2067 7261 6469  aggregates gradi
-00000c80: 656e 7473 2028 756e 6465 7273 746f 6f64  ents (understood
-00000c90: 2061 7320 6120 6469 6666 6572 656e 6365   as a difference
-00000ca0: 2062 6574 7765 656e 2074 6865 2077 6569   between the wei
-00000cb0: 6768 7473 0a20 2020 2020 2020 206f 6620  ghts.        of 
-00000cc0: 6120 6d6f 6465 6c20 6166 7465 7220 616c  a model after al
-00000cd0: 6c20 7420 6570 6f63 6873 206f 6620 7468  l t epochs of th
-00000ce0: 6520 6c6f 6361 6c20 7472 6169 6e69 6e67  e local training
-00000cf0: 2920 616e 6420 6167 6772 6567 6174 6573  ) and aggregates
-00000d00: 2061 6363 6f72 6469 6e67 2074 6f20 0a20   according to . 
-00000d10: 2020 2020 2020 2070 726f 7669 6465 6420         provided 
-00000d20: 7275 6c65 2e20 5468 6520 6576 616c 7561  rule. The evalua
-00000d30: 7469 6f6e 2070 726f 6365 7373 2069 7320  tion process is 
-00000d40: 6d65 6e61 6765 6420 6279 2074 6865 2069  menaged by the i
-00000d50: 6e73 7461 6e63 6520 6f66 2074 6865 2045  nstance of the E
-00000d60: 7661 6c75 6174 696f 6e0a 2020 2020 2020  valuation.      
-00000d70: 2020 4d61 6e61 6765 7220 6f62 6a65 6374    Manager object
-00000d80: 2c20 7768 6963 6820 6973 2063 616c 6c65  , which is calle
-00000d90: 6420 7570 6f6e 2065 6163 6820 6974 6572  d upon each iter
-00000da0: 6174 696f 6e2e 0a0a 2020 2020 2020 2020  ation...        
-00000db0: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
-00000dc0: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
-00000dd0: 2020 2020 2020 6e6f 6465 735f 6461 7461        nodes_data
-00000de0: 3a20 6c69 7374 5b64 6174 6173 6574 732e  : list[datasets.
-00000df0: 6172 726f 775f 6461 7461 7365 742e 4461  arrow_dataset.Da
-00000e00: 7461 7365 742c 2064 6174 6173 6574 732e  taset, datasets.
-00000e10: 6172 726f 775f 6461 7461 7365 742e 4461  arrow_dataset.Da
-00000e20: 7461 7365 745d 3a20 0a20 2020 2020 2020  taset]: .       
-00000e30: 2020 2020 2041 206c 6973 7420 636f 6e74       A list cont
-00000e40: 6169 6e69 6e67 2074 7261 696e 2073 6574  aining train set
-00000e50: 2061 6e64 2074 6573 7420 7365 7420 7772   and test set wr
-00000e60: 6170 7065 6420 0a20 2020 2020 2020 2020  apped .         
-00000e70: 2020 2069 6e20 6120 6875 6767 696e 6720     in a hugging 
-00000e80: 6661 6365 2061 7272 6f77 5f64 6174 6173  face arrow_datas
-00000e90: 6574 2e44 6174 6173 6574 2063 6f6e 7461  et.Dataset conta
-00000ea0: 696e 6572 730a 2020 2020 2020 2020 0a20  iners.        . 
-00000eb0: 2020 2020 2020 2052 6574 7572 6e73 0a20         Returns. 
-00000ec0: 2020 2020 2020 202d 2d2d 2d2d 2d2d 0a20         -------. 
-00000ed0: 2020 2020 2020 2069 6e74 0a20 2020 2020         int.     
-00000ee0: 2020 2020 2020 2052 6574 7572 6e73 2030         Returns 0
-00000ef0: 206f 6e20 7468 6520 7375 6363 6573 7366   on the successf
-00000f00: 756c 2063 6f6d 706c 6574 696f 6e20 6f66  ul completion of
-00000f10: 2074 6865 2074 7261 696e 696e 672e 0a20   the training.. 
-00000f20: 2020 2020 2020 2020 2020 2063 0100 0000             c....
-00000f30: 0000 0000 0000 0000 0200 0000 0300 0000  ................
-00000f40: 5300 0000 7310 0000 0067 007c 005d 047d  S...s....g.|.].}
-00000f50: 017c 0191 0271 0253 0072 1800 0000 7218  .|...q.S.r....r.
-00000f60: 0000 00a9 02da 022e 30da 046e 6f64 6572  ........0..noder
-00000f70: 1800 0000 7218 0000 0072 1900 0000 da0a  ....r....r......
-00000f80: 3c6c 6973 7463 6f6d 703e 4e00 0000 7302  <listcomp>N...s.
-00000f90: 0000 0010 007a 3945 7661 6c75 6174 6f72  .....z9Evaluator
-00000fa0: 5f4f 7263 6865 7374 7261 746f 722e 7472  _Orchestrator.tr
-00000fb0: 6169 6e5f 7072 6f74 6f63 6f6c 2e3c 6c6f  ain_protocol.<lo
-00000fc0: 6361 6c73 3e2e 3c6c 6973 7463 6f6d 703e  cals>.<listcomp>
-00000fd0: 5429 02da 0f61 7263 6869 7665 5f6d 616e  T)...archive_man
-00000fe0: 6167 6572 5a06 6c6f 6767 6572 2902 da07  agerZ.logger)...
-00000ff0: 7765 6967 6874 7372 1100 0000 2904 7211  weightsr....).r.
-00001000: 0000 00da 056d 6f64 656c da05 6e6f 6465  .....model..node
-00001010: 73da 0a69 7465 7261 7469 6f6e 7329 02da  s..iterations)..
-00001020: 0c6e 6f64 6573 5f6e 756d 6265 7272 2100  .nodes_numberr!.
-00001030: 0000 2903 5a0a 6e6f 6465 735f 6c69 7374  ..).Z.nodes_list
-00001040: da0a 6d6f 6465 6c5f 6c69 7374 5a09 6461  ..model_listZ.da
-00001050: 7461 5f6c 6973 747a 0a49 7465 7261 7469  ta_listz.Iterati
-00001060: 6f6e 2029 015a 0e70 7265 7669 6f75 735f  on ).Z.previous_
-00001070: 6d6f 6465 6c29 015a 1270 7265 7669 6f75  model).Z.previou
-00001080: 735f 6f70 7469 6d69 7a65 7229 02da 0b73  s_optimizer)...s
-00001090: 616d 706c 655f 7369 7a65 da13 6f72 6368  ample_size..orch
-000010a0: 6573 7472 6174 6f72 5f6c 6f67 6765 7229  estrator_logger)
-000010b0: 01da 0473 697a 6563 0100 0000 0000 0000  ...sizec........
-000010c0: 0000 0000 0200 0000 0700 0000 1300 0000  ................
-000010d0: f31c 0000 0067 007c 005d 0a7d 0188 00a0  .....g.|.].}....
-000010e0: 0074 017c 0164 0066 02a1 0291 0271 0253  .t.|.d.f.....q.S
-000010f0: 00a9 01da 0967 7261 6469 656e 7473 a902  .....gradients..
-00001100: 5a0b 6170 706c 795f 6173 796e 6372 0500  Z.apply_asyncr..
-00001110: 0000 721b 0000 00a9 015a 0470 6f6f 6c72  ..r......Z.poolr
-00001120: 1800 0000 7219 0000 0072 1e00 0000 7a00  ....r....r....z.
-00001130: 0000 f302 0000 001c 004e 6301 0000 0000  .........Nc.....
-00001140: 0000 0000 0000 0002 0000 0007 0000 0013  ................
-00001150: 0000 0072 2900 0000 722a 0000 0072 2c00  ...r)...r*...r,.
-00001160: 0000 721b 0000 0072 2d00 0000 7218 0000  ..r....r-...r...
-00001170: 0072 1900 0000 721e 0000 0081 0000 0072  .r....r........r
-00001180: 2e00 0000 2902 7220 0000 005a 0564 656c  ....).r ...Z.del
-00001190: 7461 2901 5a0d 7570 6461 7465 645f 6d6f  ta).Z.updated_mo
-000011a0: 6465 6c29 0372 2b00 0000 5a0f 6e6f 6465  del).r+...Z.node
-000011b0: 735f 696e 5f73 616d 706c 65da 0969 7465  s_in_sample..ite
-000011c0: 7261 7469 6f6e 2903 722f 0000 00da 0d63  ration).r/.....c
-000011d0: 656e 7472 616c 5f6d 6f64 656c 7222 0000  entral_modelr"..
-000011e0: 0029 0172 2f00 0000 2901 da04 7061 7468  .).r/...)...path
-000011f0: 7a11 5472 6169 6e69 6e67 2063 6f6d 706c  z.Training compl
-00001200: 6574 6572 0100 0000 292e 7211 0000 0072  eter....).r....r
-00001210: 2300 0000 da0f 6e75 6d62 6572 5f6f 665f  #.....number_of_
-00001220: 6e6f 6465 73da 106c 6f63 616c 5f77 6172  nodes..local_war
-00001230: 6d5f 7374 6172 74da 0572 616e 6765 7226  m_start..ranger&
-00001240: 0000 00da 0f65 6e61 626c 655f 6172 6368  .....enable_arch
-00001250: 6976 6572 720a 0000 005a 1161 7263 6869  iverr....Z.archi
-00001260: 7665 725f 7365 7474 696e 6773 7227 0000  ver_settingsr'..
-00001270: 00da 126f 7074 696d 697a 6572 5f73 6574  ...optimizer_set
-00001280: 7469 6e67 7372 0800 0000 7230 0000 005a  tingsr....r0...Z
-00001290: 0b67 6574 5f77 6569 6768 7473 7209 0000  .get_weightsr...
-000012a0: 005a 1265 7661 6c75 6174 6f72 5f73 6574  .Z.evaluator_set
-000012b0: 7469 6e67 7372 0300 0000 5a0e 6e6f 6465  tingsr....Z.node
-000012c0: 735f 7365 7474 696e 6773 5a14 6d6f 6465  s_settingsZ.mode
-000012d0: 6c5f 696e 6974 6961 6c69 7a61 7469 6f6e  l_initialization
-000012e0: 5a0b 6365 6e74 7261 6c5f 6e65 745a 146e  Z.central_netZ.n
-000012f0: 6f64 6573 5f69 6e69 7469 616c 697a 6174  odes_initializat
-00001300: 696f 6eda 0469 6e66 6f5a 1770 7265 7365  ion..infoZ.prese
-00001310: 7276 655f 7072 6576 696f 7573 5f6d 6f64  rve_previous_mod
-00001320: 656c 5a1b 7072 6573 6572 7665 5f70 7265  elZ.preserve_pre
-00001330: 7669 6f75 735f 6f70 7469 6d69 7a65 7272  vious_optimizerr
-00001340: 0400 0000 5a09 6261 7463 685f 6a6f 6272  ....Z.batch_jobr
-00001350: 0c00 0000 5a07 6368 756e 6b65 72da 0562  ....Z.chunker..b
-00001360: 6174 6368 720d 0000 00da 0367 6574 da04  atchr......get..
-00001370: 636f 7079 5a08 6465 6570 636f 7079 7206  copyZ.deepcopyr.
-00001380: 0000 005a 0f63 6f6d 7075 7465 5f61 7665  ...Z.compute_ave
-00001390: 7261 6765 5a0c 6665 645f 6f70 7469 6d69  rageZ.fed_optimi
-000013a0: 7a65 5a16 7072 6573 6572 7665 5f75 7064  zeZ.preserve_upd
-000013b0: 6174 6564 5f6d 6f64 656c 5a0d 7472 6163  ated_modelZ.trac
-000013c0: 6b5f 7265 7375 6c74 735a 0e75 7064 6174  k_resultsZ.updat
-000013d0: 655f 7765 6967 6874 7372 2100 0000 5a18  e_weightsr!...Z.
-000013e0: 6172 6368 6976 655f 7472 6169 6e69 6e67  archive_training
-000013f0: 5f72 6573 756c 7473 da0a 6675 6c6c 5f64  _results..full_d
-00001400: 6562 7567 5a0e 6c6f 675f 6770 755f 6d65  ebugZ.log_gpu_me
-00001410: 6d6f 7279 5a11 6669 6e61 6c69 7a65 5f74  moryZ.finalize_t
-00001420: 7261 636b 696e 675a 106d 6574 7269 6373  rackingZ.metrics
-00001430: 5f73 6176 6570 6174 685a 0863 7269 7469  _savepathZ.criti
-00001440: 6361 6c29 1972 1500 0000 721a 0000 0072  cal).r....r....r
-00001450: 2300 0000 7224 0000 0072 3300 0000 7222  #...r$...r3...r"
-00001460: 0000 0072 2600 0000 721f 0000 0072 3600  ...r&...r....r6.
-00001470: 0000 5a05 4f70 7469 6d5a 1265 7661 6c75  ..Z.OptimZ.evalu
-00001480: 6174 696f 6e5f 6d61 6e61 6765 725a 0b6e  ation_managerZ.n
-00001490: 6f64 6573 5f67 7265 656e 7225 0000 0072  odes_greenr%...r
-000014a0: 2f00 0000 722b 0000 005a 0d73 616d 706c  /...r+...Z.sampl
-000014b0: 6564 5f6e 6f64 6573 7238 0000 005a 0772  ed_nodesr8...Z.r
-000014c0: 6573 756c 7473 da06 7265 7375 6c74 5a07  esults..resultZ.
-000014d0: 6e6f 6465 5f69 645a 0d6d 6f64 656c 5f77  node_idZ.model_w
-000014e0: 6569 6768 7473 5a0f 6d6f 6465 6c5f 6772  eightsZ.model_gr
-000014f0: 6164 6965 6e74 735a 0867 7261 645f 6176  adientsZ.grad_av
-00001500: 675a 0f75 7064 6174 6564 5f77 6569 6768  gZ.updated_weigh
-00001510: 7473 721d 0000 0072 1800 0000 722d 0000  tsr....r....r-..
-00001520: 0072 1900 0000 da0e 7472 6169 6e5f 7072  .r......train_pr
-00001530: 6f74 6f63 6f6c 3300 0000 739e 0000 0008  otocol3...s.....
-00001540: 1808 0108 0112 0108 010c 0302 0106 0102  ................
-00001550: 0106 fe08 050a 0102 0106 ff08 0404 0102  ................
-00001560: 0102 0106 fd04 0606 0104 ff06 0304 0106  ................
-00001570: ff06 0302 0102 0106 fe0c 0410 0104 010e  ................
-00001580: 020c 0104 0202 0102 0106 fe06 0314 010a  ................
-00001590: 0112 0108 020c 0110 0102 fe1c fd02 8002  ................
-000015a0: ff0a 0812 0108 020c 0110 0102 fe1c fd0a  ................
-000015b0: 080c 0202 0106 ff0e 0306 0302 0102 0106  ................
-000015c0: fe0c 0508 0210 010e 0306 0104 0102 0106  ................
-000015d0: fe0c 040a 0102 800e 030a 0104 017a 2545  .............z%E
-000015e0: 7661 6c75 6174 6f72 5f4f 7263 6865 7374  valuator_Orchest
-000015f0: 7261 746f 722e 7472 6169 6e5f 7072 6f74  rator.train_prot
-00001600: 6f63 6f6c 290c da08 5f5f 6e61 6d65 5f5f  ocol)...__name__
-00001610: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
-00001620: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
-00001630: 635f 5f72 0b00 0000 7214 0000 00da 046c  c__r....r......l
-00001640: 6973 74da 0864 6174 6173 6574 735a 0d61  ist..datasetsZ.a
-00001650: 7272 6f77 5f64 6174 6173 6574 5a07 4461  rrow_datasetZ.Da
-00001660: 7461 7365 7472 3d00 0000 da0d 5f5f 636c  tasetr=.....__cl
-00001670: 6173 7363 656c 6c5f 5f72 1800 0000 7218  asscell__r....r.
-00001680: 0000 0072 1600 0000 7219 0000 0072 1000  ...r....r....r..
-00001690: 0000 1500 0000 7314 0000 0008 0004 0116  ......s.........
-000016a0: 0802 1508 0106 0104 ff02 ff02 0212 fe72  ...............r
-000016b0: 1000 0000 291c 5a35 6173 6f63 6969 7461  ....).Z5asociita
-000016c0: 2e63 6f6d 706f 6e65 6e74 732e 6f72 6368  .components.orch
-000016d0: 6573 7472 6174 6f72 2e67 656e 6572 6963  estrator.generic
-000016e0: 5f6f 7263 6865 7374 7261 746f 7272 0200  _orchestratorr..
-000016f0: 0000 5a1d 6173 6f63 6969 7461 2e75 7469  ..Z.asociita.uti
-00001700: 6c73 2e6f 7263 6865 7374 7261 7469 6f6e  ls.orchestration
-00001710: 7372 0300 0000 7204 0000 0072 0500 0000  sr....r....r....
-00001720: 5a1b 6173 6f63 6969 7461 2e75 7469 6c73  Z.asociita.utils
-00001730: 2e63 6f6d 7075 7461 7469 6f6e 7372 0600  .computationsr..
-00001740: 0000 5a16 6173 6f63 6969 7461 2e75 7469  ..Z.asociita.uti
-00001750: 6c73 2e6c 6f67 6765 7273 7207 0000 005a  ls.loggersr....Z
-00001760: 1961 736f 6369 6974 612e 7574 696c 732e  .asociita.utils.
-00001770: 6f70 7469 6d69 7a65 7273 7208 0000 005a  optimizersr....Z
-00001780: 3061 736f 6369 6974 612e 636f 6d70 6f6e  0asociita.compon
-00001790: 656e 7473 2e65 7661 6c75 6174 6f72 2e65  ents.evaluator.e
-000017a0: 7661 6c75 6174 696f 6e5f 6d61 6e61 6765  valuation_manage
-000017b0: 7272 0900 0000 5a2c 6173 6f63 6969 7461  rr....Z,asociita
-000017c0: 2e63 6f6d 706f 6e65 6e74 732e 6172 6368  .components.arch
-000017d0: 6976 6572 2e61 7263 6869 7665 5f6d 616e  iver.archive_man
-000017e0: 6167 6572 720a 0000 005a 2561 736f 6369  agerr....Z%asoci
-000017f0: 6974 612e 636f 6d70 6f6e 656e 7473 2e73  ita.components.s
-00001800: 6574 7469 6e67 732e 7365 7474 696e 6773  ettings.settings
-00001810: 720b 0000 005a 1661 736f 6369 6974 612e  r....Z.asociita.
-00001820: 7574 696c 732e 6865 6c70 6572 7372 0c00  utils.helpersr..
-00001830: 0000 7243 0000 0072 3a00 0000 5a0f 6d75  ..rC...r:...Z.mu
-00001840: 6c74 6970 726f 6365 7373 696e 6772 0d00  ltiprocessingr..
-00001850: 0000 720e 0000 0072 2700 0000 720f 0000  ..r....r'...r...
-00001860: 0072 1000 0000 7218 0000 0072 1800 0000  .r....r....r....
-00001870: 7218 0000 0072 1900 0000 da08 3c6d 6f64  r....r......<mod
-00001880: 756c 653e 0100 0000 7322 0000 000c 0014  ule>....s"......
-00001890: 010c 010c 0114 010c 010c 010c 010c 010c  ................
-000018a0: 0108 0108 0110 0108 030c 010c 0114 03    ...............
+000000d0: 6d18 5a18 0100 6400 640c 6c16 6d19 5a19  m.Z...d.d.l.m.Z.
+000000e0: 0100 6519 640d 640e 640f 8d02 0100 4700  ..e.d.d.d.....G.
+000000f0: 6410 6411 8400 6411 6501 8303 5a1a 640a  d.d...d.e...Z.d.
+00000100: 5300 2912 e900 0000 0029 01da 0c4f 7263  S.)......)...Orc
+00000110: 6865 7374 7261 746f 7229 03da 0c63 7265  hestrator)...cre
+00000120: 6174 655f 6e6f 6465 73da 0c73 616d 706c  ate_nodes..sampl
+00000130: 655f 6e6f 6465 73da 0b74 7261 696e 5f6e  e_nodes..train_n
+00000140: 6f64 6573 2901 da0b 4167 6772 6567 6174  odes)...Aggregat
+00000150: 6f72 7329 01da 074c 6f67 6765 7273 2901  ors)...Loggers).
+00000160: da0a 4f70 7469 6d69 7a65 7273 2901 da12  ..Optimizers)...
+00000170: 4576 616c 7561 7469 6f6e 5f4d 616e 6167  Evaluation_Manag
+00000180: 6572 2901 da0f 4172 6368 6976 655f 4d61  er)...Archive_Ma
+00000190: 6e61 6765 7229 01da 0853 6574 7469 6e67  nager)...Setting
+000001a0: 7329 01da 0748 656c 7065 7273 4e29 02da  s)...HelpersN)..
+000001b0: 0450 6f6f 6cda 074d 616e 6167 6572 2901  .Pool..Manager).
+000001c0: da10 7365 745f 7374 6172 745f 6d65 7468  ..set_start_meth
+000001d0: 6f64 5a05 7370 6177 6e54 2901 5a05 666f  odZ.spawnT).Z.fo
+000001e0: 7263 6563 0000 0000 0000 0000 0000 0000  rcec............
+000001f0: 0000 0000 0400 0000 0000 0000 734c 0000  ............sL..
+00000200: 0065 005a 0164 005a 0264 015a 0364 0265  .e.Z.d.Z.d.Z.d.e
+00000210: 0464 0364 0466 0487 0066 0164 0564 0684  .d.d.f...f.d.d..
+00000220: 0c5a 0564 0765 0665 076a 086a 0965 076a  .Z.d.e.e.j.j.e.j
+00000230: 086a 0966 0219 0064 0364 0466 0464 0864  .j.f...d.d.f.d.d
+00000240: 0984 045a 0a87 0004 005a 0b53 0029 0ada  ...Z.....Z.S.)..
+00000250: 1645 7661 6c75 6174 6f72 5f4f 7263 6865  .Evaluator_Orche
+00000260: 7374 7261 746f 7261 1102 0000 4f72 6368  stratora....Orch
+00000270: 6573 7472 6174 6f72 2069 7320 6120 6365  estrator is a ce
+00000280: 6e74 7261 6c20 6f62 6a65 6374 206e 6563  ntral object nec
+00000290: 6573 7361 7279 2066 6f72 2070 6572 666f  essary for perfo
+000002a0: 726d 696e 6720 7468 6520 7369 6d75 6c61  rming the simula
+000002b0: 7469 6f6e 2e0a 2020 2020 2020 2020 4974  tion..        It
+000002c0: 2063 6f6e 6e65 6374 7320 7468 6520 6e6f   connects the no
+000002d0: 6465 732c 206d 6169 6e74 6169 6e20 7468  des, maintain th
+000002e0: 6520 6b6e 6f77 6c65 6467 6520 6162 6f75  e knowledge abou
+000002f0: 7420 7468 6569 7220 7374 6174 6520 616e  t their state an
+00000300: 6420 6d61 6e61 6765 7320 7468 650a 2020  d manages the.  
+00000310: 2020 2020 2020 6d75 6c74 6974 6872 6561        multithrea
+00000320: 6420 706f 6f6c 2e20 4576 616c 7561 746f  d pool. Evaluato
+00000330: 7220 6f72 6368 6573 7472 6174 6f72 2069  r orchestrator i
+00000340: 7320 6120 6368 696c 6420 636c 6173 7320  s a child class 
+00000350: 6f66 2074 6865 2047 656e 6572 6963 204f  of the Generic O
+00000360: 7263 6865 7374 7261 746f 722e 0a20 2020  rchestrator..   
+00000370: 2020 2020 2055 6e6c 696b 6520 6974 7320       Unlike its 
+00000380: 7061 7265 6e74 2c20 4576 616c 7561 746f  parent, Evaluato
+00000390: 7220 7065 7266 6f72 6d73 2061 2074 7261  r performs a tra
+000003a0: 696e 696e 6720 7573 696e 6720 4665 6465  ining using Fede
+000003b0: 7261 7465 6420 4f70 7469 6d69 7a61 7469  rated Optimizati
+000003c0: 6f6e 0a20 2020 2020 2020 202d 2070 7365  on.        - pse
+000003d0: 7564 6f2d 6772 6164 6965 6e74 7320 6672  udo-gradients fr
+000003e0: 6f6d 2074 6865 206d 6f64 656c 7320 616e  om the models an
+000003f0: 6420 6d6f 6d65 6e74 756d 2e20 4164 6469  d momentum. Addi
+00000400: 7469 6f6e 616c 6c79 2c20 4576 616c 7561  tionally, Evalua
+00000410: 746f 7220 4f72 6368 6573 7472 6174 6f72  tor Orchestrator
+00000420: 0a20 2020 2020 2020 2069 7320 6162 6c65  .        is able
+00000430: 2074 6f20 6173 7365 7373 2063 6c69 656e   to assess clien
+00000440: 7473 206d 6172 6769 6e61 6c20 636f 6e74  ts marginal cont
+00000450: 7269 6275 7469 6f6e 2077 6974 6820 7468  ribution with th
+00000460: 6520 6865 6c70 206f 6620 4576 616c 7561  e help of Evalua
+00000470: 7469 6f6e 204d 616e 6167 6572 2eda 0873  tion Manager...s
+00000480: 6574 7469 6e67 73da 0672 6574 7572 6e4e  ettings..returnN
+00000490: 6302 0000 0000 0000 0000 0000 0003 0000  c...............
+000004a0: 0004 0000 000b 0000 0073 1400 0000 7400  .........s....t.
+000004b0: 8300 6a01 7c01 7c02 6401 8d02 0100 6402  ..j.|.|.d.....d.
+000004c0: 5300 2903 610c 0300 004f 7263 6865 7374  S.).a....Orchest
+000004d0: 7261 746f 7220 6973 2069 6e69 7469 616c  rator is initial
+000004e0: 697a 6564 2062 7920 7061 7373 696e 6720  ized by passing 
+000004f0: 616e 2069 6e73 7461 6e63 650a 2020 2020  an instance.    
+00000500: 2020 2020 6f66 2074 6865 2053 6574 7469      of the Setti
+00000510: 6e67 7320 6f62 6a65 6374 2e20 5365 7474  ngs object. Sett
+00000520: 696e 6773 206f 626a 6563 7420 636f 6e74  ings object cont
+00000530: 6169 6e73 2061 6c6c 2074 6865 2072 656c  ains all the rel
+00000540: 6576 616e 7420 636f 6e66 6967 7572 6174  evant configurat
+00000550: 696f 6e61 6c0a 2020 2020 2020 2020 7365  ional.        se
+00000560: 7474 696e 6773 2074 6861 7420 616e 2069  ttings that an i
+00000570: 6e73 7461 6e63 6520 6f66 2074 6865 204f  nstance of the O
+00000580: 7263 6865 7374 7261 746f 7220 6f62 6a65  rchestrator obje
+00000590: 6374 206d 6179 206e 6565 6420 746f 2063  ct may need to c
+000005a0: 6f6d 706c 6574 6520 7468 6520 7369 6d75  omplete the simu
+000005b0: 6c61 7469 6f6e 2e0a 2020 2020 2020 2020  lation..        
+000005c0: 4576 616c 7561 746f 7220 4f72 6368 6573  Evaluator Orches
+000005d0: 7472 6174 6f72 2061 6464 6974 696f 6e61  trator additiona
+000005e0: 6c79 2072 6571 7569 7265 7320 6120 636f  ly requires a co
+000005f0: 6e66 6967 7572 6174 696f 6e73 2070 6173  nfigurations pas
+00000600: 7365 6420 746f 2074 6865 204f 7074 696d  sed to the Optim
+00000610: 697a 6572 200a 2020 2020 2020 2020 616e  izer .        an
+00000620: 6420 4576 616c 7561 746f 7220 4d61 6e61  d Evaluator Mana
+00000630: 6765 7220 7570 6f6e 2069 7473 2069 6e69  ger upon its ini
+00000640: 7469 616c 697a 6174 696f 6e2e 0a20 2020  tialization..   
+00000650: 2020 2020 200a 2020 2020 2020 2020 5061       .        Pa
+00000660: 7261 6d65 7465 7273 0a20 2020 2020 2020  rameters.       
+00000670: 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020 2020   ----------.    
+00000680: 2020 2020 7365 7474 696e 6773 3a20 5365      settings: Se
+00000690: 7474 696e 6773 200a 2020 2020 2020 2020  ttings .        
+000006a0: 2020 2020 416e 2069 6e73 7461 6e63 6520      An instance 
+000006b0: 6f66 2074 6865 2053 6574 7469 6e67 7320  of the Settings 
+000006c0: 6f62 6a65 6374 2063 6f74 6169 6e69 6e67  object cotaining
+000006d0: 2061 6c6c 2074 6865 2073 6574 7469 6e67   all the setting
+000006e0: 7320 6f66 2074 6865 206f 7263 6865 7374  s of the orchest
+000006f0: 7261 746f 722e 0a20 2020 2020 2020 2020  rator..         
+00000700: 2020 2054 6865 2045 7661 6c75 6174 6f72     The Evaluator
+00000710: 204f 7263 6865 7374 7261 746f 7220 6164   Orchestrator ad
+00000720: 6469 7469 6f6e 616c 7920 7265 7175 6972  ditionaly requir
+00000730: 6573 2074 6865 2070 6173 7365 6420 6f62  es the passed ob
+00000740: 6a65 6374 2074 6f20 636f 6e74 6169 6e20  ject to contain 
+00000750: 6120 0a20 2020 2020 2020 2020 2020 2063  a .            c
+00000760: 6f6e 6669 6775 7261 7469 6f6e 2066 6f72  onfiguration for
+00000770: 2074 6865 204f 7074 696d 697a 6572 2061   the Optimizer a
+00000780: 6e64 2074 6865 2045 7661 6c75 6174 696f  nd the Evaluatio
+00000790: 6e20 4d61 6e61 6765 722e 0a20 2020 2020  n Manager..     
+000007a0: 2020 0a20 2020 2020 2020 5265 7475 726e    .       Return
+000007b0: 730a 2020 2020 2020 202d 2d2d 2d2d 2d2d  s.       -------
+000007c0: 0a20 2020 2020 2020 4e6f 6e65 0a20 2020  .       None.   
+000007d0: 2020 2020 2029 01da 066b 7761 7267 734e       )...kwargsN
+000007e0: 2902 da05 7375 7065 72da 085f 5f69 6e69  )...super..__ini
+000007f0: 745f 5f29 03da 0473 656c 6672 1100 0000  t__)...selfr....
+00000800: 7213 0000 00a9 01da 095f 5f63 6c61 7373  r........__class
+00000810: 5f5f a900 fa86 2f68 6f6d 652f 6d7a 757a  __..../home/mzuz
+00000820: 6961 6b2f 736e 6170 2f73 6e61 7064 2d64  iak/snap/snapd-d
+00000830: 6573 6b74 6f70 2d69 6e74 6567 7261 7469  esktop-integrati
+00000840: 6f6e 2f38 332f 446f 6375 6d65 6e74 732f  on/83/Documents/
+00000850: 4173 6f63 6969 7461 2f61 736f 6369 6974  Asociita/asociit
+00000860: 612f 6173 6f63 6969 7461 2f63 6f6d 706f  a/asociita/compo
+00000870: 6e65 6e74 732f 6f72 6368 6573 7472 6174  nents/orchestrat
+00000880: 6f72 2f65 7661 6c75 6174 6f72 5f6f 7263  or/evaluator_orc
+00000890: 6865 7374 7261 746f 722e 7079 7215 0000  hestrator.pyr...
+000008a0: 001d 0000 0073 0200 0000 1412 7a1f 4576  .....s......z.Ev
+000008b0: 616c 7561 746f 725f 4f72 6368 6573 7472  aluator_Orchestr
+000008c0: 6174 6f72 2e5f 5f69 6e69 745f 5fda 0a6e  ator.__init__..n
+000008d0: 6f64 6573 5f64 6174 6163 0200 0000 0000  odes_datac......
+000008e0: 0000 0000 0000 1900 0000 0a00 0000 0300  ................
+000008f0: 0000 7374 0200 007c 006a 006a 017d 027c  ..st...|.j.j.}.|
+00000900: 006a 006a 027d 037c 006a 006a 037d 0464  .j.j.}.|.j.j.}.d
+00000910: 0164 0284 0074 047c 0383 0144 0083 017d  .d...t.|...D...}
+00000920: 057c 006a 006a 057d 067c 006a 006a 0664  .|.j.j.}.|.j.j.d
+00000930: 036b 0272 2874 077c 006a 006a 087c 006a  .k.r(t.|.j.j.|.j
+00000940: 0964 048d 027d 077c 006a 006a 0a7d 0874  .d...}.|.j.j.}.t
+00000950: 0b7c 006a 0ca0 0da1 007c 0864 058d 027d  .|.j.....|.d...}
+00000960: 0974 0e7c 006a 006a 0f7c 006a 0c7c 057c  .t.|.j.j.|.j.|.|
+00000970: 0264 068d 047d 0a74 107c 057c 006a 006a  .d...}.t.|.|.j.j
+00000980: 1183 027d 0b7c 006a 127c 037c 006a 1364  ...}.|.j.|.|.j.d
+00000990: 078d 027d 0c7c 006a 147c 0b7c 0c7c 0164  ...}.|.j.|.|.|.d
+000009a0: 088d 037d 0b74 047c 0283 0144 005d cf7d  ...}.t.|...D.].}
+000009b0: 0d7c 006a 09a0 1564 097c 0d9b 009d 02a1  .|.j...d.|......
+000009c0: 0101 0069 007d 0e7c 0a6a 167c 006a 0c64  ...i.}.|.j.|.j.d
+000009d0: 0a8d 0101 007c 0a6a 177c 0964 0b8d 0101  .....|.j.|.d....
+000009e0: 0074 187c 0b7c 067c 006a 0964 0c8d 037d  .t.|.|.|.j.d...}
+000009f0: 0f7c 006a 1972 bb74 1a6a 1b7c 0f7c 006a  .|.j.r.t.j.|.|.j
+00000a00: 1c64 0d8d 0244 005d 317d 1074 1d7c 0683  .d...D.]1}.t.|..
+00000a10: 018f 2389 0087 0066 0164 0e64 0284 087c  ..#....f.d.d...|
+00000a20: 1044 0083 017d 117c 1144 005d 0f7d 127c  .D...}.|.D.].}.|
+00000a30: 12a0 1ea1 005c 027d 137d 1474 1fa0 207c  .....\.}.}.t.. |
+00000a40: 14a1 017c 0e7c 133c 0071 9a57 0064 0f04  ...|.|.<.q.W.d..
+00000a50: 0004 0083 0301 006e 0831 0073 b477 0101  .......n.1.s.w..
+00000a60: 0001 0001 0059 0001 0071 886e 2f74 1d7c  .....Y...q.n/t.|
+00000a70: 0683 018f 2389 0087 0066 0164 1064 0284  ....#....f.d.d..
+00000a80: 087c 0f44 0083 017d 117c 1144 005d 0f7d  .|.D...}.|.D.].}
+00000a90: 127c 12a0 1ea1 005c 027d 137d 1574 1fa0  .|.....\.}.}.t..
+00000aa0: 207c 15a1 017c 0e7c 133c 0071 cb57 0064   |...|.|.<.q.W.d
+00000ab0: 0f04 0004 0083 0301 006e 0831 0073 e577  .........n.1.s.w
+00000ac0: 0101 0001 0001 0059 0001 0074 21a0 227c  .......Y...t!."|
+00000ad0: 0ea1 017d 167c 096a 237c 006a 0ca0 0da1  ...}.|.j#|.j....
+00000ae0: 007c 1664 118d 027d 177c 0a6a 247c 006a  .|.d...}.|.j$|.j
+00000af0: 0c64 128d 0101 007c 0a6a 257c 0e7c 0f7c  .d.....|.j%|.|.|
+00000b00: 0d64 138d 0301 007c 006a 0ca0 267c 17a1  .d.....|.j..&|..
+00000b10: 0101 007c 0b44 005d 097d 187c 186a 27a0  ...|.D.].}.|.j'.
+00000b20: 267c 17a1 0101 0090 0171 107c 006a 006a  &|.......q.|.j.j
+00000b30: 0664 036b 0290 0172 2a7c 076a 287c 0d7c  .d.k...r*|.j(|.|
+00000b40: 006a 0c7c 0b64 148d 0301 0071 5b7c 0a6a  .j.|.d.....q[|.j
+00000b50: 297c 076a 2a64 158d 017d 117c 006a 09a0  )|.j*d...}.|.j..
+00000b60: 2b64 16a1 0101 0064 1753 0029 1861 b603  +d.....d.S.).a..
+00000b70: 0000 2250 6572 666f 726d 7320 6120 6675  .."Performs a fu
+00000b80: 6c6c 2066 6564 6572 6174 6564 2074 7261  ll federated tra
+00000b90: 696e 696e 6720 6163 636f 7264 696e 6720  ining according 
+00000ba0: 746f 2074 6865 2069 6e69 7469 616c 697a  to the initializ
+00000bb0: 6564 0a20 2020 2020 2020 2073 6574 7469  ed.        setti
+00000bc0: 6e67 732e 2054 6865 2074 7261 696e 5f70  ngs. The train_p
+00000bd0: 726f 746f 636f 6c20 6f66 2074 6865 206f  rotocol of the o
+00000be0: 7263 6865 7374 7261 746f 722e 6576 616c  rchestrator.eval
+00000bf0: 7561 746f 725f 6f72 6368 6573 7472 6174  uator_orchestrat
+00000c00: 6f72 0a20 2020 2020 2020 2066 6f6c 6c6f  or.        follo
+00000c10: 7773 2061 2070 6f70 756c 6172 2046 6564  ws a popular Fed
+00000c20: 4176 6720 6765 6e65 7261 6c69 7361 7469  Avg generalisati
+00000c30: 6f6e 2c20 4665 644f 7074 2e20 496e 7374  on, FedOpt. Inst
+00000c40: 6561 6420 6f66 2077 6569 6768 7473 2066  ead of weights f
+00000c50: 726f 6d20 6561 6368 0a20 2020 2020 2020  rom each.       
+00000c60: 2063 6c69 656e 7473 2c20 6974 2061 6767   clients, it agg
+00000c70: 7265 6761 7465 7320 6772 6164 6965 6e74  regates gradient
+00000c80: 7320 2875 6e64 6572 7374 6f6f 6420 6173  s (understood as
+00000c90: 2061 2064 6966 6665 7265 6e63 6520 6265   a difference be
+00000ca0: 7477 6565 6e20 7468 6520 7765 6967 6874  tween the weight
+00000cb0: 730a 2020 2020 2020 2020 6f66 2061 206d  s.        of a m
+00000cc0: 6f64 656c 2061 6674 6572 2061 6c6c 2074  odel after all t
+00000cd0: 2065 706f 6368 7320 6f66 2074 6865 206c   epochs of the l
+00000ce0: 6f63 616c 2074 7261 696e 696e 6729 2061  ocal training) a
+00000cf0: 6e64 2061 6767 7265 6761 7465 7320 6163  nd aggregates ac
+00000d00: 636f 7264 696e 6720 746f 200a 2020 2020  cording to .    
+00000d10: 2020 2020 7072 6f76 6964 6564 2072 756c      provided rul
+00000d20: 652e 2054 6865 2065 7661 6c75 6174 696f  e. The evaluatio
+00000d30: 6e20 7072 6f63 6573 7320 6973 206d 656e  n process is men
+00000d40: 6167 6564 2062 7920 7468 6520 696e 7374  aged by the inst
+00000d50: 616e 6365 206f 6620 7468 6520 4576 616c  ance of the Eval
+00000d60: 7561 7469 6f6e 0a20 2020 2020 2020 204d  uation.        M
+00000d70: 616e 6167 6572 206f 626a 6563 742c 2077  anager object, w
+00000d80: 6869 6368 2069 7320 6361 6c6c 6564 2075  hich is called u
+00000d90: 706f 6e20 6561 6368 2069 7465 7261 7469  pon each iterati
+00000da0: 6f6e 2e0a 0a20 2020 2020 2020 2050 6172  on...        Par
+00000db0: 616d 6574 6572 730a 2020 2020 2020 2020  ameters.        
+00000dc0: 2d2d 2d2d 2d2d 2d2d 2d2d 0a20 2020 2020  ----------.     
+00000dd0: 2020 206e 6f64 6573 5f64 6174 613a 206c     nodes_data: l
+00000de0: 6973 745b 6461 7461 7365 7473 2e61 7272  ist[datasets.arr
+00000df0: 6f77 5f64 6174 6173 6574 2e44 6174 6173  ow_dataset.Datas
+00000e00: 6574 2c20 6461 7461 7365 7473 2e61 7272  et, datasets.arr
+00000e10: 6f77 5f64 6174 6173 6574 2e44 6174 6173  ow_dataset.Datas
+00000e20: 6574 5d3a 200a 2020 2020 2020 2020 2020  et]: .          
+00000e30: 2020 4120 6c69 7374 2063 6f6e 7461 696e    A list contain
+00000e40: 696e 6720 7472 6169 6e20 7365 7420 616e  ing train set an
+00000e50: 6420 7465 7374 2073 6574 2077 7261 7070  d test set wrapp
+00000e60: 6564 200a 2020 2020 2020 2020 2020 2020  ed .            
+00000e70: 696e 2061 2068 7567 6769 6e67 2066 6163  in a hugging fac
+00000e80: 6520 6172 726f 775f 6461 7461 7365 742e  e arrow_dataset.
+00000e90: 4461 7461 7365 7420 636f 6e74 6169 6e65  Dataset containe
+00000ea0: 7273 0a20 2020 2020 2020 200a 2020 2020  rs.        .    
+00000eb0: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00000ec0: 2020 2020 2d2d 2d2d 2d2d 2d0a 2020 2020      -------.    
+00000ed0: 2020 2020 696e 740a 2020 2020 2020 2020      int.        
+00000ee0: 2020 2020 5265 7475 726e 7320 3020 6f6e      Returns 0 on
+00000ef0: 2074 6865 2073 7563 6365 7373 6675 6c20   the successful 
+00000f00: 636f 6d70 6c65 7469 6f6e 206f 6620 7468  completion of th
+00000f10: 6520 7472 6169 6e69 6e67 2e0a 2020 2020  e training..    
+00000f20: 2020 2020 2020 2020 6301 0000 0000 0000          c.......
+00000f30: 0000 0000 0002 0000 0003 0000 0053 0000  .............S..
+00000f40: 0073 1000 0000 6700 7c00 5d04 7d01 7c01  .s....g.|.].}.|.
+00000f50: 9102 7102 5300 7219 0000 0072 1900 0000  ..q.S.r....r....
+00000f60: a902 da02 2e30 da04 6e6f 6465 7219 0000  .....0..noder...
+00000f70: 0072 1900 0000 721a 0000 00da 0a3c 6c69  .r....r......<li
+00000f80: 7374 636f 6d70 3e4d 0000 0073 0200 0000  stcomp>M...s....
+00000f90: 1000 7a39 4576 616c 7561 746f 725f 4f72  ..z9Evaluator_Or
+00000fa0: 6368 6573 7472 6174 6f72 2e74 7261 696e  chestrator.train
+00000fb0: 5f70 726f 746f 636f 6c2e 3c6c 6f63 616c  _protocol.<local
+00000fc0: 733e 2e3c 6c69 7374 636f 6d70 3e54 2902  s>.<listcomp>T).
+00000fd0: da0f 6172 6368 6976 655f 6d61 6e61 6765  ..archive_manage
+00000fe0: 725a 066c 6f67 6765 7229 02da 0777 6569  rZ.logger)...wei
+00000ff0: 6768 7473 7211 0000 0029 0472 1100 0000  ghtsr....).r....
+00001000: da05 6d6f 6465 6cda 056e 6f64 6573 da0a  ..model..nodes..
+00001010: 6974 6572 6174 696f 6e73 2902 da0c 6e6f  iterations)...no
+00001020: 6465 735f 6e75 6d62 6572 7222 0000 0029  des_numberr"...)
+00001030: 035a 0a6e 6f64 6573 5f6c 6973 74da 0a6d  .Z.nodes_list..m
+00001040: 6f64 656c 5f6c 6973 745a 0964 6174 615f  odel_listZ.data_
+00001050: 6c69 7374 7a0a 4974 6572 6174 696f 6e20  listz.Iteration 
+00001060: 2901 5a0e 7072 6576 696f 7573 5f6d 6f64  ).Z.previous_mod
+00001070: 656c 2901 5a12 7072 6576 696f 7573 5f6f  el).Z.previous_o
+00001080: 7074 696d 697a 6572 2902 da0b 7361 6d70  ptimizer)...samp
+00001090: 6c65 5f73 697a 65da 136f 7263 6865 7374  le_size..orchest
+000010a0: 7261 746f 725f 6c6f 6767 6572 2901 da04  rator_logger)...
+000010b0: 7369 7a65 6301 0000 0000 0000 0000 0000  sizec...........
+000010c0: 0002 0000 0007 0000 0013 0000 00f3 1c00  ................
+000010d0: 0000 6700 7c00 5d0a 7d01 8800 a000 7401  ..g.|.].}.....t.
+000010e0: 7c01 6400 6602 a102 9102 7102 5300 a901  |.d.f.....q.S...
+000010f0: da09 6772 6164 6965 6e74 73a9 025a 0b61  ..gradients..Z.a
+00001100: 7070 6c79 5f61 7379 6e63 7205 0000 0072  pply_asyncr....r
+00001110: 1c00 0000 a901 5a04 706f 6f6c 7219 0000  ......Z.poolr...
+00001120: 0072 1a00 0000 721f 0000 0079 0000 00f3  .r....r....y....
+00001130: 0200 0000 1c00 4e63 0100 0000 0000 0000  ......Nc........
+00001140: 0000 0000 0200 0000 0700 0000 1300 0000  ................
+00001150: 722a 0000 0072 2b00 0000 722d 0000 0072  r*...r+...r-...r
+00001160: 1c00 0000 722e 0000 0072 1900 0000 721a  ....r....r....r.
+00001170: 0000 0072 1f00 0000 8000 0000 722f 0000  ...r........r/..
+00001180: 0029 0272 2100 0000 5a05 6465 6c74 6129  .).r!...Z.delta)
+00001190: 015a 0d75 7064 6174 6564 5f6d 6f64 656c  .Z.updated_model
+000011a0: 2903 722c 0000 005a 0f6e 6f64 6573 5f69  ).r,...Z.nodes_i
+000011b0: 6e5f 7361 6d70 6c65 da09 6974 6572 6174  n_sample..iterat
+000011c0: 696f 6e29 0372 3000 0000 da0d 6365 6e74  ion).r0.....cent
+000011d0: 7261 6c5f 6d6f 6465 6c72 2300 0000 2901  ral_modelr#...).
+000011e0: da04 7061 7468 7a11 5472 6169 6e69 6e67  ..pathz.Training
+000011f0: 2063 6f6d 706c 6574 6572 0100 0000 292c   completer....),
+00001200: 7211 0000 0072 2400 0000 da0f 6e75 6d62  r....r$.....numb
+00001210: 6572 5f6f 665f 6e6f 6465 73da 106c 6f63  er_of_nodes..loc
+00001220: 616c 5f77 6172 6d5f 7374 6172 74da 0572  al_warm_start..r
+00001230: 616e 6765 7227 0000 00da 0f65 6e61 626c  anger'.....enabl
+00001240: 655f 6172 6368 6976 6572 720a 0000 005a  e_archiverr....Z
+00001250: 1161 7263 6869 7665 725f 7365 7474 696e  .archiver_settin
+00001260: 6773 7228 0000 00da 126f 7074 696d 697a  gsr(.....optimiz
+00001270: 6572 5f73 6574 7469 6e67 7372 0800 0000  er_settingsr....
+00001280: 7231 0000 005a 0b67 6574 5f77 6569 6768  r1...Z.get_weigh
+00001290: 7473 7209 0000 005a 1265 7661 6c75 6174  tsr....Z.evaluat
+000012a0: 6f72 5f73 6574 7469 6e67 7372 0300 0000  or_settingsr....
+000012b0: 5a0e 6e6f 6465 735f 7365 7474 696e 6773  Z.nodes_settings
+000012c0: 5a14 6d6f 6465 6c5f 696e 6974 6961 6c69  Z.model_initiali
+000012d0: 7a61 7469 6f6e 5a0b 6365 6e74 7261 6c5f  zationZ.central_
+000012e0: 6e65 745a 146e 6f64 6573 5f69 6e69 7469  netZ.nodes_initi
+000012f0: 616c 697a 6174 696f 6eda 0469 6e66 6f5a  alization..infoZ
+00001300: 1770 7265 7365 7276 655f 7072 6576 696f  .preserve_previo
+00001310: 7573 5f6d 6f64 656c 5a1b 7072 6573 6572  us_modelZ.preser
+00001320: 7665 5f70 7265 7669 6f75 735f 6f70 7469  ve_previous_opti
+00001330: 6d69 7a65 7272 0400 0000 5a09 6261 7463  mizerr....Z.batc
+00001340: 685f 6a6f 6272 0c00 0000 5a07 6368 756e  h_jobr....Z.chun
+00001350: 6b65 72da 0562 6174 6368 720d 0000 00da  ker..batchr.....
+00001360: 0367 6574 da04 636f 7079 5a08 6465 6570  .get..copyZ.deep
+00001370: 636f 7079 7206 0000 005a 0f63 6f6d 7075  copyr....Z.compu
+00001380: 7465 5f61 7665 7261 6765 5a0c 6665 645f  te_averageZ.fed_
+00001390: 6f70 7469 6d69 7a65 5a16 7072 6573 6572  optimizeZ.preser
+000013a0: 7665 5f75 7064 6174 6564 5f6d 6f64 656c  ve_updated_model
+000013b0: 5a0d 7472 6163 6b5f 7265 7375 6c74 735a  Z.track_resultsZ
+000013c0: 0e75 7064 6174 655f 7765 6967 6874 7372  .update_weightsr
+000013d0: 2200 0000 5a18 6172 6368 6976 655f 7472  "...Z.archive_tr
+000013e0: 6169 6e69 6e67 5f72 6573 756c 7473 5a11  aining_resultsZ.
+000013f0: 6669 6e61 6c69 7a65 5f74 7261 636b 696e  finalize_trackin
+00001400: 675a 106d 6574 7269 6373 5f73 6176 6570  gZ.metrics_savep
+00001410: 6174 685a 0863 7269 7469 6361 6c29 1972  athZ.critical).r
+00001420: 1600 0000 721b 0000 0072 2400 0000 7225  ....r....r$...r%
+00001430: 0000 0072 3400 0000 7223 0000 0072 2700  ...r4...r#...r'.
+00001440: 0000 7220 0000 0072 3700 0000 5a05 4f70  ..r ...r7...Z.Op
+00001450: 7469 6d5a 1265 7661 6c75 6174 696f 6e5f  timZ.evaluation_
+00001460: 6d61 6e61 6765 725a 0b6e 6f64 6573 5f67  managerZ.nodes_g
+00001470: 7265 656e 7226 0000 0072 3000 0000 722c  reenr&...r0...r,
+00001480: 0000 005a 0d73 616d 706c 6564 5f6e 6f64  ...Z.sampled_nod
+00001490: 6573 7239 0000 005a 0772 6573 756c 7473  esr9...Z.results
+000014a0: da06 7265 7375 6c74 5a07 6e6f 6465 5f69  ..resultZ.node_i
+000014b0: 645a 0d6d 6f64 656c 5f77 6569 6768 7473  dZ.model_weights
+000014c0: 5a0f 6d6f 6465 6c5f 6772 6164 6965 6e74  Z.model_gradient
+000014d0: 735a 0867 7261 645f 6176 675a 0f75 7064  sZ.grad_avgZ.upd
+000014e0: 6174 6564 5f77 6569 6768 7473 721e 0000  ated_weightsr...
+000014f0: 0072 1900 0000 722e 0000 0072 1a00 0000  .r....r....r....
+00001500: da0e 7472 6169 6e5f 7072 6f74 6f63 6f6c  ..train_protocol
+00001510: 3200 0000 739a 0000 0008 1808 0108 0112  2...s...........
+00001520: 0108 010c 0302 0106 0104 0106 fe08 050a  ................
+00001530: 0102 0106 ff08 0404 0102 0102 0106 fd04  ................
+00001540: 0606 0104 ff06 0304 0106 ff06 0302 0102  ................
+00001550: 0106 fe0c 0412 0104 010e 020c 0104 0202  ................
+00001560: 0104 0106 fe06 0314 010a 0112 0108 020c  ................
+00001570: 0110 0102 fe1c fd02 8002 ff0a 0812 0108  ................
+00001580: 020c 0110 0102 fe1c fd0a 080c 0202 0106  ................
+00001590: ff0e 0306 0302 0102 0106 fe0c 0508 0210  ................
+000015a0: 010e 0306 0104 0102 0106 fe02 800e 060c  ................
+000015b0: 0104 017a 2545 7661 6c75 6174 6f72 5f4f  ...z%Evaluator_O
+000015c0: 7263 6865 7374 7261 746f 722e 7472 6169  rchestrator.trai
+000015d0: 6e5f 7072 6f74 6f63 6f6c 290c da08 5f5f  n_protocol)...__
+000015e0: 6e61 6d65 5f5f da0a 5f5f 6d6f 6475 6c65  name__..__module
+000015f0: 5f5f da0c 5f5f 7175 616c 6e61 6d65 5f5f  __..__qualname__
+00001600: da07 5f5f 646f 635f 5f72 0b00 0000 7215  ..__doc__r....r.
+00001610: 0000 00da 046c 6973 74da 0864 6174 6173  .....list..datas
+00001620: 6574 735a 0d61 7272 6f77 5f64 6174 6173  etsZ.arrow_datas
+00001630: 6574 5a07 4461 7461 7365 7472 3d00 0000  etZ.Datasetr=...
+00001640: da0d 5f5f 636c 6173 7363 656c 6c5f 5f72  ..__classcell__r
+00001650: 1900 0000 7219 0000 0072 1700 0000 721a  ....r....r....r.
+00001660: 0000 0072 1000 0000 1400 0000 7314 0000  ...r........s...
+00001670: 0008 0004 0116 0802 1508 0106 0104 ff02  ................
+00001680: ff02 0212 fe72 1000 0000 291b 5a35 6173  .....r....).Z5as
+00001690: 6f63 6969 7461 2e63 6f6d 706f 6e65 6e74  ociita.component
+000016a0: 732e 6f72 6368 6573 7472 6174 6f72 2e67  s.orchestrator.g
+000016b0: 656e 6572 6963 5f6f 7263 6865 7374 7261  eneric_orchestra
+000016c0: 746f 7272 0200 0000 5a1d 6173 6f63 6969  torr....Z.asocii
+000016d0: 7461 2e75 7469 6c73 2e6f 7263 6865 7374  ta.utils.orchest
+000016e0: 7261 7469 6f6e 7372 0300 0000 7204 0000  rationsr....r...
+000016f0: 0072 0500 0000 5a1b 6173 6f63 6969 7461  .r....Z.asociita
+00001700: 2e75 7469 6c73 2e63 6f6d 7075 7461 7469  .utils.computati
+00001710: 6f6e 7372 0600 0000 5a16 6173 6f63 6969  onsr....Z.asocii
+00001720: 7461 2e75 7469 6c73 2e6c 6f67 6765 7273  ta.utils.loggers
+00001730: 7207 0000 005a 1961 736f 6369 6974 612e  r....Z.asociita.
+00001740: 7574 696c 732e 6f70 7469 6d69 7a65 7273  utils.optimizers
+00001750: 7208 0000 005a 3061 736f 6369 6974 612e  r....Z0asociita.
+00001760: 636f 6d70 6f6e 656e 7473 2e65 7661 6c75  components.evalu
+00001770: 6174 6f72 2e65 7661 6c75 6174 696f 6e5f  ator.evaluation_
+00001780: 6d61 6e61 6765 7272 0900 0000 5a2c 6173  managerr....Z,as
+00001790: 6f63 6969 7461 2e63 6f6d 706f 6e65 6e74  ociita.component
+000017a0: 732e 6172 6368 6976 6572 2e61 7263 6869  s.archiver.archi
+000017b0: 7665 5f6d 616e 6167 6572 720a 0000 005a  ve_managerr....Z
+000017c0: 2561 736f 6369 6974 612e 636f 6d70 6f6e  %asociita.compon
+000017d0: 656e 7473 2e73 6574 7469 6e67 732e 7365  ents.settings.se
+000017e0: 7474 696e 6773 720b 0000 005a 1661 736f  ttingsr....Z.aso
+000017f0: 6369 6974 612e 7574 696c 732e 6865 6c70  ciita.utils.help
+00001800: 6572 7372 0c00 0000 7243 0000 0072 3b00  ersr....rC...r;.
+00001810: 0000 5a0f 6d75 6c74 6970 726f 6365 7373  ..Z.multiprocess
+00001820: 696e 6772 0d00 0000 720e 0000 0072 0f00  ingr....r....r..
+00001830: 0000 7210 0000 0072 1900 0000 7219 0000  ..r....r....r...
+00001840: 0072 1900 0000 721a 0000 00da 083c 6d6f  .r....r......<mo
+00001850: 6475 6c65 3e01 0000 0073 2000 0000 0c00  dule>....s .....
+00001860: 1401 0c01 0c01 1401 0c01 0c01 0c01 0c01  ................
+00001870: 0c01 0801 0801 1001 0c03 0c01 1403       ..............
```

### Comparing `asociita-0.3.2/asociita/components/orchestrator/__pycache__/fedopt_orchestrator.cpython-310.pyc` & `asociita-0.3.3/asociita/components/orchestrator/__pycache__/fedopt_orchestrator.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/orchestrator/__pycache__/generic_orchestrator.cpython-310.pyc` & `asociita-0.3.3/asociita/components/orchestrator/__pycache__/generic_orchestrator.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 13 09:32:16 2023 UTC, .py size: 11545 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 a0c4 af64 192d 0000  o..........d.-..
+00000000: 6f0d 0d0a 0000 0000 baf1 b364 192d 0000  o..........d.-..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 d600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6402 6c02 6d03 5a03 0100 6400 6403 6c04  d.l.m.Z...d.d.l.
 00000050: 6d05 5a05 0100 6400 6404 6c06 6d07 5a07  m.Z...d.d.l.m.Z.
 00000060: 0100 6400 6405 6c08 6d09 5a09 0100 6400  ..d.d.l.m.Z...d.
 00000070: 6406 6c0a 6d0b 5a0b 0100 6400 6407 6c0c  d.l.m.Z...d.d.l.
@@ -165,17 +165,17 @@
 00000a40: 6869 7465 6374 7572 6520 7468 6174 2077  hitecture that w
 00000a50: 696c 6c20 6265 2075 7365 6420 7468 726f  ill be used thro
 00000a60: 7567 686f 7574 2074 6865 2074 7261 696e  ughout the train
 00000a70: 696e 672e 0a20 2020 2020 2020 200a 2020  ing..        .  
 00000a80: 2020 2020 2020 5265 7475 726e 730a 2020        Returns.  
 00000a90: 2020 2020 2020 2d2d 2d2d 2d2d 2d0a 2020        -------.  
 00000aa0: 2020 2020 2020 4e6f 6e65 da0c 6f72 6368        None..orch
-00000ab0: 6573 7472 6174 6f72 2904 7215 0000 00da  estrator).r.....
+00000ab0: 6573 7472 6174 6f72 2904 7215 0000 005a  estrator).r....Z
 00000ac0: 036e 6574 5a0d 6c6f 6361 6c5f 6461 7461  .netZ.local_data
-00000ad0: 7365 74da 096e 6f64 655f 6e61 6d65 4e29  set..node_nameN)
+00000ad0: 7365 745a 096e 6f64 655f 6e61 6d65 4e29  setZ.node_nameN)
 00000ae0: 0672 2200 0000 da0b 6365 6e74 7261 6c5f  .r".....central_
 00000af0: 6e65 7472 0400 0000 7215 0000 00da 0e6d  netr....r......m
 00000b00: 6f64 656c 5f73 6574 7469 6e67 73da 0d63  odel_settings..c
 00000b10: 656e 7472 616c 5f6d 6f64 656c 2903 721d  entral_model).r.
 00000b20: 0000 0072 1a00 0000 7222 0000 0072 1f00  ...r....r"...r..
 00000b30: 0000 721f 0000 0072 2000 0000 da14 7072  ..r....r .....pr
 00000b40: 6570 6172 655f 6f72 6368 6573 7472 6174  epare_orchestrat
@@ -270,23 +270,23 @@
 000010d0: 0072 1f00 0000 7220 0000 00da 0a3c 6c69  .r....r .....<li
 000010e0: 7374 636f 6d70 3e7d 0000 0073 0200 0000  stcomp>}...s....
 000010f0: 1600 7a35 4f72 6368 6573 7472 6174 6f72  ..z5Orchestrator
 00001100: 2e6d 6f64 656c 5f69 6e69 7469 616c 697a  .model_initializ
 00001110: 6174 696f 6e2e 3c6c 6f63 616c 733e 2e3c  ation.<locals>.<
 00001120: 6c69 7374 636f 6d70 3e29 02da 134e 6f74  listcomp>)...Not
 00001130: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-00001140: da05 7261 6e67 6529 0572 1d00 0000 722a  ..range).r....r*
-00001150: 0000 0072 1a00 0000 722b 0000 00da 0a6d  ...r....r+.....m
-00001160: 6f64 656c 5f6c 6973 7472 1f00 0000 7230  odel_listr....r0
+00001140: da05 7261 6e67 6529 0572 1d00 0000 7228  ..range).r....r(
+00001150: 0000 0072 1a00 0000 7229 0000 00da 0a6d  ...r....r).....m
+00001160: 6f64 656c 5f6c 6973 7472 1f00 0000 722e  odel_listr....r.
 00001170: 0000 0072 2000 0000 da14 6d6f 6465 6c5f  ...r .....model_
 00001180: 696e 6974 6961 6c69 7a61 7469 6f6e 5900  initializationY.
 00001190: 0000 7308 0000 0008 2008 0116 0304 017a  ..s..... ......z
 000011a0: 214f 7263 6865 7374 7261 746f 722e 6d6f  !Orchestrator.mo
 000011b0: 6465 6c5f 696e 6974 6961 6c69 7a61 7469  del_initializati
-000011c0: 6f6e da0a 6e6f 6465 735f 6c69 7374 7234  on..nodes_listr4
+000011c0: 6f6e da0a 6e6f 6465 735f 6c69 7374 7232  on..nodes_listr2
 000011d0: 0000 00da 0964 6174 615f 6c69 7374 6304  .....data_listc.
 000011e0: 0000 0000 0000 0000 0000 000a 0000 0005  ................
 000011f0: 0000 0043 0000 0073 5c00 0000 6700 7d04  ...C...s\...g.}.
 00001200: 7400 7c01 7c02 7c03 8303 4400 5d10 5c03  t.|.|.|...D.].\.
 00001210: 7d05 7d06 7d07 7c05 a001 7c06 7c07 a102  }.}.}.|...|.|...
 00001220: 0100 7c04 a002 7c05 a101 0100 7108 6700  ..|...|.....q.g.
 00001230: 7d08 7c04 4400 5d0e 7d09 7403 7c09 7c00  }.|.D.].}.t.|.|.
@@ -347,17 +347,17 @@
 000015a0: 2020 2020 2020 200a 2020 2020 2020 2020         .        
 000015b0: 5261 6973 6573 0a20 2020 2020 2020 202d  Raises.        -
 000015c0: 2d2d 2d2d 2d0a 2020 2020 2020 2020 2020  -----.          
 000015d0: 2020 6c69 7374 5b46 6564 6572 6174 6564    list[Federated
 000015e0: 4e6f 6465 5d29 0172 1c00 0000 2905 da03  Node]).r....)...
 000015f0: 7a69 705a 0c70 7265 7061 7265 5f6e 6f64  zipZ.prepare_nod
 00001600: 65da 0661 7070 656e 6472 0800 0000 721c  e..appendr....r.
-00001610: 0000 0029 0a72 1d00 0000 7236 0000 0072  ...).r....r6...r
-00001620: 3400 0000 7237 0000 00da 0772 6573 756c  4...r7.....resul
-00001630: 7473 da04 6e6f 6465 721a 0000 00da 0764  ts..noder......d
+00001610: 0000 0029 0a72 1d00 0000 7234 0000 0072  ...).r....r4...r
+00001620: 3200 0000 7235 0000 00da 0772 6573 756c  2...r5.....resul
+00001630: 7473 da04 6e6f 6465 721a 0000 005a 0764  ts..noder....Z.d
 00001640: 6174 6173 6574 da0b 6e6f 6465 735f 6772  ataset..nodes_gr
 00001650: 6565 6eda 0672 6573 756c 7472 1f00 0000  een..resultr....
 00001660: 721f 0000 0072 2000 0000 da14 6e6f 6465  r....r .....node
 00001670: 735f 696e 6974 6961 6c69 7a61 7469 6f6e  s_initialization
 00001680: 8100 0000 7318 0000 0004 1b16 010c 010c  ....s...........
 00001690: 0104 0108 0104 0104 0106 ff0a 0202 8004  ................
 000016a0: 017a 214f 7263 6865 7374 7261 746f 722e  .z!Orchestrator.
@@ -443,68 +443,68 @@
 00001ba0: 2020 2020 2020 2052 6574 7572 6e73 2030         Returns 0
 00001bb0: 206f 6e20 7468 6520 7375 6363 6573 7366   on the successf
 00001bc0: 756c 2063 6f6d 706c 6574 696f 6e20 6f66  ul completion of
 00001bd0: 2074 6865 2074 7261 696e 696e 672e 6301   the training.c.
 00001be0: 0000 0000 0000 0000 0000 0002 0000 0003  ................
 00001bf0: 0000 0053 0000 0073 1000 0000 6700 7c00  ...S...s....g.|.
 00001c00: 5d04 7d01 7c01 9102 7102 5300 721f 0000  ].}.|...q.S.r...
-00001c10: 0072 1f00 0000 a902 722e 0000 0072 3b00  .r......r....r;.
+00001c10: 0072 1f00 0000 a902 722c 0000 0072 3900  .r......r,...r9.
 00001c20: 0000 721f 0000 0072 1f00 0000 7220 0000  ..r....r....r ..
-00001c30: 0072 3100 0000 c000 0000 7302 0000 0010  .r1.......s.....
+00001c30: 0072 2f00 0000 c000 0000 7302 0000 0010  .r/.......s.....
 00001c40: 007a 2f4f 7263 6865 7374 7261 746f 722e  .z/Orchestrator.
 00001c50: 7472 6169 6e5f 7072 6f74 6f63 6f6c 2e3c  train_protocol.<
 00001c60: 6c6f 6361 6c73 3e2e 3c6c 6973 7463 6f6d  locals>.<listcom
 00001c70: 703e 5429 02da 0f61 7263 6869 7665 5f6d  p>T)...archive_m
 00001c80: 616e 6167 6572 da06 6c6f 6767 6572 2902  anager..logger).
-00001c90: 722a 0000 0072 1a00 0000 2903 7236 0000  r*...r....).r6..
-00001ca0: 0072 3400 0000 7237 0000 007a 0a49 7465  .r4...r7...z.Ite
+00001c90: 7228 0000 0072 1a00 0000 2903 7234 0000  r(...r....).r4..
+00001ca0: 0072 3200 0000 7235 0000 007a 0a49 7465  .r2...r5...z.Ite
 00001cb0: 7261 7469 6f6e 2029 02da 0b73 616d 706c  ration )...sampl
 00001cc0: 655f 7369 7a65 721c 0000 0029 01da 0473  e_sizer....)...s
 00001cd0: 697a 6563 0100 0000 0000 0000 0000 0000  izec............
 00001ce0: 0200 0000 0600 0000 1300 0000 f31a 0000  ................
 00001cf0: 0067 007c 005d 097d 0188 00a0 0074 017c  .g.|.].}.....t.|
 00001d00: 0166 01a1 0291 0271 0253 0072 1f00 0000  .f.....q.S.r....
 00001d10: a902 da0b 6170 706c 795f 6173 796e 6372  ....apply_asyncr
-00001d20: 0a00 0000 7241 0000 00a9 01da 0470 6f6f  ....rA.......poo
-00001d30: 6c72 1f00 0000 7220 0000 0072 3100 0000  lr....r ...r1...
+00001d20: 0a00 0000 723e 0000 00a9 01da 0470 6f6f  ....r>.......poo
+00001d30: 6c72 1f00 0000 7220 0000 0072 2f00 0000  lr....r ...r/...
 00001d40: e300 0000 f302 0000 001a 004e 6301 0000  ...........Nc...
 00001d50: 0000 0000 0000 0000 0002 0000 0006 0000  ................
-00001d60: 0013 0000 0072 4600 0000 721f 0000 0072  .....rF...r....r
-00001d70: 4700 0000 7241 0000 0072 4900 0000 721f  G...rA...rI...r.
-00001d80: 0000 0072 2000 0000 7231 0000 00ea 0000  ...r ...r1......
-00001d90: 0072 4b00 0000 2903 da09 6974 6572 6174  .rK...)...iterat
-00001da0: 696f 6e72 2800 0000 da05 6e6f 6465 7329  ionr(.....nodes)
-00001db0: 0172 4c00 0000 7a11 5472 6169 6e69 6e67  .rL...z.Training
+00001d60: 0013 0000 0072 4300 0000 721f 0000 0072  .....rC...r....r
+00001d70: 4400 0000 723e 0000 0072 4600 0000 721f  D...r>...rF...r.
+00001d80: 0000 0072 2000 0000 722f 0000 00ea 0000  ...r ...r/......
+00001d90: 0072 4800 0000 2903 da09 6974 6572 6174  .rH...)...iterat
+00001da0: 696f 6e72 2600 0000 da05 6e6f 6465 7329  ionr&.....nodes)
+00001db0: 0172 4900 0000 7a11 5472 6169 6e69 6e67  .rI...z.Training
 00001dc0: 2063 6f6d 706c 6574 6572 0100 0000 2920   completer....) 
 00001dd0: 7215 0000 00da 0a69 7465 7261 7469 6f6e  r......iteration
 00001de0: 73da 0f6e 756d 6265 725f 6f66 5f6e 6f64  s..number_of_nod
-00001df0: 6573 722b 0000 0072 3300 0000 7244 0000  esr+...r3...rD..
+00001df0: 6573 7229 0000 0072 3100 0000 7241 0000  esr)...r1...rA..
 00001e00: 00da 0f65 6e61 626c 655f 6172 6368 6976  ...enable_archiv
 00001e10: 6572 720b 0000 00da 1161 7263 6869 7665  err......archive
 00001e20: 725f 7365 7474 696e 6773 721c 0000 0072  r_settingsr....r
 00001e30: 0700 0000 da0e 6e6f 6465 735f 7365 7474  ......nodes_sett
-00001e40: 696e 6773 7235 0000 0072 2600 0000 723f  ingsr5...r&...r?
+00001e40: 696e 6773 7233 0000 0072 2400 0000 723c  ingsr3...r$...r<
 00001e50: 0000 00da 0469 6e66 6f72 0900 0000 7218  .....infor....r.
 00001e60: 0000 0072 1000 0000 da07 6368 756e 6b65  ...r......chunke
 00001e70: 7272 1900 0000 720d 0000 0072 1b00 0000  rr....r....r....
 00001e80: 7205 0000 00da 0f63 6f6d 7075 7465 5f61  r......compute_a
 00001e90: 7665 7261 6765 721a 0000 00da 0e75 7064  verager......upd
-00001ea0: 6174 655f 7765 6967 6874 7372 2800 0000  ate_weightsr(...
+00001ea0: 6174 655f 7765 6967 6874 7372 2600 0000  ate_weightsr&...
 00001eb0: da18 6172 6368 6976 655f 7472 6169 6e69  ..archive_traini
 00001ec0: 6e67 5f72 6573 756c 7473 7217 0000 0072  ng_resultsr....r
 00001ed0: 0f00 0000 da08 6372 6974 6963 616c 2914  ......critical).
-00001ee0: 721d 0000 0072 4000 0000 724e 0000 0072  r....r@...rN...r
-00001ef0: 2a00 0000 722b 0000 0072 4d00 0000 7244  *...r+...rM...rD
-00001f00: 0000 0072 4200 0000 723d 0000 0072 3400  ...rB...r=...r4.
-00001f10: 0000 724c 0000 00da 0777 6569 6768 7473  ..rL.....weights
+00001ee0: 721d 0000 0072 3d00 0000 724b 0000 0072  r....r=...rK...r
+00001ef0: 2800 0000 7229 0000 0072 4a00 0000 7241  (...r)...rJ...rA
+00001f00: 0000 0072 3f00 0000 723a 0000 0072 3200  ...r?...r:...r2.
+00001f10: 0000 7249 0000 00da 0777 6569 6768 7473  ..rI.....weights
 00001f20: da0d 7361 6d70 6c65 645f 6e6f 6465 7372  ..sampled_nodesr
-00001f30: 1900 0000 723a 0000 0072 3e00 0000 da07  ....r:...r>.....
+00001f30: 1900 0000 7238 0000 0072 3b00 0000 da07  ....r8...r;.....
 00001f40: 6e6f 6465 5f69 64da 0d6d 6f64 656c 5f77  node_id..model_w
-00001f50: 6569 6768 7473 da03 6176 6772 3b00 0000  eights..avgr;...
-00001f60: 721f 0000 0072 4900 0000 7220 0000 00da  r....rI...r ....
+00001f50: 6569 6768 7473 5a03 6176 6772 3900 0000  eightsZ.avgr9...
+00001f60: 721f 0000 0072 4600 0000 7220 0000 00da  r....rF...r ....
 00001f70: 0e74 7261 696e 5f70 726f 746f 636f 6ca8  .train_protocol.
 00001f80: 0000 0073 7600 0000 0815 0801 0801 1201  ...sv...........
 00001f90: 0801 0c03 0201 0601 0401 06fe 0405 0601  ................
 00001fa0: 04ff 0605 0401 06ff 0604 0201 0201 06fe  ................
 00001fb0: 0c06 1201 0401 0402 0201 0401 06fe 0603  ................
 00001fc0: 1401 0a01 1201 0802 0c01 0a01 02fe 1cfd  ................
 00001fd0: 0280 02ff 0a08 1201 0802 0c01 0a01 02fe  ................
@@ -513,27 +513,27 @@
 00002000: 4f72 6368 6573 7472 6174 6f72 2e74 7261  Orchestrator.tra
 00002010: 696e 5f70 726f 746f 636f 6c29 0146 2914  in_protocol).F).
 00002020: da08 5f5f 6e61 6d65 5f5f da0a 5f5f 6d6f  ..__name__..__mo
 00002030: 6475 6c65 5f5f da0c 5f5f 7175 616c 6e61  dule__..__qualna
 00002040: 6d65 5f5f da07 5f5f 646f 635f 5f72 0c00  me__..__doc__r..
 00002050: 0000 7221 0000 0072 0e00 0000 da08 6461  ..r!...r......da
 00002060: 7461 7365 7473 da0d 6172 726f 775f 6461  tasets..arrow_da
-00002070: 7461 7365 74da 0744 6174 6173 6574 7229  taset..Datasetr)
-00002080: 0000 00da 0369 6e74 7202 0000 00da 064d  .....intr......M
+00002070: 7461 7365 74da 0744 6174 6173 6574 7227  taset..Datasetr'
+00002080: 0000 00da 0369 6e74 7202 0000 005a 064d  .....intr....Z.M
 00002090: 6f64 756c 65da 046c 6973 74da 0462 6f6f  odule..list..boo
-000020a0: 6c72 3500 0000 7203 0000 0072 3f00 0000  lr5...r....r?...
-000020b0: 725e 0000 0072 1f00 0000 721f 0000 0072  r^...r....r....r
+000020a0: 6c72 3300 0000 7203 0000 0072 3c00 0000  lr3...r....r<...
+000020b0: 725a 0000 0072 1f00 0000 721f 0000 0072  rZ...r....r....r
 000020c0: 1f00 0000 7220 0000 0072 1400 0000 1500  ....r ...r......
 000020d0: 0000 7354 0000 0008 0004 0102 0602 0102  ..sT............
 000020e0: ff02 020a fe02 2402 0102 ff06 0202 fe02  ......$.........
 000020f0: 030a fd02 1c04 fd02 0102 ff12 0202 fe02  ................
 00002100: 0302 fd08 040a fc02 2806 0102 ff08 0202  ........(.......
 00002110: fe08 0306 0104 ff02 fd06 050a fb02 2708  ..............'.
 00002120: 0106 0104 ff02 ff02 020e fe72 1400 0000  ...........r....
-00002130: 291f 7263 0000 0072 2c00 0000 da06 7479  ).rc...r,.....ty
+00002130: 291f 725f 0000 0072 2a00 0000 da06 7479  ).r_...r*.....ty
 00002140: 7069 6e67 7202 0000 005a 2861 736f 6369  pingr....Z(asoci
 00002150: 6974 612e 636f 6d70 6f6e 656e 7473 2e6e  ita.components.n
 00002160: 6f64 6573 2e66 6564 6572 6174 6564 5f6e  odes.federated_n
 00002170: 6f64 6572 0300 0000 5a27 6173 6f63 6969  oder....Z'asocii
 00002180: 7461 2e6d 6f64 656c 732e 7079 746f 7263  ta.models.pytorc
 00002190: 682e 6665 6465 7261 7465 645f 6d6f 6465  h.federated_mode
 000021a0: 6c72 0400 0000 da1b 6173 6f63 6969 7461  lr......asociita
@@ -546,16 +546,16 @@
 00002210: 0000 0072 0a00 0000 da2c 6173 6f63 6969  ...r.....,asocii
 00002220: 7461 2e63 6f6d 706f 6e65 6e74 732e 6172  ta.components.ar
 00002230: 6368 6976 6572 2e61 7263 6869 7665 5f6d  chiver.archive_m
 00002240: 616e 6167 6572 720b 0000 00da 2561 736f  anagerr.....%aso
 00002250: 6369 6974 612e 636f 6d70 6f6e 656e 7473  ciita.components
 00002260: 2e73 6574 7469 6e67 732e 7365 7474 696e  .settings.settin
 00002270: 6773 720c 0000 00da 0f6d 756c 7469 7072  gsr......multipr
-00002280: 6f63 6573 7369 6e67 720d 0000 00da 0574  ocessingr......t
-00002290: 6f72 6368 720e 0000 00da 1761 736f 6369  orchr......asoci
+00002280: 6f63 6573 7369 6e67 720d 0000 005a 0574  ocessingr....Z.t
+00002290: 6f72 6368 720e 0000 005a 1761 736f 6369  orchr....Z.asoci
 000022a0: 6974 612e 7574 696c 732e 6465 6275 6767  ita.utils.debugg
 000022b0: 6572 720f 0000 00da 1661 736f 6369 6974  err......asociit
 000022c0: 612e 7574 696c 732e 6865 6c70 6572 7372  a.utils.helpersr
 000022d0: 1000 0000 7211 0000 0072 1400 0000 721f  ....r....r....r.
 000022e0: 0000 0072 1f00 0000 721f 0000 0072 2000  ...r....r....r .
 000022f0: 0000 da08 3c6d 6f64 756c 653e 0100 0000  ....<module>....
 00002300: 7322 0000 0008 0008 010c 010c 010c 010c  s"..............
```

### Comparing `asociita-0.3.2/asociita/components/orchestrator/evaluator_orchestrator.py` & `asociita-0.3.3/asociita/components/orchestrator/evaluator_orchestrator.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         It connects the nodes, maintain the knowledge about their state and manages the
         multithread pool. Evaluator orchestrator is a child class of the Generic Orchestrator.
         Unlike its parent, Evaluator performs a training using Federated Optimization
         - pseudo-gradients from the models and momentum. Additionally, Evaluator Orchestrator
         is able to assess clients marginal contribution with the help of Evaluation Manager."""
     
     
-    def __init__(self, settings: Settings) -> None:
+    def __init__(self, settings: Settings, **kwargs) -> None:
         """Orchestrator is initialized by passing an instance
         of the Settings object. Settings object contains all the relevant configurational
         settings that an instance of the Orchestrator object may need to complete the simulation.
         Evaluator Orchestrator additionaly requires a configurations passed to the Optimizer 
         and Evaluator Manager upon its initialization.
         
         Parameters
@@ -40,15 +40,15 @@
             The Evaluator Orchestrator additionaly requires the passed object to contain a 
             configuration for the Optimizer and the Evaluation Manager.
        
        Returns
        -------
        None
         """
-        super().__init__(settings)
+        super().__init__(settings, kwargs=kwargs)
     
 
     def train_protocol(self,
                 nodes_data: list[datasets.arrow_dataset.Dataset, 
                 datasets.arrow_dataset.Dataset]) -> None:
         """"Performs a full federated training according to the initialized
         settings. The train_protocol of the orchestrator.evaluator_orchestrator
```

### Comparing `asociita-0.3.2/asociita/components/orchestrator/fedopt_orchestrator.py` & `asociita-0.3.3/asociita/components/orchestrator/fedopt_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/orchestrator/generic_orchestrator.py` & `asociita-0.3.3/asociita/components/orchestrator/generic_orchestrator.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/settings/__pycache__/evaluator_settings.cpython-310.pyc` & `asociita-0.3.3/asociita/components/settings/__pycache__/evaluator_settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/settings/__pycache__/fedopt_settings.cpython-310.pyc` & `asociita-0.3.3/asociita/components/settings/__pycache__/fedopt_settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/settings/__pycache__/init_settings.cpython-310.pyc` & `asociita-0.3.3/asociita/components/settings/__pycache__/init_settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/settings/__pycache__/settings.cpython-310.pyc` & `asociita-0.3.3/asociita/components/settings/__pycache__/settings.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/settings/evaluator_settings.py` & `asociita-0.3.3/asociita/components/settings/evaluator_settings.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/settings/fedopt_settings.py` & `asociita-0.3.3/asociita/components/settings/fedopt_settings.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/settings/init_settings.py` & `asociita-0.3.3/asociita/components/settings/init_settings.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/components/settings/settings.py` & `asociita-0.3.3/asociita/components/settings/settings.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/datasets/__pycache__/fetch_data.cpython-310.pyc` & `asociita-0.3.3/asociita/datasets/__pycache__/fetch_data.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/datasets/__pycache__/load_cifar.cpython-310.pyc` & `asociita-0.3.3/asociita/datasets/__pycache__/load_cifar.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/datasets/__pycache__/load_fmnist.cpython-310.pyc` & `asociita-0.3.3/asociita/datasets/__pycache__/load_fmnist.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/datasets/__pycache__/load_mnist.cpython-310.pyc` & `asociita-0.3.3/asociita/datasets/__pycache__/load_mnist.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/datasets/__pycache__/save_blueprint.cpython-310.pyc` & `asociita-0.3.3/asociita/datasets/__pycache__/save_blueprint.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/datasets/__pycache__/shard_splits.cpython-310.pyc` & `asociita-0.3.3/asociita/datasets/__pycache__/shard_splits.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/datasets/__pycache__/shard_transformation.cpython-310.pyc` & `asociita-0.3.3/asociita/datasets/__pycache__/shard_transformation.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/datasets/fetch_data.py` & `asociita-0.3.3/asociita/datasets/fetch_data.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/datasets/load_cifar.py` & `asociita-0.3.3/asociita/datasets/load_cifar.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/datasets/load_fmnist.py` & `asociita-0.3.3/asociita/datasets/load_fmnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/datasets/load_mnist.py` & `asociita-0.3.3/asociita/datasets/load_mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/datasets/save_blueprint.py` & `asociita-0.3.3/asociita/datasets/save_blueprint.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/datasets/shard_splits.py` & `asociita-0.3.3/asociita/datasets/shard_splits.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/datasets/shard_transformation.py` & `asociita-0.3.3/asociita/datasets/shard_transformation.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/exceptions/__pycache__/evaluatorexception.cpython-310.pyc` & `asociita-0.3.3/asociita/exceptions/__pycache__/evaluatorexception.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/exceptions/__pycache__/settingexception.cpython-310.pyc` & `asociita-0.3.3/asociita/exceptions/__pycache__/settingexception.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/models/pytorch/__pycache__/cifar10.cpython-310.pyc` & `asociita-0.3.3/asociita/models/pytorch/__pycache__/cifar10.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/models/pytorch/__pycache__/federated_model.cpython-310.pyc` & `asociita-0.3.3/asociita/models/pytorch/__pycache__/federated_model.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 13 09:54:08 2023 UTC, .py size: 17178 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 c0c9 af64 1a43 0000  o..........d.C..
+00000000: 6f0d 0d0a 0000 0000 baf1 b364 1a43 0000  o..........d.C..
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 c600 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 6400 6401 6c01 5a01 6400  d.l.Z.d.d.l.Z.d.
 00000040: 6401 6c02 5a03 6400 6402 6c04 6d05 5a05  d.l.Z.d.d.l.m.Z.
 00000050: 0100 6400 6403 6c06 6d07 5a07 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6404 6c06 6d08 5a08 0100 6400 6405 6c09  d.l.m.Z...d.d.l.
 00000070: 6d0a 5a0a 6d0b 5a0b 6d0c 5a0c 6d0d 5a0d  m.Z.m.Z.m.Z.m.Z.
```

### Comparing `asociita-0.3.2/asociita/models/pytorch/__pycache__/fmnist.cpython-310.pyc` & `asociita-0.3.3/asociita/models/pytorch/__pycache__/fmnist.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/models/pytorch/__pycache__/mnist.cpython-310.pyc` & `asociita-0.3.3/asociita/models/pytorch/__pycache__/mnist.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/models/pytorch/cifar10.py` & `asociita-0.3.3/asociita/models/pytorch/cifar10.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/models/pytorch/federated_model.py` & `asociita-0.3.3/asociita/models/pytorch/federated_model.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/models/pytorch/mnist.py` & `asociita-0.3.3/asociita/models/pytorch/mnist.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/__pycache__/computations.cpython-310.pyc` & `asociita-0.3.3/asociita/utils/__pycache__/computations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/__pycache__/custom_transformations.cpython-310.pyc` & `asociita-0.3.3/asociita/utils/__pycache__/custom_transformations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/__pycache__/debugger.cpython-310.pyc` & `asociita-0.3.3/asociita/utils/__pycache__/debugger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/__pycache__/handlers.cpython-310.pyc` & `asociita-0.3.3/asociita/utils/__pycache__/handlers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/__pycache__/helpers.cpython-310.pyc` & `asociita-0.3.3/asociita/utils/__pycache__/helpers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/__pycache__/loggers.cpython-310.pyc` & `asociita-0.3.3/asociita/utils/__pycache__/loggers.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Thu Jul 13 09:58:47 2023 UTC, .py size: 1640 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 21% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 d7ca af64 6806 0000  o..........dh...
+00000000: 6f0d 0d0a 0000 0000 baf1 b364 6806 0000  o..........dh...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0003 0000 0040 0000 0073 1a00 0000 6400  .....@...s....d.
 00000030: 6401 6c00 5a00 4700 6402 6403 8400 6403  d.l.Z.G.d.d...d.
 00000040: 8302 5a01 6401 5300 2904 e900 0000 004e  ..Z.d.S.)......N
 00000050: 6300 0000 0000 0000 0000 0000 0000 0000  c...............
 00000060: 0003 0000 0040 0000 0073 3000 0000 6500  .....@...s0...e.
 00000070: 5a01 6400 5a02 6503 6401 6402 8400 8301  Z.d.Z.e.d.d.....
```

### Comparing `asociita-0.3.2/asociita/utils/__pycache__/optimizers.cpython-310.pyc` & `asociita-0.3.3/asociita/utils/__pycache__/optimizers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/__pycache__/orchestrations.cpython-310.pyc` & `asociita-0.3.3/asociita/utils/__pycache__/orchestrations.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/__pycache__/showcase.cpython-310.pyc` & `asociita-0.3.3/asociita/utils/__pycache__/showcase.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/computations.py` & `asociita-0.3.3/asociita/utils/computations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/custom_transformations.py` & `asociita-0.3.3/asociita/utils/custom_transformations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/debugger.py` & `asociita-0.3.3/asociita/utils/debugger.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/handlers.py` & `asociita-0.3.3/asociita/utils/handlers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/helpers.py` & `asociita-0.3.3/asociita/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/loggers.py` & `asociita-0.3.3/asociita/utils/loggers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/optimizers.py` & `asociita-0.3.3/asociita/utils/optimizers.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/orchestrations.py` & `asociita-0.3.3/asociita/utils/orchestrations.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/asociita/utils/showcase.py` & `asociita-0.3.3/asociita/utils/showcase.py`

 * *Files identical despite different names*

### Comparing `asociita-0.3.2/pyproject.toml` & `asociita-0.3.3/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "asociita"
-version = "0.3.2"
+version = "0.3.3"
 description = "An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting."
 authors = ["Maciej Zuziak <maciejkrzysztof.zuziak@isti.cnr.it>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/Scolpe/Asociita"
 repository = "https://github.com/Scolpe/Asociita"
```

### Comparing `asociita-0.3.2/PKG-INFO` & `asociita-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: asociita
-Version: 0.3.2
+Version: 0.3.3
 Summary: An intuitive and modular simulator for assessing the marginal value of a client's contribution in a decentralized setting.
 Home-page: https://github.com/Scolpe/Asociita
 License: MIT
 Author: Maciej Zuziak
 Author-email: maciejkrzysztof.zuziak@isti.cnr.it
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

