# Comparing `tmp/PyShoreVolume-1.0.3.tar.gz` & `tmp/PyShoreVolume-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyShoreVolume-1.0.3.tar", last modified: Fri May 26 16:27:29 2023, max compression
+gzip compressed data, was "PyShoreVolume-1.0.4.tar", last modified: Tue Jul 18 11:20:49 2023, max compression
```

## Comparing `PyShoreVolume-1.0.3.tar` & `PyShoreVolume-1.0.4.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.533633 PyShoreVolume-1.0.3/
--rw-r--r--   0 owenjames   (501) staff       (20)    16078 2023-05-26 16:27:29.533757 PyShoreVolume-1.0.3/PKG-INFO
--rw-r--r--   0 owenjames   (501) staff       (20)    15186 2023-04-27 16:59:49.000000 PyShoreVolume-1.0.3/README.txt
--rw-r--r--   0 owenjames   (501) staff       (20)      117 2023-05-26 16:27:29.534273 PyShoreVolume-1.0.3/setup.cfg
--rw-r--r--   0 owenjames   (501) staff       (20)     2579 2023-05-26 16:23:37.000000 PyShoreVolume-1.0.3/setup.py
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.513538 PyShoreVolume-1.0.3/src/
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.515344 PyShoreVolume-1.0.3/src/PyShoreVolume/
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.516743 PyShoreVolume-1.0.3/src/PyShoreVolume/CleanandTransectLocator/
--rw-r--r--   0 owenjames   (501) staff       (20)     6705 2023-04-26 16:01:36.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/CleanandTransectLocator/DataCleaning.py
--rw-r--r--   0 owenjames   (501) staff       (20)     5970 2023-04-26 14:58:53.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/CleanandTransectLocator/TransectDefinition.py
--rw-r--r--   0 owenjames   (501) staff       (20)      258 2023-04-26 10:05:08.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/CleanandTransectLocator/__init__.py
--rw-r--r--   0 owenjames   (501) staff       (20)     3355 2023-05-02 13:07:00.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/DOD1.py
--rw-r--r--   0 owenjames   (501) staff       (20)     5508 2023-05-02 13:08:54.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/DataImportandTransectDefinition1.py
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.528368 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/
--rw-r--r--   0 owenjames   (501) staff       (20)    28792 2023-05-10 13:13:01.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/End Point Rate.jpg
--rw-r--r--   0 owenjames   (501) staff       (20)     1197 2023-05-17 14:53:48.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/File_Organisation_Script.py
--rw-r--r--   0 owenjames   (501) staff       (20)        5 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.cpg
--rw-r--r--   0 owenjames   (501) staff       (20)   853906 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.dbf
--rw-r--r--   0 owenjames   (501) staff       (20)      417 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.prj
--rw-r--r--   0 owenjames   (501) staff       (20)    36528 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.shp
--rw-r--r--   0 owenjames   (501) staff       (20)    10508 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.shx
--rw-r--r--   0 owenjames   (501) staff       (20)   236652 2023-05-09 10:01:48.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/NetShorelineMovementErosionandAccretion.jpg
--rw-r--r--   0 owenjames   (501) staff       (20)     1587 2023-05-17 14:54:14.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/QGISMergedShoreline.py
--rw-r--r--   0 owenjames   (501) staff       (20)        5 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.cpg
--rw-r--r--   0 owenjames   (501) staff       (20)     6261 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.dbf
--rw-r--r--   0 owenjames   (501) staff       (20)      417 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.prj
--rw-r--r--   0 owenjames   (501) staff       (20)     7756 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.shp
--rw-r--r--   0 owenjames   (501) staff       (20)      796 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.shx
--rw-r--r--   0 owenjames   (501) staff       (20)        0 2023-05-01 13:34:09.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/__init__.py
--rw-r--r--   0 owenjames   (501) staff       (20)    32234 2023-05-10 13:13:01.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/eprresults.pkl
--rw-r--r--   0 owenjames   (501) staff       (20)     9487 2023-05-08 13:42:46.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/lrrdictionary.pkl
--rw-r--r--   0 owenjames   (501) staff       (20)   224924 2023-05-09 10:09:18.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/netshorelinemovement.jpg
--rw-r--r--   0 owenjames   (501) staff       (20)    21751 2023-05-08 13:43:15.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/nsm.pkl
--rw-r--r--   0 owenjames   (501) staff       (20)    21748 2023-05-08 13:42:54.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/scedic.pkl
--rw-r--r--   0 owenjames   (501) staff       (20)   235175 2023-05-09 10:02:52.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/shorleinechangeenvelope.jpg
--rwxr--r--   0 owenjames   (501) staff       (20)     1806 2023-05-02 13:05:10.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/SCA1.py
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.531320 PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/
--rw-r--r--   0 owenjames   (501) staff       (20)    11033 2023-05-03 09:55:00.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/EPR.py
--rw-r--r--   0 owenjames   (501) staff       (20)     5629 2023-04-26 16:11:01.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/LRR.py
--rw-r--r--   0 owenjames   (501) staff       (20)     7895 2023-05-26 14:52:49.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/NSM.py
--rw-r--r--   0 owenjames   (501) staff       (20)     9638 2023-05-03 10:00:49.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/NSMEandA.py
--rw-r--r--   0 owenjames   (501) staff       (20)     7935 2023-05-03 07:48:32.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/SCE.py
--rw-r--r--   0 owenjames   (501) staff       (20)      181 2023-03-22 20:35:05.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/__init__.py
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.533328 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/
--rw-r--r--   0 owenjames   (501) staff       (20)    15278 2023-05-03 10:08:13.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/DEMofDifference.py
--rw-r--r--   0 owenjames   (501) staff       (20)     6106 2023-05-03 09:06:39.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/DODSubPlot.py
--rw-r--r--   0 owenjames   (501) staff       (20)     1772 2023-05-03 09:26:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/MaskingDEM.py
--rw-r--r--   0 owenjames   (501) staff       (20)     3219 2023-04-28 12:05:59.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/NetVolumeChange.py
--rw-r--r--   0 owenjames   (501) staff       (20)    11070 2023-05-03 09:27:46.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/OldesttoNewest.py
--rw-r--r--   0 owenjames   (501) staff       (20)    73653 2023-05-03 09:50:15.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/SeasonalDOD.py
--rw-r--r--   0 owenjames   (501) staff       (20)      458 2023-04-28 10:20:21.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/__init__.py
--rw-r--r--   0 owenjames   (501) staff       (20)      236 2023-05-02 14:03:43.000000 PyShoreVolume-1.0.3/src/PyShoreVolume/__init__.py
-drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-05-26 16:27:29.516101 PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/
--rw-r--r--   0 owenjames   (501) staff       (20)    16078 2023-05-26 16:27:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/PKG-INFO
--rw-r--r--   0 owenjames   (501) staff       (20)     2036 2023-05-26 16:27:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/SOURCES.txt
--rw-r--r--   0 owenjames   (501) staff       (20)        1 2023-05-26 16:27:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/dependency_links.txt
--rw-r--r--   0 owenjames   (501) staff       (20)      256 2023-05-26 16:27:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/requires.txt
--rw-r--r--   0 owenjames   (501) staff       (20)       59 2023-05-26 16:27:29.000000 PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/top_level.txt
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-07-18 11:20:49.454801 PyShoreVolume-1.0.4/
+-rw-r--r--   0 owenjames   (501) staff       (20)    16078 2023-07-18 11:20:49.454925 PyShoreVolume-1.0.4/PKG-INFO
+-rw-r--r--   0 owenjames   (501) staff       (20)    15186 2023-04-27 16:59:49.000000 PyShoreVolume-1.0.4/README.txt
+-rw-r--r--   0 owenjames   (501) staff       (20)      117 2023-07-18 11:20:49.455422 PyShoreVolume-1.0.4/setup.cfg
+-rw-r--r--   0 owenjames   (501) staff       (20)     2579 2023-07-18 09:52:36.000000 PyShoreVolume-1.0.4/setup.py
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-07-18 11:20:49.395449 PyShoreVolume-1.0.4/src/
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-07-18 11:20:49.397633 PyShoreVolume-1.0.4/src/PyShoreVolume/
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-07-18 11:20:49.418848 PyShoreVolume-1.0.4/src/PyShoreVolume/CleanandTransectLocator/
+-rw-r--r--   0 owenjames   (501) staff       (20)     3906 2023-07-14 10:27:04.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/CleanandTransectLocator/DataCleaning.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     5970 2023-04-26 14:58:53.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/CleanandTransectLocator/TransectDefinition.py
+-rw-r--r--   0 owenjames   (501) staff       (20)      258 2023-04-26 10:05:08.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/CleanandTransectLocator/__init__.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     3355 2023-05-02 13:07:00.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/DOD1.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     5518 2023-06-22 08:41:50.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/DataImportandTransectDefinition1.py
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-07-18 11:20:49.448142 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/
+-rw-r--r--   0 owenjames   (501) staff       (20)    28792 2023-05-10 13:13:01.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/End Point Rate.jpg
+-rw-r--r--   0 owenjames   (501) staff       (20)     1197 2023-05-17 14:53:48.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/File_Organisation_Script.py
+-rw-r--r--   0 owenjames   (501) staff       (20)        5 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Intersections2.cpg
+-rw-r--r--   0 owenjames   (501) staff       (20)   853906 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Intersections2.dbf
+-rw-r--r--   0 owenjames   (501) staff       (20)      417 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Intersections2.prj
+-rw-r--r--   0 owenjames   (501) staff       (20)    36528 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Intersections2.shp
+-rw-r--r--   0 owenjames   (501) staff       (20)    10508 2023-04-26 15:59:05.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Intersections2.shx
+-rw-r--r--   0 owenjames   (501) staff       (20)   236652 2023-05-09 10:01:48.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/NetShorelineMovementErosionandAccretion.jpg
+-rw-r--r--   0 owenjames   (501) staff       (20)     1587 2023-05-17 14:54:14.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/QGISMergedShoreline.py
+-rw-r--r--   0 owenjames   (501) staff       (20)        5 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Transect1.cpg
+-rw-r--r--   0 owenjames   (501) staff       (20)     6261 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Transect1.dbf
+-rw-r--r--   0 owenjames   (501) staff       (20)      417 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Transect1.prj
+-rw-r--r--   0 owenjames   (501) staff       (20)     7756 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Transect1.shp
+-rw-r--r--   0 owenjames   (501) staff       (20)      796 2023-04-23 13:26:29.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Transect1.shx
+-rw-r--r--   0 owenjames   (501) staff       (20)        0 2023-05-01 13:34:09.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/__init__.py
+-rw-r--r--   0 owenjames   (501) staff       (20)    32234 2023-05-10 13:13:01.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/eprresults.pkl
+-rw-r--r--   0 owenjames   (501) staff       (20)     9487 2023-05-08 13:42:46.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/lrrdictionary.pkl
+-rw-r--r--   0 owenjames   (501) staff       (20)   224924 2023-05-09 10:09:18.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/netshorelinemovement.jpg
+-rw-r--r--   0 owenjames   (501) staff       (20)    21751 2023-05-08 13:43:15.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/nsm.pkl
+-rw-r--r--   0 owenjames   (501) staff       (20)    21748 2023-05-08 13:42:54.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/scedic.pkl
+-rw-r--r--   0 owenjames   (501) staff       (20)   235175 2023-05-09 10:02:52.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/shorleinechangeenvelope.jpg
+-rwxr--r--   0 owenjames   (501) staff       (20)     1806 2023-05-02 13:05:10.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/SCA1.py
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-07-18 11:20:49.451791 PyShoreVolume-1.0.4/src/PyShoreVolume/ShorelineChange/
+-rw-r--r--   0 owenjames   (501) staff       (20)    11033 2023-05-03 09:55:00.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/ShorelineChange/EPR.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     5629 2023-04-26 16:11:01.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/ShorelineChange/LRR.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     7895 2023-05-26 14:52:49.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/ShorelineChange/NSM.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     9638 2023-05-03 10:00:49.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/ShorelineChange/NSMEandA.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     7935 2023-05-03 07:48:32.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/ShorelineChange/SCE.py
+-rw-r--r--   0 owenjames   (501) staff       (20)      181 2023-03-22 20:35:05.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/ShorelineChange/__init__.py
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-07-18 11:20:49.454454 PyShoreVolume-1.0.4/src/PyShoreVolume/VolumeChanges/
+-rw-r--r--   0 owenjames   (501) staff       (20)    15278 2023-05-03 10:08:13.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/VolumeChanges/DEMofDifference.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     6106 2023-05-03 09:06:39.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/VolumeChanges/DODSubPlot.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     1772 2023-05-03 09:26:29.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/VolumeChanges/MaskingDEM.py
+-rw-r--r--   0 owenjames   (501) staff       (20)     3219 2023-04-28 12:05:59.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/VolumeChanges/NetVolumeChange.py
+-rw-r--r--   0 owenjames   (501) staff       (20)    11070 2023-05-03 09:27:46.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/VolumeChanges/OldesttoNewest.py
+-rw-r--r--   0 owenjames   (501) staff       (20)    73653 2023-05-03 09:50:15.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/VolumeChanges/SeasonalDOD.py
+-rw-r--r--   0 owenjames   (501) staff       (20)      458 2023-04-28 10:20:21.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/VolumeChanges/__init__.py
+-rw-r--r--   0 owenjames   (501) staff       (20)      236 2023-05-02 14:03:43.000000 PyShoreVolume-1.0.4/src/PyShoreVolume/__init__.py
+drwxr-xr-x   0 owenjames   (501) staff       (20)        0 2023-07-18 11:20:49.399480 PyShoreVolume-1.0.4/src/PyShoreVolume.egg-info/
+-rw-r--r--   0 owenjames   (501) staff       (20)    16078 2023-07-18 11:20:49.000000 PyShoreVolume-1.0.4/src/PyShoreVolume.egg-info/PKG-INFO
+-rw-r--r--   0 owenjames   (501) staff       (20)     2036 2023-07-18 11:20:49.000000 PyShoreVolume-1.0.4/src/PyShoreVolume.egg-info/SOURCES.txt
+-rw-r--r--   0 owenjames   (501) staff       (20)        1 2023-07-18 11:20:49.000000 PyShoreVolume-1.0.4/src/PyShoreVolume.egg-info/dependency_links.txt
+-rw-r--r--   0 owenjames   (501) staff       (20)      256 2023-07-18 11:20:49.000000 PyShoreVolume-1.0.4/src/PyShoreVolume.egg-info/requires.txt
+-rw-r--r--   0 owenjames   (501) staff       (20)       59 2023-07-18 11:20:49.000000 PyShoreVolume-1.0.4/src/PyShoreVolume.egg-info/top_level.txt
```

### Comparing `PyShoreVolume-1.0.3/PKG-INFO` & `PyShoreVolume-1.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyShoreVolume
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python Based Shoreline Change and Beach Volume Analysis Tool
 Home-page: https://github.com/owencaseyjames/PyShoreVolume
 Author: Owen Casey James
 Author-email: owen.james@kcl.ac.uk
 License: MIT
 Keywords: Shoreline Erosion SCA Volume Digital Elevation Model EPR SCA NSM LRR
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyShoreVolume-1.0.3/README.txt` & `PyShoreVolume-1.0.4/README.txt`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/setup.py` & `PyShoreVolume-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='PyShoreVolume',
-      version ='1.0.3',
+      version ='1.0.4',
       description ='Python Based Shoreline Change and Beach Volume Analysis Tool',
       author ='Owen Casey James',
       author_email = 'owen.james@kcl.ac.uk',
       licence ='MIT',
       keywords = 'Shoreline Erosion SCA Volume Digital Elevation Model EPR SCA NSM LRR',
       long_description=long_description,
       long_description_content_type='text/markdown',
```

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/CleanandTransectLocator/DataCleaning.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/CleanandTransectLocator/TransectDefinition.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 """
-Created on Fri Jan  6 15:09:47 2023
+Created on Mon Aug 15 13:16:41 2022
 
 @author: owenjames
 """
-#DataCleaning.py
 
+#TransectDefinition.py
 
+
+#imports geoplot as gplt
 import geopandas as gpd
 from geopandas import GeoSeries, GeoDataFrame
 import pandas as pd
 
 import os 
 
 import scipy
@@ -47,144 +49,126 @@
 
 import time
 
 import datetime
 from datetime import datetime, timezone
 
 import geopy.distance
-
-import datetime
-from datetime import datetime
-
+ 
 import pickle
 
+import sys
 
-def cleaning(intersected):
+
+##Number 1
+###Add transect points to geodataframe (X AND Y are transect root coord from the linestring) Number 1
+###If wrong way around the erosion and accretion values  will be the wrong way around. Baseline m
+def transectstartlocator1(baseline, intersectednew):
         """
-        Data cleaning protocol to remove duplicate intersections of the same year
-        along the same transect only keeping one that is closest to the seaward 
-        side from the intersections with no 'layer' value. 
+        Locates the starting coordinates of each transect and merges them into the 
+        into the intersection data frame.
     
         Parameters
         ----------
-        intersected : Pandas GeoDataframe
+        baseline : Pandas GeoDataframe 
+            GeoDataframe of cross transects shapefile
+        intersectednew : Pandas GeoDataframe
+            Geodataframe containing 'TR_ID' field of transect numbers, 'layer' field 
+            with YYYYMM integer values, 'geometry_x' field of each shoreline intersection,
+    
+        Returns
+        -------
+        intersected: Pandas GeoDatafame
+             Geodataframe of the intersect file with the correspondng coordinates of
+             the transect starting point on the seaward side in the fields 'X' and 'Y'.
+             Allows Erosion/Accretion rates to be measured in other functions.
+    
+        """
+        x = []
+        y = []
+        trid = []
+        val = 0
+        for i in baseline['geometry']:
+            # print(baseline['geometry'][val].coords[1])
+            x.append(baseline['geometry'][val].coords[1][0])
+            y.append(baseline['geometry'][val].coords[1][1])
+            trid.append(baseline['TR_ID'][val])
+            val = val + 1
+        transectgeoms = GeoDataFrame({'X':x,'Y':y,'TR_ID':trid})
+        transectgeoms = GeoDataFrame(transectgeoms, geometry=gpd.points_from_xy(transectgeoms.X,transectgeoms.Y))
+        transectgeoms.plot()
+        
+        if 'X' in intersectednew.columns: 
+            transectgeoms.set_index('TR_ID').combine_first(intersectednew.set_index('TR_ID'))            
+        else:    
+            intersectednew = intersectednew.merge(transectgeoms, on='TR_ID', how= 'left')      
+        intersected = intersectednew.set_geometry('geometry_x')
+        
+        return intersected
+
+### Number 2
+##If transect and thus baseline start locations are on the other sifde of the transect 
+def transectstartlocator2(baseline, intersectednew):
+        """
+        ocates the starting coordinates of each transect and merges them into the 
+        into the intersection data frame.
+        
+        Parameters
+        ----------
+        baseline : Pandas GeoDataframe 
+            GeoDataframe of cross transects shapefile
+        intersectednew : Pandas GeoDataframe
             Geodataframe containing 'TR_ID' field of transect numbers, 'layer' field 
             with YYYYMM integer values, 'geometry_x' field of each shoreline intersection,
-            and 'geometry_y' of each transect starting location. 
-            
     
         Returns
         -------
-        intersectednew : Pandas GeoDataFrame
-            Geodataframe that only contains the closet intersect to the shoreline from 
-            that date, with all other intesects removed. Also removes any intersection
-            point that do not have a value in the 'layer' column to identify their date.
+        intersected: Pandas GeoDatafame
+             Geodataframe of the intersect file with the correspondng coordinates of
+             the transect starting point on the seaward side in the fields 'X' and 'Y'.
+             Allows Erosion/Accretion rates to be measured in other functions.
         """
+        x = []
+        y = []
+        trid = []
+        val = 0
+        for i in baseline['geometry']:
+            # print(baseline['geometry'][val].coords[0])
+            x.append(baseline['geometry'][val].coords[0][0])
+            y.append(baseline['geometry'][val].coords[0][1])
+            trid.append(baseline['TR_ID'][val])
+            val = val + 1
+        transectgeoms = GeoDataFrame({'X':x,'Y':y,'TR_ID':trid})
+        transectgeoms = GeoDataFrame(transectgeoms, geometry=gpd.points_from_xy(transectgeoms.X,transectgeoms.Y))
+        transectgeoms.plot()
+        
+        if 'X' in intersectednew.columns: 
+            transectgeoms.set_index('TR_ID').combine_first(intersectednew.set_index('TR_ID'))
+        else:    
+            intersectednew = intersectednew.merge(transectgeoms, on='TR_ID', how= 'left')
+            
+        intersected = intersectednew.set_geometry('geometry_x')
+        
+        return intersected
+    
+        
+
+# if __name__ =='__main__':
+#     sys.exit()
     
-        intersected = intersected.sort_values(by=['TR_ID'])
-        uniquetrans = intersected.TR_ID.unique()
-        val = int(min(intersected['TR_ID']))
-        listy = []
-
-        dicty = {}
-        for e, ids in enumerate(uniquetrans):
-                # if val == ids: 
-                # print(ids, e)
-                s = GeoDataFrame(intersected.loc[intersected['TR_ID'] == ids])
-                # print(s)
-                # s = s.loc[s['Z']== median]
-                s = s.set_geometry('geometry_x').to_crs(epsg=3857)
-                ##tr - transect geometry point
-                tr = s
-                tr = tr.set_geometry('geometry_y').to_crs(epsg=3857)
-                uniquelayer = s['layer'].drop_duplicates()
-                #print(tr, uniquelayer)      
-        
-         ####Iterate through the available years taking the intersect closest to baseline first
-        
-                for i in uniquelayer:
-                    yeardrop = s.loc[s['layer']==i]
-                    trs = tr.iloc[0]
-                    # print(trs)
-                    dists = yeardrop['geometry_x'].distance(trs['geometry_y'])
-                    # print(dists)
-                    gdf1 = intersected.loc[dists.idxmin()]
-                    gdf1 = gdf1.T
-                    dicty = {}
-                    dicty.update(gdf1)
-                    listy.append(dicty)     
-                
-        
-        intersectednew = GeoDataFrame(listy)
-        intersectednew = intersectednew.set_geometry('geometry_x') 
-        intersectednew = GeoDataFrame(intersectednew[~intersectednew['layer'].isnull()])
-        return intersectednew
-        #print(len(intersectednew))
-
-
-
-###lower level
-# vals = int(min(lowerranges['TR_ID']))
-# listlower = []
-# for ids in lowerranges['TR_ID']:
-#     if vals == ids: 
-#         # print(ids)
-#         s = GeoDataFrame(lowerranges.loc[lowerranges['TR_ID'] == ids])
-                        
-#         #### find individual dates to use as the index
-#         uniquelayer = s['layer'].drop_duplicates()
-                
-#         #####iterate through the available years taking the closest to baseline first
-#         for i in uniquelayer:
-#                 #             ###find the index of the first year in this transect
-#                 indexes = s.loc[s['layer']==i].index[0]
-#                 # print(indexes['ID'])
-#                               ###Same for the upper and lower ranges
-#                 indexlow = lowerranges[lowerranges['layer']==i].index[0]    
-#                               # print(intersectednew.loc[indexes])
-#                 gdf1 = lowerranges.loc[indexes]
-#                 gdf1 = gdf1.T
-#                 dicty = {}
-#                 dicty.update(gdf1)
-#                 listlower.append(dicty)
-#         vals = vals + 1
-# intersectedlower = GeoDataFrame(listlower)
-# intersectedlower.rename(columns={'geometry_x':'geometry_lower','Z':'Z_lower'}, inplace=True)
-# intersectedlower = intersectedlower.set_geometry('geometry_lower')
-
-
-# # ####Higherlevel
-# val = int(min(intersected['TR_ID']))
-# listy = []
-# maxi = max(intersected['Z'])
-# # print(median)
-# for ids in intersected['TR_ID']:
-#     if val == ids: 
-#         # print(ids)
-#         s = GeoDataFrame(intersected.loc[intersected['TR_ID'] == ids])
-#         s = s.loc[s['Z']== maxi]
-        
-# #       ### find individual dates to use as the index
-#         uniquelayer = s['layer'].drop_duplicates()
-        
-
-# # #       ####iterate through the available years taking the closest to baseline first
-#         for i in uniquelayer:
-# #             ###find the index of the first year in this transect
-#               indexes = s.loc[s['layer']==i].index[0]
-#               ###Same for the upper and lower ranges
-#               indexlow = lowerranges[lowerranges['layer']==i].index[0]
-#               # print(intersectednew.loc[indexes])
-#               gdf1 = intersected.loc[indexes]
-#               gdf1 = gdf1.T
-#               dicty = {}
-#               dicty.update(gdf1)
-#               listy.append(dicty)
-#         val = val + 1
-# intersectedhigher = GeoDataFrame(listy)
-# intersectedhigher.rename(columns={'geometry_x':'geometry_higher','Z':'Z_higher'}, inplace=True)
-# intersectedhigher = intersectedhigher.set_geometry('geometry_higher') 
-# # print(intersectedhigher['Z'].max())
-# # print(intersectedhigher)
+####DECIDE IF WE WILL GO AHEAD WITH THIS (MULTIPLE CONTOUR VALUES)
+###Set geometry column now that Geometry x is the coords of the intersected point
+# intersected = intersected.set_geometry('geometry_x')
+
+# ###Extract the intersections of contours produced from errors
+# lowerranges = GeoDataFrame(intersected.loc[intersected['Z']== intersected['Z'].min()])
+# lowerranges = lowerranges.set_geometry('geometry_x')
+
+
+# higherranges = intersected.loc[intersected['Z']== intersected['Z'].max()]
+# # higherranges['TR_ID'] = higherranges['TR_ID'].astype(int)
+# # higher = GeoDataFrame(intersectednew.loc[intersectednew['Z']== intersectednew['Z'].max()])
+# higherranges= higherranges.set_geometry('geometry_x')
+# print(max(higherranges['TR_ID']))
+# print(max(lowerranges['TR_ID']))
+# highers.TR_ID.dtype
 
-# intersectednew = pd.merge(intersectednew,intersectedhigher[['TR_ID','layer','geometry_higher','Z_higher']], on = ['TR_ID','layer'])
-# intersectednew = pd.merge(intersectednew,intersectedlower[['TR_ID','layer','geometry_lower','Z_lower']], on = ['TR_ID','layer'])
```

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/CleanandTransectLocator/TransectDefinition.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/DataImportandTransectDefinition1.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,169 +1,140 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-"""
-Created on Mon Aug 15 13:16:41 2022
-
-@author: owenjames
-"""
-
-#TransectDefinition.py
-
-
-#imports geoplot as gplt
+#DataImportandTransectDefinition.py>
+import PyShoreVolume 
+from  PyShoreVolume.CleanandTransectLocator.DataCleaning import cleaning
+from PyShoreVolume.CleanandTransectLocator.TransectDefinition import transectstartlocator2, transectstartlocator1
+import os
 import geopandas as gpd
-from geopandas import GeoSeries, GeoDataFrame
-import pandas as pd
-
-import os 
 
-import scipy
-from scipy.spatial import ConvexHull, convex_hull_plot_2d
-from scipy.spatial.distance import cdist, pdist
 
-import statsmodels.api as sm
-
-import numpy as np
-
-import shapely
-from shapely.geometry import Point, MultiPoint
-from shapely.ops import nearest_points
+##Directories ** Dont forget '/' at the end
+#os.chdir('/Users/owenjames/Dropbox/PhD/Shoreline_Data/cco_data-20220625114304/data/lidar/')
+#path = '/Users/owenjames/Dropbox/PhD/Shoreline_Data/cco_data-20220625114304/data/lidar/'
+
+###!!! NEEED TO STATE IN DESCRIPTION THE 
+
+class DataImportandTransectDefinition(): 
+
+    ###Save to path 
+    
+    def __init__(self, CRS, intersects, transects, path, measurementerror, georeferror):
+        
+        self.CRS = CRS
+        self.intersects = intersects
+        self.transects = transects
+        self.path = path
+        self.measurementerror = measurementerror
+        self.georeferror = georeferror 
+        
+
+    def transectstartlocator1(self):
+        self.intersects = transectstartlocator1(self.transects, self.intersects)
+        return self.intersects
+        
+    def transectstartlocator2(self):
+        self.intersects = transectstartlocator2(self.transects, self.intersects)
+        return self.intersects
+    
+    def cleaning(self):
+        self.intersects = cleaning(self.intersects, self.CRS)
+        return self.intersects
+    
+    def results(self):
+        directory = 'results/'
+        save_to_path = os.path.join(self.path, directory)  
+        return save_to_path
+    
+    def errors(self):
+        uniques = gpd.GeoDataFrame()
+        uniques['layer'] = gpd.GeoDataFrame(self.intersects['layer'].unique())
+        uniques = uniques.sort_values(by = ['layer'])
+        uniques['Georef Err'] = self.georeferror
+        uniques['Measurement Err'] = self.measurementerror
+        if 'Georef Err' in self.intersects.columns: 
+            uniques.set_index('layer').combine_first(self.intersects.set_index('layer'))            
+        else:    
+            self.intersects = self.intersects.merge(uniques, on='layer', how= 'left')   
+        self.intersects = self.intersects.set_geometry('geometry_x')
+        return self.intersects
+    
+    
+#Extending amount of coordinates 
+# gpd.options.display_precision = 10
 
-import sklearn
-from sklearn import preprocessing
-from sklearn import linear_model
-from sklearn.linear_model import LinearRegression 
-from sklearn.metrics import r2_score, mean_squared_error
+# ##Desired CRS (Used in geopy measurements - go to site to find most suitable)
+# CRS = 4277
+# ##Specify the crs ellipsoid (Used in geopy distance measurements - go to site to find mathing ellipsoid for crs)
+# ellipsoidal = 'Airy (1830)'
 
-import seaborn as sns
 
-import matplotlib
-import matplotlib.pyplot as plt
-from matplotlib import cm
-from matplotlib.colors import LinearSegmentedColormap
-from mpl_toolkits.axes_grid1 import make_axes_locatable
-from matplotlib.lines import Line2D
 
-import contextily as ctx
 
-import pyproj
+##Read in intersects shapefile 
+# intersectdata = gpd.read_file(r'intersects.shp')
+# intersectednew = intersectdata.to_crs(epsg=CRS)
 
-import time
+# ###Review data
+# print(intersectednew.columns)
 
-import datetime
-from datetime import datetime, timezone
+# ####Read in baseline layer 
 
-import geopy.distance
- 
-import pickle
+# print(baseline['geometry'])
 
-import sys
+# ####Errors 
+# measurementerror = 0.3
+# digitisingerror = 0
 
 
-##Number 1
 ###Add transect points to geodataframe (X AND Y are transect root coord from the linestring) Number 1
 ###If wrong way around the erosion and accretion values  will be the wrong way around. Baseline m
-def transectstartlocator1(baseline, intersectednew):
-        """
-        Locates the starting coordinates of each transect and merges them into the 
-        into the intersection data frame.
-    
-        Parameters
-        ----------
-        baseline : Pandas GeoDataframe 
-            GeoDataframe of cross transects shapefile
-        intersectednew : Pandas GeoDataframe
-            Geodataframe containing 'TR_ID' field of transect numbers, 'layer' field 
-            with YYYYMM integer values, 'geometry_x' field of each shoreline intersection,
-    
-        Returns
-        -------
-        intersected: Pandas GeoDatafame
-             Geodataframe of the intersect file with the correspondng coordinates of
-             the transect starting point on the seaward side in the fields 'X' and 'Y'.
-             Allows Erosion/Accretion rates to be measured in other functions.
-    
-        """
-        x = []
-        y = []
-        trid = []
-        val = 0
-        for i in baseline['geometry']:
-            # print(baseline['geometry'][val].coords[1])
-            x.append(baseline['geometry'][val].coords[1][0])
-            y.append(baseline['geometry'][val].coords[1][1])
-            trid.append(baseline['TR_ID'][val])
-            val = val + 1
-        transectgeoms = GeoDataFrame({'X':x,'Y':y,'TR_ID':trid})
-        transectgeoms = GeoDataFrame(transectgeoms, geometry=gpd.points_from_xy(transectgeoms.X,transectgeoms.Y))
-        transectgeoms.plot()
-        
-        if 'X' in intersectednew.columns: 
-            transectgeoms.set_index('TR_ID').combine_first(intersectednew.set_index('TR_ID'))            
-        else:    
-            intersectednew = intersectednew.merge(transectgeoms, on='TR_ID', how= 'left')      
-        intersected = intersectednew.set_geometry('geometry_x')
-        
-        return intersected
-
-### Number 2
-##If transect and thus baseline start locations are on the other sifde of the transect 
-def transectstartlocator2(baseline, intersectednew):
-        """
-        ocates the starting coordinates of each transect and merges them into the 
-        into the intersection data frame.
-        
-        Parameters
-        ----------
-        baseline : Pandas GeoDataframe 
-            GeoDataframe of cross transects shapefile
-        intersectednew : Pandas GeoDataframe
-            Geodataframe containing 'TR_ID' field of transect numbers, 'layer' field 
-            with YYYYMM integer values, 'geometry_x' field of each shoreline intersection,
-    
-        Returns
-        -------
-        intersected: Pandas GeoDatafame
-             Geodataframe of the intersect file with the correspondng coordinates of
-             the transect starting point on the seaward side in the fields 'X' and 'Y'.
-             Allows Erosion/Accretion rates to be measured in other functions.
-        """
-        x = []
-        y = []
-        trid = []
-        val = 0
-        for i in baseline['geometry']:
-            # print(baseline['geometry'][val].coords[0])
-            x.append(baseline['geometry'][val].coords[0][0])
-            y.append(baseline['geometry'][val].coords[0][1])
-            trid.append(baseline['TR_ID'][val])
-            val = val + 1
-        transectgeoms = GeoDataFrame({'X':x,'Y':y,'TR_ID':trid})
-        transectgeoms = GeoDataFrame(transectgeoms, geometry=gpd.points_from_xy(transectgeoms.X,transectgeoms.Y))
-        transectgeoms.plot()
-        
-        if 'X' in intersectednew.columns: 
-            transectgeoms.set_index('TR_ID').combine_first(intersectednew.set_index('TR_ID'))
-        else:    
-            intersectednew = intersectednew.merge(transectgeoms, on='TR_ID', how= 'left')
-            
-        intersected = intersectednew.set_geometry('geometry_x')
-        
-        return intersected
-    
+# def transectstartlocator(baseline):
+#         x = []
+#         y = []
+#         trid = []
+#         val = 0
+#         for i in baseline['geometry']:
+#             # print(baseline['geometry'][val].coords[0])
+#             x.append(baseline['geometry'][val].coords[1][0])
+#             y.append(baseline['geometry'][val].coords[1][1])
+#             trid.append(baseline['TR_ID'][val])
+#             val = val + 1
+#         transectgeoms = GeoDataFrame({'X':x,'Y':y,'TR_ID':trid})
+#         transectgeoms = GeoDataFrame(transectgeoms, geometry=gpd.points_from_xy(transectgeoms.X,transectgeoms.Y))
+#         intersected = intersectednew.merge(transectgeoms, on='TR_ID', how= 'left')
+
+# # #Plot to review transect baselines
+#         transectgeoms.plot()
+#         intersected = intersected.set_geometry('geometry_x')
+# # transectgeoms.plot()
+# ### Number 2
+# ##If transect and thus baseline start locations are on the other sifde of the transect 
+# def transectstartlocator2(baseline):
+#         x = []
+#         y = []
+#         trid = []
+#         val = 0
+#         for i in baseline['geometry']:
+#             # print(baseline['geometry'][val].coords[0])
+#             x.append(baseline['geometry'][val].coords[0][0])
+#             y.append(baseline['geometry'][val].coords[0][1])
+#             trid.append(baseline['TR_ID'][val])
+#             val = val + 1
+#         transectgeoms = GeoDataFrame({'X':x,'Y':y,'TR_ID':trid})
+#         transectgeoms = GeoDataFrame(transectgeoms, geometry=gpd.points_from_xy(transectgeoms.X,transectgeoms.Y))
+#         intersected = intersectednew.merge(transectgeoms, on='TR_ID', how= 'left')
+
+# # #Plot to review transect baselines
+#         transectgeoms.plot()
+#         intersected = intersected.set_geometry('geometry_x')
         
 
-# if __name__ =='__main__':
-#     sys.exit()
-    
-####DECIDE IF WE WILL GO AHEAD WITH THIS (MULTIPLE CONTOUR VALUES)
-###Set geometry column now that Geometry x is the coords of the intersected point
+# ###Set geometry column now that Geometry x is the coords of the intersected point
 # intersected = intersected.set_geometry('geometry_x')
 
-# ###Extract the intersections of contours produced from errors
+###Extract the intersections of contours produced from errors
 # lowerranges = GeoDataFrame(intersected.loc[intersected['Z']== intersected['Z'].min()])
 # lowerranges = lowerranges.set_geometry('geometry_x')
 
 
 # higherranges = intersected.loc[intersected['Z']== intersected['Z'].max()]
 # # higherranges['TR_ID'] = higherranges['TR_ID'].astype(int)
 # # higher = GeoDataFrame(intersectednew.loc[intersectednew['Z']== intersectednew['Z'].max()])
```

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/DOD1.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/DOD1.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/End Point Rate.jpg` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/End Point Rate.jpg`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/File_Organisation_Script.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/File_Organisation_Script.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.dbf` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Intersections2.dbf`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.shp` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Intersections2.shp`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Intersections2.shx` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Intersections2.shx`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/NetShorelineMovementErosionandAccretion.jpg` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/NetShorelineMovementErosionandAccretion.jpg`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/QGISMergedShoreline.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/QGISMergedShoreline.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.dbf` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Transect1.dbf`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.shp` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Transect1.shp`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/Transect1.shx` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/Transect1.shx`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/eprresults.pkl` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/eprresults.pkl`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/lrrdictionary.pkl` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/lrrdictionary.pkl`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/netshorelinemovement.jpg` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/netshorelinemovement.jpg`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/nsm.pkl` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/nsm.pkl`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/scedic.pkl` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/scedic.pkl`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/Extra/shorleinechangeenvelope.jpg` & `PyShoreVolume-1.0.4/src/PyShoreVolume/Extra/shorleinechangeenvelope.jpg`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/SCA1.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/SCA1.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/EPR.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/ShorelineChange/EPR.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/LRR.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/ShorelineChange/LRR.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/NSM.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/ShorelineChange/NSM.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/NSMEandA.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/ShorelineChange/NSMEandA.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/ShorelineChange/SCE.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/ShorelineChange/SCE.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/DEMofDifference.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/VolumeChanges/DEMofDifference.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/DODSubPlot.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/VolumeChanges/DODSubPlot.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/MaskingDEM.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/VolumeChanges/MaskingDEM.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/NetVolumeChange.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/VolumeChanges/NetVolumeChange.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/OldesttoNewest.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/VolumeChanges/OldesttoNewest.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume/VolumeChanges/SeasonalDOD.py` & `PyShoreVolume-1.0.4/src/PyShoreVolume/VolumeChanges/SeasonalDOD.py`

 * *Files identical despite different names*

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/PKG-INFO` & `PyShoreVolume-1.0.4/src/PyShoreVolume.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyShoreVolume
-Version: 1.0.3
+Version: 1.0.4
 Summary: Python Based Shoreline Change and Beach Volume Analysis Tool
 Home-page: https://github.com/owencaseyjames/PyShoreVolume
 Author: Owen Casey James
 Author-email: owen.james@kcl.ac.uk
 License: MIT
 Keywords: Shoreline Erosion SCA Volume Digital Elevation Model EPR SCA NSM LRR
 Classifier: Development Status :: 4 - Beta
```

### Comparing `PyShoreVolume-1.0.3/src/PyShoreVolume.egg-info/SOURCES.txt` & `PyShoreVolume-1.0.4/src/PyShoreVolume.egg-info/SOURCES.txt`

 * *Files identical despite different names*

