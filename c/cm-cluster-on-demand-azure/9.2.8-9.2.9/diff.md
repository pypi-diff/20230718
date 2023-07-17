# Comparing `tmp/cm-cluster-on-demand-azure-9.2.8.tar.gz` & `tmp/cm-cluster-on-demand-azure-9.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm-cluster-on-demand-azure-9.2.8.tar", last modified: Tue Dec 27 18:19:28 2022, max compression
+gzip compressed data, was "cm-cluster-on-demand-azure-9.2.9.tar", last modified: Mon Feb 20 12:11:28 2023, max compression
```

## Comparing `cm-cluster-on-demand-azure-9.2.8.tar` & `cm-cluster-on-demand-azure-9.2.9.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:28.449311 cm-cluster-on-demand-azure-9.2.8/
--rw-r--r--   0 root         (0) root         (0)    11358 2022-12-27 18:19:08.000000 cm-cluster-on-demand-azure-9.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       83 2022-12-27 18:19:08.000000 cm-cluster-on-demand-azure-9.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1936 2022-12-27 18:19:28.445311 cm-cluster-on-demand-azure-9.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1023 2022-12-27 18:19:08.000000 cm-cluster-on-demand-azure-9.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:28.445311 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/
--rw-r--r--   0 root         (0) root         (0)      596 2022-12-27 18:19:08.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2022-12-27 18:19:27.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:28.445311 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/azure_actions/
--rw-r--r--   0 root         (0) root         (0)      596 2022-12-27 18:19:08.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/azure_actions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5906 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/azure_actions/credentials.py
--rw-r--r--   0 root         (0) root         (0)     8496 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/azure_actions/storage.py
--rw-r--r--   0 root         (0) root         (0)     5755 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/azure_actions/terms.py
--rw-r--r--   0 root         (0) root         (0)     2835 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/azure_actions/throttle.py
--rw-r--r--   0 root         (0) root         (0)     4817 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/base.py
--rw-r--r--   0 root         (0) root         (0)     3103 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/cli.py
--rw-r--r--   0 root         (0) root         (0)    37455 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/clustercreate.py
--rw-r--r--   0 root         (0) root         (0)    11184 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/clusterdelete.py
--rw-r--r--   0 root         (0) root         (0)     7794 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/clusterlist.py
--rw-r--r--   0 root         (0) root         (0)     1438 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/configdump.py
--rw-r--r--   0 root         (0) root         (0)     1450 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/configshow.py
--rw-r--r--   0 root         (0) root         (0)     1905 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/configuration.py
--rw-r--r--   0 root         (0) root         (0)     3145 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/constants.py
--rw-r--r--   0 root         (0) root         (0)     2516 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/eula.py
--rw-r--r--   0 root         (0) root         (0)     2158 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/imagelist.py
--rw-r--r--   0 root         (0) root         (0)     4938 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/images.py
--rw-r--r--   0 root         (0) root         (0)     1107 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/inbound_traffic_rule.py
--rw-r--r--   0 root         (0) root         (0)     1831 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/paramvalidation.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:28.445311 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/resources/
--rw-r--r--   0 root         (0) root         (0)      511 2022-12-27 18:19:08.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/resources/avset.json
--rw-r--r--   0 root         (0) root         (0)     1489 2022-12-27 18:19:08.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/resources/head-node-nic.json
--rw-r--r--   0 root         (0) root         (0)     2441 2022-12-27 18:19:08.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/resources/head-node.json
--rw-r--r--   0 root         (0) root         (0)      570 2022-12-27 18:19:08.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/resources/pub-ip.json
--rw-r--r--   0 root         (0) root         (0)      476 2022-12-27 18:19:08.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/resources/sec-group.json
--rw-r--r--   0 root         (0) root         (0)     1275 2022-12-27 18:19:08.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/resources/vpc.json
--rw-r--r--   0 root         (0) root         (0)     1951 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/summary.py
--rw-r--r--   0 root         (0) root         (0)     2706 2022-12-27 18:19:08.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/template.json
--rw-r--r--   0 root         (0) root         (0)     4341 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/template_builder.py
--rw-r--r--   0 root         (0) root         (0)     7113 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/vmsizelist.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:28.445311 cm-cluster-on-demand-azure-9.2.8/cm_cluster_on_demand_azure.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1936 2022-12-27 18:19:28.000000 cm-cluster-on-demand-azure-9.2.8/cm_cluster_on_demand_azure.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1540 2022-12-27 18:19:28.000000 cm-cluster-on-demand-azure-9.2.8/cm_cluster_on_demand_azure.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-27 18:19:28.000000 cm-cluster-on-demand-azure-9.2.8/cm_cluster_on_demand_azure.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       68 2022-12-27 18:19:28.000000 cm-cluster-on-demand-azure-9.2.8/cm_cluster_on_demand_azure.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      371 2022-12-27 18:19:28.000000 cm-cluster-on-demand-azure-9.2.8/cm_cluster_on_demand_azure.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2022-12-27 18:19:28.000000 cm-cluster-on-demand-azure-9.2.8/cm_cluster_on_demand_azure.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-27 18:19:28.449311 cm-cluster-on-demand-azure-9.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2990 2022-12-27 18:19:11.000000 cm-cluster-on-demand-azure-9.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:28.283678 cm-cluster-on-demand-azure-9.2.9/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-02-20 12:11:10.000000 cm-cluster-on-demand-azure-9.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       83 2023-02-20 12:11:10.000000 cm-cluster-on-demand-azure-9.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-02-20 12:11:28.283678 cm-cluster-on-demand-azure-9.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1023 2023-02-20 12:11:10.000000 cm-cluster-on-demand-azure-9.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:28.283678 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-02-20 12:11:10.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-02-20 12:11:27.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:28.283678 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/azure_actions/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-02-20 12:11:10.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/azure_actions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5906 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/azure_actions/credentials.py
+-rw-r--r--   0 root         (0) root         (0)     8496 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/azure_actions/storage.py
+-rw-r--r--   0 root         (0) root         (0)     5755 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/azure_actions/terms.py
+-rw-r--r--   0 root         (0) root         (0)     2835 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/azure_actions/throttle.py
+-rw-r--r--   0 root         (0) root         (0)     4817 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/base.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/cli.py
+-rw-r--r--   0 root         (0) root         (0)    37455 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/clustercreate.py
+-rw-r--r--   0 root         (0) root         (0)    11184 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/clusterdelete.py
+-rw-r--r--   0 root         (0) root         (0)     7794 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/clusterlist.py
+-rw-r--r--   0 root         (0) root         (0)     1438 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/configdump.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/configshow.py
+-rw-r--r--   0 root         (0) root         (0)     1905 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     3145 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/constants.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/eula.py
+-rw-r--r--   0 root         (0) root         (0)     2158 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/imagelist.py
+-rw-r--r--   0 root         (0) root         (0)     4938 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/images.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/inbound_traffic_rule.py
+-rw-r--r--   0 root         (0) root         (0)     1831 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/paramvalidation.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:28.283678 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/resources/
+-rw-r--r--   0 root         (0) root         (0)      511 2023-02-20 12:11:10.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/resources/avset.json
+-rw-r--r--   0 root         (0) root         (0)     1489 2023-02-20 12:11:10.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/resources/head-node-nic.json
+-rw-r--r--   0 root         (0) root         (0)     2441 2023-02-20 12:11:10.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/resources/head-node.json
+-rw-r--r--   0 root         (0) root         (0)      570 2023-02-20 12:11:10.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/resources/pub-ip.json
+-rw-r--r--   0 root         (0) root         (0)      476 2023-02-20 12:11:10.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/resources/sec-group.json
+-rw-r--r--   0 root         (0) root         (0)     1275 2023-02-20 12:11:10.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/resources/vpc.json
+-rw-r--r--   0 root         (0) root         (0)     1951 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/summary.py
+-rw-r--r--   0 root         (0) root         (0)     2706 2023-02-20 12:11:10.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/template.json
+-rw-r--r--   0 root         (0) root         (0)     4341 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/template_builder.py
+-rw-r--r--   0 root         (0) root         (0)     7113 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/vmsizelist.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:28.283678 cm-cluster-on-demand-azure-9.2.9/cm_cluster_on_demand_azure.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1936 2023-02-20 12:11:27.000000 cm-cluster-on-demand-azure-9.2.9/cm_cluster_on_demand_azure.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1540 2023-02-20 12:11:28.000000 cm-cluster-on-demand-azure-9.2.9/cm_cluster_on_demand_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-20 12:11:27.000000 cm-cluster-on-demand-azure-9.2.9/cm_cluster_on_demand_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       68 2023-02-20 12:11:27.000000 cm-cluster-on-demand-azure-9.2.9/cm_cluster_on_demand_azure.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      371 2023-02-20 12:11:27.000000 cm-cluster-on-demand-azure-9.2.9/cm_cluster_on_demand_azure.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2023-02-20 12:11:27.000000 cm-cluster-on-demand-azure-9.2.9/cm_cluster_on_demand_azure.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-20 12:11:28.283678 cm-cluster-on-demand-azure-9.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2990 2023-02-20 12:11:13.000000 cm-cluster-on-demand-azure-9.2.9/setup.py
```

### Comparing `cm-cluster-on-demand-azure-9.2.8/LICENSE` & `cm-cluster-on-demand-azure-9.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-azure-9.2.8/PKG-INFO` & `cm-cluster-on-demand-azure-9.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm-cluster-on-demand-azure
-Version: 9.2.8
+Version: 9.2.9
 Summary: Bright Cluster on Demand Azure
 Home-page: https://www.brightcomputing.com/
 Author: Cloudteam
 Author-email: cloudteam@brightcomputing.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cm-cluster-on-demand-azure-9.2.8/README.md` & `cm-cluster-on-demand-azure-9.2.9/README.md`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/__init__.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/__init__.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/azure_actions/__init__.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/azure_actions/__init__.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/azure_actions/credentials.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/azure_actions/credentials.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 #
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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/azure_actions/storage.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/azure_actions/storage.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/azure_actions/terms.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/azure_actions/terms.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/azure_actions/throttle.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/azure_actions/throttle.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/base.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/base.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/cli.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/cli.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/clustercreate.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/clustercreate.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/clusterdelete.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/clusterdelete.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/clusterlist.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/clusterlist.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/configdump.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/configdump.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/configshow.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/configshow.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/configuration.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/configuration.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/constants.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/constants.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/eula.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/eula.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/imagelist.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/imagelist.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/images.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/images.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/inbound_traffic_rule.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/inbound_traffic_rule.py`

 * *Files 2% similar despite different names*

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/paramvalidation.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/paramvalidation.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/resources/head-node-nic.json` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/resources/head-node-nic.json`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/resources/head-node.json` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/resources/head-node.json`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/resources/pub-ip.json` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/resources/pub-ip.json`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/resources/vpc.json` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/resources/vpc.json`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/summary.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/summary.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/template.json` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/template.json`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/template_builder.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/template_builder.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/clusterondemandazure/vmsizelist.py` & `cm-cluster-on-demand-azure-9.2.9/clusterondemandazure/vmsizelist.py`

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

### Comparing `cm-cluster-on-demand-azure-9.2.8/cm_cluster_on_demand_azure.egg-info/PKG-INFO` & `cm-cluster-on-demand-azure-9.2.9/cm_cluster_on_demand_azure.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm-cluster-on-demand-azure
-Version: 9.2.8
+Version: 9.2.9
 Summary: Bright Cluster on Demand Azure
 Home-page: https://www.brightcomputing.com/
 Author: Cloudteam
 Author-email: cloudteam@brightcomputing.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cm-cluster-on-demand-azure-9.2.8/cm_cluster_on_demand_azure.egg-info/SOURCES.txt` & `cm-cluster-on-demand-azure-9.2.9/cm_cluster_on_demand_azure.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-azure-9.2.8/setup.py` & `cm-cluster-on-demand-azure-9.2.9/setup.py`

 * *Files 2% similar despite different names*

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

