# Comparing `tmp/dicomset-0.0.1.tar.gz` & `tmp/dicomset-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/baclark/code/dicomset/dist/.tmp-2xn6t13e/dicomset-0.0.1.tar", last modified: Fri Feb 24 00:15:43 2023, max compression
+gzip compressed data, was "dicomset-0.0.2.tar", last modified: Tue Jul 18 03:22:51 2023, max compression
```

## Comparing `dicomset-0.0.1.tar` & `dicomset-0.0.2.tar`

### file list

```diff
@@ -1,11 +1,25 @@
-drwxr-xr-x   0 baclark  (13517) punim1413 (11483)        0 2023-02-24 00:15:43.767199 dicomset-0.0.1/
--rw-r--r--   0 baclark  (13517) punim1413 (11483)     1056 2023-02-24 00:09:47.000000 dicomset-0.0.1/LICENSE
--rw-r--r--   0 baclark  (13517) punim1413 (11483)      682 2023-02-24 00:15:43.767183 dicomset-0.0.1/PKG-INFO
--rw-r--r--   0 baclark  (13517) punim1413 (11483)      172 2023-02-24 00:09:47.000000 dicomset-0.0.1/README.md
-drwxr-xr-x   0 baclark  (13517) punim1413 (11483)        0 2023-02-24 00:15:43.765197 dicomset-0.0.1/dicomset.egg-info/
--rw-r--r--   0 baclark  (13517) punim1413 (11483)      682 2023-02-24 00:15:43.000000 dicomset-0.0.1/dicomset.egg-info/PKG-INFO
--rw-r--r--   0 baclark  (13517) punim1413 (11483)      160 2023-02-24 00:15:43.000000 dicomset-0.0.1/dicomset.egg-info/SOURCES.txt
--rw-r--r--   0 baclark  (13517) punim1413 (11483)        1 2023-02-24 00:15:43.000000 dicomset-0.0.1/dicomset.egg-info/dependency_links.txt
--rw-r--r--   0 baclark  (13517) punim1413 (11483)        1 2023-02-24 00:15:43.000000 dicomset-0.0.1/dicomset.egg-info/top_level.txt
--rw-r--r--   0 baclark  (13517) punim1413 (11483)      577 2023-02-24 00:09:47.000000 dicomset-0.0.1/pyproject.toml
--rw-r--r--   0 baclark  (13517) punim1413 (11483)       38 2023-02-24 00:15:43.768183 dicomset-0.0.1/setup.cfg
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.725281 dicomset-0.0.2/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      270 2023-07-18 03:22:51.725114 dicomset-0.0.2/PKG-INFO
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:21.000000 dicomset-0.0.2/README.md
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.722146 dicomset-0.0.2/dicomset.egg-info/
+-rw-r--r--   0 clarkbrett (990701463) 678807148      270 2023-07-18 03:22:51.000000 dicomset-0.0.2/dicomset.egg-info/PKG-INFO
+-rw-r--r--   0 clarkbrett (990701463) 678807148      441 2023-07-18 03:22:51.000000 dicomset-0.0.2/dicomset.egg-info/SOURCES.txt
+-rw-r--r--   0 clarkbrett (990701463) 678807148        1 2023-07-18 03:22:51.000000 dicomset-0.0.2/dicomset.egg-info/dependency_links.txt
+-rw-r--r--   0 clarkbrett (990701463) 678807148        5 2023-07-18 03:22:51.000000 dicomset-0.0.2/dicomset.egg-info/top_level.txt
+-rw-r--r--   0 clarkbrett (990701463) 678807148       38 2023-07-18 03:22:51.725327 dicomset-0.0.2/setup.cfg
+-rw-r--r--   0 clarkbrett (990701463) 678807148      506 2023-07-18 03:21:23.000000 dicomset-0.0.2/setup.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.722447 dicomset-0.0.2/test/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:21.000000 dicomset-0.0.2/test/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.722731 dicomset-0.0.2/test/code/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:22.000000 dicomset-0.0.2/test/code/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.722953 dicomset-0.0.2/test/code/dataset/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:22.000000 dicomset-0.0.2/test/code/dataset/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.723256 dicomset-0.0.2/test/code/dataset/raw/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:22.000000 dicomset-0.0.2/test/code/dataset/raw/__init__.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.723924 dicomset-0.0.2/test/code/dataset/raw/dicom/
+-rw-r--r--   0 clarkbrett (990701463) 678807148       59 2023-07-18 02:44:22.000000 dicomset-0.0.2/test/code/dataset/raw/dicom/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1680 2023-07-18 03:06:08.000000 dicomset-0.0.2/test/code/dataset/raw/dicom/test_rtstruct_converter.py
+drwxr-xr-x   0 clarkbrett (990701463) 678807148        0 2023-07-18 03:22:51.724831 dicomset-0.0.2/test/code/metrics/
+-rw-r--r--   0 clarkbrett (990701463) 678807148        0 2023-07-18 02:44:22.000000 dicomset-0.0.2/test/code/metrics/__init__.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     1395 2023-07-18 03:06:08.000000 dicomset-0.0.2/test/code/metrics/test_dice.py
+-rw-r--r--   0 clarkbrett (990701463) 678807148     2516 2023-07-18 03:06:08.000000 dicomset-0.0.2/test/code/metrics/test_hausdorff.py
```

