# Comparing `tmp/xautoml-0.1.1.tar.gz` & `tmp/xautoml-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xautoml-0.1.1.tar", last modified: Tue Mar  1 13:15:03 2022, max compression
+gzip compressed data, was "xautoml-0.1.2.tar", last modified: Fri Apr  8 06:30:39 2022, max compression
```

## Comparing `xautoml-0.1.1.tar` & `xautoml-0.1.2.tar`

### file list

```diff
@@ -1,202 +1,202 @@
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.504152 xautoml-0.1.1/
--rw-rw-r--   0 marc      (1000) marc      (1000)     1512 2021-05-28 09:36:11.000000 xautoml-0.1.1/LICENSE
--rw-rw-r--   0 marc      (1000) marc      (1000)      429 2021-05-28 09:36:08.000000 xautoml-0.1.1/MANIFEST.in
--rw-rw-r--   0 marc      (1000) marc      (1000)     5762 2022-03-01 13:15:03.504152 xautoml-0.1.1/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1000)     4987 2022-03-01 13:14:26.000000 xautoml-0.1.1/README.md
--rw-rw-r--   0 marc      (1000) marc      (1000)      175 2021-05-28 09:31:04.000000 xautoml-0.1.1/install.json
--rw-rw-r--   0 marc      (1000) marc      (1000)     3428 2022-03-01 13:07:41.000000 xautoml-0.1.1/package.json
--rw-rw-r--   0 marc      (1000) marc      (1000)      563 2021-05-28 09:36:04.000000 xautoml-0.1.1/pyproject.toml
--rw-rw-r--   0 marc      (1000) marc      (1000)       38 2022-03-01 13:15:03.504152 xautoml-0.1.1/setup.cfg
--rw-rw-r--   0 marc      (1000) marc      (1000)     2477 2022-03-01 08:58:04.000000 xautoml-0.1.1/setup.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.460152 xautoml-0.1.1/src/
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.460152 xautoml-0.1.1/src/components/
--rw-rw-r--   0 marc      (1000) marc      (1000)     5184 2022-03-01 12:50:19.000000 xautoml-0.1.1/src/components/candidate_inspections.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     4814 2022-02-01 20:14:40.000000 xautoml-0.1.1/src/components/comparison.tsx
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.464152 xautoml-0.1.1/src/components/details/
--rw-rw-r--   0 marc      (1000) marc      (1000)     7318 2022-02-08 17:50:52.000000 xautoml-0.1.1/src/components/details/configuration.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     1726 2022-01-05 21:30:41.000000 xautoml-0.1.1/src/components/details/confusion_matrix.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     2211 2022-02-01 20:14:40.000000 xautoml-0.1.1/src/components/details/dataset_table.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)    14840 2022-02-08 15:11:02.000000 xautoml-0.1.1/src/components/details/feature_importance.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     9279 2022-02-08 15:11:02.000000 xautoml-0.1.1/src/components/details/global_surrogate.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)    15789 2022-02-08 15:11:02.000000 xautoml-0.1.1/src/components/details/hp_importance.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)    14217 2022-02-01 20:14:40.000000 xautoml-0.1.1/src/components/details/local_surrogate.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)      514 2022-03-01 12:50:24.000000 xautoml-0.1.1/src/components/details/model.ts
--rw-rw-r--   0 marc      (1000) marc      (1000)     7875 2022-02-08 19:56:05.000000 xautoml-0.1.1/src/components/details/performance_details.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     3306 2022-02-01 20:14:40.000000 xautoml-0.1.1/src/components/details/pipeline_hyperparameters.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     6038 2022-03-01 12:58:10.000000 xautoml-0.1.1/src/components/details/pipeline_visualization.tsx
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.464152 xautoml-0.1.1/src/components/ensemble/
--rw-rw-r--   0 marc      (1000) marc      (1000)     2800 2022-01-13 18:11:39.000000 xautoml-0.1.1/src/components/ensemble/decision_surface.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     2939 2022-02-02 15:32:38.000000 xautoml-0.1.1/src/components/ensemble/ensemble_details.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     5973 2022-01-22 18:08:58.000000 xautoml-0.1.1/src/components/ensemble/ensemble_table.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     8156 2022-02-01 20:14:40.000000 xautoml-0.1.1/src/components/ensemble.tsx
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.464152 xautoml-0.1.1/src/components/general/
--rw-rw-r--   0 marc      (1000) marc      (1000)     2567 2022-01-22 20:17:53.000000 xautoml-0.1.1/src/components/general/meta_information.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     1639 2022-01-19 21:29:50.000000 xautoml-0.1.1/src/components/general/performance_distribution.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     4877 2022-01-14 11:47:47.000000 xautoml-0.1.1/src/components/general/performance_timeline.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     5692 2022-01-20 22:42:45.000000 xautoml-0.1.1/src/components/general/roc_curve.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)    20551 2022-03-01 13:05:12.000000 xautoml-0.1.1/src/components/leaderboard.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     3490 2022-02-01 20:14:40.000000 xautoml-0.1.1/src/components/optimization_overview.tsx
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.464152 xautoml-0.1.1/src/components/pc/
--rw-rw-r--   0 marc      (1000) marc      (1000)     4953 2021-12-17 15:06:43.000000 xautoml-0.1.1/src/components/pc/brush.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)      171 2021-12-24 09:48:18.000000 xautoml-0.1.1/src/components/pc/constants.ts
--rw-rw-r--   0 marc      (1000) marc      (1000)     9797 2022-02-03 08:55:01.000000 xautoml-0.1.1/src/components/pc/model.ts
--rw-rw-r--   0 marc      (1000) marc      (1000)    12074 2022-02-03 13:47:43.000000 xautoml-0.1.1/src/components/pc/parallel_corrdinates.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     9515 2022-02-01 15:06:40.000000 xautoml-0.1.1/src/components/pc/pc_axis.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     3439 2022-02-01 20:14:40.000000 xautoml-0.1.1/src/components/pc/pc_choice.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     6026 2022-02-03 10:01:38.000000 xautoml-0.1.1/src/components/pc/pc_line.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     8971 2022-02-08 18:38:08.000000 xautoml-0.1.1/src/components/pc/util.ts
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.464152 xautoml-0.1.1/src/components/search_space/
--rw-rw-r--   0 marc      (1000) marc      (1000)      396 2021-12-24 09:48:18.000000 xautoml-0.1.1/src/components/search_space/model.ts
--rw-rw-r--   0 marc      (1000) marc      (1000)    10263 2022-02-04 16:06:03.000000 xautoml-0.1.1/src/components/search_space/optimization_progress.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     9975 2022-02-04 14:19:32.000000 xautoml-0.1.1/src/components/search_space/sampling_history.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     7347 2022-02-01 20:14:40.000000 xautoml-0.1.1/src/components/search_space/structure_search_graph.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)    11048 2022-02-04 17:47:59.000000 xautoml-0.1.1/src/components/search_space.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     3833 2022-02-01 20:14:40.000000 xautoml-0.1.1/src/dao.ts
--rw-rw-r--   0 marc      (1000) marc      (1000)     1610 2021-12-24 09:57:35.000000 xautoml-0.1.1/src/index.ts
--rw-rw-r--   0 marc      (1000) marc      (1000)    11368 2022-02-08 15:11:02.000000 xautoml-0.1.1/src/jupyter.ts
--rw-rw-r--   0 marc      (1000) marc      (1000)    13946 2022-03-01 13:02:12.000000 xautoml-0.1.1/src/model.ts
--rw-rw-r--   0 marc      (1000) marc      (1000)     9742 2022-02-01 20:14:40.000000 xautoml-0.1.1/src/root.tsx
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.468152 xautoml-0.1.1/src/util/
--rw-rw-r--   0 marc      (1000) marc      (1000)     1109 2022-01-06 12:45:23.000000 xautoml-0.1.1/src/util/KeyValue.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     3467 2022-01-12 09:07:37.000000 xautoml-0.1.1/src/util/collapse.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)      897 2021-12-28 20:09:48.000000 xautoml-0.1.1/src/util/error.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     2561 2021-12-25 17:52:58.000000 xautoml-0.1.1/src/util/flexible-svg.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)      433 2022-01-05 17:08:46.000000 xautoml-0.1.1/src/util/heading.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     1068 2022-01-06 10:28:34.000000 xautoml-0.1.1/src/util/help.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     5692 2022-02-01 20:14:40.000000 xautoml-0.1.1/src/util/importance_overview.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)      702 2022-01-07 16:27:26.000000 xautoml-0.1.1/src/util/jupyter-button.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     1234 2022-01-06 14:00:55.000000 xautoml-0.1.1/src/util/layout.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)      329 2021-12-24 09:48:18.000000 xautoml-0.1.1/src/util/loading.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     4020 2022-02-08 15:11:02.000000 xautoml-0.1.1/src/util/raw_dataset.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     2614 2022-01-10 12:42:54.000000 xautoml-0.1.1/src/util/recharts.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)      884 2021-12-08 12:44:37.000000 xautoml-0.1.1/src/util/tabpanel.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     8199 2022-02-01 20:14:40.000000 xautoml-0.1.1/src/util/tree_structure.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     1345 2021-12-28 20:09:48.000000 xautoml-0.1.1/src/util/warning.tsx
--rw-rw-r--   0 marc      (1000) marc      (1000)     3133 2022-02-08 18:12:32.000000 xautoml-0.1.1/src/util.ts
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.468152 xautoml-0.1.1/style/
--rw-rw-r--   0 marc      (1000) marc      (1000)    10686 2022-02-08 19:54:16.000000 xautoml-0.1.1/style/base.css
--rw-rw-r--   0 marc      (1000) marc      (1000)       25 2021-10-16 11:19:09.000000 xautoml-0.1.1/style/index.css
--rw-rw-r--   0 marc      (1000) marc      (1000)       21 2021-05-26 19:13:54.000000 xautoml-0.1.1/style/index.js
--rw-rw-r--   0 marc      (1000) marc      (1000)     4621 2021-09-25 14:21:23.000000 xautoml-0.1.1/style/jupyter.svg
--rw-rw-r--   0 marc      (1000) marc      (1000)      594 2021-11-24 18:54:00.000000 xautoml-0.1.1/tsconfig.json
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.468152 xautoml-0.1.1/xautoml/
--rw-rw-r--   0 marc      (1000) marc      (1000)      824 2021-05-28 11:28:31.000000 xautoml-0.1.1/xautoml/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      395 2022-02-01 20:14:40.000000 xautoml-0.1.1/xautoml/_helper.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      441 2021-05-28 11:28:27.000000 xautoml-0.1.1/xautoml/_version.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    23431 2022-03-01 08:23:00.000000 xautoml-0.1.1/xautoml/adapter.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4918 2022-03-01 08:20:08.000000 xautoml-0.1.1/xautoml/config_similarity.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4180 2022-03-01 08:20:08.000000 xautoml-0.1.1/xautoml/ensemble.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1085 2022-01-24 11:01:42.000000 xautoml-0.1.1/xautoml/fake.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     8372 2022-03-01 08:20:08.000000 xautoml-0.1.1/xautoml/graph_similarity.py
--rw-rw-r--   0 marc      (1000) marc      (1000)       38 2022-03-01 08:48:29.000000 xautoml-0.1.1/xautoml/handlers.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     8128 2022-03-01 08:25:03.000000 xautoml-0.1.1/xautoml/hp_importance.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.468152 xautoml-0.1.1/xautoml/labextension/
--rw-rw-r--   0 marc      (1000) marc      (1000)    20438 2022-03-01 12:53:37.000000 xautoml-0.1.1/xautoml/labextension/build_log.json
--rw-rw-r--   0 marc      (1000) marc      (1000)     3570 2022-03-01 13:05:27.000000 xautoml-0.1.1/xautoml/labextension/package.json
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.504152 xautoml-0.1.1/xautoml/labextension/static/
--rw-rw-r--   0 marc      (1000) marc      (1000)   412454 2022-03-01 13:04:34.000000 xautoml-0.1.1/xautoml/labextension/static/lib_index_js.501b1a62f9c38ddd812b.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   341796 2022-03-01 13:04:34.000000 xautoml-0.1.1/xautoml/labextension/static/lib_index_js.501b1a62f9c38ddd812b.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)   412522 2022-03-01 13:05:27.000000 xautoml-0.1.1/xautoml/labextension/static/lib_index_js.502fd3a9cc6c92d6f591.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   341870 2022-03-01 13:05:27.000000 xautoml-0.1.1/xautoml/labextension/static/lib_index_js.502fd3a9cc6c92d6f591.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)   412308 2022-03-01 12:58:19.000000 xautoml-0.1.1/xautoml/labextension/static/lib_index_js.5fe887d7b7a8ac72fc36.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   341638 2022-03-01 12:58:19.000000 xautoml-0.1.1/xautoml/labextension/static/lib_index_js.5fe887d7b7a8ac72fc36.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)   412270 2022-03-01 12:56:15.000000 xautoml-0.1.1/xautoml/labextension/static/lib_index_js.8f01bcbb99c2065d2192.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   341600 2022-03-01 12:56:15.000000 xautoml-0.1.1/xautoml/labextension/static/lib_index_js.8f01bcbb99c2065d2192.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)   412312 2022-03-01 13:02:20.000000 xautoml-0.1.1/xautoml/labextension/static/lib_index_js.9b5313ccecf3b93fdb20.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   341642 2022-03-01 13:02:20.000000 xautoml-0.1.1/xautoml/labextension/static/lib_index_js.9b5313ccecf3b93fdb20.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)   412102 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/lib_index_js.db69110a493cf4705cb0.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   341399 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/lib_index_js.db69110a493cf4705cb0.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)    27461 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-36f31a.9e464fbf6e3483c2e9ab.js
--rw-rw-r--   0 marc      (1000) marc      (1000)    18346 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-36f31a.9e464fbf6e3483c2e9ab.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)     5627 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-7f3338.56735e5382d181d596df.js
--rw-rw-r--   0 marc      (1000) marc      (1000)     3051 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-7f3338.56735e5382d181d596df.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)      810 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/node_modules_babel_runtime_helpers_interopRequireDefault_js.c535f40556b43a78ad4c.js
--rw-rw-r--   0 marc      (1000) marc      (1000)      563 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/node_modules_babel_runtime_helpers_interopRequireDefault_js.c535f40556b43a78ad4c.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)      779 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/node_modules_d3-dag_bundle_sync_recursive.f14d00bf0acbaccd2b37.js
--rw-rw-r--   0 marc      (1000) marc      (1000)      619 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/node_modules_d3-dag_bundle_sync_recursive.f14d00bf0acbaccd2b37.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)     1920 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/node_modules_d3-ease_src_exp_js.4a5f97bc213ba7d52fa3.js
--rw-rw-r--   0 marc      (1000) marc      (1000)      821 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/node_modules_d3-ease_src_exp_js.4a5f97bc213ba7d52fa3.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)     2115 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/node_modules_memoize-one_dist_memoize-one_esm_js.1ff743ff2d8d6c8c51e6.js
--rw-rw-r--   0 marc      (1000) marc      (1000)     1948 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/node_modules_memoize-one_dist_memoize-one_esm_js.1ff743ff2d8d6c8c51e6.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)    44574 2022-03-01 13:02:20.000000 xautoml-0.1.1/xautoml/labextension/static/remoteEntry.216da5d12a1be0bf8d83.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)    44574 2022-03-01 13:04:34.000000 xautoml-0.1.1/xautoml/labextension/static/remoteEntry.24d1f891ac5575800434.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)    44574 2022-03-01 12:56:15.000000 xautoml-0.1.1/xautoml/labextension/static/remoteEntry.2f372dc7f1b00fdccb53.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)    44574 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/remoteEntry.829185034e32a3a0ea99.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)    45613 2022-03-01 13:05:27.000000 xautoml-0.1.1/xautoml/labextension/static/remoteEntry.96873ac07d1a8f07b25c.js
--rw-rw-r--   0 marc      (1000) marc      (1000)    44574 2022-03-01 13:05:27.000000 xautoml-0.1.1/xautoml/labextension/static/remoteEntry.96873ac07d1a8f07b25c.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)    44574 2022-03-01 12:58:19.000000 xautoml-0.1.1/xautoml/labextension/static/remoteEntry.f13baef9edaeb761b135.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)      151 2022-03-01 12:53:37.000000 xautoml-0.1.1/xautoml/labextension/static/style.js
--rw-rw-r--   0 marc      (1000) marc      (1000)    33221 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/style_index_css.c8843f86800ceb459e3d.js
--rw-rw-r--   0 marc      (1000) marc      (1000)    38690 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/style_index_css.c8843f86800ceb459e3d.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)    95169 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_classnames_index_js-node_modules_lodash_isEqual_js.75587459728afe6cc748.js
--rw-rw-r--   0 marc      (1000) marc      (1000)    89308 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_classnames_index_js-node_modules_lodash_isEqual_js.75587459728afe6cc748.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)    12044 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f71148bf061d5119bdad.js
--rw-rw-r--   0 marc      (1000) marc      (1000)    13769 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f71148bf061d5119bdad.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)    88354 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_d3-dag_bundle_d3-dag_esm_min_js.09cb9ecb1b6911f66720.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   106927 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_d3-dag_bundle_d3-dag_esm_min_js.09cb9ecb1b6911f66720.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)   248572 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_d3-scale_src_index_js-node_modules_d3-shape_src_area_js-node_modules_d3--caf5af.db0372ffdf6a4441784e.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   177546 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_d3-scale_src_index_js-node_modules_d3-shape_src_area_js-node_modules_d3--caf5af.db0372ffdf6a4441784e.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)  1031361 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_d3_index_js.4d45a37894f902446937.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   630198 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_d3_index_js.4d45a37894f902446937.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)   242440 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Avatar_Avatar_js-node_modules_material-ui_core_esm_-413d96.0cc4c1464fc16245b4ec.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   239897 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Avatar_Avatar_js-node_modules_material-ui_core_esm_-413d96.0cc4c1464fc16245b4ec.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)   374039 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Checkbox_Checkbox_js-node_modules_material-ui_core_-da75eb.bffdd92e736ff98f4579.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   308632 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Checkbox_Checkbox_js-node_modules_material-ui_core_-da75eb.bffdd92e736ff98f4579.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)   186119 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Collapse_Collapse_js-node_modules_material-ui_core_-4fe852.d1bd5e3ec3e641a02387.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   157738 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Collapse_Collapse_js-node_modules_material-ui_core_-4fe852.d1bd5e3ec3e641a02387.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)   927241 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_index_js.269833f9d86c68103a29.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   697911 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_index_js.269833f9d86c68103a29.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)   285008 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_utils_createSvgIcon_js.1ce7f7dd7d79522653b3.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   255194 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_utils_createSvgIcon_js.1ce7f7dd7d79522653b3.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)    33774 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_icons_KeyboardArrowDown_js-node_modules_material-ui_icons_Ke-8370f2.5cd0e830e24ed213a793.js
--rw-rw-r--   0 marc      (1000) marc      (1000)    34078 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_icons_KeyboardArrowDown_js-node_modules_material-ui_icons_Ke-8370f2.5cd0e830e24ed213a793.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000) 10656879 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_icons_esm_index_js.5ae151e2203f82f49908.js
--rw-rw-r--   0 marc      (1000) marc      (1000)  4122062 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_icons_esm_index_js.5ae151e2203f82f49908.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)   357516 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_lab_esm_index_js.74baedfea25f6e14abea.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   299780 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_lab_esm_index_js.74baedfea25f6e14abea.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)   101497 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_memoizee_index_js.351b5bbf5ccfe187a70f.js
--rw-rw-r--   0 marc      (1000) marc      (1000)    96692 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_memoizee_index_js.351b5bbf5ccfe187a70f.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)    39437 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_prop-types_index_js.76920d8992c01aa3732c.js
--rw-rw-r--   0 marc      (1000) marc      (1000)    44590 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_prop-types_index_js.76920d8992c01aa3732c.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)   344730 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_rc-slider_es_index_js.d87b5e830387c5756f0e.js
--rw-rw-r--   0 marc      (1000) marc      (1000)   296601 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_rc-slider_es_index_js.d87b5e830387c5756f0e.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)    50447 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_react-move_es_index_js.6461e26c4e5974c983b7.js
--rw-rw-r--   0 marc      (1000) marc      (1000)    39783 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_react-move_es_index_js.6461e26c4e5974c983b7.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)  1485433 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_recharts_es6_index_js.12271722fd3fb37e484e.js
--rw-rw-r--   0 marc      (1000) marc      (1000)  1485617 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_recharts_es6_index_js.12271722fd3fb37e484e.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)    34648 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_resize-observer-polyfill_dist_ResizeObserver_es_js.1bbb13fa0f5d7ffa66ca.js
--rw-rw-r--   0 marc      (1000) marc      (1000)    41579 2022-03-01 12:53:48.000000 xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_resize-observer-polyfill_dist_ResizeObserver_es_js.1bbb13fa0f5d7ffa66ca.js.map
--rw-rw-r--   0 marc      (1000) marc      (1000)    21430 2022-03-01 09:41:19.000000 xautoml-0.1.1/xautoml/main.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    11105 2022-03-01 08:51:46.000000 xautoml-0.1.1/xautoml/model_details.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     4307 2022-03-01 08:20:08.000000 xautoml-0.1.1/xautoml/models.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2957 2022-03-01 08:56:00.000000 xautoml-0.1.1/xautoml/output.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     6097 2022-03-01 08:45:09.000000 xautoml-0.1.1/xautoml/roc_auc.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.504152 xautoml-0.1.1/xautoml/tests/
--rw-rw-r--   0 marc      (1000) marc      (1000)     2871 2022-03-01 13:08:02.000000 xautoml-0.1.1/xautoml/tests/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      433 2022-03-01 13:08:05.000000 xautoml-0.1.1/xautoml/tests/test_config_similarity.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1114 2022-02-08 15:11:02.000000 xautoml-0.1.1/xautoml/tests/test_ensemble_inspection.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      907 2022-02-08 15:11:02.000000 xautoml-0.1.1/xautoml/tests/test_feature_importance.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     3609 2022-03-01 08:51:46.000000 xautoml-0.1.1/xautoml/tests/test_hpimportance.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2484 2022-02-08 15:11:02.000000 xautoml-0.1.1/xautoml/tests/test_main.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     3109 2022-02-08 15:11:02.000000 xautoml-0.1.1/xautoml/tests/test_model_details.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      830 2022-02-08 15:11:02.000000 xautoml-0.1.1/xautoml/tests/test_output.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      647 2022-02-08 15:11:02.000000 xautoml-0.1.1/xautoml/tests/test_roc_curve.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     2239 2022-02-08 15:11:02.000000 xautoml-0.1.1/xautoml/tests/test_sub_pipeline.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.504152 xautoml-0.1.1/xautoml/util/
--rw-rw-r--   0 marc      (1000) marc      (1000)       92 2021-08-19 13:57:10.000000 xautoml-0.1.1/xautoml/util/__init__.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1068 2021-12-08 12:44:37.000000 xautoml-0.1.1/xautoml/util/async_queue.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1926 2022-03-01 08:20:08.000000 xautoml-0.1.1/xautoml/util/auto_sklearn.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     1560 2022-03-01 08:20:08.000000 xautoml-0.1.1/xautoml/util/config.py
--rw-rw-r--   0 marc      (1000) marc      (1000)       54 2022-01-01 20:58:22.000000 xautoml-0.1.1/xautoml/util/constants.py
--rw-rw-r--   0 marc      (1000) marc      (1000)     3538 2022-03-01 08:21:40.000000 xautoml-0.1.1/xautoml/util/datasets.py
--rw-rw-r--   0 marc      (1000) marc      (1000)      235 2022-02-02 15:32:38.000000 xautoml-0.1.1/xautoml/util/flaml.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    10572 2022-02-02 15:32:38.000000 xautoml-0.1.1/xautoml/util/mlinsights.py
--rw-rw-r--   0 marc      (1000) marc      (1000)    13759 2022-03-01 09:45:21.000000 xautoml-0.1.1/xautoml/util/pipeline_utils.py
-drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-03-01 13:15:03.468152 xautoml-0.1.1/xautoml.egg-info/
--rw-rw-r--   0 marc      (1000) marc      (1000)     5762 2022-03-01 13:15:03.000000 xautoml-0.1.1/xautoml.egg-info/PKG-INFO
--rw-rw-r--   0 marc      (1000) marc      (1000)    10628 2022-03-01 13:15:03.000000 xautoml-0.1.1/xautoml.egg-info/SOURCES.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)        1 2022-03-01 13:15:03.000000 xautoml-0.1.1/xautoml.egg-info/dependency_links.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)        1 2022-01-04 14:28:05.000000 xautoml-0.1.1/xautoml.egg-info/not-zip-safe
--rw-rw-r--   0 marc      (1000) marc      (1000)       90 2022-03-01 13:15:03.000000 xautoml-0.1.1/xautoml.egg-info/requires.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)        8 2022-03-01 13:15:03.000000 xautoml-0.1.1/xautoml.egg-info/top_level.txt
--rw-rw-r--   0 marc      (1000) marc      (1000)   321744 2022-01-04 14:31:26.000000 xautoml-0.1.1/yarn.lock
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.840513 xautoml-0.1.2/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1512 2021-05-28 09:36:11.000000 xautoml-0.1.2/LICENSE
+-rw-rw-r--   0 marc      (1000) marc      (1000)      429 2021-05-28 09:36:08.000000 xautoml-0.1.2/MANIFEST.in
+-rw-rw-r--   0 marc      (1000) marc      (1000)     7099 2022-04-08 06:30:39.840513 xautoml-0.1.2/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1000)     6324 2022-04-08 06:29:22.000000 xautoml-0.1.2/README.md
+-rw-rw-r--   0 marc      (1000) marc      (1000)      175 2021-05-28 09:31:04.000000 xautoml-0.1.2/install.json
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3428 2022-04-08 06:29:22.000000 xautoml-0.1.2/package.json
+-rw-rw-r--   0 marc      (1000) marc      (1000)      566 2022-04-08 06:29:22.000000 xautoml-0.1.2/pyproject.toml
+-rw-rw-r--   0 marc      (1000) marc      (1000)       38 2022-04-08 06:30:39.840513 xautoml-0.1.2/setup.cfg
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2480 2022-04-08 06:29:22.000000 xautoml-0.1.2/setup.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.756513 xautoml-0.1.2/src/
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.760513 xautoml-0.1.2/src/components/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5184 2022-03-01 12:50:19.000000 xautoml-0.1.2/src/components/candidate_inspections.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4814 2022-02-01 20:14:40.000000 xautoml-0.1.2/src/components/comparison.tsx
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.760513 xautoml-0.1.2/src/components/details/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     7318 2022-02-08 17:50:52.000000 xautoml-0.1.2/src/components/details/configuration.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1726 2022-01-05 21:30:41.000000 xautoml-0.1.2/src/components/details/confusion_matrix.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2211 2022-02-01 20:14:40.000000 xautoml-0.1.2/src/components/details/dataset_table.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)    14840 2022-02-08 15:11:02.000000 xautoml-0.1.2/src/components/details/feature_importance.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     9279 2022-02-08 15:11:02.000000 xautoml-0.1.2/src/components/details/global_surrogate.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)    15789 2022-02-08 15:11:02.000000 xautoml-0.1.2/src/components/details/hp_importance.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)    14217 2022-02-01 20:14:40.000000 xautoml-0.1.2/src/components/details/local_surrogate.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)      514 2022-03-01 12:50:24.000000 xautoml-0.1.2/src/components/details/model.ts
+-rw-rw-r--   0 marc      (1000) marc      (1000)     7875 2022-02-08 19:56:05.000000 xautoml-0.1.2/src/components/details/performance_details.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3306 2022-02-01 20:14:40.000000 xautoml-0.1.2/src/components/details/pipeline_hyperparameters.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     6038 2022-03-01 12:58:10.000000 xautoml-0.1.2/src/components/details/pipeline_visualization.tsx
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.760513 xautoml-0.1.2/src/components/ensemble/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2800 2022-01-13 18:11:39.000000 xautoml-0.1.2/src/components/ensemble/decision_surface.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2939 2022-02-02 15:32:38.000000 xautoml-0.1.2/src/components/ensemble/ensemble_details.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5973 2022-01-22 18:08:58.000000 xautoml-0.1.2/src/components/ensemble/ensemble_table.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     8156 2022-02-01 20:14:40.000000 xautoml-0.1.2/src/components/ensemble.tsx
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.764513 xautoml-0.1.2/src/components/general/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2567 2022-01-22 20:17:53.000000 xautoml-0.1.2/src/components/general/meta_information.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1639 2022-01-19 21:29:50.000000 xautoml-0.1.2/src/components/general/performance_distribution.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4877 2022-01-14 11:47:47.000000 xautoml-0.1.2/src/components/general/performance_timeline.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5692 2022-01-20 22:42:45.000000 xautoml-0.1.2/src/components/general/roc_curve.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)    20551 2022-03-01 13:05:12.000000 xautoml-0.1.2/src/components/leaderboard.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3490 2022-02-01 20:14:40.000000 xautoml-0.1.2/src/components/optimization_overview.tsx
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.764513 xautoml-0.1.2/src/components/pc/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4953 2021-12-17 15:06:43.000000 xautoml-0.1.2/src/components/pc/brush.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)      171 2021-12-24 09:48:18.000000 xautoml-0.1.2/src/components/pc/constants.ts
+-rw-rw-r--   0 marc      (1000) marc      (1000)     9797 2022-02-03 08:55:01.000000 xautoml-0.1.2/src/components/pc/model.ts
+-rw-rw-r--   0 marc      (1000) marc      (1000)    12074 2022-02-03 13:47:43.000000 xautoml-0.1.2/src/components/pc/parallel_corrdinates.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     9515 2022-02-01 15:06:40.000000 xautoml-0.1.2/src/components/pc/pc_axis.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3439 2022-02-01 20:14:40.000000 xautoml-0.1.2/src/components/pc/pc_choice.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     6026 2022-02-03 10:01:38.000000 xautoml-0.1.2/src/components/pc/pc_line.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     8971 2022-02-08 18:38:08.000000 xautoml-0.1.2/src/components/pc/util.ts
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.764513 xautoml-0.1.2/src/components/search_space/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      396 2021-12-24 09:48:18.000000 xautoml-0.1.2/src/components/search_space/model.ts
+-rw-rw-r--   0 marc      (1000) marc      (1000)    10263 2022-02-04 16:06:03.000000 xautoml-0.1.2/src/components/search_space/optimization_progress.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     9975 2022-02-04 14:19:32.000000 xautoml-0.1.2/src/components/search_space/sampling_history.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     7347 2022-02-01 20:14:40.000000 xautoml-0.1.2/src/components/search_space/structure_search_graph.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)    11048 2022-02-04 17:47:59.000000 xautoml-0.1.2/src/components/search_space.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3833 2022-02-01 20:14:40.000000 xautoml-0.1.2/src/dao.ts
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1610 2021-12-24 09:57:35.000000 xautoml-0.1.2/src/index.ts
+-rw-rw-r--   0 marc      (1000) marc      (1000)    11368 2022-02-08 15:11:02.000000 xautoml-0.1.2/src/jupyter.ts
+-rw-rw-r--   0 marc      (1000) marc      (1000)    13946 2022-03-01 13:02:12.000000 xautoml-0.1.2/src/model.ts
+-rw-rw-r--   0 marc      (1000) marc      (1000)     9742 2022-02-01 20:14:40.000000 xautoml-0.1.2/src/root.tsx
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.768513 xautoml-0.1.2/src/util/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1109 2022-01-06 12:45:23.000000 xautoml-0.1.2/src/util/KeyValue.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3467 2022-01-12 09:07:37.000000 xautoml-0.1.2/src/util/collapse.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)      897 2021-12-28 20:09:48.000000 xautoml-0.1.2/src/util/error.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2561 2021-12-25 17:52:58.000000 xautoml-0.1.2/src/util/flexible-svg.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)      433 2022-01-05 17:08:46.000000 xautoml-0.1.2/src/util/heading.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1068 2022-01-06 10:28:34.000000 xautoml-0.1.2/src/util/help.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5692 2022-02-01 20:14:40.000000 xautoml-0.1.2/src/util/importance_overview.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)      702 2022-01-07 16:27:26.000000 xautoml-0.1.2/src/util/jupyter-button.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1234 2022-01-06 14:00:55.000000 xautoml-0.1.2/src/util/layout.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)      329 2021-12-24 09:48:18.000000 xautoml-0.1.2/src/util/loading.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4020 2022-02-08 15:11:02.000000 xautoml-0.1.2/src/util/raw_dataset.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2614 2022-01-10 12:42:54.000000 xautoml-0.1.2/src/util/recharts.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)      884 2021-12-08 12:44:37.000000 xautoml-0.1.2/src/util/tabpanel.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     8199 2022-02-01 20:14:40.000000 xautoml-0.1.2/src/util/tree_structure.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1345 2021-12-28 20:09:48.000000 xautoml-0.1.2/src/util/warning.tsx
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3133 2022-02-08 18:12:32.000000 xautoml-0.1.2/src/util.ts
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.768513 xautoml-0.1.2/style/
+-rw-rw-r--   0 marc      (1000) marc      (1000)    10686 2022-02-08 19:54:16.000000 xautoml-0.1.2/style/base.css
+-rw-rw-r--   0 marc      (1000) marc      (1000)       25 2021-10-16 11:19:09.000000 xautoml-0.1.2/style/index.css
+-rw-rw-r--   0 marc      (1000) marc      (1000)       21 2021-05-26 19:13:54.000000 xautoml-0.1.2/style/index.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4621 2021-09-25 14:21:23.000000 xautoml-0.1.2/style/jupyter.svg
+-rw-rw-r--   0 marc      (1000) marc      (1000)      594 2021-11-24 18:54:00.000000 xautoml-0.1.2/tsconfig.json
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.772513 xautoml-0.1.2/xautoml/
+-rw-rw-r--   0 marc      (1000) marc      (1000)      824 2021-05-28 11:28:31.000000 xautoml-0.1.2/xautoml/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      395 2022-02-01 20:14:40.000000 xautoml-0.1.2/xautoml/_helper.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      441 2021-05-28 11:28:27.000000 xautoml-0.1.2/xautoml/_version.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    23431 2022-03-01 08:23:00.000000 xautoml-0.1.2/xautoml/adapter.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4918 2022-03-01 08:20:08.000000 xautoml-0.1.2/xautoml/config_similarity.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4180 2022-03-01 08:20:08.000000 xautoml-0.1.2/xautoml/ensemble.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1085 2022-01-24 11:01:42.000000 xautoml-0.1.2/xautoml/fake.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     8372 2022-03-01 08:20:08.000000 xautoml-0.1.2/xautoml/graph_similarity.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)       38 2022-03-01 08:48:29.000000 xautoml-0.1.2/xautoml/handlers.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     8128 2022-03-01 08:25:03.000000 xautoml-0.1.2/xautoml/hp_importance.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.772513 xautoml-0.1.2/xautoml/labextension/
+-rw-rw-r--   0 marc      (1000) marc      (1000)    20438 2022-03-01 12:53:37.000000 xautoml-0.1.2/xautoml/labextension/build_log.json
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3570 2022-03-01 13:05:27.000000 xautoml-0.1.2/xautoml/labextension/package.json
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.836513 xautoml-0.1.2/xautoml/labextension/static/
+-rw-rw-r--   0 marc      (1000) marc      (1000)   412454 2022-03-01 13:04:34.000000 xautoml-0.1.2/xautoml/labextension/static/lib_index_js.501b1a62f9c38ddd812b.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   341796 2022-03-01 13:04:34.000000 xautoml-0.1.2/xautoml/labextension/static/lib_index_js.501b1a62f9c38ddd812b.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)   412522 2022-03-01 13:05:27.000000 xautoml-0.1.2/xautoml/labextension/static/lib_index_js.502fd3a9cc6c92d6f591.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   341870 2022-03-01 13:05:27.000000 xautoml-0.1.2/xautoml/labextension/static/lib_index_js.502fd3a9cc6c92d6f591.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)   412308 2022-03-01 12:58:19.000000 xautoml-0.1.2/xautoml/labextension/static/lib_index_js.5fe887d7b7a8ac72fc36.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   341638 2022-03-01 12:58:19.000000 xautoml-0.1.2/xautoml/labextension/static/lib_index_js.5fe887d7b7a8ac72fc36.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)   412270 2022-03-01 12:56:15.000000 xautoml-0.1.2/xautoml/labextension/static/lib_index_js.8f01bcbb99c2065d2192.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   341600 2022-03-01 12:56:15.000000 xautoml-0.1.2/xautoml/labextension/static/lib_index_js.8f01bcbb99c2065d2192.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)   412312 2022-03-01 13:02:20.000000 xautoml-0.1.2/xautoml/labextension/static/lib_index_js.9b5313ccecf3b93fdb20.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   341642 2022-03-01 13:02:20.000000 xautoml-0.1.2/xautoml/labextension/static/lib_index_js.9b5313ccecf3b93fdb20.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)   412102 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/lib_index_js.db69110a493cf4705cb0.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   341399 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/lib_index_js.db69110a493cf4705cb0.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)    27461 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-36f31a.9e464fbf6e3483c2e9ab.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)    18346 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-36f31a.9e464fbf6e3483c2e9ab.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)     5627 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-7f3338.56735e5382d181d596df.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3051 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-7f3338.56735e5382d181d596df.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)      810 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/node_modules_babel_runtime_helpers_interopRequireDefault_js.c535f40556b43a78ad4c.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)      563 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/node_modules_babel_runtime_helpers_interopRequireDefault_js.c535f40556b43a78ad4c.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)      779 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/node_modules_d3-dag_bundle_sync_recursive.f14d00bf0acbaccd2b37.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)      619 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/node_modules_d3-dag_bundle_sync_recursive.f14d00bf0acbaccd2b37.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1920 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/node_modules_d3-ease_src_exp_js.4a5f97bc213ba7d52fa3.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)      821 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/node_modules_d3-ease_src_exp_js.4a5f97bc213ba7d52fa3.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2115 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/node_modules_memoize-one_dist_memoize-one_esm_js.1ff743ff2d8d6c8c51e6.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1948 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/node_modules_memoize-one_dist_memoize-one_esm_js.1ff743ff2d8d6c8c51e6.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)    44574 2022-03-01 13:02:20.000000 xautoml-0.1.2/xautoml/labextension/static/remoteEntry.216da5d12a1be0bf8d83.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)    44574 2022-03-01 13:04:34.000000 xautoml-0.1.2/xautoml/labextension/static/remoteEntry.24d1f891ac5575800434.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)    44574 2022-03-01 12:56:15.000000 xautoml-0.1.2/xautoml/labextension/static/remoteEntry.2f372dc7f1b00fdccb53.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)    44574 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/remoteEntry.829185034e32a3a0ea99.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)    45613 2022-03-01 13:05:27.000000 xautoml-0.1.2/xautoml/labextension/static/remoteEntry.96873ac07d1a8f07b25c.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)    44574 2022-03-01 13:05:27.000000 xautoml-0.1.2/xautoml/labextension/static/remoteEntry.96873ac07d1a8f07b25c.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)    44574 2022-03-01 12:58:19.000000 xautoml-0.1.2/xautoml/labextension/static/remoteEntry.f13baef9edaeb761b135.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)      151 2022-03-01 12:53:37.000000 xautoml-0.1.2/xautoml/labextension/static/style.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)    33221 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/style_index_css.c8843f86800ceb459e3d.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)    38690 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/style_index_css.c8843f86800ceb459e3d.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)    95169 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_classnames_index_js-node_modules_lodash_isEqual_js.75587459728afe6cc748.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)    89308 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_classnames_index_js-node_modules_lodash_isEqual_js.75587459728afe6cc748.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)    12044 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f71148bf061d5119bdad.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)    13769 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f71148bf061d5119bdad.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)    88354 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_d3-dag_bundle_d3-dag_esm_min_js.09cb9ecb1b6911f66720.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   106927 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_d3-dag_bundle_d3-dag_esm_min_js.09cb9ecb1b6911f66720.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)   248572 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_d3-scale_src_index_js-node_modules_d3-shape_src_area_js-node_modules_d3--caf5af.db0372ffdf6a4441784e.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   177546 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_d3-scale_src_index_js-node_modules_d3-shape_src_area_js-node_modules_d3--caf5af.db0372ffdf6a4441784e.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)  1031361 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_d3_index_js.4d45a37894f902446937.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   630198 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_d3_index_js.4d45a37894f902446937.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)   242440 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Avatar_Avatar_js-node_modules_material-ui_core_esm_-413d96.0cc4c1464fc16245b4ec.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   239897 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Avatar_Avatar_js-node_modules_material-ui_core_esm_-413d96.0cc4c1464fc16245b4ec.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)   374039 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Checkbox_Checkbox_js-node_modules_material-ui_core_-da75eb.bffdd92e736ff98f4579.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   308632 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Checkbox_Checkbox_js-node_modules_material-ui_core_-da75eb.bffdd92e736ff98f4579.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)   186119 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Collapse_Collapse_js-node_modules_material-ui_core_-4fe852.d1bd5e3ec3e641a02387.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   157738 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Collapse_Collapse_js-node_modules_material-ui_core_-4fe852.d1bd5e3ec3e641a02387.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)   927241 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_index_js.269833f9d86c68103a29.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   697911 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_index_js.269833f9d86c68103a29.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)   285008 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_utils_createSvgIcon_js.1ce7f7dd7d79522653b3.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   255194 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_utils_createSvgIcon_js.1ce7f7dd7d79522653b3.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)    33774 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_icons_KeyboardArrowDown_js-node_modules_material-ui_icons_Ke-8370f2.5cd0e830e24ed213a793.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)    34078 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_icons_KeyboardArrowDown_js-node_modules_material-ui_icons_Ke-8370f2.5cd0e830e24ed213a793.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000) 10656879 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_icons_esm_index_js.5ae151e2203f82f49908.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)  4122062 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_icons_esm_index_js.5ae151e2203f82f49908.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)   357516 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_lab_esm_index_js.74baedfea25f6e14abea.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   299780 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_lab_esm_index_js.74baedfea25f6e14abea.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)   101497 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_memoizee_index_js.351b5bbf5ccfe187a70f.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)    96692 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_memoizee_index_js.351b5bbf5ccfe187a70f.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)    39437 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_prop-types_index_js.76920d8992c01aa3732c.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)    44590 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_prop-types_index_js.76920d8992c01aa3732c.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)   344730 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_rc-slider_es_index_js.d87b5e830387c5756f0e.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)   296601 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_rc-slider_es_index_js.d87b5e830387c5756f0e.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)    50447 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_react-move_es_index_js.6461e26c4e5974c983b7.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)    39783 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_react-move_es_index_js.6461e26c4e5974c983b7.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)  1485433 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_recharts_es6_index_js.12271722fd3fb37e484e.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)  1485617 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_recharts_es6_index_js.12271722fd3fb37e484e.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)    34648 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_resize-observer-polyfill_dist_ResizeObserver_es_js.1bbb13fa0f5d7ffa66ca.js
+-rw-rw-r--   0 marc      (1000) marc      (1000)    41579 2022-03-01 12:53:48.000000 xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_resize-observer-polyfill_dist_ResizeObserver_es_js.1bbb13fa0f5d7ffa66ca.js.map
+-rw-rw-r--   0 marc      (1000) marc      (1000)    21430 2022-03-01 09:41:19.000000 xautoml-0.1.2/xautoml/main.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    11105 2022-03-01 08:51:46.000000 xautoml-0.1.2/xautoml/model_details.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     4307 2022-03-01 08:20:08.000000 xautoml-0.1.2/xautoml/models.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2957 2022-03-01 08:56:00.000000 xautoml-0.1.2/xautoml/output.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     6097 2022-03-01 08:45:09.000000 xautoml-0.1.2/xautoml/roc_auc.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.840513 xautoml-0.1.2/xautoml/tests/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2871 2022-03-01 13:08:02.000000 xautoml-0.1.2/xautoml/tests/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      433 2022-03-01 13:08:05.000000 xautoml-0.1.2/xautoml/tests/test_config_similarity.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1114 2022-02-08 15:11:02.000000 xautoml-0.1.2/xautoml/tests/test_ensemble_inspection.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      907 2022-02-08 15:11:02.000000 xautoml-0.1.2/xautoml/tests/test_feature_importance.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3609 2022-03-01 08:51:46.000000 xautoml-0.1.2/xautoml/tests/test_hpimportance.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2484 2022-02-08 15:11:02.000000 xautoml-0.1.2/xautoml/tests/test_main.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3109 2022-02-08 15:11:02.000000 xautoml-0.1.2/xautoml/tests/test_model_details.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      830 2022-02-08 15:11:02.000000 xautoml-0.1.2/xautoml/tests/test_output.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      647 2022-02-08 15:11:02.000000 xautoml-0.1.2/xautoml/tests/test_roc_curve.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     2239 2022-02-08 15:11:02.000000 xautoml-0.1.2/xautoml/tests/test_sub_pipeline.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.840513 xautoml-0.1.2/xautoml/util/
+-rw-rw-r--   0 marc      (1000) marc      (1000)       92 2021-08-19 13:57:10.000000 xautoml-0.1.2/xautoml/util/__init__.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1068 2021-12-08 12:44:37.000000 xautoml-0.1.2/xautoml/util/async_queue.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1926 2022-03-01 08:20:08.000000 xautoml-0.1.2/xautoml/util/auto_sklearn.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     1560 2022-03-01 08:20:08.000000 xautoml-0.1.2/xautoml/util/config.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)       54 2022-01-01 20:58:22.000000 xautoml-0.1.2/xautoml/util/constants.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)     3538 2022-03-01 08:21:40.000000 xautoml-0.1.2/xautoml/util/datasets.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)      235 2022-02-02 15:32:38.000000 xautoml-0.1.2/xautoml/util/flaml.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    10572 2022-02-02 15:32:38.000000 xautoml-0.1.2/xautoml/util/mlinsights.py
+-rw-rw-r--   0 marc      (1000) marc      (1000)    13759 2022-03-01 09:45:21.000000 xautoml-0.1.2/xautoml/util/pipeline_utils.py
+drwxrwxr-x   0 marc      (1000) marc      (1000)        0 2022-04-08 06:30:39.772513 xautoml-0.1.2/xautoml.egg-info/
+-rw-rw-r--   0 marc      (1000) marc      (1000)     7099 2022-04-08 06:30:39.000000 xautoml-0.1.2/xautoml.egg-info/PKG-INFO
+-rw-rw-r--   0 marc      (1000) marc      (1000)    10628 2022-04-08 06:30:39.000000 xautoml-0.1.2/xautoml.egg-info/SOURCES.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)        1 2022-04-08 06:30:39.000000 xautoml-0.1.2/xautoml.egg-info/dependency_links.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)        1 2022-01-04 14:28:05.000000 xautoml-0.1.2/xautoml.egg-info/not-zip-safe
+-rw-rw-r--   0 marc      (1000) marc      (1000)       93 2022-04-08 06:30:39.000000 xautoml-0.1.2/xautoml.egg-info/requires.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)        8 2022-04-08 06:30:39.000000 xautoml-0.1.2/xautoml.egg-info/top_level.txt
+-rw-rw-r--   0 marc      (1000) marc      (1000)   321744 2022-01-04 14:31:26.000000 xautoml-0.1.2/yarn.lock
```

### Comparing `xautoml-0.1.1/LICENSE` & `xautoml-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/PKG-INFO` & `xautoml-0.1.2/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,30 +1,7 @@
-Metadata-Version: 2.1
-Name: xautoml
-Version: 0.1.1
-Summary: A JupyterLab extension to visualize and explain AutoML optimization procedures.
-Home-page: https://github.com/Ennosigaeon/xautoml
-Author: Marc Zoeller
-Author-email: marc.zoeller@usu.com
-License: BSD-3-Clause
-Keywords: Jupyter,JupyterLab,JupyterLab3
-Platform: Linux
-Platform: Mac OS X
-Platform: Windows
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Framework :: Jupyter
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # XAutoML: A Visual Analytics Tool for Establishing Trust in Automated Machine Learning
 
 XAutoML is an interactive visual analytics tool for explaining AutoML optimisation procedures and ML pipelines
 constructed by AutoML. It combines interactive visualizations with established techniques from explainable AI (XAI) to
 make the complete AutoML procedure transparent and explainable. We integrate XAutoML with Jupyter to enable experienced
 users to extend the visual analytics with advanced ad-hoc visualizations based on information extracted from XAutoML
 
@@ -38,14 +15,21 @@
 but we plan to add support for further AutoML systems. You can find a video introducing XAutoML on [YouTube](https://www.youtube.com/watch?v=AyqMrdlds7o).
 
 [![XAutoML: A Visual Analytics Tool for Establishing Trust in Automated Machine Learning](https://yt-embed.herokuapp.com/embed?v=AyqMrdlds7o)](https://www.youtube.com/watch?v=AyqMrdlds7o "XAutoML: A Visual Analytics Tool for Establishing Trust in Automated Machine Learning")
 
 
 ## Install
 
+Create a new environment with python >= 3.7 and make sure swig is installed either on your system or inside the
+environment.
+
+Install swig
+- You can either install swig via conda (`conda install swig`)
+- Or follow the [official documentation](https://www.swig.org/download.html) to install it
+
 To install the extension, execute:
 
 ```bash
 pip install xautoml
 ```
 
 ## Usage
@@ -103,14 +87,26 @@
 If the server extension is installed and enabled, but you are not seeing
 the frontend extension, check the frontend extension is installed:
 
 ```bash
 jupyter labextension list
 ```
 
+If the installation failed with the following exception
+```
+[...]
+    Running setup.py install for pyrfr ... error
+    ERROR: Command errored out with exit status 1:
+    [...]
+    swig.exe -python -c++ -modern -py3 -features nondynamic -I./include -o pyrfr/regression_wrap.cpp pyrfr/regression.i
+    error: command 'swig.exe' failed: No such file or directory
+[...]
+```
+verify that you have swig installed (see [Installation](#Introduction) above).
+
 
 ## Contributing
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
@@ -161,12 +157,28 @@
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `xautoml` within that folder.
 
 
 ### Release new version
 Increase version number in `package.json` and upload the latest build to pypi.
 ```bash
-python setup.py sdist
+pip install build
+python -m build -s
 python -m twine upload dist/*
 ```
 
 
+## Citation
+If you are using `XAutoML`, please cite it as
+
+    @article{Zoller2022,
+        author = "Z{\"{o}}ller, Marc-Andr{\'{e}} and Titov, Waldemar and Schlegel, Thomas and Huber, Marco F.",
+        title = "{XAutoML: A Visual Analytics Tool for Establishing Trust in Automated Machine Learning}",
+        journal = "arXiv preprint arXiv: 2202.11954",
+        volume = "1",
+        year = "2022",
+        pages = "1-34",
+        url = "http://arxiv.org/abs/2202.11954",
+        eprint = "2202.11954",
+        archivePrefix = "arXiv",
+        arxivId = "2202.11954"
+    }
```

### Comparing `xautoml-0.1.1/package.json` & `xautoml-0.1.2/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9722222222222222%*

 * *Differences: {"'version'": "'0.1.2'"}*

```diff
@@ -102,9 +102,9 @@
         "watch:src": "tsc -w"
     },
     "sideEffects": [
         "style/*.css"
     ],
     "style": "style/index.css",
     "types": "lib/index.d.ts",
-    "version": "0.1.1"
+    "version": "0.1.2"
 }
```

### Comparing `xautoml-0.1.1/pyproject.toml` & `xautoml-0.1.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [build-system]
-requires = ["jupyter_packaging~=0.10,<2", "jupyterlab~=3.0"]
+requires = ["jupyter_packaging~=0.10,<2", "jupyterlab>=3.0,<4"]
 build-backend = "jupyter_packaging.build_api"
 
 [tool.jupyter-packaging.options]
 skip-if-exists = ["xautoml/labextension/static/style.js"]
 ensured-targets = ["xautoml/labextension/static/style.js", "xautoml/labextension/package.json"]
 
 [tool.jupyter-packaging.builder]
```

### Comparing `xautoml-0.1.1/setup.py` & `xautoml-0.1.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -41,20 +41,20 @@
     author_email=pkg_json["author"]["email"],
     description=pkg_json["description"],
     license=pkg_json["license"],
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     install_requires=[
-        "jupyterlab~=3.2",
+        "jupyterlab>=3.0,<4",
         "lime~=0.2",
         "fanova~=2.0",
         "dswizard-components~=0.2",
         "openml~=0.12",
-        "pandas~=1.3.5"
+        "pandas>=1.3.0"
     ],
     zip_safe=False,
     include_package_data=True,
     python_requires=">=3.6",
     platforms="Linux, Mac OS X, Windows",
     keywords=["Jupyter", "JupyterLab", "JupyterLab3"],
     classifiers=[
```

### Comparing `xautoml-0.1.1/src/components/candidate_inspections.tsx` & `xautoml-0.1.2/src/components/candidate_inspections.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/comparison.tsx` & `xautoml-0.1.2/src/components/comparison.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/details/configuration.tsx` & `xautoml-0.1.2/src/components/details/configuration.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/details/confusion_matrix.tsx` & `xautoml-0.1.2/src/components/details/confusion_matrix.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/details/dataset_table.tsx` & `xautoml-0.1.2/src/components/details/dataset_table.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/details/feature_importance.tsx` & `xautoml-0.1.2/src/components/details/feature_importance.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/details/global_surrogate.tsx` & `xautoml-0.1.2/src/components/details/global_surrogate.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/details/hp_importance.tsx` & `xautoml-0.1.2/src/components/details/hp_importance.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/details/local_surrogate.tsx` & `xautoml-0.1.2/src/components/details/local_surrogate.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/details/model.ts` & `xautoml-0.1.2/src/components/details/model.ts`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/details/performance_details.tsx` & `xautoml-0.1.2/src/components/details/performance_details.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/details/pipeline_hyperparameters.tsx` & `xautoml-0.1.2/src/components/details/pipeline_hyperparameters.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/details/pipeline_visualization.tsx` & `xautoml-0.1.2/src/components/details/pipeline_visualization.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/ensemble/decision_surface.tsx` & `xautoml-0.1.2/src/components/ensemble/decision_surface.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/ensemble/ensemble_details.tsx` & `xautoml-0.1.2/src/components/ensemble/ensemble_details.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/ensemble/ensemble_table.tsx` & `xautoml-0.1.2/src/components/ensemble/ensemble_table.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/ensemble.tsx` & `xautoml-0.1.2/src/components/ensemble.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/general/meta_information.tsx` & `xautoml-0.1.2/src/components/general/meta_information.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/general/performance_distribution.tsx` & `xautoml-0.1.2/src/components/general/performance_distribution.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/general/performance_timeline.tsx` & `xautoml-0.1.2/src/components/general/performance_timeline.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/general/roc_curve.tsx` & `xautoml-0.1.2/src/components/general/roc_curve.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/leaderboard.tsx` & `xautoml-0.1.2/src/components/leaderboard.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/optimization_overview.tsx` & `xautoml-0.1.2/src/components/optimization_overview.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/pc/brush.tsx` & `xautoml-0.1.2/src/components/pc/brush.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/pc/model.ts` & `xautoml-0.1.2/src/components/pc/model.ts`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/pc/parallel_corrdinates.tsx` & `xautoml-0.1.2/src/components/pc/parallel_corrdinates.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/pc/pc_axis.tsx` & `xautoml-0.1.2/src/components/pc/pc_axis.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/pc/pc_choice.tsx` & `xautoml-0.1.2/src/components/pc/pc_choice.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/pc/pc_line.tsx` & `xautoml-0.1.2/src/components/pc/pc_line.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/pc/util.ts` & `xautoml-0.1.2/src/components/pc/util.ts`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/search_space/optimization_progress.tsx` & `xautoml-0.1.2/src/components/search_space/optimization_progress.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/search_space/sampling_history.tsx` & `xautoml-0.1.2/src/components/search_space/sampling_history.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/search_space/structure_search_graph.tsx` & `xautoml-0.1.2/src/components/search_space/structure_search_graph.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/components/search_space.tsx` & `xautoml-0.1.2/src/components/search_space.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/dao.ts` & `xautoml-0.1.2/src/dao.ts`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/index.ts` & `xautoml-0.1.2/src/index.ts`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/jupyter.ts` & `xautoml-0.1.2/src/jupyter.ts`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/model.ts` & `xautoml-0.1.2/src/model.ts`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/root.tsx` & `xautoml-0.1.2/src/root.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/util/KeyValue.tsx` & `xautoml-0.1.2/src/util/KeyValue.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/util/collapse.tsx` & `xautoml-0.1.2/src/util/collapse.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/util/error.tsx` & `xautoml-0.1.2/src/util/error.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/util/flexible-svg.tsx` & `xautoml-0.1.2/src/util/flexible-svg.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/util/help.tsx` & `xautoml-0.1.2/src/util/help.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/util/importance_overview.tsx` & `xautoml-0.1.2/src/util/importance_overview.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/util/jupyter-button.tsx` & `xautoml-0.1.2/src/util/jupyter-button.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/util/layout.tsx` & `xautoml-0.1.2/src/util/layout.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/util/raw_dataset.tsx` & `xautoml-0.1.2/src/util/raw_dataset.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/util/recharts.tsx` & `xautoml-0.1.2/src/util/recharts.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/util/tabpanel.tsx` & `xautoml-0.1.2/src/util/tabpanel.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/util/tree_structure.tsx` & `xautoml-0.1.2/src/util/tree_structure.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/util/warning.tsx` & `xautoml-0.1.2/src/util/warning.tsx`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/src/util.ts` & `xautoml-0.1.2/src/util.ts`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/style/base.css` & `xautoml-0.1.2/style/base.css`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/style/jupyter.svg` & `xautoml-0.1.2/style/jupyter.svg`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/tsconfig.json` & `xautoml-0.1.2/tsconfig.json`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/__init__.py` & `xautoml-0.1.2/xautoml/__init__.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/adapter.py` & `xautoml-0.1.2/xautoml/adapter.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/config_similarity.py` & `xautoml-0.1.2/xautoml/config_similarity.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/ensemble.py` & `xautoml-0.1.2/xautoml/ensemble.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/fake.py` & `xautoml-0.1.2/xautoml/fake.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/graph_similarity.py` & `xautoml-0.1.2/xautoml/graph_similarity.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/hp_importance.py` & `xautoml-0.1.2/xautoml/hp_importance.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/build_log.json` & `xautoml-0.1.2/xautoml/labextension/build_log.json`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/package.json` & `xautoml-0.1.2/xautoml/labextension/package.json`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/lib_index_js.501b1a62f9c38ddd812b.js` & `xautoml-0.1.2/xautoml/labextension/static/lib_index_js.501b1a62f9c38ddd812b.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/lib_index_js.501b1a62f9c38ddd812b.js.map` & `xautoml-0.1.2/xautoml/labextension/static/lib_index_js.501b1a62f9c38ddd812b.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/lib_index_js.502fd3a9cc6c92d6f591.js` & `xautoml-0.1.2/xautoml/labextension/static/lib_index_js.502fd3a9cc6c92d6f591.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/lib_index_js.502fd3a9cc6c92d6f591.js.map` & `xautoml-0.1.2/xautoml/labextension/static/lib_index_js.502fd3a9cc6c92d6f591.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/lib_index_js.5fe887d7b7a8ac72fc36.js` & `xautoml-0.1.2/xautoml/labextension/static/lib_index_js.5fe887d7b7a8ac72fc36.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/lib_index_js.5fe887d7b7a8ac72fc36.js.map` & `xautoml-0.1.2/xautoml/labextension/static/lib_index_js.5fe887d7b7a8ac72fc36.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/lib_index_js.8f01bcbb99c2065d2192.js` & `xautoml-0.1.2/xautoml/labextension/static/lib_index_js.8f01bcbb99c2065d2192.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/lib_index_js.8f01bcbb99c2065d2192.js.map` & `xautoml-0.1.2/xautoml/labextension/static/lib_index_js.8f01bcbb99c2065d2192.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/lib_index_js.9b5313ccecf3b93fdb20.js` & `xautoml-0.1.2/xautoml/labextension/static/lib_index_js.9b5313ccecf3b93fdb20.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/lib_index_js.9b5313ccecf3b93fdb20.js.map` & `xautoml-0.1.2/xautoml/labextension/static/lib_index_js.9b5313ccecf3b93fdb20.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/lib_index_js.db69110a493cf4705cb0.js` & `xautoml-0.1.2/xautoml/labextension/static/lib_index_js.db69110a493cf4705cb0.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/lib_index_js.db69110a493cf4705cb0.js.map` & `xautoml-0.1.2/xautoml/labextension/static/lib_index_js.db69110a493cf4705cb0.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-36f31a.9e464fbf6e3483c2e9ab.js` & `xautoml-0.1.2/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-36f31a.9e464fbf6e3483c2e9ab.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-36f31a.9e464fbf6e3483c2e9ab.js.map` & `xautoml-0.1.2/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-36f31a.9e464fbf6e3483c2e9ab.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-7f3338.56735e5382d181d596df.js` & `xautoml-0.1.2/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-7f3338.56735e5382d181d596df.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-7f3338.56735e5382d181d596df.js.map` & `xautoml-0.1.2/xautoml/labextension/static/node_modules_babel_runtime_helpers_esm_assertThisInitialized_js-node_modules_babel_runtime_he-7f3338.56735e5382d181d596df.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/node_modules_babel_runtime_helpers_interopRequireDefault_js.c535f40556b43a78ad4c.js` & `xautoml-0.1.2/xautoml/labextension/static/node_modules_babel_runtime_helpers_interopRequireDefault_js.c535f40556b43a78ad4c.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/node_modules_babel_runtime_helpers_interopRequireDefault_js.c535f40556b43a78ad4c.js.map` & `xautoml-0.1.2/xautoml/labextension/static/node_modules_babel_runtime_helpers_interopRequireDefault_js.c535f40556b43a78ad4c.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/node_modules_d3-dag_bundle_sync_recursive.f14d00bf0acbaccd2b37.js` & `xautoml-0.1.2/xautoml/labextension/static/node_modules_d3-dag_bundle_sync_recursive.f14d00bf0acbaccd2b37.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/node_modules_d3-dag_bundle_sync_recursive.f14d00bf0acbaccd2b37.js.map` & `xautoml-0.1.2/xautoml/labextension/static/node_modules_d3-dag_bundle_sync_recursive.f14d00bf0acbaccd2b37.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/node_modules_d3-ease_src_exp_js.4a5f97bc213ba7d52fa3.js` & `xautoml-0.1.2/xautoml/labextension/static/node_modules_d3-ease_src_exp_js.4a5f97bc213ba7d52fa3.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/node_modules_d3-ease_src_exp_js.4a5f97bc213ba7d52fa3.js.map` & `xautoml-0.1.2/xautoml/labextension/static/node_modules_d3-ease_src_exp_js.4a5f97bc213ba7d52fa3.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/node_modules_memoize-one_dist_memoize-one_esm_js.1ff743ff2d8d6c8c51e6.js` & `xautoml-0.1.2/xautoml/labextension/static/node_modules_memoize-one_dist_memoize-one_esm_js.1ff743ff2d8d6c8c51e6.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/node_modules_memoize-one_dist_memoize-one_esm_js.1ff743ff2d8d6c8c51e6.js.map` & `xautoml-0.1.2/xautoml/labextension/static/node_modules_memoize-one_dist_memoize-one_esm_js.1ff743ff2d8d6c8c51e6.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/remoteEntry.216da5d12a1be0bf8d83.js.map` & `xautoml-0.1.2/xautoml/labextension/static/remoteEntry.216da5d12a1be0bf8d83.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/remoteEntry.24d1f891ac5575800434.js.map` & `xautoml-0.1.2/xautoml/labextension/static/remoteEntry.24d1f891ac5575800434.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/remoteEntry.2f372dc7f1b00fdccb53.js.map` & `xautoml-0.1.2/xautoml/labextension/static/remoteEntry.2f372dc7f1b00fdccb53.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/remoteEntry.829185034e32a3a0ea99.js.map` & `xautoml-0.1.2/xautoml/labextension/static/remoteEntry.829185034e32a3a0ea99.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/remoteEntry.96873ac07d1a8f07b25c.js` & `xautoml-0.1.2/xautoml/labextension/static/remoteEntry.96873ac07d1a8f07b25c.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/remoteEntry.96873ac07d1a8f07b25c.js.map` & `xautoml-0.1.2/xautoml/labextension/static/remoteEntry.96873ac07d1a8f07b25c.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/remoteEntry.f13baef9edaeb761b135.js.map` & `xautoml-0.1.2/xautoml/labextension/static/remoteEntry.f13baef9edaeb761b135.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/style_index_css.c8843f86800ceb459e3d.js` & `xautoml-0.1.2/xautoml/labextension/static/style_index_css.c8843f86800ceb459e3d.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/style_index_css.c8843f86800ceb459e3d.js.map` & `xautoml-0.1.2/xautoml/labextension/static/style_index_css.c8843f86800ceb459e3d.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_classnames_index_js-node_modules_lodash_isEqual_js.75587459728afe6cc748.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_classnames_index_js-node_modules_lodash_isEqual_js.75587459728afe6cc748.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_classnames_index_js-node_modules_lodash_isEqual_js.75587459728afe6cc748.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_classnames_index_js-node_modules_lodash_isEqual_js.75587459728afe6cc748.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f71148bf061d5119bdad.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f71148bf061d5119bdad.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f71148bf061d5119bdad.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_css-loader_dist_runtime_api_js-node_modules_css-loader_dist_runtime_cssW-72eba1.f71148bf061d5119bdad.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_d3-dag_bundle_d3-dag_esm_min_js.09cb9ecb1b6911f66720.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_d3-dag_bundle_d3-dag_esm_min_js.09cb9ecb1b6911f66720.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_d3-dag_bundle_d3-dag_esm_min_js.09cb9ecb1b6911f66720.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_d3-dag_bundle_d3-dag_esm_min_js.09cb9ecb1b6911f66720.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_d3-scale_src_index_js-node_modules_d3-shape_src_area_js-node_modules_d3--caf5af.db0372ffdf6a4441784e.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_d3-scale_src_index_js-node_modules_d3-shape_src_area_js-node_modules_d3--caf5af.db0372ffdf6a4441784e.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_d3-scale_src_index_js-node_modules_d3-shape_src_area_js-node_modules_d3--caf5af.db0372ffdf6a4441784e.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_d3-scale_src_index_js-node_modules_d3-shape_src_area_js-node_modules_d3--caf5af.db0372ffdf6a4441784e.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_d3_index_js.4d45a37894f902446937.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_d3_index_js.4d45a37894f902446937.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_d3_index_js.4d45a37894f902446937.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_d3_index_js.4d45a37894f902446937.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Avatar_Avatar_js-node_modules_material-ui_core_esm_-413d96.0cc4c1464fc16245b4ec.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Avatar_Avatar_js-node_modules_material-ui_core_esm_-413d96.0cc4c1464fc16245b4ec.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Avatar_Avatar_js-node_modules_material-ui_core_esm_-413d96.0cc4c1464fc16245b4ec.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Avatar_Avatar_js-node_modules_material-ui_core_esm_-413d96.0cc4c1464fc16245b4ec.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Checkbox_Checkbox_js-node_modules_material-ui_core_-da75eb.bffdd92e736ff98f4579.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Checkbox_Checkbox_js-node_modules_material-ui_core_-da75eb.bffdd92e736ff98f4579.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Checkbox_Checkbox_js-node_modules_material-ui_core_-da75eb.bffdd92e736ff98f4579.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Checkbox_Checkbox_js-node_modules_material-ui_core_-da75eb.bffdd92e736ff98f4579.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Collapse_Collapse_js-node_modules_material-ui_core_-4fe852.d1bd5e3ec3e641a02387.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Collapse_Collapse_js-node_modules_material-ui_core_-4fe852.d1bd5e3ec3e641a02387.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Collapse_Collapse_js-node_modules_material-ui_core_-4fe852.d1bd5e3ec3e641a02387.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_Collapse_Collapse_js-node_modules_material-ui_core_-4fe852.d1bd5e3ec3e641a02387.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_index_js.269833f9d86c68103a29.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_index_js.269833f9d86c68103a29.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_index_js.269833f9d86c68103a29.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_index_js.269833f9d86c68103a29.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_utils_createSvgIcon_js.1ce7f7dd7d79522653b3.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_utils_createSvgIcon_js.1ce7f7dd7d79522653b3.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_utils_createSvgIcon_js.1ce7f7dd7d79522653b3.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_core_esm_utils_createSvgIcon_js.1ce7f7dd7d79522653b3.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_icons_KeyboardArrowDown_js-node_modules_material-ui_icons_Ke-8370f2.5cd0e830e24ed213a793.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_icons_KeyboardArrowDown_js-node_modules_material-ui_icons_Ke-8370f2.5cd0e830e24ed213a793.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_icons_KeyboardArrowDown_js-node_modules_material-ui_icons_Ke-8370f2.5cd0e830e24ed213a793.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_icons_KeyboardArrowDown_js-node_modules_material-ui_icons_Ke-8370f2.5cd0e830e24ed213a793.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_icons_esm_index_js.5ae151e2203f82f49908.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_icons_esm_index_js.5ae151e2203f82f49908.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_icons_esm_index_js.5ae151e2203f82f49908.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_icons_esm_index_js.5ae151e2203f82f49908.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_lab_esm_index_js.74baedfea25f6e14abea.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_lab_esm_index_js.74baedfea25f6e14abea.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_material-ui_lab_esm_index_js.74baedfea25f6e14abea.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_material-ui_lab_esm_index_js.74baedfea25f6e14abea.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_memoizee_index_js.351b5bbf5ccfe187a70f.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_memoizee_index_js.351b5bbf5ccfe187a70f.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_memoizee_index_js.351b5bbf5ccfe187a70f.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_memoizee_index_js.351b5bbf5ccfe187a70f.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_prop-types_index_js.76920d8992c01aa3732c.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_prop-types_index_js.76920d8992c01aa3732c.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_prop-types_index_js.76920d8992c01aa3732c.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_prop-types_index_js.76920d8992c01aa3732c.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_rc-slider_es_index_js.d87b5e830387c5756f0e.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_rc-slider_es_index_js.d87b5e830387c5756f0e.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_rc-slider_es_index_js.d87b5e830387c5756f0e.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_rc-slider_es_index_js.d87b5e830387c5756f0e.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_react-move_es_index_js.6461e26c4e5974c983b7.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_react-move_es_index_js.6461e26c4e5974c983b7.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_react-move_es_index_js.6461e26c4e5974c983b7.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_react-move_es_index_js.6461e26c4e5974c983b7.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_recharts_es6_index_js.12271722fd3fb37e484e.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_recharts_es6_index_js.12271722fd3fb37e484e.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_recharts_es6_index_js.12271722fd3fb37e484e.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_recharts_es6_index_js.12271722fd3fb37e484e.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_resize-observer-polyfill_dist_ResizeObserver_es_js.1bbb13fa0f5d7ffa66ca.js` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_resize-observer-polyfill_dist_ResizeObserver_es_js.1bbb13fa0f5d7ffa66ca.js`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/labextension/static/vendors-node_modules_resize-observer-polyfill_dist_ResizeObserver_es_js.1bbb13fa0f5d7ffa66ca.js.map` & `xautoml-0.1.2/xautoml/labextension/static/vendors-node_modules_resize-observer-polyfill_dist_ResizeObserver_es_js.1bbb13fa0f5d7ffa66ca.js.map`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/main.py` & `xautoml-0.1.2/xautoml/main.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/model_details.py` & `xautoml-0.1.2/xautoml/model_details.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/models.py` & `xautoml-0.1.2/xautoml/models.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/output.py` & `xautoml-0.1.2/xautoml/output.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/roc_auc.py` & `xautoml-0.1.2/xautoml/roc_auc.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/tests/__init__.py` & `xautoml-0.1.2/xautoml/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/tests/test_ensemble_inspection.py` & `xautoml-0.1.2/xautoml/tests/test_ensemble_inspection.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/tests/test_feature_importance.py` & `xautoml-0.1.2/xautoml/tests/test_feature_importance.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/tests/test_hpimportance.py` & `xautoml-0.1.2/xautoml/tests/test_hpimportance.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/tests/test_main.py` & `xautoml-0.1.2/xautoml/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/tests/test_model_details.py` & `xautoml-0.1.2/xautoml/tests/test_model_details.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/tests/test_output.py` & `xautoml-0.1.2/xautoml/tests/test_output.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/tests/test_roc_curve.py` & `xautoml-0.1.2/xautoml/tests/test_roc_curve.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/tests/test_sub_pipeline.py` & `xautoml-0.1.2/xautoml/tests/test_sub_pipeline.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/util/async_queue.py` & `xautoml-0.1.2/xautoml/util/async_queue.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/util/auto_sklearn.py` & `xautoml-0.1.2/xautoml/util/auto_sklearn.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/util/config.py` & `xautoml-0.1.2/xautoml/util/config.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/util/datasets.py` & `xautoml-0.1.2/xautoml/util/datasets.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/util/mlinsights.py` & `xautoml-0.1.2/xautoml/util/mlinsights.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml/util/pipeline_utils.py` & `xautoml-0.1.2/xautoml/util/pipeline_utils.py`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/xautoml.egg-info/PKG-INFO` & `xautoml-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xautoml
-Version: 0.1.1
+Version: 0.1.2
 Summary: A JupyterLab extension to visualize and explain AutoML optimization procedures.
 Home-page: https://github.com/Ennosigaeon/xautoml
 Author: Marc Zoeller
 Author-email: marc.zoeller@usu.com
 License: BSD-3-Clause
 Keywords: Jupyter,JupyterLab,JupyterLab3
 Platform: Linux
@@ -38,14 +38,21 @@
 but we plan to add support for further AutoML systems. You can find a video introducing XAutoML on [YouTube](https://www.youtube.com/watch?v=AyqMrdlds7o).
 
 [![XAutoML: A Visual Analytics Tool for Establishing Trust in Automated Machine Learning](https://yt-embed.herokuapp.com/embed?v=AyqMrdlds7o)](https://www.youtube.com/watch?v=AyqMrdlds7o "XAutoML: A Visual Analytics Tool for Establishing Trust in Automated Machine Learning")
 
 
 ## Install
 
+Create a new environment with python >= 3.7 and make sure swig is installed either on your system or inside the
+environment.
+
+Install swig
+- You can either install swig via conda (`conda install swig`)
+- Or follow the [official documentation](https://www.swig.org/download.html) to install it
+
 To install the extension, execute:
 
 ```bash
 pip install xautoml
 ```
 
 ## Usage
@@ -103,14 +110,26 @@
 If the server extension is installed and enabled, but you are not seeing
 the frontend extension, check the frontend extension is installed:
 
 ```bash
 jupyter labextension list
 ```
 
+If the installation failed with the following exception
+```
+[...]
+    Running setup.py install for pyrfr ... error
+    ERROR: Command errored out with exit status 1:
+    [...]
+    swig.exe -python -c++ -modern -py3 -features nondynamic -I./include -o pyrfr/regression_wrap.cpp pyrfr/regression.i
+    error: command 'swig.exe' failed: No such file or directory
+[...]
+```
+verify that you have swig installed (see [Installation](#Introduction) above).
+
 
 ## Contributing
 
 ### Development install
 
 Note: You will need NodeJS to build the extension package.
 
@@ -161,12 +180,30 @@
 command. To find its location, you can run `jupyter labextension list` to figure out where the `labextensions`
 folder is located. Then you can remove the symlink named `xautoml` within that folder.
 
 
 ### Release new version
 Increase version number in `package.json` and upload the latest build to pypi.
 ```bash
-python setup.py sdist
+pip install build
+python -m build -s
 python -m twine upload dist/*
 ```
 
 
+## Citation
+If you are using `XAutoML`, please cite it as
+
+    @article{Zoller2022,
+        author = "Z{\"{o}}ller, Marc-Andr{\'{e}} and Titov, Waldemar and Schlegel, Thomas and Huber, Marco F.",
+        title = "{XAutoML: A Visual Analytics Tool for Establishing Trust in Automated Machine Learning}",
+        journal = "arXiv preprint arXiv: 2202.11954",
+        volume = "1",
+        year = "2022",
+        pages = "1-34",
+        url = "http://arxiv.org/abs/2202.11954",
+        eprint = "2202.11954",
+        archivePrefix = "arXiv",
+        arxivId = "2202.11954"
+    }
+
+
```

### Comparing `xautoml-0.1.1/xautoml.egg-info/SOURCES.txt` & `xautoml-0.1.2/xautoml.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `xautoml-0.1.1/yarn.lock` & `xautoml-0.1.2/yarn.lock`

 * *Files identical despite different names*

