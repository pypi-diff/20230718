# Comparing `tmp/cm-cluster-on-demand-config-9.2.8.tar.gz` & `tmp/cm-cluster-on-demand-config-9.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm-cluster-on-demand-config-9.2.8.tar", last modified: Tue Dec 27 18:19:25 2022, max compression
+gzip compressed data, was "cm-cluster-on-demand-config-9.2.9.tar", last modified: Mon Feb 20 12:11:26 2023, max compression
```

## Comparing `cm-cluster-on-demand-config-9.2.8.tar` & `cm-cluster-on-demand-config-9.2.9.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:25.781301 cm-cluster-on-demand-config-9.2.8/
--rw-r--r--   0 root         (0) root         (0)    11358 2022-12-27 18:19:08.000000 cm-cluster-on-demand-config-9.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       84 2022-12-27 18:19:08.000000 cm-cluster-on-demand-config-9.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      597 2022-12-27 18:19:25.781301 cm-cluster-on-demand-config-9.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      245 2022-12-27 18:19:08.000000 cm-cluster-on-demand-config-9.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:25.769301 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/
--rw-r--r--   0 root         (0) root         (0)     3135 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2022-12-27 18:19:24.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/_version.py
--rw-r--r--   0 root         (0) root         (0)     4549 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/argparse_factory.py
--rw-r--r--   0 root         (0) root         (0)     7509 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/command_context.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:25.769301 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/config_dump/
--rw-r--r--   0 root         (0) root         (0)      887 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/config_dump/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4666 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/config_dump/full_ini_config_dump.py
--rw-r--r--   0 root         (0) root         (0)     2592 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/config_dump/human_readable_config_dump.py
--rw-r--r--   0 root         (0) root         (0)     1523 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/config_dump/minimal_ini_config_dump.py
--rw-r--r--   0 root         (0) root         (0)     1209 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/config_dump/utils.py
--rw-r--r--   0 root         (0) root         (0)     1572 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/config_file_encoding.py
--rw-r--r--   0 root         (0) root         (0)    16667 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/config_namespace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:25.773301 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/
--rw-r--r--   0 root         (0) root         (0)      869 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5135 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/collective_configuration.py
--rw-r--r--   0 root         (0) root         (0)     3630 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/command_configuration.py
--rw-r--r--   0 root         (0) root         (0)     1556 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/configuration.py
--rw-r--r--   0 root         (0) root         (0)     1369 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/configuration_for_namespace_view.py
--rw-r--r--   0 root         (0) root         (0)     1451 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/configuration_item.py
--rw-r--r--   0 root         (0) root         (0)     1318 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/configuration_view.py
--rw-r--r--   0 root         (0) root         (0)     1415 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/global_configuration.py
--rw-r--r--   0 root         (0) root         (0)    12911 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration_validation.py
--rw-r--r--   0 root         (0) root         (0)     2708 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/determine_invoked_command.py
--rw-r--r--   0 root         (0) root         (0)     1291 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:25.773301 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/explain/
--rw-r--r--   0 root         (0) root         (0)      675 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/explain/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10309 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/explain/explain.py
--rw-r--r--   0 root         (0) root         (0)     2979 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/explain/find_parameters.py
--rw-r--r--   0 root         (0) root         (0)     2387 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/explain/namespace_tree.py
--rw-r--r--   0 root         (0) root         (0)      914 2022-12-27 18:19:08.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/explain/template.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:25.773301 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/expression_parser/
--rw-r--r--   0 root         (0) root         (0)     1565 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/expression_parser/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1830 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/expression_parser/evaluator.py
--rw-r--r--   0 root         (0) root         (0)     5035 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/expression_parser/grammar.py
--rw-r--r--   0 root         (0) root         (0)     1354 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/expression_parser/lexeme_stream.py
--rw-r--r--   0 root         (0) root         (0)     2334 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/expression_parser/parser.py
--rw-r--r--   0 root         (0) root         (0)     1483 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/expression_parser/tokenizer.py
--rw-r--r--   0 root         (0) root         (0)     3291 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/factory_method_factory.py
--rw-r--r--   0 root         (0) root         (0)     1092 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/global_config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:25.773301 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/
--rw-r--r--   0 root         (0) root         (0)     1036 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3704 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/generate_sources.py
--rw-r--r--   0 root         (0) root         (0)     1630 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/load_boot_configuration.py
--rw-r--r--   0 root         (0) root         (0)     7440 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/load_collective_configuration.py
--rw-r--r--   0 root         (0) root         (0)     3535 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/load_command_configuration.py
--rw-r--r--   0 root         (0) root         (0)     2161 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/shared.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:25.773301 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/tests/
--rw-r--r--   0 root         (0) root         (0)      596 2022-12-27 18:19:08.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4625 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/tests/source_decorators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:25.777301 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/
--rw-r--r--   0 root         (0) root         (0)     1250 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4553 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/enumeration_parameter.py
--rw-r--r--   0 root         (0) root         (0)     1420 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/optional_parameter.py
--rw-r--r--   0 root         (0) root         (0)     2120 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/parameter.py
--rw-r--r--   0 root         (0) root         (0)     2701 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/parameter_creation_completion.py
--rw-r--r--   0 root         (0) root         (0)     7528 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/parameter_creation_validation.py
--rw-r--r--   0 root         (0) root         (0)     1053 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/positional_parameter.py
--rw-r--r--   0 root         (0) root         (0)     3179 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/repeating_positional_parameter.py
--rw-r--r--   0 root         (0) root         (0)     4417 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/simple_parameter.py
--rw-r--r--   0 root         (0) root         (0)     3077 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/simple_positional_parameter.py
--rw-r--r--   0 root         (0) root         (0)     2678 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/switch_parameter.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:25.777301 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/tests/
--rw-r--r--   0 root         (0) root         (0)      596 2022-12-27 18:19:08.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2241 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/tests/optional_parameter_test_case.py
--rw-r--r--   0 root         (0) root         (0)     7281 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/tests/parameter_test_case.py
--rw-r--r--   0 root         (0) root         (0)     1001 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/tests/positional_parameter_test_case.py
--rw-r--r--   0 root         (0) root         (0)     2143 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parser_utils.py
--rw-r--r--   0 root         (0) root         (0)     9221 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/print_help.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:25.777301 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/
--rw-r--r--   0 root         (0) root         (0)     1055 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2817 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/cli_source.py
--rw-r--r--   0 root         (0) root         (0)     4528 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/config_file_source.py
--rw-r--r--   0 root         (0) root         (0)     1452 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/dynamic_default_source.py
--rw-r--r--   0 root         (0) root         (0)      747 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/enforcing_config_file_source.py
--rw-r--r--   0 root         (0) root         (0)     3452 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/env_source.py
--rw-r--r--   0 root         (0) root         (0)     1430 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/source.py
--rw-r--r--   0 root         (0) root         (0)     1270 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/static_default_source.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:25.777301 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/tests/
--rw-r--r--   0 root         (0) root         (0)      596 2022-12-27 18:19:08.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:25.777301 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/tab_completion/
--rw-r--r--   0 root         (0) root         (0)      726 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/tab_completion/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2188 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/tab_completion/generate.py
--rw-r--r--   0 root         (0) root         (0)     2949 2022-12-27 18:19:08.000000 cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/tab_completion/template.sh.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:25.781301 cm-cluster-on-demand-config-9.2.8/cm_cluster_on_demand_config.egg-info/
--rw-r--r--   0 root         (0) root         (0)      597 2022-12-27 18:19:25.000000 cm-cluster-on-demand-config-9.2.8/cm_cluster_on_demand_config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     4087 2022-12-27 18:19:25.000000 cm-cluster-on-demand-config-9.2.8/cm_cluster_on_demand_config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-27 18:19:25.000000 cm-cluster-on-demand-config-9.2.8/cm_cluster_on_demand_config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2022-12-27 18:19:25.000000 cm-cluster-on-demand-config-9.2.8/cm_cluster_on_demand_config.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2022-12-27 18:19:25.000000 cm-cluster-on-demand-config-9.2.8/cm_cluster_on_demand_config.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-27 18:19:25.781301 cm-cluster-on-demand-config-9.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2041 2022-12-27 18:19:11.000000 cm-cluster-on-demand-config-9.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:26.487759 cm-cluster-on-demand-config-9.2.9/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-02-20 12:11:10.000000 cm-cluster-on-demand-config-9.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       84 2023-02-20 12:11:10.000000 cm-cluster-on-demand-config-9.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      597 2023-02-20 12:11:26.487759 cm-cluster-on-demand-config-9.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      245 2023-02-20 12:11:10.000000 cm-cluster-on-demand-config-9.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:26.479759 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/
+-rw-r--r--   0 root         (0) root         (0)     3135 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-02-20 12:11:25.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/_version.py
+-rw-r--r--   0 root         (0) root         (0)     4549 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/argparse_factory.py
+-rw-r--r--   0 root         (0) root         (0)     7509 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/command_context.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:26.479759 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/config_dump/
+-rw-r--r--   0 root         (0) root         (0)      887 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/config_dump/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4666 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/config_dump/full_ini_config_dump.py
+-rw-r--r--   0 root         (0) root         (0)     2592 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/config_dump/human_readable_config_dump.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/config_dump/minimal_ini_config_dump.py
+-rw-r--r--   0 root         (0) root         (0)     1209 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/config_dump/utils.py
+-rw-r--r--   0 root         (0) root         (0)     1572 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/config_file_encoding.py
+-rw-r--r--   0 root         (0) root         (0)    16667 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/config_namespace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:26.479759 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/
+-rw-r--r--   0 root         (0) root         (0)      869 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5135 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/collective_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3630 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/command_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     1556 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     1369 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/configuration_for_namespace_view.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/configuration_item.py
+-rw-r--r--   0 root         (0) root         (0)     1318 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/configuration_view.py
+-rw-r--r--   0 root         (0) root         (0)     1415 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/global_configuration.py
+-rw-r--r--   0 root         (0) root         (0)    12911 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration_validation.py
+-rw-r--r--   0 root         (0) root         (0)     2708 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/determine_invoked_command.py
+-rw-r--r--   0 root         (0) root         (0)     1291 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:26.479759 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/explain/
+-rw-r--r--   0 root         (0) root         (0)      675 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/explain/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10309 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/explain/explain.py
+-rw-r--r--   0 root         (0) root         (0)     2979 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/explain/find_parameters.py
+-rw-r--r--   0 root         (0) root         (0)     2387 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/explain/namespace_tree.py
+-rw-r--r--   0 root         (0) root         (0)      914 2023-02-20 12:11:10.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/explain/template.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:26.479759 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/expression_parser/
+-rw-r--r--   0 root         (0) root         (0)     1565 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/expression_parser/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1830 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/expression_parser/evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     5035 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/expression_parser/grammar.py
+-rw-r--r--   0 root         (0) root         (0)     1354 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/expression_parser/lexeme_stream.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/expression_parser/parser.py
+-rw-r--r--   0 root         (0) root         (0)     1483 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/expression_parser/tokenizer.py
+-rw-r--r--   0 root         (0) root         (0)     3291 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/factory_method_factory.py
+-rw-r--r--   0 root         (0) root         (0)     1092 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/global_config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:26.483759 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/
+-rw-r--r--   0 root         (0) root         (0)     1036 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3704 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/generate_sources.py
+-rw-r--r--   0 root         (0) root         (0)     1630 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/load_boot_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     7440 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/load_collective_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/load_command_configuration.py
+-rw-r--r--   0 root         (0) root         (0)     2161 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/shared.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:26.483759 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/tests/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-02-20 12:11:10.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4625 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/tests/source_decorators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:26.483759 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/
+-rw-r--r--   0 root         (0) root         (0)     1250 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4553 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/enumeration_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     1420 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/optional_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     2120 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/parameter.py
+-rw-r--r--   0 root         (0) root         (0)     2701 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/parameter_creation_completion.py
+-rw-r--r--   0 root         (0) root         (0)     7528 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/parameter_creation_validation.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/positional_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     3179 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/repeating_positional_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     4417 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/simple_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     3077 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/simple_positional_parameter.py
+-rw-r--r--   0 root         (0) root         (0)     2678 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/switch_parameter.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:26.483759 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/tests/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-02-20 12:11:10.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2241 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/tests/optional_parameter_test_case.py
+-rw-r--r--   0 root         (0) root         (0)     7281 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/tests/parameter_test_case.py
+-rw-r--r--   0 root         (0) root         (0)     1001 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/tests/positional_parameter_test_case.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parser_utils.py
+-rw-r--r--   0 root         (0) root         (0)     9221 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/print_help.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:26.487759 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/
+-rw-r--r--   0 root         (0) root         (0)     1055 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2817 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/cli_source.py
+-rw-r--r--   0 root         (0) root         (0)     4528 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/config_file_source.py
+-rw-r--r--   0 root         (0) root         (0)     1452 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/dynamic_default_source.py
+-rw-r--r--   0 root         (0) root         (0)      747 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/enforcing_config_file_source.py
+-rw-r--r--   0 root         (0) root         (0)     3452 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/env_source.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/source.py
+-rw-r--r--   0 root         (0) root         (0)     1270 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/static_default_source.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:26.487759 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/tests/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-02-20 12:11:10.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:26.487759 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/tab_completion/
+-rw-r--r--   0 root         (0) root         (0)      726 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/tab_completion/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2188 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/tab_completion/generate.py
+-rw-r--r--   0 root         (0) root         (0)     2949 2023-02-20 12:11:10.000000 cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/tab_completion/template.sh.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:26.487759 cm-cluster-on-demand-config-9.2.9/cm_cluster_on_demand_config.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      597 2023-02-20 12:11:26.000000 cm-cluster-on-demand-config-9.2.9/cm_cluster_on_demand_config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     4087 2023-02-20 12:11:26.000000 cm-cluster-on-demand-config-9.2.9/cm_cluster_on_demand_config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-20 12:11:26.000000 cm-cluster-on-demand-config-9.2.9/cm_cluster_on_demand_config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2023-02-20 12:11:26.000000 cm-cluster-on-demand-config-9.2.9/cm_cluster_on_demand_config.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2023-02-20 12:11:26.000000 cm-cluster-on-demand-config-9.2.9/cm_cluster_on_demand_config.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-20 12:11:26.487759 cm-cluster-on-demand-config-9.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2041 2023-02-20 12:11:13.000000 cm-cluster-on-demand-config-9.2.9/setup.py
```

### Comparing `cm-cluster-on-demand-config-9.2.8/LICENSE` & `cm-cluster-on-demand-config-9.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-config-9.2.8/PKG-INFO` & `cm-cluster-on-demand-config-9.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm-cluster-on-demand-config
-Version: 9.2.8
+Version: 9.2.9
 Summary: Bright Computing COD configuration library
 Home-page: https://www.brightcomputing.com/
 Author: Cloudteam
 Author-email: cloudteam@brightcomputing.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/__init__.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/argparse_factory.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/argparse_factory.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/command_context.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/command_context.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/config_dump/__init__.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/config_dump/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/config_dump/full_ini_config_dump.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/config_dump/full_ini_config_dump.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/config_dump/human_readable_config_dump.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/config_dump/human_readable_config_dump.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/config_dump/minimal_ini_config_dump.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/config_dump/minimal_ini_config_dump.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/config_dump/utils.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/config_dump/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/config_file_encoding.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/config_file_encoding.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/config_namespace.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/config_namespace.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/__init__.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/collective_configuration.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/collective_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/command_configuration.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/command_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/configuration.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/configuration_for_namespace_view.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/configuration_for_namespace_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/configuration_item.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/configuration_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/configuration_view.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/configuration_view.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration/global_configuration.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration/global_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/configuration_validation.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/configuration_validation.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/determine_invoked_command.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/determine_invoked_command.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/exceptions.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/explain/__init__.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/explain/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/explain/explain.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/explain/explain.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/explain/find_parameters.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/explain/find_parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/explain/namespace_tree.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/explain/namespace_tree.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/explain/template.mako` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/explain/template.mako`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/expression_parser/__init__.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/expression_parser/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/expression_parser/evaluator.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/expression_parser/evaluator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/expression_parser/grammar.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/expression_parser/grammar.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/expression_parser/lexeme_stream.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/expression_parser/lexeme_stream.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/expression_parser/parser.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/expression_parser/parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/expression_parser/tokenizer.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/expression_parser/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/factory_method_factory.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/factory_method_factory.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/global_config.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/global_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/__init__.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/generate_sources.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/generate_sources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/load_boot_configuration.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/load_boot_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/load_collective_configuration.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/load_collective_configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/load_command_configuration.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/load_command_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/shared.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/shared.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/tests/__init__.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/tests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/load_configuration/tests/source_decorators.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/load_configuration/tests/source_decorators.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/__init__.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/enumeration_parameter.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/enumeration_parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/optional_parameter.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/optional_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/parameter.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/parameter_creation_completion.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/parameter_creation_completion.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/parameter_creation_validation.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/parameter_creation_validation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/positional_parameter.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/positional_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/repeating_positional_parameter.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/repeating_positional_parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/simple_parameter.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/simple_parameter.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/simple_positional_parameter.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/simple_positional_parameter.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/switch_parameter.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/switch_parameter.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/tests/__init__.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/tests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/tests/optional_parameter_test_case.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/tests/optional_parameter_test_case.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/tests/parameter_test_case.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/tests/parameter_test_case.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parameter/tests/positional_parameter_test_case.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parameter/tests/positional_parameter_test_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/parser_utils.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/parser_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/print_help.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/print_help.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/__init__.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/cli_source.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/cli_source.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/config_file_source.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/config_file_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/dynamic_default_source.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/dynamic_default_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/enforcing_config_file_source.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/enforcing_config_file_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/env_source.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/env_source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/source.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/static_default_source.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/static_default_source.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/sources/tests/__init__.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/sources/tests/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/tab_completion/__init__.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/tab_completion/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/tab_completion/generate.py` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/tab_completion/generate.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

### Comparing `cm-cluster-on-demand-config-9.2.8/clusterondemandconfig/tab_completion/template.sh.mako` & `cm-cluster-on-demand-config-9.2.9/clusterondemandconfig/tab_completion/template.sh.mako`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-config-9.2.8/cm_cluster_on_demand_config.egg-info/PKG-INFO` & `cm-cluster-on-demand-config-9.2.9/cm_cluster_on_demand_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm-cluster-on-demand-config
-Version: 9.2.8
+Version: 9.2.9
 Summary: Bright Computing COD configuration library
 Home-page: https://www.brightcomputing.com/
 Author: Cloudteam
 Author-email: cloudteam@brightcomputing.com
 License: UNKNOWN
 Platform: UNKNOWN
 Requires-Python: >=3.9
```

### Comparing `cm-cluster-on-demand-config-9.2.8/cm_cluster_on_demand_config.egg-info/SOURCES.txt` & `cm-cluster-on-demand-config-9.2.9/cm_cluster_on_demand_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-config-9.2.8/setup.py` & `cm-cluster-on-demand-config-9.2.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #!/usr/bin/env python
-# Copyright 2004-2022 Bright Computing Holding BV
+# Copyright 2004-2023 Bright Computing Holding BV
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
```

