# Comparing `tmp/profiling-helpers-0.1.0.tar.gz` & `tmp/profiling-helpers-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "profiling-helpers-0.1.0.tar", last modified: Thu Jul 14 11:46:37 2022, max compression
+gzip compressed data, was "profiling-helpers-0.2.0.tar", last modified: Tue Jul 18 06:54:03 2023, max compression
```

## Comparing `profiling-helpers-0.1.0.tar` & `profiling-helpers-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 11:46:37.249715 profiling-helpers-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-07-14 11:46:25.000000 profiling-helpers-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-07-14 11:46:37.249715 profiling-helpers-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1024 2022-07-14 11:46:25.000000 profiling-helpers-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       81 2022-07-14 11:46:25.000000 profiling-helpers-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-07-14 11:46:37.253715 profiling-helpers-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 11:46:37.249715 profiling-helpers-0.1.0/src/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-07-14 11:46:25.000000 profiling-helpers-0.1.0/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 11:46:37.249715 profiling-helpers-0.1.0/src/profiling_helpers/
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-07-14 11:46:25.000000 profiling-helpers-0.1.0/src/profiling_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2246 2022-07-14 11:46:25.000000 profiling-helpers-0.1.0/src/profiling_helpers/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-14 11:46:37.249715 profiling-helpers-0.1.0/src/profiling_helpers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     1901 2022-07-14 11:46:37.000000 profiling-helpers-0.1.0/src/profiling_helpers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      351 2022-07-14 11:46:37.000000 profiling-helpers-0.1.0/src/profiling_helpers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-14 11:46:37.000000 profiling-helpers-0.1.0/src/profiling_helpers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-07-14 11:46:37.000000 profiling-helpers-0.1.0/src/profiling_helpers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2022-07-14 11:46:37.000000 profiling-helpers-0.1.0/src/profiling_helpers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:54:03.143578 profiling-helpers-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-07-18 06:53:49.000000 profiling-helpers-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-18 06:54:03.143578 profiling-helpers-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-18 06:53:49.000000 profiling-helpers-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-18 06:53:49.000000 profiling-helpers-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-18 06:54:03.143578 profiling-helpers-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:54:03.139578 profiling-helpers-0.2.0/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 06:53:49.000000 profiling-helpers-0.2.0/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:54:03.143578 profiling-helpers-0.2.0/src/profiling_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-18 06:53:49.000000 profiling-helpers-0.2.0/src/profiling_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3352 2023-07-18 06:53:49.000000 profiling-helpers-0.2.0/src/profiling_helpers/profiling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2970 2023-07-18 06:53:49.000000 profiling-helpers-0.2.0/src/profiling_helpers/save_targets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:54:03.143578 profiling-helpers-0.2.0/src/profiling_helpers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2457 2023-07-18 06:54:03.000000 profiling-helpers-0.2.0/src/profiling_helpers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-18 06:54:03.000000 profiling-helpers-0.2.0/src/profiling_helpers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 06:54:03.000000 profiling-helpers-0.2.0/src/profiling_helpers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-07-18 06:54:03.000000 profiling-helpers-0.2.0/src/profiling_helpers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-07-18 06:54:03.000000 profiling-helpers-0.2.0/src/profiling_helpers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 06:54:03.143578 profiling-helpers-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-18 06:53:49.000000 profiling-helpers-0.2.0/tests/test_profiling.py
```

### Comparing `profiling-helpers-0.1.0/LICENSE` & `profiling-helpers-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `profiling-helpers-0.1.0/PKG-INFO` & `profiling-helpers-0.2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: profiling-helpers
-Version: 0.1.0
+Version: 0.2.0
 Summary: A small utility library that wraps cProfile and makes it easy to debug performance problems in your Python code.
 Home-page: https://github.com/NobisIndustries/python-profiling-helpers
 Author: Fabian Nobis
 Author-email: fabiannobis@gmx.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/NobisIndustries/python-profiling-helpers/issues
 Keywords: cProfile,profiling,performance
 Platform: any
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: aws
 Provides-Extra: dev
 License-File: LICENSE
 
 # Profiling Helpers
 
 A small python package that wraps Python's own `cProfile` library to make it more user friendly.
 
 
 When developing Python programs, you'll sometimes have functions that take a long time to execute and
 you are really not sure why. Profiling helps to find and analyze these bottlenecks and guides you
 into fixing performance problems. Uses [snakeviz](https://jiffyclub.github.io/snakeviz/) for interactive visualizations.
 
 Install it with `pip install profiling-helpers`.
+Visualize profile files with `snakeviz profile_xyz.prof`.
 
 There are two decorators, `time_it` and `profile_it`. Use them anywhere in your code, like this:
 
 ```python
 from profiling_helpers import time_it, profile_it
 from time import sleep
 
@@ -50,7 +52,22 @@
 @profile_it("my/profile/save/dir", open_visualization=True)
 def my_slow_function(x):
     sleep(10)
     return x
 
 my_slow_function(42)  # Opens snakeviz after this function is completed
 ```
+
+Profiles are normally saved on the local file system. If you have other save targets, you can
+either use included FileSavers (currently only for AWS S3) or implement your own one by inheriting
+from the `BaseFileSaver` class. Here is a variant with S3:
+
+```python
+from profiling_helpers import profile_it, S3FileSaver
+
+@profile_it(S3FileSaver("s3://my-bucket/my/path/to/profiles/", kms_key_id="..."))
+def my_slow_function(x):
+    sleep(10)
+    return x
+
+my_slow_function(42)
+```
```

### Comparing `profiling-helpers-0.1.0/README.md` & `profiling-helpers-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 
 When developing Python programs, you'll sometimes have functions that take a long time to execute and
 you are really not sure why. Profiling helps to find and analyze these bottlenecks and guides you
 into fixing performance problems. Uses [snakeviz](https://jiffyclub.github.io/snakeviz/) for interactive visualizations.
 
 Install it with `pip install profiling-helpers`.
+Visualize profile files with `snakeviz profile_xyz.prof`.
 
 There are two decorators, `time_it` and `profile_it`. Use them anywhere in your code, like this:
 
 ```python
 from profiling_helpers import time_it, profile_it
 from time import sleep
 
@@ -28,7 +29,22 @@
 @profile_it("my/profile/save/dir", open_visualization=True)
 def my_slow_function(x):
     sleep(10)
     return x
 
 my_slow_function(42)  # Opens snakeviz after this function is completed
 ```
+
+Profiles are normally saved on the local file system. If you have other save targets, you can
+either use included FileSavers (currently only for AWS S3) or implement your own one by inheriting
+from the `BaseFileSaver` class. Here is a variant with S3:
+
+```python
+from profiling_helpers import profile_it, S3FileSaver
+
+@profile_it(S3FileSaver("s3://my-bucket/my/path/to/profiles/", kms_key_id="..."))
+def my_slow_function(x):
+    sleep(10)
+    return x
+
+my_slow_function(42)
+```
```

### Comparing `profiling-helpers-0.1.0/setup.cfg` & `profiling-helpers-0.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [metadata]
 name = profiling-helpers
-version = 0.1.0
+version = 0.2.0
 author = Fabian Nobis
 author_email = fabiannobis@gmx.de
 url = https://github.com/NobisIndustries/python-profiling-helpers
 description = A small utility library that wraps cProfile and makes it easy to debug performance problems in your Python code.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_file = LICENSE
 platform = any
 keywords = cProfile, profiling, performance
 classifiers = 
-	Development Status :: 3 - Alpha
+	Development Status :: 4 - Beta
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Topic :: Software Development :: Libraries :: Python Modules
 project_urls = 
 	Bug Tracker = https://github.com/NobisIndustries/python-profiling-helpers/issues
@@ -25,14 +25,16 @@
 package_dir = 
 	= src
 python_requires = >=3.7
 install_requires = 
 	snakeviz>=2.1.1
 
 [options.extras_require]
+aws = 
+	boto3>=1.28.0
 dev = 
 	pre-commit
 	build
 	pytest
 
 [bdist_wheel]
 universal = true
```

### Comparing `profiling-helpers-0.1.0/src/profiling_helpers.egg-info/PKG-INFO` & `profiling-helpers-0.2.0/src/profiling_helpers.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,41 @@
 Metadata-Version: 2.1
 Name: profiling-helpers
-Version: 0.1.0
+Version: 0.2.0
 Summary: A small utility library that wraps cProfile and makes it easy to debug performance problems in your Python code.
 Home-page: https://github.com/NobisIndustries/python-profiling-helpers
 Author: Fabian Nobis
 Author-email: fabiannobis@gmx.de
 License: MIT
 Project-URL: Bug Tracker, https://github.com/NobisIndustries/python-profiling-helpers/issues
 Keywords: cProfile,profiling,performance
 Platform: any
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
+Provides-Extra: aws
 Provides-Extra: dev
 License-File: LICENSE
 
 # Profiling Helpers
 
 A small python package that wraps Python's own `cProfile` library to make it more user friendly.
 
 
 When developing Python programs, you'll sometimes have functions that take a long time to execute and
 you are really not sure why. Profiling helps to find and analyze these bottlenecks and guides you
 into fixing performance problems. Uses [snakeviz](https://jiffyclub.github.io/snakeviz/) for interactive visualizations.
 
 Install it with `pip install profiling-helpers`.
+Visualize profile files with `snakeviz profile_xyz.prof`.
 
 There are two decorators, `time_it` and `profile_it`. Use them anywhere in your code, like this:
 
 ```python
 from profiling_helpers import time_it, profile_it
 from time import sleep
 
@@ -50,7 +52,22 @@
 @profile_it("my/profile/save/dir", open_visualization=True)
 def my_slow_function(x):
     sleep(10)
     return x
 
 my_slow_function(42)  # Opens snakeviz after this function is completed
 ```
+
+Profiles are normally saved on the local file system. If you have other save targets, you can
+either use included FileSavers (currently only for AWS S3) or implement your own one by inheriting
+from the `BaseFileSaver` class. Here is a variant with S3:
+
+```python
+from profiling_helpers import profile_it, S3FileSaver
+
+@profile_it(S3FileSaver("s3://my-bucket/my/path/to/profiles/", kms_key_id="..."))
+def my_slow_function(x):
+    sleep(10)
+    return x
+
+my_slow_function(42)
+```
```

