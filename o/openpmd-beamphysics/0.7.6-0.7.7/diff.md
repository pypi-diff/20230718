# Comparing `tmp/openpmd-beamphysics-0.7.6.tar.gz` & `tmp/openpmd-beamphysics-0.7.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/openPMD-beamphysics/openPMD-beamphysics/dist/.tmp-xfqepgl4/openpmd-beamphysics-0.7.6.tar", last modified: Wed Jun 28 20:58:37 2023, max compression
+gzip compressed data, was "/home/runner/work/openPMD-beamphysics/openPMD-beamphysics/dist/.tmp-irn1_pkw/openpmd-beamphysics-0.7.7.tar", last modified: Tue Jul 18 18:30:32 2023, max compression
```

## Comparing `openpmd-beamphysics-0.7.6.tar` & `openpmd-beamphysics-0.7.7.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:58:37.000000 openpmd-beamphysics-0.7.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-28 20:58:37.000000 openpmd-beamphysics-0.7.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:58:37.000000 openpmd-beamphysics-0.7.6/openpmd_beamphysics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-06-28 20:58:37.000000 openpmd-beamphysics-0.7.6/openpmd_beamphysics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-06-28 20:58:37.000000 openpmd-beamphysics-0.7.6/openpmd_beamphysics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-28 20:58:37.000000 openpmd-beamphysics-0.7.6/openpmd_beamphysics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-06-28 20:58:37.000000 openpmd-beamphysics-0.7.6/openpmd_beamphysics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-28 20:58:37.000000 openpmd-beamphysics-0.7.6/openpmd_beamphysics.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:58:37.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-28 20:58:37.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:58:37.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/fields/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/fields/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/fields/conversion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/fields/expansion.py
--rw-r--r--   0 runner    (1001) docker     (123)    23902 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/fields/fieldmesh.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:58:37.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/ansys.py
--rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/astra.py
--rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/bmad.py
--rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/elegant.py
--rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/genesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/gpt.py
--rw-r--r--   0 runner    (1001) docker     (123)    22750 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/impact.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/litrack.py
--rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/lucretia.py
--rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/opal.py
--rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/simion.py
--rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/superfish.py
--rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/labels.py
--rw-r--r--   0 runner    (1001) docker     (123)    36475 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/particles.py
--rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/readers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/species.py
--rw-r--r--   0 runner    (1001) docker     (123)    10530 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/statistics.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/units.py
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/pmd_beamphysics/writers.py
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-28 20:58:37.000000 openpmd-beamphysics-0.7.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-28 20:58:37.000000 openpmd-beamphysics-0.7.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/tests/test_particlegroup.py
--rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-06-28 20:58:29.000000 openpmd-beamphysics-0.7.6/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12849 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/conversion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/expansion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23902 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/fieldmesh.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/ansys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12299 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/astra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/bmad.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6756 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/elegant.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15427 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/genesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4681 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/gpt.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22750 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/impact.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/litrack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6488 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/lucretia.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2877 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/opal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6599 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/simion.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9149 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/superfish.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3645 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/labels.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35085 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/particles.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12072 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/plot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10189 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/readers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/species.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12643 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/statistics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14211 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/pmd_beamphysics/writers.py
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 18:30:32.000000 openpmd-beamphysics-0.7.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1697 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/tests/test_particlegroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78254 2023-07-18 18:30:23.000000 openpmd-beamphysics-0.7.7/versioneer.py
```

### Comparing `openpmd-beamphysics-0.7.6/LICENSE` & `openpmd-beamphysics-0.7.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/PKG-INFO` & `openpmd-beamphysics-0.7.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpmd-beamphysics
-Version: 0.7.6
+Version: 0.7.7
 Home-page: https://github.com/ChristopherMayes/openPMD-beamphysics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openPMD-beamphysics
```

### Comparing `openpmd-beamphysics-0.7.6/README.md` & `openpmd-beamphysics-0.7.7/README.md`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/openpmd_beamphysics.egg-info/PKG-INFO` & `openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openpmd-beamphysics
-Version: 0.7.6
+Version: 0.7.7
 Home-page: https://github.com/ChristopherMayes/openPMD-beamphysics
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # openPMD-beamphysics
```

### Comparing `openpmd-beamphysics-0.7.6/openpmd_beamphysics.egg-info/SOURCES.txt` & `openpmd-beamphysics-0.7.7/openpmd_beamphysics.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/fields/analysis.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/analysis.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/fields/conversion.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/conversion.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/fields/expansion.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/expansion.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/fields/fieldmesh.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/fields/fieldmesh.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/ansys.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/ansys.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/astra.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/astra.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/bmad.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/bmad.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/elegant.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/elegant.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/genesis.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/genesis.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/gpt.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/gpt.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/impact.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/impact.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/litrack.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/litrack.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/lucretia.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/lucretia.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/opal.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/opal.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/simion.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/simion.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/interfaces/superfish.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/interfaces/superfish.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/labels.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/labels.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/particles.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/particles.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,19 +12,18 @@
 from pmd_beamphysics.interfaces.elegant import write_elegant
 
 from pmd_beamphysics.plot import density_plot, marginal_plot, slice_plot
 
 from pmd_beamphysics.readers import particle_array, particle_paths
 from pmd_beamphysics.species import charge_of, mass_of
 
-from pmd_beamphysics.statistics import norm_emit_calc, normalized_particle_coordinate, particle_amplitude, particle_twiss_dispersion, matched_particles
+from pmd_beamphysics.statistics import norm_emit_calc, normalized_particle_coordinate, particle_amplitude, particle_twiss_dispersion, matched_particles, resample_particles
 from pmd_beamphysics.writers import write_pmd_bunch, pmd_init
 
 from h5py import File
-from scipy import stats as scipy_stats
 import numpy as np
 from copy import deepcopy
 import functools
 import os
 
 
 #-----------------------------------------
@@ -867,23 +866,18 @@
     def split(self, n_chunks = 100, key='z'):
         return split_particles(self, n_chunks=n_chunks, key=key)
     
     def copy(self):
         """Returns a deep copy"""
         return deepcopy(self)    
     
-    
-    # Operator overloading    
-    
-    # Resample
-    def resample(self, n):
-        """
-        Resamples n particles.
-        """
-        return resample(self, n)
+    @functools.wraps(resample_particles)
+    def resample(self, n=0):
+        data = resample_particles(self, n)
+        return ParticleGroup(data=data)
     
     # Internal sorting
     def _sort(self, key):
         """Sorts internal arrays by key"""
         ixlist = np.argsort(self[key])
         for k in self._settable_array_keys:
             self._data[k] = self[k][ixlist]    
@@ -1083,54 +1077,14 @@
         plist.append(p)
         
     return plist
 
 
 
 
-def resample(particle_group, n):
-    """
-    Resamples a ParticleGroup randomly.
-    
-    If weights are equal, a random subset of particles will be selected.
-    Otherwise, particles will be sampled according to their weight.
-    Note that this latter method can result in duplicate particles.
-    
-    Returns a new ParticleGroup instance.
-    
-    """
-    n_old = particle_group.n_particle
-    if n > n_old:
-        raise ValueError(f'Cannot supersample {n_old} to {n}')
-    
-    weight = particle_group.weight
-    
-    # Equal weights
-    if len(set(particle_group.weight)) == 1:
-        ixlist = np.random.choice(n_old, n, replace=False)
-        
-    # variable weights        
-    else:
-        # From SciPy example:
-        # https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.rv_discrete.html#scipy.stats.rv_discrete
-        pk = weight / np.sum(weight) # Probabilities
-        xk = np.arange(len(pk)) # index
-        ixsampler = scipy_stats.rv_discrete(name='ixsampler', values=(xk, pk))        
-        ixlist = ixsampler.rvs(size=n)
-        
-    weight = np.full(n, particle_group.charge/n)
-    
-    data = {}
-    for key in particle_group._settable_array_keys:
-        data[key] = particle_group[key][ixlist]
-    data['species'] = particle_group['species']
-    data['weight'] = weight
-    
-    return ParticleGroup(data=data)
-
 
 
 def particle_parts(particle_group, x):
     """
     Gets parts of a ParticleGroup object. Returns a new ParticleGroup
     """
     data = {}
```

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/plot.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/plot.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/readers.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/readers.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/species.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/species.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/statistics.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/statistics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import numpy as np
-
-
+from scipy import stats as scipy_stats
 
 def norm_emit_calc(particle_group, planes=['x']):
     """
     
     2d, 4d, 6d normalized emittance calc
     
     planes = ['x', 'y'] is the 4d emittance
@@ -421,7 +420,69 @@
         for k in keys:
             sdat[k][i] = pg[k]
             
     return sdat
 
 
 
+def resample_particles(particle_group, n=0):
+    """
+    Resamples a ParticleGroup randomly.
+
+    If n equals particle_group.n_particle or n=0, 
+    particle indices will be scrambled.
+    
+    Otherwise if weights are equal, a random subset of particles will be selected.
+    
+    Otherwise if weights are not equal, particles will be sampled according to their weight using a method from SciPy:
+    https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.rv_discrete.html#scipy.stats.rv_discrete
+    Note that this latter method can result in duplicate particles, and can be very slow for a large number of particles.
+
+    Parameters
+    ----------
+    n: int, default = 0
+        Number to resample. 
+        If n = 0, this will use all particles.
+
+    Returns
+    -------
+    data: dict of ParticleGroup data
+    
+    """
+    n_old = particle_group.n_particle
+    if n == 0:
+        n = n_old
+
+    if n > n_old:
+        raise ValueError(f'Cannot supersample {n_old} to {n}')
+    
+    weight = particle_group.weight
+    
+    # Equal weights
+    if len(set(particle_group.weight)) == 1:
+        ixlist = np.random.choice(n_old, n, replace=False)
+        weight = np.full(n, particle_group.charge/n)
+        
+    # variable weights        
+    else:
+        if n == n_old:
+            ixlist = np.random.choice(n_old, n, replace=False)
+            weight = weight[ixlist] #just scramble
+        else:
+            # From SciPy example:
+            # https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.rv_discrete.html#scipy.stats.rv_discrete
+            pk = weight / np.sum(weight) # Probabilities
+            xk = np.arange(len(pk)) # index
+            ixsampler = scipy_stats.rv_discrete(name='ixsampler', values=(xk, pk))        
+            ixlist = ixsampler.rvs(size=n)
+            weight = np.full(n, particle_group.charge/n)
+    
+    data = {}
+    for key in particle_group._settable_array_keys:
+        data[key] = particle_group[key][ixlist]
+    data['species'] = particle_group['species']
+    data['weight'] = weight
+    
+    return data
+
+
+
```

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/tools.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/tools.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/units.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/units.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/pmd_beamphysics/writers.py` & `openpmd-beamphysics-0.7.7/pmd_beamphysics/writers.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/setup.py` & `openpmd-beamphysics-0.7.7/setup.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/tests/test_particlegroup.py` & `openpmd-beamphysics-0.7.7/tests/test_particlegroup.py`

 * *Files identical despite different names*

### Comparing `openpmd-beamphysics-0.7.6/versioneer.py` & `openpmd-beamphysics-0.7.7/versioneer.py`

 * *Files identical despite different names*

