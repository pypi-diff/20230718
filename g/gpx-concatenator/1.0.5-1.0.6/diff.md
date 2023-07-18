# Comparing `tmp/gpx-concatenator-1.0.5.tar.gz` & `tmp/gpx-concatenator-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpx-concatenator-1.0.5.tar", last modified: Tue Jul 11 22:39:28 2023, max compression
+gzip compressed data, was "gpx-concatenator-1.0.6.tar", last modified: Tue Jul 18 21:20:21 2023, max compression
```

## Comparing `gpx-concatenator-1.0.5.tar` & `gpx-concatenator-1.0.6.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 22:39:28.556841 gpx-concatenator-1.0.5/
--rw-r--r--   0 teolebras   (501) staff       (20)     1070 2023-07-09 14:10:22.000000 gpx-concatenator-1.0.5/LICENSE
--rw-r--r--   0 teolebras   (501) staff       (20)     3822 2023-07-11 22:39:28.555911 gpx-concatenator-1.0.5/PKG-INFO
--rw-r--r--   0 teolebras   (501) staff       (20)     3602 2023-07-11 21:07:45.000000 gpx-concatenator-1.0.5/README.md
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 22:39:28.540431 gpx-concatenator-1.0.5/gpx_concatenator/
--rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:20.000000 gpx-concatenator-1.0.5/gpx_concatenator/__init__.py
--rw-r--r--   0 teolebras   (501) staff       (20)     3801 2023-07-09 12:34:30.000000 gpx-concatenator-1.0.5/gpx_concatenator/gpx_colorizer.py
--rw-r--r--   0 teolebras   (501) staff       (20)     2646 2023-07-09 14:03:22.000000 gpx-concatenator-1.0.5/gpx_concatenator/gpx_concatenator.py
--rw-r--r--   0 teolebras   (501) staff       (20)     1071 2023-07-09 12:34:30.000000 gpx-concatenator-1.0.5/gpx_concatenator/gpx_file.py
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 22:39:28.552676 gpx-concatenator-1.0.5/gpx_concatenator/tests/
--rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 15:24:44.000000 gpx-concatenator-1.0.5/gpx_concatenator/tests/__init__.py
--rw-r--r--   0 teolebras   (501) staff       (20)     2204 2023-07-09 15:22:39.000000 gpx-concatenator-1.0.5/gpx_concatenator/tests/gpx_colorizer_test.py
--rw-r--r--   0 teolebras   (501) staff       (20)      870 2023-07-09 15:37:16.000000 gpx-concatenator-1.0.5/gpx_concatenator/tests/gpx_file_test.py
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 22:39:28.550284 gpx-concatenator-1.0.5/gpx_concatenator.egg-info/
--rw-r--r--   0 teolebras   (501) staff       (20)     3822 2023-07-11 22:39:28.000000 gpx-concatenator-1.0.5/gpx_concatenator.egg-info/PKG-INFO
--rw-r--r--   0 teolebras   (501) staff       (20)      514 2023-07-11 22:39:28.000000 gpx-concatenator-1.0.5/gpx_concatenator.egg-info/SOURCES.txt
--rw-r--r--   0 teolebras   (501) staff       (20)        1 2023-07-11 22:39:28.000000 gpx-concatenator-1.0.5/gpx_concatenator.egg-info/dependency_links.txt
--rw-r--r--   0 teolebras   (501) staff       (20)       55 2023-07-11 22:39:28.000000 gpx-concatenator-1.0.5/gpx_concatenator.egg-info/entry_points.txt
--rw-r--r--   0 teolebras   (501) staff       (20)       25 2023-07-11 22:39:28.000000 gpx-concatenator-1.0.5/gpx_concatenator.egg-info/top_level.txt
-drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-11 22:39:28.554269 gpx-concatenator-1.0.5/scripts/
--rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:26.000000 gpx-concatenator-1.0.5/scripts/__init__.py
--rw-r--r--   0 teolebras   (501) staff       (20)     1426 2023-07-11 22:39:11.000000 gpx-concatenator-1.0.5/scripts/main.py
--rw-r--r--   0 teolebras   (501) staff       (20)       38 2023-07-11 22:39:28.557203 gpx-concatenator-1.0.5/setup.cfg
--rw-r--r--   0 teolebras   (501) staff       (20)      585 2023-07-11 22:39:16.000000 gpx-concatenator-1.0.5/setup.py
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-18 21:20:21.953539 gpx-concatenator-1.0.6/
+-rw-r--r--   0 teolebras   (501) staff       (20)     1070 2023-07-09 14:10:22.000000 gpx-concatenator-1.0.6/LICENSE
+-rw-r--r--   0 teolebras   (501) staff       (20)     3822 2023-07-18 21:20:21.951301 gpx-concatenator-1.0.6/PKG-INFO
+-rw-r--r--   0 teolebras   (501) staff       (20)     3602 2023-07-11 21:07:45.000000 gpx-concatenator-1.0.6/README.md
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-18 21:20:21.937881 gpx-concatenator-1.0.6/gpx_concatenator/
+-rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:20.000000 gpx-concatenator-1.0.6/gpx_concatenator/__init__.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     3801 2023-07-09 12:34:30.000000 gpx-concatenator-1.0.6/gpx_concatenator/gpx_colorizer.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     2646 2023-07-09 14:03:22.000000 gpx-concatenator-1.0.6/gpx_concatenator/gpx_concatenator.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     1071 2023-07-09 12:34:30.000000 gpx-concatenator-1.0.6/gpx_concatenator/gpx_file.py
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-18 21:20:21.948898 gpx-concatenator-1.0.6/gpx_concatenator/tests/
+-rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 15:24:44.000000 gpx-concatenator-1.0.6/gpx_concatenator/tests/__init__.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     2204 2023-07-09 15:22:39.000000 gpx-concatenator-1.0.6/gpx_concatenator/tests/gpx_colorizer_test.py
+-rw-r--r--   0 teolebras   (501) staff       (20)      870 2023-07-09 15:37:16.000000 gpx-concatenator-1.0.6/gpx_concatenator/tests/gpx_file_test.py
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-18 21:20:21.945885 gpx-concatenator-1.0.6/gpx_concatenator.egg-info/
+-rw-r--r--   0 teolebras   (501) staff       (20)     3822 2023-07-18 21:20:21.000000 gpx-concatenator-1.0.6/gpx_concatenator.egg-info/PKG-INFO
+-rw-r--r--   0 teolebras   (501) staff       (20)      514 2023-07-18 21:20:21.000000 gpx-concatenator-1.0.6/gpx_concatenator.egg-info/SOURCES.txt
+-rw-r--r--   0 teolebras   (501) staff       (20)        1 2023-07-18 21:20:21.000000 gpx-concatenator-1.0.6/gpx_concatenator.egg-info/dependency_links.txt
+-rw-r--r--   0 teolebras   (501) staff       (20)       55 2023-07-18 21:20:21.000000 gpx-concatenator-1.0.6/gpx_concatenator.egg-info/entry_points.txt
+-rw-r--r--   0 teolebras   (501) staff       (20)       25 2023-07-18 21:20:21.000000 gpx-concatenator-1.0.6/gpx_concatenator.egg-info/top_level.txt
+drwxr-xr-x   0 teolebras   (501) staff       (20)        0 2023-07-18 21:20:21.950583 gpx-concatenator-1.0.6/scripts/
+-rw-r--r--   0 teolebras   (501) staff       (20)        0 2023-07-09 14:02:26.000000 gpx-concatenator-1.0.6/scripts/__init__.py
+-rw-r--r--   0 teolebras   (501) staff       (20)     1432 2023-07-18 21:18:54.000000 gpx-concatenator-1.0.6/scripts/main.py
+-rw-r--r--   0 teolebras   (501) staff       (20)       38 2023-07-18 21:20:21.953680 gpx-concatenator-1.0.6/setup.cfg
+-rw-r--r--   0 teolebras   (501) staff       (20)      585 2023-07-18 21:20:16.000000 gpx-concatenator-1.0.6/setup.py
```

### Comparing `gpx-concatenator-1.0.5/LICENSE` & `gpx-concatenator-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.5/PKG-INFO` & `gpx-concatenator-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpx-concatenator
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tool for concatenating GPX files
 Author: iambrianna
 Author-email: iambrianna@proton.me
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GPX Concatenator
```

### Comparing `gpx-concatenator-1.0.5/README.md` & `gpx-concatenator-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.5/gpx_concatenator/gpx_colorizer.py` & `gpx-concatenator-1.0.6/gpx_concatenator/gpx_colorizer.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.5/gpx_concatenator/gpx_concatenator.py` & `gpx-concatenator-1.0.6/gpx_concatenator/gpx_concatenator.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.5/gpx_concatenator/gpx_file.py` & `gpx-concatenator-1.0.6/gpx_concatenator/gpx_file.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.5/gpx_concatenator/tests/gpx_colorizer_test.py` & `gpx-concatenator-1.0.6/gpx_concatenator/tests/gpx_colorizer_test.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.5/gpx_concatenator/tests/gpx_file_test.py` & `gpx-concatenator-1.0.6/gpx_concatenator/tests/gpx_file_test.py`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.5/gpx_concatenator.egg-info/PKG-INFO` & `gpx-concatenator-1.0.6/gpx_concatenator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gpx-concatenator
-Version: 1.0.5
+Version: 1.0.6
 Summary: Tool for concatenating GPX files
 Author: iambrianna
 Author-email: iambrianna@proton.me
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # GPX Concatenator
```

### Comparing `gpx-concatenator-1.0.5/gpx_concatenator.egg-info/SOURCES.txt` & `gpx-concatenator-1.0.6/gpx_concatenator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gpx-concatenator-1.0.5/scripts/main.py` & `gpx-concatenator-1.0.6/scripts/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import argparse
 from gpx_concatenator.gpx_concatenator import GPXConcatenator
 import argcomplete
 
 def main():
     # Create an argument parser
     parser = argparse.ArgumentParser(description='GPX Concatenator')
-    parser.add_argument('-i', '--input-dir', default='input', help='Directory containing input files', type=argcomplete.completers.DirectoriesCompleter())
+    parser.add_argument('-i', '--input-dir', default='input', help='Directory containing input files').completer = argcomplete.completers.DirectoriesCompleter()
     parser.add_argument('-o', '--output-file', default='output.gpx', help='Output file name', type=argparse.FileType('w'))
     parser.add_argument('-m', '--enable-metadata', action='store_true', help='Enable metadata in the output file')
     parser.add_argument('-c', '--enable-coloring', action='store_true', help='Enable coloring in the output file')
 
     # Activate autocompletion for paths
     argcomplete.autocomplete(parser)
```

### Comparing `gpx-concatenator-1.0.5/setup.py` & `gpx-concatenator-1.0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='gpx-concatenator',
-    version='1.0.5',
+    version='1.0.6',
     description='Tool for concatenating GPX files',
     author='iambrianna',
     author_email='iambrianna@proton.me',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'gpx-concatenator = scripts.main:main',
```

