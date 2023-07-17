# Comparing `tmp/fal-0.9.2.tar.gz` & `tmp/fal-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fal-0.9.2.tar", max compression
+gzip compressed data, was "fal-0.9.3.tar", max compression
```

## Comparing `fal-0.9.2.tar` & `fal-0.9.3.tar`

### file list

```diff
@@ -1,46 +1,90 @@
--rw-r--r--   0        0        0    11804 2023-06-28 15:00:25.701967 fal-0.9.2/README.md
--rw-r--r--   0        0        0     2498 2023-06-28 15:00:40.853979 fal-0.9.2/pyproject.toml
--rw-r--r--   0        0        0      221 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/__init__.py
--rw-r--r--   0        0        0       21 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/cli/__init__.py
--rw-r--r--   0        0        0     7450 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/cli/args.py
--rw-r--r--   0        0        0     1019 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/cli/cli.py
--rw-r--r--   0        0        0     5469 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/cli/dbt_runner.py
--rw-r--r--   0        0        0     5815 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/cli/fal_runner.py
--rw-r--r--   0        0        0     4430 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/cli/flow_runner.py
--rw-r--r--   0        0        0       56 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/cli/model_generator/__init__.py
--rw-r--r--   0        0        0     5505 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/cli/model_generator/model_generator.py
--rw-r--r--   0        0        0     3180 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/cli/model_generator/module_check.py
--rw-r--r--   0        0        0     9742 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/cli/selectors.py
--rw-r--r--   0        0        0    12306 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/fal_script.py
--rw-r--r--   0        0        0        0 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/feature_store/__init__.py
--rw-r--r--   0        0        0      401 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/feature_store/feature.py
--rw-r--r--   0        0        0     8394 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/node_graph.py
--rw-r--r--   0        0        0        0 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/packages/__init__.py
--rw-r--r--   0        0        0     1603 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/packages/bridge.py
--rw-r--r--   0        0        0     5332 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/packages/dependency_analysis.py
--rw-r--r--   0        0        0      793 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/packages/environments/__init__.py
--rw-r--r--   0        0        0     9482 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/packages/environments/base.py
--rw-r--r--   0        0        0     4395 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/packages/environments/conda.py
--rw-r--r--   0        0        0     3369 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/packages/environments/virtual_env.py
--rw-r--r--   0        0        0     4776 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/packages/isolated_runner.py
--rw-r--r--   0        0        0        0 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/planner/__init__.py
--rw-r--r--   0        0        0     5635 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/planner/executor.py
--rw-r--r--   0        0        0     6475 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/planner/plan.py
--rw-r--r--   0        0        0     6761 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/planner/schedule.py
--rw-r--r--   0        0        0     9041 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/planner/tasks.py
--rw-r--r--   0        0        0        0 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/telemetry/__init__.py
--rw-r--r--   0        0        0    11416 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/telemetry/telemetry.py
--rw-r--r--   0        0        0     3043 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/typing.py
--rw-r--r--   0        0        0     1711 2023-06-28 15:00:25.713967 fal-0.9.2/src/fal/utils.py
--rw-r--r--   0        0        0        0 2023-06-28 15:00:25.713967 fal-0.9.2/src/faldbt/__init__.py
--rw-r--r--   0        0        0    24563 2023-06-28 15:00:25.713967 fal-0.9.2/src/faldbt/lib.py
--rw-r--r--   0        0        0     3273 2023-06-28 15:00:25.713967 fal-0.9.2/src/faldbt/logger.py
--rw-r--r--   0        0        0     1850 2023-06-28 15:00:25.713967 fal-0.9.2/src/faldbt/magics.py
--rw-r--r--   0        0        0     9057 2023-06-28 15:00:25.713967 fal-0.9.2/src/faldbt/parse.py
--rw-r--r--   0        0        0    27131 2023-06-28 15:00:25.713967 fal-0.9.2/src/faldbt/project.py
--rw-r--r--   0        0        0        0 2023-06-28 15:00:25.713967 fal-0.9.2/src/faldbt/utils/__init__.py
--rw-r--r--   0        0        0     1970 2023-06-28 15:00:25.713967 fal-0.9.2/src/faldbt/utils/yaml_helper.py
--rw-r--r--   0        0        0      317 2023-06-28 15:00:25.713967 fal-0.9.2/src/faldbt/version.py
--rw-r--r--   0        0        0       33 2023-06-28 15:00:25.713967 fal-0.9.2/tests/_fal_testing/__init__.py
--rw-r--r--   0        0        0     1786 2023-06-28 15:00:25.713967 fal-0.9.2/tests/_fal_testing/utils.py
--rw-r--r--   0        0        0    13982 1970-01-01 00:00:00.000000 fal-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0    10531 2023-07-17 22:13:58.416296 fal-0.9.3/README.md
+-rw-r--r--   0        0        0     2352 2023-07-17 22:14:12.652501 fal-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0      639 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal/__init__.py
+-rw-r--r--   0        0        0       18 2023-07-17 22:14:13.156509 fal-0.9.3/src/dbt/adapters/fal/__version__.py
+-rw-r--r--   0        0        0      392 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal/connections.py
+-rw-r--r--   0        0        0     3369 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal/impl.py
+-rw-r--r--   0        0        0     2768 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal/load_db_profile.py
+-rw-r--r--   0        0        0     4091 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal/wrappers.py
+-rw-r--r--   0        0        0      344 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/__init__.py
+-rw-r--r--   0        0        0       18 2023-07-17 22:14:13.156509 fal-0.9.3/src/dbt/adapters/fal_experimental/__version__.py
+-rw-r--r--   0        0        0     4861 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/adapter.py
+-rw-r--r--   0        0        0     8381 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/adapter_support.py
+-rw-r--r--   0        0        0     1627 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/connections.py
+-rw-r--r--   0        0        0     8714 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/impl.py
+-rw-r--r--   0        0        0     3192 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/support/athena.py
+-rw-r--r--   0        0        0     2686 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/support/bigquery.py
+-rw-r--r--   0        0        0      980 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/support/duckdb.py
+-rw-r--r--   0        0        0     2977 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/support/postgres.py
+-rw-r--r--   0        0        0     1633 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/support/redshift.py
+-rw-r--r--   0        0        0     2781 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/support/snowflake.py
+-rw-r--r--   0        0        0      821 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/support/trino.py
+-rw-r--r--   0        0        0       25 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/telemetry/__init__.py
+-rw-r--r--   0        0        0    10767 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/telemetry/telemetry.py
+-rw-r--r--   0        0        0     6572 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/teleport.py
+-rw-r--r--   0        0        0     1153 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/teleport_adapter_support.py
+-rw-r--r--   0        0        0     4719 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/teleport_support/duckdb.py
+-rw-r--r--   0        0        0     2972 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/teleport_support/snowflake.py
+-rw-r--r--   0        0        0     1256 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/utils/__init__.py
+-rw-r--r--   0        0        0     9804 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/utils/environments.py
+-rw-r--r--   0        0        0     1970 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/adapters/fal_experimental/utils/yaml_helper.py
+-rw-r--r--   0        0        0      208 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/fal/adapters/python/__init__.py
+-rw-r--r--   0        0        0    11898 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/fal/adapters/python/connections.py
+-rw-r--r--   0        0        0    10015 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/fal/adapters/python/impl.py
+-rw-r--r--   0        0        0      181 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/fal/adapters/teleport/__init__.py
+-rw-r--r--   0        0        0     3498 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/fal/adapters/teleport/impl.py
+-rw-r--r--   0        0        0     2310 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/fal/adapters/teleport/info.py
+-rw-r--r--   0        0        0       52 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/include/fal/__init__.py
+-rw-r--r--   0        0        0       70 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/include/fal/dbt_project.yml
+-rw-r--r--   0        0        0     1213 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/include/fal/macros/materializations/table.sql
+-rw-r--r--   0        0        0      265 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/include/fal/macros/teleport_duckdb.sql
+-rw-r--r--   0        0        0      921 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/include/fal/macros/teleport_snowflake.sql
+-rw-r--r--   0        0        0       52 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/include/fal_experimental/__init__.py
+-rw-r--r--   0        0        0       83 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/include/fal_experimental/dbt_project.yml
+-rw-r--r--   0        0        0      989 2023-07-17 22:13:58.428296 fal-0.9.3/src/dbt/include/fal_experimental/macros/materializations/table.sql
+-rw-r--r--   0        0        0     1829 2023-07-17 22:13:58.428296 fal-0.9.3/src/fal/__init__.py
+-rw-r--r--   0        0        0      238 2023-07-17 22:13:58.428296 fal-0.9.3/src/fal/dbt/__init__.py
+-rw-r--r--   0        0        0       30 2023-07-17 22:13:58.428296 fal-0.9.3/src/fal/dbt/cli/__init__.py
+-rw-r--r--   0        0        0     7458 2023-07-17 22:13:58.428296 fal-0.9.3/src/fal/dbt/cli/args.py
+-rw-r--r--   0        0        0     1432 2023-07-17 22:13:58.428296 fal-0.9.3/src/fal/dbt/cli/cli.py
+-rw-r--r--   0        0        0     5482 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/cli/dbt_runner.py
+-rw-r--r--   0        0        0     5857 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/cli/fal_runner.py
+-rw-r--r--   0        0        0     4475 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/cli/flow_runner.py
+-rw-r--r--   0        0        0       56 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/cli/model_generator/__init__.py
+-rw-r--r--   0        0        0     5543 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/cli/model_generator/model_generator.py
+-rw-r--r--   0        0        0     3180 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/cli/model_generator/module_check.py
+-rw-r--r--   0        0        0     9759 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/cli/selectors.py
+-rw-r--r--   0        0        0    12349 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/fal_script.py
+-rw-r--r--   0        0        0        0 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/feature_store/__init__.py
+-rw-r--r--   0        0        0      401 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/feature_store/feature.py
+-rw-r--r--   0        0        0        0 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/integration/__init__.py
+-rw-r--r--   0        0        0    24589 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/integration/lib.py
+-rw-r--r--   0        0        0     3273 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/integration/logger.py
+-rw-r--r--   0        0        0     1867 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/integration/magics.py
+-rw-r--r--   0        0        0     9103 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/integration/parse.py
+-rw-r--r--   0        0        0    27168 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/integration/project.py
+-rw-r--r--   0        0        0        0 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/integration/utils/__init__.py
+-rw-r--r--   0        0        0     1970 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/integration/utils/yaml_helper.py
+-rw-r--r--   0        0        0      317 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/integration/version.py
+-rw-r--r--   0        0        0     1530 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/new/project.py
+-rw-r--r--   0        0        0     8411 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/node_graph.py
+-rw-r--r--   0        0        0        0 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/packages/__init__.py
+-rw-r--r--   0        0        0     1603 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/packages/bridge.py
+-rw-r--r--   0        0        0     4948 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/packages/dependency_analysis.py
+-rw-r--r--   0        0        0      805 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/packages/environments/__init__.py
+-rw-r--r--   0        0        0     9499 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/packages/environments/base.py
+-rw-r--r--   0        0        0     4407 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/packages/environments/conda.py
+-rw-r--r--   0        0        0     3381 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/packages/environments/virtual_env.py
+-rw-r--r--   0        0        0     4823 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/packages/isolated_runner.py
+-rw-r--r--   0        0        0        0 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/planner/__init__.py
+-rw-r--r--   0        0        0     5669 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/planner/executor.py
+-rw-r--r--   0        0        0     6496 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/planner/plan.py
+-rw-r--r--   0        0        0     6790 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/planner/schedule.py
+-rw-r--r--   0        0        0     9079 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/planner/tasks.py
+-rw-r--r--   0        0        0        0 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/telemetry/__init__.py
+-rw-r--r--   0        0        0    11441 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/telemetry/telemetry.py
+-rw-r--r--   0        0        0     3060 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/typing.py
+-rw-r--r--   0        0        0     1728 2023-07-17 22:13:58.432296 fal-0.9.3/src/fal/dbt/utils.py
+-rw-r--r--   0        0        0       33 2023-07-17 22:13:58.432296 fal-0.9.3/tests/_fal_testing/__init__.py
+-rw-r--r--   0        0        0     1794 2023-07-17 22:13:58.432296 fal-0.9.3/tests/_fal_testing/utils.py
+-rw-r--r--   0        0        0    12552 1970-01-01 00:00:00.000000 fal-0.9.3/PKG-INFO
```

### Comparing `fal-0.9.2/README.md` & `fal-0.9.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,99 @@
-<!-- <base href="https://github.com/fal-ai/fal/blob/-/projects/fal/" target="_blank" /> -->
+<!-- <base href="https://github.com/fal-ai/fal/blob/-/projects/adapter/" target="_blank" /> -->
 
-# fal: do more with dbt
+# Welcome to dbt-fal 👋 do more with dbt
 
-fal is the easiest way to run Python with your [dbt](https://www.getdbt.com/) project.
+dbt-fal adapter is the ✨easiest✨ way to run your [dbt Python models](https://docs.getdbt.com/docs/building-a-dbt-project/building-models/python-models).
 
-# Introduction
+Starting with dbt v1.3, you can now build your dbt models in Python. This leads to some cool use cases that was once difficult to build with SQL alone. Some examples are:
 
-With the `fal` CLI, you can:
+- Using Python stats libraries to calculate stats
+- Building forecasts
+- Building other predictive models such as classification and clustering
+
+This is fantastic! BUT, there is still one issue though! The developer experience with Snowflake and Bigquery is not great, and there is no Python support for Redshift and Postgres.
+
+dbt-fal provides the best environment to run your Python models that works with all other data warehouses! With dbt-fal, you can:
+
+- Build and test your models locally
+- Isolate each model to run in its own environment with its own dependencies
+- [Coming Soon] Run your Python models in the ☁️ cloud ☁️ with elasticly scaling Python environments.
+- [Coming Soon] Even add GPUs to your models for some heavier workloads such as training ML models.
+
+## Getting Started
+
+### 1. Install dbt-fal
+`pip install dbt-fal[bigquery,snowflake]` *Add your current warehouse here*
+
+### 2. Update your `profiles.yml` and add the fal adapter
+
+```yaml
+jaffle_shop:
+  target: dev_with_fal
+  outputs:
+    dev_with_fal:
+      type: fal
+      db_profile: dev_bigquery # This points to your main adapter
+    dev_bigquery:
+      type: bigquery
+      ...
+```
+
+Don't forget to point to your main adapter with the `db_profile` attribute. This is how the fal adapter knows how to connect to your data warehouse.
+
+### 3. `dbt run`!
+That is it! It is really that simple 😊
+
+### 4. [🚨 Cool Feature Alert 🚨] Environment management with dbt-fal
+If you want some help with environment management (vs sticking to the default env that the dbt process runs in), you can create a fal_project.yml in the same folder as your dbt project and have “named environments”:
+
+In your dbt project folder:
+```bash
+$ touch fal_project.yml
+
+# Paste the config below
+environments:
+  - name: ml
+    type: venv
+    requirements:
+      - prophet
+```
+
+and then in your dbt model:
+
+```bash
+$ vi models/orders_forecast.py
+
+def model(dbt, fal):
+    dbt.config(fal_environment="ml") # Add this line
+
+    df: pd.DataFrame = dbt.ref("orders_daily")
+```
+
+The `dbt.config(fal_environment=“ml”)` will give you an isolated clean env to run things in, so you dont pollute your package space.
+
+### 5. [Coming Soon™️] Move your compute to the Cloud!
+Let us know if you are interested in this. We are looking for beta users.
+
+# `dbt-fal` command line tool
+
+With the `dbt-fal` CLI, you can:
 
 - [Send Slack notifications](https://github.com/fal-ai/fal/blob/-/examples/slack-example) upon dbt model success or failure.
 - [Load data from external data sources](https://blog.fal.ai/populate-dbt-models-with-csv-data/) before a model starts running.
 - [Download dbt models](https://docs.fal.ai/fal/python-package) into a Python context with a familiar syntax: `ref('my_dbt_model')` using `FalDbt`
 - [Programatically access rich metadata](https://docs.fal.ai/fal/reference/variables-and-functions) about your dbt project.
 
 Head to our [documentation site](https://docs.fal.ai/) for a deeper dive or play with [in-depth examples](https://github.com/fal-ai/fal/blob/-/examples/README.md) to see how fal can help you get more done with dbt.
 
-> ❗️ If you would like to write data back to your data-warehouse, we recommend using the [`dbt-fal`](https://pypi.org/project/dbt-fal/) adapter.
 
-# Getting Started
-
-## 1. Install `fal`
+## 1. Install `dbt-fal`
 
 ```bash
-$ pip install fal
+$ pip install dbt-fal[postgres]
 ```
 
 ## 2. Go to your dbt project directory
 
 ```bash
 $ cd ~/src/my_dbt_project
 ```
@@ -68,65 +135,31 @@
         description: Date
     meta:
       fal:
         scripts:
           - send_slack_message.py
 ```
 
-## 5. Run `fal flow run`
+## 5. Run `dbt-fal flow run`
 
 ```bash
-$ fal flow run
-# both your dbt models and fal scripts are run
+$ dbt-fal flow run
+# both your dbt models and python scripts are run
 ```
 
 ## 6. Alternatively run `dbt` and `fal` consecutively
 
 ```bash
 $ dbt run
 # Your dbt models are run
 
-$ fal run
+$ dbt-fal run
 # Your python scripts are run
 ```
 
-# Examples
-
-To explore what is possible with fal, take a look at the in-depth examples below. We will be adding more examples here over time:
-
-- [Example 1: Send Slack notifications](https://github.com/fal-ai/fal/blob/-/examples/slack-example/README.md)
-- [Example 2: Use dbt from a Jupyter Notebook](https://github.com/fal-ai/fal/blob/-/examples/write_jupyter_notebook/README.md)
-- [Example 3: Read and parse dbt metadata](https://github.com/fal-ai/fal/blob/-/examples/read_dbt_metadata/README.md)
-- [Example 4: Metric forecasting](https://github.com/fal-ai/fal/blob/-/examples/metric-forecast/README.md)
-- [Example 5: Sentiment analysis on support tickets](https://github.com/fal-ai/fal/blob/-/examples/sentiment-analysis/README.md)
-- [Example 6: Anomaly Detection](https://github.com/fal-ai/fal/blob/-/examples/anomaly-detection/README.md)
-- [Example 7: Incorporate fal in CI/CD workflow](https://github.com/fal-ai/fal/blob/-/examples/ci_example/README.md)
-- [Example 8: Send events to Datadog](https://github.com/fal-ai/fal/blob/-/examples/datadog_event/README.md)
-- [Example 9: Write dbt artifacts to GCS](https://github.com/fal-ai/fal/blob/-/examples/write_to_gcs/README.md)
-- [Example 10: Write dbt artifacts to AWS S3](https://github.com/fal-ai/fal/blob/-/examples/write_to_aws/README.md)
-
-[Check out the examples directory for more](https://github.com/fal-ai/fal/blob/-/examples/README.md)
-
-# How it works?
-
-`fal` is a command line tool that can read the state of your `dbt` project and help you run Python scripts after your `dbt run`s by leveraging the [`meta` config](https://docs.getdbt.com/reference/resource-configs/meta).
-
-```yaml
-models:
-  - name: historical_ozone_levels
-    ...
-    meta:
-      fal:
-        post-hook:
-          # scripts will run concurrently
-          - send_slack_message.py
-          - another_python_script.py
-```
-
-`fal` also provides useful helpers within the Python context to seamlessly interact with dbt models: `ref("my_dbt_model_name")` will pull a dbt model into your Python script as a [`pandas.DataFrame`](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html).
 
 ## Running scripts before dbt runs
 
 Run scripts before the model runs by using the `pre-hook:` configuration option.
 
 Given the following schema.yml:
 
@@ -141,19 +174,19 @@
       fal:
         pre-hook:
           - fal_scripts/trigger_fivetran.py
         post-hook:
           - fal_scripts/slack.py
 ```
 
-`fal flow run` will run `fal_scripts/trigger_fivetran.py`, then the `boston` dbt model, and finally `fal_scripts/slack.py`.
+`dbt-fal flow run` will run `fal_scripts/trigger_fivetran.py`, then the `boston` dbt model, and finally `fal_scripts/slack.py`.
 If a model is selected with a selection flag (e.g. `--select boston`), the hooks associated to the model will always run with it.
 
 ```bash
-$ fal flow run --select boston
+$ dbt-fal flow run --select boston
 ```
 
 # Concepts
 
 ## profile.yml and Credentials
 
 `fal` integrates with `dbt`'s `profile.yml` file to access and read data from the data warehouse. Once you setup credentials in your `profile.yml` file for your existing `dbt` workflows anytime you use `ref` or `source` to create a dataframe `fal` authenticates using the credentials specified in the `profile.yml` file.
@@ -256,21 +289,22 @@
 ```python
 from sqlalchemy.types import Integer
 # Upload but specifically create the `value` column with type `integer`
 # Can be useful if data has `None` values
 write_to_model(df, dtype={'value': Integer()})
 ```
 
+
 ## Importing `fal` as a Python package
 
 You may be interested in accessing dbt models and sources easily from a Jupyter Notebook or another Python script.
 For that, just import the `fal` package and intantiate a FalDbt project:
 
 ```py
-from fal import FalDbt
+from fal.dbt import FalDbt
 faldbt = FalDbt(profiles_dir="~/.dbt", project_dir="../my_project")
 
 faldbt.list_sources()
 # [
 #    DbtSource(name='results' ...),
 #    DbtSource(name='ticket_data_sentiment_analysis' ...)
 #    ...
@@ -286,66 +320,17 @@
 
 sentiments = faldbt.source('results', 'ticket_data_sentiment_analysis')
 # pandas.DataFrame
 tickets = faldbt.ref('stg_zendesk_ticket_data')
 # pandas.DataFrame
 ```
 
-# Supported `dbt` versions
-
-The latest `fal` version currently supports dbt `1.4.*`.
-
-If you need another version, [open an issue](https://github.com/fal-ai/fal/issues/new) and we will take a look!
-
-# Contributing / Development
-
-We use Poetry for dependency management and easy development testing.
-
-Use Poetry shell to trying your changes right away:
-
-```sh
-~ $ cd fal
-
-~/fal $ poetry install
-
-~/fal $ poetry shell
-Spawning shell within [...]/fal-eFX98vrn-py3.8
-
-~/fal fal-eFX98vrn-py3.8 $ cd ../dbt_project
-
-~/dbt_project fal-eFX98vrn-py3.8 $ fal flow run
-19:27:30  Found 5 models, 0 tests, 0 snapshots, 0 analyses, 165 macros, 0 operations, 0 seed files, 1 source, 0 exposures, 0 metrics
-19:27:30 | Starting fal run for following models and scripts:
-[...]
-```
-
-## Running tests
-
-Tests rely on a Postgres database to be present, this can be achieved with docker-compose:
-
-```sh
-~/fal $ docker-compose -f tests/docker-compose.yml up -d
-Creating network "tests_default" with the default driver
-Creating fal_db ... done
-
-# Necessary for the import test
-~/fal $ dbt run --profiles-dir tests/mock/mockProfile --project-dir tests/mock
-Running with dbt=1.0.1
-[...]
-Completed successfully
-Done. PASS=5 WARN=0 ERROR=0 SKIP=0 TOTAL=5
-
-~/fal $ pytest -s
-```
-
 # Why are we building this?
 
 We think `dbt` is great because it empowers data people to get more done with the tools that they are already familiar with.
 
-`dbt`'s SQL only design is powerful, but if you ever want to get out of SQL-land and connect to external services or get into Python-land for any reason, you will have a hard time. We built `fal` to enable Python workloads (sending alerts to Slack, building predictive models, pushing data to non-data-warehouse destinations and more) **right within `dbt`**.
-
 This library will form the basis of our attempt to more comprehensively enable **data science workloads** downstream of `dbt`. And because having reliable data pipelines is the most important ingredient in building predictive analytics, we are building a library that integrates well with dbt.
 
 # Have feedback or need help?
 
 - Join us in [fal on Discord](https://discord.com/invite/Fyc9PwrccF)
 - Join the [dbt Community](http://community.getdbt.com/) and go into our [#tools-fal channel](https://getdbt.slack.com/archives/C02V8QW3Q4Q)
```

### Comparing `fal-0.9.2/pyproject.toml` & `fal-0.9.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,95 +1,99 @@
 [tool.poetry]
 name = "fal"
-version = "0.9.2"
-description = "fal allows you to run python scripts directly from your dbt project."
-homepage = "https://github.com/fal-ai/fal/blob/-/projects/fal"
-documentation = "https://docs.fal.ai"
-repository = "https://github.com/fal-ai/fal"
+version = "0.9.3"
+description = "Run python scripts from any dbt project."
 readme = "README.md"
+homepage = "https://github.com/fal-ai/fal"
+repository = "https://github.com/fal-ai/fal"
 authors = [ "Features & Labels <hello@fal.ai>" ]
 packages = [
+    { include = "dbt", from = "src" },
+    # cli package
     { include = "fal", from = "src" },
-    { include = "faldbt", from = "src" },
-    { include = "_fal_testing", from = "tests" }
+    { include = "_fal_testing", from = "tests" },
 ]
 
-keywords = [ "dbt", "pandas" ]
+keywords = [ "dbt", "pandas", "fal", "runtime" ]
 classifiers = [
     "Development Status :: 4 - Beta"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7.2, <3.12"
 dbt-core = ">=1.5,<=1.5.1"
 pandas = "^1.3.4"
+posthog = "^1.4.5"
+"backports.functools_lru_cache" = "^1.6.4"
+
+# cli
 PyYAML = "^6.0"
 agate-sql = "^0.5.8"
-requests = "^2.27.1"
-posthog = "^1.4.5"
 astor = "^0.8.1"
 deprecation = "^2.1.0"
-"backports.functools_lru_cache" = "^1.6.4"
 
-# Environment management related dependencies
+## Environment management related dependencies
+## TODO use fal-serverless instead
 platformdirs = "^2.5.2"
 virtualenv = "^20.16.2"
 dill = ">=0.3.6,<0.3.7"
-importlib-metadata = ">=4.12.0"
-packaging = ">20.9"
+
+# dbt-fal
+sqlalchemy = "^1.4.41"
 
 # Adapters
 
 ## snowflake
 snowflake-connector-python = { version = "~=3.0", extras = ["pandas"], optional = true }
 
 ## bigquery
 ### version defined by dbt-bigquery, installs pyarrow<8
 google-cloud-bigquery = { version = "~3.5.0", extras = ["pandas"], optional = true }
 
 ## redshift
+awswrangler = { version = ">=3.0.0", extras = ["redshift"], optional = true, python = ">=3.8" }
 sqlalchemy-redshift = { version = "^0.8.9", optional = true }
 
 ## duckdb
 duckdb-engine = { version = "^0.1.8", optional = true }
 
-# dev
-pytest = { version = "^5.2", optional = true }
-black = { version = "^22.3", optional = true }
-behave = { version = "^1.2.6", optional = true }
-mock = { version = "^4.0.3", optional = true }
-pytest-mock = { version = "^3.7.0", optional = true }
-matplotlib = { version = "^3.5.2", optional = true }
+## trino
+trino = { version = "~0.321.0", extras = ["sqlalchemy"], optional = true }
+
+# teleport
+s3fs = { version = ">=2022.8.2", optional = true }
+
+# fal cloud
+packaging = ">=23"
+fal-serverless = "^0.6.35"
+importlib-metadata = "^6.0.0"
 
 [tool.poetry.extras]
 postgres = []
 snowflake = ["snowflake-connector-python"]
 bigquery = ["google-cloud-bigquery"]
-redshift = ["sqlalchemy-redshift"]
+redshift = ["awswrangler", "sqlalchemy-redshift"]
 duckdb = ["duckdb-engine"]
 athena = []
-test = [
-    "pytest",
-    "black",
-    "behave",
-    "mock",
-    "pytest-mock",
-]
-dev = [
-    "matplotlib"
-]
-cloud = []
+trino = ["trino"]
+teleport = ["s3fs"]
+
+[tool.poetry.group.dev]
+optional = true
 
-[tool.poetry.dev-dependencies]
-pytest = { version = "^5.2", optional = true }
-black = { version = "^22.3", optional = true }
-behave = { version = "^1.2.6", optional = true }
-mock = { version = "^4.0.3", optional = true }
-pytest-mock = { version = "^3.7.0", optional = true }
-matplotlib = { version = "^3.5.2", optional = true }
+[tool.poetry.group.dev.dependencies]
+pytest = "^5.2"
+black = "^22.3"
+behave = "^1.2.6"
+mock = "^4.0.3"
+pytest-mock = "^3.7.0"
+matplotlib = "^3.5.2"
+requests = "^2.27.1"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
-fal = "fal.cli:cli"
+dbt-fal = "fal.dbt.cli:cli"
+# NOTE: deprecated use
+fal = "fal.dbt.cli:fal_cli"
```

### Comparing `fal-0.9.2/src/fal/cli/args.py` & `fal-0.9.3/src/fal/dbt/cli/args.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,19 +200,19 @@
     _add_vars_option(flow_run_parser)
     _add_target_option(flow_run_parser)
     _add_full_refresh_option(flow_run_parser)
 
 
 def _build_cli_parser():
     parser = argparse.ArgumentParser(
-        prog="fal",
+        prog="dbt-fal",
         description="Run Python scripts on dbt models",
     )
 
-    version = pkg_resources.get_distribution("fal").version
+    version = pkg_resources.get_distribution("dbt-fal").version
     parser.add_argument(
         "-v",
         "--version",
         action="version",
         version=f"fal {version}",
         help="show fal version",
     )
```

### Comparing `fal-0.9.2/src/fal/cli/dbt_runner.py` & `fal-0.9.3/src/fal/dbt/cli/dbt_runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import multiprocessing
 from multiprocessing.connection import Connection
 from typing import Any, Dict, Optional, List
 import warnings
 import json
-from faldbt.logger import LOGGER
+from fal.dbt.integration.logger import LOGGER
 import os
 import argparse
 
 
 class DbtCliOutput:
     def __init__(
         self,
```

### Comparing `fal-0.9.2/src/fal/cli/fal_runner.py` & `fal-0.9.3/src/fal/dbt/cli/fal_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import argparse
 from pathlib import Path
 from typing import Any, Dict, List
 
-from fal.planner.executor import parallel_executor
-from fal.planner.schedule import Scheduler
-from fal.planner.tasks import FalLocalHookTask, Status, TaskGroup
+from fal.dbt.planner.executor import parallel_executor
+from fal.dbt.planner.schedule import Scheduler
+from fal.dbt.planner.tasks import FalLocalHookTask, Status, TaskGroup
 
-from fal.fal_script import FalScript, TimingType
-from faldbt.project import FAL, DbtModel, FalDbt, FalGeneralException
+from fal.dbt.fal_script import FalScript, TimingType
+from fal.dbt.integration.project import FAL, DbtModel, FalDbt, FalGeneralException
 
 
 def create_fal_dbt(
     args: argparse.Namespace, generated_models: Dict[str, Path] = {}
 ) -> FalDbt:
     real_state = None
     if hasattr(args, "state") and args.state is not None:
@@ -147,15 +147,15 @@
 
     if (
         not all
         and not selected
         and not before
         and faldbt._run_results.native_run_result is None
     ):
-        from faldbt.parse import FalParseError
+        from fal.dbt.integration.parse import FalParseError
 
         raise FalParseError(
             "Cannot define models to run without selection flags or dbt run_results artifact or --before flag"
         )
 
     models = _get_models_with_keyword(faldbt)
```

### Comparing `fal-0.9.2/src/fal/cli/flow_runner.py` & `fal-0.9.3/src/fal/dbt/cli/flow_runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 import json
 import copy
 from pathlib import Path
 from typing import Any, Dict, Optional, cast, Union
 
-from fal.cli.fal_runner import create_fal_dbt
-from fal.cli.selectors import ExecutionPlan
-from fal.cli.model_generator import generate_python_dbt_models
-from fal.fal_script import FalScript
-from fal.node_graph import DbtModelNode, FalFlowNode, NodeGraph, ScriptNode
-from faldbt.project import FalDbt, NodeStatus
+from fal.dbt.cli.fal_runner import create_fal_dbt
+from fal.dbt.cli.selectors import ExecutionPlan
+from fal.dbt.cli.model_generator import generate_python_dbt_models
+from fal.dbt.fal_script import FalScript
+from fal.dbt.node_graph import DbtModelNode, FalFlowNode, NodeGraph, ScriptNode
+from fal.dbt.integration.project import FalDbt, NodeStatus
 import argparse
 
 
 DBT_RUN_RESULTS_FILENAME = "run_results.json"
 FAL_RUN_RESULTS_FILENAME = "fal_results.json"
 RUN_RESULTS_KEY = "results"
 ELAPSED_TIME_KEY = "elapsed_time"
 
 
 def run_threaded(
     fal_dbt: FalDbt,
     parsed: argparse.Namespace,
     node_graph: NodeGraph,
 ) -> int:
-    from fal.planner.plan import (
+    from fal.dbt.planner.plan import (
         OriginGraph,
         FilteredGraph,
         PlannedGraph,
         ScriptConnectedGraph,
     )
-    from fal.planner.schedule import schedule_graph
-    from fal.planner.executor import parallel_executor
+    from fal.dbt.planner.schedule import schedule_graph
+    from fal.dbt.planner.executor import parallel_executor
 
     execution_plan = ExecutionPlan.create_plan_from_graph(parsed, node_graph, fal_dbt)
 
     origin_graph = OriginGraph(node_graph.graph)
     filtered_graph = FilteredGraph.from_execution_plan(
         origin_graph, execution_plan=execution_plan
     )
```

### Comparing `fal-0.9.2/src/fal/cli/model_generator/model_generator.py` & `fal-0.9.3/src/fal/dbt/cli/model_generator/model_generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 import ast
 from functools import partial
 import re
 from typing import Callable, Iterable, List, TypeVar
 from pathlib import Path
-from fal.fal_script import python_from_file
+from fal.dbt.fal_script import python_from_file
 
-from faldbt.parse import get_fal_models_dirs, load_dbt_project_contract
-from fal.cli.model_generator.module_check import (
+from fal.dbt.integration.parse import get_fal_models_dirs, load_dbt_project_contract
+from fal.dbt.cli.model_generator.module_check import (
     generate_dbt_dependencies,
     write_to_model_check,
 )
 
-from faldbt.logger import LOGGER
+from fal.dbt.integration.logger import LOGGER
 
-from fal.telemetry import telemetry
+from fal.dbt.telemetry import telemetry
 
 SQL_MODEL_TEMPLATE = """
 {{ config(materialized='ephemeral') }}
 /*
 FAL_GENERATED __checksum__
 
 Script dependencies:
```

### Comparing `fal-0.9.2/src/fal/cli/model_generator/module_check.py` & `fal-0.9.3/src/fal/dbt/cli/model_generator/module_check.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.2/src/fal/cli/selectors.py` & `fal-0.9.3/src/fal/dbt/cli/selectors.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import itertools
 import re
 from dataclasses import dataclass
 from typing import List, Optional, Union, Iterator
-from fal.node_graph import NodeGraph
-from faldbt.project import CompileArgs, FalDbt, FalGeneralException
+from fal.dbt.node_graph import NodeGraph
+from fal.dbt.integration.project import CompileArgs, FalDbt, FalGeneralException
 from dbt.task.compile import CompileTask
 from enum import Enum
 from functools import reduce
 import networkx as nx
 
 
 class ExecutionPlan:
```

### Comparing `fal-0.9.2/src/fal/fal_script.py` & `fal-0.9.3/src/fal/dbt/fal_script.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,22 +5,22 @@
 from pathlib import Path
 from functools import partial
 from dataclasses import dataclass, field
 from deprecation import deprecated
 
 import hashlib
 
-from faldbt.parse import normalize_path
-from faldbt.project import DbtModel, FalDbt, FAL
+from fal.dbt.integration.parse import normalize_path
+from fal.dbt.integration.project import DbtModel, FalDbt, FAL
 
 from dbt.contracts.results import RunStatus
 from dbt.config.runtime import RuntimeConfig
-from faldbt.logger import LOGGER
+from fal.dbt.integration.logger import LOGGER
 
-from fal.telemetry import telemetry
+from fal.dbt.telemetry import telemetry
 
 from dbt.contracts.graph.nodes import ColumnInfo
 
 
 class TimingType(Enum):
     PRE = "pre"
     POST = "post"
```

### Comparing `fal-0.9.2/src/fal/node_graph.py` & `fal-0.9.3/src/fal/dbt/node_graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 from dataclasses import dataclass
 from typing import List, Tuple, Dict, cast
 
-from fal.fal_script import FalScript, TimingType
-from faldbt.project import DbtModel, FalDbt
+from fal.dbt.fal_script import FalScript, TimingType
+from fal.dbt.integration.project import DbtModel, FalDbt
 from pathlib import Path
 import networkx as nx
 import os as os
 from functools import reduce
 from enum import Enum
```

### Comparing `fal-0.9.2/src/fal/packages/bridge.py` & `fal-0.9.3/src/fal/dbt/packages/bridge.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.2/src/fal/packages/dependency_analysis.py` & `fal-0.9.3/src/fal/dbt/packages/dependency_analysis.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from pathlib import Path
 from typing import Iterator, List, Optional, Tuple
 
 import importlib_metadata
 
-from fal.utils import cache_static
+from fal.dbt.utils import cache_static
 
 import importlib_metadata
 
 
 def _get_project_root_path(pacakge: str) -> Path:
-    import fal
+    import fal.dbt as fal
 
     # If this is a development version, we'll install
     # the current fal itself.
     path = Path(fal.__file__)
     while path is not None:
         if (path.parent / ".git").exists():
             break
@@ -37,25 +37,20 @@
     for dbt_plugin_name in package_distributions.get("dbt", []):
         distribution = importlib_metadata.distribution(dbt_plugin_name)
 
         # Skip dbt-core since it will be determined by other packages being installed
         if dbt_plugin_name == "dbt-core":
             continue
 
-        # Handle dbt-fal separately (since it needs to be installed
-        # with its extras).
+        # Skip dbt-fal since it is already handled by _get_dbt_fal_package_name
         if dbt_plugin_name == "dbt-fal":
             continue
 
         yield dbt_plugin_name, distribution.version
 
-    package_info = _get_dbt_fal_package_name()
-    if package_info:
-        yield package_info
-
 
 def _find_fal_extras(package: str) -> set[str]:
     # Return a possible set of extras that might be required when installing
     # fal in the new environment. The original form which the user has installed
     # is not present to us (it is not saved anywhere during the package installation
     # process, so there is no way for us to know how a user initially installed fal).
     # We'll therefore be as generous as possible and install all the extras for all
@@ -82,61 +77,47 @@
     # There will be adapters which we won't have an extra for (e.g. oraceledb)
     # and there will be extras which the user did not install the adapter for
     # (e.g. dbt-redshift). We want to take the intersection of all the adapters
     # that the user has installed and all the extras that fal provides and find
     # the smallest possible subset of extras that we can install.
     return available_dbt_adapters.intersection(all_extras)
 
-def _is_fal_pre_release() -> bool:
-    raw_fal_version = importlib_metadata.version("fal")
+def _running_pre_release() -> bool:
+    raw_fal_version = importlib_metadata.version("dbt-fal")
     return _version_is_prerelease(raw_fal_version)
 
 def _version_is_prerelease(raw_version: str) -> bool:
     from packaging.version import Version
 
     package_version = Version(raw_version)
     return package_version.is_prerelease
 
-def _get_dbt_fal_package_name() -> Optional[Tuple[str, Optional[str]]]:
-    try:
-        dbt_fal_version = importlib_metadata.version("dbt-fal")
-    except importlib_metadata.PackageNotFoundError:
-        # It might not be installed.
-        return None
-
-    if _is_fal_pre_release():
-        dbt_fal_dep = str(_get_project_root_path("adapter"))
-        # We are going to install it from the local path.
-        dbt_fal_version = None
+def _get_dbt_fal_package() -> Tuple[str, Optional[str]]:
+    if _running_pre_release():
+        proj_path = _get_project_root_path("adapter")
+        if proj_path.exists():
+            # We are going to install it from the local path.
+            dbt_fal_dep = str(proj_path)
+            dbt_fal_version = None
+        else:
+            # We are going to install it from PyPI.
+            dbt_fal_dep = "dbt-fal"
+            dbt_fal_version = importlib_metadata.version("dbt-fal")
     else:
         dbt_fal_dep = "dbt-fal"
+        dbt_fal_version = importlib_metadata.version("dbt-fal")
 
     dbt_fal_extras = _find_fal_extras("dbt-fal")
     if dbt_fal_extras:
         dbt_fal_dep += f"[{','.join(dbt_fal_extras)}]"
 
     return dbt_fal_dep, dbt_fal_version
 
-def _get_fal_package_name() -> Tuple[str, Optional[str]]:
-    if _is_fal_pre_release():
-        fal_dep = str(_get_project_root_path("fal"))
-        fal_version = None
-    else:
-        fal_dep = "fal"
-        fal_version = importlib_metadata.version("fal")
-
-    fal_extras = _find_fal_extras("fal")
-    if fal_extras:
-        fal_dep += f"[{','.join(fal_extras)}]"
-
-    return fal_dep, fal_version
-
-
 def get_default_requirements() -> Iterator[Tuple[str, Optional[str]]]:
-    yield _get_fal_package_name()
+    yield _get_dbt_fal_package()
     yield from _get_dbt_packages()
 
 
 @cache_static
 def get_default_pip_dependencies() -> List[str]:
     return [
         f"{package}=={version}" if version else package
```

### Comparing `fal-0.9.2/src/fal/packages/environments/__init__.py` & `fal-0.9.3/src/fal/dbt/packages/environments/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from typing import List, Optional, Dict, Any
 
-from fal.packages.environments.base import BASE_CACHE_DIR, BaseEnvironment
-from fal.packages.environments.conda import CondaEnvironment
-from fal.packages.environments.virtual_env import VirtualPythonEnvironment
+from fal.dbt.packages.environments.base import BASE_CACHE_DIR, BaseEnvironment
+from fal.dbt.packages.environments.conda import CondaEnvironment
+from fal.dbt.packages.environments.virtual_env import VirtualPythonEnvironment
 
 REGISTERED_ENVIRONMENTS: Dict[str, BaseEnvironment] = {
     "conda": CondaEnvironment,
     "venv": VirtualPythonEnvironment,
 }
```

### Comparing `fal-0.9.2/src/fal/packages/environments/base.py` & `fal-0.9.3/src/fal/dbt/packages/environments/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,16 +9,16 @@
 from contextlib import ExitStack, contextmanager, nullcontext
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Callable, ContextManager, Generic, Iterator, TypeVar, Dict, Any
 
 from platformdirs import user_cache_dir
 
-from faldbt.logger import LOGGER
-from fal.packages import bridge, isolated_runner
+from fal.dbt.integration.logger import LOGGER
+from fal.dbt.packages import bridge, isolated_runner
 
 BASE_CACHE_DIR = Path(user_cache_dir("fal", "fal"))
 BASE_CACHE_DIR.mkdir(exist_ok=True)
 
 T = TypeVar("T")
 K = TypeVar("K", bound="BaseEnvironment")
 BasicCallable = Callable[[], int]
```

### Comparing `fal-0.9.2/src/fal/packages/environments/conda.py` & `fal-0.9.3/src/fal/dbt/packages/environments/conda.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,23 @@
 import shutil
 import subprocess
 import sysconfig
 from dataclasses import dataclass
 from pathlib import Path
 from typing import List, Dict, Any
 
-from fal.packages.environments.base import (
+from fal.dbt.packages.environments.base import (
     BASE_CACHE_DIR,
     BaseEnvironment,
     DualPythonIPC,
     log_env,
     rmdir_on_fail,
 )
-from fal.packages.environments.virtual_env import get_primary_virtual_env
-from fal.utils import cache_static
+from fal.dbt.packages.environments.virtual_env import get_primary_virtual_env
+from fal.dbt.utils import cache_static
 
 _BASE_CONDA_DIR = BASE_CACHE_DIR / "conda"
 _BASE_CONDA_DIR.mkdir(exist_ok=True)
 
 # Specify the path where the conda binary might
 # reside in (or mamba, if it is the preferred one).
 _CONDA_COMMAND = os.environ.get("CONDA_EXE", "conda")
```

### Comparing `fal-0.9.2/src/fal/packages/environments/virtual_env.py` & `fal-0.9.3/src/fal/dbt/packages/environments/virtual_env.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,25 +3,25 @@
 import sys
 import hashlib
 import subprocess
 from dataclasses import dataclass, field
 from pathlib import Path
 from typing import List, Dict, Any
 
-from fal.packages.dependency_analysis import get_default_pip_dependencies
-from fal.packages.environments.base import (
+from fal.dbt.packages.dependency_analysis import get_default_pip_dependencies
+from fal.dbt.packages.environments.base import (
     BASE_CACHE_DIR,
     BaseEnvironment,
     DualPythonIPC,
     get_executable_path,
     log_env,
     python_path_for,
     rmdir_on_fail,
 )
-from fal.utils import cache_static
+from fal.dbt.utils import cache_static
 
 _BASE_VENV_DIR = BASE_CACHE_DIR / "venvs"
 _BASE_VENV_DIR.mkdir(exist_ok=True)
 
 
 @dataclass
 class VirtualPythonEnvironment(BaseEnvironment[Path], make_thread_safe=True):
```

### Comparing `fal-0.9.2/src/fal/packages/isolated_runner.py` & `fal-0.9.3/src/fal/dbt/packages/isolated_runner.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,16 +32,16 @@
 #
 
 IS_DEBUG_MODE = os.getenv("FAL_DEBUG_ISOLATED_RUNNER") == "1"
 DEBUG_TIMEOUT = 60 * 15
 
 
 def run_client(address: str, *, with_pdb: bool = False) -> int:
-    from faldbt.logger import LOGGER
-    from fal.packages import bridge
+    from fal.dbt.integration.logger import LOGGER
+    from fal.dbt.packages import bridge
 
     if with_pdb:
         # This condition will only be activated if we want to
         # debug the isolated process by passing the --with-pdb
         # flag when executing the binary.
         breakpoint()
 
@@ -84,16 +84,16 @@
             "PYTHONPATH",
         ]
         if session_variable in os.environ
     )
 
 
 def _fal_main() -> None:
-    from faldbt.logger import LOGGER
-    from fal.packages import bridge
+    from fal.dbt.integration.logger import LOGGER
+    from fal.dbt.packages import bridge
 
     LOGGER.debug("Starting the isolated process at PID {}", os.getpid())
 
     parser = ArgumentParser()
     parser.add_argument("listen_at")
     parser.add_argument("--with-pdb", action="store_true", default=False)
 
@@ -121,15 +121,15 @@
     for site_dir in python_path.split(os.pathsep):
         site.addsitedir(site_dir)
 
 
 def main():
     _process_primary_env_packages()
 
-    from faldbt.logger import log_manager
+    from fal.dbt.integration.logger import log_manager
 
     # TODO: do we still need this?
     with log_manager.applicationbound():
         _fal_main()
 
 
 if __name__ == "__main__":
```

### Comparing `fal-0.9.2/src/fal/planner/executor.py` & `fal-0.9.3/src/fal/dbt/planner/executor.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
     Future,
     ThreadPoolExecutor,
     wait,
 )
 from dataclasses import dataclass, field
 from typing import Iterator, List, Optional
 
-from fal.planner.schedule import SUCCESS, Scheduler
-from fal.planner.tasks import (
+from fal.dbt.planner.schedule import SUCCESS, Scheduler
+from fal.dbt.planner.tasks import (
     TaskGroup,
     Task,
     Status,
     DBTTask,
     FalLocalHookTask,
     HookType,
 )
-from faldbt.project import FalDbt
+from fal.dbt.integration.project import FalDbt
 
-from faldbt.logger import LOGGER
+from fal.dbt.integration.logger import LOGGER
 
 
 class State(Enum):
     PRE_HOOKS = auto()
     MAIN_TASK = auto()
     POST_HOOKS = auto()
```

### Comparing `fal-0.9.2/src/fal/planner/plan.py` & `fal-0.9.3/src/fal/dbt/planner/plan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 from typing import Callable, Iterator, List, Set
 
 import networkx as nx
-from fal.node_graph import NodeKind
-from fal.cli.selectors import ExecutionPlan, _is_before_script, _is_after_script
-from faldbt.logger import LOGGER
+from fal.dbt.node_graph import NodeKind
+from fal.dbt.cli.selectors import ExecutionPlan, _is_before_script, _is_after_script
+from fal.dbt.integration.logger import LOGGER
 from dataclasses import dataclass
 
 
 @dataclass
 class OriginGraph:
     graph: nx.DiGraph
```

### Comparing `fal-0.9.2/src/fal/planner/schedule.py` & `fal-0.9.3/src/fal/dbt/planner/schedule.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,29 @@
 
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Iterator, List, Optional
 
 import networkx as nx
 
-from faldbt.project import DbtModel
-from fal.node_graph import DbtModelNode, NodeGraph, NodeKind, ScriptNode
-from fal.planner.tasks import (
+from fal.dbt.integration.project import DbtModel
+from fal.dbt.node_graph import DbtModelNode, NodeGraph, NodeKind, ScriptNode
+from fal.dbt.planner.tasks import (
     SUCCESS,
     Task,
     DBTTask,
     FalIsolatedHookTask,
     FalLocalHookTask,
     FalModelTask,
     TaskGroup,
     Status,
     HookType,
 )
-from fal.utils import DynamicIndexProvider
-from fal.fal_script import Hook, IsolatedHook, create_hook, TimingType
+from fal.dbt.utils import DynamicIndexProvider
+from fal.dbt.fal_script import Hook, IsolatedHook, create_hook, TimingType
 
 
 def create_hook_task(
     hook: Hook,
     bound_model: DbtModel,
     hook_type: HookType = HookType.HOOK,
     timing_type: Optional[TimingType] = None,
```

### Comparing `fal-0.9.2/src/fal/planner/tasks.py` & `fal-0.9.3/src/fal/dbt/planner/tasks.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 import uuid
 from functools import partial
 from contextlib import contextmanager
 from dataclasses import dataclass, field
 from enum import Enum, auto
 from typing import Iterator, List, Any, Optional, Dict, Tuple, Union
 
-from faldbt.logger import LOGGER
+from fal.dbt.integration.logger import LOGGER
 
-from fal.fal_script import FalScript, TimingType
-from fal.utils import print_run_info, DynamicIndexProvider
-from faldbt.project import DbtModel, FalDbt, NodeStatus
+from fal.dbt.fal_script import FalScript, TimingType
+from fal.dbt.utils import print_run_info, DynamicIndexProvider
+from fal.dbt.integration.project import DbtModel, FalDbt, NodeStatus
 
 from datetime import datetime, timezone
 
 SUCCESS = 0
 FAILURE = 1
 
 
@@ -158,15 +158,15 @@
 
 
 @dataclass
 class DBTTask(Task):
     model_ids: List[str]
 
     def execute(self, args: argparse.Namespace, fal_dbt: FalDbt) -> int:
-        from fal.cli.dbt_runner import dbt_run_through_python
+        from fal.dbt.cli.dbt_runner import dbt_run_through_python
 
         model_names = _unique_ids_to_model_names(self.model_ids)
         output = dbt_run_through_python(
             args, model_names, fal_dbt.target_path, self.run_index
         )
 
         for node, status, adapter_response in _map_cli_output_model_results(
```

### Comparing `fal-0.9.2/src/fal/telemetry/telemetry.py` & `fal-0.9.3/src/fal/dbt/telemetry/telemetry.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import uuid
 from functools import wraps
 from typing import Any, List, Optional
 import inspect
 from contextlib import contextmanager
 from dbt.config.runtime import RuntimeConfig
 
-from fal.utils import cache_static
+from fal.dbt.utils import cache_static
 
 import platform
 
 
 TELEMETRY_VERSION = "0.0.2"
 DEFAULT_HOME_DIR = "~/.fal"
 CONF_DIR = "stats"
@@ -123,15 +123,15 @@
         return target["type"]
     return None
 
 
 def fal_installed_version():
     """Returns: fal version"""
     try:
-        return pkg_resources.get_distribution("fal").version
+        return pkg_resources.get_distribution("dbt-fal").version
     except ImportError:
         return
 
 
 def is_airflow():
     """Returns: True for Airflow env"""
     return "AIRFLOW_CONFIG" in os.environ or "AIRFLOW_HOME" in os.environ
@@ -238,16 +238,16 @@
             return e
 
 
 @cache_static
 def get_dbt_config():
     try:
         from dbt.flags import PROFILES_DIR
-        from fal.cli.args import parse_args
-        from faldbt.parse import get_dbt_config
+        from fal.dbt.cli.args import parse_args
+        from fal.dbt.integration.parse import get_dbt_config
 
         args = parse_args(sys.argv[1:])
 
         profiles_dir: str = PROFILES_DIR  # type: ignore
         if args.profiles_dir is not None:
             profiles_dir = args.profiles_dir
```

### Comparing `fal-0.9.2/src/fal/typing.py` & `fal-0.9.3/src/fal/dbt/typing.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 
 from __future__ import annotations
 from typing import TYPE_CHECKING
 
 if TYPE_CHECKING:
     import pandas as pd
     from typing import Optional, Dict, List, Protocol, Any
-    from faldbt.project import DbtModel, DbtTest, DbtSource, Feature
-    from fal.fal_script import Context, CurrentModel
+    from fal.dbt.integration.project import DbtModel, DbtTest, DbtSource, Feature
+    from fal.dbt.fal_script import Context, CurrentModel
 
     class _List_Sources(Protocol):
         def __call__(self) -> List[DbtSource]:
             """
             List tables available for `source` usage
             """
             ...
```

### Comparing `fal-0.9.2/src/fal/utils.py` & `fal-0.9.3/src/fal/dbt/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """Fal utilities."""
 import copy
-from faldbt.logger import LOGGER
+from fal.dbt.integration.logger import LOGGER
 from typing import List, TYPE_CHECKING, TypeVar
 
 try:
     from functools import lru_cache
 except ImportError:
     from backports.functools_lru_cache import lru_cache
 
 if TYPE_CHECKING:
-    from fal.fal_script import FalScript
+    from fal.dbt.fal_script import FalScript
 
 
 def print_run_info(scripts: List["FalScript"]):
     """Print information on the current fal run."""
     models_str = "\n".join(map(lambda script: script.id, scripts))
     LOGGER.info(f"Starting fal run for following models and scripts: \n{models_str}\n")
```

### Comparing `fal-0.9.2/src/faldbt/lib.py` & `fal-0.9.3/src/fal/dbt/integration/lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 import sqlalchemy
 from sqlalchemy.sql.ddl import CreateTable
 from sqlalchemy.sql import Insert
 
 from dbt.contracts.sql import RemoteRunResult
 
 
-from faldbt import parse
-from faldbt.logger import LOGGER
+from fal.dbt.integration import parse
+from fal.dbt.integration.logger import LOGGER
 
 
 class WriteModeEnum(Enum):
     APPEND = "append"
     OVERWRITE = "overwrite"
```

### Comparing `fal-0.9.2/src/faldbt/logger.py` & `fal-0.9.3/src/fal/dbt/integration/logger.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.2/src/faldbt/magics.py` & `fal-0.9.3/src/fal/dbt/integration/magics.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from IPython.core.magic import register_line_magic, needs_local_scope
 from functools import partial
-from fal import FalDbt
+from fal.dbt import FalDbt
 
 
 @register_line_magic
 @needs_local_scope
 def init_fal(line="", local_ns={}):
     '''
     Init fal magic variables. Must provide project_dir and profiles_dir.
 
     Example:
     """
-    from faldbt.magics import init_fal
+    from fal.dbt.integration.magics import init_fal
 
     %init_fal project_dir=/my_project_dir profiles_dir=/my_profiles_dir default_model_name=my_model
     """
     '''
     args = dict([arg.split("=") for arg in line.split()])
     if not args.get("project_dir") or not args.get("profiles_dir"):
         raise Exception(
```

### Comparing `fal-0.9.2/src/faldbt/parse.py` & `fal-0.9.3/src/fal/dbt/integration/parse.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,22 +10,22 @@
 from dbt.contracts.graph.manifest import Manifest
 from dbt.contracts.results import RunResultsArtifact, FreshnessExecutionResultArtifact
 from dbt.contracts.project import UserConfig
 from dbt.config.profile import read_user_config
 
 from dbt.exceptions import IncompatibleSchemaError, DbtRuntimeError
 
-from fal.utils import cache_static
+from fal.dbt.utils import cache_static
 
-from faldbt.logger import LOGGER
-from faldbt.utils.yaml_helper import load_yaml
-from fal.telemetry import telemetry
+from fal.dbt.integration.logger import LOGGER
+from fal.dbt.integration.utils.yaml_helper import load_yaml
+from fal.dbt.telemetry import telemetry
 
 if TYPE_CHECKING:
-    from fal.packages.environments import BaseEnvironment
+    from fal.dbt.packages.environments import BaseEnvironment
 
 FAL_SCRIPTS_PATH = "fal-scripts-path"
 FAL_MODELS_PATHS = "fal-models-paths"
 
 
 class FalParseError(Exception):
     pass
@@ -221,16 +221,16 @@
 def _get_required_key(data: Dict[str, Any], name: str) -> Any:
     if name not in data:
         raise FalParseError("Missing required key: " + name)
     return data[name]
 
 
 def load_environments(base_dir: str) -> Dict[str, "BaseEnvironment"]:
-    from fal.packages.environments import create_environment
-    from fal.fal_script import _is_local_environment
+    from fal.dbt.packages.environments import create_environment
+    from fal.dbt.fal_script import _is_local_environment
 
     try:
         fal_project_path = os.path.join(base_dir, "fal_project.yml")
         if not os.path.exists(fal_project_path):
             raise FalParseError(f"{fal_project_path} must exist to define environments")
 
         fal_project = load_yaml(fal_project_path)
```

### Comparing `fal-0.9.2/src/faldbt/project.py` & `fal-0.9.3/src/fal/dbt/integration/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     Tuple,
     Sequence,
     TYPE_CHECKING,
 )
 from pathlib import Path
 from deprecation import deprecated
 
-import faldbt.version as version
+import fal.dbt.integration.version as version
 
 from dbt.cli.resolvers import default_profiles_dir
 from dbt.cli.main import dbtRunner, dbtRunnerResult
 
 from dbt.contracts.graph.nodes import (
     SourceDefinition,
     TestMetadata,
@@ -45,24 +45,24 @@
 )
 from dbt.task.compile import CompileTask
 
 from . import parse
 from . import lib
 from . import version
 
-from fal.feature_store.feature import Feature
+from fal.dbt.feature_store.feature import Feature
 
 import pandas as pd
 
-from fal.telemetry import telemetry
-from fal.utils import has_side_effects
+from fal.dbt.telemetry import telemetry
+from fal.dbt.utils import has_side_effects
 
 if TYPE_CHECKING:
-    from fal.fal_script import Hook, TimingType
-    from fal.packages.environments import BaseEnvironment
+    from fal.dbt.fal_script import Hook, TimingType
+    from fal.dbt.packages.environments import BaseEnvironment
 
 
 class FalGeneralException(Exception):
     pass
 
 
 FAL = "fal"
@@ -248,15 +248,15 @@
     def get_depends_on_nodes(self) -> List[str]:
         return self.node.depends_on_nodes
 
     def get_hooks(
         self,
         hook_type: "TimingType",
     ) -> List["Hook"]:
-        from fal.fal_script import create_hook, TimingType
+        from fal.dbt.fal_script import create_hook, TimingType
 
         meta = self.meta or {}
 
         keyword_dict = meta.get(FAL) or {}
         if not isinstance(keyword_dict, dict):
             return []
```

### Comparing `fal-0.9.2/src/faldbt/utils/yaml_helper.py` & `fal-0.9.3/src/dbt/adapters/fal_experimental/utils/yaml_helper.py`

 * *Files identical despite different names*

### Comparing `fal-0.9.2/tests/_fal_testing/utils.py` & `fal-0.9.3/tests/_fal_testing/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     )
 
 
 def get_environment_type():
     # To determine whether this is a fal-created environment or not
     # we'll check whether the executable that is running this script
     # is located under any of the designated fal environment directories.
-    from fal.packages.environments.virtual_env import _BASE_VENV_DIR
-    from fal.packages.environments.conda import _BASE_CONDA_DIR
+    from fal.dbt.packages.environments.virtual_env import _BASE_VENV_DIR
+    from fal.dbt.packages.environments.conda import _BASE_CONDA_DIR
 
     executable_path = Path(sys.executable)
     for environment_type, prefix in [
         ("venv", _BASE_VENV_DIR),
         ("conda", _BASE_CONDA_DIR),
     ]:
         if prefix in executable_path.parents:
```

### Comparing `fal-0.9.2/PKG-INFO` & `fal-0.9.3/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,84 +1,147 @@
 Metadata-Version: 2.1
 Name: fal
-Version: 0.9.2
-Summary: fal allows you to run python scripts directly from your dbt project.
-Home-page: https://github.com/fal-ai/fal/blob/-/projects/fal
-Keywords: dbt,pandas
+Version: 0.9.3
+Summary: Run python scripts from any dbt project.
+Home-page: https://github.com/fal-ai/fal
+Keywords: dbt,pandas,fal,runtime
 Author: Features & Labels
 Author-email: hello@fal.ai
 Requires-Python: >=3.7.2,<3.12
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: athena
 Provides-Extra: bigquery
-Provides-Extra: cloud
-Provides-Extra: dev
 Provides-Extra: duckdb
 Provides-Extra: postgres
 Provides-Extra: redshift
 Provides-Extra: snowflake
-Provides-Extra: test
+Provides-Extra: teleport
+Provides-Extra: trino
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: agate-sql (>=0.5.8,<0.6.0)
 Requires-Dist: astor (>=0.8.1,<0.9.0)
+Requires-Dist: awswrangler[redshift] (>=3.0.0) ; (python_version >= "3.8") and (extra == "redshift")
 Requires-Dist: backports.functools_lru_cache (>=1.6.4,<2.0.0)
-Requires-Dist: behave (>=1.2.6,<2.0.0) ; extra == "test"
-Requires-Dist: black (>=22.3,<23.0) ; extra == "test"
 Requires-Dist: dbt-core (>=1.5,<=1.5.1)
 Requires-Dist: deprecation (>=2.1.0,<3.0.0)
 Requires-Dist: dill (>=0.3.6,<0.3.7)
 Requires-Dist: duckdb-engine (>=0.1.8,<0.2.0) ; extra == "duckdb"
+Requires-Dist: fal-serverless (>=0.6.35,<0.7.0)
 Requires-Dist: google-cloud-bigquery[pandas] (>=3.5.0,<3.6.0) ; extra == "bigquery"
-Requires-Dist: importlib-metadata (>=4.12.0)
-Requires-Dist: matplotlib (>=3.5.2,<4.0.0) ; extra == "dev"
-Requires-Dist: mock (>=4.0.3,<5.0.0) ; extra == "test"
-Requires-Dist: packaging (>20.9)
+Requires-Dist: importlib-metadata (>=6.0.0,<7.0.0)
+Requires-Dist: packaging (>=23)
 Requires-Dist: pandas (>=1.3.4,<2.0.0)
 Requires-Dist: platformdirs (>=2.5.2,<3.0.0)
 Requires-Dist: posthog (>=1.4.5,<2.0.0)
-Requires-Dist: pytest (>=5.2,<6.0) ; extra == "test"
-Requires-Dist: pytest-mock (>=3.7.0,<4.0.0) ; extra == "test"
-Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: s3fs (>=2022.8.2) ; extra == "teleport"
 Requires-Dist: snowflake-connector-python[pandas] (>=3.0,<4.0) ; extra == "snowflake"
+Requires-Dist: sqlalchemy (>=1.4.41,<2.0.0)
 Requires-Dist: sqlalchemy-redshift (>=0.8.9,<0.9.0) ; extra == "redshift"
+Requires-Dist: trino[sqlalchemy] (>=0.321.0,<0.322.0) ; extra == "trino"
 Requires-Dist: virtualenv (>=20.16.2,<21.0.0)
-Project-URL: Documentation, https://docs.fal.ai
 Project-URL: Repository, https://github.com/fal-ai/fal
 Description-Content-Type: text/markdown
 
-<!-- <base href="https://github.com/fal-ai/fal/blob/-/projects/fal/" target="_blank" /> -->
+<!-- <base href="https://github.com/fal-ai/fal/blob/-/projects/adapter/" target="_blank" /> -->
 
-# fal: do more with dbt
+# Welcome to dbt-fal 👋 do more with dbt
 
-fal is the easiest way to run Python with your [dbt](https://www.getdbt.com/) project.
+dbt-fal adapter is the ✨easiest✨ way to run your [dbt Python models](https://docs.getdbt.com/docs/building-a-dbt-project/building-models/python-models).
 
-# Introduction
+Starting with dbt v1.3, you can now build your dbt models in Python. This leads to some cool use cases that was once difficult to build with SQL alone. Some examples are:
 
-With the `fal` CLI, you can:
+- Using Python stats libraries to calculate stats
+- Building forecasts
+- Building other predictive models such as classification and clustering
+
+This is fantastic! BUT, there is still one issue though! The developer experience with Snowflake and Bigquery is not great, and there is no Python support for Redshift and Postgres.
+
+dbt-fal provides the best environment to run your Python models that works with all other data warehouses! With dbt-fal, you can:
+
+- Build and test your models locally
+- Isolate each model to run in its own environment with its own dependencies
+- [Coming Soon] Run your Python models in the ☁️ cloud ☁️ with elasticly scaling Python environments.
+- [Coming Soon] Even add GPUs to your models for some heavier workloads such as training ML models.
+
+## Getting Started
+
+### 1. Install dbt-fal
+`pip install dbt-fal[bigquery,snowflake]` *Add your current warehouse here*
+
+### 2. Update your `profiles.yml` and add the fal adapter
+
+```yaml
+jaffle_shop:
+  target: dev_with_fal
+  outputs:
+    dev_with_fal:
+      type: fal
+      db_profile: dev_bigquery # This points to your main adapter
+    dev_bigquery:
+      type: bigquery
+      ...
+```
+
+Don't forget to point to your main adapter with the `db_profile` attribute. This is how the fal adapter knows how to connect to your data warehouse.
+
+### 3. `dbt run`!
+That is it! It is really that simple 😊
+
+### 4. [🚨 Cool Feature Alert 🚨] Environment management with dbt-fal
+If you want some help with environment management (vs sticking to the default env that the dbt process runs in), you can create a fal_project.yml in the same folder as your dbt project and have “named environments”:
+
+In your dbt project folder:
+```bash
+$ touch fal_project.yml
+
+# Paste the config below
+environments:
+  - name: ml
+    type: venv
+    requirements:
+      - prophet
+```
+
+and then in your dbt model:
+
+```bash
+$ vi models/orders_forecast.py
+
+def model(dbt, fal):
+    dbt.config(fal_environment="ml") # Add this line
+
+    df: pd.DataFrame = dbt.ref("orders_daily")
+```
+
+The `dbt.config(fal_environment=“ml”)` will give you an isolated clean env to run things in, so you dont pollute your package space.
+
+### 5. [Coming Soon™️] Move your compute to the Cloud!
+Let us know if you are interested in this. We are looking for beta users.
+
+# `dbt-fal` command line tool
+
+With the `dbt-fal` CLI, you can:
 
 - [Send Slack notifications](https://github.com/fal-ai/fal/blob/-/examples/slack-example) upon dbt model success or failure.
 - [Load data from external data sources](https://blog.fal.ai/populate-dbt-models-with-csv-data/) before a model starts running.
 - [Download dbt models](https://docs.fal.ai/fal/python-package) into a Python context with a familiar syntax: `ref('my_dbt_model')` using `FalDbt`
 - [Programatically access rich metadata](https://docs.fal.ai/fal/reference/variables-and-functions) about your dbt project.
 
 Head to our [documentation site](https://docs.fal.ai/) for a deeper dive or play with [in-depth examples](https://github.com/fal-ai/fal/blob/-/examples/README.md) to see how fal can help you get more done with dbt.
 
-> ❗️ If you would like to write data back to your data-warehouse, we recommend using the [`dbt-fal`](https://pypi.org/project/dbt-fal/) adapter.
 
-# Getting Started
-
-## 1. Install `fal`
+## 1. Install `dbt-fal`
 
 ```bash
-$ pip install fal
+$ pip install dbt-fal[postgres]
 ```
 
 ## 2. Go to your dbt project directory
 
 ```bash
 $ cd ~/src/my_dbt_project
 ```
@@ -120,65 +183,31 @@
         description: Date
     meta:
       fal:
         scripts:
           - send_slack_message.py
 ```
 
-## 5. Run `fal flow run`
+## 5. Run `dbt-fal flow run`
 
 ```bash
-$ fal flow run
-# both your dbt models and fal scripts are run
+$ dbt-fal flow run
+# both your dbt models and python scripts are run
 ```
 
 ## 6. Alternatively run `dbt` and `fal` consecutively
 
 ```bash
 $ dbt run
 # Your dbt models are run
 
-$ fal run
+$ dbt-fal run
 # Your python scripts are run
 ```
 
-# Examples
-
-To explore what is possible with fal, take a look at the in-depth examples below. We will be adding more examples here over time:
-
-- [Example 1: Send Slack notifications](https://github.com/fal-ai/fal/blob/-/examples/slack-example/README.md)
-- [Example 2: Use dbt from a Jupyter Notebook](https://github.com/fal-ai/fal/blob/-/examples/write_jupyter_notebook/README.md)
-- [Example 3: Read and parse dbt metadata](https://github.com/fal-ai/fal/blob/-/examples/read_dbt_metadata/README.md)
-- [Example 4: Metric forecasting](https://github.com/fal-ai/fal/blob/-/examples/metric-forecast/README.md)
-- [Example 5: Sentiment analysis on support tickets](https://github.com/fal-ai/fal/blob/-/examples/sentiment-analysis/README.md)
-- [Example 6: Anomaly Detection](https://github.com/fal-ai/fal/blob/-/examples/anomaly-detection/README.md)
-- [Example 7: Incorporate fal in CI/CD workflow](https://github.com/fal-ai/fal/blob/-/examples/ci_example/README.md)
-- [Example 8: Send events to Datadog](https://github.com/fal-ai/fal/blob/-/examples/datadog_event/README.md)
-- [Example 9: Write dbt artifacts to GCS](https://github.com/fal-ai/fal/blob/-/examples/write_to_gcs/README.md)
-- [Example 10: Write dbt artifacts to AWS S3](https://github.com/fal-ai/fal/blob/-/examples/write_to_aws/README.md)
-
-[Check out the examples directory for more](https://github.com/fal-ai/fal/blob/-/examples/README.md)
-
-# How it works?
-
-`fal` is a command line tool that can read the state of your `dbt` project and help you run Python scripts after your `dbt run`s by leveraging the [`meta` config](https://docs.getdbt.com/reference/resource-configs/meta).
-
-```yaml
-models:
-  - name: historical_ozone_levels
-    ...
-    meta:
-      fal:
-        post-hook:
-          # scripts will run concurrently
-          - send_slack_message.py
-          - another_python_script.py
-```
-
-`fal` also provides useful helpers within the Python context to seamlessly interact with dbt models: `ref("my_dbt_model_name")` will pull a dbt model into your Python script as a [`pandas.DataFrame`](https://pandas.pydata.org/pandas-docs/stable/reference/api/pandas.DataFrame.html).
 
 ## Running scripts before dbt runs
 
 Run scripts before the model runs by using the `pre-hook:` configuration option.
 
 Given the following schema.yml:
 
@@ -193,19 +222,19 @@
       fal:
         pre-hook:
           - fal_scripts/trigger_fivetran.py
         post-hook:
           - fal_scripts/slack.py
 ```
 
-`fal flow run` will run `fal_scripts/trigger_fivetran.py`, then the `boston` dbt model, and finally `fal_scripts/slack.py`.
+`dbt-fal flow run` will run `fal_scripts/trigger_fivetran.py`, then the `boston` dbt model, and finally `fal_scripts/slack.py`.
 If a model is selected with a selection flag (e.g. `--select boston`), the hooks associated to the model will always run with it.
 
 ```bash
-$ fal flow run --select boston
+$ dbt-fal flow run --select boston
 ```
 
 # Concepts
 
 ## profile.yml and Credentials
 
 `fal` integrates with `dbt`'s `profile.yml` file to access and read data from the data warehouse. Once you setup credentials in your `profile.yml` file for your existing `dbt` workflows anytime you use `ref` or `source` to create a dataframe `fal` authenticates using the credentials specified in the `profile.yml` file.
@@ -308,21 +337,22 @@
 ```python
 from sqlalchemy.types import Integer
 # Upload but specifically create the `value` column with type `integer`
 # Can be useful if data has `None` values
 write_to_model(df, dtype={'value': Integer()})
 ```
 
+
 ## Importing `fal` as a Python package
 
 You may be interested in accessing dbt models and sources easily from a Jupyter Notebook or another Python script.
 For that, just import the `fal` package and intantiate a FalDbt project:
 
 ```py
-from fal import FalDbt
+from fal.dbt import FalDbt
 faldbt = FalDbt(profiles_dir="~/.dbt", project_dir="../my_project")
 
 faldbt.list_sources()
 # [
 #    DbtSource(name='results' ...),
 #    DbtSource(name='ticket_data_sentiment_analysis' ...)
 #    ...
@@ -338,67 +368,18 @@
 
 sentiments = faldbt.source('results', 'ticket_data_sentiment_analysis')
 # pandas.DataFrame
 tickets = faldbt.ref('stg_zendesk_ticket_data')
 # pandas.DataFrame
 ```
 
-# Supported `dbt` versions
-
-The latest `fal` version currently supports dbt `1.4.*`.
-
-If you need another version, [open an issue](https://github.com/fal-ai/fal/issues/new) and we will take a look!
-
-# Contributing / Development
-
-We use Poetry for dependency management and easy development testing.
-
-Use Poetry shell to trying your changes right away:
-
-```sh
-~ $ cd fal
-
-~/fal $ poetry install
-
-~/fal $ poetry shell
-Spawning shell within [...]/fal-eFX98vrn-py3.8
-
-~/fal fal-eFX98vrn-py3.8 $ cd ../dbt_project
-
-~/dbt_project fal-eFX98vrn-py3.8 $ fal flow run
-19:27:30  Found 5 models, 0 tests, 0 snapshots, 0 analyses, 165 macros, 0 operations, 0 seed files, 1 source, 0 exposures, 0 metrics
-19:27:30 | Starting fal run for following models and scripts:
-[...]
-```
-
-## Running tests
-
-Tests rely on a Postgres database to be present, this can be achieved with docker-compose:
-
-```sh
-~/fal $ docker-compose -f tests/docker-compose.yml up -d
-Creating network "tests_default" with the default driver
-Creating fal_db ... done
-
-# Necessary for the import test
-~/fal $ dbt run --profiles-dir tests/mock/mockProfile --project-dir tests/mock
-Running with dbt=1.0.1
-[...]
-Completed successfully
-Done. PASS=5 WARN=0 ERROR=0 SKIP=0 TOTAL=5
-
-~/fal $ pytest -s
-```
-
 # Why are we building this?
 
 We think `dbt` is great because it empowers data people to get more done with the tools that they are already familiar with.
 
-`dbt`'s SQL only design is powerful, but if you ever want to get out of SQL-land and connect to external services or get into Python-land for any reason, you will have a hard time. We built `fal` to enable Python workloads (sending alerts to Slack, building predictive models, pushing data to non-data-warehouse destinations and more) **right within `dbt`**.
-
 This library will form the basis of our attempt to more comprehensively enable **data science workloads** downstream of `dbt`. And because having reliable data pipelines is the most important ingredient in building predictive analytics, we are building a library that integrates well with dbt.
 
 # Have feedback or need help?
 
 - Join us in [fal on Discord](https://discord.com/invite/Fyc9PwrccF)
 - Join the [dbt Community](http://community.getdbt.com/) and go into our [#tools-fal channel](https://getdbt.slack.com/archives/C02V8QW3Q4Q)
```

