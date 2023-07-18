# Comparing `tmp/PySolidState-0.1.1.tar.gz` & `tmp/PySolidState-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySolidState-0.1.1.tar", last modified: Mon Jul 17 14:50:12 2023, max compression
+gzip compressed data, was "PySolidState-0.1.2.tar", last modified: Tue Jul 18 20:35:02 2023, max compression
```

## Comparing `PySolidState-0.1.1.tar` & `PySolidState-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-07-17 14:50:12.870828 PySolidState-0.1.1/
--rw-rw-rw-   0        0        0     1122 2023-07-17 14:50:12.868827 PySolidState-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-17 14:50:12.819828 PySolidState-0.1.1/PySolidState/
--rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.1.1/PySolidState/__init__.py
-drwxrwxrwx   0        0        0        0 2023-07-17 14:50:12.864827 PySolidState-0.1.1/PySolidState/crystal_structure/
--rw-rw-rw-   0        0        0        0 2023-07-08 17:20:16.000000 PySolidState-0.1.1/PySolidState/crystal_structure/__init__.py
--rw-rw-rw-   0        0        0      786 2023-07-08 17:20:16.000000 PySolidState-0.1.1/PySolidState/crystal_structure/atom.py
--rw-rw-rw-   0        0        0     7632 2023-07-17 14:48:35.000000 PySolidState-0.1.1/PySolidState/crystal_structure/base.py
--rw-rw-rw-   0        0        0     7052 2023-07-17 14:48:22.000000 PySolidState-0.1.1/PySolidState/crystal_structure/crystalStructure.py
--rw-rw-rw-   0        0        0    16788 2023-07-17 13:58:51.000000 PySolidState-0.1.1/PySolidState/crystal_structure/lattice.py
--rw-rw-rw-   0        0        0     3431 2023-07-08 17:20:16.000000 PySolidState-0.1.1/PySolidState/crystal_structure/lattices.json
-drwxrwxrwx   0        0        0        0 2023-07-17 14:50:12.847824 PySolidState-0.1.1/PySolidState.egg-info/
--rw-rw-rw-   0        0        0     1122 2023-07-17 14:50:12.000000 PySolidState-0.1.1/PySolidState.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      481 2023-07-17 14:50:12.000000 PySolidState-0.1.1/PySolidState.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-17 14:50:12.000000 PySolidState-0.1.1/PySolidState.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       31 2023-07-17 14:50:12.000000 PySolidState-0.1.1/PySolidState.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-17 14:50:12.000000 PySolidState-0.1.1/PySolidState.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      416 2023-07-16 01:06:43.000000 PySolidState-0.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-07-17 14:50:12.870828 PySolidState-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1380 2023-07-17 14:49:50.000000 PySolidState-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 20:35:02.029773 PySolidState-0.1.2/
+-rw-rw-rw-   0        0        0     6955 2023-07-18 20:35:02.025774 PySolidState-0.1.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 20:35:01.950770 PySolidState-0.1.2/PySolidState/
+-rw-rw-rw-   0        0        0        0 2023-07-18 20:32:01.000000 PySolidState-0.1.2/PySolidState/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 20:35:02.021773 PySolidState-0.1.2/PySolidState/crystal_structure/
+-rw-rw-rw-   0        0        0        0 2023-07-18 20:32:01.000000 PySolidState-0.1.2/PySolidState/crystal_structure/__init__.py
+-rw-rw-rw-   0        0        0      786 2023-07-18 20:32:01.000000 PySolidState-0.1.2/PySolidState/crystal_structure/atom.py
+-rw-rw-rw-   0        0        0     7632 2023-07-18 20:32:01.000000 PySolidState-0.1.2/PySolidState/crystal_structure/base.py
+-rw-rw-rw-   0        0        0     7052 2023-07-18 20:32:01.000000 PySolidState-0.1.2/PySolidState/crystal_structure/crystalStructure.py
+-rw-rw-rw-   0        0        0    16788 2023-07-18 20:32:01.000000 PySolidState-0.1.2/PySolidState/crystal_structure/lattice.py
+-rw-rw-rw-   0        0        0     3431 2023-07-18 20:32:01.000000 PySolidState-0.1.2/PySolidState/crystal_structure/lattices.json
+drwxrwxrwx   0        0        0        0 2023-07-18 20:35:01.995776 PySolidState-0.1.2/PySolidState.egg-info/
+-rw-rw-rw-   0        0        0     6955 2023-07-18 20:35:01.000000 PySolidState-0.1.2/PySolidState.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      481 2023-07-18 20:35:01.000000 PySolidState-0.1.2/PySolidState.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 20:35:01.000000 PySolidState-0.1.2/PySolidState.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       31 2023-07-18 20:35:01.000000 PySolidState-0.1.2/PySolidState.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-07-18 20:35:01.000000 PySolidState-0.1.2/PySolidState.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     6056 2023-07-18 20:34:24.000000 PySolidState-0.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-18 20:35:02.029773 PySolidState-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1380 2023-07-18 20:34:51.000000 PySolidState-0.1.2/setup.py
```

### Comparing `PySolidState-0.1.1/PySolidState/crystal_structure/atom.py` & `PySolidState-0.1.2/PySolidState/crystal_structure/atom.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.1/PySolidState/crystal_structure/base.py` & `PySolidState-0.1.2/PySolidState/crystal_structure/base.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.1/PySolidState/crystal_structure/crystalStructure.py` & `PySolidState-0.1.2/PySolidState/crystal_structure/crystalStructure.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.1/PySolidState/crystal_structure/lattice.py` & `PySolidState-0.1.2/PySolidState/crystal_structure/lattice.py`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.1/PySolidState/crystal_structure/lattices.json` & `PySolidState-0.1.2/PySolidState/crystal_structure/lattices.json`

 * *Files identical despite different names*

### Comparing `PySolidState-0.1.1/setup.py` & `PySolidState-0.1.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="PySolidState",
-    version="0.1.1",
+    version="0.1.2",
     description="PySolidState is a library developed to facilitate the study of solid-state materials, ranging from crystal structures to tight-binding models. It provides a set of tools and functionalities that enable researchers and students to analyze and simulate various aspects of the solid-state physics.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/miguelta281/PySolidState",
     author="Jose Miguel Tarazona, Yerimi Gamboa Caballero, Felipe",
     author_email="makesens19@gmail.com",
     license="GNU General Public License v3.0",
```

