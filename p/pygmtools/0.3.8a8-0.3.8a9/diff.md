# Comparing `tmp/pygmtools-0.3.8a8.tar.gz` & `tmp/pygmtools-0.3.8a9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmtools-0.3.8a8.tar", last modified: Sat Jul  8 07:48:56 2023, max compression
+gzip compressed data, was "pygmtools-0.3.8a9.tar", last modified: Sat Jul  8 10:33:19 2023, max compression
```

## Comparing `pygmtools-0.3.8a8.tar` & `pygmtools-0.3.8a9.tar`

### file list

```diff
@@ -1,44 +1,42 @@
-drwxrwxrwx   0        0        0        0 2023-07-08 07:48:56.668162 pygmtools-0.3.8a8/
--rw-rw-rw-   0        0        0      508 2023-05-03 08:07:01.000000 pygmtools-0.3.8a8/LICENSE
--rw-rw-rw-   0        0        0    13827 2023-07-08 07:48:56.668162 pygmtools-0.3.8a8/PKG-INFO
--rw-rw-rw-   0        0        0    12718 2023-05-03 08:07:01.000000 pygmtools-0.3.8a8/README.md
-drwxrwxrwx   0        0        0        0 2023-07-08 07:48:56.656801 pygmtools-0.3.8a8/pygmtools/
--rw-rw-rw-   0        0        0     2120 2023-07-08 07:48:34.000000 pygmtools-0.3.8a8/pygmtools/__init__.py
--rw-rw-rw-   0        0        0    27000 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/benchmark.py
--rw-rw-rw-   0        0        0    58666 2023-07-07 12:42:20.000000 pygmtools-0.3.8a8/pygmtools/classic_solvers.py
--rw-rw-rw-   0        0        0    59231 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/dataset.py
--rw-rw-rw-   0        0        0     3112 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/dataset_config.py
--rw-rw-rw-   0        0        0    58908 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/jittor_backend.py
--rw-rw-rw-   0        0        0    12371 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/jittor_modules.py
-drwxrwxrwx   0        0        0        0 2023-07-08 07:48:56.661244 pygmtools-0.3.8a8/pygmtools/lib/
--rw-rw-rw-   0        0        0  1138391 2023-07-02 08:40:47.000000 pygmtools-0.3.8a8/pygmtools/lib/a_star.tar.gz
--rw-rw-rw-   0        0        0  3203980 2023-07-02 08:39:54.000000 pygmtools-0.3.8a8/pygmtools/lib/a_star.zip
--rw-rw-rw-   0        0        0    77128 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/linear_solvers.py
--rw-rw-rw-   0        0        0    21736 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/mindspore_backend.py
--rw-rw-rw-   0        0        0    44038 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/multi_graph_solvers.py
--rw-rw-rw-   0        0        0    70477 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/neural_solvers.py
--rw-rw-rw-   0        0        0    60669 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/numpy_backend.py
--rw-rw-rw-   0        0        0    15282 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/numpy_modules.py
--rw-rw-rw-   0        0        0    57860 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/paddle_backend.py
--rw-rw-rw-   0        0        0    11899 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/paddle_modules.py
--rw-rw-rw-   0        0        0    15443 2023-07-07 12:38:50.000000 pygmtools-0.3.8a8/pygmtools/pytorch_astar_modules.py
--rw-rw-rw-   0        0        0    74579 2023-07-07 12:56:18.000000 pygmtools-0.3.8a8/pygmtools/pytorch_backend.py
--rw-rw-rw-   0        0        0    12329 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/pytorch_modules.py
--rw-rw-rw-   0        0        0    23046 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/tensorflow_backend.py
--rw-rw-rw-   0        0        0      508 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/tensorflow_modules.py
--rw-rw-rw-   0        0        0    51707 2023-07-07 11:54:30.000000 pygmtools-0.3.8a8/pygmtools/utils.py
-drwxrwxrwx   0        0        0        0 2023-07-08 07:48:56.658935 pygmtools-0.3.8a8/pygmtools.egg-info/
--rw-rw-rw-   0        0        0    13827 2023-07-08 07:48:56.000000 pygmtools-0.3.8a8/pygmtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      982 2023-07-08 07:48:56.000000 pygmtools-0.3.8a8/pygmtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-08 07:48:56.000000 pygmtools-0.3.8a8/pygmtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-07-08 07:48:56.000000 pygmtools-0.3.8a8/pygmtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-07-08 07:48:56.000000 pygmtools-0.3.8a8/pygmtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-08 07:48:56.668162 pygmtools-0.3.8a8/setup.cfg
--rw-rw-rw-   0        0        0     6259 2023-07-08 07:48:21.000000 pygmtools-0.3.8a8/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-08 07:48:56.667124 pygmtools-0.3.8a8/tests/
--rw-rw-rw-   0        0        0    16089 2023-07-02 10:34:16.000000 pygmtools-0.3.8a8/tests/test_classic_solvers.py
--rw-rw-rw-   0        0        0     5561 2023-05-03 08:07:01.000000 pygmtools-0.3.8a8/tests/test_dataset.py
--rw-rw-rw-   0        0        0     3800 2023-05-03 08:07:01.000000 pygmtools-0.3.8a8/tests/test_misc.py
--rw-rw-rw-   0        0        0    13302 2023-05-03 08:07:01.000000 pygmtools-0.3.8a8/tests/test_multi_graph_solvers.py
--rw-rw-rw-   0        0        0     9288 2023-05-03 08:07:01.000000 pygmtools-0.3.8a8/tests/test_neural_solvers.py
--rw-rw-rw-   0        0        0     1007 2023-05-03 08:07:01.000000 pygmtools-0.3.8a8/tests/test_utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 10:33:19.301498 pygmtools-0.3.8a9/
+-rw-rw-rw-   0        0        0      508 2023-05-03 08:07:01.000000 pygmtools-0.3.8a9/LICENSE
+-rw-rw-rw-   0        0        0    13827 2023-07-08 10:33:19.301498 pygmtools-0.3.8a9/PKG-INFO
+-rw-rw-rw-   0        0        0    12718 2023-05-03 08:07:01.000000 pygmtools-0.3.8a9/README.md
+drwxrwxrwx   0        0        0        0 2023-07-08 10:33:19.296498 pygmtools-0.3.8a9/pygmtools/
+-rw-rw-rw-   0        0        0     2120 2023-07-08 07:57:16.000000 pygmtools-0.3.8a9/pygmtools/__init__.py
+-rw-rw-rw-   0        0        0    58368 2023-07-08 10:21:43.000000 pygmtools-0.3.8a9/pygmtools/a_star.cp310-win_amd64.pyd
+-rw-rw-rw-   0        0        0    27000 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/benchmark.py
+-rw-rw-rw-   0        0        0    58666 2023-07-07 12:42:20.000000 pygmtools-0.3.8a9/pygmtools/classic_solvers.py
+-rw-rw-rw-   0        0        0    59231 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/dataset.py
+-rw-rw-rw-   0        0        0     3112 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/dataset_config.py
+-rw-rw-rw-   0        0        0    58908 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/jittor_backend.py
+-rw-rw-rw-   0        0        0    12371 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/jittor_modules.py
+-rw-rw-rw-   0        0        0    77128 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/linear_solvers.py
+-rw-rw-rw-   0        0        0    21736 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/mindspore_backend.py
+-rw-rw-rw-   0        0        0    44038 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/multi_graph_solvers.py
+-rw-rw-rw-   0        0        0    70477 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/neural_solvers.py
+-rw-rw-rw-   0        0        0    60669 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/numpy_backend.py
+-rw-rw-rw-   0        0        0    15282 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/numpy_modules.py
+-rw-rw-rw-   0        0        0    57860 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/paddle_backend.py
+-rw-rw-rw-   0        0        0    11899 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/paddle_modules.py
+-rw-rw-rw-   0        0        0    15443 2023-07-07 12:38:50.000000 pygmtools-0.3.8a9/pygmtools/pytorch_astar_modules.py
+-rw-rw-rw-   0        0        0    74579 2023-07-07 12:56:18.000000 pygmtools-0.3.8a9/pygmtools/pytorch_backend.py
+-rw-rw-rw-   0        0        0    12329 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/pytorch_modules.py
+-rw-rw-rw-   0        0        0    23046 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/tensorflow_backend.py
+-rw-rw-rw-   0        0        0      508 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/tensorflow_modules.py
+-rw-rw-rw-   0        0        0    51707 2023-07-07 11:54:30.000000 pygmtools-0.3.8a9/pygmtools/utils.py
+drwxrwxrwx   0        0        0        0 2023-07-08 10:33:19.301498 pygmtools-0.3.8a9/pygmtools.egg-info/
+-rw-rw-rw-   0        0        0    13827 2023-07-08 10:33:19.000000 pygmtools-0.3.8a9/pygmtools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      966 2023-07-08 10:33:19.000000 pygmtools-0.3.8a9/pygmtools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-08 10:33:19.000000 pygmtools-0.3.8a9/pygmtools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-07-08 10:33:19.000000 pygmtools-0.3.8a9/pygmtools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-07-08 10:33:19.000000 pygmtools-0.3.8a9/pygmtools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-08 10:33:19.301498 pygmtools-0.3.8a9/setup.cfg
+-rw-rw-rw-   0        0        0     6695 2023-07-08 10:32:58.000000 pygmtools-0.3.8a9/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-08 10:33:19.301498 pygmtools-0.3.8a9/tests/
+-rw-rw-rw-   0        0        0    16089 2023-07-02 10:34:16.000000 pygmtools-0.3.8a9/tests/test_classic_solvers.py
+-rw-rw-rw-   0        0        0     5561 2023-05-03 08:07:01.000000 pygmtools-0.3.8a9/tests/test_dataset.py
+-rw-rw-rw-   0        0        0     3800 2023-05-03 08:07:01.000000 pygmtools-0.3.8a9/tests/test_misc.py
+-rw-rw-rw-   0        0        0    13302 2023-05-03 08:07:01.000000 pygmtools-0.3.8a9/tests/test_multi_graph_solvers.py
+-rw-rw-rw-   0        0        0     9288 2023-05-03 08:07:01.000000 pygmtools-0.3.8a9/tests/test_neural_solvers.py
+-rw-rw-rw-   0        0        0     1007 2023-05-03 08:07:01.000000 pygmtools-0.3.8a9/tests/test_utils.py
```

### Comparing `pygmtools-0.3.8a8/PKG-INFO` & `pygmtools-0.3.8a9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.3.8a8
+Version: 0.3.8a9
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
```

### Comparing `pygmtools-0.3.8a8/README.md` & `pygmtools-0.3.8a9/README.md`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/__init__.py` & `pygmtools-0.3.8a9/pygmtools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 from .benchmark import Benchmark
 from .linear_solvers import sinkhorn, hungarian
 from .classic_solvers import rrwm, sm, ipfp, a_star
 from .multi_graph_solvers import cao, mgm_floyd, gamgm
 from .neural_solvers import pca_gm, ipca_gm, cie, ngm
 import pygmtools.utils as utils
 BACKEND = 'numpy'
-__version__ = '0.3.8-alpha8'
+__version__ = '0.3.8-alpha9'
 __author__ = 'ThinkLab at SJTU'
 
 
 def env_report():
     """
     Print environment report
     """
```

### Comparing `pygmtools-0.3.8a8/pygmtools/benchmark.py` & `pygmtools-0.3.8a9/pygmtools/benchmark.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/classic_solvers.py` & `pygmtools-0.3.8a9/pygmtools/classic_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/dataset.py` & `pygmtools-0.3.8a9/pygmtools/dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/dataset_config.py` & `pygmtools-0.3.8a9/pygmtools/dataset_config.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/jittor_backend.py` & `pygmtools-0.3.8a9/pygmtools/jittor_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/jittor_modules.py` & `pygmtools-0.3.8a9/pygmtools/jittor_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/linear_solvers.py` & `pygmtools-0.3.8a9/pygmtools/linear_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/mindspore_backend.py` & `pygmtools-0.3.8a9/pygmtools/mindspore_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/multi_graph_solvers.py` & `pygmtools-0.3.8a9/pygmtools/multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/neural_solvers.py` & `pygmtools-0.3.8a9/pygmtools/neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/numpy_backend.py` & `pygmtools-0.3.8a9/pygmtools/numpy_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/numpy_modules.py` & `pygmtools-0.3.8a9/pygmtools/numpy_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/paddle_backend.py` & `pygmtools-0.3.8a9/pygmtools/paddle_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/paddle_modules.py` & `pygmtools-0.3.8a9/pygmtools/paddle_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/pytorch_astar_modules.py` & `pygmtools-0.3.8a9/pygmtools/pytorch_astar_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/pytorch_backend.py` & `pygmtools-0.3.8a9/pygmtools/pytorch_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/pytorch_modules.py` & `pygmtools-0.3.8a9/pygmtools/pytorch_modules.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/tensorflow_backend.py` & `pygmtools-0.3.8a9/pygmtools/tensorflow_backend.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools/utils.py` & `pygmtools-0.3.8a9/pygmtools/utils.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/pygmtools.egg-info/PKG-INFO` & `pygmtools-0.3.8a9/pygmtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pygmtools
-Version: 0.3.8a8
+Version: 0.3.8a9
 Summary: pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. pygmtools also provides dataset API for standard graph matching benchmarks.
 Home-page: https://pygmtools.readthedocs.io/
 Author: ThinkLab at SJTU
 License: Mulan PSL v2
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Operating System :: OS Independent
```

### Comparing `pygmtools-0.3.8a8/pygmtools.egg-info/SOURCES.txt` & `pygmtools-0.3.8a9/pygmtools.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 LICENSE
 README.md
 setup.py
 pygmtools/__init__.py
+pygmtools/a_star.cp310-win_amd64.pyd
 pygmtools/benchmark.py
 pygmtools/classic_solvers.py
 pygmtools/dataset.py
 pygmtools/dataset_config.py
 pygmtools/jittor_backend.py
 pygmtools/jittor_modules.py
 pygmtools/linear_solvers.py
@@ -23,15 +24,13 @@
 pygmtools/tensorflow_modules.py
 pygmtools/utils.py
 pygmtools.egg-info/PKG-INFO
 pygmtools.egg-info/SOURCES.txt
 pygmtools.egg-info/dependency_links.txt
 pygmtools.egg-info/requires.txt
 pygmtools.egg-info/top_level.txt
-pygmtools/lib/a_star.tar.gz
-pygmtools/lib/a_star.zip
 tests/test_classic_solvers.py
 tests/test_dataset.py
 tests/test_misc.py
 tests/test_multi_graph_solvers.py
 tests/test_neural_solvers.py
 tests/test_utils.py
```

### Comparing `pygmtools-0.3.8a8/setup.py` & `pygmtools-0.3.8a9/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,51 +9,22 @@
 import sys
 from shutil import rmtree
 import re
 import platform
 from setuptools import find_packages, setup, Command
 import tarfile
 import zipfile
-import os
 import distro
 import shutil
-import atexit
-from setuptools.command.install import install
-
-def unzip_file(zip_file_path, extract_folder_path):
-    with zipfile.ZipFile(zip_file_path, 'r') as zipObj:
-        zipObj.extractall(extract_folder_path)
-
-def untar_file(tar_file_path, extract_folder_path):
-    with tarfile.open(tar_file_path, 'r:gz') as tarObj:
-        tarObj.extractall(extract_folder_path)
+from wheel.bdist_wheel import bdist_wheel as _bdist_wheel
 
 def get_property(prop, project):
     result = re.search(r'{}\s*=\s*[\'"]([^\'"]*)[\'"]'.format(prop), open(project + '/__init__.py').read())
     return result.group(1)
 
-def get_os_and_python_version():
-    system = platform.system()
-    python_version = ".".join(map(str, sys.version_info[:2]))
-    if system.lower() == "windows":
-        os_version = "windows"
-    elif system.lower() == "darwin":
-        os_version = "macos"
-    elif system.lower() == "linux":
-        os_version = distro.name().lower()
-    else:
-        raise ValueError("Unknown System")
-    if (os_version == 'windows'):
-        if (python_version == '3.11'):
-            python_version = '3.10'
-    else:
-        if (python_version == '3.10') or (python_version == '3.11'):
-            python_version = '3.9'
-    return os_version, python_version
-
 # Package meta-data.
 NAME = 'pygmtools'
 DESCRIPTION = 'pygmtools provides graph matching solvers in Python API and supports numpy and pytorch backends. ' \
               'pygmtools also provides dataset API for standard graph matching benchmarks.'
 URL = 'https://pygmtools.readthedocs.io/'
 AUTHOR = get_property('__author__', NAME)
 VERSION = get_property('__version__', NAME)
@@ -79,42 +50,76 @@
 if not VERSION:
     project_slug = NAME.lower().replace("-", "_").replace(" ", "_")
     with open(os.path.join(here, project_slug, '__version__.py')) as f:
         exec(f.read(), about)
 else:
     about['__version__'] = VERSION
 
-def post_install():
-    print("Detect OS Version...")
-    os_version, python_version = get_os_and_python_version()
-    print("OS Version: ",os_version)
-    filename={  'windows':{ '3.7':'a_star.cp37-win_amd64.pyd',
-                            '3.8':'a_star.cp38-win_amd64.pyd',
-                            '3.9':'a_star.cp37-win_amd64.pyd',
-                            '3.10':'a_star.cp310-win_amd64.pyd'},
-                'macos'  :{ '3.7':'a_star.cpython-37m-darwin.so',
-                            '3.8':'a_star.cpython-38-darwin.so',
-                            '3.9':'a_star.cpython-39-darwin.so'},
-                'ubuntu' :{ '3.7':'a_star.cpython-37m-x86_64-linux-gnu.so',
-                            '3.8':'a_star.cpython-38-x86_64-linux-gnu.so',
-                            '3.9':'a_star.cpython-39-x86_64-linux-gnu.so'}}
-    print("using ",filename)
-    dynamic_link = filename[os_version][python_version]
-    if not os.path.exists(os.path.join(NAME,dynamic_link)):
-        if os_version == 'windows':
-            unzip_file(os.path.join(NAME,'lib/a_star.zip'),os.path.join(NAME,'lib'))
+
+
+class CustomBdistWheelCommand(_bdist_wheel):
+    def run(self):
+        # Call the original run() method
+        _bdist_wheel.run(self)
+
+    def unzip_file(self, zip_file_path, extract_folder_path):
+        with zipfile.ZipFile(zip_file_path, 'r') as zipObj:
+            zipObj.extractall(extract_folder_path)
+
+    def untar_file(self, tar_file_path, extract_folder_path):
+        with tarfile.open(tar_file_path, 'r:gz') as tarObj:
+            tarObj.extractall(extract_folder_path)
+
+    def get_os_and_python_version(self):
+        system = platform.system()
+        python_version = ".".join(map(str, sys.version_info[:2]))
+        if system.lower() == "windows":
+            os_version = "windows"
+        elif system.lower() == "darwin":
+            os_version = "macos"
+        elif system.lower() == "linux":
+            os_version = distro.name().lower()
+        else:
+            raise ValueError("Unknown System")
+        if (os_version == 'windows'):
+            if (python_version == '3.11'):
+                python_version = '3.10'
         else:
-            untar_file(os.path.join(NAME,'lib/a_star.tar.gz'),os.path.join(NAME,'lib'))
-        shutil.copy2(os.path.join(NAME,'lib',dynamic_link), NAME)
+            if (python_version == '3.10') or (python_version == '3.11'):
+                python_version = '3.9'
+        return os_version, python_version
+        
+    def add_dynamic_link(self):
+        print("Detect OS Version...")
+        os_version, python_version = self.get_os_and_python_version()
+        print("OS Version: ",os_version)
+        filename={  'windows':{ '3.7':'a_star.cp37-win_amd64.pyd',
+                                '3.8':'a_star.cp38-win_amd64.pyd',
+                                '3.9':'a_star.cp37-win_amd64.pyd',
+                                '3.10':'a_star.cp310-win_amd64.pyd'},
+                    'macos'  :{ '3.7':'a_star.cpython-37m-darwin.so',
+                                '3.8':'a_star.cpython-38-darwin.so',
+                                '3.9':'a_star.cpython-39-darwin.so'},
+                    'ubuntu' :{ '3.7':'a_star.cpython-37m-x86_64-linux-gnu.so',
+                                '3.8':'a_star.cpython-38-x86_64-linux-gnu.so',
+                                '3.9':'a_star.cpython-39-x86_64-linux-gnu.so'}}
+        dynamic_link = filename[os_version][python_version]
+        print("using ",dynamic_link)
+        print('abs:',os.path.abspath(os.path.join(NAME,dynamic_link)))
+        if not os.path.exists(os.path.join(NAME,dynamic_link)):
+            print("copying ",dynamic_link)
+            if os_version == 'windows':
+                self.unzip_file(os.path.join(NAME,'lib','a_star.zip'),os.path.join(NAME,'lib'))
+            else:
+                self.untar_file(os.path.join(NAME,'lib/a_star.tar.gz'),os.path.join(NAME,'lib'))
+            shutil.copy2(os.path.join(NAME,'lib',dynamic_link), NAME) 
+            print("copying from {} to {}".format(os.path.join(NAME,'lib',dynamic_link),NAME))
 
-class PostInstallCommand(install):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        atexit.register(post_install)
 
+             
 class UploadCommand(Command):
     """Support setup.py upload."""
 
     description = 'Build and publish the package.'
     user_options = []
 
     @staticmethod
@@ -153,29 +158,29 @@
     version=about['__version__'],
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     author=AUTHOR,
     url=URL,
     packages=find_packages(exclude=["tests", "*.tests", "*.tests.*", "tests.*"]),
-    package_data={NAME: ['lib/*.zip', 'lib/*.tar.gz']},
+    package_data={NAME: ['lib/*', '*.pyd', '*.so']},
     install_requires=REQUIRED,
     extras_require=EXTRAS,
     include_package_data=True,
     license='Mulan PSL v2',
     python_requires='>=3.7',
-    classifiers=(
+    classifiers=[
         'License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)',
         'Programming Language :: Python :: 3 :: Only',
         'Operating System :: OS Independent',
         'Environment :: GPU :: NVIDIA CUDA',
         'Environment :: Console',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Topic :: Scientific/Engineering :: Image Recognition',
         'Topic :: Scientific/Engineering :: Mathematics',
-    ),
+    ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
-        'install': PostInstallCommand,
+        'bdist_wheel': CustomBdistWheelCommand,
     },
 )
```

### Comparing `pygmtools-0.3.8a8/tests/test_classic_solvers.py` & `pygmtools-0.3.8a9/tests/test_classic_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/tests/test_dataset.py` & `pygmtools-0.3.8a9/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/tests/test_misc.py` & `pygmtools-0.3.8a9/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/tests/test_multi_graph_solvers.py` & `pygmtools-0.3.8a9/tests/test_multi_graph_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/tests/test_neural_solvers.py` & `pygmtools-0.3.8a9/tests/test_neural_solvers.py`

 * *Files identical despite different names*

### Comparing `pygmtools-0.3.8a8/tests/test_utils.py` & `pygmtools-0.3.8a9/tests/test_utils.py`

 * *Files identical despite different names*

