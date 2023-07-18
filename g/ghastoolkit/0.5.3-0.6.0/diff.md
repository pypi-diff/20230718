# Comparing `tmp/ghastoolkit-0.5.3.tar.gz` & `tmp/ghastoolkit-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.5.3.tar", last modified: Mon Jul 17 14:30:31 2023, max compression
+gzip compressed data, was "ghastoolkit-0.6.0.tar", last modified: Tue Jul 18 17:01:51 2023, max compression
```

## Comparing `ghastoolkit-0.5.3.tar` & `ghastoolkit-0.6.0.tar`

### file list

```diff
@@ -1,66 +1,67 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.317153 ghastoolkit-0.5.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.321153 ghastoolkit-0.5.3/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.321153 ghastoolkit-0.5.3/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.321153 ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/ext.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.321153 ghastoolkit-0.5.3/src/ghastoolkit/codeql/packs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/packs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/packs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3857 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/packs/pack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/packs/packs.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/codeql/results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     8164 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/github.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/src/ghastoolkit/octokit/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.321153 ghastoolkit-0.5.3/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-17 14:30:31.000000 ghastoolkit-0.5.3/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-07-17 14:30:31.000000 ghastoolkit-0.5.3/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 14:30:31.000000 ghastoolkit-0.5.3/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-17 14:30:31.000000 ghastoolkit-0.5.3/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 14:30:31.000000 ghastoolkit-0.5.3/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 14:30:31.325154 ghastoolkit-0.5.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_clearlydefined.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_codeql_dataext.py
--rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-17 14:29:58.000000 ghastoolkit-0.5.3/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.809985 ghastoolkit-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-18 17:01:51.809985 ghastoolkit-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 17:01:51.809985 ghastoolkit-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.801986 ghastoolkit-0.6.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.805986 ghastoolkit-0.6.0/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.805986 ghastoolkit-0.6.0/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10889 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.805986 ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/ext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.805986 ghastoolkit-0.6.0/src/ghastoolkit/codeql/packs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/packs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2653 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/packs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/packs/pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/packs/packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/codeql/results.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.805986 ghastoolkit-0.6.0/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2892 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2079 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9579 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8018 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/github.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.809985 ghastoolkit-0.6.0/src/ghastoolkit/octokit/graphql/
+-rw-r--r--   0 runner    (1001) docker     (123)     2352 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11077 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4983 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.809985 ghastoolkit-0.6.0/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.809985 ghastoolkit-0.6.0/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4375 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.805986 ghastoolkit-0.6.0/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-07-18 17:01:51.000000 ghastoolkit-0.6.0/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-07-18 17:01:51.000000 ghastoolkit-0.6.0/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:01:51.000000 ghastoolkit-0.6.0/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-07-18 17:01:51.000000 ghastoolkit-0.6.0/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 17:01:51.000000 ghastoolkit-0.6.0/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:01:51.809985 ghastoolkit-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_clearlydefined.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_codeql_dataext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1539 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_codeql_packs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-18 17:01:23.000000 ghastoolkit-0.6.0/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.5.3/LICENSE` & `ghastoolkit-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/PKG-INFO` & `ghastoolkit-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.5.3
+Version: 0.6.0
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.5.3/README.md` & `ghastoolkit-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/pyproject.toml` & `ghastoolkit-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.5.3"
+version = "0.6.0"
 authors = [{ name = "GeekMasher" }]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Development Status :: 4 - Beta",
     "License :: OSI Approved :: MIT License",
```

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/__init__.py` & `ghastoolkit-0.6.0/src/ghastoolkit/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.5.3"
+__version__ = "0.6.0"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/__main__.py` & `ghastoolkit-0.6.0/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/codeql/cli.py` & `ghastoolkit-0.6.0/src/ghastoolkit/codeql/cli.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.6.0/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/__main__.py` & `ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/ext.py` & `ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/ext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/codeql/dataextensions/models.py` & `ghastoolkit-0.6.0/src/ghastoolkit/codeql/dataextensions/models.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/codeql/packs/packs.py` & `ghastoolkit-0.6.0/src/ghastoolkit/codeql/packs/packs.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/codeql/results.py` & `ghastoolkit-0.6.0/src/ghastoolkit/codeql/results.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/octokit/advisories.py` & `ghastoolkit-0.6.0/src/ghastoolkit/octokit/advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/octokit/clearlydefined.py` & `ghastoolkit-0.6.0/src/ghastoolkit/octokit/clearlydefined.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.6.0/src/ghastoolkit/octokit/codescanning.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,88 +1,92 @@
+"""GitHub Code Scanning API Module."""
 from dataclasses import dataclass
 import json
 import logging
 from typing import Any, List, Optional
 from ghastoolkit.octokit.github import GitHub, Repository
 from ghastoolkit.octokit.octokit import OctoItem, RestRequest
 
 logger = logging.getLogger("ghastoolkit.octokit.codescanning")
 
 
 @dataclass
 class CodeAlert(OctoItem):
-    """Code Alert from Code Scanning API"""
+    """Code Alert from Code Scanning API."""
 
     number: int
     """Unique Identifier"""
     state: str
     """State of the alert. States can be `open`, `closed`, `dismissed`, or `fixed`."""
 
     created_at: str
-    """Alert Creation date and time"""
+    """Alert Creation date and time."""
 
     rule: dict
-    """Rule Data (rule_id, severity, description, etc)"""
+    """Rule Data (rule_id, severity, description, etc)."""
     tool: dict
-    """Tool information (name, version, guid)"""
+    """Tool information (name, version, guid)."""
 
     _instances: Optional[list[dict]] = None
 
     @property
     def rule_id(self) -> str:
-        """Rule Identifier"""
+        """Rule Identifier."""
         return self.rule.get("id", "NA")
 
     @property
     def description(self) -> Optional[str]:
-        """Rule Description / Title"""
+        """Rule Description / Title."""
         return self.rule.get("description")
 
     @property
     def tool_name(self) -> str:
-        """Tool name"""
+        """Tool name."""
         return self.tool.get("name", "NA")
 
     @property
     def tool_fullname(self) -> str:
-        """Full tool name with version information"""
+        """Full tool name with version information."""
         version = self.tool.get("version")
         return f"{self.tool_name}@{version}"
 
     @property
     def severity(self) -> str:
-        """Severity of the alert using `security_severity_level`"""
+        """Severity of the alert using `security_severity_level`."""
         return self.rule.get("security_severity_level", "NA")
 
     @property
     def instances(self) -> list[dict]:
-        """Get list of instances of the alert"""
+        """Get list of instances of the alert."""
         if not self._instances:
             self._instances = CodeScanning().getAlertInstances(self.number)
         return self._instances
 
     def __str__(self) -> str:
+        """To String."""
         return f"CodeAlert({self.number}, '{self.state}', '{self.tool_name}', '{self.rule_id}')"
 
 
 class CodeScanning:
+    """Code Scanning."""
+
     def __init__(self, repository: Optional[Repository] = None) -> None:
-        """GitHub Code Scanning REST API
+        """Code Scanning REST API.
 
         https://docs.github.com/en/rest/code-scanning
         """
         self.repository = repository or GitHub.repository
         self.tools: List[str] = []
 
         if not self.repository:
             raise Exception("CodeScanning requires Repository to be set")
         self.rest = RestRequest(self.repository)
 
     def getOrganizationAlerts(self, state: str = "open") -> list[dict[Any, Any]]:
-        """Get Organization Alerts
+        """Get Organization Alerts.
 
         https://docs.github.com/en/rest/code-scanning#list-code-scanning-alerts-for-an-organization
         """
         results = self.rest.get(
             "/orgs/{org}/code-scanning/alerts", {"state": state}, authenticated=True
         )
         if isinstance(results, list):
@@ -93,15 +97,16 @@
         self,
         state: str = "open",
         tool_name: Optional[str] = None,
         ref: Optional[str] = None,
         sort: Optional[str] = None,
         severity: Optional[str] = None,
     ) -> list[CodeAlert]:
-        """Get all code scanning alerts
+        """Get all code scanning alerts.
+
         https://docs.github.com/en/rest/code-scanning#list-code-scanning-alerts-for-a-repository
         """
         results = self.rest.get(
             "/repos/{owner}/{repo}/code-scanning/alerts",
             {
                 "state": state,
                 "tool_name": tool_name,
@@ -137,76 +142,76 @@
                 results.append(alert)
         return results
 
     @RestRequest.restGet(
         "/repos/{owner}/{repo}/code-scanning/alerts/{alert_number}", authenticated=True
     )
     def getAlert(self, alert_number: int) -> CodeAlert:
-        """Get Single Alert information from Code Scanning
+        """Get Single Alert information from Code Scanning.
 
         https://docs.github.com/en/rest/code-scanning#get-a-code-scanning-alert
         """
         return {}
 
     def getAlertInstances(
         self, alert_number: int, ref: Optional[str] = None
     ) -> list[dict]:
-        """Get a list of alert instances"""
+        """Get a list of alert instances."""
         result = self.rest.get(
             "/repos/{owner}/{repo}/code-scanning/alerts/{alert_number}/instances",
             {"alert_number": alert_number, "ref": ref},
         )
         return result
 
     def getAnalyses(
         self, reference: Optional[str] = None, tool: Optional[str] = None
     ) -> list[dict]:
-        """Get a list of all the analyses for a given repository
+        """Get a list of all the analyses for a given repository.
 
         https://docs.github.com/en/enterprise-cloud@latest/rest/code-scanning#list-code-scanning-analyses-for-a-repository
         """
         results = self.rest.get(
             "/repos/{org}/{repo}/code-scanning/analyses",
             {"tool_name": tool, "ref": reference or self.repository.reference},
         )
         if isinstance(results, list):
             return results
         raise Exception(f"")
 
     def getLatestAnalyses(
         self, reference: Optional[str] = None, tool: Optional[str] = None
     ) -> list[dict]:
-        """Get Latest Analyses for every tool"""
+        """Get Latest Analyses for every tool."""
         tools = set()
         results = []
         for analysis in self.getAnalyses(reference, tool):
             name = analysis.get("tool", {}).get("name")
             if name in tools:
                 continue
             tools.add(name)
             results.append(analysis)
 
         self.tools = list(tools)
 
         return results
 
     def getTools(self, reference: Optional[str] = None) -> List[str]:
-        """Get list of tools from the latest analyses"""
+        """Get list of tools from the latest analyses."""
         if len(self.tools) == 0:
             self.getLatestAnalyses(reference)
         return self.tools
 
     def getSarifId(self, url: str) -> int:
-        """Get the latest SARIF ID from a URL"""
+        """Get the latest SARIF ID from a URL."""
         if url and "/" in url:
             return int(url.split("/")[-1])
         return -1
 
     def downloadSARIF(self, output: str, sarif_id: int) -> bool:
-        """Get SARIF by ID (UUID)"""
+        """Get SARIF by ID (UUID)."""
         logger.debug(f"Downloading SARIF file :: {sarif_id}")
 
         # need to change "Accept" and then reset
         og_accept = self.rest.session.headers.pop("Accept")
         self.rest.session.headers["Accept"] = "application/sarif+json"
         result = self.rest.get(
             "/repos/{org}/{repo}/code-scanning/analyses/{sarif_id}",
@@ -219,22 +224,59 @@
             json.dump(result, handle, indent=2)
         logger.debug("Saved SARIF file")
         return True
 
     # CodeQL
 
     def getCodeQLDatabases(self) -> list[dict]:
-        """List CodeQL databases for a repository
+        """List CodeQL databases for a repository.
 
         https://docs.github.com/en/rest/code-scanning?apiVersion=2022-11-28#list-codeql-databases-for-a-repository
         """
         return self.rest.get("/repos/{owner}/{repo}/code-scanning/codeql/databases")
 
     def getCodeQLDatabase(self, language: str) -> dict:
-        """Get a CodeQL database for a repository
+        """Get a CodeQL database for a repository.
 
         https://docs.github.com/en/rest/code-scanning?apiVersion=2022-11-28#get-a-codeql-database-for-a-repository
         """
         return self.rest.get(
-            "/repos/{owner}/{repo}/code-scanning/codeql/databases/{language}",
+            "/repos/{oner}/{repo}/code-scanning/codeql/databases/{language}",
             {"language": language},
         )
+
+    def getPacks(self, visibility: str = "internal") -> List[dict]:
+        """Get all CodeQL Packs from remote GitHub instance.
+
+        CodeQL Packs are stored in GitHub's container registry so this function might
+        return other container images.
+        """
+        result = self.rest.get(
+            "/orgs/{org}/packages",
+            {"package_type": "container", "visibility": visibility},
+        )
+        if isinstance(result, list):
+            return result
+        return []
+
+    def getPackVersions(self, pack_name: str) -> list[dict]:
+        """Get a list of all remote pack versions."""
+        if "/" in pack_name:
+            # full name
+            org, pack_name = pack_name.split("/")
+        else:
+            org = self.repository.owner
+
+        result = self.rest.get(
+            "/orgs/{pack_org}/packages/{package_type}/{package_name}/versions",
+            {"pack_org": org, "package_type": "container", "package_name": pack_name},
+        )
+        if isinstance(result, list):
+            return result
+        return []
+
+    def getLatestPackVersion(self, pack_name: str) -> dict:
+        """Get the current remote CodeQL pack version."""
+        versions = self.getPackVersions(pack_name)
+        if len(versions) != 0:
+            return versions[0]
+        return {}
```

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.6.0/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.6.0/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.6.0/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/octokit/graphql/__init__.py` & `ghastoolkit-0.6.0/src/ghastoolkit/octokit/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.6.0/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.6.0/src/ghastoolkit/octokit/secretscanning.py`

 * *Files 24% similar despite different names*

```diff
@@ -7,101 +7,134 @@
 
 
 logger = logging.getLogger("ghastoolkit.octokit.secretscanning")
 
 
 @dataclass
 class SecretAlert(OctoItem):
+    """Secret Scanning Alert."""
+
     number: int
     state: str
 
     created_at: str
 
     secret_type: str
     secret_type_display_name: str
     secret: str
 
     _locations: list[dict] = field(default_factory=list)
     _sha: Optional[str] = None
 
     @property
     def locations(self) -> list[dict]:
-        """Get Alert locations (use cache or request from API)"""
+        """Get Alert locations.
+
+        Use cache or request from API."""
         if not self._locations:
             self._locations = SecretScanning().getAlertLocations(self.number)
         return self._locations
 
     @property
     def commit_sha(self) -> Optional[str]:
-        """Get commit sha if present"""
+        """Get commit sha if present."""
         if self._sha is None:
             for loc in self.locations:
                 if loc.get("type") == "commit":
                     self._sha = loc.get("details", {}).get("blob_sha")
                     break
         return self._sha
 
     def __str__(self) -> str:
         return f"SecretAlert({self.number}, '{self.secret_type}')"
 
 
 class SecretScanning:
+    """Secret Scanning API."""
+
     def __init__(self, repository: Optional[Repository] = None) -> None:
+        """Initialise Secret Scanning API."""
         self.repository = repository or GitHub.repository
         if not self.repository:
             raise Exception("SecretScanning requires Repository to be set")
 
         self.rest = RestRequest(self.repository)
 
+        self.state = None
+
+    def isEnabled(self) -> bool:
+        """Check to see if Secret Scanning is enabled or not."""
+        if not self.state:
+            self.state = self.getStatus()
+        # if advanced_security is disabled, secret scanning will be
+        adsec = self.state.get("advanced_security", {}).get("status", "disabled")
+        return self.state.get("secret_scanning", {}).get("status", adsec) == "enabled"
+
+    def isPushProtectionEnabled(self) -> bool:
+        """Check if Push Protection is enabled."""
+        if not self.state:
+            self.state = self.getStatus()
+        status = self.state.get("secret_scanning_push_protection", {}).get(
+            "status", "disabled"
+        )
+        return status == "enabled"
+
+    def getStatus(self) -> dict:
+        """Get Status of GitHub Advanced Security."""
+        result = self.rest.get("get/repos/{owner}/{repo}")
+        if isinstance(result, dict):
+            return result.get("source", {}).get("security_and_analysis", {})
+        raise Exception("Failed to get the current state of secret scanning")
+
     def getOrganizationAlerts(self, state: Optional[str] = None) -> list[dict]:
-        """Get Organization Alerts
+        """Get Organization Alerts.
 
         https://docs.github.com/en/rest/secret-scanning#list-secret-scanning-alerts-for-an-organization
         """
         results = self.rest.get("/orgs/{org}/secret-scanning/alerts", {"state": state})
         if isinstance(results, list):
             return results
         raise Exception(f"Error getting organization secret scanning results")
 
     @RestRequest.restGet("/repos/{owner}/{repo}/secret-scanning/alerts")
     def getAlerts(self, state: str = "open") -> list[SecretAlert]:
-        """Get Repository alerts
+        """Get Repository alerts.
 
         https://docs.github.com/en/rest/secret-scanning#list-secret-scanning-alerts-for-a-repository
         """
         return []
 
     def getAlert(
         self, alert_number: int, state: Optional[str] = None
     ) -> Optional[SecretAlert]:
-        """Get Alert by `alert_number`
+        """Get Alert by `alert_number`.
 
         https://docs.github.com/en/rest/secret-scanning#get-a-secret-scanning-alert
         """
         results = self.rest.get(
             "/repos/{owner}/{repo}/secret-scanning/alerts/{alert_number}",
             {"alert_number": alert_number, "state": state},
         )
         if isinstance(results, dict):
             return loadOctoItem(SecretAlert, results)
 
     def getAlertsInPR(self) -> list[SecretAlert]:
-        """Get Alerts in a Pull Request"""
+        """Get Alerts in a Pull Request."""
         results = []
         pr_commits = self.repository.getPullRequestCommits()
         logger.debug(f"Number of Commits in PR :: {len(pr_commits)}")
 
         for alert in self.getAlerts("open"):
             if alert.commit_sha in pr_commits:
                 results.append(alert)
 
         return results
 
     def getAlertLocations(self, alert_number: int) -> list[dict]:
-        """Get Alert Locations by `alert_number`
+        """Get Alert Locations by `alert_number`.
 
         https://docs.github.com/en/rest/secret-scanning#list-locations-for-a-secret-scanning-alert
         """
         results = self.rest.get(
             "/repos/{owner}/{repo}/secret-scanning/alerts/{alert_number}/locations",
             {"alert_number": alert_number},
         )
```

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.6.0/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/supplychain/advisories.py` & `ghastoolkit-0.6.0/src/ghastoolkit/supplychain/advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.6.0/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.6.0/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.6.0/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.6.0/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.5.3
+Version: 0.6.0
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.5.3/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.6.0/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 src/ghastoolkit/supplychain/advisories.py
 src/ghastoolkit/supplychain/dependencies.py
 src/ghastoolkit/supplychain/dependencyalert.py
 src/ghastoolkit/supplychain/licensing.py
 tests/test_advisories.py
 tests/test_clearlydefined.py
 tests/test_codeql_dataext.py
+tests/test_codeql_packs.py
 tests/test_codeqldb.py
 tests/test_codescanning.py
 tests/test_default.py
 tests/test_dependencies.py
 tests/test_depgraph.py
 tests/test_github.py
 tests/test_licenses.py
```

### Comparing `ghastoolkit-0.5.3/tests/test_advisories.py` & `ghastoolkit-0.6.0/tests/test_advisories.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/tests/test_codeql_dataext.py` & `ghastoolkit-0.6.0/tests/test_codeql_dataext.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/tests/test_codeqldb.py` & `ghastoolkit-0.6.0/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/tests/test_codescanning.py` & `ghastoolkit-0.6.0/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/tests/test_default.py` & `ghastoolkit-0.6.0/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/tests/test_dependencies.py` & `ghastoolkit-0.6.0/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/tests/test_depgraph.py` & `ghastoolkit-0.6.0/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/tests/test_github.py` & `ghastoolkit-0.6.0/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/tests/test_licenses.py` & `ghastoolkit-0.6.0/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/tests/test_octokit.py` & `ghastoolkit-0.6.0/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.5.3/tests/test_secretscanning.py` & `ghastoolkit-0.6.0/tests/test_secretscanning.py`

 * *Files identical despite different names*

