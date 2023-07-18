# Comparing `tmp/foc-0.1.4.tar.gz` & `tmp/foc-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foc-0.1.4.tar", last modified: Sat Jul 15 21:06:18 2023, max compression
+gzip compressed data, was "foc-0.1.5.tar", last modified: Tue Jul 18 13:13:02 2023, max compression
```

## Comparing `foc-0.1.4.tar` & `foc-0.1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-15 21:06:18.546649 foc-0.1.4/
--rw-r--r--   0 thyeem     (501) staff       (20)      412 2023-07-15 21:05:41.000000 foc-0.1.4/ChangeLog.md
--rw-r--r--   0 thyeem     (501) staff       (20)     1068 2023-05-15 21:22:31.000000 foc-0.1.4/LICENSE
--rw-r--r--   0 thyeem     (501) staff       (20)       55 2023-06-06 23:18:02.000000 foc-0.1.4/MANIFEST.in
--rw-r--r--   0 thyeem     (501) staff       (20)    17346 2023-07-15 21:06:18.546802 foc-0.1.4/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)    16885 2023-07-15 21:05:41.000000 foc-0.1.4/README.md
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-15 21:06:18.544744 foc-0.1.4/foc/
--rw-r--r--   0 thyeem     (501) staff       (20)    18950 2023-07-15 21:05:41.000000 foc-0.1.4/foc/__init__.py
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-15 21:06:18.545914 foc-0.1.4/foc.egg-info/
--rw-r--r--   0 thyeem     (501) staff       (20)    17346 2023-07-15 21:06:18.000000 foc-0.1.4/foc.egg-info/PKG-INFO
--rw-r--r--   0 thyeem     (501) staff       (20)      221 2023-07-15 21:06:18.000000 foc-0.1.4/foc.egg-info/SOURCES.txt
--rw-r--r--   0 thyeem     (501) staff       (20)        1 2023-07-15 21:06:18.000000 foc-0.1.4/foc.egg-info/dependency_links.txt
--rw-r--r--   0 thyeem     (501) staff       (20)       10 2023-07-15 21:06:18.000000 foc-0.1.4/foc.egg-info/top_level.txt
--rw-r--r--   0 thyeem     (501) staff       (20)      102 2023-07-15 21:06:18.547502 foc-0.1.4/setup.cfg
--rw-r--r--   0 thyeem     (501) staff       (20)      700 2023-07-15 21:05:41.000000 foc-0.1.4/setup.py
-drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-15 21:06:18.546413 foc-0.1.4/tests/
--rw-r--r--   0 thyeem     (501) staff       (20)        0 2023-06-11 20:28:50.000000 foc-0.1.4/tests/__init__.py
--rw-r--r--   0 thyeem     (501) staff       (20)     8330 2023-07-15 21:05:41.000000 foc-0.1.4/tests/test_foc.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-18 13:13:02.527659 foc-0.1.5/
+-rw-r--r--   0 thyeem     (501) staff       (20)      464 2023-07-18 13:12:03.000000 foc-0.1.5/ChangeLog.md
+-rw-r--r--   0 thyeem     (501) staff       (20)     1068 2023-06-07 00:06:02.000000 foc-0.1.5/LICENSE
+-rw-r--r--   0 thyeem     (501) staff       (20)       55 2023-06-07 00:06:02.000000 foc-0.1.5/MANIFEST.in
+-rw-r--r--   0 thyeem     (501) staff       (20)    17346 2023-07-18 13:13:02.527739 foc-0.1.5/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)    16885 2023-07-18 12:48:54.000000 foc-0.1.5/README.md
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-18 13:13:02.523555 foc-0.1.5/foc/
+-rw-r--r--   0 thyeem     (501) staff       (20)    19101 2023-07-18 12:58:34.000000 foc-0.1.5/foc/__init__.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-18 13:13:02.524018 foc-0.1.5/foc.egg-info/
+-rw-r--r--   0 thyeem     (501) staff       (20)    17346 2023-07-18 13:13:02.000000 foc-0.1.5/foc.egg-info/PKG-INFO
+-rw-r--r--   0 thyeem     (501) staff       (20)      221 2023-07-18 13:13:02.000000 foc-0.1.5/foc.egg-info/SOURCES.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)        1 2023-07-18 13:13:02.000000 foc-0.1.5/foc.egg-info/dependency_links.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)       10 2023-07-18 13:13:02.000000 foc-0.1.5/foc.egg-info/top_level.txt
+-rw-r--r--   0 thyeem     (501) staff       (20)      102 2023-07-18 13:13:02.528006 foc-0.1.5/setup.cfg
+-rw-r--r--   0 thyeem     (501) staff       (20)      700 2023-07-18 13:09:51.000000 foc-0.1.5/setup.py
+drwxr-xr-x   0 thyeem     (501) staff       (20)        0 2023-07-18 13:13:02.527528 foc-0.1.5/tests/
+-rw-r--r--   0 thyeem     (501) staff       (20)        0 2023-06-15 10:03:02.000000 foc-0.1.5/tests/__init__.py
+-rw-r--r--   0 thyeem     (501) staff       (20)     8338 2023-07-18 12:57:28.000000 foc-0.1.5/tests/test_foc.py
```

### Comparing `foc-0.1.4/LICENSE` & `foc-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `foc-0.1.4/PKG-INFO` & `foc-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foc
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collection of python functions for somebody's sanity
 Home-page: https://github.com/thyeem/foc
 Author: Francis Lim
 Author-email: thyeem@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `foc-0.1.4/README.md` & `foc-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `foc-0.1.4/foc/__init__.py` & `foc-0.1.5/foc/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,22 +105,23 @@
     "flatl",
     "flatt",
     "flatd",
     "flats",
     "fread",
     "fwrite",
     "split_at",
-    "chunk_of",
+    "chunks_of",
     "capture",
     "captures",
     "error",
     "HOME",
     "cd",
     "pwd",
     "ls",
+    "grep",
     "normpath",
     "exists",
     "dirname",
     "basename",
     "mkdir",
     "rmdir",
     "bytes_to_int",
@@ -672,18 +673,18 @@
             fh.write(f"{line}\n")
     return f
 
 
 def split_at(ix, x):
     """split iterables at the given splitting-indices"""
     s = flatl(0, ix, None)
-    return [[*it.islice(x, begin, end)] for begin, end in zip(s, s[1:])]
+    return ([*it.islice(x, begin, end)] for begin, end in zip(s, s[1:]))
 
 
-def chunk_of(n, x, fill=None):
+def chunks_of(n, x, fill=None):
     """split interables into the given `n-length` pieces"""
     return it.zip_longest(*(iter(x),) * n, fillvalue=fill)
 
 
 def capture(p, string):
     x = captures(p, string)
     if x:
@@ -710,16 +711,22 @@
     return pwd()
 
 
 def pwd():
     return os.getcwd()
 
 
-def ls(path="."):
-    return os.listdir(normpath(path, abs=True))
+def ls(d=".", path=False, abs=False):
+    d = normpath(d, abs=abs)
+    return [f"{d}/{f}" for f in os.listdir(d)] if path else os.listdir(d)
+
+
+@safe
+def grep(regex):
+    return vl_(f_(re.search, regex))
 
 
 def normpath(path, abs=False):
     return cf_(
         os.path.abspath if abs else id,
         os.path.normpath,
         os.path.expanduser,
```

### Comparing `foc-0.1.4/foc.egg-info/PKG-INFO` & `foc-0.1.5/foc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foc
-Version: 0.1.4
+Version: 0.1.5
 Summary: A collection of python functions for somebody's sanity
 Home-page: https://github.com/thyeem/foc
 Author: Francis Lim
 Author-email: thyeem@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `foc-0.1.4/setup.py` & `foc-0.1.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="foc",
-    version="0.1.4",
+    version="0.1.5",
     author="Francis Lim",
     author_email="thyeem@gmail.com",
     description="A collection of python functions for somebody's sanity",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires=[],
     url="https://github.com/thyeem/foc",
```

### Comparing `foc-0.1.4/tests/test_foc.py` & `foc-0.1.5/tests/test_foc.py`

 * *Files 0% similar despite different names*

```diff
@@ -397,19 +397,19 @@
 
 
 def test_captures():
     assert captures(r"\d+", "2023Year-05Month-24Day") == ["2023", "05", "24"]
 
 
 def test_split_at():
-    assert split_at((3, 5), range(1, 11)) == [[1, 2, 3], [4, 5], [6, 7, 8, 9, 10]]
+    assert list(split_at((3, 5), range(1, 11))) == [[1, 2, 3], [4, 5], [6, 7, 8, 9, 10]]
 
 
-def test_chunk_of():
-    assert list(chunk_of(3, range(1, 11))) == [
+def test_chunks_of():
+    assert list(chunks_of(3, range(1, 11))) == [
         (1, 2, 3),
         (4, 5, 6),
         (7, 8, 9),
         (10, None, None),
     ]
```

