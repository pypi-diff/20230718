# Comparing `tmp/bingo_bongo_cat-0.0.5.tar.gz` & `tmp/bingo_bongo_cat-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bingo_bongo_cat-0.0.5.tar", last modified: Tue Jul 18 17:26:51 2023, max compression
+gzip compressed data, was "bingo_bongo_cat-0.0.6.tar", last modified: Tue Jul 18 17:37:51 2023, max compression
```

## Comparing `bingo_bongo_cat-0.0.5.tar` & `bingo_bongo_cat-0.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 17:26:51.989096 bingo_bongo_cat-0.0.5/
--rw-rw-rw-   0        0        0        0 2023-07-18 16:57:14.000000 bingo_bongo_cat-0.0.5/LICENSE
--rw-rw-rw-   0        0        0      646 2023-07-18 17:26:51.988096 bingo_bongo_cat-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0     1007 2023-07-18 06:31:56.000000 bingo_bongo_cat-0.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-07-18 17:26:51.975098 bingo_bongo_cat-0.0.5/bingo_bongo_cat/
--rw-rw-rw-   0        0        0       36 2023-07-18 17:25:59.000000 bingo_bongo_cat-0.0.5/bingo_bongo_cat/__init__.py
--rw-rw-rw-   0        0        0     1698 2023-07-18 17:03:38.000000 bingo_bongo_cat-0.0.5/bingo_bongo_cat/bingo_bongo_cat.py
-drwxrwxrwx   0        0        0        0 2023-07-18 17:26:51.984095 bingo_bongo_cat-0.0.5/bingo_bongo_cat.egg-info/
--rw-rw-rw-   0        0        0      646 2023-07-18 17:26:51.000000 bingo_bongo_cat-0.0.5/bingo_bongo_cat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-07-18 17:26:51.000000 bingo_bongo_cat-0.0.5/bingo_bongo_cat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 17:26:51.000000 bingo_bongo_cat-0.0.5/bingo_bongo_cat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2023-07-18 17:26:51.000000 bingo_bongo_cat-0.0.5/bingo_bongo_cat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-07-18 17:26:51.989096 bingo_bongo_cat-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0      916 2023-07-18 17:26:18.000000 bingo_bongo_cat-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:37:51.600356 bingo_bongo_cat-0.0.6/
+-rw-rw-rw-   0        0        0        0 2023-07-18 16:57:14.000000 bingo_bongo_cat-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0      646 2023-07-18 17:37:51.599352 bingo_bongo_cat-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0     1007 2023-07-18 06:31:56.000000 bingo_bongo_cat-0.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-07-18 17:37:51.579356 bingo_bongo_cat-0.0.6/bingo_bongo_cat/
+-rw-rw-rw-   0        0        0       22 2023-07-18 17:37:28.000000 bingo_bongo_cat-0.0.6/bingo_bongo_cat/__init__.py
+-rw-rw-rw-   0        0        0     1586 2023-07-18 17:37:40.000000 bingo_bongo_cat-0.0.6/bingo_bongo_cat/bingo_bongo_cat.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:37:51.591354 bingo_bongo_cat-0.0.6/bingo_bongo_cat.egg-info/
+-rw-rw-rw-   0        0        0      646 2023-07-18 17:37:51.000000 bingo_bongo_cat-0.0.6/bingo_bongo_cat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-07-18 17:37:51.000000 bingo_bongo_cat-0.0.6/bingo_bongo_cat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 17:37:51.000000 bingo_bongo_cat-0.0.6/bingo_bongo_cat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2023-07-18 17:37:51.000000 bingo_bongo_cat-0.0.6/bingo_bongo_cat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-07-18 17:37:51.600356 bingo_bongo_cat-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0      916 2023-07-18 17:30:04.000000 bingo_bongo_cat-0.0.6/setup.py
```

### Comparing `bingo_bongo_cat-0.0.5/PKG-INFO` & `bingo_bongo_cat-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingo_bongo_cat
-Version: 0.0.5
+Version: 0.0.6
 Summary: Cat that prints messages.
 Author: Kyle Levy
 Author-email: 
 Keywords: python,debugging,cat,funny
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bingo_bongo_cat-0.0.5/README.md` & `bingo_bongo_cat-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `bingo_bongo_cat-0.0.5/bingo_bongo_cat/bingo_bongo_cat.py` & `bingo_bongo_cat-0.0.6/bingo_bongo_cat/bingo_bongo_cat.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,12 +46,8 @@
             │  {text}  │
             ┕━━{tb_line}━━┙
                V"""
         if quiet == False:
             print(speechBubble)
             print(self.cat)
 
-        return str(speechBubble+'\n'+self.cat)
-
-# Calling the function to demonstrate the error
-if __name__ == '__main__':
-    FunnyCat().say("Hi Y'all!")
+        return str(speechBubble+'\n'+self.cat)
```

### Comparing `bingo_bongo_cat-0.0.5/bingo_bongo_cat.egg-info/PKG-INFO` & `bingo_bongo_cat-0.0.6/bingo_bongo_cat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bingo-bongo-cat
-Version: 0.0.5
+Version: 0.0.6
 Summary: Cat that prints messages.
 Author: Kyle Levy
 Author-email: 
 Keywords: python,debugging,cat,funny
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `bingo_bongo_cat-0.0.5/setup.py` & `bingo_bongo_cat-0.0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.5'
+VERSION = '0.0.6'
 DESCRIPTION = 'Cat that prints messages.'
 LONG_DESCRIPTION = 'A package which makes troubleshooting code a little less painful by adding a cute cat to let you know where you went wrong.'
 
 # Setting up
 setup(
     name="bingo_bongo_cat",
     version=VERSION,
```

