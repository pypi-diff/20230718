# Comparing `tmp/pyvoikko-0.2.tar.gz` & `tmp/pyvoikko-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvoikko-0.2.tar", last modified: Fri Jul  7 11:10:04 2023, max compression
+gzip compressed data, was "pyvoikko-0.3.tar", last modified: Tue Jul 18 10:10:24 2023, max compression
```

## Comparing `pyvoikko-0.2.tar` & `pyvoikko-0.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 11:10:04.816772 pyvoikko-0.2/
--rw-r--r--   0 iikka      (501) staff       (20)    35140 2023-07-06 21:40:03.000000 pyvoikko-0.2/LICENSE
--rw-r--r--   0 iikka      (501) staff       (20)     1750 2023-07-07 11:10:04.816811 pyvoikko-0.2/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)     1098 2023-07-06 22:23:41.000000 pyvoikko-0.2/README.md
--rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:43.000000 pyvoikko-0.2/pyproject.toml
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 11:10:04.815564 pyvoikko-0.2/pyvoikko/
--rw-r--r--   0 iikka      (501) staff       (20)      594 2023-07-07 10:42:45.000000 pyvoikko-0.2/pyvoikko/__init__.py
--rw-r--r--   0 iikka      (501) staff       (20)     5161 2023-07-07 10:42:55.000000 pyvoikko-0.2/pyvoikko/analysis.py
--rw-r--r--   0 iikka      (501) staff       (20)     2010 2023-07-06 21:59:47.000000 pyvoikko-0.2/pyvoikko/constants.py
--rw-r--r--   0 iikka      (501) staff       (20)  1071442 2023-07-06 20:45:08.000000 pyvoikko-0.2/pyvoikko/voikko.kfst
-drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-07 11:10:04.816668 pyvoikko-0.2/pyvoikko.egg-info/
--rw-r--r--   0 iikka      (501) staff       (20)     1750 2023-07-07 11:10:04.000000 pyvoikko-0.2/pyvoikko.egg-info/PKG-INFO
--rw-r--r--   0 iikka      (501) staff       (20)      286 2023-07-07 11:10:04.000000 pyvoikko-0.2/pyvoikko.egg-info/SOURCES.txt
--rw-r--r--   0 iikka      (501) staff       (20)        1 2023-07-07 11:10:04.000000 pyvoikko-0.2/pyvoikko.egg-info/dependency_links.txt
--rw-r--r--   0 iikka      (501) staff       (20)        5 2023-07-07 11:10:04.000000 pyvoikko-0.2/pyvoikko.egg-info/requires.txt
--rw-r--r--   0 iikka      (501) staff       (20)        9 2023-07-07 11:10:04.000000 pyvoikko-0.2/pyvoikko.egg-info/top_level.txt
--rw-r--r--   0 iikka      (501) staff       (20)      816 2023-07-07 11:10:04.817015 pyvoikko-0.2/setup.cfg
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-18 10:10:24.499179 pyvoikko-0.3/
+-rw-r--r--   0 iikka      (501) staff       (20)    35140 2023-07-06 21:40:03.000000 pyvoikko-0.3/LICENSE
+-rw-r--r--   0 iikka      (501) staff       (20)     1750 2023-07-18 10:10:24.499225 pyvoikko-0.3/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)     1098 2023-07-06 22:23:41.000000 pyvoikko-0.3/README.md
+-rw-r--r--   0 iikka      (501) staff       (20)       81 2023-07-05 14:02:43.000000 pyvoikko-0.3/pyproject.toml
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-18 10:10:24.498067 pyvoikko-0.3/pyvoikko/
+-rw-r--r--   0 iikka      (501) staff       (20)      594 2023-07-07 10:42:45.000000 pyvoikko-0.3/pyvoikko/__init__.py
+-rw-r--r--   0 iikka      (501) staff       (20)     5301 2023-07-18 10:01:27.000000 pyvoikko-0.3/pyvoikko/analysis.py
+-rw-r--r--   0 iikka      (501) staff       (20)     2010 2023-07-06 21:59:47.000000 pyvoikko-0.3/pyvoikko/constants.py
+-rw-r--r--   0 iikka      (501) staff       (20)  1071442 2023-07-06 20:45:08.000000 pyvoikko-0.3/pyvoikko/voikko.kfst
+drwxr-xr-x   0 iikka      (501) staff       (20)        0 2023-07-18 10:10:24.499060 pyvoikko-0.3/pyvoikko.egg-info/
+-rw-r--r--   0 iikka      (501) staff       (20)     1750 2023-07-18 10:10:24.000000 pyvoikko-0.3/pyvoikko.egg-info/PKG-INFO
+-rw-r--r--   0 iikka      (501) staff       (20)      286 2023-07-18 10:10:24.000000 pyvoikko-0.3/pyvoikko.egg-info/SOURCES.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        1 2023-07-18 10:10:24.000000 pyvoikko-0.3/pyvoikko.egg-info/dependency_links.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        5 2023-07-18 10:10:24.000000 pyvoikko-0.3/pyvoikko.egg-info/requires.txt
+-rw-r--r--   0 iikka      (501) staff       (20)        9 2023-07-18 10:10:24.000000 pyvoikko-0.3/pyvoikko.egg-info/top_level.txt
+-rw-r--r--   0 iikka      (501) staff       (20)      816 2023-07-18 10:10:24.499431 pyvoikko-0.3/setup.cfg
```

### Comparing `pyvoikko-0.2/LICENSE` & `pyvoikko-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvoikko-0.2/PKG-INFO` & `pyvoikko-0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvoikko
-Version: 0.2
+Version: 0.3
 Summary: A pure-python implementation of the Voikko library that provides Finnish morphological analysis
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Keywords: finnish nlp morphology
```

### Comparing `pyvoikko-0.2/README.md` & `pyvoikko-0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyvoikko-0.2/pyvoikko/__init__.py` & `pyvoikko-0.3/pyvoikko/__init__.py`

 * *Files identical despite different names*

### Comparing `pyvoikko-0.2/pyvoikko/analysis.py` & `pyvoikko-0.3/pyvoikko/analysis.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,15 +86,19 @@
         if len(analyses) == 1:
             return analyses[0]
         
         return analyses[-1]._replace(
             COMPOUND_PARTS=analyses,
             FSTOUTPUT=analysis,
             FORM = "".join([analysis.FORM for analysis in analyses]),
-            BASEFORM = "".join([analysis.BASEFORM + ("-" if analysis.FORM.endswith("-") else "") for analysis in analyses]),
+            BASEFORM = "".join([
+                (analysis.BASEFORM if analysis.CLASS in {"laatusana", "nimisana_laatusana"} else analysis.FORM)
+                + ("-" if analysis.FORM.endswith("-") else "")
+                for analysis in analyses
+            ]),
         )
 
     @staticmethod
     def _from_unitary_voikko_analysis(parts: list[str]):
         in_Xp = False
         in_Xr = False
```

### Comparing `pyvoikko-0.2/pyvoikko/constants.py` & `pyvoikko-0.3/pyvoikko/constants.py`

 * *Files identical despite different names*

### Comparing `pyvoikko-0.2/pyvoikko/voikko.kfst` & `pyvoikko-0.3/pyvoikko/voikko.kfst`

 * *Files identical despite different names*

### Comparing `pyvoikko-0.2/pyvoikko.egg-info/PKG-INFO` & `pyvoikko-0.3/pyvoikko.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvoikko
-Version: 0.2
+Version: 0.3
 Summary: A pure-python implementation of the Voikko library that provides Finnish morphological analysis
 Home-page: https://github.com/fergusq/fst-python
 Author: Iikka Hauhio
 Author-email: iikka.hauhio@helsinki.fi
 License: GNU GPLv3
 Project-URL: Bug Tracker, https://github.com/fergusq/fst-python/issues
 Keywords: finnish nlp morphology
```

### Comparing `pyvoikko-0.2/setup.cfg` & `pyvoikko-0.3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyvoikko
-version = 0.2
+version = 0.3
 author = Iikka Hauhio
 author_email = iikka.hauhio@helsinki.fi
 description = A pure-python implementation of the Voikko library that provides Finnish morphological analysis
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = finnish nlp morphology
 license = GNU GPLv3
```

