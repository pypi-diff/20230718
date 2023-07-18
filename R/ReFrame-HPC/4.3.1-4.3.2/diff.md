# Comparing `tmp/ReFrame-HPC-4.3.1.tar.gz` & `tmp/ReFrame-HPC-4.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ReFrame-HPC-4.3.1.tar", last modified: Fri Jul  7 20:59:18 2023, max compression
+gzip compressed data, was "ReFrame-HPC-4.3.2.tar", last modified: Tue Jul 18 07:01:01 2023, max compression
```

## Comparing `ReFrame-HPC-4.3.1.tar` & `ReFrame-HPC-4.3.2.tar`

### file list

```diff
@@ -1,89 +1,89 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:59:18.988805 ReFrame-HPC-4.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-07 20:59:18.988805 ReFrame-HPC-4.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/README_minimal.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:59:18.976805 ReFrame-HPC-4.3.1/ReFrame_HPC.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-07 20:59:18.000000 ReFrame-HPC-4.3.1/ReFrame_HPC.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-07 20:59:18.000000 ReFrame-HPC-4.3.1/ReFrame_HPC.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 20:59:18.000000 ReFrame-HPC-4.3.1/ReFrame_HPC.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-07 20:59:18.000000 ReFrame-HPC-4.3.1/ReFrame_HPC.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-07 20:59:18.000000 ReFrame-HPC-4.3.1/ReFrame_HPC.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:59:18.976805 ReFrame-HPC-4.3.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/bin/reframe
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:59:18.976805 ReFrame-HPC-4.3.1/reframe/
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:59:18.980805 ReFrame-HPC-4.3.1/reframe/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)    32121 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/buildsystems.py
--rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)    24544 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/containers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/deferrable.py
--rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/environments.py
--rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)    44510 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:59:18.980805 ReFrame-HPC-4.3.1/reframe/core/launchers/
--rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/launchers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/launchers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/launchers/mpi.py
--rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/launchers/rsh.py
--rw-r--r--   0 runner    (1001) docker     (123)    34546 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    36657 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/meta.py
--rw-r--r--   0 runner    (1001) docker     (123)    37547 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/modules.py
--rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/namespaces.py
--rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)    94662 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:59:18.984805 ReFrame-HPC-4.3.1/reframe/core/schedulers/
--rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/schedulers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/schedulers/flux.py
--rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/schedulers/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/schedulers/lsf.py
--rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/schedulers/oar.py
--rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/schedulers/pbs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/schedulers/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/schedulers/sge.py
--rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/schedulers/slurm.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/shell.py
--rw-r--r--   0 runner    (1001) docker     (123)    22804 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/systems.py
--rw-r--r--   0 runner    (1001) docker     (123)    29596 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/core/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:59:18.988805 ReFrame-HPC-4.3.1/reframe/frontend/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/frontend/argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/frontend/autodetect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/frontend/ci.py
--rw-r--r--   0 runner    (1001) docker     (123)    57029 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/frontend/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/frontend/dependencies.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:59:18.988805 ReFrame-HPC-4.3.1/reframe/frontend/executors/
--rw-r--r--   0 runner    (1001) docker     (123)    21499 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/frontend/executors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/frontend/executors/policies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/frontend/filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/frontend/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/frontend/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/frontend/runreport.py
--rw-r--r--   0 runner    (1001) docker     (123)    16299 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/frontend/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/frontend/testgenerators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:59:18.988805 ReFrame-HPC-4.3.1/reframe/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)    26220 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/schemas/config.json
--rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/schemas/junit.xsd
--rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/schemas/runreport.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 20:59:18.988805 ReFrame-HPC-4.3.1/reframe/utility/
--rw-r--r--   0 runner    (1001) docker     (123)    49673 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/utility/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/utility/color.py
--rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/utility/cpuinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/utility/jsonext.py
--rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/utility/osext.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/utility/profile.py
--rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/utility/sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/utility/typecheck.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/utility/udeps.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-07 20:59:04.000000 ReFrame-HPC-4.3.1/reframe/utility/versioning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-07 20:59:18.992805 ReFrame-HPC-4.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:01.549566 ReFrame-HPC-4.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-18 07:01:01.549566 ReFrame-HPC-4.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5257 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3608 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/README_minimal.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:01.537566 ReFrame-HPC-4.3.2/ReFrame_HPC.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-07-18 07:01:01.000000 ReFrame-HPC-4.3.2/ReFrame_HPC.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2082 2023-07-18 07:01:01.000000 ReFrame-HPC-4.3.2/ReFrame_HPC.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:01:01.000000 ReFrame-HPC-4.3.2/ReFrame_HPC.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-07-18 07:01:01.000000 ReFrame-HPC-4.3.2/ReFrame_HPC.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-18 07:01:01.000000 ReFrame-HPC-4.3.2/ReFrame_HPC.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:01.537566 ReFrame-HPC-4.3.2/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      546 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/bin/reframe
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:01.537566 ReFrame-HPC-4.3.2/reframe/
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:01.541566 ReFrame-HPC-4.3.2/reframe/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32121 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/buildsystems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7455 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24544 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8980 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6854 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9592 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/deferrable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8686 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/environments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10627 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5699 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44510 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:01.541566 ReFrame-HPC-4.3.2/reframe/core/launchers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3032 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/launchers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/launchers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5427 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/launchers/mpi.py
+-rw-r--r--   0 runner    (1001) docker     (123)      973 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/launchers/rsh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34546 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36657 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37547 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/namespaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16354 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    94662 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14317 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:01.541566 ReFrame-HPC-4.3.2/reframe/core/schedulers/
+-rw-r--r--   0 runner    (1001) docker     (123)    19439 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/schedulers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/schedulers/flux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6577 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/schedulers/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/schedulers/lsf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6644 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/schedulers/oar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9805 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/schedulers/pbs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1440 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/schedulers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5177 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/schedulers/sge.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25280 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/schedulers/slurm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/shell.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22804 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/systems.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29596 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/core/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:01.545566 ReFrame-HPC-4.3.2/reframe/frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11479 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/frontend/argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8272 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/frontend/autodetect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/frontend/ci.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57029 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/frontend/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7614 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/frontend/dependencies.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:01.545566 ReFrame-HPC-4.3.2/reframe/frontend/executors/
+-rw-r--r--   0 runner    (1001) docker     (123)    21499 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/frontend/executors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22692 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/frontend/executors/policies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/frontend/filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8363 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/frontend/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3052 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/frontend/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8849 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/frontend/runreport.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16299 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/frontend/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6240 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/frontend/testgenerators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:01.545566 ReFrame-HPC-4.3.2/reframe/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)    26220 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/schemas/config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9385 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/schemas/junit.xsd
+-rw-r--r--   0 runner    (1001) docker     (123)     6506 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/schemas/runreport.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:01:01.549566 ReFrame-HPC-4.3.2/reframe/utility/
+-rw-r--r--   0 runner    (1001) docker     (123)    49673 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/utility/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/utility/color.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10279 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/utility/cpuinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3814 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/utility/jsonext.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21443 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/utility/osext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/utility/profile.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32327 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/utility/sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14330 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/utility/typecheck.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/utility/udeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-07-18 07:00:51.000000 ReFrame-HPC-4.3.2/reframe/utility/versioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1245 2023-07-18 07:01:01.549566 ReFrame-HPC-4.3.2/setup.cfg
```

### Comparing `ReFrame-HPC-4.3.1/LICENSE` & `ReFrame-HPC-4.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/PKG-INFO` & `ReFrame-HPC-4.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.3.1
+Version: 4.3.2
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ReFrame-HPC-4.3.1/README.md` & `ReFrame-HPC-4.3.2/README.md`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/README_minimal.md` & `ReFrame-HPC-4.3.2/README_minimal.md`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/ReFrame_HPC.egg-info/PKG-INFO` & `ReFrame-HPC-4.3.2/ReFrame_HPC.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ReFrame-HPC
-Version: 4.3.1
+Version: 4.3.2
 Summary: ReFrame is a powerful framework for writing system regression tests and benchmarks, specifically targeted to HPC systems
 Home-page: https://github.com/reframe-hpc/reframe
 Author: Swiss National Supercomputing Center (CSCS/ETH Zurich), ReFrame Project Developers
 License: BSD 3-Clause
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `ReFrame-HPC-4.3.1/ReFrame_HPC.egg-info/SOURCES.txt` & `ReFrame-HPC-4.3.2/ReFrame_HPC.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/bin/reframe` & `ReFrame-HPC-4.3.2/bin/reframe`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/__init__.py` & `ReFrame-HPC-4.3.2/reframe/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 # ReFrame Project Developers. See the top-level LICENSE file for details.
 #
 # SPDX-License-Identifier: BSD-3-Clause
 
 import os
 import sys
 
-VERSION = '4.3.1'
+VERSION = '4.3.2'
 INSTALL_PREFIX = os.path.normpath(
     os.path.abspath(os.path.join(os.path.dirname(__file__), '..'))
 )
 MIN_PYTHON_VERSION = (3, 6, 0)
 
 # Check python version
 if sys.version_info[:3] < MIN_PYTHON_VERSION:
```

### Comparing `ReFrame-HPC-4.3.1/reframe/core/backends.py` & `ReFrame-HPC-4.3.2/reframe/core/backends.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/buildsystems.py` & `ReFrame-HPC-4.3.2/reframe/core/buildsystems.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/builtins.py` & `ReFrame-HPC-4.3.2/reframe/core/builtins.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/config.py` & `ReFrame-HPC-4.3.2/reframe/core/config.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/containers.py` & `ReFrame-HPC-4.3.2/reframe/core/containers.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/decorators.py` & `ReFrame-HPC-4.3.2/reframe/core/decorators.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/deferrable.py` & `ReFrame-HPC-4.3.2/reframe/core/deferrable.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/environments.py` & `ReFrame-HPC-4.3.2/reframe/core/environments.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/exceptions.py` & `ReFrame-HPC-4.3.2/reframe/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/fields.py` & `ReFrame-HPC-4.3.2/reframe/core/fields.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/fixtures.py` & `ReFrame-HPC-4.3.2/reframe/core/fixtures.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/hooks.py` & `ReFrame-HPC-4.3.2/reframe/core/hooks.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/launchers/__init__.py` & `ReFrame-HPC-4.3.2/reframe/core/launchers/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/launchers/local.py` & `ReFrame-HPC-4.3.2/reframe/core/launchers/local.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/launchers/mpi.py` & `ReFrame-HPC-4.3.2/reframe/core/launchers/mpi.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/launchers/rsh.py` & `ReFrame-HPC-4.3.2/reframe/core/launchers/rsh.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/logging.py` & `ReFrame-HPC-4.3.2/reframe/core/logging.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/meta.py` & `ReFrame-HPC-4.3.2/reframe/core/meta.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/modules.py` & `ReFrame-HPC-4.3.2/reframe/core/modules.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/namespaces.py` & `ReFrame-HPC-4.3.2/reframe/core/namespaces.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/parameters.py` & `ReFrame-HPC-4.3.2/reframe/core/parameters.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/pipeline.py` & `ReFrame-HPC-4.3.2/reframe/core/pipeline.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/runtime.py` & `ReFrame-HPC-4.3.2/reframe/core/runtime.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/schedulers/__init__.py` & `ReFrame-HPC-4.3.2/reframe/core/schedulers/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/schedulers/flux.py` & `ReFrame-HPC-4.3.2/reframe/core/schedulers/flux.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/schedulers/local.py` & `ReFrame-HPC-4.3.2/reframe/core/schedulers/local.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/schedulers/lsf.py` & `ReFrame-HPC-4.3.2/reframe/core/schedulers/lsf.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/schedulers/oar.py` & `ReFrame-HPC-4.3.2/reframe/core/schedulers/oar.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/schedulers/pbs.py` & `ReFrame-HPC-4.3.2/reframe/core/schedulers/pbs.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/schedulers/registry.py` & `ReFrame-HPC-4.3.2/reframe/core/schedulers/registry.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/schedulers/sge.py` & `ReFrame-HPC-4.3.2/reframe/core/schedulers/sge.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/schedulers/slurm.py` & `ReFrame-HPC-4.3.2/reframe/core/schedulers/slurm.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/settings.py` & `ReFrame-HPC-4.3.2/reframe/core/settings.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/shell.py` & `ReFrame-HPC-4.3.2/reframe/core/shell.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/systems.py` & `ReFrame-HPC-4.3.2/reframe/core/systems.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/variables.py` & `ReFrame-HPC-4.3.2/reframe/core/variables.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/core/warnings.py` & `ReFrame-HPC-4.3.2/reframe/core/warnings.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/frontend/argparse.py` & `ReFrame-HPC-4.3.2/reframe/frontend/argparse.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/frontend/autodetect.py` & `ReFrame-HPC-4.3.2/reframe/frontend/autodetect.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/frontend/ci.py` & `ReFrame-HPC-4.3.2/reframe/frontend/ci.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/frontend/cli.py` & `ReFrame-HPC-4.3.2/reframe/frontend/cli.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/frontend/dependencies.py` & `ReFrame-HPC-4.3.2/reframe/frontend/dependencies.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/frontend/executors/__init__.py` & `ReFrame-HPC-4.3.2/reframe/frontend/executors/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/frontend/executors/policies.py` & `ReFrame-HPC-4.3.2/reframe/frontend/executors/policies.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/frontend/filters.py` & `ReFrame-HPC-4.3.2/reframe/frontend/filters.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/frontend/loader.py` & `ReFrame-HPC-4.3.2/reframe/frontend/loader.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/frontend/printer.py` & `ReFrame-HPC-4.3.2/reframe/frontend/printer.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/frontend/runreport.py` & `ReFrame-HPC-4.3.2/reframe/frontend/runreport.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/frontend/statistics.py` & `ReFrame-HPC-4.3.2/reframe/frontend/statistics.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/frontend/testgenerators.py` & `ReFrame-HPC-4.3.2/reframe/frontend/testgenerators.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/schemas/config.json` & `ReFrame-HPC-4.3.2/reframe/schemas/config.json`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/schemas/junit.xsd` & `ReFrame-HPC-4.3.2/reframe/schemas/junit.xsd`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/schemas/runreport.json` & `ReFrame-HPC-4.3.2/reframe/schemas/runreport.json`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/utility/__init__.py` & `ReFrame-HPC-4.3.2/reframe/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/utility/color.py` & `ReFrame-HPC-4.3.2/reframe/utility/color.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/utility/cpuinfo.py` & `ReFrame-HPC-4.3.2/reframe/utility/cpuinfo.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/utility/jsonext.py` & `ReFrame-HPC-4.3.2/reframe/utility/jsonext.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/utility/osext.py` & `ReFrame-HPC-4.3.2/reframe/utility/osext.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/utility/profile.py` & `ReFrame-HPC-4.3.2/reframe/utility/profile.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/utility/sanity.py` & `ReFrame-HPC-4.3.2/reframe/utility/sanity.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/utility/typecheck.py` & `ReFrame-HPC-4.3.2/reframe/utility/typecheck.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/utility/udeps.py` & `ReFrame-HPC-4.3.2/reframe/utility/udeps.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/reframe/utility/versioning.py` & `ReFrame-HPC-4.3.2/reframe/utility/versioning.py`

 * *Files identical despite different names*

### Comparing `ReFrame-HPC-4.3.1/setup.cfg` & `ReFrame-HPC-4.3.2/setup.cfg`

 * *Files identical despite different names*

