# Comparing `tmp/fuzzy_magic-0.1.1.tar.gz` & `tmp/fuzzy_magic-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fuzzy_magic-0.1.1.tar", last modified: Mon Jun 19 12:42:16 2023, max compression
+gzip compressed data, was "fuzzy_magic-0.1.2.tar", last modified: Tue Jul 18 14:27:39 2023, max compression
```

## Comparing `fuzzy_magic-0.1.1.tar` & `fuzzy_magic-0.1.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-06-19 12:42:16.693120 fuzzy_magic-0.1.1/
--rw-r--r--   0 plopez    (1000) plopez    (1000)     1068 2023-06-13 07:43:46.000000 fuzzy_magic-0.1.1/LICENSE.txt
--rw-r--r--   0 plopez    (1000) plopez    (1000)     1257 2023-06-19 12:42:16.693120 fuzzy_magic-0.1.1/PKG-INFO
--rw-r--r--   0 plopez    (1000) plopez    (1000)      751 2023-06-19 12:23:07.000000 fuzzy_magic-0.1.1/README.md
-drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-06-19 12:42:16.693120 fuzzy_magic-0.1.1/fuzzy_magic/
--rw-r--r--   0 plopez    (1000) plopez    (1000)       78 2023-06-19 11:32:42.000000 fuzzy_magic-0.1.1/fuzzy_magic/__init__.py
--rw-r--r--   0 plopez    (1000) plopez    (1000)     2281 2023-05-26 12:52:15.000000 fuzzy_magic-0.1.1/fuzzy_magic/exceptions.py
--rw-r--r--   0 plopez    (1000) plopez    (1000)     8176 2023-06-19 11:49:50.000000 fuzzy_magic-0.1.1/fuzzy_magic/fuzzy.py
--rw-r--r--   0 plopez    (1000) plopez    (1000)     6132 2023-06-19 11:50:13.000000 fuzzy_magic-0.1.1/fuzzy_magic/lvs.py
--rw-r--r--   0 plopez    (1000) plopez    (1000)     1437 2023-06-19 11:50:01.000000 fuzzy_magic-0.1.1/fuzzy_magic/memberships.py
--rw-r--r--   0 plopez    (1000) plopez    (1000)     4401 2023-06-19 11:50:21.000000 fuzzy_magic-0.1.1/fuzzy_magic/rules.py
-drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-06-19 12:42:16.693120 fuzzy_magic-0.1.1/fuzzy_magic.egg-info/
--rw-r--r--   0 plopez    (1000) plopez    (1000)     1257 2023-06-19 12:42:16.000000 fuzzy_magic-0.1.1/fuzzy_magic.egg-info/PKG-INFO
--rw-r--r--   0 plopez    (1000) plopez    (1000)      420 2023-06-19 12:42:16.000000 fuzzy_magic-0.1.1/fuzzy_magic.egg-info/SOURCES.txt
--rw-r--r--   0 plopez    (1000) plopez    (1000)        1 2023-06-19 12:42:16.000000 fuzzy_magic-0.1.1/fuzzy_magic.egg-info/dependency_links.txt
--rw-r--r--   0 plopez    (1000) plopez    (1000)       30 2023-06-19 12:42:16.000000 fuzzy_magic-0.1.1/fuzzy_magic.egg-info/requires.txt
--rw-r--r--   0 plopez    (1000) plopez    (1000)       12 2023-06-19 12:42:16.000000 fuzzy_magic-0.1.1/fuzzy_magic.egg-info/top_level.txt
--rw-r--r--   0 plopez    (1000) plopez    (1000)      576 2023-06-19 12:42:06.000000 fuzzy_magic-0.1.1/pyproject.toml
--rw-r--r--   0 plopez    (1000) plopez    (1000)       38 2023-06-19 12:42:16.693120 fuzzy_magic-0.1.1/setup.cfg
--rw-r--r--   0 plopez    (1000) plopez    (1000)      728 2023-06-19 12:42:01.000000 fuzzy_magic-0.1.1/setup.py
-drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-06-19 12:42:16.693120 fuzzy_magic-0.1.1/test/
--rw-r--r--   0 plopez    (1000) plopez    (1000)     1386 2023-05-26 12:52:15.000000 fuzzy_magic-0.1.1/test/test_fuzzy.py
--rw-r--r--   0 plopez    (1000) plopez    (1000)      519 2023-05-18 15:36:42.000000 fuzzy_magic-0.1.1/test/test_memberships.py
--rw-r--r--   0 plopez    (1000) plopez    (1000)     3034 2023-05-18 15:30:36.000000 fuzzy_magic-0.1.1/test/test_rules.py
+drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-07-18 14:27:39.100789 fuzzy_magic-0.1.2/
+-rw-r--r--   0 plopez    (1000) plopez    (1000)     1068 2023-06-13 07:43:46.000000 fuzzy_magic-0.1.2/LICENSE.txt
+-rw-r--r--   0 plopez    (1000) plopez    (1000)     1257 2023-07-18 14:27:39.100789 fuzzy_magic-0.1.2/PKG-INFO
+-rw-r--r--   0 plopez    (1000) plopez    (1000)      751 2023-06-19 13:38:29.000000 fuzzy_magic-0.1.2/README.md
+drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-07-18 14:27:39.100789 fuzzy_magic-0.1.2/fuzzy_magic/
+-rw-r--r--   0 plopez    (1000) plopez    (1000)       78 2023-06-19 11:32:42.000000 fuzzy_magic-0.1.2/fuzzy_magic/__init__.py
+-rw-r--r--   0 plopez    (1000) plopez    (1000)     2281 2023-05-26 12:52:15.000000 fuzzy_magic-0.1.2/fuzzy_magic/exceptions.py
+-rw-r--r--   0 plopez    (1000) plopez    (1000)     8132 2023-07-17 14:33:09.000000 fuzzy_magic-0.1.2/fuzzy_magic/fuzzy.py
+-rw-r--r--   0 plopez    (1000) plopez    (1000)     6132 2023-06-19 11:50:13.000000 fuzzy_magic-0.1.2/fuzzy_magic/lvs.py
+-rw-r--r--   0 plopez    (1000) plopez    (1000)     1437 2023-06-19 11:50:01.000000 fuzzy_magic-0.1.2/fuzzy_magic/memberships.py
+-rw-r--r--   0 plopez    (1000) plopez    (1000)     4401 2023-06-19 11:50:21.000000 fuzzy_magic-0.1.2/fuzzy_magic/rules.py
+drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-07-18 14:27:39.100789 fuzzy_magic-0.1.2/fuzzy_magic.egg-info/
+-rw-r--r--   0 plopez    (1000) plopez    (1000)     1257 2023-07-18 14:27:39.000000 fuzzy_magic-0.1.2/fuzzy_magic.egg-info/PKG-INFO
+-rw-r--r--   0 plopez    (1000) plopez    (1000)      420 2023-07-18 14:27:39.000000 fuzzy_magic-0.1.2/fuzzy_magic.egg-info/SOURCES.txt
+-rw-r--r--   0 plopez    (1000) plopez    (1000)        1 2023-07-18 14:27:39.000000 fuzzy_magic-0.1.2/fuzzy_magic.egg-info/dependency_links.txt
+-rw-r--r--   0 plopez    (1000) plopez    (1000)       30 2023-07-18 14:27:39.000000 fuzzy_magic-0.1.2/fuzzy_magic.egg-info/requires.txt
+-rw-r--r--   0 plopez    (1000) plopez    (1000)       12 2023-07-18 14:27:39.000000 fuzzy_magic-0.1.2/fuzzy_magic.egg-info/top_level.txt
+-rw-r--r--   0 plopez    (1000) plopez    (1000)      576 2023-07-18 14:27:01.000000 fuzzy_magic-0.1.2/pyproject.toml
+-rw-r--r--   0 plopez    (1000) plopez    (1000)       38 2023-07-18 14:27:39.100789 fuzzy_magic-0.1.2/setup.cfg
+-rw-r--r--   0 plopez    (1000) plopez    (1000)      728 2023-07-18 14:26:38.000000 fuzzy_magic-0.1.2/setup.py
+drwxr-xr-x   0 plopez    (1000) plopez    (1000)        0 2023-07-18 14:27:39.100789 fuzzy_magic-0.1.2/test/
+-rw-r--r--   0 plopez    (1000) plopez    (1000)     1386 2023-05-26 12:52:15.000000 fuzzy_magic-0.1.2/test/test_fuzzy.py
+-rw-r--r--   0 plopez    (1000) plopez    (1000)      519 2023-05-18 15:36:42.000000 fuzzy_magic-0.1.2/test/test_memberships.py
+-rw-r--r--   0 plopez    (1000) plopez    (1000)     3034 2023-05-18 15:30:36.000000 fuzzy_magic-0.1.2/test/test_rules.py
```

### Comparing `fuzzy_magic-0.1.1/LICENSE.txt` & `fuzzy_magic-0.1.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fuzzy_magic-0.1.1/PKG-INFO` & `fuzzy_magic-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzy_magic
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Fuzzy Logic library to create Mamdani Fuzzy Systems the easiest way possible
 Home-page: https://github.com/EXUS-AI-Labs/ailabs-fuzzylogic
 Author: Pedro López
 Author-email: Pedro López <p.lopez@exus.ai>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fuzzy_magic-0.1.1/README.md` & `fuzzy_magic-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `fuzzy_magic-0.1.1/fuzzy_magic/exceptions.py` & `fuzzy_magic-0.1.2/fuzzy_magic/exceptions.py`

 * *Files identical despite different names*

### Comparing `fuzzy_magic-0.1.1/fuzzy_magic/fuzzy.py` & `fuzzy_magic-0.1.2/fuzzy_magic/fuzzy.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,14 @@
         """
             Creation of the whole Fuzzy System taking into account
             the lvs and rules parsed in the creation of the object
 
             Returns: the Fuzzy System
         """
         FS = self.lvs.add_lvs_to_fs()
-        print(FS.get_fuzzy_sets('Service'))
         FS = self.rules.add_rules_to_fs(FS)
 
         return FS
 
 def create_fuzzy_rules(filepath="./data/rules.txt"):
     """
         This method has as aim the creation of the Fuzzy Rules in a
```

### Comparing `fuzzy_magic-0.1.1/fuzzy_magic/lvs.py` & `fuzzy_magic-0.1.2/fuzzy_magic/lvs.py`

 * *Files identical despite different names*

### Comparing `fuzzy_magic-0.1.1/fuzzy_magic/memberships.py` & `fuzzy_magic-0.1.2/fuzzy_magic/memberships.py`

 * *Files identical despite different names*

### Comparing `fuzzy_magic-0.1.1/fuzzy_magic/rules.py` & `fuzzy_magic-0.1.2/fuzzy_magic/rules.py`

 * *Files identical despite different names*

### Comparing `fuzzy_magic-0.1.1/fuzzy_magic.egg-info/PKG-INFO` & `fuzzy_magic-0.1.2/fuzzy_magic.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuzzy-magic
-Version: 0.1.1
+Version: 0.1.2
 Summary: A Fuzzy Logic library to create Mamdani Fuzzy Systems the easiest way possible
 Home-page: https://github.com/EXUS-AI-Labs/ailabs-fuzzylogic
 Author: Pedro López
 Author-email: Pedro López <p.lopez@exus.ai>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `fuzzy_magic-0.1.1/pyproject.toml` & `fuzzy_magic-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0","numpy==1.23.5","simpful==2.10.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "fuzzy_magic"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Pedro López", email="p.lopez@exus.ai" },
 ]
 description = "A Fuzzy Logic library to create Mamdani Fuzzy Systems the easiest way possible"
 readme = "README.md"
 requires-python = ">=3.6"
 dependencies=["numpy==1.23.5","simpful==2.10.0"]
```

### Comparing `fuzzy_magic-0.1.1/setup.py` & `fuzzy_magic-0.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "fuzzy_magic",
-    version = "0.1.1",
+    version = "0.1.2",
     author = "Pedro López",
     author_email = "p.lopez@exus.ai",
     url = "https://github.com/EXUS-AI-Labs/ailabs-fuzzylogic",
     description = "A Fuzzy Logic library to create Mamdani Fuzzy Systems the easiest way possible",
     long_description = long_description,
     classifiers = [
         "Programming Language :: Python :: 3",
```

### Comparing `fuzzy_magic-0.1.1/test/test_fuzzy.py` & `fuzzy_magic-0.1.2/test/test_fuzzy.py`

 * *Files identical despite different names*

### Comparing `fuzzy_magic-0.1.1/test/test_memberships.py` & `fuzzy_magic-0.1.2/test/test_memberships.py`

 * *Files identical despite different names*

### Comparing `fuzzy_magic-0.1.1/test/test_rules.py` & `fuzzy_magic-0.1.2/test/test_rules.py`

 * *Files identical despite different names*

