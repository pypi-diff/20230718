# Comparing `tmp/pyviscous-1.2.0.tar.gz` & `tmp/pyviscous-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyviscous-1.2.0.tar", last modified: Tue Jul 18 02:31:52 2023, max compression
+gzip compressed data, was "pyviscous-1.2.1.tar", last modified: Tue Jul 18 03:39:49 2023, max compression
```

## Comparing `pyviscous-1.2.0.tar` & `pyviscous-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-07-18 02:31:52.343800 pyviscous-1.2.0/
--rw-r--r--   0 hongliliu   (501) staff       (20)     1603 2023-07-18 02:24:06.000000 pyviscous-1.2.0/LICENSE
--rw-r--r--   0 hongliliu   (501) staff       (20)     2645 2023-07-18 02:31:52.343483 pyviscous-1.2.0/PKG-INFO
--rw-r--r--   0 hongliliu   (501) staff       (20)     1830 2023-07-18 02:24:06.000000 pyviscous-1.2.0/README.md
-drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-07-18 02:31:52.341407 pyviscous-1.2.0/pyviscous/
--rwxr-xr-x   0 hongliliu   (501) staff       (20)       85 2023-07-18 02:24:06.000000 pyviscous-1.2.0/pyviscous/__init__.py
--rw-r--r--   0 hongliliu   (501) staff       (20)    24534 2023-07-18 02:24:06.000000 pyviscous-1.2.0/pyviscous/plot.py
--rwxr-xr-x   0 hongliliu   (501) staff       (20)    22364 2023-07-18 02:24:06.000000 pyviscous-1.2.0/pyviscous/pyviscous.py
-drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-07-18 02:31:52.343018 pyviscous-1.2.0/pyviscous.egg-info/
--rw-r--r--   0 hongliliu   (501) staff       (20)     2645 2023-07-18 02:31:51.000000 pyviscous-1.2.0/pyviscous.egg-info/PKG-INFO
--rw-r--r--   0 hongliliu   (501) staff       (20)      321 2023-07-18 02:31:52.000000 pyviscous-1.2.0/pyviscous.egg-info/SOURCES.txt
--rw-r--r--   0 hongliliu   (501) staff       (20)        1 2023-07-18 02:31:51.000000 pyviscous-1.2.0/pyviscous.egg-info/dependency_links.txt
--rw-r--r--   0 hongliliu   (501) staff       (20)       49 2023-07-18 02:31:52.000000 pyviscous-1.2.0/pyviscous.egg-info/entry_points.txt
--rw-r--r--   0 hongliliu   (501) staff       (20)        1 2023-07-18 02:27:23.000000 pyviscous-1.2.0/pyviscous.egg-info/not-zip-safe
--rw-r--r--   0 hongliliu   (501) staff       (20)       54 2023-07-18 02:31:52.000000 pyviscous-1.2.0/pyviscous.egg-info/requires.txt
--rw-r--r--   0 hongliliu   (501) staff       (20)       10 2023-07-18 02:31:52.000000 pyviscous-1.2.0/pyviscous.egg-info/top_level.txt
--rw-r--r--   0 hongliliu   (501) staff       (20)       38 2023-07-18 02:31:52.343906 pyviscous-1.2.0/setup.cfg
--rwxr-xr-x   0 hongliliu   (501) staff       (20)     1692 2023-07-18 02:24:06.000000 pyviscous-1.2.0/setup.py
+drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-07-18 03:39:49.175521 pyviscous-1.2.1/
+-rw-r--r--   0 hongliliu   (501) staff       (20)     1603 2023-07-18 02:24:06.000000 pyviscous-1.2.1/LICENSE
+-rw-r--r--   0 hongliliu   (501) staff       (20)     2625 2023-07-18 03:39:49.175281 pyviscous-1.2.1/PKG-INFO
+-rw-r--r--   0 hongliliu   (501) staff       (20)     1830 2023-07-18 02:24:06.000000 pyviscous-1.2.1/README.md
+drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-07-18 03:39:49.172574 pyviscous-1.2.1/pyviscous/
+-rwxr-xr-x   0 hongliliu   (501) staff       (20)       85 2023-07-18 02:24:06.000000 pyviscous-1.2.1/pyviscous/__init__.py
+-rw-r--r--   0 hongliliu   (501) staff       (20)    24534 2023-07-18 02:24:06.000000 pyviscous-1.2.1/pyviscous/plot.py
+-rwxr-xr-x   0 hongliliu   (501) staff       (20)    22364 2023-07-18 02:24:06.000000 pyviscous-1.2.1/pyviscous/pyviscous.py
+drwxr-xr-x   0 hongliliu   (501) staff       (20)        0 2023-07-18 03:39:49.174947 pyviscous-1.2.1/pyviscous.egg-info/
+-rw-r--r--   0 hongliliu   (501) staff       (20)     2625 2023-07-18 03:39:49.000000 pyviscous-1.2.1/pyviscous.egg-info/PKG-INFO
+-rw-r--r--   0 hongliliu   (501) staff       (20)      321 2023-07-18 03:39:49.000000 pyviscous-1.2.1/pyviscous.egg-info/SOURCES.txt
+-rw-r--r--   0 hongliliu   (501) staff       (20)        1 2023-07-18 03:39:49.000000 pyviscous-1.2.1/pyviscous.egg-info/dependency_links.txt
+-rw-r--r--   0 hongliliu   (501) staff       (20)       49 2023-07-18 03:39:49.000000 pyviscous-1.2.1/pyviscous.egg-info/entry_points.txt
+-rw-r--r--   0 hongliliu   (501) staff       (20)        1 2023-07-18 02:27:23.000000 pyviscous-1.2.1/pyviscous.egg-info/not-zip-safe
+-rw-r--r--   0 hongliliu   (501) staff       (20)       59 2023-07-18 03:39:49.000000 pyviscous-1.2.1/pyviscous.egg-info/requires.txt
+-rw-r--r--   0 hongliliu   (501) staff       (20)       10 2023-07-18 03:39:49.000000 pyviscous-1.2.1/pyviscous.egg-info/top_level.txt
+-rw-r--r--   0 hongliliu   (501) staff       (20)       38 2023-07-18 03:39:49.175590 pyviscous-1.2.1/setup.cfg
+-rwxr-xr-x   0 hongliliu   (501) staff       (20)     1697 2023-07-18 03:36:48.000000 pyviscous-1.2.1/setup.py
```

### Comparing `pyviscous-1.2.0/LICENSE` & `pyviscous-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyviscous-1.2.0/PKG-INFO` & `pyviscous-1.2.1/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyviscous
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python codes to implement the VISCOUSm global sensitivity analysis framework
 Home-page: https://github.com/CH-Earth/pyviscous
 Author: Hongli Liu
 Author-email: hongliliu68@gmail.com
 License: GNU General Public License v3
 Keywords: pyviscous
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -43,9 +42,7 @@
 ### References
 Liu, H., Clark, M. P., Gharari, S., Sheikholeslami, R., Freer, J., Knoben, W. J. M., Marsh C. B., & Papalexiou, S. M. (2022) pyVISCOUS: An open-source tool for computationally frugal global sensitivity analysis. (Submitted to Water Resources Research)
 
 Sheikholeslami, R., Gharari, S., Papalexiou, S. M., & Clark, M. P. (2021) VISCOUS: A variance-based sensitivity analysis using copulas for efficient identification of dominant hydrological processes. Water Resources Research, 57, e2020WR028435, https://doi.org/10.1029/2020WR028435
 
 ---
 This package was created with Cookiecutter and the `https://github.com/audreyr/cookiecutter-pypackage` project template.
-
-
```

### Comparing `pyviscous-1.2.0/README.md` & `pyviscous-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyviscous-1.2.0/pyviscous/plot.py` & `pyviscous-1.2.1/pyviscous/plot.py`

 * *Files identical despite different names*

### Comparing `pyviscous-1.2.0/pyviscous/pyviscous.py` & `pyviscous-1.2.1/pyviscous/pyviscous.py`

 * *Files identical despite different names*

### Comparing `pyviscous-1.2.0/pyviscous.egg-info/PKG-INFO` & `pyviscous-1.2.1/pyviscous.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: pyviscous
-Version: 1.2.0
+Version: 1.2.1
 Summary: Python codes to implement the VISCOUSm global sensitivity analysis framework
 Home-page: https://github.com/CH-Earth/pyviscous
 Author: Hongli Liu
 Author-email: hongliliu68@gmail.com
 License: GNU General Public License v3
 Keywords: pyviscous
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
@@ -43,9 +42,7 @@
 ### References
 Liu, H., Clark, M. P., Gharari, S., Sheikholeslami, R., Freer, J., Knoben, W. J. M., Marsh C. B., & Papalexiou, S. M. (2022) pyVISCOUS: An open-source tool for computationally frugal global sensitivity analysis. (Submitted to Water Resources Research)
 
 Sheikholeslami, R., Gharari, S., Papalexiou, S. M., & Clark, M. P. (2021) VISCOUS: A variance-based sensitivity analysis using copulas for efficient identification of dominant hydrological processes. Water Resources Research, 57, e2020WR028435, https://doi.org/10.1029/2020WR028435
 
 ---
 This package was created with Cookiecutter and the `https://github.com/audreyr/cookiecutter-pypackage` project template.
-
-
```

### Comparing `pyviscous-1.2.0/setup.py` & `pyviscous-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 try:
     from setuptools import setup
 except:
     from distutils.core import setup
 
 from setuptools import find_packages
 
-requirements = ['numpy', 'pandas', 'scipy', 'sklearn', 'copulae', 'matplotlib', 'jupyter']
+requirements = ['numpy', 'pandas', 'scipy', 'scikit-learn', 'copulae', 'matplotlib', 'jupyter']
 
 test_requirements = [ ]
 
 # read the contents of your README file for distribution on PyPI
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
@@ -43,14 +43,14 @@
     include_package_data=True,
     keywords='pyviscous',
     name='pyviscous',
     packages=find_packages(include=['pyviscous', 'pyviscous.*', 'plot.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/CH-Earth/pyviscous',
-    version='1.2.0',
+    version='1.2.1',
     zip_safe=False,
     long_description=long_description,
     long_description_content_type='text/markdown',
 )
```

