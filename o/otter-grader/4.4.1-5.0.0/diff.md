# Comparing `tmp/otter-grader-4.4.1.tar.gz` & `tmp/otter-grader-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otter-grader-4.4.1.tar", last modified: Sat Jul  8 20:33:06 2023, max compression
+gzip compressed data, was "otter-grader-5.0.0.tar", last modified: Tue Jul 18 03:45:31 2023, max compression
```

## Comparing `otter-grader-4.4.1.tar` & `otter-grader-5.0.0.tar`

### file list

```diff
@@ -1,170 +1,198 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.289065 otter-grader-4.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-08 20:32:38.000000 otter-grader-4.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-08 20:32:38.000000 otter-grader-4.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-08 20:33:06.289065 otter-grader-4.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-08 20:32:38.000000 otter-grader-4.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.277065 otter-grader-4.4.1/otter/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.277065 otter-grader-4.4.1/otter/assign/
--rw-r--r--   0 runner    (1001) docker     (123)     7678 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11334 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/blocks.py
--rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/cell_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/feature_toggle.py
--rw-r--r--   0 runner    (1001) docker     (123)    16894 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/question_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.277065 otter-grader-4.4.1/otter/assign/r_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/r_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/r_adapter/cell_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/r_adapter/rmarkdown_converter.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/r_adapter/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/r_adapter/tests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13842 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/tests_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    11365 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/assign/v0/
--rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/assignment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/cell_generators.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/assign/v0/convert/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/convert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/convert/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/convert/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/questions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/assign/v0/r_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/r_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/r_adapter/tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/output.py
--rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/solutions.py
--rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/assign/v0/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/check/
--rw-r--r--   0 runner    (1001) docker     (123)     3558 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/check/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17923 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/check/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)    18909 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/check/notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/check/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/check/validate_export/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/check/validate_export/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/check/validate_export/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8313 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/execute/
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/execute/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/execute/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/execute/execute_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/execute/execute_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/execute/transforms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/export/
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/export/exporters/
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/base_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.281065 otter-grader-4.4.1/otter/export/exporters/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/export/exporters/templates/via_html/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_html/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_html/index.html.j2
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_html.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/export/exporters/templates/via_latex/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_latex/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_latex/index.tex.j2
--rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_latex.tpl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/export/exporters/templates/via_latex_xecjk/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_latex_xecjk/conf.json
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/templates/via_latex_xecjk.tpl
--rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2603 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/via_html.py
--rw-r--r--   0 runner    (1001) docker     (123)     3475 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/exporters/via_latex.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/export/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/generate/
--rw-r--r--   0 runner    (1001) docker     (123)     8451 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.269065 otter-grader-4.4.1/otter/generate/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/generate/templates/python/
--rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/python/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-08 20:33:04.000000 otter-grader-4.4.1/otter/generate/templates/python/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/python/run_autograder
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/python/run_otter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/python/setup.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/generate/templates/r/
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/r/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/r/requirements.r
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-08 20:33:04.000000 otter-grader-4.4.1/otter/generate/templates/r/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/r/run_autograder
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/r/run_otter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/templates/r/setup.sh
--rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/token.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/generate/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/grade/
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/grade/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/grade/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8032 2023-07-08 20:33:04.000000 otter-grader-4.4.1/otter/grade/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/grade/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/plugins/
--rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9124 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/abstract_plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/plugins/builtin/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/builtin/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/plugins/builtin/gmail_notifications/
--rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/builtin/gmail_notifications/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/plugins/builtin/gmail_notifications/bin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/builtin/gmail_notifications/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/builtin/grade_override.py
--rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/plugins/builtin/rate_limiting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/run/
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.285065 otter-grader-4.4.1/otter/run/run_autograder/
--rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/run_autograder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/run_autograder/autograder_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.289065 otter-grader-4.4.1/otter/run/run_autograder/runners/
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/run_autograder/runners/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6918 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/run_autograder/runners/abstract_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/run_autograder/runners/python_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/run_autograder/runners/r_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/run/run_autograder/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.289065 otter-grader-4.4.1/otter/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)    15243 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/test_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/test_files/abstract_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/test_files/exception_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/test_files/metadata_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/test_files/ok_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/test_files/ottr_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    13040 2023-07-08 20:32:38.000000 otter-grader-4.4.1/otter/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-08 20:33:04.000000 otter-grader-4.4.1/otter/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.289065 otter-grader-4.4.1/otter_grader.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-08 20:33:06.000000 otter-grader-4.4.1/otter_grader.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-08 20:33:06.000000 otter-grader-4.4.1/otter_grader.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-08 20:33:06.000000 otter-grader-4.4.1/otter_grader.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-08 20:33:06.000000 otter-grader-4.4.1/otter_grader.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-08 20:33:06.000000 otter-grader-4.4.1/otter_grader.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-08 20:33:06.000000 otter-grader-4.4.1/otter_grader.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-08 20:32:38.000000 otter-grader-4.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-08 20:33:06.289065 otter-grader-4.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-08 20:32:38.000000 otter-grader-4.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.289065 otter-grader-4.4.1/test/
--rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_assign.py
--rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_export.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-08 20:33:06.289065 otter-grader-4.4.1/test/test_generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3191 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_generate/test_autograder.py
--rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_generate/test_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_grade.py
--rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_notebook.py
--rw-r--r--   0 runner    (1001) docker     (123)    15187 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-08 20:32:38.000000 otter-grader-4.4.1/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.904800 otter-grader-5.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-07-18 03:45:03.000000 otter-grader-5.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-18 03:45:03.000000 otter-grader-5.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-18 03:45:31.904800 otter-grader-5.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1982 2023-07-18 03:45:03.000000 otter-grader-5.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.888800 otter-grader-5.0.0/otter/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2021 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/assign/
+-rw-r--r--   0 runner    (1001) docker     (123)     6249 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12049 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3439 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/blocks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5679 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/cell_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/feature_toggle.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17237 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4899 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/question_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/assign/r_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/r_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/r_adapter/cell_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4884 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/r_adapter/rmarkdown_converter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/r_adapter/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2997 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/r_adapter/tests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/assign/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/tests_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11113 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/assign/v0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8405 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/assignment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/cell_generators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/assign/v0/convert/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/convert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/convert/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/convert/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6760 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2465 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/questions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/assign/v0/r_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/r_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4687 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/r_adapter/tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5262 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5314 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3902 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4868 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/solutions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7883 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/tests.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11122 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/assign/v0/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/check/
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17962 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/check/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18283 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/check/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9321 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/check/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.892800 otter-grader-5.0.0/otter/check/validate_export/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/check/validate_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/check/validate_export/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8454 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/execute/
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3260 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/execute/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3671 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/execute/execute_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5085 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/execute/execute_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/execute/preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2246 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/execute/transforms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/export/
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/export/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/export/exporters/
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/base_exporter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/export/exporters/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/export/exporters/templates/via_html/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_html/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_html/index.html.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_html.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/export/exporters/templates/via_latex/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_latex/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_latex/index.tex.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      894 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_latex.tpl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/export/exporters/templates/via_latex_xecjk/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_latex_xecjk/conf.json
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/templates/via_latex_xecjk.tpl
+-rw-r--r--   0 runner    (1001) docker     (123)     3330 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/exporters/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/export/exporters/via_html.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/export/exporters/via_latex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/export/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)    10977 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.888800 otter-grader-5.0.0/otter/generate/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/generate/templates/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/common/run_autograder
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/common/run_otter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/generate/templates/python/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/python/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/python/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/python/run_autograder
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/python/run_otter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/python/setup.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/generate/templates/r/
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/r/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/r/requirements.r
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/r/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/r/run_autograder
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/r/run_otter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/templates/r/setup.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     3106 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/generate/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3095 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/generate/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/grade/
+-rw-r--r--   0 runner    (1001) docker     (123)      818 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/grade/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     4938 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/grade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7674 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/grade/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1595 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/grade/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)     7636 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8553 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/plugins/abstract_plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/plugins/builtin/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/plugins/builtin/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/plugins/builtin/gmail_notifications/
+-rw-r--r--   0 runner    (1001) docker     (123)     6061 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/plugins/builtin/gmail_notifications/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.896800 otter-grader-5.0.0/otter/plugins/builtin/gmail_notifications/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/plugins/builtin/gmail_notifications/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14192 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5949 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/plugins/builtin/grade_override.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4759 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/plugins/builtin/rate_limiting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/otter/run/
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/run/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/otter/run/run_autograder/
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/run/run_autograder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4733 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/run/run_autograder/autograder_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/otter/run/run_autograder/runners/
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/run/run_autograder/runners/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7639 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/run/run_autograder/runners/abstract_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/run/run_autograder/runners/python_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/run/run_autograder/runners/r_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/run/run_autograder/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/otter/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)    15291 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/test_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9442 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/test_files/abstract_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/test_files/exception_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4831 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/test_files/metadata_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6103 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/test_files/ok_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-07-18 03:45:04.000000 otter-grader-5.0.0/otter/test_files/ottr_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10510 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-07-18 03:45:30.000000 otter-grader-5.0.0/otter/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/otter_grader.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-07-18 03:45:31.000000 otter-grader-5.0.0/otter_grader.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5190 2023-07-18 03:45:31.000000 otter-grader-5.0.0/otter_grader.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 03:45:31.000000 otter-grader-5.0.0/otter_grader.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-07-18 03:45:31.000000 otter-grader-5.0.0/otter_grader.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-18 03:45:31.000000 otter-grader-5.0.0/otter_grader.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 03:45:31.000000 otter-grader-5.0.0/otter_grader.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-18 03:45:30.000000 otter-grader-5.0.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 03:45:31.904800 otter-grader-5.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-07-18 03:45:04.000000 otter-grader-5.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/test/test_assign/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_assign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7726 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_assign/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8054 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_assign.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/test/test_check/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_check/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_check/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_check/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7331 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_check/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5013 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20296 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/test/test_execute/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_execute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4364 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_execute/test_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_execute/test_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/test/test_export/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_export/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_export/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_export.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.900800 otter-grader-5.0.0/test/test_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:04.000000 otter-grader-5.0.0/test/test_generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_generate/test_autograder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2443 2023-07-18 03:45:04.000000 otter-grader-5.0.0/test/test_generate/test_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_generate/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.904800 otter-grader-5.0.0/test/test_grade/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_grade/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_grade/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9052 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_grade.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4049 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7540 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_notebook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:31.904800 otter-grader-5.0.0/test/test_run/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_run/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15221 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_run/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15187 2023-07-18 03:45:30.000000 otter-grader-5.0.0/test/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-18 03:45:04.000000 otter-grader-5.0.0/test/test_utils.py
```

### Comparing `otter-grader-4.4.1/LICENSE` & `otter-grader-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/PKG-INFO` & `otter-grader-5.0.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-grader
-Version: 4.4.1
+Version: 5.0.0
 Summary: Python and Jupyter Notebook autograder
 Home-page: https://github.com/ucbds-infra/otter-grader
 Author: Christopher Pyles
 Author-email: otter-grader@berkeley.edu
 License: BSD-3-Clause
 Description: # Otter-Grader
```

### Comparing `otter-grader-4.4.1/README.md` & `otter-grader-5.0.0/README.md`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/api.py` & `otter-grader-5.0.0/otter/api.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/__init__.py` & `otter-grader-5.0.0/otter/assign/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 """Assignment creation tool for Otter-Grader"""
 
-import json
 import os
 import pathlib
 import warnings
 
 from .assignment import Assignment
 from .output import write_output_directories
 from .utils import run_tests, write_otter_config_file, run_generate_autograder
@@ -13,39 +12,37 @@
 from ..plugins import PluginCollection
 from ..utils import chdir, get_relpath, knit_rmd_file, loggers
 
 
 LOGGER = loggers.get_logger(__name__)
 
 
-def main(master, result, *, no_pdfs=False, no_run_tests=False, username=None, password=None, 
-         debug=False, v0=False):
+def main(
+    master,
+    result,
+    *,
+    no_pdfs=False,
+    no_run_tests=False,
+    username=None,
+    password=None, 
+    debug=False,
+):
     """
     Runs Otter Assign on a master notebook.
 
     Args:
         master (``str``): path to master notebook
         result (``str``): path to result directory
         no_pdfs (``bool``): whether to ignore any configurations indicating PDF generation for this run
         no_run_tests (``bool``): prevents Otter tests from being automatically run on the solutions 
             notebook
         username (``str``): a username for Gradescope for generating a token
         password (``str``): a password for Gradescope for generating a token
         debug (``bool``): whether to run in debug mode (without ignoring errors during testing)
-        v0 (``bool``): whether to use Otter Assign Format v0 instead of v1
     """
-    if v0:
-        warnings.warn(
-            "The Otter Assign v0 format is now deprecated and will be removed in Otter v5.",
-            FutureWarning)
-
-        from .v0 import main as v0_main
-        return v0_main(master, result, no_pdfs=no_pdfs, no_run_tests=no_run_tests, username=username, 
-            password=password, debug=debug)
-
     LOGGER.debug(f"User-specified master path: {master}")
     LOGGER.debug(f"User-specified result path: {result}")
     master, result = pathlib.Path(os.path.abspath(master)), pathlib.Path(os.path.abspath(result))
 
     assignment = Assignment()
 
     result = get_relpath(master.parent, result)
@@ -57,40 +54,35 @@
     with chdir(master.parent):
         LOGGER.info("Generating views")
         write_output_directories(assignment)
 
         # update seed variables
         if assignment.seed.variable:
             LOGGER.debug("Processing seed dict")
-            if assignment.generate_enabled:
-                LOGGER.debug("Otter Generate configuration found while processing seed dict")
-                assignment.generate.seed = assignment.seed.autograder_value
-                assignment.generate.seed_variable = assignment.seed.variable
-                LOGGER.debug("Added seed information to assignment.generate")
+            assignment.generate.seed = assignment.seed.autograder_value
+            assignment.generate.seed_variable = assignment.seed.variable
+            LOGGER.debug("Added seed information to assignment.generate")
 
         # check that we have a seed if needed
         if assignment.seed_required:
             LOGGER.debug("Assignment seed is required")
-            if assignment.generate_enabled and \
-                    not isinstance(assignment.generate.seed, int):
+            if not isinstance(assignment.generate.seed, int):
                 raise RuntimeError("Seeding cell found but no or invalid seed provided")
 
         plugins, pc = assignment.plugins, None
         if plugins:
             LOGGER.debug("Processing plugins")
             pc = PluginCollection(plugins, "", {})
             pc.run("during_assign", assignment)
-            if assignment.generate_enabled:
-                LOGGER.debug("Adding plugin configurations to Otter Generate configuration")
-                assignment.generate.plugins = assignment.generate.plugins + plugins
-
-        # generate Gradescope autograder zipfile
-        if assignment.generate_enabled:
-            LOGGER.info("Generating autograder zipfile")
-            run_generate_autograder(assignment, username, password, plugin_collection=pc)
+
+            LOGGER.debug("Adding plugin configurations to Otter Generate configuration")
+            assignment.generate.plugins = assignment.generate.plugins + plugins
+
+        LOGGER.info("Generating autograder zipfile")
+        run_generate_autograder(assignment, username, password, plugin_collection=pc)
 
         # generate PDF of solutions
         if assignment.solutions_pdf and not no_pdfs:
             LOGGER.info("Generating solutions PDF")
             filtering = assignment.solutions_pdf == 'filtered'
 
             src = os.path.abspath(str(assignment.get_ag_path(master.name)))
@@ -155,30 +147,16 @@
                 warnings.warn(
                     "Otter Service and serialized environments are unsupported with R, "
                     "configurations ignored")
             else:
                 write_otter_config_file(assignment)
 
         # run tests on autograder notebook
-        if assignment.run_tests and not no_run_tests and assignment.is_python:
+        if assignment.run_tests and not no_run_tests:
             LOGGER.info("Running tests against the solutions notebook")
 
-            seed = assignment.generate.seed if assignment.generate_enabled else None
-            LOGGER.debug(f"Resolved seed for running tests: {seed}")
-
-            if assignment.generate_enabled:
-                LOGGER.debug("Retrieving updated plugins from otter_config.json for running tests")
-                test_pc = PluginCollection(
-                    assignment.generate.plugins, assignment.ag_notebook_path, {})
-
-            else:
-                LOGGER.debug("Using pre-configured plugins for running tests")
-                test_pc = pc
-
-            run_tests(
-                assignment.get_ag_path(master.name),
-                debug=debug,
-                seed=seed,
-                plugin_collection=test_pc,
-            )
+            run_tests(assignment, debug=debug)
 
             LOGGER.info("All autograder tests passed.")
+
+        else:
+            LOGGER.info("Skipping tests")
```

### Comparing `otter-grader-4.4.1/otter/assign/assignment.py` & `otter-grader-5.0.0/otter/assign/assignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 """Assignment configurations for Otter Assign"""
 
+import datetime as dt
 import fica
 import os
 import pathlib
+import warnings
 import yaml
 
 from typing import Any, Dict, List, Optional, Union
 
 from ..run.run_autograder.autograder_config import AutograderConfig
 from ..utils import Loggable
 
@@ -126,18 +128,17 @@
 
     seed: SeedValue = fica.Key(
         description="intercell seeding configurations",
         default=None,
         subkey_container=SeedValue,
     )
 
-    generate: Union[bool, AutograderConfig] = fica.Key(
+    generate: AutograderConfig = fica.Key(
         description="grading configurations to be passed to Otter Generate as an " \
-            "otter_config.json; if false, Otter Generate is disabled",
-        default=False,
+            "otter_config.json",
         subkey_container=AutograderConfig,
     )
 
     save_environment: bool = fica.Key(
         description="whether to save the student's environment in the log",
         default=False,
     )
@@ -205,14 +206,19 @@
     )
 
     python_version: Optional[Union[str, int, float]] = fica.Key(
         description="the version of Python to use in the grading image (must be 3.6+)",
         default=None,
     )
 
+    channel_priority_strict: bool = fica.Key(
+        description="whether to set conda's channel_priority config to strict in the setup.sh file",
+        default=True,
+    )
+
     lang: Optional[str] = None
     """the language of the assignment"""
 
     master: pathlib.Path = None
     """the path to the master notebook"""
 
     result: pathlib.Path = None
@@ -224,22 +230,33 @@
     # TODO: rename this
     _temp_test_dir: Optional[str] = None
     """the path to a directory of test files for Otter Generate"""
 
     notebook_basename: Optional[str] = None
     """the basename of the master notebook file"""
 
+    _ag_zip_name: Optional[str] = None
+    """
+    the file name for the autograder zip file; this value is generated the first time it is accessed
+    since it contians a timestamp
+    """
+
     def __init__(self, user_config: Dict[str, Any] = {}, **kwargs) -> None:
         self._logger.debug(f"Initializing with config: {user_config}")
         super().__init__(user_config, **kwargs)
 
         # convert a boolean to a config object for self.generate if indicated
         if self.generate is True:
             self.generate = AutograderConfig()
 
+        if self.variables:
+            warnings.warn(
+                "The variables key of the assignment config is deprecated and will be removed in " \
+                    "v6.0.0. Please use generate.seed_variables instead.", DeprecationWarning)
+
     def update(self, user_config: Dict[str, Any]):
         self._logger.debug(f"Updating config: {user_config}")
         ret = super().update(user_config)
         if self.generate is True:
             self.generate = AutograderConfig()
         return ret
 
@@ -260,55 +277,56 @@
     @property
     def is_rmd(self):
         """
         Whether the input file is an RMarkdown document
         """
         return self.master.suffix.lower() == ".rmd"
 
-    @property
-    def generate_enabled(self):
-        """
-        Whether Otter Generate is enabled for this assignment
-        """
-        return self.generate is not False
-
     def get_otter_config(self):
         """
         Get the contents of ``otter_config.json`` for this assignment.
 
         Returns:
             ``dict[str, object]``: the ``otter_config.json`` file as a ``dict``
         """
-        if not self.generate_enabled:
-            raise ValueError("Otter Generate is not configured for this assignment")
-
-        otter_config = self.generate
-
         if self.is_r:
-            otter_config.lang = "r"
+            self.generate.lang = "r"
 
         # TODO: move this config out of the assignment metadata and into the generate key
         if self.variables:
-            otter_config.serialized_variables = str(self.variables)
+            self.generate.serialized_variables = str(self.variables)
 
         if self.name:
-            otter_config.assignment_name = self.name
+            self.generate.assignment_name = self.name
 
-        return otter_config.get_user_config()
+        return self.generate.get_user_config()
 
     @property
     def notebook_basename(self):
         """the basename of the notebook"""
         return os.path.basename(str(self.master))
 
     @property
     def ag_notebook_path(self):
         """the path to the autograder notebook"""
         return self.get_ag_path(self.notebook_basename)
 
+    @property
+    def ag_zip_name(self):
+        """the file name of the autograder zip file"""
+        if self._ag_zip_name is None:
+            timestamp = dt.datetime.now().strftime("%Y_%m_%dT%H_%M_%S_%f")
+            self._ag_zip_name = f"{self.master.stem}-autograder_{timestamp}.zip"
+        return self._ag_zip_name
+
+    @property
+    def ag_zip_path(self):
+        """the path to the autograder zip file"""
+        return self.get_ag_path(self.ag_zip_name)
+
     def get_ag_path(self, path=""):
         """
         Get the path to the autograder output directory or a file in that directory.
 
         Args:
             path (``str | pathlib.Path``): a path to append to the autograder output directory path
```

### Comparing `otter-grader-4.4.1/otter/assign/blocks.py` & `otter-grader-5.0.0/otter/assign/blocks.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Assignment block parsing for Otter Assign"""
 
+import nbformat
 import re
 import yaml
 
 from enum import Enum
 
 from .utils import get_source, is_cell_type
 
@@ -15,27 +16,66 @@
 
     QUESTION = "question"
     PROMPT = "prompt"
     SOLUTION = "solution"
     TESTS = "tests"
 
 
+def extract_fenced_otter_cell(cell):
+    """
+    Converts a Markdown config cell to a raw config cell.
+
+    A Markdown cell with the contents
+
+    .. code-block::
+
+        ```otter
+        <cell contents>
+        ```
+
+    would become a raw cell with the contents
+
+    .. code-block::
+
+        <cell contents>
+
+    If the contents are not wrapped in a code block with the language set to ``otter``, the cell is
+    returned unchanged.
+
+    Args:
+        cell (``nbformat.NotebookNode``): the cell to extract the config from
+
+    Returns:
+        ``nbformat.NotebookNode``: the unfenced cell contents
+    """
+    if not is_cell_type(cell, "markdown"):
+        return cell
+
+    source = get_source(cell)
+    if source[0].strip() == "```otter" and \
+            all(not l.strip() == "```" for l in source[1:-1]) and source[-1].strip() == "```":
+        return nbformat.v4.new_raw_cell("\n".join(source[1:-1]))
+
+    return cell
+
+
 def is_block_boundary_cell(cell, block_type, end=False):
     """
     Determine whether ``cell`` is a boundary cell for a ``block_type`` block. If ``end`` is true,
     the block should be an end block; otherwise, it should be a begin block.
 
     Args:
         cell (``nbformat.NotebookNode``): the cell to check
         block_type (``BlockType``): the block type to check for
         end (``bool``, optional): whether to check for an end boundary instead of a begin
 
     Returns:
         ``bool``: whether the cell is a boundary cell of type ``block_type``
     """
+    cell = extract_fenced_otter_cell(cell)
     begin_or_end = 'end' if end else 'begin'
     regex = fr"#\s+{ begin_or_end }\s+{ block_type.value }\s*"
     source = get_source(cell)
     return is_cell_type(cell, "raw") and bool(re.match(regex, source[0], flags=re.IGNORECASE))
 
 
 def is_assignment_config_cell(cell):
@@ -54,14 +94,15 @@
 
     Args:
         cell (``nbformat.NotebookNode``): the cell to check
 
     Returns:
         ``bool``: whether the cell is an assignment config cell
     """
+    cell = extract_fenced_otter_cell(cell)
     regex = r"#\s+assignment\s+config\s*"
     source = get_source(cell)
     return is_cell_type(cell, "raw") and bool(re.match(regex, source[0], flags=re.IGNORECASE))
 
 
 def get_cell_config(cell):
     """
@@ -72,12 +113,12 @@
 
     Returns:
         ``dict[str, object]``: the parsed configurations
 
     Raises:
         ``TypeError``: if parsing the YAML does not return a dictionary
     """
-    source = get_source(cell)
+    source = get_source(extract_fenced_otter_cell(cell))
     config = yaml.full_load("\n".join(source))
     if not isinstance(config, dict) and config is not None:
         raise TypeError(f"Found a begin cell configuration that is not a dictionary: {cell}")
     return config
```

### Comparing `otter-grader-4.4.1/otter/assign/cell_factory.py` & `otter-grader-5.0.0/otter/assign/cell_factory.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/feature_toggle.py` & `otter-grader-5.0.0/otter/assign/feature_toggle.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/notebook_transformer.py` & `otter-grader-5.0.0/otter/assign/notebook_transformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .question_config import QuestionConfig
 from .r_adapter import rmarkdown_converter
 from .r_adapter.cell_factory import RCellFactory
 from .solutions import has_seed, SOLUTION_CELL_TAG, overwrite_seed_vars, strip_ignored_lines, \
     strip_solutions_and_output
 from .tests_manager import AssignmentTestsManager
 from .utils import add_tag, add_assignment_name_to_notebook, AssignNotebookFormatException, \
-    get_source, is_cell_type, is_ignore_cell, remove_cell_ids
+    get_source, is_cell_type, is_ignore_cell, lock, remove_cell_ids
 
 
 class NotebookTransformer:
     """
     A transformer for master notebooks that converts them to autograder- and
     student-formatted notebooks.
 
@@ -65,14 +65,15 @@
             return cell
 
         cell = copy.deepcopy(cell)
         source = get_source(cell)
         tag = "<!-- " + ("END" if end else "BEGIN") + " QUESTION -->"
         source = [tag, ""] + source
         cell['source'] = "\n".join(source)
+        lock(cell)
         return cell
 
     @staticmethod
     def add_point_value_info_to_cell(cell, points):
         """
         Add the point value information to the provided cell, returning a copy.
 
@@ -305,14 +306,18 @@
 
             if export_delim_cell is not None:
                 transformed_cells.append(export_delim_cell)
 
             if has_seed(cell):
                 self.assignment.seed_required = True
 
+            # if this cell is part of the question text, lock it
+            if len(curr_block) == 1:
+                lock(cell)
+
             # this is just a normal cell so add it to transformed_cells
             transformed_cells.append(cell)
 
         # if the last cell was the end of a manually-graded question, add a close export tag
         if need_end_export:
             transformed_cells.append(
                 self.add_export_tag_to_cell(nbformat.v4.new_markdown_cell(), end=True))
@@ -368,14 +373,20 @@
             output_path (``pathlib.Path | str``): the path at which to write the notebook
             sanitize (``bool``): whether to sanitize the notebook (i.e. write the student version)
         """
         nb = self._get_sanitized_nb() if sanitize else self.transformed_nb
         if self.nb_transformer.assignment.is_rmd:
             rmarkdown_converter.write_as_rmd(nb, str(output_path), not sanitize)
         else:
+            try:
+                from nbformat.validator import normalize
+            except ImportError:
+                normalize = lambda nb: (0, nb)
+
+            _, nb = normalize(nb)
             nbformat.write(nb, str(output_path))
 
     def write_tests(self, tests_dir, include_hidden, force_files):
         """
         Write the tests, either to the notebook metadata or files in ``tests_dir`` as indicated by
         the assignment config.
```

### Comparing `otter-grader-4.4.1/otter/assign/output.py` & `otter-grader-5.0.0/otter/assign/output.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 from .assignment import Assignment
 from .notebook_transformer import NotebookTransformer, TransformedNotebookContainer
 from .r_adapter import rmarkdown_converter
 from .r_adapter.tests_manager import RAssignmentTestsManager
 from .tests_manager import AssignmentTestsManager
 from .utils import get_notebook_language
 
-from ..utils import NBFORMAT_VERSION
+from ..utils import loggers, NBFORMAT_VERSION
+
+
+LOGGER = loggers.get_logger(__name__)
 
 
 def write_output_dir(
     transformed_nb: TransformedNotebookContainer,
     output_dir: pathlib.Path,
     assignment: Assignment,
     sanitize: bool,
@@ -53,15 +56,15 @@
             output_fn = "environment.yml"
             shutil.copy(assignment.environment, str(output_dir / output_fn))
 
     # write tests
     transformed_nb.write_tests(str(tests_dir), not sanitize, assignment.tests.files)
 
     # write a temp dir for otter generate tests
-    if not sanitize and assignment.generate_enabled:
+    if not sanitize:
         assignment._temp_test_dir = pathlib.Path(tempfile.mkdtemp())
         transformed_nb.write_tests(str(assignment._temp_test_dir), True, True)
 
     transformed_nb.write_transformed_nb(output_path, sanitize)
 
     # copy files
     for file in assignment.files:
@@ -118,7 +121,10 @@
     shutil.rmtree(student_dir, ignore_errors=True)
     os.makedirs(autograder_dir, exist_ok=True)
     os.makedirs(student_dir, exist_ok=True)
 
     # populate directories
     write_output_dir(transformed_nb, autograder_dir, assignment, False)
     write_output_dir(transformed_nb, student_dir, assignment, True)
+
+    # print assignment summary
+    LOGGER.info(nb_transformer.tests_mgr.generate_assignment_summary())
```

### Comparing `otter-grader-4.4.1/otter/assign/plugins.py` & `otter-grader-5.0.0/otter/assign/plugins.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/question_config.py` & `otter-grader-5.0.0/otter/assign/question_config.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/r_adapter/cell_factory.py` & `otter-grader-5.0.0/otter/assign/r_adapter/cell_factory.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/r_adapter/rmarkdown_converter.py` & `otter-grader-5.0.0/otter/assign/r_adapter/rmarkdown_converter.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/r_adapter/solutions.py` & `otter-grader-5.0.0/otter/assign/r_adapter/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/r_adapter/tests_manager.py` & `otter-grader-5.0.0/otter/assign/r_adapter/tests_manager.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/solutions.py` & `otter-grader-5.0.0/otter/assign/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/tests_manager.py` & `otter-grader-5.0.0/otter/assign/tests_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Assignment tests manager for Otter Assign"""
 
 import os
+import pandas as pd
 import pprint
 import re
 import yaml
 
 from dataclasses import dataclass
 from jinja2 import Template
 from typing import Any, Dict, List, Optional, Union
@@ -371,21 +372,49 @@
         Args:
             question (``otter.assign.question_config.QuestionConfig``): the question config
 
         Returns:
             ``int | float``: the point value of the question
         """
         test_cases = self._tests_by_question.get(question.name, [])
+
+        points = question.points
+        if isinstance(points, dict):
+            points = points.get('each', 1) * len(test_cases)
+
         if len(test_cases) == 0:
-            if question.points is None and question.manual:
+            if points is None and question.manual:
                 raise ValueError(
                     f"Point value unspecified for question with no test cases: {question.name}")
 
-            return question.points if question.points is not None else 1
+            return points if points is not None else 1
 
         try:
-            resolved_test_cases = TestFile.resolve_test_file_points(question.points, test_cases)
+            resolved_test_cases = TestFile.resolve_test_file_points(points, test_cases)
         except Exception as e:
             raise type(e)(f"Error in \"{question.name}\" test cases: {e}")
 
         points = round(sum(tc.points for tc in resolved_test_cases), 5)
         return int(points) if points % 1 == 0 else points
+
+    def generate_assignment_summary(self):
+        """
+        Generate a summary of the assignment's questions.
+
+        Returns:
+            ``str``: the summary
+        """
+        rows, manual, autograded, total = [], 0, 0, 0
+        for question_name in sorted(self._tests_by_question.keys()):
+            config = self._questions[question_name]
+            points = self.determine_question_point_value(config)
+            rows.append({"name": question_name, "points": points})
+            total += points
+            if config.manual: manual += points
+            else: autograded += points
+
+        summary = f"Assignment summary:\n"
+        summary += f"Total points: {total}\n"
+        summary += f"Autograded:   {autograded}\n"
+        summary += f"Manual:       {manual}\n\n"
+        summary += str(pd.DataFrame(rows))
+        return summary
```

### Comparing `otter-grader-4.4.1/otter/assign/utils.py` & `otter-grader-5.0.0/otter/assign/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 """Utilities for Otter Assign"""
 
 import copy
-import datetime as dt
 import json
 import os
 import pathlib
 import re
 import shutil
 
-from glob import glob
+from contextlib import redirect_stdout, redirect_stderr
+from io import StringIO
 from textwrap import indent
 
-from ..execute import grade_notebook
+from ..api import grade_submission
 from ..generate import main as generate_autograder
-from ..utils import get_source, NOTEBOOK_METADATA_KEY
+from ..utils import get_source, NOTEBOOK_METADATA_KEY, loggers
+
+
+LOGGER = loggers.get_logger(__name__)
 
 
 class EmptyCellException(Exception):
     """
     Exception for empty cells to indicate deletion
     """
 
@@ -66,15 +69,15 @@
     Determine whether a cell is of a specific type.
 
     Args:
         cell (``nbformat.NotebookNode``): the cell to check
         cell_type (``str``): the cell type to check for
 
     Returns:
-        ``bool``: whether ``cell`` is of type ``cell_type``        
+        ``bool``: whether ``cell`` is of type ``cell_type``
     """
     return cell["cell_type"] == cell_type
 
 
 def remove_output(nb):
     """
     Remove all outputs from a notebook in-place.
@@ -185,43 +188,39 @@
         return str_to_doctest(code_lines, lines + ["... " + line])
     elif len(lines) > 0 and lines[-1].strip().endswith("\\"):
         return str_to_doctest(code_lines, lines + ["... " + line])
     else:
         return str_to_doctest(code_lines, lines + [">>> " + line])
 
 
-def run_tests(nb_path, debug=False, seed=None, plugin_collection=None):
+def run_tests(assignment, debug=False):
     """
     Grade a notebook and throw an error if it does not receive a perfect score.
 
     Args:
-        nb_path (``pathlib.Path``): the path to the notebook to grade
-        debug (``bool``, optional): whether to raise errors instead of ignoring them
-        seed (``int``, optional): an RNG seed for notebook execution
-        plugin_collection (``otter.plugins.PluginCollection``, optional): plugins to run while
-            grading
+        assignment (``otter.assgin.assignment.Assignment``): the assignment config
+        debug (``bool``): whether to throw errors instead of swallowing them during grading
 
     Raises:
         ``RuntimeError``: if the grade received by the notebook is not 100%
     """
-    curr_dir = os.getcwd()
-    os.chdir(nb_path.parent)
+    stdout = StringIO()
+    with redirect_stdout(stdout), redirect_stderr(stdout):
+        results = grade_submission(
+            str(assignment.ag_notebook_path),
+            str(assignment.ag_zip_path),
+            debug=debug,
+        )
 
-    results = grade_notebook(
-        nb_path.name, tests_glob=glob(os.path.join("tests", "*.py")), cwd=os.getcwd(), 
-    	test_dir=os.path.join(os.getcwd(), "tests"), ignore_errors = not debug, seed=seed,
-        plugin_collection=plugin_collection
-    )
+    LOGGER.debug(f"Otter Run output:\n{stdout.getvalue()}")
 
     if results.total != results.possible:
         raise RuntimeError(f"Some autograder tests failed in the autograder notebook:\n" + \
             indent(results.summary(), '    '))
 
-    os.chdir(curr_dir)
-
 
 def write_otter_config_file(assignment):
     """
     Create an Otter configuration file (a ``.otter`` file) for students to use Otter tools,
     including saving environments and submitting to an Otter Service deployment, using assignment
     configurations. Writes the resulting file to the ``autograder`` and ``student`` subdirectories
     of ``assignment.result``.
@@ -244,15 +243,15 @@
     with open(assignment.get_stu_path(config_name), "w+") as f:
         json.dump(config, f, indent=4)
 
 
 # TODO: update for new assign format
 def run_generate_autograder(assignment, gs_username, gs_password, plugin_collection=None):
     """
-    Run Otter Generate on the autograder directory to generate a Gradescope zip file. Relies on 
+    Run Otter Generate on the autograder directory to generate a Gradescope zip file. Relies on
     configurations in ``assignment.generate``.
 
     Args:
         assignment (``otter.assign.assignment.Assignment``): the assignment configurations
         gs_username (``str``): Gradescope username for token generation
         gs_password (``str``): Gradescope password for token generation
         plugin_collection (``otter.plugins.PluginCollection``, optional): a plugin collection to pass
@@ -309,32 +308,30 @@
     if otter_config:
         # TODO: move this filename into a global variable somewhere and remove all of the places
         # it's hardcoded
         with open("otter_config.json", "w+") as f:
             json.dump(otter_config, f, indent=2)
 
     # TODO: change generate_autograder so that only necessary kwargs are needed
-    timestamp = dt.datetime.now().strftime("%Y_%m_%dT%H_%M_%S_%f")
-    notebook_name = assignment.master.stem
-    output_path = f"{notebook_name}-autograder_{timestamp}.zip"
     generate_autograder(
         tests_dir=test_dir,
-        output_path=output_path,
+        output_path=assignment.ag_zip_name,
         config="otter_config.json" if otter_config else None,
         lang="python" if assignment.is_python else "r",
         requirements=requirements,
         overwrite_requirements=assignment.overwrite_requirements,
         environment="environment.yml" if assignment.environment else None,
         no_environment=False,
         username=gs_username,
         password=gs_password,
         files=files,
         plugin_collection=plugin_collection,
         assignment=assignment,
         python_version=assignment.get_python_version(),
+        channel_priority_strict=assignment.channel_priority_strict,
     )
 
     # clean up temp tests dir
     if assignment._temp_test_dir is not None:
         shutil.rmtree(str(assignment._temp_test_dir))
 
     os.chdir(curr_dir)
```

### Comparing `otter-grader-4.4.1/otter/assign/v0/__init__.py` & `otter-grader-5.0.0/otter/assign/v0/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/assignment.py` & `otter-grader-5.0.0/otter/assign/v0/assignment.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/cell_generators.py` & `otter-grader-5.0.0/otter/assign/v0/cell_generators.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/constants.py` & `otter-grader-5.0.0/otter/assign/v0/constants.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/convert/__main__.py` & `otter-grader-5.0.0/otter/assign/v0/convert/__main__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/convert/notebook_transformer.py` & `otter-grader-5.0.0/otter/assign/v0/convert/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/notebook_transformer.py` & `otter-grader-5.0.0/otter/assign/v0/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/output.py` & `otter-grader-5.0.0/otter/assign/v0/output.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/plugins.py` & `otter-grader-5.0.0/otter/assign/v0/plugins.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/questions.py` & `otter-grader-5.0.0/otter/assign/v0/questions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/r_adapter/tests.py` & `otter-grader-5.0.0/otter/assign/v0/r_adapter/tests.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py` & `otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/notebook_transformer.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/output.py` & `otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/output.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/solutions.py` & `otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/tests.py` & `otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/tests.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/rmarkdown_adapter/utils.py` & `otter-grader-5.0.0/otter/assign/v0/rmarkdown_adapter/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/solutions.py` & `otter-grader-5.0.0/otter/assign/v0/solutions.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/tests.py` & `otter-grader-5.0.0/otter/assign/v0/tests.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/assign/v0/utils.py` & `otter-grader-5.0.0/otter/assign/v0/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/check/__init__.py` & `otter-grader-5.0.0/otter/check/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,42 +2,43 @@
 
 import os
 
 from glob import glob
 
 from .logs import LogEntry, EventType
 from .notebook import _OTTER_LOG_FILENAME
+from .utils import list_test_files
 
 from ..execute import grade_notebook
-from ..utils import block_print, loggers
+from ..utils import loggers
 
 
 _ALLOWED_EXTENSIONS = {".py", ".ipynb"}
 LOGGER = loggers.get_logger(__name__)
 
 
 def _log_event(event_type, results=[], question=None, success=True, error=None):
     """
     Logs an event
 
     Args:
         event_type (``otter.logs.EventType``): the type of event
-        results (``list`` of ``otter.test_files.abstract_test.TestCollectionResults``, optional): the 
+        results (``list`` of ``otter.test_files.abstract_test.TestCollectionResults``, optional): the
             results of any checks recorded by the entry
         question (``str``, optional): the question name for this check
         success (``bool``, optional): whether the operation was successful
         error (``Exception``, optional): the exception thrown by the operation, if applicable
     """
     LOGGER.debug(f"Creating a LogEntry of type {event_type}")
 
     LogEntry(
         event_type,
         results=results,
-        question=question, 
-        success=success, 
+        question=question,
+        success=success,
         error=error
     ).flush_to_file(_OTTER_LOG_FILENAME)
 
     LOGGER.debug(f"LogEntry created successfully")
 
 
 def main(file, *, tests_path="./tests", question=None, seed=None):
@@ -61,15 +62,15 @@
 
             LOGGER.info(f"Found test file {test_path}")
             qs = [test_path]
 
         else:
             LOGGER.info(f"Searching for test files in tests directory")
 
-            qs = glob(os.path.join(tests_path, "*.py"))
+            qs = list_test_files(tests_path)
 
             LOGGER.debug(f"Found test files: {', '.join(qs)}")
 
         LOGGER.debug(f"Checking for existence of submission file '{file}'")
         if not os.path.isfile(file):
             raise FileNotFoundError(f"{file} does not exist")
 
@@ -80,21 +81,22 @@
             raise ValueError(f"Invalid extension for file '{ext}'; must be one of {_ALLOWED_EXTENSIONS}")
 
         script = ext == ".py"
         LOGGER.debug(f"Determined if submission is a Python script: {script}")
 
         LOGGER.debug(f"Seed value: {seed}")
         LOGGER.info("Grading submission")
-        with block_print():
-            results = grade_notebook(
-                file,
-                tests_glob=qs,
-                script=script,
-                seed=seed,
-            )
+
+        results = grade_notebook(
+            file,
+            tests_glob=qs,
+            test_dir=tests_path,
+            script=script,
+            seed=seed,
+        )
 
         percentage = results.total / results.possible
         LOGGER.debug(f"Determined score percentage: {percentage}")
 
         if percentage == 1:
             output = "All tests passed!"
```

### Comparing `otter-grader-4.4.1/otter/check/logs.py` & `otter-grader-5.0.0/otter/check/logs.py`

 * *Files 1% similar despite different names*

```diff
@@ -287,15 +287,16 @@
                     break
 
             log = list(sorted(log, key = lambda l: l.timestamp, reverse = not ascending))
 
             return log
 
         finally:
-            file.close()
+            if "file" in locals():
+                file.close()
 
     @staticmethod
     def shelve_environment(env, variables=None, ignore_modules=[]):
         """
         Pickles an environment ``env`` using dill, ignoring any functions whose module is listed in
         ``ignore_modules``. Returns the pickle file contents as a ``bytes`` object and a list of
         variable names that were unable to be shelved/ignored during shelving.
```

### Comparing `otter-grader-4.4.1/otter/check/notebook.py` & `otter-grader-5.0.0/otter/check/notebook.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,28 +3,27 @@
 import datetime as dt
 import inspect
 import json
 import os
 import warnings
 import zipfile
 
-from contextlib import contextmanager
 from glob import glob
 from IPython.display import display, HTML
 from textwrap import indent
 
 from .logs import LogEntry, EventType, Log
 from .utils import grade_zip_file, grading_mode_disabled, incompatible_with, IPythonInterpreter, \
     list_available_tests, logs_event, resolve_test_info, save_notebook
 
 from ..execute import Checker
 from ..export import export_notebook
 from ..plugins import PluginCollection
 from ..test_files import GradingResults
-from ..utils import Loggable, loggers
+from ..utils import Loggable
 
 
 _OTTER_LOG_FILENAME = ".OTTER_LOG"
 _SHELVE = False
 _ZIP_NAME_FILENAME = "__zip_filename__"
 
 
@@ -91,39 +90,23 @@
             _SHELVE = self._config.get("save_environment", False)
             self._ignore_modules = self._config.get("ignore_modules", [])
             self._vars_to_store = self._config.get("variables", None)
 
             self._notebook = self._config["notebook"]
 
     @classmethod
-    @contextmanager
-    def grading_mode(cls, tests_dir):
-        """
-        A context manager for the ``Notebook`` grading mode. Yields a pointer to the list of results
-        that will be populated during grading.
-
-        **It is the caller's responsibility to maintain the pointer.** The pointer in the ``Checker``
-        class will be overwritten when the context exits.
-        """
+    def init_grading_mode(cls, tests_dir):
         logger = cls._get_logger()
         logger.info("Entering Notebook grading mode")
         logger.debug(f"Overriding tests directory: {tests_dir}")
         cls._grading_mode = True
         cls._tests_dir_override = tests_dir
         Checker.clear_results()
         Checker.enable_tracking()
 
-        yield Checker.get_results()
-
-        logger.info("Exiting Notebook grading mode")
-        cls._grading_mode = False
-        cls._tests_dir_override = None
-        Checker.disable_tracking()
-        Checker.clear_results()
-
     @incompatible_with(IPythonInterpreter.PYOLITE, throw_error=False)
     def _log_event(self, event_type, results=[], question=None, success=True, error=None, shelve_env={}):
         """
         Logs an event
 
         Args:
             event_type (``otter.logs.EventType``): the type of event
```

### Comparing `otter-grader-4.4.1/otter/check/utils.py` & `otter-grader-5.0.0/otter/check/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -197,14 +197,29 @@
             self._log_event(event_type, results=results, question=question, shelve_env=shelve_env)
 
         return results
 
     return event_logger
 
 
+def list_test_files(tests_dir):
+    """
+    Find all of the test files in the specified directory (that is, all ``.py`` files that are not
+    named ``__init__.py``) and return their paths in a sorted list.
+
+    Args:
+        tests_dir (``str``): the path to the tests directory
+
+    Returns:
+        ``list[str]``: the sorted list of all test file paths in ``tests_dir``
+    """
+    return sorted([file for file in glob(os.path.join(tests_dir, "*.py")) \
+            if file != "__init__.py"])
+
+
 def list_available_tests(tests_dir, nb_path):
     """
     Get a list of available questions by searching the tests directory (if present) or the notebook
     metadata.
 
     Args:
         tests_dir (``str``): the path to the tests directory
@@ -212,16 +227,15 @@
 
     Returns:
         ``list[str]``: the sorted list of question names
     """
     get_stem = lambda p: os.path.splitext(os.path.basename(p))[0]
 
     if tests_dir and os.path.isdir(tests_dir):
-        tests = [get_stem(file) for file in glob(os.path.join(tests_dir, "*.py")) \
-            if file != "__init__.py"]
+        tests = map(get_stem, list_test_files(tests_dir))
 
     else:
         if nb_path is None:
             raise ValueError("Tests directory does not exist and no notebook path provided")
 
         nb = nbf.read(nb_path, as_version=NBFORMAT_VERSION)
         tests = list(nb["metadata"][NOTEBOOK_METADATA_KEY]["tests"].keys())
```

### Comparing `otter-grader-4.4.1/otter/check/validate_export/__main__.py` & `otter-grader-5.0.0/otter/check/validate_export/__main__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/cli.py` & `otter-grader-5.0.0/otter/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -52,15 +52,14 @@
 @click.argument("master", type=click.Path(exists=True, dir_okay=False))
 @click.argument("result", type=click.Path())
 @click.option("--no-run-tests", is_flag=True, help="Do not run the tests against the autograder notebook")
 @click.option("--no-pdfs", is_flag=True, help="Do not generate PDFs; overrides assignment config")
 @click.option("--username", help="Gradescope username for generating a token")
 @click.option("--password", help="Gradescope password for generating a token")
 @click.option("--debug", is_flag=True, help="Do not ignore errors in running tests for debugging")
-@click.option("--v0", is_flag=True, help="Use Otter Assign format v0 instead of v1")
 def assign_cli(*args, **kwargs):
     """
     Create distribution versions of the Otter Assign formatted notebook MASTER and write the
     results to the directory RESULT, which will be created if it does not already exist.
     """
     return assign(*args, **kwargs)
 
@@ -84,15 +83,15 @@
 @_verbosity
 @click.argument("src", type=click.Path(exists=True, dir_okay=False))
 @click.argument("dest", required=False, type=click.Path())
 @click.option("--filtering", is_flag=True, help="Whether the PDF should be filtered")
 @click.option("--pagebreaks", is_flag=True, help="Whether the PDF should have pagebreaks between questions")
 @click.option("-s", "--save", is_flag=True, help="Save intermediate file(s) as well")
 @click.option("-e", "--exporter", default=defaults["exporter"], type=click.Choice(["latex", "html"]), help="Type of PDF exporter to use")
-@click.option("--no-xecjk", is_flag=True, help="Force-disable xeCJK in Otter's LaTeX template")
+@click.option("--xecjk", is_flag=True, help="Enable xeCJK in Otter's LaTeX template")
 def export_cli(*args, **kwargs):
     """
     Export a Jupyter Notebook SRC as a PDF at DEST with optional filtering.
 
     If unspecified, DEST is assumed to be the basename of SRC with a .pdf extension.
     """
     return export(*args, **kwargs)
@@ -111,50 +110,44 @@
 @click.option("-e", "--environment", type=click.Path(exists=True, dir_okay=False), help="Path to environment.yml file; ./environment.yml automatically checked (overwrite)")
 @click.option("--no-environment", is_flag=True, help="Disable auto-inclusion of unespecified environment file at ./environment.yml")
 @click.option("-l", "--lang", help="Assignment programming language; defaults to Python")
 @click.option("--username", help="Gradescope username for generating a token")
 @click.option("--password", help="Gradescope password for generating a token")
 @click.option("--token", help="Gradescope token for uploading PDFs")
 @click.option("--python-version", help="Python version to use in the grading image")
+@click.option("--channel-priority-strict", is_flag=True, help="Whether to set conda's channel_priority to strict in the setup.sh file")
 @click.argument("files", nargs=-1)
 def generate_cli(*args, **kwargs):
     """
     Generate a zip file to configure an Otter autograder, including FILES as support files.
     """
     return generate(*args, **kwargs)
 
 
 defaults = grade.__kwdefaults__
 @cli.command("grade")
 @_verbosity
-
-# necessary path arguments
-@click.option("-p", "--path", default=defaults["path"], help="Path to directory of submissions")
+@click.argument("paths", nargs=-1, type=click.Path(exists=True))
+@click.option("-n", "--name", help="An assignment name to use in the Docker image tag")
 @click.option("-a", "--autograder", default=defaults["autograder"], help="Path to autograder zip file")
 @click.option("-o", "--output-dir", default=defaults["output_dir"], help="Directory to which to write output")
-
-# submission format arguments
-@click.option("-z", "--zips", is_flag=True, help="Whether submissions are zip files from Notebook.export")
 @click.option("--ext", default=defaults["ext"], type=click.Choice(_ALLOWED_EXTENSIONS), help="The extension to glob for submissions")
-
-# PDF export options
 @click.option("--pdfs", is_flag=True, help="Whether to copy notebook PDFs out of containers")
-
-# other settings and optional arguments
-@click.option("--containers", type=click.INT, help="Specify number of containers to run in parallel")
-@click.option("--image", default=defaults["image"], help="Custom docker image to run on")
+@click.option("--containers", default=defaults["containers"], type=click.INT, help="Specify number of containers to run in parallel")
+@click.option("--image", default=defaults["image"], help="A Docker image tag to use as the base image")
 @click.option("--timeout", type=click.INT, help="Submission execution timeout in seconds")
 @click.option("--no-network", is_flag=True, help="Disable networking in the containers")
 @click.option("--no-kill", is_flag=True, help="Do not kill containers after grading")
-
+@click.option("--debug", is_flag=True, help="Run in debug mode (without ignoring errors thrown during execution)")
 @click.option("--prune", is_flag=True, help="Prune all of Otter's grading images")
 @click.option("-f", "--force", is_flag=True, help="Force action (don't ask for confirmation)")
 def grade_cli(*args, **kwargs):
     """
-    Grade assignments locally using Docker containers.
+    Grade submissions in PATHS locally using Docker containers. PATHS can be individual file paths
+    or directories containing submissions ending with extension EXT.
     """
     g = grade(*args, **kwargs)
     if g is not None:
         click.echo(g)
     return g
```

### Comparing `otter-grader-4.4.1/otter/execute/__init__.py` & `otter-grader-5.0.0/otter/execute/execute_log.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,103 +1,92 @@
-"""Execution and grading internals for Otter-Grader"""
+"""Execution of a submission through log deserialization"""
 
-import nbformat
+import re
 
-from .checker import Checker
-from .execute_log import execute_log
-from .execute_notebook import execute_notebook
-from .transforms import filter_ignored_cells, script_to_notebook
+from IPython.core.inputsplitter import IPythonInputSplitter
+from unittest import mock
 
-from ..test_files import create_test_file, GradingResults
-from ..utils import id_generator, NBFORMAT_VERSION
+from ..utils import get_variable_type
 
 
-def grade_notebook(submission_path, *, tests_glob=None, name=None, ignore_errors=True, script=False, 
-    cwd=None, test_dir=None, seed=None, seed_variable=None, log=None, variables=None, 
-    plugin_collection=None):
+def execute_log(nb, log, check_results_list_name="check_results_secret", initial_env=None, 
+                ignore_errors=False, cwd=None, test_dir=None, variables=None):
     """
-    Grade an assignment file and return grade information
+    Execute a notebook from logged environments and return the global environment that results.
+
+    If ``ignore_errors`` is true, exceptions are swallowed.
 
     Args:
-        submission_path (``str``): path to a single notebook or Python script
-        tests_glob (``list`` of ``str``, optional): paths to test files to run
-        name (``str``, optional): initial environment name
-        ignore_errors (``bool``, optional): whether errors in execution should be ignored
-        script (``bool``, optional): whether the ``submission_path`` is a Python script
+        nb (``nbformat.NotebookNode``): the notebook to execute
+        log (``otter.check.logs.Log``): log from notebook execution
+        check_results_list_name (``str``, optional): the name of the list to collect check results in
+        initial_env (``str``, optional): name of initial environment
+        ignore_errors (``bool``, optional): whether exceptions should be ignored
         cwd (``str``, optional): working directory of execution to be appended to ``sys.path`` in 
             grading environment
         test_dir (``str``, optional): path to directory of tests in grading environment
-        seed (``int``, optional): random seed for intercell seeding
-        seed_variable (``str``, optional): a variable name to override with the seed
-        log (``otter.check.logs.Log``, optional): log from which to grade questions
         variables (``dict``, optional): map of variable names -> type string to check type of deserialized
-            object to prevent arbitrary code from being put into the environment; ignored if log is ``None``
-        plugin_collection (``otter.plugins.PluginCollection``, optional): a set of plugins to run on
-            this assignment during execution and grading
+            object to prevent arbitrary code from being put into the environment
 
-    Returns:
-        ``otter.test_files.GradingResults``: the results of grading
+    Results:
+        ``dict``: global environment resulting from executing all code of the input notebook
     """
-    if not script:
-        nb = nbformat.read(submission_path, as_version=NBFORMAT_VERSION)
-
+    if initial_env:
+        global_env = initial_env.copy()
     else:
-        with open(submission_path) as f:
-            nb = f.read()
-
-        nb = script_to_notebook(nb)
-
-    if plugin_collection is not None:
-        nb = plugin_collection.before_execution(nb)
-
-    # remove any ignored cells from the notebook
-    if not script:
-        nb = filter_ignored_cells(nb)
-
-    secret = id_generator()
-    results_array = "check_results_{}".format(secret)
-    initial_env = {
-        results_array: []
-    }
-
-    if name:
-        initial_env["__name__"] = name
-
-    if log is not None:
-        global_env = execute_log(
-            nb, log, results_array, initial_env, ignore_errors=ignore_errors, cwd=cwd, test_dir=test_dir, 
-            variables=variables)
+        global_env = {}
 
+    if test_dir:
+        source = f"import otter\ngrader = otter.Notebook(\"{test_dir}\")\n"
     else:
-        global_env = execute_notebook(
-            nb, results_array, initial_env, ignore_errors=ignore_errors, cwd=cwd, test_dir=test_dir, 
-            seed=seed, seed_variable=seed_variable)
-
-    if plugin_collection is not None:
-        plugin_collection.run("after_execution", global_env)
-
-    tests_run = global_env[results_array]
-
-    # Check for tests which were not included in the notebook and specified by tests_globs
-    # Allows instructors to run notebooks with additional tests not accessible to user
-    if tests_glob:
-        # unpack list of paths into a single list
-        tested_set = [test.path for test in tests_run]
-        extra_tests = []
-        for t in sorted(tests_glob):
-            include = True
-            for tested in tested_set:
-                if tested in t or t in tested:     # e.g. if 'tests/q1.py' is in /srv/repo/lab01/tests/q1.py
-                    include = False
-
-            if include:
-                extra_tests.append(create_test_file(t))
-                extra_tests[-1].run(global_env)
+        source = f"import otter\ngrader = otter.Notebook()\n"
 
-        tests_run += extra_tests
+    if cwd:
+        source +=  f"import sys\nsys.path.append(\"{cwd}\")\n"
 
-    results = GradingResults(tests_run)
+    logged_questions = []
+    m = mock.mock_open()
+    with mock.patch("otter.Notebook._log_event", m):
+        exec(source, global_env)
+
+        for cell in nb['cells']:
+            if cell['cell_type'] == 'code':
+                # transform the input to executable Python
+                # FIXME: use appropriate IPython functions here
+                isp = IPythonInputSplitter(line_input_checker=False)
+
+                code_lines = []
+                cell_source_lines = cell['source']
+                source_is_str_bool = False
+                if isinstance(cell_source_lines, str):
+                    source_is_str_bool = True
+                    cell_source_lines = cell_source_lines.split('\n')
+
+                # only execute import statements
+                cell_source_lines = [re.sub(r"^\s+", "", l) for l in cell_source_lines if "import" in l]                                
+
+                for line in cell_source_lines:
+                    try:
+                        exec(line, global_env)
+
+                    except:
+                        if not ignore_errors:
+                            raise
+
+        for entry in log.question_iterator():
+            shelf = entry.unshelve(global_env)
+
+            if variables is not None:
+                for k, v in shelf.items():
+                    full_type = get_variable_type(v)
+                    if not (k in variables and variables[k] == full_type):
+                        del shelf[k]
+                        print(f"Found variable of different type than expected: {k}")
+
+            global_env.update(shelf)
+            global_env[check_results_list_name].append(
+                global_env["grader"].check(entry.question, global_env=global_env))
+            logged_questions.append(entry.question)
 
-    if plugin_collection is not None:
-        plugin_collection.run("after_grading", results)
+    print("Questions executed from log: {}".format(", ".join(logged_questions)))
 
-    return results
+    return global_env
```

### Comparing `otter-grader-4.4.1/otter/execute/checker.py` & `otter-grader-5.0.0/otter/execute/checker.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,27 +48,22 @@
         points to it.
         """
         cls._test_files = []
 
     @classmethod
     def check(cls, nb_or_test_path, test_name=None, global_env=None):
         """
-        Checks a global environment against given test file. If ``global_env`` is ``None``, the global 
-        environment of the calling frame is used; i.e., the following two calls are equivalent:
-
-        .. code-block:: python
-
-            check('tests/q1.py')
-            check('tests/q1.py', global_env=globals())
+        Checks a global environment against a test, which may be stored in a file or in a notebook's
+        metadata.
 
         Args:
             nb_or_test_path (``str``): path to test file or notebook
             test_name (``str``, optional): the name of the test if a notebook metadata test
-            global_env (``dict``, optional): a global environment resulting from the execution 
-                of a python script or notebook
+            global_env (``dict``, optional): the global environment in which to run the test; if
+                unspecified, the calling frame's global environment is used
 
         Returns:
             ``otter.test_files.abstract_test.TestFile``: result of running the tests in the 
             given global environment
         """
         test = create_test_file(nb_or_test_path, test_name=test_name)
 
@@ -77,7 +72,32 @@
 
         test.run(global_env)
 
         if cls._track_results:
             cls._test_files.append(test)
 
         return test
+
+    @classmethod
+    def check_if_not_already_checked(cls, test_path, global_env=None):
+        """
+        Run the specified test if it has not already been run (that is, if its result is not cached
+        in this ``Checker`` instance).
+
+        This method only works with test files.
+
+        Args:
+            test_path (``str``): path to test file
+            global_env (``dict``, optional): the global environment in which to run the test; if
+                unspecified, the calling frame's global environment is used
+
+        Returns:
+            ``otter.test_files.abstract_test.TestFile``: result of running the tests in the 
+            given global environment
+        """
+        if any(test_path in tf.path or tf.path in test_path for tf in cls._test_files):
+            return
+
+        if global_env is None:
+            global_env = inspect.currentframe().f_back.f_globals
+
+        return cls.check(test_path, global_env=global_env)
```

### Comparing `otter-grader-4.4.1/otter/execute/execute_log.py` & `otter-grader-5.0.0/otter/execute/execute_notebook.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,92 +1,137 @@
-"""Execution of a submission through log deserialization"""
+"""Execution of a Jupyter Notebook"""
 
-import re
+import copy
+import os
+import tempfile
 
-from IPython.core.inputsplitter import IPythonInputSplitter
-from unittest import mock
+from contextlib import redirect_stdout, redirect_stderr
+from IPython.display import display
 
-from ..utils import get_variable_type
+try:
+    from IPython.core.inputtransformer2 import TransformerManager
+    _IPYTHON_7 = True
+except ImportError:
+    from IPython.core.inputsplitter import IPythonInputSplitter
+    _IPYTHON_7 = False
 
+from .transforms import create_collected_check_cell
 
-def execute_log(nb, log, check_results_list_name="check_results_secret", initial_env=None, 
-                ignore_errors=False, cwd=None, test_dir=None, variables=None):
+from ..utils import id_generator
+
+
+def execute_notebook(nb, check_results_list_name="check_results_secret", initial_env=None, 
+                     ignore_errors=False, cwd=None, test_dir=None, seed=None, seed_variable=None):
     """
-    Execute a notebook from logged environments and return the global environment that results.
+    Execute a notebook and return the global environment that results from execution.
 
     If ``ignore_errors`` is true, exceptions are swallowed.
 
     Args:
         nb (``nbformat.NotebookNode``): the notebook to execute
-        log (``otter.check.logs.Log``): log from notebook execution
         check_results_list_name (``str``, optional): the name of the list to collect check results in
-        initial_env (``str``, optional): name of initial environment
+        initial_env (``dict``, optional): an initial environment
         ignore_errors (``bool``, optional): whether exceptions should be ignored
         cwd (``str``, optional): working directory of execution to be appended to ``sys.path`` in 
             grading environment
         test_dir (``str``, optional): path to directory of tests in grading environment
-        variables (``dict``, optional): map of variable names -> type string to check type of deserialized
-            object to prevent arbitrary code from being put into the environment
+        seed (``int``, optional): random seed for intercell seeding
+        seed_variable (``str``, optional): a variable name to override with the seed
 
     Results:
         ``dict``: global environment resulting from executing all code of the input notebook
     """
     if initial_env:
         global_env = initial_env.copy()
+
     else:
         global_env = {}
 
-    if test_dir:
-        source = f"import otter\ngrader = otter.Notebook(\"{test_dir}\")\n"
-    else:
-        source = f"import otter\ngrader = otter.Notebook()\n"
+    # add display from IPython
+    global_env["display"] = display
 
-    if cwd:
-        source +=  f"import sys\nsys.path.append(\"{cwd}\")\n"
+    test_dir = test_dir if test_dir is not None else './tests'
 
-    logged_questions = []
-    m = mock.mock_open()
-    with mock.patch("otter.Notebook._log_event", m):
-        exec(source, global_env)
+    from ..check.notebook import Notebook
+    with Notebook.grading_mode(tests_dir = test_dir if test_dir is not None else './tests') as check_results:
+        # add dummy Notebook class so that we can collect results
+        secret = id_generator()
+        notebook_class_name = f"Notebook_{secret}"
+        global_env[notebook_class_name] = Notebook
+
+        source = ""
+
+        if cwd:
+            source = f"import sys\nsys.path.append(r\"{cwd}\")\n"
+            exec(source, global_env)
+
+        if seed is not None and seed_variable is None:
+            import numpy as np
+            import random
+            global_env["np"] = np
+            global_env["random"] = random
 
         for cell in nb['cells']:
             if cell['cell_type'] == 'code':
-                # transform the input to executable Python
-                # FIXME: use appropriate IPython functions here
-                isp = IPythonInputSplitter(line_input_checker=False)
-
-                code_lines = []
-                cell_source_lines = cell['source']
-                source_is_str_bool = False
-                if isinstance(cell_source_lines, str):
-                    source_is_str_bool = True
-                    cell_source_lines = cell_source_lines.split('\n')
-
-                # only execute import statements
-                cell_source_lines = [re.sub(r"^\s+", "", l) for l in cell_source_lines if "import" in l]                                
-
-                for line in cell_source_lines:
-                    try:
-                        exec(line, global_env)
-
-                    except:
-                        if not ignore_errors:
-                            raise
-
-        for entry in log.question_iterator():
-            shelf = entry.unshelve(global_env)
-
-            if variables is not None:
-                for k, v in shelf.items():
-                    full_type = get_variable_type(v)
-                    if not (k in variables and variables[k] == full_type):
-                        del shelf[k]
-                        print(f"Found variable of different type than expected: {k}")
-
-            global_env.update(shelf)
-            global_env[check_results_list_name].append(
-                global_env["grader"].check(entry.question, global_env=global_env))
-            logged_questions.append(entry.question)
+                if _IPYTHON_7:
+                    isp = TransformerManager()
+
+                else:
+                    isp = IPythonInputSplitter(line_input_checker=False)
+
+                try:
+                    code_lines = []
+                    cell_source_lines = cell['source']
+                    # TODO: use otter.utils.get_source
+                    source_is_str_bool = False
+                    if isinstance(cell_source_lines, str):
+                        source_is_str_bool = True
+                        cell_source_lines = cell_source_lines.split('\n')
+
+                    for line in cell_source_lines:
+                        if not line.startswith('%') and  "interact(" not in line:
+                            code_lines.append(line)
+                            if source_is_str_bool:
+                                code_lines.append('\n')
+
+                    # TODO: move to helper function
+                    if seed is not None:
+                        if seed_variable is None:
+                            cell_source = f"np.random.seed({seed})\nrandom.seed({seed})\n" + \
+                                isp.transform_cell(''.join(code_lines))
+
+                        else:
+                            cell_source = f"{seed_variable} = {seed}\n" + \
+                                isp.transform_cell(''.join(code_lines))
+
+                    else:
+                        cell_source = isp.transform_cell(''.join(code_lines))
+
+                    with open(os.devnull, 'w') as f, redirect_stdout(f), redirect_stderr(f):
+                        exec(cell_source, global_env)
+
+                    source += cell_source
+
+                except:
+                    if not ignore_errors:
+                        raise
+
+            # add any required checks from this cell
+            source += create_collected_check_cell(cell, notebook_class_name, test_dir)
+
+        with tempfile.NamedTemporaryFile(mode="w", suffix=".py") as ntf:
+            ntf.write(source)
+            ntf.seek(0)
+
+            try:
+                cleaned_source = compile(source, filename=ntf.name, mode="exec")
+                with open(os.devnull, 'w') as f, redirect_stdout(f), redirect_stderr(f):
+                    exec(cleaned_source, global_env)
+
+            except:
+                if not ignore_errors:
+                    raise
 
-    print("Questions executed from log: {}".format(", ".join(logged_questions)))
+        # add the collected results to the global env
+        global_env[check_results_list_name] = check_results
 
     return global_env
```

### Comparing `otter-grader-4.4.1/otter/execute/transforms.py` & `otter-grader-5.0.0/otter/execute/transforms.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/export/__init__.py` & `otter-grader-5.0.0/otter/export/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,31 +41,31 @@
     Exporter = get_exporter(exporter_type=exporter_type)
     Exporter.convert_notebook(nb_path, pdf_name, **kwargs)
 
     return pdf_name
 
 
 def main(src, *, dest=None, exporter=None, filtering=False, pagebreaks=False, save=False, 
-         no_xecjk=False):
+         xecjk=False):
     """
     Runs Otter Export
 
     Args:
         src (``str``): path to source notebook
         dest (``Optional[str]``): path at which to write PDF
         exporter (``Optional[str]``): exporter name
         filtering (``bool``): whether to filter cells using HTML comments
         pagebreaks (``bool``): whether to pagebreak between filtered regions; ignored if ``filtering``
             is ``False``
         save (``bool``): whether to save any intermediate files (e.g. ``.tex``, ``.html``)
-        no_xecjk (``bool``): whether to disable xeCJK in the LaTeX template
+        xecjk (``bool``): whether to use xeCJK in the LaTeX template
     """
     export_notebook(
         src,
         dest = dest,
         exporter_type = exporter,
         filtering = filtering,
         pagebreaks = pagebreaks,
         save_tex = save,
         save_html = save,
-        no_xecjk=no_xecjk,
+        xecjk=xecjk,
     )
```

### Comparing `otter-grader-4.4.1/otter/export/exporters/__init__.py` & `otter-grader-5.0.0/otter/export/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/export/exporters/base_exporter.py` & `otter-grader-5.0.0/otter/export/exporters/base_exporter.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/export/exporters/templates/via_html/index.html.j2` & `otter-grader-5.0.0/otter/export/exporters/templates/via_html/index.html.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/export/exporters/templates/via_html.tpl` & `otter-grader-5.0.0/otter/export/exporters/templates/via_html.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/export/exporters/templates/via_latex/index.tex.j2` & `otter-grader-5.0.0/otter/export/exporters/templates/via_latex/index.tex.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/export/exporters/templates/via_latex.tpl` & `otter-grader-5.0.0/otter/export/exporters/templates/via_latex.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2` & `otter-grader-5.0.0/otter/export/exporters/templates/via_latex_xecjk/index.tex.j2`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/export/exporters/templates/via_latex_xecjk.tpl` & `otter-grader-5.0.0/otter/export/exporters/templates/via_latex_xecjk.tpl`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/export/exporters/utils.py` & `otter-grader-5.0.0/otter/export/exporters/utils.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/export/exporters/via_html.py` & `otter-grader-5.0.0/otter/export/exporters/via_html.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 """PDF via HTML exporter"""
 
 import nbconvert
 import os
-import pdfkit
 import shutil
 
 from io import BytesIO
-from PyPDF2 import PdfFileMerger
 
 from .base_exporter import BaseExporter, NBCONVERT_6, TEMPLATE_DIR
 from .utils import notebook_pdf_generator
 
 
 class PDFViaHTMLExporter(BaseExporter):
     """
     Exports notebooks to PDF files using HTML as an intermediary
 
     Converts IPython notebooks to PDFs by first converting them into temporary HTML files that are then
     converted to PDFs using wkhtmltopdf and its Python API pdfkit which are then stitched together (if
-    pagebreaks are enabled) using PyPDF2.
+    pagebreaks are enabled) using pypdf.
 
     Attributes:
         default_options (``dict``): the default options for this exporter
     """
 
     default_options = BaseExporter.default_options.copy()
     default_options.update({
         "save_html": False,
         "template": "via_html"
     })
 
     @classmethod
     def convert_notebook(cls, nb_path, dest, **kwargs):
-        assert shutil.which("wkhtmltopdf") is not None, "Cannot export via HTML without wkhtmltopdf"
+        if shutil.which("wkhtmltopdf") is None:
+            raise RuntimeError("Cannot export via HTML without wkhtmltopdf")
+
+        import pdfkit
+        from pypdf import PdfMerger
 
         options = cls.default_options.copy()
         options.update(kwargs)
 
         nb = cls.load_notebook(nb_path, filtering=options["filtering"], pagebreaks=options["pagebreaks"])
 
         if NBCONVERT_6:
@@ -50,15 +52,15 @@
 
         if options["save_html"]:
             html, _ = nbconvert.export(exporter, nb)
             html_path = os.path.splitext(dest)[0] + ".html"
             with open(html_path, "wb+") as f:
                 f.write(html.encode("utf-8"))
 
-        merger = PdfFileMerger()
+        merger = PdfMerger()
         for subnb in notebook_pdf_generator(nb):
             html, _ = nbconvert.export(exporter, subnb)
 
             pdfkit_options = {
                 'enable-local-file-access': None, 
                 'quiet': '', 
                 'print-media-type': '', 
@@ -66,13 +68,13 @@
             }
             pdf_contents = pdfkit.from_string(html, False, options=pdfkit_options)
 
             output = BytesIO()
             output.write(pdf_contents)
             output.seek(0)
 
-            merger.append(output, import_bookmarks=False)
+            merger.append(output, import_outline=False)
 
         merger.write(dest)
 
         if NBCONVERT_6:
             nbconvert.TemplateExporter.template_name = orig_template_name
```

### Comparing `otter-grader-4.4.1/otter/export/exporters/via_latex.py` & `otter-grader-5.0.0/otter/export/exporters/via_latex.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,20 +27,17 @@
     default_options = BaseExporter.default_options.copy()
     default_options.update({
         "save_tex": False,
         "template": "via_latex",
     })
 
     @classmethod
-    def convert_notebook(cls, nb_path, dest, xecjk=False, no_xecjk=False, **kwargs):
+    def convert_notebook(cls, nb_path, dest, xecjk=False, **kwargs):
         warnings.filterwarnings("ignore", r"invalid escape sequence '\\c'", DeprecationWarning)
 
-        if xecjk and no_xecjk:
-            raise ValueError("xeCJK LaTeX template indicated but disallowed")
-
         options = cls.default_options.copy()
         options.update(kwargs)
 
         # choose the template to allow Chinese, Japanese, and Korean characters if necessary
         if xecjk:
             options["template"] = "via_latex_xecjk"
 
@@ -67,22 +64,18 @@
                     output_file.write(latex_output[0])
 
             pdf_output = nbconvert.export(pdf_exporter, nb)
             with open(dest, "wb") as output_file:
                 output_file.write(pdf_output[0])
 
         except nbconvert.pdf.LatexFailed as error:
-            if not xecjk and not no_xecjk:
-                cls.convert_notebook(nb_path, dest, xecjk=True, **kwargs)
-
-            else:
-                message = "There was an error generating your LaTeX; showing full error message:\n"
-                message += indent(error.output, "    ")
-                if xecjk:
-                    message += "\n\nIf the error above is related to xeCJK or fandol in LaTeX " \
-                        "and you don't require this functionality, try running again with " \
-                        "no_xecjk set to True or the --no-xecjk flag."
-                raise ExportFailedException(message)
+            message = "There was an error generating your LaTeX; showing full error message:\n"
+            message += indent(error.output, "    ")
+            if xecjk:
+                message += "\n\nIf the error above is related to xeCJK or fandol in LaTeX " \
+                    "and you don't require this functionality, try running again without " \
+                    "xecjk set to True or the --xecjk flag."
+            raise ExportFailedException(message)
 
         finally:
             if NBCONVERT_6:
                 nbconvert.TemplateExporter.template_name = orig_template_name
```

### Comparing `otter-grader-4.4.1/otter/generate/__init__.py` & `otter-grader-5.0.0/otter/generate/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -4,52 +4,137 @@
 import os
 import pathlib
 import pkg_resources
 import re
 import yaml
 import zipfile
 
+from dataclasses import dataclass
 from glob import glob
 from jinja2 import Template
+from typing import Any, Dict, List, Optional
 
 from .token import APIClient
-from .utils import zip_folder
+from .utils import merge_conda_environments, zip_folder
 
 from ..plugins import PluginCollection
 from ..run.run_autograder.autograder_config import AutograderConfig
-from ..utils import load_default_file
+from ..utils import dump_yaml, load_default_file
+from ..version import __version__
 
 
-DEFAULT_PYTHON_VERSION = "3.7"
-MINICONDA_INSTALL_URL = "https://repo.anaconda.com/miniconda/Miniconda3-py38_4.10.3-Linux-x86_64.sh"
+DEFAULT_PYTHON_VERSION = "3.9"
 OTTER_ENV_NAME = "otter-env"
-OTTR_BRANCH = "v1.2.0"  # this should match a release tag on GitHub
+OTTR_VERSION = "1.2.0"
 TEMPLATE_DIR = pkg_resources.resource_filename(__name__, "templates")
+GENERAL_TEMPLATE_DIR = os.path.join(TEMPLATE_DIR, "general")
 
 
+@dataclass
+class CondaEnvironment:
+
+    python_version: str
+
+    is_r: bool
+
+    requirements: List[str]
+
+    overwrite_requirements: bool
+
+    user_environment: Optional[Dict[str, Any]]
+
+    def to_dict(self):
+        environment = {
+            "name": OTTER_ENV_NAME,
+            "channels": ["defaults", "conda-forge"],
+            "dependencies": [
+                f"python={self.python_version}",
+                "pip",
+                "nb_conda_kernels",
+            ],
+        }
+
+        if self.is_r:
+            environment["channels"].append("r")
+            environment["dependencies"].extend([
+                "r-base>=4.0.0",
+                "r-essentials",
+                "r-devtools",
+                "libgit2",
+                "libgomp",
+                "r-gert",
+                "r-usethis",
+                "r-testthat",
+                "r-startup",
+                "r-rmarkdown",
+                "r-stringi",
+            ])
+
+        pip_deps = self.requirements if self.overwrite_requirements else [
+            "datascience",
+            "jupyter_client", 
+            "ipykernel", 
+            "matplotlib", 
+            "pandas", 
+            "ipywidgets", 
+            "scipy", 
+            "seaborn", 
+            "scikit-learn", 
+            "jinja2", 
+            "nbconvert", 
+            "nbformat", 
+            "dill",
+            "numpy",
+            "gspread",
+            "pypdf",
+            f"otter-grader=={__version__}",
+            *self.requirements,
+        ]
+
+        environment["dependencies"].append({"pip": pip_deps})
+
+        if self.is_r:
+            environment["dependencies"][-1]["pip"].append("rpy2")
+
+        if self.user_environment:
+            environment = merge_conda_environments(
+                self.user_environment, environment, OTTER_ENV_NAME)
+
+        return environment
+
+    def to_str(self):
+        return dump_yaml(self.to_dict(), indent=2)
+        # return yaml.safe_dump(self.to_dict(), sort_keys=False, indent=2)
+
+
+COMMON_TEMPLATES = [
+    os.path.join(TEMPLATE_DIR, "common", "run_autograder"),
+    os.path.join(TEMPLATE_DIR, "common", "run_otter.py"),
+]
+
 LANGUAGE_BASED_CONFIGURATIONS = {
     "python": {
         "test_file_pattern": "*.py",
         "requirements_filename": "requirements.txt",
-        "template_dir": os.path.join(TEMPLATE_DIR, "python"),
+        "templates": [*COMMON_TEMPLATES, os.path.join(TEMPLATE_DIR, "python", "setup.sh")]
     },
     "r": {
         "test_file_pattern": "*.[Rr]",
         "requirements_filename": "requirements.R",
-        "template_dir": os.path.join(TEMPLATE_DIR, "r"),
+        "templates": [*COMMON_TEMPLATES, os.path.join(TEMPLATE_DIR, "r", "setup.sh")]
     },
 }
 
 
 def main(*, tests_dir="./tests", output_path="autograder.zip", config=None, no_config=False, 
          lang=None, requirements=None, no_requirements=False, overwrite_requirements=False, 
          environment=None, no_environment=False, username=None, password=None, token=None, files=[], 
-         assignment=None, plugin_collection=None, python_version=None):
+         assignment=None, plugin_collection=None, python_version=None, channel_priority_strict=True):
     """
-    Runs Otter Generate
+    Run Otter Generate.
 
     Args:
         tests_dir (``str``): path to directory of test files for this assignment
         output_path (``str``): the path at which to write the output zip file
         config (``str``): path to an Otter configuration JSON file
         no_config (``bool``): disables auto-inclusion of Otter config file at ./otter_config.json
         lang (``str``): the language of the assignment; one of ``["python", "r"]``
@@ -63,14 +148,16 @@
         username (``str``): a username for Gradescope for generating a token
         password (``str``): a password for Gradescope for generating a token
         token (``str``): a token for Gradescope
         files (``list[str]``): list of file paths to add to the zip file
         assignment (``otter.assign.assignment.Assignment``, optional): the assignment configurations
             if used with Otter Assign
         python_version (``str | None``): the version of Python to use (installed with conda)
+        channel_priority_strict (``bool``): whether to set conda's channel_priority to strict in
+            the ``setup.sh`` file
 
     Raises:
         ``FileNotFoundError``: if the specified Otter configuration JSON file could not be found
         ``ValueError``: if the configurations specify a Gradescope course ID or assignment ID but not
             both
     """
     # read in otter_config.json
@@ -114,62 +201,68 @@
         otter_config["lang"] = lang
 
     if ag_config.lang not in LANGUAGE_BASED_CONFIGURATIONS.keys():
         raise ValueError(f"Invalid language specified: {ag_config.lang}")
 
     lang_config = LANGUAGE_BASED_CONFIGURATIONS[ag_config.lang]
 
-    template_dir = lang_config["template_dir"]
-
     templates = {}
-    for fn in os.listdir(template_dir):
-        fp = os.path.join(template_dir, fn)
-        if os.path.isfile(fp): # prevents issue w/ finding __pycache__ in template dirs
-            with open(fp) as f:
-                templates[fn] = Template(f.read())
+    for template_path in lang_config["templates"]:
+        fn = os.path.basename(template_path)
+        with open(template_path) as f:
+            templates[fn] = Template(f.read())
 
     if python_version is not None:
         match = re.match(r"(\d+)\.(\d+)(\.\d+)?", python_version)
         if not match:
             raise ValueError("Invalid Python version specified")
         if int(match.group(1)) < 3 or int(match.group(2)) < 6:
             raise ValueError("Otter is only compatible with Python 3.6+")
 
     template_context = {
         "autograder_dir": ag_config.autograder_dir,
         "otter_env_name": OTTER_ENV_NAME,
-        "miniconda_install_url": MINICONDA_INSTALL_URL,
-        "ottr_branch": OTTR_BRANCH,
-        "channel_priority_strict": ag_config.channel_priority_strict,
-        "python_version": python_version or DEFAULT_PYTHON_VERSION,
+        "ottr_version": OTTR_VERSION,
+        "channel_priority_strict": channel_priority_strict,
+        "has_r_requirements": False,
     }
 
     if plugin_collection is None:
         plugin_collection = PluginCollection(otter_config.get("plugins", []), None, {})
 
     else:
         plugin_collection.add_new_plugins(otter_config.get("plugins", []))
 
     plugin_collection.run("during_generate", otter_config, assignment)
 
     # open requirements if it exists
+    extra_requirements, r_requirements = [], None
     with load_default_file(requirements, lang_config["requirements_filename"], 
                            default_disabled=no_requirements,) as reqs:
-        template_context["other_requirements"] = reqs if reqs is not None else ""
-
-    template_context["overwrite_requirements"] = overwrite_requirements
+        if reqs is not None:
+            if ag_config.lang == "python":
+                extra_requirements = [l for l in reqs.split("\n") if l.strip() and not l.strip().startswith("#")]
+            elif ag_config.lang == "r":
+                r_requirements = reqs
+                template_context["has_r_requirements"] = True
 
     # open environment if it exists
-    # unlike requirements.txt, we will always overwrite, not append by default
+    user_environment = None
     with load_default_file(environment, "environment.yml", default_disabled=no_environment) as env_contents:
         template_context["other_environment"] = env_contents
         if env_contents is not None:
-            data = yaml.safe_load(env_contents)
-            data['name'] = template_context["otter_env_name"]
-            template_context["other_environment"] = yaml.safe_dump(data, default_flow_style=False)
+            user_environment = yaml.safe_load(env_contents)
+
+    conda_environment = CondaEnvironment(
+        python_version or DEFAULT_PYTHON_VERSION,
+        ag_config.lang == "r",
+        extra_requirements,
+        overwrite_requirements,
+        user_environment,
+    )
 
     rendered = {}
     for fn, template in templates.items():
         rendered[fn] = template.render(**template_context)
 
     if os.path.exists(output_path):
         os.remove(output_path)
@@ -179,26 +272,28 @@
             zf.writestr(fn, contents)
 
         arc_test_dir = "tests"
         pattern = lang_config["test_file_pattern"]
         for file in glob(os.path.join(tests_dir, pattern)):
             zf.write(file, arcname=os.path.join(arc_test_dir, os.path.basename(file)))
 
+        if r_requirements is not None:
+            zf.writestr("requirements.r", r_requirements)
+
+        zf.writestr("environment.yml", conda_environment.to_str())
+
         zf.writestr("otter_config.json", json.dumps(otter_config, indent=2))
 
-        # copy files into tmp
+        # copy files into zip file
         if len(files) > 0:
             for file in files:
                 full_fp = os.path.abspath(file)
                 if os.getcwd() not in full_fp:
                     raise ValueError(f"{file} is not in the working directory")
 
                 relative_fp = pathlib.Path(full_fp).relative_to(pathlib.Path(os.getcwd()))
                 if os.path.isfile(full_fp):
                     zf.write(file, arcname=os.path.join("files", relative_fp))
                 elif os.path.isdir(full_fp):
                     zip_folder(zf, full_fp, prefix=os.path.join("files", os.path.split(relative_fp)[0]))
                 else:
                     raise ValueError(f"Could not find file or directory '{full_fp}'")
-
-    if assignment is not None:
-        assignment._otter_config = otter_config
```

### Comparing `otter-grader-4.4.1/otter/generate/token.py` & `otter-grader-5.0.0/otter/generate/token.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/grade/Dockerfile` & `otter-grader-5.0.0/otter/grade/Dockerfile`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,26 @@
-ARG BASE_IMAGE=ucbdsinfra/otter-grader
+ARG BASE_IMAGE=ubuntu:22.04
+
 FROM ${BASE_IMAGE}
-RUN apt-get update && apt-get install -y curl unzip dos2unix && apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
-RUN mkdir -p /autograder/source
-ARG BASE_IMAGE
+
+RUN apt-get update && \
+    apt-get install -y curl unzip dos2unix && \
+    apt-get clean && \
+    rm -rf /var/lib/apt/lists/* /var/tmp/*
+
+RUN mkdir -p /autograder/source && \
+    mkdir -p /autograder/submission && \
+    mkdir -p /autograder/results
+
 ENV BASE_IMAGE=$BASE_IMAGE
 ADD run_autograder /autograder/run_autograder
 ADD setup.sh environment.yml requirements.* /autograder/source/
+
 RUN dos2unix /autograder/run_autograder /autograder/source/setup.sh && \
     chmod +x /autograder/run_autograder && \
-    apt-get update && bash /autograder/source/setup.sh && apt-get clean && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* && \
-    mkdir -p /autograder/submission && \
-    mkdir -p /autograder/results
+    apt-get update && bash /autograder/source/setup.sh && \
+    apt-get clean && \
+    rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/*
+
 ADD otter_config.json run_otter.py /autograder/source/
 ADD files* /autograder/source/files/
 ADD tests /autograder/source/tests/
```

### Comparing `otter-grader-4.4.1/otter/grade/containers.py` & `otter-grader-5.0.0/otter/grade/containers.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,164 +1,171 @@
 """Docker container management for Otter Grade"""
 
-import glob
+import json
 import os
 import pandas as pd
-import pickle
+import pathlib
 import pkg_resources
 import shutil
 import tempfile
 import zipfile
 
 from concurrent.futures import ThreadPoolExecutor, wait
 from python_on_whales import docker
 from textwrap import indent
-from typing import Optional
+from typing import List, Optional
 
-from .utils import generate_hash, OTTER_DOCKER_IMAGE_TAG
+from .utils import OTTER_DOCKER_IMAGE_NAME
 
+from ..run.run_autograder.autograder_config import AutograderConfig
 from ..utils import loggers
 
 
 LOGGER = loggers.get_logger(__name__)
 
 
-def build_image(zip_path, base_image, tag):
+def build_image(ag_zip_path: str, base_image: str, tag: str, config: AutograderConfig):
     """
     Creates a grading image based on the autograder zip file and attaches a tag.
 
     Args:
-        zip_path (``str``): path to the autograder zip file
+        ag_zip_path (``str``): path to the autograder zip file
         base_image (``str``): base Docker image to build from
         tag (``str``): tag to be added when creating the image
+        config (``otter.run.run_autograder.autograder_config.AutograderConfig``): config overrides
+            for the autograder
 
     Returns:
         ``str``: the tag of the newly-build Docker image
     """
-    image = OTTER_DOCKER_IMAGE_TAG + ":" + tag
-    dockerfile = pkg_resources.resource_filename(__name__, "Dockerfile")
+    image = OTTER_DOCKER_IMAGE_NAME + ":" + tag
+    dockerfile_path = pkg_resources.resource_filename(__name__, "Dockerfile")
 
-    if not docker.image.exists(image):
-        LOGGER.info(f"Building new image using {base_image} as base image")
+    LOGGER.info(f"Building image using {base_image} as base image")
+
+    with tempfile.TemporaryDirectory() as temp_dir:
+        with zipfile.ZipFile(ag_zip_path, 'r') as zip_ref:
+            zip_ref.extractall(temp_dir)
+
+        # Update the otter_config.json file from the autograder zip with the provided config
+        # overrides.
+        config_path = pathlib.Path(temp_dir) / "otter_config.json"
+        old_config = AutograderConfig()
+        if config_path.exists():
+            old_config = AutograderConfig(json.loads(config_path.read_text("utf-8")))
+
+        old_config.update(config.get_user_config())
+        config_path.write_text(json.dumps(old_config.get_user_config()))
+
+        docker.build(
+            temp_dir,
+            build_args={"BASE_IMAGE": base_image},
+            tags=[image],
+            file=dockerfile_path,
+            load=True,
+        )
 
-        tmp_dir = tempfile.mkdtemp()
-        with zipfile.ZipFile(zip_path, 'r') as zip_ref:
-            zip_ref.extractall(tmp_dir)
-
-        docker.build(tmp_dir, build_args={
-            "BASE_IMAGE": base_image
-        }, tags=[image], file=dockerfile, load=True)
-        shutil.rmtree(tmp_dir)
     return image
 
 
-def launch_grade(zip_path, submissions_dir, num_containers=None, ext="ipynb", no_kill=False, 
-                 output_path="./", zips=False, image="ucbdsinfra/otter-grader", pdfs=False, 
-                 timeout=None, network=True):
-    """
-    Grades notebooks in parallel Docker containers
-
-    This function runs ``num_containers`` Docker containers in parallel to grade the student submissions
-    in ``submissions_dir`` using the autograder configuration file at ``zip_path``. It can additionally 
-    generate PDFs for the parts of the assignment needing manual grading.
+def launch_containers(
+    ag_zip_path: str,
+    submission_paths: List[str],
+    num_containers: int,
+    base_image: str,
+    tag: str,
+    config: AutograderConfig,
+    **kwargs,
+):
+    """
+    Grade submissions in parallel Docker containers.
+
+    This function runs ``num_containers`` Docker containers in parallel to grade the student
+    submissions in ``submissions_dir`` using the autograder configuration file at ``ag_zip_path``. 
+    If indicated, it copies the PDFs generated of the submissions out of their containers.
 
     Args:
-        zip_path(``str``): path to zip file used to set up container
-        submissions_dir (``str``): path to directory of student submissions to be graded
-        num_containers (``int``, optional): The number of parallel containers that will be run
-        ext (``str``, optional): the submission file extension for globbing
-        no_kill (``bool``, optional): whether the grading containers should be kept running after
-            grading finishes
-        output_path (``str``, optional): path at which to write grades CSVs copied from the container
-        zips (``bool``, optional): whether the submissions are zip files formatted from ``Notebook.export``
-        image (``str``, optional): a base image to use for building Docker images
-        pdfs (``bool``, optional): whether to copy PDFs out of the containers
-        timeout (``int``): timeout in seconds for each container
-        network (``bool``): whether to enable networking in the containers
+        ag_zip_path (``str``): path to zip file used to set up container
+        submission_paths (``str``): paths of submissions to be graded
+        num_containers (``int``): number of containers to run in parallel
+        base_image (``str``): the name of a base image to use for building Docker images
+        tag (``str``): a tag to use for the ``otter-grade`` image created for this assignment
+        config (``otter.run.run_autograder.autograder_config.AutograderConfig``): config overrides
+            for the autograder
+        **kwargs: additional kwargs passed to ``grade_submission``
 
     Returns:
-        ``list`` of ``pandas.core.frame.DataFrame``: the grades returned by each container spawned during
-            grading
+        ``list[pandas.core.frame.DataFrame]``: the grades returned by each container spawned
+            during grading
     """
-    if not num_containers:
-        num_containers = 4
-
     pool = ThreadPoolExecutor(num_containers)
     futures = []
-    img = build_image(zip_path, image, generate_hash(zip_path, image))
+    image = build_image(ag_zip_path, base_image, tag, config)
 
-    if zips:
-        pattern = "*.zip"
-    else:
-        pattern = f"*.{ext}"
-
-    submissions = glob.glob(os.path.join(submissions_dir, pattern))
-    pdf_dir = os.path.join(output_path, "submission_pdfs")
-
-    for subm_path in submissions:
-        futures += [
-            pool.submit(
-                grade_assignments,
-                submission_path=subm_path,
-                image=img,
-                no_kill=no_kill,
-                pdf_dir=pdf_dir,
-                pdfs=pdfs,
-                timeout=timeout,
-                network=network,
-            )
-        ]
+    for subm_path in submission_paths:
+        futures += [pool.submit(
+            grade_submission,
+            submission_path=subm_path,
+            image=image,
+            # config=config,
+            **kwargs,
+        )]
 
     # stop execution while containers are running
     finished_futures = wait(futures)
 
     # return list of dataframes
     return [df.result() for df in finished_futures[0]]
 
 
-def grade_assignments(submission_path, image, no_kill=False, pdf_dir=None, pdfs=False, 
-                      timeout: Optional[int] = None, network=True):
+def grade_submission(
+    submission_path: str,
+    image: str,
+    no_kill: bool = False,
+    pdf_dir: Optional[str] = None,
+    timeout: Optional[int] = None,
+    network: bool = True,
+):
     """
-    Grades multiple submissions in a directory using a single docker container. If no PDF assignment is
-    wanted, set all three PDF params (``unfiltered_pdfs``, ``tag_filter``, and ``html_filter``) to ``False``.
+    Grade a submission in a Docker container.
 
     Args:
         submission_path (``str``): path to the submission to be graded
         image (``str``): a Docker image tag to be used for grading environment
-        no_kill (``bool``, optional): whether the grading containers should be kept running after
+        no_kill (``bool``): whether the grading containers should be kept running after
             grading finishes
-        pdf_dir (``str``, optional): directory in which to put notebook PDFs, if applicable
-        pdfs (``bool``, optional): whether to copy PDFs out of the containers
-        timeout (``int``): timeout in seconds for each container
+        pdf_dir (``str``, optional): a directory in which to put the notebook PDF, if applicable
+        timeout (``int``, optional): timeout in seconds for each container
         network (``bool``): whether to enable networking in the containers
 
     Returns:
         ``pandas.core.frame.DataFrame``: A dataframe of file to grades information
     """
+    import dill
+
     temp_subm_file, temp_subm_path = tempfile.mkstemp()
     shutil.copyfile(submission_path, temp_subm_path)
 
     results_file, results_path = tempfile.mkstemp(suffix=".pkl")
     pdf_path = None
-    if pdfs:
+    if pdf_dir:
         pdf_file, pdf_path = tempfile.mkstemp(suffix=".pdf")
 
     try:
         nb_basename = os.path.basename(submission_path)
         nb_name = os.path.splitext(nb_basename)[0]
 
         volumes = [
             (temp_subm_path, f"/autograder/submission/{nb_basename}"),
             (results_path, "/autograder/results/results.pkl")
         ]
-        if pdfs:
+        if pdf_dir:
             volumes.append((pdf_path, f"/autograder/submission/{nb_name}.pdf"))
 
         args = {}
-
         if network is not None and not network:
             args['networks'] = 'none'
 
         container = docker.container.create(image, command=["/autograder/run_autograder"], **args)
 
         for local_path, container_path in volumes:
             docker.container.copy(local_path, (container, container_path))
@@ -195,32 +202,31 @@
         for local_path, container_path in volumes:
             docker.container.copy((container, container_path), local_path)
 
         if not no_kill:
             container.remove()
 
         if exit != 0:
-            raise Exception(f"Executing '{submission_path}' in docker container failed! Exit code: {exit}")
+            raise Exception(
+                f"Executing '{submission_path}' in docker container failed! Exit code: {exit}")
 
         with open(results_path, "rb") as f:
-            scores = pickle.load(f)
+            scores = dill.load(f)
 
         scores_dict = scores.to_dict()
         scores_dict["percent_correct"] = scores.total / scores.possible
 
         scores_dict = {t: [scores_dict[t]["score"]] if type(scores_dict[t]) == dict else scores_dict[t] for t in scores_dict}
-        scores_dict["file"] = os.path.split(submission_path)[1]
+        scores_dict["file"] = submission_path
         df = pd.DataFrame(scores_dict)
 
-        if pdfs:
+        if pdf_dir:
             os.makedirs(pdf_dir, exist_ok=True)
 
             local_pdf_path = os.path.join(pdf_dir, f"{nb_name}.pdf")
             shutil.copy(pdf_path, local_pdf_path)
 
     finally:
         os.remove(results_path)
         os.remove(temp_subm_path)
-        if pdfs:
-            os.remove(pdf_path)
 
     return df
```

### Comparing `otter-grader-4.4.1/otter/plugins/__init__.py` & `otter-grader-5.0.0/otter/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/plugins/abstract_plugin.py` & `otter-grader-5.0.0/otter/plugins/abstract_plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -18,15 +18,14 @@
     - ``during_assign``: run during Otter Assign after output directories are written
     - ``during_generate``: run during Otter Generate while all files are in-memory and before the
       the `tmp` directory is created
     - ``from_notebook``: run as students as they work through the notebook; see ``Notebook.run_plugin``
     - ``notebook_export``: run by ``Notebook.export`` for adding files to the export zip file
     - ``before_grading``: run before the submission is executed for altering configurations
     - ``before_execution``: run before the submission is executed for altering the submission
-    - ``after_execution``: run after the submission is executed
     - ``after_grading``: run after all tests are run and scores are assigned
     - ``generate_report``: run after results are written
 
     See the docstring for the default implementation of each method for more information, including
     arguments and return values. If plugin has no actions for any event above, that method should raise
     ``otter.plugins.PluginEventNotSupportedException``. (This is the default behavior of this ABC, so
     inheriting from this class will do this for you for any methods you don't overwrite.)
@@ -165,28 +164,14 @@
             ``nbformat.NotebookNode`` or ``str``: the altered submission to be executed
 
         Raises:
             ``PluginEventNotSupportedException``: if the event is not supported by this plugin
         """
         raise PluginEventNotSupportedException()
 
-    def after_execution(self, global_env):
-        """
-        Plugin event run after the execution of the submission which can modify the resulting global
-        environment.
-
-        Args:
-            global_env (``dict``): the environment resulting from the execution of the students' code;
-                see ``otter.execute``
-
-        Raises:
-            ``PluginEventNotSupportedException``: if the event is not supported by this plugin
-        """
-        raise PluginEventNotSupportedException()
-
     def after_grading(self, results):
         """
         Plugin event run after all tests are run on the resulting environment that gets passed the 
         ``otter.test_files.GradingResults`` object that stores the grading results for each test case.
 
         Args:
             results (``otter.test_files.GradingResults``): the results of all test cases
```

### Comparing `otter-grader-4.4.1/otter/plugins/builtin/gmail_notifications/__init__.py` & `otter-grader-5.0.0/otter/plugins/builtin/gmail_notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py` & `otter-grader-5.0.0/otter/plugins/builtin/gmail_notifications/bin/gmail_oauth2.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/plugins/builtin/grade_override.py` & `otter-grader-5.0.0/otter/plugins/builtin/grade_override.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/plugins/builtin/rate_limiting.py` & `otter-grader-5.0.0/otter/plugins/builtin/rate_limiting.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/run/__init__.py` & `otter-grader-5.0.0/otter/run/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/run/run_autograder/__init__.py` & `otter-grader-5.0.0/otter/run/run_autograder/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/run/run_autograder/autograder_config.py` & `otter-grader-5.0.0/otter/run/run_autograder/autograder_config.py`

 * *Files 5% similar despite different names*

```diff
@@ -100,16 +100,16 @@
     lang = fica.Key(
         description="the language of the assignment; one of {'python', 'r'}",
         default="python",
         validator=fica.validators.choice(["python", "r"]),
     )
 
     miniconda_path = fica.Key(
-        description="the path to the miniconda install directory",
-        default="/root/miniconda3",
+        description="the path to the mamba install directory",
+        default="/root/mambaforge",
     )
 
     plugins = fica.Key(
         description="a list of plugin names and configuration details for grading",
         default=[],
     )
 
@@ -135,19 +135,14 @@
 
     log_level = fica.Key(
         description="a log level for logging messages; any value suitable for " \
             "``logging.Logger.setLevel``",
         default=None,
     )
 
-    channel_priority_strict = fica.Key(
-        description="whether to set conda's channel_priority config to strict in the setup.sh file",
-        default=True,
-    )
-
     assignment_name = fica.Key(
         description="a name for the assignment to ensure that students submit to the correct " \
             "autograder",
         default=None,
     )
 
     warn_missing_pdf = fica.Key(
@@ -157,7 +152,13 @@
     )
 
     force_public_test_summary = fica.Key(
         description="whether to show a summary of public test case results when show_hidden is " \
             "true",
         default=True,
     )
+
+    submit_blank_pdf_on_export_failure = fica.Key(
+        description="whether to submit a blank PDF to the manual-grading Gradescope assignment " \
+            "if a PDF cannot be generated from the submission",
+        default=False,
+    )
```

### Comparing `otter-grader-4.4.1/otter/run/run_autograder/runners/__init__.py` & `otter-grader-5.0.0/otter/run/run_autograder/runners/__init__.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/run/run_autograder/runners/abstract_runner.py` & `otter-grader-5.0.0/otter/run/run_autograder/runners/abstract_runner.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Abstract runner class for the autograder"""
 
 import json
 import os
 import shutil
+import tempfile
 
 from abc import ABC, abstractmethod
 
 from ..autograder_config import AutograderConfig
-from ..utils import OtterRuntimeError
+from ..utils import OtterRuntimeError, write_blank_page_to_stare_at_before_you
 
 from ....utils import NOTEBOOK_METADATA_KEY
 
 
 class AbstractLanguageRunner(ABC):
     """
     A class defining the logic of running the autograder and generating grading results.
@@ -120,37 +121,54 @@
             scores (``otter.test_files.GradingResults``): the grading results (so an error can be
                 appended if needed)
         """
         try:
             pdf_path = self.write_pdf(submission_path)
 
             if submit:
-                # get student email
-                with open("../submission_metadata.json", encoding="utf-8") as f:
-                    metadata = json.load(f)
-
-                student_emails = []
-                for user in metadata["users"]:
-                    student_emails.append(user["email"])
-
-                for student_email in student_emails:
-                    client.upload_pdf_submission(
-                        self.ag_config.course_id,
-                        self.ag_config.assignment_id,
-                        student_email,
-                        pdf_path,
-                    )
-
-                print("\n\nSuccessfully uploaded submissions for: {}".format(
-                    ", ".join(student_emails)))
+                self.submit_pdf(client, pdf_path)
 
         except Exception as e:
             print(f"\n\nError encountered while generating and submitting PDF:\n{e}")
             scores.set_pdf_error(e)
 
+            if self.ag_config.submit_blank_pdf_on_export_failure and submit:
+                print("\nUploading a blank PDF due to export failure")
+                with tempfile.NamedTemporaryFile(suffix=".pdf") as ntf:
+                    write_blank_page_to_stare_at_before_you(ntf.name)
+                    self.submit_pdf(client, ntf.name)
+
+    def submit_pdf(self, client, pdf_path):
+        """
+        Upload the PDF at ``pdf_path`` to the Gradescope assignment specified in the config. Does
+        not check whether the assignment configuration is valid.
+
+        Args:
+            client (``otter.generate.token.APIClient``): the Gradescope client
+            pdf_path (``str``): path to the PDF file to upload
+        """
+        # get student email
+        with open("../submission_metadata.json", encoding="utf-8") as f:
+            metadata = json.load(f)
+
+        student_emails = []
+        for user in metadata["users"]:
+            student_emails.append(user["email"])
+
+        for student_email in student_emails:
+            client.upload_pdf_submission(
+                self.ag_config.course_id,
+                self.ag_config.assignment_id,
+                student_email,
+                pdf_path,
+            )
+
+        print("\n\nSuccessfully uploaded submissions for: {}".format(
+            ", ".join(student_emails)))
+
     @abstractmethod
     def validate_submission(self, submission_path):
         """
         Validate the submission, raising an error/warning if appropriate.
 
         This method should be invoked as part of the implementation of another abstract method
         (either ``resolve_submission_path`` or ``run``).
```

### Comparing `otter-grader-4.4.1/otter/run/run_autograder/runners/python_runner.py` & `otter-grader-5.0.0/otter/run/run_autograder/runners/python_runner.py`

 * *Files 3% similar despite different names*

```diff
@@ -61,15 +61,15 @@
                 raise OtterRuntimeError("No gradable files found in submission")
 
         return subm_path
 
     def write_pdf(self, nb_path):
         pdf_path = os.path.splitext(nb_path)[0] + ".pdf"
         export_notebook(
-            nb_path, dest=pdf_path, filtering=self.ag_config.filtering, 
+            nb_path, dest=pdf_path, filtering=self.ag_config.filtering,
             pagebreaks=self.ag_config.pagebreaks, exporter_type="latex")
 
         return pdf_path
 
     def run(self):
         os.environ["PATH"] = f"{self.ag_config.miniconda_path}/bin:" + os.environ.get("PATH")
 
@@ -119,20 +119,19 @@
             else:
                 if self.ag_config.grade_from_log:
                     raise OtterRuntimeError("Grade from log indicated but log not found")
 
                 log = None
 
             scores = grade_notebook(
-                subm_path, 
-                tests_glob = glob("./tests/*.py"), 
-                name = "submission", 
-                cwd = os.getcwd(), 
+                subm_path,
+                tests_glob = glob("./tests/*.py"),
+                cwd = os.getcwd(),
                 test_dir = "./tests",
-                ignore_errors = not self.ag_config.debug, 
+                ignore_errors = not self.ag_config.debug,
                 seed = self.ag_config.seed,
                 seed_variable = self.ag_config.seed_variable,
                 log = log if self.ag_config.grade_from_log else None,
                 variables = self.ag_config.serialized_variables,
                 plugin_collection = plugin_collection,
                 script = os.path.splitext(subm_path)[1] == ".py",
             )
@@ -156,10 +155,10 @@
 
             if generate_pdf:
                 self.write_and_maybe_submit_pdf(client, subm_path, has_token, scores)
 
             if plugin_collection:
                 report = plugin_collection.generate_report()
                 if report.strip():
-                    print("\n\n" + report)        
+                    print("\n\n" + report)
 
         return scores
```

### Comparing `otter-grader-4.4.1/otter/run/run_autograder/runners/r_runner.py` & `otter-grader-5.0.0/otter/run/run_autograder/runners/r_runner.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/test_files/__init__.py` & `otter-grader-5.0.0/otter/test_files/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,21 +79,22 @@
     Attributes:
         results (``dict``): maps test names to ``GradingTestCaseResult`` named tuples containing the 
             test result information
         output (``str``): a string to include in the output field for Gradescope
         all_hidden (``bool``): whether all results should be hidden from the student on Gradescope
         tests (``list`` of ``str``): list of test names according to the keys of ``results``
     """
-    def __init__(self, test_files):
+    def __init__(self, test_files, notebook=None):
         self._plugin_data = {}
         self.results = {tf.name: tf for tf in test_files}
         # self.results = {}
         self.output = None
         self.all_hidden = False
         self.pdf_error = None
+        self.notebook = notebook
 
     def __repr__(self):
         return self.summary()
 
     @classmethod
     def from_ottr_json(cls, ottr_output):
         """
```

### Comparing `otter-grader-4.4.1/otter/test_files/abstract_test.py` & `otter-grader-5.0.0/otter/test_files/abstract_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/test_files/exception_test.py` & `otter-grader-5.0.0/otter/test_files/exception_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/test_files/metadata_test.py` & `otter-grader-5.0.0/otter/test_files/metadata_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/test_files/ok_test.py` & `otter-grader-5.0.0/otter/test_files/ok_test.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/otter/utils.py` & `otter-grader-5.0.0/otter/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,39 +5,30 @@
 import os
 import pathlib
 import random
 import re
 import string
 import shutil
 import tempfile
+import yaml
 
-from collections.abc import Mapping
 from contextlib import contextmanager, redirect_stdout
 from functools import lru_cache
 from IPython import get_ipython
 
 
 # TODO: migrate other uses to this constant
 NBFORMAT_VERSION = 4
 """the version of the Jupyter notebook format to use"""
 
 NOTEBOOK_METADATA_KEY = "otter"
 """the key used for all Otter metadata added to a notebook"""
 
 
 @contextmanager
-def block_print():
-    """
-    Context manager that disables printing to stdout
-    """
-    with open(os.devnull, "w") as f, redirect_stdout(f):
-        yield
-
-
-@contextmanager
 def hide_outputs():
     """
     Context manager for hiding outputs from ``display()`` calls. IPython handles matplotlib outputs 
     specially, so those are supressed too.
     """
     ipy = get_ipython()
     if ipy is None:
@@ -196,96 +187,14 @@
 
     if ret_str:
         return out
 
     print(out, **kwargs)
 
 
-# TODO: remove when Otter Assign format v0 is removed
-def convert_config_description_dict(configs, for_docs=False):
-    """
-    Recursively converts a documented list of dictionary configurations into a dictionary with the 
-    default values loaded.
-
-    Expects a list of the form:
-
-    .. code-block:: python
-
-        [
-            {
-                "key": "config_name",
-                "description": "a description of the config for documentation",
-                "default": True,  # the default config value
-            },
-            {
-                "key": "required_config_name",
-                "description": "a description of the config for documentation",
-                "required": True,  # indicates that this must be user-specified and has no default
-            },
-            {
-                "key": "nested_config_name",
-                "description": "a description of the config for documentation",
-                "default": None,
-                "subkeys": [  # note that a list is used for nested dict configs
-                    {
-                        "key": "subconfig",
-                        "description": "a nested key",
-                        "default": None,
-                    }
-                ],
-            },
-        ]
-
-    The list above gets converted to a dictionary mapping each ``key`` to each ``default``:
-
-    .. code-block:: python
-
-        {
-            "config_name": True,
-            "nested_config_name": None,
-        }
-
-    If ``for_docs`` is true, then any specified subkeys are set as the mapped value in the dictionary,
-    and if the config is required, its default is set to ``None``.
-
-    .. code-block:: python
-
-        {
-            "config_name": True,
-            "required_config_name": None,
-            "nested_config_name": {
-                "subconfig": None,
-            },
-        }
-
-    Any configurations with ``default`` unspecified have their default value set to ``None``. Any
-    configurations marked with ``"required": True`` are not included in the output dict (so that
-    they raise a ``KeyError`` if unspecified).
-
-    Args:
-        configs (``list[dict[str,object]]``): the configurations with the structure defined above
-
-    Returns:
-        ``dict[str,object]``: a dictionary mapping keys to default values
-    """
-    res = {}
-    for d in configs:
-        default = d.get("default")
-        subkeys = d.get("subkeys")
-        if isinstance(default, list) and len(default) > 0 and \
-                all(isinstance(e, dict) for e in default):
-            default = convert_config_description_dict(default)
-        elif for_docs and isinstance(subkeys, list) and len(subkeys) > 0 and \
-                all(isinstance(e, dict) for e in subkeys):
-            default = convert_config_description_dict(subkeys)
-        if not d.get("required", False) or for_docs:
-            res[d["key"]] = default
-    return res
-
-
 def assert_path_exists(path_tuples):
     """
     Ensure that a series of file paths exist and are of a specific type, or raise a ``ValueError``.
 
     Elements of ``path_tuples`` should be 2-tuples where the first element is a string representing 
     the file path and the second element is ``True`` if the path should be a directory, ``False`` if 
     it should be a file, and ``None`` if it doesn't matter.
@@ -434,7 +343,26 @@
     Import a module or raise an ``ImportError`` if it is unable to be imported. Return values are
     stored in an LRU cache.
     """
     try:
         return importlib.import_module(module)
     except:
         raise ImportError(f"Could not import required module: {module}")
+
+
+class _CorrectIndentationDumper(yaml.Dumper):
+    def increase_indent(self, flow=False, *args, **kwargs):
+        return super().increase_indent(flow=flow, indentless=False)
+
+
+def dump_yaml(o, **kwargs):
+    """
+    Dump an object to a YAML string using the ``_CorrectIndentationDumper`` dumper.
+
+    Args:
+        o (``object``): the object to dump
+        **kwargs: additional keyword arguments passed to ``yaml.dump``
+
+    Returns:
+        ``str``: the YAML representation of ``o``
+    """
+    return yaml.dump(o, sort_keys=False, Dumper=_CorrectIndentationDumper, **kwargs)
```

### Comparing `otter-grader-4.4.1/otter/version.py` & `otter-grader-5.0.0/otter/version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """Version and printable logo"""
 
 import sys
 
 from textwrap import dedent
 
 
-__version__ = "4.4.1"
+__version__ = "5.0.0"
 
 
 LOGO_WITH_VERSION = fr"""
   _________        __          __               
  /  _____  \    __|  |__    __|  |__               
 |  /     \  |  |__    __|  |__    __|   _______    _  _____
 | |       | |     |  |        |  |     |  ___  |  | |/ ____|
```

### Comparing `otter-grader-4.4.1/otter_grader.egg-info/PKG-INFO` & `otter-grader-5.0.0/otter_grader.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otter-grader
-Version: 4.4.1
+Version: 5.0.0
 Summary: Python and Jupyter Notebook autograder
 Home-page: https://github.com/ucbds-infra/otter-grader
 Author: Christopher Pyles
 Author-email: otter-grader@berkeley.edu
 License: BSD-3-Clause
 Description: # Otter-Grader
```

### Comparing `otter-grader-4.4.1/otter_grader.egg-info/SOURCES.txt` & `otter-grader-5.0.0/otter_grader.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 otter/check/utils.py
 otter/check/validate_export/__init__.py
 otter/check/validate_export/__main__.py
 otter/execute/__init__.py
 otter/execute/checker.py
 otter/execute/execute_log.py
 otter/execute/execute_notebook.py
+otter/execute/preprocessor.py
 otter/execute/transforms.py
 otter/export/__init__.py
 otter/export/utils.py
 otter/export/exporters/__init__.py
 otter/export/exporters/base_exporter.py
 otter/export/exporters/utils.py
 otter/export/exporters/via_html.py
@@ -75,14 +76,16 @@
 otter/export/exporters/templates/via_latex/conf.json
 otter/export/exporters/templates/via_latex/index.tex.j2
 otter/export/exporters/templates/via_latex_xecjk/conf.json
 otter/export/exporters/templates/via_latex_xecjk/index.tex.j2
 otter/generate/__init__.py
 otter/generate/token.py
 otter/generate/utils.py
+otter/generate/templates/common/run_autograder
+otter/generate/templates/common/run_otter.py
 otter/generate/templates/python/environment.yml
 otter/generate/templates/python/requirements.txt
 otter/generate/templates/python/run_autograder
 otter/generate/templates/python/run_otter.py
 otter/generate/templates/python/setup.sh
 otter/generate/templates/r/environment.yml
 otter/generate/templates/r/requirements.r
@@ -118,18 +121,36 @@
 otter/test_files/ottr_test.py
 otter_grader.egg-info/PKG-INFO
 otter_grader.egg-info/SOURCES.txt
 otter_grader.egg-info/dependency_links.txt
 otter_grader.egg-info/entry_points.txt
 otter_grader.egg-info/requires.txt
 otter_grader.egg-info/top_level.txt
+test/test_api.py
 test/test_assign.py
 test/test_check.py
+test/test_cli.py
 test/test_export.py
 test/test_grade.py
 test/test_logs.py
 test/test_notebook.py
 test/test_run.py
 test/test_utils.py
+test/test_assign/__init__.py
+test/test_assign/test_integration.py
+test/test_check/__init__.py
+test/test_check/test_cli.py
+test/test_check/test_logs.py
+test/test_check/test_notebook.py
+test/test_execute/__init__.py
+test/test_execute/test_checker.py
+test/test_execute/test_integration.py
+test/test_export/__init__.py
+test/test_export/test_integration.py
 test/test_generate/__init__.py
 test/test_generate/test_autograder.py
-test/test_generate/test_token.py
+test/test_generate/test_token.py
+test/test_generate/test_utils.py
+test/test_grade/__init__.py
+test/test_grade/test_integration.py
+test/test_run/__init__.py
+test/test_run/test_integration.py
```

### Comparing `otter-grader-4.4.1/setup.py` & `otter-grader-5.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/test/test_assign.py` & `otter-grader-5.0.0/test/test_assign.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/test/test_check.py` & `otter-grader-5.0.0/test/test_check.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/test/test_export.py` & `otter-grader-5.0.0/test/test_export.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/test/test_generate/test_autograder.py` & `otter-grader-5.0.0/test/test_generate/test_autograder.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from unittest import mock
 
 from otter.generate import main as generate
 
 from ..utils import assert_dirs_equal, TestFileManager, unzip_to_temp
 
 
-FILE_MANAGER = TestFileManager("test/test_generate/test-autograder")
+FILE_MANAGER = TestFileManager(__file__)
 OUTPUT_PATH = FILE_MANAGER.get_path("autograder.zip")
 
 
 @pytest.fixture(autouse=True)
 def cleanup_output(cleanup_enabled):
     yield
     if cleanup_enabled and os.path.exists(OUTPUT_PATH):
@@ -34,33 +34,34 @@
         no_environment = True,  # don't use the environment.yml in the root of the repo
     )
 
     with unzip_to_temp(FILE_MANAGER.get_path("autograder.zip")) as unzipped_dir:
         assert_dirs_equal(unzipped_dir, FILE_MANAGER.get_path("autograder-correct"))
 
 
-def test_autograder_with_token():
+@mock.patch("otter.generate.APIClient")
+def test_autograder_with_token(mocked_client):
     """
     Check that the correct zip file is generated when a token is specified instead of a username
     and password.
 
     This test also checks that directories are copied correctly when listed in the ``files``
     argument.
     """
     # create the zipfile
-    with mock.patch("otter.generate.APIClient") as mocked_client:
-        generate(
-            tests_dir = FILE_MANAGER.get_path("tests"),
-            output_path = OUTPUT_PATH,
-            requirements = FILE_MANAGER.get_path("requirements.txt"),
-            config = FILE_MANAGER.get_path("otter_config.json"),
-            files = [FILE_MANAGER.get_path("data")],
-            no_environment = True,  # don't use the environment.yml in the root of the repo
-        )
-        mocked_client.assert_not_called()
+    generate(
+        tests_dir = FILE_MANAGER.get_path("tests"),
+        output_path = OUTPUT_PATH,
+        requirements = FILE_MANAGER.get_path("requirements.txt"),
+        config = FILE_MANAGER.get_path("otter_config.json"),
+        files = [FILE_MANAGER.get_path("data")],
+        no_environment = True,  # don't use the environment.yml in the root of the repo
+    )
+
+    mocked_client.assert_not_called()
 
     with unzip_to_temp(FILE_MANAGER.get_path("autograder.zip")) as unzipped_dir:
         assert_dirs_equal(unzipped_dir, FILE_MANAGER.get_path("autograder-token-correct"))
 
 
 def test_custom_env():
     """
@@ -85,11 +86,30 @@
     """
     # create the zipfile
     generate(
         tests_dir = FILE_MANAGER.get_path("tests"),
         output_path = OUTPUT_PATH,
         config = FILE_MANAGER.get_path("r_otter_config.json"),
         no_environment = True,
+        channel_priority_strict = False,
     )
 
     with unzip_to_temp(FILE_MANAGER.get_path("autograder.zip")) as unzipped_dir:
         assert_dirs_equal(unzipped_dir, FILE_MANAGER.get_path("autograder-r-correct"))
+
+
+def test_r_with_requirements():
+    """
+    Check that the R autograder configuration with a requirements file is generated correctly.
+    """
+    # create the zipfile
+    generate(
+        tests_dir = FILE_MANAGER.get_path("tests"),
+        output_path = OUTPUT_PATH,
+        config = FILE_MANAGER.get_path("r_otter_config.json"),
+        requirements = FILE_MANAGER.get_path("requirements.r"),
+        no_environment = True,
+        channel_priority_strict = False,
+    )
+
+    with unzip_to_temp(FILE_MANAGER.get_path("autograder.zip")) as unzipped_dir:
+        assert_dirs_equal(unzipped_dir, FILE_MANAGER.get_path("autograder-r-requirements-correct"))
```

### Comparing `otter-grader-4.4.1/test/test_generate/test_token.py` & `otter-grader-5.0.0/test/test_generate/test_token.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/test/test_grade.py` & `otter-grader-5.0.0/test/test_grade.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/test/test_logs.py` & `otter-grader-5.0.0/test/test_logs.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/test/test_notebook.py` & `otter-grader-5.0.0/test/test_notebook.py`

 * *Files identical despite different names*

### Comparing `otter-grader-4.4.1/test/test_run.py` & `otter-grader-5.0.0/test/test_run.py`

 * *Files identical despite different names*

