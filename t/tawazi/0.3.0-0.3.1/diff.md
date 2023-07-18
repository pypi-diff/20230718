# Comparing `tmp/tawazi-0.3.0.tar.gz` & `tmp/tawazi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tawazi-0.3.0.tar", last modified: Thu Jun  1 08:00:33 2023, max compression
+gzip compressed data, was "tawazi-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tawazi-0.3.0.tar` & `tawazi-0.3.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0       74 2023-03-10 19:29:40.629046 tawazi-0.3.0/.bandit
--rw-r--r--   0        0        0       58 2022-09-09 17:49:07.274039 tawazi-0.3.0/.flake8
--rw-r--r--   0        0        0      655 2023-03-10 19:29:40.629046 tawazi-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      567 2023-03-10 19:29:40.629046 tawazi-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     1216 2023-03-10 19:29:40.633046 tawazi-0.3.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0        0        0      529 2022-09-02 12:29:48.007747 tawazi-0.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0      625 2023-05-30 16:13:24.605608 tawazi-0.3.0/.github/workflows/documentation-validation-workflow.yml
--rw-r--r--   0        0        0      686 2023-03-10 19:29:40.633046 tawazi-0.3.0/.github/workflows/formatting-workflow.yml
--rw-r--r--   0        0        0     1522 2023-03-28 14:35:03.514988 tawazi-0.3.0/.github/workflows/testing-workflow.yml
--rw-r--r--   0        0        0     1834 2023-03-10 19:29:40.633046 tawazi-0.3.0/.gitignore
--rw-r--r--   0        0        0     1032 2023-05-23 11:46:23.707166 tawazi-0.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0     3889 2023-06-01 07:58:52.768041 tawazi-0.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     5220 2022-09-09 17:49:07.274039 tawazi-0.3.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2376 2022-09-09 17:49:07.274039 tawazi-0.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0    11336 2022-06-08 12:47:16.124172 tawazi-0.3.0/LICENSE
--rw-r--r--   0        0        0     4294 2023-05-24 15:05:58.301886 tawazi-0.3.0/README.md
--rw-r--r--   0        0        0       54 2023-03-10 19:29:40.633046 tawazi-0.3.0/codecov.yml
--rw-r--r--   0        0        0      163 2023-05-24 15:53:47.635584 tawazi-0.3.0/documentation/DAGExecution.md
--rw-r--r--   0        0        0      268 2023-05-24 15:53:47.635584 tawazi-0.3.0/documentation/dag.md
--rw-r--r--   0        0        0       78 2023-05-24 15:53:47.635584 tawazi-0.3.0/documentation/decorators.md
--rw-r--r--   0        0        0     2630 2023-03-28 14:31:27.414878 tawazi-0.3.0/documentation/future_developments.md
--rw-r--r--   0        0        0    21196 2023-05-31 15:06:23.150540 tawazi-0.3.0/documentation/index.md
--rw-r--r--   0        0        0      323 2023-05-30 16:13:24.605608 tawazi-0.3.0/documentation/nodes.md
--rw-r--r--   0        0        0      179 2023-05-31 15:06:23.150540 tawazi-0.3.0/documentation/others.md
--rw-r--r--   0        0        0    86587 2023-03-10 18:51:45.700072 tawazi-0.3.0/documentation/tawazi_GIF.gif
--rw-r--r--   0        0        0     1733 2023-03-10 19:29:40.633046 tawazi-0.3.0/example.py
--rw-r--r--   0        0        0     1074 2023-05-31 15:06:23.150540 tawazi-0.3.0/mkdocs.yml
--rw-r--r--   0        0        0     1972 2023-06-01 07:58:52.768041 tawazi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      509 2023-06-01 07:58:52.768041 tawazi-0.3.0/tawazi/__init__.py
--rw-r--r--   0        0        0       70 2023-05-30 15:35:12.327370 tawazi-0.3.0/tawazi/_dag/__init__.py
--rw-r--r--   0        0        0    46163 2023-05-30 16:13:24.605608 tawazi-0.3.0/tawazi/_dag/dag.py
--rw-r--r--   0        0        0     5943 2023-05-31 15:06:23.150540 tawazi-0.3.0/tawazi/_dag/digraph.py
--rw-r--r--   0        0        0    10561 2023-05-31 15:06:23.150540 tawazi-0.3.0/tawazi/_dag/helpers.py
--rw-r--r--   0        0        0     9781 2023-05-31 15:06:23.150540 tawazi-0.3.0/tawazi/_decorators.py
--rw-r--r--   0        0        0     3122 2023-05-30 16:13:24.609608 tawazi-0.3.0/tawazi/_helpers.py
--rw-r--r--   0        0        0      487 2023-05-24 15:05:58.305886 tawazi-0.3.0/tawazi/_object_helpers.py
--rw-r--r--   0        0        0     2483 2023-05-31 15:06:23.150540 tawazi-0.3.0/tawazi/config.py
--rw-r--r--   0        0        0     3963 2023-05-31 15:06:23.150540 tawazi-0.3.0/tawazi/consts.py
--rw-r--r--   0        0        0     1862 2023-05-30 16:13:24.609608 tawazi-0.3.0/tawazi/errors.py
--rw-r--r--   0        0        0      316 2023-05-24 16:00:12.734872 tawazi-0.3.0/tawazi/node/__init__.py
--rw-r--r--   0        0        0     2866 2023-05-24 16:00:12.734872 tawazi-0.3.0/tawazi/node/functions.py
--rw-r--r--   0        0        0      994 2023-05-24 16:00:12.734872 tawazi-0.3.0/tawazi/node/helpers.py
--rw-r--r--   0        0        0    33386 2023-05-31 15:06:23.150540 tawazi-0.3.0/tawazi/node/node.py
--rw-r--r--   0        0        0     3362 2023-05-30 16:13:24.609608 tawazi-0.3.0/tawazi/profile.py
--rw-r--r--   0        0        0        0 2023-03-14 13:47:29.118468 tawazi-0.3.0/tawazi/py.typed
--rw-r--r--   0        0        0       68 2023-03-10 19:29:40.641045 tawazi-0.3.0/tests/__init__.py
--rw-r--r--   0        0        0     3751 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_active.py
--rw-r--r--   0        0        0     2641 2023-05-31 15:06:23.150540 tawazi-0.3.0/tests/test_behavior.py
--rw-r--r--   0        0        0     2292 2023-05-30 09:51:14.013295 tawazi-0.3.0/tests/test_build.py
--rw-r--r--   0        0        0     7666 2023-05-24 14:25:42.922948 tawazi-0.3.0/tests/test_cache_feature.py
--rw-r--r--   0        0        0     1425 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_compound_priority.py
--rw-r--r--   0        0        0     4288 2023-05-31 15:06:23.150540 tawazi-0.3.0/tests/test_config.py
--rw-r--r--   0        0        0     5337 2023-05-11 14:42:39.170761 tawazi-0.3.0/tests/test_dag_compose.py
--rw-r--r--   0        0        0     1740 2023-03-10 19:29:40.641045 tawazi-0.3.0/tests/test_dag_config.py
--rw-r--r--   0        0        0     2883 2023-05-24 18:48:26.478266 tawazi-0.3.0/tests/test_dagexecutor.py
--rw-r--r--   0        0        0     4022 2023-05-30 16:13:24.609608 tawazi-0.3.0/tests/test_debug_nodes.py
--rw-r--r--   0        0        0      730 2023-03-10 19:29:40.641045 tawazi-0.3.0/tests/test_decorator.py
--rw-r--r--   0        0        0     1325 2023-05-30 09:51:14.013295 tawazi-0.3.0/tests/test_edge_cases_dag.py
--rw-r--r--   0        0        0      362 2023-05-24 14:25:42.922948 tawazi-0.3.0/tests/test_error_during_dag_build.py
--rw-r--r--   0        0        0     4079 2023-05-30 16:13:24.609608 tawazi-0.3.0/tests/test_exclude_nodes.py
--rw-r--r--   0        0        0      422 2023-03-10 19:29:40.641045 tawazi-0.3.0/tests/test_execution_time.py
--rw-r--r--   0        0        0     1318 2023-05-24 14:25:42.922948 tawazi-0.3.0/tests/test_graph.py
--rw-r--r--   0        0        0      610 2023-03-10 19:29:40.641045 tawazi-0.3.0/tests/test_imbricated_dags.py
--rw-r--r--   0        0        0     2262 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_methods.py
--rw-r--r--   0        0        0     5791 2023-05-22 15:30:39.805326 tawazi-0.3.0/tests/test_multiple_return_value_for_exec_node.py
--rw-r--r--   0        0        0     2446 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_multiple_return_value_for_graph.py
--rw-r--r--   0        0        0      413 2023-03-10 19:29:40.641045 tawazi-0.3.0/tests/test_non_picklable_arguments.py
--rw-r--r--   0        0        0     2299 2023-05-31 13:03:56.304999 tawazi-0.3.0/tests/test_op.py
--rw-r--r--   0        0        0    18550 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_operators.py
--rw-r--r--   0        0        0     2609 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_ops_interface.py
--rw-r--r--   0        0        0     1410 2023-05-30 16:13:24.609608 tawazi-0.3.0/tests/test_pipeline_input_output.py
--rw-r--r--   0        0        0     3388 2023-05-24 14:25:42.922948 tawazi-0.3.0/tests/test_priority_sequential.py
--rw-r--r--   0        0        0     2801 2023-05-24 14:25:42.922948 tawazi-0.3.0/tests/test_profiling.py
--rw-r--r--   0        0        0     1508 2023-05-31 15:06:23.150540 tawazi-0.3.0/tests/test_resource.py
--rw-r--r--   0        0        0     2899 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_safe_execution.py
--rw-r--r--   0        0        0      279 2023-03-10 19:29:40.645045 tawazi-0.3.0/tests/test_same_op_reuse.py
--rw-r--r--   0        0        0    10318 2023-05-30 16:13:24.609608 tawazi-0.3.0/tests/test_setup_nodes.py
--rw-r--r--   0        0        0     3592 2023-05-30 09:51:09.709460 tawazi-0.3.0/tests/test_subgraph.py
--rw-r--r--   0        0        0      909 2023-04-12 15:30:48.423260 tawazi-0.3.0/tests/test_tags.py
--rw-r--r--   0        0        0     1841 2023-05-30 16:13:24.609608 tawazi-0.3.0/tests/test_typing.py
--rw-r--r--   0        0        0      776 2023-03-10 19:29:40.645045 tawazi-0.3.0/tests/test_wrapped_function.py
--rw-r--r--   0        0        0        0 2023-03-10 18:51:45.704072 tawazi-0.3.0/tests/tests/__init__.py
--rw-r--r--   0        0        0     5292 1970-01-01 00:00:00.000000 tawazi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0       74 2023-06-22 08:51:55.496693 tawazi-0.3.1/.bandit
+-rw-r--r--   0        0        0       58 2023-06-22 08:51:55.496693 tawazi-0.3.1/.flake8
+-rw-r--r--   0        0        0      655 2023-06-22 08:51:55.496693 tawazi-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      567 2023-06-22 08:51:55.496693 tawazi-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     1216 2023-06-22 08:51:55.496693 tawazi-0.3.1/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0        0        0      529 2023-06-22 08:51:55.496693 tawazi-0.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      625 2023-06-22 08:51:55.496693 tawazi-0.3.1/.github/workflows/documentation-validation-workflow.yml
+-rw-r--r--   0        0        0      686 2023-07-18 10:30:38.850498 tawazi-0.3.1/.github/workflows/formatting-workflow.yml
+-rw-r--r--   0        0        0     1522 2023-06-22 08:51:55.496693 tawazi-0.3.1/.github/workflows/testing-workflow.yml
+-rw-r--r--   0        0        0     1834 2023-06-22 08:51:55.496693 tawazi-0.3.1/.gitignore
+-rw-r--r--   0        0        0     1032 2023-07-18 12:55:48.244884 tawazi-0.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     4132 2023-07-18 14:21:50.336231 tawazi-0.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     5220 2023-06-22 08:51:55.496693 tawazi-0.3.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2376 2023-06-22 08:51:55.496693 tawazi-0.3.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11336 2023-06-22 08:51:55.496693 tawazi-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4294 2023-06-22 08:51:55.496693 tawazi-0.3.1/README.md
+-rw-r--r--   0        0        0       54 2023-06-22 08:51:55.496693 tawazi-0.3.1/codecov.yml
+-rw-r--r--   0        0        0      163 2023-06-22 08:51:55.496693 tawazi-0.3.1/documentation/DAGExecution.md
+-rw-r--r--   0        0        0      268 2023-06-22 08:51:55.496693 tawazi-0.3.1/documentation/dag.md
+-rw-r--r--   0        0        0       78 2023-06-22 08:51:55.496693 tawazi-0.3.1/documentation/decorators.md
+-rw-r--r--   0        0        0     2630 2023-07-06 13:02:46.428218 tawazi-0.3.1/documentation/future_developments.md
+-rw-r--r--   0        0        0    21196 2023-07-06 13:02:46.428218 tawazi-0.3.1/documentation/index.md
+-rw-r--r--   0        0        0      323 2023-06-22 08:51:55.496693 tawazi-0.3.1/documentation/nodes.md
+-rw-r--r--   0        0        0      179 2023-06-22 08:51:55.496693 tawazi-0.3.1/documentation/others.md
+-rw-r--r--   0        0        0    86587 2023-06-22 08:51:55.496693 tawazi-0.3.1/documentation/tawazi_GIF.gif
+-rw-r--r--   0        0        0     1733 2023-06-22 08:51:55.496693 tawazi-0.3.1/example.py
+-rw-r--r--   0        0        0     1074 2023-06-22 08:51:55.496693 tawazi-0.3.1/mkdocs.yml
+-rw-r--r--   0        0        0     1972 2023-07-18 14:21:50.336231 tawazi-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      509 2023-07-18 14:21:50.336231 tawazi-0.3.1/tawazi/__init__.py
+-rw-r--r--   0        0        0       70 2023-06-22 08:51:55.496693 tawazi-0.3.1/tawazi/_dag/__init__.py
+-rw-r--r--   0        0        0    46753 2023-07-18 12:55:48.248884 tawazi-0.3.1/tawazi/_dag/dag.py
+-rw-r--r--   0        0        0     5943 2023-06-22 08:51:55.500692 tawazi-0.3.1/tawazi/_dag/digraph.py
+-rw-r--r--   0        0        0    10561 2023-07-18 10:05:08.242049 tawazi-0.3.1/tawazi/_dag/helpers.py
+-rw-r--r--   0        0        0     9781 2023-07-06 13:02:46.428218 tawazi-0.3.1/tawazi/_decorators.py
+-rw-r--r--   0        0        0     3122 2023-07-06 13:02:46.428218 tawazi-0.3.1/tawazi/_helpers.py
+-rw-r--r--   0        0        0      487 2023-06-22 08:51:55.500692 tawazi-0.3.1/tawazi/_object_helpers.py
+-rw-r--r--   0        0        0     2481 2023-07-18 12:55:48.248884 tawazi-0.3.1/tawazi/config.py
+-rw-r--r--   0        0        0     3963 2023-07-06 13:02:46.428218 tawazi-0.3.1/tawazi/consts.py
+-rw-r--r--   0        0        0     1862 2023-07-18 10:04:44.370576 tawazi-0.3.1/tawazi/errors.py
+-rw-r--r--   0        0        0      316 2023-06-22 08:51:55.500692 tawazi-0.3.1/tawazi/node/__init__.py
+-rw-r--r--   0        0        0     2866 2023-06-22 08:51:55.500692 tawazi-0.3.1/tawazi/node/functions.py
+-rw-r--r--   0        0        0      994 2023-06-22 08:51:55.500692 tawazi-0.3.1/tawazi/node/helpers.py
+-rw-r--r--   0        0        0    33386 2023-07-18 08:34:51.911775 tawazi-0.3.1/tawazi/node/node.py
+-rw-r--r--   0        0        0     3362 2023-06-22 08:51:55.500692 tawazi-0.3.1/tawazi/profile.py
+-rw-r--r--   0        0        0        0 2023-06-22 08:51:55.500692 tawazi-0.3.1/tawazi/py.typed
+-rw-r--r--   0        0        0       68 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/__init__.py
+-rw-r--r--   0        0        0     3751 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_active.py
+-rw-r--r--   0        0        0     2641 2023-07-06 13:02:46.432218 tawazi-0.3.1/tests/test_behavior.py
+-rw-r--r--   0        0        0     2292 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_build.py
+-rw-r--r--   0        0        0     7666 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_cache_feature.py
+-rw-r--r--   0        0        0     1425 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_compound_priority.py
+-rw-r--r--   0        0        0     4288 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_config.py
+-rw-r--r--   0        0        0     5337 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_dag_compose.py
+-rw-r--r--   0        0        0     1740 2023-07-06 13:02:46.432218 tawazi-0.3.1/tests/test_dag_config.py
+-rw-r--r--   0        0        0     2883 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_dagexecutor.py
+-rw-r--r--   0        0        0     4974 2023-07-18 12:55:48.248884 tawazi-0.3.1/tests/test_debug_nodes.py
+-rw-r--r--   0        0        0      730 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_decorator.py
+-rw-r--r--   0        0        0     1294 2023-07-18 12:55:48.248884 tawazi-0.3.1/tests/test_edge_cases_dag.py
+-rw-r--r--   0        0        0      362 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_error_during_dag_build.py
+-rw-r--r--   0        0        0     4079 2023-07-18 10:03:15.248578 tawazi-0.3.1/tests/test_exclude_nodes.py
+-rw-r--r--   0        0        0      422 2023-07-06 13:02:46.432218 tawazi-0.3.1/tests/test_execution_time.py
+-rw-r--r--   0        0        0     1318 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_graph.py
+-rw-r--r--   0        0        0      610 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_imbricated_dags.py
+-rw-r--r--   0        0        0     2262 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_methods.py
+-rw-r--r--   0        0        0     5791 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_multiple_return_value_for_exec_node.py
+-rw-r--r--   0        0        0     2446 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_multiple_return_value_for_graph.py
+-rw-r--r--   0        0        0      413 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_non_picklable_arguments.py
+-rw-r--r--   0        0        0     2299 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_op.py
+-rw-r--r--   0        0        0    18550 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_operators.py
+-rw-r--r--   0        0        0     2609 2023-07-06 13:02:46.432218 tawazi-0.3.1/tests/test_ops_interface.py
+-rw-r--r--   0        0        0     1410 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_pipeline_input_output.py
+-rw-r--r--   0        0        0     3388 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_priority_sequential.py
+-rw-r--r--   0        0        0     2801 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_profiling.py
+-rw-r--r--   0        0        0     1508 2023-07-06 13:02:46.432218 tawazi-0.3.1/tests/test_resource.py
+-rw-r--r--   0        0        0     2899 2023-07-06 13:02:46.432218 tawazi-0.3.1/tests/test_safe_execution.py
+-rw-r--r--   0        0        0      279 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_same_op_reuse.py
+-rw-r--r--   0        0        0    10318 2023-06-30 01:26:07.246783 tawazi-0.3.1/tests/test_setup_nodes.py
+-rw-r--r--   0        0        0     3592 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_subgraph.py
+-rw-r--r--   0        0        0      909 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_tags.py
+-rw-r--r--   0        0        0     1841 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_typing.py
+-rw-r--r--   0        0        0      776 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/test_wrapped_function.py
+-rw-r--r--   0        0        0        0 2023-06-22 08:51:55.500692 tawazi-0.3.1/tests/tests/__init__.py
+-rw-r--r--   0        0        0     5292 1970-01-01 00:00:00.000000 tawazi-0.3.1/PKG-INFO
```

### Comparing `tawazi-0.3.0/.github/ISSUE_TEMPLATE/bug_report.md` & `tawazi-0.3.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/.github/ISSUE_TEMPLATE/feature_request.md` & `tawazi-0.3.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/.github/PULL_REQUEST_TEMPLATE.md` & `tawazi-0.3.1/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/.github/dependabot.yml` & `tawazi-0.3.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/.github/workflows/documentation-validation-workflow.yml` & `tawazi-0.3.1/.github/workflows/documentation-validation-workflow.yml`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/.github/workflows/formatting-workflow.yml` & `tawazi-0.3.1/.github/workflows/formatting-workflow.yml`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/.github/workflows/testing-workflow.yml` & `tawazi-0.3.1/.github/workflows/testing-workflow.yml`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/.gitignore` & `tawazi-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/.pre-commit-config.yaml` & `tawazi-0.3.1/.pre-commit-config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   - repo: https://github.com/charliermarsh/ruff-pre-commit
     rev: "v0.0.269"
     hooks:
     - id: ruff
       args: ["--fix"]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.1.1
+    rev: v1.4.1
     hooks:
       - id: mypy
         # files:
         args: []
         additional_dependencies:
           - pydantic
           - loguru # to be removed when loguru is removed
```

### Comparing `tawazi-0.3.0/CHANGELOG.md` & `tawazi-0.3.1/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## v0.3.1 (2023-07-18)
+
+### Bug Fixes
+* If a debug ExecNode depends on a variable data, the DAG.setup method hanged forever
+* If a debug ExecNodes are provided the DAG.setup method sometimes fails
+* Tawazi is compatible with pydantic v1 only
+
 ## v0.3.0 (2023-05-31)
 
 ### Improvement
 
 * Run the ExecNode’s function with arbitrary arguments names
 * pass in arguments & return values from created DAGs like normal functions
 * Setup ExecNodes
```

### Comparing `tawazi-0.3.0/CODE_OF_CONDUCT.md` & `tawazi-0.3.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/CONTRIBUTING.md` & `tawazi-0.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/LICENSE` & `tawazi-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/README.md` & `tawazi-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/documentation/future_developments.md` & `tawazi-0.3.1/documentation/future_developments.md`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/documentation/index.md` & `tawazi-0.3.1/documentation/index.md`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/documentation/tawazi_GIF.gif` & `tawazi-0.3.1/documentation/tawazi_GIF.gif`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/example.py` & `tawazi-0.3.1/example.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/mkdocs.yml` & `tawazi-0.3.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/pyproject.toml` & `tawazi-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 
 [project]
 name = "tawazi"
-version = "0.3.0"
+version = "0.3.1"
 description = "This library helps you execute a set of functions in a Directed Acyclic Graph (DAG) dependency structure in parallel in a production environment."
 authors = [{name = "Mindee", email = "contact@mindee.com"}]
 maintainers = [
     {name = "Bashir Abdel Wahed"},
     {name = "Matthias Cremieux"}
 ]
 license = {file = "LICENSE" }
 readme = "README.md"
 requires-python=">=3.7,<4"
 dependencies = [
     "networkx>=2,<4",
-    "pydantic>=1.0",
+    "pydantic~=1.0",
     "loguru",
     "PyYaml>=6",
     "typing_extensions>=3.10"
 ]
 
 [project.optional-dependencies]
 dev = [
@@ -31,15 +31,15 @@
     "pytest-codeblocks"
 ]
 
 doc = [
     "mkdocs>=1.4.0",
     "mike==1.1.2",
     "mkdocs-exclude==1.0.2",
-    "mkdocs-material==9.1.15",
+    "mkdocs-material==9.1.18",
     "mkdocstrings-python"
 ]
 
 [tool.pytest.ini_options]
 addopts = "--pdbcls=IPython.terminal.debugger:TerminalPdb --cov-report=term-missing:skip-covered --junit-xml=pytest-junit.xml --cov=tawazi"
 
 [tool.mypy]
```

### Comparing `tawazi-0.3.0/tawazi/_dag/dag.py` & `tawazi-0.3.1/tawazi/_dag/dag.py`

 * *Files 1% similar despite different names*

```diff
@@ -499,26 +499,46 @@
 
         Returns:
             List[Identifier]: Leaf ExecNodes' Identities
         """
         return list(chain(*(self._alias_to_ids(alias) for alias in target_nodes)))
 
     def _extend_leaves_ids_debug_xns(self, leaves_ids: List[Identifier]) -> List[Identifier]:
+        """Extend the leaves_ids to contain all runnable debug node ids.
+
+        For example:
+        A
+        |
+        B
+        | \
+        D E
+
+        if D is not a debug ExecNode and E is a debug ExecNode.
+        If the subgraph whose leaf ExecNode D is executed,
+        E should also be included in the execution because it can be executed (debug node whose inputs are provided)
+        Hence we should extend the subgraph containing only D to also contain E
+
+        Args:
+            leaves_ids (List[Identifier]): the leaves ids of the subgraph
+
+        Returns:
+            List[Identifier]: the leaves ids of the new extended subgraph that contains more debug ExecNodes
+        """
         new_debug_xn_discovered = True
         while new_debug_xn_discovered:
             new_debug_xn_discovered = False
             for id_ in leaves_ids:
                 for successor_id in self.frwrd_deps[id_]:
                     is_successor_debug = self.node_dict[successor_id].debug
                     if successor_id not in leaves_ids and is_successor_debug:
                         # a new debug XN has been discovered!
-                        new_debug_xn_discovered = True
                         preds_of_succs_ids = [xn_id for xn_id in self.bckrd_deps[successor_id]]
 
                         if set(preds_of_succs_ids).issubset(set(leaves_ids)):
+                            new_debug_xn_discovered = True
                             # this new XN can run by only running the current leaves_ids
                             leaves_ids.append(successor_id)
         return leaves_ids
 
     def setup(
         self,
         target_nodes: Optional[Sequence[Alias]] = None,
@@ -535,19 +555,15 @@
             target_nodes (Optional[List[XNId]], optional): The ExecNodes that the user aims to use in the DAG.
                 This might include setup or non setup ExecNodes. If None is provided, will run all setup ExecNodes. Defaults to None.
             exclude_nodes (Optional[List[XNId]], optional): The ExecNodes that the user aims to exclude from the DAG.
                 The user is responsible for ensuring that the overlapping between the target_nodes and exclude_nodes is logical.
         """
         # 1. select all setup ExecNodes
         #  do not copy the setup nodes because we want them to be modified per DAG instance!
-        all_setup_nodes = {
-            id_: xn
-            for id_, xn in self.node_dict.items()
-            if xn.setup or (isinstance(xn, ArgExecNode) and xn.executed)
-        }
+        all_setup_nodes = {id_: xn for id_, xn in self.node_dict.items() if xn.setup}
 
         # 2. if target_nodes is not provided run all setup ExecNodes
         if target_nodes is None:
             target_ids = list(all_setup_nodes.keys())
             graph = self._make_subgraph(target_ids, exclude_nodes)
 
         else:
@@ -561,15 +577,15 @@
             graph = self._make_subgraph(target_ids, exclude_nodes)
             ids_to_remove = [id_ for id_ in graph if id_ not in all_setup_nodes]
 
             for id_ in ids_to_remove:
                 graph.remove_node(id_)
         # TODO: handle debug XNs!
 
-        self._execute(graph, all_setup_nodes)
+        self._execute(graph)
 
     def executor(self, **kwargs: Any) -> "DAGExecution[P, RVDAG]":
         """Generates a DAGExecution for the DAG.
 
         Args:
             **kwargs (Any): keyword arguments to be passed to DAGExecution's constructor
```

### Comparing `tawazi-0.3.0/tawazi/_dag/digraph.py` & `tawazi-0.3.1/tawazi/_dag/digraph.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tawazi/_dag/helpers.py` & `tawazi-0.3.1/tawazi/_dag/helpers.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tawazi/_decorators.py` & `tawazi-0.3.1/tawazi/_decorators.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tawazi/_helpers.py` & `tawazi-0.3.1/tawazi/_helpers.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tawazi/config.py` & `tawazi-0.3.1/tawazi/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,18 +28,18 @@
     # - "Ignore": do nothing
     TAWAZI_EXECNODE_OUTSIDE_DAG_BEHAVIOR: XNOutsideDAGCall = XNOutsideDAGCall.error
 
     # choose the default Resource to use to execute the ExecNodes
     TAWAZI_DEFAULT_RESOURCE = Resource.thread
 
     # Logger settings
-    LOGURU_LEVEL: str = Field("PROD", env="TAWAZI_LOGGER_LEVEL")
-    LOGURU_BACKTRACE: bool = Field(False, env="TAWAZI_LOGGER_BT")
+    LOGURU_LEVEL: str = Field(default="PROD", env="TAWAZI_LOGGER_LEVEL")
+    LOGURU_BACKTRACE: bool = Field(default=False, env="TAWAZI_LOGGER_BT")
     # Caution: to set to False if used in prod (exposes variable names)
-    LOGURU_DIAGNOSE: bool = Field(False, env="TAWAZI_LOGGER_DIAGNOSE")
+    LOGURU_DIAGNOSE: bool = Field(default=False, env="TAWAZI_LOGGER_DIAGNOSE")
 
     @validator("LOGURU_LEVEL")
     def _validate_loguru_level(cls, v: str) -> str:  # noqa: N805
         if v == "PROD":
             from loguru import logger
 
             logger.disable("tawazi")
@@ -60,8 +60,8 @@
     def _validate_default_resource(cls, v: str) -> str:  # noqa: N805
         accepted_values = Resource.__members__.values()
         if v not in accepted_values:
             raise ValueError(f"TAWAZI_DEFAULT_RESOURCE must be one of {accepted_values}")
         return v
 
 
-cfg = Config()  # type: ignore[call-arg]
+cfg = Config()
```

### Comparing `tawazi-0.3.0/tawazi/consts.py` & `tawazi-0.3.1/tawazi/consts.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tawazi/errors.py` & `tawazi-0.3.1/tawazi/errors.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tawazi/node/functions.py` & `tawazi-0.3.1/tawazi/node/functions.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tawazi/node/helpers.py` & `tawazi-0.3.1/tawazi/node/helpers.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tawazi/node/node.py` & `tawazi-0.3.1/tawazi/node/node.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tawazi/profile.py` & `tawazi-0.3.1/tawazi/profile.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_active.py` & `tawazi-0.3.1/tests/test_active.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_behavior.py` & `tawazi-0.3.1/tests/test_behavior.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_build.py` & `tawazi-0.3.1/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_cache_feature.py` & `tawazi-0.3.1/tests/test_cache_feature.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_compound_priority.py` & `tawazi-0.3.1/tests/test_compound_priority.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_config.py` & `tawazi-0.3.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_dag_compose.py` & `tawazi-0.3.1/tests/test_dag_compose.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_dag_config.py` & `tawazi-0.3.1/tests/test_dag_config.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_dagexecutor.py` & `tawazi-0.3.1/tests/test_dagexecutor.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_debug_nodes.py` & `tawazi-0.3.1/tests/test_debug_nodes.py`

 * *Files 12% similar despite different names*

```diff
@@ -173,10 +173,60 @@
 
     exec_ = pipe.executor(target_nodes=["stub", "incr"])
     assert exec_(0) == 0
     assert print_share_var == 1
     assert inc_shared_var == 1
 
 
+def test_debug_node_depends_on_variable_and_constant() -> None:
+    import tawazi
+
+    tawazi.config.cfg.RUN_DEBUG_NODES = True
+
+    @xn(debug=True)
+    def example1(arg: Any) -> None:
+        pass
+
+    @xn(debug=False)
+    def example2(arg: Any, arg2: Any) -> None:
+        pass
+
+    @xn(debug=True)
+    def example3(arg: Any, arg2: Any) -> None:
+        pass
+
+    @dag
+    def pipeline(docs: Any) -> List[Any]:
+        example1(docs)
+        example2(0, 0)
+        example3(docs, 0)
+        return []
+
+    pipeline.setup()
+
+
+def test_debug_node_with_setup() -> None:
+    import tawazi
+
+    tawazi.config.cfg.RUN_DEBUG_NODES = True
+
+    @xn(debug=True)
+    def example1(arg: Any) -> None:
+        pass
+
+    @xn(debug=False)
+    def example2(arg: Any, arg2: Any) -> None:
+        pass
+
+    @dag
+    def pipeline(docs: Any) -> List[Any]:
+        example1(0)  # replace by example1(docs)
+        example2(0, 0)
+
+        return []
+
+    pipeline.setup()
+
+
 # should this be True ???
 # def test_return_debug_node_value_should_raise_error():
 # pass
```

### Comparing `tawazi-0.3.0/tests/test_decorator.py` & `tawazi-0.3.1/tests/test_decorator.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_edge_cases_dag.py` & `tawazi-0.3.1/tests/test_edge_cases_dag.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     def toto(a: str, b: str) -> str:
         return a + "_wow_" + b
 
     @dag
     def my_dag() -> Tuple[Any, ...]:
         var_a = xn(partial(func, a="x"))(b="y")
         var_b = xn(partial(func, b="y"))(a="x")
-        var_c = xn(lambda x: x)("e")  # type: ignore[no-any-return]
+        var_c = xn(lambda x: x)("e")
         var_d = toto(var_a, var_b)
 
         return var_a, var_b, var_c, var_d
 
     res_a, res_b, res_c, res_d = my_dag()
 
     assert res_a == "xy"
```

### Comparing `tawazi-0.3.0/tests/test_exclude_nodes.py` & `tawazi-0.3.1/tests/test_exclude_nodes.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_graph.py` & `tawazi-0.3.1/tests/test_graph.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_imbricated_dags.py` & `tawazi-0.3.1/tests/test_imbricated_dags.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_methods.py` & `tawazi-0.3.1/tests/test_methods.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_multiple_return_value_for_exec_node.py` & `tawazi-0.3.1/tests/test_multiple_return_value_for_exec_node.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_multiple_return_value_for_graph.py` & `tawazi-0.3.1/tests/test_multiple_return_value_for_graph.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_op.py` & `tawazi-0.3.1/tests/test_op.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_operators.py` & `tawazi-0.3.1/tests/test_operators.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_ops_interface.py` & `tawazi-0.3.1/tests/test_ops_interface.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_pipeline_input_output.py` & `tawazi-0.3.1/tests/test_pipeline_input_output.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_priority_sequential.py` & `tawazi-0.3.1/tests/test_priority_sequential.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_profiling.py` & `tawazi-0.3.1/tests/test_profiling.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_resource.py` & `tawazi-0.3.1/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_safe_execution.py` & `tawazi-0.3.1/tests/test_safe_execution.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_setup_nodes.py` & `tawazi-0.3.1/tests/test_setup_nodes.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_subgraph.py` & `tawazi-0.3.1/tests/test_subgraph.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_tags.py` & `tawazi-0.3.1/tests/test_tags.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_typing.py` & `tawazi-0.3.1/tests/test_typing.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/tests/test_wrapped_function.py` & `tawazi-0.3.1/tests/test_wrapped_function.py`

 * *Files identical despite different names*

### Comparing `tawazi-0.3.0/PKG-INFO` & `tawazi-0.3.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 Metadata-Version: 2.1
 Name: tawazi
-Version: 0.3.0
+Version: 0.3.1
 Summary: This library helps you execute a set of functions in a Directed Acyclic Graph (DAG) dependency structure in parallel in a production environment.
 Author-email: Mindee <contact@mindee.com>
 Maintainer: Bashir Abdel Wahed, Matthias Cremieux
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Requires-Dist: networkx>=2,<4
-Requires-Dist: pydantic>=1.0
+Requires-Dist: pydantic~=1.0
 Requires-Dist: loguru
 Requires-Dist: PyYaml>=6
 Requires-Dist: typing_extensions>=3.10
 Requires-Dist: matplotlib>=3.5.3 ; extra == "dev"
 Requires-Dist: pytest>=7.1.2 ; extra == "dev"
 Requires-Dist: pytest-cov>=4.0.0 ; extra == "dev"
 Requires-Dist: pytest-codeblocks ; extra == "dev"
 Requires-Dist: mkdocs>=1.4.0 ; extra == "doc"
 Requires-Dist: mike==1.1.2 ; extra == "doc"
 Requires-Dist: mkdocs-exclude==1.0.2 ; extra == "doc"
-Requires-Dist: mkdocs-material==9.1.15 ; extra == "doc"
+Requires-Dist: mkdocs-material==9.1.18 ; extra == "doc"
 Requires-Dist: mkdocstrings-python ; extra == "doc"
 Provides-Extra: dev
 Provides-Extra: doc
 
 # tawazi
 <!--Python badges -->
 [![Python 3.7](https://img.shields.io/badge/python-3.7%20|%203.8%20|%203.9%20|%203.10%20|%203.11-blue.svg)](https://www.python.org/)
```

