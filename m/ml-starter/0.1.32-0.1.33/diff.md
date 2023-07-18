# Comparing `tmp/ml-starter-0.1.32.tar.gz` & `tmp/ml-starter-0.1.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ml-starter-0.1.32.tar", last modified: Tue Jul 18 05:37:01 2023, max compression
+gzip compressed data, was "ml-starter-0.1.33.tar", last modified: Tue Jul 18 06:20:58 2023, max compression
```

## Comparing `ml-starter-0.1.32.tar` & `ml-starter-0.1.33.tar`

### file list

```diff
@@ -1,183 +1,183 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.484514 ml-starter-0.1.32/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 05:36:49.000000 ml-starter-0.1.32/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-18 05:36:49.000000 ml-starter-0.1.32/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-18 05:37:01.484514 ml-starter-0.1.32/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-18 05:36:49.000000 ml-starter-0.1.32/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.440514 ml-starter-0.1.32/ml/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.444514 ml-starter-0.1.32/ml/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/core/common_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/core/env.py
--rw-r--r--   0 runner    (1001) docker     (123)    26629 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/core/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/core/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.444514 ml-starter-0.1.32/ml/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/launchers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/launchers/mp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/launchers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/launchers/torchrun.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.448514 ml-starter-0.1.32/ml/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/loggers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/loggers/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)    45793 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/loggers/multi.py
--rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/loggers/stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/loggers/tensorboard.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.448514 ml-starter-0.1.32/ml/lr_schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/lr_schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/lr_schedulers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/lr_schedulers/constant.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/lr_schedulers/cosine.py
--rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/lr_schedulers/cosine_decay.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/lr_schedulers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/lr_schedulers/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/lr_schedulers/linear_no_decay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.452514 ml-starter-0.1.32/ml/lr_schedulers/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/lr_schedulers/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/lr_schedulers/scripts/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.452514 ml-starter-0.1.32/ml/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/models/activations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/models/codebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/models/diffusion.py
--rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/models/embeddings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/models/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/models/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/models/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)    56014 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/models/lora.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/models/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/models/norms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/models/parallel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.456514 ml-starter-0.1.32/ml/optimizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/optimizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/optimizers/adam.py
--rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/optimizers/adan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/optimizers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/optimizers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/optimizers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/optimizers/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/optimizers/sgd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/optimizers/shampoo.py
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/optimizers/types.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.460514 ml-starter-0.1.32/ml/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/scripts/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/scripts/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/scripts/resolve.py
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/scripts/stage.py
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/scripts/train.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.460514 ml-starter-0.1.32/ml/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19338 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.464514 ml-starter-0.1.32/ml/tasks/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/datasets/async_iterable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/datasets/clippify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/datasets/collate.py
--rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/datasets/error_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/datasets/multi_iter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/datasets/samplers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/datasets/streaming.py
--rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/datasets/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/datasets/video_file.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.464514 ml-starter-0.1.32/ml/tasks/environments/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/environments/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/environments/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/environments/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.464514 ml-starter-0.1.32/ml/tasks/gan/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/gan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/gan/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.464514 ml-starter-0.1.32/ml/tasks/losses/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/losses/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/losses/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/losses/loss.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.464514 ml-starter-0.1.32/ml/tasks/rl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/rl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/rl/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/rl/replay.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.468514 ml-starter-0.1.32/ml/tasks/sl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/sl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/tasks/sl/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.468514 ml-starter-0.1.32/ml/trainers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23597 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/gan.py
--rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/learning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.472514 ml-starter-0.1.32/ml/trainers/mixins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/mixins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/mixins/compile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/mixins/cpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/mixins/data_parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/mixins/gpu_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/mixins/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/mixins/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/mixins/monitor_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/mixins/profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/mixins/step_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/rl.py
--rw-r--r--   0 runner    (1001) docker     (123)    11397 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/trainers/sl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.480513 ml-starter-0.1.32/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/amp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/atomic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/augmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/caching.py
--rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/datetime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.484514 ml-starter-0.1.32/ml/utils/device/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/device/auto.py
--rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/device/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/device/cpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/device/gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/device/metal.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/large_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/meter.py
--rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/mixed_precision.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/networking.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/parallel.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/spectrogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/staging.py
--rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/testing.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/tokens.py
--rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/torch_distributed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.484514 ml-starter-0.1.32/ml/utils/triton/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/triton/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/triton/kmeans.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/triton/lion.py
--rw-r--r--   0 runner    (1001) docker     (123)    20942 2023-07-18 05:36:49.000000 ml-starter-0.1.32/ml/utils/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 05:37:01.484514 ml-starter-0.1.32/ml_starter.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-18 05:37:01.000000 ml-starter-0.1.32/ml_starter.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-18 05:37:01.000000 ml-starter-0.1.32/ml_starter.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 05:37:01.000000 ml-starter-0.1.32/ml_starter.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-18 05:37:01.000000 ml-starter-0.1.32/ml_starter.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-18 05:37:01.000000 ml-starter-0.1.32/ml_starter.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-18 05:36:49.000000 ml-starter-0.1.32/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 05:36:49.000000 ml-starter-0.1.32/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 05:36:49.000000 ml-starter-0.1.32/requirements-docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-18 05:36:49.000000 ml-starter-0.1.32/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-18 05:37:01.488514 ml-starter-0.1.32/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-18 05:36:49.000000 ml-starter-0.1.32/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.656810 ml-starter-0.1.33/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 06:20:45.000000 ml-starter-0.1.33/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-18 06:20:45.000000 ml-starter-0.1.33/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-18 06:20:58.656810 ml-starter-0.1.33/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-07-18 06:20:45.000000 ml-starter-0.1.33/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.612810 ml-starter-0.1.33/ml/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10585 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.612810 ml-starter-0.1.33/ml/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/core/common_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5582 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/core/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26629 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/core/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.616810 ml-starter-0.1.33/ml/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/launchers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/launchers/mp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10293 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/launchers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4184 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/launchers/torchrun.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.616810 ml-starter-0.1.33/ml/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/loggers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2910 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/loggers/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45793 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/loggers/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5216 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/loggers/stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13749 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/loggers/tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.620810 ml-starter-0.1.33/ml/lr_schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/lr_schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2168 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/lr_schedulers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/lr_schedulers/constant.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/lr_schedulers/cosine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2393 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/lr_schedulers/cosine_decay.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/lr_schedulers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/lr_schedulers/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/lr_schedulers/linear_no_decay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.620810 ml-starter-0.1.33/ml/lr_schedulers/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/lr_schedulers/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2269 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/lr_schedulers/scripts/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.624810 ml-starter-0.1.33/ml/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5761 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/models/activations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/models/codebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10750 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/models/diffusion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8934 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/models/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/models/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5168 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/models/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2812 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/models/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56014 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/models/lora.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/models/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12566 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/models/norms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16373 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/models/parallel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.628810 ml-starter-0.1.33/ml/optimizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/optimizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4277 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/optimizers/adam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3661 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/optimizers/adan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/optimizers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/optimizers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/optimizers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/optimizers/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/optimizers/sgd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/optimizers/shampoo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/optimizers/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.628810 ml-starter-0.1.33/ml/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3592 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/scripts/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/scripts/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/scripts/resolve.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/scripts/stage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/scripts/train.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.628810 ml-starter-0.1.33/ml/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19338 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.632810 ml-starter-0.1.33/ml/tasks/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/datasets/async_iterable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/datasets/clippify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7618 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/datasets/collate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10047 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/datasets/error_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/datasets/multi_iter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1588 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/datasets/samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/datasets/streaming.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6998 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/datasets/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/datasets/video_file.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.632810 ml-starter-0.1.33/ml/tasks/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1658 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/environments/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/environments/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13448 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/environments/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.632810 ml-starter-0.1.33/ml/tasks/gan/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/gan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/gan/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.636810 ml-starter-0.1.33/ml/tasks/losses/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5905 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/losses/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/losses/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7060 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/losses/loss.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.636810 ml-starter-0.1.33/ml/tasks/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18539 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/rl/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3826 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/rl/replay.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.636810 ml-starter-0.1.33/ml/tasks/sl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/sl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/tasks/sl/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.640810 ml-starter-0.1.33/ml/trainers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24021 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11607 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/gan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9168 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/learning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.640810 ml-starter-0.1.33/ml/trainers/mixins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/mixins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/mixins/compile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9418 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/mixins/cpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/mixins/data_parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/mixins/gpu_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/mixins/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6797 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/mixins/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/mixins/monitor_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/mixins/profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/mixins/step_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7914 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/rl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11397 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/trainers/sl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.652810 ml-starter-0.1.33/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4882 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/amp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3726 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3297 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/atomic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14832 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/augmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/caching.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8596 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2062 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5091 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/datetime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.652810 ml-starter-0.1.33/ml/utils/device/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/device/auto.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7832 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/device/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/device/cpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1911 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/device/gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/device/metal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1478 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/large_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4957 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/meter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4433 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/mixed_precision.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/networking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11253 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/parallel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16056 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/spectrogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/staging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6313 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/testing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13173 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/tokens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7921 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/torch_distributed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.656810 ml-starter-0.1.33/ml/utils/triton/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/triton/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1969 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/triton/kmeans.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/triton/lion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20942 2023-07-18 06:20:45.000000 ml-starter-0.1.33/ml/utils/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:20:58.656810 ml-starter-0.1.33/ml_starter.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-07-18 06:20:58.000000 ml-starter-0.1.33/ml_starter.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-07-18 06:20:58.000000 ml-starter-0.1.33/ml_starter.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:20:58.000000 ml-starter-0.1.33/ml_starter.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-18 06:20:58.000000 ml-starter-0.1.33/ml_starter.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-07-18 06:20:58.000000 ml-starter-0.1.33/ml_starter.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-18 06:20:45.000000 ml-starter-0.1.33/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 06:20:45.000000 ml-starter-0.1.33/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 06:20:45.000000 ml-starter-0.1.33/requirements-docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-18 06:20:45.000000 ml-starter-0.1.33/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-18 06:20:58.656810 ml-starter-0.1.33/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-18 06:20:45.000000 ml-starter-0.1.33/setup.py
```

### Comparing `ml-starter-0.1.32/LICENSE` & `ml-starter-0.1.33/LICENSE`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/PKG-INFO` & `ml-starter-0.1.33/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.32
+Version: 0.1.33
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.32/README.md` & `ml-starter-0.1.33/README.md`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/api.py` & `ml-starter-0.1.33/ml/api.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/core/common_types.py` & `ml-starter-0.1.33/ml/core/common_types.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/core/config.py` & `ml-starter-0.1.33/ml/core/config.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/core/env.py` & `ml-starter-0.1.33/ml/core/env.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/core/registry.py` & `ml-starter-0.1.33/ml/core/registry.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/core/state.py` & `ml-starter-0.1.33/ml/core/state.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/launchers/base.py` & `ml-starter-0.1.33/ml/launchers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/launchers/mp.py` & `ml-starter-0.1.33/ml/launchers/mp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/launchers/slurm.py` & `ml-starter-0.1.33/ml/launchers/slurm.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/launchers/torchrun.py` & `ml-starter-0.1.33/ml/launchers/torchrun.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/loggers/base.py` & `ml-starter-0.1.33/ml/loggers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/loggers/meter.py` & `ml-starter-0.1.33/ml/loggers/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/loggers/multi.py` & `ml-starter-0.1.33/ml/loggers/multi.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/loggers/stdout.py` & `ml-starter-0.1.33/ml/loggers/stdout.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/loggers/tensorboard.py` & `ml-starter-0.1.33/ml/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/lr_schedulers/base.py` & `ml-starter-0.1.33/ml/lr_schedulers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/lr_schedulers/constant.py` & `ml-starter-0.1.33/ml/lr_schedulers/constant.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/lr_schedulers/cosine.py` & `ml-starter-0.1.33/ml/lr_schedulers/cosine.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/lr_schedulers/cosine_decay.py` & `ml-starter-0.1.33/ml/lr_schedulers/cosine_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/lr_schedulers/gan.py` & `ml-starter-0.1.33/ml/lr_schedulers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/lr_schedulers/linear.py` & `ml-starter-0.1.33/ml/lr_schedulers/linear.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/lr_schedulers/linear_no_decay.py` & `ml-starter-0.1.33/ml/lr_schedulers/linear_no_decay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/lr_schedulers/scripts/plot.py` & `ml-starter-0.1.33/ml/lr_schedulers/scripts/plot.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/models/activations.py` & `ml-starter-0.1.33/ml/models/activations.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/models/base.py` & `ml-starter-0.1.33/ml/models/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/models/codebook.py` & `ml-starter-0.1.33/ml/models/codebook.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/models/diffusion.py` & `ml-starter-0.1.33/ml/models/diffusion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/models/embeddings.py` & `ml-starter-0.1.33/ml/models/embeddings.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/models/gan.py` & `ml-starter-0.1.33/ml/models/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/models/init.py` & `ml-starter-0.1.33/ml/models/init.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/models/kmeans.py` & `ml-starter-0.1.33/ml/models/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/models/lora.py` & `ml-starter-0.1.33/ml/models/lora.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/models/modules.py` & `ml-starter-0.1.33/ml/models/modules.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/models/norms.py` & `ml-starter-0.1.33/ml/models/norms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/models/parallel.py` & `ml-starter-0.1.33/ml/models/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/optimizers/adam.py` & `ml-starter-0.1.33/ml/optimizers/adam.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/optimizers/adan.py` & `ml-starter-0.1.33/ml/optimizers/adan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/optimizers/base.py` & `ml-starter-0.1.33/ml/optimizers/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/optimizers/common.py` & `ml-starter-0.1.33/ml/optimizers/common.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/optimizers/gan.py` & `ml-starter-0.1.33/ml/optimizers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/optimizers/lion.py` & `ml-starter-0.1.33/ml/optimizers/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/optimizers/sgd.py` & `ml-starter-0.1.33/ml/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/optimizers/shampoo.py` & `ml-starter-0.1.33/ml/optimizers/shampoo.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/scripts/cli.py` & `ml-starter-0.1.33/ml/scripts/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/scripts/stage.py` & `ml-starter-0.1.33/ml/scripts/stage.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/scripts/train.py` & `ml-starter-0.1.33/ml/scripts/train.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/base.py` & `ml-starter-0.1.33/ml/tasks/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/datasets/async_iterable.py` & `ml-starter-0.1.33/ml/tasks/datasets/async_iterable.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/datasets/clippify.py` & `ml-starter-0.1.33/ml/tasks/datasets/clippify.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/datasets/collate.py` & `ml-starter-0.1.33/ml/tasks/datasets/collate.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/datasets/error_handling.py` & `ml-starter-0.1.33/ml/tasks/datasets/error_handling.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/datasets/multi_iter.py` & `ml-starter-0.1.33/ml/tasks/datasets/multi_iter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/datasets/samplers.py` & `ml-starter-0.1.33/ml/tasks/datasets/samplers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/datasets/streaming.py` & `ml-starter-0.1.33/ml/tasks/datasets/streaming.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/datasets/transforms.py` & `ml-starter-0.1.33/ml/tasks/datasets/transforms.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/datasets/video_file.py` & `ml-starter-0.1.33/ml/tasks/datasets/video_file.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/environments/base.py` & `ml-starter-0.1.33/ml/tasks/environments/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/environments/utils.py` & `ml-starter-0.1.33/ml/tasks/environments/utils.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/environments/worker.py` & `ml-starter-0.1.33/ml/tasks/environments/worker.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/gan/base.py` & `ml-starter-0.1.33/ml/tasks/gan/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/losses/audio.py` & `ml-starter-0.1.33/ml/tasks/losses/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/losses/image.py` & `ml-starter-0.1.33/ml/tasks/losses/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/losses/loss.py` & `ml-starter-0.1.33/ml/tasks/losses/loss.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/rl/base.py` & `ml-starter-0.1.33/ml/tasks/rl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/rl/replay.py` & `ml-starter-0.1.33/ml/tasks/rl/replay.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/tasks/sl/base.py` & `ml-starter-0.1.33/ml/tasks/sl/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/trainers/base.py` & `ml-starter-0.1.33/ml/trainers/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from pickle import UnpicklingError
 from typing import Any, Callable, Generic, Literal, TypeVar, cast, get_args
 
 import torch
 from omegaconf import II, MISSING, DictConfig, ListConfig, OmegaConf
 from torch import Tensor
 from torch.optim.optimizer import Optimizer
+from torch.serialization import MAP_LOCATION
 
 from ml.core.config import BaseConfig, BaseObject, conf_field
 from ml.core.env import get_ml_config_path
 from ml.core.state import State
 from ml.loggers.base import BaseLogger
 from ml.loggers.multi import MultiLogger
 from ml.lr_schedulers.base import BaseLRScheduler, SchedulerAdapter
@@ -326,39 +327,48 @@
         ckpt: str | Path | dict,
         task: TaskT,
         model: ModelT,
         optims: Optimizer | dict[str, Optimizer] | None = None,
         lr_scheds: SchedulerAdapter | dict[str, SchedulerAdapter] | None = None,
         *,
         weights_only: bool = True,
+        map_location: MAP_LOCATION = None,
     ) -> State:
         """Loads a given checkpoint, from a path or dictionary.
 
         Args:
             ckpt: The checkpoint to load.
             task: The task to load the checkpoint into.
             model: The model to load the checkpoint into.
             optims: The optimizer to load the checkpoint into.
             lr_scheds: The learning rate scheduler to load the checkpoint into.
             weights_only: If set, only load the model weights.
+            map_location: The location to map the loaded checkpoint to.
 
         Returns:
             The state loaded from the checkpoint.
 
         Raises:
             UnpicklingError: If there is some issue unpickling the checkpoint.
         """
         with Timer("loading checkpoint", spinner=True):
             if isinstance(ckpt, (str, Path)):
                 try:
-                    ckpt = cast(dict, torch.load(ckpt, weights_only=weights_only))
+                    ckpt = cast(dict, torch.load(ckpt, weights_only=weights_only, map_location=map_location))
                 except UnpicklingError:
                     if weights_only:
                         logger.warning("Failed to load checkpoint using `weights_only` flag, retrying without it")
-                        ckpt = cast(dict, torch.load(cast(str | Path, ckpt), weights_only=False))
+                        ckpt = cast(
+                            dict,
+                            torch.load(
+                                cast(str | Path, ckpt),
+                                weights_only=False,
+                                map_location=map_location,
+                            ),
+                        )
                     else:
                         raise
 
             def try_load_state_dict(model: ModelT, state_dict: dict[str, Any]) -> bool:
                 try:
                     model.load_state_dict(state_dict)
                     return True
```

### Comparing `ml-starter-0.1.32/ml/trainers/gan.py` & `ml-starter-0.1.33/ml/trainers/gan.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/trainers/learning.py` & `ml-starter-0.1.33/ml/trainers/learning.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/trainers/mixins/compile.py` & `ml-starter-0.1.33/ml/trainers/mixins/compile.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/trainers/mixins/cpu_stats.py` & `ml-starter-0.1.33/ml/trainers/mixins/cpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/trainers/mixins/data_parallel.py` & `ml-starter-0.1.33/ml/trainers/mixins/data_parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/trainers/mixins/gpu_stats.py` & `ml-starter-0.1.33/ml/trainers/mixins/gpu_stats.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/trainers/mixins/heartbeat.py` & `ml-starter-0.1.33/ml/trainers/mixins/heartbeat.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/trainers/mixins/mixed_precision.py` & `ml-starter-0.1.33/ml/trainers/mixins/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/trainers/mixins/monitor_process.py` & `ml-starter-0.1.33/ml/trainers/mixins/monitor_process.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/trainers/mixins/profiler.py` & `ml-starter-0.1.33/ml/trainers/mixins/profiler.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/trainers/mixins/step_wrapper.py` & `ml-starter-0.1.33/ml/trainers/mixins/step_wrapper.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/trainers/rl.py` & `ml-starter-0.1.33/ml/trainers/rl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/trainers/sl.py` & `ml-starter-0.1.33/ml/trainers/sl.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/amp.py` & `ml-starter-0.1.33/ml/utils/amp.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/argparse.py` & `ml-starter-0.1.33/ml/utils/argparse.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/atomic.py` & `ml-starter-0.1.33/ml/utils/atomic.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/attention.py` & `ml-starter-0.1.33/ml/utils/attention.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/audio.py` & `ml-starter-0.1.33/ml/utils/audio.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/augmentation.py` & `ml-starter-0.1.33/ml/utils/augmentation.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/caching.py` & `ml-starter-0.1.33/ml/utils/caching.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/checkpoint.py` & `ml-starter-0.1.33/ml/utils/checkpoint.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/cli.py` & `ml-starter-0.1.33/ml/utils/cli.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/colors.py` & `ml-starter-0.1.33/ml/utils/colors.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/containers.py` & `ml-starter-0.1.33/ml/utils/containers.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/data.py` & `ml-starter-0.1.33/ml/utils/data.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/datetime.py` & `ml-starter-0.1.33/ml/utils/datetime.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/device/auto.py` & `ml-starter-0.1.33/ml/utils/device/auto.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/device/base.py` & `ml-starter-0.1.33/ml/utils/device/base.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/device/cpu.py` & `ml-starter-0.1.33/ml/utils/device/cpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/device/gpu.py` & `ml-starter-0.1.33/ml/utils/device/gpu.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/device/metal.py` & `ml-starter-0.1.33/ml/utils/device/metal.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/distributed.py` & `ml-starter-0.1.33/ml/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/exceptions.py` & `ml-starter-0.1.33/ml/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/image.py` & `ml-starter-0.1.33/ml/utils/image.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/io.py` & `ml-starter-0.1.33/ml/utils/io.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/large_models.py` & `ml-starter-0.1.33/ml/utils/large_models.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/logging.py` & `ml-starter-0.1.33/ml/utils/logging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/meter.py` & `ml-starter-0.1.33/ml/utils/meter.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/mixed_precision.py` & `ml-starter-0.1.33/ml/utils/mixed_precision.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/networking.py` & `ml-starter-0.1.33/ml/utils/networking.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/numpy.py` & `ml-starter-0.1.33/ml/utils/numpy.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/parallel.py` & `ml-starter-0.1.33/ml/utils/parallel.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/spectrogram.py` & `ml-starter-0.1.33/ml/utils/spectrogram.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/staging.py` & `ml-starter-0.1.33/ml/utils/staging.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/testing.py` & `ml-starter-0.1.33/ml/utils/testing.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/timer.py` & `ml-starter-0.1.33/ml/utils/timer.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/tokens.py` & `ml-starter-0.1.33/ml/utils/tokens.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/torch_distributed.py` & `ml-starter-0.1.33/ml/utils/torch_distributed.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/triton/kmeans.py` & `ml-starter-0.1.33/ml/utils/triton/kmeans.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/triton/lion.py` & `ml-starter-0.1.33/ml/utils/triton/lion.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml/utils/video.py` & `ml-starter-0.1.33/ml/utils/video.py`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/ml_starter.egg-info/PKG-INFO` & `ml-starter-0.1.33/ml_starter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ml-starter
-Version: 0.1.32
+Version: 0.1.33
 Summary: ML project template repository
 Home-page: https://github.com/codekansas/ml-starter
 Author: Benjamin Bolte
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ml-starter-0.1.32/ml_starter.egg-info/SOURCES.txt` & `ml-starter-0.1.33/ml_starter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/pyproject.toml` & `ml-starter-0.1.33/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ml-starter-0.1.32/setup.py` & `ml-starter-0.1.33/setup.py`

 * *Files identical despite different names*

