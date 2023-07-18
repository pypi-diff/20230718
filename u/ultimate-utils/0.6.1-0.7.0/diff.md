# Comparing `tmp/ultimate-utils-0.6.1.tar.gz` & `tmp/ultimate-utils-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultimate-utils-0.6.1.tar", last modified: Wed Aug 17 19:02:02 2022, max compression
+gzip compressed data, was "ultimate-utils-0.7.0.tar", last modified: Tue Jul 18 01:51:31 2023, max compression
```

## Comparing `ultimate-utils-0.6.1.tar` & `ultimate-utils-0.7.0.tar`

### file list

```diff
@@ -1,139 +1,411 @@
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.551937 ultimate-utils-0.6.1/
--rw-r--r--   0 brandomiranda   (501) staff       (20)     1065 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/LICENSE
--rw-r--r--   0 brandomiranda   (501) staff       (20)     6708 2022-08-17 19:02:02.551647 ultimate-utils-0.6.1/PKG-INFO
--rw-r--r--   0 brandomiranda   (501) staff       (20)     6347 2022-08-17 19:01:41.000000 ultimate-utils-0.6.1/README.md
--rw-r--r--   0 brandomiranda   (501) staff       (20)       38 2022-08-17 19:02:02.552038 ultimate-utils-0.6.1/setup.cfg
--rw-r--r--   0 brandomiranda   (501) staff       (20)     3193 2022-08-17 18:54:12.000000 ultimate-utils-0.6.1/setup.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.510959 ultimate-utils-0.6.1/ultimate-utils-proj-src/
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.517437 ultimate-utils-0.6.1/ultimate-utils-proj-src/ultimate_utils.egg-info/
--rw-r--r--   0 brandomiranda   (501) staff       (20)     6708 2022-08-17 19:02:01.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/ultimate_utils.egg-info/PKG-INFO
--rw-r--r--   0 brandomiranda   (501) staff       (20)     7310 2022-08-17 19:02:02.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/ultimate_utils.egg-info/SOURCES.txt
--rw-r--r--   0 brandomiranda   (501) staff       (20)        1 2022-08-17 19:02:02.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/ultimate_utils.egg-info/dependency_links.txt
--rw-r--r--   0 brandomiranda   (501) staff       (20)      190 2022-08-17 19:02:02.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/ultimate_utils.egg-info/requires.txt
--rw-r--r--   0 brandomiranda   (501) staff       (20)        7 2022-08-17 19:02:02.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/ultimate_utils.egg-info/top_level.txt
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.518766 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/
--rw-r--r--   0 brandomiranda   (501) staff       (20)    61504 2022-08-16 14:48:26.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/__init__.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.520302 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/argparse_uu/
--rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/argparse_uu/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     3694 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/argparse_uu/args_tinfer.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    11409 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/argparse_uu/common.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    13518 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/argparse_uu/meta_learning.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    13401 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/argparse_uu/supervised_learning.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     6510 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/emailing.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    14486 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/logger.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.520607 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/logging_uu/
--rw-r--r--   0 brandomiranda   (501) staff       (20)     1119 2022-06-20 17:57:14.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/logging_uu/__init__.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.521769 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/logging_uu/wandb_logging/
--rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/logging_uu/wandb_logging/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     2744 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/logging_uu/wandb_logging/common.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     6100 2022-08-16 13:55:38.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/logging_uu/wandb_logging/meta_learning.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     5321 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/logging_uu/wandb_logging/supervised_learning.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.522461 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/plot/
--rw-r--r--   0 brandomiranda   (501) staff       (20)    42820 2022-06-09 15:17:00.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/plot/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     1438 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/plot/image_visualization.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     6098 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/stats_collector_mit.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.523938 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/
--rw-r--r--   0 brandomiranda   (501) staff       (20)   122949 2022-06-14 18:59:19.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/__init__.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.525478 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/agents/
--rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/agents/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)      112 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/agents/common.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     5336 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/agents/supervised_learning.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    20759 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/agents/synth_agents.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    12365 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/agents/tactic_predictor_tactician_agent.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.526452 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/checkpointing_uu/
--rw-r--r--   0 brandomiranda   (501) staff       (20)      882 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/checkpointing_uu/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     8230 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/checkpointing_uu/meta_learning.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     4313 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/checkpointing_uu/supervised_learning.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.527953 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/data_uu/
--rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/data_uu/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     5160 2022-08-15 16:00:23.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_data_preprocessing.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     8509 2022-08-10 23:04:55.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_dataset.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     7949 2022-08-11 16:31:18.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_tokenizer.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     2432 2022-08-10 15:06:22.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_trainer.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.532290 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/
--rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     7724 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/cifar100.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    25079 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/cifar100fs_fc100.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     9018 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/common.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     8539 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/data_loader_cifar.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     3690 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/download_coqgym_dataset.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     3704 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/download_miniimagenet.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     4169 2022-06-15 19:42:57.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/helpers.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     5480 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/indexable_l2l_task_dataset.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.536095 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/
--rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/common.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     6833 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/dataset_based_few_shot_learning_l2l_loader.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    18288 2022-06-09 15:17:00.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/gaussian_1d_tasksets.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    13149 2022-06-15 19:42:57.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/gaussian_nd_tasksets.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     2341 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/helpers.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     9346 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/l2l_mini_imagenet_mi.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     8060 2022-06-15 19:42:57.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/l2l_ml_tasksets.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     7764 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/l2l_to_torchmeta_dataloader.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    13058 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/rfs_meta_learning_data_loaders.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    25658 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/torchmeta_ml_dataloaders.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     3243 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/transforms_cfg_rfs.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    17599 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_lstm_dataloader.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    13277 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/miniimagenet_rfs.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     7370 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/mnist.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     3690 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/unzip_coqgym_dataset.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.536652 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataset/
--rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataset/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     8205 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataset/rfs_mini_imagenet.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.536952 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dgl_uu/
--rw-r--r--   0 brandomiranda   (501) staff       (20)       91 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dgl_uu/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    29222 2022-06-16 13:43:07.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/distributed.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.538129 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/eval/
--rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/eval/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     8149 2022-06-09 15:17:00.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/eval/eval.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     8536 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/eval/my_eval_fewshot_rfs.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     8213 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/eval/my_meta_eval_rfs.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.539941 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/mains/
--rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/mains/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    12512 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/mains/common.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    21296 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/mains/main_meta_learning.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     5514 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/mains/main_sl_with_ddp.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    10507 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/mains/main_synth.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    13592 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/mains/main_tree_nn.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.541522 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/
--rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    27192 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/maml_differentiable_optimizer.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    17973 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/maml_meta_learner.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    15357 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/meta_lstm_meta_learner.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    15019 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/pretrain_convergence.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.542385 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/metrics/
--rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/metrics/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    11556 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/metrics/confidence_intervals.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     6556 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/metrics/metrics.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     9495 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/mit_trainer_code.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.546562 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/
--rw-r--r--   0 brandomiranda   (501) staff       (20)    11212 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    16744 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/custom_layers.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     4454 2022-06-15 19:42:57.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/fullyconnected.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     3464 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/hbf.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.547207 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/hf_uu/
--rw-r--r--   0 brandomiranda   (501) staff       (20)     4259 2022-08-15 16:23:07.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/hf_uu/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)      372 2022-08-11 18:38:50.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/hf_uu/t5_uu.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     5293 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/kcnn.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     5077 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/l2l_models.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    10821 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/learner_from_opt_as_few_shot_paper.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    16820 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/mit_nn_models.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     1945 2022-06-09 15:17:00.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/probe_networks.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    20677 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/resnet_rfs.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     3182 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/rfs_convnet.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     1391 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/spp.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.549378 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/
--rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     8939 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/adafactor_uu.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     2473 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/adam_uu.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)      764 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/common.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)      292 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/optimizers.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     3117 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/sgd_uu.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     4785 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/tensorboard.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.549701 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/torch_geometric/
--rw-r--r--   0 brandomiranda   (501) staff       (20)      902 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/torch_geometric/__init__.py
-drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2022-08-17 19:02:02.550997 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/training/
--rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/training/__init__.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     8716 2022-06-03 15:04:27.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/training/common.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)    10143 2022-07-14 18:27:25.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/training/meta_training.py
--rw-r--r--   0 brandomiranda   (501) staff       (20)     8976 2022-06-15 19:42:57.000000 ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/training/supervised_learning.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.521300 ultimate-utils-0.7.0/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4127 2022-09-07 20:32:28.000000 ultimate-utils-0.7.0/.gitignore
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1077 2022-09-15 18:43:30.000000 ultimate-utils-0.7.0/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1065 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/LICENSE
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    26981 2023-07-18 01:51:31.521103 ultimate-utils-0.7.0/PKG-INFO
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    26639 2023-07-11 18:15:50.000000 ultimate-utils-0.7.0/README.md
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.466072 ultimate-utils-0.7.0/docker_files_ repo/
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.465997 ultimate-utils-0.7.0/docker_files_ repo/docker_files/
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.474428 ultimate-utils-0.7.0/docker_files_ repo/docker_files/runtime/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1833 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files/runtime/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)       50 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files/runtime/container_setup.sh
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      849 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files/runtime/fake_gui.sh
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.474555 ultimate-utils-0.7.0/docker_files_ repo/docker_files/test_pytorch/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      973 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files/test_pytorch/Dockerfile
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.474964 ultimate-utils-0.7.0/docker_files_ repo/docker_files/tf_gpu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      907 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files/tf_gpu/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      140 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files/tf_gpu/batch_main.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      531 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files/tf_gpu/container_setup.sh
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.475114 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.475651 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/dgx1_tf/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      843 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/dgx1_tf/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      437 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/dgx1_tf/Dockerfile_old
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      628 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/dgx1_tf/Dockerfile_tf10
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      230 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/dgx1_tf/test.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.476050 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/dgx1_torch/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      247 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/dgx1_torch/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      589 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/dgx1_torch/run_torch_test.txt
+-rw-r--r--   0 brandomiranda   (501) staff       (20)       84 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/dgx1_torch/test.lua
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.476180 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/echo_hello/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)       22 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/echo_hello/hello.sh
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      103 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/run_cpu_matrix_mul_text.sh
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.476569 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf10_cpu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1464 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf10_cpu/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      140 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf10_cpu/batch_main.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      531 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf10_cpu/container_setup.sh
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.476853 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf10_gpu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1055 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf10_gpu/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1055 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf10_gpu/Dockerfile_old
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.477244 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      872 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      140 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu/batch_main.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      531 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu/container_setup.sh
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.477627 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu_anaconda/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      722 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu_anaconda/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      140 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu_anaconda/batch_main.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      530 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu_anaconda/container_setup.sh
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.477908 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu_no_entry/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1208 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu_no_entry/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      140 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu_no_entry/print_args.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.478316 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu_py3.4/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      947 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu_py3.4/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      140 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu_py3.4/batch_main.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      530 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu_py3.4/container_setup.sh
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.478807 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu_py3.5/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1309 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu_py3.5/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      140 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu_py3.5/batch_main.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      531 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_cpu_py3.5/container_setup.sh
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.479205 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      907 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      140 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu/batch_main.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      531 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu/container_setup.sh
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.479615 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_anaconda/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      726 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_anaconda/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      140 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_anaconda/batch_main.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      530 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_anaconda/container_setup.sh
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.480035 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_nightly/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      885 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_nightly/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      140 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_nightly/batch_main.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      530 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_nightly/container_setup.sh
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.480463 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_py3.4/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      955 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_py3.4/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      140 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_py3.4/batch_main.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      530 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_py3.4/container_setup.sh
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.480869 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_tf1/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      892 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_tf1/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      140 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_tf1/batch_main.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      530 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/tf_gpu_tf1/container_setup.sh
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.481655 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/vim_img/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      163 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/vim_img/Dockerfile
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3807 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/vim_img/bashrc_dgx1
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1051 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/vim_img/bashrc_local
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      399 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/vim_img/cvim
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     2310 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/vim_img/pvim.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      419 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/vim_img/unit_test_pvim.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.481789 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/volumes_test/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      307 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/volumes_test/Dockerfile
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.481923 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/volumes_test/folder/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)       18 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/docker_files_ repo/docker_files_examples/volumes_test/folder/hello_world.txt
+-rw-r--r--   0 brandomiranda   (501) staff       (20)       38 2023-07-18 01:51:31.521345 ultimate-utils-0.7.0/setup.cfg
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3438 2023-07-18 01:50:40.000000 ultimate-utils-0.7.0/setup.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.482833 ultimate-utils-0.7.0/sh_files_repo/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      323 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/sh_files_repo/interactive.sub
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1759 2022-05-12 22:10:38.000000 ultimate-utils-0.7.0/sh_files_repo/job.sub
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     8377 2022-11-16 02:49:12.000000 ultimate-utils-0.7.0/sh_files_repo/main.sh
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      833 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/sh_files_repo/main_vision.sh
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      645 2022-11-09 23:02:04.000000 ultimate-utils-0.7.0/sh_files_repo/run_expt.sh
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      988 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/sh_files_repo/run_tb.sh
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4308 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/sh_files_repo/setup_new_vm.sh
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.484006 ultimate-utils-0.7.0/tutorials_for_myself/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2021-12-09 18:57:56.000000 ultimate-utils-0.7.0/tutorials_for_myself/__init__.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.484651 ultimate-utils-0.7.0/tutorials_for_myself/anatome_pg/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3832 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/anatome_pg/original_anatome_hypothesis_testing.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     5040 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/anatome_pg/original_anatome_pg.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     7538 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/anatome_pg/sanity_checks_original_anatome.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      484 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/cat_vs_stack_pytorch.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.484783 ultimate-utils-0.7.0/tutorials_for_myself/cca/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      934 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/cca/pwcca4cnns.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.485208 ultimate-utils-0.7.0/tutorials_for_myself/concurrency/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1215 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/concurrency/generator_example.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     2236 2022-06-15 22:34:18.000000 ultimate-utils-0.7.0/tutorials_for_myself/concurrency/synchronous.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      486 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/concurrency/trio_example.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      855 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/dataclass.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     5342 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/docker_tutorial.md
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      505 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/example_msg.capnp
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      430 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/forced_named_arguments_start_in_the_middle.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     5055 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/modules_in_python_bmg.md
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.485613 ultimate-utils-0.7.0/tutorials_for_myself/my_learn2learn/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     6156 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/my_learn2learn/l2l_maml_miniimagenet.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4756 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/my_learn2learn/learn2learn_cherry_distributed.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4746 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/my_learn2learn/learn2learn_ddp.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.485755 ultimate-utils-0.7.0/tutorials_for_myself/my_pyplot/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3468 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/my_pyplot/my_custom_error_bands.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.485892 ultimate-utils-0.7.0/tutorials_for_myself/my_pytorch/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      149 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/my_pytorch/ddp.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.486169 ultimate-utils-0.7.0/tutorials_for_myself/my_pytorch/transformers_pytorch/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     7263 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/my_pytorch/transformers_pytorch/transformer_notes.md
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    16444 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/my_pytorch/transformers_pytorch/transformer_pytorch_tutorial.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.486322 ultimate-utils-0.7.0/tutorials_for_myself/my_seaborn/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     6933 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/my_seaborn/seaborn_error_bands.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.486451 ultimate-utils-0.7.0/tutorials_for_myself/my_sklearn/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1674 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/my_sklearn/logistic_regression_get_weights.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.486587 ultimate-utils-0.7.0/tutorials_for_myself/my_torchmeta/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4550 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/my_torchmeta/torchmeta_ddp.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.486715 ultimate-utils-0.7.0/tutorials_for_myself/oop_python/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     2263 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/oop_python/simple_super.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.487092 ultimate-utils-0.7.0/tutorials_for_myself/packaging_project/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2021-12-09 18:57:56.000000 ultimate-utils-0.7.0/tutorials_for_myself/packaging_project/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      270 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/packaging_project/module_sys_path.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.487717 ultimate-utils-0.7.0/tutorials_for_myself/packaging_project/pkg1/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      214 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/packaging_project/pkg1/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      151 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/packaging_project/pkg1/imported_module.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      147 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/packaging_project/pkg1/imported_module_by_front_dot.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      164 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/packaging_project/pkg1/module.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      524 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/packaging_project/setup.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3591 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/progressbar2.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.487871 ultimate-utils-0.7.0/tutorials_for_myself/pushing_to_pypi/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    10052 2022-09-07 20:32:28.000000 ultimate-utils-0.7.0/tutorials_for_myself/pushing_to_pypi/README.md
+-rw-r--r--   0 brandomiranda   (501) staff       (20)   339003 2023-02-10 04:02:18.000000 ultimate-utils-0.7.0/tutorials_for_myself/python_pg1.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.488157 ultimate-utils-0.7.0/tutorials_for_myself/remote-pycharm-project-test/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2021-12-09 19:13:28.000000 ultimate-utils-0.7.0/tutorials_for_myself/remote-pycharm-project-test/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      955 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/tutorials_for_myself/remote-pycharm-project-test/solver.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.488313 ultimate-utils-0.7.0/ultimate-utils-proj-src/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4130 2021-12-24 22:43:55.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/execute_tensorboard.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.489109 ultimate-utils-0.7.0/ultimate-utils-proj-src/ultimate_utils.egg-info/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    26981 2023-07-18 01:51:31.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/ultimate_utils.egg-info/PKG-INFO
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    19833 2023-07-18 01:51:31.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/ultimate_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        1 2023-07-18 01:51:31.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/ultimate_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      171 2023-07-18 01:51:31.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/ultimate_utils.egg-info/requires.txt
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        7 2023-07-18 01:51:31.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/ultimate_utils.egg-info/top_level.txt
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.489706 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    75434 2023-07-13 00:19:53.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/__init__.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.490403 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/argparse_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2021-12-16 23:51:38.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/argparse_uu/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3694 2021-12-14 19:05:18.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/argparse_uu/args_tinfer.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    15236 2023-07-05 18:16:39.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/argparse_uu/common.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    34207 2023-05-16 18:05:38.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/argparse_uu/meta_learning.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    20986 2023-03-16 19:20:24.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/argparse_uu/supervised_learning.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     6510 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/emailing.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.490673 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-06-28 02:07:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     6737 2023-07-13 00:31:15.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/common.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.490920 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/data_hf/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-07-06 01:01:01.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/data_hf/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1547 2023-07-06 01:10:43.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/data_hf/common.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.491580 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/hf_argparse/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-06-29 00:45:33.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/hf_argparse/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     7172 2023-06-29 00:50:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/hf_argparse/args_alpaca.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4036 2023-06-29 00:48:06.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/hf_argparse/args_alpaca_farm.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     6227 2023-07-13 01:41:39.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/hf_argparse/common.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     6058 2023-07-12 23:38:56.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/hf_argparse/falcon_uu_training_args.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.491727 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/inference_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-06-28 19:50:57.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/inference_uu/__init__.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.491840 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/mains_hf/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-07-06 00:10:18.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/mains_hf/__init__.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.492062 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/mains_hf/falcon_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-07-06 00:10:27.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/mains_hf/falcon_uu/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3891 2023-07-13 01:41:39.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/mains_hf/falcon_uu/main_falcon_uu.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.492840 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/model_tokenizer/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-06-28 19:42:16.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/model_tokenizer/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3186 2023-06-28 22:24:51.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/model_tokenizer/alpaca_uu.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1717 2023-07-18 00:37:13.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/model_tokenizer/camel_hf_uu.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     5065 2023-07-11 20:00:47.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/model_tokenizer/falcon_guanaco.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    14849 2023-07-13 00:44:37.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/model_tokenizer/falcon_uu_mdl_tok.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1018 2023-07-07 19:51:11.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/model_tokenizer/init_new_token_in_model.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.493961 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/train/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-06-29 21:33:23.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/train/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     6798 2023-06-30 01:04:47.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/train/common.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3178 2023-07-13 00:31:42.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/train/full_fine_tuning.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.494689 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/train/sft/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-06-30 01:21:17.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/train/sft/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3795 2023-07-12 17:23:37.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/train/sft/falcon_lambda_labs.py
+-rw-rw-r--   0 brandomiranda   (501) staff       (20)     7879 2023-06-01 22:26:16.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/train/sft/falcon_peft.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3069 2023-07-12 01:10:18.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/train/sft/qlora_ft.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-07-06 00:49:14.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/train/train_causal.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-07-06 00:48:53.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/hf_uu/train/train_seq2seq.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.495316 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/jax_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-06-30 22:56:33.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/jax_uu/__init__.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.497313 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/jax_uu/models/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-03-05 02:53:10.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/jax_uu/models/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)       97 2023-03-05 17:51:18.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/jax_uu/models/flash_attn.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      215 2023-03-10 22:52:06.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/jax_uu/models/layer_norm_autoregressive.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     9802 2023-03-06 18:04:54.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/jax_uu/models/mha_simple.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    17765 2023-03-02 23:34:35.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/logger.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.497486 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/logging_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1119 2022-07-12 23:03:30.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/logging_uu/__init__.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.497877 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/logging_uu/wandb_logging/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2021-12-16 19:27:19.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/logging_uu/wandb_logging/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     9749 2023-06-29 22:06:17.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/logging_uu/wandb_logging/common.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    19929 2023-03-22 18:53:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/logging_uu/wandb_logging/supervised_learning.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.498264 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/numpy_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-11-26 18:16:02.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/numpy_uu/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3944 2023-01-28 03:16:44.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/numpy_uu/common.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.498814 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/plot/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    42769 2023-02-02 19:44:56.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/plot/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    12323 2023-01-20 03:36:00.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/plot/histograms_uu.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     8062 2022-11-17 23:56:47.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/plot/image_visualization.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     6098 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_collector_mit.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.499529 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-01-13 04:57:30.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/__init__.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.499782 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/anova_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-01-30 18:12:49.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/anova_uu/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     9672 2023-01-30 19:21:33.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/anova_uu/anova.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)       59 2023-01-28 03:16:43.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/ci_uu.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    19385 2023-02-10 00:40:22.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/effect_size.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.499921 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/eps_none_zero_hypothesis_testing_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-01-24 19:55:31.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/eps_none_zero_hypothesis_testing_uu/__init__.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.500042 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/lrt_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-01-24 19:55:08.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/lrt_uu/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4236 2023-02-09 22:55:27.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/overfitting.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.500550 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/p_values_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-01-18 04:20:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/p_values_uu/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      632 2023-01-18 04:32:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/p_values_uu/common.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3933 2023-02-09 02:44:48.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/p_values_uu/t_test_uu.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1512 2023-01-18 19:52:58.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/p_values_uu/z_test_uu.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     6200 2023-01-25 02:19:49.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/power.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.500805 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/regression_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-01-26 19:17:05.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/regression_uu/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     2037 2023-01-30 18:24:28.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_uu/regression_uu/r2.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.500949 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/theorem_proving/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-06-22 18:11:23.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/theorem_proving/__init__.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.501070 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/theorem_proving/isabelle/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-06-22 18:11:15.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/theorem_proving/isabelle/__init__.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.501701 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)   127460 2023-07-11 01:53:36.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/__init__.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.502507 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/agents/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2021-12-16 22:16:11.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/agents/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      112 2021-12-17 23:29:33.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/agents/common.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1348 2021-12-14 22:04:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/agents/readme.md
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     5372 2023-03-22 18:41:49.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/agents/supervised_learning.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    20759 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/agents/synth_agents.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    12365 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/agents/tactic_predictor_tactician_agent.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.502921 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/checkpointing_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      882 2022-01-17 23:10:04.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/checkpointing_uu/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     8230 2022-02-09 00:48:00.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/checkpointing_uu/meta_learning.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4543 2022-10-26 23:31:09.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/checkpointing_uu/supervised_learning.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.503579 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/data_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2021-12-13 19:38:28.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/data_uu/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     5160 2022-09-07 20:32:28.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_data_preprocessing.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     9335 2022-09-07 20:32:28.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_dataset.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     7949 2022-09-07 20:32:28.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_tokenizer.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     2432 2022-09-07 20:32:28.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_trainer.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.505309 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-01-20 19:53:35.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     8105 2022-09-27 18:39:45.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/cifar100.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    25079 2022-05-12 18:22:15.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/cifar100fs_fc100.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    13049 2023-01-30 18:55:07.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/common.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     8539 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/data_loader_cifar.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3690 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/download_coqgym_dataset.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3734 2022-11-04 00:17:11.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/download_miniimagenet.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    15433 2023-05-16 18:05:38.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/helpers.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.505569 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/mds_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-01-31 21:09:49.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/mds_uu/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1298 2023-01-31 21:10:00.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/mds_uu/common.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.508038 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-01-20 19:31:43.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4322 2023-02-05 00:57:26.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/aircraft_l2l.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4231 2023-01-19 23:00:34.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/cifarfs_l2l.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    21031 2023-04-07 16:43:53.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/delaunay_l2l.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4305 2023-02-05 00:57:26.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/flower_l2l.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    18288 2022-06-13 23:20:24.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/gaussian_1d_tasksets.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    13149 2022-06-15 22:34:18.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/gaussian_nd_tasksets.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3158 2023-04-07 16:43:53.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/helpers.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    24957 2023-05-16 18:05:38.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/l2l_ml_tasksets.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    17506 2023-03-24 22:15:57.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/l2l_to_torchmeta_dataloader.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    23136 2023-05-16 18:05:38.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/mds_l2l.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    13218 2023-01-19 23:00:34.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/mini_imagenet_mi_l2l.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    10000 2023-01-19 23:00:34.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/omniglot_l2l.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    13058 2022-03-03 00:18:20.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/rfs_meta_learning_data_loaders.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    26603 2023-03-01 22:26:05.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/torchmeta_ml_dataloaders.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3243 2022-03-01 20:02:03.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/transforms_cfg_rfs.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    17599 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_lstm_dataloader.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    13277 2022-02-10 20:52:11.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/miniimagenet_rfs.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     7370 2022-02-10 21:25:49.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/mnist.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3690 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/unzip_coqgym_dataset.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.509584 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/usl/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-01-20 21:44:33.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/usl/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    12367 2023-03-16 17:50:05.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/usl/usl_dataloaders.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    77611 2023-05-16 18:05:38.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/usl/usl_patricks_l2l.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     5356 2023-02-21 00:34:02.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/usl/usl_vggair.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.510431 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataset/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-03-01 20:05:22.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataset/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    31384 2023-02-06 22:37:37.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataset/concate_dataset.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    32396 2023-03-07 23:43:21.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataset/delaunay_uu.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     7576 2022-11-23 00:15:18.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataset/delauny_data_statistics_and_visualizations.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     8205 2022-03-02 22:03:06.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataset/rfs_mini_imagenet.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.510572 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dgl_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)       91 2022-09-07 20:32:28.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dgl_uu/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    32788 2023-03-20 23:34:49.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/distributed.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.511095 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/eval/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-01-17 22:10:53.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/eval/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3577 2023-03-22 18:04:59.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/eval/eval.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     8536 2022-03-01 19:27:13.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/eval/my_eval_fewshot_rfs.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     8213 2022-03-01 19:23:39.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/eval/my_meta_eval_rfs.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.511996 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/mains/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2021-12-16 21:26:15.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/mains/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    19355 2023-04-14 19:59:08.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/mains/common.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    21302 2023-01-27 00:34:34.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/mains/main_meta_learning.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     5514 2022-02-03 00:26:40.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/mains/main_sl_with_ddp.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    10507 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/mains/main_synth.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    13592 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/mains/main_tree_nn.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.513120 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2021-12-13 22:19:39.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    11323 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/license_higher.txt
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3206 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/license_pytorch.txt
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    29607 2023-01-28 03:17:43.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/maml_differentiable_optimizer.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    21527 2023-03-22 18:28:07.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/maml_meta_learner.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    15357 2022-01-21 18:45:59.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/meta_lstm_meta_learner.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      430 2022-01-21 18:18:24.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/notes_license.txt.md
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    16630 2023-03-23 01:20:35.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/pretrain_convergence.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.513750 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-01-21 18:04:18.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/__init__.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.514866 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/cca/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    11358 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/cca/LICENSE
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      206 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/cca/NOTICE
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    16395 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/cca/cca_core.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     6768 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/cca/dft_ccas.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1621 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/cca/numpy_pca.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4008 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/cca/numpy_pls.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4051 2023-01-28 03:17:58.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/cca/pwcca.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     2608 2023-01-28 03:17:58.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/cca/uutils_cca_core_addendums.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.515121 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/complexity/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-01-28 03:38:26.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/complexity/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4047 2023-02-07 22:12:50.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/complexity/task2vec_norm_complexity.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    21567 2023-02-09 02:12:45.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/confidence_intervals.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.515361 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/diversity/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2021-12-13 22:19:28.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/diversity/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    45568 2023-04-25 18:23:53.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/diversity/diversity.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.516348 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/diversity/task2vec_based_metrics/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2022-09-21 23:44:35.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/diversity/task2vec_based_metrics/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3256 2023-02-07 21:49:33.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/diversity/task2vec_based_metrics/models.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1778 2023-01-28 03:21:31.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/diversity/task2vec_based_metrics/small_datasets_example_from_task2vec.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    17754 2023-02-07 21:47:27.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/diversity/task2vec_based_metrics/task2vec.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     9483 2023-02-07 22:11:52.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/diversity/task2vec_based_metrics/task_similarity.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     2053 2021-12-08 23:39:18.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/diversity/task2vec_based_metrics/utils.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     5430 2021-12-08 23:39:18.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/diversity/task2vec_based_metrics/variational.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    41020 2023-04-25 18:26:17.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/main_task2vec_div_compute_vision.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     6556 2023-01-28 03:16:07.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/metrics.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     9495 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/mit_trainer_code.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.518114 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    11212 2022-02-09 23:01:40.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    16744 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/custom_layers.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4454 2022-06-15 22:34:18.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/fullyconnected.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3464 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/hbf.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.518501 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/hf_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4259 2022-09-07 20:32:28.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/hf_uu/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      372 2022-09-07 20:32:28.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/hf_uu/t5_uu.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    22361 2023-03-23 00:21:00.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/hf_uu/vit_uu.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     5293 2021-12-13 22:34:59.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/kcnn.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     5077 2022-03-28 22:50:43.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/l2l_models.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    10905 2022-10-31 20:51:10.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/learner_from_opt_as_few_shot_paper.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    11272 2023-04-25 18:25:42.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/linear_model_from_nn.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    16820 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/mit_nn_models.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     2959 2023-02-07 21:50:11.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/probe_networks.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    21242 2023-03-15 22:07:56.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/resnet_rfs.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3182 2022-01-31 19:37:28.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/rfs_convnet.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1391 2021-12-13 22:33:55.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/spp.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.519281 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     9035 2023-02-09 01:46:05.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/adafactor_uu.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     2473 2022-02-03 00:30:48.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/adam_uu.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      764 2021-12-19 20:37:27.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/common.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      292 2021-12-14 17:36:22.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/optimizers.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     3117 2022-02-18 17:59:00.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/sgd_uu.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.519889 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/scaling_laws/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-06-21 23:16:12.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/scaling_laws/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-06-21 23:41:34.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/scaling_laws/bnsl.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    13371 2023-06-27 03:15:18.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/scaling_laws/chinchilla.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1371 2023-06-21 23:47:14.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/scaling_laws/flops_estimations.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      575 2023-06-21 23:23:42.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/scaling_laws/llama.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     4738 2022-11-13 20:19:27.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/tensorboard.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.520018 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/torch_geometric/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)      902 2021-12-08 23:34:32.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/torch_geometric/__init__.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.520515 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/training/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2021-12-13 21:32:20.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/training/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    15598 2023-03-24 22:17:18.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/training/common.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)    11323 2023-03-22 18:04:59.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/training/meta_training.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     9073 2023-03-01 22:54:15.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/training/supervised_learning.py
+drwxr-xr-x   0 brandomiranda   (501) staff       (20)        0 2023-07-18 01:51:31.520874 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/wandb_uu/
+-rw-r--r--   0 brandomiranda   (501) staff       (20)        0 2023-06-29 22:01:09.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/wandb_uu/__init__.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     1437 2023-06-29 22:12:27.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/wandb_uu/common.py
+-rw-r--r--   0 brandomiranda   (501) staff       (20)     6909 2023-07-12 00:57:56.000000 ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/wandb_uu/sweeps_common.py
```

### Comparing `ultimate-utils-0.6.1/LICENSE` & `ultimate-utils-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/__init__.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 """
 Utils class with useful helper functions
 
 utils: https://www.quora.com/What-do-utils-files-tend-to-be-in-computer-programming-documentation
 """
 import json
 import pickle
+import re
 import subprocess
 import time
 
 import math
+import torch
 from datetime import datetime
 from pprint import pprint
 
 import dill
 import networkx as nx
 import numpy as np
 import random
@@ -39,19 +41,19 @@
 
 from lark import Lark, tree, Tree, Token
 
 from collections import deque
 
 from argparse import Namespace
 
-from typing import Union, Any, Optional, Match
+from typing import Union, Any, Optional, Match, Callable
 
 import progressbar
 
-from uutils.logging_uu.wandb_logging.common import setup_wand
+from uutils.logging_uu.wandb_logging.common import setup_wandb
 from uutils.torch_uu.distributed import find_free_port
 
 
 def hello():
     import uutils
     print(f'\nhello from uutils __init__.py in:\n{uutils}\n')
 
@@ -60,273 +62,42 @@
     hello()
 
 
 def hello_world():
     hello()
 
 
-def print_pids():
-    import torch.multiprocessing as mp
-
-    print('running main()')
-    print(f'current process: {mp.current_process()}')
-    print(f'pid: {os.getpid()}')
-
-# -
-
 def print_file(path_or_str: Union[str, Path]) -> None:
     """ prints the content of a file """
     cat_file(path2filename=path_or_str)
 
 
-# - getting args for expts
-
-def setup_args_for_experiment(args: Namespace,
-                              num_workers: int = 0,
-                              use_tb: bool = False  # not needed anymore since wandb exists
-                              ) -> Namespace:
+def clear_file_contents(path2file: Union[str, Path]):
     """
-    Sets up programming details for experiment to run but it should not affect the machine learning results.
-    The pretty print & save the args in alphabetically sorted order.
+    Clears contents of a file.
 
-    Note:
-        - This function assume the arguments for the experiment have been given already (e.g. through the terminal
-        or manually hardcoded in the main/run script).
 
-    Example/Recommended pattern to use:
-    1. From terminal (e.g. by running a bash main.sh script that runs python main_experiment.py):
-        args = parse_basic_meta_learning_args_from_terminal()
-        args = uutils.setup_args_for_experiment(args)
-        main(args)
-        wandb.finish() if is_lead_worker(args.rank) and args.log_to_wandb else None
-        print("Done with experiment, success!\a")
-
-    2. From script (also called, manual or hardcoded)
-        args = parse_basic_meta_learning_args_from_terminal()
-        args = manual_values_for_run(args)  # e.g. args.batch_size = 64, or ckpt
-        args = uutils.setup_args_for_experiment(args)
-        main(args)
-        wandb.finish() if is_lead_worker(args.rank) and args.log_to_wandb else None
-        print("Done with experiment, success!\a")
-
-    Things it sets up:
-        - 1. makes sure it has intial index (or use the one provided by user/checkpoint
-        - gets rank, port for DDP
-        - sets determinism or not
-        - device name
-        - dirs & filenames for logging
-        - cluster job id stuff
-        - pid, githash
-        - best_val_loss as -infinity
-        - wandb be stuff based on your options
-    todo:
-        - decide where to put annealing, likely in the parse args from terminal and set the default there. Likely
-        no annealing as default, or some rate that is done 5 times during entire training time or something like
-        that is based on something that tends to work.
-    """
-    import torch
-    import logging
-    import uutils
-    from uutils.logger import Logger as uuLogger
+    reason it works from SO:
+        the reason this works (in both C++ and python) is because by default when you open a file for writing, it truncates the existing contents. So really it's sorta a side effect, and thus I would prefer the explicit call to truncate() for clarity reasons, even though it is unnecessary.
 
-    # - 0. to make sure epochs or iterations is explicit, set it up in the argparse arguments
-    assert args.training_mode in ['epochs', 'iterations']
-    # - 1. set the iteration/epoch number to start training from
-    if args.training_mode == 'iterations':
-        # set the training iteration to start from beginning or from specified value (e.g. from ckpt iteration index).
-        args.it = 0 if not hasattr(args, 'it') else args.it
-        assert args.it >= 0, f'Iteration to train has to be start at zero or above but got: {args.it}'
-        args.epoch_num = -1
-    elif args.training_mode == 'epochs':
-        # set the training epoch number to start from beginning or from specified value e.g. from ckpt epoch_num index.
-        args.epoch_num = 0 if not hasattr(args, 'epoch_num') else args.epoch_num
-        assert args.epoch_num >= 0, f'Epoch number to train has to be start at zero or above but got: {args.epoch_num}'
-        args.it = -1
-    else:
-        raise ValueError(f'Invalid training mode: {args.training_mode}')
-    # - annealing learning rate...
-    # if (not args.no_validation) and (args.lr_reduce_steps is not None):
-    #     print('--lr_reduce_steps is applicable only when no_validation == True', 'ERROR')
-
-    # NOTE: this should be done outside cuz flags have to be declared first then parsed, args = parser.parse_args()
-    if hasattr(args, 'no_validation'):
-        args.validation = not args.no_validation
-
-    # - distributed params
-    args.rank = -1  # should be written by each worker with their rank, if not we are running serially
-    args.master_port = find_free_port()
-
-    # - determinism
-    if hasattr(args, 'always_use_deterministic_algorithms'):
-        if args.always_use_deterministic_algorithms:
-            uutils.torch_uu.make_code_deterministic(args.seed)
-            logging.warning(f'Seed being ignored, seed value: {args.seed=}')
-
-    # - get device name
-    print(f'{args.seed=}')
-    args.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
-    print(f'device: {args.device}')
-
-    # - get cluster info (including hostname)
-    load_cluster_jobids_to(args)
-
-    # - get log_root
-    # usually in options: parser.add_argument('--log_root', type=str, default=Path('~/data/logs/').expanduser())
-    args.log_root: Path = Path('~/data/logs/').expanduser() if not hasattr(args, 'log_root') else args.log_root
-    args.log_root: Path = Path(args.log_root).expanduser() if isinstance(args.log_root, str) else args.log_root
-    args.log_root: Path = args.log_root.expanduser()
-    args.current_time = datetime.now().strftime('%b%d_%H-%M-%S')
-    args.log_root = args.log_root / f'logs_{args.current_time}_jobid_{args.jobid}'
-    args.log_root.mkdir(parents=True, exist_ok=True)
-    # create tb in log_root
-    if use_tb:
-        from torch.utils.tensorboard import SummaryWriter
-        args.tb_dir = args.log_root / 'tb'
-        args.tb_dir.mkdir(parents=True, exist_ok=True)
-        args.tb = SummaryWriter(log_dir=args.tb_dir)
-
-    # - setup expanded path to checkpoint
-    if hasattr(args, 'path_to_checkpoint'):
-        # str -> Path(path_to_checkpoint).expand()
-        if isinstance(args.path_to_checkpoint, str):
-            args.path_to_checkpoint = Path(args.path_to_checkpoint).expanduser()
-        elif isinstance(args.path_to_checkpoint, Path):
-            args.path_to_checkpoint.expanduser()
-        elif args.path_to_checkpoint is None:  # do nothing since the args defualt is None
-            pass
-        else:
-            raise ValueError(f'Path to checkpoint is not of the right type: {type(args.path_to_checkpoint)=},'
-                             f'with value: {args.path_to_checkpoint=}')
-
-    # - get device name if possible
-    try:
-        args.gpu_name = torch.cuda.get_device_name(0)
-    except:
-        args.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
-        args.gpu_name = args.device
-    print(f'\nargs.gpu_name = {args.gpu_name}\n')  # print gpu_name if available else cpu
-
-    # - save PID
-    args.PID = str(os.getpid())
-    if torch.cuda.is_available():
-        args.nccl = torch.cuda.nccl.version()
-
-    # - email option (warning, not recommended! very unreliable, especially from cluster to cluster)
-    # logging.warning('uutils email is not recommended! very unreliable, especially from cluster to cluster)
-    # args.mail_user = 'brando.science@gmail.com'
-    # args.pw_path = Path('~/pw_app.config.json').expanduser()
-
-    # - try to get githash, might fail and return error string in field but whatever
-    args.githash: str = try_to_get_git_revision_hash_short()
-    args.githash_short: str = try_to_get_git_revision_hash_short()
-    args.githash_long: str = try_to_get_git_revision_hash_long()
-
-    # - get my logger, its set at the agent level
-    args.logger: uuLogger = uutils.logger.Logger(args)
-
-    # - best val loss
-    args.best_val_loss: float = float('inf')
-
-    # - wandb
-    if hasattr(args, 'log_to_wandb'):
-        setup_wand(args)
-    else:
-        pass
-
-    # - for debugging
-    # args.environ = [str(f'{env_var_name}={env_valaue}, ') for env_var_name, env_valaue in os.environ.items()]
+    ref: https://stackoverflow.com/questions/2769061/how-to-erase-the-file-contents-of-text-file-in-python
+    """
+    path2file: Path = expanduser(path2file)
+    open(path2file, "w").close()
+    # f = open('file.txt', 'r+')
+    # f.truncate(0)  # need '0' when using r+
 
-    # - to avoid pytorch multiprocessing issues with CUDA: https://pytorch.org/docs/stable/data.html
-    args.pin_memory = False
-    args.num_workers = num_workers
-
-    # - return
-    uutils.print_args(args)
-    uutils.save_args(args)
-    return args
 
+def print_python_version():
+    import sys
 
-def _parse_basic_meta_learning_args_from_terminal() -> Namespace:
-    """
-    Parse the arguments from the terminal so that the experiment runs as the user specified there.
-    Example/Recommended pattern to use:
-        See setup_args_for_experiment(...) to avoid copy pasting example/only mantain it in one place.
-    Note:
-        - Strongly recommended to see setup_args_for_experiment(...)
-    """
-    import argparse
-    # import torch.nn as nn
+    print(f'python version: {sys.version=}')
 
-    parser = argparse.ArgumentParser()
 
-    # experimental setup
-    parser.add_argument('--debug', action='store_true', help='if debug')
-    parser.add_argument('--force_log', action='store_true', help='to force logging')
-    parser.add_argument('--serial', action='store_true', help='if running serially')
-    parser.add_argument('--args_hardcoded_in_script', action='store_true',
-                        help='set to true if the args will be set from the script manually'
-                             'e.g. by hardcoding them in the script.')
-
-    parser.add_argument('--split', type=str, default='train', help=' train, val, test')
-    # this is the name used in synth agent, parser.add_argument('--data_set_path', type=str, default='', help='path to data set splits')
-    parser.add_argument('--data_path', type=str, default='VALUE SET IN MAIN Meta-L SCRIPT',
-                        help='path to data set splits')
-
-    parser.add_argument('--log_root', type=str, default=Path('~/data/logs/').expanduser())
-
-    parser.add_argument('--num_epochs', type=int, default=-1)
-    parser.add_argument('--num_its', type=int, default=-1)
-    parser.add_argument('--training_mode', type=str, default='iterations')
-    # parser.add_argument('--no_validation', action='store_true', help='no validation is performed')
-    # parser.add_argument('--embed_dim', type=int, default=256)
-    # parser.add_argument('--nhead', type=int, default=8)
-    # parser.add_argument('--num_layers', type=int, default=1)
-    # parser.add_argument('--criterion', type=str, help='loss criterion', default=nn.CrossEntropyLoss())
-
-    # - optimization
-    # parser.add_argument('--optimizer', type=str, default='Adam')
-    # parser.add_argument('--learning_rate', type=float, default=1e-5)
-    # parser.add_argument('--num_warmup_steps', type=int, default=-1)
-    # parser.add_argument('--momentum', type=float, default=0.9)
-    # parser.add_argument('--batch_size', type=int, default=128)
-    # parser.add_argument('--l2', type=float, default=0.0)
-    # parser.add_argument('--lr_reduce_steps', default=3, type=int,
-    #                     help='the number of steps before reducing the learning rate \
-    #                     (only applicable when no_validation == True)')
-    # parser.add_argument('--lr_reduce_patience', type=int, default=10)
-
-    # - miscellaneous
-    parser.add_argument('--path_to_checkpoint', type=str, default=None,
-                        help='the model checkpoint path to resume from.')
-    parser.add_argument('--seed', type=int, default=0)
-    parser.add_argument('--always_use_deterministic_algorithms', action='store_true',
-                        help='tries to make pytorch fully determinsitic')
-    # for now default is 4 since meta-learning code is not parallizable right now.
-    parser.add_argument('--num_workers', type=int, default=4,
-                        help='the number of data_lib-loading threads (when running serially')
-
-    # - sims/dists computations
-    parser.add_argument('--sim_compute_parallel', action='store_true', help='compute sim or dist in parallel.')
-    parser.add_argument('--metrics_as_dist', action='store_true', help='')
-    parser.add_argument('--show_layerwise_sims', action='store_true', help='show sim/dist values per layer too')
-
-    # - wandb
-    parser.add_argument('--log_to_wandb', action='store_true', help='store to weights and biases')
-    parser.add_argument('--wandb_project', type=str, default='meta-learning-playground')
-    parser.add_argument('--wandb_entity', type=str, default='brando')
-    parser.add_argument('--wandb_group', type=str, default='experiment_debug', help='helps grouping experiment runs')
-    # parser.add_argument('--wandb_log_freq', type=int, default=10)
-    # parser.add_argument('--wandb_ckpt_freq', type=int, default=100)
-    # parser.add_argument('--wanbd_mdl_watch_log_freq', type=int, default=-1)
-
-    # - parse arguments
-    args = parser.parse_args()
-    # - load cluster ids so that wandb can use it later for naming runs, experiments, etc.
-    load_cluster_jobids_to(args)
-    return args
+# - getting args for expts
 
 
 def parse_args() -> Namespace:
     """
         Parses command line arguments
     """
     parser = argparse.ArgumentParser(description="Pretraining Experiment")
@@ -511,23 +282,61 @@
         git_hash: str = str(_get_git_revision_hash())
         return git_hash
     except Exception as e:
         print(f'(Not critical), unable to retrieve githash for reason: {e}')
         return f'{e}'
 
 
-def run_bash_command(cmd: str) -> Any:
-    import subprocess
+def run_bash_command(cmd: str, use_run: bool = True) -> Any:
+    """
+    Runs a given command in bash from within python.
 
-    process = subprocess.Popen(cmd.split(), stdout=subprocess.PIPE)
-    output, error = process.communicate()
-    if error:
-        raise Exception(error)
+    Details (from SO):
+        The main difference is that subprocess.run() executes a command and waits for it to finish, while with
+        subprocess.Popen you can continue doing your stuff while the process finishes and then just repeatedly call
+        Popen.communicate() yourself to pass and receive data to your process. Secondly, subprocess.run() returns
+        subprocess.CompletedProcess.
+        subprocess.run() just wraps Popen and Popen.communicate() so you don't need to make a loop to pass/receive data
+        or wait for the process to finish.
+
+    ref:
+        - https://stackoverflow.com/questions/39187886/what-is-the-difference-between-subprocess-popen-and-subprocess-run#:~:text=The%20main%20difference%20is%20that,receive%20data%20to%20your%20process.
+    """
+    import subprocess
+    if use_run:
+        # - recommended, see comment above. My understanding is that this blocks until done
+        res = subprocess.run(cmd.split(), check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        return res
     else:
-        return output
+        # - I think this is fine for simple commands but I think one has to loop through the communicate until done
+        process = subprocess.Popen(cmd.split(), stdout=subprocess.PIPE)
+        output, error = process.communicate()
+        if error:
+            raise Exception(error)
+        else:
+            return output
+
+
+def stanford_reauth():
+    """"
+    re-authenticates the python process in the kerberos system so that the
+    python process is not killed randomly.
+
+    ref: https://unix.stackexchange.com/questions/724902/how-does-one-send-new-commands-to-run-to-an-already-running-nohup-process-or-run
+    """
+    reauth_cmd: str = f'echo $SU_PASSWORD | /afs/cs/software/bin/reauth'
+    out = run_bash_command(reauth_cmd)
+    print('Output of reauth (/afs/cs/software/bin/reauth with password): ')
+    print(f'--> {out=}')
+    raise Exception('For now we are not doing reauth within python')
+
+
+def get_nvidia_smi_output() -> str:
+    out = run_bash_command('nvidia-smi')
+    return out
 
 
 def _get_git_revision_hash():
     """ ref: https://stackoverflow.com/questions/14989858/get-the-current-git-hash-in-a-python-script """
     return subprocess.check_output(['git', 'rev-parse', 'HEAD']).decode('ascii').strip()
 
 
@@ -612,14 +421,40 @@
     try:
         shutil.rmtree(str(path))
     except OSError:
         # do nothing if removing fails
         pass
 
 
+def copy_folders_recursively(src_root: Union[str, Path], root4dst: Union[str, Path],
+                             dirnames4dst: list[Union[str, Path]]):
+    """
+    Copying dirnames in src_root into roo4dst. Note dirnames4dst should be the same as the dirnames in the sorc.
+
+    note: copying the files was fast locally! Likely the downloading of the data from network + extracting is what causes
+    things to be slow.
+
+    :param src_root:
+    :param root4dst:
+    :param dirnames4dst:
+    :return:
+    """
+    root: Path = expanduser(root4dst)
+    src_root: Path = expanduser(src_root)
+    from distutils.dir_util import copy_tree
+    for dirname in dirnames4dst:
+        dirname: Path = expanduser(dirname)
+        src: Path = src_root / expanduser(dirname)
+        dst: Path = root / expanduser(dirname)
+        src: str = str(src)
+        dst: str = str(dst)
+        print(f'copying: {src=} -> {dst=}')
+        copy_tree(src, dst)
+
+
 def oslist_for_path(path):
     return [f for f in path.iterdir() if f.is_dir()]
 
 
 def _make_and_check_dir(path):
     """
     NOT NEEDED use:
@@ -659,18 +494,20 @@
     m = math.floor(s / 60)  # compute amount of whole integer minutes it took
     s -= m * 60  # compute how much time remaining time was spent in seconds
     ##
     msg = f"time passed: hours:{h}, minutes={m}, seconds={s}"
     return msg, h
 
 
-def report_times(start: float) -> str:
+def report_times(start: float, verbose: bool = False) -> str:
     import time
     duration_secs = time.time() - start
     msg = f"time passed: hours:{duration_secs / (60 ** 2)}, minutes={duration_secs / 60}, seconds={duration_secs}"
+    if verbose:
+        print(msg)
     return msg
 
 
 def is_NaN(value):
     """
     Checks is value is problematic by checking if the value:
     is not finite, is infinite or is already NaN
@@ -754,14 +591,60 @@
     ref: https://stackoverflow.com/a/432948/1601580
     """
     assert (True + True + True + False) == 3, 'Semantics of python changed'  # guard against change semantics of python.
     xor_bool: bool = (bool(a) + bool(b) == 1)
     return xor_bool
 
 
+def check_number_of_files_open_vs_allowed_open():
+    """
+    Checks if the number of files open is close to the number of files that can be open.
+
+    ref: https://stackoverflow.com/questions/12090503/listing-open-files-using-python
+    """
+    import resource
+    soft_limit, hard_limit = resource.getrlimit(resource.RLIMIT_NOFILE)
+    print(f"soft_limit={soft_limit}, hard_limit={hard_limit}")
+    # import psutil
+    # p = psutil.Process()
+    # print(f"number of files open={p.num_fds()}")
+    import psutil
+    open_files = 0
+    for process in psutil.process_iter():
+        try:
+            files = process.open_files()
+            open_files += len(files)
+        except (psutil.NoSuchProcess, psutil.AccessDenied, psutil.ZombieProcess):
+            pass
+
+    print(f"Number of open files: {open_files}")
+
+
+def get_filtered_local_params(local_vars, verbose: bool = False, var_name_in_front: str = '') -> dict[str, Any]:
+    """
+    Set local_vars = locals() from parent function to print parent function input parameters & names.
+
+suggested call:
+    get_filtered_local_params(locals(), verbose=verbose, var_name_in_front='training_arguments') if verbose else None
+    """
+    # Get all local variables done outside the function
+    # e.g. local_vars = locals()
+
+    # Filter out undesired variables
+    filtered_vars = {k: v for k, v in local_vars.items() if k != 'self' and not k.startswith('__')}
+
+    # Print the variable names and their values
+    if verbose:
+        if var_name_in_front != '':
+            print(f"{var_name_in_front}:")
+        for var_name, var_value in filtered_vars.items():
+            print(f"{var_name}: {var_value}")
+    return filtered_vars
+
+
 ##
 
 def make_and_check_dir2(path):
     """
         tries to make dir/file, if it exists already does nothing else creates it.
     """
     try:
@@ -775,42 +658,59 @@
 """
 Greater than 4 I get this error:
 
 ValueError: Seed must be between 0 and 2**32 - 1
 """
 
 
-def get_truly_random_seed_through_os():
+def get_truly_random_seed_through_os(rand_size: int = 4) -> int:
     """
     Usually the best random sample you could get in any programming language is generated through the operating system. 
     In Python, you can use the os module.
 
     source: https://stackoverflow.com/questions/57416925/best-practices-for-generating-a-random-seeds-to-seed-pytorch/57416967#57416967
     """
-    RAND_SIZE = 4
     random_data = os.urandom(
-        RAND_SIZE
+        rand_size
     )  # Return a string of size random bytes suitable for cryptographic use.
-    random_seed = int.from_bytes(random_data, byteorder="big")
-    return random_seed
+    random_seed: int = int.from_bytes(random_data, byteorder="big")
+    return int(random_seed)
 
 
-def seed_everything(seed=42):
+def get_different_pseudo_random_seed_every_time_using_time() -> int:
+    """ Get a different pseudo random seed every time using time."""
+    import random
+    import time
+
+    # random.seed(int(time.time()))
+    seed: int = int(time.time())
+    return seed
+
+
+def seed_everything(seed: int,
+                    seed_torch: bool = True,
+                    ):
     """
     https://stackoverflow.com/questions/57416925/best-practices-for-generating-a-random-seeds-to-seed-pytorch
     """
-    import torch
     import random
+    import numpy as np
+    import os
 
     random.seed(seed)
-    os.environ["PYTHONHASHSEED"] = str(seed)
     np.random.seed(seed)
-    torch.manual_seed(seed)
-    torch.backends.cudnn.deterministic = True
-    torch.backends.cudnn.benchmark = False
+    os.environ["PYTHONHASHSEED"] = str(seed)
+    if seed_torch:
+        import torch
+        torch.manual_seed(seed)
+        # makes convs deterministic: https://stackoverflow.com/a/66647424/1601580, torch.backends.cudnn.deterministic=True only applies to CUDA convolution operations, and nothing else. Therefore, no, it will not guarantee that your training process is deterministic
+        torch.backends.cudnn.deterministic = True
+        torch.backends.cudnn.benchmark = False
+        # #torch.use_deterministic_algorithms(True) # do not uncomment
+        # fully_deterministic: bool = uutils.torch_uu.make_code_deterministic(args.seed)
 
 
 def get_hostname_mit():
     from socket import gethostname
 
     hostname = gethostname()
     if "polestar-old" in hostname or hostname == "gpu-16" or hostname == "gpu-17":
@@ -946,40 +846,44 @@
         sorted_names: list = sorted(dict_args.keys(), key=lambda x: x)
     [print(f'{k, dict_args[k]}') for k in sorted_names]
     # pprint_any_dict(dict_args)
     # pprint(vars(args))
 
 
 def pprint_args(args: Namespace):
+    print(f'args=')
     print_args(args)
+    print()
 
 
 def pprint_dict(dic):
     pprint_any_dict(dic)
 
 
-def pprint_any_dict(dic: dict, indent: Optional[int] = None):
+def pprint_any_dict(dic: dict, indent: Optional[int] = None, var_name_in_front: str = ''):
     """
     This pretty prints a json.
 
     Note: this is not the same as pprint.
 
     Warning:
         - if indent is an int then the values will become strings.
 
     todo: how to have pprint do indent and keep value without making it into a string.
     """
     import json
+    if var_name_in_front != '':
+        print(f'{var_name_in_front}=')
 
     if indent:
         # make all keys strings recursively with their naitve str function
         dic = to_json(dic)
         print(json.dumps(dic, indent=4, sort_keys=True))  # only this one works...idk why
     else:
-        pprint(dict)
+        pprint(dic)
     # return pretty_dic
 
 
 def pprint_namespace(ns):
     """ pretty prints a namespace """
     pprint_any_dict(ns)
 
@@ -1017,22 +921,22 @@
     force: this argument when true forces anything that isn't jsonable into a string so that you force it to save as
     json data anyway. e.g. objs, function, tensorboard etc. are made into ANY string representation they have & saved.
     This is likely useful when you have param args floating around carying pointers/refs to arbitrary data but you
     want to save it anyway.
     """
     import json
 
-    path2filename = expanduser(path2filename)
+    path2filename: Path = expanduser(path2filename)
 
     data = to_json(data) if force else data
     with open(path2filename, mode) as f:
         json.dump(data, f, indent=indent, sort_keys=sort_keys)
 
 
-def expanduser(path: Union[str, Path]):
+def expanduser(path: Union[str, Path]) -> Path:
     """
 
     note: if you give in a path no need to get the output of this function because it mutates path. If you
     give a string you do need to assign the output to a new variable
     :param path:
     :return:
     """
@@ -1146,15 +1050,15 @@
     latex = latex.replace('+-', ' $\\pm$ ')
     return latex
 
 
 ##
 
 def create_logs_dir_and_load(opts):
-    from uutils import load_cluster_jobids_to
+    # from uutils import load_cluster_jobids_to
     from datetime import datetime
 
     load_cluster_jobids_to(opts)
     # opts.log_root = Path('~/data/logs/').expanduser()
     # create and load in args path to current experiments from log folder path
     opts.current_time = datetime.now().strftime('%b%d_%H-%M-%S')
     opts.log_experiment_dir = opts.log_root / f'logs_{opts.current_time}_jobid_{opts.jobid}'
@@ -1173,14 +1077,47 @@
 
 
 def save_args(args: Namespace, args_filename: str = 'args.json'):
     """ Saves args, crucially in sorted order. """
     save_opts(args, args_filename)
 
 
+def get_home_pwd_local_machine_snap() -> None:
+    """
+    Gets the path to local machine in snap (lfs) with user name appended at the end.
+
+bash command:
+# Local machine as Home
+export LOCAL_MACHINE_PWD=$(python3 -c "import socket;hostname=socket.gethostname().split('.')[0];print(f'/lfs/{hostname}/0/brando9');")
+mkdir -p $LOCAL_MACHINE_PWD
+export WANDB_DIR=$LOCAL_MACHINE_PWD
+export HOME=$LOCAL_MACHINE_PWD
+
+# Without python, doesn't work fix some day...
+# export LOCAL_MACHINE_PWD=$(python3 -c "import socket;hostname=socket.gethostname().split('.')[0];print(f'/lfs/{hostname}/0/brando9');")
+# export LOCAL_MACHINE_PWD=$(python3 -c "import uutils; uutils.get_home_pwd_local_machine_snap()")
+export HOSTNAME=$(hostname)
+export LOCAL_MACHINE_PWD="/lfs/${HOSTNAME::-13}/0/brando9"
+mkdir -p $LOCAL_MACHINE_PWD
+export WANDB_DIR=$LOCAL_MACHINE_PWD
+export HOME=$LOCAL_MACHINE_PWD
+
+ref:
+    - one liner: https://stackoverflow.com/questions/27658675/how-to-remove-last-n-characters-from-a-string-in-bash
+    """
+    import socket
+    hostname: str = socket.gethostname()
+    hostname: str = hostname.split('.')[0]
+    local_pwd: str = f'/lfs/{hostname}/0/brando9'
+    print(local_pwd)  # returns to terminal
+    # return local_pwd
+    # on liner
+    # import socket;hostname = socket.gethostname().split('.')[0];print(f'/lfs/{hostname}/0/brando9');
+
+
 def load_cluster_jobids_to(args):
     import os
 
     # Get Get job number of cluster
     args.jobid = -1
     args.slurm_jobid, args.slurm_array_task_id = -1, -1
     args.condor_jobid = -1
@@ -1201,14 +1138,18 @@
         try:
             args.jobid = int(os.environ["PBS_JOBID"])
         except:
             args.jobid = os.environ["PBS_JOBID"]
     if 'dgx' in str(gethostname()):
         args.jobid = f'{args.jobid}_pid_{os.getpid()}'
 
+    if 'LSB_JOBID' in os.environ:
+        jobid: str = str(os.environ['LSB_JOBID'])
+        args.jobid = jobid
+
 
 def set_system_wide_force_flush():
     """
     Force flushes the entire print function everywhere.
 
     https://stackoverflow.com/questions/230751/how-to-flush-output-of-print-function
     :return:
@@ -1279,15 +1220,15 @@
     # https://stackoverflow.com/questions/20597088/display-a-png-image-from-python-on-mint-15-linux
     img = mpimg.imread(path2file)
     plt.imshow(img)
     plt.show()
 
     # remove file https://stackoverflow.com/questions/6996603/how-to-delete-a-file-or-folder
     if not save_file:
-        path2file.unlink()
+        path2file.unlink(missing_ok=True)
 
 
 def visualize_lark(string: str, parser: Lark, path2filename: Union[str, Path]):
     if type(path2filename) is str:
         path2filename = Path(path2filename).expanduser()
     else:
         path2filename = path2filename.expanduser()
@@ -1501,14 +1442,33 @@
     # - the merged args
     # node: The vars() function returns the __dict__ attribute to values of the given object e.g {field:value}.
     merged_key_values_for_namespace: dict = merge_two_dicts(vars(starting_args), vars(updater_args))
     args = Namespace(**merged_key_values_for_namespace)
     return args
 
 
+def check_dict1_is_in_dict2(dict1: dict,
+                            dict2: dict,
+                            verbose: bool = False,
+                            ) -> bool:
+    """
+    Check if dict1 is in dict2. i.e. dict1 <= dict2.
+    """
+    for k, v in dict1.items():
+        if k not in dict2:
+            print(f'--> {k=} is not in dict2 with value {dict1[k]=}')
+            return False
+        if v != dict2[k]:
+            print(f'--> {k=} is in dict2 but with different value \n{dict1[k]=} \n{dict2[k]=}')
+            return False
+        if verbose:
+            print(f"--> {k=} is in both dicts, look: \n{dict1[k]=} \n{dict2[k]=} \n")
+    return True
+
+
 def is_pos_def(x: np.ndarray) -> bool:
     """
     ref:
         - https://stackoverflow.com/questions/16266720/find-out-if-matrix-is-positive-definite-with-numpy
     """
     return np.all(np.linalg.eigvals(x) > 0)
 
@@ -1566,14 +1526,348 @@
         return True
     else:
         is_negative_integer: bool = value.startswith("-") and value[1:].isdigit()
         is_integer: bool = is_positive_integer or is_negative_integer
         return is_integer
 
 
+def is_anonymous_function(f: Any) -> bool:
+    """
+    Returns true if it's an anonynouys function.
+
+    ref: https://stackoverflow.com/questions/3655842/how-can-i-test-whether-a-variable-holds-a-lambda
+    """
+    if hasattr(f, '__name__'):
+        return callable(f) and f.__name__ == "<lambda>"
+    else:
+        return False
+
+
+def get_anonymous_function_attributes(anything: Any,
+                                      halt: bool = False,
+                                      verbose: bool = False,
+                                      very_verbose: bool = False,
+                                      ) -> dict[str, Callable]:
+    """
+    Returns the dictionary of name of fields to anonymous functions in the past anything thing.
+
+    :param very_verbose:
+    :param anything:
+    :param halt:
+    :param verbose:
+    :return:
+    """
+    anons: dict = {}
+    for field_name in dir(anything):
+        field = getattr(anything, field_name)
+        if very_verbose:
+            print(f'{field_name=}')
+            print(f'{field=}')
+        if is_anonymous_function(field):
+            if verbose or very_verbose:
+                print(f'{field_name=}')
+                print(f'{field=}')
+            if halt:
+                from pdb import set_trace as st
+                st()
+            anons[str(field_name)] = field
+    return anons
+
+
+def get_anonymous_function_attributes_recursive(anything: Any, path: str = '', print_output: bool = False) -> dict[
+    str, Callable]:
+    """
+    Finds in a dictionary from path of field_name calling to the callable anonymous function.
+    It is recommended that you hardcode path to the name of the top object being given to this function (sorry I tried
+    doing .__name__ of anything but it doesn't always have that field set).
+
+    :param anything:
+    :param path:
+    :return:
+    """
+    anons: dict = {}
+
+    def _get_anonymous_function_attributes_recursive(anything: Any, path: Optional[str] = '') -> None:
+
+        if is_anonymous_function(anything):
+            # assert field is anything, f'Err not save thing/obj: \n{field=}\n{anything=}'
+            # key: str = str(dict(obj=anything, field_name=field_name))
+            key: str = str(path)
+            anons[key] = anything
+        else:
+            for field_name in dir(anything):
+                # most likely it's one of YOUR field causing the anonymous function bug, so only loop through those
+                if not bool(re.search(r'__(.+)__', field_name)):
+                    field = getattr(anything, field_name)
+                    # only recurse if new field is not itself
+                    if field is not anything:  # avoids infinite recursions
+                        # needs a new variable or the paths for different field will INCORRECTLY crash
+                        path_for_this_field = f'{path}.{field_name}'
+                        print(f'{path_for_this_field}')
+                        _get_anonymous_function_attributes_recursive(field, path_for_this_field)
+        return
+
+    _get_anonymous_function_attributes_recursive(anything, path)
+    if print_output:
+        print(f'top path given {path=}')
+        print(f'{len(anons.keys())=}')
+        for k, v in anons.items():
+            print()
+            print(f'{k=}')
+            print(f'{v=}')
+    return anons
+
+
+def download_and_extract(url: str,
+                         path_used_for_zip: Path = Path('~/data/'),
+                         path_used_for_dataset: Path = Path('~/data/tmp/'),
+                         rm_zip_file_after_extraction: bool = True,
+                         force_rewrite_data_from_url_to_file: bool = False,
+                         clean_old_zip_file: bool = False,
+                         gdrive_file_id: Optional[str] = None,
+                         gdrive_filename: Optional[str] = None,
+                         ):
+    """
+    Downloads data and tries to extract it according to different protocols/file types.
+
+    note:
+        - to force a download do:
+            force_rewrite_data_from_url_to_file = True
+            clean_old_zip_file = True
+        - to NOT remove file after extraction:
+            rm_zip_file_after_extraction = False
+
+
+    Tested with:
+    - zip files, yes!
+
+    Later:
+    - todo: tar, gz, gdrive
+    force_rewrite_data_from_url_to_file = remvoes the data from url (likely a zip file) and redownloads the zip file.
+    """
+    path_used_for_zip: Path = expanduser(path_used_for_zip)
+    path_used_for_zip.mkdir(parents=True, exist_ok=True)
+    path_used_for_dataset: Path = expanduser(path_used_for_dataset)
+    path_used_for_dataset.mkdir(parents=True, exist_ok=True)
+    # - download data from url
+    if gdrive_filename is None:  # get data from url, not using gdrive
+        import ssl
+        ctx = ssl.create_default_context()
+        ctx.check_hostname = False
+        ctx.verify_mode = ssl.CERT_NONE
+        print("downloading data from url: ", url)
+        import urllib
+        import http
+        response: http.client.HTTPResponse = urllib.request.urlopen(url, context=ctx)
+        print(f'{type(response)=}')
+        data = response
+        # save zipfile like data to path given
+        filename = url.rpartition('/')[2]
+        path2file: Path = path_used_for_zip / filename
+    else:  # gdrive case
+        from torchvision.datasets.utils import download_file_from_google_drive
+        # if zip not there re-download it or force get the data
+        path2file: Path = path_used_for_zip / gdrive_filename
+        if not path2file.exists():
+            download_file_from_google_drive(gdrive_file_id, path_used_for_zip, gdrive_filename)
+        filename = gdrive_filename
+    # -- write downloaded data from the url to a file
+    print(f'{path2file=}')
+    print(f'{filename=}')
+    if clean_old_zip_file:
+        path2file.unlink(missing_ok=True)
+    if filename.endswith('.zip') or filename.endswith('.pkl'):
+        # if path to file does not exist or force to write down the data
+        if not path2file.exists() or force_rewrite_data_from_url_to_file:
+            # delete file if there is one if your going to force a rewrite
+            path2file.unlink(missing_ok=True) if force_rewrite_data_from_url_to_file else None
+            print(f'about to write downloaded data from url to: {path2file=}')
+            # wb+ is used sinze the zip file was in bytes, otherwise w+ is fine if the data is a string
+            with open(path2file, 'wb+') as f:
+                # with open(path2file, 'w+') as f:
+                print(f'{f=}')
+                print(f'{f.name=}')
+                f.write(data.read())
+            print(f'done writing downloaded from url to: {path2file=}')
+    elif filename.endswith('.gz'):
+        pass  # the download of the data doesn't seem to be explicitly handled by me, that is done in the extract step by a magic function tarfile.open
+    # elif is_tar_file(filename):
+    #     os.system(f'tar -xvzf {path_2_zip_with_filename} -C {path_2_dataset}/')
+    else:
+        raise ValueError(f'File type {filename=} not supported.')
+
+    # - unzip data written in the file
+    extract_to = path_used_for_dataset
+    print(f'about to extract: {path2file=}')
+    print(f'extract to target: {extract_to=}')
+    if filename.endswith('.zip'):
+        import zipfile  # this one is for zip files, inspired from l2l
+        zip_ref = zipfile.ZipFile(path2file, 'r')
+        zip_ref.extractall(extract_to)
+        zip_ref.close()
+        if rm_zip_file_after_extraction:
+            path2file.unlink(missing_ok=True)
+    elif filename.endswith('.gz'):
+        import tarfile
+        file = tarfile.open(fileobj=response, mode="r|gz")
+        file.extractall(path=extract_to)
+        file.close()
+    elif filename.endswith('.pkl'):
+        # no need to extract it, but when you use the data make sure you torch.load it or pickle.load it.
+        print(f'about to test torch.load of: {path2file=}')
+        data = torch.load(path2file)  # just to test
+        assert data is not None
+        print(f'{data=}')
+        pass
+    else:
+        raise ValueError(f'File type {filename=} not supported, edit code to support it.')
+        # path_2_zip_with_filename = path_2_ziplike / filename
+        # os.system(f'tar -xvzf {path_2_zip_with_filename} -C {path_2_dataset}/')
+        # if rm_zip_file:
+        #     path_2_zip_with_filename.unlink(missing_ok=True)
+        # # raise ValueError(f'File type {filename=} not supported.')
+    print(f'done extracting: {path2file=}')
+    print(f'extracted at location: {path_used_for_dataset=}')
+    print(f'-->Succes downloading & extracting dataset at location: {path_used_for_dataset=}')
+
+
+def _download_url_no_ctx(url):
+    # data = urllib.request.urlopen(url)
+    # filename = url.rpartition('/')[2]
+    # file_path = os.path.join(root, raw_folder, filename)
+    # with open(file_path, 'wb') as f:
+    #     f.write(data.read())
+    # file_processed = os.path.join(root, processed_folder)
+    pass
+
+
+def _download_and_unzip_with_tar_xvzf_py_shell_cmd(url: str, extract_to: Path = Path('~/data/tmp/'),
+                                                   mode="r|gz") -> Path:
+    """
+
+    this is based on my download_and_extract_miniimagenet but that one uses google to get data so idk if this will work.
+    """
+    import ssl
+    ctx = ssl.create_default_context()
+    ctx.check_hostname = False
+    ctx.verify_mode = ssl.CERT_NONE
+
+    print("downloading dataset from ", url)
+    import urllib
+    response = urllib.request.urlopen(url, context=ctx)
+    # data = urllib.request.urlopen(url)  # note: l2l just does this without ctx
+    # from torchvision.datasets.utils import download_file_from_google_drive, extract_archive
+    # path = path.expanduser()
+    # file_id = '1rV3aj_hgfNTfCakffpPm7Vhpr1in87CR'
+    # filename_zip = 'miniImagenet.tgz'
+    # if zip not there re-download it
+    # path_2_zip = path / filename_zip
+    # if not path_2_zip.exists():
+    #     download_file_from_google_drive(file_id, path, filename_zip)
+
+    with open(response, mode='r') as file:
+        print("extracting to ", extract_to)
+        path_2_zip: str = str(expanduser(extract_to / str(file.name)).name)
+        print("path_2_zip is ", path_2_zip)
+        os.system(f'tar -xvzf {path_2_zip} -C {extract_to}/')
+        return extract_to / str(file.name)
+
+
+def _download_and_unzip_tinfer(url: str, extract_to: Path = Path('~/data/tmp/')) -> Path:
+    """download and unzip ala tinfer proj & returns the path it extracted to."""
+    extract_to: Path = expanduser(extract_to)
+    import ssl
+    ctx = ssl.create_default_context()
+    ctx.check_hostname = False
+    ctx.verify_mode = ssl.CERT_NONE
+
+    print("downloading dataset from ", url)
+    import urllib
+    response = urllib.request.urlopen(url, context=ctx)
+    import tarfile
+    file = tarfile.open(fileobj=response, mode="r|gz")
+    print("extracting to ", extract_to)
+    file.extractall(path=extract_to)
+    file.close()
+
+    # todo test bellow to see if file.name is actually correct/works as I expect
+    path_2_zip = extract_to / str(file.name)
+    return path_2_zip
+
+
+def _download_ala_l2l_their_original_code(urls, root, raw_folder, processed_folder):
+    from six.moves import urllib
+    import zipfile
+
+    # if self._check_exists():
+    #     return
+
+    # download files
+    try:
+        os.makedirs(os.path.join(root, raw_folder))
+        os.makedirs(os.path.join(root, processed_folder))
+    except OSError as e:
+        import errno
+        if e.errno == errno.EEXIST:
+            pass
+        else:
+            raise
+
+    for url in urls:
+        print('== Downloading ' + url)
+        data = urllib.request.urlopen(url)
+        filename = url.rpartition('/')[2]
+        file_path = os.path.join(root, raw_folder, filename)
+        with open(file_path, 'wb') as f:
+            f.write(data.read())
+        file_processed = os.path.join(root, processed_folder)
+        print("== Unzip from " + file_path + " to " + file_processed)
+
+        zip_ref = zipfile.ZipFile(file_path, 'r')
+        zip_ref.extractall(file_processed)
+        zip_ref.close()
+    print("Download finished.")
+
+
+# -- bytes for model size
+
+def calculate_bytes_for_model_size(num_params: int,
+                                   precision: str = 'float32_bytes',
+                                   ) -> int:
+    """
+    Calculates size of model in given precision ideally in bytes:
+        size = num_params * precision in bytes (number of bytes to represent float)
+
+    bits -> bytes == bits / 8 (since 1 bytes is 8 bits)
+
+    number of GigaBytes for model size = num_params * precision in bytes
+    1 Byte = 8 bits ~ 1 character = 1 addressable unit in memmory
+    FB32 = 4 bytes = 4 * 8 bits = 32 bits = 1S 8Exp 23Mantissa
+    FB16 = 2 bytes = 2 * 8 bits = 16 bits = 1S 5Exp 10Mantissa
+    BF16 = 2 bytes = 2 * 8 bits = 16 bits = 1S 8Exp 7Mantissa
+    Example:
+        num_params = 176B (bloom-176B)  # note gpt3 175B params
+        precision = 'bfloat16_bytes'  # 4 bytes
+        size = 176B * 4 = 176 * 10**8 * 2 = 352 * 10**8 = 352GB (giga bytes)
+    :param num_params:
+    :return:
+    """
+    size: int = -1
+    if precision == 'float32_bytes':
+        num_bytes: int = 4
+        size: int = num_params * num_bytes
+    if 'bytes' not in precision or 'bits' in precision:  #
+        # return in bits
+        size: int = num_params * num_bytes * 8
+        return size
+    else:
+        # return in bytes
+        return size
+
+
 # -- regex
 
 def matches_regex(regex: str, content: str) -> Optional[Match[str]]:
     import re
     return re.match(regex, content)
 
 
@@ -1588,14 +1882,65 @@
         assert re.match(regex, content), f'Failed on {content=} with {regex=}'
         if re.match(regex, content):
             print(content)
 
 
 # --  other
 
+def get_duplicates(lst: list) -> list:
+    """
+    Returns the duplicate elements in the list.
+
+    ref: https://stackoverflow.com/questions/9835762/how-do-i-find-the-duplicates-in-a-list-and-create-another-list-with-them
+    """
+    seen: set = set()
+    dup: list = []
+    for val in lst:
+        if val in seen:
+            dup.append(val)
+        else:
+            seen.add(val)
+    return dup
+
+
+def get_non_intersecting_elements(lst: list) -> list:
+    """
+    Gets you the elements that are not common to the two lists i.e. not intersecting elements.
+
+    ref: https://stackoverflow.com/questions/9835762/how-do-i-find-the-duplicates-in-a-list-and-create-another-list-with-them
+    """
+    seen: set = set()
+    not_intersect: set = set()
+    for val in lst:
+        if val not in seen:
+            not_intersect.add(val)
+            seen.add(val)
+        else:
+            not_intersect.remove(val)
+    return list(not_intersect)
+
+
+def list_of_elements_present(lst: list) -> list:
+    """
+    Gets you the elements in the list (in the SO post it's refered as the unique elements list).
+
+    ref: https://stackoverflow.com/questions/9835762/how-do-i-find-the-duplicates-in-a-list-and-create-another-list-with-them
+    :param lst:
+    :return:
+    """
+    # seen = set()
+    # uniq = []
+    # for x in a:
+    #     if x not in seen:
+    #         uniq.append(x)
+    #         seen.add(x)
+    # return uniq
+    return list(set(lst))
+
+
 def lists_equal(l1: list, l2: list) -> bool:
     """
 
     import collections
     compare = lambda x, y: collections.Counter(x) == collections.Counter(y)
     ref:
         - https://stackoverflow.com/questions/9623114/check-if-two-unordered-lists-are-equal
@@ -1604,14 +1949,86 @@
     import collections
     compare = lambda x, y: collections.Counter(x) == collections.Counter(y)
     set_comp = set(l1) == set(l2)  # removes duplicates, so returns true when not sometimes :(
     multiset_comp = compare(l1, l2)  # approximates multiset
     return set_comp and multiset_comp  # set_comp is gere in case the compare function doesn't work
 
 
+def get_intersection_overlap(a, b) -> float:
+    """
+    Returns the intersection over union of two bounding boxes.
+    Note, lower and upper bounds intersect exactly, it is considered not an intersection.
+
+    ref:
+        - https://stackoverflow.com/a/2953979/1601580
+    """
+    return max(0, min(a[1], b[1]) - max(a[0], b[0]))
+
+
+def get_intersection_overlap_care_about_exact_match(a, b) -> float:
+    """
+    Return the amount of overlap, in bp
+    between a and b.
+    If >0, the number of bp of overlap
+    If 0,  they are book-ended.
+    If <0, the distance in bp between them
+
+    - positive if intersect
+    - negative if not intersect
+    - zero if exqct match
+
+    ref:
+        - https://stackoverflow.com/a/52388579/1601580
+    """
+    return min(a[1], b[1]) - max(a[0], b[0])
+
+
+# -- tests
+
+def overlap_intersection_test_():
+    """
+    want to test if two intervals intersect/overlap and return true if they do
+    """
+    print('----')
+    print(f'{get_intersection_overlap([10, 25], [20, 38])}')
+    assert get_intersection_overlap([10, 25], [20, 38]) == 5
+    print(f'{get_intersection_overlap([20, 38], [10, 25])}')
+    assert get_intersection_overlap([20, 38], [10, 25]) == 5
+
+    print(f'{get_intersection_overlap([10, 15], [20, 38])}')
+    assert get_intersection_overlap([10, 15], [20, 38]) == 0
+    print(f'{get_intersection_overlap([20, 38], [10, 15])}')
+    assert get_intersection_overlap([20, 38], [10, 15]) == 0
+
+    print(f'{get_intersection_overlap([10, 15], [15, 38])}')
+    assert get_intersection_overlap([10, 15], [15, 38]) == 0
+    print(f'{get_intersection_overlap([15, 38], [10, 15])}')
+    assert get_intersection_overlap([15, 38], [10, 15]) == 0
+
+    # -
+    print('----')
+    # positive if intersect
+    print(f'{get_intersection_overlap_care_about_exact_match([10, 25], [20, 38])}')
+    assert get_intersection_overlap_care_about_exact_match([10, 25], [20, 38]) == 5
+    print(f'{get_intersection_overlap_care_about_exact_match([20, 38], [10, 25])}')
+    assert get_intersection_overlap_care_about_exact_match([20, 38], [10, 25]) == 5
+
+    # negative if not intersect
+    print(f'{get_intersection_overlap_care_about_exact_match([10, 15], [20, 38])}')
+    assert get_intersection_overlap_care_about_exact_match([10, 15], [20, 38]) == -5
+    print(f'{get_intersection_overlap_care_about_exact_match([20, 38], [10, 15])}')
+    assert get_intersection_overlap_care_about_exact_match([20, 38], [10, 15]) == -5
+
+    # zero if exqct match
+    print(f'{get_intersection_overlap_care_about_exact_match([10, 15], [15, 38])}')
+    assert get_intersection_overlap_care_about_exact_match([10, 15], [15, 38]) == 0
+    print(f'{get_intersection_overlap_care_about_exact_match([15, 38], [10, 15])}')
+    assert get_intersection_overlap_care_about_exact_match([15, 38], [10, 15]) == 0
+
+
 def draw_test():
     # import pylab
     # import matplotlib.my_pyplot as plt
     import networkx as n
     # https://stackoverflow.com/questions/20133479/how-to-draw-directed-graphs-using-networkx-in-python
     g = nx.DiGraph()
     print(f'{g.is_directed()=}')
@@ -1700,16 +2117,19 @@
     args: Namespace = get_args_from_checkpoint_json_file(path=path_to_checkpoint, filename='args.json')
     pprint_args(args)
     args: Namespace = map_args_fields_from_string_to_usable_value(args)
     print('----')
     pprint_args(args)
 
 
+# --
+
 if __name__ == '__main__':
     print('starting __main__ at __init__')
     # test_draw()
     # test_dfs()
     # test_good_progressbar()
     # xor_test()
     # merge_args_test()
-    _map_args_fields_from_string_to_usable_value_test()
+    # _map_args_fields_from_string_to_usable_value_test()
+    overlap_intersection_test_()
     print('Done!\a')
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/argparse_uu/args_tinfer.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/argparse_uu/args_tinfer.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/argparse_uu/common.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/argparse_uu/common.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,43 @@
+from copy import deepcopy
+
 import os
+import sys
 from argparse import Namespace
 from pathlib import Path
-from typing import Optional
+from typing import Optional, Union
 
 from uutils import find_free_port, load_cluster_jobids_to, try_to_get_git_revision_hash_short, \
     try_to_get_git_revision_hash_long
 
 from datetime import datetime
 
+from uutils.logging_uu.wandb_logging.common import setup_wandb
 
 def create_default_log_root(args: Namespace):
     """
     Create the default place where we save things to.
     """
-    args.log_root: Path = Path('~/data/logs/').expanduser() if not hasattr(args, 'log_root') else args.log_root
+    import random
+    # - make sure prefix $HOME/data/logs/ is in args.log_root Path
+    print(f'{args.log_root=}')
+    # args.log_root: Path = Path('~/data/logs/').expanduser() if not hasattr(args, 'log_root') else args.log_root
+    # for now always overwrite the log_root since you need to guarantee the given log_root is on the machine this process is running on.
+    args.log_root: Path = Path('~/data/logs/').expanduser()
     args.log_root: Path = Path(args.log_root).expanduser() if isinstance(args.log_root, str) else args.log_root
     args.log_root: Path = args.log_root.expanduser()
+    assert isinstance(args.log_root, Path), f'Error, it is not of type Path: {args.log_root=}'
     args.current_time = datetime.now().strftime('%b%d_%H-%M-%S')
-    args.log_root = args.log_root / f'logs_{args.current_time}_jobid_{args.jobid}'
+    # wandb_str helps to identify which wandb runs are more likely to be important (since they used wandb)
+    wandb_str: str = f'_wandb_{args.log_to_wandb}' if hasattr(args, 'log_to_wandb') else 'code_without_wandb'
+    args.PID = str(os.getpid()) if not hasattr(args, 'PID') else args.PID
+    args.jobid: int = random.randint(0, 50000) if not hasattr(args, 'jobid') else args.jobid
+    args.log_root = args.log_root / f'logs_{args.current_time}_jobid_{args.jobid}_pid_{args.PID}{wandb_str}'
     args.log_root.mkdir(parents=True, exist_ok=True)
+    print(f'{args.log_root=}')
 
 
 def setup_args_for_experiment(args: Namespace,
                               num_workers: Optional[int] = 0,
                               use_tb: bool = False  # not needed anymore since wandb exists
                               ) -> Namespace:
     """
@@ -66,14 +81,15 @@
     """
     import torch
     import logging
     import uutils
     from uutils.logger import Logger as uuLogger
 
     # - set the iteration/epoch number to start training from
+    # args.training_mode = 'iterations' if args.training_mode is None else args.training_mode
     if 'iterations' in args.training_mode:
         # set the training iteration to start from beginning or from specified value (e.g. from ckpt iteration index).
         args.it = 0 if not hasattr(args, 'it') else args.it
         assert args.it >= 0, f'Iteration to train has to be start at zero or above but got: {args.it}'
         args.epoch_num = -1
     elif 'epochs' in args.training_mode:
         # set the training epoch number to start from beginning or from specified value e.g. from ckpt epoch_num index.
@@ -115,126 +131,144 @@
     if not hasattr(args, 'augment_train'):
         args.augment_train = True if not hasattr(args, 'not_augment_train') else not args.not_augment_train
 
     # NOTE: this should be done outside cuz flags have to be declared first then parsed, args = parser.parse_args()
     if hasattr(args, 'no_validation'):
         args.validation = not args.no_validation
 
-    # - distributed params
+    # - default "empty" distributed params, for now each dist main sets up their own dist rank e.g. ddp, l2l, etc in their main
     args.rank = -1  # should be written by each worker with their rank, if not we are running serially
     args.master_port = find_free_port()
-
-    # - determinism
-    if hasattr(args, 'always_use_deterministic_algorithms'):
-        if args.always_use_deterministic_algorithms:
-            uutils.torch_uu.make_code_deterministic(args.seed)
-            logging.warning(f'Seed being ignored, seed value: {args.seed=}')
-
-    # - get device name
-    print(f'{args.seed=}')
-    # args.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
-    from uutils.torch_uu.distributed import set_devices
-    set_devices(args)  # args.device = rank or .device
-    print(f'device: {args.device}')
+    # note, currently the true distributed args are set up in the main train file/func todo: perhaps move here? might have to make cases, one for ddp, pytorch mp, one serial, one l2l...worth it?
 
     # - get cluster info (including hostname)
     load_cluster_jobids_to(args)
 
-    # - get log_root
-    # usually in options: parser.add_argument('--log_root', type=str, default=Path('~/data/logs/').expanduser())
-    create_default_log_root(args)
-    # create tb in log_root
-    if use_tb:
-        from torch.utils.tensorboard import SummaryWriter
-        args.tb_dir = args.log_root / 'tb'
-        args.tb_dir.mkdir(parents=True, exist_ok=True)
-        args.tb = SummaryWriter(log_dir=args.tb_dir)
+    # - save PID
+    args.PID = str(os.getpid())
+    print(f'{args.PID=}')
+    if torch.cuda.is_available():
+        args.nccl = torch.cuda.nccl.version()
 
-    # - setup expanded path to checkpoint
-    if hasattr(args, 'path_to_checkpoint'):
-        # str -> Path(path_to_checkpoint).expand()
-        if args.path_to_checkpoint is not None:
-            if isinstance(args.path_to_checkpoint, str):
-                args.path_to_checkpoint = Path(args.path_to_checkpoint).expanduser()
-            elif isinstance(args.path_to_checkpoint, Path):
-                args.path_to_checkpoint.expanduser()
-            else:
-                raise ValueError(f'Path to checkpoint is not of the right type: {type(args.path_to_checkpoint)=},'
-                                 f'with value: {args.path_to_checkpoint=}')
+    # - determinism?
+    print(f'Original seed from args: {args.seed=}')
+    if hasattr(args, 'always_use_deterministic_algorithms'):
+        # this does set the seed but it also does much more e.g. tries to make convs etc deterministic if possible.
+        fully_deterministic: bool = False
+        if args.always_use_deterministic_algorithms:
+            fully_deterministic: bool = uutils.torch_uu.make_code_deterministic(args.seed)
+        # todo fix, warn only if code is not fully deterministic
+        if not fully_deterministic:
+            logging.warning(f'Seed possibly being ignored, seed value: {args.seed=}')
+    # - seed only if the user chose a seed, else set a truly different seed. Reason we decided this 1. if we set the seed & make sure it's always different we can always have the code act differently 2. by always acting randomly AND choosing a seed and saving it in args it makes our code (hopefully fully reproducible, but this details about torch might not make it but at least we are trying really hard to be reproducible)
+    if args.seed != -1:  # if seed set (-1 is not set), args.seed != -1 means seed not set
+        uutils.seed_everything(args.seed)
+    else:
+        # if seed not seed then set a truly random seed, this should be different even if python is re-ran given it uses the OS
+        args.seed = uutils.get_truly_random_seed_through_os(rand_size=3)
+    print(f'Seed after code tries to setup args: {args.seed=}')
 
-    # - get device name if possible
+    # - get device name: Decided to not put it here since for now this function is not ran by each rank, but instead by the main process, so we can't get the device name here, we have to get it in the main train file/func
+    # args.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+    # from uutils.torch_uu.distributed import set_devices
+    # set_devices(args)  # args.device = rank or .device
+    # print(f'device: {args.device}')
+    # get device name if possible
     try:
         args.gpu_name = torch.cuda.get_device_name(0)
     except:
         args.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
         args.gpu_name = args.device
     print(f'\nargs.gpu_name = {args.gpu_name}\n')  # print gpu_name if available else cpu
 
-    # - save PID
-    args.PID = str(os.getpid())
-    if torch.cuda.is_available():
-        args.nccl = torch.cuda.nccl.version()
-
     # - email option (warning, not recommended! very unreliable, especially from cluster to cluster)
     # logging.warning('uutils email is not recommended! very unreliable, especially from cluster to cluster)
     # args.mail_user = 'brando.science@gmail.com'
     # args.pw_path = Path('~/pw_app.config.json').expanduser()
 
     # - try to get githash, might fail and return error string in field but whatever
     args.githash: str = try_to_get_git_revision_hash_short()
     args.githash_short: str = try_to_get_git_revision_hash_short()
     args.githash_long: str = try_to_get_git_revision_hash_long()
 
     # - get my logger, its set at the agent level
     args.logger: uuLogger = uutils.logger.Logger(args)
 
+    # - get log_root
+    # usually in options: parser.add_argument('--log_root', type=str, default=Path('~/data/logs/').expanduser())
+    create_default_log_root(args)
+
+    # - get bar
+    from uutils.torch_uu.training.common import get_trainer_progress_bar
+    args.bar = get_trainer_progress_bar(args)
+
     # - best val loss
     args.best_val_loss: float = float('inf')
 
-    # - wandb
+    # -- wandb.  note, nice safety property of my logging when it does log to wandb it always checks rank.
     if hasattr(args, 'log_to_wandb'):
         if not hasattr(args, 'dist_option'):  # backwards compatibility, if no dist_option just setup wandb as "normal"
+            # read above 2 comments and one bellow
             setup_wandb(args)
-        elif args.dist_option != 'l2l_dist':
-            #  in this case wandb has to be setup in the train code, since it's not being ran with ddp, instead the
-            # script itself is distributed and pytorch manages it (i.e. pytorch torch.distributed.run manages the
-            # mp.spawn or spwaning processes somehow.
-            pass
+        else:  # hasattr(args, 'dist_option')
+            # todo this might be set up cleaner if we setup args in this function and not in main train
+            # if custom dist_option needed then we might need more careful starting & setting up wandb e.g. if multiple python processes are used
+            if args.dist_option != 'l2l_dist':
+                # todo this might be set up cleaner if we setup args in this function and not in main train
+                # in this case wandb has to be setup in the train code, since it's not being ran with ddp, instead the
+                # script itself is distributed and pytorch manages it i.e. pytorch torch.distributed.run manages the
+                # mp.spawn or spwaning processes somehow.
+                pass
+            elif args.dist_option == 'l2l_dist':
+                # todo this might be set up cleaner if we setup args in this function and not in main train
+                # setup of wandb is done in main train after args.rank is set up properly,
+                pass
+        # # - set up wandb
+        # # thought this was justified to ignore above since the main (singe) python process sets up wandb once and then the spawned processes always check their rank before logging to wandb
+        # # BUT, due to multiple python process thing in the != l2l_dist it might mean this setsup wandb multiple times, so main or train code needs to check rank to avoid this
+        # ### WARNING, don't use in this func, see l2l_dist case, setup_wandb(args)  # already checks args.log_to_wandb inside of it
+
     # - for debugging
     # args.environ = [str(f'{env_var_name}={env_valaue}, ') for env_var_name, env_valaue in os.environ.items()]
 
     # - to avoid pytorch multiprocessing issues with CUDA: https://pytorch.org/docs/stable/data.html
     args.pin_memory = False
     args.num_workers = num_workers if num_workers is not None else args.num_workers
 
+    # - run re-auth if in stanford cluster
+    from socket import gethostname
+    if 'stanford' in gethostname():
+        # bellow commented out because this was used for nohup but we aren't doing nohup anymore
+        # print(f'In stanford hostname: {gethostname()=}, about to do stanford reauth in python')
+        # from uutils import stanford_reauth
+        # stanford_reauth()
+        # print(f'finished calling stanford reauth inside python')
+        pass
+
+    # create tb in log_root
+    if use_tb:
+        from torch.utils.tensorboard import SummaryWriter
+        args.tb_dir = args.log_root / 'tb'
+        args.tb_dir.mkdir(parents=True, exist_ok=True)
+        args.tb = SummaryWriter(log_dir=args.tb_dir)
+
+    # - setup expanded path to checkpoint
+    if hasattr(args, 'path_to_checkpoint'):
+        # str -> Path(path_to_checkpoint).expand()
+        if args.path_to_checkpoint is not None:
+            if isinstance(args.path_to_checkpoint, str):
+                args.path_to_checkpoint = Path(args.path_to_checkpoint).expanduser()
+            elif isinstance(args.path_to_checkpoint, Path):
+                args.path_to_checkpoint.expanduser()
+            else:
+                raise ValueError(f'Path to checkpoint is not of the right type: {type(args.path_to_checkpoint)=},'
+                                 f'with value: {args.path_to_checkpoint=}')
+
+    # - save os.environ
+    # make a deep copy of os.environ
+    # args.environ = deepcopy(dict(os.environ))
+    args.CUDA_VISIBLE_DEVICES = os.environ.get('CUDA_VISIBLE_DEVICES', None)
+
     # - return
     uutils.print_args(args)
     uutils.save_args(args)
     return args
-
-
-def setup_wandb(args: Namespace):
-    if args.log_to_wandb:
-        # os.environ['WANDB_MODE'] = 'offline'
-        import wandb
-        print(f'{wandb=}')
-
-        # - set run name
-        run_name = None
-        # if in cluster use the cluster jobid
-        if hasattr(args, 'jobid'):
-            # if jobid is actually set to something, use that as the run name in ui
-            if args.jobid is not None and args.jobid != -1 and str(args.jobid) != '-1':
-                run_name: str = f'jobid={str(args.jobid)}'
-        # if user gives run_name overwrite that always
-        if hasattr(args, 'run_name'):
-            run_name = args.run_name if args.run_name is not None else run_name
-        args.run_name = run_name
-        # - initialize wandb
-        wandb.init(project=args.wandb_project,
-                   entity=args.wandb_entity,
-                   # job_type="job_type",
-                   name=run_name,
-                   group=args.experiment_name
-                   )
-        # - save args in wandb
-        wandb.config.update(args)
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/argparse_uu/meta_learning.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/mains/main_tree_nn.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,238 +1,307 @@
-from argparse import Namespace
-from pathlib import Path
-
-from torch import nn
-
-from uutils import load_cluster_jobids_to
-
-
-def fix_for_backwards_compatibility(args: Namespace) -> Namespace:
-    args.meta_batch_size_train = args.batch_size
-    args.meta_batch_size_eval = args.batch_size_eval
+#!/home/miranda9/miniconda3/envs/automl-meta-learning/bin/python
 
-    args.log_train_freq = args.log_freq
-    args.log_val_freq = args.log_freq
+"""
+main file for train models with SL for prediticing hashes
 
-    # - unsure if to remove
-    args.eval_iters = 1
+python main_training_sl_predict_hash.py --no_validation --exp_id test1
 
-    args.outer_lr = args.lr
-    args.n_classes = args.n_cls
-    return args
+"""
+from pdb import set_trace as st
+import os
+import sys
+
+from socket import gethostname
+
+from datetime import datetime
+
+# pprint(sys.path)
+import torch
+import torch.nn as nn
+import torch.multiprocessing as mp
+
+from data_lib.dag.dag_dataloader import get_dataloader_from_dag_files, get_dataloader_from_dag_files_syn_sem, test_dag_syn_sem
+from data_lib.dataloader_hash_dataset import get_distributed_dataloader_from_feat_file
+from progressbar import ProgressBar
+from uutils import save_opts, load_cluster_jobids_to, set_system_wide_force_flush
+from uutils.torch_uu import print_dict_of_dataloaders_dataset_types
+from uutils.torch_uu.distributed import setup_process, cleanup, set_sharing_strategy, move_to_ddp, find_free_port, \
+    clean_end_with_sigsegv_hack, is_lead_worker, is_running_serially, \
+    print_process_info, set_devices, is_running_parallel
+from torch.optim.lr_scheduler import ReduceLROnPlateau
+
+# ML4Coq
+from agents import HashPredictorAgent
+from embeddings_zoo.tactic_predictor import get_tree_nn_tactic_predictor_hash_predictor, \
+    get_tree_nn_tactic_predictor_hash_predictor_dag_dataset
 
+import numpy as np
+from numpy import random
 
-def parse_args_meta_learning() -> Namespace:
-    """
-    WARNING: SOME NAMES MIGHT HAVE COPIES TO MAKE THINGS BACKWARD COMPATIBLE.
+from pathlib import Path
 
-    Parse the arguments from the terminal so that the experiment runs as the user specified there.
 
-    Example/Recommended pattern to use:
-        See setup_args_for_experiment(...) to avoid copy pasting example/only mantain it in one place.
+sys.stdout.flush()  # no delay in print statements
 
-    Note:
-        - Strongly recommended to see setup_args_for_experiment(...)
-    """
+def parse_args():
     import argparse
-    # import torch.nn as nn
 
     parser = argparse.ArgumentParser()
 
-    # -- create argument options
+    # parser.add_argument('--tac_grammar', type=str, default=Path('/ml4coq-proj-src/embeddings_zoo/tactic_decoders/tactics.ebnf').expanduser())
+
+    # experimental setup
     parser.add_argument('--debug', action='store_true', help='if debug')
-    # parser.add_argument('--serial', action='store_true', help='if running serially')
-    parser.add_argument('--parallel', action='store_true', help='if running in parallel')
+    parser.add_argument('--serial', action='store_true', help='if running serially')
+    # parser.add_argument('--include_synthetic', action='store_true')
+    parser.add_argument('--exp_id', type=str, default='exp id:')
+    # - data set arguments
+    # dag
+    # we only need the path to dag_dat_prep since that contains the paths to the train, val, test splits
+    parser.add_argument('--path2dataprep', type=str, default=Path("~/data/lasse_datasets_coq/split_dag_data_prep.pt").expanduser())
+    parser.add_argument('--path2vocabs', type=str, default=Path('~/data/lasse_datasets_coq/dag_counters.pt').expanduser())
+    parser.add_argument('--path2hash2idx', type=str, default=Path('~/data/lasse_datasets_coq/dag_hash2index.pt').expanduser())
+
+    parser.add_argument('--mode', type=str, default='syntactic')
+    parser.add_argument('--split', type=str, default='train', help='dont train on val or test. This flag is mainly '
+                                                                   'for the options "train" and "test_debug".')
 
-    # - path to log_root
     parser.add_argument('--log_root', type=str, default=Path('~/data/logs/').expanduser())
 
-    # - training options
-    parser.add_argument('--training_mode', type=str, default='epochs_train_convergence',
-                        help='valid/possible values: '
-                             'fit_single_batch'
-                             'iterations'
-                             'epochs'
-                             'iterations_train_convergence'
-                             'epochs_train_convergence'
-                             '- Note: since the code checkpoints the best validation model anyway, it is already doing'
-                             'early stopping, so early stopping criterion is not implemented. You can kill the job'
-                             'if you see from the logs in wanbd that you are done.'
-                        )
-    parser.add_argument('--num_epochs', type=int, default=-1)
-    parser.add_argument('--num_its', type=int, default=-1)
-    # parser.add_argument('--no_validation', action='store_true', help='no validation is performed')
-    parser.add_argument('--train_convergence_patience', type=int, default=5, help='How long to wait for converge of'
-                                                                                  'training. Note this code should'
-                                                                                  'be saving the validation ckpt'
-                                                                                  'so you are automatically doing '
-                                                                                  'early stopping already.')
-    # model & loss function options
-    parser.add_argument('--model_option',
-                        type=str,
-                        default="5CNN_opt_as_model_for_few_shot_sl",
-                        help="Options: e.g."
-                             "5CNN_opt_as_model_for_few_shot_sl"
-                             "resnet12_rfs"
-                        )
-    parser.add_argument('--loss', type=str, help='loss/criterion', default=nn.CrossEntropyLoss())
+    parser.add_argument('--num_epochs', type=int, default=100)
+    parser.add_argument('--resume_path', type=str, default='', help='the path for model checkpoint to resume')
+    parser.add_argument('--no_validation', action='store_true', help='no validation is performed')
+    # parser.add_argument('--save_model_epochs', type=int, default=10, help='the number of epochs between model savings')
+    parser.add_argument('--num_workers', type=int, default=0, help='the number of data_lib-loading threads (when running serially')
+    parser.add_argument('--smoke', action='store_true')
+    parser.add_argument('--seed', type=int, default=0)
+    parser.add_argument('--ckpt_freq_in_hours', type=int, default=6)
+    parser.add_argument('--filter', type=str)
+
+    # term encoder
+    parser.add_argument('--term_encoder_embedding_dim', type=int, default=256)
+
+    # tactic label classifier
+    # parser.add_argument('--size_limit', type=int, default=50)
+    # parser.add_argument('--embedding_dim_decoder', type=int, default=256, help='dimension of the grammar embeddings')
+    # parser.add_argument('--symbol_dim', type=int, default=256, help='dimension of the terminal/nonteaarminal symbol embeddings')
+    # parser.add_argument('--hidden_dim', type=int, default=256, help='dimension of the LSTM controller')
+    # parser.add_argument('--teacher_forcing', type=float, default=1.0)
+    parser.add_argument('--criterion', type=str, help='loss criterion', default=nn.CrossEntropyLoss())
 
     # optimization
-    parser.add_argument('--opt_option', type=str, default='AdafactorDefaultFair')
-    parser.add_argument('--lr', type=float, default=None, help='Warning: use a learning rate according to'
-                                                               'how previous work trains your model.'
-                                                               'Otherwise, tuning might be needed.'
-                                                               'Vision resnets usually use 1e-3'
-                                                               'and transformers have a smaller'
-                                                               'learning 1e-4 or 1e-5.'
-                                                               'It might be a good start to have the'
-                                                               'Adafactor optimizer with lr=None and'
-                                                               'a its defualt scheduler called'
-                                                               'every epoch or every '
-                                                               '1(1-beta_2)^-1=2000 iterations.'
-                                                               'Doing a hp search with with wanbd'
-                                                               'a good idea.')
-    parser.add_argument('--grad_clip_mode', type=str, default=None)
-    parser.add_argument('--num_warmup_steps', type=int, default=-1)
-    parser.add_argument('--scheduler_option', type=str, default='AdafactorSchedule', help='Its strongly recommended')
-    parser.add_argument('--log_scheduler_freq', type=int, default=-1, help='default is to put the epochs or iterations '
-                                                                           'default either log every epoch or log ever '
-                                                                           '~100 iterations.')
-
-    # - data set args
-    parser.add_argument('--batch_size', type=int, default=4)
-    parser.add_argument('--batch_size_eval', type=int, default=2)
-    parser.add_argument('--split', type=str, default='train', help="possible values: "
-                                                                   "'train', val', test'")
-    # warning: sl name is path_to_data_set here its data_path
-    parser.add_argument('--data_option', type=str, default='None')
-    parser.add_argument('--data_path', type=str, default=None)
-    # parser.add_argument('--data_path', type=str, default='torchmeta_miniimagenet',
-    #                     help='path to data set splits. The code will assume everything is saved in'
-    #                          'the uutils standard place in ~/data/, ~/data/logs, etc. see the setup args'
-    #                          'setup method and log_root.')
-    # parser.add_argument('--path_to_data_set', type=str, default='None')
-    parser.add_argument('--data_augmentation', type=str, default=None)
-    parser.add_argument('--not_augment_train', action='store_false', default=True)
-    parser.add_argument('--augment_val', action='store_true', default=True)
-    parser.add_argument('--augment_test', action='store_true', default=False)
-    # parser.add_argument('--l2', type=float, default=0.0)
-
-    # - checkpoint options
-    parser.add_argument('--path_to_checkpoint', type=str, default=None, help='the path to the model checkpoint to '
-                                                                             'resume training.'
-                                                                             'e.g. path: '
-                                                                             '~/data_folder_fall2020_spring2021/logs/nov_all_mini_imagenet_expts/logs_Nov05_15-44-03_jobid_668/ckpt.pt')
-    parser.add_argument('--ckpt_freq', type=int, default=-1)
-
-    # - dist/distributed options
-    parser.add_argument('--init_method', type=str, default=None)
-
-    # - miscellaneous arguments
-    parser.add_argument('--log_freq', type=int, default=-1, help='default is to put the epochs or iterations default'
-                                                                 'either log every epoch or log ever ~100 iterations')
-    parser.add_argument('--seed', type=int, default=0)
-    parser.add_argument('--always_use_deterministic_algorithms', action='store_true',
-                        help='tries to make pytorch fully deterministic')
-    parser.add_argument('--num_workers', type=int, default=-1,
-                        help='the number of data_lib-loading threads (when running serially')
-    parser.add_argument('--pin_memory', action='store_true', default=False, help="Using pinning is an"
-                                                                                 "advanced tip according to"
-                                                                                 "pytorch docs, so will "
-                                                                                 "leave it False as default"
-                                                                                 "use it at your own risk"
-                                                                                 "of further debugging and"
-                                                                                 "spending time on none"
-                                                                                 "essential, likely over"
-                                                                                 "optimizing. See:"
-                                                                                 "https://pytorch.org/docs/stable/notes/cuda.html#cuda-memory-pinning")
-    parser.add_argument('--log_to_tb', action='store_true', help='store to weights and biases')
-
-    # - wandb
-    parser.add_argument('--log_to_wandb', action='store_true', help='store to weights and biases')
-    parser.add_argument('--wandb_project', type=str, default='meta-learning-playground')
-    parser.add_argument('--wandb_entity', type=str, default='brando')
-    # parser.add_argument('--wandb_project', type=str, default='test-project')
-    # parser.add_argument('--wandb_entity', type=str, default='brando-uiuc')
-    parser.add_argument('--wandb_group', type=str, default='experiment_debug', help='helps grouping experiment runs')
-    # parser.add_argument('--wandb_log_freq', type=int, default=10)
-    # parser.add_argument('--wandb_ckpt_freq', type=int, default=100)
-    # parser.add_argument('--wanbd_mdl_watch_log_freq', type=int, default=-1)
-
-    # - manual loads
-    parser.add_argument('--manual_loads_name', type=str, default='None')
-
-    # - meta-learner specific
-    parser.add_argument('--k_shots', type=int, default=5, help="")
-    parser.add_argument('--k_eval', type=int, default=15, help="")
-    parser.add_argument('--n_cls', type=int, default=5, help="")  # n_ways
-    parser.add_argument('--n_aug_support_samples', type=int, default=1,
-                        help="The puzzling rfs increase in support examples")
-
-    # - parse arguments
-    args = parser.parse_args()
-    args.criterion = args.loss
-    assert args.criterion is args.loss
-    # - load cluster ids so that wandb can use it later for naming runs, experiments, etc.
-    load_cluster_jobids_to(args)
-    return args
-
-
-# def parse_option_rfs():
-#     """
-#
-#     ref: https://github.com/WangYueFt/rfs/blob/f8c837ba93c62dd0ac68a2f4019c619aa86b8421/eval_fewshot.py#L24
-#     """
-#     from models import model_dict, model_pool
-#     from models.util import create_model
-#
-#     hostname = socket.gethostname()
-#
-#     parser = argparse.ArgumentParser('argument for training')
-#
-#     # load pretrained model
-#     parser.add_argument('--model', type=str, default='resnet12', choices=model_pool)
-#     parser.add_argument('--model_path', type=str, default=None, help='absolute path to .pth model')
-#
-#     # dataset
-#     parser.add_argument('--dataset', type=str, default='miniImageNet', choices=['miniImageNet', 'tieredImageNet',
-#                                                                                 'CIFAR-FS', 'FC100'])
-#     parser.add_argument('--transform', type=str, default='A', choices=transforms_list)
-#
-#     # meta setting
-#     parser.add_argument('--n_test_runs', type=int, default=600, metavar='N',
-#                         help='Number of test runs')
-#     parser.add_argument('--n_ways', type=int, default=5, metavar='N',
-#                         help='Number of classes for doing each classification run')
-#     parser.add_argument('--n_shots', type=int, default=1, metavar='N',
-#                         help='Number of shots in test')
-#     parser.add_argument('--n_queries', type=int, default=15, metavar='N',
-#                         help='Number of query in test')
-#     parser.add_argument('--n_aug_support_samples', default=5, type=int,
-#                         help='The number of augmented samples for each meta test sample')
-#     parser.add_argument('--data_root', type=str, default='data', metavar='N',
-#                         help='Root dataset')
-#     parser.add_argument('--num_workers', type=int, default=3, metavar='N',
-#                         help='Number of workers for dataloader')
-#     parser.add_argument('--test_batch_size', type=int, default=1, metavar='test_batch_size',
-#                         help='Size of test batch)')
-#
-#     opt = parser.parse_args()
-#
-#     if 'trainval' in opt.model_path:
-#         opt.use_trainval = True
-#     else:
-#         opt.use_trainval = False
-#
-#     # set the path according to the environment
-#     if hostname.startswith('visiongpu'):
-#         opt.data_root = '/data/vision/phillipi/rep-learn/{}'.format(opt.dataset)
-#         opt.data_aug = True
-#     elif hostname.startswith('instance'):
-#         opt.data_root = '/mnt/globalssd/fewshot/{}'.format(opt.dataset)
-#         opt.data_aug = True
-#     elif opt.data_root != 'data':
-#         opt.data_aug = True
-#     else:
-#         raise NotImplementedError('server invalid: {}'.format(hostname))
-#
-#     return opt
+    parser.add_argument('--optimizer', type=str, default='Adam')
+    parser.add_argument('--learning_rate', type=float, default=1e-3)
+    # parser.add_argument('--momentum', type=float, default=0.9)
+    # parser.add_argument('--batchsize', type=int, default=128)
+    parser.add_argument('--batch_size', type=int, default=128)
+    # parser.add_argument('--l2', type=float, default=1e-6)
+    parser.add_argument('--l2', type=float, default=0.0)
+    parser.add_argument('--lr_reduce_patience', type=int, default=10)
+    parser.add_argument('--lr_reduce_steps', default=3, type=int,
+                        help='the number of steps before reducing the learning rate \
+                        (only applicable when no_validation == True)')
+
+    # debugging flags
+    parser.add_argument('--train_set_length', type=int, default=236_436)
+
+    opts = parser.parse_args()
+
+    # to have checkpointing work every 6 hours.
+    opts.start = time.time()
+    opts.next_time_to_ckpt_in_hours = 0.0
+
+    opts.validation = not opts.no_validation
+
+    # distributed params
+    opts.rank = -1  # should be written by each worker with their rank, if not we are running serially
+    opts.master_port = find_free_port()
+
+    # TODO IMPROVE THIS
+    torch.manual_seed(opts.seed)
+    torch.backends.cudnn.deterministic = True
+    torch.backends.cudnn.benchmark = False
+    np.random.seed(opts.seed)
+    random.seed(opts.seed)
+    opts.device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+    print(f'device: {opts.device}')
+
+    load_cluster_jobids_to(opts)
+    opts.current_time = datetime.now().strftime('%b%d_%H-%M-%S')
+    opts.log_root = opts.log_root / f'logs_{opts.current_time}_jobid_{opts.jobid}'
+    opts.log_root.mkdir(parents=True, exist_ok=True)
+    opts.tb_dir = opts.log_root / 'tb'
+    opts.tb_dir.mkdir(parents=True, exist_ok=True)
+
+    # annealing learning rate is only applicable when data_lib set is train TODO figure out later
+    if (not opts.no_validation) and (opts.lr_reduce_steps is not None):
+        print('--lr_reduce_steps is applicable only when no_validation == True', 'ERROR')
+
+    # get device name if possible
+    try:
+        opts.gpu_name = torch.cuda.get_device_name(0)
+        print(f'\nopts.gpu_name = {opts.gpu_name}\n')
+    except:
+        opts.gpu_name = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+
+    opts.PID = str(os.getpid())
+    if torch.cuda.is_available():
+        opts.nccl = torch.cuda.nccl.version()
+    return opts
+
+def load_checkpoint(opts, optimizer, model):
+    start_epoch = 0
+    if opts.resume_path != '':  # if the path is not empty then there is a model checkpoint
+        if opts.device.type == 'cpu':
+            checkpoint = torch.load(opts.resume, map_location='cpu')
+        else:  # use GPU
+            checkpoint = torch.load(opts.resume)
+        model.load_state_dict(checkpoint['state_dict'])
+        optimizer.load_state_dict(checkpoint['optimizer'])
+        start_epoch = checkpoint['n_epoch'] + 1
+        model.to(opts.device)
+    if is_running_parallel(opts.rank):  # halt all processes until everyone has loaded checkpoint
+        torch.distributed.barrier()
+    return start_epoch
+
+def main_distributed():
+    """
+    train tree_nn in parallel
+
+    Note: end-to-end ddp example on mnist: https://yangkky.github.io/2019/07/08/distributed-pytorch-tutorial.html
+    :return:
+    """
+    # parse the options
+    opts = parse_args()
+    [print(f'{k,v}') for k, v in vars(opts).items()]
+
+    # parallel train
+    if torch.cuda.is_available():
+        opts.world_size = torch.cuda.device_count()
+        print(f"{torch.cuda.device_count()=}")
+    elif opts.serial:
+        opts.world_size = 1
+        print('RUNNING SERIALLY')
+    else:
+        # opts.world_size = mp.cpu_count() - 1  # 1 process is main, the rest are (parallel) trainers
+        opts.world_size = 4
+
+    # spawn the distributed training code
+    print(f'\n{opts.world_size=}')
+    save_opts(opts)
+    if opts.serial:
+        print('RUNNING SERIALLY')
+        train(rank=-1, opts=opts)
+    else:
+        print('\nABOUT TO SPAWN WORKERS')
+        # mp.set_sharing_strategy('file_system')
+        set_sharing_strategy()
+        print('done setting sharing strategy...next mp.spawn')
+        mp.spawn(fn=train, args=(opts,), nprocs=opts.world_size)
+        print('done mp.spwan')
+
+def train(rank, opts):
+    print_process_info(rank, flush=True)
+    # have each process save the rank
+    opts.rank = rank
+    set_devices(opts)  # basically opts.gpu = rank if not debugging/serially
+    # setup up worker
+    setup_process(opts, rank, master_port=opts.master_port, world_size=opts.world_size)
+    print(f'setup process done for rank={rank}')
+
+    # create the dataloaders
+    # dataloaders = get_distributed_dataloader_from_feat_file(opts, rank, opts.world_size)
+    # dataloaders = get_dataloader_from_dag_files(opts, opts.rank, opts.world_size)
+    dataloaders = get_dataloader_from_dag_files_syn_sem(opts, opts.rank, opts.world_size, opts.mode)
+    if is_lead_worker(rank):
+        print_dict_of_dataloaders_dataset_types(dataloaders)
+        # [print_dataloaders_info(opts, dataloaders, split) for split, _ in dataloaders.items()]
+
+    # create the model (TE + Decoder)
+    # tactic_predictor = get_tree_nn_tactic_predictor_hash_predictor(opts)
+    tactic_predictor = get_tree_nn_tactic_predictor_hash_predictor_dag_dataset(opts)
+    tactic_predictor = move_to_ddp(rank, opts, tactic_predictor)
+
+    # TODO figure out dist checkpointing later
+    # start_epoch = load_checkpoint(opts, optimizer, tactic_predictor)
+    start_epoch = 0
+
+    # create the optimizer
+    # optimizer = torch_uu.optim.SGD(tactic_predictor.parameters(), lr=opts.learning_rate, momentum=opts.momentum, weight_decay=opts.l2)
+    optimizer = torch.optim.Adam(tactic_predictor.parameters(), lr=opts.learning_rate, weight_decay=opts.l2)
+
+    # Agent does everything, proving, training, evaluate etc.
+    agent = HashPredictorAgent(tactic_predictor, optimizer, dataloaders, opts)
+
+    # decay/anneal learning rate wrt epochs
+    if opts.no_validation:  # only train set
+        # use a fix step scheduler, decays the learning rate of each parameter group by gamma every step_size epochs.
+        # scheduler = StepLR(optimizer, step_size=opts.lr_reduce_steps, gamma=0.1)
+        # for now if only train lets overfit to train_loss
+        scheduler = ReduceLROnPlateau(optimizer, patience=opts.lr_reduce_patience, verbose=True)  # temporary
+    else:  # decay learning rate when validation loss got stuck
+        # scheduler that decays if stuck on a plateu
+        scheduler = ReduceLROnPlateau(optimizer, patience=opts.lr_reduce_patience, verbose=True)
+
+    # -- Start Training Loop
+    agent.log('====> about to start train loop')
+    # train_loop(opts, agent, scheduler, start_epoch)
+    train_loop_test(opts, agent, scheduler, start_epoch)
+    # agent.train_single_batch()
+
+    # -- Clean Up Distributed Processes
+    print(f'\n----> about to cleanup worker with rank {rank}')
+    cleanup(rank)
+    print(f'clean up done successfully! {rank}')
+
+def train_loop(opts, agent, scheduler, start_epoch):
+    agent.log('Starting training...')
+    for n_epoch in range(start_epoch, start_epoch + opts.num_epochs):
+        opts.num_epoch = n_epoch
+        # training
+        train_loss, train_acc = agent.train(n_epoch)
+        agent.log_train_stats(n_epoch, train_loss, train_acc, val_iterations=0, val_ckpt=True)
+        agent.save(n_epoch)
+
+        # validation
+        # if opts.validation:
+        #     val_loss, val_acc = agent.valid(n_epoch)
+        # anneal the learning rate
+        # if opts.no_validation:
+        #     # scheduler.step()  # fix step scheduler
+        #     scheduler.step(train_loss)
+        # else:  # use the validation loss to anneal
+        #     scheduler.step(val_loss)
+    agent.log('-------> done training!')
+
+def train_loop_test(opts, agent, scheduler, start_epoch):
+    set_system_wide_force_flush()
+    agent.print_dataloaders_info(opts.split)
+    agent.log('Starting training...')
+    opts.it = 0
+    opts.n_epoch = 0
+    # train_loss, train_acc = agent.predict_tactic_hashes(prediction_mode='train')
+    while True:
+        train_loss, train_acc = agent.train_test_debug(opts.split)
+        agent.save_every_x(opts.n_epoch)  # saves ckpt every 6 hours
+        scheduler.step(train_loss)
+
+        # if train_acc >= 1.0 and train_loss <= 0.01:
+        if train_acc >= 1.0:
+            agent.log_train_stats(opts.it, train_loss, train_acc, val_ckpt=True)
+            agent.save(opts.n_epoch)
+            opts.n_epoch += 1
+            break  # halt once both the accuracy is high enough AND train loss is low enough
+        opts.n_epoch += 1
+
+    agent.log(f'-------> done training at {opts.n_epoch=} and {opts.it=}')
+
+if __name__ == '__main__':
+    import time
+    # start script
+    start = time.time()
+    print(f'-----> device = {torch.device("cuda" if torch.cuda.is_available() else "cpu")}\n')
+    main_distributed()
+    duration_secs = time.time() - start
+    print(f"time passed: hours:{duration_secs / (60 ** 2)}, minutes={duration_secs / 60}, seconds={duration_secs}")
+    print(f'\n---> hostname: {gethostname()}')
+    print('DONE!!!\a')
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/argparse_uu/supervised_learning.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/argparse_uu/supervised_learning.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,51 +1,57 @@
+import logging
 from argparse import Namespace
 from pathlib import Path
 from typing import Optional
 
 import torch
 from torch import nn
+from torch.nn import *
 
-from uutils import load_cluster_jobids_to, merge_args
+# later, doesn't let me do
+
+from uutils import load_cluster_jobids_to, merge_args, expanduser
+
+from pdb import set_trace as st
 
 
 def parse_args_standard_sl() -> Namespace:
     import argparse
 
     # - great terminal argument parser
     parser = argparse.ArgumentParser()
 
     # -- create argument options
-    parser.add_argument('--debug', action='store_true', help='if debug')
-    # parser.add_argument('--serial', action='store_true', help='if running serially')
-    parser.add_argument('--parallel', action='store_true', help='if running in parallel')
+    parser.add_argument('--debug', action='store_true', help='if debug', default=False)
+    # parser.add_argument('--serial', action='store_true', help='if running serially', default=False)
+    parser.add_argument('--parallel', action='store_true', help='if running in parallel', default=False)
 
     # - path to log_root
     parser.add_argument('--log_root', type=str, default=Path('~/data/logs/').expanduser())
 
     # - training options
-    parser.add_argument('--training_mode', type=str, default='epochs_train_convergence',
+    parser.add_argument('--training_mode', type=str, default='iterations',
                         help='valid/possible values: '
                              'fit_single_batch'
                              'iterations'
                              'epochs'
                              'iterations_train_convergence'
                              'epochs_train_convergence'
                              '- Note: since the code checkpoints the best validation model anyway, it is already doing'
                              'early stopping, so early stopping criterion is not implemented. You can kill the job'
                              'if you see from the logs in wanbd that you are done.'
                         )
     parser.add_argument('--num_epochs', type=int, default=-1)
     parser.add_argument('--num_its', type=int, default=-1)
     # parser.add_argument('--no_validation', action='store_true', help='no validation is performed')
     parser.add_argument('--train_convergence_patience', type=int, default=10, help='How long to wait for converge of'
-                                                                                  'training. Note this code should'
-                                                                                  'be saving the validation ckpt'
-                                                                                  'so you are automatically doing '
-                                                                                  'early stopping already.')
+                                                                                   'training. Note this code should'
+                                                                                   'be saving the validation ckpt'
+                                                                                   'so you are automatically doing '
+                                                                                   'early stopping already.')
 
     # model & loss function options
     parser.add_argument('--model_option',
                         type=str,
                         default="5CNN_opt_as_model_for_few_shot_sl",
                         help="Options: e.g."
                              "5CNN_opt_as_model_for_few_shot_sl"
@@ -76,21 +82,25 @@
                                                                            '~100 iterations.')
 
     # - data set args
     parser.add_argument('--batch_size', type=int, default=128)
     parser.add_argument('--batch_size_eval', type=int, default=128)
     parser.add_argument('--split', type=str, default='train', help="possible values: "
                                                                    "'train', val', test'")
-    parser.add_argument('--data_path', type=str, default=Path('~/data/mnist/').expanduser(),
+
+    parser.add_argument('--data_option', type=str, default='mds',
+                        help='data option, make sure you set data_path and data_augmentation')
+    parser.add_argument('--data_path', type=str, default=Path('~/data/mds/records/').expanduser(),
+                        # Path('~/data/mnist/').expanduser()
                         help='path to data set splits. The code will assume everything is saved in'
                              'the uutils standard place in ~/data/, ~/data/logs, etc. see the setup args'
                              'setup method and log_root.')
     parser.add_argument('--data_augmentation', type=str, default=None)
     parser.add_argument('--not_augment_train', action='store_false', default=True)
-    parser.add_argument('--augment_val', action='store_true', default=True)
+    parser.add_argument('--augment_val', action='store_true', default=False)
     parser.add_argument('--augment_test', action='store_true', default=False)
     # parser.add_argument('--l2', type=float, default=0.0)
 
     # - checkpoint options
     parser.add_argument('--path_to_checkpoint', type=str, default=None, help='the path to the model checkpoint to '
                                                                              'resume training.'
                                                                              'e.g. path: '
@@ -99,47 +109,118 @@
 
     # - dist/distributed options
     parser.add_argument('--init_method', type=str, default=None)
 
     # - miscellaneous arguments
     parser.add_argument('--log_freq', type=int, default=-1, help='default is to put the epochs or iterations default'
                                                                  'either log every epoch or log ever ~100 iterations')
-    parser.add_argument('--seed', type=int, default=0)
+    parser.add_argument('--seed', type=int, default=-1)
     parser.add_argument('--always_use_deterministic_algorithms', action='store_true',
-                        help='tries to make pytorch fully deterministic')
+                        help='tries to make pytorch fully deterministic', default=False)
     parser.add_argument('--num_workers', type=int, default=-1,
                         help='the number of data_lib-loading threads (when running serially')
     parser.add_argument('--pin_memory', action='store_true', default=False, help="Using pinning is an"
                                                                                  "advanced tip according to"
                                                                                  "pytorch docs, so will "
                                                                                  "leave it False as default"
                                                                                  "use it at your own risk"
                                                                                  "of further debugging and"
                                                                                  "spending time on none"
                                                                                  "essential, likely over"
                                                                                  "optimizing. See:"
                                                                                  "https://pytorch.org/docs/stable/notes/cuda.html#cuda-memory-pinning")
-    parser.add_argument('--log_to_tb', action='store_true', help='store to weights and biases')
+    parser.add_argument('--log_to_tb', action='store_true', help='store to weights and biases', default=False)
+
+    # - stat analysis
+    parser.add_argument('--stats_analysis_option', type=str,
+                        default='stats_analysis_with_emphasis_on_effect_size_and_and_full_performance_comp')
 
     # - wandb
-    parser.add_argument('--log_to_wandb', action='store_true', help='store to weights and biases')
+    parser.add_argument('--log_to_wandb', action='store_true', help='store to weights and biases', default=False)
     parser.add_argument('--wandb_project', type=str, default='meta-learning-playground')
     parser.add_argument('--wandb_entity', type=str, default='brando')
     # parser.add_argument('--wandb_project', type=str, default='test-project')
     # parser.add_argument('--wandb_entity', type=str, default='brando-uiuc')
     parser.add_argument('--wandb_group', type=str, default='experiment_debug', help='helps grouping experiment runs')
     # parser.add_argument('--wandb_log_freq', type=int, default=10)
     # parser.add_argument('--wandb_ckpt_freq', type=int, default=100)
     # parser.add_argument('--wanbd_mdl_watch_log_freq', type=int, default=-1)
 
     # - manual loads
     parser.add_argument('--manual_loads_name', type=str, default='None')
 
+    # - 5CNN args
+    parser.add_argument('--filter_size', type=int, default=-1, help="Filter size for 5CNN.")
+
+    # ========MDS args 1/25=========#
+    parser.add_argument('--image_size', type=int, default=84,
+                        help='Images will be resized to this value')
+    # mscoco and traffic sign are val only
+    parser.add_argument('--sources', nargs="+",
+                        default=['ilsvrc_2012', 'aircraft', 'cu_birds', 'dtd', 'fungi', 'omniglot',
+                                 'quickdraw', 'vgg_flower', 'traffic_sign'],
+                        help='List of datasets to use')
+
+    parser.add_argument('--train_transforms', nargs="+", default=['random_resized_crop', 'random_flip'],
+                        help='Transforms applied to training data', )
+
+    parser.add_argument('--test_transforms', nargs="+", default=['resize', 'center_crop'],
+                        help='Transforms applied to test data', )
+
+    parser.add_argument('--shuffle', type=bool, default=True,
+                        help='Whether or not to shuffle data')
+
+    # Episode configuration
+    # WARNING! this min_examples_in_class should match args.k_shots + args.k_eval in MAML for a fair comparison
+    parser.add_argument('--min_examples_in_class', type=int, default=20)
+
+    # supervised learning doesnt need ways/shots
+    parser.add_argument('--num_ways', type=int, default=None)
+    parser.add_argument('--num_support', type=int, default=None)
+    parser.add_argument('--num_query', type=int, default=None)
+
+    parser.add_argument('--min_ways', type=int, default=2,
+                        help='Minimum # of ways per task')  # doesn't matter since we fixed 5-way setting (so trivially >2 ways)
+
+    parser.add_argument('--max_ways_upper_bound', type=int, default=1000000000000,
+                        help='Maximum # of ways per task')
+
+    parser.add_argument('--max_num_query', type=int, default=1000000000000,
+                        help='Maximum # of query samples')
+
+    parser.add_argument('--max_support_set_size', type=int, default=1000000000000,
+                        help='Maximum # of support samples')
+
+    parser.add_argument('--max_support_size_contrib_per_class', type=int, default=1000000000000,
+                        help='Maximum # of support samples per class')
+
+    parser.add_argument('--min_log_weight', type=float, default=-0.69314718055994529,
+                        help='Do not touch, used to randomly sample support set')
+
+    parser.add_argument('--max_log_weight', type=float, default=0.69314718055994529,
+                        help='Do not touch, used to randomly sample support set')
+
+    # Hierarchy options
+    parser.add_argument('--ignore_bilevel_ontology', type=bool, default=False,
+                        help='Whether or not to use superclass for BiLevel datasets (e.g Omniglot)')
+
+    parser.add_argument('--ignore_dag_ontology', type=bool, default=False,
+                        help='Whether to ignore ImageNet DAG ontology when sampling \
+                                          classes from it. This has no effect if ImageNet is not  \
+                                          part of the benchmark.')
+
+    parser.add_argument('--ignore_hierarchy_probability', type=float, default=0.,
+                        help='if using a hierarchy, this flag makes the sampler \
+                                          ignore the hierarchy for this proportion of episodes \
+                                          and instead sample categories uniformly.')
+    # ======end MDS args 1/25=======#
+
     # - parse arguments
     args: Namespace = parser.parse_args()
+
     args.criterion = args.loss
     assert args.criterion is args.loss
     # - load cluster ids so that wandb can use it later for naming runs, experiments, etc.
     load_cluster_jobids_to(args)
     return args
 
 
@@ -150,25 +231,33 @@
     Get args from supervised learning and merge it with current args. Default precedence is the checkpoint args
     since you want to keep training from the checkpoint value.
 
     Note:
         - model, opt, scheduler objs won't be present but will be loaded later.
         - To create a new path to checkpoint the checkpointed model this code overwrites
     """
+    print('----> Recovering args & model from checkpoint')
+    logging.info('-----> Recovering args & model from checkpoint')
+    # -
+    args.path_to_checkpoint: Path = expanduser(args.path_to_checkpoint)
+    print(f'{args.path_to_checkpoint=}')
     ckpt: dict = torch.load(args.path_to_checkpoint, map_location=torch.device('cpu'))
     # ckpt: dict = torch.load(args.path_to_checkpoint, map_location=args.device)
     args_dict: dict = ckpt['args_dict']
     del ckpt  # since ckpt might have lots of data from previous training, not needed her when recovering only args
     args_ckpt: Namespace = Namespace(**args_dict)
 
     # - updater args has precedence.
     if precedence_to_args_checkpoint:
         args: Namespace = merge_args(starting_args=args, updater_args=args_ckpt)
     else:
         args: Namespace = merge_args(starting_args=args_ckpt, updater_args=args)
+    # from torch.nn import CrossEntropyLoss
+    # later, doesn't let me do import all with * locally :(
+    args.loss = eval(args.loss)
 
     # - create a correct path to save the new model that will be checkpointe and not break the previous checkpoint
     from uutils.argparse_uu.common import create_default_log_root
     create_default_log_root(args)  # creates a new log root with the current job number etc
     return args
 
 
@@ -209,7 +298,78 @@
     #     args: Namespace = merge_args(starting_args=args_ckpt, updater_args=args)
     # # - always overwrite the path to the checkpoint with the one given by the user
     # # (since relitive paths aren't saved properly since they are usually saved as expanded paths)
     # args.path_to_checkpoint: Path = path2args
     # args.log_root: Path = Path('~/data/logs/')
     # return args
     raise NotImplementedError
+
+
+# - some default args
+
+def get_args_mi_usl_default(args: Optional[Namespace] = None, log_to_wandb: Optional[bool] = None):
+    import os
+    # -
+    args: Namespace = parse_args_standard_sl() if args is None else args
+    # - model
+    args.n_cls = 64
+    # args.n_cls = 64 + 1100  # mio
+    # args.n_cls = 1262  # micod
+    # args.n_cls = 5  # 5-way
+    args.n_classes = args.n_cls
+    args.model_option = '5CNN_opt_as_model_for_few_shot'
+    args.filter_size = 4
+    args.model_hps = dict(image_size=84, bn_eps=1e-3, bn_momentum=0.95, n_classes=args.n_cls,
+                          filter_size=args.filter_size, levels=None, spp=False, in_channels=3)
+
+    # - data
+    # args.data_option = 'hdb4_micod'
+    # args.n_classes = args.n_cls
+    # args.data_augmentation = 'hdb4_micod'
+    args.data_path = Path('~/data/miniImageNet_rfs/miniImageNet').expanduser()
+    args.data_option = str(args.data_path)
+
+    # - training mode
+    args.training_mode = 'iterations'
+    # args.num_its = 100_000  # mds 50_000: https://gitA,aahub.com/google-research/meta-dataset/blob/d6574b42c0f501225f682d651c631aef24ad0916/meta_dataset/learn/gin/best/pretrain_imagenet_resnet.gin#L20
+    # args.num_its = 2_000_000  # hdb4 resnetrfs about 2.5 more than above
+    args.num_its = 6
+
+    # - debug flag
+    # args.debug = True
+    args.debug = False
+
+    # - opt
+    # args.opt_option = 'AdafactorDefaultFair'
+    args.opt_option = 'Adam_rfs_cifarfs'
+    args.batch_size = 256
+    args.lr = 1e-3
+    args.opt_hps: dict = dict(lr=args.lr)
+
+    # - scheduler
+    # args.scheduler_option = 'AdafactorSchedule'
+    # args.scheduler_option = 'None'
+    args.scheduler_option = 'Adam_cosine_scheduler_rfs_cifarfs'
+    args.log_scheduler_freq = 1
+    args.T_max = args.num_its // args.log_scheduler_freq  # intended 800K/2k
+    args.eta_min = 1e-5  # match MAML++
+    args.scheduler_hps: dict = dict(T_max=args.T_max, eta_min=args.eta_min)
+    print(f'{args.T_max=}')
+
+    # - logging params
+    args.log_freq = args.num_its // 4  # logs 4 times
+    # args.smart_logging_ckpt = dict(smart_logging_type='log_more_often_after_threshold_is_reached',
+    #                                metric_to_use='train_acc', threshold=0.9, log_speed_up=10)
+
+    # -- wandb args
+    args.wandb_project = 'entire-diversity-spectrum'
+    # - wandb expt args
+    args.experiment_name = f'{args.manual_loads_name} {args.model_option} {args.data_option} {args.filter_size} {os.path.basename(__file__)}'
+    args.run_name = f'{args.manual_loads_name} {args.model_option} {args.opt_option} {args.lr} {args.scheduler_option} {args.filter_size}: {args.jobid=}'
+    # args.log_to_wandb = True  # set false for the this default dummy args
+    # args.log_to_wandb = False  # set false for the this default dummy args
+    args.log_to_wandb = False if log_to_wandb is None else log_to_wandb
+
+    # -- Setup up remaining stuff for experiment
+    from uutils.argparse_uu.common import setup_args_for_experiment
+    args: Namespace = setup_args_for_experiment(args)
+    return args
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/emailing.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/emailing.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/logger.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import logging
+import os
+import sys
 from argparse import Namespace
 from typing import Any, Union
 
 import torch
 import torch.nn as nn
 
 # import matplotlib as mpl
@@ -18,14 +20,60 @@
 import uutils
 # from uutils.torch_uu.distributed import is_lead_worker
 from uutils.torch_uu import r2_score_from_torch
 from uutils.torch_uu.distributed import is_lead_worker
 from uutils.torch_uu.models import get_simple_model
 from uutils.torch_uu.tensorboard import log_2_tb_supervisedlearning
 
+from pdb import set_trace as st
+
+
+def print_acc_loss_from_training_curve(path: Union[str, Path],
+                                       learning_stats_fname: str = 'experiment_stats.json',
+                                       metrics: list[str] = ['acc', 'loss'],
+                                       splits: list[str] = ['train', 'val'],
+                                       # test missing cuz we don't eval on test during training, no cheating!
+                                       idx: int = -1,  # last value
+                                       clear_accidental_ckpt_str_in_path: str = '/ckpt.pt'
+                                       ) -> dict:
+    """ print acc and loss from training curve ckpt.
+
+    Intention:
+    # path ~ log_root / 'experiment_stats.json'
+    path = '~/data/logs/logs_Feb04_17-38-21_jobid_855372_pid_2723881_wandb_True/experiment_stats.json'
+    # get dict and print acc and loss, split
+
+    """
+    if 'debug_5cnn_2filters' in str(path):
+        data: dict = dict()
+        for split in splits:
+            for metric in metrics:
+                data[f'{split}_{metric}_{idx}'] = -1
+        return data
+    # hopefully something like '~/data/logs/logs_Feb04_17-38-21_jobid_855372_pid_2723881_wandb_True/experiment_stats.json'
+    path: Path = uutils.expanduser(path)
+    if learning_stats_fname != 'experiment_stats.json':
+        path = path / learning_stats_fname
+    # - clear accidental ckpt str in path, remove it, then following code adds the right name to experiment json file
+    if clear_accidental_ckpt_str_in_path in str(path):
+        path: str = str(path).replace(clear_accidental_ckpt_str_in_path, '')
+        path: Path = uutils.expanduser(path)
+    # if end of string is not json, then user forgot to put the path to experiment run, so put your best guess based on how uutils works by default
+    if not str(path).endswith('.json'):
+        path = path / learning_stats_fname
+    # - get loss/accs/metrics from training learning curve stats stored
+    data: dict = dict()
+    with open(path, 'r') as f:
+        experiment_stats: dict = json.load(f)
+        for split in splits:
+            for metric in metrics:
+                print(f'{split} {metric}: {experiment_stats[split][metric][idx]}')
+                data[f'{split}_{metric}_{idx}'] = experiment_stats[split][metric][idx]
+    return data
+
 
 def save_model_as_string(args: Namespace, model: nn.Module):
     """ save model as as string. """
     with open(args.log_root / 'model_as_str.txt', 'w+') as f:
         # json.dump({'base_model': str(base_model), 'meta_learner': str(meta_learner)}, f, indent=4)
         f.write(str(model))
 
@@ -82,14 +130,19 @@
         :param log_file_name:
         :return:
         """
         if is_lead_worker(self.args.rank):
             # - guarantees it prints to console
             # from pprint import pprint
             # pprint(msg)
+            # st()
+            # print(msg, flush=flush, file=sys.stdout)
+            # uncomment two lines bellow perhaps to debug vit issue
+            # print(f'{sys.stdout=}')
+            # print(f'{os.path.realpath(sys.stdout.name)=}')
             print(msg, flush=flush)
             # print(msg, file=sys.stdout, flush=flush)
             # - to make sure it prints to the logger file too not just to console
             if log_file_name is not None:
                 print(msg, file=self.args.log_root / log_file_name, flush=flush)
 
     # def pretty_log(self, obj: Any):
@@ -102,15 +155,14 @@
     #     from pprint import pprint
     #     if is_lead_worker(self.args.rank):
     #         pprint(obj)
     #         # # - to make sure it prints to the logger file too not just to console
     #         # if log_file_name is not None:
     #         #     print(msg, file=self.args.log_root / log_file_name, flush=True)
 
-
     def record_train_stats_stats_collector(self, it: int, loss: float, acc: float):
         """
         Records the loss, acc and the iteration it happened.
 
         Note: recording the iteration it happened helps for plotting.
         Note: self.experiment_stats[train][loss/acc][it] is the loss/acc for the train phase at iteration it.
         Note: for each training iteration you log time. For each epoch you log at the end of each epoch.
@@ -193,15 +245,15 @@
             self,
             title='Learnig & Evaluation Curves',
 
             grid: bool = True,
             show: bool = False,
 
             wandb_log_fig: bool = False
-        ):
+    ):
         if is_lead_worker(self.args.rank):
             # plt.style.use('default')
             # self.save_experiment_stats_to_json_file()
 
             if not hasattr(self.args, 'target_type'):
                 tag1 = f'Train loss'
                 tag2 = f'Train accuracy/R2'
@@ -236,17 +288,17 @@
             loss_ax1.legend()
             loss_ax1.set_title(title)
             loss_ax1.set_ylabel('Loss')
             loss_ax1.grid(grid)
 
             # - plot stuff into acc axis
             acc_ax2.plot(self.experiment_stats['train']['its'], self.experiment_stats['train']['acc'],
-                          label=tag2, linestyle='-', marker='x', color='b', linewidth=1)
+                         label=tag2, linestyle='-', marker='x', color='b', linewidth=1)
             acc_ax2.plot(self.experiment_stats['val']['its'], self.experiment_stats['val']['acc'],
-                          label=tag4, linestyle='-', marker='x', color='c', linewidth=1)
+                         label=tag4, linestyle='-', marker='x', color='c', linewidth=1)
 
             acc_ax2.legend()
             x_axis_label: str = self.args.training_mode  # epochs or iterations
             acc_ax2.set_xlabel(x_axis_label)
             acc_ax2.set_ylabel(ylabel_acc)
             acc_ax2.grid(grid)
 
@@ -263,22 +315,23 @@
                 import wandb
 
                 wandb.log(data={'fig': fig}, step=args.it, commit=True)
             # careful: even if you return the figure it seems it needs to be closed inside here anyway...so if you close it
             # but return it who knows what might happen.
             plt.close('all')  # https://stackoverflow.com/questions/21884271/warning-about-too-many-open-figures
 
+
 def save_current_plots_and_stats(
         title='Learnig & Evaluation Curves',
 
         grid: bool = True,
         show: bool = False,
 
-        wandb_log_fig = False
-    ):
+        wandb_log_fig=False
+):
     """
     TODO - adapt so that logger doesn't have this function as a method attached to the object
 
     :param title:
     :param grid:
     :param show:
     :param wandb_log_fig:
@@ -286,15 +339,16 @@
     """
     # plt.style.use('default')
     # self.save_experiment_stats_to_json_file()
 
     tag1 = f'Train loss'
     # tag2 = f'Train accuracy/R2'
     tag3 = f'Eval loss'
-    experiment_stats = uutils.load_json('~/Desktop/paper_figs/logs_Nov23_11-39-21_jobid_438713.iam-pbs/experiment_stats.json')
+    experiment_stats = uutils.load_json(
+        '~/Desktop/paper_figs/logs_Nov23_11-39-21_jobid_438713.iam-pbs/experiment_stats.json')
 
     # - get figure with two axis, loss above and accuracy bellow
     fig, (loss_ax1, acc_ax2) = plt.subplots(nrows=2, ncols=1, sharex=True)
 
     # - plot stuff into loss axis
     loss_ax1.plot(experiment_stats['train']['its'], experiment_stats['train']['loss'],
                   label=tag1, linestyle='-', marker='x', color='r', linewidth=1)
@@ -331,7 +385,31 @@
     #     assert False, 'Not tested'
     #     import wandb
     #
     #     wandb.log(data={'fig': fig}, step=args.it, commit=True)
     # careful: even if you return the figure it seems it needs to be closed inside here anyway...so if you close it
     # but return it who knows what might happen.
     # plt.close('all')  # https://stackoverflow.com/questions/21884271/warning-about-too-many-open-figures
+
+
+# - main, tests, examples, tutorials, etc.
+
+def test_print_acc_loss_from_training_curve():
+    path = '~/data/logs/logs_Mar30_08-17-19_jobid_17733_pid_142663'
+    print_acc_loss_from_training_curve(path)
+    path = '~/data/logs/logs_Mar30_08-17-19_jobid_17733_pid_142663/ckpt.pt/experiment_stats.json'
+    print_acc_loss_from_training_curve(path)
+
+
+# - run main, tests, examples, tutorials, etc.
+
+if __name__ == '__main__':
+    import time
+
+    start_time = time.time()
+    test_print_acc_loss_from_training_curve()
+    print(f'Done! Finished in {time.time() - start_time:.2f} seconds\a\n'
+          f''
+          f''
+          f''
+          f''
+          f'')
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/logging_uu/__init__.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/logging_uu/__init__.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/plot/__init__.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/plot/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,16 @@
          show: bool = False,
          save_plot: bool = False,
          plot_filename: str = 'plot',
          title: Optional[str] = None,
          label: Optional[str] = None,
          y_hline: Optional[float] = None, y_hline_label: Optional[str] = None,
          x_hline: Optional[float] = None, x_hline_label: Optional[str] = None,
-         new_plot: bool = False, marker: Optional = None, color: Optional = None,
+         new_plot: bool = False,
+         marker: Optional = None, color: Optional = None,
          tight_layout: bool = False
          ):
     """
     Nice easy plot function to quickly plot x vs y and labeling the x and y.
 
     Nice optional args, like plotting straight (horizontal or vertical lines), saving MI_plots_sl_vs_maml_1st_attempt, showing the plot, adding
     optional legends etc.
@@ -166,14 +167,15 @@
     plt.title(title)
     plt.xlabel(xlabel)
     plt.ylabel(ylabel)
 
     if show:
         plt.show()
 
+
 # def pdist(embeddings, distance='cosine') -> np.ndarray:
 #     distance_fn = _DISTANCES[distance]
 #     n = len(embeddings)
 #     distance_matrix = np.zeros([n, n])
 #     if distance != 'asymmetric_kl':
 #         for (i, e1), (j, e2) in itertools.combinations(enumerate(embeddings), 2):
 #             distance_matrix[i, j] = distance_fn(e1, e2)
@@ -196,14 +198,15 @@
     linkage_matrix = linkage(cond_distance_matrix, method='complete', optimal_ordering=True)
     if labels is not None:
         distance_matrix = pd.DataFrame(distance_matrix, index=labels, columns=labels)
     sns.clustermap(distance_matrix, row_linkage=linkage_matrix, col_linkage=linkage_matrix, cmap='viridis_r')
     if show_plot:
         plt.show()
 
+
 def plot_distance_matrix_heatmap_only(distance_matrix, labels=None, show_plot=True):
     import seaborn as sns
     import pandas as pd
     import matplotlib.pyplot as plt
     # from task2vec.task_similarity import pdist
     # distance_matrix = pdist(embeddings, distance=distance)
     if labels is not None:
@@ -1020,27 +1023,29 @@
 
     x_vals_as_symbols: list[str] = [f'Val{v:0.2f}' for v in x]
     plot_with_error_bands(x=x, y=y1mean, yerr=y1err, xlabel='x', ylabel='y', title='Custom Seaborn',
                           x_vals_as_symbols=x_vals_as_symbols)
     plot_with_error_bands(x=x, y=y2mean, yerr=y2err, xlabel='x', ylabel='y', title='Custom Seaborn',
                           x_vals_as_symbols=x_vals_as_symbols)
     plt.show()
-    
-def smooth(scalars, weight = 0.8):  # Weight between 0 and 1
+
+
+def smooth(scalars, weight=0.8):  # Weight between 0 and 1
     # Curve smoothing function, for noisy plots, etc
     # From https://stackoverflow.com/questions/42281844/what-is-the-mathematics-behind-the-smoothing-parameter-in-tensorboards-scalar
     last = scalars[0]  # First value in the plot (first timestep)
     smoothed = list()
     for point in scalars:
         smoothed_val = last * weight + (1 - weight) * point  # Calculate smoothed value
-        smoothed.append(smoothed_val)                        # Save it
-        last = smoothed_val                                  # Anchor the last smoothed value
+        smoothed.append(smoothed_val)  # Save it
+        last = smoothed_val  # Anchor the last smoothed value
 
     return smoothed
-    
+
+
 if __name__ == '__main__':
     # save_plot_test()
     # default_seabron_example()
     # plot_seaborn_curve_with_x_values_y_values_test()
     # plot_with_error_bands_test()
     # plot_with_error_bands_xticks_test()
     bar_graph_with_eroror_bars_full_example()
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/stats_collector_mit.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/stats_collector_mit.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/__init__.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,14 @@
 import copy
 
 from argparse import Namespace
 
 # from torch.optim.lr_scheduler import _LRScheduler
 
 # from uutils.torch_uu.optim_uu.optimizers import get_default_uu_adafactor_optimizer_and_scheduler_fairseq
-from uutils.torch_uu.tensorboard import log_2_tb
 
 import gc
 
 import urllib.request
 
 from pprint import pprint
 
@@ -66,14 +65,21 @@
     On the terminal do:
     python -c "import uutils; uutils.torch_uu.hello()"
     """
     import uutils.torch_uu as torch_uu
     print(f'\nhello from torch_uu __init__.py in:\n{torch_uu}\n')
 
 
+def print_python_and_torch_version():
+    import sys
+    print(f'python version: {sys.version=}')
+    import torch
+    print(f'{torch.version=}')
+
+
 def gpu_test_torch_any_device():
     """
     python -c "import uutils; uutils.torch_uu.gpu_test_torch_any_device()"
     """
     from torch import Tensor
 
     print(f'device name: {device_name()}')
@@ -81,77 +87,112 @@
     x: Tensor = torch.randn(2, 4).to(device)
     y: Tensor = torch.randn(4, 1).to(device)
     out: Tensor = (x @ y)
     assert out.size() == torch.Size([2, 1])
     print(f'Success, torch works with whatever device is shown in the output tensor:\n{out=}')
 
 
-def gpu_test():
+def gpu_test() -> None:
     """
     python -c "import uutils; uutils.torch_uu.gpu_test()"
     """
+    import sys
+    print(f'python version: {sys.version=}')
+    import torch
+    print(f'{torch.version=}')
+    print(f'torch.__version__={torch.__version__}')
+
     from torch import Tensor
 
     print(f'device name: {device_name()}')
     x: Tensor = torch.randn(2, 4).cuda()
     y: Tensor = torch.randn(4, 1).cuda()
     out: Tensor = (x @ y)
     assert out.size() == torch.Size([2, 1])
     print(f'Success, no Cuda errors means it worked see:\n{out=}')
 
 
+def gpu_minimalist_test() -> None:
+    """
+    prints pytorch version & does some gpu/cuda 2D matrix multiplication computation.
+
+    python -c "import torch; print(torch.__version__); print((torch.randn(2, 4).cuda() @ torch.randn(4, 1).cuda()))"
+    """
+    import torch;
+    print(torch.__version__);
+    print((torch.randn(2, 4).cuda() @ torch.randn(4, 1).cuda()))
+
+def bfloat16_avail() -> bool:
+    """ Checks if bfloat16 is available in your nvidia arch, usually ampere.
+
+    As of my last training data in September 2021, the Nvidia Quadro RTX 8000 is based on the Turing architecture, not Ampere. This was the successor to the Pascal architecture and predecessor to the Ampere architecture.
+    The RTX 8000, like other Turing cards, features RT (Ray Tracing) cores for realistic lighting effects and Tensor cores for AI workloads such as deep learning. It also has 48 GB of GDDR6 memory.
+    However, Nvidia regularly releases new GPUs and architectures, so you might want to check their latest product offerings. Remember, I can only provide information up to my last update in September 2021.
+    """
+    # get major revision to infer if bfloat is avail, ampere is needed my snap Quadro RTX 8000 is not Ampere.
+    major, _ = torch.cuda.get_device_capability()  # _ refers to minor revisions to arch
+    if major >= 8:
+        print("=" * 80)
+        print("Your GPU supports bfloat16, you can accelerate training with the argument --bfloat16")
+        print("=" * 80)
+        return True
+    else:
+        return False
+
 # -
 
 def device_name():
     return gpu_name_otherwise_cpu()
 
 
-def gpu_name_otherwise_cpu():
+def gpu_name_otherwise_cpu(print_to_stdout: bool = False):
     gpu_name_or_cpu = None
     try:
         gpu_name_or_cpu = torch.cuda.get_device_name(0)
     except:
         device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
         gpu_name_or_cpu = device
+    print(f'{gpu_name_or_cpu=}') if print_to_stdout else None
     return gpu_name_or_cpu
 
 
 def make_code_deterministic(seed: int, always_use_deterministic_algorithms: bool = True):
     """
 
-    Note: use_deterministic_algorithms makes all algorithms deterministic while torch_uu.backends.cudnn.deterministic=True
-    makes convs only determinsitic. There is also a way to choose algorithms based on hardware performance, to
-    avoid that use torch_uu.backends.cudnn.benchmark = False (note the agorithm chosen even if determinsitic might be
-    random itself so the other two flags are useful).
-
-    todo -
+    Note:
+        - always_use_deterministic_algorithms: not all algorithms are deterministic. If one doesn't have determinstic
+        algorithm for a given operation, it will throw an error.
+    todo - (idk if this CAN be fixed by me, easily)
      - fix this:
       RuntimeError: Deterministic behavior was enabled with either `torch_uu.use_deterministic_algorithms(True)` or `at::Context::setDeterministicAlgorithms(true)`, but this operation is not deterministic because it uses CuBLAS and you have CUDA >= 10.2. To enable deterministic behavior in this case, you must set an environment variable before running your PyTorch application: CUBLAS_WORKSPACE_CONFIG=:4096:8 or CUBLAS_WORKSPACE_CONFIG=:16:8. For more information, go to https://docs.nvidia.com/cuda/cublas/index.html#cublasApi_reproducibility
      - figure out the worker in dataloader thing...https://pytorch.org/docs/stable/notes/randomness.html
      - read the RNN LSTM part
+
     ref:
         - https://pytorch.org/docs/stable/notes/randomness.html
         - https://stackoverflow.com/questions/66130547/what-does-the-difference-between-torch-backends-cudnn-deterministic-true-and
     :return:
     """
     import random
     import numpy as np
     import torch
-    # - make pytorch determinsitc
-    # makes all ops determinsitic no matter what. Note this throws an errors if you code has an op that doesn't have determinsitic implementation
-    torch.manual_seed(seed)
+    import os
+
+    # - make pytorch determinsitc, makes all ops determinsitic no matter what. Note this throws an errors if you code has an op that doesn't have determinsitic implementation
     if always_use_deterministic_algorithms:
         torch.use_deterministic_algorithms(True)
-    # makes convs deterministic
-    torch.backends.cudnn.deterministic = True
-    # doesn't allow benchmarking to select fastest algorithms for specific ops
-    torch.backends.cudnn.benchmark = False
+        # try:
+        #     torch.set_deterministic(True)
+        #     return True
+        # except Exception as e:
+        #     logging.warning(f'could not set torch to deterministic, {e=}')
+        #     return False
     # - make python determinsitic
-    np.random.seed(seed)
-    random.seed(seed)
+    from uutils import seed_everything
+    seed_everything(seed)
 
 
 def index(tensor: Tensor, value, ith_match: int = 0) -> Union[int, Tensor]:
     """
     Returns generalized index (i.e. location/coordinate) of the first occurence of value
     in Tensor. For flat tensors (i.e. arrays/lists) it returns the indices of the occurrences
     of the value you are looking for. Otherwise, it returns the "index" as a coordinate.
@@ -244,18 +285,24 @@
         x_batch = x_batch.to(args.device)
     if isinstance(y_batch, Tensor):
         y_batch = y_batch.to(args.device)
     return x_batch, y_batch
 
 
 def process_meta_batch(args, batch) -> tuple[torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor]:
+    """
+    Processes the meta batch (batch of tasks) and returns the data in the correct format, as follows:
+    shape of data [T, n*K, C, H, W], [T, n*K], [T, n*K, C, H, W], [T, n*K]
+    """
     # - upack the data
     if type(batch) == dict:
+        # spt_x, spt_y, qry_x, qry_y are of shape [T, n*K, C, H, W], [T, n*K], [T, n*K, C, H, W], [T, n*K]
         (spt_x, spt_y), (qry_x, qry_y) = batch["train"], batch["test"]
     elif type(batch) == tuple or type(batch) == list:
+        # spt_x, spt_y, qry_x, qry_y are of shape [T, n*K, C, H, W], [T, n*K], [T, n*K, C, H, W], [T, n*K]
         spt_x, spt_y, qry_x, qry_y = batch
     else:
         raise ValueError(f'Not implemented how to process this batch of type {type(batch)} with value {batch=}')
     # invariant: we have spt_x, spt_y, qry_x, qry_y after here
     # assert len(spt_x.size()) == 4, f'Expected [B,n*k, C,H,W]}'  cant actually put this due to regression tasks :(
 
     # - convert to float32 single float, somehow the ckpts seem to need this for sinusoid
@@ -327,26 +374,43 @@
     return get_device_from(args.model)
 
 
 def get_device_from_args2(args):
     return next(args.model.parameters()).device
 
 
-def get_device(gpu_idx: int = 0) -> torch.device:
+def get_device(gpu_idx: Optional[int] = 0) -> torch.device:
     """
-    Get default gpu torch device.
-
-    :param gpu_idx:
-    :return:
+    Get default gpu torch device or use cpu
     """
+    # gpu_idx: int = 0 if gpu_idx is None else gpu_idx
     device: torch.device = torch.device(f"cuda:{gpu_idx}" if torch.cuda.is_available() else "cpu")
-    # device: torch.device = torch.device(f"cuda:0" if torch.cuda.is_available() else "cpu")
     return device
 
 
+# def get_device_via_env_variables(deterministic: bool = False, verbose: bool = True) -> torch.device:
+#     device: torch.device = torch.device("cpu")
+#     if torch.cuda.is_available():
+#         if 'CUDA_VISIBLE_DEVICES' not in os.environ:
+#             device: torch.device = torch.device("cuda:0")
+#         else:
+#             gpu_idx: list[str] = os.environ['CUDA_VISIBLE_DEVICES'].split(',')
+#             if len(gpu_idx) == 1:
+#                 gpu_idx: str = gpu_idx[0]
+#             else:
+#                 # generate random int from 0 to len(gpu_idx) with import statement
+#                 import random
+#                 idx: int = random.randint(0, len(gpu_idx) - 1) if not deterministic else -1
+#                 gpu_idx: str = gpu_idx[idx]
+#             device: torch.device = torch.device(f"cuda:{gpu_idx}")
+#     if verbose:
+#         print(f'{device=}')
+#     return device
+
+
 def create_detached_deep_copy_old(mdl):
     mdl_new = copy.deepcopy(mdl)
     detached_params = mdl.state_dict()
     # set to detached
     for name, w in mdl.named_parameters():
         w_detached = nn.Parameter(w.detach())
         detached_params[name] = w_detached
@@ -452,29 +516,50 @@
     if detach:
         lp_norms = [w.detach().norm(p) for name, w in mdl.named_parameters()]
     else:
         lp_norms = [w.norm(p) for name, w in mdl.named_parameters()]
     return sum(lp_norms)
 
 
-def norm(f: nn.Module, l: int = 2, detach: bool = False):
+def norm(f: nn.Module, l: int = 2, detach: bool = False, cpu: bool = False) -> Tensor:
     # return sum([w.detach().norm(l) for w in f.parameters()])
-    return lp_norm(f, p=l, detach=detach)
+    norm_val: Tensor = lp_norm(f, p=l, detach=detach)
+    # move to cpu
+    norm_val: Tensor = norm_val.cpu() if cpu else norm_val
+    return norm_val
+
+
+def count_number_of_parameters(model: nn.Module, only_trainable: bool = True) -> int:
+    """
+    Counts the number of trainable params. If all params, specify only_trainable = False.
+
+    Ref:
+        - https://discuss.pytorch.org/t/how-do-i-check-the-number-of-parameters-of-a-model/4325/9?u=brando_miranda
+        - https://stackoverflow.com/questions/49201236/check-the-total-number-of-parameters-in-a-pytorch-model/62764464#62764464
+    :return:
+    """
+    if only_trainable:
+        num_params: int = sum(p.numel() for p in model.parameters() if p.requires_grad)
+    else:  # counts trainable and none-traibale
+        num_params: int = sum(p.numel() for p in model.parameters() if p)
+    assert num_params > 0, f'Err: {num_params=}'
+    return int(num_params)
 
 
 def normalize(x: Tensor) -> Tensor:
     """
     Normalizes to unit circle.
 
     From rfs: original code: https://github.com/WangYueFt/rfs/blob/f8c837ba93c62dd0ac68a2f4019c619aa86b8421/eval/meta_eval.py#L27
     """
     norm = x.pow(2).sum(1, keepdim=True).pow(1. / 2)
     out = x.div(norm)
     return out
 
+
 def check_two_models_equal(model1, model2):
     '''
     Checks if two models are equal.
 
     https://discuss.pytorch.org/t/check-if-models-have-same-weights/4351
     '''
     for p1, p2 in zip(model1.parameters(), model2.parameters()):
@@ -1040,29 +1125,21 @@
             log_train_stats(args.it, train_loss, train_acc)
             # agent.save(args.it)  # very expensive! since your only fitting one batch its ok to save it every time you log - but you might want to do this left often.
             break  # halt once both the accuracy is high enough AND train loss is low enough
 
     return avg_loss.item(), avg_acc.item()
 
 
-##
-
-
-##
-
 def count_nb_params(net):
     count = 0
     for p in net.parameters():
         count += p.data.nelement()
     return count
 
 
-##
-
-
 def preprocess_grad_loss(x, p=10, eps=1e-8):
     """ Preprocessing (vectorized) implementation from the paper:
 
     if |x| >= e^-p (not too small)
         coord1, coord2 = (log(|x| + eps)/p, sign(x))
     else: (too small
         coord1, coord2 = (-1, (e^p)*x)
@@ -1961,14 +2038,15 @@
     :param model:
     :param train_batch:
     :param val_batch:
     :param optimizer:
     :param tolerance:
     :return:
     """
+    from uutils.torch_uu.tensorboard import log_2_tb
     avg_loss = AverageMeter('train loss')
     avg_acc = AverageMeter('train accuracy')
 
     it = 0
     train_loss = float('inf')
     x_train_batch, y_train_batch = train_batch
     x_val_batch, y_val_batch = val_batch
@@ -2285,137 +2363,140 @@
                                                             iter_tasks=None,
                                                             log_to_wandb: bool = False,
                                                             show_layerwise_sims: bool = True
                                                             ):
     """
     Goal is to see if similarity is small s <<< 0.9 (at least s < 0.8) since this suggests that
     """
-    import wandb
-    import uutils.torch_uu as torch_uu
-    from pprint import pprint
-    from uutils.torch_uu import summarize_similarities
-    from uutils.torch_uu.distributed import is_lead_worker
-    # - is it epoch or iteration
-    it_or_epoch: str = 'epoch_num' if args.training_mode == 'epochs' else 'it'
-    sim_or_dist: str = 'sim'
-    if hasattr(args, 'metrics_as_dist'):
-        sim_or_dist: str = 'dist' if args.metrics_as_dist else sim_or_dist
-    total_its: int = args.num_empochs if args.training_mode == 'epochs' else args.num_its
-
-    if (it == total_its - 1 or force_log) and is_lead_worker(args.rank):
-        # if (it % log_freq_for_detection_of_feature_reuse == 0 or it == total_its - 1 or force_log) and is_lead_worker(args.rank):
-        #     if hasattr(args, 'metrics_as_dist'):
-        #         sims = args.meta_learner.compute_functional_similarities(spt_x, spt_y, qry_x, qry_y, args.layer_names, parallel=parallel, iter_tasks=iter_tasks, metric_as_dist=args.metrics_as_dist)
-        #     else:
-        #         sims = args.meta_learner.compute_functional_similarities(spt_x, spt_y, qry_x, qry_y, args.layer_names, parallel=parallel, iter_tasks=iter_tasks)
-        sims = distances_btw_models(args, mdl1, mdl2, batch_x, batch_y, args.layer_names, args.metrics_as_dist)
-        print(sims)
-        # mean_layer_wise_sim, std_layer_wise_sim, mean_summarized_rep_sim, std_summarized_rep_sim = summarize_similarities(args, sims)
-
-        # -- log (print)
-        args.logger.log(f' \n------ {sim_or_dist} stats: {it_or_epoch}={it} ------')
-        # - per layer
-        # if show_layerwise_sims:
-        print(f'---- Layer-Wise metrics ----')
-        # print(f'mean_layer_wise_{sim_or_dist} (per layer)')
-        # pprint(mean_layer_wise_sim)
-        # print(f'std_layer_wise_{sim_or_dist} (per layer)')
-        # pprint(std_layer_wise_sim)
-        #
-        # # - rep sim
-        # print(f'---- Representation metrics ----')
-        # print(f'mean_summarized_rep_{sim_or_dist} (summary for rep layer)')
-        # pprint(mean_summarized_rep_sim)
-        # print(f'std_summarized_rep_{sim_or_dist} (summary for rep layer)')
-        # pprint(std_summarized_rep_sim)
-        # args.logger.log(f' -- sim stats : {it_or_epoch}={it} --')
-
-        # error bars with wandb: https://community.wandb.ai/t/how-does-one-plot-plots-with-error-bars/651
-        # - log to wandb
-        # if log_to_wandb:
-        #     if it == 0:
-        #         # have all metrics be tracked with it or epoch (custom step)
-        #         #     wandb.define_metric(f'layer average {metric}', step_metric=it_or_epoch)
-        #         for metric in mean_summarized_rep_sim.keys():
-        #             wandb.define_metric(f'rep mean {metric}', step_metric=it_or_epoch)
-        #     # wandb.log per layer
-        #     rep_summary_log = {f'rep mean {metric}': sim for metric, sim in mean_summarized_rep_sim.items()}
-        #     rep_summary_log[it_or_epoch] = it
-        #     wandb.log(rep_summary_log, commit=True)
+    # import wandb
+    # import uutils.torch_uu as torch_uu
+    # from pprint import pprint
+    # from uutils.torch_uu import summarize_similarities
+    # from uutils.torch_uu.distributed import is_lead_worker
+    # # - is it epoch or iteration
+    # it_or_epoch: str = 'epoch_num' if args.training_mode == 'epochs' else 'it'
+    # sim_or_dist: str = 'sim'
+    # if hasattr(args, 'metrics_as_dist'):
+    #     sim_or_dist: str = 'dist' if args.metrics_as_dist else sim_or_dist
+    # total_its: int = args.num_empochs if args.training_mode == 'epochs' else args.num_its
+    #
+    # if (it == total_its - 1 or force_log) and is_lead_worker(args.rank):
+    #     # if (it % log_freq_for_detection_of_feature_reuse == 0 or it == total_its - 1 or force_log) and is_lead_worker(args.rank):
+    #     #     if hasattr(args, 'metrics_as_dist'):
+    #     #         sims = args.meta_learner.compute_functional_similarities(spt_x, spt_y, qry_x, qry_y, args.layer_names, parallel=parallel, iter_tasks=iter_tasks, metric_as_dist=args.metrics_as_dist)
+    #     #     else:
+    #     #         sims = args.meta_learner.compute_functional_similarities(spt_x, spt_y, qry_x, qry_y, args.layer_names, parallel=parallel, iter_tasks=iter_tasks)
+    #     sims = distances_btw_models(args, mdl1, mdl2, batch_x, batch_y, args.layer_names, args.metrics_as_dist)
+    #     print(sims)
+    #     # mean_layer_wise_sim, std_layer_wise_sim, mean_summarized_rep_sim, std_summarized_rep_sim = summarize_similarities(args, sims)
+    #
+    #     # -- log (print)
+    #     args.logger.log(f' \n------ {sim_or_dist} stats: {it_or_epoch}={it} ------')
+    #     # - per layer
+    #     # if show_layerwise_sims:
+    #     print(f'---- Layer-Wise metrics ----')
+    #     # print(f'mean_layer_wise_{sim_or_dist} (per layer)')
+    #     # pprint(mean_layer_wise_sim)
+    #     # print(f'std_layer_wise_{sim_or_dist} (per layer)')
+    #     # pprint(std_layer_wise_sim)
+    #     #
+    #     # # - rep sim
+    #     # print(f'---- Representation metrics ----')
+    #     # print(f'mean_summarized_rep_{sim_or_dist} (summary for rep layer)')
+    #     # pprint(mean_summarized_rep_sim)
+    #     # print(f'std_summarized_rep_{sim_or_dist} (summary for rep layer)')
+    #     # pprint(std_summarized_rep_sim)
+    #     # args.logger.log(f' -- sim stats : {it_or_epoch}={it} --')
+    #
+    #     # error bars with wandb: https://community.wandb.ai/t/how-does-one-plot-plots-with-error-bars/651
+    #     # - log to wandb
+    #     # if log_to_wandb:
+    #     #     if it == 0:
+    #     #         # have all metrics be tracked with it or epoch (custom step)
+    #     #         #     wandb.define_metric(f'layer average {metric}', step_metric=it_or_epoch)
+    #     #         for metric in mean_summarized_rep_sim.keys():
+    #     #             wandb.define_metric(f'rep mean {metric}', step_metric=it_or_epoch)
+    #     #     # wandb.log per layer
+    #     #     rep_summary_log = {f'rep mean {metric}': sim for metric, sim in mean_summarized_rep_sim.items()}
+    #     #     rep_summary_log[it_or_epoch] = it
+    #     #     wandb.log(rep_summary_log, commit=True)
+    raise NotImplementedError
 
 
 def distances_btw_models(args: Namespace,
                          model1: nn.Module, model2: nn.Module,
                          batch_x: torch.Tensor, batch_y: torch.Tensor,
                          layer_names: list[str],
                          metrics_as_dist: bool = True) -> dict:
-    """
-    Compute the distance/sim between two models give a batch of example (this assumes there are no tasks involved, just
-    two batch of any type of examples).
-    """
-    L: int = len(layer_names)
-    # make into eval
-    model1.eval()
-    model2.eval()
-    # -- compute sims
-    x: torch.Tensor = batch_x
-    if torch.cuda.is_available():
-        x = x.cuda()
-    # - compute cca sims
-    cca: list[float] = get_cxa_similarities_per_layer(model1, model2, x, layer_names, sim_type='pwcca')
-    cka: list[float] = get_cxa_similarities_per_layer(model1, model2, x, layer_names, sim_type='lincka')
-    assert len(cca) == L
-    assert len(cka) == L
-    # -- get l2 sims per layer
-    # op = get_l2_similarities_per_layer(model1, model2, x, layer_names, sim_type='op_torch')
-    # nes = get_l2_similarities_per_layer(model1, model2, x, layer_names, sim_type='nes_torch')
-    # cosine = get_l2_similarities_per_layer(model1, model2, x, layer_names, sim_type='cosine_torch')
-
-    # y = self.base_model(qry_x_t)
-    # y_adapt = fmodel(qry_x_t)
-    # # dim=0 because we have single numbers and we are taking the NES in the batch direction
-    # nes_output = uutils.torch_uu.nes_torch(y.squeeze(), y_adapt.squeeze(), dim=0).item()
+    # """
+    # Compute the distance/sim between two models give a batch of example (this assumes there are no tasks involved, just
+    # two batch of any type of examples).
+    # """
+    # L: int = len(layer_names)
+    # # make into eval
+    # model1.eval()
+    # model2.eval()
+    # # -- compute sims
+    # x: torch.Tensor = batch_x
+    # if torch.cuda.is_available():
+    #     x = x.cuda()
+    # # - compute cca sims
+    # cca: list[float] = get_cxa_similarities_per_layer(model1, model2, x, layer_names, sim_type='pwcca')
+    # cka: list[float] = get_cxa_similarities_per_layer(model1, model2, x, layer_names, sim_type='lincka')
+    # assert len(cca) == L
+    # assert len(cka) == L
+    # # -- get l2 sims per layer
+    # # op = get_l2_similarities_per_layer(model1, model2, x, layer_names, sim_type='op_torch')
+    # # nes = get_l2_similarities_per_layer(model1, model2, x, layer_names, sim_type='nes_torch')
+    # # cosine = get_l2_similarities_per_layer(model1, model2, x, layer_names, sim_type='cosine_torch')
     #
-    # query_loss = self.args.criterion(y, y_adapt).item()
-    # # sims = [cca, cka, nes, cosine, nes_output, query_loss]
-    # -- from [Tasks, Sims] -> [Sims, Tasks]
-    # sims = {'cca': [], 'cka': [], 'op': [],  # [L]
-    #         'nes': [], 'cosine': [],  # [L, K]
-    #         'nes_output': [], 'query_loss': []  # [1]
-    #         }
-    # sims = {'cca': cca, 'cka': cka, 'op': op,  # [L]
-    #         'nes': nes, 'cosine': cosine,  # [L, K]
-    #         'nes_output': nes_output, 'query_loss': query_loss  # [1]
-    #         }
-    # sims = {metric: tensorify(sim).detach() for metric, sim in sims.items()}
-    out_metrics: dict = {}
-    for metric, sim in sims.items():
-        out_metrics[metric] = tensorify(sim).detach()
-        if metrics_as_dist and metric != 'query_loss':
-            out_metrics[metric] = 1.0 - out_metrics[metric]
-            if metric != 'cosine':
-                error_tolerance: float = -0.0001
-                assert (out_metrics[
-                            metric] >= error_tolerance).all(), f'Distances are positive but got a negative value somewhere for metric {metric=}.'
-    return out_metrics
+    # # y = self.base_model(qry_x_t)
+    # # y_adapt = fmodel(qry_x_t)
+    # # # dim=0 because we have single numbers and we are taking the NES in the batch direction
+    # # nes_output = uutils.torch_uu.nes_torch(y.squeeze(), y_adapt.squeeze(), dim=0).item()
+    # #
+    # # query_loss = self.args.criterion(y, y_adapt).item()
+    # # # sims = [cca, cka, nes, cosine, nes_output, query_loss]
+    # # -- from [Tasks, Sims] -> [Sims, Tasks]
+    # # sims = {'cca': [], 'cka': [], 'op': [],  # [L]
+    # #         'nes': [], 'cosine': [],  # [L, K]
+    # #         'nes_output': [], 'query_loss': []  # [1]
+    # #         }
+    # # sims = {'cca': cca, 'cka': cka, 'op': op,  # [L]
+    # #         'nes': nes, 'cosine': cosine,  # [L, K]
+    # #         'nes_output': nes_output, 'query_loss': query_loss  # [1]
+    # #         }
+    # # sims = {metric: tensorify(sim).detach() for metric, sim in sims.items()}
+    # out_metrics: dict = {}
+    # for metric, sim in sims.items():
+    #     out_metrics[metric] = tensorify(sim).detach()
+    #     if metrics_as_dist and metric != 'query_loss':
+    #         out_metrics[metric] = 1.0 - out_metrics[metric]
+    #         if metric != 'cosine':
+    #             error_tolerance: float = -0.0001
+    #             assert (out_metrics[
+    #                         metric] >= error_tolerance).all(), f'Distances are positive but got a negative value somewhere for metric {metric=}.'
+    # return out_metrics
+    raise NotImplementedError
 
 
 def get_cxa_similarities_per_layer(model1: nn.Module, model2: nn.Module,
                                    x: torch.Tensor, layer_names: list[str],
                                    sim_type: str = 'pwcca'):
     """
     Get [..., s_l, ...] cca sim per layer (for this data set)
     """
-    from uutils.torch_uu import cxa_sim
-    sims_per_layer = []
-    for layer_name in layer_names:
-        # sim = cxa_sim(model1, model2, x, layer_name, cca_size=self.args.cca_size, iters=1, cxa_sim_type=sim_type)
-        sim = cxa_sim(model1, model2, x, layer_name, iters=1, cxa_sim_type=sim_type)
-        sims_per_layer.append(sim)
-    return sims_per_layer  # [..., s_l, ...]_l
+    # from uutils.torch_uu import cxa_sim
+    # sims_per_layer = []
+    # for layer_name in layer_names:
+    #     # sim = cxa_sim(model1, model2, x, layer_name, cca_size=self.args.cca_size, iters=1, cxa_sim_type=sim_type)
+    #     sim = cxa_sim(model1, model2, x, layer_name, iters=1, cxa_sim_type=sim_type)
+    #     sims_per_layer.append(sim)
+    # return sims_per_layer  # [..., s_l, ...]_l
+    raise NotImplementedError
 
 
 def compare_based_on_mdl1_vs_mdl2(args: Namespace, meta_dataloader):
     print(f'{args.num_workers=}')
     # print(f'-->{args.meta_batch_size_eval=}')
     print(f'-->{args.num_its=}')
     # print(f'-->{args.nb_inner_train_steps=}')
@@ -2675,14 +2756,15 @@
     """
     data: torch.Tensor = torch.distributions.Normal(loc=loc, scale=scale).sample((B, Din))
     return data
 
 
 # --
 
+
 # -- tests
 
 def ned_test():
     import torch.nn as nn
 
     # dim = 1  # apply cosine accross the second dimension/feature dimension
 
@@ -2778,121 +2860,121 @@
     #
     x = torch.randn(3, 3, 3)
     print(f'{x.sum()=}')
     out = x @ x
     print(f'{out.sum()}')
 
 
-def op_test():
-    from uutils.torch_uu.models import hardcoded_3_layer_model
+# def op_test():
+#     from uutils.torch_uu.models import hardcoded_3_layer_model
+#
+#     force = True
+#     # force = False
+#     mdl1 = hardcoded_3_layer_model(5, 1)
+#     mdl2 = hardcoded_3_layer_model(5, 1)
+#     batch_size = 4
+#     X = torch.randn(batch_size, 5)
+#     import copy
+#     from uutils.torch_uu import l2_sim_torch
+#     # get [..., s_l, ...] sim per layer (for this data set)
+#     modules = zip(mdl1.named_children(), mdl2.named_children())
+#     sims_per_layer = []
+#     out1 = X
+#     out2 = X
+#     for (name1, m1), (name2, m2) in modules:
+#         # if name1 in layer_names:
+#         if 'ReLU' in name1 or force:  # only compute on activation
+#             out1 = m1(out1)
+#             m2_callable = copy.deepcopy(m1)
+#             m2_callable.load_state_dict(m2.state_dict())
+#             out2 = m2_callable(out2)
+#             sim = l2_sim_torch(out1, out2, sim_type='op_torch')
+#             sims_per_layer.append((name1, sim))
+#     pprint(sims_per_layer)
 
-    force = True
-    # force = False
-    mdl1 = hardcoded_3_layer_model(5, 1)
-    mdl2 = hardcoded_3_layer_model(5, 1)
-    batch_size = 4
-    X = torch.randn(batch_size, 5)
-    import copy
-    from uutils.torch_uu import l2_sim_torch
-    # get [..., s_l, ...] sim per layer (for this data set)
-    modules = zip(mdl1.named_children(), mdl2.named_children())
-    sims_per_layer = []
-    out1 = X
-    out2 = X
-    for (name1, m1), (name2, m2) in modules:
-        # if name1 in layer_names:
-        if 'ReLU' in name1 or force:  # only compute on activation
-            out1 = m1(out1)
-            m2_callable = copy.deepcopy(m1)
-            m2_callable.load_state_dict(m2.state_dict())
-            out2 = m2_callable(out2)
-            sim = l2_sim_torch(out1, out2, sim_type='op_torch')
-            sims_per_layer.append((name1, sim))
-    pprint(sims_per_layer)
-
-
-def anatome_test_are_same_nets_very_similar():
-    """
-    Same model with same data even if down sampled, should show similar nets.
-    """
-    from uutils.torch_uu.models import hardcoded_3_layer_model
-    B = 1024
-    Din = 524
-    downsample_size = 4
-    Dout = Din
-    mdl1 = hardcoded_3_layer_model(Din, Dout)
-    mdl2 = mdl1
-    # - layer name
-    # layer_name = 'fc0'
-    # layer_name = 'fc1'
-    layer_name = 'fc2'
-    # - data
-    X: torch.Tensor = torch.distributions.Uniform(low=-1, high=1).sample((B, Din))
-    scca_full: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None)
-    assert (abs(scca_full - 1.0) < 1e-5)
-    scca_downsampled: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=downsample_size)
-    assert (abs(scca_downsampled - 1.0) < 1e-5)
-
-
-def anatome_test_are_random_vs_pretrain_resnets_different():
-    """
-    random vs pre-trained nets should show different nets
-    - no downsample
-    - still true if downsample (but perhaps similarity increases, due to collapsing nets makes r.v.s
-    interact more btw each other, so correlation is expected to increase).
-    """
-    from torchvision.models import resnet18
-    B = 1024
-    C, H, W = 3, 64, 64
-    print(f'Din ~ {(C*H*W)=}')
-    downsample_size = 4
-    mdl1 = resnet18()
-    mdl2 = resnet18(pretrained=True)
-    # - layer name
-    # layer_name = 'bn1'
-    # layer_name = 'layer1.0.bn2'
-    # layer_name = 'layer2.1.bn2'
-    layer_name = 'layer4.1.bn2'
-    # layer_name = 'fc'
-    print(f'{layer_name=}')
-
-    # # -- we expect low CCA/sim since random nets vs pre-trained nets are different (especially on real data)
-    # # - random data test
-    X: torch.Tensor = torch.distributions.Uniform(low=-1, high=1).sample((B, C, H, W))
-    scca_full_random_data: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None, cxa_dist_type='pwcca')
-    # scca_full_random_data: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None, cxa_dist_type='lincka')
-    # scca_full_random_data: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None, cxa_dist_type='svcca')
-    print(f'Are random net & pre-trained net similar? They should not (so sim should be small):\n'
-          f'-> {scca_full_random_data=} (but might be more similar than expected on random data)')
-    # scca_downsampled: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=downsample_size)
-    # print(f'Are random net & pre-trained net similar? They should not (so sim should be small): {scca_downsampled=}')
 
-    #
-    mdl1 = resnet18()
-    mdl2 = resnet18(pretrained=True)
-    # - mini-imagenet test (the difference should be accentuated btw random net & pre-trained on real img data)
-    from uutils.torch_uu.dataloaders import get_set_of_examples_from_mini_imagenet
-    B = 512
-    k_eval: int = B  # num examples is about M = k_eval*(num_classes) = B*(num_classes)
-    X: torch.Tensor = get_set_of_examples_from_mini_imagenet(k_eval)
-    scca_full_mini_imagenet_data: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None)
-    scca_full_random_data: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None, cxa_dist_type='pwcca')
-    # scca_full_random_data: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None, cxa_dist_type='lincka')
-    # scca_full_random_data: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None, cxa_dist_type='svcca')
-    print(f'Are random net & pre-trained net similar? They should not (so sim should be small):\n'
-          f'{scca_full_mini_imagenet_data=} (the difference should be accentuated with real data, so lowest sim)')
-    print()
-    # assert(scca_full_mini_imagenet_data < scca_full_random_data), f'Sim should decrease, because the pre-trained net' \
-    #                                                               f'was trained on real images, so the weights are' \
-    #                                                               f'tuned for it but random weights are not, which' \
-    #                                                               f'should increase the difference so the sim' \
-    #                                                               f'should be lowest here. i.e. we want ' \
-    #                                                               f'{scca_full_mini_imagenet_data}<{scca_full_random_data}'
-    # scca_downsampled: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=downsample_size)
-    # print(f'Are random net & pre-trained net similar? They should not (so sim should be small): {scca_downsampled=}')
+# def anatome_test_are_same_nets_very_similar():
+#     """
+#     Same model with same data even if down sampled, should show similar nets.
+#     """
+#     from uutils.torch_uu.models import hardcoded_3_layer_model
+#     B = 1024
+#     Din = 524
+#     downsample_size = 4
+#     Dout = Din
+#     mdl1 = hardcoded_3_layer_model(Din, Dout)
+#     mdl2 = mdl1
+#     # - layer name
+#     # layer_name = 'fc0'
+#     # layer_name = 'fc1'
+#     layer_name = 'fc2'
+#     # - data
+#     X: torch.Tensor = torch.distributions.Uniform(low=-1, high=1).sample((B, Din))
+#     scca_full: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None)
+#     assert (abs(scca_full - 1.0) < 1e-5)
+#     scca_downsampled: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=downsample_size)
+#     assert (abs(scca_downsampled - 1.0) < 1e-5)
+
+
+# def anatome_test_are_random_vs_pretrain_resnets_different():
+#     """
+#     random vs pre-trained nets should show different nets
+#     - no downsample
+#     - still true if downsample (but perhaps similarity increases, due to collapsing nets makes r.v.s
+#     interact more btw each other, so correlation is expected to increase).
+#     """
+#     from torchvision.models import resnet18
+#     B = 1024
+#     C, H, W = 3, 64, 64
+#     print(f'Din ~ {(C*H*W)=}')
+#     downsample_size = 4
+#     mdl1 = resnet18()
+#     mdl2 = resnet18(pretrained=True)
+#     # - layer name
+#     # layer_name = 'bn1'
+#     # layer_name = 'layer1.0.bn2'
+#     # layer_name = 'layer2.1.bn2'
+#     layer_name = 'layer4.1.bn2'
+#     # layer_name = 'fc'
+#     print(f'{layer_name=}')
+#
+#     # # -- we expect low CCA/sim since random nets vs pre-trained nets are different (especially on real data)
+#     # # - random data test
+#     X: torch.Tensor = torch.distributions.Uniform(low=-1, high=1).sample((B, C, H, W))
+#     scca_full_random_data: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None, cxa_dist_type='pwcca')
+#     # scca_full_random_data: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None, cxa_dist_type='lincka')
+#     # scca_full_random_data: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None, cxa_dist_type='svcca')
+#     print(f'Are random net & pre-trained net similar? They should not (so sim should be small):\n'
+#           f'-> {scca_full_random_data=} (but might be more similar than expected on random data)')
+#     # scca_downsampled: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=downsample_size)
+#     # print(f'Are random net & pre-trained net similar? They should not (so sim should be small): {scca_downsampled=}')
+#
+#     #
+#     mdl1 = resnet18()
+#     mdl2 = resnet18(pretrained=True)
+#     # - mini-imagenet test (the difference should be accentuated btw random net & pre-trained on real img data)
+#     from uutils.torch_uu.dataloaders import get_set_of_examples_from_mini_imagenet
+#     B = 512
+#     k_eval: int = B  # num examples is about M = k_eval*(num_classes) = B*(num_classes)
+#     X: torch.Tensor = get_set_of_examples_from_mini_imagenet(k_eval)
+#     scca_full_mini_imagenet_data: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None)
+#     scca_full_random_data: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None, cxa_dist_type='pwcca')
+#     # scca_full_random_data: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None, cxa_dist_type='lincka')
+#     # scca_full_random_data: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=None, cxa_dist_type='svcca')
+#     print(f'Are random net & pre-trained net similar? They should not (so sim should be small):\n'
+#           f'{scca_full_mini_imagenet_data=} (the difference should be accentuated with real data, so lowest sim)')
+#     print()
+#     # assert(scca_full_mini_imagenet_data < scca_full_random_data), f'Sim should decrease, because the pre-trained net' \
+#     #                                                               f'was trained on real images, so the weights are' \
+#     #                                                               f'tuned for it but random weights are not, which' \
+#     #                                                               f'should increase the difference so the sim' \
+#     #                                                               f'should be lowest here. i.e. we want ' \
+#     #                                                               f'{scca_full_mini_imagenet_data}<{scca_full_random_data}'
+#     # scca_downsampled: float = sCXA(mdl1, mdl2, X, layer_name, downsample_size=downsample_size)
+#     # print(f'Are random net & pre-trained net similar? They should not (so sim should be small): {scca_downsampled=}')
 
 
 def anatome_test_what_happens_when_downsampling_increases_do_nets_get_more_similar_or_different():
     """
     - real, fake data
     - focus on pre-trained net since that is what I am comparing stuff during my research, not random nets.
     """
@@ -2962,38 +3044,38 @@
     pred = clipped_resnet(dummy_input)
     loss = pred.log().mean()
     loss.backward()
 
     print(clipped_resnet.fc.bias.grad[:25])
 
 
-def _resume_from_checkpoint_meta_learning_for_resnets_rfs_test():
-    import uutils
-    from uutils.torch_uu.models import reset_all_weights
-    import copy
-    # - get args to ckpt
-    args: Namespace = Namespace()
-    args.path_to_checkpoint: str = '~/data_folder_fall2020_spring2021/logs/nov_all_mini_imagenet_expts/logs_Nov05_15-44-03_jobid_668'
-    args: Namespace = uutils.make_args_from_metalearning_checkpoint(args=args,
-                                                                    path2args=args.path_to_checkpoint,
-                                                                    filename='args.json',
-                                                                    precedence_to_args_checkpoint=True,
-                                                                    it=37_500)
-    args: Namespace = uutils.setup_args_for_experiment(args)
-    # - get model from ckpt
-    mdl_ckpt, outer_opt, meta_learner = get_model_opt_meta_learner_to_resume_checkpoint_resnets_rfs(args,
-                                                                                                    path2ckpt=args.path_to_checkpoint,
-                                                                                                    filename='ckpt_file.pt')
-    # - mdl_rand
-    mdl_rand = copy.deepcopy(mdl_ckpt)
-    reset_all_weights(mdl_rand)
-    # - print if ckpt model is different from a random model
-    print(lp_norm(mdl_ckpt))
-    print(lp_norm(mdl_rand))
-    assert (lp_norm(mdl_ckpt) != lp_norm(mdl_rand))
+# def _resume_from_checkpoint_meta_learning_for_resnets_rfs_test():
+#     import uutils
+#     from uutils.torch_uu.models import reset_all_weights
+#     import copy
+#     # - get args to ckpt
+#     args: Namespace = Namespace()
+#     args.path_to_checkpoint: str = '~/data_folder_fall2020_spring2021/logs/nov_all_mini_imagenet_expts/logs_Nov05_15-44-03_jobid_668'
+#     args: Namespace = uutils.make_args_from_metalearning_checkpoint(args=args,
+#                                                                     path2args=args.path_to_checkpoint,
+#                                                                     filename='args.json',
+#                                                                     precedence_to_args_checkpoint=True,
+#                                                                     it=37_500)
+#     args: Namespace = uutils.setup_args_for_experiment(args)
+#     # - get model from ckpt
+#     mdl_ckpt, outer_opt, meta_learner = get_model_opt_meta_learner_to_resume_checkpoint_resnets_rfs(args,
+#                                                                                                     path2ckpt=args.path_to_checkpoint,
+#                                                                                                     filename='ckpt_file.pt')
+#     # - mdl_rand
+#     mdl_rand = copy.deepcopy(mdl_ckpt)
+#     reset_all_weights(mdl_rand)
+#     # - print if ckpt model is different from a random model
+#     print(lp_norm(mdl_ckpt))
+#     print(lp_norm(mdl_rand))
+#     assert (lp_norm(mdl_ckpt) != lp_norm(mdl_rand))
 
 
 # -- _main
 
 if __name__ == '__main__':
     # test_ned()
     # test_tensorify()
@@ -3001,9 +3083,9 @@
     # test_topk_accuracy_and_accuracy()
     # test_simple_determinism()
     # op_test()
     # anatome_test_are_same_nets_very_similar()
     # anatome_test_are_random_vs_pretrain_resnets_different()
     # verbose_exec_test()
     # feature_extractor_hook_test()
-    _resume_from_checkpoint_meta_learning_for_resnets_rfs_test()
+    # _resume_from_checkpoint_meta_learning_for_resnets_rfs_test()
     print('Done\a')
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/agents/synth_agents.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/agents/synth_agents.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/agents/tactic_predictor_tactician_agent.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/agents/tactic_predictor_tactician_agent.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/checkpointing_uu/__init__.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/checkpointing_uu/__init__.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/checkpointing_uu/meta_learning.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/checkpointing_uu/meta_learning.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/checkpointing_uu/supervised_learning.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/checkpointing_uu/supervised_learning.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,14 +40,17 @@
 
     Ref:
         - standard way: https://pytorch.org/tutorials/recipes/recipes/saving_and_loading_a_general_checkpoint.html
         - https://stackoverflow.com/questions/70129895/why-is-it-not-recommended-to-save-the-optimizer-model-etc-as-pickable-dillable
         - DDP checkpointing: https://stackoverflow.com/questions/70386800/what-is-the-proper-way-to-checkpoint-during-training-when-using-distributed-data
     """
     if is_lead_worker(args.rank):
+        print(f'saving checkpoint at: {(args.log_root/ckpt_filename)=}')
+        print(f'{type(args.model)=}')
+        print(f'{args.model_option=}')
         import pickle
         if not ignore_logger:
             args.logger.save_current_plots_and_stats() if hasattr(args, 'logger') else None
 
         # - ckpt
         args_pickable: Namespace = uutils.make_args_pickable(args)
         # note not saving any objects, to make sure checkpoint is loadable later with no problems
@@ -72,14 +75,15 @@
                     'scheduler_str': str(args.scheduler),
                     'scheduler_state_dict': try_to_get_scheduler_state_dict(args.scheduler),
                     'scheduler_hps': args.scheduler_hps,
                     'scheduler_option': args.scheduler_option,
                     },
                    pickle_module=pickle,
                    f=args.log_root / ckpt_filename)
+        print(f'saving checkpoint success at {(args.log_root/ckpt_filename)=}')
     return
 
 # todo - make a folder for it in models uutils and put this at the bottom
 # def load_model_resnet12_rfs(args: Namespace) -> nn.Module:
 #     pass
 #     # - get the hps of the model & build the instance
 #
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_data_preprocessing.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_data_preprocessing.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_dataset.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_dataset.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,29 @@
 
 from datasets import load_dataset, DatasetDict, Dataset
 
 from uutils import expanduser
 from uutils.torch_uu import approx_equal
 
 
+def get_data_set_with_tr_val_ts_splits(path2filename_train: Union[str, Path],
+                                       path2filename_test: Union[str, Path],
+                                       train_size: float = 0.9,
+                                       seed: int = 0,
+                                       ) -> DatasetDict:
+    expanduser(path2filename_train)
+    expanduser(path2filename_test)
+    train_dataset: Dataset = get_dataset_from_json_file(path2filename_train)
+    test_dataset: Dataset = get_dataset_from_json_file(path2filename_test)
+    # - split train to train & val randomly
+    train_val: DatasetDict = train_dataset.train_test_split(train_size=train_size, seed=seed)
+    dataset: DatasetDict = DatasetDict(train=train_val['train'], validation=train_val['test'], test=test_dataset)
+    return dataset
+
+
 def get_data_set_with_splits(all_data: Dataset,
                              train_size: float = 0.8,
                              validation_size: float = 0.1,
                              test_size: float = 0.1,
                              seed: int = 0,
                              ) -> DatasetDict:
     original_size: int = len(all_data)
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_tokenizer.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_tokenizer.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_trainer.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/data_uu/hf_uu_trainer.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/cifar100.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/cifar100.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 """
 from argparse import Namespace
 from pathlib import Path
 from typing import Optional, Callable
 
 import numpy as np
 import torch
-from PIL.Image import Image
+# from PIL.Image import Image
+import PIL.Image as Image
 from torch.utils.data import random_split, DataLoader
 from torchvision import datasets
 from torchvision.transforms import transforms
 
 from uutils.torch_uu.dataloaders.common import split_inidices, \
     get_serial_or_distributed_dataloaders
 
@@ -39,16 +40,16 @@
                    'augment_test': args.augment_train,
                    'num_workers': args.num_workers,
                    'pin_memory': args.pin_memory,
                    'rank': args.rank,
                    'world_size': args.world_size,
                    'merge': None
                    }
-    train_loader, val_loader = get_train_valid_loader(**train_kwargs)
-    test_loader: DataLoader = get_test_loader(**test_kwargs)
+    train_loader, val_loader = get_train_valid_loader_for_cirfar100(**train_kwargs)
+    test_loader: DataLoader = get_test_loader_for_cifar100(**test_kwargs)
     args.n_cls = 100  # all splits share same # classes
     dataloaders: dict = {'train': train_loader, 'val': val_loader, 'test': test_loader}
     return dataloaders
 
 
 def get_transform(augment: bool):
     if augment:
@@ -66,29 +67,29 @@
             lambda x: Image.fromarray(x),
             transforms.ToTensor(),
             normalize_cifar100
         ])
     return transform
 
 
-def get_train_valid_loader(data_path: Path,
-                           batch_size: int = 128,
-                           batch_size_eval: int = 64,
-                           seed: Optional[int] = None,
-                           augment_train: bool = True,
-                           augment_val: bool = False,
-                           val_size: Optional[float] = 0.2,
-                           shuffle: bool = False,  # false for reproducibility, and any split is as good as any other.
-                           num_workers: int = -1,
-                           pin_memory: bool = False,
-
-                           rank: int = -1,
-                           world_size: int = 1,
-                           merge: Optional[Callable] = None,
-                           ) -> tuple[DataLoader, DataLoader]:
+def get_train_valid_loader_for_cirfar100(data_path: Path,
+                                         batch_size: int = 128,
+                                         batch_size_eval: int = 64,
+                                         seed: Optional[int] = None,
+                                         augment_train: bool = True,
+                                         augment_val: bool = False,
+                                         val_size: Optional[float] = 0.2,
+                                         shuffle: bool = False,  # false for reproducibility, and any split is as good as any other.
+                                         num_workers: int = -1,
+                                         pin_memory: bool = False,
+
+                                         rank: int = -1,
+                                         world_size: int = 1,
+                                         merge: Optional[Callable] = None,
+                                         ) -> tuple[DataLoader, DataLoader]:
     """
     Utility function for loading and returning train and valid
     multi-process iterators over the CIFAR100 dataset. A sample
     9x9 grid of the images can be optionally displayed.
     If using CUDA, num_workers should be set to 1 and pin_memory to True.
     """
     # train_kwargs = {'batch_size': args.batch_size}
@@ -116,25 +117,25 @@
                                                                      merge,
                                                                      num_workers,
                                                                      pin_memory
                                                                      )
     return train_loader, val_loader
 
 
-def get_test_loader(data_path,
-                    batch_size_eval: int = 64,
-                    shuffle: bool = True,
-                    augment_test: bool = False,
-                    num_workers: int = -1,
-                    pin_memory=False,
-
-                    rank: int = -1,
-                    world_size: int = 1,
-                    merge: Optional[Callable] = None,
-                    ) -> DataLoader:
+def get_test_loader_for_cifar100(data_path,
+                                 batch_size_eval: int = 64,
+                                 shuffle: bool = True,
+                                 augment_test: bool = False,
+                                 num_workers: int = -1,
+                                 pin_memory=False,
+
+                                 rank: int = -1,
+                                 world_size: int = 1,
+                                 merge: Optional[Callable] = None,
+                                 ) -> DataLoader:
     """
     Utility function for loading and returning a multi-process
     test iterator over the CIFAR100 dataset.
     If using CUDA, num_workers should be set to 1 and pin_memory to True.
     Params
     ------
     - data_path: path directory to the dataset.
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/cifar100fs_fc100.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/cifar100fs_fc100.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/common.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/data_loader_cifar.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,178 +1,247 @@
 """
+Create train, val, test iterators for CIFAR-10 [1].
+Easily extended to MNIST, CIFAR-100 and Imagenet.
+[1]: https://discuss.pytorch.org/t/feedback-on-pytorch-for-kaggle-competitions/2252/4
 
-# - creating data train, val, test data sets & data laoders
-
-ref:
-    - https://stackoverflow.com/questions/70400439/what-is-the-proper-way-to-create-training-validation-and-test-set-in-pytorch-or
-
-# - data augmentation
-Current belief is that augmenting the validation set should be fine, especially if you want to actually encourage
-generalization since it makes the val set harder and it allows you to make val split percentage slightly lower since
-your validation set was increased size.
-
-For reproducibility of other work, especially for scientific pursues rather than "lets beat state of the art" - to make
-it easier to compare results use what they use. e.g. it seems only augmenting the train set is the common thing,
-especially when I looked at the augmentation strategies in min-imagenet and mnist.
-
-Test set augmentation helps mostly to make test set harder (so acc should go down) - but it also increases variance
-since the data size was increased. If you are reporting results most likely augmenting the data set is a good idea
-- especially if you are going to compute test set errors when comparing accuracy with previous work.
-Also, the way CI intervals are computed with t_p * std_n / sqrt n, means that the avg test error will be smaller, so
-you are fine in general.
-Default code I see doesn't augment test set so I most likely won't either.
-
-ref:
-    - https://stats.stackexchange.com/questions/320800/data-augmentation-on-training-set-only/320967#320967
-    - https://arxiv.org/abs/1809.01442, https://stats.stackexchange.com/a/390470/28986
-
-# - pin_memory
-For data loading, passing pin_memory=True to a DataLoader will automatically put the fetched data Tensors in pinned
-memory, and thus enables faster data transfer to CUDA-enabled GPUs. Note on pinning:
-This is an advanced tip. If you overuse pinned memory, it can cause serious problems when running low on RAM, and
-you should be aware that pinning is often an expensive operation. Thus, will leave it's default as False.
-
-ref:
-    - on pin_memory: https://pytorch.org/docs/stable/data.html
+https://gist.github.com/kevinzakka/d33bf8d6c7f06a9d8c76d97a7879f5cb
 """
-from typing import Callable, Optional, Union
 
-import numpy as np
 import torch
-from numpy.random import RandomState
-from torch.utils.data import Dataset, SubsetRandomSampler, random_split, DataLoader, RandomSampler
+import numpy as np
 
+from pathlib import Path
 
-def get_train_val_split_random_sampler(
-        train_dataset: Dataset,
-        val_dataset: Dataset,
-        val_size: float = 0.2,
-        batch_size: int = 128,
-        batch_size_eval: int = 64,
-        num_workers: int = 4,
-        pin_memory: bool = False
-        #     random_seed: Optional[int] = None,
-) -> tuple[DataLoader, DataLoader]:
-    """
-    Note:
-        - this will use different transforms for val and train if the objects you pass have different transforms.
-        - note train_dataset, val_dataset whill often be the same data set object but different instances with different
-        transforms for each data set.
-
-    Recommended use:
-        - this one is recommended when you want the train & val to have different transforms e.g. when doing scientific
-        work - instead of beating benchmark work - and the train, val sets had different transforms.
+#from utils import plot_images
+from torchvision import datasets
+from torchvision import transforms
+from torch.utils.data.sampler import SubsetRandomSampler
+
+from utils.utils import get_random_seed
+
+device = torch.device("cuda:0" if torch.cuda.is_available() else "cpu")
+
+CIFAR_DATA_PATH = Path('~/predicting_generalization/automl/data/').expanduser()
+
+def get_train_val_loader(data_dir,
+                           batch_size,
+                           augment,
+                           device,
+                           random_seed,
+                           val_size=0.1,
+                           shuffle=True,
+                           show_sample=False,
+                           num_workers=4):
+    '''
+    Utility function for loading and returning train and val
+    multi-process iterators over the CIFAR-10 dataset. A sample
+    9x9 grid of the images can be optionally displayed.
+    If using CUDA, num_workers should be set to 1 and pin_memory to True.
+    Params
+    ------
+    - data_dir: path directory to the dataset.
+    - batch_size: how many samples per batch to load.
+    - augment: whether to apply the data augmentation scheme
+      mentioned in the paper. Only applied on the train split.
+    - device: device
+    - random_seed: fix seed for reproducibility.
+    - val_size: percentage split of the training set used for
+      the valation set. Should be a float in the range [0, 1].
+    - shuffle: whether to shuffle the train/valation indices.
+    - show_sample: plot 9x9 sample grid of the dataset.
+    - num_workers: number of subprocesses to use when loading the dataset.
+
+    pin_memory: whether to copy tensors into CUDA pinned memory. Set it to
+      True if using GPU.
+    Returns
+    -------
+    - train_loader: training set iterator.
+    - val_loader: valation set iterator.
+    '''
+    pin_memory = False
+    if 'cuda' in device.type:
+        pin_memory = True
+
+    error_msg = "[!] val_size should be in the range [0, 1]."
+    assert ((val_size >= 0) and (val_size <= 1)), error_msg
+
+    normalize = transforms.Normalize(
+        mean=[0.4914, 0.4822, 0.4465],
+        std=[0.2023, 0.1994, 0.2010],
+    )
+    #normalize = transforms.Normalize((0.5,0.5,0.5),(0.5,0.5,0.5))
+
+    # define transforms
+    val_transform = transforms.Compose([
+            transforms.ToTensor(),
+            normalize,
+    ])
+    if augment:
+        train_transform = transforms.Compose([
+            transforms.RandomCrop(32, padding=4),
+            transforms.RandomHorizontalFlip(),
+            transforms.ToTensor(),
+            normalize,
+        ])
+    else:
+        train_transform = transforms.Compose([
+            transforms.ToTensor(),
+            normalize,
+        ])
+
+    # load the dataset
+    train_dataset = datasets.CIFAR10(
+        root=data_dir, train=True,
+        download=True, transform=train_transform,
+    )
+
+    val_dataset = datasets.CIFAR10(
+        root=data_dir, train=True,
+        download=True, transform=val_transform,
+    )
 
-    ref:
-        - https://gist.github.com/MattKleinsmith/5226a94bad5dd12ed0b871aed98cb123
-    """
-    assert 0 <= val_size <= 1.0, f"Error: {val_size} valid_size should be in the range [0, 1]."
     num_train = len(train_dataset)
     indices = list(range(num_train))
-    split_idx = int(np.floor(val_size * num_train))
-
-    # I don't think this is needed since later the sampler randomly samples data from a given list
-    # if shuffle == True:
-    #     np.random.seed(random_seed)
-    #     np.random.shuffle(indices)
+    split = int(np.floor(val_size * num_train))
 
-    train_idx, valid_idx = indices[:split_idx], indices[split_idx:]
-    assert len(train_idx) != 0 and len(valid_idx) != 0
+    if shuffle:
+        np.random.seed(random_seed)
+        np.random.shuffle(indices)
 
-    # Samples elements randomly from a given list of indices, without replacement.
+    train_idx, val_idx = indices[split:], indices[:split]
     train_sampler = SubsetRandomSampler(train_idx)
-    valid_sampler = SubsetRandomSampler(valid_idx)
-
-    train_loader = torch.utils.data.DataLoader(train_dataset,
-                                               batch_size=batch_size, sampler=train_sampler,
-                                               num_workers=num_workers, pin_memory=pin_memory)
-    valid_loader = torch.utils.data.DataLoader(val_dataset,
-                                               batch_size=batch_size_eval, sampler=valid_sampler,
-                                               num_workers=num_workers, pin_memory=pin_memory)
-    return train_loader, valid_loader
-
-
-def get_train_val_split_with_split(
-        train_dataset: Dataset,
-        train_val_split: list[int, int],  # e.g. [50_000, 10_000] for mnist
-        batch_size: int = 128,
-        batch_size_eval: int = 64,
-        num_workers: int = 4,
-        pin_memory: bool = False
-) -> tuple[DataLoader, DataLoader]:
-    """
-    Note:
-        - this will have the train and val sets have the same transform.
-
-    ref:
-        - https://gist.github.com/MattKleinsmith/5226a94bad5dd12ed0b871aed98cb123
-        - change transform: https://discuss.pytorch.org/t/changing-transforms-after-creating-a-dataset/64929/4
-    """
-    train_dataset, valid_dataset = random_split(train_dataset, train_val_split)
-    train_loader = torch.utils.data.DataLoader(train_dataset,
-                                               batch_size=batch_size, num_workers=num_workers, pin_memory=pin_memory)
-    valid_loader = torch.utils.data.DataLoader(valid_dataset,
-                                               batch_size=batch_size_eval, num_workers=num_workers,
-                                               pin_memory=pin_memory)
-    return train_loader, valid_loader
-
-
-def get_serial_or_distributed_dataloaders(train_dataset: Dataset,
-                                          val_dataset: Dataset,
-                                          batch_size: int = 128,
-                                          batch_size_eval: int = 64,
-                                          rank: int = -1,
-                                          world_size: int = 1,
-                                          merge: Optional[Callable] = None,
-                                          num_workers: int = -1,  # -1 means its running serially
-                                          pin_memory: bool = False,
-                                          ):
-    """
-
-    """
-    from uutils.torch_uu.distributed import is_running_serially
-    if is_running_serially(rank):
-        train_sampler = RandomSampler(train_dataset)
-        val_sampler = RandomSampler(val_dataset)
-        num_workers = 4 if num_workers == -1 else num_workers
-    else:
-        assert (batch_size >= world_size), f'Each worker must get at least one data point, so batch_size >= world_size' \
-                                           f'but got: {batch_size}{world_size}'
-        from torch.utils.data import DistributedSampler
-
-        # note: shuffle = True by default
-        train_sampler = DistributedSampler(train_dataset, num_replicas=world_size, rank=rank)
-        val_sampler = DistributedSampler(val_dataset, num_replicas=world_size, rank=rank)
-        # set the input num_workers but for ddp 0 is recommended afaik, todo - check
-        num_workers = 0 if num_workers == -1 else num_workers
-    # get dist dataloaders
-    train_loader = DataLoader(train_dataset,
-                              batch_size=batch_size,
-                              sampler=train_sampler,
-                              collate_fn=merge,
-                              num_workers=num_workers,
-                              pin_memory=pin_memory)
-    val_loader = DataLoader(val_dataset,
-                            batch_size=batch_size_eval,
-                            sampler=val_sampler,
-                            collate_fn=merge,
-                            num_workers=num_workers,
-                            pin_memory=pin_memory)
-    # return dataloaders
-    # dataloaders = {'train': train_dataloader, 'val': val_dataloader, 'test': test_dataloader}
-    # iter(train_dataloader)  # if this fails its likely your running in pycharm and need to set num_workers flag to 0
-    return train_loader, val_loader
-
-
-def split_inidices(indices: list,
-                   test_size: Optional = None,
-                   random_state: Optional[Union[int, RandomState, None]] = None,
-                   shuffle: bool = False,  # false for reproducibility, and any split is as good as any other.
-                   ) -> tuple[list[int], list[int]]:
-    import sklearn.model_selection
-    # - api: https://scikit-learn.org/stable/modules/generated/sklearn.model_selection.train_test_split.html
-    train_indices, val_indices = sklearn.model_selection.train_test_split(indices, test_size=test_size,
-                                                                          random_state=random_state,
-                                                                          shuffle=shuffle)
-    return train_indices, val_indices
+    val_sampler = SubsetRandomSampler(val_idx)
 
-# - visualization help
+    train_loader = torch.utils.data.DataLoader(
+        train_dataset, batch_size=batch_size, sampler=train_sampler,
+        num_workers=num_workers, pin_memory=pin_memory,
+    )
+    val_loader = torch.utils.data.DataLoader(
+        val_dataset, batch_size=batch_size, sampler=val_sampler,
+        num_workers=num_workers, pin_memory=pin_memory,
+    )
+
+    # visualize some images
+    if show_sample:
+        sample_loader = torch.utils.data.DataLoader(
+            train_dataset, batch_size=9, shuffle=shuffle,
+            num_workers=num_workers, pin_memory=pin_memory,
+        )
+        data_iter = iter(sample_loader)
+        images, labels = data_iter.next()
+        X = images.numpy().transpose([0, 2, 3, 1])
+        # plot_images(X, labels)
+
+    return (train_loader, val_loader)
+
+
+def get_test_loader(data_dir,
+                    batch_size,
+                    device,
+                    shuffle=True,
+                    num_workers=4):
+    '''
+    Utility function for loading and returning a multi-process
+    test iterator over the CIFAR-10 dataset.
+    If using CUDA, num_workers should be set to 1 and pin_memory to True.
+    Params
+    ------
+    - data_dir: path directory to the dataset.
+    - batch_size: how many samples per batch to load.
+    - device: device
+    - shuffle: whether to shuffle the dataset after every epoch.
+    - num_workers: number of subprocesses to use when loading the dataset.
+
+    pin_memory: whether to copy tensors into CUDA pinned memory. Set it to
+      True if using GPU.
+    Returns
+    -------
+    - data_loader: test set iterator.
+    '''
+    pin_memory = False
+    if 'cuda' in device.type:
+        pin_memory = True
+
+    normalize = transforms.Normalize(
+        mean=[0.485, 0.456, 0.406],
+        std=[0.229, 0.224, 0.225],
+    )
+    #normalize = transforms.Normalize((0.5,0.5,0.5),(0.5,0.5,0.5))
+
+    # define transform
+    transform = transforms.Compose([
+        transforms.ToTensor(),
+        normalize,
+    ])
+
+    dataset = datasets.CIFAR10(
+        root=data_dir, train=False,
+        download=True, transform=transform,
+    )
+
+    data_loader = torch.utils.data.DataLoader(
+        dataset, batch_size=batch_size, shuffle=shuffle,
+        num_workers=num_workers, pin_memory=pin_memory,
+    )
+
+    return data_loader
+
+def get_cifar10_for_data_point_mdl_gen(batch_size=512, num_workers=4, augment=False, random_seed=None):
+    '''
+    Gets the data sets for training the models that will be data points
+    '''
+    #data_dir = data_dir if data_dir is not None else CIFAR_DATA_PATH
+    data_dir = str(CIFAR_DATA_PATH)
+    #print(f'--> {data_dir}')
+    ##
+    val_size = 0.1
+    random_seed = get_random_seed() if random_seed is None else random_seed
+    #st()
+    trainloader, valloader = get_train_val_loader(data_dir, batch_size, augment, device, random_seed,
+                            val_size=val_size, shuffle=True, show_sample=False, num_workers=num_workers)
+    #st()
+    ##
+    batch_size_test = 1024
+    testloader = get_test_loader(data_dir, batch_size_test, device, shuffle=True, num_workers=num_workers)
+    return trainloader, valloader, testloader
+
+def get_cifar10_for_automl(batch_size=512, num_workers=4, augment=False, random_seed=None, val_size=0.5):
+    """
+
+    Args:
+        batch_size:
+        num_workers:
+        augment:
+        random_seed:
+        val_size:
+
+    Returns:
+
+    """
+    #data_dir = data_dir if data_dir is not None else CIFAR_DATA_PATH
+    data_dir = str(CIFAR_DATA_PATH)
+    ##
+    if random_seed is None:
+        random_seed = get_random_seed()
+    trainloader, valloader = get_train_val_loader(data_dir, batch_size, augment, device, random_seed,
+                            val_size=val_size, shuffle=True, show_sample=False, num_workers=num_workers)
+    ##
+    batch_size_test = 1024
+    testloader = get_test_loader(data_dir, batch_size_test, device, shuffle=True, num_workers=num_workers)
+    return trainloader, valloader, testloader
+
+def _dont_get_cifar10(batch_size=256, num_workers=4):
+    '''
+    DONT USE!!!!!!
+
+    get cifar10 data set
+    TODO: make batch, num_workers etc parameters
+    '''
+    error_msg = "---> ERROR: YOU ARE USING A FORBIDDEN METHOD!!!! STOP! \a"
+    print(error_msg)
+    raise ValueError(error_msg)
+    transform = transforms.Compose([transforms.ToTensor(),transforms.Normalize((0.5,0.5,0.5),(0.5,0.5,0.5))])
+    trainset = torchvision.datasets.CIFAR10(root='./data', train=True, download=True, transform=transform)
+    trainloader = torch.utils.data.DataLoader(trainset, batch_size=batch_size, shuffle=True, num_workers=num_workers)
+    testset = torchvision.datasets.CIFAR10(root='./data', train=False, download=True, transform=transform)
+    testloader = torch.utils.data.DataLoader(testset, batch_size=batch_size, shuffle=False, num_workers=num_workers)
+    return transform, trainset, trainloader, testset, testloader
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/download_coqgym_dataset.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/download_coqgym_dataset.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/download_miniimagenet.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/download_miniimagenet.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,18 +44,20 @@
         download_file_from_google_drive(file_id, path, filename_zip)
     else:
         print(f'Zip file to data set is already there at {path_2_zip}')
     # if actual data is not in appriopriate location extract it from zip to location
     extracted_dataset_path = path / 'miniImagenet'
     if not extracted_dataset_path.exists():
         # improve: https://stackoverflow.com/questions/3451111/unzipping-files-in-python
-        os.system(f'tar -xvzf {path_2_zip} -C {path}/')  # extract data set in above location i.e at path / 'miniImagenet'
+        os.system(
+            f'tar -xvzf {path_2_zip} -C {path}/')  # extract data set in above location i.e at path / 'miniImagenet'
     else:
         print(f'Extracted data set from zip is there already! Check it at: {extracted_dataset_path}')
 
+
 def download_and_extract_miniimagenet_rfs(path):
     """ Function to download miniImagent from google drive link.
     sources:
         - original: https://www.dropbox.com/sh/6yd1ygtyc3yd981/AABVeEqzC08YQv4UZk7lNHvya?dl=0
     """
     import os
     from torchvision.datasets.utils import download_file_from_google_drive, extract_archive
@@ -64,32 +66,34 @@
 
     file_id = '1rV3aj_hgfNTfCakffpPm7Vhpr1in87CR'
     filename_zip = 'miniImageNet.tar.gz'
     # if zip not there re-download it
     path_2_zip = path / filename_zip
     if not path_2_zip.exists():
         # download_file_from_google_drive(file_id, path, filename_zip)
-        assert(False)
+        assert (False)
     else:
         print(f'Zip file to data set is already there at {path_2_zip}')
     # if actual data is not in appriopriate location extract it from zip to location
     extracted_dataset_path = path / 'miniImagenet'
     if not extracted_dataset_path.exists():
         # improve: https://stackoverflow.com/questions/3451111/unzipping-files-in-python
-        os.system(f'tar -xvzf {path_2_zip} -C {path}/')  # extract data set in above location i.e at path / 'miniImagenet'
+        os.system(
+            f'tar -xvzf {path_2_zip} -C {path}/')  # extract data set in above location i.e at path / 'miniImagenet'
     else:
         print(f'Extracted data set from zip is there already! Check it at: {extracted_dataset_path}')
 
+
 if __name__ == "__main__":
     start = time.time()
     print('-> starting Downlooad')
 
     # dir to place mini-imagenet
     # path = Path('~/data/miniimagenet_meta_lstm/').expanduser()
     path = Path('~/data/miniImageNet_rfs/').expanduser()
     print(f'download path = {path}')
     # download_and_extract_miniimagenet(path)
     download_and_extract_miniimagenet_rfs(path)
 
     print('--> DONE')
     time_passed_msg, _, _, _ = report_times(start)
-    print(f'--> {time_passed_msg}')
+    print(f'--> {time_passed_msg}')
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/gaussian_1d_tasksets.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/gaussian_1d_tasksets.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/gaussian_nd_tasksets.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/gaussian_nd_tasksets.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/helpers.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,43 +1,58 @@
+"""
+Mosty likely Torchmeta.
+"""
 from argparse import Namespace
 from pathlib import Path
 
 from torch import nn
 
 
-def get_meta_learning_dataloader(args: Namespace) -> dict:
+def get_meta_learning_dataloaders(args: Namespace) -> dict:  # TorchMeta
+    """
+    Most likely Torchmeta
+    """
+    args.data_option = None if not hasattr(args, 'data_option') else args.data_option
     # Get Meta-Sets for few shot learning
     # if isinstance(args.data_path, Path):
     if args.data_option == 'Path':
         # if path is given use the path
         if 'fully_connected' in str(args.data_path.name):
             from uutils.torch_uu.dataloaders import get_torchmeta_rand_fnn_dataloaders
-            args.dataloaders = get_torchmeta_rand_fnn_dataloaders(args)
+            dataloaders = get_torchmeta_rand_fnn_dataloaders(args)
             raise NotImplementedError
         else:
             raise ValueError(f'Not such task: {args.data_path}')
     else:
         if args.data_option == 'torchmeta_miniimagenet':
             from uutils.torch_uu.dataloaders.meta_learning.torchmeta_ml_dataloaders import \
                 get_miniimagenet_dataloaders_torchmeta
-            args.dataloaders = get_miniimagenet_dataloaders_torchmeta(args)
+            dataloaders = get_miniimagenet_dataloaders_torchmeta(args)
             # raise NotImplementedError
         elif args.data_option == 'torchmeta_cifarfs':
             from uutils.torch_uu.dataloaders.meta_learning.torchmeta_ml_dataloaders import \
                 get_cifarfs_dataloaders_torchmeta
-            args.dataloaders = get_cifarfs_dataloaders_torchmeta(args)
+            dataloaders = get_cifarfs_dataloaders_torchmeta(args)
         elif args.data_option == 'torchmeta_sinusoid':
             from uutils.torch_uu.dataloaders import get_torchmeta_sinusoid_dataloaders
-            args.dataloaders = get_torchmeta_sinusoid_dataloaders(args)
+            dataloaders = get_torchmeta_sinusoid_dataloaders(args)
             raise NotImplementedError
         elif args.data_option == 'rfs_meta_learning_miniimagenet':
             from uutils.torch_uu.dataloaders.meta_learning.rfs_meta_learning_data_loaders import \
                 get_rfs_meta_learning_mi_dataloader
-            args.dataloaders = get_rfs_meta_learning_mi_dataloader(args)
+            dataloaders = get_rfs_meta_learning_mi_dataloader(args)
+        elif args.data_option == 'mds':
+            # todo, would be nice to move this code to uutils @patrick so import is from uutils
+            from diversity_src.dataloaders.metadataset_episodic_loader import get_mds_loaders
+            dataloaders: dict = get_mds_loaders(args)
+            for split in dataloaders.keys():
+                dataloaders[split].episodic_batch_2_task_dataset = True
+            # [setattr(dataloaders[split], 'episodic_batch_2_task_dataset', True) for split in dataloaders.keys()]
         elif 'l2l_data' in str(args.data_path):
+            # -- Converts a l2l data set as torchmeta data loader. Returns a batch of tasks, the way that torchmeta would.
             # note: this line is mainly intended for data ananlysis! not meant for ddp, see this if you want that but idk if it will work: https://github.com/learnables/learn2learn/issues/263
             from uutils.torch_uu.dataloaders.meta_learning.l2l_to_torchmeta_dataloader import \
                 get_l2l_torchmeta_dataloaders
-            args.dataloaders: dict = get_l2l_torchmeta_dataloaders(args)
+            dataloaders: dict = get_l2l_torchmeta_dataloaders(args)  # respects normal pytorch dl api afaik
         else:
             raise ValueError(f'Not such task: {args.data_path}')
-        return args.dataloaders
+        return dataloaders
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/rfs_meta_learning_data_loaders.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/rfs_meta_learning_data_loaders.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/torchmeta_ml_dataloaders.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/torchmeta_ml_dataloaders.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 from torchmeta.utils.data import BatchMetaDataLoader
 from torchvision import transforms as transforms
 
 import urllib.request
 
 from pathlib import Path
 
+from uutils import report_times, expanduser
+
 
 def process_batch_sl(args, batch):
     batch_x, batch_y = batch
     if torch.cuda.is_available():
         if args.device:
             batch_x, batch_y = batch_x.to(args.device), batch_y.to(args.device)
         else:
@@ -105,21 +107,24 @@
     if miniimagenet is not in that path it will download it later on.
 
     Note:
         - this is a weird hack since the torchmeta helper functions doesn't let me just pass the actual path to the folder
         containing the dataset but instead wants the path to the folder containing the data set instead of the direct
         path to the data set.
     """
+    dummy_datapath: Path = expanduser(dummy_datapath)
     if dummy_datapath == 'miniimagenet':
         # - this is the location torchmeta expects to be pointed to
         data_path: Path = Path('//').expanduser()
-    else:
+    elif '/data/miniimagenet' in str(dummy_datapath):
         # splits by folder removes the word miniimagenet and gives the real path to torchmeta's miniimagenet
         # -- ~/data/miniimagenet/ -> ~/data/
         data_path: Path = Path('/'.join(str(dummy_datapath.expanduser()).split('/')[:-1]))
+    else:
+        data_path: Path = expanduser('~/data/')
     return data_path
 
 
 def get_miniimagenet_datasets_torchmeta(args: Namespace) -> dict:
     """
     Note:
         - torchmeta considers the path to the data set the path to the folder where the folder containing the dataset
@@ -160,14 +165,19 @@
     # - mini-imagenet has C(64,5) exponential # of tasks so 1 epoch is intractable, don't train with epochs
     # and for now all training is done with classification
     args.trainin_with_epochs = False
     args.criterion = nn.CrossEntropyLoss()
     # - get data sets
     datasets = get_miniimagenet_datasets_torchmeta(args)
     # - get dataloaders
+    if not hasattr(args, 'meta_batch_size_train'):
+        args.meta_batch_size_train = 4
+    if not hasattr(args, 'meta_batch_size_eval'):
+        args.meta_batch_size_eval = 2
+    args.num_workers = 4 if args.num_workers == -1 or args.num_workers is None else args.num_workers
     meta_train_dataloader = BatchMetaDataLoader(datasets['train'],
                                                 batch_size=args.meta_batch_size_train,
                                                 num_workers=args.num_workers)
     meta_val_dataloader = BatchMetaDataLoader(datasets['val'],
                                               batch_size=args.meta_batch_size_eval,
                                               num_workers=args.num_workers)
     meta_test_dataloader = BatchMetaDataLoader(datasets['test'],
@@ -257,34 +267,41 @@
     args.k_eval = k_eval
     args.meta_batch_size_train = meta_batch_size
     args.meta_batch_size_eval = meta_batch_size
     args.num_workers = num_workers
     return args
 
 
-def get_minimum_args_for_torchmeta_mini_imagenet_dataloader(data_path: Path = Path('//'),
-                                                            k_eval: int = 15, k_shots: int = 5,
-                                                            n_classes: int = 5,
-                                                            meta_batch_size_train: int = 2,
-                                                            meta_batch_size_eval: int = 2,
-                                                            num_workers: int = 0) -> Namespace:
+def get_minimum_args_for_torchmeta_mini_imagenet_dataloader(
+        data_path: Path = Path('~/data/torchmeta_data/miniimagenet'),
+        k_eval: int = 15, k_shots: int = 5,
+        n_classes: int = 5,
+        meta_batch_size_train: int = 2,
+        meta_batch_size_eval: int = 2,
+        num_workers: int = 0) -> Namespace:
     """
     Gets the minimum args for torchmeta mini imagenet dataloader to work.
 
     Note, you can update default values if you want.
     """
     args: Namespace = Namespace()
     args.data_path = data_path.expanduser()  # for some datasets this is enough
     args.n_classes = n_classes
     args.k_shots = k_shots
     args.k_eval = k_eval
     args.meta_batch_size_train = meta_batch_size_train
     args.meta_batch_size_eval = meta_batch_size_eval
     args.num_workers = num_workers
     args.device = uutils.torch_uu.get_device()
+    # - new to force seeing torchmeta imgs
+    args.jobid = -1
+    args.log_freq = 1
+    args.lr = None
+    args.n_cls = 5
+    args.seed = 0
     return args
 
 
 def get_set_of_examples_from_mini_imagenet(k_eval: int = 15) -> torch.Tensor:
     from uutils.torch_uu import process_meta_batch
     args: Namespace = Namespace()
     args.data_path = Path('//').expanduser()  # for some datasets this is enough
@@ -385,14 +402,15 @@
 
 def get_cifarfs_dataloaders_torchmeta(args: Namespace) -> dict:
     args.criterion = nn.CrossEntropyLoss()
     # - get data sets
     datasets = get_cifarfs_datasets_torchmeta(args)
 
     # - get dataloaders
+    args.num_workers = 4 if args.num_workers == -1 or args.num_workers is None else args.num_workers
     meta_train_dataloader = BatchMetaDataLoader(datasets['train'],
                                                 batch_size=args.meta_batch_size_train,
                                                 num_workers=args.num_workers)
     meta_val_dataloader = BatchMetaDataLoader(datasets['val'],
                                               batch_size=args.meta_batch_size_eval,
                                               num_workers=args.num_workers)
     meta_test_dataloader = BatchMetaDataLoader(datasets['test'],
@@ -402,14 +420,15 @@
     dataloaders = {'train': meta_train_dataloader, 'val': meta_val_dataloader, 'test': meta_test_dataloader}
     return dataloaders
 
 
 # -- Sinusoid
 
 def get_torchmeta_sinusoid_dataloaders(args):
+    args.num_workers = 4 if args.num_workers == -1 or args.num_workers is None else args.num_workers
     dataset = sinusoid(shots=args.k_eval, test_shots=args.k_eval)
     train_dataloader = BatchMetaDataLoader(dataset, batch_size=args.meta_batch_size_train,
                                            num_workers=args.num_workers)
     val_dataloader = BatchMetaDataLoader(dataset, batch_size=args.meta_batch_size_eval,
                                          num_workers=args.num_workers)
     test_dataloader = BatchMetaDataLoader(dataset, batch_size=args.meta_batch_size_eval,
                                           num_workers=args.num_workers)
@@ -418,14 +437,15 @@
     return dataloaders
 
 
 # -- rand_fnn
 
 def get_torchmeta_rand_fnn_dataloaders(args):
     # get data
+    from uutils.torch_uu.data_uu.synthetic.rand_fnn import RandFNN
     dataset_train = RandFNN(args.data_path, 'train')
     dataset_val = RandFNN(args.data_path, 'val')
     dataset_test = RandFNN(args.data_path, 'test')
     # get meta-sets
     metaset_train = ClassSplitter(dataset_train,
                                   num_train_per_class=args.k_shots,
                                   num_test_per_class=args.k_eval,
@@ -433,14 +453,15 @@
     metaset_val = ClassSplitter(dataset_val, num_train_per_class=args.k_shots,
                                 num_test_per_class=args.k_eval,
                                 shuffle=True)
     metaset_test = ClassSplitter(dataset_test, num_train_per_class=args.k_shots,
                                  num_test_per_class=args.k_eval,
                                  shuffle=True)
     # get meta-dataloader
+    args.num_workers = 4 if args.num_workers == -1 or args.num_workers is None else args.num_workers
     train_dataloader = BatchMetaDataLoader(metaset_train,
                                            batch_size=args.meta_batch_size_train,
                                            num_workers=args.num_workers)
     val_dataloader = BatchMetaDataLoader(metaset_val,
                                          batch_size=args.meta_batch_size_eval,
                                          num_workers=args.num_workers)
     test_dataloader = BatchMetaDataLoader(metaset_test,
@@ -469,23 +490,25 @@
     train_dataset = dataset(args, split='train')
     val_dataset = dataset(args, split='val')
     test_dataset = dataset(args, split='test')
     if is_running_serially(rank):
         train_sampler, val_sampler, test_sampler = None, None, None
         # args.num_workers = args.num_workers if hasattr(args, 'num_workers') else 4
         args.num_workers = 4
+        args.num_workers = 4 if args.num_workers == -1 or args.num_workers is None else args.num_workers
     else:
         # get dist samplers
         assert (args.batch_size >= world_size)
         from torch.utils.data import DistributedSampler
         train_sampler = DistributedSampler(train_dataset, num_replicas=world_size, rank=rank)
         val_sampler = DistributedSampler(val_dataset, num_replicas=world_size, rank=rank)
         test_sampler = DistributedSampler(test_dataset, num_replicas=world_size, rank=rank)
         # todo - figure out what is the best for ddp. But my guess is that 0 is fine as hardcoded value & only overwrite if args.num_wokers has a none -1 or none else use my hardcoded default
         args.num_workers = 0
+        args.num_workers = 0 if args.num_workers == -1 or args.num_workers is None else args.num_workers
     # get dist dataloaders
     train_dataloader = DataLoader(train_dataset,
                                   batch_size=args.batch_size,
                                   sampler=train_sampler,
                                   collate_fn=merge,
                                   num_workers=args.num_workers)
     val_dataloader = DataLoader(val_dataset,
@@ -570,12 +593,10 @@
 
         print(f'Test inputs shape: {qry_x.size()}')  # (2, 75, 3, 28, 28)
         print(f'Test targets shape: {qry_y.size()}')  # (2, 75)
         break
 
 
 if __name__ == '__main__':
-    from uutils import report_times
-
     start = time.time()
     mini_imagenet_loop()
     print(f'Time passed: {report_times(start)}')
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/transforms_cfg_rfs.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_learning/transforms_cfg_rfs.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_lstm_dataloader.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/meta_lstm_dataloader.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/miniimagenet_rfs.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/miniimagenet_rfs.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/mnist.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/mnist.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/unzip_coqgym_dataset.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataloaders/unzip_coqgym_dataset.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/dataset/rfs_mini_imagenet.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/dataset/rfs_mini_imagenet.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/distributed.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/distributed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 For code used in distributed training.
 """
 
 import time
+import uutils
 from argparse import Namespace
 from pathlib import Path
 from typing import Tuple, Union, Callable, Any, Optional
 
 import torch
 import torch.distributed as dist
 
@@ -18,14 +19,22 @@
 
 from torch.utils.data import Dataset, DataLoader, DistributedSampler
 
 import os
 
 from pdb import set_trace as st
 
+from uutils.torch_uu import get_device
+
+
+def get_default_world_size() -> int:
+    """ Get the number of GPUs available to the current process, otherwise return 1 (e.g in cpu case). """
+    world_size: int = torch.cuda.device_count() if torch.cuda.is_available() else 1
+    return world_size
+
 
 def set_gpu_id_if_available_simple(args):
     """
     Main idea is args.gpu = rank for simple case except in debug/serially running.
 
     :param args:
     :return:
@@ -33,30 +42,31 @@
     if torch.cuda.is_available():
         # if running serially then there is only 1 gpu the 0th one otherwise the rank is the gpu in simple cases
         args.gpu = 0 if is_running_serially(args.rank) else args.rank  # makes sure code works with 1 gpu and serially
     else:
         args.gpu = torch.device("cuda" if torch.cuda.is_available() else "cpu")
 
 
-def set_devices(args):
+def set_devices(args, verbose: bool = False):
     """
-    Set device to the gpu id if its distributed pytorch parallel otherwise to the device available.
+    Set device to the gpu id, but if its distributed ddp (via rank) otherwise to the device available.
 
-    :param args:
-    :return:
+    Note:
+        - this code is used in the main() or train() code -- for each rank, even serially -- not in the set_up_args() code.
+        Because to get the right gpu_idx it we need to know the rank.
+        - reason we don't just do args.device = ... is because we have this if statement to check if we are parallel
+        or not and set it according to the rank if using parallel.
     """
     if is_running_serially(args.rank):
-        args.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+        args.device = get_device()  # serial so no gpu_idx given nor rank given, so cpu or cuda:0
     else:
-        args.device = args.rank
-
-    # todo - I'm not sure if the code bellow should be here...
-    if is_running_parallel(args.rank):
-        if str(torch.device("cuda" if torch.cuda.is_available() else "cpu")) != 'cpu':
-            torch.cuda.set_device(args.device)  # is this right if we do parallel cpu?
+        assert args.rank != -1, "Error: running in parallel but rank is -1 (serial)."
+        args.device = get_device(args.rank)
+    if verbose:
+        print(f"{args.device=}")
 
 
 def set_devices_and_seed_ala_l2l(args: Namespace, seed: Optional[None] = None, cuda: bool = True) -> torch.device:
     """
     original code:
 
     print(rank)
@@ -76,70 +86,65 @@
     else:
         args.device = torch.device('cpu')
         if cuda and torch.cuda.device_count():
             device_id = args.rank % torch.cuda.device_count()
             args.device = torch.device('cuda:' + str(device_id))
         print(args.rank, ':', args.device)
 
-    # - set seed
-    import random
-    import numpy as np
-
+    # -- set seed, so all processes in distributed training will act differently my modifying seed using their ags.rank
+    # - note, this assumes either the seed is passed from args.seed and thus the user or the setup code has set the seed
+    # if seed is not set in this function (seed is None or -1) then get the one from the args (note it might still not be set by the user), else if set then use the one passed in.
     seed: int = args.seed if seed is None else seed
-    # rank: int = torch.distributed.get_rank()
-    seed += args.rank
-    random.seed(seed)
-    np.random.seed(seed)
-    if cuda and torch.cuda.device_count():
-        torch.manual_seed(seed)
-        # sebas code doesn't have this so I am leaving it out.
-        # if is_running_parallel(args.rank):
-        #     if str(torch.device("cuda" if torch.cuda.is_available() else "cpu")) != 'cpu':
-        #         torch.cuda.set_device(args.device)  # is this right if we do parallel cpu?
+    # rank: int = torch.distributed.get_rank()  # this is what sebas does but we should've already have a rank
+    seed += args.rank  # create see from rank so that process acts different and all of em don't just do the same thing
+    # once a seed for each rank has been decided, set it
+    uutils.seed_everything(seed)
+
+    # - set seed
+    # import random
+    # import numpy as np
+    # random.seed(seed)
+    # np.random.seed(seed)
+    # if cuda and torch.cuda.device_count():
+    #     torch.manual_seed(seed)
+    #     # sebas code doesn't have this so I am leaving it out.
+    #     # if is_running_parallel(args.rank):
+    #     #     if str(torch.device("cuda" if torch.cuda.is_available() else "cpu")) != 'cpu':
+    #     #         torch.cuda.set_device(args.device)  # is this right if we do parallel cpu?
 
 
 # torch.cuda.manual_seed(seed)
 
 
 def process_batch_ddp(args: Namespace, batch: Any) -> tuple[Tensor, Tensor]:
     """
     Make sure args has the gpu for each worker.
 
     :param args:
     :param batch:
     :return:
     """
-    x, y = batch
-    if type(x) == torch.Tensor:
-        # x = x.to(args.gpu)
-        x = x.to(args.device)
-    if type(y) == torch.Tensor:
-        # y = y.to(args.gpu)
-        y = y.to(args.device)
-    return x, y
-
-
-def process_batch_ddp_union_rfs(args: Namespace, batch: Any) -> tuple[Tensor, Tensor]:
-    """
-    Make sure args has the gpu for each worker.
-
-    :param args:
-    :param batch:
-    :return:
-    """
+    # weird == 3 due to rfs I think, see: ref: https://github.com/WangYueFt/rfs/
     if len(batch) == 3:
         x, y, _ = batch
     elif len(batch) == 2:
         x, y = batch
     else:
         # img, target, item, sample_idx = batch
-        x, y, item, sample_idx = batch
+        # x, y, item, sample_idx = batch
         raise NotImplementedError
-    x = x.to(args.device)
-    y = y.to(args.device)
+    # if isinstance(batch, dict):
+    #     x, y = batch['train'][0], batch['train'][1]
+    #     # x, y = batch['test'][0], batch['test'][1]
+    if type(x) == torch.Tensor:
+        # x = x.to(args.gpu)
+        x = x.to(args.device)
+    if type(y) == torch.Tensor:
+        # y = y.to(args.gpu)
+        y = y.to(args.device)
     return x, y
 
 
 def move_to_ddp_gpu_via_dict_mutation(args: Namespace, batch: dict) -> dict:
     # temporary fix for backwards compatibility
     return move_model_to_ddp_gpu_via_dict_mutation(args, batch)
 
@@ -323,20 +328,27 @@
         #     world_size=world_size,
         # )
         # dist.init_process_group(backend=backend, init_method="env://")
         # dist.init_process_group(backend=backend, init_method=None)
         # torch.distributed.barrier()  # causes this warning: https://github.com/pytorch/pytorch/issues/60752
 
 
-def cleanup(rank):
+def cleanup(rank: int,
+            clean_up_wand: bool = False,
+            args: Optional[Namespace] = None,
+            ):
     """ Destroy a given process group, and deinitialize the distributed package """
     # only destroy the process distributed group if the code is not running serially
     if is_running_parallel(rank):
         torch.distributed.barrier()
         dist.destroy_process_group()
+    if clean_up_wand:
+        # cleanup_wandb(args, delete_wandb_dir=True)
+        from uutils.logging_uu.wandb_logging.common import cleanup_wandb
+        cleanup_wandb(args, delete_wandb_dir=False)
 
 
 def get_batch(batch: Tuple[Tensor, Tensor], rank) -> Tuple[Tensor, Tensor]:
     x, y = batch
     if torch.cuda.is_available():
         x, y = x.to(rank), y.to(rank)
     else:
@@ -408,39 +420,57 @@
 
     :param rank:
     :param args:
     :param model:
     :param force: force is meant to force it into DDP. Meant for debugging.
     :return:
     """
+    # - set device if not set, don't put in setup args because need to running this in it's own python process & rank if it's running parallel
+    if not hasattr(args, 'device'):
+        set_devices(args)  # this sets device if parallel or serial correctly using rank
+    if args.device is None:
+        set_devices(args)  # this sets device if parallel or serial correctly using rank
+    # - move model to device
     if is_running_parallel(rank) or force:
         # model.criterion = self.args.criterion.to(rank)  # I think its not needed since I already put it in the TP so when TP is moved to DDP the rank is moved automatically I hope
         # if gpu avail do the standard of creating a model and moving the model to the GPU with id rank
         if torch.cuda.is_available():
             # create model and move it to GPU with id rank
             model = model.to(args.device)
             model = DistributedDataParallel(model, find_unused_parameters=True, device_ids=[args.device])
         else:
             # if we want multiple cpu just make sure the model is shared properly accross the cpus with shared_memory()
             # note that op is a no op if it's already in shared_memory
             model = model.share_memory()
             model = DistributedDataParallel(model,
                                             find_unused_parameters=True)  # I think removing the devices ids should be fine...
     else:  # running serially
+        # args.device = get_device()  # not needed anymore
         model = model.to(args.device)
     return model
 
 
 def move_model_to_dist_device_or_serial_device(rank: int, args: Namespace, model: nn.Module, force: bool = False):
-    if not hasattr(args, 'dist_option'):
-        # for backwards compatibility, default try to do ddp or just serial to device
+    """
+    Moves the model to the right device & handles the case when we are using the special l2l_distributed option in
+    args.dist_option. Otherwise, it just behave as expected, move the model to gpu:0 (or cpu) if serial and to the
+    right gpu if running in parallel according to the args.rank.
+
+    Note:
+        - this code is only needed because of l2l distributed. For that set flag args.dist_option = 'l2l_dist'.
+        Otherwise, don't worry about it.
+    """
+    # set_devices(args)
+    if not hasattr(args, 'dist_option'):  # this flag is not needed unless your running l2l_dist.
+        # just more device according to serial or ddp. Doesn't handle l2l special case
         model = move_model_to_ddp(rank, args, model, force)
     else:
         if args.dist_option == 'ddp':
-            model = move_model_to_ddp(rank, args, model, force)
+            # model = move_model_to_ddp(rank, args, model, force)
+            raise ValueError(f'Error: {args.dist_option=} is not needed anymore.')
         elif args.dist_option == 'l2l_dist':
             # based on https://github.com/learnables/learn2learn/issues/263
             model = model.to(args.device)  # this works for serial and parallel (my guess, just moves to proc's device)
         elif is_running_serially(args.rank):
             model = move_model_to_ddp(rank, args, model, force)
         else:
             raise ValueError(f'Not a valid way to move a model to (dist) device: {args.dist_option=}')
@@ -556,14 +586,15 @@
         torch.distributed.barrier()
         if rank != 0:
             time.sleep(1)
 
 
 def dist_log(msg: str, rank, flush: bool = False, use_pprint: bool = False):
     """Prints only if the current process is the leader (e.g. rank = -1)."""
+    #         torch.distributed.barrier() # could be used to sync prints?
     if is_lead_worker(rank):
         if not use_pprint:
             print(msg, flush=flush)
         else:
             from pprint import pprint
             pprint(msg)
 
@@ -588,14 +619,36 @@
     try:
         local_rank: int = int(os.environ["LOCAL_RANK"])
     except:
         local_rank: int = -1
     return local_rank
 
 
+def is_main_process_using_local_rank() -> bool:
+    """
+    Determines if it's the main process using the local rank.
+
+    based on print statements:
+        local_rank=0
+        local_rank=1
+
+    other ref:
+        # - set up processes a la l2l
+        local_rank: int = get_local_rank()
+        print(f'{local_rank=}')
+        init_process_group_l2l(args, local_rank=local_rank, world_size=args.world_size, init_method=args.init_method)
+        rank: int = torch.distributed.get_rank() if is_running_parallel(local_rank) else -1
+        args.rank = rank  # have each process save the rank
+        set_devices_and_seed_ala_l2l(args)  # args.device = rank or .device
+        print(f'setup process done for rank={args.rank}')
+    """
+    local_rank: int = get_local_rank()
+    return local_rank == -1 or local_rank == 0  # -1 means serial, 0 likely means parallel
+
+
 # -- tests
 
 # - hello world parallel test (no ddp)
 
 def runfn_test(rank, args, world_size, master_port):
     args.gpu = rank
     setup_process(rank, world_size, master_port)
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/eval/my_eval_fewshot_rfs.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/eval/my_eval_fewshot_rfs.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/eval/my_meta_eval_rfs.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/eval/my_meta_eval_rfs.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/mains/main_meta_learning.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/mains/main_meta_learning.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 from uutils.torch_uu.distributed import is_lead_worker
 
 
 def manual_args_load() -> Namespace:
     """
     Manually load args.
 
-    Divided into three parts (due to legacy code)
+    Divided into three parts (due to legacy_mains code)
     1. parse args from terminal
     2. manually load args in this script
     3. add remaining common setup args to experiment
 
     :param args:
     :return:
     """
@@ -286,15 +286,15 @@
         args.base_model.cuda()
     print(f'{args.base_model=}')
 
     # Set up Meta-Learner
     args.scheduler = None
     if args.meta_learner_name == 'maml_fixed_inner_lr':
         args.grad_clip_rate = None
-        args.meta_learner = MAMLMetaLearner(args, args.base_model, fo=args.fo, lr_inner=args.inner_lr)
+        args.meta_learner = MAMLMetaLearner(args, args.base_model, fo=args.fo, inner_lr=args.inner_lr)
         args.outer_opt = optim.Adam(args.meta_learner.parameters(), args.outer_lr)
         # args.outer_opt = Adafactor(args.meta_learner.parameters(), scale_parameter=True, relative_step=True, warmup_init=True, lr=None)
         # args.scheduler = AdafactorSchedule(args.outer_opt)
     elif args.meta_learner_name == "FitFinalLayer":
         args.meta_learner = FitFinalLayer(args, args.base_model)
         args.inner_opt_name = 'PFF'
         args.outer_opt = 'None'
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/mains/main_sl_with_ddp.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/mains/main_sl_with_ddp.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/mains/main_synth.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/mains/main_synth.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/maml_differentiable_optimizer.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/maml_differentiable_optimizer.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import torch
 from higher.patch import _MonkeyPatchBase
 from torch import nn
 from torch import optim
 from torch import Tensor
 from torch.optim.optimizer import required
 
-from anatome.helper import LayerIdentifier, dist_data_set_per_layer
+# from anatome.helper import LayerIdentifier, dist_data_set_per_layer
 # from meta_learning.meta_learners.pretrain_convergence import get_adapted_according_to_ffl
 
 from pdb import set_trace as st
 
 from uutils.torch_uu import tensorify
 from uutils.torch_uu.metrics.confidence_intervals import torch_compute_confidence_interval, \
     mean_confidence_interval
@@ -76,16 +76,16 @@
                         buf = _add(buf.mul(momentum), 1 - dampening, g)
                         param_state['momentum_buffer'] = buf
                     if nesterov:
                         g = _add(g, momentum, buf)
                     else:
                         g = buf
 
-                if self.fo:  # first-order
-                    g = g.detach()  # dissallows flow of higher order grad while still letting params track gradients.
+                # if self.fo:  # first-order
+                #     g = g.detach()  # dissallows flow of higher order grad while still letting params track gradients.
                 group['params'][p_idx] = _add(p, -group['lr'], g)
 
 
 higher.register_optim(NonDiffMAML, MAML)
 
 
 def get_maml_inner_optimizer(model: nn.Module, inner_lr: float) -> NonDiffMAML:
@@ -176,24 +176,27 @@
     # - get fmodel and diffopt ready for inner adaptation
     # base_model.train() if training else base_model.eval()
     fmodel, diffopt = get_diff_optimizer_and_functional_model(base_model,
                                                               inner_opt,
                                                               copy_initial_weights=copy_initial_weights,
                                                               track_higher_grads=track_higher_grads)
     # - do inner addptation using task/support set
-    # print(f'>maml_new (before inner adapt): {fmodel.model.features.conv1.weight.norm(2)=}')
-    diffopt.fo = fo
+    # diffopt.fo = fo
     base_model.train() if training else base_model.eval()
     for i_inner in range(nb_inner_train_steps):
         # base model forward pass
         spt_logits_t = fmodel(spt_x_t)
         inner_loss = criterion(spt_logits_t, spt_y_t)
-        # inner-opt update
-        diffopt.step(inner_loss)
-    # print(f'>maml_new (after inner adapt): {fmodel.model.features.conv1.weight.norm(2)=}')
+        if not fo:
+            assert track_higher_grads == True
+            diffopt.step(inner_loss)
+        else:
+            assert copy_initial_weights == False
+            assert track_higher_grads == True  # I know it's confusing, see SO here: https://stackoverflow.com/questions/70961541/what-is-the-official-implementation-of-first-order-maml-using-the-higher-pytorch
+            diffopt.step(inner_loss, grad_callback=lambda grads: [g.detach() for g in grads])
     return fmodel
 
 
 def _get_maml_adapted_model_with_higher_one_task_with_context_manager(base_model: nn.Module,
                                                                       inner_opt: optim.Optimizer,
                                                                       spt_x_t: Tensor, spt_y_t: Tensor,
                                                                       training: bool,
@@ -253,15 +256,16 @@
         subsample_effective_num_data_method: Optional[str] = None,
         subsample_effective_num_data_param: Optional[int] = None,
         metric_as_sim_or_dist: str = 'dist',
         force_cpu: bool = False,
         training: bool = True,
         copy_initial_weights: bool = False,
         track_higher_grads: bool = False
-) -> list[OrderedDict[LayerIdentifier, float]]:
+) -> list[OrderedDict[str, float]]:
+    # ) -> list[OrderedDict[LayerIdentifier, float]]:
     """
     :param mdl:
     :param spt_x: not as a tuple due to having to move them to gpu potentially.
     :param spt_y:
     :param qry_x:
     :param qry_y:
     :param layer_names:
@@ -279,20 +283,24 @@
     :param metric_as_sim_or_dist:
     :param force_cpu:
     :param training:
     :param copy_initial_weights:
     :param track_higher_grads:
     :return:
     """
+    from anatome.helper import LayerIdentifier, dist_data_set_per_layer
     # - [B, M, C, H, W] -> [B, L]
     L: int = len(layer_names)
     B: int = spt_x.size(0)
-    dists_per_batch_per_layer: list[OrderedDict[LayerIdentifier, float]] = []
+    # dists_per_batch_per_layer: list[OrderedDict[LayerIdentifier, float]] = []
+    dists_per_batch_per_layer: list[OrderedDict[str, float]] = []
     for t in range(B):
         spt_x_t, spt_y_t, qry_x_t, qry_y_t = spt_x[t], spt_y[t], qry_x[t], qry_y[t]
+        # assert spt_x_t.size() == torch.Size([5*5, 84, 3, 3])
+        # assert qry_x_t.size() == torch.Size([5*15, 84, 3, 3])
         #
         adapted_mdl: FuncModel = get_maml_adapted_model_with_higher_one_task(mdl,
                                                                              inner_opt,
                                                                              spt_x_t, spt_y_t,
                                                                              training,
                                                                              copy_initial_weights,
                                                                              track_higher_grads,
@@ -346,22 +354,24 @@
         subsample_effective_num_data_method: Optional[str] = None,
         subsample_effective_num_data_param: Optional[int] = None,
         metric_as_sim_or_dist: str = 'dist',
         force_cpu: bool = False,
         training: bool = True,
         copy_initial_weights: bool = False,
         track_higher_grads: bool = False
-) -> list[OrderedDict[LayerIdentifier, float]]:
+) -> list[OrderedDict[str, float]]:
+    # ) -> list[OrderedDict[LayerIdentifier, float]]:
     """
     todo:
         - modify code so that it takes two meta-learners and returns the adapted model according to the meta-learner
         object. Note you can't make it functional since each meta-learner modifies the model with it's own code, so
         you eventually need to pattern the class to the function being used (or have the object carry that function
         intrinsically).
     """
+    from anatome.helper import LayerIdentifier, dist_data_set_per_layer
     # - [B, M, C, H, W] -> [B, L]
     L: int = len(layer_names)
     B: int = spt_x.size(0)
     dists_per_batch_per_layer: list[OrderedDict[LayerIdentifier, float]] = []
     for t in range(B):
         spt_x_t, spt_y_t, qry_x_t, qry_y_t = spt_x[t], spt_y[t], qry_x[t], qry_y[t]
         #
@@ -452,62 +462,87 @@
 def meta_learner_forward_adapt_batch_of_tasks(meta_learner, spt_x, spt_y, qry_x, qry_y,
                                               training: bool = True,  # always true to avoid .eval()
                                               call_backward: bool = False,  # not needed during testing/inference
                                               ) -> tuple[float, float, float, float]:
     """
     Returns the acc & loss on the meta-batch of query sets.
 
+    For important details see:
+        get_list_losses_accs_meta_learner_forward_adapt_batch_of_tasks(...)
+
+    """
+    meta_losses, meta_accs = get_lists_losses_accs_meta_learner_forward_adapt_batch_of_tasks(meta_learner,
+                                                                                             spt_x, spt_y, qry_x, qry_y,
+                                                                                             training, call_backward)
+    meta_loss, meta_loss_ci = mean_confidence_interval(meta_losses)
+    meta_acc, meta_acc_ci = mean_confidence_interval(meta_accs)
+    return meta_loss, meta_loss_ci, meta_acc, meta_acc_ci
+
+
+def get_lists_losses_accs_meta_learner_forward_adapt_batch_of_tasks(meta_learner,
+                                                                    spt_x, spt_y, qry_x, qry_y,
+                                                                    training: bool = True,
+                                                                    # always true to avoid .eval()
+                                                                    call_backward: bool = False,
+                                                                    # not needed during testing/inference
+                                                                    ) -> tuple[list[float], list[float]]:
+    """
+    Returns the accs & losses on the meta-batch of query sets.
+
     Note:
         - training true ensures .eval() is never called (due to BN, we always want batch stats)
         - call_backward collects gradients for outer_opt. Due to optimization of calling it here, we have the option
         to call it or not.
         - crucially, this code uses the code that does not use the context manager from higher. This is so to
         test that code that is later use to compare models using ultimate-anatome.
-
     """
     # - get inner opt
-    inner_opt = get_maml_inner_optimizer(meta_learner.base_model, meta_learner.lr_inner)
+    inner_opt = get_maml_inner_optimizer(meta_learner.base_model, meta_learner.inner_lr)
 
     # - adapt
     meta_learner.base_model.train() if training else meta_learner.base_model.eval()
     meta_batch_size = spt_x.size(0)
     meta_losses, meta_accs = [], []
+    # print(f'{meta_learner_forward_adapt_batch_of_tasks=}')
     for t in range(meta_batch_size):
         spt_x_t, spt_y_t, qry_x_t, qry_y_t = spt_x[t], spt_y[t], qry_x[t], qry_y[t]
         # - Inner Loop Adaptation
-        # st()
+        # assert meta_learner.args.copy_initial_weights == False
+        # assert meta_learner.args.track_higher_grads == False
         fmodel: FuncModel = get_maml_adapted_model_with_higher_one_task(meta_learner.base_model,
                                                                         inner_opt,
                                                                         spt_x_t, spt_y_t,
                                                                         training,
                                                                         copy_initial_weights=meta_learner.args.copy_initial_weights,
                                                                         track_higher_grads=meta_learner.args.track_higher_grads,
                                                                         fo=meta_learner.fo,
-                                                                        nb_inner_train_steps=meta_learner.args.nb_inner_train_steps,
+                                                                        nb_inner_train_steps=meta_learner.nb_inner_train_steps,
                                                                         criterion=meta_learner.args.criterion)
 
         # Evaluate on query set for current task
         qry_logits_t = fmodel(qry_x_t)
         qry_loss_t = meta_learner.args.criterion(qry_logits_t, qry_y_t)
 
         # Accumulate gradients wrt meta-params for each task: https://github.com/facebookresearch/higher/issues/104
         # note this is more mem efficient (removes intermediate data needed since backward has already been called)
         if call_backward:
             (qry_loss_t / meta_batch_size).backward()
+            # print(f'{t=}')
+            # print(f"{meta_learner.args.opt.param_groups[0]['params'][0].grad.norm()}")
+            # print(f"{meta_learner.args.opt.param_groups[0]['params'][0].grad is not None=}")
+            assert meta_learner.args.opt.param_groups[0]['params'][0].grad is not None
 
         # get accuracy
         if meta_learner.target_type == 'classification':
             from uutils.torch_uu import calc_accuracy_from_logits
             qry_acc_t = calc_accuracy_from_logits(y_logits=qry_logits_t, y=qry_y_t)
         else:
             from uutils.torch_uu import r2_score_from_torch
             qry_acc_t = r2_score_from_torch(qry_y_t, qry_logits_t).item()
 
         # collect losses & accs
         meta_losses.append(qry_loss_t.item())
-        # meta_losses.append(qry_loss_t)
         meta_accs.append(qry_acc_t)
-
     assert len(meta_losses) == meta_batch_size
-    meta_loss, meta_loss_ci = mean_confidence_interval(meta_losses)
-    meta_acc, meta_acc_ci = mean_confidence_interval(meta_accs)
-    return meta_loss, meta_loss_ci, meta_acc, meta_acc_ci
+    assert isinstance(meta_losses[0], float)
+    assert isinstance(meta_accs[0], float)
+    return meta_losses, meta_accs
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/maml_meta_learner.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/maml_meta_learner.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,259 +1,138 @@
 import logging
 from argparse import Namespace
-from typing import Callable
+from typing import Callable, Any
 
-import learn2learn
 import torch
 import torch.nn as nn
-from learn2learn.data import TaskDataset
 from torch import Tensor
-from torch.multiprocessing import Pool
-from torch.optim.optimizer import required
-from torch.optim import Optimizer as Optimizer
-
-import higher
-from higher.optim import _add
-from higher.optim import DifferentiableOptimizer
-from higher.optim import _GroupedGradsType
+# from torch.multiprocessing import Pool
+# from torch.optim.optimizer import required
+# from torch.optim import Optimizer as Optimizer
+#
+# import higher
+# from higher.optim import _add
+# from higher.optim import DifferentiableOptimizer
+# from higher.optim import _GroupedGradsType
 
 import uutils
 from uutils.torch_uu import functional_diff_norm, ned_torch, r2_score_from_torch, calc_accuracy_from_logits, \
     normalize_matrix_for_similarity, process_meta_batch
 from uutils.torch_uu import tensorify
 
 import numpy as np
 
+from uutils.torch_uu.meta_learners.maml_differentiable_optimizer import \
+    get_lists_losses_accs_meta_learner_forward_adapt_batch_of_tasks
 from uutils.torch_uu.metrics.confidence_intervals import torch_compute_confidence_interval
 
-Spt_x, Spt_y, Qry_x, Qry_y = torch.Tensor, torch.Tensor, torch.Tensor, torch.Tensor
-Task = tuple[Spt_x, Spt_y, Qry_x, Qry_y]
-Batch = list
-
-
-class EmptyOpt(Optimizer):  # This is just an example
-    def __init__(self, params, *args, **kwargs):
-        defaults = {'args': args, 'kwargs': kwargs}
-        super().__init__(params, defaults)
-
-
-class NonDiffMAML(Optimizer):  # copy pasted from torch.optim.SGD
-
-    def __init__(self, params, lr=required, momentum=0, dampening=0,
-                 weight_decay=0, nesterov=False):
-        if lr is not required and lr < 0.0:
-            raise ValueError("Invalid learning rate: {}".format(lr))
-        if momentum < 0.0:
-            raise ValueError("Invalid momentum value: {}".format(momentum))
-        if weight_decay < 0.0:
-            raise ValueError("Invalid weight_decay value: {}".format(weight_decay))
-
-        defaults = dict(lr=lr, momentum=momentum, dampening=dampening,
-                        weight_decay=weight_decay, nesterov=nesterov)
-
-        if nesterov and (momentum <= 0 or dampening != 0):
-            raise ValueError("Nesterov momentum requires a momentum and zero dampening")
-        super().__init__(params, defaults)
-
-
-class MAML(DifferentiableOptimizer):  # copy pasted from DifferentiableSGD but with the g.detach() line of code
-
-    def _update(self, grouped_grads: _GroupedGradsType, **kwargs) -> None:
-        zipped = zip(self.param_groups, grouped_grads)
-        for group_idx, (group, grads) in enumerate(zipped):
-            weight_decay = group['weight_decay']
-            momentum = group['momentum']
-            dampening = group['dampening']
-            nesterov = group['nesterov']
-
-            for p_idx, (p, g) in enumerate(zip(group['params'], grads)):
-                if g is None:
-                    continue
-
-                if weight_decay != 0:
-                    g = _add(g, weight_decay, p)
-                if momentum != 0:
-                    param_state = self.state[group_idx][p_idx]
-                    if 'momentum_buffer' not in param_state:
-                        buf = param_state['momentum_buffer'] = g
-                    else:
-                        buf = param_state['momentum_buffer']
-                        buf = _add(buf.mul(momentum), 1 - dampening, g)
-                        param_state['momentum_buffer'] = buf
-                    if nesterov:
-                        g = _add(g, momentum, buf)
-                    else:
-                        g = buf
-
-                if self.fo:  # first-order
-                    g = g.detach()  # dissallows flow of higher order grad while still letting params track gradients.
-                group['params'][p_idx] = _add(p, -group['lr'], g)
+from pdb import set_trace as st
 
-
-higher.register_optim(NonDiffMAML, MAML)
+from copy import deepcopy
 
 
 class MAMLMetaLearner(nn.Module):
     def __init__(
             self,
-            args,
-
-            base_model,
+            args: Namespace,
+            model: nn.Module,
 
-            lr_inner=1e-1,  # careful with setting this to small or doing to few inner adaptation steps
-            fo=False,
-            inner_debug=False,
-            target_type='classification'
+            inner_debug: bool = False,
+            target_type: str = 'classification'
     ):
         super().__init__()
         self.args = args  # args for experiment
-        self.base_model = base_model
-
-        self.lr_inner = lr_inner
-        self.fo = fo
-        self.inner_debug = inner_debug
+        self.model = model
+        self.nb_inner_train_steps = deepcopy(self.args.nb_inner_train_steps)
+        self.inner_lr = deepcopy(self.args.inner_lr)
+        if not hasattr(args, 'fo'):
+            self.args.fo = True
+        self.fo = deepcopy(self.args.fo)
 
         self.target_type = target_type
 
-    def forward(self, batch, training: bool = True, call_backward: bool = False):
-        """
-        Does L(A(theta,S), Q) = sum^N_{t=1} L(A(theta,S_t),Q_t) where A(theta,S) is the inner-adaptation loop.
-        It also accumulates the gradient (for memory efficiency) for the outer-optimizer to later use
-
-        Decision for BN/eval:
-        - during training always use .train().
-        During eval use the meta-train stats so do .eval() (and using .train() is always wrong since it cheats).
-        Having track_running_stats=False seems overly complicated and nobody seems to use it...so why use it?
-
-        ref for BN/eval:
-            - https://stats.stackexchange.com/questions/544048/what-does-the-batch-norm-layer-for-maml-model-agnostic-meta-learning-do-for-du
-            - https://github.com/tristandeleu/pytorch-maml/issues/19
-        """
-        spt_x, spt_y, qry_x, qry_y = process_meta_batch(self.args, batch)
-        from uutils.torch_uu.meta_learners.maml_differentiable_optimizer import \
-            meta_learner_forward_adapt_batch_of_tasks
-        meta_loss, meta_loss_ci, meta_acc, meta_acc_ci = meta_learner_forward_adapt_batch_of_tasks(self, spt_x, spt_y,
-                                                                                                   qry_x, qry_y,
-                                                                                                   training,
-                                                                                                   call_backward)
-        return meta_loss, meta_loss_ci, meta_acc, meta_acc_ci
-
-    def eval_forward(self, batch, training: bool = True, call_backward: bool = False):
-        meta_loss, meta_loss_ci, meta_acc, meta_acc_ci = self.forward(batch, training, call_backward)
-        return meta_loss, meta_loss_ci, meta_acc, meta_acc_ci
-
-    def eval(self):
-        """
-        Note: decision is to do .train() for all meta-train and .eval() for meta-eval.
-        ref: https://stats.stackexchange.com/questions/544048/what-does-the-batch-norm-layer-for-maml-model-agnostic-meta-learning-do-for-du
-        """
-        logging.warning('Calling MAML.eval(). You sure you want to do that?')
-        self.base_model.eval()
-
-    def parameters(self):
-        return self.base_model.parameters()
-
-    def regression(self):
-        self.target_type = 'regression'
-        self.args.target_type = 'regression'
-
-    def classification(self):
-        self.target_type = 'classification'
-        self.args.target_type = 'classification'
-
-    def cuda(self):
-        self.base_model.cuda()
-
-
-class MAMLMetaLearner(nn.Module):
-    def __init__(
-            self,
-            args,
-            base_model,
-
-            inner_debug=False,
-            target_type='classification'
-    ):
-        super().__init__()
-        self.args = args  # args for experiment
-        self.base_model = base_model
-        # assert base_model is args.model
-
         self.inner_debug = inner_debug
-        self.target_type = target_type
 
+    # for backwards compatibility
+    # field as function base_model return model
     @property
-    def lr_inner(self) -> float:
-        return self.args.inner_lr
+    def base_model(self):
+        return self.model
 
-    @lr_inner.setter
-    def lr_inner(self, new_val: float):
-        self.args.inner_lr = new_val
-
-    @property
-    def fo(self):
-        return self.args.fo
-
-    # @property
-    # def mdl(self) -> torch.nn.Module:
-    #     return uutils.torch.get_model(self.mdl_)
+    # set field as function base_model
+    @base_model.setter
+    def base_model(self, model: nn.Module):
+        self.model = model
 
     def forward(self, batch, training: bool = True, call_backward: bool = False):
         """
         Does L(A(theta,S), Q) = sum^N_{t=1} L(A(theta,S_t),Q_t) where A(theta,S) is the inner-adaptation loop.
         It also accumulates the gradient (for memory efficiency) for the outer-optimizer to later use
 
         Decision for BN/eval:
-        - during training always use .train().
-
-        ref for BN/eval:
-            - https://stats.stackexchange.com/questions/544048/what-does-the-batch-norm-layer-for-maml-model-agnostic-meta-learning-do-for-du
+            - during meta-training always use .train(), see: https://stats.stackexchange.com/a/551153/28986
         """
         spt_x, spt_y, qry_x, qry_y = process_meta_batch(self.args, batch)
         from uutils.torch_uu.meta_learners.maml_differentiable_optimizer import \
             meta_learner_forward_adapt_batch_of_tasks
         meta_loss, meta_loss_ci, meta_acc, meta_acc_ci = meta_learner_forward_adapt_batch_of_tasks(self, spt_x, spt_y,
                                                                                                    qry_x, qry_y,
                                                                                                    training,
                                                                                                    call_backward)
-        return meta_loss, meta_loss_ci, meta_acc, meta_acc_ci
+        return meta_loss, meta_acc
 
     def eval_forward(self, batch, training: bool = True, call_backward: bool = False):
-        meta_loss, meta_loss_ci, meta_acc, meta_acc_ci = self.forward(batch, training, call_backward)
-        return meta_loss, meta_loss_ci, meta_acc, meta_acc_ci
+        """
+        Does a forward pass ala l2l. It's the same as forward just so that all Agents have the same interface.
+        This one looks redundant and it is, but it's here for consistency with the SL agents.
+        The eval forward is different in SL agents.
+        """
+        loss, loss_ci, acc, acc_ci = eval_forward(self, batch, training=training, call_backward=call_backward)
+        return loss, loss_ci, acc, acc_ci
+
+    def get_lists_accs_losses(self, batch, training: bool = True, call_backward: bool = False):
+        spt_x, spt_y, qry_x, qry_y = process_meta_batch(self.args, batch)
+        # note bellow code is already in forward, but we need to call it here to get the lists explicitly (no redundant code! ;) )
+        meta_losses, meta_accs = get_lists_losses_accs_meta_learner_forward_adapt_batch_of_tasks(self, spt_x, spt_y,
+                                                                                                 qry_x, qry_y,
+                                                                                                 training,
+                                                                                                 call_backward)
+        return meta_losses, meta_accs
 
     def eval(self):
         """
         Note: decision is to do .train() for all meta-train
         ref: https://stats.stackexchange.com/questions/544048/what-does-the-batch-norm-layer-for-maml-model-agnostic-meta-learning-do-for-du
         """
         logging.warning('Calling MAML.eval(). You sure you want to do that?')
-        raise ValueError(f'Why are you calling eval during meta-learning? Read: https://stats.stackexchange.com/questions/544048/what-does-the-batch-norm-layer-for-maml-model-agnostic-meta-learning-do-for-du')
-        self.base_model.eval()
+        raise ValueError(
+            f'Why are you calling eval during meta-learning? Read: https://stats.stackexchange.com/questions/544048/what-does-the-batch-norm-layer-for-maml-model-agnostic-meta-learning-do-for-du')
+        self.model.eval()
 
     def parameters(self):
-        return self.base_model.parameters()
+        return self.model.parameters()
 
     def regression(self):
         self.target_type = 'regression'
         self.args.target_type = 'regression'
 
     def classification(self):
         self.target_type = 'classification'
         self.args.target_type = 'classification'
 
     def cuda(self):
-        self.base_model.cuda()
+        self.model.cuda()
 
 
 # - l2l
 
 def fast_adapt(args: Namespace,
                task_data, learner, loss, adaptation_steps, shots, ways, device) -> tuple[Tensor, Tensor]:
     """"""
+    import learn2learn
     # [n*(k+k_eval), C, H, W] (or [n(k+k_eval), D])
     data, labels = task_data
     data, labels = data.to(device), labels.to(device)
 
     # Separate data into adaptation/evalutation sets
     # [n*(k+k_eval), C, H, W] -> [n*k, C, H, W] and [n*k_eval, C, H, W]
     (support_data, support_labels), (query_data, query_labels) = learn2learn.data.partition_task(
@@ -266,15 +145,17 @@
     # checks [n*k] since these are the labels
     assert support_labels.size() == torch.Size([shots * ways])
 
     # Adapt the model
     for step in range(adaptation_steps):
         # - note the loss is usually in the final layer for my models
         adaptation_error = loss(learner(support_data), support_labels)
+        # st()
         learner.adapt(adaptation_error)
+        # st()
 
     # Evaluate the adapted model
     predictions: Tensor = learner(query_data)
     evaluation_error: Tensor = loss(predictions, query_labels)
 
     # get accuracy
     if args.agent.target_type == 'classification':
@@ -282,145 +163,290 @@
     else:
         from uutils.torch_uu import r2_score_from_torch
         evaluation_accuracy = r2_score_from_torch(query_labels, predictions)
         raise NotImplementedError
     return evaluation_error, evaluation_accuracy
 
 
-def forward(meta_learner,
-            args: Namespace,
-            task_dataset: TaskDataset,  # args.tasksets.train, args.tasksets.validation or args.tasksets.test
-            meta_batch_size: int,  # suggested max(batch_size or eval // args.world_size, 2)
-
-            training: bool = True,  # always true to avoid .eval()
-            call_backward: bool = False,  # not needed during testing/inference
-            ):
+def get_lists_accs_losses_l2l(meta_learner,
+                              args: Namespace,
+                              task_dataset,  # from learn2learn.data import TaskDataset,
+                              # args.tasksets.train, args.tasksets.validation or args.tasksets.test
+                              meta_batch_size: int,  # suggested max(batch_size or eval // args.world_size, 2)
+
+                              training: bool = True,  # always true to avoid .eval()
+                              call_backward: bool = False,  # not needed during testing/inference
+                              ):
     """
-    Returns the acc & loss on the meta-batch from the task in task_dataset.
+    Returns the (meta) accs & losses on the meta-batch/task_dataset.
 
     Note:
-    - training true ensures .eval() is never called (due to BN, we always want batch stats)
-    - call_backward collects gradients for outer_opt. Due to optimization of calling it here, we have the option
-    to call it or not.
+        - training true ensures .eval() is never called (due to BN, we always want batch stats)
+        - call_backward collects gradients for outer_opt. Due to optimization of calling it here, we have the option to call it or not.
     """
     assert args is meta_learner.args
-    assert args.meta_learner is meta_learner
-    assert args.agent is meta_learner
+    # -
+    from learn2learn.data import TaskDataset
+    task_dataset: TaskDataset = task_dataset  # args.tasksets.train, args.tasksets.validation or args.tasksets.test
 
     # - adapt
-    meta_learner.base_model.train() if training else meta_learner.base_model.eval()
+    meta_learner.model.train() if training else meta_learner.model.eval()
     meta_losses, meta_accs = [], []
     for task in range(meta_batch_size):
+        # print(f'{task=}')
         # - Sample all data data for spt & qry sets for current task: thus size [n*(k+k_eval), C, H, W] (or [n(k+k_eval), D])
         task_data: list = task_dataset.sample()  # data, labels
 
         # -- Inner Loop Adaptation
         learner = meta_learner.maml.clone()
         loss, acc = fast_adapt(
             args=args,
             task_data=task_data,
             learner=learner,
             loss=args.loss,
-            adaptation_steps=args.nb_inner_train_steps,
+            adaptation_steps=meta_learner.nb_inner_train_steps,
             shots=args.k_shots,
             ways=args.n_classes,
             device=args.device,
         )
         if call_backward:
             loss.backward()
         # collect losses & accs
-        meta_losses.append(loss)
-        meta_accs.append(acc)
+        meta_losses.append(loss.item())
+        meta_accs.append(acc.item())
     assert len(meta_losses) == meta_batch_size
     assert len(meta_accs) == meta_batch_size
-    meta_loss, meta_loss_ci = torch_compute_confidence_interval(tensorify(meta_losses))
-    meta_acc, meta_acc_ci = torch_compute_confidence_interval(tensorify(meta_accs))
-    return meta_loss, meta_loss_ci, meta_acc, meta_acc_ci
+    return meta_losses, meta_accs
 
 
 class MAMLMetaLearnerL2L(nn.Module):
     def __init__(
             self,
-            args,
-            base_model,
+            args: Namespace,
+            model: nn.Module,
 
-            target_type='classification',
-            min_batch_size=1,
+            target_type: str = 'classification',
     ):
+        import learn2learn
         super().__init__()
         self.args = args  # args for experiment
-        self.base_model = base_model
         assert args is self.args
-        assert base_model is args.model
-        self.maml = learn2learn.algorithms.MAML(args.model, lr=args.inner_lr, first_order=args.first_order)
+        self.model = model
+        assert model is args.model
+        self.inner_lr = deepcopy(args.inner_lr)
+        self.nb_inner_train_steps = deepcopy(args.nb_inner_train_steps)
+        self.first_order = deepcopy(args.first_order)
+        # learn2learn: Maybe try with allow_nograd=True and/or allow_unused=True ?
+        allow_unused = args.allow_unused if hasattr(args, 'allow_unused') else None
+        self.maml = learn2learn.algorithms.MAML(self.model,
+                                                lr=self.inner_lr,
+                                                first_order=self.first_order,
+                                                allow_unused=allow_unused
+                                                )
         # maml = l2l.algorithms.MAML(model, lr=fast_lr, first_order=False)
         # opt = torch.optim.Adam(maml.parameters(), meta_lr)
         # opt = cherry.optim.Distributed(maml.parameters(), opt=opt, sync=1)
 
         self.target_type = target_type
-        self.min_batch_size = min_batch_size
 
-    def forward(self, task_dataset: TaskDataset, training: bool = True, call_backward: bool = False):
+    # for backwards compatibility
+    # field as function base_model return model
+    @property
+    def base_model(self):
+        return self.model
+
+    # set field as function base_model
+    @base_model.setter
+    def base_model(self, model: nn.Module):
+        self.model = model
+
+    def forward(self, task_dataset, training: bool = True, call_backward: bool = False):
         """
         Does a forward pass ala l2l.
 
         Decision for BN/eval:
-            - during training always use .train().
-            During eval use the meta-train stats so do .eval() (and using .train() is always wrong since it cheats).
-            Having track_running_stats=False seems overly complicated and nobody seems to use it...so why use it?
-
-        ref for BN/eval:
-            - https://stats.stackexchange.com/questions/544048/what-does-the-batch-norm-layer-for-maml-model-agnostic-meta-learning-do-for-du
-            - https://github.com/tristandeleu/pytorch-maml/issues/19
-        """
-        meta_batch_size: int = max(self.args.batch_size // self.args.world_size, 1)
-        meta_loss, meta_loss_ci, meta_acc, meta_acc_ci = forward(meta_learner=self,
-                                                                 args=self.args,
-                                                                 task_dataset=task_dataset,  # eg args.tasksets.train
-                                                                 training=training,  # always true to avoid .eval()
-                                                                 meta_batch_size=meta_batch_size,
-
-                                                                 call_backward=call_backward,  # False for val/test
-                                                                 )
-        return meta_loss, meta_loss_ci, meta_acc, meta_acc_ci
-
-    def eval_forward(self, task_dataset: TaskDataset, training: bool = True, call_backward: bool = False):
-        meta_batch_size: int = max(self.args.batch_size // self.args.world_size, 1)
-        meta_loss, meta_loss_ci, meta_acc, meta_acc_ci = forward(meta_learner=self,
-                                                                 args=self.args,
-                                                                 task_dataset=task_dataset,  # eg args.tasksets.train
-                                                                 training=training,  # always true to avoid .eval()
-                                                                 meta_batch_size=meta_batch_size,
-
-                                                                 call_backward=call_backward,  # False for val/test
-                                                                 )
-        return meta_loss, meta_loss_ci, meta_acc, meta_acc_ci
+            - during meta-training always use .train(), see: https://stats.stackexchange.com/a/551153/28986
+        """
+        # - type task_dataset (since we don't want to globally import learn2learn here if you're not using it but still needs stuff in this file)
+        from learn2learn.data import TaskDataset
+        task_dataset: TaskDataset = task_dataset  # args.tasksets.train, args.tasksets.validation or args.tasksets.test
+        # assert self.args.batch_size_eval == task_dataset.num_tasks, f"Err: {self.args.batch_size_eva} != {task_dataset.num_tasks}"
+        # assert self.args.batch_size == task_dataset.num_tasks, f"Err: {self.args.batch_size} != {task_dataset.num_tasks}"
+        # meta_batch_size: int = max(self.args.batch_size // self.args.world_size, 1)
+        # meta_batch_size: int = max(task_dataset.num_tasks // self.args.world_size, 1)
+        # meta_losses, meta_accs = get_lists_accs_losses_l2l(self, self.args, task_dataset, meta_batch_size, training,
+        #                                                    call_backward)
+        meta_losses, meta_accs = self.get_lists_accs_losses(task_dataset, training, call_backward)
+        loss, loss_ci = torch_compute_confidence_interval(tensorify(meta_losses))
+        acc, acc_ci = torch_compute_confidence_interval(tensorify(meta_accs))
+        return loss, acc
+
+    def eval_forward(self, task_dataset, training: bool = True, call_backward: bool = False):
+        """
+        Does a forward pass ala l2l. It's the same as forward just so that all Agents have the same interface.
+        This one looks redundant and it is, but it's here for consistency with the SL agents, since
+        the eval forward is different in SL agents (e.g. torch.no_grad is used in SL agent but here we don't).
+        """
+        # - type task_dataset (since we don't want to globally import learn2learn here if you're not using it but still needs stuff in this file)
+        from learn2learn.data import TaskDataset
+        task_dataset: TaskDataset = task_dataset  # args.tasksets.train, args.tasksets.validation or args.tasksets.test
+        # assert self.args.batch_size_eval == task_dataset.num_tasks, f"Err: {self.args.batch_size_eva} != {task_dataset.num_tasks}"
+        # assert self.args.batch_size == task_dataset.num_tasks, f"Err: {self.args.batch_size} != {task_dataset.num_tasks}"
+        # meta_batch_size: int = max(self.args.batch_size // self.args.world_size, 1)
+        # meta_batch_size: int = max(task_dataset.num_tasks // self.args.world_size, 1)
+        # meta_losses, meta_accs = get_lists_accs_losses_l2l(self, self.args, task_dataset, meta_batch_size, training,
+        #                                                    call_backward)
+        loss, loss_ci, acc, acc_ci = eval_forward(self, task_dataset, training=training, call_backward=call_backward)
+        return loss, loss_ci, acc, acc_ci
+
+    def get_lists_accs_losses(self, task_dataset, training: bool = True, call_backward: bool = False):
+        """
+        Returns the acc & loss on the meta-batch from the task in task_dataset.
+        """
+        # -
+        from learn2learn.data import TaskDataset
+        task_dataset: TaskDataset = task_dataset  # args.tasksets.train, args.tasksets.validation or args.tasksets.test
+        # -
+        # meta_batch_size: int = max(self.args.batch_size // self.args.world_size, 1)
+        meta_batch_size: int = max(task_dataset.num_tasks // self.args.world_size, 1)
+        meta_batch_size: int = max(self.args.batch_size_eval // self.args.world_size, 1)
+        # note bellow code is already in forward, but we need to call it here to get the lists explicitly (no redundant code! ;) )
+        meta_losses, meta_accs = get_lists_accs_losses_l2l(meta_learner=self,
+                                                           args=self.args,
+                                                           task_dataset=task_dataset,  # eg args.tasksets.train
+                                                           training=training,  # always true to avoid .eval()
+                                                           meta_batch_size=meta_batch_size,
+                                                           call_backward=call_backward,  # False for val/test
+                                                           )
+        return meta_losses, meta_accs
 
     def eval(self):
         """
         Note: decision is to do .train() for all meta-train and .eval() for meta-eval.
         ref: https://stats.stackexchange.com/questions/544048/what-does-the-batch-norm-layer-for-maml-model-agnostic-meta-learning-do-for-du
         """
         logging.warning('Calling MAML.eval(). You sure you want to do that?')
-        self.base_model.eval()
+        self.model.eval()
 
     def parameters(self):
-        # return self.base_model.parameters()
-        # todo would be nice to check if self.maml.parameters() and self.base_model.parameters() are the same
+        # return self.model.parameters()
+        # todo would be nice to check if self.maml.parameters() and self.model.parameters() are the same
         return self.maml.parameters()
 
     def regression(self):
         self.target_type = 'regression'
         self.args.target_type = 'regression'
 
     def classification(self):
         self.target_type = 'classification'
         self.args.target_type = 'classification'
 
     def cuda(self):
-        self.base_model.cuda()
+        self.model.cuda()
+
+
+# -- eval code
+
+def eval_forward(model: nn.Module, data: Any, training: bool = False, call_backward: bool = False):
+    """
+    Note:
+        - training = True makes sense for meta-learning (or if you want norms to use batch statistics, but it might
+        change your running statistics).
+    """
+    from uutils.torch_uu.metrics.confidence_intervals import mean_confidence_interval
+    assert call_backward == False, 'call_backward should be False for eval_forward'
+    losses, accs = model.get_lists_accs_losses(data, training, call_backward=call_backward)
+    loss, loss_ci = mean_confidence_interval(losses)
+    acc, acc_ci = mean_confidence_interval(accs)
+    return loss, loss_ci, acc, acc_ci
+
+
+# --
+
+def get_minimum_args_to_run_maml_torchmeta_on_mi_5cnn() -> Namespace:
+    from uutils.torch_uu.models.learner_from_opt_as_few_shot_paper import get_defaul_args_for_5cnn
+    from pathlib import Path
+    from uutils.argparse_uu.meta_learning import parse_args_meta_learning
+    from uutils.argparse_uu.common import setup_args_for_experiment
+    args: Namespace = parse_args_meta_learning()
+    args = get_defaul_args_for_5cnn(args)
+    args.data_option = 'torchmeta_miniimagenet'
+    args.data_path = Path('~/data/torchmeta_data/').expanduser()
+    args.inner_lr = 0.1
+    args.nb_inner_train_steps = 5
+    args.copy_initial_weights = False  # DONT PUT TRUE. details: set to True only if you do NOT want to train base model's initialization https://stackoverflow.com/questions/60311183/what-does-the-copy-initial-weights-documentation-mean-in-the-higher-library-for
+    # args.track_higher_grads = True  # not FO maml
+    args.track_higher_grads = False  # fo? https://github.com/facebookresearch/higher/issues/63
+    args.training_mode = 'iterations'
+    args.num_its = 2
+    args: Namespace = setup_args_for_experiment(args)
+    return args
 
 
 # - tests
 
+def check_training_fo_maml():
+    print('---- checking fo MAML torchmeta higher')
+    track_higher_grads = False
+    print(f'{track_higher_grads=}')
+    check_training_meta_train_fixed_iterations(track_higher_grads)
+    print('---- success! Of fo MAML torchmeta higher')
+
+
+def check_training_meta_train_fixed_iterations(track_higher_grads: bool = True):
+    from uutils.torch_uu.models.learner_from_opt_as_few_shot_paper import get_default_learner_and_hps_dict
+    from uutils.torch_uu.training.meta_training import meta_train_fixed_iterations
+    from uutils.torch_uu.dataloaders.meta_learning.helpers import get_meta_learning_dataloaders
+    from uutils.torch_uu.optim_uu.adam_uu import get_opt_adam_default
+    from uutils.torch_uu.optim_uu.adam_uu import get_cosine_scheduler_adam_rfs_cifarfs
+
+    args = get_minimum_args_to_run_maml_torchmeta_on_mi_5cnn()
+    args.track_higher_grads = track_higher_grads
+    args.model, args.model_hps = get_default_learner_and_hps_dict()
+    args.agent = MAMLMetaLearner(args, args.model)
+    args.meta_learner = args.agent
+    opt_hps = {}
+    args.opt, args.opt_hps = get_opt_adam_default(args.model, **opt_hps)
+    scheduler_hps = {}
+    args.scheduler, args.scheduler_hps = get_cosine_scheduler_adam_rfs_cifarfs(args.opt, **scheduler_hps)
+    args.dataloaders: dict = get_meta_learning_dataloaders(args)
+    print(f'{args.dataloaders=}')
+    assert args.data_option == 'torchmeta_miniimagenet', f'Err: {args.data_option=}'
+    print()
+    meta_train_fixed_iterations(args, args.agent, args.dataloaders, args.opt, args.scheduler)
+
+
+def check_torchmeta_4_tuple_works_with_meta_learner_agent():
+    from uutils.torch_uu.models.learner_from_opt_as_few_shot_paper import get_defaul_args_for_5cnn
+    from uutils.torch_uu.models.learner_from_opt_as_few_shot_paper import get_learner_from_args
+    from uutils.torch_uu.dataloaders.meta_learning.helpers import get_meta_learning_dataloaders
+    from pathlib import Path
+    from uutils.argparse_uu.meta_learning import parse_args_meta_learning
+    from uutils.argparse_uu.common import setup_args_for_experiment
+
+    args: Namespace = parse_args_meta_learning()
+    args = get_defaul_args_for_5cnn(args)
+    args.data_option = 'torchmeta_miniimagenet'
+    args.data_path = Path('~/data/torchmeta_data/').expanduser()
+    args.inner_lr = 0.1
+    args.nb_inner_train_steps = 5
+    args.copy_initial_weights = False  # DONT PUT TRUE. details: set to True only if you do NOT want to train base model's initialization https://stackoverflow.com/questions/60311183/what-does-the-copy-initial-weights-documentation-mean-in-the-higher-library-for
+    args.track_higher_grads = False  # fo? https://github.com/facebookresearch/higher/issues/63
+    args: Namespace = setup_args_for_experiment(args)
+    model = get_learner_from_args(args)  # random 5cnn
+    agent = MAMLMetaLearner(args, model)
+
+    args.dataloaders: dict = get_meta_learning_dataloaders(args)
+    print(f'{args.dataloaders=}')
+    assert args.data_option == 'torchmeta_miniimagenet', f'Err: {args.data_option=}'
+    for batch in args.dataloaders['train']:
+        losses = agent(batch)
+        print(f'{losses=}')
+        break
+
+
 if __name__ == "__main__":
+    # check_torchmeta_4_tuple_works_with_meta_learner_agent()
+    # check_training_loop_fit_one_batch()
+    # check_training_meta_train_fixed_iterations()
+    check_training_fo_maml()
     print('Done, all Tests Passed! \a')
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/meta_lstm_meta_learner.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/meta_lstm_meta_learner.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/pretrain_convergence.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/meta_learners/pretrain_convergence.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from argparse import Namespace
+
 import torch
 import torch.nn as nn
 
 import numpy as np
 
 from sklearn import metrics
 from sklearn.linear_model import LogisticRegression
@@ -20,68 +22,97 @@
 
 # https://github.com/WangYueFt/rfs/blob/master/eval/meta_eval.py
 from uutils.torch_uu import r2_score_from_torch, process_meta_batch, tensorify, normalize
 from uutils.torch_uu.metrics.confidence_intervals import torch_compute_confidence_interval, \
     mean_confidence_interval
 from uutils.torch_uu.models import getattr_model
 
-# import torch
-# from sklearn import metrics
-# from sklearn.svm import SVC, LinearSVC
-# from sklearn.linear_model import LogisticRegression
-# from sklearn.neighbors import KNeighborsClassifier
-# from sklearn.ensemble import RandomForestClassifier
-#
-# from sklearn.pipeline import make_pipeline
-# from sklearn.preprocessing import StandardScaler
-
 from pdb import set_trace as st, set_trace
 
 
 class FitFinalLayer(nn.Module):
 
     def __init__(self,
-                 args,
-                 base_model,
-                 target_type='classification',
-                 classifier='LR'):
+                 args: Namespace,
+                 model: nn.Module,
+                 target_type: str = 'classification',
+                 classifier: str = 'LR',
+                 ):
         super().__init__()
         self.args = args
-        self.base_model = base_model
+        self.model = model
         self.target_type = target_type
         self.classifier = classifier
 
+    @property
+    def base_model(self):
+        return self.model
+
+    # set field as function base_model
+    @base_model.setter
+    def base_model(self, model: nn.Module):
+        self.model = model
+
     def forward(self, batch,
                 training: bool = True,
                 is_norm: bool = False,
                 ):
         """
         training true since we want BN to use batch statistics (and not cheat, etc)
         """
+        # -- Get average meta-loss/acc of the meta-learner i.e. 1/B sum_b Loss(qrt_i, f) = E_B E_K[loss(qrt[b,k], f)]
+        # average loss on task of size K-eval over a meta-batch of size B (so B tasks)
+        meta_losses, meta_accs = self.get_lists_accs_losses(batch, training, is_norm)
+
+        # -- return loss, acc with CIs
+        meta_loss, meta_loss_ci = mean_confidence_interval(meta_losses)
+        meta_acc, meta_acc_ci = mean_confidence_interval(meta_accs)
+        return meta_loss, meta_loss_ci, meta_acc, meta_acc_ci
+
+    def eval_forward(self, batch,
+                     training: bool = True,
+                     is_norm: bool = False,
+                     ):
+        """
+        note:
+            - Does a forward pass. It's the same as forward just so that all Agents have the same interface.
+            This one looks redundant and it is, but it's here for consistency with the SL agents.
+            The eval forward is different in SL agents.
+            - training true since we want BN to use batch statistics (and not cheat, etc)
+        """
+        meta_loss, meta_loss_std, meta_acc, meta_acc_std = self.forward(batch, training, is_norm)
+        return meta_loss, meta_loss_std, meta_acc, meta_acc_std
+
+    def get_lists_accs_losses(self, batch,
+                              training: bool = True,
+                              is_norm: bool = False,
+                              ):
+        """
+        Get the list of accuracies and losses for each task in the meta-batch
+        """
         spt_x, spt_y, qry_x, qry_y = process_meta_batch(self.args, batch)
         # Accumulate gradient of meta-loss wrt fmodel.param(t=0)
         meta_batch_size = spt_x.size(0)
         meta_losses, meta_accs = [], []
         for t in range(meta_batch_size):
             spt_x_t, spt_y_t, qry_x_t, qry_y_t = spt_x[t], spt_y[t], qry_x[t], qry_y[t]
 
-            self.base_model.train() if training else self.base_model.eval()
-            spt_embeddings_t = self.get_embedding(spt_x_t, self.base_model).detach()
-            qry_embeddings_t = self.get_embedding(qry_x_t, self.base_model).detach()
+            self.model.train() if training else self.model.eval()
+            spt_embeddings_t = self.get_embedding(spt_x_t, self.model).detach()
+            qry_embeddings_t = self.get_embedding(qry_x_t, self.model).detach()
 
             if is_norm:
                 spt_embeddings_t = normalize(spt_embeddings_t)
                 qry_embeddings_t = normalize(qry_embeddings_t)
 
             if self.target_type == 'classification':
                 spt_embeddings_t = spt_embeddings_t.view(spt_embeddings_t.size(0), -1).cpu().numpy()
                 qry_embeddings_t = qry_embeddings_t.view(qry_embeddings_t.size(0), -1).cpu().numpy()
                 spt_y_t = spt_y_t.view(-1).cpu().numpy()
                 qry_y_t = qry_y_t.view(-1).cpu().numpy()
-                # set_trace()
                 # print(f'{spt_embeddings_t.shape=}')
 
                 # Inner-Adapt final layer with spt set
                 mdl = LogisticRegression(random_state=0,
                                          solver='lbfgs',
                                          max_iter=1000,
                                          multi_class='multinomial')
@@ -130,61 +161,48 @@
                 # Predict using adapted final layer with qrt set
                 query_y_pred_t = torch.Tensor(mdl.predict(qry_embeddings_t))
                 qry_loss_t = self.args.criterion(query_y_pred_t, qry_y_t)
                 qry_acc_t = r2_score_from_torch(qry_y_t, query_y_pred_t)
             else:
                 raise ValueError(f'Not implement: {self.target_type}')
 
-            # collect losses & accs for logging/debugging
+            # collect losses & accs
             meta_losses.append(qry_loss_t.item())
-            # meta_losses.append(qry_loss_t)
             meta_accs.append(qry_acc_t)
+        assert len(meta_losses) == meta_batch_size, f'Error: {len(meta_losses)=} {meta_batch_size=}'
+        return meta_losses, meta_accs
 
-        # Get average meta-loss/acc of the meta-learner i.e. 1/B sum_b Loss(qrt_i, f) = E_B E_K[loss(qrt[b,k], f)]
-        # average loss on task of size K-eval over a meta-batch of size B (so B tasks)
-        assert (len(meta_losses) == meta_batch_size)
-        meta_loss, meta_loss_ci = mean_confidence_interval(meta_losses)
-        meta_acc, meta_acc_ci = mean_confidence_interval(meta_accs)
-        return meta_loss, meta_loss_ci, meta_acc, meta_acc_ci
-
-    def eval_forward(self, batch, training: bool = True):
-        """
-        training true since we want BN to use batch statistics (and not cheat, etc)
-        """
-        meta_loss, meta_loss_std, meta_acc, meta_acc_std = self.forward(batch, training)
-        return meta_loss, meta_loss_std, meta_acc, meta_acc_std
-
-    def get_embedding(self, x: Tensor, base_model: nn.Module) -> Tensor:
-        return get_embedding(x=x, base_model=base_model)
+    def get_embedding(self, x: Tensor, model: nn.Module) -> Tensor:
+        return get_embedding(x=x, model=model)
 
     def regression(self):
         self.target_type = 'regression'
 
     def classification(self):
         self.target_type = 'classification'
 
     def train(self):
-        self.base_model.train()
+        self.model.train()
 
     def eval(self):
-        self.base_model.eval()
+        self.model.eval()
 
 
-def get_adapted_according_to_ffl(base_model, spt_x_t, spt_y_t, qry_x_t, qry_y_t,
+def get_adapted_according_to_ffl(model, spt_x_t, spt_y_t, qry_x_t, qry_y_t,
                                  layer_to_replace: str,
                                  training: bool = True,
                                  target_type: str = 'classification',
                                  classifier: str = 'LR', ) -> nn.Module:
     """
     Return the adapted model such that the final layer has the LR fined tuned model.
     """
     # spt_x_t, spt_y_t, qry_x_t, qry_y_t = spt_x[t], spt_y[t], qry_x[t], qry_y[t]
-    base_model.train() if training else base_model.eval()
-    spt_embeddings_t = get_embedding(spt_x_t, base_model).detach()
-    qry_embeddings_t = get_embedding(qry_x_t, base_model).detach()
+    model.train() if training else model.eval()
+    spt_embeddings_t = get_embedding(spt_x_t, model).detach()
+    qry_embeddings_t = get_embedding(qry_x_t, model).detach()
     if target_type == 'classification':
         spt_embeddings_t = spt_embeddings_t.view(spt_embeddings_t.size(0), -1).cpu().numpy()
         qry_embeddings_t = qry_embeddings_t.view(qry_embeddings_t.size(0), -1).cpu().numpy()
         spt_y_t = spt_y_t.view(-1).cpu().numpy()
         qry_y_t = qry_y_t.view(-1).cpu().numpy()
 
         # Inner-Adapt final layer with spt set
@@ -199,17 +217,17 @@
             clf = LogisticRegression(random_state=0, solver='lbfgs', max_iter=1000,
                                      multi_class='multinomial')
             clf.fit(spt_embeddings_t, spt_y_t)
             # query_y_pred_t = clf.predict(qry_embeddings_t)
             query_y_probs_t = clf.predict_proba(qry_embeddings_t)
 
             # - get layer_to_replace e.g. model.cls
-            module: nn.Module = getattr_model(base_model, layer_to_replace)
+            module: nn.Module = getattr_model(model, layer_to_replace)
             assert module is not None, f'Final layer module is None instead of a pytorch module see: {module=}'
-            # assert module is base_model.model.cls
+            # assert module is model.model.cls
 
             # - replace weights into model
             # coef_ndarray of shape (1, n_features) or (n_classes, n_features)
             new_weights: np.ndarray = clf.coef_  # (n_classes, n_features) -> [n_features, n_classes]
             new_biases: np.ndarray = clf.intercept_  # (n_classes,) -> [n_features,]
             num_classes, num_features = new_weights.shape[0], new_weights.shape[1]  # in_features, out_features=Dout
             module.weight = torch.nn.Parameter(torch.from_numpy(new_weights).to(torch.float32))
@@ -235,35 +253,36 @@
         # # Predict using adapted final layer with qrt set
         # query_y_pred_t = torch.Tensor(mdl.predict(qry_embeddings_t))
         # qry_loss_t = args.criterion(query_y_pred_t, qry_y_t)
         # qry_acc_t = r2_score_from_torch(qry_y_t, query_y_pred_t)
         assert False
     else:
         raise ValueError(f'Not implement: {target_type}')
-    return base_model
+    return model
 
 
-def get_embedding(x: Tensor, base_model: nn.Module) -> Tensor:
+def get_embedding(x: Tensor, model: nn.Module) -> Tensor:
     """ apply f until the last layer, instead return that as the embedding """
     out = x
     # if it has a get embedding later
-    if hasattr(base_model, 'get_embedding'):
-        out = base_model.get_embedding(x)
+    if hasattr(model, 'get_embedding'):
+        out = model.get_embedding(x)
         return out
     # for l2l
-    if hasattr(base_model, 'features'):
-        out = base_model.features(x)
-        return out
-    # for handling base_models with self.model.features self.model.cls format
-    if hasattr(base_model, 'model'):
-        out = base_model.model.features(x)
+    if hasattr(model, 'features'):
+        out = model.features(x)
         return out
-    # for handling synthetic base base_models
+    # for handling models with self.model.features self.model.cls format
+    if hasattr(model, 'model'):
+        if hasattr(model.model, 'features'):
+            out = model.model.features(x)
+            return out
+    # for handling synthetic base models
     # https://discuss.pytorch.org/t/module-children-vs-module-modules/4551/3
-    for name, m in base_model.named_children():
+    for name, m in model.named_children():
         if 'final' in name:
             return out
         if 'l2' in name and 'final' not in name:  # cuz I forgot to write final...sorry!
             return out
         if name == 'fc':
             return out
         out = m(out)
@@ -291,43 +310,64 @@
     query = query / query_norm
 
     cosine_distance = query @ support.transpose()
     max_idx = np.argmax(cosine_distance, axis=1)
     pred = [support_ys[idx] for idx in max_idx]
     return pred
 
+
 def Proto(support, support_ys, query, opt):
     """Protonet classifier"""
     nc = support.shape[-1]
     support = np.reshape(support, (-1, 1, opt.n_ways, opt.n_shots, nc))
     support = support.mean(axis=3)
     batch_size = support.shape[0]
     query = np.reshape(query, (batch_size, -1, 1, nc))
     logits = - ((query - support) ** 2).sum(-1)
     pred = np.argmax(logits, axis=-1)
     pred = np.reshape(pred, (-1,))
     return pred
 
+
 # - tests
 
-def setup_and_get_logger(args):
-    args.logging = True
-    args.log_root = Path('//experiments/logs/').expanduser()
-    current_logs_dir = Path(f'logs')
-    args.current_logs_path = args.log_root / current_logs_dir
-    args.current_logs_path.mkdir(parents=True, exist_ok=True)
-    # set up path + log filename
-    my_stdout_filename = Path('my_stdout.log')
-    args.my_stdout_filepath = args.current_logs_path / my_stdout_filename
-    # make logger
-    logger = Logger(args)  # logs to file & console
-    return logger
+def features_vit_pre_train():
+    # - ViT feature extractor
+    from transformers import ViTFeatureExtractor, ViTModel
+    from uutils.torch_uu.mains.common import get_and_create_model_opt_scheduler_for_run
+    from uutils.argparse_uu.meta_learning import get_args_vit_mdl_maml_l2l_agent_default
+    args: Namespace = get_args_vit_mdl_maml_l2l_agent_default()
+    from uutils.torch_uu.distributed import set_devices
+    set_devices(args)
+    get_and_create_model_opt_scheduler_for_run(args)
+    print(f'{type(args.model)=}')
+    x = torch.randn(25, 3, 84, 84)
+    features = get_embedding(x, args.model)
+    print(f'{features.shape=}')
+    print()
+
+    # - using my ViT cls class
+    from uutils.torch_uu.dataloaders.meta_learning.l2l_to_torchmeta_dataloader import \
+        forward_pass_with_pretrain_convergence_ffl_meta_learner
+    forward_pass_with_pretrain_convergence_ffl_meta_learner()
+    agent = FitFinalLayer(args, args.model)
+    x = torch.randn(3, 25, 3, 84, 84)
+    y = torch.randint(low=0, high=5, size=(x.size(0), x.size(1)), dtype=torch.long)
+    meta_loss, meta_loss_ci, meta_acc, meta_acc_ci = agent([x, y, x, y])
+    print(f'{meta_loss=}, {meta_loss_ci=}, {meta_acc=}, {meta_acc_ci=}')
+
+    # -
+    from uutils.torch_uu.dataloaders.meta_learning.l2l_to_torchmeta_dataloader import \
+        forward_pass_with_pretrain_convergence_ffl_meta_learner
+    forward_pass_with_pretrain_convergence_ffl_meta_learner()
+    agent = FitFinalLayer(args, args.model)
 
 
 if __name__ == '__main__':
     print('__main__ started!')
     import time
 
     start = time.time()
     # test_f_rand_is_worse_than_f_avg()
+    features_vit_pre_train()
     seconds = time.time() - start
     print(f'seconds = {seconds}, hours = {seconds / 60} \n\a')
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/metrics/metrics.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/metrics/metrics.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/mit_trainer_code.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/mit_trainer_code.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/__init__.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/__init__.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/custom_layers.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/fullyconnected.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/fullyconnected.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/hbf.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/hbf.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/hf_uu/__init__.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/hf_uu/__init__.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/kcnn.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/kcnn.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/l2l_models.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/l2l_models.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/learner_from_opt_as_few_shot_paper.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/learner_from_opt_as_few_shot_paper.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,23 +29,25 @@
 from uutils.torch_uu.models.spp import SPP
 
 
 def helloworld(msg="hello"):
     print(f'hello world with mgs: {msg}')
 
 
-def get_defaul_args_for_5cnn() -> Namespace:
-    args: Namespace = Namespace()
-    args.image_size = 84
-    args.bn_eps = 1e-3
-    args.bn_momentum = 0.95
-    args.n_classes = 5
-    args.filter_size = 32
-    args.levels = None
-    args.spp = False
+def get_defaul_args_for_5cnn(args: Optional = None) -> Namespace:
+    if args is None:
+        args: Namespace = Namespace()
+    else:
+        args.image_size = 84
+        args.bn_eps = 1e-3
+        args.bn_momentum = 0.95
+        args.n_classes = 5
+        args.filter_size = 32
+        args.levels = None
+        args.spp = False
     return args
 
 
 def get_learner_from_args(args: Namespace) -> nn.Module:
     return Learner(args.image_size, args.bn_eps, args.bn_momentum, args.n_classes)
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/mit_nn_models.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/mit_nn_models.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/probe_networks.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/probe_networks.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,68 @@
 from argparse import Namespace
+from torch.nn import Module
 from typing import Optional
 
-import task2vec
-from models import get_model, gaussian_net
-from task2vec import ProbeNetwork
-
+from uutils.torch_uu.metrics.diversity.task2vec_based_metrics.task2vec import ProbeNetwork
 
 def get_probe_network(args: Namespace,
 
                       model_option: Optional[str] = None,
                       **model_hps
-                      ) -> task2vec.ProbeNetwork:
+                      ) -> ProbeNetwork:
     """
     Note: a model is not the same as a probe network. Make sure you respect the probe network interface.
 
     :param args:
     :param model_option:
     :return:
     """
+    from uutils.torch_uu.metrics.diversity.task2vec_based_metrics.models import get_model
+
+    # print(f'{get_model=}')
     model_option: str = args.model_option if model_option is None else model_option
     if model_option == 'None':
         probe_network: ProbeNetwork = get_model('resnet18', pretrained=True, num_classes=5)
     elif model_option == 'resnet18_pretrained_imagenet':
         probe_network: ProbeNetwork = get_model('resnet18', pretrained=True, num_classes=args.n_cls)
     elif model_option == 'resnet18_random':
         probe_network: ProbeNetwork = get_model('resnet18', pretrained=False, num_classes=args.n_cls)
     elif model_option == 'resnet34_pretrained_imagenet':
         probe_network: ProbeNetwork = get_model('resnet34', pretrained=True, num_classes=args.n_cls)
     elif model_option == 'resnet34_random':
         probe_network: ProbeNetwork = get_model('resnet34', pretrained=False, num_classes=args.n_cls)
     elif model_option == '5cnn_random':
-        # probe_network: nn.Module = get_default_learner()
+        from uutils.torch_uu.models.learner_from_opt_as_few_shot_paper import get_default_learner_and_hps_dict
+        probe_network, _ = get_default_learner_and_hps_dict()  # 5cnn
+        # probe_network: Module = get_default_learner()
         # probe_network: ProbeNetwork = get_5CNN_random_probe_network()
+        # not implemented because it needs the probe network API I think...
         raise NotImplementedError
     elif model_option == '3FNN_5_gaussian':
+        from models import get_model, gaussian_net
         probe_network: ProbeNetwork = gaussian_net(num_classes=args.n_cls)
     else:
         raise ValueError(f'')
 
-    assert isinstance(probe_network, task2vec.ProbeNetwork), f'Make sure your model is of type ProbeNework & respects' \
+    assert isinstance(probe_network, ProbeNetwork), f'Make sure your model is of type ProbeNework & respects' \
                                                              f'its API. Got type: {type(probe_network)}'
+    # -
+    from uutils.torch_uu.distributed import move_model_to_dist_device_or_serial_device
+    probe_network = move_model_to_dist_device_or_serial_device(args.rank, args, probe_network)
     return probe_network
+
+
+# tests
+
+def get_model_test():
+    print(f'{get_model=}')
+    probe_network: ProbeNetwork = get_model('resnet18', pretrained=True, num_classes=5)
+    print(probe_network)
+
+    args = Namespace(n_cls=5)
+    args.model_option = 'resnet18_pretrained_imagenet'
+    probe_network: ProbeNetwork = get_probe_network(args)
+    print(probe_network)
+
+
+if __name__ == '__main__':
+    get_model_test()
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/resnet_rfs.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/resnet_rfs.py`

 * *Files 1% similar despite different names*

```diff
@@ -257,36 +257,45 @@
     def get_embedding(self, x):
         [f0, f1, f2, f3, feat], x = self.forward(x, is_feat=True)
         return feat
 
 
 def resnet12(keep_prob=1.0, avg_pool=False, **kwargs):
     """Constructs a ResNet-12 model.
+    indeed, only (1 + 1 + 1 + 1) * 3 + 1 = 12 + 1 layers
+
+    note:
+        - each block has 3 conv layers, so 1,1,1,1 blocks has 3,3,3,3 conv layers so 12 layers. When it says its
+        a resnet 12 it means it has 12 conv layers.
     """
     model = ResNet(BasicBlock, [1, 1, 1, 1], keep_prob=keep_prob, avg_pool=avg_pool, **kwargs)
     return model
 
 
 def resnet18(keep_prob=1.0, avg_pool=False, **kwargs):
     """Constructs a ResNet-18 model.
+    indeed, only (1 + 1 + 2 + 2) * 3 + 1 = 19 layers
     """
     model = ResNet(BasicBlock, [1, 1, 2, 2], keep_prob=keep_prob, avg_pool=avg_pool, **kwargs)
     return model
 
 
 def resnet24(keep_prob=1.0, avg_pool=False, **kwargs):
     """Constructs a ResNet-24 model.
     """
     model = ResNet(BasicBlock, [2, 2, 2, 2], keep_prob=keep_prob, avg_pool=avg_pool, **kwargs)
     return model
 
 
 def resnet50(keep_prob=1.0, avg_pool=False, **kwargs):
     """Constructs a ResNet-50 model.
-    indeed, only (3 + 4 + 6 + 3) * 3 + 1 = 49 layers
+    indeed, only (3 + 4 + 6 + 3) * 3 + 1 = 48+1 = 49 layers
+
+    note: it doesn't seem to be consistent with their own couting for resnet12. Sometimes they count the final layer
+    sometimes they dont't.
     """
     model = ResNet(BasicBlock, [3, 4, 6, 3], keep_prob=keep_prob, avg_pool=avg_pool, **kwargs)
     return model
 
 
 def resnet101(keep_prob=1.0, avg_pool=False, **kwargs):
     """Constructs a ResNet-101 model.
@@ -332,14 +341,15 @@
     model = ResNet(BasicBlock, [3, 4, 23, 3], keep_prob=keep_prob, avg_pool=avg_pool, use_se=True, **kwargs)
     return model
 
 
 model_dict = {
     'resnet12_rfs': resnet12,
     'resnet12_rfs_mi': resnet12,
+    'resnet12_hdb1_mio': resnet12,
     'resnet12_rfs_cifarfs_fc100': resnet12,
 
     'resnet18_rfs': resnet18,
     'resnet24_rfs': resnet24,
     'resnet50_rfs': resnet50,
     'resnet101_rfs': resnet101,
     'seresnet12_rfs': seresnet12,
@@ -363,30 +373,32 @@
     ref:
         - https://github.com/WangYueFt/rfs/blob/f8c837ba93c62dd0ac68a2f4019c619aa86b8421/models/util.py#L7
     """
     model_hps: dict = {'avg_pool': avg_pool,
                        'drop_rate': drop_rate,
                        'dropblock_size': dropblock_size,
                        'num_classes': num_classes}
+    # print(f'about to return model {model_opt}')
     model: nn.Module = model_dict[model_opt](avg_pool=avg_pool,
                                              drop_rate=drop_rate,
                                              dropblock_size=dropblock_size,
                                              num_classes=num_classes)
+    # print(f'got model {type(model)=}')
     return model, model_hps
 
 
 def get_resnet_rfs_model_cifarfs_fc100(model_opt: str,
                                        num_classes,
                                        avg_pool=True,
                                        drop_rate=0.1,
                                        dropblock_size=2,
                                        ) -> tuple[nn.Module, dict]:
     """
     ref:
-        - https://github.com/WangYueFt/rfs/blob/f8c837ba93c62dd0ac68a2f4019c619aa86b8421/models/util.py#L7
+        - https://github.com/WangYueFt/rfs/blob/f8c837ba93c62dd0ac68a2f4019c619aa86b8421/models/util.py#L23
     """
     model_hps: dict = {'avg_pool': avg_pool,
                        'drop_rate': drop_rate,
                        'dropblock_size': dropblock_size,
                        'num_classes': num_classes}
     model: nn.Module = model_dict[model_opt](avg_pool=avg_pool,
                                              drop_rate=drop_rate,
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/rfs_convnet.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/rfs_convnet.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/models/spp.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/models/spp.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/adafactor_uu.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/adafactor_uu.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,19 +67,14 @@
 def get_uutils_default_adafactor_from_torch_optimizer_and_scheduler_default(mdl: nn.Module,
                                                                             lr: float = 1e-4,
                                                                             scheduler_opt: Optional[str] = None
                                                                             ) -> tuple[Optimizer, _LRScheduler]:
     """
     Gets adafactor with uutils default parameters.
 
-    e.g.:
-    >>> import torch_optimizer as optim
-    # model = ...
-    >>> optimizer = optim.DiffGrad(model.parameters(), lr=0.001)
-    >>> optimizer.step()
     refs:
         - https://github.com/jettify/pytorch-optimizer/issues/405
         - https://github.com/huggingface/transformers/issues/14574
         - https://stackoverflow.com/questions/70218565/how-to-have-adafactor-run-a-custom-rfs-resnet12-with-maml-with-the-torch-opt?noredirect=1&lq=1
         - https://stackoverflow.com/questions/70171427/adafactor-from-transformers-hugging-face-only-works-with-transfromers-does-it
     """
     import torch_optimizer as optim
@@ -190,14 +185,17 @@
                                                    weight_decay=0.0,
                                                    scale_parameter=True,
                                                    relative_step=True,
                                                    warmup_init=False,
                                                    ) -> tuple[Optimizer, dict]:
     """
     Get the optimizer and scheduler objects for the current model and the hyperparameters (hps) that created it.
+
+    note:
+        - set when "AdafactorDefaultFair" is on.
     """
     # - hps
     opt_hps: dict = dict(
         lr=lr,
         eps=eps,
         clip_threshold=clip_threshold,
         decay_rate=decay_rate,
@@ -205,14 +203,15 @@
         weight_decay=weight_decay,
         scale_parameter=scale_parameter,
         relative_step=relative_step,
         warmup_init=warmup_init,
     )
 
     # - get opt & scheduler from hps
+    # if import throws bug you likely need:  pip install setuptools==59.5.0 ref: https://stackoverflow.com/questions/70520120/attributeerror-module-setuptools-distutils-has-no-attribute-version
     from fairseq import optim
     optimizer: Optimizer = optim.adafactor.Adafactor(params=mdl.parameters(), **opt_hps)
     return optimizer, opt_hps
 
 
 def get_default_adafactor_scheduler_fairseq_and_hps_dict(optimizer: Optimizer,
                                                          initial_lr=0.0,
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/adam_uu.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/adam_uu.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/common.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/common.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/sgd_uu.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/optim_uu/sgd_uu.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/tensorboard.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/tensorboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # from torch_uu.utils.tensorboard import SummaryWriter  # https://deeplizard.com/learn/video/psexxmdrufm
 from pathlib import Path
 
+
 def log_2_tb(tb, args, it, tag1: str, loss: float, tag2: str, acc: float):
     # tb = SummaryWriter(log_dir=args.current_logs_path)  # uncomment for documentation to work
     # tag1 = tag1.replace(' ', '_')
     # tag2 = tag2.replace(' ', '_')
     tb.add_scalar(tag1, float(loss), it)
     tb.add_scalar(tag2, float(acc), it)
 
+
 def log_2_tb_supervisedlearning(tb, args, it, loss, acc, split):
     """
     :param tb:
     :param acc:
     :param acc_err:
     :param loss:
     :param it:
@@ -30,14 +32,15 @@
         tag2 = f'{split}_accuracy'
     else:
         raise ValueError(f'Error: args.target_type = {args.target_type} not valid.')
     # tb = SummaryWriter(log_dir=args.current_logs_path)  # uncomment for documentation to work
     tb.add_scalar(tag1, loss, it)
     tb.add_scalar(tag2, acc, it)
 
+
 def log_2_tb_metalearning(tb, args, it, loss, acc, split):
     """
     :param tb:
     :param acc:
     :param loss:
     :param it:
     :param args:
@@ -55,14 +58,15 @@
         tag2 = f'meta-{split}_accuracy'
     else:
         raise ValueError(f'Error: args.target_type = {args.target_type} not valid.')
     # tb = SummaryWriter(log_dir=args.current_logs_path)  # uncomment for documentation to work
     tb.add_scalar(tag1, loss, it)
     tb.add_scalar(tag2, acc, it)
 
+
 def log_2_tb_metalearning_old(tb, args, it, loss, acc_err, split):
     """
     :param acc:
     :param loss:
     :param it:
     :param args:
     :param split: train, val, test
@@ -76,45 +80,48 @@
         tag2 = f'meta-{split}_accuracy'
     else:
         raise ValueError(f'Error: args.target_type = {args.target_type} not valid.')
     # tb = SummaryWriter(log_dir=args.current_logs_path)  # uncomment for documentation to work
     tb.add_scalar(tag1, loss, it)
     tb.add_scalar(tag2, acc_err, it)
 
+
 def tensorboard_run_list_2_matplotlib_list(data: list[tuple], smoothing_weight: float) -> tuple[list, list]:
     """
     :param data: data in format [..., [time, it, value], ...]
         e.g [[1603380383.1535034, 200, 1.5554816722869873], [1603381593.4793968, 900, 1.235633373260498]
     :return:
     """
     its: list[int] = []
     values: list[float] = []
     for _, it, value in data:
         its.append(it)
         values.append(value)
     values = my_tb_smooth(scalars=values, weight=smoothing_weight)
     return its, values
 
+
 def my_tb_smooth(scalars: list[float], weight: float) -> list[float]:  # Weight between 0 and 1
     """
 
     ref: https://stackoverflow.com/questions/42011419/is-it-possible-to-call-tensorboard-smooth-function-manually
 
     :param scalars:
     :param weight:
     :return:
     """
     last = scalars[0]  # First value in the plot (first timestep)
     smoothed: list = []
     for point in scalars:
         smoothed_val = last * weight + (1 - weight) * point  # Calculate smoothed value
-        smoothed.append(smoothed_val)                        # Save it
-        last = smoothed_val                                  # Anchor the last smoothed value
+        smoothed.append(smoothed_val)  # Save it
+        last = smoothed_val  # Anchor the last smoothed value
     return smoothed
 
+
 # -- tests
 
 def test():
     from datetime import datetime
     print('\n---running tb test, writing ot a tb...')
     import numpy as np
     from torch.utils.tensorboard import SummaryWriter  # https://deeplizard.com/learn/video/psexxmdrufm
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/torch_geometric/__init__.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/torch_geometric/__init__.py`

 * *Files identical despite different names*

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/training/meta_training.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/training/supervised_learning.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,74 +1,68 @@
 """
+
+To save time, debug, coding; have everything be in terms of iterations, but control the frequency of logging with
+the log frequency parameter. When calling the epochs function, automatically set that in that function,
+else set some defaults in the argparse.
+
+
+# - halt when converged
+ref:
+    - https://forums.pytorchlightning.ai/t/what-is-the-standard-way-to-halt-a-script-when-it-has-converged/1415
+    - https://stackoverflow.com/questions/70405985/what-is-the-standard-way-to-train-a-pytorch-script-until-convergence
 """
 from argparse import Namespace
 from typing import Any
 
-import torch
-from learn2learn.data import TaskDataset
 from progressbar import ProgressBar
-from torch import Tensor
+from torch import nn, Tensor
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler
 
-import uutils
-from uutils.logging_uu.wandb_logging.meta_learning import log_zeroth_step
-from uutils.logging_uu.wandb_logging.supervised_learning import log_train_val_stats
-from uutils.torch_uu.checkpointing_uu.meta_learning import save_for_meta_learning
-from uutils.torch_uu.training.common import gradient_clip, scheduler_step, check_halt, get_trainer_progress_bar, \
+from uutils.logging_uu.wandb_logging.supervised_learning import log_train_val_stats, log_zeroth_step, \
+    log_train_val_stats_simple
+from uutils.torch_uu import AverageMeter
+from uutils.torch_uu.agents.common import Agent
+from uutils.torch_uu.distributed import print_dist, is_lead_worker
+from uutils.torch_uu.training.common import get_trainer_progress_bar, scheduler_step, check_halt, gradient_clip, \
     ConvergenceMeter
 
-from pdb import set_trace as st
-
 
-def print_inside_halt(args: Namespace, halt: bool, i: int = 0):
-    if args.it % args.log_freq == 0 or halt or args.debug:  # todo: remove? temporary for debugging
-        print(f'-- inside the halt, ith: {i=}')
-
-
-def meta_train_agent_fit_single_batch(args: Namespace,
-                                      meta_learner,
-                                      dataloaders: dict,
-                                      opt: Optimizer,
-                                      scheduler: _LRScheduler,
-                                      acc_tolerance: float = 1.0,
-                                      train_loss_tolerance: float = 0.01,
-                                      ):
+def train_agent_fit_single_batch(args: Namespace,
+                                 model: Agent,
+                                 dataloaders: dict,
+                                 opt: Optimizer,
+                                 scheduler: _LRScheduler,
+                                 acc_tolerance: float = 1.0,
+                                 train_loss_tolerance: float = 0.01,
+                                 ):
     """
     Train for a single batch
+
+    Note:
+        - eval_sl always chooses a different val set. So the val set should be stuck at ~0 if the model is only
+        fitting 1 batch (as this code does).
     """
-    # get one fixed meta-batch
-    # if hasattr(args, 'tasksets'):
-    #    # hack for l2l
-    #    from learn2learn.data import TaskDataset
-    #    split: str = 'validation' if split == 'val' else split
-    #    task_dataset: TaskDataset = getattr(args.tasksets, split)
-    #    assert self.args.batch_size >= 1
-    #    train_batch = : list = [task_dataset.sample() for task_num in range(self.args.batch_size)]
-    #    # train_batch = task_dataset
-    # else:  # torchmeta which has same api as pytorch dataloader
     train_batch: Any = next(iter(dataloaders['train']))
 
     # first batch
     args.it = 0  # training a single batch shouldn't need to use ckpts so this is ok
     args.best_val_loss = float('inf')  # training a single batch shouldn't need to use ckpts so this is ok
 
     # - create progress bar
     args.bar: ProgressBar = get_trainer_progress_bar(args)
 
     # - train in epochs
-    args.convg_meter: ConvergenceMeter = ConvergenceMeter(name='train loss',
-                                                          convergence_patience=args.train_convergence_patience)
-    # log_zeroth_step(args, model)
+    args.convg_meter = ConvergenceMeter(name='train loss', convergence_patience=args.train_convergence_patience)
+    log_zeroth_step(args, model)
     halt: bool = False
     while not halt:
         opt.zero_grad()
-        train_loss, train_acc, train_loss_std, train_acc_std = meta_learner(train_batch, call_backward=True)
-        # train_loss.backward()  # each process synchronizes its gradients in the backward pass
-        assert opt.param_groups[0]['params'][0].grad is not None
+        train_loss, train_acc = model(train_batch, training=True)
+        train_loss.backward()  # each process synchronizes its gradients in the backward pass
         gradient_clip(args, opt)
         opt.step()  # the right update is done since all procs have the right synced grads
         if (args.it % args.log_scheduler_freq == 0) or args.debug:
             scheduler_step(args, scheduler)
 
         # - break
         halt: bool = train_acc >= acc_tolerance and train_loss <= train_loss_tolerance
@@ -76,53 +70,50 @@
 
         args.it += 1
 
         # - log full stats
         # when logging after +=1, log idx will be wrt real idx i.e. 0 doesn't mean first it means true 0
         if args.epoch_num % args.log_freq == 0 or halt or args.debug:
             step_name: str = 'epoch_num' if 'epochs' in args.training_mode else 'it'
-            log_train_val_stats(args, args.it, step_name, train_loss, train_acc, training=True)
+            log_train_val_stats(args, args.it, step_name, train_loss.item(), train_acc.item())
 
         if halt:
             break
 
     return train_loss, train_acc
 
 
-def meta_train_fixed_iterations(args: Namespace,
-                                meta_learner,
-                                dataloaders,
-                                outer_opt,
-                                scheduler,
-                                training: bool = True
-                                ) -> tuple[Tensor, Tensor, Tensor, Tensor]:
-    """
-    Train using the meta-training (e.g. episodic training) over batches of tasks using a fixed number of iterations
-    assuming the number of tasks is small i.e. one epoch is doable and not infinite/super exponential
-    (e.g. in regression when a task can be considered as a function).
-
-    Note: if num tasks is small then we have two loops, one while we have not finished all fixed its and the other
-    over the dataloader for the tasks.
-    """
-    print('Starting training!')
-
-    # args.bar = uutils.get_good_progressbar(max_value=progressbar.UnknownLength)
-    args.bar = uutils.get_good_progressbar(max_value=args.num_its)
-    meta_learner.train() if training else meta_learner.eval()
+def train_agent_iterations(args: Namespace,
+                           model: Agent,
+                           dataloaders: dict,
+                           opt: Optimizer,
+                           scheduler: _LRScheduler,
+                           ) -> tuple[Tensor, Tensor]:
+    """
+    Trains models wrt to number of iterations given. Should halt once the number of iterations desired is reached. 
+    """
+    print_dist('Starting training...', args.rank)
+    print_dist(f'{train_agent_iterations=}', args.rank)
+
+    # - create progress bar
+    args.bar: ProgressBar = get_trainer_progress_bar(args)
+
+    # - train
+    args.convg_meter = ConvergenceMeter(name='train loss', convergence_patience=args.train_convergence_patience)
+    log_zeroth_step(args, model)
     halt: bool = False
-    # TODO have a logging of the zeroth step...
-    print('About to enter the while not halt loop training...')
+    # - continually try to train accross the entire epoch but stop once the number of iterations desired is reached
     while not halt:
-        for batch_idx, batch in enumerate(dataloaders['train']):
-            outer_opt.zero_grad()
-            train_loss, train_acc, train_loss_std, train_acc_std = meta_learner(batch, call_backward=True)
-            # train_loss.backward()  # NOTE: backward was already called in meta-learner due to MEM optimization.
-            assert outer_opt.param_groups[0]['params'][0].grad is not None
-            gradient_clip(args, outer_opt)  # do gradient clipping: * If ‖g‖ ≥ c Then g := c * g/‖g‖
-            outer_opt.step()
+        # -- train for one epoch
+        for i, batch in enumerate(dataloaders['train']):
+            opt.zero_grad()
+            train_loss, train_acc = model(batch, training=True)
+            train_loss.backward()  # each process synchronizes its gradients in the backward pass
+            gradient_clip(args, opt)
+            opt.step()  # the right update is done since all procs have the right synced grads
 
             # - scheduler
             if (args.it % args.log_scheduler_freq == 0) or args.debug:
                 scheduler_step(args, scheduler)
 
             # - convergence (or idx + 1 == n, this means you've done n loops where idx = it or epoch_num).
             halt: bool = check_halt(args)
@@ -130,86 +121,97 @@
             # - go to next it & before that check if we should halt
             args.it += 1
 
             # - log full stats
             # when logging after +=1, log idx will be wrt real idx i.e. 0 doesn't mean first it means true 0
             if args.it % args.log_freq == 0 or halt or args.debug:
                 step_name: str = 'epoch_num' if 'epochs' in args.training_mode else 'it'
-                log_train_val_stats(args, args.it, step_name, train_loss, train_acc, training=True)
-                # args.convg_meter.update(train_loss)
+                log_train_val_stats(args, args.it, step_name, train_loss, train_acc)
+                args.convg_meter.update(train_loss)
 
             # - break out of the inner loop to start halting, the outer loop will terminate too since halt is True.
             if halt:
                 break
 
-    return train_loss, train_acc, train_loss_std, train_acc_std
+    return train_loss, train_acc
+
 
+def train_agent_epochs(args: Namespace,
+                       model: Agent,
+                       dataloaders: dict,
+                       opt: Optimizer,
+                       scheduler: _LRScheduler,
+                       ) -> tuple[Tensor, Tensor]:
+    """
+    Trains model one epoch at a time - i.e. it's epochs based rather than iteration based.
+    """
+    print_dist('Starting training...', args.rank)
+    print_dist(f'{train_agent_epochs=}', args.rank)
+    B: int = args.batch_size
 
-def meta_train_iterations_ala_l2l(args: Namespace,
-                                  meta_learner,
-                                  outer_opt,
-                                  scheduler,
-
-                                  training: bool = True
-                                  ):
-    """"""
-    # torch.autograd.set_detect_anomaly(True)
-    print('Starting training!')
-    meta_batch_size: int = args.batch_size // args.world_size
-    # print(args.batch_size, meta_batch_size, "args and Meta BatchSize")
-    # args.bar = uutils.get_good_progressbar(max_value=progressbar.UnknownLength)
-    args.bar = uutils.get_good_progressbar(max_value=args.num_its)
-    meta_learner.train() if training else meta_learner.eval()
-    halt: bool = False
+    # - create progress bar
+    args.bar: ProgressBar = get_trainer_progress_bar(args)
 
-    # ----added - 0th iter---#
-    log_zeroth_step(args, meta_learner)
-    # --------#
+    # - train
+    log_zeroth_step(args, model)
+    halt: bool = False
+    # - continually train but one epoch at a time
     while not halt:
-        # print_inside_halt(args, halt, 0)  # todo: remove? temporary for debugging
-        outer_opt.zero_grad()
-        # print_inside_halt(args, halt, 1)  # todo: remove? temporary for debugging
-
-        # - forward pass. Since the data fetching is different for l2l we do it this way
-        task_dataset: TaskDataset = args.tasksets.train
-        # print_inside_halt(args, halt, 2)  # todo: remove? temporary for debugging
-        train_loss, train_loss_std, train_acc, train_acc_std = meta_learner(task_dataset, call_backward=True)
-        # print_inside_halt(args, halt, 3)  # todo: remove? temporary for debugging
-        # train_loss.backward()  # NOTE: backward was already called in meta-learner due to MEM optimization.
-        assert outer_opt.param_groups[0]['params'][0].grad is not None
-        # print_inside_halt(args, halt, 4)  # todo: remove? temporary for debugging
-
-        # - Grad clip  (optional)
-        gradient_clip(args, outer_opt)  # do gradient clipping: * If ‖g‖ ≥ c Then g := c * g/‖g‖
-        # print_inside_halt(args, halt, 5)  # todo: remove? temporary for debugging
-
-        # - Opt Step - Average the accumulated gradients and optimize
-        from uutils.torch_uu.distributed import is_running_parallel
-        # print_inside_halt(args, halt, 6)  # todo: remove? temporary for debugging
-        if is_running_parallel(args.rank):
-            for p in meta_learner.parameters():
-                p.grad.data.mul_(1.0 / meta_batch_size)
-        # print_inside_halt(args, halt, 7)  # todo: remove? temporary for debugging
-        outer_opt.step()  # averages gradients across all workers
-        # print_inside_halt(args, halt, 8)  # todo: remove? temporary for debugging
+        # -- train for one epoch
+        avg_loss = AverageMeter('train loss')
+        avg_acc = AverageMeter('train accuracy')
+        for i, batch in enumerate(dataloaders['train']):
+            opt.zero_grad()
+            train_loss, train_acc = model(batch, training=True)
+            train_loss.backward()  # each process synchronizes its gradients in the backward pass
+            gradient_clip(args, opt)
+            opt.step()  # the right update is done since all procs have the right synced grads
+
+            # - meter updates
+            avg_loss.update(train_loss.item(), B), avg_acc.update(train_acc, B)
+            if args.debug:
+                print_dist(msg=f'[{args.epoch_num=}, {i=}] {train_loss=}, {train_acc=}', rank=args.rank, flush=True)
 
-        # - Scheduler
-        if (args.it % args.log_scheduler_freq == 0) or args.debug:
+        # - scheduler, not in first/0th epoch though
+        if (args.epoch_num % args.log_scheduler_freq == 0) or args.debug:
             scheduler_step(args, scheduler)
 
-        # - Convergence (or idx + 1 == n, this means you've done n loops where idx = it or epoch_num).
+        # convergence (or idx + 1 == n, this means you've done n loops where idx = it or epoch_num).
         halt: bool = check_halt(args)
 
         # - go to next it & before that check if we should halt
-        args.it += 1
+        args.epoch_num += 1
 
-        # - log full stats
+        # - log full epoch stats
         # when logging after +=1, log idx will be wrt real idx i.e. 0 doesn't mean first it means true 0
-        if args.it % args.log_freq == 0 or halt or args.debug:
+        if args.epoch_num % args.log_freq == 0 or halt or args.debug:
             step_name: str = 'epoch_num' if 'epochs' in args.training_mode else 'it'
-            log_train_val_stats(args, args.it, step_name, train_loss, train_acc, training=True)
-            # args.convg_meter.update(train_loss)
+            log_train_val_stats(args, args.epoch_num, step_name, avg_loss.item(), avg_acc.item())
+            args.convg_meter.update(avg_loss.item())
 
-        # - break out of the inner loop to start halting, the outer loop will terminate too since halt is True.
-        if halt:
-            break
-    return train_loss, train_acc, train_loss_std, train_acc_std
+    return avg_loss.item(), avg_acc.item()
+
+
+# -- run __main__
+
+def training_test_():
+    # - usl
+    from uutils.torch_uu.mains.common import get_and_create_model_opt_scheduler_for_run
+    from uutils.argparse_uu.supervised_learning import get_args_mi_usl_default
+    from uutils.torch_uu.agents.supervised_learning import ClassificationSLAgent
+    args: Namespace = get_args_mi_usl_default()
+    get_and_create_model_opt_scheduler_for_run(args)
+    args.agent = ClassificationSLAgent(args, args.model)
+    from uutils.torch_uu.dataloaders.helpers import get_sl_dataloader
+    args.dataloaders = get_sl_dataloader(args)
+    train_loss, train_acc = train_agent_iterations(args, args.agent, args.dataloaders, args.opt, args.scheduler)
+    print(f'{train_loss, train_acc=}')
+
+
+# - run __main__
+
+if __name__ == '__main__':
+    import time
+
+    start = time.time()
+    training_test_()
+    print(f'Done in {time.time() - start} seconds.')
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `ultimate-utils-0.6.1/ultimate-utils-proj-src/uutils/torch_uu/training/supervised_learning.py` & `ultimate-utils-0.7.0/ultimate-utils-proj-src/uutils/torch_uu/training/meta_training.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,63 @@
 """
-
-To save time, debug, coding; have everything be in terms of iterations, but control the frequency of logging with
-the log frequency parameter. When calling the epochs function, automatically set that in that function,
-else set some defaults in the argparse.
-
-
-# - halt when converged
-ref:
-    - https://forums.pytorchlightning.ai/t/what-is-the-standard-way-to-halt-a-script-when-it-has-converged/1415
-    - https://stackoverflow.com/questions/70405985/what-is-the-standard-way-to-train-a-pytorch-script-until-convergence
 """
 from argparse import Namespace
 from typing import Any
 
+import torch
+from learn2learn.data import TaskDataset
 from progressbar import ProgressBar
-from torch import nn, Tensor
+from torch import Tensor
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler
+from torch.utils.data import DataLoader
 
-from uutils.logging_uu.wandb_logging.supervised_learning import log_train_val_stats, log_zeroth_step, \
-    log_train_val_stats_simple
-from uutils.torch_uu import AverageMeter
-from uutils.torch_uu.agents.common import Agent
-from uutils.torch_uu.distributed import print_dist, is_lead_worker
-from uutils.torch_uu.training.common import get_trainer_progress_bar, scheduler_step, check_halt, gradient_clip, \
+import uutils
+from uutils.logging_uu.wandb_logging.supervised_learning import log_train_val_stats, log_zeroth_step
+from uutils.torch_uu.checkpointing_uu.meta_learning import save_for_meta_learning
+from uutils.torch_uu.training.common import gradient_clip, scheduler_step, check_halt, get_trainer_progress_bar, \
     ConvergenceMeter
 
+from pdb import set_trace as st
+
 
-def train_agent_fit_single_batch(args: Namespace,
-                                 model: Agent,
-                                 dataloaders: dict,
-                                 opt: Optimizer,
-                                 scheduler: _LRScheduler,
-                                 acc_tolerance: float = 1.0,
-                                 train_loss_tolerance: float = 0.01,
-                                 ):
+def print_inside_halt(args: Namespace, halt: bool, i: int = 0):
+    if args.it % args.log_freq == 0 or halt or args.debug:  # todo: remove? temporary for debugging
+        print(f'-- inside the halt, ith: {i=}')
+
+
+def meta_train_agent_fit_single_batch(args: Namespace,
+                                      meta_learner,
+                                      dataloaders: dict,
+                                      opt: Optimizer,
+                                      scheduler: _LRScheduler,
+                                      acc_tolerance: float = 1.0,
+                                      train_loss_tolerance: float = 0.01,
+                                      ):
     """
     Train for a single batch
-
-    Note:
-        - eval_sl always chooses a different val set. So the val set should be stuck at ~0 if the model is only
-        fitting 1 batch (as this code does).
     """
     train_batch: Any = next(iter(dataloaders['train']))
 
     # first batch
     args.it = 0  # training a single batch shouldn't need to use ckpts so this is ok
     args.best_val_loss = float('inf')  # training a single batch shouldn't need to use ckpts so this is ok
 
     # - create progress bar
     args.bar: ProgressBar = get_trainer_progress_bar(args)
 
     # - train in epochs
-    args.convg_meter: ConvergenceMeter = ConvergenceMeter(name='train loss', convergence_patience=args.train_convergence_patience)
-    log_zeroth_step(args, model)
+    args.convg_meter = ConvergenceMeter(name='train loss', convergence_patience=args.train_convergence_patience)
+    # log_zeroth_step(args, model) # not needed for fit single batch
     halt: bool = False
     while not halt:
         opt.zero_grad()
-        train_loss, train_acc = model(train_batch, training=True)
-        train_loss.backward()  # each process synchronizes its gradients in the backward pass
+        train_loss, train_loss_ci, train_acc, train_acc_ci = meta_learner(train_batch, call_backward=True)
+        # train_loss.backward()  # each process synchronizes its gradients in the backward pass
+        assert opt.param_groups[0]['params'][0].grad is not None
         gradient_clip(args, opt)
         opt.step()  # the right update is done since all procs have the right synced grads
         if (args.it % args.log_scheduler_freq == 0) or args.debug:
             scheduler_step(args, scheduler)
 
         # - break
         halt: bool = train_acc >= acc_tolerance and train_loss <= train_loss_tolerance
@@ -70,141 +65,183 @@
 
         args.it += 1
 
         # - log full stats
         # when logging after +=1, log idx will be wrt real idx i.e. 0 doesn't mean first it means true 0
         if args.epoch_num % args.log_freq == 0 or halt or args.debug:
             step_name: str = 'epoch_num' if 'epochs' in args.training_mode else 'it'
-            log_train_val_stats(args, args.it, step_name, train_loss, train_acc)
+            log_train_val_stats(args, args.it, step_name, train_loss, train_acc, training=True)
 
         if halt:
             break
 
     return train_loss, train_acc
 
 
-def train_agent_iterations(args: Namespace,
-                           model: Agent,
-                           dataloaders: dict,
-                           opt: Optimizer,
-                           scheduler: _LRScheduler,
-                           ) -> tuple[Tensor, Tensor]:
-    """
-    Trains model one epoch at a time - i.e. it's epochs based rather than iteration based.
-    """
-    print_dist('Starting training...', args.rank)
+def meta_train_fixed_iterations(args: Namespace,
+                                meta_learner,
+                                dataloaders,
+                                outer_opt,
+                                scheduler,
+                                training: bool = True
+                                ) -> tuple[Tensor, Tensor, Tensor, Tensor]:
+    """
+    Train using the meta-training (e.g. episodic training) over batches of tasks using a fixed number of iterations
+    assuming the number of tasks is small i.e. one epoch is doable and not infinite/super exponential
+    (e.g. in regression when a task can be considered as a function).
+
+    Note: if num tasks is small then we have two loops, one while we have not finished all fixed its and the other
+    over the dataloader for the tasks.
+    """
+    # - imports
+    from uutils.torch_uu.dataloaders.meta_learning.l2l_to_torchmeta_dataloader import \
+        episodic_batch_2_task_dataset
+
+    # - start!
+    print('----> Starting training!')
+    print(f'{meta_train_fixed_iterations=}')
 
     # - create progress bar
     args.bar: ProgressBar = get_trainer_progress_bar(args)
+    meta_learner.train() if training else meta_learner.eval()
+    halt: bool = False
 
-    # - train in epochs
+    # - meta-train
     args.convg_meter = ConvergenceMeter(name='train loss', convergence_patience=args.train_convergence_patience)
-    log_zeroth_step(args, model)
-    halt: bool = False
+    log_zeroth_step(args, meta_learner)
+    # - continually meta-train until halt condition is met (usually convergence or reaching max its)
+    print('--> Starting the episodic meta-training loop. Getting batches ala episodic way (e.g. ala torchmeta way)...')
+    loader: DataLoader = dataloaders['train']
     while not halt:
-        # -- train for one epoch
-        for i, batch in enumerate(dataloaders['train']):
-            opt.zero_grad()
-            train_loss, train_acc = model(batch, training=True)
-            train_loss.backward()  # each process synchronizes its gradients in the backward pass
-            gradient_clip(args, opt)
-            opt.step()  # the right update is done since all procs have the right synced grads
+        for batch_idx, batch in enumerate(loader):
+            outer_opt.zero_grad()
+            assert outer_opt is args.opt
+
+            if hasattr(loader, 'episodic_batch_2_task_dataset'):  # mainly for mds
+                batch: TaskDataset = episodic_batch_2_task_dataset(batch, loader, meta_learner)
+            train_loss, train_acc = meta_learner(batch, call_backward=True)
+            # train_loss.backward()  # NOTE: backward was already called in meta-learner due to MEM optimization.
+            assert outer_opt.param_groups[0]['params'][0].grad is not None
+            gradient_clip(args, outer_opt)  # do gradient clipping: * If ‖g‖ ≥ c Then g := c * g/‖g‖
+            outer_opt.step()
 
             # - scheduler
             if (args.it % args.log_scheduler_freq == 0) or args.debug:
                 scheduler_step(args, scheduler)
 
             # - convergence (or idx + 1 == n, this means you've done n loops where idx = it or epoch_num).
             halt: bool = check_halt(args)
 
             # - go to next it & before that check if we should halt
             args.it += 1
 
             # - log full stats
             # when logging after +=1, log idx will be wrt real idx i.e. 0 doesn't mean first it means true 0
-            if args.epoch_num % args.log_freq == 0 or halt or args.debug:
+            if args.it % args.log_freq == 0 or halt or args.debug:
                 step_name: str = 'epoch_num' if 'epochs' in args.training_mode else 'it'
-                log_train_val_stats(args, args.it, step_name, train_loss, train_acc)
+                log_train_val_stats(args, args.it, step_name, train_loss, train_acc, training=True)
                 args.convg_meter.update(train_loss)
 
             # - break out of the inner loop to start halting, the outer loop will terminate too since halt is True.
             if halt:
                 break
-
     return train_loss, train_acc
 
 
-def train_agent_epochs(args: Namespace,
-                       model: Agent,
-                       dataloaders: dict,
-                       opt: Optimizer,
-                       scheduler: _LRScheduler,
-                       ) -> tuple[Tensor, Tensor]:
-    """
-    Trains model one epoch at a time - i.e. it's epochs based rather than iteration based.
-    """
-    print_dist('Starting training...', args.rank)
-    B: int = args.batch_size
+def meta_train_iterations_ala_l2l(args: Namespace,
+                                  meta_learner,
+                                  outer_opt,
+                                  scheduler,
+                                  training: bool = True
+                                  ):
+    """"""
+    # torch.distributed.barrier()
+    print('Starting training!')
+    print(f'{meta_train_iterations_ala_l2l=}')
+    meta_batch_size: int = args.batch_size // args.world_size
+    # meta_batch_size: int = max(args.batch_size // args.world_size, 1)
+    # assert args.batch_size >= args.world_size, f'If batch size is smaller training might be slightly wrong when in distributed.'
 
     # - create progress bar
     args.bar: ProgressBar = get_trainer_progress_bar(args)
-
-    # - train in epochs
-    args.convg_meter = ConvergenceMeter(name='train loss', convergence_patience=args.train_convergence_patience)
-    log_zeroth_step(args, model)
+    meta_learner.train() if training else meta_learner.eval()
     halt: bool = False
 
-    # ----added - 0th iter---#
-    args.epochs_num = 0
-    avg_loss = AverageMeter('train loss')
-    avg_acc = AverageMeter('train accuracy')
-    for i, batch in enumerate(dataloaders['train']):
-        #opt.zero_grad()
-        train_loss, train_acc = model(batch, training=True)
-        #train_loss.backward()  # each process synchronizes its gradients in the backward pass
-        #gradient_clip(args, opt)
-        #opt.step()  # the right update is done since all procs have the right synced grads
-
-        # - meter updates
-        avg_loss.update(train_loss.item(), B), avg_acc.update(train_acc, B)
-        if args.debug:
-            print_dist(msg=f'[{args.epoch_num=}, {i=}] {train_loss=}, {train_acc=}', rank=args.rank, flush=True)
-    step_name: str = 'epoch_num' if 'epochs' in args.training_mode else 'it'
-    log_train_val_stats(args, args.epoch_num, step_name, avg_loss.item(), avg_acc.item())
-    args.epochs_num = 1
-    # --------#
+    # - meta-train
+    args.convg_meter = ConvergenceMeter(name='train loss', convergence_patience=args.train_convergence_patience)
+    log_zeroth_step(args, meta_learner)
+    # - continually meta-train until halt condition is met (usually convergence or reaching max its)
     while not halt:
-        # -- train for one epoch
-        avg_loss = AverageMeter('train loss')
-        avg_acc = AverageMeter('train accuracy')
-        for i, batch in enumerate(dataloaders['train']):
-            opt.zero_grad()
-            train_loss, train_acc = model(batch, training=True)
-            train_loss.backward()  # each process synchronizes its gradients in the backward pass
-            gradient_clip(args, opt)
-            opt.step()  # the right update is done since all procs have the right synced grads
-
-            # - meter updates
-            avg_loss.update(train_loss.item(), B), avg_acc.update(train_acc, B)
-            if args.debug:
-                print_dist(msg=f'[{args.epoch_num=}, {i=}] {train_loss=}, {train_acc=}', rank=args.rank, flush=True)
+        outer_opt.zero_grad()
+
+        # - forward pass. Since the data fetching is different for l2l we do it this way
+        task_dataset: TaskDataset = args.dataloaders.train
+        train_loss, train_acc = meta_learner(task_dataset, call_backward=True)
+        # train_loss.backward()  # NOTE: backward was already called in meta-learner due to MEM optimization.
+        assert outer_opt.param_groups[0]['params'][0].grad is not None
+
+        # - Grad clip  (optional)
+        gradient_clip(args, outer_opt)  # do gradient clipping: * If ‖g‖ ≥ c Then g := c * g/‖g‖
+
+        # - Opt Step - Average the accumulated gradients and optimize
+        from uutils.torch_uu.distributed import is_running_parallel
+        if is_running_parallel(args.rank):
+            for p in meta_learner.parameters():
+                if p.grad is not None:
+                    p.grad.data.mul_(1.0 / meta_batch_size)
+        outer_opt.step()  # averages gradients across all workers
 
-        # - scheduler, not in first/0th epoch though
-        if (args.epoch_num % args.log_scheduler_freq == 0) or args.debug:
+        # - Scheduler
+        if (args.it % args.log_scheduler_freq == 0) or args.debug:
             scheduler_step(args, scheduler)
 
-        # convergence (or idx + 1 == n, this means you've done n loops where idx = it or epoch_num).
+        # - Convergence (or idx + 1 == n, this means you've done n loops where idx = it or epoch_num).
         halt: bool = check_halt(args)
 
         # - go to next it & before that check if we should halt
-        args.epoch_num += 1
+        args.it += 1
 
-        # - log full epoch stats
+        # - log full stats
         # when logging after +=1, log idx will be wrt real idx i.e. 0 doesn't mean first it means true 0
-        if args.epoch_num % args.log_freq == 0 or halt or args.debug:
+        if args.it % args.log_freq == 0 or halt or args.debug:
             step_name: str = 'epoch_num' if 'epochs' in args.training_mode else 'it'
-            log_train_val_stats(args, args.epoch_num, step_name, avg_loss.item(), avg_acc.item())
-            args.convg_meter.update(avg_loss.item())
+            log_train_val_stats(args, args.it, step_name, train_loss, train_acc, training=True)
+            args.convg_meter.update(train_loss)
 
-    return avg_loss.item(), avg_acc.item()
+        # - break out of the inner loop to start halting, the outer loop will terminate too since halt is True.
+        if halt:
+            break
+    return train_loss, train_acc
 
+# - tests tutorials
 
+def training_test_():
+    # - torchmeta
+    from uutils.argparse_uu.meta_learning import get_args_mi_torchmeta_default
+    from uutils.torch_uu.mains.common import get_and_create_model_opt_scheduler_for_run
+    from uutils.torch_uu.meta_learners.maml_meta_learner import MAMLMetaLearner
+    args: Namespace = get_args_mi_torchmeta_default()
+    get_and_create_model_opt_scheduler_for_run(args)
+    args.agent = MAMLMetaLearner(args, args.model)
+    from uutils.torch_uu.dataloaders.meta_learning.helpers import get_meta_learning_dataloaders
+    args.dataloaders = get_meta_learning_dataloaders(args)
+    train_loss, train_acc = meta_train_fixed_iterations(args, args.agent, args.dataloaders, args.opt, args.scheduler)
+    print(f'{train_loss, train_acc=}')
+    # - l2l
+    from uutils.argparse_uu.meta_learning import get_args_mi_l2l_default
+    from uutils.torch_uu.dataloaders.meta_learning.l2l_ml_tasksets import get_l2l_tasksets
+    from uutils.torch_uu.mains.common import get_and_create_model_opt_scheduler_for_run
+    from uutils.torch_uu.meta_learners.maml_meta_learner import MAMLMetaLearnerL2L
+    args: Namespace = get_args_mi_l2l_default()
+    get_and_create_model_opt_scheduler_for_run(args)
+    args.agent = MAMLMetaLearnerL2L(args, args.model)
+    args.dataloaders = get_l2l_tasksets(args)
+    train_loss, train_acc = meta_train_iterations_ala_l2l(args, args.agent, args.opt, args.scheduler)
+    print(f'{train_loss, train_acc=}')
+
+# - run __main__
+
+if __name__ == '__main__':
+    import time
+    start = time.time()
+    training_test_()
+    print(f'Done in {time.time() - start} seconds.')
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

