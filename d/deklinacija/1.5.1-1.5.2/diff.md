# Comparing `tmp/deklinacija-1.5.1.tar.gz` & `tmp/deklinacija-1.5.2.tar.gz`

## Comparing `deklinacija-1.5.1.tar` & `deklinacija-1.5.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.5.1/.github/workflows/python-package.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.5.1/deklinacija/__init__.py
--rw-r--r--   0        0        0    21542 2020-02-02 00:00:00.000000 deklinacija-1.5.1/deklinacija/module.py
--rw-r--r--   0        0        0     5323 2020-02-02 00:00:00.000000 deklinacija-1.5.1/deklinacija/utils.py
--rw-r--r--   0        0        0     2758 2020-02-02 00:00:00.000000 deklinacija-1.5.1/deklinacija/vokativ_database.csv
--rw-r--r--   0        0        0     2547 2020-02-02 00:00:00.000000 deklinacija-1.5.1/tests/names_female.txt
--rw-r--r--   0        0        0     4360 2020-02-02 00:00:00.000000 deklinacija-1.5.1/tests/names_male.txt
--rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 deklinacija-1.5.1/tests/test_names.py
--rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 deklinacija-1.5.1/.gitignore
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.5.1/LICENSE
--rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 deklinacija-1.5.1/README.md
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.5.1/pyproject.toml
--rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 deklinacija-1.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1347 2020-02-02 00:00:00.000000 deklinacija-1.5.2/.github/workflows/python-package.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 deklinacija-1.5.2/deklinacija/__init__.py
+-rw-r--r--   0        0        0    21641 2020-02-02 00:00:00.000000 deklinacija-1.5.2/deklinacija/module.py
+-rw-r--r--   0        0        0     5512 2020-02-02 00:00:00.000000 deklinacija-1.5.2/deklinacija/utils.py
+-rw-r--r--   0        0        0     5986 2020-02-02 00:00:00.000000 deklinacija-1.5.2/deklinacija/vokativ_database.csv
+-rw-r--r--   0        0        0     3001 2020-02-02 00:00:00.000000 deklinacija-1.5.2/tests/names_female.txt
+-rw-r--r--   0        0        0     4658 2020-02-02 00:00:00.000000 deklinacija-1.5.2/tests/names_male.txt
+-rw-r--r--   0        0        0     1537 2020-02-02 00:00:00.000000 deklinacija-1.5.2/tests/test_names.py
+-rw-r--r--   0        0        0     3229 2020-02-02 00:00:00.000000 deklinacija-1.5.2/.gitignore
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 deklinacija-1.5.2/LICENSE
+-rw-r--r--   0        0        0     3326 2020-02-02 00:00:00.000000 deklinacija-1.5.2/README.md
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 deklinacija-1.5.2/pyproject.toml
+-rw-r--r--   0        0        0     3796 2020-02-02 00:00:00.000000 deklinacija-1.5.2/PKG-INFO
```

### Comparing `deklinacija-1.5.1/.github/workflows/python-package.yml` & `deklinacija-1.5.2/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.1/deklinacija/module.py` & `deklinacija-1.5.2/deklinacija/module.py`

 * *Files 0% similar despite different names*

```diff
@@ -485,27 +485,30 @@
                 name[-1] = "Е"
         return "".join(name)
 
     if utils.toCyrillic(name[-1].lower()) in ["о", "и", "у", "е"]:
         return "".join(name)
 
     if name[-1].lower() in ["a", "а"]:
-        if len(nameSep) <= 5:
+        if len(nameSep) <= 6:
             try:
                 if name[-1].isupper():
                     if utils.isLatin(name[-1]):
                         return rest+(utils.toLatin(utils.vokativ_db[utils.toCyrillic(utils.formatName(name))])[-1].upper())
                     else:
                         return rest+(utils.vokativ_db[utils.toCyrillic(utils.formatName(name))][-1].upper())
                 else:
                     if utils.isLatin(name[-1]):
                         return rest+(utils.toLatin(utils.vokativ_db[utils.toCyrillic(utils.formatName(name))])[-1])
                     else:
                         return rest+(utils.vokativ_db[utils.toCyrillic(utils.formatName(name))][-1])
             except KeyError:
+                if len(nameSep) == 6:
+                    return "".join(name)
+                
                 if name[-1].islower():
                     if utils.isLatin(name[-1]):
                         if name[-2].lower() in ["и", "i"]:
                             name.insert(-1, "j")
                         name[-1] = "o"
                     else:
                         if name[-2].lower() in ["и", "i"]:
```

### Comparing `deklinacija-1.5.1/deklinacija/utils.py` & `deklinacija-1.5.2/deklinacija/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -145,15 +145,18 @@
 
 def isZvucni(letter):
     if toCyrillic(letter.lower()) in ZVUCNI:
         return True
     else:
         return False
 
-# For converting the csv to cyrillic
+#Excel formula for filtering names shorter or equal to 5 characters and ending in cyrillic "а"
+#(assumes that names start from the second row): 
+# =FILTER(A2:B1970;(LEN(A2:A1970)<=5)*(RIGHT(A2:A1970)="а"))
+#For converting the csv to cyrillic:
 # with open('deklinacija/vokativ_database.csv',"r+",encoding="utf-8") as f:
 
 #     reader = dict(csv.reader(f, delimiter=","))
 #     converted = {}
 #     text = ""
 
 #     for (k,v) in reader.items():
@@ -162,24 +165,22 @@
 #         text = text + kConverted + "," + vConverted + "\n"
 
 #     f.truncate(0)
 #     f.write(text)
 
 
 def formatName(word):
+    if type(word) == list:
+        word = "".join(word).lower()
     word = list(word)
     word[0] = word[0].upper()
-    n = 1
-    while n < len(word):
-        word[n] = word[n].lower()
-        n += 1
     return "".join(word)
 
 
 module_path = os.path.abspath(__file__)
 
 module_directory = os.path.dirname(module_path)
 
 csv_file_path = os.path.join(module_directory, 'vokativ_database.csv')
 
 with open(csv_file_path, "r", encoding="utf-8") as file:
-    vokativ_db = dict(csv.reader(file, delimiter=","))
+    vokativ_db = dict(csv.reader(file, delimiter=";"))
```

### Comparing `deklinacija-1.5.1/tests/names_female.txt` & `deklinacija-1.5.2/tests/names_female.txt`

 * *Files 16% similar despite different names*

```diff
@@ -8,8 +8,11 @@
 {'nominativ': 'Daria', 'genitiv': 'Darije', 'dativ': 'Dariji', 'akuzativ': 'Dariju', 'vokativ': 'Daria', 'instrumental': 'Darijom', 'lokativ': 'Dariji'}
 {'nominativ': 'Anžujska', 'genitiv': 'Anžujske', 'dativ': 'Anžujskoj', 'akuzativ': 'Anžujsku', 'vokativ': 'Anžujska', 'instrumental': 'Anžujskom', 'lokativ': 'Anžujskoj'}
 {'nominativ': 'Subotički', 'genitiv': 'Subotički', 'dativ': 'Subotički', 'akuzativ': 'Subotički', 'vokativ': 'Subotički', 'instrumental': 'Subotički', 'lokativ': 'Subotički'}
 {'nominativ': 'Petka', 'genitiv': 'Petke', 'dativ': 'Petkoj', 'akuzativ': 'Petku', 'vokativ': 'Petko', 'instrumental': 'Petkom', 'lokativ': 'Petkoj'}
 {'nominativ': 'Lana Petrović', 'genitiv': 'Lane Petrović', 'dativ': 'Lani Petrović', 'akuzativ': 'Lanu Petrović', 'vokativ': 'Lano Petrović', 'instrumental': 'Lanom Petrović', 'lokativ': 'Lani Petrović'}
 {'nominativ': 'Sandra Anžujska', 'genitiv': 'Sandre Anžujske', 'dativ': 'Sandri Anžujskoj', 'akuzativ': 'Sandru Anžujsku', 'vokativ': 'Sandra Anžujska', 'instrumental': 'Sandrom Anžujskom', 'lokativ': 'Sandri Anžujskoj'}
 {'nominativ': 'Milica Tabova', 'genitiv': 'Milice Tabove', 'dativ': 'Milici Tabovoj', 'akuzativ': 'Milicu Tabovu', 'vokativ': 'Milice Tabova', 'instrumental': 'Milicom Tabovom', 'lokativ': 'Milici Tabovoj'}
-{'nominativ': 'Milica Releva', 'genitiv': 'Milice Releve', 'dativ': 'Milici Relevoj', 'akuzativ': 'Milicu Relevu', 'vokativ': 'Milice Releva', 'instrumental': 'Milicom Relevom', 'lokativ': 'Milici Relevoj'}
+{'nominativ': 'Milica Releva', 'genitiv': 'Milice Releve', 'dativ': 'Milici Relevoj', 'akuzativ': 'Milicu Relevu', 'vokativ': 'Milice Releva', 'instrumental': 'Milicom Relevom', 'lokativ': 'Milici Relevoj'}
+{'nominativ': 'Ivana', 'genitiv': 'Ivane', 'dativ': 'Ivani', 'akuzativ': 'Ivanu', 'vokativ': 'Ivana', 'instrumental': 'Ivanom', 'lokativ': 'Ivani'}
+{'nominativ': 'IVANA', 'genitiv': 'IVANE', 'dativ': 'IVANI', 'akuzativ': 'IVANU', 'vokativ': 'IVANA', 'instrumental': 'IVANOM', 'lokativ': 'IVANI'}
+{'nominativ': 'STRUJA', 'genitiv': 'STRUJE', 'dativ': 'STRUJI', 'akuzativ': 'STRUJU', 'vokativ': 'STRUJO', 'instrumental': 'STRUJOM', 'lokativ': 'STRUJI'}
```

### Comparing `deklinacija-1.5.1/tests/names_male.txt` & `deklinacija-1.5.2/tests/names_male.txt`

 * *Files 2% similar despite different names*

```diff
@@ -19,8 +19,10 @@
 {'nominativ': 'Opanak', 'genitiv': 'Opanka', 'dativ': 'Opanku', 'akuzativ': 'Opanka', 'vokativ': 'Opanku', 'instrumental': 'Opankom', 'lokativ': 'Opanku'}
 {'nominativ': 'Vlah', 'genitiv': 'Vlaha', 'dativ': 'Vlahu', 'akuzativ': 'Vlaha', 'vokativ': 'Vlaše', 'instrumental': 'Vlahom', 'lokativ': 'Vlahu'}
 {'nominativ': 'Subotički', 'genitiv': 'Subotičkog', 'dativ': 'Subotičkom', 'akuzativ': 'Subotičkog', 'vokativ': 'Subotički', 'instrumental': 'Subotičkim', 'lokativ': 'Subotičkom'}
 {'nominativ': 'Niški', 'genitiv': 'Niškog', 'dativ': 'Niškom', 'akuzativ': 'Niškog', 'vokativ': 'Niški', 'instrumental': 'Niškim', 'lokativ': 'Niškom'}
 {'nominativ': 'Srpski', 'genitiv': 'Srpskog', 'dativ': 'Srpskom', 'akuzativ': 'Srpskog', 'vokativ': 'Srpski', 'instrumental': 'Srpskim', 'lokativ': 'Srpskom'}
 {'nominativ': 'Dario Subotički', 'genitiv': 'Darija Subotičkog', 'dativ': 'Dariju Subotičkom', 'akuzativ': 'Darija Subotičkog', 'vokativ': 'Dario Subotički', 'instrumental': 'Darijem Subotičkim', 'lokativ': 'Dariju Subotičkom'}       
 {'nominativ': 'Minja Niški', 'genitiv': 'Minje Niškog', 'dativ': 'Minji Niškom', 'akuzativ': 'Minju Niškog', 'vokativ': 'Minja Niški', 'instrumental': 'Minjom Niškim', 'lokativ': 'Minji Niškom'}
-{'nominativ': 'Miki Srpski', 'genitiv': 'Mikija Srpskog', 'dativ': 'Mikiju Srpskom', 'akuzativ': 'Mikija Srpskog', 'vokativ': 'Miki Srpski', 'instrumental': 'Mikijem Srpskim', 'lokativ': 'Mikiju Srpskom'}
+{'nominativ': 'Miki Srpski', 'genitiv': 'Mikija Srpskog', 'dativ': 'Mikiju Srpskom', 'akuzativ': 'Mikija Srpskog', 'vokativ': 'Miki Srpski', 'instrumental': 'Mikijem Srpskim', 'lokativ': 'Mikiju Srpskom'}
+{'nominativ': 'RELJA', 'genitiv': 'RELJE', 'dativ': 'RELJI', 'akuzativ': 'RELJU', 'vokativ': 'RELJA', 'instrumental': 'RELJOM', 'lokativ': 'RELJI'}
+{'nominativ': 'ALEK', 'genitiv': 'ALEKA', 'dativ': 'ALEKU', 'akuzativ': 'ALEKA', 'vokativ': 'ALEČE', 'instrumental': 'ALEKOM', 'lokativ': 'ALEKU'}
```

### Comparing `deklinacija-1.5.1/tests/test_names.py` & `deklinacija-1.5.2/tests/test_names.py`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.1/.gitignore` & `deklinacija-1.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.1/LICENSE` & `deklinacija-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.1/README.md` & `deklinacija-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `deklinacija-1.5.1/pyproject.toml` & `deklinacija-1.5.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "deklinacija"
-version = "1.5.1"
+version = "1.5.2"
 authors = [
   { name="urelja", email="code.relja@gmail.com" },
 ]
 description = "A Python library for declension of personal names in Serbian"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `deklinacija-1.5.1/PKG-INFO` & `deklinacija-1.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deklinacija
-Version: 1.5.1
+Version: 1.5.2
 Summary: A Python library for declension of personal names in Serbian
 Project-URL: Homepage, https://github.com/urelja/deklinacija
 Project-URL: Bug Tracker, https://github.com/urelja/deklinacija/issues
 Author-email: urelja <code.relja@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

