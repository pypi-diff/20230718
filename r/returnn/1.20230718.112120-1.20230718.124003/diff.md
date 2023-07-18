# Comparing `tmp/returnn-1.20230718.112120.tar.gz` & `tmp/returnn-1.20230718.124003.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/returnn-1.20230718.112120.tar", last modified: Tue Jul 18 11:34:28 2023, max compression
+gzip compressed data, was "dist/returnn-1.20230718.124003.tar", last modified: Tue Jul 18 12:56:37 2023, max compression
```

## Comparing `returnn-1.20230718.112120.tar` & `returnn-1.20230718.124003.tar`

### file list

```diff
@@ -1,450 +1,450 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/.kateconfig
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/_setup_info_generated.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/demos/
--rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/12AX.cluster_map
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-fwd.config
--rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-horovod-mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-horovod-mpi.py.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-horovod-mpi.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-hyper-param-tuning.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-iter-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-list-devices.py
--rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-lua-torch-layer.config
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-pretrain.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-record-and-push-to-webserver.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-rf.config
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-rhn-enwik8.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-sprint-interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-att-copy.config
--rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-attention.config
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-chunking-blstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-contribrnn-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-enc-dec.config
--rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-hard-att-copy.config
--rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-lstm-benchmark.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-maxgradnorm-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-native-lstm-lowmem.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-native-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-native-lstm2.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-native-lstm2.12ax.tuned.config
--rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-neural-transducer.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-rec-explicit-lstm.config
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-rec-explicit-rnn.config
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-rec-self-att.config
--rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-search-compiled-graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-tf-vanilla-lstm.12ax.config
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-timit-lstm-ctc.config
--rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-torch.config
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo-upd-mult-model.lstm.12ax.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/demo.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/demos/mdlstm/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/IAM_lines/
--rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
--rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/README.txt
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/chars.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/config_demo
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/config_fwd
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/config_real
--rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/create_IAM_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/decode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/features/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/features/raw/
--rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/features/raw/demo.h5
--rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/lines.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/split/
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/split/eval.txt
--rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/split/train.txt
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/IAM/split/valid.txt
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/demos/mdlstm/artificial/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/artificial/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/artificial/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/artificial/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/artificial/trainconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/demos/mdlstm/artificial_rgb/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/artificial_rgb/create_test_h5.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/artificial_rgb/forwardconfig
--rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/artificial_rgb/go.sh
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/demos/mdlstm/artificial_rgb/trainconfig
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/
--rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/__old_mod_loader__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/__setup__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/audio.py
--rw-r--r--   0 runner    (1001) docker     (123)    63188 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/bundle_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/cached.py
--rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/cached2.py
--rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/generating.py
--rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/hdf.py
--rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/lm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/map.py
--rw-r--r--   0 runner    (1001) docker     (123)    76099 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/multi_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/normalization_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/numpy_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/raw_wav.py
--rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/stereo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/datasets/util/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/util/feature_extraction.py
--rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/datasets/util/vocabulary.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/engine/
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/engine/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/engine/batch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/extern/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-18 11:34:05.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/.git
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/aligner.gif
--rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/check.png
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/core.h
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
--rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/ref_rna.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
--rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
--rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-18 11:34:08.000000 returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/test.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/extern/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/extern/graph_editor/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/extern/graph_editor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/extern/graph_editor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/extern/graph_editor/edit.py
--rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/extern/graph_editor/reroute.py
--rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/extern/graph_editor/select.py
--rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/extern/graph_editor/subgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/extern/graph_editor/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/extern/graph_editor/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/forward_iface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40460 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/_numpy_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    21015 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/array_.py
--rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/container.py
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/dropout.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/dtype.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/frontend/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/encoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/encoder/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/encoder/conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/linear.py
--rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/math_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/matmul.py
--rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/module.py
--rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/parameter.py
--rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/run_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/tensor_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/frontend/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/import_/
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/import_/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/import_/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/import_/git.py
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/import_/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/learning_rate_control.py
--rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/log.py
--rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/native_op.cpp
--rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/pretrain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/sprint/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/sprint/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/sprint/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/sprint/control.py
--rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/sprint/error_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/sprint/extern_interface.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/sprint/interface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/tensor/
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tensor/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tensor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   100183 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tensor/_dim_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)   158177 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tensor/_tensor_extra.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tensor/_tensor_mixin_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tensor/_tensor_op_overloads.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tensor/control_flow_ctx.py
--rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tensor/dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tensor/marked_dim.py
--rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tensor/tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tensor/tensor_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tensor/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/tf/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/compat.py
--rw-r--r--   0 runner    (1001) docker     (123)    36646 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/data_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)   146879 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/tf/frontend_layers/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/frontend_layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40440 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/frontend_layers/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/frontend_layers/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/frontend_layers/cond.py
--rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/frontend_layers/config_entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/frontend_layers/debug_eager_mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/frontend_layers/dims.py
--rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/frontend_layers/layer.py
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/frontend_layers/make_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/frontend_layers/parameter_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/frontend_layers/prev_tensor_ref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/tf/frontend_low_level/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/frontend_low_level/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/frontend_low_level/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/horovod.py
--rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/hyper_param_tuning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/tf/layers/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   151302 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/layers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)   586746 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/layers/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)   544225 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/layers/rec.py
--rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/layers/segmental_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/layers/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/layers/variable.py
--rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/native_op.py
--rw-r--r--   0 runner    (1001) docker     (123)   224089 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/sprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    71539 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/tf/util/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   302119 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/util/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/util/gradient_checkpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/util/ken_lm.py
--rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/tf/util/open_fst.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/torch/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/torch/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/torch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/torch/data/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/torch/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/torch/data/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/torch/data/returnn_dataset_wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/torch/data/tensor_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/torch/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)    36812 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/torch/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/torch/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/torch/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    73187 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/torch/frontend/_backend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/torch/frontend/_rand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/torch/frontend/bridge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/torch/functional/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/torch/functional/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/torch/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/torch/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn/util/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   144901 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/util/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/util/better_exchook.py
--rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/util/bpe.py
--rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/util/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/util/debug_helpers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/util/fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/util/literal_py_to_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/util/pprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/util/py-to-pickle.cpp
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/util/py_compat.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/util/sig_proc.py
--rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/returnn/util/task_system.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/returnn.egg-info/top_level.txt
--rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/tests/
--rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/DummySprintExec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/PyCharm-inspection-profile.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/tests/PyCharm.idea/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/PyCharm.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/PyCharm.idea/.name
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/PyCharm.idea/codeStyleSettings.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/tests/PyCharm.idea/codeStyles/
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/PyCharm.idea/codeStyles/Project.xml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/tests/PyCharm.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/PyCharm.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/PyCharm.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/PyCharm.idea/returnn.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/tests/PyCharm.idea/scopes/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/PyCharm.idea/scopes/scope_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/_set_num_threads1.py
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/_setup_returnn_env.py
--rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/_setup_test_env.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/bpe-unicode-demo.codes
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/bpe-unicode-demo.vocab
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/lexicon_opt.fst
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/lexicon_opt.isyms
--rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/lexicon_opt.jpg
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/lexicon_opt.osyms
--rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/lint_common.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/pycharm-inspect.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/pylint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/returnn-as-framework.py
--rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/rf_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/spelling.dic
--rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_Dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_Fsa.py
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_GeneratingDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_HDFDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_LearningRateControl.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_Log.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_MultiProcDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_PTDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_Pretrain.py
--rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_SprintDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_SprintInterface.py
--rw-r--r--   0 runner    (1001) docker     (123)   238033 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_TFEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_TFNativeOp.py
--rw-r--r--   0 runner    (1001) docker     (123)   555550 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_TFNetworkLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)   580572 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_TFNetworkRecLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_TFNetworkSigProcLayer.py
--rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_TFUpdater.py
--rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_TFUtil.py
--rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_TF_determinism.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_TaskSystem.py
--rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_TaskSystem_SharedMem.py
--rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_TranslationDataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_Util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_demos.py
--rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_fork_exec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_hdf_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_rf_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_rf_attention.py
--rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_rf_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_rf_cond.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_rf_const.py
--rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_rf_container.py
--rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_rf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_rf_encoder_conformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_rf_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_rf_math.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_rf_normalization.py
--rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_rf_rec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_rf_reduce.py
--rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_rf_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_tensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_torch_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_torch_frontend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tests/test_torch_internal_frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/_setup_returnn_env.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/analyze-dataset-batches.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/bliss-collect-seq-lens.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/bliss-dump-text.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/bliss-get-segment-names.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    18501 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/bliss-to-ogg-zip.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/bpe-create-lexicon.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/calculate-word-error-rate.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/cleanup-old-models.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/collect-orth-symbols.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/collect-words.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/compile_native_op.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/compile_tf_graph.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/debug-dump-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/debug-plot-search-scores.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/dump-dataset-raw-strings.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/dump-dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/dump-forward-stats.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/dump-forward.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/dump-network-json.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/dump-pickle.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/extract_state_tying_from_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/get-attention-weights.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/get-best-model-epoch.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/hdf_dump.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/hdf_dump_translation_dataset.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/import-blocks-mt-model.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/import-t2t-mt-model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/tools/lattice_rescorer/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/tools/lattice_rescorer/example/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/example/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/example/libs_list
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:34:28.000000 returnn-1.20230718.112120/tools/lattice_rescorer/example/network.040/
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
--rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/example/rescore_lattice.sh
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/example/state_vars_list
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/example/tensor_names_list
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/file.h
--rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/htklatticerescorer.cc
--rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/htklatticerescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/main.cc
--rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/rescorer.h
--rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/vocabulary.cc
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/lattice_rescorer/vocabulary.h
--rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/tf_avg_checkpoints.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/tf_inspect_checkpoint.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/tf_inspect_summary_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-18 11:34:04.000000 returnn-1.20230718.112120/tools/torch_export_to_onnx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/.kateconfig
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10244 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3573 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/_setup_info_generated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/demos/
+-rw-r--r--   0 runner    (1001) docker     (123)    36006 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/12AX.cluster_map
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-fwd.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2703 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-horovod-mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-horovod-mpi.py.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      264 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-horovod-mpi.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-hyper-param-tuning.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2396 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-iter-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3635 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-list-devices.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2848 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-lua-torch-layer.config
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-pretrain.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2331 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-record-and-push-to-webserver.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1950 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3136 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-rf.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-rhn-enwik8.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1378 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-sprint-interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-att-copy.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2428 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-attention.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-chunking-blstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-contribrnn-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-enc-dec.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)    11615 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-hard-att-copy.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7287 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-lstm-benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-maxgradnorm-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-native-lstm-lowmem.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-native-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-native-lstm2.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-native-lstm2.12ax.tuned.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1794 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-neural-transducer.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1825 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-rec-explicit-lstm.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-rec-explicit-rnn.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-rec-self-att.config
+-rw-r--r--   0 runner    (1001) docker     (123)     5188 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-search-compiled-graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-tf-vanilla-lstm.12ax.config
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-timit-lstm-ctc.config
+-rw-r--r--   0 runner    (1001) docker     (123)     2975 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-torch.config
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo-upd-mult-model.lstm.12ax.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      651 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/demo.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/demos/mdlstm/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/IAM_lines/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43239 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    43552 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/IAM_lines/a01-007-04.png
+-rwxr-xr-x   0 runner    (1001) docker     (123)    45111 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/IAM_lines/a01-007-06.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/chars.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1896 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/config_demo
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/config_fwd
+-rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/config_real
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10194 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/create_IAM_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      749 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/decode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/features/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/features/raw/
+-rw-r--r--   0 runner    (1001) docker     (123)   248580 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/features/raw/demo.h5
+-rwxr-xr-x   0 runner    (1001) docker     (123)       86 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/lines.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/split/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/split/eval.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    69536 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/split/train.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/IAM/split/valid.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/demos/mdlstm/artificial/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2804 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/artificial/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/artificial/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/artificial/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/artificial/trainconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/demos/mdlstm/artificial_rgb/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2966 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/artificial_rgb/create_test_h5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/artificial_rgb/forwardconfig
+-rwxr-xr-x   0 runner    (1001) docker     (123)      105 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/artificial_rgb/go.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/demos/mdlstm/artificial_rgb/trainconfig
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/
+-rw-r--r--   0 runner    (1001) docker     (123)     1012 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25926 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6981 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/__old_mod_loader__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/__setup__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24267 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18032 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/audio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63188 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/bundle_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24892 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/cached.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11658 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/cached2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94213 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/generating.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65113 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/hdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    85120 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9065 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/map.py
+-rw-r--r--   0 runner    (1001) docker     (123)    76099 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11167 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/multi_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14596 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/normalization_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5291 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/numpy_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9127 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/raw_wav.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56015 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17608 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/stereo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/datasets/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23915 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/util/feature_extraction.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20445 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/datasets/util/vocabulary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15421 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/engine/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/engine/batch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/extern/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-18 12:56:20.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/.git
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13770 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/aligner.gif
+-rw-r--r--   0 runner    (1001) docker     (123)    51077 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/check.png
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/core_cpu.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2089 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)    11544 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6961 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/ref_rna.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/tensorflow_binding/
+-rw-r--r--   0 runner    (1001) docker     (123)     6150 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/
+-rw-r--r--   0 runner    (1001) docker     (123)     1693 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-07-18 12:56:22.000000 returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/test.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/extern/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/extern/graph_editor/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/extern/graph_editor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/extern/graph_editor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/extern/graph_editor/edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19826 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/extern/graph_editor/reroute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29772 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/extern/graph_editor/select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26578 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/extern/graph_editor/subgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30380 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/extern/graph_editor/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18727 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/extern/graph_editor/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/forward_iface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40460 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5359 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/_numpy_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21015 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/array_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20878 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6015 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22357 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3538 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/dropout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/dtype.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/frontend/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/encoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/encoder/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15428 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/encoder/conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5855 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2186 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15485 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/math_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1945 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/matmul.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9877 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9687 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/parameter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11035 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7528 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7225 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17654 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/run_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4530 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/tensor_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/frontend/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/import_/
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/import_/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8148 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/import_/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13961 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/import_/git.py
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/import_/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33063 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/learning_rate_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12235 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35760 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/native_op.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)   244393 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23542 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/pretrain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/sprint/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/sprint/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31545 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/sprint/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31137 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/sprint/control.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23313 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/sprint/error_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12305 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/sprint/extern_interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/sprint/interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/tensor/
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tensor/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tensor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100493 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tensor/_dim_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)   158177 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tensor/_tensor_extra.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tensor/_tensor_mixin_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4890 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tensor/_tensor_op_overloads.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tensor/control_flow_ctx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3884 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tensor/dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tensor/marked_dim.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7680 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tensor/tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tensor/tensor_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4532 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tensor/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/tf/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36646 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/data_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15108 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)   146879 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/tf/frontend_layers/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/frontend_layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40440 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/frontend_layers/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/frontend_layers/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/frontend_layers/cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4480 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/frontend_layers/config_entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/frontend_layers/debug_eager_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5712 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/frontend_layers/dims.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71987 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/frontend_layers/layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/frontend_layers/make_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/frontend_layers/parameter_assign.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/frontend_layers/prev_tensor_ref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/tf/frontend_low_level/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/frontend_low_level/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20349 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/frontend_low_level/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5404 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/horovod.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31611 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/hyper_param_tuning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/tf/layers/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151302 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/layers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)   586746 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/layers/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)   544225 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/layers/rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21515 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/layers/segmental_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52409 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/layers/signal_processing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11446 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/layers/variable.py
+-rw-r--r--   0 runner    (1001) docker     (123)    79733 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/native_op.py
+-rw-r--r--   0 runner    (1001) docker     (123)   224089 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5471 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/sprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71539 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/tf/util/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   302119 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28839 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/util/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6076 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/util/gradient_checkpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17333 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/util/ken_lm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11277 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/tf/util/open_fst.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/torch/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/torch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/torch/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/torch/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12294 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/torch/data/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5502 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/torch/data/returnn_dataset_wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1340 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/torch/data/tensor_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6338 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/torch/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37372 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/torch/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/torch/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/torch/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    73187 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/torch/frontend/_backend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/torch/frontend/_rand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/torch/frontend/bridge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/torch/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/torch/functional/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/torch/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12700 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/torch/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn/util/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   144901 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/util/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/util/better_exchook.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17977 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/util/bpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15987 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/util/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2905 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/util/debug_helpers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    59177 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/util/fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/util/literal_py_to_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8131 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/util/pprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14846 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/util/py-to-pickle.cpp
+-rw-r--r--   0 runner    (1001) docker     (123)      277 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/util/py_compat.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7273 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/util/sig_proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27230 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/returnn/util/task_system.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12544 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/returnn.egg-info/top_level.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)      461 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3392 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/DummySprintExec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/PyCharm-inspection-profile.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/tests/PyCharm.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/PyCharm.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/PyCharm.idea/.name
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/PyCharm.idea/codeStyleSettings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/tests/PyCharm.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/PyCharm.idea/codeStyles/Project.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/PyCharm.idea/codeStyles/codeStyleConfig.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/tests/PyCharm.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)     2743 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/PyCharm.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/PyCharm.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/PyCharm.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/PyCharm.idea/returnn.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/tests/PyCharm.idea/scopes/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/PyCharm.idea/scopes/scope_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/_set_num_threads1.py
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/_setup_returnn_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9271 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/_setup_test_env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/bpe-unicode-demo.codes
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/bpe-unicode-demo.vocab
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/lexicon_opt.fst
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/lexicon_opt.isyms
+-rw-r--r--   0 runner    (1001) docker     (123)    34282 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/lexicon_opt.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/lexicon_opt.osyms
+-rw-r--r--   0 runner    (1001) docker     (123)     6880 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/lint_common.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29203 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/pycharm-inspect.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2960 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/returnn-as-framework.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9228 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/rf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/spelling.dic
+-rw-r--r--   0 runner    (1001) docker     (123)     7845 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_Dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13634 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_Fsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_GeneratingDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32796 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_HDFDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10326 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_LearningRateControl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_Log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_MultiProcDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3333 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_PTDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_Pretrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21403 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5014 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_SprintDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_SprintInterface.py
+-rw-r--r--   0 runner    (1001) docker     (123)   238033 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_TFEngine.py
+-rw-r--r--   0 runner    (1001) docker     (123)   135453 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_TFNativeOp.py
+-rw-r--r--   0 runner    (1001) docker     (123)   555550 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_TFNetworkLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)   580572 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_TFNetworkRecLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14485 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_TFNetworkSigProcLayer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20312 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_TFUpdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)   188146 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_TFUtil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3082 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_TF_determinism.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_TaskSystem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5088 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_TaskSystem_SharedMem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9378 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_TranslationDataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14944 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_Util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11304 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_demos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7375 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_fork_exec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2893 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_hdf_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9868 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_rf_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_rf_attention.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8107 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_rf_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9490 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_rf_cond.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_rf_const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4591 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_rf_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11673 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_rf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_rf_encoder_conformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_rf_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_rf_math.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_rf_normalization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15470 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_rf_rec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_rf_reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1052 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_rf_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_tensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8435 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3122 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_torch_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15594 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_torch_frontend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15534 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tests/test_torch_internal_frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/_setup_returnn_env.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9650 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/analyze-dataset-batches.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3943 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/bliss-collect-seq-lens.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      780 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/bliss-dump-text.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6608 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/bliss-get-segment-names.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    18501 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/bliss-to-ogg-zip.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5644 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/bpe-create-lexicon.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10532 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/calculate-word-error-rate.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1759 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/cleanup-old-models.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10783 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/collect-orth-symbols.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6801 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/collect-words.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4395 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/compile_native_op.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    81620 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/compile_tf_graph.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8500 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/debug-dump-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    47001 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/debug-plot-search-scores.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6048 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/dump-dataset-raw-strings.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12524 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/dump-dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5770 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/dump-forward-stats.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2576 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/dump-forward.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1596 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/dump-network-json.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      719 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/dump-pickle.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    16425 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/extract_state_tying_from_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14986 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/get-attention-weights.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2936 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/get-best-model-epoch.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3900 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/hdf_dump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19622 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/hdf_dump_translation_dataset.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    49563 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/import-blocks-mt-model.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    31498 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/import-t2t-mt-model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/tools/lattice_rescorer/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     7825 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/tools/lattice_rescorer/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/example/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/example/libs_list
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 12:56:37.000000 returnn-1.20230718.124003/tools/lattice_rescorer/example/network.040/
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config
+-rwxr-xr-x   0 runner    (1001) docker     (123)      800 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/example/rescore_lattice.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/example/state_vars_list
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/example/tensor_names_list
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/file.h
+-rw-r--r--   0 runner    (1001) docker     (123)    26055 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/htklatticerescorer.cc
+-rw-r--r--   0 runner    (1001) docker     (123)    10856 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/htklatticerescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12488 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/main.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     2184 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/rescorer.h
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/vocabulary.cc
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/lattice_rescorer/vocabulary.h
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5438 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/tf_avg_checkpoints.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6269 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/tf_inspect_checkpoint.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1288 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/tf_inspect_summary_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8947 2023-07-18 12:56:19.000000 returnn-1.20230718.124003/tools/torch_export_to_onnx.py
```

### Comparing `returnn-1.20230718.112120/.gitignore` & `returnn-1.20230718.124003/.gitignore`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/.gitmodules` & `returnn-1.20230718.124003/.gitmodules`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/CHANGELOG.md` & `returnn-1.20230718.124003/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/CODEOWNERS` & `returnn-1.20230718.124003/CODEOWNERS`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/CONTRIBUTING.md` & `returnn-1.20230718.124003/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/LICENSE` & `returnn-1.20230718.124003/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/MANIFEST.in` & `returnn-1.20230718.124003/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/PKG-INFO` & `returnn-1.20230718.124003/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230718.112120
+Version: 1.20230718.124003
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230718.112120/README.rst` & `returnn-1.20230718.124003/README.rst`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/__init__.py` & `returnn-1.20230718.124003/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/12AX.cluster_map` & `returnn-1.20230718.124003/demos/12AX.cluster_map`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-fwd.config` & `returnn-1.20230718.124003/demos/demo-fwd.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-horovod-mpi.py` & `returnn-1.20230718.124003/demos/demo-horovod-mpi.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-horovod-mpi.py.sh` & `returnn-1.20230718.124003/demos/demo-horovod-mpi.py.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-hyper-param-tuning.config` & `returnn-1.20230718.124003/demos/demo-hyper-param-tuning.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-iter-dataset.py` & `returnn-1.20230718.124003/demos/demo-iter-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-list-devices.py` & `returnn-1.20230718.124003/demos/demo-list-devices.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-lua-torch-layer.config` & `returnn-1.20230718.124003/demos/demo-lua-torch-layer.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-record-and-push-to-webserver.py` & `returnn-1.20230718.124003/demos/demo-record-and-push-to-webserver.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-returnn-as-framework.py` & `returnn-1.20230718.124003/demos/demo-returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-rf.config` & `returnn-1.20230718.124003/demos/demo-rf.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-rhn-enwik8.config` & `returnn-1.20230718.124003/demos/demo-rhn-enwik8.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-sprint-interface.py` & `returnn-1.20230718.124003/demos/demo-sprint-interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-att-copy.config` & `returnn-1.20230718.124003/demos/demo-tf-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-attention.config` & `returnn-1.20230718.124003/demos/demo-tf-attention.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-chunking-blstm.12ax.config` & `returnn-1.20230718.124003/demos/demo-tf-chunking-blstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-contribrnn-lstm.12ax.config` & `returnn-1.20230718.124003/demos/demo-tf-contribrnn-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-enc-dec.config` & `returnn-1.20230718.124003/demos/demo-tf-enc-dec.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-hard-att-copy.config` & `returnn-1.20230718.124003/demos/demo-tf-hard-att-copy.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-lstm-benchmark.py` & `returnn-1.20230718.124003/demos/demo-tf-lstm-benchmark.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-maxgradnorm-lstm.12ax.config` & `returnn-1.20230718.124003/demos/demo-tf-maxgradnorm-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-native-lstm-lowmem.12ax.config` & `returnn-1.20230718.124003/demos/demo-tf-native-lstm-lowmem.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-native-lstm.12ax.config` & `returnn-1.20230718.124003/demos/demo-tf-native-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-native-lstm2.12ax.config` & `returnn-1.20230718.124003/demos/demo-tf-native-lstm2.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-native-lstm2.12ax.tuned.config` & `returnn-1.20230718.124003/demos/demo-tf-native-lstm2.12ax.tuned.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-neural-transducer.12ax.config` & `returnn-1.20230718.124003/demos/demo-tf-neural-transducer.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-rec-explicit-lstm.config` & `returnn-1.20230718.124003/demos/demo-tf-rec-explicit-lstm.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-rec-explicit-rnn.config` & `returnn-1.20230718.124003/demos/demo-tf-rec-explicit-rnn.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-rec-self-att.config` & `returnn-1.20230718.124003/demos/demo-tf-rec-self-att.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-search-compiled-graph.py` & `returnn-1.20230718.124003/demos/demo-tf-search-compiled-graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-tf-vanilla-lstm.12ax.config` & `returnn-1.20230718.124003/demos/demo-tf-vanilla-lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-timit-lstm-ctc.config` & `returnn-1.20230718.124003/demos/demo-timit-lstm-ctc.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-torch.config` & `returnn-1.20230718.124003/demos/demo-torch.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo-upd-mult-model.lstm.12ax.config` & `returnn-1.20230718.124003/demos/demo-upd-mult-model.lstm.12ax.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/demo.sh` & `returnn-1.20230718.124003/demos/demo.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png` & `returnn-1.20230718.124003/demos/mdlstm/IAM/IAM_lines/a01-000u-00.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/IAM/IAM_lines/a01-007-04.png` & `returnn-1.20230718.124003/demos/mdlstm/IAM/IAM_lines/a01-007-04.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/IAM/IAM_lines/a01-007-06.png` & `returnn-1.20230718.124003/demos/mdlstm/IAM/IAM_lines/a01-007-06.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/IAM/README.txt` & `returnn-1.20230718.124003/demos/mdlstm/IAM/README.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/IAM/config_demo` & `returnn-1.20230718.124003/demos/mdlstm/IAM/config_demo`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/IAM/config_fwd` & `returnn-1.20230718.124003/demos/mdlstm/IAM/config_fwd`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/IAM/config_real` & `returnn-1.20230718.124003/demos/mdlstm/IAM/config_real`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/IAM/create_IAM_dataset.py` & `returnn-1.20230718.124003/demos/mdlstm/IAM/create_IAM_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/IAM/decode.py` & `returnn-1.20230718.124003/demos/mdlstm/IAM/decode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/IAM/features/raw/demo.h5` & `returnn-1.20230718.124003/demos/mdlstm/IAM/features/raw/demo.h5`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/IAM/split/eval.txt` & `returnn-1.20230718.124003/demos/mdlstm/IAM/split/eval.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/IAM/split/train.txt` & `returnn-1.20230718.124003/demos/mdlstm/IAM/split/train.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/IAM/split/valid.txt` & `returnn-1.20230718.124003/demos/mdlstm/IAM/split/valid.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/artificial/create_test_h5.py` & `returnn-1.20230718.124003/demos/mdlstm/artificial/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/artificial/forwardconfig` & `returnn-1.20230718.124003/demos/mdlstm/artificial/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/artificial/trainconfig` & `returnn-1.20230718.124003/demos/mdlstm/artificial/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/artificial_rgb/create_test_h5.py` & `returnn-1.20230718.124003/demos/mdlstm/artificial_rgb/create_test_h5.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/artificial_rgb/forwardconfig` & `returnn-1.20230718.124003/demos/mdlstm/artificial_rgb/forwardconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/demos/mdlstm/artificial_rgb/trainconfig` & `returnn-1.20230718.124003/demos/mdlstm/artificial_rgb/trainconfig`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/__init__.py` & `returnn-1.20230718.124003/returnn/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/__main__.py` & `returnn-1.20230718.124003/returnn/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/__old_mod_loader__.py` & `returnn-1.20230718.124003/returnn/__old_mod_loader__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/__setup__.py` & `returnn-1.20230718.124003/returnn/__setup__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/config.py` & `returnn-1.20230718.124003/returnn/config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/audio.py` & `returnn-1.20230718.124003/returnn/datasets/audio.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/basic.py` & `returnn-1.20230718.124003/returnn/datasets/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/bundle_file.py` & `returnn-1.20230718.124003/returnn/datasets/bundle_file.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/cached.py` & `returnn-1.20230718.124003/returnn/datasets/cached.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/cached2.py` & `returnn-1.20230718.124003/returnn/datasets/cached2.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/generating.py` & `returnn-1.20230718.124003/returnn/datasets/generating.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/hdf.py` & `returnn-1.20230718.124003/returnn/datasets/hdf.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/lm.py` & `returnn-1.20230718.124003/returnn/datasets/lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/map.py` & `returnn-1.20230718.124003/returnn/datasets/map.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/meta.py` & `returnn-1.20230718.124003/returnn/datasets/meta.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/multi_proc.py` & `returnn-1.20230718.124003/returnn/datasets/multi_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/normalization_data.py` & `returnn-1.20230718.124003/returnn/datasets/normalization_data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/numpy_dump.py` & `returnn-1.20230718.124003/returnn/datasets/numpy_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/raw_wav.py` & `returnn-1.20230718.124003/returnn/datasets/raw_wav.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/sprint.py` & `returnn-1.20230718.124003/returnn/datasets/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/stereo.py` & `returnn-1.20230718.124003/returnn/datasets/stereo.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/util/feature_extraction.py` & `returnn-1.20230718.124003/returnn/datasets/util/feature_extraction.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/datasets/util/vocabulary.py` & `returnn-1.20230718.124003/returnn/datasets/util/vocabulary.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/engine/base.py` & `returnn-1.20230718.124003/returnn/engine/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/engine/batch.py` & `returnn-1.20230718.124003/returnn/engine/batch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/__init__.py` & `returnn-1.20230718.124003/returnn/extern/WarpRna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/__main__.py` & `returnn-1.20230718.124003/returnn/extern/WarpRna/__main__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/LICENSE` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/README.md` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/aligner.gif` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/aligner.gif`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/check.png` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/check.png`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/core.cu` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/core.h` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/core_cpu.cpp` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/core_cpu.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/LICENSE`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/binding.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.cu`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/core.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/pytorch_binding/warp_rna/test.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/ref_rna.py` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/ref_rna.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/tensorflow_binding/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/tensorflow_binding/src/warp_rna_op_kernel_tmpl.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/tensorflow_binding/warp_rna/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/WarpRna/warp-rna/test.cpp` & `returnn-1.20230718.124003/returnn/extern/WarpRna/warp-rna/test.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/graph_editor/__init__.py` & `returnn-1.20230718.124003/returnn/extern/graph_editor/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/graph_editor/edit.py` & `returnn-1.20230718.124003/returnn/extern/graph_editor/edit.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/graph_editor/reroute.py` & `returnn-1.20230718.124003/returnn/extern/graph_editor/reroute.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/graph_editor/select.py` & `returnn-1.20230718.124003/returnn/extern/graph_editor/select.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/graph_editor/subgraph.py` & `returnn-1.20230718.124003/returnn/extern/graph_editor/subgraph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/graph_editor/transform.py` & `returnn-1.20230718.124003/returnn/extern/graph_editor/transform.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/extern/graph_editor/util.py` & `returnn-1.20230718.124003/returnn/extern/graph_editor/util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/forward_iface.py` & `returnn-1.20230718.124003/returnn/forward_iface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/__init__.py` & `returnn-1.20230718.124003/returnn/frontend/__init__.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/_backend.py` & `returnn-1.20230718.124003/returnn/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/_numpy_backend.py` & `returnn-1.20230718.124003/returnn/frontend/_numpy_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/_utils.py` & `returnn-1.20230718.124003/returnn/frontend/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/array_.py` & `returnn-1.20230718.124003/returnn/frontend/array_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/attention.py` & `returnn-1.20230718.124003/returnn/frontend/attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/cond.py` & `returnn-1.20230718.124003/returnn/frontend/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/const.py` & `returnn-1.20230718.124003/returnn/frontend/const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/container.py` & `returnn-1.20230718.124003/returnn/frontend/container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/conv.py` & `returnn-1.20230718.124003/returnn/frontend/conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/device.py` & `returnn-1.20230718.124003/returnn/frontend/device.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/dims.py` & `returnn-1.20230718.124003/returnn/frontend/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/dropout.py` & `returnn-1.20230718.124003/returnn/frontend/dropout.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/dtype.py` & `returnn-1.20230718.124003/returnn/frontend/dtype.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/encoder/base.py` & `returnn-1.20230718.124003/returnn/frontend/encoder/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/encoder/conformer.py` & `returnn-1.20230718.124003/returnn/frontend/encoder/conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/init.py` & `returnn-1.20230718.124003/returnn/frontend/init.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/linear.py` & `returnn-1.20230718.124003/returnn/frontend/linear.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/loop.py` & `returnn-1.20230718.124003/returnn/frontend/loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/loss.py` & `returnn-1.20230718.124003/returnn/frontend/loss.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/math_.py` & `returnn-1.20230718.124003/returnn/frontend/math_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/matmul.py` & `returnn-1.20230718.124003/returnn/frontend/matmul.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/module.py` & `returnn-1.20230718.124003/returnn/frontend/module.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/normalization.py` & `returnn-1.20230718.124003/returnn/frontend/normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/parameter.py` & `returnn-1.20230718.124003/returnn/frontend/parameter.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/rand.py` & `returnn-1.20230718.124003/returnn/frontend/rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/rec.py` & `returnn-1.20230718.124003/returnn/frontend/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/reduce.py` & `returnn-1.20230718.124003/returnn/frontend/reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/run_ctx.py` & `returnn-1.20230718.124003/returnn/frontend/run_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/signal.py` & `returnn-1.20230718.124003/returnn/frontend/signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/state.py` & `returnn-1.20230718.124003/returnn/frontend/state.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/tensor_array.py` & `returnn-1.20230718.124003/returnn/frontend/tensor_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/frontend/types.py` & `returnn-1.20230718.124003/returnn/frontend/types.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/import_/common.py` & `returnn-1.20230718.124003/returnn/import_/common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/import_/git.py` & `returnn-1.20230718.124003/returnn/import_/git.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/import_/import_.py` & `returnn-1.20230718.124003/returnn/import_/import_.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/learning_rate_control.py` & `returnn-1.20230718.124003/returnn/learning_rate_control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/log.py` & `returnn-1.20230718.124003/returnn/log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/native_op.cpp` & `returnn-1.20230718.124003/returnn/native_op.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/native_op.py` & `returnn-1.20230718.124003/returnn/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/pretrain.py` & `returnn-1.20230718.124003/returnn/pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/sprint/cache.py` & `returnn-1.20230718.124003/returnn/sprint/cache.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/sprint/control.py` & `returnn-1.20230718.124003/returnn/sprint/control.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/sprint/error_signals.py` & `returnn-1.20230718.124003/returnn/sprint/error_signals.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/sprint/extern_interface.py` & `returnn-1.20230718.124003/returnn/sprint/extern_interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/sprint/interface.py` & `returnn-1.20230718.124003/returnn/sprint/interface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tensor/_dim_extra.py` & `returnn-1.20230718.124003/returnn/tensor/_dim_extra.py`

 * *Files 0% similar despite different names*

```diff
@@ -725,5538 +725,5557 @@
 00002d40: 663a 0a20 2020 2020 2020 2020 2020 2074  f:.            t
 00002d50: 6167 2e73 616d 655f 6173 203d 2073 656c  ag.same_as = sel
 00002d60: 6620 2023 206e 6f74 2064 6563 6c61 7265  f  # not declare
 00002d70: 5f73 616d 655f 6173 2c20 6e6f 6e65 206f  _same_as, none o
 00002d80: 6620 7468 6520 6578 7472 6120 6368 6563  f the extra chec
 00002d90: 6b73 206e 6565 6465 640a 2020 2020 2020  ks needed.      
 00002da0: 2020 7265 7475 726e 2074 6167 0a0a 2020    return tag..  
-00002db0: 2020 6465 6620 5f63 616e 5f75 7365 5f69    def _can_use_i
-00002dc0: 6e5f 6374 7828 7365 6c66 2c20 6374 7829  n_ctx(self, ctx)
-00002dd0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00002de0: 2020 2020 2020 3a70 6172 616d 2043 6f6e        :param Con
-00002df0: 7472 6f6c 466c 6f77 436f 6e74 6578 747c  trolFlowContext|
-00002e00: 4e6f 6e65 2063 7478 3a0a 2020 2020 2020  None ctx:.      
-00002e10: 2020 3a72 7479 7065 3a20 626f 6f6c 0a20    :rtype: bool. 
-00002e20: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00002e30: 2020 2069 6620 7365 6c66 2e63 6f6e 7472     if self.contr
-00002e40: 6f6c 5f66 6c6f 775f 6374 7820 3d3d 2063  ol_flow_ctx == c
-00002e50: 7478 3a0a 2020 2020 2020 2020 2020 2020  tx:.            
-00002e60: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-00002e70: 2020 2020 6672 6f6d 2072 6574 7572 6e6e      from returnn
-00002e80: 2e74 662e 7574 696c 2e64 6174 6120 696d  .tf.util.data im
-00002e90: 706f 7274 2043 6f6e 7472 6f6c 466c 6f77  port ControlFlow
-00002ea0: 436f 6e74 6578 740a 0a20 2020 2020 2020  Context..       
-00002eb0: 2069 6620 6e6f 7420 436f 6e74 726f 6c46   if not ControlF
-00002ec0: 6c6f 7743 6f6e 7465 7874 2e69 735f 7061  lowContext.is_pa
-00002ed0: 7265 6e74 5f6f 725f 7361 6d65 2873 656c  rent_or_same(sel
-00002ee0: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
-00002ef0: 7478 2c20 6374 7829 3a0a 2020 2020 2020  tx, ctx):.      
-00002f00: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-00002f10: 7365 0a20 2020 2020 2020 2061 7373 6572  se.        asser
-00002f20: 7420 6374 780a 2020 2020 2020 2020 2320  t ctx.        # 
-00002f30: 452e 672e 2063 7478 203d 3d20 6c6f 6f70  E.g. ctx == loop
-00002f40: 2874 696d 655f 6469 6d29 2c20 7768 656e  (time_dim), when
-00002f50: 2073 656c 662e 636f 6e74 726f 6c5f 666c   self.control_fl
-00002f60: 6f77 5f63 7478 203d 3d20 4e6f 6e65 2c0a  ow_ctx == None,.
-00002f70: 2020 2020 2020 2020 2320 7765 2063 616e          # we can
-00002f80: 2075 7365 2073 656c 6620 696e 2063 7478   use self in ctx
-00002f90: 2c20 6966 6620 7469 6d65 5f64 696d 206e  , iff time_dim n
-00002fa0: 6f74 2069 6e20 7365 6c66 2e64 796e 5f73  ot in self.dyn_s
-00002fb0: 697a 655f 6578 742e 6469 6d5f 7461 6773  ize_ext.dim_tags
-00002fc0: 2e0a 2020 2020 2020 2020 2320 5765 2063  ..        # We c
-00002fd0: 616e 206f 6e6c 7920 646f 2074 6869 7320  an only do this 
-00002fe0: 6368 6563 6b20 6966 2077 6520 6b6e 6f77  check if we know
-00002ff0: 2061 626f 7574 2064 796e 5f73 697a 655f   about dyn_size_
-00003000: 6578 742e 0a20 2020 2020 2020 2069 6620  ext..        if 
-00003010: 6e6f 7420 7365 6c66 2e64 796e 5f73 697a  not self.dyn_siz
-00003020: 655f 6578 743a 0a20 2020 2020 2020 2020  e_ext:.         
-00003030: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-00003040: 2020 2020 2020 2020 7061 7265 6e74 5f64          parent_d
-00003050: 696d 7320 3d20 436f 6e74 726f 6c46 6c6f  ims = ControlFlo
-00003060: 7743 6f6e 7465 7874 2e63 6f6c 6c65 6374  wContext.collect
-00003070: 5f70 6172 656e 745f 6469 6d73 2863 7478  _parent_dims(ctx
-00003080: 290a 2020 2020 2020 2020 666f 7220 6469  ).        for di
-00003090: 6d20 696e 2073 656c 662e 6479 6e5f 7369  m in self.dyn_si
-000030a0: 7a65 5f65 7874 2e64 696d 5f74 6167 733a  ze_ext.dim_tags:
-000030b0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000030c0: 6469 6d20 696e 2070 6172 656e 745f 6469  dim in parent_di
-000030d0: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-000030e0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-000030f0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00003100: 5472 7565 0a0a 2020 2020 6465 6620 5f76  True..    def _v
-00003110: 616c 6964 6174 655f 696e 5f63 7572 7265  alidate_in_curre
-00003120: 6e74 5f67 7261 7068 2873 656c 6629 3a0a  nt_graph(self):.
-00003130: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00003140: 2020 2020 3a72 7479 7065 3a20 626f 6f6c      :rtype: bool
-00003150: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00003160: 2020 2020 2069 6620 280a 2020 2020 2020       if (.      
-00003170: 2020 2020 2020 7365 6c66 2e64 796e 5f73        self.dyn_s
-00003180: 697a 655f 6578 7420 616e 6420 6e6f 7420  ize_ext and not 
-00003190: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
-000031a0: 742e 6973 5f76 616c 6964 5f69 6e5f 6375  t.is_valid_in_cu
-000031b0: 7272 656e 745f 6772 6170 6828 290a 2020  rrent_graph().  
-000031c0: 2020 2020 2020 293a 2020 2320 6d61 7962        ):  # mayb
-000031d0: 6520 6672 6f6d 2061 6e20 6561 726c 6965  e from an earlie
-000031e0: 7220 7275 6e20 7768 6963 6820 7265 7573  r run which reus
-000031f0: 6573 2074 6865 2064 696d 2074 6167 0a20  es the dim tag. 
-00003200: 2020 2020 2020 2020 2020 2023 2052 6573             # Res
-00003210: 6574 2061 6e64 2063 6c65 616e 7570 2e0a  et and cleanup..
-00003220: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003230: 2e64 796e 5f73 697a 655f 6578 7420 3d20  .dyn_size_ext = 
-00003240: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
-00003250: 742e 636f 7079 5f74 656d 706c 6174 6528  t.copy_template(
-00003260: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
-00003270: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
-00003280: 6261 7463 6820 3d20 4e6f 6e65 0a20 2020  batch = None.   
-00003290: 2020 2020 2020 2020 2073 616d 655f 6261           same_ba
-000032a0: 7365 203d 2073 656c 662e 6765 745f 7361  se = self.get_sa
-000032b0: 6d65 5f62 6173 6528 290a 2020 2020 2020  me_base().      
-000032c0: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
-000032d0: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
-000032e0: 4d65 6d62 6572 0a20 2020 2020 2020 2020  Member.         
-000032f0: 2020 2069 6620 7361 6d65 5f62 6173 652e     if same_base.
-00003300: 5f65 7874 7261 3a0a 2020 2020 2020 2020  _extra:.        
-00003310: 2020 2020 2020 2020 2320 6e6f 696e 7370          # noinsp
-00003320: 6563 7469 6f6e 2050 7950 726f 7465 6374  ection PyProtect
-00003330: 6564 4d65 6d62 6572 0a20 2020 2020 2020  edMember.       
-00003340: 2020 2020 2020 2020 2073 616d 655f 6261           same_ba
-00003350: 7365 2e5f 6578 7472 612e 7361 6d65 5f66  se._extra.same_f
-00003360: 6f72 5f62 6174 6368 5f63 7478 2e70 6f70  or_batch_ctx.pop
-00003370: 2828 7365 6c66 2e62 6174 6368 2c20 7365  ((self.batch, se
-00003380: 6c66 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  lf.control_flow_
-00003390: 6374 7829 2c20 4e6f 6e65 290a 2020 2020  ctx), None).    
-000033a0: 2020 2020 2020 2020 7365 6c66 2e62 6174          self.bat
-000033b0: 6368 203d 204e 6f6e 6520 2023 2069 7420  ch = None  # it 
-000033c0: 6973 2069 6e76 616c 6964 2069 6e20 7468  is invalid in th
-000033d0: 6520 6e65 7720 6772 6170 680a 2020 2020  e new graph.    
-000033e0: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
-000033f0: 7472 6f6c 5f66 6c6f 775f 6374 7820 3d20  trol_flow_ctx = 
-00003400: 4e6f 6e65 2020 2320 616c 736f 2069 6e76  None  # also inv
-00003410: 616c 6964 0a20 2020 2020 2020 2020 2020  alid.           
-00003420: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-00003430: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-00003440: 650a 0a20 2020 2064 6566 205f 6d61 7962  e..    def _mayb
-00003450: 655f 7570 6461 7465 2873 656c 663a 2044  e_update(self: D
-00003460: 696d 293a 0a20 2020 2020 2020 2069 6620  im):.        if 
-00003470: 7365 6c66 2e69 735f 6261 7463 685f 6469  self.is_batch_di
-00003480: 6d28 293a 0a20 2020 2020 2020 2020 2020  m():.           
-00003490: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-000034a0: 6966 2069 7369 6e73 7461 6e63 6528 7365  if isinstance(se
-000034b0: 6c66 2e73 697a 652c 2069 6e74 293a 0a20  lf.size, int):. 
-000034c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-000034d0: 6e0a 2020 2020 2020 2020 6966 206e 6f74  n.        if not
-000034e0: 2073 656c 662e 5f65 7874 7261 3a0a 2020   self._extra:.  
-000034f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00003500: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00003510: 7365 6c66 2e62 6174 6368 3a0a 2020 2020  self.batch:.    
-00003520: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00003530: 6479 6e5f 7369 7a65 5f65 7874 2061 6e64  dyn_size_ext and
-00003540: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-00003550: 7874 2e62 6174 6368 3a0a 2020 2020 2020  xt.batch:.      
-00003560: 2020 2020 2020 2020 2020 7365 6c66 2e62            self.b
-00003570: 6174 6368 203d 2073 656c 662e 6479 6e5f  atch = self.dyn_
-00003580: 7369 7a65 5f65 7874 2e62 6174 6368 0a20  size_ext.batch. 
-00003590: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000035a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000035b0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-000035c0: 6578 7472 6120 3d20 7365 6c66 2e5f 6765  extra = self._ge
-000035d0: 745f 7361 6d65 5f62 6173 655f 6578 7472  t_same_base_extr
-000035e0: 6128 290a 2020 2020 2020 2020 6966 206e  a().        if n
-000035f0: 6f74 2065 7874 7261 3a0a 2020 2020 2020  ot extra:.      
-00003600: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00003610: 2020 2020 206b 6579 203d 2028 7365 6c66       key = (self
-00003620: 2e62 6174 6368 2c20 7365 6c66 2e63 6f6e  .batch, self.con
-00003630: 7472 6f6c 5f66 6c6f 775f 6374 7829 0a20  trol_flow_ctx). 
-00003640: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-00003650: 796e 5f73 697a 655f 6578 7420 616e 6420  yn_size_ext and 
-00003660: 6b65 7920 6e6f 7420 696e 2065 7874 7261  key not in extra
-00003670: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
-00003680: 6374 783a 0a20 2020 2020 2020 2020 2020  ctx:.           
-00003690: 2065 7874 7261 2e73 616d 655f 666f 725f   extra.same_for_
-000036a0: 6261 7463 685f 6374 785b 6b65 795d 203d  batch_ctx[key] =
-000036b0: 2073 656c 660a 2020 2020 2020 2020 2320   self.        # 
-000036c0: 4368 6563 6b20 6966 2077 6520 6361 6e20  Check if we can 
-000036d0: 6669 6e64 206d 6f72 650a 2020 2020 2020  find more.      
-000036e0: 2020 6966 206b 6579 2069 6e20 6578 7472    if key in extr
-000036f0: 612e 7361 6d65 5f66 6f72 5f62 6174 6368  a.same_for_batch
-00003700: 5f63 7478 3a0a 2020 2020 2020 2020 2020  _ctx:.          
-00003710: 2020 7361 6d65 203d 2065 7874 7261 2e73    same = extra.s
-00003720: 616d 655f 666f 725f 6261 7463 685f 6374  ame_for_batch_ct
-00003730: 785b 6b65 795d 0a20 2020 2020 2020 2020  x[key].         
-00003740: 2020 2069 6620 7361 6d65 2069 7320 6e6f     if same is no
-00003750: 7420 7365 6c66 3a0a 2020 2020 2020 2020  t self:.        
-00003760: 2020 2020 2020 2020 6966 2073 616d 652e          if same.
-00003770: 6479 6e5f 7369 7a65 5f65 7874 2061 6e64  dyn_size_ext and
-00003780: 206e 6f74 2073 656c 662e 6479 6e5f 7369   not self.dyn_si
-00003790: 7a65 5f65 7874 3a0a 2020 2020 2020 2020  ze_ext:.        
-000037a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000037b0: 2e64 796e 5f73 697a 655f 6578 7420 3d20  .dyn_size_ext = 
-000037c0: 7361 6d65 2e64 796e 5f73 697a 655f 6578  same.dyn_size_ex
-000037d0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-000037e0: 2020 6966 2073 616d 652e 6479 6e5f 7369    if same.dyn_si
-000037f0: 7a65 5f65 7874 2061 6e64 2073 616d 652e  ze_ext and same.
-00003800: 6479 6e5f 7369 7a65 5f65 7874 2e70 6c61  dyn_size_ext.pla
-00003810: 6365 686f 6c64 6572 2069 7320 6e6f 7420  ceholder is not 
-00003820: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-00003830: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
-00003840: 662e 6479 6e5f 7369 7a65 5f65 7874 2e70  f.dyn_size_ext.p
-00003850: 6c61 6365 686f 6c64 6572 2069 7320 4e6f  laceholder is No
-00003860: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00003870: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00003880: 2e64 796e 5f73 697a 655f 6578 7420 3d20  .dyn_size_ext = 
-00003890: 7361 6d65 2e64 796e 5f73 697a 655f 6578  same.dyn_size_ex
-000038a0: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
-000038b0: 2020 6966 2073 656c 662e 6479 6e5f 7369    if self.dyn_si
-000038c0: 7a65 5f65 7874 2061 6e64 206e 6f74 2073  ze_ext and not s
-000038d0: 616d 652e 6479 6e5f 7369 7a65 5f65 7874  ame.dyn_size_ext
-000038e0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000038f0: 2020 2020 2020 7361 6d65 2e64 796e 5f73        same.dyn_s
-00003900: 697a 655f 6578 7420 3d20 7365 6c66 2e64  ize_ext = self.d
-00003910: 796e 5f73 697a 655f 6578 740a 2020 2020  yn_size_ext.    
-00003920: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00003930: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-00003940: 2061 6e64 2073 656c 662e 6479 6e5f 7369   and self.dyn_si
-00003950: 7a65 5f65 7874 2e70 6c61 6365 686f 6c64  ze_ext.placehold
-00003960: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
-00003970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00003980: 2020 2020 6966 206e 6f74 2073 616d 652e      if not same.
-00003990: 6479 6e5f 7369 7a65 5f65 7874 206f 7220  dyn_size_ext or 
-000039a0: 7361 6d65 2e64 796e 5f73 697a 655f 6578  same.dyn_size_ex
-000039b0: 742e 706c 6163 6568 6f6c 6465 7220 6973  t.placeholder is
-000039c0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000039d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-000039e0: 616d 652e 6479 6e5f 7369 7a65 5f65 7874  ame.dyn_size_ext
-000039f0: 203d 2073 656c 662e 6479 6e5f 7369 7a65   = self.dyn_size
-00003a00: 5f65 7874 0a0a 2020 2020 6465 6620 6765  _ext..    def ge
-00003a10: 745f 666f 725f 6261 7463 685f 6374 7828  t_for_batch_ctx(
-00003a20: 7365 6c66 3a20 4469 6d2c 2062 6174 6368  self: Dim, batch
-00003a30: 2c20 6374 782c 2061 6c6c 6f77 5f6e 6f6e  , ctx, allow_non
-00003a40: 653d 4661 6c73 6529 202d 3e20 4f70 7469  e=False) -> Opti
-00003a50: 6f6e 616c 5b44 696d 5d3a 0a20 2020 2020  onal[Dim]:.     
-00003a60: 2020 2022 2222 0a20 2020 2020 2020 2057     """.        W
-00003a70: 6172 6e69 6e67 3a20 5468 6973 2069 7320  arning: This is 
-00003a80: 6f6e 6c79 2066 6f72 2054 656e 736f 7246  only for TensorF
-00003a90: 6c6f 772c 2061 6e64 2061 6c73 6f20 7765  low, and also we
-00003aa0: 206d 6967 6874 2077 616e 7420 746f 2072   might want to r
-00003ab0: 656d 6f76 6520 6974 2e0a 2020 2020 2020  emove it..      
-00003ac0: 2020 6874 7470 733a 2f2f 6769 7468 7562    https://github
-00003ad0: 2e63 6f6d 2f72 7774 682d 6936 2f72 6574  .com/rwth-i6/ret
-00003ae0: 7572 6e6e 2f69 7373 7565 732f 3937 350a  urnn/issues/975.
-00003af0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00003b00: 4261 7463 6849 6e66 6f20 6261 7463 683a  BatchInfo batch:
-00003b10: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00003b20: 436f 6e74 726f 6c46 6c6f 7743 6f6e 7465  ControlFlowConte
-00003b30: 7874 7c4e 6f6e 6520 6374 783a 0a20 2020  xt|None ctx:.   
-00003b40: 2020 2020 203a 7061 7261 6d20 626f 6f6c       :param bool
-00003b50: 2061 6c6c 6f77 5f6e 6f6e 653a 0a20 2020   allow_none:.   
-00003b60: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00003b70: 2061 7373 6572 7420 7365 6c66 2e63 616e   assert self.can
-00003b80: 5f62 655f 7573 6564 5f61 735f 6469 6d28  _be_used_as_dim(
-00003b90: 290a 2020 2020 2020 2020 6966 2073 656c  ).        if sel
-00003ba0: 662e 6261 7463 6820 3d3d 2062 6174 6368  f.batch == batch
-00003bb0: 2061 6e64 2073 656c 662e 636f 6e74 726f   and self.contro
-00003bc0: 6c5f 666c 6f77 5f63 7478 203d 3d20 6374  l_flow_ctx == ct
-00003bd0: 7820 616e 6420 7365 6c66 2e64 796e 5f73  x and self.dyn_s
-00003be0: 697a 655f 6578 743a 0a20 2020 2020 2020  ize_ext:.       
-00003bf0: 2020 2020 2073 656c 662e 5f76 616c 6964       self._valid
-00003c00: 6174 655f 696e 5f63 7572 7265 6e74 5f67  ate_in_current_g
-00003c10: 7261 7068 2829 0a20 2020 2020 2020 2020  raph().         
-00003c20: 2020 2073 656c 662e 5f6d 6179 6265 5f75     self._maybe_u
-00003c30: 7064 6174 6528 290a 2020 2020 2020 2020  pdate().        
-00003c40: 2020 2020 6966 2073 656c 662e 6261 7463      if self.batc
-00003c50: 6820 3d3d 2062 6174 6368 2061 6e64 2073  h == batch and s
-00003c60: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
-00003c70: 5f63 7478 203d 3d20 6374 7820 616e 6420  _ctx == ctx and 
-00003c80: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
-00003c90: 743a 2020 2320 6368 6563 6b20 6167 6169  t:  # check agai
-00003ca0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00003cb0: 2020 7265 7475 726e 2073 656c 660a 2020    return self.  
-00003cc0: 2020 2020 2020 6966 2073 656c 662e 6973        if self.is
-00003cd0: 5f62 6174 6368 5f64 696d 2829 3a0a 2020  _batch_dim():.  
-00003ce0: 2020 2020 2020 2020 2020 2320 5765 2069            # We i
-00003cf0: 676e 6f72 6520 7468 6520 6374 7820 666f  gnore the ctx fo
-00003d00: 7220 7468 6520 6261 7463 6820 6469 6d20  r the batch dim 
-00003d10: 6375 7272 656e 746c 792e 0a20 2020 2020  currently..     
-00003d20: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-00003d30: 6174 6368 203d 3d20 6261 7463 683a 0a20  atch == batch:. 
-00003d40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00003d50: 6574 7572 6e20 7365 6c66 0a20 2020 2020  eturn self.     
-00003d60: 2020 2020 2020 2069 6620 6261 7463 682e         if batch.
-00003d70: 6973 5f67 6c6f 6261 6c5f 6261 7463 6828  is_global_batch(
-00003d80: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00003d90: 2020 2072 6574 7572 6e20 5f64 2e62 6174     return _d.bat
-00003da0: 6368 5f64 696d 2020 2320 7265 7573 6520  ch_dim  # reuse 
-00003db0: 676c 6f62 616c 2062 6174 6368 2064 696d  global batch dim
-00003dc0: 2069 6620 706f 7373 6962 6c65 0a20 2020   if possible.   
-00003dd0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00003de0: 5f64 2e44 696d 286b 696e 643d 4469 6d54  _d.Dim(kind=DimT
-00003df0: 7970 6573 2e42 6174 6368 2c20 6465 7363  ypes.Batch, desc
-00003e00: 7269 7074 696f 6e3d 2262 6174 6368 3a25  ription="batch:%
-00003e10: 7322 2025 2062 6174 6368 2e73 686f 7274  s" % batch.short
-00003e20: 5f72 6570 7228 292c 2062 6174 6368 3d62  _repr(), batch=b
-00003e30: 6174 6368 2c20 6469 6d65 6e73 696f 6e3d  atch, dimension=
-00003e40: 4e6f 6e65 290a 2020 2020 2020 2020 6966  None).        if
-00003e50: 206e 6f74 2073 656c 662e 6973 5f64 796e   not self.is_dyn
-00003e60: 616d 6963 2829 3a0a 2020 2020 2020 2020  amic():.        
-00003e70: 2020 2020 2320 4966 2073 7461 7469 6320      # If static 
-00003e80: 6469 6d2c 206e 6f20 6566 6665 6374 2e0a  dim, no effect..
-00003e90: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-00003ea0: 7274 206e 6f74 2073 656c 662e 6261 7463  rt not self.batc
-00003eb0: 680a 2020 2020 2020 2020 2020 2020 7265  h.            re
-00003ec0: 7475 726e 2073 656c 660a 2020 2020 2020  turn self.      
-00003ed0: 2020 6966 2062 6174 6368 2e69 735f 6272    if batch.is_br
-00003ee0: 6f61 6463 6173 7428 293a 0a20 2020 2020  oadcast():.     
-00003ef0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00003f00: 6c66 2020 2320 6a75 7374 206c 6561 7665  lf  # just leave
-00003f10: 2061 732d 6973 2e20 7368 6f75 6c64 206e   as-is. should n
-00003f20: 6f74 206d 6174 7465 722e 0a20 2020 2020  ot matter..     
-00003f30: 2020 2069 6620 7365 6c66 2e5f 6578 7472     if self._extr
-00003f40: 613a 0a20 2020 2020 2020 2020 2020 2073  a:.            s
-00003f50: 616d 655f 6261 7365 203d 2073 656c 662e  ame_base = self.
-00003f60: 6765 745f 7361 6d65 5f62 6173 6528 290a  get_same_base().
-00003f70: 2020 2020 2020 2020 2020 2020 7361 6d65              same
-00003f80: 5f62 6173 652e 5f76 616c 6964 6174 655f  _base._validate_
-00003f90: 696e 5f63 7572 7265 6e74 5f67 7261 7068  in_current_graph
-00003fa0: 2829 0a20 2020 2020 2020 2020 2020 2023  ().            #
-00003fb0: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
-00003fc0: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
-00003fd0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-00003fe0: 616d 655f 6261 7365 2e5f 6578 7472 613a  ame_base._extra:
-00003ff0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00004000: 2066 726f 6d20 7265 7475 726e 6e2e 7466   from returnn.tf
-00004010: 2e75 7469 6c2e 6461 7461 2069 6d70 6f72  .util.data impor
-00004020: 7420 436f 6e74 726f 6c46 6c6f 7743 6f6e  t ControlFlowCon
-00004030: 7465 7874 0a0a 2020 2020 2020 2020 2020  text..          
-00004040: 2020 2020 2020 666f 7220 6374 785f 2069        for ctx_ i
-00004050: 6e20 436f 6e74 726f 6c46 6c6f 7743 6f6e  n ControlFlowCon
-00004060: 7465 7874 2e61 6273 5f63 7478 5f73 7461  text.abs_ctx_sta
-00004070: 636b 5f77 6974 685f 726f 6f74 2863 7478  ck_with_root(ctx
-00004080: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00004090: 2020 2020 2020 2023 206e 6f69 6e73 7065         # noinspe
-000040a0: 6374 696f 6e20 5079 5072 6f74 6563 7465  ction PyProtecte
-000040b0: 644d 656d 6265 720a 2020 2020 2020 2020  dMember.        
-000040c0: 2020 2020 2020 2020 2020 2020 7461 6720              tag 
-000040d0: 3d20 7361 6d65 5f62 6173 652e 5f65 7874  = same_base._ext
-000040e0: 7261 2e73 616d 655f 666f 725f 6261 7463  ra.same_for_batc
-000040f0: 685f 6374 782e 6765 7428 2862 6174 6368  h_ctx.get((batch
-00004100: 2c20 6374 785f 292c 204e 6f6e 6529 0a20  , ctx_), None). 
-00004110: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004120: 2020 2069 6620 7461 6720 616e 6420 7461     if tag and ta
-00004130: 672e 5f63 616e 5f75 7365 5f69 6e5f 6374  g._can_use_in_ct
-00004140: 7828 6374 7829 2061 6e64 2074 6167 2e5f  x(ctx) and tag._
-00004150: 7661 6c69 6461 7465 5f69 6e5f 6375 7272  validate_in_curr
-00004160: 656e 745f 6772 6170 6828 293a 0a20 2020  ent_graph():.   
-00004170: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004180: 2020 2020 2061 7373 6572 7420 280a 2020       assert (.  
-00004190: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041a0: 2020 2020 2020 2020 2020 7461 672e 6261            tag.ba
-000041b0: 7463 6820 3d3d 2062 6174 6368 0a20 2020  tch == batch.   
-000041c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000041d0: 2020 2020 2029 2020 2320 736f 6d65 2063       )  # some c
-000041e0: 6f64 6520 7570 6461 7465 6420 6261 7463  ode updated batc
-000041f0: 6820 6469 7265 6374 6c79 2028 696e 636f  h directly (inco
-00004200: 7272 6563 746c 7929 2061 6e64 2063 6f75  rrectly) and cou
-00004210: 6c64 2074 7269 6767 6572 2074 6869 730a  ld trigger this.
-00004220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004230: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-00004240: 6167 0a20 2020 2020 2020 2020 2020 2069  ag.            i
-00004250: 6620 7361 6d65 5f62 6173 652e 6261 7463  f same_base.batc
-00004260: 6820 3d3d 2062 6174 6368 2061 6e64 2073  h == batch and s
-00004270: 616d 655f 6261 7365 2e5f 6361 6e5f 7573  ame_base._can_us
-00004280: 655f 696e 5f63 7478 2863 7478 2920 616e  e_in_ctx(ctx) an
-00004290: 6420 7361 6d65 5f62 6173 652e 6479 6e5f  d same_base.dyn_
-000042a0: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
-000042b0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-000042c0: 2073 616d 655f 6261 7365 0a20 2020 2020   same_base.     
-000042d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
-000042e0: 2020 2020 2073 616d 655f 6261 7365 203d       same_base =
-000042f0: 2073 656c 660a 2020 2020 2020 2020 7361   self.        sa
-00004300: 6d65 5f62 6173 655f 6578 7472 6120 3d20  me_base_extra = 
-00004310: 7361 6d65 5f62 6173 652e 5f6d 616b 655f  same_base._make_
-00004320: 6578 7472 6128 290a 2020 2020 2020 2020  extra().        
-00004330: 2320 4f6b 2c20 6e6f 7468 696e 6720 6d61  # Ok, nothing ma
-00004340: 7463 6869 6e67 2066 6f75 6e64 2e0a 2020  tching found..  
-00004350: 2020 2020 2020 6966 2063 7478 3a0a 2020        if ctx:.  
-00004360: 2020 2020 2020 2020 2020 2320 4368 6563            # Chec
-00004370: 6b20 6966 2074 6865 2063 7478 2069 7320  k if the ctx is 
-00004380: 7265 616c 6c79 2072 656c 6576 616e 742c  really relevant,
-00004390: 2077 6865 6e20 7468 6973 2069 7320 6465   when this is de
-000043a0: 7269 7665 6420 6672 6f6d 206f 7468 6572  rived from other
-000043b0: 2074 6167 732e 0a20 2020 2020 2020 2020   tags..         
-000043c0: 2020 2064 6572 6976 6564 5f62 6173 6573     derived_bases
-000043d0: 203d 2073 616d 655f 6261 7365 2e67 6574   = same_base.get
-000043e0: 5f64 6572 6976 6564 5f62 6173 6573 5f73  _derived_bases_s
-000043f0: 6574 2829 0a20 2020 2020 2020 2020 2020  et().           
-00004400: 2064 6572 6976 6564 5f62 6173 6573 2e72   derived_bases.r
-00004410: 656d 6f76 6528 7361 6d65 5f62 6173 6529  emove(same_base)
-00004420: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00004430: 6465 7269 7665 645f 6261 7365 733a 0a20  derived_bases:. 
-00004440: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00004450: 6572 6976 6564 5f63 7478 7320 3d20 7365  erived_ctxs = se
-00004460: 7428 290a 2020 2020 2020 2020 2020 2020  t().            
-00004470: 2020 2020 666f 7220 6420 696e 2064 6572      for d in der
-00004480: 6976 6564 5f62 6173 6573 3a0a 2020 2020  ived_bases:.    
-00004490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000044a0: 7769 7468 2075 7469 6c2e 6775 6172 645f  with util.guard_
-000044b0: 696e 6669 6e69 7465 5f72 6563 7572 7369  infinite_recursi
-000044c0: 6f6e 285f 642e 4469 6d2e 6765 745f 666f  on(_d.Dim.get_fo
-000044d0: 725f 6261 7463 685f 6374 782c 2064 293a  r_batch_ctx, d):
-000044e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000044f0: 2020 2020 2020 2020 2064 203d 2064 2e67           d = d.g
-00004500: 6574 5f66 6f72 5f62 6174 6368 5f63 7478  et_for_batch_ctx
-00004510: 2862 6174 6368 3d62 6174 6368 2c20 6374  (batch=batch, ct
-00004520: 783d 6374 7829 0a20 2020 2020 2020 2020  x=ctx).         
-00004530: 2020 2020 2020 2020 2020 2069 6620 642e             if d.
-00004540: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
-00004550: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00004560: 2020 2020 2020 2020 2020 6465 7269 7665            derive
-00004570: 645f 6374 7873 2e61 6464 2864 2e63 6f6e  d_ctxs.add(d.con
-00004580: 7472 6f6c 5f66 6c6f 775f 6374 7829 0a20  trol_flow_ctx). 
-00004590: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000045a0: 6620 6e6f 7420 6465 7269 7665 645f 6374  f not derived_ct
-000045b0: 7873 3a0a 2020 2020 2020 2020 2020 2020  xs:.            
-000045c0: 2020 2020 2020 2020 6374 7820 3d20 4e6f          ctx = No
-000045d0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-000045e0: 2020 2065 6c69 6620 6c65 6e28 6465 7269     elif len(deri
-000045f0: 7665 645f 6374 7873 2920 3d3d 2031 3a0a  ved_ctxs) == 1:.
-00004600: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004610: 2020 2020 6374 7820 3d20 6465 7269 7665      ctx = derive
-00004620: 645f 6374 7873 2e70 6f70 2829 0a20 2020  d_ctxs.pop().   
-00004630: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00004640: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00004650: 2020 2020 2020 2072 6169 7365 204e 6f74         raise Not
-00004660: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
-00004670: 2822 6e6f 7420 7965 7420 696d 706c 656d  ("not yet implem
-00004680: 656e 7465 643a 206d 756c 7469 706c 6520  ented: multiple 
-00004690: 6465 7269 7665 6420 6374 7873 3a20 2572  derived ctxs: %r
-000046a0: 2220 2520 2864 6572 6976 6564 5f63 7478  " % (derived_ctx
-000046b0: 732c 2929 0a20 2020 2020 2020 2064 796e  s,)).        dyn
-000046c0: 5f73 697a 655f 6578 7420 3d20 4e6f 6e65  _size_ext = None
-000046d0: 0a20 2020 2020 2020 2023 204d 6179 6265  .        # Maybe
-000046e0: 2077 6520 6861 7665 2073 7468 2077 6974   we have sth wit
-000046f0: 6820 7468 6520 6261 7365 2062 6174 6368  h the base batch
-00004700: 2077 6974 686f 7574 2062 6561 6d20 6f72   without beam or
-00004710: 2070 6164 6465 6420 6261 7463 6820 7768   padded batch wh
-00004720: 6963 6820 7765 2063 616e 2065 7874 656e  ich we can exten
-00004730: 642e 0a20 2020 2020 2020 2069 6620 6261  d..        if ba
-00004740: 7463 6820 213d 2062 6174 6368 2e67 6574  tch != batch.get
-00004750: 5f67 6c6f 6261 6c5f 6261 7365 2829 3a0a  _global_base():.
-00004760: 2020 2020 2020 2020 2020 2020 6261 7463              batc
-00004770: 685f 6261 7365 203d 2062 6174 6368 2e67  h_base = batch.g
-00004780: 6574 5f67 6c6f 6261 6c5f 6261 7365 2829  et_global_base()
-00004790: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
-000047a0: 655f 6361 6e5f 7573 655f 696e 5f63 7478  e_can_use_in_ctx
-000047b0: 203d 204e 6f6e 6520 2023 2074 7970 653a   = None  # type:
-000047c0: 204f 7074 696f 6e61 6c5b 5f64 2e44 696d   Optional[_d.Dim
-000047d0: 5d0a 2020 2020 2020 2020 2020 2020 2320  ].            # 
-000047e0: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
-000047f0: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
-00004800: 2020 2020 2020 2020 2020 2069 6620 7361             if sa
-00004810: 6d65 5f62 6173 652e 6261 7463 6820 3d3d  me_base.batch ==
-00004820: 2062 6174 6368 5f62 6173 6520 616e 6420   batch_base and 
-00004830: 7361 6d65 5f62 6173 652e 5f63 616e 5f75  same_base._can_u
-00004840: 7365 5f69 6e5f 6374 7828 6374 7829 2061  se_in_ctx(ctx) a
-00004850: 6e64 2073 616d 655f 6261 7365 2e64 796e  nd same_base.dyn
-00004860: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
-00004870: 2020 2020 2020 2020 2020 2062 6173 655f             base_
-00004880: 6361 6e5f 7573 655f 696e 5f63 7478 203d  can_use_in_ctx =
-00004890: 2073 616d 655f 6261 7365 0a20 2020 2020   same_base.     
-000048a0: 2020 2020 2020 2065 6c69 6620 7361 6d65         elif same
-000048b0: 5f62 6173 652e 5f65 7874 7261 3a0a 2020  _base._extra:.  
-000048c0: 2020 2020 2020 2020 2020 2020 2020 6672                fr
-000048d0: 6f6d 2072 6574 7572 6e6e 2e74 662e 7574  om returnn.tf.ut
-000048e0: 696c 2e64 6174 6120 696d 706f 7274 2043  il.data import C
-000048f0: 6f6e 7472 6f6c 466c 6f77 436f 6e74 6578  ontrolFlowContex
-00004900: 740a 0a20 2020 2020 2020 2020 2020 2020  t..             
-00004910: 2020 2066 6f72 2063 7478 5f20 696e 2043     for ctx_ in C
-00004920: 6f6e 7472 6f6c 466c 6f77 436f 6e74 6578  ontrolFlowContex
-00004930: 742e 6162 735f 6374 785f 7374 6163 6b5f  t.abs_ctx_stack_
-00004940: 7769 7468 5f72 6f6f 7428 6374 7829 3a0a  with_root(ctx):.
-00004950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004960: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
-00004970: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
-00004980: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
-00004990: 2020 2020 2020 2020 2074 6167 203d 2073           tag = s
-000049a0: 616d 655f 6261 7365 2e5f 6578 7472 612e  ame_base._extra.
-000049b0: 7361 6d65 5f66 6f72 5f62 6174 6368 5f63  same_for_batch_c
-000049c0: 7478 2e67 6574 2828 6261 7463 685f 6261  tx.get((batch_ba
-000049d0: 7365 2c20 6374 785f 292c 204e 6f6e 6529  se, ctx_), None)
-000049e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000049f0: 2020 2020 2069 6620 7461 6720 616e 6420       if tag and 
-00004a00: 7461 672e 5f63 616e 5f75 7365 5f69 6e5f  tag._can_use_in_
-00004a10: 6374 7828 6374 7829 2061 6e64 2074 6167  ctx(ctx) and tag
-00004a20: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
-00004a30: 7272 656e 745f 6772 6170 6828 2920 616e  rrent_graph() an
-00004a40: 6420 7461 672e 6479 6e5f 7369 7a65 5f65  d tag.dyn_size_e
-00004a50: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
-00004a60: 2020 2020 2020 2020 2020 2020 6261 7365              base
-00004a70: 5f63 616e 5f75 7365 5f69 6e5f 6374 7820  _can_use_in_ctx 
-00004a80: 3d20 7461 670a 2020 2020 2020 2020 2020  = tag.          
-00004a90: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00004aa0: 6561 6b0a 2020 2020 2020 2020 2020 2020  eak.            
-00004ab0: 6966 2062 6173 655f 6361 6e5f 7573 655f  if base_can_use_
-00004ac0: 696e 5f63 7478 2061 6e64 2062 6173 655f  in_ctx and base_
-00004ad0: 6361 6e5f 7573 655f 696e 5f63 7478 2e64  can_use_in_ctx.d
-00004ae0: 796e 5f73 697a 655f 6578 743a 0a20 2020  yn_size_ext:.   
-00004af0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004b00: 6261 7365 5f63 616e 5f75 7365 5f69 6e5f  base_can_use_in_
-00004b10: 6374 782e 6479 6e5f 7369 7a65 5f65 7874  ctx.dyn_size_ext
-00004b20: 2e68 6176 655f 6261 7463 685f 6178 6973  .have_batch_axis
-00004b30: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-00004b40: 2020 2020 2020 2020 2320 5468 6520 7361          # The sa
-00004b50: 6d65 5f62 6173 6520 6861 7320 736f 6d65  me_base has some
-00004b60: 2064 796e 2073 697a 6520 7769 7468 6f75   dyn size withou
-00004b70: 7420 616e 7920 6265 616d 206e 6f72 2063  t any beam nor c
-00004b80: 6f6e 7472 6f6c 2066 6c6f 7720 636f 6e74  ontrol flow cont
-00004b90: 6578 742e 0a20 2020 2020 2020 2020 2020  ext..           
-00004ba0: 2020 2020 2020 2020 2023 2057 6520 6361           # We ca
-00004bb0: 6e20 6578 7061 6e64 2069 7420 746f 2074  n expand it to t
-00004bc0: 6865 2063 7572 7265 6e74 2062 6561 6d2c  he current beam,
-00004bd0: 206f 7220 6578 7465 6e64 2062 7920 7061   or extend by pa
-00004be0: 6464 6564 2062 6174 6368 2e0a 2020 2020  dded batch..    
-00004bf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c00: 6479 6e5f 7369 7a65 5f65 7874 203d 2062  dyn_size_ext = b
-00004c10: 6173 655f 6361 6e5f 7573 655f 696e 5f63  ase_can_use_in_c
-00004c20: 7478 2e64 796e 5f73 697a 655f 6578 742e  tx.dyn_size_ext.
-00004c30: 636f 7079 5f65 7874 656e 645f 6261 7463  copy_extend_batc
-00004c40: 6828 6261 7463 6829 0a20 2020 2020 2020  h(batch).       
-00004c50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00004c60: 6261 7463 682e 6265 616d 3a0a 2020 2020  batch.beam:.    
-00004c70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004c80: 2020 2020 6479 6e5f 7369 7a65 5f65 7874      dyn_size_ext
-00004c90: 203d 2062 6173 655f 6361 6e5f 7573 655f   = base_can_use_
-00004ca0: 696e 5f63 7478 2e64 796e 5f73 697a 655f  in_ctx.dyn_size_
-00004cb0: 6578 742e 636f 7079 5f65 7874 656e 645f  ext.copy_extend_
-00004cc0: 7769 7468 5f62 6561 6d28 6261 7463 682e  with_beam(batch.
-00004cd0: 6265 616d 290a 2020 2020 2020 2020 2020  beam).          
-00004ce0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00004cf0: 2064 796e 5f73 697a 655f 6578 742e 6261   dyn_size_ext.ba
-00004d00: 7463 6820 3d3d 2062 6174 6368 0a20 2020  tch == batch.   
-00004d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d20: 2069 6620 6479 6e5f 7369 7a65 5f65 7874   if dyn_size_ext
-00004d30: 2e70 6c61 6365 686f 6c64 6572 2069 7320  .placeholder is 
-00004d40: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00004d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004d60: 2020 6265 616d 5f65 7870 616e 6465 645f    beam_expanded_
-00004d70: 6261 7365 5f64 6174 6120 3d20 6765 7461  base_data = geta
-00004d80: 7474 7228 0a20 2020 2020 2020 2020 2020  ttr(.           
-00004d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004da0: 2064 796e 5f73 697a 655f 6578 742e 706c   dyn_size_ext.pl
-00004db0: 6163 6568 6f6c 6465 722c 2022 5f52 4554  aceholder, "_RET
-00004dc0: 5552 4e4e 5f62 6561 6d5f 6578 7061 6e64  URNN_beam_expand
-00004dd0: 6564 5f62 6173 655f 6461 7461 222c 204e  ed_base_data", N
-00004de0: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
-00004df0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00004e00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e10: 2020 2020 2020 6966 2062 6174 6368 2e62        if batch.b
-00004e20: 6561 6d3a 0a20 2020 2020 2020 2020 2020  eam:.           
-00004e30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e40: 2061 7373 6572 7420 6265 616d 5f65 7870   assert beam_exp
-00004e50: 616e 6465 645f 6261 7365 5f64 6174 610a  anded_base_data.
-00004e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004e70: 2020 2020 2020 2020 2320 4e6f 7465 3a20          # Note: 
-00004e80: 5468 6520 6265 616d 2065 7870 616e 7369  The beam expansi
-00004e90: 6f6e 2075 7365 6420 7469 6c69 6e67 2c20  on used tiling, 
-00004ea0: 7768 6963 6820 6361 6e20 6265 2063 6163  which can be cac
-00004eb0: 6865 642e 0a20 2020 2020 2020 2020 2020  hed..           
-00004ec0: 2020 2020 2020 2020 2020 2020 2023 2054               # T
-00004ed0: 6869 7320 6d65 616e 7320 7468 6174 2077  his means that w
-00004ee0: 6520 636f 756c 6420 656e 6420 7570 2077  e could end up w
-00004ef0: 6974 6820 7468 6520 7361 6d65 2073 697a  ith the same siz
-00004f00: 6520 7465 6e73 6f72 2028 706c 6163 6568  e tensor (placeh
-00004f10: 6f6c 6465 7229 0a20 2020 2020 2020 2020  older).         
-00004f20: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-00004f30: 2066 6f72 206d 756c 7469 706c 6520 6469   for multiple di
-00004f40: 6666 6572 656e 7420 6265 616d 732c 0a20  fferent beams,. 
-00004f50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004f60: 2020 2020 2020 2023 2077 6865 6e20 7468         # when th
-00004f70: 6572 6520 6172 6520 6469 6666 6572 656e  ere are differen
-00004f80: 7420 6265 616d 7320 7769 7468 2073 616d  t beams with sam
-00004f90: 6520 6265 616d 2073 697a 6521 0a20 2020  e beam size!.   
-00004fa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00004fb0: 2020 2020 2023 2054 6869 7320 6272 6561       # This brea
-00004fc0: 6b73 2074 6865 2063 7572 7265 6e74 206c  ks the current l
-00004fd0: 6f67 6963 2069 6e20 6765 745f 7461 675f  ogic in get_tag_
-00004fe0: 6672 6f6d 5f73 697a 655f 7465 6e73 6f72  from_size_tensor
-00004ff0: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005000: 2020 2020 2020 2020 2020 2320 4173 2061            # As a
-00005010: 2077 6f72 6b61 726f 756e 642c 2077 6520   workaround, we 
-00005020: 6d61 6b65 2061 6e20 6578 706c 6963 6974  make an explicit
-00005030: 206e 6577 2074 656e 736f 7220 6865 7265   new tensor here
-00005040: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
-00005050: 2020 2020 2020 2020 2020 696d 706f 7274            import
-00005060: 2074 656e 736f 7266 6c6f 7720 6173 2074   tensorflow as t
-00005070: 660a 2020 2020 2020 2020 2020 2020 2020  f.              
-00005080: 2020 2020 2020 2020 2020 6672 6f6d 2072            from r
-00005090: 6574 7572 6e6e 2e74 662e 7574 696c 2e62  eturnn.tf.util.b
-000050a0: 6173 6963 2069 6d70 6f72 7420 6765 745f  asic import get_
-000050b0: 7661 6c69 645f 7363 6f70 655f 6e61 6d65  valid_scope_name
-000050c0: 5f66 726f 6d5f 7374 722c 2073 616d 655f  _from_str, same_
-000050d0: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
-000050e0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-000050f0: 2020 2020 2020 2020 2020 7769 7468 2073            with s
-00005100: 616d 655f 636f 6e74 726f 6c5f 666c 6f77  ame_control_flow
-00005110: 5f63 7478 2864 796e 5f73 697a 655f 6578  _ctx(dyn_size_ex
-00005120: 742e 706c 6163 6568 6f6c 6465 7229 3a0a  t.placeholder):.
+00002db0: 2020 6465 6620 7265 7365 745f 6561 6765    def reset_eage
+00002dc0: 7228 7365 6c66 3a20 4469 6d29 3a0a 2020  r(self: Dim):.  
+00002dd0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00002de0: 2020 496e 2061 6e20 6561 6765 722d 6261    In an eager-ba
+00002df0: 7365 6420 6672 616d 6577 6f72 6b2c 2064  sed framework, d
+00002e00: 796e 5f73 697a 655f 6578 742e 7261 775f  yn_size_ext.raw_
+00002e10: 7465 6e73 6f72 2065 7463 2077 696c 6c20  tensor etc will 
+00002e20: 6265 2064 6966 6665 7265 6e74 2069 6e20  be different in 
+00002e30: 6561 6368 2073 7465 702e 0a20 2020 2020  each step..     
+00002e40: 2020 2054 6869 7320 7265 7365 7473 2065     This resets e
+00002e50: 7665 7279 7468 696e 6720 7265 6c61 7465  verything relate
+00002e60: 642e 0a20 2020 2020 2020 2054 6869 7320  d..        This 
+00002e70: 6361 6e20 616c 736f 2069 6e63 6c75 6465  can also include
+00002e80: 2063 6163 6865 732e 0a20 2020 2020 2020   caches..       
+00002e90: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+00002ea0: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+00002eb0: 743a 0a20 2020 2020 2020 2020 2020 2073  t:.            s
+00002ec0: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+00002ed0: 2e72 6177 5f74 656e 736f 7220 3d20 4e6f  .raw_tensor = No
+00002ee0: 6e65 0a0a 2020 2020 6465 6620 5f63 616e  ne..    def _can
+00002ef0: 5f75 7365 5f69 6e5f 6374 7828 7365 6c66  _use_in_ctx(self
+00002f00: 2c20 6374 7829 3a0a 2020 2020 2020 2020  , ctx):.        
+00002f10: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
+00002f20: 616d 2043 6f6e 7472 6f6c 466c 6f77 436f  am ControlFlowCo
+00002f30: 6e74 6578 747c 4e6f 6e65 2063 7478 3a0a  ntext|None ctx:.
+00002f40: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00002f50: 626f 6f6c 0a20 2020 2020 2020 2022 2222  bool.        """
+00002f60: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00002f70: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
+00002f80: 7820 3d3d 2063 7478 3a0a 2020 2020 2020  x == ctx:.      
+00002f90: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+00002fa0: 650a 2020 2020 2020 2020 6672 6f6d 2072  e.        from r
+00002fb0: 6574 7572 6e6e 2e74 662e 7574 696c 2e64  eturnn.tf.util.d
+00002fc0: 6174 6120 696d 706f 7274 2043 6f6e 7472  ata import Contr
+00002fd0: 6f6c 466c 6f77 436f 6e74 6578 740a 0a20  olFlowContext.. 
+00002fe0: 2020 2020 2020 2069 6620 6e6f 7420 436f         if not Co
+00002ff0: 6e74 726f 6c46 6c6f 7743 6f6e 7465 7874  ntrolFlowContext
+00003000: 2e69 735f 7061 7265 6e74 5f6f 725f 7361  .is_parent_or_sa
+00003010: 6d65 2873 656c 662e 636f 6e74 726f 6c5f  me(self.control_
+00003020: 666c 6f77 5f63 7478 2c20 6374 7829 3a0a  flow_ctx, ctx):.
+00003030: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00003040: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+00003050: 2061 7373 6572 7420 6374 780a 2020 2020   assert ctx.    
+00003060: 2020 2020 2320 452e 672e 2063 7478 203d      # E.g. ctx =
+00003070: 3d20 6c6f 6f70 2874 696d 655f 6469 6d29  = loop(time_dim)
+00003080: 2c20 7768 656e 2073 656c 662e 636f 6e74  , when self.cont
+00003090: 726f 6c5f 666c 6f77 5f63 7478 203d 3d20  rol_flow_ctx == 
+000030a0: 4e6f 6e65 2c0a 2020 2020 2020 2020 2320  None,.        # 
+000030b0: 7765 2063 616e 2075 7365 2073 656c 6620  we can use self 
+000030c0: 696e 2063 7478 2c20 6966 6620 7469 6d65  in ctx, iff time
+000030d0: 5f64 696d 206e 6f74 2069 6e20 7365 6c66  _dim not in self
+000030e0: 2e64 796e 5f73 697a 655f 6578 742e 6469  .dyn_size_ext.di
+000030f0: 6d5f 7461 6773 2e0a 2020 2020 2020 2020  m_tags..        
+00003100: 2320 5765 2063 616e 206f 6e6c 7920 646f  # We can only do
+00003110: 2074 6869 7320 6368 6563 6b20 6966 2077   this check if w
+00003120: 6520 6b6e 6f77 2061 626f 7574 2064 796e  e know about dyn
+00003130: 5f73 697a 655f 6578 742e 0a20 2020 2020  _size_ext..     
+00003140: 2020 2069 6620 6e6f 7420 7365 6c66 2e64     if not self.d
+00003150: 796e 5f73 697a 655f 6578 743a 0a20 2020  yn_size_ext:.   
+00003160: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00003170: 4661 6c73 650a 2020 2020 2020 2020 7061  False.        pa
+00003180: 7265 6e74 5f64 696d 7320 3d20 436f 6e74  rent_dims = Cont
+00003190: 726f 6c46 6c6f 7743 6f6e 7465 7874 2e63  rolFlowContext.c
+000031a0: 6f6c 6c65 6374 5f70 6172 656e 745f 6469  ollect_parent_di
+000031b0: 6d73 2863 7478 290a 2020 2020 2020 2020  ms(ctx).        
+000031c0: 666f 7220 6469 6d20 696e 2073 656c 662e  for dim in self.
+000031d0: 6479 6e5f 7369 7a65 5f65 7874 2e64 696d  dyn_size_ext.dim
+000031e0: 5f74 6167 733a 0a20 2020 2020 2020 2020  _tags:.         
+000031f0: 2020 2069 6620 6469 6d20 696e 2070 6172     if dim in par
+00003200: 656e 745f 6469 6d73 3a0a 2020 2020 2020  ent_dims:.      
+00003210: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00003220: 2046 616c 7365 0a20 2020 2020 2020 2072   False.        r
+00003230: 6574 7572 6e20 5472 7565 0a0a 2020 2020  eturn True..    
+00003240: 6465 6620 5f76 616c 6964 6174 655f 696e  def _validate_in
+00003250: 5f63 7572 7265 6e74 5f67 7261 7068 2873  _current_graph(s
+00003260: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00003270: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
+00003280: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
+00003290: 2222 0a20 2020 2020 2020 2069 6620 280a  "".        if (.
+000032a0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000032b0: 2e64 796e 5f73 697a 655f 6578 7420 616e  .dyn_size_ext an
+000032c0: 6420 6e6f 7420 7365 6c66 2e64 796e 5f73  d not self.dyn_s
+000032d0: 697a 655f 6578 742e 6973 5f76 616c 6964  ize_ext.is_valid
+000032e0: 5f69 6e5f 6375 7272 656e 745f 6772 6170  _in_current_grap
+000032f0: 6828 290a 2020 2020 2020 2020 293a 2020  h().        ):  
+00003300: 2320 6d61 7962 6520 6672 6f6d 2061 6e20  # maybe from an 
+00003310: 6561 726c 6965 7220 7275 6e20 7768 6963  earlier run whic
+00003320: 6820 7265 7573 6573 2074 6865 2064 696d  h reuses the dim
+00003330: 2074 6167 0a20 2020 2020 2020 2020 2020   tag.           
+00003340: 2023 2052 6573 6574 2061 6e64 2063 6c65   # Reset and cle
+00003350: 616e 7570 2e0a 2020 2020 2020 2020 2020  anup..          
+00003360: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
+00003370: 6578 7420 3d20 7365 6c66 2e64 796e 5f73  ext = self.dyn_s
+00003380: 697a 655f 6578 742e 636f 7079 5f74 656d  ize_ext.copy_tem
+00003390: 706c 6174 6528 290a 2020 2020 2020 2020  plate().        
+000033a0: 2020 2020 7365 6c66 2e64 796e 5f73 697a      self.dyn_siz
+000033b0: 655f 6578 742e 6261 7463 6820 3d20 4e6f  e_ext.batch = No
+000033c0: 6e65 0a20 2020 2020 2020 2020 2020 2073  ne.            s
+000033d0: 616d 655f 6261 7365 203d 2073 656c 662e  ame_base = self.
+000033e0: 6765 745f 7361 6d65 5f62 6173 6528 290a  get_same_base().
+000033f0: 2020 2020 2020 2020 2020 2020 2320 6e6f              # no
+00003400: 696e 7370 6563 7469 6f6e 2050 7950 726f  inspection PyPro
+00003410: 7465 6374 6564 4d65 6d62 6572 0a20 2020  tectedMember.   
+00003420: 2020 2020 2020 2020 2069 6620 7361 6d65           if same
+00003430: 5f62 6173 652e 5f65 7874 7261 3a0a 2020  _base._extra:.  
+00003440: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00003450: 6e6f 696e 7370 6563 7469 6f6e 2050 7950  noinspection PyP
+00003460: 726f 7465 6374 6564 4d65 6d62 6572 0a20  rotectedMember. 
+00003470: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00003480: 616d 655f 6261 7365 2e5f 6578 7472 612e  ame_base._extra.
+00003490: 7361 6d65 5f66 6f72 5f62 6174 6368 5f63  same_for_batch_c
+000034a0: 7478 2e70 6f70 2828 7365 6c66 2e62 6174  tx.pop((self.bat
+000034b0: 6368 2c20 7365 6c66 2e63 6f6e 7472 6f6c  ch, self.control
+000034c0: 5f66 6c6f 775f 6374 7829 2c20 4e6f 6e65  _flow_ctx), None
+000034d0: 290a 2020 2020 2020 2020 2020 2020 7365  ).            se
+000034e0: 6c66 2e62 6174 6368 203d 204e 6f6e 6520  lf.batch = None 
+000034f0: 2023 2069 7420 6973 2069 6e76 616c 6964   # it is invalid
+00003500: 2069 6e20 7468 6520 6e65 7720 6772 6170   in the new grap
+00003510: 680a 2020 2020 2020 2020 2020 2020 7365  h.            se
+00003520: 6c66 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  lf.control_flow_
+00003530: 6374 7820 3d20 4e6f 6e65 2020 2320 616c  ctx = None  # al
+00003540: 736f 2069 6e76 616c 6964 0a20 2020 2020  so invalid.     
+00003550: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00003560: 6c73 650a 2020 2020 2020 2020 7265 7475  lse.        retu
+00003570: 726e 2054 7275 650a 0a20 2020 2064 6566  rn True..    def
+00003580: 205f 6d61 7962 655f 7570 6461 7465 2873   _maybe_update(s
+00003590: 656c 663a 2044 696d 293a 0a20 2020 2020  elf: Dim):.     
+000035a0: 2020 2069 6620 7365 6c66 2e69 735f 6261     if self.is_ba
+000035b0: 7463 685f 6469 6d28 293a 0a20 2020 2020  tch_dim():.     
+000035c0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+000035d0: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+000035e0: 6e63 6528 7365 6c66 2e73 697a 652c 2069  nce(self.size, i
+000035f0: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
+00003600: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00003610: 6966 206e 6f74 2073 656c 662e 5f65 7874  if not self._ext
+00003620: 7261 3a0a 2020 2020 2020 2020 2020 2020  ra:.            
+00003630: 7265 7475 726e 0a20 2020 2020 2020 2069  return.        i
+00003640: 6620 6e6f 7420 7365 6c66 2e62 6174 6368  f not self.batch
+00003650: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
+00003660: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
+00003670: 7874 2061 6e64 2073 656c 662e 6479 6e5f  xt and self.dyn_
+00003680: 7369 7a65 5f65 7874 2e62 6174 6368 3a0a  size_ext.batch:.
+00003690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000036a0: 7365 6c66 2e62 6174 6368 203d 2073 656c  self.batch = sel
+000036b0: 662e 6479 6e5f 7369 7a65 5f65 7874 2e62  f.dyn_size_ext.b
+000036c0: 6174 6368 0a20 2020 2020 2020 2020 2020  atch.           
+000036d0: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+000036e0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+000036f0: 2020 2020 2020 6578 7472 6120 3d20 7365        extra = se
+00003700: 6c66 2e5f 6765 745f 7361 6d65 5f62 6173  lf._get_same_bas
+00003710: 655f 6578 7472 6128 290a 2020 2020 2020  e_extra().      
+00003720: 2020 6966 206e 6f74 2065 7874 7261 3a0a    if not extra:.
+00003730: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00003740: 726e 0a20 2020 2020 2020 206b 6579 203d  rn.        key =
+00003750: 2028 7365 6c66 2e62 6174 6368 2c20 7365   (self.batch, se
+00003760: 6c66 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  lf.control_flow_
+00003770: 6374 7829 0a20 2020 2020 2020 2069 6620  ctx).        if 
+00003780: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+00003790: 7420 616e 6420 6b65 7920 6e6f 7420 696e  t and key not in
+000037a0: 2065 7874 7261 2e73 616d 655f 666f 725f   extra.same_for_
+000037b0: 6261 7463 685f 6374 783a 0a20 2020 2020  batch_ctx:.     
+000037c0: 2020 2020 2020 2065 7874 7261 2e73 616d         extra.sam
+000037d0: 655f 666f 725f 6261 7463 685f 6374 785b  e_for_batch_ctx[
+000037e0: 6b65 795d 203d 2073 656c 660a 2020 2020  key] = self.    
+000037f0: 2020 2020 2320 4368 6563 6b20 6966 2077      # Check if w
+00003800: 6520 6361 6e20 6669 6e64 206d 6f72 650a  e can find more.
+00003810: 2020 2020 2020 2020 6966 206b 6579 2069          if key i
+00003820: 6e20 6578 7472 612e 7361 6d65 5f66 6f72  n extra.same_for
+00003830: 5f62 6174 6368 5f63 7478 3a0a 2020 2020  _batch_ctx:.    
+00003840: 2020 2020 2020 2020 7361 6d65 203d 2065          same = e
+00003850: 7874 7261 2e73 616d 655f 666f 725f 6261  xtra.same_for_ba
+00003860: 7463 685f 6374 785b 6b65 795d 0a20 2020  tch_ctx[key].   
+00003870: 2020 2020 2020 2020 2069 6620 7361 6d65           if same
+00003880: 2069 7320 6e6f 7420 7365 6c66 3a0a 2020   is not self:.  
+00003890: 2020 2020 2020 2020 2020 2020 2020 6966                if
+000038a0: 2073 616d 652e 6479 6e5f 7369 7a65 5f65   same.dyn_size_e
+000038b0: 7874 2061 6e64 206e 6f74 2073 656c 662e  xt and not self.
+000038c0: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
+000038d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000038e0: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
+000038f0: 6578 7420 3d20 7361 6d65 2e64 796e 5f73  ext = same.dyn_s
+00003900: 697a 655f 6578 740a 2020 2020 2020 2020  ize_ext.        
+00003910: 2020 2020 2020 2020 6966 2073 616d 652e          if same.
+00003920: 6479 6e5f 7369 7a65 5f65 7874 2061 6e64  dyn_size_ext and
+00003930: 2073 616d 652e 6479 6e5f 7369 7a65 5f65   same.dyn_size_e
+00003940: 7874 2e70 6c61 6365 686f 6c64 6572 2069  xt.placeholder i
+00003950: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
+00003960: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003970: 6966 2073 656c 662e 6479 6e5f 7369 7a65  if self.dyn_size
+00003980: 5f65 7874 2e70 6c61 6365 686f 6c64 6572  _ext.placeholder
+00003990: 2069 7320 4e6f 6e65 3a0a 2020 2020 2020   is None:.      
+000039a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000039b0: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
+000039c0: 6578 7420 3d20 7361 6d65 2e64 796e 5f73  ext = same.dyn_s
+000039d0: 697a 655f 6578 740a 2020 2020 2020 2020  ize_ext.        
+000039e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000039f0: 6479 6e5f 7369 7a65 5f65 7874 2061 6e64  dyn_size_ext and
+00003a00: 206e 6f74 2073 616d 652e 6479 6e5f 7369   not same.dyn_si
+00003a10: 7a65 5f65 7874 3a0a 2020 2020 2020 2020  ze_ext:.        
+00003a20: 2020 2020 2020 2020 2020 2020 7361 6d65              same
+00003a30: 2e64 796e 5f73 697a 655f 6578 7420 3d20  .dyn_size_ext = 
+00003a40: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+00003a50: 740a 2020 2020 2020 2020 2020 2020 2020  t.              
+00003a60: 2020 6966 2073 656c 662e 6479 6e5f 7369    if self.dyn_si
+00003a70: 7a65 5f65 7874 2061 6e64 2073 656c 662e  ze_ext and self.
+00003a80: 6479 6e5f 7369 7a65 5f65 7874 2e70 6c61  dyn_size_ext.pla
+00003a90: 6365 686f 6c64 6572 2069 7320 6e6f 7420  ceholder is not 
+00003aa0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00003ab0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+00003ac0: 2073 616d 652e 6479 6e5f 7369 7a65 5f65   same.dyn_size_e
+00003ad0: 7874 206f 7220 7361 6d65 2e64 796e 5f73  xt or same.dyn_s
+00003ae0: 697a 655f 6578 742e 706c 6163 6568 6f6c  ize_ext.placehol
+00003af0: 6465 7220 6973 204e 6f6e 653a 0a20 2020  der is None:.   
+00003b00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003b10: 2020 2020 2073 616d 652e 6479 6e5f 7369       same.dyn_si
+00003b20: 7a65 5f65 7874 203d 2073 656c 662e 6479  ze_ext = self.dy
+00003b30: 6e5f 7369 7a65 5f65 7874 0a0a 2020 2020  n_size_ext..    
+00003b40: 6465 6620 6765 745f 666f 725f 6261 7463  def get_for_batc
+00003b50: 685f 6374 7828 7365 6c66 3a20 4469 6d2c  h_ctx(self: Dim,
+00003b60: 2062 6174 6368 2c20 6374 782c 2061 6c6c   batch, ctx, all
+00003b70: 6f77 5f6e 6f6e 653d 4661 6c73 6529 202d  ow_none=False) -
+00003b80: 3e20 4f70 7469 6f6e 616c 5b44 696d 5d3a  > Optional[Dim]:
+00003b90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00003ba0: 2020 2020 2057 6172 6e69 6e67 3a20 5468       Warning: Th
+00003bb0: 6973 2069 7320 6f6e 6c79 2066 6f72 2054  is is only for T
+00003bc0: 656e 736f 7246 6c6f 772c 2061 6e64 2061  ensorFlow, and a
+00003bd0: 6c73 6f20 7765 206d 6967 6874 2077 616e  lso we might wan
+00003be0: 7420 746f 2072 656d 6f76 6520 6974 2e0a  t to remove it..
+00003bf0: 2020 2020 2020 2020 6874 7470 733a 2f2f          https://
+00003c00: 6769 7468 7562 2e63 6f6d 2f72 7774 682d  github.com/rwth-
+00003c10: 6936 2f72 6574 7572 6e6e 2f69 7373 7565  i6/returnn/issue
+00003c20: 732f 3937 350a 0a20 2020 2020 2020 203a  s/975..        :
+00003c30: 7061 7261 6d20 4261 7463 6849 6e66 6f20  param BatchInfo 
+00003c40: 6261 7463 683a 0a20 2020 2020 2020 203a  batch:.        :
+00003c50: 7061 7261 6d20 436f 6e74 726f 6c46 6c6f  param ControlFlo
+00003c60: 7743 6f6e 7465 7874 7c4e 6f6e 6520 6374  wContext|None ct
+00003c70: 783a 0a20 2020 2020 2020 203a 7061 7261  x:.        :para
+00003c80: 6d20 626f 6f6c 2061 6c6c 6f77 5f6e 6f6e  m bool allow_non
+00003c90: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00003ca0: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
+00003cb0: 6c66 2e63 616e 5f62 655f 7573 6564 5f61  lf.can_be_used_a
+00003cc0: 735f 6469 6d28 290a 2020 2020 2020 2020  s_dim().        
+00003cd0: 6966 2073 656c 662e 6261 7463 6820 3d3d  if self.batch ==
+00003ce0: 2062 6174 6368 2061 6e64 2073 656c 662e   batch and self.
+00003cf0: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
+00003d00: 203d 3d20 6374 7820 616e 6420 7365 6c66   == ctx and self
+00003d10: 2e64 796e 5f73 697a 655f 6578 743a 0a20  .dyn_size_ext:. 
+00003d20: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00003d30: 5f76 616c 6964 6174 655f 696e 5f63 7572  _validate_in_cur
+00003d40: 7265 6e74 5f67 7261 7068 2829 0a20 2020  rent_graph().   
+00003d50: 2020 2020 2020 2020 2073 656c 662e 5f6d           self._m
+00003d60: 6179 6265 5f75 7064 6174 6528 290a 2020  aybe_update().  
+00003d70: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00003d80: 662e 6261 7463 6820 3d3d 2062 6174 6368  f.batch == batch
+00003d90: 2061 6e64 2073 656c 662e 636f 6e74 726f   and self.contro
+00003da0: 6c5f 666c 6f77 5f63 7478 203d 3d20 6374  l_flow_ctx == ct
+00003db0: 7820 616e 6420 7365 6c66 2e64 796e 5f73  x and self.dyn_s
+00003dc0: 697a 655f 6578 743a 2020 2320 6368 6563  ize_ext:  # chec
+00003dd0: 6b20 6167 6169 6e0a 2020 2020 2020 2020  k again.        
+00003de0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00003df0: 656c 660a 2020 2020 2020 2020 6966 2073  elf.        if s
+00003e00: 656c 662e 6973 5f62 6174 6368 5f64 696d  elf.is_batch_dim
+00003e10: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00003e20: 2320 5765 2069 676e 6f72 6520 7468 6520  # We ignore the 
+00003e30: 6374 7820 666f 7220 7468 6520 6261 7463  ctx for the batc
+00003e40: 6820 6469 6d20 6375 7272 656e 746c 792e  h dim currently.
+00003e50: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003e60: 7365 6c66 2e62 6174 6368 203d 3d20 6261  self.batch == ba
+00003e70: 7463 683a 0a20 2020 2020 2020 2020 2020  tch:.           
+00003e80: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00003e90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00003ea0: 6261 7463 682e 6973 5f67 6c6f 6261 6c5f  batch.is_global_
+00003eb0: 6261 7463 6828 293a 0a20 2020 2020 2020  batch():.       
+00003ec0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00003ed0: 5f64 2e62 6174 6368 5f64 696d 2020 2320  _d.batch_dim  # 
+00003ee0: 7265 7573 6520 676c 6f62 616c 2062 6174  reuse global bat
+00003ef0: 6368 2064 696d 2069 6620 706f 7373 6962  ch dim if possib
+00003f00: 6c65 0a20 2020 2020 2020 2020 2020 2072  le.            r
+00003f10: 6574 7572 6e20 5f64 2e44 696d 286b 696e  eturn _d.Dim(kin
+00003f20: 643d 4469 6d54 7970 6573 2e42 6174 6368  d=DimTypes.Batch
+00003f30: 2c20 6465 7363 7269 7074 696f 6e3d 2262  , description="b
+00003f40: 6174 6368 3a25 7322 2025 2062 6174 6368  atch:%s" % batch
+00003f50: 2e73 686f 7274 5f72 6570 7228 292c 2062  .short_repr(), b
+00003f60: 6174 6368 3d62 6174 6368 2c20 6469 6d65  atch=batch, dime
+00003f70: 6e73 696f 6e3d 4e6f 6e65 290a 2020 2020  nsion=None).    
+00003f80: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
+00003f90: 6973 5f64 796e 616d 6963 2829 3a0a 2020  is_dynamic():.  
+00003fa0: 2020 2020 2020 2020 2020 2320 4966 2073            # If s
+00003fb0: 7461 7469 6320 6469 6d2c 206e 6f20 6566  tatic dim, no ef
+00003fc0: 6665 6374 2e0a 2020 2020 2020 2020 2020  fect..          
+00003fd0: 2020 6173 7365 7274 206e 6f74 2073 656c    assert not sel
+00003fe0: 662e 6261 7463 680a 2020 2020 2020 2020  f.batch.        
+00003ff0: 2020 2020 7265 7475 726e 2073 656c 660a      return self.
+00004000: 2020 2020 2020 2020 6966 2062 6174 6368          if batch
+00004010: 2e69 735f 6272 6f61 6463 6173 7428 293a  .is_broadcast():
+00004020: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00004030: 7572 6e20 7365 6c66 2020 2320 6a75 7374  urn self  # just
+00004040: 206c 6561 7665 2061 732d 6973 2e20 7368   leave as-is. sh
+00004050: 6f75 6c64 206e 6f74 206d 6174 7465 722e  ould not matter.
+00004060: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00004070: 2e5f 6578 7472 613a 0a20 2020 2020 2020  ._extra:.       
+00004080: 2020 2020 2073 616d 655f 6261 7365 203d       same_base =
+00004090: 2073 656c 662e 6765 745f 7361 6d65 5f62   self.get_same_b
+000040a0: 6173 6528 290a 2020 2020 2020 2020 2020  ase().          
+000040b0: 2020 7361 6d65 5f62 6173 652e 5f76 616c    same_base._val
+000040c0: 6964 6174 655f 696e 5f63 7572 7265 6e74  idate_in_current
+000040d0: 5f67 7261 7068 2829 0a20 2020 2020 2020  _graph().       
+000040e0: 2020 2020 2023 206e 6f69 6e73 7065 6374       # noinspect
+000040f0: 696f 6e20 5079 5072 6f74 6563 7465 644d  ion PyProtectedM
+00004100: 656d 6265 720a 2020 2020 2020 2020 2020  ember.          
+00004110: 2020 6966 2073 616d 655f 6261 7365 2e5f    if same_base._
+00004120: 6578 7472 613a 0a20 2020 2020 2020 2020  extra:.         
+00004130: 2020 2020 2020 2066 726f 6d20 7265 7475         from retu
+00004140: 726e 6e2e 7466 2e75 7469 6c2e 6461 7461  rnn.tf.util.data
+00004150: 2069 6d70 6f72 7420 436f 6e74 726f 6c46   import ControlF
+00004160: 6c6f 7743 6f6e 7465 7874 0a0a 2020 2020  lowContext..    
+00004170: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00004180: 6374 785f 2069 6e20 436f 6e74 726f 6c46  ctx_ in ControlF
+00004190: 6c6f 7743 6f6e 7465 7874 2e61 6273 5f63  lowContext.abs_c
+000041a0: 7478 5f73 7461 636b 5f77 6974 685f 726f  tx_stack_with_ro
+000041b0: 6f74 2863 7478 293a 0a20 2020 2020 2020  ot(ctx):.       
+000041c0: 2020 2020 2020 2020 2020 2020 2023 206e               # n
+000041d0: 6f69 6e73 7065 6374 696f 6e20 5079 5072  oinspection PyPr
+000041e0: 6f74 6563 7465 644d 656d 6265 720a 2020  otectedMember.  
+000041f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004200: 2020 7461 6720 3d20 7361 6d65 5f62 6173    tag = same_bas
+00004210: 652e 5f65 7874 7261 2e73 616d 655f 666f  e._extra.same_fo
+00004220: 725f 6261 7463 685f 6374 782e 6765 7428  r_batch_ctx.get(
+00004230: 2862 6174 6368 2c20 6374 785f 292c 204e  (batch, ctx_), N
+00004240: 6f6e 6529 0a20 2020 2020 2020 2020 2020  one).           
+00004250: 2020 2020 2020 2020 2069 6620 7461 6720           if tag 
+00004260: 616e 6420 7461 672e 5f63 616e 5f75 7365  and tag._can_use
+00004270: 5f69 6e5f 6374 7828 6374 7829 2061 6e64  _in_ctx(ctx) and
+00004280: 2074 6167 2e5f 7661 6c69 6461 7465 5f69   tag._validate_i
+00004290: 6e5f 6375 7272 656e 745f 6772 6170 6828  n_current_graph(
+000042a0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000042b0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+000042c0: 7420 280a 2020 2020 2020 2020 2020 2020  t (.            
+000042d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000042e0: 7461 672e 6261 7463 6820 3d3d 2062 6174  tag.batch == bat
+000042f0: 6368 0a20 2020 2020 2020 2020 2020 2020  ch.             
+00004300: 2020 2020 2020 2020 2020 2029 2020 2320             )  # 
+00004310: 736f 6d65 2063 6f64 6520 7570 6461 7465  some code update
+00004320: 6420 6261 7463 6820 6469 7265 6374 6c79  d batch directly
+00004330: 2028 696e 636f 7272 6563 746c 7929 2061   (incorrectly) a
+00004340: 6e64 2063 6f75 6c64 2074 7269 6767 6572  nd could trigger
+00004350: 2074 6869 730a 2020 2020 2020 2020 2020   this.          
+00004360: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00004370: 7475 726e 2074 6167 0a20 2020 2020 2020  turn tag.       
+00004380: 2020 2020 2069 6620 7361 6d65 5f62 6173       if same_bas
+00004390: 652e 6261 7463 6820 3d3d 2062 6174 6368  e.batch == batch
+000043a0: 2061 6e64 2073 616d 655f 6261 7365 2e5f   and same_base._
+000043b0: 6361 6e5f 7573 655f 696e 5f63 7478 2863  can_use_in_ctx(c
+000043c0: 7478 2920 616e 6420 7361 6d65 5f62 6173  tx) and same_bas
+000043d0: 652e 6479 6e5f 7369 7a65 5f65 7874 3a0a  e.dyn_size_ext:.
+000043e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000043f0: 7265 7475 726e 2073 616d 655f 6261 7365  return same_base
+00004400: 0a20 2020 2020 2020 2065 6c73 653a 0a20  .        else:. 
+00004410: 2020 2020 2020 2020 2020 2073 616d 655f             same_
+00004420: 6261 7365 203d 2073 656c 660a 2020 2020  base = self.    
+00004430: 2020 2020 7361 6d65 5f62 6173 655f 6578      same_base_ex
+00004440: 7472 6120 3d20 7361 6d65 5f62 6173 652e  tra = same_base.
+00004450: 5f6d 616b 655f 6578 7472 6128 290a 2020  _make_extra().  
+00004460: 2020 2020 2020 2320 4f6b 2c20 6e6f 7468        # Ok, noth
+00004470: 696e 6720 6d61 7463 6869 6e67 2066 6f75  ing matching fou
+00004480: 6e64 2e0a 2020 2020 2020 2020 6966 2063  nd..        if c
+00004490: 7478 3a0a 2020 2020 2020 2020 2020 2020  tx:.            
+000044a0: 2320 4368 6563 6b20 6966 2074 6865 2063  # Check if the c
+000044b0: 7478 2069 7320 7265 616c 6c79 2072 656c  tx is really rel
+000044c0: 6576 616e 742c 2077 6865 6e20 7468 6973  evant, when this
+000044d0: 2069 7320 6465 7269 7665 6420 6672 6f6d   is derived from
+000044e0: 206f 7468 6572 2074 6167 732e 0a20 2020   other tags..   
+000044f0: 2020 2020 2020 2020 2064 6572 6976 6564           derived
+00004500: 5f62 6173 6573 203d 2073 616d 655f 6261  _bases = same_ba
+00004510: 7365 2e67 6574 5f64 6572 6976 6564 5f62  se.get_derived_b
+00004520: 6173 6573 5f73 6574 2829 0a20 2020 2020  ases_set().     
+00004530: 2020 2020 2020 2064 6572 6976 6564 5f62         derived_b
+00004540: 6173 6573 2e72 656d 6f76 6528 7361 6d65  ases.remove(same
+00004550: 5f62 6173 6529 0a20 2020 2020 2020 2020  _base).         
+00004560: 2020 2069 6620 6465 7269 7665 645f 6261     if derived_ba
+00004570: 7365 733a 0a20 2020 2020 2020 2020 2020  ses:.           
+00004580: 2020 2020 2064 6572 6976 6564 5f63 7478       derived_ctx
+00004590: 7320 3d20 7365 7428 290a 2020 2020 2020  s = set().      
+000045a0: 2020 2020 2020 2020 2020 666f 7220 6420            for d 
+000045b0: 696e 2064 6572 6976 6564 5f62 6173 6573  in derived_bases
+000045c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000045d0: 2020 2020 2020 7769 7468 2075 7469 6c2e        with util.
+000045e0: 6775 6172 645f 696e 6669 6e69 7465 5f72  guard_infinite_r
+000045f0: 6563 7572 7369 6f6e 285f 642e 4469 6d2e  ecursion(_d.Dim.
+00004600: 6765 745f 666f 725f 6261 7463 685f 6374  get_for_batch_ct
+00004610: 782c 2064 293a 0a20 2020 2020 2020 2020  x, d):.         
+00004620: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00004630: 203d 2064 2e67 6574 5f66 6f72 5f62 6174   = d.get_for_bat
+00004640: 6368 5f63 7478 2862 6174 6368 3d62 6174  ch_ctx(batch=bat
+00004650: 6368 2c20 6374 783d 6374 7829 0a20 2020  ch, ctx=ctx).   
+00004660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004670: 2069 6620 642e 636f 6e74 726f 6c5f 666c   if d.control_fl
+00004680: 6f77 5f63 7478 3a0a 2020 2020 2020 2020  ow_ctx:.        
+00004690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000046a0: 6465 7269 7665 645f 6374 7873 2e61 6464  derived_ctxs.add
+000046b0: 2864 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  (d.control_flow_
+000046c0: 6374 7829 0a20 2020 2020 2020 2020 2020  ctx).           
+000046d0: 2020 2020 2069 6620 6e6f 7420 6465 7269       if not deri
+000046e0: 7665 645f 6374 7873 3a0a 2020 2020 2020  ved_ctxs:.      
+000046f0: 2020 2020 2020 2020 2020 2020 2020 6374                ct
+00004700: 7820 3d20 4e6f 6e65 0a20 2020 2020 2020  x = None.       
+00004710: 2020 2020 2020 2020 2065 6c69 6620 6c65           elif le
+00004720: 6e28 6465 7269 7665 645f 6374 7873 2920  n(derived_ctxs) 
+00004730: 3d3d 2031 3a0a 2020 2020 2020 2020 2020  == 1:.          
+00004740: 2020 2020 2020 2020 2020 6374 7820 3d20            ctx = 
+00004750: 6465 7269 7665 645f 6374 7873 2e70 6f70  derived_ctxs.pop
+00004760: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
+00004770: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00004780: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+00004790: 7365 204e 6f74 496d 706c 656d 656e 7465  se NotImplemente
+000047a0: 6445 7272 6f72 2822 6e6f 7420 7965 7420  dError("not yet 
+000047b0: 696d 706c 656d 656e 7465 643a 206d 756c  implemented: mul
+000047c0: 7469 706c 6520 6465 7269 7665 6420 6374  tiple derived ct
+000047d0: 7873 3a20 2572 2220 2520 2864 6572 6976  xs: %r" % (deriv
+000047e0: 6564 5f63 7478 732c 2929 0a20 2020 2020  ed_ctxs,)).     
+000047f0: 2020 2064 796e 5f73 697a 655f 6578 7420     dyn_size_ext 
+00004800: 3d20 4e6f 6e65 0a20 2020 2020 2020 2023  = None.        #
+00004810: 204d 6179 6265 2077 6520 6861 7665 2073   Maybe we have s
+00004820: 7468 2077 6974 6820 7468 6520 6261 7365  th with the base
+00004830: 2062 6174 6368 2077 6974 686f 7574 2062   batch without b
+00004840: 6561 6d20 6f72 2070 6164 6465 6420 6261  eam or padded ba
+00004850: 7463 6820 7768 6963 6820 7765 2063 616e  tch which we can
+00004860: 2065 7874 656e 642e 0a20 2020 2020 2020   extend..       
+00004870: 2069 6620 6261 7463 6820 213d 2062 6174   if batch != bat
+00004880: 6368 2e67 6574 5f67 6c6f 6261 6c5f 6261  ch.get_global_ba
+00004890: 7365 2829 3a0a 2020 2020 2020 2020 2020  se():.          
+000048a0: 2020 6261 7463 685f 6261 7365 203d 2062    batch_base = b
+000048b0: 6174 6368 2e67 6574 5f67 6c6f 6261 6c5f  atch.get_global_
+000048c0: 6261 7365 2829 0a20 2020 2020 2020 2020  base().         
+000048d0: 2020 2062 6173 655f 6361 6e5f 7573 655f     base_can_use_
+000048e0: 696e 5f63 7478 203d 204e 6f6e 6520 2023  in_ctx = None  #
+000048f0: 2074 7970 653a 204f 7074 696f 6e61 6c5b   type: Optional[
+00004900: 5f64 2e44 696d 5d0a 2020 2020 2020 2020  _d.Dim].        
+00004910: 2020 2020 2320 6e6f 696e 7370 6563 7469      # noinspecti
+00004920: 6f6e 2050 7950 726f 7465 6374 6564 4d65  on PyProtectedMe
+00004930: 6d62 6572 0a20 2020 2020 2020 2020 2020  mber.           
+00004940: 2069 6620 7361 6d65 5f62 6173 652e 6261   if same_base.ba
+00004950: 7463 6820 3d3d 2062 6174 6368 5f62 6173  tch == batch_bas
+00004960: 6520 616e 6420 7361 6d65 5f62 6173 652e  e and same_base.
+00004970: 5f63 616e 5f75 7365 5f69 6e5f 6374 7828  _can_use_in_ctx(
+00004980: 6374 7829 2061 6e64 2073 616d 655f 6261  ctx) and same_ba
+00004990: 7365 2e64 796e 5f73 697a 655f 6578 743a  se.dyn_size_ext:
+000049a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000049b0: 2062 6173 655f 6361 6e5f 7573 655f 696e   base_can_use_in
+000049c0: 5f63 7478 203d 2073 616d 655f 6261 7365  _ctx = same_base
+000049d0: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+000049e0: 6620 7361 6d65 5f62 6173 652e 5f65 7874  f same_base._ext
+000049f0: 7261 3a0a 2020 2020 2020 2020 2020 2020  ra:.            
+00004a00: 2020 2020 6672 6f6d 2072 6574 7572 6e6e      from returnn
+00004a10: 2e74 662e 7574 696c 2e64 6174 6120 696d  .tf.util.data im
+00004a20: 706f 7274 2043 6f6e 7472 6f6c 466c 6f77  port ControlFlow
+00004a30: 436f 6e74 6578 740a 0a20 2020 2020 2020  Context..       
+00004a40: 2020 2020 2020 2020 2066 6f72 2063 7478           for ctx
+00004a50: 5f20 696e 2043 6f6e 7472 6f6c 466c 6f77  _ in ControlFlow
+00004a60: 436f 6e74 6578 742e 6162 735f 6374 785f  Context.abs_ctx_
+00004a70: 7374 6163 6b5f 7769 7468 5f72 6f6f 7428  stack_with_root(
+00004a80: 6374 7829 3a0a 2020 2020 2020 2020 2020  ctx):.          
+00004a90: 2020 2020 2020 2020 2020 2320 6e6f 696e            # noin
+00004aa0: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
+00004ab0: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
+00004ac0: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+00004ad0: 6167 203d 2073 616d 655f 6261 7365 2e5f  ag = same_base._
+00004ae0: 6578 7472 612e 7361 6d65 5f66 6f72 5f62  extra.same_for_b
+00004af0: 6174 6368 5f63 7478 2e67 6574 2828 6261  atch_ctx.get((ba
+00004b00: 7463 685f 6261 7365 2c20 6374 785f 292c  tch_base, ctx_),
+00004b10: 204e 6f6e 6529 0a20 2020 2020 2020 2020   None).         
+00004b20: 2020 2020 2020 2020 2020 2069 6620 7461             if ta
+00004b30: 6720 616e 6420 7461 672e 5f63 616e 5f75  g and tag._can_u
+00004b40: 7365 5f69 6e5f 6374 7828 6374 7829 2061  se_in_ctx(ctx) a
+00004b50: 6e64 2074 6167 2e5f 7661 6c69 6461 7465  nd tag._validate
+00004b60: 5f69 6e5f 6375 7272 656e 745f 6772 6170  _in_current_grap
+00004b70: 6828 2920 616e 6420 7461 672e 6479 6e5f  h() and tag.dyn_
+00004b80: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
+00004b90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ba0: 2020 6261 7365 5f63 616e 5f75 7365 5f69    base_can_use_i
+00004bb0: 6e5f 6374 7820 3d20 7461 670a 2020 2020  n_ctx = tag.    
+00004bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004bd0: 2020 2020 6272 6561 6b0a 2020 2020 2020      break.      
+00004be0: 2020 2020 2020 6966 2062 6173 655f 6361        if base_ca
+00004bf0: 6e5f 7573 655f 696e 5f63 7478 2061 6e64  n_use_in_ctx and
+00004c00: 2062 6173 655f 6361 6e5f 7573 655f 696e   base_can_use_in
+00004c10: 5f63 7478 2e64 796e 5f73 697a 655f 6578  _ctx.dyn_size_ex
+00004c20: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00004c30: 2020 2069 6620 6261 7365 5f63 616e 5f75     if base_can_u
+00004c40: 7365 5f69 6e5f 6374 782e 6479 6e5f 7369  se_in_ctx.dyn_si
+00004c50: 7a65 5f65 7874 2e68 6176 655f 6261 7463  ze_ext.have_batc
+00004c60: 685f 6178 6973 2829 3a0a 2020 2020 2020  h_axis():.      
+00004c70: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00004c80: 5468 6520 7361 6d65 5f62 6173 6520 6861  The same_base ha
+00004c90: 7320 736f 6d65 2064 796e 2073 697a 6520  s some dyn size 
+00004ca0: 7769 7468 6f75 7420 616e 7920 6265 616d  without any beam
+00004cb0: 206e 6f72 2063 6f6e 7472 6f6c 2066 6c6f   nor control flo
+00004cc0: 7720 636f 6e74 6578 742e 0a20 2020 2020  w context..     
+00004cd0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00004ce0: 2057 6520 6361 6e20 6578 7061 6e64 2069   We can expand i
+00004cf0: 7420 746f 2074 6865 2063 7572 7265 6e74  t to the current
+00004d00: 2062 6561 6d2c 206f 7220 6578 7465 6e64   beam, or extend
+00004d10: 2062 7920 7061 6464 6564 2062 6174 6368   by padded batch
+00004d20: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00004d30: 2020 2020 2020 6479 6e5f 7369 7a65 5f65        dyn_size_e
+00004d40: 7874 203d 2062 6173 655f 6361 6e5f 7573  xt = base_can_us
+00004d50: 655f 696e 5f63 7478 2e64 796e 5f73 697a  e_in_ctx.dyn_siz
+00004d60: 655f 6578 742e 636f 7079 5f65 7874 656e  e_ext.copy_exten
+00004d70: 645f 6261 7463 6828 6261 7463 6829 0a20  d_batch(batch). 
+00004d80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004d90: 2020 2069 6620 6261 7463 682e 6265 616d     if batch.beam
+00004da0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00004db0: 2020 2020 2020 2020 2020 6479 6e5f 7369            dyn_si
+00004dc0: 7a65 5f65 7874 203d 2062 6173 655f 6361  ze_ext = base_ca
+00004dd0: 6e5f 7573 655f 696e 5f63 7478 2e64 796e  n_use_in_ctx.dyn
+00004de0: 5f73 697a 655f 6578 742e 636f 7079 5f65  _size_ext.copy_e
+00004df0: 7874 656e 645f 7769 7468 5f62 6561 6d28  xtend_with_beam(
+00004e00: 6261 7463 682e 6265 616d 290a 2020 2020  batch.beam).    
+00004e10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e20: 6173 7365 7274 2064 796e 5f73 697a 655f  assert dyn_size_
+00004e30: 6578 742e 6261 7463 6820 3d3d 2062 6174  ext.batch == bat
+00004e40: 6368 0a20 2020 2020 2020 2020 2020 2020  ch.             
+00004e50: 2020 2020 2020 2069 6620 6479 6e5f 7369         if dyn_si
+00004e60: 7a65 5f65 7874 2e70 6c61 6365 686f 6c64  ze_ext.placehold
+00004e70: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
+00004e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004e90: 2020 2020 2020 2020 6265 616d 5f65 7870          beam_exp
+00004ea0: 616e 6465 645f 6261 7365 5f64 6174 6120  anded_base_data 
+00004eb0: 3d20 6765 7461 7474 7228 0a20 2020 2020  = getattr(.     
+00004ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004ed0: 2020 2020 2020 2064 796e 5f73 697a 655f         dyn_size_
+00004ee0: 6578 742e 706c 6163 6568 6f6c 6465 722c  ext.placeholder,
+00004ef0: 2022 5f52 4554 5552 4e4e 5f62 6561 6d5f   "_RETURNN_beam_
+00004f00: 6578 7061 6e64 6564 5f62 6173 655f 6461  expanded_base_da
+00004f10: 7461 222c 204e 6f6e 650a 2020 2020 2020  ta", None.      
+00004f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f30: 2020 290a 2020 2020 2020 2020 2020 2020    ).            
+00004f40: 2020 2020 2020 2020 2020 2020 6966 2062              if b
+00004f50: 6174 6368 2e62 6561 6d3a 0a20 2020 2020  atch.beam:.     
+00004f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00004f70: 2020 2020 2020 2061 7373 6572 7420 6265         assert be
+00004f80: 616d 5f65 7870 616e 6465 645f 6261 7365  am_expanded_base
+00004f90: 5f64 6174 610a 2020 2020 2020 2020 2020  _data.          
+00004fa0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+00004fb0: 4e6f 7465 3a20 5468 6520 6265 616d 2065  Note: The beam e
+00004fc0: 7870 616e 7369 6f6e 2075 7365 6420 7469  xpansion used ti
+00004fd0: 6c69 6e67 2c20 7768 6963 6820 6361 6e20  ling, which can 
+00004fe0: 6265 2063 6163 6865 642e 0a20 2020 2020  be cached..     
+00004ff0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005000: 2020 2023 2054 6869 7320 6d65 616e 7320     # This means 
+00005010: 7468 6174 2077 6520 636f 756c 6420 656e  that we could en
+00005020: 6420 7570 2077 6974 6820 7468 6520 7361  d up with the sa
+00005030: 6d65 2073 697a 6520 7465 6e73 6f72 2028  me size tensor (
+00005040: 706c 6163 6568 6f6c 6465 7229 0a20 2020  placeholder).   
+00005050: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005060: 2020 2020 2023 2066 6f72 206d 756c 7469       # for multi
+00005070: 706c 6520 6469 6666 6572 656e 7420 6265  ple different be
+00005080: 616d 732c 0a20 2020 2020 2020 2020 2020  ams,.           
+00005090: 2020 2020 2020 2020 2020 2020 2023 2077               # w
+000050a0: 6865 6e20 7468 6572 6520 6172 6520 6469  hen there are di
+000050b0: 6666 6572 656e 7420 6265 616d 7320 7769  fferent beams wi
+000050c0: 7468 2073 616d 6520 6265 616d 2073 697a  th same beam siz
+000050d0: 6521 0a20 2020 2020 2020 2020 2020 2020  e!.             
+000050e0: 2020 2020 2020 2020 2020 2023 2054 6869             # Thi
+000050f0: 7320 6272 6561 6b73 2074 6865 2063 7572  s breaks the cur
+00005100: 7265 6e74 206c 6f67 6963 2069 6e20 6765  rent logic in ge
+00005110: 745f 7461 675f 6672 6f6d 5f73 697a 655f  t_tag_from_size_
+00005120: 7465 6e73 6f72 2e0a 2020 2020 2020 2020  tensor..        
 00005130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005140: 2020 2020 2020 2020 2020 2020 6479 6e5f              dyn_
-00005150: 7369 7a65 5f65 7874 2e70 6c61 6365 686f  size_ext.placeho
-00005160: 6c64 6572 203d 2074 662e 6964 656e 7469  lder = tf.identi
-00005170: 7479 280a 2020 2020 2020 2020 2020 2020  ty(.            
+00005140: 2320 4173 2061 2077 6f72 6b61 726f 756e  # As a workaroun
+00005150: 642c 2077 6520 6d61 6b65 2061 6e20 6578  d, we make an ex
+00005160: 706c 6963 6974 206e 6577 2074 656e 736f  plicit new tenso
+00005170: 7220 6865 7265 2e0a 2020 2020 2020 2020  r here..        
 00005180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005190: 2020 2020 6479 6e5f 7369 7a65 5f65 7874      dyn_size_ext
-000051a0: 2e70 6c61 6365 686f 6c64 6572 2c0a 2020  .placeholder,.  
+00005190: 696d 706f 7274 2074 656e 736f 7266 6c6f  import tensorflo
+000051a0: 7720 6173 2074 660a 2020 2020 2020 2020  w as tf.        
 000051b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000051c0: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-000051d0: 6d65 3d67 6574 5f76 616c 6964 5f73 636f  me=get_valid_sco
-000051e0: 7065 5f6e 616d 655f 6672 6f6d 5f73 7472  pe_name_from_str
-000051f0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00005200: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005210: 2020 2020 2020 2225 735f 6765 745f 666f        "%s_get_fo
-00005220: 725f 6261 7463 685f 6374 785f 2573 2220  r_batch_ctx_%s" 
-00005230: 2520 2864 796e 5f73 697a 655f 6578 742e  % (dyn_size_ext.
-00005240: 6e61 6d65 2c20 6261 7463 682e 7368 6f72  name, batch.shor
-00005250: 745f 7265 7072 2829 290a 2020 2020 2020  t_repr()).      
-00005260: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005270: 2020 2020 2020 2020 2020 292c 0a20 2020            ),.   
-00005280: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005290: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-000052a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000052b0: 2020 2069 6620 6261 7463 682e 6265 616d     if batch.beam
-000052c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000052d0: 2020 2020 2020 2020 2020 2020 2020 6479                dy
-000052e0: 6e5f 7369 7a65 5f65 7874 2e70 6c61 6365  n_size_ext.place
-000052f0: 686f 6c64 6572 2e5f 5245 5455 524e 4e5f  holder._RETURNN_
-00005300: 6479 6e5f 7369 7a65 5f62 6561 6d20 3d20  dyn_size_beam = 
-00005310: 6261 7463 682e 6265 616d 0a20 2020 2020  batch.beam.     
-00005320: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005330: 2020 2020 2020 2064 796e 5f73 697a 655f         dyn_size_
-00005340: 6578 742e 706c 6163 6568 6f6c 6465 722e  ext.placeholder.
-00005350: 5f52 4554 5552 4e4e 5f62 6561 6d5f 6578  _RETURNN_beam_ex
-00005360: 7061 6e64 6564 5f62 6173 655f 6461 7461  panded_base_data
-00005370: 203d 2062 6561 6d5f 6578 7061 6e64 6564   = beam_expanded
-00005380: 5f62 6173 655f 6461 7461 0a20 2020 2020  _base_data.     
-00005390: 2020 2069 6620 6e6f 7420 6479 6e5f 7369     if not dyn_si
-000053a0: 7a65 5f65 7874 2061 6e64 2061 6c6c 6f77  ze_ext and allow
-000053b0: 5f6e 6f6e 6520 616e 6420 6e6f 7420 7361  _none and not sa
-000053c0: 6d65 5f62 6173 652e 6465 7269 7665 645f  me_base.derived_
-000053d0: 6672 6f6d 5f6f 703a 0a20 2020 2020 2020  from_op:.       
-000053e0: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
-000053f0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00005400: 6479 6e5f 7369 7a65 5f65 7874 2061 6e64  dyn_size_ext and
-00005410: 2073 616d 655f 6261 7365 5f65 7874 7261   same_base_extra
-00005420: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
-00005430: 6374 783a 0a20 2020 2020 2020 2020 2020  ctx:.           
-00005440: 2023 2054 6865 7265 2061 7265 2065 6172   # There are ear
-00005450: 6c69 6572 2065 6e74 7269 6573 2069 6e20  lier entries in 
-00005460: 5f73 616d 655f 666f 725f 6261 7463 685f  _same_for_batch_
-00005470: 6374 780a 2020 2020 2020 2020 2020 2020  ctx.            
-00005480: 2320 2d2d 206d 6179 6265 2077 6520 6361  # -- maybe we ca
-00005490: 6e20 696e 6665 7220 6479 6e5f 7369 7a65  n infer dyn_size
-000054a0: 5f65 7874 2c20 6576 656e 2077 6974 6820  _ext, even with 
-000054b0: 6469 6666 6572 656e 7420 6261 7463 682e  different batch.
-000054c0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-000054d0: 2028 6261 7463 685f 2c20 6374 785f 292c   (batch_, ctx_),
-000054e0: 206f 7468 6572 2069 6e20 7361 6d65 5f62   other in same_b
-000054f0: 6173 655f 6578 7472 612e 7361 6d65 5f66  ase_extra.same_f
-00005500: 6f72 5f62 6174 6368 5f63 7478 2e69 7465  or_batch_ctx.ite
-00005510: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-00005520: 2020 2020 2020 6966 2063 7478 5f20 3d3d        if ctx_ ==
-00005530: 2063 7478 2061 6e64 206f 7468 6572 2e64   ctx and other.d
-00005540: 796e 5f73 697a 655f 6578 743a 0a20 2020  yn_size_ext:.   
-00005550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005560: 2064 796e 5f73 697a 655f 6578 7420 3d20   dyn_size_ext = 
-00005570: 6f74 6865 722e 6479 6e5f 7369 7a65 5f65  other.dyn_size_e
-00005580: 7874 2e63 6f70 795f 7465 6d70 6c61 7465  xt.copy_template
-00005590: 2829 0a20 2020 2020 2020 2020 2020 2020  ().             
-000055a0: 2020 2020 2020 2064 796e 5f73 697a 655f         dyn_size_
-000055b0: 6578 742e 6265 616d 203d 2062 6174 6368  ext.beam = batch
-000055c0: 2e62 6561 6d0a 2020 2020 2020 2020 2020  .beam.          
-000055d0: 2020 2020 2020 2020 2020 6479 6e5f 7369            dyn_si
-000055e0: 7a65 5f65 7874 2e62 6174 6368 203d 2062  ze_ext.batch = b
-000055f0: 6174 6368 0a20 2020 2020 2020 2020 2020  atch.           
-00005600: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
-00005610: 2020 2020 2020 2063 7478 203d 2064 796e         ctx = dyn
-00005620: 5f73 697a 655f 6578 742e 636f 6e74 726f  _size_ext.contro
-00005630: 6c5f 666c 6f77 5f63 7478 2069 6620 6479  l_flow_ctx if dy
-00005640: 6e5f 7369 7a65 5f65 7874 2065 6c73 6520  n_size_ext else 
-00005650: 6374 780a 2020 2020 2020 2020 6469 6d5f  ctx.        dim_
-00005660: 7461 6720 3d20 4e6f 6e65 0a20 2020 2020  tag = None.     
-00005670: 2020 2066 6f72 2063 616e 6469 6461 7465     for candidate
-00005680: 2069 6e20 5b73 656c 662c 2073 616d 655f   in [self, same_
-00005690: 6261 7365 5d3a 0a20 2020 2020 2020 2020  base]:.         
-000056a0: 2020 2069 6620 280a 2020 2020 2020 2020     if (.        
-000056b0: 2020 2020 2020 2020 2863 616e 6469 6461          (candida
-000056c0: 7465 2e62 6174 6368 203d 3d20 6261 7463  te.batch == batc
-000056d0: 6820 6f72 2028 6e6f 7420 6361 6e64 6964  h or (not candid
-000056e0: 6174 652e 6261 7463 6820 616e 6420 6261  ate.batch and ba
-000056f0: 7463 682e 6973 5f67 6c6f 6261 6c5f 6261  tch.is_global_ba
-00005700: 7463 6828 2929 290a 2020 2020 2020 2020  tch())).        
-00005710: 2020 2020 2020 2020 616e 6420 6e6f 7420          and not 
-00005720: 6361 6e64 6964 6174 652e 636f 6e74 726f  candidate.contro
-00005730: 6c5f 666c 6f77 5f63 7478 0a20 2020 2020  l_flow_ctx.     
-00005740: 2020 2020 2020 2020 2020 2061 6e64 206e             and n
-00005750: 6f74 2063 7478 0a20 2020 2020 2020 2020  ot ctx.         
-00005760: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
-00005770: 2020 2020 2020 2320 5468 6520 7361 6d65        # The same
-00005780: 5f62 6173 6520 696e 7374 616e 6365 2069  _base instance i
-00005790: 7320 6569 7468 6572 2075 6e64 6566 696e  s either undefin
-000057a0: 6564 2028 6e6f 2062 6174 6368 2c20 6e6f  ed (no batch, no
-000057b0: 2063 7478 290a 2020 2020 2020 2020 2020   ctx).          
-000057c0: 2020 2020 2020 2320 6f72 2069 7420 6973        # or it is
-000057d0: 2064 6566 696e 6564 2066 6f72 2074 6865   defined for the
-000057e0: 2073 616d 6520 6261 7463 6820 616e 6420   same batch and 
-000057f0: 6374 782e 0a20 2020 2020 2020 2020 2020  ctx..           
-00005800: 2020 2020 2023 2049 6e20 616e 7920 6361       # In any ca
-00005810: 7365 2c20 7265 7573 6520 6974 2074 6865  se, reuse it the
-00005820: 6e2e 0a20 2020 2020 2020 2020 2020 2020  n..             
-00005830: 2020 2063 616e 6469 6461 7465 2e62 6174     candidate.bat
-00005840: 6368 203d 2062 6174 6368 0a20 2020 2020  ch = batch.     
-00005850: 2020 2020 2020 2020 2020 2069 6620 6479             if dy
-00005860: 6e5f 7369 7a65 5f65 7874 3a0a 2020 2020  n_size_ext:.    
-00005870: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005880: 6966 2063 616e 6469 6461 7465 2e64 796e  if candidate.dyn
-00005890: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
-000058a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058b0: 2020 2063 616e 6469 6461 7465 2e64 796e     candidate.dyn
-000058c0: 5f73 697a 655f 6578 742e 6261 7463 6820  _size_ext.batch 
-000058d0: 3d20 6261 7463 680a 2020 2020 2020 2020  = batch.        
-000058e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000058f0: 6173 7365 7274 2063 616e 6469 6461 7465  assert candidate
-00005900: 2e64 796e 5f73 697a 655f 6578 742e 6469  .dyn_size_ext.di
-00005910: 6d5f 7461 6773 203d 3d20 6479 6e5f 7369  m_tags == dyn_si
-00005920: 7a65 5f65 7874 2e64 696d 5f74 6167 730a  ze_ext.dim_tags.
-00005930: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005940: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00005950: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005960: 2020 6361 6e64 6964 6174 652e 6479 6e5f    candidate.dyn_
-00005970: 7369 7a65 5f65 7874 203d 2064 796e 5f73  size_ext = dyn_s
-00005980: 697a 655f 6578 740a 2020 2020 2020 2020  ize_ext.        
-00005990: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-000059a0: 7274 206e 6f74 2063 616e 6469 6461 7465  rt not candidate
-000059b0: 2e64 796e 5f73 697a 655f 6578 742e 636f  .dyn_size_ext.co
-000059c0: 6e74 726f 6c5f 666c 6f77 5f63 7478 0a20  ntrol_flow_ctx. 
-000059d0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-000059e0: 6c69 6620 6361 6e64 6964 6174 652e 6479  lif candidate.dy
-000059f0: 6e5f 7369 7a65 5f65 7874 3a0a 2020 2020  n_size_ext:.    
-00005a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005a10: 6361 6e64 6964 6174 652e 6479 6e5f 7369  candidate.dyn_si
-00005a20: 7a65 5f65 7874 2e62 6174 6368 203d 2062  ze_ext.batch = b
-00005a30: 6174 6368 0a20 2020 2020 2020 2020 2020  atch.           
-00005a40: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00005a50: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-00005a60: 616e 6469 6461 7465 2e63 6f6d 706c 6574  andidate.complet
-00005a70: 655f 6479 6e5f 7369 7a65 2874 656d 706c  e_dyn_size(templ
-00005a80: 6174 655f 6f6e 6c79 3d54 7275 6529 0a20  ate_only=True). 
-00005a90: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00005aa0: 696d 5f74 6167 203d 2063 616e 6469 6461  im_tag = candida
-00005ab0: 7465 0a20 2020 2020 2020 2020 2020 2020  te.             
-00005ac0: 2020 2062 7265 616b 0a20 2020 2020 2020     break.       
-00005ad0: 2069 6620 6e6f 7420 6469 6d5f 7461 673a   if not dim_tag:
-00005ae0: 0a20 2020 2020 2020 2020 2020 2064 696d  .            dim
-00005af0: 5f74 6167 203d 205f 642e 4469 6d28 0a20  _tag = _d.Dim(. 
-00005b00: 2020 2020 2020 2020 2020 2020 2020 206b                 k
-00005b10: 696e 643d 7365 6c66 2e6b 696e 642c 0a20  ind=self.kind,. 
-00005b20: 2020 2020 2020 2020 2020 2020 2020 2064                 d
-00005b30: 6573 6372 6970 7469 6f6e 3d73 656c 662e  escription=self.
-00005b40: 6465 7363 7269 7074 696f 6e2c 0a20 2020  description,.   
-00005b50: 2020 2020 2020 2020 2020 2020 2064 696d               dim
-00005b60: 656e 7369 6f6e 3d73 656c 662e 6469 6d65  ension=self.dime
-00005b70: 6e73 696f 6e2c 0a20 2020 2020 2020 2020  nsion,.         
-00005b80: 2020 2020 2020 2061 7574 6f5f 6765 6e65         auto_gene
-00005b90: 7261 7465 643d 7365 6c66 2e61 7574 6f5f  rated=self.auto_
-00005ba0: 6765 6e65 7261 7465 642c 0a20 2020 2020  generated,.     
-00005bb0: 2020 2020 2020 2020 2020 2062 6174 6368             batch
-00005bc0: 3d62 6174 6368 2c0a 2020 2020 2020 2020  =batch,.        
-00005bd0: 2020 2020 2020 2020 636f 6e74 726f 6c5f          control_
-00005be0: 666c 6f77 5f63 7478 3d63 7478 2c0a 2020  flow_ctx=ctx,.  
-00005bf0: 2020 2020 2020 2020 2020 2020 2020 6479                dy
-00005c00: 6e5f 7369 7a65 5f65 7874 3d64 796e 5f73  n_size_ext=dyn_s
-00005c10: 697a 655f 6578 742c 0a20 2020 2020 2020  ize_ext,.       
-00005c20: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00005c30: 2020 2064 696d 5f74 6167 2e73 616d 655f     dim_tag.same_
-00005c40: 6173 203d 2073 616d 655f 6261 7365 0a20  as = same_base. 
-00005c50: 2020 2020 2020 2069 6620 6479 6e5f 7369         if dyn_si
-00005c60: 7a65 5f65 7874 2061 6e64 2064 796e 5f73  ze_ext and dyn_s
-00005c70: 697a 655f 6578 742e 706c 6163 6568 6f6c  ize_ext.placehol
-00005c80: 6465 7220 6973 206e 6f74 204e 6f6e 653a  der is not None:
-00005c90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00005ca0: 5f64 2e44 696d 2e67 6574 5f74 6167 5f66  _d.Dim.get_tag_f
-00005cb0: 726f 6d5f 7369 7a65 5f74 656e 736f 7228  rom_size_tensor(
-00005cc0: 6479 6e5f 7369 7a65 5f65 7874 2e70 6c61  dyn_size_ext.pla
-00005cd0: 6365 686f 6c64 6572 2920 6973 204e 6f6e  ceholder) is Non
-00005ce0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-00005cf0: 2020 2064 696d 5f74 6167 2e73 6574 5f74     dim_tag.set_t
-00005d00: 6167 5f6f 6e5f 7369 7a65 5f74 656e 736f  ag_on_size_tenso
-00005d10: 7228 6479 6e5f 7369 7a65 5f65 7874 2e70  r(dyn_size_ext.p
-00005d20: 6c61 6365 686f 6c64 6572 2c20 6261 7463  laceholder, batc
-00005d30: 683d 6261 7463 6829 0a20 2020 2020 2020  h=batch).       
-00005d40: 2073 616d 655f 6261 7365 5f65 7874 7261   same_base_extra
-00005d50: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
-00005d60: 6374 785b 2862 6174 6368 2c20 6374 7829  ctx[(batch, ctx)
-00005d70: 5d20 3d20 6469 6d5f 7461 670a 2020 2020  ] = dim_tag.    
-00005d80: 2020 2020 6469 6d5f 7461 672e 636f 6d70      dim_tag.comp
-00005d90: 6c65 7465 5f64 796e 5f73 697a 6528 7465  lete_dyn_size(te
-00005da0: 6d70 6c61 7465 5f6f 6e6c 793d 5472 7565  mplate_only=True
-00005db0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-00005dc0: 2064 696d 5f74 6167 0a0a 2020 2020 6465   dim_tag..    de
-00005dd0: 6620 7265 7365 745f 6261 7463 685f 6374  f reset_batch_ct
-00005de0: 7828 7365 6c66 3a20 4469 6d29 3a0a 2020  x(self: Dim):.  
-00005df0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00005e00: 2020 466f 7220 7468 6520 7365 6c66 2069    For the self i
-00005e10: 6e73 7461 6e63 652c 2072 6573 6574 2062  nstance, reset b
-00005e20: 6174 6368 2061 6e64 2063 6f6e 7465 7874  atch and context
-00005e30: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00005e40: 2020 2020 2020 6966 2073 656c 662e 5f65        if self._e
-00005e50: 7874 7261 3a0a 2020 2020 2020 2020 2020  xtra:.          
-00005e60: 2020 7365 6c66 2e5f 6578 7472 612e 7361    self._extra.sa
-00005e70: 6d65 5f66 6f72 5f62 6174 6368 5f63 7478  me_for_batch_ctx
-00005e80: 2e70 6f70 2828 7365 6c66 2e62 6174 6368  .pop((self.batch
-00005e90: 2c20 7365 6c66 2e63 6f6e 7472 6f6c 5f66  , self.control_f
-00005ea0: 6c6f 775f 6374 7829 2c20 4e6f 6e65 290a  low_ctx), None).
-00005eb0: 2020 2020 2020 2020 7365 6c66 2e62 6174          self.bat
-00005ec0: 6368 203d 204e 6f6e 650a 2020 2020 2020  ch = None.      
-00005ed0: 2020 7365 6c66 2e63 6f6e 7472 6f6c 5f66    self.control_f
-00005ee0: 6c6f 775f 6374 7820 3d20 4e6f 6e65 0a20  low_ctx = None. 
-00005ef0: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-00005f00: 796e 5f73 697a 655f 6578 7420 616e 6420  yn_size_ext and 
-00005f10: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
-00005f20: 742e 6261 7463 683a 0a20 2020 2020 2020  t.batch:.       
-00005f30: 2020 2020 2073 656c 662e 6479 6e5f 7369       self.dyn_si
-00005f40: 7a65 5f65 7874 203d 2073 656c 662e 6479  ze_ext = self.dy
-00005f50: 6e5f 7369 7a65 5f65 7874 2e63 6f70 795f  n_size_ext.copy_
-00005f60: 7465 6d70 6c61 7465 2829 0a20 2020 2020  template().     
-00005f70: 2020 2020 2020 2073 656c 662e 6479 6e5f         self.dyn_
-00005f80: 7369 7a65 5f65 7874 2e62 6174 6368 203d  size_ext.batch =
-00005f90: 204e 6f6e 650a 0a20 2020 2064 6566 2073   None..    def s
-00005fa0: 6574 5f64 796e 5f73 697a 655f 6578 745f  et_dyn_size_ext_
-00005fb0: 666f 725f 6261 7463 685f 6374 7828 7365  for_batch_ctx(se
-00005fc0: 6c66 2c20 6261 7463 682c 2063 7478 2c20  lf, batch, ctx, 
-00005fd0: 6479 6e5f 7369 7a65 5f65 7874 293a 0a20  dyn_size_ext):. 
-00005fe0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00005ff0: 2020 203a 7061 7261 6d20 4261 7463 6849     :param BatchI
-00006000: 6e66 6f20 6261 7463 683a 0a20 2020 2020  nfo batch:.     
-00006010: 2020 203a 7061 7261 6d20 436f 6e74 726f     :param Contro
-00006020: 6c46 6c6f 7743 6f6e 7465 7874 7c4e 6f6e  lFlowContext|Non
-00006030: 6520 6374 783a 0a20 2020 2020 2020 203a  e ctx:.        :
-00006040: 7061 7261 6d20 4461 7461 2064 796e 5f73  param Data dyn_s
-00006050: 697a 655f 6578 743a 0a20 2020 2020 2020  ize_ext:.       
-00006060: 2022 2222 0a20 2020 2020 2020 2061 7373   """.        ass
-00006070: 6572 7420 7365 6c66 2e63 616e 5f62 655f  ert self.can_be_
-00006080: 7573 6564 5f61 735f 6469 6d28 290a 2020  used_as_dim().  
-00006090: 2020 2020 2020 7361 6d65 203d 2073 656c        same = sel
-000060a0: 662e 6765 745f 666f 725f 6261 7463 685f  f.get_for_batch_
-000060b0: 6374 7828 6261 7463 682c 2063 7478 290a  ctx(batch, ctx).
-000060c0: 2020 2020 2020 2020 6173 7365 7274 2064          assert d
-000060d0: 796e 5f73 697a 655f 6578 742e 6261 7463  yn_size_ext.batc
-000060e0: 6820 3d3d 2062 6174 6368 2061 6e64 2064  h == batch and d
-000060f0: 796e 5f73 697a 655f 6578 742e 636f 6e74  yn_size_ext.cont
-00006100: 726f 6c5f 666c 6f77 5f63 7478 203d 3d20  rol_flow_ctx == 
-00006110: 6374 780a 2020 2020 2020 2020 6966 2073  ctx.        if s
-00006120: 616d 652e 6479 6e5f 7369 7a65 5f65 7874  ame.dyn_size_ext
-00006130: 3a0a 2020 2020 2020 2020 2020 2020 6173  :.            as
-00006140: 7365 7274 2073 616d 652e 6479 6e5f 7369  sert same.dyn_si
-00006150: 7a65 5f65 7874 2e64 696d 5f74 6167 7320  ze_ext.dim_tags 
-00006160: 3d3d 2064 796e 5f73 697a 655f 6578 742e  == dyn_size_ext.
-00006170: 6469 6d5f 7461 6773 0a20 2020 2020 2020  dim_tags.       
-00006180: 2020 2020 2069 6620 6479 6e5f 7369 7a65       if dyn_size
-00006190: 5f65 7874 2e70 6c61 6365 686f 6c64 6572  _ext.placeholder
-000061a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000061b0: 2020 2020 2020 2020 2020 2020 2020 7361                sa
-000061c0: 6d65 2e64 796e 5f73 697a 655f 6578 742e  me.dyn_size_ext.
-000061d0: 706c 6163 6568 6f6c 6465 7220 3d20 6479  placeholder = dy
-000061e0: 6e5f 7369 7a65 5f65 7874 2e70 6c61 6365  n_size_ext.place
-000061f0: 686f 6c64 6572 0a20 2020 2020 2020 2065  holder.        e
-00006200: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-00006210: 2073 616d 652e 6479 6e5f 7369 7a65 5f65   same.dyn_size_e
-00006220: 7874 203d 2064 796e 5f73 697a 655f 6578  xt = dyn_size_ex
-00006230: 740a 2020 2020 2020 2020 7365 6c66 2e5f  t.        self._
-00006240: 6d61 7962 655f 7570 6461 7465 2829 0a0a  maybe_update()..
-00006250: 2020 2020 6465 6620 6765 745f 6479 6e5f      def get_dyn_
-00006260: 7369 7a65 5f65 7874 5f66 6f72 5f62 6174  size_ext_for_bat
-00006270: 6368 5f63 7478 2873 656c 662c 2062 6174  ch_ctx(self, bat
-00006280: 6368 2c20 6374 782c 2074 656d 706c 6174  ch, ctx, templat
-00006290: 655f 6f6e 6c79 3d46 616c 7365 293a 0a20  e_only=False):. 
-000062a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000062b0: 2020 203a 7061 7261 6d20 4261 7463 6849     :param BatchI
-000062c0: 6e66 6f7c 4e6f 6e65 2062 6174 6368 3a0a  nfo|None batch:.
-000062d0: 2020 2020 2020 2020 3a70 6172 616d 2043          :param C
-000062e0: 6f6e 7472 6f6c 466c 6f77 436f 6e74 6578  ontrolFlowContex
-000062f0: 747c 4e6f 6e65 2063 7478 3a0a 2020 2020  t|None ctx:.    
-00006300: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
-00006310: 7465 6d70 6c61 7465 5f6f 6e6c 793a 0a20  template_only:. 
-00006320: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-00006330: 6174 617c 4e6f 6e65 0a20 2020 2020 2020  ata|None.       
-00006340: 2022 2222 0a20 2020 2020 2020 2061 7373   """.        ass
-00006350: 6572 7420 7365 6c66 2e63 616e 5f62 655f  ert self.can_be_
-00006360: 7573 6564 5f61 735f 6469 6d28 290a 2020  used_as_dim().  
-00006370: 2020 2020 2020 6966 206e 6f74 2062 6174        if not bat
-00006380: 6368 2061 6e64 2073 656c 662e 6261 7463  ch and self.batc
-00006390: 683a 0a20 2020 2020 2020 2020 2020 2023  h:.            #
-000063a0: 2041 7373 756d 6520 676c 6f62 616c 2062   Assume global b
-000063b0: 6174 6368 2e0a 2020 2020 2020 2020 2020  atch..          
-000063c0: 2020 6261 7463 6820 3d20 7365 6c66 2e62    batch = self.b
-000063d0: 6174 6368 2e67 6574 5f67 6c6f 6261 6c5f  atch.get_global_
-000063e0: 6261 7365 2829 0a20 2020 2020 2020 2069  base().        i
-000063f0: 6620 6e6f 7420 6261 7463 683a 0a20 2020  f not batch:.   
-00006400: 2020 2020 2020 2020 2023 2054 6869 7320           # This 
-00006410: 6973 2075 7375 616c 6c79 206e 6f74 2076  is usually not v
-00006420: 616c 6964 2e20 486f 7765 7665 722c 2074  alid. However, t
-00006430: 6869 7320 6361 7365 2063 616e 2068 6170  his case can hap
-00006440: 7065 6e20 6561 726c 7920 6174 2069 6e69  pen early at ini
-00006450: 7469 616c 697a 6174 696f 6e2e 0a20 2020  tialization..   
-00006460: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-00006470: 6261 7463 6820 3d3d 2073 656c 662e 6261  batch == self.ba
-00006480: 7463 6820 616e 6420 6374 7820 3d3d 2073  tch and ctx == s
-00006490: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
-000064a0: 5f63 7478 0a20 2020 2020 2020 2020 2020  _ctx.           
-000064b0: 2072 6574 7572 6e20 7365 6c66 2e64 796e   return self.dyn
-000064c0: 5f73 697a 655f 6578 740a 2020 2020 2020  _size_ext.      
-000064d0: 2020 7361 6d65 203d 2073 656c 662e 6765    same = self.ge
-000064e0: 745f 666f 725f 6261 7463 685f 6374 7828  t_for_batch_ctx(
-000064f0: 6261 7463 682c 2063 7478 2c20 616c 6c6f  batch, ctx, allo
-00006500: 775f 6e6f 6e65 3d54 7275 6529 0a20 2020  w_none=True).   
-00006510: 2020 2020 2069 6620 6e6f 7420 7361 6d65       if not same
-00006520: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00006530: 7475 726e 204e 6f6e 650a 2020 2020 2020  turn None.      
-00006540: 2020 7361 6d65 2e63 6f6d 706c 6574 655f    same.complete_
-00006550: 6479 6e5f 7369 7a65 2874 656d 706c 6174  dyn_size(templat
-00006560: 655f 6f6e 6c79 3d74 656d 706c 6174 655f  e_only=template_
-00006570: 6f6e 6c79 290a 2020 2020 2020 2020 7265  only).        re
-00006580: 7475 726e 2073 616d 652e 6479 6e5f 7369  turn same.dyn_si
-00006590: 7a65 5f65 7874 0a0a 2020 2020 4070 726f  ze_ext..    @pro
-000065a0: 7065 7274 790a 2020 2020 6465 6620 6479  perty.    def dy
-000065b0: 6e5f 7369 7a65 2873 656c 6629 3a0a 2020  n_size(self):.  
-000065c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000065d0: 2020 3a72 6574 7572 6e3a 2064 796e 2073    :return: dyn s
-000065e0: 697a 6520 2f20 7365 7120 6c65 6e20 2875  ize / seq len (u
-000065f0: 7375 616c 6c79 206f 6620 7368 6170 6520  sually of shape 
-00006600: 5b42 5d29 2c20 6f72 204e 6f6e 650a 2020  [B]), or None.  
-00006610: 2020 2020 2020 2020 4966 2074 6865 2064          If the d
-00006620: 796e 2073 697a 6520 6361 6e20 706f 7465  yn size can pote
-00006630: 6e74 6961 6c6c 7920 6265 206f 6620 6120  ntially be of a 
-00006640: 6469 6666 6572 656e 7420 7368 6170 652c  different shape,
-00006650: 2064 6972 6563 746c 7920 6163 6365 7373   directly access
-00006660: 2064 796e 5f73 697a 655f 6578 742e 0a20   dyn_size_ext.. 
-00006670: 2020 2020 2020 203a 7274 7970 653a 2074         :rtype: t
-00006680: 662e 5465 6e73 6f72 7c4e 6f6e 650a 2020  f.Tensor|None.  
-00006690: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000066a0: 2020 6966 2073 656c 662e 6479 6e5f 7369    if self.dyn_si
-000066b0: 7a65 5f65 7874 3a0a 2020 2020 2020 2020  ze_ext:.        
-000066c0: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-000066d0: 6479 6e5f 7369 7a65 5f65 7874 2e70 6c61  dyn_size_ext.pla
-000066e0: 6365 686f 6c64 6572 0a20 2020 2020 2020  ceholder.       
-000066f0: 2072 6574 7572 6e20 4e6f 6e65 0a0a 2020   return None..  
-00006700: 2020 4064 796e 5f73 697a 652e 7365 7474    @dyn_size.sett
-00006710: 6572 0a20 2020 2064 6566 2064 796e 5f73  er.    def dyn_s
-00006720: 697a 6528 7365 6c66 2c20 6479 6e5f 7369  ize(self, dyn_si
-00006730: 7a65 293a 0a20 2020 2020 2020 2022 2222  ze):.        """
-00006740: 0a20 2020 2020 2020 2041 6c73 6f20 7365  .        Also se
-00006750: 6520 3a66 756e 633a 6073 6574 5f64 796e  e :func:`set_dyn
-00006760: 5f73 697a 655f 6578 745f 666f 725f 6261  _size_ext_for_ba
-00006770: 7463 685f 6374 7860 2e0a 0a20 2020 2020  tch_ctx`...     
-00006780: 2020 203a 7061 7261 6d20 7466 2e54 656e     :param tf.Ten
-00006790: 736f 7220 6479 6e5f 7369 7a65 3a0a 2020  sor dyn_size:.  
-000067a0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-000067b0: 2020 6966 2073 656c 662e 6479 6e5f 7369    if self.dyn_si
-000067c0: 7a65 5f65 7874 2061 6e64 2073 656c 662e  ze_ext and self.
-000067d0: 6479 6e5f 7369 7a65 5f65 7874 2e70 6c61  dyn_size_ext.pla
-000067e0: 6365 686f 6c64 6572 2069 7320 6479 6e5f  ceholder is dyn_
-000067f0: 7369 7a65 3a20 2023 2066 6173 7420 7061  size:  # fast pa
-00006800: 7468 2063 6865 636b 0a20 2020 2020 2020  th check.       
-00006810: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-00006820: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
-00006830: 6361 6e5f 6265 5f75 7365 645f 6173 5f64  can_be_used_as_d
-00006840: 696d 2829 0a20 2020 2020 2020 206f 7468  im().        oth
-00006850: 6572 203d 205f 642e 4469 6d2e 6765 745f  er = _d.Dim.get_
-00006860: 7461 675f 6672 6f6d 5f73 697a 655f 7465  tag_from_size_te
-00006870: 6e73 6f72 2864 796e 5f73 697a 6529 0a20  nsor(dyn_size). 
-00006880: 2020 2020 2020 2069 6620 6f74 6865 723a         if other:
-00006890: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-000068a0: 662e 6465 636c 6172 655f 7361 6d65 5f61  f.declare_same_a
-000068b0: 7328 6f74 6865 7229 0a20 2020 2020 2020  s(other).       
-000068c0: 2020 2020 2069 6620 7365 6c66 2e62 6174       if self.bat
-000068d0: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
-000068e0: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
-000068f0: 6261 7463 6820 3d3d 206f 7468 6572 2e62  batch == other.b
-00006900: 6174 6368 2061 6e64 2073 656c 662e 636f  atch and self.co
-00006910: 6e74 726f 6c5f 666c 6f77 5f63 7478 203d  ntrol_flow_ctx =
-00006920: 3d20 6f74 6865 722e 636f 6e74 726f 6c5f  = other.control_
-00006930: 666c 6f77 5f63 7478 0a20 2020 2020 2020  flow_ctx.       
-00006940: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-00006950: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-00006960: 6261 7463 6820 3d20 6f74 6865 722e 6261  batch = other.ba
-00006970: 7463 680a 2020 2020 2020 2020 2020 2020  tch.            
-00006980: 2020 2020 7365 6c66 2e63 6f6e 7472 6f6c      self.control
-00006990: 5f66 6c6f 775f 6374 7820 3d20 6f74 6865  _flow_ctx = othe
-000069a0: 722e 636f 6e74 726f 6c5f 666c 6f77 5f63  r.control_flow_c
-000069b0: 7478 0a20 2020 2020 2020 2020 2020 2073  tx.            s
-000069c0: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-000069d0: 203d 206f 7468 6572 2e64 796e 5f73 697a   = other.dyn_siz
-000069e0: 655f 6578 740a 2020 2020 2020 2020 2020  e_ext.          
-000069f0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00006a00: 2073 656c 662e 5f69 6e69 745f 6465 6661   self._init_defa
-00006a10: 756c 745f 6479 6e5f 7369 7a65 5f65 7874  ult_dyn_size_ext
-00006a20: 2864 796e 5f73 697a 6529 0a20 2020 2020  (dyn_size).     
-00006a30: 2020 2073 656c 662e 7365 745f 7461 675f     self.set_tag_
-00006a40: 6f6e 5f73 697a 655f 7465 6e73 6f72 2864  on_size_tensor(d
-00006a50: 796e 5f73 697a 6529 0a0a 2020 2020 6465  yn_size)..    de
-00006a60: 6620 5f69 6e69 745f 6465 6661 756c 745f  f _init_default_
-00006a70: 6479 6e5f 7369 7a65 5f65 7874 2873 656c  dyn_size_ext(sel
-00006a80: 662c 2064 796e 5f73 697a 6529 3a0a 2020  f, dyn_size):.  
-00006a90: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00006aa0: 2020 3a70 6172 616d 2074 662e 5465 6e73    :param tf.Tens
-00006ab0: 6f72 2064 796e 5f73 697a 653a 0a20 2020  or dyn_size:.   
-00006ac0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00006ad0: 2069 6620 7365 6c66 2e64 796e 5f73 697a   if self.dyn_siz
-00006ae0: 655f 6578 743a 0a20 2020 2020 2020 2020  e_ext:.         
-00006af0: 2020 2069 6620 7365 6c66 2e64 796e 5f73     if self.dyn_s
-00006b00: 697a 655f 6578 742e 706c 6163 6568 6f6c  ize_ext.placehol
-00006b10: 6465 7220 6973 206e 6f74 204e 6f6e 653a  der is not None:
-00006b20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006b30: 2023 2044 6f20 6e6f 7420 616c 6c6f 7720   # Do not allow 
-00006b40: 7265 7365 7474 696e 6720 6974 2074 6f20  resetting it to 
-00006b50: 7374 6820 6469 6666 6572 656e 742e 0a20  sth different.. 
-00006b60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00006b70: 7373 6572 7420 7365 6c66 2e64 796e 5f73  ssert self.dyn_s
-00006b80: 697a 655f 6578 742e 706c 6163 6568 6f6c  ize_ext.placehol
-00006b90: 6465 7220 6973 2064 796e 5f73 697a 650a  der is dyn_size.
-00006ba0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-00006bb0: 2020 2020 2020 2020 2020 6265 616d 203d            beam =
-00006bc0: 2067 6574 6174 7472 2864 796e 5f73 697a   getattr(dyn_siz
-00006bd0: 652c 2022 5f52 4554 5552 4e4e 5f64 796e  e, "_RETURNN_dyn
-00006be0: 5f73 697a 655f 6265 616d 222c 204e 6f6e  _size_beam", Non
-00006bf0: 6529 0a20 2020 2020 2020 2020 2020 2073  e).            s
-00006c00: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-00006c10: 203d 205f 742e 5465 6e73 6f72 280a 2020   = _t.Tensor(.  
-00006c20: 2020 2020 2020 2020 2020 2020 2020 6e61                na
-00006c30: 6d65 3d28 2225 733a 6479 6e5f 7369 7a65  me=("%s:dyn_size
-00006c40: 2220 2520 7365 6c66 2e64 6573 6372 6970  " % self.descrip
-00006c50: 7469 6f6e 2920 6966 2073 656c 662e 6465  tion) if self.de
-00006c60: 7363 7269 7074 696f 6e20 656c 7365 2064  scription else d
-00006c70: 796e 5f73 697a 652e 6f70 2e6e 616d 652c  yn_size.op.name,
-00006c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00006c90: 2064 7479 7065 3d5f 742e 5465 6e73 6f72   dtype=_t.Tensor
-00006ca0: 2e73 697a 655f 6474 7970 652c 0a20 2020  .size_dtype,.   
-00006cb0: 2020 2020 2020 2020 2020 2020 2073 6861               sha
-00006cc0: 7065 3d28 292c 0a20 2020 2020 2020 2020  pe=(),.         
-00006cd0: 2020 2020 2020 2062 6174 6368 5f64 696d         batch_dim
-00006ce0: 5f61 7869 733d 302c 0a20 2020 2020 2020  _axis=0,.       
-00006cf0: 2020 2020 2020 2020 2062 6174 6368 3d73           batch=s
-00006d00: 656c 662e 6261 7463 682c 0a20 2020 2020  elf.batch,.     
-00006d10: 2020 2020 2020 2020 2020 2062 6561 6d3d             beam=
-00006d20: 6265 616d 2c0a 2020 2020 2020 2020 2020  beam,.          
-00006d30: 2020 2020 2020 636f 6e74 726f 6c5f 666c        control_fl
-00006d40: 6f77 5f63 7478 3d73 656c 662e 636f 6e74  ow_ctx=self.cont
-00006d50: 726f 6c5f 666c 6f77 5f63 7478 2c0a 2020  rol_flow_ctx,.  
-00006d60: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00006d70: 2020 2020 7365 6c66 2e64 796e 5f73 697a      self.dyn_siz
-00006d80: 655f 6578 742e 706c 6163 6568 6f6c 6465  e_ext.placeholde
-00006d90: 7220 3d20 6479 6e5f 7369 7a65 0a0a 2020  r = dyn_size..  
-00006da0: 2020 6465 6620 6765 745f 6d61 736b 2873    def get_mask(s
-00006db0: 656c 663a 2044 696d 2c20 2a2c 2064 696d  elf: Dim, *, dim
-00006dc0: 5f6f 7264 6572 3a20 4f70 7469 6f6e 616c  _order: Optional
-00006dd0: 5b53 6571 7565 6e63 655b 4469 6d5d 5d20  [Sequence[Dim]] 
-00006de0: 3d20 4e6f 6e65 2920 2d3e 205f 742e 5465  = None) -> _t.Te
-00006df0: 6e73 6f72 3a0a 2020 2020 2020 2020 2222  nsor:.        ""
-00006e00: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
-00006e10: 2064 696d 5f6f 7264 6572 3a20 6966 2067   dim_order: if g
-00006e20: 6976 656e 2c20 7468 6520 6469 6d73 206f  iven, the dims o
-00006e30: 6620 7468 6520 6d61 736b 2077 696c 6c20  f the mask will 
-00006e40: 6265 2069 6e20 7468 6973 206f 7264 6572  be in this order
-00006e50: 2e0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00006e60: 6973 2063 616e 2062 6520 7573 6566 756c  is can be useful
-00006e70: 2069 6620 7468 6520 6d61 736b 2069 7320   if the mask is 
-00006e80: 6272 6f61 6463 6173 7465 6420 6167 6169  broadcasted agai
-00006e90: 6e73 7420 736f 6d65 206f 7468 6572 2074  nst some other t
-00006ea0: 656e 736f 722e 0a20 2020 2020 2020 203a  ensor..        :
-00006eb0: 7265 7475 726e 3a20 6966 206e 6565 645f  return: if need_
-00006ec0: 6d61 736b 696e 6728 292c 2074 6865 2063  masking(), the c
-00006ed0: 6f72 7265 7370 6f6e 6469 6e67 206d 6173  orresponding mas
-00006ee0: 6b2e 0a20 2020 2020 2020 2020 2020 2049  k..            I
-00006ef0: 6620 7468 6973 2069 7320 652e 672e 2074  f this is e.g. t
-00006f00: 6865 2074 696d 652d 6469 6d20 5420 6f66  he time-dim T of
-00006f10: 2073 6861 7065 205b 425d 2c20 7468 656e   shape [B], then
-00006f20: 2074 6865 206d 6173 6b20 7769 6c6c 2062   the mask will b
-00006f30: 6520 6f66 2073 6861 7065 205b 422c 545d  e of shape [B,T]
-00006f40: 2e0a 2020 2020 2020 2020 2020 2020 5468  ..            Th
-00006f50: 6520 6d61 736b 2063 6f75 6c64 2062 6520  e mask could be 
-00006f60: 7573 6564 2077 6974 6820 3a66 756e 633a  used with :func:
-00006f70: 606d 6173 6b65 645f 7365 6c65 6374 6020  `masked_select` 
-00006f80: 2860 6062 6f6f 6c65 616e 5f6d 6173 6b60  (``boolean_mask`
-00006f90: 6029 206f 7220 6060 7768 6572 6560 602e  `) or ``where``.
-00006fa0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00006fb0: 2020 2020 2069 6d70 6f72 7420 7265 7475       import retu
-00006fc0: 726e 6e2e 6672 6f6e 7465 6e64 2061 7320  rnn.frontend as 
-00006fd0: 7266 0a0a 2020 2020 2020 2020 6173 7365  rf..        asse
-00006fe0: 7274 2073 656c 662e 6479 6e5f 7369 7a65  rt self.dyn_size
-00006ff0: 5f65 7874 2061 6e64 2073 656c 662e 6479  _ext and self.dy
-00007000: 6e5f 7369 7a65 5f65 7874 2e72 6177 5f74  n_size_ext.raw_t
-00007010: 656e 736f 7220 6973 206e 6f74 204e 6f6e  ensor is not Non
-00007020: 650a 2020 2020 2020 2020 2320 6e6f 696e  e.        # noin
-00007030: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
-00007040: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
-00007050: 2020 2062 6163 6b65 6e64 203d 2073 656c     backend = sel
-00007060: 662e 6479 6e5f 7369 7a65 5f65 7874 2e5f  f.dyn_size_ext._
-00007070: 7261 775f 6261 636b 656e 640a 0a20 2020  raw_backend..   
-00007080: 2020 2020 206d 6178 5f69 6478 203d 2072       max_idx = r
-00007090: 662e 7265 6475 6365 280a 2020 2020 2020  f.reduce(.      
-000070a0: 2020 2020 2020 7365 6c66 2e64 796e 5f73        self.dyn_s
-000070b0: 697a 655f 6578 742c 0a20 2020 2020 2020  ize_ext,.       
-000070c0: 2020 2020 2061 7869 733d 7365 6c66 2e64       axis=self.d
-000070d0: 796e 5f73 697a 655f 6578 742e 6469 6d73  yn_size_ext.dims
-000070e0: 2c0a 2020 2020 2020 2020 2020 2020 6d6f  ,.            mo
-000070f0: 6465 3d22 6d61 7822 2c0a 2020 2020 2020  de="max",.      
-00007100: 2020 2020 2020 2320 4d61 736b 696e 6720        # Masking 
-00007110: 6865 7265 2069 7320 6e6f 7420 616c 7761  here is not alwa
-00007120: 7973 2070 6f73 7369 626c 652c 2065 2e67  ys possible, e.g
-00007130: 2e20 6966 2077 6520 6861 7665 0a20 2020  . if we have.   
-00007140: 2020 2020 2020 2020 2023 2074 6167 203d           # tag =
-00007150: 2044 696d 7b27 7365 6c66 2d61 7474 2d6b   Dim{'self-att-k
-00007160: 6579 7327 5b27 7469 6d65 3a76 6172 3a65  eys'['time:var:e
-00007170: 7874 6572 6e5f 6461 7461 3a63 6c61 7373  xtern_data:class
-00007180: 6573 275b 425d 5d7d 0a20 2020 2020 2020  es'[B]]}.       
-00007190: 2020 2020 2075 7365 5f6d 6173 6b3d 4661       use_mask=Fa
-000071a0: 6c73 652c 0a20 2020 2020 2020 2029 0a20  lse,.        ). 
-000071b0: 2020 2020 2020 2023 2057 6520 7573 6520         # We use 
-000071c0: 7468 6520 6173 7375 6d70 7469 6f6e 2074  the assumption t
-000071d0: 6861 7420 7365 6c66 2e70 6c61 6365 686f  hat self.placeho
-000071e0: 6c64 6572 2e73 6861 7065 5b61 7869 735d  lder.shape[axis]
-000071f0: 203d 3d20 6d61 785f 6964 782e 0a20 2020   == max_idx..   
-00007200: 2020 2020 2023 2073 697a 655f 6578 7420       # size_ext 
-00007210: 6d69 6768 7420 6861 7665 2069 6e76 616c  might have inval
-00007220: 6964 2028 7a65 726f 2920 7369 7a65 730a  id (zero) sizes.
-00007230: 2020 2020 2020 2020 2320 7768 656e 2069          # when i
-00007240: 7420 6974 7365 6c66 2068 6173 2073 6f6d  t itself has som
-00007250: 6520 7061 6464 696e 672c 2065 2e67 2e20  e padding, e.g. 
-00007260: 7768 656e 2069 7473 206f 776e 2073 6861  when its own sha
-00007270: 7065 2069 7320 6479 6e61 6d69 632e 0a20  pe is dynamic.. 
-00007280: 2020 2020 2020 2023 2041 207a 6572 6f20         # A zero 
-00007290: 7369 7a65 2063 616e 206c 6561 6420 746f  size can lead to
-000072a0: 2070 726f 626c 656d 7320 696e 2073 6f6d   problems in som
-000072b0: 6520 6361 7365 732c 2065 2e67 2e20 696e  e cases, e.g. in
-000072c0: 2053 6f66 746d 6178 4f76 6572 5370 6174   SoftmaxOverSpat
-000072d0: 6961 6c4c 6179 6572 2c0a 2020 2020 2020  ialLayer,.      
-000072e0: 2020 2320 7768 656e 2065 7665 7279 7468    # when everyth
-000072f0: 696e 6720 6973 206d 6173 6b65 6420 746f  ing is masked to
-00007300: 202d 696e 662c 2069 7420 7265 7375 6c74   -inf, it result
-00007310: 7320 696e 206e 616e 2c0a 2020 2020 2020  s in nan,.      
-00007320: 2020 2320 616e 6420 7468 6973 206c 696b    # and this lik
-00007330: 656c 7920 7072 6f64 7563 6573 206e 616e  ely produces nan
-00007340: 2069 6e20 6261 636b 7072 6f70 206f 7220   in backprop or 
-00007350: 656c 7365 7768 6572 652e 0a20 2020 2020  elsewhere..     
-00007360: 2020 2023 2054 6875 732c 206d 6173 6b20     # Thus, mask 
-00007370: 7369 7a65 5f65 7874 2069 7473 656c 662c  size_ext itself,
-00007380: 2061 6e64 2073 6574 2074 6865 2070 6164   and set the pad
-00007390: 6465 6420 7661 6c75 6573 2074 6f20 312e  ded values to 1.
-000073a0: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
-000073b0: 6173 7375 6d65 7320 7468 6174 206d 6178  assumes that max
-000073c0: 5f69 6478 203e 3d20 312e 0a20 2020 2020  _idx >= 1..     
-000073d0: 2020 2073 697a 655f 6578 7420 3d20 7365     size_ext = se
-000073e0: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
-000073f0: 636f 7079 5f6d 6173 6b65 6428 6d61 785f  copy_masked(max_
-00007400: 6964 7829 0a20 2020 2020 2020 2069 6478  idx).        idx
-00007410: 5f72 616e 6765 203d 2062 6163 6b65 6e64  _range = backend
-00007420: 2e72 616e 6765 5f6f 7665 725f 6469 6d28  .range_over_dim(
-00007430: 7365 6c66 290a 2020 2020 2020 2020 7365  self).        se
-00007440: 715f 6d61 736b 203d 2072 662e 636f 6d70  q_mask = rf.comp
-00007450: 6172 6528 6964 785f 7261 6e67 652c 2022  are(idx_range, "
-00007460: 3c22 2c20 7369 7a65 5f65 7874 2c20 616c  <", size_ext, al
-00007470: 6c6f 775f 6272 6f61 6463 6173 745f 616c  low_broadcast_al
-00007480: 6c5f 736f 7572 6365 733d 5472 7565 2c20  l_sources=True, 
-00007490: 6469 6d5f 6f72 6465 723d 6469 6d5f 6f72  dim_order=dim_or
-000074a0: 6465 7229 0a20 2020 2020 2020 2072 6574  der).        ret
-000074b0: 7572 6e20 7365 715f 6d61 736b 0a0a 2020  urn seq_mask..  
-000074c0: 2020 6465 6620 6973 5f62 6174 6368 5f64    def is_batch_d
-000074d0: 696d 2873 656c 6629 3a0a 2020 2020 2020  im(self):.      
-000074e0: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
-000074f0: 6574 7572 6e3a 2077 6865 7468 6572 2074  eturn: whether t
-00007500: 6869 7320 6469 6d20 7461 6720 6973 206f  his dim tag is o
-00007510: 6620 6b69 6e64 2062 6174 6368 0a20 2020  f kind batch.   
-00007520: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-00007530: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
-00007540: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00007550: 662e 6b69 6e64 203d 3d20 4469 6d54 7970  f.kind == DimTyp
-00007560: 6573 2e42 6174 6368 0a0a 2020 2020 6465  es.Batch..    de
-00007570: 6620 6973 5f66 6561 7475 7265 5f64 696d  f is_feature_dim
-00007580: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-00007590: 2222 220a 2020 2020 2020 2020 3a72 6574  """.        :ret
-000075a0: 7572 6e3a 2077 6865 7468 6572 2074 6869  urn: whether thi
-000075b0: 7320 6469 6d20 7461 6720 6973 206f 6620  s dim tag is of 
-000075c0: 6b69 6e64 2066 6561 7475 7265 0a20 2020  kind feature.   
-000075d0: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-000075e0: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
-000075f0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-00007600: 662e 6b69 6e64 203d 3d20 4469 6d54 7970  f.kind == DimTyp
-00007610: 6573 2e46 6561 7475 7265 0a0a 2020 2020  es.Feature..    
-00007620: 6465 6620 6973 5f73 7061 7469 616c 5f64  def is_spatial_d
-00007630: 696d 2873 656c 6629 3a0a 2020 2020 2020  im(self):.      
-00007640: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
-00007650: 6574 7572 6e3a 2077 6865 7468 6572 2074  eturn: whether t
-00007660: 6869 7320 6469 6d20 7461 6720 6973 206f  his dim tag is o
-00007670: 6620 6b69 6e64 2073 7061 7469 616c 0a20  f kind spatial. 
-00007680: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
-00007690: 6f6f 6c0a 2020 2020 2020 2020 2222 220a  ool.        """.
-000076a0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000076b0: 656c 662e 6b69 6e64 203d 3d20 4469 6d54  elf.kind == DimT
-000076c0: 7970 6573 2e53 7061 7469 616c 0a0a 2020  ypes.Spatial..  
-000076d0: 2020 6465 6620 6973 5f64 696d 5f6b 6e6f    def is_dim_kno
-000076e0: 776e 2873 656c 6629 3a0a 2020 2020 2020  wn(self):.      
-000076f0: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
-00007700: 6574 7572 6e3a 2077 6865 7468 6572 2077  eturn: whether w
-00007710: 6520 6b6e 6f77 2074 6865 2064 696d 656e  e know the dimen
-00007720: 7369 6f6e 3b20 6261 7369 6361 6c6c 7920  sion; basically 
-00007730: 7768 6574 6865 7220 7468 6973 2069 7320  whether this is 
-00007740: 6465 6669 6e65 640a 2020 2020 2020 2020  defined.        
-00007750: 2020 2861 6c74 686f 7567 6820 606e 6f74    (although `not
-00007760: 2073 656c 662e 756e 6465 6669 6e65 6460   self.undefined`
-00007770: 2069 7320 6465 6669 6e65 6420 736c 6967   is defined slig
-00007780: 6874 6c79 2064 6966 6665 7265 6e74 6c79  htly differently
-00007790: 290a 2020 2020 2020 2020 3a72 7479 7065  ).        :rtype
-000077a0: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
-000077b0: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
-000077c0: 6c66 2e69 735f 6261 7463 685f 6469 6d28  lf.is_batch_dim(
-000077d0: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-000077e0: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-000077f0: 2020 2069 6620 6e6f 7420 7365 6c66 2e69     if not self.i
-00007800: 735f 6479 6e61 6d69 6328 2920 616e 6420  s_dynamic() and 
-00007810: 7365 6c66 2e64 696d 656e 7369 6f6e 2069  self.dimension i
-00007820: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00007830: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-00007840: 7275 650a 2020 2020 2020 2020 6966 2073  rue.        if s
-00007850: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-00007860: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-00007870: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-00007880: 2020 6578 7472 6120 3d20 7365 6c66 2e5f    extra = self._
-00007890: 6765 745f 7361 6d65 5f62 6173 655f 6578  get_same_base_ex
-000078a0: 7472 6128 290a 2020 2020 2020 2020 6966  tra().        if
-000078b0: 2065 7874 7261 3a0a 2020 2020 2020 2020   extra:.        
-000078c0: 2020 2020 666f 7220 5f2c 206f 7468 6572      for _, other
-000078d0: 2069 6e20 6578 7472 612e 7361 6d65 5f66   in extra.same_f
-000078e0: 6f72 5f62 6174 6368 5f63 7478 2e69 7465  or_batch_ctx.ite
-000078f0: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-00007900: 2020 2020 2020 6966 206f 7468 6572 2e64        if other.d
-00007910: 796e 5f73 697a 655f 6578 743a 0a20 2020  yn_size_ext:.   
-00007920: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00007930: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
-00007940: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-00007950: 650a 0a20 2020 2064 6566 2069 735f 6479  e..    def is_dy
-00007960: 6e61 6d69 6328 7365 6c66 2920 2d3e 2062  namic(self) -> b
-00007970: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
-00007980: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-00007990: 3a20 7768 6574 6865 7220 7468 6520 6469  : whether the di
-000079a0: 6d20 6973 206e 6f74 2073 7461 7469 632e  m is not static.
-000079b0: 2075 7375 616c 6c79 206d 6561 6e73 2074   usually means t
-000079c0: 6861 7420 6974 2068 6173 2073 6571 206c  hat it has seq l
-000079d0: 656e 6774 6873 0a20 2020 2020 2020 2022  engths.        "
-000079e0: 2222 0a20 2020 2020 2020 2072 6574 7572  "".        retur
-000079f0: 6e20 7365 6c66 2e64 696d 656e 7369 6f6e  n self.dimension
-00007a00: 2069 7320 4e6f 6e65 2061 6e64 206e 6f74   is None and not
-00007a10: 2073 656c 662e 6973 5f62 6174 6368 5f64   self.is_batch_d
-00007a20: 696d 2829 0a0a 2020 2020 6465 6620 6973  im()..    def is
-00007a30: 5f73 7461 7469 6328 7365 6c66 2920 2d3e  _static(self) ->
-00007a40: 2062 6f6f 6c3a 0a20 2020 2020 2020 2022   bool:.        "
-00007a50: 2222 0a20 2020 2020 2020 203a 7265 7475  "".        :retu
-00007a60: 726e 3a20 7374 6174 6963 0a20 2020 2020  rn: static.     
-00007a70: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00007a80: 6574 7572 6e20 6e6f 7420 7365 6c66 2e69  eturn not self.i
-00007a90: 735f 6479 6e61 6d69 6328 290a 0a20 2020  s_dynamic()..   
-00007aa0: 2064 6566 206e 6565 645f 6d61 736b 696e   def need_maskin
-00007ab0: 6728 7365 6c66 293a 0a20 2020 2020 2020  g(self):.       
-00007ac0: 2022 2222 0a20 2020 2020 2020 203a 7265   """.        :re
-00007ad0: 7475 726e 3a20 7768 6574 6865 7220 6469  turn: whether di
-00007ae0: 6d20 6973 2073 7461 7469 6320 6f72 2064  m is static or d
-00007af0: 796e 616d 6963 2062 7574 2077 6974 6820  ynamic but with 
-00007b00: 7363 616c 6172 2064 796e 5f73 697a 655f  scalar dyn_size_
-00007b10: 6578 740a 2020 2020 2020 2020 2222 220a  ext.        """.
-00007b20: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00007b30: 6973 5f73 7461 7469 6328 293a 0a20 2020  is_static():.   
-00007b40: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-00007b50: 2e63 6170 6163 6974 7920 6973 206e 6f74  .capacity is not
-00007b60: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00007b70: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00007b80: 6c66 2e73 697a 6520 3c20 7365 6c66 2e63  lf.size < self.c
-00007b90: 6170 6163 6974 790a 2020 2020 2020 2020  apacity.        
-00007ba0: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00007bb0: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-00007bc0: 2e63 6170 6163 6974 7920 6973 206e 6f74  .capacity is not
-00007bd0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00007be0: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-00007bf0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
-00007c00: 6c66 2e64 796e 5f73 697a 655f 6578 743a  lf.dyn_size_ext:
-00007c10: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00007c20: 7572 6e20 5472 7565 2020 2320 756e 6b6e  urn True  # unkn
-00007c30: 6f77 6e0a 2020 2020 2020 2020 7265 7475  own.        retu
-00007c40: 726e 2073 656c 662e 6479 6e5f 7369 7a65  rn self.dyn_size
-00007c50: 5f65 7874 2e62 6174 6368 5f6e 6469 6d20  _ext.batch_ndim 
-00007c60: 3e20 300a 0a20 2020 2064 6566 2063 616e  > 0..    def can
-00007c70: 5f62 655f 7573 6564 5f61 735f 6469 6d28  _be_used_as_dim(
-00007c80: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
-00007c90: 2222 0a20 2020 2020 2020 203a 7265 7475  "".        :retu
-00007ca0: 726e 3a20 7768 6574 6865 7220 7468 6973  rn: whether this
-00007cb0: 2063 616e 2062 6520 7573 6564 2061 7320   can be used as 
-00007cc0: 6120 6469 6d20 696e 203a 636c 6173 733a  a dim in :class:
-00007cd0: 6044 6174 6160 2c20 692e 652e 2069 7420  `Data`, i.e. it 
-00007ce0: 6973 206e 6f74 2073 7065 6369 616c 0a20  is not special. 
-00007cf0: 2020 2020 2020 203a 7274 7970 653a 2062         :rtype: b
-00007d00: 6f6f 6c0a 2020 2020 2020 2020 2222 220a  ool.        """.
-00007d10: 2020 2020 2020 2020 7265 7475 726e 206e          return n
-00007d20: 6f74 2073 656c 662e 7370 6563 6961 6c0a  ot self.special.
-00007d30: 0a20 2020 2064 6566 2069 735f 7361 6d65  .    def is_same
-00007d40: 5f73 697a 655f 7465 6e73 6f72 2873 656c  _size_tensor(sel
-00007d50: 662c 2078 293a 0a20 2020 2020 2020 2022  f, x):.        "
-00007d60: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-00007d70: 6d20 7466 2e54 656e 736f 7220 783a 0a20  m tf.Tensor x:. 
-00007d80: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00007d90: 7768 6574 6865 7220 7468 6973 2064 696d  whether this dim
-00007da0: 2074 6167 2066 6f72 2074 6869 7320 7370   tag for this sp
-00007db0: 6563 6966 6963 2062 6174 6368 2028 696e  ecific batch (in
-00007dc0: 636c 2062 6561 6d29 2069 7320 7468 6520  cl beam) is the 
-00007dd0: 7361 6d65 2061 7320 7468 6520 6769 7665  same as the give
-00007de0: 6e20 7369 7a65 0a20 2020 2020 2020 203a  n size.        :
-00007df0: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
-00007e00: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00007e10: 6966 2073 656c 662e 6479 6e5f 7369 7a65  if self.dyn_size
-00007e20: 5f65 7874 2061 6e64 2078 2069 7320 7365  _ext and x is se
-00007e30: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
-00007e40: 706c 6163 6568 6f6c 6465 723a 0a20 2020  placeholder:.   
-00007e50: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00007e60: 5472 7565 0a20 2020 2020 2020 2074 6167  True.        tag
-00007e70: 203d 205f 4469 6d4d 6978 696e 2e67 6574   = _DimMixin.get
-00007e80: 5f74 6167 5f66 726f 6d5f 7369 7a65 5f74  _tag_from_size_t
-00007e90: 656e 736f 7228 7829 0a20 2020 2020 2020  ensor(x).       
-00007ea0: 2069 6620 7461 6720 616e 6420 7461 6720   if tag and tag 
-00007eb0: 3d3d 2073 656c 663a 0a20 2020 2020 2020  == self:.       
-00007ec0: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00007ed0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-00007ee0: 7365 6c66 2e5f 6578 7472 613a 0a20 2020  self._extra:.   
-00007ef0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00007f00: 4661 6c73 650a 2020 2020 2020 2020 6966  False.        if
-00007f10: 2075 7469 6c2e 5265 6649 6445 7128 7829   util.RefIdEq(x)
-00007f20: 2069 6e20 7365 6c66 2e5f 6578 7472 612e   in self._extra.
-00007f30: 6479 6e5f 7369 7a65 5f73 616d 653a 0a20  dyn_size_same:. 
-00007f40: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00007f50: 6e20 5472 7565 0a20 2020 2020 2020 2072  n True.        r
-00007f60: 6574 7572 6e20 4661 6c73 650a 0a20 2020  eturn False..   
-00007f70: 2064 6566 2073 6574 5f74 6167 5f6f 6e5f   def set_tag_on_
-00007f80: 7369 7a65 5f74 656e 736f 7228 7365 6c66  size_tensor(self
-00007f90: 3a20 4469 6d2c 2078 2c20 6261 7463 683d  : Dim, x, batch=
-00007fa0: 4e6f 6e65 2c20 7361 6d65 5f61 735f 6265  None, same_as_be
-00007fb0: 666f 7265 3d46 616c 7365 2920 2d3e 2044  fore=False) -> D
-00007fc0: 696d 3a0a 2020 2020 2020 2020 2222 220a  im:.        """.
-00007fd0: 2020 2020 2020 2020 5468 6973 2066 756e          This fun
-00007fe0: 6374 696f 6e20 6973 2075 7365 640a 2020  ction is used.  
-00007ff0: 2020 2020 2020 746f 2063 6f75 706c 6520        to couple 
-00008000: 6120 7466 2e54 656e 736f 7220 696e 7374  a tf.Tensor inst
-00008010: 616e 6365 2072 6570 7265 7365 6e74 696e  ance representin
-00008020: 6720 7468 6520 6479 6e20 7369 7a65 0a20  g the dyn size. 
-00008030: 2020 2020 2020 2077 6974 6820 7468 6520         with the 
-00008040: 6469 6d20 7461 672e 0a0a 2020 2020 2020  dim tag...      
-00008050: 2020 5468 6973 2069 7320 7573 7561 6c6c    This is usuall
-00008060: 7920 6120 6e65 776c 7920 6372 6561 7465  y a newly create
-00008070: 6420 6469 6d20 7461 672c 0a20 2020 2020  d dim tag,.     
-00008080: 2020 2077 6869 6368 2069 7320 7965 7420     which is yet 
-00008090: 756e 7365 742e 0a0a 2020 2020 2020 2020  unset...        
-000080a0: 4974 2069 7320 616c 736f 2075 7365 6420  It is also used 
-000080b0: 746f 2063 6f75 706c 6520 616e 2065 7869  to couple an exi
-000080c0: 7374 696e 6720 6469 6d20 7461 6720 7769  sting dim tag wi
-000080d0: 7468 206f 7468 6572 2064 796e 2073 697a  th other dyn siz
-000080e0: 6573 0a20 2020 2020 2020 2077 6869 6368  es.        which
-000080f0: 206a 7573 7420 6469 6666 6572 2062 7920   just differ by 
-00008100: 616e 2065 7870 616e 7369 6f6e 206f 6620  an expansion of 
-00008110: 7468 6520 6261 7463 6820 2865 2e67 2e20  the batch (e.g. 
-00008120: 7365 6172 6368 2062 6561 6d29 2e0a 0a20  search beam)... 
-00008130: 2020 2020 2020 2053 6565 2061 6c73 6f20         See also 
-00008140: 3a66 756e 633a 6067 6574 5f74 6167 5f66  :func:`get_tag_f
-00008150: 726f 6d5f 7369 7a65 5f74 656e 736f 7260  rom_size_tensor`
-00008160: 2e0a 2020 2020 2020 2020 416c 736f 2073  ..        Also s
-00008170: 6565 203a 6675 6e63 3a60 7365 745f 6479  ee :func:`set_dy
-00008180: 6e5f 7369 7a65 5f65 7874 5f66 6f72 5f62  n_size_ext_for_b
-00008190: 6174 6368 5f63 7478 602e 0a0a 2020 2020  atch_ctx`...    
-000081a0: 2020 2020 3a70 6172 616d 2078 3a20 7261      :param x: ra
-000081b0: 7720 7465 6e73 6f72 2c20 666f 7220 6578  w tensor, for ex
-000081c0: 616d 706c 6520 7466 2e54 656e 736f 720a  ample tf.Tensor.
-000081d0: 2020 2020 2020 2020 3a70 6172 616d 2042          :param B
-000081e0: 6174 6368 496e 666f 7c4e 6f6e 6520 6261  atchInfo|None ba
-000081f0: 7463 683a 0a20 2020 2020 2020 203a 7061  tch:.        :pa
-00008200: 7261 6d20 626f 6f6c 2073 616d 655f 6173  ram bool same_as
-00008210: 5f62 6566 6f72 653a 2069 6d70 6c69 6573  _before: implies
-00008220: 2069 7420 7761 7320 7365 7420 6265 666f   it was set befo
-00008230: 7265 2c20 616e 6420 7468 6520 6e65 7720  re, and the new 
-00008240: 7369 7a65 2069 7320 7468 6520 7361 6d65  size is the same
-00008250: 2e0a 2020 2020 2020 2020 2020 652e 672e  ..          e.g.
-00008260: 2069 7420 636f 756c 6420 6265 2073 6f6d   it could be som
-00008270: 6520 6964 656e 7469 7479 2077 6974 6820  e identity with 
-00008280: 6164 6465 6420 6368 6563 6b73 2c20 6f72  added checks, or
-00008290: 206f 7468 6572 2063 6861 6e67 652e 0a20   other change.. 
-000082a0: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-000082b0: 7365 6c66 206f 7220 6e65 7720 6469 6d20  self or new dim 
-000082c0: 7461 670a 2020 2020 2020 2020 2222 220a  tag.        """.
-000082d0: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-000082e0: 656c 662e 6361 6e5f 6265 5f75 7365 645f  elf.can_be_used_
-000082f0: 6173 5f64 696d 2829 0a20 2020 2020 2020  as_dim().       
-00008300: 2023 2049 7427 7320 756e 7573 7561 6c20   # It's unusual 
-00008310: 6966 2073 656c 662e 6469 6d65 6e73 696f  if self.dimensio
-00008320: 6e20 6973 206e 6f74 204e 6f6e 652c 2062  n is not None, b
-00008330: 7574 206c 6574 2773 2061 6363 6570 7420  ut let's accept 
-00008340: 7468 6174 2e0a 2020 2020 2020 2020 6966  that..        if
-00008350: 2068 6173 6174 7472 2878 2c20 225f 6973   hasattr(x, "_is
-00008360: 5f73 697a 655f 6f66 5f64 696d 5f74 6167  _size_of_dim_tag
-00008370: 2229 3a0a 2020 2020 2020 2020 2020 2020  "):.            
-00008380: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
-00008390: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
-000083a0: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-000083b0: 6572 7420 782e 5f69 735f 7369 7a65 5f6f  ert x._is_size_o
-000083c0: 665f 6469 6d5f 7461 6720 696e 2028 4e6f  f_dim_tag in (No
-000083d0: 6e65 2c20 7365 6c66 290a 2020 2020 2020  ne, self).      
-000083e0: 2020 2320 4966 2077 6520 616c 7265 6164    # If we alread
-000083f0: 7920 6861 7665 2061 6e6f 7468 6572 2064  y have another d
-00008400: 796e 2073 697a 6520 7365 7420 6f72 2064  yn size set or d
-00008410: 6966 6665 7265 6e74 2062 6174 6368 2c20  ifferent batch, 
-00008420: 6372 6561 7465 2061 206e 6577 2044 696d  create a new Dim
-00008430: 2069 6e73 7461 6e63 652e 0a20 2020 2020   instance..     
-00008440: 2020 2069 6620 7365 6c66 2e62 6174 6368     if self.batch
-00008450: 2061 6e64 2062 6174 6368 2061 6e64 2073   and batch and s
-00008460: 656c 662e 6261 7463 6820 213d 2062 6174  elf.batch != bat
-00008470: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
-00008480: 6173 7365 7274 206e 6f74 2073 616d 655f  assert not same_
-00008490: 6173 5f62 6566 6f72 6520 2023 2069 7420  as_before  # it 
-000084a0: 6361 6e6e 6f74 2062 6520 7468 6520 7361  cannot be the sa
-000084b0: 6d65 2077 6865 6e20 6974 2069 7320 616e  me when it is an
-000084c0: 6f74 6865 7220 6261 7463 682e 2e2e 0a20  other batch.... 
-000084d0: 2020 2020 2020 2020 2020 206e 6577 5f64             new_d
-000084e0: 696d 5f74 6167 203d 2073 656c 662e 6765  im_tag = self.ge
-000084f0: 745f 666f 725f 6261 7463 685f 6374 7828  t_for_batch_ctx(
-00008500: 6261 7463 683d 6261 7463 682c 2063 7478  batch=batch, ctx
-00008510: 3d73 656c 662e 636f 6e74 726f 6c5f 666c  =self.control_fl
-00008520: 6f77 5f63 7478 290a 2020 2020 2020 2020  ow_ctx).        
-00008530: 2020 2020 6e65 775f 6469 6d5f 7461 672e      new_dim_tag.
-00008540: 7365 745f 7461 675f 6f6e 5f73 697a 655f  set_tag_on_size_
-00008550: 7465 6e73 6f72 2878 2c20 6261 7463 683d  tensor(x, batch=
-00008560: 6261 7463 6829 0a20 2020 2020 2020 2020  batch).         
-00008570: 2020 2072 6574 7572 6e20 6e65 775f 6469     return new_di
-00008580: 6d5f 7461 670a 2020 2020 2020 2020 6966  m_tag.        if
-00008590: 2073 656c 662e 6479 6e5f 7369 7a65 2069   self.dyn_size i
-000085a0: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2073  s not None and s
-000085b0: 656c 662e 6479 6e5f 7369 7a65 2069 7320  elf.dyn_size is 
-000085c0: 6e6f 7420 783a 0a20 2020 2020 2020 2020  not x:.         
-000085d0: 2020 2069 6620 7365 6c66 2e5f 6578 7472     if self._extr
-000085e0: 6120 616e 6420 7574 696c 2e52 6566 4964  a and util.RefId
-000085f0: 4571 2878 2920 696e 2073 656c 662e 5f65  Eq(x) in self._e
-00008600: 7874 7261 2e64 796e 5f73 697a 655f 7361  xtra.dyn_size_sa
-00008610: 6d65 3a0a 2020 2020 2020 2020 2020 2020  me:.            
-00008620: 2020 2020 7061 7373 2020 2320 6f6b 2c20      pass  # ok, 
-00008630: 7061 7373 206f 6e0a 2020 2020 2020 2020  pass on.        
-00008640: 2020 2020 656c 6966 2073 616d 655f 6173      elif same_as
-00008650: 5f62 6566 6f72 653a 0a20 2020 2020 2020  _before:.       
-00008660: 2020 2020 2020 2020 2073 656c 662e 5f6d           self._m
-00008670: 616b 655f 6578 7472 6128 292e 6479 6e5f  ake_extra().dyn_
-00008680: 7369 7a65 5f73 616d 652e 6164 6428 7574  size_same.add(ut
-00008690: 696c 2e52 6566 4964 4571 2878 2929 0a20  il.RefIdEq(x)). 
-000086a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
-000086b0: 2041 6e64 206e 6f77 2070 6173 7320 6f6e   And now pass on
-000086c0: 2e0a 2020 2020 2020 2020 2020 2020 656c  ..            el
-000086d0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-000086e0: 2020 2020 6173 7365 7274 2073 656c 662e      assert self.
-000086f0: 6261 7463 6820 616e 6420 6261 7463 680a  batch and batch.
-00008700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008710: 2320 4974 2773 206e 6f74 2063 6c65 6172  # It's not clear
-00008720: 2077 6861 7420 746f 2064 6f2e 2057 6520   what to do. We 
-00008730: 636f 756c 6420 6372 6561 7465 2061 206e  could create a n
-00008740: 6577 2064 696d 2074 6167 2c20 6275 7420  ew dim tag, but 
-00008750: 7468 6520 7369 7a65 7320 6d69 6768 7420  the sizes might 
-00008760: 6265 2064 6966 6665 7265 6e74 2e0a 2020  be different..  
-00008770: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00008780: 5573 7561 6c6c 7920 7765 2073 686f 756c  Usually we shoul
-00008790: 6420 6e6f 7420 6765 7420 6865 7265 2e0a  d not get here..
-000087a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000087b0: 2320 536f 2066 6f72 206e 6f77 2c20 6a75  # So for now, ju
-000087c0: 7374 2065 7272 6f72 2e0a 2020 2020 2020  st error..      
-000087d0: 2020 2020 2020 2020 2020 2320 6e6f 696e            # noin
-000087e0: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
-000087f0: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
-00008800: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
-00008810: 7265 7475 726e 6e2e 6672 6f6e 7465 6e64  returnn.frontend
-00008820: 2e5f 6261 636b 656e 6420 696d 706f 7274  ._backend import
-00008830: 2067 6574 5f62 6163 6b65 6e64 5f62 795f   get_backend_by_
-00008840: 7261 775f 7465 6e73 6f72 5f74 7970 650a  raw_tensor_type.
-00008850: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00008860: 2072 6169 7365 2045 7863 6570 7469 6f6e   raise Exception
-00008870: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00008880: 2020 2020 2020 225c 6e22 2e6a 6f69 6e28        "\n".join(
-00008890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000088a0: 2020 2020 2020 2020 205b 0a20 2020 2020           [.     
-000088b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088c0: 2020 2020 2020 2028 0a20 2020 2020 2020         (.       
-000088d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000088e0: 2020 2020 2020 2020 2022 2572 2028 2572           "%r (%r
-000088f0: 2920 616c 7265 6164 7920 6861 7320 7369  ) already has si
-00008900: 7a65 2025 722c 220a 2020 2020 2020 2020  ze %r,".        
-00008910: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008920: 2020 2020 2020 2020 2220 616e 6420 616e          " and an
-00008930: 6f74 6865 7220 696e 636f 6d70 6174 6962  other incompatib
-00008940: 6c65 2073 697a 6520 2572 2028 6261 7463  le size %r (batc
-00008950: 6820 2572 2920 6973 2062 6569 6e67 2061  h %r) is being a
-00008960: 7373 6967 6e65 642e 220a 2020 2020 2020  ssigned.".      
-00008970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008980: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00008990: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089a0: 2020 2020 2520 2873 656c 662c 2073 656c      % (self, sel
-000089b0: 662e 6465 7363 7269 7074 696f 6e2c 2073  f.description, s
-000089c0: 656c 662e 6479 6e5f 7369 7a65 2c20 782c  elf.dyn_size, x,
-000089d0: 2062 6174 6368 292c 0a20 2020 2020 2020   batch),.       
-000089e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000089f0: 2020 2020 2022 5c6e 4e65 7720 7369 7a65       "\nNew size
-00008a00: 2063 6f6d 7075 7461 7469 6f6e 2067 7261   computation gra
-00008a10: 7068 3a22 2c0a 2020 2020 2020 2020 2020  ph:",.          
-00008a20: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a30: 2020 6765 745f 6261 636b 656e 645f 6279    get_backend_by
-00008a40: 5f72 6177 5f74 656e 736f 725f 7479 7065  _raw_tensor_type
-00008a50: 2874 7970 6528 7829 292e 666f 726d 6174  (type(x)).format
-00008a60: 5f67 7261 7068 5f6f 7574 7075 7428 782c  _graph_output(x,
-00008a70: 206d 6178 5f64 6570 7468 3d33 292c 0a20   max_depth=3),. 
-00008a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008a90: 2020 2020 2020 2020 2020 2022 5c6e 5468             "\nTh
-00008aa0: 6973 2069 7320 6d61 7962 6520 7468 6520  is is maybe the 
-00008ab0: 7265 7375 6c74 206f 6620 616e 2069 6e63  result of an inc
-00008ac0: 6f72 7265 6374 2064 6563 6c61 7265 5f73  orrect declare_s
-00008ad0: 616d 655f 6173 2e20 222c 0a20 2020 2020  ame_as. ",.     
-00008ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008af0: 2020 2020 2020 2022 7361 6d65 5f61 7320         "same_as 
-00008b00: 3d20 2573 2220 2520 7365 6c66 2e73 616d  = %s" % self.sam
-00008b10: 655f 6173 2c0a 2020 2020 2020 2020 2020  e_as,.          
-00008b20: 2020 2020 2020 2020 2020 2020 2020 5d0a                ].
-00008b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008b40: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00008b50: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-00008b60: 6966 2062 6174 6368 2061 6e64 2067 6574  if batch and get
-00008b70: 6174 7472 2878 2c20 225f 5245 5455 524e  attr(x, "_RETURN
-00008b80: 4e5f 6479 6e5f 7369 7a65 5f62 6561 6d22  N_dyn_size_beam"
-00008b90: 2c20 4e6f 6e65 293a 0a20 2020 2020 2020  , None):.       
-00008ba0: 2020 2020 2061 7373 6572 7420 6261 7463       assert batc
-00008bb0: 682e 6265 616d 203d 3d20 6765 7461 7474  h.beam == getatt
-00008bc0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-00008bd0: 2020 2078 2c20 225f 5245 5455 524e 4e5f     x, "_RETURNN_
-00008be0: 6479 6e5f 7369 7a65 5f62 6561 6d22 0a20  dyn_size_beam". 
-00008bf0: 2020 2020 2020 2020 2020 2029 2c20 2225             ), "%
-00008c00: 733a 2064 796e 2073 697a 6520 2573 2068  s: dyn size %s h
-00008c10: 6173 2075 6e65 7870 6563 7465 6420 6261  as unexpected ba
-00008c20: 7463 6820 2573 2c20 6578 7065 6374 6564  tch %s, expected
-00008c30: 2025 7322 2025 2028 0a20 2020 2020 2020   %s" % (.       
-00008c40: 2020 2020 2020 2020 2073 656c 662c 0a20           self,. 
-00008c50: 2020 2020 2020 2020 2020 2020 2020 2078                 x
-00008c60: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00008c70: 2020 6261 7463 682c 0a20 2020 2020 2020    batch,.       
-00008c80: 2020 2020 2020 2020 2067 6574 6174 7472           getattr
-00008c90: 2878 2c20 225f 5245 5455 524e 4e5f 6479  (x, "_RETURNN_dy
-00008ca0: 6e5f 7369 7a65 5f62 6561 6d22 292c 0a20  n_size_beam"),. 
-00008cb0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
-00008cc0: 2020 2020 2069 6620 7365 6c66 2e62 6174       if self.bat
-00008cd0: 6368 2061 6e64 2062 6174 6368 3a0a 2020  ch and batch:.  
-00008ce0: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00008cf0: 2073 656c 662e 6261 7463 6820 3d3d 2062   self.batch == b
-00008d00: 6174 6368 0a20 2020 2020 2020 2065 6c69  atch.        eli
-00008d10: 6620 6261 7463 6820 616e 6420 6e6f 7420  f batch and not 
-00008d20: 7365 6c66 2e62 6174 6368 3a0a 2020 2020  self.batch:.    
-00008d30: 2020 2020 2020 2020 7365 6c66 2e62 6174          self.bat
-00008d40: 6368 203d 2062 6174 6368 2020 2320 6f76  ch = batch  # ov
-00008d50: 6572 7461 6b65 0a20 2020 2020 2020 2069  ertake.        i
-00008d60: 6620 6e6f 7420 7365 6c66 2e69 735f 6261  f not self.is_ba
-00008d70: 7463 685f 6469 6d28 2920 616e 6420 7365  tch_dim() and se
-00008d80: 6c66 2e69 735f 6479 6e61 6d69 6328 293a  lf.is_dynamic():
-00008d90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00008da0: 7361 6d65 5f61 735f 6265 666f 7265 3a0a  same_as_before:.
-00008db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008dc0: 6173 7365 7274 2073 656c 662e 6479 6e5f  assert self.dyn_
-00008dd0: 7369 7a65 5f65 7874 2061 6e64 2073 656c  size_ext and sel
-00008de0: 662e 6479 6e5f 7369 7a65 5f65 7874 2e70  f.dyn_size_ext.p
-00008df0: 6c61 6365 686f 6c64 6572 2069 7320 6e6f  laceholder is no
-00008e00: 7420 4e6f 6e65 0a20 2020 2020 2020 2020  t None.         
-00008e10: 2020 2020 2020 2023 2044 6f20 6e6f 7420         # Do not 
-00008e20: 6f76 6572 7772 6974 6520 6974 2e0a 2020  overwrite it..  
-00008e30: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-00008e40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00008e50: 7365 6c66 2e5f 696e 6974 5f64 6566 6175  self._init_defau
-00008e60: 6c74 5f64 796e 5f73 697a 655f 6578 7428  lt_dyn_size_ext(
-00008e70: 7829 0a20 2020 2020 2020 2069 6620 6765  x).        if ge
-00008e80: 7461 7474 7228 782c 2022 5f69 735f 7369  tattr(x, "_is_si
-00008e90: 7a65 5f6f 665f 6469 6d5f 7461 6722 2c20  ze_of_dim_tag", 
-00008ea0: 4e6f 6e65 2920 6973 204e 6f6e 653a 0a20  None) is None:. 
-00008eb0: 2020 2020 2020 2020 2020 2073 6574 6174             setat
-00008ec0: 7472 2878 2c20 225f 6973 5f73 697a 655f  tr(x, "_is_size_
-00008ed0: 6f66 5f64 696d 5f74 6167 222c 2073 656c  of_dim_tag", sel
-00008ee0: 6629 0a20 2020 2020 2020 2072 6574 7572  f).        retur
-00008ef0: 6e20 7365 6c66 0a0a 2020 2020 4063 6c61  n self..    @cla
-00008f00: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-00008f10: 2067 6574 5f74 6167 5f66 726f 6d5f 7369   get_tag_from_si
-00008f20: 7a65 5f74 656e 736f 7228 636c 732c 2078  ze_tensor(cls, x
-00008f30: 2920 2d3e 204f 7074 696f 6e61 6c5b 5f64  ) -> Optional[_d
-00008f40: 2e44 696d 5d3a 0a20 2020 2020 2020 2022  .Dim]:.        "
-00008f50: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-00008f60: 6d20 7466 2e54 656e 736f 7220 783a 2073  m tf.Tensor x: s
-00008f70: 697a 6520 7465 6e73 6f72 2e20 6861 7320  ize tensor. has 
-00008f80: 6265 656e 2073 6574 2062 6566 6f72 6520  been set before 
-00008f90: 7669 6120 3a66 756e 633a 6073 6574 5f74  via :func:`set_t
-00008fa0: 6167 5f6f 6e5f 7369 7a65 5f74 656e 736f  ag_on_size_tenso
-00008fb0: 7260 0a20 2020 2020 2020 2022 2222 0a20  r`.        """. 
-00008fc0: 2020 2020 2020 2072 6574 7572 6e20 6765         return ge
-00008fd0: 7461 7474 7228 782c 2022 5f69 735f 7369  tattr(x, "_is_si
-00008fe0: 7a65 5f6f 665f 6469 6d5f 7461 6722 2c20  ze_of_dim_tag", 
-00008ff0: 4e6f 6e65 290a 0a20 2020 2064 6566 2063  None)..    def c
-00009000: 6f6d 706c 6574 655f 6479 6e5f 7369 7a65  omplete_dyn_size
-00009010: 2873 656c 662c 2074 656d 706c 6174 655f  (self, template_
-00009020: 6f6e 6c79 3d46 616c 7365 293a 0a20 2020  only=False):.   
-00009030: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00009040: 2049 6e20 6361 7365 2077 6520 6361 6e20   In case we can 
-00009050: 6361 6c63 756c 6174 6520 7468 6520 6479  calculate the dy
-00009060: 6e20 7369 7a65 2c20 646f 2074 6861 7420  n size, do that 
-00009070: 6e6f 772e 0a0a 2020 2020 2020 2020 3a70  now...        :p
-00009080: 6172 616d 2062 6f6f 6c20 7465 6d70 6c61  aram bool templa
-00009090: 7465 5f6f 6e6c 793a 0a20 2020 2020 2020  te_only:.       
-000090a0: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-000090b0: 6e6f 7420 7365 6c66 2e69 735f 6479 6e61  not self.is_dyna
-000090c0: 6d69 6328 293a 0a20 2020 2020 2020 2020  mic():.         
-000090d0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-000090e0: 2020 7365 6c66 2e5f 7661 6c69 6461 7465    self._validate
-000090f0: 5f69 6e5f 6375 7272 656e 745f 6772 6170  _in_current_grap
-00009100: 6828 290a 2020 2020 2020 2020 6966 2073  h().        if s
-00009110: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-00009120: 2061 6e64 2028 7365 6c66 2e64 796e 5f73   and (self.dyn_s
-00009130: 697a 655f 6578 742e 706c 6163 6568 6f6c  ize_ext.placehol
-00009140: 6465 7220 6973 206e 6f74 204e 6f6e 6520  der is not None 
-00009150: 6f72 2074 656d 706c 6174 655f 6f6e 6c79  or template_only
-00009160: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00009170: 6574 7572 6e0a 2020 2020 2020 2020 7361  eturn.        sa
-00009180: 6d65 5f62 6173 6520 3d20 7365 6c66 2e67  me_base = self.g
-00009190: 6574 5f73 616d 655f 6261 7365 2829 0a20  et_same_base(). 
-000091a0: 2020 2020 2020 206f 7020 3d20 7365 6c66         op = self
-000091b0: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-000091c0: 206f 7220 7361 6d65 5f62 6173 652e 6465   or same_base.de
-000091d0: 7269 7665 645f 6672 6f6d 5f6f 700a 2020  rived_from_op.  
-000091e0: 2020 2020 2020 6966 206e 6f74 206f 703a        if not op:
-000091f0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00009200: 7572 6e0a 0a20 2020 2020 2020 2066 6f72  urn..        for
-00009210: 2078 2069 6e20 6f70 2e69 6e70 7574 733a   x in op.inputs:
-00009220: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00009230: 7365 6c66 2e62 6174 6368 3a0a 2020 2020  self.batch:.    
-00009240: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
-00009250: 782e 6765 745f 666f 725f 6261 7463 685f  x.get_for_batch_
-00009260: 6374 7828 7365 6c66 2e62 6174 6368 2c20  ctx(self.batch, 
-00009270: 7365 6c66 2e63 6f6e 7472 6f6c 5f66 6c6f  self.control_flo
-00009280: 775f 6374 7829 0a20 2020 2020 2020 2020  w_ctx).         
-00009290: 2020 2078 2e63 6f6d 706c 6574 655f 6479     x.complete_dy
-000092a0: 6e5f 7369 7a65 2874 656d 706c 6174 655f  n_size(template_
-000092b0: 6f6e 6c79 3d74 656d 706c 6174 655f 6f6e  only=template_on
-000092c0: 6c79 290a 0a20 2020 2020 2020 2062 6163  ly)..        bac
-000092d0: 6b65 6e64 203d 204e 6f6e 650a 2020 2020  kend = None.    
-000092e0: 2020 2020 666f 7220 7820 696e 206f 702e      for x in op.
-000092f0: 696e 7075 7473 3a0a 2020 2020 2020 2020  inputs:.        
-00009300: 2020 2020 6966 2073 656c 662e 6261 7463      if self.batc
-00009310: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
-00009320: 2020 2078 203d 2078 2e67 6574 5f66 6f72     x = x.get_for
-00009330: 5f62 6174 6368 5f63 7478 2873 656c 662e  _batch_ctx(self.
-00009340: 6261 7463 682c 2073 656c 662e 636f 6e74  batch, self.cont
-00009350: 726f 6c5f 666c 6f77 5f63 7478 290a 2020  rol_flow_ctx).  
-00009360: 2020 2020 2020 2020 2020 6966 2078 2e64            if x.d
-00009370: 796e 5f73 697a 655f 6578 7420 616e 6420  yn_size_ext and 
-00009380: 782e 6479 6e5f 7369 7a65 5f65 7874 2e72  x.dyn_size_ext.r
-00009390: 6177 5f74 656e 736f 7220 6973 206e 6f74  aw_tensor is not
-000093a0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-000093b0: 2020 2020 2020 2023 206e 6f69 6e73 7065         # noinspe
-000093c0: 6374 696f 6e20 5079 5072 6f74 6563 7465  ction PyProtecte
-000093d0: 644d 656d 6265 720a 2020 2020 2020 2020  dMember.        
-000093e0: 2020 2020 2020 2020 6261 636b 656e 6420          backend 
-000093f0: 3d20 782e 6479 6e5f 7369 7a65 5f65 7874  = x.dyn_size_ext
-00009400: 2e5f 7261 775f 6261 636b 656e 640a 2020  ._raw_backend.  
-00009410: 2020 2020 2020 2020 2020 2020 2020 6272                br
-00009420: 6561 6b0a 0a20 2020 2020 2020 2073 697a  eak..        siz
-00009430: 655f 6474 7970 6520 3d20 4e6f 6e65 0a20  e_dtype = None. 
-00009440: 2020 2020 2020 2066 6f72 2078 2069 6e20         for x in 
-00009450: 6f70 2e69 6e70 7574 733a 0a20 2020 2020  op.inputs:.     
-00009460: 2020 2020 2020 2069 6620 7365 6c66 2e62         if self.b
-00009470: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
-00009480: 2020 2020 2020 7820 3d20 782e 6765 745f        x = x.get_
-00009490: 666f 725f 6261 7463 685f 6374 7828 7365  for_batch_ctx(se
-000094a0: 6c66 2e62 6174 6368 2c20 7365 6c66 2e63  lf.batch, self.c
-000094b0: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 7829  ontrol_flow_ctx)
-000094c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000094d0: 782e 6479 6e5f 7369 7a65 5f65 7874 3a0a  x.dyn_size_ext:.
-000094e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000094f0: 7369 7a65 5f64 7479 7065 203d 2078 2e64  size_dtype = x.d
-00009500: 796e 5f73 697a 655f 6578 742e 6474 7970  yn_size_ext.dtyp
-00009510: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-00009520: 2020 6272 6561 6b0a 2020 2020 2020 2020    break.        
-00009530: 6966 206e 6f74 2073 697a 655f 6474 7970  if not size_dtyp
-00009540: 653a 0a20 2020 2020 2020 2020 2020 2073  e:.            s
-00009550: 697a 655f 6474 7970 6520 3d20 5f74 2e54  ize_dtype = _t.T
-00009560: 656e 736f 722e 7369 7a65 5f64 7479 7065  ensor.size_dtype
-00009570: 0a0a 2020 2020 2020 2020 696d 706f 7274  ..        import
-00009580: 206e 756d 7079 0a20 2020 2020 2020 2069   numpy.        i
-00009590: 6d70 6f72 7420 7265 7475 726e 6e2e 6672  mport returnn.fr
-000095a0: 6f6e 7465 6e64 2061 7320 7266 0a0a 2020  ontend as rf..  
-000095b0: 2020 2020 2020 7466 203d 2074 665f 7574        tf = tf_ut
-000095c0: 696c 203d 2074 656e 736f 725f 7574 696c  il = tensor_util
-000095d0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-000095e0: 6966 2062 6163 6b65 6e64 2061 6e64 2062  if backend and b
-000095f0: 6163 6b65 6e64 2e69 735f 7465 6e73 6f72  ackend.is_tensor
-00009600: 666c 6f77 3a0a 2020 2020 2020 2020 2020  flow:.          
-00009610: 2020 696d 706f 7274 2074 656e 736f 7266    import tensorf
-00009620: 6c6f 7720 6173 2074 660a 0a20 2020 2020  low as tf..     
-00009630: 2020 2020 2020 2069 6620 6261 636b 656e         if backen
-00009640: 642e 5261 7754 656e 736f 7254 7970 6520  d.RawTensorType 
-00009650: 3d3d 2074 662e 5465 6e73 6f72 3a0a 2020  == tf.Tensor:.  
-00009660: 2020 2020 2020 2020 2020 2020 2020 6672                fr
-00009670: 6f6d 2072 6574 7572 6e6e 2e74 662e 7574  om returnn.tf.ut
-00009680: 696c 2069 6d70 6f72 7420 6261 7369 6320  il import basic 
-00009690: 6173 2074 665f 7574 696c 0a20 2020 2020  as tf_util.     
-000096a0: 2020 2020 2020 2020 2020 2066 726f 6d20             from 
-000096b0: 7465 6e73 6f72 666c 6f77 2e70 7974 686f  tensorflow.pytho
-000096c0: 6e2e 6672 616d 6577 6f72 6b20 696d 706f  n.framework impo
-000096d0: 7274 2074 656e 736f 725f 7574 696c 0a20  rt tensor_util. 
-000096e0: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
-000096f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009700: 2074 6620 3d20 4e6f 6e65 0a0a 2020 2020   tf = None..    
-00009710: 2020 2020 6b69 6e64 203d 206f 702e 6b69      kind = op.ki
-00009720: 6e64 0a20 2020 2020 2020 2069 6620 6b69  nd.        if ki
-00009730: 6e64 2e65 6e64 7377 6974 6828 225f 7269  nd.endswith("_ri
-00009740: 6768 7422 293a 0a20 2020 2020 2020 2020  ght"):.         
-00009750: 2020 206b 696e 6420 3d20 6b69 6e64 5b3a     kind = kind[:
-00009760: 202d 6c65 6e28 225f 7269 6768 7422 295d   -len("_right")]
-00009770: 2020 2320 6f72 6465 7220 646f 6573 206e    # order does n
-00009780: 6f74 206d 6174 7465 7220 6865 7265 0a20  ot matter here. 
-00009790: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
-000097a0: 6e64 7377 6974 6828 225f 6c65 6674 2229  ndswith("_left")
-000097b0: 3a0a 2020 2020 2020 2020 2020 2020 6b69  :.            ki
-000097c0: 6e64 203d 206b 696e 645b 3a20 2d6c 656e  nd = kind[: -len
-000097d0: 2822 5f6c 6566 7422 295d 0a0a 2020 2020  ("_left")]..    
-000097e0: 2020 2020 6465 6620 5f69 735f 6e65 6761      def _is_nega
-000097f0: 7469 7665 2878 5f5f 293a 0a20 2020 2020  tive(x__):.     
-00009800: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-00009810: 616e 6365 2878 5f5f 2c20 6e75 6d70 792e  ance(x__, numpy.
-00009820: 6e64 6172 7261 7929 3a0a 2020 2020 2020  ndarray):.      
-00009830: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009840: 2028 785f 5f20 3c20 3029 2e61 6e79 2829   (x__ < 0).any()
-00009850: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00009860: 6973 696e 7374 616e 6365 2878 5f5f 2c20  isinstance(x__, 
-00009870: 2869 6e74 2c20 666c 6f61 742c 206e 756d  (int, float, num
-00009880: 7079 2e6e 756d 6265 7229 293a 0a20 2020  py.number)):.   
-00009890: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-000098a0: 7572 6e20 785f 5f20 3c20 300a 2020 2020  urn x__ < 0.    
-000098b0: 2020 2020 2020 2020 6966 206e 6f74 2074          if not t
-000098c0: 663a 0a20 2020 2020 2020 2020 2020 2020  f:.             
-000098d0: 2020 2072 6574 7572 6e20 4661 6c73 650a     return False.
-000098e0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-000098f0: 7274 2069 7369 6e73 7461 6e63 6528 785f  rt isinstance(x_
-00009900: 5f2c 2074 662e 5465 6e73 6f72 290a 2020  _, tf.Tensor).  
-00009910: 2020 2020 2020 2020 2020 785f 5f20 3d20            x__ = 
-00009920: 7465 6e73 6f72 5f75 7469 6c2e 636f 6e73  tensor_util.cons
-00009930: 7461 6e74 5f76 616c 7565 2878 5f5f 290a  tant_value(x__).
-00009940: 2020 2020 2020 2020 2020 2020 6966 2078              if x
-00009950: 5f5f 2069 7320 6e6f 7420 4e6f 6e65 3a0a  __ is not None:.
+000051c0: 6672 6f6d 2072 6574 7572 6e6e 2e74 662e  from returnn.tf.
+000051d0: 7574 696c 2e62 6173 6963 2069 6d70 6f72  util.basic impor
+000051e0: 7420 6765 745f 7661 6c69 645f 7363 6f70  t get_valid_scop
+000051f0: 655f 6e61 6d65 5f66 726f 6d5f 7374 722c  e_name_from_str,
+00005200: 2073 616d 655f 636f 6e74 726f 6c5f 666c   same_control_fl
+00005210: 6f77 5f63 7478 0a0a 2020 2020 2020 2020  ow_ctx..        
+00005220: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005230: 7769 7468 2073 616d 655f 636f 6e74 726f  with same_contro
+00005240: 6c5f 666c 6f77 5f63 7478 2864 796e 5f73  l_flow_ctx(dyn_s
+00005250: 697a 655f 6578 742e 706c 6163 6568 6f6c  ize_ext.placehol
+00005260: 6465 7229 3a0a 2020 2020 2020 2020 2020  der):.          
+00005270: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005280: 2020 6479 6e5f 7369 7a65 5f65 7874 2e70    dyn_size_ext.p
+00005290: 6c61 6365 686f 6c64 6572 203d 2074 662e  laceholder = tf.
+000052a0: 6964 656e 7469 7479 280a 2020 2020 2020  identity(.      
+000052b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000052c0: 2020 2020 2020 2020 2020 6479 6e5f 7369            dyn_si
+000052d0: 7a65 5f65 7874 2e70 6c61 6365 686f 6c64  ze_ext.placehold
+000052e0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+000052f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005300: 2020 2020 6e61 6d65 3d67 6574 5f76 616c      name=get_val
+00005310: 6964 5f73 636f 7065 5f6e 616d 655f 6672  id_scope_name_fr
+00005320: 6f6d 5f73 7472 280a 2020 2020 2020 2020  om_str(.        
+00005330: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005340: 2020 2020 2020 2020 2020 2020 2225 735f              "%s_
+00005350: 6765 745f 666f 725f 6261 7463 685f 6374  get_for_batch_ct
+00005360: 785f 2573 2220 2520 2864 796e 5f73 697a  x_%s" % (dyn_siz
+00005370: 655f 6578 742e 6e61 6d65 2c20 6261 7463  e_ext.name, batc
+00005380: 682e 7368 6f72 745f 7265 7072 2829 290a  h.short_repr()).
+00005390: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000053b0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+000053c0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000053d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000053e0: 2020 2020 2020 2020 2069 6620 6261 7463           if batc
+000053f0: 682e 6265 616d 3a0a 2020 2020 2020 2020  h.beam:.        
+00005400: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005410: 2020 2020 6479 6e5f 7369 7a65 5f65 7874      dyn_size_ext
+00005420: 2e70 6c61 6365 686f 6c64 6572 2e5f 5245  .placeholder._RE
+00005430: 5455 524e 4e5f 6479 6e5f 7369 7a65 5f62  TURNN_dyn_size_b
+00005440: 6561 6d20 3d20 6261 7463 682e 6265 616d  eam = batch.beam
+00005450: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005460: 2020 2020 2020 2020 2020 2020 2064 796e               dyn
+00005470: 5f73 697a 655f 6578 742e 706c 6163 6568  _size_ext.placeh
+00005480: 6f6c 6465 722e 5f52 4554 5552 4e4e 5f62  older._RETURNN_b
+00005490: 6561 6d5f 6578 7061 6e64 6564 5f62 6173  eam_expanded_bas
+000054a0: 655f 6461 7461 203d 2062 6561 6d5f 6578  e_data = beam_ex
+000054b0: 7061 6e64 6564 5f62 6173 655f 6461 7461  panded_base_data
+000054c0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+000054d0: 6479 6e5f 7369 7a65 5f65 7874 2061 6e64  dyn_size_ext and
+000054e0: 2061 6c6c 6f77 5f6e 6f6e 6520 616e 6420   allow_none and 
+000054f0: 6e6f 7420 7361 6d65 5f62 6173 652e 6465  not same_base.de
+00005500: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
+00005510: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00005520: 6e20 4e6f 6e65 0a20 2020 2020 2020 2069  n None.        i
+00005530: 6620 6e6f 7420 6479 6e5f 7369 7a65 5f65  f not dyn_size_e
+00005540: 7874 2061 6e64 2073 616d 655f 6261 7365  xt and same_base
+00005550: 5f65 7874 7261 2e73 616d 655f 666f 725f  _extra.same_for_
+00005560: 6261 7463 685f 6374 783a 0a20 2020 2020  batch_ctx:.     
+00005570: 2020 2020 2020 2023 2054 6865 7265 2061         # There a
+00005580: 7265 2065 6172 6c69 6572 2065 6e74 7269  re earlier entri
+00005590: 6573 2069 6e20 5f73 616d 655f 666f 725f  es in _same_for_
+000055a0: 6261 7463 685f 6374 780a 2020 2020 2020  batch_ctx.      
+000055b0: 2020 2020 2020 2320 2d2d 206d 6179 6265        # -- maybe
+000055c0: 2077 6520 6361 6e20 696e 6665 7220 6479   we can infer dy
+000055d0: 6e5f 7369 7a65 5f65 7874 2c20 6576 656e  n_size_ext, even
+000055e0: 2077 6974 6820 6469 6666 6572 656e 7420   with different 
+000055f0: 6261 7463 682e 0a20 2020 2020 2020 2020  batch..         
+00005600: 2020 2066 6f72 2028 6261 7463 685f 2c20     for (batch_, 
+00005610: 6374 785f 292c 206f 7468 6572 2069 6e20  ctx_), other in 
+00005620: 7361 6d65 5f62 6173 655f 6578 7472 612e  same_base_extra.
+00005630: 7361 6d65 5f66 6f72 5f62 6174 6368 5f63  same_for_batch_c
+00005640: 7478 2e69 7465 6d73 2829 3a0a 2020 2020  tx.items():.    
+00005650: 2020 2020 2020 2020 2020 2020 6966 2063              if c
+00005660: 7478 5f20 3d3d 2063 7478 2061 6e64 206f  tx_ == ctx and o
+00005670: 7468 6572 2e64 796e 5f73 697a 655f 6578  ther.dyn_size_ex
+00005680: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00005690: 2020 2020 2020 2064 796e 5f73 697a 655f         dyn_size_
+000056a0: 6578 7420 3d20 6f74 6865 722e 6479 6e5f  ext = other.dyn_
+000056b0: 7369 7a65 5f65 7874 2e63 6f70 795f 7465  size_ext.copy_te
+000056c0: 6d70 6c61 7465 2829 0a20 2020 2020 2020  mplate().       
+000056d0: 2020 2020 2020 2020 2020 2020 2064 796e               dyn
+000056e0: 5f73 697a 655f 6578 742e 6265 616d 203d  _size_ext.beam =
+000056f0: 2062 6174 6368 2e62 6561 6d0a 2020 2020   batch.beam.    
+00005700: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005710: 6479 6e5f 7369 7a65 5f65 7874 2e62 6174  dyn_size_ext.bat
+00005720: 6368 203d 2062 6174 6368 0a20 2020 2020  ch = batch.     
+00005730: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00005740: 7265 616b 0a20 2020 2020 2020 2063 7478  reak.        ctx
+00005750: 203d 2064 796e 5f73 697a 655f 6578 742e   = dyn_size_ext.
+00005760: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
+00005770: 2069 6620 6479 6e5f 7369 7a65 5f65 7874   if dyn_size_ext
+00005780: 2065 6c73 6520 6374 780a 2020 2020 2020   else ctx.      
+00005790: 2020 6469 6d5f 7461 6720 3d20 4e6f 6e65    dim_tag = None
+000057a0: 0a20 2020 2020 2020 2066 6f72 2063 616e  .        for can
+000057b0: 6469 6461 7465 2069 6e20 5b73 656c 662c  didate in [self,
+000057c0: 2073 616d 655f 6261 7365 5d3a 0a20 2020   same_base]:.   
+000057d0: 2020 2020 2020 2020 2069 6620 280a 2020           if (.  
+000057e0: 2020 2020 2020 2020 2020 2020 2020 2863                (c
+000057f0: 616e 6469 6461 7465 2e62 6174 6368 203d  andidate.batch =
+00005800: 3d20 6261 7463 6820 6f72 2028 6e6f 7420  = batch or (not 
+00005810: 6361 6e64 6964 6174 652e 6261 7463 6820  candidate.batch 
+00005820: 616e 6420 6261 7463 682e 6973 5f67 6c6f  and batch.is_glo
+00005830: 6261 6c5f 6261 7463 6828 2929 290a 2020  bal_batch())).  
+00005840: 2020 2020 2020 2020 2020 2020 2020 616e                an
+00005850: 6420 6e6f 7420 6361 6e64 6964 6174 652e  d not candidate.
+00005860: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
+00005870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005880: 2061 6e64 206e 6f74 2063 7478 0a20 2020   and not ctx.   
+00005890: 2020 2020 2020 2020 2029 3a0a 2020 2020           ):.    
+000058a0: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
+000058b0: 6520 7361 6d65 5f62 6173 6520 696e 7374  e same_base inst
+000058c0: 616e 6365 2069 7320 6569 7468 6572 2075  ance is either u
+000058d0: 6e64 6566 696e 6564 2028 6e6f 2062 6174  ndefined (no bat
+000058e0: 6368 2c20 6e6f 2063 7478 290a 2020 2020  ch, no ctx).    
+000058f0: 2020 2020 2020 2020 2020 2020 2320 6f72              # or
+00005900: 2069 7420 6973 2064 6566 696e 6564 2066   it is defined f
+00005910: 6f72 2074 6865 2073 616d 6520 6261 7463  or the same batc
+00005920: 6820 616e 6420 6374 782e 0a20 2020 2020  h and ctx..     
+00005930: 2020 2020 2020 2020 2020 2023 2049 6e20             # In 
+00005940: 616e 7920 6361 7365 2c20 7265 7573 6520  any case, reuse 
+00005950: 6974 2074 6865 6e2e 0a20 2020 2020 2020  it then..       
+00005960: 2020 2020 2020 2020 2063 616e 6469 6461           candida
+00005970: 7465 2e62 6174 6368 203d 2062 6174 6368  te.batch = batch
+00005980: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005990: 2069 6620 6479 6e5f 7369 7a65 5f65 7874   if dyn_size_ext
+000059a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000059b0: 2020 2020 2020 6966 2063 616e 6469 6461        if candida
+000059c0: 7465 2e64 796e 5f73 697a 655f 6578 743a  te.dyn_size_ext:
+000059d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000059e0: 2020 2020 2020 2020 2063 616e 6469 6461           candida
+000059f0: 7465 2e64 796e 5f73 697a 655f 6578 742e  te.dyn_size_ext.
+00005a00: 6261 7463 6820 3d20 6261 7463 680a 2020  batch = batch.  
+00005a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a20: 2020 2020 2020 6173 7365 7274 2063 616e        assert can
+00005a30: 6469 6461 7465 2e64 796e 5f73 697a 655f  didate.dyn_size_
+00005a40: 6578 742e 6469 6d5f 7461 6773 203d 3d20  ext.dim_tags == 
+00005a50: 6479 6e5f 7369 7a65 5f65 7874 2e64 696d  dyn_size_ext.dim
+00005a60: 5f74 6167 730a 2020 2020 2020 2020 2020  _tags.          
+00005a70: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00005a80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005a90: 2020 2020 2020 2020 6361 6e64 6964 6174          candidat
+00005aa0: 652e 6479 6e5f 7369 7a65 5f65 7874 203d  e.dyn_size_ext =
+00005ab0: 2064 796e 5f73 697a 655f 6578 740a 2020   dyn_size_ext.  
+00005ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ad0: 2020 6173 7365 7274 206e 6f74 2063 616e    assert not can
+00005ae0: 6469 6461 7465 2e64 796e 5f73 697a 655f  didate.dyn_size_
+00005af0: 6578 742e 636f 6e74 726f 6c5f 666c 6f77  ext.control_flow
+00005b00: 5f63 7478 0a20 2020 2020 2020 2020 2020  _ctx.           
+00005b10: 2020 2020 2065 6c69 6620 6361 6e64 6964       elif candid
+00005b20: 6174 652e 6479 6e5f 7369 7a65 5f65 7874  ate.dyn_size_ext
+00005b30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00005b40: 2020 2020 2020 6361 6e64 6964 6174 652e        candidate.
+00005b50: 6479 6e5f 7369 7a65 5f65 7874 2e62 6174  dyn_size_ext.bat
+00005b60: 6368 203d 2062 6174 6368 0a20 2020 2020  ch = batch.     
+00005b70: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00005b80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005b90: 2020 2020 2063 616e 6469 6461 7465 2e63       candidate.c
+00005ba0: 6f6d 706c 6574 655f 6479 6e5f 7369 7a65  omplete_dyn_size
+00005bb0: 2874 656d 706c 6174 655f 6f6e 6c79 3d54  (template_only=T
+00005bc0: 7275 6529 0a20 2020 2020 2020 2020 2020  rue).           
+00005bd0: 2020 2020 2064 696d 5f74 6167 203d 2063       dim_tag = c
+00005be0: 616e 6469 6461 7465 0a20 2020 2020 2020  andidate.       
+00005bf0: 2020 2020 2020 2020 2062 7265 616b 0a20           break. 
+00005c00: 2020 2020 2020 2069 6620 6e6f 7420 6469         if not di
+00005c10: 6d5f 7461 673a 0a20 2020 2020 2020 2020  m_tag:.         
+00005c20: 2020 2064 696d 5f74 6167 203d 205f 642e     dim_tag = _d.
+00005c30: 4469 6d28 0a20 2020 2020 2020 2020 2020  Dim(.           
+00005c40: 2020 2020 206b 696e 643d 7365 6c66 2e6b       kind=self.k
+00005c50: 696e 642c 0a20 2020 2020 2020 2020 2020  ind,.           
+00005c60: 2020 2020 2064 6573 6372 6970 7469 6f6e       description
+00005c70: 3d73 656c 662e 6465 7363 7269 7074 696f  =self.descriptio
+00005c80: 6e2c 0a20 2020 2020 2020 2020 2020 2020  n,.             
+00005c90: 2020 2064 696d 656e 7369 6f6e 3d73 656c     dimension=sel
+00005ca0: 662e 6469 6d65 6e73 696f 6e2c 0a20 2020  f.dimension,.   
+00005cb0: 2020 2020 2020 2020 2020 2020 2061 7574               aut
+00005cc0: 6f5f 6765 6e65 7261 7465 643d 7365 6c66  o_generated=self
+00005cd0: 2e61 7574 6f5f 6765 6e65 7261 7465 642c  .auto_generated,
+00005ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005cf0: 2062 6174 6368 3d62 6174 6368 2c0a 2020   batch=batch,.  
+00005d00: 2020 2020 2020 2020 2020 2020 2020 636f                co
+00005d10: 6e74 726f 6c5f 666c 6f77 5f63 7478 3d63  ntrol_flow_ctx=c
+00005d20: 7478 2c0a 2020 2020 2020 2020 2020 2020  tx,.            
+00005d30: 2020 2020 6479 6e5f 7369 7a65 5f65 7874      dyn_size_ext
+00005d40: 3d64 796e 5f73 697a 655f 6578 742c 0a20  =dyn_size_ext,. 
+00005d50: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+00005d60: 2020 2020 2020 2020 2064 696d 5f74 6167           dim_tag
+00005d70: 2e73 616d 655f 6173 203d 2073 616d 655f  .same_as = same_
+00005d80: 6261 7365 0a20 2020 2020 2020 2069 6620  base.        if 
+00005d90: 6479 6e5f 7369 7a65 5f65 7874 2061 6e64  dyn_size_ext and
+00005da0: 2064 796e 5f73 697a 655f 6578 742e 706c   dyn_size_ext.pl
+00005db0: 6163 6568 6f6c 6465 7220 6973 206e 6f74  aceholder is not
+00005dc0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00005dd0: 2020 2069 6620 5f64 2e44 696d 2e67 6574     if _d.Dim.get
+00005de0: 5f74 6167 5f66 726f 6d5f 7369 7a65 5f74  _tag_from_size_t
+00005df0: 656e 736f 7228 6479 6e5f 7369 7a65 5f65  ensor(dyn_size_e
+00005e00: 7874 2e70 6c61 6365 686f 6c64 6572 2920  xt.placeholder) 
+00005e10: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
+00005e20: 2020 2020 2020 2020 2064 696d 5f74 6167           dim_tag
+00005e30: 2e73 6574 5f74 6167 5f6f 6e5f 7369 7a65  .set_tag_on_size
+00005e40: 5f74 656e 736f 7228 6479 6e5f 7369 7a65  _tensor(dyn_size
+00005e50: 5f65 7874 2e70 6c61 6365 686f 6c64 6572  _ext.placeholder
+00005e60: 2c20 6261 7463 683d 6261 7463 6829 0a20  , batch=batch). 
+00005e70: 2020 2020 2020 2073 616d 655f 6261 7365         same_base
+00005e80: 5f65 7874 7261 2e73 616d 655f 666f 725f  _extra.same_for_
+00005e90: 6261 7463 685f 6374 785b 2862 6174 6368  batch_ctx[(batch
+00005ea0: 2c20 6374 7829 5d20 3d20 6469 6d5f 7461  , ctx)] = dim_ta
+00005eb0: 670a 2020 2020 2020 2020 6469 6d5f 7461  g.        dim_ta
+00005ec0: 672e 636f 6d70 6c65 7465 5f64 796e 5f73  g.complete_dyn_s
+00005ed0: 697a 6528 7465 6d70 6c61 7465 5f6f 6e6c  ize(template_onl
+00005ee0: 793d 5472 7565 290a 2020 2020 2020 2020  y=True).        
+00005ef0: 7265 7475 726e 2064 696d 5f74 6167 0a0a  return dim_tag..
+00005f00: 2020 2020 6465 6620 7265 7365 745f 6261      def reset_ba
+00005f10: 7463 685f 6374 7828 7365 6c66 3a20 4469  tch_ctx(self: Di
+00005f20: 6d29 3a0a 2020 2020 2020 2020 2222 220a  m):.        """.
+00005f30: 2020 2020 2020 2020 466f 7220 7468 6520          For the 
+00005f40: 7365 6c66 2069 6e73 7461 6e63 652c 2072  self instance, r
+00005f50: 6573 6574 2062 6174 6368 2061 6e64 2063  eset batch and c
+00005f60: 6f6e 7465 7874 2e0a 2020 2020 2020 2020  ontext..        
+00005f70: 2222 220a 2020 2020 2020 2020 6966 2073  """.        if s
+00005f80: 656c 662e 5f65 7874 7261 3a0a 2020 2020  elf._extra:.    
+00005f90: 2020 2020 2020 2020 7365 6c66 2e5f 6578          self._ex
+00005fa0: 7472 612e 7361 6d65 5f66 6f72 5f62 6174  tra.same_for_bat
+00005fb0: 6368 5f63 7478 2e70 6f70 2828 7365 6c66  ch_ctx.pop((self
+00005fc0: 2e62 6174 6368 2c20 7365 6c66 2e63 6f6e  .batch, self.con
+00005fd0: 7472 6f6c 5f66 6c6f 775f 6374 7829 2c20  trol_flow_ctx), 
+00005fe0: 4e6f 6e65 290a 2020 2020 2020 2020 7365  None).        se
+00005ff0: 6c66 2e62 6174 6368 203d 204e 6f6e 650a  lf.batch = None.
+00006000: 2020 2020 2020 2020 7365 6c66 2e63 6f6e          self.con
+00006010: 7472 6f6c 5f66 6c6f 775f 6374 7820 3d20  trol_flow_ctx = 
+00006020: 4e6f 6e65 0a20 2020 2020 2020 2069 6620  None.        if 
+00006030: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+00006040: 7420 616e 6420 7365 6c66 2e64 796e 5f73  t and self.dyn_s
+00006050: 697a 655f 6578 742e 6261 7463 683a 0a20  ize_ext.batch:. 
+00006060: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00006070: 6479 6e5f 7369 7a65 5f65 7874 203d 2073  dyn_size_ext = s
+00006080: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+00006090: 2e63 6f70 795f 7465 6d70 6c61 7465 2829  .copy_template()
+000060a0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+000060b0: 662e 6479 6e5f 7369 7a65 5f65 7874 2e62  f.dyn_size_ext.b
+000060c0: 6174 6368 203d 204e 6f6e 650a 0a20 2020  atch = None..   
+000060d0: 2064 6566 2073 6574 5f64 796e 5f73 697a   def set_dyn_siz
+000060e0: 655f 6578 745f 666f 725f 6261 7463 685f  e_ext_for_batch_
+000060f0: 6374 7828 7365 6c66 2c20 6261 7463 682c  ctx(self, batch,
+00006100: 2063 7478 2c20 6479 6e5f 7369 7a65 5f65   ctx, dyn_size_e
+00006110: 7874 293a 0a20 2020 2020 2020 2022 2222  xt):.        """
+00006120: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00006130: 4261 7463 6849 6e66 6f20 6261 7463 683a  BatchInfo batch:
+00006140: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00006150: 436f 6e74 726f 6c46 6c6f 7743 6f6e 7465  ControlFlowConte
+00006160: 7874 7c4e 6f6e 6520 6374 783a 0a20 2020  xt|None ctx:.   
+00006170: 2020 2020 203a 7061 7261 6d20 4461 7461       :param Data
+00006180: 2064 796e 5f73 697a 655f 6578 743a 0a20   dyn_size_ext:. 
+00006190: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000061a0: 2020 2061 7373 6572 7420 7365 6c66 2e63     assert self.c
+000061b0: 616e 5f62 655f 7573 6564 5f61 735f 6469  an_be_used_as_di
+000061c0: 6d28 290a 2020 2020 2020 2020 7361 6d65  m().        same
+000061d0: 203d 2073 656c 662e 6765 745f 666f 725f   = self.get_for_
+000061e0: 6261 7463 685f 6374 7828 6261 7463 682c  batch_ctx(batch,
+000061f0: 2063 7478 290a 2020 2020 2020 2020 6173   ctx).        as
+00006200: 7365 7274 2064 796e 5f73 697a 655f 6578  sert dyn_size_ex
+00006210: 742e 6261 7463 6820 3d3d 2062 6174 6368  t.batch == batch
+00006220: 2061 6e64 2064 796e 5f73 697a 655f 6578   and dyn_size_ex
+00006230: 742e 636f 6e74 726f 6c5f 666c 6f77 5f63  t.control_flow_c
+00006240: 7478 203d 3d20 6374 780a 2020 2020 2020  tx == ctx.      
+00006250: 2020 6966 2073 616d 652e 6479 6e5f 7369    if same.dyn_si
+00006260: 7a65 5f65 7874 3a0a 2020 2020 2020 2020  ze_ext:.        
+00006270: 2020 2020 6173 7365 7274 2073 616d 652e      assert same.
+00006280: 6479 6e5f 7369 7a65 5f65 7874 2e64 696d  dyn_size_ext.dim
+00006290: 5f74 6167 7320 3d3d 2064 796e 5f73 697a  _tags == dyn_siz
+000062a0: 655f 6578 742e 6469 6d5f 7461 6773 0a20  e_ext.dim_tags. 
+000062b0: 2020 2020 2020 2020 2020 2069 6620 6479             if dy
+000062c0: 6e5f 7369 7a65 5f65 7874 2e70 6c61 6365  n_size_ext.place
+000062d0: 686f 6c64 6572 2069 7320 6e6f 7420 4e6f  holder is not No
+000062e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000062f0: 2020 2020 7361 6d65 2e64 796e 5f73 697a      same.dyn_siz
+00006300: 655f 6578 742e 706c 6163 6568 6f6c 6465  e_ext.placeholde
+00006310: 7220 3d20 6479 6e5f 7369 7a65 5f65 7874  r = dyn_size_ext
+00006320: 2e70 6c61 6365 686f 6c64 6572 0a20 2020  .placeholder.   
+00006330: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00006340: 2020 2020 2020 2073 616d 652e 6479 6e5f         same.dyn_
+00006350: 7369 7a65 5f65 7874 203d 2064 796e 5f73  size_ext = dyn_s
+00006360: 697a 655f 6578 740a 2020 2020 2020 2020  ize_ext.        
+00006370: 7365 6c66 2e5f 6d61 7962 655f 7570 6461  self._maybe_upda
+00006380: 7465 2829 0a0a 2020 2020 6465 6620 6765  te()..    def ge
+00006390: 745f 6479 6e5f 7369 7a65 5f65 7874 5f66  t_dyn_size_ext_f
+000063a0: 6f72 5f62 6174 6368 5f63 7478 2873 656c  or_batch_ctx(sel
+000063b0: 662c 2062 6174 6368 2c20 6374 782c 2074  f, batch, ctx, t
+000063c0: 656d 706c 6174 655f 6f6e 6c79 3d46 616c  emplate_only=Fal
+000063d0: 7365 293a 0a20 2020 2020 2020 2022 2222  se):.        """
+000063e0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000063f0: 4261 7463 6849 6e66 6f7c 4e6f 6e65 2062  BatchInfo|None b
+00006400: 6174 6368 3a0a 2020 2020 2020 2020 3a70  atch:.        :p
+00006410: 6172 616d 2043 6f6e 7472 6f6c 466c 6f77  aram ControlFlow
+00006420: 436f 6e74 6578 747c 4e6f 6e65 2063 7478  Context|None ctx
+00006430: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
+00006440: 2062 6f6f 6c20 7465 6d70 6c61 7465 5f6f   bool template_o
+00006450: 6e6c 793a 0a20 2020 2020 2020 203a 7274  nly:.        :rt
+00006460: 7970 653a 2044 6174 617c 4e6f 6e65 0a20  ype: Data|None. 
+00006470: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00006480: 2020 2061 7373 6572 7420 7365 6c66 2e63     assert self.c
+00006490: 616e 5f62 655f 7573 6564 5f61 735f 6469  an_be_used_as_di
+000064a0: 6d28 290a 2020 2020 2020 2020 6966 206e  m().        if n
+000064b0: 6f74 2062 6174 6368 2061 6e64 2073 656c  ot batch and sel
+000064c0: 662e 6261 7463 683a 0a20 2020 2020 2020  f.batch:.       
+000064d0: 2020 2020 2023 2041 7373 756d 6520 676c       # Assume gl
+000064e0: 6f62 616c 2062 6174 6368 2e0a 2020 2020  obal batch..    
+000064f0: 2020 2020 2020 2020 6261 7463 6820 3d20          batch = 
+00006500: 7365 6c66 2e62 6174 6368 2e67 6574 5f67  self.batch.get_g
+00006510: 6c6f 6261 6c5f 6261 7365 2829 0a20 2020  lobal_base().   
+00006520: 2020 2020 2069 6620 6e6f 7420 6261 7463       if not batc
+00006530: 683a 0a20 2020 2020 2020 2020 2020 2023  h:.            #
+00006540: 2054 6869 7320 6973 2075 7375 616c 6c79   This is usually
+00006550: 206e 6f74 2076 616c 6964 2e20 486f 7765   not valid. Howe
+00006560: 7665 722c 2074 6869 7320 6361 7365 2063  ver, this case c
+00006570: 616e 2068 6170 7065 6e20 6561 726c 7920  an happen early 
+00006580: 6174 2069 6e69 7469 616c 697a 6174 696f  at initializatio
+00006590: 6e2e 0a20 2020 2020 2020 2020 2020 2061  n..            a
+000065a0: 7373 6572 7420 6261 7463 6820 3d3d 2073  ssert batch == s
+000065b0: 656c 662e 6261 7463 6820 616e 6420 6374  elf.batch and ct
+000065c0: 7820 3d3d 2073 656c 662e 636f 6e74 726f  x == self.contro
+000065d0: 6c5f 666c 6f77 5f63 7478 0a20 2020 2020  l_flow_ctx.     
+000065e0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+000065f0: 6c66 2e64 796e 5f73 697a 655f 6578 740a  lf.dyn_size_ext.
+00006600: 2020 2020 2020 2020 7361 6d65 203d 2073          same = s
+00006610: 656c 662e 6765 745f 666f 725f 6261 7463  elf.get_for_batc
+00006620: 685f 6374 7828 6261 7463 682c 2063 7478  h_ctx(batch, ctx
+00006630: 2c20 616c 6c6f 775f 6e6f 6e65 3d54 7275  , allow_none=Tru
+00006640: 6529 0a20 2020 2020 2020 2069 6620 6e6f  e).        if no
+00006650: 7420 7361 6d65 3a0a 2020 2020 2020 2020  t same:.        
+00006660: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00006670: 2020 2020 2020 2020 7361 6d65 2e63 6f6d          same.com
+00006680: 706c 6574 655f 6479 6e5f 7369 7a65 2874  plete_dyn_size(t
+00006690: 656d 706c 6174 655f 6f6e 6c79 3d74 656d  emplate_only=tem
+000066a0: 706c 6174 655f 6f6e 6c79 290a 2020 2020  plate_only).    
+000066b0: 2020 2020 7265 7475 726e 2073 616d 652e      return same.
+000066c0: 6479 6e5f 7369 7a65 5f65 7874 0a0a 2020  dyn_size_ext..  
+000066d0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+000066e0: 6465 6620 6479 6e5f 7369 7a65 2873 656c  def dyn_size(sel
+000066f0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
+00006700: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+00006710: 2064 796e 2073 697a 6520 2f20 7365 7120   dyn size / seq 
+00006720: 6c65 6e20 2875 7375 616c 6c79 206f 6620  len (usually of 
+00006730: 7368 6170 6520 5b42 5d29 2c20 6f72 204e  shape [B]), or N
+00006740: 6f6e 650a 2020 2020 2020 2020 2020 4966  one.          If
+00006750: 2074 6865 2064 796e 2073 697a 6520 6361   the dyn size ca
+00006760: 6e20 706f 7465 6e74 6961 6c6c 7920 6265  n potentially be
+00006770: 206f 6620 6120 6469 6666 6572 656e 7420   of a different 
+00006780: 7368 6170 652c 2064 6972 6563 746c 7920  shape, directly 
+00006790: 6163 6365 7373 2064 796e 5f73 697a 655f  access dyn_size_
+000067a0: 6578 742e 0a20 2020 2020 2020 203a 7274  ext..        :rt
+000067b0: 7970 653a 2074 662e 5465 6e73 6f72 7c4e  ype: tf.Tensor|N
+000067c0: 6f6e 650a 2020 2020 2020 2020 2222 220a  one.        """.
+000067d0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000067e0: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
+000067f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00006800: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
+00006810: 7874 2e70 6c61 6365 686f 6c64 6572 0a20  xt.placeholder. 
+00006820: 2020 2020 2020 2072 6574 7572 6e20 4e6f         return No
+00006830: 6e65 0a0a 2020 2020 4064 796e 5f73 697a  ne..    @dyn_siz
+00006840: 652e 7365 7474 6572 0a20 2020 2064 6566  e.setter.    def
+00006850: 2064 796e 5f73 697a 6528 7365 6c66 2c20   dyn_size(self, 
+00006860: 6479 6e5f 7369 7a65 293a 0a20 2020 2020  dyn_size):.     
+00006870: 2020 2022 2222 0a20 2020 2020 2020 2041     """.        A
+00006880: 6c73 6f20 7365 6520 3a66 756e 633a 6073  lso see :func:`s
+00006890: 6574 5f64 796e 5f73 697a 655f 6578 745f  et_dyn_size_ext_
+000068a0: 666f 725f 6261 7463 685f 6374 7860 2e0a  for_batch_ctx`..
+000068b0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+000068c0: 7466 2e54 656e 736f 7220 6479 6e5f 7369  tf.Tensor dyn_si
+000068d0: 7a65 3a0a 2020 2020 2020 2020 2222 220a  ze:.        """.
+000068e0: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+000068f0: 6479 6e5f 7369 7a65 5f65 7874 2061 6e64  dyn_size_ext and
+00006900: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
+00006910: 7874 2e70 6c61 6365 686f 6c64 6572 2069  xt.placeholder i
+00006920: 7320 6479 6e5f 7369 7a65 3a20 2023 2066  s dyn_size:  # f
+00006930: 6173 7420 7061 7468 2063 6865 636b 0a20  ast path check. 
+00006940: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00006950: 6e0a 2020 2020 2020 2020 6173 7365 7274  n.        assert
+00006960: 2073 656c 662e 6361 6e5f 6265 5f75 7365   self.can_be_use
+00006970: 645f 6173 5f64 696d 2829 0a20 2020 2020  d_as_dim().     
+00006980: 2020 206f 7468 6572 203d 205f 642e 4469     other = _d.Di
+00006990: 6d2e 6765 745f 7461 675f 6672 6f6d 5f73  m.get_tag_from_s
+000069a0: 697a 655f 7465 6e73 6f72 2864 796e 5f73  ize_tensor(dyn_s
+000069b0: 697a 6529 0a20 2020 2020 2020 2069 6620  ize).        if 
+000069c0: 6f74 6865 723a 0a20 2020 2020 2020 2020  other:.         
+000069d0: 2020 2073 656c 662e 6465 636c 6172 655f     self.declare_
+000069e0: 7361 6d65 5f61 7328 6f74 6865 7229 0a20  same_as(other). 
+000069f0: 2020 2020 2020 2020 2020 2069 6620 7365             if se
+00006a00: 6c66 2e62 6174 6368 3a0a 2020 2020 2020  lf.batch:.      
+00006a10: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00006a20: 2073 656c 662e 6261 7463 6820 3d3d 206f   self.batch == o
+00006a30: 7468 6572 2e62 6174 6368 2061 6e64 2073  ther.batch and s
+00006a40: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
+00006a50: 5f63 7478 203d 3d20 6f74 6865 722e 636f  _ctx == other.co
+00006a60: 6e74 726f 6c5f 666c 6f77 5f63 7478 0a20  ntrol_flow_ctx. 
+00006a70: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+00006a80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006a90: 2073 656c 662e 6261 7463 6820 3d20 6f74   self.batch = ot
+00006aa0: 6865 722e 6261 7463 680a 2020 2020 2020  her.batch.      
+00006ab0: 2020 2020 2020 2020 2020 7365 6c66 2e63            self.c
+00006ac0: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 7820  ontrol_flow_ctx 
+00006ad0: 3d20 6f74 6865 722e 636f 6e74 726f 6c5f  = other.control_
+00006ae0: 666c 6f77 5f63 7478 0a20 2020 2020 2020  flow_ctx.       
+00006af0: 2020 2020 2073 656c 662e 6479 6e5f 7369       self.dyn_si
+00006b00: 7a65 5f65 7874 203d 206f 7468 6572 2e64  ze_ext = other.d
+00006b10: 796e 5f73 697a 655f 6578 740a 2020 2020  yn_size_ext.    
+00006b20: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00006b30: 2020 2020 2020 2073 656c 662e 5f69 6e69         self._ini
+00006b40: 745f 6465 6661 756c 745f 6479 6e5f 7369  t_default_dyn_si
+00006b50: 7a65 5f65 7874 2864 796e 5f73 697a 6529  ze_ext(dyn_size)
+00006b60: 0a20 2020 2020 2020 2073 656c 662e 7365  .        self.se
+00006b70: 745f 7461 675f 6f6e 5f73 697a 655f 7465  t_tag_on_size_te
+00006b80: 6e73 6f72 2864 796e 5f73 697a 6529 0a0a  nsor(dyn_size)..
+00006b90: 2020 2020 6465 6620 5f69 6e69 745f 6465      def _init_de
+00006ba0: 6661 756c 745f 6479 6e5f 7369 7a65 5f65  fault_dyn_size_e
+00006bb0: 7874 2873 656c 662c 2064 796e 5f73 697a  xt(self, dyn_siz
+00006bc0: 6529 3a0a 2020 2020 2020 2020 2222 220a  e):.        """.
+00006bd0: 2020 2020 2020 2020 3a70 6172 616d 2074          :param t
+00006be0: 662e 5465 6e73 6f72 2064 796e 5f73 697a  f.Tensor dyn_siz
+00006bf0: 653a 0a20 2020 2020 2020 2022 2222 0a20  e:.        """. 
+00006c00: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
+00006c10: 796e 5f73 697a 655f 6578 743a 0a20 2020  yn_size_ext:.   
+00006c20: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00006c30: 2e64 796e 5f73 697a 655f 6578 742e 706c  .dyn_size_ext.pl
+00006c40: 6163 6568 6f6c 6465 7220 6973 206e 6f74  aceholder is not
+00006c50: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+00006c60: 2020 2020 2020 2023 2044 6f20 6e6f 7420         # Do not 
+00006c70: 616c 6c6f 7720 7265 7365 7474 696e 6720  allow resetting 
+00006c80: 6974 2074 6f20 7374 6820 6469 6666 6572  it to sth differ
+00006c90: 656e 742e 0a20 2020 2020 2020 2020 2020  ent..           
+00006ca0: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
+00006cb0: 2e64 796e 5f73 697a 655f 6578 742e 706c  .dyn_size_ext.pl
+00006cc0: 6163 6568 6f6c 6465 7220 6973 2064 796e  aceholder is dyn
+00006cd0: 5f73 697a 650a 2020 2020 2020 2020 656c  _size.        el
+00006ce0: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00006cf0: 6265 616d 203d 2067 6574 6174 7472 2864  beam = getattr(d
+00006d00: 796e 5f73 697a 652c 2022 5f52 4554 5552  yn_size, "_RETUR
+00006d10: 4e4e 5f64 796e 5f73 697a 655f 6265 616d  NN_dyn_size_beam
+00006d20: 222c 204e 6f6e 6529 0a20 2020 2020 2020  ", None).       
+00006d30: 2020 2020 2073 656c 662e 6479 6e5f 7369       self.dyn_si
+00006d40: 7a65 5f65 7874 203d 205f 742e 5465 6e73  ze_ext = _t.Tens
+00006d50: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+00006d60: 2020 2020 6e61 6d65 3d28 2225 733a 6479      name=("%s:dy
+00006d70: 6e5f 7369 7a65 2220 2520 7365 6c66 2e64  n_size" % self.d
+00006d80: 6573 6372 6970 7469 6f6e 2920 6966 2073  escription) if s
+00006d90: 656c 662e 6465 7363 7269 7074 696f 6e20  elf.description 
+00006da0: 656c 7365 2064 796e 5f73 697a 652e 6f70  else dyn_size.op
+00006db0: 2e6e 616d 652c 0a20 2020 2020 2020 2020  .name,.         
+00006dc0: 2020 2020 2020 2064 7479 7065 3d5f 742e         dtype=_t.
+00006dd0: 5465 6e73 6f72 2e73 697a 655f 6474 7970  Tensor.size_dtyp
+00006de0: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00006df0: 2020 2073 6861 7065 3d28 292c 0a20 2020     shape=(),.   
+00006e00: 2020 2020 2020 2020 2020 2020 2062 6174               bat
+00006e10: 6368 5f64 696d 5f61 7869 733d 302c 0a20  ch_dim_axis=0,. 
+00006e20: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00006e30: 6174 6368 3d73 656c 662e 6261 7463 682c  atch=self.batch,
+00006e40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00006e50: 2062 6561 6d3d 6265 616d 2c0a 2020 2020   beam=beam,.    
+00006e60: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+00006e70: 726f 6c5f 666c 6f77 5f63 7478 3d73 656c  rol_flow_ctx=sel
+00006e80: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
+00006e90: 7478 2c0a 2020 2020 2020 2020 2020 2020  tx,.            
+00006ea0: 290a 2020 2020 2020 2020 7365 6c66 2e64  ).        self.d
+00006eb0: 796e 5f73 697a 655f 6578 742e 706c 6163  yn_size_ext.plac
+00006ec0: 6568 6f6c 6465 7220 3d20 6479 6e5f 7369  eholder = dyn_si
+00006ed0: 7a65 0a0a 2020 2020 6465 6620 6765 745f  ze..    def get_
+00006ee0: 6d61 736b 2873 656c 663a 2044 696d 2c20  mask(self: Dim, 
+00006ef0: 2a2c 2064 696d 5f6f 7264 6572 3a20 4f70  *, dim_order: Op
+00006f00: 7469 6f6e 616c 5b53 6571 7565 6e63 655b  tional[Sequence[
+00006f10: 4469 6d5d 5d20 3d20 4e6f 6e65 2920 2d3e  Dim]] = None) ->
+00006f20: 205f 742e 5465 6e73 6f72 3a0a 2020 2020   _t.Tensor:.    
+00006f30: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00006f40: 3a70 6172 616d 2064 696d 5f6f 7264 6572  :param dim_order
+00006f50: 3a20 6966 2067 6976 656e 2c20 7468 6520  : if given, the 
+00006f60: 6469 6d73 206f 6620 7468 6520 6d61 736b  dims of the mask
+00006f70: 2077 696c 6c20 6265 2069 6e20 7468 6973   will be in this
+00006f80: 206f 7264 6572 2e0a 2020 2020 2020 2020   order..        
+00006f90: 2020 2020 5468 6973 2063 616e 2062 6520      This can be 
+00006fa0: 7573 6566 756c 2069 6620 7468 6520 6d61  useful if the ma
+00006fb0: 736b 2069 7320 6272 6f61 6463 6173 7465  sk is broadcaste
+00006fc0: 6420 6167 6169 6e73 7420 736f 6d65 206f  d against some o
+00006fd0: 7468 6572 2074 656e 736f 722e 0a20 2020  ther tensor..   
+00006fe0: 2020 2020 203a 7265 7475 726e 3a20 6966       :return: if
+00006ff0: 206e 6565 645f 6d61 736b 696e 6728 292c   need_masking(),
+00007000: 2074 6865 2063 6f72 7265 7370 6f6e 6469   the correspondi
+00007010: 6e67 206d 6173 6b2e 0a20 2020 2020 2020  ng mask..       
+00007020: 2020 2020 2049 6620 7468 6973 2069 7320       If this is 
+00007030: 652e 672e 2074 6865 2074 696d 652d 6469  e.g. the time-di
+00007040: 6d20 5420 6f66 2073 6861 7065 205b 425d  m T of shape [B]
+00007050: 2c20 7468 656e 2074 6865 206d 6173 6b20  , then the mask 
+00007060: 7769 6c6c 2062 6520 6f66 2073 6861 7065  will be of shape
+00007070: 205b 422c 545d 2e0a 2020 2020 2020 2020   [B,T]..        
+00007080: 2020 2020 5468 6520 6d61 736b 2063 6f75      The mask cou
+00007090: 6c64 2062 6520 7573 6564 2077 6974 6820  ld be used with 
+000070a0: 3a66 756e 633a 606d 6173 6b65 645f 7365  :func:`masked_se
+000070b0: 6c65 6374 6020 2860 6062 6f6f 6c65 616e  lect` (``boolean
+000070c0: 5f6d 6173 6b60 6029 206f 7220 6060 7768  _mask``) or ``wh
+000070d0: 6572 6560 602e 0a20 2020 2020 2020 2022  ere``..        "
+000070e0: 2222 0a20 2020 2020 2020 2069 6d70 6f72  "".        impor
+000070f0: 7420 7265 7475 726e 6e2e 6672 6f6e 7465  t returnn.fronte
+00007100: 6e64 2061 7320 7266 0a0a 2020 2020 2020  nd as rf..      
+00007110: 2020 6173 7365 7274 2073 656c 662e 6479    assert self.dy
+00007120: 6e5f 7369 7a65 5f65 7874 2061 6e64 2073  n_size_ext and s
+00007130: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+00007140: 2e72 6177 5f74 656e 736f 7220 6973 206e  .raw_tensor is n
+00007150: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
+00007160: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
+00007170: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
+00007180: 0a20 2020 2020 2020 2062 6163 6b65 6e64  .        backend
+00007190: 203d 2073 656c 662e 6479 6e5f 7369 7a65   = self.dyn_size
+000071a0: 5f65 7874 2e5f 7261 775f 6261 636b 656e  _ext._raw_backen
+000071b0: 640a 0a20 2020 2020 2020 206d 6178 5f69  d..        max_i
+000071c0: 6478 203d 2072 662e 7265 6475 6365 280a  dx = rf.reduce(.
+000071d0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000071e0: 2e64 796e 5f73 697a 655f 6578 742c 0a20  .dyn_size_ext,. 
+000071f0: 2020 2020 2020 2020 2020 2061 7869 733d             axis=
+00007200: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+00007210: 742e 6469 6d73 2c0a 2020 2020 2020 2020  t.dims,.        
+00007220: 2020 2020 6d6f 6465 3d22 6d61 7822 2c0a      mode="max",.
+00007230: 2020 2020 2020 2020 2020 2020 2320 4d61              # Ma
+00007240: 736b 696e 6720 6865 7265 2069 7320 6e6f  sking here is no
+00007250: 7420 616c 7761 7973 2070 6f73 7369 626c  t always possibl
+00007260: 652c 2065 2e67 2e20 6966 2077 6520 6861  e, e.g. if we ha
+00007270: 7665 0a20 2020 2020 2020 2020 2020 2023  ve.            #
+00007280: 2074 6167 203d 2044 696d 7b27 7365 6c66   tag = Dim{'self
+00007290: 2d61 7474 2d6b 6579 7327 5b27 7469 6d65  -att-keys'['time
+000072a0: 3a76 6172 3a65 7874 6572 6e5f 6461 7461  :var:extern_data
+000072b0: 3a63 6c61 7373 6573 275b 425d 5d7d 0a20  :classes'[B]]}. 
+000072c0: 2020 2020 2020 2020 2020 2075 7365 5f6d             use_m
+000072d0: 6173 6b3d 4661 6c73 652c 0a20 2020 2020  ask=False,.     
+000072e0: 2020 2029 0a20 2020 2020 2020 2023 2057     ).        # W
+000072f0: 6520 7573 6520 7468 6520 6173 7375 6d70  e use the assump
+00007300: 7469 6f6e 2074 6861 7420 7365 6c66 2e70  tion that self.p
+00007310: 6c61 6365 686f 6c64 6572 2e73 6861 7065  laceholder.shape
+00007320: 5b61 7869 735d 203d 3d20 6d61 785f 6964  [axis] == max_id
+00007330: 782e 0a20 2020 2020 2020 2023 2073 697a  x..        # siz
+00007340: 655f 6578 7420 6d69 6768 7420 6861 7665  e_ext might have
+00007350: 2069 6e76 616c 6964 2028 7a65 726f 2920   invalid (zero) 
+00007360: 7369 7a65 730a 2020 2020 2020 2020 2320  sizes.        # 
+00007370: 7768 656e 2069 7420 6974 7365 6c66 2068  when it itself h
+00007380: 6173 2073 6f6d 6520 7061 6464 696e 672c  as some padding,
+00007390: 2065 2e67 2e20 7768 656e 2069 7473 206f   e.g. when its o
+000073a0: 776e 2073 6861 7065 2069 7320 6479 6e61  wn shape is dyna
+000073b0: 6d69 632e 0a20 2020 2020 2020 2023 2041  mic..        # A
+000073c0: 207a 6572 6f20 7369 7a65 2063 616e 206c   zero size can l
+000073d0: 6561 6420 746f 2070 726f 626c 656d 7320  ead to problems 
+000073e0: 696e 2073 6f6d 6520 6361 7365 732c 2065  in some cases, e
+000073f0: 2e67 2e20 696e 2053 6f66 746d 6178 4f76  .g. in SoftmaxOv
+00007400: 6572 5370 6174 6961 6c4c 6179 6572 2c0a  erSpatialLayer,.
+00007410: 2020 2020 2020 2020 2320 7768 656e 2065          # when e
+00007420: 7665 7279 7468 696e 6720 6973 206d 6173  verything is mas
+00007430: 6b65 6420 746f 202d 696e 662c 2069 7420  ked to -inf, it 
+00007440: 7265 7375 6c74 7320 696e 206e 616e 2c0a  results in nan,.
+00007450: 2020 2020 2020 2020 2320 616e 6420 7468          # and th
+00007460: 6973 206c 696b 656c 7920 7072 6f64 7563  is likely produc
+00007470: 6573 206e 616e 2069 6e20 6261 636b 7072  es nan in backpr
+00007480: 6f70 206f 7220 656c 7365 7768 6572 652e  op or elsewhere.
+00007490: 0a20 2020 2020 2020 2023 2054 6875 732c  .        # Thus,
+000074a0: 206d 6173 6b20 7369 7a65 5f65 7874 2069   mask size_ext i
+000074b0: 7473 656c 662c 2061 6e64 2073 6574 2074  tself, and set t
+000074c0: 6865 2070 6164 6465 6420 7661 6c75 6573  he padded values
+000074d0: 2074 6f20 312e 0a20 2020 2020 2020 2023   to 1..        #
+000074e0: 2054 6869 7320 6173 7375 6d65 7320 7468   This assumes th
+000074f0: 6174 206d 6178 5f69 6478 203e 3d20 312e  at max_idx >= 1.
+00007500: 0a20 2020 2020 2020 2073 697a 655f 6578  .        size_ex
+00007510: 7420 3d20 7365 6c66 2e64 796e 5f73 697a  t = self.dyn_siz
+00007520: 655f 6578 742e 636f 7079 5f6d 6173 6b65  e_ext.copy_maske
+00007530: 6428 6d61 785f 6964 7829 0a20 2020 2020  d(max_idx).     
+00007540: 2020 2069 6478 5f72 616e 6765 203d 2062     idx_range = b
+00007550: 6163 6b65 6e64 2e72 616e 6765 5f6f 7665  ackend.range_ove
+00007560: 725f 6469 6d28 7365 6c66 290a 2020 2020  r_dim(self).    
+00007570: 2020 2020 7365 715f 6d61 736b 203d 2072      seq_mask = r
+00007580: 662e 636f 6d70 6172 6528 6964 785f 7261  f.compare(idx_ra
+00007590: 6e67 652c 2022 3c22 2c20 7369 7a65 5f65  nge, "<", size_e
+000075a0: 7874 2c20 616c 6c6f 775f 6272 6f61 6463  xt, allow_broadc
+000075b0: 6173 745f 616c 6c5f 736f 7572 6365 733d  ast_all_sources=
+000075c0: 5472 7565 2c20 6469 6d5f 6f72 6465 723d  True, dim_order=
+000075d0: 6469 6d5f 6f72 6465 7229 0a20 2020 2020  dim_order).     
+000075e0: 2020 2072 6574 7572 6e20 7365 715f 6d61     return seq_ma
+000075f0: 736b 0a0a 2020 2020 6465 6620 6973 5f62  sk..    def is_b
+00007600: 6174 6368 5f64 696d 2873 656c 6629 3a0a  atch_dim(self):.
+00007610: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00007620: 2020 2020 3a72 6574 7572 6e3a 2077 6865      :return: whe
+00007630: 7468 6572 2074 6869 7320 6469 6d20 7461  ther this dim ta
+00007640: 6720 6973 206f 6620 6b69 6e64 2062 6174  g is of kind bat
+00007650: 6368 0a20 2020 2020 2020 203a 7274 7970  ch.        :rtyp
+00007660: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+00007670: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00007680: 726e 2073 656c 662e 6b69 6e64 203d 3d20  rn self.kind == 
+00007690: 4469 6d54 7970 6573 2e42 6174 6368 0a0a  DimTypes.Batch..
+000076a0: 2020 2020 6465 6620 6973 5f66 6561 7475      def is_featu
+000076b0: 7265 5f64 696d 2873 656c 6629 3a0a 2020  re_dim(self):.  
+000076c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000076d0: 2020 3a72 6574 7572 6e3a 2077 6865 7468    :return: wheth
+000076e0: 6572 2074 6869 7320 6469 6d20 7461 6720  er this dim tag 
+000076f0: 6973 206f 6620 6b69 6e64 2066 6561 7475  is of kind featu
+00007700: 7265 0a20 2020 2020 2020 203a 7274 7970  re.        :rtyp
+00007710: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+00007720: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+00007730: 726e 2073 656c 662e 6b69 6e64 203d 3d20  rn self.kind == 
+00007740: 4469 6d54 7970 6573 2e46 6561 7475 7265  DimTypes.Feature
+00007750: 0a0a 2020 2020 6465 6620 6973 5f73 7061  ..    def is_spa
+00007760: 7469 616c 5f64 696d 2873 656c 6629 3a0a  tial_dim(self):.
+00007770: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00007780: 2020 2020 3a72 6574 7572 6e3a 2077 6865      :return: whe
+00007790: 7468 6572 2074 6869 7320 6469 6d20 7461  ther this dim ta
+000077a0: 6720 6973 206f 6620 6b69 6e64 2073 7061  g is of kind spa
+000077b0: 7469 616c 0a20 2020 2020 2020 203a 7274  tial.        :rt
+000077c0: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+000077d0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+000077e0: 7475 726e 2073 656c 662e 6b69 6e64 203d  turn self.kind =
+000077f0: 3d20 4469 6d54 7970 6573 2e53 7061 7469  = DimTypes.Spati
+00007800: 616c 0a0a 2020 2020 6465 6620 6973 5f64  al..    def is_d
+00007810: 696d 5f6b 6e6f 776e 2873 656c 6629 3a0a  im_known(self):.
+00007820: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00007830: 2020 2020 3a72 6574 7572 6e3a 2077 6865      :return: whe
+00007840: 7468 6572 2077 6520 6b6e 6f77 2074 6865  ther we know the
+00007850: 2064 696d 656e 7369 6f6e 3b20 6261 7369   dimension; basi
+00007860: 6361 6c6c 7920 7768 6574 6865 7220 7468  cally whether th
+00007870: 6973 2069 7320 6465 6669 6e65 640a 2020  is is defined.  
+00007880: 2020 2020 2020 2020 2861 6c74 686f 7567          (althoug
+00007890: 6820 606e 6f74 2073 656c 662e 756e 6465  h `not self.unde
+000078a0: 6669 6e65 6460 2069 7320 6465 6669 6e65  fined` is define
+000078b0: 6420 736c 6967 6874 6c79 2064 6966 6665  d slightly diffe
+000078c0: 7265 6e74 6c79 290a 2020 2020 2020 2020  rently).        
+000078d0: 3a72 7479 7065 3a20 626f 6f6c 0a20 2020  :rtype: bool.   
+000078e0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000078f0: 2069 6620 7365 6c66 2e69 735f 6261 7463   if self.is_batc
+00007900: 685f 6469 6d28 293a 0a20 2020 2020 2020  h_dim():.       
+00007910: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00007920: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+00007930: 7365 6c66 2e69 735f 6479 6e61 6d69 6328  self.is_dynamic(
+00007940: 2920 616e 6420 7365 6c66 2e64 696d 656e  ) and self.dimen
+00007950: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
+00007960: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00007970: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+00007980: 2020 6966 2073 656c 662e 6479 6e5f 7369    if self.dyn_si
+00007990: 7a65 5f65 7874 3a0a 2020 2020 2020 2020  ze_ext:.        
+000079a0: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+000079b0: 2020 2020 2020 2020 6578 7472 6120 3d20          extra = 
+000079c0: 7365 6c66 2e5f 6765 745f 7361 6d65 5f62  self._get_same_b
+000079d0: 6173 655f 6578 7472 6128 290a 2020 2020  ase_extra().    
+000079e0: 2020 2020 6966 2065 7874 7261 3a0a 2020      if extra:.  
+000079f0: 2020 2020 2020 2020 2020 666f 7220 5f2c            for _,
+00007a00: 206f 7468 6572 2069 6e20 6578 7472 612e   other in extra.
+00007a10: 7361 6d65 5f66 6f72 5f62 6174 6368 5f63  same_for_batch_c
+00007a20: 7478 2e69 7465 6d73 2829 3a0a 2020 2020  tx.items():.    
+00007a30: 2020 2020 2020 2020 2020 2020 6966 206f              if o
+00007a40: 7468 6572 2e64 796e 5f73 697a 655f 6578  ther.dyn_size_ex
+00007a50: 743a 0a20 2020 2020 2020 2020 2020 2020  t:.             
+00007a60: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
+00007a70: 7565 0a20 2020 2020 2020 2072 6574 7572  ue.        retur
+00007a80: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
+00007a90: 2069 735f 6479 6e61 6d69 6328 7365 6c66   is_dynamic(self
+00007aa0: 2920 2d3e 2062 6f6f 6c3a 0a20 2020 2020  ) -> bool:.     
+00007ab0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00007ac0: 7265 7475 726e 3a20 7768 6574 6865 7220  return: whether 
+00007ad0: 7468 6520 6469 6d20 6973 206e 6f74 2073  the dim is not s
+00007ae0: 7461 7469 632e 2075 7375 616c 6c79 206d  tatic. usually m
+00007af0: 6561 6e73 2074 6861 7420 6974 2068 6173  eans that it has
+00007b00: 2073 6571 206c 656e 6774 6873 0a20 2020   seq lengths.   
+00007b10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00007b20: 2072 6574 7572 6e20 7365 6c66 2e64 696d   return self.dim
+00007b30: 656e 7369 6f6e 2069 7320 4e6f 6e65 2061  ension is None a
+00007b40: 6e64 206e 6f74 2073 656c 662e 6973 5f62  nd not self.is_b
+00007b50: 6174 6368 5f64 696d 2829 0a0a 2020 2020  atch_dim()..    
+00007b60: 6465 6620 6973 5f73 7461 7469 6328 7365  def is_static(se
+00007b70: 6c66 2920 2d3e 2062 6f6f 6c3a 0a20 2020  lf) -> bool:.   
+00007b80: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00007b90: 203a 7265 7475 726e 3a20 7374 6174 6963   :return: static
+00007ba0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00007bb0: 2020 2020 2072 6574 7572 6e20 6e6f 7420       return not 
+00007bc0: 7365 6c66 2e69 735f 6479 6e61 6d69 6328  self.is_dynamic(
+00007bd0: 290a 0a20 2020 2064 6566 206e 6565 645f  )..    def need_
+00007be0: 6d61 736b 696e 6728 7365 6c66 293a 0a20  masking(self):. 
+00007bf0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00007c00: 2020 203a 7265 7475 726e 3a20 7768 6574     :return: whet
+00007c10: 6865 7220 6469 6d20 6973 2073 7461 7469  her dim is stati
+00007c20: 6320 6f72 2064 796e 616d 6963 2062 7574  c or dynamic but
+00007c30: 2077 6974 6820 7363 616c 6172 2064 796e   with scalar dyn
+00007c40: 5f73 697a 655f 6578 740a 2020 2020 2020  _size_ext.      
+00007c50: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00007c60: 2073 656c 662e 6973 5f73 7461 7469 6328   self.is_static(
+00007c70: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00007c80: 6620 7365 6c66 2e63 6170 6163 6974 7920  f self.capacity 
+00007c90: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00007ca0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+00007cb0: 7572 6e20 7365 6c66 2e73 697a 6520 3c20  urn self.size < 
+00007cc0: 7365 6c66 2e63 6170 6163 6974 790a 2020  self.capacity.  
+00007cd0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00007ce0: 2046 616c 7365 0a20 2020 2020 2020 2069   False.        i
+00007cf0: 6620 7365 6c66 2e63 6170 6163 6974 7920  f self.capacity 
+00007d00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00007d10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00007d20: 5472 7565 0a20 2020 2020 2020 2069 6620  True.        if 
+00007d30: 6e6f 7420 7365 6c66 2e64 796e 5f73 697a  not self.dyn_siz
+00007d40: 655f 6578 743a 0a20 2020 2020 2020 2020  e_ext:.         
+00007d50: 2020 2072 6574 7572 6e20 5472 7565 2020     return True  
+00007d60: 2320 756e 6b6e 6f77 6e0a 2020 2020 2020  # unknown.      
+00007d70: 2020 7265 7475 726e 2073 656c 662e 6479    return self.dy
+00007d80: 6e5f 7369 7a65 5f65 7874 2e62 6174 6368  n_size_ext.batch
+00007d90: 5f6e 6469 6d20 3e20 300a 0a20 2020 2064  _ndim > 0..    d
+00007da0: 6566 2063 616e 5f62 655f 7573 6564 5f61  ef can_be_used_a
+00007db0: 735f 6469 6d28 7365 6c66 293a 0a20 2020  s_dim(self):.   
+00007dc0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00007dd0: 203a 7265 7475 726e 3a20 7768 6574 6865   :return: whethe
+00007de0: 7220 7468 6973 2063 616e 2062 6520 7573  r this can be us
+00007df0: 6564 2061 7320 6120 6469 6d20 696e 203a  ed as a dim in :
+00007e00: 636c 6173 733a 6044 6174 6160 2c20 692e  class:`Data`, i.
+00007e10: 652e 2069 7420 6973 206e 6f74 2073 7065  e. it is not spe
+00007e20: 6369 616c 0a20 2020 2020 2020 203a 7274  cial.        :rt
+00007e30: 7970 653a 2062 6f6f 6c0a 2020 2020 2020  ype: bool.      
+00007e40: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00007e50: 7475 726e 206e 6f74 2073 656c 662e 7370  turn not self.sp
+00007e60: 6563 6961 6c0a 0a20 2020 2064 6566 2069  ecial..    def i
+00007e70: 735f 7361 6d65 5f73 697a 655f 7465 6e73  s_same_size_tens
+00007e80: 6f72 2873 656c 662c 2078 293a 0a20 2020  or(self, x):.   
+00007e90: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00007ea0: 203a 7061 7261 6d20 7466 2e54 656e 736f   :param tf.Tenso
+00007eb0: 7220 783a 0a20 2020 2020 2020 203a 7265  r x:.        :re
+00007ec0: 7475 726e 3a20 7768 6574 6865 7220 7468  turn: whether th
+00007ed0: 6973 2064 696d 2074 6167 2066 6f72 2074  is dim tag for t
+00007ee0: 6869 7320 7370 6563 6966 6963 2062 6174  his specific bat
+00007ef0: 6368 2028 696e 636c 2062 6561 6d29 2069  ch (incl beam) i
+00007f00: 7320 7468 6520 7361 6d65 2061 7320 7468  s the same as th
+00007f10: 6520 6769 7665 6e20 7369 7a65 0a20 2020  e given size.   
+00007f20: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
+00007f30: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
+00007f40: 2020 2020 2020 6966 2073 656c 662e 6479        if self.dy
+00007f50: 6e5f 7369 7a65 5f65 7874 2061 6e64 2078  n_size_ext and x
+00007f60: 2069 7320 7365 6c66 2e64 796e 5f73 697a   is self.dyn_siz
+00007f70: 655f 6578 742e 706c 6163 6568 6f6c 6465  e_ext.placeholde
+00007f80: 723a 0a20 2020 2020 2020 2020 2020 2072  r:.            r
+00007f90: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
+00007fa0: 2020 2074 6167 203d 205f 4469 6d4d 6978     tag = _DimMix
+00007fb0: 696e 2e67 6574 5f74 6167 5f66 726f 6d5f  in.get_tag_from_
+00007fc0: 7369 7a65 5f74 656e 736f 7228 7829 0a20  size_tensor(x). 
+00007fd0: 2020 2020 2020 2069 6620 7461 6720 616e         if tag an
+00007fe0: 6420 7461 6720 3d3d 2073 656c 663a 0a20  d tag == self:. 
+00007ff0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00008000: 6e20 5472 7565 0a20 2020 2020 2020 2069  n True.        i
+00008010: 6620 6e6f 7420 7365 6c66 2e5f 6578 7472  f not self._extr
+00008020: 613a 0a20 2020 2020 2020 2020 2020 2072  a:.            r
+00008030: 6574 7572 6e20 4661 6c73 650a 2020 2020  eturn False.    
+00008040: 2020 2020 6966 2075 7469 6c2e 5265 6649      if util.RefI
+00008050: 6445 7128 7829 2069 6e20 7365 6c66 2e5f  dEq(x) in self._
+00008060: 6578 7472 612e 6479 6e5f 7369 7a65 5f73  extra.dyn_size_s
+00008070: 616d 653a 0a20 2020 2020 2020 2020 2020  ame:.           
+00008080: 2072 6574 7572 6e20 5472 7565 0a20 2020   return True.   
+00008090: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
+000080a0: 650a 0a20 2020 2064 6566 2073 6574 5f74  e..    def set_t
+000080b0: 6167 5f6f 6e5f 7369 7a65 5f74 656e 736f  ag_on_size_tenso
+000080c0: 7228 7365 6c66 3a20 4469 6d2c 2078 2c20  r(self: Dim, x, 
+000080d0: 6261 7463 683d 4e6f 6e65 2c20 7361 6d65  batch=None, same
+000080e0: 5f61 735f 6265 666f 7265 3d46 616c 7365  _as_before=False
+000080f0: 2920 2d3e 2044 696d 3a0a 2020 2020 2020  ) -> Dim:.      
+00008100: 2020 2222 220a 2020 2020 2020 2020 5468    """.        Th
+00008110: 6973 2066 756e 6374 696f 6e20 6973 2075  is function is u
+00008120: 7365 640a 2020 2020 2020 2020 746f 2063  sed.        to c
+00008130: 6f75 706c 6520 6120 7466 2e54 656e 736f  ouple a tf.Tenso
+00008140: 7220 696e 7374 616e 6365 2072 6570 7265  r instance repre
+00008150: 7365 6e74 696e 6720 7468 6520 6479 6e20  senting the dyn 
+00008160: 7369 7a65 0a20 2020 2020 2020 2077 6974  size.        wit
+00008170: 6820 7468 6520 6469 6d20 7461 672e 0a0a  h the dim tag...
+00008180: 2020 2020 2020 2020 5468 6973 2069 7320          This is 
+00008190: 7573 7561 6c6c 7920 6120 6e65 776c 7920  usually a newly 
+000081a0: 6372 6561 7465 6420 6469 6d20 7461 672c  created dim tag,
+000081b0: 0a20 2020 2020 2020 2077 6869 6368 2069  .        which i
+000081c0: 7320 7965 7420 756e 7365 742e 0a0a 2020  s yet unset...  
+000081d0: 2020 2020 2020 4974 2069 7320 616c 736f        It is also
+000081e0: 2075 7365 6420 746f 2063 6f75 706c 6520   used to couple 
+000081f0: 616e 2065 7869 7374 696e 6720 6469 6d20  an existing dim 
+00008200: 7461 6720 7769 7468 206f 7468 6572 2064  tag with other d
+00008210: 796e 2073 697a 6573 0a20 2020 2020 2020  yn sizes.       
+00008220: 2077 6869 6368 206a 7573 7420 6469 6666   which just diff
+00008230: 6572 2062 7920 616e 2065 7870 616e 7369  er by an expansi
+00008240: 6f6e 206f 6620 7468 6520 6261 7463 6820  on of the batch 
+00008250: 2865 2e67 2e20 7365 6172 6368 2062 6561  (e.g. search bea
+00008260: 6d29 2e0a 0a20 2020 2020 2020 2053 6565  m)...        See
+00008270: 2061 6c73 6f20 3a66 756e 633a 6067 6574   also :func:`get
+00008280: 5f74 6167 5f66 726f 6d5f 7369 7a65 5f74  _tag_from_size_t
+00008290: 656e 736f 7260 2e0a 2020 2020 2020 2020  ensor`..        
+000082a0: 416c 736f 2073 6565 203a 6675 6e63 3a60  Also see :func:`
+000082b0: 7365 745f 6479 6e5f 7369 7a65 5f65 7874  set_dyn_size_ext
+000082c0: 5f66 6f72 5f62 6174 6368 5f63 7478 602e  _for_batch_ctx`.
+000082d0: 0a0a 2020 2020 2020 2020 3a70 6172 616d  ..        :param
+000082e0: 2078 3a20 7261 7720 7465 6e73 6f72 2c20   x: raw tensor, 
+000082f0: 666f 7220 6578 616d 706c 6520 7466 2e54  for example tf.T
+00008300: 656e 736f 720a 2020 2020 2020 2020 3a70  ensor.        :p
+00008310: 6172 616d 2042 6174 6368 496e 666f 7c4e  aram BatchInfo|N
+00008320: 6f6e 6520 6261 7463 683a 0a20 2020 2020  one batch:.     
+00008330: 2020 203a 7061 7261 6d20 626f 6f6c 2073     :param bool s
+00008340: 616d 655f 6173 5f62 6566 6f72 653a 2069  ame_as_before: i
+00008350: 6d70 6c69 6573 2069 7420 7761 7320 7365  mplies it was se
+00008360: 7420 6265 666f 7265 2c20 616e 6420 7468  t before, and th
+00008370: 6520 6e65 7720 7369 7a65 2069 7320 7468  e new size is th
+00008380: 6520 7361 6d65 2e0a 2020 2020 2020 2020  e same..        
+00008390: 2020 652e 672e 2069 7420 636f 756c 6420    e.g. it could 
+000083a0: 6265 2073 6f6d 6520 6964 656e 7469 7479  be some identity
+000083b0: 2077 6974 6820 6164 6465 6420 6368 6563   with added chec
+000083c0: 6b73 2c20 6f72 206f 7468 6572 2063 6861  ks, or other cha
+000083d0: 6e67 652e 0a20 2020 2020 2020 203a 7265  nge..        :re
+000083e0: 7475 726e 3a20 7365 6c66 206f 7220 6e65  turn: self or ne
+000083f0: 7720 6469 6d20 7461 670a 2020 2020 2020  w dim tag.      
+00008400: 2020 2222 220a 2020 2020 2020 2020 6173    """.        as
+00008410: 7365 7274 2073 656c 662e 6361 6e5f 6265  sert self.can_be
+00008420: 5f75 7365 645f 6173 5f64 696d 2829 0a20  _used_as_dim(). 
+00008430: 2020 2020 2020 2023 2049 7427 7320 756e         # It's un
+00008440: 7573 7561 6c20 6966 2073 656c 662e 6469  usual if self.di
+00008450: 6d65 6e73 696f 6e20 6973 206e 6f74 204e  mension is not N
+00008460: 6f6e 652c 2062 7574 206c 6574 2773 2061  one, but let's a
+00008470: 6363 6570 7420 7468 6174 2e0a 2020 2020  ccept that..    
+00008480: 2020 2020 6966 2068 6173 6174 7472 2878      if hasattr(x
+00008490: 2c20 225f 6973 5f73 697a 655f 6f66 5f64  , "_is_size_of_d
+000084a0: 696d 5f74 6167 2229 3a0a 2020 2020 2020  im_tag"):.      
+000084b0: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
+000084c0: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
+000084d0: 4d65 6d62 6572 0a20 2020 2020 2020 2020  Member.         
+000084e0: 2020 2061 7373 6572 7420 782e 5f69 735f     assert x._is_
+000084f0: 7369 7a65 5f6f 665f 6469 6d5f 7461 6720  size_of_dim_tag 
+00008500: 696e 2028 4e6f 6e65 2c20 7365 6c66 290a  in (None, self).
+00008510: 2020 2020 2020 2020 2320 4966 2077 6520          # If we 
+00008520: 616c 7265 6164 7920 6861 7665 2061 6e6f  already have ano
+00008530: 7468 6572 2064 796e 2073 697a 6520 7365  ther dyn size se
+00008540: 7420 6f72 2064 6966 6665 7265 6e74 2062  t or different b
+00008550: 6174 6368 2c20 6372 6561 7465 2061 206e  atch, create a n
+00008560: 6577 2044 696d 2069 6e73 7461 6e63 652e  ew Dim instance.
+00008570: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00008580: 2e62 6174 6368 2061 6e64 2062 6174 6368  .batch and batch
+00008590: 2061 6e64 2073 656c 662e 6261 7463 6820   and self.batch 
+000085a0: 213d 2062 6174 6368 3a0a 2020 2020 2020  != batch:.      
+000085b0: 2020 2020 2020 6173 7365 7274 206e 6f74        assert not
+000085c0: 2073 616d 655f 6173 5f62 6566 6f72 6520   same_as_before 
+000085d0: 2023 2069 7420 6361 6e6e 6f74 2062 6520   # it cannot be 
+000085e0: 7468 6520 7361 6d65 2077 6865 6e20 6974  the same when it
+000085f0: 2069 7320 616e 6f74 6865 7220 6261 7463   is another batc
+00008600: 682e 2e2e 0a20 2020 2020 2020 2020 2020  h....           
+00008610: 206e 6577 5f64 696d 5f74 6167 203d 2073   new_dim_tag = s
+00008620: 656c 662e 6765 745f 666f 725f 6261 7463  elf.get_for_batc
+00008630: 685f 6374 7828 6261 7463 683d 6261 7463  h_ctx(batch=batc
+00008640: 682c 2063 7478 3d73 656c 662e 636f 6e74  h, ctx=self.cont
+00008650: 726f 6c5f 666c 6f77 5f63 7478 290a 2020  rol_flow_ctx).  
+00008660: 2020 2020 2020 2020 2020 6e65 775f 6469            new_di
+00008670: 6d5f 7461 672e 7365 745f 7461 675f 6f6e  m_tag.set_tag_on
+00008680: 5f73 697a 655f 7465 6e73 6f72 2878 2c20  _size_tensor(x, 
+00008690: 6261 7463 683d 6261 7463 6829 0a20 2020  batch=batch).   
+000086a0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000086b0: 6e65 775f 6469 6d5f 7461 670a 2020 2020  new_dim_tag.    
+000086c0: 2020 2020 6966 2073 656c 662e 6479 6e5f      if self.dyn_
+000086d0: 7369 7a65 2069 7320 6e6f 7420 4e6f 6e65  size is not None
+000086e0: 2061 6e64 2073 656c 662e 6479 6e5f 7369   and self.dyn_si
+000086f0: 7a65 2069 7320 6e6f 7420 783a 0a20 2020  ze is not x:.   
+00008700: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+00008710: 2e5f 6578 7472 6120 616e 6420 7574 696c  ._extra and util
+00008720: 2e52 6566 4964 4571 2878 2920 696e 2073  .RefIdEq(x) in s
+00008730: 656c 662e 5f65 7874 7261 2e64 796e 5f73  elf._extra.dyn_s
+00008740: 697a 655f 7361 6d65 3a0a 2020 2020 2020  ize_same:.      
+00008750: 2020 2020 2020 2020 2020 7061 7373 2020            pass  
+00008760: 2320 6f6b 2c20 7061 7373 206f 6e0a 2020  # ok, pass on.  
+00008770: 2020 2020 2020 2020 2020 656c 6966 2073            elif s
+00008780: 616d 655f 6173 5f62 6566 6f72 653a 0a20  ame_as_before:. 
+00008790: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+000087a0: 656c 662e 5f6d 616b 655f 6578 7472 6128  elf._make_extra(
+000087b0: 292e 6479 6e5f 7369 7a65 5f73 616d 652e  ).dyn_size_same.
+000087c0: 6164 6428 7574 696c 2e52 6566 4964 4571  add(util.RefIdEq
+000087d0: 2878 2929 0a20 2020 2020 2020 2020 2020  (x)).           
+000087e0: 2020 2020 2023 2041 6e64 206e 6f77 2070       # And now p
+000087f0: 6173 7320 6f6e 2e0a 2020 2020 2020 2020  ass on..        
+00008800: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+00008810: 2020 2020 2020 2020 2020 6173 7365 7274            assert
+00008820: 2073 656c 662e 6261 7463 6820 616e 6420   self.batch and 
+00008830: 6261 7463 680a 2020 2020 2020 2020 2020  batch.          
+00008840: 2020 2020 2020 2320 4974 2773 206e 6f74        # It's not
+00008850: 2063 6c65 6172 2077 6861 7420 746f 2064   clear what to d
+00008860: 6f2e 2057 6520 636f 756c 6420 6372 6561  o. We could crea
+00008870: 7465 2061 206e 6577 2064 696d 2074 6167  te a new dim tag
+00008880: 2c20 6275 7420 7468 6520 7369 7a65 7320  , but the sizes 
+00008890: 6d69 6768 7420 6265 2064 6966 6665 7265  might be differe
+000088a0: 6e74 2e0a 2020 2020 2020 2020 2020 2020  nt..            
+000088b0: 2020 2020 2320 5573 7561 6c6c 7920 7765      # Usually we
+000088c0: 2073 686f 756c 6420 6e6f 7420 6765 7420   should not get 
+000088d0: 6865 7265 2e0a 2020 2020 2020 2020 2020  here..          
+000088e0: 2020 2020 2020 2320 536f 2066 6f72 206e        # So for n
+000088f0: 6f77 2c20 6a75 7374 2065 7272 6f72 2e0a  ow, just error..
+00008900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008910: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
+00008920: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
+00008930: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008940: 2066 726f 6d20 7265 7475 726e 6e2e 6672   from returnn.fr
+00008950: 6f6e 7465 6e64 2e5f 6261 636b 656e 6420  ontend._backend 
+00008960: 696d 706f 7274 2067 6574 5f62 6163 6b65  import get_backe
+00008970: 6e64 5f62 795f 7261 775f 7465 6e73 6f72  nd_by_raw_tensor
+00008980: 5f74 7970 650a 0a20 2020 2020 2020 2020  _type..         
+00008990: 2020 2020 2020 2072 6169 7365 2045 7863         raise Exc
+000089a0: 6570 7469 6f6e 280a 2020 2020 2020 2020  eption(.        
+000089b0: 2020 2020 2020 2020 2020 2020 225c 6e22              "\n"
+000089c0: 2e6a 6f69 6e28 0a20 2020 2020 2020 2020  .join(.         
+000089d0: 2020 2020 2020 2020 2020 2020 2020 205b                 [
+000089e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000089f0: 2020 2020 2020 2020 2020 2020 2028 0a20               (. 
+00008a00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a10: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00008a20: 2572 2028 2572 2920 616c 7265 6164 7920  %r (%r) already 
+00008a30: 6861 7320 7369 7a65 2025 722c 220a 2020  has size %r,".  
+00008a40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008a50: 2020 2020 2020 2020 2020 2020 2020 2220                " 
+00008a60: 616e 6420 616e 6f74 6865 7220 696e 636f  and another inco
+00008a70: 6d70 6174 6962 6c65 2073 697a 6520 2572  mpatible size %r
+00008a80: 2028 6261 7463 6820 2572 2920 6973 2062   (batch %r) is b
+00008a90: 6569 6e67 2061 7373 6967 6e65 642e 220a  eing assigned.".
+00008aa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ab0: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00008ac0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008ad0: 2020 2020 2020 2020 2020 2520 2873 656c            % (sel
+00008ae0: 662c 2073 656c 662e 6465 7363 7269 7074  f, self.descript
+00008af0: 696f 6e2c 2073 656c 662e 6479 6e5f 7369  ion, self.dyn_si
+00008b00: 7a65 2c20 782c 2062 6174 6368 292c 0a20  ze, x, batch),. 
+00008b10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b20: 2020 2020 2020 2020 2020 2022 5c6e 4e65             "\nNe
+00008b30: 7720 7369 7a65 2063 6f6d 7075 7461 7469  w size computati
+00008b40: 6f6e 2067 7261 7068 3a22 2c0a 2020 2020  on graph:",.    
+00008b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008b60: 2020 2020 2020 2020 6765 745f 6261 636b          get_back
+00008b70: 656e 645f 6279 5f72 6177 5f74 656e 736f  end_by_raw_tenso
+00008b80: 725f 7479 7065 2874 7970 6528 7829 292e  r_type(type(x)).
+00008b90: 666f 726d 6174 5f67 7261 7068 5f6f 7574  format_graph_out
+00008ba0: 7075 7428 782c 206d 6178 5f64 6570 7468  put(x, max_depth
+00008bb0: 3d33 292c 0a20 2020 2020 2020 2020 2020  =3),.           
+00008bc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008bd0: 2022 5c6e 5468 6973 2069 7320 6d61 7962   "\nThis is mayb
+00008be0: 6520 7468 6520 7265 7375 6c74 206f 6620  e the result of 
+00008bf0: 616e 2069 6e63 6f72 7265 6374 2064 6563  an incorrect dec
+00008c00: 6c61 7265 5f73 616d 655f 6173 2e20 222c  lare_same_as. ",
+00008c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00008c20: 2020 2020 2020 2020 2020 2020 2022 7361               "sa
+00008c30: 6d65 5f61 7320 3d20 2573 2220 2520 7365  me_as = %s" % se
+00008c40: 6c66 2e73 616d 655f 6173 2c0a 2020 2020  lf.same_as,.    
+00008c50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00008c60: 2020 2020 5d0a 2020 2020 2020 2020 2020      ].          
+00008c70: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00008c80: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
+00008c90: 2020 2020 2020 6966 2062 6174 6368 2061        if batch a
+00008ca0: 6e64 2067 6574 6174 7472 2878 2c20 225f  nd getattr(x, "_
+00008cb0: 5245 5455 524e 4e5f 6479 6e5f 7369 7a65  RETURNN_dyn_size
+00008cc0: 5f62 6561 6d22 2c20 4e6f 6e65 293a 0a20  _beam", None):. 
+00008cd0: 2020 2020 2020 2020 2020 2061 7373 6572             asser
+00008ce0: 7420 6261 7463 682e 6265 616d 203d 3d20  t batch.beam == 
+00008cf0: 6765 7461 7474 7228 0a20 2020 2020 2020  getattr(.       
+00008d00: 2020 2020 2020 2020 2078 2c20 225f 5245           x, "_RE
+00008d10: 5455 524e 4e5f 6479 6e5f 7369 7a65 5f62  TURNN_dyn_size_b
+00008d20: 6561 6d22 0a20 2020 2020 2020 2020 2020  eam".           
+00008d30: 2029 2c20 2225 733a 2064 796e 2073 697a   ), "%s: dyn siz
+00008d40: 6520 2573 2068 6173 2075 6e65 7870 6563  e %s has unexpec
+00008d50: 7465 6420 6261 7463 6820 2573 2c20 6578  ted batch %s, ex
+00008d60: 7065 6374 6564 2025 7322 2025 2028 0a20  pected %s" % (. 
+00008d70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00008d80: 656c 662c 0a20 2020 2020 2020 2020 2020  elf,.           
+00008d90: 2020 2020 2078 2c0a 2020 2020 2020 2020       x,.        
+00008da0: 2020 2020 2020 2020 6261 7463 682c 0a20          batch,. 
+00008db0: 2020 2020 2020 2020 2020 2020 2020 2067                 g
+00008dc0: 6574 6174 7472 2878 2c20 225f 5245 5455  etattr(x, "_RETU
+00008dd0: 524e 4e5f 6479 6e5f 7369 7a65 5f62 6561  RNN_dyn_size_bea
+00008de0: 6d22 292c 0a20 2020 2020 2020 2020 2020  m"),.           
+00008df0: 2029 0a20 2020 2020 2020 2069 6620 7365   ).        if se
+00008e00: 6c66 2e62 6174 6368 2061 6e64 2062 6174  lf.batch and bat
+00008e10: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
+00008e20: 6173 7365 7274 2073 656c 662e 6261 7463  assert self.batc
+00008e30: 6820 3d3d 2062 6174 6368 0a20 2020 2020  h == batch.     
+00008e40: 2020 2065 6c69 6620 6261 7463 6820 616e     elif batch an
+00008e50: 6420 6e6f 7420 7365 6c66 2e62 6174 6368  d not self.batch
+00008e60: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00008e70: 6c66 2e62 6174 6368 203d 2062 6174 6368  lf.batch = batch
+00008e80: 2020 2320 6f76 6572 7461 6b65 0a20 2020    # overtake.   
+00008e90: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00008ea0: 2e69 735f 6261 7463 685f 6469 6d28 2920  .is_batch_dim() 
+00008eb0: 616e 6420 7365 6c66 2e69 735f 6479 6e61  and self.is_dyna
+00008ec0: 6d69 6328 293a 0a20 2020 2020 2020 2020  mic():.         
+00008ed0: 2020 2069 6620 7361 6d65 5f61 735f 6265     if same_as_be
+00008ee0: 666f 7265 3a0a 2020 2020 2020 2020 2020  fore:.          
+00008ef0: 2020 2020 2020 6173 7365 7274 2073 656c        assert sel
+00008f00: 662e 6479 6e5f 7369 7a65 5f65 7874 2061  f.dyn_size_ext a
+00008f10: 6e64 2073 656c 662e 6479 6e5f 7369 7a65  nd self.dyn_size
+00008f20: 5f65 7874 2e70 6c61 6365 686f 6c64 6572  _ext.placeholder
+00008f30: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
+00008f40: 2020 2020 2020 2020 2020 2020 2023 2044               # D
+00008f50: 6f20 6e6f 7420 6f76 6572 7772 6974 6520  o not overwrite 
+00008f60: 6974 2e0a 2020 2020 2020 2020 2020 2020  it..            
+00008f70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+00008f80: 2020 2020 2020 7365 6c66 2e5f 696e 6974        self._init
+00008f90: 5f64 6566 6175 6c74 5f64 796e 5f73 697a  _default_dyn_siz
+00008fa0: 655f 6578 7428 7829 0a20 2020 2020 2020  e_ext(x).       
+00008fb0: 2069 6620 6765 7461 7474 7228 782c 2022   if getattr(x, "
+00008fc0: 5f69 735f 7369 7a65 5f6f 665f 6469 6d5f  _is_size_of_dim_
+00008fd0: 7461 6722 2c20 4e6f 6e65 2920 6973 204e  tag", None) is N
+00008fe0: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00008ff0: 2073 6574 6174 7472 2878 2c20 225f 6973   setattr(x, "_is
+00009000: 5f73 697a 655f 6f66 5f64 696d 5f74 6167  _size_of_dim_tag
+00009010: 222c 2073 656c 6629 0a20 2020 2020 2020  ", self).       
+00009020: 2072 6574 7572 6e20 7365 6c66 0a0a 2020   return self..  
+00009030: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+00009040: 2020 2064 6566 2067 6574 5f74 6167 5f66     def get_tag_f
+00009050: 726f 6d5f 7369 7a65 5f74 656e 736f 7228  rom_size_tensor(
+00009060: 636c 732c 2078 2920 2d3e 204f 7074 696f  cls, x) -> Optio
+00009070: 6e61 6c5b 5f64 2e44 696d 5d3a 0a20 2020  nal[_d.Dim]:.   
+00009080: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00009090: 203a 7061 7261 6d20 7466 2e54 656e 736f   :param tf.Tenso
+000090a0: 7220 783a 2073 697a 6520 7465 6e73 6f72  r x: size tensor
+000090b0: 2e20 6861 7320 6265 656e 2073 6574 2062  . has been set b
+000090c0: 6566 6f72 6520 7669 6120 3a66 756e 633a  efore via :func:
+000090d0: 6073 6574 5f74 6167 5f6f 6e5f 7369 7a65  `set_tag_on_size
+000090e0: 5f74 656e 736f 7260 0a20 2020 2020 2020  _tensor`.       
+000090f0: 2022 2222 0a20 2020 2020 2020 2072 6574   """.        ret
+00009100: 7572 6e20 6765 7461 7474 7228 782c 2022  urn getattr(x, "
+00009110: 5f69 735f 7369 7a65 5f6f 665f 6469 6d5f  _is_size_of_dim_
+00009120: 7461 6722 2c20 4e6f 6e65 290a 0a20 2020  tag", None)..   
+00009130: 2064 6566 2063 6f6d 706c 6574 655f 6479   def complete_dy
+00009140: 6e5f 7369 7a65 2873 656c 662c 2074 656d  n_size(self, tem
+00009150: 706c 6174 655f 6f6e 6c79 3d46 616c 7365  plate_only=False
+00009160: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00009170: 2020 2020 2020 2049 6e20 6361 7365 2077         In case w
+00009180: 6520 6361 6e20 6361 6c63 756c 6174 6520  e can calculate 
+00009190: 7468 6520 6479 6e20 7369 7a65 2c20 646f  the dyn size, do
+000091a0: 2074 6861 7420 6e6f 772e 0a0a 2020 2020   that now...    
+000091b0: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
+000091c0: 7465 6d70 6c61 7465 5f6f 6e6c 793a 0a20  template_only:. 
+000091d0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000091e0: 2020 2069 6620 6e6f 7420 7365 6c66 2e69     if not self.i
+000091f0: 735f 6479 6e61 6d69 6328 293a 0a20 2020  s_dynamic():.   
+00009200: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+00009210: 2020 2020 2020 2020 7365 6c66 2e5f 7661          self._va
+00009220: 6c69 6461 7465 5f69 6e5f 6375 7272 656e  lidate_in_curren
+00009230: 745f 6772 6170 6828 290a 2020 2020 2020  t_graph().      
+00009240: 2020 6966 2073 656c 662e 6479 6e5f 7369    if self.dyn_si
+00009250: 7a65 5f65 7874 2061 6e64 2028 7365 6c66  ze_ext and (self
+00009260: 2e64 796e 5f73 697a 655f 6578 742e 706c  .dyn_size_ext.pl
+00009270: 6163 6568 6f6c 6465 7220 6973 206e 6f74  aceholder is not
+00009280: 204e 6f6e 6520 6f72 2074 656d 706c 6174   None or templat
+00009290: 655f 6f6e 6c79 293a 0a20 2020 2020 2020  e_only):.       
+000092a0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+000092b0: 2020 2020 7361 6d65 5f62 6173 6520 3d20      same_base = 
+000092c0: 7365 6c66 2e67 6574 5f73 616d 655f 6261  self.get_same_ba
+000092d0: 7365 2829 0a20 2020 2020 2020 206f 7020  se().        op 
+000092e0: 3d20 7365 6c66 2e64 6572 6976 6564 5f66  = self.derived_f
+000092f0: 726f 6d5f 6f70 206f 7220 7361 6d65 5f62  rom_op or same_b
+00009300: 6173 652e 6465 7269 7665 645f 6672 6f6d  ase.derived_from
+00009310: 5f6f 700a 2020 2020 2020 2020 6966 206e  _op.        if n
+00009320: 6f74 206f 703a 0a20 2020 2020 2020 2020  ot op:.         
+00009330: 2020 2072 6574 7572 6e0a 0a20 2020 2020     return..     
+00009340: 2020 2066 6f72 2078 2069 6e20 6f70 2e69     for x in op.i
+00009350: 6e70 7574 733a 0a20 2020 2020 2020 2020  nputs:.         
+00009360: 2020 2069 6620 7365 6c66 2e62 6174 6368     if self.batch
+00009370: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009380: 2020 7820 3d20 782e 6765 745f 666f 725f    x = x.get_for_
+00009390: 6261 7463 685f 6374 7828 7365 6c66 2e62  batch_ctx(self.b
+000093a0: 6174 6368 2c20 7365 6c66 2e63 6f6e 7472  atch, self.contr
+000093b0: 6f6c 5f66 6c6f 775f 6374 7829 0a20 2020  ol_flow_ctx).   
+000093c0: 2020 2020 2020 2020 2078 2e63 6f6d 706c           x.compl
+000093d0: 6574 655f 6479 6e5f 7369 7a65 2874 656d  ete_dyn_size(tem
+000093e0: 706c 6174 655f 6f6e 6c79 3d74 656d 706c  plate_only=templ
+000093f0: 6174 655f 6f6e 6c79 290a 0a20 2020 2020  ate_only)..     
+00009400: 2020 2062 6163 6b65 6e64 203d 204e 6f6e     backend = Non
+00009410: 650a 2020 2020 2020 2020 666f 7220 7820  e.        for x 
+00009420: 696e 206f 702e 696e 7075 7473 3a0a 2020  in op.inputs:.  
+00009430: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+00009440: 662e 6261 7463 683a 0a20 2020 2020 2020  f.batch:.       
+00009450: 2020 2020 2020 2020 2078 203d 2078 2e67           x = x.g
+00009460: 6574 5f66 6f72 5f62 6174 6368 5f63 7478  et_for_batch_ctx
+00009470: 2873 656c 662e 6261 7463 682c 2073 656c  (self.batch, sel
+00009480: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
+00009490: 7478 290a 2020 2020 2020 2020 2020 2020  tx).            
+000094a0: 6966 2078 2e64 796e 5f73 697a 655f 6578  if x.dyn_size_ex
+000094b0: 7420 616e 6420 782e 6479 6e5f 7369 7a65  t and x.dyn_size
+000094c0: 5f65 7874 2e72 6177 5f74 656e 736f 7220  _ext.raw_tensor 
+000094d0: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+000094e0: 2020 2020 2020 2020 2020 2020 2023 206e               # n
+000094f0: 6f69 6e73 7065 6374 696f 6e20 5079 5072  oinspection PyPr
+00009500: 6f74 6563 7465 644d 656d 6265 720a 2020  otectedMember.  
+00009510: 2020 2020 2020 2020 2020 2020 2020 6261                ba
+00009520: 636b 656e 6420 3d20 782e 6479 6e5f 7369  ckend = x.dyn_si
+00009530: 7a65 5f65 7874 2e5f 7261 775f 6261 636b  ze_ext._raw_back
+00009540: 656e 640a 2020 2020 2020 2020 2020 2020  end.            
+00009550: 2020 2020 6272 6561 6b0a 0a20 2020 2020      break..     
+00009560: 2020 2073 697a 655f 6474 7970 6520 3d20     size_dtype = 
+00009570: 4e6f 6e65 0a20 2020 2020 2020 2066 6f72  None.        for
+00009580: 2078 2069 6e20 6f70 2e69 6e70 7574 733a   x in op.inputs:
+00009590: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+000095a0: 7365 6c66 2e62 6174 6368 3a0a 2020 2020  self.batch:.    
+000095b0: 2020 2020 2020 2020 2020 2020 7820 3d20              x = 
+000095c0: 782e 6765 745f 666f 725f 6261 7463 685f  x.get_for_batch_
+000095d0: 6374 7828 7365 6c66 2e62 6174 6368 2c20  ctx(self.batch, 
+000095e0: 7365 6c66 2e63 6f6e 7472 6f6c 5f66 6c6f  self.control_flo
+000095f0: 775f 6374 7829 0a20 2020 2020 2020 2020  w_ctx).         
+00009600: 2020 2069 6620 782e 6479 6e5f 7369 7a65     if x.dyn_size
+00009610: 5f65 7874 3a0a 2020 2020 2020 2020 2020  _ext:.          
+00009620: 2020 2020 2020 7369 7a65 5f64 7479 7065        size_dtype
+00009630: 203d 2078 2e64 796e 5f73 697a 655f 6578   = x.dyn_size_ex
+00009640: 742e 6474 7970 650a 2020 2020 2020 2020  t.dtype.        
+00009650: 2020 2020 2020 2020 6272 6561 6b0a 2020          break.  
+00009660: 2020 2020 2020 6966 206e 6f74 2073 697a        if not siz
+00009670: 655f 6474 7970 653a 0a20 2020 2020 2020  e_dtype:.       
+00009680: 2020 2020 2073 697a 655f 6474 7970 6520       size_dtype 
+00009690: 3d20 5f74 2e54 656e 736f 722e 7369 7a65  = _t.Tensor.size
+000096a0: 5f64 7479 7065 0a0a 2020 2020 2020 2020  _dtype..        
+000096b0: 696d 706f 7274 206e 756d 7079 0a20 2020  import numpy.   
+000096c0: 2020 2020 2069 6d70 6f72 7420 7265 7475       import retu
+000096d0: 726e 6e2e 6672 6f6e 7465 6e64 2061 7320  rnn.frontend as 
+000096e0: 7266 0a0a 2020 2020 2020 2020 7466 203d  rf..        tf =
+000096f0: 2074 665f 7574 696c 203d 2074 656e 736f   tf_util = tenso
+00009700: 725f 7574 696c 203d 204e 6f6e 650a 2020  r_util = None.  
+00009710: 2020 2020 2020 6966 2062 6163 6b65 6e64        if backend
+00009720: 2061 6e64 2062 6163 6b65 6e64 2e69 735f   and backend.is_
+00009730: 7465 6e73 6f72 666c 6f77 3a0a 2020 2020  tensorflow:.    
+00009740: 2020 2020 2020 2020 696d 706f 7274 2074          import t
+00009750: 656e 736f 7266 6c6f 7720 6173 2074 660a  ensorflow as tf.
+00009760: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00009770: 6261 636b 656e 642e 5261 7754 656e 736f  backend.RawTenso
+00009780: 7254 7970 6520 3d3d 2074 662e 5465 6e73  rType == tf.Tens
+00009790: 6f72 3a0a 2020 2020 2020 2020 2020 2020  or:.            
+000097a0: 2020 2020 6672 6f6d 2072 6574 7572 6e6e      from returnn
+000097b0: 2e74 662e 7574 696c 2069 6d70 6f72 7420  .tf.util import 
+000097c0: 6261 7369 6320 6173 2074 665f 7574 696c  basic as tf_util
+000097d0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000097e0: 2066 726f 6d20 7465 6e73 6f72 666c 6f77   from tensorflow
+000097f0: 2e70 7974 686f 6e2e 6672 616d 6577 6f72  .python.framewor
+00009800: 6b20 696d 706f 7274 2074 656e 736f 725f  k import tensor_
+00009810: 7574 696c 0a20 2020 2020 2020 2020 2020  util.           
+00009820: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
+00009830: 2020 2020 2020 2074 6620 3d20 4e6f 6e65         tf = None
+00009840: 0a0a 2020 2020 2020 2020 6b69 6e64 203d  ..        kind =
+00009850: 206f 702e 6b69 6e64 0a20 2020 2020 2020   op.kind.       
+00009860: 2069 6620 6b69 6e64 2e65 6e64 7377 6974   if kind.endswit
+00009870: 6828 225f 7269 6768 7422 293a 0a20 2020  h("_right"):.   
+00009880: 2020 2020 2020 2020 206b 696e 6420 3d20           kind = 
+00009890: 6b69 6e64 5b3a 202d 6c65 6e28 225f 7269  kind[: -len("_ri
+000098a0: 6768 7422 295d 2020 2320 6f72 6465 7220  ght")]  # order 
+000098b0: 646f 6573 206e 6f74 206d 6174 7465 7220  does not matter 
+000098c0: 6865 7265 0a20 2020 2020 2020 2069 6620  here.        if 
+000098d0: 6b69 6e64 2e65 6e64 7377 6974 6828 225f  kind.endswith("_
+000098e0: 6c65 6674 2229 3a0a 2020 2020 2020 2020  left"):.        
+000098f0: 2020 2020 6b69 6e64 203d 206b 696e 645b      kind = kind[
+00009900: 3a20 2d6c 656e 2822 5f6c 6566 7422 295d  : -len("_left")]
+00009910: 0a0a 2020 2020 2020 2020 6465 6620 5f69  ..        def _i
+00009920: 735f 6e65 6761 7469 7665 2878 5f5f 293a  s_negative(x__):
+00009930: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00009940: 6973 696e 7374 616e 6365 2878 5f5f 2c20  isinstance(x__, 
+00009950: 6e75 6d70 792e 6e64 6172 7261 7929 3a0a  numpy.ndarray):.
 00009960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009970: 7265 7475 726e 205f 6973 5f6e 6567 6174  return _is_negat
-00009980: 6976 6528 785f 5f29 0a20 2020 2020 2020  ive(x__).       
-00009990: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-000099a0: 650a 0a20 2020 2020 2020 2064 6566 205f  e..        def _
-000099b0: 6269 6e5f 6f70 5f74 6628 612c 2062 293a  bin_op_tf(a, b):
-000099c0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-000099d0: 7465 6d70 6c61 7465 5f6f 6e6c 793a 0a20  template_only:. 
-000099e0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000099f0: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
-00009a00: 2020 2020 2020 2069 6620 6120 6973 204e         if a is N
-00009a10: 6f6e 6520 6f72 2062 2069 7320 4e6f 6e65  one or b is None
-00009a20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00009a30: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
-00009a40: 2020 2020 2020 2020 2020 6173 7365 7274            assert
-00009a50: 2069 7369 6e73 7461 6e63 6528 612c 2074   isinstance(a, t
-00009a60: 662e 5465 6e73 6f72 2920 616e 6420 6973  f.Tensor) and is
-00009a70: 696e 7374 616e 6365 2862 2c20 2869 6e74  instance(b, (int
-00009a80: 2c20 7466 2e54 656e 736f 7229 290a 2020  , tf.Tensor)).  
-00009a90: 2020 2020 2020 2020 2020 7769 7468 2074            with t
-00009aa0: 665f 7574 696c 2e73 616d 655f 636f 6e74  f_util.same_cont
-00009ab0: 726f 6c5f 666c 6f77 5f63 7478 285b 612c  rol_flow_ctx([a,
-00009ac0: 2062 5d29 3a0a 2020 2020 2020 2020 2020   b]):.          
-00009ad0: 2020 2020 2020 6966 206b 696e 6420 3d3d        if kind ==
-00009ae0: 2022 6164 6422 3a0a 2020 2020 2020 2020   "add":.        
-00009af0: 2020 2020 2020 2020 2020 2020 7573 655f              use_
-00009b00: 7265 6c75 203d 205f 6973 5f6e 6567 6174  relu = _is_negat
-00009b10: 6976 6528 6129 206f 7220 5f69 735f 6e65  ive(a) or _is_ne
-00009b20: 6761 7469 7665 2862 2920 2023 2066 6f72  gative(b)  # for
-00009b30: 2064 796e 616d 6963 2074 656e 736f 7273   dynamic tensors
-00009b40: 2c20 6173 7375 6d65 2061 6c6c 2070 6f73  , assume all pos
-00009b50: 6974 6976 650a 2020 2020 2020 2020 2020  itive.          
-00009b60: 2020 2020 2020 2020 2020 6966 2075 7365            if use
-00009b70: 5f72 656c 753a 0a20 2020 2020 2020 2020  _relu:.         
-00009b80: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00009b90: 6574 7572 6e20 7466 2e63 6f6e 7665 7274  eturn tf.convert
-00009ba0: 5f74 6f5f 7465 6e73 6f72 2874 665f 7574  _to_tensor(tf_ut
-00009bb0: 696c 2e73 696d 706c 6966 795f 6e6f 6e5f  il.simplify_non_
-00009bc0: 6e65 6761 7469 7665 5f73 6571 5f6c 656e  negative_seq_len
-00009bd0: 6774 6828 6120 2b20 6229 290a 2020 2020  gth(a + b)).    
-00009be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009bf0: 7265 7475 726e 2061 202b 2062 0a20 2020  return a + b.   
-00009c00: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
-00009c10: 6620 6b69 6e64 203d 3d20 2273 7562 223a  f kind == "sub":
-00009c20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00009c30: 2020 2020 2072 6574 7572 6e20 7466 2e63       return tf.c
-00009c40: 6f6e 7665 7274 5f74 6f5f 7465 6e73 6f72  onvert_to_tensor
-00009c50: 2874 665f 7574 696c 2e73 696d 706c 6966  (tf_util.simplif
-00009c60: 795f 6e6f 6e5f 6e65 6761 7469 7665 5f73  y_non_negative_s
-00009c70: 6571 5f6c 656e 6774 6828 6120 2d20 6229  eq_length(a - b)
-00009c80: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00009c90: 2020 656c 6966 206b 696e 6420 3d3d 2022    elif kind == "
-00009ca0: 6d75 6c22 3a0a 2020 2020 2020 2020 2020  mul":.          
-00009cb0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009cc0: 2061 202a 2062 0a20 2020 2020 2020 2020   a * b.         
-00009cd0: 2020 2020 2020 2065 6c69 6620 6b69 6e64         elif kind
-00009ce0: 2069 6e20 2822 666c 6f6f 7264 6976 222c   in ("floordiv",
-00009cf0: 2022 7472 7565 6469 7622 293a 2020 2320   "truediv"):  # 
-00009d00: 7472 7565 6469 7620 6173 7375 6d65 7320  truediv assumes 
-00009d10: 7468 6572 6520 6973 206e 6f20 7265 6d61  there is no rema
-00009d20: 696e 6465 720a 2020 2020 2020 2020 2020  inder.          
-00009d30: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00009d40: 2061 202f 2f20 620a 2020 2020 2020 2020   a // b.        
-00009d50: 2020 2020 2020 2020 656c 6966 206b 696e          elif kin
-00009d60: 6420 3d3d 2022 6365 696c 6469 7622 3a0a  d == "ceildiv":.
-00009d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009d80: 2020 2020 7265 7475 726e 202d 282d 6120      return -(-a 
-00009d90: 2f2f 2062 290a 2020 2020 2020 2020 2020  // b).          
-00009da0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
-00009db0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009dc0: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00009dd0: 2822 756e 6b6e 6f77 6e20 6f70 206b 696e  ("unknown op kin
-00009de0: 6420 2572 2220 2520 6f70 2e6b 696e 6429  d %r" % op.kind)
-00009df0: 0a0a 2020 2020 2020 2020 6465 6620 5f62  ..        def _b
-00009e00: 696e 5f6f 7028 612c 2062 293a 0a20 2020  in_op(a, b):.   
-00009e10: 2020 2020 2020 2020 2069 6620 7465 6d70           if temp
-00009e20: 6c61 7465 5f6f 6e6c 7920 6f72 206e 6f74  late_only or not
-00009e30: 2062 6163 6b65 6e64 3a0a 2020 2020 2020   backend:.      
-00009e40: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-00009e50: 6e73 7461 6e63 6528 612c 205f 742e 5465  nstance(a, _t.Te
-00009e60: 6e73 6f72 2920 616e 6420 6973 696e 7374  nsor) and isinst
-00009e70: 616e 6365 2862 2c20 5f74 2e54 656e 736f  ance(b, _t.Tenso
-00009e80: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-00009e90: 2020 2020 2020 2020 7265 7475 726e 205f          return _
-00009ea0: 742e 5465 6e73 6f72 2e67 6574 5f63 6f6d  t.Tensor.get_com
-00009eb0: 6d6f 6e5f 6461 7461 285b 612c 2062 5d2c  mon_data([a, b],
-00009ec0: 2061 6c6c 6f77 5f62 726f 6164 6361 7374   allow_broadcast
-00009ed0: 5f61 6c6c 5f73 6f75 7263 6573 3d54 7275  _all_sources=Tru
-00009ee0: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
-00009ef0: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
-00009f00: 2861 2c20 5f74 2e54 656e 736f 7229 3a0a  (a, _t.Tensor):.
-00009f10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00009f20: 2020 2020 7265 7475 726e 2061 0a20 2020      return a.   
-00009f30: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00009f40: 6973 696e 7374 616e 6365 2862 2c20 5f74  isinstance(b, _t
-00009f50: 2e54 656e 736f 7229 3a0a 2020 2020 2020  .Tensor):.      
-00009f60: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00009f70: 7475 726e 2062 0a20 2020 2020 2020 2020  turn b.         
-00009f80: 2020 2069 6620 6b69 6e64 203d 3d20 2261     if kind == "a
-00009f90: 6464 223a 0a20 2020 2020 2020 2020 2020  dd":.           
-00009fa0: 2020 2020 2072 6574 7572 6e20 5f72 656c       return _rel
-00009fb0: 7528 6120 2b20 6229 0a20 2020 2020 2020  u(a + b).       
-00009fc0: 2020 2020 2065 6c69 6620 6b69 6e64 203d       elif kind =
-00009fd0: 3d20 2273 7562 223a 0a20 2020 2020 2020  = "sub":.       
-00009fe0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00009ff0: 5f72 656c 7528 6120 2d20 6229 0a20 2020  _relu(a - b).   
-0000a000: 2020 2020 2020 2020 2065 6c69 6620 6b69           elif ki
-0000a010: 6e64 203d 3d20 226d 756c 223a 0a20 2020  nd == "mul":.   
-0000a020: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-0000a030: 7572 6e20 6120 2a20 620a 2020 2020 2020  urn a * b.      
-0000a040: 2020 2020 2020 656c 6966 206b 696e 6420        elif kind 
-0000a050: 696e 2028 2266 6c6f 6f72 6469 7622 2c20  in ("floordiv", 
-0000a060: 2274 7275 6564 6976 2229 3a20 2023 2074  "truediv"):  # t
-0000a070: 7275 6564 6976 2061 7373 756d 6573 2074  ruediv assumes t
-0000a080: 6865 7265 2069 7320 6e6f 2072 656d 6169  here is no remai
-0000a090: 6e64 6572 0a20 2020 2020 2020 2020 2020  nder.           
-0000a0a0: 2020 2020 2072 6574 7572 6e20 6120 2f2f       return a //
-0000a0b0: 2062 0a20 2020 2020 2020 2020 2020 2065   b.            e
-0000a0c0: 6c69 6620 6b69 6e64 203d 3d20 2263 6569  lif kind == "cei
-0000a0d0: 6c64 6976 223a 0a20 2020 2020 2020 2020  ldiv":.         
-0000a0e0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-0000a0f0: 616e 6365 2861 2c20 5f74 2e54 656e 736f  ance(a, _t.Tenso
-0000a100: 7229 3a0a 2020 2020 2020 2020 2020 2020  r):.            
-0000a110: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-0000a120: 662e 6365 696c 5f64 6976 6964 6528 612c  f.ceil_divide(a,
-0000a130: 2062 290a 2020 2020 2020 2020 2020 2020   b).            
-0000a140: 2020 2020 7265 7475 726e 202d 282d 6120      return -(-a 
-0000a150: 2f2f 2062 290a 2020 2020 2020 2020 2020  // b).          
-0000a160: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000a170: 2020 2020 2020 2020 7261 6973 6520 5661          raise Va
-0000a180: 6c75 6545 7272 6f72 2822 756e 6b6e 6f77  lueError("unknow
-0000a190: 6e20 6f70 206b 696e 6420 2572 2220 2520  n op kind %r" % 
-0000a1a0: 6f70 2e6b 696e 6429 0a0a 2020 2020 2020  op.kind)..      
-0000a1b0: 2020 6465 6620 5f72 656c 7528 6129 3a0a    def _relu(a):.
-0000a1c0: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-0000a1d0: 7369 6e73 7461 6e63 6528 612c 205f 742e  sinstance(a, _t.
-0000a1e0: 5465 6e73 6f72 293a 0a20 2020 2020 2020  Tensor):.       
-0000a1f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000a200: 7266 2e72 656c 7528 6129 0a20 2020 2020  rf.relu(a).     
-0000a210: 2020 2020 2020 2065 6c69 6620 6973 696e         elif isin
-0000a220: 7374 616e 6365 2861 2c20 696e 7429 3a0a  stance(a, int):.
-0000a230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a240: 7265 7475 726e 206d 6178 2861 2c20 3029  return max(a, 0)
-0000a250: 0a20 2020 2020 2020 2020 2020 2065 6c73  .            els
-0000a260: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
-0000a270: 2020 2072 6169 7365 2054 7970 6545 7272     raise TypeErr
-0000a280: 6f72 2866 2263 6f6d 706c 6574 655f 6479  or(f"complete_dy
-0000a290: 6e5f 7369 7a65 3a20 5f72 656c 753a 2075  n_size: _relu: u
-0000a2a0: 6e65 7870 6563 7465 6420 7479 7065 207b  nexpected type {
-0000a2b0: 7479 7065 2861 297d 2229 0a0a 2020 2020  type(a)}")..    
-0000a2c0: 2020 2020 795f 6e61 6d65 203d 2073 656c      y_name = sel
-0000a2d0: 662e 6465 7363 7269 7074 696f 6e20 2b20  f.description + 
-0000a2e0: 223a 7365 712d 6c65 6e67 7468 220a 2020  ":seq-length".  
-0000a2f0: 2020 2020 2020 793a 204f 7074 696f 6e61        y: Optiona
-0000a300: 6c5b 5f74 2e54 656e 736f 725d 203d 204e  l[_t.Tensor] = N
-0000a310: 6f6e 6520 2023 2072 6573 756c 7469 6e67  one  # resulting
-0000a320: 2064 796e 2073 697a 650a 2020 2020 2020   dyn size.      
-0000a330: 2020 696e 7075 7473 203d 206c 6973 7428    inputs = list(
-0000a340: 6f70 2e69 6e70 7574 7329 0a20 2020 2020  op.inputs).     
-0000a350: 2020 2061 7373 6572 7420 696e 7075 7473     assert inputs
-0000a360: 0a20 2020 2020 2020 2077 6869 6c65 2069  .        while i
-0000a370: 6e70 7574 733a 0a20 2020 2020 2020 2020  nputs:.         
-0000a380: 2020 2078 203d 2069 6e70 7574 732e 706f     x = inputs.po
-0000a390: 7028 3029 0a20 2020 2020 2020 2020 2020  p(0).           
-0000a3a0: 2069 6620 6e6f 7420 782e 6973 5f64 796e   if not x.is_dyn
-0000a3b0: 616d 6963 2829 3a20 2023 2073 7461 7469  amic():  # stati
-0000a3c0: 630a 2020 2020 2020 2020 2020 2020 2020  c.              
-0000a3d0: 2020 6173 7365 7274 2078 2e64 696d 656e    assert x.dimen
-0000a3e0: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
-0000a3f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a400: 2069 6620 7920 6973 204e 6f6e 653a 0a20   if y is None:. 
-0000a410: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a420: 2020 2069 6620 6e6f 7420 7465 6d70 6c61     if not templa
-0000a430: 7465 5f6f 6e6c 7920 616e 6420 6261 636b  te_only and back
-0000a440: 656e 6420 616e 6420 6e6f 7420 7466 3a0a  end and not tf:.
-0000a450: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a460: 2020 2020 2020 2020 7920 3d20 6261 636b          y = back
-0000a470: 656e 642e 636f 6e76 6572 745f 746f 5f74  end.convert_to_t
-0000a480: 656e 736f 7228 782e 6469 6d65 6e73 696f  ensor(x.dimensio
-0000a490: 6e2c 2064 696d 733d 5b5d 2c20 6474 7970  n, dims=[], dtyp
-0000a4a0: 653d 7369 7a65 5f64 7479 7065 2c20 6e61  e=size_dtype, na
-0000a4b0: 6d65 3d79 5f6e 616d 6529 0a20 2020 2020  me=y_name).     
-0000a4c0: 2020 2020 2020 2020 2020 2020 2020 2065                 e
-0000a4d0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000a4e0: 2020 2020 2020 2020 2020 2020 2079 203d               y =
-0000a4f0: 205f 742e 5465 6e73 6f72 280a 2020 2020   _t.Tensor(.    
-0000a500: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a510: 2020 2020 2020 2020 6e61 6d65 3d79 5f6e          name=y_n
-0000a520: 616d 652c 0a20 2020 2020 2020 2020 2020  ame,.           
-0000a530: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a540: 2064 696d 5f74 6167 733d 5b5d 2c0a 2020   dim_tags=[],.  
-0000a550: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a560: 2020 2020 2020 2020 2020 6474 7970 653d            dtype=
-0000a570: 7369 7a65 5f64 7479 7065 2c0a 2020 2020  size_dtype,.    
-0000a580: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a590: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-0000a5a0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000a5b0: 206e 6f74 2074 656d 706c 6174 655f 6f6e   not template_on
-0000a5c0: 6c79 2061 6e64 2074 663a 0a20 2020 2020  ly and tf:.     
-0000a5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a5e0: 2020 2020 2020 2077 6974 6820 7466 2e63         with tf.c
-0000a5f0: 6f6e 7472 6f6c 5f64 6570 656e 6465 6e63  ontrol_dependenc
-0000a600: 6965 7328 4e6f 6e65 293a 2020 2320 7468  ies(None):  # th
-0000a610: 6973 2077 696c 6c20 7265 7365 7420 7468  is will reset th
-0000a620: 6520 636f 6e74 6578 740a 2020 2020 2020  e context.      
-0000a630: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a640: 2020 2020 2020 2020 2020 792e 7261 775f            y.raw_
-0000a650: 7465 6e73 6f72 203d 2074 662e 636f 6e73  tensor = tf.cons
-0000a660: 7461 6e74 2878 2e64 696d 656e 7369 6f6e  tant(x.dimension
-0000a670: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000a680: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
-0000a690: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000a6a0: 6620 7466 3a0a 2020 2020 2020 2020 2020  f tf:.          
-0000a6b0: 2020 2020 2020 2020 2020 792e 706c 6163            y.plac
-0000a6c0: 6568 6f6c 6465 7220 3d20 5f62 696e 5f6f  eholder = _bin_o
-0000a6d0: 705f 7466 2879 2e70 6c61 6365 686f 6c64  p_tf(y.placehold
-0000a6e0: 6572 2c20 782e 6469 6d65 6e73 696f 6e29  er, x.dimension)
-0000a6f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000a700: 2065 6c73 653a 0a20 2020 2020 2020 2020   else:.         
-0000a710: 2020 2020 2020 2020 2020 2079 203d 205f             y = _
-0000a720: 6269 6e5f 6f70 2879 2c20 782e 6469 6d65  bin_op(y, x.dime
-0000a730: 6e73 696f 6e29 0a20 2020 2020 2020 2020  nsion).         
-0000a740: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
-0000a750: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000a760: 656c 662e 6261 7463 683a 0a20 2020 2020  elf.batch:.     
-0000a770: 2020 2020 2020 2020 2020 2078 203d 2078             x = x
-0000a780: 2e67 6574 5f66 6f72 5f62 6174 6368 5f63  .get_for_batch_c
-0000a790: 7478 2873 656c 662e 6261 7463 682c 2073  tx(self.batch, s
-0000a7a0: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
-0000a7b0: 5f63 7478 290a 2020 2020 2020 2020 2020  _ctx).          
-0000a7c0: 2020 782e 636f 6d70 6c65 7465 5f64 796e    x.complete_dyn
-0000a7d0: 5f73 697a 6528 7465 6d70 6c61 7465 5f6f  _size(template_o
-0000a7e0: 6e6c 793d 7465 6d70 6c61 7465 5f6f 6e6c  nly=template_onl
-0000a7f0: 7929 0a20 2020 2020 2020 2020 2020 2069  y).            i
-0000a800: 6620 6e6f 7420 782e 6479 6e5f 7369 7a65  f not x.dyn_size
-0000a810: 5f65 7874 3a0a 2020 2020 2020 2020 2020  _ext:.          
-0000a820: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-0000a830: 2020 2020 2020 2020 2078 203d 2078 2e64           x = x.d
-0000a840: 796e 5f73 697a 655f 6578 740a 2020 2020  yn_size_ext.    
-0000a850: 2020 2020 2020 2020 6966 2079 2069 7320          if y is 
-0000a860: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
-0000a870: 2020 2020 2020 7920 3d20 782e 636f 7079        y = x.copy
-0000a880: 286e 616d 653d 795f 6e61 6d65 290a 2020  (name=y_name).  
-0000a890: 2020 2020 2020 2020 2020 2020 2020 636f                co
-0000a8a0: 6e74 696e 7565 0a20 2020 2020 2020 2020  ntinue.         
-0000a8b0: 2020 2069 6620 782e 6469 6d5f 7461 6773     if x.dim_tags
-0000a8c0: 2021 3d20 792e 6469 6d5f 7461 6773 3a0a   != y.dim_tags:.
-0000a8d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000a8e0: 636f 6d6d 6f6e 203d 205f 742e 5465 6e73  common = _t.Tens
-0000a8f0: 6f72 2e67 6574 5f63 6f6d 6d6f 6e5f 6461  or.get_common_da
-0000a900: 7461 285b 782c 2079 5d2c 2061 6c6c 6f77  ta([x, y], allow
-0000a910: 5f62 726f 6164 6361 7374 5f61 6c6c 5f73  _broadcast_all_s
-0000a920: 6f75 7263 6573 3d54 7275 6529 0a20 2020  ources=True).   
-0000a930: 2020 2020 2020 2020 2020 2020 2078 5f20               x_ 
-0000a940: 3d20 782e 636f 7079 5f63 6f6d 7061 7469  = x.copy_compati
-0000a950: 626c 655f 746f 2863 6f6d 6d6f 6e29 2069  ble_to(common) i
-0000a960: 6620 782e 6469 6d5f 7461 6773 2065 6c73  f x.dim_tags els
-0000a970: 6520 780a 2020 2020 2020 2020 2020 2020  e x.            
-0000a980: 2020 2020 795f 203d 2079 2e63 6f70 795f      y_ = y.copy_
-0000a990: 636f 6d70 6174 6962 6c65 5f74 6f28 636f  compatible_to(co
-0000a9a0: 6d6d 6f6e 2920 6966 2079 2e64 696d 5f74  mmon) if y.dim_t
-0000a9b0: 6167 7320 656c 7365 2079 0a20 2020 2020  ags else y.     
-0000a9c0: 2020 2020 2020 2020 2020 2079 203d 2063             y = c
-0000a9d0: 6f6d 6d6f 6e0a 2020 2020 2020 2020 2020  ommon.          
-0000a9e0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000a9f0: 2020 2020 2020 2020 785f 2c20 795f 203d          x_, y_ =
-0000aa00: 2078 2c20 790a 2020 2020 2020 2020 2020   x, y.          
-0000aa10: 2020 6966 2074 663a 0a20 2020 2020 2020    if tf:.       
-0000aa20: 2020 2020 2020 2020 2079 2e70 6c61 6365           y.place
-0000aa30: 686f 6c64 6572 203d 205f 6269 6e5f 6f70  holder = _bin_op
-0000aa40: 5f74 6628 795f 2e70 6c61 6365 686f 6c64  _tf(y_.placehold
-0000aa50: 6572 2c20 785f 2e70 6c61 6365 686f 6c64  er, x_.placehold
-0000aa60: 6572 290a 2020 2020 2020 2020 2020 2020  er).            
-0000aa70: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-0000aa80: 2020 2020 2020 7920 3d20 5f62 696e 5f6f        y = _bin_o
-0000aa90: 7028 795f 2c20 785f 290a 2020 2020 2020  p(y_, x_).      
-0000aaa0: 2020 6173 7365 7274 2079 2c20 6622 6f70    assert y, f"op
-0000aab0: 207b 6f70 7d3f 220a 2020 2020 2020 2020   {op}?".        
-0000aac0: 6966 2073 656c 662e 6479 6e5f 7369 7a65  if self.dyn_size
-0000aad0: 5f65 7874 3a0a 2020 2020 2020 2020 2020  _ext:.          
-0000aae0: 2020 6173 7365 7274 2073 656c 662e 6479    assert self.dy
-0000aaf0: 6e5f 7369 7a65 5f65 7874 2e64 696d 5f74  n_size_ext.dim_t
-0000ab00: 6167 7320 3d3d 2079 2e64 696d 5f74 6167  ags == y.dim_tag
-0000ab10: 730a 2020 2020 2020 2020 6966 2079 2e62  s.        if y.b
-0000ab20: 6174 6368 3a0a 2020 2020 2020 2020 2020  atch:.          
-0000ab30: 2020 6966 2073 656c 662e 6261 7463 683a    if self.batch:
-0000ab40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ab50: 2061 7373 6572 7420 7365 6c66 2e62 6174   assert self.bat
-0000ab60: 6368 203d 3d20 792e 6261 7463 680a 2020  ch == y.batch.  
-0000ab70: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-0000ab80: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000ab90: 7365 6c66 2e62 6174 6368 203d 2079 2e62  self.batch = y.b
-0000aba0: 6174 6368 0a20 2020 2020 2020 2073 656c  atch.        sel
-0000abb0: 662e 6479 6e5f 7369 7a65 5f65 7874 203d  f.dyn_size_ext =
-0000abc0: 2079 0a20 2020 2020 2020 2069 6620 7466   y.        if tf
-0000abd0: 2061 6e64 2079 2e70 6c61 6365 686f 6c64   and y.placehold
-0000abe0: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a0a  er is not None:.
-0000abf0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-0000ac00: 2e73 6574 5f74 6167 5f6f 6e5f 7369 7a65  .set_tag_on_size
-0000ac10: 5f74 656e 736f 7228 792e 706c 6163 6568  _tensor(y.placeh
-0000ac20: 6f6c 6465 7229 0a0a 2020 2020 6465 6620  older)..    def 
-0000ac30: 6973 5f65 7175 616c 280a 2020 2020 2020  is_equal(.      
-0000ac40: 2020 7365 6c66 2c0a 2020 2020 2020 2020    self,.        
-0000ac50: 6f74 6865 722c 0a20 2020 2020 2020 2069  other,.        i
-0000ac60: 676e 6f72 655f 6665 6174 7572 655f 6469  gnore_feature_di
-0000ac70: 6d3d 4661 6c73 652c 0a20 2020 2020 2020  m=False,.       
-0000ac80: 2061 6c6c 6f77 5f73 616d 655f 6665 6174   allow_same_feat
-0000ac90: 7572 655f 6469 6d3d 4661 6c73 652c 0a20  ure_dim=False,. 
-0000aca0: 2020 2020 2020 2061 6c6c 6f77 5f73 616d         allow_sam
-0000acb0: 655f 7370 6174 6961 6c5f 6469 6d3d 4e6f  e_spatial_dim=No
-0000acc0: 6e65 2c0a 2020 2020 2020 2020 7472 6561  ne,.        trea
-0000acd0: 745f 6665 6174 7572 655f 6173 5f73 7061  t_feature_as_spa
-0000ace0: 7469 616c 3d46 616c 7365 2c0a 2020 2020  tial=False,.    
-0000acf0: 2020 2020 6272 6f61 6463 6173 745f 6d61      broadcast_ma
-0000ad00: 7463 6865 733d 4661 6c73 652c 0a20 2020  tches=False,.   
-0000ad10: 2020 2020 2075 6e6b 6e6f 776e 5f73 7061       unknown_spa
-0000ad20: 7469 616c 5f6d 6174 6368 6573 3d46 616c  tial_matches=Fal
-0000ad30: 7365 2c0a 2020 2020 2020 2020 756e 6465  se,.        unde
-0000ad40: 6669 6e65 645f 6d61 7463 6865 733d 4661  fined_matches=Fa
-0000ad50: 6c73 652c 0a20 2020 2020 2020 2064 6572  lse,.        der
-0000ad60: 6976 6564 5f6d 6174 6368 6573 3d46 616c  ived_matches=Fal
-0000ad70: 7365 2c0a 2020 2020 293a 0a20 2020 2020  se,.    ):.     
-0000ad80: 2020 2022 2222 0a20 2020 2020 2020 2043     """.        C
-0000ad90: 6f6d 7061 7265 7320 7365 6c66 2074 6f20  ompares self to 
-0000ada0: 6f74 6865 7220 666f 7220 6571 7561 6c69  other for equali
-0000adb0: 7479 2e0a 0a20 2020 2020 2020 204e 6f74  ty...        Not
-0000adc0: 6520 7468 6174 2074 6865 2064 6566 6175  e that the defau
-0000add0: 6c74 2062 6568 6176 696f 7220 6973 2076  lt behavior is v
-0000ade0: 6572 7920 7265 7374 7269 6374 6976 652e  ery restrictive.
-0000adf0: 0a20 2020 2020 2020 2055 7365 2066 756e  .        Use fun
-0000ae00: 6374 696f 6e73 2073 7563 6820 6173 203a  ctions such as :
-0000ae10: 6675 6e63 3a60 6765 745f 616c 6c5f 6469  func:`get_all_di
-0000ae20: 6d65 6e73 696f 6e5f 7461 6773 6020 6f72  mension_tags` or
-0000ae30: 203a 6675 6e63 3a60 6765 745f 6578 6973   :func:`get_exis
-0000ae40: 7469 6e67 5f74 6167 5f66 726f 6d5f 636f  ting_tag_from_co
-0000ae50: 6c6c 6563 7469 6f6e 600a 2020 2020 2020  llection`.      
-0000ae60: 2020 746f 2065 7870 6c69 6369 746c 7920    to explicitly 
-0000ae70: 7370 6563 6966 7920 7468 6520 6265 6861  specify the beha
-0000ae80: 7669 6f72 2066 6f72 2074 6865 2063 6f6d  vior for the com
-0000ae90: 7061 7269 736f 6e2e 0a0a 2020 2020 2020  parison...      
-0000aea0: 2020 416c 736f 206e 6f74 6520 7468 6174    Also note that
-0000aeb0: 2074 6865 2064 6566 696e 6974 696f 6e20   the definition 
-0000aec0: 6973 2073 6c69 6768 746c 7920 6164 2d68  is slightly ad-h
-0000aed0: 6f63 2066 6f72 2073 6f6d 6520 6361 7365  oc for some case
-0000aee0: 732c 0a20 2020 2020 2020 2061 6e64 206d  s,.        and m
-0000aef0: 6967 6874 2070 6f74 656e 7469 616c 6c79  ight potentially
-0000af00: 2063 6861 6e67 6520 696e 2074 6865 2066   change in the f
-0000af10: 7574 7572 652e 0a20 2020 2020 2020 2020  uture..         
-0000af20: 2068 7474 7073 3a2f 2f67 6974 6875 622e   https://github.
-0000af30: 636f 6d2f 7277 7468 2d69 362f 7265 7475  com/rwth-i6/retu
-0000af40: 726e 6e2f 6973 7375 6573 2f36 3334 0a0a  rnn/issues/634..
-0000af50: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
-0000af60: 696d 206f 7468 6572 3a0a 2020 2020 2020  im other:.      
-0000af70: 2020 3a70 6172 616d 2062 6f6f 6c20 6967    :param bool ig
-0000af80: 6e6f 7265 5f66 6561 7475 7265 5f64 696d  nore_feature_dim
-0000af90: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-0000afa0: 2062 6f6f 6c20 616c 6c6f 775f 7361 6d65   bool allow_same
-0000afb0: 5f66 6561 7475 7265 5f64 696d 3a0a 2020  _feature_dim:.  
-0000afc0: 2020 2020 2020 3a70 6172 616d 2062 6f6f        :param boo
-0000afd0: 6c7c 4e6f 6e65 2061 6c6c 6f77 5f73 616d  l|None allow_sam
-0000afe0: 655f 7370 6174 6961 6c5f 6469 6d3a 0a20  e_spatial_dim:. 
-0000aff0: 2020 2020 2020 203a 7061 7261 6d20 626f         :param bo
-0000b000: 6f6c 2074 7265 6174 5f66 6561 7475 7265  ol treat_feature
-0000b010: 5f61 735f 7370 6174 6961 6c3a 0a20 2020  _as_spatial:.   
-0000b020: 2020 2020 203a 7061 7261 6d20 626f 6f6c       :param bool
-0000b030: 2062 726f 6164 6361 7374 5f6d 6174 6368   broadcast_match
-0000b040: 6573 3a0a 2020 2020 2020 2020 3a70 6172  es:.        :par
-0000b050: 616d 2062 6f6f 6c20 756e 6b6e 6f77 6e5f  am bool unknown_
-0000b060: 7370 6174 6961 6c5f 6d61 7463 6865 733a  spatial_matches:
-0000b070: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000b080: 626f 6f6c 2075 6e64 6566 696e 6564 5f6d  bool undefined_m
-0000b090: 6174 6368 6573 3a0a 2020 2020 2020 2020  atches:.        
-0000b0a0: 3a70 6172 616d 2062 6f6f 6c20 6465 7269  :param bool deri
-0000b0b0: 7665 645f 6d61 7463 6865 733a 0a20 2020  ved_matches:.   
-0000b0c0: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-0000b0d0: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
-0000b0e0: 2020 2020 2020 6672 6f6d 2072 6574 7572        from retur
-0000b0f0: 6e6e 2e75 7469 6c20 696d 706f 7274 2042  nn.util import B
-0000b100: 6568 6176 696f 7256 6572 7369 6f6e 0a0a  ehaviorVersion..
-0000b110: 2020 2020 2020 2020 6966 2073 656c 6620          if self 
-0000b120: 6973 206f 7468 6572 3a20 2023 2066 6972  is other:  # fir
-0000b130: 7374 2073 6f6d 6520 6661 7374 2070 6174  st some fast pat
-0000b140: 6820 6368 6563 6b0a 2020 2020 2020 2020  h check.        
-0000b150: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
-0000b160: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000b170: 7370 6563 6961 6c20 6f72 206f 7468 6572  special or other
-0000b180: 2e73 7065 6369 616c 3a0a 2020 2020 2020  .special:.      
-0000b190: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0000b1a0: 7365 2020 2320 6f6e 6c79 2074 7275 6520  se  # only true 
-0000b1b0: 6966 2073 616d 6520 696e 7374 616e 6365  if same instance
-0000b1c0: 2c20 6368 6563 6b20 6162 6f76 650a 2020  , check above.  
-0000b1d0: 2020 2020 2020 6966 2061 6c6c 6f77 5f73        if allow_s
-0000b1e0: 616d 655f 7370 6174 6961 6c5f 6469 6d20  ame_spatial_dim 
-0000b1f0: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-0000b200: 2020 2020 2061 6c6c 6f77 5f73 616d 655f       allow_same_
-0000b210: 7370 6174 6961 6c5f 6469 6d20 3d20 616c  spatial_dim = al
-0000b220: 6c6f 775f 7361 6d65 5f66 6561 7475 7265  low_same_feature
-0000b230: 5f64 696d 0a20 2020 2020 2020 2073 656c  _dim.        sel
-0000b240: 665f 6261 7365 203d 2073 656c 662e 6765  f_base = self.ge
-0000b250: 745f 7361 6d65 5f64 6572 6976 6564 5f62  t_same_derived_b
-0000b260: 6173 6528 7361 6d65 5f64 696d 3d54 7275  ase(same_dim=Tru
-0000b270: 6529 2069 6620 6465 7269 7665 645f 6d61  e) if derived_ma
-0000b280: 7463 6865 7320 656c 7365 2073 656c 662e  tches else self.
-0000b290: 6765 745f 7361 6d65 5f62 6173 6528 290a  get_same_base().
-0000b2a0: 2020 2020 2020 2020 6f74 6865 725f 6261          other_ba
-0000b2b0: 7365 203d 206f 7468 6572 2e67 6574 5f73  se = other.get_s
-0000b2c0: 616d 655f 6465 7269 7665 645f 6261 7365  ame_derived_base
-0000b2d0: 2873 616d 655f 6469 6d3d 5472 7565 2920  (same_dim=True) 
-0000b2e0: 6966 2064 6572 6976 6564 5f6d 6174 6368  if derived_match
-0000b2f0: 6573 2065 6c73 6520 6f74 6865 722e 6765  es else other.ge
-0000b300: 745f 7361 6d65 5f62 6173 6528 290a 2020  t_same_base().  
-0000b310: 2020 2020 2020 6966 2073 656c 665f 6261        if self_ba
-0000b320: 7365 2069 7320 6f74 6865 725f 6261 7365  se is other_base
-0000b330: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000b340: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-0000b350: 2020 6966 2073 656c 665f 6261 7365 2e64    if self_base.d
-0000b360: 6572 6976 6564 5f66 726f 6d5f 6f70 2061  erived_from_op a
-0000b370: 6e64 206f 7468 6572 5f62 6173 652e 6465  nd other_base.de
-0000b380: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
-0000b390: 2020 2020 2020 2020 2020 2069 6620 7365             if se
-0000b3a0: 6c66 5f62 6173 652e 6465 7269 7665 645f  lf_base.derived_
-0000b3b0: 6672 6f6d 5f6f 7020 3d3d 206f 7468 6572  from_op == other
-0000b3c0: 5f62 6173 652e 6465 7269 7665 645f 6672  _base.derived_fr
-0000b3d0: 6f6d 5f6f 703a 0a20 2020 2020 2020 2020  om_op:.         
-0000b3e0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0000b3f0: 7565 0a20 2020 2020 2020 2073 656c 665f  ue.        self_
-0000b400: 6b69 6e64 203d 2073 656c 662e 6b69 6e64  kind = self.kind
-0000b410: 0a20 2020 2020 2020 206f 7468 6572 5f6b  .        other_k
-0000b420: 696e 6420 3d20 6f74 6865 722e 6b69 6e64  ind = other.kind
-0000b430: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000b440: 5f6b 696e 6420 3d3d 206f 7468 6572 5f6b  _kind == other_k
-0000b450: 696e 6420 3d3d 2044 696d 5479 7065 732e  ind == DimTypes.
-0000b460: 4665 6174 7572 6520 616e 6420 6967 6e6f  Feature and igno
-0000b470: 7265 5f66 6561 7475 7265 5f64 696d 3a0a  re_feature_dim:.
-0000b480: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000b490: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-0000b4a0: 6966 2074 7265 6174 5f66 6561 7475 7265  if treat_feature
-0000b4b0: 5f61 735f 7370 6174 6961 6c3a 0a20 2020  _as_spatial:.   
-0000b4c0: 2020 2020 2020 2020 2023 204e 6f74 653a           # Note:
-0000b4d0: 204e 6f20 6b69 6e64 2061 7420 616c 6c3a   No kind at all:
-0000b4e0: 2052 6569 6e74 6572 7072 6574 2074 7265   Reinterpret tre
-0000b4f0: 6174 5f66 6561 7475 7265 5f61 735f 7370  at_feature_as_sp
-0000b500: 6174 6961 6c20 6120 6269 743a 0a20 2020  atial a bit:.   
-0000b510: 2020 2020 2020 2020 2023 2041 7373 756d           # Assum
-0000b520: 6520 7468 6174 2077 6520 7761 6e74 2074  e that we want t
-0000b530: 6865 6d20 616c 6c20 746f 2062 6520 6861  hem all to be ha
-0000b540: 6e64 6c65 6420 7468 6520 7361 6d65 2c20  ndled the same, 
-0000b550: 6e6f 206d 6174 7465 7220 7468 6520 6b69  no matter the ki
-0000b560: 6e64 2e0a 2020 2020 2020 2020 2020 2020  nd..            
-0000b570: 2320 2845 7863 6570 7420 6f66 2062 6174  # (Except of bat
-0000b580: 6368 2064 696d 206b 696e 642c 2077 6869  ch dim kind, whi
-0000b590: 6368 2069 7320 7374 696c 6c20 6578 636c  ch is still excl
-0000b5a0: 7564 6564 2068 6572 652e 290a 2020 2020  uded here.).    
-0000b5b0: 2020 2020 2020 2020 6966 2073 656c 665f          if self_
-0000b5c0: 6b69 6e64 203d 3d20 4469 6d54 7970 6573  kind == DimTypes
-0000b5d0: 2e46 6561 7475 7265 206f 7220 6e6f 7420  .Feature or not 
-0000b5e0: 7365 6c66 5f6b 696e 643a 0a20 2020 2020  self_kind:.     
-0000b5f0: 2020 2020 2020 2020 2020 2073 656c 665f             self_
-0000b600: 6b69 6e64 203d 2044 696d 5479 7065 732e  kind = DimTypes.
-0000b610: 5370 6174 6961 6c0a 2020 2020 2020 2020  Spatial.        
-0000b620: 2020 2020 6966 206f 7468 6572 5f6b 696e      if other_kin
-0000b630: 6420 3d3d 2044 696d 5479 7065 732e 4665  d == DimTypes.Fe
-0000b640: 6174 7572 6520 6f72 206e 6f74 206f 7468  ature or not oth
-0000b650: 6572 5f6b 696e 643a 0a20 2020 2020 2020  er_kind:.       
-0000b660: 2020 2020 2020 2020 206f 7468 6572 5f6b           other_k
-0000b670: 696e 6420 3d20 4469 6d54 7970 6573 2e53  ind = DimTypes.S
-0000b680: 7061 7469 616c 0a20 2020 2020 2020 2069  patial.        i
-0000b690: 6620 7365 6c66 2e64 696d 656e 7369 6f6e  f self.dimension
-0000b6a0: 2021 3d20 6f74 6865 722e 6469 6d65 6e73   != other.dimens
-0000b6b0: 696f 6e3a 0a20 2020 2020 2020 2020 2020  ion:.           
-0000b6c0: 2069 6620 6272 6f61 6463 6173 745f 6d61   if broadcast_ma
-0000b6d0: 7463 6865 7320 616e 6420 2873 656c 662e  tches and (self.
-0000b6e0: 6469 6d65 6e73 696f 6e20 3d3d 2031 206f  dimension == 1 o
-0000b6f0: 7220 6f74 6865 722e 6469 6d65 6e73 696f  r other.dimensio
-0000b700: 6e20 3d3d 2031 293a 0a20 2020 2020 2020  n == 1):.       
-0000b710: 2020 2020 2020 2020 2070 6173 7320 2023           pass  #
-0000b720: 2070 6173 7320 6f6e 0a20 2020 2020 2020   pass on.       
-0000b730: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
-0000b740: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000b750: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
-0000b760: 6966 2073 656c 665f 6b69 6e64 2021 3d20  if self_kind != 
-0000b770: 6f74 6865 725f 6b69 6e64 3a0a 2020 2020  other_kind:.    
-0000b780: 2020 2020 2020 2020 7265 7475 726e 2046          return F
-0000b790: 616c 7365 0a20 2020 2020 2020 2069 6620  alse.        if 
-0000b7a0: 7365 6c66 5f6b 696e 6420 3d3d 206f 7468  self_kind == oth
-0000b7b0: 6572 5f6b 696e 6420 3d3d 2044 696d 5479  er_kind == DimTy
-0000b7c0: 7065 732e 4261 7463 683a 0a20 2020 2020  pes.Batch:.     
-0000b7d0: 2020 2020 2020 2023 204e 6f74 653a 2054         # Note: T
-0000b7e0: 6869 7320 6d69 6768 7420 6265 2069 6e63  his might be inc
-0000b7f0: 6f72 7265 6374 2069 6e20 736f 6d65 2063  orrect in some c
-0000b800: 6173 6573 2c0a 2020 2020 2020 2020 2020  ases,.          
-0000b810: 2020 2320 652e 672e 2066 6f72 2062 6561    # e.g. for bea
-0000b820: 6d20 7365 6172 6368 2077 6865 6e20 7765  m search when we
-0000b830: 2068 6176 6520 7468 6520 6265 616d 2068   have the beam h
-0000b840: 6964 6465 6e20 696e 2074 6865 2062 6174  idden in the bat
-0000b850: 6368 2064 696d 2c0a 2020 2020 2020 2020  ch dim,.        
-0000b860: 2020 2020 2320 6f72 2077 6865 6e20 7765      # or when we
-0000b870: 2075 7365 6420 4d65 7267 6544 696d 734c   used MergeDimsL
-0000b880: 6179 6572 206f 6e20 7468 6520 6261 7463  ayer on the batc
-0000b890: 6820 6178 6973 2c20 6f72 2073 6f2e 0a20  h axis, or so.. 
-0000b8a0: 2020 2020 2020 2020 2020 2023 2057 6520             # We 
-0000b8b0: 6d69 6768 7420 6e65 6564 2074 6f20 6578  might need to ex
-0000b8c0: 7465 6e64 2074 6865 206c 6f67 6963 2068  tend the logic h
-0000b8d0: 6572 6520 6c61 7465 722e 0a20 2020 2020  ere later..     
-0000b8e0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-0000b8f0: 7565 0a20 2020 2020 2020 2069 6620 4265  ue.        if Be
-0000b900: 6861 7669 6f72 5665 7273 696f 6e2e 6765  haviorVersion.ge
-0000b910: 7428 2920 3e3d 2031 363a 0a20 2020 2020  t() >= 16:.     
-0000b920: 2020 2020 2020 2023 2045 6974 6865 7220         # Either 
-0000b930: 7365 6c66 206f 7220 6f74 6865 7220 6973  self or other is
-0000b940: 2073 6f6d 6520 6469 6d20 7461 6720 6578   some dim tag ex
-0000b950: 706c 6963 6974 6c79 2063 7265 6174 6564  plicitly created
-0000b960: 2062 7920 7468 6520 7573 6572 2c0a 2020   by the user,.  
-0000b970: 2020 2020 2020 2020 2020 2320 616e 6420            # and 
-0000b980: 7468 6579 2061 7265 206e 6f74 2074 6865  they are not the
-0000b990: 2073 616d 652c 2073 6f20 7765 206e 6576   same, so we nev
-0000b9a0: 6572 2074 7265 6174 2074 6865 6d20 6173  er treat them as
-0000b9b0: 2065 7175 616c 2e0a 2020 2020 2020 2020   equal..        
-0000b9c0: 2020 2020 6966 206e 6f74 2073 656c 662e      if not self.
-0000b9d0: 6175 746f 5f67 656e 6572 6174 6564 206f  auto_generated o
-0000b9e0: 7220 6e6f 7420 6f74 6865 722e 6175 746f  r not other.auto
-0000b9f0: 5f67 656e 6572 6174 6564 3a0a 2020 2020  _generated:.    
-0000ba00: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-0000ba10: 726f 6164 6361 7374 5f6d 6174 6368 6573  roadcast_matches
-0000ba20: 2061 6e64 2028 0a20 2020 2020 2020 2020   and (.         
-0000ba30: 2020 2020 2020 2020 2020 2028 7365 6c66             (self
-0000ba40: 2e64 696d 656e 7369 6f6e 203d 3d20 3120  .dimension == 1 
-0000ba50: 616e 6420 7365 6c66 2e61 7574 6f5f 6765  and self.auto_ge
-0000ba60: 6e65 7261 7465 6429 206f 7220 286f 7468  nerated) or (oth
-0000ba70: 6572 2e64 696d 656e 7369 6f6e 203d 3d20  er.dimension == 
-0000ba80: 3120 616e 6420 6f74 6865 722e 6175 746f  1 and other.auto
-0000ba90: 5f67 656e 6572 6174 6564 290a 2020 2020  _generated).    
-0000baa0: 2020 2020 2020 2020 2020 2020 293a 0a20              ):. 
-0000bab0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bac0: 2020 2070 6173 7320 2023 2065 7863 6570     pass  # excep
-0000bad0: 7469 6f6e 2c20 616c 6c6f 7720 6272 6f61  tion, allow broa
-0000bae0: 6463 6173 7420 6c6f 6769 630a 2020 2020  dcast logic.    
-0000baf0: 2020 2020 2020 2020 2020 2020 656c 7365              else
-0000bb00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000bb10: 2020 2020 2020 7265 7475 726e 2046 616c        return Fal
-0000bb20: 7365 0a20 2020 2020 2020 2069 6620 7365  se.        if se
-0000bb30: 6c66 5f6b 696e 6420 3d3d 206f 7468 6572  lf_kind == other
-0000bb40: 5f6b 696e 6420 3d3d 2044 696d 5479 7065  _kind == DimType
-0000bb50: 732e 4665 6174 7572 653a 0a20 2020 2020  s.Feature:.     
-0000bb60: 2020 2020 2020 2069 6620 616c 6c6f 775f         if allow_
-0000bb70: 7361 6d65 5f66 6561 7475 7265 5f64 696d  same_feature_dim
-0000bb80: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000bb90: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
-0000bba0: 2020 2020 2020 6966 2073 656c 665f 6b69        if self_ki
-0000bbb0: 6e64 203d 3d20 6f74 6865 725f 6b69 6e64  nd == other_kind
-0000bbc0: 203d 3d20 4469 6d54 7970 6573 2e53 7061   == DimTypes.Spa
-0000bbd0: 7469 616c 3a0a 2020 2020 2020 2020 2020  tial:.          
-0000bbe0: 2020 6966 2061 6c6c 6f77 5f73 616d 655f    if allow_same_
-0000bbf0: 7370 6174 6961 6c5f 6469 6d3a 0a20 2020  spatial_dim:.   
-0000bc00: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000bc10: 7365 6c66 2e64 696d 656e 7369 6f6e 2069  self.dimension i
-0000bc20: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-0000bc30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000bc40: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-0000bc50: 2020 2020 2020 2020 2020 2020 6966 2062              if b
-0000bc60: 726f 6164 6361 7374 5f6d 6174 6368 6573  roadcast_matches
-0000bc70: 2061 6e64 2028 7365 6c66 2e64 696d 656e   and (self.dimen
-0000bc80: 7369 6f6e 203d 3d20 3120 6f72 206f 7468  sion == 1 or oth
-0000bc90: 6572 2e64 696d 656e 7369 6f6e 203d 3d20  er.dimension == 
-0000bca0: 3129 3a0a 2020 2020 2020 2020 2020 2020  1):.            
-0000bcb0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
-0000bcc0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
-0000bcd0: 6966 2075 6e6b 6e6f 776e 5f73 7061 7469  if unknown_spati
-0000bce0: 616c 5f6d 6174 6368 6573 2061 6e64 2028  al_matches and (
-0000bcf0: 2873 656c 662e 6479 6e5f 7369 7a65 2069  (self.dyn_size i
-0000bd00: 7320 4e6f 6e65 2920 6f72 2028 6f74 6865  s None) or (othe
-0000bd10: 722e 6479 6e5f 7369 7a65 2069 7320 4e6f  r.dyn_size is No
-0000bd20: 6e65 2929 3a0a 2020 2020 2020 2020 2020  ne)):.          
-0000bd30: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
-0000bd40: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
-0000bd50: 2075 6e64 6566 696e 6564 5f6d 6174 6368   undefined_match
-0000bd60: 6573 2061 6e64 2028 7365 6c66 2e75 6e64  es and (self.und
-0000bd70: 6566 696e 6564 206f 7220 6f74 6865 722e  efined or other.
-0000bd80: 756e 6465 6669 6e65 6429 3a0a 2020 2020  undefined):.    
-0000bd90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000bda0: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-0000bdb0: 2320 496e 2070 7269 6e63 6970 6c65 2c20  # In principle, 
-0000bdc0: 7765 2077 6f75 6c64 2077 616e 7420 746f  we would want to
-0000bdd0: 2063 6865 636b 2066 6f72 2069 6465 6e74   check for ident
-0000bde0: 6974 7920 2873 656c 6620 6973 206f 7468  ity (self is oth
-0000bdf0: 6572 292e 0a20 2020 2020 2020 2023 2057  er)..        # W
-0000be00: 6520 6375 7272 656e 746c 7920 7573 6520  e currently use 
-0000be10: 7468 6520 6465 7363 7269 7074 696f 6e20  the description 
-0000be20: 6265 6361 7573 6520 7468 6520 6964 656e  because the iden
-0000be30: 7469 7479 2077 6f75 6c64 206e 6f74 2062  tity would not b
-0000be40: 6520 7468 6520 7361 6d65 0a20 2020 2020  e the same.     
-0000be50: 2020 2023 2069 6e20 6361 7365 206f 6620     # in case of 
-0000be60: 7465 6d70 6c61 7465 2063 6f6e 7374 7275  template constru
-0000be70: 6374 696f 6e20 7768 6572 6520 6120 6469  ction where a di
-0000be80: 6d20 7461 6720 6973 206f 6e63 6520 6372  m tag is once cr
-0000be90: 6561 7465 6420 666f 7220 6120 7465 6d70  eated for a temp
-0000bea0: 6c61 7465 206c 6179 6572 2c0a 2020 2020  late layer,.    
-0000beb0: 2020 2020 2320 616e 6420 7468 656e 206c      # and then l
-0000bec0: 6174 6572 2061 6761 696e 2066 6f72 2074  ater again for t
-0000bed0: 6865 2072 6561 6c20 6c61 7965 722e 0a20  he real layer.. 
-0000bee0: 2020 2020 2020 2069 6620 7365 6c66 2e61         if self.a
-0000bef0: 7574 6f5f 6765 6e65 7261 7465 6420 616e  uto_generated an
-0000bf00: 6420 6f74 6865 722e 6175 746f 5f67 656e  d other.auto_gen
-0000bf10: 6572 6174 6564 2061 6e64 2073 656c 662e  erated and self.
-0000bf20: 6465 7363 7269 7074 696f 6e20 3d3d 206f  description == o
-0000bf30: 7468 6572 2e64 6573 6372 6970 7469 6f6e  ther.description
-0000bf40: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-0000bf50: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
-0000bf60: 2020 7265 7475 726e 2046 616c 7365 0a0a    return False..
-0000bf70: 2020 2020 6465 6620 5f5f 6571 5f5f 2873      def __eq__(s
-0000bf80: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
-0000bf90: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000bfa0: 203a 7061 7261 6d20 4469 6d20 6f74 6865   :param Dim othe
-0000bfb0: 723a 0a20 2020 2020 2020 203a 7274 7970  r:.        :rtyp
-0000bfc0: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
-0000bfd0: 3a72 6574 7572 6e3a 203a 6675 6e63 3a60  :return: :func:`
-0000bfe0: 6973 5f65 7175 616c 6020 7769 7468 2064  is_equal` with d
-0000bff0: 6566 6175 6c74 206f 7074 696f 6e73 0a20  efault options. 
-0000c000: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000c010: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-0000c020: 616e 6365 286f 7468 6572 2c20 5f64 2e44  ance(other, _d.D
-0000c030: 696d 293a 0a20 2020 2020 2020 2020 2020  im):.           
-0000c040: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-0000c050: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
-0000c060: 662e 6973 5f65 7175 616c 286f 7468 6572  f.is_equal(other
-0000c070: 290a 0a20 2020 2064 6566 205f 5f6e 655f  )..    def __ne_
-0000c080: 5f28 7365 6c66 3a20 4469 6d2c 206f 7468  _(self: Dim, oth
-0000c090: 6572 3a20 4469 6d29 3a0a 2020 2020 2020  er: Dim):.      
-0000c0a0: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
-0000c0b0: 6172 616d 2044 696d 206f 7468 6572 3a0a  aram Dim other:.
-0000c0c0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-0000c0d0: 626f 6f6c 0a20 2020 2020 2020 2022 2222  bool.        """
-0000c0e0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-0000c0f0: 6e6f 7420 2873 656c 6620 3d3d 206f 7468  not (self == oth
-0000c100: 6572 290a 0a20 2020 2064 6566 205f 5f68  er)..    def __h
-0000c110: 6173 685f 5f28 7365 6c66 293a 0a20 2020  ash__(self):.   
-0000c120: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000c130: 203a 7274 7970 653a 2069 6e74 0a20 2020   :rtype: int.   
-0000c140: 2020 2020 203a 7265 7475 726e 3a20 6861       :return: ha
-0000c150: 7368 2c20 6d61 7463 6869 6e67 2074 6f20  sh, matching to 
-0000c160: 3a66 756e 633a 605f 5f65 715f 5f60 0a20  :func:`__eq__`. 
-0000c170: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000c180: 2020 2023 2054 6869 7320 6d75 7374 206d     # This must m
-0000c190: 6174 6368 2074 6865 2062 6568 6176 696f  atch the behavio
-0000c1a0: 7220 696e 205f 5f65 715f 5f2c 2077 6869  r in __eq__, whi
-0000c1b0: 6368 2069 7320 6973 5f65 7175 616c 2077  ch is is_equal w
-0000c1c0: 6974 6820 6465 6661 756c 7420 6f70 7469  ith default opti
-0000c1d0: 6f6e 732e 0a20 2020 2020 2020 2023 2049  ons..        # I
-0000c1e0: 2e65 2e20 6469 6666 6572 656e 7420 6861  .e. different ha
-0000c1f0: 7368 2069 6d70 6c69 6573 206e 6f74 2065  sh implies not e
-0000c200: 7175 616c 2028 6275 7420 7361 6d65 2068  qual (but same h
-0000c210: 6173 6820 6e6f 7420 6e65 6365 7373 6172  ash not necessar
-0000c220: 696c 7920 6571 7561 6c29 2e0a 2020 2020  ily equal)..    
-0000c230: 2020 2020 6966 2073 656c 662e 7370 6563      if self.spec
-0000c240: 6961 6c3a 0a20 2020 2020 2020 2020 2020  ial:.           
-0000c250: 2072 6574 7572 6e20 6861 7368 2869 6428   return hash(id(
-0000c260: 7365 6c66 2929 0a20 2020 2020 2020 2069  self)).        i
-0000c270: 6620 7365 6c66 2e69 735f 6261 7463 685f  f self.is_batch_
-0000c280: 6469 6d28 293a 0a20 2020 2020 2020 2020  dim():.         
-0000c290: 2020 2072 6574 7572 6e20 6861 7368 2828     return hash((
-0000c2a0: 2929 0a20 2020 2020 2020 2077 6974 6820  )).        with 
-0000c2b0: 7574 696c 2e67 7561 7264 5f69 6e66 696e  util.guard_infin
-0000c2c0: 6974 655f 7265 6375 7273 696f 6e28 5f64  ite_recursion(_d
-0000c2d0: 2e44 696d 2e5f 5f68 6173 685f 5f2c 2073  .Dim.__hash__, s
-0000c2e0: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
-0000c2f0: 2020 6261 7365 203d 2073 656c 662e 6765    base = self.ge
-0000c300: 745f 7361 6d65 5f62 6173 6528 290a 2020  t_same_base().  
-0000c310: 2020 2020 2020 2020 2020 6966 2062 6173            if bas
-0000c320: 6520 6973 206e 6f74 2073 656c 663a 0a20  e is not self:. 
-0000c330: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-0000c340: 6574 7572 6e20 6861 7368 2862 6173 6529  eturn hash(base)
-0000c350: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-0000c360: 7365 6c66 2e64 6572 6976 6564 5f66 726f  self.derived_fro
-0000c370: 6d5f 6f70 3a0a 2020 2020 2020 2020 2020  m_op:.          
-0000c380: 2020 2020 2020 7265 7475 726e 2068 6173        return has
-0000c390: 6828 7365 6c66 2e64 6572 6976 6564 5f66  h(self.derived_f
-0000c3a0: 726f 6d5f 6f70 290a 2020 2020 2020 2020  rom_op).        
-0000c3b0: 2020 2020 6966 2073 656c 662e 6175 746f      if self.auto
-0000c3c0: 5f67 656e 6572 6174 6564 3a0a 2020 2020  _generated:.    
-0000c3d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000c3e0: 726e 2068 6173 6828 2862 6173 652e 6b69  rn hash((base.ki
-0000c3f0: 6e64 2c20 6261 7365 2e64 696d 656e 7369  nd, base.dimensi
-0000c400: 6f6e 2c20 6261 7365 2e64 6573 6372 6970  on, base.descrip
-0000c410: 7469 6f6e 2929 0a20 2020 2020 2020 2020  tion)).         
-0000c420: 2020 2072 6574 7572 6e20 6861 7368 2869     return hash(i
-0000c430: 6428 6261 7365 2929 0a0a 2020 2020 6465  d(base))..    de
-0000c440: 6620 5f5f 6c74 5f5f 2873 656c 663a 2044  f __lt__(self: D
-0000c450: 696d 2c20 6f74 6865 723a 2044 696d 293a  im, other: Dim):
-0000c460: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000c470: 2020 2020 2044 6566 696e 6520 736f 6d65       Define some
-0000c480: 206f 7264 6572 2e20 5468 6973 2069 7320   order. This is 
-0000c490: 6a75 7374 2073 7563 6820 7468 6174 2060  just such that `
-0000c4a0: 736f 7274 6564 6020 776f 726b 732c 206f  sorted` works, o
-0000c4b0: 7220 736f 6d65 2064 6966 6620 7265 706f  r some diff repo
-0000c4c0: 7274 696e 672c 206f 7220 736f 2e0a 2020  rting, or so..  
-0000c4d0: 2020 2020 2020 4974 2069 7320 6f6e 2073        It is on s
-0000c4e0: 796d 626f 6c69 6320 6c65 7665 6c2c 2069  ymbolic level, i
-0000c4f0: 2e65 2e20 6974 2064 6f65 7320 6e6f 7420  .e. it does not 
-0000c500: 636f 6e73 6964 6572 2074 6865 2061 6374  consider the act
-0000c510: 7561 6c20 6469 6d65 6e73 696f 6e20 7661  ual dimension va
-0000c520: 6c75 652e 0a20 2020 2020 2020 2054 6865  lue..        The
-0000c530: 2064 6566 696e 6564 206f 7264 6572 2073   defined order s
-0000c540: 6f6d 6577 6861 7420 6172 6269 7472 6172  omewhat arbitrar
-0000c550: 792c 2073 6f20 646f 206e 6f74 2072 656c  y, so do not rel
-0000c560: 7920 6f6e 2074 6865 2065 7861 6374 2062  y on the exact b
-0000c570: 6568 6176 696f 722c 0a20 2020 2020 2020  ehavior,.       
-0000c580: 2061 7320 7468 6973 206d 6967 6874 2063   as this might c
-0000c590: 6861 6e67 6520 6174 2073 6f6d 6520 6c61  hange at some la
-0000c5a0: 7465 7220 706f 696e 742e 0a20 2020 2020  ter point..     
-0000c5b0: 2020 2043 7572 7265 6e74 6c79 2c20 6974     Currently, it
-0000c5c0: 2064 6570 656e 6473 206f 6e20 7468 6520   depends on the 
-0000c5d0: 6372 6561 7469 6f6e 2069 6e64 6578 2e0a  creation index..
-0000c5e0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-0000c5f0: 4469 6d20 6f74 6865 723a 0a20 2020 2020  Dim other:.     
-0000c600: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
-0000c610: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-0000c620: 2020 2020 6966 206e 6f74 2069 7369 6e73      if not isins
-0000c630: 7461 6e63 6528 6f74 6865 722c 2028 5f64  tance(other, (_d
-0000c640: 2e44 696d 2c20 5f6d 2e4d 6172 6b65 6444  .Dim, _m.MarkedD
-0000c650: 696d 2929 3a0a 2020 2020 2020 2020 2020  im)):.          
-0000c660: 2020 7261 6973 6520 5479 7065 4572 726f    raise TypeErro
-0000c670: 7228 2263 616e 6e6f 7420 636f 6d70 6172  r("cannot compar
-0000c680: 6520 2572 2077 6974 6820 2572 2220 2520  e %r with %r" % 
-0000c690: 2873 656c 662c 206f 7468 6572 2929 0a20  (self, other)). 
-0000c6a0: 2020 2020 2020 2069 6620 7365 6c66 203d         if self =
-0000c6b0: 3d20 6f74 6865 723a 0a20 2020 2020 2020  = other:.       
-0000c6c0: 2020 2020 2072 6574 7572 6e20 4661 6c73       return Fals
-0000c6d0: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
-0000c6e0: 2064 696d 5f63 6d70 5f76 616c 7565 2873   dim_cmp_value(s
-0000c6f0: 656c 6629 203c 2064 696d 5f63 6d70 5f76  elf) < dim_cmp_v
-0000c700: 616c 7565 286f 7468 6572 290a 0a20 2020  alue(other)..   
-0000c710: 2064 6566 205f 5f67 745f 5f28 7365 6c66   def __gt__(self
-0000c720: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-0000c730: 2020 2222 220a 2020 2020 2020 2020 5365    """.        Se
-0000c740: 6520 3a66 756e 633a 605f 5f6c 745f 5f60  e :func:`__lt__`
-0000c750: 2e0a 0a20 2020 2020 2020 203a 7061 7261  ...        :para
-0000c760: 6d20 4469 6d20 6f74 6865 723a 0a20 2020  m Dim other:.   
-0000c770: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-0000c780: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
-0000c790: 2020 2020 2020 7265 7475 726e 206f 7468        return oth
-0000c7a0: 6572 203c 2073 656c 660a 0a20 2020 2064  er < self..    d
-0000c7b0: 6566 205f 5f67 655f 5f28 7365 6c66 2c20  ef __ge__(self, 
-0000c7c0: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
-0000c7d0: 7265 7475 726e 206e 6f74 2073 656c 6620  return not self 
-0000c7e0: 3c20 6f74 6865 720a 0a20 2020 2064 6566  < other..    def
-0000c7f0: 205f 5f6c 655f 5f28 7365 6c66 2c20 6f74   __le__(self, ot
-0000c800: 6865 7229 3a0a 2020 2020 2020 2020 7265  her):.        re
-0000c810: 7475 726e 206e 6f74 2073 656c 6620 3e20  turn not self > 
-0000c820: 6f74 6865 720a 0a20 2020 2064 6566 2067  other..    def g
-0000c830: 6574 5f73 616d 655f 6261 7365 2873 656c  et_same_base(sel
-0000c840: 663a 205f 642e 4469 6d29 202d 3e20 5f64  f: _d.Dim) -> _d
-0000c850: 2e44 696d 3a0a 2020 2020 2020 2020 2222  .Dim:.        ""
-0000c860: 220a 2020 2020 2020 2020 3a72 6574 7572  ".        :retur
-0000c870: 6e3a 2073 616d 6520 6261 7365 0a20 2020  n: same base.   
-0000c880: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-0000c890: 2069 6620 6e6f 7420 7365 6c66 2e5f 6578   if not self._ex
-0000c8a0: 7472 613a 0a20 2020 2020 2020 2020 2020  tra:.           
-0000c8b0: 2072 6574 7572 6e20 7365 6c66 0a20 2020   return self.   
-0000c8c0: 2020 2020 2062 6173 6520 3d20 7365 6c66       base = self
-0000c8d0: 0a20 2020 2020 2020 2077 6869 6c65 2062  .        while b
-0000c8e0: 6173 652e 7361 6d65 5f61 733a 0a20 2020  ase.same_as:.   
-0000c8f0: 2020 2020 2020 2020 2062 6173 6520 3d20           base = 
-0000c900: 6261 7365 2e73 616d 655f 6173 0a20 2020  base.same_as.   
-0000c910: 2020 2020 2072 6574 7572 6e20 6261 7365       return base
-0000c920: 0a0a 2020 2020 6465 6620 6765 745f 7361  ..    def get_sa
-0000c930: 6d65 5f64 6572 6976 6564 5f62 6173 6528  me_derived_base(
-0000c940: 7365 6c66 3a20 5f64 2e44 696d 2c20 2a2c  self: _d.Dim, *,
-0000c950: 2073 616d 655f 6469 6d3a 2062 6f6f 6c20   same_dim: bool 
-0000c960: 3d20 4661 6c73 6529 202d 3e20 5f64 2e44  = False) -> _d.D
-0000c970: 696d 3a0a 2020 2020 2020 2020 2222 220a  im:.        """.
-0000c980: 2020 2020 2020 2020 3a70 6172 616d 2073          :param s
-0000c990: 616d 655f 6469 6d3a 2069 6620 5472 7565  ame_dim: if True
-0000c9a0: 2c20 7265 7475 726e 2074 6865 206c 6173  , return the las
-0000c9b0: 7420 6261 7365 2077 6869 6368 2068 6173  t base which has
-0000c9c0: 2074 6865 2073 616d 6520 6469 6d65 6e73   the same dimens
-0000c9d0: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
-0000c9e0: 2054 6865 2064 6572 6976 6564 2062 6173   The derived bas
-0000c9f0: 6520 6d69 6768 7420 6861 7665 2061 2064  e might have a d
-0000ca00: 6966 6665 7265 6e74 2064 696d 656e 7369  ifferent dimensi
-0000ca10: 6f6e 2e0a 2020 2020 2020 2020 2020 2020  on..            
-0000ca20: 496e 2063 6173 6520 6974 2069 7320 6479  In case it is dy
-0000ca30: 6e61 6d69 632c 2074 6865 2064 696d 656e  namic, the dimen
-0000ca40: 7369 6f6e 2069 7320 4e6f 6e65 2c20 736f  sion is None, so
-0000ca50: 2069 7420 6973 2061 6c77 6179 7320 7468   it is always th
-0000ca60: 6520 7361 6d65 2e0a 2020 2020 2020 2020  e same..        
-0000ca70: 2020 2020 496e 2063 6173 6520 6974 2069      In case it i
-0000ca80: 7320 7374 6174 6963 2c20 7468 6572 6520  s static, there 
-0000ca90: 6d69 6768 7420 6265 2061 2064 6966 6665  might be a diffe
-0000caa0: 7265 6e74 2064 696d 656e 7369 6f6e 2e0a  rent dimension..
-0000cab0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-0000cac0: 2073 616d 6520 6261 7365 2c20 6275 7420   same base, but 
-0000cad0: 616c 736f 2063 6f6e 7369 6465 7220 6465  also consider de
-0000cae0: 7269 7665 645f 6672 6f6d 5f2e 2e2e 0a20  rived_from_.... 
-0000caf0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000cb00: 2020 206c 6173 745f 6261 7365 5f73 656c     last_base_sel
-0000cb10: 665f 6469 6d20 3d20 7365 6c66 0a20 2020  f_dim = self.   
-0000cb20: 2020 2020 2062 6173 6520 3d20 7365 6c66       base = self
-0000cb30: 0a20 2020 2020 2020 2076 6973 6974 6564  .        visited
-0000cb40: 203d 207b 7d0a 2020 2020 2020 2020 7768   = {}.        wh
-0000cb50: 696c 6520 6261 7365 2e73 616d 655f 6173  ile base.same_as
-0000cb60: 206f 7220 6261 7365 2e64 6572 6976 6564   or base.derived
-0000cb70: 5f66 726f 6d5f 7461 673a 0a20 2020 2020  _from_tag:.     
-0000cb80: 2020 2020 2020 2061 7373 6572 7420 6964         assert id
-0000cb90: 2862 6173 6529 206e 6f74 2069 6e20 7669  (base) not in vi
-0000cba0: 7369 7465 6420 2023 2073 686f 756c 6420  sited  # should 
-0000cbb0: 6e6f 7420 6861 7665 2063 7963 6c65 732e  not have cycles.
-0000cbc0: 206e 6f72 6d61 6c6c 7920 7468 6973 2073   normally this s
-0000cbd0: 686f 756c 6420 6e65 7665 7220 6265 2074  hould never be t
-0000cbe0: 7269 6767 6572 6564 0a20 2020 2020 2020  riggered.       
-0000cbf0: 2020 2020 2076 6973 6974 6564 5b69 6428       visited[id(
-0000cc00: 6261 7365 295d 203d 2062 6173 650a 2020  base)] = base.  
-0000cc10: 2020 2020 2020 2020 2020 6966 2062 6173            if bas
-0000cc20: 652e 7361 6d65 5f61 733a 0a20 2020 2020  e.same_as:.     
-0000cc30: 2020 2020 2020 2020 2020 2062 6173 6520             base 
-0000cc40: 3d20 6261 7365 2e73 616d 655f 6173 0a20  = base.same_as. 
-0000cc50: 2020 2020 2020 2020 2020 2020 2020 2063                 c
-0000cc60: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
-0000cc70: 2020 2020 6261 7365 203d 2062 6173 652e      base = base.
-0000cc80: 6465 7269 7665 645f 6672 6f6d 5f74 6167  derived_from_tag
-0000cc90: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-0000cca0: 6572 7420 6261 7365 0a20 2020 2020 2020  ert base.       
-0000ccb0: 2020 2020 2069 6620 6261 7365 2e64 696d       if base.dim
-0000ccc0: 656e 7369 6f6e 203d 3d20 7365 6c66 2e64  ension == self.d
-0000ccd0: 696d 656e 7369 6f6e 3a0a 2020 2020 2020  imension:.      
-0000cce0: 2020 2020 2020 2020 2020 6c61 7374 5f62            last_b
-0000ccf0: 6173 655f 7365 6c66 5f64 696d 203d 2062  ase_self_dim = b
-0000cd00: 6173 650a 2020 2020 2020 2020 7265 7475  ase.        retu
-0000cd10: 726e 206c 6173 745f 6261 7365 5f73 656c  rn last_base_sel
-0000cd20: 665f 6469 6d20 6966 2073 616d 655f 6469  f_dim if same_di
-0000cd30: 6d20 656c 7365 2062 6173 650a 0a20 2020  m else base..   
-0000cd40: 2064 6566 2067 6574 5f64 6572 6976 6564   def get_derived
-0000cd50: 5f62 6173 6573 5f73 6574 2873 656c 6629  _bases_set(self)
-0000cd60: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000cd70: 2020 2020 2020 3a72 7479 7065 3a20 7365        :rtype: se
-0000cd80: 745b 4469 6d5d 0a20 2020 2020 2020 2022  t[Dim].        "
-0000cd90: 2222 0a20 2020 2020 2020 2072 6573 203d  "".        res =
-0000cda0: 2073 6574 2829 0a20 2020 2020 2020 2071   set().        q
-0000cdb0: 7565 7565 203d 205b 7365 6c66 5d0a 2020  ueue = [self].  
-0000cdc0: 2020 2020 2020 7669 7369 7465 6420 3d20        visited = 
-0000cdd0: 7b7d 2020 2320 7479 7065 3a20 4469 6374  {}  # type: Dict
-0000cde0: 5b69 6e74 2c5f 642e 4469 6d5d 2020 2320  [int,_d.Dim]  # 
-0000cdf0: 6279 2069 640a 2020 2020 2020 2020 7768  by id.        wh
-0000ce00: 696c 6520 7175 6575 653a 0a20 2020 2020  ile queue:.     
-0000ce10: 2020 2020 2020 2062 6173 6520 3d20 7175         base = qu
-0000ce20: 6575 652e 706f 7028 2d31 290a 2020 2020  eue.pop(-1).    
-0000ce30: 2020 2020 2020 2020 6966 2062 6173 652e          if base.
-0000ce40: 7361 6d65 5f61 733a 0a20 2020 2020 2020  same_as:.       
-0000ce50: 2020 2020 2020 2020 2062 6173 6520 3d20           base = 
-0000ce60: 6261 7365 2e73 616d 655f 6173 0a20 2020  base.same_as.   
-0000ce70: 2020 2020 2020 2020 2069 6620 6964 2862           if id(b
-0000ce80: 6173 6529 2069 6e20 7669 7369 7465 643a  ase) in visited:
-0000ce90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000cea0: 2063 6f6e 7469 6e75 650a 2020 2020 2020   continue.      
-0000ceb0: 2020 2020 2020 7669 7369 7465 645b 6964        visited[id
-0000cec0: 2862 6173 6529 5d20 3d20 6261 7365 0a20  (base)] = base. 
-0000ced0: 2020 2020 2020 2020 2020 2072 6573 2e61             res.a
-0000cee0: 6464 2862 6173 6529 0a20 2020 2020 2020  dd(base).       
-0000cef0: 2020 2020 2069 6620 6261 7365 2e64 6572       if base.der
-0000cf00: 6976 6564 5f66 726f 6d5f 6f70 3a0a 2020  ived_from_op:.  
-0000cf10: 2020 2020 2020 2020 2020 2020 2020 7175                qu
-0000cf20: 6575 652e 6578 7465 6e64 2862 6173 652e  eue.extend(base.
-0000cf30: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
-0000cf40: 696e 7075 7473 290a 2020 2020 2020 2020  inputs).        
-0000cf50: 2020 2020 656c 6966 2062 6173 652e 6465      elif base.de
-0000cf60: 7269 7665 645f 6672 6f6d 5f74 6167 3a0a  rived_from_tag:.
-0000cf70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000cf80: 7175 6575 652e 6170 7065 6e64 2862 6173  queue.append(bas
-0000cf90: 652e 6465 7269 7665 645f 6672 6f6d 5f74  e.derived_from_t
-0000cfa0: 6167 290a 2020 2020 2020 2020 7265 7475  ag).        retu
-0000cfb0: 726e 2072 6573 0a0a 2020 2020 4070 726f  rn res..    @pro
-0000cfc0: 7065 7274 790a 2020 2020 6465 6620 756e  perty.    def un
-0000cfd0: 6465 6669 6e65 6428 7365 6c66 3a20 5f64  defined(self: _d
-0000cfe0: 2e44 696d 2920 2d3e 2062 6f6f 6c3a 0a20  .Dim) -> bool:. 
-0000cff0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000d000: 2020 203a 7265 7475 726e 3a20 7768 6574     :return: whet
-0000d010: 6865 7220 7468 6520 756e 6465 6669 6e65  her the undefine
-0000d020: 6420 666c 6167 2069 7320 7365 742c 2069  d flag is set, i
-0000d030: 6e20 7365 6c66 2c20 6261 7365 732c 206f  n self, bases, o
-0000d040: 7220 616e 7920 6465 7269 7665 6420 6261  r any derived ba
-0000d050: 7365 732e 2061 6c73 6f20 7365 6520 3a66  ses. also see :f
-0000d060: 756e 633a 6069 735f 6469 6d5f 6b6e 6f77  unc:`is_dim_know
-0000d070: 6e60 0a20 2020 2020 2020 2022 2222 0a20  n`.        """. 
-0000d080: 2020 2020 2020 2062 6173 6520 3d20 7365         base = se
-0000d090: 6c66 0a20 2020 2020 2020 2076 6973 6974  lf.        visit
-0000d0a0: 6564 203d 207b 7d0a 2020 2020 2020 2020  ed = {}.        
-0000d0b0: 7768 696c 6520 6261 7365 2e73 616d 655f  while base.same_
-0000d0c0: 6173 206f 7220 6261 7365 2e64 6572 6976  as or base.deriv
-0000d0d0: 6564 5f66 726f 6d5f 7461 673a 0a20 2020  ed_from_tag:.   
-0000d0e0: 2020 2020 2020 2020 2061 7373 6572 7420           assert 
-0000d0f0: 6964 2862 6173 6529 206e 6f74 2069 6e20  id(base) not in 
-0000d100: 7669 7369 7465 6420 2023 2073 686f 756c  visited  # shoul
-0000d110: 6420 6e6f 7420 6861 7665 2063 7963 6c65  d not have cycle
-0000d120: 732e 206e 6f72 6d61 6c6c 7920 7468 6973  s. normally this
-0000d130: 2073 686f 756c 6420 6e65 7665 7220 6265   should never be
-0000d140: 2074 7269 6767 6572 6564 0a20 2020 2020   triggered.     
-0000d150: 2020 2020 2020 2076 6973 6974 6564 5b69         visited[i
-0000d160: 6428 6261 7365 295d 203d 2062 6173 650a  d(base)] = base.
-0000d170: 2020 2020 2020 2020 2020 2020 2320 6e6f              # no
-0000d180: 696e 7370 6563 7469 6f6e 2050 7950 726f  inspection PyPro
-0000d190: 7465 6374 6564 4d65 6d62 6572 0a20 2020  tectedMember.   
-0000d1a0: 2020 2020 2020 2020 2069 6620 6261 7365           if base
-0000d1b0: 2e5f 6578 7472 6120 616e 6420 6261 7365  ._extra and base
-0000d1c0: 2e5f 6578 7472 612e 756e 6465 6669 6e65  ._extra.undefine
-0000d1d0: 643a 0a20 2020 2020 2020 2020 2020 2020  d:.             
-0000d1e0: 2020 2072 6574 7572 6e20 5472 7565 0a20     return True. 
-0000d1f0: 2020 2020 2020 2020 2020 2069 6620 6261             if ba
-0000d200: 7365 2e73 616d 655f 6173 3a0a 2020 2020  se.same_as:.    
-0000d210: 2020 2020 2020 2020 2020 2020 6261 7365              base
-0000d220: 203d 2062 6173 652e 7361 6d65 5f61 730a   = base.same_as.
-0000d230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000d240: 636f 6e74 696e 7565 0a20 2020 2020 2020  continue.       
-0000d250: 2020 2020 2062 6173 6520 3d20 6261 7365       base = base
-0000d260: 2e64 6572 6976 6564 5f66 726f 6d5f 7461  .derived_from_ta
-0000d270: 670a 2020 2020 2020 2020 2020 2020 6173  g.            as
-0000d280: 7365 7274 2062 6173 650a 2020 2020 2020  sert base.      
-0000d290: 2020 2320 6e6f 696e 7370 6563 7469 6f6e    # noinspection
-0000d2a0: 2050 7950 726f 7465 6374 6564 4d65 6d62   PyProtectedMemb
-0000d2b0: 6572 0a20 2020 2020 2020 2072 6574 7572  er.        retur
-0000d2c0: 6e20 6261 7365 2e5f 6578 7472 6120 616e  n base._extra an
-0000d2d0: 6420 6261 7365 2e5f 6578 7472 612e 756e  d base._extra.un
-0000d2e0: 6465 6669 6e65 640a 0a20 2020 2064 6566  defined..    def
-0000d2f0: 2064 6563 6c61 7265 5f73 616d 655f 6173   declare_same_as
-0000d300: 2873 656c 663a 205f 642e 4469 6d2c 206f  (self: _d.Dim, o
-0000d310: 7468 6572 3a20 5f64 2e44 696d 293a 0a20  ther: _d.Dim):. 
-0000d320: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-0000d330: 2020 203a 7061 7261 6d20 6f74 6865 723a     :param other:
-0000d340: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-0000d350: 2020 2020 2061 7373 6572 7420 7365 6c66       assert self
-0000d360: 2e63 616e 5f62 655f 7573 6564 5f61 735f  .can_be_used_as_
-0000d370: 6469 6d28 2920 616e 6420 6f74 6865 722e  dim() and other.
-0000d380: 6361 6e5f 6265 5f75 7365 645f 6173 5f64  can_be_used_as_d
-0000d390: 696d 2829 2020 2320 6465 636c 6172 655f  im()  # declare_
-0000d3a0: 7361 6d65 5f61 7320 646f 6573 206e 6f74  same_as does not
-0000d3b0: 206d 616b 6520 7365 6e73 6520 6f74 6865   make sense othe
-0000d3c0: 7277 6973 650a 2020 2020 2020 2020 2320  rwise.        # 
-0000d3d0: 4e6f 7465 3a20 4368 6563 6b20 6069 7360  Note: Check `is`
-0000d3e0: 2c20 6e6f 7420 603d 3d60 2e20 603d 3d60  , not `==`. `==`
-0000d3f0: 2063 616e 2062 6520 7472 7565 2065 7665   can be true eve
-0000d400: 6e20 7468 6f75 6768 2073 616d 655f 6173  n though same_as
-0000d410: 2061 7265 206e 6f74 2074 6865 2073 616d   are not the sam
-0000d420: 6520 696e 7374 616e 6365 2c0a 2020 2020  e instance,.    
-0000d430: 2020 2020 2320 652e 672e 2076 6961 2061      # e.g. via a
-0000d440: 7574 6f5f 6765 6e65 7261 7465 642e 0a20  uto_generated.. 
-0000d450: 2020 2020 2020 2069 6620 7365 6c66 2069         if self i
-0000d460: 7320 6f74 6865 723a 0a20 2020 2020 2020  s other:.       
-0000d470: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-0000d480: 2020 2020 7365 6c66 2e5f 6d61 7962 655f      self._maybe_
-0000d490: 7570 6461 7465 2829 0a20 2020 2020 2020  update().       
-0000d4a0: 2073 656c 662e 5f76 616c 6964 6174 655f   self._validate_
-0000d4b0: 696e 5f63 7572 7265 6e74 5f67 7261 7068  in_current_graph
-0000d4c0: 2829 0a20 2020 2020 2020 206f 7468 6572  ().        other
-0000d4d0: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
-0000d4e0: 7272 656e 745f 6772 6170 6828 290a 2020  rrent_graph().  
-0000d4f0: 2020 2020 2020 6f74 6865 725f 7361 6d65        other_same
-0000d500: 5f62 6173 6520 3d20 6f74 6865 722e 6765  _base = other.ge
-0000d510: 745f 7361 6d65 5f62 6173 6528 290a 2020  t_same_base().  
-0000d520: 2020 2020 2020 6966 2073 656c 6620 6973        if self is
-0000d530: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000d540: 206f 7220 7365 6c66 2e73 616d 655f 6173   or self.same_as
-0000d550: 2069 7320 6f74 6865 725f 7361 6d65 5f62   is other_same_b
-0000d560: 6173 653a 0a20 2020 2020 2020 2020 2020  ase:.           
-0000d570: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-0000d580: 7365 6c66 5f73 616d 655f 6173 203d 2073  self_same_as = s
-0000d590: 656c 662e 6765 745f 7361 6d65 5f62 6173  elf.get_same_bas
-0000d5a0: 6528 290a 2020 2020 2020 2020 6966 2073  e().        if s
-0000d5b0: 656c 665f 7361 6d65 5f61 7320 6973 206f  elf_same_as is o
-0000d5c0: 7468 6572 5f73 616d 655f 6261 7365 3a0a  ther_same_base:.
-0000d5d0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-0000d5e0: 726e 0a20 2020 2020 2020 2069 6620 6f74  rn.        if ot
-0000d5f0: 6865 725f 7361 6d65 5f62 6173 652e 6765  her_same_base.ge
-0000d600: 745f 7361 6d65 5f64 6572 6976 6564 5f62  t_same_derived_b
-0000d610: 6173 6528 2920 6973 2073 656c 665f 7361  ase() is self_sa
-0000d620: 6d65 5f61 733a 0a20 2020 2020 2020 2020  me_as:.         
-0000d630: 2020 2023 2057 6520 6163 7475 616c 6c79     # We actually
-0000d640: 2077 616e 7420 6974 2074 6f20 6265 2074   want it to be t
-0000d650: 6865 206f 7468 6572 2077 6179 2061 726f  he other way aro
-0000d660: 756e 642e 0a20 2020 2020 2020 2020 2020  und..           
-0000d670: 2077 6974 6820 7574 696c 2e67 7561 7264   with util.guard
-0000d680: 5f69 6e66 696e 6974 655f 7265 6375 7273  _infinite_recurs
-0000d690: 696f 6e28 5f64 2e44 696d 2e64 6563 6c61  ion(_d.Dim.decla
-0000d6a0: 7265 5f73 616d 655f 6173 2c20 6f74 6865  re_same_as, othe
-0000d6b0: 722c 2073 656c 6629 3a0a 2020 2020 2020  r, self):.      
-0000d6c0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000d6d0: 206f 7468 6572 2e64 6563 6c61 7265 5f73   other.declare_s
-0000d6e0: 616d 655f 6173 2873 656c 6629 0a20 2020  ame_as(self).   
-0000d6f0: 2020 2020 2069 6620 7365 6c66 2e62 6174       if self.bat
-0000d700: 6368 3a0a 2020 2020 2020 2020 2020 2020  ch:.            
-0000d710: 2320 4966 2073 656c 6620 6973 2064 6566  # If self is def
-0000d720: 696e 6564 2028 7365 6c66 2e69 735f 6469  ined (self.is_di
-0000d730: 6d5f 6b6e 6f77 6e29 2c20 6265 2066 6169  m_known), be fai
-0000d740: 7220 746f 206f 7468 6572 2c20 616e 6420  r to other, and 
-0000d750: 6164 6170 7420 6974 2074 6f20 7468 6520  adapt it to the 
-0000d760: 7269 6768 7420 6261 7463 682c 0a20 2020  right batch,.   
-0000d770: 2020 2020 2020 2020 2023 2073 7563 6820           # such 
-0000d780: 7468 6174 206f 7468 6572 2e69 735f 6469  that other.is_di
-0000d790: 6d5f 6b6e 6f77 6e20 6973 2063 6f72 7265  m_known is corre
-0000d7a0: 6374 2c20 6279 2070 6f74 656e 7469 616c  ct, by potential
-0000d7b0: 6c79 2063 6f6d 706c 6574 696e 6720 6974  ly completing it
-0000d7c0: 2e0a 2020 2020 2020 2020 2020 2020 6f74  ..            ot
-0000d7d0: 6865 725f 203d 206f 7468 6572 2e67 6574  her_ = other.get
-0000d7e0: 5f66 6f72 5f62 6174 6368 5f63 7478 2873  _for_batch_ctx(s
-0000d7f0: 656c 662e 6261 7463 682c 2063 7478 3d73  elf.batch, ctx=s
-0000d800: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
-0000d810: 5f63 7478 290a 2020 2020 2020 2020 656c  _ctx).        el
-0000d820: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-0000d830: 6f74 6865 725f 203d 206f 7468 6572 0a20  other_ = other. 
-0000d840: 2020 2020 2020 2069 6620 280a 2020 2020         if (.    
-0000d850: 2020 2020 2020 2020 2873 656c 662e 6973          (self.is
-0000d860: 5f64 696d 5f6b 6e6f 776e 2829 2061 6e64  _dim_known() and
-0000d870: 206e 6f74 206f 7468 6572 5f2e 6973 5f64   not other_.is_d
-0000d880: 696d 5f6b 6e6f 776e 2829 290a 2020 2020  im_known()).    
-0000d890: 2020 2020 2020 2020 6f72 0a20 2020 2020          or.     
-0000d8a0: 2020 2020 2020 2023 204c 696b 6520 6973         # Like is
-0000d8b0: 5f64 696d 5f6b 6e6f 776e 2062 7574 2066  _dim_known but f
-0000d8c0: 6f72 2073 7461 7469 6320 6469 6d73 2c20  or static dims, 
-0000d8d0: 7765 206d 6967 6874 206b 6e6f 7720 626f  we might know bo
-0000d8e0: 7468 2c0a 2020 2020 2020 2020 2020 2020  th,.            
-0000d8f0: 2320 6275 7420 7468 6520 6465 7269 7665  # but the derive
-0000d900: 645f 6672 6f6d 5f6f 7020 7374 696c 6c20  d_from_op still 
-0000d910: 776f 756c 6420 7072 6f76 6964 6520 6d6f  would provide mo
-0000d920: 7265 2069 6e66 6f72 6d61 7469 6f6e 2e0a  re information..
-0000d930: 2020 2020 2020 2020 2020 2020 280a 2020              (.  
-0000d940: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000d950: 6c66 5f73 616d 655f 6173 2e64 6572 6976  lf_same_as.deriv
-0000d960: 6564 5f66 726f 6d5f 6f70 0a20 2020 2020  ed_from_op.     
-0000d970: 2020 2020 2020 2020 2020 2061 6e64 206e             and n
-0000d980: 6f74 206f 7468 6572 5f73 616d 655f 6261  ot other_same_ba
-0000d990: 7365 2e64 6572 6976 6564 5f66 726f 6d5f  se.derived_from_
-0000d9a0: 6f70 0a20 2020 2020 2020 2020 2020 2020  op.             
-0000d9b0: 2020 2061 6e64 206f 7468 6572 206e 6f74     and other not
-0000d9c0: 2069 6e20 7365 6c66 2e67 6574 5f64 6572   in self.get_der
-0000d9d0: 6976 6564 5f62 6173 6573 5f73 6574 2829  ived_bases_set()
-0000d9e0: 0a20 2020 2020 2020 2020 2020 2029 0a20  .            ). 
-0000d9f0: 2020 2020 2020 2020 2020 206f 7220 286e             or (n
-0000da00: 6f74 2073 656c 662e 756e 6465 6669 6e65  ot self.undefine
-0000da10: 6420 616e 6420 6f74 6865 725f 2e75 6e64  d and other_.und
-0000da20: 6566 696e 6564 290a 2020 2020 2020 2020  efined).        
-0000da30: 293a 0a20 2020 2020 2020 2020 2020 2077  ):.            w
-0000da40: 6974 6820 7574 696c 2e67 7561 7264 5f69  ith util.guard_i
-0000da50: 6e66 696e 6974 655f 7265 6375 7273 696f  nfinite_recursio
-0000da60: 6e28 5f64 2e44 696d 2e64 6563 6c61 7265  n(_d.Dim.declare
-0000da70: 5f73 616d 655f 6173 2c20 6f74 6865 722c  _same_as, other,
-0000da80: 2073 656c 6629 3a0a 2020 2020 2020 2020   self):.        
-0000da90: 2020 2020 2020 2020 7265 7475 726e 206f          return o
-0000daa0: 7468 6572 2e64 6563 6c61 7265 5f73 616d  ther.declare_sam
-0000dab0: 655f 6173 2873 656c 6629 0a20 2020 2020  e_as(self).     
-0000dac0: 2020 206f 7468 6572 5f64 6572 6976 6564     other_derived
-0000dad0: 5f62 6173 6573 203d 206f 7468 6572 2e67  _bases = other.g
-0000dae0: 6574 5f64 6572 6976 6564 5f62 6173 6573  et_derived_bases
-0000daf0: 5f73 6574 2829 0a20 2020 2020 2020 2073  _set().        s
-0000db00: 656c 665f 6465 7269 7665 645f 6261 7365  elf_derived_base
-0000db10: 7320 3d20 7365 6c66 2e67 6574 5f64 6572  s = self.get_der
-0000db20: 6976 6564 5f62 6173 6573 5f73 6574 2829  ived_bases_set()
-0000db30: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
-0000db40: 725f 6465 7269 7665 645f 6261 7365 7320  r_derived_bases 
-0000db50: 213d 2073 656c 665f 6465 7269 7665 645f  != self_derived_
-0000db60: 6261 7365 7320 616e 6420 7365 6c66 5f64  bases and self_d
-0000db70: 6572 6976 6564 5f62 6173 6573 2e69 7373  erived_bases.iss
-0000db80: 7562 7365 7428 6f74 6865 725f 6465 7269  ubset(other_deri
-0000db90: 7665 645f 6261 7365 7329 3a0a 2020 2020  ved_bases):.    
-0000dba0: 2020 2020 2020 2020 2320 4176 6f69 6420          # Avoid 
-0000dbb0: 6379 636c 6573 206f 6e20 6465 7269 7665  cycles on derive
-0000dbc0: 645f 6672 6f6d 5f74 6167 2e20 6874 7470  d_from_tag. http
-0000dbd0: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f72  s://github.com/r
-0000dbe0: 7774 682d 6936 2f72 6574 7572 6e6e 2f69  wth-i6/returnn/i
-0000dbf0: 7373 7565 732f 3130 3534 0a20 2020 2020  ssues/1054.     
-0000dc00: 2020 2020 2020 2077 6974 6820 7574 696c         with util
-0000dc10: 2e67 7561 7264 5f69 6e66 696e 6974 655f  .guard_infinite_
-0000dc20: 7265 6375 7273 696f 6e28 5f64 2e44 696d  recursion(_d.Dim
-0000dc30: 2e64 6563 6c61 7265 5f73 616d 655f 6173  .declare_same_as
-0000dc40: 2c20 6f74 6865 722c 2073 656c 6629 3a0a  , other, self):.
-0000dc50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000dc60: 7265 7475 726e 206f 7468 6572 2e64 6563  return other.dec
-0000dc70: 6c61 7265 5f73 616d 655f 6173 2873 656c  lare_same_as(sel
-0000dc80: 6629 0a20 2020 2020 2020 2069 6620 7365  f).        if se
-0000dc90: 6c66 2e5f 6578 7472 613a 0a20 2020 2020  lf._extra:.     
-0000dca0: 2020 2020 2020 2073 656c 662e 5f65 7874         self._ext
-0000dcb0: 7261 2e64 6572 6976 6564 5f66 726f 6d5f  ra.derived_from_
-0000dcc0: 6f70 203d 204e 6f6e 650a 2020 2020 2020  op = None.      
-0000dcd0: 2020 2020 2020 7365 6c66 2e5f 6578 7472        self._extr
-0000dce0: 612e 6465 7269 7665 645f 6672 6f6d 5f74  a.derived_from_t
-0000dcf0: 6167 203d 204e 6f6e 650a 2020 2020 2020  ag = None.      
-0000dd00: 2020 6966 2073 656c 665f 7361 6d65 5f61    if self_same_a
-0000dd10: 7320 6973 206e 6f74 2073 656c 663a 0a20  s is not self:. 
-0000dd20: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-0000dd30: 7420 6e6f 7420 7365 6c66 5f73 616d 655f  t not self_same_
-0000dd40: 6173 2e73 616d 655f 6173 0a20 2020 2020  as.same_as.     
-0000dd50: 2020 2020 2020 2069 6620 7365 6c66 5f73         if self_s
-0000dd60: 616d 655f 6173 2069 7320 6f74 6865 725f  ame_as is other_
-0000dd70: 7361 6d65 5f62 6173 653a 0a20 2020 2020  same_base:.     
-0000dd80: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-0000dd90: 6e0a 2020 2020 2020 2020 2020 2020 7769  n.            wi
-0000dda0: 7468 2075 7469 6c2e 6775 6172 645f 696e  th util.guard_in
-0000ddb0: 6669 6e69 7465 5f72 6563 7572 7369 6f6e  finite_recursion
-0000ddc0: 285f 642e 4469 6d2e 6465 636c 6172 655f  (_d.Dim.declare_
-0000ddd0: 7361 6d65 5f61 732c 2073 656c 665f 7361  same_as, self_sa
-0000dde0: 6d65 5f61 732c 206f 7468 6572 5f73 616d  me_as, other_sam
-0000ddf0: 655f 6261 7365 293a 0a20 2020 2020 2020  e_base):.       
-0000de00: 2020 2020 2020 2020 2073 656c 665f 7361           self_sa
-0000de10: 6d65 5f61 732e 6465 636c 6172 655f 7361  me_as.declare_sa
-0000de20: 6d65 5f61 7328 6f74 6865 725f 7361 6d65  me_as(other_same
-0000de30: 5f62 6173 6529 0a20 2020 2020 2020 2020  _base).         
-0000de40: 2020 2069 6620 2873 656c 662e 6479 6e5f     if (self.dyn_
-0000de50: 7369 7a65 5f65 7874 2069 7320 4e6f 6e65  size_ext is None
-0000de60: 206f 7220 6e6f 7420 7365 6c66 2e5f 7661   or not self._va
-0000de70: 6c69 6461 7465 5f69 6e5f 6375 7272 656e  lidate_in_curren
-0000de80: 745f 6772 6170 6828 2929 2061 6e64 2073  t_graph()) and s
-0000de90: 656c 665f 7361 6d65 5f61 732e 6479 6e5f  elf_same_as.dyn_
-0000dea0: 7369 7a65 5f65 7874 3a0a 2020 2020 2020  size_ext:.      
-0000deb0: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
-0000dec0: 796e 5f73 697a 655f 6578 7420 3d20 7365  yn_size_ext = se
-0000ded0: 6c66 5f73 616d 655f 6173 2e67 6574 5f64  lf_same_as.get_d
-0000dee0: 796e 5f73 697a 655f 6578 745f 666f 725f  yn_size_ext_for_
-0000def0: 6261 7463 685f 6374 7828 0a20 2020 2020  batch_ctx(.     
-0000df00: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000df10: 656c 662e 6261 7463 682c 2073 656c 662e  elf.batch, self.
-0000df20: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
-0000df30: 2c20 7465 6d70 6c61 7465 5f6f 6e6c 793d  , template_only=
-0000df40: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
-0000df50: 2020 2020 2029 0a20 2020 2020 2020 2065       ).        e
-0000df60: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000df70: 2069 6620 7365 6c66 2e5f 6578 7472 613a   if self._extra:
-0000df80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000df90: 2066 6f72 2064 696d 5f20 696e 2073 656c   for dim_ in sel
-0000dfa0: 662e 5f65 7874 7261 2e73 616d 655f 666f  f._extra.same_fo
-0000dfb0: 725f 6261 7463 685f 6374 782e 7661 6c75  r_batch_ctx.valu
-0000dfc0: 6573 2829 3a0a 2020 2020 2020 2020 2020  es():.          
-0000dfd0: 2020 2020 2020 2020 2020 2320 6e6f 696e            # noin
-0000dfe0: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
-0000dff0: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
-0000e000: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000e010: 6620 6469 6d5f 2e5f 6578 7472 613a 0a20  f dim_._extra:. 
-0000e020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e030: 2020 2020 2020 2023 206e 6f69 6e73 7065         # noinspe
-0000e040: 6374 696f 6e20 5079 5072 6f74 6563 7465  ction PyProtecte
-0000e050: 644d 656d 6265 720a 2020 2020 2020 2020  dMember.        
-0000e060: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e070: 6469 6d5f 2e5f 6578 7472 612e 6465 7269  dim_._extra.deri
-0000e080: 7665 645f 6672 6f6d 5f6f 7020 3d20 4e6f  ved_from_op = No
-0000e090: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
-0000e0a0: 2020 2020 2020 2020 2020 2023 206e 6f69             # noi
-0000e0b0: 6e73 7065 6374 696f 6e20 5079 5072 6f74  nspection PyProt
-0000e0c0: 6563 7465 644d 656d 6265 720a 2020 2020  ectedMember.    
-0000e0d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e0e0: 2020 2020 6469 6d5f 2e5f 6578 7472 612e      dim_._extra.
-0000e0f0: 6465 7269 7665 645f 6672 6f6d 5f74 6167  derived_from_tag
-0000e100: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000e110: 2320 4e6f 7720 6d65 7267 6520 6578 6973  # Now merge exis
-0000e120: 7469 6e67 2076 6172 6961 6e74 732e 2042  ting variants. B
-0000e130: 7574 206f 6e6c 7920 6966 206e 6f74 2064  ut only if not d
-0000e140: 6572 6976 6564 2076 6961 206f 702c 2062  erived via op, b
-0000e150: 6563 6175 7365 2069 6e20 7468 6174 2063  ecause in that c
-0000e160: 6173 652c 2077 6520 6361 6e20 2861 6e64  ase, we can (and
-0000e170: 2073 686f 756c 6421 290a 2020 2020 2020   should!).      
-0000e180: 2020 2320 6175 746f 6d61 7469 6361 6c6c    # automaticall
-0000e190: 7920 696e 6665 7220 6974 2e20 4e6f 7465  y infer it. Note
-0000e1a0: 2074 6861 7420 7765 206f 6e6c 7920 676f   that we only go
-0000e1b0: 7420 6865 7265 2077 6865 6e20 7468 6520  t here when the 
-0000e1c0: 6f74 6865 7220 6973 206e 6f74 2074 6865  other is not the
-0000e1d0: 2073 616d 6520 6469 6d2c 2073 6f20 6974   same dim, so it
-0000e1e0: 206d 6561 6e73 2074 6861 740a 2020 2020   means that.    
-0000e1f0: 2020 2020 2320 7468 6520 6f74 6865 7220      # the other 
-0000e200: 6973 2072 6561 6c6c 7920 6469 6666 6572  is really differ
-0000e210: 656e 742c 2074 6865 2073 697a 6573 2061  ent, the sizes a
-0000e220: 7265 2070 6f74 656e 7469 616c 6c79 2064  re potentially d
-0000e230: 6966 6665 7265 6e74 2c20 6275 7420 7765  ifferent, but we
-0000e240: 2077 616e 7420 746f 206f 7665 7274 616b   want to overtak
-0000e250: 6520 7468 6520 6f74 6865 722e 0a20 2020  e the other..   
-0000e260: 2020 2020 2069 6620 6f74 6865 725f 7361       if other_sa
-0000e270: 6d65 5f62 6173 652e 6465 7269 7665 645f  me_base.derived_
-0000e280: 6672 6f6d 5f6f 703a 0a20 2020 2020 2020  from_op:.       
-0000e290: 2020 2020 2023 2043 6c65 616e 7570 2065       # Cleanup e
-0000e2a0: 7665 7279 7468 696e 672c 2065 7370 2070  verything, esp p
-0000e2b0: 6f74 656e 7469 616c 2061 6c72 6561 6479  otential already
-0000e2c0: 2063 6f6d 7075 7465 6420 7369 7a65 732c   computed sizes,
-0000e2d0: 2061 7320 7468 6573 6520 6d69 6768 7420   as these might 
-0000e2e0: 6265 2069 6e76 616c 6964 2e0a 2020 2020  be invalid..    
-0000e2f0: 2020 2020 2020 2020 666f 7220 6469 6d5f          for dim_
-0000e300: 2069 6e20 5b73 656c 665f 7361 6d65 5f61   in [self_same_a
-0000e310: 732c 2073 656c 665d 202b 2028 6c69 7374  s, self] + (list
-0000e320: 2873 656c 662e 5f65 7874 7261 2e73 616d  (self._extra.sam
-0000e330: 655f 666f 725f 6261 7463 685f 6374 782e  e_for_batch_ctx.
-0000e340: 7661 6c75 6573 2829 2920 6966 2073 656c  values()) if sel
-0000e350: 662e 5f65 7874 7261 2065 6c73 6520 5b5d  f._extra else []
-0000e360: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000e370: 2020 2069 6620 6469 6d5f 2e64 796e 5f73     if dim_.dyn_s
-0000e380: 697a 655f 6578 743a 0a20 2020 2020 2020  ize_ext:.       
-0000e390: 2020 2020 2020 2020 2020 2020 2064 696d               dim
-0000e3a0: 5f2e 6479 6e5f 7369 7a65 5f65 7874 2e70  _.dyn_size_ext.p
-0000e3b0: 6c61 6365 686f 6c64 6572 203d 204e 6f6e  laceholder = Non
-0000e3c0: 650a 2020 2020 2020 2020 6f74 6865 725f  e.        other_
-0000e3d0: 7361 6d65 5f62 6173 652e 5f6d 6572 6765  same_base._merge
-0000e3e0: 5f73 616d 655f 666f 725f 6261 7463 685f  _same_for_batch_
-0000e3f0: 6374 785f 6469 6374 2873 656c 6629 0a20  ctx_dict(self). 
-0000e400: 2020 2020 2020 206f 7468 6572 2e5f 6d61         other._ma
-0000e410: 7962 655f 7570 6461 7465 2829 0a20 2020  ybe_update().   
-0000e420: 2020 2020 2073 656c 662e 7361 6d65 5f61       self.same_a
-0000e430: 7320 3d20 6f74 6865 725f 7361 6d65 5f62  s = other_same_b
-0000e440: 6173 650a 2020 2020 2020 2020 7365 6c66  ase.        self
-0000e450: 2e5f 6d61 7962 655f 7570 6461 7465 2829  ._maybe_update()
-0000e460: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
-0000e470: 2e64 796e 5f73 697a 6520 6973 206e 6f74  .dyn_size is not
-0000e480: 204e 6f6e 6520 616e 6420 6f74 6865 725f   None and other_
-0000e490: 7361 6d65 5f62 6173 652e 6479 6e5f 7369  same_base.dyn_si
-0000e4a0: 7a65 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ze is not None:.
-0000e4b0: 2020 2020 2020 2020 2020 2020 6966 2073              if s
-0000e4c0: 656c 662e 6479 6e5f 7369 7a65 2069 7320  elf.dyn_size is 
-0000e4d0: 6e6f 7420 6f74 6865 725f 7361 6d65 5f62  not other_same_b
-0000e4e0: 6173 652e 6479 6e5f 7369 7a65 3a0a 2020  ase.dyn_size:.  
-0000e4f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-0000e500: 2073 656c 662e 6261 7463 6820 3d3d 206f   self.batch == o
-0000e510: 7468 6572 5f73 616d 655f 6261 7365 2e62  ther_same_base.b
-0000e520: 6174 6368 2061 6e64 2073 656c 662e 636f  atch and self.co
-0000e530: 6e74 726f 6c5f 666c 6f77 5f63 7478 203d  ntrol_flow_ctx =
-0000e540: 3d20 6f74 6865 725f 7361 6d65 5f62 6173  = other_same_bas
-0000e550: 652e 636f 6e74 726f 6c5f 666c 6f77 5f63  e.control_flow_c
-0000e560: 7478 3a0a 2020 2020 2020 2020 2020 2020  tx:.            
-0000e570: 2020 2020 2020 2020 2320 4e6f 7465 3a20          # Note: 
-0000e580: 496e 7374 6561 6420 6f66 206d 616b 696e  Instead of makin
-0000e590: 6720 7468 6973 2061 2077 6172 6e69 6e67  g this a warning
-0000e5a0: 2c20 7765 2063 6f75 6c64 2061 6c73 6f20  , we could also 
-0000e5b0: 656e 666f 7263 6520 7468 6973 2061 7420  enforce this at 
-0000e5c0: 736f 6d65 2070 6f69 6e74 2e0a 2020 2020  some point..    
-0000e5d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e5e0: 2320 2020 5468 6520 7573 6572 2073 686f  #   The user sho
-0000e5f0: 756c 6420 6265 2061 626c 6520 746f 2066  uld be able to f
-0000e600: 6978 2060 6578 7465 726e 5f64 6174 6160  ix `extern_data`
-0000e610: 2069 6e20 7468 6520 636f 6e66 6967 0a20   in the config. 
-0000e620: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e630: 2020 2023 2020 2073 7563 6820 7468 6174     #   such that
-0000e640: 2074 6869 7320 6973 2063 6f72 7265 6374   this is correct
-0000e650: 2069 6e20 7468 6520 6669 7273 7420 706c   in the first pl
-0000e660: 6163 652e 0a20 2020 2020 2020 2020 2020  ace..           
-0000e670: 2020 2020 2020 2020 2023 2020 2041 6c73           #   Als
-0000e680: 6f2c 2069 6e20 6164 6469 7469 6f6e 2074  o, in addition t
-0000e690: 6f20 7468 6973 2077 6172 6e69 6e67 2c0a  o this warning,.
-0000e6a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e6b0: 2020 2020 2320 2020 7765 206d 6967 6874      #   we might
-0000e6c0: 2077 616e 7420 746f 2061 6464 2073 6f6d   want to add som
-0000e6d0: 6520 7275 6e74 696d 6520 6368 6563 6b20  e runtime check 
-0000e6e0: 6f6e 2074 6865 2065 7120 6f66 2074 6865  on the eq of the
-0000e6f0: 2064 796e 2073 697a 6573 2e0a 2020 2020   dyn sizes..    
-0000e700: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e710: 7072 696e 7428 0a20 2020 2020 2020 2020  print(.         
-0000e720: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-0000e730: 5761 726e 696e 673a 2061 7373 756d 696e  Warning: assumin
-0000e740: 6720 6469 6d20 7461 6773 2061 7265 2073  g dim tags are s
-0000e750: 616d 6520 7769 7468 2064 6966 6665 7265  ame with differe
-0000e760: 6e74 2073 697a 6520 706c 6163 6568 6f6c  nt size placehol
-0000e770: 6465 7273 3a20 2572 2076 7320 2572 220a  ders: %r vs %r".
-0000e780: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e790: 2020 2020 2020 2020 2520 2873 656c 662e          % (self.
-0000e7a0: 6479 6e5f 7369 7a65 2c20 6f74 6865 725f  dyn_size, other_
-0000e7b0: 7361 6d65 5f62 6173 652e 6479 6e5f 7369  same_base.dyn_si
-0000e7c0: 7a65 290a 2020 2020 2020 2020 2020 2020  ze).            
-0000e7d0: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000e7e0: 2020 2320 4966 2077 6520 6861 7665 2061    # If we have a
-0000e7f0: 2064 6566 696e 6564 2073 6f75 7263 652c   defined source,
-0000e800: 2061 6e64 2074 6869 7320 6973 2061 2064   and this is a d
-0000e810: 796e 616d 6963 2073 7061 7469 616c 2061  ynamic spatial a
-0000e820: 7869 732c 2061 6e64 2069 7420 7761 7320  xis, and it was 
-0000e830: 756e 6465 6669 6e65 6420 6265 666f 7265  undefined before
-0000e840: 2c0a 2020 2020 2020 2020 2320 6d61 7962  ,.        # mayb
-0000e850: 6520 7765 2063 616e 206f 7665 7274 616b  e we can overtak
-0000e860: 6520 7468 6520 7369 7a65 5f70 6c61 6365  e the size_place
-0000e870: 686f 6c64 6572 206e 6f77 2e0a 2020 2020  holder now..    
-0000e880: 2020 2020 6966 206f 7468 6572 5f73 616d      if other_sam
-0000e890: 655f 6261 7365 2e64 796e 5f73 697a 6520  e_base.dyn_size 
-0000e8a0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
-0000e8b0: 7365 6c66 2e5f 6578 7472 6120 616e 6420  self._extra and 
-0000e8c0: 7365 6c66 2e5f 6578 7472 612e 7372 635f  self._extra.src_
-0000e8d0: 6461 7461 3a0a 2020 2020 2020 2020 2020  data:.          
-0000e8e0: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
-0000e8f0: 6e63 6528 7365 6c66 2e5f 6578 7472 612e  nce(self._extra.
-0000e900: 7372 635f 6178 6973 2c20 696e 7429 0a20  src_axis, int). 
-0000e910: 2020 2020 2020 2020 2020 2023 204d 6179             # May
-0000e920: 6265 2069 7420 6368 616e 6765 6420 696e  be it changed in
-0000e930: 2074 6865 206d 6561 6e77 6869 6c65 2c20   the meanwhile, 
-0000e940: 736f 2063 6865 636b 2e0a 2020 2020 2020  so check..      
-0000e950: 2020 2020 2020 7461 6720 3d20 7365 6c66        tag = self
-0000e960: 2e5f 6578 7472 612e 7372 635f 6461 7461  ._extra.src_data
-0000e970: 2e67 6574 5f64 696d 5f74 6167 2873 656c  .get_dim_tag(sel
-0000e980: 662e 5f65 7874 7261 2e73 7263 5f61 7869  f._extra.src_axi
-0000e990: 7329 0a20 2020 2020 2020 2020 2020 2069  s).            i
-0000e9a0: 6620 7461 672e 6465 7363 7269 7074 696f  f tag.descriptio
-0000e9b0: 6e20 3d3d 2073 656c 662e 6465 7363 7269  n == self.descri
-0000e9c0: 7074 696f 6e20 616e 6420 286e 6f74 2074  ption and (not t
-0000e9d0: 6167 2e64 796e 5f73 697a 655f 6578 7420  ag.dyn_size_ext 
-0000e9e0: 6f72 206e 6f74 2074 6167 2e5f 7661 6c69  or not tag._vali
-0000e9f0: 6461 7465 5f69 6e5f 6375 7272 656e 745f  date_in_current_
-0000ea00: 6772 6170 6828 2929 3a0a 2020 2020 2020  graph()):.      
-0000ea10: 2020 2020 2020 2020 2020 7461 672e 6479            tag.dy
-0000ea20: 6e5f 7369 7a65 5f65 7874 203d 2073 656c  n_size_ext = sel
-0000ea30: 662e 6765 745f 6479 6e5f 7369 7a65 5f65  f.get_dyn_size_e
-0000ea40: 7874 5f66 6f72 5f62 6174 6368 5f63 7478  xt_for_batch_ctx
-0000ea50: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000ea60: 2020 2020 2020 7461 672e 6261 7463 682c        tag.batch,
-0000ea70: 2074 6167 2e63 6f6e 7472 6f6c 5f66 6c6f   tag.control_flo
-0000ea80: 775f 6374 782c 2074 656d 706c 6174 655f  w_ctx, template_
-0000ea90: 6f6e 6c79 3d54 7275 650a 2020 2020 2020  only=True.      
-0000eaa0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000eab0: 2020 2020 2020 2020 2020 2020 7461 672e              tag.
-0000eac0: 5f6d 6179 6265 5f75 7064 6174 6528 290a  _maybe_update().
-0000ead0: 2020 2020 2020 2020 2320 4966 206f 7468          # If oth
-0000eae0: 6572 7320 6479 6e5f 7369 7a65 2069 7320  ers dyn_size is 
-0000eaf0: 4e6f 6e65 2062 7574 2077 6520 6861 7665  None but we have
-0000eb00: 2061 2064 796e 5f73 697a 652c 206d 6179   a dyn_size, may
-0000eb10: 6265 2075 7064 6174 6520 6f74 6865 7273  be update others
-0000eb20: 2064 796e 5f73 697a 652e 0a20 2020 2020   dyn_size..     
-0000eb30: 2020 2069 6620 7365 6c66 2e64 796e 5f73     if self.dyn_s
-0000eb40: 697a 6520 6973 206e 6f74 204e 6f6e 6520  ize is not None 
-0000eb50: 616e 6420 6f74 6865 725f 7361 6d65 5f62  and other_same_b
-0000eb60: 6173 652e 6479 6e5f 7369 7a65 2069 7320  ase.dyn_size is 
-0000eb70: 6e6f 7420 7365 6c66 2e64 796e 5f73 697a  not self.dyn_siz
-0000eb80: 653a 0a20 2020 2020 2020 2020 2020 2023  e:.            #
-0000eb90: 2043 6f75 6c64 2062 6520 756e 7365 7420   Could be unset 
-0000eba0: 6966 2069 7420 636f 6d65 7320 6672 6f6d  if it comes from
-0000ebb0: 2074 6865 2063 6f6e 6669 672c 206f 7220   the config, or 
-0000ebc0: 6672 6f6d 2070 7265 7620 6772 6170 6820  from prev graph 
-0000ebd0: 6372 6561 7469 6f6e 2e0a 2020 2020 2020  creation..      
-0000ebe0: 2020 2020 2020 2320 5468 6973 2069 7320        # This is 
-0000ebf0: 696d 706f 7274 616e 7420 7375 6368 2074  important such t
-0000ec00: 6861 7420 7365 6c66 2e63 616e 5f63 6f6d  hat self.can_com
-0000ec10: 7061 7265 2829 2069 7320 7361 6e65 2e0a  pare() is sane..
-0000ec20: 2020 2020 2020 2020 2020 2020 6966 206f              if o
-0000ec30: 7468 6572 5f73 616d 655f 6261 7365 2e64  ther_same_base.d
-0000ec40: 796e 5f73 697a 6520 6973 204e 6f6e 6520  yn_size is None 
-0000ec50: 6f72 206e 6f74 206f 7468 6572 5f73 616d  or not other_sam
-0000ec60: 655f 6261 7365 2e5f 7661 6c69 6461 7465  e_base._validate
-0000ec70: 5f69 6e5f 6375 7272 656e 745f 6772 6170  _in_current_grap
-0000ec80: 6828 293a 0a20 2020 2020 2020 2020 2020  h():.           
-0000ec90: 2020 2020 206f 7468 6572 5f73 616d 655f       other_same_
-0000eca0: 6261 7365 2e64 796e 5f73 697a 655f 6578  base.dyn_size_ex
-0000ecb0: 7420 3d20 7365 6c66 2e67 6574 5f64 796e  t = self.get_dyn
-0000ecc0: 5f73 697a 655f 6578 745f 666f 725f 6261  _size_ext_for_ba
-0000ecd0: 7463 685f 6374 7828 0a20 2020 2020 2020  tch_ctx(.       
-0000ece0: 2020 2020 2020 2020 2020 2020 206f 7468               oth
-0000ecf0: 6572 5f73 616d 655f 6261 7365 2e62 6174  er_same_base.bat
-0000ed00: 6368 2c20 6f74 6865 725f 7361 6d65 5f62  ch, other_same_b
-0000ed10: 6173 652e 636f 6e74 726f 6c5f 666c 6f77  ase.control_flow
-0000ed20: 5f63 7478 2c20 7465 6d70 6c61 7465 5f6f  _ctx, template_o
-0000ed30: 6e6c 793d 5472 7565 0a20 2020 2020 2020  nly=True.       
-0000ed40: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-0000ed50: 2020 2020 2020 2020 2020 206f 7468 6572             other
-0000ed60: 5f73 616d 655f 6261 7365 2e5f 6d61 7962  _same_base._mayb
-0000ed70: 655f 7570 6461 7465 2829 0a20 2020 2020  e_update().     
-0000ed80: 2020 2069 6620 6e6f 7420 7365 6c66 2e64     if not self.d
-0000ed90: 796e 5f73 697a 655f 6578 7420 6f72 206e  yn_size_ext or n
-0000eda0: 6f74 2073 656c 662e 5f76 616c 6964 6174  ot self._validat
-0000edb0: 655f 696e 5f63 7572 7265 6e74 5f67 7261  e_in_current_gra
-0000edc0: 7068 2829 3a0a 2020 2020 2020 2020 2020  ph():.          
-0000edd0: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
-0000ede0: 6578 7420 3d20 6f74 6865 725f 7361 6d65  ext = other_same
-0000edf0: 5f62 6173 652e 6765 745f 6479 6e5f 7369  _base.get_dyn_si
-0000ee00: 7a65 5f65 7874 5f66 6f72 5f62 6174 6368  ze_ext_for_batch
-0000ee10: 5f63 7478 280a 2020 2020 2020 2020 2020  _ctx(.          
-0000ee20: 2020 2020 2020 7365 6c66 2e62 6174 6368        self.batch
-0000ee30: 2c20 7365 6c66 2e63 6f6e 7472 6f6c 5f66  , self.control_f
-0000ee40: 6c6f 775f 6374 782c 2074 656d 706c 6174  low_ctx, templat
-0000ee50: 655f 6f6e 6c79 3d54 7275 650a 2020 2020  e_only=True.    
-0000ee60: 2020 2020 2020 2020 290a 2020 2020 2020          ).      
-0000ee70: 2020 2020 2020 7365 6c66 2e5f 6d61 7962        self._mayb
-0000ee80: 655f 7570 6461 7465 2829 0a20 2020 2020  e_update().     
-0000ee90: 2020 2065 6c69 6620 6f74 6865 725f 7361     elif other_sa
-0000eea0: 6d65 5f62 6173 652e 6479 6e5f 7369 7a65  me_base.dyn_size
-0000eeb0: 5f65 7874 2069 7320 4e6f 6e65 206f 7220  _ext is None or 
-0000eec0: 6e6f 7420 6f74 6865 725f 7361 6d65 5f62  not other_same_b
-0000eed0: 6173 652e 5f76 616c 6964 6174 655f 696e  ase._validate_in
-0000eee0: 5f63 7572 7265 6e74 5f67 7261 7068 2829  _current_graph()
-0000eef0: 3a0a 2020 2020 2020 2020 2020 2020 6f74  :.            ot
-0000ef00: 6865 725f 7361 6d65 5f62 6173 652e 6479  her_same_base.dy
-0000ef10: 6e5f 7369 7a65 5f65 7874 203d 2073 656c  n_size_ext = sel
-0000ef20: 662e 6765 745f 6479 6e5f 7369 7a65 5f65  f.get_dyn_size_e
-0000ef30: 7874 5f66 6f72 5f62 6174 6368 5f63 7478  xt_for_batch_ctx
-0000ef40: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-0000ef50: 2020 6f74 6865 725f 7361 6d65 5f62 6173    other_same_bas
-0000ef60: 652e 6261 7463 682c 206f 7468 6572 5f73  e.batch, other_s
-0000ef70: 616d 655f 6261 7365 2e63 6f6e 7472 6f6c  ame_base.control
-0000ef80: 5f66 6c6f 775f 6374 782c 2074 656d 706c  _flow_ctx, templ
-0000ef90: 6174 655f 6f6e 6c79 3d54 7275 650a 2020  ate_only=True.  
-0000efa0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-0000efb0: 2020 2020 2020 2020 6f74 6865 725f 7361          other_sa
-0000efc0: 6d65 5f62 6173 652e 5f6d 6179 6265 5f75  me_base._maybe_u
-0000efd0: 7064 6174 6528 290a 2020 2020 2020 2020  pdate().        
-0000efe0: 6966 2073 656c 662e 6973 5f64 696d 5f6b  if self.is_dim_k
-0000eff0: 6e6f 776e 2829 2061 6e64 206f 7468 6572  nown() and other
-0000f000: 2e69 735f 6469 6d5f 6b6e 6f77 6e28 293a  .is_dim_known():
-0000f010: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
-0000f020: 6572 7420 7365 6c66 2e64 696d 656e 7369  ert self.dimensi
-0000f030: 6f6e 203d 3d20 6f74 6865 722e 6469 6d65  on == other.dime
-0000f040: 6e73 696f 6e0a 2020 2020 2020 2020 656c  nsion.        el
-0000f050: 6966 2073 656c 662e 6973 5f64 696d 5f6b  if self.is_dim_k
-0000f060: 6e6f 776e 2829 2061 6e64 206e 6f74 206f  nown() and not o
-0000f070: 7468 6572 2e69 735f 6469 6d5f 6b6e 6f77  ther.is_dim_know
-0000f080: 6e28 293a 0a20 2020 2020 2020 2020 2020  n():.           
-0000f090: 206f 7468 6572 2e63 6170 6163 6974 7920   other.capacity 
-0000f0a0: 3d20 7365 6c66 2e63 6170 6163 6974 790a  = self.capacity.
-0000f0b0: 2020 2020 2020 2020 2020 2020 6f74 6865              othe
-0000f0c0: 722e 7369 7a65 203d 2073 656c 662e 7369  r.size = self.si
-0000f0d0: 7a65 0a20 2020 2020 2020 2065 6c69 6620  ze.        elif 
-0000f0e0: 6e6f 7420 7365 6c66 2e69 735f 6469 6d5f  not self.is_dim_
-0000f0f0: 6b6e 6f77 6e28 2920 616e 6420 6f74 6865  known() and othe
-0000f100: 722e 6973 5f64 696d 5f6b 6e6f 776e 2829  r.is_dim_known()
-0000f110: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
-0000f120: 6c66 2e63 6170 6163 6974 7920 3d20 6f74  lf.capacity = ot
-0000f130: 6865 722e 6361 7061 6369 7479 0a20 2020  her.capacity.   
-0000f140: 2020 2020 2020 2020 2073 656c 662e 7369           self.si
-0000f150: 7a65 203d 206f 7468 6572 2e73 697a 650a  ze = other.size.
-0000f160: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-0000f170: 766f 6361 6220 616e 6420 6e6f 7420 6f74  vocab and not ot
-0000f180: 6865 725f 7361 6d65 5f62 6173 652e 766f  her_same_base.vo
-0000f190: 6361 623a 0a20 2020 2020 2020 2020 2020  cab:.           
-0000f1a0: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000f1b0: 2e76 6f63 6162 203d 2073 656c 662e 766f  .vocab = self.vo
-0000f1c0: 6361 620a 2020 2020 2020 2020 656c 6966  cab.        elif
-0000f1d0: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
-0000f1e0: 2e76 6f63 6162 2061 6e64 206e 6f74 2073  .vocab and not s
-0000f1f0: 656c 662e 766f 6361 623a 0a20 2020 2020  elf.vocab:.     
-0000f200: 2020 2020 2020 2073 656c 662e 766f 6361         self.voca
-0000f210: 6220 3d20 6f74 6865 725f 7361 6d65 5f62  b = other_same_b
-0000f220: 6173 652e 766f 6361 620a 2020 2020 2020  ase.vocab.      
-0000f230: 2020 7365 6c66 2e5f 6d61 6b65 5f65 7874    self._make_ext
-0000f240: 7261 2829 0a20 2020 2020 2020 2073 656c  ra().        sel
-0000f250: 665f 7361 6d65 5f61 732e 5f6d 616b 655f  f_same_as._make_
-0000f260: 6578 7472 6128 290a 2020 2020 2020 2020  extra().        
-0000f270: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
-0000f280: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
-0000f290: 0a20 2020 2020 2020 2073 656c 662e 5f65  .        self._e
-0000f2a0: 7874 7261 2e61 7574 6f5f 6765 6e65 7261  xtra.auto_genera
-0000f2b0: 7465 6420 3d20 7365 6c66 5f73 616d 655f  ted = self_same_
-0000f2c0: 6173 2e5f 6578 7472 612e 6175 746f 5f67  as._extra.auto_g
-0000f2d0: 656e 6572 6174 6564 203d 206f 7468 6572  enerated = other
-0000f2e0: 5f73 616d 655f 6261 7365 2e61 7574 6f5f  _same_base.auto_
-0000f2f0: 6765 6e65 7261 7465 640a 2020 2020 2020  generated.      
-0000f300: 2020 2320 5461 6b65 206f 7665 7220 6465    # Take over de
-0000f310: 7269 7665 645f 6672 6f6d 5f6f 702e 2048  rived_from_op. H
-0000f320: 6f77 6576 6572 2c20 6f6e 6c79 2069 6620  owever, only if 
-0000f330: 7468 6973 2077 6f75 6c64 206e 6f74 2069  this would not i
-0000f340: 6e74 726f 6475 6365 2063 7963 6c65 7321  ntroduce cycles!
-0000f350: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
-0000f360: 7365 6c66 5f64 6572 6976 6564 5f62 6173  self_derived_bas
-0000f370: 6573 2e69 7373 7570 6572 7365 7428 6f74  es.issuperset(ot
-0000f380: 6865 725f 6465 7269 7665 645f 6261 7365  her_derived_base
-0000f390: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-0000f3a0: 6966 2073 656c 662e 6465 7269 7665 645f  if self.derived_
-0000f3b0: 6672 6f6d 5f6f 7020 616e 6420 6e6f 7420  from_op and not 
-0000f3c0: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
-0000f3d0: 6465 7269 7665 645f 6672 6f6d 5f6f 703a  derived_from_op:
-0000f3e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f3f0: 2023 206e 6f69 6e73 7065 6374 696f 6e20   # noinspection 
-0000f400: 5079 5072 6f74 6563 7465 644d 656d 6265  PyProtectedMembe
-0000f410: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
-0000f420: 2020 6f74 6865 725f 7361 6d65 5f62 6173    other_same_bas
-0000f430: 652e 5f6d 616b 655f 6578 7472 6128 292e  e._make_extra().
-0000f440: 6465 7269 7665 645f 6672 6f6d 5f6f 7020  derived_from_op 
-0000f450: 3d20 7365 6c66 2e64 6572 6976 6564 5f66  = self.derived_f
-0000f460: 726f 6d5f 6f70 0a20 2020 2020 2020 2020  rom_op.         
-0000f470: 2020 2065 6c69 6620 6f74 6865 725f 7361     elif other_sa
-0000f480: 6d65 5f62 6173 652e 6465 7269 7665 645f  me_base.derived_
-0000f490: 6672 6f6d 5f6f 7020 616e 6420 6e6f 7420  from_op and not 
-0000f4a0: 7365 6c66 2e64 6572 6976 6564 5f66 726f  self.derived_fro
-0000f4b0: 6d5f 6f70 3a0a 2020 2020 2020 2020 2020  m_op:.          
-0000f4c0: 2020 2020 2020 7365 6c66 2e5f 6d61 6b65        self._make
-0000f4d0: 5f65 7874 7261 2829 2e64 6572 6976 6564  _extra().derived
-0000f4e0: 5f66 726f 6d5f 6f70 203d 206f 7468 6572  _from_op = other
-0000f4f0: 5f73 616d 655f 6261 7365 2e64 6572 6976  _same_base.deriv
-0000f500: 6564 5f66 726f 6d5f 6f70 0a20 2020 2020  ed_from_op.     
-0000f510: 2020 2069 6620 7365 6c66 2e5f 6578 7472     if self._extr
-0000f520: 6120 616e 6420 6e6f 7420 6f74 6865 725f  a and not other_
-0000f530: 7361 6d65 5f62 6173 652e 6973 5f64 796e  same_base.is_dyn
-0000f540: 616d 6963 2829 3a0a 2020 2020 2020 2020  amic():.        
-0000f550: 2020 2020 2320 5468 6f73 6520 6d69 6768      # Those migh
-0000f560: 7420 6265 2073 6574 2076 6961 2067 6574  t be set via get
-0000f570: 5f62 6174 6368 5f66 6f72 5f63 7478 2066  _batch_for_ctx f
-0000f580: 6f72 2061 6e20 756e 6465 6669 6e65 6420  or an undefined 
-0000f590: 6469 6d2c 0a20 2020 2020 2020 2020 2020  dim,.           
-0000f5a0: 2023 2077 6869 6368 206e 6f77 2062 6563   # which now bec
-0000f5b0: 6f6d 6573 2073 7461 7469 6320 6475 6520  omes static due 
-0000f5c0: 746f 2060 6f74 6865 7260 2e0a 2020 2020  to `other`..    
-0000f5d0: 2020 2020 2020 2020 7365 6c66 2e5f 6578          self._ex
-0000f5e0: 7472 612e 6261 7463 6820 3d20 4e6f 6e65  tra.batch = None
-0000f5f0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000f600: 662e 5f65 7874 7261 2e63 6f6e 7472 6f6c  f._extra.control
-0000f610: 5f66 6c6f 775f 6374 7820 3d20 4e6f 6e65  _flow_ctx = None
-0000f620: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
-0000f630: 206b 6579 2c20 6469 6d5f 2069 6e20 7365   key, dim_ in se
-0000f640: 6c66 2e5f 6578 7472 612e 7361 6d65 5f66  lf._extra.same_f
-0000f650: 6f72 5f62 6174 6368 5f63 7478 2e69 7465  or_batch_ctx.ite
-0000f660: 6d73 2829 3a0a 2020 2020 2020 2020 2020  ms():.          
-0000f670: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
-0000f680: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
-0000f690: 4d65 6d62 6572 0a20 2020 2020 2020 2020  Member.         
-0000f6a0: 2020 2020 2020 2064 696d 5f65 7874 7261         dim_extra
-0000f6b0: 203d 2064 696d 5f2e 5f65 7874 7261 0a20   = dim_._extra. 
-0000f6c0: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000f6d0: 6620 6469 6d5f 6578 7472 613a 0a20 2020  f dim_extra:.   
-0000f6e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6f0: 2064 696d 5f65 7874 7261 2e62 6174 6368   dim_extra.batch
-0000f700: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
-0000f710: 2020 2020 2020 2020 2020 2020 6469 6d5f              dim_
-0000f720: 6578 7472 612e 636f 6e74 726f 6c5f 666c  extra.control_fl
-0000f730: 6f77 5f63 7478 203d 204e 6f6e 650a 2020  ow_ctx = None.  
-0000f740: 2020 2020 2020 6966 2073 656c 662e 6261        if self.ba
-0000f750: 7463 683a 0a20 2020 2020 2020 2020 2020  tch:.           
-0000f760: 2073 656c 665f 203d 2073 656c 662e 6765   self_ = self.ge
-0000f770: 745f 666f 725f 6261 7463 685f 6374 7828  t_for_batch_ctx(
-0000f780: 6261 7463 683d 7365 6c66 2e62 6174 6368  batch=self.batch
-0000f790: 2c20 6374 783d 7365 6c66 2e63 6f6e 7472  , ctx=self.contr
-0000f7a0: 6f6c 5f66 6c6f 775f 6374 7829 0a20 2020  ol_flow_ctx).   
-0000f7b0: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
-0000f7c0: 5f20 6973 206e 6f74 2073 656c 663a 0a20  _ is not self:. 
-0000f7d0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-0000f7e0: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
-0000f7f0: 5f63 7478 203d 2073 656c 665f 2e63 6f6e  _ctx = self_.con
-0000f800: 7472 6f6c 5f66 6c6f 775f 6374 7820 2023  trol_flow_ctx  #
-0000f810: 206d 6967 6874 2062 6520 6469 6666 6572   might be differ
-0000f820: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
-0000f830: 2020 2020 7365 6c66 2e64 796e 5f73 697a      self.dyn_siz
-0000f840: 655f 6578 7420 3d20 7365 6c66 5f2e 6479  e_ext = self_.dy
-0000f850: 6e5f 7369 7a65 5f65 7874 2020 2320 6d69  n_size_ext  # mi
-0000f860: 6768 7420 6265 2075 6e73 6574 0a0a 2020  ght be unset..  
-0000f870: 2020 6465 6620 5f6d 6572 6765 5f73 616d    def _merge_sam
-0000f880: 655f 666f 725f 6261 7463 685f 6374 785f  e_for_batch_ctx_
-0000f890: 6469 6374 2873 656c 663a 205f 642e 4469  dict(self: _d.Di
-0000f8a0: 6d2c 206f 7468 6572 3a20 5f64 2e44 696d  m, other: _d.Dim
-0000f8b0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-0000f8c0: 2020 2020 2020 203a 7061 7261 6d20 6f74         :param ot
-0000f8d0: 6865 723a 0a20 2020 2020 2020 2022 2222  her:.        """
-0000f8e0: 0a20 2020 2020 2020 2023 206e 6f69 6e73  .        # noins
-0000f8f0: 7065 6374 696f 6e20 5079 5072 6f74 6563  pection PyProtec
-0000f900: 7465 644d 656d 6265 720a 2020 2020 2020  tedMember.      
-0000f910: 2020 6966 206e 6f74 2073 656c 662e 5f65    if not self._e
-0000f920: 7874 7261 2061 6e64 206e 6f74 206f 7468  xtra and not oth
-0000f930: 6572 2e5f 6578 7472 613a 0a20 2020 2020  er._extra:.     
-0000f940: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-0000f950: 2020 2020 2020 7365 6c66 2e5f 7661 6c69        self._vali
-0000f960: 6461 7465 5f69 6e5f 6375 7272 656e 745f  date_in_current_
-0000f970: 6772 6170 6828 290a 2020 2020 2020 2020  graph().        
-0000f980: 6966 2073 656c 662e 5f65 7874 7261 3a0a  if self._extra:.
-0000f990: 2020 2020 2020 2020 2020 2020 666f 7220              for 
-0000f9a0: 5f2c 2064 696d 2069 6e20 6c69 7374 2873  _, dim in list(s
-0000f9b0: 656c 662e 5f65 7874 7261 2e73 616d 655f  elf._extra.same_
-0000f9c0: 666f 725f 6261 7463 685f 6374 782e 6974  for_batch_ctx.it
-0000f9d0: 656d 7328 2929 3a0a 2020 2020 2020 2020  ems()):.        
-0000f9e0: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
-0000f9f0: 7369 6e73 7461 6e63 6528 6469 6d2c 205f  sinstance(dim, _
-0000fa00: 642e 4469 6d29 0a20 2020 2020 2020 2020  d.Dim).         
-0000fa10: 2020 2020 2020 2064 696d 2e5f 7661 6c69         dim._vali
-0000fa20: 6461 7465 5f69 6e5f 6375 7272 656e 745f  date_in_current_
-0000fa30: 6772 6170 6828 290a 2020 2020 2020 2020  graph().        
-0000fa40: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
-0000fa50: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
-0000fa60: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
-0000fa70: 722e 5f65 7874 7261 3a0a 2020 2020 2020  r._extra:.      
-0000fa80: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
-0000fa90: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
-0000faa0: 4d65 6d62 6572 0a20 2020 2020 2020 2020  Member.         
-0000fab0: 2020 2066 6f72 206b 6579 2c20 6469 6d20     for key, dim 
-0000fac0: 696e 206f 7468 6572 2e5f 6578 7472 612e  in other._extra.
-0000fad0: 7361 6d65 5f66 6f72 5f62 6174 6368 5f63  same_for_batch_c
-0000fae0: 7478 2e69 7465 6d73 2829 3a0a 2020 2020  tx.items():.    
-0000faf0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
-0000fb00: 6f74 2064 696d 2e5f 7661 6c69 6461 7465  ot dim._validate
-0000fb10: 5f69 6e5f 6375 7272 656e 745f 6772 6170  _in_current_grap
-0000fb20: 6828 293a 0a20 2020 2020 2020 2020 2020  h():.           
-0000fb30: 2020 2020 2020 2020 2063 6f6e 7469 6e75           continu
-0000fb40: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
-0000fb50: 2020 7365 6c66 5f64 696d 203d 2073 656c    self_dim = sel
-0000fb60: 662e 5f6d 616b 655f 6578 7472 6128 292e  f._make_extra().
-0000fb70: 7361 6d65 5f66 6f72 5f62 6174 6368 5f63  same_for_batch_c
-0000fb80: 7478 2e67 6574 286b 6579 2c20 4e6f 6e65  tx.get(key, None
-0000fb90: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000fba0: 2020 6966 2073 656c 665f 6469 6d20 616e    if self_dim an
-0000fbb0: 6420 2873 656c 665f 6469 6d2e 6479 6e5f  d (self_dim.dyn_
-0000fbc0: 7369 7a65 5f65 7874 206f 7220 6e6f 7420  size_ext or not 
-0000fbd0: 6469 6d2e 6479 6e5f 7369 7a65 5f65 7874  dim.dyn_size_ext
-0000fbe0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-0000fbf0: 2020 2020 2020 2063 6f6e 7469 6e75 6520         continue 
-0000fc00: 2023 206b 6565 7020 6f75 7273 0a20 2020   # keep ours.   
-0000fc10: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-0000fc20: 6e6f 7420 6469 6d2e 6479 6e5f 7369 7a65  not dim.dyn_size
-0000fc30: 5f65 7874 3a0a 2020 2020 2020 2020 2020  _ext:.          
-0000fc40: 2020 2020 2020 2020 2020 636f 6e74 696e            contin
-0000fc50: 7565 2020 2320 756e 6465 6669 6e65 642c  ue  # undefined,
-0000fc60: 2064 6f20 6e6f 7420 6f76 6572 7461 6b65   do not overtake
-0000fc70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000fc80: 2073 656c 662e 5f65 7874 7261 2e73 616d   self._extra.sam
-0000fc90: 655f 666f 725f 6261 7463 685f 6374 785b  e_for_batch_ctx[
-0000fca0: 6b65 795d 203d 2064 696d 0a20 2020 2020  key] = dim.     
-0000fcb0: 2020 2020 2020 2023 206e 6f69 6e73 7065         # noinspe
-0000fcc0: 6374 696f 6e20 5079 5072 6f74 6563 7465  ction PyProtecte
-0000fcd0: 644d 656d 6265 720a 2020 2020 2020 2020  dMember.        
-0000fce0: 2020 2020 6f74 6865 722e 5f65 7874 7261      other._extra
-0000fcf0: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
-0000fd00: 6374 782e 636c 6561 7228 2920 2023 2077  ctx.clear()  # w
-0000fd10: 6520 6f6e 6c79 2077 616e 7420 746f 2068  e only want to h
-0000fd20: 6176 6520 6974 206f 6e63 650a 0a20 2020  ave it once..   
-0000fd30: 2023 206e 6f69 6e73 7065 6374 696f 6e20   # noinspection 
-0000fd40: 5079 5072 6f74 6563 7465 644d 656d 6265  PyProtectedMembe
-0000fd50: 720a 2020 2020 6465 6620 6465 7269 7665  r.    def derive
-0000fd60: 5f66 726f 6d28 7365 6c66 3a20 5f64 2e44  _from(self: _d.D
-0000fd70: 696d 2c20 6261 7365 3a20 5f64 2e44 696d  im, base: _d.Dim
-0000fd80: 2c20 7365 745f 6465 7269 7665 645f 6672  , set_derived_fr
-0000fd90: 6f6d 5f66 6c61 673a 2062 6f6f 6c20 3d20  om_flag: bool = 
-0000fda0: 5472 7565 293a 0a20 2020 2020 2020 2022  True):.        "
-0000fdb0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-0000fdc0: 6d20 6261 7365 3a20 6469 6d0a 2020 2020  m base: dim.    
-0000fdd0: 2020 2020 3a70 6172 616d 2073 6574 5f64      :param set_d
-0000fde0: 6572 6976 6564 5f66 726f 6d5f 666c 6167  erived_from_flag
-0000fdf0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-0000fe00: 2020 2020 2020 7365 6c66 5f62 6173 6520        self_base 
-0000fe10: 3d20 7365 6c66 2e67 6574 5f73 616d 655f  = self.get_same_
-0000fe20: 6261 7365 2829 0a20 2020 2020 2020 2073  base().        s
-0000fe30: 656c 665f 6261 7365 5f65 7874 7261 203d  elf_base_extra =
-0000fe40: 2073 656c 665f 6261 7365 2e5f 6d61 6b65   self_base._make
-0000fe50: 5f65 7874 7261 2829 0a20 2020 2020 2020  _extra().       
-0000fe60: 2069 6620 7365 745f 6465 7269 7665 645f   if set_derived_
-0000fe70: 6672 6f6d 5f66 6c61 673a 0a20 2020 2020  from_flag:.     
-0000fe80: 2020 2020 2020 2069 6620 7365 6c66 5f62         if self_b
-0000fe90: 6173 655f 6578 7472 612e 6465 7269 7665  ase_extra.derive
-0000fea0: 645f 6672 6f6d 5f74 6167 3a0a 2020 2020  d_from_tag:.    
-0000feb0: 2020 2020 2020 2020 2020 2020 6173 7365              asse
-0000fec0: 7274 2073 656c 665f 6261 7365 5f65 7874  rt self_base_ext
-0000fed0: 7261 2e64 6572 6976 6564 5f66 726f 6d5f  ra.derived_from_
-0000fee0: 7461 6720 3d3d 2062 6173 650a 2020 2020  tag == base.    
-0000fef0: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
-0000ff00: 2020 2020 2020 2020 2020 2020 2020 7365                se
-0000ff10: 6c66 5f62 6173 655f 6578 7472 612e 6465  lf_base_extra.de
-0000ff20: 7269 7665 645f 6672 6f6d 5f74 6167 203d  rived_from_tag =
-0000ff30: 2062 6173 650a 2020 2020 2020 2020 6966   base.        if
-0000ff40: 2073 656c 662e 6973 5f64 796e 616d 6963   self.is_dynamic
-0000ff50: 2829 206f 7220 6e6f 7420 7365 6c66 2e69  () or not self.i
-0000ff60: 735f 6469 6d5f 6b6e 6f77 6e28 293a 0a20  s_dim_known():. 
-0000ff70: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-0000ff80: 7420 7365 6c66 2e62 6174 6368 2061 6e64  t self.batch and
-0000ff90: 2062 6173 652e 6261 7463 683a 0a20 2020   base.batch:.   
-0000ffa0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-0000ffb0: 662e 6261 7463 6820 3d20 6261 7365 2e62  f.batch = base.b
-0000ffc0: 6174 6368 0a20 2020 2020 2020 2020 2020  atch.           
-0000ffd0: 2020 2020 2073 656c 662e 636f 6e74 726f       self.contro
-0000ffe0: 6c5f 666c 6f77 5f63 7478 203d 2062 6173  l_flow_ctx = bas
-0000fff0: 652e 636f 6e74 726f 6c5f 666c 6f77 5f63  e.control_flow_c
-00010000: 7478 0a20 2020 2020 2020 2020 2020 2020  tx.             
-00010010: 2020 206b 6579 203d 2062 6173 652e 6261     key = base.ba
-00010020: 7463 682c 2062 6173 652e 636f 6e74 726f  tch, base.contro
-00010030: 6c5f 666c 6f77 5f63 7478 0a20 2020 2020  l_flow_ctx.     
-00010040: 2020 2020 2020 2020 2020 2061 7373 6572             asser
-00010050: 7420 6b65 7920 6e6f 7420 696e 2073 656c  t key not in sel
-00010060: 665f 6261 7365 5f65 7874 7261 2e73 616d  f_base_extra.sam
-00010070: 655f 666f 725f 6261 7463 685f 6374 780a  e_for_batch_ctx.
-00010080: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010090: 7365 6c66 5f62 6173 655f 6578 7472 612e  self_base_extra.
-000100a0: 7361 6d65 5f66 6f72 5f62 6174 6368 5f63  same_for_batch_c
-000100b0: 7478 5b6b 6579 5d20 3d20 7365 6c66 0a20  tx[key] = self. 
-000100c0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
-000100d0: 7420 7365 6c66 2e64 796e 5f73 697a 655f  t self.dyn_size_
-000100e0: 6578 743a 0a20 2020 2020 2020 2020 2020  ext:.           
-000100f0: 2020 2020 2069 6620 6261 7365 2e64 796e       if base.dyn
-00010100: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
-00010110: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00010120: 6620 6261 7365 2e62 6174 6368 2061 6e64  f base.batch and
-00010130: 2062 6173 652e 6261 7463 6820 3d3d 2073   base.batch == s
-00010140: 656c 662e 6261 7463 6820 616e 6420 6261  elf.batch and ba
-00010150: 7365 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  se.control_flow_
-00010160: 6374 7820 3d3d 2073 656c 662e 636f 6e74  ctx == self.cont
-00010170: 726f 6c5f 666c 6f77 5f63 7478 3a0a 2020  rol_flow_ctx:.  
-00010180: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010190: 2020 2020 2020 7365 6c66 2e64 796e 5f73        self.dyn_s
-000101a0: 697a 655f 6578 7420 3d20 6261 7365 2e64  ize_ext = base.d
-000101b0: 796e 5f73 697a 655f 6578 742e 636f 7079  yn_size_ext.copy
-000101c0: 5f74 656d 706c 6174 6528 6e61 6d65 3d22  _template(name="
-000101d0: 2573 3a73 697a 6522 2025 2073 656c 665f  %s:size" % self_
-000101e0: 6261 7365 2e64 6573 6372 6970 7469 6f6e  base.description
-000101f0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-00010200: 2020 656c 6966 2062 6173 652e 6973 5f62    elif base.is_b
-00010210: 6174 6368 5f64 696d 2829 3a0a 2020 2020  atch_dim():.    
-00010220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010230: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
-00010240: 7420 3d20 5f74 2e54 656e 736f 7228 0a20  t = _t.Tensor(. 
-00010250: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010260: 2020 2020 2020 206e 616d 653d 2225 733a         name="%s:
-00010270: 6261 7463 6822 2025 2073 656c 665f 6261  batch" % self_ba
-00010280: 7365 2e64 6573 6372 6970 7469 6f6e 2c20  se.description, 
-00010290: 7368 6170 653d 2829 2c20 6474 7970 653d  shape=(), dtype=
-000102a0: 2269 6e74 3332 222c 2062 6174 6368 5f64  "int32", batch_d
-000102b0: 696d 5f61 7869 733d 4e6f 6e65 0a20 2020  im_axis=None.   
-000102c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000102d0: 2029 0a0a 2020 2020 6465 6620 636f 7079   )..    def copy
-000102e0: 5f66 726f 6d28 7365 6c66 3a20 4469 6d2c  _from(self: Dim,
-000102f0: 206f 7468 6572 3a20 4469 6d29 3a0a 2020   other: Dim):.  
-00010300: 2020 2020 2020 2222 2264 6566 696e 6522        """define"
-00010310: 2222 0a20 2020 2020 2020 2073 656c 662e  "".        self.
-00010320: 7369 7a65 203d 206f 7468 6572 2e73 697a  size = other.siz
-00010330: 650a 2020 2020 2020 2020 7365 6c66 2e63  e.        self.c
-00010340: 6170 6163 6974 7920 3d20 6f74 6865 722e  apacity = other.
-00010350: 6361 7061 6369 7479 0a20 2020 2020 2020  capacity.       
-00010360: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-00010370: 7874 203d 206f 7468 6572 2e64 796e 5f73  xt = other.dyn_s
-00010380: 697a 655f 6578 740a 2020 2020 2020 2020  ize_ext.        
-00010390: 7365 6c66 2e64 6572 6976 655f 6672 6f6d  self.derive_from
-000103a0: 286f 7468 6572 290a 0a20 2020 2040 636c  (other)..    @cl
-000103b0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
-000103c0: 6620 6765 745f 6578 6973 7469 6e67 5f74  f get_existing_t
-000103d0: 6167 5f66 726f 6d5f 636f 6c6c 6563 7469  ag_from_collecti
-000103e0: 6f6e 2863 6c73 2c20 6f74 6865 722c 2074  on(cls, other, t
-000103f0: 6167 732c 2069 735f 6571 7561 6c5f 6f70  ags, is_equal_op
-00010400: 7473 3d4e 6f6e 6529 3a0a 2020 2020 2020  ts=None):.      
-00010410: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
-00010420: 6172 616d 2044 696d 206f 7468 6572 3a0a  aram Dim other:.
-00010430: 2020 2020 2020 2020 3a70 6172 616d 206c          :param l
-00010440: 6973 745b 4469 6d5d 7c74 7570 6c65 5b44  ist[Dim]|tuple[D
-00010450: 696d 5d7c 7365 745b 4469 6d5d 2074 6167  im]|set[Dim] tag
-00010460: 733a 0a20 2020 2020 2020 203a 7061 7261  s:.        :para
-00010470: 6d20 6469 6374 5b73 7472 5d7c 4e6f 6e65  m dict[str]|None
-00010480: 2069 735f 6571 7561 6c5f 6f70 7473 3a20   is_equal_opts: 
-00010490: 7061 7373 6564 2074 6f20 4469 6d2e 6973  passed to Dim.is
-000104a0: 5f65 7175 616c 0a20 2020 2020 2020 203a  _equal.        :
-000104b0: 7274 7970 653a 2044 696d 7c4e 6f6e 650a  rtype: Dim|None.
-000104c0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000104d0: 2020 2020 6966 2069 735f 6571 7561 6c5f      if is_equal_
-000104e0: 6f70 7473 2069 7320 4e6f 6e65 3a0a 2020  opts is None:.  
-000104f0: 2020 2020 2020 2020 2020 6973 5f65 7175            is_equ
-00010500: 616c 5f6f 7074 7320 3d20 7b7d 0a20 2020  al_opts = {}.   
-00010510: 2020 2020 2023 2057 6520 646f 2070 6f74       # We do pot
-00010520: 656e 7469 616c 206d 756c 7469 706c 6520  ential multiple 
-00010530: 726f 756e 6473 2c20 7375 6368 2074 6861  rounds, such tha
-00010540: 7420 7765 2070 7265 6665 7220 226d 6f72  t we prefer "mor
-00010550: 6520 6571 7561 6c22 2028 7573 696e 6720  e equal" (using 
-00010560: 6c65 7373 2069 735f 6571 7561 6c5f 6f70  less is_equal_op
-00010570: 7473 292e 0a20 2020 2020 2020 2072 6f75  ts)..        rou
-00010580: 6e64 7320 3d20 5b7b 7d5d 0a20 2020 2020  nds = [{}].     
-00010590: 2020 2069 6620 6973 5f65 7175 616c 5f6f     if is_equal_o
-000105a0: 7074 733a 0a20 2020 2020 2020 2020 2020  pts:.           
-000105b0: 2069 6620 2262 726f 6164 6361 7374 5f6d   if "broadcast_m
-000105c0: 6174 6368 6573 2220 696e 2069 735f 6571  atches" in is_eq
-000105d0: 7561 6c5f 6f70 7473 3a0a 2020 2020 2020  ual_opts:.      
-000105e0: 2020 2020 2020 2020 2020 726f 756e 6473            rounds
-000105f0: 2e61 7070 656e 6428 7b6b 3a20 7620 666f  .append({k: v fo
-00010600: 7220 286b 2c20 7629 2069 6e20 6973 5f65  r (k, v) in is_e
-00010610: 7175 616c 5f6f 7074 732e 6974 656d 7328  qual_opts.items(
-00010620: 2920 6966 206b 2021 3d20 2262 726f 6164  ) if k != "broad
-00010630: 6361 7374 5f6d 6174 6368 6573 227d 290a  cast_matches"}).
-00010640: 2020 2020 2020 2020 2020 2020 726f 756e              roun
-00010650: 6473 2e61 7070 656e 6428 6973 5f65 7175  ds.append(is_equ
-00010660: 616c 5f6f 7074 7329 0a20 2020 2020 2020  al_opts).       
-00010670: 2066 6f72 205f 6973 5f65 7175 616c 5f6f   for _is_equal_o
-00010680: 7074 7320 696e 2072 6f75 6e64 733a 0a20  pts in rounds:. 
-00010690: 2020 2020 2020 2020 2020 2066 6f72 205f             for _
-000106a0: 7461 6720 696e 2074 6167 733a 0a20 2020  tag in tags:.   
-000106b0: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-000106c0: 5f74 6167 2e69 735f 6571 7561 6c28 6f74  _tag.is_equal(ot
-000106d0: 6865 722c 202a 2a5f 6973 5f65 7175 616c  her, **_is_equal
-000106e0: 5f6f 7074 7329 3a0a 2020 2020 2020 2020  _opts):.        
-000106f0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00010700: 726e 205f 7461 670a 2020 2020 2020 2020  rn _tag.        
-00010710: 7265 7475 726e 204e 6f6e 650a 0a20 2020  return None..   
-00010720: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00010730: 2020 6465 6620 6765 745f 616c 6c5f 6469    def get_all_di
-00010740: 6d65 6e73 696f 6e5f 7461 6773 2863 6c73  mension_tags(cls
-00010750: 2c20 6461 7461 5f6c 6973 742c 2069 735f  , data_list, is_
-00010760: 6571 7561 6c5f 6f70 7473 3d4e 6f6e 652c  equal_opts=None,
-00010770: 2075 6e69 7175 655f 7365 7061 7261 7465   unique_separate
-00010780: 5f61 7865 733d 5472 7565 293a 0a20 2020  _axes=True):.   
-00010790: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000107a0: 203a 7061 7261 6d20 6c69 7374 5b5f 742e   :param list[_t.
-000107b0: 5465 6e73 6f72 5d20 6461 7461 5f6c 6973  Tensor] data_lis
-000107c0: 743a 0a20 2020 2020 2020 203a 7061 7261  t:.        :para
-000107d0: 6d20 6469 6374 5b73 7472 5d7c 4e6f 6e65  m dict[str]|None
-000107e0: 2069 735f 6571 7561 6c5f 6f70 7473 3a20   is_equal_opts: 
-000107f0: 7061 7373 6564 2074 6f20 4469 6d2e 6973  passed to Dim.is
-00010800: 5f65 7175 616c 0a20 2020 2020 2020 203a  _equal.        :
-00010810: 7061 7261 6d20 626f 6f6c 2075 6e69 7175  param bool uniqu
-00010820: 655f 7365 7061 7261 7465 5f61 7865 733a  e_separate_axes:
-00010830: 2065 2e67 2e20 6461 7461 5f6c 6973 743d   e.g. data_list=
-00010840: 5b44 6174 6120 7769 7468 2073 6861 7065  [Data with shape
-00010850: 2028 422c 352c 352c 3130 295d 2072 6573   (B,5,5,10)] res
-00010860: 756c 7473 2069 6e20 3420 6469 6d20 7461  ults in 4 dim ta
-00010870: 6773 2c20 6e6f 7420 332e 0a20 2020 2020  gs, not 3..     
-00010880: 2020 203a 7265 7475 726e 3a20 6c69 7374     :return: list
-00010890: 206f 6620 6469 6d65 6e73 696f 6e20 7461   of dimension ta
-000108a0: 6773 2c20 6469 6374 2066 6f72 2064 6174  gs, dict for dat
-000108b0: 6120 2d3e 206c 6973 7420 6f66 2064 696d  a -> list of dim
-000108c0: 656e 7369 6f6e 2074 6167 7320 2866 6f72  ension tags (for
-000108d0: 2065 6163 6820 6178 6973 290a 2020 2020   each axis).    
-000108e0: 2020 2020 3a72 7479 7065 3a20 286c 6973      :rtype: (lis
-000108f0: 745b 4469 6d5d 2c20 7574 696c 2e44 6963  t[Dim], util.Dic
-00010900: 7452 6566 4b65 7973 5b5f 742e 5465 6e73  tRefKeys[_t.Tens
-00010910: 6f72 2c20 6c69 7374 5b44 696d 5d5d 290a  or, list[Dim]]).
-00010920: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00010930: 2020 2020 7461 6773 203d 205b 5d0a 2020      tags = [].  
-00010940: 2020 2020 2020 6461 7461 5f61 7865 735f        data_axes_
-00010950: 6469 6374 203d 2075 7469 6c2e 4469 6374  dict = util.Dict
-00010960: 5265 664b 6579 7328 2920 2023 2074 7970  RefKeys()  # typ
-00010970: 653a 2075 7469 6c2e 4469 6374 5265 664b  e: util.DictRefK
-00010980: 6579 735b 5f74 2e54 656e 736f 722c 204c  eys[_t.Tensor, L
-00010990: 6973 745b 4469 6d5d 5d0a 2020 2020 2020  ist[Dim]].      
-000109a0: 2020 666f 7220 6461 7461 2069 6e20 6461    for data in da
-000109b0: 7461 5f6c 6973 743a 0a20 2020 2020 2020  ta_list:.       
-000109c0: 2020 2020 2064 6174 615f 6178 6573 5f64       data_axes_d
-000109d0: 6963 745b 6461 7461 5d20 3d20 5b5d 0a20  ict[data] = []. 
-000109e0: 2020 2020 2020 2020 2020 2065 7869 7374             exist
-000109f0: 696e 675f 7461 675f 636f 6c6c 6563 7469  ing_tag_collecti
-00010a00: 6f6e 5f66 6f72 5f64 6174 6120 3d20 6c69  on_for_data = li
-00010a10: 7374 2874 6167 7329 2069 6620 756e 6971  st(tags) if uniq
-00010a20: 7565 5f73 6570 6172 6174 655f 6178 6573  ue_separate_axes
-00010a30: 2065 6c73 6520 7461 6773 0a20 2020 2020   else tags.     
-00010a40: 2020 2020 2020 2066 6f72 2061 7869 7320         for axis 
-00010a50: 696e 2072 616e 6765 2864 6174 612e 6261  in range(data.ba
-00010a60: 7463 685f 6e64 696d 293a 0a20 2020 2020  tch_ndim):.     
-00010a70: 2020 2020 2020 2020 2020 2074 6167 203d             tag =
-00010a80: 2064 6174 612e 6765 745f 6469 6d5f 7461   data.get_dim_ta
-00010a90: 6728 6178 6973 290a 2020 2020 2020 2020  g(axis).        
-00010aa0: 2020 2020 2020 2020 6578 6973 7469 6e67          existing
-00010ab0: 5f74 6167 203d 2063 6c73 2e67 6574 5f65  _tag = cls.get_e
-00010ac0: 7869 7374 696e 675f 7461 675f 6672 6f6d  xisting_tag_from
-00010ad0: 5f63 6f6c 6c65 6374 696f 6e28 0a20 2020  _collection(.   
-00010ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010af0: 2074 6167 2c20 7461 6773 3d65 7869 7374   tag, tags=exist
-00010b00: 696e 675f 7461 675f 636f 6c6c 6563 7469  ing_tag_collecti
-00010b10: 6f6e 5f66 6f72 5f64 6174 612c 2069 735f  on_for_data, is_
-00010b20: 6571 7561 6c5f 6f70 7473 3d69 735f 6571  equal_opts=is_eq
-00010b30: 7561 6c5f 6f70 7473 0a20 2020 2020 2020  ual_opts.       
-00010b40: 2020 2020 2020 2020 2029 0a20 2020 2020           ).     
-00010b50: 2020 2020 2020 2020 2020 2069 6620 6578             if ex
-00010b60: 6973 7469 6e67 5f74 6167 3a0a 2020 2020  isting_tag:.    
-00010b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010b80: 6966 2075 6e69 7175 655f 7365 7061 7261  if unique_separa
-00010b90: 7465 5f61 7865 733a 0a20 2020 2020 2020  te_axes:.       
-00010ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010bb0: 2065 7869 7374 696e 675f 7461 675f 636f   existing_tag_co
-00010bc0: 6c6c 6563 7469 6f6e 5f66 6f72 5f64 6174  llection_for_dat
-00010bd0: 612e 7265 6d6f 7665 2865 7869 7374 696e  a.remove(existin
-00010be0: 675f 7461 6729 2020 2320 646f 6e27 7420  g_tag)  # don't 
-00010bf0: 7461 6b65 2069 7420 6167 6169 6e20 666f  take it again fo
-00010c00: 7220 7468 6973 2064 6174 610a 2020 2020  r this data.    
-00010c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010c20: 7265 706c 6163 655f 6578 6973 7469 6e67  replace_existing
-00010c30: 203d 2028 0a20 2020 2020 2020 2020 2020   = (.           
-00010c40: 2020 2020 2020 2020 2020 2020 2065 7869               exi
-00010c50: 7374 696e 675f 7461 672e 756e 6465 6669  sting_tag.undefi
-00010c60: 6e65 6420 616e 6420 6e6f 7420 7461 672e  ned and not tag.
-00010c70: 756e 6465 6669 6e65 6420 616e 6420 7461  undefined and ta
-00010c80: 672e 6469 6d65 6e73 696f 6e20 3d3d 2065  g.dimension == e
-00010c90: 7869 7374 696e 675f 7461 672e 6469 6d65  xisting_tag.dime
-00010ca0: 6e73 696f 6e0a 2020 2020 2020 2020 2020  nsion.          
-00010cb0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
-00010cc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010cd0: 6966 2072 6570 6c61 6365 5f65 7869 7374  if replace_exist
-00010ce0: 696e 673a 2020 2320 5265 706c 6163 6520  ing:  # Replace 
-00010cf0: 7468 6520 6578 6973 7469 6e67 2062 7920  the existing by 
-00010d00: 7468 6520 6e65 7720 7461 672e 0a20 2020  the new tag..   
-00010d10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d20: 2020 2020 2074 6167 735b 7461 6773 2e69       tags[tags.i
-00010d30: 6e64 6578 2865 7869 7374 696e 675f 7461  ndex(existing_ta
-00010d40: 6729 5d20 3d20 7461 670a 2020 2020 2020  g)] = tag.      
-00010d50: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010d60: 2020 666f 7220 5f2c 2064 696d 735f 2069    for _, dims_ i
-00010d70: 6e20 6461 7461 5f61 7865 735f 6469 6374  n data_axes_dict
-00010d80: 2e69 7465 6d73 2829 3a0a 2020 2020 2020  .items():.      
-00010d90: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010da0: 2020 2020 2020 6469 6d73 5f5b 3a5d 203d        dims_[:] =
-00010db0: 205b 7461 6720 6966 2064 203d 3d20 6578   [tag if d == ex
-00010dc0: 6973 7469 6e67 5f74 6167 2065 6c73 6520  isting_tag else 
-00010dd0: 6420 666f 7220 6420 696e 2064 696d 735f  d for d in dims_
-00010de0: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-00010df0: 2020 2020 2020 2020 2020 6578 6973 7469            existi
-00010e00: 6e67 5f74 6167 203d 2074 6167 0a20 2020  ng_tag = tag.   
-00010e10: 2020 2020 2020 2020 2020 2020 2065 6c73               els
-00010e20: 653a 2020 2320 6e6f 2065 7869 7374 696e  e:  # no existin
-00010e30: 6720 7461 670a 2020 2020 2020 2020 2020  g tag.          
-00010e40: 2020 2020 2020 2020 2020 7461 6773 2e61            tags.a
-00010e50: 7070 656e 6428 7461 6729 0a20 2020 2020  ppend(tag).     
-00010e60: 2020 2020 2020 2020 2020 2064 6174 615f             data_
-00010e70: 6178 6573 5f64 6963 745b 6461 7461 5d2e  axes_dict[data].
-00010e80: 6170 7065 6e64 2865 7869 7374 696e 675f  append(existing_
-00010e90: 7461 6720 6f72 2074 6167 290a 2020 2020  tag or tag).    
-00010ea0: 2020 2020 7265 7475 726e 2074 6167 732c      return tags,
-00010eb0: 2064 6174 615f 6178 6573 5f64 6963 740a   data_axes_dict.
-00010ec0: 0a20 2020 2040 636c 6173 736d 6574 686f  .    @classmetho
-00010ed0: 640a 2020 2020 6465 6620 6765 745f 756e  d.    def get_un
-00010ee0: 6971 5f63 6f6c 6c65 6374 696f 6e28 636c  iq_collection(cl
-00010ef0: 732c 2074 6167 732c 2069 735f 6571 7561  s, tags, is_equa
-00010f00: 6c5f 6f70 7473 3d4e 6f6e 6529 3a0a 2020  l_opts=None):.  
-00010f10: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00010f20: 2020 3a70 6172 616d 206c 6973 745b 4469    :param list[Di
-00010f30: 6d5d 7c74 7570 6c65 5b44 696d 5d7c 7365  m]|tuple[Dim]|se
-00010f40: 745b 4469 6d5d 2074 6167 733a 0a20 2020  t[Dim] tags:.   
-00010f50: 2020 2020 203a 7061 7261 6d20 6469 6374       :param dict
-00010f60: 5b73 7472 5d7c 4e6f 6e65 2069 735f 6571  [str]|None is_eq
-00010f70: 7561 6c5f 6f70 7473 3a20 7061 7373 6564  ual_opts: passed
-00010f80: 2074 6f20 4469 6d2e 6973 5f65 7175 616c   to Dim.is_equal
-00010f90: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00010fa0: 206c 6973 745b 4469 6d5d 0a20 2020 2020   list[Dim].     
-00010fb0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00010fc0: 6573 203d 205b 5d0a 2020 2020 2020 2020  es = [].        
-00010fd0: 666f 7220 7461 6720 696e 2074 6167 733a  for tag in tags:
-00010fe0: 0a20 2020 2020 2020 2020 2020 2065 7820  .            ex 
-00010ff0: 3d20 636c 732e 6765 745f 6578 6973 7469  = cls.get_existi
-00011000: 6e67 5f74 6167 5f66 726f 6d5f 636f 6c6c  ng_tag_from_coll
-00011010: 6563 7469 6f6e 2874 6167 2c20 7265 732c  ection(tag, res,
-00011020: 2069 735f 6571 7561 6c5f 6f70 7473 3d69   is_equal_opts=i
-00011030: 735f 6571 7561 6c5f 6f70 7473 290a 2020  s_equal_opts).  
-00011040: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00011050: 2065 783a 0a20 2020 2020 2020 2020 2020   ex:.           
-00011060: 2020 2020 2072 6573 2e61 7070 656e 6428       res.append(
-00011070: 7461 6729 0a20 2020 2020 2020 2072 6574  tag).        ret
-00011080: 7572 6e20 7265 730a 0a20 2020 2064 6566  urn res..    def
-00011090: 2067 6574 5f73 697a 655f 7465 6e73 6f72   get_size_tensor
-000110a0: 2873 656c 6629 202d 3e20 5f74 2e54 656e  (self) -> _t.Ten
-000110b0: 736f 723a 0a20 2020 2020 2020 2022 2222  sor:.        """
-000110c0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
-000110d0: 3a20 7369 7a65 2074 656e 736f 722c 206f  : size tensor, o
-000110e0: 7220 6479 6e5f 7369 7a65 5f65 7874 2069  r dyn_size_ext i
-000110f0: 6620 6465 6669 6e65 640a 2020 2020 2020  f defined.      
-00011100: 2020 3a72 7479 7065 3a20 5f74 2e54 656e    :rtype: _t.Ten
-00011110: 736f 720a 2020 2020 2020 2020 2222 220a  sor.        """.
-00011120: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
-00011130: 6479 6e5f 7369 7a65 5f65 7874 3a0a 2020  dyn_size_ext:.  
-00011140: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00011150: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
-00011160: 7874 0a0a 2020 2020 2020 2020 696d 706f  xt..        impo
-00011170: 7274 2072 6574 7572 6e6e 2e66 726f 6e74  rt returnn.front
-00011180: 656e 6420 6173 2072 660a 0a20 2020 2020  end as rf..     
-00011190: 2020 2061 7373 6572 7420 7365 6c66 2e73     assert self.s
-000111a0: 697a 6520 6973 206e 6f74 204e 6f6e 650a  ize is not None.
-000111b0: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-000111c0: 662e 636f 6e76 6572 745f 746f 5f74 656e  f.convert_to_ten
-000111d0: 736f 7228 7365 6c66 2e73 697a 652c 206e  sor(self.size, n
-000111e0: 616d 653d 2225 733a 7369 7a65 2220 2520  ame="%s:size" % 
-000111f0: 7365 6c66 2e64 6573 6372 6970 7469 6f6e  self.description
-00011200: 290a 0a20 2020 2064 6566 2067 6574 5f64  )..    def get_d
-00011210: 696d 5f76 616c 7565 2873 656c 6629 202d  im_value(self) -
-00011220: 3e20 556e 696f 6e5b 696e 742c 205f 742e  > Union[int, _t.
-00011230: 5261 7754 656e 736f 7254 7970 655d 3a0a  RawTensorType]:.
-00011240: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011250: 2020 2020 496e 6665 7273 2074 6865 2064      Infers the d
-00011260: 696d 2074 6869 7320 6178 6973 2073 686f  im this axis sho
-00011270: 756c 6420 6861 7665 2069 6620 756e 6272  uld have if unbr
-00011280: 6f61 6463 6173 7465 642e 0a20 2020 2020  oadcasted..     
-00011290: 2020 2049 6620 6073 656c 662e 7372 635f     If `self.src_
-000112a0: 6461 7461 6020 6861 7320 6120 706c 6163  data` has a plac
-000112b0: 6568 6f6c 6465 722c 2077 696c 6c20 7573  eholder, will us
-000112c0: 6520 7468 6520 7368 6170 6520 6672 6f6d  e the shape from
-000112d0: 2074 6865 7265 2e0a 2020 2020 2020 2020   there..        
-000112e0: 4f74 6865 7277 6973 652c 2075 7365 7320  Otherwise, uses 
-000112f0: 6073 656c 662e 6469 6d65 6e73 696f 6e60  `self.dimension`
-00011300: 2028 6966 2073 7461 7469 6329 206f 7220   (if static) or 
-00011310: 6073 656c 662e 6479 6e5f 7369 7a65 6020  `self.dyn_size` 
-00011320: 2869 6620 6479 6e61 6d69 6329 2e0a 0a20  (if dynamic)... 
-00011330: 2020 2020 2020 203a 7265 7475 726e 3a20         :return: 
-00011340: 6d61 7828 7369 7a65 206f 7220 6479 6e5f  max(size or dyn_
-00011350: 7369 7a65 290a 2020 2020 2020 2020 2222  size).        ""
-00011360: 220a 2020 2020 2020 2020 7265 7320 3d20  ".        res = 
-00011370: 7365 6c66 2e67 6574 5f64 696d 5f76 616c  self.get_dim_val
-00011380: 7565 5f74 656e 736f 7228 290a 2020 2020  ue_tensor().    
-00011390: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-000113a0: 6528 7265 732c 205f 742e 5465 6e73 6f72  e(res, _t.Tensor
-000113b0: 293a 0a20 2020 2020 2020 2020 2020 2061  ):.            a
-000113c0: 7373 6572 7420 7265 732e 6469 6d73 203d  ssert res.dims =
-000113d0: 3d20 2829 0a20 2020 2020 2020 2020 2020  = ().           
-000113e0: 2072 6574 7572 6e20 7265 732e 7261 775f   return res.raw_
-000113f0: 7465 6e73 6f72 0a20 2020 2020 2020 2061  tensor.        a
-00011400: 7373 6572 7420 6973 696e 7374 616e 6365  ssert isinstance
-00011410: 2872 6573 2c20 696e 7429 0a20 2020 2020  (res, int).     
-00011420: 2020 2072 6574 7572 6e20 7265 730a 0a20     return res.. 
-00011430: 2020 2064 6566 2067 6574 5f64 696d 5f76     def get_dim_v
-00011440: 616c 7565 5f74 656e 736f 7228 7365 6c66  alue_tensor(self
-00011450: 2920 2d3e 2055 6e69 6f6e 5b69 6e74 2c20  ) -> Union[int, 
-00011460: 5f74 2e54 656e 736f 725d 3a0a 2020 2020  _t.Tensor]:.    
-00011470: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00011480: 496e 6665 7273 2074 6865 2064 696d 2074  Infers the dim t
-00011490: 6869 7320 6178 6973 2073 686f 756c 6420  his axis should 
-000114a0: 6861 7665 2069 6620 756e 6272 6f61 6463  have if unbroadc
-000114b0: 6173 7465 642e 0a20 2020 2020 2020 2049  asted..        I
-000114c0: 6620 6073 656c 662e 7372 635f 6461 7461  f `self.src_data
-000114d0: 6020 6861 7320 6120 706c 6163 6568 6f6c  ` has a placehol
-000114e0: 6465 722c 2077 696c 6c20 7573 6520 7468  der, will use th
-000114f0: 6520 7368 6170 6520 6672 6f6d 2074 6865  e shape from the
-00011500: 7265 2e0a 2020 2020 2020 2020 4f74 6865  re..        Othe
-00011510: 7277 6973 652c 2075 7365 7320 6073 656c  rwise, uses `sel
-00011520: 662e 6469 6d65 6e73 696f 6e60 2028 6966  f.dimension` (if
-00011530: 2073 7461 7469 6329 206f 7220 6073 656c   static) or `sel
-00011540: 662e 6479 6e5f 7369 7a65 6020 2869 6620  f.dyn_size` (if 
-00011550: 6479 6e61 6d69 6329 2e0a 0a20 2020 2020  dynamic)...     
-00011560: 2020 203a 7265 7475 726e 3a20 6d61 7828     :return: max(
-00011570: 7369 7a65 206f 7220 6479 6e5f 7369 7a65  size or dyn_size
-00011580: 290a 2020 2020 2020 2020 2222 220a 2020  ).        """.  
-00011590: 2020 2020 2020 696d 706f 7274 2072 6574        import ret
-000115a0: 7572 6e6e 2e66 726f 6e74 656e 6420 6173  urnn.frontend as
-000115b0: 2072 660a 0a20 2020 2020 2020 2069 6620   rf..        if 
-000115c0: 7365 6c66 2e64 696d 656e 7369 6f6e 2069  self.dimension i
-000115d0: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-000115e0: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-000115f0: 656c 662e 6469 6d65 6e73 696f 6e0a 2020  elf.dimension.  
-00011600: 2020 2020 2020 6966 2073 656c 662e 6479        if self.dy
-00011610: 6e5f 7369 7a65 5f65 7874 2061 6e64 2073  n_size_ext and s
-00011620: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
-00011630: 2e70 6c61 6365 686f 6c64 6572 2069 7320  .placeholder is 
-00011640: 6e6f 7420 4e6f 6e65 3a20 2023 2066 6173  not None:  # fas
-00011650: 7420 7061 7468 0a20 2020 2020 2020 2020  t path.         
-00011660: 2020 2069 6620 7365 6c66 2e64 796e 5f73     if self.dyn_s
-00011670: 697a 655f 6578 742e 6261 7463 685f 6e64  ize_ext.batch_nd
-00011680: 696d 203e 2030 3a0a 2020 2020 2020 2020  im > 0:.        
-00011690: 2020 2020 2020 2020 7265 7475 726e 2072          return r
-000116a0: 662e 7265 6475 6365 5f6d 6178 280a 2020  f.reduce_max(.  
-000116b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000116c0: 2020 7365 6c66 2e64 796e 5f73 697a 655f    self.dyn_size_
-000116d0: 6578 742c 0a20 2020 2020 2020 2020 2020  ext,.           
-000116e0: 2020 2020 2020 2020 2061 7869 733d 7365           axis=se
-000116f0: 6c66 2e64 796e 5f73 697a 655f 6578 742e  lf.dyn_size_ext.
-00011700: 6469 6d5f 7461 6773 2c0a 2020 2020 2020  dim_tags,.      
-00011710: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00011720: 4d61 736b 696e 6720 6973 206e 6f74 2061  Masking is not a
-00011730: 6c77 6179 7320 706f 7373 6962 6c65 2068  lways possible h
-00011740: 6572 652c 2065 2e67 2e0a 2020 2020 2020  ere, e.g..      
-00011750: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00011760: 7365 6c66 203d 2044 696d 7b27 7365 6c66  self = Dim{'self
-00011770: 2d61 7474 2d6b 6579 7327 5b27 7469 6d65  -att-keys'['time
-00011780: 3a76 6172 3a65 7874 6572 6e5f 6461 7461  :var:extern_data
-00011790: 3a63 6c61 7373 6573 275b 425d 5d7d 2e0a  :classes'[B]]}..
-000117a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000117b0: 2020 2020 7573 655f 6d61 736b 3d46 616c      use_mask=Fal
-000117c0: 7365 2c0a 2020 2020 2020 2020 2020 2020  se,.            
-000117d0: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-000117e0: 2020 7265 7475 726e 2073 656c 662e 6479    return self.dy
-000117f0: 6e5f 7369 7a65 5f65 7874 0a20 2020 2020  n_size_ext.     
-00011800: 2020 2069 6620 7365 6c66 2e69 735f 6261     if self.is_ba
-00011810: 7463 685f 6469 6d28 293a 0a20 2020 2020  tch_dim():.     
-00011820: 2020 2020 2020 2072 6573 203d 204e 6f6e         res = Non
-00011830: 650a 2020 2020 2020 2020 2020 2020 6966  e.            if
-00011840: 2073 656c 662e 5f65 7874 7261 2061 6e64   self._extra and
-00011850: 2073 656c 662e 5f65 7874 7261 2e73 7263   self._extra.src
-00011860: 5f64 6174 613a 0a20 2020 2020 2020 2020  _data:.         
-00011870: 2020 2020 2020 2072 6573 203d 2073 656c         res = sel
-00011880: 662e 5f65 7874 7261 2e73 7263 5f64 6174  f._extra.src_dat
-00011890: 612e 6765 745f 6261 7463 685f 6469 6d28  a.get_batch_dim(
-000118a0: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
-000118b0: 6966 2073 656c 662e 6261 7463 683a 0a20  if self.batch:. 
-000118c0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-000118d0: 6573 203d 2073 656c 662e 6261 7463 682e  es = self.batch.
-000118e0: 6469 6d0a 2020 2020 2020 2020 2020 2020  dim.            
-000118f0: 6966 2069 7369 6e73 7461 6e63 6528 7265  if isinstance(re
-00011900: 732c 2069 6e74 293a 0a20 2020 2020 2020  s, int):.       
-00011910: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00011920: 7265 730a 2020 2020 2020 2020 2020 2020  res.            
-00011930: 6966 2072 6573 2069 7320 6e6f 7420 4e6f  if res is not No
-00011940: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00011950: 2020 2020 7265 7475 726e 205f 742e 5465      return _t.Te
-00011960: 6e73 6f72 2822 6261 7463 6822 2c20 6469  nsor("batch", di
-00011970: 6d73 3d28 292c 2064 7479 7065 3d72 662e  ms=(), dtype=rf.
-00011980: 6765 745f 6465 6661 756c 745f 6172 7261  get_default_arra
-00011990: 795f 696e 6465 785f 6474 7970 6528 292c  y_index_dtype(),
-000119a0: 2072 6177 5f74 656e 736f 723d 7265 7329   raw_tensor=res)
-000119b0: 0a20 2020 2020 2020 2069 6620 280a 2020  .        if (.  
-000119c0: 2020 2020 2020 2020 2020 7365 6c66 2e5f            self._
-000119d0: 6578 7472 610a 2020 2020 2020 2020 2020  extra.          
-000119e0: 2020 616e 6420 7365 6c66 2e5f 6578 7472    and self._extr
-000119f0: 612e 7372 635f 6461 7461 2069 7320 6e6f  a.src_data is no
-00011a00: 7420 4e6f 6e65 0a20 2020 2020 2020 2020  t None.         
-00011a10: 2020 2061 6e64 2073 656c 662e 5f65 7874     and self._ext
-00011a20: 7261 2e73 7263 5f61 7869 7320 6973 206e  ra.src_axis is n
-00011a30: 6f74 204e 6f6e 650a 2020 2020 2020 2020  ot None.        
-00011a40: 2020 2020 616e 6420 7365 6c66 2e5f 6578      and self._ex
-00011a50: 7472 612e 7372 635f 6461 7461 2e70 6c61  tra.src_data.pla
-00011a60: 6365 686f 6c64 6572 2069 7320 6e6f 7420  ceholder is not 
-00011a70: 4e6f 6e65 0a20 2020 2020 2020 2029 3a0a  None.        ):.
-00011a80: 2020 2020 2020 2020 2020 2020 7265 7320              res 
-00011a90: 3d20 7365 6c66 2e5f 6578 7472 612e 7372  = self._extra.sr
-00011aa0: 635f 6461 7461 2e67 6574 5f64 696d 2873  c_data.get_dim(s
-00011ab0: 656c 662e 5f65 7874 7261 2e73 7263 5f61  elf._extra.src_a
-00011ac0: 7869 7329 0a20 2020 2020 2020 2020 2020  xis).           
-00011ad0: 2069 6620 6973 696e 7374 616e 6365 2872   if isinstance(r
-00011ae0: 6573 2c20 696e 7429 3a0a 2020 2020 2020  es, int):.      
-00011af0: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00011b00: 2072 6573 0a20 2020 2020 2020 2020 2020   res.           
-00011b10: 2072 6574 7572 6e20 5f74 2e54 656e 736f   return _t.Tenso
-00011b20: 7228 2262 6174 6368 222c 2064 696d 733d  r("batch", dims=
-00011b30: 2829 2c20 6474 7970 653d 7266 2e67 6574  (), dtype=rf.get
-00011b40: 5f64 6566 6175 6c74 5f61 7272 6179 5f69  _default_array_i
-00011b50: 6e64 6578 5f64 7479 7065 2829 2c20 7261  ndex_dtype(), ra
-00011b60: 775f 7465 6e73 6f72 3d72 6573 290a 2020  w_tensor=res).  
-00011b70: 2020 2020 2020 7365 6c66 2e63 6f6d 706c        self.compl
-00011b80: 6574 655f 6479 6e5f 7369 7a65 2829 0a20  ete_dyn_size(). 
-00011b90: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-00011ba0: 796e 5f73 697a 655f 6578 7420 616e 6420  yn_size_ext and 
-00011bb0: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
-00011bc0: 742e 706c 6163 6568 6f6c 6465 7220 6973  t.placeholder is
-00011bd0: 206e 6f74 204e 6f6e 653a 0a20 2020 2020   not None:.     
-00011be0: 2020 2020 2020 2069 6620 7365 6c66 2e64         if self.d
-00011bf0: 796e 5f73 697a 655f 6578 742e 6261 7463  yn_size_ext.batc
-00011c00: 685f 6e64 696d 203e 2030 3a0a 2020 2020  h_ndim > 0:.    
-00011c10: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00011c20: 726e 2072 662e 7265 6475 6365 5f6d 6178  rn rf.reduce_max
-00011c30: 2873 656c 662e 6479 6e5f 7369 7a65 5f65  (self.dyn_size_e
-00011c40: 7874 2c20 6178 6973 3d73 656c 662e 6479  xt, axis=self.dy
-00011c50: 6e5f 7369 7a65 5f65 7874 2e64 696d 5f74  n_size_ext.dim_t
-00011c60: 6167 7329 0a20 2020 2020 2020 2020 2020  ags).           
-00011c70: 2072 6574 7572 6e20 7365 6c66 2e64 796e   return self.dyn
-00011c80: 5f73 697a 655f 6578 740a 2020 2020 2020  _size_ext.      
-00011c90: 2020 7261 6973 6520 4578 6365 7074 696f    raise Exceptio
-00011ca0: 6e28 2225 733a 206e 6565 6420 706c 6163  n("%s: need plac
-00011cb0: 6568 6f6c 6465 722c 2073 656c 662e 6469  eholder, self.di
-00011cc0: 6d65 6e73 696f 6e20 6f72 2073 656c 662e  mension or self.
-00011cd0: 6479 6e5f 7369 7a65 2066 6f72 2064 696d  dyn_size for dim
-00011ce0: 2076 616c 7565 2220 2520 7365 6c66 290a   value" % self).
-00011cf0: 0a20 2020 2064 6566 2061 7869 735f 7370  .    def axis_sp
-00011d00: 6c69 745f 696e 666f 2873 656c 6629 3a0a  lit_info(self):.
-00011d10: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011d20: 2020 2020 3a72 6574 7572 6e3a 2061 7869      :return: axi
-00011d30: 7320 7370 6c69 7420 696e 666f 2e20 7365  s split info. se
-00011d40: 6520 3a66 756e 633a 6067 6574 5f70 6172  e :func:`get_par
-00011d50: 616d 5f61 7865 735f 7370 6c69 745f 696e  am_axes_split_in
-00011d60: 666f 6020 616e 6420 7573 6167 6520 2865  fo` and usage (e
-00011d70: 2e67 2e20 7072 6574 7261 696e 696e 6729  .g. pretraining)
-00011d80: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-00011d90: 206c 6973 745b 696e 747c 4e6f 6e65 5d0a   list[int|None].
-00011da0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00011db0: 2020 2020 7361 6d65 5f62 6173 6520 3d20      same_base = 
-00011dc0: 7365 6c66 2e67 6574 5f73 616d 655f 6261  self.get_same_ba
-00011dd0: 7365 2829 0a20 2020 2020 2020 206f 7020  se().        op 
-00011de0: 3d20 7365 6c66 2e64 6572 6976 6564 5f66  = self.derived_f
-00011df0: 726f 6d5f 6f70 206f 7220 7361 6d65 5f62  rom_op or same_b
-00011e00: 6173 652e 6465 7269 7665 645f 6672 6f6d  ase.derived_from
-00011e10: 5f6f 700a 2020 2020 2020 2020 6966 206e  _op.        if n
-00011e20: 6f74 206f 703a 0a20 2020 2020 2020 2020  ot op:.         
-00011e30: 2020 2072 6574 7572 6e20 5b73 656c 662e     return [self.
-00011e40: 6469 6d65 6e73 696f 6e5d 0a20 2020 2020  dimension].     
-00011e50: 2020 2069 6620 6f70 2e6b 696e 6420 3d3d     if op.kind ==
-00011e60: 2022 6164 6422 3a0a 2020 2020 2020 2020   "add":.        
-00011e70: 2020 2020 7265 7475 726e 2073 756d 285b      return sum([
-00011e80: 782e 6178 6973 5f73 706c 6974 5f69 6e66  x.axis_split_inf
-00011e90: 6f28 2920 666f 7220 7820 696e 206f 702e  o() for x in op.
-00011ea0: 696e 7075 7473 5d2c 205b 5d29 2020 2320  inputs], [])  # 
-00011eb0: 666c 6174 7465 6e0a 2020 2020 2020 2020  flatten.        
-00011ec0: 6966 206f 702e 6b69 6e64 203d 3d20 226d  if op.kind == "m
-00011ed0: 756c 223a 0a20 2020 2020 2020 2020 2020  ul":.           
-00011ee0: 2072 6573 203d 205b 315d 0a20 2020 2020   res = [1].     
-00011ef0: 2020 2020 2020 2066 6f72 2078 2069 6e20         for x in 
-00011f00: 6f70 2e69 6e70 7574 733a 0a20 2020 2020  op.inputs:.     
-00011f10: 2020 2020 2020 2020 2020 2072 6573 203d             res =
-00011f20: 2073 756d 285b 6e20 2a20 782e 6178 6973   sum([n * x.axis
-00011f30: 5f73 706c 6974 5f69 6e66 6f28 2920 6966  _split_info() if
-00011f40: 206e 2069 7320 6e6f 7420 4e6f 6e65 2065   n is not None e
-00011f50: 6c73 6520 4e6f 6e65 2066 6f72 206e 2069  lse None for n i
-00011f60: 6e20 7265 735d 2c20 5b5d 2920 2023 2066  n res], [])  # f
-00011f70: 6c61 7474 656e 0a20 2020 2020 2020 2020  latten.         
-00011f80: 2020 2072 6574 7572 6e20 7265 730a 2020     return res.  
-00011f90: 2020 2020 2020 7265 7475 726e 205b 7365        return [se
-00011fa0: 6c66 2e64 696d 656e 7369 6f6e 5d0a 0a20  lf.dimension].. 
-00011fb0: 2020 2064 6566 205f 6765 745f 7361 6d65     def _get_same
-00011fc0: 5f62 6173 655f 6578 7472 6128 7365 6c66  _base_extra(self
-00011fd0: 2920 2d3e 204f 7074 696f 6e61 6c5b 5f44  ) -> Optional[_D
-00011fe0: 696d 4578 7472 615d 3a0a 2020 2020 2020  imExtra]:.      
-00011ff0: 2020 6966 206e 6f74 2073 656c 662e 5f65    if not self._e
-00012000: 7874 7261 3a0a 2020 2020 2020 2020 2020  xtra:.          
-00012010: 2020 7265 7475 726e 204e 6f6e 650a 2020    return None.  
-00012020: 2020 2020 2020 6261 7365 203d 2073 656c        base = sel
-00012030: 662e 6765 745f 7361 6d65 5f62 6173 6528  f.get_same_base(
-00012040: 290a 2020 2020 2020 2020 2320 6e6f 696e  ).        # noin
-00012050: 7370 6563 7469 6f6e 2050 7950 726f 7465  spection PyProte
-00012060: 6374 6564 4d65 6d62 6572 0a20 2020 2020  ctedMember.     
-00012070: 2020 2072 6574 7572 6e20 6261 7365 2e5f     return base._
-00012080: 6578 7472 610a 0a20 2020 2064 6566 205f  extra..    def _
-00012090: 6d61 6b65 5f65 7874 7261 2873 656c 663a  make_extra(self:
-000120a0: 205f 642e 4469 6d29 202d 3e20 5f44 696d   _d.Dim) -> _Dim
-000120b0: 4578 7472 613a 0a20 2020 2020 2020 2069  Extra:.        i
-000120c0: 6620 6e6f 7420 7365 6c66 2e5f 6578 7472  f not self._extr
-000120d0: 613a 0a20 2020 2020 2020 2020 2020 2073  a:.            s
-000120e0: 656c 662e 5f65 7874 7261 203d 205f 4469  elf._extra = _Di
-000120f0: 6d45 7874 7261 2864 696d 3d73 656c 6629  mExtra(dim=self)
-00012100: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012110: 7365 6c66 2e5f 6578 7472 610a 0a20 2020  self._extra..   
-00012120: 2040 7072 6f70 6572 7479 0a20 2020 2064   @property.    d
-00012130: 6566 2076 6f63 6162 2873 656c 6629 3a0a  ef vocab(self):.
-00012140: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012150: 2020 2020 3a72 7479 7065 3a20 7265 7475      :rtype: retu
-00012160: 726e 6e2e 6461 7461 7365 7473 2e75 7469  rnn.datasets.uti
-00012170: 6c2e 766f 6361 6275 6c61 7279 2e56 6f63  l.vocabulary.Voc
-00012180: 6162 756c 6172 797c 4e6f 6e65 0a20 2020  abulary|None.   
-00012190: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-000121a0: 2065 7874 7261 203d 2073 656c 662e 5f67   extra = self._g
-000121b0: 6574 5f73 616d 655f 6261 7365 5f65 7874  et_same_base_ext
-000121c0: 7261 2829 0a20 2020 2020 2020 2069 6620  ra().        if 
-000121d0: 6578 7472 613a 0a20 2020 2020 2020 2020  extra:.         
-000121e0: 2020 2072 6574 7572 6e20 6578 7472 612e     return extra.
-000121f0: 766f 6361 620a 2020 2020 2020 2020 7265  vocab.        re
-00012200: 7475 726e 204e 6f6e 650a 0a20 2020 2040  turn None..    @
-00012210: 766f 6361 622e 7365 7474 6572 0a20 2020  vocab.setter.   
-00012220: 2064 6566 2076 6f63 6162 2873 656c 662c   def vocab(self,
-00012230: 2076 6f63 6162 293a 0a20 2020 2020 2020   vocab):.       
-00012240: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00012250: 7261 6d20 7265 7475 726e 6e2e 6461 7461  ram returnn.data
-00012260: 7365 7473 2e75 7469 6c2e 766f 6361 6275  sets.util.vocabu
-00012270: 6c61 7279 2e56 6f63 6162 756c 6172 797c  lary.Vocabulary|
-00012280: 4e6f 6e65 2076 6f63 6162 3a0a 2020 2020  None vocab:.    
-00012290: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000122a0: 6966 2076 6f63 6162 2069 7320 7365 6c66  if vocab is self
-000122b0: 2e76 6f63 6162 3a0a 2020 2020 2020 2020  .vocab:.        
-000122c0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-000122d0: 2020 2069 6620 7365 6c66 2e73 616d 655f     if self.same_
-000122e0: 6173 3a0a 2020 2020 2020 2020 2020 2020  as:.            
-000122f0: 7365 6c66 2e67 6574 5f73 616d 655f 6261  self.get_same_ba
-00012300: 7365 2829 2e76 6f63 6162 203d 2076 6f63  se().vocab = voc
-00012310: 6162 0a20 2020 2020 2020 2020 2020 2072  ab.            r
-00012320: 6574 7572 6e0a 2020 2020 2020 2020 6578  eturn.        ex
-00012330: 7472 6120 3d20 7365 6c66 2e5f 6765 745f  tra = self._get_
-00012340: 7361 6d65 5f62 6173 655f 6578 7472 6128  same_base_extra(
-00012350: 290a 2020 2020 2020 2020 6966 2065 7874  ).        if ext
-00012360: 7261 3a0a 2020 2020 2020 2020 2020 2020  ra:.            
-00012370: 6578 7472 612e 766f 6361 6220 3d20 766f  extra.vocab = vo
-00012380: 6361 620a 0a20 2020 2023 2054 6865 206b  cab..    # The k
-00012390: 696e 6420 6f66 206f 7065 7261 7469 6f6e  ind of operation
-000123a0: 7320 7765 2068 6176 653a 0a20 2020 2023  s we have:.    #
-000123b0: 2061 202b 2062 3a20 7061 6464 696e 672c   a + b: padding,
-000123c0: 2063 6f6e 6361 740a 2020 2020 2320 6120   concat.    # a 
-000123d0: 2d20 623a 2077 696e 646f 7720 7769 7468  - b: window with
-000123e0: 2076 616c 6964 2066 7261 6d65 7320 6f6e   valid frames on
-000123f0: 6c79 0a20 2020 2023 2061 202a 2062 3a20  ly.    # a * b: 
-00012400: 6d65 7267 6520 6469 6d73 2c20 7570 7361  merge dims, upsa
-00012410: 6d70 6c65 2c20 7472 616e 7370 6f73 6564  mple, transposed
-00012420: 2063 6f6e 7620 7769 7468 2073 7472 6964   conv with strid
-00012430: 696e 670a 2020 2020 2320 6120 2f20 6220  ing.    # a / b 
-00012440: 2877 6865 6e20 6120 2520 6220 3d3d 2030  (when a % b == 0
-00012450: 293a 2073 706c 6974 2064 696d 732c 2064  ): split dims, d
-00012460: 6f77 6e73 616d 706c 652c 2063 6f6e 7620  ownsample, conv 
-00012470: 7769 7468 2073 7472 6964 696e 670a 2020  with striding.  
-00012480: 2020 2320 6365 696c 6469 7628 612c 2062    # ceildiv(a, b
-00012490: 293a 2063 6f6e 7620 7769 7468 2073 7472  ): conv with str
-000124a0: 6964 696e 670a 2020 2020 2320 6375 7374  iding.    # cust
-000124b0: 6f6d 3a20 7265 7065 6174 2c20 7265 6d6f  om: repeat, remo
-000124c0: 7665 2c20 6d61 736b 2c20 6c6f 6f70 2077  ve, mask, loop w
-000124d0: 6974 6820 6479 6e20 656e 640a 2020 2020  ith dyn end.    
-000124e0: 2320 4e6f 7465 2074 6861 7420 7765 2064  # Note that we d
-000124f0: 6966 6665 7265 6e74 6961 7465 2062 6574  ifferentiate bet
-00012500: 7765 656e 2074 6865 206f 7264 6572 2c20  ween the order, 
-00012510: 692e 652e 2061 202b 2062 2021 3d20 6220  i.e. a + b != b 
-00012520: 2b20 612e 0a20 2020 2023 204e 6f74 6520  + a..    # Note 
-00012530: 7468 6174 2077 6520 616c 7761 7973 2068  that we always h
-00012540: 6176 6520 7468 6520 6173 7375 6d70 7469  ave the assumpti
-00012550: 6f6e 2074 6861 7420 6120 6469 6d65 6e73  on that a dimens
-00012560: 696f 6e20 6973 206e 6f6e 2d6e 6567 6174  ion is non-negat
-00012570: 6976 652e 0a20 2020 2023 2054 6869 7320  ive..    # This 
-00012580: 6173 7375 6d70 7469 6f6e 2069 7320 6e65  assumption is ne
-00012590: 6365 7373 6172 7920 666f 7220 736f 6d65  cessary for some
-000125a0: 2073 696d 706c 6966 6963 6174 696f 6e73   simplifications
-000125b0: 2e0a 2020 2020 2320 6874 7470 733a 2f2f  ..    # https://
-000125c0: 6769 7468 7562 2e63 6f6d 2f72 7774 682d  github.com/rwth-
-000125d0: 6936 2f72 6574 7572 6e6e 2f70 756c 6c2f  i6/returnn/pull/
-000125e0: 3835 330a 0a20 2020 2064 6566 205f 5f61  853..    def __a
-000125f0: 6464 5f5f 2873 656c 663a 2044 696d 2c20  dd__(self: Dim, 
-00012600: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
-00012610: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
-00012620: 616d 2044 696d 7c69 6e74 206f 7468 6572  am Dim|int other
-00012630: 3a0a 2020 2020 2020 2020 3a72 6574 7572  :.        :retur
-00012640: 6e3a 2073 656c 6620 2b20 6f74 6865 722e  n: self + other.
-00012650: 206e 6f74 6520 7468 6174 2074 6869 7320   note that this 
-00012660: 6973 206e 6f74 2063 6f6d 6d75 7461 7469  is not commutati
-00012670: 7665 2c20 692e 652e 2064 6966 6665 7265  ve, i.e. differe
-00012680: 6e74 2066 726f 6d20 6f74 6865 7220 2b20  nt from other + 
-00012690: 7365 6c66 2e0a 2020 2020 2020 2020 3a72  self..        :r
-000126a0: 7479 7065 3a20 4469 6d0a 2020 2020 2020  type: Dim.      
-000126b0: 2020 2222 220a 2020 2020 2020 2020 7465    """.        te
-000126c0: 726d 203d 205f 4f70 4c69 6e65 6172 5465  rm = _OpLinearTe
-000126d0: 726d 2e66 726f 6d5f 6469 6d28 7365 6c66  rm.from_dim(self
-000126e0: 290a 2020 2020 2020 2020 7465 726d 2e65  ).        term.e
-000126f0: 7874 656e 645f 6164 645f 7375 625f 286f  xtend_add_sub_(o
-00012700: 7468 6572 2c20 6b69 6e64 3d22 6164 6422  ther, kind="add"
-00012710: 2c20 7269 6768 743d 5472 7565 290a 2020  , right=True).  
-00012720: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
-00012730: 6d2e 6173 5f64 696d 2829 0a0a 2020 2020  m.as_dim()..    
-00012740: 6465 6620 5f5f 7261 6464 5f5f 2873 656c  def __radd__(sel
-00012750: 663a 2044 696d 2c20 6f74 6865 7229 3a0a  f: Dim, other):.
-00012760: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00012770: 2020 2020 3a70 6172 616d 2044 696d 7c69      :param Dim|i
-00012780: 6e74 206f 7468 6572 3a0a 2020 2020 2020  nt other:.      
-00012790: 2020 3a72 6574 7572 6e3a 206f 7468 6572    :return: other
-000127a0: 202b 2073 656c 660a 2020 2020 2020 2020   + self.        
-000127b0: 3a72 7479 7065 3a20 4469 6d0a 2020 2020  :rtype: Dim.    
-000127c0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000127d0: 7465 726d 203d 205f 4f70 4c69 6e65 6172  term = _OpLinear
-000127e0: 5465 726d 2e66 726f 6d5f 6469 6d28 7365  Term.from_dim(se
-000127f0: 6c66 290a 2020 2020 2020 2020 7465 726d  lf).        term
-00012800: 2e65 7874 656e 645f 6164 645f 7375 625f  .extend_add_sub_
-00012810: 286f 7468 6572 2c20 6b69 6e64 3d22 6164  (other, kind="ad
-00012820: 6422 2c20 7269 6768 743d 4661 6c73 6529  d", right=False)
-00012830: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00012840: 7465 726d 2e61 735f 6469 6d28 290a 0a20  term.as_dim().. 
-00012850: 2020 2064 6566 205f 5f73 7562 5f5f 2873     def __sub__(s
-00012860: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
-00012870: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012880: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
-00012890: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-000128a0: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
-000128b0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-000128c0: 6574 7572 6e20 7365 6c66 2e73 7562 5f72  eturn self.sub_r
-000128d0: 6967 6874 286f 7468 6572 290a 0a20 2020  ight(other)..   
-000128e0: 2064 6566 2073 7562 5f72 6967 6874 2873   def sub_right(s
-000128f0: 656c 663a 2044 696d 2c20 6f74 6865 7229  elf: Dim, other)
-00012900: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00012910: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
-00012920: 7c69 6e74 206f 7468 6572 3a0a 2020 2020  |int other:.    
-00012930: 2020 2020 3a72 6574 7572 6e3a 2073 656c      :return: sel
-00012940: 6620 2d20 6f74 6865 720a 2020 2020 2020  f - other.      
-00012950: 2020 3a72 7479 7065 3a20 4469 6d0a 2020    :rtype: Dim.  
-00012960: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00012970: 2020 7465 726d 203d 205f 4f70 4c69 6e65    term = _OpLine
-00012980: 6172 5465 726d 2e66 726f 6d5f 6469 6d28  arTerm.from_dim(
-00012990: 7365 6c66 290a 2020 2020 2020 2020 7465  self).        te
-000129a0: 726d 2e65 7874 656e 645f 6164 645f 7375  rm.extend_add_su
-000129b0: 625f 286f 7468 6572 2c20 6b69 6e64 3d22  b_(other, kind="
-000129c0: 7375 6222 2c20 7269 6768 743d 5472 7565  sub", right=True
-000129d0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
-000129e0: 2074 6572 6d2e 6173 5f64 696d 2829 0a0a   term.as_dim()..
-000129f0: 2020 2020 6465 6620 7375 625f 6c65 6674      def sub_left
-00012a00: 2873 656c 663a 2044 696d 2c20 6f74 6865  (self: Dim, othe
-00012a10: 7229 3a0a 2020 2020 2020 2020 2222 220a  r):.        """.
-00012a20: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
-00012a30: 696d 7c69 6e74 206f 7468 6572 3a0a 2020  im|int other:.  
-00012a40: 2020 2020 2020 3a72 6574 7572 6e3a 2028        :return: (
-00012a50: 2d6f 7468 6572 2920 2b20 7365 6c66 0a20  -other) + self. 
-00012a60: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-00012a70: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
-00012a80: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
-00012a90: 704c 696e 6561 7254 6572 6d2e 6672 6f6d  pLinearTerm.from
-00012aa0: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
-00012ab0: 2020 2074 6572 6d2e 6578 7465 6e64 5f61     term.extend_a
-00012ac0: 6464 5f73 7562 5f28 6f74 6865 722c 206b  dd_sub_(other, k
-00012ad0: 696e 643d 2273 7562 222c 2072 6967 6874  ind="sub", right
-00012ae0: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-00012af0: 7265 7475 726e 2074 6572 6d2e 6173 5f64  return term.as_d
-00012b00: 696d 2829 0a0a 2020 2020 6465 6620 5f5f  im()..    def __
-00012b10: 6d75 6c5f 5f28 7365 6c66 3a20 4469 6d2c  mul__(self: Dim,
-00012b20: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-00012b30: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00012b40: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
-00012b50: 723a 0a20 2020 2020 2020 203a 7274 7970  r:.        :rtyp
-00012b60: 653a 2044 696d 0a20 2020 2020 2020 2022  e: Dim.        "
-00012b70: 2222 0a20 2020 2020 2020 2074 6572 6d20  "".        term 
-00012b80: 3d20 5f4f 704c 696e 6561 7254 6572 6d2e  = _OpLinearTerm.
-00012b90: 6672 6f6d 5f64 696d 2873 656c 6629 0a20  from_dim(self). 
-00012ba0: 2020 2020 2020 2074 6572 6d2e 6578 7465         term.exte
-00012bb0: 6e64 5f6d 756c 5f64 6976 5f28 6f74 6865  nd_mul_div_(othe
-00012bc0: 722c 206b 696e 643d 226d 756c 222c 2072  r, kind="mul", r
-00012bd0: 6967 6874 3d54 7275 6529 0a20 2020 2020  ight=True).     
-00012be0: 2020 2072 6574 7572 6e20 7465 726d 2e61     return term.a
-00012bf0: 735f 6469 6d28 290a 0a20 2020 2064 6566  s_dim()..    def
-00012c00: 205f 5f72 6d75 6c5f 5f28 7365 6c66 3a20   __rmul__(self: 
-00012c10: 4469 6d2c 206f 7468 6572 293a 0a20 2020  Dim, other):.   
-00012c20: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012c30: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
-00012c40: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-00012c50: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
-00012c60: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
-00012c70: 6572 6d20 3d20 5f4f 704c 696e 6561 7254  erm = _OpLinearT
-00012c80: 6572 6d2e 6672 6f6d 5f64 696d 2873 656c  erm.from_dim(sel
-00012c90: 6629 0a20 2020 2020 2020 2074 6572 6d2e  f).        term.
-00012ca0: 6578 7465 6e64 5f6d 756c 5f64 6976 5f28  extend_mul_div_(
-00012cb0: 6f74 6865 722c 206b 696e 643d 226d 756c  other, kind="mul
-00012cc0: 222c 2072 6967 6874 3d46 616c 7365 290a  ", right=False).
-00012cd0: 2020 2020 2020 2020 7265 7475 726e 2074          return t
-00012ce0: 6572 6d2e 6173 5f64 696d 2829 0a0a 2020  erm.as_dim()..  
-00012cf0: 2020 6465 6620 5f5f 666c 6f6f 7264 6976    def __floordiv
-00012d00: 5f5f 2873 656c 663a 2044 696d 2c20 6f74  __(self: Dim, ot
-00012d10: 6865 7229 3a0a 2020 2020 2020 2020 2222  her):.        ""
-00012d20: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
-00012d30: 2044 696d 7c69 6e74 206f 7468 6572 3a0a   Dim|int other:.
-00012d40: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00012d50: 4469 6d0a 2020 2020 2020 2020 2222 220a  Dim.        """.
-00012d60: 2020 2020 2020 2020 7465 726d 203d 205f          term = _
-00012d70: 4f70 4c69 6e65 6172 5465 726d 2e66 726f  OpLinearTerm.fro
-00012d80: 6d5f 6469 6d28 7365 6c66 290a 2020 2020  m_dim(self).    
-00012d90: 2020 2020 7465 726d 2e65 7874 656e 645f      term.extend_
-00012da0: 6d75 6c5f 6469 765f 286f 7468 6572 2c20  mul_div_(other, 
-00012db0: 6b69 6e64 3d22 666c 6f6f 7264 6976 222c  kind="floordiv",
-00012dc0: 2072 6967 6874 3d54 7275 6529 0a20 2020   right=True).   
-00012dd0: 2020 2020 2072 6574 7572 6e20 7465 726d       return term
-00012de0: 2e61 735f 6469 6d28 290a 0a20 2020 2064  .as_dim()..    d
-00012df0: 6566 205f 5f74 7275 6564 6976 5f5f 2873  ef __truediv__(s
-00012e00: 656c 662c 206f 7468 6572 293a 0a20 2020  elf, other):.   
-00012e10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00012e20: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
-00012e30: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-00012e40: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
-00012e50: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00012e60: 6574 7572 6e20 7365 6c66 2e64 6976 5f72  eturn self.div_r
-00012e70: 6967 6874 286f 7468 6572 290a 0a20 2020  ight(other)..   
-00012e80: 2064 6566 2064 6976 5f6c 6566 7428 7365   def div_left(se
-00012e90: 6c66 3a20 4469 6d2c 206f 7468 6572 293a  lf: Dim, other):
-00012ea0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00012eb0: 2020 2020 203a 7061 7261 6d20 4469 6d7c       :param Dim|
-00012ec0: 696e 7420 6f74 6865 723a 0a20 2020 2020  int other:.     
-00012ed0: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
-00012ee0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00012ef0: 2020 2074 6572 6d20 3d20 5f4f 704c 696e     term = _OpLin
-00012f00: 6561 7254 6572 6d2e 6672 6f6d 5f64 696d  earTerm.from_dim
-00012f10: 2873 656c 6629 0a20 2020 2020 2020 2074  (self).        t
-00012f20: 6572 6d2e 6578 7465 6e64 5f6d 756c 5f64  erm.extend_mul_d
-00012f30: 6976 5f28 6f74 6865 722c 206b 696e 643d  iv_(other, kind=
-00012f40: 2274 7275 6564 6976 222c 2072 6967 6874  "truediv", right
-00012f50: 3d46 616c 7365 290a 2020 2020 2020 2020  =False).        
-00012f60: 7265 7475 726e 2074 6572 6d2e 6173 5f64  return term.as_d
-00012f70: 696d 2829 0a0a 2020 2020 6465 6620 6469  im()..    def di
-00012f80: 765f 7269 6768 7428 7365 6c66 3a20 4469  v_right(self: Di
-00012f90: 6d2c 206f 7468 6572 293a 0a20 2020 2020  m, other):.     
-00012fa0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-00012fb0: 7061 7261 6d20 4469 6d7c 696e 7420 6f74  param Dim|int ot
-00012fc0: 6865 723a 0a20 2020 2020 2020 203a 7274  her:.        :rt
-00012fd0: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
-00012fe0: 2022 2222 0a20 2020 2020 2020 2074 6572   """.        ter
-00012ff0: 6d20 3d20 5f4f 704c 696e 6561 7254 6572  m = _OpLinearTer
-00013000: 6d2e 6672 6f6d 5f64 696d 2873 656c 6629  m.from_dim(self)
-00013010: 0a20 2020 2020 2020 2074 6572 6d2e 6578  .        term.ex
-00013020: 7465 6e64 5f6d 756c 5f64 6976 5f28 6f74  tend_mul_div_(ot
-00013030: 6865 722c 206b 696e 643d 2274 7275 6564  her, kind="trued
-00013040: 6976 222c 2072 6967 6874 3d54 7275 6529  iv", right=True)
-00013050: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013060: 7465 726d 2e61 735f 6469 6d28 290a 0a20  term.as_dim().. 
-00013070: 2020 2064 6566 2063 6569 6c64 6976 5f6c     def ceildiv_l
-00013080: 6566 7428 7365 6c66 3a20 4469 6d2c 206f  eft(self: Dim, o
-00013090: 7468 6572 293a 0a20 2020 2020 2020 2022  ther):.        "
-000130a0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-000130b0: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
-000130c0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
-000130d0: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
-000130e0: 0a20 2020 2020 2020 2074 6572 6d20 3d20  .        term = 
-000130f0: 5f4f 704c 696e 6561 7254 6572 6d2e 6672  _OpLinearTerm.fr
-00013100: 6f6d 5f64 696d 2873 656c 6629 0a20 2020  om_dim(self).   
-00013110: 2020 2020 2074 6572 6d2e 6578 7465 6e64       term.extend
-00013120: 5f6d 756c 5f64 6976 5f28 6f74 6865 722c  _mul_div_(other,
-00013130: 206b 696e 643d 2263 6569 6c64 6976 222c   kind="ceildiv",
-00013140: 2072 6967 6874 3d46 616c 7365 290a 2020   right=False).  
-00013150: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
-00013160: 6d2e 6173 5f64 696d 2829 0a0a 2020 2020  m.as_dim()..    
-00013170: 6465 6620 6365 696c 6469 765f 7269 6768  def ceildiv_righ
-00013180: 7428 7365 6c66 3a20 4469 6d2c 206f 7468  t(self: Dim, oth
-00013190: 6572 293a 0a20 2020 2020 2020 2022 2222  er):.        """
-000131a0: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000131b0: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
-000131c0: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-000131d0: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
-000131e0: 2020 2020 2020 2074 6572 6d20 3d20 5f4f         term = _O
-000131f0: 704c 696e 6561 7254 6572 6d2e 6672 6f6d  pLinearTerm.from
-00013200: 5f64 696d 2873 656c 6629 0a20 2020 2020  _dim(self).     
-00013210: 2020 2074 6572 6d2e 6578 7465 6e64 5f6d     term.extend_m
-00013220: 756c 5f64 6976 5f28 6f74 6865 722c 206b  ul_div_(other, k
-00013230: 696e 643d 2263 6569 6c64 6976 222c 2072  ind="ceildiv", r
-00013240: 6967 6874 3d54 7275 6529 0a20 2020 2020  ight=True).     
-00013250: 2020 2072 6574 7572 6e20 7465 726d 2e61     return term.a
-00013260: 735f 6469 6d28 290a 0a20 2020 2064 6566  s_dim()..    def
-00013270: 205f 5f6e 6567 5f5f 2873 656c 6629 3a0a   __neg__(self):.
-00013280: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013290: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
-000132a0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-000132b0: 2020 2020 7265 7475 726e 202d 3120 2a20      return -1 * 
-000132c0: 7365 6c66 0a0a 2020 2020 6465 6620 6973  self..    def is
-000132d0: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
-000132e0: 5f64 696d 2873 656c 6629 202d 3e20 626f  _dim(self) -> bo
-000132f0: 6f6c 3a0a 2020 2020 2020 2020 2222 220a  ol:.        """.
-00013300: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
-00013310: 2064 6572 6976 6564 206f 7020 6f66 2074   derived op of t
-00013320: 7970 6520 636f 6e73 7461 6e74 0a20 2020  ype constant.   
-00013330: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00013340: 2072 6574 7572 6e20 7365 6c66 2e64 6572   return self.der
-00013350: 6976 6564 5f66 726f 6d5f 6f70 2061 6e64  ived_from_op and
-00013360: 2073 656c 662e 6465 7269 7665 645f 6672   self.derived_fr
-00013370: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 2263  om_op.kind == "c
-00013380: 6f6e 7374 616e 7422 0a0a 0a64 6566 205f  onstant"...def _
-00013390: 6d61 6b65 5f63 6f6e 7374 616e 745f 7374  make_constant_st
-000133a0: 6174 6963 5f64 696d 2876 616c 7565 2c20  atic_dim(value, 
-000133b0: 6b69 6e64 3d4e 6f6e 6529 3a0a 2020 2020  kind=None):.    
-000133c0: 2222 220a 2020 2020 3a70 6172 616d 2069  """.    :param i
-000133d0: 6e74 2076 616c 7565 3a0a 2020 2020 3a70  nt value:.    :p
-000133e0: 6172 616d 2045 6e74 6974 797c 4e6f 6e65  aram Entity|None
-000133f0: 206b 696e 643a 0a20 2020 203a 7274 7970   kind:.    :rtyp
-00013400: 653a 2044 696d 0a20 2020 2022 2222 0a20  e: Dim.    """. 
-00013410: 2020 2072 6574 7572 6e20 5f64 2e44 696d     return _d.Dim
-00013420: 280a 2020 2020 2020 2020 6469 6d65 6e73  (.        dimens
-00013430: 696f 6e3d 7661 6c75 652c 0a20 2020 2020  ion=value,.     
-00013440: 2020 206b 696e 643d 6b69 6e64 206f 7220     kind=kind or 
-00013450: 4469 6d54 7970 6573 2e55 6e73 7065 6369  DimTypes.Unspeci
-00013460: 6669 6564 2c0a 2020 2020 2020 2020 6465  fied,.        de
-00013470: 7363 7269 7074 696f 6e3d 2275 6e6e 616d  scription="unnam
-00013480: 6564 5f25 7364 696d 5f25 6922 2025 2028  ed_%sdim_%i" % (
-00013490: 6b69 6e64 2e6e 616d 6520 2b20 225f 2220  kind.name + "_" 
-000134a0: 6966 206b 696e 6420 656c 7365 2022 222c  if kind else "",
-000134b0: 2076 616c 7565 292c 0a20 2020 2020 2020   value),.       
-000134c0: 2064 6572 6976 6564 5f66 726f 6d5f 6f70   derived_from_op
-000134d0: 3d4f 7028 6b69 6e64 3d22 636f 6e73 7461  =Op(kind="consta
-000134e0: 6e74 222c 2069 6e70 7574 733d 5b5d 2c20  nt", inputs=[], 
-000134f0: 6174 7472 6962 733d 7b22 7661 6c75 6522  attribs={"value"
-00013500: 3a20 7661 6c75 657d 292c 0a20 2020 2020  : value}),.     
-00013510: 2020 2061 7574 6f5f 6765 6e65 7261 7465     auto_generate
-00013520: 643d 5472 7565 2c0a 2020 2020 290a 0a0a  d=True,.    )...
-00013530: 636c 6173 7320 4f70 3a0a 2020 2020 2222  class Op:.    ""
-00013540: 220a 2020 2020 4f70 206f 6e20 3a63 6c61  ".    Op on :cla
-00013550: 7373 3a60 4469 6d60 2077 6869 6368 2072  ss:`Dim` which r
-00013560: 6573 756c 7473 2069 6e20 6120 6465 7269  esults in a deri
-00013570: 7665 6420 3a63 6c61 7373 3a60 4469 6d60  ved :class:`Dim`
-00013580: 2e0a 2020 2020 2222 220a 0a20 2020 2064  ..    """..    d
-00013590: 6566 205f 5f69 6e69 745f 5f28 7365 6c66  ef __init__(self
-000135a0: 2c20 6b69 6e64 2c20 696e 7075 7473 2c20  , kind, inputs, 
-000135b0: 6174 7472 6962 733d 4e6f 6e65 293a 0a20  attribs=None):. 
-000135c0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000135d0: 2020 203a 7061 7261 6d20 7374 7220 6b69     :param str ki
-000135e0: 6e64 3a20 2261 6464 222c 2022 7375 6222  nd: "add", "sub"
-000135f0: 2c20 226d 756c 222c 2022 6365 696c 6469  , "mul", "ceildi
-00013600: 7622 0a20 2020 2020 2020 203a 7061 7261  v".        :para
-00013610: 6d20 6c69 7374 5b44 696d 5d20 696e 7075  m list[Dim] inpu
-00013620: 7473 3a0a 2020 2020 2020 2020 3a70 6172  ts:.        :par
-00013630: 616d 2064 6963 745b 7374 725d 7c4e 6f6e  am dict[str]|Non
-00013640: 6520 6174 7472 6962 733a 0a20 2020 2020  e attribs:.     
-00013650: 2020 2022 2222 0a20 2020 2020 2020 2073     """.        s
-00013660: 656c 662e 6b69 6e64 203d 206b 696e 640a  elf.kind = kind.
-00013670: 2020 2020 2020 2020 7365 6c66 2e69 6e70          self.inp
-00013680: 7574 7320 3d20 696e 7075 7473 0a20 2020  uts = inputs.   
-00013690: 2020 2020 2073 656c 662e 6f75 7470 7574       self.output
-000136a0: 203d 204e 6f6e 6520 2023 2074 7970 653a   = None  # type:
-000136b0: 204f 7074 696f 6e61 6c5b 5f64 2e44 696d   Optional[_d.Dim
-000136c0: 5d0a 2020 2020 2020 2020 7365 6c66 2e61  ].        self.a
-000136d0: 7474 7269 6273 203d 2061 7474 7269 6273  ttribs = attribs
-000136e0: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
-000136f0: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
-00013700: 2020 6174 7472 6962 7320 3d20 2822 2025    attribs = (" %
-00013710: 7222 2025 2073 656c 662e 6174 7472 6962  r" % self.attrib
-00013720: 7329 2069 6620 7365 6c66 2e61 7474 7269  s) if self.attri
-00013730: 6273 2065 6c73 6520 2222 0a20 2020 2020  bs else "".     
-00013740: 2020 2072 6574 7572 6e20 223c 4469 6d2e     return "<Dim.
-00013750: 4f70 2025 7220 2573 2573 3e22 2025 2028  Op %r %s%s>" % (
-00013760: 7365 6c66 2e6b 696e 642c 2073 656c 662e  self.kind, self.
-00013770: 696e 7075 7473 2c20 6174 7472 6962 7329  inputs, attribs)
-00013780: 0a0a 2020 2020 6465 6620 5f76 616c 7565  ..    def _value
-00013790: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
-000137a0: 7265 7475 726e 2073 656c 662e 6b69 6e64  return self.kind
-000137b0: 2c20 7475 706c 6528 7365 6c66 2e69 6e70  , tuple(self.inp
-000137c0: 7574 7329 2c20 6672 6f7a 656e 7365 7428  uts), frozenset(
-000137d0: 7365 6c66 2e61 7474 7269 6273 2e69 7465  self.attribs.ite
-000137e0: 6d73 2829 2920 6966 2073 656c 662e 6174  ms()) if self.at
-000137f0: 7472 6962 7320 656c 7365 204e 6f6e 650a  tribs else None.
-00013800: 0a20 2020 2064 6566 205f 5f68 6173 685f  .    def __hash_
-00013810: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
-00013820: 2072 6574 7572 6e20 6861 7368 2873 656c   return hash(sel
-00013830: 662e 5f76 616c 7565 2829 290a 0a20 2020  f._value())..   
-00013840: 2064 6566 205f 5f65 715f 5f28 7365 6c66   def __eq__(self
-00013850: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
-00013860: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00013870: 6f74 6865 722c 204f 7029 3a0a 2020 2020  other, Op):.    
-00013880: 2020 2020 2020 2020 7265 7475 726e 2073          return s
-00013890: 656c 662e 5f76 616c 7565 2829 203d 3d20  elf._value() == 
-000138a0: 6f74 6865 722e 5f76 616c 7565 2829 0a20  other._value(). 
-000138b0: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-000138c0: 6c73 650a 0a20 2020 2064 6566 205f 5f6e  lse..    def __n
-000138d0: 655f 5f28 7365 6c66 2c20 6f74 6865 7229  e__(self, other)
-000138e0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
-000138f0: 206e 6f74 2073 656c 662e 5f5f 6571 5f5f   not self.__eq__
-00013900: 286f 7468 6572 290a 0a0a 6465 6620 5f67  (other)...def _g
-00013910: 6574 5f64 6573 6372 6970 7469 6f6e 2864  et_description(d
-00013920: 696d 2c20 6272 6163 6b65 7473 3d54 7275  im, brackets=Tru
-00013930: 6529 3a0a 2020 2020 2222 220a 2020 2020  e):.    """.    
-00013940: 3a70 6172 616d 2044 696d 2064 696d 3a0a  :param Dim dim:.
-00013950: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
-00013960: 6272 6163 6b65 7473 3a20 6164 6420 6272  brackets: add br
-00013970: 6163 6b65 7473 2077 6865 6e20 6e65 6365  ackets when nece
-00013980: 7373 6172 790a 2020 2020 3a72 7479 7065  ssary.    :rtype
-00013990: 3a20 7374 720a 2020 2020 2222 220a 2020  : str.    """.  
-000139a0: 2020 6966 2064 696d 2e64 6573 6372 6970    if dim.descrip
-000139b0: 7469 6f6e 2061 6e64 2064 696d 2e64 6573  tion and dim.des
-000139c0: 6372 6970 7469 6f6e 2e73 7461 7274 7377  cription.startsw
-000139d0: 6974 6828 2275 6e6e 616d 6564 5f22 2920  ith("unnamed_") 
-000139e0: 616e 6420 6469 6d2e 6469 6d65 6e73 696f  and dim.dimensio
-000139f0: 6e20 6973 206e 6f74 204e 6f6e 653a 0a20  n is not None:. 
-00013a00: 2020 2020 2020 2072 6574 7572 6e20 7374         return st
-00013a10: 7228 6469 6d2e 6469 6d65 6e73 696f 6e29  r(dim.dimension)
-00013a20: 0a20 2020 2069 6620 6469 6d2e 6465 7363  .    if dim.desc
-00013a30: 7269 7074 696f 6e3a 0a20 2020 2020 2020  ription:.       
-00013a40: 2069 6620 6272 6163 6b65 7473 3a0a 2020   if brackets:.  
-00013a50: 2020 2020 2020 2020 2020 696d 706f 7274            import
-00013a60: 2072 650a 0a20 2020 2020 2020 2020 2020   re..           
-00013a70: 2069 6620 7265 2e73 6561 7263 6828 225b   if re.search("[
-00013a80: 2b5c 5c2d 2f20 5d22 2c20 6469 6d2e 6465  +\\-/ ]", dim.de
-00013a90: 7363 7269 7074 696f 6e29 3a0a 2020 2020  scription):.    
-00013aa0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00013ab0: 726e 2022 2825 7329 2220 2520 6469 6d2e  rn "(%s)" % dim.
-00013ac0: 6465 7363 7269 7074 696f 6e0a 2020 2020  description.    
-00013ad0: 2020 2020 7265 7475 726e 2064 696d 2e64      return dim.d
-00013ae0: 6573 6372 6970 7469 6f6e 0a20 2020 2072  escription.    r
-00013af0: 6574 7572 6e20 2275 6e6e 616d 6564 5f25  eturn "unnamed_%
-00013b00: 735f 6469 6d25 7322 2025 2028 6469 6d2e  s_dim%s" % (dim.
-00013b10: 6b69 6e64 2c20 6469 6d2e 6469 6d65 6e73  kind, dim.dimens
-00013b20: 696f 6e20 6966 2064 696d 2e64 696d 656e  ion if dim.dimen
-00013b30: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
-00013b40: 2065 6c73 6520 223f 2229 0a0a 0a63 6c61   else "?")...cla
-00013b50: 7373 205f 4f70 4d75 6c74 5465 726d 3a0a  ss _OpMultTerm:.
-00013b60: 2020 2020 2222 220a 2020 2020 7265 7072      """.    repr
-00013b70: 6573 656e 7473 2073 7468 206c 696b 6520  esents sth like 
-00013b80: 6120 2a20 6220 2a20 630a 2020 2020 2222  a * b * c.    ""
-00013b90: 220a 0a20 2020 2040 636c 6173 736d 6574  "..    @classmet
-00013ba0: 686f 640a 2020 2020 6465 6620 6672 6f6d  hod.    def from
-00013bb0: 5f64 696d 2863 6c73 2c20 6469 6d3a 205f  _dim(cls, dim: _
-00013bc0: 642e 4469 6d29 202d 3e20 5f4f 704d 756c  d.Dim) -> _OpMul
-00013bd0: 7454 6572 6d3a 0a20 2020 2020 2020 2022  tTerm:.        "
-00013be0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-00013bf0: 6d20 6469 6d3a 0a20 2020 2020 2020 203a  m dim:.        :
-00013c00: 7265 7475 726e 3a20 6f70 206d 756c 7420  return: op mult 
-00013c10: 7465 726d 0a20 2020 2020 2020 2022 2222  term.        """
-00013c20: 0a20 2020 2020 2020 2064 696d 203d 2064  .        dim = d
-00013c30: 696d 2e67 6574 5f73 616d 655f 6261 7365  im.get_same_base
-00013c40: 2829 0a20 2020 2020 2020 2069 6620 6469  ().        if di
-00013c50: 6d2e 6469 6d65 6e73 696f 6e20 3d3d 2031  m.dimension == 1
-00013c60: 2061 6e64 2064 696d 2e69 735f 636f 6e73   and dim.is_cons
-00013c70: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
-00013c80: 293a 0a20 2020 2020 2020 2020 2020 2072  ):.            r
-00013c90: 6574 7572 6e20 636c 732e 6f6e 6528 290a  eturn cls.one().
-00013ca0: 2020 2020 2020 2020 6966 2064 696d 2e64          if dim.d
-00013cb0: 6572 6976 6564 5f66 726f 6d5f 6f70 2061  erived_from_op a
-00013cc0: 6e64 2064 696d 2e64 6572 6976 6564 5f66  nd dim.derived_f
-00013cd0: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 2022  rom_op.kind == "
-00013ce0: 6d75 6c22 3a0a 2020 2020 2020 2020 2020  mul":.          
-00013cf0: 2020 7265 7475 726e 2063 6c73 286c 6973    return cls(lis
-00013d00: 7428 6469 6d2e 6465 7269 7665 645f 6672  t(dim.derived_fr
-00013d10: 6f6d 5f6f 702e 696e 7075 7473 2929 0a20  om_op.inputs)). 
-00013d20: 2020 2020 2020 2072 6574 7572 6e20 636c         return cl
-00013d30: 7328 5b64 696d 5d29 0a0a 2020 2020 4063  s([dim])..    @c
-00013d40: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
-00013d50: 6566 2066 726f 6d5f 6469 6d5f 6661 6374  ef from_dim_fact
-00013d60: 6f72 7328 636c 732c 2064 696d 7329 3a0a  ors(cls, dims):.
-00013d70: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00013d80: 2020 2020 3a70 6172 616d 206c 6973 745b      :param list[
-00013d90: 4469 6d5d 2064 696d 733a 0a20 2020 2020  Dim] dims:.     
-00013da0: 2020 203a 7274 7970 653a 2044 696d 2e5f     :rtype: Dim._
-00013db0: 4f70 4d75 6c74 5465 726d 0a20 2020 2020  OpMultTerm.     
-00013dc0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00013dd0: 6573 203d 2063 6c73 2e6f 6e65 2829 0a20  es = cls.one(). 
-00013de0: 2020 2020 2020 2066 6f72 2064 2069 6e20         for d in 
-00013df0: 6469 6d73 3a0a 2020 2020 2020 2020 2020  dims:.          
-00013e00: 2020 7265 732e 6578 7465 6e64 5f6d 756c    res.extend_mul
-00013e10: 5f64 6976 5f28 642c 206b 696e 643d 226d  _div_(d, kind="m
-00013e20: 756c 222c 2072 6967 6874 3d54 7275 6529  ul", right=True)
-00013e30: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00013e40: 7265 730a 0a20 2020 2040 636c 6173 736d  res..    @classm
-00013e50: 6574 686f 640a 2020 2020 6465 6620 6f6e  ethod.    def on
-00013e60: 6528 636c 7329 3a0a 2020 2020 2020 2020  e(cls):.        
-00013e70: 2222 220a 2020 2020 2020 2020 3a72 7479  """.        :rty
-00013e80: 7065 3a20 4469 6d2e 5f4f 704d 756c 7454  pe: Dim._OpMultT
-00013e90: 6572 6d0a 2020 2020 2020 2020 2222 220a  erm.        """.
-00013ea0: 2020 2020 2020 2020 7265 7475 726e 2063          return c
-00013eb0: 6c73 285b 5d29 0a0a 2020 2020 6465 6620  ls([])..    def 
-00013ec0: 5f5f 696e 6974 5f5f 2873 656c 662c 2074  __init__(self, t
-00013ed0: 6572 6d73 293a 0a20 2020 2020 2020 2022  erms):.        "
-00013ee0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
-00013ef0: 6d20 6c69 7374 5b44 696d 5d20 7465 726d  m list[Dim] term
-00013f00: 733a 0a20 2020 2020 2020 2022 2222 0a20  s:.        """. 
-00013f10: 2020 2020 2020 2073 656c 662e 7465 726d         self.term
-00013f20: 7320 3d20 7465 726d 730a 0a20 2020 2064  s = terms..    d
-00013f30: 6566 205f 5f68 6173 685f 5f28 7365 6c66  ef __hash__(self
-00013f40: 293a 0a20 2020 2020 2020 2072 6574 7572  ):.        retur
-00013f50: 6e20 6861 7368 2874 7570 6c65 2873 656c  n hash(tuple(sel
-00013f60: 662e 7465 726d 7329 290a 0a20 2020 2064  f.terms))..    d
-00013f70: 6566 205f 5f65 715f 5f28 7365 6c66 2c20  ef __eq__(self, 
-00013f80: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
-00013f90: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
-00013fa0: 616d 2044 696d 7c44 696d 2e5f 4f70 4d75  am Dim|Dim._OpMu
-00013fb0: 6c74 5465 726d 206f 7468 6572 3a0a 2020  ltTerm other:.  
-00013fc0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
-00013fd0: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00013fe0: 6f74 6865 722c 205f 4f70 4d75 6c74 5465  other, _OpMultTe
-00013ff0: 726d 293a 0a20 2020 2020 2020 2020 2020  rm):.           
-00014000: 2072 6574 7572 6e20 7365 6c66 2e74 6572   return self.ter
-00014010: 6d73 203d 3d20 6f74 6865 722e 7465 726d  ms == other.term
-00014020: 730a 2020 2020 2020 2020 7265 7475 726e  s.        return
-00014030: 2046 616c 7365 0a0a 2020 2020 6465 6620   False..    def 
-00014040: 5f5f 6e65 5f5f 2873 656c 662c 206f 7468  __ne__(self, oth
-00014050: 6572 293a 0a20 2020 2020 2020 2072 6574  er):.        ret
-00014060: 7572 6e20 6e6f 7420 7365 6c66 2e5f 5f65  urn not self.__e
-00014070: 715f 5f28 6f74 6865 7229 0a0a 2020 2020  q__(other)..    
-00014080: 6465 6620 5f5f 7265 7072 5f5f 2873 656c  def __repr__(sel
-00014090: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-000140a0: 726e 2022 4469 6d2e 5f4f 704d 756c 7454  rn "Dim._OpMultT
-000140b0: 6572 6d28 2572 2922 2025 2028 7365 6c66  erm(%r)" % (self
-000140c0: 2e74 6572 6d73 2c29 0a0a 2020 2020 4070  .terms,)..    @p
-000140d0: 726f 7065 7274 790a 2020 2020 6465 6620  roperty.    def 
-000140e0: 6469 6d65 6e73 696f 6e28 7365 6c66 293a  dimension(self):
-000140f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00014100: 2020 2020 203a 7274 7970 653a 2069 6e74       :rtype: int
-00014110: 7c4e 6f6e 650a 2020 2020 2020 2020 2222  |None.        ""
-00014120: 220a 2020 2020 2020 2020 6469 6d20 3d20  ".        dim = 
-00014130: 310a 2020 2020 2020 2020 666f 7220 7061  1.        for pa
-00014140: 7274 2069 6e20 7365 6c66 2e74 6572 6d73  rt in self.terms
-00014150: 3a0a 2020 2020 2020 2020 2020 2020 6966  :.            if
-00014160: 2070 6172 742e 6469 6d65 6e73 696f 6e20   part.dimension 
-00014170: 6973 204e 6f6e 653a 0a20 2020 2020 2020  is None:.       
-00014180: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-00014190: 4e6f 6e65 0a20 2020 2020 2020 2020 2020  None.           
-000141a0: 2064 696d 202a 3d20 7061 7274 2e64 696d   dim *= part.dim
-000141b0: 656e 7369 6f6e 0a20 2020 2020 2020 2072  ension.        r
-000141c0: 6574 7572 6e20 6469 6d0a 0a20 2020 2064  eturn dim..    d
-000141d0: 6566 2062 6173 655f 7465 726d 2873 656c  ef base_term(sel
-000141e0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-000141f0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-00014200: 4469 6d0a 2020 2020 2020 2020 2222 220a  Dim.        """.
-00014210: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
-00014220: 656c 662e 7465 726d 730a 2020 2020 2020  elf.terms.      
-00014230: 2020 7265 7475 726e 2073 656c 662e 7465    return self.te
-00014240: 726d 735b 2d31 5d0a 0a20 2020 2064 6566  rms[-1]..    def
-00014250: 2069 735f 6f6e 6528 7365 6c66 293a 0a20   is_one(self):. 
-00014260: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00014270: 2020 203a 7274 7970 653a 2062 6f6f 6c0a     :rtype: bool.
-00014280: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00014290: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
-000142a0: 656c 662e 7465 726d 730a 0a20 2020 2064  elf.terms..    d
-000142b0: 6566 2069 735f 636f 6e73 7461 6e74 5f73  ef is_constant_s
-000142c0: 7461 7469 635f 6469 6d28 7365 6c66 293a  tatic_dim(self):
-000142d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000142e0: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
-000142f0: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
-00014300: 2020 2020 2020 6966 206e 6f74 2073 656c        if not sel
-00014310: 662e 7465 726d 733a 0a20 2020 2020 2020  f.terms:.       
-00014320: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
-00014330: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00014340: 616c 6c28 7465 726d 2e69 735f 636f 6e73  all(term.is_cons
-00014350: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
-00014360: 2920 666f 7220 7465 726d 2069 6e20 7365  ) for term in se
-00014370: 6c66 2e74 6572 6d73 290a 0a20 2020 2064  lf.terms)..    d
-00014380: 6566 2063 6f70 7928 7365 6c66 293a 0a20  ef copy(self):. 
-00014390: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-000143a0: 2020 203a 7274 7970 653a 2044 696d 2e5f     :rtype: Dim._
-000143b0: 4f70 4d75 6c74 5465 726d 0a20 2020 2020  OpMultTerm.     
-000143c0: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-000143d0: 6574 7572 6e20 5f4f 704d 756c 7454 6572  eturn _OpMultTer
-000143e0: 6d28 6c69 7374 2873 656c 662e 7465 726d  m(list(self.term
-000143f0: 7329 290a 0a20 2020 2064 6566 206e 6567  s))..    def neg
-00014400: 6174 6976 6528 7365 6c66 293a 0a20 2020  ative(self):.   
-00014410: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
-00014420: 203a 7274 7970 653a 2044 696d 2e5f 4f70   :rtype: Dim._Op
-00014430: 4d75 6c74 5465 726d 0a20 2020 2020 2020  MultTerm.       
-00014440: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
-00014450: 7365 6c66 2e74 6572 6d73 2061 6e64 2073  self.terms and s
-00014460: 656c 662e 7465 726d 735b 305d 2e69 735f  elf.terms[0].is_
-00014470: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
-00014480: 6469 6d28 2920 616e 6420 7365 6c66 2e74  dim() and self.t
-00014490: 6572 6d73 5b30 5d2e 6469 6d65 6e73 696f  erms[0].dimensio
-000144a0: 6e20 3d3d 202d 313a 0a20 2020 2020 2020  n == -1:.       
-000144b0: 2020 2020 2072 6574 7572 6e20 5f4f 704d       return _OpM
-000144c0: 756c 7454 6572 6d28 7365 6c66 2e74 6572  ultTerm(self.ter
-000144d0: 6d73 5b31 3a5d 290a 2020 2020 2020 2020  ms[1:]).        
-000144e0: 7265 7320 3d20 7365 6c66 2e63 6f70 7928  res = self.copy(
-000144f0: 290a 2020 2020 2020 2020 7265 732e 6578  ).        res.ex
-00014500: 7465 6e64 5f6d 756c 5f64 6976 5f28 5f6d  tend_mul_div_(_m
-00014510: 616b 655f 636f 6e73 7461 6e74 5f73 7461  ake_constant_sta
-00014520: 7469 635f 6469 6d28 2d31 292c 206b 696e  tic_dim(-1), kin
-00014530: 643d 226d 756c 222c 2072 6967 6874 3d46  d="mul", right=F
-00014540: 616c 7365 290a 2020 2020 2020 2020 7265  alse).        re
-00014550: 7475 726e 2072 6573 0a0a 2020 2020 6465  turn res..    de
-00014560: 6620 6469 7669 7369 626c 6528 7365 6c66  f divisible(self
-00014570: 2c20 6f74 6865 722c 2072 6967 6874 293a  , other, right):
-00014580: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00014590: 2020 2020 203a 7061 7261 6d20 4469 6d20       :param Dim 
-000145a0: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
-000145b0: 7061 7261 6d20 626f 6f6c 2072 6967 6874  param bool right
-000145c0: 3a0a 2020 2020 2020 2020 3a72 6574 7572  :.        :retur
-000145d0: 6e3a 2077 6865 7468 6572 2077 6520 6361  n: whether we ca
-000145e0: 6e20 6469 7669 6465 206f 7468 6572 2c20  n divide other, 
-000145f0: 7769 7468 6f75 7420 7265 6d61 696e 6465  without remainde
-00014600: 720a 2020 2020 2020 2020 3a72 7479 7065  r.        :rtype
-00014610: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
-00014620: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
-00014630: 7420 7365 6c66 2e74 6572 6d73 3a0a 2020  t self.terms:.  
-00014640: 2020 2020 2020 2020 2020 7265 7475 726e            return
-00014650: 2046 616c 7365 0a20 2020 2020 2020 2069   False.        i
-00014660: 6620 6f74 6865 722e 6465 7269 7665 645f  f other.derived_
-00014670: 6672 6f6d 5f6f 7020 616e 6420 6f74 6865  from_op and othe
-00014680: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
-00014690: 702e 6b69 6e64 203d 3d20 226d 756c 223a  p.kind == "mul":
-000146a0: 0a20 2020 2020 2020 2020 2020 2074 6d70  .            tmp
-000146b0: 203d 2073 656c 662e 636f 7079 2829 0a20   = self.copy(). 
-000146c0: 2020 2020 2020 2020 2020 2066 6f72 2074             for t
-000146d0: 6572 6d20 696e 206f 7468 6572 2e64 6572  erm in other.der
-000146e0: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
-000146f0: 7574 7320 6966 2072 6967 6874 2065 6c73  uts if right els
-00014700: 6520 7265 7665 7273 6564 286f 7468 6572  e reversed(other
-00014710: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
-00014720: 2e69 6e70 7574 7329 3a0a 2020 2020 2020  .inputs):.      
-00014730: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
-00014740: 2074 6d70 2e64 6976 6973 6962 6c65 2874   tmp.divisible(t
-00014750: 6572 6d2c 2072 6967 6874 3d72 6967 6874  erm, right=right
-00014760: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00014770: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
-00014780: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
-00014790: 2020 2020 746d 702e 6578 7465 6e64 5f6d      tmp.extend_m
-000147a0: 756c 5f64 6976 5f28 7465 726d 2c20 6b69  ul_div_(term, ki
-000147b0: 6e64 3d22 7472 7565 6469 7622 2c20 7269  nd="truediv", ri
-000147c0: 6768 743d 7269 6768 7429 0a20 2020 2020  ght=right).     
-000147d0: 2020 2020 2020 2072 6574 7572 6e20 5472         return Tr
-000147e0: 7565 0a20 2020 2020 2020 206d 6f73 745f  ue.        most_
-000147f0: 7265 6365 6e74 5f74 6572 6d20 3d20 7365  recent_term = se
-00014800: 6c66 2e74 6572 6d73 5b2d 3120 6966 2072  lf.terms[-1 if r
-00014810: 6967 6874 2065 6c73 6520 305d 0a20 2020  ight else 0].   
-00014820: 2020 2020 2069 6620 6f74 6865 7220 3d3d       if other ==
-00014830: 206d 6f73 745f 7265 6365 6e74 5f74 6572   most_recent_ter
-00014840: 6d3a 0a20 2020 2020 2020 2020 2020 2072  m:.            r
-00014850: 6574 7572 6e20 5472 7565 0a20 2020 2020  eturn True.     
-00014860: 2020 2069 6620 6d6f 7374 5f72 6563 656e     if most_recen
-00014870: 745f 7465 726d 2e64 696d 656e 7369 6f6e  t_term.dimension
-00014880: 2069 7320 6e6f 7420 4e6f 6e65 2061 6e64   is not None and
-00014890: 206f 7468 6572 2e64 696d 656e 7369 6f6e   other.dimension
-000148a0: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-000148b0: 2020 2020 2020 2020 2020 6966 206d 6f73            if mos
-000148c0: 745f 7265 6365 6e74 5f74 6572 6d2e 6469  t_recent_term.di
-000148d0: 6d65 6e73 696f 6e20 2520 6f74 6865 722e  mension % other.
-000148e0: 6469 6d65 6e73 696f 6e20 3d3d 2030 3a0a  dimension == 0:.
-000148f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014900: 7265 7475 726e 2054 7275 650a 2020 2020  return True.    
-00014910: 2020 2020 7265 7475 726e 2046 616c 7365      return False
-00014920: 0a0a 2020 2020 6465 6620 6361 6e5f 7369  ..    def can_si
-00014930: 6d70 6c69 6679 2873 656c 662c 206f 7468  mplify(self, oth
-00014940: 6572 2c20 6b69 6e64 2c20 7269 6768 7429  er, kind, right)
-00014950: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
-00014960: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
-00014970: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
-00014980: 3a70 6172 616d 2073 7472 206b 696e 643a  :param str kind:
-00014990: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-000149a0: 626f 6f6c 2072 6967 6874 3a0a 2020 2020  bool right:.    
-000149b0: 2020 2020 3a72 6574 7572 6e3a 2077 6865      :return: whe
-000149c0: 7468 6572 2077 6520 6361 6e20 7369 6d70  ther we can simp
-000149d0: 6c69 6679 2077 6865 6e20 6170 706c 7969  lify when applyi
-000149e0: 6e67 2074 6869 7320 6f70 6572 6174 696f  ng this operatio
-000149f0: 6e0a 2020 2020 2020 2020 3a72 7479 7065  n.        :rtype
-00014a00: 3a20 626f 6f6c 0a20 2020 2020 2020 2022  : bool.        "
-00014a10: 2222 0a20 2020 2020 2020 2069 6620 6f74  "".        if ot
-00014a20: 6865 722e 6465 7269 7665 645f 6672 6f6d  her.derived_from
-00014a30: 5f6f 7020 616e 6420 6f74 6865 722e 6465  _op and other.de
-00014a40: 7269 7665 645f 6672 6f6d 5f6f 702e 6b69  rived_from_op.ki
-00014a50: 6e64 203d 3d20 226d 756c 223a 0a20 2020  nd == "mul":.   
-00014a60: 2020 2020 2020 2020 2074 6d70 203d 2073           tmp = s
-00014a70: 656c 662e 636f 7079 2829 0a20 2020 2020  elf.copy().     
-00014a80: 2020 2020 2020 2066 6f72 2074 6572 6d20         for term 
-00014a90: 696e 206f 7468 6572 2e64 6572 6976 6564  in other.derived
-00014aa0: 5f66 726f 6d5f 6f70 2e69 6e70 7574 7320  _from_op.inputs 
-00014ab0: 6966 2072 6967 6874 2065 6c73 6520 7265  if right else re
-00014ac0: 7665 7273 6564 286f 7468 6572 2e64 6572  versed(other.der
-00014ad0: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
-00014ae0: 7574 7329 3a0a 2020 2020 2020 2020 2020  uts):.          
-00014af0: 2020 2020 2020 6966 206e 6f74 2074 6d70        if not tmp
-00014b00: 2e63 616e 5f73 696d 706c 6966 7928 7465  .can_simplify(te
-00014b10: 726d 2c20 6b69 6e64 3d6b 696e 642c 2072  rm, kind=kind, r
-00014b20: 6967 6874 3d72 6967 6874 293a 0a20 2020  ight=right):.   
-00014b30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b40: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
-00014b50: 2020 2020 2020 2020 2020 2020 2020 746d                tm
-00014b60: 702e 6578 7465 6e64 5f6d 756c 5f64 6976  p.extend_mul_div
-00014b70: 5f28 7465 726d 2c20 6b69 6e64 3d6b 696e  _(term, kind=kin
-00014b80: 642c 2072 6967 6874 3d72 6967 6874 290a  d, right=right).
-00014b90: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00014ba0: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
-00014bb0: 6964 7820 3d20 7365 6c66 2e5f 7369 6d70  idx = self._simp
-00014bc0: 6c69 6679 5f74 6572 6d5f 6964 7828 6f74  lify_term_idx(ot
-00014bd0: 6865 722c 206b 696e 643d 6b69 6e64 2c20  her, kind=kind, 
-00014be0: 7269 6768 743d 7269 6768 7429 0a20 2020  right=right).   
-00014bf0: 2020 2020 2072 6574 7572 6e20 6964 7820       return idx 
-00014c00: 6973 206e 6f74 204e 6f6e 650a 0a20 2020  is not None..   
-00014c10: 2064 6566 205f 7369 6d70 6c69 6679 5f74   def _simplify_t
-00014c20: 6572 6d5f 6964 7828 7365 6c66 2c20 6f74  erm_idx(self, ot
-00014c30: 6865 722c 206b 696e 642c 2072 6967 6874  her, kind, right
-00014c40: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00014c50: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
-00014c60: 6d20 6f74 6865 723a 0a20 2020 2020 2020  m other:.       
-00014c70: 203a 7061 7261 6d20 7374 7220 6b69 6e64   :param str kind
-00014c80: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-00014c90: 2062 6f6f 6c20 7269 6768 743a 0a20 2020   bool right:.   
-00014ca0: 2020 2020 203a 7265 7475 726e 3a20 696e       :return: in
-00014cb0: 6465 7820 6f66 2074 6572 6d20 746f 2073  dex of term to s
-00014cc0: 696d 706c 6966 790a 2020 2020 2020 2020  implify.        
-00014cd0: 3a72 7479 7065 3a20 696e 747c 4e6f 6e65  :rtype: int|None
-00014ce0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00014cf0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
-00014d00: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
-00014d10: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
-00014d20: 2020 2020 2020 2020 6966 206b 696e 6420          if kind 
-00014d30: 3d3d 2022 6d75 6c22 3a0a 2020 2020 2020  == "mul":.      
-00014d40: 2020 2020 2020 2320 5765 2077 616e 7420        # We want 
-00014d50: 2862 202a 2061 2920 2f2f 2062 2021 3d20  (b * a) // b != 
-00014d60: 612e 0a20 2020 2020 2020 2020 2020 2023  a..            #
-00014d70: 2048 6f77 6576 6572 2c20 7765 2077 616e   However, we wan
-00014d80: 7420 6820 2a20 2832 202a 2061 202f 2f20  t h * (2 * a // 
-00014d90: 6829 203d 3d20 3220 2a20 612e 0a20 2020  h) == 2 * a..   
-00014da0: 2020 2020 2020 2020 2023 2053 6f2c 2066           # So, f
-00014db0: 6f72 2060 6d75 6c60 2c20 616e 6420 6f6e  or `mul`, and on
-00014dc0: 6c79 2066 6f72 2060 6d75 6c60 2c20 6368  ly for `mul`, ch
-00014dd0: 6563 6b20 616c 6c20 7465 726d 732c 2077  eck all terms, w
-00014de0: 6865 7468 6572 2077 6520 6361 6e20 7369  hether we can si
-00014df0: 6d70 6c69 6679 2073 6f6d 6520 6469 7669  mplify some divi
-00014e00: 7369 6f6e 2d74 6572 6d2e 0a20 2020 2020  sion-term..     
-00014e10: 2020 2020 2020 2066 6f72 2069 2c20 7465         for i, te
-00014e20: 726d 2069 6e20 7265 7665 7273 6564 286c  rm in reversed(l
-00014e30: 6973 7428 656e 756d 6572 6174 6528 7365  ist(enumerate(se
-00014e40: 6c66 2e74 6572 6d73 2929 2920 6966 2072  lf.terms))) if r
-00014e50: 6967 6874 2065 6c73 6520 656e 756d 6572  ight else enumer
-00014e60: 6174 6528 7365 6c66 2e74 6572 6d73 293a  ate(self.terms):
-00014e70: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014e80: 2061 7373 6572 7420 6973 696e 7374 616e   assert isinstan
-00014e90: 6365 2874 6572 6d2c 205f 642e 4469 6d29  ce(term, _d.Dim)
-00014ea0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014eb0: 2069 6620 7465 726d 2e64 6572 6976 6564   if term.derived
-00014ec0: 5f66 726f 6d5f 6f70 3a0a 2020 2020 2020  _from_op:.      
-00014ed0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00014ee0: 2074 6572 6d2e 6465 7269 7665 645f 6672   term.derived_fr
-00014ef0: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 2274  om_op.kind == "t
-00014f00: 7275 6564 6976 5f22 202b 2028 2272 6967  ruediv_" + ("rig
-00014f10: 6874 2220 6966 2072 6967 6874 2065 6c73  ht" if right els
-00014f20: 6520 226c 6566 7422 293a 0a20 2020 2020  e "left"):.     
-00014f30: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f40: 2020 2069 6620 7465 726d 2e64 6572 6976     if term.deriv
-00014f50: 6564 5f66 726f 6d5f 6f70 2e69 6e70 7574  ed_from_op.input
-00014f60: 735b 2d31 5d20 3d3d 206f 7468 6572 3a0a  s[-1] == other:.
-00014f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014f80: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00014f90: 726e 2069 0a20 2020 2020 2020 2020 2020  rn i.           
-00014fa0: 2020 2020 2069 6620 6f74 6865 722e 6465       if other.de
-00014fb0: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
-00014fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014fd0: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
-00014fe0: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
-00014ff0: 203d 3d20 2274 7275 6564 6976 5f22 202b   == "truediv_" +
-00015000: 2028 2272 6967 6874 2220 6966 206e 6f74   ("right" if not
-00015010: 2072 6967 6874 2065 6c73 6520 226c 6566   right else "lef
-00015020: 7422 293a 0a20 2020 2020 2020 2020 2020  t"):.           
-00015030: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00015040: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
-00015050: 6f6d 5f6f 702e 696e 7075 7473 5b2d 315d  om_op.inputs[-1]
-00015060: 203d 3d20 7465 726d 3a0a 2020 2020 2020   == term:.      
-00015070: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015080: 2020 2020 2020 7265 7475 726e 2069 0a20        return i. 
-00015090: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-000150a0: 6620 7465 726d 2e69 735f 636f 6e73 7461  f term.is_consta
-000150b0: 6e74 5f73 7461 7469 635f 6469 6d28 2920  nt_static_dim() 
-000150c0: 616e 6420 6f74 6865 722e 6973 5f63 6f6e  and other.is_con
-000150d0: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
-000150e0: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
-000150f0: 2020 2020 2020 2020 7265 7475 726e 2069          return i
-00015100: 0a20 2020 2020 2020 2023 2046 6f72 2074  .        # For t
-00015110: 6865 206c 6173 742f 6669 7273 7420 7465  he last/first te
-00015120: 726d 2c20 6578 7472 6120 6368 6563 6b73  rm, extra checks
-00015130: 2e0a 2020 2020 2020 2020 6920 3d20 6c65  ..        i = le
-00015140: 6e28 7365 6c66 2e74 6572 6d73 2920 2d20  n(self.terms) - 
-00015150: 3120 6966 2072 6967 6874 2065 6c73 6520  1 if right else 
-00015160: 300a 2020 2020 2020 2020 7465 726d 203d  0.        term =
-00015170: 2073 656c 662e 7465 726d 735b 695d 0a20   self.terms[i]. 
-00015180: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
-00015190: 6e64 7377 6974 6828 2264 6976 2229 2061  ndswith("div") a
-000151a0: 6e64 206f 7468 6572 203d 3d20 7465 726d  nd other == term
-000151b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
-000151c0: 7475 726e 2069 0a20 2020 2020 2020 206f  turn i.        o
-000151d0: 705f 6b69 6e64 203d 206b 696e 6420 2b20  p_kind = kind + 
-000151e0: 225f 2220 2b20 2822 7269 6768 7422 2069  "_" + ("right" i
-000151f0: 6620 7269 6768 7420 656c 7365 2022 6c65  f right else "le
-00015200: 6674 2229 0a20 2020 2020 2020 2069 6620  ft").        if 
-00015210: 7465 726d 2e64 6572 6976 6564 5f66 726f  term.derived_fro
-00015220: 6d5f 6f70 2061 6e64 2074 6572 6d2e 6465  m_op and term.de
-00015230: 7269 7665 645f 6672 6f6d 5f6f 702e 6b69  rived_from_op.ki
-00015240: 6e64 203d 3d20 6f70 5f6b 696e 643a 0a20  nd == op_kind:. 
-00015250: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00015260: 6e20 690a 2020 2020 2020 2020 7265 7475  n i.        retu
-00015270: 726e 204e 6f6e 650a 0a20 2020 2064 6566  rn None..    def
-00015280: 2065 7874 656e 645f 6d75 6c5f 6469 765f   extend_mul_div_
-00015290: 2873 656c 662c 206f 7468 6572 2c20 6b69  (self, other, ki
-000152a0: 6e64 2c20 7269 6768 7429 3a0a 2020 2020  nd, right):.    
-000152b0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000152c0: 3a70 6172 616d 2044 696d 206f 7468 6572  :param Dim other
-000152d0: 3a0a 2020 2020 2020 2020 3a70 6172 616d  :.        :param
-000152e0: 2073 7472 206b 696e 643a 0a20 2020 2020   str kind:.     
-000152f0: 2020 203a 7061 7261 6d20 626f 6f6c 2072     :param bool r
-00015300: 6967 6874 3a0a 2020 2020 2020 2020 2222  ight:.        ""
-00015310: 220a 2020 2020 2020 2020 6173 7365 7274  ".        assert
-00015320: 206b 696e 6420 696e 207b 226d 756c 222c   kind in {"mul",
-00015330: 2022 666c 6f6f 7264 6976 222c 2022 7472   "floordiv", "tr
-00015340: 7565 6469 7622 2c20 2263 6569 6c64 6976  uediv", "ceildiv
-00015350: 227d 0a20 2020 2020 2020 2069 6620 6f74  "}.        if ot
-00015360: 6865 722e 6973 5f63 6f6e 7374 616e 745f  her.is_constant_
-00015370: 7374 6174 6963 5f64 696d 2829 2061 6e64  static_dim() and
-00015380: 206f 7468 6572 2e64 696d 656e 7369 6f6e   other.dimension
-00015390: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
-000153a0: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
-000153b0: 2020 6966 206e 6f74 2073 656c 662e 7465    if not self.te
-000153c0: 726d 733a 0a20 2020 2020 2020 2020 2020  rms:.           
-000153d0: 2069 6620 6b69 6e64 203d 3d20 226d 756c   if kind == "mul
-000153e0: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
-000153f0: 2020 2073 656c 662e 7465 726d 732e 6170     self.terms.ap
-00015400: 7065 6e64 286f 7468 6572 290a 2020 2020  pend(other).    
-00015410: 2020 2020 2020 2020 656c 6966 206b 696e          elif kin
-00015420: 642e 656e 6473 7769 7468 2822 6469 7622  d.endswith("div"
-00015430: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00015440: 2020 2073 656c 662e 7465 726d 7320 3d20     self.terms = 
-00015450: 5b5f 4f70 4d75 6c74 5465 726d 2e6e 6577  [_OpMultTerm.new
-00015460: 5f64 6976 5f64 696d 2873 656c 662e 6173  _div_dim(self.as
-00015470: 5f64 696d 2829 2c20 6f74 6865 722c 206b  _dim(), other, k
-00015480: 696e 643d 6b69 6e64 2c20 7269 6768 743d  ind=kind, right=
-00015490: 7269 6768 7429 5d0a 2020 2020 2020 2020  right)].        
-000154a0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-000154b0: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
-000154c0: 7665 645f 6672 6f6d 5f6f 7020 616e 6420  ved_from_op and 
-000154d0: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
-000154e0: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 226d  om_op.kind == "m
-000154f0: 756c 223a 0a20 2020 2020 2020 2020 2020  ul":.           
-00015500: 2066 6f72 2074 6572 6d20 696e 206f 7468   for term in oth
-00015510: 6572 2e64 6572 6976 6564 5f66 726f 6d5f  er.derived_from_
-00015520: 6f70 2e69 6e70 7574 7320 6966 2072 6967  op.inputs if rig
-00015530: 6874 2065 6c73 6520 7265 7665 7273 6564  ht else reversed
-00015540: 286f 7468 6572 2e64 6572 6976 6564 5f66  (other.derived_f
-00015550: 726f 6d5f 6f70 2e69 6e70 7574 7329 3a0a  rom_op.inputs):.
-00015560: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015570: 7365 6c66 2e65 7874 656e 645f 6d75 6c5f  self.extend_mul_
-00015580: 6469 765f 2874 6572 6d2c 206b 696e 643d  div_(term, kind=
-00015590: 6b69 6e64 2c20 7269 6768 743d 7269 6768  kind, right=righ
-000155a0: 7429 0a20 2020 2020 2020 2020 2020 2072  t).            r
-000155b0: 6574 7572 6e0a 2020 2020 2020 2020 6964  eturn.        id
-000155c0: 7820 3d20 7365 6c66 2e5f 7369 6d70 6c69  x = self._simpli
-000155d0: 6679 5f74 6572 6d5f 6964 7828 6f74 6865  fy_term_idx(othe
-000155e0: 722c 206b 696e 643d 6b69 6e64 2c20 7269  r, kind=kind, ri
-000155f0: 6768 743d 7269 6768 7429 0a20 2020 2020  ght=right).     
-00015600: 2020 2069 6620 6964 7820 6973 206e 6f74     if idx is not
-00015610: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00015620: 2020 2074 6572 6d20 3d20 7365 6c66 2e74     term = self.t
-00015630: 6572 6d73 5b69 6478 5d0a 2020 2020 2020  erms[idx].      
-00015640: 2020 2020 2020 6173 7365 7274 2069 7369        assert isi
-00015650: 6e73 7461 6e63 6528 7465 726d 2c20 5f64  nstance(term, _d
-00015660: 2e44 696d 290a 2020 2020 2020 2020 2020  .Dim).          
-00015670: 2020 6966 206b 696e 642e 656e 6473 7769    if kind.endswi
-00015680: 7468 2822 6469 7622 2920 616e 6420 6f74  th("div") and ot
-00015690: 6865 7220 3d3d 2074 6572 6d3a 0a20 2020  her == term:.   
-000156a0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000156b0: 662e 7465 726d 732e 706f 7028 6964 7829  f.terms.pop(idx)
-000156c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000156d0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
-000156e0: 2020 2020 6966 206b 696e 6420 3d3d 2022      if kind == "
-000156f0: 6d75 6c22 2061 6e64 2074 6572 6d2e 6465  mul" and term.de
-00015700: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
-00015710: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00015720: 6620 7465 726d 2e64 6572 6976 6564 5f66  f term.derived_f
-00015730: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 2022  rom_op.kind == "
-00015740: 7472 7565 6469 765f 2220 2b20 2822 7269  truediv_" + ("ri
-00015750: 6768 7422 2069 6620 7269 6768 7420 656c  ght" if right el
-00015760: 7365 2022 6c65 6674 2229 3a0a 2020 2020  se "left"):.    
-00015770: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015780: 6966 2074 6572 6d2e 6465 7269 7665 645f  if term.derived_
-00015790: 6672 6f6d 5f6f 702e 696e 7075 7473 5b2d  from_op.inputs[-
-000157a0: 315d 203d 3d20 6f74 6865 723a 0a20 2020  1] == other:.   
-000157b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000157c0: 2020 2020 2073 656c 662e 7465 726d 735b       self.terms[
-000157d0: 6964 785d 203d 2074 6572 6d2e 6465 7269  idx] = term.deri
-000157e0: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
-000157f0: 7473 5b30 5d0a 2020 2020 2020 2020 2020  ts[0].          
-00015800: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00015810: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-00015820: 2069 6620 6b69 6e64 203d 3d20 226d 756c   if kind == "mul
-00015830: 2220 616e 6420 6f74 6865 722e 6465 7269  " and other.deri
-00015840: 7665 645f 6672 6f6d 5f6f 703a 0a20 2020  ved_from_op:.   
-00015850: 2020 2020 2020 2020 2020 2020 2069 6620               if 
-00015860: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
-00015870: 6f6d 5f6f 702e 6b69 6e64 203d 3d20 2274  om_op.kind == "t
-00015880: 7275 6564 6976 5f22 202b 2028 2272 6967  ruediv_" + ("rig
-00015890: 6874 2220 6966 206e 6f74 2072 6967 6874  ht" if not right
-000158a0: 2065 6c73 6520 226c 6566 7422 293a 0a20   else "left"):. 
-000158b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000158c0: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
-000158d0: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
-000158e0: 7473 5b2d 315d 203d 3d20 7465 726d 3a0a  ts[-1] == term:.
-000158f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015900: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
-00015910: 6d73 5b69 6478 5d20 3d20 6f74 6865 722e  ms[idx] = other.
-00015920: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
-00015930: 696e 7075 7473 5b30 5d0a 2020 2020 2020  inputs[0].      
-00015940: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015950: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
-00015960: 2020 2020 2069 6620 7465 726d 2e69 735f       if term.is_
-00015970: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
-00015980: 6469 6d28 2920 616e 6420 6f74 6865 722e  dim() and other.
-00015990: 6973 5f63 6f6e 7374 616e 745f 7374 6174  is_constant_stat
-000159a0: 6963 5f64 696d 2829 3a0a 2020 2020 2020  ic_dim():.      
-000159b0: 2020 2020 2020 2020 2020 6966 206b 696e            if kin
-000159c0: 6420 3d3d 2022 6d75 6c22 3a0a 2020 2020  d == "mul":.    
-000159d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000159e0: 6966 2074 6572 6d2e 6469 6d65 6e73 696f  if term.dimensio
-000159f0: 6e20 2a20 6f74 6865 722e 6469 6d65 6e73  n * other.dimens
-00015a00: 696f 6e20 3d3d 2031 3a0a 2020 2020 2020  ion == 1:.      
-00015a10: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015a20: 2020 7365 6c66 2e74 6572 6d73 2e70 6f70    self.terms.pop
-00015a30: 2869 6478 290a 2020 2020 2020 2020 2020  (idx).          
-00015a40: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00015a50: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-00015a60: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-00015a70: 726d 735b 6964 785d 203d 205f 6d61 6b65  rms[idx] = _make
-00015a80: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
-00015a90: 5f64 696d 2874 6572 6d2e 6469 6d65 6e73  _dim(term.dimens
-00015aa0: 696f 6e20 2a20 6f74 6865 722e 6469 6d65  ion * other.dime
-00015ab0: 6e73 696f 6e2c 206b 696e 643d 7465 726d  nsion, kind=term
-00015ac0: 2e6b 696e 6429 0a20 2020 2020 2020 2020  .kind).         
-00015ad0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00015ae0: 6e0a 2020 2020 2020 2020 2020 2020 2020  n.              
-00015af0: 2020 6966 206b 696e 642e 656e 6473 7769    if kind.endswi
-00015b00: 7468 2822 6469 7622 2920 616e 6420 7465  th("div") and te
-00015b10: 726d 2e64 696d 656e 7369 6f6e 2025 206f  rm.dimension % o
-00015b20: 7468 6572 2e64 696d 656e 7369 6f6e 203d  ther.dimension =
-00015b30: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
-00015b40: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
-00015b50: 726d 735b 6964 785d 203d 205f 6d61 6b65  rms[idx] = _make
-00015b60: 5f63 6f6e 7374 616e 745f 7374 6174 6963  _constant_static
-00015b70: 5f64 696d 2874 6572 6d2e 6469 6d65 6e73  _dim(term.dimens
-00015b80: 696f 6e20 2f2f 206f 7468 6572 2e64 696d  ion // other.dim
-00015b90: 656e 7369 6f6e 2c20 6b69 6e64 3d74 6572  ension, kind=ter
-00015ba0: 6d2e 6b69 6e64 290a 2020 2020 2020 2020  m.kind).        
-00015bb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00015bc0: 726e 0a20 2020 2020 2020 2020 2020 2020  rn.             
-00015bd0: 2020 2023 2046 616c 6c62 6163 6b20 7769     # Fallback wi
-00015be0: 7468 2067 656e 6572 6963 2068 616e 646c  th generic handl
-00015bf0: 696e 672e 0a20 2020 2020 2020 2020 2020  ing..           
-00015c00: 206f 705f 6b69 6e64 203d 206b 696e 6420   op_kind = kind 
-00015c10: 2b20 225f 2220 2b20 2822 7269 6768 7422  + "_" + ("right"
-00015c20: 2069 6620 7269 6768 7420 656c 7365 2022   if right else "
-00015c30: 6c65 6674 2229 0a20 2020 2020 2020 2020  left").         
-00015c40: 2020 2069 6620 6b69 6e64 2e65 6e64 7377     if kind.endsw
-00015c50: 6974 6828 2264 6976 2229 2061 6e64 2074  ith("div") and t
-00015c60: 6572 6d2e 6465 7269 7665 645f 6672 6f6d  erm.derived_from
-00015c70: 5f6f 7020 616e 6420 7465 726d 2e64 6572  _op and term.der
-00015c80: 6976 6564 5f66 726f 6d5f 6f70 2e6b 696e  ived_from_op.kin
-00015c90: 6420 3d3d 206f 705f 6b69 6e64 3a0a 2020  d == op_kind:.  
-00015ca0: 2020 2020 2020 2020 2020 2020 2020 6e75                nu
-00015cb0: 6d65 7261 746f 7220 3d20 7465 726d 2e64  merator = term.d
-00015cc0: 6572 6976 6564 5f66 726f 6d5f 6f70 2e69  erived_from_op.i
-00015cd0: 6e70 7574 735b 305d 0a20 2020 2020 2020  nputs[0].       
-00015ce0: 2020 2020 2020 2020 2064 656e 6f6d 696e           denomin
-00015cf0: 6174 6f72 203d 2074 6572 6d2e 6465 7269  ator = term.deri
-00015d00: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
-00015d10: 7473 5b31 5d0a 2020 2020 2020 2020 2020  ts[1].          
-00015d20: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
-00015d30: 5b69 6478 5d20 3d20 5f4f 704d 756c 7454  [idx] = _OpMultT
-00015d40: 6572 6d2e 6e65 775f 6469 765f 6469 6d28  erm.new_div_dim(
-00015d50: 6e75 6d65 7261 746f 722c 2064 656e 6f6d  numerator, denom
-00015d60: 696e 6174 6f72 202a 206f 7468 6572 2c20  inator * other, 
-00015d70: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
-00015d80: 3d72 6967 6874 290a 2020 2020 2020 2020  =right).        
-00015d90: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
-00015da0: 2020 2020 2020 2069 6620 6b69 6e64 2e65         if kind.e
-00015db0: 6e64 7377 6974 6828 2264 6976 2229 3a0a  ndswith("div"):.
-00015dc0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-00015dd0: 2e74 6572 6d73 203d 205b 5f4f 704d 756c  .terms = [_OpMul
-00015de0: 7454 6572 6d2e 6e65 775f 6469 765f 6469  tTerm.new_div_di
-00015df0: 6d28 7365 6c66 2e61 735f 6469 6d28 292c  m(self.as_dim(),
-00015e00: 206f 7468 6572 2c20 6b69 6e64 3d6b 696e   other, kind=kin
-00015e10: 642c 2072 6967 6874 3d72 6967 6874 295d  d, right=right)]
-00015e20: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00015e30: 7572 6e0a 2020 2020 2020 2020 6966 206b  urn.        if k
-00015e40: 696e 6420 3d3d 2022 6d75 6c22 3a0a 2020  ind == "mul":.  
-00015e50: 2020 2020 2020 2020 2020 6966 2072 6967            if rig
-00015e60: 6874 3a0a 2020 2020 2020 2020 2020 2020  ht:.            
-00015e70: 2020 2020 7365 6c66 2e74 6572 6d73 2e61      self.terms.a
-00015e80: 7070 656e 6428 6f74 6865 7229 0a20 2020  ppend(other).   
-00015e90: 2020 2020 2020 2020 2065 6c73 653a 0a20           else:. 
-00015ea0: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00015eb0: 656c 662e 7465 726d 732e 696e 7365 7274  elf.terms.insert
-00015ec0: 2830 2c20 6f74 6865 7229 0a20 2020 2020  (0, other).     
-00015ed0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
-00015ee0: 2020 2020 2020 6173 7365 7274 2046 616c        assert Fal
-00015ef0: 7365 0a0a 2020 2020 4063 6c61 7373 6d65  se..    @classme
-00015f00: 7468 6f64 0a20 2020 2064 6566 206e 6577  thod.    def new
-00015f10: 5f64 6976 5f64 696d 2863 6c73 2c20 6e75  _div_dim(cls, nu
-00015f20: 6d65 7261 746f 722c 2064 656e 6f6d 696e  merator, denomin
-00015f30: 6174 6f72 2c20 6b69 6e64 2c20 7269 6768  ator, kind, righ
-00015f40: 7429 3a0a 2020 2020 2020 2020 2222 220a  t):.        """.
-00015f50: 2020 2020 2020 2020 3a70 6172 616d 2044          :param D
-00015f60: 696d 206e 756d 6572 6174 6f72 3a0a 2020  im numerator:.  
-00015f70: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
-00015f80: 2064 656e 6f6d 696e 6174 6f72 3a0a 2020   denominator:.  
-00015f90: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
-00015fa0: 206b 696e 643a 2022 666c 6f6f 7264 6976   kind: "floordiv
-00015fb0: 2220 6f72 2022 6365 696c 6469 7622 206f  " or "ceildiv" o
-00015fc0: 7220 2274 7275 6564 6976 220a 2020 2020  r "truediv".    
-00015fd0: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
-00015fe0: 7269 6768 743a 0a20 2020 2020 2020 203a  right:.        :
-00015ff0: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
-00016000: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
-00016010: 696d 5f76 616c 7565 203d 204e 6f6e 650a  im_value = None.
-00016020: 2020 2020 2020 2020 6120 3d20 6e75 6d65          a = nume
-00016030: 7261 746f 722e 6469 6d65 6e73 696f 6e0a  rator.dimension.
-00016040: 2020 2020 2020 2020 6220 3d20 6465 6e6f          b = deno
-00016050: 6d69 6e61 746f 722e 6469 6d65 6e73 696f  minator.dimensio
-00016060: 6e0a 2020 2020 2020 2020 6966 2061 2069  n.        if a i
-00016070: 7320 6e6f 7420 4e6f 6e65 2061 6e64 2062  s not None and b
-00016080: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
-00016090: 2020 2020 2020 2020 2020 6966 206b 696e            if kin
-000160a0: 6420 3d3d 2022 666c 6f6f 7264 6976 223a  d == "floordiv":
-000160b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000160c0: 2064 696d 5f76 616c 7565 203d 2061 202f   dim_value = a /
-000160d0: 2f20 620a 2020 2020 2020 2020 2020 2020  / b.            
-000160e0: 656c 6966 206b 696e 6420 3d3d 2022 6365  elif kind == "ce
-000160f0: 696c 6469 7622 3a0a 2020 2020 2020 2020  ildiv":.        
-00016100: 2020 2020 2020 2020 6469 6d5f 7661 6c75          dim_valu
-00016110: 6520 3d20 2d28 2d61 202f 2f20 6229 0a20  e = -(-a // b). 
-00016120: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00016130: 6620 6120 2520 6220 3d3d 2030 2061 6e64  f a % b == 0 and
-00016140: 2072 6967 6874 3a0a 2020 2020 2020 2020   right:.        
-00016150: 2020 2020 2020 2020 2020 2020 6b69 6e64              kind
-00016160: 203d 2022 666c 6f6f 7264 6976 2220 2023   = "floordiv"  #
-00016170: 2066 6f72 206e 6963 6572 2064 6573 6372   for nicer descr
-00016180: 6970 7469 6f6e 2c20 616e 6420 646f 6573  iption, and does
-00016190: 206e 6f74 206d 6174 7465 720a 2020 2020   not matter.    
-000161a0: 2020 2020 2020 2020 656c 6966 206b 696e          elif kin
-000161b0: 6420 3d3d 2022 7472 7565 6469 7622 3a0a  d == "truediv":.
-000161c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161d0: 6966 2061 2025 2062 2021 3d20 303a 0a20  if a % b != 0:. 
-000161e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000161f0: 2020 2072 6169 7365 2056 616c 7565 4572     raise ValueEr
-00016200: 726f 7228 0a20 2020 2020 2020 2020 2020  ror(.           
-00016210: 2020 2020 2020 2020 2020 2020 2022 2573               "%s
-00016220: 2074 7275 6564 6976 2025 7320 6f6e 6c79   truediv %s only
-00016230: 2061 6c6c 6f77 6564 2069 6620 7468 6520   allowed if the 
-00016240: 7265 7375 6c74 2069 7320 616e 2069 6e74  result is an int
-00016250: 6567 6572 2220 2520 286e 756d 6572 6174  eger" % (numerat
-00016260: 6f72 2c20 6465 6e6f 6d69 6e61 746f 7229  or, denominator)
-00016270: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016280: 2020 2020 2029 0a20 2020 2020 2020 2020       ).         
-00016290: 2020 2020 2020 2064 696d 5f76 616c 7565         dim_value
-000162a0: 203d 2061 202f 2f20 620a 2020 2020 2020   = a // b.      
-000162b0: 2020 2020 2020 2020 2020 6966 2072 6967            if rig
-000162c0: 6874 3a0a 2020 2020 2020 2020 2020 2020  ht:.            
-000162d0: 2020 2020 2020 2020 6b69 6e64 203d 2022          kind = "
-000162e0: 666c 6f6f 7264 6976 2220 2023 2066 6f72  floordiv"  # for
-000162f0: 206e 6963 6572 2064 6573 6372 6970 7469   nicer descripti
-00016300: 6f6e 2c20 616e 6420 646f 6573 206e 6f74  on, and does not
-00016310: 206d 6174 7465 720a 2020 2020 2020 2020   matter.        
-00016320: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00016330: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-00016340: 5661 6c75 6545 7272 6f72 2822 696e 7661  ValueError("inva
-00016350: 6c69 6420 6b69 6e64 2025 7222 2025 2028  lid kind %r" % (
-00016360: 6b69 6e64 2c29 290a 2020 2020 2020 2020  kind,)).        
-00016370: 6966 206b 696e 6420 3d3d 2022 666c 6f6f  if kind == "floo
-00016380: 7264 6976 2220 616e 6420 7269 6768 743a  rdiv" and right:
-00016390: 0a20 2020 2020 2020 2020 2020 2064 6573  .            des
-000163a0: 6372 6970 7469 6f6e 203d 2022 2573 2f2f  cription = "%s//
-000163b0: 2573 2220 2520 285f 6765 745f 6465 7363  %s" % (_get_desc
-000163c0: 7269 7074 696f 6e28 6e75 6d65 7261 746f  ription(numerato
-000163d0: 7229 2c20 5f67 6574 5f64 6573 6372 6970  r), _get_descrip
-000163e0: 7469 6f6e 2864 656e 6f6d 696e 6174 6f72  tion(denominator
-000163f0: 2929 0a20 2020 2020 2020 2065 6c69 6620  )).        elif 
-00016400: 6b69 6e64 203d 3d20 2263 6569 6c64 6976  kind == "ceildiv
-00016410: 2220 616e 6420 7269 6768 743a 0a20 2020  " and right:.   
-00016420: 2020 2020 2020 2020 2064 6573 6372 6970           descrip
-00016430: 7469 6f6e 203d 2022 e28c 8825 732f 2573  tion = "...%s/%s
-00016440: e28c 8922 2025 2028 5f67 6574 5f64 6573  ..." % (_get_des
-00016450: 6372 6970 7469 6f6e 286e 756d 6572 6174  cription(numerat
-00016460: 6f72 292c 205f 6765 745f 6465 7363 7269  or), _get_descri
-00016470: 7074 696f 6e28 6465 6e6f 6d69 6e61 746f  ption(denominato
-00016480: 7229 290a 2020 2020 2020 2020 656c 7365  r)).        else
-00016490: 3a0a 2020 2020 2020 2020 2020 2020 6465  :.            de
-000164a0: 7363 7269 7074 696f 6e20 3d20 2225 735f  scription = "%s_
-000164b0: 2573 2825 732c 2025 7329 2220 2520 280a  %s(%s, %s)" % (.
-000164c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000164d0: 6b69 6e64 2c0a 2020 2020 2020 2020 2020  kind,.          
-000164e0: 2020 2020 2020 2272 6967 6874 2220 6966        "right" if
-000164f0: 2072 6967 6874 2065 6c73 6520 226c 6566   right else "lef
-00016500: 7422 2c0a 2020 2020 2020 2020 2020 2020  t",.            
-00016510: 2020 2020 5f67 6574 5f64 6573 6372 6970      _get_descrip
-00016520: 7469 6f6e 286e 756d 6572 6174 6f72 2c20  tion(numerator, 
-00016530: 6272 6163 6b65 7473 3d46 616c 7365 292c  brackets=False),
-00016540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00016550: 205f 6765 745f 6465 7363 7269 7074 696f   _get_descriptio
-00016560: 6e28 6465 6e6f 6d69 6e61 746f 722c 2062  n(denominator, b
-00016570: 7261 636b 6574 733d 4661 6c73 6529 2c0a  rackets=False),.
-00016580: 2020 2020 2020 2020 2020 2020 290a 2020              ).  
-00016590: 2020 2020 2020 6f70 5f6b 696e 6420 3d20        op_kind = 
-000165a0: 6b69 6e64 0a20 2020 2020 2020 2069 6620  kind.        if 
-000165b0: 6120 6973 206e 6f74 204e 6f6e 6520 616e  a is not None an
-000165c0: 6420 6220 6973 206e 6f74 204e 6f6e 6520  d b is not None 
-000165d0: 616e 6420 6120 2520 6220 3d3d 2030 3a0a  and a % b == 0:.
-000165e0: 2020 2020 2020 2020 2020 2020 6f70 5f6b              op_k
-000165f0: 696e 6420 3d20 2274 7275 6564 6976 2220  ind = "truediv" 
-00016600: 2023 206d 616b 6573 2073 6f6d 6520 6f74   # makes some ot
-00016610: 6865 7220 6368 6563 6b73 2073 696d 706c  her checks simpl
-00016620: 6572 0a20 2020 2020 2020 206f 705f 6b69  er.        op_ki
-00016630: 6e64 202b 3d20 225f 2220 2b20 2822 7269  nd += "_" + ("ri
-00016640: 6768 7422 2069 6620 7269 6768 7420 656c  ght" if right el
-00016650: 7365 2022 6c65 6674 2229 0a20 2020 2020  se "left").     
-00016660: 2020 2072 6574 7572 6e20 5f64 2e44 696d     return _d.Dim
-00016670: 280a 2020 2020 2020 2020 2020 2020 6465  (.            de
-00016680: 7363 7269 7074 696f 6e3d 6465 7363 7269  scription=descri
-00016690: 7074 696f 6e2c 0a20 2020 2020 2020 2020  ption,.         
-000166a0: 2020 206b 696e 643d 6e75 6d65 7261 746f     kind=numerato
-000166b0: 722e 6b69 6e64 2c0a 2020 2020 2020 2020  r.kind,.        
-000166c0: 2020 2020 6469 6d65 6e73 696f 6e3d 6469      dimension=di
-000166d0: 6d5f 7661 6c75 652c 0a20 2020 2020 2020  m_value,.       
-000166e0: 2020 2020 2064 6572 6976 6564 5f66 726f       derived_fro
-000166f0: 6d5f 6f70 3d4f 7028 6b69 6e64 3d6f 705f  m_op=Op(kind=op_
-00016700: 6b69 6e64 2c20 696e 7075 7473 3d5b 6e75  kind, inputs=[nu
-00016710: 6d65 7261 746f 722c 2064 656e 6f6d 696e  merator, denomin
-00016720: 6174 6f72 5d29 2c0a 2020 2020 2020 2020  ator]),.        
-00016730: 2020 2020 6465 7269 7665 645f 6672 6f6d      derived_from
-00016740: 5f74 6167 3d6e 756d 6572 6174 6f72 2c0a  _tag=numerator,.
-00016750: 2020 2020 2020 2020 290a 0a20 2020 2064          )..    d
-00016760: 6566 2061 735f 6469 6d28 7365 6c66 293a  ef as_dim(self):
-00016770: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00016780: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
-00016790: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-000167a0: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
-000167b0: 6f6e 6528 293a 0a20 2020 2020 2020 2020  one():.         
-000167c0: 2020 2072 6574 7572 6e20 5f6d 616b 655f     return _make_
-000167d0: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
-000167e0: 6469 6d28 3129 0a20 2020 2020 2020 2069  dim(1).        i
-000167f0: 6620 6c65 6e28 7365 6c66 2e74 6572 6d73  f len(self.terms
-00016800: 2920 3d3d 2031 3a0a 2020 2020 2020 2020  ) == 1:.        
-00016810: 2020 2020 7265 7475 726e 2073 656c 662e      return self.
-00016820: 7465 726d 735b 305d 0a20 2020 2020 2020  terms[0].       
-00016830: 2064 696d 5f6b 696e 6420 3d20 5f67 6574   dim_kind = _get
-00016840: 5f6d 6572 6765 645f 6469 6d5f 6b69 6e64  _merged_dim_kind
-00016850: 2873 656c 662e 7465 726d 7329 0a20 2020  (self.terms).   
-00016860: 2020 2020 2072 6574 7572 6e20 5f64 2e44       return _d.D
-00016870: 696d 280a 2020 2020 2020 2020 2020 2020  im(.            
-00016880: 6b69 6e64 3d64 696d 5f6b 696e 642c 0a20  kind=dim_kind,. 
-00016890: 2020 2020 2020 2020 2020 2064 6573 6372             descr
-000168a0: 6970 7469 6f6e 3d22 2a22 2e6a 6f69 6e28  iption="*".join(
-000168b0: 6d61 7028 5f67 6574 5f64 6573 6372 6970  map(_get_descrip
-000168c0: 7469 6f6e 2c20 7365 6c66 2e74 6572 6d73  tion, self.terms
-000168d0: 2929 2c0a 2020 2020 2020 2020 2020 2020  )),.            
-000168e0: 6469 6d65 6e73 696f 6e3d 7365 6c66 2e64  dimension=self.d
-000168f0: 696d 656e 7369 6f6e 2c0a 2020 2020 2020  imension,.      
-00016900: 2020 2020 2020 6465 7269 7665 645f 6672        derived_fr
-00016910: 6f6d 5f6f 703d 4f70 286b 696e 643d 226d  om_op=Op(kind="m
-00016920: 756c 222c 2069 6e70 7574 733d 6c69 7374  ul", inputs=list
-00016930: 2873 656c 662e 7465 726d 7329 292c 0a20  (self.terms)),. 
-00016940: 2020 2020 2020 2020 2020 2064 6572 6976             deriv
-00016950: 6564 5f66 726f 6d5f 7461 673d 7365 6c66  ed_from_tag=self
-00016960: 2e72 6570 7265 7365 6e74 6174 6976 655f  .representative_
-00016970: 7461 6728 292c 0a20 2020 2020 2020 2029  tag(),.        )
-00016980: 0a0a 2020 2020 6465 6620 7265 7072 6573  ..    def repres
-00016990: 656e 7461 7469 7665 5f74 6167 2873 656c  entative_tag(sel
-000169a0: 6629 3a0a 2020 2020 2020 2020 2222 220a  f):.        """.
-000169b0: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
-000169c0: 4469 6d7c 4e6f 6e65 0a20 2020 2020 2020  Dim|None.       
-000169d0: 2022 2222 0a20 2020 2020 2020 2023 2041   """.        # A
-000169e0: 6c73 6f20 7365 6520 4469 6d2e 5f4f 704c  lso see Dim._OpL
-000169f0: 696e 6561 7254 6572 6d2e 7265 7072 6573  inearTerm.repres
-00016a00: 656e 7461 7469 7665 5f74 6167 2829 2e0a  entative_tag()..
-00016a10: 2020 2020 2020 2020 2320 4669 7273 7420          # First 
-00016a20: 6669 6e64 2061 6e79 2064 796e 616d 6963  find any dynamic
-00016a30: 2e0a 2020 2020 2020 2020 666f 7220 7465  ..        for te
-00016a40: 726d 5f20 696e 2073 656c 662e 7465 726d  rm_ in self.term
-00016a50: 733a 0a20 2020 2020 2020 2020 2020 2069  s:.            i
-00016a60: 6620 7465 726d 5f2e 6973 5f64 796e 616d  f term_.is_dynam
-00016a70: 6963 2829 3a0a 2020 2020 2020 2020 2020  ic():.          
-00016a80: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
-00016a90: 6d5f 0a20 2020 2020 2020 2023 204e 6f77  m_.        # Now
-00016aa0: 2066 696e 6420 6e6f 6e2d 756e 7370 6563   find non-unspec
-00016ab0: 6966 6965 642e 0a20 2020 2020 2020 2066  ified..        f
-00016ac0: 6f72 2074 6572 6d5f 2069 6e20 7365 6c66  or term_ in self
-00016ad0: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
-00016ae0: 2020 2020 6966 2074 6572 6d5f 2e6b 696e      if term_.kin
-00016af0: 6420 213d 2044 696d 5479 7065 732e 556e  d != DimTypes.Un
-00016b00: 7370 6563 6966 6965 643a 0a20 2020 2020  specified:.     
-00016b10: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00016b20: 6e20 7465 726d 5f0a 2020 2020 2020 2020  n term_.        
-00016b30: 2320 4e6f 7720 6669 6e64 2061 6e79 2e0a  # Now find any..
-00016b40: 2020 2020 2020 2020 666f 7220 7465 726d          for term
-00016b50: 5f20 696e 2073 656c 662e 7465 726d 733a  _ in self.terms:
-00016b60: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00016b70: 7572 6e20 7465 726d 5f0a 2020 2020 2020  urn term_.      
-00016b80: 2020 7265 7475 726e 204e 6f6e 650a 0a0a    return None...
-00016b90: 636c 6173 7320 5f4f 704c 696e 6561 7254  class _OpLinearT
-00016ba0: 6572 6d3a 0a20 2020 2022 2222 0a20 2020  erm:.    """.   
-00016bb0: 2072 6570 7265 7365 6e74 7320 7374 6820   represents sth 
-00016bc0: 6c69 6b65 2061 202a 2062 202b 2063 0a20  like a * b + c. 
-00016bd0: 2020 2022 2222 0a0a 2020 2020 4063 6c61     """..    @cla
-00016be0: 7373 6d65 7468 6f64 0a20 2020 2064 6566  ssmethod.    def
-00016bf0: 2066 726f 6d5f 6469 6d28 636c 732c 2064   from_dim(cls, d
-00016c00: 696d 293a 0a20 2020 2020 2020 2022 2222  im):.        """
-00016c10: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00016c20: 4469 6d20 6469 6d3a 0a20 2020 2020 2020  Dim dim:.       
-00016c30: 203a 7274 7970 653a 2044 696d 2e5f 4f70   :rtype: Dim._Op
-00016c40: 4c69 6e65 6172 5465 726d 0a20 2020 2020  LinearTerm.     
-00016c50: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
-00016c60: 6573 203d 2063 6c73 2e7a 6572 6f28 290a  es = cls.zero().
-00016c70: 2020 2020 2020 2020 7265 732e 6578 7465          res.exte
-00016c80: 6e64 5f61 6464 5f73 7562 5f28 6469 6d2c  nd_add_sub_(dim,
-00016c90: 206b 696e 643d 2261 6464 222c 2072 6967   kind="add", rig
-00016ca0: 6874 3d54 7275 6529 0a20 2020 2020 2020  ht=True).       
-00016cb0: 2072 6574 7572 6e20 7265 730a 0a20 2020   return res..   
-00016cc0: 2040 636c 6173 736d 6574 686f 640a 2020   @classmethod.  
-00016cd0: 2020 6465 6620 7a65 726f 2863 6c73 293a    def zero(cls):
-00016ce0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00016cf0: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
-00016d00: 2e5f 4f70 4c69 6e65 6172 5465 726d 0a20  ._OpLinearTerm. 
-00016d10: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00016d20: 2020 2072 6574 7572 6e20 5f4f 704c 696e     return _OpLin
-00016d30: 6561 7254 6572 6d28 5b5d 290a 0a20 2020  earTerm([])..   
-00016d40: 2064 6566 205f 5f69 6e69 745f 5f28 7365   def __init__(se
-00016d50: 6c66 2c20 7465 726d 7329 3a0a 2020 2020  lf, terms):.    
-00016d60: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-00016d70: 3a70 6172 616d 206c 6973 745b 4469 6d2e  :param list[Dim.
-00016d80: 5f4f 704d 756c 7454 6572 6d5d 2074 6572  _OpMultTerm] ter
-00016d90: 6d73 3a0a 2020 2020 2020 2020 2222 220a  ms:.        """.
-00016da0: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
-00016db0: 6d73 203d 2074 6572 6d73 0a0a 2020 2020  ms = terms..    
-00016dc0: 6465 6620 5f5f 6861 7368 5f5f 2873 656c  def __hash__(sel
-00016dd0: 6629 3a0a 2020 2020 2020 2020 7265 7475  f):.        retu
-00016de0: 726e 2068 6173 6828 7475 706c 6528 7365  rn hash(tuple(se
-00016df0: 6c66 2e74 6572 6d73 2929 0a0a 2020 2020  lf.terms))..    
-00016e00: 6465 6620 5f5f 6571 5f5f 2873 656c 662c  def __eq__(self,
-00016e10: 206f 7468 6572 293a 0a20 2020 2020 2020   other):.       
-00016e20: 2069 6620 6973 696e 7374 616e 6365 286f   if isinstance(o
-00016e30: 7468 6572 2c20 5f4f 704c 696e 6561 7254  ther, _OpLinearT
-00016e40: 6572 6d29 3a0a 2020 2020 2020 2020 2020  erm):.          
-00016e50: 2020 7265 7475 726e 2073 656c 662e 7465    return self.te
-00016e60: 726d 7320 3d3d 206f 7468 6572 2e74 6572  rms == other.ter
-00016e70: 6d73 0a20 2020 2020 2020 2072 6574 7572  ms.        retur
-00016e80: 6e20 4661 6c73 650a 0a20 2020 2064 6566  n False..    def
-00016e90: 205f 5f6e 655f 5f28 7365 6c66 2c20 6f74   __ne__(self, ot
-00016ea0: 6865 7229 3a0a 2020 2020 2020 2020 7265  her):.        re
-00016eb0: 7475 726e 206e 6f74 2073 656c 662e 5f5f  turn not self.__
-00016ec0: 6571 5f5f 286f 7468 6572 290a 0a20 2020  eq__(other)..   
-00016ed0: 2064 6566 2061 735f 6469 6d28 7365 6c66   def as_dim(self
-00016ee0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
-00016ef0: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
-00016f00: 696d 0a20 2020 2020 2020 2022 2222 0a20  im.        """. 
-00016f10: 2020 2020 2020 2069 6620 7365 6c66 2e69         if self.i
-00016f20: 735f 7a65 726f 2829 3a0a 2020 2020 2020  s_zero():.      
-00016f30: 2020 2020 2020 7265 7475 726e 205f 6d61        return _ma
-00016f40: 6b65 5f63 6f6e 7374 616e 745f 7374 6174  ke_constant_stat
-00016f50: 6963 5f64 696d 2830 290a 2020 2020 2020  ic_dim(0).      
-00016f60: 2020 6966 206c 656e 2873 656c 662e 7465    if len(self.te
-00016f70: 726d 7329 203d 3d20 313a 0a20 2020 2020  rms) == 1:.     
-00016f80: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
-00016f90: 6c66 2e74 6572 6d73 5b30 5d2e 6173 5f64  lf.terms[0].as_d
-00016fa0: 696d 2829 0a20 2020 2020 2020 2061 6464  im().        add
-00016fb0: 5f70 6172 7473 203d 205b 5d0a 2020 2020  _parts = [].    
-00016fc0: 2020 2020 6465 7363 5f70 6172 7473 203d      desc_parts =
-00016fd0: 205b 5d0a 2020 2020 2020 2020 6469 6d20   [].        dim 
-00016fe0: 3d20 300a 2020 2020 2020 2020 666f 7220  = 0.        for 
-00016ff0: 7465 726d 2069 6e20 7365 6c66 2e74 6572  term in self.ter
-00017000: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
-00017010: 7320 3d20 7465 726d 2e61 735f 6469 6d28  s = term.as_dim(
-00017020: 290a 2020 2020 2020 2020 2020 2020 6164  ).            ad
-00017030: 645f 7061 7274 732e 6170 7065 6e64 2873  d_parts.append(s
-00017040: 290a 2020 2020 2020 2020 2020 2020 6465  ).            de
-00017050: 7363 5f70 6172 7473 2e61 7070 656e 6428  sc_parts.append(
-00017060: 5f67 6574 5f64 6573 6372 6970 7469 6f6e  _get_description
-00017070: 2873 2929 0a20 2020 2020 2020 2020 2020  (s)).           
-00017080: 2069 6620 6469 6d20 6973 206e 6f74 204e   if dim is not N
-00017090: 6f6e 6520 616e 6420 732e 6469 6d65 6e73  one and s.dimens
-000170a0: 696f 6e20 6973 206e 6f74 204e 6f6e 653a  ion is not None:
-000170b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000170c0: 2064 696d 202b 3d20 732e 6469 6d65 6e73   dim += s.dimens
-000170d0: 696f 6e0a 2020 2020 2020 2020 2020 2020  ion.            
-000170e0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
-000170f0: 2020 2020 2020 6469 6d20 3d20 4e6f 6e65        dim = None
-00017100: 0a20 2020 2020 2020 2069 6620 6c65 6e28  .        if len(
-00017110: 6164 645f 7061 7274 7329 203d 3d20 313a  add_parts) == 1:
-00017120: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
-00017130: 7572 6e20 6164 645f 7061 7274 735b 305d  urn add_parts[0]
-00017140: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00017150: 5f64 2e44 696d 280a 2020 2020 2020 2020  _d.Dim(.        
-00017160: 2020 2020 6b69 6e64 3d5f 6765 745f 6d65      kind=_get_me
-00017170: 7267 6564 5f64 696d 5f6b 696e 6428 6164  rged_dim_kind(ad
-00017180: 645f 7061 7274 7329 2c0a 2020 2020 2020  d_parts),.      
-00017190: 2020 2020 2020 6465 7363 7269 7074 696f        descriptio
-000171a0: 6e3d 222b 222e 6a6f 696e 2864 6573 635f  n="+".join(desc_
-000171b0: 7061 7274 7329 2c0a 2020 2020 2020 2020  parts),.        
-000171c0: 2020 2020 6469 6d65 6e73 696f 6e3d 6469      dimension=di
-000171d0: 6d2c 0a20 2020 2020 2020 2020 2020 2064  m,.            d
-000171e0: 6572 6976 6564 5f66 726f 6d5f 6f70 3d4f  erived_from_op=O
-000171f0: 7028 6b69 6e64 3d22 6164 6422 2c20 696e  p(kind="add", in
-00017200: 7075 7473 3d61 6464 5f70 6172 7473 292c  puts=add_parts),
-00017210: 0a20 2020 2020 2020 2020 2020 2064 6572  .            der
-00017220: 6976 6564 5f66 726f 6d5f 7461 673d 7365  ived_from_tag=se
-00017230: 6c66 2e72 6570 7265 7365 6e74 6174 6976  lf.representativ
-00017240: 655f 7461 6728 292c 0a20 2020 2020 2020  e_tag(),.       
-00017250: 2029 0a0a 2020 2020 6465 6620 5f5f 7265   )..    def __re
-00017260: 7072 5f5f 2873 656c 6629 3a0a 2020 2020  pr__(self):.    
-00017270: 2020 2020 7265 7475 726e 2022 4469 6d2e      return "Dim.
-00017280: 5f4f 704c 696e 6561 7254 6572 6d28 2572  _OpLinearTerm(%r
-00017290: 2922 2025 2028 7365 6c66 2e74 6572 6d73  )" % (self.terms
-000172a0: 2c29 0a0a 2020 2020 6465 6620 6973 5f7a  ,)..    def is_z
-000172b0: 6572 6f28 7365 6c66 293a 0a20 2020 2020  ero(self):.     
-000172c0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
-000172d0: 7274 7970 653a 2062 6f6f 6c0a 2020 2020  rtype: bool.    
-000172e0: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
-000172f0: 7265 7475 726e 206e 6f74 2073 656c 662e  return not self.
-00017300: 7465 726d 730a 0a20 2020 2064 6566 2065  terms..    def e
-00017310: 7874 656e 645f 6164 645f 7375 625f 2873  xtend_add_sub_(s
-00017320: 656c 662c 206f 7468 6572 2c20 6b69 6e64  elf, other, kind
-00017330: 2c20 7269 6768 7429 3a0a 2020 2020 2020  , right):.      
-00017340: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
-00017350: 6172 616d 2044 696d 7c69 6e74 206f 7468  aram Dim|int oth
-00017360: 6572 3a0a 2020 2020 2020 2020 3a70 6172  er:.        :par
-00017370: 616d 2073 7472 206b 696e 643a 2022 6164  am str kind: "ad
-00017380: 6422 206f 7220 2273 7562 220a 2020 2020  d" or "sub".    
-00017390: 2020 2020 3a70 6172 616d 2062 6f6f 6c20      :param bool 
-000173a0: 7269 6768 743a 206f 7220 6c65 6674 2e20  right: or left. 
-000173b0: 7269 6768 7420 6d65 616e 7320 7365 6c66  right means self
-000173c0: 202b 206f 7468 6572 2c20 6c65 6674 206d   + other, left m
-000173d0: 6561 6e73 206f 7468 6572 202b 2073 656c  eans other + sel
-000173e0: 660a 2020 2020 2020 2020 2222 220a 2020  f.        """.  
-000173f0: 2020 2020 2020 6173 7365 7274 206b 696e        assert kin
-00017400: 6420 696e 207b 2261 6464 222c 2022 7375  d in {"add", "su
-00017410: 6222 7d0a 2020 2020 2020 2020 6f74 6865  b"}.        othe
-00017420: 7220 3d20 7365 6c66 2e5f 6d61 6b65 5f64  r = self._make_d
-00017430: 696d 286f 7468 6572 2c20 6b69 6e64 3d6b  im(other, kind=k
-00017440: 696e 6429 0a20 2020 2020 2020 2069 6620  ind).        if 
-00017450: 6f74 6865 722e 6973 5f63 6f6e 7374 616e  other.is_constan
-00017460: 745f 7374 6174 6963 5f64 696d 2829 2061  t_static_dim() a
-00017470: 6e64 206f 7468 6572 2e64 696d 656e 7369  nd other.dimensi
-00017480: 6f6e 203d 3d20 303a 0a20 2020 2020 2020  on == 0:.       
-00017490: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
-000174a0: 2020 2020 6966 206f 7468 6572 2e64 6572      if other.der
-000174b0: 6976 6564 5f66 726f 6d5f 6f70 2061 6e64  ived_from_op and
-000174c0: 206f 7468 6572 2e64 6572 6976 6564 5f66   other.derived_f
-000174d0: 726f 6d5f 6f70 2e6b 696e 6420 3d3d 2022  rom_op.kind == "
-000174e0: 6164 6422 3a0a 2020 2020 2020 2020 2020  add":.          
-000174f0: 2020 666f 7220 6f74 6865 725f 2069 6e20    for other_ in 
-00017500: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
-00017510: 6f6d 5f6f 702e 696e 7075 7473 2069 6620  om_op.inputs if 
-00017520: 7269 6768 7420 656c 7365 2072 6576 6572  right else rever
-00017530: 7365 6428 6f74 6865 722e 6465 7269 7665  sed(other.derive
-00017540: 645f 6672 6f6d 5f6f 702e 696e 7075 7473  d_from_op.inputs
-00017550: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00017560: 2020 2073 656c 662e 6578 7465 6e64 5f61     self.extend_a
-00017570: 6464 5f73 7562 5f28 6f74 6865 725f 2c20  dd_sub_(other_, 
-00017580: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
-00017590: 3d72 6967 6874 290a 2020 2020 2020 2020  =right).        
-000175a0: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
-000175b0: 2020 2074 6572 6d20 3d20 5f4f 704d 756c     term = _OpMul
-000175c0: 7454 6572 6d2e 6672 6f6d 5f64 696d 286f  tTerm.from_dim(o
-000175d0: 7468 6572 290a 2020 2020 2020 2020 6e65  ther).        ne
-000175e0: 675f 7465 726d 203d 2074 6572 6d2e 6e65  g_term = term.ne
-000175f0: 6761 7469 7665 2829 0a20 2020 2020 2020  gative().       
-00017600: 2069 6620 6b69 6e64 203d 3d20 2273 7562   if kind == "sub
-00017610: 223a 0a20 2020 2020 2020 2020 2020 2074  ":.            t
-00017620: 6572 6d2c 206e 6567 5f74 6572 6d20 3d20  erm, neg_term = 
-00017630: 6e65 675f 7465 726d 2c20 7465 726d 0a20  neg_term, term. 
-00017640: 2020 2020 2020 206d 6f73 745f 7265 6365         most_rece
-00017650: 6e74 5f74 6572 6d20 3d20 7365 6c66 2e74  nt_term = self.t
-00017660: 6572 6d73 5b2d 3120 6966 2072 6967 6874  erms[-1 if right
-00017670: 2065 6c73 6520 305d 2069 6620 7365 6c66   else 0] if self
-00017680: 2e74 6572 6d73 2065 6c73 6520 4e6f 6e65  .terms else None
-00017690: 0a20 2020 2020 2020 2069 6620 6d6f 7374  .        if most
-000176a0: 5f72 6563 656e 745f 7465 726d 3a0a 2020  _recent_term:.  
-000176b0: 2020 2020 2020 2020 2020 6966 206d 6f73            if mos
-000176c0: 745f 7265 6365 6e74 5f74 6572 6d20 3d3d  t_recent_term ==
-000176d0: 206e 6567 5f74 6572 6d3a 0a20 2020 2020   neg_term:.     
-000176e0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
-000176f0: 7465 726d 732e 706f 7028 2d31 2069 6620  terms.pop(-1 if 
-00017700: 7269 6768 7420 656c 7365 2030 290a 2020  right else 0).  
-00017710: 2020 2020 2020 2020 2020 2020 2020 7265                re
-00017720: 7475 726e 0a20 2020 2020 2020 2020 2020  turn.           
-00017730: 2069 6620 6d6f 7374 5f72 6563 656e 745f   if most_recent_
-00017740: 7465 726d 2e69 735f 636f 6e73 7461 6e74  term.is_constant
-00017750: 5f73 7461 7469 635f 6469 6d28 2920 616e  _static_dim() an
-00017760: 6420 7465 726d 2e69 735f 636f 6e73 7461  d term.is_consta
-00017770: 6e74 5f73 7461 7469 635f 6469 6d28 293a  nt_static_dim():
-00017780: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017790: 2073 656c 662e 7465 726d 735b 2d31 2069   self.terms[-1 i
-000177a0: 6620 7269 6768 7420 656c 7365 2030 5d20  f right else 0] 
-000177b0: 3d20 5f4f 704d 756c 7454 6572 6d2e 6672  = _OpMultTerm.fr
-000177c0: 6f6d 5f64 696d 280a 2020 2020 2020 2020  om_dim(.        
-000177d0: 2020 2020 2020 2020 2020 2020 5f6d 616b              _mak
-000177e0: 655f 636f 6e73 7461 6e74 5f73 7461 7469  e_constant_stati
-000177f0: 635f 6469 6d28 6d6f 7374 5f72 6563 656e  c_dim(most_recen
-00017800: 745f 7465 726d 2e64 696d 656e 7369 6f6e  t_term.dimension
-00017810: 202b 2074 6572 6d2e 6469 6d65 6e73 696f   + term.dimensio
-00017820: 6e2c 206b 696e 643d 6f74 6865 722e 6b69  n, kind=other.ki
-00017830: 6e64 290a 2020 2020 2020 2020 2020 2020  nd).            
-00017840: 2020 2020 290a 2020 2020 2020 2020 2020      ).          
-00017850: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00017860: 2020 2020 2020 2020 2069 6620 6d6f 7374           if most
-00017870: 5f72 6563 656e 745f 7465 726d 2e74 6572  _recent_term.ter
-00017880: 6d73 2061 6e64 2074 6572 6d2e 7465 726d  ms and term.term
-00017890: 7320 616e 6420 6d6f 7374 5f72 6563 656e  s and most_recen
-000178a0: 745f 7465 726d 2e74 6572 6d73 5b2d 315d  t_term.terms[-1]
-000178b0: 203d 3d20 7465 726d 2e74 6572 6d73 5b2d   == term.terms[-
-000178c0: 315d 3a0a 2020 2020 2020 2020 2020 2020  1]:.            
-000178d0: 2020 2020 2320 4d65 7267 6520 7465 726d      # Merge term
-000178e0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-000178f0: 2020 6120 3d20 5f4f 704d 756c 7454 6572    a = _OpMultTer
-00017900: 6d2e 6672 6f6d 5f64 696d 5f66 6163 746f  m.from_dim_facto
-00017910: 7273 286d 6f73 745f 7265 6365 6e74 5f74  rs(most_recent_t
-00017920: 6572 6d2e 7465 726d 735b 3a2d 315d 292e  erm.terms[:-1]).
-00017930: 6173 5f64 696d 2829 0a20 2020 2020 2020  as_dim().       
-00017940: 2020 2020 2020 2020 2062 203d 205f 4f70           b = _Op
-00017950: 4d75 6c74 5465 726d 2e66 726f 6d5f 6469  MultTerm.from_di
-00017960: 6d5f 6661 6374 6f72 7328 7465 726d 2e74  m_factors(term.t
-00017970: 6572 6d73 5b3a 2d31 5d29 2e61 735f 6469  erms[:-1]).as_di
-00017980: 6d28 290a 2020 2020 2020 2020 2020 2020  m().            
-00017990: 2020 2020 7265 7320 3d20 5f4f 704d 756c      res = _OpMul
-000179a0: 7454 6572 6d2e 6672 6f6d 5f64 696d 2828  tTerm.from_dim((
-000179b0: 6120 2b20 6229 2069 6620 7269 6768 7420  a + b) if right 
-000179c0: 656c 7365 2028 6220 2b20 6129 290a 2020  else (b + a)).  
-000179d0: 2020 2020 2020 2020 2020 2020 2020 7265                re
-000179e0: 732e 6578 7465 6e64 5f6d 756c 5f64 6976  s.extend_mul_div
-000179f0: 5f28 7465 726d 2e74 6572 6d73 5b2d 315d  _(term.terms[-1]
-00017a00: 2c20 6b69 6e64 3d22 6d75 6c22 2c20 7269  , kind="mul", ri
-00017a10: 6768 743d 5472 7565 290a 2020 2020 2020  ght=True).      
-00017a20: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00017a30: 6572 6d73 5b2d 3120 6966 2072 6967 6874  erms[-1 if right
-00017a40: 2065 6c73 6520 305d 203d 2072 6573 0a20   else 0] = res. 
-00017a50: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00017a60: 6574 7572 6e0a 2020 2020 2020 2020 6966  eturn.        if
-00017a70: 2072 6967 6874 3a0a 2020 2020 2020 2020   right:.        
-00017a80: 2020 2020 7365 6c66 2e74 6572 6d73 2e61      self.terms.a
-00017a90: 7070 656e 6428 7465 726d 290a 2020 2020  ppend(term).    
-00017aa0: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
-00017ab0: 2020 2020 2020 7365 6c66 2e74 6572 6d73        self.terms
-00017ac0: 2e69 6e73 6572 7428 302c 2074 6572 6d29  .insert(0, term)
-00017ad0: 0a0a 2020 2020 6465 6620 6578 7465 6e64  ..    def extend
-00017ae0: 5f6d 756c 5f64 6976 5f28 7365 6c66 2c20  _mul_div_(self, 
-00017af0: 6f74 6865 722c 206b 696e 642c 2072 6967  other, kind, rig
-00017b00: 6874 293a 0a20 2020 2020 2020 2022 2222  ht):.        """
-00017b10: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
-00017b20: 4469 6d7c 696e 7420 6f74 6865 723a 0a20  Dim|int other:. 
-00017b30: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
-00017b40: 7220 6b69 6e64 3a20 226d 756c 2220 6f72  r kind: "mul" or
-00017b50: 2022 6365 696c 6469 7622 0a20 2020 2020   "ceildiv".     
-00017b60: 2020 203a 7061 7261 6d20 626f 6f6c 2072     :param bool r
-00017b70: 6967 6874 3a20 6f72 206c 6566 742e 2072  ight: or left. r
-00017b80: 6967 6874 206d 6561 6e73 2073 656c 6620  ight means self 
-00017b90: 2a20 6f74 6865 722c 206c 6566 7420 6d65  * other, left me
-00017ba0: 616e 7320 6f74 6865 7220 2a20 7365 6c66  ans other * self
-00017bb0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
-00017bc0: 2020 2020 2061 7373 6572 7420 6b69 6e64       assert kind
-00017bd0: 2069 6e20 7b22 6d75 6c22 2c20 2266 6c6f   in {"mul", "flo
-00017be0: 6f72 6469 7622 2c20 2274 7275 6564 6976  ordiv", "truediv
-00017bf0: 222c 2022 6365 696c 6469 7622 7d0a 2020  ", "ceildiv"}.  
-00017c00: 2020 2020 2020 6f74 6865 7220 3d20 7365        other = se
-00017c10: 6c66 2e5f 6d61 6b65 5f64 696d 286f 7468  lf._make_dim(oth
-00017c20: 6572 2c20 6b69 6e64 3d6b 696e 6429 0a20  er, kind=kind). 
-00017c30: 2020 2020 2020 2069 6620 6b69 6e64 203d         if kind =
-00017c40: 3d20 226d 756c 2220 616e 6420 7269 6768  = "mul" and righ
-00017c50: 743a 0a20 2020 2020 2020 2020 2020 2069  t:.            i
-00017c60: 6620 6e6f 7420 616c 6c28 7465 726d 2e63  f not all(term.c
-00017c70: 616e 5f73 696d 706c 6966 7928 6f74 6865  an_simplify(othe
-00017c80: 722c 206b 696e 643d 6b69 6e64 2c20 7269  r, kind=kind, ri
-00017c90: 6768 743d 7269 6768 7429 2066 6f72 2074  ght=right) for t
-00017ca0: 6572 6d20 696e 2073 656c 662e 7465 726d  erm in self.term
-00017cb0: 7329 3a0a 2020 2020 2020 2020 2020 2020  s):.            
-00017cc0: 2020 2020 2320 446f 2069 7420 7468 6520      # Do it the 
-00017cd0: 6f74 6865 7220 7761 7920 6172 6f75 6e64  other way around
-00017ce0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00017cf0: 2073 656c 662e 7465 726d 732c 206f 7468   self.terms, oth
-00017d00: 6572 203d 205f 4f70 4c69 6e65 6172 5465  er = _OpLinearTe
-00017d10: 726d 2e66 726f 6d5f 6469 6d28 6f74 6865  rm.from_dim(othe
-00017d20: 7229 2e74 6572 6d73 2c20 7365 6c66 2e61  r).terms, self.a
-00017d30: 735f 6469 6d28 290a 2020 2020 2020 2020  s_dim().        
-00017d40: 2020 2020 2020 2020 7269 6768 7420 3d20          right = 
-00017d50: 4661 6c73 650a 2020 2020 2020 2020 6966  False.        if
-00017d60: 206f 7468 6572 2e69 735f 636f 6e73 7461   other.is_consta
-00017d70: 6e74 5f73 7461 7469 635f 6469 6d28 2920  nt_static_dim() 
-00017d80: 616e 6420 6f74 6865 722e 6469 6d65 6e73  and other.dimens
-00017d90: 696f 6e20 3d3d 2031 3a0a 2020 2020 2020  ion == 1:.      
-00017da0: 2020 2020 2020 7265 7475 726e 0a20 2020        return.   
-00017db0: 2020 2020 2069 6620 6b69 6e64 2e65 6e64       if kind.end
-00017dc0: 7377 6974 6828 2264 6976 2229 2061 6e64  swith("div") and
-00017dd0: 206c 656e 2873 656c 662e 7465 726d 7329   len(self.terms)
-00017de0: 203e 3d20 323a 0a20 2020 2020 2020 2020   >= 2:.         
-00017df0: 2020 2069 6620 616e 7928 6e6f 7420 7465     if any(not te
-00017e00: 726d 2e64 6976 6973 6962 6c65 286f 7468  rm.divisible(oth
-00017e10: 6572 2c20 7269 6768 743d 7269 6768 7429  er, right=right)
-00017e20: 2066 6f72 2074 6572 6d20 696e 2073 656c   for term in sel
-00017e30: 662e 7465 726d 7329 3a0a 2020 2020 2020  f.terms):.      
-00017e40: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
-00017e50: 6572 6d73 203d 205b 0a20 2020 2020 2020  erms = [.       
-00017e60: 2020 2020 2020 2020 2020 2020 205f 4f70               _Op
-00017e70: 4d75 6c74 5465 726d 2e66 726f 6d5f 6469  MultTerm.from_di
-00017e80: 6d28 5f4f 704d 756c 7454 6572 6d2e 6e65  m(_OpMultTerm.ne
-00017e90: 775f 6469 765f 6469 6d28 7365 6c66 2e61  w_div_dim(self.a
-00017ea0: 735f 6469 6d28 292c 206f 7468 6572 2c20  s_dim(), other, 
-00017eb0: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
-00017ec0: 3d72 6967 6874 2929 0a20 2020 2020 2020  =right)).       
-00017ed0: 2020 2020 2020 2020 205d 0a20 2020 2020           ].     
-00017ee0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
-00017ef0: 6e0a 2020 2020 2020 2020 666f 7220 7465  n.        for te
-00017f00: 726d 2069 6e20 7365 6c66 2e74 6572 6d73  rm in self.terms
-00017f10: 3a0a 2020 2020 2020 2020 2020 2020 7465  :.            te
-00017f20: 726d 2e65 7874 656e 645f 6d75 6c5f 6469  rm.extend_mul_di
-00017f30: 765f 286f 7468 6572 2c20 6b69 6e64 3d6b  v_(other, kind=k
-00017f40: 696e 642c 2072 6967 6874 3d72 6967 6874  ind, right=right
-00017f50: 290a 0a20 2020 2064 6566 205f 6d61 6b65  )..    def _make
-00017f60: 5f64 696d 2873 656c 662c 206f 7468 6572  _dim(self, other
-00017f70: 2c20 6b69 6e64 293a 0a20 2020 2020 2020  , kind):.       
-00017f80: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
-00017f90: 7261 6d20 4469 6d7c 696e 7420 6f74 6865  ram Dim|int othe
-00017fa0: 723a 0a20 2020 2020 2020 203a 7061 7261  r:.        :para
-00017fb0: 6d20 7374 7220 6b69 6e64 3a0a 2020 2020  m str kind:.    
-00017fc0: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
-00017fd0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
-00017fe0: 2020 2020 6966 2069 7369 6e73 7461 6e63      if isinstanc
-00017ff0: 6528 6f74 6865 722c 2069 6e74 293a 0a20  e(other, int):. 
-00018000: 2020 2020 2020 2020 2020 2062 6173 655f             base_
-00018010: 7461 6720 3d20 7365 6c66 2e72 6570 7265  tag = self.repre
-00018020: 7365 6e74 6174 6976 655f 7461 6728 290a  sentative_tag().
-00018030: 2020 2020 2020 2020 2020 2020 7265 7475              retu
-00018040: 726e 205f 6d61 6b65 5f63 6f6e 7374 616e  rn _make_constan
-00018050: 745f 7374 6174 6963 5f64 696d 286f 7468  t_static_dim(oth
-00018060: 6572 2c20 6b69 6e64 3d62 6173 655f 7461  er, kind=base_ta
-00018070: 672e 6b69 6e64 2069 6620 6261 7365 5f74  g.kind if base_t
-00018080: 6167 2065 6c73 6520 4e6f 6e65 290a 2020  ag else None).  
-00018090: 2020 2020 2020 656c 6966 2069 7369 6e73        elif isins
-000180a0: 7461 6e63 6528 6f74 6865 722c 205f 642e  tance(other, _d.
-000180b0: 4469 6d29 3a0a 2020 2020 2020 2020 2020  Dim):.          
-000180c0: 2020 7265 7475 726e 206f 7468 6572 2e67    return other.g
-000180d0: 6574 5f73 616d 655f 6261 7365 2829 0a20  et_same_base(). 
-000180e0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000180f0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
-00018100: 7970 6545 7272 6f72 2822 2573 2025 7320  ypeError("%s %s 
-00018110: 2573 2069 6e76 616c 6964 2066 6f72 2074  %s invalid for t
-00018120: 7970 6520 2573 2220 2520 2873 656c 662c  ype %s" % (self,
-00018130: 206b 696e 642c 206f 7468 6572 2c20 7479   kind, other, ty
-00018140: 7065 286f 7468 6572 2929 290a 0a20 2020  pe(other)))..   
-00018150: 2064 6566 2072 6570 7265 7365 6e74 6174   def representat
-00018160: 6976 655f 7461 6728 7365 6c66 293a 0a20  ive_tag(self):. 
-00018170: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00018180: 2020 203a 7274 7970 653a 2044 696d 7c4e     :rtype: Dim|N
-00018190: 6f6e 650a 2020 2020 2020 2020 2222 220a  one.        """.
-000181a0: 2020 2020 2020 2020 2320 4669 7273 7420          # First 
-000181b0: 6669 6e64 2061 6e79 2064 796e 616d 6963  find any dynamic
-000181c0: 2e0a 2020 2020 2020 2020 666f 7220 7465  ..        for te
-000181d0: 726d 2069 6e20 7365 6c66 2e74 6572 6d73  rm in self.terms
-000181e0: 3a0a 2020 2020 2020 2020 2020 2020 666f  :.            fo
-000181f0: 7220 7465 726d 5f20 696e 2074 6572 6d2e  r term_ in term.
-00018200: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
-00018210: 2020 2020 2020 2069 6620 7465 726d 5f2e         if term_.
-00018220: 6973 5f64 796e 616d 6963 2829 3a0a 2020  is_dynamic():.  
-00018230: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018240: 2020 7265 7475 726e 2074 6572 6d5f 0a20    return term_. 
-00018250: 2020 2020 2020 2023 204e 6f77 2066 696e         # Now fin
-00018260: 6420 6e6f 6e2d 756e 7370 6563 6966 6965  d non-unspecifie
-00018270: 642e 0a20 2020 2020 2020 2066 6f72 2074  d..        for t
-00018280: 6572 6d20 696e 2073 656c 662e 7465 726d  erm in self.term
-00018290: 733a 0a20 2020 2020 2020 2020 2020 2066  s:.            f
-000182a0: 6f72 2074 6572 6d5f 2069 6e20 7465 726d  or term_ in term
-000182b0: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
-000182c0: 2020 2020 2020 2020 6966 2074 6572 6d5f          if term_
-000182d0: 2e6b 696e 6420 213d 2044 696d 5479 7065  .kind != DimType
-000182e0: 732e 556e 7370 6563 6966 6965 643a 0a20  s.Unspecified:. 
-000182f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00018300: 2020 2072 6574 7572 6e20 7465 726d 5f0a     return term_.
-00018310: 2020 2020 2020 2020 2320 4e6f 7720 6669          # Now fi
-00018320: 6e64 2061 6e79 2e0a 2020 2020 2020 2020  nd any..        
-00018330: 666f 7220 7465 726d 2069 6e20 7365 6c66  for term in self
-00018340: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
-00018350: 2020 2020 666f 7220 7465 726d 5f20 696e      for term_ in
-00018360: 2074 6572 6d2e 7465 726d 733a 0a20 2020   term.terms:.   
-00018370: 2020 2020 2020 2020 2020 2020 2072 6574               ret
-00018380: 7572 6e20 7465 726d 5f0a 2020 2020 2020  urn term_.      
-00018390: 2020 7265 7475 726e 204e 6f6e 650a 0a0a    return None...
-000183a0: 6465 6620 5f67 6574 5f6d 6572 6765 645f  def _get_merged_
-000183b0: 6469 6d5f 6b69 6e64 2864 696d 5f74 6167  dim_kind(dim_tag
-000183c0: 7329 3a0a 2020 2020 2222 220a 2020 2020  s):.    """.    
-000183d0: 3a70 6172 616d 206c 6973 745b 4469 6d5d  :param list[Dim]
-000183e0: 7c74 7570 6c65 5b44 696d 5d20 6469 6d5f  |tuple[Dim] dim_
-000183f0: 7461 6773 3a0a 2020 2020 3a72 6574 7572  tags:.    :retur
-00018400: 6e3a 2064 696d 206b 696e 640a 2020 2020  n: dim kind.    
-00018410: 3a72 7479 7065 3a20 456e 7469 7479 0a20  :rtype: Entity. 
-00018420: 2020 2022 2222 0a20 2020 2069 6620 616e     """.    if an
-00018430: 7928 7461 672e 6973 5f62 6174 6368 5f64  y(tag.is_batch_d
-00018440: 696d 2829 2066 6f72 2074 6167 2069 6e20  im() for tag in 
-00018450: 6469 6d5f 7461 6773 293a 0a20 2020 2020  dim_tags):.     
-00018460: 2020 2072 6574 7572 6e20 4469 6d54 7970     return DimTyp
-00018470: 6573 2e42 6174 6368 0a20 2020 2065 6c69  es.Batch.    eli
-00018480: 6620 616e 7928 7461 672e 6973 5f66 6561  f any(tag.is_fea
-00018490: 7475 7265 5f64 696d 2829 2066 6f72 2074  ture_dim() for t
-000184a0: 6167 2069 6e20 6469 6d5f 7461 6773 293a  ag in dim_tags):
-000184b0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-000184c0: 4469 6d54 7970 6573 2e46 6561 7475 7265  DimTypes.Feature
-000184d0: 0a20 2020 2065 6c73 653a 0a20 2020 2020  .    else:.     
-000184e0: 2020 2072 6574 7572 6e20 4469 6d54 7970     return DimTyp
-000184f0: 6573 2e53 7061 7469 616c 0a0a 0a64 6566  es.Spatial...def
-00018500: 2064 696d 5f63 6d70 5f76 616c 7565 286f   dim_cmp_value(o
-00018510: 626a 293a 0a20 2020 2022 2222 0a20 2020  bj):.    """.   
-00018520: 203a 7061 7261 6d20 4469 6d7c 5f4d 6172   :param Dim|_Mar
-00018530: 6b65 6444 696d 206f 626a 3a0a 2020 2020  kedDim obj:.    
-00018540: 3a72 6574 7572 6e3a 2061 6e79 7468 696e  :return: anythin
-00018550: 6720 7768 6963 6820 6361 6e20 6265 2063  g which can be c
-00018560: 6f6d 7061 7265 640a 2020 2020 2222 220a  ompared.    """.
-00018570: 2020 2020 2320 4d61 6b65 2044 696d 2061      # Make Dim a
-00018580: 6e64 205f 4d61 726b 6564 4469 6d20 636f  nd _MarkedDim co
-00018590: 6d70 6172 6162 6c65 2074 6f20 6561 6368  mparable to each
-000185a0: 206f 7468 6572 2e0a 2020 2020 2320 4e6f   other..    # No
-000185b0: 7465 2074 6861 7420 7468 6520 6f72 6465  te that the orde
-000185c0: 7220 6973 2072 6561 6c6c 7920 6172 6269  r is really arbi
-000185d0: 7472 6172 7920 616e 6420 646f 6573 206e  trary and does n
-000185e0: 6f74 206d 6174 7465 722e 0a20 2020 2069  ot matter..    i
-000185f0: 6620 6973 696e 7374 616e 6365 286f 626a  f isinstance(obj
-00018600: 2c20 5f64 2e44 696d 293a 0a20 2020 2020  , _d.Dim):.     
-00018610: 2020 206f 626a 203d 206f 626a 2e67 6574     obj = obj.get
-00018620: 5f73 616d 655f 6261 7365 2829 0a20 2020  _same_base().   
-00018630: 2020 2020 2072 6574 7572 6e20 280a 2020       return (.  
-00018640: 2020 2020 2020 2020 2020 2222 2c0a 2020            "",.  
-00018650: 2020 2020 2020 2020 2020 6f62 6a2e 6465            obj.de
-00018660: 7363 7269 7074 696f 6e2c 0a20 2020 2020  scription,.     
-00018670: 2020 2020 2020 206f 626a 2e6b 696e 642c         obj.kind,
-00018680: 0a20 2020 2020 2020 2020 2020 206f 626a  .            obj
-00018690: 2e64 696d 656e 7369 6f6e 2c0a 2020 2020  .dimension,.    
-000186a0: 2020 2020 2020 2020 6f62 6a2e 6479 6e5f          obj.dyn_
-000186b0: 7369 7a65 5f65 7874 2e64 696d 7320 6966  size_ext.dims if
-000186c0: 206f 626a 2e64 796e 5f73 697a 655f 6578   obj.dyn_size_ex
-000186d0: 7420 6973 206e 6f74 204e 6f6e 6520 656c  t is not None el
-000186e0: 7365 204e 6f6e 652c 0a20 2020 2020 2020  se None,.       
-000186f0: 2029 0a20 2020 2069 6620 6973 696e 7374   ).    if isinst
-00018700: 616e 6365 286f 626a 2c20 5f6d 2e4d 6172  ance(obj, _m.Mar
-00018710: 6b65 6444 696d 293a 0a20 2020 2020 2020  kedDim):.       
-00018720: 2072 6574 7572 6e20 6f62 6a2e 5f5f 636c   return obj.__cl
-00018730: 6173 735f 5f2e 5f5f 6e61 6d65 5f5f 2c20  ass__.__name__, 
-00018740: 6f62 6a2e 7461 670a 2020 2020 7265 7475  obj.tag.    retu
-00018750: 726e 206f 626a 0a                        rn obj.
+00009970: 7265 7475 726e 2028 785f 5f20 3c20 3029  return (x__ < 0)
+00009980: 2e61 6e79 2829 0a20 2020 2020 2020 2020  .any().         
+00009990: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+000099a0: 2878 5f5f 2c20 2869 6e74 2c20 666c 6f61  (x__, (int, floa
+000099b0: 742c 206e 756d 7079 2e6e 756d 6265 7229  t, numpy.number)
+000099c0: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000099d0: 2020 2072 6574 7572 6e20 785f 5f20 3c20     return x__ < 
+000099e0: 300a 2020 2020 2020 2020 2020 2020 6966  0.            if
+000099f0: 206e 6f74 2074 663a 0a20 2020 2020 2020   not tf:.       
+00009a00: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00009a10: 4661 6c73 650a 2020 2020 2020 2020 2020  False.          
+00009a20: 2020 6173 7365 7274 2069 7369 6e73 7461    assert isinsta
+00009a30: 6e63 6528 785f 5f2c 2074 662e 5465 6e73  nce(x__, tf.Tens
+00009a40: 6f72 290a 2020 2020 2020 2020 2020 2020  or).            
+00009a50: 785f 5f20 3d20 7465 6e73 6f72 5f75 7469  x__ = tensor_uti
+00009a60: 6c2e 636f 6e73 7461 6e74 5f76 616c 7565  l.constant_value
+00009a70: 2878 5f5f 290a 2020 2020 2020 2020 2020  (x__).          
+00009a80: 2020 6966 2078 5f5f 2069 7320 6e6f 7420    if x__ is not 
+00009a90: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00009aa0: 2020 2020 2020 7265 7475 726e 205f 6973        return _is
+00009ab0: 5f6e 6567 6174 6976 6528 785f 5f29 0a20  _negative(x__). 
+00009ac0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00009ad0: 6e20 4661 6c73 650a 0a20 2020 2020 2020  n False..       
+00009ae0: 2064 6566 205f 6269 6e5f 6f70 5f74 6628   def _bin_op_tf(
+00009af0: 612c 2062 293a 0a20 2020 2020 2020 2020  a, b):.         
+00009b00: 2020 2069 6620 7465 6d70 6c61 7465 5f6f     if template_o
+00009b10: 6e6c 793a 0a20 2020 2020 2020 2020 2020  nly:.           
+00009b20: 2020 2020 2072 6574 7572 6e20 4e6f 6e65       return None
+00009b30: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00009b40: 6120 6973 204e 6f6e 6520 6f72 2062 2069  a is None or b i
+00009b50: 7320 4e6f 6e65 3a0a 2020 2020 2020 2020  s None:.        
+00009b60: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00009b70: 6f6e 650a 2020 2020 2020 2020 2020 2020  one.            
+00009b80: 6173 7365 7274 2069 7369 6e73 7461 6e63  assert isinstanc
+00009b90: 6528 612c 2074 662e 5465 6e73 6f72 2920  e(a, tf.Tensor) 
+00009ba0: 616e 6420 6973 696e 7374 616e 6365 2862  and isinstance(b
+00009bb0: 2c20 2869 6e74 2c20 7466 2e54 656e 736f  , (int, tf.Tenso
+00009bc0: 7229 290a 2020 2020 2020 2020 2020 2020  r)).            
+00009bd0: 7769 7468 2074 665f 7574 696c 2e73 616d  with tf_util.sam
+00009be0: 655f 636f 6e74 726f 6c5f 666c 6f77 5f63  e_control_flow_c
+00009bf0: 7478 285b 612c 2062 5d29 3a0a 2020 2020  tx([a, b]):.    
+00009c00: 2020 2020 2020 2020 2020 2020 6966 206b              if k
+00009c10: 696e 6420 3d3d 2022 6164 6422 3a0a 2020  ind == "add":.  
+00009c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009c30: 2020 7573 655f 7265 6c75 203d 205f 6973    use_relu = _is
+00009c40: 5f6e 6567 6174 6976 6528 6129 206f 7220  _negative(a) or 
+00009c50: 5f69 735f 6e65 6761 7469 7665 2862 2920  _is_negative(b) 
+00009c60: 2023 2066 6f72 2064 796e 616d 6963 2074   # for dynamic t
+00009c70: 656e 736f 7273 2c20 6173 7375 6d65 2061  ensors, assume a
+00009c80: 6c6c 2070 6f73 6974 6976 650a 2020 2020  ll positive.    
+00009c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009ca0: 6966 2075 7365 5f72 656c 753a 0a20 2020  if use_relu:.   
+00009cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009cc0: 2020 2020 2072 6574 7572 6e20 7466 2e63       return tf.c
+00009cd0: 6f6e 7665 7274 5f74 6f5f 7465 6e73 6f72  onvert_to_tensor
+00009ce0: 2874 665f 7574 696c 2e73 696d 706c 6966  (tf_util.simplif
+00009cf0: 795f 6e6f 6e5f 6e65 6761 7469 7665 5f73  y_non_negative_s
+00009d00: 6571 5f6c 656e 6774 6828 6120 2b20 6229  eq_length(a + b)
+00009d10: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00009d20: 2020 2020 2020 7265 7475 726e 2061 202b        return a +
+00009d30: 2062 0a20 2020 2020 2020 2020 2020 2020   b.             
+00009d40: 2020 2065 6c69 6620 6b69 6e64 203d 3d20     elif kind == 
+00009d50: 2273 7562 223a 0a20 2020 2020 2020 2020  "sub":.         
+00009d60: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00009d70: 6e20 7466 2e63 6f6e 7665 7274 5f74 6f5f  n tf.convert_to_
+00009d80: 7465 6e73 6f72 2874 665f 7574 696c 2e73  tensor(tf_util.s
+00009d90: 696d 706c 6966 795f 6e6f 6e5f 6e65 6761  implify_non_nega
+00009da0: 7469 7665 5f73 6571 5f6c 656e 6774 6828  tive_seq_length(
+00009db0: 6120 2d20 6229 290a 2020 2020 2020 2020  a - b)).        
+00009dc0: 2020 2020 2020 2020 656c 6966 206b 696e          elif kin
+00009dd0: 6420 3d3d 2022 6d75 6c22 3a0a 2020 2020  d == "mul":.    
+00009de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009df0: 7265 7475 726e 2061 202a 2062 0a20 2020  return a * b.   
+00009e00: 2020 2020 2020 2020 2020 2020 2065 6c69               eli
+00009e10: 6620 6b69 6e64 2069 6e20 2822 666c 6f6f  f kind in ("floo
+00009e20: 7264 6976 222c 2022 7472 7565 6469 7622  rdiv", "truediv"
+00009e30: 293a 2020 2320 7472 7565 6469 7620 6173  ):  # truediv as
+00009e40: 7375 6d65 7320 7468 6572 6520 6973 206e  sumes there is n
+00009e50: 6f20 7265 6d61 696e 6465 720a 2020 2020  o remainder.    
+00009e60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009e70: 7265 7475 726e 2061 202f 2f20 620a 2020  return a // b.  
+00009e80: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00009e90: 6966 206b 696e 6420 3d3d 2022 6365 696c  if kind == "ceil
+00009ea0: 6469 7622 3a0a 2020 2020 2020 2020 2020  div":.          
+00009eb0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00009ec0: 202d 282d 6120 2f2f 2062 290a 2020 2020   -(-a // b).    
+00009ed0: 2020 2020 2020 2020 2020 2020 656c 7365              else
+00009ee0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00009ef0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
+00009f00: 6545 7272 6f72 2822 756e 6b6e 6f77 6e20  eError("unknown 
+00009f10: 6f70 206b 696e 6420 2572 2220 2520 6f70  op kind %r" % op
+00009f20: 2e6b 696e 6429 0a0a 2020 2020 2020 2020  .kind)..        
+00009f30: 6465 6620 5f62 696e 5f6f 7028 612c 2062  def _bin_op(a, b
+00009f40: 293a 0a20 2020 2020 2020 2020 2020 2069  ):.            i
+00009f50: 6620 7465 6d70 6c61 7465 5f6f 6e6c 7920  f template_only 
+00009f60: 6f72 206e 6f74 2062 6163 6b65 6e64 3a0a  or not backend:.
+00009f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00009f80: 6966 2069 7369 6e73 7461 6e63 6528 612c  if isinstance(a,
+00009f90: 205f 742e 5465 6e73 6f72 2920 616e 6420   _t.Tensor) and 
+00009fa0: 6973 696e 7374 616e 6365 2862 2c20 5f74  isinstance(b, _t
+00009fb0: 2e54 656e 736f 7229 3a0a 2020 2020 2020  .Tensor):.      
+00009fc0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00009fd0: 7475 726e 205f 742e 5465 6e73 6f72 2e67  turn _t.Tensor.g
+00009fe0: 6574 5f63 6f6d 6d6f 6e5f 6461 7461 285b  et_common_data([
+00009ff0: 612c 2062 5d2c 2061 6c6c 6f77 5f62 726f  a, b], allow_bro
+0000a000: 6164 6361 7374 5f61 6c6c 5f73 6f75 7263  adcast_all_sourc
+0000a010: 6573 3d54 7275 6529 0a20 2020 2020 2020  es=True).       
+0000a020: 2020 2020 2020 2020 2069 6620 6973 696e           if isin
+0000a030: 7374 616e 6365 2861 2c20 5f74 2e54 656e  stance(a, _t.Ten
+0000a040: 736f 7229 3a0a 2020 2020 2020 2020 2020  sor):.          
+0000a050: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000a060: 2061 0a20 2020 2020 2020 2020 2020 2020   a.             
+0000a070: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+0000a080: 2862 2c20 5f74 2e54 656e 736f 7229 3a0a  (b, _t.Tensor):.
+0000a090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a0a0: 2020 2020 7265 7475 726e 2062 0a20 2020      return b.   
+0000a0b0: 2020 2020 2020 2020 2069 6620 6b69 6e64           if kind
+0000a0c0: 203d 3d20 2261 6464 223a 0a20 2020 2020   == "add":.     
+0000a0d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000a0e0: 6e20 5f72 656c 7528 6120 2b20 6229 0a20  n _relu(a + b). 
+0000a0f0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
+0000a100: 6b69 6e64 203d 3d20 2273 7562 223a 0a20  kind == "sub":. 
+0000a110: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000a120: 6574 7572 6e20 5f72 656c 7528 6120 2d20  eturn _relu(a - 
+0000a130: 6229 0a20 2020 2020 2020 2020 2020 2065  b).            e
+0000a140: 6c69 6620 6b69 6e64 203d 3d20 226d 756c  lif kind == "mul
+0000a150: 223a 0a20 2020 2020 2020 2020 2020 2020  ":.             
+0000a160: 2020 2072 6574 7572 6e20 6120 2a20 620a     return a * b.
+0000a170: 2020 2020 2020 2020 2020 2020 656c 6966              elif
+0000a180: 206b 696e 6420 696e 2028 2266 6c6f 6f72   kind in ("floor
+0000a190: 6469 7622 2c20 2274 7275 6564 6976 2229  div", "truediv")
+0000a1a0: 3a20 2023 2074 7275 6564 6976 2061 7373  :  # truediv ass
+0000a1b0: 756d 6573 2074 6865 7265 2069 7320 6e6f  umes there is no
+0000a1c0: 2072 656d 6169 6e64 6572 0a20 2020 2020   remainder.     
+0000a1d0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000a1e0: 6e20 6120 2f2f 2062 0a20 2020 2020 2020  n a // b.       
+0000a1f0: 2020 2020 2065 6c69 6620 6b69 6e64 203d       elif kind =
+0000a200: 3d20 2263 6569 6c64 6976 223a 0a20 2020  = "ceildiv":.   
+0000a210: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000a220: 6973 696e 7374 616e 6365 2861 2c20 5f74  isinstance(a, _t
+0000a230: 2e54 656e 736f 7229 3a0a 2020 2020 2020  .Tensor):.      
+0000a240: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000a250: 7475 726e 2072 662e 6365 696c 5f64 6976  turn rf.ceil_div
+0000a260: 6964 6528 612c 2062 290a 2020 2020 2020  ide(a, b).      
+0000a270: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000a280: 202d 282d 6120 2f2f 2062 290a 2020 2020   -(-a // b).    
+0000a290: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000a2a0: 2020 2020 2020 2020 2020 2020 2020 7261                ra
+0000a2b0: 6973 6520 5661 6c75 6545 7272 6f72 2822  ise ValueError("
+0000a2c0: 756e 6b6e 6f77 6e20 6f70 206b 696e 6420  unknown op kind 
+0000a2d0: 2572 2220 2520 6f70 2e6b 696e 6429 0a0a  %r" % op.kind)..
+0000a2e0: 2020 2020 2020 2020 6465 6620 5f72 656c          def _rel
+0000a2f0: 7528 6129 3a0a 2020 2020 2020 2020 2020  u(a):.          
+0000a300: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
+0000a310: 612c 205f 742e 5465 6e73 6f72 293a 0a20  a, _t.Tensor):. 
+0000a320: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+0000a330: 6574 7572 6e20 7266 2e72 656c 7528 6129  eturn rf.relu(a)
+0000a340: 0a20 2020 2020 2020 2020 2020 2065 6c69  .            eli
+0000a350: 6620 6973 696e 7374 616e 6365 2861 2c20  f isinstance(a, 
+0000a360: 696e 7429 3a0a 2020 2020 2020 2020 2020  int):.          
+0000a370: 2020 2020 2020 7265 7475 726e 206d 6178        return max
+0000a380: 2861 2c20 3029 0a20 2020 2020 2020 2020  (a, 0).         
+0000a390: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+0000a3a0: 2020 2020 2020 2020 2072 6169 7365 2054           raise T
+0000a3b0: 7970 6545 7272 6f72 2866 2263 6f6d 706c  ypeError(f"compl
+0000a3c0: 6574 655f 6479 6e5f 7369 7a65 3a20 5f72  ete_dyn_size: _r
+0000a3d0: 656c 753a 2075 6e65 7870 6563 7465 6420  elu: unexpected 
+0000a3e0: 7479 7065 207b 7479 7065 2861 297d 2229  type {type(a)}")
+0000a3f0: 0a0a 2020 2020 2020 2020 795f 6e61 6d65  ..        y_name
+0000a400: 203d 2073 656c 662e 6465 7363 7269 7074   = self.descript
+0000a410: 696f 6e20 2b20 223a 7365 712d 6c65 6e67  ion + ":seq-leng
+0000a420: 7468 220a 2020 2020 2020 2020 793a 204f  th".        y: O
+0000a430: 7074 696f 6e61 6c5b 5f74 2e54 656e 736f  ptional[_t.Tenso
+0000a440: 725d 203d 204e 6f6e 6520 2023 2072 6573  r] = None  # res
+0000a450: 756c 7469 6e67 2064 796e 2073 697a 650a  ulting dyn size.
+0000a460: 2020 2020 2020 2020 696e 7075 7473 203d          inputs =
+0000a470: 206c 6973 7428 6f70 2e69 6e70 7574 7329   list(op.inputs)
+0000a480: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+0000a490: 696e 7075 7473 0a20 2020 2020 2020 2077  inputs.        w
+0000a4a0: 6869 6c65 2069 6e70 7574 733a 0a20 2020  hile inputs:.   
+0000a4b0: 2020 2020 2020 2020 2078 203d 2069 6e70           x = inp
+0000a4c0: 7574 732e 706f 7028 3029 0a20 2020 2020  uts.pop(0).     
+0000a4d0: 2020 2020 2020 2069 6620 6e6f 7420 782e         if not x.
+0000a4e0: 6973 5f64 796e 616d 6963 2829 3a20 2023  is_dynamic():  #
+0000a4f0: 2073 7461 7469 630a 2020 2020 2020 2020   static.        
+0000a500: 2020 2020 2020 2020 6173 7365 7274 2078          assert x
+0000a510: 2e64 696d 656e 7369 6f6e 2069 7320 6e6f  .dimension is no
+0000a520: 7420 4e6f 6e65 0a20 2020 2020 2020 2020  t None.         
+0000a530: 2020 2020 2020 2069 6620 7920 6973 204e         if y is N
+0000a540: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+0000a550: 2020 2020 2020 2020 2069 6620 6e6f 7420           if not 
+0000a560: 7465 6d70 6c61 7465 5f6f 6e6c 7920 616e  template_only an
+0000a570: 6420 6261 636b 656e 6420 616e 6420 6e6f  d backend and no
+0000a580: 7420 7466 3a0a 2020 2020 2020 2020 2020  t tf:.          
+0000a590: 2020 2020 2020 2020 2020 2020 2020 7920                y 
+0000a5a0: 3d20 6261 636b 656e 642e 636f 6e76 6572  = backend.conver
+0000a5b0: 745f 746f 5f74 656e 736f 7228 782e 6469  t_to_tensor(x.di
+0000a5c0: 6d65 6e73 696f 6e2c 2064 696d 733d 5b5d  mension, dims=[]
+0000a5d0: 2c20 6474 7970 653d 7369 7a65 5f64 7479  , dtype=size_dty
+0000a5e0: 7065 2c20 6e61 6d65 3d79 5f6e 616d 6529  pe, name=y_name)
+0000a5f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a600: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000a610: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a620: 2020 2079 203d 205f 742e 5465 6e73 6f72     y = _t.Tensor
+0000a630: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+0000a640: 2020 2020 2020 2020 2020 2020 2020 6e61                na
+0000a650: 6d65 3d79 5f6e 616d 652c 0a20 2020 2020  me=y_name,.     
+0000a660: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a670: 2020 2020 2020 2064 696d 5f74 6167 733d         dim_tags=
+0000a680: 5b5d 2c0a 2020 2020 2020 2020 2020 2020  [],.            
+0000a690: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6a0: 6474 7970 653d 7369 7a65 5f64 7479 7065  dtype=size_dtype
+0000a6b0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+0000a6c0: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+0000a6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a6e0: 2020 2020 6966 206e 6f74 2074 656d 706c      if not templ
+0000a6f0: 6174 655f 6f6e 6c79 2061 6e64 2074 663a  ate_only and tf:
+0000a700: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a710: 2020 2020 2020 2020 2020 2020 2077 6974               wit
+0000a720: 6820 7466 2e63 6f6e 7472 6f6c 5f64 6570  h tf.control_dep
+0000a730: 656e 6465 6e63 6965 7328 4e6f 6e65 293a  endencies(None):
+0000a740: 2020 2320 7468 6973 2077 696c 6c20 7265    # this will re
+0000a750: 7365 7420 7468 6520 636f 6e74 6578 740a  set the context.
+0000a760: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a770: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a780: 792e 7261 775f 7465 6e73 6f72 203d 2074  y.raw_tensor = t
+0000a790: 662e 636f 6e73 7461 6e74 2878 2e64 696d  f.constant(x.dim
+0000a7a0: 656e 7369 6f6e 290a 2020 2020 2020 2020  ension).        
+0000a7b0: 2020 2020 2020 2020 2020 2020 636f 6e74              cont
+0000a7c0: 696e 7565 0a20 2020 2020 2020 2020 2020  inue.           
+0000a7d0: 2020 2020 2069 6620 7466 3a0a 2020 2020       if tf:.    
+0000a7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a7f0: 792e 706c 6163 6568 6f6c 6465 7220 3d20  y.placeholder = 
+0000a800: 5f62 696e 5f6f 705f 7466 2879 2e70 6c61  _bin_op_tf(y.pla
+0000a810: 6365 686f 6c64 6572 2c20 782e 6469 6d65  ceholder, x.dime
+0000a820: 6e73 696f 6e29 0a20 2020 2020 2020 2020  nsion).         
+0000a830: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+0000a840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000a850: 2079 203d 205f 6269 6e5f 6f70 2879 2c20   y = _bin_op(y, 
+0000a860: 782e 6469 6d65 6e73 696f 6e29 0a20 2020  x.dimension).   
+0000a870: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+0000a880: 7469 6e75 650a 2020 2020 2020 2020 2020  tinue.          
+0000a890: 2020 6966 2073 656c 662e 6261 7463 683a    if self.batch:
+0000a8a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000a8b0: 2078 203d 2078 2e67 6574 5f66 6f72 5f62   x = x.get_for_b
+0000a8c0: 6174 6368 5f63 7478 2873 656c 662e 6261  atch_ctx(self.ba
+0000a8d0: 7463 682c 2073 656c 662e 636f 6e74 726f  tch, self.contro
+0000a8e0: 6c5f 666c 6f77 5f63 7478 290a 2020 2020  l_flow_ctx).    
+0000a8f0: 2020 2020 2020 2020 782e 636f 6d70 6c65          x.comple
+0000a900: 7465 5f64 796e 5f73 697a 6528 7465 6d70  te_dyn_size(temp
+0000a910: 6c61 7465 5f6f 6e6c 793d 7465 6d70 6c61  late_only=templa
+0000a920: 7465 5f6f 6e6c 7929 0a20 2020 2020 2020  te_only).       
+0000a930: 2020 2020 2069 6620 6e6f 7420 782e 6479       if not x.dy
+0000a940: 6e5f 7369 7a65 5f65 7874 3a0a 2020 2020  n_size_ext:.    
+0000a950: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000a960: 726e 0a20 2020 2020 2020 2020 2020 2078  rn.            x
+0000a970: 203d 2078 2e64 796e 5f73 697a 655f 6578   = x.dyn_size_ex
+0000a980: 740a 2020 2020 2020 2020 2020 2020 6966  t.            if
+0000a990: 2079 2069 7320 4e6f 6e65 3a0a 2020 2020   y is None:.    
+0000a9a0: 2020 2020 2020 2020 2020 2020 7920 3d20              y = 
+0000a9b0: 782e 636f 7079 286e 616d 653d 795f 6e61  x.copy(name=y_na
+0000a9c0: 6d65 290a 2020 2020 2020 2020 2020 2020  me).            
+0000a9d0: 2020 2020 636f 6e74 696e 7565 0a20 2020      continue.   
+0000a9e0: 2020 2020 2020 2020 2069 6620 782e 6469           if x.di
+0000a9f0: 6d5f 7461 6773 2021 3d20 792e 6469 6d5f  m_tags != y.dim_
+0000aa00: 7461 6773 3a0a 2020 2020 2020 2020 2020  tags:.          
+0000aa10: 2020 2020 2020 636f 6d6d 6f6e 203d 205f        common = _
+0000aa20: 742e 5465 6e73 6f72 2e67 6574 5f63 6f6d  t.Tensor.get_com
+0000aa30: 6d6f 6e5f 6461 7461 285b 782c 2079 5d2c  mon_data([x, y],
+0000aa40: 2061 6c6c 6f77 5f62 726f 6164 6361 7374   allow_broadcast
+0000aa50: 5f61 6c6c 5f73 6f75 7263 6573 3d54 7275  _all_sources=Tru
+0000aa60: 6529 0a20 2020 2020 2020 2020 2020 2020  e).             
+0000aa70: 2020 2078 5f20 3d20 782e 636f 7079 5f63     x_ = x.copy_c
+0000aa80: 6f6d 7061 7469 626c 655f 746f 2863 6f6d  ompatible_to(com
+0000aa90: 6d6f 6e29 2069 6620 782e 6469 6d5f 7461  mon) if x.dim_ta
+0000aaa0: 6773 2065 6c73 6520 780a 2020 2020 2020  gs else x.      
+0000aab0: 2020 2020 2020 2020 2020 795f 203d 2079            y_ = y
+0000aac0: 2e63 6f70 795f 636f 6d70 6174 6962 6c65  .copy_compatible
+0000aad0: 5f74 6f28 636f 6d6d 6f6e 2920 6966 2079  _to(common) if y
+0000aae0: 2e64 696d 5f74 6167 7320 656c 7365 2079  .dim_tags else y
+0000aaf0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ab00: 2079 203d 2063 6f6d 6d6f 6e0a 2020 2020   y = common.    
+0000ab10: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000ab20: 2020 2020 2020 2020 2020 2020 2020 785f                x_
+0000ab30: 2c20 795f 203d 2078 2c20 790a 2020 2020  , y_ = x, y.    
+0000ab40: 2020 2020 2020 2020 6966 2074 663a 0a20          if tf:. 
+0000ab50: 2020 2020 2020 2020 2020 2020 2020 2079                 y
+0000ab60: 2e70 6c61 6365 686f 6c64 6572 203d 205f  .placeholder = _
+0000ab70: 6269 6e5f 6f70 5f74 6628 795f 2e70 6c61  bin_op_tf(y_.pla
+0000ab80: 6365 686f 6c64 6572 2c20 785f 2e70 6c61  ceholder, x_.pla
+0000ab90: 6365 686f 6c64 6572 290a 2020 2020 2020  ceholder).      
+0000aba0: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+0000abb0: 2020 2020 2020 2020 2020 2020 7920 3d20              y = 
+0000abc0: 5f62 696e 5f6f 7028 795f 2c20 785f 290a  _bin_op(y_, x_).
+0000abd0: 2020 2020 2020 2020 6173 7365 7274 2079          assert y
+0000abe0: 2c20 6622 6f70 207b 6f70 7d3f 220a 2020  , f"op {op}?".  
+0000abf0: 2020 2020 2020 6966 2073 656c 662e 6479        if self.dy
+0000ac00: 6e5f 7369 7a65 5f65 7874 3a0a 2020 2020  n_size_ext:.    
+0000ac10: 2020 2020 2020 2020 6173 7365 7274 2073          assert s
+0000ac20: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+0000ac30: 2e64 696d 5f74 6167 7320 3d3d 2079 2e64  .dim_tags == y.d
+0000ac40: 696d 5f74 6167 730a 2020 2020 2020 2020  im_tags.        
+0000ac50: 6966 2079 2e62 6174 6368 3a0a 2020 2020  if y.batch:.    
+0000ac60: 2020 2020 2020 2020 6966 2073 656c 662e          if self.
+0000ac70: 6261 7463 683a 0a20 2020 2020 2020 2020  batch:.         
+0000ac80: 2020 2020 2020 2061 7373 6572 7420 7365         assert se
+0000ac90: 6c66 2e62 6174 6368 203d 3d20 792e 6261  lf.batch == y.ba
+0000aca0: 7463 680a 2020 2020 2020 2020 2020 2020  tch.            
+0000acb0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+0000acc0: 2020 2020 2020 7365 6c66 2e62 6174 6368        self.batch
+0000acd0: 203d 2079 2e62 6174 6368 0a20 2020 2020   = y.batch.     
+0000ace0: 2020 2073 656c 662e 6479 6e5f 7369 7a65     self.dyn_size
+0000acf0: 5f65 7874 203d 2079 0a20 2020 2020 2020  _ext = y.       
+0000ad00: 2069 6620 7466 2061 6e64 2079 2e70 6c61   if tf and y.pla
+0000ad10: 6365 686f 6c64 6572 2069 7320 6e6f 7420  ceholder is not 
+0000ad20: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000ad30: 2020 7365 6c66 2e73 6574 5f74 6167 5f6f    self.set_tag_o
+0000ad40: 6e5f 7369 7a65 5f74 656e 736f 7228 792e  n_size_tensor(y.
+0000ad50: 706c 6163 6568 6f6c 6465 7229 0a0a 2020  placeholder)..  
+0000ad60: 2020 6465 6620 6973 5f65 7175 616c 280a    def is_equal(.
+0000ad70: 2020 2020 2020 2020 7365 6c66 2c0a 2020          self,.  
+0000ad80: 2020 2020 2020 6f74 6865 722c 0a20 2020        other,.   
+0000ad90: 2020 2020 2069 676e 6f72 655f 6665 6174       ignore_feat
+0000ada0: 7572 655f 6469 6d3d 4661 6c73 652c 0a20  ure_dim=False,. 
+0000adb0: 2020 2020 2020 2061 6c6c 6f77 5f73 616d         allow_sam
+0000adc0: 655f 6665 6174 7572 655f 6469 6d3d 4661  e_feature_dim=Fa
+0000add0: 6c73 652c 0a20 2020 2020 2020 2061 6c6c  lse,.        all
+0000ade0: 6f77 5f73 616d 655f 7370 6174 6961 6c5f  ow_same_spatial_
+0000adf0: 6469 6d3d 4e6f 6e65 2c0a 2020 2020 2020  dim=None,.      
+0000ae00: 2020 7472 6561 745f 6665 6174 7572 655f    treat_feature_
+0000ae10: 6173 5f73 7061 7469 616c 3d46 616c 7365  as_spatial=False
+0000ae20: 2c0a 2020 2020 2020 2020 6272 6f61 6463  ,.        broadc
+0000ae30: 6173 745f 6d61 7463 6865 733d 4661 6c73  ast_matches=Fals
+0000ae40: 652c 0a20 2020 2020 2020 2075 6e6b 6e6f  e,.        unkno
+0000ae50: 776e 5f73 7061 7469 616c 5f6d 6174 6368  wn_spatial_match
+0000ae60: 6573 3d46 616c 7365 2c0a 2020 2020 2020  es=False,.      
+0000ae70: 2020 756e 6465 6669 6e65 645f 6d61 7463    undefined_matc
+0000ae80: 6865 733d 4661 6c73 652c 0a20 2020 2020  hes=False,.     
+0000ae90: 2020 2064 6572 6976 6564 5f6d 6174 6368     derived_match
+0000aea0: 6573 3d46 616c 7365 2c0a 2020 2020 293a  es=False,.    ):
+0000aeb0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+0000aec0: 2020 2020 2043 6f6d 7061 7265 7320 7365       Compares se
+0000aed0: 6c66 2074 6f20 6f74 6865 7220 666f 7220  lf to other for 
+0000aee0: 6571 7561 6c69 7479 2e0a 0a20 2020 2020  equality...     
+0000aef0: 2020 204e 6f74 6520 7468 6174 2074 6865     Note that the
+0000af00: 2064 6566 6175 6c74 2062 6568 6176 696f   default behavio
+0000af10: 7220 6973 2076 6572 7920 7265 7374 7269  r is very restri
+0000af20: 6374 6976 652e 0a20 2020 2020 2020 2055  ctive..        U
+0000af30: 7365 2066 756e 6374 696f 6e73 2073 7563  se functions suc
+0000af40: 6820 6173 203a 6675 6e63 3a60 6765 745f  h as :func:`get_
+0000af50: 616c 6c5f 6469 6d65 6e73 696f 6e5f 7461  all_dimension_ta
+0000af60: 6773 6020 6f72 203a 6675 6e63 3a60 6765  gs` or :func:`ge
+0000af70: 745f 6578 6973 7469 6e67 5f74 6167 5f66  t_existing_tag_f
+0000af80: 726f 6d5f 636f 6c6c 6563 7469 6f6e 600a  rom_collection`.
+0000af90: 2020 2020 2020 2020 746f 2065 7870 6c69          to expli
+0000afa0: 6369 746c 7920 7370 6563 6966 7920 7468  citly specify th
+0000afb0: 6520 6265 6861 7669 6f72 2066 6f72 2074  e behavior for t
+0000afc0: 6865 2063 6f6d 7061 7269 736f 6e2e 0a0a  he comparison...
+0000afd0: 2020 2020 2020 2020 416c 736f 206e 6f74          Also not
+0000afe0: 6520 7468 6174 2074 6865 2064 6566 696e  e that the defin
+0000aff0: 6974 696f 6e20 6973 2073 6c69 6768 746c  ition is slightl
+0000b000: 7920 6164 2d68 6f63 2066 6f72 2073 6f6d  y ad-hoc for som
+0000b010: 6520 6361 7365 732c 0a20 2020 2020 2020  e cases,.       
+0000b020: 2061 6e64 206d 6967 6874 2070 6f74 656e   and might poten
+0000b030: 7469 616c 6c79 2063 6861 6e67 6520 696e  tially change in
+0000b040: 2074 6865 2066 7574 7572 652e 0a20 2020   the future..   
+0000b050: 2020 2020 2020 2068 7474 7073 3a2f 2f67         https://g
+0000b060: 6974 6875 622e 636f 6d2f 7277 7468 2d69  ithub.com/rwth-i
+0000b070: 362f 7265 7475 726e 6e2f 6973 7375 6573  6/returnn/issues
+0000b080: 2f36 3334 0a0a 2020 2020 2020 2020 3a70  /634..        :p
+0000b090: 6172 616d 2044 696d 206f 7468 6572 3a0a  aram Dim other:.
+0000b0a0: 2020 2020 2020 2020 3a70 6172 616d 2062          :param b
+0000b0b0: 6f6f 6c20 6967 6e6f 7265 5f66 6561 7475  ool ignore_featu
+0000b0c0: 7265 5f64 696d 3a0a 2020 2020 2020 2020  re_dim:.        
+0000b0d0: 3a70 6172 616d 2062 6f6f 6c20 616c 6c6f  :param bool allo
+0000b0e0: 775f 7361 6d65 5f66 6561 7475 7265 5f64  w_same_feature_d
+0000b0f0: 696d 3a0a 2020 2020 2020 2020 3a70 6172  im:.        :par
+0000b100: 616d 2062 6f6f 6c7c 4e6f 6e65 2061 6c6c  am bool|None all
+0000b110: 6f77 5f73 616d 655f 7370 6174 6961 6c5f  ow_same_spatial_
+0000b120: 6469 6d3a 0a20 2020 2020 2020 203a 7061  dim:.        :pa
+0000b130: 7261 6d20 626f 6f6c 2074 7265 6174 5f66  ram bool treat_f
+0000b140: 6561 7475 7265 5f61 735f 7370 6174 6961  eature_as_spatia
+0000b150: 6c3a 0a20 2020 2020 2020 203a 7061 7261  l:.        :para
+0000b160: 6d20 626f 6f6c 2062 726f 6164 6361 7374  m bool broadcast
+0000b170: 5f6d 6174 6368 6573 3a0a 2020 2020 2020  _matches:.      
+0000b180: 2020 3a70 6172 616d 2062 6f6f 6c20 756e    :param bool un
+0000b190: 6b6e 6f77 6e5f 7370 6174 6961 6c5f 6d61  known_spatial_ma
+0000b1a0: 7463 6865 733a 0a20 2020 2020 2020 203a  tches:.        :
+0000b1b0: 7061 7261 6d20 626f 6f6c 2075 6e64 6566  param bool undef
+0000b1c0: 696e 6564 5f6d 6174 6368 6573 3a0a 2020  ined_matches:.  
+0000b1d0: 2020 2020 2020 3a70 6172 616d 2062 6f6f        :param boo
+0000b1e0: 6c20 6465 7269 7665 645f 6d61 7463 6865  l derived_matche
+0000b1f0: 733a 0a20 2020 2020 2020 203a 7274 7970  s:.        :rtyp
+0000b200: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+0000b210: 2222 220a 2020 2020 2020 2020 6672 6f6d  """.        from
+0000b220: 2072 6574 7572 6e6e 2e75 7469 6c20 696d   returnn.util im
+0000b230: 706f 7274 2042 6568 6176 696f 7256 6572  port BehaviorVer
+0000b240: 7369 6f6e 0a0a 2020 2020 2020 2020 6966  sion..        if
+0000b250: 2073 656c 6620 6973 206f 7468 6572 3a20   self is other: 
+0000b260: 2023 2066 6972 7374 2073 6f6d 6520 6661   # first some fa
+0000b270: 7374 2070 6174 6820 6368 6563 6b0a 2020  st path check.  
+0000b280: 2020 2020 2020 2020 2020 7265 7475 726e            return
+0000b290: 2054 7275 650a 2020 2020 2020 2020 6966   True.        if
+0000b2a0: 2073 656c 662e 7370 6563 6961 6c20 6f72   self.special or
+0000b2b0: 206f 7468 6572 2e73 7065 6369 616c 3a0a   other.special:.
+0000b2c0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000b2d0: 726e 2046 616c 7365 2020 2320 6f6e 6c79  rn False  # only
+0000b2e0: 2074 7275 6520 6966 2073 616d 6520 696e   true if same in
+0000b2f0: 7374 616e 6365 2c20 6368 6563 6b20 6162  stance, check ab
+0000b300: 6f76 650a 2020 2020 2020 2020 6966 2061  ove.        if a
+0000b310: 6c6c 6f77 5f73 616d 655f 7370 6174 6961  llow_same_spatia
+0000b320: 6c5f 6469 6d20 6973 204e 6f6e 653a 0a20  l_dim is None:. 
+0000b330: 2020 2020 2020 2020 2020 2061 6c6c 6f77             allow
+0000b340: 5f73 616d 655f 7370 6174 6961 6c5f 6469  _same_spatial_di
+0000b350: 6d20 3d20 616c 6c6f 775f 7361 6d65 5f66  m = allow_same_f
+0000b360: 6561 7475 7265 5f64 696d 0a20 2020 2020  eature_dim.     
+0000b370: 2020 2073 656c 665f 6261 7365 203d 2073     self_base = s
+0000b380: 656c 662e 6765 745f 7361 6d65 5f64 6572  elf.get_same_der
+0000b390: 6976 6564 5f62 6173 6528 7361 6d65 5f64  ived_base(same_d
+0000b3a0: 696d 3d54 7275 6529 2069 6620 6465 7269  im=True) if deri
+0000b3b0: 7665 645f 6d61 7463 6865 7320 656c 7365  ved_matches else
+0000b3c0: 2073 656c 662e 6765 745f 7361 6d65 5f62   self.get_same_b
+0000b3d0: 6173 6528 290a 2020 2020 2020 2020 6f74  ase().        ot
+0000b3e0: 6865 725f 6261 7365 203d 206f 7468 6572  her_base = other
+0000b3f0: 2e67 6574 5f73 616d 655f 6465 7269 7665  .get_same_derive
+0000b400: 645f 6261 7365 2873 616d 655f 6469 6d3d  d_base(same_dim=
+0000b410: 5472 7565 2920 6966 2064 6572 6976 6564  True) if derived
+0000b420: 5f6d 6174 6368 6573 2065 6c73 6520 6f74  _matches else ot
+0000b430: 6865 722e 6765 745f 7361 6d65 5f62 6173  her.get_same_bas
+0000b440: 6528 290a 2020 2020 2020 2020 6966 2073  e().        if s
+0000b450: 656c 665f 6261 7365 2069 7320 6f74 6865  elf_base is othe
+0000b460: 725f 6261 7365 3a0a 2020 2020 2020 2020  r_base:.        
+0000b470: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0000b480: 2020 2020 2020 2020 6966 2073 656c 665f          if self_
+0000b490: 6261 7365 2e64 6572 6976 6564 5f66 726f  base.derived_fro
+0000b4a0: 6d5f 6f70 2061 6e64 206f 7468 6572 5f62  m_op and other_b
+0000b4b0: 6173 652e 6465 7269 7665 645f 6672 6f6d  ase.derived_from
+0000b4c0: 5f6f 703a 0a20 2020 2020 2020 2020 2020  _op:.           
+0000b4d0: 2069 6620 7365 6c66 5f62 6173 652e 6465   if self_base.de
+0000b4e0: 7269 7665 645f 6672 6f6d 5f6f 7020 3d3d  rived_from_op ==
+0000b4f0: 206f 7468 6572 5f62 6173 652e 6465 7269   other_base.deri
+0000b500: 7665 645f 6672 6f6d 5f6f 703a 0a20 2020  ved_from_op:.   
+0000b510: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+0000b520: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+0000b530: 2073 656c 665f 6b69 6e64 203d 2073 656c   self_kind = sel
+0000b540: 662e 6b69 6e64 0a20 2020 2020 2020 206f  f.kind.        o
+0000b550: 7468 6572 5f6b 696e 6420 3d20 6f74 6865  ther_kind = othe
+0000b560: 722e 6b69 6e64 0a20 2020 2020 2020 2069  r.kind.        i
+0000b570: 6620 7365 6c66 5f6b 696e 6420 3d3d 206f  f self_kind == o
+0000b580: 7468 6572 5f6b 696e 6420 3d3d 2044 696d  ther_kind == Dim
+0000b590: 5479 7065 732e 4665 6174 7572 6520 616e  Types.Feature an
+0000b5a0: 6420 6967 6e6f 7265 5f66 6561 7475 7265  d ignore_feature
+0000b5b0: 5f64 696d 3a0a 2020 2020 2020 2020 2020  _dim:.          
+0000b5c0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
+0000b5d0: 2020 2020 2020 6966 2074 7265 6174 5f66        if treat_f
+0000b5e0: 6561 7475 7265 5f61 735f 7370 6174 6961  eature_as_spatia
+0000b5f0: 6c3a 0a20 2020 2020 2020 2020 2020 2023  l:.            #
+0000b600: 204e 6f74 653a 204e 6f20 6b69 6e64 2061   Note: No kind a
+0000b610: 7420 616c 6c3a 2052 6569 6e74 6572 7072  t all: Reinterpr
+0000b620: 6574 2074 7265 6174 5f66 6561 7475 7265  et treat_feature
+0000b630: 5f61 735f 7370 6174 6961 6c20 6120 6269  _as_spatial a bi
+0000b640: 743a 0a20 2020 2020 2020 2020 2020 2023  t:.            #
+0000b650: 2041 7373 756d 6520 7468 6174 2077 6520   Assume that we 
+0000b660: 7761 6e74 2074 6865 6d20 616c 6c20 746f  want them all to
+0000b670: 2062 6520 6861 6e64 6c65 6420 7468 6520   be handled the 
+0000b680: 7361 6d65 2c20 6e6f 206d 6174 7465 7220  same, no matter 
+0000b690: 7468 6520 6b69 6e64 2e0a 2020 2020 2020  the kind..      
+0000b6a0: 2020 2020 2020 2320 2845 7863 6570 7420        # (Except 
+0000b6b0: 6f66 2062 6174 6368 2064 696d 206b 696e  of batch dim kin
+0000b6c0: 642c 2077 6869 6368 2069 7320 7374 696c  d, which is stil
+0000b6d0: 6c20 6578 636c 7564 6564 2068 6572 652e  l excluded here.
+0000b6e0: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000b6f0: 2073 656c 665f 6b69 6e64 203d 3d20 4469   self_kind == Di
+0000b700: 6d54 7970 6573 2e46 6561 7475 7265 206f  mTypes.Feature o
+0000b710: 7220 6e6f 7420 7365 6c66 5f6b 696e 643a  r not self_kind:
+0000b720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b730: 2073 656c 665f 6b69 6e64 203d 2044 696d   self_kind = Dim
+0000b740: 5479 7065 732e 5370 6174 6961 6c0a 2020  Types.Spatial.  
+0000b750: 2020 2020 2020 2020 2020 6966 206f 7468            if oth
+0000b760: 6572 5f6b 696e 6420 3d3d 2044 696d 5479  er_kind == DimTy
+0000b770: 7065 732e 4665 6174 7572 6520 6f72 206e  pes.Feature or n
+0000b780: 6f74 206f 7468 6572 5f6b 696e 643a 0a20  ot other_kind:. 
+0000b790: 2020 2020 2020 2020 2020 2020 2020 206f                 o
+0000b7a0: 7468 6572 5f6b 696e 6420 3d20 4469 6d54  ther_kind = DimT
+0000b7b0: 7970 6573 2e53 7061 7469 616c 0a20 2020  ypes.Spatial.   
+0000b7c0: 2020 2020 2069 6620 7365 6c66 2e64 696d       if self.dim
+0000b7d0: 656e 7369 6f6e 2021 3d20 6f74 6865 722e  ension != other.
+0000b7e0: 6469 6d65 6e73 696f 6e3a 0a20 2020 2020  dimension:.     
+0000b7f0: 2020 2020 2020 2069 6620 6272 6f61 6463         if broadc
+0000b800: 6173 745f 6d61 7463 6865 7320 616e 6420  ast_matches and 
+0000b810: 2873 656c 662e 6469 6d65 6e73 696f 6e20  (self.dimension 
+0000b820: 3d3d 2031 206f 7220 6f74 6865 722e 6469  == 1 or other.di
+0000b830: 6d65 6e73 696f 6e20 3d3d 2031 293a 0a20  mension == 1):. 
+0000b840: 2020 2020 2020 2020 2020 2020 2020 2070                 p
+0000b850: 6173 7320 2023 2070 6173 7320 6f6e 0a20  ass  # pass on. 
+0000b860: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000b870: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000b880: 2072 6574 7572 6e20 4661 6c73 650a 2020   return False.  
+0000b890: 2020 2020 2020 6966 2073 656c 665f 6b69        if self_ki
+0000b8a0: 6e64 2021 3d20 6f74 6865 725f 6b69 6e64  nd != other_kind
+0000b8b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+0000b8c0: 7475 726e 2046 616c 7365 0a20 2020 2020  turn False.     
+0000b8d0: 2020 2069 6620 7365 6c66 5f6b 696e 6420     if self_kind 
+0000b8e0: 3d3d 206f 7468 6572 5f6b 696e 6420 3d3d  == other_kind ==
+0000b8f0: 2044 696d 5479 7065 732e 4261 7463 683a   DimTypes.Batch:
+0000b900: 0a20 2020 2020 2020 2020 2020 2023 204e  .            # N
+0000b910: 6f74 653a 2054 6869 7320 6d69 6768 7420  ote: This might 
+0000b920: 6265 2069 6e63 6f72 7265 6374 2069 6e20  be incorrect in 
+0000b930: 736f 6d65 2063 6173 6573 2c0a 2020 2020  some cases,.    
+0000b940: 2020 2020 2020 2020 2320 652e 672e 2066          # e.g. f
+0000b950: 6f72 2062 6561 6d20 7365 6172 6368 2077  or beam search w
+0000b960: 6865 6e20 7765 2068 6176 6520 7468 6520  hen we have the 
+0000b970: 6265 616d 2068 6964 6465 6e20 696e 2074  beam hidden in t
+0000b980: 6865 2062 6174 6368 2064 696d 2c0a 2020  he batch dim,.  
+0000b990: 2020 2020 2020 2020 2020 2320 6f72 2077            # or w
+0000b9a0: 6865 6e20 7765 2075 7365 6420 4d65 7267  hen we used Merg
+0000b9b0: 6544 696d 734c 6179 6572 206f 6e20 7468  eDimsLayer on th
+0000b9c0: 6520 6261 7463 6820 6178 6973 2c20 6f72  e batch axis, or
+0000b9d0: 2073 6f2e 0a20 2020 2020 2020 2020 2020   so..           
+0000b9e0: 2023 2057 6520 6d69 6768 7420 6e65 6564   # We might need
+0000b9f0: 2074 6f20 6578 7465 6e64 2074 6865 206c   to extend the l
+0000ba00: 6f67 6963 2068 6572 6520 6c61 7465 722e  ogic here later.
+0000ba10: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000ba20: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+0000ba30: 2069 6620 4265 6861 7669 6f72 5665 7273   if BehaviorVers
+0000ba40: 696f 6e2e 6765 7428 2920 3e3d 2031 363a  ion.get() >= 16:
+0000ba50: 0a20 2020 2020 2020 2020 2020 2023 2045  .            # E
+0000ba60: 6974 6865 7220 7365 6c66 206f 7220 6f74  ither self or ot
+0000ba70: 6865 7220 6973 2073 6f6d 6520 6469 6d20  her is some dim 
+0000ba80: 7461 6720 6578 706c 6963 6974 6c79 2063  tag explicitly c
+0000ba90: 7265 6174 6564 2062 7920 7468 6520 7573  reated by the us
+0000baa0: 6572 2c0a 2020 2020 2020 2020 2020 2020  er,.            
+0000bab0: 2320 616e 6420 7468 6579 2061 7265 206e  # and they are n
+0000bac0: 6f74 2074 6865 2073 616d 652c 2073 6f20  ot the same, so 
+0000bad0: 7765 206e 6576 6572 2074 7265 6174 2074  we never treat t
+0000bae0: 6865 6d20 6173 2065 7175 616c 2e0a 2020  hem as equal..  
+0000baf0: 2020 2020 2020 2020 2020 6966 206e 6f74            if not
+0000bb00: 2073 656c 662e 6175 746f 5f67 656e 6572   self.auto_gener
+0000bb10: 6174 6564 206f 7220 6e6f 7420 6f74 6865  ated or not othe
+0000bb20: 722e 6175 746f 5f67 656e 6572 6174 6564  r.auto_generated
+0000bb30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000bb40: 2020 6966 2062 726f 6164 6361 7374 5f6d    if broadcast_m
+0000bb50: 6174 6368 6573 2061 6e64 2028 0a20 2020  atches and (.   
+0000bb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000bb70: 2028 7365 6c66 2e64 696d 656e 7369 6f6e   (self.dimension
+0000bb80: 203d 3d20 3120 616e 6420 7365 6c66 2e61   == 1 and self.a
+0000bb90: 7574 6f5f 6765 6e65 7261 7465 6429 206f  uto_generated) o
+0000bba0: 7220 286f 7468 6572 2e64 696d 656e 7369  r (other.dimensi
+0000bbb0: 6f6e 203d 3d20 3120 616e 6420 6f74 6865  on == 1 and othe
+0000bbc0: 722e 6175 746f 5f67 656e 6572 6174 6564  r.auto_generated
+0000bbd0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000bbe0: 2020 293a 0a20 2020 2020 2020 2020 2020    ):.           
+0000bbf0: 2020 2020 2020 2020 2070 6173 7320 2023           pass  #
+0000bc00: 2065 7863 6570 7469 6f6e 2c20 616c 6c6f   exception, allo
+0000bc10: 7720 6272 6f61 6463 6173 7420 6c6f 6769  w broadcast logi
+0000bc20: 630a 2020 2020 2020 2020 2020 2020 2020  c.              
+0000bc30: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+0000bc40: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000bc50: 726e 2046 616c 7365 0a20 2020 2020 2020  rn False.       
+0000bc60: 2069 6620 7365 6c66 5f6b 696e 6420 3d3d   if self_kind ==
+0000bc70: 206f 7468 6572 5f6b 696e 6420 3d3d 2044   other_kind == D
+0000bc80: 696d 5479 7065 732e 4665 6174 7572 653a  imTypes.Feature:
+0000bc90: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000bca0: 616c 6c6f 775f 7361 6d65 5f66 6561 7475  allow_same_featu
+0000bcb0: 7265 5f64 696d 3a0a 2020 2020 2020 2020  re_dim:.        
+0000bcc0: 2020 2020 2020 2020 7265 7475 726e 2054          return T
+0000bcd0: 7275 650a 2020 2020 2020 2020 6966 2073  rue.        if s
+0000bce0: 656c 665f 6b69 6e64 203d 3d20 6f74 6865  elf_kind == othe
+0000bcf0: 725f 6b69 6e64 203d 3d20 4469 6d54 7970  r_kind == DimTyp
+0000bd00: 6573 2e53 7061 7469 616c 3a0a 2020 2020  es.Spatial:.    
+0000bd10: 2020 2020 2020 2020 6966 2061 6c6c 6f77          if allow
+0000bd20: 5f73 616d 655f 7370 6174 6961 6c5f 6469  _same_spatial_di
+0000bd30: 6d3a 0a20 2020 2020 2020 2020 2020 2020  m:.             
+0000bd40: 2020 2069 6620 7365 6c66 2e64 696d 656e     if self.dimen
+0000bd50: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
+0000bd60: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000bd70: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+0000bd80: 650a 2020 2020 2020 2020 2020 2020 2020  e.              
+0000bd90: 2020 6966 2062 726f 6164 6361 7374 5f6d    if broadcast_m
+0000bda0: 6174 6368 6573 2061 6e64 2028 7365 6c66  atches and (self
+0000bdb0: 2e64 696d 656e 7369 6f6e 203d 3d20 3120  .dimension == 1 
+0000bdc0: 6f72 206f 7468 6572 2e64 696d 656e 7369  or other.dimensi
+0000bdd0: 6f6e 203d 3d20 3129 3a0a 2020 2020 2020  on == 1):.      
+0000bde0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000bdf0: 7475 726e 2054 7275 650a 2020 2020 2020  turn True.      
+0000be00: 2020 2020 2020 6966 2075 6e6b 6e6f 776e        if unknown
+0000be10: 5f73 7061 7469 616c 5f6d 6174 6368 6573  _spatial_matches
+0000be20: 2061 6e64 2028 2873 656c 662e 6479 6e5f   and ((self.dyn_
+0000be30: 7369 7a65 2069 7320 4e6f 6e65 2920 6f72  size is None) or
+0000be40: 2028 6f74 6865 722e 6479 6e5f 7369 7a65   (other.dyn_size
+0000be50: 2069 7320 4e6f 6e65 2929 3a0a 2020 2020   is None)):.    
+0000be60: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000be70: 726e 2054 7275 650a 2020 2020 2020 2020  rn True.        
+0000be80: 2020 2020 6966 2075 6e64 6566 696e 6564      if undefined
+0000be90: 5f6d 6174 6368 6573 2061 6e64 2028 7365  _matches and (se
+0000bea0: 6c66 2e75 6e64 6566 696e 6564 206f 7220  lf.undefined or 
+0000beb0: 6f74 6865 722e 756e 6465 6669 6e65 6429  other.undefined)
+0000bec0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000bed0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
+0000bee0: 2020 2020 2020 2320 496e 2070 7269 6e63        # In princ
+0000bef0: 6970 6c65 2c20 7765 2077 6f75 6c64 2077  iple, we would w
+0000bf00: 616e 7420 746f 2063 6865 636b 2066 6f72  ant to check for
+0000bf10: 2069 6465 6e74 6974 7920 2873 656c 6620   identity (self 
+0000bf20: 6973 206f 7468 6572 292e 0a20 2020 2020  is other)..     
+0000bf30: 2020 2023 2057 6520 6375 7272 656e 746c     # We currentl
+0000bf40: 7920 7573 6520 7468 6520 6465 7363 7269  y use the descri
+0000bf50: 7074 696f 6e20 6265 6361 7573 6520 7468  ption because th
+0000bf60: 6520 6964 656e 7469 7479 2077 6f75 6c64  e identity would
+0000bf70: 206e 6f74 2062 6520 7468 6520 7361 6d65   not be the same
+0000bf80: 0a20 2020 2020 2020 2023 2069 6e20 6361  .        # in ca
+0000bf90: 7365 206f 6620 7465 6d70 6c61 7465 2063  se of template c
+0000bfa0: 6f6e 7374 7275 6374 696f 6e20 7768 6572  onstruction wher
+0000bfb0: 6520 6120 6469 6d20 7461 6720 6973 206f  e a dim tag is o
+0000bfc0: 6e63 6520 6372 6561 7465 6420 666f 7220  nce created for 
+0000bfd0: 6120 7465 6d70 6c61 7465 206c 6179 6572  a template layer
+0000bfe0: 2c0a 2020 2020 2020 2020 2320 616e 6420  ,.        # and 
+0000bff0: 7468 656e 206c 6174 6572 2061 6761 696e  then later again
+0000c000: 2066 6f72 2074 6865 2072 6561 6c20 6c61   for the real la
+0000c010: 7965 722e 0a20 2020 2020 2020 2069 6620  yer..        if 
+0000c020: 7365 6c66 2e61 7574 6f5f 6765 6e65 7261  self.auto_genera
+0000c030: 7465 6420 616e 6420 6f74 6865 722e 6175  ted and other.au
+0000c040: 746f 5f67 656e 6572 6174 6564 2061 6e64  to_generated and
+0000c050: 2073 656c 662e 6465 7363 7269 7074 696f   self.descriptio
+0000c060: 6e20 3d3d 206f 7468 6572 2e64 6573 6372  n == other.descr
+0000c070: 6970 7469 6f6e 3a0a 2020 2020 2020 2020  iption:.        
+0000c080: 2020 2020 7265 7475 726e 2054 7275 650a      return True.
+0000c090: 2020 2020 2020 2020 7265 7475 726e 2046          return F
+0000c0a0: 616c 7365 0a0a 2020 2020 6465 6620 5f5f  alse..    def __
+0000c0b0: 6571 5f5f 2873 656c 662c 206f 7468 6572  eq__(self, other
+0000c0c0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000c0d0: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+0000c0e0: 6d20 6f74 6865 723a 0a20 2020 2020 2020  m other:.       
+0000c0f0: 203a 7274 7970 653a 2062 6f6f 6c0a 2020   :rtype: bool.  
+0000c100: 2020 2020 2020 3a72 6574 7572 6e3a 203a        :return: :
+0000c110: 6675 6e63 3a60 6973 5f65 7175 616c 6020  func:`is_equal` 
+0000c120: 7769 7468 2064 6566 6175 6c74 206f 7074  with default opt
+0000c130: 696f 6e73 0a20 2020 2020 2020 2022 2222  ions.        """
+0000c140: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000c150: 6973 696e 7374 616e 6365 286f 7468 6572  isinstance(other
+0000c160: 2c20 5f64 2e44 696d 293a 0a20 2020 2020  , _d.Dim):.     
+0000c170: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+0000c180: 6c73 650a 2020 2020 2020 2020 7265 7475  lse.        retu
+0000c190: 726e 2073 656c 662e 6973 5f65 7175 616c  rn self.is_equal
+0000c1a0: 286f 7468 6572 290a 0a20 2020 2064 6566  (other)..    def
+0000c1b0: 205f 5f6e 655f 5f28 7365 6c66 3a20 4469   __ne__(self: Di
+0000c1c0: 6d2c 206f 7468 6572 3a20 4469 6d29 3a0a  m, other: Dim):.
+0000c1d0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000c1e0: 2020 2020 3a70 6172 616d 2044 696d 206f      :param Dim o
+0000c1f0: 7468 6572 3a0a 2020 2020 2020 2020 3a72  ther:.        :r
+0000c200: 7479 7065 3a20 626f 6f6c 0a20 2020 2020  type: bool.     
+0000c210: 2020 2022 2222 0a20 2020 2020 2020 2072     """.        r
+0000c220: 6574 7572 6e20 6e6f 7420 2873 656c 6620  eturn not (self 
+0000c230: 3d3d 206f 7468 6572 290a 0a20 2020 2064  == other)..    d
+0000c240: 6566 205f 5f68 6173 685f 5f28 7365 6c66  ef __hash__(self
+0000c250: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+0000c260: 2020 2020 2020 203a 7274 7970 653a 2069         :rtype: i
+0000c270: 6e74 0a20 2020 2020 2020 203a 7265 7475  nt.        :retu
+0000c280: 726e 3a20 6861 7368 2c20 6d61 7463 6869  rn: hash, matchi
+0000c290: 6e67 2074 6f20 3a66 756e 633a 605f 5f65  ng to :func:`__e
+0000c2a0: 715f 5f60 0a20 2020 2020 2020 2022 2222  q__`.        """
+0000c2b0: 0a20 2020 2020 2020 2023 2054 6869 7320  .        # This 
+0000c2c0: 6d75 7374 206d 6174 6368 2074 6865 2062  must match the b
+0000c2d0: 6568 6176 696f 7220 696e 205f 5f65 715f  ehavior in __eq_
+0000c2e0: 5f2c 2077 6869 6368 2069 7320 6973 5f65  _, which is is_e
+0000c2f0: 7175 616c 2077 6974 6820 6465 6661 756c  qual with defaul
+0000c300: 7420 6f70 7469 6f6e 732e 0a20 2020 2020  t options..     
+0000c310: 2020 2023 2049 2e65 2e20 6469 6666 6572     # I.e. differ
+0000c320: 656e 7420 6861 7368 2069 6d70 6c69 6573  ent hash implies
+0000c330: 206e 6f74 2065 7175 616c 2028 6275 7420   not equal (but 
+0000c340: 7361 6d65 2068 6173 6820 6e6f 7420 6e65  same hash not ne
+0000c350: 6365 7373 6172 696c 7920 6571 7561 6c29  cessarily equal)
+0000c360: 2e0a 2020 2020 2020 2020 6966 2073 656c  ..        if sel
+0000c370: 662e 7370 6563 6961 6c3a 0a20 2020 2020  f.special:.     
+0000c380: 2020 2020 2020 2072 6574 7572 6e20 6861         return ha
+0000c390: 7368 2869 6428 7365 6c66 2929 0a20 2020  sh(id(self)).   
+0000c3a0: 2020 2020 2069 6620 7365 6c66 2e69 735f       if self.is_
+0000c3b0: 6261 7463 685f 6469 6d28 293a 0a20 2020  batch_dim():.   
+0000c3c0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000c3d0: 6861 7368 2828 2929 0a20 2020 2020 2020  hash(()).       
+0000c3e0: 2077 6974 6820 7574 696c 2e67 7561 7264   with util.guard
+0000c3f0: 5f69 6e66 696e 6974 655f 7265 6375 7273  _infinite_recurs
+0000c400: 696f 6e28 5f64 2e44 696d 2e5f 5f68 6173  ion(_d.Dim.__has
+0000c410: 685f 5f2c 2073 656c 6629 3a0a 2020 2020  h__, self):.    
+0000c420: 2020 2020 2020 2020 6261 7365 203d 2073          base = s
+0000c430: 656c 662e 6765 745f 7361 6d65 5f62 6173  elf.get_same_bas
+0000c440: 6528 290a 2020 2020 2020 2020 2020 2020  e().            
+0000c450: 6966 2062 6173 6520 6973 206e 6f74 2073  if base is not s
+0000c460: 656c 663a 0a20 2020 2020 2020 2020 2020  elf:.           
+0000c470: 2020 2020 2072 6574 7572 6e20 6861 7368       return hash
+0000c480: 2862 6173 6529 0a20 2020 2020 2020 2020  (base).         
+0000c490: 2020 2069 6620 7365 6c66 2e64 6572 6976     if self.deriv
+0000c4a0: 6564 5f66 726f 6d5f 6f70 3a0a 2020 2020  ed_from_op:.    
+0000c4b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+0000c4c0: 726e 2068 6173 6828 7365 6c66 2e64 6572  rn hash(self.der
+0000c4d0: 6976 6564 5f66 726f 6d5f 6f70 290a 2020  ived_from_op).  
+0000c4e0: 2020 2020 2020 2020 2020 6966 2073 656c            if sel
+0000c4f0: 662e 6175 746f 5f67 656e 6572 6174 6564  f.auto_generated
+0000c500: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000c510: 2020 7265 7475 726e 2068 6173 6828 2862    return hash((b
+0000c520: 6173 652e 6b69 6e64 2c20 6261 7365 2e64  ase.kind, base.d
+0000c530: 696d 656e 7369 6f6e 2c20 6261 7365 2e64  imension, base.d
+0000c540: 6573 6372 6970 7469 6f6e 2929 0a20 2020  escription)).   
+0000c550: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000c560: 6861 7368 2869 6428 6261 7365 2929 0a0a  hash(id(base))..
+0000c570: 2020 2020 6465 6620 5f5f 6c74 5f5f 2873      def __lt__(s
+0000c580: 656c 663a 2044 696d 2c20 6f74 6865 723a  elf: Dim, other:
+0000c590: 2044 696d 293a 0a20 2020 2020 2020 2022   Dim):.        "
+0000c5a0: 2222 0a20 2020 2020 2020 2044 6566 696e  "".        Defin
+0000c5b0: 6520 736f 6d65 206f 7264 6572 2e20 5468  e some order. Th
+0000c5c0: 6973 2069 7320 6a75 7374 2073 7563 6820  is is just such 
+0000c5d0: 7468 6174 2060 736f 7274 6564 6020 776f  that `sorted` wo
+0000c5e0: 726b 732c 206f 7220 736f 6d65 2064 6966  rks, or some dif
+0000c5f0: 6620 7265 706f 7274 696e 672c 206f 7220  f reporting, or 
+0000c600: 736f 2e0a 2020 2020 2020 2020 4974 2069  so..        It i
+0000c610: 7320 6f6e 2073 796d 626f 6c69 6320 6c65  s on symbolic le
+0000c620: 7665 6c2c 2069 2e65 2e20 6974 2064 6f65  vel, i.e. it doe
+0000c630: 7320 6e6f 7420 636f 6e73 6964 6572 2074  s not consider t
+0000c640: 6865 2061 6374 7561 6c20 6469 6d65 6e73  he actual dimens
+0000c650: 696f 6e20 7661 6c75 652e 0a20 2020 2020  ion value..     
+0000c660: 2020 2054 6865 2064 6566 696e 6564 206f     The defined o
+0000c670: 7264 6572 2073 6f6d 6577 6861 7420 6172  rder somewhat ar
+0000c680: 6269 7472 6172 792c 2073 6f20 646f 206e  bitrary, so do n
+0000c690: 6f74 2072 656c 7920 6f6e 2074 6865 2065  ot rely on the e
+0000c6a0: 7861 6374 2062 6568 6176 696f 722c 0a20  xact behavior,. 
+0000c6b0: 2020 2020 2020 2061 7320 7468 6973 206d         as this m
+0000c6c0: 6967 6874 2063 6861 6e67 6520 6174 2073  ight change at s
+0000c6d0: 6f6d 6520 6c61 7465 7220 706f 696e 742e  ome later point.
+0000c6e0: 0a20 2020 2020 2020 2043 7572 7265 6e74  .        Current
+0000c6f0: 6c79 2c20 6974 2064 6570 656e 6473 206f  ly, it depends o
+0000c700: 6e20 7468 6520 6372 6561 7469 6f6e 2069  n the creation i
+0000c710: 6e64 6578 2e0a 0a20 2020 2020 2020 203a  ndex...        :
+0000c720: 7061 7261 6d20 4469 6d20 6f74 6865 723a  param Dim other:
+0000c730: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+0000c740: 2062 6f6f 6c0a 2020 2020 2020 2020 2222   bool.        ""
+0000c750: 220a 2020 2020 2020 2020 6966 206e 6f74  ".        if not
+0000c760: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
+0000c770: 722c 2028 5f64 2e44 696d 2c20 5f6d 2e4d  r, (_d.Dim, _m.M
+0000c780: 6172 6b65 6444 696d 2929 3a0a 2020 2020  arkedDim)):.    
+0000c790: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+0000c7a0: 7065 4572 726f 7228 2263 616e 6e6f 7420  peError("cannot 
+0000c7b0: 636f 6d70 6172 6520 2572 2077 6974 6820  compare %r with 
+0000c7c0: 2572 2220 2520 2873 656c 662c 206f 7468  %r" % (self, oth
+0000c7d0: 6572 2929 0a20 2020 2020 2020 2069 6620  er)).        if 
+0000c7e0: 7365 6c66 203d 3d20 6f74 6865 723a 0a20  self == other:. 
+0000c7f0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000c800: 6e20 4661 6c73 650a 2020 2020 2020 2020  n False.        
+0000c810: 7265 7475 726e 2064 696d 5f63 6d70 5f76  return dim_cmp_v
+0000c820: 616c 7565 2873 656c 6629 203c 2064 696d  alue(self) < dim
+0000c830: 5f63 6d70 5f76 616c 7565 286f 7468 6572  _cmp_value(other
+0000c840: 290a 0a20 2020 2064 6566 205f 5f67 745f  )..    def __gt_
+0000c850: 5f28 7365 6c66 2c20 6f74 6865 7229 3a0a  _(self, other):.
+0000c860: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+0000c870: 2020 2020 5365 6520 3a66 756e 633a 605f      See :func:`_
+0000c880: 5f6c 745f 5f60 2e0a 0a20 2020 2020 2020  _lt__`...       
+0000c890: 203a 7061 7261 6d20 4469 6d20 6f74 6865   :param Dim othe
+0000c8a0: 723a 0a20 2020 2020 2020 203a 7274 7970  r:.        :rtyp
+0000c8b0: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+0000c8c0: 2222 220a 2020 2020 2020 2020 7265 7475  """.        retu
+0000c8d0: 726e 206f 7468 6572 203c 2073 656c 660a  rn other < self.
+0000c8e0: 0a20 2020 2064 6566 205f 5f67 655f 5f28  .    def __ge__(
+0000c8f0: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
+0000c900: 2020 2020 2020 7265 7475 726e 206e 6f74        return not
+0000c910: 2073 656c 6620 3c20 6f74 6865 720a 0a20   self < other.. 
+0000c920: 2020 2064 6566 205f 5f6c 655f 5f28 7365     def __le__(se
+0000c930: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
+0000c940: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
+0000c950: 656c 6620 3e20 6f74 6865 720a 0a20 2020  elf > other..   
+0000c960: 2064 6566 2067 6574 5f73 616d 655f 6261   def get_same_ba
+0000c970: 7365 2873 656c 663a 205f 642e 4469 6d29  se(self: _d.Dim)
+0000c980: 202d 3e20 5f64 2e44 696d 3a0a 2020 2020   -> _d.Dim:.    
+0000c990: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+0000c9a0: 3a72 6574 7572 6e3a 2073 616d 6520 6261  :return: same ba
+0000c9b0: 7365 0a20 2020 2020 2020 2022 2222 0a20  se.        """. 
+0000c9c0: 2020 2020 2020 2069 6620 6e6f 7420 7365         if not se
+0000c9d0: 6c66 2e5f 6578 7472 613a 0a20 2020 2020  lf._extra:.     
+0000c9e0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+0000c9f0: 6c66 0a20 2020 2020 2020 2062 6173 6520  lf.        base 
+0000ca00: 3d20 7365 6c66 0a20 2020 2020 2020 2077  = self.        w
+0000ca10: 6869 6c65 2062 6173 652e 7361 6d65 5f61  hile base.same_a
+0000ca20: 733a 0a20 2020 2020 2020 2020 2020 2062  s:.            b
+0000ca30: 6173 6520 3d20 6261 7365 2e73 616d 655f  ase = base.same_
+0000ca40: 6173 0a20 2020 2020 2020 2072 6574 7572  as.        retur
+0000ca50: 6e20 6261 7365 0a0a 2020 2020 6465 6620  n base..    def 
+0000ca60: 6765 745f 7361 6d65 5f64 6572 6976 6564  get_same_derived
+0000ca70: 5f62 6173 6528 7365 6c66 3a20 5f64 2e44  _base(self: _d.D
+0000ca80: 696d 2c20 2a2c 2073 616d 655f 6469 6d3a  im, *, same_dim:
+0000ca90: 2062 6f6f 6c20 3d20 4661 6c73 6529 202d   bool = False) -
+0000caa0: 3e20 5f64 2e44 696d 3a0a 2020 2020 2020  > _d.Dim:.      
+0000cab0: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
+0000cac0: 6172 616d 2073 616d 655f 6469 6d3a 2069  aram same_dim: i
+0000cad0: 6620 5472 7565 2c20 7265 7475 726e 2074  f True, return t
+0000cae0: 6865 206c 6173 7420 6261 7365 2077 6869  he last base whi
+0000caf0: 6368 2068 6173 2074 6865 2073 616d 6520  ch has the same 
+0000cb00: 6469 6d65 6e73 696f 6e2e 0a20 2020 2020  dimension..     
+0000cb10: 2020 2020 2020 2054 6865 2064 6572 6976         The deriv
+0000cb20: 6564 2062 6173 6520 6d69 6768 7420 6861  ed base might ha
+0000cb30: 7665 2061 2064 6966 6665 7265 6e74 2064  ve a different d
+0000cb40: 696d 656e 7369 6f6e 2e0a 2020 2020 2020  imension..      
+0000cb50: 2020 2020 2020 496e 2063 6173 6520 6974        In case it
+0000cb60: 2069 7320 6479 6e61 6d69 632c 2074 6865   is dynamic, the
+0000cb70: 2064 696d 656e 7369 6f6e 2069 7320 4e6f   dimension is No
+0000cb80: 6e65 2c20 736f 2069 7420 6973 2061 6c77  ne, so it is alw
+0000cb90: 6179 7320 7468 6520 7361 6d65 2e0a 2020  ays the same..  
+0000cba0: 2020 2020 2020 2020 2020 496e 2063 6173            In cas
+0000cbb0: 6520 6974 2069 7320 7374 6174 6963 2c20  e it is static, 
+0000cbc0: 7468 6572 6520 6d69 6768 7420 6265 2061  there might be a
+0000cbd0: 2064 6966 6665 7265 6e74 2064 696d 656e   different dimen
+0000cbe0: 7369 6f6e 2e0a 2020 2020 2020 2020 3a72  sion..        :r
+0000cbf0: 6574 7572 6e3a 2073 616d 6520 6261 7365  eturn: same base
+0000cc00: 2c20 6275 7420 616c 736f 2063 6f6e 7369  , but also consi
+0000cc10: 6465 7220 6465 7269 7665 645f 6672 6f6d  der derived_from
+0000cc20: 5f2e 2e2e 0a20 2020 2020 2020 2022 2222  _....        """
+0000cc30: 0a20 2020 2020 2020 206c 6173 745f 6261  .        last_ba
+0000cc40: 7365 5f73 656c 665f 6469 6d20 3d20 7365  se_self_dim = se
+0000cc50: 6c66 0a20 2020 2020 2020 2062 6173 6520  lf.        base 
+0000cc60: 3d20 7365 6c66 0a20 2020 2020 2020 2076  = self.        v
+0000cc70: 6973 6974 6564 203d 207b 7d0a 2020 2020  isited = {}.    
+0000cc80: 2020 2020 7768 696c 6520 6261 7365 2e73      while base.s
+0000cc90: 616d 655f 6173 206f 7220 6261 7365 2e64  ame_as or base.d
+0000cca0: 6572 6976 6564 5f66 726f 6d5f 7461 673a  erived_from_tag:
+0000ccb0: 0a20 2020 2020 2020 2020 2020 2061 7373  .            ass
+0000ccc0: 6572 7420 6964 2862 6173 6529 206e 6f74  ert id(base) not
+0000ccd0: 2069 6e20 7669 7369 7465 6420 2023 2073   in visited  # s
+0000cce0: 686f 756c 6420 6e6f 7420 6861 7665 2063  hould not have c
+0000ccf0: 7963 6c65 732e 206e 6f72 6d61 6c6c 7920  ycles. normally 
+0000cd00: 7468 6973 2073 686f 756c 6420 6e65 7665  this should neve
+0000cd10: 7220 6265 2074 7269 6767 6572 6564 0a20  r be triggered. 
+0000cd20: 2020 2020 2020 2020 2020 2076 6973 6974             visit
+0000cd30: 6564 5b69 6428 6261 7365 295d 203d 2062  ed[id(base)] = b
+0000cd40: 6173 650a 2020 2020 2020 2020 2020 2020  ase.            
+0000cd50: 6966 2062 6173 652e 7361 6d65 5f61 733a  if base.same_as:
+0000cd60: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000cd70: 2062 6173 6520 3d20 6261 7365 2e73 616d   base = base.sam
+0000cd80: 655f 6173 0a20 2020 2020 2020 2020 2020  e_as.           
+0000cd90: 2020 2020 2063 6f6e 7469 6e75 650a 2020       continue.  
+0000cda0: 2020 2020 2020 2020 2020 6261 7365 203d            base =
+0000cdb0: 2062 6173 652e 6465 7269 7665 645f 6672   base.derived_fr
+0000cdc0: 6f6d 5f74 6167 0a20 2020 2020 2020 2020  om_tag.         
+0000cdd0: 2020 2061 7373 6572 7420 6261 7365 0a20     assert base. 
+0000cde0: 2020 2020 2020 2020 2020 2069 6620 6261             if ba
+0000cdf0: 7365 2e64 696d 656e 7369 6f6e 203d 3d20  se.dimension == 
+0000ce00: 7365 6c66 2e64 696d 656e 7369 6f6e 3a0a  self.dimension:.
+0000ce10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ce20: 6c61 7374 5f62 6173 655f 7365 6c66 5f64  last_base_self_d
+0000ce30: 696d 203d 2062 6173 650a 2020 2020 2020  im = base.      
+0000ce40: 2020 7265 7475 726e 206c 6173 745f 6261    return last_ba
+0000ce50: 7365 5f73 656c 665f 6469 6d20 6966 2073  se_self_dim if s
+0000ce60: 616d 655f 6469 6d20 656c 7365 2062 6173  ame_dim else bas
+0000ce70: 650a 0a20 2020 2064 6566 2067 6574 5f64  e..    def get_d
+0000ce80: 6572 6976 6564 5f62 6173 6573 5f73 6574  erived_bases_set
+0000ce90: 2873 656c 6629 3a0a 2020 2020 2020 2020  (self):.        
+0000cea0: 2222 220a 2020 2020 2020 2020 3a72 7479  """.        :rty
+0000ceb0: 7065 3a20 7365 745b 4469 6d5d 0a20 2020  pe: set[Dim].   
+0000cec0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000ced0: 2072 6573 203d 2073 6574 2829 0a20 2020   res = set().   
+0000cee0: 2020 2020 2071 7565 7565 203d 205b 7365       queue = [se
+0000cef0: 6c66 5d0a 2020 2020 2020 2020 7669 7369  lf].        visi
+0000cf00: 7465 6420 3d20 7b7d 2020 2320 7479 7065  ted = {}  # type
+0000cf10: 3a20 4469 6374 5b69 6e74 2c5f 642e 4469  : Dict[int,_d.Di
+0000cf20: 6d5d 2020 2320 6279 2069 640a 2020 2020  m]  # by id.    
+0000cf30: 2020 2020 7768 696c 6520 7175 6575 653a      while queue:
+0000cf40: 0a20 2020 2020 2020 2020 2020 2062 6173  .            bas
+0000cf50: 6520 3d20 7175 6575 652e 706f 7028 2d31  e = queue.pop(-1
+0000cf60: 290a 2020 2020 2020 2020 2020 2020 6966  ).            if
+0000cf70: 2062 6173 652e 7361 6d65 5f61 733a 0a20   base.same_as:. 
+0000cf80: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+0000cf90: 6173 6520 3d20 6261 7365 2e73 616d 655f  ase = base.same_
+0000cfa0: 6173 0a20 2020 2020 2020 2020 2020 2069  as.            i
+0000cfb0: 6620 6964 2862 6173 6529 2069 6e20 7669  f id(base) in vi
+0000cfc0: 7369 7465 643a 0a20 2020 2020 2020 2020  sited:.         
+0000cfd0: 2020 2020 2020 2063 6f6e 7469 6e75 650a         continue.
+0000cfe0: 2020 2020 2020 2020 2020 2020 7669 7369              visi
+0000cff0: 7465 645b 6964 2862 6173 6529 5d20 3d20  ted[id(base)] = 
+0000d000: 6261 7365 0a20 2020 2020 2020 2020 2020  base.           
+0000d010: 2072 6573 2e61 6464 2862 6173 6529 0a20   res.add(base). 
+0000d020: 2020 2020 2020 2020 2020 2069 6620 6261             if ba
+0000d030: 7365 2e64 6572 6976 6564 5f66 726f 6d5f  se.derived_from_
+0000d040: 6f70 3a0a 2020 2020 2020 2020 2020 2020  op:.            
+0000d050: 2020 2020 7175 6575 652e 6578 7465 6e64      queue.extend
+0000d060: 2862 6173 652e 6465 7269 7665 645f 6672  (base.derived_fr
+0000d070: 6f6d 5f6f 702e 696e 7075 7473 290a 2020  om_op.inputs).  
+0000d080: 2020 2020 2020 2020 2020 656c 6966 2062            elif b
+0000d090: 6173 652e 6465 7269 7665 645f 6672 6f6d  ase.derived_from
+0000d0a0: 5f74 6167 3a0a 2020 2020 2020 2020 2020  _tag:.          
+0000d0b0: 2020 2020 2020 7175 6575 652e 6170 7065        queue.appe
+0000d0c0: 6e64 2862 6173 652e 6465 7269 7665 645f  nd(base.derived_
+0000d0d0: 6672 6f6d 5f74 6167 290a 2020 2020 2020  from_tag).      
+0000d0e0: 2020 7265 7475 726e 2072 6573 0a0a 2020    return res..  
+0000d0f0: 2020 4070 726f 7065 7274 790a 2020 2020    @property.    
+0000d100: 6465 6620 756e 6465 6669 6e65 6428 7365  def undefined(se
+0000d110: 6c66 3a20 5f64 2e44 696d 2920 2d3e 2062  lf: _d.Dim) -> b
+0000d120: 6f6f 6c3a 0a20 2020 2020 2020 2022 2222  ool:.        """
+0000d130: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+0000d140: 3a20 7768 6574 6865 7220 7468 6520 756e  : whether the un
+0000d150: 6465 6669 6e65 6420 666c 6167 2069 7320  defined flag is 
+0000d160: 7365 742c 2069 6e20 7365 6c66 2c20 6261  set, in self, ba
+0000d170: 7365 732c 206f 7220 616e 7920 6465 7269  ses, or any deri
+0000d180: 7665 6420 6261 7365 732e 2061 6c73 6f20  ved bases. also 
+0000d190: 7365 6520 3a66 756e 633a 6069 735f 6469  see :func:`is_di
+0000d1a0: 6d5f 6b6e 6f77 6e60 0a20 2020 2020 2020  m_known`.       
+0000d1b0: 2022 2222 0a20 2020 2020 2020 2062 6173   """.        bas
+0000d1c0: 6520 3d20 7365 6c66 0a20 2020 2020 2020  e = self.       
+0000d1d0: 2076 6973 6974 6564 203d 207b 7d0a 2020   visited = {}.  
+0000d1e0: 2020 2020 2020 7768 696c 6520 6261 7365        while base
+0000d1f0: 2e73 616d 655f 6173 206f 7220 6261 7365  .same_as or base
+0000d200: 2e64 6572 6976 6564 5f66 726f 6d5f 7461  .derived_from_ta
+0000d210: 673a 0a20 2020 2020 2020 2020 2020 2061  g:.            a
+0000d220: 7373 6572 7420 6964 2862 6173 6529 206e  ssert id(base) n
+0000d230: 6f74 2069 6e20 7669 7369 7465 6420 2023  ot in visited  #
+0000d240: 2073 686f 756c 6420 6e6f 7420 6861 7665   should not have
+0000d250: 2063 7963 6c65 732e 206e 6f72 6d61 6c6c   cycles. normall
+0000d260: 7920 7468 6973 2073 686f 756c 6420 6e65  y this should ne
+0000d270: 7665 7220 6265 2074 7269 6767 6572 6564  ver be triggered
+0000d280: 0a20 2020 2020 2020 2020 2020 2076 6973  .            vis
+0000d290: 6974 6564 5b69 6428 6261 7365 295d 203d  ited[id(base)] =
+0000d2a0: 2062 6173 650a 2020 2020 2020 2020 2020   base.          
+0000d2b0: 2020 2320 6e6f 696e 7370 6563 7469 6f6e    # noinspection
+0000d2c0: 2050 7950 726f 7465 6374 6564 4d65 6d62   PyProtectedMemb
+0000d2d0: 6572 0a20 2020 2020 2020 2020 2020 2069  er.            i
+0000d2e0: 6620 6261 7365 2e5f 6578 7472 6120 616e  f base._extra an
+0000d2f0: 6420 6261 7365 2e5f 6578 7472 612e 756e  d base._extra.un
+0000d300: 6465 6669 6e65 643a 0a20 2020 2020 2020  defined:.       
+0000d310: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+0000d320: 5472 7565 0a20 2020 2020 2020 2020 2020  True.           
+0000d330: 2069 6620 6261 7365 2e73 616d 655f 6173   if base.same_as
+0000d340: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000d350: 2020 6261 7365 203d 2062 6173 652e 7361    base = base.sa
+0000d360: 6d65 5f61 730a 2020 2020 2020 2020 2020  me_as.          
+0000d370: 2020 2020 2020 636f 6e74 696e 7565 0a20        continue. 
+0000d380: 2020 2020 2020 2020 2020 2062 6173 6520             base 
+0000d390: 3d20 6261 7365 2e64 6572 6976 6564 5f66  = base.derived_f
+0000d3a0: 726f 6d5f 7461 670a 2020 2020 2020 2020  rom_tag.        
+0000d3b0: 2020 2020 6173 7365 7274 2062 6173 650a      assert base.
+0000d3c0: 2020 2020 2020 2020 2320 6e6f 696e 7370          # noinsp
+0000d3d0: 6563 7469 6f6e 2050 7950 726f 7465 6374  ection PyProtect
+0000d3e0: 6564 4d65 6d62 6572 0a20 2020 2020 2020  edMember.       
+0000d3f0: 2072 6574 7572 6e20 6261 7365 2e5f 6578   return base._ex
+0000d400: 7472 6120 616e 6420 6261 7365 2e5f 6578  tra and base._ex
+0000d410: 7472 612e 756e 6465 6669 6e65 640a 0a20  tra.undefined.. 
+0000d420: 2020 2064 6566 2064 6563 6c61 7265 5f73     def declare_s
+0000d430: 616d 655f 6173 2873 656c 663a 205f 642e  ame_as(self: _d.
+0000d440: 4469 6d2c 206f 7468 6572 3a20 5f64 2e44  Dim, other: _d.D
+0000d450: 696d 293a 0a20 2020 2020 2020 2022 2222  im):.        """
+0000d460: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+0000d470: 6f74 6865 723a 0a20 2020 2020 2020 2022  other:.        "
+0000d480: 2222 0a20 2020 2020 2020 2061 7373 6572  "".        asser
+0000d490: 7420 7365 6c66 2e63 616e 5f62 655f 7573  t self.can_be_us
+0000d4a0: 6564 5f61 735f 6469 6d28 2920 616e 6420  ed_as_dim() and 
+0000d4b0: 6f74 6865 722e 6361 6e5f 6265 5f75 7365  other.can_be_use
+0000d4c0: 645f 6173 5f64 696d 2829 2020 2320 6465  d_as_dim()  # de
+0000d4d0: 636c 6172 655f 7361 6d65 5f61 7320 646f  clare_same_as do
+0000d4e0: 6573 206e 6f74 206d 616b 6520 7365 6e73  es not make sens
+0000d4f0: 6520 6f74 6865 7277 6973 650a 2020 2020  e otherwise.    
+0000d500: 2020 2020 2320 4e6f 7465 3a20 4368 6563      # Note: Chec
+0000d510: 6b20 6069 7360 2c20 6e6f 7420 603d 3d60  k `is`, not `==`
+0000d520: 2e20 603d 3d60 2063 616e 2062 6520 7472  . `==` can be tr
+0000d530: 7565 2065 7665 6e20 7468 6f75 6768 2073  ue even though s
+0000d540: 616d 655f 6173 2061 7265 206e 6f74 2074  ame_as are not t
+0000d550: 6865 2073 616d 6520 696e 7374 616e 6365  he same instance
+0000d560: 2c0a 2020 2020 2020 2020 2320 652e 672e  ,.        # e.g.
+0000d570: 2076 6961 2061 7574 6f5f 6765 6e65 7261   via auto_genera
+0000d580: 7465 642e 0a20 2020 2020 2020 2069 6620  ted..        if 
+0000d590: 7365 6c66 2069 7320 6f74 6865 723a 0a20  self is other:. 
+0000d5a0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+0000d5b0: 6e0a 2020 2020 2020 2020 7365 6c66 2e5f  n.        self._
+0000d5c0: 6d61 7962 655f 7570 6461 7465 2829 0a20  maybe_update(). 
+0000d5d0: 2020 2020 2020 2073 656c 662e 5f76 616c         self._val
+0000d5e0: 6964 6174 655f 696e 5f63 7572 7265 6e74  idate_in_current
+0000d5f0: 5f67 7261 7068 2829 0a20 2020 2020 2020  _graph().       
+0000d600: 206f 7468 6572 2e5f 7661 6c69 6461 7465   other._validate
+0000d610: 5f69 6e5f 6375 7272 656e 745f 6772 6170  _in_current_grap
+0000d620: 6828 290a 2020 2020 2020 2020 6f74 6865  h().        othe
+0000d630: 725f 7361 6d65 5f62 6173 6520 3d20 6f74  r_same_base = ot
+0000d640: 6865 722e 6765 745f 7361 6d65 5f62 6173  her.get_same_bas
+0000d650: 6528 290a 2020 2020 2020 2020 6966 2073  e().        if s
+0000d660: 656c 6620 6973 206f 7468 6572 5f73 616d  elf is other_sam
+0000d670: 655f 6261 7365 206f 7220 7365 6c66 2e73  e_base or self.s
+0000d680: 616d 655f 6173 2069 7320 6f74 6865 725f  ame_as is other_
+0000d690: 7361 6d65 5f62 6173 653a 0a20 2020 2020  same_base:.     
+0000d6a0: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+0000d6b0: 2020 2020 2020 7365 6c66 5f73 616d 655f        self_same_
+0000d6c0: 6173 203d 2073 656c 662e 6765 745f 7361  as = self.get_sa
+0000d6d0: 6d65 5f62 6173 6528 290a 2020 2020 2020  me_base().      
+0000d6e0: 2020 6966 2073 656c 665f 7361 6d65 5f61    if self_same_a
+0000d6f0: 7320 6973 206f 7468 6572 5f73 616d 655f  s is other_same_
+0000d700: 6261 7365 3a0a 2020 2020 2020 2020 2020  base:.          
+0000d710: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+0000d720: 2069 6620 6f74 6865 725f 7361 6d65 5f62   if other_same_b
+0000d730: 6173 652e 6765 745f 7361 6d65 5f64 6572  ase.get_same_der
+0000d740: 6976 6564 5f62 6173 6528 2920 6973 2073  ived_base() is s
+0000d750: 656c 665f 7361 6d65 5f61 733a 0a20 2020  elf_same_as:.   
+0000d760: 2020 2020 2020 2020 2023 2057 6520 6163           # We ac
+0000d770: 7475 616c 6c79 2077 616e 7420 6974 2074  tually want it t
+0000d780: 6f20 6265 2074 6865 206f 7468 6572 2077  o be the other w
+0000d790: 6179 2061 726f 756e 642e 0a20 2020 2020  ay around..     
+0000d7a0: 2020 2020 2020 2077 6974 6820 7574 696c         with util
+0000d7b0: 2e67 7561 7264 5f69 6e66 696e 6974 655f  .guard_infinite_
+0000d7c0: 7265 6375 7273 696f 6e28 5f64 2e44 696d  recursion(_d.Dim
+0000d7d0: 2e64 6563 6c61 7265 5f73 616d 655f 6173  .declare_same_as
+0000d7e0: 2c20 6f74 6865 722c 2073 656c 6629 3a0a  , other, self):.
+0000d7f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000d800: 7265 7475 726e 206f 7468 6572 2e64 6563  return other.dec
+0000d810: 6c61 7265 5f73 616d 655f 6173 2873 656c  lare_same_as(sel
+0000d820: 6629 0a20 2020 2020 2020 2069 6620 7365  f).        if se
+0000d830: 6c66 2e62 6174 6368 3a0a 2020 2020 2020  lf.batch:.      
+0000d840: 2020 2020 2020 2320 4966 2073 656c 6620        # If self 
+0000d850: 6973 2064 6566 696e 6564 2028 7365 6c66  is defined (self
+0000d860: 2e69 735f 6469 6d5f 6b6e 6f77 6e29 2c20  .is_dim_known), 
+0000d870: 6265 2066 6169 7220 746f 206f 7468 6572  be fair to other
+0000d880: 2c20 616e 6420 6164 6170 7420 6974 2074  , and adapt it t
+0000d890: 6f20 7468 6520 7269 6768 7420 6261 7463  o the right batc
+0000d8a0: 682c 0a20 2020 2020 2020 2020 2020 2023  h,.            #
+0000d8b0: 2073 7563 6820 7468 6174 206f 7468 6572   such that other
+0000d8c0: 2e69 735f 6469 6d5f 6b6e 6f77 6e20 6973  .is_dim_known is
+0000d8d0: 2063 6f72 7265 6374 2c20 6279 2070 6f74   correct, by pot
+0000d8e0: 656e 7469 616c 6c79 2063 6f6d 706c 6574  entially complet
+0000d8f0: 696e 6720 6974 2e0a 2020 2020 2020 2020  ing it..        
+0000d900: 2020 2020 6f74 6865 725f 203d 206f 7468      other_ = oth
+0000d910: 6572 2e67 6574 5f66 6f72 5f62 6174 6368  er.get_for_batch
+0000d920: 5f63 7478 2873 656c 662e 6261 7463 682c  _ctx(self.batch,
+0000d930: 2063 7478 3d73 656c 662e 636f 6e74 726f   ctx=self.contro
+0000d940: 6c5f 666c 6f77 5f63 7478 290a 2020 2020  l_flow_ctx).    
+0000d950: 2020 2020 656c 7365 3a0a 2020 2020 2020      else:.      
+0000d960: 2020 2020 2020 6f74 6865 725f 203d 206f        other_ = o
+0000d970: 7468 6572 0a20 2020 2020 2020 2069 6620  ther.        if 
+0000d980: 280a 2020 2020 2020 2020 2020 2020 2873  (.            (s
+0000d990: 656c 662e 6973 5f64 696d 5f6b 6e6f 776e  elf.is_dim_known
+0000d9a0: 2829 2061 6e64 206e 6f74 206f 7468 6572  () and not other
+0000d9b0: 5f2e 6973 5f64 696d 5f6b 6e6f 776e 2829  _.is_dim_known()
+0000d9c0: 290a 2020 2020 2020 2020 2020 2020 6f72  ).            or
+0000d9d0: 0a20 2020 2020 2020 2020 2020 2023 204c  .            # L
+0000d9e0: 696b 6520 6973 5f64 696d 5f6b 6e6f 776e  ike is_dim_known
+0000d9f0: 2062 7574 2066 6f72 2073 7461 7469 6320   but for static 
+0000da00: 6469 6d73 2c20 7765 206d 6967 6874 206b  dims, we might k
+0000da10: 6e6f 7720 626f 7468 2c0a 2020 2020 2020  now both,.      
+0000da20: 2020 2020 2020 2320 6275 7420 7468 6520        # but the 
+0000da30: 6465 7269 7665 645f 6672 6f6d 5f6f 7020  derived_from_op 
+0000da40: 7374 696c 6c20 776f 756c 6420 7072 6f76  still would prov
+0000da50: 6964 6520 6d6f 7265 2069 6e66 6f72 6d61  ide more informa
+0000da60: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
+0000da70: 2020 280a 2020 2020 2020 2020 2020 2020    (.            
+0000da80: 2020 2020 7365 6c66 5f73 616d 655f 6173      self_same_as
+0000da90: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+0000daa0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dab0: 2061 6e64 206e 6f74 206f 7468 6572 5f73   and not other_s
+0000dac0: 616d 655f 6261 7365 2e64 6572 6976 6564  ame_base.derived
+0000dad0: 5f66 726f 6d5f 6f70 0a20 2020 2020 2020  _from_op.       
+0000dae0: 2020 2020 2020 2020 2061 6e64 206f 7468           and oth
+0000daf0: 6572 206e 6f74 2069 6e20 7365 6c66 2e67  er not in self.g
+0000db00: 6574 5f64 6572 6976 6564 5f62 6173 6573  et_derived_bases
+0000db10: 5f73 6574 2829 0a20 2020 2020 2020 2020  _set().         
+0000db20: 2020 2029 0a20 2020 2020 2020 2020 2020     ).           
+0000db30: 206f 7220 286e 6f74 2073 656c 662e 756e   or (not self.un
+0000db40: 6465 6669 6e65 6420 616e 6420 6f74 6865  defined and othe
+0000db50: 725f 2e75 6e64 6566 696e 6564 290a 2020  r_.undefined).  
+0000db60: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+0000db70: 2020 2020 2077 6974 6820 7574 696c 2e67       with util.g
+0000db80: 7561 7264 5f69 6e66 696e 6974 655f 7265  uard_infinite_re
+0000db90: 6375 7273 696f 6e28 5f64 2e44 696d 2e64  cursion(_d.Dim.d
+0000dba0: 6563 6c61 7265 5f73 616d 655f 6173 2c20  eclare_same_as, 
+0000dbb0: 6f74 6865 722c 2073 656c 6629 3a0a 2020  other, self):.  
+0000dbc0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+0000dbd0: 7475 726e 206f 7468 6572 2e64 6563 6c61  turn other.decla
+0000dbe0: 7265 5f73 616d 655f 6173 2873 656c 6629  re_same_as(self)
+0000dbf0: 0a20 2020 2020 2020 206f 7468 6572 5f64  .        other_d
+0000dc00: 6572 6976 6564 5f62 6173 6573 203d 206f  erived_bases = o
+0000dc10: 7468 6572 2e67 6574 5f64 6572 6976 6564  ther.get_derived
+0000dc20: 5f62 6173 6573 5f73 6574 2829 0a20 2020  _bases_set().   
+0000dc30: 2020 2020 2073 656c 665f 6465 7269 7665       self_derive
+0000dc40: 645f 6261 7365 7320 3d20 7365 6c66 2e67  d_bases = self.g
+0000dc50: 6574 5f64 6572 6976 6564 5f62 6173 6573  et_derived_bases
+0000dc60: 5f73 6574 2829 0a20 2020 2020 2020 2069  _set().        i
+0000dc70: 6620 6f74 6865 725f 6465 7269 7665 645f  f other_derived_
+0000dc80: 6261 7365 7320 213d 2073 656c 665f 6465  bases != self_de
+0000dc90: 7269 7665 645f 6261 7365 7320 616e 6420  rived_bases and 
+0000dca0: 7365 6c66 5f64 6572 6976 6564 5f62 6173  self_derived_bas
+0000dcb0: 6573 2e69 7373 7562 7365 7428 6f74 6865  es.issubset(othe
+0000dcc0: 725f 6465 7269 7665 645f 6261 7365 7329  r_derived_bases)
+0000dcd0: 3a0a 2020 2020 2020 2020 2020 2020 2320  :.            # 
+0000dce0: 4176 6f69 6420 6379 636c 6573 206f 6e20  Avoid cycles on 
+0000dcf0: 6465 7269 7665 645f 6672 6f6d 5f74 6167  derived_from_tag
+0000dd00: 2e20 6874 7470 733a 2f2f 6769 7468 7562  . https://github
+0000dd10: 2e63 6f6d 2f72 7774 682d 6936 2f72 6574  .com/rwth-i6/ret
+0000dd20: 7572 6e6e 2f69 7373 7565 732f 3130 3534  urnn/issues/1054
+0000dd30: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
+0000dd40: 6820 7574 696c 2e67 7561 7264 5f69 6e66  h util.guard_inf
+0000dd50: 696e 6974 655f 7265 6375 7273 696f 6e28  inite_recursion(
+0000dd60: 5f64 2e44 696d 2e64 6563 6c61 7265 5f73  _d.Dim.declare_s
+0000dd70: 616d 655f 6173 2c20 6f74 6865 722c 2073  ame_as, other, s
+0000dd80: 656c 6629 3a0a 2020 2020 2020 2020 2020  elf):.          
+0000dd90: 2020 2020 2020 7265 7475 726e 206f 7468        return oth
+0000dda0: 6572 2e64 6563 6c61 7265 5f73 616d 655f  er.declare_same_
+0000ddb0: 6173 2873 656c 6629 0a20 2020 2020 2020  as(self).       
+0000ddc0: 2069 6620 7365 6c66 2e5f 6578 7472 613a   if self._extra:
+0000ddd0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000dde0: 662e 5f65 7874 7261 2e64 6572 6976 6564  f._extra.derived
+0000ddf0: 5f66 726f 6d5f 6f70 203d 204e 6f6e 650a  _from_op = None.
+0000de00: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000de10: 2e5f 6578 7472 612e 6465 7269 7665 645f  ._extra.derived_
+0000de20: 6672 6f6d 5f74 6167 203d 204e 6f6e 650a  from_tag = None.
+0000de30: 2020 2020 2020 2020 6966 2073 656c 665f          if self_
+0000de40: 7361 6d65 5f61 7320 6973 206e 6f74 2073  same_as is not s
+0000de50: 656c 663a 0a20 2020 2020 2020 2020 2020  elf:.           
+0000de60: 2061 7373 6572 7420 6e6f 7420 7365 6c66   assert not self
+0000de70: 5f73 616d 655f 6173 2e73 616d 655f 6173  _same_as.same_as
+0000de80: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000de90: 7365 6c66 5f73 616d 655f 6173 2069 7320  self_same_as is 
+0000dea0: 6f74 6865 725f 7361 6d65 5f62 6173 653a  other_same_base:
+0000deb0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000dec0: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+0000ded0: 2020 2020 7769 7468 2075 7469 6c2e 6775      with util.gu
+0000dee0: 6172 645f 696e 6669 6e69 7465 5f72 6563  ard_infinite_rec
+0000def0: 7572 7369 6f6e 285f 642e 4469 6d2e 6465  ursion(_d.Dim.de
+0000df00: 636c 6172 655f 7361 6d65 5f61 732c 2073  clare_same_as, s
+0000df10: 656c 665f 7361 6d65 5f61 732c 206f 7468  elf_same_as, oth
+0000df20: 6572 5f73 616d 655f 6261 7365 293a 0a20  er_same_base):. 
+0000df30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+0000df40: 656c 665f 7361 6d65 5f61 732e 6465 636c  elf_same_as.decl
+0000df50: 6172 655f 7361 6d65 5f61 7328 6f74 6865  are_same_as(othe
+0000df60: 725f 7361 6d65 5f62 6173 6529 0a20 2020  r_same_base).   
+0000df70: 2020 2020 2020 2020 2069 6620 2873 656c           if (sel
+0000df80: 662e 6479 6e5f 7369 7a65 5f65 7874 2069  f.dyn_size_ext i
+0000df90: 7320 4e6f 6e65 206f 7220 6e6f 7420 7365  s None or not se
+0000dfa0: 6c66 2e5f 7661 6c69 6461 7465 5f69 6e5f  lf._validate_in_
+0000dfb0: 6375 7272 656e 745f 6772 6170 6828 2929  current_graph())
+0000dfc0: 2061 6e64 2073 656c 665f 7361 6d65 5f61   and self_same_a
+0000dfd0: 732e 6479 6e5f 7369 7a65 5f65 7874 3a0a  s.dyn_size_ext:.
+0000dfe0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000dff0: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+0000e000: 7420 3d20 7365 6c66 5f73 616d 655f 6173  t = self_same_as
+0000e010: 2e67 6574 5f64 796e 5f73 697a 655f 6578  .get_dyn_size_ex
+0000e020: 745f 666f 725f 6261 7463 685f 6374 7828  t_for_batch_ctx(
+0000e030: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e040: 2020 2020 2073 656c 662e 6261 7463 682c       self.batch,
+0000e050: 2073 656c 662e 636f 6e74 726f 6c5f 666c   self.control_fl
+0000e060: 6f77 5f63 7478 2c20 7465 6d70 6c61 7465  ow_ctx, template
+0000e070: 5f6f 6e6c 793d 5472 7565 0a20 2020 2020  _only=True.     
+0000e080: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+0000e090: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+0000e0a0: 2020 2020 2020 2069 6620 7365 6c66 2e5f         if self._
+0000e0b0: 6578 7472 613a 0a20 2020 2020 2020 2020  extra:.         
+0000e0c0: 2020 2020 2020 2066 6f72 2064 696d 5f20         for dim_ 
+0000e0d0: 696e 2073 656c 662e 5f65 7874 7261 2e73  in self._extra.s
+0000e0e0: 616d 655f 666f 725f 6261 7463 685f 6374  ame_for_batch_ct
+0000e0f0: 782e 7661 6c75 6573 2829 3a0a 2020 2020  x.values():.    
+0000e100: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e110: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
+0000e120: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
+0000e130: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000e140: 2020 2020 2069 6620 6469 6d5f 2e5f 6578       if dim_._ex
+0000e150: 7472 613a 0a20 2020 2020 2020 2020 2020  tra:.           
+0000e160: 2020 2020 2020 2020 2020 2020 2023 206e               # n
+0000e170: 6f69 6e73 7065 6374 696f 6e20 5079 5072  oinspection PyPr
+0000e180: 6f74 6563 7465 644d 656d 6265 720a 2020  otectedMember.  
+0000e190: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1a0: 2020 2020 2020 6469 6d5f 2e5f 6578 7472        dim_._extr
+0000e1b0: 612e 6465 7269 7665 645f 6672 6f6d 5f6f  a.derived_from_o
+0000e1c0: 7020 3d20 4e6f 6e65 0a20 2020 2020 2020  p = None.       
+0000e1d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e1e0: 2023 206e 6f69 6e73 7065 6374 696f 6e20   # noinspection 
+0000e1f0: 5079 5072 6f74 6563 7465 644d 656d 6265  PyProtectedMembe
+0000e200: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+0000e210: 2020 2020 2020 2020 2020 6469 6d5f 2e5f            dim_._
+0000e220: 6578 7472 612e 6465 7269 7665 645f 6672  extra.derived_fr
+0000e230: 6f6d 5f74 6167 203d 204e 6f6e 650a 2020  om_tag = None.  
+0000e240: 2020 2020 2020 2320 4e6f 7720 6d65 7267        # Now merg
+0000e250: 6520 6578 6973 7469 6e67 2076 6172 6961  e existing varia
+0000e260: 6e74 732e 2042 7574 206f 6e6c 7920 6966  nts. But only if
+0000e270: 206e 6f74 2064 6572 6976 6564 2076 6961   not derived via
+0000e280: 206f 702c 2062 6563 6175 7365 2069 6e20   op, because in 
+0000e290: 7468 6174 2063 6173 652c 2077 6520 6361  that case, we ca
+0000e2a0: 6e20 2861 6e64 2073 686f 756c 6421 290a  n (and should!).
+0000e2b0: 2020 2020 2020 2020 2320 6175 746f 6d61          # automa
+0000e2c0: 7469 6361 6c6c 7920 696e 6665 7220 6974  tically infer it
+0000e2d0: 2e20 4e6f 7465 2074 6861 7420 7765 206f  . Note that we o
+0000e2e0: 6e6c 7920 676f 7420 6865 7265 2077 6865  nly got here whe
+0000e2f0: 6e20 7468 6520 6f74 6865 7220 6973 206e  n the other is n
+0000e300: 6f74 2074 6865 2073 616d 6520 6469 6d2c  ot the same dim,
+0000e310: 2073 6f20 6974 206d 6561 6e73 2074 6861   so it means tha
+0000e320: 740a 2020 2020 2020 2020 2320 7468 6520  t.        # the 
+0000e330: 6f74 6865 7220 6973 2072 6561 6c6c 7920  other is really 
+0000e340: 6469 6666 6572 656e 742c 2074 6865 2073  different, the s
+0000e350: 697a 6573 2061 7265 2070 6f74 656e 7469  izes are potenti
+0000e360: 616c 6c79 2064 6966 6665 7265 6e74 2c20  ally different, 
+0000e370: 6275 7420 7765 2077 616e 7420 746f 206f  but we want to o
+0000e380: 7665 7274 616b 6520 7468 6520 6f74 6865  vertake the othe
+0000e390: 722e 0a20 2020 2020 2020 2069 6620 6f74  r..        if ot
+0000e3a0: 6865 725f 7361 6d65 5f62 6173 652e 6465  her_same_base.de
+0000e3b0: 7269 7665 645f 6672 6f6d 5f6f 703a 0a20  rived_from_op:. 
+0000e3c0: 2020 2020 2020 2020 2020 2023 2043 6c65             # Cle
+0000e3d0: 616e 7570 2065 7665 7279 7468 696e 672c  anup everything,
+0000e3e0: 2065 7370 2070 6f74 656e 7469 616c 2061   esp potential a
+0000e3f0: 6c72 6561 6479 2063 6f6d 7075 7465 6420  lready computed 
+0000e400: 7369 7a65 732c 2061 7320 7468 6573 6520  sizes, as these 
+0000e410: 6d69 6768 7420 6265 2069 6e76 616c 6964  might be invalid
+0000e420: 2e0a 2020 2020 2020 2020 2020 2020 666f  ..            fo
+0000e430: 7220 6469 6d5f 2069 6e20 5b73 656c 665f  r dim_ in [self_
+0000e440: 7361 6d65 5f61 732c 2073 656c 665d 202b  same_as, self] +
+0000e450: 2028 6c69 7374 2873 656c 662e 5f65 7874   (list(self._ext
+0000e460: 7261 2e73 616d 655f 666f 725f 6261 7463  ra.same_for_batc
+0000e470: 685f 6374 782e 7661 6c75 6573 2829 2920  h_ctx.values()) 
+0000e480: 6966 2073 656c 662e 5f65 7874 7261 2065  if self._extra e
+0000e490: 6c73 6520 5b5d 293a 0a20 2020 2020 2020  lse []):.       
+0000e4a0: 2020 2020 2020 2020 2069 6620 6469 6d5f           if dim_
+0000e4b0: 2e64 796e 5f73 697a 655f 6578 743a 0a20  .dyn_size_ext:. 
+0000e4c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e4d0: 2020 2064 696d 5f2e 6479 6e5f 7369 7a65     dim_.dyn_size
+0000e4e0: 5f65 7874 2e70 6c61 6365 686f 6c64 6572  _ext.placeholder
+0000e4f0: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+0000e500: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
+0000e510: 5f6d 6572 6765 5f73 616d 655f 666f 725f  _merge_same_for_
+0000e520: 6261 7463 685f 6374 785f 6469 6374 2873  batch_ctx_dict(s
+0000e530: 656c 6629 0a20 2020 2020 2020 206f 7468  elf).        oth
+0000e540: 6572 2e5f 6d61 7962 655f 7570 6461 7465  er._maybe_update
+0000e550: 2829 0a20 2020 2020 2020 2073 656c 662e  ().        self.
+0000e560: 7361 6d65 5f61 7320 3d20 6f74 6865 725f  same_as = other_
+0000e570: 7361 6d65 5f62 6173 650a 2020 2020 2020  same_base.      
+0000e580: 2020 7365 6c66 2e5f 6d61 7962 655f 7570    self._maybe_up
+0000e590: 6461 7465 2829 0a20 2020 2020 2020 2069  date().        i
+0000e5a0: 6620 7365 6c66 2e64 796e 5f73 697a 6520  f self.dyn_size 
+0000e5b0: 6973 206e 6f74 204e 6f6e 6520 616e 6420  is not None and 
+0000e5c0: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
+0000e5d0: 6479 6e5f 7369 7a65 2069 7320 6e6f 7420  dyn_size is not 
+0000e5e0: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+0000e5f0: 2020 6966 2073 656c 662e 6479 6e5f 7369    if self.dyn_si
+0000e600: 7a65 2069 7320 6e6f 7420 6f74 6865 725f  ze is not other_
+0000e610: 7361 6d65 5f62 6173 652e 6479 6e5f 7369  same_base.dyn_si
+0000e620: 7a65 3a0a 2020 2020 2020 2020 2020 2020  ze:.            
+0000e630: 2020 2020 6966 2073 656c 662e 6261 7463      if self.batc
+0000e640: 6820 3d3d 206f 7468 6572 5f73 616d 655f  h == other_same_
+0000e650: 6261 7365 2e62 6174 6368 2061 6e64 2073  base.batch and s
+0000e660: 656c 662e 636f 6e74 726f 6c5f 666c 6f77  elf.control_flow
+0000e670: 5f63 7478 203d 3d20 6f74 6865 725f 7361  _ctx == other_sa
+0000e680: 6d65 5f62 6173 652e 636f 6e74 726f 6c5f  me_base.control_
+0000e690: 666c 6f77 5f63 7478 3a0a 2020 2020 2020  flow_ctx:.      
+0000e6a0: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000e6b0: 4e6f 7465 3a20 496e 7374 6561 6420 6f66  Note: Instead of
+0000e6c0: 206d 616b 696e 6720 7468 6973 2061 2077   making this a w
+0000e6d0: 6172 6e69 6e67 2c20 7765 2063 6f75 6c64  arning, we could
+0000e6e0: 2061 6c73 6f20 656e 666f 7263 6520 7468   also enforce th
+0000e6f0: 6973 2061 7420 736f 6d65 2070 6f69 6e74  is at some point
+0000e700: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e710: 2020 2020 2020 2320 2020 5468 6520 7573        #   The us
+0000e720: 6572 2073 686f 756c 6420 6265 2061 626c  er should be abl
+0000e730: 6520 746f 2066 6978 2060 6578 7465 726e  e to fix `extern
+0000e740: 5f64 6174 6160 2069 6e20 7468 6520 636f  _data` in the co
+0000e750: 6e66 6967 0a20 2020 2020 2020 2020 2020  nfig.           
+0000e760: 2020 2020 2020 2020 2023 2020 2073 7563           #   suc
+0000e770: 6820 7468 6174 2074 6869 7320 6973 2063  h that this is c
+0000e780: 6f72 7265 6374 2069 6e20 7468 6520 6669  orrect in the fi
+0000e790: 7273 7420 706c 6163 652e 0a20 2020 2020  rst place..     
+0000e7a0: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+0000e7b0: 2020 2041 6c73 6f2c 2069 6e20 6164 6469     Also, in addi
+0000e7c0: 7469 6f6e 2074 6f20 7468 6973 2077 6172  tion to this war
+0000e7d0: 6e69 6e67 2c0a 2020 2020 2020 2020 2020  ning,.          
+0000e7e0: 2020 2020 2020 2020 2020 2320 2020 7765            #   we
+0000e7f0: 206d 6967 6874 2077 616e 7420 746f 2061   might want to a
+0000e800: 6464 2073 6f6d 6520 7275 6e74 696d 6520  dd some runtime 
+0000e810: 6368 6563 6b20 6f6e 2074 6865 2065 7120  check on the eq 
+0000e820: 6f66 2074 6865 2064 796e 2073 697a 6573  of the dyn sizes
+0000e830: 2e0a 2020 2020 2020 2020 2020 2020 2020  ..              
+0000e840: 2020 2020 2020 7072 696e 7428 0a20 2020        print(.   
+0000e850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000e860: 2020 2020 2022 5761 726e 696e 673a 2061       "Warning: a
+0000e870: 7373 756d 696e 6720 6469 6d20 7461 6773  ssuming dim tags
+0000e880: 2061 7265 2073 616d 6520 7769 7468 2064   are same with d
+0000e890: 6966 6665 7265 6e74 2073 697a 6520 706c  ifferent size pl
+0000e8a0: 6163 6568 6f6c 6465 7273 3a20 2572 2076  aceholders: %r v
+0000e8b0: 7320 2572 220a 2020 2020 2020 2020 2020  s %r".          
+0000e8c0: 2020 2020 2020 2020 2020 2020 2020 2520                % 
+0000e8d0: 2873 656c 662e 6479 6e5f 7369 7a65 2c20  (self.dyn_size, 
+0000e8e0: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
+0000e8f0: 6479 6e5f 7369 7a65 290a 2020 2020 2020  dyn_size).      
+0000e900: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000e910: 2020 2020 2020 2020 2320 4966 2077 6520          # If we 
+0000e920: 6861 7665 2061 2064 6566 696e 6564 2073  have a defined s
+0000e930: 6f75 7263 652c 2061 6e64 2074 6869 7320  ource, and this 
+0000e940: 6973 2061 2064 796e 616d 6963 2073 7061  is a dynamic spa
+0000e950: 7469 616c 2061 7869 732c 2061 6e64 2069  tial axis, and i
+0000e960: 7420 7761 7320 756e 6465 6669 6e65 6420  t was undefined 
+0000e970: 6265 666f 7265 2c0a 2020 2020 2020 2020  before,.        
+0000e980: 2320 6d61 7962 6520 7765 2063 616e 206f  # maybe we can o
+0000e990: 7665 7274 616b 6520 7468 6520 7369 7a65  vertake the size
+0000e9a0: 5f70 6c61 6365 686f 6c64 6572 206e 6f77  _placeholder now
+0000e9b0: 2e0a 2020 2020 2020 2020 6966 206f 7468  ..        if oth
+0000e9c0: 6572 5f73 616d 655f 6261 7365 2e64 796e  er_same_base.dyn
+0000e9d0: 5f73 697a 6520 6973 206e 6f74 204e 6f6e  _size is not Non
+0000e9e0: 6520 616e 6420 7365 6c66 2e5f 6578 7472  e and self._extr
+0000e9f0: 6120 616e 6420 7365 6c66 2e5f 6578 7472  a and self._extr
+0000ea00: 612e 7372 635f 6461 7461 3a0a 2020 2020  a.src_data:.    
+0000ea10: 2020 2020 2020 2020 6173 7365 7274 2069          assert i
+0000ea20: 7369 6e73 7461 6e63 6528 7365 6c66 2e5f  sinstance(self._
+0000ea30: 6578 7472 612e 7372 635f 6178 6973 2c20  extra.src_axis, 
+0000ea40: 696e 7429 0a20 2020 2020 2020 2020 2020  int).           
+0000ea50: 2023 204d 6179 6265 2069 7420 6368 616e   # Maybe it chan
+0000ea60: 6765 6420 696e 2074 6865 206d 6561 6e77  ged in the meanw
+0000ea70: 6869 6c65 2c20 736f 2063 6865 636b 2e0a  hile, so check..
+0000ea80: 2020 2020 2020 2020 2020 2020 7461 6720              tag 
+0000ea90: 3d20 7365 6c66 2e5f 6578 7472 612e 7372  = self._extra.sr
+0000eaa0: 635f 6461 7461 2e67 6574 5f64 696d 5f74  c_data.get_dim_t
+0000eab0: 6167 2873 656c 662e 5f65 7874 7261 2e73  ag(self._extra.s
+0000eac0: 7263 5f61 7869 7329 0a20 2020 2020 2020  rc_axis).       
+0000ead0: 2020 2020 2069 6620 7461 672e 6465 7363       if tag.desc
+0000eae0: 7269 7074 696f 6e20 3d3d 2073 656c 662e  ription == self.
+0000eaf0: 6465 7363 7269 7074 696f 6e20 616e 6420  description and 
+0000eb00: 286e 6f74 2074 6167 2e64 796e 5f73 697a  (not tag.dyn_siz
+0000eb10: 655f 6578 7420 6f72 206e 6f74 2074 6167  e_ext or not tag
+0000eb20: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
+0000eb30: 7272 656e 745f 6772 6170 6828 2929 3a0a  rrent_graph()):.
+0000eb40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000eb50: 7461 672e 6479 6e5f 7369 7a65 5f65 7874  tag.dyn_size_ext
+0000eb60: 203d 2073 656c 662e 6765 745f 6479 6e5f   = self.get_dyn_
+0000eb70: 7369 7a65 5f65 7874 5f66 6f72 5f62 6174  size_ext_for_bat
+0000eb80: 6368 5f63 7478 280a 2020 2020 2020 2020  ch_ctx(.        
+0000eb90: 2020 2020 2020 2020 2020 2020 7461 672e              tag.
+0000eba0: 6261 7463 682c 2074 6167 2e63 6f6e 7472  batch, tag.contr
+0000ebb0: 6f6c 5f66 6c6f 775f 6374 782c 2074 656d  ol_flow_ctx, tem
+0000ebc0: 706c 6174 655f 6f6e 6c79 3d54 7275 650a  plate_only=True.
+0000ebd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ebe0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+0000ebf0: 2020 7461 672e 5f6d 6179 6265 5f75 7064    tag._maybe_upd
+0000ec00: 6174 6528 290a 2020 2020 2020 2020 2320  ate().        # 
+0000ec10: 4966 206f 7468 6572 7320 6479 6e5f 7369  If others dyn_si
+0000ec20: 7a65 2069 7320 4e6f 6e65 2062 7574 2077  ze is None but w
+0000ec30: 6520 6861 7665 2061 2064 796e 5f73 697a  e have a dyn_siz
+0000ec40: 652c 206d 6179 6265 2075 7064 6174 6520  e, maybe update 
+0000ec50: 6f74 6865 7273 2064 796e 5f73 697a 652e  others dyn_size.
+0000ec60: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000ec70: 2e64 796e 5f73 697a 6520 6973 206e 6f74  .dyn_size is not
+0000ec80: 204e 6f6e 6520 616e 6420 6f74 6865 725f   None and other_
+0000ec90: 7361 6d65 5f62 6173 652e 6479 6e5f 7369  same_base.dyn_si
+0000eca0: 7a65 2069 7320 6e6f 7420 7365 6c66 2e64  ze is not self.d
+0000ecb0: 796e 5f73 697a 653a 0a20 2020 2020 2020  yn_size:.       
+0000ecc0: 2020 2020 2023 2043 6f75 6c64 2062 6520       # Could be 
+0000ecd0: 756e 7365 7420 6966 2069 7420 636f 6d65  unset if it come
+0000ece0: 7320 6672 6f6d 2074 6865 2063 6f6e 6669  s from the confi
+0000ecf0: 672c 206f 7220 6672 6f6d 2070 7265 7620  g, or from prev 
+0000ed00: 6772 6170 6820 6372 6561 7469 6f6e 2e0a  graph creation..
+0000ed10: 2020 2020 2020 2020 2020 2020 2320 5468              # Th
+0000ed20: 6973 2069 7320 696d 706f 7274 616e 7420  is is important 
+0000ed30: 7375 6368 2074 6861 7420 7365 6c66 2e63  such that self.c
+0000ed40: 616e 5f63 6f6d 7061 7265 2829 2069 7320  an_compare() is 
+0000ed50: 7361 6e65 2e0a 2020 2020 2020 2020 2020  sane..          
+0000ed60: 2020 6966 206f 7468 6572 5f73 616d 655f    if other_same_
+0000ed70: 6261 7365 2e64 796e 5f73 697a 6520 6973  base.dyn_size is
+0000ed80: 204e 6f6e 6520 6f72 206e 6f74 206f 7468   None or not oth
+0000ed90: 6572 5f73 616d 655f 6261 7365 2e5f 7661  er_same_base._va
+0000eda0: 6c69 6461 7465 5f69 6e5f 6375 7272 656e  lidate_in_curren
+0000edb0: 745f 6772 6170 6828 293a 0a20 2020 2020  t_graph():.     
+0000edc0: 2020 2020 2020 2020 2020 206f 7468 6572             other
+0000edd0: 5f73 616d 655f 6261 7365 2e64 796e 5f73  _same_base.dyn_s
+0000ede0: 697a 655f 6578 7420 3d20 7365 6c66 2e67  ize_ext = self.g
+0000edf0: 6574 5f64 796e 5f73 697a 655f 6578 745f  et_dyn_size_ext_
+0000ee00: 666f 725f 6261 7463 685f 6374 7828 0a20  for_batch_ctx(. 
+0000ee10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000ee20: 2020 206f 7468 6572 5f73 616d 655f 6261     other_same_ba
+0000ee30: 7365 2e62 6174 6368 2c20 6f74 6865 725f  se.batch, other_
+0000ee40: 7361 6d65 5f62 6173 652e 636f 6e74 726f  same_base.contro
+0000ee50: 6c5f 666c 6f77 5f63 7478 2c20 7465 6d70  l_flow_ctx, temp
+0000ee60: 6c61 7465 5f6f 6e6c 793d 5472 7565 0a20  late_only=True. 
+0000ee70: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+0000ee80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000ee90: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000eea0: 2e5f 6d61 7962 655f 7570 6461 7465 2829  ._maybe_update()
+0000eeb0: 0a20 2020 2020 2020 2069 6620 6e6f 7420  .        if not 
+0000eec0: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+0000eed0: 7420 6f72 206e 6f74 2073 656c 662e 5f76  t or not self._v
+0000eee0: 616c 6964 6174 655f 696e 5f63 7572 7265  alidate_in_curre
+0000eef0: 6e74 5f67 7261 7068 2829 3a0a 2020 2020  nt_graph():.    
+0000ef00: 2020 2020 2020 2020 7365 6c66 2e64 796e          self.dyn
+0000ef10: 5f73 697a 655f 6578 7420 3d20 6f74 6865  _size_ext = othe
+0000ef20: 725f 7361 6d65 5f62 6173 652e 6765 745f  r_same_base.get_
+0000ef30: 6479 6e5f 7369 7a65 5f65 7874 5f66 6f72  dyn_size_ext_for
+0000ef40: 5f62 6174 6368 5f63 7478 280a 2020 2020  _batch_ctx(.    
+0000ef50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000ef60: 2e62 6174 6368 2c20 7365 6c66 2e63 6f6e  .batch, self.con
+0000ef70: 7472 6f6c 5f66 6c6f 775f 6374 782c 2074  trol_flow_ctx, t
+0000ef80: 656d 706c 6174 655f 6f6e 6c79 3d54 7275  emplate_only=Tru
+0000ef90: 650a 2020 2020 2020 2020 2020 2020 290a  e.            ).
+0000efa0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000efb0: 2e5f 6d61 7962 655f 7570 6461 7465 2829  ._maybe_update()
+0000efc0: 0a20 2020 2020 2020 2065 6c69 6620 6f74  .        elif ot
+0000efd0: 6865 725f 7361 6d65 5f62 6173 652e 6479  her_same_base.dy
+0000efe0: 6e5f 7369 7a65 5f65 7874 2069 7320 4e6f  n_size_ext is No
+0000eff0: 6e65 206f 7220 6e6f 7420 6f74 6865 725f  ne or not other_
+0000f000: 7361 6d65 5f62 6173 652e 5f76 616c 6964  same_base._valid
+0000f010: 6174 655f 696e 5f63 7572 7265 6e74 5f67  ate_in_current_g
+0000f020: 7261 7068 2829 3a0a 2020 2020 2020 2020  raph():.        
+0000f030: 2020 2020 6f74 6865 725f 7361 6d65 5f62      other_same_b
+0000f040: 6173 652e 6479 6e5f 7369 7a65 5f65 7874  ase.dyn_size_ext
+0000f050: 203d 2073 656c 662e 6765 745f 6479 6e5f   = self.get_dyn_
+0000f060: 7369 7a65 5f65 7874 5f66 6f72 5f62 6174  size_ext_for_bat
+0000f070: 6368 5f63 7478 280a 2020 2020 2020 2020  ch_ctx(.        
+0000f080: 2020 2020 2020 2020 6f74 6865 725f 7361          other_sa
+0000f090: 6d65 5f62 6173 652e 6261 7463 682c 206f  me_base.batch, o
+0000f0a0: 7468 6572 5f73 616d 655f 6261 7365 2e63  ther_same_base.c
+0000f0b0: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 782c  ontrol_flow_ctx,
+0000f0c0: 2074 656d 706c 6174 655f 6f6e 6c79 3d54   template_only=T
+0000f0d0: 7275 650a 2020 2020 2020 2020 2020 2020  rue.            
+0000f0e0: 290a 2020 2020 2020 2020 2020 2020 6f74  ).            ot
+0000f0f0: 6865 725f 7361 6d65 5f62 6173 652e 5f6d  her_same_base._m
+0000f100: 6179 6265 5f75 7064 6174 6528 290a 2020  aybe_update().  
+0000f110: 2020 2020 2020 6966 2073 656c 662e 6973        if self.is
+0000f120: 5f64 696d 5f6b 6e6f 776e 2829 2061 6e64  _dim_known() and
+0000f130: 206f 7468 6572 2e69 735f 6469 6d5f 6b6e   other.is_dim_kn
+0000f140: 6f77 6e28 293a 0a20 2020 2020 2020 2020  own():.         
+0000f150: 2020 2061 7373 6572 7420 7365 6c66 2e64     assert self.d
+0000f160: 696d 656e 7369 6f6e 203d 3d20 6f74 6865  imension == othe
+0000f170: 722e 6469 6d65 6e73 696f 6e0a 2020 2020  r.dimension.    
+0000f180: 2020 2020 656c 6966 2073 656c 662e 6973      elif self.is
+0000f190: 5f64 696d 5f6b 6e6f 776e 2829 2061 6e64  _dim_known() and
+0000f1a0: 206e 6f74 206f 7468 6572 2e69 735f 6469   not other.is_di
+0000f1b0: 6d5f 6b6e 6f77 6e28 293a 0a20 2020 2020  m_known():.     
+0000f1c0: 2020 2020 2020 206f 7468 6572 2e63 6170         other.cap
+0000f1d0: 6163 6974 7920 3d20 7365 6c66 2e63 6170  acity = self.cap
+0000f1e0: 6163 6974 790a 2020 2020 2020 2020 2020  acity.          
+0000f1f0: 2020 6f74 6865 722e 7369 7a65 203d 2073    other.size = s
+0000f200: 656c 662e 7369 7a65 0a20 2020 2020 2020  elf.size.       
+0000f210: 2065 6c69 6620 6e6f 7420 7365 6c66 2e69   elif not self.i
+0000f220: 735f 6469 6d5f 6b6e 6f77 6e28 2920 616e  s_dim_known() an
+0000f230: 6420 6f74 6865 722e 6973 5f64 696d 5f6b  d other.is_dim_k
+0000f240: 6e6f 776e 2829 3a0a 2020 2020 2020 2020  nown():.        
+0000f250: 2020 2020 7365 6c66 2e63 6170 6163 6974      self.capacit
+0000f260: 7920 3d20 6f74 6865 722e 6361 7061 6369  y = other.capaci
+0000f270: 7479 0a20 2020 2020 2020 2020 2020 2073  ty.            s
+0000f280: 656c 662e 7369 7a65 203d 206f 7468 6572  elf.size = other
+0000f290: 2e73 697a 650a 2020 2020 2020 2020 6966  .size.        if
+0000f2a0: 2073 656c 662e 766f 6361 6220 616e 6420   self.vocab and 
+0000f2b0: 6e6f 7420 6f74 6865 725f 7361 6d65 5f62  not other_same_b
+0000f2c0: 6173 652e 766f 6361 623a 0a20 2020 2020  ase.vocab:.     
+0000f2d0: 2020 2020 2020 206f 7468 6572 5f73 616d         other_sam
+0000f2e0: 655f 6261 7365 2e76 6f63 6162 203d 2073  e_base.vocab = s
+0000f2f0: 656c 662e 766f 6361 620a 2020 2020 2020  elf.vocab.      
+0000f300: 2020 656c 6966 206f 7468 6572 5f73 616d    elif other_sam
+0000f310: 655f 6261 7365 2e76 6f63 6162 2061 6e64  e_base.vocab and
+0000f320: 206e 6f74 2073 656c 662e 766f 6361 623a   not self.vocab:
+0000f330: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+0000f340: 662e 766f 6361 6220 3d20 6f74 6865 725f  f.vocab = other_
+0000f350: 7361 6d65 5f62 6173 652e 766f 6361 620a  same_base.vocab.
+0000f360: 2020 2020 2020 2020 7365 6c66 2e5f 6d61          self._ma
+0000f370: 6b65 5f65 7874 7261 2829 0a20 2020 2020  ke_extra().     
+0000f380: 2020 2073 656c 665f 7361 6d65 5f61 732e     self_same_as.
+0000f390: 5f6d 616b 655f 6578 7472 6128 290a 2020  _make_extra().  
+0000f3a0: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
+0000f3b0: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
+0000f3c0: 4d65 6d62 6572 0a20 2020 2020 2020 2073  Member.        s
+0000f3d0: 656c 662e 5f65 7874 7261 2e61 7574 6f5f  elf._extra.auto_
+0000f3e0: 6765 6e65 7261 7465 6420 3d20 7365 6c66  generated = self
+0000f3f0: 5f73 616d 655f 6173 2e5f 6578 7472 612e  _same_as._extra.
+0000f400: 6175 746f 5f67 656e 6572 6174 6564 203d  auto_generated =
+0000f410: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000f420: 2e61 7574 6f5f 6765 6e65 7261 7465 640a  .auto_generated.
+0000f430: 2020 2020 2020 2020 2320 5461 6b65 206f          # Take o
+0000f440: 7665 7220 6465 7269 7665 645f 6672 6f6d  ver derived_from
+0000f450: 5f6f 702e 2048 6f77 6576 6572 2c20 6f6e  _op. However, on
+0000f460: 6c79 2069 6620 7468 6973 2077 6f75 6c64  ly if this would
+0000f470: 206e 6f74 2069 6e74 726f 6475 6365 2063   not introduce c
+0000f480: 7963 6c65 7321 0a20 2020 2020 2020 2069  ycles!.        i
+0000f490: 6620 6e6f 7420 7365 6c66 5f64 6572 6976  f not self_deriv
+0000f4a0: 6564 5f62 6173 6573 2e69 7373 7570 6572  ed_bases.issuper
+0000f4b0: 7365 7428 6f74 6865 725f 6465 7269 7665  set(other_derive
+0000f4c0: 645f 6261 7365 7329 3a0a 2020 2020 2020  d_bases):.      
+0000f4d0: 2020 2020 2020 6966 2073 656c 662e 6465        if self.de
+0000f4e0: 7269 7665 645f 6672 6f6d 5f6f 7020 616e  rived_from_op an
+0000f4f0: 6420 6e6f 7420 6f74 6865 725f 7361 6d65  d not other_same
+0000f500: 5f62 6173 652e 6465 7269 7665 645f 6672  _base.derived_fr
+0000f510: 6f6d 5f6f 703a 0a20 2020 2020 2020 2020  om_op:.         
+0000f520: 2020 2020 2020 2023 206e 6f69 6e73 7065         # noinspe
+0000f530: 6374 696f 6e20 5079 5072 6f74 6563 7465  ction PyProtecte
+0000f540: 644d 656d 6265 720a 2020 2020 2020 2020  dMember.        
+0000f550: 2020 2020 2020 2020 6f74 6865 725f 7361          other_sa
+0000f560: 6d65 5f62 6173 652e 5f6d 616b 655f 6578  me_base._make_ex
+0000f570: 7472 6128 292e 6465 7269 7665 645f 6672  tra().derived_fr
+0000f580: 6f6d 5f6f 7020 3d20 7365 6c66 2e64 6572  om_op = self.der
+0000f590: 6976 6564 5f66 726f 6d5f 6f70 0a20 2020  ived_from_op.   
+0000f5a0: 2020 2020 2020 2020 2065 6c69 6620 6f74           elif ot
+0000f5b0: 6865 725f 7361 6d65 5f62 6173 652e 6465  her_same_base.de
+0000f5c0: 7269 7665 645f 6672 6f6d 5f6f 7020 616e  rived_from_op an
+0000f5d0: 6420 6e6f 7420 7365 6c66 2e64 6572 6976  d not self.deriv
+0000f5e0: 6564 5f66 726f 6d5f 6f70 3a0a 2020 2020  ed_from_op:.    
+0000f5f0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000f600: 2e5f 6d61 6b65 5f65 7874 7261 2829 2e64  ._make_extra().d
+0000f610: 6572 6976 6564 5f66 726f 6d5f 6f70 203d  erived_from_op =
+0000f620: 206f 7468 6572 5f73 616d 655f 6261 7365   other_same_base
+0000f630: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+0000f640: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+0000f650: 2e5f 6578 7472 6120 616e 6420 6e6f 7420  ._extra and not 
+0000f660: 6f74 6865 725f 7361 6d65 5f62 6173 652e  other_same_base.
+0000f670: 6973 5f64 796e 616d 6963 2829 3a0a 2020  is_dynamic():.  
+0000f680: 2020 2020 2020 2020 2020 2320 5468 6f73            # Thos
+0000f690: 6520 6d69 6768 7420 6265 2073 6574 2076  e might be set v
+0000f6a0: 6961 2067 6574 5f62 6174 6368 5f66 6f72  ia get_batch_for
+0000f6b0: 5f63 7478 2066 6f72 2061 6e20 756e 6465  _ctx for an unde
+0000f6c0: 6669 6e65 6420 6469 6d2c 0a20 2020 2020  fined dim,.     
+0000f6d0: 2020 2020 2020 2023 2077 6869 6368 206e         # which n
+0000f6e0: 6f77 2062 6563 6f6d 6573 2073 7461 7469  ow becomes stati
+0000f6f0: 6320 6475 6520 746f 2060 6f74 6865 7260  c due to `other`
+0000f700: 2e0a 2020 2020 2020 2020 2020 2020 7365  ..            se
+0000f710: 6c66 2e5f 6578 7472 612e 6261 7463 6820  lf._extra.batch 
+0000f720: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0000f730: 2020 2073 656c 662e 5f65 7874 7261 2e63     self._extra.c
+0000f740: 6f6e 7472 6f6c 5f66 6c6f 775f 6374 7820  ontrol_flow_ctx 
+0000f750: 3d20 4e6f 6e65 0a20 2020 2020 2020 2020  = None.         
+0000f760: 2020 2066 6f72 206b 6579 2c20 6469 6d5f     for key, dim_
+0000f770: 2069 6e20 7365 6c66 2e5f 6578 7472 612e   in self._extra.
+0000f780: 7361 6d65 5f66 6f72 5f62 6174 6368 5f63  same_for_batch_c
+0000f790: 7478 2e69 7465 6d73 2829 3a0a 2020 2020  tx.items():.    
+0000f7a0: 2020 2020 2020 2020 2020 2020 2320 6e6f              # no
+0000f7b0: 696e 7370 6563 7469 6f6e 2050 7950 726f  inspection PyPro
+0000f7c0: 7465 6374 6564 4d65 6d62 6572 0a20 2020  tectedMember.   
+0000f7d0: 2020 2020 2020 2020 2020 2020 2064 696d               dim
+0000f7e0: 5f65 7874 7261 203d 2064 696d 5f2e 5f65  _extra = dim_._e
+0000f7f0: 7874 7261 0a20 2020 2020 2020 2020 2020  xtra.           
+0000f800: 2020 2020 2069 6620 6469 6d5f 6578 7472       if dim_extr
+0000f810: 613a 0a20 2020 2020 2020 2020 2020 2020  a:.             
+0000f820: 2020 2020 2020 2064 696d 5f65 7874 7261         dim_extra
+0000f830: 2e62 6174 6368 203d 204e 6f6e 650a 2020  .batch = None.  
+0000f840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f850: 2020 6469 6d5f 6578 7472 612e 636f 6e74    dim_extra.cont
+0000f860: 726f 6c5f 666c 6f77 5f63 7478 203d 204e  rol_flow_ctx = N
+0000f870: 6f6e 650a 2020 2020 2020 2020 6966 2073  one.        if s
+0000f880: 656c 662e 6261 7463 683a 0a20 2020 2020  elf.batch:.     
+0000f890: 2020 2020 2020 2073 656c 665f 203d 2073         self_ = s
+0000f8a0: 656c 662e 6765 745f 666f 725f 6261 7463  elf.get_for_batc
+0000f8b0: 685f 6374 7828 6261 7463 683d 7365 6c66  h_ctx(batch=self
+0000f8c0: 2e62 6174 6368 2c20 6374 783d 7365 6c66  .batch, ctx=self
+0000f8d0: 2e63 6f6e 7472 6f6c 5f66 6c6f 775f 6374  .control_flow_ct
+0000f8e0: 7829 0a20 2020 2020 2020 2020 2020 2069  x).            i
+0000f8f0: 6620 7365 6c66 5f20 6973 206e 6f74 2073  f self_ is not s
+0000f900: 656c 663a 0a20 2020 2020 2020 2020 2020  elf:.           
+0000f910: 2020 2020 2073 656c 662e 636f 6e74 726f       self.contro
+0000f920: 6c5f 666c 6f77 5f63 7478 203d 2073 656c  l_flow_ctx = sel
+0000f930: 665f 2e63 6f6e 7472 6f6c 5f66 6c6f 775f  f_.control_flow_
+0000f940: 6374 7820 2023 206d 6967 6874 2062 6520  ctx  # might be 
+0000f950: 6469 6666 6572 656e 740a 2020 2020 2020  different.      
+0000f960: 2020 2020 2020 2020 2020 7365 6c66 2e64            self.d
+0000f970: 796e 5f73 697a 655f 6578 7420 3d20 7365  yn_size_ext = se
+0000f980: 6c66 5f2e 6479 6e5f 7369 7a65 5f65 7874  lf_.dyn_size_ext
+0000f990: 2020 2320 6d69 6768 7420 6265 2075 6e73    # might be uns
+0000f9a0: 6574 0a0a 2020 2020 6465 6620 5f6d 6572  et..    def _mer
+0000f9b0: 6765 5f73 616d 655f 666f 725f 6261 7463  ge_same_for_batc
+0000f9c0: 685f 6374 785f 6469 6374 2873 656c 663a  h_ctx_dict(self:
+0000f9d0: 205f 642e 4469 6d2c 206f 7468 6572 3a20   _d.Dim, other: 
+0000f9e0: 5f64 2e44 696d 293a 0a20 2020 2020 2020  _d.Dim):.       
+0000f9f0: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
+0000fa00: 7261 6d20 6f74 6865 723a 0a20 2020 2020  ram other:.     
+0000fa10: 2020 2022 2222 0a20 2020 2020 2020 2023     """.        #
+0000fa20: 206e 6f69 6e73 7065 6374 696f 6e20 5079   noinspection Py
+0000fa30: 5072 6f74 6563 7465 644d 656d 6265 720a  ProtectedMember.
+0000fa40: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+0000fa50: 656c 662e 5f65 7874 7261 2061 6e64 206e  elf._extra and n
+0000fa60: 6f74 206f 7468 6572 2e5f 6578 7472 613a  ot other._extra:
+0000fa70: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+0000fa80: 7572 6e0a 2020 2020 2020 2020 7365 6c66  urn.        self
+0000fa90: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
+0000faa0: 7272 656e 745f 6772 6170 6828 290a 2020  rrent_graph().  
+0000fab0: 2020 2020 2020 6966 2073 656c 662e 5f65        if self._e
+0000fac0: 7874 7261 3a0a 2020 2020 2020 2020 2020  xtra:.          
+0000fad0: 2020 666f 7220 5f2c 2064 696d 2069 6e20    for _, dim in 
+0000fae0: 6c69 7374 2873 656c 662e 5f65 7874 7261  list(self._extra
+0000faf0: 2e73 616d 655f 666f 725f 6261 7463 685f  .same_for_batch_
+0000fb00: 6374 782e 6974 656d 7328 2929 3a0a 2020  ctx.items()):.  
+0000fb10: 2020 2020 2020 2020 2020 2020 2020 6173                as
+0000fb20: 7365 7274 2069 7369 6e73 7461 6e63 6528  sert isinstance(
+0000fb30: 6469 6d2c 205f 642e 4469 6d29 0a20 2020  dim, _d.Dim).   
+0000fb40: 2020 2020 2020 2020 2020 2020 2064 696d               dim
+0000fb50: 2e5f 7661 6c69 6461 7465 5f69 6e5f 6375  ._validate_in_cu
+0000fb60: 7272 656e 745f 6772 6170 6828 290a 2020  rrent_graph().  
+0000fb70: 2020 2020 2020 2320 6e6f 696e 7370 6563        # noinspec
+0000fb80: 7469 6f6e 2050 7950 726f 7465 6374 6564  tion PyProtected
+0000fb90: 4d65 6d62 6572 0a20 2020 2020 2020 2069  Member.        i
+0000fba0: 6620 6f74 6865 722e 5f65 7874 7261 3a0a  f other._extra:.
+0000fbb0: 2020 2020 2020 2020 2020 2020 2320 6e6f              # no
+0000fbc0: 696e 7370 6563 7469 6f6e 2050 7950 726f  inspection PyPro
+0000fbd0: 7465 6374 6564 4d65 6d62 6572 0a20 2020  tectedMember.   
+0000fbe0: 2020 2020 2020 2020 2066 6f72 206b 6579           for key
+0000fbf0: 2c20 6469 6d20 696e 206f 7468 6572 2e5f  , dim in other._
+0000fc00: 6578 7472 612e 7361 6d65 5f66 6f72 5f62  extra.same_for_b
+0000fc10: 6174 6368 5f63 7478 2e69 7465 6d73 2829  atch_ctx.items()
+0000fc20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000fc30: 2020 6966 206e 6f74 2064 696d 2e5f 7661    if not dim._va
+0000fc40: 6c69 6461 7465 5f69 6e5f 6375 7272 656e  lidate_in_curren
+0000fc50: 745f 6772 6170 6828 293a 0a20 2020 2020  t_graph():.     
+0000fc60: 2020 2020 2020 2020 2020 2020 2020 2063                 c
+0000fc70: 6f6e 7469 6e75 650a 2020 2020 2020 2020  ontinue.        
+0000fc80: 2020 2020 2020 2020 7365 6c66 5f64 696d          self_dim
+0000fc90: 203d 2073 656c 662e 5f6d 616b 655f 6578   = self._make_ex
+0000fca0: 7472 6128 292e 7361 6d65 5f66 6f72 5f62  tra().same_for_b
+0000fcb0: 6174 6368 5f63 7478 2e67 6574 286b 6579  atch_ctx.get(key
+0000fcc0: 2c20 4e6f 6e65 290a 2020 2020 2020 2020  , None).        
+0000fcd0: 2020 2020 2020 2020 6966 2073 656c 665f          if self_
+0000fce0: 6469 6d20 616e 6420 2873 656c 665f 6469  dim and (self_di
+0000fcf0: 6d2e 6479 6e5f 7369 7a65 5f65 7874 206f  m.dyn_size_ext o
+0000fd00: 7220 6e6f 7420 6469 6d2e 6479 6e5f 7369  r not dim.dyn_si
+0000fd10: 7a65 5f65 7874 293a 0a20 2020 2020 2020  ze_ext):.       
+0000fd20: 2020 2020 2020 2020 2020 2020 2063 6f6e               con
+0000fd30: 7469 6e75 6520 2023 206b 6565 7020 6f75  tinue  # keep ou
+0000fd40: 7273 0a20 2020 2020 2020 2020 2020 2020  rs.             
+0000fd50: 2020 2069 6620 6e6f 7420 6469 6d2e 6479     if not dim.dy
+0000fd60: 6e5f 7369 7a65 5f65 7874 3a0a 2020 2020  n_size_ext:.    
+0000fd70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fd80: 636f 6e74 696e 7565 2020 2320 756e 6465  continue  # unde
+0000fd90: 6669 6e65 642c 2064 6f20 6e6f 7420 6f76  fined, do not ov
+0000fda0: 6572 7461 6b65 0a20 2020 2020 2020 2020  ertake.         
+0000fdb0: 2020 2020 2020 2073 656c 662e 5f65 7874         self._ext
+0000fdc0: 7261 2e73 616d 655f 666f 725f 6261 7463  ra.same_for_batc
+0000fdd0: 685f 6374 785b 6b65 795d 203d 2064 696d  h_ctx[key] = dim
+0000fde0: 0a20 2020 2020 2020 2020 2020 2023 206e  .            # n
+0000fdf0: 6f69 6e73 7065 6374 696f 6e20 5079 5072  oinspection PyPr
+0000fe00: 6f74 6563 7465 644d 656d 6265 720a 2020  otectedMember.  
+0000fe10: 2020 2020 2020 2020 2020 6f74 6865 722e            other.
+0000fe20: 5f65 7874 7261 2e73 616d 655f 666f 725f  _extra.same_for_
+0000fe30: 6261 7463 685f 6374 782e 636c 6561 7228  batch_ctx.clear(
+0000fe40: 2920 2023 2077 6520 6f6e 6c79 2077 616e  )  # we only wan
+0000fe50: 7420 746f 2068 6176 6520 6974 206f 6e63  t to have it onc
+0000fe60: 650a 0a20 2020 2023 206e 6f69 6e73 7065  e..    # noinspe
+0000fe70: 6374 696f 6e20 5079 5072 6f74 6563 7465  ction PyProtecte
+0000fe80: 644d 656d 6265 720a 2020 2020 6465 6620  dMember.    def 
+0000fe90: 6465 7269 7665 5f66 726f 6d28 7365 6c66  derive_from(self
+0000fea0: 3a20 5f64 2e44 696d 2c20 6261 7365 3a20  : _d.Dim, base: 
+0000feb0: 5f64 2e44 696d 2c20 7365 745f 6465 7269  _d.Dim, set_deri
+0000fec0: 7665 645f 6672 6f6d 5f66 6c61 673a 2062  ved_from_flag: b
+0000fed0: 6f6f 6c20 3d20 5472 7565 293a 0a20 2020  ool = True):.   
+0000fee0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+0000fef0: 203a 7061 7261 6d20 6261 7365 3a20 6469   :param base: di
+0000ff00: 6d0a 2020 2020 2020 2020 3a70 6172 616d  m.        :param
+0000ff10: 2073 6574 5f64 6572 6976 6564 5f66 726f   set_derived_fro
+0000ff20: 6d5f 666c 6167 3a0a 2020 2020 2020 2020  m_flag:.        
+0000ff30: 2222 220a 2020 2020 2020 2020 7365 6c66  """.        self
+0000ff40: 5f62 6173 6520 3d20 7365 6c66 2e67 6574  _base = self.get
+0000ff50: 5f73 616d 655f 6261 7365 2829 0a20 2020  _same_base().   
+0000ff60: 2020 2020 2073 656c 665f 6261 7365 5f65       self_base_e
+0000ff70: 7874 7261 203d 2073 656c 665f 6261 7365  xtra = self_base
+0000ff80: 2e5f 6d61 6b65 5f65 7874 7261 2829 0a20  ._make_extra(). 
+0000ff90: 2020 2020 2020 2069 6620 7365 745f 6465         if set_de
+0000ffa0: 7269 7665 645f 6672 6f6d 5f66 6c61 673a  rived_from_flag:
+0000ffb0: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+0000ffc0: 7365 6c66 5f62 6173 655f 6578 7472 612e  self_base_extra.
+0000ffd0: 6465 7269 7665 645f 6672 6f6d 5f74 6167  derived_from_tag
+0000ffe0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+0000fff0: 2020 6173 7365 7274 2073 656c 665f 6261    assert self_ba
+00010000: 7365 5f65 7874 7261 2e64 6572 6976 6564  se_extra.derived
+00010010: 5f66 726f 6d5f 7461 6720 3d3d 2062 6173  _from_tag == bas
+00010020: 650a 2020 2020 2020 2020 2020 2020 656c  e.            el
+00010030: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
+00010040: 2020 2020 7365 6c66 5f62 6173 655f 6578      self_base_ex
+00010050: 7472 612e 6465 7269 7665 645f 6672 6f6d  tra.derived_from
+00010060: 5f74 6167 203d 2062 6173 650a 2020 2020  _tag = base.    
+00010070: 2020 2020 6966 2073 656c 662e 6973 5f64      if self.is_d
+00010080: 796e 616d 6963 2829 206f 7220 6e6f 7420  ynamic() or not 
+00010090: 7365 6c66 2e69 735f 6469 6d5f 6b6e 6f77  self.is_dim_know
+000100a0: 6e28 293a 0a20 2020 2020 2020 2020 2020  n():.           
+000100b0: 2069 6620 6e6f 7420 7365 6c66 2e62 6174   if not self.bat
+000100c0: 6368 2061 6e64 2062 6173 652e 6261 7463  ch and base.batc
+000100d0: 683a 0a20 2020 2020 2020 2020 2020 2020  h:.             
+000100e0: 2020 2073 656c 662e 6261 7463 6820 3d20     self.batch = 
+000100f0: 6261 7365 2e62 6174 6368 0a20 2020 2020  base.batch.     
+00010100: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010110: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
+00010120: 203d 2062 6173 652e 636f 6e74 726f 6c5f   = base.control_
+00010130: 666c 6f77 5f63 7478 0a20 2020 2020 2020  flow_ctx.       
+00010140: 2020 2020 2020 2020 206b 6579 203d 2062           key = b
+00010150: 6173 652e 6261 7463 682c 2062 6173 652e  ase.batch, base.
+00010160: 636f 6e74 726f 6c5f 666c 6f77 5f63 7478  control_flow_ctx
+00010170: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010180: 2061 7373 6572 7420 6b65 7920 6e6f 7420   assert key not 
+00010190: 696e 2073 656c 665f 6261 7365 5f65 7874  in self_base_ext
+000101a0: 7261 2e73 616d 655f 666f 725f 6261 7463  ra.same_for_batc
+000101b0: 685f 6374 780a 2020 2020 2020 2020 2020  h_ctx.          
+000101c0: 2020 2020 2020 7365 6c66 5f62 6173 655f        self_base_
+000101d0: 6578 7472 612e 7361 6d65 5f66 6f72 5f62  extra.same_for_b
+000101e0: 6174 6368 5f63 7478 5b6b 6579 5d20 3d20  atch_ctx[key] = 
+000101f0: 7365 6c66 0a20 2020 2020 2020 2020 2020  self.           
+00010200: 2069 6620 6e6f 7420 7365 6c66 2e64 796e   if not self.dyn
+00010210: 5f73 697a 655f 6578 743a 0a20 2020 2020  _size_ext:.     
+00010220: 2020 2020 2020 2020 2020 2069 6620 6261             if ba
+00010230: 7365 2e64 796e 5f73 697a 655f 6578 743a  se.dyn_size_ext:
+00010240: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010250: 2020 2020 2069 6620 6261 7365 2e62 6174       if base.bat
+00010260: 6368 2061 6e64 2062 6173 652e 6261 7463  ch and base.batc
+00010270: 6820 3d3d 2073 656c 662e 6261 7463 6820  h == self.batch 
+00010280: 616e 6420 6261 7365 2e63 6f6e 7472 6f6c  and base.control
+00010290: 5f66 6c6f 775f 6374 7820 3d3d 2073 656c  _flow_ctx == sel
+000102a0: 662e 636f 6e74 726f 6c5f 666c 6f77 5f63  f.control_flow_c
+000102b0: 7478 3a0a 2020 2020 2020 2020 2020 2020  tx:.            
+000102c0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+000102d0: 2e64 796e 5f73 697a 655f 6578 7420 3d20  .dyn_size_ext = 
+000102e0: 6261 7365 2e64 796e 5f73 697a 655f 6578  base.dyn_size_ex
+000102f0: 742e 636f 7079 5f74 656d 706c 6174 6528  t.copy_template(
+00010300: 6e61 6d65 3d22 2573 3a73 697a 6522 2025  name="%s:size" %
+00010310: 2073 656c 665f 6261 7365 2e64 6573 6372   self_base.descr
+00010320: 6970 7469 6f6e 290a 2020 2020 2020 2020  iption).        
+00010330: 2020 2020 2020 2020 656c 6966 2062 6173          elif bas
+00010340: 652e 6973 5f62 6174 6368 5f64 696d 2829  e.is_batch_dim()
+00010350: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010360: 2020 2020 2020 7365 6c66 2e64 796e 5f73        self.dyn_s
+00010370: 697a 655f 6578 7420 3d20 5f74 2e54 656e  ize_ext = _t.Ten
+00010380: 736f 7228 0a20 2020 2020 2020 2020 2020  sor(.           
+00010390: 2020 2020 2020 2020 2020 2020 206e 616d               nam
+000103a0: 653d 2225 733a 6261 7463 6822 2025 2073  e="%s:batch" % s
+000103b0: 656c 665f 6261 7365 2e64 6573 6372 6970  elf_base.descrip
+000103c0: 7469 6f6e 2c20 7368 6170 653d 2829 2c20  tion, shape=(), 
+000103d0: 6474 7970 653d 2269 6e74 3332 222c 2062  dtype="int32", b
+000103e0: 6174 6368 5f64 696d 5f61 7869 733d 4e6f  atch_dim_axis=No
+000103f0: 6e65 0a20 2020 2020 2020 2020 2020 2020  ne.             
+00010400: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+00010410: 6620 636f 7079 5f66 726f 6d28 7365 6c66  f copy_from(self
+00010420: 3a20 4469 6d2c 206f 7468 6572 3a20 4469  : Dim, other: Di
+00010430: 6d29 3a0a 2020 2020 2020 2020 2222 2264  m):.        """d
+00010440: 6566 696e 6522 2222 0a20 2020 2020 2020  efine""".       
+00010450: 2073 656c 662e 7369 7a65 203d 206f 7468   self.size = oth
+00010460: 6572 2e73 697a 650a 2020 2020 2020 2020  er.size.        
+00010470: 7365 6c66 2e63 6170 6163 6974 7920 3d20  self.capacity = 
+00010480: 6f74 6865 722e 6361 7061 6369 7479 0a20  other.capacity. 
+00010490: 2020 2020 2020 2073 656c 662e 6479 6e5f         self.dyn_
+000104a0: 7369 7a65 5f65 7874 203d 206f 7468 6572  size_ext = other
+000104b0: 2e64 796e 5f73 697a 655f 6578 740a 2020  .dyn_size_ext.  
+000104c0: 2020 2020 2020 7365 6c66 2e64 6572 6976        self.deriv
+000104d0: 655f 6672 6f6d 286f 7468 6572 290a 0a20  e_from(other).. 
+000104e0: 2020 2040 636c 6173 736d 6574 686f 640a     @classmethod.
+000104f0: 2020 2020 6465 6620 6765 745f 6578 6973      def get_exis
+00010500: 7469 6e67 5f74 6167 5f66 726f 6d5f 636f  ting_tag_from_co
+00010510: 6c6c 6563 7469 6f6e 2863 6c73 2c20 6f74  llection(cls, ot
+00010520: 6865 722c 2074 6167 732c 2069 735f 6571  her, tags, is_eq
+00010530: 7561 6c5f 6f70 7473 3d4e 6f6e 6529 3a0a  ual_opts=None):.
+00010540: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00010550: 2020 2020 3a70 6172 616d 2044 696d 206f      :param Dim o
+00010560: 7468 6572 3a0a 2020 2020 2020 2020 3a70  ther:.        :p
+00010570: 6172 616d 206c 6973 745b 4469 6d5d 7c74  aram list[Dim]|t
+00010580: 7570 6c65 5b44 696d 5d7c 7365 745b 4469  uple[Dim]|set[Di
+00010590: 6d5d 2074 6167 733a 0a20 2020 2020 2020  m] tags:.       
+000105a0: 203a 7061 7261 6d20 6469 6374 5b73 7472   :param dict[str
+000105b0: 5d7c 4e6f 6e65 2069 735f 6571 7561 6c5f  ]|None is_equal_
+000105c0: 6f70 7473 3a20 7061 7373 6564 2074 6f20  opts: passed to 
+000105d0: 4469 6d2e 6973 5f65 7175 616c 0a20 2020  Dim.is_equal.   
+000105e0: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
+000105f0: 7c4e 6f6e 650a 2020 2020 2020 2020 2222  |None.        ""
+00010600: 220a 2020 2020 2020 2020 6966 2069 735f  ".        if is_
+00010610: 6571 7561 6c5f 6f70 7473 2069 7320 4e6f  equal_opts is No
+00010620: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+00010630: 6973 5f65 7175 616c 5f6f 7074 7320 3d20  is_equal_opts = 
+00010640: 7b7d 0a20 2020 2020 2020 2023 2057 6520  {}.        # We 
+00010650: 646f 2070 6f74 656e 7469 616c 206d 756c  do potential mul
+00010660: 7469 706c 6520 726f 756e 6473 2c20 7375  tiple rounds, su
+00010670: 6368 2074 6861 7420 7765 2070 7265 6665  ch that we prefe
+00010680: 7220 226d 6f72 6520 6571 7561 6c22 2028  r "more equal" (
+00010690: 7573 696e 6720 6c65 7373 2069 735f 6571  using less is_eq
+000106a0: 7561 6c5f 6f70 7473 292e 0a20 2020 2020  ual_opts)..     
+000106b0: 2020 2072 6f75 6e64 7320 3d20 5b7b 7d5d     rounds = [{}]
+000106c0: 0a20 2020 2020 2020 2069 6620 6973 5f65  .        if is_e
+000106d0: 7175 616c 5f6f 7074 733a 0a20 2020 2020  qual_opts:.     
+000106e0: 2020 2020 2020 2069 6620 2262 726f 6164         if "broad
+000106f0: 6361 7374 5f6d 6174 6368 6573 2220 696e  cast_matches" in
+00010700: 2069 735f 6571 7561 6c5f 6f70 7473 3a0a   is_equal_opts:.
+00010710: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010720: 726f 756e 6473 2e61 7070 656e 6428 7b6b  rounds.append({k
+00010730: 3a20 7620 666f 7220 286b 2c20 7629 2069  : v for (k, v) i
+00010740: 6e20 6973 5f65 7175 616c 5f6f 7074 732e  n is_equal_opts.
+00010750: 6974 656d 7328 2920 6966 206b 2021 3d20  items() if k != 
+00010760: 2262 726f 6164 6361 7374 5f6d 6174 6368  "broadcast_match
+00010770: 6573 227d 290a 2020 2020 2020 2020 2020  es"}).          
+00010780: 2020 726f 756e 6473 2e61 7070 656e 6428    rounds.append(
+00010790: 6973 5f65 7175 616c 5f6f 7074 7329 0a20  is_equal_opts). 
+000107a0: 2020 2020 2020 2066 6f72 205f 6973 5f65         for _is_e
+000107b0: 7175 616c 5f6f 7074 7320 696e 2072 6f75  qual_opts in rou
+000107c0: 6e64 733a 0a20 2020 2020 2020 2020 2020  nds:.           
+000107d0: 2066 6f72 205f 7461 6720 696e 2074 6167   for _tag in tag
+000107e0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000107f0: 2020 2069 6620 5f74 6167 2e69 735f 6571     if _tag.is_eq
+00010800: 7561 6c28 6f74 6865 722c 202a 2a5f 6973  ual(other, **_is
+00010810: 5f65 7175 616c 5f6f 7074 7329 3a0a 2020  _equal_opts):.  
+00010820: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010830: 2020 7265 7475 726e 205f 7461 670a 2020    return _tag.  
+00010840: 2020 2020 2020 7265 7475 726e 204e 6f6e        return Non
+00010850: 650a 0a20 2020 2040 636c 6173 736d 6574  e..    @classmet
+00010860: 686f 640a 2020 2020 6465 6620 6765 745f  hod.    def get_
+00010870: 616c 6c5f 6469 6d65 6e73 696f 6e5f 7461  all_dimension_ta
+00010880: 6773 2863 6c73 2c20 6461 7461 5f6c 6973  gs(cls, data_lis
+00010890: 742c 2069 735f 6571 7561 6c5f 6f70 7473  t, is_equal_opts
+000108a0: 3d4e 6f6e 652c 2075 6e69 7175 655f 7365  =None, unique_se
+000108b0: 7061 7261 7465 5f61 7865 733d 5472 7565  parate_axes=True
+000108c0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+000108d0: 2020 2020 2020 203a 7061 7261 6d20 6c69         :param li
+000108e0: 7374 5b5f 742e 5465 6e73 6f72 5d20 6461  st[_t.Tensor] da
+000108f0: 7461 5f6c 6973 743a 0a20 2020 2020 2020  ta_list:.       
+00010900: 203a 7061 7261 6d20 6469 6374 5b73 7472   :param dict[str
+00010910: 5d7c 4e6f 6e65 2069 735f 6571 7561 6c5f  ]|None is_equal_
+00010920: 6f70 7473 3a20 7061 7373 6564 2074 6f20  opts: passed to 
+00010930: 4469 6d2e 6973 5f65 7175 616c 0a20 2020  Dim.is_equal.   
+00010940: 2020 2020 203a 7061 7261 6d20 626f 6f6c       :param bool
+00010950: 2075 6e69 7175 655f 7365 7061 7261 7465   unique_separate
+00010960: 5f61 7865 733a 2065 2e67 2e20 6461 7461  _axes: e.g. data
+00010970: 5f6c 6973 743d 5b44 6174 6120 7769 7468  _list=[Data with
+00010980: 2073 6861 7065 2028 422c 352c 352c 3130   shape (B,5,5,10
+00010990: 295d 2072 6573 756c 7473 2069 6e20 3420  )] results in 4 
+000109a0: 6469 6d20 7461 6773 2c20 6e6f 7420 332e  dim tags, not 3.
+000109b0: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+000109c0: 3a20 6c69 7374 206f 6620 6469 6d65 6e73  : list of dimens
+000109d0: 696f 6e20 7461 6773 2c20 6469 6374 2066  ion tags, dict f
+000109e0: 6f72 2064 6174 6120 2d3e 206c 6973 7420  or data -> list 
+000109f0: 6f66 2064 696d 656e 7369 6f6e 2074 6167  of dimension tag
+00010a00: 7320 2866 6f72 2065 6163 6820 6178 6973  s (for each axis
+00010a10: 290a 2020 2020 2020 2020 3a72 7479 7065  ).        :rtype
+00010a20: 3a20 286c 6973 745b 4469 6d5d 2c20 7574  : (list[Dim], ut
+00010a30: 696c 2e44 6963 7452 6566 4b65 7973 5b5f  il.DictRefKeys[_
+00010a40: 742e 5465 6e73 6f72 2c20 6c69 7374 5b44  t.Tensor, list[D
+00010a50: 696d 5d5d 290a 2020 2020 2020 2020 2222  im]]).        ""
+00010a60: 220a 2020 2020 2020 2020 7461 6773 203d  ".        tags =
+00010a70: 205b 5d0a 2020 2020 2020 2020 6461 7461   [].        data
+00010a80: 5f61 7865 735f 6469 6374 203d 2075 7469  _axes_dict = uti
+00010a90: 6c2e 4469 6374 5265 664b 6579 7328 2920  l.DictRefKeys() 
+00010aa0: 2023 2074 7970 653a 2075 7469 6c2e 4469   # type: util.Di
+00010ab0: 6374 5265 664b 6579 735b 5f74 2e54 656e  ctRefKeys[_t.Ten
+00010ac0: 736f 722c 204c 6973 745b 4469 6d5d 5d0a  sor, List[Dim]].
+00010ad0: 2020 2020 2020 2020 666f 7220 6461 7461          for data
+00010ae0: 2069 6e20 6461 7461 5f6c 6973 743a 0a20   in data_list:. 
+00010af0: 2020 2020 2020 2020 2020 2064 6174 615f             data_
+00010b00: 6178 6573 5f64 6963 745b 6461 7461 5d20  axes_dict[data] 
+00010b10: 3d20 5b5d 0a20 2020 2020 2020 2020 2020  = [].           
+00010b20: 2065 7869 7374 696e 675f 7461 675f 636f   existing_tag_co
+00010b30: 6c6c 6563 7469 6f6e 5f66 6f72 5f64 6174  llection_for_dat
+00010b40: 6120 3d20 6c69 7374 2874 6167 7329 2069  a = list(tags) i
+00010b50: 6620 756e 6971 7565 5f73 6570 6172 6174  f unique_separat
+00010b60: 655f 6178 6573 2065 6c73 6520 7461 6773  e_axes else tags
+00010b70: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00010b80: 2061 7869 7320 696e 2072 616e 6765 2864   axis in range(d
+00010b90: 6174 612e 6261 7463 685f 6e64 696d 293a  ata.batch_ndim):
+00010ba0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010bb0: 2074 6167 203d 2064 6174 612e 6765 745f   tag = data.get_
+00010bc0: 6469 6d5f 7461 6728 6178 6973 290a 2020  dim_tag(axis).  
+00010bd0: 2020 2020 2020 2020 2020 2020 2020 6578                ex
+00010be0: 6973 7469 6e67 5f74 6167 203d 2063 6c73  isting_tag = cls
+00010bf0: 2e67 6574 5f65 7869 7374 696e 675f 7461  .get_existing_ta
+00010c00: 675f 6672 6f6d 5f63 6f6c 6c65 6374 696f  g_from_collectio
+00010c10: 6e28 0a20 2020 2020 2020 2020 2020 2020  n(.             
+00010c20: 2020 2020 2020 2074 6167 2c20 7461 6773         tag, tags
+00010c30: 3d65 7869 7374 696e 675f 7461 675f 636f  =existing_tag_co
+00010c40: 6c6c 6563 7469 6f6e 5f66 6f72 5f64 6174  llection_for_dat
+00010c50: 612c 2069 735f 6571 7561 6c5f 6f70 7473  a, is_equal_opts
+00010c60: 3d69 735f 6571 7561 6c5f 6f70 7473 0a20  =is_equal_opts. 
+00010c70: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+00010c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010c90: 2069 6620 6578 6973 7469 6e67 5f74 6167   if existing_tag
+00010ca0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00010cb0: 2020 2020 2020 6966 2075 6e69 7175 655f        if unique_
+00010cc0: 7365 7061 7261 7465 5f61 7865 733a 0a20  separate_axes:. 
+00010cd0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ce0: 2020 2020 2020 2065 7869 7374 696e 675f         existing_
+00010cf0: 7461 675f 636f 6c6c 6563 7469 6f6e 5f66  tag_collection_f
+00010d00: 6f72 5f64 6174 612e 7265 6d6f 7665 2865  or_data.remove(e
+00010d10: 7869 7374 696e 675f 7461 6729 2020 2320  xisting_tag)  # 
+00010d20: 646f 6e27 7420 7461 6b65 2069 7420 6167  don't take it ag
+00010d30: 6169 6e20 666f 7220 7468 6973 2064 6174  ain for this dat
+00010d40: 610a 2020 2020 2020 2020 2020 2020 2020  a.              
+00010d50: 2020 2020 2020 7265 706c 6163 655f 6578        replace_ex
+00010d60: 6973 7469 6e67 203d 2028 0a20 2020 2020  isting = (.     
+00010d70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010d80: 2020 2065 7869 7374 696e 675f 7461 672e     existing_tag.
+00010d90: 756e 6465 6669 6e65 6420 616e 6420 6e6f  undefined and no
+00010da0: 7420 7461 672e 756e 6465 6669 6e65 6420  t tag.undefined 
+00010db0: 616e 6420 7461 672e 6469 6d65 6e73 696f  and tag.dimensio
+00010dc0: 6e20 3d3d 2065 7869 7374 696e 675f 7461  n == existing_ta
+00010dd0: 672e 6469 6d65 6e73 696f 6e0a 2020 2020  g.dimension.    
+00010de0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010df0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
+00010e00: 2020 2020 2020 6966 2072 6570 6c61 6365        if replace
+00010e10: 5f65 7869 7374 696e 673a 2020 2320 5265  _existing:  # Re
+00010e20: 706c 6163 6520 7468 6520 6578 6973 7469  place the existi
+00010e30: 6e67 2062 7920 7468 6520 6e65 7720 7461  ng by the new ta
+00010e40: 672e 0a20 2020 2020 2020 2020 2020 2020  g..             
+00010e50: 2020 2020 2020 2020 2020 2074 6167 735b             tags[
+00010e60: 7461 6773 2e69 6e64 6578 2865 7869 7374  tags.index(exist
+00010e70: 696e 675f 7461 6729 5d20 3d20 7461 670a  ing_tag)] = tag.
+00010e80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010e90: 2020 2020 2020 2020 666f 7220 5f2c 2064          for _, d
+00010ea0: 696d 735f 2069 6e20 6461 7461 5f61 7865  ims_ in data_axe
+00010eb0: 735f 6469 6374 2e69 7465 6d73 2829 3a0a  s_dict.items():.
+00010ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010ed0: 2020 2020 2020 2020 2020 2020 6469 6d73              dims
+00010ee0: 5f5b 3a5d 203d 205b 7461 6720 6966 2064  _[:] = [tag if d
+00010ef0: 203d 3d20 6578 6973 7469 6e67 5f74 6167   == existing_tag
+00010f00: 2065 6c73 6520 6420 666f 7220 6420 696e   else d for d in
+00010f10: 2064 696d 735f 5d0a 2020 2020 2020 2020   dims_].        
+00010f20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f30: 6578 6973 7469 6e67 5f74 6167 203d 2074  existing_tag = t
+00010f40: 6167 0a20 2020 2020 2020 2020 2020 2020  ag.             
+00010f50: 2020 2065 6c73 653a 2020 2320 6e6f 2065     else:  # no e
+00010f60: 7869 7374 696e 6720 7461 670a 2020 2020  xisting tag.    
+00010f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00010f80: 7461 6773 2e61 7070 656e 6428 7461 6729  tags.append(tag)
+00010f90: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010fa0: 2064 6174 615f 6178 6573 5f64 6963 745b   data_axes_dict[
+00010fb0: 6461 7461 5d2e 6170 7065 6e64 2865 7869  data].append(exi
+00010fc0: 7374 696e 675f 7461 6720 6f72 2074 6167  sting_tag or tag
+00010fd0: 290a 2020 2020 2020 2020 7265 7475 726e  ).        return
+00010fe0: 2074 6167 732c 2064 6174 615f 6178 6573   tags, data_axes
+00010ff0: 5f64 6963 740a 0a20 2020 2040 636c 6173  _dict..    @clas
+00011000: 736d 6574 686f 640a 2020 2020 6465 6620  smethod.    def 
+00011010: 6765 745f 756e 6971 5f63 6f6c 6c65 6374  get_uniq_collect
+00011020: 696f 6e28 636c 732c 2074 6167 732c 2069  ion(cls, tags, i
+00011030: 735f 6571 7561 6c5f 6f70 7473 3d4e 6f6e  s_equal_opts=Non
+00011040: 6529 3a0a 2020 2020 2020 2020 2222 220a  e):.        """.
+00011050: 2020 2020 2020 2020 3a70 6172 616d 206c          :param l
+00011060: 6973 745b 4469 6d5d 7c74 7570 6c65 5b44  ist[Dim]|tuple[D
+00011070: 696d 5d7c 7365 745b 4469 6d5d 2074 6167  im]|set[Dim] tag
+00011080: 733a 0a20 2020 2020 2020 203a 7061 7261  s:.        :para
+00011090: 6d20 6469 6374 5b73 7472 5d7c 4e6f 6e65  m dict[str]|None
+000110a0: 2069 735f 6571 7561 6c5f 6f70 7473 3a20   is_equal_opts: 
+000110b0: 7061 7373 6564 2074 6f20 4469 6d2e 6973  passed to Dim.is
+000110c0: 5f65 7175 616c 0a20 2020 2020 2020 203a  _equal.        :
+000110d0: 7274 7970 653a 206c 6973 745b 4469 6d5d  rtype: list[Dim]
+000110e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000110f0: 2020 2020 2072 6573 203d 205b 5d0a 2020       res = [].  
+00011100: 2020 2020 2020 666f 7220 7461 6720 696e        for tag in
+00011110: 2074 6167 733a 0a20 2020 2020 2020 2020   tags:.         
+00011120: 2020 2065 7820 3d20 636c 732e 6765 745f     ex = cls.get_
+00011130: 6578 6973 7469 6e67 5f74 6167 5f66 726f  existing_tag_fro
+00011140: 6d5f 636f 6c6c 6563 7469 6f6e 2874 6167  m_collection(tag
+00011150: 2c20 7265 732c 2069 735f 6571 7561 6c5f  , res, is_equal_
+00011160: 6f70 7473 3d69 735f 6571 7561 6c5f 6f70  opts=is_equal_op
+00011170: 7473 290a 2020 2020 2020 2020 2020 2020  ts).            
+00011180: 6966 206e 6f74 2065 783a 0a20 2020 2020  if not ex:.     
+00011190: 2020 2020 2020 2020 2020 2072 6573 2e61             res.a
+000111a0: 7070 656e 6428 7461 6729 0a20 2020 2020  ppend(tag).     
+000111b0: 2020 2072 6574 7572 6e20 7265 730a 0a20     return res.. 
+000111c0: 2020 2064 6566 2067 6574 5f73 697a 655f     def get_size_
+000111d0: 7465 6e73 6f72 2873 656c 6629 202d 3e20  tensor(self) -> 
+000111e0: 5f74 2e54 656e 736f 723a 0a20 2020 2020  _t.Tensor:.     
+000111f0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00011200: 7265 7475 726e 3a20 7369 7a65 2074 656e  return: size ten
+00011210: 736f 722c 206f 7220 6479 6e5f 7369 7a65  sor, or dyn_size
+00011220: 5f65 7874 2069 6620 6465 6669 6e65 640a  _ext if defined.
+00011230: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00011240: 5f74 2e54 656e 736f 720a 2020 2020 2020  _t.Tensor.      
+00011250: 2020 2222 220a 2020 2020 2020 2020 6966    """.        if
+00011260: 2073 656c 662e 6479 6e5f 7369 7a65 5f65   self.dyn_size_e
+00011270: 7874 3a0a 2020 2020 2020 2020 2020 2020  xt:.            
+00011280: 7265 7475 726e 2073 656c 662e 6479 6e5f  return self.dyn_
+00011290: 7369 7a65 5f65 7874 0a0a 2020 2020 2020  size_ext..      
+000112a0: 2020 696d 706f 7274 2072 6574 7572 6e6e    import returnn
+000112b0: 2e66 726f 6e74 656e 6420 6173 2072 660a  .frontend as rf.
+000112c0: 0a20 2020 2020 2020 2061 7373 6572 7420  .        assert 
+000112d0: 7365 6c66 2e73 697a 6520 6973 206e 6f74  self.size is not
+000112e0: 204e 6f6e 650a 2020 2020 2020 2020 7265   None.        re
+000112f0: 7475 726e 2072 662e 636f 6e76 6572 745f  turn rf.convert_
+00011300: 746f 5f74 656e 736f 7228 7365 6c66 2e73  to_tensor(self.s
+00011310: 697a 652c 206e 616d 653d 2225 733a 7369  ize, name="%s:si
+00011320: 7a65 2220 2520 7365 6c66 2e64 6573 6372  ze" % self.descr
+00011330: 6970 7469 6f6e 290a 0a20 2020 2064 6566  iption)..    def
+00011340: 2067 6574 5f64 696d 5f76 616c 7565 2873   get_dim_value(s
+00011350: 656c 6629 202d 3e20 556e 696f 6e5b 696e  elf) -> Union[in
+00011360: 742c 205f 742e 5261 7754 656e 736f 7254  t, _t.RawTensorT
+00011370: 7970 655d 3a0a 2020 2020 2020 2020 2222  ype]:.        ""
+00011380: 220a 2020 2020 2020 2020 496e 6665 7273  ".        Infers
+00011390: 2074 6865 2064 696d 2074 6869 7320 6178   the dim this ax
+000113a0: 6973 2073 686f 756c 6420 6861 7665 2069  is should have i
+000113b0: 6620 756e 6272 6f61 6463 6173 7465 642e  f unbroadcasted.
+000113c0: 0a20 2020 2020 2020 2049 6620 6073 656c  .        If `sel
+000113d0: 662e 7372 635f 6461 7461 6020 6861 7320  f.src_data` has 
+000113e0: 6120 706c 6163 6568 6f6c 6465 722c 2077  a placeholder, w
+000113f0: 696c 6c20 7573 6520 7468 6520 7368 6170  ill use the shap
+00011400: 6520 6672 6f6d 2074 6865 7265 2e0a 2020  e from there..  
+00011410: 2020 2020 2020 4f74 6865 7277 6973 652c        Otherwise,
+00011420: 2075 7365 7320 6073 656c 662e 6469 6d65   uses `self.dime
+00011430: 6e73 696f 6e60 2028 6966 2073 7461 7469  nsion` (if stati
+00011440: 6329 206f 7220 6073 656c 662e 6479 6e5f  c) or `self.dyn_
+00011450: 7369 7a65 6020 2869 6620 6479 6e61 6d69  size` (if dynami
+00011460: 6329 2e0a 0a20 2020 2020 2020 203a 7265  c)...        :re
+00011470: 7475 726e 3a20 6d61 7828 7369 7a65 206f  turn: max(size o
+00011480: 7220 6479 6e5f 7369 7a65 290a 2020 2020  r dyn_size).    
+00011490: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+000114a0: 7265 7320 3d20 7365 6c66 2e67 6574 5f64  res = self.get_d
+000114b0: 696d 5f76 616c 7565 5f74 656e 736f 7228  im_value_tensor(
+000114c0: 290a 2020 2020 2020 2020 6966 2069 7369  ).        if isi
+000114d0: 6e73 7461 6e63 6528 7265 732c 205f 742e  nstance(res, _t.
+000114e0: 5465 6e73 6f72 293a 0a20 2020 2020 2020  Tensor):.       
+000114f0: 2020 2020 2061 7373 6572 7420 7265 732e       assert res.
+00011500: 6469 6d73 203d 3d20 2829 0a20 2020 2020  dims == ().     
+00011510: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00011520: 732e 7261 775f 7465 6e73 6f72 0a20 2020  s.raw_tensor.   
+00011530: 2020 2020 2061 7373 6572 7420 6973 696e       assert isin
+00011540: 7374 616e 6365 2872 6573 2c20 696e 7429  stance(res, int)
+00011550: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00011560: 7265 730a 0a20 2020 2064 6566 2067 6574  res..    def get
+00011570: 5f64 696d 5f76 616c 7565 5f74 656e 736f  _dim_value_tenso
+00011580: 7228 7365 6c66 2920 2d3e 2055 6e69 6f6e  r(self) -> Union
+00011590: 5b69 6e74 2c20 5f74 2e54 656e 736f 725d  [int, _t.Tensor]
+000115a0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000115b0: 2020 2020 2020 496e 6665 7273 2074 6865        Infers the
+000115c0: 2064 696d 2074 6869 7320 6178 6973 2073   dim this axis s
+000115d0: 686f 756c 6420 6861 7665 2069 6620 756e  hould have if un
+000115e0: 6272 6f61 6463 6173 7465 642e 0a20 2020  broadcasted..   
+000115f0: 2020 2020 2049 6620 6073 656c 662e 7372       If `self.sr
+00011600: 635f 6461 7461 6020 6861 7320 6120 706c  c_data` has a pl
+00011610: 6163 6568 6f6c 6465 722c 2077 696c 6c20  aceholder, will 
+00011620: 7573 6520 7468 6520 7368 6170 6520 6672  use the shape fr
+00011630: 6f6d 2074 6865 7265 2e0a 2020 2020 2020  om there..      
+00011640: 2020 4f74 6865 7277 6973 652c 2075 7365    Otherwise, use
+00011650: 7320 6073 656c 662e 6469 6d65 6e73 696f  s `self.dimensio
+00011660: 6e60 2028 6966 2073 7461 7469 6329 206f  n` (if static) o
+00011670: 7220 6073 656c 662e 6479 6e5f 7369 7a65  r `self.dyn_size
+00011680: 6020 2869 6620 6479 6e61 6d69 6329 2e0a  ` (if dynamic)..
+00011690: 0a20 2020 2020 2020 203a 7265 7475 726e  .        :return
+000116a0: 3a20 6d61 7828 7369 7a65 206f 7220 6479  : max(size or dy
+000116b0: 6e5f 7369 7a65 290a 2020 2020 2020 2020  n_size).        
+000116c0: 2222 220a 2020 2020 2020 2020 696d 706f  """.        impo
+000116d0: 7274 2072 6574 7572 6e6e 2e66 726f 6e74  rt returnn.front
+000116e0: 656e 6420 6173 2072 660a 0a20 2020 2020  end as rf..     
+000116f0: 2020 2069 6620 7365 6c66 2e64 696d 656e     if self.dimen
+00011700: 7369 6f6e 2069 7320 6e6f 7420 4e6f 6e65  sion is not None
+00011710: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+00011720: 7475 726e 2073 656c 662e 6469 6d65 6e73  turn self.dimens
+00011730: 696f 6e0a 2020 2020 2020 2020 6966 2073  ion.        if s
+00011740: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+00011750: 2061 6e64 2073 656c 662e 6479 6e5f 7369   and self.dyn_si
+00011760: 7a65 5f65 7874 2e70 6c61 6365 686f 6c64  ze_ext.placehold
+00011770: 6572 2069 7320 6e6f 7420 4e6f 6e65 3a20  er is not None: 
+00011780: 2023 2066 6173 7420 7061 7468 0a20 2020   # fast path.   
+00011790: 2020 2020 2020 2020 2069 6620 7365 6c66           if self
+000117a0: 2e64 796e 5f73 697a 655f 6578 742e 6261  .dyn_size_ext.ba
+000117b0: 7463 685f 6e64 696d 203e 2030 3a0a 2020  tch_ndim > 0:.  
+000117c0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+000117d0: 7475 726e 2072 662e 7265 6475 6365 5f6d  turn rf.reduce_m
+000117e0: 6178 280a 2020 2020 2020 2020 2020 2020  ax(.            
+000117f0: 2020 2020 2020 2020 7365 6c66 2e64 796e          self.dyn
+00011800: 5f73 697a 655f 6578 742c 0a20 2020 2020  _size_ext,.     
+00011810: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00011820: 7869 733d 7365 6c66 2e64 796e 5f73 697a  xis=self.dyn_siz
+00011830: 655f 6578 742e 6469 6d5f 7461 6773 2c0a  e_ext.dim_tags,.
+00011840: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011850: 2020 2020 2320 4d61 736b 696e 6720 6973      # Masking is
+00011860: 206e 6f74 2061 6c77 6179 7320 706f 7373   not always poss
+00011870: 6962 6c65 2068 6572 652c 2065 2e67 2e0a  ible here, e.g..
+00011880: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011890: 2020 2020 2320 7365 6c66 203d 2044 696d      # self = Dim
+000118a0: 7b27 7365 6c66 2d61 7474 2d6b 6579 7327  {'self-att-keys'
+000118b0: 5b27 7469 6d65 3a76 6172 3a65 7874 6572  ['time:var:exter
+000118c0: 6e5f 6461 7461 3a63 6c61 7373 6573 275b  n_data:classes'[
+000118d0: 425d 5d7d 2e0a 2020 2020 2020 2020 2020  B]]}..          
+000118e0: 2020 2020 2020 2020 2020 7573 655f 6d61            use_ma
+000118f0: 736b 3d46 616c 7365 2c0a 2020 2020 2020  sk=False,.      
+00011900: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00011910: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00011920: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+00011930: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00011940: 2e69 735f 6261 7463 685f 6469 6d28 293a  .is_batch_dim():
+00011950: 0a20 2020 2020 2020 2020 2020 2072 6573  .            res
+00011960: 203d 204e 6f6e 650a 2020 2020 2020 2020   = None.        
+00011970: 2020 2020 6966 2073 656c 662e 5f65 7874      if self._ext
+00011980: 7261 2061 6e64 2073 656c 662e 5f65 7874  ra and self._ext
+00011990: 7261 2e73 7263 5f64 6174 613a 0a20 2020  ra.src_data:.   
+000119a0: 2020 2020 2020 2020 2020 2020 2072 6573               res
+000119b0: 203d 2073 656c 662e 5f65 7874 7261 2e73   = self._extra.s
+000119c0: 7263 5f64 6174 612e 6765 745f 6261 7463  rc_data.get_batc
+000119d0: 685f 6469 6d28 290a 2020 2020 2020 2020  h_dim().        
+000119e0: 2020 2020 656c 6966 2073 656c 662e 6261      elif self.ba
+000119f0: 7463 683a 0a20 2020 2020 2020 2020 2020  tch:.           
+00011a00: 2020 2020 2072 6573 203d 2073 656c 662e       res = self.
+00011a10: 6261 7463 682e 6469 6d0a 2020 2020 2020  batch.dim.      
+00011a20: 2020 2020 2020 6966 2069 7369 6e73 7461        if isinsta
+00011a30: 6e63 6528 7265 732c 2069 6e74 293a 0a20  nce(res, int):. 
+00011a40: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+00011a50: 6574 7572 6e20 7265 730a 2020 2020 2020  eturn res.      
+00011a60: 2020 2020 2020 6966 2072 6573 2069 7320        if res is 
+00011a70: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+00011a80: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00011a90: 205f 742e 5465 6e73 6f72 2822 6261 7463   _t.Tensor("batc
+00011aa0: 6822 2c20 6469 6d73 3d28 292c 2064 7479  h", dims=(), dty
+00011ab0: 7065 3d72 662e 6765 745f 6465 6661 756c  pe=rf.get_defaul
+00011ac0: 745f 6172 7261 795f 696e 6465 785f 6474  t_array_index_dt
+00011ad0: 7970 6528 292c 2072 6177 5f74 656e 736f  ype(), raw_tenso
+00011ae0: 723d 7265 7329 0a20 2020 2020 2020 2069  r=res).        i
+00011af0: 6620 280a 2020 2020 2020 2020 2020 2020  f (.            
+00011b00: 7365 6c66 2e5f 6578 7472 610a 2020 2020  self._extra.    
+00011b10: 2020 2020 2020 2020 616e 6420 7365 6c66          and self
+00011b20: 2e5f 6578 7472 612e 7372 635f 6461 7461  ._extra.src_data
+00011b30: 2069 7320 6e6f 7420 4e6f 6e65 0a20 2020   is not None.   
+00011b40: 2020 2020 2020 2020 2061 6e64 2073 656c           and sel
+00011b50: 662e 5f65 7874 7261 2e73 7263 5f61 7869  f._extra.src_axi
+00011b60: 7320 6973 206e 6f74 204e 6f6e 650a 2020  s is not None.  
+00011b70: 2020 2020 2020 2020 2020 616e 6420 7365            and se
+00011b80: 6c66 2e5f 6578 7472 612e 7372 635f 6461  lf._extra.src_da
+00011b90: 7461 2e70 6c61 6365 686f 6c64 6572 2069  ta.placeholder i
+00011ba0: 7320 6e6f 7420 4e6f 6e65 0a20 2020 2020  s not None.     
+00011bb0: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00011bc0: 2020 7265 7320 3d20 7365 6c66 2e5f 6578    res = self._ex
+00011bd0: 7472 612e 7372 635f 6461 7461 2e67 6574  tra.src_data.get
+00011be0: 5f64 696d 2873 656c 662e 5f65 7874 7261  _dim(self._extra
+00011bf0: 2e73 7263 5f61 7869 7329 0a20 2020 2020  .src_axis).     
+00011c00: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00011c10: 616e 6365 2872 6573 2c20 696e 7429 3a0a  ance(res, int):.
+00011c20: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011c30: 7265 7475 726e 2072 6573 0a20 2020 2020  return res.     
+00011c40: 2020 2020 2020 2072 6574 7572 6e20 5f74         return _t
+00011c50: 2e54 656e 736f 7228 2262 6174 6368 222c  .Tensor("batch",
+00011c60: 2064 696d 733d 2829 2c20 6474 7970 653d   dims=(), dtype=
+00011c70: 7266 2e67 6574 5f64 6566 6175 6c74 5f61  rf.get_default_a
+00011c80: 7272 6179 5f69 6e64 6578 5f64 7479 7065  rray_index_dtype
+00011c90: 2829 2c20 7261 775f 7465 6e73 6f72 3d72  (), raw_tensor=r
+00011ca0: 6573 290a 2020 2020 2020 2020 7365 6c66  es).        self
+00011cb0: 2e63 6f6d 706c 6574 655f 6479 6e5f 7369  .complete_dyn_si
+00011cc0: 7a65 2829 0a20 2020 2020 2020 2069 6620  ze().        if 
+00011cd0: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+00011ce0: 7420 616e 6420 7365 6c66 2e64 796e 5f73  t and self.dyn_s
+00011cf0: 697a 655f 6578 742e 706c 6163 6568 6f6c  ize_ext.placehol
+00011d00: 6465 7220 6973 206e 6f74 204e 6f6e 653a  der is not None:
+00011d10: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
+00011d20: 7365 6c66 2e64 796e 5f73 697a 655f 6578  self.dyn_size_ex
+00011d30: 742e 6261 7463 685f 6e64 696d 203e 2030  t.batch_ndim > 0
+00011d40: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011d50: 2020 7265 7475 726e 2072 662e 7265 6475    return rf.redu
+00011d60: 6365 5f6d 6178 2873 656c 662e 6479 6e5f  ce_max(self.dyn_
+00011d70: 7369 7a65 5f65 7874 2c20 6178 6973 3d73  size_ext, axis=s
+00011d80: 656c 662e 6479 6e5f 7369 7a65 5f65 7874  elf.dyn_size_ext
+00011d90: 2e64 696d 5f74 6167 7329 0a20 2020 2020  .dim_tags).     
+00011da0: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00011db0: 6c66 2e64 796e 5f73 697a 655f 6578 740a  lf.dyn_size_ext.
+00011dc0: 2020 2020 2020 2020 7261 6973 6520 4578          raise Ex
+00011dd0: 6365 7074 696f 6e28 2225 733a 206e 6565  ception("%s: nee
+00011de0: 6420 706c 6163 6568 6f6c 6465 722c 2073  d placeholder, s
+00011df0: 656c 662e 6469 6d65 6e73 696f 6e20 6f72  elf.dimension or
+00011e00: 2073 656c 662e 6479 6e5f 7369 7a65 2066   self.dyn_size f
+00011e10: 6f72 2064 696d 2076 616c 7565 2220 2520  or dim value" % 
+00011e20: 7365 6c66 290a 0a20 2020 2064 6566 2061  self)..    def a
+00011e30: 7869 735f 7370 6c69 745f 696e 666f 2873  xis_split_info(s
+00011e40: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00011e50: 220a 2020 2020 2020 2020 3a72 6574 7572  ".        :retur
+00011e60: 6e3a 2061 7869 7320 7370 6c69 7420 696e  n: axis split in
+00011e70: 666f 2e20 7365 6520 3a66 756e 633a 6067  fo. see :func:`g
+00011e80: 6574 5f70 6172 616d 5f61 7865 735f 7370  et_param_axes_sp
+00011e90: 6c69 745f 696e 666f 6020 616e 6420 7573  lit_info` and us
+00011ea0: 6167 6520 2865 2e67 2e20 7072 6574 7261  age (e.g. pretra
+00011eb0: 696e 696e 6729 0a20 2020 2020 2020 203a  ining).        :
+00011ec0: 7274 7970 653a 206c 6973 745b 696e 747c  rtype: list[int|
+00011ed0: 4e6f 6e65 5d0a 2020 2020 2020 2020 2222  None].        ""
+00011ee0: 220a 2020 2020 2020 2020 7361 6d65 5f62  ".        same_b
+00011ef0: 6173 6520 3d20 7365 6c66 2e67 6574 5f73  ase = self.get_s
+00011f00: 616d 655f 6261 7365 2829 0a20 2020 2020  ame_base().     
+00011f10: 2020 206f 7020 3d20 7365 6c66 2e64 6572     op = self.der
+00011f20: 6976 6564 5f66 726f 6d5f 6f70 206f 7220  ived_from_op or 
+00011f30: 7361 6d65 5f62 6173 652e 6465 7269 7665  same_base.derive
+00011f40: 645f 6672 6f6d 5f6f 700a 2020 2020 2020  d_from_op.      
+00011f50: 2020 6966 206e 6f74 206f 703a 0a20 2020    if not op:.   
+00011f60: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00011f70: 5b73 656c 662e 6469 6d65 6e73 696f 6e5d  [self.dimension]
+00011f80: 0a20 2020 2020 2020 2069 6620 6f70 2e6b  .        if op.k
+00011f90: 696e 6420 3d3d 2022 6164 6422 3a0a 2020  ind == "add":.  
+00011fa0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00011fb0: 2073 756d 285b 782e 6178 6973 5f73 706c   sum([x.axis_spl
+00011fc0: 6974 5f69 6e66 6f28 2920 666f 7220 7820  it_info() for x 
+00011fd0: 696e 206f 702e 696e 7075 7473 5d2c 205b  in op.inputs], [
+00011fe0: 5d29 2020 2320 666c 6174 7465 6e0a 2020  ])  # flatten.  
+00011ff0: 2020 2020 2020 6966 206f 702e 6b69 6e64        if op.kind
+00012000: 203d 3d20 226d 756c 223a 0a20 2020 2020   == "mul":.     
+00012010: 2020 2020 2020 2072 6573 203d 205b 315d         res = [1]
+00012020: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00012030: 2078 2069 6e20 6f70 2e69 6e70 7574 733a   x in op.inputs:
+00012040: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012050: 2072 6573 203d 2073 756d 285b 6e20 2a20   res = sum([n * 
+00012060: 782e 6178 6973 5f73 706c 6974 5f69 6e66  x.axis_split_inf
+00012070: 6f28 2920 6966 206e 2069 7320 6e6f 7420  o() if n is not 
+00012080: 4e6f 6e65 2065 6c73 6520 4e6f 6e65 2066  None else None f
+00012090: 6f72 206e 2069 6e20 7265 735d 2c20 5b5d  or n in res], []
+000120a0: 2920 2023 2066 6c61 7474 656e 0a20 2020  )  # flatten.   
+000120b0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+000120c0: 7265 730a 2020 2020 2020 2020 7265 7475  res.        retu
+000120d0: 726e 205b 7365 6c66 2e64 696d 656e 7369  rn [self.dimensi
+000120e0: 6f6e 5d0a 0a20 2020 2064 6566 205f 6765  on]..    def _ge
+000120f0: 745f 7361 6d65 5f62 6173 655f 6578 7472  t_same_base_extr
+00012100: 6128 7365 6c66 2920 2d3e 204f 7074 696f  a(self) -> Optio
+00012110: 6e61 6c5b 5f44 696d 4578 7472 615d 3a0a  nal[_DimExtra]:.
+00012120: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+00012130: 656c 662e 5f65 7874 7261 3a0a 2020 2020  elf._extra:.    
+00012140: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00012150: 6f6e 650a 2020 2020 2020 2020 6261 7365  one.        base
+00012160: 203d 2073 656c 662e 6765 745f 7361 6d65   = self.get_same
+00012170: 5f62 6173 6528 290a 2020 2020 2020 2020  _base().        
+00012180: 2320 6e6f 696e 7370 6563 7469 6f6e 2050  # noinspection P
+00012190: 7950 726f 7465 6374 6564 4d65 6d62 6572  yProtectedMember
+000121a0: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000121b0: 6261 7365 2e5f 6578 7472 610a 0a20 2020  base._extra..   
+000121c0: 2064 6566 205f 6d61 6b65 5f65 7874 7261   def _make_extra
+000121d0: 2873 656c 663a 205f 642e 4469 6d29 202d  (self: _d.Dim) -
+000121e0: 3e20 5f44 696d 4578 7472 613a 0a20 2020  > _DimExtra:.   
+000121f0: 2020 2020 2069 6620 6e6f 7420 7365 6c66       if not self
+00012200: 2e5f 6578 7472 613a 0a20 2020 2020 2020  ._extra:.       
+00012210: 2020 2020 2073 656c 662e 5f65 7874 7261       self._extra
+00012220: 203d 205f 4469 6d45 7874 7261 2864 696d   = _DimExtra(dim
+00012230: 3d73 656c 6629 0a20 2020 2020 2020 2072  =self).        r
+00012240: 6574 7572 6e20 7365 6c66 2e5f 6578 7472  eturn self._extr
+00012250: 610a 0a20 2020 2040 7072 6f70 6572 7479  a..    @property
+00012260: 0a20 2020 2064 6566 2076 6f63 6162 2873  .    def vocab(s
+00012270: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+00012280: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
+00012290: 3a20 7265 7475 726e 6e2e 6461 7461 7365  : returnn.datase
+000122a0: 7473 2e75 7469 6c2e 766f 6361 6275 6c61  ts.util.vocabula
+000122b0: 7279 2e56 6f63 6162 756c 6172 797c 4e6f  ry.Vocabulary|No
+000122c0: 6e65 0a20 2020 2020 2020 2022 2222 0a20  ne.        """. 
+000122d0: 2020 2020 2020 2065 7874 7261 203d 2073         extra = s
+000122e0: 656c 662e 5f67 6574 5f73 616d 655f 6261  elf._get_same_ba
+000122f0: 7365 5f65 7874 7261 2829 0a20 2020 2020  se_extra().     
+00012300: 2020 2069 6620 6578 7472 613a 0a20 2020     if extra:.   
+00012310: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00012320: 6578 7472 612e 766f 6361 620a 2020 2020  extra.vocab.    
+00012330: 2020 2020 7265 7475 726e 204e 6f6e 650a      return None.
+00012340: 0a20 2020 2040 766f 6361 622e 7365 7474  .    @vocab.sett
+00012350: 6572 0a20 2020 2064 6566 2076 6f63 6162  er.    def vocab
+00012360: 2873 656c 662c 2076 6f63 6162 293a 0a20  (self, vocab):. 
+00012370: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012380: 2020 203a 7061 7261 6d20 7265 7475 726e     :param return
+00012390: 6e2e 6461 7461 7365 7473 2e75 7469 6c2e  n.datasets.util.
+000123a0: 766f 6361 6275 6c61 7279 2e56 6f63 6162  vocabulary.Vocab
+000123b0: 756c 6172 797c 4e6f 6e65 2076 6f63 6162  ulary|None vocab
+000123c0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000123d0: 2020 2020 2020 6966 2076 6f63 6162 2069        if vocab i
+000123e0: 7320 7365 6c66 2e76 6f63 6162 3a0a 2020  s self.vocab:.  
+000123f0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00012400: 0a20 2020 2020 2020 2069 6620 7365 6c66  .        if self
+00012410: 2e73 616d 655f 6173 3a0a 2020 2020 2020  .same_as:.      
+00012420: 2020 2020 2020 7365 6c66 2e67 6574 5f73        self.get_s
+00012430: 616d 655f 6261 7365 2829 2e76 6f63 6162  ame_base().vocab
+00012440: 203d 2076 6f63 6162 0a20 2020 2020 2020   = vocab.       
+00012450: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00012460: 2020 2020 6578 7472 6120 3d20 7365 6c66      extra = self
+00012470: 2e5f 6765 745f 7361 6d65 5f62 6173 655f  ._get_same_base_
+00012480: 6578 7472 6128 290a 2020 2020 2020 2020  extra().        
+00012490: 6966 2065 7874 7261 3a0a 2020 2020 2020  if extra:.      
+000124a0: 2020 2020 2020 6578 7472 612e 766f 6361        extra.voca
+000124b0: 6220 3d20 766f 6361 620a 0a20 2020 2023  b = vocab..    #
+000124c0: 2054 6865 206b 696e 6420 6f66 206f 7065   The kind of ope
+000124d0: 7261 7469 6f6e 7320 7765 2068 6176 653a  rations we have:
+000124e0: 0a20 2020 2023 2061 202b 2062 3a20 7061  .    # a + b: pa
+000124f0: 6464 696e 672c 2063 6f6e 6361 740a 2020  dding, concat.  
+00012500: 2020 2320 6120 2d20 623a 2077 696e 646f    # a - b: windo
+00012510: 7720 7769 7468 2076 616c 6964 2066 7261  w with valid fra
+00012520: 6d65 7320 6f6e 6c79 0a20 2020 2023 2061  mes only.    # a
+00012530: 202a 2062 3a20 6d65 7267 6520 6469 6d73   * b: merge dims
+00012540: 2c20 7570 7361 6d70 6c65 2c20 7472 616e  , upsample, tran
+00012550: 7370 6f73 6564 2063 6f6e 7620 7769 7468  sposed conv with
+00012560: 2073 7472 6964 696e 670a 2020 2020 2320   striding.    # 
+00012570: 6120 2f20 6220 2877 6865 6e20 6120 2520  a / b (when a % 
+00012580: 6220 3d3d 2030 293a 2073 706c 6974 2064  b == 0): split d
+00012590: 696d 732c 2064 6f77 6e73 616d 706c 652c  ims, downsample,
+000125a0: 2063 6f6e 7620 7769 7468 2073 7472 6964   conv with strid
+000125b0: 696e 670a 2020 2020 2320 6365 696c 6469  ing.    # ceildi
+000125c0: 7628 612c 2062 293a 2063 6f6e 7620 7769  v(a, b): conv wi
+000125d0: 7468 2073 7472 6964 696e 670a 2020 2020  th striding.    
+000125e0: 2320 6375 7374 6f6d 3a20 7265 7065 6174  # custom: repeat
+000125f0: 2c20 7265 6d6f 7665 2c20 6d61 736b 2c20  , remove, mask, 
+00012600: 6c6f 6f70 2077 6974 6820 6479 6e20 656e  loop with dyn en
+00012610: 640a 2020 2020 2320 4e6f 7465 2074 6861  d.    # Note tha
+00012620: 7420 7765 2064 6966 6665 7265 6e74 6961  t we differentia
+00012630: 7465 2062 6574 7765 656e 2074 6865 206f  te between the o
+00012640: 7264 6572 2c20 692e 652e 2061 202b 2062  rder, i.e. a + b
+00012650: 2021 3d20 6220 2b20 612e 0a20 2020 2023   != b + a..    #
+00012660: 204e 6f74 6520 7468 6174 2077 6520 616c   Note that we al
+00012670: 7761 7973 2068 6176 6520 7468 6520 6173  ways have the as
+00012680: 7375 6d70 7469 6f6e 2074 6861 7420 6120  sumption that a 
+00012690: 6469 6d65 6e73 696f 6e20 6973 206e 6f6e  dimension is non
+000126a0: 2d6e 6567 6174 6976 652e 0a20 2020 2023  -negative..    #
+000126b0: 2054 6869 7320 6173 7375 6d70 7469 6f6e   This assumption
+000126c0: 2069 7320 6e65 6365 7373 6172 7920 666f   is necessary fo
+000126d0: 7220 736f 6d65 2073 696d 706c 6966 6963  r some simplific
+000126e0: 6174 696f 6e73 2e0a 2020 2020 2320 6874  ations..    # ht
+000126f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
+00012700: 2f72 7774 682d 6936 2f72 6574 7572 6e6e  /rwth-i6/returnn
+00012710: 2f70 756c 6c2f 3835 330a 0a20 2020 2064  /pull/853..    d
+00012720: 6566 205f 5f61 6464 5f5f 2873 656c 663a  ef __add__(self:
+00012730: 2044 696d 2c20 6f74 6865 7229 3a0a 2020   Dim, other):.  
+00012740: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00012750: 2020 3a70 6172 616d 2044 696d 7c69 6e74    :param Dim|int
+00012760: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
+00012770: 3a72 6574 7572 6e3a 2073 656c 6620 2b20  :return: self + 
+00012780: 6f74 6865 722e 206e 6f74 6520 7468 6174  other. note that
+00012790: 2074 6869 7320 6973 206e 6f74 2063 6f6d   this is not com
+000127a0: 6d75 7461 7469 7665 2c20 692e 652e 2064  mutative, i.e. d
+000127b0: 6966 6665 7265 6e74 2066 726f 6d20 6f74  ifferent from ot
+000127c0: 6865 7220 2b20 7365 6c66 2e0a 2020 2020  her + self..    
+000127d0: 2020 2020 3a72 7479 7065 3a20 4469 6d0a      :rtype: Dim.
+000127e0: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+000127f0: 2020 2020 7465 726d 203d 205f 4f70 4c69      term = _OpLi
+00012800: 6e65 6172 5465 726d 2e66 726f 6d5f 6469  nearTerm.from_di
+00012810: 6d28 7365 6c66 290a 2020 2020 2020 2020  m(self).        
+00012820: 7465 726d 2e65 7874 656e 645f 6164 645f  term.extend_add_
+00012830: 7375 625f 286f 7468 6572 2c20 6b69 6e64  sub_(other, kind
+00012840: 3d22 6164 6422 2c20 7269 6768 743d 5472  ="add", right=Tr
+00012850: 7565 290a 2020 2020 2020 2020 7265 7475  ue).        retu
+00012860: 726e 2074 6572 6d2e 6173 5f64 696d 2829  rn term.as_dim()
+00012870: 0a0a 2020 2020 6465 6620 5f5f 7261 6464  ..    def __radd
+00012880: 5f5f 2873 656c 663a 2044 696d 2c20 6f74  __(self: Dim, ot
+00012890: 6865 7229 3a0a 2020 2020 2020 2020 2222  her):.        ""
+000128a0: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+000128b0: 2044 696d 7c69 6e74 206f 7468 6572 3a0a   Dim|int other:.
+000128c0: 2020 2020 2020 2020 3a72 6574 7572 6e3a          :return:
+000128d0: 206f 7468 6572 202b 2073 656c 660a 2020   other + self.  
+000128e0: 2020 2020 2020 3a72 7479 7065 3a20 4469        :rtype: Di
+000128f0: 6d0a 2020 2020 2020 2020 2222 220a 2020  m.        """.  
+00012900: 2020 2020 2020 7465 726d 203d 205f 4f70        term = _Op
+00012910: 4c69 6e65 6172 5465 726d 2e66 726f 6d5f  LinearTerm.from_
+00012920: 6469 6d28 7365 6c66 290a 2020 2020 2020  dim(self).      
+00012930: 2020 7465 726d 2e65 7874 656e 645f 6164    term.extend_ad
+00012940: 645f 7375 625f 286f 7468 6572 2c20 6b69  d_sub_(other, ki
+00012950: 6e64 3d22 6164 6422 2c20 7269 6768 743d  nd="add", right=
+00012960: 4661 6c73 6529 0a20 2020 2020 2020 2072  False).        r
+00012970: 6574 7572 6e20 7465 726d 2e61 735f 6469  eturn term.as_di
+00012980: 6d28 290a 0a20 2020 2064 6566 205f 5f73  m()..    def __s
+00012990: 7562 5f5f 2873 656c 662c 206f 7468 6572  ub__(self, other
+000129a0: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+000129b0: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+000129c0: 6d7c 696e 7420 6f74 6865 723a 0a20 2020  m|int other:.   
+000129d0: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
+000129e0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000129f0: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00012a00: 2e73 7562 5f72 6967 6874 286f 7468 6572  .sub_right(other
+00012a10: 290a 0a20 2020 2064 6566 2073 7562 5f72  )..    def sub_r
+00012a20: 6967 6874 2873 656c 663a 2044 696d 2c20  ight(self: Dim, 
+00012a30: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
+00012a40: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
+00012a50: 616d 2044 696d 7c69 6e74 206f 7468 6572  am Dim|int other
+00012a60: 3a0a 2020 2020 2020 2020 3a72 6574 7572  :.        :retur
+00012a70: 6e3a 2073 656c 6620 2d20 6f74 6865 720a  n: self - other.
+00012a80: 2020 2020 2020 2020 3a72 7479 7065 3a20          :rtype: 
+00012a90: 4469 6d0a 2020 2020 2020 2020 2222 220a  Dim.        """.
+00012aa0: 2020 2020 2020 2020 7465 726d 203d 205f          term = _
+00012ab0: 4f70 4c69 6e65 6172 5465 726d 2e66 726f  OpLinearTerm.fro
+00012ac0: 6d5f 6469 6d28 7365 6c66 290a 2020 2020  m_dim(self).    
+00012ad0: 2020 2020 7465 726d 2e65 7874 656e 645f      term.extend_
+00012ae0: 6164 645f 7375 625f 286f 7468 6572 2c20  add_sub_(other, 
+00012af0: 6b69 6e64 3d22 7375 6222 2c20 7269 6768  kind="sub", righ
+00012b00: 743d 5472 7565 290a 2020 2020 2020 2020  t=True).        
+00012b10: 7265 7475 726e 2074 6572 6d2e 6173 5f64  return term.as_d
+00012b20: 696d 2829 0a0a 2020 2020 6465 6620 7375  im()..    def su
+00012b30: 625f 6c65 6674 2873 656c 663a 2044 696d  b_left(self: Dim
+00012b40: 2c20 6f74 6865 7229 3a0a 2020 2020 2020  , other):.      
+00012b50: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
+00012b60: 6172 616d 2044 696d 7c69 6e74 206f 7468  aram Dim|int oth
+00012b70: 6572 3a0a 2020 2020 2020 2020 3a72 6574  er:.        :ret
+00012b80: 7572 6e3a 2028 2d6f 7468 6572 2920 2b20  urn: (-other) + 
+00012b90: 7365 6c66 0a20 2020 2020 2020 203a 7274  self.        :rt
+00012ba0: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
+00012bb0: 2022 2222 0a20 2020 2020 2020 2074 6572   """.        ter
+00012bc0: 6d20 3d20 5f4f 704c 696e 6561 7254 6572  m = _OpLinearTer
+00012bd0: 6d2e 6672 6f6d 5f64 696d 2873 656c 6629  m.from_dim(self)
+00012be0: 0a20 2020 2020 2020 2074 6572 6d2e 6578  .        term.ex
+00012bf0: 7465 6e64 5f61 6464 5f73 7562 5f28 6f74  tend_add_sub_(ot
+00012c00: 6865 722c 206b 696e 643d 2273 7562 222c  her, kind="sub",
+00012c10: 2072 6967 6874 3d46 616c 7365 290a 2020   right=False).  
+00012c20: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
+00012c30: 6d2e 6173 5f64 696d 2829 0a0a 2020 2020  m.as_dim()..    
+00012c40: 6465 6620 5f5f 6d75 6c5f 5f28 7365 6c66  def __mul__(self
+00012c50: 3a20 4469 6d2c 206f 7468 6572 293a 0a20  : Dim, other):. 
+00012c60: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00012c70: 2020 203a 7061 7261 6d20 4469 6d7c 696e     :param Dim|in
+00012c80: 7420 6f74 6865 723a 0a20 2020 2020 2020  t other:.       
+00012c90: 203a 7274 7970 653a 2044 696d 0a20 2020   :rtype: Dim.   
+00012ca0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00012cb0: 2074 6572 6d20 3d20 5f4f 704c 696e 6561   term = _OpLinea
+00012cc0: 7254 6572 6d2e 6672 6f6d 5f64 696d 2873  rTerm.from_dim(s
+00012cd0: 656c 6629 0a20 2020 2020 2020 2074 6572  elf).        ter
+00012ce0: 6d2e 6578 7465 6e64 5f6d 756c 5f64 6976  m.extend_mul_div
+00012cf0: 5f28 6f74 6865 722c 206b 696e 643d 226d  _(other, kind="m
+00012d00: 756c 222c 2072 6967 6874 3d54 7275 6529  ul", right=True)
+00012d10: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00012d20: 7465 726d 2e61 735f 6469 6d28 290a 0a20  term.as_dim().. 
+00012d30: 2020 2064 6566 205f 5f72 6d75 6c5f 5f28     def __rmul__(
+00012d40: 7365 6c66 3a20 4469 6d2c 206f 7468 6572  self: Dim, other
+00012d50: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00012d60: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+00012d70: 6d7c 696e 7420 6f74 6865 723a 0a20 2020  m|int other:.   
+00012d80: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
+00012d90: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012da0: 2020 2020 2074 6572 6d20 3d20 5f4f 704c       term = _OpL
+00012db0: 696e 6561 7254 6572 6d2e 6672 6f6d 5f64  inearTerm.from_d
+00012dc0: 696d 2873 656c 6629 0a20 2020 2020 2020  im(self).       
+00012dd0: 2074 6572 6d2e 6578 7465 6e64 5f6d 756c   term.extend_mul
+00012de0: 5f64 6976 5f28 6f74 6865 722c 206b 696e  _div_(other, kin
+00012df0: 643d 226d 756c 222c 2072 6967 6874 3d46  d="mul", right=F
+00012e00: 616c 7365 290a 2020 2020 2020 2020 7265  alse).        re
+00012e10: 7475 726e 2074 6572 6d2e 6173 5f64 696d  turn term.as_dim
+00012e20: 2829 0a0a 2020 2020 6465 6620 5f5f 666c  ()..    def __fl
+00012e30: 6f6f 7264 6976 5f5f 2873 656c 663a 2044  oordiv__(self: D
+00012e40: 696d 2c20 6f74 6865 7229 3a0a 2020 2020  im, other):.    
+00012e50: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00012e60: 3a70 6172 616d 2044 696d 7c69 6e74 206f  :param Dim|int o
+00012e70: 7468 6572 3a0a 2020 2020 2020 2020 3a72  ther:.        :r
+00012e80: 7479 7065 3a20 4469 6d0a 2020 2020 2020  type: Dim.      
+00012e90: 2020 2222 220a 2020 2020 2020 2020 7465    """.        te
+00012ea0: 726d 203d 205f 4f70 4c69 6e65 6172 5465  rm = _OpLinearTe
+00012eb0: 726d 2e66 726f 6d5f 6469 6d28 7365 6c66  rm.from_dim(self
+00012ec0: 290a 2020 2020 2020 2020 7465 726d 2e65  ).        term.e
+00012ed0: 7874 656e 645f 6d75 6c5f 6469 765f 286f  xtend_mul_div_(o
+00012ee0: 7468 6572 2c20 6b69 6e64 3d22 666c 6f6f  ther, kind="floo
+00012ef0: 7264 6976 222c 2072 6967 6874 3d54 7275  rdiv", right=Tru
+00012f00: 6529 0a20 2020 2020 2020 2072 6574 7572  e).        retur
+00012f10: 6e20 7465 726d 2e61 735f 6469 6d28 290a  n term.as_dim().
+00012f20: 0a20 2020 2064 6566 205f 5f74 7275 6564  .    def __trued
+00012f30: 6976 5f5f 2873 656c 662c 206f 7468 6572  iv__(self, other
+00012f40: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00012f50: 2020 2020 2020 203a 7061 7261 6d20 4469         :param Di
+00012f60: 6d7c 696e 7420 6f74 6865 723a 0a20 2020  m|int other:.   
+00012f70: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
+00012f80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00012f90: 2020 2020 2072 6574 7572 6e20 7365 6c66       return self
+00012fa0: 2e64 6976 5f72 6967 6874 286f 7468 6572  .div_right(other
+00012fb0: 290a 0a20 2020 2064 6566 2064 6976 5f6c  )..    def div_l
+00012fc0: 6566 7428 7365 6c66 3a20 4469 6d2c 206f  eft(self: Dim, o
+00012fd0: 7468 6572 293a 0a20 2020 2020 2020 2022  ther):.        "
+00012fe0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+00012ff0: 6d20 4469 6d7c 696e 7420 6f74 6865 723a  m Dim|int other:
+00013000: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00013010: 2044 696d 0a20 2020 2020 2020 2022 2222   Dim.        """
+00013020: 0a20 2020 2020 2020 2074 6572 6d20 3d20  .        term = 
+00013030: 5f4f 704c 696e 6561 7254 6572 6d2e 6672  _OpLinearTerm.fr
+00013040: 6f6d 5f64 696d 2873 656c 6629 0a20 2020  om_dim(self).   
+00013050: 2020 2020 2074 6572 6d2e 6578 7465 6e64       term.extend
+00013060: 5f6d 756c 5f64 6976 5f28 6f74 6865 722c  _mul_div_(other,
+00013070: 206b 696e 643d 2274 7275 6564 6976 222c   kind="truediv",
+00013080: 2072 6967 6874 3d46 616c 7365 290a 2020   right=False).  
+00013090: 2020 2020 2020 7265 7475 726e 2074 6572        return ter
+000130a0: 6d2e 6173 5f64 696d 2829 0a0a 2020 2020  m.as_dim()..    
+000130b0: 6465 6620 6469 765f 7269 6768 7428 7365  def div_right(se
+000130c0: 6c66 3a20 4469 6d2c 206f 7468 6572 293a  lf: Dim, other):
+000130d0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+000130e0: 2020 2020 203a 7061 7261 6d20 4469 6d7c       :param Dim|
+000130f0: 696e 7420 6f74 6865 723a 0a20 2020 2020  int other:.     
+00013100: 2020 203a 7274 7970 653a 2044 696d 0a20     :rtype: Dim. 
+00013110: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00013120: 2020 2074 6572 6d20 3d20 5f4f 704c 696e     term = _OpLin
+00013130: 6561 7254 6572 6d2e 6672 6f6d 5f64 696d  earTerm.from_dim
+00013140: 2873 656c 6629 0a20 2020 2020 2020 2074  (self).        t
+00013150: 6572 6d2e 6578 7465 6e64 5f6d 756c 5f64  erm.extend_mul_d
+00013160: 6976 5f28 6f74 6865 722c 206b 696e 643d  iv_(other, kind=
+00013170: 2274 7275 6564 6976 222c 2072 6967 6874  "truediv", right
+00013180: 3d54 7275 6529 0a20 2020 2020 2020 2072  =True).        r
+00013190: 6574 7572 6e20 7465 726d 2e61 735f 6469  eturn term.as_di
+000131a0: 6d28 290a 0a20 2020 2064 6566 2063 6569  m()..    def cei
+000131b0: 6c64 6976 5f6c 6566 7428 7365 6c66 3a20  ldiv_left(self: 
+000131c0: 4469 6d2c 206f 7468 6572 293a 0a20 2020  Dim, other):.   
+000131d0: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+000131e0: 203a 7061 7261 6d20 4469 6d7c 696e 7420   :param Dim|int 
+000131f0: 6f74 6865 723a 0a20 2020 2020 2020 203a  other:.        :
+00013200: 7274 7970 653a 2044 696d 0a20 2020 2020  rtype: Dim.     
+00013210: 2020 2022 2222 0a20 2020 2020 2020 2074     """.        t
+00013220: 6572 6d20 3d20 5f4f 704c 696e 6561 7254  erm = _OpLinearT
+00013230: 6572 6d2e 6672 6f6d 5f64 696d 2873 656c  erm.from_dim(sel
+00013240: 6629 0a20 2020 2020 2020 2074 6572 6d2e  f).        term.
+00013250: 6578 7465 6e64 5f6d 756c 5f64 6976 5f28  extend_mul_div_(
+00013260: 6f74 6865 722c 206b 696e 643d 2263 6569  other, kind="cei
+00013270: 6c64 6976 222c 2072 6967 6874 3d46 616c  ldiv", right=Fal
+00013280: 7365 290a 2020 2020 2020 2020 7265 7475  se).        retu
+00013290: 726e 2074 6572 6d2e 6173 5f64 696d 2829  rn term.as_dim()
+000132a0: 0a0a 2020 2020 6465 6620 6365 696c 6469  ..    def ceildi
+000132b0: 765f 7269 6768 7428 7365 6c66 3a20 4469  v_right(self: Di
+000132c0: 6d2c 206f 7468 6572 293a 0a20 2020 2020  m, other):.     
+000132d0: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+000132e0: 7061 7261 6d20 4469 6d7c 696e 7420 6f74  param Dim|int ot
+000132f0: 6865 723a 0a20 2020 2020 2020 203a 7274  her:.        :rt
+00013300: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
+00013310: 2022 2222 0a20 2020 2020 2020 2074 6572   """.        ter
+00013320: 6d20 3d20 5f4f 704c 696e 6561 7254 6572  m = _OpLinearTer
+00013330: 6d2e 6672 6f6d 5f64 696d 2873 656c 6629  m.from_dim(self)
+00013340: 0a20 2020 2020 2020 2074 6572 6d2e 6578  .        term.ex
+00013350: 7465 6e64 5f6d 756c 5f64 6976 5f28 6f74  tend_mul_div_(ot
+00013360: 6865 722c 206b 696e 643d 2263 6569 6c64  her, kind="ceild
+00013370: 6976 222c 2072 6967 6874 3d54 7275 6529  iv", right=True)
+00013380: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00013390: 7465 726d 2e61 735f 6469 6d28 290a 0a20  term.as_dim().. 
+000133a0: 2020 2064 6566 205f 5f6e 6567 5f5f 2873     def __neg__(s
+000133b0: 656c 6629 3a0a 2020 2020 2020 2020 2222  elf):.        ""
+000133c0: 220a 2020 2020 2020 2020 3a72 7479 7065  ".        :rtype
+000133d0: 3a20 4469 6d0a 2020 2020 2020 2020 2222  : Dim.        ""
+000133e0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+000133f0: 202d 3120 2a20 7365 6c66 0a0a 2020 2020   -1 * self..    
+00013400: 6465 6620 6973 5f63 6f6e 7374 616e 745f  def is_constant_
+00013410: 7374 6174 6963 5f64 696d 2873 656c 6629  static_dim(self)
+00013420: 202d 3e20 626f 6f6c 3a0a 2020 2020 2020   -> bool:.      
+00013430: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
+00013440: 6574 7572 6e3a 2064 6572 6976 6564 206f  eturn: derived o
+00013450: 7020 6f66 2074 7970 6520 636f 6e73 7461  p of type consta
+00013460: 6e74 0a20 2020 2020 2020 2022 2222 0a20  nt.        """. 
+00013470: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00013480: 6c66 2e64 6572 6976 6564 5f66 726f 6d5f  lf.derived_from_
+00013490: 6f70 2061 6e64 2073 656c 662e 6465 7269  op and self.deri
+000134a0: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
+000134b0: 203d 3d20 2263 6f6e 7374 616e 7422 0a0a   == "constant"..
+000134c0: 0a64 6566 205f 6d61 6b65 5f63 6f6e 7374  .def _make_const
+000134d0: 616e 745f 7374 6174 6963 5f64 696d 2876  ant_static_dim(v
+000134e0: 616c 7565 2c20 6b69 6e64 3d4e 6f6e 6529  alue, kind=None)
+000134f0: 3a0a 2020 2020 2222 220a 2020 2020 3a70  :.    """.    :p
+00013500: 6172 616d 2069 6e74 2076 616c 7565 3a0a  aram int value:.
+00013510: 2020 2020 3a70 6172 616d 2045 6e74 6974      :param Entit
+00013520: 797c 4e6f 6e65 206b 696e 643a 0a20 2020  y|None kind:.   
+00013530: 203a 7274 7970 653a 2044 696d 0a20 2020   :rtype: Dim.   
+00013540: 2022 2222 0a20 2020 2072 6574 7572 6e20   """.    return 
+00013550: 5f64 2e44 696d 280a 2020 2020 2020 2020  _d.Dim(.        
+00013560: 6469 6d65 6e73 696f 6e3d 7661 6c75 652c  dimension=value,
+00013570: 0a20 2020 2020 2020 206b 696e 643d 6b69  .        kind=ki
+00013580: 6e64 206f 7220 4469 6d54 7970 6573 2e55  nd or DimTypes.U
+00013590: 6e73 7065 6369 6669 6564 2c0a 2020 2020  nspecified,.    
+000135a0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
+000135b0: 2275 6e6e 616d 6564 5f25 7364 696d 5f25  "unnamed_%sdim_%
+000135c0: 6922 2025 2028 6b69 6e64 2e6e 616d 6520  i" % (kind.name 
+000135d0: 2b20 225f 2220 6966 206b 696e 6420 656c  + "_" if kind el
+000135e0: 7365 2022 222c 2076 616c 7565 292c 0a20  se "", value),. 
+000135f0: 2020 2020 2020 2064 6572 6976 6564 5f66         derived_f
+00013600: 726f 6d5f 6f70 3d4f 7028 6b69 6e64 3d22  rom_op=Op(kind="
+00013610: 636f 6e73 7461 6e74 222c 2069 6e70 7574  constant", input
+00013620: 733d 5b5d 2c20 6174 7472 6962 733d 7b22  s=[], attribs={"
+00013630: 7661 6c75 6522 3a20 7661 6c75 657d 292c  value": value}),
+00013640: 0a20 2020 2020 2020 2061 7574 6f5f 6765  .        auto_ge
+00013650: 6e65 7261 7465 643d 5472 7565 2c0a 2020  nerated=True,.  
+00013660: 2020 290a 0a0a 636c 6173 7320 4f70 3a0a    )...class Op:.
+00013670: 2020 2020 2222 220a 2020 2020 4f70 206f      """.    Op o
+00013680: 6e20 3a63 6c61 7373 3a60 4469 6d60 2077  n :class:`Dim` w
+00013690: 6869 6368 2072 6573 756c 7473 2069 6e20  hich results in 
+000136a0: 6120 6465 7269 7665 6420 3a63 6c61 7373  a derived :class
+000136b0: 3a60 4469 6d60 2e0a 2020 2020 2222 220a  :`Dim`..    """.
+000136c0: 0a20 2020 2064 6566 205f 5f69 6e69 745f  .    def __init_
+000136d0: 5f28 7365 6c66 2c20 6b69 6e64 2c20 696e  _(self, kind, in
+000136e0: 7075 7473 2c20 6174 7472 6962 733d 4e6f  puts, attribs=No
+000136f0: 6e65 293a 0a20 2020 2020 2020 2022 2222  ne):.        """
+00013700: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00013710: 7374 7220 6b69 6e64 3a20 2261 6464 222c  str kind: "add",
+00013720: 2022 7375 6222 2c20 226d 756c 222c 2022   "sub", "mul", "
+00013730: 6365 696c 6469 7622 0a20 2020 2020 2020  ceildiv".       
+00013740: 203a 7061 7261 6d20 6c69 7374 5b44 696d   :param list[Dim
+00013750: 5d20 696e 7075 7473 3a0a 2020 2020 2020  ] inputs:.      
+00013760: 2020 3a70 6172 616d 2064 6963 745b 7374    :param dict[st
+00013770: 725d 7c4e 6f6e 6520 6174 7472 6962 733a  r]|None attribs:
+00013780: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00013790: 2020 2020 2073 656c 662e 6b69 6e64 203d       self.kind =
+000137a0: 206b 696e 640a 2020 2020 2020 2020 7365   kind.        se
+000137b0: 6c66 2e69 6e70 7574 7320 3d20 696e 7075  lf.inputs = inpu
+000137c0: 7473 0a20 2020 2020 2020 2073 656c 662e  ts.        self.
+000137d0: 6f75 7470 7574 203d 204e 6f6e 6520 2023  output = None  #
+000137e0: 2074 7970 653a 204f 7074 696f 6e61 6c5b   type: Optional[
+000137f0: 5f64 2e44 696d 5d0a 2020 2020 2020 2020  _d.Dim].        
+00013800: 7365 6c66 2e61 7474 7269 6273 203d 2061  self.attribs = a
+00013810: 7474 7269 6273 0a0a 2020 2020 6465 6620  ttribs..    def 
+00013820: 5f5f 7265 7072 5f5f 2873 656c 6629 3a0a  __repr__(self):.
+00013830: 2020 2020 2020 2020 6174 7472 6962 7320          attribs 
+00013840: 3d20 2822 2025 7222 2025 2073 656c 662e  = (" %r" % self.
+00013850: 6174 7472 6962 7329 2069 6620 7365 6c66  attribs) if self
+00013860: 2e61 7474 7269 6273 2065 6c73 6520 2222  .attribs else ""
+00013870: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00013880: 223c 4469 6d2e 4f70 2025 7220 2573 2573  "<Dim.Op %r %s%s
+00013890: 3e22 2025 2028 7365 6c66 2e6b 696e 642c  >" % (self.kind,
+000138a0: 2073 656c 662e 696e 7075 7473 2c20 6174   self.inputs, at
+000138b0: 7472 6962 7329 0a0a 2020 2020 6465 6620  tribs)..    def 
+000138c0: 5f76 616c 7565 2873 656c 6629 3a0a 2020  _value(self):.  
+000138d0: 2020 2020 2020 7265 7475 726e 2073 656c        return sel
+000138e0: 662e 6b69 6e64 2c20 7475 706c 6528 7365  f.kind, tuple(se
+000138f0: 6c66 2e69 6e70 7574 7329 2c20 6672 6f7a  lf.inputs), froz
+00013900: 656e 7365 7428 7365 6c66 2e61 7474 7269  enset(self.attri
+00013910: 6273 2e69 7465 6d73 2829 2920 6966 2073  bs.items()) if s
+00013920: 656c 662e 6174 7472 6962 7320 656c 7365  elf.attribs else
+00013930: 204e 6f6e 650a 0a20 2020 2064 6566 205f   None..    def _
+00013940: 5f68 6173 685f 5f28 7365 6c66 293a 0a20  _hash__(self):. 
+00013950: 2020 2020 2020 2072 6574 7572 6e20 6861         return ha
+00013960: 7368 2873 656c 662e 5f76 616c 7565 2829  sh(self._value()
+00013970: 290a 0a20 2020 2064 6566 205f 5f65 715f  )..    def __eq_
+00013980: 5f28 7365 6c66 2c20 6f74 6865 7229 3a0a  _(self, other):.
+00013990: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+000139a0: 7461 6e63 6528 6f74 6865 722c 204f 7029  tance(other, Op)
+000139b0: 3a0a 2020 2020 2020 2020 2020 2020 7265  :.            re
+000139c0: 7475 726e 2073 656c 662e 5f76 616c 7565  turn self._value
+000139d0: 2829 203d 3d20 6f74 6865 722e 5f76 616c  () == other._val
+000139e0: 7565 2829 0a20 2020 2020 2020 2072 6574  ue().        ret
+000139f0: 7572 6e20 4661 6c73 650a 0a20 2020 2064  urn False..    d
+00013a00: 6566 205f 5f6e 655f 5f28 7365 6c66 2c20  ef __ne__(self, 
+00013a10: 6f74 6865 7229 3a0a 2020 2020 2020 2020  other):.        
+00013a20: 7265 7475 726e 206e 6f74 2073 656c 662e  return not self.
+00013a30: 5f5f 6571 5f5f 286f 7468 6572 290a 0a0a  __eq__(other)...
+00013a40: 6465 6620 5f67 6574 5f64 6573 6372 6970  def _get_descrip
+00013a50: 7469 6f6e 2864 696d 2c20 6272 6163 6b65  tion(dim, bracke
+00013a60: 7473 3d54 7275 6529 3a0a 2020 2020 2222  ts=True):.    ""
+00013a70: 220a 2020 2020 3a70 6172 616d 2044 696d  ".    :param Dim
+00013a80: 2064 696d 3a0a 2020 2020 3a70 6172 616d   dim:.    :param
+00013a90: 2062 6f6f 6c20 6272 6163 6b65 7473 3a20   bool brackets: 
+00013aa0: 6164 6420 6272 6163 6b65 7473 2077 6865  add brackets whe
+00013ab0: 6e20 6e65 6365 7373 6172 790a 2020 2020  n necessary.    
+00013ac0: 3a72 7479 7065 3a20 7374 720a 2020 2020  :rtype: str.    
+00013ad0: 2222 220a 2020 2020 6966 2064 696d 2e64  """.    if dim.d
+00013ae0: 6573 6372 6970 7469 6f6e 2061 6e64 2064  escription and d
+00013af0: 696d 2e64 6573 6372 6970 7469 6f6e 2e73  im.description.s
+00013b00: 7461 7274 7377 6974 6828 2275 6e6e 616d  tartswith("unnam
+00013b10: 6564 5f22 2920 616e 6420 6469 6d2e 6469  ed_") and dim.di
+00013b20: 6d65 6e73 696f 6e20 6973 206e 6f74 204e  mension is not N
+00013b30: 6f6e 653a 0a20 2020 2020 2020 2072 6574  one:.        ret
+00013b40: 7572 6e20 7374 7228 6469 6d2e 6469 6d65  urn str(dim.dime
+00013b50: 6e73 696f 6e29 0a20 2020 2069 6620 6469  nsion).    if di
+00013b60: 6d2e 6465 7363 7269 7074 696f 6e3a 0a20  m.description:. 
+00013b70: 2020 2020 2020 2069 6620 6272 6163 6b65         if bracke
+00013b80: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
+00013b90: 696d 706f 7274 2072 650a 0a20 2020 2020  import re..     
+00013ba0: 2020 2020 2020 2069 6620 7265 2e73 6561         if re.sea
+00013bb0: 7263 6828 225b 2b5c 5c2d 2f20 5d22 2c20  rch("[+\\-/ ]", 
+00013bc0: 6469 6d2e 6465 7363 7269 7074 696f 6e29  dim.description)
+00013bd0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013be0: 2020 7265 7475 726e 2022 2825 7329 2220    return "(%s)" 
+00013bf0: 2520 6469 6d2e 6465 7363 7269 7074 696f  % dim.descriptio
+00013c00: 6e0a 2020 2020 2020 2020 7265 7475 726e  n.        return
+00013c10: 2064 696d 2e64 6573 6372 6970 7469 6f6e   dim.description
+00013c20: 0a20 2020 2072 6574 7572 6e20 2275 6e6e  .    return "unn
+00013c30: 616d 6564 5f25 735f 6469 6d25 7322 2025  amed_%s_dim%s" %
+00013c40: 2028 6469 6d2e 6b69 6e64 2c20 6469 6d2e   (dim.kind, dim.
+00013c50: 6469 6d65 6e73 696f 6e20 6966 2064 696d  dimension if dim
+00013c60: 2e64 696d 656e 7369 6f6e 2069 7320 6e6f  .dimension is no
+00013c70: 7420 4e6f 6e65 2065 6c73 6520 223f 2229  t None else "?")
+00013c80: 0a0a 0a63 6c61 7373 205f 4f70 4d75 6c74  ...class _OpMult
+00013c90: 5465 726d 3a0a 2020 2020 2222 220a 2020  Term:.    """.  
+00013ca0: 2020 7265 7072 6573 656e 7473 2073 7468    represents sth
+00013cb0: 206c 696b 6520 6120 2a20 6220 2a20 630a   like a * b * c.
+00013cc0: 2020 2020 2222 220a 0a20 2020 2040 636c      """..    @cl
+00013cd0: 6173 736d 6574 686f 640a 2020 2020 6465  assmethod.    de
+00013ce0: 6620 6672 6f6d 5f64 696d 2863 6c73 2c20  f from_dim(cls, 
+00013cf0: 6469 6d3a 205f 642e 4469 6d29 202d 3e20  dim: _d.Dim) -> 
+00013d00: 5f4f 704d 756c 7454 6572 6d3a 0a20 2020  _OpMultTerm:.   
+00013d10: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00013d20: 203a 7061 7261 6d20 6469 6d3a 0a20 2020   :param dim:.   
+00013d30: 2020 2020 203a 7265 7475 726e 3a20 6f70       :return: op
+00013d40: 206d 756c 7420 7465 726d 0a20 2020 2020   mult term.     
+00013d50: 2020 2022 2222 0a20 2020 2020 2020 2064     """.        d
+00013d60: 696d 203d 2064 696d 2e67 6574 5f73 616d  im = dim.get_sam
+00013d70: 655f 6261 7365 2829 0a20 2020 2020 2020  e_base().       
+00013d80: 2069 6620 6469 6d2e 6469 6d65 6e73 696f   if dim.dimensio
+00013d90: 6e20 3d3d 2031 2061 6e64 2064 696d 2e69  n == 1 and dim.i
+00013da0: 735f 636f 6e73 7461 6e74 5f73 7461 7469  s_constant_stati
+00013db0: 635f 6469 6d28 293a 0a20 2020 2020 2020  c_dim():.       
+00013dc0: 2020 2020 2072 6574 7572 6e20 636c 732e       return cls.
+00013dd0: 6f6e 6528 290a 2020 2020 2020 2020 6966  one().        if
+00013de0: 2064 696d 2e64 6572 6976 6564 5f66 726f   dim.derived_fro
+00013df0: 6d5f 6f70 2061 6e64 2064 696d 2e64 6572  m_op and dim.der
+00013e00: 6976 6564 5f66 726f 6d5f 6f70 2e6b 696e  ived_from_op.kin
+00013e10: 6420 3d3d 2022 6d75 6c22 3a0a 2020 2020  d == "mul":.    
+00013e20: 2020 2020 2020 2020 7265 7475 726e 2063          return c
+00013e30: 6c73 286c 6973 7428 6469 6d2e 6465 7269  ls(list(dim.deri
+00013e40: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
+00013e50: 7473 2929 0a20 2020 2020 2020 2072 6574  ts)).        ret
+00013e60: 7572 6e20 636c 7328 5b64 696d 5d29 0a0a  urn cls([dim])..
+00013e70: 2020 2020 4063 6c61 7373 6d65 7468 6f64      @classmethod
+00013e80: 0a20 2020 2064 6566 2066 726f 6d5f 6469  .    def from_di
+00013e90: 6d5f 6661 6374 6f72 7328 636c 732c 2064  m_factors(cls, d
+00013ea0: 696d 7329 3a0a 2020 2020 2020 2020 2222  ims):.        ""
+00013eb0: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+00013ec0: 206c 6973 745b 4469 6d5d 2064 696d 733a   list[Dim] dims:
+00013ed0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+00013ee0: 2044 696d 2e5f 4f70 4d75 6c74 5465 726d   Dim._OpMultTerm
+00013ef0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00013f00: 2020 2020 2072 6573 203d 2063 6c73 2e6f       res = cls.o
+00013f10: 6e65 2829 0a20 2020 2020 2020 2066 6f72  ne().        for
+00013f20: 2064 2069 6e20 6469 6d73 3a0a 2020 2020   d in dims:.    
+00013f30: 2020 2020 2020 2020 7265 732e 6578 7465          res.exte
+00013f40: 6e64 5f6d 756c 5f64 6976 5f28 642c 206b  nd_mul_div_(d, k
+00013f50: 696e 643d 226d 756c 222c 2072 6967 6874  ind="mul", right
+00013f60: 3d54 7275 6529 0a20 2020 2020 2020 2072  =True).        r
+00013f70: 6574 7572 6e20 7265 730a 0a20 2020 2040  eturn res..    @
+00013f80: 636c 6173 736d 6574 686f 640a 2020 2020  classmethod.    
+00013f90: 6465 6620 6f6e 6528 636c 7329 3a0a 2020  def one(cls):.  
+00013fa0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+00013fb0: 2020 3a72 7479 7065 3a20 4469 6d2e 5f4f    :rtype: Dim._O
+00013fc0: 704d 756c 7454 6572 6d0a 2020 2020 2020  pMultTerm.      
+00013fd0: 2020 2222 220a 2020 2020 2020 2020 7265    """.        re
+00013fe0: 7475 726e 2063 6c73 285b 5d29 0a0a 2020  turn cls([])..  
+00013ff0: 2020 6465 6620 5f5f 696e 6974 5f5f 2873    def __init__(s
+00014000: 656c 662c 2074 6572 6d73 293a 0a20 2020  elf, terms):.   
+00014010: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00014020: 203a 7061 7261 6d20 6c69 7374 5b44 696d   :param list[Dim
+00014030: 5d20 7465 726d 733a 0a20 2020 2020 2020  ] terms:.       
+00014040: 2022 2222 0a20 2020 2020 2020 2073 656c   """.        sel
+00014050: 662e 7465 726d 7320 3d20 7465 726d 730a  f.terms = terms.
+00014060: 0a20 2020 2064 6566 205f 5f68 6173 685f  .    def __hash_
+00014070: 5f28 7365 6c66 293a 0a20 2020 2020 2020  _(self):.       
+00014080: 2072 6574 7572 6e20 6861 7368 2874 7570   return hash(tup
+00014090: 6c65 2873 656c 662e 7465 726d 7329 290a  le(self.terms)).
+000140a0: 0a20 2020 2064 6566 205f 5f65 715f 5f28  .    def __eq__(
+000140b0: 7365 6c66 2c20 6f74 6865 7229 3a0a 2020  self, other):.  
+000140c0: 2020 2020 2020 2222 220a 2020 2020 2020        """.      
+000140d0: 2020 3a70 6172 616d 2044 696d 7c44 696d    :param Dim|Dim
+000140e0: 2e5f 4f70 4d75 6c74 5465 726d 206f 7468  ._OpMultTerm oth
+000140f0: 6572 3a0a 2020 2020 2020 2020 2222 220a  er:.        """.
+00014100: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00014110: 7461 6e63 6528 6f74 6865 722c 205f 4f70  tance(other, _Op
+00014120: 4d75 6c74 5465 726d 293a 0a20 2020 2020  MultTerm):.     
+00014130: 2020 2020 2020 2072 6574 7572 6e20 7365         return se
+00014140: 6c66 2e74 6572 6d73 203d 3d20 6f74 6865  lf.terms == othe
+00014150: 722e 7465 726d 730a 2020 2020 2020 2020  r.terms.        
+00014160: 7265 7475 726e 2046 616c 7365 0a0a 2020  return False..  
+00014170: 2020 6465 6620 5f5f 6e65 5f5f 2873 656c    def __ne__(sel
+00014180: 662c 206f 7468 6572 293a 0a20 2020 2020  f, other):.     
+00014190: 2020 2072 6574 7572 6e20 6e6f 7420 7365     return not se
+000141a0: 6c66 2e5f 5f65 715f 5f28 6f74 6865 7229  lf.__eq__(other)
+000141b0: 0a0a 2020 2020 6465 6620 5f5f 7265 7072  ..    def __repr
+000141c0: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+000141d0: 2020 7265 7475 726e 2022 4469 6d2e 5f4f    return "Dim._O
+000141e0: 704d 756c 7454 6572 6d28 2572 2922 2025  pMultTerm(%r)" %
+000141f0: 2028 7365 6c66 2e74 6572 6d73 2c29 0a0a   (self.terms,)..
+00014200: 2020 2020 4070 726f 7065 7274 790a 2020      @property.  
+00014210: 2020 6465 6620 6469 6d65 6e73 696f 6e28    def dimension(
+00014220: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00014230: 2222 0a20 2020 2020 2020 203a 7274 7970  "".        :rtyp
+00014240: 653a 2069 6e74 7c4e 6f6e 650a 2020 2020  e: int|None.    
+00014250: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00014260: 6469 6d20 3d20 310a 2020 2020 2020 2020  dim = 1.        
+00014270: 666f 7220 7061 7274 2069 6e20 7365 6c66  for part in self
+00014280: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
+00014290: 2020 2020 6966 2070 6172 742e 6469 6d65      if part.dime
+000142a0: 6e73 696f 6e20 6973 204e 6f6e 653a 0a20  nsion is None:. 
+000142b0: 2020 2020 2020 2020 2020 2020 2020 2072                 r
+000142c0: 6574 7572 6e20 4e6f 6e65 0a20 2020 2020  eturn None.     
+000142d0: 2020 2020 2020 2064 696d 202a 3d20 7061         dim *= pa
+000142e0: 7274 2e64 696d 656e 7369 6f6e 0a20 2020  rt.dimension.   
+000142f0: 2020 2020 2072 6574 7572 6e20 6469 6d0a       return dim.
+00014300: 0a20 2020 2064 6566 2062 6173 655f 7465  .    def base_te
+00014310: 726d 2873 656c 6629 3a0a 2020 2020 2020  rm(self):.      
+00014320: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
+00014330: 7479 7065 3a20 4469 6d0a 2020 2020 2020  type: Dim.      
+00014340: 2020 2222 220a 2020 2020 2020 2020 6173    """.        as
+00014350: 7365 7274 2073 656c 662e 7465 726d 730a  sert self.terms.
+00014360: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00014370: 656c 662e 7465 726d 735b 2d31 5d0a 0a20  elf.terms[-1].. 
+00014380: 2020 2064 6566 2069 735f 6f6e 6528 7365     def is_one(se
+00014390: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000143a0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000143b0: 2062 6f6f 6c0a 2020 2020 2020 2020 2222   bool.        ""
+000143c0: 220a 2020 2020 2020 2020 7265 7475 726e  ".        return
+000143d0: 206e 6f74 2073 656c 662e 7465 726d 730a   not self.terms.
+000143e0: 0a20 2020 2064 6566 2069 735f 636f 6e73  .    def is_cons
+000143f0: 7461 6e74 5f73 7461 7469 635f 6469 6d28  tant_static_dim(
+00014400: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+00014410: 2222 0a20 2020 2020 2020 203a 7274 7970  "".        :rtyp
+00014420: 653a 2062 6f6f 6c0a 2020 2020 2020 2020  e: bool.        
+00014430: 2222 220a 2020 2020 2020 2020 6966 206e  """.        if n
+00014440: 6f74 2073 656c 662e 7465 726d 733a 0a20  ot self.terms:. 
+00014450: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+00014460: 6e20 5472 7565 0a20 2020 2020 2020 2072  n True.        r
+00014470: 6574 7572 6e20 616c 6c28 7465 726d 2e69  eturn all(term.i
+00014480: 735f 636f 6e73 7461 6e74 5f73 7461 7469  s_constant_stati
+00014490: 635f 6469 6d28 2920 666f 7220 7465 726d  c_dim() for term
+000144a0: 2069 6e20 7365 6c66 2e74 6572 6d73 290a   in self.terms).
+000144b0: 0a20 2020 2064 6566 2063 6f70 7928 7365  .    def copy(se
+000144c0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000144d0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000144e0: 2044 696d 2e5f 4f70 4d75 6c74 5465 726d   Dim._OpMultTerm
+000144f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00014500: 2020 2020 2072 6574 7572 6e20 5f4f 704d       return _OpM
+00014510: 756c 7454 6572 6d28 6c69 7374 2873 656c  ultTerm(list(sel
+00014520: 662e 7465 726d 7329 290a 0a20 2020 2064  f.terms))..    d
+00014530: 6566 206e 6567 6174 6976 6528 7365 6c66  ef negative(self
+00014540: 293a 0a20 2020 2020 2020 2022 2222 0a20  ):.        """. 
+00014550: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
+00014560: 696d 2e5f 4f70 4d75 6c74 5465 726d 0a20  im._OpMultTerm. 
+00014570: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00014580: 2020 2069 6620 7365 6c66 2e74 6572 6d73     if self.terms
+00014590: 2061 6e64 2073 656c 662e 7465 726d 735b   and self.terms[
+000145a0: 305d 2e69 735f 636f 6e73 7461 6e74 5f73  0].is_constant_s
+000145b0: 7461 7469 635f 6469 6d28 2920 616e 6420  tatic_dim() and 
+000145c0: 7365 6c66 2e74 6572 6d73 5b30 5d2e 6469  self.terms[0].di
+000145d0: 6d65 6e73 696f 6e20 3d3d 202d 313a 0a20  mension == -1:. 
+000145e0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000145f0: 6e20 5f4f 704d 756c 7454 6572 6d28 7365  n _OpMultTerm(se
+00014600: 6c66 2e74 6572 6d73 5b31 3a5d 290a 2020  lf.terms[1:]).  
+00014610: 2020 2020 2020 7265 7320 3d20 7365 6c66        res = self
+00014620: 2e63 6f70 7928 290a 2020 2020 2020 2020  .copy().        
+00014630: 7265 732e 6578 7465 6e64 5f6d 756c 5f64  res.extend_mul_d
+00014640: 6976 5f28 5f6d 616b 655f 636f 6e73 7461  iv_(_make_consta
+00014650: 6e74 5f73 7461 7469 635f 6469 6d28 2d31  nt_static_dim(-1
+00014660: 292c 206b 696e 643d 226d 756c 222c 2072  ), kind="mul", r
+00014670: 6967 6874 3d46 616c 7365 290a 2020 2020  ight=False).    
+00014680: 2020 2020 7265 7475 726e 2072 6573 0a0a      return res..
+00014690: 2020 2020 6465 6620 6469 7669 7369 626c      def divisibl
+000146a0: 6528 7365 6c66 2c20 6f74 6865 722c 2072  e(self, other, r
+000146b0: 6967 6874 293a 0a20 2020 2020 2020 2022  ight):.        "
+000146c0: 2222 0a20 2020 2020 2020 203a 7061 7261  "".        :para
+000146d0: 6d20 4469 6d20 6f74 6865 723a 0a20 2020  m Dim other:.   
+000146e0: 2020 2020 203a 7061 7261 6d20 626f 6f6c       :param bool
+000146f0: 2072 6967 6874 3a0a 2020 2020 2020 2020   right:.        
+00014700: 3a72 6574 7572 6e3a 2077 6865 7468 6572  :return: whether
+00014710: 2077 6520 6361 6e20 6469 7669 6465 206f   we can divide o
+00014720: 7468 6572 2c20 7769 7468 6f75 7420 7265  ther, without re
+00014730: 6d61 696e 6465 720a 2020 2020 2020 2020  mainder.        
+00014740: 3a72 7479 7065 3a20 626f 6f6c 0a20 2020  :rtype: bool.   
+00014750: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00014760: 2069 6620 6e6f 7420 7365 6c66 2e74 6572   if not self.ter
+00014770: 6d73 3a0a 2020 2020 2020 2020 2020 2020  ms:.            
+00014780: 7265 7475 726e 2046 616c 7365 0a20 2020  return False.   
+00014790: 2020 2020 2069 6620 6f74 6865 722e 6465       if other.de
+000147a0: 7269 7665 645f 6672 6f6d 5f6f 7020 616e  rived_from_op an
+000147b0: 6420 6f74 6865 722e 6465 7269 7665 645f  d other.derived_
+000147c0: 6672 6f6d 5f6f 702e 6b69 6e64 203d 3d20  from_op.kind == 
+000147d0: 226d 756c 223a 0a20 2020 2020 2020 2020  "mul":.         
+000147e0: 2020 2074 6d70 203d 2073 656c 662e 636f     tmp = self.co
+000147f0: 7079 2829 0a20 2020 2020 2020 2020 2020  py().           
+00014800: 2066 6f72 2074 6572 6d20 696e 206f 7468   for term in oth
+00014810: 6572 2e64 6572 6976 6564 5f66 726f 6d5f  er.derived_from_
+00014820: 6f70 2e69 6e70 7574 7320 6966 2072 6967  op.inputs if rig
+00014830: 6874 2065 6c73 6520 7265 7665 7273 6564  ht else reversed
+00014840: 286f 7468 6572 2e64 6572 6976 6564 5f66  (other.derived_f
+00014850: 726f 6d5f 6f70 2e69 6e70 7574 7329 3a0a  rom_op.inputs):.
+00014860: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014870: 6966 206e 6f74 2074 6d70 2e64 6976 6973  if not tmp.divis
+00014880: 6962 6c65 2874 6572 6d2c 2072 6967 6874  ible(term, right
+00014890: 3d72 6967 6874 293a 0a20 2020 2020 2020  =right):.       
+000148a0: 2020 2020 2020 2020 2020 2020 2072 6574               ret
+000148b0: 7572 6e20 4661 6c73 650a 2020 2020 2020  urn False.      
+000148c0: 2020 2020 2020 2020 2020 746d 702e 6578            tmp.ex
+000148d0: 7465 6e64 5f6d 756c 5f64 6976 5f28 7465  tend_mul_div_(te
+000148e0: 726d 2c20 6b69 6e64 3d22 7472 7565 6469  rm, kind="truedi
+000148f0: 7622 2c20 7269 6768 743d 7269 6768 7429  v", right=right)
+00014900: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00014910: 7572 6e20 5472 7565 0a20 2020 2020 2020  urn True.       
+00014920: 206d 6f73 745f 7265 6365 6e74 5f74 6572   most_recent_ter
+00014930: 6d20 3d20 7365 6c66 2e74 6572 6d73 5b2d  m = self.terms[-
+00014940: 3120 6966 2072 6967 6874 2065 6c73 6520  1 if right else 
+00014950: 305d 0a20 2020 2020 2020 2069 6620 6f74  0].        if ot
+00014960: 6865 7220 3d3d 206d 6f73 745f 7265 6365  her == most_rece
+00014970: 6e74 5f74 6572 6d3a 0a20 2020 2020 2020  nt_term:.       
+00014980: 2020 2020 2072 6574 7572 6e20 5472 7565       return True
+00014990: 0a20 2020 2020 2020 2069 6620 6d6f 7374  .        if most
+000149a0: 5f72 6563 656e 745f 7465 726d 2e64 696d  _recent_term.dim
+000149b0: 656e 7369 6f6e 2069 7320 6e6f 7420 4e6f  ension is not No
+000149c0: 6e65 2061 6e64 206f 7468 6572 2e64 696d  ne and other.dim
+000149d0: 656e 7369 6f6e 2069 7320 6e6f 7420 4e6f  ension is not No
+000149e0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000149f0: 6966 206d 6f73 745f 7265 6365 6e74 5f74  if most_recent_t
+00014a00: 6572 6d2e 6469 6d65 6e73 696f 6e20 2520  erm.dimension % 
+00014a10: 6f74 6865 722e 6469 6d65 6e73 696f 6e20  other.dimension 
+00014a20: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00014a30: 2020 2020 2020 7265 7475 726e 2054 7275        return Tru
+00014a40: 650a 2020 2020 2020 2020 7265 7475 726e  e.        return
+00014a50: 2046 616c 7365 0a0a 2020 2020 6465 6620   False..    def 
+00014a60: 6361 6e5f 7369 6d70 6c69 6679 2873 656c  can_simplify(sel
+00014a70: 662c 206f 7468 6572 2c20 6b69 6e64 2c20  f, other, kind, 
+00014a80: 7269 6768 7429 3a0a 2020 2020 2020 2020  right):.        
+00014a90: 2222 220a 2020 2020 2020 2020 3a70 6172  """.        :par
+00014aa0: 616d 2044 696d 206f 7468 6572 3a0a 2020  am Dim other:.  
+00014ab0: 2020 2020 2020 3a70 6172 616d 2073 7472        :param str
+00014ac0: 206b 696e 643a 0a20 2020 2020 2020 203a   kind:.        :
+00014ad0: 7061 7261 6d20 626f 6f6c 2072 6967 6874  param bool right
+00014ae0: 3a0a 2020 2020 2020 2020 3a72 6574 7572  :.        :retur
+00014af0: 6e3a 2077 6865 7468 6572 2077 6520 6361  n: whether we ca
+00014b00: 6e20 7369 6d70 6c69 6679 2077 6865 6e20  n simplify when 
+00014b10: 6170 706c 7969 6e67 2074 6869 7320 6f70  applying this op
+00014b20: 6572 6174 696f 6e0a 2020 2020 2020 2020  eration.        
+00014b30: 3a72 7479 7065 3a20 626f 6f6c 0a20 2020  :rtype: bool.   
+00014b40: 2020 2020 2022 2222 0a20 2020 2020 2020       """.       
+00014b50: 2069 6620 6f74 6865 722e 6465 7269 7665   if other.derive
+00014b60: 645f 6672 6f6d 5f6f 7020 616e 6420 6f74  d_from_op and ot
+00014b70: 6865 722e 6465 7269 7665 645f 6672 6f6d  her.derived_from
+00014b80: 5f6f 702e 6b69 6e64 203d 3d20 226d 756c  _op.kind == "mul
+00014b90: 223a 0a20 2020 2020 2020 2020 2020 2074  ":.            t
+00014ba0: 6d70 203d 2073 656c 662e 636f 7079 2829  mp = self.copy()
+00014bb0: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00014bc0: 2074 6572 6d20 696e 206f 7468 6572 2e64   term in other.d
+00014bd0: 6572 6976 6564 5f66 726f 6d5f 6f70 2e69  erived_from_op.i
+00014be0: 6e70 7574 7320 6966 2072 6967 6874 2065  nputs if right e
+00014bf0: 6c73 6520 7265 7665 7273 6564 286f 7468  lse reversed(oth
+00014c00: 6572 2e64 6572 6976 6564 5f66 726f 6d5f  er.derived_from_
+00014c10: 6f70 2e69 6e70 7574 7329 3a0a 2020 2020  op.inputs):.    
+00014c20: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+00014c30: 6f74 2074 6d70 2e63 616e 5f73 696d 706c  ot tmp.can_simpl
+00014c40: 6966 7928 7465 726d 2c20 6b69 6e64 3d6b  ify(term, kind=k
+00014c50: 696e 642c 2072 6967 6874 3d72 6967 6874  ind, right=right
+00014c60: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+00014c70: 2020 2020 2020 2072 6574 7572 6e20 4661         return Fa
+00014c80: 6c73 650a 2020 2020 2020 2020 2020 2020  lse.            
+00014c90: 2020 2020 746d 702e 6578 7465 6e64 5f6d      tmp.extend_m
+00014ca0: 756c 5f64 6976 5f28 7465 726d 2c20 6b69  ul_div_(term, ki
+00014cb0: 6e64 3d6b 696e 642c 2072 6967 6874 3d72  nd=kind, right=r
+00014cc0: 6967 6874 290a 2020 2020 2020 2020 2020  ight).          
+00014cd0: 2020 7265 7475 726e 2054 7275 650a 2020    return True.  
+00014ce0: 2020 2020 2020 6964 7820 3d20 7365 6c66        idx = self
+00014cf0: 2e5f 7369 6d70 6c69 6679 5f74 6572 6d5f  ._simplify_term_
+00014d00: 6964 7828 6f74 6865 722c 206b 696e 643d  idx(other, kind=
+00014d10: 6b69 6e64 2c20 7269 6768 743d 7269 6768  kind, right=righ
+00014d20: 7429 0a20 2020 2020 2020 2072 6574 7572  t).        retur
+00014d30: 6e20 6964 7820 6973 206e 6f74 204e 6f6e  n idx is not Non
+00014d40: 650a 0a20 2020 2064 6566 205f 7369 6d70  e..    def _simp
+00014d50: 6c69 6679 5f74 6572 6d5f 6964 7828 7365  lify_term_idx(se
+00014d60: 6c66 2c20 6f74 6865 722c 206b 696e 642c  lf, other, kind,
+00014d70: 2072 6967 6874 293a 0a20 2020 2020 2020   right):.       
+00014d80: 2022 2222 0a20 2020 2020 2020 203a 7061   """.        :pa
+00014d90: 7261 6d20 4469 6d20 6f74 6865 723a 0a20  ram Dim other:. 
+00014da0: 2020 2020 2020 203a 7061 7261 6d20 7374         :param st
+00014db0: 7220 6b69 6e64 3a0a 2020 2020 2020 2020  r kind:.        
+00014dc0: 3a70 6172 616d 2062 6f6f 6c20 7269 6768  :param bool righ
+00014dd0: 743a 0a20 2020 2020 2020 203a 7265 7475  t:.        :retu
+00014de0: 726e 3a20 696e 6465 7820 6f66 2074 6572  rn: index of ter
+00014df0: 6d20 746f 2073 696d 706c 6966 790a 2020  m to simplify.  
+00014e00: 2020 2020 2020 3a72 7479 7065 3a20 696e        :rtype: in
+00014e10: 747c 4e6f 6e65 0a20 2020 2020 2020 2022  t|None.        "
+00014e20: 2222 0a20 2020 2020 2020 2069 6620 6e6f  "".        if no
+00014e30: 7420 7365 6c66 2e74 6572 6d73 3a0a 2020  t self.terms:.  
+00014e40: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00014e50: 204e 6f6e 650a 2020 2020 2020 2020 6966   None.        if
+00014e60: 206b 696e 6420 3d3d 2022 6d75 6c22 3a0a   kind == "mul":.
+00014e70: 2020 2020 2020 2020 2020 2020 2320 5765              # We
+00014e80: 2077 616e 7420 2862 202a 2061 2920 2f2f   want (b * a) //
+00014e90: 2062 2021 3d20 612e 0a20 2020 2020 2020   b != a..       
+00014ea0: 2020 2020 2023 2048 6f77 6576 6572 2c20       # However, 
+00014eb0: 7765 2077 616e 7420 6820 2a20 2832 202a  we want h * (2 *
+00014ec0: 2061 202f 2f20 6829 203d 3d20 3220 2a20   a // h) == 2 * 
+00014ed0: 612e 0a20 2020 2020 2020 2020 2020 2023  a..            #
+00014ee0: 2053 6f2c 2066 6f72 2060 6d75 6c60 2c20   So, for `mul`, 
+00014ef0: 616e 6420 6f6e 6c79 2066 6f72 2060 6d75  and only for `mu
+00014f00: 6c60 2c20 6368 6563 6b20 616c 6c20 7465  l`, check all te
+00014f10: 726d 732c 2077 6865 7468 6572 2077 6520  rms, whether we 
+00014f20: 6361 6e20 7369 6d70 6c69 6679 2073 6f6d  can simplify som
+00014f30: 6520 6469 7669 7369 6f6e 2d74 6572 6d2e  e division-term.
+00014f40: 0a20 2020 2020 2020 2020 2020 2066 6f72  .            for
+00014f50: 2069 2c20 7465 726d 2069 6e20 7265 7665   i, term in reve
+00014f60: 7273 6564 286c 6973 7428 656e 756d 6572  rsed(list(enumer
+00014f70: 6174 6528 7365 6c66 2e74 6572 6d73 2929  ate(self.terms))
+00014f80: 2920 6966 2072 6967 6874 2065 6c73 6520  ) if right else 
+00014f90: 656e 756d 6572 6174 6528 7365 6c66 2e74  enumerate(self.t
+00014fa0: 6572 6d73 293a 0a20 2020 2020 2020 2020  erms):.         
+00014fb0: 2020 2020 2020 2061 7373 6572 7420 6973         assert is
+00014fc0: 696e 7374 616e 6365 2874 6572 6d2c 205f  instance(term, _
+00014fd0: 642e 4469 6d29 0a20 2020 2020 2020 2020  d.Dim).         
+00014fe0: 2020 2020 2020 2069 6620 7465 726d 2e64         if term.d
+00014ff0: 6572 6976 6564 5f66 726f 6d5f 6f70 3a0a  erived_from_op:.
+00015000: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015010: 2020 2020 6966 2074 6572 6d2e 6465 7269      if term.deri
+00015020: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
+00015030: 203d 3d20 2274 7275 6564 6976 5f22 202b   == "truediv_" +
+00015040: 2028 2272 6967 6874 2220 6966 2072 6967   ("right" if rig
+00015050: 6874 2065 6c73 6520 226c 6566 7422 293a  ht else "left"):
+00015060: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015070: 2020 2020 2020 2020 2069 6620 7465 726d           if term
+00015080: 2e64 6572 6976 6564 5f66 726f 6d5f 6f70  .derived_from_op
+00015090: 2e69 6e70 7574 735b 2d31 5d20 3d3d 206f  .inputs[-1] == o
+000150a0: 7468 6572 3a0a 2020 2020 2020 2020 2020  ther:.          
+000150b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000150c0: 2020 7265 7475 726e 2069 0a20 2020 2020    return i.     
+000150d0: 2020 2020 2020 2020 2020 2069 6620 6f74             if ot
+000150e0: 6865 722e 6465 7269 7665 645f 6672 6f6d  her.derived_from
+000150f0: 5f6f 703a 0a20 2020 2020 2020 2020 2020  _op:.           
+00015100: 2020 2020 2020 2020 2069 6620 6f74 6865           if othe
+00015110: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
+00015120: 702e 6b69 6e64 203d 3d20 2274 7275 6564  p.kind == "trued
+00015130: 6976 5f22 202b 2028 2272 6967 6874 2220  iv_" + ("right" 
+00015140: 6966 206e 6f74 2072 6967 6874 2065 6c73  if not right els
+00015150: 6520 226c 6566 7422 293a 0a20 2020 2020  e "left"):.     
+00015160: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015170: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
+00015180: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
+00015190: 7473 5b2d 315d 203d 3d20 7465 726d 3a0a  ts[-1] == term:.
+000151a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000151b0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+000151c0: 726e 2069 0a20 2020 2020 2020 2020 2020  rn i.           
+000151d0: 2020 2020 2069 6620 7465 726d 2e69 735f       if term.is_
+000151e0: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
+000151f0: 6469 6d28 2920 616e 6420 6f74 6865 722e  dim() and other.
+00015200: 6973 5f63 6f6e 7374 616e 745f 7374 6174  is_constant_stat
+00015210: 6963 5f64 696d 2829 3a0a 2020 2020 2020  ic_dim():.      
+00015220: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00015230: 7475 726e 2069 0a20 2020 2020 2020 2023  turn i.        #
+00015240: 2046 6f72 2074 6865 206c 6173 742f 6669   For the last/fi
+00015250: 7273 7420 7465 726d 2c20 6578 7472 6120  rst term, extra 
+00015260: 6368 6563 6b73 2e0a 2020 2020 2020 2020  checks..        
+00015270: 6920 3d20 6c65 6e28 7365 6c66 2e74 6572  i = len(self.ter
+00015280: 6d73 2920 2d20 3120 6966 2072 6967 6874  ms) - 1 if right
+00015290: 2065 6c73 6520 300a 2020 2020 2020 2020   else 0.        
+000152a0: 7465 726d 203d 2073 656c 662e 7465 726d  term = self.term
+000152b0: 735b 695d 0a20 2020 2020 2020 2069 6620  s[i].        if 
+000152c0: 6b69 6e64 2e65 6e64 7377 6974 6828 2264  kind.endswith("d
+000152d0: 6976 2229 2061 6e64 206f 7468 6572 203d  iv") and other =
+000152e0: 3d20 7465 726d 3a0a 2020 2020 2020 2020  = term:.        
+000152f0: 2020 2020 7265 7475 726e 2069 0a20 2020      return i.   
+00015300: 2020 2020 206f 705f 6b69 6e64 203d 206b       op_kind = k
+00015310: 696e 6420 2b20 225f 2220 2b20 2822 7269  ind + "_" + ("ri
+00015320: 6768 7422 2069 6620 7269 6768 7420 656c  ght" if right el
+00015330: 7365 2022 6c65 6674 2229 0a20 2020 2020  se "left").     
+00015340: 2020 2069 6620 7465 726d 2e64 6572 6976     if term.deriv
+00015350: 6564 5f66 726f 6d5f 6f70 2061 6e64 2074  ed_from_op and t
+00015360: 6572 6d2e 6465 7269 7665 645f 6672 6f6d  erm.derived_from
+00015370: 5f6f 702e 6b69 6e64 203d 3d20 6f70 5f6b  _op.kind == op_k
+00015380: 696e 643a 0a20 2020 2020 2020 2020 2020  ind:.           
+00015390: 2072 6574 7572 6e20 690a 2020 2020 2020   return i.      
+000153a0: 2020 7265 7475 726e 204e 6f6e 650a 0a20    return None.. 
+000153b0: 2020 2064 6566 2065 7874 656e 645f 6d75     def extend_mu
+000153c0: 6c5f 6469 765f 2873 656c 662c 206f 7468  l_div_(self, oth
+000153d0: 6572 2c20 6b69 6e64 2c20 7269 6768 7429  er, kind, right)
+000153e0: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+000153f0: 2020 2020 2020 3a70 6172 616d 2044 696d        :param Dim
+00015400: 206f 7468 6572 3a0a 2020 2020 2020 2020   other:.        
+00015410: 3a70 6172 616d 2073 7472 206b 696e 643a  :param str kind:
+00015420: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00015430: 626f 6f6c 2072 6967 6874 3a0a 2020 2020  bool right:.    
+00015440: 2020 2020 2222 220a 2020 2020 2020 2020      """.        
+00015450: 6173 7365 7274 206b 696e 6420 696e 207b  assert kind in {
+00015460: 226d 756c 222c 2022 666c 6f6f 7264 6976  "mul", "floordiv
+00015470: 222c 2022 7472 7565 6469 7622 2c20 2263  ", "truediv", "c
+00015480: 6569 6c64 6976 227d 0a20 2020 2020 2020  eildiv"}.       
+00015490: 2069 6620 6f74 6865 722e 6973 5f63 6f6e   if other.is_con
+000154a0: 7374 616e 745f 7374 6174 6963 5f64 696d  stant_static_dim
+000154b0: 2829 2061 6e64 206f 7468 6572 2e64 696d  () and other.dim
+000154c0: 656e 7369 6f6e 203d 3d20 313a 0a20 2020  ension == 1:.   
+000154d0: 2020 2020 2020 2020 2072 6574 7572 6e0a           return.
+000154e0: 2020 2020 2020 2020 6966 206e 6f74 2073          if not s
+000154f0: 656c 662e 7465 726d 733a 0a20 2020 2020  elf.terms:.     
+00015500: 2020 2020 2020 2069 6620 6b69 6e64 203d         if kind =
+00015510: 3d20 226d 756c 223a 0a20 2020 2020 2020  = "mul":.       
+00015520: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+00015530: 726d 732e 6170 7065 6e64 286f 7468 6572  rms.append(other
+00015540: 290a 2020 2020 2020 2020 2020 2020 656c  ).            el
+00015550: 6966 206b 696e 642e 656e 6473 7769 7468  if kind.endswith
+00015560: 2822 6469 7622 293a 0a20 2020 2020 2020  ("div"):.       
+00015570: 2020 2020 2020 2020 2073 656c 662e 7465           self.te
+00015580: 726d 7320 3d20 5b5f 4f70 4d75 6c74 5465  rms = [_OpMultTe
+00015590: 726d 2e6e 6577 5f64 6976 5f64 696d 2873  rm.new_div_dim(s
+000155a0: 656c 662e 6173 5f64 696d 2829 2c20 6f74  elf.as_dim(), ot
+000155b0: 6865 722c 206b 696e 643d 6b69 6e64 2c20  her, kind=kind, 
+000155c0: 7269 6768 743d 7269 6768 7429 5d0a 2020  right=right)].  
+000155d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000155e0: 0a20 2020 2020 2020 2069 6620 6f74 6865  .        if othe
+000155f0: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
+00015600: 7020 616e 6420 6f74 6865 722e 6465 7269  p and other.deri
+00015610: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
+00015620: 203d 3d20 226d 756c 223a 0a20 2020 2020   == "mul":.     
+00015630: 2020 2020 2020 2066 6f72 2074 6572 6d20         for term 
+00015640: 696e 206f 7468 6572 2e64 6572 6976 6564  in other.derived
+00015650: 5f66 726f 6d5f 6f70 2e69 6e70 7574 7320  _from_op.inputs 
+00015660: 6966 2072 6967 6874 2065 6c73 6520 7265  if right else re
+00015670: 7665 7273 6564 286f 7468 6572 2e64 6572  versed(other.der
+00015680: 6976 6564 5f66 726f 6d5f 6f70 2e69 6e70  ived_from_op.inp
+00015690: 7574 7329 3a0a 2020 2020 2020 2020 2020  uts):.          
+000156a0: 2020 2020 2020 7365 6c66 2e65 7874 656e        self.exten
+000156b0: 645f 6d75 6c5f 6469 765f 2874 6572 6d2c  d_mul_div_(term,
+000156c0: 206b 696e 643d 6b69 6e64 2c20 7269 6768   kind=kind, righ
+000156d0: 743d 7269 6768 7429 0a20 2020 2020 2020  t=right).       
+000156e0: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+000156f0: 2020 2020 6964 7820 3d20 7365 6c66 2e5f      idx = self._
+00015700: 7369 6d70 6c69 6679 5f74 6572 6d5f 6964  simplify_term_id
+00015710: 7828 6f74 6865 722c 206b 696e 643d 6b69  x(other, kind=ki
+00015720: 6e64 2c20 7269 6768 743d 7269 6768 7429  nd, right=right)
+00015730: 0a20 2020 2020 2020 2069 6620 6964 7820  .        if idx 
+00015740: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00015750: 2020 2020 2020 2020 2074 6572 6d20 3d20           term = 
+00015760: 7365 6c66 2e74 6572 6d73 5b69 6478 5d0a  self.terms[idx].
+00015770: 2020 2020 2020 2020 2020 2020 6173 7365              asse
+00015780: 7274 2069 7369 6e73 7461 6e63 6528 7465  rt isinstance(te
+00015790: 726d 2c20 5f64 2e44 696d 290a 2020 2020  rm, _d.Dim).    
+000157a0: 2020 2020 2020 2020 6966 206b 696e 642e          if kind.
+000157b0: 656e 6473 7769 7468 2822 6469 7622 2920  endswith("div") 
+000157c0: 616e 6420 6f74 6865 7220 3d3d 2074 6572  and other == ter
+000157d0: 6d3a 0a20 2020 2020 2020 2020 2020 2020  m:.             
+000157e0: 2020 2073 656c 662e 7465 726d 732e 706f     self.terms.po
+000157f0: 7028 6964 7829 0a20 2020 2020 2020 2020  p(idx).         
+00015800: 2020 2020 2020 2072 6574 7572 6e0a 2020         return.  
+00015810: 2020 2020 2020 2020 2020 6966 206b 696e            if kin
+00015820: 6420 3d3d 2022 6d75 6c22 2061 6e64 2074  d == "mul" and t
+00015830: 6572 6d2e 6465 7269 7665 645f 6672 6f6d  erm.derived_from
+00015840: 5f6f 703a 0a20 2020 2020 2020 2020 2020  _op:.           
+00015850: 2020 2020 2069 6620 7465 726d 2e64 6572       if term.der
+00015860: 6976 6564 5f66 726f 6d5f 6f70 2e6b 696e  ived_from_op.kin
+00015870: 6420 3d3d 2022 7472 7565 6469 765f 2220  d == "truediv_" 
+00015880: 2b20 2822 7269 6768 7422 2069 6620 7269  + ("right" if ri
+00015890: 6768 7420 656c 7365 2022 6c65 6674 2229  ght else "left")
+000158a0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+000158b0: 2020 2020 2020 6966 2074 6572 6d2e 6465        if term.de
+000158c0: 7269 7665 645f 6672 6f6d 5f6f 702e 696e  rived_from_op.in
+000158d0: 7075 7473 5b2d 315d 203d 3d20 6f74 6865  puts[-1] == othe
+000158e0: 723a 0a20 2020 2020 2020 2020 2020 2020  r:.             
+000158f0: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00015900: 7465 726d 735b 6964 785d 203d 2074 6572  terms[idx] = ter
+00015910: 6d2e 6465 7269 7665 645f 6672 6f6d 5f6f  m.derived_from_o
+00015920: 702e 696e 7075 7473 5b30 5d0a 2020 2020  p.inputs[0].    
+00015930: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015940: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00015950: 2020 2020 2020 2069 6620 6b69 6e64 203d         if kind =
+00015960: 3d20 226d 756c 2220 616e 6420 6f74 6865  = "mul" and othe
+00015970: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
+00015980: 703a 0a20 2020 2020 2020 2020 2020 2020  p:.             
+00015990: 2020 2069 6620 6f74 6865 722e 6465 7269     if other.deri
+000159a0: 7665 645f 6672 6f6d 5f6f 702e 6b69 6e64  ved_from_op.kind
+000159b0: 203d 3d20 2274 7275 6564 6976 5f22 202b   == "truediv_" +
+000159c0: 2028 2272 6967 6874 2220 6966 206e 6f74   ("right" if not
+000159d0: 2072 6967 6874 2065 6c73 6520 226c 6566   right else "lef
+000159e0: 7422 293a 0a20 2020 2020 2020 2020 2020  t"):.           
+000159f0: 2020 2020 2020 2020 2069 6620 6f74 6865           if othe
+00015a00: 722e 6465 7269 7665 645f 6672 6f6d 5f6f  r.derived_from_o
+00015a10: 702e 696e 7075 7473 5b2d 315d 203d 3d20  p.inputs[-1] == 
+00015a20: 7465 726d 3a0a 2020 2020 2020 2020 2020  term:.          
+00015a30: 2020 2020 2020 2020 2020 2020 2020 7365                se
+00015a40: 6c66 2e74 6572 6d73 5b69 6478 5d20 3d20  lf.terms[idx] = 
+00015a50: 6f74 6865 722e 6465 7269 7665 645f 6672  other.derived_fr
+00015a60: 6f6d 5f6f 702e 696e 7075 7473 5b30 5d0a  om_op.inputs[0].
+00015a70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015a80: 2020 2020 2020 2020 7265 7475 726e 0a20          return. 
+00015a90: 2020 2020 2020 2020 2020 2069 6620 7465             if te
+00015aa0: 726d 2e69 735f 636f 6e73 7461 6e74 5f73  rm.is_constant_s
+00015ab0: 7461 7469 635f 6469 6d28 2920 616e 6420  tatic_dim() and 
+00015ac0: 6f74 6865 722e 6973 5f63 6f6e 7374 616e  other.is_constan
+00015ad0: 745f 7374 6174 6963 5f64 696d 2829 3a0a  t_static_dim():.
+00015ae0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015af0: 6966 206b 696e 6420 3d3d 2022 6d75 6c22  if kind == "mul"
+00015b00: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00015b10: 2020 2020 2020 6966 2074 6572 6d2e 6469        if term.di
+00015b20: 6d65 6e73 696f 6e20 2a20 6f74 6865 722e  mension * other.
+00015b30: 6469 6d65 6e73 696f 6e20 3d3d 2031 3a0a  dimension == 1:.
+00015b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b50: 2020 2020 2020 2020 7365 6c66 2e74 6572          self.ter
+00015b60: 6d73 2e70 6f70 2869 6478 290a 2020 2020  ms.pop(idx).    
+00015b70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015b80: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00015b90: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015ba0: 656c 662e 7465 726d 735b 6964 785d 203d  elf.terms[idx] =
+00015bb0: 205f 6d61 6b65 5f63 6f6e 7374 616e 745f   _make_constant_
+00015bc0: 7374 6174 6963 5f64 696d 2874 6572 6d2e  static_dim(term.
+00015bd0: 6469 6d65 6e73 696f 6e20 2a20 6f74 6865  dimension * othe
+00015be0: 722e 6469 6d65 6e73 696f 6e2c 206b 696e  r.dimension, kin
+00015bf0: 643d 7465 726d 2e6b 696e 6429 0a20 2020  d=term.kind).   
+00015c00: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015c10: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00015c20: 2020 2020 2020 2020 6966 206b 696e 642e          if kind.
+00015c30: 656e 6473 7769 7468 2822 6469 7622 2920  endswith("div") 
+00015c40: 616e 6420 7465 726d 2e64 696d 656e 7369  and term.dimensi
+00015c50: 6f6e 2025 206f 7468 6572 2e64 696d 656e  on % other.dimen
+00015c60: 7369 6f6e 203d 3d20 303a 0a20 2020 2020  sion == 0:.     
+00015c70: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00015c80: 656c 662e 7465 726d 735b 6964 785d 203d  elf.terms[idx] =
+00015c90: 205f 6d61 6b65 5f63 6f6e 7374 616e 745f   _make_constant_
+00015ca0: 7374 6174 6963 5f64 696d 2874 6572 6d2e  static_dim(term.
+00015cb0: 6469 6d65 6e73 696f 6e20 2f2f 206f 7468  dimension // oth
+00015cc0: 6572 2e64 696d 656e 7369 6f6e 2c20 6b69  er.dimension, ki
+00015cd0: 6e64 3d74 6572 6d2e 6b69 6e64 290a 2020  nd=term.kind).  
+00015ce0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015cf0: 2020 7265 7475 726e 0a20 2020 2020 2020    return.       
+00015d00: 2020 2020 2020 2020 2023 2046 616c 6c62           # Fallb
+00015d10: 6163 6b20 7769 7468 2067 656e 6572 6963  ack with generic
+00015d20: 2068 616e 646c 696e 672e 0a20 2020 2020   handling..     
+00015d30: 2020 2020 2020 206f 705f 6b69 6e64 203d         op_kind =
+00015d40: 206b 696e 6420 2b20 225f 2220 2b20 2822   kind + "_" + ("
+00015d50: 7269 6768 7422 2069 6620 7269 6768 7420  right" if right 
+00015d60: 656c 7365 2022 6c65 6674 2229 0a20 2020  else "left").   
+00015d70: 2020 2020 2020 2020 2069 6620 6b69 6e64           if kind
+00015d80: 2e65 6e64 7377 6974 6828 2264 6976 2229  .endswith("div")
+00015d90: 2061 6e64 2074 6572 6d2e 6465 7269 7665   and term.derive
+00015da0: 645f 6672 6f6d 5f6f 7020 616e 6420 7465  d_from_op and te
+00015db0: 726d 2e64 6572 6976 6564 5f66 726f 6d5f  rm.derived_from_
+00015dc0: 6f70 2e6b 696e 6420 3d3d 206f 705f 6b69  op.kind == op_ki
+00015dd0: 6e64 3a0a 2020 2020 2020 2020 2020 2020  nd:.            
+00015de0: 2020 2020 6e75 6d65 7261 746f 7220 3d20      numerator = 
+00015df0: 7465 726d 2e64 6572 6976 6564 5f66 726f  term.derived_fro
+00015e00: 6d5f 6f70 2e69 6e70 7574 735b 305d 0a20  m_op.inputs[0]. 
+00015e10: 2020 2020 2020 2020 2020 2020 2020 2064                 d
+00015e20: 656e 6f6d 696e 6174 6f72 203d 2074 6572  enominator = ter
+00015e30: 6d2e 6465 7269 7665 645f 6672 6f6d 5f6f  m.derived_from_o
+00015e40: 702e 696e 7075 7473 5b31 5d0a 2020 2020  p.inputs[1].    
+00015e50: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00015e60: 2e74 6572 6d73 5b69 6478 5d20 3d20 5f4f  .terms[idx] = _O
+00015e70: 704d 756c 7454 6572 6d2e 6e65 775f 6469  pMultTerm.new_di
+00015e80: 765f 6469 6d28 6e75 6d65 7261 746f 722c  v_dim(numerator,
+00015e90: 2064 656e 6f6d 696e 6174 6f72 202a 206f   denominator * o
+00015ea0: 7468 6572 2c20 6b69 6e64 3d6b 696e 642c  ther, kind=kind,
+00015eb0: 2072 6967 6874 3d72 6967 6874 290a 2020   right=right).  
+00015ec0: 2020 2020 2020 2020 2020 2020 2020 7265                re
+00015ed0: 7475 726e 0a20 2020 2020 2020 2069 6620  turn.        if 
+00015ee0: 6b69 6e64 2e65 6e64 7377 6974 6828 2264  kind.endswith("d
+00015ef0: 6976 2229 3a0a 2020 2020 2020 2020 2020  iv"):.          
+00015f00: 2020 7365 6c66 2e74 6572 6d73 203d 205b    self.terms = [
+00015f10: 5f4f 704d 756c 7454 6572 6d2e 6e65 775f  _OpMultTerm.new_
+00015f20: 6469 765f 6469 6d28 7365 6c66 2e61 735f  div_dim(self.as_
+00015f30: 6469 6d28 292c 206f 7468 6572 2c20 6b69  dim(), other, ki
+00015f40: 6e64 3d6b 696e 642c 2072 6967 6874 3d72  nd=kind, right=r
+00015f50: 6967 6874 295d 0a20 2020 2020 2020 2020  ight)].         
+00015f60: 2020 2072 6574 7572 6e0a 2020 2020 2020     return.      
+00015f70: 2020 6966 206b 696e 6420 3d3d 2022 6d75    if kind == "mu
+00015f80: 6c22 3a0a 2020 2020 2020 2020 2020 2020  l":.            
+00015f90: 6966 2072 6967 6874 3a0a 2020 2020 2020  if right:.      
+00015fa0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00015fb0: 6572 6d73 2e61 7070 656e 6428 6f74 6865  erms.append(othe
+00015fc0: 7229 0a20 2020 2020 2020 2020 2020 2065  r).            e
+00015fd0: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
+00015fe0: 2020 2020 2073 656c 662e 7465 726d 732e       self.terms.
+00015ff0: 696e 7365 7274 2830 2c20 6f74 6865 7229  insert(0, other)
+00016000: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+00016010: 7572 6e0a 2020 2020 2020 2020 6173 7365  urn.        asse
+00016020: 7274 2046 616c 7365 0a0a 2020 2020 4063  rt False..    @c
+00016030: 6c61 7373 6d65 7468 6f64 0a20 2020 2064  lassmethod.    d
+00016040: 6566 206e 6577 5f64 6976 5f64 696d 2863  ef new_div_dim(c
+00016050: 6c73 2c20 6e75 6d65 7261 746f 722c 2064  ls, numerator, d
+00016060: 656e 6f6d 696e 6174 6f72 2c20 6b69 6e64  enominator, kind
+00016070: 2c20 7269 6768 7429 3a0a 2020 2020 2020  , right):.      
+00016080: 2020 2222 220a 2020 2020 2020 2020 3a70    """.        :p
+00016090: 6172 616d 2044 696d 206e 756d 6572 6174  aram Dim numerat
+000160a0: 6f72 3a0a 2020 2020 2020 2020 3a70 6172  or:.        :par
+000160b0: 616d 2044 696d 2064 656e 6f6d 696e 6174  am Dim denominat
+000160c0: 6f72 3a0a 2020 2020 2020 2020 3a70 6172  or:.        :par
+000160d0: 616d 2073 7472 206b 696e 643a 2022 666c  am str kind: "fl
+000160e0: 6f6f 7264 6976 2220 6f72 2022 6365 696c  oordiv" or "ceil
+000160f0: 6469 7622 206f 7220 2274 7275 6564 6976  div" or "truediv
+00016100: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+00016110: 2062 6f6f 6c20 7269 6768 743a 0a20 2020   bool right:.   
+00016120: 2020 2020 203a 7274 7970 653a 2044 696d       :rtype: Dim
+00016130: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00016140: 2020 2020 2064 696d 5f76 616c 7565 203d       dim_value =
+00016150: 204e 6f6e 650a 2020 2020 2020 2020 6120   None.        a 
+00016160: 3d20 6e75 6d65 7261 746f 722e 6469 6d65  = numerator.dime
+00016170: 6e73 696f 6e0a 2020 2020 2020 2020 6220  nsion.        b 
+00016180: 3d20 6465 6e6f 6d69 6e61 746f 722e 6469  = denominator.di
+00016190: 6d65 6e73 696f 6e0a 2020 2020 2020 2020  mension.        
+000161a0: 6966 2061 2069 7320 6e6f 7420 4e6f 6e65  if a is not None
+000161b0: 2061 6e64 2062 2069 7320 6e6f 7420 4e6f   and b is not No
+000161c0: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
+000161d0: 6966 206b 696e 6420 3d3d 2022 666c 6f6f  if kind == "floo
+000161e0: 7264 6976 223a 0a20 2020 2020 2020 2020  rdiv":.         
+000161f0: 2020 2020 2020 2064 696d 5f76 616c 7565         dim_value
+00016200: 203d 2061 202f 2f20 620a 2020 2020 2020   = a // b.      
+00016210: 2020 2020 2020 656c 6966 206b 696e 6420        elif kind 
+00016220: 3d3d 2022 6365 696c 6469 7622 3a0a 2020  == "ceildiv":.  
+00016230: 2020 2020 2020 2020 2020 2020 2020 6469                di
+00016240: 6d5f 7661 6c75 6520 3d20 2d28 2d61 202f  m_value = -(-a /
+00016250: 2f20 6229 0a20 2020 2020 2020 2020 2020  / b).           
+00016260: 2020 2020 2069 6620 6120 2520 6220 3d3d       if a % b ==
+00016270: 2030 2061 6e64 2072 6967 6874 3a0a 2020   0 and right:.  
+00016280: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016290: 2020 6b69 6e64 203d 2022 666c 6f6f 7264    kind = "floord
+000162a0: 6976 2220 2023 2066 6f72 206e 6963 6572  iv"  # for nicer
+000162b0: 2064 6573 6372 6970 7469 6f6e 2c20 616e   description, an
+000162c0: 6420 646f 6573 206e 6f74 206d 6174 7465  d does not matte
+000162d0: 720a 2020 2020 2020 2020 2020 2020 656c  r.            el
+000162e0: 6966 206b 696e 6420 3d3d 2022 7472 7565  if kind == "true
+000162f0: 6469 7622 3a0a 2020 2020 2020 2020 2020  div":.          
+00016300: 2020 2020 2020 6966 2061 2025 2062 2021        if a % b !
+00016310: 3d20 303a 0a20 2020 2020 2020 2020 2020  = 0:.           
+00016320: 2020 2020 2020 2020 2072 6169 7365 2056           raise V
+00016330: 616c 7565 4572 726f 7228 0a20 2020 2020  alueError(.     
+00016340: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016350: 2020 2022 2573 2074 7275 6564 6976 2025     "%s truediv %
+00016360: 7320 6f6e 6c79 2061 6c6c 6f77 6564 2069  s only allowed i
+00016370: 6620 7468 6520 7265 7375 6c74 2069 7320  f the result is 
+00016380: 616e 2069 6e74 6567 6572 2220 2520 286e  an integer" % (n
+00016390: 756d 6572 6174 6f72 2c20 6465 6e6f 6d69  umerator, denomi
+000163a0: 6e61 746f 7229 0a20 2020 2020 2020 2020  nator).         
+000163b0: 2020 2020 2020 2020 2020 2029 0a20 2020             ).   
+000163c0: 2020 2020 2020 2020 2020 2020 2064 696d               dim
+000163d0: 5f76 616c 7565 203d 2061 202f 2f20 620a  _value = a // b.
+000163e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000163f0: 6966 2072 6967 6874 3a0a 2020 2020 2020  if right:.      
+00016400: 2020 2020 2020 2020 2020 2020 2020 6b69                ki
+00016410: 6e64 203d 2022 666c 6f6f 7264 6976 2220  nd = "floordiv" 
+00016420: 2023 2066 6f72 206e 6963 6572 2064 6573   # for nicer des
+00016430: 6372 6970 7469 6f6e 2c20 616e 6420 646f  cription, and do
+00016440: 6573 206e 6f74 206d 6174 7465 720a 2020  es not matter.  
+00016450: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
+00016460: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00016470: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
+00016480: 2822 696e 7661 6c69 6420 6b69 6e64 2025  ("invalid kind %
+00016490: 7222 2025 2028 6b69 6e64 2c29 290a 2020  r" % (kind,)).  
+000164a0: 2020 2020 2020 6966 206b 696e 6420 3d3d        if kind ==
+000164b0: 2022 666c 6f6f 7264 6976 2220 616e 6420   "floordiv" and 
+000164c0: 7269 6768 743a 0a20 2020 2020 2020 2020  right:.         
+000164d0: 2020 2064 6573 6372 6970 7469 6f6e 203d     description =
+000164e0: 2022 2573 2f2f 2573 2220 2520 285f 6765   "%s//%s" % (_ge
+000164f0: 745f 6465 7363 7269 7074 696f 6e28 6e75  t_description(nu
+00016500: 6d65 7261 746f 7229 2c20 5f67 6574 5f64  merator), _get_d
+00016510: 6573 6372 6970 7469 6f6e 2864 656e 6f6d  escription(denom
+00016520: 696e 6174 6f72 2929 0a20 2020 2020 2020  inator)).       
+00016530: 2065 6c69 6620 6b69 6e64 203d 3d20 2263   elif kind == "c
+00016540: 6569 6c64 6976 2220 616e 6420 7269 6768  eildiv" and righ
+00016550: 743a 0a20 2020 2020 2020 2020 2020 2064  t:.            d
+00016560: 6573 6372 6970 7469 6f6e 203d 2022 e28c  escription = "..
+00016570: 8825 732f 2573 e28c 8922 2025 2028 5f67  .%s/%s..." % (_g
+00016580: 6574 5f64 6573 6372 6970 7469 6f6e 286e  et_description(n
+00016590: 756d 6572 6174 6f72 292c 205f 6765 745f  umerator), _get_
+000165a0: 6465 7363 7269 7074 696f 6e28 6465 6e6f  description(deno
+000165b0: 6d69 6e61 746f 7229 290a 2020 2020 2020  minator)).      
+000165c0: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
+000165d0: 2020 2020 6465 7363 7269 7074 696f 6e20      description 
+000165e0: 3d20 2225 735f 2573 2825 732c 2025 7329  = "%s_%s(%s, %s)
+000165f0: 2220 2520 280a 2020 2020 2020 2020 2020  " % (.          
+00016600: 2020 2020 2020 6b69 6e64 2c0a 2020 2020        kind,.    
+00016610: 2020 2020 2020 2020 2020 2020 2272 6967              "rig
+00016620: 6874 2220 6966 2072 6967 6874 2065 6c73  ht" if right els
+00016630: 6520 226c 6566 7422 2c0a 2020 2020 2020  e "left",.      
+00016640: 2020 2020 2020 2020 2020 5f67 6574 5f64            _get_d
+00016650: 6573 6372 6970 7469 6f6e 286e 756d 6572  escription(numer
+00016660: 6174 6f72 2c20 6272 6163 6b65 7473 3d46  ator, brackets=F
+00016670: 616c 7365 292c 0a20 2020 2020 2020 2020  alse),.         
+00016680: 2020 2020 2020 205f 6765 745f 6465 7363         _get_desc
+00016690: 7269 7074 696f 6e28 6465 6e6f 6d69 6e61  ription(denomina
+000166a0: 746f 722c 2062 7261 636b 6574 733d 4661  tor, brackets=Fa
+000166b0: 6c73 6529 2c0a 2020 2020 2020 2020 2020  lse),.          
+000166c0: 2020 290a 2020 2020 2020 2020 6f70 5f6b    ).        op_k
+000166d0: 696e 6420 3d20 6b69 6e64 0a20 2020 2020  ind = kind.     
+000166e0: 2020 2069 6620 6120 6973 206e 6f74 204e     if a is not N
+000166f0: 6f6e 6520 616e 6420 6220 6973 206e 6f74  one and b is not
+00016700: 204e 6f6e 6520 616e 6420 6120 2520 6220   None and a % b 
+00016710: 3d3d 2030 3a0a 2020 2020 2020 2020 2020  == 0:.          
+00016720: 2020 6f70 5f6b 696e 6420 3d20 2274 7275    op_kind = "tru
+00016730: 6564 6976 2220 2023 206d 616b 6573 2073  ediv"  # makes s
+00016740: 6f6d 6520 6f74 6865 7220 6368 6563 6b73  ome other checks
+00016750: 2073 696d 706c 6572 0a20 2020 2020 2020   simpler.       
+00016760: 206f 705f 6b69 6e64 202b 3d20 225f 2220   op_kind += "_" 
+00016770: 2b20 2822 7269 6768 7422 2069 6620 7269  + ("right" if ri
+00016780: 6768 7420 656c 7365 2022 6c65 6674 2229  ght else "left")
+00016790: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000167a0: 5f64 2e44 696d 280a 2020 2020 2020 2020  _d.Dim(.        
+000167b0: 2020 2020 6465 7363 7269 7074 696f 6e3d      description=
+000167c0: 6465 7363 7269 7074 696f 6e2c 0a20 2020  description,.   
+000167d0: 2020 2020 2020 2020 206b 696e 643d 6e75           kind=nu
+000167e0: 6d65 7261 746f 722e 6b69 6e64 2c0a 2020  merator.kind,.  
+000167f0: 2020 2020 2020 2020 2020 6469 6d65 6e73            dimens
+00016800: 696f 6e3d 6469 6d5f 7661 6c75 652c 0a20  ion=dim_value,. 
+00016810: 2020 2020 2020 2020 2020 2064 6572 6976             deriv
+00016820: 6564 5f66 726f 6d5f 6f70 3d4f 7028 6b69  ed_from_op=Op(ki
+00016830: 6e64 3d6f 705f 6b69 6e64 2c20 696e 7075  nd=op_kind, inpu
+00016840: 7473 3d5b 6e75 6d65 7261 746f 722c 2064  ts=[numerator, d
+00016850: 656e 6f6d 696e 6174 6f72 5d29 2c0a 2020  enominator]),.  
+00016860: 2020 2020 2020 2020 2020 6465 7269 7665            derive
+00016870: 645f 6672 6f6d 5f74 6167 3d6e 756d 6572  d_from_tag=numer
+00016880: 6174 6f72 2c0a 2020 2020 2020 2020 290a  ator,.        ).
+00016890: 0a20 2020 2064 6566 2061 735f 6469 6d28  .    def as_dim(
+000168a0: 7365 6c66 293a 0a20 2020 2020 2020 2022  self):.        "
+000168b0: 2222 0a20 2020 2020 2020 203a 7274 7970  "".        :rtyp
+000168c0: 653a 2044 696d 0a20 2020 2020 2020 2022  e: Dim.        "
+000168d0: 2222 0a20 2020 2020 2020 2069 6620 7365  "".        if se
+000168e0: 6c66 2e69 735f 6f6e 6528 293a 0a20 2020  lf.is_one():.   
+000168f0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00016900: 5f6d 616b 655f 636f 6e73 7461 6e74 5f73  _make_constant_s
+00016910: 7461 7469 635f 6469 6d28 3129 0a20 2020  tatic_dim(1).   
+00016920: 2020 2020 2069 6620 6c65 6e28 7365 6c66       if len(self
+00016930: 2e74 6572 6d73 2920 3d3d 2031 3a0a 2020  .terms) == 1:.  
+00016940: 2020 2020 2020 2020 2020 7265 7475 726e            return
+00016950: 2073 656c 662e 7465 726d 735b 305d 0a20   self.terms[0]. 
+00016960: 2020 2020 2020 2064 696d 5f6b 696e 6420         dim_kind 
+00016970: 3d20 5f67 6574 5f6d 6572 6765 645f 6469  = _get_merged_di
+00016980: 6d5f 6b69 6e64 2873 656c 662e 7465 726d  m_kind(self.term
+00016990: 7329 0a20 2020 2020 2020 2072 6574 7572  s).        retur
+000169a0: 6e20 5f64 2e44 696d 280a 2020 2020 2020  n _d.Dim(.      
+000169b0: 2020 2020 2020 6b69 6e64 3d64 696d 5f6b        kind=dim_k
+000169c0: 696e 642c 0a20 2020 2020 2020 2020 2020  ind,.           
+000169d0: 2064 6573 6372 6970 7469 6f6e 3d22 2a22   description="*"
+000169e0: 2e6a 6f69 6e28 6d61 7028 5f67 6574 5f64  .join(map(_get_d
+000169f0: 6573 6372 6970 7469 6f6e 2c20 7365 6c66  escription, self
+00016a00: 2e74 6572 6d73 2929 2c0a 2020 2020 2020  .terms)),.      
+00016a10: 2020 2020 2020 6469 6d65 6e73 696f 6e3d        dimension=
+00016a20: 7365 6c66 2e64 696d 656e 7369 6f6e 2c0a  self.dimension,.
+00016a30: 2020 2020 2020 2020 2020 2020 6465 7269              deri
+00016a40: 7665 645f 6672 6f6d 5f6f 703d 4f70 286b  ved_from_op=Op(k
+00016a50: 696e 643d 226d 756c 222c 2069 6e70 7574  ind="mul", input
+00016a60: 733d 6c69 7374 2873 656c 662e 7465 726d  s=list(self.term
+00016a70: 7329 292c 0a20 2020 2020 2020 2020 2020  s)),.           
+00016a80: 2064 6572 6976 6564 5f66 726f 6d5f 7461   derived_from_ta
+00016a90: 673d 7365 6c66 2e72 6570 7265 7365 6e74  g=self.represent
+00016aa0: 6174 6976 655f 7461 6728 292c 0a20 2020  ative_tag(),.   
+00016ab0: 2020 2020 2029 0a0a 2020 2020 6465 6620       )..    def 
+00016ac0: 7265 7072 6573 656e 7461 7469 7665 5f74  representative_t
+00016ad0: 6167 2873 656c 6629 3a0a 2020 2020 2020  ag(self):.      
+00016ae0: 2020 2222 220a 2020 2020 2020 2020 3a72    """.        :r
+00016af0: 7479 7065 3a20 4469 6d7c 4e6f 6e65 0a20  type: Dim|None. 
+00016b00: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+00016b10: 2020 2023 2041 6c73 6f20 7365 6520 4469     # Also see Di
+00016b20: 6d2e 5f4f 704c 696e 6561 7254 6572 6d2e  m._OpLinearTerm.
+00016b30: 7265 7072 6573 656e 7461 7469 7665 5f74  representative_t
+00016b40: 6167 2829 2e0a 2020 2020 2020 2020 2320  ag()..        # 
+00016b50: 4669 7273 7420 6669 6e64 2061 6e79 2064  First find any d
+00016b60: 796e 616d 6963 2e0a 2020 2020 2020 2020  ynamic..        
+00016b70: 666f 7220 7465 726d 5f20 696e 2073 656c  for term_ in sel
+00016b80: 662e 7465 726d 733a 0a20 2020 2020 2020  f.terms:.       
+00016b90: 2020 2020 2069 6620 7465 726d 5f2e 6973       if term_.is
+00016ba0: 5f64 796e 616d 6963 2829 3a0a 2020 2020  _dynamic():.    
+00016bb0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00016bc0: 726e 2074 6572 6d5f 0a20 2020 2020 2020  rn term_.       
+00016bd0: 2023 204e 6f77 2066 696e 6420 6e6f 6e2d   # Now find non-
+00016be0: 756e 7370 6563 6966 6965 642e 0a20 2020  unspecified..   
+00016bf0: 2020 2020 2066 6f72 2074 6572 6d5f 2069       for term_ i
+00016c00: 6e20 7365 6c66 2e74 6572 6d73 3a0a 2020  n self.terms:.  
+00016c10: 2020 2020 2020 2020 2020 6966 2074 6572            if ter
+00016c20: 6d5f 2e6b 696e 6420 213d 2044 696d 5479  m_.kind != DimTy
+00016c30: 7065 732e 556e 7370 6563 6966 6965 643a  pes.Unspecified:
+00016c40: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016c50: 2072 6574 7572 6e20 7465 726d 5f0a 2020   return term_.  
+00016c60: 2020 2020 2020 2320 4e6f 7720 6669 6e64        # Now find
+00016c70: 2061 6e79 2e0a 2020 2020 2020 2020 666f   any..        fo
+00016c80: 7220 7465 726d 5f20 696e 2073 656c 662e  r term_ in self.
+00016c90: 7465 726d 733a 0a20 2020 2020 2020 2020  terms:.         
+00016ca0: 2020 2072 6574 7572 6e20 7465 726d 5f0a     return term_.
+00016cb0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+00016cc0: 6f6e 650a 0a0a 636c 6173 7320 5f4f 704c  one...class _OpL
+00016cd0: 696e 6561 7254 6572 6d3a 0a20 2020 2022  inearTerm:.    "
+00016ce0: 2222 0a20 2020 2072 6570 7265 7365 6e74  "".    represent
+00016cf0: 7320 7374 6820 6c69 6b65 2061 202a 2062  s sth like a * b
+00016d00: 202b 2063 0a20 2020 2022 2222 0a0a 2020   + c.    """..  
+00016d10: 2020 4063 6c61 7373 6d65 7468 6f64 0a20    @classmethod. 
+00016d20: 2020 2064 6566 2066 726f 6d5f 6469 6d28     def from_dim(
+00016d30: 636c 732c 2064 696d 293a 0a20 2020 2020  cls, dim):.     
+00016d40: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00016d50: 7061 7261 6d20 4469 6d20 6469 6d3a 0a20  param Dim dim:. 
+00016d60: 2020 2020 2020 203a 7274 7970 653a 2044         :rtype: D
+00016d70: 696d 2e5f 4f70 4c69 6e65 6172 5465 726d  im._OpLinearTerm
+00016d80: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00016d90: 2020 2020 2072 6573 203d 2063 6c73 2e7a       res = cls.z
+00016da0: 6572 6f28 290a 2020 2020 2020 2020 7265  ero().        re
+00016db0: 732e 6578 7465 6e64 5f61 6464 5f73 7562  s.extend_add_sub
+00016dc0: 5f28 6469 6d2c 206b 696e 643d 2261 6464  _(dim, kind="add
+00016dd0: 222c 2072 6967 6874 3d54 7275 6529 0a20  ", right=True). 
+00016de0: 2020 2020 2020 2072 6574 7572 6e20 7265         return re
+00016df0: 730a 0a20 2020 2040 636c 6173 736d 6574  s..    @classmet
+00016e00: 686f 640a 2020 2020 6465 6620 7a65 726f  hod.    def zero
+00016e10: 2863 6c73 293a 0a20 2020 2020 2020 2022  (cls):.        "
+00016e20: 2222 0a20 2020 2020 2020 203a 7274 7970  "".        :rtyp
+00016e30: 653a 2044 696d 2e5f 4f70 4c69 6e65 6172  e: Dim._OpLinear
+00016e40: 5465 726d 0a20 2020 2020 2020 2022 2222  Term.        """
+00016e50: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00016e60: 5f4f 704c 696e 6561 7254 6572 6d28 5b5d  _OpLinearTerm([]
+00016e70: 290a 0a20 2020 2064 6566 205f 5f69 6e69  )..    def __ini
+00016e80: 745f 5f28 7365 6c66 2c20 7465 726d 7329  t__(self, terms)
+00016e90: 3a0a 2020 2020 2020 2020 2222 220a 2020  :.        """.  
+00016ea0: 2020 2020 2020 3a70 6172 616d 206c 6973        :param lis
+00016eb0: 745b 4469 6d2e 5f4f 704d 756c 7454 6572  t[Dim._OpMultTer
+00016ec0: 6d5d 2074 6572 6d73 3a0a 2020 2020 2020  m] terms:.      
+00016ed0: 2020 2222 220a 2020 2020 2020 2020 7365    """.        se
+00016ee0: 6c66 2e74 6572 6d73 203d 2074 6572 6d73  lf.terms = terms
+00016ef0: 0a0a 2020 2020 6465 6620 5f5f 6861 7368  ..    def __hash
+00016f00: 5f5f 2873 656c 6629 3a0a 2020 2020 2020  __(self):.      
+00016f10: 2020 7265 7475 726e 2068 6173 6828 7475    return hash(tu
+00016f20: 706c 6528 7365 6c66 2e74 6572 6d73 2929  ple(self.terms))
+00016f30: 0a0a 2020 2020 6465 6620 5f5f 6571 5f5f  ..    def __eq__
+00016f40: 2873 656c 662c 206f 7468 6572 293a 0a20  (self, other):. 
+00016f50: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
+00016f60: 616e 6365 286f 7468 6572 2c20 5f4f 704c  ance(other, _OpL
+00016f70: 696e 6561 7254 6572 6d29 3a0a 2020 2020  inearTerm):.    
+00016f80: 2020 2020 2020 2020 7265 7475 726e 2073          return s
+00016f90: 656c 662e 7465 726d 7320 3d3d 206f 7468  elf.terms == oth
+00016fa0: 6572 2e74 6572 6d73 0a20 2020 2020 2020  er.terms.       
+00016fb0: 2072 6574 7572 6e20 4661 6c73 650a 0a20   return False.. 
+00016fc0: 2020 2064 6566 205f 5f6e 655f 5f28 7365     def __ne__(se
+00016fd0: 6c66 2c20 6f74 6865 7229 3a0a 2020 2020  lf, other):.    
+00016fe0: 2020 2020 7265 7475 726e 206e 6f74 2073      return not s
+00016ff0: 656c 662e 5f5f 6571 5f5f 286f 7468 6572  elf.__eq__(other
+00017000: 290a 0a20 2020 2064 6566 2061 735f 6469  )..    def as_di
+00017010: 6d28 7365 6c66 293a 0a20 2020 2020 2020  m(self):.       
+00017020: 2022 2222 0a20 2020 2020 2020 203a 7274   """.        :rt
+00017030: 7970 653a 2044 696d 0a20 2020 2020 2020  ype: Dim.       
+00017040: 2022 2222 0a20 2020 2020 2020 2069 6620   """.        if 
+00017050: 7365 6c66 2e69 735f 7a65 726f 2829 3a0a  self.is_zero():.
+00017060: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00017070: 726e 205f 6d61 6b65 5f63 6f6e 7374 616e  rn _make_constan
+00017080: 745f 7374 6174 6963 5f64 696d 2830 290a  t_static_dim(0).
+00017090: 2020 2020 2020 2020 6966 206c 656e 2873          if len(s
+000170a0: 656c 662e 7465 726d 7329 203d 3d20 313a  elf.terms) == 1:
+000170b0: 0a20 2020 2020 2020 2020 2020 2072 6574  .            ret
+000170c0: 7572 6e20 7365 6c66 2e74 6572 6d73 5b30  urn self.terms[0
+000170d0: 5d2e 6173 5f64 696d 2829 0a20 2020 2020  ].as_dim().     
+000170e0: 2020 2061 6464 5f70 6172 7473 203d 205b     add_parts = [
+000170f0: 5d0a 2020 2020 2020 2020 6465 7363 5f70  ].        desc_p
+00017100: 6172 7473 203d 205b 5d0a 2020 2020 2020  arts = [].      
+00017110: 2020 6469 6d20 3d20 300a 2020 2020 2020    dim = 0.      
+00017120: 2020 666f 7220 7465 726d 2069 6e20 7365    for term in se
+00017130: 6c66 2e74 6572 6d73 3a0a 2020 2020 2020  lf.terms:.      
+00017140: 2020 2020 2020 7320 3d20 7465 726d 2e61        s = term.a
+00017150: 735f 6469 6d28 290a 2020 2020 2020 2020  s_dim().        
+00017160: 2020 2020 6164 645f 7061 7274 732e 6170      add_parts.ap
+00017170: 7065 6e64 2873 290a 2020 2020 2020 2020  pend(s).        
+00017180: 2020 2020 6465 7363 5f70 6172 7473 2e61      desc_parts.a
+00017190: 7070 656e 6428 5f67 6574 5f64 6573 6372  ppend(_get_descr
+000171a0: 6970 7469 6f6e 2873 2929 0a20 2020 2020  iption(s)).     
+000171b0: 2020 2020 2020 2069 6620 6469 6d20 6973         if dim is
+000171c0: 206e 6f74 204e 6f6e 6520 616e 6420 732e   not None and s.
+000171d0: 6469 6d65 6e73 696f 6e20 6973 206e 6f74  dimension is not
+000171e0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
+000171f0: 2020 2020 2020 2064 696d 202b 3d20 732e         dim += s.
+00017200: 6469 6d65 6e73 696f 6e0a 2020 2020 2020  dimension.      
+00017210: 2020 2020 2020 656c 7365 3a0a 2020 2020        else:.    
+00017220: 2020 2020 2020 2020 2020 2020 6469 6d20              dim 
+00017230: 3d20 4e6f 6e65 0a20 2020 2020 2020 2069  = None.        i
+00017240: 6620 6c65 6e28 6164 645f 7061 7274 7329  f len(add_parts)
+00017250: 203d 3d20 313a 0a20 2020 2020 2020 2020   == 1:.         
+00017260: 2020 2072 6574 7572 6e20 6164 645f 7061     return add_pa
+00017270: 7274 735b 305d 0a20 2020 2020 2020 2072  rts[0].        r
+00017280: 6574 7572 6e20 5f64 2e44 696d 280a 2020  eturn _d.Dim(.  
+00017290: 2020 2020 2020 2020 2020 6b69 6e64 3d5f            kind=_
+000172a0: 6765 745f 6d65 7267 6564 5f64 696d 5f6b  get_merged_dim_k
+000172b0: 696e 6428 6164 645f 7061 7274 7329 2c0a  ind(add_parts),.
+000172c0: 2020 2020 2020 2020 2020 2020 6465 7363              desc
+000172d0: 7269 7074 696f 6e3d 222b 222e 6a6f 696e  ription="+".join
+000172e0: 2864 6573 635f 7061 7274 7329 2c0a 2020  (desc_parts),.  
+000172f0: 2020 2020 2020 2020 2020 6469 6d65 6e73            dimens
+00017300: 696f 6e3d 6469 6d2c 0a20 2020 2020 2020  ion=dim,.       
+00017310: 2020 2020 2064 6572 6976 6564 5f66 726f       derived_fro
+00017320: 6d5f 6f70 3d4f 7028 6b69 6e64 3d22 6164  m_op=Op(kind="ad
+00017330: 6422 2c20 696e 7075 7473 3d61 6464 5f70  d", inputs=add_p
+00017340: 6172 7473 292c 0a20 2020 2020 2020 2020  arts),.         
+00017350: 2020 2064 6572 6976 6564 5f66 726f 6d5f     derived_from_
+00017360: 7461 673d 7365 6c66 2e72 6570 7265 7365  tag=self.represe
+00017370: 6e74 6174 6976 655f 7461 6728 292c 0a20  ntative_tag(),. 
+00017380: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+00017390: 6620 5f5f 7265 7072 5f5f 2873 656c 6629  f __repr__(self)
+000173a0: 3a0a 2020 2020 2020 2020 7265 7475 726e  :.        return
+000173b0: 2022 4469 6d2e 5f4f 704c 696e 6561 7254   "Dim._OpLinearT
+000173c0: 6572 6d28 2572 2922 2025 2028 7365 6c66  erm(%r)" % (self
+000173d0: 2e74 6572 6d73 2c29 0a0a 2020 2020 6465  .terms,)..    de
+000173e0: 6620 6973 5f7a 6572 6f28 7365 6c66 293a  f is_zero(self):
+000173f0: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00017400: 2020 2020 203a 7274 7970 653a 2062 6f6f       :rtype: boo
+00017410: 6c0a 2020 2020 2020 2020 2222 220a 2020  l.        """.  
+00017420: 2020 2020 2020 7265 7475 726e 206e 6f74        return not
+00017430: 2073 656c 662e 7465 726d 730a 0a20 2020   self.terms..   
+00017440: 2064 6566 2065 7874 656e 645f 6164 645f   def extend_add_
+00017450: 7375 625f 2873 656c 662c 206f 7468 6572  sub_(self, other
+00017460: 2c20 6b69 6e64 2c20 7269 6768 7429 3a0a  , kind, right):.
+00017470: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00017480: 2020 2020 3a70 6172 616d 2044 696d 7c69      :param Dim|i
+00017490: 6e74 206f 7468 6572 3a0a 2020 2020 2020  nt other:.      
+000174a0: 2020 3a70 6172 616d 2073 7472 206b 696e    :param str kin
+000174b0: 643a 2022 6164 6422 206f 7220 2273 7562  d: "add" or "sub
+000174c0: 220a 2020 2020 2020 2020 3a70 6172 616d  ".        :param
+000174d0: 2062 6f6f 6c20 7269 6768 743a 206f 7220   bool right: or 
+000174e0: 6c65 6674 2e20 7269 6768 7420 6d65 616e  left. right mean
+000174f0: 7320 7365 6c66 202b 206f 7468 6572 2c20  s self + other, 
+00017500: 6c65 6674 206d 6561 6e73 206f 7468 6572  left means other
+00017510: 202b 2073 656c 660a 2020 2020 2020 2020   + self.        
+00017520: 2222 220a 2020 2020 2020 2020 6173 7365  """.        asse
+00017530: 7274 206b 696e 6420 696e 207b 2261 6464  rt kind in {"add
+00017540: 222c 2022 7375 6222 7d0a 2020 2020 2020  ", "sub"}.      
+00017550: 2020 6f74 6865 7220 3d20 7365 6c66 2e5f    other = self._
+00017560: 6d61 6b65 5f64 696d 286f 7468 6572 2c20  make_dim(other, 
+00017570: 6b69 6e64 3d6b 696e 6429 0a20 2020 2020  kind=kind).     
+00017580: 2020 2069 6620 6f74 6865 722e 6973 5f63     if other.is_c
+00017590: 6f6e 7374 616e 745f 7374 6174 6963 5f64  onstant_static_d
+000175a0: 696d 2829 2061 6e64 206f 7468 6572 2e64  im() and other.d
+000175b0: 696d 656e 7369 6f6e 203d 3d20 303a 0a20  imension == 0:. 
+000175c0: 2020 2020 2020 2020 2020 2072 6574 7572             retur
+000175d0: 6e0a 2020 2020 2020 2020 6966 206f 7468  n.        if oth
+000175e0: 6572 2e64 6572 6976 6564 5f66 726f 6d5f  er.derived_from_
+000175f0: 6f70 2061 6e64 206f 7468 6572 2e64 6572  op and other.der
+00017600: 6976 6564 5f66 726f 6d5f 6f70 2e6b 696e  ived_from_op.kin
+00017610: 6420 3d3d 2022 6164 6422 3a0a 2020 2020  d == "add":.    
+00017620: 2020 2020 2020 2020 666f 7220 6f74 6865          for othe
+00017630: 725f 2069 6e20 6f74 6865 722e 6465 7269  r_ in other.deri
+00017640: 7665 645f 6672 6f6d 5f6f 702e 696e 7075  ved_from_op.inpu
+00017650: 7473 2069 6620 7269 6768 7420 656c 7365  ts if right else
+00017660: 2072 6576 6572 7365 6428 6f74 6865 722e   reversed(other.
+00017670: 6465 7269 7665 645f 6672 6f6d 5f6f 702e  derived_from_op.
+00017680: 696e 7075 7473 293a 0a20 2020 2020 2020  inputs):.       
+00017690: 2020 2020 2020 2020 2073 656c 662e 6578           self.ex
+000176a0: 7465 6e64 5f61 6464 5f73 7562 5f28 6f74  tend_add_sub_(ot
+000176b0: 6865 725f 2c20 6b69 6e64 3d6b 696e 642c  her_, kind=kind,
+000176c0: 2072 6967 6874 3d72 6967 6874 290a 2020   right=right).  
+000176d0: 2020 2020 2020 2020 2020 7265 7475 726e            return
+000176e0: 0a20 2020 2020 2020 2074 6572 6d20 3d20  .        term = 
+000176f0: 5f4f 704d 756c 7454 6572 6d2e 6672 6f6d  _OpMultTerm.from
+00017700: 5f64 696d 286f 7468 6572 290a 2020 2020  _dim(other).    
+00017710: 2020 2020 6e65 675f 7465 726d 203d 2074      neg_term = t
+00017720: 6572 6d2e 6e65 6761 7469 7665 2829 0a20  erm.negative(). 
+00017730: 2020 2020 2020 2069 6620 6b69 6e64 203d         if kind =
+00017740: 3d20 2273 7562 223a 0a20 2020 2020 2020  = "sub":.       
+00017750: 2020 2020 2074 6572 6d2c 206e 6567 5f74       term, neg_t
+00017760: 6572 6d20 3d20 6e65 675f 7465 726d 2c20  erm = neg_term, 
+00017770: 7465 726d 0a20 2020 2020 2020 206d 6f73  term.        mos
+00017780: 745f 7265 6365 6e74 5f74 6572 6d20 3d20  t_recent_term = 
+00017790: 7365 6c66 2e74 6572 6d73 5b2d 3120 6966  self.terms[-1 if
+000177a0: 2072 6967 6874 2065 6c73 6520 305d 2069   right else 0] i
+000177b0: 6620 7365 6c66 2e74 6572 6d73 2065 6c73  f self.terms els
+000177c0: 6520 4e6f 6e65 0a20 2020 2020 2020 2069  e None.        i
+000177d0: 6620 6d6f 7374 5f72 6563 656e 745f 7465  f most_recent_te
+000177e0: 726d 3a0a 2020 2020 2020 2020 2020 2020  rm:.            
+000177f0: 6966 206d 6f73 745f 7265 6365 6e74 5f74  if most_recent_t
+00017800: 6572 6d20 3d3d 206e 6567 5f74 6572 6d3a  erm == neg_term:
+00017810: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00017820: 2073 656c 662e 7465 726d 732e 706f 7028   self.terms.pop(
+00017830: 2d31 2069 6620 7269 6768 7420 656c 7365  -1 if right else
+00017840: 2030 290a 2020 2020 2020 2020 2020 2020   0).            
+00017850: 2020 2020 7265 7475 726e 0a20 2020 2020      return.     
+00017860: 2020 2020 2020 2069 6620 6d6f 7374 5f72         if most_r
+00017870: 6563 656e 745f 7465 726d 2e69 735f 636f  ecent_term.is_co
+00017880: 6e73 7461 6e74 5f73 7461 7469 635f 6469  nstant_static_di
+00017890: 6d28 2920 616e 6420 7465 726d 2e69 735f  m() and term.is_
+000178a0: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
+000178b0: 6469 6d28 293a 0a20 2020 2020 2020 2020  dim():.         
+000178c0: 2020 2020 2020 2073 656c 662e 7465 726d         self.term
+000178d0: 735b 2d31 2069 6620 7269 6768 7420 656c  s[-1 if right el
+000178e0: 7365 2030 5d20 3d20 5f4f 704d 756c 7454  se 0] = _OpMultT
+000178f0: 6572 6d2e 6672 6f6d 5f64 696d 280a 2020  erm.from_dim(.  
+00017900: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017910: 2020 5f6d 616b 655f 636f 6e73 7461 6e74    _make_constant
+00017920: 5f73 7461 7469 635f 6469 6d28 6d6f 7374  _static_dim(most
+00017930: 5f72 6563 656e 745f 7465 726d 2e64 696d  _recent_term.dim
+00017940: 656e 7369 6f6e 202b 2074 6572 6d2e 6469  ension + term.di
+00017950: 6d65 6e73 696f 6e2c 206b 696e 643d 6f74  mension, kind=ot
+00017960: 6865 722e 6b69 6e64 290a 2020 2020 2020  her.kind).      
+00017970: 2020 2020 2020 2020 2020 290a 2020 2020            ).    
+00017980: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00017990: 726e 0a20 2020 2020 2020 2020 2020 2069  rn.            i
+000179a0: 6620 6d6f 7374 5f72 6563 656e 745f 7465  f most_recent_te
+000179b0: 726d 2e74 6572 6d73 2061 6e64 2074 6572  rm.terms and ter
+000179c0: 6d2e 7465 726d 7320 616e 6420 6d6f 7374  m.terms and most
+000179d0: 5f72 6563 656e 745f 7465 726d 2e74 6572  _recent_term.ter
+000179e0: 6d73 5b2d 315d 203d 3d20 7465 726d 2e74  ms[-1] == term.t
+000179f0: 6572 6d73 5b2d 315d 3a0a 2020 2020 2020  erms[-1]:.      
+00017a00: 2020 2020 2020 2020 2020 2320 4d65 7267            # Merg
+00017a10: 6520 7465 726d 730a 2020 2020 2020 2020  e terms.        
+00017a20: 2020 2020 2020 2020 6120 3d20 5f4f 704d          a = _OpM
+00017a30: 756c 7454 6572 6d2e 6672 6f6d 5f64 696d  ultTerm.from_dim
+00017a40: 5f66 6163 746f 7273 286d 6f73 745f 7265  _factors(most_re
+00017a50: 6365 6e74 5f74 6572 6d2e 7465 726d 735b  cent_term.terms[
+00017a60: 3a2d 315d 292e 6173 5f64 696d 2829 0a20  :-1]).as_dim(). 
+00017a70: 2020 2020 2020 2020 2020 2020 2020 2062                 b
+00017a80: 203d 205f 4f70 4d75 6c74 5465 726d 2e66   = _OpMultTerm.f
+00017a90: 726f 6d5f 6469 6d5f 6661 6374 6f72 7328  rom_dim_factors(
+00017aa0: 7465 726d 2e74 6572 6d73 5b3a 2d31 5d29  term.terms[:-1])
+00017ab0: 2e61 735f 6469 6d28 290a 2020 2020 2020  .as_dim().      
+00017ac0: 2020 2020 2020 2020 2020 7265 7320 3d20            res = 
+00017ad0: 5f4f 704d 756c 7454 6572 6d2e 6672 6f6d  _OpMultTerm.from
+00017ae0: 5f64 696d 2828 6120 2b20 6229 2069 6620  _dim((a + b) if 
+00017af0: 7269 6768 7420 656c 7365 2028 6220 2b20  right else (b + 
+00017b00: 6129 290a 2020 2020 2020 2020 2020 2020  a)).            
+00017b10: 2020 2020 7265 732e 6578 7465 6e64 5f6d      res.extend_m
+00017b20: 756c 5f64 6976 5f28 7465 726d 2e74 6572  ul_div_(term.ter
+00017b30: 6d73 5b2d 315d 2c20 6b69 6e64 3d22 6d75  ms[-1], kind="mu
+00017b40: 6c22 2c20 7269 6768 743d 5472 7565 290a  l", right=True).
+00017b50: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017b60: 7365 6c66 2e74 6572 6d73 5b2d 3120 6966  self.terms[-1 if
+00017b70: 2072 6967 6874 2065 6c73 6520 305d 203d   right else 0] =
+00017b80: 2072 6573 0a20 2020 2020 2020 2020 2020   res.           
+00017b90: 2020 2020 2072 6574 7572 6e0a 2020 2020       return.    
+00017ba0: 2020 2020 6966 2072 6967 6874 3a0a 2020      if right:.  
+00017bb0: 2020 2020 2020 2020 2020 7365 6c66 2e74            self.t
+00017bc0: 6572 6d73 2e61 7070 656e 6428 7465 726d  erms.append(term
+00017bd0: 290a 2020 2020 2020 2020 656c 7365 3a0a  ).        else:.
+00017be0: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+00017bf0: 2e74 6572 6d73 2e69 6e73 6572 7428 302c  .terms.insert(0,
+00017c00: 2074 6572 6d29 0a0a 2020 2020 6465 6620   term)..    def 
+00017c10: 6578 7465 6e64 5f6d 756c 5f64 6976 5f28  extend_mul_div_(
+00017c20: 7365 6c66 2c20 6f74 6865 722c 206b 696e  self, other, kin
+00017c30: 642c 2072 6967 6874 293a 0a20 2020 2020  d, right):.     
+00017c40: 2020 2022 2222 0a20 2020 2020 2020 203a     """.        :
+00017c50: 7061 7261 6d20 4469 6d7c 696e 7420 6f74  param Dim|int ot
+00017c60: 6865 723a 0a20 2020 2020 2020 203a 7061  her:.        :pa
+00017c70: 7261 6d20 7374 7220 6b69 6e64 3a20 226d  ram str kind: "m
+00017c80: 756c 2220 6f72 2022 6365 696c 6469 7622  ul" or "ceildiv"
+00017c90: 0a20 2020 2020 2020 203a 7061 7261 6d20  .        :param 
+00017ca0: 626f 6f6c 2072 6967 6874 3a20 6f72 206c  bool right: or l
+00017cb0: 6566 742e 2072 6967 6874 206d 6561 6e73  eft. right means
+00017cc0: 2073 656c 6620 2a20 6f74 6865 722c 206c   self * other, l
+00017cd0: 6566 7420 6d65 616e 7320 6f74 6865 7220  eft means other 
+00017ce0: 2a20 7365 6c66 0a20 2020 2020 2020 2022  * self.        "
+00017cf0: 2222 0a20 2020 2020 2020 2061 7373 6572  "".        asser
+00017d00: 7420 6b69 6e64 2069 6e20 7b22 6d75 6c22  t kind in {"mul"
+00017d10: 2c20 2266 6c6f 6f72 6469 7622 2c20 2274  , "floordiv", "t
+00017d20: 7275 6564 6976 222c 2022 6365 696c 6469  ruediv", "ceildi
+00017d30: 7622 7d0a 2020 2020 2020 2020 6f74 6865  v"}.        othe
+00017d40: 7220 3d20 7365 6c66 2e5f 6d61 6b65 5f64  r = self._make_d
+00017d50: 696d 286f 7468 6572 2c20 6b69 6e64 3d6b  im(other, kind=k
+00017d60: 696e 6429 0a20 2020 2020 2020 2069 6620  ind).        if 
+00017d70: 6b69 6e64 203d 3d20 226d 756c 2220 616e  kind == "mul" an
+00017d80: 6420 7269 6768 743a 0a20 2020 2020 2020  d right:.       
+00017d90: 2020 2020 2069 6620 6e6f 7420 616c 6c28       if not all(
+00017da0: 7465 726d 2e63 616e 5f73 696d 706c 6966  term.can_simplif
+00017db0: 7928 6f74 6865 722c 206b 696e 643d 6b69  y(other, kind=ki
+00017dc0: 6e64 2c20 7269 6768 743d 7269 6768 7429  nd, right=right)
+00017dd0: 2066 6f72 2074 6572 6d20 696e 2073 656c   for term in sel
+00017de0: 662e 7465 726d 7329 3a0a 2020 2020 2020  f.terms):.      
+00017df0: 2020 2020 2020 2020 2020 2320 446f 2069            # Do i
+00017e00: 7420 7468 6520 6f74 6865 7220 7761 7920  t the other way 
+00017e10: 6172 6f75 6e64 0a20 2020 2020 2020 2020  around.         
+00017e20: 2020 2020 2020 2073 656c 662e 7465 726d         self.term
+00017e30: 732c 206f 7468 6572 203d 205f 4f70 4c69  s, other = _OpLi
+00017e40: 6e65 6172 5465 726d 2e66 726f 6d5f 6469  nearTerm.from_di
+00017e50: 6d28 6f74 6865 7229 2e74 6572 6d73 2c20  m(other).terms, 
+00017e60: 7365 6c66 2e61 735f 6469 6d28 290a 2020  self.as_dim().  
+00017e70: 2020 2020 2020 2020 2020 2020 2020 7269                ri
+00017e80: 6768 7420 3d20 4661 6c73 650a 2020 2020  ght = False.    
+00017e90: 2020 2020 6966 206f 7468 6572 2e69 735f      if other.is_
+00017ea0: 636f 6e73 7461 6e74 5f73 7461 7469 635f  constant_static_
+00017eb0: 6469 6d28 2920 616e 6420 6f74 6865 722e  dim() and other.
+00017ec0: 6469 6d65 6e73 696f 6e20 3d3d 2031 3a0a  dimension == 1:.
+00017ed0: 2020 2020 2020 2020 2020 2020 7265 7475              retu
+00017ee0: 726e 0a20 2020 2020 2020 2069 6620 6b69  rn.        if ki
+00017ef0: 6e64 2e65 6e64 7377 6974 6828 2264 6976  nd.endswith("div
+00017f00: 2229 2061 6e64 206c 656e 2873 656c 662e  ") and len(self.
+00017f10: 7465 726d 7329 203e 3d20 323a 0a20 2020  terms) >= 2:.   
+00017f20: 2020 2020 2020 2020 2069 6620 616e 7928           if any(
+00017f30: 6e6f 7420 7465 726d 2e64 6976 6973 6962  not term.divisib
+00017f40: 6c65 286f 7468 6572 2c20 7269 6768 743d  le(other, right=
+00017f50: 7269 6768 7429 2066 6f72 2074 6572 6d20  right) for term 
+00017f60: 696e 2073 656c 662e 7465 726d 7329 3a0a  in self.terms):.
+00017f70: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017f80: 7365 6c66 2e74 6572 6d73 203d 205b 0a20  self.terms = [. 
+00017f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00017fa0: 2020 205f 4f70 4d75 6c74 5465 726d 2e66     _OpMultTerm.f
+00017fb0: 726f 6d5f 6469 6d28 5f4f 704d 756c 7454  rom_dim(_OpMultT
+00017fc0: 6572 6d2e 6e65 775f 6469 765f 6469 6d28  erm.new_div_dim(
+00017fd0: 7365 6c66 2e61 735f 6469 6d28 292c 206f  self.as_dim(), o
+00017fe0: 7468 6572 2c20 6b69 6e64 3d6b 696e 642c  ther, kind=kind,
+00017ff0: 2072 6967 6874 3d72 6967 6874 2929 0a20   right=right)). 
+00018000: 2020 2020 2020 2020 2020 2020 2020 205d                 ]
+00018010: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00018020: 2072 6574 7572 6e0a 2020 2020 2020 2020   return.        
+00018030: 666f 7220 7465 726d 2069 6e20 7365 6c66  for term in self
+00018040: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
+00018050: 2020 2020 7465 726d 2e65 7874 656e 645f      term.extend_
+00018060: 6d75 6c5f 6469 765f 286f 7468 6572 2c20  mul_div_(other, 
+00018070: 6b69 6e64 3d6b 696e 642c 2072 6967 6874  kind=kind, right
+00018080: 3d72 6967 6874 290a 0a20 2020 2064 6566  =right)..    def
+00018090: 205f 6d61 6b65 5f64 696d 2873 656c 662c   _make_dim(self,
+000180a0: 206f 7468 6572 2c20 6b69 6e64 293a 0a20   other, kind):. 
+000180b0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000180c0: 2020 203a 7061 7261 6d20 4469 6d7c 696e     :param Dim|in
+000180d0: 7420 6f74 6865 723a 0a20 2020 2020 2020  t other:.       
+000180e0: 203a 7061 7261 6d20 7374 7220 6b69 6e64   :param str kind
+000180f0: 3a0a 2020 2020 2020 2020 3a72 7479 7065  :.        :rtype
+00018100: 3a20 4469 6d0a 2020 2020 2020 2020 2222  : Dim.        ""
+00018110: 220a 2020 2020 2020 2020 6966 2069 7369  ".        if isi
+00018120: 6e73 7461 6e63 6528 6f74 6865 722c 2069  nstance(other, i
+00018130: 6e74 293a 0a20 2020 2020 2020 2020 2020  nt):.           
+00018140: 2062 6173 655f 7461 6720 3d20 7365 6c66   base_tag = self
+00018150: 2e72 6570 7265 7365 6e74 6174 6976 655f  .representative_
+00018160: 7461 6728 290a 2020 2020 2020 2020 2020  tag().          
+00018170: 2020 7265 7475 726e 205f 6d61 6b65 5f63    return _make_c
+00018180: 6f6e 7374 616e 745f 7374 6174 6963 5f64  onstant_static_d
+00018190: 696d 286f 7468 6572 2c20 6b69 6e64 3d62  im(other, kind=b
+000181a0: 6173 655f 7461 672e 6b69 6e64 2069 6620  ase_tag.kind if 
+000181b0: 6261 7365 5f74 6167 2065 6c73 6520 4e6f  base_tag else No
+000181c0: 6e65 290a 2020 2020 2020 2020 656c 6966  ne).        elif
+000181d0: 2069 7369 6e73 7461 6e63 6528 6f74 6865   isinstance(othe
+000181e0: 722c 205f 642e 4469 6d29 3a0a 2020 2020  r, _d.Dim):.    
+000181f0: 2020 2020 2020 2020 7265 7475 726e 206f          return o
+00018200: 7468 6572 2e67 6574 5f73 616d 655f 6261  ther.get_same_ba
+00018210: 7365 2829 0a20 2020 2020 2020 2065 6c73  se().        els
+00018220: 653a 0a20 2020 2020 2020 2020 2020 2072  e:.            r
+00018230: 6169 7365 2054 7970 6545 7272 6f72 2822  aise TypeError("
+00018240: 2573 2025 7320 2573 2069 6e76 616c 6964  %s %s %s invalid
+00018250: 2066 6f72 2074 7970 6520 2573 2220 2520   for type %s" % 
+00018260: 2873 656c 662c 206b 696e 642c 206f 7468  (self, kind, oth
+00018270: 6572 2c20 7479 7065 286f 7468 6572 2929  er, type(other))
+00018280: 290a 0a20 2020 2064 6566 2072 6570 7265  )..    def repre
+00018290: 7365 6e74 6174 6976 655f 7461 6728 7365  sentative_tag(se
+000182a0: 6c66 293a 0a20 2020 2020 2020 2022 2222  lf):.        """
+000182b0: 0a20 2020 2020 2020 203a 7274 7970 653a  .        :rtype:
+000182c0: 2044 696d 7c4e 6f6e 650a 2020 2020 2020   Dim|None.      
+000182d0: 2020 2222 220a 2020 2020 2020 2020 2320    """.        # 
+000182e0: 4669 7273 7420 6669 6e64 2061 6e79 2064  First find any d
+000182f0: 796e 616d 6963 2e0a 2020 2020 2020 2020  ynamic..        
+00018300: 666f 7220 7465 726d 2069 6e20 7365 6c66  for term in self
+00018310: 2e74 6572 6d73 3a0a 2020 2020 2020 2020  .terms:.        
+00018320: 2020 2020 666f 7220 7465 726d 5f20 696e      for term_ in
+00018330: 2074 6572 6d2e 7465 726d 733a 0a20 2020   term.terms:.   
+00018340: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+00018350: 7465 726d 5f2e 6973 5f64 796e 616d 6963  term_.is_dynamic
+00018360: 2829 3a0a 2020 2020 2020 2020 2020 2020  ():.            
+00018370: 2020 2020 2020 2020 7265 7475 726e 2074          return t
+00018380: 6572 6d5f 0a20 2020 2020 2020 2023 204e  erm_.        # N
+00018390: 6f77 2066 696e 6420 6e6f 6e2d 756e 7370  ow find non-unsp
+000183a0: 6563 6966 6965 642e 0a20 2020 2020 2020  ecified..       
+000183b0: 2066 6f72 2074 6572 6d20 696e 2073 656c   for term in sel
+000183c0: 662e 7465 726d 733a 0a20 2020 2020 2020  f.terms:.       
+000183d0: 2020 2020 2066 6f72 2074 6572 6d5f 2069       for term_ i
+000183e0: 6e20 7465 726d 2e74 6572 6d73 3a0a 2020  n term.terms:.  
+000183f0: 2020 2020 2020 2020 2020 2020 2020 6966                if
+00018400: 2074 6572 6d5f 2e6b 696e 6420 213d 2044   term_.kind != D
+00018410: 696d 5479 7065 732e 556e 7370 6563 6966  imTypes.Unspecif
+00018420: 6965 643a 0a20 2020 2020 2020 2020 2020  ied:.           
+00018430: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
+00018440: 7465 726d 5f0a 2020 2020 2020 2020 2320  term_.        # 
+00018450: 4e6f 7720 6669 6e64 2061 6e79 2e0a 2020  Now find any..  
+00018460: 2020 2020 2020 666f 7220 7465 726d 2069        for term i
+00018470: 6e20 7365 6c66 2e74 6572 6d73 3a0a 2020  n self.terms:.  
+00018480: 2020 2020 2020 2020 2020 666f 7220 7465            for te
+00018490: 726d 5f20 696e 2074 6572 6d2e 7465 726d  rm_ in term.term
+000184a0: 733a 0a20 2020 2020 2020 2020 2020 2020  s:.             
+000184b0: 2020 2072 6574 7572 6e20 7465 726d 5f0a     return term_.
+000184c0: 2020 2020 2020 2020 7265 7475 726e 204e          return N
+000184d0: 6f6e 650a 0a0a 6465 6620 5f67 6574 5f6d  one...def _get_m
+000184e0: 6572 6765 645f 6469 6d5f 6b69 6e64 2864  erged_dim_kind(d
+000184f0: 696d 5f74 6167 7329 3a0a 2020 2020 2222  im_tags):.    ""
+00018500: 220a 2020 2020 3a70 6172 616d 206c 6973  ".    :param lis
+00018510: 745b 4469 6d5d 7c74 7570 6c65 5b44 696d  t[Dim]|tuple[Dim
+00018520: 5d20 6469 6d5f 7461 6773 3a0a 2020 2020  ] dim_tags:.    
+00018530: 3a72 6574 7572 6e3a 2064 696d 206b 696e  :return: dim kin
+00018540: 640a 2020 2020 3a72 7479 7065 3a20 456e  d.    :rtype: En
+00018550: 7469 7479 0a20 2020 2022 2222 0a20 2020  tity.    """.   
+00018560: 2069 6620 616e 7928 7461 672e 6973 5f62   if any(tag.is_b
+00018570: 6174 6368 5f64 696d 2829 2066 6f72 2074  atch_dim() for t
+00018580: 6167 2069 6e20 6469 6d5f 7461 6773 293a  ag in dim_tags):
+00018590: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+000185a0: 4469 6d54 7970 6573 2e42 6174 6368 0a20  DimTypes.Batch. 
+000185b0: 2020 2065 6c69 6620 616e 7928 7461 672e     elif any(tag.
+000185c0: 6973 5f66 6561 7475 7265 5f64 696d 2829  is_feature_dim()
+000185d0: 2066 6f72 2074 6167 2069 6e20 6469 6d5f   for tag in dim_
+000185e0: 7461 6773 293a 0a20 2020 2020 2020 2072  tags):.        r
+000185f0: 6574 7572 6e20 4469 6d54 7970 6573 2e46  eturn DimTypes.F
+00018600: 6561 7475 7265 0a20 2020 2065 6c73 653a  eature.    else:
+00018610: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
+00018620: 4469 6d54 7970 6573 2e53 7061 7469 616c  DimTypes.Spatial
+00018630: 0a0a 0a64 6566 2064 696d 5f63 6d70 5f76  ...def dim_cmp_v
+00018640: 616c 7565 286f 626a 293a 0a20 2020 2022  alue(obj):.    "
+00018650: 2222 0a20 2020 203a 7061 7261 6d20 4469  "".    :param Di
+00018660: 6d7c 5f4d 6172 6b65 6444 696d 206f 626a  m|_MarkedDim obj
+00018670: 3a0a 2020 2020 3a72 6574 7572 6e3a 2061  :.    :return: a
+00018680: 6e79 7468 696e 6720 7768 6963 6820 6361  nything which ca
+00018690: 6e20 6265 2063 6f6d 7061 7265 640a 2020  n be compared.  
+000186a0: 2020 2222 220a 2020 2020 2320 4d61 6b65    """.    # Make
+000186b0: 2044 696d 2061 6e64 205f 4d61 726b 6564   Dim and _Marked
+000186c0: 4469 6d20 636f 6d70 6172 6162 6c65 2074  Dim comparable t
+000186d0: 6f20 6561 6368 206f 7468 6572 2e0a 2020  o each other..  
+000186e0: 2020 2320 4e6f 7465 2074 6861 7420 7468    # Note that th
+000186f0: 6520 6f72 6465 7220 6973 2072 6561 6c6c  e order is reall
+00018700: 7920 6172 6269 7472 6172 7920 616e 6420  y arbitrary and 
+00018710: 646f 6573 206e 6f74 206d 6174 7465 722e  does not matter.
+00018720: 0a20 2020 2069 6620 6973 696e 7374 616e  .    if isinstan
+00018730: 6365 286f 626a 2c20 5f64 2e44 696d 293a  ce(obj, _d.Dim):
+00018740: 0a20 2020 2020 2020 206f 626a 203d 206f  .        obj = o
+00018750: 626a 2e67 6574 5f73 616d 655f 6261 7365  bj.get_same_base
+00018760: 2829 0a20 2020 2020 2020 2072 6574 7572  ().        retur
+00018770: 6e20 280a 2020 2020 2020 2020 2020 2020  n (.            
+00018780: 2222 2c0a 2020 2020 2020 2020 2020 2020  "",.            
+00018790: 6f62 6a2e 6465 7363 7269 7074 696f 6e2c  obj.description,
+000187a0: 0a20 2020 2020 2020 2020 2020 206f 626a  .            obj
+000187b0: 2e6b 696e 642c 0a20 2020 2020 2020 2020  .kind,.         
+000187c0: 2020 206f 626a 2e64 696d 656e 7369 6f6e     obj.dimension
+000187d0: 2c0a 2020 2020 2020 2020 2020 2020 6f62  ,.            ob
+000187e0: 6a2e 6479 6e5f 7369 7a65 5f65 7874 2e64  j.dyn_size_ext.d
+000187f0: 696d 7320 6966 206f 626a 2e64 796e 5f73  ims if obj.dyn_s
+00018800: 697a 655f 6578 7420 6973 206e 6f74 204e  ize_ext is not N
+00018810: 6f6e 6520 656c 7365 204e 6f6e 652c 0a20  one else None,. 
+00018820: 2020 2020 2020 2029 0a20 2020 2069 6620         ).    if 
+00018830: 6973 696e 7374 616e 6365 286f 626a 2c20  isinstance(obj, 
+00018840: 5f6d 2e4d 6172 6b65 6444 696d 293a 0a20  _m.MarkedDim):. 
+00018850: 2020 2020 2020 2072 6574 7572 6e20 6f62         return ob
+00018860: 6a2e 5f5f 636c 6173 735f 5f2e 5f5f 6e61  j.__class__.__na
+00018870: 6d65 5f5f 2c20 6f62 6a2e 7461 670a 2020  me__, obj.tag.  
+00018880: 2020 7265 7475 726e 206f 626a 0a           return obj.
```

### Comparing `returnn-1.20230718.112120/returnn/tensor/_tensor_extra.py` & `returnn-1.20230718.124003/returnn/tensor/_tensor_extra.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tensor/_tensor_mixin_base.py` & `returnn-1.20230718.124003/returnn/tensor/_tensor_mixin_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tensor/_tensor_op_overloads.py` & `returnn-1.20230718.124003/returnn/tensor/_tensor_op_overloads.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tensor/control_flow_ctx.py` & `returnn-1.20230718.124003/returnn/tensor/control_flow_ctx.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tensor/dim.py` & `returnn-1.20230718.124003/returnn/tensor/dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tensor/marked_dim.py` & `returnn-1.20230718.124003/returnn/tensor/marked_dim.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tensor/tensor.py` & `returnn-1.20230718.124003/returnn/tensor/tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tensor/tensor_dict.py` & `returnn-1.20230718.124003/returnn/tensor/tensor_dict.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tensor/utils.py` & `returnn-1.20230718.124003/returnn/tensor/utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/compat.py` & `returnn-1.20230718.124003/returnn/tf/compat.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/data_pipeline.py` & `returnn-1.20230718.124003/returnn/tf/data_pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/distributed.py` & `returnn-1.20230718.124003/returnn/tf/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/engine.py` & `returnn-1.20230718.124003/returnn/tf/engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/frontend_layers/_backend.py` & `returnn-1.20230718.124003/returnn/tf/frontend_layers/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/frontend_layers/_utils.py` & `returnn-1.20230718.124003/returnn/tf/frontend_layers/_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/frontend_layers/cond.py` & `returnn-1.20230718.124003/returnn/tf/frontend_layers/cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/frontend_layers/config_entry_points.py` & `returnn-1.20230718.124003/returnn/tf/frontend_layers/config_entry_points.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/frontend_layers/debug_eager_mode.py` & `returnn-1.20230718.124003/returnn/tf/frontend_layers/debug_eager_mode.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/frontend_layers/dims.py` & `returnn-1.20230718.124003/returnn/tf/frontend_layers/dims.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/frontend_layers/layer.py` & `returnn-1.20230718.124003/returnn/tf/frontend_layers/layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/frontend_layers/make_layer.py` & `returnn-1.20230718.124003/returnn/tf/frontend_layers/make_layer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/frontend_layers/parameter_assign.py` & `returnn-1.20230718.124003/returnn/tf/frontend_layers/parameter_assign.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/frontend_layers/prev_tensor_ref.py` & `returnn-1.20230718.124003/returnn/tf/frontend_layers/prev_tensor_ref.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/frontend_low_level/_backend.py` & `returnn-1.20230718.124003/returnn/tf/frontend_low_level/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/horovod.py` & `returnn-1.20230718.124003/returnn/tf/horovod.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/hyper_param_tuning.py` & `returnn-1.20230718.124003/returnn/tf/hyper_param_tuning.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/layers/base.py` & `returnn-1.20230718.124003/returnn/tf/layers/base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/layers/basic.py` & `returnn-1.20230718.124003/returnn/tf/layers/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/layers/rec.py` & `returnn-1.20230718.124003/returnn/tf/layers/rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/layers/segmental_model.py` & `returnn-1.20230718.124003/returnn/tf/layers/segmental_model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/layers/signal_processing.py` & `returnn-1.20230718.124003/returnn/tf/layers/signal_processing.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/layers/variable.py` & `returnn-1.20230718.124003/returnn/tf/layers/variable.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/native_op.py` & `returnn-1.20230718.124003/returnn/tf/native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/network.py` & `returnn-1.20230718.124003/returnn/tf/network.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/sprint.py` & `returnn-1.20230718.124003/returnn/tf/sprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/updater.py` & `returnn-1.20230718.124003/returnn/tf/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/util/basic.py` & `returnn-1.20230718.124003/returnn/tf/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/util/data.py` & `returnn-1.20230718.124003/returnn/tf/util/data.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/util/gradient_checkpoint.py` & `returnn-1.20230718.124003/returnn/tf/util/gradient_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/util/ken_lm.py` & `returnn-1.20230718.124003/returnn/tf/util/ken_lm.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/tf/util/open_fst.py` & `returnn-1.20230718.124003/returnn/tf/util/open_fst.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/torch/data/pipeline.py` & `returnn-1.20230718.124003/returnn/torch/data/pipeline.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/torch/data/returnn_dataset_wrapper.py` & `returnn-1.20230718.124003/returnn/torch/data/returnn_dataset_wrapper.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/torch/data/tensor_utils.py` & `returnn-1.20230718.124003/returnn/torch/data/tensor_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/torch/distributed.py` & `returnn-1.20230718.124003/returnn/torch/distributed.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/torch/engine.py` & `returnn-1.20230718.124003/returnn/torch/engine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Main engine for PyTorch
 """
 
 from __future__ import annotations
-from typing import Optional, Union, Callable, Dict
+from typing import Optional, Union, Callable, Dict, List
 from contextlib import nullcontext
 
 import gc
 import os
 import numpy
 import torch
 import time
@@ -715,35 +715,41 @@
     :param extern_data_raw: This comes out of the DataLoader.
     :param extern_data_template: Specified via `extern_data` in the config.
     :param device: E.g. the GPU.
     :return: tensor dict, like extern_data_template, but with raw tensors set to Torch tensors, on the right device.
     """
     assert isinstance(extern_data_raw, dict) and extern_data_raw
     batch_dim = _get_batch_dim_from_extern_data(extern_data_template)
-    batch_dim.dyn_size_ext = None  # if it is dynamic, reset now, and set it below
+    for dim in _get_dyn_dims_from_extern_data(extern_data_template):
+        dim.reset_eager()  # they will be reset below
+    if batch_dim.size is None and batch_dim.dyn_size_ext is None:
+        batch_dim.dyn_size_ext = Tensor(batch_dim.name or "batch", dims=[], dtype="int32")
     extern_data = TensorDict()
     for k, data in extern_data_template.data.items():
         data = data.copy_template()
         raw_tensor = extern_data_raw[k]
         if isinstance(raw_tensor, torch.Tensor):
             data.dtype = str(raw_tensor.dtype).split(".")[-1]  # just overwrite for now...
             data.raw_tensor = raw_tensor.to(device)
         elif isinstance(raw_tensor, numpy.ndarray):
             data.raw_tensor = raw_tensor  # leave it as it is
         else:
             raise TypeError(f"Unexpected type {type(raw_tensor)} for {k} in extern_data_raw.")
 
-        if batch_dim.size is None and batch_dim.dyn_size_ext is None:
-            batch_dim.dyn_size_ext = Tensor(batch_dim.name or "batch", dims=[], dtype="int32")
+        if batch_dim.dyn_size_ext and batch_dim.dyn_size_ext.raw_tensor is None:
             batch_dim.dyn_size_ext.raw_tensor = torch.tensor(extern_data_raw[k].shape[0], dtype=torch.int32)
 
         # This has certain assumptions on the dataset, the data pipeline and collate_batch.
         # Namely, we expect that we get the batch dim in the first dim (see collate_batch).
         # We also expect that the sequence lengths are in the second dim, if it is dynamic.
-        if len(data.dims) >= 2 and data.dims[1].dimension is None:
+        if (
+            len(data.dims) >= 2
+            and data.dims[1].size is None
+            and (not data.dims[1].dyn_size_ext or data.dims[1].dyn_size_ext.raw_tensor is None)
+        ):
             assert k + ":seq_len" in extern_data_raw, (
                 f"extern_data {data}, dyn spatial dim, missing {k}:seq_len in raw dict, "
                 f"check dataset or collate_batch"
             )
             size = extern_data_raw[k + ":seq_len"]
             # Sequence lengths have to be on CPU for the later call to rnn.pack_padded_sequence
             assert size.device.type == "cpu"
@@ -761,14 +767,25 @@
 def _get_batch_dim_from_extern_data(extern_data: TensorDict) -> Dim:
     # We expect that the batch dim is the first dim in any of the tensors.
     # See collate_batch.
     batch_dim = next(iter(extern_data.data.values())).dims[0]
     return batch_dim
 
 
+def _get_dyn_dims_from_extern_data(extern_data: TensorDict) -> List[Dim]:
+    visited = set()
+    res = []
+    for k, v in extern_data.data.items():
+        for dim in v.dims:
+            if dim not in visited and dim.size is None:
+                visited.add(dim)
+                res.append(dim)
+    return res
+
+
 def _print_process(report_prefix, step, eval_info):
     """
     Similar but simplified from TF engine _print_process.
 
     :param str report_prefix:
     :param int step:
     :param dict[str] eval_info: via :func:`_collect_eval_info`
```

### Comparing `returnn-1.20230718.112120/returnn/torch/frontend/_backend.py` & `returnn-1.20230718.124003/returnn/torch/frontend/_backend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/torch/frontend/_rand.py` & `returnn-1.20230718.124003/returnn/torch/frontend/_rand.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/torch/frontend/bridge.py` & `returnn-1.20230718.124003/returnn/torch/frontend/bridge.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/torch/updater.py` & `returnn-1.20230718.124003/returnn/torch/updater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/util/basic.py` & `returnn-1.20230718.124003/returnn/util/basic.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/util/better_exchook.py` & `returnn-1.20230718.124003/returnn/util/better_exchook.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/util/bpe.py` & `returnn-1.20230718.124003/returnn/util/bpe.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/util/debug.py` & `returnn-1.20230718.124003/returnn/util/debug.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/util/debug_helpers.py` & `returnn-1.20230718.124003/returnn/util/debug_helpers.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/util/fsa.py` & `returnn-1.20230718.124003/returnn/util/fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/util/literal_py_to_pickle.py` & `returnn-1.20230718.124003/returnn/util/literal_py_to_pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/util/pprint.py` & `returnn-1.20230718.124003/returnn/util/pprint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/util/py-to-pickle.cpp` & `returnn-1.20230718.124003/returnn/util/py-to-pickle.cpp`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/util/sig_proc.py` & `returnn-1.20230718.124003/returnn/util/sig_proc.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn/util/task_system.py` & `returnn-1.20230718.124003/returnn/util/task_system.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/returnn.egg-info/PKG-INFO` & `returnn-1.20230718.124003/returnn.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: returnn
-Version: 1.20230718.112120
+Version: 1.20230718.124003
 Summary: The RWTH extensible training framework for universal recurrent neural networks
 Home-page: https://github.com/rwth-i6/returnn/
 Author: Albert Zeyer
 Author-email: albzey@gmail.com
 License: RETURNN license
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
```

### Comparing `returnn-1.20230718.112120/returnn.egg-info/SOURCES.txt` & `returnn-1.20230718.124003/returnn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/setup.py` & `returnn-1.20230718.124003/setup.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/DummySprintExec.py` & `returnn-1.20230718.124003/tests/DummySprintExec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/PyCharm-inspection-profile.xml` & `returnn-1.20230718.124003/tests/PyCharm-inspection-profile.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/PyCharm.idea/codeStyleSettings.xml` & `returnn-1.20230718.124003/tests/PyCharm.idea/codeStyleSettings.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml` & `returnn-1.20230718.124003/tests/PyCharm.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/_set_num_threads1.py` & `returnn-1.20230718.124003/tests/_set_num_threads1.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/_setup_test_env.py` & `returnn-1.20230718.124003/tests/_setup_test_env.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/bpe-unicode-demo.codes` & `returnn-1.20230718.124003/tests/bpe-unicode-demo.codes`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/bpe-unicode-demo.vocab` & `returnn-1.20230718.124003/tests/bpe-unicode-demo.vocab`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/lexicon_opt.isyms` & `returnn-1.20230718.124003/tests/lexicon_opt.isyms`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/lexicon_opt.jpg` & `returnn-1.20230718.124003/tests/lexicon_opt.jpg`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/lint_common.py` & `returnn-1.20230718.124003/tests/lint_common.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/pycharm-inspect.py` & `returnn-1.20230718.124003/tests/pycharm-inspect.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/pylint.py` & `returnn-1.20230718.124003/tests/pylint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/returnn-as-framework.py` & `returnn-1.20230718.124003/tests/returnn-as-framework.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/rf_utils.py` & `returnn-1.20230718.124003/tests/rf_utils.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/spelling.dic` & `returnn-1.20230718.124003/tests/spelling.dic`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_Config.py` & `returnn-1.20230718.124003/tests/test_Config.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_Dataset.py` & `returnn-1.20230718.124003/tests/test_Dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_Fsa.py` & `returnn-1.20230718.124003/tests/test_Fsa.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_GeneratingDataset.py` & `returnn-1.20230718.124003/tests/test_GeneratingDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_HDFDataset.py` & `returnn-1.20230718.124003/tests/test_HDFDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_LearningRateControl.py` & `returnn-1.20230718.124003/tests/test_LearningRateControl.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_Log.py` & `returnn-1.20230718.124003/tests/test_Log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_MultiProcDataset.py` & `returnn-1.20230718.124003/tests/test_MultiProcDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_PTDataset.py` & `returnn-1.20230718.124003/tests/test_PTDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_Pretrain.py` & `returnn-1.20230718.124003/tests/test_Pretrain.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_ResNet.py` & `returnn-1.20230718.124003/tests/test_ResNet.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_SprintDataset.py` & `returnn-1.20230718.124003/tests/test_SprintDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_SprintInterface.py` & `returnn-1.20230718.124003/tests/test_SprintInterface.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_TFEngine.py` & `returnn-1.20230718.124003/tests/test_TFEngine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_TFNativeOp.py` & `returnn-1.20230718.124003/tests/test_TFNativeOp.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_TFNetworkLayer.py` & `returnn-1.20230718.124003/tests/test_TFNetworkLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_TFNetworkRecLayer.py` & `returnn-1.20230718.124003/tests/test_TFNetworkRecLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_TFNetworkSigProcLayer.py` & `returnn-1.20230718.124003/tests/test_TFNetworkSigProcLayer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_TFUpdater.py` & `returnn-1.20230718.124003/tests/test_TFUpdater.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_TFUtil.py` & `returnn-1.20230718.124003/tests/test_TFUtil.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_TF_determinism.py` & `returnn-1.20230718.124003/tests/test_TF_determinism.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_TaskSystem.py` & `returnn-1.20230718.124003/tests/test_TaskSystem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_TaskSystem_SharedMem.py` & `returnn-1.20230718.124003/tests/test_TaskSystem_SharedMem.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_TranslationDataset.py` & `returnn-1.20230718.124003/tests/test_TranslationDataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_Util.py` & `returnn-1.20230718.124003/tests/test_Util.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_demos.py` & `returnn-1.20230718.124003/tests/test_demos.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_fork_exec.py` & `returnn-1.20230718.124003/tests/test_fork_exec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_hdf_dump.py` & `returnn-1.20230718.124003/tests/test_hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_rf_array.py` & `returnn-1.20230718.124003/tests/test_rf_array.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_rf_attention.py` & `returnn-1.20230718.124003/tests/test_rf_attention.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_rf_base.py` & `returnn-1.20230718.124003/tests/test_rf_base.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_rf_cond.py` & `returnn-1.20230718.124003/tests/test_rf_cond.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_rf_const.py` & `returnn-1.20230718.124003/tests/test_rf_const.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_rf_container.py` & `returnn-1.20230718.124003/tests/test_rf_container.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_rf_conv.py` & `returnn-1.20230718.124003/tests/test_rf_conv.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_rf_encoder_conformer.py` & `returnn-1.20230718.124003/tests/test_rf_encoder_conformer.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_rf_loop.py` & `returnn-1.20230718.124003/tests/test_rf_loop.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_rf_math.py` & `returnn-1.20230718.124003/tests/test_rf_math.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_rf_normalization.py` & `returnn-1.20230718.124003/tests/test_rf_normalization.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_rf_rec.py` & `returnn-1.20230718.124003/tests/test_rf_rec.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_rf_reduce.py` & `returnn-1.20230718.124003/tests/test_rf_reduce.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_rf_signal.py` & `returnn-1.20230718.124003/tests/test_rf_signal.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_tensor.py` & `returnn-1.20230718.124003/tests/test_tensor.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_tools.py` & `returnn-1.20230718.124003/tests/test_tools.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_torch_engine.py` & `returnn-1.20230718.124003/tests/test_torch_engine.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_torch_frontend.py` & `returnn-1.20230718.124003/tests/test_torch_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tests/test_torch_internal_frontend.py` & `returnn-1.20230718.124003/tests/test_torch_internal_frontend.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/analyze-dataset-batches.py` & `returnn-1.20230718.124003/tools/analyze-dataset-batches.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/bliss-collect-seq-lens.py` & `returnn-1.20230718.124003/tools/bliss-collect-seq-lens.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/bliss-dump-text.py` & `returnn-1.20230718.124003/tools/bliss-dump-text.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/bliss-get-segment-names.py` & `returnn-1.20230718.124003/tools/bliss-get-segment-names.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/bliss-to-ogg-zip.py` & `returnn-1.20230718.124003/tools/bliss-to-ogg-zip.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/bpe-create-lexicon.py` & `returnn-1.20230718.124003/tools/bpe-create-lexicon.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/calculate-word-error-rate.py` & `returnn-1.20230718.124003/tools/calculate-word-error-rate.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/cleanup-old-models.py` & `returnn-1.20230718.124003/tools/cleanup-old-models.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/collect-orth-symbols.py` & `returnn-1.20230718.124003/tools/collect-orth-symbols.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/collect-words.py` & `returnn-1.20230718.124003/tools/collect-words.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/compile_native_op.py` & `returnn-1.20230718.124003/tools/compile_native_op.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/compile_tf_graph.py` & `returnn-1.20230718.124003/tools/compile_tf_graph.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/debug-dump-search-scores.py` & `returnn-1.20230718.124003/tools/debug-dump-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/debug-plot-search-scores.py` & `returnn-1.20230718.124003/tools/debug-plot-search-scores.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/dump-dataset-raw-strings.py` & `returnn-1.20230718.124003/tools/dump-dataset-raw-strings.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/dump-dataset.py` & `returnn-1.20230718.124003/tools/dump-dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/dump-forward-stats.py` & `returnn-1.20230718.124003/tools/dump-forward-stats.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/dump-forward.py` & `returnn-1.20230718.124003/tools/dump-forward.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/dump-network-json.py` & `returnn-1.20230718.124003/tools/dump-network-json.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/dump-pickle.py` & `returnn-1.20230718.124003/tools/dump-pickle.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/extract_state_tying_from_dataset.py` & `returnn-1.20230718.124003/tools/extract_state_tying_from_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/get-attention-weights.py` & `returnn-1.20230718.124003/tools/get-attention-weights.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/get-best-model-epoch.py` & `returnn-1.20230718.124003/tools/get-best-model-epoch.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/hdf_dump.py` & `returnn-1.20230718.124003/tools/hdf_dump.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/hdf_dump_translation_dataset.py` & `returnn-1.20230718.124003/tools/hdf_dump_translation_dataset.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/import-blocks-mt-model.py` & `returnn-1.20230718.124003/tools/import-blocks-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/import-t2t-mt-model.py` & `returnn-1.20230718.124003/tools/import-t2t-mt-model.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/lattice_rescorer/Makefile` & `returnn-1.20230718.124003/tools/lattice_rescorer/Makefile`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/lattice_rescorer/README.md` & `returnn-1.20230718.124003/tools/lattice_rescorer/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/lattice_rescorer/example/README.md` & `returnn-1.20230718.124003/tools/lattice_rescorer/example/README.md`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config` & `returnn-1.20230718.124003/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config` & `returnn-1.20230718.124003/tools/lattice_rescorer/example/network.040/i600_m600_m600.sgd_b16_lr0_cl2.newbobabs.keep_over_epoch.lstm2.config`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/lattice_rescorer/example/rescore_lattice.sh` & `returnn-1.20230718.124003/tools/lattice_rescorer/example/rescore_lattice.sh`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/lattice_rescorer/file.h` & `returnn-1.20230718.124003/tools/lattice_rescorer/file.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/lattice_rescorer/htklatticerescorer.cc` & `returnn-1.20230718.124003/tools/lattice_rescorer/htklatticerescorer.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/lattice_rescorer/htklatticerescorer.h` & `returnn-1.20230718.124003/tools/lattice_rescorer/htklatticerescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/lattice_rescorer/main.cc` & `returnn-1.20230718.124003/tools/lattice_rescorer/main.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/lattice_rescorer/rescorer.h` & `returnn-1.20230718.124003/tools/lattice_rescorer/rescorer.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/lattice_rescorer/vocabulary.cc` & `returnn-1.20230718.124003/tools/lattice_rescorer/vocabulary.cc`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/lattice_rescorer/vocabulary.h` & `returnn-1.20230718.124003/tools/lattice_rescorer/vocabulary.h`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/tf_avg_checkpoints.py` & `returnn-1.20230718.124003/tools/tf_avg_checkpoints.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/tf_inspect_checkpoint.py` & `returnn-1.20230718.124003/tools/tf_inspect_checkpoint.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/tf_inspect_summary_log.py` & `returnn-1.20230718.124003/tools/tf_inspect_summary_log.py`

 * *Files identical despite different names*

### Comparing `returnn-1.20230718.112120/tools/torch_export_to_onnx.py` & `returnn-1.20230718.124003/tools/torch_export_to_onnx.py`

 * *Files identical despite different names*

