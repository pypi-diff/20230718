# Comparing `tmp/BinPackerPro-0.0.4.tar.gz` & `tmp/BinPackerPro-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BinPackerPro-0.0.4.tar", last modified: Tue Jul 18 06:16:19 2023, max compression
+gzip compressed data, was "BinPackerPro-0.0.5.tar", last modified: Tue Jul 18 07:30:43 2023, max compression
```

## Comparing `BinPackerPro-0.0.4.tar` & `BinPackerPro-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 06:16:19.395791 BinPackerPro-0.0.4/
-drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 06:16:19.394371 BinPackerPro-0.0.4/BinPackerPro/
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     6181 2023-07-18 06:15:48.000000 BinPackerPro-0.0.4/BinPackerPro/BinPackerPro.py
--rw-r--r--   0 anasheikharshad   (501) staff       (20)        0 2023-07-17 11:01:08.000000 BinPackerPro-0.0.4/BinPackerPro/__init__.py
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     1000 2023-07-18 06:15:48.000000 BinPackerPro-0.0.4/BinPackerPro/auxiliary_methods.py
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      169 2023-07-17 11:16:34.000000 BinPackerPro-0.0.4/BinPackerPro/constants.py
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     1147 2023-07-17 12:05:26.000000 BinPackerPro-0.0.4/BinPackerPro/plot.py
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     6131 2023-07-18 06:15:48.000000 BinPackerPro-0.0.4/BinPackerPro/utils.py
-drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 06:16:19.395616 BinPackerPro-0.0.4/BinPackerPro.egg-info/
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      413 2023-07-18 06:16:19.000000 BinPackerPro-0.0.4/BinPackerPro.egg-info/PKG-INFO
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      372 2023-07-18 06:16:19.000000 BinPackerPro-0.0.4/BinPackerPro.egg-info/SOURCES.txt
--rw-r--r--   0 anasheikharshad   (501) staff       (20)        1 2023-07-18 06:16:19.000000 BinPackerPro-0.0.4/BinPackerPro.egg-info/dependency_links.txt
--rw-r--r--   0 anasheikharshad   (501) staff       (20)       31 2023-07-18 06:16:19.000000 BinPackerPro-0.0.4/BinPackerPro.egg-info/requires.txt
--rw-r--r--   0 anasheikharshad   (501) staff       (20)       13 2023-07-18 06:16:19.000000 BinPackerPro-0.0.4/BinPackerPro.egg-info/top_level.txt
--rw-r--r--   0 anasheikharshad   (501) staff       (20)     1073 2023-07-17 11:14:54.000000 BinPackerPro-0.0.4/LICENSE
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      413 2023-07-18 06:16:19.395875 BinPackerPro-0.0.4/PKG-INFO
--rw-r--r--   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 06:13:12.000000 BinPackerPro-0.0.4/README.md
--rw-r--r--   0 anasheikharshad   (501) staff       (20)       79 2023-07-18 06:16:19.396176 BinPackerPro-0.0.4/setup.cfg
--rw-r--r--   0 anasheikharshad   (501) staff       (20)      639 2023-07-18 06:10:37.000000 BinPackerPro-0.0.4/setup.py
+drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 07:30:43.038606 BinPackerPro-0.0.5/
+drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 07:30:43.037489 BinPackerPro-0.0.5/BinPackerPro/
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     6300 2023-07-18 07:27:54.000000 BinPackerPro-0.0.5/BinPackerPro/BinPackerPro.py
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)        0 2023-07-17 11:01:08.000000 BinPackerPro-0.0.5/BinPackerPro/__init__.py
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     1000 2023-07-18 06:15:48.000000 BinPackerPro-0.0.5/BinPackerPro/auxiliary_methods.py
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)      169 2023-07-17 11:16:34.000000 BinPackerPro-0.0.5/BinPackerPro/constants.py
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     1147 2023-07-17 12:05:26.000000 BinPackerPro-0.0.5/BinPackerPro/plot.py
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     6131 2023-07-18 06:15:48.000000 BinPackerPro-0.0.5/BinPackerPro/utils.py
+drwxr-xr-x   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 07:30:43.038416 BinPackerPro-0.0.5/BinPackerPro.egg-info/
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)      413 2023-07-18 07:30:42.000000 BinPackerPro-0.0.5/BinPackerPro.egg-info/PKG-INFO
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)      372 2023-07-18 07:30:43.000000 BinPackerPro-0.0.5/BinPackerPro.egg-info/SOURCES.txt
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)        1 2023-07-18 07:30:42.000000 BinPackerPro-0.0.5/BinPackerPro.egg-info/dependency_links.txt
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)       31 2023-07-18 07:30:42.000000 BinPackerPro-0.0.5/BinPackerPro.egg-info/requires.txt
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)       13 2023-07-18 07:30:42.000000 BinPackerPro-0.0.5/BinPackerPro.egg-info/top_level.txt
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)     1073 2023-07-17 11:14:54.000000 BinPackerPro-0.0.5/LICENSE
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)      413 2023-07-18 07:30:43.038695 BinPackerPro-0.0.5/PKG-INFO
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)        0 2023-07-18 06:13:12.000000 BinPackerPro-0.0.5/README.md
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)       79 2023-07-18 07:30:43.038982 BinPackerPro-0.0.5/setup.cfg
+-rw-r--r--   0 anasheikharshad   (501) staff       (20)      639 2023-07-18 07:28:40.000000 BinPackerPro-0.0.5/setup.py
```

### Comparing `BinPackerPro-0.0.4/BinPackerPro/BinPackerPro.py` & `BinPackerPro-0.0.5/BinPackerPro/BinPackerPro.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,29 +18,32 @@
         self.pallet_length = pallet_length
         self.pallet_width = pallet_width
         self.pallet_height = pallet_height
         self.dimension_units = dimension_units
         self.pallet_weight = pallet_weight
         self.weight_units = weight_units
         self.pacakge_list = pacakge_list
-        self.pallet_number = 1
         self.GlobPalletList = []
 
-    def pack(self):
+    def pack(self,pacakge_list = None,pallet_number = None):
+        if not pacakge_list:
+            pacakge_list = self.pacakge_list
+        if not pallet_number:
+            pallet_number = 1
         packer = Packer()
         packer.add_bin(
             Bin(
-                f"pallet-{self.pallet_number}",
+                f"pallet-{pallet_number}",
                 self.pallet_length,
                 self.pallet_height,
                 self.pallet_width,
                 self.pallet_weight,
             )
         )
-        for package in self.pacakge_list:
+        for package in pacakge_list:
             if (
                 package["Length"] > self.pallet_length
                 or package["Height"] > self.pallet_height
                 or package["Width"] > self.pallet_width
             ):
                 return "error"
             packer.add_item(
@@ -54,28 +57,28 @@
             )
         packer.pack(bigger_first=True, distribute_items=False, number_of_decimals=2)
         PalletLength = 0
         PalletHeight = 0
         PalletWidth = 0
         PalletWeight = 0
         BoxCount = 0
-        pallet = {"PalletName": f"pallet-{self.pallet_number}", "BoxArrangementList": []}
+        pallet = {"PalletName": f"pallet-{pallet_number}", "BoxArrangementList": []}
         for b in packer.bins:
             for item in b.items:
                 BoxCount += 1
                 pallet["BoxArrangementList"].append(
                     {
                         "BoxName": item.name,
                         "BoxLength": str(item.width),
                         "BoxWidth": str(item.depth),
                         "BoxHeight": str(item.height),
                         "BoxWeight": str(item.weight),
                         "BoxPosition": [str(cordinate) for cordinate in item.position],
                         "BoxRotation": str(item.rotation_type),
-                        "PalletName": f"pallet-{self.pallet_number}",
+                        "PalletName": f"pallet-{pallet_number}",
                     }
                 )
                 PalletWeight += item.weight
                 if item.rotation_type == 0:
                     w = item.position[0] + item.width
                     h = item.position[1] + item.height
                     d = item.position[2] + item.depth
@@ -108,15 +111,15 @@
                             "Width": item.depth,
                             "Height": item.height,
                             "Unit": self.dimension_units,
                         },
                         "Weight": {"Value": item.weight, "Unit": self.weight_units},
                     }
                 )
-            l = self.pack(PackageList, self.pallet_number + 1)
+            l = self.pack(PackageList, pallet_number + 1)
             return l
 
     def get_box_arrangement(self):
         return self.GlobPalletList
 
     def get_box_arrangement_plot(self, file_path):
         pp = PdfPages(
```

### Comparing `BinPackerPro-0.0.4/BinPackerPro/auxiliary_methods.py` & `BinPackerPro-0.0.5/BinPackerPro/auxiliary_methods.py`

 * *Files identical despite different names*

### Comparing `BinPackerPro-0.0.4/BinPackerPro/plot.py` & `BinPackerPro-0.0.5/BinPackerPro/plot.py`

 * *Files identical despite different names*

### Comparing `BinPackerPro-0.0.4/BinPackerPro/utils.py` & `BinPackerPro-0.0.5/BinPackerPro/utils.py`

 * *Files identical despite different names*

### Comparing `BinPackerPro-0.0.4/LICENSE` & `BinPackerPro-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `BinPackerPro-0.0.4/setup.py` & `BinPackerPro-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from distutils.core import setup
 setup(
   name = 'BinPackerPro',         
   packages = ['BinPackerPro'],   
-  version = '0.0.4',     
+  version = '0.0.5',     
   license='MIT',      
   description = 'bin packer pro',  
   author = 'Shaik Arshad',                 
   author_email = 'smdar7@example.com',     
   url = 'https://github.com/pypa/binpackerpro',   
   install_requires=[           
           'matplotlib==3.3',
```

