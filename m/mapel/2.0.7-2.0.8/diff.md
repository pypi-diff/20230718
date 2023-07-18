# Comparing `tmp/mapel-2.0.7.tar.gz` & `tmp/mapel-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mapel-2.0.7.tar", last modified: Mon Jul 17 15:53:14 2023, max compression
+gzip compressed data, was "mapel-2.0.8.tar", last modified: Tue Jul 18 07:11:19 2023, max compression
```

## Comparing `mapel-2.0.7.tar` & `mapel-2.0.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:14.501773 mapel-2.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-17 15:53:03.000000 mapel-2.0.7/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-17 15:53:14.497773 mapel-2.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-17 15:53:03.000000 mapel-2.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 15:53:14.497773 mapel-2.0.7/mapel.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-17 15:53:14.000000 mapel-2.0.7/mapel.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-17 15:53:14.000000 mapel-2.0.7/mapel.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:53:14.000000 mapel-2.0.7/mapel.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-17 15:53:14.000000 mapel-2.0.7/mapel.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 15:53:14.000000 mapel-2.0.7/mapel.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-17 15:53:03.000000 mapel-2.0.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-17 15:53:03.000000 mapel-2.0.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 15:53:14.501773 mapel-2.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:19.177318 mapel-2.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-07-18 07:11:08.000000 mapel-2.0.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-18 07:11:19.177318 mapel-2.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-07-18 07:11:08.000000 mapel-2.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:11:19.177318 mapel-2.0.8/mapel.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2477 2023-07-18 07:11:19.000000 mapel-2.0.8/mapel.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-07-18 07:11:19.000000 mapel-2.0.8/mapel.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:11:19.000000 mapel-2.0.8/mapel.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-18 07:11:19.000000 mapel-2.0.8/mapel.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:11:19.000000 mapel-2.0.8/mapel.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-18 07:11:08.000000 mapel-2.0.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-07-18 07:11:08.000000 mapel-2.0.8/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 07:11:19.177318 mapel-2.0.8/setup.cfg
```

### Comparing `mapel-2.0.7/LICENSE.txt` & `mapel-2.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mapel-2.0.7/PKG-INFO` & `mapel-2.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel
-Version: 2.0.7
+Version: 2.0.8
 Summary: Map of Elections---all packages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Piotr Faliszewski <faliszew@agh.edu.pl>, Lukasz Janeczko <lukij1997@gmail.com>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-2.0.7/README.md` & `mapel-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `mapel-2.0.7/mapel.egg-info/PKG-INFO` & `mapel-2.0.8/mapel.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mapel
-Version: 2.0.7
+Version: 2.0.8
 Summary: Map of Elections---all packages
 Author-email: Stanislaw Szufa <s.szufa@gmail.com>, Niclas Boehmer <niclas.boehmer@tu-berlin.de>, Piotr Faliszewski <faliszew@agh.edu.pl>, Lukasz Janeczko <lukij1997@gmail.com>, Andrzej Kaczmarczyk <andrzej.kaczmarczyk@agh.edu.pl>, Kasper Sapala <kasper.sapala@gmail.com>, Tomasz Was <tomasz.t.was@gmail.com>
 License: Copyright (c) 2018-2022 Stanislaw Szufa and contributors
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
```

### Comparing `mapel-2.0.7/pyproject.toml` & `mapel-2.0.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mapel"
-version = "2.0.7"
+version = "2.0.8"
 authors = [
  {name = "Stanislaw Szufa", email = "s.szufa@gmail.com"},
  {name = "Niclas Boehmer", email = "niclas.boehmer@tu-berlin.de"},
  {name = "Piotr Faliszewski", email = "faliszew@agh.edu.pl"},
  {name = "Lukasz Janeczko", email = "lukij1997@gmail.com"},
  {name = "Andrzej Kaczmarczyk", email = "andrzej.kaczmarczyk@agh.edu.pl"},
  {name = "Kasper Sapala", email = "kasper.sapala@gmail.com"},
```

