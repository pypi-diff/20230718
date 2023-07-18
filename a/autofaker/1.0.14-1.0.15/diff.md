# Comparing `tmp/autofaker-1.0.14.tar.gz` & `tmp/autofaker-1.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autofaker-1.0.14.tar", last modified: Thu Apr 20 10:34:49 2023, max compression
+gzip compressed data, was "autofaker-1.0.15.tar", last modified: Tue Jul 18 15:51:20 2023, max compression
```

## Comparing `autofaker-1.0.14.tar` & `autofaker-1.0.15.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:34:49.104710 autofaker-1.0.14/
--rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-20 10:34:20.000000 autofaker-1.0.14/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-20 10:34:20.000000 autofaker-1.0.14/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-04-20 10:34:49.104710 autofaker-1.0.14/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-04-20 10:34:20.000000 autofaker-1.0.14/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-20 10:34:20.000000 autofaker-1.0.14/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 10:34:49.104710 autofaker-1.0.14/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-04-20 10:34:33.000000 autofaker-1.0.14/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:34:49.096710 autofaker-1.0.14/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:34:49.096710 autofaker-1.0.14/src/autofaker/
--rw-r--r--   0 runner    (1001) docker     (123)      215 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/autodata.py
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1005 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     4964 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4872 2023-04-20 10:34:20.000000 autofaker-1.0.14/src/autofaker/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:34:49.100710 autofaker-1.0.14/src/autofaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-04-20 10:34:48.000000 autofaker-1.0.14/src/autofaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-04-20 10:34:49.000000 autofaker-1.0.14/src/autofaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 10:34:48.000000 autofaker-1.0.14/src/autofaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-20 10:34:48.000000 autofaker-1.0.14/src/autofaker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-20 10:34:48.000000 autofaker-1.0.14/src/autofaker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:34:49.104710 autofaker-1.0.14/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:34:49.104710 autofaker-1.0.14/tests/pytests/
--rw-r--r--   0 runner    (1001) docker     (123)     7156 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/pytests/test_decorator_anonymous_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/pytests/test_decorator_anonymous_data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/pytests/test_decorator_anonymous_data_classes_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/pytests/test_decorator_anonymous_dataframe_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/pytests/test_decorator_anonymous_enum_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/pytests/test_decorator_anonymous_nested_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/pytests/test_decorator_anonymous_simple_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_complex_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_data_class_with_fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3941 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3281 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_data_classes_with_fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5507 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_dataframe_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      822 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_dataframe_with_fakes.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_enum_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_nested_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3021 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_nested_classes_with_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)      928 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_simple_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7483 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_anonymous_sut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_many_anonymous_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_many_anonymous_dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_many_anonymous_nested_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_many_anonymous_nested_classes_with_lists.py
--rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_create_many_anonymous_simple_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/test_decorator_exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 10:34:49.104710 autofaker-1.0.14/tests/unittests/
--rw-r--r--   0 runner    (1001) docker     (123)     8712 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/unittests/test_decorator_anonymous_builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/unittests/test_decorator_anonymous_data_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/unittests/test_decorator_anonymous_data_classes_nested.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/unittests/test_decorator_anonymous_dataframe_pandas.py
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/unittests/test_decorator_anonymous_enum_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3669 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/unittests/test_decorator_anonymous_nested_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-04-20 10:34:20.000000 autofaker-1.0.14/tests/unittests/test_decorator_anonymous_simple_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:51:20.920544 autofaker-1.0.15/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-07-18 15:51:00.000000 autofaker-1.0.15/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-18 15:51:00.000000 autofaker-1.0.15/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-07-18 15:51:20.920544 autofaker-1.0.15/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11288 2023-07-18 15:51:00.000000 autofaker-1.0.15/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-18 15:51:00.000000 autofaker-1.0.15/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 15:51:20.920544 autofaker-1.0.15/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-07-18 15:51:08.000000 autofaker-1.0.15/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:51:20.908544 autofaker-1.0.15/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:51:20.912544 autofaker-1.0.15/src/autofaker/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-07-18 15:51:00.000000 autofaker-1.0.15/src/autofaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-07-18 15:51:00.000000 autofaker-1.0.15/src/autofaker/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-18 15:51:00.000000 autofaker-1.0.15/src/autofaker/autodata.py
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-18 15:51:00.000000 autofaker-1.0.15/src/autofaker/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-07-18 15:51:00.000000 autofaker-1.0.15/src/autofaker/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      941 2023-07-18 15:51:00.000000 autofaker-1.0.15/src/autofaker/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-18 15:51:00.000000 autofaker-1.0.15/src/autofaker/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-07-18 15:51:00.000000 autofaker-1.0.15/src/autofaker/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-07-18 15:51:00.000000 autofaker-1.0.15/src/autofaker/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-07-18 15:51:00.000000 autofaker-1.0.15/src/autofaker/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      765 2023-07-18 15:51:00.000000 autofaker-1.0.15/src/autofaker/fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-07-18 15:51:00.000000 autofaker-1.0.15/src/autofaker/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:51:20.912544 autofaker-1.0.15/src/autofaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13912 2023-07-18 15:51:20.000000 autofaker-1.0.15/src/autofaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2274 2023-07-18 15:51:20.000000 autofaker-1.0.15/src/autofaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:51:20.000000 autofaker-1.0.15/src/autofaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-07-18 15:51:20.000000 autofaker-1.0.15/src/autofaker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-18 15:51:20.000000 autofaker-1.0.15/src/autofaker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:51:20.916544 autofaker-1.0.15/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:51:20.916544 autofaker-1.0.15/tests/pytests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5959 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/pytests/test_decorator_anonymous_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2361 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/pytests/test_decorator_anonymous_data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/pytests/test_decorator_anonymous_data_classes_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2573 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/pytests/test_decorator_anonymous_dataframe_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/pytests/test_decorator_anonymous_enum_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/pytests/test_decorator_anonymous_nested_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2586 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/pytests/test_decorator_anonymous_simple_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_anonymous_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_anonymous_complex_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3271 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_anonymous_data_class_with_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3959 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_anonymous_data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3723 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_anonymous_data_classes_with_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5623 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_anonymous_dataframe_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_anonymous_dataframe_with_fakes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_anonymous_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_anonymous_enum_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_anonymous_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2103 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_anonymous_nested_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_anonymous_nested_classes_with_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_anonymous_simple_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_anonymous_sut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_many_anonymous_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_many_anonymous_dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2420 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_many_anonymous_nested_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_many_anonymous_nested_classes_with_lists.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_create_many_anonymous_simple_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/test_decorator_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:51:20.916544 autofaker-1.0.15/tests/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)     7451 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/unittests/test_decorator_anonymous_builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/unittests/test_decorator_anonymous_data_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/unittests/test_decorator_anonymous_data_classes_nested.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/unittests/test_decorator_anonymous_dataframe_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/unittests/test_decorator_anonymous_enum_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3793 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/unittests/test_decorator_anonymous_nested_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3105 2023-07-18 15:51:00.000000 autofaker-1.0.15/tests/unittests/test_decorator_anonymous_simple_classes.py
```

### Comparing `autofaker-1.0.14/LICENSE` & `autofaker-1.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.14/PKG-INFO` & `autofaker-1.0.15/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofaker
-Version: 1.0.14
+Version: 1.0.15
 Summary: Python library designed to minimize the setup/arrange phase of your unit tests
 Home-page: https://github.com/christianhelle/autofaker
 Author: Christian Helle
 Author-email: christian.helle@outlook.com
 License: MIT License
 Description: AutoFaker is a Python library designed to minimize the setup/arrange phase of your unit tests by removing the need to manually 
         write code to create anonymous variables as part of a test cases setup/arrange phase.
```

### Comparing `autofaker-1.0.14/README.md` & `autofaker-1.0.15/README.md`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.14/src/autofaker/attributes.py` & `autofaker-1.0.15/src/autofaker/attributes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 class Attributes:
     def __init__(self, instance):
         self.instance = instance
 
     def get_members(self):
         return [
-            attr for attr in dir(self.instance)
+            attr
+            for attr in dir(self.instance)
             if not callable(getattr(self.instance, attr)) and not attr.startswith("__")
         ]
 
     def get_attribute(self, member):
         return getattr(self.instance, member)
 
     def get_typename(self, member):
```

### Comparing `autofaker-1.0.14/src/autofaker/autodata.py` & `autofaker-1.0.15/src/autofaker/autodata.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.14/src/autofaker/builtins.py` & `autofaker-1.0.15/src/autofaker/builtins.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.14/src/autofaker/dataframe.py` & `autofaker-1.0.15/src/autofaker/dataframe.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,16 +11,19 @@
         self.data = []
         for _ in range(rows):
             row = TypeDataGenerator.create(t, use_fake_data=use_fake_data).generate()
             self.data.append(row)
 
     def generate(self):
         members = [
-            attr for attr in dir(self.data[0])
-            if dataclasses.is_dataclass(getattr(self.data[0], attr)) or not callable(getattr(self.data[0], attr)) and not attr.startswith("__")
+            attr
+            for attr in dir(self.data[0])
+            if dataclasses.is_dataclass(getattr(self.data[0], attr))
+            or not callable(getattr(self.data[0], attr))
+            and not attr.startswith("__")
         ]
         rows = []
         for d in self.data:
             row = []
             for member in members:
                 row.append(Attributes(d).get_attribute(member))
             rows.append(row)
```

### Comparing `autofaker-1.0.14/src/autofaker/dates.py` & `autofaker-1.0.15/src/autofaker/dates.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import datetime
 import random
 
 from autofaker.base import TypeDataGeneratorBase
 
 
 def is_date_type(type_name) -> bool:
-    return type_name in [
-        'datetime',
-        'date'
-    ]
+    return type_name in ["datetime", "date"]
 
 
 class DatetimeGenerator(TypeDataGeneratorBase):
     def generate(self):
         year = datetime.date.today().year
-        return datetime.datetime(random.randint(year - 10, year + 10),
-                                 random.randint(1, 12),
-                                 random.randint(1, 28),
-                                 random.randint(0, 23),
-                                 random.randint(0, 59),
-                                 random.randint(0, 59),
-                                 random.randint(0, 999))
+        return datetime.datetime(
+            random.randint(year - 10, year + 10),
+            random.randint(1, 12),
+            random.randint(1, 28),
+            random.randint(0, 23),
+            random.randint(0, 59),
+            random.randint(0, 59),
+            random.randint(0, 999),
+        )
 
 
 class DateGenerator(TypeDataGeneratorBase):
     def generate(self):
         year = datetime.date.today().year
-        return datetime.datetime(random.randint(year - 10, year + 10),
-                                 random.randint(1, 12),
-                                 random.randint(1, 28))
+        return datetime.datetime(
+            random.randint(year - 10, year + 10),
+            random.randint(1, 12),
+            random.randint(1, 28),
+        )
```

### Comparing `autofaker-1.0.14/src/autofaker/decorators.py` & `autofaker-1.0.15/src/autofaker/decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -29,17 +29,29 @@
     :param use_fake_data: bool - Set this to True to use Faker to generate data, otherwise False to generate anonymous data
     :param type types: tuple - The types to generate data. This is optional and will use the arguments from the function being decorated if not specified
     """
 
     def decorator(function):
         def wrapper(*args):
             if __get_class_that_defined_method(function) is None:
-                return function(*tuple(__create_function_args(function, *tuple(types), use_fake_data=use_fake_data)))
-            return function(__get_test_class(*args),
-                            *tuple(__create_function_args(function, *tuple(types), use_fake_data=use_fake_data)))
+                return function(
+                    *tuple(
+                        __create_function_args(
+                            function, *tuple(types), use_fake_data=use_fake_data
+                        )
+                    )
+                )
+            return function(
+                __get_test_class(*args),
+                *tuple(
+                    __create_function_args(
+                        function, *tuple(types), use_fake_data=use_fake_data
+                    )
+                )
+            )
 
         return wrapper
 
     return decorator
 
 
 def fakedata(*types: object):
@@ -61,17 +73,27 @@
 
     :param types: object - The types to generate data. This is optional and will use the arguments from the function being decorated if not specified
     """
 
     def decorator(function):
         def wrapper(*args):
             if __get_class_that_defined_method(function) is None:
-                return function(*tuple(__create_function_args(function, *tuple(types), use_fake_data=True)))
-            return function(__get_test_class(*args),
-                            *tuple(__create_function_args(function, *tuple(types), use_fake_data=True)))
+                return function(
+                    *tuple(
+                        __create_function_args(
+                            function, *tuple(types), use_fake_data=True
+                        )
+                    )
+                )
+            return function(
+                __get_test_class(*args),
+                *tuple(
+                    __create_function_args(function, *tuple(types), use_fake_data=True)
+                )
+            )
 
         return wrapper
 
     return decorator
 
 
 def autopandas(t: object, rows: int = 3, use_fake_data: bool = False):
@@ -81,15 +103,17 @@
     :param type t: object - The class that represents the DataFrame. This can be a plain old class or a @dataclass
     :param type rows: int - The number of rows to generate for the DataFrame (default 3)
     :param use_fake_data: bool - Set this to True to use Faker to generate data, otherwise False to generate anonymous data
     """
 
     def decorator(function):
         def wrapper(*args):
-            pdf = PandasDataFrameGenerator(t, rows, use_fake_data=use_fake_data).generate()
+            pdf = PandasDataFrameGenerator(
+                t, rows, use_fake_data=use_fake_data
+            ).generate()
             if __get_class_that_defined_method(function) is None:
                 return function(pdf)
             return function(__get_test_class(*args), pdf)
 
         return wrapper
 
     return decorator
@@ -104,34 +128,40 @@
     """
     return autopandas(t, rows, use_fake_data=True)
 
 
 def __get_test_class(*args):
     test_class = args[0]
     if issubclass(test_class.__class__, unittest.TestCase) is False:
-        raise NotImplementedError("This way of creating anonymous objects are only supported from unit tests")
+        raise NotImplementedError(
+            "This way of creating anonymous objects are only supported from unit tests"
+        )
     return test_class
 
 
 def __get_class_that_defined_method(meth):
     if inspect.isfunction(meth):
-        cls = getattr(inspect.getmodule(meth),
-                      meth.__qualname__.split('.<locals>', 1)[0].rsplit('.', 1)[0],
-                      None)
+        cls = getattr(
+            inspect.getmodule(meth),
+            meth.__qualname__.split(".<locals>", 1)[0].rsplit(".", 1)[0],
+            None,
+        )
         if isinstance(cls, type):
             return cls
-    return getattr(meth, '__objclass__', None)  # handle special descriptor objects
+    return getattr(meth, "__objclass__", None)  # handle special descriptor objects
 
 
 def __create_function_args(function, *types, use_fake_data: bool = False) -> List:
     values = []
     argtpes = inspect.getfullargspec(function)
     args = argtpes.annotations.values() if types is None or len(types) == 0 else types
     for t in args:
         value = Autodata.create(t, use_fake_data)
         values.append(value)
     pos = 1
     if __get_class_that_defined_method(function) is None:
         pos = 0
     if len(argtpes.args) - pos != len(values):
-        raise ValueError("Missing argument annotations. Please declare the type of every argument")
+        raise ValueError(
+            "Missing argument annotations. Please declare the type of every argument"
+        )
     return values
```

### Comparing `autofaker-1.0.14/src/autofaker/factory.py` & `autofaker-1.0.15/src/autofaker/factory.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,56 @@
 from autofaker.builtins import (
-    IntegerGenerator,
-    FloatGenerator,
     BooleanGenerator,
+    ByteArrayGenerator,
+    BytesGenerator,
     ComplexGenerator,
+    FloatGenerator,
+    IntegerGenerator,
+    MemoryViewGenerator,
     RangeGenerator,
-    BytesGenerator,
-    ByteArrayGenerator,
-    MemoryViewGenerator
 )
-from autofaker.fakes import FakeStringGenerator, StringGenerator, FakeIntegerGenerator
+from autofaker.fakes import FakeIntegerGenerator, FakeStringGenerator, StringGenerator
 
 
 class BuiltinTypeDataGeneratorFactory:
     @staticmethod
     def is_supported(type_name) -> bool:
         return type_name in [
-            'int',
-            'str',
-            'float',
-            'complex',
-            'bool',
-            'range',
-            'bytes',
-            'bytearray',
-            'memoryview'
+            "int",
+            "str",
+            "float",
+            "complex",
+            "bool",
+            "range",
+            "bytes",
+            "bytearray",
+            "memoryview",
         ]
 
     @staticmethod
     def create(type_name, field_name: str = None, use_fake_data: bool = False):
-        if type_name == 'int':
-            return FakeIntegerGenerator() \
-                if field_name is not None and use_fake_data is True \
+        if type_name == "int":
+            return (
+                FakeIntegerGenerator()
+                if field_name is not None and use_fake_data is True
                 else IntegerGenerator()
-        if type_name == 'str':
-            return FakeStringGenerator(field_name) \
-                if field_name is not None and use_fake_data is True \
+            )
+        if type_name == "str":
+            return (
+                FakeStringGenerator(field_name)
+                if field_name is not None and use_fake_data is True
                 else StringGenerator()
-        if type_name == 'float':
+            )
+        if type_name == "float":
             return FloatGenerator()
-        if type_name == 'complex':
+        if type_name == "complex":
             return ComplexGenerator()
-        if type_name == 'bool':
+        if type_name == "bool":
             return BooleanGenerator()
-        if type_name == 'range':
+        if type_name == "range":
             return RangeGenerator()
-        if type_name == 'bytes':
+        if type_name == "bytes":
             return BytesGenerator()
-        if type_name == 'bytearray':
+        if type_name == "bytearray":
             return ByteArrayGenerator()
-        if type_name == 'memoryview':
+        if type_name == "memoryview":
             return MemoryViewGenerator()
```

### Comparing `autofaker-1.0.14/src/autofaker/fakes.py` & `autofaker-1.0.15/src/autofaker/fakes.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.14/src/autofaker/generator.py` & `autofaker-1.0.15/src/autofaker/generator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,65 +1,75 @@
 import dataclasses
 import inspect
 
 import typing_inspect
 
 from autofaker.attributes import Attributes
-from autofaker.dates import DatetimeGenerator, DateGenerator, is_date_type
+from autofaker.dates import DateGenerator, DatetimeGenerator, is_date_type
+from autofaker.enums import EnumGenerator, is_enum
 from autofaker.factory import BuiltinTypeDataGeneratorFactory
 from autofaker.fakes import TypeDataGeneratorBase
-from autofaker.enums import EnumGenerator, is_enum
 
 
 class TypeDataGenerator:
     @staticmethod
-    def create(t, field_name: str = None, use_fake_data: bool = False) -> TypeDataGeneratorBase:
+    def create(
+        t, field_name: str = None, use_fake_data: bool = False
+    ) -> TypeDataGeneratorBase:
         type_name = TypeDataGenerator._get_type_name(t).lower()
         if BuiltinTypeDataGeneratorFactory.is_supported(type_name):
-            return BuiltinTypeDataGeneratorFactory.create(type_name, field_name, use_fake_data)
+            return BuiltinTypeDataGeneratorFactory.create(
+                type_name, field_name, use_fake_data
+            )
         if is_date_type(type_name):
-            return TypeDataGenerator.create_datetime(type_name, field_name, use_fake_data)
-        if type_name == 'list':
+            return TypeDataGenerator.create_datetime(
+                type_name, field_name, use_fake_data
+            )
+        if type_name == "list":
             return ListGenerator(t)
         if is_enum(t):
             return EnumGenerator(t)
-        return DataClassGenerator(t, use_fake_data=use_fake_data) \
-            if dataclasses.is_dataclass(t) \
+        return (
+            DataClassGenerator(t, use_fake_data=use_fake_data)
+            if dataclasses.is_dataclass(t)
             else ClassGenerator(t, use_fake_data=use_fake_data)
+        )
 
     @staticmethod
     def create_datetime(type_name, field_name: str = None, use_fake_data: bool = False):
-        if type_name == 'datetime':
+        if type_name == "datetime":
             return DatetimeGenerator()
-        if type_name == 'date':
+        if type_name == "date":
             return DateGenerator()
 
     @staticmethod
     def _get_type_name(t) -> str:
         try:
             return t.__name__
         except Exception:
             attributes = dir(t)
-            if '_name' in attributes:
+            if "_name" in attributes:
                 return t._name
             return type(t).__name__
 
 
 class DataClassGenerator(TypeDataGeneratorBase):
     def __init__(self, cls, use_fake_data: bool = False):
         self.use_fake_data = use_fake_data
         self.cls = cls
 
     def generate(self):
         args = []
         fields = dataclasses.fields(self.cls)
         for field in fields:
-            generator = TypeDataGenerator.create(field.type, field.name, use_fake_data=self.use_fake_data)
+            generator = TypeDataGenerator.create(
+                field.type, field.name, use_fake_data=self.use_fake_data
+            )
             args.append((field.name, field.type, generator.generate()))
-        name = self.cls.__module__ + '.' + self.cls.__qualname__
+        name = self.cls.__module__ + "." + self.cls.__qualname__
         instance = dataclasses.make_dataclass(name, args)
         return instance
 
 
 class ClassGenerator(TypeDataGeneratorBase):
     def __init__(self, cls, use_fake_data: bool = False):
         self.use_fake_data = use_fake_data
@@ -69,34 +79,35 @@
         if not self._is_supported():
             return None
 
         attributes = Attributes(self.instance)
         members = attributes.get_members()
         for member in members:
             attr = attributes.get_attribute(member)
-            if type(attr).__name__ == 'list':
+            if type(attr).__name__ == "list":
                 for i in range(len(attr)):
                     attr[i] = self._try_generate(attr[i])
             else:
                 attributes.set_value(member, self._try_generate(attr))
         return self.instance
 
     def _is_supported(self):
         import pandas
-        unsupported_types = [
-            pandas.core.frame.DataFrame
-        ]
+
+        unsupported_types = [pandas.core.frame.DataFrame]
         for t in unsupported_types:
             if isinstance(self.instance, t):
                 return False
         return True
 
     def _try_generate(self, attr):
         try:
-            generator = TypeDataGenerator.create(type(attr), use_fake_data=self.use_fake_data)
+            generator = TypeDataGenerator.create(
+                type(attr), use_fake_data=self.use_fake_data
+            )
             return generator.generate()
         except TypeError as e:
             print(e)
 
     def _try_create_instance(self, cls):
         try:
             self.instance = cls()
@@ -108,28 +119,34 @@
         values = []
         for t in init_args.annotations.values():
             origin = typing_inspect.get_origin(t)
             if origin == list:
                 list_arg = typing_inspect.get_args(t)
                 items = []
                 for _ in range(3):
-                    generator = TypeDataGenerator.create(list_arg[0], use_fake_data=self.use_fake_data)
+                    generator = TypeDataGenerator.create(
+                        list_arg[0], use_fake_data=self.use_fake_data
+                    )
                     items.append(generator.generate())
                 values.append(items)
             else:
-                generator = TypeDataGenerator.create(t, use_fake_data=self.use_fake_data)
+                generator = TypeDataGenerator.create(
+                    t, use_fake_data=self.use_fake_data
+                )
                 value = generator.generate()
                 values.append(value)
         self.instance = cls(*tuple(values))
 
 
 class ListGenerator(TypeDataGeneratorBase):
     def __init__(self, t, use_fake_data: bool = False):
         self.use_fake_data = use_fake_data
         self.list_arg = typing_inspect.get_args(t)
 
     def generate(self):
         items = []
         for _ in range(3):
-            generator = TypeDataGenerator.create(self.list_arg[0], use_fake_data=self.use_fake_data)
+            generator = TypeDataGenerator.create(
+                self.list_arg[0], use_fake_data=self.use_fake_data
+            )
             items.append(generator.generate())
         return items
```

### Comparing `autofaker-1.0.14/src/autofaker.egg-info/PKG-INFO` & `autofaker-1.0.15/src/autofaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autofaker
-Version: 1.0.14
+Version: 1.0.15
 Summary: Python library designed to minimize the setup/arrange phase of your unit tests
 Home-page: https://github.com/christianhelle/autofaker
 Author: Christian Helle
 Author-email: christian.helle@outlook.com
 License: MIT License
 Description: AutoFaker is a Python library designed to minimize the setup/arrange phase of your unit tests by removing the need to manually 
         write code to create anonymous variables as part of a test cases setup/arrange phase.
```

### Comparing `autofaker-1.0.14/src/autofaker.egg-info/SOURCES.txt` & `autofaker-1.0.15/src/autofaker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.14/tests/pytests/test_decorator_anonymous_builtins.py` & `autofaker-1.0.15/tests/pytests/test_decorator_anonymous_builtins.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from datetime import datetime, date
+from datetime import date, datetime
 
 from autofaker import autodata, fakedata
 
-
 # Anonymous Primitives Via Decorator Tests
 
+
 @autodata(str)
 def test_create_str_using_decorator(text):
     assert text is not None
 
 
 @autodata(int)
 def test_create_int_using_decorator(number):
@@ -58,14 +58,15 @@
 @autodata(date)
 def test_create_date_using_decorator(d):
     assert None is not d
 
 
 # Anonymous Primitives Via Decorator With Fakes
 
+
 @autodata(str, use_fake_data=True)
 def test_create_str_using_decorator_with_fake_data(text):
     assert text is not None
 
 
 @autodata(int, use_fake_data=True)
 def test_create_int_using_decorator_with_fake_data(number):
@@ -115,49 +116,59 @@
 @autodata(date, use_fake_data=True)
 def test_create_date_using_decorator_with_fake_data(d):
     assert None is not d
 
 
 # Multiple Anonymous Primitives Via Decorator Tests
 
+
 @autodata(str, int, float, complex, range, bytes, bytearray, memoryview)
-def test_create_primitives_using_decorator(text, number, decimal, complex_type, range_type, buffer, buffer2, memview):
+def test_create_primitives_using_decorator(
+    text, number, decimal, complex_type, range_type, buffer, buffer2, memview
+):
     assert text is not None
     assert number != 0
     assert decimal != float()
     assert complex_type != complex()
     assert range_type != range(0)
     assert buffer != bytes()
     assert buffer2 != bytearray()
     assert memview != memoryview(bytes())
 
 
-@autodata(str, int, float, complex, range, bytes, bytearray, memoryview, use_fake_data=True)
-def test_create_primitives_using_decorator_with_fakes(text, number, decimal, complex_type, range_type, buffer, buffer2, memview):
+@autodata(
+    str, int, float, complex, range, bytes, bytearray, memoryview, use_fake_data=True
+)
+def test_create_primitives_using_decorator_with_fakes(
+    text, number, decimal, complex_type, range_type, buffer, buffer2, memview
+):
     assert text is not None
     assert number != 0
     assert decimal != float()
     assert complex_type != complex()
     assert range_type != range(0)
     assert buffer != bytes()
     assert buffer2 != bytearray()
     assert memview != memoryview(bytes())
 
 
 # Multiple Arguments Via Decorator Tests
 
+
 @fakedata()
-def test_create_anonymous_arguments_using_decorator(text: str,
-                                                    number: int,
-                                                    decimal: float,
-                                                    complex_type: complex,
-                                                    range_type: range,
-                                                    buffer: bytes,
-                                                    buffer2: bytearray,
-                                                    memview: memoryview):
+def test_create_anonymous_arguments_using_decorator(
+    text: str,
+    number: int,
+    decimal: float,
+    complex_type: complex,
+    range_type: range,
+    buffer: bytes,
+    buffer2: bytearray,
+    memview: memoryview,
+):
     print(text)
     print(number)
     print(decimal)
     print(complex_type)
     assert text is not None
     assert number != 0
     assert decimal != float()
@@ -165,22 +176,24 @@
     assert range_type != range(0)
     assert buffer != bytes()
     assert buffer2 != bytearray()
     assert memview != memoryview(bytes())
 
 
 @fakedata()
-def test_create_fake_arguments_using_decorator(text: str,
-                                               number: int,
-                                               decimal: float,
-                                               complex_type: complex,
-                                               range_type: range,
-                                               buffer: bytes,
-                                               buffer2: bytearray,
-                                               memview: memoryview):
+def test_create_fake_arguments_using_decorator(
+    text: str,
+    number: int,
+    decimal: float,
+    complex_type: complex,
+    range_type: range,
+    buffer: bytes,
+    buffer2: bytearray,
+    memview: memoryview,
+):
     print(text)
     print(number)
     print(decimal)
     print(complex_type)
     assert text is not None
     assert number != 0
     assert decimal != float()
@@ -188,22 +201,24 @@
     assert range_type != range(0)
     assert buffer != bytes()
     assert buffer2 != bytearray()
     assert memview != memoryview(bytes())
 
 
 @autodata()
-def test_create_arguments_using_decorator(text: str,
-                                          number: int,
-                                          decimal: float,
-                                          complex_type: complex,
-                                          range_type: range,
-                                          buffer: bytes,
-                                          buffer2: bytearray,
-                                          memview: memoryview):
+def test_create_arguments_using_decorator(
+    text: str,
+    number: int,
+    decimal: float,
+    complex_type: complex,
+    range_type: range,
+    buffer: bytes,
+    buffer2: bytearray,
+    memview: memoryview,
+):
     print(text)
     print(number)
     print(decimal)
     print(complex_type)
     assert text is not None
     assert number != 0
     assert decimal != float()
@@ -211,22 +226,24 @@
     assert range_type != range(0)
     assert buffer != bytes()
     assert buffer2 != bytearray()
     assert memview != memoryview(bytes())
 
 
 @autodata(use_fake_data=True)
-def test_create_arguments_using_decorator_with_fakes(text: str,
-                                                     number: int,
-                                                     decimal: float,
-                                                     complex_type: complex,
-                                                     range_type: range,
-                                                     buffer: bytes,
-                                                     buffer2: bytearray,
-                                                     memview: memoryview):
+def test_create_arguments_using_decorator_with_fakes(
+    text: str,
+    number: int,
+    decimal: float,
+    complex_type: complex,
+    range_type: range,
+    buffer: bytes,
+    buffer2: bytearray,
+    memview: memoryview,
+):
     print(text)
     print(number)
     print(decimal)
     print(complex_type)
     assert text is not None
     assert number != 0
     assert decimal != float()
```

### Comparing `autofaker-1.0.14/tests/pytests/test_decorator_anonymous_data_classes.py` & `autofaker-1.0.15/tests/pytests/test_decorator_anonymous_data_classes.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     id: int
     name: str
     text: str
 
 
 # Anonymous DataClass Via Decorator Test Cases
 
+
 @autodata(DataClass)
 def test_create_data_class_using_decorator_returns_not_none(instance):
     assert instance is not None
 
 
 @autodata(DataClass)
 def test_create_data_class_using_decorator_returns_dataclass(instance):
@@ -27,36 +28,41 @@
 def test_create_data_class_returns_instance_with_new_values(instance):
     assert instance.id != int()
     assert instance.name != str()
     assert instance.text != str()
 
 
 @autodata()
-def test_create_data_class_argument_returns_instance_with_new_values(instance: DataClass):
+def test_create_data_class_argument_returns_instance_with_new_values(
+    instance: DataClass,
+):
     assert instance.id != int()
     assert instance.name != str()
     assert instance.text != str()
 
 
 @autodata()
-def test_create_anonymous_data_class_returns_instance_with_new_values(instance: DataClass):
+def test_create_anonymous_data_class_returns_instance_with_new_values(
+    instance: DataClass,
+):
     assert instance.id != int()
     assert instance.name != str()
     assert instance.text != str()
 
 
 @fakedata()
 def test_create_fake_data_class_returns_instance_with_new_values(instance: DataClass):
     assert instance.id != int()
     assert instance.name != str()
     assert instance.text != str()
 
 
 # Anonymous DataClass Via Decorator With Fakes Test Cases
 
+
 @autodata(DataClass, use_fake_data=True)
 def test_create_data_class_using_decorator_returns_not_none_with_fake_data(instance):
     assert instance is not None
 
 
 @autodata(DataClass, use_fake_data=True)
 def test_create_data_class_using_decorator_returns_dataclass_with_fake_data(instance):
@@ -66,18 +72,22 @@
 @autodata(DataClass, use_fake_data=True)
 def test_create_data_class_returns_instance_with_new_values_with_fake_data(instance):
     assert instance.id != int()
     assert instance.text != str()
 
 
 @autodata(use_fake_data=True)
-def test_create_data_class_argument_returns_instance_with_new_values_with_fake_data(instance: DataClass):
+def test_create_data_class_argument_returns_instance_with_new_values_with_fake_data(
+    instance: DataClass,
+):
     assert instance.id != int()
     assert instance.name != str()
     assert instance.text != str()
 
 
 @fakedata()
-def test_create_fake_data_class_returns_instance_with_new_values_with_fake_data(instance: DataClass):
+def test_create_fake_data_class_returns_instance_with_new_values_with_fake_data(
+    instance: DataClass,
+):
     assert instance.id != int()
     assert instance.name != str()
     assert instance.text != str()
```

### Comparing `autofaker-1.0.14/tests/pytests/test_decorator_anonymous_data_classes_nested.py` & `autofaker-1.0.15/tests/pytests/test_decorator_anonymous_data_classes_nested.py`

 * *Files 17% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     name: str
     text: str
     inner: NestedClass
 
 
 # Anonymous Nested Class Via Decorator Test Cases
 
+
 @autodata(NestedClass)
 def test_create_nested_class_using_decorator_returns_not_none(instance):
     assert instance is not None
 
 
 @autodata(NestedClass)
 def test_create_nested_class_using_decorator_returns_dataclass(instance):
@@ -43,36 +44,43 @@
 def test_create_nested_class_returns_instance_with_new_values(instance):
     assert instance.id != 0
     assert instance.inner.id != 0
     assert instance.inner.text != str()
 
 
 @autodata()
-def test_create_nested_class_argument_returns_instance_with_new_values(instance: NestedClass):
+def test_create_nested_class_argument_returns_instance_with_new_values(
+    instance: NestedClass,
+):
     assert instance.id != 0
     assert instance.name != str()
     assert instance.text != str()
 
 
 @autodata()
-def test_create_anonymous_nested_class_returns_instance_with_new_values(instance: NestedClass):
+def test_create_anonymous_nested_class_returns_instance_with_new_values(
+    instance: NestedClass,
+):
     assert instance.id != 0
     assert instance.name != str()
     assert instance.text != str()
 
 
 @fakedata()
-def test_create_fake_nested_class_returns_instance_with_new_values(instance: NestedClass):
+def test_create_fake_nested_class_returns_instance_with_new_values(
+    instance: NestedClass,
+):
     assert instance.id != 0
     assert instance.name != str()
     assert instance.text != str()
 
 
 # Anonymous Double Nested Class Via Decorator With Fakes Test Cases
 
+
 @autodata(DoubleNestedClass, use_fake_data=True)
 def test_create_double_nested_class_using_decorator_returns_not_none(instance):
     assert instance is not None
 
 
 @autodata(DoubleNestedClass, use_fake_data=True)
 def test_create_nested_class_using_decorator_returns_dataclass(instance):
@@ -83,16 +91,20 @@
 def test_create_double_nested_class_returns_instance_with_new_values(instance):
     assert instance.id != 0
     assert instance.inner.inner.id != 0
     assert instance.inner.inner.text != str()
 
 
 @autodata(use_fake_data=True)
-def test_create_double_nested_class_argument_using_decorator_returns_not_none(instance: DoubleNestedClass):
+def test_create_double_nested_class_argument_using_decorator_returns_not_none(
+    instance: DoubleNestedClass,
+):
     assert instance is not None
 
 
 @fakedata()
-def test_create_double_nested_class_argument_returns_instance_with_new_values(instance: DoubleNestedClass):
+def test_create_double_nested_class_argument_returns_instance_with_new_values(
+    instance: DoubleNestedClass,
+):
     assert instance.id != 0
     assert instance.inner.inner.id != 0
     assert instance.inner.inner.text != str()
```

### Comparing `autofaker-1.0.14/tests/pytests/test_decorator_anonymous_dataframe_pandas.py` & `autofaker-1.0.15/tests/pytests/test_decorator_anonymous_dataframe_pandas.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from dataclasses import dataclass
 
 import pandas
 
-from autofaker import autopandas, fakepandas, autodata
+from autofaker import autodata, autopandas, fakepandas
 
 
 class SimpleClassA:
     id = -1
-    name: 'test'
-    text = 'test'
+    name: "test"
+    text = "test"
 
 
 class SimpleClassB:
     def __init__(self, id: int, name: str, text: str):
         self.text = text
         self.name = name
         self.id = id
@@ -22,85 +22,102 @@
     def __init__(self, a: SimpleClassA, b: SimpleClassB):
         self.b = b
         self.a = a
 
 
 # Anonymous Pandas DataFrame Via Decorator
 
+
 @autopandas(SimpleClassA)
 def test_create_anonymous_pandas_dataframe_returns_not_none(df: pandas.DataFrame):
     assert df is not None
 
 
 @autopandas(SimpleClassA, 10)
-def test_create_anonymous_pandas_dataframe_with_rowcount_returns_not_empty(df: pandas.DataFrame):
+def test_create_anonymous_pandas_dataframe_with_rowcount_returns_not_empty(
+    df: pandas.DataFrame,
+):
     assert len(df.index) != 0
 
 
 @fakepandas(SimpleClassA)
 def test_create_fake_pandas_dataframe_returns_not_none(df: pandas.DataFrame):
     assert df is not None
 
 
 @fakepandas(SimpleClassA, 10)
-def test_create_fake_pandas_dataframe_with_rowcount_returns_not_empty(df: pandas.DataFrame):
+def test_create_fake_pandas_dataframe_with_rowcount_returns_not_empty(
+    df: pandas.DataFrame,
+):
     assert len(df.index) != 0
 
 
 @autopandas(SimpleClassA)
 def test_can_create_anonymous_pandas_dataframes(cls):
     print(cls)
     assert not cls.empty
 
 
 @autopandas(SimpleClassB)
-def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_arguments(cls):
+def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_arguments(
+    cls,
+):
     print(cls)
     assert not cls.empty
 
 
 @autopandas(SimpleClassC)
-def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_class_arguments(cls):
+def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_class_arguments(
+    cls,
+):
     print(cls)
     assert not cls.empty
 
 
 @dataclass
 class DataClass:
     id: int
     name: str
     text: str
 
 
 # Anonymous Pandas DataFrame Via Decorator From DataClass
 
+
 @autopandas(DataClass)
 def test_create_anonymous_pandas_dataframe_returns_not_none(df: pandas.DataFrame):
     assert df is not None
 
 
 @autopandas(DataClass, 10)
-def test_create_anonymous_pandas_dataframe_with_rowcount_returns_not_empty(df: pandas.DataFrame):
+def test_create_anonymous_pandas_dataframe_with_rowcount_returns_not_empty(
+    df: pandas.DataFrame,
+):
     assert len(df.index) != 0
 
 
 @fakepandas(DataClass, 10)
-def test_create_fake_pandas_dataframe_with_rowcount_returns_not_empty(df: pandas.DataFrame):
+def test_create_fake_pandas_dataframe_with_rowcount_returns_not_empty(
+    df: pandas.DataFrame,
+):
     assert len(df.index) != 0
 
 
 @fakepandas(DataClass)
 def test_create_fake_pandas_dataframe_returns_not_none(df: pandas.DataFrame):
     assert df is not None
 
 
 # Autodata Decorator Ignores Pandas
 
+
 @autodata()
 def test_autodata_decorator_ignores_pandas_dataframe(df: pandas.DataFrame):
     assert df is None
 
 
 @autodata()
-def test_autodata_decorator_ignores_only_pandas_dataframe(text: str, df: pandas.DataFrame):
+def test_autodata_decorator_ignores_only_pandas_dataframe(
+    text: str, df: pandas.DataFrame
+):
     assert None is not text
     assert df is None
```

### Comparing `autofaker-1.0.14/tests/pytests/test_decorator_anonymous_nested_classes.py` & `autofaker-1.0.15/tests/pytests/test_decorator_anonymous_nested_classes.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,33 @@
 from autofaker import autodata, fakedata
 
 
 class SimpleClass:
     id = -1
-    name = 'name'
-    text = 'test'
+    name = "name"
+    text = "test"
 
 
 class NestedClass:
     id = -1
-    name = 'name'
-    text = 'test'
+    name = "name"
+    text = "test"
     inner = SimpleClass()
 
 
 class DoubleNestedClass:
     id = -1
-    name = 'name'
-    text = 'test'
+    name = "name"
+    text = "test"
     inner = NestedClass()
 
 
 # Anonymous Nested Class Via Decorator
 
+
 @autodata(NestedClass)
 def test_create_nested_class_using_decorator_returns_not_none(instance):
     assert instance is not None
 
 
 @autodata(NestedClass)
 def test_create_nested_class_using_decorator_returns_instance(instance):
@@ -37,63 +38,82 @@
 def test_create_nested_class_returns_instance_with_new_values(instance):
     assert instance.id != NestedClass().id
     assert instance.inner.id != SimpleClass().id
     assert instance.inner.text != SimpleClass().text
 
 
 @autodata()
-def test_create_nested_class_argument_returns_instance_with_new_values(instance: NestedClass):
+def test_create_nested_class_argument_returns_instance_with_new_values(
+    instance: NestedClass,
+):
     assert instance.id != NestedClass().id
     assert instance.inner.id != SimpleClass().id
     assert instance.inner.text != SimpleClass().text
 
 
 @autodata()
-def test_create_anonymous_nested_class_returns_instance_with_new_values(instance: NestedClass):
+def test_create_anonymous_nested_class_returns_instance_with_new_values(
+    instance: NestedClass,
+):
     assert instance.id != SimpleClass().id
     assert instance.name != SimpleClass().name
     assert instance.text != SimpleClass().text
 
 
 @fakedata()
-def test_create_fake_nested_class_returns_instance_with_new_values(instance: NestedClass):
+def test_create_fake_nested_class_returns_instance_with_new_values(
+    instance: NestedClass,
+):
     assert instance.id != NestedClass().id
     assert instance.name != SimpleClass().name
     assert instance.text != SimpleClass().text
 
 
 # Anonymous Double Nested Class Via Decorator With Fakes
 
+
 @autodata(DoubleNestedClass, use_fake_data=True)
-def test_create_double_nested_class_using_decorator_returns_not_none_with_fake_data(instance):
+def test_create_double_nested_class_using_decorator_returns_not_none_with_fake_data(
+    instance,
+):
     assert instance is not None
 
 
 @autodata(DoubleNestedClass, use_fake_data=True)
-def test_create_double_nested_class_using_decorator_returns_instance_with_fake_data(instance):
+def test_create_double_nested_class_using_decorator_returns_instance_with_fake_data(
+    instance,
+):
     assert isinstance(instance, DoubleNestedClass)
 
 
 @autodata(DoubleNestedClass, use_fake_data=True)
-def test_create_double_nested_class_returns_instance_with_new_values_with_fake_data(instance):
+def test_create_double_nested_class_returns_instance_with_new_values_with_fake_data(
+    instance,
+):
     assert instance.id != DoubleNestedClass().id
     assert instance.inner != DoubleNestedClass().inner
     assert instance.inner.id != DoubleNestedClass().id
     assert instance.inner.text != DoubleNestedClass().text
 
 
 @autodata(use_fake_data=True)
-def test_create_double_nested_class_argument_using_decorator_returns_not_none_with_fake_data(instance: DoubleNestedClass):
+def test_create_double_nested_class_argument_using_decorator_returns_not_none_with_fake_data(
+    instance: DoubleNestedClass,
+):
     assert instance is not None
 
 
 @autodata(use_fake_data=True)
-def test_create_double_nested_class_argument_using_decorator_returns_instance_with_fake_data(instance: DoubleNestedClass):
+def test_create_double_nested_class_argument_using_decorator_returns_instance_with_fake_data(
+    instance: DoubleNestedClass,
+):
     assert isinstance(instance, DoubleNestedClass)
 
 
 @fakedata()
-def test_create_double_nested_class_argument_returns_instance_with_new_values_with_fake_data(instance: DoubleNestedClass):
+def test_create_double_nested_class_argument_returns_instance_with_new_values_with_fake_data(
+    instance: DoubleNestedClass,
+):
     assert instance.id != DoubleNestedClass().id
     assert instance.inner != DoubleNestedClass().inner
     assert instance.inner.id != SimpleClass().id
     assert instance.inner.text != SimpleClass().text
```

### Comparing `autofaker-1.0.14/tests/pytests/test_decorator_anonymous_simple_classes.py` & `autofaker-1.0.15/tests/pytests/test_decorator_anonymous_simple_classes.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from autofaker import autodata, fakedata
 
 
 class SimpleClass:
     id = -1
-    name = 'name'
-    text = 'test'
+    name = "name"
+    text = "test"
 
 
 # Anonymous Simple Class Via Decorator
 
+
 @autodata(SimpleClass)
 def test_create_simple_class_using_decorator_returns_not_none(instance):
     assert instance is not None
 
 
 @autodata(SimpleClass)
 def test_create_simple_class_using_decorator_returns_instance(instance):
@@ -23,36 +24,43 @@
 def test_create_simple_class_returns_instance_with_new_values(instance):
     assert instance.id != SimpleClass().id
     assert instance.name != SimpleClass().name
     assert instance.text != SimpleClass().text
 
 
 @autodata()
-def test_create_simple_class_argument_returns_instance_with_new_values(instance: SimpleClass):
+def test_create_simple_class_argument_returns_instance_with_new_values(
+    instance: SimpleClass,
+):
     assert instance.id != SimpleClass().id
     assert instance.name != SimpleClass().name
     assert instance.text != SimpleClass().text
 
 
 @autodata()
-def test_create_anonymous_simple_class_returns_instance_with_new_values(instance: SimpleClass):
+def test_create_anonymous_simple_class_returns_instance_with_new_values(
+    instance: SimpleClass,
+):
     assert instance.id != SimpleClass().id
     assert instance.name != SimpleClass().name
     assert instance.text != SimpleClass().text
 
 
 @fakedata()
-def test_create_fake_simple_class_returns_instance_with_new_values(instance: SimpleClass):
+def test_create_fake_simple_class_returns_instance_with_new_values(
+    instance: SimpleClass,
+):
     assert instance.id != SimpleClass().id
     assert instance.name != SimpleClass().name
     assert instance.text != SimpleClass().text
 
 
 # Anonymous Simple Class Via Decorator With Fakes
 
+
 @autodata(SimpleClass, use_fake_data=True)
 def test_create_simple_class_using_decorator_with_fake_data_returns_not_none(instance):
     assert instance is not None
 
 
 @autodata(SimpleClass, use_fake_data=True)
 def test_create_simple_class_using_decorator_with_fake_data_returns_instance(instance):
@@ -62,18 +70,22 @@
 @autodata(SimpleClass, use_fake_data=True)
 def test_create_simple_class_returns_instance_with_new_values_using_fake_data(instance):
     assert instance.id != SimpleClass().id
     assert instance.text != SimpleClass().text
 
 
 @autodata(use_fake_data=True)
-def test_create_simple_class_argument_returns_instance_with_new_values_using_fake_data(instance: SimpleClass):
+def test_create_simple_class_argument_returns_instance_with_new_values_using_fake_data(
+    instance: SimpleClass,
+):
     assert instance.id != SimpleClass().id
     assert instance.name != SimpleClass().name
     assert instance.text != SimpleClass().text
 
 
 @fakedata()
-def test_create_fake_simple_class_returns_instance_with_new_values_using_fake_data(instance: SimpleClass):
+def test_create_fake_simple_class_returns_instance_with_new_values_using_fake_data(
+    instance: SimpleClass,
+):
     assert instance.id != SimpleClass().id
     assert instance.name != SimpleClass().name
     assert instance.text != SimpleClass().text
```

### Comparing `autofaker-1.0.14/tests/test_create_anonymous_builtins.py` & `autofaker-1.0.15/tests/test_create_anonymous_builtins.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.14/tests/test_create_anonymous_complex_classes.py` & `autofaker-1.0.15/tests/test_create_anonymous_complex_classes.py`

 * *Files 15% similar despite different names*

```diff
@@ -64,15 +64,18 @@
     def test_can_construct_sut(self):
         self.assertIsNotNone(Autodata.create(ConstructorWithClassArguments))
 
     def test_constructed_sut_inner_not_none(self):
         self.assertIsNotNone(Autodata.create(ConstructorWithClassArguments).inner)
 
     def test_constructed_sut_inner_has_correct_type(self):
-        self.assertIsInstance(Autodata.create(ConstructorWithClassArguments).inner, ConstructorWithPrimitiveArguments)
+        self.assertIsInstance(
+            Autodata.create(ConstructorWithClassArguments).inner,
+            ConstructorWithPrimitiveArguments,
+        )
 
 
 class ConstructorWithNestedClassArguments:
     def __init__(self, cls: ConstructorWithClassArguments):
         self.inner = cls
 
 
@@ -80,40 +83,59 @@
     def test_can_construct_sut(self):
         self.assertIsNotNone(Autodata.create(ConstructorWithNestedClassArguments))
 
     def test_constructed_sut_inner_not_none(self):
         self.assertIsNotNone(Autodata.create(ConstructorWithNestedClassArguments).inner)
 
     def test_constructed_sut_inner_has_correct_type(self):
-        self.assertIsInstance(Autodata.create(ConstructorWithNestedClassArguments).inner, ConstructorWithClassArguments)
+        self.assertIsInstance(
+            Autodata.create(ConstructorWithNestedClassArguments).inner,
+            ConstructorWithClassArguments,
+        )
 
     def test_constructed_sut_inner_inner_has_correct_type(self):
-        self.assertIsInstance(Autodata.create(ConstructorWithNestedClassArguments).inner.inner, ConstructorWithPrimitiveArguments)
+        self.assertIsInstance(
+            Autodata.create(ConstructorWithNestedClassArguments).inner.inner,
+            ConstructorWithPrimitiveArguments,
+        )
 
 
 class ConstructorWithDoubleNestedClassArguments:
     def __init__(self, cls: ConstructorWithNestedClassArguments):
         self.inner = cls
 
 
 class ConstructorWithDoubleNestedClassArgumentsTests(unittest.TestCase):
     def test_can_construct_sut(self):
         self.assertIsNotNone(Autodata.create(ConstructorWithDoubleNestedClassArguments))
 
     def test_constructed_sut_inner_not_none(self):
-        self.assertIsNotNone(Autodata.create(ConstructorWithDoubleNestedClassArguments).inner)
+        self.assertIsNotNone(
+            Autodata.create(ConstructorWithDoubleNestedClassArguments).inner
+        )
 
     def test_constructed_sut_inner_has_correct_type(self):
-        self.assertIsInstance(Autodata.create(ConstructorWithDoubleNestedClassArguments).inner, ConstructorWithNestedClassArguments)
+        self.assertIsInstance(
+            Autodata.create(ConstructorWithDoubleNestedClassArguments).inner,
+            ConstructorWithNestedClassArguments,
+        )
 
     def test_constructed_sut_inner_inner_has_correct_type(self):
-        self.assertIsInstance(Autodata.create(ConstructorWithDoubleNestedClassArguments).inner.inner, ConstructorWithClassArguments)
+        self.assertIsInstance(
+            Autodata.create(ConstructorWithDoubleNestedClassArguments).inner.inner,
+            ConstructorWithClassArguments,
+        )
 
     def test_constructed_sut_inner_inner_inner_has_correct_type(self):
-        self.assertIsInstance(Autodata.create(ConstructorWithDoubleNestedClassArguments).inner.inner.inner, ConstructorWithPrimitiveArguments)
+        self.assertIsInstance(
+            Autodata.create(
+                ConstructorWithDoubleNestedClassArguments
+            ).inner.inner.inner,
+            ConstructorWithPrimitiveArguments,
+        )
 
 
 @dataclass
 class DataClass:
     id: int
     name: str
     age: int
@@ -129,21 +151,27 @@
     def test_can_construct_sut(self):
         self.assertIsNotNone(Autodata.create(ConstructorWithDataClassArguments))
 
     def test_constructed_sut_id_not_none(self):
         self.assertIsNotNone(Autodata.create(ConstructorWithDataClassArguments).data.id)
 
     def test_constructed_sut_age_not_none(self):
-        self.assertIsNotNone(Autodata.create(ConstructorWithDataClassArguments).data.age)
+        self.assertIsNotNone(
+            Autodata.create(ConstructorWithDataClassArguments).data.age
+        )
 
     def test_constructed_sut_name_not_none(self):
-        self.assertIsNotNone(Autodata.create(ConstructorWithDataClassArguments).data.name)
+        self.assertIsNotNone(
+            Autodata.create(ConstructorWithDataClassArguments).data.name
+        )
 
     def test_constructed_sut_email_not_none(self):
-        self.assertIsNotNone(Autodata.create(ConstructorWithDataClassArguments).data.email)
+        self.assertIsNotNone(
+            Autodata.create(ConstructorWithDataClassArguments).data.email
+        )
 
 
 class ConstructorWithListArguments:
     def __init__(self, texts: List[str], numbers: List[int]):
         self.numbers = numbers
         self.texts = texts
```

### Comparing `autofaker-1.0.14/tests/test_create_anonymous_data_class_with_fakes.py` & `autofaker-1.0.15/tests/test_create_anonymous_data_class_with_fakes.py`

 * *Files 16% similar despite different names*

```diff
@@ -29,57 +29,75 @@
     text: str
     word: str
 
 
 def is_uuid(s: str):
     try:
         from uuid import UUID
+
         UUID(s)
         return True
     except ValueError:
         return False
 
 
 class AnonymousDataClassWithFakesTestCase(unittest.TestCase):
-
     def test_create_dataclass_name_returns_not_uuid(self):
         self.assertFalse(is_uuid(Autodata.create(DataClass, use_fake_data=True).name))
 
     def test_create_dataclass_first_name_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create(DataClass, use_fake_data=True).first_name))
+        self.assertFalse(
+            is_uuid(Autodata.create(DataClass, use_fake_data=True).first_name)
+        )
 
     def test_create_dataclass_last_name_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create(DataClass, use_fake_data=True).last_name))
+        self.assertFalse(
+            is_uuid(Autodata.create(DataClass, use_fake_data=True).last_name)
+        )
 
     def test_create_dataclass_address_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create(DataClass, use_fake_data=True).address))
+        self.assertFalse(
+            is_uuid(Autodata.create(DataClass, use_fake_data=True).address)
+        )
 
     def test_create_dataclass_job_returns_not_uuid(self):
         self.assertFalse(is_uuid(Autodata.create(DataClass, use_fake_data=True).job))
 
     def test_create_dataclass_country_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create(DataClass, use_fake_data=True).country))
+        self.assertFalse(
+            is_uuid(Autodata.create(DataClass, use_fake_data=True).country)
+        )
 
     def test_create_dataclass_currency_name_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create(DataClass, use_fake_data=True).currency_name))
+        self.assertFalse(
+            is_uuid(Autodata.create(DataClass, use_fake_data=True).currency_name)
+        )
 
     def test_create_dataclass_currency_code_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create(DataClass, use_fake_data=True).currency_code))
+        self.assertFalse(
+            is_uuid(Autodata.create(DataClass, use_fake_data=True).currency_code)
+        )
 
     def test_create_dataclass_email_returns_not_uuid(self):
         self.assertFalse(is_uuid(Autodata.create(DataClass, use_fake_data=True).email))
 
     def test_create_dataclass_safe_email_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create(DataClass, use_fake_data=True).safe_email))
+        self.assertFalse(
+            is_uuid(Autodata.create(DataClass, use_fake_data=True).safe_email)
+        )
 
     def test_create_dataclass_company_email_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create(DataClass, use_fake_data=True).company_email))
+        self.assertFalse(
+            is_uuid(Autodata.create(DataClass, use_fake_data=True).company_email)
+        )
 
     def test_create_dataclass_hostname_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create(DataClass, use_fake_data=True).hostname))
+        self.assertFalse(
+            is_uuid(Autodata.create(DataClass, use_fake_data=True).hostname)
+        )
 
     def test_create_dataclass_ipv4_returns_not_uuid(self):
         self.assertFalse(is_uuid(Autodata.create(DataClass, use_fake_data=True).ipv4))
 
     def test_create_dataclass_ipv6_returns_not_uuid(self):
         self.assertFalse(is_uuid(Autodata.create(DataClass, use_fake_data=True).ipv6))
```

### Comparing `autofaker-1.0.14/tests/test_create_anonymous_data_classes.py` & `autofaker-1.0.15/tests/test_create_anonymous_data_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 @dataclass
 class DataClass:
     id: int
     text: str
 
 
 class AnonymousDataClassTestCase(unittest.TestCase):
-
     def test_create_data_class_returns_not_none(self):
         self.assertIsNotNone(Autodata.create(DataClass))
 
     def test_create_data_class_returns_dataclass(self):
         self.assertTrue(dataclasses.is_dataclass(Autodata.create(DataClass)))
 
     def test_create_many_data_class_returns_not_none(self):
@@ -24,71 +23,70 @@
 
     def test_create_many_data_class_returns_list(self):
         self.assertIsInstance(Autodata.create_many(DataClass), list)
 
     def test_create_many_data_class_returns_dataclass(self):
         data = Autodata.create(DataClass)
         self.assertNotEqual(0, data.id)
-        self.assertNotEqual('', data.text)
+        self.assertNotEqual("", data.text)
 
 
 @dataclass
 class NestedDataClass:
     id: int
     text: str
     inner: DataClass
 
 
 class AnonymousNestedClassTestCase(unittest.TestCase):
-
     def test_create_nested_class_returns_not_none(self):
         self.assertIsNotNone(Autodata.create(NestedDataClass))
 
     def test_create_data_class_returns_dataclass(self):
         self.assertTrue(dataclasses.is_dataclass(Autodata.create(NestedDataClass)))
 
     def test_create_nested_class_returns_instance_with_nested_not_none(self):
         self.assertIsNotNone(Autodata.create(NestedDataClass).inner)
 
     def test_create_nested_class_returns_instance_with_new_nested_instance(self):
         result = Autodata.create(NestedDataClass)
         self.assertNotEqual(result.id, 0)
         self.assertNotEqual(result.inner.id, 0)
-        self.assertNotEqual(result.inner.text, '')
+        self.assertNotEqual(result.inner.text, "")
 
 
 @dataclass
 class DoubleNestedDataClass:
     id: int
     text: str
     inner: NestedDataClass
 
 
 class AnonymousDoubleNestedDataClassTestCase(unittest.TestCase):
-
     def test_create_nested_class_returns_not_none(self):
         self.assertIsNotNone(Autodata.create(DoubleNestedDataClass))
 
     def test_create_data_class_returns_dataclass(self):
-        self.assertTrue(dataclasses.is_dataclass(Autodata.create(DoubleNestedDataClass)))
+        self.assertTrue(
+            dataclasses.is_dataclass(Autodata.create(DoubleNestedDataClass))
+        )
 
     def test_create_nested_class_returns_instance_with_nested_not_none(self):
         self.assertIsNotNone(Autodata.create(DoubleNestedDataClass).inner)
 
     def test_create_nested_class_returns_instance_with_new_nested_instance(self):
         result = Autodata.create(DoubleNestedDataClass)
         self.assertNotEqual(result.id, 0)
         self.assertNotEqual(result.inner.id, 0)
-        self.assertNotEqual(result.inner.text, '')
+        self.assertNotEqual(result.inner.text, "")
         self.assertNotEqual(result.inner.inner.id, 0)
-        self.assertNotEqual(result.inner.inner.text, '')
+        self.assertNotEqual(result.inner.inner.text, "")
 
 
 class AnonymousInlineDataClassTestCase(unittest.TestCase):
-
     def test_create_data_class_returns_not_none(self):
         @dataclass
         class InlineDataClass:
             id: int
             text: str
 
         self.assertIsNotNone(Autodata.create(InlineDataClass))
@@ -121,8 +119,8 @@
         @dataclass
         class InlineDataClass:
             id: int
             text: str
 
         data = Autodata.create(InlineDataClass)
         self.assertNotEqual(0, data.id)
-        self.assertNotEqual('', data.text)
+        self.assertNotEqual("", data.text)
```

### Comparing `autofaker-1.0.14/tests/test_create_anonymous_data_classes_with_fakes.py` & `autofaker-1.0.15/tests/test_create_anonymous_data_classes_with_fakes.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,62 +29,100 @@
     text: str
     word: str
 
 
 def is_uuid(s: str):
     try:
         from uuid import UUID
+
         UUID(s)
         return True
     except ValueError:
         return False
 
 
 class AnonymousDataClassWithFakesTestCase(unittest.TestCase):
-
     def test_create_many_dataclass_name_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].name))
+        self.assertFalse(
+            is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].name)
+        )
 
     def test_create_many_dataclass_first_name_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].first_name))
+        self.assertFalse(
+            is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].first_name)
+        )
 
     def test_create_many_dataclass_last_name_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].last_name))
+        self.assertFalse(
+            is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].last_name)
+        )
 
     def test_create_many_dataclass_address_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].address))
+        self.assertFalse(
+            is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].address)
+        )
 
     def test_create_many_dataclass_job_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].job))
+        self.assertFalse(
+            is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].job)
+        )
 
     def test_create_many_dataclass_country_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].country))
+        self.assertFalse(
+            is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].country)
+        )
 
     def test_create_many_dataclass_currency_name_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].currency_name))
+        self.assertFalse(
+            is_uuid(
+                Autodata.create_many(DataClass, use_fake_data=True)[2].currency_name
+            )
+        )
 
     def test_create_many_dataclass_currency_code_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].currency_code))
+        self.assertFalse(
+            is_uuid(
+                Autodata.create_many(DataClass, use_fake_data=True)[2].currency_code
+            )
+        )
 
     def test_create_many_dataclass_email_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].email))
+        self.assertFalse(
+            is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].email)
+        )
 
     def test_create_many_dataclass_safe_email_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].safe_email))
+        self.assertFalse(
+            is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].safe_email)
+        )
 
     def test_create_many_dataclass_company_email_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].company_email))
+        self.assertFalse(
+            is_uuid(
+                Autodata.create_many(DataClass, use_fake_data=True)[2].company_email
+            )
+        )
 
     def test_create_many_dataclass_hostname_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].hostname))
+        self.assertFalse(
+            is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].hostname)
+        )
 
     def test_create_many_dataclass_ipv4_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].ipv4))
+        self.assertFalse(
+            is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].ipv4)
+        )
 
     def test_create_many_dataclass_ipv6_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].ipv6))
+        self.assertFalse(
+            is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].ipv6)
+        )
 
     def test_create_many_dataclass_text_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].text))
+        self.assertFalse(
+            is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].text)
+        )
 
     def test_create_many_dataclass_word_returns_not_uuid(self):
-        self.assertFalse(is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].word))
+        self.assertFalse(
+            is_uuid(Autodata.create_many(DataClass, use_fake_data=True)[2].word)
+        )
```

### Comparing `autofaker-1.0.14/tests/test_create_anonymous_dataframe_pandas.py` & `autofaker-1.0.15/tests/test_create_anonymous_dataframe_pandas.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from dataclasses import dataclass
 
 from autofaker import Autodata
 
 
 class SimpleClassA:
     id = -1
-    name = 'test'
-    text = 'test'
+    name = "test"
+    text = "test"
 
 
 class SimpleClassB:
     def __init__(self, id: int, name: str, text: str):
         self.text = text
         self.name = name
         self.id = id
@@ -20,63 +20,69 @@
 class SimpleClassC:
     def __init__(self, a: SimpleClassA, b: SimpleClassB):
         self.b = b
         self.a = a
 
 
 class CreateAnonymousPandasDataFrameTests(unittest.TestCase):
-
     def test_create_anonymous_pandas_dataframe_returns_not_none(self):
         df = Autodata.create_pandas_dataframe(SimpleClassA)
         self.assertIsNotNone(df)
 
     def test_create_anonymous_pandas_dataframe_returns_not_empty(self):
         df = Autodata.create_pandas_dataframe(SimpleClassA)
         self.assertNotEqual(len(df.index), 0)
 
     def test_create_anonymous_pandas_dataframe_with_rowcount_returns_not_empty(self):
         df = Autodata.create_pandas_dataframe(SimpleClassA, 10)
         self.assertEqual(len(df.index), 10)
 
-    def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_arguments(self):
+    def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_arguments(
+        self,
+    ):
         df = Autodata.create_pandas_dataframe(SimpleClassB)
-        self.assertTrue('id' in df.columns)
-        self.assertTrue('name' in df.columns)
-        self.assertTrue('text' in df.columns)
-
-    def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_class_arguments(self):
+        self.assertTrue("id" in df.columns)
+        self.assertTrue("name" in df.columns)
+        self.assertTrue("text" in df.columns)
+
+    def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_class_arguments(
+        self,
+    ):
         df = Autodata.create_pandas_dataframe(SimpleClassC)
-        self.assertTrue('a' in df.columns)
-        self.assertTrue('b' in df.columns)
+        self.assertTrue("a" in df.columns)
+        self.assertTrue("b" in df.columns)
 
 
 class CreateFakePandasDataFrameTests(unittest.TestCase):
-
     def test_create_fake_pandas_dataframe_returns_not_none(self):
         df = Autodata.create_pandas_dataframe(SimpleClassA, use_fake_data=True)
         self.assertIsNotNone(df)
 
     def test_create_fake_pandas_dataframe_returns_not_empty(self):
         df = Autodata.create_pandas_dataframe(SimpleClassA, use_fake_data=True)
         self.assertNotEqual(len(df.index), 0)
 
     def test_create_fake_pandas_dataframe_with_rowcount_returns_not_empty(self):
         df = Autodata.create_pandas_dataframe(SimpleClassA, 10, use_fake_data=True)
         self.assertEqual(len(df.index), 10)
 
-    def test_can_create_fake_pandas_dataframes_from_class_with_constructor_arguments(self):
+    def test_can_create_fake_pandas_dataframes_from_class_with_constructor_arguments(
+        self,
+    ):
         df = Autodata.create_pandas_dataframe(SimpleClassB, use_fake_data=True)
-        self.assertTrue('id' in df.columns)
-        self.assertTrue('name' in df.columns)
-        self.assertTrue('text' in df.columns)
-
-    def test_can_create_fake_pandas_dataframes_from_class_with_constructor_class_arguments(self):
+        self.assertTrue("id" in df.columns)
+        self.assertTrue("name" in df.columns)
+        self.assertTrue("text" in df.columns)
+
+    def test_can_create_fake_pandas_dataframes_from_class_with_constructor_class_arguments(
+        self,
+    ):
         df = Autodata.create_pandas_dataframe(SimpleClassC, use_fake_data=True)
-        self.assertTrue('a' in df.columns)
-        self.assertTrue('b' in df.columns)
+        self.assertTrue("a" in df.columns)
+        self.assertTrue("b" in df.columns)
 
 
 @dataclass
 class DataClass:
     id: int
     name: str
     text: str
@@ -92,56 +98,62 @@
     def __init__(self, a: DataClass, b: SimpleClassA, c: HybridClassA):
         self.c = c
         self.b = b
         self.a = a
 
 
 class CreateAnonymousPandasDataFrameFromDataClassTests(unittest.TestCase):
-
     def test_create_anonymous_pandas_dataframe_returns_not_none(self):
         df = Autodata.create_pandas_dataframe(DataClass)
         self.assertIsNotNone(df)
 
     def test_create_anonymous_pandas_dataframe_returns_not_empty(self):
         df = Autodata.create_pandas_dataframe(DataClass)
         self.assertNotEqual(len(df.index), 0)
 
     def test_create_anonymous_pandas_dataframe_with_rowcount_returns_not_empty(self):
         df = Autodata.create_pandas_dataframe(DataClass, 10)
         self.assertEqual(len(df.index), 10)
 
-    def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_class_arguments(self):
+    def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_class_arguments(
+        self,
+    ):
         df = Autodata.create_pandas_dataframe(HybridClassA)
-        self.assertTrue('b' in df.columns)
-        self.assertTrue('a' in df.columns)
+        self.assertTrue("b" in df.columns)
+        self.assertTrue("a" in df.columns)
 
-    def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_hybrid_class_arguments(self):
+    def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_hybrid_class_arguments(
+        self,
+    ):
         df = Autodata.create_pandas_dataframe(HybridClassB)
-        self.assertTrue('c' in df.columns)
-        self.assertTrue('b' in df.columns)
-        self.assertTrue('a' in df.columns)
+        self.assertTrue("c" in df.columns)
+        self.assertTrue("b" in df.columns)
+        self.assertTrue("a" in df.columns)
 
 
 class CreateFakePandasDataFrameFromDataClassTests(unittest.TestCase):
-
     def test_create_fake_pandas_dataframe_returns_not_none(self):
         df = Autodata.create_pandas_dataframe(DataClass, use_fake_data=True)
         self.assertIsNotNone(df)
 
     def test_create_fake_pandas_dataframe_returns_not_empty(self):
         df = Autodata.create_pandas_dataframe(DataClass, use_fake_data=True)
         self.assertNotEqual(len(df.index), 0)
 
     def test_create_fake_pandas_dataframe_with_rowcount_returns_not_empty(self):
         df = Autodata.create_pandas_dataframe(DataClass, 10, use_fake_data=True)
         self.assertEqual(len(df.index), 10)
 
-    def test_can_create_fake_pandas_dataframes_from_class_with_constructor_class_arguments(self):
+    def test_can_create_fake_pandas_dataframes_from_class_with_constructor_class_arguments(
+        self,
+    ):
         df = Autodata.create_pandas_dataframe(HybridClassA, use_fake_data=True)
-        self.assertTrue('b' in df.columns)
-        self.assertTrue('a' in df.columns)
+        self.assertTrue("b" in df.columns)
+        self.assertTrue("a" in df.columns)
 
-    def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_hybrid_class_arguments(self):
+    def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_hybrid_class_arguments(
+        self,
+    ):
         df = Autodata.create_pandas_dataframe(HybridClassB, use_fake_data=True)
-        self.assertTrue('c' in df.columns)
-        self.assertTrue('b' in df.columns)
-        self.assertTrue('a' in df.columns)
+        self.assertTrue("c" in df.columns)
+        self.assertTrue("b" in df.columns)
+        self.assertTrue("a" in df.columns)
```

### Comparing `autofaker-1.0.14/tests/test_create_anonymous_dataframe_with_fakes.py` & `autofaker-1.0.15/tests/test_create_anonymous_dataframe_with_fakes.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -29,20 +29,20 @@
     text: str
     word: str
 
 
 def is_uuid(s: str):
     try:
         from uuid import UUID
+
         UUID(s)
         return True
     except ValueError:
         return False
 
 
 class AnonymousDataClassWithFakesTestCase(unittest.TestCase):
-
     def test_create_pandas_dataframe_returns_not_none(self):
         pdf = Autodata.create_pandas_dataframe(DataClass, use_fake_data=True)
         print()
         print(pdf)
         self.assertIsNotNone(pdf)
```

### Comparing `autofaker-1.0.14/tests/test_create_anonymous_dates.py` & `autofaker-1.0.15/tests/test_create_anonymous_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from datetime import datetime, date
+from datetime import date, datetime
 
 from autofaker import Autodata
 
 
 class AnonymousDatetimeTestCase(unittest.TestCase):
     def test_create_datetime_returns_not_none(self):
         self.assertIsNotNone(Autodata.create(datetime))
```

### Comparing `autofaker-1.0.14/tests/test_create_anonymous_lists.py` & `autofaker-1.0.15/tests/test_create_anonymous_lists.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import unittest
 from abc import abstractmethod
 from dataclasses import dataclass
-from datetime import datetime, date
+from datetime import date, datetime
 from typing import List
 
 from autofaker import Autodata
 
 
 class CreateTestCase(unittest.TestCase):
     @abstractmethod
```

### Comparing `autofaker-1.0.14/tests/test_create_anonymous_nested_classes.py` & `autofaker-1.0.15/tests/test_create_anonymous_nested_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import unittest
 
 from autofaker import Autodata
 
 
 class SimpleClass:
     id = -1
-    text = 'test'
+    text = "test"
 
 
 class NestedClass:
     id = -1
-    text = 'test'
+    text = "test"
     inner = SimpleClass()
 
 
 class DoubleNestedClass:
     id = -1
-    text = 'test'
+    text = "test"
     inner = NestedClass()
 
 
 class AnonymousNestedClassTestCase(unittest.TestCase):
-
     def test_create_nested_class_returns_not_none(self):
         self.assertIsNotNone(Autodata.create(NestedClass))
 
     def test_create_nested_class_returns_instance(self):
         self.assertIsInstance(Autodata.create(NestedClass), NestedClass)
 
     def test_create_nested_class_returns_instance_with_nested_not_none(self):
@@ -35,15 +34,14 @@
         result = Autodata.create(NestedClass)
         self.assertNotEqual(result.id, NestedClass().id)
         self.assertNotEqual(result.inner.id, SimpleClass().id)
         self.assertNotEqual(result.inner.text, SimpleClass().text)
 
 
 class AnonymousDoubleNestedClassTestCase(unittest.TestCase):
-
     def test_create_nested_class_returns_not_none(self):
         self.assertIsNotNone(Autodata.create(DoubleNestedClass))
 
     def test_create_nested_class_returns_instance(self):
         self.assertIsInstance(Autodata.create(DoubleNestedClass), DoubleNestedClass)
 
     def test_create_nested_class_returns_instance_with_nested_not_none(self):
```

### Comparing `autofaker-1.0.14/tests/test_create_anonymous_nested_classes_with_lists.py` & `autofaker-1.0.15/tests/test_create_anonymous_nested_classes_with_lists.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import unittest
 
 from autofaker import Autodata
 
 
 class SimpleClass:
     id = -1
-    text = 'test'
+    text = "test"
 
 
 class NestedWithCollectionClass:
     id = -1
-    text = 'test'
+    text = "test"
     inner = [SimpleClass(), SimpleClass()]
 
 
 class NestedWithNestedCollectionClass:
     id = -1
-    text = 'test'
+    text = "test"
     inner = [NestedWithCollectionClass(), NestedWithCollectionClass()]
 
 
 class AnonymousNestedClassWithCollectionTestCase(unittest.TestCase):
-
     def test_create_nested_class_returns_not_none(self):
         self.assertIsNotNone(Autodata.create(NestedWithCollectionClass))
 
     def test_create_nested_class_returns_instance(self):
-        self.assertIsInstance(Autodata.create(NestedWithCollectionClass), NestedWithCollectionClass)
+        self.assertIsInstance(
+            Autodata.create(NestedWithCollectionClass), NestedWithCollectionClass
+        )
 
     def test_create_nested_class_returns_instance_with_nested_not_none(self):
         self.assertIsNotNone(Autodata.create(NestedWithCollectionClass).inner)
 
     def test_create_nested_class_returns_instance_with_nested_not_empty(self):
         self.assertNotEqual(0, len(Autodata.create(NestedWithCollectionClass).inner))
 
@@ -40,29 +41,34 @@
         for cls in result.inner:
             self.assertIsNotNone(cls)
             self.assertNotEqual(cls.id, SimpleClass().id)
             self.assertNotEqual(cls.text, SimpleClass().text)
 
 
 class AnonymousNestedClassWithNestedCollectionTestCase(unittest.TestCase):
-
     def test_create_nested_class_returns_not_none(self):
         self.assertIsNotNone(Autodata.create(NestedWithCollectionClass))
 
     def test_create_nested_class_returns_instance(self):
-        self.assertIsInstance(Autodata.create(NestedWithCollectionClass), NestedWithCollectionClass)
+        self.assertIsInstance(
+            Autodata.create(NestedWithCollectionClass), NestedWithCollectionClass
+        )
 
     def test_create_nested_class_returns_instance_with_inner_not_none(self):
         self.assertIsNotNone(Autodata.create(NestedWithNestedCollectionClass).inner)
 
     def test_create_nested_class_returns_instance_with_inner_not_empty(self):
-        self.assertNotEqual(0, len(Autodata.create(NestedWithNestedCollectionClass).inner))
+        self.assertNotEqual(
+            0, len(Autodata.create(NestedWithNestedCollectionClass).inner)
+        )
 
     def test_create_nested_class_returns_instance_with_nested_inner_not_empty(self):
-        self.assertNotEqual(0, len(Autodata.create(NestedWithNestedCollectionClass).inner[0].inner))
+        self.assertNotEqual(
+            0, len(Autodata.create(NestedWithNestedCollectionClass).inner[0].inner)
+        )
 
     def test_create_nested_class_returns_instance_with_new_nested_instance(self):
         result = Autodata.create(NestedWithNestedCollectionClass)
         self.assertNotEqual(result.id, NestedWithNestedCollectionClass().id)
         self.assertNotEqual(result.text, NestedWithNestedCollectionClass().text)
         for cls in result.inner:
             self.assertIsNotNone(cls)
```

### Comparing `autofaker-1.0.14/tests/test_create_anonymous_simple_classes.py` & `autofaker-1.0.15/tests/test_create_anonymous_simple_classes.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import unittest
 
 from autofaker import Autodata
 
 
 class AnonymousSimpleClassTestCase(unittest.TestCase):
-
     def test_create_local_class_returns_not_none(self):
         class X:
             pass
 
         self.assertIsNotNone(Autodata.create(X))
 
     def test_create_local_class_returns_instance(self):
@@ -27,8 +26,8 @@
         result = Autodata.create(SimpleClass)
         self.assertNotEqual(result.id, SimpleClass().id)
         self.assertNotEqual(result.text, SimpleClass().text)
 
 
 class SimpleClass:
     id = -1
-    text = 'test'
+    text = "test"
```

### Comparing `autofaker-1.0.14/tests/test_create_anonymous_sut.py` & `autofaker-1.0.15/tests/test_create_anonymous_sut.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,45 +7,50 @@
 
 class Calculator:
     def add(self, number1: int, number2: int):
         return number1 + number2
 
 
 class CalculatorTests(unittest.TestCase):
-
     def test_can_add_two_numbers(self):
         numbers = Autodata.create_many(int, 2)
         sut = Autodata.create(Calculator)
         result = sut.add(numbers[0], numbers[1])
         self.assertEqual(numbers[0] + numbers[1], result)
 
     @autodata(Calculator, int, int)
     def test_can_add_two_numbers_using_test_arguments(self, sut, number1, number2):
         result = sut.add(number1, number2)
         self.assertEqual(number1 + number2, result)
 
     @autodata
-    def test_can_add_two_numbers_using_annotated_arguments(self, sut: Calculator, number1: int, number2: int):
+    def test_can_add_two_numbers_using_annotated_arguments(
+        self, sut: Calculator, number1: int, number2: int
+    ):
         result = sut.add(number1, number2)
         self.assertEqual(number1 + number2, result)
 
     @autodata
-    def test_can_add_two_numbers_using_anonymous_arguments(self, sut: Calculator, number1: int, number2: int):
+    def test_can_add_two_numbers_using_anonymous_arguments(
+        self, sut: Calculator, number1: int, number2: int
+    ):
         result = sut.add(number1, number2)
         self.assertEqual(number1 + number2, result)
 
     @fakedata
-    def test_can_add_two_numbers_using_fake_arguments(self, sut: Calculator, number1: int, number2: int):
+    def test_can_add_two_numbers_using_fake_arguments(
+        self, sut: Calculator, number1: int, number2: int
+    ):
         result = sut.add(number1, number2)
         self.assertEqual(number1 + number2, result)
 
 
 class Person:
     age = 10
-    name = 'test'
+    name = "test"
 
     def get_introduction(self):
         return f"Hi! My name is {self.name} and I'm {self.age} years old"
 
 
 class Staff:
     def __init__(self):
@@ -63,15 +68,14 @@
 
     def introduce(self):
         for person in self.people:
             print(person.get_introduction())
 
 
 class StaffTests(unittest.TestCase):
-
     def test_introduce_everyone(self):
         people = Autodata.create_many(Person)
         sut = Autodata.create(Staff)
         sut.add_people(people)
         sut.introduce()
         self.assertEqual(len(people), sut.get_head_count())
 
@@ -106,15 +110,18 @@
     def test_can_construct_sut(self):
         self.assertIsNotNone(Autodata.create(ConstructorWithClassArguments))
 
     def test_constructed_sut_inner_not_none(self):
         self.assertIsNotNone(Autodata.create(ConstructorWithClassArguments).inner)
 
     def test_constructed_sut_inner_has_correct_type(self):
-        self.assertIsInstance(Autodata.create(ConstructorWithClassArguments).inner, ConstructorWithPrimitiveArguments)
+        self.assertIsInstance(
+            Autodata.create(ConstructorWithClassArguments).inner,
+            ConstructorWithPrimitiveArguments,
+        )
 
 
 class ConstructorWithNestedClassArguments:
     def __init__(self, cls: ConstructorWithClassArguments):
         self.inner = cls
 
 
@@ -122,40 +129,59 @@
     def test_can_construct_sut(self):
         self.assertIsNotNone(Autodata.create(ConstructorWithNestedClassArguments))
 
     def test_constructed_sut_inner_not_none(self):
         self.assertIsNotNone(Autodata.create(ConstructorWithNestedClassArguments).inner)
 
     def test_constructed_sut_inner_has_correct_type(self):
-        self.assertIsInstance(Autodata.create(ConstructorWithNestedClassArguments).inner, ConstructorWithClassArguments)
+        self.assertIsInstance(
+            Autodata.create(ConstructorWithNestedClassArguments).inner,
+            ConstructorWithClassArguments,
+        )
 
     def test_constructed_sut_inner_inner_has_correct_type(self):
-        self.assertIsInstance(Autodata.create(ConstructorWithNestedClassArguments).inner.inner, ConstructorWithPrimitiveArguments)
+        self.assertIsInstance(
+            Autodata.create(ConstructorWithNestedClassArguments).inner.inner,
+            ConstructorWithPrimitiveArguments,
+        )
 
 
 class ConstructorWithDoubleNestedClassArguments:
     def __init__(self, cls: ConstructorWithNestedClassArguments):
         self.inner = cls
 
 
 class ConstructorWithDoubleNestedClassArgumentsTests(unittest.TestCase):
     def test_can_construct_sut(self):
         self.assertIsNotNone(Autodata.create(ConstructorWithDoubleNestedClassArguments))
 
     def test_constructed_sut_inner_not_none(self):
-        self.assertIsNotNone(Autodata.create(ConstructorWithDoubleNestedClassArguments).inner)
+        self.assertIsNotNone(
+            Autodata.create(ConstructorWithDoubleNestedClassArguments).inner
+        )
 
     def test_constructed_sut_inner_has_correct_type(self):
-        self.assertIsInstance(Autodata.create(ConstructorWithDoubleNestedClassArguments).inner, ConstructorWithNestedClassArguments)
+        self.assertIsInstance(
+            Autodata.create(ConstructorWithDoubleNestedClassArguments).inner,
+            ConstructorWithNestedClassArguments,
+        )
 
     def test_constructed_sut_inner_inner_has_correct_type(self):
-        self.assertIsInstance(Autodata.create(ConstructorWithDoubleNestedClassArguments).inner.inner, ConstructorWithClassArguments)
+        self.assertIsInstance(
+            Autodata.create(ConstructorWithDoubleNestedClassArguments).inner.inner,
+            ConstructorWithClassArguments,
+        )
 
     def test_constructed_sut_inner_inner_inner_has_correct_type(self):
-        self.assertIsInstance(Autodata.create(ConstructorWithDoubleNestedClassArguments).inner.inner.inner, ConstructorWithPrimitiveArguments)
+        self.assertIsInstance(
+            Autodata.create(
+                ConstructorWithDoubleNestedClassArguments
+            ).inner.inner.inner,
+            ConstructorWithPrimitiveArguments,
+        )
 
 
 @dataclass
 class DataClass:
     id: int
     name: str
     age: int
@@ -171,21 +197,27 @@
     def test_can_construct_sut(self):
         self.assertIsNotNone(Autodata.create(ConstructorWithDataClassArguments))
 
     def test_constructed_sut_id_not_none(self):
         self.assertIsNotNone(Autodata.create(ConstructorWithDataClassArguments).data.id)
 
     def test_constructed_sut_age_not_none(self):
-        self.assertIsNotNone(Autodata.create(ConstructorWithDataClassArguments).data.age)
+        self.assertIsNotNone(
+            Autodata.create(ConstructorWithDataClassArguments).data.age
+        )
 
     def test_constructed_sut_name_not_none(self):
-        self.assertIsNotNone(Autodata.create(ConstructorWithDataClassArguments).data.name)
+        self.assertIsNotNone(
+            Autodata.create(ConstructorWithDataClassArguments).data.name
+        )
 
     def test_constructed_sut_email_not_none(self):
-        self.assertIsNotNone(Autodata.create(ConstructorWithDataClassArguments).data.email)
+        self.assertIsNotNone(
+            Autodata.create(ConstructorWithDataClassArguments).data.email
+        )
 
 
 class ConstructorWithListArguments:
     def __init__(self, texts: List[str], numbers: List[int]):
         self.numbers = numbers
         self.texts = texts
```

### Comparing `autofaker-1.0.14/tests/test_create_many_anonymous_builtins.py` & `autofaker-1.0.15/tests/test_create_many_anonymous_builtins.py`

 * *Files identical despite different names*

### Comparing `autofaker-1.0.14/tests/test_create_many_anonymous_dates.py` & `autofaker-1.0.15/tests/test_create_many_anonymous_dates.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,15 +26,17 @@
             return
         size = random.randint(1, 10)
         self.assertEqual(len(Autodata.create_many(self.getType(), size)), size)
 
     def test_create_many_returns_list_with_non_defaults(self):
         if self.getType() is None:
             return
-        self.assertNotEqual(Autodata.create_many(self.getType()), [self.getType()(1970, 1, 1)])
+        self.assertNotEqual(
+            Autodata.create_many(self.getType()), [self.getType()(1970, 1, 1)]
+        )
 
 
 class AnonymousDatetimeListTestCase(CreateManyTestCase):
     def getType(self):
         return datetime
```

### Comparing `autofaker-1.0.14/tests/test_create_many_anonymous_nested_classes.py` & `autofaker-1.0.15/tests/test_create_many_anonymous_nested_classes.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import unittest
 
 from autofaker import Autodata
 
 
 class SimpleClass:
     id = -1
-    text = 'test'
+    text = "test"
 
 
 class NestedClass:
     id = -1
-    text = 'test'
+    text = "test"
     inner = SimpleClass()
 
 
 class DoubleNestedClass:
     id = -1
-    text = 'test'
+    text = "test"
     inner = NestedClass()
 
 
 class AnonymousNestedClassTestCase(unittest.TestCase):
-
     def test_create_many_nested_class_returns_not_none(self):
         self.assertIsNotNone(Autodata.create_many(NestedClass))
 
     def test_create_many_nested_class_returns_list(self):
         self.assertIsInstance(Autodata.create_many(NestedClass), list)
 
     def test_create_many_nested_class_returns_list_with_not_none(self):
@@ -38,15 +37,14 @@
         for item in result:
             self.assertNotEqual(item.id, NestedClass().id)
             self.assertNotEqual(item.inner.id, SimpleClass().id)
             self.assertNotEqual(item.inner.text, SimpleClass().text)
 
 
 class AnonymousDoubleNestedClassTestCase(unittest.TestCase):
-
     def test_create_many_nested_class_returns_not_none(self):
         self.assertIsNotNone(Autodata.create_many(DoubleNestedClass))
 
     def test_create_many_nested_class_returns_instance(self):
         self.assertIsInstance(Autodata.create_many(DoubleNestedClass), list)
 
     def test_create_many_nested_class_returns_instance_with_nested_not_none(self):
@@ -57,13 +55,15 @@
 
     def test_create_many_nested_class_returns_instance_with_new_nested_instance(self):
         result = Autodata.create_many(DoubleNestedClass)
         for item in result:
             self.assertNotEqual(item.id, DoubleNestedClass().id)
             self.assertNotEqual(item.inner, NestedClass())
 
-    def test_create_many_nested_class_returns_instance_with_new_double_nested_instance(self):
+    def test_create_many_nested_class_returns_instance_with_new_double_nested_instance(
+        self,
+    ):
         result = Autodata.create_many(DoubleNestedClass)
         for item in result:
             self.assertNotEqual(item.id, DoubleNestedClass().id)
             self.assertNotEqual(item.inner.inner.id, SimpleClass().id)
             self.assertNotEqual(item.inner.inner.text, SimpleClass().text)
```

### Comparing `autofaker-1.0.14/tests/test_create_many_anonymous_nested_classes_with_lists.py` & `autofaker-1.0.15/tests/test_create_many_anonymous_nested_classes_with_lists.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import unittest
 
 from autofaker import Autodata
 
 
 class SimpleClass:
     id = -1
-    text = 'test'
+    text = "test"
 
 
 class NestedWithCollectionClass:
     id = -1
-    text = 'test'
+    text = "test"
     inner = [SimpleClass(), SimpleClass()]
 
 
 class NestedWithNestedCollectionClass:
     id = -1
-    text = 'test'
+    text = "test"
     inner = [NestedWithCollectionClass(), NestedWithCollectionClass()]
 
 
 class AnonymousNestedClassWithCollectionTestCase(unittest.TestCase):
-
     def test_create_many_nested_class_returns_not_none(self):
         self.assertIsNotNone(Autodata.create_many(NestedWithCollectionClass))
 
     def test_create_many_nested_class_returns_list(self):
         self.assertIsInstance(Autodata.create_many(NestedWithCollectionClass), list)
 
     def test_create_many_nested_class_returns_instances_with_nested_not_none(self):
@@ -45,15 +44,14 @@
             for cls in item.inner:
                 self.assertIsNotNone(cls)
                 self.assertNotEqual(cls.id, SimpleClass().id)
                 self.assertNotEqual(cls.text, SimpleClass().text)
 
 
 class AnonymousNestedClassWithNestedCollectionTestCase(unittest.TestCase):
-
     def test_create_many_nested_class_returns_not_none(self):
         self.assertIsNotNone(Autodata.create_many(NestedWithCollectionClass))
 
     def test_create_many_nested_class_returns_list(self):
         self.assertIsInstance(Autodata.create_many(NestedWithCollectionClass), list)
 
     def test_create_many_nested_class_returns_instances_with_inner_not_none(self):
@@ -62,15 +60,17 @@
             self.assertIsNotNone(item.inner)
 
     def test_create_many_nested_class_returns_instances_with_inner_not_empty(self):
         result = Autodata.create_many(NestedWithNestedCollectionClass)
         for item in result:
             self.assertNotEqual(0, len(item.inner))
 
-    def test_create_many_nested_class_returns_instances_with_nested_inner_not_empty(self):
+    def test_create_many_nested_class_returns_instances_with_nested_inner_not_empty(
+        self,
+    ):
         result = Autodata.create_many(NestedWithNestedCollectionClass)
         for item in result:
             for cls in item.inner:
                 self.assertNotEqual(0, len(cls.inner))
 
     def test_create_many_nested_class_returns_instances_with_new_nested_instances(self):
         result = Autodata.create_many(NestedWithNestedCollectionClass)
```

### Comparing `autofaker-1.0.14/tests/test_create_many_anonymous_simple_classes.py` & `autofaker-1.0.15/tests/test_create_many_anonymous_simple_classes.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import unittest
 
 from autofaker import Autodata
 
 
 class SimpleClass:
     id = -1
-    text = 'test'
+    text = "test"
 
 
 class AnonymousSimpleClassTestCase(unittest.TestCase):
     def test_create_many_returns_not_none(self):
         self.assertIsNotNone(Autodata.create_many(SimpleClass))
 
     def test_create_many_returns_list(self):
```

### Comparing `autofaker-1.0.14/tests/test_decorator_exceptions.py` & `autofaker-1.0.15/tests/test_decorator_exceptions.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import unittest
 from dataclasses import dataclass
 
 import pandas
 
-from autofaker import autodata, fakedata, autopandas, fakepandas
+from autofaker import autodata, autopandas, fakedata, fakepandas
 
 
 @dataclass
 class DataClass:
     id: int
     name: str
     text: str
@@ -25,90 +25,97 @@
 
 @autopandas(DataClass)
 def autopandas_test_method(df: pandas.DataFrame):
     pass
 
 
 class AnonymousPrimitivesViaDecoratorThrowsExceptionsTests(unittest.TestCase):
-
     def test_autodata_throws_error_when_decorating_non_testmethod(self):
         with self.assertRaises(NotImplementedError):
+
             class X:
                 @autodata(str, str, str)
                 def not_test_method(self):
                     pass
 
             X().not_test_method()
 
     def test_autodata_throws_error_when_used_without_arguments(self):
         with self.assertRaises(NotImplementedError):
+
             class X:
                 @autodata()
                 def not_test_method(self):
                     pass
 
             X().not_test_method()
 
     def test_autodata_throws_error_when_used_without_arguments_annotation(self):
         with self.assertRaises(ValueError):
+
             class X(unittest.TestCase):
                 @autodata()
                 def not_test_method(self, text, number, decimal):
                     pass
 
             X().not_test_method()
 
     def test_fakedata_throws_error_when_decorating_non_testmethod(self):
         with self.assertRaises(NotImplementedError):
+
             class X:
                 @fakedata(str, str, str)
                 def not_test_method(self):
                     pass
 
             X().not_test_method()
 
     def test_fakedata_throws_error_when_used_without_arguments(self):
         with self.assertRaises(NotImplementedError):
+
             class X:
                 @fakedata()
                 def not_test_method(self):
                     pass
 
             X().not_test_method()
 
     def test_fakedata_throws_error_when_used_without_arguments_annotation(self):
         with self.assertRaises(ValueError):
+
             class X(unittest.TestCase):
                 @fakedata()
                 def not_test_method(self, text, number, decimal):
                     pass
 
             X().not_test_method()
 
     def test_autopandas_throws_error_when_decorating_non_testmethod(self):
         class SimpleClass:
             id = -1
-            name = 'name'
-            text = 'test'
+            name = "name"
+            text = "test"
 
         with self.assertRaises(NotImplementedError):
+
             class X:
                 @autopandas(SimpleClass)
                 def not_test_method(self, df):
                     pass
 
             X().not_test_method()
 
     def test_fakepandas_throws_error_when_decorating_non_testmethod(self):
         class SimpleClass:
             id = -1
-            name = 'name'
-            text = 'test'
+            name = "name"
+            text = "test"
 
         with self.assertRaises(NotImplementedError):
+
             class X:
                 @fakepandas(SimpleClass)
                 def not_test_method(self, df):
                     pass
 
             X().not_test_method()
```

### Comparing `autofaker-1.0.14/tests/unittests/test_decorator_anonymous_builtins.py` & `autofaker-1.0.15/tests/unittests/test_decorator_anonymous_builtins.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import unittest
-from datetime import datetime, date
+from datetime import date, datetime
 
 from autofaker import autodata, fakedata
 
 
 class AnonymousPrimitivesViaDecoratorTests(unittest.TestCase):
-
     @autodata(str)
     def test_create_str_using_decorator(self, text):
         self.assertIsNotNone(text)
 
     @autodata(int)
     def test_create_int_using_decorator(self, number):
         self.assertIsNotNone(number)
@@ -48,15 +47,14 @@
 
     @autodata(date)
     def test_create_date_using_decorator(self, d):
         self.assertIsNotNone(d)
 
 
 class AnonymousPrimitivesViaDecoratorWithFakesTests(unittest.TestCase):
-
     @autodata(str, use_fake_data=True)
     def test_create_str_using_decorator(self, text):
         self.assertIsNotNone(text)
 
     @autodata(int, use_fake_data=True)
     def test_create_int_using_decorator(self, number):
         self.assertIsNotNone(number)
@@ -95,119 +93,139 @@
 
     @autodata(date, use_fake_data=True)
     def test_create_date_using_decorator(self, d):
         self.assertIsNotNone(d)
 
 
 class MultipleAnonymousPrimitivesViaDecoratorTests(unittest.TestCase):
-
     @autodata(str, int, float, complex, range, bytes, bytearray, memoryview)
-    def test_create_primitives_using_decorator(self, text, number, decimal, complex_type, range_type, buffer, buffer2, memview):
+    def test_create_primitives_using_decorator(
+        self, text, number, decimal, complex_type, range_type, buffer, buffer2, memview
+    ):
         self.assertIsNotNone(text)
         self.assertNotEqual(number, 0)
         self.assertNotEqual(decimal, float())
         self.assertNotEqual(complex_type, complex())
         self.assertNotEqual(range_type, range(0))
         self.assertNotEqual(buffer, bytes())
         self.assertNotEqual(buffer2, bytearray())
         self.assertNotEqual(memview, memoryview(bytes()))
 
-    @autodata(str, int, float, complex, range, bytes, bytearray, memoryview, use_fake_data=True)
-    def test_create_primitives_using_decorator_with_fakes(self, text, number, decimal, complex_type, range_type, buffer, buffer2, memview):
+    @autodata(
+        str,
+        int,
+        float,
+        complex,
+        range,
+        bytes,
+        bytearray,
+        memoryview,
+        use_fake_data=True,
+    )
+    def test_create_primitives_using_decorator_with_fakes(
+        self, text, number, decimal, complex_type, range_type, buffer, buffer2, memview
+    ):
         self.assertIsNotNone(text)
         self.assertNotEqual(number, 0)
         self.assertNotEqual(decimal, float())
         self.assertNotEqual(complex_type, complex())
         self.assertNotEqual(range_type, range(0))
         self.assertNotEqual(buffer, bytes())
         self.assertNotEqual(buffer2, bytearray())
         self.assertNotEqual(memview, memoryview(bytes()))
 
 
 class MultipleArgumentsViaDecoratorTests(unittest.TestCase):
-
     @fakedata()
-    def test_create_anonymous_arguments_using_decorator(self,
-                                                        text: str,
-                                                        number: int,
-                                                        decimal: float,
-                                                        complex_type: complex,
-                                                        range_type: range,
-                                                        buffer: bytes,
-                                                        buffer2: bytearray,
-                                                        memview: memoryview):
+    def test_create_anonymous_arguments_using_decorator(
+        self,
+        text: str,
+        number: int,
+        decimal: float,
+        complex_type: complex,
+        range_type: range,
+        buffer: bytes,
+        buffer2: bytearray,
+        memview: memoryview,
+    ):
         print(text)
         print(number)
         print(decimal)
         print(complex_type)
         self.assertIsNotNone(text)
         self.assertNotEqual(number, 0)
         self.assertNotEqual(decimal, float())
         self.assertNotEqual(complex_type, complex())
         self.assertNotEqual(range_type, range(0))
         self.assertNotEqual(buffer, bytes())
         self.assertNotEqual(buffer2, bytearray())
         self.assertNotEqual(memview, memoryview(bytes()))
 
     @fakedata()
-    def test_create_fake_arguments_using_decorator(self,
-                                                   text: str,
-                                                   number: int,
-                                                   decimal: float,
-                                                   complex_type: complex,
-                                                   range_type: range,
-                                                   buffer: bytes,
-                                                   buffer2: bytearray,
-                                                   memview: memoryview):
+    def test_create_fake_arguments_using_decorator(
+        self,
+        text: str,
+        number: int,
+        decimal: float,
+        complex_type: complex,
+        range_type: range,
+        buffer: bytes,
+        buffer2: bytearray,
+        memview: memoryview,
+    ):
         print(text)
         print(number)
         print(decimal)
         print(complex_type)
         self.assertIsNotNone(text)
         self.assertNotEqual(number, 0)
         self.assertNotEqual(decimal, float())
         self.assertNotEqual(complex_type, complex())
         self.assertNotEqual(range_type, range(0))
         self.assertNotEqual(buffer, bytes())
         self.assertNotEqual(buffer2, bytearray())
         self.assertNotEqual(memview, memoryview(bytes()))
 
     @autodata()
-    def test_create_arguments_using_decorator(self,
-                                              text: str,
-                                              number: int,
-                                              decimal: float,
-                                              complex_type: complex,
-                                              range_type: range,
-                                              buffer: bytes,
-                                              buffer2: bytearray,
-                                              memview: memoryview):
+    def test_create_arguments_using_decorator(
+        self,
+        text: str,
+        number: int,
+        decimal: float,
+        complex_type: complex,
+        range_type: range,
+        buffer: bytes,
+        buffer2: bytearray,
+        memview: memoryview,
+    ):
         print(text)
         print(number)
         print(decimal)
         print(complex_type)
         self.assertIsNotNone(text)
         self.assertNotEqual(number, 0)
         self.assertNotEqual(decimal, float())
         self.assertNotEqual(complex_type, complex())
         self.assertNotEqual(range_type, range(0))
         self.assertNotEqual(buffer, bytes())
         self.assertNotEqual(buffer2, bytearray())
         self.assertNotEqual(memview, memoryview(bytes()))
 
     @autodata(use_fake_data=True)
-    def test_create_arguments_using_decorator_with_fakes(self,
-                                                         text: str,
-                                                         number: int,
-                                                         decimal: float,
-                                                         complex_type: complex,
-                                                         range_type: range,
-                                                         buffer: bytes,
-                                                         buffer2: bytearray,
-                                                         memview: memoryview):
+    def test_create_arguments_using_decorator_with_fakes(
+        self,
+        text: str,
+        number: int,
+        decimal: float,
+        complex_type: complex,
+        range_type: range,
+        buffer: bytes,
+        buffer2: bytearray,
+        memview: memoryview,
+    ):
         print(text)
         print(number)
         print(decimal)
         print(complex_type)
         self.assertIsNotNone(text)
         self.assertNotEqual(number, 0)
         self.assertNotEqual(decimal, float())
```

### Comparing `autofaker-1.0.14/tests/unittests/test_decorator_anonymous_data_classes.py` & `autofaker-1.0.15/tests/unittests/test_decorator_anonymous_data_classes.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 class DataClass:
     id: int
     name: str
     text: str
 
 
 class AnonymousDataClassViaDecoratorTestCase(unittest.TestCase):
-
     @autodata(DataClass)
     def test_create_data_class_using_decorator_returns_not_none(self, instance):
         self.assertIsNotNone(instance)
 
     @autodata(DataClass)
     def test_create_data_class_using_decorator_returns_dataclass(self, instance):
         self.assertTrue(dataclasses.is_dataclass(instance))
@@ -25,51 +24,60 @@
     @autodata(DataClass)
     def test_create_data_class_returns_instance_with_new_values(self, instance):
         self.assertNotEqual(instance.id, int())
         self.assertNotEqual(instance.name, str())
         self.assertNotEqual(instance.text, str())
 
     @autodata()
-    def test_create_data_class_argument_returns_instance_with_new_values(self, instance: DataClass):
+    def test_create_data_class_argument_returns_instance_with_new_values(
+        self, instance: DataClass
+    ):
         self.assertNotEqual(instance.id, int())
         self.assertNotEqual(instance.name, str())
         self.assertNotEqual(instance.text, str())
 
     @autodata()
-    def test_create_anonymous_data_class_returns_instance_with_new_values(self, instance: DataClass):
+    def test_create_anonymous_data_class_returns_instance_with_new_values(
+        self, instance: DataClass
+    ):
         self.assertNotEqual(instance.id, int())
         self.assertNotEqual(instance.name, str())
         self.assertNotEqual(instance.text, str())
 
     @fakedata()
-    def test_create_fake_data_class_returns_instance_with_new_values(self, instance: DataClass):
+    def test_create_fake_data_class_returns_instance_with_new_values(
+        self, instance: DataClass
+    ):
         self.assertNotEqual(instance.id, int())
         self.assertNotEqual(instance.name, str())
         self.assertNotEqual(instance.text, str())
 
 
 class AnonymousDataClassViaDecoratorWithFakesTestCase(unittest.TestCase):
-
     @autodata(DataClass, use_fake_data=True)
     def test_create_data_class_using_decorator_returns_not_none(self, instance):
         self.assertIsNotNone(instance)
 
     @autodata(DataClass, use_fake_data=True)
     def test_create_data_class_using_decorator_returns_dataclass(self, instance):
         self.assertTrue(dataclasses.is_dataclass(instance))
 
     @autodata(DataClass, use_fake_data=True)
     def test_create_data_class_returns_instance_with_new_values(self, instance):
         self.assertNotEqual(instance.id, int())
         self.assertNotEqual(instance.text, str())
 
     @autodata(use_fake_data=True)
-    def test_create_data_class_argument_returns_instance_with_new_values(self, instance: DataClass):
+    def test_create_data_class_argument_returns_instance_with_new_values(
+        self, instance: DataClass
+    ):
         self.assertNotEqual(instance.id, int())
         self.assertNotEqual(instance.name, str())
         self.assertNotEqual(instance.text, str())
 
     @fakedata()
-    def test_create_fake_data_class_returns_instance_with_new_values(self, instance: DataClass):
+    def test_create_fake_data_class_returns_instance_with_new_values(
+        self, instance: DataClass
+    ):
         self.assertNotEqual(instance.id, int())
         self.assertNotEqual(instance.name, str())
         self.assertNotEqual(instance.text, str())
```

### Comparing `autofaker-1.0.14/tests/unittests/test_decorator_anonymous_data_classes_nested.py` & `autofaker-1.0.15/tests/unittests/test_decorator_anonymous_data_classes_nested.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,14 @@
     id: int
     name: str
     text: str
     inner: NestedClass
 
 
 class AnonymousNestedClassViaDecoratorTestCase(unittest.TestCase):
-
     @autodata(NestedClass)
     def test_create_nested_class_using_decorator_returns_not_none(self, instance):
         self.assertIsNotNone(instance)
 
     @autodata(NestedClass)
     def test_create_nested_class_using_decorator_returns_dataclass(self, instance):
         self.assertTrue(dataclasses.is_dataclass(instance))
@@ -41,50 +40,63 @@
     @autodata(NestedClass)
     def test_create_nested_class_returns_instance_with_new_values(self, instance):
         self.assertNotEqual(instance.id, 0)
         self.assertNotEqual(instance.inner.id, 0)
         self.assertNotEqual(instance.inner.text, str())
 
     @autodata()
-    def test_create_nested_class_argument_returns_instance_with_new_values(self, instance: NestedClass):
+    def test_create_nested_class_argument_returns_instance_with_new_values(
+        self, instance: NestedClass
+    ):
         self.assertNotEqual(instance.id, 0)
         self.assertNotEqual(instance.name, str())
         self.assertNotEqual(instance.text, str())
 
     @autodata()
-    def test_create_anonymous_nested_class_returns_instance_with_new_values(self, instance: NestedClass):
+    def test_create_anonymous_nested_class_returns_instance_with_new_values(
+        self, instance: NestedClass
+    ):
         self.assertNotEqual(instance.id, 0)
         self.assertNotEqual(instance.name, str())
         self.assertNotEqual(instance.text, str())
 
     @fakedata()
-    def test_create_fake_nested_class_returns_instance_with_new_values(self, instance: NestedClass):
+    def test_create_fake_nested_class_returns_instance_with_new_values(
+        self, instance: NestedClass
+    ):
         self.assertNotEqual(instance.id, 0)
         self.assertNotEqual(instance.name, str())
         self.assertNotEqual(instance.text, str())
 
 
 class AnonymousDoubleNestedClassViaDecoratorWithFakesTestCase(unittest.TestCase):
-
     @autodata(DoubleNestedClass, use_fake_data=True)
-    def test_create_double_nested_class_using_decorator_returns_not_none(self, instance):
+    def test_create_double_nested_class_using_decorator_returns_not_none(
+        self, instance
+    ):
         self.assertIsNotNone(instance)
 
     @autodata(DoubleNestedClass, use_fake_data=True)
     def test_create_nested_class_using_decorator_returns_dataclass(self, instance):
         self.assertTrue(dataclasses.is_dataclass(instance))
 
     @autodata(DoubleNestedClass, use_fake_data=True)
-    def test_create_double_nested_class_returns_instance_with_new_values(self, instance):
+    def test_create_double_nested_class_returns_instance_with_new_values(
+        self, instance
+    ):
         self.assertNotEqual(instance.id, 0)
         self.assertNotEqual(instance.inner.inner.id, 0)
         self.assertNotEqual(instance.inner.inner.text, str())
 
     @autodata(use_fake_data=True)
-    def test_create_double_nested_class_argument_using_decorator_returns_not_none(self, instance: DoubleNestedClass):
+    def test_create_double_nested_class_argument_using_decorator_returns_not_none(
+        self, instance: DoubleNestedClass
+    ):
         self.assertIsNotNone(instance)
 
     @fakedata()
-    def test_create_double_nested_class_argument_returns_instance_with_new_values(self, instance: DoubleNestedClass):
+    def test_create_double_nested_class_argument_returns_instance_with_new_values(
+        self, instance: DoubleNestedClass
+    ):
         self.assertNotEqual(instance.id, 0)
         self.assertNotEqual(instance.inner.inner.id, 0)
         self.assertNotEqual(instance.inner.inner.text, str())
```

### Comparing `autofaker-1.0.14/tests/unittests/test_decorator_anonymous_dataframe_pandas.py` & `autofaker-1.0.15/tests/unittests/test_decorator_anonymous_dataframe_pandas.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import unittest
 from dataclasses import dataclass
 
 import pandas
 
-from autofaker import autopandas, fakepandas, autodata
+from autofaker import autodata, autopandas, fakepandas
 
 
 class SimpleClassA:
     id = -1
-    name: 'test'
-    text = 'test'
+    name: "test"
+    text = "test"
 
 
 class SimpleClassB:
     def __init__(self, id: int, name: str, text: str):
         self.text = text
         self.name = name
         self.id = id
@@ -22,73 +22,88 @@
 class SimpleClassC:
     def __init__(self, a: SimpleClassA, b: SimpleClassB):
         self.b = b
         self.a = a
 
 
 class AnonymousPandasDataFrameViaDecoratorTests(unittest.TestCase):
-
     @autopandas(SimpleClassA)
-    def test_create_anonymous_pandas_dataframe_returns_not_none(self, df: pandas.DataFrame):
+    def test_create_anonymous_pandas_dataframe_returns_not_none(
+        self, df: pandas.DataFrame
+    ):
         self.assertIsNotNone(df)
 
     @autopandas(SimpleClassA, 10)
-    def test_create_anonymous_pandas_dataframe_with_rowcount_returns_not_empty(self, df: pandas.DataFrame):
+    def test_create_anonymous_pandas_dataframe_with_rowcount_returns_not_empty(
+        self, df: pandas.DataFrame
+    ):
         self.assertNotEqual(len(df.index), 0)
 
     @fakepandas(SimpleClassA)
     def test_create_fake_pandas_dataframe_returns_not_none(self, df: pandas.DataFrame):
         self.assertIsNotNone(df)
 
     @fakepandas(SimpleClassA, 10)
-    def test_create_fake_pandas_dataframe_with_rowcount_returns_not_empty(self, df: pandas.DataFrame):
+    def test_create_fake_pandas_dataframe_with_rowcount_returns_not_empty(
+        self, df: pandas.DataFrame
+    ):
         self.assertNotEqual(len(df.index), 0)
 
     @autopandas(SimpleClassA)
     def test_can_create_anonymous_pandas_dataframes(self, cls):
         self.assertIsNotNone(cls)
 
     @autopandas(SimpleClassB)
-    def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_arguments(self, cls):
+    def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_arguments(
+        self, cls
+    ):
         self.assertIsNotNone(cls)
 
     @autopandas(SimpleClassC)
-    def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_class_arguments(self, cls):
+    def test_can_create_anonymous_pandas_dataframes_from_class_with_constructor_class_arguments(
+        self, cls
+    ):
         self.assertIsNotNone(cls)
 
 
 @dataclass
 class DataClass:
     id: int
     name: str
     text: str
 
 
 class AnonymousPandasDataFrameViaDecoratorFromDataClassTests(unittest.TestCase):
-
     @autopandas(DataClass)
-    def test_create_anonymous_pandas_dataframe_returns_not_none(self, df: pandas.DataFrame):
+    def test_create_anonymous_pandas_dataframe_returns_not_none(
+        self, df: pandas.DataFrame
+    ):
         self.assertIsNotNone(df)
 
     @autopandas(DataClass, 10)
-    def test_create_anonymous_pandas_dataframe_with_rowcount_returns_not_empty(self, df: pandas.DataFrame):
+    def test_create_anonymous_pandas_dataframe_with_rowcount_returns_not_empty(
+        self, df: pandas.DataFrame
+    ):
         self.assertNotEqual(len(df.index), 0)
 
     @fakepandas(DataClass, 10)
-    def test_create_fake_pandas_dataframe_with_rowcount_returns_not_empty(self, df: pandas.DataFrame):
+    def test_create_fake_pandas_dataframe_with_rowcount_returns_not_empty(
+        self, df: pandas.DataFrame
+    ):
         self.assertNotEqual(len(df.index), 0)
 
     @fakepandas(DataClass)
     def test_create_fake_pandas_dataframe_returns_not_none(self, df: pandas.DataFrame):
         self.assertIsNotNone(df)
 
 
 class AutodataDecoratorIgnoresPandas(unittest.TestCase):
-
     @autodata()
     def test_autodata_decorator_ignores_pandas_dataframe(self, df: pandas.DataFrame):
         self.assertIsNone(df)
 
     @autodata()
-    def test_autodata_decorator_ignores_only_pandas_dataframe(self, text: str, df: pandas.DataFrame):
+    def test_autodata_decorator_ignores_only_pandas_dataframe(
+        self, text: str, df: pandas.DataFrame
+    ):
         self.assertIsNotNone(text)
         self.assertIsNone(df)
```

### Comparing `autofaker-1.0.14/tests/unittests/test_decorator_anonymous_nested_classes.py` & `autofaker-1.0.15/tests/unittests/test_decorator_anonymous_nested_classes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,33 @@
 import unittest
 
 from autofaker import autodata, fakedata
 
 
 class SimpleClass:
     id = -1
-    name = 'name'
-    text = 'test'
+    name = "name"
+    text = "test"
 
 
 class NestedClass:
     id = -1
-    name = 'name'
-    text = 'test'
+    name = "name"
+    text = "test"
     inner = SimpleClass()
 
 
 class DoubleNestedClass:
     id = -1
-    name = 'name'
-    text = 'test'
+    name = "name"
+    text = "test"
     inner = NestedClass()
 
 
 class AnonymousNestedClassViaDecoratorTestCase(unittest.TestCase):
-
     @autodata(NestedClass)
     def test_create_nested_class_using_decorator_returns_not_none(self, instance):
         self.assertIsNotNone(instance)
 
     @autodata(NestedClass)
     def test_create_nested_class_using_decorator_returns_instance(self, instance):
         self.assertIsInstance(instance, NestedClass)
@@ -36,57 +35,74 @@
     @autodata(NestedClass)
     def test_create_nested_class_returns_instance_with_new_values(self, instance):
         self.assertNotEqual(instance.id, NestedClass().id)
         self.assertNotEqual(instance.inner.id, SimpleClass().id)
         self.assertNotEqual(instance.inner.text, SimpleClass().text)
 
     @autodata()
-    def test_create_nested_class_argument_returns_instance_with_new_values(self, instance: NestedClass):
+    def test_create_nested_class_argument_returns_instance_with_new_values(
+        self, instance: NestedClass
+    ):
         self.assertNotEqual(instance.id, NestedClass().id)
         self.assertNotEqual(instance.name, SimpleClass().name)
         self.assertNotEqual(instance.text, SimpleClass().text)
 
     @autodata()
-    def test_create_anonymous_nested_class_returns_instance_with_new_values(self, instance: NestedClass):
+    def test_create_anonymous_nested_class_returns_instance_with_new_values(
+        self, instance: NestedClass
+    ):
         self.assertNotEqual(instance.id, SimpleClass().id)
         self.assertNotEqual(instance.name, SimpleClass().name)
         self.assertNotEqual(instance.text, SimpleClass().text)
 
     @fakedata()
-    def test_create_fake_nested_class_returns_instance_with_new_values(self, instance: NestedClass):
+    def test_create_fake_nested_class_returns_instance_with_new_values(
+        self, instance: NestedClass
+    ):
         print(instance)
         self.assertNotEqual(instance.id, NestedClass().id)
         self.assertNotEqual(instance.name, SimpleClass().name)
         self.assertNotEqual(instance.text, SimpleClass().text)
 
 
 class AnonymousDoubleNestedClassViaDecoratorWithFakesTestCase(unittest.TestCase):
-
     @autodata(DoubleNestedClass, use_fake_data=True)
-    def test_create_double_nested_class_using_decorator_returns_not_none(self, instance):
+    def test_create_double_nested_class_using_decorator_returns_not_none(
+        self, instance
+    ):
         self.assertIsNotNone(instance)
 
     @autodata(DoubleNestedClass, use_fake_data=True)
-    def test_create_double_nested_class_using_decorator_returns_instance(self, instance):
+    def test_create_double_nested_class_using_decorator_returns_instance(
+        self, instance
+    ):
         self.assertIsInstance(instance, DoubleNestedClass)
 
     @autodata(DoubleNestedClass, use_fake_data=True)
-    def test_create_double_nested_class_returns_instance_with_new_values(self, instance):
+    def test_create_double_nested_class_returns_instance_with_new_values(
+        self, instance
+    ):
         self.assertNotEqual(instance.id, DoubleNestedClass().id)
         self.assertNotEqual(instance.inner, DoubleNestedClass().inner)
         self.assertNotEqual(instance.inner.inner.id, SimpleClass().id)
         self.assertNotEqual(instance.inner.inner.text, SimpleClass().text)
 
     @autodata(use_fake_data=True)
-    def test_create_double_nested_class_argument_using_decorator_returns_not_none(self, instance: DoubleNestedClass):
+    def test_create_double_nested_class_argument_using_decorator_returns_not_none(
+        self, instance: DoubleNestedClass
+    ):
         self.assertIsNotNone(instance)
 
     @autodata(use_fake_data=True)
-    def test_create_double_nested_class_argument_using_decorator_returns_instance(self, instance: DoubleNestedClass):
+    def test_create_double_nested_class_argument_using_decorator_returns_instance(
+        self, instance: DoubleNestedClass
+    ):
         self.assertIsInstance(instance, DoubleNestedClass)
 
     @fakedata()
-    def test_create_double_nested_class_argument_returns_instance_with_new_values(self, instance: DoubleNestedClass):
+    def test_create_double_nested_class_argument_returns_instance_with_new_values(
+        self, instance: DoubleNestedClass
+    ):
         self.assertNotEqual(instance.id, DoubleNestedClass().id)
         self.assertNotEqual(instance.inner, DoubleNestedClass().inner)
         self.assertNotEqual(instance.inner.inner.id, SimpleClass().id)
         self.assertNotEqual(instance.inner.inner.text, SimpleClass().text)
```

### Comparing `autofaker-1.0.14/tests/unittests/test_decorator_anonymous_simple_classes.py` & `autofaker-1.0.15/tests/unittests/test_decorator_anonymous_simple_classes.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import unittest
 
 from autofaker import autodata, fakedata
 
 
 class SimpleClass:
     id = -1
-    name = 'name'
-    text = 'test'
+    name = "name"
+    text = "test"
 
 
 class AnonymousSimpleClassViaDecoratorTestCase(unittest.TestCase):
-
     @autodata(SimpleClass)
     def test_create_simple_class_using_decorator_returns_not_none(self, instance):
         self.assertIsNotNone(instance)
 
     @autodata(SimpleClass)
     def test_create_simple_class_using_decorator_returns_instance(self, instance):
         self.assertIsInstance(instance, SimpleClass)
@@ -22,51 +21,60 @@
     @autodata(SimpleClass)
     def test_create_simple_class_returns_instance_with_new_values(self, instance):
         self.assertNotEqual(instance.id, SimpleClass().id)
         self.assertNotEqual(instance.name, SimpleClass().name)
         self.assertNotEqual(instance.text, SimpleClass().text)
 
     @autodata()
-    def test_create_simple_class_argument_returns_instance_with_new_values(self, instance: SimpleClass):
+    def test_create_simple_class_argument_returns_instance_with_new_values(
+        self, instance: SimpleClass
+    ):
         self.assertNotEqual(instance.id, SimpleClass().id)
         self.assertNotEqual(instance.name, SimpleClass().name)
         self.assertNotEqual(instance.text, SimpleClass().text)
 
     @autodata()
-    def test_create_anonymous_simple_class_returns_instance_with_new_values(self, instance: SimpleClass):
+    def test_create_anonymous_simple_class_returns_instance_with_new_values(
+        self, instance: SimpleClass
+    ):
         self.assertNotEqual(instance.id, SimpleClass().id)
         self.assertNotEqual(instance.name, SimpleClass().name)
         self.assertNotEqual(instance.text, SimpleClass().text)
 
     @fakedata()
-    def test_create_fake_simple_class_returns_instance_with_new_values(self, instance: SimpleClass):
+    def test_create_fake_simple_class_returns_instance_with_new_values(
+        self, instance: SimpleClass
+    ):
         self.assertNotEqual(instance.id, SimpleClass().id)
         self.assertNotEqual(instance.name, SimpleClass().name)
         self.assertNotEqual(instance.text, SimpleClass().text)
 
 
 class AnonymousSimpleClassViaDecoratorWithFakesTestCase(unittest.TestCase):
-
     @autodata(SimpleClass, use_fake_data=True)
     def test_create_simple_class_using_decorator_returns_not_none(self, instance):
         self.assertIsNotNone(instance)
 
     @autodata(SimpleClass, use_fake_data=True)
     def test_create_simple_class_using_decorator_returns_instance(self, instance):
         self.assertIsInstance(instance, SimpleClass)
 
     @autodata(SimpleClass, use_fake_data=True)
     def test_create_simple_class_returns_instance_with_new_values(self, instance):
         self.assertNotEqual(instance.id, SimpleClass().id)
         self.assertNotEqual(instance.text, SimpleClass().text)
 
     @autodata(use_fake_data=True)
-    def test_create_simple_class_argument_returns_instance_with_new_values(self, instance: SimpleClass):
+    def test_create_simple_class_argument_returns_instance_with_new_values(
+        self, instance: SimpleClass
+    ):
         self.assertNotEqual(instance.id, SimpleClass().id)
         self.assertNotEqual(instance.name, SimpleClass().name)
         self.assertNotEqual(instance.text, SimpleClass().text)
 
     @fakedata()
-    def test_create_fake_simple_class_returns_instance_with_new_values(self, instance: SimpleClass):
+    def test_create_fake_simple_class_returns_instance_with_new_values(
+        self, instance: SimpleClass
+    ):
         self.assertNotEqual(instance.id, SimpleClass().id)
         self.assertNotEqual(instance.name, SimpleClass().name)
         self.assertNotEqual(instance.text, SimpleClass().text)
```

