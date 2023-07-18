# Comparing `tmp/petab-0.2.2.tar.gz` & `tmp/petab-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petab-0.2.2.tar", last modified: Sat Jun 24 08:27:13 2023, max compression
+gzip compressed data, was "petab-0.2.3.tar", last modified: Tue Jul 18 06:43:43 2023, max compression
```

## Comparing `petab-0.2.2.tar` & `petab-0.2.3.tar`

### file list

```diff
@@ -1,77 +1,77 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.469408 petab-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-06-24 08:27:03.000000 petab-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-24 08:27:03.000000 petab-0.2.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-24 08:27:13.469408 petab-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-06-24 08:27:03.000000 petab-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.465408 petab-0.2.2/petab/
--rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-06-24 08:27:03.000000 petab-0.2.2/petab/C.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-24 08:27:03.000000 petab-0.2.2/petab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-06-24 08:27:03.000000 petab-0.2.2/petab/calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-06-24 08:27:03.000000 petab-0.2.2/petab/composite_problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-06-24 08:27:03.000000 petab-0.2.2/petab/conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-06-24 08:27:03.000000 petab-0.2.2/petab/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-06-24 08:27:03.000000 petab-0.2.2/petab/format_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    38465 2023-06-24 08:27:03.000000 petab-0.2.2/petab/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-06-24 08:27:03.000000 petab-0.2.2/petab/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-06-24 08:27:03.000000 petab-0.2.2/petab/measurements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.465408 petab-0.2.2/petab/models/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-24 08:27:03.000000 petab-0.2.2/petab/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-06-24 08:27:03.000000 petab-0.2.2/petab/models/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-06-24 08:27:03.000000 petab-0.2.2/petab/models/pysb_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-06-24 08:27:03.000000 petab-0.2.2/petab/models/sbml_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-06-24 08:27:03.000000 petab-0.2.2/petab/observables.py
--rw-r--r--   0 runner    (1001) docker     (123)    28086 2023-06-24 08:27:03.000000 petab-0.2.2/petab/parameter_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-06-24 08:27:03.000000 petab-0.2.2/petab/parameters.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4855 2023-06-24 08:27:03.000000 petab-0.2.2/petab/petablint.py
--rw-r--r--   0 runner    (1001) docker     (123)    33071 2023-06-24 08:27:03.000000 petab-0.2.2/petab/problem.py
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-06-24 08:27:03.000000 petab-0.2.2/petab/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-06-24 08:27:03.000000 petab-0.2.2/petab/sbml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.465408 petab-0.2.2/petab/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-06-24 08:27:03.000000 petab-0.2.2/petab/schemas/petab_schema.v1.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-06-24 08:27:03.000000 petab-0.2.2/petab/schemas/petab_schema.v2.0.0.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-24 08:27:03.000000 petab-0.2.2/petab/simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-06-24 08:27:03.000000 petab-0.2.2/petab/simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-24 08:27:03.000000 petab-0.2.2/petab/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.465408 petab-0.2.2/petab/visualize/
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/data_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/helper_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/lint.py
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/plot_data_and_simulation.py
--rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/plot_residuals.py
--rw-r--r--   0 runner    (1001) docker     (123)    27428 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/plotter.py
--rw-r--r--   0 runner    (1001) docker     (123)    36510 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.465408 petab-0.2.2/petab/visualize/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/templates/mystyle.css
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-24 08:27:03.000000 petab-0.2.2/petab/visualize/templates/report.html
--rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-06-24 08:27:03.000000 petab-0.2.2/petab/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.465408 petab-0.2.2/petab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-06-24 08:27:13.000000 petab-0.2.2/petab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-06-24 08:27:13.000000 petab-0.2.2/petab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-24 08:27:13.000000 petab-0.2.2/petab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-06-24 08:27:13.000000 petab-0.2.2/petab.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-24 08:27:13.000000 petab-0.2.2/petab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-24 08:27:13.000000 petab-0.2.2/petab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-24 08:27:03.000000 petab-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-24 08:27:13.469408 petab-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-06-24 08:27:03.000000 petab-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-24 08:27:13.469408 petab-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_calculate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_combine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_conditions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_deprecated.py
--rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_lint.py
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_measurements.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_model_pysb.py
--rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_observables.py
--rw-r--r--   0 runner    (1001) docker     (123)    21256 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_parameter_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24580 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_petab.py
--rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_sbml.py
--rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_simplify.py
--rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_simulate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_visualization.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_visualization_data_overview.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-06-24 08:27:03.000000 petab-0.2.2/tests/test_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:43:43.897692 petab-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-18 06:43:27.000000 petab-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-18 06:43:27.000000 petab-0.2.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-18 06:43:43.897692 petab-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-18 06:43:27.000000 petab-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:43:43.885692 petab-0.2.3/petab/
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-07-18 06:43:27.000000 petab-0.2.3/petab/C.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-18 06:43:27.000000 petab-0.2.3/petab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-07-18 06:43:27.000000 petab-0.2.3/petab/calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2696 2023-07-18 06:43:27.000000 petab-0.2.3/petab/composite_problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3133 2023-07-18 06:43:27.000000 petab-0.2.3/petab/conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15992 2023-07-18 06:43:27.000000 petab-0.2.3/petab/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-18 06:43:27.000000 petab-0.2.3/petab/format_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38465 2023-07-18 06:43:27.000000 petab-0.2.3/petab/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2984 2023-07-18 06:43:27.000000 petab-0.2.3/petab/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10555 2023-07-18 06:43:27.000000 petab-0.2.3/petab/measurements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:43:43.885692 petab-0.2.3/petab/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-18 06:43:27.000000 petab-0.2.3/petab/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4361 2023-07-18 06:43:27.000000 petab-0.2.3/petab/models/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7402 2023-07-18 06:43:27.000000 petab-0.2.3/petab/models/pysb_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-18 06:43:27.000000 petab-0.2.3/petab/models/sbml_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6407 2023-07-18 06:43:27.000000 petab-0.2.3/petab/observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28086 2023-07-18 06:43:27.000000 petab-0.2.3/petab/parameter_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19024 2023-07-18 06:43:27.000000 petab-0.2.3/petab/parameters.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4855 2023-07-18 06:43:27.000000 petab-0.2.3/petab/petablint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33071 2023-07-18 06:43:27.000000 petab-0.2.3/petab/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-07-18 06:43:27.000000 petab-0.2.3/petab/sampling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12067 2023-07-18 06:43:27.000000 petab-0.2.3/petab/sbml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:43:43.889692 petab-0.2.3/petab/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     2469 2023-07-18 06:43:27.000000 petab-0.2.3/petab/schemas/petab_schema.v1.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-07-18 06:43:27.000000 petab-0.2.3/petab/schemas/petab_schema.v2.0.0.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-07-18 06:43:27.000000 petab-0.2.3/petab/simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9195 2023-07-18 06:43:27.000000 petab-0.2.3/petab/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-18 06:43:27.000000 petab-0.2.3/petab/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:43:43.889692 petab-0.2.3/petab/visualize/
+-rw-r--r--   0 runner    (1001) docker     (123)      786 2023-07-18 06:43:27.000000 petab-0.2.3/petab/visualize/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-07-18 06:43:27.000000 petab-0.2.3/petab/visualize/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-07-18 06:43:27.000000 petab-0.2.3/petab/visualize/data_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2896 2023-07-18 06:43:27.000000 petab-0.2.3/petab/visualize/helper_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5039 2023-07-18 06:43:27.000000 petab-0.2.3/petab/visualize/lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-07-18 06:43:27.000000 petab-0.2.3/petab/visualize/plot_data_and_simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6056 2023-07-18 06:43:27.000000 petab-0.2.3/petab/visualize/plot_residuals.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27428 2023-07-18 06:43:27.000000 petab-0.2.3/petab/visualize/plotter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36510 2023-07-18 06:43:27.000000 petab-0.2.3/petab/visualize/plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:43:43.889692 petab-0.2.3/petab/visualize/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-07-18 06:43:27.000000 petab-0.2.3/petab/visualize/templates/mystyle.css
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 06:43:27.000000 petab-0.2.3/petab/visualize/templates/report.html
+-rw-r--r--   0 runner    (1001) docker     (123)     9488 2023-07-18 06:43:27.000000 petab-0.2.3/petab/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:43:43.885692 petab-0.2.3/petab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-18 06:43:43.000000 petab-0.2.3/petab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1596 2023-07-18 06:43:43.000000 petab-0.2.3/petab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:43:43.000000 petab-0.2.3/petab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-07-18 06:43:43.000000 petab-0.2.3/petab.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-07-18 06:43:43.000000 petab-0.2.3/petab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 06:43:43.000000 petab-0.2.3/petab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-18 06:43:27.000000 petab-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 06:43:43.897692 petab-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 2023-07-18 06:43:27.000000 petab-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:43:43.897692 petab-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    10571 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_calculate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2206 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_deprecated.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18921 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_lint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4146 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_measurements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_model_pysb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5480 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_observables.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21256 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_parameter_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8699 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24580 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_petab.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_sbml.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4754 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_simplify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8171 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_simulate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16075 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_visualization_data_overview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-18 06:43:27.000000 petab-0.2.3/tests/test_yaml.py
```

### Comparing `petab-0.2.2/LICENSE` & `petab-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/PKG-INFO` & `petab-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab
-Version: 0.2.2
+Version: 0.2.3
 Summary: Parameter estimation tabular data
 Home-page: https://github.com/PEtab-dev/libpetab-python
 Author: The PEtab developers
 Author-email: daniel.weindl@helmholtz-muenchen.de
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `petab-0.2.2/README.md` & `petab-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/C.py` & `petab-0.2.3/petab/C.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/__init__.py` & `petab-0.2.3/petab/__init__.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/calculate.py` & `petab-0.2.3/petab/calculate.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/composite_problem.py` & `petab-0.2.3/petab/composite_problem.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/conditions.py` & `petab-0.2.3/petab/conditions.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/core.py` & `petab-0.2.3/petab/core.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/lint.py` & `petab-0.2.3/petab/lint.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/mapping.py` & `petab-0.2.3/petab/mapping.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/measurements.py` & `petab-0.2.3/petab/measurements.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/models/model.py` & `petab-0.2.3/petab/models/model.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/models/pysb_model.py` & `petab-0.2.3/petab/models/pysb_model.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/models/sbml_model.py` & `petab-0.2.3/petab/models/sbml_model.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/observables.py` & `petab-0.2.3/petab/observables.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/parameter_mapping.py` & `petab-0.2.3/petab/parameter_mapping.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/parameters.py` & `petab-0.2.3/petab/parameters.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/petablint.py` & `petab-0.2.3/petab/petablint.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/problem.py` & `petab-0.2.3/petab/problem.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/sampling.py` & `petab-0.2.3/petab/sampling.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/sbml.py` & `petab-0.2.3/petab/sbml.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/schemas/petab_schema.v1.0.0.yaml` & `petab-0.2.3/petab/schemas/petab_schema.v1.0.0.yaml`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/schemas/petab_schema.v2.0.0.yaml` & `petab-0.2.3/petab/schemas/petab_schema.v2.0.0.yaml`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/simplify.py` & `petab-0.2.3/petab/simplify.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/simulate.py` & `petab-0.2.3/petab/simulate.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/visualize/cli.py` & `petab-0.2.3/petab/visualize/cli.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/visualize/data_overview.py` & `petab-0.2.3/petab/visualize/data_overview.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/visualize/helper_functions.py` & `petab-0.2.3/petab/visualize/helper_functions.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/visualize/lint.py` & `petab-0.2.3/petab/visualize/lint.py`

 * *Files 1% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     Adds default values to the given visualization table where no value was
     specified.
     """
     def set_default(column: str, value):
         if column not in vis_df:
             vis_df[column] = value
         elif value is not None:
-            vis_df[column].fillna(value)
+            vis_df[column].fillna(value, inplace=True)
 
     set_default(C.PLOT_NAME, "")
     set_default(C.PLOT_TYPE_SIMULATION, C.LINE_PLOT)
     set_default(C.PLOT_TYPE_DATA, C.MEAN_AND_SD)
     set_default(C.DATASET_ID, None)
     set_default(C.X_VALUES, C.TIME)
     set_default(C.X_OFFSET, 0)
```

### Comparing `petab-0.2.2/petab/visualize/plot_data_and_simulation.py` & `petab-0.2.3/petab/visualize/plot_data_and_simulation.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/visualize/plot_residuals.py` & `petab-0.2.3/petab/visualize/plot_residuals.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/visualize/plotter.py` & `petab-0.2.3/petab/visualize/plotter.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/visualize/plotting.py` & `petab-0.2.3/petab/visualize/plotting.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/visualize/templates/report.html` & `petab-0.2.3/petab/visualize/templates/report.html`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab/yaml.py` & `petab-0.2.3/petab/yaml.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/petab.egg-info/PKG-INFO` & `petab-0.2.3/petab.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: petab
-Version: 0.2.2
+Version: 0.2.3
 Summary: Parameter estimation tabular data
 Home-page: https://github.com/PEtab-dev/libpetab-python
 Author: The PEtab developers
 Author-email: daniel.weindl@helmholtz-muenchen.de
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
 Provides-Extra: tests
```

### Comparing `petab-0.2.2/petab.egg-info/SOURCES.txt` & `petab-0.2.3/petab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/setup.py` & `petab-0.2.3/setup.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_calculate.py` & `petab-0.2.3/tests/test_calculate.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_combine.py` & `petab-0.2.3/tests/test_combine.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_conditions.py` & `petab-0.2.3/tests/test_conditions.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_deprecated.py` & `petab-0.2.3/tests/test_deprecated.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_lint.py` & `petab-0.2.3/tests/test_lint.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_mapping.py` & `petab-0.2.3/tests/test_mapping.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_measurements.py` & `petab-0.2.3/tests/test_measurements.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_model_pysb.py` & `petab-0.2.3/tests/test_model_pysb.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_observables.py` & `petab-0.2.3/tests/test_observables.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_parameter_mapping.py` & `petab-0.2.3/tests/test_parameter_mapping.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_parameters.py` & `petab-0.2.3/tests/test_parameters.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_petab.py` & `petab-0.2.3/tests/test_petab.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_sbml.py` & `petab-0.2.3/tests/test_sbml.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_simplify.py` & `petab-0.2.3/tests/test_simplify.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_simulate.py` & `petab-0.2.3/tests/test_simulate.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_visualization.py` & `petab-0.2.3/tests/test_visualization.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_visualization_data_overview.py` & `petab-0.2.3/tests/test_visualization_data_overview.py`

 * *Files identical despite different names*

### Comparing `petab-0.2.2/tests/test_yaml.py` & `petab-0.2.3/tests/test_yaml.py`

 * *Files identical despite different names*

