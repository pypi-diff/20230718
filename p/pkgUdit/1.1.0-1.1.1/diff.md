# Comparing `tmp/pkgUdit-1.1.0-py3-none-any.whl.zip` & `tmp/pkgUdit-1.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,14 @@
-Zip file size: 3074 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      119 b- defN 23-Jul-18 17:40 pkgUdit/__init__.py
--rw-rw-rw-  2.0 fat     1886 b- defN 23-Jul-18 17:16 pkgUdit/pswdGen.py
--rw-rw-rw-  2.0 fat     1079 b- defN 23-Jul-18 17:48 pkgUdit-1.1.0.dist-info/License.txt
--rw-rw-rw-  2.0 fat      352 b- defN 23-Jul-18 17:48 pkgUdit-1.1.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-18 17:48 pkgUdit-1.1.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-18 17:48 pkgUdit-1.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      539 b- defN 23-Jul-18 17:48 pkgUdit-1.1.0.dist-info/RECORD
-7 files, 4087 bytes uncompressed, 2120 bytes compressed:  48.1%
+Zip file size: 5206 bytes, number of entries: 12
+-rw-rw-rw-  2.0 fat       83 b- defN 23-Jul-18 16:29 pkgUdit/Names.csv
+-rw-rw-rw-  2.0 fat       90 b- defN 23-Jul-18 16:29 pkgUdit/Places.csv
+-rw-rw-rw-  2.0 fat      292 b- defN 23-Jul-18 20:33 pkgUdit/__init__.py
+-rw-rw-rw-  2.0 fat     2874 b- defN 23-Jul-18 16:39 pkgUdit/d.py
+-rw-rw-rw-  2.0 fat     2293 b- defN 23-Jul-18 20:45 pkgUdit/pswdGen.py
+-rw-rw-rw-  2.0 fat       83 b- defN 23-Jul-18 20:33 pkgUdit/data/names.csv
+-rw-rw-rw-  2.0 fat       90 b- defN 23-Jul-18 20:33 pkgUdit/data/places.csv
+-rw-rw-rw-  2.0 fat     1079 b- defN 23-Jul-18 20:48 pkgUdit-1.1.1.dist-info/License.txt
+-rw-rw-rw-  2.0 fat      352 b- defN 23-Jul-18 20:48 pkgUdit-1.1.1.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-18 20:48 pkgUdit-1.1.1.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-18 20:48 pkgUdit-1.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      908 b- defN 23-Jul-18 20:48 pkgUdit-1.1.1.dist-info/RECORD
+12 files, 8256 bytes uncompressed, 3688 bytes compressed:  55.3%
```

## zipnote {}

```diff
@@ -1,22 +1,37 @@
+Filename: pkgUdit/Names.csv
+Comment: 
+
+Filename: pkgUdit/Places.csv
+Comment: 
+
 Filename: pkgUdit/__init__.py
 Comment: 
 
+Filename: pkgUdit/d.py
+Comment: 
+
 Filename: pkgUdit/pswdGen.py
 Comment: 
 
-Filename: pkgUdit-1.1.0.dist-info/License.txt
+Filename: pkgUdit/data/names.csv
+Comment: 
+
+Filename: pkgUdit/data/places.csv
+Comment: 
+
+Filename: pkgUdit-1.1.1.dist-info/License.txt
 Comment: 
 
-Filename: pkgUdit-1.1.0.dist-info/METADATA
+Filename: pkgUdit-1.1.1.dist-info/METADATA
 Comment: 
 
-Filename: pkgUdit-1.1.0.dist-info/WHEEL
+Filename: pkgUdit-1.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: pkgUdit-1.1.0.dist-info/top_level.txt
+Filename: pkgUdit-1.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: pkgUdit-1.1.0.dist-info/RECORD
+Filename: pkgUdit-1.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pkgUdit/__init__.py

```diff
@@ -1,8 +1,18 @@
-from pswdGen import generatePass
+# import sys
+# import os
 
+# Add the parent directory to the Python path
+# print(__file__)
+# parent_dir = os.path.dirname(os.path.abspath(__file__))
+# sys.path.append(parent_dir)
 
 
-def generatePassword():
-    return generatePass()
 
-print(generatePassword())
+from .pswdGen import generatePass
+
+
+
+# def generatePassword():
+#     return generatePass()
+
+
```

## pkgUdit/pswdGen.py

```diff
@@ -1,24 +1,39 @@
 import random
 import csv
+import os
+
+module_dir = os.path.dirname(__file__)
+# print(module_dir)
+# contents = os.listdir(module_dir)
+# print(contents)
+module_dir = os.path.dirname(__file__)
+
 
 numerals = ['0','1','2','3','4','5','6','7','8','9']
 lowerCaps = ['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z']
 upperChars = ['A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z']
 
 combinedChars = numerals + lowerCaps + upperChars
+file_name = 'names.csv'
+file_path = os.path.join(module_dir, file_name)
 
-with open('Names.csv') as names_file:
+with open(file_path) as names_file:
         
         names_reader = csv.reader(names_file)
         nameList = []
         for row in names_reader:
             nameList.append(row[0])
-        
-with open('Places.csv') as places_file:
+            
+file_name = 'places.csv'
+file_path = os.path.join(module_dir, file_name)
+# print(file_path)
+# print(type file_path)
+# with open('plcea.csv') as places_file:
+with open(file_path) as places_file:
     places_reader = csv.reader(places_file)
     placeList = []
 
     for row in places_reader:
         placeList.append(row[0])
 
 def custom_choice(combinedChars):
```

## Comparing `pkgUdit-1.1.0.dist-info/License.txt` & `pkgUdit-1.1.1.dist-info/License.txt`

 * *Files identical despite different names*

