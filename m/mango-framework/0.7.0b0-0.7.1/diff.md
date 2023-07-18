# Comparing `tmp/mango-framework-0.7.0b0.tar.gz` & `tmp/mango-framework-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-framework-0.7.0b0.tar", last modified: Tue Jul 18 02:30:28 2023, max compression
+gzip compressed data, was "mango-framework-0.7.1.tar", last modified: Tue Jul 18 02:31:29 2023, max compression
```

## Comparing `mango-framework-0.7.0b0.tar` & `mango-framework-0.7.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-18 02:30:28.565906 mango-framework-0.7.0b0/
--rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.7.0b0/LICENSE
--rw-r--r--   0 mohammed   (501) staff       (20)     1922 2023-07-18 02:30:28.565778 mango-framework-0.7.0b0/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)     1240 2023-07-17 12:32:59.000000 mango-framework-0.7.0b0/README.md
--rw-r--r--   0 mohammed   (501) staff       (20)     6471 2023-07-18 02:29:33.000000 mango-framework-0.7.0b0/mango.py
-drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-18 02:30:28.565565 mango-framework-0.7.0b0/mango_framework.egg-info/
--rw-r--r--   0 mohammed   (501) staff       (20)     1922 2023-07-18 02:30:28.000000 mango-framework-0.7.0b0/mango_framework.egg-info/PKG-INFO
--rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-18 02:30:28.000000 mango-framework-0.7.0b0/mango_framework.egg-info/SOURCES.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-18 02:30:28.000000 mango-framework-0.7.0b0/mango_framework.egg-info/dependency_links.txt
--rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-18 02:30:28.000000 mango-framework-0.7.0b0/mango_framework.egg-info/top_level.txt
--rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-18 02:30:28.565945 mango-framework-0.7.0b0/setup.cfg
--rw-r--r--   0 mohammed   (501) staff       (20)      870 2023-07-18 02:29:39.000000 mango-framework-0.7.0b0/setup.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-18 02:31:29.103772 mango-framework-0.7.1/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1023 2023-07-17 05:13:07.000000 mango-framework-0.7.1/LICENSE
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-18 02:31:29.103647 mango-framework-0.7.1/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)     1240 2023-07-17 12:32:59.000000 mango-framework-0.7.1/README.md
+-rw-r--r--   0 mohammed   (501) staff       (20)     6470 2023-07-18 02:31:21.000000 mango-framework-0.7.1/mango.py
+drwxr-xr-x   0 mohammed   (501) staff       (20)        0 2023-07-18 02:31:29.103439 mango-framework-0.7.1/mango_framework.egg-info/
+-rw-r--r--   0 mohammed   (501) staff       (20)     1920 2023-07-18 02:31:29.000000 mango-framework-0.7.1/mango_framework.egg-info/PKG-INFO
+-rw-r--r--   0 mohammed   (501) staff       (20)      191 2023-07-18 02:31:29.000000 mango-framework-0.7.1/mango_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-18 02:31:29.000000 mango-framework-0.7.1/mango_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)        1 2023-07-18 02:31:29.000000 mango-framework-0.7.1/mango_framework.egg-info/top_level.txt
+-rw-r--r--   0 mohammed   (501) staff       (20)       38 2023-07-18 02:31:29.103810 mango-framework-0.7.1/setup.cfg
+-rw-r--r--   0 mohammed   (501) staff       (20)      869 2023-07-18 02:31:18.000000 mango-framework-0.7.1/setup.py
```

### Comparing `mango-framework-0.7.0b0/LICENSE` & `mango-framework-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mango-framework-0.7.0b0/PKG-INFO` & `mango-framework-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.7.0b0
+Version: 0.7.1
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-0.7.0b0/README.md` & `mango-framework-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `mango-framework-0.7.0b0/mango.py` & `mango-framework-0.7.1/mango.py`

 * *Files 0% similar despite different names*

```diff
@@ -180,15 +180,15 @@
         }
     </style>
 </head>
 <body>
     <h1>Server successfully started, but there are no routes or the "/" route is empty</h1>
     <img class="mango-img" src="https://th.bing.com/th/id/R.54bad49b520690f3858b1f396194779d?rik=QSeITH3EbHg4Vw&pid=ImgRaw&r=0" alt="Mango">
     <footer>
-        Version: 0.7.0b
+        Version: 0.7.1
         <br>
         <a class="link" href="https://pypi.org/project/mango-framework/">Check out the development!</a>
     </footer>
 </body>
 </html>
 """
```

### Comparing `mango-framework-0.7.0b0/mango_framework.egg-info/PKG-INFO` & `mango-framework-0.7.1/mango_framework.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-framework
-Version: 0.7.0b0
+Version: 0.7.1
 Summary: A lightweight and highly customizable Python framework for building web applications
 Home-page: https://github.com/momo-AUX1/mango
 Author: Mohammed
 Author-email: fdlnaal@gmail.com
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `mango-framework-0.7.0b0/setup.py` & `mango-framework-0.7.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='mango-framework',
-    version='0.7.0b',
+    version='0.7.1',
     author='Mohammed',
     author_email='fdlnaal@gmail.com',
     description='A lightweight and highly customizable Python framework for building web applications',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/momo-AUX1/mango',
     packages=['.'],
```

