# Comparing `tmp/abtem-1.0.0b8.tar.gz` & `tmp/abtem-1.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/abtem-1.0.0b8.tar", last modified: Mon Oct 19 09:53:59 2020, max compression
+gzip compressed data, was "dist\abtem-1.0.0b9.tar", last modified: Mon Oct 26 19:40:40 2020, max compression
```

## Comparing `abtem-1.0.0b8.tar` & `abtem-1.0.0b9.tar`

### file list

```diff
@@ -1,63 +1,65 @@
-drwxr-xr-x   0 jacobmadsen   (501) staff       (20)        0 2020-10-19 09:53:59.000000 abtem-1.0.0b8/
--rw-r--r--   0 jacobmadsen   (501) staff       (20)       61 2020-08-13 08:35:50.000000 abtem-1.0.0b8/MANIFEST.in
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     2570 2020-10-19 09:53:59.000000 abtem-1.0.0b8/PKG-INFO
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     1936 2020-08-13 08:35:50.000000 abtem-1.0.0b8/README.md
-drwxr-xr-x   0 jacobmadsen   (501) staff       (20)        0 2020-10-19 09:53:59.000000 abtem-1.0.0b8/abtem/
--rw-r--r--   0 jacobmadsen   (501) staff       (20)      545 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/__init__.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)       54 2020-10-19 09:50:47.000000 abtem-1.0.0b8/abtem/_version.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)    22268 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/base_classes.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     5960 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/cpu_kernels.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     9062 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/cuda_kernels.py
-drwxr-xr-x   0 jacobmadsen   (501) staff       (20)        0 2020-10-19 09:53:59.000000 abtem-1.0.0b8/abtem/data/
--rw-r--r--   0 jacobmadsen   (501) staff       (20)    14894 2020-08-13 08:56:23.000000 abtem-1.0.0b8/abtem/data/kirkland.txt
--rw-r--r--   0 jacobmadsen   (501) staff       (20)    21338 2020-08-13 08:56:23.000000 abtem-1.0.0b8/abtem/data/lobato.txt
--rw-r--r--   0 jacobmadsen   (501) staff       (20)    24780 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/detect.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     7427 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/device.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)    10299 2020-10-18 21:35:10.000000 abtem-1.0.0b8/abtem/dft.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)    22067 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/measure.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     5743 2020-10-19 09:50:47.000000 abtem-1.0.0b8/abtem/noise.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     6135 2020-08-27 07:08:20.000000 abtem-1.0.0b8/abtem/parametrizations.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     8440 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/plot.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)    35270 2020-10-18 21:35:28.000000 abtem-1.0.0b8/abtem/potentials.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)    16905 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/scan.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     4580 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/structures.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     5202 2020-08-25 09:52:17.000000 abtem-1.0.0b8/abtem/tanh_sinh.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     5519 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/temperature.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)    21604 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/transfer.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     6996 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/utils.py
-drwxr-xr-x   0 jacobmadsen   (501) staff       (20)        0 2020-10-19 09:53:59.000000 abtem-1.0.0b8/abtem/visualize/
--rw-r--r--   0 jacobmadsen   (501) staff       (20)       34 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/visualize/__init__.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     3686 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/visualize/bqplot.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     7381 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/visualize/mpl.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     1773 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/visualize/utils.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     2476 2020-10-18 21:05:08.000000 abtem-1.0.0b8/abtem/visualize/widgets.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)    63205 2020-10-19 09:50:47.000000 abtem-1.0.0b8/abtem/waves.py
-drwxr-xr-x   0 jacobmadsen   (501) staff       (20)        0 2020-10-19 09:53:59.000000 abtem-1.0.0b8/abtem.egg-info/
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     2570 2020-10-19 09:53:59.000000 abtem-1.0.0b8/abtem.egg-info/PKG-INFO
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     1141 2020-10-19 09:53:59.000000 abtem-1.0.0b8/abtem.egg-info/SOURCES.txt
--rw-r--r--   0 jacobmadsen   (501) staff       (20)        1 2020-10-19 09:53:59.000000 abtem-1.0.0b8/abtem.egg-info/dependency_links.txt
--rw-r--r--   0 jacobmadsen   (501) staff       (20)       65 2020-10-19 09:53:59.000000 abtem-1.0.0b8/abtem.egg-info/requires.txt
--rw-r--r--   0 jacobmadsen   (501) staff       (20)       11 2020-10-19 09:53:59.000000 abtem-1.0.0b8/abtem.egg-info/top_level.txt
--rw-r--r--   0 jacobmadsen   (501) staff       (20)       38 2020-10-19 09:53:59.000000 abtem-1.0.0b8/setup.cfg
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     1097 2020-08-18 11:01:32.000000 abtem-1.0.0b8/setup.py
-drwxr-xr-x   0 jacobmadsen   (501) staff       (20)        0 2020-10-19 09:53:59.000000 abtem-1.0.0b8/test/
--rw-r--r--   0 jacobmadsen   (501) staff       (20)        0 2020-08-13 08:35:50.000000 abtem-1.0.0b8/test/__init__.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)      605 2020-08-18 11:01:32.000000 abtem-1.0.0b8/test/conftest.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     1757 2020-10-19 09:50:18.000000 abtem-1.0.0b8/test/test_antialias.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     1442 2020-08-18 16:48:17.000000 abtem-1.0.0b8/test/test_cache.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     1803 2020-08-18 16:48:17.000000 abtem-1.0.0b8/test/test_ctf.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     1040 2020-10-19 09:50:18.000000 abtem-1.0.0b8/test/test_detect.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     2197 2020-08-22 17:50:23.000000 abtem-1.0.0b8/test/test_dft.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     1225 2020-08-18 16:48:17.000000 abtem-1.0.0b8/test/test_energy.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     1167 2020-08-18 16:48:17.000000 abtem-1.0.0b8/test/test_event.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     3960 2020-10-19 09:50:18.000000 abtem-1.0.0b8/test/test_export.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     3439 2020-10-19 09:50:18.000000 abtem-1.0.0b8/test/test_grid.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     1710 2020-10-19 09:50:18.000000 abtem-1.0.0b8/test/test_kirkland.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     3747 2020-10-19 09:50:18.000000 abtem-1.0.0b8/test/test_potential_integration.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)      787 2020-08-13 08:35:50.000000 abtem-1.0.0b8/test/test_potential_parametrization.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     2558 2020-10-19 09:50:18.000000 abtem-1.0.0b8/test/test_potentials.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     8176 2020-10-19 09:50:18.000000 abtem-1.0.0b8/test/test_prism.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)      750 2020-10-18 21:05:08.000000 abtem-1.0.0b8/test/test_propagator.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     3900 2020-10-19 09:50:18.000000 abtem-1.0.0b8/test/test_scan.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     1696 2020-08-18 11:01:32.000000 abtem-1.0.0b8/test/test_temperature.py
--rw-r--r--   0 jacobmadsen   (501) staff       (20)     6523 2020-10-19 09:50:18.000000 abtem-1.0.0b8/test/test_waves.py
+drwxrwxrwx   0        0        0        0 2020-10-26 19:40:40.925694 abtem-1.0.0b9/
+-rw-rw-rw-   0        0        0       63 2020-08-12 14:10:11.000000 abtem-1.0.0b9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3085 2020-10-26 19:40:40.925694 abtem-1.0.0b9/PKG-INFO
+-rw-rw-rw-   0        0        0     2390 2020-10-19 23:45:50.000000 abtem-1.0.0b9/README.md
+drwxrwxrwx   0        0        0        0 2020-10-26 19:40:40.784641 abtem-1.0.0b9/abtem/
+-rw-rw-rw-   0        0        0      567 2020-10-22 22:12:28.000000 abtem-1.0.0b9/abtem/__init__.py
+-rw-rw-rw-   0        0        0       57 2020-10-26 19:38:40.000000 abtem-1.0.0b9/abtem/_version.py
+-rw-rw-rw-   0        0        0    20569 2020-10-26 17:20:29.000000 abtem-1.0.0b9/abtem/base_classes.py
+-rw-rw-rw-   0        0        0     3596 2020-10-21 16:20:20.000000 abtem-1.0.0b9/abtem/cpu_kernels.py
+-rw-rw-rw-   0        0        0     5154 2020-10-25 15:08:51.000000 abtem-1.0.0b9/abtem/cuda_kernels.py
+drwxrwxrwx   0        0        0        0 2020-10-26 19:40:40.814506 abtem-1.0.0b9/abtem/data/
+-rw-rw-rw-   0        0        0    14999 2020-09-27 08:24:36.000000 abtem-1.0.0b9/abtem/data/kirkland.txt
+-rw-rw-rw-   0        0        0    21443 2020-09-27 08:24:36.000000 abtem-1.0.0b9/abtem/data/lobato.txt
+-rw-rw-rw-   0        0        0    27605 2020-10-25 19:19:38.000000 abtem-1.0.0b9/abtem/detect.py
+-rw-rw-rw-   0        0        0     7443 2020-10-24 15:04:19.000000 abtem-1.0.0b9/abtem/device.py
+-rw-rw-rw-   0        0        0    10574 2020-10-18 22:41:27.000000 abtem-1.0.0b9/abtem/dft.py
+-rw-rw-rw-   0        0        0     2658 2020-10-24 14:55:19.000000 abtem-1.0.0b9/abtem/interpolate.py
+-rw-rw-rw-   0        0        0    23167 2020-10-22 21:56:05.000000 abtem-1.0.0b9/abtem/measure.py
+-rw-rw-rw-   0        0        0     5923 2020-10-19 09:47:01.000000 abtem-1.0.0b9/abtem/noise.py
+-rw-rw-rw-   0        0        0     6275 2020-09-27 08:24:36.000000 abtem-1.0.0b9/abtem/parametrizations.py
+-rw-rw-rw-   0        0        0     8725 2020-10-12 21:23:24.000000 abtem-1.0.0b9/abtem/plot.py
+-rw-rw-rw-   0        0        0    38134 2020-10-26 09:23:11.000000 abtem-1.0.0b9/abtem/potentials.py
+-rw-rw-rw-   0        0        0    17426 2020-10-17 12:19:45.000000 abtem-1.0.0b9/abtem/scan.py
+-rw-rw-rw-   0        0        0     4729 2020-10-13 22:23:12.000000 abtem-1.0.0b9/abtem/structures.py
+-rw-rw-rw-   0        0        0     5382 2020-09-27 08:24:36.000000 abtem-1.0.0b9/abtem/tanh_sinh.py
+-rw-rw-rw-   0        0        0     5707 2020-10-18 15:22:26.000000 abtem-1.0.0b9/abtem/temperature.py
+-rw-rw-rw-   0        0        0    22812 2020-10-22 18:53:29.000000 abtem-1.0.0b9/abtem/transfer.py
+-rw-rw-rw-   0        0        0     7672 2020-10-23 06:52:43.000000 abtem-1.0.0b9/abtem/utils.py
+drwxrwxrwx   0        0        0        0 2020-10-26 19:40:40.838601 abtem-1.0.0b9/abtem/visualize/
+-rw-rw-rw-   0        0        0       35 2020-10-02 18:09:58.000000 abtem-1.0.0b9/abtem/visualize/__init__.py
+-rw-rw-rw-   0        0        0     4606 2020-10-22 18:35:38.000000 abtem-1.0.0b9/abtem/visualize/bqplot.py
+-rw-rw-rw-   0        0        0     7635 2020-10-22 22:10:19.000000 abtem-1.0.0b9/abtem/visualize/mpl.py
+-rw-rw-rw-   0        0        0     1845 2020-10-08 11:35:08.000000 abtem-1.0.0b9/abtem/visualize/utils.py
+-rw-rw-rw-   0        0        0     2730 2020-10-22 11:01:18.000000 abtem-1.0.0b9/abtem/visualize/widgets.py
+-rw-rw-rw-   0        0        0    64674 2020-10-26 19:38:40.000000 abtem-1.0.0b9/abtem/waves.py
+drwxrwxrwx   0        0        0        0 2020-10-26 19:40:40.812505 abtem-1.0.0b9/abtem.egg-info/
+-rw-rw-rw-   0        0        0     3085 2020-10-26 19:40:40.000000 abtem-1.0.0b9/abtem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1187 2020-10-26 19:40:40.000000 abtem-1.0.0b9/abtem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-10-26 19:40:40.000000 abtem-1.0.0b9/abtem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2020-10-26 19:40:40.000000 abtem-1.0.0b9/abtem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2020-10-26 19:40:40.000000 abtem-1.0.0b9/abtem.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2020-10-26 19:40:40.925694 abtem-1.0.0b9/setup.cfg
+-rw-rw-rw-   0        0        0     1139 2020-08-21 09:45:36.000000 abtem-1.0.0b9/setup.py
+drwxrwxrwx   0        0        0        0 2020-10-26 19:40:40.924703 abtem-1.0.0b9/test/
+-rw-rw-rw-   0        0        0        0 2020-08-12 14:10:11.000000 abtem-1.0.0b9/test/__init__.py
+-rw-rw-rw-   0        0        0      624 2020-08-21 09:45:36.000000 abtem-1.0.0b9/test/conftest.py
+-rw-rw-rw-   0        0        0     1803 2020-10-25 14:24:37.000000 abtem-1.0.0b9/test/test_antialias.py
+-rw-rw-rw-   0        0        0     1509 2020-08-21 09:45:36.000000 abtem-1.0.0b9/test/test_cache.py
+-rw-rw-rw-   0        0        0     1866 2020-08-21 09:45:36.000000 abtem-1.0.0b9/test/test_ctf.py
+-rw-rw-rw-   0        0        0     2172 2020-10-25 17:39:56.000000 abtem-1.0.0b9/test/test_detect.py
+-rw-rw-rw-   0        0        0     2272 2020-08-22 18:38:01.000000 abtem-1.0.0b9/test/test_dft.py
+-rw-rw-rw-   0        0        0     1275 2020-08-21 09:45:36.000000 abtem-1.0.0b9/test/test_energy.py
+-rw-rw-rw-   0        0        0     1219 2020-08-21 09:45:36.000000 abtem-1.0.0b9/test/test_event.py
+-rw-rw-rw-   0        0        0     4074 2020-10-17 12:21:41.000000 abtem-1.0.0b9/test/test_export.py
+-rw-rw-rw-   0        0        0     3550 2020-10-10 16:23:26.000000 abtem-1.0.0b9/test/test_grid.py
+-rw-rw-rw-   0        0        0     2089 2020-10-25 15:04:28.000000 abtem-1.0.0b9/test/test_interpolate.py
+-rw-rw-rw-   0        0        0     1908 2020-10-25 12:12:17.000000 abtem-1.0.0b9/test/test_kirkland.py
+-rw-rw-rw-   0        0        0     3850 2020-10-20 21:52:45.000000 abtem-1.0.0b9/test/test_potential_integration.py
+-rw-rw-rw-   0        0        0      809 2020-08-12 14:10:11.000000 abtem-1.0.0b9/test/test_potential_parametrization.py
+-rw-rw-rw-   0        0        0     2627 2020-10-21 20:54:05.000000 abtem-1.0.0b9/test/test_potentials.py
+-rw-rw-rw-   0        0        0     8381 2020-10-18 12:46:47.000000 abtem-1.0.0b9/test/test_prism.py
+-rw-rw-rw-   0        0        0      773 2020-09-19 11:48:06.000000 abtem-1.0.0b9/test/test_propagator.py
+-rw-rw-rw-   0        0        0     4007 2020-10-08 22:33:51.000000 abtem-1.0.0b9/test/test_scan.py
+-rw-rw-rw-   0        0        0     1736 2020-08-21 09:45:36.000000 abtem-1.0.0b9/test/test_temperature.py
+-rw-rw-rw-   0        0        0     6750 2020-10-10 16:24:26.000000 abtem-1.0.0b9/test/test_waves.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `abtem-1.0.0b8/PKG-INFO` & `abtem-1.0.0b9/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,55 @@
-Metadata-Version: 1.2
-Name: abtem
-Version: 1.0.0b8
-Summary: ab initio Transmission Electron Microscopy
-Home-page: https://github.com/jacobjma/abtem
-Author: Jacob Madsen
-Author-email: jacob.madsen@univie.ac.at
-Maintainer: Jacob Madsen
-Maintainer-email: jacob.madsen@univie.ac.at
-License: UNKNOWN
-Description: # abTEM: ab initio Transmission Electron Microscopy
-        
-        [![PyPI version](https://badge.fury.io/py/abtem.svg)](https://badge.fury.io/py/abtem)
-        [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-        [![Documentation Status](https://readthedocs.org/projects/abtem/badge/?version=latest)](https://abtem.readthedocs.io/en/latest/?badge=latest)
-        [![Gitter](https://badges.gitter.im/abTEM/community.svg)](https://gitter.im/abTEM/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-        
-        [**Docs**](https://abtem.readthedocs.io/en/latest/index.html)
-        | [**Install Guide**](https://abtem.readthedocs.io/en/latest/install.html)
-        | [**Examples**](https://github.com/jacobjma/abTEM/tree/master/examples)
-        | [**Gitter**](https://gitter.im/abTEM/)
-        
-        **This program is under development and subject to changes. Please be aware and report issues.**
-        
-        abTEM provides a Python API for running simulations of (scanning) transmission electron microscopy images and diffraction patterns using the multislice or PRISM algorithms. It is designed to closely integrate with atomistic simulations using the Atomic Simulation Environment (ASE), and to directly use *ab initio* electrostatic potentials from the high-performance density functional theory code GPAW.
-        
-        ## Installation
-        
-        You can install abTEM using `pip`:
-        
-        ```sh
-        $ pip install abtem
-        ```
-        
-        For detailed instructions on installing abTEM, see [the installation guide](https://abtem.readthedocs.io/en/latest/install.html).
-        
-        ## Getting started
-        
-        To get started using abTEM, please visit our [walkthrough](https://abtem.readthedocs.io/en/latest/walkthrough/introduction.html).
-        
-        ## Contact
-        * Chat on [gitter](https://gitter.im/abTEM/)
-        * Write the [maintainer](https://github.com/jacobjma) directly
-        * Bug reports and development: [github issues](https://github.com/jacobjma/abTEM/issues)
-        
-        Please send us bug reports, patches, code, ideas and questions.
-        
-Platform: any
-Requires-Python: >=3.6
+Metadata-Version: 1.2
+Name: abtem
+Version: 1.0.0b9
+Summary: ab initio Transmission Electron Microscopy
+Home-page: https://github.com/jacobjma/abtem
+Author: Jacob Madsen
+Author-email: jacob.madsen@univie.ac.at
+Maintainer: Jacob Madsen
+Maintainer-email: jacob.madsen@univie.ac.at
+License: UNKNOWN
+Description: # abTEM: ab initio Transmission Electron Microscopy
+        
+        [![PyPI version](https://badge.fury.io/py/abtem.svg)](https://badge.fury.io/py/abtem)
+        [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+        [![Documentation Status](https://readthedocs.org/projects/abtem/badge/?version=latest)](https://abtem.readthedocs.io/en/latest/?badge=latest)
+        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jacobjma/abTEM/master?filepath=examples%2Findex.ipynb)
+        [![Gitter](https://badges.gitter.im/abTEM/community.svg)](https://gitter.im/abTEM/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+        
+        [**Docs**](https://abtem.readthedocs.io/en/latest/index.html)
+        | [**Install Guide**](https://abtem.readthedocs.io/en/latest/install.html)
+        | [**Examples**](https://github.com/jacobjma/abTEM/tree/master/examples)
+        | [**Gitter**](https://gitter.im/abTEM/)
+        
+        **This program is under development and subject to changes. Please be aware and report issues.**
+        
+        abTEM provides a Python API for running simulations of (scanning) transmission electron microscopy images and diffraction patterns using the multislice or PRISM algorithms. It is designed to closely integrate with atomistic simulations using the Atomic Simulation Environment (ASE), and to directly use *ab initio* electrostatic potentials from the high-performance density functional theory code GPAW.
+        
+        ## Installation
+        
+        You can install abTEM using `pip`:
+        
+        ```sh
+        $ pip install abtem
+        ```
+        
+        For detailed instructions on installing abTEM, see [the installation guide](https://abtem.readthedocs.io/en/latest/install.html).
+        
+        ## Getting started
+        
+        To get started using abTEM, please visit our [walkthrough](https://abtem.readthedocs.io/en/latest/walkthrough/introduction.html) or check out one of the [examples](https://github.com/jacobjma/abTEM/tree/master/examples).
+        
+        To try abTEM in your webbrowser, click the binder link:
+        
+        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jacobjma/abTEM/master?filepath=examples%2Findex.ipynb)
+        
+        
+        ## Contact
+        * Chat on [gitter](https://gitter.im/abTEM/)
+        * Write the [maintainer](https://github.com/jacobjma) directly
+        * Bug reports and development: [github issues](https://github.com/jacobjma/abTEM/issues)
+        
+        Please send us bug reports, patches, code, ideas and questions.
+        
+Platform: any
+Requires-Python: >=3.6
```

### Comparing `abtem-1.0.0b8/README.md` & `abtem-1.0.0b9/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,42 @@
-# abTEM: ab initio Transmission Electron Microscopy
-
-[![PyPI version](https://badge.fury.io/py/abtem.svg)](https://badge.fury.io/py/abtem)
-[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-[![Documentation Status](https://readthedocs.org/projects/abtem/badge/?version=latest)](https://abtem.readthedocs.io/en/latest/?badge=latest)
-[![Gitter](https://badges.gitter.im/abTEM/community.svg)](https://gitter.im/abTEM/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-
-[**Docs**](https://abtem.readthedocs.io/en/latest/index.html)
-| [**Install Guide**](https://abtem.readthedocs.io/en/latest/install.html)
-| [**Examples**](https://github.com/jacobjma/abTEM/tree/master/examples)
-| [**Gitter**](https://gitter.im/abTEM/)
-
-**This program is under development and subject to changes. Please be aware and report issues.**
-
-abTEM provides a Python API for running simulations of (scanning) transmission electron microscopy images and diffraction patterns using the multislice or PRISM algorithms. It is designed to closely integrate with atomistic simulations using the Atomic Simulation Environment (ASE), and to directly use *ab initio* electrostatic potentials from the high-performance density functional theory code GPAW.
-
-## Installation
-
-You can install abTEM using `pip`:
-
-```sh
-$ pip install abtem
-```
-
-For detailed instructions on installing abTEM, see [the installation guide](https://abtem.readthedocs.io/en/latest/install.html).
-
-## Getting started
-
-To get started using abTEM, please visit our [walkthrough](https://abtem.readthedocs.io/en/latest/walkthrough/introduction.html).
-
-## Contact
-* Chat on [gitter](https://gitter.im/abTEM/)
-* Write the [maintainer](https://github.com/jacobjma) directly
-* Bug reports and development: [github issues](https://github.com/jacobjma/abTEM/issues)
-
-Please send us bug reports, patches, code, ideas and questions.
+# abTEM: ab initio Transmission Electron Microscopy
+
+[![PyPI version](https://badge.fury.io/py/abtem.svg)](https://badge.fury.io/py/abtem)
+[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+[![Documentation Status](https://readthedocs.org/projects/abtem/badge/?version=latest)](https://abtem.readthedocs.io/en/latest/?badge=latest)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jacobjma/abTEM/master?filepath=examples%2Findex.ipynb)
+[![Gitter](https://badges.gitter.im/abTEM/community.svg)](https://gitter.im/abTEM/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+
+[**Docs**](https://abtem.readthedocs.io/en/latest/index.html)
+| [**Install Guide**](https://abtem.readthedocs.io/en/latest/install.html)
+| [**Examples**](https://github.com/jacobjma/abTEM/tree/master/examples)
+| [**Gitter**](https://gitter.im/abTEM/)
+
+**This program is under development and subject to changes. Please be aware and report issues.**
+
+abTEM provides a Python API for running simulations of (scanning) transmission electron microscopy images and diffraction patterns using the multislice or PRISM algorithms. It is designed to closely integrate with atomistic simulations using the Atomic Simulation Environment (ASE), and to directly use *ab initio* electrostatic potentials from the high-performance density functional theory code GPAW.
+
+## Installation
+
+You can install abTEM using `pip`:
+
+```sh
+$ pip install abtem
+```
+
+For detailed instructions on installing abTEM, see [the installation guide](https://abtem.readthedocs.io/en/latest/install.html).
+
+## Getting started
+
+To get started using abTEM, please visit our [walkthrough](https://abtem.readthedocs.io/en/latest/walkthrough/introduction.html) or check out one of the [examples](https://github.com/jacobjma/abTEM/tree/master/examples).
+
+To try abTEM in your webbrowser, click the binder link:
+
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jacobjma/abTEM/master?filepath=examples%2Findex.ipynb)
+
+
+## Contact
+* Chat on [gitter](https://gitter.im/abTEM/)
+* Write the [maintainer](https://github.com/jacobjma) directly
+* Bug reports and development: [github issues](https://github.com/jacobjma/abTEM/issues)
+
+Please send us bug reports, patches, code, ideas and questions.
```

### Comparing `abtem-1.0.0b8/abtem/__init__.py` & `abtem-1.0.0b9/abtem/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-"""Main abTEM module."""
-from abtem import waves
-from abtem.detect import AnnularDetector, FlexibleAnnularDetector, SegmentedDetector, PixelatedDetector, \
-    WavefunctionDetector
-from abtem.plot import show_atoms
-from abtem.potentials import Potential, PotentialArray
-from abtem.scan import GridScan, LineScan
-from abtem.temperature import AbstractFrozenPhonons, FrozenPhonons
-from abtem.transfer import CTF
-from abtem.waves import PlaneWave, Probe, SMatrix, Waves
-from abtem.measure import Measurement
-
-from abtem._version import __version__
+"""Main abTEM module."""
+from abtem import waves
+from abtem.detect import AnnularDetector, FlexibleAnnularDetector, SegmentedDetector, PixelatedDetector, \
+    WavefunctionDetector
+from abtem.visualize.mpl import show_atoms
+from abtem.potentials import Potential, PotentialArray
+from abtem.scan import GridScan, LineScan
+from abtem.temperature import AbstractFrozenPhonons, FrozenPhonons
+from abtem.transfer import CTF
+from abtem.waves import PlaneWave, Probe, SMatrix, Waves
+from abtem.measure import Measurement
+
+from abtem._version import __version__
```

### Comparing `abtem-1.0.0b8/abtem/data/kirkland.txt` & `abtem-1.0.0b9/abtem/data/kirkland.txt`

 * *Ordering differences only*

 * *Files 5% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-From "Advanced Computing in Electron Microscopy", Kirkland E.J., 2nd ed., 2010
-Z,a1,a2,a3,b1,b2,b3,c1,c2,c3,d1,d2,d3
-1,0.0042029832,0.0627762505,0.0300907347,0.225350888,0.22536695,0.225331756,0.0677756695,0.0035660924,0.0276135815,4.38854001,0.403884823,1.44490166
-2,1.87544e-05,0.0004105958,0.196300059,0.212427997,0.332212279,0.517325152,0.0083601574,0.0295102022,4.659e-07,0.366668239,1.37171827,37576.8025
-3,0.0745843816,0.071538225,0.145315229,0.881151424,0.0459142904,0.881301714,1.12125769,0.0025173653,0.358434971,18.8483665,0.159189995,6.12371
-4,0.0611642897,0.125755034,0.200831548,0.0990182132,0.0990272412,1.87392509,0.787242876,0.0015884785,0.273962031,9.32794929,0.0891900236,3.20687658
-5,0.125716066,0.173314452,0.184774811,0.14825883,0.148257216,3.34227311,0.195250221,0.529642075,0.001082305,1.97339463,5.70035553,0.0564857237
-6,0.212080767,0.199811865,0.168254385,0.208605417,0.208610186,5.57870773,0.14204836,0.363830672,0.000835012,1.33311887,3.80800263,0.040398262
-7,0.533015554,0.0529008883,0.0924159648,0.290952515,10.3547896,10.3540028,0.261799101,0.0008802621,0.110166555,2.76252723,0.0347681236,0.993421736
-8,0.339969204,0.307570172,0.130369072,0.38157028,0.381571436,19.1919745,0.0883326058,0.1965867,0.00099622,0.760635525,2.07401094,0.0303266869
-9,0.230560593,0.526889648,0.124346755,0.480754213,0.480763895,39.530672,0.0012461689,0.0720452555,0.153075777,0.0262181803,0.592495593,1.59127671
-10,0.408371771,0.454418858,0.144564923,0.588228627,0.588288655,121.246013,0.0591531395,0.124003718,0.0016498604,0.46396354,1.23413025,0.0205869217
-11,0.136471662,0.770677865,0.156862014,0.0499965301,0.881899664,16.1768579,0.996821513,0.038030467,0.127685089,20.013261,0.260516254,0.699559329
-12,0.304384121,0.756270563,0.101164809,0.0842014377,1.64065598,29.7142975,0.0345203403,0.971751327,0.120593012,0.216596094,12.1236852,0.560865838
-13,0.777419424,0.0578312036,0.426386499,2.71058227,71.7532098,0.0913331555,0.11340722,0.790114035,0.0323293496,0.448867451,8.66366718,0.178503463
-14,1.06543892,0.120143691,0.180915263,1.04118455,68.7113368,0.0887533926,1.1206562,0.0305452816,1.59963502,3.70062619,0.214097897,9.99096638
-15,1.05284447,0.299440284,0.117460748,1.3196259,0.12846052,102.190163,0.960643452,0.0263555748,1.3805933,2.87477555,0.182076844,7.49165526
-16,1.01646916,0.441766748,0.121503863,1.69181965,0.174180288,167.011091,0.82796667,0.0233022533,1.18302846,2.3034281,0.15695415,5.85782891
-17,0.944221116,0.437322049,0.254547926,0.240052374,9.30510439,9.30486346,0.0547763323,0.800087488,0.0107488641,0.168655688,2.97849774,0.0684240646
-18,1.06983288,0.424631786,0.243897949,0.287791022,12.4156957,12.4158868,0.0479446296,0.764958952,0.0082312843,0.136979796,2.43940729,0.0527258749
-19,0.692717865,0.965161085,0.148466588,7.1084999,0.357532901,0.0393763275,0.0264645027,1.80883768,0.543900018,0.103591321,32.2845199,1.67791374
-20,0.366902871,0.866378999,0.6672033,0.0614274129,0.570881727,7.82965639,0.487743636,1.82406314,0.0220248453,1.32531318,21.0056032,0.091185345
-21,0.378871777,0.900022505,0.715288914,0.0698910162,0.521061541,7.8770792,0.0188640973,0.407945949,1.6178654,0.0817512708,1.11141388,18.0840759
-22,0.362383267,0.984232966,0.741715642,0.0754707114,0.497757309,8.17659391,0.362555269,1.4915939,0.0161659509,0.955524906,16.2221677,0.0733140839
-23,0.352961378,0.746791014,1.08364068,0.0819204103,8.81189511,0.510646075,1.3901361,0.331273356,0.0140422612,14.8901841,0.838543079,0.0657432678
-24,1.34348379,0.507040328,0.426358955,1.25814353,11.5042811,0.0853660389,0.0117241826,0.511966516,0.338285828,0.0600177061,1.53772451,0.662418319
-25,0.326697613,0.717297,1.33212464,0.0888813083,11.1300198,0.582141104,0.280801702,1.15499241,0.0111984488,0.671583145,12.6825395,0.0532334467
-26,0.313454847,0.689290016,1.47141531,0.0899325756,13.0366038,0.633345291,1.03298688,0.258280285,0.010346069,11.6783425,0.609116446,0.0481610627
-27,0.315878278,1.60139005,0.656394338,0.0946683246,0.699436449,15.6954403,0.936746624,0.0097756265,0.238378578,10.939241,0.0437446816,0.556286483
-28,1.7225463,0.329543044,0.6230072,0.776606908,0.10226236,19.4156207,0.0094349651,0.854063515,0.221073515,0.0398684596,10.4078166,0.51086933
-29,0.358774531,1.76181348,0.636905053,0.106153463,1.01640995,15.3659093,0.0074493067,0.189002347,0.229619589,0.0385345989,0.39842779,0.901419843
-30,0.570893973,1.98908856,0.306060585,0.126534614,2.17781965,37.8619003,0.235600223,0.397061102,0.0068565723,0.367019041,0.866419596,0.0335778823
-31,0.625528464,2.05302901,0.28960812,0.11000565,2.41095786,47.8685736,0.207910594,0.345079617,0.006556343,0.327807224,0.743139061,0.0309411369
-32,0.59095269,0.53998066,2.00626188,0.118375976,71.8937433,1.39304889,0.749705041,0.183581347,0.0095219074,6.8994335,0.364667232,0.026988865
-33,0.777875218,0.59384815,1.95918751,0.150733157,142.882209,1.74750339,0.179880226,0.863267222,0.0095905343,0.331800852,5.85490274,0.0233777569
-34,0.958390681,0.603851342,1.90828931,0.183775557,196.819224,2.15082053,0.173885956,0.935265145,0.0086225466,0.300006024,4.92471215,0.0212308108
-35,1.1413617,0.518118737,1.85731975,0.21870871,193.916682,2.65755396,0.168217399,0.975705606,0.0072418787,0.271719918,4.194825,0.0199325718
-36,0.32438697,1.31732163,1.79912614,63.1317973,0.254706036,3.23668394,0.0042996143,1.00429433,0.162188197,0.019896561,3.61094513,0.245583672
-37,0.290445351,2.44201329,0.769435449,0.0368420227,1.16013332,16.9591472,1.58687,0.0028161759,0.12866383,2.53082574,0.0188577417,0.210753969
-38,0.0137373086,1.97548672,1.59261029,0.0187469061,6.3607923,0.221992482,0.173263882,4.66280378,0.0016126506,0.201624958,25.3027803,0.0153610568
-39,0.675302747,0.47028672,2.63497677,0.0654331847,106.108709,2.0664354,0.109621746,0.960348773,0.0052892156,0.193131925,1.63310938,0.0166083821
-40,2.64365505,0.554225147,0.761376625,2.20202699,178.260107,0.0767218745,0.0060294689,0.099163053,0.95678202,0.0155143296,0.176175995,1.54330682
-41,0.659532875,1.84545854,1.25584405,0.086614549,5.94774398,0.640851475,0.122253422,0.706638328,0.0026238159,0.16664605,1.62853268,0.0082625786
-42,0.61016012,1.26544,1.97428762,0.0911628054,0.506776025,5.89590381,0.648028962,0.0026038082,0.113887493,1.46634108,0.0078433631,0.15511434
-43,0.855189183,1.66219641,1.45575475,0.102962151,7.64907,1.01639987,0.105445664,0.771657112,0.0022099264,0.142303338,1.34659349,0.0079035898
-44,0.470847093,1.58180781,2.02419818,0.0933029874,0.452831347,7.11489023,0.0019703626,0.626912639,0.10264132,0.007561816,1.25399858,0.133786087
-45,0.420051553,1.76266507,2.02735641,0.0938882628,0.464441687,8.19346046,0.0014548718,0.6228096,0.0991529915,0.0078270452,1.17194153,0.124532839
-46,2.10475155,2.03884487,0.182067264,8.6860647,0.378924449,0.142921634,0.0952040948,0.591445248,0.0011332868,0.1171259,1.07843808,0.0078025209
-47,2.0798139,0.443170726,1.96515215,9.92540297,0.104920104,0.640103839,0.596130591,0.478016333,0.094645847,0.88959479,1.98509407,0.112744464
-48,1.63657549,2.17927989,0.77130069,12.4540381,1.4513466,0.126695757,0.66419388,0.764563285,0.0861126689,0.777659202,1.6607521,0.105728357
-49,2.24820632,1.64706864,0.788679265,1.51913507,13.0113424,0.106128184,0.0812579069,0.668280346,0.638467475,0.099404562,1.49742063,0.718422635
-50,2.1664462,0.688691021,1.92431751,11.3174909,0.110131285,0.674464853,0.565359888,0.918683861,0.0780542213,0.73356461,10.2310312,0.0931104308
-51,1.73662114,0.99987138,2.13972409,0.884334719,0.138462121,11.9666432,0.560566526,0.993772747,0.0737374982,0.67267288,8.72330411,0.0878577715
-52,2.09383882,1.56940519,1.30941993,12.6856869,1.21236537,0.166633292,0.0698067804,1.04969537,0.555594354,0.0830817576,7.43147857,0.617487676
-53,1.60186925,1.98510264,1.482262,0.195031538,13.6976183,1.80304795,0.553807199,1.11728722,0.0660720847,0.56791234,6.40879878,0.0786615429
-54,1.60015487,1.71644581,1.84968351,2.92913354,15.588299,0.222525983,0.0623813648,1.21387555,0.554051946,0.0745581223,5.56013271,0.521994521
-55,2.95236854,0.428105721,1.89599233,6.01461952,46.4151246,0.180109756,0.0548012938,4.708386,0.590356719,0.0712799633,45.6702799,0.47023631
-56,3.19434243,1.98289586,0.155121052,9.27352241,0.228741632,0.0382000231,0.0673222354,4.48474211,0.542674414,0.0730961745,29.5703565,0.408647015
-57,2.05036425,0.142114311,3.23538151,0.220348417,0.0396438056,9.56979169,0.0634683429,3.97960586,0.520116711,0.0692443091,25.3178406,0.383614098
-58,3.22990759,0.157618307,2.13477838,9.94660135,0.0415378676,0.240480572,0.501907609,3.8088901,0.0596625028,0.366252019,24.3275968,0.0659653503
-59,0.158189324,3.18141995,2.2762214,0.0391309056,10.4139545,0.281671757,3.97705472,0.0558448277,0.485207954,26.1872978,0.0630921695,0.354234369
-60,0.181379417,3.17616396,2.35221519,0.0437324793,10.7842572,0.305571833,3.83125763,0.0525889976,0.470090742,25.4745408,0.0602676073,0.339017003
-61,0.192986811,2.43756023,3.17248504,0.043778597,0.329336996,11.1259996,3.58105414,0.456529394,0.0494812177,24.6709586,0.324990282,0.05765531
-62,0.212002595,3.16891754,2.51503494,0.0457703608,11.4536599,0.355561054,0.444080845,3.36742101,0.0465652543,0.311953363,24.0291435,0.0552266819
-63,2.59355002,3.16557522,0.229402652,0.382452612,11.7675155,0.0476642249,0.43225778,3.1726192,0.0437958317,0.299719833,23.4462738,0.052944068
-64,3.19144939,2.55766431,0.332681934,12.0224655,0.408338876,0.0585819814,0.041424313,2.61036728,0.420526863,0.0506771477,19.9344244,0.28568624
-65,0.259407462,3.16177855,2.75095751,0.0504689354,12.3140183,0.438337626,2.79247686,0.0385931001,0.410881708,22.3797309,0.0487920992,0.277622892
-66,3.16055396,2.82751709,0.275140255,12.5470414,0.467899094,0.0523226982,0.40096716,2.63110834,0.0361333817,0.267614884,21.9498166,0.0468871497
-67,0.288642467,2.90567296,3.15960159,0.0540507687,0.497581077,12.7599505,0.391280259,2.48596038,0.0337664478,0.258151831,21.5400972,0.0450664323
-68,3.15573213,0.31151956,2.97722406,12.9729009,0.0581399387,0.531213394,0.381563854,2.40247532,0.0315224214,0.249195776,21.3627616,0.0433253257
-69,3.1559197,0.32254471,3.05569053,13.1232407,0.0597223323,0.561876773,0.02928451,0.372487205,2.27833695,0.0416534255,0.240821967,21.0034185
-70,3.10794704,3.14091221,0.375660454,0.606347847,13.3705269,0.072981474,0.361901097,2.45409082,0.027238399,0.232652051,21.2695209,0.0399969597
-71,3.11446863,0.539634353,3.06460915,13.8968881,0.0891708508,0.679919563,0.0258563745,2.13983556,0.347788231,0.0382808522,18.0078788,0.222706591
-72,3.01166899,3.16284788,0.633421771,0.710401889,13.8262192,0.0948486572,0.341417198,1.53566013,0.0240723773,0.214129678,15.5298698,0.036783369
-73,3.20236821,0.830098413,2.86552297,13.8446369,0.118381581,0.766369118,0.0224813887,1.40165263,0.333740596,0.0352934622,14.6148877,0.205704486
-74,0.924906855,2.75554557,3.3044006,0.128663377,0.765826479,13.447117,0.329973862,1.09916444,0.0206498883,0.198218895,13.5087534,0.0338918459
-75,1.96952105,1.21726619,4.10391685,49.883062,0.133243809,1.84396916,0.0290791978,0.230696669,0.608840299,0.0284192813,0.190968784,1.37090356
-76,2.06385867,1.29603406,3.96920673,40.5671697,0.146559047,1.82561596,0.0269835487,0.231083999,0.630466774,0.0284172045,0.179765184,1.38911543
-77,2.21522726,1.37573155,3.78244405,32.446409,0.160920048,1.78756553,0.024464324,0.236932016,0.648471412,0.0282909938,0.170692368,1.3792839
-78,0.98469794,2.73987079,3.61696715,0.160910839,0.718971667,12.9281016,0.302885602,0.278370726,0.0152124129,0.170134854,1.49862703,0.0283510822
-79,0.961263398,3.6958103,2.77567491,0.170932277,12.9335319,0.68999707,0.295414176,0.311475743,0.0143237267,0.16352551,1.39200901,0.0271265337
-80,1.29200491,2.75161478,3.49387949,0.183432865,0.942368371,14.6235654,0.277304636,0.43023281,0.0148294351,0.155110144,1.2887167,0.0261903834
-81,3.7596473,3.21195904,0.647767825,13.5041513,0.666330993,0.0922518234,0.276123274,0.31883881,0.0131668419,0.150312897,1.12565588,0.0248879842
-82,1.00795975,3.09796153,3.61296864,0.117268427,0.880453235,14.7325812,0.262401476,0.405621995,0.0131812509,0.143491014,1.04103506,0.0239575415
-83,1.59826875,4.38233925,2.06074719,0.156897471,2.47094692,57.2438972,0.194426023,0.822704978,0.0233226953,0.132979109,0.956532528,0.0223038435
-84,1.71463223,2.1411596,4.37512413,97.9262841,0.210193717,3.66948812,0.021621668,0.197843837,0.65204792,0.0198456144,0.133758807,0.780432104
-85,1.48047794,2.0917463,4.75246033,125.943919,0.183803008,4.19890596,0.0185643958,0.205859375,0.713540948,0.0181383503,0.133035404,0.703031938
-86,0.630022295,3.80962881,3.89756067,0.140909762,30.851554,0.651559763,0.2407551,2.62868577,0.0314285931,0.108899672,6.42383261,0.0242346699
-87,5.23288135,2.48604205,0.323431354,8.60599536,0.304543982,0.0387759096,0.255403596,0.553607228,0.0057527889,0.128717724,0.536977452,0.012941779
-88,1.44192685,3.55291725,3.91259586,0.118740873,1.0173975,63.1814783,0.216173519,3.94191605,0.0460422605,0.0955806441,35.0602732,0.0220850385
-89,1.45864127,4.18945405,3.65866182,0.107760494,88.9090649,1.05088931,0.208479229,3.16528117,0.0523892556,0.0909335557,31.3297788,0.0208807697
-90,1.19014064,2.55380607,4.68110181,0.0773468729,0.659693681,12.8013896,0.226121303,0.358250545,0.0078226395,0.108632194,0.456765664,0.0162623474
-91,4.68537504,2.98413708,0.891988061,14.4503632,0.556438592,0.0669512914,0.224825384,0.304444846,0.0094816271,0.103235396,0.427255647,0.0177730611
-92,4.63343606,3.18157056,0.876455075,16.3377267,0.569517868,0.0688860012,0.221685477,0.2729171,0.0111737298,0.098425455,0.409470917,0.018621541
-93,4.56773888,3.40325179,0.861841923,19.0992795,0.590099634,0.0703204851,0.21972887,0.238176903,0.0138306499,0.093633428,0.393554882,0.0194437286
-94,5.45671123,0.111687906,3.30260343,10.189272,0.0398131313,0.314622212,0.184568319,0.493644263,3.57484743,0.10422086,0.46308054,21.9369542
-95,5.38321999,0.123343236,3.4646909,10.7289857,0.0415137806,0.339326208,0.175437132,3.39800073,0.469459519,0.0998932346,21.1601535,0.45199697
-96,5.38402377,3.49861264,0.188039547,11.1211419,0.35675021,0.0539853583,0.169143137,3.19595016,0.464393059,0.0960082633,18.0694389,0.436318197
-97,3.66090688,0.203054678,5.30697515,0.384420906,0.0548547131,11.7150262,0.160934046,3.04808401,0.443610295,0.0921020329,17.3525367,0.427132359
-98,3.9415039,5.16915345,0.161941074,0.418246722,12.5201788,0.0481540117,0.415299561,2.91761325,0.151474927,0.424913856,19.0899693,0.0881568925
-99,4.09780623,5.10079393,0.174617289,0.446021145,13.1768613,0.0502742829,2.76774658,0.144496639,0.402772109,18.4815393,0.0846232592,0.4176401
-100,4.2493482,5.03556594,0.188920613,0.475263933,13.8570834,0.0526975158,0.394356058,2.612131,0.138001927,0.411193751,17.8537905,0.0812774434
-101,0.200942931,4.40119869,4.97250102,0.0548366518,0.504248434,14.5721366,2.47530599,0.386883197,0.131936095,17.2978308,0.405043898,0.0780821071
-102,0.216052899,4.91106799,4.5486287,0.0583584058,15.3264212,0.53443476,2.36114249,0.126277292,0.381364501,16.8164803,0.0750304633,0.399305852
-103,4.86738014,0.319974401,4.58872425,16.032052,0.0670871138,0.577039373,0.121482448,2.31639872,0.379258137,0.0722275899,14.1279737,0.389973484
+From "Advanced Computing in Electron Microscopy", Kirkland E.J., 2nd ed., 2010
+Z,a1,a2,a3,b1,b2,b3,c1,c2,c3,d1,d2,d3
+1,0.0042029832,0.0627762505,0.0300907347,0.225350888,0.22536695,0.225331756,0.0677756695,0.0035660924,0.0276135815,4.38854001,0.403884823,1.44490166
+2,1.87544e-05,0.0004105958,0.196300059,0.212427997,0.332212279,0.517325152,0.0083601574,0.0295102022,4.659e-07,0.366668239,1.37171827,37576.8025
+3,0.0745843816,0.071538225,0.145315229,0.881151424,0.0459142904,0.881301714,1.12125769,0.0025173653,0.358434971,18.8483665,0.159189995,6.12371
+4,0.0611642897,0.125755034,0.200831548,0.0990182132,0.0990272412,1.87392509,0.787242876,0.0015884785,0.273962031,9.32794929,0.0891900236,3.20687658
+5,0.125716066,0.173314452,0.184774811,0.14825883,0.148257216,3.34227311,0.195250221,0.529642075,0.001082305,1.97339463,5.70035553,0.0564857237
+6,0.212080767,0.199811865,0.168254385,0.208605417,0.208610186,5.57870773,0.14204836,0.363830672,0.000835012,1.33311887,3.80800263,0.040398262
+7,0.533015554,0.0529008883,0.0924159648,0.290952515,10.3547896,10.3540028,0.261799101,0.0008802621,0.110166555,2.76252723,0.0347681236,0.993421736
+8,0.339969204,0.307570172,0.130369072,0.38157028,0.381571436,19.1919745,0.0883326058,0.1965867,0.00099622,0.760635525,2.07401094,0.0303266869
+9,0.230560593,0.526889648,0.124346755,0.480754213,0.480763895,39.530672,0.0012461689,0.0720452555,0.153075777,0.0262181803,0.592495593,1.59127671
+10,0.408371771,0.454418858,0.144564923,0.588228627,0.588288655,121.246013,0.0591531395,0.124003718,0.0016498604,0.46396354,1.23413025,0.0205869217
+11,0.136471662,0.770677865,0.156862014,0.0499965301,0.881899664,16.1768579,0.996821513,0.038030467,0.127685089,20.013261,0.260516254,0.699559329
+12,0.304384121,0.756270563,0.101164809,0.0842014377,1.64065598,29.7142975,0.0345203403,0.971751327,0.120593012,0.216596094,12.1236852,0.560865838
+13,0.777419424,0.0578312036,0.426386499,2.71058227,71.7532098,0.0913331555,0.11340722,0.790114035,0.0323293496,0.448867451,8.66366718,0.178503463
+14,1.06543892,0.120143691,0.180915263,1.04118455,68.7113368,0.0887533926,1.1206562,0.0305452816,1.59963502,3.70062619,0.214097897,9.99096638
+15,1.05284447,0.299440284,0.117460748,1.3196259,0.12846052,102.190163,0.960643452,0.0263555748,1.3805933,2.87477555,0.182076844,7.49165526
+16,1.01646916,0.441766748,0.121503863,1.69181965,0.174180288,167.011091,0.82796667,0.0233022533,1.18302846,2.3034281,0.15695415,5.85782891
+17,0.944221116,0.437322049,0.254547926,0.240052374,9.30510439,9.30486346,0.0547763323,0.800087488,0.0107488641,0.168655688,2.97849774,0.0684240646
+18,1.06983288,0.424631786,0.243897949,0.287791022,12.4156957,12.4158868,0.0479446296,0.764958952,0.0082312843,0.136979796,2.43940729,0.0527258749
+19,0.692717865,0.965161085,0.148466588,7.1084999,0.357532901,0.0393763275,0.0264645027,1.80883768,0.543900018,0.103591321,32.2845199,1.67791374
+20,0.366902871,0.866378999,0.6672033,0.0614274129,0.570881727,7.82965639,0.487743636,1.82406314,0.0220248453,1.32531318,21.0056032,0.091185345
+21,0.378871777,0.900022505,0.715288914,0.0698910162,0.521061541,7.8770792,0.0188640973,0.407945949,1.6178654,0.0817512708,1.11141388,18.0840759
+22,0.362383267,0.984232966,0.741715642,0.0754707114,0.497757309,8.17659391,0.362555269,1.4915939,0.0161659509,0.955524906,16.2221677,0.0733140839
+23,0.352961378,0.746791014,1.08364068,0.0819204103,8.81189511,0.510646075,1.3901361,0.331273356,0.0140422612,14.8901841,0.838543079,0.0657432678
+24,1.34348379,0.507040328,0.426358955,1.25814353,11.5042811,0.0853660389,0.0117241826,0.511966516,0.338285828,0.0600177061,1.53772451,0.662418319
+25,0.326697613,0.717297,1.33212464,0.0888813083,11.1300198,0.582141104,0.280801702,1.15499241,0.0111984488,0.671583145,12.6825395,0.0532334467
+26,0.313454847,0.689290016,1.47141531,0.0899325756,13.0366038,0.633345291,1.03298688,0.258280285,0.010346069,11.6783425,0.609116446,0.0481610627
+27,0.315878278,1.60139005,0.656394338,0.0946683246,0.699436449,15.6954403,0.936746624,0.0097756265,0.238378578,10.939241,0.0437446816,0.556286483
+28,1.7225463,0.329543044,0.6230072,0.776606908,0.10226236,19.4156207,0.0094349651,0.854063515,0.221073515,0.0398684596,10.4078166,0.51086933
+29,0.358774531,1.76181348,0.636905053,0.106153463,1.01640995,15.3659093,0.0074493067,0.189002347,0.229619589,0.0385345989,0.39842779,0.901419843
+30,0.570893973,1.98908856,0.306060585,0.126534614,2.17781965,37.8619003,0.235600223,0.397061102,0.0068565723,0.367019041,0.866419596,0.0335778823
+31,0.625528464,2.05302901,0.28960812,0.11000565,2.41095786,47.8685736,0.207910594,0.345079617,0.006556343,0.327807224,0.743139061,0.0309411369
+32,0.59095269,0.53998066,2.00626188,0.118375976,71.8937433,1.39304889,0.749705041,0.183581347,0.0095219074,6.8994335,0.364667232,0.026988865
+33,0.777875218,0.59384815,1.95918751,0.150733157,142.882209,1.74750339,0.179880226,0.863267222,0.0095905343,0.331800852,5.85490274,0.0233777569
+34,0.958390681,0.603851342,1.90828931,0.183775557,196.819224,2.15082053,0.173885956,0.935265145,0.0086225466,0.300006024,4.92471215,0.0212308108
+35,1.1413617,0.518118737,1.85731975,0.21870871,193.916682,2.65755396,0.168217399,0.975705606,0.0072418787,0.271719918,4.194825,0.0199325718
+36,0.32438697,1.31732163,1.79912614,63.1317973,0.254706036,3.23668394,0.0042996143,1.00429433,0.162188197,0.019896561,3.61094513,0.245583672
+37,0.290445351,2.44201329,0.769435449,0.0368420227,1.16013332,16.9591472,1.58687,0.0028161759,0.12866383,2.53082574,0.0188577417,0.210753969
+38,0.0137373086,1.97548672,1.59261029,0.0187469061,6.3607923,0.221992482,0.173263882,4.66280378,0.0016126506,0.201624958,25.3027803,0.0153610568
+39,0.675302747,0.47028672,2.63497677,0.0654331847,106.108709,2.0664354,0.109621746,0.960348773,0.0052892156,0.193131925,1.63310938,0.0166083821
+40,2.64365505,0.554225147,0.761376625,2.20202699,178.260107,0.0767218745,0.0060294689,0.099163053,0.95678202,0.0155143296,0.176175995,1.54330682
+41,0.659532875,1.84545854,1.25584405,0.086614549,5.94774398,0.640851475,0.122253422,0.706638328,0.0026238159,0.16664605,1.62853268,0.0082625786
+42,0.61016012,1.26544,1.97428762,0.0911628054,0.506776025,5.89590381,0.648028962,0.0026038082,0.113887493,1.46634108,0.0078433631,0.15511434
+43,0.855189183,1.66219641,1.45575475,0.102962151,7.64907,1.01639987,0.105445664,0.771657112,0.0022099264,0.142303338,1.34659349,0.0079035898
+44,0.470847093,1.58180781,2.02419818,0.0933029874,0.452831347,7.11489023,0.0019703626,0.626912639,0.10264132,0.007561816,1.25399858,0.133786087
+45,0.420051553,1.76266507,2.02735641,0.0938882628,0.464441687,8.19346046,0.0014548718,0.6228096,0.0991529915,0.0078270452,1.17194153,0.124532839
+46,2.10475155,2.03884487,0.182067264,8.6860647,0.378924449,0.142921634,0.0952040948,0.591445248,0.0011332868,0.1171259,1.07843808,0.0078025209
+47,2.0798139,0.443170726,1.96515215,9.92540297,0.104920104,0.640103839,0.596130591,0.478016333,0.094645847,0.88959479,1.98509407,0.112744464
+48,1.63657549,2.17927989,0.77130069,12.4540381,1.4513466,0.126695757,0.66419388,0.764563285,0.0861126689,0.777659202,1.6607521,0.105728357
+49,2.24820632,1.64706864,0.788679265,1.51913507,13.0113424,0.106128184,0.0812579069,0.668280346,0.638467475,0.099404562,1.49742063,0.718422635
+50,2.1664462,0.688691021,1.92431751,11.3174909,0.110131285,0.674464853,0.565359888,0.918683861,0.0780542213,0.73356461,10.2310312,0.0931104308
+51,1.73662114,0.99987138,2.13972409,0.884334719,0.138462121,11.9666432,0.560566526,0.993772747,0.0737374982,0.67267288,8.72330411,0.0878577715
+52,2.09383882,1.56940519,1.30941993,12.6856869,1.21236537,0.166633292,0.0698067804,1.04969537,0.555594354,0.0830817576,7.43147857,0.617487676
+53,1.60186925,1.98510264,1.482262,0.195031538,13.6976183,1.80304795,0.553807199,1.11728722,0.0660720847,0.56791234,6.40879878,0.0786615429
+54,1.60015487,1.71644581,1.84968351,2.92913354,15.588299,0.222525983,0.0623813648,1.21387555,0.554051946,0.0745581223,5.56013271,0.521994521
+55,2.95236854,0.428105721,1.89599233,6.01461952,46.4151246,0.180109756,0.0548012938,4.708386,0.590356719,0.0712799633,45.6702799,0.47023631
+56,3.19434243,1.98289586,0.155121052,9.27352241,0.228741632,0.0382000231,0.0673222354,4.48474211,0.542674414,0.0730961745,29.5703565,0.408647015
+57,2.05036425,0.142114311,3.23538151,0.220348417,0.0396438056,9.56979169,0.0634683429,3.97960586,0.520116711,0.0692443091,25.3178406,0.383614098
+58,3.22990759,0.157618307,2.13477838,9.94660135,0.0415378676,0.240480572,0.501907609,3.8088901,0.0596625028,0.366252019,24.3275968,0.0659653503
+59,0.158189324,3.18141995,2.2762214,0.0391309056,10.4139545,0.281671757,3.97705472,0.0558448277,0.485207954,26.1872978,0.0630921695,0.354234369
+60,0.181379417,3.17616396,2.35221519,0.0437324793,10.7842572,0.305571833,3.83125763,0.0525889976,0.470090742,25.4745408,0.0602676073,0.339017003
+61,0.192986811,2.43756023,3.17248504,0.043778597,0.329336996,11.1259996,3.58105414,0.456529394,0.0494812177,24.6709586,0.324990282,0.05765531
+62,0.212002595,3.16891754,2.51503494,0.0457703608,11.4536599,0.355561054,0.444080845,3.36742101,0.0465652543,0.311953363,24.0291435,0.0552266819
+63,2.59355002,3.16557522,0.229402652,0.382452612,11.7675155,0.0476642249,0.43225778,3.1726192,0.0437958317,0.299719833,23.4462738,0.052944068
+64,3.19144939,2.55766431,0.332681934,12.0224655,0.408338876,0.0585819814,0.041424313,2.61036728,0.420526863,0.0506771477,19.9344244,0.28568624
+65,0.259407462,3.16177855,2.75095751,0.0504689354,12.3140183,0.438337626,2.79247686,0.0385931001,0.410881708,22.3797309,0.0487920992,0.277622892
+66,3.16055396,2.82751709,0.275140255,12.5470414,0.467899094,0.0523226982,0.40096716,2.63110834,0.0361333817,0.267614884,21.9498166,0.0468871497
+67,0.288642467,2.90567296,3.15960159,0.0540507687,0.497581077,12.7599505,0.391280259,2.48596038,0.0337664478,0.258151831,21.5400972,0.0450664323
+68,3.15573213,0.31151956,2.97722406,12.9729009,0.0581399387,0.531213394,0.381563854,2.40247532,0.0315224214,0.249195776,21.3627616,0.0433253257
+69,3.1559197,0.32254471,3.05569053,13.1232407,0.0597223323,0.561876773,0.02928451,0.372487205,2.27833695,0.0416534255,0.240821967,21.0034185
+70,3.10794704,3.14091221,0.375660454,0.606347847,13.3705269,0.072981474,0.361901097,2.45409082,0.027238399,0.232652051,21.2695209,0.0399969597
+71,3.11446863,0.539634353,3.06460915,13.8968881,0.0891708508,0.679919563,0.0258563745,2.13983556,0.347788231,0.0382808522,18.0078788,0.222706591
+72,3.01166899,3.16284788,0.633421771,0.710401889,13.8262192,0.0948486572,0.341417198,1.53566013,0.0240723773,0.214129678,15.5298698,0.036783369
+73,3.20236821,0.830098413,2.86552297,13.8446369,0.118381581,0.766369118,0.0224813887,1.40165263,0.333740596,0.0352934622,14.6148877,0.205704486
+74,0.924906855,2.75554557,3.3044006,0.128663377,0.765826479,13.447117,0.329973862,1.09916444,0.0206498883,0.198218895,13.5087534,0.0338918459
+75,1.96952105,1.21726619,4.10391685,49.883062,0.133243809,1.84396916,0.0290791978,0.230696669,0.608840299,0.0284192813,0.190968784,1.37090356
+76,2.06385867,1.29603406,3.96920673,40.5671697,0.146559047,1.82561596,0.0269835487,0.231083999,0.630466774,0.0284172045,0.179765184,1.38911543
+77,2.21522726,1.37573155,3.78244405,32.446409,0.160920048,1.78756553,0.024464324,0.236932016,0.648471412,0.0282909938,0.170692368,1.3792839
+78,0.98469794,2.73987079,3.61696715,0.160910839,0.718971667,12.9281016,0.302885602,0.278370726,0.0152124129,0.170134854,1.49862703,0.0283510822
+79,0.961263398,3.6958103,2.77567491,0.170932277,12.9335319,0.68999707,0.295414176,0.311475743,0.0143237267,0.16352551,1.39200901,0.0271265337
+80,1.29200491,2.75161478,3.49387949,0.183432865,0.942368371,14.6235654,0.277304636,0.43023281,0.0148294351,0.155110144,1.2887167,0.0261903834
+81,3.7596473,3.21195904,0.647767825,13.5041513,0.666330993,0.0922518234,0.276123274,0.31883881,0.0131668419,0.150312897,1.12565588,0.0248879842
+82,1.00795975,3.09796153,3.61296864,0.117268427,0.880453235,14.7325812,0.262401476,0.405621995,0.0131812509,0.143491014,1.04103506,0.0239575415
+83,1.59826875,4.38233925,2.06074719,0.156897471,2.47094692,57.2438972,0.194426023,0.822704978,0.0233226953,0.132979109,0.956532528,0.0223038435
+84,1.71463223,2.1411596,4.37512413,97.9262841,0.210193717,3.66948812,0.021621668,0.197843837,0.65204792,0.0198456144,0.133758807,0.780432104
+85,1.48047794,2.0917463,4.75246033,125.943919,0.183803008,4.19890596,0.0185643958,0.205859375,0.713540948,0.0181383503,0.133035404,0.703031938
+86,0.630022295,3.80962881,3.89756067,0.140909762,30.851554,0.651559763,0.2407551,2.62868577,0.0314285931,0.108899672,6.42383261,0.0242346699
+87,5.23288135,2.48604205,0.323431354,8.60599536,0.304543982,0.0387759096,0.255403596,0.553607228,0.0057527889,0.128717724,0.536977452,0.012941779
+88,1.44192685,3.55291725,3.91259586,0.118740873,1.0173975,63.1814783,0.216173519,3.94191605,0.0460422605,0.0955806441,35.0602732,0.0220850385
+89,1.45864127,4.18945405,3.65866182,0.107760494,88.9090649,1.05088931,0.208479229,3.16528117,0.0523892556,0.0909335557,31.3297788,0.0208807697
+90,1.19014064,2.55380607,4.68110181,0.0773468729,0.659693681,12.8013896,0.226121303,0.358250545,0.0078226395,0.108632194,0.456765664,0.0162623474
+91,4.68537504,2.98413708,0.891988061,14.4503632,0.556438592,0.0669512914,0.224825384,0.304444846,0.0094816271,0.103235396,0.427255647,0.0177730611
+92,4.63343606,3.18157056,0.876455075,16.3377267,0.569517868,0.0688860012,0.221685477,0.2729171,0.0111737298,0.098425455,0.409470917,0.018621541
+93,4.56773888,3.40325179,0.861841923,19.0992795,0.590099634,0.0703204851,0.21972887,0.238176903,0.0138306499,0.093633428,0.393554882,0.0194437286
+94,5.45671123,0.111687906,3.30260343,10.189272,0.0398131313,0.314622212,0.184568319,0.493644263,3.57484743,0.10422086,0.46308054,21.9369542
+95,5.38321999,0.123343236,3.4646909,10.7289857,0.0415137806,0.339326208,0.175437132,3.39800073,0.469459519,0.0998932346,21.1601535,0.45199697
+96,5.38402377,3.49861264,0.188039547,11.1211419,0.35675021,0.0539853583,0.169143137,3.19595016,0.464393059,0.0960082633,18.0694389,0.436318197
+97,3.66090688,0.203054678,5.30697515,0.384420906,0.0548547131,11.7150262,0.160934046,3.04808401,0.443610295,0.0921020329,17.3525367,0.427132359
+98,3.9415039,5.16915345,0.161941074,0.418246722,12.5201788,0.0481540117,0.415299561,2.91761325,0.151474927,0.424913856,19.0899693,0.0881568925
+99,4.09780623,5.10079393,0.174617289,0.446021145,13.1768613,0.0502742829,2.76774658,0.144496639,0.402772109,18.4815393,0.0846232592,0.4176401
+100,4.2493482,5.03556594,0.188920613,0.475263933,13.8570834,0.0526975158,0.394356058,2.612131,0.138001927,0.411193751,17.8537905,0.0812774434
+101,0.200942931,4.40119869,4.97250102,0.0548366518,0.504248434,14.5721366,2.47530599,0.386883197,0.131936095,17.2978308,0.405043898,0.0780821071
+102,0.216052899,4.91106799,4.5486287,0.0583584058,15.3264212,0.53443476,2.36114249,0.126277292,0.381364501,16.8164803,0.0750304633,0.399305852
+103,4.86738014,0.319974401,4.58872425,16.032052,0.0670871138,0.577039373,0.121482448,2.31639872,0.379258137,0.0722275899,14.1279737,0.389973484
```

### Comparing `abtem-1.0.0b8/abtem/data/lobato.txt` & `abtem-1.0.0b9/abtem/data/lobato.txt`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,105 +1,105 @@
-From "An accurate parameterization for scattering factors, electron densities and electrostatic potentials for neutral atoms that obey all physical constraints", Lobato I. and van Dyck D., Acta Cryst. 70:636-649, 2014
-Z,a1,a2,a3,a4,a5,b1,b2,b3,b4,b5
-1,0.00647384848835291,-0.49019257678022900,0.57328416039087600,-0.37940330148399000,0.55442647477407900,2.78519885379148000,2.77620428330644000,2.77538591050625000,2.76759302867258000,2.76511897642927000
-2,3.05745116099835000,-62.00447791273250000,64.00555370846140000,-5.00132578542780000,0.15179882870052600,1.08967248726078000,0.93983879814312100,0.92528903438626500,0.82294749870865000,0.57739311067540200
-3,3.92622272886147000,-4.54861962639998000,2.19335312878658000,0.06994512650339650,0.00209864224851937,8.14276013517280000,4.98941077007855000,4.14428999239410000,0.40192231506568000,0.15647903471982300
-4,3.39824970557054000,-1.90866886095696000,0.03907021175392270,-0.01116310102107140,0.00946204465357523,4.44270178622409000,3.32451542526423000,0.18977288034821400,0.08719186146446030,0.08278090600413400
-5,1.47279248639329000,-0.40193304219938700,0.30599895698268900,0.01961442171731680,0.00097717710608820,3.74974048281819000,0.58806653613967300,0.51563961310301100,0.12137757008060300,0.06809824121603130
-6,124.46608862134300000,-220.35285707896300000,195.23535228047900000,-98.10793612697990000,0.01420230412136230,2.42120849256005000,2.30537943752425000,2.04851932106564000,1.93352552917547000,0.07689768184783390
-7,58.13271507025560000,-147.54240908781200000,130.14306564963900000,-39.61956740841540000,0.01059577633314800,1.70044856413471000,1.55903852601740000,1.41576827473146000,1.27841818205455000,0.05655877984748050
-8,29.94740452423620000,-77.61012662552780000,99.88177646231440000,-51.21270055056730000,0.00819618954446032,1.30283987880010000,1.15794105258309000,1.00988549338025000,0.94332797143326600,0.04331976113218250
-9,0.94898489450352400,-30.13339230435540000,52.79650781273380000,-22.70627037952720000,0.00656997664531441,1.45882933198645000,0.68877999318768000,0.65423986934669500,0.61483613081199400,0.03428374194950110
-10,0.58274119222090700,0.37067656184105400,-0.54674496735080900,0.41405268248020800,0.00519903080863993,1.28118573143877000,0.44452089717047700,0.19865087551048100,0.18547724665627600,0.02757383820338850
-11,23.67006039467920000,-21.85317861597420000,0.59249944810894600,-0.02446522903102440,0.00483950221706535,8.45148773514603000,8.04096600474298000,0.62499600052631500,0.13245039494729600,0.02339943620498780
-12,4.85501047687149000,-2.66220906476843000,0.47800123608510800,-0.07023070646920640,0.00398905828104019,5.94639273842456000,4.17130312520697000,0.39826980815037400,0.16188618583747400,0.01953450563631030
-13,2.83409561607507000,-4.28004133378261000,4.42191680548311000,-0.03457744718964000,0.00352385941406079,6.66235023980533000,0.55129472222402100,0.50932896344597300,0.11178483742533100,0.01676023518052570
-14,2.87189142611612000,-2.06173501195173000,2.17114024204478000,-0.06630736330588010,0.00301070709670513,5.08487103642989000,0.42917818530512600,0.36648543419216200,0.11971061129690300,0.01439945361283970
-15,2.79151840023151000,-4.36506837823822000,4.43558455516699000,-0.08096357733994730,0.00267900017966440,3.90065961865466000,0.32982596837715000,0.30608995650588800,0.10808323254597200,0.01258944953311860
-16,2.67971415610199000,-0.47425282223075500,0.51483594898968700,-0.09583600249907220,0.00248871963818935,3.06889121199971000,0.37821670218580900,0.18872181190254800,0.09233705900314940,0.01119208772411440
-17,2.56624839980020000,-0.33887635082859100,1.14584558755515000,-0.92310931654707900,0.00229168002041042,2.41594920365612000,0.42141423931021600,0.10959240497583000,0.09909554582267530,0.00999665948927521
-18,2.45981746414068000,-0.36419817707699500,0.25058447722247400,-0.05774370295443450,0.00230143866828583,1.94004631988856000,0.39924106788439800,0.11747240627441200,0.05678037260236210,0.00915579832920708
-19,5.81107878601454000,-50.25370965394220000,48.86094120598420000,0.07406285920483820,0.00072780273862622,12.66914833990360000,3.95641039698166000,3.68385059577154000,0.10745851756956200,0.00665576789391501
-20,21.17811615241590000,-339.04382431746800000,322.75695852329600000,0.06500776738969960,0.00065587436657859,6.39608619431736000,3.74024713891749000,3.64888449922605000,0.09450906345146730,0.00598520619883758
-21,12.60351865721480000,-276.87538205370200000,268.87160390734200000,0.05568241788974580,0.00057707125514540,6.15625615363852000,3.08873554266679000,3.02727663298548000,0.08188747483752150,0.00538289832050797
-22,8.57595775238129000,-210.33156346530400000,206.09717260154100000,0.04777739489772610,0.00050571648448032,6.00780668875581000,2.60285856745213000,2.55352345051105000,0.07114294840241530,0.00485628439383726
-23,6.52768433234789000,-200.43057682917200000,198.01505388999400000,0.04139115180640050,0.00044745502432986,5.83552479352448000,2.23255952381127000,2.19786018594229000,0.06239738768285470,0.00440383649079958
-24,3.02831784843691000,-95.53939330814320000,96.17615623521980000,0.03597773159579870,0.00039149289071842,8.35911504314631000,1.80263790264103000,1.77509488957047000,0.05481444121431130,0.00399828968916034
-25,4.37417550633122000,-160.92551091877900000,160.27330806032200000,0.03123038610491620,0.00034696602102094,5.51031705504928000,1.68798216402433000,1.66614047777702000,0.04833703903212770,0.00364746960053068
-26,3.79810090836859000,-91.68935493816870000,91.44542521554290000,0.02727543440276040,0.00030337985438377,5.31712645899433000,1.49713094884748000,1.46809241804410000,0.04272478501289540,0.00332791855231874
-27,3.33037874467544000,-77.00175964729670000,77.07252217905160000,0.02399046690405690,0.00026825666552394,5.18135964579543000,1.32915122265139000,1.30284928963228000,0.03806454868263710,0.00305010007991570
-28,2.96908078725286000,-75.74770691290400000,76.03982876253070000,0.02101621136929670,0.00023115175113515,5.04180949109380000,1.18275507921629000,1.16216545846629000,0.03374790878830350,0.00278680862070740
-29,1.75207145212145000,-43.04105234921240000,44.07059155435730000,0.01868761540881440,0.00020172732479162,6.18750497986187000,1.00266263628976000,0.98538431135303000,0.03029847039161170,0.00255855598748879
-30,2.46637110499459000,-61.46785413325370000,62.01769452374810000,0.01641601739314160,0.00017248711759538,4.91028078493815000,0.96789852032299200,0.95128383477535500,0.02696009676675660,0.00234109611046253
-31,2.76010203108428000,-34.44526142074670000,35.22622672440160000,0.01320671969994190,0.00012594556092825,6.10128224537662000,0.76514331355346400,0.75132862338285900,0.02248796343172510,0.00206737374278712
-32,3.18241635260000000,-52.45140378111660000,52.96908271622180000,0.01140961685918640,0.00009509543581451,5.01719040860914000,0.71239576443779800,0.70228019252819400,0.01967472956940150,0.00184146614494011
-33,3.45642969119604000,-33.31760444317210000,33.57121938553320000,0.00979002295640342,0.00006534348622652,4.01358016032945000,0.66235577805062900,0.64577194105607300,0.01709193532310110,0.00160301602839420
-34,3.64905047801926000,-43.68516622212380000,43.69202886011540000,0.00844902284199144,0.00003786114741100,3.25043267112593000,0.60966620165028900,0.59697130080212300,0.01485545127403620,0.00133625587356563
-35,3.83846312224289000,-52.27234710112330000,51.98612794956590000,0.00733955989338044,0.00001646942079513,2.61189470573232000,0.56619506287471800,0.55527932669987300,0.01297464694324400,0.00102986536855875
-36,4.02541030310827000,-46.30423320789290000,45.72136819041010000,0.00635337959625315,0.00000133477845256,2.13648381443740000,0.52659116645413100,0.51413678446457700,0.01128072422420060,0.00048808985794097
-37,3.38975351595394000,2.14348348679172000,0.35432260351097800,0.00374009340085664,0.00000030034250234,20.57448143681710000,1.91079945218516000,0.19741058939660300,0.00813459465343988,0.00029268579105695
-38,4.77092509299826000,1.47597850155283000,0.30445135554418800,0.00359474981916728,0.00000030008554923,13.36688813304120000,1.33738379577196000,0.17753236943778200,0.00779105033001826,0.00028225513964854
-39,4.60721019875234000,1.42801851039840000,0.29558104557775300,0.00338997840852895,0.00000026686297497,10.86869055571510000,1.31137455873124000,0.16802287078471100,0.00735964545350478,0.00026234328102139
-40,4.31175453406871000,1.49331578039339000,0.28123605012888400,0.00309337738455747,0.00000025802444851,9.45896580517490000,1.33063622845245000,0.15650687144445300,0.00682410523811735,0.00024981887911070
-41,3.11179039113495000,2.20259060945803000,0.27033077491002000,0.00268799194751098,0.00000023254948335,10.69031413430230000,1.65316356158933000,0.14511518571896900,0.00613956351582850,0.00023224023593767
-42,2.83105968432053000,2.34858137489674000,0.24510588842969600,0.00235282108218515,0.00000023127083834,10.43571957589500000,1.60482868674597000,0.13169693477460600,0.00554977901383345,0.00022274746376490
-43,2.57179859323352000,2.45633741957203000,0.22065844088137100,0.00205531418012438,0.00000023213294779,10.16431171313770000,1.53441919244550000,0.11913861975411000,0.00501853240882988,0.00021459037912086
-44,2.33230030353946000,2.53578025489049000,0.19820804213602600,0.00176120130460053,0.00000019812941155,9.92167460159959000,1.45585668808788000,0.10768218787334900,0.00447243545654967,0.00019657471623250
-45,2.11352534859470000,2.58636316155013000,0.17706391386368600,0.00149737051003056,0.00000020548144556,9.65913725859762000,1.37106656934329000,0.09703530275846480,0.00397128509088792,0.00019135519073780
-46,0.64215979618268700,2.97914814426328000,0.16815442600427000,0.00133744213878407,0.00000019141096825,5.97479750263406000,1.43359432541277000,0.09098684011726770,0.00362410137116162,0.00018068891441605
-47,1.55317216680389000,2.63930364699988000,0.14201548695678800,0.00100850460099760,0.00000019463842997,8.15620235758956000,1.21600887481801000,0.07900988649158730,0.00296547901363949,0.00017459309591915
-48,61.53078519928600000,-78.60167412015820000,21.55012926027700000,0.13768501566419100,0.00032464493094652,3.11468102533247000,2.76016983388574000,1.93551312324722000,0.07224683472602930,0.00117001629624684
-49,4.22232177901524000,-26.41213183532020000,27.28528527087460000,0.12161790188413800,0.00030688354637153,6.07265510403227000,1.64550178959387000,1.52257074939506000,0.06565079146952250,0.00112093851473035
-50,5.14222074642053000,-25.49454137625760000,25.74144875486010000,0.11177822759219900,0.00029364738473774,5.27272636474484000,1.53194959209148000,1.40257525040087000,0.06116853872630860,0.00107560815394522
-51,6.24164031831883000,-93.38687244195520000,92.63328758298840000,0.10341269222129800,0.00028184842689439,4.26984108082687000,1.39407746140250000,1.35566854910434000,0.05726679496521990,0.00103307954282067
-52,7.37743301813403000,-126.02510693162800000,124.12840500409500000,0.09599783718185690,0.00027107221639888,3.46917757783897000,1.29759810886736000,1.26771067646066000,0.05377717501794230,0.00099308457702918
-53,9.64400666272123000,-122.92443535011200000,118.68256481656700000,0.08950259470255390,0.00026127612149048,2.72645545366544000,1.23723425850866000,1.20062036872249000,0.05066786822851990,0.00095543788338350
-54,15.54517496748600000,-118.24102785674400000,108.00952496319700000,0.08362593419922210,0.00025199186242907,2.10637340865492000,1.20860376129512000,1.15395270567214000,0.04781893912748240,0.00091988625759261
-55,4.28708739181692000,3.23250665422965000,0.67402953356170600,0.06189080833876970,0.00023561205295219,22.65878707985410000,2.23797386470064000,0.36899556866431600,0.04022665752984840,0.00088376189087804
-56,6.24475187390461000,2.35172271416388000,0.47427937322225200,0.06381138742868490,0.00023465128056279,15.14313541909850000,1.45379000604814000,0.32083564638780100,0.04043545320946990,0.00085408113128003
-57,6.09788179599509000,2.19495164736675000,0.54817279196002200,0.06166695732226620,0.00022680735586471,12.42885443158540000,1.50535992352023000,0.33373803971712400,0.03877445534999980,0.00082404988406487
-58,5.79526879647240000,2.37022664107843000,0.47139875690111400,0.05743682605878660,0.00021897948925966,14.28010550582560000,1.35969015719134000,0.30201734966351400,0.03664367981470070,0.00079543452651837
-59,5.60406255377525000,2.35796259561812000,0.47600109857288200,0.05441233743152470,0.00021141460220515,13.95174902305740000,1.31239754917439000,0.29493370119295600,0.03486015424623240,0.00076826168266181
-60,5.42908391969770000,2.33687325360880000,0.48337355410488100,0.05146549645574790,0.00020377613286376,13.65036494276600000,1.26759841390319000,0.28861068157692900,0.03312918074466090,0.00074234848380127
-61,5.26774445089444000,2.30855813326305000,0.49326547902601200,0.04863562797416960,0.00019630884232068,13.36020968273940000,1.22585856586941000,0.28291963212786600,0.03147353971271370,0.00071765802506962
-62,5.12680428517077000,2.26925534008380000,0.50420930045330200,0.04569239924162220,0.00018867505049389,13.15815010261290000,1.18129508243337000,0.27710703821906200,0.02979576045495440,0.00069401109919910
-63,4.97962359749809000,2.24183087455669000,0.51293396140289300,0.04298018484983340,0.00018138169248579,12.83926630780330000,1.14705446420486000,0.27038716093524300,0.02824187149526020,0.00067148660317399
-64,5.07835830045611000,1.95744027181659000,0.59282598322137500,0.04195020341439250,0.00017524109152832,10.51327254690470000,1.11764941281524000,0.28438674183367500,0.02726633276413470,0.00065031086070730
-65,4.71161636657300000,2.17261950786578000,0.53971760134286500,0.03797960045478110,0.00016692376356484,12.31094159485390000,1.08743796767492000,0.25980496550927500,0.02532899238951890,0.00062927856696191
-66,4.59075504485146000,2.13572373036567000,0.55135556009415200,0.03560584067185130,0.00015982401685679,12.06567406233690000,1.05811737115864000,0.25399443891866100,0.02395087396496490,0.00060948274843329
-67,4.48400110626710000,2.08904347078539000,0.56593261831610400,0.03327035902110630,0.00015244561028289,11.87492506915700000,1.02828493708789000,0.24890780790807600,0.02258440655321470,0.00059037444515942
-68,4.37665140786963000,2.04645150383634000,0.58066286059158700,0.03123885283277660,0.00014537486966254,11.66530807171390000,1.00314769675495000,0.24415329268631200,0.02136185800007310,0.00057211033845477
-69,4.28308318247419000,1.99538001453730000,0.59705357133250400,0.02909516688695590,0.00013806476903752,11.49619059566830000,0.97703910201882000,0.23942913297582900,0.02009122333272550,0.00055437713849227
-70,4.19563840737123000,1.94333285978645000,0.61244661728546500,0.02715152076949320,0.00013059478735193,11.41077504566520000,0.94901192445487700,0.23495032653530400,0.01890515762809750,0.00053723364920971
-71,4.35692593296384000,1.69589204777315000,0.66390452006847000,0.02630200187602810,0.00012549731849982,9.29434514718568000,0.91050004595742000,0.23874659591137600,0.01820985425464620,0.00052155937196356
-72,4.33138405664923000,1.52764864728680000,0.73579592289123800,0.02495263232014020,0.00011874085258106,7.87684433810288000,0.94251564262774800,0.24169948003980600,0.01728998944485090,0.00050583463131353
-73,4.19726001319642000,1.46854806774708000,0.78393124821108800,0.02324940948643950,0.00011126135860729,6.93674024894457000,1.01725276618348000,0.23894893971507000,0.01623324330753810,0.00049023900402115
-74,3.97629715819077000,1.52292684257341000,0.79770624639056100,0.02136667415586850,0.00010307868938572,6.29685779228774000,1.11289951157691000,0.23105704067847300,0.01510135455672040,0.00047468247710503
-75,3.75144381439811000,1.62768802977632000,0.78175675545427100,0.01951708039122910,0.00009431998042934,5.79754636082953000,1.18223631077710000,0.21991358602477000,0.01398104554814560,0.00045912712582984
-76,3.48401517338711000,1.79377920416965000,0.74487835669192000,0.01754277851624340,0.00008448723515689,5.43998846080953000,1.22792134140128000,0.20620885699290900,0.01278994017211460,0.00044303222678748
-77,1.59956578198844000,2.97534452194120000,0.69509267836688200,0.01487796274586880,0.00006905495791016,5.79244447385567000,1.55300982973226000,0.18862633593664800,0.01117634706624530,0.00042277236165555
-78,2.04021563975728000,2.89922634624825000,0.63634408381579700,0.01320719195954080,0.00005673821925001,6.65819429609627000,1.41337923778932000,0.17400010450217900,0.01006878045302100,0.00040307710569222
-79,1.67593467064870000,3.00486602969729000,0.59534001316163500,0.01171631866230940,0.00004296782976398,5.52231093211402000,1.38007223007196000,0.16222923765594500,0.00901814890416575,0.00037927766747767
-80,2.23522850443105000,2.68276638651994000,0.55519492621243300,0.01072733543662580,0.00003284739920463,5.02030988960240000,1.23077590583777000,0.15224812299286300,0.00828399116906210,0.00035624193893176
-81,2.80342737412510000,2.71882787966020000,0.52247591539199900,0.00984537836971042,0.00002345245265083,6.55876872804534000,1.16972422516667000,0.14355669180017800,0.00761976526230039,0.00032962767390299
-82,3.60861020997771000,2.45056774737198000,0.47863950010725700,0.00887214235169215,0.00001040019329095,6.58162594621962000,1.02772852660588000,0.13353368063472000,0.00684861238948429,0.00027638887545667
-83,4.24209901057315000,2.09994342055827000,0.43283663137992200,0.00802021570381059,0.00000072178503085,5.75280115536080000,0.87390148919546100,0.12359995618052400,0.00617600333058570,0.00014149517761723
-84,4.63620095668962000,1.78063311426987000,0.40373044395273800,0.00768539554668674,0.00000008954159028,4.88825299780982000,0.75631052688007400,0.11730236445224900,0.00593034394242894,0.00007666686638730
-85,4.96592250595070000,1.43815561507033000,0.37129920057929800,0.00747256428450201,0.00000011411528415,4.09129378787496000,0.62922899660255100,0.11109667869553500,0.00577235010347761,0.00008085118938794
-86,5.30615614475033000,1.11733160236072000,0.31585872311085400,0.00720342242310210,0.00000010735533055,3.48800735481655000,0.48119074114977100,0.10187446794575300,0.00559245374417078,0.00007795066735407
-87,4.52053399042336000,4.10695397909124000,0.71394687850372800,0.01692940276874530,0.00008574921291917,19.44822342329480000,1.89824673155996000,0.16955356359534100,0.01148195675489340,0.00034612203825798
-88,6.52401072001873000,3.20787080745661000,0.54047877434963700,0.00878278806898853,0.00000691010602949,14.00925542989740000,1.32635035961665000,0.13140856838603600,0.00628647434520409,0.00022783998145895
-89,6.89602853559619000,2.83514154536523000,0.50350688188881500,0.00802294510966706,0.00000009204009548,11.07638256703980000,1.17132616290503000,0.12349465139179900,0.00573515595790497,0.00007197075418025
-90,7.09374900162630000,2.52912373903194000,0.48210781988888900,0.00771936674145111,0.00000007271141994,9.09473795165944000,1.06391667033161000,0.11861944662187700,0.00553945708895034,0.00006584947305285
-91,6.43401324797284000,2.97099970535788000,0.46079665178784800,0.00724033125775455,0.00000006362366643,10.25968513072970000,1.13177452306163000,0.11277593536238200,0.00527459583353132,0.00006192638240888
-92,6.21070826784019000,3.03934453825623000,0.43733998443916200,0.00680714764147316,0.00000006182293277,10.02141058591620000,1.10399880155883000,0.10721897316245300,0.00502432130850682,0.00006005069941972
-93,6.00431598308986000,3.09431654531418000,0.41280848771641700,0.00640891657880066,0.00000006730073762,9.81793046719106000,1.06978705068029000,0.10163529144864500,0.00479524846888725,0.00006028065987265
-94,5.20061716810304000,3.49849440367144000,0.40541493113132000,0.00622343700826529,0.00000006008593295,11.20383101944060000,1.12846369546928000,0.09893334726861310,0.00465917431977950,0.00005725906389623
-95,5.02533860036029000,3.51843988285154000,0.38195034944627200,0.00582110208096211,0.00000006526093388,10.97721906976280000,1.08477214832630000,0.09367468748538350,0.00442682346873485,0.00005738568370505
-96,5.34656100260619000,3.22468466560910000,0.34946175262544500,0.00529251756748815,0.00000006159176302,9.23118379752449000,0.97283622919383500,0.08705962209665620,0.00413011964465032,0.00005494638944497
-97,5.22582350334004000,3.22818873995295000,0.32709887882385100,0.00488882575592239,0.00000005212722694,9.07135706618718000,0.93112427745663400,0.08207206020598450,0.00389029655993416,0.00005103679766366
-98,4.58641247753547000,3.51869595665101000,0.31926171420120500,0.00472979647985625,0.00000005513244808,10.31861020923350000,0.95727883782923200,0.07968074314438800,0.00377193199996848,0.00005097508603760
-99,4.45799480675412000,3.50867212637662000,0.30137538052831500,0.00440763746214481,0.00000004887879032,10.08906933834010000,0.91944644736162200,0.07564191777863290,0.00357026465124809,0.00004804951743958
-100,4.33897576401170000,3.49185098896403000,0.28147109901628600,0.00400209271499046,0.00000005529298082,9.96330937223836000,0.87808395698297400,0.07116371157687770,0.00332152404215077,0.00004851031794604
-101,4.22729470403101000,3.47249227510661000,0.26482222949689800,0.00369072877833192,0.00000006258714262,9.72400602040031000,0.84287377596021000,0.06735347439748510,0.00312364606263320,0.00004912170970176
-102,4.10951702443020000,3.45799132522750000,0.24708735122238600,0.00330423920940995,0.00000005991049262,9.67735994510120000,0.80694004247081700,0.06328154369541670,0.00287544639641209,0.00004706791536976
-103,4.52147421198378000,3.20212985587804000,0.22302872695645100,0.00281716453892029,0.00000004064279540,8.28309906861142000,0.73191895812539300,0.05809427730186550,0.00256168016047444,0.00004038165155290
+From "An accurate parameterization for scattering factors, electron densities and electrostatic potentials for neutral atoms that obey all physical constraints", Lobato I. and van Dyck D., Acta Cryst. 70:636-649, 2014
+Z,a1,a2,a3,a4,a5,b1,b2,b3,b4,b5
+1,0.00647384848835291,-0.49019257678022900,0.57328416039087600,-0.37940330148399000,0.55442647477407900,2.78519885379148000,2.77620428330644000,2.77538591050625000,2.76759302867258000,2.76511897642927000
+2,3.05745116099835000,-62.00447791273250000,64.00555370846140000,-5.00132578542780000,0.15179882870052600,1.08967248726078000,0.93983879814312100,0.92528903438626500,0.82294749870865000,0.57739311067540200
+3,3.92622272886147000,-4.54861962639998000,2.19335312878658000,0.06994512650339650,0.00209864224851937,8.14276013517280000,4.98941077007855000,4.14428999239410000,0.40192231506568000,0.15647903471982300
+4,3.39824970557054000,-1.90866886095696000,0.03907021175392270,-0.01116310102107140,0.00946204465357523,4.44270178622409000,3.32451542526423000,0.18977288034821400,0.08719186146446030,0.08278090600413400
+5,1.47279248639329000,-0.40193304219938700,0.30599895698268900,0.01961442171731680,0.00097717710608820,3.74974048281819000,0.58806653613967300,0.51563961310301100,0.12137757008060300,0.06809824121603130
+6,124.46608862134300000,-220.35285707896300000,195.23535228047900000,-98.10793612697990000,0.01420230412136230,2.42120849256005000,2.30537943752425000,2.04851932106564000,1.93352552917547000,0.07689768184783390
+7,58.13271507025560000,-147.54240908781200000,130.14306564963900000,-39.61956740841540000,0.01059577633314800,1.70044856413471000,1.55903852601740000,1.41576827473146000,1.27841818205455000,0.05655877984748050
+8,29.94740452423620000,-77.61012662552780000,99.88177646231440000,-51.21270055056730000,0.00819618954446032,1.30283987880010000,1.15794105258309000,1.00988549338025000,0.94332797143326600,0.04331976113218250
+9,0.94898489450352400,-30.13339230435540000,52.79650781273380000,-22.70627037952720000,0.00656997664531441,1.45882933198645000,0.68877999318768000,0.65423986934669500,0.61483613081199400,0.03428374194950110
+10,0.58274119222090700,0.37067656184105400,-0.54674496735080900,0.41405268248020800,0.00519903080863993,1.28118573143877000,0.44452089717047700,0.19865087551048100,0.18547724665627600,0.02757383820338850
+11,23.67006039467920000,-21.85317861597420000,0.59249944810894600,-0.02446522903102440,0.00483950221706535,8.45148773514603000,8.04096600474298000,0.62499600052631500,0.13245039494729600,0.02339943620498780
+12,4.85501047687149000,-2.66220906476843000,0.47800123608510800,-0.07023070646920640,0.00398905828104019,5.94639273842456000,4.17130312520697000,0.39826980815037400,0.16188618583747400,0.01953450563631030
+13,2.83409561607507000,-4.28004133378261000,4.42191680548311000,-0.03457744718964000,0.00352385941406079,6.66235023980533000,0.55129472222402100,0.50932896344597300,0.11178483742533100,0.01676023518052570
+14,2.87189142611612000,-2.06173501195173000,2.17114024204478000,-0.06630736330588010,0.00301070709670513,5.08487103642989000,0.42917818530512600,0.36648543419216200,0.11971061129690300,0.01439945361283970
+15,2.79151840023151000,-4.36506837823822000,4.43558455516699000,-0.08096357733994730,0.00267900017966440,3.90065961865466000,0.32982596837715000,0.30608995650588800,0.10808323254597200,0.01258944953311860
+16,2.67971415610199000,-0.47425282223075500,0.51483594898968700,-0.09583600249907220,0.00248871963818935,3.06889121199971000,0.37821670218580900,0.18872181190254800,0.09233705900314940,0.01119208772411440
+17,2.56624839980020000,-0.33887635082859100,1.14584558755515000,-0.92310931654707900,0.00229168002041042,2.41594920365612000,0.42141423931021600,0.10959240497583000,0.09909554582267530,0.00999665948927521
+18,2.45981746414068000,-0.36419817707699500,0.25058447722247400,-0.05774370295443450,0.00230143866828583,1.94004631988856000,0.39924106788439800,0.11747240627441200,0.05678037260236210,0.00915579832920708
+19,5.81107878601454000,-50.25370965394220000,48.86094120598420000,0.07406285920483820,0.00072780273862622,12.66914833990360000,3.95641039698166000,3.68385059577154000,0.10745851756956200,0.00665576789391501
+20,21.17811615241590000,-339.04382431746800000,322.75695852329600000,0.06500776738969960,0.00065587436657859,6.39608619431736000,3.74024713891749000,3.64888449922605000,0.09450906345146730,0.00598520619883758
+21,12.60351865721480000,-276.87538205370200000,268.87160390734200000,0.05568241788974580,0.00057707125514540,6.15625615363852000,3.08873554266679000,3.02727663298548000,0.08188747483752150,0.00538289832050797
+22,8.57595775238129000,-210.33156346530400000,206.09717260154100000,0.04777739489772610,0.00050571648448032,6.00780668875581000,2.60285856745213000,2.55352345051105000,0.07114294840241530,0.00485628439383726
+23,6.52768433234789000,-200.43057682917200000,198.01505388999400000,0.04139115180640050,0.00044745502432986,5.83552479352448000,2.23255952381127000,2.19786018594229000,0.06239738768285470,0.00440383649079958
+24,3.02831784843691000,-95.53939330814320000,96.17615623521980000,0.03597773159579870,0.00039149289071842,8.35911504314631000,1.80263790264103000,1.77509488957047000,0.05481444121431130,0.00399828968916034
+25,4.37417550633122000,-160.92551091877900000,160.27330806032200000,0.03123038610491620,0.00034696602102094,5.51031705504928000,1.68798216402433000,1.66614047777702000,0.04833703903212770,0.00364746960053068
+26,3.79810090836859000,-91.68935493816870000,91.44542521554290000,0.02727543440276040,0.00030337985438377,5.31712645899433000,1.49713094884748000,1.46809241804410000,0.04272478501289540,0.00332791855231874
+27,3.33037874467544000,-77.00175964729670000,77.07252217905160000,0.02399046690405690,0.00026825666552394,5.18135964579543000,1.32915122265139000,1.30284928963228000,0.03806454868263710,0.00305010007991570
+28,2.96908078725286000,-75.74770691290400000,76.03982876253070000,0.02101621136929670,0.00023115175113515,5.04180949109380000,1.18275507921629000,1.16216545846629000,0.03374790878830350,0.00278680862070740
+29,1.75207145212145000,-43.04105234921240000,44.07059155435730000,0.01868761540881440,0.00020172732479162,6.18750497986187000,1.00266263628976000,0.98538431135303000,0.03029847039161170,0.00255855598748879
+30,2.46637110499459000,-61.46785413325370000,62.01769452374810000,0.01641601739314160,0.00017248711759538,4.91028078493815000,0.96789852032299200,0.95128383477535500,0.02696009676675660,0.00234109611046253
+31,2.76010203108428000,-34.44526142074670000,35.22622672440160000,0.01320671969994190,0.00012594556092825,6.10128224537662000,0.76514331355346400,0.75132862338285900,0.02248796343172510,0.00206737374278712
+32,3.18241635260000000,-52.45140378111660000,52.96908271622180000,0.01140961685918640,0.00009509543581451,5.01719040860914000,0.71239576443779800,0.70228019252819400,0.01967472956940150,0.00184146614494011
+33,3.45642969119604000,-33.31760444317210000,33.57121938553320000,0.00979002295640342,0.00006534348622652,4.01358016032945000,0.66235577805062900,0.64577194105607300,0.01709193532310110,0.00160301602839420
+34,3.64905047801926000,-43.68516622212380000,43.69202886011540000,0.00844902284199144,0.00003786114741100,3.25043267112593000,0.60966620165028900,0.59697130080212300,0.01485545127403620,0.00133625587356563
+35,3.83846312224289000,-52.27234710112330000,51.98612794956590000,0.00733955989338044,0.00001646942079513,2.61189470573232000,0.56619506287471800,0.55527932669987300,0.01297464694324400,0.00102986536855875
+36,4.02541030310827000,-46.30423320789290000,45.72136819041010000,0.00635337959625315,0.00000133477845256,2.13648381443740000,0.52659116645413100,0.51413678446457700,0.01128072422420060,0.00048808985794097
+37,3.38975351595394000,2.14348348679172000,0.35432260351097800,0.00374009340085664,0.00000030034250234,20.57448143681710000,1.91079945218516000,0.19741058939660300,0.00813459465343988,0.00029268579105695
+38,4.77092509299826000,1.47597850155283000,0.30445135554418800,0.00359474981916728,0.00000030008554923,13.36688813304120000,1.33738379577196000,0.17753236943778200,0.00779105033001826,0.00028225513964854
+39,4.60721019875234000,1.42801851039840000,0.29558104557775300,0.00338997840852895,0.00000026686297497,10.86869055571510000,1.31137455873124000,0.16802287078471100,0.00735964545350478,0.00026234328102139
+40,4.31175453406871000,1.49331578039339000,0.28123605012888400,0.00309337738455747,0.00000025802444851,9.45896580517490000,1.33063622845245000,0.15650687144445300,0.00682410523811735,0.00024981887911070
+41,3.11179039113495000,2.20259060945803000,0.27033077491002000,0.00268799194751098,0.00000023254948335,10.69031413430230000,1.65316356158933000,0.14511518571896900,0.00613956351582850,0.00023224023593767
+42,2.83105968432053000,2.34858137489674000,0.24510588842969600,0.00235282108218515,0.00000023127083834,10.43571957589500000,1.60482868674597000,0.13169693477460600,0.00554977901383345,0.00022274746376490
+43,2.57179859323352000,2.45633741957203000,0.22065844088137100,0.00205531418012438,0.00000023213294779,10.16431171313770000,1.53441919244550000,0.11913861975411000,0.00501853240882988,0.00021459037912086
+44,2.33230030353946000,2.53578025489049000,0.19820804213602600,0.00176120130460053,0.00000019812941155,9.92167460159959000,1.45585668808788000,0.10768218787334900,0.00447243545654967,0.00019657471623250
+45,2.11352534859470000,2.58636316155013000,0.17706391386368600,0.00149737051003056,0.00000020548144556,9.65913725859762000,1.37106656934329000,0.09703530275846480,0.00397128509088792,0.00019135519073780
+46,0.64215979618268700,2.97914814426328000,0.16815442600427000,0.00133744213878407,0.00000019141096825,5.97479750263406000,1.43359432541277000,0.09098684011726770,0.00362410137116162,0.00018068891441605
+47,1.55317216680389000,2.63930364699988000,0.14201548695678800,0.00100850460099760,0.00000019463842997,8.15620235758956000,1.21600887481801000,0.07900988649158730,0.00296547901363949,0.00017459309591915
+48,61.53078519928600000,-78.60167412015820000,21.55012926027700000,0.13768501566419100,0.00032464493094652,3.11468102533247000,2.76016983388574000,1.93551312324722000,0.07224683472602930,0.00117001629624684
+49,4.22232177901524000,-26.41213183532020000,27.28528527087460000,0.12161790188413800,0.00030688354637153,6.07265510403227000,1.64550178959387000,1.52257074939506000,0.06565079146952250,0.00112093851473035
+50,5.14222074642053000,-25.49454137625760000,25.74144875486010000,0.11177822759219900,0.00029364738473774,5.27272636474484000,1.53194959209148000,1.40257525040087000,0.06116853872630860,0.00107560815394522
+51,6.24164031831883000,-93.38687244195520000,92.63328758298840000,0.10341269222129800,0.00028184842689439,4.26984108082687000,1.39407746140250000,1.35566854910434000,0.05726679496521990,0.00103307954282067
+52,7.37743301813403000,-126.02510693162800000,124.12840500409500000,0.09599783718185690,0.00027107221639888,3.46917757783897000,1.29759810886736000,1.26771067646066000,0.05377717501794230,0.00099308457702918
+53,9.64400666272123000,-122.92443535011200000,118.68256481656700000,0.08950259470255390,0.00026127612149048,2.72645545366544000,1.23723425850866000,1.20062036872249000,0.05066786822851990,0.00095543788338350
+54,15.54517496748600000,-118.24102785674400000,108.00952496319700000,0.08362593419922210,0.00025199186242907,2.10637340865492000,1.20860376129512000,1.15395270567214000,0.04781893912748240,0.00091988625759261
+55,4.28708739181692000,3.23250665422965000,0.67402953356170600,0.06189080833876970,0.00023561205295219,22.65878707985410000,2.23797386470064000,0.36899556866431600,0.04022665752984840,0.00088376189087804
+56,6.24475187390461000,2.35172271416388000,0.47427937322225200,0.06381138742868490,0.00023465128056279,15.14313541909850000,1.45379000604814000,0.32083564638780100,0.04043545320946990,0.00085408113128003
+57,6.09788179599509000,2.19495164736675000,0.54817279196002200,0.06166695732226620,0.00022680735586471,12.42885443158540000,1.50535992352023000,0.33373803971712400,0.03877445534999980,0.00082404988406487
+58,5.79526879647240000,2.37022664107843000,0.47139875690111400,0.05743682605878660,0.00021897948925966,14.28010550582560000,1.35969015719134000,0.30201734966351400,0.03664367981470070,0.00079543452651837
+59,5.60406255377525000,2.35796259561812000,0.47600109857288200,0.05441233743152470,0.00021141460220515,13.95174902305740000,1.31239754917439000,0.29493370119295600,0.03486015424623240,0.00076826168266181
+60,5.42908391969770000,2.33687325360880000,0.48337355410488100,0.05146549645574790,0.00020377613286376,13.65036494276600000,1.26759841390319000,0.28861068157692900,0.03312918074466090,0.00074234848380127
+61,5.26774445089444000,2.30855813326305000,0.49326547902601200,0.04863562797416960,0.00019630884232068,13.36020968273940000,1.22585856586941000,0.28291963212786600,0.03147353971271370,0.00071765802506962
+62,5.12680428517077000,2.26925534008380000,0.50420930045330200,0.04569239924162220,0.00018867505049389,13.15815010261290000,1.18129508243337000,0.27710703821906200,0.02979576045495440,0.00069401109919910
+63,4.97962359749809000,2.24183087455669000,0.51293396140289300,0.04298018484983340,0.00018138169248579,12.83926630780330000,1.14705446420486000,0.27038716093524300,0.02824187149526020,0.00067148660317399
+64,5.07835830045611000,1.95744027181659000,0.59282598322137500,0.04195020341439250,0.00017524109152832,10.51327254690470000,1.11764941281524000,0.28438674183367500,0.02726633276413470,0.00065031086070730
+65,4.71161636657300000,2.17261950786578000,0.53971760134286500,0.03797960045478110,0.00016692376356484,12.31094159485390000,1.08743796767492000,0.25980496550927500,0.02532899238951890,0.00062927856696191
+66,4.59075504485146000,2.13572373036567000,0.55135556009415200,0.03560584067185130,0.00015982401685679,12.06567406233690000,1.05811737115864000,0.25399443891866100,0.02395087396496490,0.00060948274843329
+67,4.48400110626710000,2.08904347078539000,0.56593261831610400,0.03327035902110630,0.00015244561028289,11.87492506915700000,1.02828493708789000,0.24890780790807600,0.02258440655321470,0.00059037444515942
+68,4.37665140786963000,2.04645150383634000,0.58066286059158700,0.03123885283277660,0.00014537486966254,11.66530807171390000,1.00314769675495000,0.24415329268631200,0.02136185800007310,0.00057211033845477
+69,4.28308318247419000,1.99538001453730000,0.59705357133250400,0.02909516688695590,0.00013806476903752,11.49619059566830000,0.97703910201882000,0.23942913297582900,0.02009122333272550,0.00055437713849227
+70,4.19563840737123000,1.94333285978645000,0.61244661728546500,0.02715152076949320,0.00013059478735193,11.41077504566520000,0.94901192445487700,0.23495032653530400,0.01890515762809750,0.00053723364920971
+71,4.35692593296384000,1.69589204777315000,0.66390452006847000,0.02630200187602810,0.00012549731849982,9.29434514718568000,0.91050004595742000,0.23874659591137600,0.01820985425464620,0.00052155937196356
+72,4.33138405664923000,1.52764864728680000,0.73579592289123800,0.02495263232014020,0.00011874085258106,7.87684433810288000,0.94251564262774800,0.24169948003980600,0.01728998944485090,0.00050583463131353
+73,4.19726001319642000,1.46854806774708000,0.78393124821108800,0.02324940948643950,0.00011126135860729,6.93674024894457000,1.01725276618348000,0.23894893971507000,0.01623324330753810,0.00049023900402115
+74,3.97629715819077000,1.52292684257341000,0.79770624639056100,0.02136667415586850,0.00010307868938572,6.29685779228774000,1.11289951157691000,0.23105704067847300,0.01510135455672040,0.00047468247710503
+75,3.75144381439811000,1.62768802977632000,0.78175675545427100,0.01951708039122910,0.00009431998042934,5.79754636082953000,1.18223631077710000,0.21991358602477000,0.01398104554814560,0.00045912712582984
+76,3.48401517338711000,1.79377920416965000,0.74487835669192000,0.01754277851624340,0.00008448723515689,5.43998846080953000,1.22792134140128000,0.20620885699290900,0.01278994017211460,0.00044303222678748
+77,1.59956578198844000,2.97534452194120000,0.69509267836688200,0.01487796274586880,0.00006905495791016,5.79244447385567000,1.55300982973226000,0.18862633593664800,0.01117634706624530,0.00042277236165555
+78,2.04021563975728000,2.89922634624825000,0.63634408381579700,0.01320719195954080,0.00005673821925001,6.65819429609627000,1.41337923778932000,0.17400010450217900,0.01006878045302100,0.00040307710569222
+79,1.67593467064870000,3.00486602969729000,0.59534001316163500,0.01171631866230940,0.00004296782976398,5.52231093211402000,1.38007223007196000,0.16222923765594500,0.00901814890416575,0.00037927766747767
+80,2.23522850443105000,2.68276638651994000,0.55519492621243300,0.01072733543662580,0.00003284739920463,5.02030988960240000,1.23077590583777000,0.15224812299286300,0.00828399116906210,0.00035624193893176
+81,2.80342737412510000,2.71882787966020000,0.52247591539199900,0.00984537836971042,0.00002345245265083,6.55876872804534000,1.16972422516667000,0.14355669180017800,0.00761976526230039,0.00032962767390299
+82,3.60861020997771000,2.45056774737198000,0.47863950010725700,0.00887214235169215,0.00001040019329095,6.58162594621962000,1.02772852660588000,0.13353368063472000,0.00684861238948429,0.00027638887545667
+83,4.24209901057315000,2.09994342055827000,0.43283663137992200,0.00802021570381059,0.00000072178503085,5.75280115536080000,0.87390148919546100,0.12359995618052400,0.00617600333058570,0.00014149517761723
+84,4.63620095668962000,1.78063311426987000,0.40373044395273800,0.00768539554668674,0.00000008954159028,4.88825299780982000,0.75631052688007400,0.11730236445224900,0.00593034394242894,0.00007666686638730
+85,4.96592250595070000,1.43815561507033000,0.37129920057929800,0.00747256428450201,0.00000011411528415,4.09129378787496000,0.62922899660255100,0.11109667869553500,0.00577235010347761,0.00008085118938794
+86,5.30615614475033000,1.11733160236072000,0.31585872311085400,0.00720342242310210,0.00000010735533055,3.48800735481655000,0.48119074114977100,0.10187446794575300,0.00559245374417078,0.00007795066735407
+87,4.52053399042336000,4.10695397909124000,0.71394687850372800,0.01692940276874530,0.00008574921291917,19.44822342329480000,1.89824673155996000,0.16955356359534100,0.01148195675489340,0.00034612203825798
+88,6.52401072001873000,3.20787080745661000,0.54047877434963700,0.00878278806898853,0.00000691010602949,14.00925542989740000,1.32635035961665000,0.13140856838603600,0.00628647434520409,0.00022783998145895
+89,6.89602853559619000,2.83514154536523000,0.50350688188881500,0.00802294510966706,0.00000009204009548,11.07638256703980000,1.17132616290503000,0.12349465139179900,0.00573515595790497,0.00007197075418025
+90,7.09374900162630000,2.52912373903194000,0.48210781988888900,0.00771936674145111,0.00000007271141994,9.09473795165944000,1.06391667033161000,0.11861944662187700,0.00553945708895034,0.00006584947305285
+91,6.43401324797284000,2.97099970535788000,0.46079665178784800,0.00724033125775455,0.00000006362366643,10.25968513072970000,1.13177452306163000,0.11277593536238200,0.00527459583353132,0.00006192638240888
+92,6.21070826784019000,3.03934453825623000,0.43733998443916200,0.00680714764147316,0.00000006182293277,10.02141058591620000,1.10399880155883000,0.10721897316245300,0.00502432130850682,0.00006005069941972
+93,6.00431598308986000,3.09431654531418000,0.41280848771641700,0.00640891657880066,0.00000006730073762,9.81793046719106000,1.06978705068029000,0.10163529144864500,0.00479524846888725,0.00006028065987265
+94,5.20061716810304000,3.49849440367144000,0.40541493113132000,0.00622343700826529,0.00000006008593295,11.20383101944060000,1.12846369546928000,0.09893334726861310,0.00465917431977950,0.00005725906389623
+95,5.02533860036029000,3.51843988285154000,0.38195034944627200,0.00582110208096211,0.00000006526093388,10.97721906976280000,1.08477214832630000,0.09367468748538350,0.00442682346873485,0.00005738568370505
+96,5.34656100260619000,3.22468466560910000,0.34946175262544500,0.00529251756748815,0.00000006159176302,9.23118379752449000,0.97283622919383500,0.08705962209665620,0.00413011964465032,0.00005494638944497
+97,5.22582350334004000,3.22818873995295000,0.32709887882385100,0.00488882575592239,0.00000005212722694,9.07135706618718000,0.93112427745663400,0.08207206020598450,0.00389029655993416,0.00005103679766366
+98,4.58641247753547000,3.51869595665101000,0.31926171420120500,0.00472979647985625,0.00000005513244808,10.31861020923350000,0.95727883782923200,0.07968074314438800,0.00377193199996848,0.00005097508603760
+99,4.45799480675412000,3.50867212637662000,0.30137538052831500,0.00440763746214481,0.00000004887879032,10.08906933834010000,0.91944644736162200,0.07564191777863290,0.00357026465124809,0.00004804951743958
+100,4.33897576401170000,3.49185098896403000,0.28147109901628600,0.00400209271499046,0.00000005529298082,9.96330937223836000,0.87808395698297400,0.07116371157687770,0.00332152404215077,0.00004851031794604
+101,4.22729470403101000,3.47249227510661000,0.26482222949689800,0.00369072877833192,0.00000006258714262,9.72400602040031000,0.84287377596021000,0.06735347439748510,0.00312364606263320,0.00004912170970176
+102,4.10951702443020000,3.45799132522750000,0.24708735122238600,0.00330423920940995,0.00000005991049262,9.67735994510120000,0.80694004247081700,0.06328154369541670,0.00287544639641209,0.00004706791536976
+103,4.52147421198378000,3.20212985587804000,0.22302872695645100,0.00281716453892029,0.00000004064279540,8.28309906861142000,0.73191895812539300,0.05809427730186550,0.00256168016047444,0.00004038165155290
```

### Comparing `abtem-1.0.0b8/abtem/device.py` & `abtem-1.0.0b9/abtem/device.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,231 +1,228 @@
-from typing import Union, Callable
-import numpy as np
-import psutil
-import pyfftw
-
-from abtem.cpu_kernels import abs2, complex_exponential, interpolate_radial_functions, scale_reduce, \
-    windowed_scale_reduce, sum_run_length_encoded
-
-FFTW_EFFORT = 'FFTW_MEASURE'
-FFTW_THREADS = 12
-FFTW_TIMELIMIT = 600
-
-try:  # This should be the only place import cupy, to make it a non-essential dependency
-    import cupy as cp
-    import cupyx.scipy.fft
-    import cupyx.scipy.ndimage as ndimage
-    from abtem.cuda_kernels import launch_interpolate_radial_functions, launch_scale_reduce, \
-        launch_windowed_scale_reduce, launch_superpose_deltas, launch_sum_run_length_encoded
-
-    get_array_module = cp.get_array_module
-
-
-    def fft2_convolve(array: cp.array, kernel: cp.array, overwrite_x: bool = True):
-        """
-        2d FFT convolution using GPU.
-        """
-        array = cupyx.scipy.fftpack.fft2(array, overwrite_x=overwrite_x)
-        array *= kernel
-        array = cupyx.scipy.fftpack.ifft2(array, overwrite_x=overwrite_x)
-        return array
-
-
-    def fft2(array, overwrite_x=True):
-        return cupyx.scipy.fft.fft2(array, overwrite_x=overwrite_x)
-
-
-    def ifft2(array, overwrite_x=True):
-        return cupyx.scipy.fft.ifft2(array, overwrite_x=overwrite_x)
-
-
-    def pin_array(array):
-        print(array.dtype, array.shape)
-        mem = cp.cuda.alloc_pinned_memory(array.nbytes)
-
-        src = np.frombuffer(mem, array.dtype, array.size).reshape(array.shape)
-        src[...] = array
-        return src
-
-
-    gpu_functions = {'fft2': fft2,
-                     'ifft2': ifft2,
-                     'fft2_convolve': fft2_convolve,
-                     'pin_array': pin_array,
-                     'complex_exponential': lambda x: cp.exp(1.j * x),
-                     'abs2': lambda x: cp.abs(x) ** 2,
-                     'interpolate_radial_functions': launch_interpolate_radial_functions,
-                     'scale_reduce': launch_scale_reduce,
-                     'sum_run_length_encoded': launch_sum_run_length_encoded,
-                     'windowed_scale_reduce': launch_windowed_scale_reduce,
-                     'superpose_deltas': launch_superpose_deltas}
-
-    asnumpy = cp.asnumpy
-
-except ImportError:  # cupy is not available
-    cp = None
-    get_array_module = lambda *args, **kwargs: np
-    gpu_functions = None
-    asnumpy = np.asarray
-    import scipy.ndimage as ndimage
-
-
-def create_fftw_objects(array, allow_new_plan=True):
-    """
-    Creates FFTW object for forward and backward Fourier transforms. The input array will be
-    transformed in place. The function tries to retrieve FFTW plans from wisdom only.
-    If no plan exists for the input array, a new plan is cached and then retrieved.
-
-    :param array: Numpy array to be transformed. 2 dimensions or more.
-    :param allow_new_plan: If false raise an exception instead of caching a new plan.
-    :return:
-    """
-
-    try:
-        # try using cached FFTW plan
-        fftw_forward = pyfftw.FFTW(array, array, axes=(-1, -2),
-                                   threads=FFTW_THREADS,
-                                   flags=(FFTW_EFFORT, 'FFTW_WISDOM_ONLY', 'FFTW_DESTROY_INPUT'))
-        fftw_backward = pyfftw.FFTW(array, array, axes=(-1, -2),
-                                    direction='FFTW_BACKWARD', threads=FFTW_THREADS,
-                                    flags=(FFTW_EFFORT, 'FFTW_WISDOM_ONLY', 'FFTW_DESTROY_INPUT'))
-        return fftw_forward, fftw_backward
-
-    except RuntimeError as e:
-        if (not allow_new_plan):
-            fftw_forward = pyfftw.builders.fft2(array)
-            fftw_backward = pyfftw.builders.ifft2(array)
-            return fftw_forward, fftw_backward
-        # if ('No FFTW wisdom is known for this plan.' != str(e)) or (not allow_new_plan):
-        #    raise
-
-        # create new FFTW object, not to be used, but the plan will remain in the cache
-        dummy = pyfftw.byte_align(np.zeros_like(array))
-        # this is necessary because FFTW overwrites the array during planning
-
-        pyfftw.FFTW(dummy, dummy,
-                    axes=(-1, -2),
-                    threads=FFTW_THREADS,
-                    flags=(FFTW_EFFORT, 'FFTW_DESTROY_INPUT'),
-                    planning_timelimit=FFTW_TIMELIMIT)
-
-        pyfftw.FFTW(dummy, dummy, axes=(-1, -2),
-                    direction='FFTW_BACKWARD',
-                    threads=FFTW_THREADS,
-                    flags=(FFTW_EFFORT, 'FFTW_DESTROY_INPUT'),
-                    planning_timelimit=FFTW_TIMELIMIT)
-
-        return create_fftw_objects(array, False)
-
-
-def fft2_convolve(array, kernel, overwrite_x=True):
-    def _fft_convolve(array, kernel):
-        fftw_forward, fftw_backward = create_fftw_objects(array)
-        fftw_forward()
-        array *= kernel
-        fftw_backward()
-        return array
-
-    if not overwrite_x:
-        array = array.copy()
-
-    return _fft_convolve(array, kernel)
-
-
-def fft2(array, overwrite_x=True):
-    if not overwrite_x:
-        array = array.copy()
-
-    fftw_forward, fftw_backward = create_fftw_objects(array)
-    return fftw_forward()
-
-
-def ifft2(array, overwrite_x=True):
-    if not overwrite_x:
-        array = array.copy()
-
-    fftw_forward, fftw_backward = create_fftw_objects(array)
-    return fftw_backward()
-
-
-cpu_functions = {'fft2': fft2,
-                 'ifft2': ifft2,
-                 'fft2_convolve': fft2_convolve,
-                 'abs2': abs2,
-                 'pin_array': lambda x: x,
-                 'complex_exponential': complex_exponential,
-                 'interpolate_radial_functions': interpolate_radial_functions,
-                 'sum_run_length_encoded': sum_run_length_encoded,
-                 'scale_reduce': scale_reduce,
-                 'windowed_scale_reduce': windowed_scale_reduce}
-
-
-def get_device_function(xp, name: str) -> Callable:
-    """
-    Return the function appropriate to the given array library.
-
-    :param xp: The array library. Must numpy or cupy.
-    :param name: Name of function.
-    """
-    if (xp is cp):
-        return gpu_functions[name]
-    elif xp is np:
-        return cpu_functions[name]
-    else:
-        raise RuntimeError('The array library ')
-
-
-def get_array_module_from_device(device):
-    if device == 'cpu':
-        return np
-
-    if device == 'gpu':
-        if cp is None:
-            raise RuntimeError('CuPy is not installed, only CPU calculations available')
-        return cp
-
-    return get_array_module(device)
-
-
-def copy_to_device(array, device):
-    """
-    Copy array to a device.
-
-    :param array: Array to be copied.
-    :param device:
-    :return:
-    """
-    if (device == 'cpu') or (device is None) or (device is np):
-        return asnumpy(array)
-
-    elif (device == 'gpu') or (device is cp):
-        if cp is None:
-            raise RuntimeError('CuPy is not installed, only CPU calculations available')
-        return cp.asarray(array)
-
-    else:
-        raise RuntimeError()
-
-
-def get_available_memory(device: str) -> float:
-    if device == 'cpu':
-        return psutil.virtual_memory().available
-
-    else:
-        mempool = cp.get_default_memory_pool()
-        mempool.free_all_blocks()
-
-        if device == 'gpu':
-            device = cp.cuda.Device(0)
-        return device.mem_info[0]
-
-
-class HasDeviceMixin:
-    _device: str
-
-    @property
-    def device(self):
-        return self._device
-
-    @property
-    def calculation_device(self):
-        return self._device
+from typing import Union, Callable
+import numpy as np
+import psutil
+import pyfftw
+
+from abtem.cpu_kernels import abs2, complex_exponential, interpolate_radial_functions, sum_run_length_encoded
+from abtem.interpolate import interpolate_bilinear_cpu
+
+FFTW_EFFORT = 'FFTW_MEASURE'
+FFTW_THREADS = 12
+FFTW_TIMELIMIT = 600
+
+try:  # This should be the only place import cupy, to make it a non-essential dependency
+    import cupy as cp
+    import cupyx.scipy.fft
+    import cupyx.scipy.ndimage as ndimage
+    from abtem.cuda_kernels import launch_interpolate_radial_functions, launch_sum_run_length_encoded, \
+        interpolate_bilinear_gpu
+
+    get_array_module = cp.get_array_module
+
+
+    def fft2_convolve(array: cp.array, kernel: cp.array, overwrite_x: bool = True):
+        """
+        2d FFT convolution using GPU.
+        """
+        array = cupyx.scipy.fftpack.fft2(array, overwrite_x=overwrite_x)
+        array *= kernel
+        array = cupyx.scipy.fftpack.ifft2(array, overwrite_x=overwrite_x)
+        return array
+
+
+    def fft2(array, overwrite_x=True):
+        return cupyx.scipy.fft.fft2(array, overwrite_x=overwrite_x)
+
+
+    def ifft2(array, overwrite_x=True):
+        return cupyx.scipy.fft.ifft2(array, overwrite_x=overwrite_x)
+
+
+    def pin_array(array):
+        print(array.dtype, array.shape)
+        mem = cp.cuda.alloc_pinned_memory(array.nbytes)
+
+        src = np.frombuffer(mem, array.dtype, array.size).reshape(array.shape)
+        src[...] = array
+        return src
+
+
+    gpu_functions = {'fft2': fft2,
+                     'ifft2': ifft2,
+                     'fft2_convolve': fft2_convolve,
+                     'pin_array': pin_array,
+                     'complex_exponential': lambda x: cp.exp(1.j * x),
+                     'abs2': lambda x: cp.abs(x) ** 2,
+                     'interpolate_radial_functions': launch_interpolate_radial_functions,
+                     'interpolate_bilinear': interpolate_bilinear_gpu,
+                     'sum_run_length_encoded': launch_sum_run_length_encoded}
+
+    asnumpy = cp.asnumpy
+
+except ImportError:  # cupy is not available
+    cp = None
+    get_array_module = lambda *args, **kwargs: np
+    gpu_functions = None
+    asnumpy = np.asarray
+    import scipy.ndimage as ndimage
+
+
+def create_fftw_objects(array, allow_new_plan=True):
+    """
+    Creates FFTW object for forward and backward Fourier transforms. The input array will be
+    transformed in place. The function tries to retrieve FFTW plans from wisdom only.
+    If no plan exists for the input array, a new plan is cached and then retrieved.
+
+    :param array: Numpy array to be transformed. 2 dimensions or more.
+    :param allow_new_plan: If false raise an exception instead of caching a new plan.
+    :return:
+    """
+
+    try:
+        # try using cached FFTW plan
+        fftw_forward = pyfftw.FFTW(array, array, axes=(-1, -2),
+                                   threads=FFTW_THREADS,
+                                   flags=(FFTW_EFFORT, 'FFTW_WISDOM_ONLY', 'FFTW_DESTROY_INPUT'))
+        fftw_backward = pyfftw.FFTW(array, array, axes=(-1, -2),
+                                    direction='FFTW_BACKWARD', threads=FFTW_THREADS,
+                                    flags=(FFTW_EFFORT, 'FFTW_WISDOM_ONLY', 'FFTW_DESTROY_INPUT'))
+        return fftw_forward, fftw_backward
+
+    except RuntimeError as e:
+        if (not allow_new_plan):
+            fftw_forward = pyfftw.builders.fft2(array)
+            fftw_backward = pyfftw.builders.ifft2(array)
+            return fftw_forward, fftw_backward
+        # if ('No FFTW wisdom is known for this plan.' != str(e)) or (not allow_new_plan):
+        #    raise
+
+        # create new FFTW object, not to be used, but the plan will remain in the cache
+        dummy = pyfftw.byte_align(np.zeros_like(array))
+        # this is necessary because FFTW overwrites the array during planning
+
+        pyfftw.FFTW(dummy, dummy,
+                    axes=(-1, -2),
+                    threads=FFTW_THREADS,
+                    flags=(FFTW_EFFORT, 'FFTW_DESTROY_INPUT'),
+                    planning_timelimit=FFTW_TIMELIMIT)
+
+        pyfftw.FFTW(dummy, dummy, axes=(-1, -2),
+                    direction='FFTW_BACKWARD',
+                    threads=FFTW_THREADS,
+                    flags=(FFTW_EFFORT, 'FFTW_DESTROY_INPUT'),
+                    planning_timelimit=FFTW_TIMELIMIT)
+
+        return create_fftw_objects(array, False)
+
+
+def fft2_convolve(array, kernel, overwrite_x=True):
+    def _fft_convolve(array, kernel):
+        fftw_forward, fftw_backward = create_fftw_objects(array)
+        fftw_forward()
+        array *= kernel
+        fftw_backward()
+        return array
+
+    if not overwrite_x:
+        array = array.copy()
+
+    return _fft_convolve(array, kernel)
+
+
+def fft2(array, overwrite_x=True):
+    if not overwrite_x:
+        array = array.copy()
+
+    fftw_forward, fftw_backward = create_fftw_objects(array)
+    return fftw_forward()
+
+
+def ifft2(array, overwrite_x=True):
+    if not overwrite_x:
+        array = array.copy()
+
+    fftw_forward, fftw_backward = create_fftw_objects(array)
+    return fftw_backward()
+
+
+cpu_functions = {'fft2': fft2,
+                 'ifft2': ifft2,
+                 'fft2_convolve': fft2_convolve,
+                 'abs2': abs2,
+                 'pin_array': lambda x: x,
+                 'complex_exponential': complex_exponential,
+                 'interpolate_radial_functions': interpolate_radial_functions,
+                 'interpolate_bilinear': interpolate_bilinear_cpu,
+                 'sum_run_length_encoded': sum_run_length_encoded}
+
+
+def get_device_function(xp, name: str) -> Callable:
+    """
+    Return the function appropriate to the given array library.
+
+    :param xp: The array library. Must numpy or cupy.
+    :param name: Name of function.
+    """
+    if (xp is cp):
+        return gpu_functions[name]
+    elif xp is np:
+        return cpu_functions[name]
+    else:
+        raise RuntimeError('The array library ')
+
+
+def get_array_module_from_device(device):
+    if device == 'cpu':
+        return np
+
+    if device == 'gpu':
+        if cp is None:
+            raise RuntimeError('CuPy is not installed, only CPU calculations available')
+        return cp
+
+    return get_array_module(device)
+
+
+def copy_to_device(array, device):
+    """
+    Copy array to a device.
+
+    :param array: Array to be copied.
+    :param device:
+    :return:
+    """
+    if (device == 'cpu') or (device is None) or (device is np):
+        return asnumpy(array)
+
+    elif (device == 'gpu') or (device is cp):
+        if cp is None:
+            raise RuntimeError('CuPy is not installed, only CPU calculations available')
+        return cp.asarray(array)
+
+    else:
+        raise RuntimeError()
+
+
+def get_available_memory(device: str) -> float:
+    if device == 'cpu':
+        return psutil.virtual_memory().available
+
+    else:
+        mempool = cp.get_default_memory_pool()
+        mempool.free_all_blocks()
+
+        if device == 'gpu':
+            device = cp.cuda.Device(0)
+        return device.mem_info[0]
+
+
+class HasDeviceMixin:
+    _device: str
+
+    @property
+    def device(self):
+        return self._device
+
+    @property
+    def calculation_device(self):
+        return self._device
```

### Comparing `abtem-1.0.0b8/abtem/dft.py` & `abtem-1.0.0b9/abtem/dft.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,275 +1,275 @@
-"""Module to handle ab initio electrostatic potentials from the DFT code GPAW."""
-from typing import Sequence, Tuple, Union
-
-import numpy as np
-from ase import units
-from scipy.interpolate import interp1d, interpn
-
-from abtem.base_classes import Grid
-from abtem.device import get_device_function
-from abtem.potentials import AbstractPotentialBuilder, PotentialArray, _disc_meshgrid, pad_atoms, \
-    PotentialIntegrator
-from abtem.structures import orthogonalize_cell
-from abtem.utils import subdivide_into_batches
-
-import warnings
-
-try:
-    from gpaw.atom.shapefunc import shape_functions
-    from gpaw import GPAW
-except ImportError:
-    warnings.warn('This functionality of abTEM requires GPAW, see https://wiki.fysik.dtu.dk/gpaw/.')
-
-
-def interpolate_rectangle(array: np.ndarray,
-                          cell: np.ndarray,
-                          extent: Sequence[float],
-                          gpts: Sequence[int],
-                          origin: Sequence[float] = None):
-    """
-    Interpolation to rectangle function
-
-    A function to interpolate an array to a given rectangle, here used to convert electrostatic potentials
-    from non-orthogonal cells to rectangular ones for use in abTEM multislice simulations.
-
-    :param array: Electrostatic potential array to be interpolated.
-    :param cell: ASE atoms simulation cell.
-    :param extent: Extent of the rectangle [Å].
-    :param gpts: Number of interpolation grid points.
-    :param origin: Origin of the rectangle. Default is (0,0).
-    """
-
-    if origin is None:
-        origin = (0., 0.)
-
-    origin = np.array(origin)
-    extent = np.array(extent)
-
-    P = np.array(cell)
-    P_inv = np.linalg.inv(P)
-    origin_t = np.dot(origin, P_inv)
-    origin_t = origin_t % 1.0
-
-    lower = np.dot(origin_t, P)
-    upper = lower + extent
-
-    padded_array = np.zeros((array.shape[0] + 1, array.shape[1] + 1))
-    padded_array[:-1, :-1] = array
-    padded_array[-1, :] = padded_array[0, :]
-    padded_array[:, -1] = padded_array[:, 0]
-
-    x = np.linspace(0, 1, padded_array.shape[0], endpoint=True)
-    y = np.linspace(0, 1, padded_array.shape[1], endpoint=True)
-
-    x_ = np.linspace(lower[0], upper[0], gpts[0], endpoint=False)
-    y_ = np.linspace(lower[1], upper[1], gpts[1], endpoint=False)
-    x_, y_ = np.meshgrid(x_, y_, indexing='ij')
-
-    p = np.array([x_.ravel(), y_.ravel()]).T
-    p = np.dot(p, P_inv) % 1.0
-
-    interpolated = interpn((x, y), padded_array, p, method='splinef2d')
-    return interpolated.reshape((gpts[0], gpts[1]))
-
-
-def get_paw_corrections(atom_index: int, calculator, rcgauss: float = 0.005) -> Tuple[np.ndarray, np.ndarray]:
-    """
-    PAW corrections function
-
-    Function to calculate the projector-augmented wave corrections to the electrostatic potential, needed to
-    calculate the all-electron potential from a converged calculation. This is implemented independently in
-    abTEM to enable dealing with non-orthogonal cells, and to allow working with slices of large potentials.
-
-    Parameters
-    ----------
-    atom_index: int
-        Index of the atom for which the corrections are calculated.
-    calculator: GPAW object
-        Converged GPAW calculation.
-    rcgauss: float
-        Radius of the Gaussian smearing of the nuclear potentials [Å]. Default value is 0.005 Å.
-
-    Returns
-    -------
-    two 1d arrays
-        The evaluation points and values of the core contribution to the electronstatic potential.
-    """
-
-    dens = calculator.density
-    dens.D_asp.redistribute(dens.atom_partition.as_serial())
-    dens.Q_aL.redistribute(dens.atom_partition.as_serial())
-
-    D_sp = dens.D_asp[atom_index]
-
-    setup = dens.setups[atom_index]
-    c = setup.xc_correction
-    rgd = c.rgd
-    ghat_g = shape_functions(rgd, **setup.data.shape_function, lmax=0)[0]
-    Z_g = shape_functions(rgd, 'gauss', rcgauss, lmax=0)[0] * setup.Z
-    D_q = np.dot(D_sp.sum(0), c.B_pqL[:, :, 0])
-    dn_g = np.dot(D_q, (c.n_qg - c.nt_qg)) * np.sqrt(4 * np.pi)
-    dn_g += 4 * np.pi * (c.nc_g - c.nct_g)
-    dn_g -= Z_g
-    dn_g -= dens.Q_aL[atom_index][0] * ghat_g * np.sqrt(4 * np.pi)
-    dv_g = rgd.poisson(dn_g) / np.sqrt(4 * np.pi)
-    dv_g[1:] /= rgd.r_g[1:]
-    dv_g[0] = dv_g[1]
-    dv_g[-1] = 0.0
-
-    return rgd.r_g, dv_g
-
-
-class GPAWPotential(AbstractPotentialBuilder):
-    """
-    GPAW DFT potential object
-
-    The GPAW potential object is used to calculate electrostatic potential of a converged GPAW calculator object.
-
-    Parameters
-    ----------
-    calculator: GPAW object
-        A converged GPAW calculator.
-    origin: two float, optional
-        xy-origin of the electrostatic potential relative to the xy-origin of the Atoms object [Å].
-    gpts: one or two int
-        Number of grid points describing each slice of the potential.
-    sampling: one or two float
-        Lateral sampling of the potential [1 / Å].
-    slice_thickness: float
-        Thickness of the potential slices in Å for calculating the number of slices used by the multislice algorithm.
-        Default is 0.5 Å.
-    core_size: float
-        The standard deviation of the Gaussian function representing the atomic core.
-    """
-
-    def __init__(self,
-                 calculator,
-                 gpts: Union[int, Sequence[int]] = None,
-                 sampling: Union[float, Sequence[float]] = None,
-                 # origin: Union[float, Sequence[float]] = None,
-                 slice_thickness=.5,
-                 core_size=.005,
-                 storage='cpu'):
-
-        self._calculator = calculator
-        self._core_size = core_size
-
-        thickness = calculator.atoms.cell[2, 2]
-        nz = calculator.hamiltonian.finegd.N_c[2]
-        num_slices = int(np.ceil(nz / np.floor(slice_thickness / (thickness / nz))))
-
-        self._voxel_height = thickness / nz
-        self._slice_vertical_voxels = subdivide_into_batches(nz, num_slices)
-
-        # TODO: implement support for non-periodic extent
-
-        self._origin = (0., 0.)
-        extent = np.diag(orthogonalize_cell(calculator.atoms.copy()).cell)[:2]
-
-        self._grid = Grid(extent=extent, gpts=gpts, sampling=sampling, lock_extent=True)
-
-        super().__init__(storage=storage)
-
-    @property
-    def calculator(self):
-        return self._calculator
-
-    @property
-    def core_size(self):
-        return self._core_size
-
-    @property
-    def origin(self):
-        return self._origin
-
-    @property
-    def num_slices(self):
-        return len(self._slice_vertical_voxels)
-
-    def get_slice_thickness(self, i):
-        return self._slice_vertical_voxels[i] * self._voxel_height
-
-    def generate_slices(self, first_slice=0, last_slice=None, max_batch=1):
-
-        interpolate_radial_functions = get_device_function(np, 'interpolate_radial_functions')
-
-        if last_slice is None:
-            last_slice = len(self)
-
-        valence = self._calculator.get_electrostatic_potential()
-        cell = self._calculator.atoms.cell[:2, :2]
-
-        atoms = self._calculator.atoms.copy()
-        atoms.set_tags(range(len(atoms)))
-        atoms = orthogonalize_cell(atoms)
-
-        indices_by_number = {number: np.where(atoms.numbers == number)[0] for number in np.unique(atoms.numbers)}
-
-        na = sum(self._slice_vertical_voxels[:first_slice])
-        a = na * self._voxel_height
-        for i in range(first_slice, last_slice):
-            nb = na + self._slice_vertical_voxels[i]
-            b = a + self._slice_vertical_voxels[i] * self._voxel_height
-
-            projected_valence = valence[..., na:nb].sum(axis=-1) * self._voxel_height
-            projected_valence = interpolate_rectangle(projected_valence, cell, self.extent, self.gpts, self._origin)
-
-            array = np.zeros(self.gpts, dtype=np.float32)
-            for number, indices in indices_by_number.items():
-                slice_atoms = atoms[indices]
-
-                if len(slice_atoms) == 0:
-                    continue
-
-                r = self._calculator.density.setups[indices[0]].xc_correction.rgd.r_g[1:] * units.Bohr
-                cutoff = r[-1]
-
-                margin = np.int(np.ceil(cutoff / np.min(self.sampling)))
-                rows, cols = _disc_meshgrid(margin)
-                disc_indices = np.hstack((rows[:, None], cols[:, None]))
-
-                slice_atoms = slice_atoms[(slice_atoms.positions[:, 2] > a - cutoff) *
-                                          (slice_atoms.positions[:, 2] < b + cutoff)]
-
-                slice_atoms = pad_atoms(slice_atoms, cutoff)
-
-                R = np.geomspace(1e-8, cutoff, int(np.ceil(cutoff / np.min(self.sampling))) * 10)
-
-                vr = np.zeros((len(slice_atoms), len(R)), np.float32)
-                dvdr = np.zeros((len(slice_atoms), len(R)), np.float32)
-                for j, atom in enumerate(slice_atoms):
-                    r, v = get_paw_corrections(atom.tag, self._calculator, self._core_size)
-
-                    f = interp1d(r * units.Bohr, v, fill_value=(v[0], 0), bounds_error=False, kind='linear')
-
-                    integrator = PotentialIntegrator(f, R)
-                    am, bm = a - atom.z, b - atom.z
-
-                    vr[j], dvdr[j, :-1] = integrator.integrate(am, bm)
-
-                sampling = np.asarray(self.sampling, dtype=np.float32)
-
-                interpolate_radial_functions(array,
-                                             disc_indices,
-                                             slice_atoms.positions,
-                                             vr,
-                                             R,
-                                             dvdr,
-                                             sampling)
-
-            array = -(projected_valence + array / np.sqrt(4 * np.pi) * units.Ha)
-
-            yield i, i + 1, PotentialArray(array, np.array([self.get_slice_thickness(i)]), extent=self.extent)
-
-            a = b
-            na = nb
-
-    def __copy__(self):
-        slice_thickness = self.calculator.atoms.cell[2, 2] / self.num_slices
-        return self.__class__(self.calculator,
-                              gpts=self.gpts,
-                              sampling=self.sampling,
-                              # origin=self.origin,
-                              slice_thickness=slice_thickness,
-                              core_size=self.core_size,
-                              storage=self._storage)
+"""Module to handle ab initio electrostatic potentials from the DFT code GPAW."""
+from typing import Sequence, Tuple, Union
+
+import numpy as np
+from ase import units
+from scipy.interpolate import interp1d, interpn
+
+from abtem.base_classes import Grid
+from abtem.device import get_device_function
+from abtem.potentials import AbstractPotentialBuilder, PotentialArray, _disc_meshgrid, pad_atoms, \
+    PotentialIntegrator
+from abtem.structures import orthogonalize_cell
+from abtem.utils import subdivide_into_batches
+
+import warnings
+
+try:
+    from gpaw.atom.shapefunc import shape_functions
+    from gpaw import GPAW
+except ImportError:
+    warnings.warn('This functionality of abTEM requires GPAW, see https://wiki.fysik.dtu.dk/gpaw/.')
+
+
+def interpolate_rectangle(array: np.ndarray,
+                          cell: np.ndarray,
+                          extent: Sequence[float],
+                          gpts: Sequence[int],
+                          origin: Sequence[float] = None):
+    """
+    Interpolation to rectangle function
+
+    A function to interpolate an array to a given rectangle, here used to convert electrostatic potentials
+    from non-orthogonal cells to rectangular ones for use in abTEM multislice simulations.
+
+    :param array: Electrostatic potential array to be interpolated.
+    :param cell: ASE atoms simulation cell.
+    :param extent: Extent of the rectangle [Å].
+    :param gpts: Number of interpolation grid points.
+    :param origin: Origin of the rectangle. Default is (0,0).
+    """
+
+    if origin is None:
+        origin = (0., 0.)
+
+    origin = np.array(origin)
+    extent = np.array(extent)
+
+    P = np.array(cell)
+    P_inv = np.linalg.inv(P)
+    origin_t = np.dot(origin, P_inv)
+    origin_t = origin_t % 1.0
+
+    lower = np.dot(origin_t, P)
+    upper = lower + extent
+
+    padded_array = np.zeros((array.shape[0] + 1, array.shape[1] + 1))
+    padded_array[:-1, :-1] = array
+    padded_array[-1, :] = padded_array[0, :]
+    padded_array[:, -1] = padded_array[:, 0]
+
+    x = np.linspace(0, 1, padded_array.shape[0], endpoint=True)
+    y = np.linspace(0, 1, padded_array.shape[1], endpoint=True)
+
+    x_ = np.linspace(lower[0], upper[0], gpts[0], endpoint=False)
+    y_ = np.linspace(lower[1], upper[1], gpts[1], endpoint=False)
+    x_, y_ = np.meshgrid(x_, y_, indexing='ij')
+
+    p = np.array([x_.ravel(), y_.ravel()]).T
+    p = np.dot(p, P_inv) % 1.0
+
+    interpolated = interpn((x, y), padded_array, p, method='splinef2d')
+    return interpolated.reshape((gpts[0], gpts[1]))
+
+
+def get_paw_corrections(atom_index: int, calculator, rcgauss: float = 0.005) -> Tuple[np.ndarray, np.ndarray]:
+    """
+    PAW corrections function
+
+    Function to calculate the projector-augmented wave corrections to the electrostatic potential, needed to
+    calculate the all-electron potential from a converged calculation. This is implemented independently in
+    abTEM to enable dealing with non-orthogonal cells, and to allow working with slices of large potentials.
+
+    Parameters
+    ----------
+    atom_index: int
+        Index of the atom for which the corrections are calculated.
+    calculator: GPAW object
+        Converged GPAW calculation.
+    rcgauss: float
+        Radius of the Gaussian smearing of the nuclear potentials [Å]. Default value is 0.005 Å.
+
+    Returns
+    -------
+    two 1d arrays
+        The evaluation points and values of the core contribution to the electronstatic potential.
+    """
+
+    dens = calculator.density
+    dens.D_asp.redistribute(dens.atom_partition.as_serial())
+    dens.Q_aL.redistribute(dens.atom_partition.as_serial())
+
+    D_sp = dens.D_asp[atom_index]
+
+    setup = dens.setups[atom_index]
+    c = setup.xc_correction
+    rgd = c.rgd
+    ghat_g = shape_functions(rgd, **setup.data.shape_function, lmax=0)[0]
+    Z_g = shape_functions(rgd, 'gauss', rcgauss, lmax=0)[0] * setup.Z
+    D_q = np.dot(D_sp.sum(0), c.B_pqL[:, :, 0])
+    dn_g = np.dot(D_q, (c.n_qg - c.nt_qg)) * np.sqrt(4 * np.pi)
+    dn_g += 4 * np.pi * (c.nc_g - c.nct_g)
+    dn_g -= Z_g
+    dn_g -= dens.Q_aL[atom_index][0] * ghat_g * np.sqrt(4 * np.pi)
+    dv_g = rgd.poisson(dn_g) / np.sqrt(4 * np.pi)
+    dv_g[1:] /= rgd.r_g[1:]
+    dv_g[0] = dv_g[1]
+    dv_g[-1] = 0.0
+
+    return rgd.r_g, dv_g
+
+
+class GPAWPotential(AbstractPotentialBuilder):
+    """
+    GPAW DFT potential object
+
+    The GPAW potential object is used to calculate electrostatic potential of a converged GPAW calculator object.
+
+    Parameters
+    ----------
+    calculator: GPAW object
+        A converged GPAW calculator.
+    origin: two float, optional
+        xy-origin of the electrostatic potential relative to the xy-origin of the Atoms object [Å].
+    gpts: one or two int
+        Number of grid points describing each slice of the potential.
+    sampling: one or two float
+        Lateral sampling of the potential [1 / Å].
+    slice_thickness: float
+        Thickness of the potential slices in Å for calculating the number of slices used by the multislice algorithm.
+        Default is 0.5 Å.
+    core_size: float
+        The standard deviation of the Gaussian function representing the atomic core.
+    """
+
+    def __init__(self,
+                 calculator,
+                 gpts: Union[int, Sequence[int]] = None,
+                 sampling: Union[float, Sequence[float]] = None,
+                 # origin: Union[float, Sequence[float]] = None,
+                 slice_thickness=.5,
+                 core_size=.005,
+                 storage='cpu'):
+
+        self._calculator = calculator
+        self._core_size = core_size
+
+        thickness = calculator.atoms.cell[2, 2]
+        nz = calculator.hamiltonian.finegd.N_c[2]
+        num_slices = int(np.ceil(nz / np.floor(slice_thickness / (thickness / nz))))
+
+        self._voxel_height = thickness / nz
+        self._slice_vertical_voxels = subdivide_into_batches(nz, num_slices)
+
+        # TODO: implement support for non-periodic extent
+
+        self._origin = (0., 0.)
+        extent = np.diag(orthogonalize_cell(calculator.atoms.copy()).cell)[:2]
+
+        self._grid = Grid(extent=extent, gpts=gpts, sampling=sampling, lock_extent=True)
+
+        super().__init__(storage=storage)
+
+    @property
+    def calculator(self):
+        return self._calculator
+
+    @property
+    def core_size(self):
+        return self._core_size
+
+    @property
+    def origin(self):
+        return self._origin
+
+    @property
+    def num_slices(self):
+        return len(self._slice_vertical_voxels)
+
+    def get_slice_thickness(self, i):
+        return self._slice_vertical_voxels[i] * self._voxel_height
+
+    def generate_slices(self, first_slice=0, last_slice=None, max_batch=1):
+
+        interpolate_radial_functions = get_device_function(np, 'interpolate_radial_functions')
+
+        if last_slice is None:
+            last_slice = len(self)
+
+        valence = self._calculator.get_electrostatic_potential()
+        cell = self._calculator.atoms.cell[:2, :2]
+
+        atoms = self._calculator.atoms.copy()
+        atoms.set_tags(range(len(atoms)))
+        atoms = orthogonalize_cell(atoms)
+
+        indices_by_number = {number: np.where(atoms.numbers == number)[0] for number in np.unique(atoms.numbers)}
+
+        na = sum(self._slice_vertical_voxels[:first_slice])
+        a = na * self._voxel_height
+        for i in range(first_slice, last_slice):
+            nb = na + self._slice_vertical_voxels[i]
+            b = a + self._slice_vertical_voxels[i] * self._voxel_height
+
+            projected_valence = valence[..., na:nb].sum(axis=-1) * self._voxel_height
+            projected_valence = interpolate_rectangle(projected_valence, cell, self.extent, self.gpts, self._origin)
+
+            array = np.zeros(self.gpts, dtype=np.float32)
+            for number, indices in indices_by_number.items():
+                slice_atoms = atoms[indices]
+
+                if len(slice_atoms) == 0:
+                    continue
+
+                r = self._calculator.density.setups[indices[0]].xc_correction.rgd.r_g[1:] * units.Bohr
+                cutoff = r[-1]
+
+                margin = np.int(np.ceil(cutoff / np.min(self.sampling)))
+                rows, cols = _disc_meshgrid(margin)
+                disc_indices = np.hstack((rows[:, None], cols[:, None]))
+
+                slice_atoms = slice_atoms[(slice_atoms.positions[:, 2] > a - cutoff) *
+                                          (slice_atoms.positions[:, 2] < b + cutoff)]
+
+                slice_atoms = pad_atoms(slice_atoms, cutoff)
+
+                R = np.geomspace(1e-8, cutoff, int(np.ceil(cutoff / np.min(self.sampling))) * 10)
+
+                vr = np.zeros((len(slice_atoms), len(R)), np.float32)
+                dvdr = np.zeros((len(slice_atoms), len(R)), np.float32)
+                for j, atom in enumerate(slice_atoms):
+                    r, v = get_paw_corrections(atom.tag, self._calculator, self._core_size)
+
+                    f = interp1d(r * units.Bohr, v, fill_value=(v[0], 0), bounds_error=False, kind='linear')
+
+                    integrator = PotentialIntegrator(f, R)
+                    am, bm = a - atom.z, b - atom.z
+
+                    vr[j], dvdr[j, :-1] = integrator.integrate(am, bm)
+
+                sampling = np.asarray(self.sampling, dtype=np.float32)
+
+                interpolate_radial_functions(array,
+                                             disc_indices,
+                                             slice_atoms.positions,
+                                             vr,
+                                             R,
+                                             dvdr,
+                                             sampling)
+
+            array = -(projected_valence + array / np.sqrt(4 * np.pi) * units.Ha)
+
+            yield i, i + 1, PotentialArray(array, np.array([self.get_slice_thickness(i)]), extent=self.extent)
+
+            a = b
+            na = nb
+
+    def __copy__(self):
+        slice_thickness = self.calculator.atoms.cell[2, 2] / self.num_slices
+        return self.__class__(self.calculator,
+                              gpts=self.gpts,
+                              sampling=self.sampling,
+                              # origin=self.origin,
+                              slice_thickness=slice_thickness,
+                              core_size=self.core_size,
+                              storage=self._storage)
```

### Comparing `abtem-1.0.0b8/abtem/measure.py` & `abtem-1.0.0b9/abtem/measure.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,658 +1,669 @@
-"""Module to describe the detection of scattered electron waves."""
-from collections.abc import Iterable
-from abc import ABCMeta
-from copy import copy
-from typing import Sequence, Tuple
-
-import h5py
-import imageio
-import numpy as np
-import scipy.misc
-import scipy.ndimage
-from scipy.interpolate import interpn
-from scipy.ndimage import zoom
-
-from abtem.device import asnumpy
-from abtem.visualize.mpl import show_measurement_2d, show_measurement_1d
-
-
-class Calibration:
-    """
-    Calibration object
-
-    The calibration object represents the sampling of a uniformly sampled Measurement.
-
-    Parameters
-    ----------
-    offset: float
-        The lower bound of the sampling points.
-    sampling: float
-        The distance between sampling points.
-    units: str
-        The units of the calibration shown in plots.
-    name: str
-        The name of this calibration to be shown in plots.
-    """
-
-    def __init__(self, offset: float, sampling: float, units: str, name: str = ''):
-        self.offset = offset
-        self.sampling = sampling
-        self.units = units
-        self.name = name
-
-    def __eq__(self, other):
-        return ((self.offset == other.offset) &
-                (self.sampling == other.sampling) &
-                (self.units == other.units) &
-                (self.name == other.name))
-
-    def __copy__(self):
-        return self.__class__(self.offset, self.sampling, self.units, self.name)
-
-    def copy(self):
-        """
-        Make a copy.
-        """
-        return copy(self)
-
-
-def _fourier_space_offset(n: int, d: float):
-    """
-    Calculate the Fourier space offset.
-
-    Parameters
-    ----------
-    n : int
-        Number of sampling points.
-    d : float
-        Real space sampling density.
-    """
-
-    if n % 2 == 0:
-        return -1 / (2 * d)
-    else:
-        return -1 / (2 * d) + 1 / (2 * d * n)
-
-
-def calibrations_from_grid(gpts: Sequence[int],
-                           sampling: Sequence[float],
-                           names: Sequence[str] = None,
-                           units: str = None,
-                           fourier_space: bool = False,
-                           scale_factor: float = 1.0) -> Tuple[Calibration]:
-    """
-    Returns the spatial calibrations for a given computational grid and sampling.
-
-    Parameters
-    ----------
-    gpts: list of int
-        Number of grid points in the x and y directions.
-    sampling: list of float
-        Sampling of the potential in Å.
-    names: list of str, optional
-        The name of this calibration.
-    units: str, optional
-        Units for the calibration.
-    fourier_space: bool, optional
-        Setting for calibrating either in the reciprocal or real space. Default is False.
-    scale_factor: float, optional
-        Scaling factor for the calibration. Default is 1.0.
-
-    Returns
-    -------
-    calibrations: Tuple of Calibrations
-    """
-
-    if names is None:
-        names = ('',) * len(gpts)
-    elif len(names) != len(gpts):
-        raise RuntimeError()
-
-    if units is None:
-        if fourier_space:
-            units = '1 / Å'
-        else:
-            units = 'Å'
-
-    calibrations = ()
-    if fourier_space:
-        for name, n, d in zip(names, gpts, sampling):
-            r = n * d
-            offset = _fourier_space_offset(n, d)
-            calibrations += (Calibration(offset * scale_factor, 1 / r * scale_factor, units, name),)
-    else:
-        for name, d in zip(names, sampling):
-            calibrations += (Calibration(0., d * scale_factor, units, name),)
-
-    return calibrations
-
-
-class Measurement:  # (metaclass=ABCMeta):
-    """
-    Measurement object.
-
-    Parameters
-    ----------
-    array: ndarray
-        The array representing the measurements. The array can be any dimension.
-    calibrations: list of Calibration objects
-        The calibration for each dimension of the measurement array.
-    units: str
-        The units of the array values to be displayed in plots.
-    name: str
-        The name of the array values to be displayed in plots.
-    """
-
-    def __init__(self, array, calibrations=None, units='', name=''):
-
-        if issubclass(array.__class__, self.__class__):
-            measurement = array
-
-            array = measurement.array
-            calibrations = measurement.calibrations
-            units = measurement.array
-            name = measurement.name
-
-        if not isinstance(calibrations, Iterable):
-            calibrations = [calibrations] * len(array.shape)
-
-        if len(calibrations) != len(array.shape):
-            raise RuntimeError(
-                'The number of calibrations must equal the number of array dimensions. For undefined use None.')
-
-        self._array = asnumpy(array)
-        self._calibrations = calibrations
-        self._units = units
-        self._name = name
-
-    def __getitem__(self, args):
-        if isinstance(args, Iterable):
-            args += (slice(None),) * (len(self.array.shape) - len(args))
-        else:
-            args = (args,) + (slice(None),) * (len(self.array.shape) - 1)
-
-        new_array = self.array[args]
-        new_calibrations = []
-        for i, (arg, calibration) in enumerate(zip(args, self.calibrations)):
-            if isinstance(arg, slice):
-                if arg.start is None:
-                    offset = calibration.offset
-                else:
-                    offset = arg.start * calibration.sampling + calibration.offset
-
-                new_calibrations.append(Calibration(offset=offset,
-                                                    sampling=calibration.sampling,
-                                                    units=calibration.units, name=calibration.name))
-            elif isinstance(arg, Iterable):
-                new_calibrations.append(None)
-
-            elif not isinstance(arg, int):
-                raise TypeError('Indices must be integers or slices, not float')
-
-        return self.__class__(new_array, new_calibrations)
-
-    @property
-    def extent(self):
-        extent = ()
-        for i, calibration in enumerate(self.calibrations):
-            if calibration is None:
-                extent += (None, None)
-            else:
-                extent += (calibration.offset, calibration.offset + self.array.shape[i] * calibration.sampling)
-        return extent
-
-    def __len__(self):
-        return self.shape[0]
-
-    @property
-    def array(self):
-        """
-        Array of measurements.
-        """
-        return self._array
-
-    # @array.setter
-    # def array(self, array):
-    #     """
-    #     Array of measurements.
-    #     """
-    #     self._array[:] = array
-
-    @property
-    def shape(self):
-        """
-        The shape of the measurement array.
-        """
-        return self._array.shape
-
-    @property
-    def units(self):
-        """
-        The units of the array values to be displayed in plots.
-        """
-        return self._units
-
-    @property
-    def name(self):
-        """
-        The name of the array values to be displayed in plots.
-        """
-        return self._name
-
-    @property
-    def dimensions(self):
-        """
-        The measurement dimensions.
-        """
-        return len(self.array.shape)
-
-    @property
-    def calibrations(self):
-        """
-        The measurement calibrations.
-        """
-        return self._calibrations
-
-    def check_match_calibrations(self, other):
-        for calibration, other_calibration in zip(self.calibrations, other.calibrations):
-            if not calibration == other_calibration:
-                raise ValueError('Calibration mismatch, operation not possible.')
-
-    def __isub__(self, other):
-        if isinstance(other, self.__class__):
-            self.check_match_calibrations(other)
-            self._array -= other.array
-        else:
-            self._array -= asnumpy(other)
-
-    def __sub__(self, other):
-        if isinstance(other, self.__class__):
-            self.check_match_calibrations(other)
-            new_array = self.array - other.array
-        else:
-            new_array = self._array - asnumpy(other)
-        return self.__class__(new_array, calibrations=self.calibrations, units=self.units, name=self.name)
-
-    def __iadd__(self, other):
-        if isinstance(other, self.__class__):
-            self.check_match_calibrations(other)
-            self._array += other.array
-        else:
-            self._array += asnumpy(other)
-
-    def __add__(self, other):
-        if isinstance(other, self.__class__):
-            self.check_match_calibrations(other)
-            new_array = self.array + other.array
-        else:
-            new_array = self._array + asnumpy(other)
-        return self.__class__(new_array, calibrations=self.calibrations, units=self.units, name=self.name)
-
-    def _reduction(self, reduction_function, axis):
-        if not isinstance(axis, Iterable):
-            axis = (axis,)
-
-        array = reduction_function(self.array, axis=axis)
-
-        axis = [d % len(self.calibrations) for d in axis]
-        calibrations = [self.calibrations[i] for i in range(len(self.calibrations)) if i not in axis]
-
-        return self.__class__(array, calibrations)
-
-    # def integrate(self, axes, start=0, end=None, use_units=True):
-    #
-    #     if end is None:
-    #         end = ()
-    #         for axis in axes:
-    #             end += (self.array.shape[axis],)
-    #
-    #     else:
-    #         end = list(end)
-    #         for axis in axes:
-    #             end[axis]
-    #
-    #     if not isinstance(axes, Iterable):
-    #         axes = (axes,)
-    #
-    #     if not isinstance(start, Iterable):
-    #         start = (start,) * len(axes)
-    #
-    #     if not isinstance(end, Iterable):
-    #         end = (end,) * len(axes)
-
-    def sum(self, axis):
-        """
-        Sum of measurment elements over a given axis.
-
-        Parameters
-        ----------
-        axis: int or tuple of ints
-            Axis or axes along which a sum is performed. If axis is negative it counts from the last to the first axis.
-
-        Returns
-        -------
-        Measurement
-            A measurement with the same shape, but with the specified axis removed.
-        """
-        return self._reduction(np.mean, axis)
-
-    def mean(self, axis):
-        """
-        Mean of measurment elements over a given axis.
-
-        Parameters
-        ----------
-        axis: int or tuple of ints
-            Axis or axes along which a sum is performed. If axis is negative it counts from the last to the first axis.
-
-        Returns
-        -------
-        Measurement object
-            A measurement with the same shape, but with the specified axis removed.
-        """
-        return self._reduction(np.mean, axis)
-
-    def interpolate(self, new_sampling):
-        import warnings
-        warnings.filterwarnings('ignore', '.*output shape of zoom.*')
-
-        scale_factors = [calibration.sampling / new_sampling for calibration in self.calibrations]
-        new_array = zoom(self.array, scale_factors, mode='wrap')
-
-        calibrations = []
-        for calibration in self.calibrations:
-            calibrations.append(copy(calibration))
-            calibrations[-1].sampling = new_sampling
-
-        return self.__class__(new_array, calibrations, name=self.name, units=self.units)
-
-    def tile(self, multiples):
-        """
-        Tile the measurement.
-
-        Parameters
-        ----------
-        multiples: two int
-            The number of repetitions of the measurement along each axis.
-
-        Returns
-        -------
-        Measurement object
-            The tiled potential.
-        """
-        new_array = np.tile(self._array, multiples)
-        return self.__class__(new_array, self.calibrations, name=self.name, units=self.units)
-
-    @classmethod
-    def read(cls, path):
-        """
-        Read measurement from a hdf5 file.
-
-        path: str
-            The path to read the file.
-        """
-
-        with h5py.File(path, 'r') as f:
-            datasets = {}
-            for key in f.keys():
-                datasets[key] = f.get(key)[()]
-
-        calibrations = []
-        for i in range(len(datasets['offset'])):
-            calibrations.append(Calibration(offset=datasets['offset'][i],
-                                            sampling=datasets['sampling'][i],
-                                            units=datasets['units'][i].decode('utf-8'),
-                                            name=datasets['name'][i].decode('utf-8')))
-
-        # print(datasets['array'].shape)
-        # import matplotlib.pyplot as plt
-        # plt.imshow(datasets['array'])
-        # plt.show()
-
-        return cls(datasets['array'], calibrations)
-
-    def write(self, path, mode='w'):
-        """
-        Write measurement to a hdf5 file.
-
-        path: str
-            The path to write the file.
-        """
-
-        with h5py.File(path, mode) as f:
-            f.create_dataset('array', data=self.array)
-            f.create_dataset('offset', data=[calibration.offset for calibration in self.calibrations])
-            f.create_dataset('sampling', data=[calibration.sampling for calibration in self.calibrations])
-            units = [calibration.units.encode('utf-8') for calibration in self.calibrations]
-            f.create_dataset('units', (len(units),), 'S10', units)
-            names = [calibration.name.encode('utf-8') for calibration in self.calibrations]
-            f.create_dataset('name', (len(names),), 'S10', names)
-
-        return path
-
-    def save_as_image(self, path):
-        """
-        Write the measurement array to an image file. The array will be normalized and converted to 16-bit integers.
-
-        path: str
-            The path to write the file.
-        """
-
-        if self.dimensions != 2:
-            raise RuntimeError('Only 2d measurements can be saved as an image.')
-
-        array = (self.array - self.array.min()) / self.array.ptp() * np.iinfo(np.uint16).max
-        array = array.astype(np.uint16)
-        imageio.imwrite(path, array.T)
-
-    def __copy__(self):
-        calibrations = []
-        for calibration in self.calibrations:
-            calibrations.append(copy(calibration))
-        return self.__class__(self._array.copy(), calibrations=calibrations)
-
-    def copy(self):
-        """
-        Make a copy.
-        """
-        return copy(self)
-
-    def squeeze(self):
-        new_meaurement = self.copy()
-        calibrations = [calib for calib, num_elem in zip(self.calibrations, self.array.shape) if num_elem > 1]
-        new_meaurement._calibrations = calibrations
-        new_meaurement._array = np.squeeze(asnumpy(new_meaurement.array))
-        return new_meaurement
-
-    def interpolate_line(self, start, end, gpts=None, sampling=None):
-        from abtem.scan import LineScan
-
-        if not (self.dimensions == 2):
-            raise RuntimeError()
-
-        if (self.calibrations[0] is None) or (self.calibrations[1] is None):
-            raise RuntimeError()
-
-        if self.calibrations[0].units != self.calibrations[1].units:
-            raise RuntimeError()
-
-        if (gpts is None) & (sampling is None):
-            sampling = (self.calibrations[0].sampling + self.calibrations[1].sampling) / 2.
-
-        x = np.linspace(self.calibrations[0].offset, self.shape[0] * self.calibrations[0].sampling, self.shape[0])
-        y = np.linspace(self.calibrations[1].offset, self.shape[1] * self.calibrations[1].sampling, self.shape[1])
-
-        scan = LineScan(start=start, end=end, gpts=gpts, sampling=sampling)
-
-        interpolated_array = interpn((x, y), self.array, scan.get_positions())
-
-        calibration = Calibration(offset=0, sampling=scan.sampling[0],
-                                  units=self.calibrations[0].units,
-                                  name=self.calibrations[0].name)
-        return Measurement(interpolated_array, calibration)
-
-    def show(self, ax=None, **kwargs):
-        """
-        Show the measurement.
-
-        Parameters
-        ----------
-        kwargs:
-            Additional keyword arguments for the abtem.plot.show_image function.
-        """
-        if self.dimensions == 1:
-            return show_measurement_1d(self, ax=ax, **kwargs)
-        else:
-            return show_measurement_2d(self, ax=ax, **kwargs)
-
-
-class FlexibleAnnularMeasurement(Measurement):
-
-    def __init__(self, array, spatial_sampling, angular_sampling, angular_offset=0.):
-        if not isinstance(spatial_sampling, Iterable):
-            spatial_sampling = (spatial_sampling,) * (len(array.shape) - 1)
-
-        calibrations = [Calibration(0., d, 'Å', name) for d, name in zip(spatial_sampling, ('x', 'y'))]
-        calibrations += [Calibration(angular_offset, angular_sampling, 'mrad', 'alpha')]
-
-        super().__init__(array, calibrations)
-
-    def integrate(self, start, end):
-        offset = self.calibrations[-1].offset
-        sampling = self.calibrations[-1].sampling
-
-        start = int((start - offset) / sampling)
-        stop = int((end - offset) / sampling)
-
-        array = self.array[..., start:stop].sum(-1)
-        return Measurement(array, calibrations=self.calibrations[:-1])
-
-
-class DiffractionPatterns(Measurement):
-
-    def __init__(self, array, spatial_sampling, angular_sampling):
-        pass
-
-
-def probe_profile(probe_measurement: Measurement, angle: float = 0.) -> Measurement:
-    calibrations = probe_measurement.calibrations
-    extent = (calibrations[-2].sampling * probe_measurement.array.shape[-2],
-              calibrations[-1].sampling * probe_measurement.array.shape[-1])
-
-    point0 = np.array((extent[0] / 2, extent[1] / 2))
-    point1 = point0 + np.array([np.cos(np.pi * angle / 180), np.sin(np.pi * angle / 180)])
-    point0, point1 = _line_intersect_rectangle(point0, point1, (0., 0.), extent)
-    line_profile = interpolate_line(probe_measurement, point0, point1)
-    return line_profile
-
-
-def block_zeroth_order_spot(diffraction_pattern: Measurement):
-    shape = diffraction_pattern.shape
-    diffraction_pattern._array[..., shape[-2] // 2, shape[-1] // 2] = diffraction_pattern.array.min()
-    return diffraction_pattern
-
-
-def _line_intersect_rectangle(point0, point1, lower_corner, upper_corner):
-    if point0[0] == point1[0]:
-        return (point0[0], lower_corner[1]), (point0[0], upper_corner[1])
-
-    m = (point1[1] - point0[1]) / (point1[0] - point0[0])
-
-    def y(x):
-        return m * (x - point0[0]) + point0[1]
-
-    def x(y):
-        return (y - point0[1]) / m + point0[0]
-
-    if y(0) < lower_corner[1]:
-        intersect0 = (x(lower_corner[1]), y(x(lower_corner[1])))
-    else:
-        intersect0 = (0, y(lower_corner[0]))
-
-    if y(upper_corner[0]) > upper_corner[1]:
-        intersect1 = (x(upper_corner[1]), y(x(upper_corner[1])))
-    else:
-        intersect1 = (upper_corner[0], y(upper_corner[0]))
-
-    return intersect0, intersect1
-
-
-def interpolate_line(measurement: Measurement, start, end, gpts=None, sampling=None):
-    from abtem.scan import LineScan
-
-    array = np.squeeze(measurement.array)
-
-    if not (len(array.shape) == 2):
-        raise RuntimeError()
-
-    if (measurement.calibrations[-1] is None) or (measurement.calibrations[-2] is None):
-        raise RuntimeError()
-
-    if measurement.calibrations[-2].units != measurement.calibrations[-1].units:
-        raise RuntimeError()
-
-    if (gpts is None) & (sampling is None):
-        sampling = (measurement.calibrations[-2].sampling + measurement.calibrations[-1].sampling) / 2.
-
-    x = np.linspace(measurement.calibrations[-2].offset,
-                    measurement.shape[-2] * measurement.calibrations[-2].sampling,
-                    measurement.shape[-2])
-    y = np.linspace(measurement.calibrations[1].offset,
-                    measurement.shape[-1] * measurement.calibrations[-1].sampling,
-                    measurement.shape[-1])
-
-    line_scan = LineScan(start=start, end=end, gpts=gpts, sampling=sampling)
-
-    interpolated_array = interpn((x, y), array, line_scan.get_positions())
-
-    return Measurement(interpolated_array,
-                       Calibration(offset=0,
-                                   sampling=line_scan.sampling[0],
-                                   units=measurement.calibrations[-2].units,
-                                   name=measurement.calibrations[-2].name))
-
-
-def calculate_fwhm(measurement: Measurement):
-    """Function for calculating the full width at half maximum value for a 1D function."""
-
-    array = measurement.array
-    peak_idx = np.argmax(array)
-    peak_value = array[peak_idx]
-    left = np.argmin(np.abs(array[:peak_idx] - peak_value / 2))
-    right = peak_idx + np.argmin(np.abs(array[peak_idx:] - peak_value / 2))
-
-    fwhm = right - left
-    if measurement.calibrations[0] is not None:
-        fwhm = fwhm * measurement.calibrations[0].sampling
-
-    return fwhm
-
-
-def center_of_mass(measurement: Measurement):
-    """Function for estimating the intensity center-of-mass for a given measurement."""
-
-    if (measurement.dimensions != 3) and (measurement.dimensions != 4):
-        raise RuntimeError()
-
-    if not (measurement.calibrations[-1].units == measurement.calibrations[-2].units):
-        raise RuntimeError()
-
-    shape = measurement.array.shape[-2:]
-    center = np.array(shape) / 2 - np.array([.5 * (shape[-2] % 2), .5 * (shape[-1] % 2)])
-    com = np.zeros(measurement.array.shape[:-2] + (2,))
-
-    if measurement.dimensions == 3:
-        for i in range(measurement.array.shape[0]):
-            com[i] = scipy.ndimage.measurements.center_of_mass(measurement.array[i])
-        com = com - center[None]
-    else:
-        for i in range(measurement.array.shape[0]):
-            for j in range(measurement.array.shape[1]):
-                com[i, j] = scipy.ndimage.measurements.center_of_mass(measurement.array[i, j])
-        com = com - center[None, None]
-
-    com[..., 0] = com[..., 0] * measurement.calibrations[-2].sampling
-    com[..., 1] = com[..., 1] * measurement.calibrations[-1].sampling
-
-    return (Measurement(com[..., 0], measurement.calibrations[:-2], units='mrad', name='com_x'),
-            Measurement(com[..., 1], measurement.calibrations[:-2], units='mrad', name='com_y'))
+"""Module to describe the detection of scattered electron waves."""
+from collections.abc import Iterable
+from abc import ABCMeta
+from copy import copy
+from typing import Sequence, Tuple
+
+import h5py
+import imageio
+import numpy as np
+import scipy.misc
+import scipy.ndimage
+from scipy.interpolate import interpn
+from scipy.ndimage import zoom
+
+from abtem.device import asnumpy
+from abtem.visualize.mpl import show_measurement_2d, show_measurement_1d
+from abtem.utils import _disc_meshgrid
+
+
+class Calibration:
+    """
+    Calibration object
+
+    The calibration object represents the sampling of a uniformly sampled Measurement.
+
+    Parameters
+    ----------
+    offset: float
+        The lower bound of the sampling points.
+    sampling: float
+        The distance between sampling points.
+    units: str
+        The units of the calibration shown in plots.
+    name: str
+        The name of this calibration to be shown in plots.
+    """
+
+    def __init__(self, offset: float, sampling: float, units: str, name: str = ''):
+        self.offset = offset
+        self.sampling = sampling
+        self.units = units
+        self.name = name
+
+    def __eq__(self, other):
+        return ((self.offset == other.offset) &
+                (self.sampling == other.sampling) &
+                (self.units == other.units) &
+                (self.name == other.name))
+
+    def coordinates(self, n):
+        return np.linspace(self.offset, n * self.sampling + self.offset, n, endpoint=False)
+
+    def __copy__(self):
+        return self.__class__(self.offset, self.sampling, self.units, self.name)
+
+    def copy(self):
+        """
+        Make a copy.
+        """
+        return copy(self)
+
+
+def _fourier_space_offset(n: int, d: float):
+    """
+    Calculate the Fourier space offset.
+
+    Parameters
+    ----------
+    n : int
+        Number of sampling points.
+    d : float
+        Real space sampling density.
+    """
+
+    if n % 2 == 0:
+        return -1 / (2 * d)
+    else:
+        return -1 / (2 * d) + 1 / (2 * d * n)
+
+
+def calibrations_from_grid(gpts: Sequence[int],
+                           sampling: Sequence[float],
+                           names: Sequence[str] = None,
+                           units: str = None,
+                           fourier_space: bool = False,
+                           scale_factor: float = 1.0) -> Tuple[Calibration]:
+    """
+    Returns the spatial calibrations for a given computational grid and sampling.
+
+    Parameters
+    ----------
+    gpts: list of int
+        Number of grid points in the x and y directions.
+    sampling: list of float
+        Sampling of the potential in Å.
+    names: list of str, optional
+        The name of this calibration.
+    units: str, optional
+        Units for the calibration.
+    fourier_space: bool, optional
+        Setting for calibrating either in the reciprocal or real space. Default is False.
+    scale_factor: float, optional
+        Scaling factor for the calibration. Default is 1.0.
+
+    Returns
+    -------
+    calibrations: Tuple of Calibrations
+    """
+
+    if names is None:
+        names = ('',) * len(gpts)
+    elif len(names) != len(gpts):
+        raise RuntimeError()
+
+    if units is None:
+        if fourier_space:
+            units = '1 / Å'
+        else:
+            units = 'Å'
+
+    calibrations = ()
+    if fourier_space:
+        for name, n, d in zip(names, gpts, sampling):
+            r = n * d
+            offset = _fourier_space_offset(n, d)
+            calibrations += (Calibration(offset * scale_factor, 1 / r * scale_factor, units, name),)
+    else:
+        for name, d in zip(names, sampling):
+            calibrations += (Calibration(0., d * scale_factor, units, name),)
+
+    return calibrations
+
+
+class Measurement:  # (metaclass=ABCMeta):
+    """
+    Measurement object.
+
+    Parameters
+    ----------
+    array: ndarray
+        The array representing the measurements. The array can be any dimension.
+    calibrations: list of Calibration objects
+        The calibration for each dimension of the measurement array.
+    units: str
+        The units of the array values to be displayed in plots.
+    name: str
+        The name of the array values to be displayed in plots.
+    """
+
+    def __init__(self, array, calibrations=None, units='', name=''):
+
+        if issubclass(array.__class__, self.__class__):
+            measurement = array
+
+            array = measurement.array
+            calibrations = measurement.calibrations
+            units = measurement.array
+            name = measurement.name
+
+        if not isinstance(calibrations, Iterable):
+            calibrations = [calibrations] * len(array.shape)
+
+        if len(calibrations) != len(array.shape):
+            raise RuntimeError(
+                'The number of calibrations must equal the number of array dimensions. For undefined use None.')
+
+        self._array = asnumpy(array)
+        self._calibrations = calibrations
+        self._units = units
+        self._name = name
+
+    def __getitem__(self, args):
+        if isinstance(args, Iterable):
+            args += (slice(None),) * (len(self.array.shape) - len(args))
+        else:
+            args = (args,) + (slice(None),) * (len(self.array.shape) - 1)
+
+        new_array = self.array[args]
+        new_calibrations = []
+        for i, (arg, calibration) in enumerate(zip(args, self.calibrations)):
+            if isinstance(arg, slice):
+                if arg.start is None:
+                    offset = calibration.offset
+                else:
+                    offset = arg.start * calibration.sampling + calibration.offset
+
+                new_calibrations.append(Calibration(offset=offset,
+                                                    sampling=calibration.sampling,
+                                                    units=calibration.units, name=calibration.name))
+            elif isinstance(arg, Iterable):
+                new_calibrations.append(None)
+
+            elif not isinstance(arg, int):
+                raise TypeError('Indices must be integers or slices, not float')
+
+        return self.__class__(new_array, new_calibrations)
+
+    @property
+    def extent(self):
+        extent = ()
+        for i, calibration in enumerate(self.calibrations):
+            if calibration is None:
+                extent += (None, None)
+            else:
+                extent += (calibration.offset, calibration.offset + self.array.shape[i] * calibration.sampling)
+        return extent
+
+    def __len__(self):
+        return self.shape[0]
+
+    @property
+    def array(self):
+        """
+        Array of measurements.
+        """
+        return self._array
+
+    # @array.setter
+    # def array(self, array):
+    #     """
+    #     Array of measurements.
+    #     """
+    #     self._array[:] = array
+
+    @property
+    def shape(self):
+        """
+        The shape of the measurement array.
+        """
+        return self._array.shape
+
+    @property
+    def units(self):
+        """
+        The units of the array values to be displayed in plots.
+        """
+        return self._units
+
+    @property
+    def name(self):
+        """
+        The name of the array values to be displayed in plots.
+        """
+        return self._name
+
+    @property
+    def dimensions(self):
+        """
+        The measurement dimensions.
+        """
+        return len(self.array.shape)
+
+    @property
+    def calibrations(self):
+        """
+        The measurement calibrations.
+        """
+        return self._calibrations
+
+    def check_match_calibrations(self, other):
+        for calibration, other_calibration in zip(self.calibrations, other.calibrations):
+            if not calibration == other_calibration:
+                raise ValueError('Calibration mismatch, operation not possible.')
+
+    def __isub__(self, other):
+        if isinstance(other, self.__class__):
+            self.check_match_calibrations(other)
+            self._array -= other.array
+        else:
+            self._array -= asnumpy(other)
+
+    def __sub__(self, other):
+        if isinstance(other, self.__class__):
+            self.check_match_calibrations(other)
+            new_array = self.array - other.array
+        else:
+            new_array = self._array - asnumpy(other)
+        return self.__class__(new_array, calibrations=self.calibrations, units=self.units, name=self.name)
+
+    def __iadd__(self, other):
+        if isinstance(other, self.__class__):
+            self.check_match_calibrations(other)
+            self._array += other.array
+        else:
+            self._array += asnumpy(other)
+
+    def __add__(self, other):
+        if isinstance(other, self.__class__):
+            self.check_match_calibrations(other)
+            new_array = self.array + other.array
+        else:
+            new_array = self._array + asnumpy(other)
+        return self.__class__(new_array, calibrations=self.calibrations, units=self.units, name=self.name)
+
+    def _reduction(self, reduction_function, axis):
+        if not isinstance(axis, Iterable):
+            axis = (axis,)
+
+        array = reduction_function(self.array, axis=axis)
+
+        axis = [d % len(self.calibrations) for d in axis]
+        calibrations = [self.calibrations[i] for i in range(len(self.calibrations)) if i not in axis]
+
+        return self.__class__(array, calibrations)
+
+    # def integrate(self, axes, start=0, end=None, use_units=True):
+    #
+    #     if end is None:
+    #         end = ()
+    #         for axis in axes:
+    #             end += (self.array.shape[axis],)
+    #
+    #     else:
+    #         end = list(end)
+    #         for axis in axes:
+    #             end[axis]
+    #
+    #     if not isinstance(axes, Iterable):
+    #         axes = (axes,)
+    #
+    #     if not isinstance(start, Iterable):
+    #         start = (start,) * len(axes)
+    #
+    #     if not isinstance(end, Iterable):
+    #         end = (end,) * len(axes)
+
+    def sum(self, axis):
+        """
+        Sum of measurment elements over a given axis.
+
+        Parameters
+        ----------
+        axis: int or tuple of ints
+            Axis or axes along which a sum is performed. If axis is negative it counts from the last to the first axis.
+
+        Returns
+        -------
+        Measurement
+            A measurement with the same shape, but with the specified axis removed.
+        """
+        return self._reduction(np.mean, axis)
+
+    def mean(self, axis):
+        """
+        Mean of measurment elements over a given axis.
+
+        Parameters
+        ----------
+        axis: int or tuple of ints
+            Axis or axes along which a sum is performed. If axis is negative it counts from the last to the first axis.
+
+        Returns
+        -------
+        Measurement object
+            A measurement with the same shape, but with the specified axis removed.
+        """
+        return self._reduction(np.mean, axis)
+
+    def interpolate(self, new_sampling):
+        import warnings
+        warnings.filterwarnings('ignore', '.*output shape of zoom.*')
+
+        scale_factors = [calibration.sampling / new_sampling for calibration in self.calibrations]
+        new_array = zoom(self.array, scale_factors, mode='wrap')
+
+        calibrations = []
+        for calibration in self.calibrations:
+            calibrations.append(copy(calibration))
+            calibrations[-1].sampling = new_sampling
+
+        return self.__class__(new_array, calibrations, name=self.name, units=self.units)
+
+    def tile(self, multiples):
+        """
+        Tile the measurement.
+
+        Parameters
+        ----------
+        multiples: two int
+            The number of repetitions of the measurement along each axis.
+
+        Returns
+        -------
+        Measurement object
+            The tiled potential.
+        """
+        new_array = np.tile(self._array, multiples)
+        return self.__class__(new_array, self.calibrations, name=self.name, units=self.units)
+
+    @classmethod
+    def read(cls, path):
+        """
+        Read measurement from a hdf5 file.
+
+        path: str
+            The path to read the file.
+        """
+
+        with h5py.File(path, 'r') as f:
+            datasets = {}
+            for key in f.keys():
+                datasets[key] = f.get(key)[()]
+
+        calibrations = []
+        for i in range(len(datasets['offset'])):
+            calibrations.append(Calibration(offset=datasets['offset'][i],
+                                            sampling=datasets['sampling'][i],
+                                            units=datasets['units'][i].decode('utf-8'),
+                                            name=datasets['name'][i].decode('utf-8')))
+
+        # print(datasets['array'].shape)
+        # import matplotlib.pyplot as plt
+        # plt.imshow(datasets['array'])
+        # plt.show()
+
+        return cls(datasets['array'], calibrations)
+
+    def write(self, path, mode='w'):
+        """
+        Write measurement to a hdf5 file.
+
+        path: str
+            The path to write the file.
+        """
+
+        with h5py.File(path, mode) as f:
+            f.create_dataset('array', data=self.array)
+            f.create_dataset('offset', data=[calibration.offset for calibration in self.calibrations])
+            f.create_dataset('sampling', data=[calibration.sampling for calibration in self.calibrations])
+            units = [calibration.units.encode('utf-8') for calibration in self.calibrations]
+            f.create_dataset('units', (len(units),), 'S10', units)
+            names = [calibration.name.encode('utf-8') for calibration in self.calibrations]
+            f.create_dataset('name', (len(names),), 'S10', names)
+
+        return path
+
+    def save_as_image(self, path):
+        """
+        Write the measurement array to an image file. The array will be normalized and converted to 16-bit integers.
+
+        path: str
+            The path to write the file.
+        """
+
+        if self.dimensions != 2:
+            raise RuntimeError('Only 2d measurements can be saved as an image.')
+
+        array = (self.array - self.array.min()) / self.array.ptp() * np.iinfo(np.uint16).max
+        array = array.astype(np.uint16)
+        imageio.imwrite(path, array.T)
+
+    def __copy__(self):
+        calibrations = []
+        for calibration in self.calibrations:
+            calibrations.append(copy(calibration))
+        return self.__class__(self._array.copy(), calibrations=calibrations)
+
+    def copy(self):
+        """
+        Make a copy.
+        """
+        return copy(self)
+
+    def squeeze(self):
+        new_meaurement = self.copy()
+        calibrations = [calib for calib, num_elem in zip(self.calibrations, self.array.shape) if num_elem > 1]
+        new_meaurement._calibrations = calibrations
+        new_meaurement._array = np.squeeze(asnumpy(new_meaurement.array))
+        return new_meaurement
+
+    def interpolate_line(self, start, end, gpts=None, sampling=None):
+        from abtem.scan import LineScan
+
+        if not (self.dimensions == 2):
+            raise RuntimeError()
+
+        if (self.calibrations[0] is None) or (self.calibrations[1] is None):
+            raise RuntimeError()
+
+        if self.calibrations[0].units != self.calibrations[1].units:
+            raise RuntimeError()
+
+        if (gpts is None) & (sampling is None):
+            sampling = (self.calibrations[0].sampling + self.calibrations[1].sampling) / 2.
+
+        x = np.linspace(self.calibrations[0].offset, self.shape[0] * self.calibrations[0].sampling, self.shape[0])
+        y = np.linspace(self.calibrations[1].offset, self.shape[1] * self.calibrations[1].sampling, self.shape[1])
+
+        scan = LineScan(start=start, end=end, gpts=gpts, sampling=sampling)
+
+        interpolated_array = interpn((x, y), self.array, scan.get_positions())
+
+        calibration = Calibration(offset=0, sampling=scan.sampling[0],
+                                  units=self.calibrations[0].units,
+                                  name=self.calibrations[0].name)
+        return Measurement(interpolated_array, calibration)
+
+    def show(self, ax=None, **kwargs):
+        """
+        Show the measurement.
+
+        Parameters
+        ----------
+        kwargs:
+            Additional keyword arguments for the abtem.plot.show_image function.
+        """
+        if self.dimensions == 1:
+            return show_measurement_1d(self, ax=ax, **kwargs)
+        else:
+            return show_measurement_2d(self, ax=ax, **kwargs)
+
+
+class FlexibleAnnularMeasurement(Measurement):
+
+    def __init__(self, array, spatial_sampling, angular_sampling, angular_offset=0.):
+        if not isinstance(spatial_sampling, Iterable):
+            spatial_sampling = (spatial_sampling,) * (len(array.shape) - 1)
+
+        calibrations = [Calibration(0., d, 'Å', name) for d, name in zip(spatial_sampling, ('x', 'y'))]
+        calibrations += [Calibration(angular_offset, angular_sampling, 'mrad', 'alpha')]
+
+        super().__init__(array, calibrations)
+
+    def integrate(self, start, end):
+        offset = self.calibrations[-1].offset
+        sampling = self.calibrations[-1].sampling
+
+        start = int((start - offset) / sampling)
+        stop = int((end - offset) / sampling)
+
+        array = self.array[..., start:stop].sum(-1)
+        return Measurement(array, calibrations=self.calibrations[:-1])
+
+
+class DiffractionPatterns(Measurement):
+
+    def __init__(self, array, spatial_sampling, angular_sampling):
+        pass
+
+
+def probe_profile(probe_measurement: Measurement, angle: float = 0.) -> Measurement:
+    calibrations = probe_measurement.calibrations
+    extent = (calibrations[-2].sampling * probe_measurement.array.shape[-2],
+              calibrations[-1].sampling * probe_measurement.array.shape[-1])
+
+    point0 = np.array((extent[0] / 2, extent[1] / 2))
+    point1 = point0 + np.array([np.cos(np.pi * angle / 180), np.sin(np.pi * angle / 180)])
+    point0, point1 = _line_intersect_rectangle(point0, point1, (0., 0.), extent)
+    line_profile = interpolate_line(probe_measurement, point0, point1)
+    return line_profile
+
+
+def block_zeroth_order_spot(diffraction_pattern: Measurement, angular_radius=1):
+    alpha_x = diffraction_pattern.calibrations[-2].coordinates(diffraction_pattern.array.shape[-2])
+    alpha_y = diffraction_pattern.calibrations[-1].coordinates(diffraction_pattern.array.shape[-1])
+
+    alpha_x, alpha_y = np.meshgrid(alpha_x, alpha_y, indexing='ij')
+
+    alpha = alpha_x ** 2 + alpha_y ** 2
+    block = alpha > angular_radius ** 2
+
+    diffraction_pattern._array *= block
+    return diffraction_pattern
+
+
+def _line_intersect_rectangle(point0, point1, lower_corner, upper_corner):
+    if point0[0] == point1[0]:
+        return (point0[0], lower_corner[1]), (point0[0], upper_corner[1])
+
+    m = (point1[1] - point0[1]) / (point1[0] - point0[0])
+
+    def y(x):
+        return m * (x - point0[0]) + point0[1]
+
+    def x(y):
+        return (y - point0[1]) / m + point0[0]
+
+    if y(0) < lower_corner[1]:
+        intersect0 = (x(lower_corner[1]), y(x(lower_corner[1])))
+    else:
+        intersect0 = (0, y(lower_corner[0]))
+
+    if y(upper_corner[0]) > upper_corner[1]:
+        intersect1 = (x(upper_corner[1]), y(x(upper_corner[1])))
+    else:
+        intersect1 = (upper_corner[0], y(upper_corner[0]))
+
+    return intersect0, intersect1
+
+
+def interpolate_line(measurement: Measurement, start, end, gpts=None, sampling=None):
+    from abtem.scan import LineScan
+
+    array = np.squeeze(measurement.array)
+
+    if not (len(array.shape) == 2):
+        raise RuntimeError()
+
+    if (measurement.calibrations[-1] is None) or (measurement.calibrations[-2] is None):
+        raise RuntimeError()
+
+    if measurement.calibrations[-2].units != measurement.calibrations[-1].units:
+        raise RuntimeError()
+
+    if (gpts is None) & (sampling is None):
+        sampling = (measurement.calibrations[-2].sampling + measurement.calibrations[-1].sampling) / 2.
+
+    x = np.linspace(measurement.calibrations[-2].offset,
+                    measurement.shape[-2] * measurement.calibrations[-2].sampling,
+                    measurement.shape[-2])
+    y = np.linspace(measurement.calibrations[1].offset,
+                    measurement.shape[-1] * measurement.calibrations[-1].sampling,
+                    measurement.shape[-1])
+
+    line_scan = LineScan(start=start, end=end, gpts=gpts, sampling=sampling)
+
+    interpolated_array = interpn((x, y), array, line_scan.get_positions())
+
+    return Measurement(interpolated_array,
+                       Calibration(offset=0,
+                                   sampling=line_scan.sampling[0],
+                                   units=measurement.calibrations[-2].units,
+                                   name=measurement.calibrations[-2].name))
+
+
+def calculate_fwhm(measurement: Measurement):
+    """Function for calculating the full width at half maximum value for a 1D function."""
+
+    array = measurement.array
+    peak_idx = np.argmax(array)
+    peak_value = array[peak_idx]
+    left = np.argmin(np.abs(array[:peak_idx] - peak_value / 2))
+    right = peak_idx + np.argmin(np.abs(array[peak_idx:] - peak_value / 2))
+
+    fwhm = right - left
+    if measurement.calibrations[0] is not None:
+        fwhm = fwhm * measurement.calibrations[0].sampling
+
+    return fwhm
+
+
+def center_of_mass(measurement: Measurement):
+    """Function for estimating the intensity center-of-mass for a given measurement."""
+
+    if (measurement.dimensions != 3) and (measurement.dimensions != 4):
+        raise RuntimeError()
+
+    if not (measurement.calibrations[-1].units == measurement.calibrations[-2].units):
+        raise RuntimeError()
+
+    shape = measurement.array.shape[-2:]
+    center = np.array(shape) / 2 - np.array([.5 * (shape[-2] % 2), .5 * (shape[-1] % 2)])
+    com = np.zeros(measurement.array.shape[:-2] + (2,))
+
+    if measurement.dimensions == 3:
+        for i in range(measurement.array.shape[0]):
+            com[i] = scipy.ndimage.measurements.center_of_mass(measurement.array[i])
+        com = com - center[None]
+    else:
+        for i in range(measurement.array.shape[0]):
+            for j in range(measurement.array.shape[1]):
+                com[i, j] = scipy.ndimage.measurements.center_of_mass(measurement.array[i, j])
+        com = com - center[None, None]
+
+    com[..., 0] = com[..., 0] * measurement.calibrations[-2].sampling
+    com[..., 1] = com[..., 1] * measurement.calibrations[-1].sampling
+
+    return (Measurement(com[..., 0], measurement.calibrations[:-2], units='mrad', name='com_x'),
+            Measurement(com[..., 1], measurement.calibrations[:-2], units='mrad', name='com_y'))
```

### Comparing `abtem-1.0.0b8/abtem/noise.py` & `abtem-1.0.0b9/abtem/noise.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,180 +1,180 @@
-"""Module for describing different kinds of noise."""
-import numpy as np
-from scipy.interpolate import RegularGridInterpolator
-
-from abtem.measure import Measurement
-
-
-def _pixel_times(dwell_time, flyback_time, shape):
-    """
-    Pixel times internal function
-
-    Function for calculating scan pixel times.
-
-    Parameters
-    ----------
-    dwell_time : float
-        Dwell time on a single pixel in s.
-    flyback_time : float
-        Flyback time for the scanning probe at the end of each scan line in s.
-    shape : two ints
-        Dimensions of a scan in pixels.
-    """
-
-    line_time = (dwell_time * shape[1]) + flyback_time
-    slow_time = np.tile(np.linspace(line_time, shape[0] * line_time, shape[0])[:, None], (1, shape[1]))
-    fast_time = np.tile(np.linspace((line_time - flyback_time) / shape[1],
-                                    line_time - flyback_time, shape[1]), (shape[0], 1))
-    return slow_time + fast_time
-
-
-def _single_axis_distortion(time, max_frequency, num_components):
-    """
-    Single axis distortion internal function
-
-    Function for emulating a scan distortion along a single axis.
-
-    Parameters
-    ----------
-    time : float
-        Time constant for the distortion in s.
-    max_frequency : float
-        Maximum noise frequency in 1 / s.
-    num_components: int
-        Number of frequency components.
-    """
-
-    frequencies = np.random.rand(num_components, 1, 1) * max_frequency
-    amplitudes = np.random.rand(num_components, 1, 1) / np.sqrt(frequencies)
-    displacements = np.random.rand(num_components, 1, 1) / frequencies
-    return (amplitudes * np.sin(2 * np.pi * (time + displacements) * frequencies)).sum(axis=0)
-
-
-def _make_displacement_field(time, max_frequency, num_components, rms_power):
-    """
-    Displacement field creation internal function
-
-    Function to create a displacement field to emulate 2D scan distortion.
-
-    Parameters
-    ----------
-    time : float
-       Time constant for the distortion in s.
-    max_frequency : float
-       Maximum noise frequency in 1 / s.
-    num_components : int
-       Number of frequency components.
-    rms_power : float
-       Root-mean-square power of the distortion.
-    """
-
-    profile_x = _single_axis_distortion(time, max_frequency, num_components)
-    profile_y = _single_axis_distortion(time, max_frequency, num_components)
-
-    x_mag_deviation = np.gradient(profile_x, axis=1)
-    y_mag_deviation = np.gradient(profile_y, axis=0)
-
-    frame_mag_deviation = (1 + x_mag_deviation) * (1 + y_mag_deviation) - 1
-    frame_mag_deviation = np.sqrt(np.mean(frame_mag_deviation ** 2))
-
-    # 235.5 = 2.355 * 100 %; 2.355 converts from 1/e width to FWHM
-
-    profile_x *= rms_power / (235.5 * frame_mag_deviation)
-    profile_y *= rms_power / (235.5 * frame_mag_deviation)
-
-    return profile_x, profile_y
-
-
-def _apply_displacement_field(image, distortion_x, distortion_y):
-    """
-    Displacement field applying function
-
-    Function to apply a displacement field to an image.
-
-    Parameters
-    ----------
-    image : ndarray
-        Image array.
-    distortion_x : ndarray
-        Displacement field along the x axis.
-    distortion_y : ndarray
-        Displacement field along the y axis.
-    """
-
-    x = np.arange(0, image.shape[0])
-    y = np.arange(0, image.shape[1])
-
-    interpolating_function = RegularGridInterpolator([x, y], image, fill_value=None)
-
-    y, x = np.meshgrid(y, x)
-    p = np.array([(x + distortion_x).ravel(), (y + distortion_y).ravel()]).T
-
-    p[:, 0] = np.clip(p[:, 0], 0, x.max())
-    p[:, 1] = np.clip(p[:, 1], 0, y.max())
-
-    warped = interpolating_function(p)
-    return warped.reshape(image.shape)
-
-
-def add_scan_noise(measurement: Measurement, dwell_time: float, flyback_time: float, max_frequency: float,
-                   rms_power: float, num_components: int = 200):
-    """
-    Add scan noise to a measurement.
-
-    Parameters
-    ----------
-    measurement: Measurement object or 2d array
-        The measurement to add noise to.
-    dwell_time: float
-        Dwell time on a single pixel in s.
-    flyback_time: float
-        Flyback time for the scanning probe at the end of each scan line in s.
-    max_frequency: float
-        Maximum noise frequency in 1 / s.
-    rms_power: float
-        Root-mean-square power of the distortion in unit of percent.
-    num_components: int, optional
-        Number of frequency components. More components will be more 'white' but will take longer.
-
-    Returns
-    -------
-    measurement: Measurement object
-        The noisy measurement.
-    """
-
-    measurement = measurement.copy()
-    if isinstance(measurement, Measurement):
-        array = measurement.array
-    else:
-        array = measurement
-
-    time = _pixel_times(dwell_time, flyback_time, array.T.shape)
-    displacement_x, displacement_y = _make_displacement_field(time, max_frequency, num_components, rms_power)
-    array = _apply_displacement_field(array[:].T, displacement_x, displacement_y)
-    array[:] = array.T
-    return measurement
-
-
-def poisson_noise(measurement: Measurement, dose: float):
-    """
-    Add Poisson noise to a measurment.
-
-    Parameters
-    ----------
-    measurement: Measurement object
-        The measurement to add noise to.
-    dose: float
-        The irradiation dose in electrons per Å^2.
-
-    Returns
-    -------
-    measurement: Measurement object
-        The noisy measurement.
-    """
-
-    pixel_area = np.product([calibration.sampling for calibration in measurement.calibrations[-2:]])
-    measurement = measurement.copy()
-    array = measurement.array
-    measurement.array[:] = array / np.sum(array) * dose * pixel_area * np.prod(array.shape)
-    measurement.array[:] = np.random.poisson(array).astype(np.float)
-    return measurement
+"""Module for describing different kinds of noise."""
+import numpy as np
+from scipy.interpolate import RegularGridInterpolator
+
+from abtem.measure import Measurement
+
+
+def _pixel_times(dwell_time, flyback_time, shape):
+    """
+    Pixel times internal function
+
+    Function for calculating scan pixel times.
+
+    Parameters
+    ----------
+    dwell_time : float
+        Dwell time on a single pixel in s.
+    flyback_time : float
+        Flyback time for the scanning probe at the end of each scan line in s.
+    shape : two ints
+        Dimensions of a scan in pixels.
+    """
+
+    line_time = (dwell_time * shape[1]) + flyback_time
+    slow_time = np.tile(np.linspace(line_time, shape[0] * line_time, shape[0])[:, None], (1, shape[1]))
+    fast_time = np.tile(np.linspace((line_time - flyback_time) / shape[1],
+                                    line_time - flyback_time, shape[1]), (shape[0], 1))
+    return slow_time + fast_time
+
+
+def _single_axis_distortion(time, max_frequency, num_components):
+    """
+    Single axis distortion internal function
+
+    Function for emulating a scan distortion along a single axis.
+
+    Parameters
+    ----------
+    time : float
+        Time constant for the distortion in s.
+    max_frequency : float
+        Maximum noise frequency in 1 / s.
+    num_components: int
+        Number of frequency components.
+    """
+
+    frequencies = np.random.rand(num_components, 1, 1) * max_frequency
+    amplitudes = np.random.rand(num_components, 1, 1) / np.sqrt(frequencies)
+    displacements = np.random.rand(num_components, 1, 1) / frequencies
+    return (amplitudes * np.sin(2 * np.pi * (time + displacements) * frequencies)).sum(axis=0)
+
+
+def _make_displacement_field(time, max_frequency, num_components, rms_power):
+    """
+    Displacement field creation internal function
+
+    Function to create a displacement field to emulate 2D scan distortion.
+
+    Parameters
+    ----------
+    time : float
+       Time constant for the distortion in s.
+    max_frequency : float
+       Maximum noise frequency in 1 / s.
+    num_components : int
+       Number of frequency components.
+    rms_power : float
+       Root-mean-square power of the distortion.
+    """
+
+    profile_x = _single_axis_distortion(time, max_frequency, num_components)
+    profile_y = _single_axis_distortion(time, max_frequency, num_components)
+
+    x_mag_deviation = np.gradient(profile_x, axis=1)
+    y_mag_deviation = np.gradient(profile_y, axis=0)
+
+    frame_mag_deviation = (1 + x_mag_deviation) * (1 + y_mag_deviation) - 1
+    frame_mag_deviation = np.sqrt(np.mean(frame_mag_deviation ** 2))
+
+    # 235.5 = 2.355 * 100 %; 2.355 converts from 1/e width to FWHM
+
+    profile_x *= rms_power / (235.5 * frame_mag_deviation)
+    profile_y *= rms_power / (235.5 * frame_mag_deviation)
+
+    return profile_x, profile_y
+
+
+def _apply_displacement_field(image, distortion_x, distortion_y):
+    """
+    Displacement field applying function
+
+    Function to apply a displacement field to an image.
+
+    Parameters
+    ----------
+    image : ndarray
+        Image array.
+    distortion_x : ndarray
+        Displacement field along the x axis.
+    distortion_y : ndarray
+        Displacement field along the y axis.
+    """
+
+    x = np.arange(0, image.shape[0])
+    y = np.arange(0, image.shape[1])
+
+    interpolating_function = RegularGridInterpolator([x, y], image, fill_value=None)
+
+    y, x = np.meshgrid(y, x)
+    p = np.array([(x + distortion_x).ravel(), (y + distortion_y).ravel()]).T
+
+    p[:, 0] = np.clip(p[:, 0], 0, x.max())
+    p[:, 1] = np.clip(p[:, 1], 0, y.max())
+
+    warped = interpolating_function(p)
+    return warped.reshape(image.shape)
+
+
+def add_scan_noise(measurement: Measurement, dwell_time: float, flyback_time: float, max_frequency: float,
+                   rms_power: float, num_components: int = 200):
+    """
+    Add scan noise to a measurement.
+
+    Parameters
+    ----------
+    measurement: Measurement object or 2d array
+        The measurement to add noise to.
+    dwell_time: float
+        Dwell time on a single pixel in s.
+    flyback_time: float
+        Flyback time for the scanning probe at the end of each scan line in s.
+    max_frequency: float
+        Maximum noise frequency in 1 / s.
+    rms_power: float
+        Root-mean-square power of the distortion in unit of percent.
+    num_components: int, optional
+        Number of frequency components. More components will be more 'white' but will take longer.
+
+    Returns
+    -------
+    measurement: Measurement object
+        The noisy measurement.
+    """
+
+    measurement = measurement.copy()
+    if isinstance(measurement, Measurement):
+        array = measurement.array
+    else:
+        array = measurement
+
+    time = _pixel_times(dwell_time, flyback_time, array.T.shape)
+    displacement_x, displacement_y = _make_displacement_field(time, max_frequency, num_components, rms_power)
+    array = _apply_displacement_field(array[:].T, displacement_x, displacement_y)
+    array[:] = array.T
+    return measurement
+
+
+def poisson_noise(measurement: Measurement, dose: float):
+    """
+    Add Poisson noise to a measurment.
+
+    Parameters
+    ----------
+    measurement: Measurement object
+        The measurement to add noise to.
+    dose: float
+        The irradiation dose in electrons per Å^2.
+
+    Returns
+    -------
+    measurement: Measurement object
+        The noisy measurement.
+    """
+
+    pixel_area = np.product([calibration.sampling for calibration in measurement.calibrations[-2:]])
+    measurement = measurement.copy()
+    array = measurement.array
+    measurement.array[:] = array / np.sum(array) * dose * pixel_area * np.prod(array.shape)
+    measurement.array[:] = np.random.poisson(array).astype(np.float)
+    return measurement
```

### Comparing `abtem-1.0.0b8/abtem/parametrizations.py` & `abtem-1.0.0b9/abtem/parametrizations.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,140 +1,140 @@
-"""Module to describe independent atom model parametrizations of the scattering potential."""
-import csv
-import os
-from scipy.special import kn
-
-import numpy as np
-from numba import jit
-
-_ROOT = os.path.abspath(os.path.dirname(__file__))
-
-
-def _set_path(path):
-    """Internal function to set the parametrization data directory."""
-    return os.path.join(_ROOT, 'data', path)
-
-
-def load_parameters(filename):
-    """Function to load parameters from a CSV file."""
-    path = os.path.join(os.path.dirname(os.path.abspath(__file__)), filename)
-    parameters = {}
-    with open(path, 'r') as csvfile:
-        reader = csv.reader(csvfile, delimiter=',')
-        next(reader)
-        keys = next(reader)
-        for _, row in enumerate(reader):
-            values = list(map(float, row))
-            parameters[int(row[0])] = dict(zip(keys, values))
-    return parameters
-
-
-def load_lobato_parameters():
-    """Function to load the default Lobato parameters (doi:10.1107/S205327331401643X)."""
-    parameters = {}
-
-    for key, value in load_parameters(_set_path('lobato.txt')).items():
-        a = np.array([value[key] for key in ('a1', 'a2', 'a3', 'a4', 'a5')])
-        b = np.array([value[key] for key in ('b1', 'b2', 'b3', 'b4', 'b5')])
-        a = np.pi ** 2 * a / b ** (3 / 2.)
-        b = 2 * np.pi / np.sqrt(b)
-        parameters[key] = np.vstack((a, b))
-
-    return parameters
-
-
-@jit(nopython=True, nogil=True)
-def lobato_scattering(k2, p):
-    return ((p[0, 0] * (2. + p[1, 0] * k2) / (1. + p[1, 0] * k2) ** 2) +
-            (p[0, 1] * (2. + p[1, 1] * k2) / (1. + p[1, 1] * k2) ** 2) +
-            (p[0, 2] * (2. + p[1, 2] * k2) / (1. + p[1, 2] * k2) ** 2) +
-            (p[0, 3] * (2. + p[1, 3] * k2) / (1. + p[1, 3] * k2) ** 2) +
-            (p[0, 4] * (2. + p[1, 4] * k2) / (1. + p[1, 4] * k2) ** 2))
-
-
-@jit(nopython=True, nogil=True)
-def lobato(r, p):
-    return (p[0, 0] * (2. / (p[1, 0] * r) + 1.) * np.exp(-p[1, 0] * r) +
-            p[0, 1] * (2. / (p[1, 1] * r) + 1.) * np.exp(-p[1, 1] * r) +
-            p[0, 2] * (2. / (p[1, 2] * r) + 1.) * np.exp(-p[1, 2] * r) +
-            p[0, 3] * (2. / (p[1, 3] * r) + 1.) * np.exp(-p[1, 3] * r) +
-            p[0, 4] * (2. / (p[1, 4] * r) + 1.) * np.exp(-p[1, 4] * r))
-
-
-@jit(nopython=True, nogil=True)
-def dvdr_lobato(r, p):
-    dvdr = - (p[0, 0] * (2. / (p[1, 0] * r ** 2) + 2. / r + p[1, 0]) * np.exp(-p[1, 0] * r) +
-              p[0, 1] * (2. / (p[1, 1] * r ** 2) + 2. / r + p[1, 1]) * np.exp(-p[1, 1] * r) +
-              p[0, 2] * (2. / (p[1, 2] * r ** 2) + 2. / r + p[1, 2]) * np.exp(-p[1, 2] * r) +
-              p[0, 3] * (2. / (p[1, 3] * r ** 2) + 2. / r + p[1, 3]) * np.exp(-p[1, 3] * r) +
-              p[0, 4] * (2. / (p[1, 4] * r ** 2) + 2. / r + p[1, 4]) * np.exp(-p[1, 4] * r))
-
-    return dvdr
-
-
-@jit(nopython=True, nogil=True)
-def d2vdr2_lobato(r, p):
-    d2vdr2 = (p[0, 0] * (2 * (p[1, 0] * r + 2) / (p[1, 0] * r ** 3) +
-                         2 * (p[1, 0] * r + 1) / r ** 2 + p[1, 0] ** 2) * np.exp(-p[1, 0] * r) +
-              p[0, 1] * (2 * (p[1, 1] * r + 2) / (p[1, 1] * r ** 3) +
-                         2 * (p[1, 1] * r + 1) / r ** 2 + p[1, 1] ** 2) * np.exp(-p[1, 1] * r) +
-              p[0, 2] * (2 * (p[1, 2] * r + 2) / (p[1, 2] * r ** 3) +
-                         2 * (p[1, 2] * r + 1) / r ** 2 + p[1, 2] ** 2) * np.exp(-p[1, 2] * r) +
-              p[0, 3] * (2 * (p[1, 3] * r + 2) / (p[1, 3] * r ** 3) +
-                         2 * (p[1, 3] * r + 1) / r ** 2 + p[1, 3] ** 2) * np.exp(-p[1, 3] * r) +
-              p[0, 4] * (2 * (p[1, 4] * r + 2) / (p[1, 4] * r ** 3) +
-                         2 * (p[1, 4] * r + 1) / r ** 2 + p[1, 4] ** 2) * np.exp(-p[1, 4] * r))
-
-    return d2vdr2
-
-
-def load_kirkland_parameters():
-    """Function to load the Kirkland parameters (doi:10.1007/978-1-4419-6533-2)."""
-    parameters = {}
-
-    for key, value in load_parameters(_set_path('kirkland.txt')).items():
-        a = np.array([value[key] for key in ('a1', 'a2', 'a3')])
-        b = np.array([value[key] for key in ('b1', 'b2', 'b3')])
-        c = np.array([value[key] for key in ('c1', 'c2', 'c3')])
-        d = np.array([value[key] for key in ('d1', 'd2', 'd3')])
-        a = np.pi * a
-        b = 2. * np.pi * np.sqrt(b)
-        c = np.pi ** (3. / 2.) * c / d ** (3. / 2.)
-        d = np.pi ** 2 / d
-        parameters[key] = np.vstack((a, b, c, d))
-
-    return parameters
-
-
-@jit(nopython=True, nogil=True)
-def kirkland(r, p):
-    return (p[0, 0] * np.exp(-p[1, 0] * r) / r + p[2, 0] * np.exp(-p[3, 0] * r ** 2.) +
-            p[0, 1] * np.exp(-p[1, 1] * r) / r + p[2, 1] * np.exp(-p[3, 1] * r ** 2.) +
-            p[0, 2] * np.exp(-p[1, 2] * r) / r + p[2, 2] * np.exp(-p[3, 2] * r ** 2.))
-
-
-@jit(nopython=True, nogil=True)
-def dvdr_kirkland(r, p):
-    dvdr = (- p[0, 0] * (1 / r + p[1, 0]) * np.exp(-p[1, 0] * r) / r -
-            2 * p[2, 0] * p[3, 0] * r * np.exp(-p[3, 0] * r ** 2)
-            - p[0, 1] * (1 / r + p[1, 1]) * np.exp(-p[1, 1] * r) / r -
-            2 * p[2, 1] * p[3, 1] * r * np.exp(-p[3, 1] * r ** 2)
-            - p[0, 2] * (1 / r + p[1, 2]) * np.exp(-p[1, 2] * r) / r -
-            2 * p[2, 2] * p[3, 2] * r * np.exp(-p[3, 2] * r ** 2))
-    return dvdr
-
-
-def kirkland_projected(r, p):
-    v = (2 * p[0, 0] * kn(0, p[1, 0] * r) + np.sqrt(np.pi / p[3, 0]) * p[2, 0] * np.exp(-p[3, 0] * r ** 2.) +
-         2 * p[0, 1] * kn(0, p[1, 1] * r) + np.sqrt(np.pi / p[3, 1]) * p[2, 1] * np.exp(-p[3, 1] * r ** 2.) +
-         2 * p[0, 2] * kn(0, p[1, 2] * r) + np.sqrt(np.pi / p[3, 2]) * p[2, 2] * np.exp(-p[3, 2] * r ** 2.))
-    return v
-
-
-def kirkland_projected_fourier(k, p):
-    f = (4 * np.pi * p[0, 0] / (4 * np.pi ** 2 * k ** 2 + p[1, 0] ** 2) +
-         np.sqrt(np.pi / p[3, 0]) * p[2, 0] * np.pi / p[3, 0] * np.exp(-np.pi ** 2 * k ** 2. / p[3, 0]) +
-         4 * np.pi * p[0, 1] / (4 * np.pi ** 2 * k ** 2 + p[1, 1] ** 2) +
-         np.sqrt(np.pi / p[3, 1]) * p[2, 1] * np.pi / p[3, 1] * np.exp(-np.pi ** 2 * k ** 2. / p[3, 1]) +
-         4 * np.pi * p[0, 2] / (4 * np.pi ** 2 * k ** 2 + p[1, 2] ** 2) +
-         np.sqrt(np.pi / p[3, 2]) * p[2, 2] * np.pi / p[3, 2] * np.exp(-np.pi ** 2 * k ** 2. / p[3, 2]))
-    return f
+"""Module to describe independent atom model parametrizations of the scattering potential."""
+import csv
+import os
+from scipy.special import kn
+
+import numpy as np
+from numba import jit
+
+_ROOT = os.path.abspath(os.path.dirname(__file__))
+
+
+def _set_path(path):
+    """Internal function to set the parametrization data directory."""
+    return os.path.join(_ROOT, 'data', path)
+
+
+def load_parameters(filename):
+    """Function to load parameters from a CSV file."""
+    path = os.path.join(os.path.dirname(os.path.abspath(__file__)), filename)
+    parameters = {}
+    with open(path, 'r') as csvfile:
+        reader = csv.reader(csvfile, delimiter=',')
+        next(reader)
+        keys = next(reader)
+        for _, row in enumerate(reader):
+            values = list(map(float, row))
+            parameters[int(row[0])] = dict(zip(keys, values))
+    return parameters
+
+
+def load_lobato_parameters():
+    """Function to load the default Lobato parameters (doi:10.1107/S205327331401643X)."""
+    parameters = {}
+
+    for key, value in load_parameters(_set_path('lobato.txt')).items():
+        a = np.array([value[key] for key in ('a1', 'a2', 'a3', 'a4', 'a5')])
+        b = np.array([value[key] for key in ('b1', 'b2', 'b3', 'b4', 'b5')])
+        a = np.pi ** 2 * a / b ** (3 / 2.)
+        b = 2 * np.pi / np.sqrt(b)
+        parameters[key] = np.vstack((a, b))
+
+    return parameters
+
+
+@jit(nopython=True, nogil=True)
+def lobato_scattering(k2, p):
+    return ((p[0, 0] * (2. + p[1, 0] * k2) / (1. + p[1, 0] * k2) ** 2) +
+            (p[0, 1] * (2. + p[1, 1] * k2) / (1. + p[1, 1] * k2) ** 2) +
+            (p[0, 2] * (2. + p[1, 2] * k2) / (1. + p[1, 2] * k2) ** 2) +
+            (p[0, 3] * (2. + p[1, 3] * k2) / (1. + p[1, 3] * k2) ** 2) +
+            (p[0, 4] * (2. + p[1, 4] * k2) / (1. + p[1, 4] * k2) ** 2))
+
+
+@jit(nopython=True, nogil=True)
+def lobato(r, p):
+    return (p[0, 0] * (2. / (p[1, 0] * r) + 1.) * np.exp(-p[1, 0] * r) +
+            p[0, 1] * (2. / (p[1, 1] * r) + 1.) * np.exp(-p[1, 1] * r) +
+            p[0, 2] * (2. / (p[1, 2] * r) + 1.) * np.exp(-p[1, 2] * r) +
+            p[0, 3] * (2. / (p[1, 3] * r) + 1.) * np.exp(-p[1, 3] * r) +
+            p[0, 4] * (2. / (p[1, 4] * r) + 1.) * np.exp(-p[1, 4] * r))
+
+
+@jit(nopython=True, nogil=True)
+def dvdr_lobato(r, p):
+    dvdr = - (p[0, 0] * (2. / (p[1, 0] * r ** 2) + 2. / r + p[1, 0]) * np.exp(-p[1, 0] * r) +
+              p[0, 1] * (2. / (p[1, 1] * r ** 2) + 2. / r + p[1, 1]) * np.exp(-p[1, 1] * r) +
+              p[0, 2] * (2. / (p[1, 2] * r ** 2) + 2. / r + p[1, 2]) * np.exp(-p[1, 2] * r) +
+              p[0, 3] * (2. / (p[1, 3] * r ** 2) + 2. / r + p[1, 3]) * np.exp(-p[1, 3] * r) +
+              p[0, 4] * (2. / (p[1, 4] * r ** 2) + 2. / r + p[1, 4]) * np.exp(-p[1, 4] * r))
+
+    return dvdr
+
+
+@jit(nopython=True, nogil=True)
+def d2vdr2_lobato(r, p):
+    d2vdr2 = (p[0, 0] * (2 * (p[1, 0] * r + 2) / (p[1, 0] * r ** 3) +
+                         2 * (p[1, 0] * r + 1) / r ** 2 + p[1, 0] ** 2) * np.exp(-p[1, 0] * r) +
+              p[0, 1] * (2 * (p[1, 1] * r + 2) / (p[1, 1] * r ** 3) +
+                         2 * (p[1, 1] * r + 1) / r ** 2 + p[1, 1] ** 2) * np.exp(-p[1, 1] * r) +
+              p[0, 2] * (2 * (p[1, 2] * r + 2) / (p[1, 2] * r ** 3) +
+                         2 * (p[1, 2] * r + 1) / r ** 2 + p[1, 2] ** 2) * np.exp(-p[1, 2] * r) +
+              p[0, 3] * (2 * (p[1, 3] * r + 2) / (p[1, 3] * r ** 3) +
+                         2 * (p[1, 3] * r + 1) / r ** 2 + p[1, 3] ** 2) * np.exp(-p[1, 3] * r) +
+              p[0, 4] * (2 * (p[1, 4] * r + 2) / (p[1, 4] * r ** 3) +
+                         2 * (p[1, 4] * r + 1) / r ** 2 + p[1, 4] ** 2) * np.exp(-p[1, 4] * r))
+
+    return d2vdr2
+
+
+def load_kirkland_parameters():
+    """Function to load the Kirkland parameters (doi:10.1007/978-1-4419-6533-2)."""
+    parameters = {}
+
+    for key, value in load_parameters(_set_path('kirkland.txt')).items():
+        a = np.array([value[key] for key in ('a1', 'a2', 'a3')])
+        b = np.array([value[key] for key in ('b1', 'b2', 'b3')])
+        c = np.array([value[key] for key in ('c1', 'c2', 'c3')])
+        d = np.array([value[key] for key in ('d1', 'd2', 'd3')])
+        a = np.pi * a
+        b = 2. * np.pi * np.sqrt(b)
+        c = np.pi ** (3. / 2.) * c / d ** (3. / 2.)
+        d = np.pi ** 2 / d
+        parameters[key] = np.vstack((a, b, c, d))
+
+    return parameters
+
+
+@jit(nopython=True, nogil=True)
+def kirkland(r, p):
+    return (p[0, 0] * np.exp(-p[1, 0] * r) / r + p[2, 0] * np.exp(-p[3, 0] * r ** 2.) +
+            p[0, 1] * np.exp(-p[1, 1] * r) / r + p[2, 1] * np.exp(-p[3, 1] * r ** 2.) +
+            p[0, 2] * np.exp(-p[1, 2] * r) / r + p[2, 2] * np.exp(-p[3, 2] * r ** 2.))
+
+
+@jit(nopython=True, nogil=True)
+def dvdr_kirkland(r, p):
+    dvdr = (- p[0, 0] * (1 / r + p[1, 0]) * np.exp(-p[1, 0] * r) / r -
+            2 * p[2, 0] * p[3, 0] * r * np.exp(-p[3, 0] * r ** 2)
+            - p[0, 1] * (1 / r + p[1, 1]) * np.exp(-p[1, 1] * r) / r -
+            2 * p[2, 1] * p[3, 1] * r * np.exp(-p[3, 1] * r ** 2)
+            - p[0, 2] * (1 / r + p[1, 2]) * np.exp(-p[1, 2] * r) / r -
+            2 * p[2, 2] * p[3, 2] * r * np.exp(-p[3, 2] * r ** 2))
+    return dvdr
+
+
+def kirkland_projected(r, p):
+    v = (2 * p[0, 0] * kn(0, p[1, 0] * r) + np.sqrt(np.pi / p[3, 0]) * p[2, 0] * np.exp(-p[3, 0] * r ** 2.) +
+         2 * p[0, 1] * kn(0, p[1, 1] * r) + np.sqrt(np.pi / p[3, 1]) * p[2, 1] * np.exp(-p[3, 1] * r ** 2.) +
+         2 * p[0, 2] * kn(0, p[1, 2] * r) + np.sqrt(np.pi / p[3, 2]) * p[2, 2] * np.exp(-p[3, 2] * r ** 2.))
+    return v
+
+
+def kirkland_projected_fourier(k, p):
+    f = (4 * np.pi * p[0, 0] / (4 * np.pi ** 2 * k ** 2 + p[1, 0] ** 2) +
+         np.sqrt(np.pi / p[3, 0]) * p[2, 0] * np.pi / p[3, 0] * np.exp(-np.pi ** 2 * k ** 2. / p[3, 0]) +
+         4 * np.pi * p[0, 1] / (4 * np.pi ** 2 * k ** 2 + p[1, 1] ** 2) +
+         np.sqrt(np.pi / p[3, 1]) * p[2, 1] * np.pi / p[3, 1] * np.exp(-np.pi ** 2 * k ** 2. / p[3, 1]) +
+         4 * np.pi * p[0, 2] / (4 * np.pi ** 2 * k ** 2 + p[1, 2] ** 2) +
+         np.sqrt(np.pi / p[3, 2]) * p[2, 2] * np.pi / p[3, 2] * np.exp(-np.pi ** 2 * k ** 2. / p[3, 2]))
+    return f
```

### Comparing `abtem-1.0.0b8/abtem/plot.py` & `abtem-1.0.0b9/abtem/plot.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,285 +1,285 @@
-"""Module for plotting atoms, images, line scans, and diffraction patterns."""
-from collections.abc import Iterable
-
-from numbers import Number
-from abc import ABCMeta, abstractmethod
-
-import matplotlib.pyplot as plt
-import numpy as np
-from abtem.cpu_kernels import abs2
-from ase.data import covalent_radii
-from ase.data.colors import cpk_colors
-from matplotlib.collections import PatchCollection
-from matplotlib.patches import Circle
-
-#: Array to facilitate the display of cell boundaries.
-_cube = np.array([[[0, 0, 0], [0, 0, 1]],
-                  [[0, 0, 0], [0, 1, 0]],
-                  [[0, 0, 0], [1, 0, 0]],
-                  [[0, 0, 1], [0, 1, 1]],
-                  [[0, 0, 1], [1, 0, 1]],
-                  [[0, 1, 0], [1, 1, 0]],
-                  [[0, 1, 0], [0, 1, 1]],
-                  [[1, 0, 0], [1, 1, 0]],
-                  [[1, 0, 0], [1, 0, 1]],
-                  [[0, 1, 1], [1, 1, 1]],
-                  [[1, 0, 1], [1, 1, 1]],
-                  [[1, 1, 0], [1, 1, 1]]])
-
-
-def _plane2axes(plane):
-    """Internal function for extracting axes from a plane."""
-    axes = ()
-    last_axis = [0, 1, 2]
-    for axis in list(plane):
-        if axis == 'x':
-            axes += (0,)
-            last_axis.remove(0)
-        if axis == 'y':
-            axes += (1,)
-            last_axis.remove(1)
-        if axis == 'z':
-            axes += (2,)
-            last_axis.remove(2)
-    return axes + (last_axis[0],)
-
-
-def show_atoms(atoms, repeat=(1, 1), scans=None, plane='xy', ax=None, scale_atoms=.5, title=None, numbering=False):
-    """
-    Show atoms function
-
-    Function to display atoms, especially in Jupyter notebooks.
-
-    Parameters
-    ----------
-    atoms : ASE atoms object
-        The atoms to be shown.
-    repeat : two ints, optional
-        Tiling of the image. Default is (1,1), ie. no tiling.
-    scans : ndarray, optional
-        List of scans to apply. Default is None.
-    plane : str
-        The projection plane.
-    ax : axes object
-        pyplot axes object.
-    scale_atoms : float
-        Scaling factor for the atom display sizes. Default is 0.5.
-    title : str
-        Title of the displayed image. Default is None.
-    numbering : bool
-        Option to set plot numbering. Default is False.
-    """
-
-    if ax is None:
-        fig, ax = plt.subplots()
-
-    axes = _plane2axes(plane)
-
-    atoms = atoms.copy()
-    cell = atoms.cell
-    atoms *= repeat + (1,)
-
-    for line in _cube:
-        cell_lines = np.array([np.dot(line[0], cell), np.dot(line[1], cell)])
-        ax.plot(cell_lines[:, axes[0]], cell_lines[:, axes[1]], 'k-')
-
-    if len(atoms) > 0:
-        positions = atoms.positions[:, axes[:2]]
-        order = np.argsort(atoms.positions[:, axes[2]])
-        positions = positions[order]
-
-        colors = cpk_colors[atoms.numbers[order]]
-        sizes = covalent_radii[atoms.numbers[order]] * scale_atoms
-
-        circles = []
-        for position, size in zip(positions, sizes):
-            circles.append(Circle(position, size))
-
-        coll = PatchCollection(circles, facecolors=colors, edgecolors='black')
-        ax.add_collection(coll)
-
-        ax.axis('equal')
-        ax.set_xlabel(plane[0] + ' [Å]')
-        ax.set_ylabel(plane[1] + ' [Å]')
-
-        ax.set_title(title)
-
-        if numbering:
-            for i, (position, size) in enumerate(zip(positions, sizes)):
-                ax.annotate('{}'.format(order[i]), xy=position, ha="center", va="center")
-
-    if scans is not None:
-        if not isinstance(scans, Iterable):
-            scans = [scans]
-
-        for scan in scans:
-            scan.add_to_mpl_plot(ax)
-
-
-def show_image(array, calibrations, ax=None, title=None, colorbar=False, cmap='gray', figsize=None, scans=None,
-               log_scale=False, discrete=False, cbar_label=None, vmin=None, vmax=None, power=1,**kwargs):
-    """
-    Show image function
-
-    Function to display an image.
-
-    Parameters
-    ----------
-    array : ndarray
-        Image array.
-    calibrations : tuple of calibration objects.
-        Spatial calibrations.
-    ax : axes object
-        pyplot axes object.
-    title : str, optional
-        Image title. Default is None.
-    colorbar : bool, optional
-        Option to show a colorbar. Default is False.
-    cmap : str, optional
-        Colormap name. Default is 'gray'.
-    figsize : float, pair of float, optional
-        Size of the figure in inches, either as a square for one number or a rectangle for two. Default is None.
-    scans : ndarray, optional
-        Array of scans. Default is None.
-    log_scale : bool, optional
-        Option to set a logarithmic intensity scale. Default is False.
-    discrete : bool, optional
-        Option to discretize intensity values to integers. Default is False.
-    cbar_label : str, optional
-        Text label for the color bar. Default is None.
-    vmin : float, optional
-        Minimum of the intensity scale. Default is None.
-    vmax : float, optional
-        Maximum of the intensity scale. Default is None.
-    kwargs :
-        Remaining keyword arguments are passed to pyplot.
-    """
-
-    if np.iscomplexobj(array):
-        array = abs2(array)
-
-    if ax is None:
-        fig, ax = plt.subplots(figsize=figsize)
-
-    if log_scale:
-        if isinstance(log_scale, Number) & (not isinstance(log_scale, bool)):
-            array = np.log(1 + log_scale * array)
-        else:
-            array = np.log(array)
-
-    if power != 1.:
-        array = array ** power
-
-    extent = []
-    for calibration, num_elem in zip(calibrations, array.shape):
-        extent.append(calibration.offset)
-        extent.append(calibration.offset + num_elem * calibration.sampling)
-
-    if vmin is None:
-        vmin = np.min(array)
-        if discrete:
-            vmin -= .5
-
-    if vmax is None:
-        vmax = np.max(array)
-        if discrete:
-            vmax += .5
-
-    if discrete:
-        cmap = plt.get_cmap(cmap, np.max(array) - np.min(array) + 1)
-
-    im = ax.imshow(array.T, extent=extent, cmap=cmap, origin='lower', vmin=vmin, vmax=vmax, **kwargs)
-
-    if colorbar:
-        cax = plt.colorbar(im, ax=ax, label=cbar_label)
-        if discrete:
-            cax.set_ticks(ticks=np.arange(np.min(array), np.max(array) + 1))
-
-    ax.set_xlabel('{} [{}]'.format(calibrations[0].name, calibrations[0].units))
-    ax.set_ylabel('{} [{}]'.format(calibrations[1].name, calibrations[1].units))
-
-    if title is not None:
-        ax.set_title(title)
-
-    if scans is not None:
-        if not isinstance(scans, Iterable):
-            scans = [scans]
-
-        for scan in scans:
-            scan.add_to_mpl_plot(ax)
-
-    return ax, im
-
-
-def show_line(array, calibration, ax=None, title=None, legend=False, **kwargs):
-    """
-    Show line function
-
-    Function to display a line scan.
-
-    Parameters
-    ----------
-    array : ndarray
-        Array of measurement values along a line.
-    calibration : calibration object
-        Spatial calibration for the line.
-    ax : axes object, optional
-        pyplot axes object.
-    title : str, optional
-        Title for the plot. Default is None.
-    legend : bool, optional
-        Option to display a plot legend. Default is False.
-    kwargs :
-       Remaining keyword arguments are passed to pyplot.
-    """
-
-    x = np.linspace(calibration.offset, calibration.offset + len(array) * calibration.sampling, len(array))
-
-    if ax is None:
-        ax = plt.subplot()
-
-    ax.plot(x, array, **kwargs)
-    ax.set_xlabel('{} [{}]'.format(calibration.name, calibration.units))
-
-    if title is not None:
-        ax.set_title(title)
-
-    if legend:
-        ax.legend()
-
-    return ax
-
-
-class PlotableMixin:
-
-    @abstractmethod
-    def add_to_bokeh_plot(self, p, *args, **kwargs):
-        pass
-
-    def show_bokeh(self, p=None, push_notebook=False, **kwargs):
-        from bokeh import plotting
-        from bokeh.io import show
-
-        if push_notebook:
-            from bokeh.io import push_notebook
-
-        if p is None:
-            p = plotting.Figure(plot_width=300, plot_height=300)
-
-        self.add_to_bokeh_plot(p, push_notebook=push_notebook, **kwargs)
-
-        show(p, notebook_handle=push_notebook)
-        return p
-
-    @abstractmethod
-    def add_to_mpl_plot(self, *args, **kwargs):
-        pass
-
-    def show(self, ax=None, *args, **kwargs):
-        import matplotlib.pyplot as plt
-
-        if ax is None:
-            ax = plt.subplot()
-        self.add_to_mpl_plot(ax=ax, **kwargs)
-        plt.show()
-        return ax
+"""Module for plotting atoms, images, line scans, and diffraction patterns."""
+from collections.abc import Iterable
+
+from numbers import Number
+from abc import ABCMeta, abstractmethod
+
+import matplotlib.pyplot as plt
+import numpy as np
+from abtem.cpu_kernels import abs2
+from ase.data import covalent_radii
+from ase.data.colors import cpk_colors
+from matplotlib.collections import PatchCollection
+from matplotlib.patches import Circle
+
+#: Array to facilitate the display of cell boundaries.
+_cube = np.array([[[0, 0, 0], [0, 0, 1]],
+                  [[0, 0, 0], [0, 1, 0]],
+                  [[0, 0, 0], [1, 0, 0]],
+                  [[0, 0, 1], [0, 1, 1]],
+                  [[0, 0, 1], [1, 0, 1]],
+                  [[0, 1, 0], [1, 1, 0]],
+                  [[0, 1, 0], [0, 1, 1]],
+                  [[1, 0, 0], [1, 1, 0]],
+                  [[1, 0, 0], [1, 0, 1]],
+                  [[0, 1, 1], [1, 1, 1]],
+                  [[1, 0, 1], [1, 1, 1]],
+                  [[1, 1, 0], [1, 1, 1]]])
+
+
+def _plane2axes(plane):
+    """Internal function for extracting axes from a plane."""
+    axes = ()
+    last_axis = [0, 1, 2]
+    for axis in list(plane):
+        if axis == 'x':
+            axes += (0,)
+            last_axis.remove(0)
+        if axis == 'y':
+            axes += (1,)
+            last_axis.remove(1)
+        if axis == 'z':
+            axes += (2,)
+            last_axis.remove(2)
+    return axes + (last_axis[0],)
+
+
+def show_atoms(atoms, repeat=(1, 1), scans=None, plane='xy', ax=None, scale_atoms=.5, title=None, numbering=False):
+    """
+    Show atoms function
+
+    Function to display atoms, especially in Jupyter notebooks.
+
+    Parameters
+    ----------
+    atoms : ASE atoms object
+        The atoms to be shown.
+    repeat : two ints, optional
+        Tiling of the image. Default is (1,1), ie. no tiling.
+    scans : ndarray, optional
+        List of scans to apply. Default is None.
+    plane : str
+        The projection plane.
+    ax : axes object
+        pyplot axes object.
+    scale_atoms : float
+        Scaling factor for the atom display sizes. Default is 0.5.
+    title : str
+        Title of the displayed image. Default is None.
+    numbering : bool
+        Option to set plot numbering. Default is False.
+    """
+
+    if ax is None:
+        fig, ax = plt.subplots()
+
+    axes = _plane2axes(plane)
+
+    atoms = atoms.copy()
+    cell = atoms.cell
+    atoms *= repeat + (1,)
+
+    for line in _cube:
+        cell_lines = np.array([np.dot(line[0], cell), np.dot(line[1], cell)])
+        ax.plot(cell_lines[:, axes[0]], cell_lines[:, axes[1]], 'k-')
+
+    if len(atoms) > 0:
+        positions = atoms.positions[:, axes[:2]]
+        order = np.argsort(atoms.positions[:, axes[2]])
+        positions = positions[order]
+
+        colors = cpk_colors[atoms.numbers[order]]
+        sizes = covalent_radii[atoms.numbers[order]] * scale_atoms
+
+        circles = []
+        for position, size in zip(positions, sizes):
+            circles.append(Circle(position, size))
+
+        coll = PatchCollection(circles, facecolors=colors, edgecolors='black')
+        ax.add_collection(coll)
+
+        ax.axis('equal')
+        ax.set_xlabel(plane[0] + ' [Å]')
+        ax.set_ylabel(plane[1] + ' [Å]')
+
+        ax.set_title(title)
+
+        if numbering:
+            for i, (position, size) in enumerate(zip(positions, sizes)):
+                ax.annotate('{}'.format(order[i]), xy=position, ha="center", va="center")
+
+    if scans is not None:
+        if not isinstance(scans, Iterable):
+            scans = [scans]
+
+        for scan in scans:
+            scan.add_to_mpl_plot(ax)
+
+
+def show_image(array, calibrations, ax=None, title=None, colorbar=False, cmap='gray', figsize=None, scans=None,
+               log_scale=False, discrete=False, cbar_label=None, vmin=None, vmax=None, power=1,**kwargs):
+    """
+    Show image function
+
+    Function to display an image.
+
+    Parameters
+    ----------
+    array : ndarray
+        Image array.
+    calibrations : tuple of calibration objects.
+        Spatial calibrations.
+    ax : axes object
+        pyplot axes object.
+    title : str, optional
+        Image title. Default is None.
+    colorbar : bool, optional
+        Option to show a colorbar. Default is False.
+    cmap : str, optional
+        Colormap name. Default is 'gray'.
+    figsize : float, pair of float, optional
+        Size of the figure in inches, either as a square for one number or a rectangle for two. Default is None.
+    scans : ndarray, optional
+        Array of scans. Default is None.
+    log_scale : bool, optional
+        Option to set a logarithmic intensity scale. Default is False.
+    discrete : bool, optional
+        Option to discretize intensity values to integers. Default is False.
+    cbar_label : str, optional
+        Text label for the color bar. Default is None.
+    vmin : float, optional
+        Minimum of the intensity scale. Default is None.
+    vmax : float, optional
+        Maximum of the intensity scale. Default is None.
+    kwargs :
+        Remaining keyword arguments are passed to pyplot.
+    """
+
+    if np.iscomplexobj(array):
+        array = abs2(array)
+
+    if ax is None:
+        fig, ax = plt.subplots(figsize=figsize)
+
+    if log_scale:
+        if isinstance(log_scale, Number) & (not isinstance(log_scale, bool)):
+            array = np.log(1 + log_scale * array)
+        else:
+            array = np.log(array)
+
+    if power != 1.:
+        array = array ** power
+
+    extent = []
+    for calibration, num_elem in zip(calibrations, array.shape):
+        extent.append(calibration.offset)
+        extent.append(calibration.offset + num_elem * calibration.sampling)
+
+    if vmin is None:
+        vmin = np.min(array)
+        if discrete:
+            vmin -= .5
+
+    if vmax is None:
+        vmax = np.max(array)
+        if discrete:
+            vmax += .5
+
+    if discrete:
+        cmap = plt.get_cmap(cmap, np.max(array) - np.min(array) + 1)
+
+    im = ax.imshow(array.T, extent=extent, cmap=cmap, origin='lower', vmin=vmin, vmax=vmax, **kwargs)
+
+    if colorbar:
+        cax = plt.colorbar(im, ax=ax, label=cbar_label)
+        if discrete:
+            cax.set_ticks(ticks=np.arange(np.min(array), np.max(array) + 1))
+
+    ax.set_xlabel('{} [{}]'.format(calibrations[0].name, calibrations[0].units))
+    ax.set_ylabel('{} [{}]'.format(calibrations[1].name, calibrations[1].units))
+
+    if title is not None:
+        ax.set_title(title)
+
+    if scans is not None:
+        if not isinstance(scans, Iterable):
+            scans = [scans]
+
+        for scan in scans:
+            scan.add_to_mpl_plot(ax)
+
+    return ax, im
+
+
+def show_line(array, calibration, ax=None, title=None, legend=False, **kwargs):
+    """
+    Show line function
+
+    Function to display a line scan.
+
+    Parameters
+    ----------
+    array : ndarray
+        Array of measurement values along a line.
+    calibration : calibration object
+        Spatial calibration for the line.
+    ax : axes object, optional
+        pyplot axes object.
+    title : str, optional
+        Title for the plot. Default is None.
+    legend : bool, optional
+        Option to display a plot legend. Default is False.
+    kwargs :
+       Remaining keyword arguments are passed to pyplot.
+    """
+
+    x = np.linspace(calibration.offset, calibration.offset + len(array) * calibration.sampling, len(array))
+
+    if ax is None:
+        ax = plt.subplot()
+
+    ax.plot(x, array, **kwargs)
+    ax.set_xlabel('{} [{}]'.format(calibration.name, calibration.units))
+
+    if title is not None:
+        ax.set_title(title)
+
+    if legend:
+        ax.legend()
+
+    return ax
+
+
+class PlotableMixin:
+
+    @abstractmethod
+    def add_to_bokeh_plot(self, p, *args, **kwargs):
+        pass
+
+    def show_bokeh(self, p=None, push_notebook=False, **kwargs):
+        from bokeh import plotting
+        from bokeh.io import show
+
+        if push_notebook:
+            from bokeh.io import push_notebook
+
+        if p is None:
+            p = plotting.Figure(plot_width=300, plot_height=300)
+
+        self.add_to_bokeh_plot(p, push_notebook=push_notebook, **kwargs)
+
+        show(p, notebook_handle=push_notebook)
+        return p
+
+    @abstractmethod
+    def add_to_mpl_plot(self, *args, **kwargs):
+        pass
+
+    def show(self, ax=None, *args, **kwargs):
+        import matplotlib.pyplot as plt
+
+        if ax is None:
+            ax = plt.subplot()
+        self.add_to_mpl_plot(ax=ax, **kwargs)
+        plt.show()
+        return ax
```

### Comparing `abtem-1.0.0b8/abtem/potentials.py` & `abtem-1.0.0b9/abtem/potentials.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,999 +1,1029 @@
-"""Module to calculate potentials using the independent atom model."""
-from abc import ABCMeta, abstractmethod
-from typing import Union, Sequence, Callable, Generator
-
-import h5py
-import numpy as np
-from copy import copy
-
-from ase import Atoms
-from ase import units
-
-from scipy.optimize import brentq
-
-from abtem.base_classes import Grid, HasGridMixin, Cache, cached_method, HasAcceleratorMixin, Accelerator, Event, \
-    watched_property, AntialiasFilter
-from abtem.device import get_device_function, get_array_module, get_array_module_from_device, copy_to_device, \
-    HasDeviceMixin, asnumpy
-from abtem.measure import calibrations_from_grid, Measurement
-from abtem.parametrizations import kirkland, dvdr_kirkland, load_kirkland_parameters, kirkland_projected_fourier
-from abtem.parametrizations import lobato, dvdr_lobato, load_lobato_parameters
-from abtem.plot import show_image
-from abtem.structures import is_cell_orthogonal
-from abtem.tanh_sinh import integrate, tanh_sinh_nodes_and_weights
-from abtem.temperature import AbstractFrozenPhonons, DummyFrozenPhonons
-from abtem.utils import energy2sigma, ProgressBar, generate_batches
-
-# Vacuum permitivity in ASE units
-eps0 = units._eps0 * units.A ** 2 * units.s ** 4 / (units.kg * units.m ** 3)
-
-# Conversion factor from unitless potential parametrizations to ASE potential units
-kappa = 4 * np.pi * eps0 / (2 * np.pi * units.Bohr * units._e * units.C)
-
-
-class AbstractPotential(HasGridMixin, metaclass=ABCMeta):
-    """
-    Potential abstract base class
-
-    Base class common for all potentials.
-    """
-
-    def __len__(self):
-        return self.num_slices
-
-    @property
-    @abstractmethod
-    def num_slices(self):
-        """The number of projected potential slices."""
-        pass
-
-    def check_slice_idx(self, i):
-        """Raises an error if i is greater than the number of slices."""
-        if i >= self.num_slices:
-            raise RuntimeError('Slice index {} too large for potential with {} slices'.format(i, self.num_slices))
-
-    def generate_transmission_functions(self, energy, first_slice=0, last_slice=None, max_batch=1):
-        """
-        Generate the potential one slice at a time.
-
-        Parameters
-        ----------
-        start: int
-            First potential slice.
-        end: int, optional
-            Last potential slice.
-
-        Returns
-        -------
-        generator of ProjectedPotential objects
-        """
-        antialias_filter = AntialiasFilter()
-
-        for start, end, potential_slice in self.generate_slices(first_slice, last_slice, max_batch=max_batch):
-            yield start, end, potential_slice.as_transmission_function(energy,
-                                                                       in_place=True,
-                                                                       max_batch=max_batch,
-                                                                       antialias_filter=antialias_filter)
-
-    @abstractmethod
-    def generate_slices(self, first_slice=0, last_slice=None, max_batch=1):
-        """
-        Generate the potential one slice at a time.
-
-        Parameters
-        ----------
-        start: int
-            First potential slice.
-        end: int, optional
-            Last potential slice.
-
-        Returns
-        -------
-        generator of ProjectedPotential objects
-        """
-
-        pass
-
-    @abstractmethod
-    def get_slice_thickness(self, i):
-        """
-        Get the slice thickness [Å].
-
-        Parameters
-        ----------
-        i: int
-            Slice index.
-        """
-
-        pass
-
-    def __iter__(self):
-        for _, __, p in self.generate_slices(max_batch=1):
-            yield p
-
-    def get_projected_potential(self, items) -> 'PotentialArray':
-        """
-        Get projected potential for the slice or slices.
-
-        Parameters
-        ----------
-        items: int or slice
-            The potential slice(s) (either a single index or a range, ie. a Python slice [start:end]) to include in the
-            projection.
-
-        Returns
-        -------
-        ProjectedPotential object
-            The projected potential.
-        """
-
-        if isinstance(items, int):
-            if items >= self.num_slices:
-                raise StopIteration
-            return next(self.generate_slices(items, items + 1, max_batch=1))[2]
-
-        elif isinstance(items, slice):
-            raise NotImplementedError()
-
-            if items.start is None:
-                start = 0
-            else:
-                start = items.start
-
-            if items.stop is None:
-                stop = len(self)
-            else:
-                stop = items.stop
-
-            if items.step is None:
-                step = 1
-            else:
-                step = items.step
-
-            projected = self[start]
-            for i in range(start + 1, stop, step):
-                projected._array += self[i]._array
-                projected._thickness += self.get_slice_thickness(i)
-            return projected
-        else:
-            raise TypeError('Potential must indexed with integers or slices, not {}'.format(type(items)))
-
-    def __getitem__(self, items):
-        return self.get_projected_potential(items)
-
-    # def show(self, **kwargs):
-    #     """
-    #     Show the potential projection. This requires building all potential slices.
-    #
-    #     Parameters
-    #     ----------
-    #     kwargs:
-    #         Additional keyword arguments for abtem.plot.show_image.
-    #     """
-    #
-    #     self[:].show(**kwargs)
-
-    def copy(self):
-        """Make a copy."""
-        return copy(self)
-
-
-class AbstractPotentialBuilder(AbstractPotential):
-    """Potential builder abstract class."""
-
-    def __init__(self, precalculate=True, storage='cpu'):
-        self._precalculate = precalculate
-        self._storage = storage
-
-    def build(self, pbar: Union[bool, ProgressBar] = False, energy=None, max_batch=1, first_slice=0,
-              last_slice=None) -> 'PotentialArray':
-        """
-        Precalcaulate the potential as a potential array.
-
-        Parameters
-        ----------
-        pbar: bool
-            If true, show progress bar.
-
-        Returns
-        -------
-        PotentialArray object
-        """
-
-        self.grid.check_is_defined()
-
-        if last_slice is None:
-            last_slice = len(self)
-
-        storage_xp = get_array_module_from_device(self._storage)
-
-        if energy is None:
-            array = storage_xp.zeros((last_slice - first_slice,) + (self.gpts[0], self.gpts[1]), dtype=np.float32)
-            generator = self.generate_slices(max_batch=max_batch, first_slice=first_slice, last_slice=last_slice)
-        else:
-            array = storage_xp.zeros((last_slice - first_slice,) + (self.gpts[0], self.gpts[1]), dtype=np.complex64)
-            generator = self.generate_transmission_functions(energy=energy,
-                                                             max_batch=max_batch,
-                                                             first_slice=first_slice,
-                                                             last_slice=last_slice)
-
-        slice_thicknesses = np.zeros(last_slice - first_slice)
-
-        if isinstance(pbar, bool):
-            pbar = ProgressBar(total=len(self), desc='Potential', disable=not pbar)
-            close_pbar = True
-        else:
-            close_pbar = False
-
-        pbar.reset()
-        for start, end, potential_slice in generator:
-            array[start:end] = copy_to_device(potential_slice.array, self._storage)
-            slice_thicknesses[start:end] = potential_slice.slice_thicknesses
-            pbar.update(1)
-
-        pbar.refresh()
-
-        if close_pbar:
-            pbar.close()
-
-        if energy is None:
-            return PotentialArray(array, slice_thicknesses=slice_thicknesses, extent=self.extent)
-        else:
-            return TransmissionFunction(array, slice_thicknesses=slice_thicknesses, extent=self.extent, energy=energy)
-
-    def project(self):
-        return self.build().project()
-
-
-class AbstractTDSPotentialBuilder(AbstractPotentialBuilder):
-    """Thermal diffuse scattering builder abstract class."""
-
-    def __init__(self, precalculate=True, storage='cpu'):
-        super().__init__(precalculate=precalculate, storage=storage)
-
-    @property
-    @abstractmethod
-    def frozen_phonons(self):
-        pass
-
-    @abstractmethod
-    def generate_frozen_phonon_potentials(self, pbar):
-        pass
-
-
-class PotentialIntegrator:
-    """
-    Perform finite integrals of a radial function along a straight line.
-
-    Parameters
-    ----------
-    function: callable
-        Radial function to integrate.
-    r: array of float
-        The evaluation points of the integrals.
-    cutoff: float, optional
-        The radial function is assumed to be zero outside this threshold.
-    cache_size: int, optional
-        The maximum number of integrals that will be cached.
-    cache_key_decimals: int, optional
-        The number of decimals used in the cache keys.
-    tolerance: float, optional
-        The absolute error tolerance of the integrals.
-    """
-
-    def __init__(self,
-                 function: Callable,
-                 r: np.ndarray,
-                 cutoff: float = None,
-                 cache_size: int = 4096,
-                 cache_key_decimals: int = 2,
-                 tolerance: float = 1e-6):
-
-        self._function = function
-        self._r = r
-
-        if cutoff is None:
-            self._cutoff = r[-1]
-        else:
-            self._cutoff = cutoff
-
-        self._cache = Cache(cache_size)
-        self._cache_key_decimals = cache_key_decimals
-        self._tolerance = tolerance
-
-    @property
-    def r(self):
-        return self._r
-
-    @property
-    def cutoff(self):
-        return self._cutoff
-
-    def integrate(self, a: float, b: float):
-        """
-        Evaulate the integrals of the radial function at the evaluation points.
-
-        Parameters
-        ----------
-        a: float
-            Lower limit of integrals.
-        b: float
-            Upper limit of integrals.
-
-        Returns
-        -------
-        1d array
-            The evaulated integrals.
-        """
-
-        a = round(a, self._cache_key_decimals)
-        b = round(b, self._cache_key_decimals)
-
-        split = a * b < 0
-        a = max(min(a, b), -self.cutoff)
-        b = min(max(a, b), self.cutoff)
-        if split:  # split the integral
-            values1, derivatives1 = self._do_integrate(0, abs(a))
-            values2, derivatives2 = self._do_integrate(0, abs(b))
-            result = (values1 + values2, derivatives1 + derivatives2)
-        else:
-            result = self._do_integrate(a, b)
-        return result
-
-    @cached_method('_cache')
-    def _do_integrate(self, a, b):
-        zm = (b - a) / 2.
-        zp = (a + b) / 2.
-
-        def f(z):
-            return self._function(np.sqrt(self.r[0] ** 2 + (z * zm + zp) ** 2))
-
-        value, error_estimate, step_size, order = integrate(f, -1, 1, self._tolerance)
-        xk, wk = tanh_sinh_nodes_and_weights(step_size, order)
-
-        def f(z):
-            return self._function(np.sqrt(self.r[:, None] ** 2 + (z * zm + zp) ** 2))
-
-        values = np.sum(f(xk[None]) * wk[None], axis=1) * zm
-        derivatives = np.diff(values) / np.diff(self.r)
-        return values, derivatives
-
-
-def pad_atoms(atoms: Atoms, margin: float):
-    """
-    Repeat the atoms in x and y, retaining only the repeated atoms within the margin distance from the cell boundary.
-
-    Parameters
-    ----------
-    atoms: ASE Atoms object
-        The atoms that should be padded.
-    margin: float
-        The padding margin.
-
-    Returns
-    -------
-    ASE Atoms object
-        Padded atoms.
-    """
-
-    if not is_cell_orthogonal(atoms):
-        raise RuntimeError('The cell of the atoms must be orthogonal.')
-
-    left = atoms[atoms.positions[:, 0] < margin]
-    left.positions[:, 0] += atoms.cell[0, 0]
-    right = atoms[atoms.positions[:, 0] > atoms.cell[0, 0] - margin]
-    right.positions[:, 0] -= atoms.cell[0, 0]
-
-    atoms += left + right
-
-    top = atoms[atoms.positions[:, 1] < margin]
-    top.positions[:, 1] += atoms.cell[1, 1]
-    bottom = atoms[atoms.positions[:, 1] > atoms.cell[1, 1] - margin]
-    bottom.positions[:, 1] -= atoms.cell[1, 1]
-    atoms += top + bottom
-    return atoms
-
-
-def _disc_meshgrid(r):
-    """Internal function to return all indices inside a disk with a given radius."""
-    cols = np.zeros((2 * r + 1, 2 * r + 1)).astype(np.int32)
-    cols[:] = np.linspace(0, 2 * r, 2 * r + 1) - r
-    rows = cols.T
-    inside = (rows ** 2 + cols ** 2) <= r ** 2
-    return rows[inside], cols[inside]
-
-
-def superpose_deltas(positions, z, array):
-    shape = array.shape[-2:]
-    xp = get_array_module(array)
-    rounded = xp.floor(positions).astype(xp.int32)
-    rows, cols = rounded[:, 0], rounded[:, 1]
-
-    array[z, rows, cols] += (1 - (positions[:, 0] - rows)) * (1 - (positions[:, 1] - cols))
-    array[z, (rows + 1) % shape[0], cols] += (positions[:, 0] - rows) * (1 - (positions[:, 1] - cols))
-    array[z, rows, (cols + 1) % shape[1]] += (1 - (positions[:, 0] - rows)) * (positions[:, 1] - cols)
-    array[z, (rows + 1) % shape[0], (cols + 1) % shape[1]] += (rows - positions[:, 0]) * (cols - positions[:, 1])
-
-
-class Potential(AbstractTDSPotentialBuilder, HasDeviceMixin):
-    """
-    Potential object.
-
-    The potential object is used to calculate the electrostatic potential of a set of atoms represented by an ASE atoms
-    object. The potential is calculated with the Independent Atom Model (IAM) using a user-defined parametrization
-    of the atomic potentials.
-
-    Parameters
-    ----------
-    atoms: Atoms or FrozenPhonons object
-        Atoms or FrozenPhonons defining the atomic configuration(s) used in the IAM of the electrostatic potential(s).
-    gpts: one or two int, optional
-        Number of grid points describing each slice of the potential.
-    sampling: one or two float, optional
-        Lateral sampling of the potential [1 / Å].
-    slice_thickness: float, optional
-        Thickness of the potential slices in Å for calculating the number of slices used by the multislice algorithm.
-        Default is 0.5 Å.
-    parametrization: 'lobato' or 'kirkland', optional
-        The potential parametrization describes the radial dependence of the potential for each element. Two of the
-        most accurate parametrizations are available by Lobato et. al. and Kirkland. The abTEM default is 'lobato'.
-        See the citation guide for references.
-    projection: 'finite' or 'infinite'
-        If 'finite' the 3d potential is numerically integrated between the slice boundaries. If 'infinite' the infinite
-        potential projection of each atom will be assigned to a single slice.
-    cutoff_tolerance: float, optional
-        The error tolerance used for deciding the radial cutoff distance of the potential [eV / e]. The cutoff is only
-        relevant for potentials using the 'finite' projection scheme.
-    device: str, optional
-        The device used for calculating the potential. The default is 'cpu'.
-    storage: str, optional
-        The device on which to store the created potential. The default is 'None', defaulting to the chosen device.
-    """
-
-    def __init__(self,
-                 atoms: Union[Atoms, AbstractFrozenPhonons] = None,
-                 gpts: Union[int, Sequence[int]] = None,
-                 sampling: Union[float, Sequence[float]] = None,
-                 slice_thickness: float = .5,
-                 parametrization: str = 'lobato',
-                 projection: str = 'finite',
-                 cutoff_tolerance: float = 1e-3,
-                 device='cpu',
-                 precalculate=True,
-                 storage=None):
-
-        self._cutoff_tolerance = cutoff_tolerance
-        self._parametrization = parametrization
-        self._slice_thickness = slice_thickness
-
-        self._storage = storage
-
-        if parametrization.lower() == 'lobato':
-            self._parameters = load_lobato_parameters()
-            self._function = lobato
-            self._derivative = dvdr_lobato
-
-        elif parametrization.lower() == 'kirkland':
-            self._parameters = load_kirkland_parameters()
-            self._function = kirkland
-            self._derivative = dvdr_kirkland
-        else:
-            raise RuntimeError('Parametrization {} not recognized'.format(parametrization))
-
-        if projection == 'infinite':
-            if parametrization.lower() != 'kirkland':
-                raise RuntimeError('Infinite projections are only implemented for the Kirkland parametrization')
-        elif (projection != 'finite'):
-            raise RuntimeError('Projection must be "finite" or "infinite"')
-
-        self._projection = projection
-
-        if isinstance(atoms, AbstractFrozenPhonons):
-            self._frozen_phonons = atoms
-        else:
-            self._frozen_phonons = DummyFrozenPhonons(atoms)
-
-        atoms = next(iter(self._frozen_phonons))
-
-        if np.abs(atoms.cell[2, 2]) < 1e-12:
-            raise RuntimeError('Atoms cell has no thickness')
-
-        if not is_cell_orthogonal(atoms):
-            raise RuntimeError('Atoms are not orthogonal')
-
-        self._atoms = atoms
-        self._grid = Grid(extent=np.diag(atoms.cell)[:2], gpts=gpts, sampling=sampling, lock_extent=True)
-
-        self._cutoffs = {}
-        self._integrators = {}
-        self._disc_indices = {}
-
-        def grid_changed_callback(*args, **kwargs):
-            self._integrators = {}
-            self._disc_indices = {}
-
-        self.grid.changed.register(grid_changed_callback)
-        self.changed = Event()
-
-        self._device = device
-
-        if storage is None:
-            storage = device
-
-        super().__init__(precalculate=precalculate, storage=storage)
-
-    @property
-    def parametrization(self):
-        """The potential parametrization."""
-        return self._parameters
-
-    @property
-    def projection(self):
-        """The projection method."""
-        return self._projection
-
-    @property
-    def parameters(self):
-        """The parameters of the potential parametrization."""
-        return self._parameters
-
-    @property
-    def function(self):
-        """The potential function of the parametrization."""
-        return self._function
-
-    @property
-    def atoms(self):
-        """Atoms object defining the atomic configuration."""
-        return self._atoms
-
-    @property
-    def frozen_phonons(self):
-        """FrozenPhonons object defining the atomic configuration(s)."""
-        return self._frozen_phonons
-
-    @property
-    def cutoff_tolerance(self):
-        """The error tolerance used for deciding the radial cutoff distance of the potential [eV / e]."""
-        return self._cutoff_tolerance
-
-    @property
-    def num_slices(self):
-        """The number of projected potential slices."""
-        return int(np.ceil(self._atoms.cell[2, 2] / self._slice_thickness))
-
-    @property
-    def slice_thickness(self):
-        """The thickness of the projected potential slices."""
-        return self._slice_thickness
-
-    @slice_thickness.setter
-    @watched_property('changed')
-    def slice_thickness(self, value):
-        self._slice_thickness = value
-
-    def get_slice_thickness(self, i):
-        return self._atoms.cell[2, 2] / self.num_slices
-
-    def get_cutoff(self, number: int) -> float:
-        """
-        Cutoff distance for atomic number given an error tolerance.
-
-        Parameters
-        ----------
-        number: int
-            Atomic number.
-
-        Returns
-        -------
-        cutoff: float
-            The potential cutoff.
-        """
-
-        try:
-            return self._cutoffs[number]
-        except KeyError:
-            def f(r):
-                return self.function(r, self.parameters[number]) - self.cutoff_tolerance
-
-            self._cutoffs[number] = brentq(f, 1e-7, 1000)
-            return self._cutoffs[number]
-
-    def get_tapered_function(self, number: int) -> Callable:
-        """
-        Tapered potential function for atomic number.
-
-        Parameters
-        ----------
-        number: int
-            Atomic number.
-
-        Returns
-        -------
-        callable
-        """
-
-        cutoff = self.get_cutoff(number)
-        rolloff = .85 * cutoff
-
-        def soft_function(r):
-            result = np.zeros_like(r)
-            valid = r < cutoff
-            transition = valid * (r > rolloff)
-            result[valid] = self._function(r[valid], self.parameters[number])
-            result[transition] *= (np.cos(np.pi * (r[transition] - rolloff) / (cutoff - rolloff)) + 1.) / 2
-            return result
-
-        return soft_function
-
-    def get_integrator(self, number: int) -> PotentialIntegrator:
-        """
-        Potential integrator for atomic number.
-
-        Parameters
-        ----------
-        number: int
-            Atomic number.
-
-        Returns
-        -------
-        PotentialIntegrator object
-        """
-
-        try:
-            return self._integrators[number]
-        except KeyError:
-            cutoff = self.get_cutoff(number)
-            soft_function = self.get_tapered_function(number)
-            inner_cutoff = np.min(self.sampling)
-            num_points = int(np.ceil(cutoff / np.min(self.sampling) * 5.))
-            r = np.geomspace(inner_cutoff, cutoff, num_points)
-            self._integrators[number] = PotentialIntegrator(soft_function, r, cutoff)
-            return self._integrators[number]
-
-    def _get_radial_interpolation_points(self, number):
-        """Internal function for the indices of the radial interpolation points."""
-        try:
-            return self._disc_indices[number]
-        except KeyError:
-            cutoff = self.get_cutoff(number)
-            margin = np.int(np.ceil(cutoff / np.min(self.sampling)))
-            rows, cols = _disc_meshgrid(margin)
-            self._disc_indices[number] = np.hstack((rows[:, None], cols[:, None]))
-            return self._disc_indices[number]
-
-    def generate_slices(self, first_slice=0, last_slice=None, max_batch=1) -> Generator:
-        self.grid.check_is_defined()
-
-        if last_slice is None:
-            last_slice = len(self)
-
-        if self.projection == 'finite':
-            return self._generate_slices_finite(first_slice=first_slice, last_slice=last_slice, max_batch=max_batch)
-        else:
-            return self._generate_slices_infinite(first_slice=first_slice, last_slice=last_slice, max_batch=max_batch)
-
-    def _generate_slices_infinite(self, first_slice=0, last_slice=None, max_batch=1) -> Generator:
-        xp = get_array_module_from_device(self._device)
-        fft2_convolve = get_device_function(xp, 'fft2_convolve')
-
-        atoms = self.atoms.copy()
-        atoms.wrap()
-        indices_by_number = {number: np.where(atoms.numbers == number)[0] for number in np.unique(atoms.numbers)}
-
-        kx = xp.fft.fftfreq(self.gpts[0], self.sampling[0])
-        ky = xp.fft.fftfreq(self.gpts[1], self.sampling[1])
-        kx, ky = xp.meshgrid(kx, ky, indexing='ij')
-        k = xp.sqrt(kx ** 2 + ky ** 2)
-
-        sinc = xp.sinc(xp.sqrt((kx * self.sampling[0]) ** 2 + (kx * self.sampling[1]) ** 2))
-
-        scattering_factors = {}
-        for atomic_number in indices_by_number.keys():
-            f = kirkland_projected_fourier(k, self.parameters[atomic_number])
-            scattering_factors[atomic_number] = (f / (sinc * self.sampling[0] * self.sampling[1] * kappa)).astype(
-                xp.complex64)
-
-        slice_idx = np.floor(atoms.positions[:, 2] / atoms.cell[2, 2] * self.num_slices).astype(np.int)
-
-        start, end = next(generate_batches(last_slice - first_slice, max_batch=max_batch, start=first_slice))
-        array = xp.zeros((end - start, len(indices_by_number),) + self.gpts, dtype=xp.complex64)
-
-        for start, end in generate_batches(last_slice - first_slice, max_batch=max_batch, start=first_slice):
-            array[:] = 0.
-            slice_thicknesses = [self.get_slice_thickness(i) for i in range(start, end)]
-
-            for j, (number, indices) in enumerate(indices_by_number.items()):
-                in_slice = (slice_idx >= start) * (slice_idx < end) * (atoms.numbers == number)
-                slice_atoms = atoms[in_slice]
-
-                positions = xp.asarray(slice_atoms.positions[:, :2] / self.sampling)
-                superpose_deltas(positions, slice_idx[in_slice] - start, array[:, j])
-                fft2_convolve(array[:, j], scattering_factors[number])
-
-            yield start, end, PotentialArray(array.real.sum(1)[:end - start], slice_thicknesses, extent=self.extent)
-
-    def _generate_slices_finite(self, first_slice=0, last_slice=None, max_batch=1) -> Generator:
-        xp = get_array_module_from_device(self._device)
-
-        interpolate_radial_functions = get_device_function(xp, 'interpolate_radial_functions')
-
-        atoms = self.atoms.copy()
-        atoms.wrap()
-        indices_by_number = {number: np.where(atoms.numbers == number)[0] for number in np.unique(atoms.numbers)}
-
-        array = xp.zeros(self.gpts, dtype=xp.float32)
-        a = np.sum([self.get_slice_thickness(i) for i in range(0, first_slice)])
-        for i in range(first_slice, last_slice):
-            array[:] = 0.
-            b = a + self.get_slice_thickness(i)
-
-            for number, indices in indices_by_number.items():
-                slice_atoms = atoms[indices]
-
-                integrator = self.get_integrator(number)
-
-                disc_indices = xp.asarray(self._get_radial_interpolation_points(number))
-
-                slice_atoms = slice_atoms[(slice_atoms.positions[:, 2] > a - integrator.cutoff) *
-                                          (slice_atoms.positions[:, 2] < b + integrator.cutoff)]
-
-                slice_atoms = pad_atoms(slice_atoms, integrator.cutoff)
-
-                if len(slice_atoms) == 0:
-                    continue
-
-                vr = np.zeros((len(slice_atoms), integrator.r.shape[0]), np.float32)
-                dvdr = np.zeros((len(slice_atoms), integrator.r.shape[0]), np.float32)
-                for j, atom in enumerate(slice_atoms):
-                    am, bm = a - atom.z, b - atom.z
-                    vr[j], dvdr[j, :-1] = integrator.integrate(am, bm)
-                vr = xp.asarray(vr, dtype=xp.float32)
-                dvdr = xp.asarray(dvdr, dtype=xp.float32)
-                r = xp.asarray(integrator.r, dtype=xp.float32)
-
-                slice_positions = xp.asarray(slice_atoms.positions[:, :2], dtype=xp.float32)
-                sampling = xp.asarray(self.sampling, dtype=xp.float32)
-
-                interpolate_radial_functions(array,
-                                             disc_indices,
-                                             slice_positions,
-                                             vr,
-                                             r,
-                                             dvdr,
-                                             sampling)
-            a = b
-
-            yield i, i + 1, PotentialArray(array[None] / kappa,
-                                           np.array([self.get_slice_thickness(i)]),
-                                           extent=self.extent)
-
-    def generate_frozen_phonon_potentials(self, pbar: Union[ProgressBar, bool] = True):
-        """
-        Function to generate scattering potentials for a set of frozen phonon configurations.
-
-        Parameters
-        ----------
-        pbar: bool, optional
-            Display a progress bar. Default is True.
-
-        Returns
-        -------
-        generator
-            Generator of potentials.
-        """
-
-        if isinstance(pbar, bool):
-            pbar = ProgressBar(total=len(self), desc='Potential', disable=(not pbar) or (not self._precalculate))
-
-        for atoms in self.frozen_phonons:
-            self.atoms.positions[:] = atoms.positions
-            self.atoms.wrap()
-            pbar.reset()
-            
-            if self._precalculate:
-                yield self.build(pbar=pbar)
-            else:
-                yield self
-
-        pbar.refresh()
-        pbar.close()
-
-    def __copy__(self):
-        return self.__class__(atoms=self.frozen_phonons.copy(),
-                              gpts=self.gpts,
-                              slice_thickness=self.slice_thickness,
-                              parametrization=self.parametrization,
-                              cutoff_tolerance=self.cutoff_tolerance,
-                              device=self.device,
-                              storage=self._storage)
-
-
-class PotentialArray(AbstractPotential, HasGridMixin):
-    """
-    Potential array object
-
-    The potential array represents slices of the electrostatic potential as an array.
-
-    Parameters
-    ----------
-    array: 3D array
-        The array representing the potential slices. The first dimension is the slice index and the last two are the
-        spatial dimensions.
-    slice_thicknesses: float
-        The thicknesses of potential slices in Å. If a float, the thickness is the same for all slices.
-        If a sequence, the length must equal the length of the potential array.
-    extent: one or two float, optional
-        Lateral extent of the potential [Å].
-    sampling: one or two float, optional
-        Lateral sampling of the potential [1 / Å].
-    """
-
-    def __init__(self,
-                 array: np.ndarray,
-                 slice_thicknesses: Union[float, Sequence[float]],
-                 extent: Union[float, Sequence[float]] = None,
-                 sampling: Union[float, Sequence[float]] = None):
-
-        if (len(array.shape) != 2) & (len(array.shape) != 3):
-            raise RuntimeError()
-
-        slice_thicknesses = np.array(slice_thicknesses)
-
-        if slice_thicknesses.shape == ():
-            slice_thicknesses = np.tile(slice_thicknesses, array.shape[0])
-        elif (slice_thicknesses.shape != (array.shape[0],)) & (len(array.shape) == 3):
-            raise ValueError()
-
-        self._array = array
-        self._slice_thicknesses = slice_thicknesses
-        self._grid = Grid(extent=extent, gpts=self.array.shape[-2:], sampling=sampling, lock_gpts=True)
-
-    def as_transmission_function(self, energy, in_place=True, max_batch=1, antialias_filter=None):
-        """
-        Calculate the transmission functions for a specific energy.
-
-        Parameters
-        ----------
-        energy: float
-            Electron energy [eV].
-
-        Returns
-        -------
-        TransmissionFunctions object
-        """
-
-        xp = get_array_module(self.array)
-        complex_exponential = get_device_function(xp, 'complex_exponential')
-
-        array = self._array
-        if not in_place:
-            array = array.copy()
-
-        array = complex_exponential(energy2sigma(energy) * array)
-
-        t = TransmissionFunction(array,
-                                 slice_thicknesses=self._slice_thicknesses.copy(),
-                                 extent=self.extent,
-                                 energy=energy)
-
-        if antialias_filter is None:
-            antialias_filter = AntialiasFilter()
-
-        for start, end, potential_slices in t.generate_slices(max_batch=max_batch):
-            antialias_filter.bandlimit(potential_slices)
-
-        return t
-
-    @property
-    def array(self):
-        """The potential array."""
-        return self._array
-
-    @property
-    def num_slices(self):
-        return self._array.shape[0]
-
-    def get_slice_thickness(self, i):
-        return self._slice_thicknesses[i]
-
-    @property
-    def slice_thicknesses(self):
-        return self._slice_thicknesses
-
-    @property
-    def thickness(self):
-        return np.sum(self._slice_thicknesses)
-
-    def generate_slices(self, first_slice=0, last_slice=None, max_batch=1):
-        if last_slice is None:
-            last_slice = len(self)
-
-        for start, end in generate_batches(last_slice - first_slice, max_batch=max_batch, start=first_slice):
-            slice_thicknesses = np.array([self.get_slice_thickness(i) for i in range(start, end)])
-            yield start, end, self.__class__(self.array[start:end],
-                                             slice_thicknesses=slice_thicknesses,
-                                             extent=self.extent)
-
-    def tile(self, multiples):
-        """
-        Tile the potential.
-
-        Parameters
-        ----------
-        multiples: two int
-            The number of repetitions of the potential along each axis.
-
-        Returns
-        -------
-        PotentialArray object
-            The tiled potential.
-        """
-
-        assert len(multiples) == 2
-        new_array = np.tile(self.array, (1,) + multiples)
-        new_extent = (self.extent[0] * multiples[0], self.extent[1] * multiples[1])
-        return self.__class__(array=new_array, slice_thicknesses=self._slice_thicknesses, extent=new_extent)
-
-    def write(self, path):
-        with h5py.File(path, 'w') as f:
-            f.create_dataset('array', data=self.array)
-            f.create_dataset('slice_thicknesses', data=self._slice_thicknesses)
-            f.create_dataset('extent', data=self.extent)
-
-    @classmethod
-    def read(cls, path):
-        with h5py.File(path, 'r') as f:
-            datasets = {}
-            for key in f.keys():
-                datasets[key] = f.get(key)[()]
-
-        return cls(array=datasets['array'], slice_thicknesses=datasets['slice_thicknesses'], extent=datasets['extent'])
-
-    def transmit(self, waves):
-        return self.as_transmission_function(waves.energy).transmit(waves)
-
-    def project(self):
-        calibrations = calibrations_from_grid(self.grid.gpts, self.grid.sampling, names=['x', 'y'])
-        array = asnumpy(self.array.sum(0))
-        array -= array.min()
-        return Measurement(array, calibrations)
-
-    def __copy___(self):
-        return self.__class__(array=self.array.copy(),
-                              slice_thicknesses=self._slice_thicknesses.copy(),
-                              extent=self.extent)
-
-
-class TransmissionFunction(PotentialArray, HasAcceleratorMixin):
-    """Class to describe transmission functions."""
-
-    def __init__(self,
-                 array: np.ndarray,
-                 slice_thicknesses: Union[float, Sequence[float]],
-                 extent: Union[float, Sequence[float]] = None,
-                 sampling: Union[float, Sequence[float]] = None,
-                 energy: float = None):
-        self._accelerator = Accelerator(energy=energy)
-        super().__init__(array, slice_thicknesses, extent, sampling)
-
-    def as_transmission_function(self, energy, in_place=True, max_batch=1, antialias_filter=None):
-        if energy != self.energy:
-            raise RuntimeError()
-
-        return self
-
-    def generate_transmission_functions(self, energy, first_slice=0, last_slice=None, max_batch=1):
-        if energy != self.energy:
-            raise RuntimeError()
-        return self.generate_slices(first_slice=first_slice, last_slice=last_slice, max_batch=max_batch)
-
-    def transmit(self, waves):
-        self.accelerator.check_match(waves)
-        xp = get_array_module(waves._array)
-
-        # if len(self.array.shape) == 2:
-        #    waves._array *= copy_to_device(self.array[None], xp)
-        # else:
-        waves._array *= copy_to_device(self.array, xp)
-        return waves
+"""Module to calculate potentials using the independent atom model."""
+from abc import ABCMeta, abstractmethod
+from copy import copy
+from typing import Union, Sequence, Callable, Generator
+
+import h5py
+import numpy as np
+from ase import Atoms
+from ase import units
+from scipy.optimize import brentq
+
+from abtem.base_classes import Grid, HasGridMixin, Cache, cached_method, HasAcceleratorMixin, Accelerator, Event, \
+    watched_property, AntialiasFilter
+from abtem.device import get_device_function, get_array_module, get_array_module_from_device, copy_to_device, \
+    HasDeviceMixin, asnumpy, get_available_memory
+from abtem.measure import calibrations_from_grid, Measurement
+from abtem.parametrizations import kirkland, dvdr_kirkland, load_kirkland_parameters, kirkland_projected_fourier
+from abtem.parametrizations import lobato, dvdr_lobato, load_lobato_parameters
+from abtem.structures import is_cell_orthogonal
+from abtem.tanh_sinh import integrate, tanh_sinh_nodes_and_weights
+from abtem.temperature import AbstractFrozenPhonons, DummyFrozenPhonons
+from abtem.utils import energy2sigma, ProgressBar, generate_batches, _disc_meshgrid
+
+# Vacuum permitivity in ASE units
+eps0 = units._eps0 * units.A ** 2 * units.s ** 4 / (units.kg * units.m ** 3)
+
+# Conversion factor from unitless potential parametrizations to ASE potential units
+kappa = 4 * np.pi * eps0 / (2 * np.pi * units.Bohr * units._e * units.C)
+
+
+class AbstractPotential(HasGridMixin, metaclass=ABCMeta):
+    """
+    Potential abstract base class
+
+    Base class common for all potentials.
+    """
+
+    def __len__(self):
+        return self.num_slices
+
+    @property
+    @abstractmethod
+    def num_slices(self):
+        """The number of projected potential slices."""
+        pass
+
+    def check_slice_idx(self, i):
+        """Raises an error if i is greater than the number of slices."""
+        if i >= self.num_slices:
+            raise RuntimeError('Slice index {} too large for potential with {} slices'.format(i, self.num_slices))
+
+    def generate_transmission_functions(self, energy, first_slice=0, last_slice=None, max_batch=1):
+        """
+        Generate the transmission functions one slice at a time.
+
+        Parameters
+        ----------
+        energy: float
+            Electron energy [eV].
+        first_slice: int
+            First potential slice to generate.
+        last_slice: int, optional
+            Last potential slice generate.
+        max_batch: int
+            Maximum number of potential slices calculated in parallel.
+
+        Returns
+        -------
+        generator of PotentialArray objects
+        """
+        antialias_filter = AntialiasFilter()
+
+        for start, end, potential_slice in self.generate_slices(first_slice, last_slice, max_batch=max_batch):
+            yield start, end, potential_slice.as_transmission_function(energy,
+                                                                       in_place=True,
+                                                                       max_batch=max_batch,
+                                                                       antialias_filter=antialias_filter)
+
+    @abstractmethod
+    def generate_slices(self, first_slice=0, last_slice=None, max_batch=1):
+        """
+        Generate the potential slices.
+
+        Parameters
+        ----------
+        first_slice: int
+            First potential slice to generate.
+        last_slice: int, optional
+            Last potential slice generate.
+        max_batch: int
+            Maximum number of potential slices calculated in parallel.
+
+        Returns
+        -------
+        generator of PotentialArray objects
+        """
+
+        pass
+
+    @abstractmethod
+    def get_slice_thickness(self, i):
+        """
+        Get the slice thickness [Å].
+
+        Parameters
+        ----------
+        i: int
+            Slice index.
+        """
+
+        pass
+
+    def __iter__(self):
+        for _, __, p in self.generate_slices(max_batch=1):
+            yield p
+
+    # def show(self, **kwargs):
+    #     """
+    #     Show the potential projection. This requires building all potential slices.
+    #
+    #     Parameters
+    #     ----------
+    #     kwargs:
+    #         Additional keyword arguments for abtem.plot.show_image.
+    #     """
+    #
+    #     self[:].show(**kwargs)
+
+    def copy(self):
+        """Make a copy."""
+        return copy(self)
+
+
+class AbstractPotentialBuilder(AbstractPotential):
+    """Potential builder abstract class."""
+
+    def __init__(self, precalculate=True, device='cpu', storage='cpu'):
+        self._precalculate = precalculate
+        self._storage = storage
+        self._device = device
+
+    def _estimate_max_batch(self):
+        memory_per_wave = 2 * 4 * self.gpts[0] * self.gpts[1]
+        available_memory = .2 * get_available_memory(self._device)
+        return min(int(available_memory / memory_per_wave), len(self))
+
+    def __getitem__(self, items):
+        if isinstance(items, int):
+            if items >= self.num_slices:
+                raise StopIteration
+            return next(self.generate_slices(items, items + 1, max_batch=1))[2]
+
+        elif isinstance(items, slice):
+            if items.start is None:
+                first_slice = 0
+            else:
+                first_slice = items.start
+
+            if items.stop is None:
+                last_slice = len(self)
+            else:
+                last_slice = items.stop
+
+            if items.step is None:
+                step = 1
+            else:
+                step = items.step
+
+            return self.build(first_slice, last_slice, pbar=False)[::step]
+        else:
+            raise TypeError('Potential must indexed with integers or slices, not {}'.format(type(items)))
+
+    def build(self,
+              first_slice: int = 0,
+              last_slice: int = None,
+              energy: float = None,
+              max_batch: int = None,
+              pbar: Union[bool, ProgressBar] = False,
+              ) -> 'PotentialArray':
+        """
+        Precalcaulate the potential as a potential array.
+
+        Parameters
+        ----------
+        first_slice: int
+            First potential slice to generate.
+        last_slice: int, optional
+            Last potential slice generate.
+        energy: float
+            Electron energy [eV]. If given, the transmission functions will be returned.
+        max_batch: int
+            Maximum number of potential slices calculated in parallel.
+        pbar: bool
+            If true, show progress bar.
+
+        Returns
+        -------
+        PotentialArray object
+        """
+
+        self.grid.check_is_defined()
+
+        if last_slice is None:
+            last_slice = len(self)
+
+        if max_batch is None:
+            max_batch = self._estimate_max_batch()
+
+        storage_xp = get_array_module_from_device(self._storage)
+
+        if energy is None:
+            array = storage_xp.zeros((last_slice - first_slice,) + (self.gpts[0], self.gpts[1]), dtype=np.float32)
+            generator = self.generate_slices(max_batch=max_batch, first_slice=first_slice, last_slice=last_slice)
+        else:
+            array = storage_xp.zeros((last_slice - first_slice,) + (self.gpts[0], self.gpts[1]), dtype=np.complex64)
+            generator = self.generate_transmission_functions(energy=energy,
+                                                             max_batch=max_batch,
+                                                             first_slice=first_slice,
+                                                             last_slice=last_slice)
+
+        slice_thicknesses = np.zeros(last_slice - first_slice)
+
+        if isinstance(pbar, bool):
+            pbar = ProgressBar(total=len(self), desc='Potential', disable=not pbar)
+            close_pbar = True
+        else:
+            close_pbar = False
+
+        pbar.reset()
+        for start, end, potential_slice in generator:
+            array[start:end] = copy_to_device(potential_slice.array, self._storage)
+            slice_thicknesses[start:end] = potential_slice.slice_thicknesses
+            pbar.update(end - start)
+
+        pbar.refresh()
+
+        if close_pbar:
+            pbar.close()
+
+        if energy is None:
+            return PotentialArray(array, slice_thicknesses=slice_thicknesses, extent=self.extent)
+        else:
+            return TransmissionFunction(array, slice_thicknesses=slice_thicknesses, extent=self.extent, energy=energy)
+
+    def project(self):
+        return self.build().project()
+
+
+class AbstractTDSPotentialBuilder(AbstractPotentialBuilder):
+    """Thermal diffuse scattering builder abstract class."""
+
+    def __init__(self, precalculate=True, storage='cpu'):
+        super().__init__(precalculate=precalculate, storage=storage)
+
+    @property
+    @abstractmethod
+    def frozen_phonons(self):
+        pass
+
+    @abstractmethod
+    def generate_frozen_phonon_potentials(self, pbar):
+        pass
+
+
+class PotentialIntegrator:
+    """
+    Perform finite integrals of a radial function along a straight line.
+
+    Parameters
+    ----------
+    function: callable
+        Radial function to integrate.
+    r: array of float
+        The evaluation points of the integrals.
+    cutoff: float, optional
+        The radial function is assumed to be zero outside this threshold.
+    cache_size: int, optional
+        The maximum number of integrals that will be cached.
+    cache_key_decimals: int, optional
+        The number of decimals used in the cache keys.
+    tolerance: float, optional
+        The absolute error tolerance of the integrals.
+    """
+
+    def __init__(self,
+                 function: Callable,
+                 r: np.ndarray,
+                 max_interval,
+                 cutoff: float = None,
+                 cache_size: int = 4096,
+                 cache_key_decimals: int = 2,
+                 tolerance: float = 1e-6):
+
+        self._function = function
+        self._r = r
+
+        if cutoff is None:
+            self._cutoff = r[-1]
+        else:
+            self._cutoff = cutoff
+
+        self._cache = Cache(cache_size)
+        self._cache_key_decimals = cache_key_decimals
+        self._tolerance = tolerance
+
+        def f(z):
+            return self._function(np.sqrt(self.r[0] ** 2 + (z * max_interval / 2 + max_interval / 2) ** 2))
+
+        value, error_estimate, step_size, order = integrate(f, -1, 1, self._tolerance)
+        step_size = step_size
+        order = order
+
+        self._xk, self._wk = tanh_sinh_nodes_and_weights(step_size, order)
+
+    @property
+    def r(self):
+        return self._r
+
+    @property
+    def cutoff(self):
+        return self._cutoff
+
+    def integrate(self, z, a: float, b: float, xp):
+        """
+        Evaulate the integrals of the radial function at the evaluation points.
+
+        Parameters
+        ----------
+        a: float
+            Lower limit of integrals.
+        b: float
+            Upper limit of integrals.
+
+        Returns
+        -------
+        1d array
+            The evaulated integrals.
+        """
+
+        vr = np.zeros((len(z), self.r.shape[0]), np.float32)
+        dvdr = np.zeros((len(z), self.r.shape[0]), np.float32)
+        a = np.round(a - z, self._cache_key_decimals)
+        b = np.round(b - z, self._cache_key_decimals)
+
+        split = a * b < 0
+
+        a, b = np.abs(a), np.abs(b)
+        a, b = np.minimum(a, b), np.minimum(np.maximum(a, b), self.cutoff)
+
+        for i, (ai, bi) in enumerate(zip(a, b)):
+            if split[i]:  # split the integral
+                values1, derivatives1 = self._do_integrate(0, ai)
+                values2, derivatives2 = self._do_integrate(0, bi)
+                result = (values1 + values2, derivatives1 + derivatives2)
+            else:
+                result = self._do_integrate(ai, bi)
+
+            vr[i] = result[0]
+            dvdr[i, :-1] = result[1]
+
+        return vr, dvdr
+
+    @cached_method('_cache')
+    def _do_integrate(self, a, b):
+        zm = (b - a) / 2.
+        zp = (a + b) / 2.
+
+        def f(z):
+            return self._function(np.sqrt(self.r[:, None] ** 2 + (z * zm + zp) ** 2))
+
+        values = np.sum(f(self._xk[None]) * self._wk[None], axis=1) * zm
+        derivatives = np.diff(values) / np.diff(self.r)
+
+        return values, derivatives
+
+
+def pad_atoms(atoms: Atoms, margin: float):
+    """
+    Repeat the atoms in x and y, retaining only the repeated atoms within the margin distance from the cell boundary.
+
+    Parameters
+    ----------
+    atoms: ASE Atoms object
+        The atoms that should be padded.
+    margin: float
+        The padding margin.
+
+    Returns
+    -------
+    ASE Atoms object
+        Padded atoms.
+    """
+
+    if not is_cell_orthogonal(atoms):
+        raise RuntimeError('The cell of the atoms must be orthogonal.')
+
+    left = atoms[atoms.positions[:, 0] < margin]
+    left.positions[:, 0] += atoms.cell[0, 0]
+    right = atoms[atoms.positions[:, 0] > atoms.cell[0, 0] - margin]
+    right.positions[:, 0] -= atoms.cell[0, 0]
+
+    atoms += left + right
+
+    top = atoms[atoms.positions[:, 1] < margin]
+    top.positions[:, 1] += atoms.cell[1, 1]
+    bottom = atoms[atoms.positions[:, 1] > atoms.cell[1, 1] - margin]
+    bottom.positions[:, 1] -= atoms.cell[1, 1]
+    atoms += top + bottom
+    return atoms
+
+
+def superpose_deltas(positions, z, array):
+    shape = array.shape[-2:]
+    xp = get_array_module(array)
+    rounded = xp.floor(positions).astype(xp.int32)
+    rows, cols = rounded[:, 0], rounded[:, 1]
+
+    array[z, rows, cols] += (1 - (positions[:, 0] - rows)) * (1 - (positions[:, 1] - cols))
+    array[z, (rows + 1) % shape[0], cols] += (positions[:, 0] - rows) * (1 - (positions[:, 1] - cols))
+    array[z, rows, (cols + 1) % shape[1]] += (1 - (positions[:, 0] - rows)) * (positions[:, 1] - cols)
+    array[z, (rows + 1) % shape[0], (cols + 1) % shape[1]] += (rows - positions[:, 0]) * (cols - positions[:, 1])
+
+
+class Potential(AbstractTDSPotentialBuilder, HasDeviceMixin):
+    """
+    Potential object.
+
+    The potential object is used to calculate the electrostatic potential of a set of atoms represented by an ASE atoms
+    object. The potential is calculated with the Independent Atom Model (IAM) using a user-defined parametrization
+    of the atomic potentials.
+
+    Parameters
+    ----------
+    atoms: Atoms or FrozenPhonons object
+        Atoms or FrozenPhonons defining the atomic configuration(s) used in the IAM of the electrostatic potential(s).
+    gpts: one or two int, optional
+        Number of grid points describing each slice of the potential.
+    sampling: one or two float, optional
+        Lateral sampling of the potential [1 / Å].
+    slice_thickness: float, optional
+        Thickness of the potential slices in Å for calculating the number of slices used by the multislice algorithm.
+        Default is 0.5 Å.
+    parametrization: 'lobato' or 'kirkland', optional
+        The potential parametrization describes the radial dependence of the potential for each element. Two of the
+        most accurate parametrizations are available by Lobato et. al. and Kirkland. The abTEM default is 'lobato'.
+        See the citation guide for references.
+    projection: 'finite' or 'infinite'
+        If 'finite' the 3d potential is numerically integrated between the slice boundaries. If 'infinite' the infinite
+        potential projection of each atom will be assigned to a single slice.
+    cutoff_tolerance: float, optional
+        The error tolerance used for deciding the radial cutoff distance of the potential [eV / e]. The cutoff is only
+        relevant for potentials using the 'finite' projection scheme.
+    device: str, optional
+        The device used for calculating the potential. The default is 'cpu'.
+    storage: str, optional
+        The device on which to store the created potential. The default is 'None', defaulting to the chosen device.
+    """
+
+    def __init__(self,
+                 atoms: Union[Atoms, AbstractFrozenPhonons] = None,
+                 gpts: Union[int, Sequence[int]] = None,
+                 sampling: Union[float, Sequence[float]] = None,
+                 slice_thickness: float = .5,
+                 parametrization: str = 'lobato',
+                 projection: str = 'finite',
+                 cutoff_tolerance: float = 1e-3,
+                 device='cpu',
+                 precalculate=True,
+                 storage=None):
+
+        self._cutoff_tolerance = cutoff_tolerance
+        self._parametrization = parametrization
+        self._slice_thickness = slice_thickness
+
+        self._storage = storage
+
+        if parametrization.lower() == 'lobato':
+            self._parameters = load_lobato_parameters()
+            self._function = lobato
+            self._derivative = dvdr_lobato
+
+        elif parametrization.lower() == 'kirkland':
+            self._parameters = load_kirkland_parameters()
+            self._function = kirkland
+            self._derivative = dvdr_kirkland
+        else:
+            raise RuntimeError('Parametrization {} not recognized'.format(parametrization))
+
+        if projection == 'infinite':
+            if parametrization.lower() != 'kirkland':
+                raise RuntimeError('Infinite projections are only implemented for the Kirkland parametrization')
+        elif (projection != 'finite'):
+            raise RuntimeError('Projection must be "finite" or "infinite"')
+
+        self._projection = projection
+
+        if isinstance(atoms, AbstractFrozenPhonons):
+            self._frozen_phonons = atoms
+        else:
+            self._frozen_phonons = DummyFrozenPhonons(atoms)
+
+        atoms = next(iter(self._frozen_phonons))
+
+        if np.abs(atoms.cell[2, 2]) < 1e-12:
+            raise RuntimeError('Atoms cell has no thickness')
+
+        if not is_cell_orthogonal(atoms):
+            raise RuntimeError('Atoms are not orthogonal')
+
+        self._atoms = atoms
+        self._grid = Grid(extent=np.diag(atoms.cell)[:2], gpts=gpts, sampling=sampling, lock_extent=True)
+
+        self._cutoffs = {}
+        self._integrators = {}
+        self._disc_indices = {}
+
+        def grid_changed_callback(*args, **kwargs):
+            self._integrators = {}
+            self._disc_indices = {}
+
+        self.grid.changed.register(grid_changed_callback)
+        self.changed = Event()
+
+        self._device = device
+
+        if storage is None:
+            storage = device
+
+        super().__init__(precalculate=precalculate, storage=storage)
+
+    @property
+    def parametrization(self):
+        """The potential parametrization."""
+        return self._parameters
+
+    @property
+    def projection(self):
+        """The projection method."""
+        return self._projection
+
+    @property
+    def parameters(self):
+        """The parameters of the potential parametrization."""
+        return self._parameters
+
+    @property
+    def function(self):
+        """The potential function of the parametrization."""
+        return self._function
+
+    @property
+    def atoms(self):
+        """Atoms object defining the atomic configuration."""
+        return self._atoms
+
+    @property
+    def frozen_phonons(self):
+        """FrozenPhonons object defining the atomic configuration(s)."""
+        return self._frozen_phonons
+
+    @property
+    def cutoff_tolerance(self):
+        """The error tolerance used for deciding the radial cutoff distance of the potential [eV / e]."""
+        return self._cutoff_tolerance
+
+    @property
+    def num_slices(self):
+        """The number of projected potential slices."""
+        return int(np.ceil(self._atoms.cell[2, 2] / self._slice_thickness))
+
+    @property
+    def slice_thickness(self):
+        """The thickness of the projected potential slices."""
+        return self._slice_thickness
+
+    @slice_thickness.setter
+    @watched_property('changed')
+    def slice_thickness(self, value):
+        self._slice_thickness = value
+
+    def get_slice_thickness(self, i):
+        return self._atoms.cell[2, 2] / self.num_slices
+
+    def get_cutoff(self, number: int) -> float:
+        """
+        Cutoff distance for atomic number given an error tolerance.
+
+        Parameters
+        ----------
+        number: int
+            Atomic number.
+
+        Returns
+        -------
+        cutoff: float
+            The potential cutoff.
+        """
+
+        try:
+            return self._cutoffs[number]
+        except KeyError:
+            def f(r):
+                return self.function(r, self.parameters[number]) - self.cutoff_tolerance
+
+            self._cutoffs[number] = brentq(f, 1e-7, 1000)
+            return self._cutoffs[number]
+
+    def get_tapered_function(self, number: int) -> Callable:
+        """
+        Tapered potential function for atomic number.
+
+        Parameters
+        ----------
+        number: int
+            Atomic number.
+
+        Returns
+        -------
+        callable
+        """
+
+        cutoff = self.get_cutoff(number)
+        rolloff = .85 * cutoff
+
+        def soft_function(r):
+            result = np.zeros_like(r)
+            valid = r < cutoff
+            transition = valid * (r > rolloff)
+            result[valid] = self._function(r[valid], self.parameters[number])
+            result[transition] *= (np.cos(np.pi * (r[transition] - rolloff) / (cutoff - rolloff)) + 1.) / 2
+            return result
+
+        return soft_function
+
+    def get_integrator(self, number: int) -> PotentialIntegrator:
+        """
+        Potential integrator for atomic number.
+
+        Parameters
+        ----------
+        number: int
+            Atomic number.
+
+        Returns
+        -------
+        PotentialIntegrator object
+        """
+
+        try:
+            return self._integrators[number]
+        except KeyError:
+            cutoff = self.get_cutoff(number)
+            soft_function = self.get_tapered_function(number)
+            inner_cutoff = np.min(self.sampling) / 2.
+            num_points = int(np.ceil(cutoff / np.min(self.sampling) * 2.))
+            r = np.geomspace(inner_cutoff, cutoff, num_points)
+            max_interval = self.slice_thickness
+            self._integrators[number] = PotentialIntegrator(soft_function, r, max_interval, cutoff)
+            return self._integrators[number]
+
+    def _get_radial_interpolation_points(self, number):
+        """Internal function for the indices of the radial interpolation points."""
+        try:
+            return self._disc_indices[number]
+        except KeyError:
+            cutoff = self.get_cutoff(number)
+            margin = np.int(np.ceil(cutoff / np.min(self.sampling)))
+            rows, cols = _disc_meshgrid(margin)
+            self._disc_indices[number] = np.hstack((rows[:, None], cols[:, None]))
+            return self._disc_indices[number]
+
+    def generate_slices(self, first_slice=0, last_slice=None, max_batch=1) -> Generator:
+        self.grid.check_is_defined()
+
+        if last_slice is None:
+            last_slice = len(self)
+
+        if self.projection == 'finite':
+            return self._generate_slices_finite(first_slice=first_slice, last_slice=last_slice, max_batch=max_batch)
+        else:
+            return self._generate_slices_infinite(first_slice=first_slice, last_slice=last_slice, max_batch=max_batch)
+
+    def _generate_slices_infinite(self, first_slice=0, last_slice=None, max_batch=1) -> Generator:
+        xp = get_array_module_from_device(self._device)
+        fft2_convolve = get_device_function(xp, 'fft2_convolve')
+
+        atoms = self.atoms.copy()
+        atoms.wrap()
+        indices_by_number = {number: np.where(atoms.numbers == number)[0] for number in np.unique(atoms.numbers)}
+
+        kx = xp.fft.fftfreq(self.gpts[0], self.sampling[0])
+        ky = xp.fft.fftfreq(self.gpts[1], self.sampling[1])
+        kx, ky = xp.meshgrid(kx, ky, indexing='ij')
+        k = xp.sqrt(kx ** 2 + ky ** 2)
+
+        sinc = xp.sinc(xp.sqrt((kx * self.sampling[0]) ** 2 + (kx * self.sampling[1]) ** 2))
+
+        scattering_factors = {}
+        for atomic_number in indices_by_number.keys():
+            f = kirkland_projected_fourier(k, self.parameters[atomic_number])
+            scattering_factors[atomic_number] = (f / (sinc * self.sampling[0] * self.sampling[1] * kappa)).astype(
+                xp.complex64)
+
+        slice_idx = np.floor(atoms.positions[:, 2] / atoms.cell[2, 2] * self.num_slices).astype(np.int)
+
+        start, end = next(generate_batches(last_slice - first_slice, max_batch=max_batch, start=first_slice))
+        array = xp.zeros((end - start, len(indices_by_number),) + self.gpts, dtype=xp.complex64)
+
+        for start, end in generate_batches(last_slice - first_slice, max_batch=max_batch, start=first_slice):
+            array[:] = 0.
+
+            for j, (number, indices) in enumerate(indices_by_number.items()):
+                in_slice = (slice_idx >= start) * (slice_idx < end) * (atoms.numbers == number)
+                slice_atoms = atoms[in_slice]
+
+                positions = xp.asarray(slice_atoms.positions[:, :2] / self.sampling)
+
+                superpose_deltas(positions, slice_idx[in_slice] - start, array[:, j])
+
+                fft2_convolve(array[:, j], scattering_factors[number])
+
+            slice_thicknesses = [self.get_slice_thickness(i) for i in range(start, end)]
+            yield start, end, PotentialArray(array.real.sum(1)[:end - start], slice_thicknesses, extent=self.extent)
+
+    def _generate_slices_finite(self, first_slice=0, last_slice=None, max_batch=1) -> Generator:
+        xp = get_array_module_from_device(self._device)
+
+        interpolate_radial_functions = get_device_function(xp, 'interpolate_radial_functions')
+
+        atoms = self.atoms.copy()
+        atoms.wrap()
+        indices_by_number = {number: np.where(atoms.numbers == number)[0] for number in np.unique(atoms.numbers)}
+
+        start, end = next(generate_batches(last_slice - first_slice, max_batch=max_batch, start=first_slice))
+        array = xp.zeros((end - start,) + self.gpts, dtype=xp.float32)
+
+        slice_edges = np.linspace(0, self.atoms.cell[2, 2], self.num_slices + 1)
+
+        for start, end in generate_batches(last_slice - first_slice, max_batch=max_batch, start=first_slice):
+            array[:] = 0.
+
+            for number, indices in indices_by_number.items():
+                species_atoms = atoms[indices]
+                integrator = self.get_integrator(number)
+                disc_indices = xp.asarray(self._get_radial_interpolation_points(number))
+
+                a = slice_edges[start]
+                b = slice_edges[end]
+                chunk_atoms = species_atoms[(species_atoms.positions[:, 2] > a - integrator.cutoff) *
+                                            (species_atoms.positions[:, 2] < b + integrator.cutoff)]
+                chunk_atoms = pad_atoms(chunk_atoms, integrator.cutoff)
+                chunk_positions = chunk_atoms.positions
+
+                if len(chunk_atoms) == 0:
+                    continue
+
+                positions = np.zeros((0, 3), dtype=xp.float32)
+                A = np.zeros((0,), dtype=xp.float32)
+                B = np.zeros((0,), dtype=xp.float32)
+                run_length_enconding = np.zeros((end - start + 1,), dtype=xp.int32)
+                # print(end, start)
+                for i, j in enumerate(range(start, end)):
+                    a = slice_edges[j]
+                    b = slice_edges[j + 1]
+                    slice_positions = chunk_positions[(chunk_positions[:, 2] > a - integrator.cutoff) *
+                                                      (chunk_positions[:, 2] < b + integrator.cutoff)]
+
+                    # if len(slice_positions) == 0:
+                    #    continue
+
+                    positions = np.vstack((positions, slice_positions))
+                    A = np.concatenate((A, [a] * len(slice_positions)))
+                    B = np.concatenate((B, [b] * len(slice_positions)))
+
+                    run_length_enconding[i + 1] = run_length_enconding[i] + len(slice_positions)
+                    # print(i)
+
+                # print(run_length_enconding, end, start)
+                # sss
+                vr, dvdr = integrator.integrate(positions[:, 2], A, B, xp=xp)
+
+                vr = xp.asarray(vr, dtype=xp.float32)
+                dvdr = xp.asarray(dvdr, dtype=xp.float32)
+                r = xp.asarray(integrator.r, dtype=xp.float32)
+                sampling = xp.asarray(self.sampling, dtype=xp.float32)
+
+                interpolate_radial_functions(array,
+                                             run_length_enconding,
+                                             disc_indices,
+                                             positions,
+                                             vr,
+                                             r,
+                                             dvdr,
+                                             sampling)
+
+            slice_thicknesses = [self.get_slice_thickness(i) for i in range(start, end)]
+
+            yield start, end, PotentialArray(array[:end - start] / kappa,
+                                             slice_thicknesses,
+                                             extent=self.extent)
+
+    def generate_frozen_phonon_potentials(self, pbar: Union[ProgressBar, bool] = True):
+        """
+        Function to generate scattering potentials for a set of frozen phonon configurations.
+
+        Parameters
+        ----------
+        pbar: bool, optional
+            Display a progress bar. Default is True.
+
+        Returns
+        -------
+        generator
+            Generator of potentials.
+        """
+
+        if isinstance(pbar, bool):
+            pbar = ProgressBar(total=len(self), desc='Potential', disable=(not pbar) or (not self._precalculate))
+
+        for atoms in self.frozen_phonons:
+            self.atoms.positions[:] = atoms.positions
+            self.atoms.wrap()
+            pbar.reset()
+
+            if self._precalculate:
+                yield self.build(pbar=pbar)
+            else:
+                yield self
+
+        pbar.refresh()
+        pbar.close()
+
+    def __copy__(self):
+        return self.__class__(atoms=self.frozen_phonons.copy(),
+                              gpts=self.gpts,
+                              slice_thickness=self.slice_thickness,
+                              parametrization=self.parametrization,
+                              cutoff_tolerance=self.cutoff_tolerance,
+                              device=self.device,
+                              storage=self._storage)
+
+
+class PotentialArray(AbstractPotential, HasGridMixin):
+    """
+    Potential array object
+
+    The potential array represents slices of the electrostatic potential as an array.
+
+    Parameters
+    ----------
+    array: 3D array
+        The array representing the potential slices. The first dimension is the slice index and the last two are the
+        spatial dimensions.
+    slice_thicknesses: float
+        The thicknesses of potential slices in Å. If a float, the thickness is the same for all slices.
+        If a sequence, the length must equal the length of the potential array.
+    extent: one or two float, optional
+        Lateral extent of the potential [Å].
+    sampling: one or two float, optional
+        Lateral sampling of the potential [1 / Å].
+    """
+
+    def __init__(self,
+                 array: np.ndarray,
+                 slice_thicknesses: Union[float, Sequence[float]],
+                 extent: Union[float, Sequence[float]] = None,
+                 sampling: Union[float, Sequence[float]] = None):
+
+        if (len(array.shape) != 2) & (len(array.shape) != 3):
+            raise RuntimeError()
+
+        slice_thicknesses = np.array(slice_thicknesses)
+
+        if slice_thicknesses.shape == ():
+            slice_thicknesses = np.tile(slice_thicknesses, array.shape[0])
+        elif (slice_thicknesses.shape != (array.shape[0],)) & (len(array.shape) == 3):
+            raise ValueError()
+
+        self._array = array
+        self._slice_thicknesses = slice_thicknesses
+        self._grid = Grid(extent=extent, gpts=self.array.shape[-2:], sampling=sampling, lock_gpts=True)
+
+    def __getitem__(self, items):
+        return PotentialArray(self.array[items], self._slice_thicknesses[items], extent=self.extent)
+
+    def as_transmission_function(self, energy, in_place=True, max_batch=1, antialias_filter=None):
+        """
+        Calculate the transmission functions for a specific energy.
+
+        Parameters
+        ----------
+        energy: float
+            Electron energy [eV].
+
+        Returns
+        -------
+        TransmissionFunctions object
+        """
+
+        xp = get_array_module(self.array)
+        complex_exponential = get_device_function(xp, 'complex_exponential')
+
+        array = self._array
+        if not in_place:
+            array = array.copy()
+
+        array = complex_exponential(energy2sigma(energy) * array)
+
+        t = TransmissionFunction(array,
+                                 slice_thicknesses=self._slice_thicknesses.copy(),
+                                 extent=self.extent,
+                                 energy=energy)
+
+        if antialias_filter is None:
+            antialias_filter = AntialiasFilter()
+
+        for start, end, potential_slices in t.generate_slices(max_batch=max_batch):
+            antialias_filter.bandlimit(potential_slices)
+
+        return t
+
+    @property
+    def array(self):
+        """The potential array."""
+        return self._array
+
+    @property
+    def num_slices(self):
+        return self._array.shape[0]
+
+    def get_slice_thickness(self, i):
+        return self._slice_thicknesses[i]
+
+    @property
+    def slice_thicknesses(self):
+        return self._slice_thicknesses
+
+    @property
+    def thickness(self):
+        return np.sum(self._slice_thicknesses)
+
+    def generate_slices(self, first_slice=0, last_slice=None, max_batch=1):
+        if last_slice is None:
+            last_slice = len(self)
+
+        for start, end in generate_batches(last_slice - first_slice, max_batch=max_batch, start=first_slice):
+            slice_thicknesses = np.array([self.get_slice_thickness(i) for i in range(start, end)])
+            yield start, end, self.__class__(self.array[start:end],
+                                             slice_thicknesses=slice_thicknesses,
+                                             extent=self.extent)
+
+    def tile(self, multiples):
+        """
+        Tile the potential.
+
+        Parameters
+        ----------
+        multiples: two int
+            The number of repetitions of the potential along each axis.
+
+        Returns
+        -------
+        PotentialArray object
+            The tiled potential.
+        """
+
+        assert len(multiples) == 2
+        new_array = np.tile(self.array, (1,) + multiples)
+        new_extent = (self.extent[0] * multiples[0], self.extent[1] * multiples[1])
+        return self.__class__(array=new_array, slice_thicknesses=self._slice_thicknesses, extent=new_extent)
+
+    def write(self, path):
+        with h5py.File(path, 'w') as f:
+            f.create_dataset('array', data=self.array)
+            f.create_dataset('slice_thicknesses', data=self._slice_thicknesses)
+            f.create_dataset('extent', data=self.extent)
+
+    @classmethod
+    def read(cls, path):
+        with h5py.File(path, 'r') as f:
+            datasets = {}
+            for key in f.keys():
+                datasets[key] = f.get(key)[()]
+
+        return cls(array=datasets['array'], slice_thicknesses=datasets['slice_thicknesses'], extent=datasets['extent'])
+
+    def transmit(self, waves):
+        return self.as_transmission_function(waves.energy).transmit(waves)
+
+    def project(self):
+        calibrations = calibrations_from_grid(self.grid.gpts, self.grid.sampling, names=['x', 'y'])
+        array = asnumpy(self.array.sum(0))
+        array -= array.min()
+        return Measurement(array, calibrations)
+
+    def __copy___(self):
+        return self.__class__(array=self.array.copy(),
+                              slice_thicknesses=self._slice_thicknesses.copy(),
+                              extent=self.extent)
+
+
+class TransmissionFunction(PotentialArray, HasAcceleratorMixin):
+    """Class to describe transmission functions."""
+
+    def __init__(self,
+                 array: np.ndarray,
+                 slice_thicknesses: Union[float, Sequence[float]],
+                 extent: Union[float, Sequence[float]] = None,
+                 sampling: Union[float, Sequence[float]] = None,
+                 energy: float = None):
+        self._accelerator = Accelerator(energy=energy)
+        super().__init__(array, slice_thicknesses, extent, sampling)
+
+    def as_transmission_function(self, energy, in_place=True, max_batch=1, antialias_filter=None):
+        if energy != self.energy:
+            raise RuntimeError()
+
+        return self
+
+    def generate_transmission_functions(self, energy, first_slice=0, last_slice=None, max_batch=1):
+        if energy != self.energy:
+            raise RuntimeError()
+        return self.generate_slices(first_slice=first_slice, last_slice=last_slice, max_batch=max_batch)
+
+    def transmit(self, waves):
+        self.accelerator.check_match(waves)
+        xp = get_array_module(waves._array)
+        waves._array *= copy_to_device(self.array, xp)
+        return waves
```

### Comparing `abtem-1.0.0b8/abtem/structures.py` & `abtem-1.0.0b9/abtem/structures.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-"""Module for modifying ASE atoms objects for use in abTEM."""
-from fractions import Fraction
-
-import numpy as np
-from ase import Atoms
-from scipy.linalg import polar
-
-
-def is_cell_hexagonal(atoms: Atoms):
-    """
-    Function to check whether the cell of an ASE atoms object is hexagonal.
-    """
-    cell = atoms.get_cell()
-
-    a = np.linalg.norm(cell[0], axis=0)
-    b = np.linalg.norm(cell[1], axis=0)
-    c = np.linalg.norm(cell[2], axis=0)
-    angle = np.arccos(np.dot(cell[0], cell[1]) / (a * b))
-
-    return np.isclose(a, b) & (np.isclose(angle, np.pi / 3) | np.isclose(angle, 2 * np.pi / 3)) & (c == cell[2, 2])
-
-
-def is_cell_orthogonal(atoms: Atoms, tol: float = 1e-12):
-    """
-    Check whether an Atoms object has an orthogonal cell.
-    """
-    return not np.any(np.abs(atoms.cell[~np.eye(3, dtype=bool)]) > tol)
-
-
-def is_cell_valid(atoms: Atoms, tol: float = 1e-12) -> bool:
-    """
-    Check whether the cell of an ASE atoms object can be converted to a structure that is usable by abTEM.
-
-    Parameters
-    ----------
-    atoms: ASE atoms object
-        The atoms that should be checked.
-    tol: float
-        Components of the lattice vectors below this value are considered to be zero.
-
-    Returns
-    -------
-    bool
-        If true, the atomic structure is usable by abTEM.
-    """
-    if np.abs(atoms.cell[0, 0] - np.linalg.norm(atoms.cell[0])) > tol:
-        return False
-
-    if np.abs(atoms.cell[1, 2]) > tol:
-        return False
-
-    if np.abs(atoms.cell[2, 2] - np.linalg.norm(atoms.cell[2])) > tol:
-        return False
-
-    return True
-
-
-def standardize_cell(atoms: Atoms, tol: float = 1e-12):
-    """
-    Standardize the cell of an ASE atoms object. The atoms are rotated so one of the lattice vectors in the xy-plane
-    aligns with the x-axis, then all of the lattice vectors are made positive.
-
-    Parameters
-    ----------
-    atoms: ASE atoms object
-        The atoms that should be standardized
-    tol: float
-        Components of the lattice vectors below this value are considered to be zero.
-
-    Returns
-    -------
-    atoms: ASE atoms object
-        The standardized atoms.
-    """
-    cell = np.array(atoms.cell)
-
-    vertical_vector = np.where(np.all(np.abs(cell[:, :2]) < tol, axis=1))[0]
-
-    if len(vertical_vector) != 1:
-        raise RuntimeError('Invalid cell: no vertical lattice vector')
-
-    cell[[vertical_vector[0], 2]] = cell[[2, vertical_vector[0]]]
-    r = np.arctan2(atoms.cell[0, 1], atoms.cell[0, 0]) / np.pi * 180
-
-    atoms.set_cell(cell)
-
-    if r != 0.:
-        atoms.rotate(-r, 'z', rotate_cell=True)
-
-    if not is_cell_valid(atoms, tol):
-        raise RuntimeError('This cell cannot be made orthogonal using currently implemented methods.')
-
-    atoms.set_cell(np.abs(atoms.get_cell()))
-
-    atoms.wrap()
-    return atoms
-
-
-def orthogonalize_cell(atoms: Atoms, limit_denominator: int = 10, return_strain=False):
-    """
-    Make the cell of an ASE atoms object orthogonal. This is accomplished by repeating the cell until the x-component
-    of the lattice vectors in the xy-plane closely matches. If the ratio between the x-components is irrational this
-    may not be possible without introducing some strain. However, the amount of strain can be made arbitrarily small
-    by using many repetitions.
-
-    Parameters
-    ----------
-    atoms: ASE atoms object
-        The non-orthogonal atoms object.
-    limit_denominator: int
-        The maximum denominator in the rational approximation. Increase this to allow more repetitions and hence less
-        strain.
-    return_strain: bool
-        If true, return the strain tensor that were applied to make the atoms orthogonal.
-
-    Returns
-    -------
-    atoms: ASE atoms object
-        The orthogonal atoms.
-    strain_tensor: 2x2 array
-        The applied strain tensor. Only provided if return_strain is true.
-    """
-    if is_cell_orthogonal(atoms):
-        return atoms
-
-    atoms = atoms.copy()
-    atoms = standardize_cell(atoms)
-
-    fraction = atoms.cell[0, 0] / atoms.cell[1, 0]
-    fraction = Fraction(fraction).limit_denominator(limit_denominator)
-
-    atoms *= (fraction.denominator, fraction.numerator, 1)
-
-    new_cell = atoms.cell.copy()
-    new_cell[1, 0] = new_cell[0, 0]
-
-    a = np.linalg.solve(atoms.cell[:2, :2], new_cell[:2, :2])
-    _, strain_tensor = polar(a, side='left')
-    strain_tensor[0, 0] -= 1
-    strain_tensor[1, 1] -= 1
-
-    atoms.set_cell(new_cell, scale_atoms=True)
-    atoms.set_cell(np.diag(atoms.cell))
-    atoms.wrap()
-
-    if return_strain:
-        return atoms, strain_tensor
-    else:
-        return atoms
+"""Module for modifying ASE atoms objects for use in abTEM."""
+from fractions import Fraction
+
+import numpy as np
+from ase import Atoms
+from scipy.linalg import polar
+
+
+def is_cell_hexagonal(atoms: Atoms):
+    """
+    Function to check whether the cell of an ASE atoms object is hexagonal.
+    """
+    cell = atoms.get_cell()
+
+    a = np.linalg.norm(cell[0], axis=0)
+    b = np.linalg.norm(cell[1], axis=0)
+    c = np.linalg.norm(cell[2], axis=0)
+    angle = np.arccos(np.dot(cell[0], cell[1]) / (a * b))
+
+    return np.isclose(a, b) & (np.isclose(angle, np.pi / 3) | np.isclose(angle, 2 * np.pi / 3)) & (c == cell[2, 2])
+
+
+def is_cell_orthogonal(atoms: Atoms, tol: float = 1e-12):
+    """
+    Check whether an Atoms object has an orthogonal cell.
+    """
+    return not np.any(np.abs(atoms.cell[~np.eye(3, dtype=bool)]) > tol)
+
+
+def is_cell_valid(atoms: Atoms, tol: float = 1e-12) -> bool:
+    """
+    Check whether the cell of an ASE atoms object can be converted to a structure that is usable by abTEM.
+
+    Parameters
+    ----------
+    atoms: ASE atoms object
+        The atoms that should be checked.
+    tol: float
+        Components of the lattice vectors below this value are considered to be zero.
+
+    Returns
+    -------
+    bool
+        If true, the atomic structure is usable by abTEM.
+    """
+    if np.abs(atoms.cell[0, 0] - np.linalg.norm(atoms.cell[0])) > tol:
+        return False
+
+    if np.abs(atoms.cell[1, 2]) > tol:
+        return False
+
+    if np.abs(atoms.cell[2, 2] - np.linalg.norm(atoms.cell[2])) > tol:
+        return False
+
+    return True
+
+
+def standardize_cell(atoms: Atoms, tol: float = 1e-12):
+    """
+    Standardize the cell of an ASE atoms object. The atoms are rotated so one of the lattice vectors in the xy-plane
+    aligns with the x-axis, then all of the lattice vectors are made positive.
+
+    Parameters
+    ----------
+    atoms: ASE atoms object
+        The atoms that should be standardized
+    tol: float
+        Components of the lattice vectors below this value are considered to be zero.
+
+    Returns
+    -------
+    atoms: ASE atoms object
+        The standardized atoms.
+    """
+    cell = np.array(atoms.cell)
+
+    vertical_vector = np.where(np.all(np.abs(cell[:, :2]) < tol, axis=1))[0]
+
+    if len(vertical_vector) != 1:
+        raise RuntimeError('Invalid cell: no vertical lattice vector')
+
+    cell[[vertical_vector[0], 2]] = cell[[2, vertical_vector[0]]]
+    r = np.arctan2(atoms.cell[0, 1], atoms.cell[0, 0]) / np.pi * 180
+
+    atoms.set_cell(cell)
+
+    if r != 0.:
+        atoms.rotate(-r, 'z', rotate_cell=True)
+
+    if not is_cell_valid(atoms, tol):
+        raise RuntimeError('This cell cannot be made orthogonal using currently implemented methods.')
+
+    atoms.set_cell(np.abs(atoms.get_cell()))
+
+    atoms.wrap()
+    return atoms
+
+
+def orthogonalize_cell(atoms: Atoms, limit_denominator: int = 10, return_strain=False):
+    """
+    Make the cell of an ASE atoms object orthogonal. This is accomplished by repeating the cell until the x-component
+    of the lattice vectors in the xy-plane closely matches. If the ratio between the x-components is irrational this
+    may not be possible without introducing some strain. However, the amount of strain can be made arbitrarily small
+    by using many repetitions.
+
+    Parameters
+    ----------
+    atoms: ASE atoms object
+        The non-orthogonal atoms object.
+    limit_denominator: int
+        The maximum denominator in the rational approximation. Increase this to allow more repetitions and hence less
+        strain.
+    return_strain: bool
+        If true, return the strain tensor that were applied to make the atoms orthogonal.
+
+    Returns
+    -------
+    atoms: ASE atoms object
+        The orthogonal atoms.
+    strain_tensor: 2x2 array
+        The applied strain tensor. Only provided if return_strain is true.
+    """
+    if is_cell_orthogonal(atoms):
+        return atoms
+
+    atoms = atoms.copy()
+    atoms = standardize_cell(atoms)
+
+    fraction = atoms.cell[0, 0] / atoms.cell[1, 0]
+    fraction = Fraction(fraction).limit_denominator(limit_denominator)
+
+    atoms *= (fraction.denominator, fraction.numerator, 1)
+
+    new_cell = atoms.cell.copy()
+    new_cell[1, 0] = new_cell[0, 0]
+
+    a = np.linalg.solve(atoms.cell[:2, :2], new_cell[:2, :2])
+    _, strain_tensor = polar(a, side='left')
+    strain_tensor[0, 0] -= 1
+    strain_tensor[1, 1] -= 1
+
+    atoms.set_cell(new_cell, scale_atoms=True)
+    atoms.set_cell(np.diag(atoms.cell))
+    atoms.wrap()
+
+    if return_strain:
+        return atoms, strain_tensor
+    else:
+        return atoms
```

### Comparing `abtem-1.0.0b8/abtem/transfer.py` & `abtem-1.0.0b9/abtem/transfer.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,549 +1,565 @@
-"""Module to describe the contrast transfer function."""
-from collections import defaultdict
-from typing import Mapping, Union
-
-import numpy as np
-
-from abtem.base_classes import HasAcceleratorMixin, Accelerator, watched_method, watched_property, Event
-from abtem.device import get_array_module, get_device_function
-from abtem.measure import Measurement, Calibration
-from abtem.plot import PlotableMixin
-from abtem.utils import energy2wavelength
-
-#: Symbols for the polar representation of all optical aberrations up to the fifth order.
-polar_symbols = ('C10', 'C12', 'phi12',
-                 'C21', 'phi21', 'C23', 'phi23',
-                 'C30', 'C32', 'phi32', 'C34', 'phi34',
-                 'C41', 'phi41', 'C43', 'phi43', 'C45', 'phi45',
-                 'C50', 'C52', 'phi52', 'C54', 'phi54', 'C56', 'phi56')
-
-#: Aliases for the most commonly used optical aberrations.
-polar_aliases = {'defocus': 'C10', 'astigmatism': 'C12', 'astigmatism_angle': 'phi12',
-                 'coma': 'C21', 'coma_angle': 'phi21',
-                 'Cs': 'C30',
-                 'C5': 'C50'}
-
-
-class CTF(HasAcceleratorMixin, PlotableMixin):
-    """
-    Contrast transfer function object
-
-    The Contrast Transfer Function (CTF) describes the aberrations of the objective lens in HRTEM and specifies how the
-    condenser system shapes the probe in STEM.
-
-    abTEM implements phase aberrations up to 5th order using polar coefficients. See Eq. 2.22 in the reference [1]_.
-    Cartesian coefficients can be converted to polar using the utility function abtem.transfer.cartesian2polar.
-
-    Partial coherence is included as an envelope in the quasi-coherent approximation. See Chapter 3.2 in reference [1]_.
-
-    For a more detailed discussion with examples, see our `walkthrough
-    <https://abtem.readthedocs.io/en/latest/walkthrough/05_contrast_transfer_function.html>`_.
-
-    Parameters
-    ----------
-    semiangle_cutoff: float
-        The semiangle cutoff describes the sharp Fourier space cutoff due to the objective aperture [mrad].
-    rolloff: float
-        Softens the cutoff. A value of 0 gives a hard cutoff, while 1 gives the softest possible cutoff [Å].
-    focal_spread: float
-        The 1/e width of the focal spread due to chromatic aberration and lens current instability [Å].
-    angular_spread: float
-        The 1/e width of the angular deviations due to source size [Å].
-    gaussian_spread:
-        The 1/e width image deflections due to vibrations and thermal magnetic noise [Å].
-    energy: float
-        The electron energy of the wave functions this contrast transfer function will be applied to [eV].
-    parameters: dict
-        Mapping from aberration symbols to their corresponding values. All aberration magnitudes should be given in Å.
-    kwargs:
-        Provide the aberration coefficients as keyword arguments.
-
-    References
-    ----------
-    .. [1] Kirkland, E. J. (2010). Advanced Computing in Electron Microscopy (2nd ed.). Springer.
-
-    """
-
-    def __init__(self, semiangle_cutoff: float = np.inf, rolloff: float = 0.1, focal_spread: float = 0.,
-                 angular_spread: float = 0., gaussian_spread: float = 0., energy: float = None,
-                 parameters: Mapping[str, float] = None, **kwargs):
-
-        for key in kwargs.keys():
-            if (key not in polar_symbols) and (key not in polar_aliases.keys()):
-                raise ValueError('{} not a recognized parameter'.format(key))
-
-        self.changed = Event()
-
-        self._accelerator = Accelerator(energy=energy)
-        self._accelerator.changed.register(self.changed.notify)
-
-        self._semiangle_cutoff = semiangle_cutoff
-        self._rolloff = rolloff
-        self._focal_spread = focal_spread
-        self._angular_spread = angular_spread
-        self._gaussian_spread = gaussian_spread
-        self._parameters = dict(zip(polar_symbols, [0.] * len(polar_symbols)))
-
-        if parameters is None:
-            parameters = {}
-
-        parameters.update(kwargs)
-        self.set_parameters(parameters)
-
-        def parametrization_property(key):
-
-            def getter(self):
-                return self._parameters[key]
-
-            def setter(self, value):
-                old = getattr(self, key)
-                self._parameters[key] = value
-                self.changed.notify(**{'notifier': self, 'property_name': key, 'change': old != value})
-
-            return property(getter, setter)
-
-        for symbol in polar_symbols:
-            setattr(self.__class__, symbol, parametrization_property(symbol))
-
-        for key, value in polar_aliases.items():
-            if key != 'defocus':
-                setattr(self.__class__, key, parametrization_property(value))
-
-    @property
-    def nyquist_sampling(self):
-        return 1 / (4 * self.semiangle_cutoff / self.wavelength * 1e-3)
-
-    @property
-    def parameters(self):
-        """The parameters."""
-        return self._parameters
-
-    @property
-    def defocus(self) -> float:
-        """The defocus [Å]."""
-        return - self._parameters['C10']
-
-    @defocus.setter
-    def defocus(self, value: float):
-        self.C10 = -value
-
-    @property
-    def semiangle_cutoff(self) -> float:
-        """The semi-angle cutoff [mrad]."""
-        return self._semiangle_cutoff
-
-    @semiangle_cutoff.setter
-    @watched_property('changed')
-    def semiangle_cutoff(self, value: float):
-        self._semiangle_cutoff = value
-
-    @property
-    def rolloff(self) -> float:
-        """The fraction of soft tapering of the cutoff."""
-        return self._rolloff
-
-    @rolloff.setter
-    @watched_property('changed')
-    def rolloff(self, value: float):
-        self._rolloff = value
-
-    @property
-    def focal_spread(self) -> float:
-        """The focal spread [Å]."""
-        return self._focal_spread
-
-    @focal_spread.setter
-    @watched_property('changed')
-    def focal_spread(self, value: float):
-        """The angular spread [mrad]."""
-        self._focal_spread = value
-
-    @property
-    def angular_spread(self) -> float:
-        return self._angular_spread
-
-    @angular_spread.setter
-    @watched_property('changed')
-    def angular_spread(self, value: float):
-        self._angular_spread = value
-
-    @property
-    def gaussian_spread(self) -> float:
-        """The Gaussian spread [Å]."""
-        return self._gaussian_spread
-
-    @gaussian_spread.setter
-    @watched_property('changed')
-    def gaussian_spread(self, value: float):
-        self._gaussian_spread = value
-
-    @watched_method('changed')
-    def set_parameters(self, parameters: dict):
-        """
-        Set the phase of the phase aberration.
-
-        Parameters
-        ----------
-        parameters: dict
-            Mapping from aberration symbols to their corresponding values.
-        """
-
-        for symbol, value in parameters.items():
-            if symbol in self._parameters.keys():
-                self._parameters[symbol] = value
-
-            elif symbol == 'defocus':
-                self._parameters[polar_aliases[symbol]] = -value
-
-            elif symbol in polar_aliases.keys():
-                self._parameters[polar_aliases[symbol]] = value
-
-            else:
-                raise ValueError('{} not a recognized parameter'.format(symbol))
-
-        return parameters
-
-    def evaluate_aperture(self, alpha: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
-        xp = get_array_module(alpha)
-        semiangle_cutoff = self.semiangle_cutoff / 1000
-
-        if self.semiangle_cutoff == xp.inf:
-            return xp.ones_like(alpha)
-
-        if self.rolloff > 0.:
-            rolloff = self.rolloff * semiangle_cutoff
-            array = .5 * (1 + xp.cos(np.pi * (alpha - semiangle_cutoff + rolloff) / rolloff))
-            array[alpha > semiangle_cutoff] = 0.
-            array = xp.where(alpha > semiangle_cutoff - rolloff, array, xp.ones_like(alpha, dtype=xp.float32))
-        else:
-            array = xp.array(alpha < semiangle_cutoff).astype(xp.float32)
-        return array
-
-    def evaluate_temporal_envelope(self, alpha: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
-        xp = get_array_module(alpha)
-        return xp.exp(- (.5 * xp.pi / self.wavelength * self.focal_spread * alpha ** 2) ** 2).astype(xp.float32)
-
-    def evaluate_gaussian_envelope(self, alpha: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
-        xp = get_array_module(alpha)
-        return xp.exp(- .5 * self.gaussian_spread ** 2 * alpha ** 2 / self.wavelength ** 2)
-
-    def evaluate_spatial_envelope(self, alpha: Union[float, np.ndarray], phi: Union[float, np.ndarray]) -> \
-            Union[float, np.ndarray]:
-        xp = get_array_module(alpha)
-        p = self.parameters
-        dchi_dk = 2 * xp.pi / self.wavelength * (
-                (p['C12'] * xp.cos(2. * (phi - p['phi12'])) + p['C10']) * alpha +
-                (p['C23'] * xp.cos(3. * (phi - p['phi23'])) +
-                 p['C21'] * xp.cos(1. * (phi - p['phi21']))) * alpha ** 2 +
-                (p['C34'] * xp.cos(4. * (phi - p['phi34'])) +
-                 p['C32'] * xp.cos(2. * (phi - p['phi32'])) + p['C30']) * alpha ** 3 +
-                (p['C45'] * xp.cos(5. * (phi - p['phi45'])) +
-                 p['C43'] * xp.cos(3. * (phi - p['phi43'])) +
-                 p['C41'] * xp.cos(1. * (phi - p['phi41']))) * alpha ** 4 +
-                (p['C56'] * xp.cos(6. * (phi - p['phi56'])) +
-                 p['C54'] * xp.cos(4. * (phi - p['phi54'])) +
-                 p['C52'] * xp.cos(2. * (phi - p['phi52'])) + p['C50']) * alpha ** 5)
-
-        dchi_dphi = -2 * xp.pi / self.wavelength * (
-                1 / 2. * (2. * p['C12'] * xp.sin(2. * (phi - p['phi12']))) * alpha +
-                1 / 3. * (3. * p['C23'] * xp.sin(3. * (phi - p['phi23'])) +
-                          1. * p['C21'] * xp.sin(1. * (phi - p['phi21']))) * alpha ** 2 +
-                1 / 4. * (4. * p['C34'] * xp.sin(4. * (phi - p['phi34'])) +
-                          2. * p['C32'] * xp.sin(2. * (phi - p['phi32']))) * alpha ** 3 +
-                1 / 5. * (5. * p['C45'] * xp.sin(5. * (phi - p['phi45'])) +
-                          3. * p['C43'] * xp.sin(3. * (phi - p['phi43'])) +
-                          1. * p['C41'] * xp.sin(1. * (phi - p['phi41']))) * alpha ** 4 +
-                1 / 6. * (6. * p['C56'] * xp.sin(6. * (phi - p['phi56'])) +
-                          4. * p['C54'] * xp.sin(4. * (phi - p['phi54'])) +
-                          2. * p['C52'] * xp.sin(2. * (phi - p['phi52']))) * alpha ** 5)
-
-        return xp.exp(-xp.sign(self.angular_spread) * (self.angular_spread / 2 / 1000) ** 2 *
-                      (dchi_dk ** 2 + dchi_dphi ** 2))
-
-    def evaluate_chi(self, alpha: Union[float, np.ndarray], phi: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
-        xp = get_array_module(alpha)
-        p = self.parameters
-
-        alpha2 = alpha ** 2
-        alpha = xp.array(alpha)
-
-        array = xp.zeros(alpha.shape, dtype=np.float32)
-        if any([p[symbol] != 0. for symbol in ('C10', 'C12', 'phi12')]):
-            array += (1 / 2 * alpha2 *
-                      (p['C10'] +
-                       p['C12'] * xp.cos(2 * (phi - p['phi12']))))
-
-        if any([p[symbol] != 0. for symbol in ('C21', 'phi21', 'C23', 'phi23')]):
-            array += (1 / 3 * alpha2 * alpha *
-                      (p['C21'] * xp.cos(phi - p['phi21']) +
-                       p['C23'] * xp.cos(3 * (phi - p['phi23']))))
-
-        if any([p[symbol] != 0. for symbol in ('C30', 'C32', 'phi32', 'C34', 'phi34')]):
-            array += (1 / 4 * alpha2 ** 2 *
-                      (p['C30'] +
-                       p['C32'] * xp.cos(2 * (phi - p['phi32'])) +
-                       p['C34'] * xp.cos(4 * (phi - p['phi34']))))
-
-        if any([p[symbol] != 0. for symbol in ('C41', 'phi41', 'C43', 'phi43', 'C45', 'phi41')]):
-            array += (1 / 5 * alpha2 ** 2 * alpha *
-                      (p['C41'] * xp.cos((phi - p['phi41'])) +
-                       p['C43'] * xp.cos(3 * (phi - p['phi43'])) +
-                       p['C45'] * xp.cos(5 * (phi - p['phi45']))))
-
-        if any([p[symbol] != 0. for symbol in ('C50', 'C52', 'phi52', 'C54', 'phi54', 'C56', 'phi56')]):
-            array += (1 / 6 * alpha2 ** 3 *
-                      (p['C50'] +
-                       p['C52'] * xp.cos(2 * (phi - p['phi52'])) +
-                       p['C54'] * xp.cos(4 * (phi - p['phi54'])) +
-                       p['C56'] * xp.cos(6 * (phi - p['phi56']))))
-
-        array = 2 * xp.pi / self.wavelength * array
-        return array
-
-    def evaluate_aberrations(self, alpha: Union[float, np.ndarray], phi: Union[float, np.ndarray]) -> \
-            Union[float, np.ndarray]:
-        xp = get_array_module(alpha)
-        complex_exponential = get_device_function(xp, 'complex_exponential')
-        return complex_exponential(-self.evaluate_chi(alpha, phi))
-
-    def evaluate(self, alpha: Union[float, np.ndarray], phi: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
-        array = self.evaluate_aberrations(alpha, phi)
-
-        if self.semiangle_cutoff < np.inf:
-            array *= self.evaluate_aperture(alpha)
-
-        if self.focal_spread > 0.:
-            array *= self.evaluate_temporal_envelope(alpha)
-
-        if self.angular_spread > 0.:
-            array *= self.evaluate_spatial_envelope(alpha, phi)
-
-        if self.gaussian_spread > 0.:
-            array *= self.evaluate_gaussian_envelope(alpha)
-
-        return array
-
-    def profiles(self, max_semiangle: float = None, phi: float = 0.):
-        if max_semiangle is None:
-            if self._semiangle_cutoff == np.inf:
-                max_semiangle = 50
-            else:
-                max_semiangle = self._semiangle_cutoff * 1.6
-
-        alpha = np.linspace(0, max_semiangle / 1000., 500)
-
-        aberrations = self.evaluate_aberrations(alpha, phi)
-        aperture = self.evaluate_aperture(alpha)
-        temporal_envelope = self.evaluate_temporal_envelope(alpha)
-        spatial_envelope = self.evaluate_spatial_envelope(alpha, phi)
-        gaussian_envelope = self.evaluate_gaussian_envelope(alpha)
-        envelope = aperture * temporal_envelope * spatial_envelope * gaussian_envelope
-
-        calibration = Calibration(offset=0., sampling=(alpha[1] - alpha[0]) * 1000., units='mrad', name='alpha')
-
-        profiles = {}
-        profiles['ctf'] = Measurement(aberrations.imag * envelope, calibrations=[calibration], name='CTF')
-        profiles['aperture'] = Measurement(aperture, calibrations=[calibration], name='Aperture')
-        profiles['temporal_envelope'] = Measurement(temporal_envelope,
-                                                    calibrations=[calibration],
-                                                    name='Temporal')
-        profiles['spatial_envelope'] = Measurement(spatial_envelope, calibrations=[calibration],
-                                                   name='Spatial')
-        profiles['gaussian_spread'] = Measurement(gaussian_envelope, calibrations=[calibration],
-                                                  name='Gaussian')
-        profiles['envelope'] = Measurement(envelope, calibrations=[calibration], name='Envelope')
-        return profiles
-
-    def apply(self, waves, interact=False, sliders=None):
-        from abtem.visualize.bqplot import show_measurement_2d
-        from abtem.visualize.widgets import quick_sliders
-        import ipywidgets as widgets
-
-        if interact:
-            image_waves = waves.copy()
-
-            def update():
-                image_waves._array[:] = waves.apply_ctf(self).array
-                return image_waves.intensity()
-
-            figure, callback = show_measurement_2d(update)
-
-            self.changed.register(callback)
-            if sliders:
-                sliders = quick_sliders(self, **sliders)
-                figure = widgets.HBox([figure, widgets.VBox(sliders)])
-            return image_waves, figure
-        else:
-            if sliders:
-                raise RuntimeError()
-
-            return waves.apply_ctf(self)
-
-    def interact(self, max_semiangle: float = None, phi: float = 0., sliders=None):
-        import bqplot.pyplot as plt
-        from abtem.visualize.bqplot import show_measurement_1d
-        from abtem.visualize.widgets import quick_sliders
-        import ipywidgets as widgets
-
-        figure = plt.figure(fig_margin={'top': 0, 'bottom': 50, 'left': 50, 'right': 0})
-        figure.layout.height = '250px'
-        figure.layout.width = '300px'
-
-        _, callback = show_measurement_1d(lambda: self.profiles(max_semiangle, phi).values(), figure)
-        self.changed.register(callback)
-
-        if sliders:
-            sliders = quick_sliders(self, **sliders)
-            return widgets.HBox([figure, widgets.VBox(sliders)])
-        else:
-            return figure
-
-    def show(self, max_semiangle: float = None, phi: float = 0, ax=None, **kwargs):
-        """
-        Show the contrast transfer function.
-
-        Parameters
-        ----------
-        max_semiangle: float
-            Maximum semiangle to display in the plot.
-        ax: matplotlib Axes, optional
-            If given, the plot will be added to this matplotlib axes.
-        phi: float, optional
-            The contrast transfer function will be plotted along this angle. Default is 0.
-        n: int, optional
-            Number of evaluation points to use in the plot. Default is 1000.
-        title: str, optional
-            The title of the plot. Default is 'None'.
-        kwargs:
-            Additional keyword arguments for the line plots.
-        """
-        import matplotlib.pyplot as plt
-
-        if ax is None:
-            ax = plt.subplot()
-
-        for key, profile in self.profiles(max_semiangle, phi).items():
-            if not np.all(profile.array == 1.):
-                ax, lines = profile.show(legend=True, ax=ax, **kwargs)
-
-        return ax
-
-    def copy(self):
-        parameters = self.parameters.copy()
-        return self.__class__(semiangle_cutoff=self.semiangle_cutoff,
-                              rolloff=self.rolloff,
-                              focal_spread=self.focal_spread,
-                              angular_spread=self.angular_spread,
-                              gaussian_spread=self.gaussian_spread,
-                              energy=self.energy,
-                              parameters=parameters)
-
-
-def scherzer_defocus(Cs, energy):
-    """
-    Calculate the Scherzer defocus.
-
-    Parameters
-    ----------
-    Cs: float
-        Spherical aberration [Å].
-    energy: float
-        Electron energy [eV].
-
-    Returns
-    -------
-    float
-        The Scherzer defocus.
-    """
-
-    return np.sign(Cs) * np.sqrt(3 / 2 * np.abs(Cs) * energy2wavelength(energy))
-
-
-def point_resolution(Cs: float, energy: float):
-    """
-    Calculate the point resolution.
-
-    Parameters
-    ----------
-    Cs: float
-        Spherical aberration [Å].
-    energy: float
-        Electron energy [eV].
-
-    Returns
-    -------
-    float
-        The point resolution.
-    """
-
-    return (energy2wavelength(energy) ** 3 * np.abs(Cs) / 6) ** (1 / 4)
-
-
-def polar2cartesian(polar):
-    """
-    Convert between polar and Cartesian aberration coefficients.
-
-    Parameters
-    ----------
-    polar: dict
-        Mapping from polar aberration symbols to their corresponding values.
-
-    Returns
-    -------
-    dict
-        Mapping from cartesian aberration symbols to their corresponding values.
-    """
-
-    polar = defaultdict(lambda: 0, polar)
-
-    cartesian = dict()
-    cartesian['C10'] = polar['C10']
-    cartesian['C12a'] = - polar['C12'] * np.cos(2 * polar['phi12'])
-    cartesian['C12b'] = polar['C12'] * np.sin(2 * polar['phi12'])
-    cartesian['C21a'] = polar['C21'] * np.sin(polar['phi21'])
-    cartesian['C21b'] = polar['C21'] * np.cos(polar['phi21'])
-    cartesian['C23a'] = - polar['C23'] * np.sin(3 * polar['phi23'])
-    cartesian['C23b'] = polar['C23'] * np.cos(3 * polar['phi23'])
-    cartesian['C30'] = polar['C30']
-    cartesian['C32a'] = - polar['C32'] * np.cos(2 * polar['phi32'])
-    cartesian['C32b'] = polar['C32'] * np.cos(np.pi / 2 - 2 * polar['phi32'])
-    cartesian['C34a'] = polar['C34'] * np.cos(-4 * polar['phi34'])
-    K = np.sqrt(3 + np.sqrt(8.))
-    cartesian['C34b'] = 1 / 4. * (1 + K ** 2) ** 2 / (K ** 3 - K) * polar['C34'] * np.cos(
-        4 * np.arctan(1 / K) - 4 * polar['phi34'])
-
-    return cartesian
-
-
-def cartesian2polar(cartesian):
-    """
-    Convert between Cartesian and polar aberration coefficients.
-
-    Parameters
-    ----------
-    cartesian: dict
-        Mapping from Cartesian aberration symbols to their corresponding values.
-
-    Returns
-    -------
-    dict
-        Mapping from polar aberration symbols to their corresponding values.
-    """
-
-    cartesian = defaultdict(lambda: 0, cartesian)
-
-    polar = dict()
-    polar['C10'] = cartesian['C10']
-    polar['C12'] = - np.sqrt(cartesian['C12a'] ** 2 + cartesian['C12b'] ** 2)
-    polar['phi12'] = - np.arctan2(cartesian['C12b'], cartesian['C12a']) / 2.
-    polar['C21'] = np.sqrt(cartesian['C21a'] ** 2 + cartesian['C21b'] ** 2)
-    polar['phi21'] = np.arctan2(cartesian['C21a'], cartesian['C21b'])
-    polar['C23'] = np.sqrt(cartesian['C23a'] ** 2 + cartesian['C23b'] ** 2)
-    polar['phi23'] = -np.arctan2(cartesian['C23a'], cartesian['C23b']) / 3.
-    polar['C30'] = cartesian['C30']
-    polar['C32'] = -np.sqrt(cartesian['C32a'] ** 2 + cartesian['C32b'] ** 2)
-    polar['phi32'] = -np.arctan2(cartesian['C32b'], cartesian['C32a']) / 2.
-    polar['C34'] = np.sqrt(cartesian['C34a'] ** 2 + cartesian['C34b'] ** 2)
-    polar['phi34'] = np.arctan2(cartesian['C34b'], cartesian['C34a']) / 4
-
-    return polar
+"""Module to describe the contrast transfer function."""
+from collections import defaultdict
+from typing import Mapping, Union
+
+import numpy as np
+
+from abtem.base_classes import HasAcceleratorMixin, Accelerator, watched_method, watched_property, Event
+from abtem.device import get_array_module, get_device_function
+from abtem.measure import Measurement, Calibration
+from abtem.plot import PlotableMixin
+from abtem.utils import energy2wavelength, spatial_frequencies, polar_coordinates
+
+#: Symbols for the polar representation of all optical aberrations up to the fifth order.
+polar_symbols = ('C10', 'C12', 'phi12',
+                 'C21', 'phi21', 'C23', 'phi23',
+                 'C30', 'C32', 'phi32', 'C34', 'phi34',
+                 'C41', 'phi41', 'C43', 'phi43', 'C45', 'phi45',
+                 'C50', 'C52', 'phi52', 'C54', 'phi54', 'C56', 'phi56')
+
+#: Aliases for the most commonly used optical aberrations.
+polar_aliases = {'defocus': 'C10', 'astigmatism': 'C12', 'astigmatism_angle': 'phi12',
+                 'coma': 'C21', 'coma_angle': 'phi21',
+                 'Cs': 'C30',
+                 'C5': 'C50'}
+
+
+class CTF(HasAcceleratorMixin, PlotableMixin):
+    """
+    Contrast transfer function object
+
+    The Contrast Transfer Function (CTF) describes the aberrations of the objective lens in HRTEM and specifies how the
+    condenser system shapes the probe in STEM.
+
+    abTEM implements phase aberrations up to 5th order using polar coefficients. See Eq. 2.22 in the reference [1]_.
+    Cartesian coefficients can be converted to polar using the utility function abtem.transfer.cartesian2polar.
+
+    Partial coherence is included as an envelope in the quasi-coherent approximation. See Chapter 3.2 in reference [1]_.
+
+    For a more detailed discussion with examples, see our `walkthrough
+    <https://abtem.readthedocs.io/en/latest/walkthrough/05_contrast_transfer_function.html>`_.
+
+    Parameters
+    ----------
+    semiangle_cutoff: float
+        The semiangle cutoff describes the sharp Fourier space cutoff due to the objective aperture [mrad].
+    rolloff: float
+        Softens the cutoff. A value of 0 gives a hard cutoff, while 1 gives the softest possible cutoff [Å].
+    focal_spread: float
+        The 1/e width of the focal spread due to chromatic aberration and lens current instability [Å].
+    angular_spread: float
+        The 1/e width of the angular deviations due to source size [Å].
+    gaussian_spread:
+        The 1/e width image deflections due to vibrations and thermal magnetic noise [Å].
+    energy: float
+        The electron energy of the wave functions this contrast transfer function will be applied to [eV].
+    parameters: dict
+        Mapping from aberration symbols to their corresponding values. All aberration magnitudes should be given in Å.
+    kwargs:
+        Provide the aberration coefficients as keyword arguments.
+
+    References
+    ----------
+    .. [1] Kirkland, E. J. (2010). Advanced Computing in Electron Microscopy (2nd ed.). Springer.
+
+    """
+
+    def __init__(self, semiangle_cutoff: float = np.inf, rolloff: float = 0.1, focal_spread: float = 0.,
+                 angular_spread: float = 0., gaussian_spread: float = 0., energy: float = None,
+                 parameters: Mapping[str, float] = None, **kwargs):
+
+        for key in kwargs.keys():
+            if (key not in polar_symbols) and (key not in polar_aliases.keys()):
+                raise ValueError('{} not a recognized parameter'.format(key))
+
+        self.changed = Event()
+
+        self._accelerator = Accelerator(energy=energy)
+        self._accelerator.changed.register(self.changed.notify)
+
+        self._semiangle_cutoff = semiangle_cutoff
+        self._rolloff = rolloff
+        self._focal_spread = focal_spread
+        self._angular_spread = angular_spread
+        self._gaussian_spread = gaussian_spread
+        self._parameters = dict(zip(polar_symbols, [0.] * len(polar_symbols)))
+
+        if parameters is None:
+            parameters = {}
+
+        parameters.update(kwargs)
+        self.set_parameters(parameters)
+
+        def parametrization_property(key):
+
+            def getter(self):
+                return self._parameters[key]
+
+            def setter(self, value):
+                old = getattr(self, key)
+                self._parameters[key] = value
+                self.changed.notify(**{'notifier': self, 'property_name': key, 'change': old != value})
+
+            return property(getter, setter)
+
+        for symbol in polar_symbols:
+            setattr(self.__class__, symbol, parametrization_property(symbol))
+
+        for key, value in polar_aliases.items():
+            if key != 'defocus':
+                setattr(self.__class__, key, parametrization_property(value))
+
+    @property
+    def nyquist_sampling(self):
+        return 1 / (4 * self.semiangle_cutoff / self.wavelength * 1e-3)
+
+    @property
+    def parameters(self):
+        """The parameters."""
+        return self._parameters
+
+    @property
+    def defocus(self) -> float:
+        """The defocus [Å]."""
+        return - self._parameters['C10']
+
+    @defocus.setter
+    def defocus(self, value: float):
+        self.C10 = -value
+
+    @property
+    def semiangle_cutoff(self) -> float:
+        """The semi-angle cutoff [mrad]."""
+        return self._semiangle_cutoff
+
+    @semiangle_cutoff.setter
+    @watched_property('changed')
+    def semiangle_cutoff(self, value: float):
+        self._semiangle_cutoff = value
+
+    @property
+    def rolloff(self) -> float:
+        """The fraction of soft tapering of the cutoff."""
+        return self._rolloff
+
+    @rolloff.setter
+    @watched_property('changed')
+    def rolloff(self, value: float):
+        self._rolloff = value
+
+    @property
+    def focal_spread(self) -> float:
+        """The focal spread [Å]."""
+        return self._focal_spread
+
+    @focal_spread.setter
+    @watched_property('changed')
+    def focal_spread(self, value: float):
+        """The angular spread [mrad]."""
+        self._focal_spread = value
+
+    @property
+    def angular_spread(self) -> float:
+        return self._angular_spread
+
+    @angular_spread.setter
+    @watched_property('changed')
+    def angular_spread(self, value: float):
+        self._angular_spread = value
+
+    @property
+    def gaussian_spread(self) -> float:
+        """The Gaussian spread [Å]."""
+        return self._gaussian_spread
+
+    @gaussian_spread.setter
+    @watched_property('changed')
+    def gaussian_spread(self, value: float):
+        self._gaussian_spread = value
+
+    @watched_method('changed')
+    def set_parameters(self, parameters: dict):
+        """
+        Set the phase of the phase aberration.
+
+        Parameters
+        ----------
+        parameters: dict
+            Mapping from aberration symbols to their corresponding values.
+        """
+
+        for symbol, value in parameters.items():
+            if symbol in self._parameters.keys():
+                self._parameters[symbol] = value
+
+            elif symbol == 'defocus':
+                self._parameters[polar_aliases[symbol]] = -value
+
+            elif symbol in polar_aliases.keys():
+                self._parameters[polar_aliases[symbol]] = value
+
+            else:
+                raise ValueError('{} not a recognized parameter'.format(symbol))
+
+        return parameters
+
+    def evaluate_aperture(self, alpha: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+        xp = get_array_module(alpha)
+        semiangle_cutoff = self.semiangle_cutoff / 1000
+
+        if self.semiangle_cutoff == xp.inf:
+            return xp.ones_like(alpha)
+
+        if self.rolloff > 0.:
+            rolloff = self.rolloff * semiangle_cutoff
+            array = .5 * (1 + xp.cos(np.pi * (alpha - semiangle_cutoff + rolloff) / rolloff))
+            array[alpha > semiangle_cutoff] = 0.
+            array = xp.where(alpha > semiangle_cutoff - rolloff, array, xp.ones_like(alpha, dtype=xp.float32))
+        else:
+            array = xp.array(alpha < semiangle_cutoff).astype(xp.float32)
+        return array
+
+    def evaluate_temporal_envelope(self, alpha: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+        xp = get_array_module(alpha)
+        return xp.exp(- (.5 * xp.pi / self.wavelength * self.focal_spread * alpha ** 2) ** 2).astype(xp.float32)
+
+    def evaluate_gaussian_envelope(self, alpha: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+        xp = get_array_module(alpha)
+        return xp.exp(- .5 * self.gaussian_spread ** 2 * alpha ** 2 / self.wavelength ** 2)
+
+    def evaluate_spatial_envelope(self, alpha: Union[float, np.ndarray], phi: Union[float, np.ndarray]) -> \
+            Union[float, np.ndarray]:
+        xp = get_array_module(alpha)
+        p = self.parameters
+        dchi_dk = 2 * xp.pi / self.wavelength * (
+                (p['C12'] * xp.cos(2. * (phi - p['phi12'])) + p['C10']) * alpha +
+                (p['C23'] * xp.cos(3. * (phi - p['phi23'])) +
+                 p['C21'] * xp.cos(1. * (phi - p['phi21']))) * alpha ** 2 +
+                (p['C34'] * xp.cos(4. * (phi - p['phi34'])) +
+                 p['C32'] * xp.cos(2. * (phi - p['phi32'])) + p['C30']) * alpha ** 3 +
+                (p['C45'] * xp.cos(5. * (phi - p['phi45'])) +
+                 p['C43'] * xp.cos(3. * (phi - p['phi43'])) +
+                 p['C41'] * xp.cos(1. * (phi - p['phi41']))) * alpha ** 4 +
+                (p['C56'] * xp.cos(6. * (phi - p['phi56'])) +
+                 p['C54'] * xp.cos(4. * (phi - p['phi54'])) +
+                 p['C52'] * xp.cos(2. * (phi - p['phi52'])) + p['C50']) * alpha ** 5)
+
+        dchi_dphi = -2 * xp.pi / self.wavelength * (
+                1 / 2. * (2. * p['C12'] * xp.sin(2. * (phi - p['phi12']))) * alpha +
+                1 / 3. * (3. * p['C23'] * xp.sin(3. * (phi - p['phi23'])) +
+                          1. * p['C21'] * xp.sin(1. * (phi - p['phi21']))) * alpha ** 2 +
+                1 / 4. * (4. * p['C34'] * xp.sin(4. * (phi - p['phi34'])) +
+                          2. * p['C32'] * xp.sin(2. * (phi - p['phi32']))) * alpha ** 3 +
+                1 / 5. * (5. * p['C45'] * xp.sin(5. * (phi - p['phi45'])) +
+                          3. * p['C43'] * xp.sin(3. * (phi - p['phi43'])) +
+                          1. * p['C41'] * xp.sin(1. * (phi - p['phi41']))) * alpha ** 4 +
+                1 / 6. * (6. * p['C56'] * xp.sin(6. * (phi - p['phi56'])) +
+                          4. * p['C54'] * xp.sin(4. * (phi - p['phi54'])) +
+                          2. * p['C52'] * xp.sin(2. * (phi - p['phi52']))) * alpha ** 5)
+
+        return xp.exp(-xp.sign(self.angular_spread) * (self.angular_spread / 2 / 1000) ** 2 *
+                      (dchi_dk ** 2 + dchi_dphi ** 2))
+
+    def evaluate_chi(self, alpha: Union[float, np.ndarray], phi: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+        xp = get_array_module(alpha)
+        p = self.parameters
+
+        alpha2 = alpha ** 2
+        alpha = xp.array(alpha)
+
+        array = xp.zeros(alpha.shape, dtype=np.float32)
+        if any([p[symbol] != 0. for symbol in ('C10', 'C12', 'phi12')]):
+            array += (1 / 2 * alpha2 *
+                      (p['C10'] +
+                       p['C12'] * xp.cos(2 * (phi - p['phi12']))))
+
+        if any([p[symbol] != 0. for symbol in ('C21', 'phi21', 'C23', 'phi23')]):
+            array += (1 / 3 * alpha2 * alpha *
+                      (p['C21'] * xp.cos(phi - p['phi21']) +
+                       p['C23'] * xp.cos(3 * (phi - p['phi23']))))
+
+        if any([p[symbol] != 0. for symbol in ('C30', 'C32', 'phi32', 'C34', 'phi34')]):
+            array += (1 / 4 * alpha2 ** 2 *
+                      (p['C30'] +
+                       p['C32'] * xp.cos(2 * (phi - p['phi32'])) +
+                       p['C34'] * xp.cos(4 * (phi - p['phi34']))))
+
+        if any([p[symbol] != 0. for symbol in ('C41', 'phi41', 'C43', 'phi43', 'C45', 'phi41')]):
+            array += (1 / 5 * alpha2 ** 2 * alpha *
+                      (p['C41'] * xp.cos((phi - p['phi41'])) +
+                       p['C43'] * xp.cos(3 * (phi - p['phi43'])) +
+                       p['C45'] * xp.cos(5 * (phi - p['phi45']))))
+
+        if any([p[symbol] != 0. for symbol in ('C50', 'C52', 'phi52', 'C54', 'phi54', 'C56', 'phi56')]):
+            array += (1 / 6 * alpha2 ** 3 *
+                      (p['C50'] +
+                       p['C52'] * xp.cos(2 * (phi - p['phi52'])) +
+                       p['C54'] * xp.cos(4 * (phi - p['phi54'])) +
+                       p['C56'] * xp.cos(6 * (phi - p['phi56']))))
+
+        array = 2 * xp.pi / self.wavelength * array
+        return array
+
+    def evaluate_aberrations(self, alpha: Union[float, np.ndarray], phi: Union[float, np.ndarray]) -> \
+            Union[float, np.ndarray]:
+        xp = get_array_module(alpha)
+        complex_exponential = get_device_function(xp, 'complex_exponential')
+        return complex_exponential(-self.evaluate_chi(alpha, phi))
+
+    def evaluate(self, alpha: Union[float, np.ndarray], phi: Union[float, np.ndarray]) -> Union[float, np.ndarray]:
+        array = self.evaluate_aberrations(alpha, phi)
+
+        if self.semiangle_cutoff < np.inf:
+            array *= self.evaluate_aperture(alpha)
+
+        if self.focal_spread > 0.:
+            array *= self.evaluate_temporal_envelope(alpha)
+
+        if self.angular_spread > 0.:
+            array *= self.evaluate_spatial_envelope(alpha, phi)
+
+        if self.gaussian_spread > 0.:
+            array *= self.evaluate_gaussian_envelope(alpha)
+
+        return array
+
+    def evaluate_on_grid(self, grid, xp=np):
+        kx, ky = spatial_frequencies(grid.gpts, grid.sampling)
+        kx = kx.reshape((1, -1, 1))
+        ky = ky.reshape((1, 1, -1))
+        kx = xp.asarray(kx)
+        ky = xp.asarray(ky)
+        alpha, phi = polar_coordinates(xp.asarray(kx * self.wavelength), xp.asarray(ky * self.wavelength))
+        return self.evaluate(alpha, phi)
+
+    def profiles(self, max_semiangle: float = None, phi: float = 0.):
+        if max_semiangle is None:
+            if self._semiangle_cutoff == np.inf:
+                max_semiangle = 50
+            else:
+                max_semiangle = self._semiangle_cutoff * 1.6
+
+        alpha = np.linspace(0, max_semiangle / 1000., 500)
+
+        aberrations = self.evaluate_aberrations(alpha, phi)
+        aperture = self.evaluate_aperture(alpha)
+        temporal_envelope = self.evaluate_temporal_envelope(alpha)
+        spatial_envelope = self.evaluate_spatial_envelope(alpha, phi)
+        gaussian_envelope = self.evaluate_gaussian_envelope(alpha)
+        envelope = aperture * temporal_envelope * spatial_envelope * gaussian_envelope
+
+        calibration = Calibration(offset=0., sampling=(alpha[1] - alpha[0]) * 1000., units='mrad', name='alpha')
+
+        profiles = {}
+        profiles['ctf'] = Measurement(aberrations.imag * envelope, calibrations=[calibration], name='CTF')
+        profiles['aperture'] = Measurement(aperture, calibrations=[calibration], name='Aperture')
+        profiles['temporal_envelope'] = Measurement(temporal_envelope,
+                                                    calibrations=[calibration],
+                                                    name='Temporal')
+        profiles['spatial_envelope'] = Measurement(spatial_envelope, calibrations=[calibration],
+                                                   name='Spatial')
+        profiles['gaussian_spread'] = Measurement(gaussian_envelope, calibrations=[calibration],
+                                                  name='Gaussian')
+        profiles['envelope'] = Measurement(envelope, calibrations=[calibration], name='Envelope')
+        return profiles
+
+    def apply(self, waves, interact=False, sliders=None, throttling=0.):
+        from abtem.visualize.bqplot import show_measurement_2d
+        from abtem.visualize.widgets import quick_sliders, throttle
+        import ipywidgets as widgets
+
+        if interact:
+            image_waves = waves.copy()
+
+            def update():
+                image_waves._array[:] = waves.apply_ctf(self).array
+                return image_waves.intensity()
+
+            figure, callback = show_measurement_2d(update)
+
+            if throttling:
+                callback = throttle(throttling)(callback)
+
+            self.changed.register(callback)
+            if sliders:
+                sliders = quick_sliders(self, **sliders)
+                figure = widgets.HBox([figure, widgets.VBox(sliders)])
+            return image_waves, figure
+        else:
+            if sliders:
+                raise RuntimeError()
+
+            return waves.apply_ctf(self)
+
+    def interact(self, max_semiangle: float = None, phi: float = 0., sliders=None, throttling=False):
+        import bqplot.pyplot as plt
+        from abtem.visualize.bqplot import show_measurement_1d
+        from abtem.visualize.widgets import quick_sliders, throttle
+        import ipywidgets as widgets
+
+        figure = plt.figure(fig_margin={'top': 0, 'bottom': 50, 'left': 50, 'right': 0})
+        figure.layout.height = '250px'
+        figure.layout.width = '300px'
+
+        _, callback = show_measurement_1d(lambda: self.profiles(max_semiangle, phi).values(), figure)
+
+        if throttling:
+            callback = throttle(throttling)(callback)
+
+        self.changed.register(callback)
+
+        if sliders:
+            sliders = quick_sliders(self, **sliders)
+            return widgets.HBox([figure, widgets.VBox(sliders)])
+        else:
+            return figure
+
+    def show(self, max_semiangle: float = None, phi: float = 0, ax=None, **kwargs):
+        """
+        Show the contrast transfer function.
+
+        Parameters
+        ----------
+        max_semiangle: float
+            Maximum semiangle to display in the plot.
+        ax: matplotlib Axes, optional
+            If given, the plot will be added to this matplotlib axes.
+        phi: float, optional
+            The contrast transfer function will be plotted along this angle. Default is 0.
+        n: int, optional
+            Number of evaluation points to use in the plot. Default is 1000.
+        title: str, optional
+            The title of the plot. Default is 'None'.
+        kwargs:
+            Additional keyword arguments for the line plots.
+        """
+        import matplotlib.pyplot as plt
+
+        if ax is None:
+            ax = plt.subplot()
+
+        for key, profile in self.profiles(max_semiangle, phi).items():
+            if not np.all(profile.array == 1.):
+                ax, lines = profile.show(legend=True, ax=ax, **kwargs)
+
+        return ax
+
+    def copy(self):
+        parameters = self.parameters.copy()
+        return self.__class__(semiangle_cutoff=self.semiangle_cutoff,
+                              rolloff=self.rolloff,
+                              focal_spread=self.focal_spread,
+                              angular_spread=self.angular_spread,
+                              gaussian_spread=self.gaussian_spread,
+                              energy=self.energy,
+                              parameters=parameters)
+
+
+def scherzer_defocus(Cs, energy):
+    """
+    Calculate the Scherzer defocus.
+
+    Parameters
+    ----------
+    Cs: float
+        Spherical aberration [Å].
+    energy: float
+        Electron energy [eV].
+
+    Returns
+    -------
+    float
+        The Scherzer defocus.
+    """
+
+    return np.sign(Cs) * np.sqrt(3 / 2 * np.abs(Cs) * energy2wavelength(energy))
+
+
+def point_resolution(Cs: float, energy: float):
+    """
+    Calculate the point resolution.
+
+    Parameters
+    ----------
+    Cs: float
+        Spherical aberration [Å].
+    energy: float
+        Electron energy [eV].
+
+    Returns
+    -------
+    float
+        The point resolution.
+    """
+
+    return (energy2wavelength(energy) ** 3 * np.abs(Cs) / 6) ** (1 / 4)
+
+
+def polar2cartesian(polar):
+    """
+    Convert between polar and Cartesian aberration coefficients.
+
+    Parameters
+    ----------
+    polar: dict
+        Mapping from polar aberration symbols to their corresponding values.
+
+    Returns
+    -------
+    dict
+        Mapping from cartesian aberration symbols to their corresponding values.
+    """
+
+    polar = defaultdict(lambda: 0, polar)
+
+    cartesian = dict()
+    cartesian['C10'] = polar['C10']
+    cartesian['C12a'] = - polar['C12'] * np.cos(2 * polar['phi12'])
+    cartesian['C12b'] = polar['C12'] * np.sin(2 * polar['phi12'])
+    cartesian['C21a'] = polar['C21'] * np.sin(polar['phi21'])
+    cartesian['C21b'] = polar['C21'] * np.cos(polar['phi21'])
+    cartesian['C23a'] = - polar['C23'] * np.sin(3 * polar['phi23'])
+    cartesian['C23b'] = polar['C23'] * np.cos(3 * polar['phi23'])
+    cartesian['C30'] = polar['C30']
+    cartesian['C32a'] = - polar['C32'] * np.cos(2 * polar['phi32'])
+    cartesian['C32b'] = polar['C32'] * np.cos(np.pi / 2 - 2 * polar['phi32'])
+    cartesian['C34a'] = polar['C34'] * np.cos(-4 * polar['phi34'])
+    K = np.sqrt(3 + np.sqrt(8.))
+    cartesian['C34b'] = 1 / 4. * (1 + K ** 2) ** 2 / (K ** 3 - K) * polar['C34'] * np.cos(
+        4 * np.arctan(1 / K) - 4 * polar['phi34'])
+
+    return cartesian
+
+
+def cartesian2polar(cartesian):
+    """
+    Convert between Cartesian and polar aberration coefficients.
+
+    Parameters
+    ----------
+    cartesian: dict
+        Mapping from Cartesian aberration symbols to their corresponding values.
+
+    Returns
+    -------
+    dict
+        Mapping from polar aberration symbols to their corresponding values.
+    """
+
+    cartesian = defaultdict(lambda: 0, cartesian)
+
+    polar = dict()
+    polar['C10'] = cartesian['C10']
+    polar['C12'] = - np.sqrt(cartesian['C12a'] ** 2 + cartesian['C12b'] ** 2)
+    polar['phi12'] = - np.arctan2(cartesian['C12b'], cartesian['C12a']) / 2.
+    polar['C21'] = np.sqrt(cartesian['C21a'] ** 2 + cartesian['C21b'] ** 2)
+    polar['phi21'] = np.arctan2(cartesian['C21a'], cartesian['C21b'])
+    polar['C23'] = np.sqrt(cartesian['C23a'] ** 2 + cartesian['C23b'] ** 2)
+    polar['phi23'] = -np.arctan2(cartesian['C23a'], cartesian['C23b']) / 3.
+    polar['C30'] = cartesian['C30']
+    polar['C32'] = -np.sqrt(cartesian['C32a'] ** 2 + cartesian['C32b'] ** 2)
+    polar['phi32'] = -np.arctan2(cartesian['C32b'], cartesian['C32a']) / 2.
+    polar['C34'] = np.sqrt(cartesian['C34a'] ** 2 + cartesian['C34b'] ** 2)
+    polar['phi34'] = np.arctan2(cartesian['C34b'], cartesian['C34a']) / 4
+
+    return polar
```

### Comparing `abtem-1.0.0b8/abtem/utils.py` & `abtem-1.0.0b9/abtem/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,250 +1,261 @@
-"""Module for various convenient utilities."""
-import numpy as np
-from ase import units
-
-from abtem.device import get_array_module, get_device_function
-from tqdm.auto import tqdm
-
-
-def energy2mass(energy):
-    """
-    Calculate relativistic mass from energy.
-
-    Parameters
-    ----------
-    energy: float
-        Energy [eV].
-
-    Returns
-    -------
-    float
-        Relativistic mass [kg]̄
-    """
-
-    return (1 + units._e * energy / (units._me * units._c ** 2)) * units._me
-
-
-def energy2wavelength(energy):
-    """
-    Calculate relativistic de Broglie wavelength from energy.
-
-    Parameters
-    ----------
-    energy: float
-        Energy [eV].
-
-    Returns
-    -------
-    float
-        Relativistic de Broglie wavelength [Å].
-    """
-
-    return units._hplanck * units._c / np.sqrt(
-        energy * (2 * units._me * units._c ** 2 / units._e + energy)) / units._e * 1.e10
-
-
-def energy2sigma(energy):
-    """
-    Calculate interaction parameter from energy.
-
-    Parameters
-    ----------
-    energy: float
-        Energy [ev].
-
-    Returns
-    -------
-    float
-        Interaction parameter [1 / (Å * eV)].
-    """
-
-    return (2 * np.pi * energy2mass(energy) * units.kg * units._e * units.C * energy2wavelength(energy) / (
-            units._hplanck * units.s * units.J) ** 2)
-
-
-def spatial_frequencies(gpts, sampling):
-    """
-    Calculate spatial frequencies of a grid.
-
-    Parameters
-    ----------
-    gpts: tuple of int
-        Number of grid points.
-    sampling: tuple of float
-        Sampling of the potential [1 / Å].
-
-    Returns
-    -------
-    tuple of arrays
-    """
-
-    return tuple(np.fft.fftfreq(n, d).astype(np.float32) for n, d in zip(gpts, sampling))
-
-
-def polar_coordinates(x, y):
-    """Calculate a polar grid for a given Cartesian grid."""
-    xp = get_array_module(x)
-    alpha = xp.sqrt(x.reshape((-1, 1)) ** 2 + y.reshape((1, -1)) ** 2)
-    phi = xp.arctan2(x.reshape((-1, 1)), y.reshape((1, -1)))
-    return alpha, phi
-
-
-def periodic_crop(array, corners, new_shape):
-    xp = get_array_module(array)
-
-    if ((corners[0] > 0) & (corners[1] > 0) & (corners[0] + new_shape[0] < array.shape[-2]) & (
-            corners[1] + new_shape[1] < array.shape[-1])):
-        array = array[..., corners[0]:corners[0] + new_shape[0], corners[1]:corners[1] + new_shape[1]]
-        return array
-
-    x = xp.arange(corners[0], corners[0] + new_shape[0], dtype=xp.int) % array.shape[-2]
-    y = xp.arange(corners[1], corners[1] + new_shape[1], dtype=xp.int) % array.shape[-1]
-
-    x, y = xp.meshgrid(x, y, indexing='ij')
-    array = array[..., x.ravel(), y.ravel()].reshape(array.shape[:-2] + new_shape)
-    return array
-
-
-def fft_interpolation_masks(shape1, shape2, xp=np, epsilon=1e-7):
-    kx1 = xp.fft.fftfreq(shape1[-2], 1 / shape1[-2])
-    ky1 = xp.fft.fftfreq(shape1[-1], 1 / shape1[-1])
-
-    kx2 = xp.fft.fftfreq(shape2[-2], 1 / shape2[-2])
-    ky2 = xp.fft.fftfreq(shape2[-1], 1 / shape2[-1])
-
-    kx_min = max(xp.min(kx1), xp.min(kx2)) - epsilon
-    kx_max = min(xp.max(kx1), xp.max(kx2)) + epsilon
-    ky_min = max(xp.min(ky1), xp.min(ky2)) - epsilon
-    ky_max = min(xp.max(ky1), xp.max(ky2)) + epsilon
-
-    kx1, ky1 = xp.meshgrid(kx1, ky1, indexing='ij')
-    kx2, ky2 = xp.meshgrid(kx2, ky2, indexing='ij')
-
-    mask1 = (kx1 <= kx_max) & (kx1 >= kx_min) & (ky1 <= ky_max) & (ky1 >= ky_min)
-    mask2 = (kx2 <= kx_max) & (kx2 >= kx_min) & (ky2 <= ky_max) & (ky2 >= ky_min)
-
-    return mask1, mask2
-
-
-def fft_crop(array, new_shape):
-    # assert np.iscomplexobj(array)
-    xp = get_array_module(array)
-
-    mask_in, mask_out = fft_interpolation_masks(array.shape, new_shape, xp=xp)
-
-    if len(new_shape) < len(array.shape):
-        new_shape = array.shape[:-2] + new_shape
-
-    new_array = xp.zeros(new_shape, dtype=array.dtype)
-
-    # shape_pad = len(new_array.shape) - len(mask_out.shape)
-    # mask_out = mask_out.reshape((1,) * shape_pad + mask_out.shape)
-    # mask_in = mask_in.reshape((1,) * shape_pad + mask_in.shape)
-    # print(mask_out.shape, new_array.shape, array.shape, mask_in.shape)
-
-    out_indices = xp.where(mask_out)
-    in_indices = xp.where(mask_in)
-
-    new_array[..., out_indices[0], out_indices[1]] = array[..., in_indices[0], in_indices[1]]
-    return new_array
-
-
-def fft_interpolate_2d(array, new_shape, normalization='values', overwrite_x=False):
-    xp = get_array_module(array)
-    fft2 = get_device_function(xp, 'fft2')
-    ifft2 = get_device_function(xp, 'ifft2')
-
-    old_size = array.shape[-2] * array.shape[-1]
-
-    if np.iscomplexobj(array):
-        array = ifft2(fft_crop(fft2(array), new_shape), overwrite_x=overwrite_x)
-    else:
-        array = ifft2(fft_crop(fft2(array), new_shape), overwrite_x=overwrite_x).real
-
-    if normalization == 'values':
-        array *= array.shape[-1] * array.shape[-2] / old_size
-    elif normalization == 'norm':
-        array *= array.shape[-1] * array.shape[-2] / old_size
-    elif (normalization != False) and (normalization != None):
-        raise RuntimeError()
-
-    return array  # * norm
-
-
-def subdivide_into_batches(num_items: int, num_batches: int = None, max_batch: int = None):
-    """
-    Split an n integer into m (almost) equal integers, such that the sum of smaller integers equals n.
-
-    Parameters
-    ----------
-    n: int
-        The integer to split.
-    m: int
-        The number integers n will be split into.
-
-    Returns
-    -------
-    list of int
-    """
-    if (num_batches is not None) & (max_batch is not None):
-        raise RuntimeError()
-
-    if num_batches is None:
-        if max_batch is not None:
-            num_batches = (num_items + (-num_items % max_batch)) // max_batch
-        else:
-            raise RuntimeError()
-
-    if num_items < num_batches:
-        raise RuntimeError('num_batches may not be larger than num_items')
-
-    elif num_items % num_batches == 0:
-        return [num_items // num_batches] * num_batches
-    else:
-        v = []
-        zp = num_batches - (num_items % num_batches)
-        pp = num_items // num_batches
-        for i in range(num_batches):
-            if i >= zp:
-                v = [pp + 1] + v
-            else:
-                v = [pp] + v
-        return v
-
-
-def generate_batches(num_items: int, num_batches: int = None, max_batch: int = None, start=0):
-    for batch in subdivide_into_batches(num_items, num_batches, max_batch):
-        end = start + batch
-        yield start, end
-
-        start = end
-
-
-class ProgressBar:
-    """Object to describe progress bar indicators for computations."""
-
-    def __init__(self, **kwargs):
-        self._tqdm = tqdm(**kwargs)
-
-    @property
-    def tqdm(self):
-        return self._tqdm
-
-    @property
-    def disable(self):
-        return self.tqdm.disable
-
-    def update(self, n):
-        if not self.disable:
-            self.tqdm.update(n)
-
-    def reset(self):
-        if not self.disable:
-            self.tqdm.reset()
-
-    def refresh(self):
-        if not self.disable:
-            self.tqdm.refresh()
-
-    def close(self):
-        self.tqdm.close()
+"""Module for various convenient utilities."""
+import numpy as np
+from ase import units
+
+from abtem.device import get_array_module, get_device_function
+from tqdm.auto import tqdm
+
+
+def energy2mass(energy):
+    """
+    Calculate relativistic mass from energy.
+
+    Parameters
+    ----------
+    energy: float
+        Energy [eV].
+
+    Returns
+    -------
+    float
+        Relativistic mass [kg]̄
+    """
+
+    return (1 + units._e * energy / (units._me * units._c ** 2)) * units._me
+
+
+def energy2wavelength(energy):
+    """
+    Calculate relativistic de Broglie wavelength from energy.
+
+    Parameters
+    ----------
+    energy: float
+        Energy [eV].
+
+    Returns
+    -------
+    float
+        Relativistic de Broglie wavelength [Å].
+    """
+
+    return units._hplanck * units._c / np.sqrt(
+        energy * (2 * units._me * units._c ** 2 / units._e + energy)) / units._e * 1.e10
+
+
+def energy2sigma(energy):
+    """
+    Calculate interaction parameter from energy.
+
+    Parameters
+    ----------
+    energy: float
+        Energy [ev].
+
+    Returns
+    -------
+    float
+        Interaction parameter [1 / (Å * eV)].
+    """
+
+    return (2 * np.pi * energy2mass(energy) * units.kg * units._e * units.C * energy2wavelength(energy) / (
+            units._hplanck * units.s * units.J) ** 2)
+
+
+def spatial_frequencies(gpts, sampling):
+    """
+    Calculate spatial frequencies of a grid.
+
+    Parameters
+    ----------
+    gpts: tuple of int
+        Number of grid points.
+    sampling: tuple of float
+        Sampling of the potential [1 / Å].
+
+    Returns
+    -------
+    tuple of arrays
+    """
+
+    return tuple(np.fft.fftfreq(n, d).astype(np.float32) for n, d in zip(gpts, sampling))
+
+
+def polar_coordinates(x, y):
+    """Calculate a polar grid for a given Cartesian grid."""
+    xp = get_array_module(x)
+    alpha = xp.sqrt(x.reshape((-1, 1)) ** 2 + y.reshape((1, -1)) ** 2)
+    phi = xp.arctan2(x.reshape((-1, 1)), y.reshape((1, -1)))
+    return alpha, phi
+
+def _disc_meshgrid(r):
+    """Internal function to return all indices inside a disk with a given radius."""
+    cols = np.zeros((2 * r + 1, 2 * r + 1)).astype(np.int32)
+    cols[:] = np.linspace(0, 2 * r, 2 * r + 1) - r
+    rows = cols.T
+    inside = (rows ** 2 + cols ** 2) <= r ** 2
+    return rows[inside], cols[inside]
+
+
+def periodic_crop(array, corners, new_shape):
+    xp = get_array_module(array)
+
+    if ((corners[0] > 0) & (corners[1] > 0) & (corners[0] + new_shape[0] < array.shape[-2]) & (
+            corners[1] + new_shape[1] < array.shape[-1])):
+        array = array[..., corners[0]:corners[0] + new_shape[0], corners[1]:corners[1] + new_shape[1]]
+        return array
+
+    x = xp.arange(corners[0], corners[0] + new_shape[0], dtype=xp.int) % array.shape[-2]
+    y = xp.arange(corners[1], corners[1] + new_shape[1], dtype=xp.int) % array.shape[-1]
+
+    x, y = xp.meshgrid(x, y, indexing='ij')
+    array = array[..., x.ravel(), y.ravel()].reshape(array.shape[:-2] + new_shape)
+    return array
+
+
+def fft_interpolation_masks(shape1, shape2, xp=np, epsilon=1e-7):
+    kx1 = xp.fft.fftfreq(shape1[-2], 1 / shape1[-2])
+    ky1 = xp.fft.fftfreq(shape1[-1], 1 / shape1[-1])
+
+    kx2 = xp.fft.fftfreq(shape2[-2], 1 / shape2[-2])
+    ky2 = xp.fft.fftfreq(shape2[-1], 1 / shape2[-1])
+
+    kx_min = max(xp.min(kx1), xp.min(kx2)) - epsilon
+    kx_max = min(xp.max(kx1), xp.max(kx2)) + epsilon
+    ky_min = max(xp.min(ky1), xp.min(ky2)) - epsilon
+    ky_max = min(xp.max(ky1), xp.max(ky2)) + epsilon
+
+    kx1, ky1 = xp.meshgrid(kx1, ky1, indexing='ij')
+    kx2, ky2 = xp.meshgrid(kx2, ky2, indexing='ij')
+
+    mask1 = (kx1 <= kx_max) & (kx1 >= kx_min) & (ky1 <= ky_max) & (ky1 >= ky_min)
+    mask2 = (kx2 <= kx_max) & (kx2 >= kx_min) & (ky2 <= ky_max) & (ky2 >= ky_min)
+
+    return mask1, mask2
+
+
+def fft_crop(array, new_shape):
+    # assert np.iscomplexobj(array)
+    xp = get_array_module(array)
+
+    mask_in, mask_out = fft_interpolation_masks(array.shape, new_shape, xp=xp)
+
+    if len(new_shape) < len(array.shape):
+        new_shape = array.shape[:-2] + new_shape
+
+    new_array = xp.zeros(new_shape, dtype=array.dtype)
+
+    # shape_pad = len(new_array.shape) - len(mask_out.shape)
+    # mask_out = mask_out.reshape((1,) * shape_pad + mask_out.shape)
+    # mask_in = mask_in.reshape((1,) * shape_pad + mask_in.shape)
+    # print(mask_out.shape, new_array.shape, array.shape, mask_in.shape)
+
+    out_indices = xp.where(mask_out)
+    in_indices = xp.where(mask_in)
+
+    new_array[..., out_indices[0], out_indices[1]] = array[..., in_indices[0], in_indices[1]]
+    return new_array
+
+
+def fft_interpolate_2d(array, new_shape, normalization='values', overwrite_x=False):
+    xp = get_array_module(array)
+    fft2 = get_device_function(xp, 'fft2')
+    ifft2 = get_device_function(xp, 'ifft2')
+
+    old_size = array.shape[-2] * array.shape[-1]
+
+    if np.iscomplexobj(array):
+        cropped = fft_crop(fft2(array), new_shape)
+        print(cropped.shape)
+        array = ifft2(cropped, overwrite_x=overwrite_x)
+    else:
+        array = xp.complex64(array)
+        array = ifft2(fft_crop(fft2(array), new_shape), overwrite_x=overwrite_x).real
+
+    if normalization == 'values':
+        array *= array.shape[-1] * array.shape[-2] / old_size
+    elif normalization == 'norm':
+        array *= array.shape[-1] * array.shape[-2] / old_size
+    elif (normalization != False) and (normalization != None):
+        raise RuntimeError()
+
+    return array  # * norm
+
+
+def subdivide_into_batches(num_items: int, num_batches: int = None, max_batch: int = None):
+    """
+    Split an n integer into m (almost) equal integers, such that the sum of smaller integers equals n.
+
+    Parameters
+    ----------
+    n: int
+        The integer to split.
+    m: int
+        The number integers n will be split into.
+
+    Returns
+    -------
+    list of int
+    """
+    if (num_batches is not None) & (max_batch is not None):
+        raise RuntimeError()
+
+    if num_batches is None:
+        if max_batch is not None:
+            num_batches = (num_items + (-num_items % max_batch)) // max_batch
+        else:
+            raise RuntimeError()
+
+    if num_items < num_batches:
+        raise RuntimeError('num_batches may not be larger than num_items')
+
+    elif num_items % num_batches == 0:
+        return [num_items // num_batches] * num_batches
+    else:
+        v = []
+        zp = num_batches - (num_items % num_batches)
+        pp = num_items // num_batches
+        for i in range(num_batches):
+            if i >= zp:
+                v = [pp + 1] + v
+            else:
+                v = [pp] + v
+        return v
+
+
+def generate_batches(num_items: int, num_batches: int = None, max_batch: int = None, start=0):
+    for batch in subdivide_into_batches(num_items, num_batches, max_batch):
+        end = start + batch
+        yield start, end
+
+        start = end
+
+
+class ProgressBar:
+    """Object to describe progress bar indicators for computations."""
+
+    def __init__(self, **kwargs):
+        self._tqdm = tqdm(**kwargs)
+
+    @property
+    def tqdm(self):
+        return self._tqdm
+
+    @property
+    def disable(self):
+        return self.tqdm.disable
+
+    def update(self, n):
+        if not self.disable:
+            self.tqdm.update(n)
+
+    def reset(self):
+        if not self.disable:
+            self.tqdm.reset()
+
+    def refresh(self):
+        if not self.disable:
+            self.tqdm.refresh()
+
+    def close(self):
+        self.tqdm.close()
```

### Comparing `abtem-1.0.0b8/abtem/visualize/mpl.py` & `abtem-1.0.0b9/abtem/visualize/mpl.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,239 +1,240 @@
-"""Module for plotting atoms, images, line scans, and diffraction patterns."""
-from collections.abc import Iterable
-
-import matplotlib.pyplot as plt
-import numpy as np
-from ase.data import covalent_radii
-from ase.data.colors import jmol_colors
-from matplotlib.collections import PatchCollection
-from matplotlib.patches import Circle
-from abtem.visualize.utils import format_label
-
-#: Array to facilitate the display of cell boundaries.
-_cube = np.array([[[0, 0, 0], [0, 0, 1]],
-                  [[0, 0, 0], [0, 1, 0]],
-                  [[0, 0, 0], [1, 0, 0]],
-                  [[0, 0, 1], [0, 1, 1]],
-                  [[0, 0, 1], [1, 0, 1]],
-                  [[0, 1, 0], [1, 1, 0]],
-                  [[0, 1, 0], [0, 1, 1]],
-                  [[1, 0, 0], [1, 1, 0]],
-                  [[1, 0, 0], [1, 0, 1]],
-                  [[0, 1, 1], [1, 1, 1]],
-                  [[1, 0, 1], [1, 1, 1]],
-                  [[1, 1, 0], [1, 1, 1]]])
-
-
-def _plane2axes(plane):
-    """Internal function for extracting axes from a plane."""
-    axes = ()
-    last_axis = [0, 1, 2]
-    for axis in list(plane):
-        if axis == 'x':
-            axes += (0,)
-            last_axis.remove(0)
-        if axis == 'y':
-            axes += (1,)
-            last_axis.remove(1)
-        if axis == 'z':
-            axes += (2,)
-            last_axis.remove(2)
-    return axes + (last_axis[0],)
-
-
-def show_atoms(atoms, repeat=(1, 1), scans=None, plane='xy', ax=None, scale_atoms=.5, title=None, numbering=False):
-    """
-    Show atoms function
-
-    Function to display atoms, especially in Jupyter notebooks.
-
-    Parameters
-    ----------
-    atoms : ASE atoms object
-        The atoms to be shown.
-    repeat : two ints, optional
-        Tiling of the image. Default is (1,1), ie. no tiling.
-    scans : ndarray, optional
-        List of scans to apply. Default is None.
-    plane : str
-        The projection plane.
-    ax : axes object
-        pyplot axes object.
-    scale_atoms : float
-        Scaling factor for the atom display sizes. Default is 0.5.
-    title : str
-        Title of the displayed image. Default is None.
-    numbering : bool
-        Option to set plot numbering. Default is False.
-    """
-
-    if ax is None:
-        fig, ax = plt.subplots()
-
-    axes = _plane2axes(plane)
-
-    atoms = atoms.copy()
-    cell = atoms.cell
-    atoms *= repeat + (1,)
-
-    for line in _cube:
-        cell_lines = np.array([np.dot(line[0], cell), np.dot(line[1], cell)])
-        ax.plot(cell_lines[:, axes[0]], cell_lines[:, axes[1]], 'k-')
-
-    if len(atoms) > 0:
-        positions = atoms.positions[:, axes[:2]]
-        order = np.argsort(atoms.positions[:, axes[2]])
-        positions = positions[order]
-
-        colors = jmol_colors[atoms.numbers[order]]
-
-        sizes = covalent_radii[atoms.numbers[order]] * scale_atoms
-
-        circles = []
-        for position, size in zip(positions, sizes):
-            circles.append(Circle(position, size))
-
-        coll = PatchCollection(circles, facecolors=colors, edgecolors='black')
-        ax.add_collection(coll)
-
-        ax.axis('equal')
-        ax.set_xlabel(plane[0] + ' [Å]')
-        ax.set_ylabel(plane[1] + ' [Å]')
-
-        ax.set_title(title)
-
-        if numbering:
-            for i, (position, size) in enumerate(zip(positions, sizes)):
-                ax.annotate('{}'.format(order[i]), xy=position, ha="center", va="center")
-
-    if scans is not None:
-        if not isinstance(scans, Iterable):
-            scans = [scans]
-
-        for scan in scans:
-            scan.add_to_mpl_plot(ax)
-
-
-def show_measurement_2d(measurement,
-                        ax=None,
-                        figsize=None,
-                        colorbar=False,
-                        cmap='gray',
-                        discrete_cmap=False,
-                        vmin=None,
-                        vmax=None,
-                        power=1.,
-                        **kwargs):
-    """
-    Show image function
-
-    Function to display an image.
-
-    Parameters
-    ----------
-    array : ndarray
-        Image array.
-    calibrations : tuple of calibration objects.
-        Spatial calibrations.
-    ax : axes object
-        pyplot axes object.
-    title : str, optional
-        Image title. Default is None.
-    colorbar : bool, optional
-        Option to show a colorbar. Default is False.
-    cmap : str, optional
-        Colormap name. Default is 'gray'.
-    figsize : float, pair of float, optional
-        Size of the figure in inches, either as a square for one number or a rectangle for two. Default is None.
-    scans : ndarray, optional
-        Array of scans. Default is None.
-    discrete : bool, optional
-        Option to discretize intensity values to integers. Default is False.
-    cbar_label : str, optional
-        Text label for the color bar. Default is None.
-    vmin : float, optional
-        Minimum of the intensity scale. Default is None.
-    vmax : float, optional
-        Maximum of the intensity scale. Default is None.
-    kwargs :
-        Remaining keyword arguments are passed to pyplot.
-    """
-
-    if ax is None:
-        fig, ax = plt.subplots(figsize=figsize)
-
-    calibrations = measurement.calibrations[-2:]
-    array = measurement.array[(0,) * (measurement.dimensions - 2) + (slice(None),) * 2]
-
-    if power != 1:
-        array = array ** power
-
-    extent = []
-    for calibration, num_elem in zip(calibrations, array.shape):
-        extent.append(calibration.offset)
-        extent.append(calibration.offset + num_elem * calibration.sampling)
-
-    if vmin is None:
-        vmin = np.min(array)
-        if discrete_cmap:
-            vmin -= .5
-
-    if vmax is None:
-        vmax = np.max(array)
-        if discrete_cmap:
-            vmax += .5
-
-    if discrete_cmap:
-        cmap = plt.get_cmap(cmap, np.max(array) - np.min(array) + 1)
-
-    im = ax.imshow(array.T, extent=extent, cmap=cmap, origin='lower', vmin=vmin, vmax=vmax, interpolation='nearest',
-                   **kwargs)
-
-    if colorbar:
-        cax = plt.colorbar(im, ax=ax, label=format_label(measurement))
-        if discrete_cmap:
-            cax.set_ticks(ticks=np.arange(np.min(array), np.max(array) + 1))
-
-    ax.set_xlabel(format_label(calibrations[-2]))
-    ax.set_ylabel(format_label(calibrations[-1]))
-
-    return ax, im
-
-
-def show_measurement_1d(measurement, ax=None, figsize=None, legend=False, title=None, **kwargs):
-    """
-    Show line function
-
-    Function to display a line scan.
-
-    Parameters
-    ----------
-    array : ndarray
-        Array of measurement values along a line.
-    calibration : calibration object
-        Spatial calibration for the line.
-    ax : axes object, optional
-        pyplot axes object.
-    title : str, optional
-        Title for the plot. Default is None.
-    legend : bool, optional
-        Option to display a plot legend. Default is False.
-    kwargs :
-       Remaining keyword arguments are passed to pyplot.
-    """
-
-    calibration = measurement.calibrations[0]
-    array = measurement.array
-    x = np.linspace(calibration.offset, calibration.offset + len(array) * calibration.sampling, len(array))
-
-    if ax is None:
-        fig, ax = plt.subplots(figsize=figsize)
-
-    lines = ax.plot(x, array, label=measurement.name, **kwargs)
-    ax.set_xlabel(format_label(calibration))
-    ax.set_ylabel(format_label(measurement))
-
-    if legend:
-        ax.legend()
-
-    return ax, lines[0]
+"""Module for plotting atoms, images, line scans, and diffraction patterns."""
+from collections.abc import Iterable
+
+import matplotlib.pyplot as plt
+import numpy as np
+from ase.data import covalent_radii
+from ase.data.colors import jmol_colors
+from matplotlib.collections import PatchCollection
+from matplotlib.patches import Circle
+from abtem.visualize.utils import format_label
+
+#: Array to facilitate the display of cell boundaries.
+_cube = np.array([[[0, 0, 0], [0, 0, 1]],
+                  [[0, 0, 0], [0, 1, 0]],
+                  [[0, 0, 0], [1, 0, 0]],
+                  [[0, 0, 1], [0, 1, 1]],
+                  [[0, 0, 1], [1, 0, 1]],
+                  [[0, 1, 0], [1, 1, 0]],
+                  [[0, 1, 0], [0, 1, 1]],
+                  [[1, 0, 0], [1, 1, 0]],
+                  [[1, 0, 0], [1, 0, 1]],
+                  [[0, 1, 1], [1, 1, 1]],
+                  [[1, 0, 1], [1, 1, 1]],
+                  [[1, 1, 0], [1, 1, 1]]])
+
+
+def _plane2axes(plane):
+    """Internal function for extracting axes from a plane."""
+    axes = ()
+    last_axis = [0, 1, 2]
+    for axis in list(plane):
+        if axis == 'x':
+            axes += (0,)
+            last_axis.remove(0)
+        if axis == 'y':
+            axes += (1,)
+            last_axis.remove(1)
+        if axis == 'z':
+            axes += (2,)
+            last_axis.remove(2)
+    return axes + (last_axis[0],)
+
+
+def show_atoms(atoms, repeat=(1, 1), scans=None, plane='xy', ax=None, scale_atoms=.5, title=None, numbering=False):
+    """
+    Show atoms function
+
+    Function to display atoms, especially in Jupyter notebooks.
+
+    Parameters
+    ----------
+    atoms : ASE atoms object
+        The atoms to be shown.
+    repeat : two ints, optional
+        Tiling of the image. Default is (1,1), ie. no tiling.
+    scans : ndarray, optional
+        List of scans to apply. Default is None.
+    plane : str
+        The projection plane.
+    ax : axes object
+        pyplot axes object.
+    scale_atoms : float
+        Scaling factor for the atom display sizes. Default is 0.5.
+    title : str
+        Title of the displayed image. Default is None.
+    numbering : bool
+        Option to set plot numbering. Default is False.
+    """
+
+    if ax is None:
+        fig, ax = plt.subplots()
+
+    axes = _plane2axes(plane)
+
+    atoms = atoms.copy()
+    cell = atoms.cell
+    atoms *= repeat + (1,)
+
+    for line in _cube:
+        cell_lines = np.array([np.dot(line[0], cell), np.dot(line[1], cell)])
+        ax.plot(cell_lines[:, axes[0]], cell_lines[:, axes[1]], 'k-')
+
+    if len(atoms) > 0:
+        positions = atoms.positions[:, axes[:2]]
+        order = np.argsort(atoms.positions[:, axes[2]])
+        positions = positions[order]
+
+        colors = jmol_colors[atoms.numbers[order]]
+
+        sizes = covalent_radii[atoms.numbers[order]] * scale_atoms
+
+        circles = []
+        for position, size in zip(positions, sizes):
+            circles.append(Circle(position, size))
+
+        coll = PatchCollection(circles, facecolors=colors, edgecolors='black')
+        ax.add_collection(coll)
+
+        ax.axis('equal')
+        ax.set_xlabel(plane[0] + ' [Å]')
+        ax.set_ylabel(plane[1] + ' [Å]')
+
+        ax.set_title(title)
+
+        if numbering:
+            for i, (position, size) in enumerate(zip(positions, sizes)):
+                ax.annotate('{}'.format(order[i]), xy=position, ha="center", va="center")
+
+    if scans is not None:
+        if not isinstance(scans, Iterable):
+            scans = [scans]
+
+        for scan in scans:
+            scan.add_to_mpl_plot(ax)
+
+    return ax
+
+def show_measurement_2d(measurement,
+                        ax=None,
+                        figsize=None,
+                        colorbar=False,
+                        cmap='gray',
+                        discrete_cmap=False,
+                        vmin=None,
+                        vmax=None,
+                        power=1.,
+                        **kwargs):
+    """
+    Show image function
+
+    Function to display an image.
+
+    Parameters
+    ----------
+    array : ndarray
+        Image array.
+    calibrations : tuple of calibration objects.
+        Spatial calibrations.
+    ax : axes object
+        pyplot axes object.
+    title : str, optional
+        Image title. Default is None.
+    colorbar : bool, optional
+        Option to show a colorbar. Default is False.
+    cmap : str, optional
+        Colormap name. Default is 'gray'.
+    figsize : float, pair of float, optional
+        Size of the figure in inches, either as a square for one number or a rectangle for two. Default is None.
+    scans : ndarray, optional
+        Array of scans. Default is None.
+    discrete : bool, optional
+        Option to discretize intensity values to integers. Default is False.
+    cbar_label : str, optional
+        Text label for the color bar. Default is None.
+    vmin : float, optional
+        Minimum of the intensity scale. Default is None.
+    vmax : float, optional
+        Maximum of the intensity scale. Default is None.
+    kwargs :
+        Remaining keyword arguments are passed to pyplot.
+    """
+
+    if ax is None:
+        fig, ax = plt.subplots(figsize=figsize)
+
+    calibrations = measurement.calibrations[-2:]
+    array = measurement.array[(0,) * (measurement.dimensions - 2) + (slice(None),) * 2]
+
+    if power != 1:
+        array = array ** power
+
+    extent = []
+    for calibration, num_elem in zip(calibrations, array.shape):
+        extent.append(calibration.offset)
+        extent.append(calibration.offset + num_elem * calibration.sampling)
+
+    if vmin is None:
+        vmin = np.min(array)
+        if discrete_cmap:
+            vmin -= .5
+
+    if vmax is None:
+        vmax = np.max(array)
+        if discrete_cmap:
+            vmax += .5
+
+    if discrete_cmap:
+        cmap = plt.get_cmap(cmap, np.max(array) - np.min(array) + 1)
+
+    im = ax.imshow(array.T, extent=extent, cmap=cmap, origin='lower', vmin=vmin, vmax=vmax, interpolation='nearest',
+                   **kwargs)
+
+    if colorbar:
+        cax = plt.colorbar(im, ax=ax, label=format_label(measurement))
+        if discrete_cmap:
+            cax.set_ticks(ticks=np.arange(np.min(array), np.max(array) + 1))
+
+    ax.set_xlabel(format_label(calibrations[-2]))
+    ax.set_ylabel(format_label(calibrations[-1]))
+
+    return ax, im
+
+
+def show_measurement_1d(measurement, ax=None, figsize=None, legend=False, title=None, **kwargs):
+    """
+    Show line function
+
+    Function to display a line scan.
+
+    Parameters
+    ----------
+    array : ndarray
+        Array of measurement values along a line.
+    calibration : calibration object
+        Spatial calibration for the line.
+    ax : axes object, optional
+        pyplot axes object.
+    title : str, optional
+        Title for the plot. Default is None.
+    legend : bool, optional
+        Option to display a plot legend. Default is False.
+    kwargs :
+       Remaining keyword arguments are passed to pyplot.
+    """
+
+    calibration = measurement.calibrations[0]
+    array = measurement.array
+    x = np.linspace(calibration.offset, calibration.offset + len(array) * calibration.sampling, len(array))
+
+    if ax is None:
+        fig, ax = plt.subplots(figsize=figsize)
+
+    lines = ax.plot(x, array, label=measurement.name, **kwargs)
+    ax.set_xlabel(format_label(calibration))
+    ax.set_ylabel(format_label(measurement))
+
+    if legend:
+        ax.legend()
+
+    return ax, lines[0]
```

### Comparing `abtem-1.0.0b8/abtem/visualize/utils.py` & `abtem-1.0.0b9/abtem/visualize/utils.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,72 +1,72 @@
-
-from colorsys import hls_to_rgb
-
-import numpy as np
-
-
-def format_label(calibration):
-    label = ''
-    if calibration.name:
-        label += f'{calibration.name}'
-
-    if calibration.units:
-        label += f' [{calibration.units}]'
-
-    return label
-
-
-def domain_coloring(z, fade_to_white=False, saturation=1.0, k=.5):
-    """
-    Domain coloring function.
-
-    Function to color a complex domain.
-
-    Parameters
-    ----------
-    z : ndarray, complex
-        Complex number to be colored.
-    fade_to_white : bool, optional
-        Option to fade the coloring to white instead of black. Default is False.
-    saturation : float, optional
-        RGB color saturation. Default is 1.0.
-    k : float, optional
-        Scaling factor for the coloring. Default is 0.5.
-    """
-
-    h = (np.angle(z) + np.pi) / (2 * np.pi) + 0.5
-    if fade_to_white:
-        r = k ** np.abs(z)
-    else:
-        r = 1 - k ** np.abs(z)
-    c = np.vectorize(hls_to_rgb)(h, r, saturation)
-    c = np.array(c).T
-
-    c = (c - c.min()) / c.ptp()
-    return c
-
-
-def _line_intersect_rectangle(point0, point1, lower_corner, upper_corner):
-    if point0[0] == point1[0]:
-        return (point0[0], lower_corner[1]), (point0[0], upper_corner[1])
-
-    m = (point1[1] - point0[1]) / (point1[0] - point0[0])
-
-    def y(x):
-        return m * (x - point0[0]) + point0[1]
-
-    def x(y):
-        return (y - point0[1]) / m + point0[0]
-
-    if y(0) < lower_corner[1]:
-        intersect0 = (x(lower_corner[1]), y(x(lower_corner[1])))
-    else:
-        intersect0 = (0, y(lower_corner[0]))
-
-    if y(upper_corner[0]) > upper_corner[1]:
-        intersect1 = (x(upper_corner[1]), y(x(upper_corner[1])))
-    else:
-        intersect1 = (upper_corner[0], y(upper_corner[0]))
-
-    return intersect0, intersect1
-
-
+
+from colorsys import hls_to_rgb
+
+import numpy as np
+
+
+def format_label(calibration):
+    label = ''
+    if calibration.name:
+        label += f'{calibration.name}'
+
+    if calibration.units:
+        label += f' [{calibration.units}]'
+
+    return label
+
+
+def domain_coloring(z, fade_to_white=False, saturation=1.0, k=.5):
+    """
+    Domain coloring function.
+
+    Function to color a complex domain.
+
+    Parameters
+    ----------
+    z : ndarray, complex
+        Complex number to be colored.
+    fade_to_white : bool, optional
+        Option to fade the coloring to white instead of black. Default is False.
+    saturation : float, optional
+        RGB color saturation. Default is 1.0.
+    k : float, optional
+        Scaling factor for the coloring. Default is 0.5.
+    """
+
+    h = (np.angle(z) + np.pi) / (2 * np.pi) + 0.5
+    if fade_to_white:
+        r = k ** np.abs(z)
+    else:
+        r = 1 - k ** np.abs(z)
+    c = np.vectorize(hls_to_rgb)(h, r, saturation)
+    c = np.array(c).T
+
+    c = (c - c.min()) / c.ptp()
+    return c
+
+
+def _line_intersect_rectangle(point0, point1, lower_corner, upper_corner):
+    if point0[0] == point1[0]:
+        return (point0[0], lower_corner[1]), (point0[0], upper_corner[1])
+
+    m = (point1[1] - point0[1]) / (point1[0] - point0[0])
+
+    def y(x):
+        return m * (x - point0[0]) + point0[1]
+
+    def x(y):
+        return (y - point0[1]) / m + point0[0]
+
+    if y(0) < lower_corner[1]:
+        intersect0 = (x(lower_corner[1]), y(x(lower_corner[1])))
+    else:
+        intersect0 = (0, y(lower_corner[0]))
+
+    if y(upper_corner[0]) > upper_corner[1]:
+        intersect1 = (x(upper_corner[1]), y(x(upper_corner[1])))
+    else:
+        intersect1 = (upper_corner[0], y(upper_corner[0]))
+
+    return intersect0, intersect1
+
+
```

### Comparing `abtem-1.0.0b8/abtem/visualize/widgets.py` & `abtem-1.0.0b9/abtem/visualize/widgets.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,91 +1,98 @@
-import asyncio
-from time import time
-
-import ipywidgets as widgets
-
-
-class Timer:
-    def __init__(self, timeout, callback):
-        self._timeout = timeout
-        self._callback = callback
-        self._task = asyncio.ensure_future(self._job())
-
-    async def _job(self):
-        await asyncio.sleep(self._timeout)
-        self._callback()
-
-    def cancel(self):
-        self._task.cancel()
-
-
-def debounce(wait):
-    """ Decorator that will postpone a function's
-        execution until after `wait` seconds
-        have elapsed since the last time it was invoked. """
-
-    def decorator(fn):
-        timer = None
-
-        def debounced(*args, **kwargs):
-            nonlocal timer
-
-            def call_it():
-                fn(*args, **kwargs)
-
-            if timer is not None:
-                timer.cancel()
-            timer = Timer(wait, call_it)
-
-        return debounced
-
-    return decorator
-
-
-def throttle(wait):
-    """ Decorator that prevents a function from being called
-        more than once every wait period. """
-
-    def decorator(fn):
-        time_of_last_call = 0
-        scheduled = False
-        new_args, new_kwargs = None, None
-
-        def throttled(*args, **kwargs):
-            nonlocal new_args, new_kwargs, time_of_last_call, scheduled
-
-            def call_it():
-                nonlocal new_args, new_kwargs, time_of_last_call, scheduled
-                time_of_last_call = time()
-                fn(*new_args, **new_kwargs)
-                scheduled = False
-
-            time_since_last_call = time() - time_of_last_call
-            new_args = args
-            new_kwargs = kwargs
-            if not scheduled:
-                new_wait = max(0, wait - time_since_last_call)
-                Timer(new_wait, call_it)
-                scheduled = True
-
-        return throttled
-
-    return decorator
-
-
-def quick_sliders(obj, continuous_update=True, **kwargs):
-    create_callback = lambda key: lambda change: setattr(obj, key, change['new'])
-
-    sliders = []
-    for key, value in kwargs.items():
-        slider = widgets.FloatSlider(value=getattr(obj, key),
-                                     min=value[0],
-                                     max=value[1],
-                                     step=value[2],
-                                     description=key,
-                                     continuous_update=continuous_update)
-
-        slider.observe(create_callback(key), 'value')
-
-        sliders += [slider]
-
-    return sliders
+import asyncio
+from time import time
+
+import ipywidgets as widgets
+
+
+class Timer:
+    def __init__(self, timeout, callback):
+        self._timeout = timeout
+        self._callback = callback
+        self._task = asyncio.ensure_future(self._job())
+
+    async def _job(self):
+        await asyncio.sleep(self._timeout)
+        self._callback()
+
+    def cancel(self):
+        self._task.cancel()
+
+
+def debounce(wait):
+    """ Decorator that will postpone a function's
+        execution until after `wait` seconds
+        have elapsed since the last time it was invoked. """
+
+    def decorator(fn):
+        timer = None
+
+        def debounced(*args, **kwargs):
+            nonlocal timer
+
+            def call_it():
+                fn(*args, **kwargs)
+
+            if timer is not None:
+                timer.cancel()
+            timer = Timer(wait, call_it)
+
+        return debounced
+
+    return decorator
+
+
+def throttle(wait):
+    """ Decorator that prevents a function from being called
+        more than once every wait period. """
+
+    def decorator(fn):
+        time_of_last_call = 0
+        scheduled = False
+        new_args, new_kwargs = None, None
+
+        def throttled(*args, **kwargs):
+            nonlocal new_args, new_kwargs, time_of_last_call, scheduled
+
+            def call_it():
+                nonlocal new_args, new_kwargs, time_of_last_call, scheduled
+                time_of_last_call = time()
+                fn(*new_args, **new_kwargs)
+                scheduled = False
+
+            time_since_last_call = time() - time_of_last_call
+            new_args = args
+            new_kwargs = kwargs
+            if not scheduled:
+                new_wait = max(0, wait - time_since_last_call)
+                Timer(new_wait, call_it)
+                scheduled = True
+
+        return throttled
+
+    return decorator
+
+
+def quick_sliders(obj, throttling=None, continuous_update=True, **kwargs):
+    def create_callback(key):
+        def callback(change):
+            setattr(obj, key, change['new'])
+
+        if throttling:
+            return throttle(throttling)(callback)
+        else:
+            return callback
+
+    sliders = []
+    for key, value in kwargs.items():
+        slider = widgets.FloatSlider(value=getattr(obj, key),
+                                     min=value[0],
+                                     max=value[1],
+                                     step=value[2],
+                                     description=key,
+                                     continuous_update=continuous_update)
+
+        slider.observe(create_callback(key), 'value')
+
+        sliders += [slider]
+
+    return sliders
```

### Comparing `abtem-1.0.0b8/abtem/waves.py` & `abtem-1.0.0b9/abtem/waves.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,1674 +1,1661 @@
-"""Module to describe electron waves and their propagation."""
-from copy import copy
-from numbers import Number
-from typing import Union, Sequence, Tuple
-
-import h5py
-import numpy as np
-from ase import Atoms
-
-from abtem.base_classes import Grid, Accelerator, cache_clear_callback, Cache, cached_method, \
-    HasGridMixin, HasAcceleratorMixin, AntialiasFilter, Event
-from abtem.detect import AbstractDetector
-from abtem.device import get_array_module, get_device_function, asnumpy, get_array_module_from_device, \
-    copy_to_device, get_available_memory, HasDeviceMixin
-from abtem.measure import calibrations_from_grid, Measurement, block_zeroth_order_spot, probe_profile
-from abtem.potentials import Potential, AbstractPotential, AbstractTDSPotentialBuilder, AbstractPotentialBuilder
-from abtem.scan import AbstractScan, GridScan
-from abtem.transfer import CTF
-from abtem.utils import polar_coordinates, ProgressBar, spatial_frequencies, subdivide_into_batches, periodic_crop, \
-    fft_crop, fft_interpolate_2d
-
-
-class FresnelPropagator:
-    """
-    Fresnel propagator object.
-
-    This class is used for propagating a wave function object using the near-field approximation (Fresnel diffraction).
-    The array representing the Fresnel propagator function is cached.
-    """
-
-    def __init__(self):
-        self._cache = Cache(1)
-
-    @cached_method('_cache')
-    def _evaluate_propagator_array(self,
-                                   gpts: Tuple[int, int],
-                                   sampling: Tuple[float, float],
-                                   wavelength: float,
-                                   dz: float,
-                                   xp) -> np.ndarray:
-        complex_exponential = get_device_function(xp, 'complex_exponential')
-        kx = xp.fft.fftfreq(gpts[0], sampling[0]).astype(xp.float32)
-        ky = xp.fft.fftfreq(gpts[1], sampling[1]).astype(xp.float32)
-        f = (complex_exponential(-(kx ** 2)[:, None] * np.pi * wavelength * dz) *
-             complex_exponential(-(ky ** 2)[None] * np.pi * wavelength * dz))
-
-        return f * AntialiasFilter().get_mask(gpts, sampling, xp)
-
-    def propagate(self, waves: Union['Waves', 'SMatrixArray'], dz: float) -> Union['Waves', 'SMatrixArray']:
-        """
-        Propagate wave functions or scattering matrix.
-
-        Parameters
-        ----------
-        waves : Waves or SMatrixArray object
-            Wave function or scattering matrix to propagate.
-        dz : float
-            Propagation distance [Å].
-
-        Returns
-        -------
-        Waves or SMatrixArray object
-            The propagated wave functions.
-        """
-        fft2_convolve = get_device_function(get_array_module(waves.array), 'fft2_convolve')
-
-        propagator_array = self._evaluate_propagator_array(waves.grid.gpts,
-                                                           waves.grid.sampling,
-                                                           dz,
-                                                           waves.wavelength,
-                                                           get_array_module(waves.array))
-
-        fft2_convolve(waves._array, propagator_array, overwrite_x=True)
-        waves._antialiasing_aperture = 2 / 3.
-
-        return waves
-
-
-def _multislice(waves: Union['Waves', 'SMatrixArray'],
-                potential: AbstractPotential,
-                propagator: FresnelPropagator = None,
-                pbar: Union[ProgressBar, bool] = True,
-                max_batch=1,
-                ) -> Union['Waves', 'SMatrixArray']:
-    waves.grid.match(potential)
-    waves.accelerator.check_is_defined()
-    waves.grid.check_is_defined()
-
-    if propagator is None:
-        propagator = FresnelPropagator()
-
-    if isinstance(pbar, bool):
-        pbar = ProgressBar(total=len(potential), desc='Multislice', disable=not pbar)
-
-    pbar.reset()
-    if max_batch == 1:
-        for start, end, t in potential.generate_transmission_functions(energy=waves.energy, max_batch=1):
-            waves = t.transmit(waves)
-            waves = propagator.propagate(waves, t.thickness)
-            pbar.update(1)
-    else:
-        for start, end, t_chunk in potential.generate_transmission_functions(energy=waves.energy, max_batch=max_batch):
-            for _, __, t_slice in t_chunk.generate_slices(max_batch=1):
-                waves = t_slice.transmit(waves)
-                waves = propagator.propagate(waves, t_slice.thickness)
-
-            pbar.update(end - start)
-
-    pbar.refresh()
-    return waves
-
-
-class _WavesLike(HasGridMixin, HasAcceleratorMixin):
-
-    def __init__(self, antialiasing_aperture=None):
-        if antialiasing_aperture is None:
-            antialiasing_aperture = AntialiasFilter.cutoff
-        self._antialiasing_aperture = antialiasing_aperture
-
-    @property
-    def antialiasing_aperture(self):
-        return self._antialiasing_aperture
-
-    @property
-    def cutoff_scattering_angles(self):
-        kcut = 1 / max(self.sampling) / 2 * self.antialiasing_aperture
-        kcut = (np.ceil(2 * self.extent[0] * kcut) / (2 * self.extent[0]) * self.wavelength * 1e3,
-                np.ceil(2 * self.extent[1] * kcut) / (2 * self.extent[1]) * self.wavelength * 1e3)
-        return kcut
-
-    @property
-    def rectangle_cutoff_scattering_angles(self):
-        rolloff = AntialiasFilter.rolloff
-        kcut = (1 / max(self.sampling) / 2 * self.antialiasing_aperture - rolloff) / np.sqrt(2)
-        kcut = (np.floor(2 * self.extent[0] * kcut) / (2 * self.extent[0]) * self.wavelength * 1e3,
-                np.floor(2 * self.extent[1] * kcut) / (2 * self.extent[1]) * self.wavelength * 1e3)
-        return kcut
-
-    @property
-    def angular_sampling(self):
-        self.grid.check_is_defined()
-        self.accelerator.check_is_defined()
-        return tuple([1 / l * self.wavelength * 1e3 for l in self.extent])
-
-    def downsampled_gpts(self, max_angle):
-        if max_angle is None:
-            gpts = self.gpts
-        elif isinstance(max_angle, str):
-            if max_angle == 'limit':
-                cutoff_scattering_angle = self.cutoff_scattering_angles
-            elif max_angle == 'valid':
-                cutoff_scattering_angle = self.rectangle_cutoff_scattering_angles
-            else:
-                raise RuntimeError()
-
-            angular_sampling = self.angular_sampling
-
-            gpts = (int(round(cutoff_scattering_angle[0] / angular_sampling[0] * 2)),
-                    int(round(cutoff_scattering_angle[1] / angular_sampling[1] * 2)))
-        elif isinstance(max_angle, Number):
-            gpts = tuple([int(2 * np.floor(max_angle / d)) + 1 for n, d in zip(self.gpts, self.angular_sampling)])
-        else:
-            raise RuntimeError()
-
-        return gpts
-
-
-class Waves(_WavesLike):
-    """
-    Waves object
-
-    The waves object can define a batch of arbitrary 2D wave functions defined by a complex numpy array.
-
-    Parameters
-    ----------
-    extent : one or two float
-        Lateral extent of wave function [Å].
-    sampling : one or two float
-        Lateral sampling of wave functions [1 / Å].
-    energy : float
-        Electron energy [eV].
-    """
-
-    def __init__(self,
-                 array: np.ndarray,
-                 extent: Union[float, Sequence[float]] = None,
-                 sampling: Union[float, Sequence[float]] = None,
-                 energy: float = None,
-                 antialiasing_aperture: float = None):
-
-        if len(array.shape) < 2:
-            raise RuntimeError('Wave function array should be have 2 dimensions or more')
-
-        self._array = array
-
-        self._grid = Grid(extent=extent, gpts=array.shape[-2:], sampling=sampling, lock_gpts=True)
-        self._accelerator = Accelerator(energy=energy)
-
-        super().__init__(antialiasing_aperture=antialiasing_aperture)
-
-    def __len__(self):
-        return len(self.array)
-
-    @property
-    def array(self) -> np.ndarray:
-        """Array representing the wave functions."""
-        return self._array
-
-    def intensity(self) -> Measurement:
-        """
-        Calculate the intensity of the wave functions at the image plane.
-
-        Returns
-        -------
-        Measurement
-            The wave function intensity.
-        """
-
-        calibrations = calibrations_from_grid(self.grid.gpts, self.grid.sampling, ['x', 'y'])
-        # array = np.squeeze(self.array)
-        array = self.array
-
-        calibrations = (None,) * (len(array.shape) - 2) + calibrations
-        abs2 = get_device_function(get_array_module(self.array), 'abs2')
-        return Measurement(abs2(array), calibrations)
-
-    def downsample(self, max_angle='valid', return_fourier_space=False):
-        xp = get_array_module(self.array)
-        fft2 = get_device_function(xp, 'fft2')
-        ifft2 = get_device_function(xp, 'ifft2')
-        array = fft2(self.array, overwrite_x=False)
-
-        gpts = self.downsampled_gpts(max_angle)
-
-        if gpts != self.gpts:
-            array = fft_crop(array, self.array.shape[:-2] + gpts)
-
-        antialiasing_aperture = min(self.antialiasing_aperture * min(self.gpts[0] / gpts[0], self.gpts[1] / gpts[1]),
-                                    1.)
-        if return_fourier_space:
-            return Waves(array, extent=self.extent, energy=self.energy, antialiasing_aperture=antialiasing_aperture)
-        else:
-            return Waves(ifft2(array), extent=self.extent, energy=self.energy,
-                         antialiasing_aperture=antialiasing_aperture)
-
-    def far_field(self, max_angle='valid', in_place=False):
-        return self.downsample(max_angle=max_angle, return_fourier_space=True)
-
-    def diffraction_pattern(self, max_angle='valid', block_zeroth_order=False) -> Measurement:
-        """
-        Calculate the intensity of the wave functions at the diffraction plane.
-
-        Returns
-        -------
-        Measurement object
-            The intensity of the diffraction pattern(s).
-        """
-        xp = get_array_module(self.array)
-        abs2 = get_device_function(xp, 'abs2')
-        waves = self.far_field(max_angle)
-
-        calibrations = calibrations_from_grid(waves.gpts,
-                                              waves.sampling,
-                                              names=['alpha_x', 'alpha_y'],
-                                              units='mrad',
-                                              scale_factor=self.wavelength * 1000,
-                                              fourier_space=True)
-
-        # array = np.squeeze(waves.array)
-        array = waves.array
-        calibrations = (None,) * (len(array.shape) - 2) + calibrations
-
-        pattern = np.fft.fftshift(asnumpy(abs2(array)), axes=(-1, -2))
-
-        measurement = Measurement(pattern, calibrations)
-
-        if block_zeroth_order:
-            block_zeroth_order_spot(measurement)
-
-        return measurement
-
-    def apply_ctf(self, ctf: CTF = None, in_place=False, **kwargs):
-        """
-        Apply the aberrations defined by a CTF object to wave function.
-
-        Parameters
-        ----------
-        ctf : CTF
-            Contrast Transfer Function object to be applied.
-        kwargs :
-            Provide the aberration coefficients as keyword arguments.
-
-        Returns
-        -------
-        Waves object
-            The wave functions with aberrations applied.
-        """
-
-        xp = get_array_module(self.array)
-        fft2_convolve = get_device_function(get_array_module(self.array), 'fft2_convolve')
-
-        if ctf is None:
-            ctf = CTF(**kwargs)
-
-        if not ctf.accelerator.energy:
-            ctf.accelerator.match(self.accelerator)
-
-        self.accelerator.check_is_defined()
-        self.grid.check_is_defined()
-
-        kx, ky = spatial_frequencies(self.grid.gpts, self.grid.sampling)
-        alpha, phi = polar_coordinates(xp.asarray(kx * self.wavelength), xp.asarray(ky * self.wavelength))
-        kernel = ctf.evaluate(alpha, phi)
-
-        return self.__class__(fft2_convolve(self.array, kernel, overwrite_x=in_place),
-                              extent=self.extent,
-                              energy=self.energy)
-
-    def multislice(self,
-                   potential: AbstractPotential,
-                   pbar: Union[ProgressBar, bool] = True,
-                   detector=None,
-                   potential_chunks=1) -> 'Waves':
-        """
-        Propagate and transmit wave function through the provided potential.
-
-        Parameters
-        ----------
-        potential : Potential
-            The potential through which to propagate the wave function.
-        pbar : bool
-            If true, display a progress bar.
-
-        Returns
-        -------
-        Waves object
-            Wave function at the exit plane of the potential.
-        """
-
-        self.grid.match(potential)
-
-        propagator = FresnelPropagator()
-
-        result = None
-        if isinstance(potential, AbstractTDSPotentialBuilder):
-            if len(potential.frozen_phonons) > 1:
-                xp = get_array_module(self.array)
-                n = len(potential.frozen_phonons)
-
-                if detector:
-                    result = detector.allocate_measurement(self, self.array.shape[:-2])
-                else:
-                    if n > 1:
-                        if self.array.shape[0] == 1:
-                            out_array = xp.zeros((n,) + self.array.shape[1:], dtype=xp.complex64)
-                        else:
-                            out_array = xp.zeros((n,) + self.array.shape, dtype=xp.complex64)
-                    else:
-                        out_array = xp.zeros(self.array.shape, dtype=xp.complex64)
-
-                    result = self.__class__(out_array,
-                                            extent=self.extent,
-                                            energy=self.energy,
-                                            antialiasing_aperture=2 / 3.)
-
-                tds_pbar = ProgressBar(total=n, desc='TDS', disable=(not pbar) or (n == 1))
-                multislice_pbar = ProgressBar(total=len(potential), desc='Multislice', disable=not pbar)
-
-                for i, potential_config in enumerate(potential.generate_frozen_phonon_potentials(pbar=pbar)):
-                    multislice_pbar.reset()
-
-                    exit_waves = _multislice(copy(self),
-                                             potential_config,
-                                             propagator=propagator,
-                                             pbar=multislice_pbar,
-                                             max_batch=potential_chunks)
-
-                    if detector:
-                        result._array += asnumpy(detector.detect(exit_waves))
-                    else:
-                        result._array[i] = exit_waves.array
-
-                    tds_pbar.update(1)
-
-                multislice_pbar.close()
-                tds_pbar.close()
-
-        if result is None:
-            result = _multislice(self, potential, propagator, pbar, max_batch=potential_chunks)
-
-            if detector:
-                result = detector.detect(result)
-
-        return result
-
-    def write(self, path: str):
-        """
-        Write wave functions to a hdf5 file.
-
-        path : str
-            The path to write the file.
-        """
-
-        with h5py.File(path, 'w') as f:
-            f.create_dataset('array', data=self.array)
-            f.create_dataset('energy', data=self.energy)
-            f.create_dataset('extent', data=self.extent)
-
-    @classmethod
-    def read(cls, path: str) -> 'Waves':
-        """
-        Read wave functions from a hdf5 file.
-
-        path : str
-            The path to read the file.
-        """
-
-        with h5py.File(path, 'r') as f:
-            datasets = {}
-            for key in f.keys():
-                datasets[key] = f.get(key)[()]
-
-        return cls(array=datasets['array'], extent=datasets['extent'], energy=datasets['energy'])
-
-    def __getitem__(self, item):
-        if len(self.array.shape) <= self.grid.dimensions:
-            raise RuntimeError()
-        return self.__class__(array=self._array[item], extent=self.extent, energy=self.energy)
-
-    def show(self, ax=None, **kwargs):
-        """
-        Show the wave function.
-
-        kwargs :
-            Additional keyword arguments for the abtem.plot.show_image function.
-        """
-        return self.intensity().show(ax=ax, **kwargs)
-
-    def __copy__(self):
-        new_copy = self.__class__(array=self._array.copy())
-        new_copy._grid = copy(self.grid)
-        new_copy._accelerator = copy(self.accelerator)
-        return new_copy
-
-    def copy(self):
-        """Make a copy."""
-        return copy(self)
-
-
-class PlaneWave(_WavesLike, HasDeviceMixin):
-    """
-    Plane wave object
-
-    The plane wave object is used for building plane waves.
-
-    Parameters
-    ----------
-    extent : two float
-        Lateral extent of wave function [Å].
-    gpts : two int
-        Number of grid points describing the wave function.
-    sampling : two float
-        Lateral sampling of wave functions [1 / Å].
-    energy : float
-        Electron energy [eV].
-    device : str
-        The plane waves will be build on this device.
-    """
-
-    def __init__(self,
-                 extent: Union[float, Sequence[float]] = None,
-                 gpts: Union[int, Sequence[int]] = None,
-                 sampling: Union[float, Sequence[float]] = None,
-                 energy: float = None,
-                 device: str = 'cpu'):
-        self._grid = Grid(extent=extent, gpts=gpts, sampling=sampling)
-        self._accelerator = Accelerator(energy=energy)
-        self._device = device
-
-        super().__init__()
-
-    def multislice(self,
-                   potential: Union[AbstractPotential, Atoms],
-                   pbar: bool = True,
-                   potential_chunks=1) -> Waves:
-        """
-        Build plane wave function and propagate it through the potential. The grid of the two will be matched.
-
-        Parameters
-        ----------
-        potential : Potential or Atoms object
-            The potential through which to propagate the wave function.
-        pbar : bool, optional
-            Display a progress bar. Default is True.
-
-        Returns
-        -------
-        Waves object
-            Wave function at the exit plane of the potential.
-        """
-
-        if isinstance(potential, Atoms):
-            potential = Potential(atoms=potential)
-        potential.grid.match(self)
-
-        return self.build().multislice(potential, pbar=pbar, potential_chunks=potential_chunks)
-
-    def build(self) -> Waves:
-        """Build the plane wave function as a Waves object."""
-        xp = get_array_module_from_device(self._device)
-        self.grid.check_is_defined()
-        array = xp.ones((1, self.gpts[0], self.gpts[1]), dtype=xp.complex64)
-        return Waves(array, extent=self.extent, energy=self.energy)
-
-    def __copy__(self, a) -> 'PlaneWave':
-        return self.__class__(extent=self.extent, gpts=self.gpts, sampling=self.sampling, energy=self.energy)
-
-    def copy(self):
-        """Make a copy."""
-        return copy(self)
-
-
-class Probe(_WavesLike, HasDeviceMixin):
-    """
-    Probe wave function object
-
-    The probe object can represent a stack of electron probe wave function for simulating scanning transmission
-    electron microscopy.
-
-    See the docs of abtem.transfer.CTF for a description of the parameters related to the contrast transfer function.
-
-    Parameters
-    ----------
-    semiangle_cutoff : float
-        Convergence semi-angle [mrad].
-    rolloff : float
-        Softens the cutoff. A value of 0 gives a hard cutoff, while 1 gives the softest possible cutoff.
-    focal_spread : float
-        The focal spread of the probe.
-    angular_spread : float
-        The angular spread of the probe
-    ctf_parameters : dict
-        The parameters describing the phase aberrations using polar notation or an alias.
-    extent : two float, optional
-        Lateral extent of wave functions [Å].
-    gpts : two int, optional
-        Number of grid points describing the wave functions.
-    sampling : two float, optional
-        Lateral sampling of wave functions [1 / Å].
-    energy : float, optional
-        Electron energy [eV].
-    device : str
-        The probe wave functions will be build on this device.
-    kwargs :
-        Provide the aberration coefficients as keyword arguments.
-    """
-
-    def __init__(self,
-                 extent: Union[float, Sequence[float]] = None,
-                 gpts: Union[int, Sequence[int]] = None,
-                 sampling: Union[float, Sequence[float]] = None,
-                 energy: float = None,
-                 ctf=None,
-                 device='cpu',
-                 **kwargs):
-
-        if ctf is None:
-            ctf = CTF(energy=energy, **kwargs)
-
-        if ctf.energy is None:
-            ctf.energy = energy
-
-        if ctf.energy != energy:
-            raise RuntimeError()
-
-        self._ctf = ctf
-        self._accelerator = self._ctf._accelerator
-
-        self._grid = Grid(extent=extent, gpts=gpts, sampling=sampling)
-
-        self.changed = Event()
-
-        self._ctf.changed.register(self.changed.notify)
-        self._grid.changed.register(self.changed.notify)
-        self._accelerator.changed.register(self.changed.notify)
-
-        self._device = device
-
-        self._ctf_cache = Cache(1)
-        self.changed.register(cache_clear_callback(self._ctf_cache))
-
-        super().__init__()
-
-    @property
-    def ctf(self) -> CTF:
-        """Probe contrast transfer function."""
-        return self._ctf
-
-    def _fourier_translation_operator(self, positions):
-        xp = get_array_module(positions)
-        complex_exponential = get_device_function(xp, 'complex_exponential')
-
-        kx, ky = spatial_frequencies(self.grid.gpts, self.grid.sampling)
-        kx = kx.reshape((1, -1, 1))
-        ky = ky.reshape((1, 1, -1))
-        kx = xp.asarray(kx)
-        ky = xp.asarray(ky)
-        positions = xp.asarray(positions)
-        x = positions[:, 0].reshape((-1,) + (1, 1))
-        y = positions[:, 1].reshape((-1,) + (1, 1))
-
-        return complex_exponential(2 * np.pi * kx * x) * complex_exponential(2 * np.pi * ky * y)
-
-    @cached_method('_ctf_cache')
-    def _evaluate_ctf(self, xp):
-        kx, ky = spatial_frequencies(self.grid.gpts, self.grid.sampling)
-        alpha, phi = polar_coordinates(xp.asarray(kx * self.wavelength), xp.asarray(ky * self.wavelength))
-        return self._ctf.evaluate(alpha, phi)
-
-    def build(self, positions: Sequence[Sequence[float]] = None) -> Waves:
-        """
-        Build probe wave functions at the provided positions.
-
-        Parameters
-        ----------
-        positions : array of xy-positions
-            Positions of the probe wave functions
-
-        Returns
-        -------
-        Waves object
-            Probe wave functions as a Waves object.
-        """
-
-        self.grid.check_is_defined()
-        self.accelerator.check_is_defined()
-        xp = get_array_module_from_device(self._device)
-        fft2 = get_device_function(xp, 'fft2')
-
-        if positions is None:
-            positions = xp.array((self.extent[0] / 2, self.extent[1] / 2), dtype=xp.float32)
-        else:
-            positions = xp.array(positions, dtype=xp.float32)
-
-        if len(positions.shape) == 1:
-            positions = xp.expand_dims(positions, axis=0)
-
-        array = fft2(self._evaluate_ctf(xp) * self._fourier_translation_operator(positions), overwrite_x=True)
-
-        return Waves(array, extent=self.extent, energy=self.energy)
-
-    def multislice(self, positions: Sequence[Sequence[float]], potential: AbstractPotential, pbar=True) -> Waves:
-        """
-        Build probe wave functions at the provided positions and propagate them through the potential.
-
-        Parameters
-        ----------
-        positions : array of xy-positions
-            Positions of the probe wave functions.
-        potential : Potential or Atoms object
-            The scattering potential.
-        pbar : bool, optional
-            Display progress bars. Default is True.
-
-        Returns
-        -------
-        Waves object
-            Probe exit wave functions as a Waves object.
-        """
-
-        if isinstance(potential, Atoms):
-            potential = Potential(potential)
-
-        self.grid.match(potential)
-        exit_probes = _multislice(self.build(positions), potential, None, pbar)
-        exit_probes._antialiasing_aperture = 2 / 3.
-        return exit_probes
-
-    def _generate_probes(self, scan: AbstractScan, potential: Union[AbstractPotential, Atoms], max_batch: int):
-        if not isinstance(max_batch, int):
-            memory_per_wave = 2 * 4 * np.prod(self.gpts)
-            available_memory = get_available_memory(self._device)
-            max_batch = min(int(available_memory * .4 / memory_per_wave), 32)
-
-        for indices, positions in scan.generate_positions(max_batch=max_batch):
-            yield indices, self.multislice(positions, potential, pbar=False)
-
-    def _generate_tds_probes(self, scan, potential, max_batch, pbar):
-        tds_bar = ProgressBar(total=len(potential.frozen_phonons), desc='TDS',
-                              disable=(not pbar) or (len(potential.frozen_phonons) == 1))
-        potential_pbar = ProgressBar(total=len(potential), desc='Potential', disable=not pbar)
-
-        for potential_config in potential.generate_frozen_phonon_potentials(pbar=potential_pbar):
-            yield self._generate_probes(scan, potential_config, max_batch)
-            tds_bar.update(1)
-
-        potential_pbar.close()
-        tds_bar.refresh()
-        tds_bar.close()
-
-    def scan(self,
-             scan: AbstractScan,
-             detectors: Union[AbstractDetector, Sequence[AbstractDetector]],
-             potential: Union[Atoms, AbstractPotential],
-             max_batch: int = None,
-             pbar: bool = True) -> dict:
-
-        """
-        Raster scan the probe across the potential and record a measurement for each detector.
-
-        Parameters
-        ----------
-        scan : Scan object
-            Scan object defining the positions of the probe wave functions.
-        detectors : List of detector objects
-            The detectors recording the measurements.
-        potential : Potential
-            The potential to scan the probe over.
-        max_batch : int, optional
-            The probe batch size. Larger batches are faster, but require more memory. Default is None.
-        pbar : bool, optional
-            Display progress bars. Default is True.
-
-        Returns
-        -------
-        dict
-            Dictionary of measurements with keys given by the detector.
-        """
-
-        self.grid.match(potential.grid)
-        self.grid.check_is_defined()
-
-        if isinstance(detectors, AbstractDetector):
-            detectors = [detectors]
-
-        scan_bar = ProgressBar(total=len(scan), desc='Scan', disable=not pbar)
-
-        if isinstance(potential, AbstractTDSPotentialBuilder):
-            probe_generators = self._generate_tds_probes(scan, potential, max_batch, pbar)
-        else:
-            if isinstance(potential, AbstractPotentialBuilder):
-                potential = potential.build(pbar=True)
-
-            probe_generators = [self._generate_probes(scan, potential, max_batch)]
-
-        measurements = {}
-        for probe_generator in probe_generators:
-            scan_bar.reset()
-            for indices, exit_probes in probe_generator:
-
-                for detector in detectors:
-                    new_measurement = detector.detect(exit_probes)
-
-                    if isinstance(potential, AbstractTDSPotentialBuilder):
-                        new_measurement /= len(potential.frozen_phonons)
-
-                    try:
-                        scan.insert_new_measurement(measurements[detector], indices, new_measurement)
-                    except KeyError:
-                        measurements[detector] = detector.allocate_measurement(exit_probes, scan)
-                        scan.insert_new_measurement(measurements[detector], indices, new_measurement)
-
-                scan_bar.update(len(indices))
-
-            scan_bar.refresh()
-
-        scan_bar.close()
-        return measurements
-
-    def profile(self, angle=0.):
-        self.grid.check_is_defined()
-        measurement = self.build((self.extent[0] / 2, self.extent[1] / 2)).intensity()
-        return probe_profile(measurement, angle=angle)
-
-    def interact(self, sliders=None, profile=False):
-        from abtem.visualize.bqplot import show_measurement_1d, show_measurement_2d
-        from abtem.visualize.widgets import quick_sliders
-        import ipywidgets as widgets
-
-        if profile:
-            figure, callback = show_measurement_1d(lambda: [self.profile()])
-        else:
-            figure, callback = show_measurement_2d(lambda: self.build().intensity())
-
-        self.changed.register(callback)
-
-        if sliders:
-            sliders = quick_sliders(self.ctf, **sliders)
-            return widgets.HBox([figure, widgets.VBox(sliders)])
-        else:
-            return figure
-
-    def __copy__(self):
-        return self.__class__(gpts=self.gpts,
-                              extent=self.extent,
-                              sampling=self.sampling,
-                              energy=self.energy,
-                              ctf=self.ctf.copy(),
-                              device=self.device)
-
-    def copy(self):
-        return copy(self)
-
-    def show(self, **kwargs):
-        """
-        Show the probe wave function.
-
-        Parameters
-        ----------
-        angle : float, optional
-            Angle along which the profile is shown [deg]. Default is 0 degrees.
-        kwargs : Additional keyword arguments for the abtem.plot.show_image function.
-        """
-        self.grid.check_is_defined()
-        return self.build((self.extent[0] / 2, self.extent[1] / 2)).intensity().show(**kwargs)
-
-
-class SMatrixArray(_WavesLike, HasDeviceMixin):
-    """
-    Scattering matrix array object.
-
-    The scattering matrix array object represents a plane wave expansion of a probe, it is used for STEM simulations
-    with the PRISM algorithm.
-
-    Parameters
-    ----------
-    array : 3d array
-        The array representation of the scattering matrix.
-    expansion_cutoff : float
-        The angular cutoff of the plane wave expansion [mrad].
-    energy : float
-        Electron energy [eV].
-    interpolation : one or two int
-        Interpolation factor.
-    k : 2d array
-        The spatial frequencies of each plane in the plane wave expansion.
-    ctf : CTF object, optional
-        The probe contrast transfer function. Default is None.
-    extent : one or two float, optional
-        Lateral extent of wave functions [Å]. Default is None (inherits extent from the potential).
-    sampling : one or two float, optional
-        Lateral sampling of wave functions [1 / Å]. Default is None (inherits sampling from the potential).
-    device : str, optional
-        The calculations will be carried out on this device. Default is 'cpu'.
-    """
-
-    def __init__(self,
-                 array: np.ndarray,
-                 expansion_cutoff: float,
-                 energy: float,
-                 k: np.ndarray,
-                 interpolation: int = None,
-                 ctf: CTF = None,
-                 sampling: Union[float, Sequence[float]] = None,
-                 extent: Union[float, Sequence[float]] = None,
-                 periodic: bool = True,
-                 offset: Sequence[float] = None,
-                 cropped_shape: Tuple[int, int] = None,
-                 antialiasing_aperture: float = None,
-                 device: str = 'cpu'):
-
-        if ctf is None:
-            ctf = CTF()
-
-        if ctf.energy is None:
-            ctf.energy = energy
-
-        if (ctf.energy != energy):
-            raise RuntimeError
-
-        self._ctf = ctf
-        self._accelerator = self._ctf._accelerator
-
-        self._grid = Grid(extent=extent, gpts=array.shape[-2:], sampling=sampling, lock_gpts=True)
-        self.changed = Event()
-
-        self._ctf.changed.register(self.changed.notify)
-        self._grid.changed.register(self.changed.notify)
-        self._accelerator.changed.register(self.changed.notify)
-
-        self._device = device
-
-        self._array = array
-        self._antialiasing_aperture = antialiasing_aperture
-
-        self._expansion_cutoff = expansion_cutoff
-        self._k = k
-        self._periodic = periodic
-
-        if offset is None:
-            offset = (0, 0)
-
-        self._offset = np.array(offset, dtype=np.int)
-
-        if (cropped_shape is None) & (interpolation is not None):
-            cropped_shape = (self.gpts[0] // interpolation, self.gpts[1] // interpolation)
-
-        self._cropped_shape = cropped_shape
-
-        super().__init__(antialiasing_aperture=antialiasing_aperture)
-
-    @property
-    def ctf(self) -> CTF:
-        """Probe contrast transfer function."""
-        return self._ctf
-
-    @property
-    def array(self) -> np.ndarray:
-        """Array representing the scattering matrix."""
-        return self._array
-
-    @property
-    def antialiasing_aperture(self):
-        return self._antialiasing_aperture
-
-    @property
-    def k(self) -> np.ndarray:
-        """The spatial frequencies of each wave in the plane wave expansion."""
-        return self._k
-
-    @property
-    def expansion_cutoff(self) -> float:
-        """Expansion cutoff."""
-        return self._expansion_cutoff
-
-    @property
-    def periodic(self):
-        return self._periodic
-
-    @property
-    def cropped_grid(self):
-        return Grid(gpts=self.cropped_shape, sampling=self.sampling, lock_gpts=True)
-
-    @property
-    def cropped_shape(self) -> Tuple[int, int]:
-        """The grid of the interpolated scattering matrix."""
-        return self._cropped_shape
-
-    @property
-    def offset(self):
-        return self._offset
-
-    def __len__(self) -> int:
-        """Number of plane waves in expansion."""
-        return len(self._array)
-
-    def _raise_not_periodic(self):
-        raise RuntimeError('not implemented for non-periodic/cropped scattering matrices')
-
-    def downsample(self, max_angle='limit', normalization=None):
-        if not self.periodic:
-            self._raise_not_periodic()
-
-        xp = get_array_module(self.array)
-        gpts = next(self._generate_partial(1, pbar=False))[2].downsample(max_angle).gpts
-
-        new_array = xp.zeros((len(self.array),) + gpts, dtype=self.array.dtype)
-        max_batch = self._max_batch_expansion()
-
-        for start, end, partial_s_matrix in self._generate_partial(max_batch, pbar=False):
-            downsampled = partial_s_matrix.downsample(max_angle)
-            new_array[start:end] = copy_to_device(downsampled.array, xp)
-
-        if self.cropped_shape == self.gpts:
-            cropped_shape = gpts
-        else:
-            cropped_shape = tuple(n // (self.gpts[i] // self.cropped_shape[i]) for i, n in enumerate(gpts))
-
-        antialiasing_aperture = downsampled.antialiasing_aperture
-
-        return self.__class__(array=new_array,
-                              expansion_cutoff=self._expansion_cutoff,
-                              k=self.k.copy(),
-                              ctf=self.ctf,
-                              extent=self.extent,
-                              energy=self.energy,
-                              periodic=self.periodic,
-                              offset=self._offset,
-                              cropped_shape=cropped_shape,
-                              antialiasing_aperture=antialiasing_aperture,
-                              device=self.device)
-
-    def crop_to_scan(self, scan):
-
-        if not isinstance(scan, GridScan):
-            raise NotImplementedError()
-
-        crop_corner, size = self._get_requisite_crop(np.array([scan.start, scan.end]))
-        new_array = periodic_crop(self.array, crop_corner, size)
-
-        return self.__class__(array=new_array,
-                              expansion_cutoff=self._expansion_cutoff,
-                              interpolation=1,
-                              k=self.k.copy(),
-                              ctf=self.ctf,
-                              sampling=self.sampling,
-                              energy=self.energy,
-                              periodic=False,
-                              offset=crop_corner,
-                              cropped_shape=self.cropped_shape,
-                              device=self.device)
-
-    def _max_batch_expansion(self):
-        memory_per_wave = 2 * 4 * self.gpts[0] * self.gpts[1]
-        available_memory = .2 * get_available_memory(self._device)
-        return min(int(available_memory / memory_per_wave), len(self))
-
-    def _max_batch_probes(self):
-        max_batch_plane_waves = self._max_batch_expansion()
-        memory_per_wave = 2 * 4 * self.cropped_shape[0] * self.cropped_shape[1]
-        memory_per_plane_wave_batch = 2 * 4 * self.gpts[0] * self.gpts[1] * max_batch_plane_waves
-        available_memory = .2 * get_available_memory(self._device) - memory_per_plane_wave_batch
-        return max(min(int(available_memory / memory_per_wave), 1024), 1)
-
-    def _generate_partial(self, max_batch: int = None, pbar: Union[ProgressBar, bool] = True):
-        if max_batch is None:
-            n_batches = 1
-        else:
-            n_batches = (len(self) + (-len(self) % max_batch)) // max_batch
-
-        if isinstance(pbar, bool):
-            pbar = ProgressBar(total=len(self), desc='Plane waves', disable=(not pbar) or (n_batches == 1))
-            close_pbar = True
-        else:
-            pbar.reset()
-            close_pbar = False
-
-        batch_sizes = subdivide_into_batches(len(self), n_batches)
-
-        xp = get_array_module_from_device(self._device)
-
-        if xp != get_array_module(self.array):
-            stream = xp.cuda.Stream(non_blocking=False)
-            partial_array = xp.empty((batch_sizes[0],) + self.gpts, dtype=xp.complex64)
-
-        else:
-            stream = None
-            partial_array = None
-
-        n = 0
-        for batch_size in batch_sizes:
-            start = n
-            end = n + batch_size
-
-            if stream is not None:
-                partial_array[:batch_size].set(self._array[start:end], stream=stream)
-                yield start, end, Waves(partial_array[:batch_size], extent=self.extent, energy=self.energy)
-
-            else:
-                yield start, end, Waves(self._array[start:end], extent=self.extent, energy=self.energy)
-
-            n += batch_size
-            pbar.update(batch_size)
-
-        pbar.refresh()
-        if close_pbar:
-            pbar.close()
-
-    def multislice(self,
-                   potential: AbstractPotential,
-                   max_batch=None,
-                   multislice_pbar: Union[ProgressBar, bool] = True,
-                   plane_waves_pbar: Union[ProgressBar, bool] = True):
-        """
-        Propagate the scattering matrix through the provided potential.
-
-        Parameters
-        ----------
-        potential : AbstractPotential object
-            Scattering potential.
-        max_batch : int, optional
-            The probe batch size. Larger batches are faster, but require more memory. Default is None.
-        multislice_pbar : bool, optional
-            Display multislice progress bar. Default is True.
-        plane_waves_pbar : bool, optional
-            Display plane waves progress bar. Default is True.
-
-        Returns
-        -------
-        Waves object.
-            Probe exit wave functions for the provided positions.
-        """
-
-        if not self.periodic:
-            self._raise_not_periodic()
-
-        if not isinstance(max_batch, int):
-            max_batch = self._max_batch_expansion()
-
-        if isinstance(multislice_pbar, bool):
-            multislice_pbar = ProgressBar(total=len(potential), desc='Multislice', disable=not multislice_pbar)
-            close_pbar = True
-        else:
-            close_pbar = False
-
-        propagator = FresnelPropagator()
-
-        for start, end, partial_s_matrix in self._generate_partial(max_batch, pbar=plane_waves_pbar):
-            _multislice(partial_s_matrix, potential, propagator=propagator, pbar=multislice_pbar)
-            self._array[start: end] = copy_to_device(partial_s_matrix.array, get_array_module(self._array))
-
-        self._antialiasing_aperture = 2 / 3.
-
-        if close_pbar:
-            multislice_pbar.close()
-        return self
-
-    def _get_ctf_coefficients(self):
-        xp = get_array_module(self._array)
-        alpha = xp.sqrt(self.k[:, 0] ** 2 + self.k[:, 1] ** 2) * self.wavelength
-        phi = xp.arctan2(self.k[:, 0], self.k[:, 1])
-        return self._ctf.evaluate(alpha, phi)
-
-    def _get_translation_coefficients(self, positions: Sequence[float]):
-        xp = get_array_module_from_device(self.device)
-        complex_exponential = get_device_function(xp, 'complex_exponential')
-        positions = xp.asarray(positions)
-        k = xp.asarray(self.k)
-        return (complex_exponential(2. * np.pi * k[:, 0][None] * positions[:, 0, None]) *
-                complex_exponential(2. * np.pi * k[:, 1][None] * positions[:, 1, None]))
-
-    def _get_coefficients(self, positions: Sequence[float]):
-        return self._get_translation_coefficients(positions) * self._get_ctf_coefficients()
-
-    def _get_requisite_crop(self, positions: Sequence[float], return_per_position: bool = False):
-        offset = (self.cropped_shape[0] // 2, self.cropped_shape[1] // 2)
-        corners = np.rint(np.array(positions) / self.sampling - offset).astype(np.int)
-        upper_corners = corners + np.asarray(self.cropped_shape)
-
-        crop_corner = (np.min(corners[:, 0]).item(), np.min(corners[:, 1]).item())
-
-        size = (np.max(upper_corners[:, 0]).item() - crop_corner[0],
-                np.max(upper_corners[:, 1]).item() - crop_corner[1])
-
-        if return_per_position:
-            return crop_corner, size, corners
-        else:
-            return crop_corner, size
-
-    def collapse(self, positions: Sequence[float], max_batch_expansion: int = None) -> Waves:
-        """
-        Collapse the scattering matrix to probe wave functions centered on the provided positions.
-
-        Parameters
-        ----------
-        positions : array of xy-positions
-            The positions of the probe wave functions.
-        max_batch_expansion : int, optional
-            The maximum number of plane waves the reduction is applied to simultanously. Default is None.
-
-        Returns
-        -------
-        Waves object
-            Probe wave functions for the provided positions.
-        """
-
-        if max_batch_expansion is None:
-            max_batch_expansion = self._max_batch_expansion()
-
-        xp = get_array_module_from_device(self.device)
-        positions = np.array(positions, dtype=xp.float32)
-
-        if positions.shape == (2,):
-            positions = positions[None]
-        elif (len(positions.shape) != 2) or (positions.shape[-1] != 2):
-            raise RuntimeError()
-
-        coefficients = self._get_coefficients(positions)
-
-        if self.cropped_shape != self.gpts:
-            crop_corner, size, corners = self._get_requisite_crop(positions, return_per_position=True)
-
-            if self._offset is not None:
-                corners -= self._offset
-                crop_corner = (crop_corner[0] - self._offset[0], crop_corner[1] - self._offset[1])
-
-            array = copy_to_device(periodic_crop(self.array, crop_corner, size), device=self._device)
-            window = xp.tensordot(coefficients, array, axes=[(1,), (0,)])
-
-            corners -= crop_corner
-            for i in range(len(corners)):
-                window[i, :self.cropped_shape[0], :self.cropped_shape[1]] = periodic_crop(window[i], corners[i],
-                                                                                          self.cropped_shape)
-
-            window = window[:, :self.cropped_shape[0], :self.cropped_shape[1]].copy()
-
-        elif max_batch_expansion >= len(self):
-            for start, end, partial_s_matrix in self._generate_partial(max_batch_expansion, pbar=False):
-                partial_coefficients = coefficients[:, start:end]
-                window = xp.tensordot(partial_coefficients, partial_s_matrix.array, axes=[(1,), (0,)])
-
-        else:
-            window = xp.tensordot(coefficients, self.array, axes=[(1,), (0,)])
-            # window = xp.tensordot(coefficients, copy_to_device(self.array, device=self._device), axes=[(1,), (0,)])
-
-        return Waves(window, sampling=self.sampling, energy=self.energy,
-                     antialiasing_aperture=self.antialiasing_aperture)
-
-    def _generate_probes(self, scan: AbstractScan, max_batch_probes, max_batch_expansion):
-
-        if not isinstance(max_batch_expansion, int):
-            max_batch_expansion = self._max_batch_expansion()
-
-        if not isinstance(max_batch_probes, int):
-            max_batch_probes = self._max_batch_probes()
-
-        for indices, positions in scan.generate_positions(max_batch=max_batch_probes):
-            yield indices, self.collapse(positions, max_batch_expansion=max_batch_expansion)
-
-    def scan(self,
-             scan: AbstractScan,
-             detectors: Sequence[AbstractDetector],
-             max_batch_probes=None,
-             max_batch_expansion=None,
-             pbar: Union[ProgressBar, bool] = True):
-
-        """
-        Raster scan the probe across the potential and record a measurement for each detector.
-
-        Parameters
-        ----------
-        scan : Scan object
-            Scan defining the positions of the probe wave functions.
-        detectors : List of Detector objects
-            The detectors recording the measurements.
-        max_batch_probes : int, optional
-            The probe batch size. Larger batches are faster, but require more memory. Default is None.
-        max_batch_expansion : int, optional
-            The expansion plane wave batch size. Default is None.
-        pbar : bool, optional
-            Display progress bars. Default is True.
-
-        Returns
-        -------
-        dict
-            Dictionary of measurements with keys given by the detector.
-        """
-
-        if isinstance(detectors, dict):
-            measurements = detectors
-        else:
-            measurements = {}
-
-        if isinstance(pbar, bool):
-            pbar = ProgressBar(total=len(scan), desc='Scan', disable=not pbar)
-
-        for indices, exit_probes in self._generate_probes(scan, max_batch_probes, max_batch_expansion):
-            for detector in detectors:
-                # for detector, measurement in measurements.items():
-                new_measurement = detector.detect(exit_probes)
-                try:
-                    scan.insert_new_measurement(measurements[detector], indices, new_measurement)
-                except KeyError:
-                    measurements[detector] = detector.allocate_measurement(exit_probes, scan)
-                    scan.insert_new_measurement(measurements[detector], indices, new_measurement)
-
-            # scan.insert_new_measurement(measurement, indices, detector.detect(exit_probes))
-            pbar.update(len(indices))
-
-        pbar.refresh()
-        pbar.close()
-        return measurements
-
-    def transfer(self, device):
-        return self.__class__(array=copy_to_device(self.array, device),
-                              expansion_cutoff=self._expansion_cutoff,
-                              k=self.k.copy(),
-                              ctf=self.ctf.copy(),
-                              extent=self.extent,
-                              offset=self.offset,
-                              cropped_shape=self.cropped_shape,
-                              energy=self.energy,
-                              antialiasing_aperture=self.antialiasing_aperture,
-                              device=self.device)
-
-    def __copy__(self, device=None):
-        return self.__class__(array=self.array.copy(),
-                              expansion_cutoff=self._expansion_cutoff,
-                              k=self.k.copy(),
-                              ctf=self.ctf.copy(),
-                              extent=self.extent,
-                              offset=self.offset,
-                              cropped_shape=self.cropped_shape,
-                              energy=self.energy,
-                              antialiasing_aperture=self.antialiasing_aperture,
-                              device=self.device)
-
-    def copy(self):
-        """Make a copy."""
-        return copy(self)
-
-
-class SMatrix(_WavesLike, HasDeviceMixin):
-    """
-    Scattering matrix builder class
-
-    The scattering matrix builder object is used for creating scattering matrices and simulating STEM experiments using
-    the PRISM algorithm.
-
-    Parameters
-    ----------
-    expansion_cutoff : float
-        The angular cutoff of the plane wave expansion [mrad].
-    energy : float
-        Electron energy [eV].
-    interpolation : one or two int, optional
-        Interpolation factor. Default is 1 (no interpolation).
-    ctf: CTF object, optional
-        The probe contrast transfer function. Default is None (aperture is set by the cutoff of the expansion).
-    extent : one or two float, optional
-        Lateral extent of wave functions [Å]. Default is None (inherits the extent from the potential).
-    gpts : one or two int, optional
-        Number of grid points describing the wave functions. Default is None (inherits the gpts from the potential).
-    sampling : one or two float, None
-        Lateral sampling of wave functions [1 / Å]. Default is None (inherits the sampling from the potential.
-    device : str, optional
-        The calculations will be carried out on this device. Default is 'cpu'.
-    storage : str, optional
-        The scattering matrix will be stored on this device. Default is None (uses the option chosen for device).
-    kwargs :
-        The parameters of a new CTF object as keyword arguments.
-    """
-
-    def __init__(self,
-                 expansion_cutoff: float,
-                 energy: float,
-                 interpolation: int = 1,
-                 ctf: CTF = None,
-                 extent: Union[float, Sequence[float]] = None,
-                 gpts: Union[int, Sequence[int]] = None,
-                 sampling: Union[float, Sequence[float]] = None,
-                 device: str = 'cpu',
-                 storage: str = None,
-                 **kwargs):
-
-        if not isinstance(interpolation, int):
-            raise ValueError('Interpolation factor must be int')
-
-        self._interpolation = interpolation
-        self._expansion_cutoff = expansion_cutoff
-
-        if ctf is None:
-            ctf = CTF(**kwargs)
-
-        if ctf.energy is None:
-            ctf.energy = energy
-
-        if (ctf.energy != energy):
-            raise RuntimeError
-
-        self._ctf = ctf
-        self._accelerator = self._ctf._accelerator
-
-        self._grid = Grid(extent=extent, gpts=gpts, sampling=sampling)
-
-        self.changed = Event()
-
-        self._ctf.changed.register(self.changed.notify)
-        self._grid.changed.register(self.changed.notify)
-        self._accelerator.changed.register(self.changed.notify)
-
-        self._device = device
-        if storage is None:
-            storage = device
-
-        self._storage = storage
-
-        super().__init__()
-
-    @property
-    def ctf(self):
-        """The contrast transfer function of the probes."""
-        return self._ctf
-
-    @ctf.setter
-    def ctf(self, value):
-        self._ctf = value
-
-    @property
-    def expansion_cutoff(self) -> float:
-        """Plane wave expansion cutoff."""
-        return self._expansion_cutoff
-
-    @expansion_cutoff.setter
-    def expansion_cutoff(self, value: float):
-        self._expansion_cutoff = value
-
-    @property
-    def interpolation(self) -> int:
-        """Interpolation factor."""
-        return self._interpolation
-
-    @interpolation.setter
-    def interpolation(self, value: int):
-        self._interpolation = value
-
-    @property
-    def interpolated_grid(self) -> Grid:
-        """The grid of the interpolated probe wave functions."""
-        interpolated_gpts = tuple(n // self.interpolation for n in self.gpts)
-        return Grid(gpts=interpolated_gpts, sampling=self.sampling, lock_gpts=True)
-
-    def _generate_tds_probes(self,
-                             scan: AbstractScan,
-                             potential: AbstractTDSPotentialBuilder,
-                             max_batch_probes: int,
-                             max_batch_expansion: int,
-                             potential_pbar: Union[ProgressBar, bool] = True,
-                             multislice_pbar: Union[ProgressBar, bool] = True,
-                             plane_waves_pbar: Union[ProgressBar, bool] = True):
-
-        if isinstance(potential_pbar, bool):
-            potential_pbar = ProgressBar(total=len(potential), desc='Potential', disable=not potential_pbar)
-
-        # if isinstance(multislice_pbar, bool):
-        #    multislice_pbar = ProgressBar(total=len(potential), desc='Multislice', disable=not multislice_pbar)
-
-        if isinstance(plane_waves_pbar, bool):
-            plane_waves_pbar = ProgressBar(total=len(self), desc='Plane waves', disable=not plane_waves_pbar)
-
-        # import cupy as cp
-        # from abtem.device import get_available_memory
-        # mempool = cp.get_default_memory_pool()
-
-        for potential_config in potential.generate_frozen_phonon_potentials(pbar=potential_pbar):
-            S = self.build()
-
-            S = S.multislice(potential_config,
-                             max_batch=max_batch_expansion,
-                             multislice_pbar=False,  # multislice_pbar,
-                             plane_waves_pbar=plane_waves_pbar)
-
-            S = S.downsample('limit')
-
-            # del potential_config
-            # mempool.free_all_blocks()
-
-            yield S._generate_probes(scan, max_batch_probes, max_batch_expansion)
-            # del S
-            # mempool.free_all_blocks()
-
-        # multislice_pbar.refresh()
-        # multislice_pbar.close()
-
-        plane_waves_pbar.refresh()
-        plane_waves_pbar.close()
-
-        potential_pbar.refresh()
-        potential_pbar.close()
-
-    def multislice(self,
-                   potential: AbstractPotential,
-                   max_batch: int = None,
-                   pbar: Union[ProgressBar, bool] = True):
-        """
-        Build scattering matrix and propagate the scattering matrix through the provided potential.
-
-        Parameters
-        ----------
-        potential : AbstractPotential
-            Scattering potential.
-        max_batch : int, optional
-            The probe batch size. Larger batches are faster, but require more memory. Default is None.
-        pbar : bool, optional
-            Display progress bars. Default is True.
-
-        Returns
-        -------
-        Waves object
-            Probe exit wave functions as a Waves object.
-        """
-
-        if isinstance(potential, Atoms):
-            potential = Potential(potential)
-
-        self.grid.match(potential)
-        return self.build().multislice(potential,
-                                       max_batch=max_batch,
-                                       multislice_pbar=pbar,
-                                       plane_waves_pbar=pbar)
-
-    def scan(self,
-             scan: AbstractScan,
-             detectors: Sequence[AbstractDetector],
-             potential: Union[Atoms, AbstractPotential],
-             max_batch_probes: int = None,
-             max_batch_expansion: int = None,
-             pbar: bool = True):
-        """
-        Build the scattering matrix. Raster scan the probe across the potential, record a measurement for each detector.
-
-        Parameters
-        ----------
-        scan : Scan object
-            Scan defining the positions of the probe wave functions.
-        detectors : List of Detector objects
-            The detectors recording the measurements.
-        potential : Potential object
-            The potential to scan the probe over.
-        max_batch_probes : int, optional
-            The probe batch size. Larger batches are faster, but require more memory. Default is None.
-        max_batch_expansion : int, optional
-            The expansion plane wave batch size. Default is None.
-        pbar : bool, optional
-            Display progress bars. Default is True.
-
-        Returns
-        -------
-        dict
-            Dictionary of measurements with keys given by the detector.
-        """
-
-        self.grid.match(potential.grid)
-        self.grid.check_is_defined()
-
-        if isinstance(potential, AbstractTDSPotentialBuilder):
-            probe_generators = self._generate_tds_probes(scan,
-                                                         potential,
-                                                         max_batch_probes=max_batch_probes,
-                                                         max_batch_expansion=max_batch_expansion,
-                                                         potential_pbar=True,
-                                                         multislice_pbar=True)
-
-            tds_bar = ProgressBar(total=len(potential.frozen_phonons), desc='TDS',
-                                  disable=(not pbar) or (len(potential.frozen_phonons) == 1))
-
-        else:
-            if isinstance(potential, AbstractPotentialBuilder):
-                potential = potential.build(pbar=True)
-
-            S = self.multislice(potential, max_batch=max_batch_expansion, pbar=pbar)
-            probe_generators = [S._generate_probes(scan,
-                                                   max_batch_probes=max_batch_probes,
-                                                   max_batch_expansion=max_batch_expansion)]
-
-            tds_bar = None
-
-        scan_bar = ProgressBar(total=len(scan), desc='Scan', disable=not pbar)
-
-        measurements = {}
-        for probe_generator in probe_generators:
-            scan_bar.reset()
-
-            for indices, exit_probes in probe_generator:
-                for detector in detectors:
-                    new_measurement = detector.detect(exit_probes)
-
-                    if isinstance(potential, AbstractTDSPotentialBuilder):
-                        new_measurement /= len(potential.frozen_phonons)
-
-                    try:
-                        scan.insert_new_measurement(measurements[detector], indices, new_measurement)
-                    except KeyError:
-                        measurements[detector] = detector.allocate_measurement(exit_probes, scan)
-                        scan.insert_new_measurement(measurements[detector], indices, new_measurement)
-
-                scan_bar.update(len(indices))
-
-            scan_bar.refresh()
-            if tds_bar:
-                tds_bar.update(1)
-
-        scan_bar.close()
-
-        if tds_bar:
-            tds_bar.refresh()
-            tds_bar.close()
-
-        return measurements
-
-    def __len__(self):
-        return len(self.k)
-
-    @property
-    def k(self):
-        xp = get_array_module_from_device(self._device)
-        n_max = int(
-            xp.ceil(self.expansion_cutoff / 1000. / (self.wavelength / self.extent[0] * self.interpolation)))
-        m_max = int(
-            xp.ceil(self.expansion_cutoff / 1000. / (self.wavelength / self.extent[1] * self.interpolation)))
-
-        n = xp.arange(-n_max, n_max + 1, dtype=xp.float32)
-        w = xp.asarray(self.extent[0], dtype=xp.float32)
-        m = xp.arange(-m_max, m_max + 1, dtype=xp.float32)
-        h = xp.asarray(self.extent[1], dtype=xp.float32)
-
-        kx = n / w * xp.float32(self.interpolation)
-        ky = m / h * xp.float32(self.interpolation)
-
-        mask = kx[:, None] ** 2 + ky[None, :] ** 2 < (self.expansion_cutoff / 1000. / self.wavelength) ** 2
-        kx, ky = xp.meshgrid(kx, ky, indexing='ij')
-        kx = kx[mask]
-        ky = ky[mask]
-        return xp.asarray((kx, ky)).T
-
-    def build(self) -> SMatrixArray:
-        """Build the scattering matrix."""
-
-        self.grid.check_is_defined()
-        self.accelerator.check_is_defined()
-        xp = get_array_module_from_device(self._device)
-        storage_xp = get_array_module_from_device(self._storage)
-        complex_exponential = get_device_function(xp, 'complex_exponential')
-
-        x = xp.linspace(0, self.extent[0], self.gpts[0], endpoint=self.grid.endpoint[0], dtype=xp.float32)
-        y = xp.linspace(0, self.extent[1], self.gpts[1], endpoint=self.grid.endpoint[1], dtype=xp.float32)
-
-        k = self.k
-
-        shape = (len(k),) + self.gpts
-        array = storage_xp.zeros(shape, dtype=np.complex64)
-
-        for i in range(len(k)):
-            array[i] = copy_to_device(complex_exponential(-2 * np.pi * k[i, 0, None, None] * x[:, None]) *
-                                      complex_exponential(-2 * np.pi * k[i, 1, None, None] * y[None, :]),
-                                      self._storage)
-
-        return SMatrixArray(array,
-                            expansion_cutoff=self.expansion_cutoff,
-                            interpolation=self.interpolation,
-                            extent=self.extent,
-                            energy=self.energy,
-                            k=k,
-                            ctf=self.ctf.copy(),
-                            device=self._device)
-
-    def profile(self, angle=0.):
-        measurement = self.build().collapse((self.extent[0] / 2, self.extent[1] / 2)).intensity()
-        return probe_profile(measurement, angle=angle)
-
-    def interact(self, sliders=None, profile=False):
-        from abtem.visualize.bqplot import show_measurement_1d, show_measurement_2d
-        from abtem.visualize.widgets import quick_sliders
-        import ipywidgets as widgets
-
-        if profile:
-            figure, callback = show_measurement_1d(lambda: [self.profile()])
-        else:
-            figure, callback = show_measurement_2d(lambda: self.build().collapse((self.extent[0] / 2,
-                                                                                  self.extent[1] / 2)).intensity())
-
-        self.changed.register(callback)
-
-        if sliders:
-            sliders = quick_sliders(self.ctf, **sliders)
-            return widgets.HBox([figure, widgets.VBox(sliders)])
-        else:
-            return figure
-
-    def show(self, **kwargs):
-        """
-        Show the probe wave function.
-
-        Parameters
-        ----------
-        angle : float, optional
-            Angle along which the profile is shown [deg]. Default is 0 degrees.
-        kwargs : Additional keyword arguments for the abtem.plot.show_image function.
-        """
-        return self.build().collapse((self.extent[0] / 2, self.extent[1] / 2)).intensity().show(**kwargs)
-
-    def __copy__(self):
-        return self.__class__(expansion_cutoff=self.expansion_cutoff,
-                              interpolation=self.interpolation,
-                              ctf=self.ctf.copy(),
-                              extent=self.extent,
-                              gpts=self.gpts,
-                              energy=self.energy,
-                              device=self._device,
-                              storage=self._storage)
-
-    def copy(self):
-        """Make a copy."""
-        return copy(self)
+"""Module to describe electron waves and their propagation."""
+from copy import copy
+from numbers import Number
+from typing import Union, Sequence, Tuple
+
+import h5py
+import numpy as np
+from ase import Atoms
+
+from abtem.base_classes import Grid, Accelerator, cache_clear_callback, Cache, cached_method, \
+    HasGridMixin, HasAcceleratorMixin, AntialiasFilter, Event
+from abtem.detect import AbstractDetector
+from abtem.device import get_array_module, get_device_function, asnumpy, get_array_module_from_device, \
+    copy_to_device, get_available_memory, HasDeviceMixin
+from abtem.measure import calibrations_from_grid, Measurement, block_zeroth_order_spot, probe_profile
+from abtem.potentials import Potential, AbstractPotential, AbstractTDSPotentialBuilder, AbstractPotentialBuilder
+from abtem.scan import AbstractScan, GridScan
+from abtem.transfer import CTF
+from abtem.utils import polar_coordinates, ProgressBar, spatial_frequencies, subdivide_into_batches, periodic_crop, \
+    fft_crop
+
+
+class FresnelPropagator:
+    """
+    Fresnel propagator object.
+
+    This class is used for propagating a wave function object using the near-field approximation (Fresnel diffraction).
+    The array representing the Fresnel propagator function is cached.
+    """
+
+    def __init__(self):
+        self._cache = Cache(1)
+
+    @cached_method('_cache')
+    def _evaluate_propagator_array(self,
+                                   gpts: Tuple[int, int],
+                                   sampling: Tuple[float, float],
+                                   wavelength: float,
+                                   dz: float,
+                                   xp) -> np.ndarray:
+        complex_exponential = get_device_function(xp, 'complex_exponential')
+        kx = xp.fft.fftfreq(gpts[0], sampling[0]).astype(xp.float32)
+        ky = xp.fft.fftfreq(gpts[1], sampling[1]).astype(xp.float32)
+        f = (complex_exponential(-(kx ** 2)[:, None] * np.pi * wavelength * dz) *
+             complex_exponential(-(ky ** 2)[None] * np.pi * wavelength * dz))
+
+        return f * AntialiasFilter().get_mask(gpts, sampling, xp)
+
+    def propagate(self, waves: Union['Waves', 'SMatrixArray'], dz: float) -> Union['Waves', 'SMatrixArray']:
+        """
+        Propagate wave functions or scattering matrix.
+
+        Parameters
+        ----------
+        waves : Waves or SMatrixArray object
+            Wave function or scattering matrix to propagate.
+        dz : float
+            Propagation distance [Å].
+
+        Returns
+        -------
+        Waves or SMatrixArray object
+            The propagated wave functions.
+        """
+        fft2_convolve = get_device_function(get_array_module(waves.array), 'fft2_convolve')
+
+        propagator_array = self._evaluate_propagator_array(waves.grid.gpts,
+                                                           waves.grid.sampling,
+                                                           dz,
+                                                           waves.wavelength,
+                                                           get_array_module(waves.array))
+
+        fft2_convolve(waves._array, propagator_array, overwrite_x=True)
+        waves._antialiasing_aperture = 2 / 3.
+
+        return waves
+
+
+def _multislice(waves: Union['Waves', 'SMatrixArray'],
+                potential: AbstractPotential,
+                propagator: FresnelPropagator = None,
+                pbar: Union[ProgressBar, bool] = True,
+                max_batch=1,
+                ) -> Union['Waves', 'SMatrixArray']:
+    waves.grid.match(potential)
+    waves.accelerator.check_is_defined()
+    waves.grid.check_is_defined()
+
+    if propagator is None:
+        propagator = FresnelPropagator()
+
+    if isinstance(pbar, bool):
+        pbar = ProgressBar(total=len(potential), desc='Multislice', disable=not pbar)
+
+    pbar.reset()
+    if max_batch == 1:
+        for start, end, t in potential.generate_transmission_functions(energy=waves.energy, max_batch=1):
+            waves = t.transmit(waves)
+            waves = propagator.propagate(waves, t.thickness)
+            pbar.update(1)
+    else:
+        for start, end, t_chunk in potential.generate_transmission_functions(energy=waves.energy, max_batch=max_batch):
+            for _, __, t_slice in t_chunk.generate_slices(max_batch=1):
+                waves = t_slice.transmit(waves)
+                waves = propagator.propagate(waves, t_slice.thickness)
+
+            pbar.update(end - start)
+
+    pbar.refresh()
+    return waves
+
+
+class _WavesLike(HasGridMixin, HasAcceleratorMixin):
+
+    def __init__(self, antialiasing_aperture=None):
+        if antialiasing_aperture is None:
+            antialiasing_aperture = AntialiasFilter.cutoff
+        self._antialiasing_aperture = antialiasing_aperture
+
+    @property
+    def antialiasing_aperture(self):
+        return self._antialiasing_aperture
+
+    @property
+    def cutoff_scattering_angles(self):
+        kcut = 1 / max(self.sampling) / 2 * min(self.antialiasing_aperture, 1)
+        kcut = (np.ceil(2 * self.extent[0] * kcut) / (2 * self.extent[0]) * self.wavelength * 1e3,
+                np.ceil(2 * self.extent[1] * kcut) / (2 * self.extent[1]) * self.wavelength * 1e3)
+        return kcut
+
+    @property
+    def rectangle_cutoff_scattering_angles(self):
+        rolloff = AntialiasFilter.rolloff
+        kcut = (1 / max(self.sampling) / 2 * self.antialiasing_aperture - rolloff) / np.sqrt(2)
+        kcut = (np.floor(2 * self.extent[0] * kcut) / (2 * self.extent[0]) * self.wavelength * 1e3,
+                np.floor(2 * self.extent[1] * kcut) / (2 * self.extent[1]) * self.wavelength * 1e3)
+        return kcut
+
+    @property
+    def angular_sampling(self):
+        self.grid.check_is_defined()
+        self.accelerator.check_is_defined()
+        return tuple([1 / l * self.wavelength * 1e3 for l in self.extent])
+
+    def downsampled_gpts(self, max_angle):
+        if max_angle is None:
+            gpts = self.gpts
+        elif isinstance(max_angle, str):
+            if max_angle == 'limit':
+                cutoff_scattering_angle = self.cutoff_scattering_angles
+            elif max_angle == 'valid':
+                cutoff_scattering_angle = self.rectangle_cutoff_scattering_angles
+            else:
+                raise RuntimeError()
+
+            angular_sampling = self.angular_sampling
+            gpts = (int(round(cutoff_scattering_angle[0] / angular_sampling[0] * 2)),
+                    int(round(cutoff_scattering_angle[1] / angular_sampling[1] * 2)))
+
+        elif isinstance(max_angle, Number):
+            gpts = tuple([int(2 * np.floor(max_angle / d)) + 1 for n, d in zip(self.gpts, self.angular_sampling)])
+        else:
+            raise RuntimeError()
+
+        return (min(gpts[0], self.gpts[0]), min(gpts[1], self.gpts[1]))
+
+
+class Waves(_WavesLike):
+    """
+    Waves object
+
+    The waves object can define a batch of arbitrary 2D wave functions defined by a complex numpy array.
+
+    Parameters
+    ----------
+    extent : one or two float
+        Lateral extent of wave function [Å].
+    sampling : one or two float
+        Lateral sampling of wave functions [1 / Å].
+    energy : float
+        Electron energy [eV].
+    antialiasing_aperture : float
+        Antialiasing aperture.
+    """
+
+    def __init__(self,
+                 array: np.ndarray,
+                 extent: Union[float, Sequence[float]] = None,
+                 sampling: Union[float, Sequence[float]] = None,
+                 energy: float = None,
+                 antialiasing_aperture: float = None):
+
+        if len(array.shape) < 2:
+            raise RuntimeError('Wave function array should be have 2 dimensions or more')
+
+        self._array = array
+
+        self._grid = Grid(extent=extent, gpts=array.shape[-2:], sampling=sampling, lock_gpts=True)
+        self._accelerator = Accelerator(energy=energy)
+
+        super().__init__(antialiasing_aperture=antialiasing_aperture)
+
+    def __len__(self):
+        return len(self.array)
+
+    @property
+    def array(self) -> np.ndarray:
+        """Array representing the wave functions."""
+        return self._array
+
+    def intensity(self) -> Measurement:
+        """
+        Calculate the intensity of the wave functions at the image plane.
+
+        Returns
+        -------
+        Measurement
+            The wave function intensity.
+        """
+
+        calibrations = calibrations_from_grid(self.grid.gpts, self.grid.sampling, ['x', 'y'])
+        # array = np.squeeze(self.array)
+        array = self.array
+
+        calibrations = (None,) * (len(array.shape) - 2) + calibrations
+        abs2 = get_device_function(get_array_module(self.array), 'abs2')
+        return Measurement(abs2(array), calibrations)
+
+    def downsample(self, max_angle='valid', return_fourier_space=False):
+        xp = get_array_module(self.array)
+        fft2 = get_device_function(xp, 'fft2')
+        ifft2 = get_device_function(xp, 'ifft2')
+        array = fft2(self.array, overwrite_x=False)
+
+        gpts = self.downsampled_gpts(max_angle)
+
+        if gpts != self.gpts:
+            array = fft_crop(array, self.array.shape[:-2] + gpts)
+
+        antialiasing_aperture = self.antialiasing_aperture * min(self.gpts[0] / gpts[0], self.gpts[1] / gpts[1])
+
+        if return_fourier_space:
+            return Waves(array, extent=self.extent, energy=self.energy, antialiasing_aperture=antialiasing_aperture)
+        else:
+            return Waves(ifft2(array), extent=self.extent, energy=self.energy,
+                         antialiasing_aperture=antialiasing_aperture)
+
+    def far_field(self, max_angle='valid', in_place=False):
+        return self.downsample(max_angle=max_angle, return_fourier_space=True)
+
+    def diffraction_pattern(self, max_angle='valid', block_zeroth_order=False) -> Measurement:
+        """
+        Calculate the intensity of the wave functions at the diffraction plane.
+
+        Returns
+        -------
+        Measurement object
+            The intensity of the diffraction pattern(s).
+        """
+        xp = get_array_module(self.array)
+        abs2 = get_device_function(xp, 'abs2')
+        waves = self.far_field(max_angle)
+
+        pattern = np.fft.fftshift(asnumpy(abs2(waves.array)), axes=(-1, -2))
+
+        calibrations = calibrations_from_grid(waves.gpts,
+                                              waves.sampling,
+                                              names=['alpha_x', 'alpha_y'],
+                                              units='mrad',
+                                              scale_factor=self.wavelength * 1000,
+                                              fourier_space=True)
+
+        calibrations = (None,) * (len(pattern.shape) - 2) + calibrations
+
+        measurement = Measurement(pattern, calibrations)
+
+        if block_zeroth_order:
+            block_zeroth_order_spot(measurement, block_zeroth_order)
+
+        return measurement
+
+    def apply_ctf(self, ctf: CTF = None, in_place=False, **kwargs):
+        """
+        Apply the aberrations defined by a CTF object to wave function.
+
+        Parameters
+        ----------
+        ctf : CTF
+            Contrast Transfer Function object to be applied.
+        kwargs :
+            Provide the aberration coefficients as keyword arguments.
+
+        Returns
+        -------
+        Waves object
+            The wave functions with aberrations applied.
+        """
+
+        xp = get_array_module(self.array)
+        fft2_convolve = get_device_function(get_array_module(self.array), 'fft2_convolve')
+
+        if ctf is None:
+            ctf = CTF(**kwargs)
+
+        if not ctf.accelerator.energy:
+            ctf.accelerator.match(self.accelerator)
+
+        self.accelerator.match(ctf.accelerator, check_match=True)
+
+        self.accelerator.check_is_defined()
+        self.grid.check_is_defined()
+
+        kx, ky = spatial_frequencies(self.grid.gpts, self.grid.sampling)
+        alpha, phi = polar_coordinates(xp.asarray(kx * self.wavelength), xp.asarray(ky * self.wavelength))
+        kernel = ctf.evaluate(alpha, phi)
+
+        return self.__class__(fft2_convolve(self.array, kernel, overwrite_x=in_place),
+                              extent=self.extent,
+                              energy=self.energy)
+
+    def multislice(self,
+                   potential: AbstractPotential,
+                   pbar: Union[ProgressBar, bool] = True,
+                   detector=None,
+                   potential_chunks=1) -> 'Waves':
+        """
+        Propagate and transmit wave function through the provided potential.
+
+        Parameters
+        ----------
+        potential : Potential
+            The potential through which to propagate the wave function.
+        pbar : bool
+            If true, display a progress bar.
+
+        Returns
+        -------
+        Waves object
+            Wave function at the exit plane of the potential.
+        """
+
+        self.grid.match(potential)
+
+        propagator = FresnelPropagator()
+
+        result = None
+        if isinstance(potential, AbstractTDSPotentialBuilder):
+            if len(potential.frozen_phonons) > 1:
+                xp = get_array_module(self.array)
+                n = len(potential.frozen_phonons)
+
+                if detector:
+                    result = detector.allocate_measurement(self, self.array.shape[:-2])
+                else:
+                    if n > 1:
+                        if self.array.shape[0] == 1:
+                            out_array = xp.zeros((n,) + self.array.shape[1:], dtype=xp.complex64)
+                        else:
+                            out_array = xp.zeros((n,) + self.array.shape, dtype=xp.complex64)
+                    else:
+                        out_array = xp.zeros(self.array.shape, dtype=xp.complex64)
+
+                    result = self.__class__(out_array,
+                                            extent=self.extent,
+                                            energy=self.energy,
+                                            antialiasing_aperture=2 / 3.)
+
+                tds_pbar = ProgressBar(total=n, desc='TDS', disable=(not pbar) or (n == 1))
+                multislice_pbar = ProgressBar(total=len(potential), desc='Multislice', disable=not pbar)
+
+                for i, potential_config in enumerate(potential.generate_frozen_phonon_potentials(pbar=pbar)):
+                    multislice_pbar.reset()
+
+                    exit_waves = _multislice(copy(self),
+                                             potential_config,
+                                             propagator=propagator,
+                                             pbar=multislice_pbar,
+                                             max_batch=potential_chunks)
+
+                    if detector:
+                        result._array += asnumpy(detector.detect(exit_waves))
+                    else:
+                        result._array[i] = exit_waves.array
+
+                    tds_pbar.update(1)
+
+                multislice_pbar.close()
+                tds_pbar.close()
+
+        if result is None:
+            result = _multislice(self, potential, propagator, pbar, max_batch=potential_chunks)
+
+            if detector:
+                result = detector.detect(result)
+
+        return result
+
+    def write(self, path: str):
+        """
+        Write wave functions to a hdf5 file.
+
+        path : str
+            The path to write the file.
+        """
+
+        with h5py.File(path, 'w') as f:
+            f.create_dataset('array', data=self.array)
+            f.create_dataset('energy', data=self.energy)
+            f.create_dataset('extent', data=self.extent)
+
+    @classmethod
+    def read(cls, path: str) -> 'Waves':
+        """
+        Read wave functions from a hdf5 file.
+
+        path : str
+            The path to read the file.
+        """
+
+        with h5py.File(path, 'r') as f:
+            datasets = {}
+            for key in f.keys():
+                datasets[key] = f.get(key)[()]
+
+        return cls(array=datasets['array'], extent=datasets['extent'], energy=datasets['energy'])
+
+    def __getitem__(self, item):
+        if len(self.array.shape) <= self.grid.dimensions:
+            raise RuntimeError()
+        return self.__class__(array=self._array[item], extent=self.extent, energy=self.energy)
+
+    def show(self, ax=None, **kwargs):
+        """
+        Show the wave function.
+
+        kwargs :
+            Additional keyword arguments for the abtem.plot.show_image function.
+        """
+        return self.intensity().show(ax=ax, **kwargs)
+
+    def __copy__(self):
+        new_copy = self.__class__(array=self._array.copy())
+        new_copy._grid = copy(self.grid)
+        new_copy._accelerator = copy(self.accelerator)
+        return new_copy
+
+    def copy(self):
+        """Make a copy."""
+        return copy(self)
+
+
+class PlaneWave(_WavesLike, HasDeviceMixin):
+    """
+    Plane wave object
+
+    The plane wave object is used for building plane waves.
+
+    Parameters
+    ----------
+    extent : two float
+        Lateral extent of wave function [Å].
+    gpts : two int
+        Number of grid points describing the wave function.
+    sampling : two float
+        Lateral sampling of wave functions [1 / Å].
+    energy : float
+        Electron energy [eV].
+    device : str
+        The plane waves will be build on this device.
+    """
+
+    def __init__(self,
+                 extent: Union[float, Sequence[float]] = None,
+                 gpts: Union[int, Sequence[int]] = None,
+                 sampling: Union[float, Sequence[float]] = None,
+                 energy: float = None,
+                 device: str = 'cpu'):
+        self._grid = Grid(extent=extent, gpts=gpts, sampling=sampling)
+        self._accelerator = Accelerator(energy=energy)
+        self._device = device
+
+        super().__init__()
+
+    def multislice(self,
+                   potential: Union[AbstractPotential, Atoms],
+                   pbar: bool = True,
+                   potential_chunks=1) -> Waves:
+        """
+        Build plane wave function and propagate it through the potential. The grid of the two will be matched.
+
+        Parameters
+        ----------
+        potential : Potential or Atoms object
+            The potential through which to propagate the wave function.
+        pbar : bool, optional
+            Display a progress bar. Default is True.
+
+        Returns
+        -------
+        Waves object
+            Wave function at the exit plane of the potential.
+        """
+
+        if isinstance(potential, Atoms):
+            potential = Potential(atoms=potential)
+        potential.grid.match(self)
+
+        return self.build().multislice(potential, pbar=pbar, potential_chunks=potential_chunks)
+
+    def build(self) -> Waves:
+        """Build the plane wave function as a Waves object."""
+        xp = get_array_module_from_device(self._device)
+        self.grid.check_is_defined()
+        array = xp.ones((1, self.gpts[0], self.gpts[1]), dtype=xp.complex64)
+        return Waves(array, extent=self.extent, energy=self.energy)
+
+    def __copy__(self, a) -> 'PlaneWave':
+        return self.__class__(extent=self.extent, gpts=self.gpts, sampling=self.sampling, energy=self.energy)
+
+    def copy(self):
+        """Make a copy."""
+        return copy(self)
+
+
+class Probe(_WavesLike, HasDeviceMixin):
+    """
+    Probe wave function object
+
+    The probe object can represent a stack of electron probe wave function for simulating scanning transmission
+    electron microscopy.
+
+    See the docs of abtem.transfer.CTF for a description of the parameters related to the contrast transfer function.
+
+    Parameters
+    ----------
+    extent : two float, optional
+        Lateral extent of wave functions [Å].
+    gpts : two int, optional
+        Number of grid points describing the wave functions.
+    sampling : two float, optional
+        Lateral sampling of wave functions [1 / Å].
+    energy : float, optional
+        Electron energy [eV].
+    device : str
+        The probe wave functions will be build on this device.
+    kwargs :
+        Provide the parameters of the contrast transfer function as keyword arguments. See the documentation for the
+        CTF object.
+    """
+
+    def __init__(self,
+                 extent: Union[float, Sequence[float]] = None,
+                 gpts: Union[int, Sequence[int]] = None,
+                 sampling: Union[float, Sequence[float]] = None,
+                 energy: float = None,
+                 ctf=None,
+                 device='cpu',
+                 **kwargs):
+
+        if ctf is None:
+            ctf = CTF(energy=energy, **kwargs)
+
+        if ctf.energy is None:
+            ctf.energy = energy
+
+        if ctf.energy != energy:
+            raise RuntimeError()
+
+        self._ctf = ctf
+        self._accelerator = self._ctf._accelerator
+
+        self._grid = Grid(extent=extent, gpts=gpts, sampling=sampling)
+
+        self.changed = Event()
+
+        self._ctf.changed.register(self.changed.notify)
+        self._grid.changed.register(self.changed.notify)
+        self._accelerator.changed.register(self.changed.notify)
+
+        self._device = device
+
+        self._ctf_cache = Cache(1)
+        self.changed.register(cache_clear_callback(self._ctf_cache))
+
+        super().__init__()
+
+    @property
+    def ctf(self) -> CTF:
+        """Probe contrast transfer function."""
+        return self._ctf
+
+    def _fourier_translation_operator(self, positions):
+        xp = get_array_module(positions)
+        complex_exponential = get_device_function(xp, 'complex_exponential')
+
+        kx, ky = spatial_frequencies(self.grid.gpts, self.grid.sampling)
+        kx = kx.reshape((1, -1, 1))
+        ky = ky.reshape((1, 1, -1))
+        kx = xp.asarray(kx)
+        ky = xp.asarray(ky)
+        positions = xp.asarray(positions)
+        x = positions[:, 0].reshape((-1,) + (1, 1))
+        y = positions[:, 1].reshape((-1,) + (1, 1))
+
+        return complex_exponential(2 * np.pi * kx * x) * complex_exponential(2 * np.pi * ky * y)
+
+    @cached_method('_ctf_cache')
+    def _evaluate_ctf(self, xp):
+        kx, ky = spatial_frequencies(self.grid.gpts, self.grid.sampling)
+        alpha, phi = polar_coordinates(xp.asarray(kx * self.wavelength), xp.asarray(ky * self.wavelength))
+        return self._ctf.evaluate(alpha, phi)
+
+    def build(self, positions: Sequence[Sequence[float]] = None) -> Waves:
+        """
+        Build probe wave functions at the provided positions.
+
+        Parameters
+        ----------
+        positions : array of xy-positions
+            Positions of the probe wave functions
+
+        Returns
+        -------
+        Waves object
+            Probe wave functions as a Waves object.
+        """
+
+        self.grid.check_is_defined()
+        self.accelerator.check_is_defined()
+        xp = get_array_module_from_device(self._device)
+        fft2 = get_device_function(xp, 'fft2')
+
+        if positions is None:
+            positions = xp.array((self.extent[0] / 2, self.extent[1] / 2), dtype=xp.float32)
+        else:
+            positions = xp.array(positions, dtype=xp.float32)
+
+        if len(positions.shape) == 1:
+            positions = xp.expand_dims(positions, axis=0)
+
+        array = fft2(self._evaluate_ctf(xp) * self._fourier_translation_operator(positions), overwrite_x=True)
+
+        return Waves(array, extent=self.extent, energy=self.energy)
+
+    def multislice(self, positions: Sequence[Sequence[float]], potential: AbstractPotential, pbar=True) -> Waves:
+        """
+        Build probe wave functions at the provided positions and propagate them through the potential.
+
+        Parameters
+        ----------
+        positions : array of xy-positions
+            Positions of the probe wave functions.
+        potential : Potential or Atoms object
+            The scattering potential.
+        pbar : bool, optional
+            Display progress bars. Default is True.
+
+        Returns
+        -------
+        Waves object
+            Probe exit wave functions as a Waves object.
+        """
+
+        if isinstance(potential, Atoms):
+            potential = Potential(potential)
+
+        self.grid.match(potential)
+        exit_probes = _multislice(self.build(positions), potential, None, pbar)
+        exit_probes._antialiasing_aperture = 2 / 3.
+        return exit_probes
+
+    def _generate_probes(self, scan: AbstractScan, potential: Union[AbstractPotential, Atoms], max_batch: int):
+        if not isinstance(max_batch, int):
+            memory_per_wave = 2 * 4 * np.prod(self.gpts)
+            available_memory = get_available_memory(self._device)
+            max_batch = min(int(available_memory * .4 / memory_per_wave), 32)
+
+        for indices, positions in scan.generate_positions(max_batch=max_batch):
+            yield indices, self.multislice(positions, potential, pbar=False)
+
+    def _generate_tds_probes(self, scan, potential, max_batch, pbar):
+        tds_bar = ProgressBar(total=len(potential.frozen_phonons), desc='TDS',
+                              disable=(not pbar) or (len(potential.frozen_phonons) == 1))
+        potential_pbar = ProgressBar(total=len(potential), desc='Potential', disable=not pbar)
+
+        for potential_config in potential.generate_frozen_phonon_potentials(pbar=potential_pbar):
+            yield self._generate_probes(scan, potential_config, max_batch)
+            tds_bar.update(1)
+
+        potential_pbar.close()
+        tds_bar.refresh()
+        tds_bar.close()
+
+    def scan(self,
+             scan: AbstractScan,
+             detectors: Union[AbstractDetector, Sequence[AbstractDetector]],
+             potential: Union[Atoms, AbstractPotential],
+             max_batch: int = None,
+             pbar: bool = True) -> dict:
+
+        """
+        Raster scan the probe across the potential and record a measurement for each detector.
+
+        Parameters
+        ----------
+        scan : Scan object
+            Scan object defining the positions of the probe wave functions.
+        detectors : List of detector objects
+            The detectors recording the measurements.
+        potential : Potential
+            The potential to scan the probe over.
+        max_batch : int, optional
+            The probe batch size. Larger batches are faster, but require more memory. Default is None.
+        pbar : bool, optional
+            Display progress bars. Default is True.
+
+        Returns
+        -------
+        dict
+            Dictionary of measurements with keys given by the detector.
+        """
+
+        self.grid.match(potential.grid)
+        self.grid.check_is_defined()
+
+        if isinstance(detectors, AbstractDetector):
+            detectors = [detectors]
+
+        scan_bar = ProgressBar(total=len(scan), desc='Scan', disable=not pbar)
+
+        if isinstance(potential, AbstractTDSPotentialBuilder):
+            probe_generators = self._generate_tds_probes(scan, potential, max_batch, pbar)
+        else:
+            if isinstance(potential, AbstractPotentialBuilder):
+                potential = potential.build(pbar=True)
+
+            probe_generators = [self._generate_probes(scan, potential, max_batch)]
+
+        measurements = {}
+        for probe_generator in probe_generators:
+            scan_bar.reset()
+            for indices, exit_probes in probe_generator:
+
+                for detector in detectors:
+                    new_measurement = detector.detect(exit_probes)
+
+                    if isinstance(potential, AbstractTDSPotentialBuilder):
+                        new_measurement /= len(potential.frozen_phonons)
+
+                    try:
+                        scan.insert_new_measurement(measurements[detector], indices, new_measurement)
+                    except KeyError:
+                        measurements[detector] = detector.allocate_measurement(exit_probes, scan)
+                        scan.insert_new_measurement(measurements[detector], indices, new_measurement)
+
+                scan_bar.update(len(indices))
+
+            scan_bar.refresh()
+
+        scan_bar.close()
+        return measurements
+
+    def profile(self, angle=0.):
+        self.grid.check_is_defined()
+        measurement = self.build((self.extent[0] / 2, self.extent[1] / 2)).intensity()
+        return probe_profile(measurement, angle=angle)
+
+    def interact(self, sliders=None, profile=False, throttling=False):
+        from abtem.visualize.bqplot import show_measurement_1d, show_measurement_2d
+        from abtem.visualize.widgets import quick_sliders, throttle
+        import ipywidgets as widgets
+
+        if profile:
+            figure, callback = show_measurement_1d(lambda: [self.profile()])
+        else:
+            figure, callback = show_measurement_2d(lambda: self.build().intensity())
+
+        if throttling:
+            callback = throttle(throttling)(callback)
+
+        self.changed.register(callback)
+
+        if sliders:
+            sliders = quick_sliders(self.ctf, **sliders)
+            return widgets.HBox([figure, widgets.VBox(sliders)])
+        else:
+            return figure
+
+    def __copy__(self):
+        return self.__class__(gpts=self.gpts,
+                              extent=self.extent,
+                              sampling=self.sampling,
+                              energy=self.energy,
+                              ctf=self.ctf.copy(),
+                              device=self.device)
+
+    def copy(self):
+        return copy(self)
+
+    def show(self, **kwargs):
+        """
+        Show the probe wave function.
+
+        Parameters
+        ----------
+        angle : float, optional
+            Angle along which the profile is shown [deg]. Default is 0 degrees.
+        kwargs : Additional keyword arguments for the abtem.plot.show_image function.
+        """
+        self.grid.check_is_defined()
+        return self.build((self.extent[0] / 2, self.extent[1] / 2)).intensity().show(**kwargs)
+
+
+class SMatrixArray(_WavesLike, HasDeviceMixin):
+    """
+    Scattering matrix array object.
+
+    The scattering matrix array object represents a plane wave expansion of a probe, it is used for STEM simulations
+    with the PRISM algorithm.
+
+    Parameters
+    ----------
+    array : 3d array
+        The array representation of the scattering matrix.
+    expansion_cutoff : float
+        The angular cutoff of the plane wave expansion [mrad].
+    energy : float
+        Electron energy [eV].
+    interpolation : one or two int
+        Interpolation factor.
+    k : 2d array
+        The spatial frequencies of each plane in the plane wave expansion.
+    ctf : CTF object, optional
+        The probe contrast transfer function. Default is None.
+    extent : one or two float, optional
+        Lateral extent of wave functions [Å]. Default is None (inherits extent from the potential).
+    sampling : one or two float, optional
+        Lateral sampling of wave functions [1 / Å]. Default is None (inherits sampling from the potential).
+    device : str, optional
+        The calculations will be carried out on this device. Default is 'cpu'.
+    """
+
+    def __init__(self,
+                 array: np.ndarray,
+                 expansion_cutoff: float,
+                 energy: float,
+                 k: np.ndarray,
+                 interpolation: int = None,
+                 ctf: CTF = None,
+                 sampling: Union[float, Sequence[float]] = None,
+                 extent: Union[float, Sequence[float]] = None,
+                 periodic: bool = True,
+                 offset: Sequence[float] = None,
+                 cropped_shape: Tuple[int, int] = None,
+                 antialiasing_aperture: float = None,
+                 device: str = 'cpu'):
+
+        if ctf is None:
+            ctf = CTF()
+
+        if ctf.energy is None:
+            ctf.energy = energy
+
+        if (ctf.energy != energy):
+            raise RuntimeError
+
+        self._ctf = ctf
+        self._accelerator = self._ctf._accelerator
+
+        self._grid = Grid(extent=extent, gpts=array.shape[-2:], sampling=sampling, lock_gpts=True)
+        self.changed = Event()
+
+        self._ctf.changed.register(self.changed.notify)
+        self._grid.changed.register(self.changed.notify)
+        self._accelerator.changed.register(self.changed.notify)
+
+        self._device = device
+
+        self._array = array
+        self._antialiasing_aperture = antialiasing_aperture
+
+        self._expansion_cutoff = expansion_cutoff
+        self._k = k
+        self._periodic = periodic
+
+        if offset is None:
+            offset = (0, 0)
+
+        self._offset = np.array(offset, dtype=np.int)
+
+        if (cropped_shape is None) & (interpolation is not None):
+            cropped_shape = (self.gpts[0] // interpolation, self.gpts[1] // interpolation)
+
+        self._cropped_shape = cropped_shape
+
+        super().__init__(antialiasing_aperture=antialiasing_aperture)
+
+    @property
+    def ctf(self) -> CTF:
+        """Probe contrast transfer function."""
+        return self._ctf
+
+    @property
+    def array(self) -> np.ndarray:
+        """Array representing the scattering matrix."""
+        return self._array
+
+    @property
+    def antialiasing_aperture(self):
+        return self._antialiasing_aperture
+
+    @property
+    def k(self) -> np.ndarray:
+        """The spatial frequencies of each wave in the plane wave expansion."""
+        return self._k
+
+    @property
+    def expansion_cutoff(self) -> float:
+        """Expansion cutoff."""
+        return self._expansion_cutoff
+
+    @property
+    def periodic(self):
+        return self._periodic
+
+    @property
+    def cropped_grid(self):
+        return Grid(gpts=self.cropped_shape, sampling=self.sampling, lock_gpts=True)
+
+    @property
+    def cropped_shape(self) -> Tuple[int, int]:
+        """The grid of the interpolated scattering matrix."""
+        return self._cropped_shape
+
+    @property
+    def offset(self):
+        return self._offset
+
+    def __len__(self) -> int:
+        """Number of plane waves in expansion."""
+        return len(self._array)
+
+    def _raise_not_periodic(self):
+        raise RuntimeError('not implemented for non-periodic/cropped scattering matrices')
+
+    def downsample(self, max_angle='limit', normalization=None):
+        if not self.periodic:
+            self._raise_not_periodic()
+
+        xp = get_array_module(self.array)
+        gpts = next(self._generate_partial(1, pbar=False))[2].downsample(max_angle).gpts
+
+        new_array = xp.zeros((len(self.array),) + gpts, dtype=self.array.dtype)
+        max_batch = self._max_batch_expansion()
+
+        for start, end, partial_s_matrix in self._generate_partial(max_batch, pbar=False):
+            downsampled = partial_s_matrix.downsample(max_angle)
+            new_array[start:end] = copy_to_device(downsampled.array, xp)
+
+        if self.cropped_shape == self.gpts:
+            cropped_shape = gpts
+        else:
+            cropped_shape = tuple(n // (self.gpts[i] // self.cropped_shape[i]) for i, n in enumerate(gpts))
+
+        antialiasing_aperture = downsampled.antialiasing_aperture
+
+        return self.__class__(array=new_array,
+                              expansion_cutoff=self._expansion_cutoff,
+                              k=self.k.copy(),
+                              ctf=self.ctf,
+                              extent=self.extent,
+                              energy=self.energy,
+                              periodic=self.periodic,
+                              offset=self._offset,
+                              cropped_shape=cropped_shape,
+                              antialiasing_aperture=antialiasing_aperture,
+                              device=self.device)
+
+    def crop_to_scan(self, scan):
+
+        if not isinstance(scan, GridScan):
+            raise NotImplementedError()
+
+        crop_corner, size = self._get_requisite_crop(np.array([scan.start, scan.end]))
+        new_array = periodic_crop(self.array, crop_corner, size)
+
+        return self.__class__(array=new_array,
+                              expansion_cutoff=self._expansion_cutoff,
+                              interpolation=1,
+                              k=self.k.copy(),
+                              ctf=self.ctf,
+                              sampling=self.sampling,
+                              energy=self.energy,
+                              periodic=False,
+                              offset=crop_corner,
+                              cropped_shape=self.cropped_shape,
+                              device=self.device)
+
+    def _max_batch_expansion(self):
+        memory_per_wave = 2 * 4 * self.gpts[0] * self.gpts[1]
+        available_memory = .2 * get_available_memory(self._device)
+        return min(int(available_memory / memory_per_wave), len(self))
+
+    def _max_batch_probes(self):
+        max_batch_plane_waves = self._max_batch_expansion()
+        memory_per_wave = 2 * 4 * self.cropped_shape[0] * self.cropped_shape[1]
+        memory_per_plane_wave_batch = 2 * 4 * self.gpts[0] * self.gpts[1] * max_batch_plane_waves
+        available_memory = .2 * get_available_memory(self._device) - memory_per_plane_wave_batch
+        return max(min(int(available_memory / memory_per_wave), 1024), 1)
+
+    def _generate_partial(self, max_batch: int = None, pbar: Union[ProgressBar, bool] = True):
+        if max_batch is None:
+            n_batches = 1
+        else:
+            n_batches = (len(self) + (-len(self) % max_batch)) // max_batch
+
+        if isinstance(pbar, bool):
+            pbar = ProgressBar(total=len(self), desc='Plane waves', disable=(not pbar) or (n_batches == 1))
+            close_pbar = True
+        else:
+            pbar.reset()
+            close_pbar = False
+
+        batch_sizes = subdivide_into_batches(len(self), n_batches)
+
+        xp = get_array_module_from_device(self._device)
+
+        # if xp != get_array_module(self.array):
+        #     stream = xp.cuda.Stream(non_blocking=False)
+        #     partial_array = xp.empty((batch_sizes[0],) + self.gpts, dtype=xp.complex64)
+        #
+        # else:
+        #     stream = None
+        #     partial_array = None
+        # partial_array = xp.empty((batch_sizes[0],) + self.gpts, dtype=xp.complex64)
+
+        n = 0
+        for batch_size in batch_sizes:
+            start = n
+            end = n + batch_size
+
+            if xp != get_array_module(self.array):
+                yield start, end, Waves(copy_to_device(self._array[start:end], xp),
+                                        extent=self.extent, energy=self.energy)
+            else:
+                yield start, end, Waves(self._array[start:end], extent=self.extent, energy=self.energy)
+
+            # if stream is not None:
+            #     partial_array[:batch_size].set(self._array[start:end], stream=stream)
+            #     yield start, end, Waves(partial_array[:batch_size], extent=self.extent, energy=self.energy)
+            # #
+            # else:
+            #     yield start, end, Waves(self._array[start:end], extent=self.extent, energy=self.energy)
+
+            n += batch_size
+            pbar.update(batch_size)
+
+        pbar.refresh()
+        if close_pbar:
+            pbar.close()
+
+    def multislice(self,
+                   potential: AbstractPotential,
+                   max_batch=None,
+                   multislice_pbar: Union[ProgressBar, bool] = True,
+                   plane_waves_pbar: Union[ProgressBar, bool] = True):
+        """
+        Propagate the scattering matrix through the provided potential.
+
+        Parameters
+        ----------
+        potential : AbstractPotential object
+            Scattering potential.
+        max_batch : int, optional
+            The probe batch size. Larger batches are faster, but require more memory. Default is None.
+        multislice_pbar : bool, optional
+            Display multislice progress bar. Default is True.
+        plane_waves_pbar : bool, optional
+            Display plane waves progress bar. Default is True.
+
+        Returns
+        -------
+        Waves object.
+            Probe exit wave functions for the provided positions.
+        """
+
+        if not self.periodic:
+            self._raise_not_periodic()
+
+        if not isinstance(max_batch, int):
+            max_batch = self._max_batch_expansion()
+
+        if isinstance(multislice_pbar, bool):
+            multislice_pbar = ProgressBar(total=len(potential), desc='Multislice', disable=not multislice_pbar)
+            close_pbar = True
+        else:
+            close_pbar = False
+
+        propagator = FresnelPropagator()
+
+        for start, end, partial_s_matrix in self._generate_partial(max_batch, pbar=plane_waves_pbar):
+            _multislice(partial_s_matrix, potential, propagator=propagator, pbar=multislice_pbar)
+            self._array[start: end] = copy_to_device(partial_s_matrix.array, get_array_module(self._array))
+
+        self._antialiasing_aperture = 2 / 3.
+
+        if close_pbar:
+            multislice_pbar.close()
+        return self
+
+    def _get_ctf_coefficients(self):
+        xp = get_array_module(self._array)
+        alpha = xp.sqrt(self.k[:, 0] ** 2 + self.k[:, 1] ** 2) * self.wavelength
+        phi = xp.arctan2(self.k[:, 0], self.k[:, 1])
+        return self._ctf.evaluate(alpha, phi)
+
+    def _get_translation_coefficients(self, positions: Sequence[float]):
+        xp = get_array_module_from_device(self.device)
+        complex_exponential = get_device_function(xp, 'complex_exponential')
+        positions = xp.asarray(positions)
+        k = xp.asarray(self.k)
+        return (complex_exponential(2. * np.pi * k[:, 0][None] * positions[:, 0, None]) *
+                complex_exponential(2. * np.pi * k[:, 1][None] * positions[:, 1, None]))
+
+    def _get_coefficients(self, positions: Sequence[float]):
+        return self._get_translation_coefficients(positions) * self._get_ctf_coefficients()
+
+    def _get_requisite_crop(self, positions: Sequence[float], return_per_position: bool = False):
+        offset = (self.cropped_shape[0] // 2, self.cropped_shape[1] // 2)
+        corners = np.rint(np.array(positions) / self.sampling - offset).astype(np.int)
+        upper_corners = corners + np.asarray(self.cropped_shape)
+
+        crop_corner = (np.min(corners[:, 0]).item(), np.min(corners[:, 1]).item())
+
+        size = (np.max(upper_corners[:, 0]).item() - crop_corner[0],
+                np.max(upper_corners[:, 1]).item() - crop_corner[1])
+
+        if return_per_position:
+            return crop_corner, size, corners
+        else:
+            return crop_corner, size
+
+    def collapse(self, positions: Sequence[float], max_batch_expansion: int = None) -> Waves:
+        """
+        Collapse the scattering matrix to probe wave functions centered on the provided positions.
+
+        Parameters
+        ----------
+        positions : array of xy-positions
+            The positions of the probe wave functions.
+        max_batch_expansion : int, optional
+            The maximum number of plane waves the reduction is applied to simultanously. Default is None.
+
+        Returns
+        -------
+        Waves object
+            Probe wave functions for the provided positions.
+        """
+
+        if max_batch_expansion is None:
+            max_batch_expansion = self._max_batch_expansion()
+
+        xp = get_array_module_from_device(self.device)
+        positions = np.array(positions, dtype=xp.float32)
+
+        if positions.shape == (2,):
+            positions = positions[None]
+        elif (len(positions.shape) != 2) or (positions.shape[-1] != 2):
+            raise RuntimeError()
+
+        coefficients = self._get_coefficients(positions)
+
+        if self.cropped_shape != self.gpts:
+            crop_corner, size, corners = self._get_requisite_crop(positions, return_per_position=True)
+
+            if self._offset is not None:
+                corners -= self._offset
+                crop_corner = (crop_corner[0] - self._offset[0], crop_corner[1] - self._offset[1])
+
+            array = copy_to_device(periodic_crop(self.array, crop_corner, size), device=self._device)
+            window = xp.tensordot(coefficients, array, axes=[(1,), (0,)])
+
+            corners -= crop_corner
+            for i in range(len(corners)):
+                window[i, :self.cropped_shape[0], :self.cropped_shape[1]] = periodic_crop(window[i], corners[i],
+                                                                                          self.cropped_shape)
+
+            window = window[:, :self.cropped_shape[0], :self.cropped_shape[1]].copy()
+
+        elif max_batch_expansion <= len(self):
+            window = xp.zeros((len(positions),) + self.gpts, dtype=xp.complex64)
+            for start, end, partial_s_matrix in self._generate_partial(max_batch_expansion, pbar=False):
+                partial_coefficients = coefficients[:, start:end]
+                window += xp.tensordot(partial_coefficients, partial_s_matrix.array, axes=[(1,), (0,)])
+
+        else:
+            window = xp.tensordot(coefficients, copy_to_device(self.array, device=self._device), axes=[(1,), (0,)])
+            # window = xp.tensordot(coefficients, copy_to_device(self.array, device=self._device), axes=[(1,), (0,)])
+
+        return Waves(window, sampling=self.sampling, energy=self.energy,
+                     antialiasing_aperture=self.antialiasing_aperture)
+
+    def _generate_probes(self, scan: AbstractScan, max_batch_probes, max_batch_expansion):
+
+        if not isinstance(max_batch_expansion, int):
+            max_batch_expansion = self._max_batch_expansion()
+
+        if not isinstance(max_batch_probes, int):
+            max_batch_probes = self._max_batch_probes()
+
+        for indices, positions in scan.generate_positions(max_batch=max_batch_probes):
+            yield indices, self.collapse(positions, max_batch_expansion=max_batch_expansion)
+
+    def scan(self,
+             scan: AbstractScan,
+             detectors: Sequence[AbstractDetector],
+             max_batch_probes=None,
+             max_batch_expansion=None,
+             pbar: Union[ProgressBar, bool] = True):
+
+        """
+        Raster scan the probe across the potential and record a measurement for each detector.
+
+        Parameters
+        ----------
+        scan : Scan object
+            Scan defining the positions of the probe wave functions.
+        detectors : List of Detector objects
+            The detectors recording the measurements.
+        max_batch_probes : int, optional
+            The probe batch size. Larger batches are faster, but require more memory. Default is None.
+        max_batch_expansion : int, optional
+            The expansion plane wave batch size. Default is None.
+        pbar : bool, optional
+            Display progress bars. Default is True.
+
+        Returns
+        -------
+        dict
+            Dictionary of measurements with keys given by the detector.
+        """
+
+        if isinstance(detectors, dict):
+            measurements = detectors
+        else:
+            measurements = {}
+
+        if isinstance(pbar, bool):
+            pbar = ProgressBar(total=len(scan), desc='Scan', disable=not pbar)
+
+        for indices, exit_probes in self._generate_probes(scan, max_batch_probes, max_batch_expansion):
+            for detector in detectors:
+                # for detector, measurement in measurements.items():
+                new_measurement = detector.detect(exit_probes)
+                try:
+                    scan.insert_new_measurement(measurements[detector], indices, new_measurement)
+                except KeyError:
+                    measurements[detector] = detector.allocate_measurement(exit_probes, scan)
+                    scan.insert_new_measurement(measurements[detector], indices, new_measurement)
+
+            # scan.insert_new_measurement(measurement, indices, detector.detect(exit_probes))
+            pbar.update(len(indices))
+
+        pbar.refresh()
+        pbar.close()
+        return measurements
+
+    def transfer(self, device):
+        return self.__class__(array=copy_to_device(self.array, device),
+                              expansion_cutoff=self._expansion_cutoff,
+                              k=self.k.copy(),
+                              ctf=self.ctf.copy(),
+                              extent=self.extent,
+                              offset=self.offset,
+                              cropped_shape=self.cropped_shape,
+                              energy=self.energy,
+                              antialiasing_aperture=self.antialiasing_aperture,
+                              device=self.device)
+
+    def __copy__(self, device=None):
+        return self.__class__(array=self.array.copy(),
+                              expansion_cutoff=self._expansion_cutoff,
+                              k=self.k.copy(),
+                              ctf=self.ctf.copy(),
+                              extent=self.extent,
+                              offset=self.offset,
+                              cropped_shape=self.cropped_shape,
+                              energy=self.energy,
+                              antialiasing_aperture=self.antialiasing_aperture,
+                              device=self.device)
+
+    def copy(self):
+        """Make a copy."""
+        return copy(self)
+
+
+class SMatrix(_WavesLike, HasDeviceMixin):
+    """
+    Scattering matrix builder class
+
+    The scattering matrix builder object is used for creating scattering matrices and simulating STEM experiments using
+    the PRISM algorithm.
+
+    Parameters
+    ----------
+    expansion_cutoff : float
+        The angular cutoff of the plane wave expansion [mrad].
+    energy : float
+        Electron energy [eV].
+    interpolation : one or two int, optional
+        Interpolation factor. Default is 1 (no interpolation).
+    ctf: CTF object, optional
+        The probe contrast transfer function. Default is None (aperture is set by the cutoff of the expansion).
+    extent : one or two float, optional
+        Lateral extent of wave functions [Å]. Default is None (inherits the extent from the potential).
+    gpts : one or two int, optional
+        Number of grid points describing the wave functions. Default is None (inherits the gpts from the potential).
+    sampling : one or two float, None
+        Lateral sampling of wave functions [1 / Å]. Default is None (inherits the sampling from the potential.
+    device : str, optional
+        The calculations will be carried out on this device. Default is 'cpu'.
+    storage : str, optional
+        The scattering matrix will be stored on this device. Default is None (uses the option chosen for device).
+    kwargs :
+        The parameters of a new CTF object as keyword arguments.
+    """
+
+    def __init__(self,
+                 expansion_cutoff: float,
+                 energy: float,
+                 interpolation: int = 1,
+                 ctf: CTF = None,
+                 extent: Union[float, Sequence[float]] = None,
+                 gpts: Union[int, Sequence[int]] = None,
+                 sampling: Union[float, Sequence[float]] = None,
+                 device: str = 'cpu',
+                 storage: str = None,
+                 **kwargs):
+
+        if not isinstance(interpolation, int):
+            raise ValueError('Interpolation factor must be int')
+
+        self._interpolation = interpolation
+        self._expansion_cutoff = expansion_cutoff
+
+        if ctf is None:
+            ctf = CTF(**kwargs)
+
+        if ctf.energy is None:
+            ctf.energy = energy
+
+        if (ctf.energy != energy):
+            raise RuntimeError
+
+        self._ctf = ctf
+        self._accelerator = self._ctf._accelerator
+
+        self._grid = Grid(extent=extent, gpts=gpts, sampling=sampling)
+
+        self.changed = Event()
+
+        self._ctf.changed.register(self.changed.notify)
+        self._grid.changed.register(self.changed.notify)
+        self._accelerator.changed.register(self.changed.notify)
+
+        self._device = device
+        if storage is None:
+            storage = device
+
+        self._storage = storage
+
+        super().__init__()
+
+    @property
+    def ctf(self):
+        """The contrast transfer function of the probes."""
+        return self._ctf
+
+    @ctf.setter
+    def ctf(self, value):
+        self._ctf = value
+
+    @property
+    def expansion_cutoff(self) -> float:
+        """Plane wave expansion cutoff."""
+        return self._expansion_cutoff
+
+    @expansion_cutoff.setter
+    def expansion_cutoff(self, value: float):
+        self._expansion_cutoff = value
+
+    @property
+    def interpolation(self) -> int:
+        """Interpolation factor."""
+        return self._interpolation
+
+    @interpolation.setter
+    def interpolation(self, value: int):
+        self._interpolation = value
+
+    @property
+    def interpolated_grid(self) -> Grid:
+        """The grid of the interpolated probe wave functions."""
+        interpolated_gpts = tuple(n // self.interpolation for n in self.gpts)
+        return Grid(gpts=interpolated_gpts, sampling=self.sampling, lock_gpts=True)
+
+    def _generate_tds_probes(self,
+                             scan: AbstractScan,
+                             potential: AbstractTDSPotentialBuilder,
+                             max_batch_probes: int,
+                             max_batch_expansion: int,
+                             potential_pbar: Union[ProgressBar, bool] = True,
+                             plane_waves_pbar: Union[ProgressBar, bool] = True):
+
+        if isinstance(potential_pbar, bool):
+            potential_pbar = ProgressBar(total=len(potential), desc='Potential', disable=not potential_pbar)
+
+        if isinstance(plane_waves_pbar, bool):
+            plane_waves_pbar = ProgressBar(total=len(self), desc='Multislice', disable=not plane_waves_pbar)
+
+        for potential_config in potential.generate_frozen_phonon_potentials(pbar=potential_pbar):
+            S = self.build()
+
+            S = S.multislice(potential_config,
+                             max_batch=max_batch_expansion,
+                             multislice_pbar=False,
+                             plane_waves_pbar=plane_waves_pbar)
+
+            S = S.downsample('limit')
+            yield S._generate_probes(scan, max_batch_probes, max_batch_expansion)
+
+        plane_waves_pbar.refresh()
+        plane_waves_pbar.close()
+
+        potential_pbar.refresh()
+        potential_pbar.close()
+
+    def multislice(self,
+                   potential: AbstractPotential,
+                   max_batch: int = None,
+                   pbar: Union[ProgressBar, bool] = True):
+        """
+        Build scattering matrix and propagate the scattering matrix through the provided potential.
+
+        Parameters
+        ----------
+        potential : AbstractPotential
+            Scattering potential.
+        max_batch : int, optional
+            The probe batch size. Larger batches are faster, but require more memory. Default is None.
+        pbar : bool, optional
+            Display progress bars. Default is True.
+
+        Returns
+        -------
+        Waves object
+            Probe exit wave functions as a Waves object.
+        """
+
+        if isinstance(potential, Atoms):
+            potential = Potential(potential)
+
+        self.grid.match(potential)
+        return self.build().multislice(potential,
+                                       max_batch=max_batch,
+                                       multislice_pbar=pbar,
+                                       plane_waves_pbar=pbar)
+
+    def scan(self,
+             scan: AbstractScan,
+             detectors: Sequence[AbstractDetector],
+             potential: Union[Atoms, AbstractPotential],
+             max_batch_probes: int = None,
+             max_batch_expansion: int = None,
+             pbar: bool = True):
+        """
+        Build the scattering matrix. Raster scan the probe across the potential, record a measurement for each detector.
+
+        Parameters
+        ----------
+        scan : Scan object
+            Scan defining the positions of the probe wave functions.
+        detectors : List of Detector objects
+            The detectors recording the measurements.
+        potential : Potential object
+            The potential to scan the probe over.
+        max_batch_probes : int, optional
+            The probe batch size. Larger batches are faster, but require more memory. Default is None.
+        max_batch_expansion : int, optional
+            The expansion plane wave batch size. Default is None.
+        pbar : bool, optional
+            Display progress bars. Default is True.
+
+        Returns
+        -------
+        dict
+            Dictionary of measurements with keys given by the detector.
+        """
+
+        self.grid.match(potential.grid)
+        self.grid.check_is_defined()
+
+        if isinstance(potential, AbstractTDSPotentialBuilder):
+            probe_generators = self._generate_tds_probes(scan,
+                                                         potential,
+                                                         max_batch_probes=max_batch_probes,
+                                                         max_batch_expansion=max_batch_expansion,
+                                                         potential_pbar=True,
+                                                         multislice_pbar=True)
+
+            tds_bar = ProgressBar(total=len(potential.frozen_phonons), desc='TDS',
+                                  disable=(not pbar) or (len(potential.frozen_phonons) == 1))
+
+        else:
+            if isinstance(potential, AbstractPotentialBuilder):
+                potential = potential.build(pbar=True)
+
+            S = self.multislice(potential, max_batch=max_batch_expansion, pbar=pbar)
+            probe_generators = [S._generate_probes(scan,
+                                                   max_batch_probes=max_batch_probes,
+                                                   max_batch_expansion=max_batch_expansion)]
+
+            tds_bar = None
+
+        scan_bar = ProgressBar(total=len(scan), desc='Scan', disable=not pbar)
+
+        measurements = {}
+        for probe_generator in probe_generators:
+            scan_bar.reset()
+
+            for indices, exit_probes in probe_generator:
+                for detector in detectors:
+                    new_measurement = detector.detect(exit_probes)
+
+                    if isinstance(potential, AbstractTDSPotentialBuilder):
+                        new_measurement /= len(potential.frozen_phonons)
+
+                    try:
+                        scan.insert_new_measurement(measurements[detector], indices, new_measurement)
+                    except KeyError:
+                        measurements[detector] = detector.allocate_measurement(exit_probes, scan)
+                        scan.insert_new_measurement(measurements[detector], indices, new_measurement)
+
+                scan_bar.update(len(indices))
+
+            scan_bar.refresh()
+            if tds_bar:
+                tds_bar.update(1)
+
+        scan_bar.close()
+
+        if tds_bar:
+            tds_bar.refresh()
+            tds_bar.close()
+
+        return measurements
+
+    def __len__(self):
+        return len(self.k)
+
+    @property
+    def k(self):
+        xp = get_array_module_from_device(self._device)
+        n_max = int(
+            xp.ceil(self.expansion_cutoff / 1000. / (self.wavelength / self.extent[0] * self.interpolation)))
+        m_max = int(
+            xp.ceil(self.expansion_cutoff / 1000. / (self.wavelength / self.extent[1] * self.interpolation)))
+
+        n = xp.arange(-n_max, n_max + 1, dtype=xp.float32)
+        w = xp.asarray(self.extent[0], dtype=xp.float32)
+        m = xp.arange(-m_max, m_max + 1, dtype=xp.float32)
+        h = xp.asarray(self.extent[1], dtype=xp.float32)
+
+        kx = n / w * xp.float32(self.interpolation)
+        ky = m / h * xp.float32(self.interpolation)
+
+        mask = kx[:, None] ** 2 + ky[None, :] ** 2 < (self.expansion_cutoff / 1000. / self.wavelength) ** 2
+        kx, ky = xp.meshgrid(kx, ky, indexing='ij')
+        kx = kx[mask]
+        ky = ky[mask]
+        return xp.asarray((kx, ky)).T
+
+    def build(self) -> SMatrixArray:
+        """Build the scattering matrix."""
+
+        self.grid.check_is_defined()
+        self.accelerator.check_is_defined()
+        xp = get_array_module_from_device(self._device)
+        storage_xp = get_array_module_from_device(self._storage)
+        complex_exponential = get_device_function(xp, 'complex_exponential')
+
+        x = xp.linspace(0, self.extent[0], self.gpts[0], endpoint=self.grid.endpoint[0], dtype=xp.float32)
+        y = xp.linspace(0, self.extent[1], self.gpts[1], endpoint=self.grid.endpoint[1], dtype=xp.float32)
+
+        k = self.k
+
+        shape = (len(k),) + self.gpts
+        array = storage_xp.zeros(shape, dtype=np.complex64)
+
+        for i in range(len(k)):
+            array[i] = copy_to_device(complex_exponential(-2 * np.pi * k[i, 0, None, None] * x[:, None]) *
+                                      complex_exponential(-2 * np.pi * k[i, 1, None, None] * y[None, :]),
+                                      self._storage)
+
+        return SMatrixArray(array,
+                            expansion_cutoff=self.expansion_cutoff,
+                            interpolation=self.interpolation,
+                            extent=self.extent,
+                            energy=self.energy,
+                            k=k,
+                            ctf=self.ctf.copy(),
+                            device=self._device)
+
+    def profile(self, angle=0.):
+        measurement = self.build().collapse((self.extent[0] / 2, self.extent[1] / 2)).intensity()
+        return probe_profile(measurement, angle=angle)
+
+    def interact(self, sliders=None, profile=False):
+        from abtem.visualize.bqplot import show_measurement_1d, show_measurement_2d
+        from abtem.visualize.widgets import quick_sliders
+        import ipywidgets as widgets
+
+        if profile:
+            figure, callback = show_measurement_1d(lambda: [self.profile()])
+        else:
+            figure, callback = show_measurement_2d(lambda: self.build().collapse((self.extent[0] / 2,
+                                                                                  self.extent[1] / 2)).intensity())
+
+        self.changed.register(callback)
+
+        if sliders:
+            sliders = quick_sliders(self.ctf, **sliders)
+            return widgets.HBox([figure, widgets.VBox(sliders)])
+        else:
+            return figure
+
+    def show(self, **kwargs):
+        """
+        Show the probe wave function.
+
+        Parameters
+        ----------
+        angle : float, optional
+            Angle along which the profile is shown [deg]. Default is 0 degrees.
+        kwargs : Additional keyword arguments for the abtem.plot.show_image function.
+        """
+        return self.build().collapse((self.extent[0] / 2, self.extent[1] / 2)).intensity().show(**kwargs)
+
+    def __copy__(self):
+        return self.__class__(expansion_cutoff=self.expansion_cutoff,
+                              interpolation=self.interpolation,
+                              ctf=self.ctf.copy(),
+                              extent=self.extent,
+                              gpts=self.gpts,
+                              energy=self.energy,
+                              device=self._device,
+                              storage=self._storage)
+
+    def copy(self):
+        """Make a copy."""
+        return copy(self)
```

### Comparing `abtem-1.0.0b8/abtem.egg-info/PKG-INFO` & `abtem-1.0.0b9/abtem.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,49 +1,55 @@
-Metadata-Version: 1.2
-Name: abtem
-Version: 1.0.0b8
-Summary: ab initio Transmission Electron Microscopy
-Home-page: https://github.com/jacobjma/abtem
-Author: Jacob Madsen
-Author-email: jacob.madsen@univie.ac.at
-Maintainer: Jacob Madsen
-Maintainer-email: jacob.madsen@univie.ac.at
-License: UNKNOWN
-Description: # abTEM: ab initio Transmission Electron Microscopy
-        
-        [![PyPI version](https://badge.fury.io/py/abtem.svg)](https://badge.fury.io/py/abtem)
-        [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
-        [![Documentation Status](https://readthedocs.org/projects/abtem/badge/?version=latest)](https://abtem.readthedocs.io/en/latest/?badge=latest)
-        [![Gitter](https://badges.gitter.im/abTEM/community.svg)](https://gitter.im/abTEM/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
-        
-        [**Docs**](https://abtem.readthedocs.io/en/latest/index.html)
-        | [**Install Guide**](https://abtem.readthedocs.io/en/latest/install.html)
-        | [**Examples**](https://github.com/jacobjma/abTEM/tree/master/examples)
-        | [**Gitter**](https://gitter.im/abTEM/)
-        
-        **This program is under development and subject to changes. Please be aware and report issues.**
-        
-        abTEM provides a Python API for running simulations of (scanning) transmission electron microscopy images and diffraction patterns using the multislice or PRISM algorithms. It is designed to closely integrate with atomistic simulations using the Atomic Simulation Environment (ASE), and to directly use *ab initio* electrostatic potentials from the high-performance density functional theory code GPAW.
-        
-        ## Installation
-        
-        You can install abTEM using `pip`:
-        
-        ```sh
-        $ pip install abtem
-        ```
-        
-        For detailed instructions on installing abTEM, see [the installation guide](https://abtem.readthedocs.io/en/latest/install.html).
-        
-        ## Getting started
-        
-        To get started using abTEM, please visit our [walkthrough](https://abtem.readthedocs.io/en/latest/walkthrough/introduction.html).
-        
-        ## Contact
-        * Chat on [gitter](https://gitter.im/abTEM/)
-        * Write the [maintainer](https://github.com/jacobjma) directly
-        * Bug reports and development: [github issues](https://github.com/jacobjma/abTEM/issues)
-        
-        Please send us bug reports, patches, code, ideas and questions.
-        
-Platform: any
-Requires-Python: >=3.6
+Metadata-Version: 1.2
+Name: abtem
+Version: 1.0.0b9
+Summary: ab initio Transmission Electron Microscopy
+Home-page: https://github.com/jacobjma/abtem
+Author: Jacob Madsen
+Author-email: jacob.madsen@univie.ac.at
+Maintainer: Jacob Madsen
+Maintainer-email: jacob.madsen@univie.ac.at
+License: UNKNOWN
+Description: # abTEM: ab initio Transmission Electron Microscopy
+        
+        [![PyPI version](https://badge.fury.io/py/abtem.svg)](https://badge.fury.io/py/abtem)
+        [![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
+        [![Documentation Status](https://readthedocs.org/projects/abtem/badge/?version=latest)](https://abtem.readthedocs.io/en/latest/?badge=latest)
+        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jacobjma/abTEM/master?filepath=examples%2Findex.ipynb)
+        [![Gitter](https://badges.gitter.im/abTEM/community.svg)](https://gitter.im/abTEM/community?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge)
+        
+        [**Docs**](https://abtem.readthedocs.io/en/latest/index.html)
+        | [**Install Guide**](https://abtem.readthedocs.io/en/latest/install.html)
+        | [**Examples**](https://github.com/jacobjma/abTEM/tree/master/examples)
+        | [**Gitter**](https://gitter.im/abTEM/)
+        
+        **This program is under development and subject to changes. Please be aware and report issues.**
+        
+        abTEM provides a Python API for running simulations of (scanning) transmission electron microscopy images and diffraction patterns using the multislice or PRISM algorithms. It is designed to closely integrate with atomistic simulations using the Atomic Simulation Environment (ASE), and to directly use *ab initio* electrostatic potentials from the high-performance density functional theory code GPAW.
+        
+        ## Installation
+        
+        You can install abTEM using `pip`:
+        
+        ```sh
+        $ pip install abtem
+        ```
+        
+        For detailed instructions on installing abTEM, see [the installation guide](https://abtem.readthedocs.io/en/latest/install.html).
+        
+        ## Getting started
+        
+        To get started using abTEM, please visit our [walkthrough](https://abtem.readthedocs.io/en/latest/walkthrough/introduction.html) or check out one of the [examples](https://github.com/jacobjma/abTEM/tree/master/examples).
+        
+        To try abTEM in your webbrowser, click the binder link:
+        
+        [![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/jacobjma/abTEM/master?filepath=examples%2Findex.ipynb)
+        
+        
+        ## Contact
+        * Chat on [gitter](https://gitter.im/abTEM/)
+        * Write the [maintainer](https://github.com/jacobjma) directly
+        * Bug reports and development: [github issues](https://github.com/jacobjma/abTEM/issues)
+        
+        Please send us bug reports, patches, code, ideas and questions.
+        
+Platform: any
+Requires-Python: >=3.6
```

### Comparing `abtem-1.0.0b8/abtem.egg-info/SOURCES.txt` & `abtem-1.0.0b9/abtem.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 abtem/_version.py
 abtem/base_classes.py
 abtem/cpu_kernels.py
 abtem/cuda_kernels.py
 abtem/detect.py
 abtem/device.py
 abtem/dft.py
+abtem/interpolate.py
 abtem/measure.py
 abtem/noise.py
 abtem/parametrizations.py
 abtem/plot.py
 abtem/potentials.py
 abtem/scan.py
 abtem/structures.py
@@ -40,14 +41,15 @@
 test/test_ctf.py
 test/test_detect.py
 test/test_dft.py
 test/test_energy.py
 test/test_event.py
 test/test_export.py
 test/test_grid.py
+test/test_interpolate.py
 test/test_kirkland.py
 test/test_potential_integration.py
 test/test_potential_parametrization.py
 test/test_potentials.py
 test/test_prism.py
 test/test_propagator.py
 test/test_scan.py
```

### Comparing `abtem-1.0.0b8/setup.py` & `abtem-1.0.0b9/setup.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import os
-from io import open as io_open
-
-from setuptools import setup, find_packages
-
-__version__ = None
-src_dir = os.path.abspath(os.path.dirname(__file__))
-version_file = os.path.join(src_dir, 'abtem', '_version.py')
-with io_open(version_file, mode='r') as fd:
-    exec(fd.read())
-
-fndoc = os.path.join(src_dir, 'README.md')
-with io_open(fndoc, mode='r', encoding='utf-8') as fd:
-    README_md = fd.read()
-
-setup(
-    name='abtem',
-    version=__version__,
-    description='ab initio Transmission Electron Microscopy',
-    long_description=README_md,
-    url='https://github.com/jacobjma/abtem',
-    author='Jacob Madsen',
-    author_email='jacob.madsen@univie.ac.at',
-    maintainer='Jacob Madsen',
-    maintainer_email='jacob.madsen@univie.ac.at',
-    platforms=['any'],
-    python_requires='>=3.6',
-    install_requires=[
-        'numpy',
-        'scipy',
-        'numba',
-        'imageio',
-        'pyfftw',
-        'h5py',
-        'matplotlib',
-        'ase',
-        'tqdm',
-        'psutil'],
-    tests_require=['pytest'],
-    packages=find_packages(),
-    include_package_data=True,
-)
+import os
+from io import open as io_open
+
+from setuptools import setup, find_packages
+
+__version__ = None
+src_dir = os.path.abspath(os.path.dirname(__file__))
+version_file = os.path.join(src_dir, 'abtem', '_version.py')
+with io_open(version_file, mode='r') as fd:
+    exec(fd.read())
+
+fndoc = os.path.join(src_dir, 'README.md')
+with io_open(fndoc, mode='r', encoding='utf-8') as fd:
+    README_md = fd.read()
+
+setup(
+    name='abtem',
+    version=__version__,
+    description='ab initio Transmission Electron Microscopy',
+    long_description=README_md,
+    url='https://github.com/jacobjma/abtem',
+    author='Jacob Madsen',
+    author_email='jacob.madsen@univie.ac.at',
+    maintainer='Jacob Madsen',
+    maintainer_email='jacob.madsen@univie.ac.at',
+    platforms=['any'],
+    python_requires='>=3.6',
+    install_requires=[
+        'numpy',
+        'scipy',
+        'numba',
+        'imageio',
+        'pyfftw',
+        'h5py',
+        'matplotlib',
+        'ase',
+        'tqdm',
+        'psutil'],
+    tests_require=['pytest'],
+    packages=find_packages(),
+    include_package_data=True,
+)
```

### Comparing `abtem-1.0.0b8/test/test_antialias.py` & `abtem-1.0.0b9/test/test_antialias.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,46 +1,46 @@
-from abtem.base_classes import AntialiasFilter
-import numpy as np
-from ase import Atoms
-from abtem.waves import Probe
-
-
-# def test_crop():
-#     f = AntialiasFilter()
-#
-#     assert np.all(f.crop(f.get_mask((128, 128), (.1, .1), np), (.1, .1), 'valid'))
-#     assert np.all(f.crop(f.get_mask((128, 128), (.1, .1), np), (.1, .1), 'valid'))
-#
-#     f = AntialiasFilter(rolloff=0.)
-#     mask_sum = f.get_mask((128, 128), (.1, .1), np).sum()
-#     assert f.crop(f.get_mask((128, 128), (.1, .1), np), (.1, .1), 'limit').sum() == mask_sum
-#     assert f.crop(f.get_mask((128, 128), (.1, .1), np), (.1, .1), 'limit').sum() == mask_sum
-
-
-def test_bandlimit():
-    atoms = Atoms(cell=(10, 10, 2))
-
-    probe = Probe(energy=300e3, semiangle_cutoff=30, rolloff=0.0, gpts=100)
-
-    #alpha_x = np.fft.fftfreq(probe.gpts[0], probe.sampling[0]) * probe.wavelength * 1000
-    #alpha_y = np.fft.fftfreq(probe.gpts[1], probe.sampling[1]) * probe.wavelength * 1000
-
-    #alpha = np.sqrt(alpha_x[:, None] ** 2 + alpha_y[None] ** 2)
-
-    #np.sum(alpha < 30)
-
-    waves = probe.multislice((0, 0), atoms, pbar=False)
-    diffraction_pattern = waves.diffraction_pattern(max_angle=30)
-
-    assert diffraction_pattern.shape == (1, 31, 31)
-
-    probe = Probe(energy=300e3, semiangle_cutoff=1e3, rolloff=0.0, gpts=100)
-    waves = probe.multislice((0, 0), atoms, pbar=False)
-
-    diffraction_pattern = waves.diffraction_pattern('limit')
-    assert not np.allclose(diffraction_pattern.array / diffraction_pattern.array.max(), 1.)
-    assert diffraction_pattern.shape == (1, 67, 67)
-
-    diffraction_pattern = waves.diffraction_pattern('valid')
-
-    assert diffraction_pattern.shape == (1, 45, 45)
-    assert np.allclose(diffraction_pattern.array / diffraction_pattern.array.max(), 1.)
+from abtem.base_classes import AntialiasFilter
+import numpy as np
+from ase import Atoms
+from abtem.waves import Probe
+
+
+# def test_crop():
+#     f = AntialiasFilter()
+#
+#     assert np.all(f.crop(f.get_mask((128, 128), (.1, .1), np), (.1, .1), 'valid'))
+#     assert np.all(f.crop(f.get_mask((128, 128), (.1, .1), np), (.1, .1), 'valid'))
+#
+#     f = AntialiasFilter(rolloff=0.)
+#     mask_sum = f.get_mask((128, 128), (.1, .1), np).sum()
+#     assert f.crop(f.get_mask((128, 128), (.1, .1), np), (.1, .1), 'limit').sum() == mask_sum
+#     assert f.crop(f.get_mask((128, 128), (.1, .1), np), (.1, .1), 'limit').sum() == mask_sum
+
+
+def test_bandlimit():
+    atoms = Atoms(cell=(10, 10, 2))
+
+    probe = Probe(energy=300e3, semiangle_cutoff=30, rolloff=0.0, gpts=100)
+
+    #alpha_x = np.fft.fftfreq(probe.gpts[0], probe.sampling[0]) * probe.wavelength * 1000
+    #alpha_y = np.fft.fftfreq(probe.gpts[1], probe.sampling[1]) * probe.wavelength * 1000
+
+    #alpha = np.sqrt(alpha_x[:, None] ** 2 + alpha_y[None] ** 2)
+
+    #np.sum(alpha < 30)
+
+    waves = probe.multislice((0, 0), atoms, pbar=False)
+    diffraction_pattern = waves.diffraction_pattern(max_angle=30)
+
+    assert diffraction_pattern.shape == (1, 31, 31)
+
+    probe = Probe(energy=300e3, semiangle_cutoff=1e3, rolloff=0.0, gpts=100)
+    waves = probe.multislice((0, 0), atoms, pbar=False)
+
+    diffraction_pattern = waves.diffraction_pattern('limit')
+    assert not np.allclose(diffraction_pattern.array / diffraction_pattern.array.max(), 1.)
+    assert diffraction_pattern.shape == (1, 67, 67)
+
+    diffraction_pattern = waves.diffraction_pattern('valid')
+
+    assert diffraction_pattern.shape == (1, 45, 45)
+    assert np.allclose(diffraction_pattern.array / diffraction_pattern.array.max(), 1.)
```

### Comparing `abtem-1.0.0b8/test/test_ctf.py` & `abtem-1.0.0b9/test/test_ctf.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,63 @@
-import numpy as np
-import pytest
-
-from abtem.base_classes import energy2wavelength
-from abtem.transfer import CTF, polar_aliases, scherzer_defocus, polar_symbols
-
-
-def test_scherzer():
-    Cs = np.random.rand() * 1e5
-    defocus = scherzer_defocus(Cs, 80e3)
-    parameters = {'C10': -defocus, 'C30': Cs}
-    alpha = (6 * energy2wavelength(80e3) / Cs) ** (1 / 4.)
-
-    ctf = CTF(energy=80e3, parameters=parameters)
-    assert np.isclose(ctf.evaluate_chi(alpha, 0.), 0, atol=1e-6)
-
-
-def test_scherzer_kwargs():
-    Cs = np.random.rand() * 1e5
-    defocus = scherzer_defocus(Cs, 80e3)
-    alpha = (6 * energy2wavelength(80e3) / Cs) ** (1 / 4.)
-
-    ctf = CTF(energy=80e3, defocus=defocus, Cs=Cs)
-    assert np.isclose(ctf.evaluate_chi(alpha, 0.), 0, atol=1e-6)
-
-
-def test_aperture():
-    ctf = CTF(semiangle_cutoff=20, rolloff=0., energy=80e3)
-    assert ctf.evaluate_aperture(.021) == 0
-    assert ctf.evaluate_aperture(.019) == 1
-
-
-def test_ctf_base_aliases():
-    random_parameters = dict(zip(polar_symbols, np.random.rand(len(polar_symbols))))
-    parameter_aliases = {alias: random_parameters[key] for alias, key in polar_aliases.items()}
-
-    CTF(parameters=random_parameters)
-    CTF(**random_parameters)
-
-    CTF(parameters=parameter_aliases)
-    CTF(**parameter_aliases)
-
-
-def test_ctf_raises():
-    with pytest.raises(ValueError) as e:
-        CTF(not_a_parameter=10)
-
-    assert str(e.value) == 'not_a_parameter not a recognized parameter'
-
-    ctf = CTF()
-    with pytest.raises(RuntimeError) as e:
-        ctf.evaluate(np.array([0]), np.array([0]))
-
-    assert str(e.value) == 'Energy is not defined'
-
-    ctf.energy = 200e3
-    ctf.evaluate(np.array([0]), np.array([0]))
-
-
-def test_ctf_event():
-    ctf = CTF(energy=80e3)
-    ctf.semiangle_cutoff = 1
-    assert ctf.changed.notify_count == 2
+import numpy as np
+import pytest
+
+from abtem.base_classes import energy2wavelength
+from abtem.transfer import CTF, polar_aliases, scherzer_defocus, polar_symbols
+
+
+def test_scherzer():
+    Cs = np.random.rand() * 1e5
+    defocus = scherzer_defocus(Cs, 80e3)
+    parameters = {'C10': -defocus, 'C30': Cs}
+    alpha = (6 * energy2wavelength(80e3) / Cs) ** (1 / 4.)
+
+    ctf = CTF(energy=80e3, parameters=parameters)
+    assert np.isclose(ctf.evaluate_chi(alpha, 0.), 0, atol=1e-6)
+
+
+def test_scherzer_kwargs():
+    Cs = np.random.rand() * 1e5
+    defocus = scherzer_defocus(Cs, 80e3)
+    alpha = (6 * energy2wavelength(80e3) / Cs) ** (1 / 4.)
+
+    ctf = CTF(energy=80e3, defocus=defocus, Cs=Cs)
+    assert np.isclose(ctf.evaluate_chi(alpha, 0.), 0, atol=1e-6)
+
+
+def test_aperture():
+    ctf = CTF(semiangle_cutoff=20, rolloff=0., energy=80e3)
+    assert ctf.evaluate_aperture(.021) == 0
+    assert ctf.evaluate_aperture(.019) == 1
+
+
+def test_ctf_base_aliases():
+    random_parameters = dict(zip(polar_symbols, np.random.rand(len(polar_symbols))))
+    parameter_aliases = {alias: random_parameters[key] for alias, key in polar_aliases.items()}
+
+    CTF(parameters=random_parameters)
+    CTF(**random_parameters)
+
+    CTF(parameters=parameter_aliases)
+    CTF(**parameter_aliases)
+
+
+def test_ctf_raises():
+    with pytest.raises(ValueError) as e:
+        CTF(not_a_parameter=10)
+
+    assert str(e.value) == 'not_a_parameter not a recognized parameter'
+
+    ctf = CTF()
+    with pytest.raises(RuntimeError) as e:
+        ctf.evaluate(np.array([0]), np.array([0]))
+
+    assert str(e.value) == 'Energy is not defined'
+
+    ctf.energy = 200e3
+    ctf.evaluate(np.array([0]), np.array([0]))
+
+
+def test_ctf_event():
+    ctf = CTF(energy=80e3)
+    ctf.semiangle_cutoff = 1
+    assert ctf.changed.notify_count == 2
```

### Comparing `abtem-1.0.0b8/test/test_energy.py` & `abtem-1.0.0b9/test/test_energy.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,50 +1,50 @@
-import numpy as np
-import pytest
-
-from abtem.base_classes import Accelerator
-from abtem.utils import energy2mass, energy2wavelength, energy2sigma
-
-
-def test_energy2mass():
-    assert np.isclose(energy2mass(300e3), 1.445736928082275e-30)
-
-
-def test_energy2wavelength():
-    assert np.isclose(energy2wavelength(300e3), 0.01968748889772767)
-
-
-def test_energy2sigma():
-    assert np.isclose(energy2sigma(300e3), 0.0006526161464700888)
-
-
-def test_energy():
-    energy = Accelerator(energy=300e3)
-
-    assert energy.energy == 300e3
-    assert np.isclose(energy.wavelength, energy2wavelength(300e3))
-
-    energy.energy = 200e3
-
-    assert np.isclose(energy.wavelength, energy2wavelength(200e3))
-
-
-def test_energy_raises():
-    accelerator1 = Accelerator(300e3)
-    accelerator2 = Accelerator()
-
-    with pytest.raises(RuntimeError):
-        accelerator2.check_is_defined()
-
-    accelerator2.energy = 200e3
-    with pytest.raises(RuntimeError):
-        accelerator1.check_match(accelerator2)
-
-    accelerator2.energy = accelerator1.energy
-    accelerator1.check_match(accelerator2)
-
-
-def test_accelerator_event():
-    accelerator = Accelerator(300e3)
-
-    accelerator.energy = 200e3
-    assert accelerator.changed._notify_count == 1
+import numpy as np
+import pytest
+
+from abtem.base_classes import Accelerator
+from abtem.utils import energy2mass, energy2wavelength, energy2sigma
+
+
+def test_energy2mass():
+    assert np.isclose(energy2mass(300e3), 1.445736928082275e-30)
+
+
+def test_energy2wavelength():
+    assert np.isclose(energy2wavelength(300e3), 0.01968748889772767)
+
+
+def test_energy2sigma():
+    assert np.isclose(energy2sigma(300e3), 0.0006526161464700888)
+
+
+def test_energy():
+    energy = Accelerator(energy=300e3)
+
+    assert energy.energy == 300e3
+    assert np.isclose(energy.wavelength, energy2wavelength(300e3))
+
+    energy.energy = 200e3
+
+    assert np.isclose(energy.wavelength, energy2wavelength(200e3))
+
+
+def test_energy_raises():
+    accelerator1 = Accelerator(300e3)
+    accelerator2 = Accelerator()
+
+    with pytest.raises(RuntimeError):
+        accelerator2.check_is_defined()
+
+    accelerator2.energy = 200e3
+    with pytest.raises(RuntimeError):
+        accelerator1.check_match(accelerator2)
+
+    accelerator2.energy = accelerator1.energy
+    accelerator1.check_match(accelerator2)
+
+
+def test_accelerator_event():
+    accelerator = Accelerator(300e3)
+
+    accelerator.energy = 200e3
+    assert accelerator.changed._notify_count == 1
```

### Comparing `abtem-1.0.0b8/test/test_export.py` & `abtem-1.0.0b9/test/test_export.py`

 * *Ordering differences only*

 * *Files 26% similar despite different names*

```diff
@@ -1,115 +1,115 @@
-import os
-
-import numpy as np
-from ase.io import read
-
-from abtem.detect import PixelatedDetector
-from abtem.measure import Measurement, calibrations_from_grid
-from abtem.potentials import Potential, PotentialArray
-from abtem.scan import LineScan, GridScan
-from abtem.waves import Probe, Waves
-
-_ROOT = os.path.abspath(os.path.dirname(__file__))
-
-
-def _set_path(path):
-    """Internal function to set the parametrization data directory."""
-    return os.path.join(_ROOT, 'data', path)
-
-
-def test_export_import_potential(tmp_path):
-    atoms = read(_set_path('orthogonal_graphene.cif'))
-
-    d = tmp_path / 'sub'
-    d.mkdir()
-    path = d / 'potential.hdf5'
-
-    potential = Potential(atoms, sampling=.05)
-    precalculated_potential = potential.build(pbar=False)
-    precalculated_potential.write(path)
-    imported_potential = PotentialArray.read(path)
-    assert np.allclose(imported_potential.array, precalculated_potential.array)
-    assert np.allclose(imported_potential.extent, precalculated_potential.extent)
-    assert np.allclose(imported_potential._slice_thicknesses, precalculated_potential._slice_thicknesses)
-
-
-def test_export_import_waves(tmp_path):
-    d = tmp_path / 'sub'
-    d.mkdir()
-    path = d / 'waves.hdf5'
-
-    waves = Probe(semiangle_cutoff=30, sampling=.05, extent=10, energy=80e3).build()
-    waves.write(path)
-    imported_waves = Waves.read(path)
-    assert np.allclose(waves.array, imported_waves.array)
-    assert np.allclose(waves.extent, imported_waves.extent)
-    assert np.allclose(waves.energy, imported_waves.energy)
-
-
-def test_export_import_measurement(tmp_path):
-    d = tmp_path / 'sub'
-    d.mkdir()
-    path = d / 'measurement.hdf5'
-
-    calibrations = calibrations_from_grid((512, 256), (.1, .3), ['x', 'y'], 'Å')
-
-    measurement = Measurement(np.random.rand(512, 256), calibrations)
-    measurement.write(path)
-    imported_measurement = Measurement.read(path)
-    assert np.allclose(measurement.array, imported_measurement.array)
-    assert measurement.calibrations[0] == imported_measurement.calibrations[0]
-    assert measurement.calibrations[1] == imported_measurement.calibrations[1]
-
-
-def test_linescan_to_file(tmp_path):
-    d = tmp_path / 'sub'
-    d.mkdir()
-    path = d / 'measurement2.hdf5'
-
-    atoms = read(_set_path('orthogonal_graphene.cif'))
-    potential = Potential(atoms=atoms, sampling=.05)
-
-    probe = Probe(energy=200e3, semiangle_cutoff=30)
-
-    probe.grid.match(potential)
-
-    scan = LineScan(start=[0, 0], end=[0, potential.extent[1]], gpts=20)
-
-    detector = PixelatedDetector()
-    export_detector = PixelatedDetector(save_file=path)
-
-    measurements = probe.scan(scan, [detector, export_detector], potential, pbar=False)
-
-    measurement = measurements[detector]
-    imported_measurement = Measurement.read(measurements[export_detector])
-
-    assert np.allclose(measurement.array, imported_measurement.array)
-    assert measurement.calibrations[0] == imported_measurement.calibrations[0]
-    assert measurement.calibrations[1] == imported_measurement.calibrations[1]
-
-
-def test_gridscan_to_file(tmp_path):
-    d = tmp_path / 'sub'
-    d.mkdir()
-    path = d / 'measurement2.hdf5'
-
-    atoms = read(_set_path('orthogonal_graphene.cif'))
-    potential = Potential(atoms=atoms, sampling=.05)
-
-    probe = Probe(energy=200e3, semiangle_cutoff=30)
-
-    probe.grid.match(potential)
-
-    scan = GridScan(start=[0, 0], end=[0, potential.extent[1]], gpts=(10,9))
-
-    detector = PixelatedDetector()
-    export_detector = PixelatedDetector(save_file=path)
-
-    measurements = probe.scan(scan, [detector, export_detector], potential, pbar=False)
-
-    measurement = measurements[detector]
-    imported_measurement = Measurement.read(measurements[export_detector])
-
-    assert np.allclose(measurement.array, imported_measurement.array)
-    assert measurement.calibrations[0] == imported_measurement.calibrations[0]
+import os
+
+import numpy as np
+from ase.io import read
+
+from abtem.detect import PixelatedDetector
+from abtem.measure import Measurement, calibrations_from_grid
+from abtem.potentials import Potential, PotentialArray
+from abtem.scan import LineScan, GridScan
+from abtem.waves import Probe, Waves
+
+_ROOT = os.path.abspath(os.path.dirname(__file__))
+
+
+def _set_path(path):
+    """Internal function to set the parametrization data directory."""
+    return os.path.join(_ROOT, 'data', path)
+
+
+def test_export_import_potential(tmp_path):
+    atoms = read(_set_path('orthogonal_graphene.cif'))
+
+    d = tmp_path / 'sub'
+    d.mkdir()
+    path = d / 'potential.hdf5'
+
+    potential = Potential(atoms, sampling=.05)
+    precalculated_potential = potential.build(pbar=False)
+    precalculated_potential.write(path)
+    imported_potential = PotentialArray.read(path)
+    assert np.allclose(imported_potential.array, precalculated_potential.array)
+    assert np.allclose(imported_potential.extent, precalculated_potential.extent)
+    assert np.allclose(imported_potential._slice_thicknesses, precalculated_potential._slice_thicknesses)
+
+
+def test_export_import_waves(tmp_path):
+    d = tmp_path / 'sub'
+    d.mkdir()
+    path = d / 'waves.hdf5'
+
+    waves = Probe(semiangle_cutoff=30, sampling=.05, extent=10, energy=80e3).build()
+    waves.write(path)
+    imported_waves = Waves.read(path)
+    assert np.allclose(waves.array, imported_waves.array)
+    assert np.allclose(waves.extent, imported_waves.extent)
+    assert np.allclose(waves.energy, imported_waves.energy)
+
+
+def test_export_import_measurement(tmp_path):
+    d = tmp_path / 'sub'
+    d.mkdir()
+    path = d / 'measurement.hdf5'
+
+    calibrations = calibrations_from_grid((512, 256), (.1, .3), ['x', 'y'], 'Å')
+
+    measurement = Measurement(np.random.rand(512, 256), calibrations)
+    measurement.write(path)
+    imported_measurement = Measurement.read(path)
+    assert np.allclose(measurement.array, imported_measurement.array)
+    assert measurement.calibrations[0] == imported_measurement.calibrations[0]
+    assert measurement.calibrations[1] == imported_measurement.calibrations[1]
+
+
+def test_linescan_to_file(tmp_path):
+    d = tmp_path / 'sub'
+    d.mkdir()
+    path = d / 'measurement2.hdf5'
+
+    atoms = read(_set_path('orthogonal_graphene.cif'))
+    potential = Potential(atoms=atoms, sampling=.05)
+
+    probe = Probe(energy=200e3, semiangle_cutoff=30)
+
+    probe.grid.match(potential)
+
+    scan = LineScan(start=[0, 0], end=[0, potential.extent[1]], gpts=20)
+
+    detector = PixelatedDetector()
+    export_detector = PixelatedDetector(save_file=path)
+
+    measurements = probe.scan(scan, [detector, export_detector], potential, pbar=False)
+
+    measurement = measurements[detector]
+    imported_measurement = Measurement.read(measurements[export_detector])
+
+    assert np.allclose(measurement.array, imported_measurement.array)
+    assert measurement.calibrations[0] == imported_measurement.calibrations[0]
+    assert measurement.calibrations[1] == imported_measurement.calibrations[1]
+
+
+def test_gridscan_to_file(tmp_path):
+    d = tmp_path / 'sub'
+    d.mkdir()
+    path = d / 'measurement2.hdf5'
+
+    atoms = read(_set_path('orthogonal_graphene.cif'))
+    potential = Potential(atoms=atoms, sampling=.05)
+
+    probe = Probe(energy=200e3, semiangle_cutoff=30)
+
+    probe.grid.match(potential)
+
+    scan = GridScan(start=[0, 0], end=[0, potential.extent[1]], gpts=(10,9))
+
+    detector = PixelatedDetector()
+    export_detector = PixelatedDetector(save_file=path)
+
+    measurements = probe.scan(scan, [detector, export_detector], potential, pbar=False)
+
+    measurement = measurements[detector]
+    imported_measurement = Measurement.read(measurements[export_detector])
+
+    assert np.allclose(measurement.array, imported_measurement.array)
+    assert measurement.calibrations[0] == imported_measurement.calibrations[0]
     assert measurement.calibrations[1] == imported_measurement.calibrations[1]
```

### Comparing `abtem-1.0.0b8/test/test_grid.py` & `abtem-1.0.0b9/test/test_grid.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,111 +1,111 @@
-import numpy as np
-import pytest
-
-from abtem.base_classes import Grid
-from abtem.waves import Probe
-
-def test_create_grid():
-    grid = Grid(extent=5, sampling=.2)
-
-    assert (grid.extent[0] == 5.) & (grid.extent[1] == 5.)
-    assert (grid.gpts[0] == 25) & (grid.gpts[1] == 25)
-    assert (grid.sampling[0] == .2) & (grid.sampling[1] == .2)
-
-    grid = Grid(sampling=.2, gpts=10)
-    assert (grid.extent[0] == 2.) & (grid.extent[1] == 2.)
-
-    grid = Grid(extent=(8, 6), gpts=10)
-    assert (grid.sampling[0] == .8) & (grid.sampling[1] == .6)
-
-    grid = Grid()
-    with pytest.raises(RuntimeError):
-        grid.check_is_defined()
-
-
-def test_change_grid():
-    grid = Grid(extent=(8, 6), gpts=10)
-
-    grid.sampling = .2
-    assert (grid.extent[0] == 8.) & (grid.extent[1] == 6.)
-    assert (grid.gpts[0] == 40) & (grid.gpts[1] == 30)
-
-    grid.gpts = 100
-    assert (grid.extent[0] == 8.) & (grid.extent[1] == 6.)
-    assert (grid.sampling[0] == .08) & (grid.sampling[1] == .06)
-
-    grid.extent = (16, 12)
-    assert (grid.gpts[0] == 100) & (grid.gpts[1] == 100)
-    assert (grid.extent[0] == 16.) & (grid.extent[1] == 12.)
-    assert (grid.sampling[0] == .16) & (grid.sampling[1] == .12)
-
-    grid.extent = (10, 10)
-    assert (grid.sampling[0] == grid.extent[0] / grid.gpts[0]) & (grid.sampling[1] == grid.extent[1] / grid.gpts[1])
-
-    grid.sampling = .3
-    assert (grid.extent[0] == grid.sampling[0] * grid.gpts[0]) & (grid.extent[1] == grid.sampling[1] * grid.gpts[1])
-
-    grid.gpts = 30
-    assert (grid.sampling[0] == grid.extent[0] / grid.gpts[0]) & (grid.sampling[1] == grid.extent[1] / grid.gpts[1])
-
-
-def test_grid_raises():
-    with pytest.raises(RuntimeError) as e:
-        Grid(extent=[5, 5, 5])
-
-    assert str(e.value) == 'Grid value length of 3 != 2'
-
-
-def test_grid_event():
-    grid = Grid()
-
-    grid.extent = 5
-    assert grid.changed._notify_count == 1
-
-    grid.gpts = 100
-    assert grid.changed._notify_count == 2
-
-    grid.sampling = .1
-    assert grid.changed._notify_count == 3
-
-
-def test_locked_grid():
-    grid = Grid(gpts=200, lock_gpts=True)
-
-    grid.extent = 10
-    assert (grid.sampling[0] == .05) & (grid.sampling[1] == .05)
-    grid.extent = 20
-    assert (grid.sampling[0] == .1) & (grid.sampling[1] == .1)
-
-    with pytest.raises(RuntimeError) as e:
-        grid.gpts = 100
-
-    assert str(e.value) == 'Grid gpts cannot be modified'
-
-
-def test_grid_match():
-    grid1 = Grid(extent=10, gpts=10)
-    grid2 = Grid()
-    grid1.match(grid2)
-
-    grid1.check_match(grid2)
-    grid2.sampling = .2
-
-    with pytest.raises(RuntimeError) as e:
-        grid1.check_match(grid2)
-
-    assert str(e.value) == 'Inconsistent grid gpts ((10, 10) != (50, 50))'
-
-
-# def test_scattering_angle():
-#     probe = Probe(extent=18, gpts=(250, 251), energy=80e3)
-#     probe = probe.build()
-#
-#     alpha_x = np.fft.fftfreq(probe.gpts[0], probe.sampling[0]) * probe.wavelength * 1000
-#     alpha_y = np.fft.fftfreq(probe.gpts[1], probe.sampling[1]) * probe.wavelength * 1000
-#
-#     assert np.isclose(alpha_x.min(), probe.max_scattering_angles[0][0])
-#     assert np.isclose(alpha_x.max(), probe.max_scattering_angles[0][1])
-#     assert np.isclose(alpha_y.min(), probe.max_scattering_angles[1][0])
-#     assert np.isclose(alpha_y.max(), probe.max_scattering_angles[1][1])
-    #assert np.sum(np.abs(alpha_x) < 65) == probe._resampled_gpts(65)[0]
-    #assert np.sum(np.abs(alpha_y) < 65) == probe._resampled_gpts(65)[1]
+import numpy as np
+import pytest
+
+from abtem.base_classes import Grid
+from abtem.waves import Probe
+
+def test_create_grid():
+    grid = Grid(extent=5, sampling=.2)
+
+    assert (grid.extent[0] == 5.) & (grid.extent[1] == 5.)
+    assert (grid.gpts[0] == 25) & (grid.gpts[1] == 25)
+    assert (grid.sampling[0] == .2) & (grid.sampling[1] == .2)
+
+    grid = Grid(sampling=.2, gpts=10)
+    assert (grid.extent[0] == 2.) & (grid.extent[1] == 2.)
+
+    grid = Grid(extent=(8, 6), gpts=10)
+    assert (grid.sampling[0] == .8) & (grid.sampling[1] == .6)
+
+    grid = Grid()
+    with pytest.raises(RuntimeError):
+        grid.check_is_defined()
+
+
+def test_change_grid():
+    grid = Grid(extent=(8, 6), gpts=10)
+
+    grid.sampling = .2
+    assert (grid.extent[0] == 8.) & (grid.extent[1] == 6.)
+    assert (grid.gpts[0] == 40) & (grid.gpts[1] == 30)
+
+    grid.gpts = 100
+    assert (grid.extent[0] == 8.) & (grid.extent[1] == 6.)
+    assert (grid.sampling[0] == .08) & (grid.sampling[1] == .06)
+
+    grid.extent = (16, 12)
+    assert (grid.gpts[0] == 100) & (grid.gpts[1] == 100)
+    assert (grid.extent[0] == 16.) & (grid.extent[1] == 12.)
+    assert (grid.sampling[0] == .16) & (grid.sampling[1] == .12)
+
+    grid.extent = (10, 10)
+    assert (grid.sampling[0] == grid.extent[0] / grid.gpts[0]) & (grid.sampling[1] == grid.extent[1] / grid.gpts[1])
+
+    grid.sampling = .3
+    assert (grid.extent[0] == grid.sampling[0] * grid.gpts[0]) & (grid.extent[1] == grid.sampling[1] * grid.gpts[1])
+
+    grid.gpts = 30
+    assert (grid.sampling[0] == grid.extent[0] / grid.gpts[0]) & (grid.sampling[1] == grid.extent[1] / grid.gpts[1])
+
+
+def test_grid_raises():
+    with pytest.raises(RuntimeError) as e:
+        Grid(extent=[5, 5, 5])
+
+    assert str(e.value) == 'Grid value length of 3 != 2'
+
+
+def test_grid_event():
+    grid = Grid()
+
+    grid.extent = 5
+    assert grid.changed._notify_count == 1
+
+    grid.gpts = 100
+    assert grid.changed._notify_count == 2
+
+    grid.sampling = .1
+    assert grid.changed._notify_count == 3
+
+
+def test_locked_grid():
+    grid = Grid(gpts=200, lock_gpts=True)
+
+    grid.extent = 10
+    assert (grid.sampling[0] == .05) & (grid.sampling[1] == .05)
+    grid.extent = 20
+    assert (grid.sampling[0] == .1) & (grid.sampling[1] == .1)
+
+    with pytest.raises(RuntimeError) as e:
+        grid.gpts = 100
+
+    assert str(e.value) == 'Grid gpts cannot be modified'
+
+
+def test_grid_match():
+    grid1 = Grid(extent=10, gpts=10)
+    grid2 = Grid()
+    grid1.match(grid2)
+
+    grid1.check_match(grid2)
+    grid2.sampling = .2
+
+    with pytest.raises(RuntimeError) as e:
+        grid1.check_match(grid2)
+
+    assert str(e.value) == 'Inconsistent grid gpts ((10, 10) != (50, 50))'
+
+
+# def test_scattering_angle():
+#     probe = Probe(extent=18, gpts=(250, 251), energy=80e3)
+#     probe = probe.build()
+#
+#     alpha_x = np.fft.fftfreq(probe.gpts[0], probe.sampling[0]) * probe.wavelength * 1000
+#     alpha_y = np.fft.fftfreq(probe.gpts[1], probe.sampling[1]) * probe.wavelength * 1000
+#
+#     assert np.isclose(alpha_x.min(), probe.max_scattering_angles[0][0])
+#     assert np.isclose(alpha_x.max(), probe.max_scattering_angles[0][1])
+#     assert np.isclose(alpha_y.min(), probe.max_scattering_angles[1][0])
+#     assert np.isclose(alpha_y.max(), probe.max_scattering_angles[1][1])
+    #assert np.sum(np.abs(alpha_x) < 65) == probe._resampled_gpts(65)[0]
+    #assert np.sum(np.abs(alpha_y) < 65) == probe._resampled_gpts(65)[1]
```

### Comparing `abtem-1.0.0b8/test/test_kirkland.py` & `abtem-1.0.0b9/test/test_kirkland.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,49 @@
-import numpy as np
-from ase import Atoms
-
-from abtem.detect import AnnularDetector
-from abtem.potentials import Potential
-from abtem.scan import LineScan
-from abtem.waves import PlaneWave, Probe
-
-
-def test_fig_5_12():
-    atoms = Atoms('CSiCuAuU', positions=[(x, 25, 4) for x in np.linspace(5, 45, 5)], cell=(50, 50, 8))
-
-    potential = Potential(atoms=atoms, gpts=512, parametrization='kirkland', cutoff_tolerance=1e-4)
-
-    waves = PlaneWave(energy=200e3)
-
-    waves = waves.multislice(potential, pbar=False)
-    waves = waves.apply_ctf(defocus=700, Cs=1.3e7, semiangle_cutoff=10.37, rolloff=0.)
-
-    intensity = np.abs(waves.array) ** 2
-
-    assert np.round(intensity.min(), 2) == np.float32(.72)
-    assert np.round(intensity.max(), 2) == np.float32(1.03)
-
-
-def test_fig():
-    atoms = Atoms('CSiCuAuU', positions=[(x, 25, 4) for x in np.linspace(5, 45, 5)], cell=(50, 50, 8))
-
-    gpts = 2048
-
-    potential = Potential(atoms=atoms, gpts=gpts, parametrization='kirkland', slice_thickness=8)
-
-    probe = Probe(energy=200e3, defocus=700, Cs=1.3e7, semiangle_cutoff=10.37)
-
-    probe.grid.match(potential)
-
-    scan = LineScan(start=[5, 25], end=[45, 25], gpts=5)
-
-    detector = AnnularDetector(inner=40, outer=200)
-
-    measurements = probe.scan(scan, [detector], potential, pbar=False)
-
-    #assert np.allclose(measurements[detector].array, [0.00010976, 0.00054356, 0.00198158, 0.00997221, 0.01098883])
-    assert np.allclose(measurements[detector].array, [0.00010933, 0.00054426, 0.00205304, 0.00986171, 0.01197426],
-                      atol=1e-5)
-    # assert np.allclose(measurements[detector].array, [0.00012474, 0.00060268, 0.0022271 , 0.00963283, 0.01076559],
+import numpy as np
+from ase import Atoms
+
+from abtem.detect import AnnularDetector
+from abtem.potentials import Potential
+from abtem.scan import LineScan
+from abtem.waves import PlaneWave, Probe
+
+
+def test_fig_5_12():
+    atoms = Atoms('CSiCuAuU', positions=[(x, 25, 4) for x in np.linspace(5, 45, 5)], cell=(50, 50, 8))
+
+    potential = Potential(atoms=atoms, gpts=512, parametrization='kirkland', cutoff_tolerance=1e-4)
+
+    waves = PlaneWave(energy=200e3)
+
+    waves = waves.multislice(potential, pbar=False)
+    waves = waves.apply_ctf(defocus=700, Cs=1.3e7, semiangle_cutoff=10.37, rolloff=0.)
+
+    intensity = np.abs(waves.array) ** 2
+
+    assert np.round(intensity.min(), 2) == np.float32(.72)
+    assert np.round(intensity.max(), 2) == np.float32(1.03)
+
+
+def test_fig():
+    atoms = Atoms('CSiCuAuU', positions=[(x, 25, 4) for x in np.linspace(5, 45, 5)], cell=(50, 50, 8))
+
+    gpts = 2048
+
+    potential = Potential(atoms=atoms, gpts=gpts, parametrization='kirkland', slice_thickness=8)
+
+    probe = Probe(energy=200e3, defocus=700, Cs=1.3e7, semiangle_cutoff=10.37)
+
+    probe.grid.match(potential)
+
+    scan = LineScan(start=[5, 25], end=[45, 25], gpts=5)
+
+    detector = AnnularDetector(inner=40, outer=200)
+
+    measurements = probe.scan(scan, [detector], potential, pbar=False)
+
+    #assert np.allclose(measurements[detector].array, [0.00010976, 0.00054356, 0.00198158, 0.00997221, 0.01098883])
+    assert np.allclose(measurements[detector].array, [0.0001168, 0.00059303, 0.00214667, 0.00977803, 0.01167613],
+                       atol=1e-5)
+    #assert np.allclose(measurements[detector].array, [0.00010933, 0.00054426, 0.00205304, 0.00986171, 0.01197426],
+                      #atol=1e-5)
+    # assert np.allclose(measurements[detector].array, [0.00012474, 0.00060268, 0.0022271 , 0.00963283, 0.01076559],
     #                    atol=1e-5)
```

### Comparing `abtem-1.0.0b8/test/test_potential_integration.py` & `abtem-1.0.0b9/test/test_potential_integration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,109 +1,107 @@
-import numpy as np
-from ase import Atoms
-
-from abtem.cpu_kernels import interpolate_radial_functions
-from abtem.parametrizations import kirkland_projected, kirkland, load_kirkland_parameters
-from abtem.potentials import PotentialIntegrator, Potential, kappa, _disc_meshgrid
-
-
-def test_gaussian_integral():
-    sigma = 3
-    f = lambda r: np.exp(-r ** 2 / (2 * sigma ** 2))
-    r = np.array([0, 30])
-    integrator = PotentialIntegrator(f, r)
-    value = integrator.integrate(-50, 50)
-    assert np.isclose(value[0][0], sigma * np.sqrt(2 * np.pi))
-
-
-def test_projected_kirkland():
-    f = lambda r: kirkland(r, parameters[6])
-    parameters = load_kirkland_parameters()
-    r = np.geomspace(.01, 10, 100)
-    integrator = PotentialIntegrator(f, r)
-    print(integrator.integrate(-10, 10), kirkland_projected(r, parameters[6]))
-    assert np.allclose(integrator.integrate(-10, 10)[0], kirkland_projected(r, parameters[6]))
-
-
-def test_cutoff():
-    tolerance = 1e-5
-    atoms = Atoms([6], [(0, 0, 0)], cell=(1, 1, 1))
-    potential = Potential(atoms, cutoff_tolerance=tolerance)
-    assert np.isclose(potential.function(potential.get_cutoff(6), potential.parameters[6]), tolerance)
-
-
-def test_interpolation():  # just a sanity check
-    from abtem.potentials import kappa
-
-    sampling = .005
-    L = 20
-    atoms = Atoms('C', positions=[(0, 0, 1.5)], cell=(L, L, 3))
-
-    potential = Potential(atoms, sampling=sampling, cutoff_tolerance=1e-3, slice_thickness=10)
-
-    interpolated = potential[0].array[0,0]
-    integrator = potential.get_integrator(6)
-
-    integrated = integrator.integrate(-1.5,1.5)[0]
-
-    r = np.linspace(0, L, len(interpolated), endpoint=False)
-
-    x = np.linspace(.005, 1.5, 10)
-    relative_errors = (np.interp(x, integrator.r, integrated) / kappa -
-                       np.interp(x, r, interpolated)) / np.interp(x, r, interpolated)
-
-    absolute_errors = (np.interp(x, integrator.r, integrated) / kappa - np.interp(x, r, interpolated))
-
-    assert np.all((np.abs(relative_errors) < 1e-4) + (np.abs(absolute_errors) < 1e-4))
-
-
-def test_geomspace():
-    sampling = .1
-    rc = 10
-    n = 100
-
-    for rf in np.linspace(.01, rc + 1, 1000):
-        r = np.geomspace(sampling, rc, n)
-        i = max(np.searchsorted(r, rf) - 1, 0)
-        dt = np.log(rc / sampling) / (n - 1)
-        j = min(max(np.floor(np.log(rf / sampling) / dt), 0), len(r) - 1)
-        assert i == j
-
-
-# def interpolate_radial_functions_launcher(func, positions, shape, cutoff, inner_cutoff):
-#     n = np.int(np.ceil(cutoff - inner_cutoff))
-#     r = np.geomspace(inner_cutoff, cutoff, 100 * n)[:-1]
-#
-#     v = func(r)
-#     v = np.tile(v.reshape(1, -1), (len(positions), 1))
-#     dvdr = np.zeros_like(v)
-#     dvdr[:, :-1] = np.diff(v) / np.diff(r)
-#
-#     # padded_shape = (shape[0] + 2 * margin, shape[1] + 2 * margin)
-#     array = np.zeros(shape, dtype=np.float32)
-#
-#     position_indices = np.rint(positions).astype(np.int)
-#
-#     rows, cols = disc_meshgrid(np.int(np.ceil(r[-1])))
-#     disc_indices = np.hstack((rows[:, None], cols[:, None]))
-#
-#     rows, cols = np.indices(shape)
-#     x = rows.astype(np.float32)
-#     y = cols.astype(np.float32)
-#
-#     interpolate_radial_functions(array, x, y, position_indices, disc_indices, positions, v, r, dvdr)
-#     return array
-#
-#
-# def test_interpolate():
-#     sigma = 128
-#     func = lambda x: np.exp(-x ** 2 / (2 * sigma ** 2))
-#
-#     shape = (2048, 2048)
-#     positions = np.array([[0, 0]])
-#     cutoff = 10 * sigma
-#     inner_cutoff = 0.001
-#
-#     array = interpolate_radial_functions_launcher(func, positions, shape, cutoff, inner_cutoff=inner_cutoff)
-#     r = np.linspace(inner_cutoff, shape[0], shape[0], endpoint=False)
-#
-#     assert np.allclose(func(r), array[0], atol=1e-6)
+import numpy as np
+from ase import Atoms
+
+from abtem.cpu_kernels import interpolate_radial_functions
+from abtem.parametrizations import kirkland_projected, kirkland, load_kirkland_parameters
+from abtem.potentials import PotentialIntegrator, Potential, kappa, _disc_meshgrid
+
+
+def test_gaussian_integral():
+    sigma = 3
+    f = lambda r: np.exp(-r ** 2 / (2 * sigma ** 2))
+    r = np.array([0, 30])
+    integrator = PotentialIntegrator(f, r, 30)
+    value = integrator.integrate(np.array([0.]), -50, 50, np)
+    assert np.isclose(value[0][0][0], sigma * np.sqrt(2 * np.pi))
+
+
+def test_projected_kirkland():
+    f = lambda r: kirkland(r, parameters[6])
+    parameters = load_kirkland_parameters()
+    r = np.geomspace(.01, 10, 100)
+    integrator = PotentialIntegrator(f, r, 20)
+    assert np.allclose(integrator.integrate(np.array([0.]), -10, 10, np)[0], kirkland_projected(r, parameters[6]))
+
+
+def test_cutoff():
+    tolerance = 1e-5
+    atoms = Atoms([6], [(0, 0, 0)], cell=(1, 1, 1))
+    potential = Potential(atoms, cutoff_tolerance=tolerance)
+    assert np.isclose(potential.function(potential.get_cutoff(6), potential.parameters[6]), tolerance)
+
+
+def test_interpolation():  # just a sanity check
+    from abtem.potentials import kappa
+
+    sampling = .005
+    L = 20
+    atoms = Atoms('C', positions=[(0, 0, 1.5)], cell=(L, L, 3))
+
+    potential = Potential(atoms, sampling=sampling, cutoff_tolerance=1e-3, slice_thickness=10)
+
+    interpolated = potential[0].array[0, 0]
+    integrator = potential.get_integrator(6)
+
+    integrated = integrator.integrate(np.array([0.]), -1.5, 1.5, np)[0][0]
+
+    r = np.linspace(0, L, len(interpolated), endpoint=False)
+
+    x = np.linspace(.005, 1.5, 10)
+    relative_errors = (np.interp(x, integrator.r, integrated) / kappa -
+                       np.interp(x, r, interpolated)) / np.interp(x, r, interpolated)
+
+    absolute_errors = (np.interp(x, integrator.r, integrated) / kappa - np.interp(x, r, interpolated))
+
+    assert np.all((np.abs(relative_errors) < 1e-4) + (np.abs(absolute_errors) < 1e-4))
+
+
+def test_geomspace():
+    sampling = .1
+    rc = 10
+    n = 100
+
+    for rf in np.linspace(.01, rc + 1, 1000):
+        r = np.geomspace(sampling, rc, n)
+        i = max(np.searchsorted(r, rf) - 1, 0)
+        dt = np.log(rc / sampling) / (n - 1)
+        j = min(max(np.floor(np.log(rf / sampling) / dt), 0), len(r) - 1)
+        assert i == j
+
+# def interpolate_radial_functions_launcher(func, positions, shape, cutoff, inner_cutoff):
+#     n = np.int(np.ceil(cutoff - inner_cutoff))
+#     r = np.geomspace(inner_cutoff, cutoff, 100 * n)[:-1]
+#
+#     v = func(r)
+#     v = np.tile(v.reshape(1, -1), (len(positions), 1))
+#     dvdr = np.zeros_like(v)
+#     dvdr[:, :-1] = np.diff(v) / np.diff(r)
+#
+#     # padded_shape = (shape[0] + 2 * margin, shape[1] + 2 * margin)
+#     array = np.zeros(shape, dtype=np.float32)
+#
+#     position_indices = np.rint(positions).astype(np.int)
+#
+#     rows, cols = disc_meshgrid(np.int(np.ceil(r[-1])))
+#     disc_indices = np.hstack((rows[:, None], cols[:, None]))
+#
+#     rows, cols = np.indices(shape)
+#     x = rows.astype(np.float32)
+#     y = cols.astype(np.float32)
+#
+#     interpolate_radial_functions(array, x, y, position_indices, disc_indices, positions, v, r, dvdr)
+#     return array
+#
+#
+# def test_interpolate():
+#     sigma = 128
+#     func = lambda x: np.exp(-x ** 2 / (2 * sigma ** 2))
+#
+#     shape = (2048, 2048)
+#     positions = np.array([[0, 0]])
+#     cutoff = 10 * sigma
+#     inner_cutoff = 0.001
+#
+#     array = interpolate_radial_functions_launcher(func, positions, shape, cutoff, inner_cutoff=inner_cutoff)
+#     r = np.linspace(inner_cutoff, shape[0], shape[0], endpoint=False)
+#
+#     assert np.allclose(func(r), array[0], atol=1e-6)
```

### Comparing `abtem-1.0.0b8/test/test_potential_parametrization.py` & `abtem-1.0.0b9/test/test_potential_parametrization.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-import numpy as np
-
-from abtem.parametrizations import lobato, kirkland, load_kirkland_parameters, load_lobato_parameters
-from abtem.potentials import kappa
-
-kirkland_parameters = load_kirkland_parameters()
-lobato_parameters = load_lobato_parameters()
-
-
-def test_similar():
-    r = np.linspace(.1, 2, 5)
-    assert np.allclose(lobato(r, lobato_parameters[47]), kirkland(r, kirkland_parameters[47]), rtol=.1)
-
-
-def test_values():
-    r = np.array([1., 1.316074, 1.7320508, 2.2795072, 3.])
-
-    assert np.allclose(lobato(r, lobato_parameters[47]) / kappa,
-                       [10.877785, 3.5969334, 1.1213292, 0.29497656, 0.05587856])
-
-    assert np.allclose(kirkland(r, kirkland_parameters[47]) / kappa,
-                       [10.966407, 3.7869546, 1.1616056, 0.2839873, 0.04958321])
+import numpy as np
+
+from abtem.parametrizations import lobato, kirkland, load_kirkland_parameters, load_lobato_parameters
+from abtem.potentials import kappa
+
+kirkland_parameters = load_kirkland_parameters()
+lobato_parameters = load_lobato_parameters()
+
+
+def test_similar():
+    r = np.linspace(.1, 2, 5)
+    assert np.allclose(lobato(r, lobato_parameters[47]), kirkland(r, kirkland_parameters[47]), rtol=.1)
+
+
+def test_values():
+    r = np.array([1., 1.316074, 1.7320508, 2.2795072, 3.])
+
+    assert np.allclose(lobato(r, lobato_parameters[47]) / kappa,
+                       [10.877785, 3.5969334, 1.1213292, 0.29497656, 0.05587856])
+
+    assert np.allclose(kirkland(r, kirkland_parameters[47]) / kappa,
+                       [10.966407, 3.7869546, 1.1616056, 0.2839873, 0.04958321])
```

### Comparing `abtem-1.0.0b8/test/test_potentials.py` & `abtem-1.0.0b9/test/test_potentials.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,71 +1,70 @@
-import numpy as np
-import pytest
-from ase import Atoms
-
-from abtem.potentials import Potential
-from abtem.device import asnumpy, cp
-
-
-def test_create_potential():
-    atoms = Atoms('C', positions=[(2, 3, 2)], cell=(4, 6, 4.3))
-
-    potential = Potential(atoms=atoms, sampling=.1)
-
-    assert (potential.extent[0] == 4) & (potential.extent[1] == 6)
-    assert potential.num_slices == 9
-    assert potential.get_slice_thickness(0) == 4.3 / 9
-
-
-def test_potential_raises():
-    with pytest.raises(RuntimeError) as e:
-        Potential(Atoms('C', positions=[(2, 2, 2)], cell=(4, 4, 0)))
-
-    assert str(e.value) == 'Atoms cell has no thickness'
-
-
-def test_potential_centered():
-    Lx = 5
-    Ly = 5
-    gpts_x = 40
-    gpts_y = 60
-
-    atoms1 = Atoms('C', positions=[(0, Ly / 2, 2)], cell=[Lx, Ly, 4])
-    atoms2 = Atoms('C', positions=[(Lx / 2, Ly / 2, 2)], cell=[Lx, Ly, 4])
-    potential1 = Potential(atoms1, gpts=(gpts_x, gpts_y), slice_thickness=4, cutoff_tolerance=1e-2)
-    potential2 = Potential(atoms2, gpts=(gpts_x, gpts_y), slice_thickness=4, cutoff_tolerance=1e-2)
-
-    assert np.allclose(potential1[0].array[0, :, gpts_y // 2],
-                       np.roll(potential2[0].array[0, :, gpts_y // 2], gpts_x // 2))
-    assert np.allclose(potential2[0].array[0, :, gpts_y // 2][1:], (potential2[0].array[0, :, gpts_y // 2])[::-1][:-1])
-    assert np.allclose(potential2[0].array[0, gpts_x // 2][1:], potential2[0].array[0, gpts_x // 2][::-1][:-1])
-
-
-def test_potential_build():
-    atoms = Atoms('CO', positions=[(2, 3, 1), (3, 2, 3)], cell=(4, 6, 4.3))
-    potential = Potential(atoms=atoms, sampling=.1)
-    array_potential = potential.build()
-    assert np.all(array_potential[2].array == potential[2].array)
-
-
-@pytest.mark.gpu
-def test_potential_build_gpu():
-    atoms = Atoms('CO', positions=[(2, 3, 1), (3, 2, 3)], cell=(4, 6, 4.3))
-    potential = Potential(atoms=atoms, sampling=.1, device='gpu')
-
-    array_potential = potential.build()
-    assert np.all(asnumpy(array_potential[2].array == potential[2].array))
-
-    potential = Potential(atoms=atoms, sampling=.1, device='cpu')
-    assert np.allclose(asnumpy(array_potential[2].array), potential[2].array)
-
-
-@pytest.mark.gpu
-def test_potential_storage():
-    atoms = Atoms('CO', positions=[(2, 3, 1), (3, 2, 3)], cell=(4, 6, 4.3))
-
-    potential = Potential(atoms=atoms, sampling=.1, device='gpu')
-    assert type(potential.build().array) is cp.ndarray
-
-    potential = Potential(atoms=atoms, sampling=.1, device='gpu', storage='cpu')
-
-    assert type(potential.build().array) is np.ndarray
+import numpy as np
+import pytest
+from ase import Atoms
+
+from abtem.potentials import Potential
+from abtem.device import asnumpy, cp
+
+
+def test_create_potential():
+    atoms = Atoms('C', positions=[(2, 3, 2)], cell=(4, 6, 4.3))
+
+    potential = Potential(atoms=atoms, sampling=.1)
+
+    assert (potential.extent[0] == 4) & (potential.extent[1] == 6)
+    assert potential.num_slices == 9
+    assert potential.get_slice_thickness(0) == 4.3 / 9
+
+
+def test_potential_raises():
+    with pytest.raises(RuntimeError) as e:
+        Potential(Atoms('C', positions=[(2, 2, 2)], cell=(4, 4, 0)))
+
+    assert str(e.value) == 'Atoms cell has no thickness'
+
+
+def test_potential_centered():
+    Lx = 5
+    Ly = 5
+    gpts_x = 40
+    gpts_y = 60
+
+    atoms1 = Atoms('C', positions=[(0, Ly / 2, 2)], cell=[Lx, Ly, 4])
+    atoms2 = Atoms('C', positions=[(Lx / 2, Ly / 2, 2)], cell=[Lx, Ly, 4])
+    potential1 = Potential(atoms1, gpts=(gpts_x, gpts_y), slice_thickness=4, cutoff_tolerance=1e-2)
+    potential2 = Potential(atoms2, gpts=(gpts_x, gpts_y), slice_thickness=4, cutoff_tolerance=1e-2)
+
+    assert np.allclose(potential1[0].array[0, :, gpts_y // 2],
+                       np.roll(potential2[0].array[0, :, gpts_y // 2], gpts_x // 2))
+    assert np.allclose(potential2[0].array[0, :, gpts_y // 2][1:], (potential2[0].array[0, :, gpts_y // 2])[::-1][:-1])
+    assert np.allclose(potential2[0].array[0, gpts_x // 2][1:], potential2[0].array[0, gpts_x // 2][::-1][:-1])
+
+
+def test_potential_build():
+    atoms = Atoms('CO', positions=[(2, 3, 1), (3, 2, 3)], cell=(4, 6, 4.3))
+    potential = Potential(atoms=atoms, sampling=.1)
+    array_potential = potential.build()
+    assert np.all(array_potential[2].array == potential[2].array)
+
+
+@pytest.mark.gpu
+def test_potential_build_gpu():
+    atoms = Atoms('CO', positions=[(2, 3, 1), (3, 2, 3)], cell=(4, 6, 4.3))
+    potential = Potential(atoms=atoms, sampling=.1, device='gpu')
+
+    array_potential = potential.build()
+    assert np.all(asnumpy(array_potential[2].array == potential[2].array))
+
+    potential = Potential(atoms=atoms, sampling=.1, device='cpu')
+    assert np.allclose(asnumpy(array_potential[2].array), potential[2].array)
+
+
+@pytest.mark.gpu
+def test_potential_storage():
+    atoms = Atoms('CO', positions=[(2, 3, 1), (3, 2, 3)], cell=(4, 6, 4.3))
+
+    potential = Potential(atoms=atoms, sampling=.1, device='gpu')
+    assert type(potential.build().array) is cp.ndarray
+
+    potential = Potential(atoms=atoms, sampling=.1, device='gpu', storage='cpu')
+    assert type(potential.build().array) is np.ndarray
```

### Comparing `abtem-1.0.0b8/test/test_prism.py` & `abtem-1.0.0b9/test/test_prism.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,205 +1,205 @@
-import os
-
-import numpy as np
-import pytest
-from abtem.detect import AnnularDetector, FlexibleAnnularDetector
-from abtem.device import asnumpy, cp
-from abtem.potentials import Potential
-from abtem.scan import LineScan, GridScan
-from abtem.waves import Probe, SMatrix
-from ase import Atoms
-from ase.io import read
-
-
-def test_prism_raises():
-    with pytest.raises(ValueError) as e:
-        SMatrix(.01, 80e3, .5)
-
-    assert str(e.value) == 'Interpolation factor must be int'
-
-    with pytest.raises(RuntimeError) as e:
-        prism = SMatrix(10, 80e3, 1)
-        prism.build()
-
-    assert str(e.value) == 'Grid extent is not defined'
-
-
-def test_prism_match_probe():
-    S_builder = SMatrix(30., 60e3, 1, extent=5, gpts=50)
-    probe = Probe(extent=5, gpts=50, energy=60e3, semiangle_cutoff=30., rolloff=0.)
-    assert np.allclose(probe.build([(0., 0.)]).array, S_builder.build().collapse([(0., 0.)]).array, atol=2e-5)
-
-
-def test_prism_translate():
-    S_builder = SMatrix(30, 60e3, 1, extent=5, gpts=50)
-    probe = Probe(extent=5, gpts=50, energy=60e3, semiangle_cutoff=30, rolloff=0)
-    assert np.allclose(probe.build(np.array([(2.5, 2.5)])).array,
-                       S_builder.build().collapse([(2.5, 2.5)]).array, atol=1e-5)
-
-
-def test_prism_interpolation():
-    S_builder = SMatrix(30, 60e3, 2, extent=10, gpts=100)
-    probe = Probe(extent=5, gpts=50, energy=60e3, semiangle_cutoff=30, rolloff=0)
-    assert np.allclose(probe.build(np.array([(2.5, 2.5)])).array,
-                       S_builder.build().collapse([(2.5, 2.5)]).array, atol=1e-5)
-
-
-def test_prism_multislice():
-    potential = Potential(Atoms('C', positions=[(0, 0, 2)], cell=(5, 5, 4)))
-    S = SMatrix(30, 60e3, 1, extent=5, gpts=500)
-    probe = Probe(extent=5, gpts=500, energy=60e3, semiangle_cutoff=30, rolloff=0.)
-    assert np.allclose(probe.build(np.array([[2.5, 2.5]])).multislice(potential, pbar=False).array,
-                       S.multislice(potential, pbar=False).collapse([(2.5, 2.5)]).array, atol=2e-5)
-
-
-def test_probe_waves_line_scan():
-    potential = Potential(Atoms('C', positions=[(2.5, 2.5, 2)], cell=(5, 5, 4)))
-    linescan = LineScan(start=[0, 0], end=[2.5, 2.5], gpts=10)
-    detector = AnnularDetector(inner=80, outer=200)
-
-    S_builder = SMatrix(30, 80e3, 1, gpts=500)
-    S = S_builder.multislice(potential, pbar=False)
-    probe = Probe(semiangle_cutoff=30, energy=80e3, gpts=500)
-
-    prism_measurements = S.scan(linescan, [detector], max_batch_probes=10, pbar=False)
-    measurements = probe.scan(linescan, [detector], potential, max_batch=50, pbar=False)
-
-    assert np.allclose(measurements[detector].array, prism_measurements[detector].array, atol=1e-6)
-
-
-def test_interpolation_scan():
-    atoms = Atoms('C', positions=[(2.5, 2.5, 2)], cell=(5, 5, 4))
-    potential = Potential(atoms)
-    linescan = LineScan(start=[0, 0], end=[2.5, 2.5], gpts=10)
-    detector = AnnularDetector(inner=80, outer=200)
-
-    probe = Probe(semiangle_cutoff=30, energy=80e3, gpts=250)
-    measurements = probe.scan(linescan, [detector], potential, max_batch=50, pbar=False)
-
-    S_builder = SMatrix(30, 80e3, 2, gpts=500)
-    atoms = Atoms('C', positions=[(2.5, 2.5, 2)], cell=(5, 5, 4))
-    atoms *= (2, 2, 1)
-    potential = Potential(atoms)
-    S = S_builder.multislice(potential, pbar=False)
-    prism_measurements = S.scan(linescan, [detector], max_batch_probes=10, pbar=False)
-
-    assert np.allclose(measurements[detector].array, prism_measurements[detector].array, atol=1e-6)
-
-
-def test_prism_batch():
-    potential = Potential(Atoms('C', positions=[(2.5, 2.5, 2)], cell=(5, 5, 4)))
-
-    S_builder = SMatrix(30, 80e3, 1, gpts=500)
-    S1 = S_builder.multislice(potential, pbar=False)
-    S2 = S_builder.multislice(potential, max_batch=5, pbar=False)
-
-    assert np.allclose(S1.array, S2.array)
-
-
-# def test_downsample():
-#     S = SMatrix(expansion_cutoff=10, interpolation=2, energy=300e3, extent=10, sampling=.05)
-#     S = S.build().downsample(normalization='values')
-#
-#     S2 = SMatrix(expansion_cutoff=10, interpolation=2, energy=300e3, extent=10, gpts=S.gpts)
-#     S2 = S2.build()
-#
-#     assert np.allclose(S.array - S2.array, 0., atol=5e-6)
-
-def test_downsample_max_angle():
-    S = SMatrix(30, 80e3, 1, gpts=500)
-    potential = Potential(Atoms('C', positions=[(2.5, 2.5, 2)], cell=(5, 5, 4)))
-    S = S.multislice(potential, pbar=False)
-    pattern1 = S.collapse((0, 0)).diffraction_pattern(max_angle=64)
-    S = S.downsample(max_angle=64)
-    pattern2 = S.collapse((0, 0)).diffraction_pattern(None)
-    pattern3 = S.collapse((0, 0)).diffraction_pattern(max_angle=64)
-
-    assert np.allclose(pattern1.array, pattern2.array, atol=1e-6 * pattern1.array.max(), rtol=1e-6)
-    assert np.allclose(pattern3.array, pattern2.array, atol=1e-6 * pattern1.array.max(), rtol=1e-6)
-
-
-def test_downsample_detect():
-    atoms = read('data/srtio3_100.cif')
-    atoms *= (4, 4, 1)
-
-    potential = Potential(atoms, gpts=256, device='gpu', projection='infinite', slice_thickness=.5,
-                          parametrization='kirkland', storage='gpu').build(pbar=False)
-
-    detector = FlexibleAnnularDetector()
-    end = (potential.extent[0] / 4, potential.extent[1] / 4)
-    gridscan = GridScan(start=[0, 0], end=end, sampling=.2)
-    S = SMatrix(energy=300e3, semiangle_cutoff=9.4, device='gpu', rolloff=0.05, expansion_cutoff=10)
-    S_exit = S.multislice(potential, pbar=False)
-    measurements = S_exit.scan(gridscan, [detector], pbar=False)
-    S_downsampled = S_exit.downsample()
-
-    downsampled_measurements = S_downsampled.scan(gridscan, [detector], pbar=False)
-
-    assert S_downsampled.array.shape != S_exit.array.shape
-    assert not np.all(measurements[detector].array == downsampled_measurements[detector].array)
-    assert np.allclose(measurements[detector].array, downsampled_measurements[detector].array)
-
-
-def test_crop():
-    S = SMatrix(expansion_cutoff=30, interpolation=3, energy=300e3, extent=10, sampling=.02).build()
-    gridscan = GridScan(start=[0, 0], end=S.extent, gpts=64)
-
-    scans = gridscan.partition_scan((2, 2))
-    cropped = S.crop_to_scan(scans[0])
-
-    assert cropped.gpts != S.gpts
-
-    position = (4.9, 0.)
-    assert np.allclose(S.collapse(position).array - cropped.collapse(position).array, 0.)
-
-
-@pytest.mark.gpu
-def test_prism_gpu():
-    potential = Potential(Atoms('C', positions=[(2.5, 2.5, 2)], cell=(5, 5, 4)))
-
-    S_builder = SMatrix(30, 80e3, 1, gpts=500, device='cpu')
-    S_cpu = S_builder.multislice(potential, pbar=False)
-
-    assert type(S_cpu.array) is np.ndarray
-
-    S_builder = SMatrix(30, 80e3, 1, gpts=500, device='gpu')
-    S_gpu = S_builder.multislice(potential, pbar=False)
-
-    assert type(S_gpu.array) is cp.ndarray
-    assert np.allclose(S_cpu.array, asnumpy(S_gpu.array))
-
-
-@pytest.mark.gpu
-def test_prism_storage():
-    potential = Potential(Atoms('C', positions=[(2.5, 2.5, 2)], cell=(5, 5, 4)))
-
-    S_builder = SMatrix(30, 80e3, 1, gpts=500, device='gpu', storage='cpu')
-    S_gpu = S_builder.multislice(potential, pbar=False)
-
-    assert type(S_gpu.array) is np.ndarray
-
-
-@pytest.mark.gpu
-def test_cropped_scan():
-    atoms = read(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data/amorphous_carbon.cif'))
-    potential = Potential(atoms, gpts=512, slice_thickness=1, device='gpu', projection='infinite',
-                          parametrization='kirkland', storage='gpu').build(pbar=True)
-    detector = AnnularDetector(inner=40, outer=60)
-    gridscan = GridScan(start=[0, 0], end=potential.extent, gpts=16)
-
-    S = SMatrix(expansion_cutoff=20, interpolation=4, energy=300e3, device='gpu', storage='cpu')  # .build()
-
-    S = S.multislice(potential, pbar=True)
-    S = S.downsample('limit')
-
-    measurements = S.scan(gridscan, [detector], max_batch_probes=64)
-
-    scans = gridscan.partition_scan((2, 2))
-    cropped_measurements = {detector: detector.allocate_measurement(S.collapse((0,0)), gridscan)}
-
-    for scan in scans:
-        cropped = S.crop_to_scan(scan)
-        cropped = cropped.transfer('gpu')
-        cropped_measurements = cropped.scan(scan, cropped_measurements, pbar=False)
-
-    assert np.allclose(cropped_measurements[detector].array, measurements[detector].array)
+import os
+
+import numpy as np
+import pytest
+from abtem.detect import AnnularDetector, FlexibleAnnularDetector
+from abtem.device import asnumpy, cp
+from abtem.potentials import Potential
+from abtem.scan import LineScan, GridScan
+from abtem.waves import Probe, SMatrix
+from ase import Atoms
+from ase.io import read
+
+
+def test_prism_raises():
+    with pytest.raises(ValueError) as e:
+        SMatrix(.01, 80e3, .5)
+
+    assert str(e.value) == 'Interpolation factor must be int'
+
+    with pytest.raises(RuntimeError) as e:
+        prism = SMatrix(10, 80e3, 1)
+        prism.build()
+
+    assert str(e.value) == 'Grid extent is not defined'
+
+
+def test_prism_match_probe():
+    S_builder = SMatrix(30., 60e3, 1, extent=5, gpts=50)
+    probe = Probe(extent=5, gpts=50, energy=60e3, semiangle_cutoff=30., rolloff=0.)
+    assert np.allclose(probe.build([(0., 0.)]).array, S_builder.build().collapse([(0., 0.)]).array, atol=2e-5)
+
+
+def test_prism_translate():
+    S_builder = SMatrix(30, 60e3, 1, extent=5, gpts=50)
+    probe = Probe(extent=5, gpts=50, energy=60e3, semiangle_cutoff=30, rolloff=0)
+    assert np.allclose(probe.build(np.array([(2.5, 2.5)])).array,
+                       S_builder.build().collapse([(2.5, 2.5)]).array, atol=1e-5)
+
+
+def test_prism_interpolation():
+    S_builder = SMatrix(30, 60e3, 2, extent=10, gpts=100)
+    probe = Probe(extent=5, gpts=50, energy=60e3, semiangle_cutoff=30, rolloff=0)
+    assert np.allclose(probe.build(np.array([(2.5, 2.5)])).array,
+                       S_builder.build().collapse([(2.5, 2.5)]).array, atol=1e-5)
+
+
+def test_prism_multislice():
+    potential = Potential(Atoms('C', positions=[(0, 0, 2)], cell=(5, 5, 4)))
+    S = SMatrix(30, 60e3, 1, extent=5, gpts=500)
+    probe = Probe(extent=5, gpts=500, energy=60e3, semiangle_cutoff=30, rolloff=0.)
+    assert np.allclose(probe.build(np.array([[2.5, 2.5]])).multislice(potential, pbar=False).array,
+                       S.multislice(potential, pbar=False).collapse([(2.5, 2.5)]).array, atol=2e-5)
+
+
+def test_probe_waves_line_scan():
+    potential = Potential(Atoms('C', positions=[(2.5, 2.5, 2)], cell=(5, 5, 4)))
+    linescan = LineScan(start=[0, 0], end=[2.5, 2.5], gpts=10)
+    detector = AnnularDetector(inner=80, outer=200)
+
+    S_builder = SMatrix(30, 80e3, 1, gpts=500)
+    S = S_builder.multislice(potential, pbar=False)
+    probe = Probe(semiangle_cutoff=30, energy=80e3, gpts=500)
+
+    prism_measurements = S.scan(linescan, [detector], max_batch_probes=10, pbar=False)
+    measurements = probe.scan(linescan, [detector], potential, max_batch=50, pbar=False)
+
+    assert np.allclose(measurements[detector].array, prism_measurements[detector].array, atol=1e-6)
+
+
+def test_interpolation_scan():
+    atoms = Atoms('C', positions=[(2.5, 2.5, 2)], cell=(5, 5, 4))
+    potential = Potential(atoms)
+    linescan = LineScan(start=[0, 0], end=[2.5, 2.5], gpts=10)
+    detector = AnnularDetector(inner=80, outer=200)
+
+    probe = Probe(semiangle_cutoff=30, energy=80e3, gpts=250)
+    measurements = probe.scan(linescan, [detector], potential, max_batch=50, pbar=False)
+
+    S_builder = SMatrix(30, 80e3, 2, gpts=500)
+    atoms = Atoms('C', positions=[(2.5, 2.5, 2)], cell=(5, 5, 4))
+    atoms *= (2, 2, 1)
+    potential = Potential(atoms)
+    S = S_builder.multislice(potential, pbar=False)
+    prism_measurements = S.scan(linescan, [detector], max_batch_probes=10, pbar=False)
+
+    assert np.allclose(measurements[detector].array, prism_measurements[detector].array, atol=1e-6)
+
+
+def test_prism_batch():
+    potential = Potential(Atoms('C', positions=[(2.5, 2.5, 2)], cell=(5, 5, 4)))
+
+    S_builder = SMatrix(30, 80e3, 1, gpts=500)
+    S1 = S_builder.multislice(potential, pbar=False)
+    S2 = S_builder.multislice(potential, max_batch=5, pbar=False)
+
+    assert np.allclose(S1.array, S2.array)
+
+
+# def test_downsample():
+#     S = SMatrix(expansion_cutoff=10, interpolation=2, energy=300e3, extent=10, sampling=.05)
+#     S = S.build().downsample(normalization='values')
+#
+#     S2 = SMatrix(expansion_cutoff=10, interpolation=2, energy=300e3, extent=10, gpts=S.gpts)
+#     S2 = S2.build()
+#
+#     assert np.allclose(S.array - S2.array, 0., atol=5e-6)
+
+def test_downsample_max_angle():
+    S = SMatrix(30, 80e3, 1, gpts=500)
+    potential = Potential(Atoms('C', positions=[(2.5, 2.5, 2)], cell=(5, 5, 4)))
+    S = S.multislice(potential, pbar=False)
+    pattern1 = S.collapse((0, 0)).diffraction_pattern(max_angle=64)
+    S = S.downsample(max_angle=64)
+    pattern2 = S.collapse((0, 0)).diffraction_pattern(None)
+    pattern3 = S.collapse((0, 0)).diffraction_pattern(max_angle=64)
+
+    assert np.allclose(pattern1.array, pattern2.array, atol=1e-6 * pattern1.array.max(), rtol=1e-6)
+    assert np.allclose(pattern3.array, pattern2.array, atol=1e-6 * pattern1.array.max(), rtol=1e-6)
+
+
+def test_downsample_detect():
+    atoms = read('data/srtio3_100.cif')
+    atoms *= (4, 4, 1)
+
+    potential = Potential(atoms, gpts=256, device='gpu', projection='infinite', slice_thickness=.5,
+                          parametrization='kirkland', storage='gpu').build(pbar=False)
+
+    detector = FlexibleAnnularDetector()
+    end = (potential.extent[0] / 4, potential.extent[1] / 4)
+    gridscan = GridScan(start=[0, 0], end=end, sampling=.2)
+    S = SMatrix(energy=300e3, semiangle_cutoff=9.4, device='gpu', rolloff=0.05, expansion_cutoff=10)
+    S_exit = S.multislice(potential, pbar=False)
+    measurements = S_exit.scan(gridscan, [detector], pbar=False)
+    S_downsampled = S_exit.downsample()
+
+    downsampled_measurements = S_downsampled.scan(gridscan, [detector], pbar=False)
+
+    assert S_downsampled.array.shape != S_exit.array.shape
+    assert not np.all(measurements[detector].array == downsampled_measurements[detector].array)
+    assert np.allclose(measurements[detector].array, downsampled_measurements[detector].array)
+
+
+def test_crop():
+    S = SMatrix(expansion_cutoff=30, interpolation=3, energy=300e3, extent=10, sampling=.02).build()
+    gridscan = GridScan(start=[0, 0], end=S.extent, gpts=64)
+
+    scans = gridscan.partition_scan((2, 2))
+    cropped = S.crop_to_scan(scans[0])
+
+    assert cropped.gpts != S.gpts
+
+    position = (4.9, 0.)
+    assert np.allclose(S.collapse(position).array - cropped.collapse(position).array, 0.)
+
+
+@pytest.mark.gpu
+def test_prism_gpu():
+    potential = Potential(Atoms('C', positions=[(2.5, 2.5, 2)], cell=(5, 5, 4)))
+
+    S_builder = SMatrix(30, 80e3, 1, gpts=500, device='cpu')
+    S_cpu = S_builder.multislice(potential, pbar=False)
+
+    assert type(S_cpu.array) is np.ndarray
+
+    S_builder = SMatrix(30, 80e3, 1, gpts=500, device='gpu')
+    S_gpu = S_builder.multislice(potential, pbar=False)
+
+    assert type(S_gpu.array) is cp.ndarray
+    assert np.allclose(S_cpu.array, asnumpy(S_gpu.array))
+
+
+@pytest.mark.gpu
+def test_prism_storage():
+    potential = Potential(Atoms('C', positions=[(2.5, 2.5, 2)], cell=(5, 5, 4)))
+
+    S_builder = SMatrix(30, 80e3, 1, gpts=500, device='gpu', storage='cpu')
+    S_gpu = S_builder.multislice(potential, pbar=False)
+
+    assert type(S_gpu.array) is np.ndarray
+
+
+@pytest.mark.gpu
+def test_cropped_scan():
+    atoms = read(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data/amorphous_carbon.cif'))
+    potential = Potential(atoms, gpts=512, slice_thickness=1, device='gpu', projection='infinite',
+                          parametrization='kirkland', storage='gpu').build(pbar=True)
+    detector = AnnularDetector(inner=40, outer=60)
+    gridscan = GridScan(start=[0, 0], end=potential.extent, gpts=16)
+
+    S = SMatrix(expansion_cutoff=20, interpolation=4, energy=300e3, device='gpu', storage='cpu')  # .build()
+
+    S = S.multislice(potential, pbar=True)
+    S = S.downsample('limit')
+
+    measurements = S.scan(gridscan, [detector], max_batch_probes=64)
+
+    scans = gridscan.partition_scan((2, 2))
+    cropped_measurements = {detector: detector.allocate_measurement(S.collapse((0,0)), gridscan)}
+
+    for scan in scans:
+        cropped = S.crop_to_scan(scan)
+        cropped = cropped.transfer('gpu')
+        cropped_measurements = cropped.scan(scan, cropped_measurements, pbar=False)
+
+    assert np.allclose(cropped_measurements[detector].array, measurements[detector].array)
```

### Comparing `abtem-1.0.0b8/test/test_propagator.py` & `abtem-1.0.0b9/test/test_propagator.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from abtem.waves import FresnelPropagator, Probe
-import numpy as np
-
-def test_propagator_cache():
-    wave = Probe(extent=10, gpts=100, energy=60e3, semiangle_cutoff=30).build()
-
-    initial_wave_array = wave.array.copy()
-
-    propagator = FresnelPropagator()
-    propagator.propagate(wave, .5)
-    propagator.propagate(wave, .5)
-
-    propagator.propagate(wave, -1)
-
-    assert np.allclose(wave.array.real[0], initial_wave_array.real[0], atol=5e-5)
-    assert np.allclose(wave.array.imag[0], initial_wave_array.imag[0], atol=5e-5)
-
-    assert propagator._cache._hits == 1
-    assert propagator._cache._misses == 2
-
-
-def testbandlimit_propagator():
-    p = FresnelPropagator()
+from abtem.waves import FresnelPropagator, Probe
+import numpy as np
+
+def test_propagator_cache():
+    wave = Probe(extent=10, gpts=100, energy=60e3, semiangle_cutoff=30).build()
+
+    initial_wave_array = wave.array.copy()
+
+    propagator = FresnelPropagator()
+    propagator.propagate(wave, .5)
+    propagator.propagate(wave, .5)
+
+    propagator.propagate(wave, -1)
+
+    assert np.allclose(wave.array.real[0], initial_wave_array.real[0], atol=5e-5)
+    assert np.allclose(wave.array.imag[0], initial_wave_array.imag[0], atol=5e-5)
+
+    assert propagator._cache._hits == 1
+    assert propagator._cache._misses == 2
+
+
+def testbandlimit_propagator():
+    p = FresnelPropagator()
     p = p._evaluate_propagator_array((256, 256), (.02, .02), 80e3, .5, np)
```

### Comparing `abtem-1.0.0b8/test/test_scan.py` & `abtem-1.0.0b9/test/test_scan.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,107 +1,107 @@
-import os
-
-import numpy as np
-import pytest
-from abtem.detect import AnnularDetector
-from abtem.potentials import Potential
-from abtem.scan import PositionScan, LineScan, GridScan
-from abtem.waves import SMatrix
-from ase.io import read
-
-
-def test_custom_scan():
-    positions = np.array([(2, 2), (1, 1)])
-    scan = PositionScan(positions=positions)
-
-    assert np.all(next(scan.generate_positions(1))[1] == positions[0])
-    assert np.all(next(scan.generate_positions(2))[1] == positions)
-
-
-def test_linescan_raises():
-    with pytest.raises(ValueError) as e:
-        LineScan(start=0, end=1)
-
-    assert str(e.value) == 'Scan start/end has incorrect shape'
-
-
-def test_line_scan():
-    start = (0, 0)
-    end = (1, 1)
-    scan = LineScan(start, end, gpts=5)
-
-    positions = scan.get_positions()
-    assert np.allclose(positions[0], start)
-    assert np.allclose(positions[-1], end)
-    assert np.allclose(positions[2], np.mean([start, end], axis=0))
-    assert np.allclose(np.linalg.norm(np.diff(positions, axis=0), axis=1), scan.sampling[0])
-
-    scan = LineScan(start, end, gpts=5, endpoint=False)
-    positions = scan.get_positions()
-    assert np.allclose(positions[0], start)
-    assert np.allclose(positions[-1], (end[0] - (end[0] - start[0]) / 5, end[1] - (end[1] - start[1]) / 5))
-
-
-def test_gridscan_raises():
-    with pytest.raises(ValueError) as e:
-        GridScan(start=0, end=1)
-
-    assert str(e.value) == 'Scan start/end has incorrect shape'
-
-
-def test_grid_scan():
-    start = (0, 0)
-    end = (1, 2)
-    scan = GridScan(start, end, gpts=5, endpoint=True)
-
-    positions = scan.get_positions()
-    assert np.all(positions[0] == start)
-    assert np.all(positions[-1] == end)
-    assert np.allclose(positions[4], [start[1], end[1]])
-    assert np.allclose(np.linalg.norm(np.diff(positions[:4], axis=0), axis=1), scan.sampling[1])
-
-    scan = GridScan(start, end, gpts=5, endpoint=False)
-    positions = scan.get_positions()
-    assert np.all(positions[0] == start)
-    assert np.allclose(positions[-1], (end[0] - (end[0] - start[0]) / 5, end[1] - (end[1] - start[1]) / 5))
-
-
-def test_partition():
-    gridscan = GridScan(start=(0, 0), end=(2, 2), sampling=.5, endpoint=False)
-    scans = gridscan.partition_scan((2, 2))
-    positions = []
-    for scan in scans:
-        positions.append(scan.get_positions())
-
-    assert np.allclose(((np.vstack(positions)[None] - gridscan.get_positions()[:, None]) ** 2).min(0), 0)
-    assert np.allclose(((np.vstack(positions)[None] - gridscan.get_positions()[:, None]) ** 2).min(1), 0)
-
-    gridscan = GridScan(start=(0, 0), end=(2, 2), sampling=.5, endpoint=True)
-    scans = gridscan.partition_scan((2, 2))
-    positions = []
-    for scan in scans:
-        positions.append(scan.get_positions())
-
-    assert np.allclose(((np.vstack(positions)[None] - gridscan.get_positions()[:, None]) ** 2).min(0), 0)
-    assert np.allclose(((np.vstack(positions)[None] - gridscan.get_positions()[:, None]) ** 2).min(1), 0)
-
-
-def test_partition_measurement():
-    atoms = read(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data/amorphous_carbon.cif'))
-    potential = Potential(atoms, gpts=512, slice_thickness=1, projection='infinite',
-                          parametrization='kirkland').build(pbar=False)
-
-    detector = AnnularDetector(inner=70, outer=100)
-    gridscan = GridScan(start=[0, 0], end=potential.extent, gpts=16)
-
-    S = SMatrix(expansion_cutoff=15, interpolation=1, energy=300e3)
-    S = S.multislice(potential, pbar=False)
-
-    measurements = S.scan(gridscan, [detector], pbar=False)
-
-    scans = gridscan.partition_scan((2, 2))
-    partitioned_measurements = {detector: detector.allocate_measurement(S.collapse((0, 0)), gridscan)}
-
-    for scan in scans:
-        partitioned_measurements = S.scan(scan, measurements, pbar=False)
-
-    assert np.allclose(partitioned_measurements[detector].array, measurements[detector].array)
+import os
+
+import numpy as np
+import pytest
+from abtem.detect import AnnularDetector
+from abtem.potentials import Potential
+from abtem.scan import PositionScan, LineScan, GridScan
+from abtem.waves import SMatrix
+from ase.io import read
+
+
+def test_custom_scan():
+    positions = np.array([(2, 2), (1, 1)])
+    scan = PositionScan(positions=positions)
+
+    assert np.all(next(scan.generate_positions(1))[1] == positions[0])
+    assert np.all(next(scan.generate_positions(2))[1] == positions)
+
+
+def test_linescan_raises():
+    with pytest.raises(ValueError) as e:
+        LineScan(start=0, end=1)
+
+    assert str(e.value) == 'Scan start/end has incorrect shape'
+
+
+def test_line_scan():
+    start = (0, 0)
+    end = (1, 1)
+    scan = LineScan(start, end, gpts=5)
+
+    positions = scan.get_positions()
+    assert np.allclose(positions[0], start)
+    assert np.allclose(positions[-1], end)
+    assert np.allclose(positions[2], np.mean([start, end], axis=0))
+    assert np.allclose(np.linalg.norm(np.diff(positions, axis=0), axis=1), scan.sampling[0])
+
+    scan = LineScan(start, end, gpts=5, endpoint=False)
+    positions = scan.get_positions()
+    assert np.allclose(positions[0], start)
+    assert np.allclose(positions[-1], (end[0] - (end[0] - start[0]) / 5, end[1] - (end[1] - start[1]) / 5))
+
+
+def test_gridscan_raises():
+    with pytest.raises(ValueError) as e:
+        GridScan(start=0, end=1)
+
+    assert str(e.value) == 'Scan start/end has incorrect shape'
+
+
+def test_grid_scan():
+    start = (0, 0)
+    end = (1, 2)
+    scan = GridScan(start, end, gpts=5, endpoint=True)
+
+    positions = scan.get_positions()
+    assert np.all(positions[0] == start)
+    assert np.all(positions[-1] == end)
+    assert np.allclose(positions[4], [start[1], end[1]])
+    assert np.allclose(np.linalg.norm(np.diff(positions[:4], axis=0), axis=1), scan.sampling[1])
+
+    scan = GridScan(start, end, gpts=5, endpoint=False)
+    positions = scan.get_positions()
+    assert np.all(positions[0] == start)
+    assert np.allclose(positions[-1], (end[0] - (end[0] - start[0]) / 5, end[1] - (end[1] - start[1]) / 5))
+
+
+def test_partition():
+    gridscan = GridScan(start=(0, 0), end=(2, 2), sampling=.5, endpoint=False)
+    scans = gridscan.partition_scan((2, 2))
+    positions = []
+    for scan in scans:
+        positions.append(scan.get_positions())
+
+    assert np.allclose(((np.vstack(positions)[None] - gridscan.get_positions()[:, None]) ** 2).min(0), 0)
+    assert np.allclose(((np.vstack(positions)[None] - gridscan.get_positions()[:, None]) ** 2).min(1), 0)
+
+    gridscan = GridScan(start=(0, 0), end=(2, 2), sampling=.5, endpoint=True)
+    scans = gridscan.partition_scan((2, 2))
+    positions = []
+    for scan in scans:
+        positions.append(scan.get_positions())
+
+    assert np.allclose(((np.vstack(positions)[None] - gridscan.get_positions()[:, None]) ** 2).min(0), 0)
+    assert np.allclose(((np.vstack(positions)[None] - gridscan.get_positions()[:, None]) ** 2).min(1), 0)
+
+
+def test_partition_measurement():
+    atoms = read(os.path.join(os.path.dirname(os.path.abspath(__file__)), 'data/amorphous_carbon.cif'))
+    potential = Potential(atoms, gpts=512, slice_thickness=1, projection='infinite',
+                          parametrization='kirkland').build(pbar=False)
+
+    detector = AnnularDetector(inner=70, outer=100)
+    gridscan = GridScan(start=[0, 0], end=potential.extent, gpts=16)
+
+    S = SMatrix(expansion_cutoff=15, interpolation=1, energy=300e3)
+    S = S.multislice(potential, pbar=False)
+
+    measurements = S.scan(gridscan, [detector], pbar=False)
+
+    scans = gridscan.partition_scan((2, 2))
+    partitioned_measurements = {detector: detector.allocate_measurement(S.collapse((0, 0)), gridscan)}
+
+    for scan in scans:
+        partitioned_measurements = S.scan(scan, measurements, pbar=False)
+
+    assert np.allclose(partitioned_measurements[detector].array, measurements[detector].array)
```

### Comparing `abtem-1.0.0b8/test/test_temperature.py` & `abtem-1.0.0b9/test/test_temperature.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import numpy as np
-import pytest
-from ase import Atoms
-
-from abtem.detect import AnnularDetector
-from abtem.potentials import Potential
-from abtem.scan import LineScan
-from abtem.waves import Probe, SMatrix
-from abtem.device import asnumpy, cp
-from abtem import FrozenPhonons
-
-
-def test_frozen_phonons_raise():
-    atoms = Atoms('CO', positions=[(2.5, 2.5, 2), (2.5, 2.5, 3)], cell=(5, 5, 4))
-
-    with pytest.raises(RuntimeError) as e:
-        frozen_phonons = FrozenPhonons(atoms, 10, sigmas={'C': .1})
-
-    assert str(e.value) == 'Displacement standard deviation not provided for all atomic species.'
-
-
-def test_probe_waves_line_scan():
-    atoms = Atoms('CO', positions=[(2.5, 2.5, 2), (2.5, 2.5, 3)], cell=(5, 5, 4))
-    frozen_phonons = FrozenPhonons(atoms, 2, sigmas={'C': 0, 'O': 0.})
-
-    potential = Potential(atoms, sampling=.05)
-    tds_potential = Potential(frozen_phonons, sampling=.05)
-
-    linescan = LineScan(start=[0, 0], end=[2.5, 2.5], gpts=10)
-    detector = AnnularDetector(inner=80, outer=200)
-
-    probe = Probe(semiangle_cutoff=30, energy=80e3, gpts=500)
-
-    measurements = probe.scan(linescan, [detector], potential, max_batch=50, pbar=False)
-    tds_measurements = probe.scan(linescan, [detector], tds_potential, max_batch=50, pbar=False)
-    assert np.allclose(measurements[detector].array, tds_measurements[detector].array, atol=1e-6)
-
-    frozen_phonons = FrozenPhonons(atoms, 2, sigmas={'C': 0, 'O': 0.1})
-    tds_potential = Potential(frozen_phonons, sampling=.05)
-    tds_measurements = probe.scan(linescan, [detector], tds_potential, max_batch=50, pbar=False)
+import numpy as np
+import pytest
+from ase import Atoms
+
+from abtem.detect import AnnularDetector
+from abtem.potentials import Potential
+from abtem.scan import LineScan
+from abtem.waves import Probe, SMatrix
+from abtem.device import asnumpy, cp
+from abtem import FrozenPhonons
+
+
+def test_frozen_phonons_raise():
+    atoms = Atoms('CO', positions=[(2.5, 2.5, 2), (2.5, 2.5, 3)], cell=(5, 5, 4))
+
+    with pytest.raises(RuntimeError) as e:
+        frozen_phonons = FrozenPhonons(atoms, 10, sigmas={'C': .1})
+
+    assert str(e.value) == 'Displacement standard deviation not provided for all atomic species.'
+
+
+def test_probe_waves_line_scan():
+    atoms = Atoms('CO', positions=[(2.5, 2.5, 2), (2.5, 2.5, 3)], cell=(5, 5, 4))
+    frozen_phonons = FrozenPhonons(atoms, 2, sigmas={'C': 0, 'O': 0.})
+
+    potential = Potential(atoms, sampling=.05)
+    tds_potential = Potential(frozen_phonons, sampling=.05)
+
+    linescan = LineScan(start=[0, 0], end=[2.5, 2.5], gpts=10)
+    detector = AnnularDetector(inner=80, outer=200)
+
+    probe = Probe(semiangle_cutoff=30, energy=80e3, gpts=500)
+
+    measurements = probe.scan(linescan, [detector], potential, max_batch=50, pbar=False)
+    tds_measurements = probe.scan(linescan, [detector], tds_potential, max_batch=50, pbar=False)
+    assert np.allclose(measurements[detector].array, tds_measurements[detector].array, atol=1e-6)
+
+    frozen_phonons = FrozenPhonons(atoms, 2, sigmas={'C': 0, 'O': 0.1})
+    tds_potential = Potential(frozen_phonons, sampling=.05)
+    tds_measurements = probe.scan(linescan, [detector], tds_potential, max_batch=50, pbar=False)
     assert not np.allclose(measurements[detector].array, tds_measurements[detector].array, atol=1e-6)
```

### Comparing `abtem-1.0.0b8/test/test_waves.py` & `abtem-1.0.0b9/test/test_waves.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,227 +1,227 @@
-from copy import copy
-
-import numpy as np
-import pytest
-
-from abtem.base_classes import Grid, AntialiasFilter
-from abtem.detect import AbstractDetector
-from abtem.measure import Measurement
-from abtem.potentials import AbstractPotential, PotentialArray
-from abtem.scan import LineScan, GridScan
-from abtem.waves import Waves, PlaneWave, Probe
-
-
-class DummyPotential(AbstractPotential):
-
-    def __init__(self, extent=None, gpts=None, sampling=None, num_slices=10):
-        self._num_slices = num_slices
-        self._grid = Grid(extent=extent, gpts=gpts, sampling=sampling)
-
-    @property
-    def num_slices(self):
-        return 10
-
-    def get_slice_thickness(self, i):
-        return .5
-
-    def generate_slices(self, start=0, end=None, max_batch=1):
-        for i in range(self.num_slices):
-            array = np.zeros(self.gpts, dtype=np.float32)
-            array[:self.gpts[0] // 2] = 1
-            yield start, end, PotentialArray(array[None],
-                                             slice_thicknesses=np.array([self.get_slice_thickness(i)]),
-                                             extent=self.extent)
-
-
-@pytest.fixture
-def potential():
-    return DummyPotential(extent=5, gpts=50)
-
-
-def test_create_waves():
-    array = np.ones((1, 25, 25), dtype=np.complex64)
-    waves = Waves(array)
-    waves.extent = 10
-
-    assert (waves.sampling[0] == 10 / array.shape[1]) & (waves.sampling[1] == 10 / array.shape[2])
-
-    with pytest.raises(RuntimeError):
-        waves.gpts = 200
-
-    waves = Waves(array, sampling=.2)
-    assert (waves.extent[0] == array.shape[1] * .2) & (waves.extent[1] == array.shape[2] * .2)
-
-
-def test_waves_raises():
-    array = np.ones((1, 25, 25), dtype=np.complex64)
-    waves = Waves(array)
-
-    with pytest.raises(RuntimeError):
-        waves.grid.check_is_defined()
-
-    waves = Waves(array, extent=5)
-
-    with pytest.raises(RuntimeError):
-        waves.accelerator.check_is_defined()
-
-    waves = Waves(array, extent=5, energy=60e3)
-
-    waves.grid.check_is_defined()
-    waves.accelerator.check_is_defined()
-
-
-def test_multislice():
-    array = np.ones((1, 25, 25), dtype=np.complex64)
-    waves = Waves(array, energy=60e3)
-
-    potential = DummyPotential(extent=5)
-
-    new_waves = waves.multislice(potential, pbar=False)
-
-    assert potential.gpts is not None
-    assert waves.extent is not None
-    assert new_waves is waves
-
-    new_waves = copy(new_waves)
-    new_waves = new_waves.multislice(potential, pbar=False)
-
-    assert potential.gpts is not None
-    assert waves.extent is not None
-    assert not np.all(np.isclose(new_waves.array, waves.array))
-
-
-def test_multislice_raises():
-    array = np.ones((1, 25, 25), dtype=np.complex64)
-    potential = DummyPotential(extent=5)
-
-    waves = Waves(array, extent=5)
-    with pytest.raises(RuntimeError) as e:
-        waves.multislice(potential, pbar=False)
-
-    assert str(e.value) == 'Energy is not defined'
-
-    waves.energy = 60e3
-    waves.multislice(potential, pbar=False)
-
-
-def test_create_plane_waves():
-    plane_wave = PlaneWave(extent=2, gpts=10, energy=60e3)
-    waves = plane_wave.build()
-    assert np.all(waves.array == np.ones((10, 10), dtype=np.complex64))
-
-
-def test_plane_waves_raises():
-    plane_waves = PlaneWave(energy=60e3)
-
-    with pytest.raises(RuntimeError) as e:
-        plane_waves.multislice(DummyPotential(extent=5), pbar=False)
-
-    assert str(e.value) == 'Grid gpts cannot be inferred'
-
-
-def test_plane_waves_multislice():
-    plane_waves = PlaneWave(gpts=50, energy=60e3)
-    plane_waves.multislice(DummyPotential(extent=5))
-
-    plane_waves = PlaneWave(sampling=.1, energy=60e3)
-    plane_waves.multislice(DummyPotential(extent=5))
-
-
-def test_create_probe_waves():
-    probe_waves = Probe(extent=10, gpts=10, energy=60e3, defocus=10, C32=30, **{'C10': 100})
-
-    waves = probe_waves.build()
-
-    assert waves.array.shape == (1, 10, 10)
-
-    waves = probe_waves.build([[0, 0], [1, 1]])
-
-    assert waves.array.shape == (2, 10, 10)
-
-
-def test_probe_waves_raises():
-    with pytest.raises(ValueError) as e:
-        Probe(not_a_parameter=10)
-
-    assert str(e.value) == 'not_a_parameter not a recognized parameter'
-
-    probe = Probe()
-    with pytest.raises(RuntimeError) as e:
-        probe.build()
-
-    assert str(e.value) == 'Grid extent is not defined'
-
-    probe.extent = 10
-    probe.gpts = 100
-    with pytest.raises(RuntimeError) as e:
-        probe.build()
-
-    assert str(e.value) == 'Energy is not defined'
-
-    probe.energy = 60e3
-    probe.build()
-
-
-def test_downsample():
-    f = AntialiasFilter()
-
-    sampling = (.1, .1)
-    gpts = (228, 229)
-
-    mask = f.get_mask(gpts, sampling, np)
-    n = np.sum(mask > 0.)
-
-    array = np.fft.ifft2(mask)
-
-    waves = Waves(array, sampling=sampling, energy=80e3)
-
-    assert np.allclose(waves.downsample('valid', return_fourier_space=True).array.real, 1.)
-    assert not np.allclose(waves.downsample('limit', return_fourier_space=True).array.real, 1.)
-    assert np.sum(waves.downsample('limit', return_fourier_space=True).array.real > 1e-6) == n
-
-
-class DummyDetector(AbstractDetector):
-
-    def __init__(self):
-        self._detect_count = 0
-        super().__init__()
-
-    def detect(self, waves):
-        self._detect_count += 1
-        return np.array([1.])
-
-    def allocate_measurement(self, waves, scan):
-        array = np.zeros(scan.shape, dtype=np.float32)
-        return Measurement(array, calibrations=scan.calibrations)
-
-
-def test_probe_waves_line_scan():
-    probe = Probe(energy=60e3)
-    detector = DummyDetector()
-    potential = DummyPotential(extent=5, sampling=.1)
-
-    scan = LineScan((0, 0), (1, 1), gpts=10)
-    measurements = probe.scan(scan, [detector], potential, max_batch=1, pbar=False)
-
-    assert detector._detect_count == 10
-    assert np.all(measurements[detector].array == 1.)
-
-    measurements = probe.scan(scan, [detector], potential, pbar=False)
-    assert detector._detect_count == 11
-    assert np.all(measurements[detector].array == 1.)
-
-    measurements = probe.scan(scan, [detector], potential, max_batch=3, pbar=False)
-    assert detector._detect_count == 15
-    assert np.all(measurements[detector].array == 1.)
-
-
-def test_probe_waves_grid_scan():
-    probe = Probe(energy=60e3)
-    detector = DummyDetector()
-    potential = DummyPotential(extent=5, sampling=.1)
-
-    scan = GridScan((0, 0), (1, 1), gpts=10)
-    measurements = probe.scan(scan, [detector], potential, max_batch=1, pbar=False)
-
-    assert detector._detect_count == 100
-    assert np.all(measurements[detector].array == 1.)
+from copy import copy
+
+import numpy as np
+import pytest
+
+from abtem.base_classes import Grid, AntialiasFilter
+from abtem.detect import AbstractDetector
+from abtem.measure import Measurement
+from abtem.potentials import AbstractPotential, PotentialArray
+from abtem.scan import LineScan, GridScan
+from abtem.waves import Waves, PlaneWave, Probe
+
+
+class DummyPotential(AbstractPotential):
+
+    def __init__(self, extent=None, gpts=None, sampling=None, num_slices=10):
+        self._num_slices = num_slices
+        self._grid = Grid(extent=extent, gpts=gpts, sampling=sampling)
+
+    @property
+    def num_slices(self):
+        return 10
+
+    def get_slice_thickness(self, i):
+        return .5
+
+    def generate_slices(self, start=0, end=None, max_batch=1):
+        for i in range(self.num_slices):
+            array = np.zeros(self.gpts, dtype=np.float32)
+            array[:self.gpts[0] // 2] = 1
+            yield start, end, PotentialArray(array[None],
+                                             slice_thicknesses=np.array([self.get_slice_thickness(i)]),
+                                             extent=self.extent)
+
+
+@pytest.fixture
+def potential():
+    return DummyPotential(extent=5, gpts=50)
+
+
+def test_create_waves():
+    array = np.ones((1, 25, 25), dtype=np.complex64)
+    waves = Waves(array)
+    waves.extent = 10
+
+    assert (waves.sampling[0] == 10 / array.shape[1]) & (waves.sampling[1] == 10 / array.shape[2])
+
+    with pytest.raises(RuntimeError):
+        waves.gpts = 200
+
+    waves = Waves(array, sampling=.2)
+    assert (waves.extent[0] == array.shape[1] * .2) & (waves.extent[1] == array.shape[2] * .2)
+
+
+def test_waves_raises():
+    array = np.ones((1, 25, 25), dtype=np.complex64)
+    waves = Waves(array)
+
+    with pytest.raises(RuntimeError):
+        waves.grid.check_is_defined()
+
+    waves = Waves(array, extent=5)
+
+    with pytest.raises(RuntimeError):
+        waves.accelerator.check_is_defined()
+
+    waves = Waves(array, extent=5, energy=60e3)
+
+    waves.grid.check_is_defined()
+    waves.accelerator.check_is_defined()
+
+
+def test_multislice():
+    array = np.ones((1, 25, 25), dtype=np.complex64)
+    waves = Waves(array, energy=60e3)
+
+    potential = DummyPotential(extent=5)
+
+    new_waves = waves.multislice(potential, pbar=False)
+
+    assert potential.gpts is not None
+    assert waves.extent is not None
+    assert new_waves is waves
+
+    new_waves = copy(new_waves)
+    new_waves = new_waves.multislice(potential, pbar=False)
+
+    assert potential.gpts is not None
+    assert waves.extent is not None
+    assert not np.all(np.isclose(new_waves.array, waves.array))
+
+
+def test_multislice_raises():
+    array = np.ones((1, 25, 25), dtype=np.complex64)
+    potential = DummyPotential(extent=5)
+
+    waves = Waves(array, extent=5)
+    with pytest.raises(RuntimeError) as e:
+        waves.multislice(potential, pbar=False)
+
+    assert str(e.value) == 'Energy is not defined'
+
+    waves.energy = 60e3
+    waves.multislice(potential, pbar=False)
+
+
+def test_create_plane_waves():
+    plane_wave = PlaneWave(extent=2, gpts=10, energy=60e3)
+    waves = plane_wave.build()
+    assert np.all(waves.array == np.ones((10, 10), dtype=np.complex64))
+
+
+def test_plane_waves_raises():
+    plane_waves = PlaneWave(energy=60e3)
+
+    with pytest.raises(RuntimeError) as e:
+        plane_waves.multislice(DummyPotential(extent=5), pbar=False)
+
+    assert str(e.value) == 'Grid gpts cannot be inferred'
+
+
+def test_plane_waves_multislice():
+    plane_waves = PlaneWave(gpts=50, energy=60e3)
+    plane_waves.multislice(DummyPotential(extent=5))
+
+    plane_waves = PlaneWave(sampling=.1, energy=60e3)
+    plane_waves.multislice(DummyPotential(extent=5))
+
+
+def test_create_probe_waves():
+    probe_waves = Probe(extent=10, gpts=10, energy=60e3, defocus=10, C32=30, **{'C10': 100})
+
+    waves = probe_waves.build()
+
+    assert waves.array.shape == (1, 10, 10)
+
+    waves = probe_waves.build([[0, 0], [1, 1]])
+
+    assert waves.array.shape == (2, 10, 10)
+
+
+def test_probe_waves_raises():
+    with pytest.raises(ValueError) as e:
+        Probe(not_a_parameter=10)
+
+    assert str(e.value) == 'not_a_parameter not a recognized parameter'
+
+    probe = Probe()
+    with pytest.raises(RuntimeError) as e:
+        probe.build()
+
+    assert str(e.value) == 'Grid extent is not defined'
+
+    probe.extent = 10
+    probe.gpts = 100
+    with pytest.raises(RuntimeError) as e:
+        probe.build()
+
+    assert str(e.value) == 'Energy is not defined'
+
+    probe.energy = 60e3
+    probe.build()
+
+
+def test_downsample():
+    f = AntialiasFilter()
+
+    sampling = (.1, .1)
+    gpts = (228, 229)
+
+    mask = f.get_mask(gpts, sampling, np)
+    n = np.sum(mask > 0.)
+
+    array = np.fft.ifft2(mask)
+
+    waves = Waves(array, sampling=sampling, energy=80e3)
+
+    assert np.allclose(waves.downsample('valid', return_fourier_space=True).array.real, 1.)
+    assert not np.allclose(waves.downsample('limit', return_fourier_space=True).array.real, 1.)
+    assert np.sum(waves.downsample('limit', return_fourier_space=True).array.real > 1e-6) == n
+
+
+class DummyDetector(AbstractDetector):
+
+    def __init__(self):
+        self._detect_count = 0
+        super().__init__()
+
+    def detect(self, waves):
+        self._detect_count += 1
+        return np.array([1.])
+
+    def allocate_measurement(self, waves, scan):
+        array = np.zeros(scan.shape, dtype=np.float32)
+        return Measurement(array, calibrations=scan.calibrations)
+
+
+def test_probe_waves_line_scan():
+    probe = Probe(energy=60e3)
+    detector = DummyDetector()
+    potential = DummyPotential(extent=5, sampling=.1)
+
+    scan = LineScan((0, 0), (1, 1), gpts=10)
+    measurements = probe.scan(scan, [detector], potential, max_batch=1, pbar=False)
+
+    assert detector._detect_count == 10
+    assert np.all(measurements[detector].array == 1.)
+
+    measurements = probe.scan(scan, [detector], potential, pbar=False)
+    assert detector._detect_count == 11
+    assert np.all(measurements[detector].array == 1.)
+
+    measurements = probe.scan(scan, [detector], potential, max_batch=3, pbar=False)
+    assert detector._detect_count == 15
+    assert np.all(measurements[detector].array == 1.)
+
+
+def test_probe_waves_grid_scan():
+    probe = Probe(energy=60e3)
+    detector = DummyDetector()
+    potential = DummyPotential(extent=5, sampling=.1)
+
+    scan = GridScan((0, 0), (1, 1), gpts=10)
+    measurements = probe.scan(scan, [detector], potential, max_batch=1, pbar=False)
+
+    assert detector._detect_count == 100
+    assert np.all(measurements[detector].array == 1.)
```

