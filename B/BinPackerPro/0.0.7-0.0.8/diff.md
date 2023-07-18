# Comparing `tmp/BinPackerPro-0.0.7.tar.gz` & `tmp/BinPackerPro-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BinPackerPro-0.0.7.tar", last modified: Tue Jul 18 07:46:21 2023, max compression
+gzip compressed data, was "BinPackerPro-0.0.8.tar", last modified: Tue Jul 18 07:59:48 2023, max compression
```

## Comparing `BinPackerPro-0.0.7.tar` & `BinPackerPro-0.0.8.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 07:46:21.635071 BinPackerPro-0.0.7/
-drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 07:46:21.633828 BinPackerPro-0.0.7/BinPackerPro/
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     6301 2023-07-18 07:43:27.000000 BinPackerPro-0.0.7/BinPackerPro/BinPackerPro.py
--rw-r--r--   0 anasheikharshad   (501) staff       (20)        0 2023-07-17 11:01:08.000000 BinPackerPro-0.0.7/BinPackerPro/__init__.py
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     1000 2023-07-18 06:15:48.000000 BinPackerPro-0.0.7/BinPackerPro/auxiliary_methods.py
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      169 2023-07-17 11:16:34.000000 BinPackerPro-0.0.7/BinPackerPro/constants.py
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     1147 2023-07-17 12:05:26.000000 BinPackerPro-0.0.7/BinPackerPro/plot.py
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     6131 2023-07-18 06:15:48.000000 BinPackerPro-0.0.7/BinPackerPro/utils.py
-drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 07:46:21.634841 BinPackerPro-0.0.7/BinPackerPro.egg-info/
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      365 2023-07-18 07:46:21.000000 BinPackerPro-0.0.7/BinPackerPro.egg-info/PKG-INFO
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      372 2023-07-18 07:46:21.000000 BinPackerPro-0.0.7/BinPackerPro.egg-info/SOURCES.txt
--rw-r--r--   0 anasheikharshad   (501) staff       (20)        1 2023-07-18 07:46:21.000000 BinPackerPro-0.0.7/BinPackerPro.egg-info/dependency_links.txt
--rw-r--r--   0 anasheikharshad   (501) staff       (20)       31 2023-07-18 07:46:21.000000 BinPackerPro-0.0.7/BinPackerPro.egg-info/requires.txt
--rw-r--r--   0 anasheikharshad   (501) staff       (20)       13 2023-07-18 07:46:21.000000 BinPackerPro-0.0.7/BinPackerPro.egg-info/top_level.txt
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     1073 2023-07-17 11:14:54.000000 BinPackerPro-0.0.7/LICENSE
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      365 2023-07-18 07:46:21.635169 BinPackerPro-0.0.7/PKG-INFO
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     1191 2023-07-18 07:43:23.000000 BinPackerPro-0.0.7/README.md
--rw-r--r--   0 anasheikharshad   (501) staff       (20)       79 2023-07-18 07:46:21.635502 BinPackerPro-0.0.7/setup.cfg
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      641 2023-07-18 07:43:02.000000 BinPackerPro-0.0.7/setup.py
+drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 07:59:48.993740 BinPackerPro-0.0.8/
+drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 07:59:48.992675 BinPackerPro-0.0.8/BinPackerPro/
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     6126 2023-07-18 07:53:02.000000 BinPackerPro-0.0.8/BinPackerPro/BinPackerPro.py
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)        0 2023-07-17 11:01:08.000000 BinPackerPro-0.0.8/BinPackerPro/__init__.py
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     1000 2023-07-18 06:15:48.000000 BinPackerPro-0.0.8/BinPackerPro/auxiliary_methods.py
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)      169 2023-07-17 11:16:34.000000 BinPackerPro-0.0.8/BinPackerPro/constants.py
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     1147 2023-07-17 12:05:26.000000 BinPackerPro-0.0.8/BinPackerPro/plot.py
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     6131 2023-07-18 06:15:48.000000 BinPackerPro-0.0.8/BinPackerPro/utils.py
+drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 07:59:48.993609 BinPackerPro-0.0.8/BinPackerPro.egg-info/
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     1598 2023-07-18 07:59:48.000000 BinPackerPro-0.0.8/BinPackerPro.egg-info/PKG-INFO
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)      372 2023-07-18 07:59:48.000000 BinPackerPro-0.0.8/BinPackerPro.egg-info/SOURCES.txt
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)        1 2023-07-18 07:59:48.000000 BinPackerPro-0.0.8/BinPackerPro.egg-info/dependency_links.txt
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)       31 2023-07-18 07:59:48.000000 BinPackerPro-0.0.8/BinPackerPro.egg-info/requires.txt
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)       13 2023-07-18 07:59:48.000000 BinPackerPro-0.0.8/BinPackerPro.egg-info/top_level.txt
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     1073 2023-07-17 11:14:54.000000 BinPackerPro-0.0.8/LICENSE
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     1598 2023-07-18 07:59:48.993833 BinPackerPro-0.0.8/PKG-INFO
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     1191 2023-07-18 07:43:23.000000 BinPackerPro-0.0.8/README.md
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)       79 2023-07-18 07:59:48.994140 BinPackerPro-0.0.8/setup.cfg
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)      747 2023-07-18 07:59:32.000000 BinPackerPro-0.0.8/setup.py
```

### Comparing `BinPackerPro-0.0.7/BinPackerPro/BinPackerPro.py` & `BinPackerPro-0.0.8/BinPackerPro/BinPackerPro.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,21 +102,18 @@
             if len(b.unfitted_items) == 0:
                 return
             pacakge_list = []
             for item in b.unfitted_items:
                 pacakge_list.append(
                     {
                         "BoxName": item.name,
-                        "Dimensions": {
-                            "Length": item.width,
-                            "Width": item.depth,
-                            "Height": item.height,
-                            "Unit": self.dimension_units,
-                        },
-                        "Weight": {"Value": item.weight, "Unit": self.weight_units},
+                        "Length": item.width,
+                        "Width": item.depth,
+                        "Height": item.height,
+                        "Weight": item.weight,
                     }
                 )
             l = self.pack(pacakge_list, pallet_number + 1)
             return l
 
     def get_box_arrangement(self):
         return self.GlobPalletList
```

### Comparing `BinPackerPro-0.0.7/BinPackerPro/auxiliary_methods.py` & `BinPackerPro-0.0.8/BinPackerPro/auxiliary_methods.py`

 * *Files identical despite different names*

### Comparing `BinPackerPro-0.0.7/BinPackerPro/plot.py` & `BinPackerPro-0.0.8/BinPackerPro/plot.py`

 * *Files identical despite different names*

### Comparing `BinPackerPro-0.0.7/BinPackerPro/utils.py` & `BinPackerPro-0.0.8/BinPackerPro/utils.py`

 * *Files identical despite different names*

### Comparing `BinPackerPro-0.0.7/LICENSE` & `BinPackerPro-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `BinPackerPro-0.0.7/README.md` & `BinPackerPro-0.0.8/README.md`

 * *Files identical despite different names*

