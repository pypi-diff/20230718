# Comparing `tmp/datumaro-1.4.0rc2.tar.gz` & `tmp/datumaro-1.4.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datumaro-1.4.0rc2.tar", last modified: Tue Jul 11 06:20:52 2023, max compression
+gzip compressed data, was "datumaro-1.4.0rc3.tar", last modified: Tue Jul 18 06:06:24 2023, max compression
```

## Comparing `datumaro-1.4.0rc2.tar` & `datumaro-1.4.0rc3.tar`

### file list

```diff
@@ -1,361 +1,367 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.746774 datumaro-1.4.0rc2/
--rw-r--r--   0 runner    (1001) docker     (123)   375078 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/3rd-party.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/NOTICE
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-11 06:20:52.746774 datumaro-1.4.0rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      860 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/requirements-core.txt
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/requirements-default.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-11 06:20:52.746774 datumaro-1.4.0rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.674769 datumaro-1.4.0rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.698771 datumaro-1.4.0rc2/src/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.702771 datumaro-1.4.0rc2/src/datumaro/capi/
--rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/capi/pybind.cpp
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.702771 datumaro-1.4.0rc2/src/datumaro/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.706771 datumaro-1.4.0rc2/src/datumaro/cli/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/detect_format.py
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/explain.py
--rw-r--r--   0 runner    (1001) docker     (123)     5392 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/explore.py
--rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/info.py
--rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/patch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.706771 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.706771 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/create.py
--rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.706771 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/checkout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/commit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/log.py
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/commands/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.706771 datumaro-1.4.0rc2/src/datumaro/cli/contexts/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/contexts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/contexts/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.706771 datumaro-1.4.0rc2/src/datumaro/cli/contexts/project/
--rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/contexts/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/contexts/source.py
--rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/contexts/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.710772 datumaro-1.4.0rc2/src/datumaro/cli/util/
--rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/util/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/util/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/cli/util/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/abstracts/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/abstracts/model_interpreter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/explorer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/prune.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/algorithms/noisy_label_detection/
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/algorithms/rise.py
--rw-r--r--   0 runner    (1001) docker     (123)    30855 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/annotation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/annotations/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/annotations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/annotations/matcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/annotations/merger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/cli_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    25024 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/comparator.py
--rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/config_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/crypter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29610 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    13445 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/dataset_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/dataset_item_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    26030 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/dataset_storage.py
--rw-r--r--   0 runner    (1001) docker     (123)    11949 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    14348 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/extractor_tfds.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/format_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/hl_ops/
--rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/hl_ops/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9950 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/launcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/lazy_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    36061 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/media_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.714772 datumaro-1.4.0rc2/src/datumaro/components/merge/
--rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/merge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/merge/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12216 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/merge/exact_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/merge/intersect_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)     4453 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/merge/union_merge.py
--rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/operations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5221 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/progress_reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    89457 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/shift_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4436 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/validator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22880 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/components/visualizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.718772 datumaro-1.4.0rc2/src/datumaro/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.718772 datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.718772 datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/details/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.722772 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ade20k2017.py
--rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ade20k2020.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.722772 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.726773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/media.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.726773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ava/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ava/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ava/ava.py
--rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/brats.py
--rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/brats_numpy.py
--rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/camvid.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.726773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/celeba/
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/celeba/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/celeba/align_celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/celeba/celeba.py
--rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cifar.py
--rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cityscapes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.726773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21198 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    28677 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/common_super_resolution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.726773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.726773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11499 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15616 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.730773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6839 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.730773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.730773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/icdar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/icdar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/icdar/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/icdar/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/icdar/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/image_dir.py
--rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/image_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/imagenet.py
--rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/imagenet_txt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kinetics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.730773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.730773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/labelme.py
--rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/lfw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.730773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/market1501.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mnist.py
--rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mnist_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mots.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.734773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/mpii_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.734773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/nyu_depth_v2.py
--rw-r--r--   0 runner    (1001) docker     (123)    38738 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/open_images.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.734773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/roboflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/roboflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11005 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/roboflow/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7169 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/roboflow/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.734773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.734773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/sly_pointcloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.734773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/importer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.738773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/tf_detection_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/tf_detection_api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/tf_detection_api/format.py
--rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/vgg_face2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/video.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.738773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16682 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    31336 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     3484 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/vott_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/vott_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/widerface.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.738773 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13857 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/exporter.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/importer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/explorer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.738773 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/ovms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.738773 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/triton.py
--rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/missing_annotation_detection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/ndr.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.738773 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.742774 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/coco.class
--rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/shift_launcher.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.742774 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.742774 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/algorithm/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/algorithm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/algorithm/algorithm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/algorithm/entropy.py
--rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/random_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/sampler/relevancy_sampler.py
--rw-r--r--   0 runner    (1001) docker     (123)    47069 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/specs.json
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/specs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.742774 datumaro-1.4.0rc2/src/datumaro/plugins/synthetic_data/
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/synthetic_data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/synthetic_data/background_colors.txt
--rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/synthetic_data/image_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/synthetic_data/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.742774 datumaro-1.4.0rc2/src/datumaro/plugins/tiling/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/tiling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/tiling/merge_tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/tiling/tile.py
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/tiling/util.py
--rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)    44130 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/plugins/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/project.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.746774 datumaro-1.4.0rc2/src/datumaro/util/
--rw-r--r--   0 runner    (1001) docker     (123)     4809 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/annotation_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/attrs_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/file_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/image.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/image_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/log_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/mask_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/meta_file_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/os_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/pickle_util.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/samples.py
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/scope.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/telemetry_stub.py
--rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/telemetry_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/util/tf_util.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-11 06:20:41.000000 datumaro-1.4.0rc2/src/datumaro/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-11 06:20:52.702771 datumaro-1.4.0rc2/src/datumaro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-11 06:20:52.000000 datumaro-1.4.0rc2/src/datumaro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    14297 2023-07-11 06:20:52.000000 datumaro-1.4.0rc2/src/datumaro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-11 06:20:52.000000 datumaro-1.4.0rc2/src/datumaro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-11 06:20:52.000000 datumaro-1.4.0rc2/src/datumaro.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-07-11 06:20:52.000000 datumaro-1.4.0rc2/src/datumaro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-11 06:20:52.000000 datumaro-1.4.0rc2/src/datumaro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.355518 datumaro-1.4.0rc3/
+-rw-r--r--   0 runner    (1001) docker     (123)   391964 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/3rd-party.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-18 06:06:24.351518 datumaro-1.4.0rc3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5571 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2642 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/requirements-core.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/requirements-default.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 06:06:24.355518 datumaro-1.4.0rc3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.267516 datumaro-1.4.0rc3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.283517 datumaro-1.4.0rc3/src/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.283517 datumaro-1.4.0rc3/src/datumaro/capi/
+-rw-r--r--   0 runner    (1001) docker     (123)     3379 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/capi/pybind.cpp
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.283517 datumaro-1.4.0rc3/src/datumaro/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5686 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.287517 datumaro-1.4.0rc3/src/datumaro/cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5509 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/detect_format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/explain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6640 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/explore.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9046 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4238 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10289 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/patch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4158 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.287517 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.291517 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5247 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1957 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/create.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5926 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.291517 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/checkout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/commit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2758 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3831 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4851 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/commands/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.291517 datumaro-1.4.0rc3/src/datumaro/cli/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9089 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/contexts/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.291517 datumaro-1.4.0rc3/src/datumaro/cli/contexts/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     4501 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/contexts/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/contexts/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4097 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/contexts/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.295517 datumaro-1.4.0rc3/src/datumaro/cli/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     4007 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13342 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/util/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/util/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5640 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/cli/util/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.299517 datumaro-1.4.0rc3/src/datumaro/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.299517 datumaro-1.4.0rc3/src/datumaro/components/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/abstracts/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1840 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/abstracts/model_interpreter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.303517 datumaro-1.4.0rc3/src/datumaro/components/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.303517 datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/explorer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13260 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/prune.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.303517 datumaro-1.4.0rc3/src/datumaro/components/algorithms/noisy_label_detection/
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/noisy_label_detection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8837 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8186 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/algorithms/rise.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30855 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/annotation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.303517 datumaro-1.4.0rc3/src/datumaro/components/annotations/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/annotations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11341 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/annotations/matcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5380 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/annotations/merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/cli_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25024 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/comparator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8101 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3570 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/config_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.303517 datumaro-1.4.0rc3/src/datumaro/components/contexts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/contexts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/contexts/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2240 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/crypter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29629 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11815 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/dataset_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6231 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/dataset_item_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26030 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/dataset_storage.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12020 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18063 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14348 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19651 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/extractor_tfds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19989 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/format_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.303517 datumaro-1.4.0rc3/src/datumaro/components/hl_ops/
+-rw-r--r--   0 runner    (1001) docker     (123)    11332 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/hl_ops/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4949 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/launcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3031 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/lazy_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36061 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/media_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.307517 datumaro-1.4.0rc3/src/datumaro/components/merge/
+-rw-r--r--   0 runner    (1001) docker     (123)     3694 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/merge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/merge/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12380 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/merge/exact_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1979 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/merge/extractor_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24284 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/merge/intersect_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/merge/union_merge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13417 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/operations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5310 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/progress_reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    89457 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9278 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/shift_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22880 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/components/visualizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.307517 datumaro-1.4.0rc3/src/datumaro/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.307517 datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.311517 datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/details/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/details/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.315517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ade20k2017.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8600 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ade20k2020.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.319517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5963 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15043 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2129 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.319517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2607 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10224 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/media.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.319517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ava/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ava/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8758 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ava/ava.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5585 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/brats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3875 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/brats_numpy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17705 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/camvid.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.319517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/celeba/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/celeba/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7823 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/celeba/align_celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10759 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/celeba/celeba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12457 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cifar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21483 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cityscapes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.323517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23394 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28679 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/extractor_merger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6779 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11404 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/page_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6517 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/common_semantic_segmentation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3317 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/common_super_resolution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.323517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16020 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21501 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.323517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16683 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15771 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.323517 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7227 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11135 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1921 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.327518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11105 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1563 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.327518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/icdar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/icdar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12137 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/icdar/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6522 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/icdar/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/icdar/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1995 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/image_dir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/image_zip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7773 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/imagenet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8357 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/imagenet_txt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5877 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kinetics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.327518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6210 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3970 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.331518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11401 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17906 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20081 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/labelme.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15150 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/lfw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.331518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11577 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12609 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6508 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/market1501.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9234 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mnist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7220 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mnist_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10932 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.331518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5407 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/mpii_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/mpii_mat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.331518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4819 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/nyu_depth_v2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38738 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/open_images.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.335518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/roboflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/roboflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11062 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/roboflow/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/roboflow/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.335518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.335518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/sly_pointcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/sly_pointcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7083 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/sly_pointcloud/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16317 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/sly_pointcloud/format.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.335518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6671 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/importer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.339518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/tf_detection_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/tf_detection_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8367 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/tf_detection_api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8966 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/tf_detection_api/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15663 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/vgg_face2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6453 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/video.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.339518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16675 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31336 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/vott_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4107 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/vott_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10301 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/widerface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.339518 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13949 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12142 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/exporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6315 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/importer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.339518 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4891 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/ovms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.343518 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/triton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6226 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/missing_annotation_detection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16787 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/ndr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.343518 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9596 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.343518 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1757 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/coco.class
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10475 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/imagenet.class
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1233 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/shift_launcher.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.347518 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.347518 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/algorithm/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/algorithm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/algorithm/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/algorithm/entropy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7786 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8772 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/sampler/relevancy_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47069 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/specs.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32124 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.347518 datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11335 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/background_colors.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    11650 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/image_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6194 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.347518 datumaro-1.4.0rc3/src/datumaro/plugins/tiling/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/tiling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9398 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/tiling/merge_tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9834 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/tiling/tile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/tiling/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48788 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44130 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/plugins/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/project.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.351518 datumaro-1.4.0rc3/src/datumaro/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/annotation_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/attrs_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/file_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11843 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/image_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/log_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12034 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/mask_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/meta_file_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8479 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/os_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/pickle_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/samples.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/scope.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/telemetry_stub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6079 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/telemetry_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/util/tf_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 06:06:15.000000 datumaro-1.4.0rc3/src/datumaro/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:06:24.283517 datumaro-1.4.0rc3/src/datumaro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6119 2023-07-18 06:06:24.000000 datumaro-1.4.0rc3/src/datumaro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    14550 2023-07-18 06:06:24.000000 datumaro-1.4.0rc3/src/datumaro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:06:24.000000 datumaro-1.4.0rc3/src/datumaro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 06:06:24.000000 datumaro-1.4.0rc3/src/datumaro.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-18 06:06:24.000000 datumaro-1.4.0rc3/src/datumaro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 06:06:24.000000 datumaro-1.4.0rc3/src/datumaro.egg-info/top_level.txt
```

### Comparing `datumaro-1.4.0rc2/3rd-party.txt` & `datumaro-1.4.0rc3/3rd-party.txt`

 * *Files 1% similar despite different names*

```diff
@@ -6973,9 +6973,332 @@
 OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 Code generated by the Protocol Buffer compiler is owned by the owner
 of the input file used when generating it.  This code is not
 standalone and requires a support library to be linked with it.  This
 support library is itself covered by the above license.
 -------------------------------------------------------------
+tabulate
+
+MIT
+
+Copyright (c) 2011-2020 Sergey Astanin and contributors
+
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
+
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+-------------------------------------------------------------
+ovmsclient
+
+Apache-2.0
+
+Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+
+-------------------------------------------------------------
+tritonclient
+
+BSD-3-Clause
+
+Copyright (c) 2021, NVIDIA CORPORATION. All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions
+are met:
+ * Redistributions of source code must retain the above copyright
+   notice, this list of conditions and the following disclaimer.
+ * Redistributions in binary form must reproduce the above copyright
+   notice, this list of conditions and the following disclaimer in the
+   documentation and/or other materials provided with the distribution.
+ * Neither the name of NVIDIA CORPORATION nor the names of its
+   contributors may be used to endorse or promote products derived
+   from this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS ``AS IS'' AND ANY
+EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+PURPOSE ARE DISCLAIMED.  IN NO EVENT SHALL THE COPYRIGHT OWNER OR
+CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL,
+EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
+PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
+PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY
+OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+(INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+-------------------------------------------------------------
+scikit-learn
+
+BSD-3-Clause
+
+Copyright (c) 2007-2023 The scikit-learn developers.
+All rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions are met:
+
+* Redistributions of source code must retain the above copyright notice, this
+  list of conditions and the following disclaimer.
+
+* Redistributions in binary form must reproduce the above copyright notice,
+  this list of conditions and the following disclaimer in the documentation
+  and/or other materials provided with the distribution.
+
+* Neither the name of the copyright holder nor the names of its
+  contributors may be used to endorse or promote products derived from
+  this software without specific prior written permission.
+
+THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS"
+AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE
+FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR
+SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
+CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
+OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
+OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+-------------------------------------------------------------
+json-stream
+
+MIT
+
+Copyright (c) 2020 Jamie Cockburn
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of
+this software and associated documentation files (the "Software"), to deal in
+the Software without restriction, including without limitation the rights to
+use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
+of the Software, and to permit persons to whom the Software is furnished to do
+so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+-------------------------------------------------------------
+
 
 * Other names and brands may be claimed as the property of others.
```

### Comparing `datumaro-1.4.0rc2/LICENSE` & `datumaro-1.4.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/PKG-INFO` & `datumaro-1.4.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.4.0rc2
+Version: 1.4.0rc3
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.4.0rc2/README.md` & `datumaro-1.4.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/pyproject.toml` & `datumaro-1.4.0rc3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/requirements-core.txt` & `datumaro-1.4.0rc3/requirements-core.txt`

 * *Files 12% similar despite different names*

```diff
@@ -53,7 +53,10 @@
 
 # Model inference launcher from the dedicated inference server
 ovmsclient
 tritonclient[all]
 
 # prune
 scikit-learn
+
+# Stream JSON parser
+json-stream
```

### Comparing `datumaro-1.4.0rc2/setup.py` & `datumaro-1.4.0rc3/setup.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/__init__.py` & `datumaro-1.4.0rc3/src/datumaro/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/capi/pybind.cpp` & `datumaro-1.4.0rc3/src/datumaro/capi/pybind.cpp`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/__main__.py` & `datumaro-1.4.0rc3/src/datumaro/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/__init__.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/compare.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/compare.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/convert.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/convert.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/detect_format.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/detect_format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/download.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/download.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/explain.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/explain.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/explore.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/patch.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,161 +1,164 @@
-# Copyright (C) 2023 Intel Corporation
+# Copyright (C) 2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
 import os
 import os.path as osp
-import shutil
 
-from datumaro.components.algorithms.hash_key_inference.explorer import Explorer
+from datumaro.components.environment import DEFAULT_ENVIRONMENT
 from datumaro.components.errors import ProjectNotFoundError
-from datumaro.util import str_to_bool
 from datumaro.util.scope import scope_add, scoped
 
 from ..util import MultilineFormatter
+from ..util.errors import CliException
 from ..util.project import load_project, parse_full_revpath
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
     parser = parser_ctor(
-        help="Explore similar data of query in dataset",
+        help="Updates dataset from another one",
         description="""
-        Applies data exploration to a dataset for image/text query.
-        The command can be useful if you have to find similar data in dataset.
+        Updates items of the first dataset with items from the second one.|n
         |n
-        The current project (-p/--project) is used as a context for plugins
-        and models. It is used when there is a dataset path in target.
+        By default, datasets are updated in-place. The '-o/--output-dir'
+        option can be used to specify another output directory. When
+        updating in-place, use the '--overwrite' parameter along with the
+        '--save-images' export option (in-place updates fail by default
+        to prevent data loss).|n
+        |n
+        Unlike the regular project data source joining, the datasets are not
+        required to have the same labels. The labels from the "patch"
+        dataset are projected onto the labels of the patched dataset,
+        so only the annotations with the matching labels are used, i.e.
+        all the annotations having unknown labels are ignored. Currently,
+        this command doesn't allow to update the label information in the
+        patched dataset.|n
+        |n
+        The command supports passing extra exporting options for the output
+        dataset. The extra options should be passed after the main arguments
+        and after the '--' separator. Particularly, this is useful to include
+        images in the output dataset with '--save-images'.|n
+        |n
+        This command can be applied to the current project targets or
+        arbitrary datasets outside a project. Note that if the target dataset
+        is read-only (e.g. if it is a project, stage or a cache entry),
+        the output directory must be provided.|n
+        |n
+        This command has the following invocation syntax:
+        - %(prog)s <target dataset revpath> <patch dataset revpath>|n
+        |n
+        <revpath> - either a dataset path or a revision path. The full
+        syntax is:|n
+        - Dataset paths:|n
+        |s|s- <dataset path>[ :<format> ]|n
+        - Revision paths:|n
+        |s|s- <project path> [ @<rev> ] [ :<target> ]|n
+        |s|s- <rev> [ :<target> ]|n
+        |s|s- <target>|n
+        |n
+        The current project (-p/--project) is also used as a context for
+        plugins, so it can be useful for dataset paths having custom formats.
         When not specified, the current project's working tree is used.|n
         |n
         Examples:|n
-        - Explore top50 similar images of image query in COCO dataset:|n
-        |s|s%(prog)s -q path/to/image.jpg -topk 50|n
-        - Explore top50 similar images of text query, elephant, in COCO dataset:|n
-        |s|s%(prog)s -q elephant -topk 50|n
-        - Explore top50 similar images of image query list in COCO dataset:|n
-        |s|s%(prog)s -q path/to/image1.jpg/ path/to/image2.jpg/ path/to/image3.jpg/ -topk 50|n
-        - Explore top50 similar images of text query list in COCO dataset:|n
-        |s|s%(prog)s -q motorcycle/ bus/ train/ -topk 50
+        - Update a VOC-like dataset with COCO-like annotations:|n
+        |s|s%(prog)s --overwrite dataset1/:voc dataset2/:coco -- --save-images|n
+        |n
+        - Generate a patched dataset, based on a project:|n
+        |s|s%(prog)s -o patched_proj1/ proj1/ proj2/|n
+        |n
+        - Update the "source1" source in the current project with a dataset:|n
+        |s|s%(prog)s -p proj/ --overwrite source1 path/to/dataset2:coco|n
+        |n
+        - Generate a patched source from a previous revision and a dataset:|n
+        |s|s%(prog)s -o new_src2/ HEAD~2:source-2 path/to/dataset2:yolo|n
+        |n
+        - Update a dataset in a custom format, described in a project plugin:|n
+        |s|s%(prog)s -p proj/ --overwrite dataset/:my_format dataset2/:coco
         """,
         formatter_class=MultilineFormatter,
     )
 
-    parser.add_argument("target", nargs="?", help="Target dataset")
+    parser.add_argument("target", help="Target dataset revpath")
+    parser.add_argument("patch", help="Patch dataset revpath")
     parser.add_argument(
-        "-q",
-        "--query",
-        dest="query",
-        required=True,
-        help="Image path or id of query to explore similar data",
+        "-o",
+        "--output-dir",
+        dest="dst_dir",
+        default=None,
+        help="Output directory (default: save in-place)",
+    )
+    parser.add_argument(
+        "--overwrite",
+        action="store_true",
+        help="Overwrite existing files in the save directory, " "if it is not empty",
     )
-    parser.add_argument("-topk", type=int, dest="topk", help="Number of similar results")
     parser.add_argument(
         "-p",
         "--project",
         dest="project_dir",
-        help="Directory of the project to operate on (default: current dir)",
-    )
-    parser.add_argument(
-        "-s",
-        "--save",
-        action="store_true",
-        default=False,
-        help="Save explorer result files on explore_result folder",
+        help="Directory of the 'current' project (default: current dir)",
     )
     parser.add_argument(
-        "--stage",
-        type=str_to_bool,
-        default=True,
-        help="""
-            Include this action as a project build step.
-            If true, this operation will be saved in the project
-            build tree, allowing to reproduce the resulting dataset later.
-            Applicable only to main project targets (i.e. data sources
-            and the 'project' target, but not intermediate stages)
-            (default: %(default)s)
-            """,
+        "extra_args",
+        nargs=argparse.REMAINDER,
+        help="Additional arguments for exporting (pass '-- -h' for help). "
+        "Must be specified after the main command arguments and after "
+        "the '--' separator",
     )
-    parser.set_defaults(command=explore_command)
+    parser.set_defaults(command=patch_command)
 
     return parser
 
 
 def get_sensitive_args():
     return {
-        explore_command: [
-            "target",
-            "query",
-            "topk",
-            "project_dir",
-        ]
+        patch_command: ["target", "patch", "dst_dir", "project_dir", "extra_args"],
     }
 
 
 @scoped
-def explore_command(args):
+def patch_command(args):
     project = None
     try:
         project = scope_add(load_project(args.project_dir))
     except ProjectNotFoundError:
         if args.project_dir:
             raise
 
-    if args.target:
-        targets = [args.target]
+    if project is not None:
+        env = project.env
     else:
-        targets = list(project.working_tree.sources)
+        env = DEFAULT_ENVIRONMENT
 
-    source_datasets = []
-    for target in targets:
-        target_dataset, _ = parse_full_revpath(target, project)
-        source_datasets.append(target_dataset)
-
-    explorer_args = {"save_hashkey": True}
-    build_tree = project.working_tree.clone()
-    for target in targets:
-        build_tree.build_targets.add_explore_stage(target, params=explorer_args)
-
-    explorer = Explorer(*source_datasets)
-    for dataset in source_datasets:
-        dst_dir = dataset.data_path
-        dataset.save(dst_dir, save_media=True, save_hashkey_meta=True)
-
-    if args.stage:
-        project.working_tree.config.update(build_tree.config)
-        project.working_tree.save()
-
-    # Get query datasetitem through query path
-    if osp.exists(args.query):
-        query_datasetitem = None
-        for dataset in source_datasets:
-            try:
-                query_datasetitem = dataset.get_datasetitem_by_path(args.query)
-            except Exception:
-                continue
-            if not query_datasetitem:
-                break
-    else:
-        query_datasetitem = args.query
+    target_dataset, _project = parse_full_revpath(args.target, project)
+    if _project is not None:
+        scope_add(_project)
+
+    try:
+        exporter = env.exporters[target_dataset.format]
+    except KeyError:
+        raise CliException("Exporter for format '%s' is not found" % args.format)
+
+    extra_args = exporter.parse_cmdline(args.extra_args)
+
+    dst_dir = args.dst_dir or target_dataset.data_path
+    if not args.overwrite and osp.isdir(dst_dir) and os.listdir(dst_dir):
+        raise CliException(
+            "Directory '%s' already exists " "(pass --overwrite to overwrite)" % dst_dir
+        )
+    dst_dir = osp.abspath(dst_dir)
+
+    patch_dataset, _project = parse_full_revpath(args.patch, project)
+    if _project is not None:
+        scope_add(_project)
+
+    target_dataset.update(patch_dataset)
 
-    results = explorer.explore_topk(query_datasetitem, args.topk)
+    target_dataset.save(save_dir=dst_dir, **extra_args)
 
-    result_path_list = []
-    log.info(f"Most similar {args.topk} results of query in dataset")
-    for result in results:
-        path = getattr(result.media, "path", None)
-        result_path_list.append(path)
-        log.info(f"id: {result.id} | subset: {result.subset} | path : {path}")
-
-    if args.save:
-        saved_result_path = osp.join(args.project_dir, "explore_result")
-        if osp.exists(saved_result_path):
-            shutil.rmtree(saved_result_path)
-        os.makedirs(saved_result_path)
-        for result in results:
-            saved_subset_path = osp.join(saved_result_path, result.subset)
-            if not osp.exists(saved_subset_path):
-                os.makedirs(saved_subset_path)
-            shutil.copyfile(path, osp.join(saved_subset_path, result.id + ".jpg"))
+    log.info("Patched dataset has been saved to '%s'" % dst_dir)
 
     return 0
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/filter.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/generate.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/generate.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/info.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/merge.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/patch.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/export.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,164 +1,181 @@
-# Copyright (C) 2021 Intel Corporation
+# Copyright (C) 2019-2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
 import os
 import os.path as osp
 
 from datumaro.components.environment import DEFAULT_ENVIRONMENT
 from datumaro.components.errors import ProjectNotFoundError
+from datumaro.components.project import ProjectBuildTargets
+from datumaro.util.os_util import make_file_name
 from datumaro.util.scope import scope_add, scoped
 
-from ..util import MultilineFormatter
-from ..util.errors import CliException
-from ..util.project import load_project, parse_full_revpath
+from ....util import MultilineFormatter
+from ....util.errors import CliException
+from ....util.project import FilterModes, generate_next_file_name, load_project
+
+__all__ = [
+    "build_parser",
+    "get_sensitive_args",
+]
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
+    builtins = sorted(DEFAULT_ENVIRONMENT.exporters)
+
     parser = parser_ctor(
-        help="Updates dataset from another one",
+        help="Export project",
         description="""
-        Updates items of the first dataset with items from the second one.|n
+        Exports a project in some format.|n
         |n
-        By default, datasets are updated in-place. The '-o/--output-dir'
-        option can be used to specify another output directory. When
-        updating in-place, use the '--overwrite' parameter along with the
-        '--save-images' export option (in-place updates fail by default
-        to prevent data loss).|n
-        |n
-        Unlike the regular project data source joining, the datasets are not
-        required to have the same labels. The labels from the "patch"
-        dataset are projected onto the labels of the patched dataset,
-        so only the annotations with the matching labels are used, i.e.
-        all the annotations having unknown labels are ignored. Currently,
-        this command doesn't allow to update the label information in the
-        patched dataset.|n
-        |n
-        The command supports passing extra exporting options for the output
-        dataset. The extra options should be passed after the main arguments
-        and after the '--' separator. Particularly, this is useful to include
-        images in the output dataset with '--save-images'.|n
-        |n
-        This command can be applied to the current project targets or
-        arbitrary datasets outside a project. Note that if the target dataset
-        is read-only (e.g. if it is a project, stage or a cache entry),
-        the output directory must be provided.|n
-        |n
-        This command has the following invocation syntax:
-        - %(prog)s <target dataset revpath> <patch dataset revpath>|n
-        |n
-        <revpath> - either a dataset path or a revision path. The full
-        syntax is:|n
-        - Dataset paths:|n
-        |s|s- <dataset path>[ :<format> ]|n
-        - Revision paths:|n
-        |s|s- <project path> [ @<rev> ] [ :<target> ]|n
-        |s|s- <rev> [ :<target> ]|n
-        |s|s- <target>|n
-        |n
-        The current project (-p/--project) is also used as a context for
-        plugins, so it can be useful for dataset paths having custom formats.
-        When not specified, the current project's working tree is used.|n
+        Each dataset format has its own export
+        options, which are passed after the '--' separator (see examples),
+        pass '-- -h' for more info. If not stated otherwise, by default
+        only annotations are exported, to include images pass
+        '--save-images' parameter.|n
+        |n
+        A filter can be passed, check the 'filter' command description for
+        more info.|n
+        |n
+        Formats:|n
+        Datasets come in a wide variety of formats. Each dataset
+        format defines its own data structure and rules on how to
+        interpret the data. Check the user manual for the list of
+        supported formats, examples and documentation.
+        |n
+        The list of supported formats can be extended by plugins.
+        Check the "plugins" section of the developer guide for information
+        about plugin implementation.|n
+        |n
+        List of builtin dataset formats: {}|n
+        |n
+        The command can only be applied to a project build target, a stage
+        or the combined 'project' target, in which case all the targets will
+        be affected.
         |n
         Examples:|n
-        - Update a VOC-like dataset with COCO-like annotations:|n
-        |s|s%(prog)s --overwrite dataset1/:voc dataset2/:coco -- --save-images|n
-        |n
-        - Generate a patched dataset, based on a project:|n
-        |s|s%(prog)s -o patched_proj1/ proj1/ proj2/|n
-        |n
-        - Update the "source1" source in the current project with a dataset:|n
-        |s|s%(prog)s -p proj/ --overwrite source1 path/to/dataset2:coco|n
-        |n
-        - Generate a patched source from a previous revision and a dataset:|n
-        |s|s%(prog)s -o new_src2/ HEAD~2:source-2 path/to/dataset2:yolo|n
+        - Export project as a VOC-like dataset, include images:|n
+        |s|s%(prog)s -f voc -- --save-images|n
         |n
-        - Update a dataset in a custom format, described in a project plugin:|n
-        |s|s%(prog)s -p proj/ --overwrite dataset/:my_format dataset2/:coco
-        """,
+        - Export project as a COCO-like dataset in other directory:|n
+        |s|s%(prog)s -f coco -o path/I/like/
+        """.format(
+            ", ".join(builtins)
+        ),
         formatter_class=MultilineFormatter,
     )
 
-    parser.add_argument("target", help="Target dataset revpath")
-    parser.add_argument("patch", help="Patch dataset revpath")
+    parser.add_argument(
+        "_positionals", nargs=argparse.REMAINDER, help=argparse.SUPPRESS
+    )  # workaround for -- eaten by positionals
+    parser.add_argument(
+        "target",
+        nargs="?",
+        default="project",
+        help="A project target to be exported (default: %(default)s)",
+    )
+    parser.add_argument("-e", "--filter", help="XML XPath filter expression for dataset items")
+    parser.add_argument(
+        "--filter-mode",
+        default=FilterModes.i.name,
+        type=FilterModes.parse,
+        help="Filter mode (options: %s; default: %s)"
+        % (", ".join(FilterModes.list_options()), "%(default)s"),
+    )
     parser.add_argument(
         "-o",
         "--output-dir",
         dest="dst_dir",
-        default=None,
-        help="Output directory (default: save in-place)",
+        help="Directory to save output (default: a subdir in the current one)",
     )
     parser.add_argument(
-        "--overwrite",
-        action="store_true",
-        help="Overwrite existing files in the save directory, " "if it is not empty",
+        "--overwrite", action="store_true", help="Overwrite existing files in the save directory"
     )
     parser.add_argument(
         "-p",
         "--project",
         dest="project_dir",
-        help="Directory of the 'current' project (default: current dir)",
+        help="Directory of the project to operate on (default: current dir)",
     )
+    parser.add_argument("-f", "--format", required=True, help="Output format")
     parser.add_argument(
         "extra_args",
         nargs=argparse.REMAINDER,
-        help="Additional arguments for exporting (pass '-- -h' for help). "
+        help="Additional arguments for exporter (pass '-- -h' for help). "
         "Must be specified after the main command arguments and after "
         "the '--' separator",
     )
-    parser.set_defaults(command=patch_command)
+    parser.set_defaults(command=export_command)
 
     return parser
 
 
 def get_sensitive_args():
     return {
-        patch_command: ["target", "patch", "dst_dir", "project_dir", "extra_args"],
+        export_command: ["dst_dir", "project_dir", "name", "extra_args", "target", "filter"],
     }
 
 
 @scoped
-def patch_command(args):
+def export_command(args):
+    has_sep = "--" in args._positionals
+    if has_sep:
+        pos = args._positionals.index("--")
+        if 1 < pos:
+            raise argparse.ArgumentError(None, message="Expected no more than 1 target argument")
+    else:
+        pos = 1
+    args.target = (args._positionals[:pos] or [ProjectBuildTargets.MAIN_TARGET])[0]
+    args.extra_args = args._positionals[pos + has_sep :]
+
+    show_plugin_help = "-h" in args.extra_args or "--help" in args.extra_args
+
     project = None
     try:
         project = scope_add(load_project(args.project_dir))
     except ProjectNotFoundError:
-        if args.project_dir:
+        if not show_plugin_help:
             raise
 
     if project is not None:
         env = project.env
     else:
         env = DEFAULT_ENVIRONMENT
 
-    target_dataset, _project = parse_full_revpath(args.target, project)
-    if _project is not None:
-        scope_add(_project)
-
     try:
-        exporter = env.exporters[target_dataset.format]
+        exporter = env.exporters[args.format]
     except KeyError:
         raise CliException("Exporter for format '%s' is not found" % args.format)
 
     extra_args = exporter.parse_cmdline(args.extra_args)
 
-    dst_dir = args.dst_dir or target_dataset.data_path
-    if not args.overwrite and osp.isdir(dst_dir) and os.listdir(dst_dir):
-        raise CliException(
-            "Directory '%s' already exists " "(pass --overwrite to overwrite)" % dst_dir
-        )
+    dst_dir = args.dst_dir
+    if dst_dir:
+        if not args.overwrite and osp.isdir(dst_dir) and os.listdir(dst_dir):
+            raise CliException(
+                "Directory '%s' already exists " "(pass --overwrite to overwrite)" % dst_dir
+            )
+    else:
+        dst_dir = generate_next_file_name("export-%s" % make_file_name(args.format))
     dst_dir = osp.abspath(dst_dir)
 
-    patch_dataset, _project = parse_full_revpath(args.patch, project)
-    if _project is not None:
-        scope_add(_project)
+    if args.filter:
+        filter_args = FilterModes.make_filter_args(args.filter_mode)
+        filter_expr = args.filter
+
+    log.info("Loading the project...")
+
+    dataset = project.working_tree.make_dataset(args.target)
+    if args.filter:
+        dataset.filter(filter_expr, **filter_args)
 
-    target_dataset.update(patch_dataset)
+    log.info("Exporting...")
 
-    target_dataset.save(save_dir=dst_dir, **extra_args)
+    dataset.export(save_dir=dst_dir, format=exporter, **extra_args)
 
-    log.info("Patched dataset has been saved to '%s'" % dst_dir)
+    log.info("Results have been saved to '%s'" % dst_dir)
 
     return 0
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/prune.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/prune.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/__init__.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/add.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/add.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/create.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/create.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/export.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/import_.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,138 +1,126 @@
-# Copyright (C) 2019-2021 Intel Corporation
+# Copyright (C) 2020-2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
 import os
-import os.path as osp
 
 from datumaro.components.environment import DEFAULT_ENVIRONMENT
 from datumaro.components.errors import ProjectNotFoundError
-from datumaro.components.project import ProjectBuildTargets
-from datumaro.util.os_util import make_file_name
-from datumaro.util.scope import scope_add, scoped
+from datumaro.util.scope import on_error_do, scope_add, scoped
 
-from ....util import MultilineFormatter
+from ....util import MultilineFormatter, join_cli_args, show_video_import_warning
 from ....util.errors import CliException
-from ....util.project import FilterModes, generate_next_file_name, load_project
+from ....util.project import generate_next_name, load_project
 
 __all__ = [
     "build_parser",
     "get_sensitive_args",
 ]
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
-    builtins = sorted(DEFAULT_ENVIRONMENT.exporters)
+    env = DEFAULT_ENVIRONMENT
+    builtins = sorted(set(env.extractors) | set(env.importers))
 
     parser = parser_ctor(
-        help="Export project",
+        help="Import dataset to project",
         description="""
-        Exports a project in some format.|n
+        Imports a data source to a project. A data source is a dataset
+        in a supported format (check 'formats' section below).|n
         |n
-        Each dataset format has its own export
-        options, which are passed after the '--' separator (see examples),
-        pass '-- -h' for more info. If not stated otherwise, by default
-        only annotations are exported, to include images pass
-        '--save-images' parameter.|n
-        |n
-        A filter can be passed, check the 'filter' command description for
-        more info.|n
+        Currently, only local paths to sources are supported.|n
+        During importing, a source is copied into the project.|n
         |n
         Formats:|n
         Datasets come in a wide variety of formats. Each dataset
         format defines its own data structure and rules on how to
         interpret the data. Check the user manual for the list of
         supported formats, examples and documentation.
         |n
         The list of supported formats can be extended by plugins.
         Check the "plugins" section of the developer guide for information
         about plugin implementation.|n
         |n
-        List of builtin dataset formats: {}|n
+        Each dataset format has its own import options, which are passed
+        after the '--' separator (see examples), pass '-- -h' for more info.|n
         |n
-        The command can only be applied to a project build target, a stage
-        or the combined 'project' target, in which case all the targets will
-        be affected.
+        Builtin formats: {}|n
         |n
         Examples:|n
-        - Export project as a VOC-like dataset, include images:|n
-        |s|s%(prog)s -f voc -- --save-images|n
+        - Add a local directory with a VOC-like dataset:|n
+        |s|s%(prog)s -f voc path/to/voc|n
+        |n
+        - Add a directory with a COCO dataset, use only a specific file:|n
+        |s|s%(prog)s -f coco_instances -r anns/train.json path/to/coco|n
         |n
-        - Export project as a COCO-like dataset in other directory:|n
-        |s|s%(prog)s -f coco -o path/I/like/
+        - Add a local file with CVAT annotations, call it 'mysource'|n
+        |s|s|s|sto the project in a specific place:|n
+        |s|s%(prog)s -f cvat -n mysource -p project/path/ path/to/cvat.xml
         """.format(
             ", ".join(builtins)
         ),
         formatter_class=MultilineFormatter,
     )
 
     parser.add_argument(
         "_positionals", nargs=argparse.REMAINDER, help=argparse.SUPPRESS
     )  # workaround for -- eaten by positionals
+    parser.add_argument("url", help="URL to the source dataset. A path to a file or directory")
     parser.add_argument(
-        "target",
-        nargs="?",
-        default="project",
-        help="A project target to be exported (default: %(default)s)",
+        "-n", "--name", help="Name of the new source (default: generate automatically)"
     )
-    parser.add_argument("-e", "--filter", help="XML XPath filter expression for dataset items")
+    parser.add_argument("-f", "--format", required=True, help="Source dataset format")
     parser.add_argument(
-        "--filter-mode",
-        default=FilterModes.i.name,
-        type=FilterModes.parse,
-        help="Filter mode (options: %s; default: %s)"
-        % (", ".join(FilterModes.list_options()), "%(default)s"),
+        "-r",
+        "--path",
+        dest="rpath",
+        help="A path relative to URL to the source data. Useful to specify "
+        "a path to subset, subtask, or a specific file in URL.",
     )
     parser.add_argument(
-        "-o",
-        "--output-dir",
-        dest="dst_dir",
-        help="Directory to save output (default: a subdir in the current one)",
-    )
-    parser.add_argument(
-        "--overwrite", action="store_true", help="Overwrite existing files in the save directory"
+        "--no-check", action="store_true", help="Don't try to read the source after importing"
     )
     parser.add_argument(
         "-p",
         "--project",
         dest="project_dir",
         help="Directory of the project to operate on (default: current dir)",
     )
-    parser.add_argument("-f", "--format", required=True, help="Output format")
     parser.add_argument(
         "extra_args",
         nargs=argparse.REMAINDER,
-        help="Additional arguments for exporter (pass '-- -h' for help). "
+        help="Additional arguments for extractor (pass '-- -h' for help). "
         "Must be specified after the main command arguments and after "
         "the '--' separator",
     )
-    parser.set_defaults(command=export_command)
+    parser.set_defaults(command=import_command)
 
     return parser
 
 
 def get_sensitive_args():
     return {
-        export_command: ["dst_dir", "project_dir", "name", "extra_args", "target", "filter"],
+        import_command: ["url", "project_dir", "rpath", "name", "extra_args"],
     }
 
 
 @scoped
-def export_command(args):
+def import_command(args):
+    # Workaround. Required positionals consume positionals from the end
+    args._positionals += join_cli_args(args, "url", "extra_args")
+
     has_sep = "--" in args._positionals
     if has_sep:
         pos = args._positionals.index("--")
-        if 1 < pos:
-            raise argparse.ArgumentError(None, message="Expected no more than 1 target argument")
     else:
         pos = 1
-    args.target = (args._positionals[:pos] or [ProjectBuildTargets.MAIN_TARGET])[0]
+    args.url = (args._positionals[:pos] or [""])[0]
     args.extra_args = args._positionals[pos + has_sep :]
 
     show_plugin_help = "-h" in args.extra_args or "--help" in args.extra_args
 
     project = None
     try:
         project = scope_add(load_project(args.project_dir))
@@ -141,41 +129,54 @@
             raise
 
     if project is not None:
         env = project.env
     else:
         env = DEFAULT_ENVIRONMENT
 
-    try:
-        exporter = env.exporters[args.format]
-    except KeyError:
-        raise CliException("Exporter for format '%s' is not found" % args.format)
-
-    extra_args = exporter.parse_cmdline(args.extra_args)
-
-    dst_dir = args.dst_dir
-    if dst_dir:
-        if not args.overwrite and osp.isdir(dst_dir) and os.listdir(dst_dir):
-            raise CliException(
-                "Directory '%s' already exists " "(pass --overwrite to overwrite)" % dst_dir
-            )
+    fmt = args.format
+    if fmt in env.importers:
+        arg_parser = env.importers[fmt]
+    elif fmt in env.extractors:
+        arg_parser = env.extractors[fmt]
     else:
-        dst_dir = generate_next_file_name("export-%s" % make_file_name(args.format))
-    dst_dir = osp.abspath(dst_dir)
-
-    if args.filter:
-        filter_args = FilterModes.make_filter_args(args.filter_mode)
-        filter_expr = args.filter
+        raise CliException(
+            "Unknown format '%s'. A format can be added"
+            " by providing an Extractor and Importer plugins" % fmt
+        )
+
+    extra_args = arg_parser.parse_cmdline(args.extra_args)
+
+    name = args.name
+    if name:
+        if name in project.working_tree.sources:
+            raise CliException("Source '%s' already exists" % name)
+    else:
+        name = generate_next_name(
+            list(project.working_tree.sources) + os.listdir(), "source", sep="-", default="1"
+        )
 
-    log.info("Loading the project...")
+    if fmt == "video_frames":
+        show_video_import_warning()
 
-    dataset = project.working_tree.make_dataset(args.target)
-    if args.filter:
-        dataset.filter(filter_expr, **filter_args)
+    project.import_source(
+        name,
+        url=args.url,
+        format=args.format,
+        options=extra_args,
+        no_cache=True,
+        no_hash=True,
+        rpath=args.rpath,
+    )
+    on_error_do(
+        project.remove_source, name, ignore_errors=True, kwargs={"force": True, "keep_data": False}
+    )
 
-    log.info("Exporting...")
+    if not args.no_check:
+        log.info("Checking the source...")
+        project.working_tree.make_dataset(name)
 
-    dataset.export(save_dir=dst_dir, format=exporter, **extra_args)
+    project.working_tree.save()
 
-    log.info("Results have been saved to '%s'" % dst_dir)
+    log.info("Source '%s' with format '%s' has been added to the project", name, args.format)
 
     return 0
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/import_.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/validate.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,182 +1,150 @@
 # Copyright (C) 2020-2021 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import argparse
 import logging as log
-import os
 
 from datumaro.components.environment import DEFAULT_ENVIRONMENT
 from datumaro.components.errors import ProjectNotFoundError
-from datumaro.util.scope import on_error_do, scope_add, scoped
-
-from ....util import MultilineFormatter, join_cli_args, show_video_import_warning
-from ....util.errors import CliException
-from ....util.project import generate_next_name, load_project
-
-__all__ = [
-    "build_parser",
-    "get_sensitive_args",
-]
+from datumaro.components.validator import TaskType
+from datumaro.util import dump_json_file
+from datumaro.util.scope import scope_add, scoped
+
+from ..util import MultilineFormatter
+from ..util.errors import CliException
+from ..util.project import generate_next_file_name, load_project, parse_full_revpath
 
 
 def build_parser(parser_ctor=argparse.ArgumentParser):
-    env = DEFAULT_ENVIRONMENT
-    builtins = sorted(set(env.extractors) | set(env.importers))
-
     parser = parser_ctor(
-        help="Import dataset to project",
+        help="Validate project",
         description="""
-        Imports a data source to a project. A data source is a dataset
-        in a supported format (check 'formats' section below).|n
-        |n
-        Currently, only local paths to sources are supported.|n
-        During importing, a source is copied into the project.|n
-        |n
-        Formats:|n
-        Datasets come in a wide variety of formats. Each dataset
-        format defines its own data structure and rules on how to
-        interpret the data. Check the user manual for the list of
-        supported formats, examples and documentation.
-        |n
-        The list of supported formats can be extended by plugins.
-        Check the "plugins" section of the developer guide for information
-        about plugin implementation.|n
-        |n
-        Each dataset format has its own import options, which are passed
-        after the '--' separator (see examples), pass '-- -h' for more info.|n
-        |n
-        Builtin formats: {}|n
+        Validates a dataset according to the task type and
+        reports summary in a JSON file.|n
+        Target dataset is specified by a revpath. The full syntax is:|n
+        - Dataset paths:|n
+        |s|s- <dataset path>[ :<format> ]|n
+        - Revision paths:|n
+        |s|s- <project path> [ @<rev> ] [ :<target> ]|n
+        |s|s- <rev> [ :<target> ]|n
+        |s|s- <target>|n
+        |n
+        Both forms use the -p/--project as a context for plugins. It can be
+        useful for dataset paths in targets. When not specified, the current
+        project's working tree is used.|n
         |n
         Examples:|n
-        - Add a local directory with a VOC-like dataset:|n
-        |s|s%(prog)s -f voc path/to/voc|n
-        |n
-        - Add a directory with a COCO dataset, use only a specific file:|n
-        |s|s%(prog)s -f coco_instances -r anns/train.json path/to/coco|n
-        |n
-        - Add a local file with CVAT annotations, call it 'mysource'|n
-        |s|s|s|sto the project in a specific place:|n
-        |s|s%(prog)s -f cvat -n mysource -p project/path/ path/to/cvat.xml
-        """.format(
-            ", ".join(builtins)
-        ),
+        - Validate a project's subset as a classification dataset:|n |n
+        |s|s%(prog)s -t classification -s train
+        """,
         formatter_class=MultilineFormatter,
     )
 
+    task_types = ", ".join(t.name for t in TaskType)
+
+    def _parse_task_type(s):
+        try:
+            return TaskType[s.lower()].name
+        except Exception:
+            raise argparse.ArgumentTypeError(
+                "Unknown task type %s. Expected " "one of: %s" % (s, task_types)
+            )
+
     parser.add_argument(
         "_positionals", nargs=argparse.REMAINDER, help=argparse.SUPPRESS
     )  # workaround for -- eaten by positionals
-    parser.add_argument("url", help="URL to the source dataset. A path to a file or directory")
     parser.add_argument(
-        "-n", "--name", help="Name of the new source (default: generate automatically)"
+        "target", default="project", nargs="?", help="Target dataset revpath (default: project)"
     )
-    parser.add_argument("-f", "--format", required=True, help="Source dataset format")
     parser.add_argument(
-        "-r",
-        "--path",
-        dest="rpath",
-        help="A path relative to URL to the source data. Useful to specify "
-        "a path to subset, subtask, or a specific file in URL.",
+        "-t",
+        "--task",
+        type=_parse_task_type,
+        required=True,
+        help="Task type for validation, one of %s" % task_types,
     )
     parser.add_argument(
-        "--no-check", action="store_true", help="Don't try to read the source after importing"
+        "-s", "--subset", dest="subset_name", help="Subset to validate (default: whole dataset)"
     )
     parser.add_argument(
         "-p",
         "--project",
         dest="project_dir",
-        help="Directory of the project to operate on (default: current dir)",
+        help="Directory of the project to validate (default: current dir)",
     )
     parser.add_argument(
         "extra_args",
         nargs=argparse.REMAINDER,
-        help="Additional arguments for extractor (pass '-- -h' for help). "
-        "Must be specified after the main command arguments and after "
-        "the '--' separator",
+        help="Optional arguments for validator (pass '-- -h' for help)",
     )
-    parser.set_defaults(command=import_command)
+    parser.set_defaults(command=validate_command)
 
     return parser
 
 
 def get_sensitive_args():
     return {
-        import_command: ["url", "project_dir", "rpath", "name", "extra_args"],
+        validate_command: ["target", "project_dir", "subset_name", "extra_args"],
     }
 
 
 @scoped
-def import_command(args):
-    # Workaround. Required positionals consume positionals from the end
-    args._positionals += join_cli_args(args, "url", "extra_args")
-
+def validate_command(args):
     has_sep = "--" in args._positionals
     if has_sep:
         pos = args._positionals.index("--")
+        if 1 < pos:
+            raise argparse.ArgumentError(None, message="Expected no more than 1 target argument")
     else:
         pos = 1
-    args.url = (args._positionals[:pos] or [""])[0]
+    args.target = (args._positionals[:pos] or ["project"])[0]
     args.extra_args = args._positionals[pos + has_sep :]
 
     show_plugin_help = "-h" in args.extra_args or "--help" in args.extra_args
 
     project = None
     try:
         project = scope_add(load_project(args.project_dir))
     except ProjectNotFoundError:
-        if not show_plugin_help:
+        if not show_plugin_help and args.project_dir:
             raise
 
     if project is not None:
         env = project.env
     else:
         env = DEFAULT_ENVIRONMENT
 
-    fmt = args.format
-    if fmt in env.importers:
-        arg_parser = env.importers[fmt]
-    elif fmt in env.extractors:
-        arg_parser = env.extractors[fmt]
-    else:
-        raise CliException(
-            "Unknown format '%s'. A format can be added"
-            " by providing an Extractor and Importer plugins" % fmt
-        )
-
-    extra_args = arg_parser.parse_cmdline(args.extra_args)
-
-    name = args.name
-    if name:
-        if name in project.working_tree.sources:
-            raise CliException("Source '%s' already exists" % name)
-    else:
-        name = generate_next_name(
-            list(project.working_tree.sources) + os.listdir(), "source", sep="-", default="1"
-        )
-
-    if fmt == "video_frames":
-        show_video_import_warning()
-
-    project.import_source(
-        name,
-        url=args.url,
-        format=args.format,
-        options=extra_args,
-        no_cache=True,
-        no_hash=True,
-        rpath=args.rpath,
-    )
-    on_error_do(
-        project.remove_source, name, ignore_errors=True, kwargs={"force": True, "keep_data": False}
-    )
-
-    if not args.no_check:
-        log.info("Checking the source...")
-        project.working_tree.make_dataset(name)
-
-    project.working_tree.save()
-
-    log.info("Source '%s' with format '%s' has been added to the project", name, args.format)
-
-    return 0
+    try:
+        validator_type = env.validators[args.task]
+    except KeyError:
+        raise CliException("Validator type '%s' is not found" % args.task)
+
+    extra_args = validator_type.parse_cmdline(args.extra_args)
+
+    dataset, target_project = parse_full_revpath(args.target, project)
+    if target_project:
+        scope_add(target_project)
+
+    dst_file_name = "validation-report"
+    if args.subset_name is not None:
+        dataset = dataset.get_subset(args.subset_name)
+        dst_file_name += f"-{args.subset_name}"
+
+    validator = validator_type(**extra_args)
+    report = validator.validate(dataset)
+
+    def _make_serializable(d):
+        for key, val in list(d.items()):
+            # tuple key to str
+            if isinstance(key, tuple) or isinstance(key, int):
+                d[str(key)] = val
+                d.pop(key)
+            if isinstance(val, dict):
+                _make_serializable(val)
+
+    _make_serializable(report)
+
+    dst_file = generate_next_file_name(dst_file_name, ext=".json")
+    log.info("Writing project validation results to '%s'" % dst_file)
+    dump_json_file(dst_file, report, indent=True, allow_numpy=True)
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/modification/remove.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/modification/remove.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/checkout.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/checkout.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/commit.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/commit.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/info.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/info.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/log.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/log.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/require_project/versioning/status.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/require_project/versioning/status.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/stats.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/stats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/commands/transform.py` & `datumaro-1.4.0rc3/src/datumaro/cli/commands/transform.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/contexts/model.py` & `datumaro-1.4.0rc3/src/datumaro/cli/contexts/model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/contexts/project/__init__.py` & `datumaro-1.4.0rc3/src/datumaro/cli/contexts/project/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/contexts/source.py` & `datumaro-1.4.0rc3/src/datumaro/cli/contexts/source.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/contexts/util.py` & `datumaro-1.4.0rc3/src/datumaro/cli/contexts/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/util/__init__.py` & `datumaro-1.4.0rc3/src/datumaro/cli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/util/compare.py` & `datumaro-1.4.0rc3/src/datumaro/cli/util/compare.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/cli/util/project.py` & `datumaro-1.4.0rc3/src/datumaro/cli/util/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/abstracts/merger.py` & `datumaro-1.4.0rc3/src/datumaro/components/abstracts/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/abstracts/model_interpreter.py` & `datumaro-1.4.0rc3/src/datumaro/components/abstracts/model_interpreter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/base.py` & `datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/explorer.py` & `datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/explorer.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-from typing import Optional, Sequence, Union
+from typing import List, Optional, Sequence, Union
 
 import numpy as np
 
 from datumaro.components.algorithms.hash_key_inference.base import HashInference
 from datumaro.components.algorithms.hash_key_inference.hashkey_util import (
     calculate_hamming,
     select_uninferenced_dataset,
@@ -59,25 +59,60 @@
             raise ValueError("Database should have hash_key")
 
         self._database_keys = np.stack(database_keys, axis=0)
         self._item_list = item_list
 
     def explore_topk(
         self,
-        query: Union[DatasetItem, str],
+        query: Union[DatasetItem, str, List[Union[DatasetItem, str]]],
         topk: Optional[int] = None,
     ):
         """
         Explore topk similar results based on hamming distance for query DatasetItem
         """
         if not topk:
             topk = self._topk
 
         database_keys = self._database_keys
 
+        if isinstance(query, list):
+            topk_for_query = int(topk // len(query)) * 2 if not len(query) == 1 else topk
+            query_hash_key_list = []
+            result_list = []
+            logits_list = []
+            for query_ in query:
+                if isinstance(query_, DatasetItem):
+                    query_key = self._get_hash_key_from_item_query(query_)
+                    query_hash_key_list.append(query_key)
+                elif isinstance(query_, str):
+                    query_key = self._get_hash_key_from_text_query(query_)
+                    query_hash_key_list.append(query_key)
+                else:
+                    raise MediaTypeError(
+                        "Unexpected media type of query '%s'. "
+                        "Expected 'DatasetItem' or 'string', actual'%s'" % (query_, type(query_))
+                    )
+
+            for query_key in query_hash_key_list:
+                unpacked_key = np.unpackbits(query_key.hash_key, axis=-1)
+                logits = calculate_hamming(unpacked_key, database_keys)
+                ind = np.argsort(logits)
+
+                item_list = np.array(self._item_list)[ind]
+                result_list.append(item_list[:topk_for_query].tolist())
+                logits_list.append(logits[ind][:topk_for_query].tolist())
+
+            result_list = np.stack(result_list, axis=0)
+            logits_list = np.stack(logits_list, axis=0)
+
+            flattened_indices = np.argsort(logits_list.ravel())
+            sorted_list = result_list.ravel()[flattened_indices]
+
+            return sorted_list[:topk]
+
         if isinstance(query, DatasetItem):
             query_key = self._get_hash_key_from_item_query(query)
         elif isinstance(query, str):
             query_key = self._get_hash_key_from_text_query(query)
         else:
             raise MediaTypeError(
                 "Unexpected media type of query '%s'. "
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py` & `datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import os
+
 import numpy as np
 
 from datumaro.components.annotation import HashKey
 from datumaro.components.dataset import Dataset
 from datumaro.components.media import MediaElement
 
 templates = [
@@ -168,7 +170,39 @@
 def calculate_hamming(B1, B2):
     """
     :param B1:  vector [n]
     :param B2:  vector [r*n]
     :return: hamming distance [r]
     """
     return np.count_nonzero(B1 != B2, axis=1)
+
+
+def match_query_subset(query_id, dataset, subset=None):
+    if subset:
+        return dataset.get(query_id, subset)
+
+    subset_names = dataset.subsets().keys()
+    for subset_name in subset_names:
+        try:
+            query_datasetitem = dataset.get(query_id, subset_name)
+            if query_datasetitem:
+                return query_datasetitem
+        except Exception:
+            pass
+
+    return None
+
+
+def check_and_convert_to_list(paths):
+    if isinstance(paths, str):
+        paths = [paths]
+    elif not isinstance(paths, list):
+        raise ValueError("Invalid value type. Expected str or list.")
+
+    valid_paths = []
+    for path in paths:
+        if os.path.exists(path):
+            valid_paths.append(path)
+        else:
+            raise ValueError(f"Invalid path: {path}")
+
+    return valid_paths
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/algorithms/hash_key_inference/prune.py` & `datumaro-1.4.0rc3/src/datumaro/components/algorithms/hash_key_inference/prune.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py` & `datumaro-1.4.0rc3/src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/algorithms/rise.py` & `datumaro-1.4.0rc3/src/datumaro/components/algorithms/rise.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/annotation.py` & `datumaro-1.4.0rc3/src/datumaro/components/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/annotations/matcher.py` & `datumaro-1.4.0rc3/src/datumaro/components/annotations/matcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/annotations/merger.py` & `datumaro-1.4.0rc3/src/datumaro/components/annotations/merger.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/cli_plugin.py` & `datumaro-1.4.0rc3/src/datumaro/components/cli_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/comparator.py` & `datumaro-1.4.0rc3/src/datumaro/components/comparator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/config.py` & `datumaro-1.4.0rc3/src/datumaro/components/config.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/config_model.py` & `datumaro-1.4.0rc3/src/datumaro/components/config_model.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/crypter.py` & `datumaro-1.4.0rc3/src/datumaro/components/crypter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/dataset.py` & `datumaro-1.4.0rc3/src/datumaro/components/dataset.py`

 * *Files 1% similar despite different names*

```diff
@@ -740,15 +740,15 @@
                     extractor_kwargs.pop("ctx")
 
                     extractors.append(
                         env.make_extractor(src_conf.format, src_conf.url, **extractor_kwargs)
                     )
 
             dataset = (
-                cls(source=extractor_merger(*extractors), env=env)
+                cls(source=extractor_merger(extractors), env=env)
                 if extractor_merger is not None
                 else cls.from_extractors(*extractors, env=env, merge_policy=merge_policy)
             )
             if eager:
                 dataset.init_cache()
         except _ImportFail as e:
             cause = e.__cause__ if getattr(e, "__cause__", None) is not None else e
@@ -794,14 +794,16 @@
 
     @property
     def is_stream(self) -> bool:
         return self._data.is_stream
 
 
 class StreamDataset(Dataset):
+    _stream = True
+
     def __init__(
         self,
         source: Optional[IDataset] = None,
         *,
         infos: Optional[DatasetInfo] = None,
         categories: Optional[CategoriesInfo] = None,
         media_type: Optional[Type[MediaElement]] = None,
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/dataset_base.py` & `datumaro-1.4.0rc3/src/datumaro/components/dataset_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-# Copyright (C) 2019-2022 Intel Corporation
+# Copyright (C) 2019-2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from __future__ import annotations
 
 import warnings
 from typing import Any, Dict, Iterator, List, Optional, Sequence, Type, TypeVar, Union, cast
 
 import attr
 import numpy as np
 from attr import attrs, field
 
 from datumaro.components.annotation import Annotation, AnnotationType, Categories
 from datumaro.components.cli_plugin import CliPlugin
-from datumaro.components.importer import ImportContext, NullImportContext, _ImportFail
+from datumaro.components.contexts.importer import ImportContext, NullImportContext
 from datumaro.components.media import Image, MediaElement, PointCloud
 from datumaro.util.attrs_util import default_if_none, not_empty
 from datumaro.util.definitions import DEFAULT_SUBSET_NAME
 
 T = TypeVar("T", bound=MediaElement)
 
 
@@ -362,60 +362,7 @@
         assert subset == self._subset, "%s != %s" % (subset, self._subset)
         return super().get(id, subset or self._subset)
 
     @property
     def subset(self) -> str:
         """Subset name of this instance."""
         return self._subset
-
-
-class ExtractorMerger(DatasetBase):
-    """A simple class to merge single-subset extractors."""
-
-    def __init__(
-        self,
-        *sources: Sequence[SubsetBase],
-    ):
-        if len(sources) == 0:
-            raise _ImportFail("It should not be empty.")
-
-        self._infos = self._check_identicalness(*[s.infos() for s in sources])
-        self._categories = self._check_identicalness(*[s.categories() for s in sources])
-        self._media_type = self._check_identicalness(*[s.media_type() for s in sources])
-        self._is_stream = self._check_identicalness(*[s.is_stream for s in sources])
-        self._subsets = {s.subset: s for s in sources}
-
-    def _check_identicalness(self, *seq: Sequence[T]) -> T:
-        if len(seq) == 0:
-            raise _ImportFail("It should not be empty.")
-
-        if seq.count(seq[0]) != len(seq):
-            raise _ImportFail("All items in the sequence should be identical.")
-
-        return seq[0]
-
-    def infos(self):
-        return self._infos
-
-    def categories(self):
-        return self._categories
-
-    def __iter__(self):
-        for subset in self._subsets.values():
-            yield from subset
-
-    def __len__(self):
-        return sum(len(subset) for subset in self._subsets.values())
-
-    def get(self, id: str, subset: Optional[str] = None):
-        if subset is None:
-            for s in self._subsets.values():
-                item = s.get(id)
-                if item is not None:
-                    return item
-
-        s = self._subset[subset]
-        return s.get(id)
-
-    @property
-    def is_stream(self) -> bool:
-        return self._is_stream
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/dataset_item_storage.py` & `datumaro-1.4.0rc3/src/datumaro/components/dataset_item_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/dataset_storage.py` & `datumaro-1.4.0rc3/src/datumaro/components/dataset_storage.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/environment.py` & `datumaro-1.4.0rc3/src/datumaro/components/environment.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,16 @@
         skip = tuple(skip | set(accept))
         return partial(cls._check_type, accept=accept, decline=decline, skip=skip)
 
     @staticmethod
     def _check_type(t, *, accept, decline, skip):
         if not issubclass(t, accept) or t in skip or (decline and issubclass(t, decline)):
             return False
-
+        if getattr(t, "__not_plugin__", None):
+            return False
         return True
 
     def __init__(self, use_lazy_import: bool = True):
         from datumaro.components.dataset_base import DatasetBase, SubsetBase
         from datumaro.components.exporter import Exporter
         from datumaro.components.generator import DatasetGenerator
         from datumaro.components.importer import Importer
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/errors.py` & `datumaro-1.4.0rc3/src/datumaro/components/errors.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/exporter.py` & `datumaro-1.4.0rc3/src/datumaro/components/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/extractor_tfds.py` & `datumaro-1.4.0rc3/src/datumaro/components/extractor_tfds.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/filter.py` & `datumaro-1.4.0rc3/src/datumaro/components/filter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/format_detection.py` & `datumaro-1.4.0rc3/src/datumaro/components/format_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/generator.py` & `datumaro-1.4.0rc3/src/datumaro/components/generator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/hl_ops/__init__.py` & `datumaro-1.4.0rc3/src/datumaro/components/hl_ops/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/importer.py` & `datumaro-1.4.0rc3/src/datumaro/components/importer.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,96 +5,40 @@
 from __future__ import annotations
 
 import os
 import os.path as osp
 from contextlib import contextmanager
 from functools import wraps
 from glob import iglob
-from typing import Callable, Dict, List, NoReturn, Optional, Tuple, Type, TypeVar
-
-import attr
-from attr import define, field
+from typing import Callable, Dict, List, Optional, Type, TypeVar
 
 from datumaro.components.cli_plugin import CliPlugin
-from datumaro.components.errors import (
-    AnnotationImportError,
-    DatasetImportError,
-    DatasetNotFoundError,
-    DatumaroError,
-    ItemImportError,
+from datumaro.components.contexts.importer import (
+    FailingImportErrorPolicy,
+    ImportContext,
+    ImportErrorPolicy,
+    NullImportContext,
+    _ImportFail,
 )
+from datumaro.components.errors import DatasetImportError, DatasetNotFoundError
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
-from datumaro.components.progress_reporting import NullProgressReporter, ProgressReporter
+from datumaro.components.merge.extractor_merger import ExtractorMerger
 from datumaro.util.definitions import SUBSET_NAME_BLACKLIST
 
 T = TypeVar("T")
-# TODO: we should refactor code to import `ExtractorMerger` from datumaro.component.dataset_base
-# Currently, it is impossible due to a circular import.
-ExtractorMerger = TypeVar("ExtractorMerger")
-
-
-class _ImportFail(DatumaroError):
-    pass
-
-
-class ImportErrorPolicy:
-    def report_item_error(self, error: Exception, *, item_id: Tuple[str, str]) -> None:
-        """
-        Allows to report a problem with a dataset item.
-        If this function returns, the extractor must skip the item.
-        """
-
-        if not isinstance(error, _ImportFail):
-            ie = ItemImportError(item_id)
-            ie.__cause__ = error
-            return self._handle_item_error(ie)
-        else:
-            raise error
-
-    def report_annotation_error(self, error: Exception, *, item_id: Tuple[str, str]) -> None:
-        """
-        Allows to report a problem with a dataset item annotation.
-        If this function returns, the extractor must skip the annotation.
-        """
 
-        if not isinstance(error, _ImportFail):
-            ie = AnnotationImportError(item_id)
-            ie.__cause__ = error
-            return self._handle_annotation_error(ie)
-        else:
-            raise error
-
-    def _handle_item_error(self, error: ItemImportError) -> None:
-        """This function must either call fail() or return."""
-        self.fail(error)
-
-    def _handle_annotation_error(self, error: AnnotationImportError) -> None:
-        """This function must either call fail() or return."""
-        self.fail(error)
-
-    def fail(self, error: Exception) -> NoReturn:
-        raise _ImportFail from error
-
-
-class FailingImportErrorPolicy(ImportErrorPolicy):
-    pass
-
-
-@define(eq=False)
-class ImportContext:
-    progress_reporter: ProgressReporter = field(
-        default=None, converter=attr.converters.default_if_none(factory=NullProgressReporter)
-    )
-    error_policy: ImportErrorPolicy = field(
-        default=None, converter=attr.converters.default_if_none(factory=FailingImportErrorPolicy)
-    )
-
-
-class NullImportContext(ImportContext):
-    pass
+__all__ = [
+    "ImportContext",
+    "NullImportContext",
+    "_ImportFail",
+    "Importer",
+    "with_subset_dirs",
+    "ImportErrorPolicy",
+    "FailingImportErrorPolicy",
+]
 
 
 class Importer(CliPlugin):
     DETECT_CONFIDENCE = FormatDetectionConfidence.LOW
 
     @classmethod
     def detect(
@@ -208,14 +152,17 @@
     def get_extractor_merger(self) -> Optional[Type[ExtractorMerger]]:
         """Extractor merger dedicated for the data format
 
         Datumaro import process spawns multiple `DatasetBase` for the detected sources.
         We can find a bunch of the detected sources from the given directory path.
         It is usually each detected source is corresponded to the subset of dataset in many data formats.
 
+        Parameters:
+            stream: There can exist a branch according to `stream` flag
+
         Returns:
             If None, use `Dataset.from_extractors()` to merge the extractors,
             Otherwise, use the return type to merge the extractors.
         """
         return None
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/launcher.py` & `datumaro-1.4.0rc3/src/datumaro/components/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/lazy_plugin.py` & `datumaro-1.4.0rc3/src/datumaro/components/lazy_plugin.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/media.py` & `datumaro-1.4.0rc3/src/datumaro/components/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/media_manager.py` & `datumaro-1.4.0rc3/src/datumaro/components/media_manager.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/merge/__init__.py` & `datumaro-1.4.0rc3/src/datumaro/components/merge/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/merge/base.py` & `datumaro-1.4.0rc3/src/datumaro/components/merge/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import logging as log
 import os
 from collections import OrderedDict
 from typing import Dict, Optional, Sequence, Type
 
 from datumaro.components.abstracts.merger import IMergerContext
 from datumaro.components.cli_plugin import CliPlugin
-from datumaro.components.dataset_base import IDataset
+from datumaro.components.dataset_base import CategoriesInfo, DatasetInfo, IDataset
 from datumaro.components.dataset_item_storage import DatasetItemStorageDatasetView
 from datumaro.components.errors import (
     ConflictingCategoriesError,
     DatasetMergeError,
     DatasetQualityError,
     MediaTypeError,
 )
@@ -24,27 +24,29 @@
     """Merge multiple datasets into one dataset"""
 
     def __init__(self, **options):
         super().__init__(**options)
         self.__dict__["_sources"] = None
         self.errors = []
 
-    def merge_infos(self, sources: Sequence[IDataset]) -> Dict:
+    @staticmethod
+    def merge_infos(sources: Sequence[DatasetInfo]) -> Dict:
         """Merge several :class:`IDataset` into one :class:`IDataset`"""
         infos = {}
         for source in sources:
             for k, v in source.items():
                 if k in infos:
                     log.warning(
                         "Duplicated infos field %s: overwrite from %s to %s", k, infos[k], v
                     )
                 infos[k] = v
         return infos
 
-    def merge_categories(self, sources: Sequence[IDataset]) -> Dict:
+    @staticmethod
+    def merge_categories(sources: Sequence[CategoriesInfo]) -> Dict:
         categories = {}
         for source_idx, source in enumerate(sources):
             for cat_type, source_cat in source.items():
                 existing_cat = categories.setdefault(cat_type, source_cat)
                 if existing_cat != source_cat and len(source_cat) != 0:
                     if len(existing_cat) == 0:
                         categories[cat_type] = source_cat
@@ -52,15 +54,16 @@
                         raise ConflictingCategoriesError(
                             "Merging of datasets with different categories is "
                             "only allowed in 'merge' command.",
                             sources=list(range(source_idx)),
                         )
         return categories
 
-    def merge_media_types(self, sources: Sequence[IDataset]) -> Optional[Type[MediaElement]]:
+    @staticmethod
+    def merge_media_types(sources: Sequence[IDataset]) -> Optional[Type[MediaElement]]:
         if sources:
             media_type = sources[0].media_type()
             for s in sources:
                 if not issubclass(s.media_type(), media_type) or not issubclass(
                     media_type, s.media_type()
                 ):
                     # Symmetric comparision is needed in the case of subclasses:
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/merge/exact_merge.py` & `datumaro-1.4.0rc3/src/datumaro/components/merge/exact_merge.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,30 +33,32 @@
         - annotations are matched by value and shared
         - in case of conflicts, throws an error
     """
 
     def __init__(self, **options):
         super().__init__(**options)
 
-    def merge(self, sources: Sequence[IDataset]) -> DatasetItemStorage:
+    @classmethod
+    def merge(cls, sources: Sequence[IDataset]) -> DatasetItemStorage:
         items = DatasetItemStorage()
         for source_idx, source in enumerate(sources):
             for item in source:
                 existing_item = items.get(item.id, item.subset)
                 if existing_item is not None:
                     try:
-                        item = self._merge_items(existing_item, item)
+                        item = cls.merge_items(existing_item, item)
                     except DatasetMergeError as e:
                         e.sources = set(range(source_idx))
                         raise e
 
                 items.put(item)
         return items
 
-    def _match_annotations_equal(self, a, b):
+    @classmethod
+    def _match_annotations_equal(cls, a, b):
         matches = []
         a_unmatched = a[:]
         b_unmatched = b[:]
         for a_ann in a:
             for b_ann in b_unmatched:
                 if a_ann != b_ann:
                     continue
@@ -64,30 +66,33 @@
                 matches.append((a_ann, b_ann))
                 a_unmatched.remove(a_ann)
                 b_unmatched.remove(b_ann)
                 break
 
         return matches, a_unmatched, b_unmatched
 
-    def _merge_annotations_equal(self, a, b):
-        matches, a_unmatched, b_unmatched = self._match_annotations_equal(a, b)
+    @classmethod
+    def _merge_annotations_equal(cls, a, b):
+        matches, a_unmatched, b_unmatched = cls._match_annotations_equal(a, b)
         return [ann_a for (ann_a, _) in matches] + a_unmatched + b_unmatched
 
-    def _merge_items(self, existing_item: DatasetItem, current_item: DatasetItem) -> DatasetItem:
+    @classmethod
+    def merge_items(cls, existing_item: DatasetItem, current_item: DatasetItem) -> DatasetItem:
         return existing_item.wrap(
-            media=self._merge_media(existing_item, current_item),
-            attributes=self._merge_attrs(
+            media=cls._merge_media(existing_item, current_item),
+            attributes=cls._merge_attrs(
                 existing_item.attributes,
                 current_item.attributes,
                 item_id=(existing_item.id, existing_item.subset),
             ),
-            annotations=self._merge_anno(existing_item.annotations, current_item.annotations),
+            annotations=cls._merge_anno(existing_item.annotations, current_item.annotations),
         )
 
-    def _merge_attrs(self, a: Dict[str, Any], b: Dict[str, Any], item_id: Tuple[str, str]) -> Dict:
+    @classmethod
+    def _merge_attrs(cls, a: Dict[str, Any], b: Dict[str, Any], item_id: Tuple[str, str]) -> Dict:
         merged = {}
 
         for name in a.keys() | b.keys():
             a_val = a.get(name, None)
             b_val = b.get(name, None)
 
             if name not in a:
@@ -99,33 +104,34 @@
             else:
                 m_val = a_val
 
             merged[name] = m_val
 
         return merged
 
+    @classmethod
     def _merge_media(
-        self, item_a: DatasetItem, item_b: DatasetItem
+        cls, item_a: DatasetItem, item_b: DatasetItem
     ) -> Union[Image, PointCloud, Video]:
         if (not item_a.media or isinstance(item_a.media, Image)) and (
             not item_b.media or isinstance(item_b.media, Image)
         ):
-            media = self._merge_images(item_a, item_b)
+            media = cls._merge_images(item_a, item_b)
         elif (not item_a.media or isinstance(item_a.media, PointCloud)) and (
             not item_b.media or isinstance(item_b.media, PointCloud)
         ):
-            media = self._merge_point_clouds(item_a, item_b)
+            media = cls._merge_point_clouds(item_a, item_b)
         elif (not item_a.media or isinstance(item_a.media, Video)) and (
             not item_b.media or isinstance(item_b.media, Video)
         ):
-            media = self._merge_videos(item_a, item_b)
+            media = cls._merge_videos(item_a, item_b)
         elif (not item_a.media or isinstance(item_a.media, MultiframeImage)) and (
             not item_b.media or isinstance(item_b.media, MultiframeImage)
         ):
-            media = self._merge_multiframe_images(item_a, item_b)
+            media = cls._merge_multiframe_images(item_a, item_b)
         elif (not item_a.media or isinstance(item_a.media, MediaElement)) and (
             not item_b.media or isinstance(item_b.media, MediaElement)
         ):
             if isinstance(item_a.media, MediaElement) and isinstance(item_b.media, MediaElement):
                 item_a_path = getattr(item_a.media, "path", None)
                 item_b_path = getattr(item_b.media, "path", None)
 
@@ -144,15 +150,16 @@
                 media = item_a.media
             else:
                 media = item_b.media
         else:
             raise MismatchingMediaError((item_a.id, item_a.subset), item_a.media, item_b.media)
         return media
 
-    def _merge_images(self, item_a: DatasetItem, item_b: DatasetItem) -> Image:
+    @classmethod
+    def _merge_images(cls, item_a: DatasetItem, item_b: DatasetItem) -> Image:
         media = None
 
         if isinstance(item_a.media, Image) and isinstance(item_b.media, Image):
             item_a_path = getattr(item_a.media, "path", None)
             item_b_path = getattr(item_b.media, "path", None)
 
             if (
@@ -210,15 +217,16 @@
         elif isinstance(item_a.media, Image):
             media = item_a.media
         else:
             media = item_b.media
 
         return media
 
-    def _merge_point_clouds(self, item_a: DatasetItem, item_b: DatasetItem) -> PointCloud:
+    @classmethod
+    def _merge_point_clouds(cls, item_a: DatasetItem, item_b: DatasetItem) -> PointCloud:
         media = None
 
         if isinstance(item_a.media, PointCloud) and isinstance(item_b.media, PointCloud):
             item_a_path = getattr(item_a.media, "path", None)
             item_b_path = getattr(item_b.media, "path", None)
 
             if item_a_path and item_b_path and item_a_path != item_b_path:
@@ -249,15 +257,16 @@
         elif isinstance(item_a.media, PointCloud):
             media = item_a.media
         else:
             media = item_b.media
 
         return media
 
-    def _merge_videos(self, item_a: DatasetItem, item_b: DatasetItem) -> Video:
+    @classmethod
+    def _merge_videos(cls, item_a: DatasetItem, item_b: DatasetItem) -> Video:
         media = None
 
         if isinstance(item_a.media, Video) and isinstance(item_b.media, Video):
             if (
                 item_a.media.path is not item_b.media.path
                 or item_a.media._start_frame is not item_b.media._start_frame
                 or item_a.media._end_frame is not item_b.media._end_frame
@@ -269,15 +278,16 @@
         elif isinstance(item_a.media, Video):
             media = item_a.media
         else:
             media = item_b.media
 
         return media
 
-    def _merge_multiframe_images(self, item_a: DatasetItem, item_b: DatasetItem) -> MultiframeImage:
+    @classmethod
+    def _merge_multiframe_images(cls, item_a: DatasetItem, item_b: DatasetItem) -> MultiframeImage:
         media = None
 
         if isinstance(item_a.media, MultiframeImage) and isinstance(item_b.media, MultiframeImage):
             if item_a.media.path and item_b.media.path and item_a.media.path != item_b.media.path:
                 raise MismatchingMediaPathError(
                     (item_a.id, item_a.subset), item_a.media.path, item_b.media.path
                 )
@@ -300,9 +310,10 @@
         elif isinstance(item_a.media, MultiframeImage):
             media = item_a.media
         else:
             media = item_b.media
 
         return media
 
-    def _merge_anno(self, a: Iterable[Annotation], b: Iterable[Annotation]) -> List[Annotation]:
-        return self._merge_annotations_equal(a, b)
+    @classmethod
+    def _merge_anno(cls, a: Iterable[Annotation], b: Iterable[Annotation]) -> List[Annotation]:
+        return cls._merge_annotations_equal(a, b)
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/merge/intersect_merge.py` & `datumaro-1.4.0rc3/src/datumaro/components/merge/intersect_merge.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/merge/union_merge.py` & `datumaro-1.4.0rc3/src/datumaro/components/merge/union_merge.py`

 * *Files 20% similar despite different names*

```diff
@@ -64,43 +64,25 @@
             label_cat = LabelCategories()
         dst_categories[AnnotationType.label] = label_cat
 
         return dst_categories
 
     def _merge_label_categories(self, sources: Sequence[IDataset]) -> LabelCategories:
         dst_cat = LabelCategories()
-        dst_indices = {}
-        dst_labels = []
-
         for src_id, src_categories in enumerate(sources):
             src_cat = src_categories.get(AnnotationType.label)
             if src_cat is None:
                 continue
 
             for src_label in src_cat.items:
-                if src_label.name not in dst_labels:
+                src_idx = src_cat.find(src_label.name)[0]
+                dst_idx = dst_cat.find(src_label.name)[0]
+                if dst_idx is None:
                     dst_cat.add(src_label.name, src_label.parent, src_label.attributes)
-                    dst_labels.append(src_label.name)
+                    dst_idx = dst_cat.find(src_label.name)[0]
 
-                    if src_cat._indices[src_label.name] in list(dst_indices.values()):
-                        dst_indices[src_label.name] = max(dst_indices.values()) + 1
-                        if self._matching_table.get(src_id, None):
-                            self._matching_table[src_id].update(
-                                {src_cat._indices[src_label.name]: max(dst_indices.values())}
-                            )
-                        else:
-                            self._matching_table[src_id] = {
-                                src_cat._indices[src_label.name]: max(dst_indices.values())
-                            }
-                    else:
-                        dst_indices[src_label.name] = src_cat._indices[src_label.name]
+                if self._matching_table.get(src_id, None):
+                    self._matching_table[src_id].update({src_idx: dst_idx})
                 else:
-                    if self._matching_table.get(src_id, None):
-                        self._matching_table[src_id].update(
-                            {src_cat._indices[src_label.name]: dst_indices[src_label.name]}
-                        )
-                    else:
-                        self._matching_table[src_id] = {
-                            src_cat._indices[src_label.name]: dst_indices[src_label.name]
-                        }
+                    self._matching_table[src_id] = {src_idx: dst_idx}
 
         return dst_cat
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/operations.py` & `datumaro-1.4.0rc3/src/datumaro/components/operations.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/progress_reporting.py` & `datumaro-1.4.0rc3/src/datumaro/components/progress_reporting.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,12 +182,14 @@
         self._cur = 0
 
     def report_status(self, progress: int):
         self._pbar.update(progress - self._cur)
         self._cur = progress
 
     def finish(self):
+        if self._total is None:
+            self._total = self._cur  # Total can be None
         self._pbar.update(self._total - self._cur)
         self._pbar.close()
 
     def split(self, count: int):
         return (TQDMProgressReporter(self._period, self._interval, **self._options),) * count
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/project.py` & `datumaro-1.4.0rc3/src/datumaro/components/project.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/shift_analyzer.py` & `datumaro-1.4.0rc3/src/datumaro/components/shift_analyzer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/transformer.py` & `datumaro-1.4.0rc3/src/datumaro/components/transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,17 @@
         ):
             self._length = len(self._extractor)
         return super().__len__()
 
     def media_type(self):
         return self._extractor.media_type()
 
+    def infos(self):
+        return self._extractor.infos()
+
 
 class ItemTransform(Transform):
     def transform_item(self, item: DatasetItem) -> Optional[DatasetItem]:
         """
         Returns a modified copy of the input item.
 
         Avoid changing and returning the input item, because it can lead to
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/validator.py` & `datumaro-1.4.0rc3/src/datumaro/components/validator.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/components/visualizer.py` & `datumaro-1.4.0rc3/src/datumaro/components/visualizer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/ac_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/details/ac.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/accuracy_checker_plugin/details/representation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ade20k2017.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ade20k2017.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ade20k2020.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ade20k2020.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/arrow_dataset.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/base.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import pyarrow as pa
 
 from datumaro.components.dataset_base import SubsetBase
 from datumaro.components.errors import MediaTypeError
 from datumaro.components.importer import ImportContext
 from datumaro.components.media import MediaType
 from datumaro.components.merge import get_merger
-from datumaro.plugins.data_formats.datumaro.base import DatumaroBase
+from datumaro.plugins.data_formats.datumaro.base import JsonReader
 from datumaro.plugins.data_formats.datumaro_binary.mapper.common import DictMapper
 
 from .arrow_dataset import ArrowDataset
 from .mapper.dataset_item import DatasetItemMapper
 
 
 class ArrowBase(SubsetBase):
@@ -43,20 +43,20 @@
         media_types = set()
 
         for path in self._paths:
             with pa.ipc.open_stream(path) as reader:
                 schema = reader.schema
 
                 _infos, _ = DictMapper.backward(schema.metadata.get(b"infos", b"\x00\x00\x00\x00"))
-                infos.append(DatumaroBase._load_infos({"infos": _infos}))
+                infos.append(JsonReader._load_infos({"infos": _infos}))
 
                 _categories, _ = DictMapper.backward(
                     schema.metadata.get(b"categories", b"\x00\x00\x00\x00")
                 )
-                categories.append(DatumaroBase._load_categories({"categories": _categories}))
+                categories.append(JsonReader._load_categories({"categories": _categories}))
 
                 (media_type,) = struct.unpack(
                     "<I", schema.metadata.get(b"media_type", b"\x00\x00\x00\x00")
                 )
                 media_types.add(MediaType(media_type).media)
 
                 dataset = ArrowDataset(path)
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/exporter.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/format.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/importer.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/media.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/arrow/mapper/utils.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/arrow/mapper/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ava/ava.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ava/ava.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/ava/ava_label_pb2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/brats.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/brats.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/brats_numpy.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/brats_numpy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/camvid.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/camvid.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/celeba/align_celeba.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/celeba/align_celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/celeba/celeba.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/celeba/celeba.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cifar.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cifar.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cityscapes.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cityscapes.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: MIT
 
 import errno
 import logging as log
 import os.path as osp
 from inspect import isclass
-from typing import Any, Dict, Optional, Tuple, Type, TypeVar, Union, overload
+from typing import Any, Dict, Iterator, Optional, Tuple, Type, TypeVar, Union, overload
 
 import pycocotools.mask as mask_utils
 from attrs import define
 
 from datumaro.components.annotation import (
     AnnotationType,
     Bbox,
@@ -36,14 +36,15 @@
 from datumaro.components.media import Image
 from datumaro.util import NOTSET, parse_json_file, take_by
 from datumaro.util.image import lazy_image, load_image
 from datumaro.util.mask_tools import bgr2index
 from datumaro.util.meta_file_util import has_meta_file, parse_meta_file
 
 from .format import CocoImporterType, CocoPath, CocoTask
+from .page_mapper import COCOPageMapper
 
 T = TypeVar("T")
 
 
 class DirPathExtracter:
     @staticmethod
     def find_rootpath(path: str) -> str:
@@ -98,14 +99,15 @@
         path,
         task,
         *,
         merge_instance_polygons: bool = False,
         keep_original_category_ids: bool = False,
         coco_importer_type: CocoImporterType = CocoImporterType.default,
         subset: Optional[str] = None,
+        stream: bool = False,
         ctx: Optional[ImportContext] = None,
     ):
         if not osp.isfile(path):
             raise FileNotFoundError(errno.ENOENT, "Can't find JSON file", path)
         self._path = path
 
         if not subset:
@@ -122,29 +124,62 @@
         else:
             raise DatasetImportError(f"Not supported type: {coco_importer_type}")
 
         self._task = task
 
         self._merge_instance_polygons = merge_instance_polygons
 
-        json_data = parse_json_file(path)
         self._label_map = {}  # coco_id -> dm_id
-        self._load_categories(
-            json_data,
-            keep_original_ids=keep_original_category_ids,
-        )
-
         if self._task == CocoTask.panoptic:
             self._mask_dir = osp.splitext(path)[0]
-        self._items = self._load_items(json_data)
+        else:
+            self._mask_dir = None
 
-        del json_data
+        self._stream = stream
+        if not stream:
+            self._page_mapper = None  # No use in case of stream = False
 
-    def __iter__(self):
-        yield from self._items.values()
+            json_data = parse_json_file(path)
+
+            self._load_categories(
+                json_data,
+                keep_original_ids=keep_original_category_ids,
+            )
+
+            self._items = self._load_items(json_data)
+
+            del json_data
+        else:
+            self._page_mapper = COCOPageMapper(path)
+
+            categories_data = self._page_mapper.stream_parse_categories_data()
+
+            self._load_categories(
+                {"categories": categories_data},
+                keep_original_ids=keep_original_category_ids,
+            )
+
+            self._length = None
+
+    def __len__(self) -> int:
+        if self.is_stream:
+            if self._length is None:
+                # Before we actually iterate over the items, we use the length of item page map.
+                # It can be different with the actual length,
+                # because there is a possiblity that an item cannot be parsed properly.
+                return len(self._page_mapper)
+            return self._length
+        else:
+            return len(self._items)
+
+    def __iter__(self) -> Iterator[DatasetItem]:
+        if self.is_stream:
+            yield from self._stream_items()
+        else:
+            yield from self._items.values()
 
     def _load_categories(self, json_data, *, keep_original_ids):
         self._categories = {}
 
         if has_meta_file(self._rootpath):
             labels = parse_meta_file(self._rootpath).keys()
             self._categories = {AnnotationType.label: LabelCategories.from_iterable(labels)}
@@ -221,94 +256,112 @@
                 label_id,
                 labels=self._parse_field(cat, "keypoints", list),
                 joints=self._parse_field(cat, "skeleton", list),
             )
 
         self._categories[AnnotationType.points] = categories
 
+    def _stream_items(self) -> Iterator[DatasetItem]:
+        pbars = self._ctx.progress_reporter
+        length = 0
+
+        for img_info, ann_infos in pbars.iter(
+            self._page_mapper,
+            desc=f"Importing '{self._subset}'",
+        ):
+            parsed = self._parse_item(img_info)
+            if parsed is None:
+                continue
+
+            _, item = parsed
+
+            for ann_info in ann_infos:
+                self._parse_anns(img_info, ann_info, item)
+
+            yield item
+            length += 1
+
+        self._length = length
+
+    def _parse_anns(self, img_info, ann_info, item):
+        if self._task is not CocoTask.panoptic:
+            self._load_annotations(ann_info, img_info, parsed_annotations=item.annotations)
+        else:
+            self._load_panoptic_ann(ann_info, parsed_annotations=item.annotations)
+
     def _load_items(self, json_data):
-        pbars = self._ctx.progress_reporter.split(2)
+        pbar = self._ctx.progress_reporter
 
         def _gen_ann(info_lists):
             while info_lists:
                 yield info_lists.pop()
 
         items = {}
         img_infos = {}
         img_lists = self._parse_field(json_data, "images", list)
-        for img_info in pbars[0].iter(
-            _gen_ann(img_lists),
-            desc=f"Parsing image info in '{osp.basename(self._path)}'",
+        for img_info in _gen_ann(img_lists):
+            parsed = self._parse_item(img_info)
+            if parsed is None:
+                continue
+
+            img_id, item = parsed
+
+            # Store item (DatasetItem) and img_info (Dict) to the integer key dictionary
+            items[img_id] = item
+            img_infos[img_id] = img_info
+
+        ann_lists = self._parse_field(json_data, "annotations", list)
+
+        for ann_info in pbar.iter(
+            _gen_ann(ann_lists),
+            desc=f"Importing '{self._subset}'",
+            total=len(ann_lists),
         ):
-            img_id = None
             try:
-                img_id = self._parse_field(img_info, "id", int)
-                img_infos[img_id] = img_info
+                img_id = self._parse_field(ann_info, "image_id", int)
+                if img_id not in img_infos:
+                    log.warn(f"Unknown image id '{img_id}'")
+                    continue
+
+                # Retrieve item (DatasetItem) and img_info (Dict) from the integer key dictionary
+                item = items[img_id]
+                img_info = img_infos[img_id]
+                self._parse_anns(img_info, ann_info, item)
 
-                if img_info.get("height") and img_info.get("width"):
-                    image_size = (
-                        self._parse_field(img_info, "height", int),
-                        self._parse_field(img_info, "width", int),
-                    )
-                else:
-                    image_size = None
-
-                file_name = self._parse_field(img_info, "file_name", str)
-                items[img_id] = DatasetItem(
-                    id=osp.splitext(file_name)[0],
-                    subset=self._subset,
-                    media=Image.from_file(
-                        path=osp.join(self._images_dir, file_name), size=image_size
-                    ),
-                    annotations=[],
-                    attributes={"id": img_id},
-                )
             except Exception as e:
-                self._ctx.error_policy.report_item_error(e, item_id=(img_id, self._subset))
+                self._ctx.error_policy.report_annotation_error(
+                    e, item_id=(ann_info.get("id", None), self._subset)
+                )
 
-        if self._task is not CocoTask.panoptic:
-            ann_lists = self._parse_field(json_data, "annotations", list)
-            for ann in pbars[1].iter(
-                _gen_ann(ann_lists),
-                desc=f"Parsing annotations in '{osp.basename(self._path)}'",
-            ):
-                img_id = None
-                try:
-                    img_id = self._parse_field(ann, "image_id", int)
-                    if img_id not in img_infos:
-                        log.warn(f"Unknown image id '{img_id}'")
-                        continue
+        return items
 
-                    self._load_annotations(
-                        ann, img_infos[img_id], parsed_annotations=items[img_id].annotations
-                    )
-                except Exception as e:
-                    self._ctx.error_policy.report_annotation_error(
-                        e, item_id=(img_id, self._subset)
-                    )
-        else:
-            ann_lists = self._parse_field(json_data, "annotations", list)
-            for ann in pbars[1].iter(
-                _gen_ann(ann_lists),
-                desc=f"Parsing annotations in '{osp.basename(self._path)}'",
-            ):
-                img_id = None
-                try:
-                    img_id = self._parse_field(ann, "image_id", int)
-                    if img_id not in img_infos:
-                        log.warn(f"Unknown image id '{img_id}'")
-                        continue
-
-                    self._load_panoptic_ann(ann, items[img_id].annotations)
-                except Exception as e:
-                    self._ctx.error_policy.report_annotation_error(
-                        e, item_id=(img_id, self._subset)
-                    )
+    def _parse_item(self, img_info: Dict[str, Any]) -> Optional[Tuple[int, DatasetItem]]:
+        try:
+            img_id = self._parse_field(img_info, "id", int)
+
+            if img_info.get("height") and img_info.get("width"):
+                image_size = (
+                    self._parse_field(img_info, "height", int),
+                    self._parse_field(img_info, "width", int),
+                )
+            else:
+                image_size = None
 
-        return items
+            file_name = self._parse_field(img_info, "file_name", str)
+            return img_id, DatasetItem(
+                id=osp.splitext(file_name)[0],
+                subset=self._subset,
+                media=Image.from_file(path=osp.join(self._images_dir, file_name), size=image_size),
+                annotations=[],
+                attributes={"id": img_id},
+            )
+        except Exception as e:
+            self._ctx.error_policy.report_item_error(
+                e, item_id=(img_info.get("id", None), self._subset)
+            )
 
     def _load_panoptic_ann(self, ann, parsed_annotations=None):
         if parsed_annotations is None:
             parsed_annotations = []
 
         # For the panoptic task, each annotation struct is a per-image
         # annotation rather than a per-object annotation.
@@ -518,14 +571,42 @@
                 Caption(caption, id=ann_id, attributes=attributes, group=group)
             )
         else:
             raise NotImplementedError()
 
         return parsed_annotations
 
+    @property
+    def is_stream(self) -> bool:
+        return self._stream
+
+    def get_dataset_item(self, item_key: int) -> Optional[DatasetItem]:
+        if self.is_stream:
+            img_info = self._page_mapper.get_item_dict(item_key)
+            ann_infos = self._page_mapper.get_anns_dict(item_key)
+
+            parsed = self._parse_item(img_info)
+            if parsed is None:
+                return None
+
+            _, item = parsed
+
+            for ann_info in ann_infos:
+                self._parse_anns(img_info, ann_info, item)
+
+            return item
+        else:
+            return self._items[item_key]
+
+    def iter_item_ids(self) -> Iterator[int]:
+        if self.is_stream:
+            return self._page_mapper.iter_item_ids()
+        else:
+            return self._items.keys()
+
 
 class CocoImageInfoBase(_CocoBase):
     def __init__(self, path, **kwargs):
         kwargs["task"] = CocoTask.image_info
         super().__init__(path, **kwargs)
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/exporter.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/exporter.py`

 * *Files 0% similar despite different names*

```diff
@@ -727,15 +727,15 @@
         for pbar, (subset_name, subset) in zip(pbars, subsets.items()):
             task_converters = self._make_task_converters()
             for task_conv in task_converters.values():
                 task_conv.save_categories(subset)
             if CocoTask.panoptic in task_converters:
                 self._make_segmentation_dir(subset_name)
 
-            for item in pbar.iter(subset, desc=f"Exporting {subset_name}"):
+            for item in pbar.iter(subset, desc=f"Exporting '{subset_name}'"):
                 try:
                     if self._save_media:
                         if item.media:
                             self._save_image(
                                 item,
                                 subdir=osp.join(
                                     self._images_dir, "" if self._merge_images else subset_name
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/format.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/coco/importer.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/coco/importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # Copyright (C) 2019-2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import logging as log
 import os.path as osp
 from glob import glob
+from typing import Optional
 
 from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME
 from datumaro.components.errors import DatasetNotFoundError
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import Importer
+from datumaro.components.merge.extractor_merger import ExtractorMerger
 from datumaro.plugins.data_formats.coco.base import (
     CocoCaptionsBase,
     CocoImageInfoBase,
     CocoInstancesBase,
     CocoLabelsBase,
     CocoPanopticBase,
     CocoPersonKeypointsBase,
     CocoStuffBase,
 )
+from datumaro.plugins.data_formats.coco.extractor_merger import COCOExtractorMerger
 
 from .format import CocoImporterType, CocoTask
 
 
 class CocoImporter(Importer):
     _TASKS = {
         CocoTask.instances: CocoInstancesBase,
@@ -60,15 +63,15 @@
             context.raise_unsupported()
 
         with context.require_any():
             for task in cls._TASKS.keys():
                 with context.alternative():
                     context.require_file(f"annotations/{task.name}_*.json")
 
-    def __call__(self, path, **extra_params):
+    def __call__(self, path, stream: bool = False, **extra_params):
         subsets = self.find_sources(path)
 
         if len(subsets) == 0:
             raise DatasetNotFoundError(path, self.NAME)
 
         # TODO: should be removed when proper label merging is implemented
         conflicting_types = {
@@ -100,14 +103,17 @@
                         continue
                 log.info("Found a dataset at '%s'" % ann_file)
 
                 options = dict(extra_params)
                 options["coco_importer_type"] = self._IMPORTER_TYPE
                 options["subset"] = subset
 
+                if stream:
+                    options["stream"] = True
+
                 sources.append(
                     {
                         "url": ann_file,
                         "format": self._TASKS[ann_type].NAME,
                         "options": options,
                     }
                 )
@@ -148,14 +154,21 @@
                 ann_type.name + "_", maxsplit=1
             )
             subset_name = parts[1] if len(parts) == 2 else DEFAULT_SUBSET_NAME
             subsets.setdefault(subset_name, {})[ann_type] = subset_path
 
         return subsets
 
+    @property
+    def can_stream(self) -> bool:
+        return True
+
+    def get_extractor_merger(self) -> Optional[ExtractorMerger]:
+        return COCOExtractorMerger
+
 
 class CocoImageInfoImporter(CocoImporter):
     _TASK = CocoTask.image_info
     _TASKS = {_TASK: CocoImporter._TASKS[_TASK]}
 
 
 class CocoCaptionsImporter(CocoImporter):
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/common_semantic_segmentation.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/common_semantic_segmentation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/common_super_resolution.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/common_super_resolution.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/exporter.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/cvat/format.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/cvat/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/roboflow/base.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,328 +1,344 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
+import csv
+import errno
+import os
 import os.path as osp
-from typing import Optional
+import re
+from typing import Dict, List, Optional, Union
+from xml.etree import ElementTree
 
 from datumaro.components.annotation import (
+    Annotation,
     AnnotationType,
     Bbox,
-    Caption,
-    Cuboid3d,
-    Ellipse,
     Label,
     LabelCategories,
-    MaskCategories,
-    Points,
-    PointsCategories,
     Polygon,
-    PolyLine,
-    RleMask,
 )
-from datumaro.components.dataset_base import DatasetItem, SubsetBase
-from datumaro.components.errors import DatasetImportError, MediaTypeError
+from datumaro.components.dataset import DatasetItem
+from datumaro.components.dataset_base import SubsetBase
+from datumaro.components.errors import InvalidAnnotationError, UndeclaredLabelError
 from datumaro.components.importer import ImportContext
-from datumaro.components.media import Image, MediaElement, PointCloud
+from datumaro.components.media import Image, ImageFromFile
+from datumaro.plugins.data_formats.coco.base import _CocoBase
+from datumaro.plugins.data_formats.coco.format import CocoImporterType, CocoTask
+from datumaro.plugins.data_formats.tf_detection_api.base import TfDetectionApiBase
+from datumaro.plugins.data_formats.tf_detection_api.format import TfrecordImporterType
+from datumaro.plugins.data_formats.voc.base import VocBase
+from datumaro.plugins.data_formats.voc.format import VocImporterType, VocTask
+from datumaro.plugins.data_formats.yolo.base import YoloUltralyticsBase
 from datumaro.util import parse_json_file
-from datumaro.version import __version__
+from datumaro.util.image import IMAGE_EXTENSIONS, ImageMeta
+from datumaro.util.os_util import find_files
 
-from .format import DATUMARO_FORMAT_VERSION, DatumaroPath
 
+class RoboflowCocoBase(_CocoBase):
+    """
+    Parses Roboflow COCO annotations written in the following format:
+    https://cocodataset.org/#format-data
+    """
 
-class DatumaroBase(SubsetBase):
-    LEGACY_VERSION = "legacy"
-    CURRENT_DATUMARO_FORMAT_VERSION = DATUMARO_FORMAT_VERSION
+    def __init__(
+        self,
+        path,
+        *,
+        subset: Optional[str] = None,
+        stream: bool = False,
+        ctx: Optional[ImportContext] = None,
+    ):
+        super().__init__(
+            path,
+            task=CocoTask.instances,
+            coco_importer_type=CocoImporterType.roboflow,
+            subset=subset,
+            stream=stream,
+            ctx=ctx,
+        )
 
-    # If Datumaro format version goes up, it will be
-    # ALLOWED_VERSIONS = {LEGACY_VERSION, 1.0, ..., CURRENT_DATUMARO_FORMAT_VERSION}
-    ALLOWED_VERSIONS = {LEGACY_VERSION, CURRENT_DATUMARO_FORMAT_VERSION}
 
+class RoboflowVocBase(VocBase):
     def __init__(
         self,
         path: str,
         *,
         subset: Optional[str] = None,
         ctx: Optional[ImportContext] = None,
     ):
-        assert osp.isfile(path), path
+        super().__init__(
+            path,
+            task=VocTask.voc_detection,
+            voc_importer_type=VocImporterType.roboflow,
+            subset=subset,
+            ctx=ctx,
+        )
+
+    def _load_categories(self, path):
+        cats = set()
+        ann_files = [file for file in os.listdir(path) if file.endswith(".xml")]
+        for ann_file in ann_files:
+            xml_file = osp.join(path, ann_file)
 
-        dm_version = self._get_dm_format_version(path)
+            root = ElementTree.parse(xml_file).getroot()
 
-        # when backward compatibility happen, we should implement version specific readers
-        if dm_version not in self.ALLOWED_VERSIONS:
-            raise DatasetImportError(
-                f"Datumaro format version of the given dataset is {dm_version}, "
-                f"but not supported by this Datumaro version: {__version__}. "
-                f"The allowed datumaro format versions are {self.ALLOWED_VERSIONS}. "
-                "Please install the latest Datumaro."
-            )
+            if root.tag != "annotation":
+                continue
 
-        self.default_reader(path=path, subset=subset, ctx=ctx)
+            for object_elem in root.iterfind("object"):
+                cat_name = self._parse_field(object_elem, "name")
+                cats.add(cat_name)
+
+        label_categories = LabelCategories()
+        for _, cat in enumerate(sorted(cats)):
+            label_categories.add(cat)
 
-    def default_reader(self, path, subset, ctx):
-        """
-        Default Datumaro reader for the latest version
-        """
-        rootpath = ""
-        if path.endswith(osp.join(DatumaroPath.ANNOTATIONS_DIR, osp.basename(path))):
-            rootpath = path.rsplit(DatumaroPath.ANNOTATIONS_DIR, maxsplit=1)[0]
-        self._rootpath = rootpath
-
-        images_dir = ""
-        if rootpath and osp.isdir(osp.join(rootpath, DatumaroPath.IMAGES_DIR)):
-            images_dir = osp.join(rootpath, DatumaroPath.IMAGES_DIR)
-        self._images_dir = images_dir
-
-        pcd_dir = ""
-        if rootpath and osp.isdir(osp.join(rootpath, DatumaroPath.PCD_DIR)):
-            pcd_dir = osp.join(rootpath, DatumaroPath.PCD_DIR)
-        self._pcd_dir = pcd_dir
+        categories = {AnnotationType.label: label_categories}
 
-        if not subset:
-            subset = osp.splitext(osp.basename(path))[0]
+        return categories
 
-        super().__init__(subset=subset, ctx=ctx)
-        self._load_impl(path)
+    def _load_subset_list(self, path):
+        return [os.path.splitext(file)[0] for file in os.listdir(path) if file.endswith(".xml")]
 
-    def _get_dm_format_version(self, path: str):
-        """
-        Get Datumaro format at exporting the dataset
-
-        Note that the regacy Datumaro doesn't store the version into exported dataset.
-        Thus it returns DatumaroBase.REGACY_VERSION
-        """
-        self._parsed_anns = parse_json_file(path)
-        return self._parsed_anns.get("dm_format_version", self.LEGACY_VERSION)
-
-    def _load_impl(self, path: str) -> None:
-        """Actual implementation of loading Datumaro format."""
-        self._infos = self._load_infos(self._parsed_anns)
-        self._categories = self._load_categories(self._parsed_anns)
-        self._items = self._load_items(self._parsed_anns)
 
-    @staticmethod
-    def _load_infos(parsed):
-        return parsed.get("infos", {})
+class RoboflowYoloBase(YoloUltralyticsBase):
+    def __init__(
+        self,
+        config_path: str,
+        image_info: Union[None, str, ImageMeta] = None,
+        urls: Optional[List[str]] = None,
+        **kwargs,
+    ) -> None:
+        super().__init__(config_path, image_info, urls, **kwargs)
+
+    def _get_rootpath(self, config_path: str) -> str:
+        return osp.dirname(config_path)
+
+    def _load_img_files(self, rootpath: str) -> Dict:
+        return {
+            self._get_fname(img_file): img_file
+            for img_file in find_files(rootpath, IMAGE_EXTENSIONS, recursive=True, max_depth=2)
+            if osp.split(osp.relpath(osp.dirname(img_file), rootpath))[0] == self._subset
+        }
 
-    @staticmethod
-    def _load_categories(parsed):
-        categories = {}
 
-        parsed_label_cat = parsed["categories"].get(AnnotationType.label.name)
-        if parsed_label_cat:
-            label_categories = LabelCategories(attributes=parsed_label_cat.get("attributes", []))
-            for item in parsed_label_cat["labels"]:
-                label_categories.add(
-                    item["name"],
-                    parent=item["parent"],
-                    attributes=item.get("attributes", []),
-                )
+class RoboflowYoloObbBase(RoboflowYoloBase):
+    def __init__(
+        self,
+        config_path: str,
+        image_info: Union[None, str, ImageMeta] = None,
+        urls: Optional[List[str]] = None,
+        **kwargs,
+    ) -> None:
+        super().__init__(config_path, image_info, urls, **kwargs)
 
-            for item in parsed_label_cat.get("label_groups", []):
-                label_categories.add_label_group(
-                    item["name"], labels=item["labels"], group_type=item["group_type"]
+    def _parse_annotations(
+        self,
+        anno_path: str,
+        image: ImageFromFile,
+        *,
+        label_categories: LabelCategories,
+    ) -> List[Annotation]:
+        lines = []
+        with open(anno_path, "r", encoding="utf-8") as f:
+            for line in f:
+                line = line.strip()
+                if line:
+                    lines.append(line)
+
+        annotations = []
+        for idx, line in enumerate(lines):
+            parts = line.split()
+            if len(parts) != 10:
+                raise InvalidAnnotationError(
+                    f"Unexpected field count {len(parts)} in the bbox description. "
+                    "Expected 10 fields (x1, y1, x2, y2, x3, y3, x4, y4, label, 0)."
                 )
+            x1, y1, x2, y2, x3, y3, x4, y4, label_name = parts[:-1]
 
-            categories[AnnotationType.label] = label_categories
+            label_name = self._parse_field(label_name, str, "bbox label name")
+            label_id = label_categories.find(label_name)[0]
 
-        parsed_mask_cat = parsed["categories"].get(AnnotationType.mask.name)
-        if parsed_mask_cat:
-            colormap = {}
-            for item in parsed_mask_cat["colormap"]:
-                colormap[int(item["label_id"])] = (item["r"], item["g"], item["b"])
-
-            mask_categories = MaskCategories(colormap=colormap)
-            categories[AnnotationType.mask] = mask_categories
-
-        parsed_points_cat = parsed["categories"].get(AnnotationType.points.name)
-        if parsed_points_cat:
-            point_categories = PointsCategories()
-            for item in parsed_points_cat["items"]:
-                point_categories.add(int(item["label_id"]), item["labels"], joints=item["joints"])
+            if label_id is None:
+                raise UndeclaredLabelError(str(label_id))
 
-            categories[AnnotationType.points] = point_categories
+            x1 = self._parse_field(x1, float, "x1")
+            y1 = self._parse_field(y1, float, "y1")
+            x2 = self._parse_field(x2, float, "x2")
+            y2 = self._parse_field(y2, float, "y2")
+            x3 = self._parse_field(x3, float, "x3")
+            y3 = self._parse_field(y3, float, "y3")
+            x4 = self._parse_field(x4, float, "x4")
+            y4 = self._parse_field(y4, float, "y4")
+            annotations.append(
+                Polygon(
+                    points=[x1, y1, x2, y2, x3, y3, x4, y4],
+                    label=label_id,
+                    id=idx,
+                    group=idx,
+                )
+            )
 
-        return categories
+        return annotations
 
-    def _load_items(self, parsed):
-        items = []
 
-        item_descs = parsed["items"]
-        while item_descs:
-            item_desc = item_descs.pop()
-            item_id = item_desc["id"]
-
-            media = None
-            image_info = item_desc.get("image")
-            if image_info:
-                image_filename = image_info.get("path") or item_id + DatumaroPath.IMAGE_EXT
-                image_path = osp.join(self._images_dir, self._subset, image_filename)
-                if not osp.isfile(image_path):
-                    # backward compatibility
-                    old_image_path = osp.join(self._images_dir, image_filename)
-                    if osp.isfile(old_image_path):
-                        image_path = old_image_path
-
-                media = Image.from_file(path=image_path, size=image_info.get("size"))
-                self._media_type = Image
-
-            pcd_info = item_desc.get("point_cloud")
-            if media and pcd_info:
-                raise MediaTypeError("Dataset cannot contain multiple media types")
-            if pcd_info:
-                pcd_path = pcd_info.get("path")
-                point_cloud = osp.join(self._pcd_dir, self._subset, pcd_path)
-
-                related_images = None
-                ri_info = item_desc.get("related_images")
-                if ri_info:
-                    related_images = [
-                        Image.from_file(
-                            size=ri.get("size"),
-                            path=osp.join(self._images_dir, self._subset, ri.get("path")),
-                        )
-                        for ri in ri_info
-                    ]
+class RoboflowCreateMlBase(SubsetBase):
+    """
+    Parses Roboflow CreateML annotations written in the following format:
+    https://cocodataset.org/#format-data
+    """
+
+    def __init__(
+        self,
+        path,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
+        if not osp.isfile(path):
+            raise FileNotFoundError(errno.ENOENT, "Can't find JSON file", path)
+        self._path = path
+
+        if not subset:
+            subset = osp.splitext(osp.basename(path))[0]
+        super().__init__(subset=subset, ctx=ctx)
 
-                media = PointCloud.from_file(path=point_cloud, extra_images=related_images)
-                self._media_type = PointCloud
+        json_data = parse_json_file(path)
+        self._categories = self._load_categories(json_data)
+        self._items = self._load_items(json_data)
+
+    def _load_categories(self, json_data):
+        cats = set()
+        for anns in json_data:
+            for ann in anns["annotations"]:
+                cats.add(ann["label"])
+
+        label_categories = LabelCategories()
+        for cat in sorted(cats):
+            label_categories.add(cat)
 
-            media_desc = item_desc.get("media")
-            if not media and media_desc and media_desc.get("path"):
-                media = MediaElement(path=media_desc.get("path"))
-                self._media_type = MediaElement
+        categories = {AnnotationType.label: label_categories}
 
-            annotations = self._load_annotations(item_desc)
+        return categories
 
-            item = DatasetItem(
-                id=item_id,
+    def _load_items(self, json_data):
+        items = {}
+        for anns in self._ctx.progress_reporter.iter(
+            json_data, desc=f"Parsing boxes in '{self._subset}'"
+        ):
+            annotations = []
+            for ann_id, ann in enumerate(anns["annotations"]):
+                label_id, _ = self._categories[AnnotationType.label].find(ann["label"])
+                if label_id is None:
+                    raise UndeclaredLabelError(ann["label"])
+
+                x = ann["coordinates"]["x"]
+                y = ann["coordinates"]["y"]
+                w = ann["coordinates"]["width"]
+                h = ann["coordinates"]["height"]
+                annotations.append(Bbox(x, y, w, h, label=label_id, id=ann_id, group=ann_id))
+
+            img_id = osp.splitext(anns["image"])[0]
+            items[img_id] = DatasetItem(
+                id=img_id,
                 subset=self._subset,
+                media=Image.from_file(path=osp.join(osp.dirname(self._path), anns["image"])),
                 annotations=annotations,
-                media=media,
-                attributes=item_desc.get("attr"),
             )
 
-            items.append(item)
+        return items.values()
 
-        return items
 
-    @staticmethod
-    def _load_annotations(item):
-        parsed = item["annotations"]
-        loaded = []
-
-        for ann in parsed:
-            ann_id = ann.get("id")
-            ann_type = AnnotationType[ann["type"]]
-            attributes = ann.get("attributes")
-            group = ann.get("group")
-
-            label_id = ann.get("label_id")
-            z_order = ann.get("z_order")
-            points = ann.get("points")
-
-            if ann_type == AnnotationType.label:
-                loaded.append(Label(label=label_id, id=ann_id, attributes=attributes, group=group))
-
-            elif ann_type == AnnotationType.mask:
-                rle = ann["rle"]
-                rle["counts"] = rle["counts"].encode("ascii")
-                loaded.append(
-                    RleMask(
-                        rle=rle,
-                        label=label_id,
-                        id=ann_id,
-                        attributes=attributes,
-                        group=group,
-                        z_order=z_order,
-                    )
-                )
+class RoboflowMulticlassBase(SubsetBase):
+    """
+    Parses Roboflow Multiclass annotations written in the following format:
+    https://cocodataset.org/#format-data
+    """
 
-            elif ann_type == AnnotationType.polyline:
-                loaded.append(
-                    PolyLine(
-                        points,
-                        label=label_id,
-                        id=ann_id,
-                        attributes=attributes,
-                        group=group,
-                        z_order=z_order,
-                    )
-                )
+    def __init__(
+        self,
+        path,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
+        if not osp.isfile(path):
+            raise FileNotFoundError(errno.ENOENT, "Can't find CSV file", path)
+        self._path = path
 
-            elif ann_type == AnnotationType.polygon:
-                loaded.append(
-                    Polygon(
-                        points,
-                        label=label_id,
-                        id=ann_id,
-                        attributes=attributes,
-                        group=group,
-                        z_order=z_order,
-                    )
-                )
+        if not subset:
+            subset = osp.splitext(osp.basename(path))[0]
+        super().__init__(subset=subset, ctx=ctx)
 
-            elif ann_type == AnnotationType.bbox:
-                x, y, w, h = ann["bbox"]
-                loaded.append(
-                    Bbox(
-                        x,
-                        y,
-                        w,
-                        h,
-                        label=label_id,
-                        id=ann_id,
-                        attributes=attributes,
-                        group=group,
-                        z_order=z_order,
-                    )
-                )
+        self._label_mapping = {}
+        self._categories = self._load_categories(path)
+        self._items = self._load_items(path)
+
+    def _load_categories(self, path):
+        with open(path, "r", encoding="utf-8") as f:
+            reader = csv.DictReader(f)
+            cats = [label.strip() for label in reader.fieldnames[1:]]
+
+        label_categories = LabelCategories()
+        for idx, cat in enumerate(sorted(cats)):
+            label_categories.add(cat)
+            self._label_mapping[cat] = idx
 
-            elif ann_type == AnnotationType.points:
-                loaded.append(
-                    Points(
-                        points,
-                        label=label_id,
-                        id=ann_id,
-                        attributes=attributes,
-                        group=group,
-                        z_order=z_order,
-                    )
-                )
+        categories = {AnnotationType.label: label_categories}
 
-            elif ann_type == AnnotationType.caption:
-                caption = ann.get("caption")
-                loaded.append(Caption(caption, id=ann_id, attributes=attributes, group=group))
-
-            elif ann_type == AnnotationType.cuboid_3d:
-                loaded.append(
-                    Cuboid3d(
-                        ann.get("position"),
-                        ann.get("rotation"),
-                        ann.get("scale"),
-                        label=label_id,
-                        id=ann_id,
-                        attributes=attributes,
-                        group=group,
-                    )
-                )
+        return categories
+
+    def _load_items(self, path):
+        items = []
+        with open(path, "r", encoding="utf-8") as f:
+            for anns in csv.DictReader(f):
+                img_id = anns.get("filename", None)
+                img_id = osp.splitext(img_id)[0] if img_id else None
+                idx = 0
+                annotations = []
+                for key, val in anns.items():
+                    if key.strip() not in self._label_mapping:
+                        continue
+                    if int(val) == 1:
+                        annotations.append(
+                            Label(label=self._label_mapping[key.strip()], id=idx, group=idx)
+                        )
+                        idx += 1
 
-            elif ann_type == AnnotationType.ellipse:
-                loaded.append(
-                    Ellipse(
-                        *points,
-                        label=label_id,
-                        id=ann_id,
-                        attributes=attributes,
-                        group=group,
-                        z_order=z_order,
+                items.append(
+                    DatasetItem(
+                        id=img_id,
+                        subset=self._subset,
+                        media=Image.from_file(
+                            path=osp.join(osp.dirname(self._path), anns["filename"])
+                        ),
+                        annotations=annotations,
                     )
                 )
 
-            elif ann_type == AnnotationType.hash_key:
-                continue
-            else:
-                raise NotImplementedError()
+        return items
+
+
+class RoboflowTfrecord(TfDetectionApiBase):
+    def __init__(
+        self,
+        path: str,
+        *,
+        subset: Optional[str] = None,
+        ctx: Optional[ImportContext] = None,
+    ):
+        super().__init__(
+            path=path, subset=subset, tfrecord_importer_type=TfrecordImporterType.roboflow, ctx=ctx
+        )
+
+    @staticmethod
+    def _parse_labelmap(text):
+        entry_pattern = r'name:\s*"([^"]+)"\s*,\s*id:\s*(\d+)'
+        entry_pattern = re.compile(entry_pattern)
+
+        matches = re.findall(entry_pattern, text)
+
+        labelmap = {name: int(id) for name, id in matches}
 
-        return loaded
+        return labelmap
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/exporter.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,29 +29,30 @@
     PointsCategories,
     Polygon,
     PolyLine,
     RleMask,
     _Shape,
 )
 from datumaro.components.crypter import NULL_CRYPTER
-from datumaro.components.dataset_base import DEFAULT_SUBSET_NAME, DatasetItem
+from datumaro.components.dataset_base import DatasetItem
 from datumaro.components.dataset_item_storage import ItemStatus
 from datumaro.components.exporter import ExportContextComponent, Exporter
 from datumaro.components.media import Image, MediaElement, PointCloud
 from datumaro.util import cast, dump_json_file
 
 from .format import DATUMARO_FORMAT_VERSION, DatumaroPath
 
 
 class _SubsetWriter:
     def __init__(self, context: Exporter, ann_file: str, export_context: ExportContextComponent):
         self._context = context
 
         self._data = {
             "dm_format_version": DATUMARO_FORMAT_VERSION,
+            "media_type": context._extractor.media_type()._type,
             "infos": {},
             "categories": {},
             "items": [],
         }
 
         self.ann_file = ann_file
         self.export_context = export_context
@@ -414,19 +415,20 @@
             for subset in self._extractor.subsets()
         }
 
         for writer in writers.values():
             writer.add_infos(self._extractor.infos())
             writer.add_categories(self._extractor.categories())
 
-        for item in self._extractor:
-            subset = item.subset or DEFAULT_SUBSET_NAME
-            writers[subset].add_item(item, pool)
+        pbar = self._ctx.progress_reporter
+        for subset_name, subset in self._extractor.subsets().items():
+            for item in pbar.iter(subset, desc=f"Exporting '{subset_name}'"):
+                writers[subset_name].add_item(item, pool)
 
-            self._check_hash_key_existence(item)
+                self._check_hash_key_existence(item)
 
         for subset, writer in writers.items():
             if self._patch and subset in self._patch.updated_subsets and writer.is_empty():
                 if osp.isfile(writer.ann_file):
                     # Remove subsets that became empty
                     os.remove(writer.ann_file)
                 continue
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro/importer.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro/importer.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # Copyright (C) 2023 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Type
 
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import Importer
+from datumaro.components.merge.extractor_merger import ExtractorMerger
 from datumaro.util import parse_json
 
 from .format import DatumaroPath
 
 
 class DatumaroImporter(Importer):
     PATH_CLS = DatumaroPath
@@ -36,7 +37,14 @@
     def find_sources(cls, path) -> List[Dict]:
         return cls._find_sources_recursive(
             path,
             cls.PATH_CLS.ANNOTATION_EXT,
             cls.NAME,
             dirname=cls.PATH_CLS.ANNOTATIONS_DIR,
         )
+
+    @property
+    def can_stream(self) -> bool:
+        return True
+
+    def get_extractor_merger(self) -> Type[ExtractorMerger]:
+        return ExtractorMerger
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/base.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from datumaro.components.importer import ImportContext
 from datumaro.components.media import Image, MediaElement, MediaType, PointCloud
 from datumaro.plugins.data_formats.datumaro_binary.format import DatumaroBinaryPath
 from datumaro.plugins.data_formats.datumaro_binary.mapper import DictMapper
 from datumaro.plugins.data_formats.datumaro_binary.mapper.common import IntListMapper
 from datumaro.plugins.data_formats.datumaro_binary.mapper.dataset_item import DatasetItemMapper
 
-from ..datumaro.base import DatumaroBase
+from ..datumaro.base import DatumaroBase, JsonReader
 
 
 class DatumaroBinaryBase(DatumaroBase):
     """"""
 
     def __init__(
         self,
@@ -96,15 +96,15 @@
         return version_header["dm_format_version"]
 
     def _read_info(self):
         self._infos = self._read_header()
 
     def _read_categories(self):
         categories = self._read_header()
-        self._categories = self._load_categories({"categories": categories})
+        self._categories = JsonReader._load_categories({"categories": categories})
 
     def _read_media_type(self):
         media_type = self._read_header()["media_type"]
         if media_type == MediaType.IMAGE:
             self._media_type = Image
         elif media_type == MediaType.POINT_CLOUD:
             self._media_type = PointCloud
@@ -181,7 +181,26 @@
         while offset < len(blob_bytes):
             item, offset = DatasetItemMapper.backward(blob_bytes, offset, media_path_prefix)
             items.append(item)
 
         assert offset == len(blob_bytes)
 
         return items
+
+    @property
+    def is_stream(self) -> bool:
+        return False
+
+    def infos(self):
+        return self._infos
+
+    def categories(self):
+        return self._categories
+
+    def media_type(self):
+        return self._media_type
+
+    def __len__(self) -> int:
+        return len(self._items)
+
+    def __iter__(self) -> DatasetItem:
+        yield from self._items
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/format.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/importer.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/__init__.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/annotation.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/common.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/dataset_item.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/datumaro_binary/mapper/media.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/icdar/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/icdar/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/icdar/exporter.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/icdar/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/image_dir.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/image_dir.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/image_zip.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/image_zip.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/imagenet.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/imagenet.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/imagenet_txt.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/imagenet_txt.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kinetics.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kinetics.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/exporter.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/format.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti/importer.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/exporter.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/kitti_raw/format.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/kitti_raw/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/labelme.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/labelme.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/lfw.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/lfw.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/format.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mapillary_vistas/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/market1501.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/market1501.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mars.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mars.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mnist.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mnist.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mnist_csv.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mnist_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mot.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mot.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mots.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mots.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/format.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/mpii_json.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/mpii_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mpii/mpii_mat.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mpii/mpii_mat.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/exporter.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/format.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/mvtec/importer.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/mvtec/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/nyu_depth_v2.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/nyu_depth_v2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/open_images.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/open_images.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/roboflow/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/image_generator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,342 +1,298 @@
-# Copyright (C) 2023 Intel Corporation
+# Copyright (C) 2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
-import csv
-import errno
+import hashlib
+import logging as log
 import os
 import os.path as osp
-import re
-from typing import Dict, List, Optional, Union
-from xml.etree import ElementTree
-
-from datumaro.components.annotation import (
-    Annotation,
-    AnnotationType,
-    Bbox,
-    Label,
-    LabelCategories,
-    Polygon,
-)
-from datumaro.components.dataset import DatasetItem
-from datumaro.components.dataset_base import SubsetBase
-from datumaro.components.errors import InvalidAnnotationError, UndeclaredLabelError
-from datumaro.components.importer import ImportContext
-from datumaro.components.media import Image, ImageFromFile
-from datumaro.plugins.data_formats.coco.base import _CocoBase
-from datumaro.plugins.data_formats.coco.format import CocoImporterType, CocoTask
-from datumaro.plugins.data_formats.tf_detection_api.base import TfDetectionApiBase
-from datumaro.plugins.data_formats.tf_detection_api.format import TfrecordImporterType
-from datumaro.plugins.data_formats.voc.base import VocBase
-from datumaro.plugins.data_formats.voc.format import VocImporterType, VocTask
-from datumaro.plugins.data_formats.yolo.base import YoloUltralyticsBase
-from datumaro.util import parse_json_file
-from datumaro.util.image import IMAGE_EXTENSIONS, ImageMeta
-from datumaro.util.os_util import find_files
+from importlib.resources import open_text
+from multiprocessing import get_context
+from random import Random
+from typing import List, Optional, Tuple
 
+import cv2 as cv
+import numpy as np
+import requests
 
-class RoboflowCocoBase(_CocoBase):
-    """
-    Parses Roboflow COCO annotations written in the following format:
-    https://cocodataset.org/#format-data
-    """
-
-    def __init__(
-        self,
-        path,
-        *,
-        subset: Optional[str] = None,
-        ctx: Optional[ImportContext] = None,
-    ):
-        super().__init__(
-            path,
-            task=CocoTask.instances,
-            coco_importer_type=CocoImporterType.roboflow,
-            subset=subset,
-            ctx=ctx,
-        )
-
-
-class RoboflowVocBase(VocBase):
-    def __init__(
-        self,
-        path: str,
-        *,
-        subset: Optional[str] = None,
-        ctx: Optional[ImportContext] = None,
-    ):
-        super().__init__(
-            path,
-            task=VocTask.voc_detection,
-            voc_importer_type=VocImporterType.roboflow,
-            subset=subset,
-            ctx=ctx,
-        )
-
-    def _load_categories(self, path):
-        cats = set()
-        ann_files = [file for file in os.listdir(path) if file.endswith(".xml")]
-        for ann_file in ann_files:
-            xml_file = osp.join(path, ann_file)
-
-            root = ElementTree.parse(xml_file).getroot()
+from datumaro.components.generator import DatasetGenerator
+from datumaro.util.definitions import get_datumaro_cache_dir
+from datumaro.util.image import save_image
+from datumaro.util.scope import on_error_do, on_exit_do, scope_add, scoped
 
-            if root.tag != "annotation":
-                continue
-
-            for object_elem in root.iterfind("object"):
-                cat_name = self._parse_field(object_elem, "name")
-                cats.add(cat_name)
-
-        label_categories = LabelCategories()
-        for _, cat in enumerate(sorted(cats)):
-            label_categories.add(cat)
-
-        categories = {AnnotationType.label: label_categories}
+from .utils import IFSFunction, augment, colorize, suppress_computation_warnings
 
-        return categories
 
-    def _load_subset_list(self, path):
-        return [os.path.splitext(file)[0] for file in os.listdir(path) if file.endswith(".xml")]
+class FractalImageGenerator(DatasetGenerator):
+    """
+    ImageGenerator generates 3-channel synthetic images with provided shape.
+    Uses the algorithm from the article: https://arxiv.org/abs/2103.13023
+    """
 
+    _MODEL_PROTO_FILENAME = "colorization_deploy_v2.prototxt"
+    _MODEL_WEIGHTS_FILENAME = "colorization_release_v2.caffemodel"
+    _HULL_PTS_FILE_NAME = "pts_in_hull.npy"
+    _COLORS_FILE = "background_colors.txt"
 
-class RoboflowYoloBase(YoloUltralyticsBase):
     def __init__(
         self,
-        config_path: str,
-        image_info: Union[None, str, ImageMeta] = None,
-        urls: Optional[List[str]] = None,
-        **kwargs,
+        output_dir: str,
+        count: int,
+        shape: Tuple[int, int],
+        model_path: str = get_datumaro_cache_dir(),
     ) -> None:
-        super().__init__(config_path, image_info, urls, **kwargs)
+        assert 0 < count, "Image count cannot be lesser than 1"
+        self._count = count
 
-    def _get_rootpath(self, config_path: str) -> str:
-        return osp.dirname(config_path)
+        self._output_dir = output_dir
+        self._model_dir = model_path
 
-    def _load_img_files(self, rootpath: str) -> Dict:
-        return {
-            self._get_fname(img_file): img_file
-            for img_file in find_files(rootpath, IMAGE_EXTENSIONS, recursive=True, max_depth=2)
-            if osp.split(osp.relpath(osp.dirname(img_file), rootpath))[0] == self._subset
-        }
+        self._cpu_count = min(os.cpu_count(), self._count)
 
+        assert len(shape) == 2
+        self._height, self._width = shape
+
+        self._weights = self._create_weights(IFSFunction.NUM_PARAMS)
+        self._threshold = 0.2
+        self._iterations = 200000
+        self._num_of_points = 100000
+
+        self._initialize_params()
+
+    def generate_dataset(self) -> None:
+        log.info(
+            "Generation of '%d' 3-channel images with height = '%d' and width = '%d'",
+            self._count,
+            self._height,
+            self._width,
+        )
 
-class RoboflowYoloObbBase(RoboflowYoloBase):
-    def __init__(
-        self,
-        config_path: str,
-        image_info: Union[None, str, ImageMeta] = None,
-        urls: Optional[List[str]] = None,
-        **kwargs,
-    ) -> None:
-        super().__init__(config_path, image_info, urls, **kwargs)
+        self._download_colorization_model(self._model_dir)
 
-    def _parse_annotations(
-        self,
-        anno_path: str,
-        image: ImageFromFile,
-        *,
-        label_categories: LabelCategories,
-    ) -> List[Annotation]:
-        lines = []
-        with open(anno_path, "r", encoding="utf-8") as f:
-            for line in f:
-                line = line.strip()
-                if line:
-                    lines.append(line)
-
-        annotations = []
-        for idx, line in enumerate(lines):
-            parts = line.split()
-            if len(parts) != 10:
-                raise InvalidAnnotationError(
-                    f"Unexpected field count {len(parts)} in the bbox description. "
-                    "Expected 10 fields (x1, y1, x2, y2, x3, y3, x4, y4, label, 0)."
+        mp_ctx = get_context("spawn")  # On Mac 10.15 and Python 3.7 fork leads to hangs
+        with mp_ctx.Pool(processes=self._cpu_count) as pool:
+            try:
+                params = pool.map(
+                    self._generate_category, [Random(i) for i in range(self._categories)]
                 )
-            x1, y1, x2, y2, x3, y3, x4, y4, label_name = parts[:-1]
-
-            label_name = self._parse_field(label_name, str, "bbox label name")
-            label_id = label_categories.find(label_name)[0]
+            finally:
+                pool.close()
+                pool.join()
+
+        instances_weights = np.repeat(self._weights, self._instances, axis=0)
+        weight_per_img = np.tile(instances_weights, (self._categories, 1))
+        params = np.array(params, dtype=object)
+        repeated_params = np.repeat(params, self._weights.shape[0] * self._instances, axis=0)
+        repeated_params = repeated_params[: self._count]
+        weight_per_img = weight_per_img[: self._count]
+        assert weight_per_img.shape[0] == len(repeated_params) == self._count
+
+        splits = min(self._cpu_count, self._count)
+        params_per_proc = np.array_split(repeated_params, splits)
+        weights_per_proc = np.array_split(weight_per_img, splits)
+
+        generation_params = []
+        offset = 0
+        for param, w in zip(params_per_proc, weights_per_proc):
+            indices = list(range(offset, offset + len(param)))
+            offset += len(param)
+            generation_params.append((param, w, indices))
+
+        with mp_ctx.Pool(processes=self._cpu_count) as pool:
+            try:
+                pool.starmap(self._generate_image_batch, generation_params)
+            finally:
+                pool.close()
+                pool.join()
+
+    @scoped
+    def _generate_image_batch(
+        self, params: np.ndarray, weights: np.ndarray, indices: List[int]
+    ) -> None:
+        scope_add(suppress_computation_warnings())
 
-            if label_id is None:
-                raise UndeclaredLabelError(str(label_id))
+        proto = osp.join(self._model_dir, self._MODEL_PROTO_FILENAME)
+        model = osp.join(self._model_dir, self._MODEL_WEIGHTS_FILENAME)
+        npy = osp.join(self._model_dir, self._HULL_PTS_FILE_NAME)
+        pts_in_hull = np.load(npy).transpose().reshape(2, 313, 1, 1).astype(np.float32)
+
+        with open_text(__package__, self._COLORS_FILE) as f:
+            background_colors = np.loadtxt(f)
+
+        net = cv.dnn.readNetFromCaffe(proto, model)
+        net.getLayer(net.getLayerId("class8_ab")).blobs = [pts_in_hull]
+        net.getLayer(net.getLayerId("conv8_313_rh")).blobs = [np.full([1, 313], 2.606, np.float32)]
+
+        for i, param, w in zip(indices, params, weights):
+            image = self._generate_image(
+                Random(i),
+                param,
+                self._iterations,
+                self._height,
+                self._width,
+                draw_point=False,
+                weight=w,
+            )
+            color_image = colorize(image, net)
+            aug_image = augment(Random(i), color_image, background_colors)
+            save_image(
+                osp.join(self._output_dir, "{:06d}.png".format(i)), aug_image, create_dir=True
+            )
 
-            x1 = self._parse_field(x1, float, "x1")
-            y1 = self._parse_field(y1, float, "y1")
-            x2 = self._parse_field(x2, float, "x2")
-            y2 = self._parse_field(y2, float, "y2")
-            x3 = self._parse_field(x3, float, "x3")
-            y3 = self._parse_field(y3, float, "y3")
-            x4 = self._parse_field(x4, float, "x4")
-            y4 = self._parse_field(y4, float, "y4")
-            annotations.append(
-                Polygon(
-                    points=[x1, y1, x2, y2, x3, y3, x4, y4],
-                    label=label_id,
-                    id=idx,
-                    group=idx,
-                )
+    def _generate_image(
+        self,
+        rng: Random,
+        params: np.ndarray,
+        iterations: int,
+        height: int,
+        width: int,
+        draw_point: bool = True,
+        weight: Optional[np.ndarray] = None,
+    ) -> np.ndarray:
+        ifs_function = IFSFunction(rng, prev_x=0.0, prev_y=0.0)
+        for param in params:
+            ifs_function.add_param(
+                param[: ifs_function.NUM_PARAMS], param[ifs_function.NUM_PARAMS], weight
             )
+        ifs_function.calculate(iterations)
+        img = ifs_function.draw(height, width, draw_point)
+        return img
+
+    @scoped
+    def _generate_category(self, rng: Random, base_h: int = 512, base_w: int = 512) -> np.ndarray:
+        scope_add(suppress_computation_warnings())
+
+        pixels = -1
+        i = 0
+        while pixels < self._threshold and i < self._iterations:
+            param_size = rng.randint(2, 7)
+            params = np.zeros((param_size, IFSFunction.NUM_PARAMS + 1), dtype=np.float32)
+
+            sum_proba = 1e-5
+            for p_idx in range(param_size):
+                a, b, c, d, e, f = [rng.uniform(-1.0, 1.0) for _ in range(IFSFunction.NUM_PARAMS)]
+                prob = abs(a * d - b * c)
+                sum_proba += prob
+                params[p_idx] = a, b, c, d, e, f, prob
+            params[:, IFSFunction.NUM_PARAMS] /= sum_proba
+
+            fractal_img = self._generate_image(rng, params, self._num_of_points, base_h, base_w)
+            pixels = np.count_nonzero(fractal_img) / (base_h * base_w)
+            i += 1
+        return params
+
+    def _initialize_params(self) -> None:
+        if self._count < self._weights.shape[0]:
+            self._weights = self._weights[: self._count, :]
+
+        instances_categories = np.ceil(self._count / self._weights.shape[0])
+        self._instances = np.ceil(np.sqrt(instances_categories)).astype(int)
+        self._categories = np.ceil(instances_categories / self._instances).astype(int)
 
-        return annotations
+    @staticmethod
+    def _create_weights(num_params):
+        # weights from https://openaccess.thecvf.com/content/ACCV2020/papers/Kataoka_Pre-training_without_Natural_Images_ACCV_2020_paper.pdf
+        BASE_WEIGHTS = np.ones((num_params,))
+        WEIGHT_INTERVAL = 0.4
+        INTERVAL_MULTIPLIERS = (-2, -1, 1, 2)
+        weight_vectors = [BASE_WEIGHTS]
+
+        for weight_index in range(num_params):
+            for multiplier in INTERVAL_MULTIPLIERS:
+                modified_weights = BASE_WEIGHTS.copy()
+                modified_weights[weight_index] += multiplier * WEIGHT_INTERVAL
+                weight_vectors.append(modified_weights)
+        weights = np.array(weight_vectors)
+        return weights
+
+    @classmethod
+    def _download_colorization_model(cls, save_dir: str) -> None:
+        prototxt_file_name = cls._MODEL_PROTO_FILENAME
+        caffemodel_file_name = cls._MODEL_WEIGHTS_FILENAME
+        hull_file_name = cls._HULL_PTS_FILE_NAME
+
+        proto_path = osp.join(save_dir, prototxt_file_name)
+        model_path = osp.join(save_dir, caffemodel_file_name)
+        hull_path = osp.join(save_dir, hull_file_name)
+        if not (
+            osp.exists(proto_path) and osp.exists(model_path) and osp.exists(hull_path)
+        ) and not os.access(save_dir, os.W_OK):
+            raise ValueError(
+                "Please provide a path to a colorization model directory or "
+                "a path to a writable directory to download the model"
+            )
 
+        for url, filename, size, sha512_checksum in [
+            (
+                f"https://raw.githubusercontent.com/richzhang/colorization/a1642d6ac6fc80fe08885edba34c166da09465f6/colorization/models/{prototxt_file_name}",
+                prototxt_file_name,
+                9945,
+                "e3dd9188771202bd296623510bcf527b41c130fc9bae584e61dcdf66917b8c4d147b7b838fec0685568f7f287235c34e8b8e9c0482b555774795be89f0442820",
+            ),
+            (
+                f"http://eecs.berkeley.edu/~rich.zhang/projects/2016_colorization/files/demo_v2/{caffemodel_file_name}",
+                caffemodel_file_name,
+                128946764,
+                "3d773dd83cfcf8e846e3a9722a4d302a3b7a0f95a0a7ae1a3d3ef5fe62eecd617f4f30eefb1d8d6123be4a8f29f7c6e64f07b36193f45710b549f3e4796570f1",
+            ),
+            (
+                f"https://raw.githubusercontent.com/richzhang/colorization/a1642d6ac6fc80fe08885edba34c166da09465f6/colorization/resources/{hull_file_name}",
+                hull_file_name,
+                5088,
+                "bf59a8a4e74b18948e4aeaa430f71eb8603bd9dbbce207ea086dd0fb976a34672beaeea6f1233a21687da710e0f8d36e86133a8532265dfda52994a7d6f0dbf5",
+            ),
+        ]:
+            save_path = osp.join(save_dir, filename)
+            if osp.exists(save_path):
+                continue
 
-class RoboflowCreateMlBase(SubsetBase):
-    """
-    Parses Roboflow CreateML annotations written in the following format:
-    https://cocodataset.org/#format-data
-    """
+            log.info("Downloading the '%s' file to '%s'", filename, save_dir)
+            try:
+                cls._download_file(
+                    url, save_path, expected_size=size, expected_checksum=sha512_checksum
+                )
+            except Exception as e:
+                raise Exception(f"Failed to download the '{filename}' file: {str(e)}") from e
 
-    def __init__(
-        self,
-        path,
-        *,
-        subset: Optional[str] = None,
-        ctx: Optional[ImportContext] = None,
-    ):
-        if not osp.isfile(path):
-            raise FileNotFoundError(errno.ENOENT, "Can't find JSON file", path)
-        self._path = path
-
-        if not subset:
-            subset = osp.splitext(osp.basename(path))[0]
-        super().__init__(subset=subset, ctx=ctx)
-
-        json_data = parse_json_file(path)
-        self._categories = self._load_categories(json_data)
-        self._items = self._load_items(json_data)
-
-    def _load_categories(self, json_data):
-        cats = set()
-        for anns in json_data:
-            for ann in anns["annotations"]:
-                cats.add(ann["label"])
-
-        label_categories = LabelCategories()
-        for cat in sorted(cats):
-            label_categories.add(cat)
-
-        categories = {AnnotationType.label: label_categories}
-
-        return categories
-
-    def _load_items(self, json_data):
-        items = {}
-        for anns in self._ctx.progress_reporter.iter(
-            json_data, desc=f"Parsing boxes in '{self._subset}'"
-        ):
-            annotations = []
-            for ann_id, ann in enumerate(anns["annotations"]):
-                label_id, _ = self._categories[AnnotationType.label].find(ann["label"])
-                if label_id is None:
-                    raise UndeclaredLabelError(ann["label"])
-
-                x = ann["coordinates"]["x"]
-                y = ann["coordinates"]["y"]
-                w = ann["coordinates"]["width"]
-                h = ann["coordinates"]["height"]
-                annotations.append(Bbox(x, y, w, h, label=label_id, id=ann_id, group=ann_id))
-
-            img_id = osp.splitext(anns["image"])[0]
-            items[img_id] = DatasetItem(
-                id=img_id,
-                subset=self._subset,
-                media=Image.from_file(path=osp.join(osp.dirname(self._path), anns["image"])),
-                annotations=annotations,
-            )
+    @staticmethod
+    @scoped
+    def _download_file(
+        url: str, output_path: str, *, timeout: int = 60, expected_size: int, expected_checksum: str
+    ) -> None:
+        BLOCK_SIZE = 2**20
 
-        return items.values()
+        assert not osp.exists(output_path)
 
+        tmp_path = output_path + ".tmp"
+        if osp.exists(tmp_path):
+            raise Exception(f"Can't write temporary file '{tmp_path}' - file exists")
 
-class RoboflowMulticlassBase(SubsetBase):
-    """
-    Parses Roboflow Multiclass annotations written in the following format:
-    https://cocodataset.org/#format-data
-    """
+        response = requests.get(url, timeout=timeout, stream=True)
+        on_exit_do(response.close)
 
-    def __init__(
-        self,
-        path,
-        *,
-        subset: Optional[str] = None,
-        ctx: Optional[ImportContext] = None,
-    ):
-        if not osp.isfile(path):
-            raise FileNotFoundError(errno.ENOENT, "Can't find CSV file", path)
-        self._path = path
-
-        if not subset:
-            subset = osp.splitext(osp.basename(path))[0]
-        super().__init__(subset=subset, ctx=ctx)
-
-        self._label_mapping = {}
-        self._categories = self._load_categories(path)
-        self._items = self._load_items(path)
-
-    def _load_categories(self, path):
-        with open(path, "r", encoding="utf-8") as f:
-            reader = csv.DictReader(f)
-            cats = [label.strip() for label in reader.fieldnames[1:]]
-
-        label_categories = LabelCategories()
-        for idx, cat in enumerate(sorted(cats)):
-            label_categories.add(cat)
-            self._label_mapping[cat] = idx
-
-        categories = {AnnotationType.label: label_categories}
-
-        return categories
-
-    def _load_items(self, path):
-        items = []
-        with open(path, "r", encoding="utf-8") as f:
-            for anns in csv.DictReader(f):
-                img_id = anns.get("filename", None)
-                img_id = osp.splitext(img_id)[0] if img_id else None
-                idx = 0
-                annotations = []
-                for key, val in anns.items():
-                    if key.strip() not in self._label_mapping:
-                        continue
-                    if int(val) == 1:
-                        annotations.append(
-                            Label(label=self._label_mapping[key.strip()], id=idx, group=idx)
-                        )
-                        idx += 1
-
-                items.append(
-                    DatasetItem(
-                        id=img_id,
-                        subset=self._subset,
-                        media=Image.from_file(
-                            path=osp.join(osp.dirname(self._path), anns["filename"])
-                        ),
-                        annotations=annotations,
-                    )
-                )
+        response.raise_for_status()
 
-        return items
+        checksum_counter = hashlib.sha512()
+        actual_size = 0
 
+        with open(tmp_path, "wb") as fd:
+            on_error_do(os.unlink, tmp_path)
 
-class RoboflowTfrecord(TfDetectionApiBase):
-    def __init__(
-        self,
-        path: str,
-        *,
-        subset: Optional[str] = None,
-        ctx: Optional[ImportContext] = None,
-    ):
-        super().__init__(
-            path=path, subset=subset, tfrecord_importer_type=TfrecordImporterType.roboflow, ctx=ctx
-        )
+            for chunk in response.iter_content(chunk_size=BLOCK_SIZE):
+                actual_size += len(chunk)
+                if actual_size > expected_size:
+                    # There is also the context-length header, but it can be corrupted or invalid
+                    # for different reasons
+                    raise Exception(
+                        f"The downloaded file has unexpected size, expected {expected_size}."
+                    )
 
-    @staticmethod
-    def _parse_labelmap(text):
-        entry_pattern = r'name:\s*"([^"]+)"\s*,\s*id:\s*(\d+)'
-        entry_pattern = re.compile(entry_pattern)
+                checksum_counter.update(chunk)
 
-        matches = re.findall(entry_pattern, text)
+                fd.write(chunk)
 
-        labelmap = {name: int(id) for name, id in matches}
+        actual_checksum = checksum_counter.hexdigest()
+        if actual_checksum.lower() != expected_checksum.lower():
+            raise Exception("The downloaded file has unexpected checksum")
 
-        return labelmap
+        os.rename(tmp_path, output_path)
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/roboflow/importer.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/roboflow/importer.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,22 @@
 # SPDX-License-Identifier: MIT
 
 import os
 import os.path as osp
 from collections import defaultdict
 from glob import glob
 from io import TextIOWrapper
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Type
 from xml.etree import ElementTree
 
 from datumaro.components.errors import DatasetImportError
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import Importer
 from datumaro.components.lazy_plugin import extra_deps
+from datumaro.components.merge.extractor_merger import ExtractorMerger
 
 
 class RoboflowCocoImporter(Importer):
     FORMAT = "roboflow_coco"
     ANN_FILE_NAME = "_annotations.coco.json"
 
     @classmethod
@@ -37,14 +38,21 @@
             subset_name = osp.basename(osp.dirname(subset_path))
             sources.append(
                 {"url": subset_path, "format": cls.FORMAT, "options": {"subset": subset_name}}
             )
 
         return sources
 
+    @property
+    def can_stream(self) -> bool:
+        return True
+
+    def get_extractor_merger(self) -> Type[ExtractorMerger]:
+        return ExtractorMerger
+
 
 class RoboflowVocImporter(Importer):
     FORMAT = "roboflow_voc"
     FORMAT_EXT = ".xml"
     ANN_DIR_NAME = ""
 
     @classmethod
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/exporter.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/segment_anything/importer.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/segment_anything/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/sly_pointcloud/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/sly_pointcloud/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/sly_pointcloud/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/format.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/synthia/importer.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/synthia/importer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/tf_detection_api/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/tf_detection_api/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/tf_detection_api/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/vgg_face2.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/vgg_face2.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/video.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/video.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -151,15 +151,15 @@
             images = {}
 
         annotations = (
             self._parse_labels() if self._task in [VocTask.voc, VocTask.voc_classification] else {}
         )
 
         for item_id in self._ctx.progress_reporter.iter(
-            self._items, desc=f"Parsing boxes in '{self._subset}'"
+            self._items, desc=f"Importing '{self._subset}'"
         ):
             log.debug("Reading item '%s'" % item_id)
             size = None
 
             try:
                 anns = annotations.get(item_id, [])
                 image = None
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/exporter.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/format.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/voc/importer.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/voc/importer.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 # Copyright (C) 2019-2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 from typing import Optional, Type
 
-from datumaro.components.dataset_base import ExtractorMerger
 from datumaro.components.format_detection import FormatDetectionContext
 from datumaro.components.importer import Importer
+from datumaro.components.merge.extractor_merger import ExtractorMerger
 
 from .format import VocPath, VocTask
 
 
 class _VocImporter(Importer):
     _TASKS = {
         VocTask.voc: ("voc", "Main"),
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/vott_csv.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/vott_csv.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/vott_json.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/vott_json.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/widerface.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/widerface.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -281,15 +281,15 @@
 
         return label_categories
 
     def __iter__(self) -> Iterator[DatasetItem]:
         subsets = self._subsets
         pbars = self._ctx.progress_reporter.split(len(subsets))
         for pbar, (subset_name, subset) in zip(pbars, subsets.items()):
-            for item in pbar.iter(subset, desc=f"Parsing '{subset_name}'"):
+            for item in pbar.iter(subset, desc=f"Importing '{subset_name}'"):
                 yield item
 
     def __len__(self):
         return sum(len(s) for s in self._subsets.values())
 
     def get_subset(self, name):
         return self._subsets[name]
@@ -328,15 +328,16 @@
         self._img_files = self._load_img_files(rootpath)
 
     def __iter__(self) -> Iterator[DatasetItem]:
         label_categories = self._categories.get(AnnotationType.label)
         if label_categories is None:
             raise DatasetImportError("label_categories should be not None.")
 
-        for url in self._urls:
+        pbar = self._ctx.progress_reporter
+        for url in pbar.iter(self._urls, desc=f"Importing '{self._subset}'"):
             try:
                 fname = self._get_fname(url)
                 img = Image.from_file(path=self._img_files[fname])
                 anns = self._parse_annotations(
                     url,
                     img,
                     label_categories=label_categories,
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/exporter.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/exporter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/format.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/format.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/data_formats/yolo/importer.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/data_formats/yolo/importer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 # SPDX-License-Identifier: MIT
 
 import os.path as osp
 from collections import defaultdict
 from io import TextIOWrapper
 from typing import Any, Dict, List, Optional, Type
 
-from datumaro.components.dataset_base import ExtractorMerger
 from datumaro.components.errors import DatasetImportError
 from datumaro.components.format_detection import FormatDetectionConfidence, FormatDetectionContext
 from datumaro.components.importer import Importer
+from datumaro.components.merge.extractor_merger import ExtractorMerger
 from datumaro.util.os_util import extract_subset_name_from_parent
 
 from .format import YoloFormatType, YoloLoosePath, YoloPath, YoloUltralyticsPath
 
 
 class _YoloStrictImporter(Importer):
     @classmethod
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/explorer.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/explorer.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/base.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/base.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/ovms.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/ovms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/samples/face_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/inference_server_plugin/triton.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/inference_server_plugin/triton.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/missing_annotation_detection.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/missing_annotation_detection.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/ndr.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/ndr.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/launcher.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/clip_text_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/clip_visual_ViT-B_32_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/coco.class` & `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/coco.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/googlenet-v4-tf_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/imagenet.class` & `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/imagenet.class`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/mobilenet_v2_pytorch_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_atss_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_gen3_ssd_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/otx_custom_object_detection_yolox_interp.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/samples/utils.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/samples/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/openvino_plugin/shift_launcher.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/openvino_plugin/shift_launcher.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/sampler/algorithm/algorithm.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/sampler/algorithm/algorithm.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/sampler/algorithm/entropy.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/sampler/algorithm/entropy.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/sampler/random_sampler.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/sampler/random_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/sampler/relevancy_sampler.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/sampler/relevancy_sampler.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/specs.json` & `datumaro-1.4.0rc3/src/datumaro/plugins/specs.json`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/specs.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/specs.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/splitter.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/splitter.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/synthetic_data/background_colors.txt` & `datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/background_colors.txt`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/synthetic_data/utils.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/synthetic_data/utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/tiling/merge_tile.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/tiling/merge_tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/tiling/tile.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/tiling/tile.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/tiling/util.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/tiling/util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/transforms.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/transforms.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/plugins/validators.py` & `datumaro-1.4.0rc3/src/datumaro/plugins/validators.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/__init__.py` & `datumaro-1.4.0rc3/src/datumaro/util/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # Copyright (C) 2019-2022 Intel Corporation
 #
 # SPDX-License-Identifier: MIT
 
 from functools import wraps
 from inspect import isclass
 from itertools import islice
-from typing import Any, Iterable, Optional, Tuple, Union
+from typing import Any, Dict, Iterable, Tuple, Union
 
 import attrs
 import orjson
+from json_stream.base import StreamingJSONList, StreamingJSONObject
 
 NOTSET = object()
 
 str_to_bool = attrs.converters.to_bool
 
 
 def find(iterable, pred=lambda x: True, default=None):
@@ -189,7 +190,15 @@
                 data,
                 sort_keys=sort_keys,
                 allow_numpy=allow_numpy,
                 indent=indent,
                 append_newline=append_newline,
             )
         )
+
+
+def to_dict_from_streaming_json(obj: Any) -> Dict[str, Any]:
+    if isinstance(obj, StreamingJSONObject):
+        return {k: to_dict_from_streaming_json(v) for k, v in obj.items()}
+    if isinstance(obj, StreamingJSONList):
+        return [to_dict_from_streaming_json(v) for v in obj]
+    return obj
```

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/annotation_util.py` & `datumaro-1.4.0rc3/src/datumaro/util/annotation_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/attrs_util.py` & `datumaro-1.4.0rc3/src/datumaro/util/attrs_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/definitions.py` & `datumaro-1.4.0rc3/src/datumaro/util/definitions.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/file_utils.py` & `datumaro-1.4.0rc3/src/datumaro/util/file_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/image.py` & `datumaro-1.4.0rc3/src/datumaro/util/image.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/image_cache.py` & `datumaro-1.4.0rc3/src/datumaro/util/image_cache.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/log_utils.py` & `datumaro-1.4.0rc3/src/datumaro/util/log_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/mask_tools.py` & `datumaro-1.4.0rc3/src/datumaro/util/mask_tools.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/meta_file_util.py` & `datumaro-1.4.0rc3/src/datumaro/util/meta_file_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/os_util.py` & `datumaro-1.4.0rc3/src/datumaro/util/os_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/pickle_util.py` & `datumaro-1.4.0rc3/src/datumaro/util/pickle_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/scope.py` & `datumaro-1.4.0rc3/src/datumaro/util/scope.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/telemetry_stub.py` & `datumaro-1.4.0rc3/src/datumaro/util/telemetry_stub.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/telemetry_utils.py` & `datumaro-1.4.0rc3/src/datumaro/util/telemetry_utils.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro/util/tf_util.py` & `datumaro-1.4.0rc3/src/datumaro/util/tf_util.py`

 * *Files identical despite different names*

### Comparing `datumaro-1.4.0rc2/src/datumaro.egg-info/PKG-INFO` & `datumaro-1.4.0rc3/src/datumaro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datumaro
-Version: 1.4.0rc2
+Version: 1.4.0rc3
 Summary: Dataset Management Framework (Datumaro)
 Home-page: https://github.com/openvinotoolkit/datumaro
 Author: Intel
 Author-email: emily.chun@intel.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `datumaro-1.4.0rc2/src/datumaro.egg-info/SOURCES.txt` & `datumaro-1.4.0rc3/src/datumaro.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -101,18 +101,21 @@
 src/datumaro/components/algorithms/hash_key_inference/hashkey_util.py
 src/datumaro/components/algorithms/hash_key_inference/prune.py
 src/datumaro/components/algorithms/noisy_label_detection/__init__.py
 src/datumaro/components/algorithms/noisy_label_detection/loss_dynamics_analyzer.py
 src/datumaro/components/annotations/__init__.py
 src/datumaro/components/annotations/matcher.py
 src/datumaro/components/annotations/merger.py
+src/datumaro/components/contexts/__init__.py
+src/datumaro/components/contexts/importer.py
 src/datumaro/components/hl_ops/__init__.py
 src/datumaro/components/merge/__init__.py
 src/datumaro/components/merge/base.py
 src/datumaro/components/merge/exact_merge.py
+src/datumaro/components/merge/extractor_merger.py
 src/datumaro/components/merge/intersect_merge.py
 src/datumaro/components/merge/union_merge.py
 src/datumaro/plugins/__init__.py
 src/datumaro/plugins/explorer.py
 src/datumaro/plugins/missing_annotation_detection.py
 src/datumaro/plugins/ndr.py
 src/datumaro/plugins/specs.json
@@ -170,16 +173,18 @@
 src/datumaro/plugins/data_formats/ava/ava_label_pb2.py
 src/datumaro/plugins/data_formats/celeba/__init__.py
 src/datumaro/plugins/data_formats/celeba/align_celeba.py
 src/datumaro/plugins/data_formats/celeba/celeba.py
 src/datumaro/plugins/data_formats/coco/__init__.py
 src/datumaro/plugins/data_formats/coco/base.py
 src/datumaro/plugins/data_formats/coco/exporter.py
+src/datumaro/plugins/data_formats/coco/extractor_merger.py
 src/datumaro/plugins/data_formats/coco/format.py
 src/datumaro/plugins/data_formats/coco/importer.py
+src/datumaro/plugins/data_formats/coco/page_mapper.py
 src/datumaro/plugins/data_formats/cvat/__init__.py
 src/datumaro/plugins/data_formats/cvat/base.py
 src/datumaro/plugins/data_formats/cvat/exporter.py
 src/datumaro/plugins/data_formats/cvat/format.py
 src/datumaro/plugins/data_formats/datumaro/__init__.py
 src/datumaro/plugins/data_formats/datumaro/base.py
 src/datumaro/plugins/data_formats/datumaro/exporter.py
```

### Comparing `datumaro-1.4.0rc2/src/datumaro.egg-info/requires.txt` & `datumaro-1.4.0rc3/src/datumaro.egg-info/requires.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 pyemd
 pyarrow
 protobuf<4
 tabulate
 ovmsclient
 tritonclient[all]
 scikit-learn
+json-stream
 opencv-python
 
 [:platform_system != "Windows" or python_version >= "3.9"]
 pycocotools>=2.0.4
 
 [:platform_system == "Windows" and python_version < "3.9"]
 pycocotools-windows
```

