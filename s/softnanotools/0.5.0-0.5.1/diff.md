# Comparing `tmp/softnanotools-0.5.0.tar.gz` & `tmp/softnanotools-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "softnanotools-0.5.0.tar", last modified: Fri Apr 28 15:27:33 2023, max compression
+gzip compressed data, was "softnanotools-0.5.1.tar", last modified: Tue Jul 18 07:30:52 2023, max compression
```

## Comparing `softnanotools-0.5.0.tar` & `softnanotools-0.5.1.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.129237 softnanotools-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 15:27:22.000000 softnanotools-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-28 15:27:22.000000 softnanotools-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-28 15:27:33.129237 softnanotools-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-04-28 15:27:22.000000 softnanotools-0.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-28 15:27:22.000000 softnanotools-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      417 2023-04-28 15:27:33.129237 softnanotools-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-28 15:27:22.000000 softnanotools-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.129237 softnanotools-0.5.0/softnanotools/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-28 15:27:33.129237 softnanotools-0.5.0/softnanotools/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools/generate/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/_package.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/_script.py
--rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools/generate/assets/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/.gitattributes.template
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/.gitignore.template
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/.pre-commit-config.yaml.template
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/MANIFEST.in.template
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/README.md.template
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/__init__.py.template
--rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/_version.py.template
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/coverage.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/pyproject.toml.template
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/quick-build.yml.template
--rw-r--r--   0 runner    (1001) docker     (123)      682 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/setup.cfg.template
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/setup.py.template
--rw-r--r--   0 runner    (1001) docker     (123)    68670 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/assets/versioneer.py.template
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools/generate/git/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/generate/git/_actions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools/logger/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/logger/_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools/notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/notebooks/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/notebooks/_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools/runner/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/runner/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/runner/_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools/timer/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/timer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-04-28 15:27:22.000000 softnanotools-0.5.0/softnanotools/timer/_timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/softnanotools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-04-28 15:27:33.000000 softnanotools-0.5.0/softnanotools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-04-28 15:27:33.000000 softnanotools-0.5.0/softnanotools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 15:27:33.000000 softnanotools-0.5.0/softnanotools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-28 15:27:33.000000 softnanotools-0.5.0/softnanotools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-28 15:27:33.000000 softnanotools-0.5.0/softnanotools.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.125236 softnanotools-0.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.129237 softnanotools-0.5.0/test/test_generate/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/test_components.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/test_module.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      590 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/test_project.py
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/test_script.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_generate/test_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.129237 softnanotools-0.5.0/test/test_logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_logger/test_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:33.129237 softnanotools-0.5.0/test/test_notebooks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_notebooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_notebooks/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_notebooks/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-28 15:27:22.000000 softnanotools-0.5.0/test/test_notebooks/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-04-28 15:27:22.000000 softnanotools-0.5.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:52.654701 softnanotools-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-18 07:30:38.000000 softnanotools-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-18 07:30:38.000000 softnanotools-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-18 07:30:52.654701 softnanotools-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2126 2023-07-18 07:30:38.000000 softnanotools-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-18 07:30:38.000000 softnanotools-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-07-18 07:30:52.654701 softnanotools-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-18 07:30:38.000000 softnanotools-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:52.654701 softnanotools-0.5.1/softnanotools/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-18 07:30:52.654701 softnanotools-0.5.1/softnanotools/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:52.646701 softnanotools-0.5.1/softnanotools/generate/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2024 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2768 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:52.650701 softnanotools-0.5.1/softnanotools/generate/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/assets/.gitattributes.template
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/assets/.gitignore.template
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/assets/.pre-commit-config.yaml.template
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/assets/MANIFEST.in.template
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/assets/README.md.template
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/assets/__init__.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)    18474 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/assets/_version.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/assets/coverage.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/assets/pyproject.toml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/assets/quick-build.yml.template
+-rw-r--r--   0 runner    (1001) docker     (123)      682 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/assets/setup.cfg.template
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/assets/setup.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)    68670 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/assets/versioneer.py.template
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:52.650701 softnanotools-0.5.1/softnanotools/generate/git/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/generate/git/_actions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:52.650701 softnanotools-0.5.1/softnanotools/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4112 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/logger/_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:52.650701 softnanotools-0.5.1/softnanotools/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/notebooks/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/notebooks/_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:52.650701 softnanotools-0.5.1/softnanotools/runner/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/runner/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2591 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/runner/_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:52.650701 softnanotools-0.5.1/softnanotools/timer/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/timer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-18 07:30:38.000000 softnanotools-0.5.1/softnanotools/timer/_timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:52.646701 softnanotools-0.5.1/softnanotools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2522 2023-07-18 07:30:52.000000 softnanotools-0.5.1/softnanotools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-18 07:30:52.000000 softnanotools-0.5.1/softnanotools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:30:52.000000 softnanotools-0.5.1/softnanotools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-07-18 07:30:52.000000 softnanotools-0.5.1/softnanotools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 07:30:52.000000 softnanotools-0.5.1/softnanotools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:52.650701 softnanotools-0.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/test_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:52.650701 softnanotools-0.5.1/test/test_generate/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/test_generate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/test_generate/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/test_generate/test_components.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/test_generate/test_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/test_generate/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/test_generate/test_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/test_generate/test_script.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/test_generate/test_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:52.654701 softnanotools-0.5.1/test/test_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/test_logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/test_logger/test_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:52.654701 softnanotools-0.5.1/test/test_notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/test_notebooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/test_notebooks/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/test_notebooks/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-18 07:30:38.000000 softnanotools-0.5.1/test/test_notebooks/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-07-18 07:30:38.000000 softnanotools-0.5.1/versioneer.py
```

### Comparing `softnanotools-0.5.0/LICENSE` & `softnanotools-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/PKG-INFO` & `softnanotools-0.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: softnanotools
-Version: 0.5.0
+Version: 0.5.1
 Summary: Tools for computing
 Home-page: https://github.com/softnanolab/softnanotools
 Author: Debesh Mandal
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `softnanotools-0.5.0/README.md` & `softnanotools-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/setup.py` & `softnanotools-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/cli.py` & `softnanotools-0.5.1/softnanotools/cli.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/generate/_components.py` & `softnanotools-0.5.1/softnanotools/generate/_components.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/generate/_module.py` & `softnanotools-0.5.1/softnanotools/generate/_module.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/generate/_package.py` & `softnanotools-0.5.1/softnanotools/generate/_package.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/generate/_project.py` & `softnanotools-0.5.1/softnanotools/generate/_project.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/generate/_script.py` & `softnanotools-0.5.1/softnanotools/generate/_script.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/generate/_tests.py` & `softnanotools-0.5.1/softnanotools/generate/_tests.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/generate/assets/.gitignore.template` & `softnanotools-0.5.1/softnanotools/generate/assets/.gitignore.template`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/generate/assets/README.md.template` & `softnanotools-0.5.1/softnanotools/generate/assets/README.md.template`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/generate/assets/_version.py.template` & `softnanotools-0.5.1/softnanotools/generate/assets/_version.py.template`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/generate/assets/coverage.yml.template` & `softnanotools-0.5.1/softnanotools/generate/assets/coverage.yml.template`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/generate/assets/quick-build.yml.template` & `softnanotools-0.5.1/softnanotools/generate/assets/quick-build.yml.template`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/generate/assets/setup.cfg.template` & `softnanotools-0.5.1/softnanotools/generate/assets/setup.cfg.template`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/generate/assets/setup.py.template` & `softnanotools-0.5.1/softnanotools/generate/assets/setup.py.template`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/generate/assets/versioneer.py.template` & `softnanotools-0.5.1/softnanotools/generate/assets/versioneer.py.template`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/generate/cli.py` & `softnanotools-0.5.1/softnanotools/generate/cli.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/logger/_logger.py` & `softnanotools-0.5.1/softnanotools/logger/_logger.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Container for the Logger class.
 
 Classes:
     Logger: tool for logging
-    NewLineFormatter: 
+    NewLineFormatter:
         formatter for the logger, ensuring prefixes can be easily
         added on each new line
 
 """
 import logging
 import os
 from pathlib import Path
@@ -91,20 +91,53 @@
         """Print a debug message for DEBUG_LEVEL<=10."""
         self.logger.debug(message)
 
     def info(self, message):
         """Print an info message for DEBUG_LEVEL<=20."""
         self.logger.info(message)
 
-    def warning(self, message):
+    def warning(self, message: str):
         """Print a warning message for DEBUG_LEVEL<=30."""
         self.logger.warning(message)
 
-    def error(self, message):
-        """Print an error message for DEBUG_LEVEL<=40."""
+    def error(
+        self,
+        message: str,
+        error: Exception = SystemError,
+        exception: Exception = None
+    ):
+        """Print an error message for DEBUG_LEVEL<=40.
+
+        Args:
+            message: message for logger to print
+            error: the error that should be raised
+            exception: any previous exceptions that caused the error
+
+        Raises:
+            Exception: (default SystemError)
+        """
         self.logger.error(message)
-        raise SystemError(message)
-
-    def kill(self, message=""):
-        """Kill program and print message for DEBUG_LEVEL<=50."""
+        if exception is None:
+            raise error(message)
+        else:
+            raise error(message) from exception
+
+    def kill(
+        self,
+        message: str,
+        exception: Exception = None
+    ):
+        """Kill program and print message for DEBUG_LEVEL<=50.
+
+        Args:
+            message: message for logger to print
+            error: the error that should be raised
+            exception: any previous exceptions that caused the error
+
+        Raises:
+            Exception: (default SystemExit)
+        """
         self.logger.critical(message)
-        raise SystemExit(message)
+        if exception is None:
+            raise SystemExit(message)
+        else:
+            raise SystemExit(message) from exception
```

### Comparing `softnanotools-0.5.0/softnanotools/notebooks/__init__.py` & `softnanotools-0.5.1/softnanotools/notebooks/__init__.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/notebooks/_core.py` & `softnanotools-0.5.1/softnanotools/notebooks/_core.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/notebooks/_utils.py` & `softnanotools-0.5.1/softnanotools/notebooks/_utils.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/runner/_runner.py` & `softnanotools-0.5.1/softnanotools/runner/_runner.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools/timer/_timer.py` & `softnanotools-0.5.1/softnanotools/timer/_timer.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/softnanotools.egg-info/PKG-INFO` & `softnanotools-0.5.1/softnanotools.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: softnanotools
-Version: 0.5.0
+Version: 0.5.1
 Summary: Tools for computing
 Home-page: https://github.com/softnanolab/softnanotools
 Author: Debesh Mandal
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.5
```

### Comparing `softnanotools-0.5.0/softnanotools.egg-info/SOURCES.txt` & `softnanotools-0.5.1/softnanotools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/test/test_generate/test_cli.py` & `softnanotools-0.5.1/test/test_generate/test_cli.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/test/test_generate/test_components.py` & `softnanotools-0.5.1/test/test_generate/test_components.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/test/test_generate/test_project.py` & `softnanotools-0.5.1/test/test_generate/test_project.py`

 * *Files identical despite different names*

### Comparing `softnanotools-0.5.0/test/test_logger/test_logger.py` & `softnanotools-0.5.1/test/test_logger/test_logger.py`

 * *Files 25% similar despite different names*

```diff
@@ -57,8 +57,44 @@
     ]
 
     with open(logfile, 'r') as f:
         for i, line in enumerate(f.readlines()):
             assert expected_output[i] == line
 
     logfile.unlink()
-    return
+    return
+
+def test_Logger_errors():
+    # Using custom error
+    logger = Logger(__name__)
+    try:
+        logger.error("Test Error", KeyError)
+    except KeyError:
+        pass
+
+    # Including traceback from previous exception
+    x = [1, 2, 3]
+    try:
+        x[4]
+    except IndexError as exc:
+        try:
+            logger.error("Test Error", exception=exc)
+        except SystemError:
+            pass
+
+def test_Logger_kills():
+    # Using custom error
+    logger = Logger(__name__)
+    try:
+        logger.kill("Test Error")
+    except SystemExit:
+        pass
+
+    # Including traceback from previous exception
+    x = [1, 2, 3]
+    try:
+        x[4]
+    except IndexError as exc:
+        try:
+            logger.kill("Test Error", exception=exc)
+        except SystemExit:
+            pass
```

### Comparing `softnanotools-0.5.0/versioneer.py` & `softnanotools-0.5.1/versioneer.py`

 * *Files identical despite different names*

