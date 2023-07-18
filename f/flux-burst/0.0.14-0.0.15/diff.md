# Comparing `tmp/flux-burst-0.0.14.tar.gz` & `tmp/flux-burst-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-burst-0.0.14.tar", last modified: Sat Jul 15 03:30:48 2023, max compression
+gzip compressed data, was "flux-burst-0.0.15.tar", last modified: Tue Jul 18 06:30:11 2023, max compression
```

## Comparing `flux-burst-0.0.14.tar` & `flux-burst-0.0.15.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-15 03:30:48.804137 flux-burst-0.0.14/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-23 19:26:31.000000 flux-burst-0.0.14/COPYRIGHT
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-23 19:26:31.000000 flux-burst-0.0.14/LICENSE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      313 2023-06-23 19:45:55.000000 flux-burst-0.0.14/MANIFEST.in
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-23 19:26:31.000000 flux-burst-0.0.14/NOTICE
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-15 03:30:48.804137 flux-burst-0.0.14/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3880 2023-07-03 07:21:31.000000 flux-burst-0.0.14/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-15 03:30:48.800137 flux-burst-0.0.14/flux_burst.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4718 2023-07-15 03:30:48.000000 flux-burst-0.0.14/flux_burst.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      744 2023-07-15 03:30:48.000000 flux-burst-0.0.14/flux_burst.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-15 03:30:48.000000 flux-burst-0.0.14/flux_burst.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2023-07-15 03:30:48.000000 flux-burst-0.0.14/flux_burst.egg-info/entry_points.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:17:14.000000 flux-burst-0.0.14/flux_burst.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      167 2023-07-15 03:30:48.000000 flux-burst-0.0.14/flux_burst.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       10 2023-07-15 03:30:48.000000 flux-burst-0.0.14/flux_burst.egg-info/top_level.txt
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-15 03:30:48.804137 flux-burst-0.0.14/fluxburst/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       62 2023-06-23 19:45:55.000000 flux-burst-0.0.14/fluxburst/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8590 2023-07-04 01:36:48.000000 flux-burst-0.0.14/fluxburst/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      746 2023-07-01 06:52:00.000000 flux-burst-0.0.14/fluxburst/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7850 2023-07-15 03:29:48.000000 flux-burst-0.0.14/fluxburst/handles.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-15 03:30:48.804137 flux-burst-0.0.14/fluxburst/kubernetes/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      209 2023-07-01 06:52:00.000000 flux-burst-0.0.14/fluxburst/kubernetes/README.md
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-07-01 06:52:00.000000 flux-burst-0.0.14/fluxburst/kubernetes/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5200 2023-07-04 01:36:48.000000 flux-burst-0.0.14/fluxburst/kubernetes/cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8953 2023-07-09 17:00:01.000000 flux-burst-0.0.14/fluxburst/kubernetes/plugins.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6127 2023-06-23 19:43:36.000000 flux-burst-0.0.14/fluxburst/logger.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2831 2023-07-04 00:51:56.000000 flux-burst-0.0.14/fluxburst/plugins.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      365 2023-07-09 16:49:50.000000 flux-burst-0.0.14/fluxburst/selectors.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      444 2023-06-24 04:45:23.000000 flux-burst-0.0.14/fluxburst/sorting.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-15 03:30:48.804137 flux-burst-0.0.14/fluxburst/utils/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      532 2023-07-15 03:29:48.000000 flux-burst-0.0.14/fluxburst/utils/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6250 2023-07-04 01:36:48.000000 flux-burst-0.0.14/fluxburst/utils/fileio.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1456 2023-07-15 03:29:48.000000 flux-burst-0.0.14/fluxburst/utils/misc.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3188 2023-06-23 19:45:55.000000 flux-burst-0.0.14/fluxburst/utils/terminal.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-07-15 03:30:11.000000 flux-burst-0.0.14/fluxburst/version.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 19:26:31.000000 flux-burst-0.0.14/pyproject.toml
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      210 2023-07-15 03:30:48.804137 flux-burst-0.0.14/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3578 2023-07-01 06:52:00.000000 flux-burst-0.0.14/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-18 06:30:11.944831 flux-burst-0.0.15/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      498 2023-06-23 19:26:31.000000 flux-burst-0.0.15/COPYRIGHT
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1108 2023-06-23 19:26:31.000000 flux-burst-0.0.15/LICENSE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      313 2023-06-23 19:45:55.000000 flux-burst-0.0.15/MANIFEST.in
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1167 2023-06-23 19:26:31.000000 flux-burst-0.0.15/NOTICE
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4981 2023-07-18 06:30:11.944831 flux-burst-0.0.15/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4143 2023-07-18 06:29:24.000000 flux-burst-0.0.15/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-18 06:30:11.944831 flux-burst-0.0.15/flux_burst.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4981 2023-07-18 06:30:11.000000 flux-burst-0.0.15/flux_burst.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      744 2023-07-18 06:30:11.000000 flux-burst-0.0.15/flux_burst.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-07-18 06:30:11.000000 flux-burst-0.0.15/flux_burst.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       53 2023-07-18 06:30:11.000000 flux-burst-0.0.15/flux_burst.egg-info/entry_points.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-06-25 03:17:14.000000 flux-burst-0.0.15/flux_burst.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      115 2023-07-18 06:30:11.000000 flux-burst-0.0.15/flux_burst.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       10 2023-07-18 06:30:11.000000 flux-burst-0.0.15/flux_burst.egg-info/top_level.txt
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-18 06:30:11.944831 flux-burst-0.0.15/fluxburst/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       62 2023-06-23 19:45:55.000000 flux-burst-0.0.15/fluxburst/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10044 2023-07-18 06:29:24.000000 flux-burst-0.0.15/fluxburst/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      746 2023-07-01 06:52:00.000000 flux-burst-0.0.15/fluxburst/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8599 2023-07-18 06:29:24.000000 flux-burst-0.0.15/fluxburst/handles.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-18 06:30:11.944831 flux-burst-0.0.15/fluxburst/kubernetes/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      209 2023-07-01 06:52:00.000000 flux-burst-0.0.15/fluxburst/kubernetes/README.md
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       43 2023-07-01 06:52:00.000000 flux-burst-0.0.15/fluxburst/kubernetes/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5200 2023-07-04 01:36:48.000000 flux-burst-0.0.15/fluxburst/kubernetes/cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8953 2023-07-09 17:00:01.000000 flux-burst-0.0.15/fluxburst/kubernetes/plugins.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6127 2023-06-23 19:43:36.000000 flux-burst-0.0.15/fluxburst/logger.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2831 2023-07-04 00:51:56.000000 flux-burst-0.0.15/fluxburst/plugins.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      365 2023-07-09 16:49:50.000000 flux-burst-0.0.15/fluxburst/selectors.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      444 2023-06-24 04:45:23.000000 flux-burst-0.0.15/fluxburst/sorting.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-07-18 06:30:11.944831 flux-burst-0.0.15/fluxburst/utils/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      532 2023-07-15 03:29:48.000000 flux-burst-0.0.15/fluxburst/utils/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6100 2023-07-18 06:29:24.000000 flux-burst-0.0.15/fluxburst/utils/fileio.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1456 2023-07-15 03:29:48.000000 flux-burst-0.0.15/fluxburst/utils/misc.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3188 2023-06-23 19:45:55.000000 flux-burst-0.0.15/fluxburst/utils/terminal.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1098 2023-07-18 06:30:07.000000 flux-burst-0.0.15/fluxburst/version.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      132 2023-06-23 19:26:31.000000 flux-burst-0.0.15/pyproject.toml
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      210 2023-07-18 06:30:11.944831 flux-burst-0.0.15/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3578 2023-07-01 06:52:00.000000 flux-burst-0.0.15/setup.py
```

### Comparing `flux-burst-0.0.14/LICENSE` & `flux-burst-0.0.15/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.14/NOTICE` & `flux-burst-0.0.15/NOTICE`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.14/PKG-INFO` & `flux-burst-0.0.15/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst
-Version: 0.0.14
+Version: 0.0.15
 Summary: Flux module that enables burstable plugins.
 Home-page: https://github.com/converged-computing/flux-burst
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting
@@ -42,17 +42,18 @@
  - 📦️ [Pypi Package](https://pypi.org/project/flux-burst/) 📦️
 
 
 ## Plugins
 
 Current and desired plugins are:
 
- - [local mock](https://github.com/flux-framework/flux-sched/issues/1009#issuecomment-1603636498)
- - [Google Cloud](https://github.com/converged-computing/flux-burst-gke)
- - AWS (not written yet)
+ - [flux-burst-local](https://github.com/converged-computing/flux-burst-local) to "burst" on a local HPC system
+ - [flux-burst-gke](https://github.com/converged-computing/flux-burst-gke) to burst to Google Kubernetes Engine
+ - [flux-burst-eks](https://github.com/converged-computing/flux-burst-eks) to burst to Amazon EKS
+ - [flux-burst-compute-engine](https://github.com/converged-computing/flux-burst-compute-engine) to burst to Google Cloud Compute Engine
 
 ## Questions
 
 - How should the plugins (or client) manage checking when to create / destroy clusters?
 - Can we have a better strategy for namespacing different bursts (e.g., beyond burst-0, burst-1, ..., burst-N)
 - We need a reasonable default for what a plugin should do if something fails (e.g., setup/config)
 - How should each plugin decide what size cluster to make? Right now I'm just taking the max size of the job, and we are assuming the jobs need the same node type.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flux-burst Version: 0.0.14 Summary: Flux module
+Metadata-Version: 2.1 Name: flux-burst Version: 0.0.15 Summary: Flux module
 that enables burstable plugins. Home-page: https://github.com/converged-
 computing/flux-burst Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting Platform: UNKNOWN Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
@@ -14,36 +14,40 @@
 (#contributors-)  [![PyPI](https://img.shields.io/pypi/v/flux-burst)](https://
 pypi.org/project/flux-burst/)  ![https://raw.githubusercontent.com/converged-
 computing/flux-burst/main/docs/assets/img/logo.png](https://
 raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/
 logo.png) This is a Python module to coordinate Flux bursting. ð§ï¸ - â­ï¸
 [Documentation](https://converged-computing.github.io/flux-burst/) â­ï¸ -
 ð¦ï¸ [Pypi Package](https://pypi.org/project/flux-burst/) ð¦ï¸ ## Plugins
-Current and desired plugins are: - [local mock](https://github.com/flux-
-framework/flux-sched/issues/1009#issuecomment-1603636498) - [Google Cloud]
-(https://github.com/converged-computing/flux-burst-gke) - AWS (not written yet)
-## Questions - How should the plugins (or client) manage checking when to
-create / destroy clusters? - Can we have a better strategy for namespacing
-different bursts (e.g., beyond burst-0, burst-1, ..., burst-N) - We need a
-reasonable default for what a plugin should do if something fails (e.g., setup/
-config) - How should each plugin decide what size cluster to make? Right now
-I'm just taking the max size of the job, and we are assuming the jobs need the
-same node type. - We will eventually want to use namespaces in a meaningful way
-(e.g., users) - We will eventually want a specific burst for a job to be able
-to customize in more detail, e.g., the namespace or other attribute that comes
-from a jobspec (right now they are global to the plugin) - Who controls
-cleanup? It can be done by the flux-burst global controller or a plugin,
-automated or manual, either way. - All plugins should have support to read in
-YAML parameters (some spec for bursting) - All plugins should be able to match
-a resource request to, for example, instance types. - Should the plugin "local
-queue" (self.jobs) assume to be associated with one burst, where the size is
-the max job size? - Should we derive names based on provided name + size so
-clusters are unique by name and size? ## ðï¸ Contributors ðï¸ We use
-the [all-contributors](https://github.com/all-contributors/all-contributors)
-tool to generate a contributors graphic below.
+Current and desired plugins are: - [flux-burst-local](https://github.com/
+converged-computing/flux-burst-local) to "burst" on a local HPC system - [flux-
+burst-gke](https://github.com/converged-computing/flux-burst-gke) to burst to
+Google Kubernetes Engine - [flux-burst-eks](https://github.com/converged-
+computing/flux-burst-eks) to burst to Amazon EKS - [flux-burst-compute-engine]
+(https://github.com/converged-computing/flux-burst-compute-engine) to burst to
+Google Cloud Compute Engine ## Questions - How should the plugins (or client)
+manage checking when to create / destroy clusters? - Can we have a better
+strategy for namespacing different bursts (e.g., beyond burst-0, burst-1, ...,
+burst-N) - We need a reasonable default for what a plugin should do if
+something fails (e.g., setup/config) - How should each plugin decide what size
+cluster to make? Right now I'm just taking the max size of the job, and we are
+assuming the jobs need the same node type. - We will eventually want to use
+namespaces in a meaningful way (e.g., users) - We will eventually want a
+specific burst for a job to be able to customize in more detail, e.g., the
+namespace or other attribute that comes from a jobspec (right now they are
+global to the plugin) - Who controls cleanup? It can be done by the flux-burst
+global controller or a plugin, automated or manual, either way. - All plugins
+should have support to read in YAML parameters (some spec for bursting) - All
+plugins should be able to match a resource request to, for example, instance
+types. - Should the plugin "local queue" (self.jobs) assume to be associated
+with one burst, where the size is the max job size? - Should we derive names
+based on provided name + size so clusters are unique by name and size? ##
+ðï¸ Contributors ðï¸ We use the [all-contributors](https://github.com/
+all-contributors/all-contributors) tool to generate a contributors graphic
+below.
 [Vanessasaurus]
  Vanessasaurus
      ð»
    ## License HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license. See [LICENSE](https://
 github.com/converged-computing/flux-burst/blob/main/LICENSE), [COPYRIGHT]
 (https://github.com/converged-computing/flux-burst/blob/main/COPYRIGHT), and
```

### Comparing `flux-burst-0.0.14/README.md` & `flux-burst-0.0.15/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -17,17 +17,18 @@
  - 📦️ [Pypi Package](https://pypi.org/project/flux-burst/) 📦️
 
 
 ## Plugins
 
 Current and desired plugins are:
 
- - [local mock](https://github.com/flux-framework/flux-sched/issues/1009#issuecomment-1603636498)
- - [Google Cloud](https://github.com/converged-computing/flux-burst-gke)
- - AWS (not written yet)
+ - [flux-burst-local](https://github.com/converged-computing/flux-burst-local) to "burst" on a local HPC system
+ - [flux-burst-gke](https://github.com/converged-computing/flux-burst-gke) to burst to Google Kubernetes Engine
+ - [flux-burst-eks](https://github.com/converged-computing/flux-burst-eks) to burst to Amazon EKS
+ - [flux-burst-compute-engine](https://github.com/converged-computing/flux-burst-compute-engine) to burst to Google Cloud Compute Engine
 
 ## Questions
 
 - How should the plugins (or client) manage checking when to create / destroy clusters?
 - Can we have a better strategy for namespacing different bursts (e.g., beyond burst-0, burst-1, ..., burst-N)
 - We need a reasonable default for what a plugin should do if something fails (e.g., setup/config)
 - How should each plugin decide what size cluster to make? Right now I'm just taking the max size of the job, and we are assuming the jobs need the same node type.
```

#### html2text {}

```diff
@@ -3,36 +3,39 @@
 (https://img.shields.io/pypi/v/flux-burst)](https://pypi.org/project/flux-
 burst/)  ![https://raw.githubusercontent.com/converged-computing/flux-burst/
 main/docs/assets/img/logo.png](https://raw.githubusercontent.com/converged-
 computing/flux-burst/main/docs/assets/img/logo.png) This is a Python module to
 coordinate Flux bursting. ð§ï¸ - â­ï¸ [Documentation](https://converged-
 computing.github.io/flux-burst/) â­ï¸ - ð¦ï¸ [Pypi Package](https://
 pypi.org/project/flux-burst/) ð¦ï¸ ## Plugins Current and desired plugins
-are: - [local mock](https://github.com/flux-framework/flux-sched/issues/
-1009#issuecomment-1603636498) - [Google Cloud](https://github.com/converged-
-computing/flux-burst-gke) - AWS (not written yet) ## Questions - How should the
-plugins (or client) manage checking when to create / destroy clusters? - Can we
-have a better strategy for namespacing different bursts (e.g., beyond burst-0,
-burst-1, ..., burst-N) - We need a reasonable default for what a plugin should
-do if something fails (e.g., setup/config) - How should each plugin decide what
-size cluster to make? Right now I'm just taking the max size of the job, and we
-are assuming the jobs need the same node type. - We will eventually want to use
-namespaces in a meaningful way (e.g., users) - We will eventually want a
-specific burst for a job to be able to customize in more detail, e.g., the
-namespace or other attribute that comes from a jobspec (right now they are
-global to the plugin) - Who controls cleanup? It can be done by the flux-burst
-global controller or a plugin, automated or manual, either way. - All plugins
-should have support to read in YAML parameters (some spec for bursting) - All
-plugins should be able to match a resource request to, for example, instance
-types. - Should the plugin "local queue" (self.jobs) assume to be associated
-with one burst, where the size is the max job size? - Should we derive names
-based on provided name + size so clusters are unique by name and size? ##
-ðï¸ Contributors ðï¸ We use the [all-contributors](https://github.com/
-all-contributors/all-contributors) tool to generate a contributors graphic
-below.
+are: - [flux-burst-local](https://github.com/converged-computing/flux-burst-
+local) to "burst" on a local HPC system - [flux-burst-gke](https://github.com/
+converged-computing/flux-burst-gke) to burst to Google Kubernetes Engine -
+[flux-burst-eks](https://github.com/converged-computing/flux-burst-eks) to
+burst to Amazon EKS - [flux-burst-compute-engine](https://github.com/converged-
+computing/flux-burst-compute-engine) to burst to Google Cloud Compute Engine ##
+Questions - How should the plugins (or client) manage checking when to create /
+destroy clusters? - Can we have a better strategy for namespacing different
+bursts (e.g., beyond burst-0, burst-1, ..., burst-N) - We need a reasonable
+default for what a plugin should do if something fails (e.g., setup/config) -
+How should each plugin decide what size cluster to make? Right now I'm just
+taking the max size of the job, and we are assuming the jobs need the same node
+type. - We will eventually want to use namespaces in a meaningful way (e.g.,
+users) - We will eventually want a specific burst for a job to be able to
+customize in more detail, e.g., the namespace or other attribute that comes
+from a jobspec (right now they are global to the plugin) - Who controls
+cleanup? It can be done by the flux-burst global controller or a plugin,
+automated or manual, either way. - All plugins should have support to read in
+YAML parameters (some spec for bursting) - All plugins should be able to match
+a resource request to, for example, instance types. - Should the plugin "local
+queue" (self.jobs) assume to be associated with one burst, where the size is
+the max job size? - Should we derive names based on provided name + size so
+clusters are unique by name and size? ## ðï¸ Contributors ðï¸ We use
+the [all-contributors](https://github.com/all-contributors/all-contributors)
+tool to generate a contributors graphic below.
 [Vanessasaurus]
  Vanessasaurus
      ð»
    ## License HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license. See [LICENSE](https://
 github.com/converged-computing/flux-burst/blob/main/LICENSE), [COPYRIGHT]
 (https://github.com/converged-computing/flux-burst/blob/main/COPYRIGHT), and
```

### Comparing `flux-burst-0.0.14/flux_burst.egg-info/PKG-INFO` & `flux-burst-0.0.15/flux_burst.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-burst
-Version: 0.0.14
+Version: 0.0.15
 Summary: Flux module that enables burstable plugins.
 Home-page: https://github.com/converged-computing/flux-burst
 Author: Vanessa Sochat
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessa Sochat
 License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting
@@ -42,17 +42,18 @@
  - 📦️ [Pypi Package](https://pypi.org/project/flux-burst/) 📦️
 
 
 ## Plugins
 
 Current and desired plugins are:
 
- - [local mock](https://github.com/flux-framework/flux-sched/issues/1009#issuecomment-1603636498)
- - [Google Cloud](https://github.com/converged-computing/flux-burst-gke)
- - AWS (not written yet)
+ - [flux-burst-local](https://github.com/converged-computing/flux-burst-local) to "burst" on a local HPC system
+ - [flux-burst-gke](https://github.com/converged-computing/flux-burst-gke) to burst to Google Kubernetes Engine
+ - [flux-burst-eks](https://github.com/converged-computing/flux-burst-eks) to burst to Amazon EKS
+ - [flux-burst-compute-engine](https://github.com/converged-computing/flux-burst-compute-engine) to burst to Google Cloud Compute Engine
 
 ## Questions
 
 - How should the plugins (or client) manage checking when to create / destroy clusters?
 - Can we have a better strategy for namespacing different bursts (e.g., beyond burst-0, burst-1, ..., burst-N)
 - We need a reasonable default for what a plugin should do if something fails (e.g., setup/config)
 - How should each plugin decide what size cluster to make? Right now I'm just taking the max size of the job, and we are assuming the jobs need the same node type.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: flux-burst Version: 0.0.14 Summary: Flux module
+Metadata-Version: 2.1 Name: flux-burst Version: 0.0.15 Summary: Flux module
 that enables burstable plugins. Home-page: https://github.com/converged-
 computing/flux-burst Author: Vanessa Sochat Author-email:
 vsoch@users.noreply.github.com Maintainer: Vanessa Sochat License: LICENSE
 Keywords: cloud,flux-framework,flux,bursting Platform: UNKNOWN Classifier:
 Intended Audience :: Science/Research Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: MIT License Classifier:
 Programming Language :: Python Classifier: Topic :: Software Development
@@ -14,36 +14,40 @@
 (#contributors-)  [![PyPI](https://img.shields.io/pypi/v/flux-burst)](https://
 pypi.org/project/flux-burst/)  ![https://raw.githubusercontent.com/converged-
 computing/flux-burst/main/docs/assets/img/logo.png](https://
 raw.githubusercontent.com/converged-computing/flux-burst/main/docs/assets/img/
 logo.png) This is a Python module to coordinate Flux bursting. ð§ï¸ - â­ï¸
 [Documentation](https://converged-computing.github.io/flux-burst/) â­ï¸ -
 ð¦ï¸ [Pypi Package](https://pypi.org/project/flux-burst/) ð¦ï¸ ## Plugins
-Current and desired plugins are: - [local mock](https://github.com/flux-
-framework/flux-sched/issues/1009#issuecomment-1603636498) - [Google Cloud]
-(https://github.com/converged-computing/flux-burst-gke) - AWS (not written yet)
-## Questions - How should the plugins (or client) manage checking when to
-create / destroy clusters? - Can we have a better strategy for namespacing
-different bursts (e.g., beyond burst-0, burst-1, ..., burst-N) - We need a
-reasonable default for what a plugin should do if something fails (e.g., setup/
-config) - How should each plugin decide what size cluster to make? Right now
-I'm just taking the max size of the job, and we are assuming the jobs need the
-same node type. - We will eventually want to use namespaces in a meaningful way
-(e.g., users) - We will eventually want a specific burst for a job to be able
-to customize in more detail, e.g., the namespace or other attribute that comes
-from a jobspec (right now they are global to the plugin) - Who controls
-cleanup? It can be done by the flux-burst global controller or a plugin,
-automated or manual, either way. - All plugins should have support to read in
-YAML parameters (some spec for bursting) - All plugins should be able to match
-a resource request to, for example, instance types. - Should the plugin "local
-queue" (self.jobs) assume to be associated with one burst, where the size is
-the max job size? - Should we derive names based on provided name + size so
-clusters are unique by name and size? ## ðï¸ Contributors ðï¸ We use
-the [all-contributors](https://github.com/all-contributors/all-contributors)
-tool to generate a contributors graphic below.
+Current and desired plugins are: - [flux-burst-local](https://github.com/
+converged-computing/flux-burst-local) to "burst" on a local HPC system - [flux-
+burst-gke](https://github.com/converged-computing/flux-burst-gke) to burst to
+Google Kubernetes Engine - [flux-burst-eks](https://github.com/converged-
+computing/flux-burst-eks) to burst to Amazon EKS - [flux-burst-compute-engine]
+(https://github.com/converged-computing/flux-burst-compute-engine) to burst to
+Google Cloud Compute Engine ## Questions - How should the plugins (or client)
+manage checking when to create / destroy clusters? - Can we have a better
+strategy for namespacing different bursts (e.g., beyond burst-0, burst-1, ...,
+burst-N) - We need a reasonable default for what a plugin should do if
+something fails (e.g., setup/config) - How should each plugin decide what size
+cluster to make? Right now I'm just taking the max size of the job, and we are
+assuming the jobs need the same node type. - We will eventually want to use
+namespaces in a meaningful way (e.g., users) - We will eventually want a
+specific burst for a job to be able to customize in more detail, e.g., the
+namespace or other attribute that comes from a jobspec (right now they are
+global to the plugin) - Who controls cleanup? It can be done by the flux-burst
+global controller or a plugin, automated or manual, either way. - All plugins
+should have support to read in YAML parameters (some spec for bursting) - All
+plugins should be able to match a resource request to, for example, instance
+types. - Should the plugin "local queue" (self.jobs) assume to be associated
+with one burst, where the size is the max job size? - Should we derive names
+based on provided name + size so clusters are unique by name and size? ##
+ðï¸ Contributors ðï¸ We use the [all-contributors](https://github.com/
+all-contributors/all-contributors) tool to generate a contributors graphic
+below.
 [Vanessasaurus]
  Vanessasaurus
      ð»
    ## License HPCIC DevTools is distributed under the terms of the MIT license.
 All new contributions must be made under this license. See [LICENSE](https://
 github.com/converged-computing/flux-burst/blob/main/LICENSE), [COPYRIGHT]
 (https://github.com/converged-computing/flux-burst/blob/main/COPYRIGHT), and
```

### Comparing `flux-burst-0.0.14/flux_burst.egg-info/SOURCES.txt` & `flux-burst-0.0.15/flux_burst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.14/fluxburst/client.py` & `flux-burst-0.0.15/fluxburst/client.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
 import collections
+import time
 
 import fluxburst.handles as handles
 import fluxburst.selectors as selectors
 import fluxburst.sorting as sorting
-from fluxburst.logger import logger
+from fluxburst.logger import setup_logger
 
 from .plugins import burstable_plugins
 
+setup_logger(quiet=False, debug=True)
+from fluxburst.logger import logger  # noqa
+
 
 class FluxBurst:
     """
     Flux Burst Client
     """
 
     def __init__(self, handle=None, mock=False, validate=True):
@@ -105,27 +109,68 @@
 
     def reset_plugins(self):
         self.plugins = collections.OrderedDict()
 
     def reset_selector(self):
         self._job_selector = selectors.is_burstable
 
+    def list_jobs(self):
+        """
+        Get all job ids in the instance.
+        """
+        listing = self.flux.list_jobs()
+        return [job["id"] for job in listing.get("jobs", [])]
+
+    def wait_for_jobs(self, jobids=None, states=None):
+        """
+        Wait for jobs to reach one or more states.
+        """
+        jobids = list(set(jobids or self.list_jobs()))
+        logger.debug(f"Waiting for {len(jobids)} to be done")
+
+        # Assume we allow jobs to complete or fail
+        states = states or ["INACTIVE"]
+
+        while jobids:
+            jobid = jobids.pop(0)
+            state = self.flux.state(jobid)
+            logger.debug(f"Job {jobid} is in state {state}")
+            if state not in states:
+                jobids.append(jobid)
+            time.sleep(5)
+            logger.debug(f"Waiting for {len(jobids)} to be done")
+
+    def run_unburst(self):
+        """
+        Given a plugin has an unburst function, run it.
+        """
+        # When we get here, undo the bursts
+        # It assumes all jobs are done
+        for _, plugin in self.iter_plugins():
+            if not hasattr(plugin, "unburst"):
+                continue
+            plugin.unburst()
+
     def run_burst(self, request_burst=False, nodes=None, tasks=None):
         """
         A full run burst includes:
 
         1. Selecting jobs using the client filter(s)
         2. In the order of plugins desired, schedule jobs
         3. Return back lookup of scheduled (by plugin)
 
         If request_burst with nodes and tasks are required, each plugin
         will simply request creation for the size/tasks needed.
         """
         # TODO what to do with unmatched jobs?
-        unmatched = self.process_queue()
+        unmatched, has_jobs = self.process_queue()
+
+        # Cut out early if no jobs
+        if not has_jobs:
+            return unmatched
 
         # When we get here, run the bursts
         for _, plugin in self.iter_plugins():
             plugin.run(request_burst=request_burst, nodes=nodes, tasks=tasks)
         return unmatched
 
     def request_burst(self, name, nodes, tasks):
@@ -164,14 +209,16 @@
         We first apply any selectors to the queue, and then hand the
         resulting filtered jobs off to burstable plugins. There could be
         more fine-tuned logic for directing jobs to plugins.
         """
         # Run filters across queue to select jobs
         # This is a dict, keys with job id, values jobinfo
         jobs = self.select_jobs()
+        if not jobs:
+            return [], False
 
         # Going through plugins, determine if matches and can run
         unmatched = []
         for _, job in jobs.items():
             scheduled = False
             for _, plugin in self.iter_plugins():
                 # Give to first burstable plugin that can accept
@@ -184,15 +231,15 @@
 
             # But if we cannot match, return to caller
             if not scheduled:
                 unmatched.append(job)
 
         if unmatched:
             logger.warning(f"There are {len(unmatched)} jobs that cannot be bursted.")
-        return unmatched
+        return unmatched, True
 
     def mark_as_scheduled(self, job, plugin_name):
         """
         Mark a job as scheduled.
 
         For now, we just remove the burstable attribute to indicate
         that it's been scheduled. We also add the plugin it was scheduled
```

### Comparing `flux-burst-0.0.14/fluxburst/defaults.py` & `flux-burst-0.0.15/fluxburst/defaults.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.14/fluxburst/handles.py` & `flux-burst-0.0.15/fluxburst/handles.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,22 +13,26 @@
     A mock flux handle that will return fake jobs, etc.
 
     This class does not require importing Flux and can be used
     for testing cases or similar.
     """
 
     def __init__(self, *args, **kwargs):
-        pass
+        # Default state to return
+        self.job_state = kwargs.get("state") or "INACTIVE"
 
     def update_jobspec(self, job):
         """
         Update a jobspec via the kvs
         """
         pass
 
+    def state(self, jobid):
+        return self.job_state
+
     def list_jobs(self):
         """
         List one fake, burstable job.
 
         Generated via:
         flux submit -N 4 --cwd /tmp --setattr=burstable hostname
         in the fluxrm/flux-sched:focal container on July 2nd 2023. Note that we
@@ -189,14 +193,34 @@
         """
         import flux
 
         if not self._handle:
             self._handle = flux.Flux()
         return self._handle
 
+    def state(self, jobid):
+        """
+        Get the state (string) for a jobid
+        """
+        import flux.job
+
+        jobid = flux.job.JobID(jobid)
+        payload = {"id": jobid, "attrs": ["all"]}
+        rpc = flux.job.list.JobListIdRPC(self.handle, "job-list.list-id", payload)
+        try:
+            jobinfo = rpc.get()
+        # The job does not exist, assume completed
+        except FileNotFoundError:
+            return "INACTIVE"
+
+        # User friendly string from integer
+        jobinfo = jobinfo["job"]
+        state = jobinfo["state"]
+        return flux.job.info.statetostr(state)
+
     def update_jobspec(self, job):
         """
         Update a jobspec via the kvs
         """
         import flux.job
 
         # This is a workaround because updating the attribute directly
```

### Comparing `flux-burst-0.0.14/fluxburst/kubernetes/cluster.py` & `flux-burst-0.0.15/fluxburst/kubernetes/cluster.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.14/fluxburst/kubernetes/plugins.py` & `flux-burst-0.0.15/fluxburst/kubernetes/plugins.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.14/fluxburst/logger.py` & `flux-burst-0.0.15/fluxburst/logger.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.14/fluxburst/plugins.py` & `flux-burst-0.0.15/fluxburst/plugins.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.14/fluxburst/utils/__init__.py` & `flux-burst-0.0.15/fluxburst/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.14/fluxburst/utils/fileio.py` & `flux-burst-0.0.15/fluxburst/utils/fileio.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,17 @@
 import os
 import re
 import shutil
 import stat
 import tempfile
 from contextlib import contextmanager
 
-from fluxburst.logger import logger
+import yaml
 
-try:
-    from ruamel_yaml import YAML
-except ImportError:
-    from ruamel.yaml import YAML
+from fluxburst.logger import logger
 
 
 @contextmanager
 def workdir(dirname):
     """
     Provide context for a working directory, e.g.,
 
@@ -217,28 +214,24 @@
     return json.dumps(json_obj, indent=4, separators=(",", ": "), cls=cls)
 
 
 def write_yaml(obj, filename):
     """
     Save yaml to file, also preserving comments.
     """
-    yaml = YAML()
-    yaml.preserve_quotes = True
-
     with open(filename, "w") as fd:
         yaml.dump(obj, fd)
 
 
 def read_yaml(filename):
     """
     Load a yaml from file, roundtrip to preserve comments
     """
-    yaml = YAML()
     with open(filename, "r") as fd:
-        content = yaml.load(fd.read())
+        content = yaml.safe_load(fd)
     return content
 
 
 def read_file(filename, mode="r"):
     """
     Read a file.
     """
```

### Comparing `flux-burst-0.0.14/fluxburst/utils/misc.py` & `flux-burst-0.0.15/fluxburst/utils/misc.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.14/fluxburst/utils/terminal.py` & `flux-burst-0.0.15/fluxburst/utils/terminal.py`

 * *Files identical despite different names*

### Comparing `flux-burst-0.0.14/fluxburst/version.py` & `flux-burst-0.0.15/fluxburst/version.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,35 +1,30 @@
 # Copyright 2023 Lawrence Livermore National Security, LLC and other
 # HPCIC DevTools Developers. See the top-level COPYRIGHT file for details.
 #
 # SPDX-License-Identifier: (MIT)
 
-__version__ = "0.0.14"
+__version__ = "0.0.15"
 AUTHOR = "Vanessa Sochat"
 EMAIL = "vsoch@users.noreply.github.com"
 NAME = "flux-burst"
 PACKAGE_URL = "https://github.com/converged-computing/flux-burst"
 KEYWORDS = "cloud, flux-framework, flux, bursting"
 DESCRIPTION = "Flux module that enables burstable plugins."
 LICENSE = "LICENSE"
 
 ################################################################################
 # Global requirements
 
-INSTALL_REQUIRES = (
-    ("ruamel.yaml", {"min_version": None}),
-    ("jsonschema", {"min_version": None}),
-    ("rich", {"min_version": None}),
-    ("oras", {"min_version": None}),
-    ("requests", {"min_version": None}),
-)
+INSTALL_REQUIRES = (("pyyaml", {"min_version": None}),)
 
 INSTALL_REQUIRES_KUBERNETES = (
     ("kubernetes", {"min_version": None}),
     ("fluxoperator", {"min_version": None}),
+    ("requests", {"min_version": None}),
 )
 
 TESTS_REQUIRES = (("pytest", {"min_version": "4.6.2"}),)
 
 ################################################################################
 # Submodule Requirements (versions that include database)
```

### Comparing `flux-burst-0.0.14/setup.py` & `flux-burst-0.0.15/setup.py`

 * *Files identical despite different names*

