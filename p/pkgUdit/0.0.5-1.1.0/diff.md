# Comparing `tmp/pkgUdit-0.0.5-py3-none-any.whl.zip` & `tmp/pkgUdit-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3119 bytes, number of entries: 7
--rw-rw-rw-  2.0 fat      958 b- defN 23-Jul-17 09:35 pkgUdit/__init__.py
--rw-rw-rw-  2.0 fat      909 b- defN 23-Jul-17 08:08 pkgUdit/pp.py
--rw-rw-rw-  2.0 fat     1079 b- defN 23-Jul-17 09:36 pkgUdit-0.0.5.dist-info/License.txt
--rw-rw-rw-  2.0 fat      352 b- defN 23-Jul-17 09:36 pkgUdit-0.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-17 09:36 pkgUdit-0.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-17 09:36 pkgUdit-0.0.5.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      533 b- defN 23-Jul-17 09:36 pkgUdit-0.0.5.dist-info/RECORD
-7 files, 3943 bytes uncompressed, 2175 bytes compressed:  44.8%
+Zip file size: 3074 bytes, number of entries: 7
+-rw-rw-rw-  2.0 fat      119 b- defN 23-Jul-18 17:40 pkgUdit/__init__.py
+-rw-rw-rw-  2.0 fat     1886 b- defN 23-Jul-18 17:16 pkgUdit/pswdGen.py
+-rw-rw-rw-  2.0 fat     1079 b- defN 23-Jul-18 17:48 pkgUdit-1.1.0.dist-info/License.txt
+-rw-rw-rw-  2.0 fat      352 b- defN 23-Jul-18 17:48 pkgUdit-1.1.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-18 17:48 pkgUdit-1.1.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       20 b- defN 23-Jul-18 17:48 pkgUdit-1.1.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      539 b- defN 23-Jul-18 17:48 pkgUdit-1.1.0.dist-info/RECORD
+7 files, 4087 bytes uncompressed, 2120 bytes compressed:  48.1%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: pkgUdit/__init__.py
 Comment: 
 
-Filename: pkgUdit/pp.py
+Filename: pkgUdit/pswdGen.py
 Comment: 
 
-Filename: pkgUdit-0.0.5.dist-info/License.txt
+Filename: pkgUdit-1.1.0.dist-info/License.txt
 Comment: 
 
-Filename: pkgUdit-0.0.5.dist-info/METADATA
+Filename: pkgUdit-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: pkgUdit-0.0.5.dist-info/WHEEL
+Filename: pkgUdit-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: pkgUdit-0.0.5.dist-info/top_level.txt
+Filename: pkgUdit-1.1.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pkgUdit-0.0.5.dist-info/RECORD
+Filename: pkgUdit-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pkgUdit/__init__.py

```diff
@@ -1,31 +1,8 @@
-import random
+from pswdGen import generatePass
 
-numerals = ['0','1','2','3','4','5','6','7','8','9']
-lowerCaps = ['a','b','c','d','e','f','g','h','i','j','k','l','m','n','o','p','q','r','s','t','u','v','w','x','y','z']
-upperChars = ['A','B','C','D','E','F','G','H','I','J','K','L','M','N','O','P','Q','R','S','T','U','V','W','X','Y','Z']
 
-combinedChars = numerals + lowerCaps + upperChars
 
+def generatePassword():
+    return generatePass()
 
-def custom_choice(combinedChars):
-    idx = random.randint(0, len(combinedChars)-1)
-    return combinedChars[idx]
-
-def make_random():
-    passLength = random.randint(6, 12)
-    password = []
-    password.append(random.choice(numerals))  # Include one numeric value
-    
-    for _ in range(passLength - 1):
-        password.append(custom_choice(combinedChars))
-    
-    random.shuffle(password)
-    return password
-
-def generatePass():
-    created_pass = make_random()
-    return ''.join(created_pass)
-
-# password = generatePass()
-# print(password)
-# print(len(password))
+print(generatePassword())
```

## Comparing `pkgUdit-0.0.5.dist-info/License.txt` & `pkgUdit-1.1.0.dist-info/License.txt`

 * *Files identical despite different names*

## Comparing `pkgUdit-0.0.5.dist-info/RECORD` & `pkgUdit-1.1.0.dist-info/RECORD`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-pkgUdit/__init__.py,sha256=hTd8PRmdhKm0vWRiOHDtP-Z9N29CLEOnIf7Jw9V_RUU,958
-pkgUdit/pp.py,sha256=ouqIsKO8SqYR1TP2NJxeq5d4TVZJl9s1TS3ozJPGNBQ,909
-pkgUdit-0.0.5.dist-info/License.txt,sha256=umiMrW63yKv-kGd3xCvjaxuSzBivxQgd5oZLf7eL9Zk,1079
-pkgUdit-0.0.5.dist-info/METADATA,sha256=XRkXFhYQcRzaSia90VvhCnqmRWHL-g8vu8oOhe-guSY,352
-pkgUdit-0.0.5.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pkgUdit-0.0.5.dist-info/top_level.txt,sha256=3CwC7EPEg2sf1KipgDsLRA_30qheFVMdK8cvKwak6Uw,20
-pkgUdit-0.0.5.dist-info/RECORD,,
+pkgUdit/__init__.py,sha256=FebOx85sZnHM_6ury04m4Saoce1tfynkXuwI1nWhRvg,119
+pkgUdit/pswdGen.py,sha256=5Le-udj_Abrm5a6W4PKMjGAuDvjFkXoBCIiRdk_hWZk,1886
+pkgUdit-1.1.0.dist-info/License.txt,sha256=umiMrW63yKv-kGd3xCvjaxuSzBivxQgd5oZLf7eL9Zk,1079
+pkgUdit-1.1.0.dist-info/METADATA,sha256=E3jgG2iQufWNTAL6p5ZhZb2eBaXvqYm9e3TaRxAYFzo,352
+pkgUdit-1.1.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pkgUdit-1.1.0.dist-info/top_level.txt,sha256=3CwC7EPEg2sf1KipgDsLRA_30qheFVMdK8cvKwak6Uw,20
+pkgUdit-1.1.0.dist-info/RECORD,,
```

