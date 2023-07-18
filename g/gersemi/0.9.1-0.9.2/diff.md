# Comparing `tmp/gersemi-0.9.1.tar.gz` & `tmp/gersemi-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gersemi-0.9.1.tar", last modified: Thu Jun 15 20:33:49 2023, max compression
+gzip compressed data, was "gersemi-0.9.2.tar", last modified: Tue Jul 18 13:55:25 2023, max compression
```

## Comparing `gersemi-0.9.1.tar` & `gersemi-0.9.2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:49.729003 gersemi-0.9.1/
--rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-06-15 20:33:41.000000 gersemi-0.9.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-06-15 20:33:49.729003 gersemi-0.9.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-06-15 20:33:41.000000 gersemi-0.9.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:49.725003 gersemi-0.9.1/gersemi/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/ast_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/base_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/base_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/builtin_commands
--rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/cmake.lark
--rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:49.729003 gersemi-0.9.1/gersemi/command_invocation_dumpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/ctest_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    24458 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/module_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/multiple_signature_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/project_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/scripting_command_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/specialized_dumpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_invocation_dumpers/two_word_keyword_isolator.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/command_line_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/custom_command_definition_finder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/dumper.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/formatted_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/keyword_with_pairs_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/keywords.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/parsing_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/postprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/result.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/return_codes.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/sanity_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/task_result.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:49.729003 gersemi-0.9.1/gersemi/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      818 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/tasks/check_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/tasks/format_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/tasks/forward_to_stdout.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/tasks/rewrite_in_place.py
--rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/tasks/show_diff.py
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-06-15 20:33:41.000000 gersemi-0.9.1/gersemi/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:49.725003 gersemi-0.9.1/gersemi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-06-15 20:33:49.000000 gersemi-0.9.1/gersemi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-06-15 20:33:49.000000 gersemi-0.9.1/gersemi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-15 20:33:49.000000 gersemi-0.9.1/gersemi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-15 20:33:49.000000 gersemi-0.9.1/gersemi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-15 20:33:49.000000 gersemi-0.9.1/gersemi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-15 20:33:49.000000 gersemi-0.9.1/gersemi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-15 20:33:49.729003 gersemi-0.9.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-06-15 20:33:41.000000 gersemi-0.9.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-15 20:33:49.729003 gersemi-0.9.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-06-15 20:33:41.000000 gersemi-0.9.1/tests/test_custom_command_dumper_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-06-15 20:33:41.000000 gersemi-0.9.1/tests/test_custom_command_formatting.py
--rw-r--r--   0 runner    (1001) docker     (123)    28369 2023-06-15 20:33:41.000000 gersemi-0.9.1/tests/test_executable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-06-15 20:33:41.000000 gersemi-0.9.1/tests/test_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-06-15 20:33:41.000000 gersemi-0.9.1/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-15 20:33:41.000000 gersemi-0.9.1/tests/test_profiling.py
--rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-06-15 20:33:41.000000 gersemi-0.9.1/tests/tests_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:55:25.961280 gersemi-0.9.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    16724 2023-07-18 13:55:16.000000 gersemi-0.9.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-07-18 13:55:25.961280 gersemi-0.9.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15532 2023-07-18 13:55:16.000000 gersemi-0.9.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:55:25.957280 gersemi-0.9.2/gersemi/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5646 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/ast_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/base_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/base_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10717 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/builtin_commands
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3626 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/cmake.lark
+-rw-r--r--   0 runner    (1001) docker     (123)     2395 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/command_invocation_dumper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:55:25.961280 gersemi-0.9.2/gersemi/command_invocation_dumpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/command_invocation_dumpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3359 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/command_invocation_dumpers/ctest_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24458 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/command_invocation_dumpers/module_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/command_invocation_dumpers/multiple_signature_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3518 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18273 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/command_invocation_dumpers/project_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33017 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/command_invocation_dumpers/scripting_command_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1769 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      779 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/command_invocation_dumpers/specialized_dumpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1998 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/command_invocation_dumpers/two_word_keyword_isolator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/command_line_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3472 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/custom_command_definition_finder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/dumper.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/formatted_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/keyword_with_pairs_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/parsing_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/postprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/return_codes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/sanity_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/task_result.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:55:25.961280 gersemi-0.9.2/gersemi/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/tasks/check_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/tasks/format_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/tasks/forward_to_stdout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/tasks/rewrite_in_place.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1668 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/tasks/show_diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-18 13:55:16.000000 gersemi-0.9.2/gersemi/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:55:25.957280 gersemi-0.9.2/gersemi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16554 2023-07-18 13:55:25.000000 gersemi-0.9.2/gersemi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2224 2023-07-18 13:55:25.000000 gersemi-0.9.2/gersemi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 13:55:25.000000 gersemi-0.9.2/gersemi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-18 13:55:25.000000 gersemi-0.9.2/gersemi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-18 13:55:25.000000 gersemi-0.9.2/gersemi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 13:55:25.000000 gersemi-0.9.2/gersemi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 13:55:25.961280 gersemi-0.9.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-07-18 13:55:16.000000 gersemi-0.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 13:55:25.961280 gersemi-0.9.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-18 13:55:16.000000 gersemi-0.9.2/tests/test_custom_command_dumper_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3703 2023-07-18 13:55:16.000000 gersemi-0.9.2/tests/test_custom_command_formatting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28369 2023-07-18 13:55:16.000000 gersemi-0.9.2/tests/test_executable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-07-18 13:55:16.000000 gersemi-0.9.2/tests/test_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1323 2023-07-18 13:55:16.000000 gersemi-0.9.2/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-07-18 13:55:16.000000 gersemi-0.9.2/tests/test_profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3114 2023-07-18 13:55:16.000000 gersemi-0.9.2/tests/tests_generator.py
```

### Comparing `gersemi-0.9.1/LICENSE` & `gersemi-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/PKG-INFO` & `gersemi-0.9.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gersemi
-Version: 0.9.1
+Version: 0.9.2
 Summary: A formatter to make your CMake code the real treasure
 Home-page: https://github.com/BlankSpruce/gersemi
 Author: Blank Spruce
 Author-email: blankspruce@protonmail.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -89,15 +89,15 @@
 
 ### [pre-commit](https://pre-commit.com/) hook
 
 You can use gersemi with a pre-commit hook by adding the following to `.pre-commit-config.yaml` of your repository:
 ```yaml
 repos:
 - repo: https://github.com/BlankSpruce/gersemi
-  rev: 0.8.3
+  rev: 0.9.2
   hooks:
   - id: gersemi
 ```
 
 Update `rev` to relevant version used in your repository. For more details refer to https://pre-commit.com/#using-the-latest-version-for-a-repository
 
 ## Formatting
```

### Comparing `gersemi-0.9.1/README.md` & `gersemi-0.9.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
 
 ### [pre-commit](https://pre-commit.com/) hook
 
 You can use gersemi with a pre-commit hook by adding the following to `.pre-commit-config.yaml` of your repository:
 ```yaml
 repos:
 - repo: https://github.com/BlankSpruce/gersemi
-  rev: 0.8.3
+  rev: 0.9.2
   hooks:
   - id: gersemi
 ```
 
 Update `rev` to relevant version used in your repository. For more details refer to https://pre-commit.com/#using-the-latest-version-for-a-repository
 
 ## Formatting
```

### Comparing `gersemi-0.9.1/gersemi/__main__.py` & `gersemi-0.9.2/gersemi/__main__.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/ast_helpers.py` & `gersemi-0.9.2/gersemi/ast_helpers.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/base_command_invocation_dumper.py` & `gersemi-0.9.2/gersemi/base_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/base_dumper.py` & `gersemi-0.9.2/gersemi/base_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/builtin_commands` & `gersemi-0.9.2/gersemi/builtin_commands`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/cache.py` & `gersemi-0.9.2/gersemi/cache.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/cmake.lark` & `gersemi-0.9.2/gersemi/cmake.lark`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/command_invocation_dumper.py` & `gersemi-0.9.2/gersemi/command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py` & `gersemi-0.9.2/gersemi/command_invocation_dumpers/argument_aware_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py` & `gersemi-0.9.2/gersemi/command_invocation_dumpers/condition_syntax_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/command_invocation_dumpers/ctest_command_dumpers.py` & `gersemi-0.9.2/gersemi/command_invocation_dumpers/ctest_command_dumpers.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/command_invocation_dumpers/module_command_dumpers.py` & `gersemi-0.9.2/gersemi/command_invocation_dumpers/module_command_dumpers.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/command_invocation_dumpers/multiple_signature_command_invocation_dumper.py` & `gersemi-0.9.2/gersemi/command_invocation_dumpers/multiple_signature_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py` & `gersemi-0.9.2/gersemi/command_invocation_dumpers/preserving_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/command_invocation_dumpers/project_command_dumpers.py` & `gersemi-0.9.2/gersemi/command_invocation_dumpers/project_command_dumpers.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/command_invocation_dumpers/scripting_command_dumpers.py` & `gersemi-0.9.2/gersemi/command_invocation_dumpers/scripting_command_dumpers.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py` & `gersemi-0.9.2/gersemi/command_invocation_dumpers/section_aware_command_invocation_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/command_invocation_dumpers/specialized_dumpers.py` & `gersemi-0.9.2/gersemi/command_invocation_dumpers/specialized_dumpers.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py` & `gersemi-0.9.2/gersemi/command_invocation_dumpers/target_link_libraries_command_dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/command_invocation_dumpers/two_word_keyword_isolator.py` & `gersemi-0.9.2/gersemi/command_invocation_dumpers/two_word_keyword_isolator.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/command_line_formatter.py` & `gersemi-0.9.2/gersemi/command_line_formatter.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/configuration.py` & `gersemi-0.9.2/gersemi/configuration.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/custom_command_definition_finder.py` & `gersemi-0.9.2/gersemi/custom_command_definition_finder.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/dumper.py` & `gersemi-0.9.2/gersemi/dumper.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/exceptions.py` & `gersemi-0.9.2/gersemi/exceptions.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/formatter.py` & `gersemi-0.9.2/gersemi/formatter.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/keyword_with_pairs_formatter.py` & `gersemi-0.9.2/gersemi/keyword_with_pairs_formatter.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/parser.py` & `gersemi-0.9.2/gersemi/parser.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/parsing_transformer.py` & `gersemi-0.9.2/gersemi/parsing_transformer.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/postprocessor.py` & `gersemi-0.9.2/gersemi/postprocessor.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/result.py` & `gersemi-0.9.2/gersemi/result.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/runner.py` & `gersemi-0.9.2/gersemi/runner.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/sanity_checker.py` & `gersemi-0.9.2/gersemi/sanity_checker.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/tasks/check_formatting.py` & `gersemi-0.9.2/gersemi/tasks/check_formatting.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/tasks/format_file.py` & `gersemi-0.9.2/gersemi/tasks/format_file.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/tasks/rewrite_in_place.py` & `gersemi-0.9.2/gersemi/tasks/rewrite_in_place.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/tasks/show_diff.py` & `gersemi-0.9.2/gersemi/tasks/show_diff.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi/utils.py` & `gersemi-0.9.2/gersemi/utils.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/gersemi.egg-info/PKG-INFO` & `gersemi-0.9.2/gersemi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gersemi
-Version: 0.9.1
+Version: 0.9.2
 Summary: A formatter to make your CMake code the real treasure
 Home-page: https://github.com/BlankSpruce/gersemi
 Author: Blank Spruce
 Author-email: blankspruce@protonmail.com
 License: MPL 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -89,15 +89,15 @@
 
 ### [pre-commit](https://pre-commit.com/) hook
 
 You can use gersemi with a pre-commit hook by adding the following to `.pre-commit-config.yaml` of your repository:
 ```yaml
 repos:
 - repo: https://github.com/BlankSpruce/gersemi
-  rev: 0.8.3
+  rev: 0.9.2
   hooks:
   - id: gersemi
 ```
 
 Update `rev` to relevant version used in your repository. For more details refer to https://pre-commit.com/#using-the-latest-version-for-a-repository
 
 ## Formatting
```

### Comparing `gersemi-0.9.1/gersemi.egg-info/SOURCES.txt` & `gersemi-0.9.2/gersemi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/setup.py` & `gersemi-0.9.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     url=about["__url__"],
     packages=find_packages(include=["gersemi", "gersemi.*"]),
     package_data={"gersemi": ["cmake.lark", "builtin_commands"]},
     install_requires=[
         "appdirs",
         "dataclasses",
         "lark>=1.0",
-        "pyyaml>=5,<6",
+        "pyyaml>=5,<7",
     ],
     extras_requires=["colorama>=0.4"],
     python_requires=">=3.6",
     entry_points={"console_scripts": ["gersemi = gersemi.__main__:main"]},
     license=about["__license__"],
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `gersemi-0.9.1/tests/test_custom_command_dumper_generation.py` & `gersemi-0.9.2/tests/test_custom_command_dumper_generation.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/tests/test_custom_command_formatting.py` & `gersemi-0.9.2/tests/test_custom_command_formatting.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/tests/test_executable.py` & `gersemi-0.9.2/tests/test_executable.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/tests/test_formatter.py` & `gersemi-0.9.2/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/tests/test_parser.py` & `gersemi-0.9.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `gersemi-0.9.1/tests/tests_generator.py` & `gersemi-0.9.2/tests/tests_generator.py`

 * *Files identical despite different names*

