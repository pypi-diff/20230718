# Comparing `tmp/mapel-marriages-2.0.7.tar.gz` & `tmp/mapel-marriages-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-marriages-2.0.7.tar", last modified: Mon Jul 17 15:53:41 2023, max compression
+gzip compressed data, was "mapel-marriages-2.0.8.tar", last modified: Tue Jul 18 07:11:46 2023, max compression
```

## Comparing `mapel-marriages-2.0.7.tar` & `mapel-marriages-2.0.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:41.941728 mapel-marriages-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-17 15:53:41.941728 mapel-marriages-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:53:41.941728 mapel-marriages-2.0.7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:41.937729 mapel-marriages-2.0.7/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:41.937729 mapel-marriages-2.0.7/src/mapel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:41.937729 mapel-marriages-2.0.7/src/mapel/marriages/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:41.937729 mapel-marriages-2.0.7/src/mapel/marriages/cultures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/cultures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/cultures/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/cultures/euclidean.py
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/cultures/impartial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/cultures/mallows.py
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/cultures/urn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/cultures_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:41.937729 mapel-marriages-2.0.7/src/mapel/marriages/distances/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/distances/main_marriages_distances.py
--rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/distances_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:41.937729 mapel-marriages-2.0.7/src/mapel/marriages/features/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/features/basic_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/features/distance_to_stability_features.py
--rw-r--r--   0 runner    (1001) docker     (123)     6624 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/features/experiments_marriage.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/features_.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:41.941728 mapel-marriages-2.0.7/src/mapel/marriages/objects/
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/objects/Marriages.py
--rw-r--r--   0 runner    (1001) docker     (123)    15775 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/objects/MarriagesExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/objects/MarriagesFamily.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/objects/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:41.941728 mapel-marriages-2.0.7/src/mapel/marriages/persistence/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/persistence/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/persistence/instance_exports.py
--rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-17 15:53:03.000000 mapel-marriages-2.0.7/src/mapel/marriages/persistence/instance_imports.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:41.941728 mapel-marriages-2.0.7/src/mapel_marriages.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-17 15:53:41.000000 mapel-marriages-2.0.7/src/mapel_marriages.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-17 15:53:41.000000 mapel-marriages-2.0.7/src/mapel_marriages.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:53:41.000000 mapel-marriages-2.0.7/src/mapel_marriages.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-17 15:53:41.000000 mapel-marriages-2.0.7/src/mapel_marriages.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-17 15:53:41.000000 mapel-marriages-2.0.7/src/mapel_marriages.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:46.429013 mapel-marriages-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-18 07:11:46.429013 mapel-marriages-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 07:11:46.429013 mapel-marriages-2.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:46.425013 mapel-marriages-2.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:46.425013 mapel-marriages-2.0.8/src/mapel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:46.429013 mapel-marriages-2.0.8/src/mapel/marriages/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:46.429013 mapel-marriages-2.0.8/src/mapel/marriages/cultures/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/cultures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/cultures/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17187 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/cultures/euclidean.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/cultures/impartial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/cultures/mallows.py
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/cultures/urn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/cultures_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:46.429013 mapel-marriages-2.0.8/src/mapel/marriages/distances/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/distances/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/distances/main_marriages_distances.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4943 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/distances_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:46.429013 mapel-marriages-2.0.8/src/mapel/marriages/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9347 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/features/basic_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4873 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/features/distance_to_stability_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6678 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/features/experiments_marriage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/features_.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:46.429013 mapel-marriages-2.0.8/src/mapel/marriages/objects/
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/objects/Marriages.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15448 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/objects/MarriagesExperiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3168 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/objects/MarriagesFamily.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/objects/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:46.429013 mapel-marriages-2.0.8/src/mapel/marriages/persistence/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/persistence/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/persistence/instance_exports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1938 2023-07-18 07:11:08.000000 mapel-marriages-2.0.8/src/mapel/marriages/persistence/instance_imports.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:46.429013 mapel-marriages-2.0.8/src/mapel_marriages.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2486 2023-07-18 07:11:46.000000 mapel-marriages-2.0.8/src/mapel_marriages.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1270 2023-07-18 07:11:46.000000 mapel-marriages-2.0.8/src/mapel_marriages.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:11:46.000000 mapel-marriages-2.0.8/src/mapel_marriages.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-18 07:11:46.000000 mapel-marriages-2.0.8/src/mapel_marriages.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-07-18 07:11:46.000000 mapel-marriages-2.0.8/src/mapel_marriages.egg-info/top_level.txt
```

### Comparing `mapel-marriages-2.0.7/LICENSE.txt` & `mapel-marriages-2.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/PKG-INFO` & `mapel-marriages-2.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-marriages
-Version: 2.0.7
+Version: 2.0.8
 Summary: Map of Marriages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-marriages-2.0.7/README.md` & `mapel-marriages-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/pyproject.toml` & `mapel-marriages-2.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65", "wheel", "pybind11>=2.6.1"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel-marriages"
-version = "2.0.7"
+version = "2.0.8"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
 ]
 description = "Map of Marriages"
 classifiers=[
     "Programming Language :: Python :: 3",
```

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/__init__.py` & `mapel-marriages-2.0.8/src/mapel/marriages/__init__.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/cultures/euclidean.py` & `mapel-marriages-2.0.8/src/mapel/marriages/cultures/euclidean.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/cultures/impartial.py` & `mapel-marriages-2.0.8/src/mapel/marriages/cultures/impartial.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/cultures/mallows.py` & `mapel-marriages-2.0.8/src/mapel/marriages/cultures/mallows.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/cultures/urn.py` & `mapel-marriages-2.0.8/src/mapel/marriages/cultures/urn.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/cultures_.py` & `mapel-marriages-2.0.8/src/mapel/marriages/cultures_.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/distances/main_marriages_distances.py` & `mapel-marriages-2.0.8/src/mapel/marriages/distances/main_marriages_distances.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/distances_.py` & `mapel-marriages-2.0.8/src/mapel/marriages/distances_.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/features/basic_features.py` & `mapel-marriages-2.0.8/src/mapel/marriages/features/basic_features.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/features/distance_to_stability_features.py` & `mapel-marriages-2.0.8/src/mapel/marriages/features/distance_to_stability_features.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/features/experiments_marriage.py` & `mapel-marriages-2.0.8/src/mapel/marriages/features/experiments_marriage.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,41 +96,42 @@
 
 
 
 def summed_rank_maximal_matching(instance):
     try:
         val,matching= rank_matching(instance,True,True)
     except:
-        return 'None'
+        return None
     # if number_blockingPairs(instance,matching)>0:
     #     print('ERROR IN summed_rank_maximal_matching')
     #     exit(0)
     return val
 
 def summed_rank_minimal_matching(instance):
     try:
         val,matching= rank_matching(instance,False,True)
     except:
-        return 'None'
+        return None
     # if number_blockingPairs(instance,matching)>0:
     #     print('ERROR IN summed_rank_minimal_matching')
     #     exit(0)
     return val
 
 def minimal_rank_maximizing_matching(instance):
     try:
         val,matching=rank_matching(instance,True,False)
     except:
-        return 'None'
+        return None
     # if number_blockingPairs(instance,matching)>0:
     #     print('ERROR IN minimal_rank_maximizing_matching')
     #     exit(0)
     return val
 
 def avg_number_of_bps_for_random_matching(instance,iterations=100):
+    instance = instance.votes
     bps=[]
     num_agents=len(instance[0])
     for _ in range(iterations):
         #create random matching
         agents=list(range(num_agents))
         shuffle(agents)
         m2=[]
@@ -138,14 +139,15 @@
             m2.append(agents.index(i))
         #print([agents,m2])
         #exit()
         bps.append(number_blockingPairs(instance,[agents,m2]))
     return statistics.mean(bps), statistics.stdev(bps)
 
 def number_of_bps_maximumWeight(instance):
+    instance = instance.votes
     num_agents=len(instance[0])
     G = nx.Graph()
     for i in range(num_agents):
         for j in range(num_agents):
             G.add_edge(i,j+num_agents,weight=2*(num_agents-1)-instance[0][i].index(j)-instance[1][j].index(i))
             #G.add_edge(i, j, weight=instance[i].index(j) + instance[j].index(i))
     matching=nx.max_weight_matching(G, maxcardinality=True)
```

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/features_.py` & `mapel-marriages-2.0.8/src/mapel/marriages/features_.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/objects/Marriages.py` & `mapel-marriages-2.0.8/src/mapel/marriages/objects/Marriages.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/objects/MarriagesExperiment.py` & `mapel-marriages-2.0.8/src/mapel/marriages/objects/MarriagesExperiment.py`

 * *Files 3% similar despite different names*

```diff
@@ -363,37 +363,28 @@
                         writer.writerow([key, feature_dict['value'][key]])
 
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
             os.mkdir(os.path.join(os.getcwd(), "election", self.experiment_id, "matrices"))
 
             # PREPARE MAP.CSV FILE
             path = os.path.join(os.getcwd(), "election", self.experiment_id, "map.csv")
 
             with open(path, 'w') as file_csv:
-                file_csv.write(
-                    "size;num_agents;culture_id;params;color;alpha;family_id;label;marker;show\n")
+                file_csv.write("size;num_agents;culture_id;params;color;alpha;family_id;label;marker;show\n")
                 file_csv.write("10;16;ic;{};black;1;IC;IC;o;t\n")
-
-
-    def get_election_id_from_model_name(self, model_id: str) -> str:
-        for family_id in self.families:
-            if self.families[family_id].culture_id == model_id:
-                return family_id
+        except:
+            pass
```

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/objects/MarriagesFamily.py` & `mapel-marriages-2.0.8/src/mapel/marriages/objects/MarriagesFamily.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/persistence/instance_exports.py` & `mapel-marriages-2.0.8/src/mapel/marriages/persistence/instance_exports.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/src/mapel/marriages/persistence/instance_imports.py` & `mapel-marriages-2.0.8/src/mapel/marriages/persistence/instance_imports.py`

 * *Files identical despite different names*

### Comparing `mapel-marriages-2.0.7/src/mapel_marriages.egg-info/PKG-INFO` & `mapel-marriages-2.0.8/src/mapel_marriages.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel-marriages
-Version: 2.0.7
+Version: 2.0.8
 Summary: Map of Marriages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-marriages-2.0.7/src/mapel_marriages.egg-info/SOURCES.txt` & `mapel-marriages-2.0.8/src/mapel_marriages.egg-info/SOURCES.txt`

 * *Files identical despite different names*

