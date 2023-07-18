# Comparing `tmp/onefuzz-8.4.0.tar.gz` & `tmp/onefuzz-8.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\onefuzz-8.4.0.tar", last modified: Mon Jun 26 18:58:59 2023, max compression
+gzip compressed data, was "dist\onefuzz-8.5.0.tar", last modified: Mon Jul 17 15:58:15 2023, max compression
```

## Comparing `onefuzz-8.4.0.tar` & `onefuzz-8.5.0.tar`

### file list

```diff
@@ -1,87 +1,88 @@
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:59.000000 onefuzz-8.4.0/
--rw-rw-rw-   0        0        0     1162 2023-06-26 18:58:16.000000 onefuzz-8.4.0/LICENSE
--rw-rw-rw-   0        0        0      162 2023-06-26 18:58:16.000000 onefuzz-8.4.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2335 2023-06-26 18:58:59.000000 onefuzz-8.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1742 2023-06-26 18:58:16.000000 onefuzz-8.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/examples/
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/examples/azure-functions-example/
--rw-rw-rw-   0        0        0      297 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/azure-functions-example/README.md
--rw-rw-rw-   0        0        0      141 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/azure-functions-example/host.json
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/examples/azure-functions-example/info/
--rw-rw-rw-   0        0        0      391 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/azure-functions-example/info/__init__.py
--rw-rw-rw-   0        0        0      319 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/azure-functions-example/info/function.json
--rw-rw-rw-   0        0        0       57 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/azure-functions-example/requirements.txt
--rw-rw-rw-   0        0        0     7557 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/domato.py
--rw-rw-rw-   0        0        0      773 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/get-running.py
--rw-rw-rw-   0        0        0     4649 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/honggfuzz.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/examples/llvm-source-coverage/
--rw-rw-rw-   0        0        0       41 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/.gitignore
--rw-rw-rw-   0        0        0     7347 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/README.md
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/examples/llvm-source-coverage/inputs/
--rw-rw-rw-   0        0        0        4 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/inputs/input.txt
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/examples/llvm-source-coverage/setup/
--rw-rw-rw-   0        0        0      398 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/setup/Makefile
--rw-rw-rw-   0        0        0     1556 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/setup/simple.c
--rw-rw-rw-   0        0        0     3277 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py
--rw-rw-rw-   0        0        0     2963 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/source-coverage.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/examples/llvm-source-coverage/tools/
--rw-rw-rw-   0        0        0     1177 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/llvm-source-coverage/tools/source-coverage.sh
--rw-rw-rw-   0        0        0     2800 2023-06-26 18:58:16.000000 onefuzz-8.4.0/examples/oss-fuzz-target.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/extra/
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/extra/pyinstaller/
--rw-rw-rw-   0        0        0      200 2023-06-26 18:58:16.000000 onefuzz-8.4.0/extra/pyinstaller/hook-onefuzz.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz/
--rw-rw-rw-   0        0        0      129 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/__init__.py
--rw-rw-rw-   0        0        0      431 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/__main__.py
--rw-rw-rw-   0        0        0      126 2023-06-26 18:58:17.000000 onefuzz-8.4.0/onefuzz/__version__.py
--rw-rw-rw-   0        0        0    68993 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/api.py
--rw-rw-rw-   0        0        0     1059 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/azcopy.py
--rw-rw-rw-   0        0        0     2982 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/azure_identity_credential_adapter.py
--rw-rw-rw-   0        0        0    22112 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/backend.py
--rw-rw-rw-   0        0        0    20501 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/cli.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz/data/
--rw-rw-rw-   0        0        0     1232 2023-06-26 18:58:57.000000 onefuzz-8.4.0/onefuzz/data/licenses.json
--rw-rw-rw-   0        0        0     1004 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/data/privacy.txt
--rw-rw-rw-   0        0        0    31463 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/debug.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz/job_templates/
--rw-rw-rw-   0        0        0        0 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/job_templates/__init__.py
--rw-rw-rw-   0        0        0     4095 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/job_templates/builder.py
--rw-rw-rw-   0        0        0     1723 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/job_templates/cache.py
--rw-rw-rw-   0        0        0     6161 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/job_templates/handlers.py
--rw-rw-rw-   0        0        0     3596 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/job_templates/job_monitor.py
--rw-rw-rw-   0        0        0     3159 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/job_templates/main.py
--rw-rw-rw-   0        0        0     1851 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/job_templates/manage.py
--rw-rw-rw-   0        0        0     1682 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/rdp.py
--rw-rw-rw-   0        0        0     3522 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/ssh.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz/status/
--rw-rw-rw-   0        0        0        0 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/status/__init__.py
--rw-rw-rw-   0        0        0    13902 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/status/cache.py
--rw-rw-rw-   0        0        0     5152 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/status/cmd.py
--rw-rw-rw-   0        0        0      905 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/status/raw.py
--rw-rw-rw-   0        0        0     1856 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/status/signalr.py
--rw-rw-rw-   0        0        0     3009 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/status/top.py
--rw-rw-rw-   0        0        0     6255 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/status/top_view.py
--rw-rw-rw-   0        0        0     2882 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/template.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:59.000000 onefuzz-8.4.0/onefuzz/templates/
--rw-rw-rw-   0        0        0    10491 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/templates/__init__.py
--rw-rw-rw-   0        0        0     7003 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/templates/afl.py
--rw-rw-rw-   0        0        0    42457 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/templates/libfuzzer.py
--rw-rw-rw-   0        0        0     8812 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/templates/ossfuzz.py
--rw-rw-rw-   0        0        0     9630 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/templates/radamsa.py
--rw-rw-rw-   0        0        0    10709 2023-06-26 18:58:16.000000 onefuzz-8.4.0/onefuzz/templates/regression.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/
--rw-rw-rw-   0        0        0     2335 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1981 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       51 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      344 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-26 18:58:58.000000 onefuzz-8.4.0/onefuzz.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       44 2023-06-26 18:58:16.000000 onefuzz-8.4.0/requirements-dev.txt
--rw-rw-rw-   0        0        0      101 2023-06-26 18:58:16.000000 onefuzz-8.4.0/requirements-lint.txt
--rw-rw-rw-   0        0        0      508 2023-06-26 18:58:17.000000 onefuzz-8.4.0/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-06-26 18:58:59.000000 onefuzz-8.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1535 2023-06-26 18:58:16.000000 onefuzz-8.4.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-26 18:58:59.000000 onefuzz-8.4.0/tests/
--rw-rw-rw-   0        0        0        0 2023-06-26 18:58:16.000000 onefuzz-8.4.0/tests/__init__.py
--rw-rw-rw-   0        0        0     2728 2023-06-26 18:58:16.000000 onefuzz-8.4.0/tests/test_template_helper.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:15.000000 onefuzz-8.5.0/
+-rw-rw-rw-   0        0        0     1162 2023-07-17 15:57:13.000000 onefuzz-8.5.0/LICENSE
+-rw-rw-rw-   0        0        0      162 2023-07-17 15:57:13.000000 onefuzz-8.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2335 2023-07-17 15:58:15.000000 onefuzz-8.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1742 2023-07-17 15:57:13.000000 onefuzz-8.5.0/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/examples/
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/examples/azure-functions-example/
+-rw-rw-rw-   0        0        0      297 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/azure-functions-example/README.md
+-rw-rw-rw-   0        0        0      141 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/azure-functions-example/host.json
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/examples/azure-functions-example/info/
+-rw-rw-rw-   0        0        0      391 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/azure-functions-example/info/__init__.py
+-rw-rw-rw-   0        0        0      319 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/azure-functions-example/info/function.json
+-rw-rw-rw-   0        0        0       57 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/azure-functions-example/requirements.txt
+-rw-rw-rw-   0        0        0     7557 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/domato.py
+-rw-rw-rw-   0        0        0      773 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/get-running.py
+-rw-rw-rw-   0        0        0     4649 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/honggfuzz.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/examples/llvm-source-coverage/
+-rw-rw-rw-   0        0        0       41 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/.gitignore
+-rw-rw-rw-   0        0        0     7347 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/README.md
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/examples/llvm-source-coverage/inputs/
+-rw-rw-rw-   0        0        0        4 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/inputs/input.txt
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/examples/llvm-source-coverage/setup/
+-rw-rw-rw-   0        0        0      398 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/setup/Makefile
+-rw-rw-rw-   0        0        0     1556 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/setup/simple.c
+-rw-rw-rw-   0        0        0     3277 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py
+-rw-rw-rw-   0        0        0     2963 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/source-coverage.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/examples/llvm-source-coverage/tools/
+-rw-rw-rw-   0        0        0     1177 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/llvm-source-coverage/tools/source-coverage.sh
+-rw-rw-rw-   0        0        0     2800 2023-07-17 15:57:13.000000 onefuzz-8.5.0/examples/oss-fuzz-target.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/extra/
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/extra/pyinstaller/
+-rw-rw-rw-   0        0        0      200 2023-07-17 15:57:13.000000 onefuzz-8.5.0/extra/pyinstaller/hook-onefuzz.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz/
+-rw-rw-rw-   0        0        0      129 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/__init__.py
+-rw-rw-rw-   0        0        0      902 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/__main__.py
+-rw-rw-rw-   0        0        0      126 2023-07-17 15:57:14.000000 onefuzz-8.5.0/onefuzz/__version__.py
+-rw-rw-rw-   0        0        0    69081 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/api.py
+-rw-rw-rw-   0        0        0     1059 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/azcopy.py
+-rw-rw-rw-   0        0        0     2982 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/azure_identity_credential_adapter.py
+-rw-rw-rw-   0        0        0    22909 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/backend.py
+-rw-rw-rw-   0        0        0    20501 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/cli.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:15.000000 onefuzz-8.5.0/onefuzz/data/
+-rw-rw-rw-   0        0        0     1232 2023-07-17 15:58:13.000000 onefuzz-8.5.0/onefuzz/data/licenses.json
+-rw-rw-rw-   0        0        0     1004 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/data/privacy.txt
+-rw-rw-rw-   0        0        0    31463 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/debug.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:15.000000 onefuzz-8.5.0/onefuzz/job_templates/
+-rw-rw-rw-   0        0        0        0 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/job_templates/__init__.py
+-rw-rw-rw-   0        0        0     4095 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/job_templates/builder.py
+-rw-rw-rw-   0        0        0     1723 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/job_templates/cache.py
+-rw-rw-rw-   0        0        0     6161 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/job_templates/handlers.py
+-rw-rw-rw-   0        0        0     3596 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/job_templates/job_monitor.py
+-rw-rw-rw-   0        0        0     3159 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/job_templates/main.py
+-rw-rw-rw-   0        0        0     1851 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/job_templates/manage.py
+-rw-rw-rw-   0        0        0      768 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/opentelemetry_exporter.py
+-rw-rw-rw-   0        0        0     1682 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/rdp.py
+-rw-rw-rw-   0        0        0     3522 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/ssh.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:15.000000 onefuzz-8.5.0/onefuzz/status/
+-rw-rw-rw-   0        0        0        0 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/status/__init__.py
+-rw-rw-rw-   0        0        0    13902 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/status/cache.py
+-rw-rw-rw-   0        0        0     5152 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/status/cmd.py
+-rw-rw-rw-   0        0        0      905 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/status/raw.py
+-rw-rw-rw-   0        0        0     1856 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/status/signalr.py
+-rw-rw-rw-   0        0        0     3009 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/status/top.py
+-rw-rw-rw-   0        0        0     6255 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/status/top_view.py
+-rw-rw-rw-   0        0        0     2882 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/template.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:15.000000 onefuzz-8.5.0/onefuzz/templates/
+-rw-rw-rw-   0        0        0    10701 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/templates/__init__.py
+-rw-rw-rw-   0        0        0     7003 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/templates/afl.py
+-rw-rw-rw-   0        0        0    43054 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/templates/libfuzzer.py
+-rw-rw-rw-   0        0        0     8812 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/templates/ossfuzz.py
+-rw-rw-rw-   0        0        0     9630 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/templates/radamsa.py
+-rw-rw-rw-   0        0        0    10709 2023-07-17 15:57:13.000000 onefuzz-8.5.0/onefuzz/templates/regression.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:15.000000 onefuzz-8.5.0/onefuzz.egg-info/
+-rw-rw-rw-   0        0        0     2335 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2015 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       51 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      443 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-07-17 15:58:14.000000 onefuzz-8.5.0/onefuzz.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       44 2023-07-17 15:57:13.000000 onefuzz-8.5.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0      101 2023-07-17 15:57:13.000000 onefuzz-8.5.0/requirements-lint.txt
+-rw-rw-rw-   0        0        0      607 2023-07-17 15:57:14.000000 onefuzz-8.5.0/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-07-17 15:58:15.000000 onefuzz-8.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     1535 2023-07-17 15:57:13.000000 onefuzz-8.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-17 15:58:15.000000 onefuzz-8.5.0/tests/
+-rw-rw-rw-   0        0        0        0 2023-07-17 15:57:13.000000 onefuzz-8.5.0/tests/__init__.py
+-rw-rw-rw-   0        0        0     2728 2023-07-17 15:57:13.000000 onefuzz-8.5.0/tests/test_template_helper.py
```

### Comparing `onefuzz-8.4.0/LICENSE` & `onefuzz-8.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/PKG-INFO` & `onefuzz-8.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzz
-Version: 8.4.0
+Version: 8.5.0
 Summary: Onefuzz Client Library for Python
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # OneFuzz SDK
```

### Comparing `onefuzz-8.4.0/README.md` & `onefuzz-8.5.0/README.md`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/examples/domato.py` & `onefuzz-8.5.0/examples/domato.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/examples/get-running.py` & `onefuzz-8.5.0/examples/get-running.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/examples/honggfuzz.py` & `onefuzz-8.5.0/examples/honggfuzz.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/examples/llvm-source-coverage/README.md` & `onefuzz-8.5.0/examples/llvm-source-coverage/README.md`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/examples/llvm-source-coverage/setup/simple.c` & `onefuzz-8.5.0/examples/llvm-source-coverage/setup/simple.c`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py` & `onefuzz-8.5.0/examples/llvm-source-coverage/source-coverage-libfuzzer.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/examples/llvm-source-coverage/source-coverage.py` & `onefuzz-8.5.0/examples/llvm-source-coverage/source-coverage.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/examples/llvm-source-coverage/tools/source-coverage.sh` & `onefuzz-8.5.0/examples/llvm-source-coverage/tools/source-coverage.sh`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/examples/oss-fuzz-target.py` & `onefuzz-8.5.0/examples/oss-fuzz-target.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/api.py` & `onefuzz-8.5.0/onefuzz/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1019,14 +1019,15 @@
         vm_count: int = 1,
         preserve_existing_outputs: bool = False,
         colocate: bool = False,
         report_list: Optional[List[str]] = None,
         minimized_stack_depth: Optional[int] = None,
         module_allowlist: Optional[str] = None,
         source_allowlist: Optional[str] = None,
+        task_env: Optional[Dict[str, str]] = None,
     ) -> models.Task:
         """
         Create a task
 
         :param bool ensemble_sync_delay: Specify duration between
             syncing inputs during ensemble fuzzing (0 to disable).
         """
@@ -1096,14 +1097,15 @@
                 type=task_type,
                 wait_for_files=task_wait_for_files,
                 report_list=report_list,
                 preserve_existing_outputs=preserve_existing_outputs,
                 minimized_stack_depth=minimized_stack_depth,
                 module_allowlist=module_allowlist,
                 source_allowlist=source_allowlist,
+                task_env=task_env,
             ),
         )
 
         return self.create_with_config(config)
 
     def list(
         self,
```

### Comparing `onefuzz-8.4.0/onefuzz/azcopy.py` & `onefuzz-8.5.0/onefuzz/azcopy.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/azure_identity_credential_adapter.py` & `onefuzz-8.5.0/onefuzz/azure_identity_credential_adapter.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/backend.py` & `onefuzz-8.5.0/onefuzz/backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,14 +28,16 @@
 from urllib.parse import urlparse, urlunparse
 from uuid import UUID
 
 import msal
 import requests
 from azure.storage.blob import ContainerClient
 from onefuzztypes import responses
+from opentelemetry import context, propagate
+from opentelemetry.instrumentation.requests import RequestsInstrumentor
 from pydantic import BaseModel
 from requests import Response
 from tenacity import RetryCallState, retry
 from tenacity.retry import retry_if_exception_type
 from tenacity.stop import stop_after_attempt
 from tenacity.wait import wait_random
 
@@ -49,14 +51,15 @@
 ONEFUZZ_BASE_PATH = os.path.join(HOME_PATH, ONEFUZZ_CACHE)
 DEFAULT_CONFIG_PATH = os.path.join(ONEFUZZ_BASE_PATH, "config.json")
 DEFAULT_TOKEN_PATH = os.path.join("~", ONEFUZZ_CACHE, "access_token.json")
 REQUEST_CONNECT_TIMEOUT = 30.0
 REQUEST_READ_TIMEOUT = 120.0
 
 LOGGER = logging.getLogger("backend")
+PROPAGATOR = propagate.get_global_textmap()
 
 
 @contextlib.contextmanager
 def _temporary_umask(new_umask: int) -> Generator[None, None, None]:
     prev_umask = None
     try:
         prev_umask = os.umask(new_umask)
@@ -116,14 +119,15 @@
     def __init__(
         self,
         config: BackendConfig,
         config_path: Optional[str] = None,
         token_path: Optional[str] = None,
         client_secret: Optional[str] = None,
     ):
+        RequestsInstrumentor().instrument()
         self.config_path = os.path.expanduser(config_path or DEFAULT_CONFIG_PATH)
         self.token_path = os.path.expanduser(token_path or DEFAULT_TOKEN_PATH)
         self.client_secret = client_secret
         self.config = config
         self.token_cache: Optional[msal.SerializableTokenCache] = None
         self.init_cache()
         self.app: Optional[msal.ClientApplication] = None
@@ -378,22 +382,36 @@
 
         # 502, 503, and 504 errors are often to Azure App issues.
         retry_codes = [401, 404, 429, 502, 503, 504]
 
         response = None
         for backoff in range(1, 10):
             try:
+                current_context = context.get_current()
                 LOGGER.debug("request %s %s %s", method, url, repr(json_data))
-                response = self.session.request(
-                    method,
-                    url,
-                    headers=headers,
-                    json=json_data,
-                    params=params,
-                    timeout=(REQUEST_CONNECT_TIMEOUT, REQUEST_READ_TIMEOUT),
+
+                request_to_downstream = requests.Request(
+                    method, url, headers=headers, json=json_data, params=params
+                )
+
+                PROPAGATOR.inject(
+                    carrier=request_to_downstream.headers,
+                    context=current_context,
+                )
+
+                correlation_id = ""
+                for span in current_context.values():
+                    correlation_id = str(hex(span.__dict__["_context"].trace_id))[2:]
+                    break
+
+                LOGGER.debug("OneFuzz CorrelationId: %s", correlation_id)
+                prep_req = self.session.prepare_request(request_to_downstream)
+
+                response = self.session.send(
+                    prep_req, timeout=(REQUEST_CONNECT_TIMEOUT, REQUEST_READ_TIMEOUT)
                 )
 
                 if response.status_code not in retry_codes:
                     break
 
                 check_application_error(response)
```

### Comparing `onefuzz-8.4.0/onefuzz/cli.py` & `onefuzz-8.5.0/onefuzz/cli.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/data/licenses.json` & `onefuzz-8.5.0/onefuzz/data/licenses.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.953125%*

 * *Differences: {'4': "{'Version': '2023.5'}", '5': "{'Version': '0.2.2'}", '6': "{'Version': '4.7.1'}"}*

```diff
@@ -23,27 +23,27 @@
         "URL": "https://www.pyinstaller.org/",
         "Version": "5.13.0"
     },
     {
         "License": "UNKNOWN",
         "Name": "pyinstaller-hooks-contrib",
         "URL": "https://github.com/pyinstaller/pyinstaller-hooks-contrib",
-        "Version": "2023.3"
+        "Version": "2023.5"
     },
     {
         "License": "BSD-3-Clause",
         "Name": "pywin32-ctypes",
         "URL": "https://github.com/enthought/pywin32-ctypes",
-        "Version": "0.2.1"
+        "Version": "0.2.2"
     },
     {
         "License": "Python Software Foundation License",
         "Name": "typing-extensions",
         "URL": "UNKNOWN",
-        "Version": "4.6.3"
+        "Version": "4.7.1"
     },
     {
         "License": "MIT License",
         "Name": "zipp",
         "URL": "https://github.com/jaraco/zipp",
         "Version": "3.15.0"
     }
```

### Comparing `onefuzz-8.4.0/onefuzz/data/privacy.txt` & `onefuzz-8.5.0/onefuzz/data/privacy.txt`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/debug.py` & `onefuzz-8.5.0/onefuzz/debug.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/job_templates/builder.py` & `onefuzz-8.5.0/onefuzz/job_templates/builder.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/job_templates/cache.py` & `onefuzz-8.5.0/onefuzz/job_templates/cache.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/job_templates/handlers.py` & `onefuzz-8.5.0/onefuzz/job_templates/handlers.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/job_templates/job_monitor.py` & `onefuzz-8.5.0/onefuzz/job_templates/job_monitor.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/job_templates/main.py` & `onefuzz-8.5.0/onefuzz/job_templates/main.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/job_templates/manage.py` & `onefuzz-8.5.0/onefuzz/job_templates/manage.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/rdp.py` & `onefuzz-8.5.0/onefuzz/rdp.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/ssh.py` & `onefuzz-8.5.0/onefuzz/ssh.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/status/cache.py` & `onefuzz-8.5.0/onefuzz/status/cache.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/status/cmd.py` & `onefuzz-8.5.0/onefuzz/status/cmd.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/status/raw.py` & `onefuzz-8.5.0/onefuzz/status/raw.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/status/signalr.py` & `onefuzz-8.5.0/onefuzz/status/signalr.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/status/top.py` & `onefuzz-8.5.0/onefuzz/status/top.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/status/top_view.py` & `onefuzz-8.5.0/onefuzz/status/top_view.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/template.py` & `onefuzz-8.5.0/onefuzz/template.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/templates/__init__.py` & `onefuzz-8.5.0/onefuzz/templates/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -106,22 +106,26 @@
     def delete_container(self, container_name: Container) -> None:
         self.onefuzz.containers.delete(container_name)
 
     def setup_notifications(self, config: Optional[NotificationConfig]) -> None:
         if not config:
             return
 
-        container: Optional[str] = None
+        containers: List[Container] = []
         if ContainerType.unique_reports in self.containers:
-            container = self.containers[ContainerType.unique_reports]
+            containers.append(self.containers[ContainerType.unique_reports])
         else:
-            container = self.containers[ContainerType.reports]
+            containers.append(self.containers[ContainerType.reports])
 
-        self.logger.info("creating notification config for %s", container)
-        self.onefuzz.notifications.create(container, config, replace_existing=True)
+        if ContainerType.regression_reports in self.containers:
+            containers.append(self.containers[ContainerType.regression_reports])
+
+        for container in containers:
+            self.logger.info("creating notification config for %s", container)
+            self.onefuzz.notifications.create(container, config, replace_existing=True)
 
     def upload_setup(
         self,
         setup_dir: Optional[Directory],
         target_exe: File,
         setup_files: Optional[List[File]] = None,
     ) -> None:
```

### Comparing `onefuzz-8.4.0/onefuzz/templates/afl.py` & `onefuzz-8.5.0/onefuzz/templates/afl.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/templates/libfuzzer.py` & `onefuzz-8.5.0/onefuzz/templates/libfuzzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,15 @@
         minimized_stack_depth: Optional[int] = None,
         module_allowlist: Optional[str] = None,
         source_allowlist: Optional[str] = None,
         analyzer_exe: Optional[str] = None,
         analyzer_options: Optional[List[str]] = None,
         analyzer_env: Optional[Dict[str, str]] = None,
         tools: Optional[Container] = None,
+        task_env: Optional[Dict[str, str]] = None,
     ) -> None:
         target_options = target_options or []
         regression_containers = [
             (ContainerType.setup, containers[ContainerType.setup]),
             (ContainerType.crashes, containers[ContainerType.crashes]),
             (ContainerType.unique_reports, containers[ContainerType.unique_reports]),
             (
@@ -121,14 +122,15 @@
             tags=tags,
             target_timeout=effective_crash_report_timeout,
             check_retry_count=check_retry_count,
             check_fuzzer_help=check_fuzzer_help,
             debug=debug,
             colocate=colocate_all_tasks or colocate_secondary_tasks,
             minimized_stack_depth=minimized_stack_depth,
+            task_env=task_env,
         )
 
         fuzzer_containers = [
             (ContainerType.setup, containers[ContainerType.setup]),
             (ContainerType.crashes, containers[ContainerType.crashes]),
             (ContainerType.inputs, containers[ContainerType.inputs]),
         ]
@@ -172,14 +174,15 @@
             target_workers=target_workers,
             tags=tags,
             debug=debug,
             ensemble_sync_delay=ensemble_sync_delay,
             colocate=colocate_all_tasks,
             check_fuzzer_help=check_fuzzer_help,
             expect_crash_on_failure=expect_crash_on_failure,
+            task_env=task_env,
         )
 
         prereq_tasks = [fuzzer_task.task_id, regression_task.task_id]
 
         coverage_containers = [
             (ContainerType.setup, containers[ContainerType.setup]),
             (ContainerType.coverage, containers[ContainerType.coverage]),
@@ -234,14 +237,15 @@
             tags=tags,
             prereq_tasks=prereq_tasks,
             debug=debug,
             colocate=colocate_all_tasks or colocate_secondary_tasks,
             check_fuzzer_help=check_fuzzer_help,
             module_allowlist=module_allowlist,
             source_allowlist=source_allowlist,
+            task_env=task_env,
         )
 
         report_containers = [
             (ContainerType.setup, containers[ContainerType.setup]),
             (ContainerType.crashes, containers[ContainerType.crashes]),
             (ContainerType.reports, containers[ContainerType.reports]),
             (ContainerType.unique_reports, containers[ContainerType.unique_reports]),
@@ -270,32 +274,29 @@
             prereq_tasks=prereq_tasks,
             target_timeout=effective_crash_report_timeout,
             check_retry_count=check_retry_count,
             check_fuzzer_help=check_fuzzer_help,
             debug=debug,
             colocate=colocate_all_tasks or colocate_secondary_tasks,
             minimized_stack_depth=minimized_stack_depth,
+            task_env=task_env,
         )
 
         if analyzer_exe is not None:
             self.logger.info("creating custom analysis")
 
-            if tools is None:
-                self.logger.error(
-                    "tools container cannot be empty when specifying a custom analyzer"
-                )
-                return None
-
             analysis_containers = [
                 (ContainerType.setup, containers[ContainerType.setup]),
-                (ContainerType.tools, tools),
                 (ContainerType.analysis, containers[ContainerType.analysis]),
                 (ContainerType.crashes, containers[ContainerType.crashes]),
             ]
 
+            if tools is not None:
+                analysis_containers.append((ContainerType.tools, tools))
+
             self._add_optional_containers(
                 analysis_containers,
                 containers,
                 [ContainerType.extra_setup, ContainerType.extra_output],
             )
 
             self.onefuzz.tasks.create(
@@ -313,14 +314,15 @@
                 analyzer_options=analyzer_options,
                 analyzer_env=analyzer_env,
                 tags=tags,
                 prereq_tasks=[fuzzer_task.task_id],
                 colocate=colocate_all_tasks or colocate_secondary_tasks,
                 debug=debug,
                 target_timeout=target_timeout,
+                task_env=task_env,
             )
 
     def basic(
         self,
         project: str,
         name: str,
         build: str,
@@ -361,14 +363,15 @@
         analyzer_exe: Optional[str] = None,
         analyzer_options: Optional[List[str]] = None,
         analyzer_env: Optional[Dict[str, str]] = None,
         tools: Optional[Container] = None,
         extra_setup_container: Optional[Container] = None,
         extra_output_container: Optional[Container] = None,
         crashes: Optional[Container] = None,
+        task_env: Optional[Dict[str, str]] = None,
     ) -> Optional[Job]:
         """
         Basic libfuzzer job
 
         :param bool ensemble_sync_delay: Specify duration between
             syncing inputs during ensemble fuzzing (0 to disable).
         """
@@ -492,14 +495,15 @@
             minimized_stack_depth=minimized_stack_depth,
             module_allowlist=module_allowlist_blob_name,
             source_allowlist=source_allowlist_blob_name,
             analyzer_exe=analyzer_exe,
             analyzer_options=analyzer_options,
             analyzer_env=analyzer_env,
             tools=tools,
+            task_env=task_env,
         )
 
         self.logger.info("done creating tasks")
         helper.wait()
         return helper.job
 
     def merge(
@@ -527,14 +531,15 @@
         dryrun: bool = False,
         notification_config: Optional[NotificationConfig] = None,
         debug: Optional[List[TaskDebugFlag]] = None,
         preserve_existing_outputs: bool = False,
         check_fuzzer_help: bool = False,
         no_check_fuzzer_help: bool = False,
         extra_setup_container: Optional[Container] = None,
+        task_env: Optional[Dict[str, str]] = None,
     ) -> Optional[Job]:
         """
         libfuzzer merge task
         """
         if check_fuzzer_help:
             self.logger.warning(
                 "--check_fuzzer_help is the default and does not need to be set; this parameter will be removed in a future version"
@@ -624,14 +629,15 @@
             target_env=target_env,
             tags=tags,
             target_timeout=crash_report_timeout,
             check_retry_count=check_retry_count,
             debug=debug,
             preserve_existing_outputs=preserve_existing_outputs,
             check_fuzzer_help=check_fuzzer_help,
+            task_env=task_env,
         )
 
         self.logger.info("done creating tasks")
         helper.wait()
         return helper.job
 
     def dotnet(
@@ -664,14 +670,15 @@
         ensemble_sync_delay: Optional[int] = None,
         colocate_all_tasks: bool = False,
         colocate_secondary_tasks: bool = True,
         expect_crash_on_failure: bool = False,
         notification_config: Optional[NotificationConfig] = None,
         extra_setup_container: Optional[Container] = None,
         crashes: Optional[Container] = None,
+        task_env: Optional[Dict[str, str]] = None,
     ) -> Optional[Job]:
         pool = self.onefuzz.pools.get(pool_name)
 
         # verify containers exist
         if existing_inputs:
             self.onefuzz.containers.get(existing_inputs)
 
@@ -778,14 +785,15 @@
             target_method=target_method,
             target_workers=target_workers,
             tags=tags,
             debug=debug,
             ensemble_sync_delay=ensemble_sync_delay,
             expect_crash_on_failure=expect_crash_on_failure,
             check_fuzzer_help=False,
+            task_env=task_env,
         )
 
         # Ensure the fuzzing task starts before we schedule the coverage and
         # crash reporting tasks (which are useless without it).
         prereq_tasks = [fuzzer_task.task_id]
 
         # Target options for the .NET harness produced by SharpFuzz, when _not_
@@ -825,14 +833,15 @@
             target_options=sharpfuzz_harness_target_options,
             target_env=target_env,
             target_timeout=target_timeout,
             tags=tags,
             prereq_tasks=prereq_tasks,
             debug=debug,
             colocate=colocate_all_tasks or colocate_secondary_tasks,
+            task_env=task_env,
         )
 
         report_containers = [
             (ContainerType.setup, containers[ContainerType.setup]),
             (ContainerType.crashes, containers[ContainerType.crashes]),
             (ContainerType.reports, containers[ContainerType.reports]),
             (ContainerType.unique_reports, containers[ContainerType.unique_reports]),
@@ -857,14 +866,15 @@
             target_env=target_env,
             tags=tags,
             prereq_tasks=prereq_tasks,
             target_timeout=target_timeout,
             check_retry_count=check_retry_count,
             debug=debug,
             colocate=colocate_all_tasks or colocate_secondary_tasks,
+            task_env=task_env,
         )
 
         self.logger.info("done creating tasks")
         helper.wait()
         return helper.job
 
     def qemu_user(
@@ -880,14 +890,15 @@
         vm_count: int = 1,
         inputs: Optional[Directory] = None,
         reboot_after_setup: bool = False,
         duration: int = 24,
         task_duration: Optional[int] = None,
         target_workers: Optional[int] = 1,
         target_options: Optional[List[str]] = None,
+        target_timeout: Optional[int] = None,
         fuzzing_target_options: Optional[List[str]] = None,
         target_env: Optional[Dict[str, str]] = None,
         tags: Optional[Dict[str, str]] = None,
         wait_for_running: bool = False,
         wait_for_files: Optional[List[ContainerType]] = None,
         existing_inputs: Optional[Container] = None,
         debug: Optional[List[TaskDebugFlag]] = None,
@@ -896,14 +907,15 @@
         crash_report_timeout: Optional[int] = 1,
         check_retry_count: Optional[int] = 300,
         check_fuzzer_help: bool = False,
         no_check_fuzzer_help: bool = False,
         extra_setup_container: Optional[Container] = None,
         crashes: Optional[Container] = None,
         readonly_inputs: Optional[Container] = None,
+        task_env: Optional[Dict[str, str]] = None,
     ) -> Optional[Job]:
         """
         libfuzzer tasks, wrapped via qemu-user (PREVIEW FEATURE)
         """
         if check_fuzzer_help:
             self.logger.warning(
                 "--check_fuzzer_help is the default and does not need to be set; this parameter will be removed in a future version"
@@ -1046,19 +1058,21 @@
             pool_name=pool_name,
             reboot_after_setup=reboot_after_setup,
             duration=task_duration if task_duration else duration,
             vm_count=vm_count,
             target_options=libfuzzer_fuzz_target_options,
             target_env=target_env,
             target_workers=target_workers,
+            target_timeout=target_timeout,
             tags=tags,
             debug=debug,
             ensemble_sync_delay=ensemble_sync_delay,
             expect_crash_on_failure=False,
             check_fuzzer_help=check_fuzzer_help,
+            task_env=task_env,
         )
 
         report_containers = [
             (ContainerType.setup, helper.containers[ContainerType.setup]),
             (ContainerType.crashes, helper.containers[ContainerType.crashes]),
             (ContainerType.reports, helper.containers[ContainerType.reports]),
             (
@@ -1087,12 +1101,13 @@
             prereq_tasks=[fuzzer_task.task_id],
             target_timeout=crash_report_timeout,
             check_retry_count=check_retry_count,
             debug=debug,
             colocate=colocate_all_tasks,
             expect_crash_on_failure=False,
             check_fuzzer_help=check_fuzzer_help,
+            task_env=task_env,
         )
 
         self.logger.info("done creating tasks")
         helper.wait()
         return helper.job
```

### Comparing `onefuzz-8.4.0/onefuzz/templates/ossfuzz.py` & `onefuzz-8.5.0/onefuzz/templates/ossfuzz.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/templates/radamsa.py` & `onefuzz-8.5.0/onefuzz/templates/radamsa.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz/templates/regression.py` & `onefuzz-8.5.0/onefuzz/templates/regression.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/onefuzz.egg-info/PKG-INFO` & `onefuzz-8.5.0/onefuzz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onefuzz
-Version: 8.4.0
+Version: 8.5.0
 Summary: Onefuzz Client Library for Python
 Home-page: https://github.com/microsoft/onefuzz/
 Author: Microsoft Corporation
 Author-email: fuzzing@microsoft.com
 License: MIT
 Description: # OneFuzz SDK
```

### Comparing `onefuzz-8.4.0/onefuzz.egg-info/SOURCES.txt` & `onefuzz-8.5.0/onefuzz.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 onefuzz/__version__.py
 onefuzz/api.py
 onefuzz/azcopy.py
 onefuzz/azure_identity_credential_adapter.py
 onefuzz/backend.py
 onefuzz/cli.py
 onefuzz/debug.py
+onefuzz/opentelemetry_exporter.py
 onefuzz/rdp.py
 onefuzz/ssh.py
 onefuzz/template.py
 onefuzz.egg-info/PKG-INFO
 onefuzz.egg-info/SOURCES.txt
 onefuzz.egg-info/dependency_links.txt
 onefuzz.egg-info/entry_points.txt
```

### Comparing `onefuzz-8.4.0/setup.py` & `onefuzz-8.5.0/setup.py`

 * *Files identical despite different names*

### Comparing `onefuzz-8.4.0/tests/test_template_helper.py` & `onefuzz-8.5.0/tests/test_template_helper.py`

 * *Files identical despite different names*

