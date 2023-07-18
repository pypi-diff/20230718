# Comparing `tmp/ewoksxrpd-0.4.0.tar.gz` & `tmp/ewoksxrpd-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ewoksxrpd-0.4.0.tar", last modified: Mon Jul  3 06:52:21 2023, max compression
+gzip compressed data, was "dist/ewoksxrpd-0.5.0.tar", last modified: Tue Jul 18 15:28:22 2023, max compression
```

## Comparing `ewoksxrpd-0.4.0.tar` & `ewoksxrpd-0.5.0.tar`

### file list

```diff
@@ -1,90 +1,91 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/
--rw-rw-rw-   0 root         (0) root         (0)     1102 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)     1305 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)     1572 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/
--rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/gui/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 06:52:15.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/gui/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    20304 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/gui/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     2667 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/gui/plots.py
--rw-rw-rw-   0 root         (0) root         (0)      960 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/gui/serialize.py
--rw-rw-rw-   0 root         (0) root         (0)     5302 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/gui/trigger_widget.py
--rw-rw-rw-   0 root         (0) root         (0)     1582 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/init_matplotlib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 06:52:15.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/ascii.py
--rw-rw-rw-   0 root         (0) root         (0)      676 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/background.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/bliss.py
--rw-rw-rw-   0 root         (0) root         (0)    15791 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/calibrate.py
--rw-rw-rw-   0 root         (0) root         (0)      160 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/convolution.py
--rw-rw-rw-   0 root         (0) root         (0)     2036 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/data_access.py
--rw-rw-rw-   0 root         (0) root         (0)     8946 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/diagnostics.py
--rw-rw-rw-   0 root         (0) root         (0)    18974 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/integrate.py
--rw-rw-rw-   0 root         (0) root         (0)     2321 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/mask.py
--rw-rw-rw-   0 root         (0) root         (0)      620 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/morphology.py
--rw-rw-rw-   0 root         (0) root         (0)     4159 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     4267 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/pyfaiconfig.py
--rw-rw-rw-   0 root         (0) root         (0)     1283 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/save_images.py
--rw-rw-rw-   0 root         (0) root         (0)     4876 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/sum.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 06:52:15.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3754 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/data_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/integrate_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    10315 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/pyfai_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1774 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     4419 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/worker.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 06:52:15.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6318 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     1629 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_ascii.py
--rw-rw-rw-   0 root         (0) root         (0)     1404 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_background.py
--rw-rw-rw-   0 root         (0) root         (0)     2253 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_batch_integrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1806 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py
--rw-rw-rw-   0 root         (0) root         (0)    10366 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_calibrate.py
--rw-rw-rw-   0 root         (0) root         (0)    20665 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_calint_workflow.py
--rw-rw-rw-   0 root         (0) root         (0)     4679 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_integrate.py
--rw-rw-rw-   0 root         (0) root         (0)     1709 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_mask.py
--rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     3795 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_nexus_integrated.py
--rw-rw-rw-   0 root         (0) root         (0)      963 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_pyfai_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      745 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_save_images.py
--rw-rw-rw-   0 root         (0) root         (0)      683 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_sum.py
--rw-rw-rw-   0 root         (0) root         (0)     1850 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/ewoksxrpd/tests/xrpd_theory.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1305 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2802 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      228 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       14 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0) root         (0)      259 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       24 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/orangecontrib/
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/
--rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1448 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/ascii.py
--rw-rw-rw-   0 root         (0) root         (0)     2635 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/background.py
--rw-rw-rw-   0 root         (0) root         (0)     1361 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/batchintegrate.py
--rw-rw-rw-   0 root         (0) root         (0)     2553 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py
--rw-rw-rw-   0 root         (0) root         (0)     1521 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/calculategeometry.py
--rw-rw-rw-   0 root         (0) root         (0)    11146 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/calibratemulti.py
--rw-rw-rw-   0 root         (0) root         (0)     7837 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/calibratesingle.py
--rw-rw-rw-   0 root         (0) root         (0)     1385 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py
--rw-rw-rw-   0 root         (0) root         (0)     1443 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/icons/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 06:52:15.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/icons/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   188527 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/icons/category.png
--rw-rw-rw-   0 root         (0) root         (0)   188527 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/icons/widget.png
--rw-rw-rw-   0 root         (0) root         (0)     2178 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/integrate1d.py
--rw-rw-rw-   0 root         (0) root         (0)     3252 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/mask.py
--rw-rw-rw-   0 root         (0) root         (0)     1965 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/nexus.py
--rw-rw-rw-   0 root         (0) root         (0)     1513 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py
--rw-rw-rw-   0 root         (0) root         (0)     1409 2023-07-03 06:47:54.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-03 06:52:21.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/tutorials/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-03 06:52:15.000000 ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/tutorials/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1102 2023-07-18 15:28:02.000000 ewoksxrpd-0.5.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      560 2023-07-18 15:28:02.000000 ewoksxrpd-0.5.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      109 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)     1600 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/
+-rw-rw-rw-   0 root         (0) root         (0)       87 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/gui/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:28:16.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/gui/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    20304 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/gui/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     2667 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/gui/plots.py
+-rw-rw-rw-   0 root         (0) root         (0)      960 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/gui/serialize.py
+-rw-rw-rw-   0 root         (0) root         (0)     5302 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/gui/trigger_widget.py
+-rw-rw-rw-   0 root         (0) root         (0)     1582 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/init_matplotlib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:28:16.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1085 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/ascii.py
+-rw-rw-rw-   0 root         (0) root         (0)      676 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/background.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/bliss.py
+-rw-rw-rw-   0 root         (0) root         (0)    15791 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/calibrate.py
+-rw-rw-rw-   0 root         (0) root         (0)      160 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/convolution.py
+-rw-rw-rw-   0 root         (0) root         (0)     2036 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/data_access.py
+-rw-rw-rw-   0 root         (0) root         (0)     8946 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/diagnostics.py
+-rw-rw-rw-   0 root         (0) root         (0)    19571 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2321 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/mask.py
+-rw-rw-rw-   0 root         (0) root         (0)      620 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/morphology.py
+-rw-rw-rw-   0 root         (0) root         (0)     4159 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     4612 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/pyfaiconfig.py
+-rw-rw-rw-   0 root         (0) root         (0)     1283 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/save_images.py
+-rw-rw-rw-   0 root         (0) root         (0)     4876 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/sum.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:28:16.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3754 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/utils/data_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/utils/integrate_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    13653 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/utils/pyfai_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1774 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     4168 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/worker.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:28:16.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6318 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     1629 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_ascii.py
+-rw-rw-rw-   0 root         (0) root         (0)     1404 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_background.py
+-rw-rw-rw-   0 root         (0) root         (0)     2525 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_batch_integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1806 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py
+-rw-rw-rw-   0 root         (0) root         (0)    10366 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_calibrate.py
+-rw-rw-rw-   0 root         (0) root         (0)    20665 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_calint_workflow.py
+-rw-rw-rw-   0 root         (0) root         (0)     1872 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_darkflat.py
+-rw-rw-rw-   0 root         (0) root         (0)     4679 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_integrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1709 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     2250 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     3795 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_nexus_integrated.py
+-rw-rw-rw-   0 root         (0) root         (0)      963 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_pyfai_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      745 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_save_images.py
+-rw-rw-rw-   0 root         (0) root         (0)      683 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_sum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1850 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/ewoksxrpd/tests/xrpd_theory.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/ewoksxrpd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1328 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/ewoksxrpd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2839 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/ewoksxrpd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/ewoksxrpd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      228 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/ewoksxrpd.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/ewoksxrpd.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0) root         (0)      286 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/ewoksxrpd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/ewoksxrpd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/orangecontrib/
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/
+-rw-rw-rw-   0 root         (0) root         (0)      529 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1448 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/ascii.py
+-rw-rw-rw-   0 root         (0) root         (0)     2635 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/background.py
+-rw-rw-rw-   0 root         (0) root         (0)     1361 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/batchintegrate.py
+-rw-rw-rw-   0 root         (0) root         (0)     2553 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py
+-rw-rw-rw-   0 root         (0) root         (0)     1521 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/calculategeometry.py
+-rw-rw-rw-   0 root         (0) root         (0)    11146 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/calibratemulti.py
+-rw-rw-rw-   0 root         (0) root         (0)     7837 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/calibratesingle.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py
+-rw-rw-rw-   0 root         (0) root         (0)     1443 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/icons/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:28:16.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/icons/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   188527 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/icons/category.png
+-rw-rw-rw-   0 root         (0) root         (0)   188527 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/icons/widget.png
+-rw-rw-rw-   0 root         (0) root         (0)     2178 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/integrate1d.py
+-rw-rw-rw-   0 root         (0) root         (0)     3252 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/mask.py
+-rw-rw-rw-   0 root         (0) root         (0)     1965 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/nexus.py
+-rw-rw-rw-   0 root         (0) root         (0)     1513 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py
+-rw-rw-rw-   0 root         (0) root         (0)     1409 2023-07-18 15:28:03.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 15:28:22.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/tutorials/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 15:28:16.000000 ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/tutorials/__init__.py
```

### Comparing `ewoksxrpd-0.4.0/LICENSE.md` & `ewoksxrpd-0.5.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/PKG-INFO` & `ewoksxrpd-0.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ewoksxrpd
-Version: 0.4.0
+Version: 0.5.0
 Summary: Data processing workflows for SAXS/WAXS
 Home-page: https://gitlab.esrf.fr/workflow/ewoksxrpd/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksxrpd/
 Project-URL: Documentation, https://ewoksxrpd.readthedocs.io/
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoksxrpd/issues/
 Keywords: orange3 add-on,ewoks
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: online
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE.md
 
 # ewoksxrpd
```

### Comparing `ewoksxrpd-0.4.0/README.md` & `ewoksxrpd-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/setup.cfg` & `ewoksxrpd-0.5.0/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -26,25 +26,27 @@
 python_requires = >=3.7
 install_requires = 
 	numpy
 	scipy
 	silx >=1.1.0
 	pyopencl
 	pyfai >=2023.3
-	ewoksdata >=0.2.6
+	ewoksdata >0.2.6
 	ewoks[orange] >=0.1.2
 	fabio
 	h5py
 namespace_packages = 
 	orangecontrib
 
 [options.packages.find]
 where = src
 
 [options.extras_require]
+online = 
+	ewoksdata[online]
 test = 
 	pytest >=7
 	matplotlib >=3.1
 dev = 
 	%(test)s
 	black >= 23
 	flake8 >=4
```

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/gui/forms.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/gui/forms.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/gui/plots.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/gui/plots.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/gui/serialize.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/gui/serialize.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/gui/trigger_widget.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/gui/trigger_widget.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/init_matplotlib.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/init_matplotlib.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/ascii.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/ascii.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/background.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/background.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/calibrate.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/calibrate.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/data_access.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/data_access.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/diagnostics.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/diagnostics.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/integrate.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/integrate.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
 
 class _BaseIntegrate(
     TaskWithDataAccess,
     input_names=["detector", "geometry", "energy"],
     optional_input_names=[
         "detector_config",
         "mask",
+        "flatfield",
+        "darkcurrent",
         "integration_options",
         "fixed_integration_options",
         "maximum_persistent_workers",
         "references",
         "monitors",
     ],
     register=False,
@@ -65,14 +67,22 @@
             self.get_input_value("detector_config", None)
         )
         config["wavelength"] = xrpd_utils.energy_wavelength(self.inputs.energy)
         if not self.missing_inputs.mask and self.inputs.mask is not None:
             config["mask"] = self.get_image(
                 data_utils.data_from_storage(self.inputs.mask)
             )
+        if not self.missing_inputs.flatfield and self.inputs.flatfield is not None:
+            config["flatfield"] = self.get_image(
+                data_utils.data_from_storage(self.inputs.flatfield)
+            )
+        if not self.missing_inputs.darkcurrent and self.inputs.darkcurrent is not None:
+            config["darkcurrent"] = self.get_image(
+                data_utils.data_from_storage(self.inputs.darkcurrent)
+            )
         return config
 
     def _pyfai_normalization_factor(
         self,
         monitors: List[Union[numpy.ndarray, Number, str, list, None]],
         references: List[Union[numpy.ndarray, Number, str, list, None]],
         ptdata: Optional[Dict[str, numpy.ndarray]] = None,
@@ -194,14 +204,15 @@
         "scan_memory_url",
         "external_output_filename",
         "nxprocess_name",
         "nxmeasurement_name",
         "nxprocess_as_default",
         "flush_period",
     ],
+    output_names=["nxdata_url"],
 ):
     """1D or 2D integration of a single detector in a single Bliss scan with saving."""
 
     def run(self):
         if self.inputs.counter_names:
             counter_names = set(self.inputs.counter_names)
         else:
@@ -363,14 +374,16 @@
                 pyfai_utils.create_nxprocess_links(
                     nxprocess,
                     measurement,
                     self._nxmeasurement_name,
                     mark_as_default=mark_as_default,
                 )
 
+            self.outputs.nxdata_url = f"{nxdata.file.filename}::{nxdata.name}"
+
     @property
     def _nxprocess_name(self):
         if self.inputs.nxprocess_name:
             return self.inputs.nxprocess_name
         default = "integrate"
         if self.inputs.detector_name:
             return f"{self.inputs.detector_name}_{default}"
```

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/mask.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/mask.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/morphology.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/morphology.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/nexus.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/pyfaiconfig.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/pyfaiconfig.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,30 @@
     Task,
     optional_input_names=[
         "filename",
         "filenames",
         "energy",
         "geometry",
         "mask",
+        "flatfield",
+        "darkcurrent",
         "detector",
         "detector_config",
         "calibrant",
         "integration_options",
     ],
     output_names=[
         "energy",
         "geometry",
         "detector",
         "detector_config",
         "calibrant",
         "mask",
+        "flatfield",
+        "darkcurrent",
         "integration_options",
     ],
 ):
     """Parse pyFAI calibration and integration parameters"""
 
     def run(self):
         input_values = self.input_values
@@ -52,14 +56,16 @@
         detector_config = integration_options.pop("detector_config", None)
         if not self.missing_inputs.detector_config:
             detector_config = input_values["detector_config"]
 
         calibrant = input_values.get("calibrant", None)
 
         mask = input_values.get("mask", None)
+        flatfield = input_values.get("flatfield", None)
+        darkcurrent = input_values.get("darkcurrent", None)
 
         geometry = {
             k: integration_options.pop(k)
             for k in ["dist", "poni1", "poni2", "rot1", "rot2", "rot3"]
             if k in integration_options
         }
         if not self.missing_inputs.geometry:
@@ -86,23 +92,27 @@
         if integrator_name in ("sigma_clip", "_sigma_clip_legacy"):
             logger.warning(
                 "'%s' is not compatible with the pyfai worker: use 'sigma_clip_ng'",
                 integrator_name,
             )
             integration_options["integrator_name"] = "sigma_clip_ng"
         if "sigma_clip_ng" == integrator_name and pmethod.split != "no":
-            raise ValueError("cannot combine sigma clipping with pixel splitting")
+            raise ValueError(
+                "to combine sigma clipping with pixel splitting, use 'sigma_clip_legacy'"
+            )
 
         # Split integration and worker options
         self.outputs.energy = energy
         self.outputs.geometry = geometry
         self.outputs.detector = detector
         self.outputs.detector_config = detector_config
         self.outputs.calibrant = calibrant
         self.outputs.mask = mask
+        self.outputs.flatfield = flatfield
+        self.outputs.darkcurrent = darkcurrent
         self.outputs.integration_options = integration_options
 
     def merged_integration_options(self) -> dict:
         """Merge integration options in this order of priority:
 
         - filename (lowest priority)
         - filenames[0]
```

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/save_images.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/save_images.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/sum.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/sum.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/data_utils.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/utils/data_utils.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/utils/xrpd_utils.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tasks/worker.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tasks/worker.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import logging
 from contextlib import contextmanager
 from collections import OrderedDict
-from typing import Iterable, Dict, Mapping, Tuple, Optional
+from typing import Iterable, Dict, Mapping, Tuple
 from ewokscore.hashing import uhash
 
-import numpy
 import pyFAI
 import pyFAI.worker
 
+from .utils import pyfai_utils
+
 _WORKER_POOL = None
 
 
 logger = logging.getLogger(__name__)
 
 
 class WorkerPool:
@@ -75,24 +76,32 @@
     def _create_worker(
         worker_options: Mapping, integration_options: Mapping
     ) -> pyFAI.worker.Worker:
         worker = pyFAI.worker.Worker(**worker_options)
         worker.output = "raw"
 
         integration_options = dict(integration_options)
-        mask = _extract_mask(integration_options)
+        mask = pyfai_utils.extract_mask(integration_options)
+        flatfield = pyfai_utils.extract_flatfield(integration_options)
+        darkcurrent = pyfai_utils.extract_darkcurrent(integration_options)
         provided = set(integration_options)
         worker.set_config(integration_options, consume_keys=True)
 
         unused = {k: v for k, v in integration_options.items() if k in provided}
         if unused:
             logger.warning("Unused pyfai integration options: %s", unused)
 
         if mask is not None:
-            worker.ai.set_mask(mask)
+            worker.ai.detector.set_mask(mask)
+        # Flat/dark correction:
+        #   Icor = (I - darkcurrent) / flatfield
+        if flatfield is not None:
+            worker.ai.detector.set_flatfield(flatfield)
+        if darkcurrent is not None:
+            worker.ai.detector.set_darkcurrent(darkcurrent)
 
         return worker
 
 
 def _get_global_pool() -> WorkerPool:
     global _WORKER_POOL
     if _WORKER_POOL is None:
@@ -107,28 +116,7 @@
 
 @contextmanager
 def persistent_worker(integration_options: Mapping) -> Iterable[pyFAI.worker.Worker]:
     """Get a worker for a particular configuration that stays in memory."""
     pool = _get_global_pool()
     with pool.worker(integration_options) as worker:
         yield worker
-
-
-def _extract_mask(integration_options: dict) -> Optional[numpy.ndarray]:
-    """Integration options related to the mask:
-
-    * mask_file: URL or None
-    * do_mask: use mask_file or not
-    * mask: URL, array or None (overwrites mask_file and do_mask when not None)
-    """
-    mask = integration_options.pop("mask", None)
-    mask_file = integration_options.get("mask_file", None)
-    do_mask = integration_options.get("do_mask", None)
-    if not do_mask:
-        mask_file = None
-    if isinstance(mask, str):
-        mask_file = mask
-        mask = None
-        do_mask = True
-    integration_options["mask_file"] = mask_file
-    integration_options["do_mask"] = do_mask
-    return mask
```

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/conftest.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_ascii.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_ascii.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_background.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_background.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_batch_integrate.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_batch_integrate.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,19 +40,27 @@
         inputs["integration_options"] = {
             "error_model": "azimuthal",
             "method": "no_csr_cython",
             "integrator_name": "sigma_clip_ng",
             "extra_options": {"max_iter": 3, "thres": 0},
         }
 
-    execute_task(
+    outputs = execute_task(
         OWIntegrateBlissScan.ewokstaskclass if qtapp is None else OWIntegrateBlissScan,
         inputs=inputs,
     )
 
+    if external:
+        expected = {
+            "nxdata_url": f"{external_output_filename}::/2.1/p3_integrate/integrated"
+        }
+    else:
+        expected = {"nxdata_url": f"{output_filename}::/2.1/p3_integrate/integrated"}
+    assert outputs == expected
+
     with h5py.File(output_filename) as root:
         data = root["2.1/measurement/p3_integrated"][()]
         if ndims == 2:
             axes = ["points", "azimuth", "2th"]
         else:
             axes = ["points", "2th"]
         assert root["2.1/p3_integrate/integrated"].attrs["axes"].tolist() == axes
```

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_bliss_integrate_no_save.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_calibrate.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_calibrate.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_calint_workflow.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_calint_workflow.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_integrate.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_integrate.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_mask.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_mask.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_nexus.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_nexus_integrated.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_nexus_integrated.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_pyfai_utils.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_pyfai_utils.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_save_images.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_save_images.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/test_sum.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tests/test_sum.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd/tests/xrpd_theory.py` & `ewoksxrpd-0.5.0/src/ewoksxrpd/tests/xrpd_theory.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/PKG-INFO` & `ewoksxrpd-0.5.0/src/ewoksxrpd.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ewoksxrpd
-Version: 0.4.0
+Version: 0.5.0
 Summary: Data processing workflows for SAXS/WAXS
 Home-page: https://gitlab.esrf.fr/workflow/ewoksxrpd/
 Author: ESRF
 Author-email: wout.de_nolf@esrf.fr
 License: MIT
 Project-URL: Source, https://gitlab.esrf.fr/workflow/ewoksxrpd/
 Project-URL: Documentation, https://ewoksxrpd.readthedocs.io/
 Project-URL: Tracker, https://gitlab.esrf.fr/workflow/ewoksxrpd/issues/
 Keywords: orange3 add-on,ewoks
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: online
 Provides-Extra: test
 Provides-Extra: dev
 Provides-Extra: doc
 License-File: LICENSE.md
 
 # ewoksxrpd
```

### Comparing `ewoksxrpd-0.4.0/src/ewoksxrpd.egg-info/SOURCES.txt` & `ewoksxrpd-0.5.0/src/ewoksxrpd.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
 src/ewoksxrpd/tests/conftest.py
 src/ewoksxrpd/tests/test_ascii.py
 src/ewoksxrpd/tests/test_background.py
 src/ewoksxrpd/tests/test_batch_integrate.py
 src/ewoksxrpd/tests/test_bliss_integrate_no_save.py
 src/ewoksxrpd/tests/test_calibrate.py
 src/ewoksxrpd/tests/test_calint_workflow.py
+src/ewoksxrpd/tests/test_darkflat.py
 src/ewoksxrpd/tests/test_integrate.py
 src/ewoksxrpd/tests/test_mask.py
 src/ewoksxrpd/tests/test_nexus.py
 src/ewoksxrpd/tests/test_nexus_integrated.py
 src/ewoksxrpd/tests/test_pyfai_utils.py
 src/ewoksxrpd/tests/test_save_images.py
 src/ewoksxrpd/tests/test_sum.py
```

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/__init__.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/__init__.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/ascii.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/ascii.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/background.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/background.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/batchintegrate.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/batchintegrate.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/blissintegratenosave.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/calculategeometry.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/calculategeometry.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/calibratemulti.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/calibratemulti.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/calibratesingle.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/calibratesingle.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/diagnose_integrate1d.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/diagnose_multicalib.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/diagnose_singlecalib.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/icons/category.png` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/icons/category.png`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/icons/widget.png` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/icons/widget.png`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/integrate1d.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/integrate1d.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/mask.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/mask.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/nexus.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/nexus.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/nexus_integrated.py`

 * *Files identical despite different names*

### Comparing `ewoksxrpd-0.4.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py` & `ewoksxrpd-0.5.0/src/orangecontrib/ewoksxrpd/pyfaiconfig.py`

 * *Files identical despite different names*

