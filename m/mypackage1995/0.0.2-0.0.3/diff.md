# Comparing `tmp/mypackage1995-0.0.2.tar.gz` & `tmp/mypackage1995-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypackage1995-0.0.2.tar", last modified: Tue Jul 18 13:59:20 2023, max compression
+gzip compressed data, was "mypackage1995-0.0.3.tar", last modified: Tue Jul 18 14:29:25 2023, max compression
```

## Comparing `mypackage1995-0.0.2.tar` & `mypackage1995-0.0.3.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 13:59:20.107354 mypackage1995-0.0.2/
--rw-rw-rw-   0        0        0        0 2023-07-18 10:53:22.000000 mypackage1995-0.0.2/LICENSE
--rw-rw-rw-   0        0        0     1135 2023-07-18 13:59:20.107354 mypackage1995-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      622 2023-07-18 11:18:00.000000 mypackage1995-0.0.2/README.md
--rw-rw-rw-   0        0        0      108 2023-07-18 10:57:17.000000 mypackage1995-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      652 2023-07-18 13:59:20.109903 mypackage1995-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-07-18 13:59:20.085232 mypackage1995-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-07-18 13:59:20.092862 mypackage1995-0.0.2/src/mypackage1995/
--rw-rw-rw-   0        0        0        0 2023-07-18 10:55:34.000000 mypackage1995-0.0.2/src/mypackage1995/__init__.py
--rw-rw-rw-   0        0        0      249 2023-07-18 13:57:19.000000 mypackage1995-0.0.2/src/mypackage1995/main.py
-drwxrwxrwx   0        0        0        0 2023-07-18 13:59:20.105846 mypackage1995-0.0.2/src/mypackage1995.egg-info/
--rw-rw-rw-   0        0        0     1135 2023-07-18 13:59:20.000000 mypackage1995-0.0.2/src/mypackage1995.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      262 2023-07-18 13:59:20.000000 mypackage1995-0.0.2/src/mypackage1995.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 13:59:20.000000 mypackage1995-0.0.2/src/mypackage1995.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-07-18 13:59:20.000000 mypackage1995-0.0.2/src/mypackage1995.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 14:29:25.225512 mypackage1995-0.0.3/
+-rw-rw-rw-   0        0        0        0 2023-07-18 10:53:22.000000 mypackage1995-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     1135 2023-07-18 14:29:25.226507 mypackage1995-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      622 2023-07-18 11:18:00.000000 mypackage1995-0.0.3/README.md
+-rw-rw-rw-   0        0        0      108 2023-07-18 10:57:17.000000 mypackage1995-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      652 2023-07-18 14:29:25.228505 mypackage1995-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 14:29:25.177509 mypackage1995-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 14:29:25.206416 mypackage1995-0.0.3/src/mypackage1995/
+-rw-rw-rw-   0        0        0        0 2023-07-18 10:55:34.000000 mypackage1995-0.0.3/src/mypackage1995/__init__.py
+-rw-rw-rw-   0        0        0      249 2023-07-18 13:57:19.000000 mypackage1995-0.0.3/src/mypackage1995/main.py
+-rw-rw-rw-   0        0        0      256 2023-07-18 14:22:14.000000 mypackage1995-0.0.3/src/mypackage1995/main2.py
+drwxrwxrwx   0        0        0        0 2023-07-18 14:29:25.222517 mypackage1995-0.0.3/src/mypackage1995.egg-info/
+-rw-rw-rw-   0        0        0     1135 2023-07-18 14:29:25.000000 mypackage1995-0.0.3/src/mypackage1995.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      317 2023-07-18 14:29:25.000000 mypackage1995-0.0.3/src/mypackage1995.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 14:29:25.000000 mypackage1995-0.0.3/src/mypackage1995.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-07-18 14:29:25.000000 mypackage1995-0.0.3/src/mypackage1995.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 14:29:25.224512 mypackage1995-0.0.3/tests/
+-rw-rw-rw-   0        0        0      174 2023-07-18 14:27:02.000000 mypackage1995-0.0.3/tests/test_mypackage1995.py
```

### Comparing `mypackage1995-0.0.2/PKG-INFO` & `mypackage1995-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypackage1995
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: jigar2099
 Author-email: jigarbhanderi@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `mypackage1995-0.0.2/README.md` & `mypackage1995-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `mypackage1995-0.0.2/setup.cfg` & `mypackage1995-0.0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 206d 7970 6163 6b61 6765 3139 3935   = mypackage1995
 00000020: 0d0a 7665 7273 696f 6e20 3d20 302e 302e  ..version = 0.0.
-00000030: 320d 0a61 7574 686f 7220 3d20 6a69 6761  2..author = jiga
+00000030: 330d 0a61 7574 686f 7220 3d20 6a69 6761  3..author = jiga
 00000040: 7232 3039 390d 0a61 7574 686f 725f 656d  r2099..author_em
 00000050: 6169 6c20 3d20 6a69 6761 7262 6861 6e64  ail = jigarbhand
 00000060: 6572 6940 676d 6169 6c2e 636f 6d0d 0a64  eri@gmail.com..d
 00000070: 6573 6372 6970 7469 6f6e 203d 2041 2073  escription = A s
 00000080: 6d61 6c6c 2065 7861 6d70 6c65 2070 6163  mall example pac
 00000090: 6b61 6765 0d0a 6c6f 6e67 5f64 6573 6372  kage..long_descr
 000000a0: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
```

### Comparing `mypackage1995-0.0.2/src/mypackage1995.egg-info/PKG-INFO` & `mypackage1995-0.0.3/src/mypackage1995.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mypackage1995
-Version: 0.0.2
+Version: 0.0.3
 Summary: A small example package
 Home-page: https://github.com/pypa/sampleproject
 Author: jigar2099
 Author-email: jigarbhanderi@gmail.com
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

