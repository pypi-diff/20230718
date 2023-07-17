# Comparing `tmp/cm-cluster-on-demand-aws-9.2.8.tar.gz` & `tmp/cm-cluster-on-demand-aws-9.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cm-cluster-on-demand-aws-9.2.8.tar", last modified: Tue Dec 27 18:19:27 2022, max compression
+gzip compressed data, was "cm-cluster-on-demand-aws-9.2.9.tar", last modified: Mon Feb 20 12:11:27 2023, max compression
```

## Comparing `cm-cluster-on-demand-aws-9.2.8.tar` & `cm-cluster-on-demand-aws-9.2.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:27.053306 cm-cluster-on-demand-aws-9.2.8/
--rw-r--r--   0 root         (0) root         (0)    11358 2022-12-27 18:19:08.000000 cm-cluster-on-demand-aws-9.2.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)       81 2022-12-27 18:19:08.000000 cm-cluster-on-demand-aws-9.2.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1970 2022-12-27 18:19:27.053306 cm-cluster-on-demand-aws-9.2.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1053 2022-12-27 18:19:08.000000 cm-cluster-on-demand-aws-9.2.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:27.053306 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/
--rw-r--r--   0 root         (0) root         (0)      596 2022-12-27 18:19:08.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2022-12-27 18:19:26.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/_version.py
--rw-r--r--   0 root         (0) root         (0)     3714 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/base.py
--rw-r--r--   0 root         (0) root         (0)     3830 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/brightsetup.py
--rw-r--r--   0 root         (0) root         (0)     3477 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/cli.py
--rw-r--r--   0 root         (0) root         (0)    18693 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/cluster.py
--rw-r--r--   0 root         (0) root         (0)    42050 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/clustercreate.py
--rw-r--r--   0 root         (0) root         (0)     2640 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/clusterdelete.py
--rw-r--r--   0 root         (0) root         (0)     6072 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/clusterlist.py
--rw-r--r--   0 root         (0) root         (0)     1898 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/clusterstart.py
--rw-r--r--   0 root         (0) root         (0)     2102 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/clusterstop.py
--rw-r--r--   0 root         (0) root         (0)     1432 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/configdump.py
--rw-r--r--   0 root         (0) root         (0)     1444 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/configshow.py
--rw-r--r--   0 root         (0) root         (0)     3047 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/configuration.py
--rw-r--r--   0 root         (0) root         (0)     1267 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/ec2connection.py
--rw-r--r--   0 root         (0) root         (0)     3901 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/efs.py
--rw-r--r--   0 root         (0) root         (0)     2280 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/imagelist.py
--rw-r--r--   0 root         (0) root         (0)     4727 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/images.py
--rw-r--r--   0 root         (0) root         (0)     2838 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/instancetype.py
--rw-r--r--   0 root         (0) root         (0)     4506 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/instancetypelist.py
--rw-r--r--   0 root         (0) root         (0)     2656 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/paramvalidation.py
--rw-r--r--   0 root         (0) root         (0)     3660 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/summary.py
--rw-r--r--   0 root         (0) root         (0)    19081 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/vpc.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-27 18:19:27.053306 cm-cluster-on-demand-aws-9.2.8/cm_cluster_on_demand_aws.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1970 2022-12-27 18:19:26.000000 cm-cluster-on-demand-aws-9.2.8/cm_cluster_on_demand_aws.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1075 2022-12-27 18:19:27.000000 cm-cluster-on-demand-aws-9.2.8/cm_cluster_on_demand_aws.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-27 18:19:26.000000 cm-cluster-on-demand-aws-9.2.8/cm_cluster_on_demand_aws.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       64 2022-12-27 18:19:26.000000 cm-cluster-on-demand-aws-9.2.8/cm_cluster_on_demand_aws.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      138 2022-12-27 18:19:26.000000 cm-cluster-on-demand-aws-9.2.8/cm_cluster_on_demand_aws.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       19 2022-12-27 18:19:26.000000 cm-cluster-on-demand-aws-9.2.8/cm_cluster_on_demand_aws.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-27 18:19:27.053306 cm-cluster-on-demand-aws-9.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2517 2022-12-27 18:19:11.000000 cm-cluster-on-demand-aws-9.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:27.383719 cm-cluster-on-demand-aws-9.2.9/
+-rw-r--r--   0 root         (0) root         (0)    11358 2023-02-20 12:11:10.000000 cm-cluster-on-demand-aws-9.2.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       81 2023-02-20 12:11:10.000000 cm-cluster-on-demand-aws-9.2.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-02-20 12:11:27.383719 cm-cluster-on-demand-aws-9.2.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1053 2023-02-20 12:11:10.000000 cm-cluster-on-demand-aws-9.2.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:27.383719 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/
+-rw-r--r--   0 root         (0) root         (0)      596 2023-02-20 12:11:10.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-02-20 12:11:26.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/_version.py
+-rw-r--r--   0 root         (0) root         (0)     3714 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/base.py
+-rw-r--r--   0 root         (0) root         (0)     3830 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/brightsetup.py
+-rw-r--r--   0 root         (0) root         (0)     3477 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/cli.py
+-rw-r--r--   0 root         (0) root         (0)    18693 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/cluster.py
+-rw-r--r--   0 root         (0) root         (0)    42050 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/clustercreate.py
+-rw-r--r--   0 root         (0) root         (0)     2640 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/clusterdelete.py
+-rw-r--r--   0 root         (0) root         (0)     6072 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/clusterlist.py
+-rw-r--r--   0 root         (0) root         (0)     1898 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/clusterstart.py
+-rw-r--r--   0 root         (0) root         (0)     2102 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/clusterstop.py
+-rw-r--r--   0 root         (0) root         (0)     1432 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/configdump.py
+-rw-r--r--   0 root         (0) root         (0)     1444 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/configshow.py
+-rw-r--r--   0 root         (0) root         (0)     3047 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/configuration.py
+-rw-r--r--   0 root         (0) root         (0)     1267 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/ec2connection.py
+-rw-r--r--   0 root         (0) root         (0)     3901 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/efs.py
+-rw-r--r--   0 root         (0) root         (0)     2280 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/imagelist.py
+-rw-r--r--   0 root         (0) root         (0)     4727 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/images.py
+-rw-r--r--   0 root         (0) root         (0)     2838 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/instancetype.py
+-rw-r--r--   0 root         (0) root         (0)     4506 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/instancetypelist.py
+-rw-r--r--   0 root         (0) root         (0)     2656 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/paramvalidation.py
+-rw-r--r--   0 root         (0) root         (0)     3660 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/summary.py
+-rw-r--r--   0 root         (0) root         (0)    19081 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/vpc.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 12:11:27.383719 cm-cluster-on-demand-aws-9.2.9/cm_cluster_on_demand_aws.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1970 2023-02-20 12:11:27.000000 cm-cluster-on-demand-aws-9.2.9/cm_cluster_on_demand_aws.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1075 2023-02-20 12:11:27.000000 cm-cluster-on-demand-aws-9.2.9/cm_cluster_on_demand_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-02-20 12:11:27.000000 cm-cluster-on-demand-aws-9.2.9/cm_cluster_on_demand_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       64 2023-02-20 12:11:27.000000 cm-cluster-on-demand-aws-9.2.9/cm_cluster_on_demand_aws.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      138 2023-02-20 12:11:27.000000 cm-cluster-on-demand-aws-9.2.9/cm_cluster_on_demand_aws.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       19 2023-02-20 12:11:27.000000 cm-cluster-on-demand-aws-9.2.9/cm_cluster_on_demand_aws.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-02-20 12:11:27.383719 cm-cluster-on-demand-aws-9.2.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2517 2023-02-20 12:11:13.000000 cm-cluster-on-demand-aws-9.2.9/setup.py
```

### Comparing `cm-cluster-on-demand-aws-9.2.8/LICENSE` & `cm-cluster-on-demand-aws-9.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-aws-9.2.8/PKG-INFO` & `cm-cluster-on-demand-aws-9.2.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm-cluster-on-demand-aws
-Version: 9.2.8
+Version: 9.2.9
 Summary: Bright Cluster on Demand Utility AWS
 Home-page: https://www.brightcomputing.com/
 Author: Cloudteam
 Author-email: cloudteam@brightcomputing.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cm-cluster-on-demand-aws-9.2.8/README.md` & `cm-cluster-on-demand-aws-9.2.9/README.md`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/__init__.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/__init__.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/base.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/base.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/brightsetup.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/brightsetup.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/cli.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/cli.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/cluster.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/cluster.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/clustercreate.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/clustercreate.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/clusterdelete.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/clusterdelete.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/clusterlist.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/clusterlist.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/clusterstart.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/clusterstart.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/clusterstop.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/clusterstop.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/configdump.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/configdump.py`

 * *Files 2% similar despite different names*

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/configshow.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/configshow.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/configuration.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/configuration.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/ec2connection.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/ec2connection.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/efs.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/efs.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/imagelist.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/imagelist.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/images.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/images.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/instancetype.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/instancetype.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/instancetypelist.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/instancetypelist.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/paramvalidation.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/paramvalidation.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/summary.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/summary.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/clusterondemandaws/vpc.py` & `cm-cluster-on-demand-aws-9.2.9/clusterondemandaws/vpc.py`

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

### Comparing `cm-cluster-on-demand-aws-9.2.8/cm_cluster_on_demand_aws.egg-info/PKG-INFO` & `cm-cluster-on-demand-aws-9.2.9/cm_cluster_on_demand_aws.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cm-cluster-on-demand-aws
-Version: 9.2.8
+Version: 9.2.9
 Summary: Bright Cluster on Demand Utility AWS
 Home-page: https://www.brightcomputing.com/
 Author: Cloudteam
 Author-email: cloudteam@brightcomputing.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cm-cluster-on-demand-aws-9.2.8/cm_cluster_on_demand_aws.egg-info/SOURCES.txt` & `cm-cluster-on-demand-aws-9.2.9/cm_cluster_on_demand_aws.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cm-cluster-on-demand-aws-9.2.8/setup.py` & `cm-cluster-on-demand-aws-9.2.9/setup.py`

 * *Files 1% similar despite different names*

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

