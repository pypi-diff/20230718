# Comparing `tmp/pyote-5.3.3.tar.gz` & `tmp/pyote-5.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyote-5.3.3.tar", last modified: Mon Jul 17 17:41:02 2023, max compression
+gzip compressed data, was "pyote-5.3.4.tar", last modified: Tue Jul 18 18:20:08 2023, max compression
```

## Comparing `pyote-5.3.3.tar` & `pyote-5.3.4.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 17:41:02.651254 pyote-5.3.3/
--rw-rw-rw-   0        0        0     1072 2017-06-14 17:12:14.000000 pyote-5.3.3/LICENSE
--rw-rw-rw-   0        0        0      194 2023-01-09 22:51:18.000000 pyote-5.3.3/MANIFEST.in
--rw-rw-rw-   0        0        0     1190 2023-07-17 17:41:02.651254 pyote-5.3.3/PKG-INFO
--rw-rw-rw-   0        0        0      285 2017-06-17 03:33:59.000000 pyote-5.3.3/README.rst
--rw-rw-rw-   0        0        0       80 2023-07-17 17:41:02.652254 pyote-5.3.3/setup.cfg
--rw-rw-rw-   0        0        0     2922 2023-06-06 20:30:01.000000 pyote-5.3.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-17 17:41:02.455457 pyote-5.3.3/src/
-drwxrwxrwx   0        0        0        0 2023-07-17 17:41:02.471068 pyote-5.3.3/src/pyote.egg-info/
--rw-rw-rw-   0        0        0     1190 2023-07-17 17:41:02.000000 pyote-5.3.3/src/pyote.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1789 2023-07-17 17:41:02.000000 pyote-5.3.3/src/pyote.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 17:41:02.000000 pyote-5.3.3/src/pyote.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2017-06-17 17:07:51.000000 pyote-5.3.3/src/pyote.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      257 2023-07-17 17:41:02.000000 pyote-5.3.3/src/pyote.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-07-17 17:41:02.000000 pyote-5.3.3/src/pyote.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-07-17 17:41:02.605894 pyote-5.3.3/src/pyoteapp/
--rwxrwxrwx   0        0        0      345 2018-11-28 18:46:03.000000 pyote-5.3.3/src/pyoteapp/PYOTE.bat
--rw-rw-rw-   0        0        0     5930 2023-03-27 21:30:02.000000 pyote-5.3.3/src/pyoteapp/SER.py
--rw-rw-rw-   0        0        0        0 2017-06-16 00:35:17.000000 pyote-5.3.3/src/pyoteapp/__init__.py
--rw-rw-rw-   0        0        0     5044 2020-01-10 23:40:03.000000 pyote-5.3.3/src/pyoteapp/autocorrtools.py
--rw-rw-rw-   0        0        0     1251 2020-01-29 05:31:51.000000 pyote-5.3.3/src/pyoteapp/blockIntegrateUtils.py
--rw-rw-rw-   0        0        0     2687 2023-01-10 05:23:59.000000 pyote-5.3.3/src/pyoteapp/checkForNewerVersion.py
--rw-rw-rw-   0        0        0    12525 2023-06-30 14:42:34.000000 pyote-5.3.3/src/pyoteapp/csvreader.py
--rw-rw-rw-   0        0        0    48292 2020-02-09 15:46:46.000000 pyote-5.3.3/src/pyoteapp/diffraction-table.p
--rw-rw-rw-   0        0        0     7549 2022-03-09 14:54:19.000000 pyote-5.3.3/src/pyoteapp/errorBarUtils.py
--rw-rw-rw-   0        0        0     8127 2020-02-15 22:41:06.000000 pyote-5.3.3/src/pyoteapp/example-penumbral.csv
--rw-rw-rw-   0        0        0     3701 2022-01-29 16:31:21.000000 pyote-5.3.3/src/pyoteapp/exponentialEdgeUtilities.py
--rw-rw-rw-   0        0        0     6835 2023-07-16 03:05:04.000000 pyote-5.3.3/src/pyoteapp/false_positive.py
--rw-rw-rw-   0        0        0     1426 2017-06-14 19:28:56.000000 pyote-5.3.3/src/pyoteapp/fixedPrecision.py
--rw-rw-rw-   0        0        0     9761 2022-08-28 02:47:10.000000 pyote-5.3.3/src/pyoteapp/genDiffraction.py
--rw-rw-rw-   0        0        0   386870 2023-07-10 15:37:00.000000 pyote-5.3.3/src/pyoteapp/gui.py
--rw-rw-rw-   0        0        0     1907 2023-06-17 17:37:29.000000 pyote-5.3.3/src/pyoteapp/helpDialog.py
--rw-rw-rw-   0        0        0    25723 2023-07-07 20:15:46.000000 pyote-5.3.3/src/pyoteapp/iterative_logl_functions.py
--rw-rw-rw-   0        0        0     5508 2023-04-09 14:19:52.000000 pyote-5.3.3/src/pyoteapp/likelihood_calculations.py
-drwxrwxrwx   0        0        0        0 2023-07-17 17:41:02.650254 pyote-5.3.3/src/pyoteapp/model-examples/
--rw-rw-rw-   0        0        0     1209 2023-05-29 17:45:05.000000 pyote-5.3.3/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p
--rw-rw-rw-   0        0        0     1204 2023-05-29 18:25:21.000000 pyote-5.3.3/src/pyoteapp/model-examples/LCP_penumbral.p
--rw-rw-rw-   0        0        0    15259 2022-12-25 19:15:36.000000 pyote-5.3.3/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0    15274 2022-12-25 19:15:25.000000 pyote-5.3.3/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0    10519 2022-12-25 19:15:13.000000 pyote-5.3.3/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0     6640 2022-12-25 19:15:12.000000 pyote-5.3.3/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv
--rw-rw-rw-   0        0        0    27881 2022-12-25 19:15:10.000000 pyote-5.3.3/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0   130669 2023-01-08 14:07:02.000000 pyote-5.3.3/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv
--rw-rw-rw-   0        0        0   882048 2023-01-03 23:22:32.000000 pyote-5.3.3/src/pyoteapp/model-help.pdf
--rw-rw-rw-   0        0        0     1926 2023-05-11 18:15:42.000000 pyote-5.3.3/src/pyoteapp/noiseUtils.py
--rw-rw-rw-   0        0        0   459673 2023-07-17 17:39:18.000000 pyote-5.3.3/src/pyoteapp/pyote-info.pdf
--rw-rw-rw-   0        0        0   449791 2023-07-17 17:31:01.000000 pyote-5.3.3/src/pyoteapp/pyote.py
--rw-rw-rw-   0        0        0    79636 2023-06-17 20:42:15.000000 pyote-5.3.3/src/pyoteapp/pyote_modelling_utility_functions.py
--rwxrwxrwx   0        0        0      321 2018-12-06 17:53:09.000000 pyote-5.3.3/src/pyoteapp/run-pyote-mac.bat
--rw-rw-rw-   0        0        0     6084 2020-04-07 15:06:10.000000 pyote-5.3.3/src/pyoteapp/showVideoFrames.py
--rw-rw-rw-   0        0        0    23501 2023-07-07 02:06:56.000000 pyote-5.3.3/src/pyoteapp/solverUtils.py
--rw-rw-rw-   0        0        0    21983 2022-12-27 20:16:10.000000 pyote-5.3.3/src/pyoteapp/subframe_timing_utilities.py
--rw-rw-rw-   0        0        0    13719 2019-02-01 18:32:12.000000 pyote-5.3.3/src/pyoteapp/timestampDialog.py
--rw-rw-rw-   0        0        0    14937 2023-04-29 22:36:35.000000 pyote-5.3.3/src/pyoteapp/timestampUtils.py
--rw-rw-rw-   0        0        0       34 2023-07-17 17:37:34.000000 pyote-5.3.3/src/pyoteapp/version.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:20:08.025495 pyote-5.3.4/
+-rw-rw-rw-   0        0        0     1072 2017-06-14 17:12:14.000000 pyote-5.3.4/LICENSE
+-rw-rw-rw-   0        0        0      194 2023-01-09 22:51:18.000000 pyote-5.3.4/MANIFEST.in
+-rw-rw-rw-   0        0        0     1190 2023-07-18 18:20:08.025495 pyote-5.3.4/PKG-INFO
+-rw-rw-rw-   0        0        0      285 2017-06-17 03:33:59.000000 pyote-5.3.4/README.rst
+-rw-rw-rw-   0        0        0       81 2023-07-18 18:20:08.025495 pyote-5.3.4/setup.cfg
+-rw-rw-rw-   0        0        0     2931 2023-07-18 02:09:20.000000 pyote-5.3.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:19:17.026797 pyote-5.3.4/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 18:20:08.009863 pyote-5.3.4/src/pyote.egg-info/
+-rw-rw-rw-   0        0        0     1190 2023-07-18 18:20:07.000000 pyote-5.3.4/src/pyote.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1789 2023-07-18 18:20:07.000000 pyote-5.3.4/src/pyote.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 18:20:07.000000 pyote-5.3.4/src/pyote.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        1 2017-06-17 17:07:51.000000 pyote-5.3.4/src/pyote.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      257 2023-07-18 18:20:07.000000 pyote-5.3.4/src/pyote.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-07-18 18:20:07.000000 pyote-5.3.4/src/pyote.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 18:20:08.025495 pyote-5.3.4/src/pyoteapp/
+-rwxrwxrwx   0        0        0      345 2018-11-28 18:46:03.000000 pyote-5.3.4/src/pyoteapp/PYOTE.bat
+-rw-rw-rw-   0        0        0     5930 2023-03-27 21:30:02.000000 pyote-5.3.4/src/pyoteapp/SER.py
+-rw-rw-rw-   0        0        0        0 2017-06-16 00:35:17.000000 pyote-5.3.4/src/pyoteapp/__init__.py
+-rw-rw-rw-   0        0        0     5044 2020-01-10 23:40:03.000000 pyote-5.3.4/src/pyoteapp/autocorrtools.py
+-rw-rw-rw-   0        0        0     1251 2020-01-29 05:31:51.000000 pyote-5.3.4/src/pyoteapp/blockIntegrateUtils.py
+-rw-rw-rw-   0        0        0     2687 2023-01-10 05:23:59.000000 pyote-5.3.4/src/pyoteapp/checkForNewerVersion.py
+-rw-rw-rw-   0        0        0    12525 2023-06-30 14:42:34.000000 pyote-5.3.4/src/pyoteapp/csvreader.py
+-rw-rw-rw-   0        0        0    48292 2020-02-09 15:46:46.000000 pyote-5.3.4/src/pyoteapp/diffraction-table.p
+-rw-rw-rw-   0        0        0     7549 2022-03-09 14:54:19.000000 pyote-5.3.4/src/pyoteapp/errorBarUtils.py
+-rw-rw-rw-   0        0        0     8127 2020-02-15 22:41:06.000000 pyote-5.3.4/src/pyoteapp/example-penumbral.csv
+-rw-rw-rw-   0        0        0     3701 2022-01-29 16:31:21.000000 pyote-5.3.4/src/pyoteapp/exponentialEdgeUtilities.py
+-rw-rw-rw-   0        0        0     6835 2023-07-16 03:05:04.000000 pyote-5.3.4/src/pyoteapp/false_positive.py
+-rw-rw-rw-   0        0        0     1426 2017-06-14 19:28:56.000000 pyote-5.3.4/src/pyoteapp/fixedPrecision.py
+-rw-rw-rw-   0        0        0     9761 2022-08-28 02:47:10.000000 pyote-5.3.4/src/pyoteapp/genDiffraction.py
+-rw-rw-rw-   0        0        0   386870 2023-07-10 15:37:00.000000 pyote-5.3.4/src/pyoteapp/gui.py
+-rw-rw-rw-   0        0        0     1907 2023-06-17 17:37:29.000000 pyote-5.3.4/src/pyoteapp/helpDialog.py
+-rw-rw-rw-   0        0        0    25723 2023-07-07 20:15:46.000000 pyote-5.3.4/src/pyoteapp/iterative_logl_functions.py
+-rw-rw-rw-   0        0        0     5508 2023-04-09 14:19:52.000000 pyote-5.3.4/src/pyoteapp/likelihood_calculations.py
+drwxrwxrwx   0        0        0        0 2023-07-18 18:20:08.025495 pyote-5.3.4/src/pyoteapp/model-examples/
+-rw-rw-rw-   0        0        0     1209 2023-05-29 17:45:05.000000 pyote-5.3.4/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p
+-rw-rw-rw-   0        0        0     1204 2023-05-29 18:25:21.000000 pyote-5.3.4/src/pyoteapp/model-examples/LCP_penumbral.p
+-rw-rw-rw-   0        0        0    15259 2022-12-25 19:15:36.000000 pyote-5.3.4/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0    15274 2022-12-25 19:15:25.000000 pyote-5.3.4/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0    10519 2022-12-25 19:15:13.000000 pyote-5.3.4/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0     6640 2022-12-25 19:15:12.000000 pyote-5.3.4/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv
+-rw-rw-rw-   0        0        0    27881 2022-12-25 19:15:10.000000 pyote-5.3.4/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0   130669 2023-01-08 14:07:02.000000 pyote-5.3.4/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv
+-rw-rw-rw-   0        0        0   882048 2023-01-03 23:22:32.000000 pyote-5.3.4/src/pyoteapp/model-help.pdf
+-rw-rw-rw-   0        0        0     1926 2023-05-11 18:15:42.000000 pyote-5.3.4/src/pyoteapp/noiseUtils.py
+-rw-rw-rw-   0        0        0   461059 2023-07-18 18:15:27.000000 pyote-5.3.4/src/pyoteapp/pyote-info.pdf
+-rw-rw-rw-   0        0        0   451841 2023-07-18 18:10:03.000000 pyote-5.3.4/src/pyoteapp/pyote.py
+-rw-rw-rw-   0        0        0    79636 2023-06-17 20:42:15.000000 pyote-5.3.4/src/pyoteapp/pyote_modelling_utility_functions.py
+-rwxrwxrwx   0        0        0      321 2018-12-06 17:53:09.000000 pyote-5.3.4/src/pyoteapp/run-pyote-mac.bat
+-rw-rw-rw-   0        0        0     6084 2020-04-07 15:06:10.000000 pyote-5.3.4/src/pyoteapp/showVideoFrames.py
+-rw-rw-rw-   0        0        0    23501 2023-07-07 02:06:56.000000 pyote-5.3.4/src/pyoteapp/solverUtils.py
+-rw-rw-rw-   0        0        0    21983 2022-12-27 20:16:10.000000 pyote-5.3.4/src/pyoteapp/subframe_timing_utilities.py
+-rw-rw-rw-   0        0        0    13719 2019-02-01 18:32:12.000000 pyote-5.3.4/src/pyoteapp/timestampDialog.py
+-rw-rw-rw-   0        0        0    14937 2023-04-29 22:36:35.000000 pyote-5.3.4/src/pyoteapp/timestampUtils.py
+-rw-rw-rw-   0        0        0       34 2023-07-18 18:12:15.000000 pyote-5.3.4/src/pyoteapp/version.py
```

### Comparing `pyote-5.3.3/LICENSE` & `pyote-5.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/PKG-INFO` & `pyote-5.3.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyote
-Version: 5.3.3
+Version: 5.3.4
 Summary: pyote is a simplified subset of R-OTE
 Home-page: https://github.com/bob-anderson-ok/py-ote
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pyote-5.3.3/setup.py` & `pyote-5.3.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,12 +70,12 @@
         maintainer='Bob Anderson',
         maintainer_email='bob.anderson.ok@gmail.com',
         keywords=KEYWORDS,
         long_description=read("README.rst"),
         packages=PACKAGES,
         package_dir={"": "src"},
         zip_safe=False,
-        package_data={'': ['*.bat']},
+        package_data={'': ['*.bat','*.xlsx']},
         include_package_data=True,
         classifiers=CLASSIFIERS,
         install_requires=INSTALL_REQUIRES,
     )
```

### Comparing `pyote-5.3.3/src/pyote.egg-info/PKG-INFO` & `pyote-5.3.4/src/pyote.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyote
-Version: 5.3.3
+Version: 5.3.4
 Summary: pyote is a simplified subset of R-OTE
 Home-page: https://github.com/bob-anderson-ok/py-ote
 Author: Bob Anderson
 Author-email: bob.anderson.ok@gmail.com
 Maintainer: Bob Anderson
 Maintainer-email: bob.anderson.ok@gmail.com
 License: License :: OSI Approved :: MIT License
```

### Comparing `pyote-5.3.3/src/pyote.egg-info/SOURCES.txt` & `pyote-5.3.4/src/pyote.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/SER.py` & `pyote-5.3.4/src/pyoteapp/SER.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/autocorrtools.py` & `pyote-5.3.4/src/pyoteapp/autocorrtools.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/blockIntegrateUtils.py` & `pyote-5.3.4/src/pyoteapp/blockIntegrateUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/checkForNewerVersion.py` & `pyote-5.3.4/src/pyoteapp/checkForNewerVersion.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/csvreader.py` & `pyote-5.3.4/src/pyoteapp/csvreader.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/diffraction-table.p` & `pyote-5.3.4/src/pyoteapp/diffraction-table.p`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/errorBarUtils.py` & `pyote-5.3.4/src/pyoteapp/errorBarUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/example-penumbral.csv` & `pyote-5.3.4/src/pyoteapp/example-penumbral.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/exponentialEdgeUtilities.py` & `pyote-5.3.4/src/pyoteapp/exponentialEdgeUtilities.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/false_positive.py` & `pyote-5.3.4/src/pyoteapp/false_positive.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/fixedPrecision.py` & `pyote-5.3.4/src/pyoteapp/fixedPrecision.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/genDiffraction.py` & `pyote-5.3.4/src/pyoteapp/genDiffraction.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/gui.py` & `pyote-5.3.4/src/pyoteapp/gui.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/helpDialog.py` & `pyote-5.3.4/src/pyoteapp/helpDialog.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/iterative_logl_functions.py` & `pyote-5.3.4/src/pyoteapp/iterative_logl_functions.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/likelihood_calculations.py` & `pyote-5.3.4/src/pyoteapp/likelihood_calculations.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p` & `pyote-5.3.4/src/pyoteapp/model-examples/LCP_high-rho-diffraction.p`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/model-examples/LCP_penumbral.p` & `pyote-5.3.4/src/pyoteapp/model-examples/LCP_penumbral.p`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.3.4/src/pyoteapp/model-examples/diffraction_miss_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.3.4/src/pyoteapp/model-examples/diffraction_with_central_spot_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv` & `pyote-5.3.4/src/pyoteapp/model-examples/disk_on_disk_annular_shotnoise_1.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv` & `pyote-5.3.4/src/pyoteapp/model-examples/edge_on_disk_miss_shotnoise_0.0_readnoise_10.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv` & `pyote-5.3.4/src/pyoteapp/model-examples/edge_on_disk_standard_penumbral_D55_R35_shotnoise_2.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv` & `pyote-5.3.4/src/pyoteapp/model-examples/high-rho-diffraction_shotnoise_2.0_readnoise_20.0.csv`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/model-help.pdf` & `pyote-5.3.4/src/pyoteapp/model-help.pdf`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/noiseUtils.py` & `pyote-5.3.4/src/pyoteapp/noiseUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/pyote-info.pdf` & `pyote-5.3.4/src/pyoteapp/pyote-info.pdf`

 * *Installing the 'pypdf' Python module from the 'python3-pypdf' package may produce a better output.*

 * *Files 4% similar despite different names*

#### pdftotext {} -

```diff
@@ -1,8 +1,12 @@
 Version history (PyOTE description – out of date - is at end)
+Version 5.3.4
+18 July 2023
+• Adds formatting to the .xlsx fit metrics file and provides a default name of the enclosing
+folder
 Version 5.3.3
 17 July 2023
 • Fixes a bug in the fit-metric.txt file duration calculation
 Version 5.3.2
 15 July 2023
 • Fixes a bug in the calculation of the duration fit metric when an already integrated csv
 file is in use.
@@ -36,19 +40,19 @@
 • Added detection of duplicate column names (only possible in a csv file from PyMovie).
 Duplicate names cause the column data to be concatenated and this cannot be
 tolerated, so when this error is found, the data import is aborted.
 The user will need to edit the csv file to resolve the name duplication.
 •
 
 Added a warning message that will only appear if a user manually calculates baseline
-statistics and then does a find event. Sometimes that is exactly what is wanted, but
+
+statistics and then does a find event. Sometimes that is exactly what is wanted, but
 those statistics become fixed and will be used for all subsequent find event clicks.
 That would be very wrong if the user is stepping through multiple light-curves in search
-
-of the “best” as they would all use the same baseline numbers (B and sigmaB).
+of the “best” as they would all use the same baseline numbers (B and sigmaB).
 •
 
 Added false-positive metric to fit-metrics and rearranged output order.
 
 Version 5.2.7
 24 June 2023
 • Minor change: corrected titles in fit-metric file from D frame to D reading num and R
@@ -99,26 +103,20 @@
 • Restores the calculation of timeDelta to 6 digit precision (it had been inadvertently
 limited to 4 digits by a previous change)
 •
 
 Fixes a bug in the calculation of flash edge times that was discovered when very high
 SNR recording was attempted
 
-Version 5.2.2
+Version 5.2.2
 13 April 2023
 • Adds diffraction modelling of an elliptical asteroid shape
-Version 5.2.1
-
-27 March 2023
-
-•
-
-Fixed problem with VizieR loading from North American .xlsx caused by Occult
+Version 5.2.1 27 March 2023
+• Fixed problem with VizieR loading from North American .xlsx caused by Occult
 sometimes putting a string in the asteroid field and sometimes an integer.
-
 •
 
 SER files with colorCode other than mono are now accepted.
 
 Version 5.2.0 17 March 2023
 • Fixes a bug in code introduced in version 5.1.0 where dropped frames are detected –
 that code did not handle an observation that passed through midnight (23:59:59)
@@ -153,20 +151,20 @@
 
 Version 5.1.0 7 February 2023
 • Changed the way data sets (lightcurves) read from a PyMovie csv file are selected for
 viewing. Whereas previously it was possible to specify a ‘prefix’ to be used when
 reading PyMovie csv files (such as ‘signal’ or ‘appsum’), it was not possible to mix-andmatch data sets with different prefixes. With this version, that now becomes possible.
 With this feature, it now becomes possible to demonstrate for yourself that there is no
 reason to process a target lightcurve in ‘aperture sum’ mode (no background
-subtraction) versus the regular ‘signal’ mode (where background subtraction is
+
+subtraction) versus the regular ‘signal’ mode (where background subtraction is
 performed). Simply display the ‘signal’ and ‘appsum’ versions of a target lightcurve and
 use the y position spinBox on one of the curves until they overlap. This should show
 that during the event, the points almost exactly overlap, so event timing will be the
-
-same.
+same.
 •
 
 Added a button to the VizieR tab that will fill most of the entry boxes in the VizieR form
 from a North American .xlsx file for that event (derived from OW/Occult 4), if one is
 available.
 
 Version 5.0.8 1 February 2023
@@ -204,19 +202,22 @@
 log file.
 •
 
 Made D and R edge time calculations work properly even when there are dropped
 readings in the observation
 
 Version 5.0.0 6 January 2023
-• Added ability to specify a block size to be used during automatic block integration.
+
+•
+
+Added ability to specify a block size to be used during automatic block integration.
 When a block size is entered, the program will determine the best offset value to use
 for the integration.
 
-•
+•
 
 Added a comprehensive set of lightcurve models together with tools to help automate
 the fitting of the new models to observation data. Models included:
 o Diffraction (including central spot for low rho events) using physical optics
 o Disk on disk (geometrical optics) for large stars
 o Edge on disk (geometrical optics) for large stars and limb angles on asteroid
 
@@ -245,19 +246,19 @@
 attention.
 Version 4.8.8 7 August 2022
 • Added message at normal program close to the effect that QBasicTimer messages
 that appear after the program has closed are harmless artifacts of the order in which
 QUI elements are closed.
 Version 4.8.7 29 July 2022
 • changed numpy version requirement to match that of PyMovie so that ultimately the
-two programs can share a virtual environment, thus saving much space.
+
+two programs can share a virtual environment, thus saving much space.
 Version 4.8.6 23 July 2022
 • added instructions telling the user how to install a new version when one is found.
-
-There are instructions for pip based installations and pipenv installations
+There are instructions for pip based installations and pipenv installations
 Version 4.8.4
 • there are no changes. This is a new version just to test the change introduced in 4.8.3
 about version detection and handling thereof.
 Version 4.8.3
 • this version removes the offer to update to a newer version when one is found. This
 has been done primarily to allow an easy transition to a distribution method that does
 not require the installation of Anaconda3, but it also gives the user more control. When
@@ -289,20 +290,21 @@
 installed Win11 on i5 processor-based computer. On those machines, finding an event
 using min/max would always hang at 99% completion. Allowing the original Python
 code to be used instead of compiling to C-code resolved that issue. As finding an event
 using min/max size minimizes the number of candidate solutions naturally, the loss of
 speed is not so important – it’s fast enough.
 version 4.6.4
 • made the 'camera response' checkbox (in the Settings/misc tab) sticky
-•
+
+•
 
 corrected the log messaging about Donly, Ronly, DandR, and min/max directions to the
 solver consistent
 
-version 4.6.3
+version 4.6.3
 • in detectability: logged new 'drop message' to the detectability.log
 version 4.6.2
 • in detectability: when event duration is or becomes less than the camera exposure
 time, the observed drop is reduced proportionately
 version 4.6.1
 • in detectability: changed calculation of number of event points from
 ceiling(dur/rdgTime) to round(dur/rdgTime)
@@ -332,19 +334,19 @@
 • cleans up the the first bin of the False-Positive histogram
 version 4.5.3
 • adds an option to validate a single point event to the Analysis tab. It uses the falsepositive test procedure to determine if the selected point had a non-zero chance to
 have been caused by baseline noise alone.
 version 4.5.2
 • fixes a bug where transition points (only present in high SNR light-curves) were not
 properly ignored during calculation of event noise. This manifested itself most clearly in
-too large error bars for magDrop
+
+too large error bars for magDrop
 version 4.5.0
 • fixes a bug introduced with the NE3 code changes that inhibited sub-frame timing
-
-adjustments.
+adjustments.
 version 4.4.9
 • fixed yet another manisfestation of the bug introduced in version 4.2.1
 version 4.4.8
 • fixed another manifestation of the bug introduced in version 4.2.1
 version 4.4.7
 • fixes a bug introduced in version 4.2.1 (February 8, 2022) that caused D values to be
 calculated as occurring 1 reading early
@@ -372,19 +374,19 @@
 to smooth the reference curve used for normalization. It is printed in green whenever
 normalization is active. It is simply the standard deviation of the normalized target
 lightcurve. Although it is quite simple, it is a value that is minimized the more level and
 the less bumpy the normalized target curve is.
 When normalization is active, at each change, a pair of metrics are printed in the log
 panel.
 The red metric is the Pearson R value of the correlation between the target lightcurve
-and the reference lightcurve; it should be maximized (using the X offset spinbox of the
+
+and the reference lightcurve; it should be maximized (using the X offset spinbox of the
 reference curve) at the point where the two curves are properly time-aligned. It is also
 affected by the smoothing interval, but this connection should be ignored.
-
-The green metric is the standard deviation of the target lightcurve – it is lowered when
+The green metric is the standard deviation of the target lightcurve – it is lowered when
 the target lightcurve has a minimum slope and the fewest and shallowest bumps. Use
 the spinbox for the number of readings in the smoothing interval to minimize this
 number.
 version 4.3.5
 • made the 'step-by' buttons radio buttons so that it is clear what the current step size is.
 •
 
@@ -419,19 +421,18 @@
 
 version 4.2.8
 • fixes 'trim problem'
 •
 
 adds 'step by' buttons that change the smoothing interval spinbox step size.
 
-version 4.2.6
+version 4.2.6
 • tidies up the lightcurve panel a bit and changes color samples for target and reference
 curves.
-
-version 4.2.5
+version 4.2.5
 • completes implementation of the time shift (left/right shift) of the reference curve for
 normalization.
 •
 
 adds dot color samples next to the lightcurve titles.
 
 version 4.2.4
@@ -471,18 +472,18 @@
 Unless a lightcurve is designated as a target (curve to be analyzed for an event) or is
 designated as a reference lightcurve, its dot color depends on the row it is in - every
 row has a unique color other than blue or green.
 Lightcurves can be displaced up or down using the Y offset spinner to control the
 displacement. This affects the display position only; the underlying values are not
 affected. This facility was added to allow the separation of lightcurves that would
 otherwise overlap in a confusing manner.
-There can only be one lightcurve selected as target.
-There can be either 0 or 1 lightcurve selected as a reference for normalization.
 
-Normalization is applied whenever the normalization reference curve smoothing
+There can only be one lightcurve selected as target.
+There can be either 0 or 1 lightcurve selected as a reference for normalization.
+Normalization is applied whenever the normalization reference curve smoothing
 interval spinbox is changed from 0. Whenever this number is changed, a new
 normalization will result. If this number is returned to zero, all normalization is removed
 and the original values restored.
 The X offset spinbox is not yet implemented. Its (future) purpose is to allow the
 reference curve used for normalization to be 'time shifted' for those cases where a
 drifting cloud affects lightcurves at slightly different times.
 •
@@ -523,18 +524,17 @@
 version 4.1.6
 • reenables Cholesky failure messages (disabled for testing)
 •
 
 Adds test to detectability routine so that the user cannot give an event duration that
 requires more points than are available in the observation.
 
-version 4.1.5
+version 4.1.5
 • changed error bar calculation reporting so that the the value reported in the
-
-containment interval report matches that reported in the Excel final report when there is
+containment interval report matches that reported in the Excel final report when there is
 no asymmetry present.
 version 4.1.4
 • This version adds tools needed to make best use of the Night Eagle 3 camera, the
 successor to the Night Eagle Astro camera (which is no longer in production). They are
 all grouped on a new tab page titled Night Eagle 3.
 •
 
@@ -586,22 +586,22 @@
 •
 
 When the exponential curve fit algorithm is in use, the light-curve plot PyOTE displays
 will be changed. Gone is the blue 'camera response' curve, replaced by brown dotted
 'theoretical' exponential edge curves that you can use to judge for yourself the
 goodness of a 'fit'.
 
-•
+•
 
 You will probably want to use the most aggressive noise reduction in most cases, but
 make sure that your expected event duration is long enough that the D transition
 exponential curve has time to settle to the bottom event plus some time to allow a good
-
-determination of the event bottom intensity. At DNR:HIGH, your expected event time
+determination of the event bottom intensity. At DNR:HIGH, your expected event time
 should be greater than 30 frames (1 second) to use this setting.
+
 •
 
 I suggest the following rules-of-thumb: can use DNR:HIGH for events 2 seconds and
 longer; can use DNR:MIDDLE for events 1 second and longer; can use DNR:LOW for
 events 0.5 seconds and longer.
 
 version 4.1.2
@@ -628,19 +628,19 @@
 Some others are available: avgbkd (shows the average pixel value in the aperture);
 stdbkg (shows the pixel noise in the background pixels in the aperture); nmaskpx
 (which shows the nuber of pixels in the sampling mask – there are times when this
 curve can be used to extrat event times).
 Note: this only applies to csv files generated by PyMovie.
 version 4.0.6
 • minor GUI changes
-version 4.0.5
+
+version 4.0.5
 • if you click outside the light-curve, the closest point will be toggled (so you don't have
 to zoom in to select the leftmost or rightmost point in a light-curve.
-
-•
+•
 
 When baseline statistics are calculated, they are reported as baseline mean and
 baseline snr (instead of just snr, which is the term we use when a drop is present).
 
 version 4.0.4
 • a few GUI changes
 •
@@ -677,18 +677,18 @@
 • detectibility graphics plots are now being being put in their own folder. The root folder is
 that of the directory where the light-curve came from. The plots will be found in
 lightCurveDirectory\DetectibilityPlots\
 In addition, if you supply a duration step size, which is the way to ask the detectibilty
 calculator to step from the given duration down until an event of that duration fails the
 False-positive test, only the final plot (where False-positive became non-zero) will be
 plotted.
-All of the above is just to cut down on clutter in the light-curve directory and to only plot
-meaningful graphics generated during the minimum duration search.
 
-version 3.9.9
+All of the above is just to cut down on clutter in the light-curve directory and to only plot
+meaningful graphics generated during the minimum duration search.
+version 3.9.9
 • whew! 3.9.8 did solve the sizing issue. So it is safe to get back in the water so...
 This version just improves the right-click context help for buttons in the new
 Detectibility calculator.
 version 3.9.8
 • one more attempt to solve the gui sizing issue.
 •
 
@@ -715,18 +715,18 @@
 version 3.9.5
 • adds automation to the 'detectibility' calculator. If a duration step size is entered, a
 series of 'detectibility' calculations will be made at decreasing durations until the falsepositive probability becomes non-zero. A unique .png (incorporates duration and
 magDrop in the file name) will be written to the directory of the light-curve and the final
 plot where detection failed will be left on-screen.
 If the duration step size is left unfilled or is zero, a single 'detectibility' calculation will be
 made as before.
-version 3.9.4
-• attempts to fix over-size initial gui.
 
-version 3.9.3
+version 3.9.4
+• attempts to fix over-size initial gui.
+version 3.9.3
 • makes various improvements to the 'detectability' calculator to make it easier to use.
 version 3.9.2
 • adds a 'detectability' calculator for use in pre-planning event observation.
 •
 
 'scrunched' the left panel buttons together to make more room for the user to move the
 horizontal splitter up (which gives more room to view the lower right panel where the
@@ -755,19 +755,19 @@
 version 3.8.6
 • checks for only a single light-curve in the csv file which was causing a 'list index out of
 range' error message
 version 3.8.5
 • changed the way QGridLayout was referenced.
 version 3.8.4
 • changed the way QTableWidgetItem and QApplication were referenced to
-accommodate the latest Anaconda version, which has reorganized where those
+
+accommodate the latest Anaconda version, which has reorganized where those
 modules are stored. A similar change was made in version 3.7.6 and I do not know
 how this has gone uncorrected for so long – I hope that I have not missed something.
-
-version 3.8.3
+version 3.8.3
 • adds display of light-curve name (if available in the csv file) to the curve-to-be-analyzed
 and the normalization curve next to their selection spinners.
 version 3.8.2
 • 3.7.5 introduced a scrollable GUI for small screens. Unfortunately, that caused resizing
 problem for all users. The version reverts back to the original GUI design.
 •
 
@@ -797,18 +797,18 @@
 associate timestamp with point).
 version 3.7.7
 • if timestamps are available in the csv file, they are used as x axis labels in the main
 plot.
 version 3.7.6
 • changed the way QMainWindow and Qapplication were referenced to accommodate
 the latest Anaconda version, which has reorganized where those modules are stored.
-This was causing a fatal startup error.
-version 3.7.5
 
-• changes the routine that looks for the latest version of PyOTE to one provided by Kia
+This was causing a fatal startup error.
+version 3.7.5
+• changes the routine that looks for the latest version of PyOTE to one provided by Kia
 Getrost. His version contacts the PyPI repository via a json query and is the officially
 supported way to get version info. My version was based on a 'hack' that depended on
 a special feature of pip (the loader that get programs from the PyPI repository) that was
 marked as 'unsupported'. That worked for many years until the pip programmers
 removed the 'special feature' as was their right (and the implicit promise/warning, I
 guess). This caused several users to always get a message that they were not running
 the most recent version of PyOTE, even though they were. Again: thanks to Kia
@@ -839,18 +839,21 @@
 adds suggestion to right-click help on penumbral fit checkbox for how to find the
 penumbral curve csv file that is provided for practice purposes.
 
 version 3.6.8
 • adds modeling of off centerline observations to lightcurve calibration curve
 generation
 version 3.6.7
-• clarified the location of the Enable Manual Timestamp Entry checkbox in the
+
+•
+
+clarified the location of the Enable Manual Timestamp Entry checkbox in the
 pop-up message appears when there are no timestamps in the csv file.
 
-version 3.6.6
+version 3.6.6
 • modified the lightcurve demo to show more clearly the camera exposure
 function and the star intensity function that are convolved with the diffraction
 lightcurve to produce the lightcurve as seen by the camera.
 The right-click help connected to the Demo button has been expanded to
 include a discussion of the convolution operation and hopefully provide some
 context to aid in understanding the star and camera function plots.
 version 3.6.5
@@ -875,17 +878,16 @@
 size. (I'm told that Occult only uses 2 digits anyway.) I also updated the context
 help associated with the … fill Excel report button
 version 3.6.0
 • provides the ability to fill entries in the Excel spreadsheet Asteroid Occultation
 Report Form from PyOTE results, thus eliminating transcription errors.
 A button to allow the user to activate this 'fill' has been added just to the right of
 
-the … write report button
-
-NOTE: the normal .xls report form that OccultWatcher creates and prefills (when
+the … write report button
+NOTE: the normal .xls report form that OccultWatcher creates and prefills (when
 requested) during your report to OccultWatcher ...
 … MUST BE CONVERTED to .xlsx for use by PyOTE!
 … For Windows users, Excel will read an .xls file and save it as .xlsx
 … For Mac/Linux users, LibreOffice will read an .xls file and save it as .xlsx
 Sorry about this extra step, but it was necessary. The downstream tools used by area
 coordinators work equally well with the .xls and .xlsx forms of the spreadsheet, so there is no
 problem sending in the .xlsx version.
@@ -910,18 +912,21 @@
 appeared not to have occurred (when the normalization effect was
 subtle/minor).
 version 3.5.6
 • fixed a bug that kept a user from selecting a new file to read if PyOTE had been
 started from PyMovie. Previously, it had only reopened the same file instead of
 giving the user a file select dialog to choose from.
 version 3.5.5
-• fixed a bug that kept occultations from being extracted from lightcurves 5 and
+
+•
+
+fixed a bug that kept occultations from being extracted from lightcurves 5 and
 up. The lightcurves above 4 could be viewed --- they just couldn't be processed
+through the event finder because they were a different type (coding error)
 
-through the event finder because they were a different type (coding error)
 version 3.5.4
 • made the 'get newest version' code identical to that in PyMovie in hopes that
 that will resolve the issue that some people experience with pip (or python)
 installing downloaded pyote in a directory where it subsequently cannot be
 discovered. The change is minute, so I'm not optimistic, but it's worth a shot.
 version 3.5.3
 • removed the blank lines between header lines extracted from the csv file and
@@ -956,17 +961,17 @@
 
 NEW: when 'trims' have been placed, a 'write csv' process will honor those
 values and produce a 'trimmed' output file.
 
 •
 
 NEW: when a light curve has been 'normalized', the changed values are written
-to the data table where, once again, a 'write csv' process will capture the results.
 
-•
+to the data table where, once again, a 'write csv' process will capture the results.
+•
 
 Added additional reminders that the start-of-exposure timestamp/timing
 convention is employed.
 
 version 3.4.9
 • Added some explanatory language to the “Excel report” section regarding the
 proper interpretation of the 'false positive probability' number.
@@ -995,29 +1000,26 @@
 version 3.4.6
 • Adds AAV Version 2 file as a type that can be read (important when Do OCR
 check is enabled)
 version 3.4.5
 • Fixes block integration which was failing when more than 4 lightcurves were
 being processed.
 •
-version 3.4.4
 
 Made use diff and Do OCR checkboxes sticky.
 
-•
-
-PyMovie files can have lightcurves extracted from more than 4 apertures (with
+version 3.4.4
+• PyMovie files can have lightcurves extracted from more than 4 apertures (with
 user supplied names). This version allows all lightcurves from PyMovie files to
 be read and made available for processing. Prior to this change, only the first 4
 lightcurves were read.
 Note: when you change the lightcurve to be analyzed (with the spinner), the log
 panel will show the aperture name for that lightcurve. That happens when the
 reference lightcurve is changed as well.
 These changes are to PyMovie file treatment ONLY.
-
 version 3.4.3
 • Fixed bug that required an entry in dist(AU) and speed(km/sec) edit boxes for a
 solution to be found (the empty entries were causing an uncaught exception).
 The intention is that PyOTE should work as it always did if a user ignores the
 new lightcurve parameter panel and makes no entries. This 'fix' was required to
 make that happen.
 version 3.4.2
@@ -1044,17 +1046,17 @@
 fiddly, so I included a test lightcurve with the download. I can't give you a
 specific location for the file because it depends on details of your particular
 installation. Find where it is by searching for example-penumbral.csv When
 you find it, copy or move it to some other folder because if you process it where
 it resides, other files will get added in your installation directory --- we really don't
 want extraneous non-program files floating around in your installation directory.
 To learn how to use the new procedure (which is a bit 'fiddly'), right-click on the
-penumbral fit checkbox --- be patient; play around.
 
-version 3.4.0
+penumbral fit checkbox --- be patient; play around.
+version 3.4.0
 • Adds the ability to specify a diffraction lightcurve for use in timing the event. A
 new panel with edit boxes for asteroid/occulting body distance (in AU --astronomical units) and asteroid/shadow speed (in km per second) has been
 added. These values are needed in order to calculate a diffraction light curve.
 In addition to modeling diffraction effects, one can add the effect of a finite star
 disk to produce a penumbral curve. NOTE: PyOTE does not yet have the ability
 to correctly analyze a penumbral curve where it takes more than 1 or 2 readings
 for the transition. That project is under way and will be in the next version.
@@ -1084,18 +1086,18 @@
 integer values, not the sub-frame values). If those timestamps are correct, the reported
 times will be correct even when there may be a few missing or duplicated frames. So
 best practice is to enter the D frame value in the spin box and visually confirm that the
 timestamp that you can see is the same as that extracted by the OCR procedure.
 Repeat for R.
 Another use for this feature is to handle the case where there is a visual timestamp, but
 either OCR was not activated during the .csv preparation, or the timestamp overlay
-came from an unsupported VTI type. The workflow would be to let PyOTE find the D
-and R frame values, but before pressing ... write report, do a Manual timestamp
 
-entry for the D and R frame entries found by viewing the relevant frames and entering
+came from an unsupported VTI type. The workflow would be to let PyOTE find the D
+and R frame values, but before pressing ... write report, do a Manual timestamp
+entry for the D and R frame entries found by viewing the relevant frames and entering
 the correct times in the Manual timestamp dialog.
 It should be noted that the manual timestamp entry can be performed even when
 timestamps were already present in the file --- your manual entries will cause all the
 timestamps to be recalculated.
 version 3.3.5:
 • Changed usage of max([a, b ,c]) to max(a, b, c) to see if this allows the Numba
 JIT compiler to work for one user that found version 3.3.4 failed to load/compile.
@@ -1123,18 +1125,18 @@
 • Changed lightcurve plot so that it conforms properly to 'start-of-exposure'.
 version 3.2.8
 • Changed font size in help files --- it was fine for Mac but too big for Win10
 version 3.2.7
 • Removed the 'hover-for-help' and replaced it with a 'right-click-on-item' to get
 help. This scheme was introduced in PyMovie and I found it easier to use than
 the 'hover' scheme. In practice, the 'hover' popped up when it was not needed,
-so most users eventually disabled it. As a result, it became so tedious to look at
-help --- enable hover; hover; read; disable hover --- that the help system was
 
-used less and less. The right-click-for-help is always available and easily
+so most users eventually disabled it. As a result, it became so tedious to look at
+help --- enable hover; hover; read; disable hover --- that the help system was
+used less and less. The right-click-for-help is always available and easily
 invoked --- hopefully this will encourage more frequent reference to it.
 version 3.2.6
 • This is a 'cosmetic' release --- there should be NO detectable differences from
 version 3.2.5 in terms of functionality.
 • All python files were brought into compliance with PEP 8 coding standards.
 Only I care about that.
 • More significantly, I removed the dependency on C code by using Numba as a
@@ -1169,18 +1171,18 @@
 original csv file gets modified and overwritten by the addition of empty fields at
 every row sufficient to match the number of columns in the longest
 header/comment row --- the spreadsheet program did this to satisfy its internal
 requirement that every row have an equal number of columns. The result is
 superfluous commas at the end of data lines (that Tangra did NOT put there).
 Until this version, that 'butchered' file could not be read. This version adds code
 to parse data lines only up to the first non-empty column. Hopefully this will not
-have ramifications in the future (like a format change that has empty fields
-followed by non-empty fields --- not a likely expectation).
 
-version 3.2.0
+have ramifications in the future (like a format change that has empty fields
+followed by non-empty fields --- not a likely expectation).
+version 3.2.0
 • Changed GUI to better align text on min max edit boxes to avoid confusion.
 version 3.1.9
 • Fixed a bug in the test for a min/max solution search being constrained by a too
 large min value.
 version 3.1.8
 • version 3.1.7 was released without an updated version history. Here is what
 was changed in 3.1.7:
@@ -1211,19 +1213,20 @@
 That 'competitor' would thus mask an event with slightly worse statistics but a
 larger magDrop. The change was to test every candidate against a straight line
 during the search. This does make the search time longer, but not too much
 longer.
 version 3.1.4:
 • Fixed error in new dropped reading detection logic when light curve was
 processed in field mode.
-•
+
+•
 
 Cleaned up some language in tooltips.
 
-version 3.1.3:
+version 3.1.3:
 • Expanded manual timestamp preset time deltas to include NTSC and PAL field
 times. Also added ability to evaluate numeric expressions entered in the
 'Custom time' box: now you can type 1.001/60.0 in that box if you wish.
 •
 
 Eliminated the 'entry num' column in the data matrix at the lower left of the GUI.
 The 'entry num' is unused and a possible source of confusion with the frame or
@@ -1265,29 +1268,26 @@
 to more clearly suggest that after finding an 'event', one should then press the
 'report' button to the right in order to complete the process.
 
 version 3.1.0:
 • Added a Mac version of a pyote startup file. It is automatically placed on the
 Desktop the first time pyote is run. Double-clicking on that Desktop file icon will
 start pyote thereafter.
-version 3.0.8:
-
-•
 
-Added a Windows batch file to the distribution that, when executed, will startup
+version 3.0.8:
+• Added a Windows batch file to the distribution that, when executed, will startup
 pyote. The file is called PYOTE.bat and is automatically copied to
 C:\Anaconda3 (if it is not already there) when pyote is first run. Now, to create a
 clickable desktop icon for starting up pyote, a user need only go to the
 C:\Anaconda3 directory, locate the PYOTE.bat file, create a shortcut to it, and
 drag the shortcut to the desktop. Remember, that file does not appear until the
 first run of pyote.
 The ‘skipped’ version numbers were caused by the need for repeated testing of
 this new feature, each test requiring a new version, even though functionality did
 not change,
-
 version 3.0.1:
 • Restored the vertical splitter between the command/plot area and the
 table/report area. Somewhere along the line this capability was accidentally
 removed, and the lack of the splitter was not noticed. Now it’s back.
 version 3.0.0:
 • No code changes. This version is the same as 2.1.6 except that it is built on
 python 3.7. The previous versions used python 3.6. This allows new users to
@@ -1308,18 +1308,18 @@
 version 2.1.3:
 • A minor change to how color bars are plotted when the automatic block
 integration feature is employed. The edges now appear between data points so
 the bands are easier to see, particularly for 2 point block sizes.
 version 2.1.2:
 • To ease usage of the automatic block integration feature, accepting the
 automatically determined block integration parameters no longer uses a modal
-query box, which interfered with the ability to explore/expand the light curve plot.
-Now there is separate button which gets enabled after an automatic block
 
-integration completes.
+query box, which interfered with the ability to explore/expand the light curve plot.
+Now there is separate button which gets enabled after an automatic block
+integration completes.
 version 2.1.1
 • Added progress bar tracking of block integration analysis because it can take an
 extended amount of time to complete the analysis when the light curve has
 many points.
 version 2.1.0
 • Added automatic determination of 'correct' block size and offset for block
 integration when user clicks Block integrate button without selecting the two
@@ -1358,18 +1358,18 @@
 Adds the ability to select which light curve is to be analyzed. Previous versions
 would only analyze the first light curve for D and R events. This flexibility is
 useful in general, but was particularly needed to support LED flash timing.
 Adds a checkbox to force manual entry of timestamp info. This is useful when
 OCR on a VTI timed light curve has catastrophic errors. It is always employed
 when using LED flash timing.
 During the error bar calculation, it is possible for the Cholesky decomposition
-needed for treating correlated noise to fail. Previous versions treated this as a
-fatal error and would not produce a final report. This version instead treats the
 
-noise as uncorrelated and continues processing to produce a final report.
+needed for treating correlated noise to fail. Previous versions treated this as a
+fatal error and would not produce a final report. This version instead treats the
+noise as uncorrelated and continues processing to produce a final report.
 version 2.0.6
 • Added additional instruction in the popup that appears when no timestamps are
 found in the csv file. This will give casual users additional guidance and
 clarification for the manual timestamp entry process.
 version 2.0.5
 • files generated by pyote now contain PYOTE in the filename.
 •
@@ -1406,17 +1406,17 @@
 modification added in version 1.46 is no longer needed.
 
 •
 
 removes unneeded 'analyze noise' buttons and rearranged other buttons to be
 in-line rather than one above the other to allow the vertical splitter between the
 plot area and report area more room to change (a help to those using screens
-with relatively low pixel densities).
 
-version 1.47
+with relatively low pixel densities).
+version 1.47
 • adds bold red highlighting to message:
 ! There is something wrong with timestamps at D and/or R or frames have been dropped !
 
 so that it is harder to miss.
 
 version 1.46
 • adds automatic recalculation of baseline and event noise parameters utilizing all
```

### Comparing `pyote-5.3.3/src/pyoteapp/pyote.py` & `pyote-5.3.4/src/pyoteapp/pyote.py`

 * *Files 0% similar despite different names*

```diff
@@ -4880,26 +4880,65 @@
         inp.setFixedSize(400, 200)
         p = inp.palette()
         p.setColor(inp.backgroundRole(), QtCore.Qt.GlobalColor.gray)
         inp.setPalette(p)
         inp.setWindowTitle('Rename fit metrics')
         inp.setLabelText('Enter name to be used for the .xlsx file: ')
 
+        lightCurveDir = os.path.dirname(self.csvFilePath)
+        head, tail = os.path.split(lightCurveDir)
+
+        inp.setTextValue(tail)
+
         if inp.exec_() == QtWidgets.QDialog.DialogCode.Accepted:
             # This gets the folder where the light-curve.csv is located
             lightCurveDir = os.path.dirname(self.csvFilePath)
             current_metric_filepath = lightCurveDir + '\\fit_metrics.txt'
             name_given = inp.textValue()
             if '.xlsx' in name_given:
                 new_metric_filepath = lightCurveDir + f'\\{name_given}'
             else:
                 new_metric_filepath = lightCurveDir + f'\\{name_given}.xlsx'
-            pd.read_csv(current_metric_filepath, index_col=0).to_excel(new_metric_filepath)
-            # os.rename(current_metric_filepath, new_metric_filepath)
-            # print(f'{new_metric_filepath}')
+
+            # Make a Pandas data frame from the csv file
+            df = pd.read_csv(current_metric_filepath)
+
+            # Create a Pandas Excel writer using xlswriter as the engine
+            writer = pd.ExcelWriter(new_metric_filepath, engine='xlsxwriter')
+
+            # Convert the dataframe to an Xlsxwriter Excel object
+            df.to_excel(writer, sheet_name='Sheet1', index=False)
+
+            # Get the xlsxwriter workbook and workbook objects
+            workbook = writer.book
+            worksheet = writer.sheets['Sheet1']
+
+            # Create some cell formats
+            formatNum4 = workbook.add_format({"num_format": "0.0000"})
+            formatNum3 = workbook.add_format({"num_format": "0.000"})
+            formatNum2 = workbook.add_format({"num_format": "0.00"})
+            formatNum1 = workbook.add_format({"num_format": "0.0"})
+
+            # Set column widths and formats
+            # worksheet.set_column(first_col, last_col, width, format)  width can be None and format can be missing
+            worksheet.set_column( 0,  0, 30)                  # aperture name
+            worksheet.set_column( 1,  1, 15, formatNum4)      # time err
+            worksheet.set_column( 2,  2, None, formatNum2)    # DNR
+            worksheet.set_column( 3,  3, None, formatNum2)    # FP metric
+            worksheet.set_column( 4,  4, None, formatNum2)    # magDrop
+            worksheet.set_column( 5,  5, 13, formatNum1)      # percent drop
+            worksheet.set_column( 6,  6, 15, formatNum4)      # duration
+            worksheet.set_column( 7,  8, 13)                  # D time  and R time
+            worksheet.set_column( 9, 10, None, formatNum2)    # D frame  and R frame
+            worksheet.set_column(11, 12, 13, formatNum2)      # D and A
+            worksheet.set_column(13, 14, 13, formatNum2)      # sigmaB and sigmaA
+            worksheet.set_column(15, 15, 15, formatNum1)      # observed drop
+            worksheet.set_column(16, 16, None, formatNum1)    # observed drop
+            worksheet.set_column(17, 17, None, formatNum1)    # FP margin
+            writer.close()
 
         inp.deleteLater()
 
     def fillExcelReport(self):
         # Open a file select dialog
         xlsxfilepath, _ = QFileDialog.getOpenFileName(
             self,  # parent
```

### Comparing `pyote-5.3.3/src/pyoteapp/pyote_modelling_utility_functions.py` & `pyote-5.3.4/src/pyoteapp/pyote_modelling_utility_functions.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/showVideoFrames.py` & `pyote-5.3.4/src/pyoteapp/showVideoFrames.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/solverUtils.py` & `pyote-5.3.4/src/pyoteapp/solverUtils.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/subframe_timing_utilities.py` & `pyote-5.3.4/src/pyoteapp/subframe_timing_utilities.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/timestampDialog.py` & `pyote-5.3.4/src/pyoteapp/timestampDialog.py`

 * *Files identical despite different names*

### Comparing `pyote-5.3.3/src/pyoteapp/timestampUtils.py` & `pyote-5.3.4/src/pyoteapp/timestampUtils.py`

 * *Files identical despite different names*

