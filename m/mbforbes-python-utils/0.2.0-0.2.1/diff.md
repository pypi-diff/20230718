# Comparing `tmp/mbforbes_python_utils-0.2.0.tar.gz` & `tmp/mbforbes_python_utils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbforbes_python_utils-0.2.0.tar", last modified: Tue Jul 18 19:30:12 2023, max compression
+gzip compressed data, was "mbforbes_python_utils-0.2.1.tar", last modified: Tue Jul 18 19:31:23 2023, max compression
```

## Comparing `mbforbes_python_utils-0.2.0.tar` & `mbforbes_python_utils-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-18 19:30:12.500818 mbforbes_python_utils-0.2.0/
--rw-r--r--   0 max        (501) staff       (20)     1071 2023-07-18 19:17:23.000000 mbforbes_python_utils-0.2.0/LICENSE.txt
--rw-r--r--   0 max        (501) staff       (20)     1150 2023-07-18 19:30:12.500707 mbforbes_python_utils-0.2.0/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      855 2023-07-18 19:30:02.000000 mbforbes_python_utils-0.2.0/README.md
-drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-18 19:30:12.500558 mbforbes_python_utils-0.2.0/mbforbes_python_utils.egg-info/
--rw-r--r--   0 max        (501) staff       (20)     1150 2023-07-18 19:30:12.000000 mbforbes_python_utils-0.2.0/mbforbes_python_utils.egg-info/PKG-INFO
--rw-r--r--   0 max        (501) staff       (20)      235 2023-07-18 19:30:12.000000 mbforbes_python_utils-0.2.0/mbforbes_python_utils.egg-info/SOURCES.txt
--rw-r--r--   0 max        (501) staff       (20)        1 2023-07-18 19:30:12.000000 mbforbes_python_utils-0.2.0/mbforbes_python_utils.egg-info/dependency_links.txt
--rw-r--r--   0 max        (501) staff       (20)       22 2023-07-18 19:30:12.000000 mbforbes_python_utils-0.2.0/mbforbes_python_utils.egg-info/top_level.txt
--rw-r--r--   0 max        (501) staff       (20)     1340 2023-07-18 19:16:57.000000 mbforbes_python_utils-0.2.0/mbforbes_python_utils.py
--rw-r--r--   0 max        (501) staff       (20)       38 2023-07-18 19:30:12.500852 mbforbes_python_utils-0.2.0/setup.cfg
--rw-r--r--   0 max        (501) staff       (20)      425 2023-07-18 19:29:07.000000 mbforbes_python_utils-0.2.0/setup.py
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-18 19:31:23.085018 mbforbes_python_utils-0.2.1/
+-rw-r--r--   0 max        (501) staff       (20)     1071 2023-07-18 19:17:23.000000 mbforbes_python_utils-0.2.1/LICENSE.txt
+-rw-r--r--   0 max        (501) staff       (20)     1156 2023-07-18 19:31:23.084900 mbforbes_python_utils-0.2.1/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      861 2023-07-18 19:30:50.000000 mbforbes_python_utils-0.2.1/README.md
+drwxr-xr-x   0 max        (501) staff       (20)        0 2023-07-18 19:31:23.084744 mbforbes_python_utils-0.2.1/mbforbes_python_utils.egg-info/
+-rw-r--r--   0 max        (501) staff       (20)     1156 2023-07-18 19:31:23.000000 mbforbes_python_utils-0.2.1/mbforbes_python_utils.egg-info/PKG-INFO
+-rw-r--r--   0 max        (501) staff       (20)      235 2023-07-18 19:31:23.000000 mbforbes_python_utils-0.2.1/mbforbes_python_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 max        (501) staff       (20)        1 2023-07-18 19:31:23.000000 mbforbes_python_utils-0.2.1/mbforbes_python_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 max        (501) staff       (20)       22 2023-07-18 19:31:23.000000 mbforbes_python_utils-0.2.1/mbforbes_python_utils.egg-info/top_level.txt
+-rw-r--r--   0 max        (501) staff       (20)     1340 2023-07-18 19:16:57.000000 mbforbes_python_utils-0.2.1/mbforbes_python_utils.py
+-rw-r--r--   0 max        (501) staff       (20)       38 2023-07-18 19:31:23.085058 mbforbes_python_utils-0.2.1/setup.cfg
+-rw-r--r--   0 max        (501) staff       (20)      425 2023-07-18 19:31:14.000000 mbforbes_python_utils-0.2.1/setup.py
```

### Comparing `mbforbes_python_utils-0.2.0/LICENSE.txt` & `mbforbes_python_utils-0.2.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mbforbes_python_utils-0.2.0/PKG-INFO` & `mbforbes_python_utils-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbforbes_python_utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: Some tiny python utils so I can be lazier.
 Home-page: https://github.com/mbforbes/python-utils
 Author: Maxwell Forbes
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -18,15 +18,15 @@
 ```sh
 # Python 3 only (I'm using Python 3.7).
 pip install mbforbes_python_utils
 ```
 
 ## Usage
 
-```
+```python
 from mbforbes_python_utils import read, write, flatten
 
 # read() removes leading/trailing whitespace.
 contents = read("foo.txt")
 
 # write() creates intermediate directories if needed.
 # Pass `info_print = False` to disable printing.
```

### Comparing `mbforbes_python_utils-0.2.0/README.md` & `mbforbes_python_utils-0.2.1/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 ```sh
 # Python 3 only (I'm using Python 3.7).
 pip install mbforbes_python_utils
 ```
 
 ## Usage
 
-```
+```python
 from mbforbes_python_utils import read, write, flatten
 
 # read() removes leading/trailing whitespace.
 contents = read("foo.txt")
 
 # write() creates intermediate directories if needed.
 # Pass `info_print = False` to disable printing.
```

### Comparing `mbforbes_python_utils-0.2.0/mbforbes_python_utils.egg-info/PKG-INFO` & `mbforbes_python_utils-0.2.1/mbforbes_python_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbforbes-python-utils
-Version: 0.2.0
+Version: 0.2.1
 Summary: Some tiny python utils so I can be lazier.
 Home-page: https://github.com/mbforbes/python-utils
 Author: Maxwell Forbes
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
@@ -18,15 +18,15 @@
 ```sh
 # Python 3 only (I'm using Python 3.7).
 pip install mbforbes_python_utils
 ```
 
 ## Usage
 
-```
+```python
 from mbforbes_python_utils import read, write, flatten
 
 # read() removes leading/trailing whitespace.
 contents = read("foo.txt")
 
 # write() creates intermediate directories if needed.
 # Pass `info_print = False` to disable printing.
```

### Comparing `mbforbes_python_utils-0.2.0/mbforbes_python_utils.py` & `mbforbes_python_utils-0.2.1/mbforbes_python_utils.py`

 * *Files identical despite different names*

