# Comparing `tmp/pycadet-0.1.0.tar.gz` & `tmp/pycadet-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pycadet-0.1.0.tar", last modified: Tue Jul 18 21:23:45 2023, max compression
+gzip compressed data, was "pycadet-0.1.1.tar", last modified: Tue Jul 18 21:29:38 2023, max compression
```

## Comparing `pycadet-0.1.0.tar` & `pycadet-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 plsek     (1000) plsek     (1000)        0 2023-07-18 21:23:45.414522 pycadet-0.1.0/
--rw-rw-r--   0 plsek     (1000) plsek     (1000)     1071 2023-03-06 16:29:32.000000 pycadet-0.1.0/LICENSE
--rw-rw-r--   0 plsek     (1000) plsek     (1000)     7886 2023-07-18 21:23:45.414522 pycadet-0.1.0/PKG-INFO
--rw-rw-r--   0 plsek     (1000) plsek     (1000)     7601 2023-07-18 21:18:19.000000 pycadet-0.1.0/README.md
-drwxrwxr-x   0 plsek     (1000) plsek     (1000)        0 2023-07-18 21:23:45.414522 pycadet-0.1.0/pycadet/
--rw-------   0 plsek     (1000) plsek     (1000)  7423136 2023-01-26 12:53:59.000000 pycadet-0.1.0/pycadet/CADET.hdf5
--rw-rw-r--   0 plsek     (1000) plsek     (1000)      215 2023-06-27 08:55:43.000000 pycadet-0.1.0/pycadet/DS9CADET
--rw-rw-r--   0 plsek     (1000) plsek     (1000)    12024 2023-07-18 14:06:21.000000 pycadet-0.1.0/pycadet/DS9CADET.py
--rw-rw-r--   0 plsek     (1000) plsek     (1000)       23 2023-06-27 10:50:40.000000 pycadet-0.1.0/pycadet/__init__.py
--rw-rw-r--   0 plsek     (1000) plsek     (1000)    12752 2023-07-17 22:09:23.000000 pycadet-0.1.0/pycadet/pycadet.py
-drwxrwxr-x   0 plsek     (1000) plsek     (1000)        0 2023-07-18 21:23:45.414522 pycadet-0.1.0/pycadet.egg-info/
--rw-rw-r--   0 plsek     (1000) plsek     (1000)     7886 2023-07-18 21:23:45.000000 pycadet-0.1.0/pycadet.egg-info/PKG-INFO
--rw-rw-r--   0 plsek     (1000) plsek     (1000)      279 2023-07-18 21:23:45.000000 pycadet-0.1.0/pycadet.egg-info/SOURCES.txt
--rw-rw-r--   0 plsek     (1000) plsek     (1000)        1 2023-07-18 21:23:45.000000 pycadet-0.1.0/pycadet.egg-info/dependency_links.txt
--rw-rw-r--   0 plsek     (1000) plsek     (1000)       52 2023-07-18 21:23:45.000000 pycadet-0.1.0/pycadet.egg-info/entry_points.txt
--rw-rw-r--   0 plsek     (1000) plsek     (1000)        8 2023-07-18 21:23:45.000000 pycadet-0.1.0/pycadet.egg-info/top_level.txt
--rw-rw-r--   0 plsek     (1000) plsek     (1000)       38 2023-07-18 21:23:45.414522 pycadet-0.1.0/setup.cfg
--rw-rw-r--   0 plsek     (1000) plsek     (1000)     5032 2023-07-18 21:20:18.000000 pycadet-0.1.0/setup.py
+drwxrwxr-x   0 plsek     (1000) plsek     (1000)        0 2023-07-18 21:29:38.258739 pycadet-0.1.1/
+-rw-rw-r--   0 plsek     (1000) plsek     (1000)     1071 2023-03-06 16:29:32.000000 pycadet-0.1.1/LICENSE
+-rw-rw-r--   0 plsek     (1000) plsek     (1000)     7886 2023-07-18 21:29:38.258739 pycadet-0.1.1/PKG-INFO
+-rw-rw-r--   0 plsek     (1000) plsek     (1000)     7601 2023-07-18 21:18:19.000000 pycadet-0.1.1/README.md
+drwxrwxr-x   0 plsek     (1000) plsek     (1000)        0 2023-07-18 21:29:38.258739 pycadet-0.1.1/pycadet/
+-rw-------   0 plsek     (1000) plsek     (1000)  7423136 2023-01-26 12:53:59.000000 pycadet-0.1.1/pycadet/CADET.hdf5
+-rw-rw-r--   0 plsek     (1000) plsek     (1000)      215 2023-06-27 08:55:43.000000 pycadet-0.1.1/pycadet/DS9CADET
+-rw-rw-r--   0 plsek     (1000) plsek     (1000)    12024 2023-07-18 14:06:21.000000 pycadet-0.1.1/pycadet/DS9CADET.py
+-rw-rw-r--   0 plsek     (1000) plsek     (1000)       23 2023-06-27 10:50:40.000000 pycadet-0.1.1/pycadet/__init__.py
+-rw-rw-r--   0 plsek     (1000) plsek     (1000)    12752 2023-07-17 22:09:23.000000 pycadet-0.1.1/pycadet/pycadet.py
+drwxrwxr-x   0 plsek     (1000) plsek     (1000)        0 2023-07-18 21:29:38.258739 pycadet-0.1.1/pycadet.egg-info/
+-rw-rw-r--   0 plsek     (1000) plsek     (1000)     7886 2023-07-18 21:29:38.000000 pycadet-0.1.1/pycadet.egg-info/PKG-INFO
+-rw-rw-r--   0 plsek     (1000) plsek     (1000)      279 2023-07-18 21:29:38.000000 pycadet-0.1.1/pycadet.egg-info/SOURCES.txt
+-rw-rw-r--   0 plsek     (1000) plsek     (1000)        1 2023-07-18 21:29:38.000000 pycadet-0.1.1/pycadet.egg-info/dependency_links.txt
+-rw-rw-r--   0 plsek     (1000) plsek     (1000)       52 2023-07-18 21:29:38.000000 pycadet-0.1.1/pycadet.egg-info/entry_points.txt
+-rw-rw-r--   0 plsek     (1000) plsek     (1000)        8 2023-07-18 21:29:38.000000 pycadet-0.1.1/pycadet.egg-info/top_level.txt
+-rw-rw-r--   0 plsek     (1000) plsek     (1000)       38 2023-07-18 21:29:38.258739 pycadet-0.1.1/setup.cfg
+-rw-rw-r--   0 plsek     (1000) plsek     (1000)     5054 2023-07-18 21:29:35.000000 pycadet-0.1.1/setup.py
```

### Comparing `pycadet-0.1.0/LICENSE` & `pycadet-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pycadet-0.1.0/PKG-INFO` & `pycadet-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycadet
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cavity Detection Tool
 Home-page: https://github.com/tomasplsek/CADET
 Author: Tomas Plsek
 Author-email: plsek@physics.muni.cz
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pycadet-0.1.0/README.md` & `pycadet-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pycadet-0.1.0/pycadet/CADET.hdf5` & `pycadet-0.1.1/pycadet/CADET.hdf5`

 * *Files identical despite different names*

### Comparing `pycadet-0.1.0/pycadet/DS9CADET.py` & `pycadet-0.1.1/pycadet/DS9CADET.py`

 * *Files identical despite different names*

### Comparing `pycadet-0.1.0/pycadet/pycadet.py` & `pycadet-0.1.1/pycadet/pycadet.py`

 * *Files identical despite different names*

### Comparing `pycadet-0.1.0/pycadet.egg-info/PKG-INFO` & `pycadet-0.1.1/pycadet.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pycadet
-Version: 0.1.0
+Version: 0.1.1
 Summary: Cavity Detection Tool
 Home-page: https://github.com/tomasplsek/CADET
 Author: Tomas Plsek
 Author-email: plsek@physics.muni.cz
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pycadet-0.1.0/setup.py` & `pycadet-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,16 @@
         for package in requirements:
             pip_install(package)
         install.run(self)
         LoadDS9CADET()
 
 
 def pip_install(package_name):
-    check_call([sys.executable, "-m", "pip", "install", package_name])
+    try: check_call([sys.executable, "-m", "pip", "install", package_name])
+    except: pass
 
 
 requirements = ["numpy >=1.8",
                 "matplotlib", # >= 3.1.1",
                 "astropy >=1.3",
                 "scipy >=0.14",
                 "pyds9 >= 1.8.1",
@@ -124,15 +125,15 @@
 }
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 MAJOR = "0"
 MINOR = "1"
-MICRO = "0"
+MICRO = "1"
 version = "%s.%s.%s" % (MAJOR, MINOR, MICRO)
 
 setup(
     name="pycadet",
     version=version,
     author="Tomas Plsek",
     author_email="plsek@physics.muni.cz",
```

