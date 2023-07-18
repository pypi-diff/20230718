# Comparing `tmp/mapel-roommates-2.0.7.tar.gz` & `tmp/mapel-roommates-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-roommates-2.0.7.tar", last modified: Mon Jul 17 15:53:35 2023, max compression
+gzip compressed data, was "mapel-roommates-2.0.8.tar", last modified: Tue Jul 18 07:11:39 2023, max compression
```

## Comparing `mapel-roommates-2.0.7.tar` & `mapel-roommates-2.0.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.177779 mapel-roommates-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-17 15:53:35.177779 mapel-roommates-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:53:35.177779 mapel-roommates-2.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.173779 mapel-roommates-2.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.173779 mapel-roommates-2.0.7/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.173779 mapel-roommates-2.0.7/src/mapel/roommates/
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.173779 mapel-roommates-2.0.7/src/mapel/roommates/cultures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures/group_separable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures/impartial.py
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures/mallows.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures/urn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/cultures_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.173779 mapel-roommates-2.0.7/src/mapel/roommates/distances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/distances/main_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/distances_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.177779 mapel-roommates-2.0.7/src/mapel/roommates/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/features/basic_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/features/distance_to_stability_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/features_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.177779 mapel-roommates-2.0.7/src/mapel/roommates/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/objects/Roommates.py
--rw-r--r--   0 runner    (1001) docker     (123)    18660 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/objects/RoommatesExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/objects/RoommatesFamily.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.177779 mapel-roommates-2.0.7/src/mapel/roommates/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/persistence/instance_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-17 15:53:03.000000 mapel-roommates-2.0.7/src/mapel/roommates/persistence/instance_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:35.177779 mapel-roommates-2.0.7/src/mapel_roommates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-17 15:53:35.000000 mapel-roommates-2.0.7/src/mapel_roommates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-17 15:53:35.000000 mapel-roommates-2.0.7/src/mapel_roommates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:53:35.000000 mapel-roommates-2.0.7/src/mapel_roommates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 15:53:35.000000 mapel-roommates-2.0.7/src/mapel_roommates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 15:53:35.000000 mapel-roommates-2.0.7/src/mapel_roommates.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.669060 mapel-roommates-2.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.669060 mapel-roommates-2.0.8/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.669060 mapel-roommates-2.0.8/src/mapel/roommates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.669060 mapel-roommates-2.0.8/src/mapel/roommates/cultures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10974 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures/group_separable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures/impartial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3805 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures/urn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1695 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/cultures_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/src/mapel/roommates/distances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/distances/main_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/distances_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/src/mapel/roommates/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10122 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/features/basic_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/features/distance_to_stability_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3148 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/features_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/src/mapel/roommates/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     4497 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/objects/Roommates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18351 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/objects/RoommatesExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/objects/RoommatesFamily.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/src/mapel/roommates/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/persistence/instance_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-07-18 07:11:08.000000 mapel-roommates-2.0.8/src/mapel/roommates/persistence/instance_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:39.673060 mapel-roommates-2.0.8/src/mapel_roommates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-07-18 07:11:39.000000 mapel-roommates-2.0.8/src/mapel_roommates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1255 2023-07-18 07:11:39.000000 mapel-roommates-2.0.8/src/mapel_roommates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:11:39.000000 mapel-roommates-2.0.8/src/mapel_roommates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 07:11:39.000000 mapel-roommates-2.0.8/src/mapel_roommates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 07:11:39.000000 mapel-roommates-2.0.8/src/mapel_roommates.egg-info/top_level.txt
```

### Comparing `mapel-roommates-2.0.7/LICENSE.txt` & `mapel-roommates-2.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/PKG-INFO` & `mapel-roommates-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-roommates
-Version: 2.0.7
+Version: 2.0.8
 Summary: Map of Roommates
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-roommates-2.0.7/README.md` & `mapel-roommates-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/pyproject.toml` & `mapel-roommates-2.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-roommates"
-version = "2.0.7"
+version = "2.0.8"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
 ]
 description = "Map of Roommates"
 classifiers=[
     "Programming Language :: Python :: 3",
```

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/__init__.py` & `mapel-roommates-2.0.8/src/mapel/roommates/__init__.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/cultures/euclidean.py` & `mapel-roommates-2.0.8/src/mapel/roommates/cultures/euclidean.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/cultures/group_separable.py` & `mapel-roommates-2.0.8/src/mapel/roommates/cultures/group_separable.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/cultures/impartial.py` & `mapel-roommates-2.0.8/src/mapel/roommates/cultures/impartial.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/cultures/mallows.py` & `mapel-roommates-2.0.8/src/mapel/roommates/cultures/mallows.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     return evaluatePolynomial(coeff, phi)
 
 
 # mat[i][j] is the probability with which candidate i ends up in position j
 def mallowsMatrix(num_candidates, lphi, pos, normalize=True):
     mat = np.zeros([num_candidates, num_candidates])
     if normalize:
-        phi = phi_from_relphi(num_candidates, lphi)
+        phi = ml.phi_from_normphi(num_candidates, lphi)
     else:
         phi = lphi
     Z = calculateZ(num_candidates, phi)
     for i in range(num_candidates):
         for j in range(num_candidates):
             freqs = [pos[k][i][j] for k in
                      range(1 + int(num_candidates * (num_candidates - 1) / 2))]
@@ -118,11 +118,11 @@
     votes = [list(range(num_agents)) for _ in range(num_agents)]
 
     votes = [rotate(vote, shift) for shift, vote in enumerate(votes)]
 
     # if 'norm-phi' not in params:
     #     params['norm-phi'] = np.random.rand()
 
-    phi = phi_from_relphi(num_agents, relphi=normphi)
+    phi = ml.phi_from_normphi(num_agents, normphi=normphi)
     votes = mallows_votes(votes, phi)
 
     return convert(votes)
```

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/cultures/urn.py` & `mapel-roommates-2.0.8/src/mapel/roommates/cultures/urn.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/cultures_.py` & `mapel-roommates-2.0.8/src/mapel/roommates/cultures_.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/distances/main_distances.py` & `mapel-roommates-2.0.8/src/mapel/roommates/distances/main_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/distances_.py` & `mapel-roommates-2.0.8/src/mapel/roommates/distances_.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/features/basic_features.py` & `mapel-roommates-2.0.8/src/mapel/roommates/features/basic_features.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/features/distance_to_stability_features.py` & `mapel-roommates-2.0.8/src/mapel/roommates/features/distance_to_stability_features.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/features_.py` & `mapel-roommates-2.0.8/src/mapel/roommates/features_.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -6,21 +6,21 @@
 import numpy as np
 from itertools import combinations
 from mapel.core.inner_distances import l2
 
 registered_roommates_features = {
     'summed_rank_minimal_matching': basic.summed_rank_minimal_matching,
     'summed_rank_maximal_matching': basic.summed_rank_maximal_matching,
-    'minimal_rank_maximizing_matching': basic.minimal_rank_maximizing_matching,
     'min_num_bps_matching': basic.min_num_bps_matching,
     'num_of_bps_min_weight': basic.num_of_bps_maximumWeight,
     'avg_num_of_bps_for_rand_matching': basic.avg_num_of_bps_for_random_matching,
     'mutuality': basic.mutuality,
     'dist_from_id_1': basic.dist_from_id_1,
     'dist_from_id_2': basic.dist_from_id_2,
+    'minimal_rank_maximizing_matching': basic.minimal_rank_maximizing_matching,
 }
 
 
 def get_local_feature(feature_id):
     if feature_id in registered_roommates_features:
         return registered_roommates_features.get(feature_id)
     return {
```

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/objects/Roommates.py` & `mapel-roommates-2.0.8/src/mapel/roommates/objects/Roommates.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/objects/RoommatesExperiment.py` & `mapel-roommates-2.0.8/src/mapel/roommates/objects/RoommatesExperiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -430,22 +430,18 @@
                                          round(feature_dict['time'][key],3)])
 
         self.features[feature_id] = feature_dict
         return feature_dict
 
     def create_structure(self) -> None:
 
-        if not os.path.isdir("election/"):
-            os.mkdir(os.path.join(os.getcwd(), "election"))
-
-        if not os.path.isdir("images/"):
-            os.mkdir(os.path.join(os.getcwd(), "images"))
-
-        if not os.path.isdir("trash/"):
-            os.mkdir(os.path.join(os.getcwd(), "trash"))
+        dirs = ["experiments", "images", "trash"]
+        for dir in dirs:
+            if not os.path.isdir(dir):
+                os.mkdir(os.path.join(os.getcwd(), dir))
 
         try:
             os.mkdir(os.path.join(os.getcwd(), "election", self.experiment_id))
             os.mkdir(os.path.join(os.getcwd(), "election", self.experiment_id, "distances"))
             os.mkdir(os.path.join(os.getcwd(), "election", self.experiment_id, "features"))
             os.mkdir(os.path.join(os.getcwd(), "election", self.experiment_id, "coordinates"))
             os.mkdir(os.path.join(os.getcwd(), "election", self.experiment_id, "instances"))
@@ -454,16 +450,12 @@
             # PREPARE MAP.CSV FILE
             path = os.path.join(os.getcwd(), "election", self.experiment_id, "map.csv")
 
             with open(path, 'w') as file_csv:
                 file_csv.write(
                     "size;num_agents;culture_id;params;color;alpha;family_id;label;marker;show\n")
                 file_csv.write("10;20;roommates_ic;{};black;1;IC;IC;o;t\n")
+        except:
+            pass
 
 
 
-    def get_election_id_from_model_name(self, culture_id: str) -> str:
-        for family_id in self.families:
-            if self.families[family_id].culture_id == culture_id:
-                return family_id
-
-
```

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/objects/RoommatesFamily.py` & `mapel-roommates-2.0.8/src/mapel/roommates/objects/RoommatesFamily.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/persistence/instance_exports.py` & `mapel-roommates-2.0.8/src/mapel/roommates/persistence/instance_exports.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/src/mapel/roommates/persistence/instance_imports.py` & `mapel-roommates-2.0.8/src/mapel/roommates/persistence/instance_imports.py`

 * *Files identical despite different names*

### Comparing `mapel-roommates-2.0.7/src/mapel_roommates.egg-info/PKG-INFO` & `mapel-roommates-2.0.8/src/mapel_roommates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-roommates
-Version: 2.0.7
+Version: 2.0.8
 Summary: Map of Roommates
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-roommates-2.0.7/src/mapel_roommates.egg-info/SOURCES.txt` & `mapel-roommates-2.0.8/src/mapel_roommates.egg-info/SOURCES.txt`

 * *Files identical despite different names*

