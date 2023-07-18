# Comparing `tmp/voxtool-0.0.1.tar.gz` & `tmp/voxtool-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "voxtool-0.0.1.tar", last modified: Tue Jul 18 13:47:59 2023, max compression
+gzip compressed data, was "voxtool-0.0.2.tar", last modified: Tue Jul 18 14:13:07 2023, max compression
```

## Comparing `voxtool-0.0.1.tar` & `voxtool-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-07-18 13:47:59.039379 voxtool-0.0.1/
--rw-r--r--   0 allucas    (501) staff       (20)     2887 2023-07-18 13:47:59.039246 voxtool-0.0.1/PKG-INFO
--rw-r--r--   0 allucas    (501) staff       (20)     2668 2023-07-17 20:44:12.000000 voxtool-0.0.1/README.md
--rw-r--r--   0 allucas    (501) staff       (20)       38 2023-07-18 13:47:59.039418 voxtool-0.0.1/setup.cfg
--rw-r--r--   0 allucas    (501) staff       (20)      696 2023-07-18 13:47:08.000000 voxtool-0.0.1/setup.py
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-07-18 13:47:59.037249 voxtool-0.0.1/voxtool/
--rw-r--r--   0 allucas    (501) staff       (20)        0 2023-07-18 12:49:14.000000 voxtool-0.0.1/voxtool/__init__.py
--rw-r--r--   0 allucas    (501) staff       (20)     1603 2023-07-17 20:44:12.000000 voxtool-0.0.1/voxtool/config.yml
--rw-r--r--   0 allucas    (501) staff       (20)      437 2023-07-18 13:41:29.000000 voxtool-0.0.1/voxtool/launch_pyloc.py
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-07-18 13:47:59.038402 voxtool-0.0.1/voxtool/model/
--rw-r--r--   0 allucas    (501) staff       (20)       20 2023-07-17 20:44:12.000000 voxtool-0.0.1/voxtool/model/__init__.py
--rw-r--r--   0 allucas    (501) staff       (20)    13666 2023-07-17 20:44:53.000000 voxtool-0.0.1/voxtool/model/interpolator.py
--rw-r--r--   0 allucas    (501) staff       (20)    30444 2023-07-17 20:44:53.000000 voxtool-0.0.1/voxtool/model/scan.py
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-07-18 13:47:59.039041 voxtool-0.0.1/voxtool/view/
--rw-r--r--   0 allucas    (501) staff       (20)       20 2023-07-17 20:44:12.000000 voxtool-0.0.1/voxtool/view/__init__.py
--rw-r--r--   0 allucas    (501) staff       (20)      477 2023-07-17 20:44:12.000000 voxtool-0.0.1/voxtool/view/pointcloud_viewer.py
--rw-r--r--   0 allucas    (501) staff       (20)    40060 2023-07-18 13:13:22.000000 voxtool-0.0.1/voxtool/view/pyloc.py
--rw-r--r--   0 allucas    (501) staff       (20)     4425 2023-07-17 20:44:53.000000 voxtool-0.0.1/voxtool/view/slice_viewer.py
-drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-07-18 13:47:59.037983 voxtool-0.0.1/voxtool.egg-info/
--rw-r--r--   0 allucas    (501) staff       (20)     2887 2023-07-18 13:47:58.000000 voxtool-0.0.1/voxtool.egg-info/PKG-INFO
--rw-r--r--   0 allucas    (501) staff       (20)      457 2023-07-18 13:47:59.000000 voxtool-0.0.1/voxtool.egg-info/SOURCES.txt
--rw-r--r--   0 allucas    (501) staff       (20)        1 2023-07-18 13:47:58.000000 voxtool-0.0.1/voxtool.egg-info/dependency_links.txt
--rw-r--r--   0 allucas    (501) staff       (20)       54 2023-07-18 13:47:58.000000 voxtool-0.0.1/voxtool.egg-info/entry_points.txt
--rw-r--r--   0 allucas    (501) staff       (20)       67 2023-07-18 13:47:58.000000 voxtool-0.0.1/voxtool.egg-info/requires.txt
--rw-r--r--   0 allucas    (501) staff       (20)        8 2023-07-18 13:47:58.000000 voxtool-0.0.1/voxtool.egg-info/top_level.txt
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-07-18 14:13:07.742457 voxtool-0.0.2/
+-rw-r--r--   0 allucas    (501) staff       (20)     3063 2023-07-18 14:13:07.742317 voxtool-0.0.2/PKG-INFO
+-rw-r--r--   0 allucas    (501) staff       (20)     2845 2023-07-18 14:12:13.000000 voxtool-0.0.2/README.md
+-rw-r--r--   0 allucas    (501) staff       (20)       38 2023-07-18 14:13:07.742506 voxtool-0.0.2/setup.cfg
+-rw-r--r--   0 allucas    (501) staff       (20)      695 2023-07-18 14:13:01.000000 voxtool-0.0.2/setup.py
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-07-18 14:13:07.738777 voxtool-0.0.2/voxtool/
+-rw-r--r--   0 allucas    (501) staff       (20)        0 2023-07-18 12:49:14.000000 voxtool-0.0.2/voxtool/__init__.py
+-rw-r--r--   0 allucas    (501) staff       (20)     1603 2023-07-17 20:44:12.000000 voxtool-0.0.2/voxtool/config.yml
+-rw-r--r--   0 allucas    (501) staff       (20)      437 2023-07-18 13:41:29.000000 voxtool-0.0.2/voxtool/launch_pyloc.py
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-07-18 14:13:07.740339 voxtool-0.0.2/voxtool/model/
+-rw-r--r--   0 allucas    (501) staff       (20)       20 2023-07-17 20:44:12.000000 voxtool-0.0.2/voxtool/model/__init__.py
+-rw-r--r--   0 allucas    (501) staff       (20)    13666 2023-07-17 20:44:53.000000 voxtool-0.0.2/voxtool/model/interpolator.py
+-rw-r--r--   0 allucas    (501) staff       (20)    30444 2023-07-17 20:44:53.000000 voxtool-0.0.2/voxtool/model/scan.py
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-07-18 14:13:07.742118 voxtool-0.0.2/voxtool/view/
+-rw-r--r--   0 allucas    (501) staff       (20)       20 2023-07-17 20:44:12.000000 voxtool-0.0.2/voxtool/view/__init__.py
+-rw-r--r--   0 allucas    (501) staff       (20)      477 2023-07-17 20:44:12.000000 voxtool-0.0.2/voxtool/view/pointcloud_viewer.py
+-rw-r--r--   0 allucas    (501) staff       (20)    40060 2023-07-18 13:13:22.000000 voxtool-0.0.2/voxtool/view/pyloc.py
+-rw-r--r--   0 allucas    (501) staff       (20)     4425 2023-07-17 20:44:53.000000 voxtool-0.0.2/voxtool/view/slice_viewer.py
+drwxr-xr-x   0 allucas    (501) staff       (20)        0 2023-07-18 14:13:07.739480 voxtool-0.0.2/voxtool.egg-info/
+-rw-r--r--   0 allucas    (501) staff       (20)     3063 2023-07-18 14:13:07.000000 voxtool-0.0.2/voxtool.egg-info/PKG-INFO
+-rw-r--r--   0 allucas    (501) staff       (20)      457 2023-07-18 14:13:07.000000 voxtool-0.0.2/voxtool.egg-info/SOURCES.txt
+-rw-r--r--   0 allucas    (501) staff       (20)        1 2023-07-18 14:13:07.000000 voxtool-0.0.2/voxtool.egg-info/dependency_links.txt
+-rw-r--r--   0 allucas    (501) staff       (20)       54 2023-07-18 14:13:07.000000 voxtool-0.0.2/voxtool.egg-info/entry_points.txt
+-rw-r--r--   0 allucas    (501) staff       (20)       67 2023-07-18 14:13:07.000000 voxtool-0.0.2/voxtool.egg-info/requires.txt
+-rw-r--r--   0 allucas    (501) staff       (20)        8 2023-07-18 14:13:07.000000 voxtool-0.0.2/voxtool.egg-info/top_level.txt
```

### Comparing `voxtool-0.0.1/PKG-INFO` & `voxtool-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 Metadata-Version: 2.1
 Name: voxtool
-Version: 0.0.1
+Version: 0.0.2
 Summary: VoxTool: A tool for labeling intracranial electrodes on CT images
-Home-page: https://github.com/your_username/voxtool
+Home-page: https://github.com/penn-cnt/ieeg-recon/
 Description-Content-Type: text/markdown
 
 # VoxTool 2.0
 
 
 ## Setup
 
-- Clone the repository from GitHub
-- Create a Conda environment from the definition file
+To install VoxTool, simply do:
+
+```
+pip install voxtool
+```
+
+We recommend using voxtool within a virtual environment. If you have anaconda installed, you can do:
+
   ```
-  conda env install -f conda_env.yml
+  conda create -n vt
   ```
-  This creates an environment named `vt` in which to run voxTool.
+
+This creates an environment named `vt` in which to run voxTool. You can then install VoxTool within that environment by doing:
+
+```
+conda activate vt
+pip install voxtool
+```
 
 ## Running
 
-- Activate the conda environment:
-  ```
-  source activate vt
-  ```
-- Launch the program:
-  ```
-  python launch_pyloc.py
-  ```
+Inside the environment where VoxTool is installed, type in the terminal:
+
+```
+voxtool
+``` 
+
+This will bring up the main VoxTool window.
 
 ## Usage
 0. Load a CT file, adjusting the threshold as necessary. To adjust the
    threshold, change the number in the bar at the top of the window
    marked ```CT Threshold```, then press the ```Update``` button next to it.
 1. If continuing a previous localization: load the existing coordinates
    from a JSON coordinate file using the ```Load Coordinates``` button.
```

### Comparing `voxtool-0.0.1/README.md` & `voxtool-0.0.2/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 # VoxTool 2.0
 
 
 ## Setup
 
-- Clone the repository from GitHub
-- Create a Conda environment from the definition file
+To install VoxTool, simply do:
+
+```
+pip install voxtool
+```
+
+We recommend using voxtool within a virtual environment. If you have anaconda installed, you can do:
+
   ```
-  conda env install -f conda_env.yml
+  conda create -n vt
   ```
-  This creates an environment named `vt` in which to run voxTool.
+
+This creates an environment named `vt` in which to run voxTool. You can then install VoxTool within that environment by doing:
+
+```
+conda activate vt
+pip install voxtool
+```
 
 ## Running
 
-- Activate the conda environment:
-  ```
-  source activate vt
-  ```
-- Launch the program:
-  ```
-  python launch_pyloc.py
-  ```
+Inside the environment where VoxTool is installed, type in the terminal:
+
+```
+voxtool
+``` 
+
+This will bring up the main VoxTool window.
 
 ## Usage
 0. Load a CT file, adjusting the threshold as necessary. To adjust the
    threshold, change the number in the bar at the top of the window
    marked ```CT Threshold```, then press the ```Update``` button next to it.
 1. If continuing a previous localization: load the existing coordinates
    from a JSON coordinate file using the ```Load Coordinates``` button.
```

### Comparing `voxtool-0.0.1/setup.py` & `voxtool-0.0.2/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup, find_packages
 
 setup(
     name='voxtool',
-    version='0.0.1',
+    version='0.0.2',
     description='VoxTool: A tool for labeling intracranial electrodes on CT images',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
-    url='https://github.com/your_username/voxtool',
+    url='https://github.com/penn-cnt/ieeg-recon/',
     install_requires=['PyQt5','mayavi', 'pyface', 'pandas', 'matplotlib', 'nibabel', 'nilearn', 'pyyaml','scipy'],
     packages=['voxtool', 'voxtool.model', 'voxtool.view'],
     include_package_data=True,
     package_data={'voxtool': ["config.yml"]},
     entry_points={
         'console_scripts': [
             'voxtool = voxtool.launch_pyloc:main'
```

### Comparing `voxtool-0.0.1/voxtool/config.yml` & `voxtool-0.0.2/voxtool/config.yml`

 * *Files identical despite different names*

### Comparing `voxtool-0.0.1/voxtool/model/interpolator.py` & `voxtool-0.0.2/voxtool/model/interpolator.py`

 * *Files identical despite different names*

### Comparing `voxtool-0.0.1/voxtool/model/scan.py` & `voxtool-0.0.2/voxtool/model/scan.py`

 * *Files identical despite different names*

### Comparing `voxtool-0.0.1/voxtool/view/pyloc.py` & `voxtool-0.0.2/voxtool/view/pyloc.py`

 * *Files identical despite different names*

### Comparing `voxtool-0.0.1/voxtool/view/slice_viewer.py` & `voxtool-0.0.2/voxtool/view/slice_viewer.py`

 * *Files identical despite different names*

### Comparing `voxtool-0.0.1/voxtool.egg-info/PKG-INFO` & `voxtool-0.0.2/voxtool.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 Metadata-Version: 2.1
 Name: voxtool
-Version: 0.0.1
+Version: 0.0.2
 Summary: VoxTool: A tool for labeling intracranial electrodes on CT images
-Home-page: https://github.com/your_username/voxtool
+Home-page: https://github.com/penn-cnt/ieeg-recon/
 Description-Content-Type: text/markdown
 
 # VoxTool 2.0
 
 
 ## Setup
 
-- Clone the repository from GitHub
-- Create a Conda environment from the definition file
+To install VoxTool, simply do:
+
+```
+pip install voxtool
+```
+
+We recommend using voxtool within a virtual environment. If you have anaconda installed, you can do:
+
   ```
-  conda env install -f conda_env.yml
+  conda create -n vt
   ```
-  This creates an environment named `vt` in which to run voxTool.
+
+This creates an environment named `vt` in which to run voxTool. You can then install VoxTool within that environment by doing:
+
+```
+conda activate vt
+pip install voxtool
+```
 
 ## Running
 
-- Activate the conda environment:
-  ```
-  source activate vt
-  ```
-- Launch the program:
-  ```
-  python launch_pyloc.py
-  ```
+Inside the environment where VoxTool is installed, type in the terminal:
+
+```
+voxtool
+``` 
+
+This will bring up the main VoxTool window.
 
 ## Usage
 0. Load a CT file, adjusting the threshold as necessary. To adjust the
    threshold, change the number in the bar at the top of the window
    marked ```CT Threshold```, then press the ```Update``` button next to it.
 1. If continuing a previous localization: load the existing coordinates
    from a JSON coordinate file using the ```Load Coordinates``` button.
```

