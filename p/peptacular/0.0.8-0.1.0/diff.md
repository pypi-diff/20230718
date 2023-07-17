# Comparing `tmp/peptacular-0.0.8.tar.gz` & `tmp/peptacular-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peptacular-0.0.8.tar", last modified: Thu Jul 13 00:21:30 2023, max compression
+gzip compressed data, was "peptacular-0.1.0.tar", last modified: Mon Jul 17 22:50:49 2023, max compression
```

## Comparing `peptacular-0.0.8.tar` & `peptacular-0.1.0.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:21:30.507984 peptacular-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-13 00:21:14.000000 peptacular-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-13 00:21:30.507984 peptacular-0.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-13 00:21:14.000000 peptacular-0.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-13 00:21:14.000000 peptacular-0.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-13 00:21:30.507984 peptacular-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-13 00:21:14.000000 peptacular-0.0.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:21:30.507984 peptacular-0.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:21:30.507984 peptacular-0.0.8/src/peptacular/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-13 00:21:14.000000 peptacular-0.0.8/src/peptacular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-13 00:21:14.000000 peptacular-0.0.8/src/peptacular/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-13 00:21:14.000000 peptacular-0.0.8/src/peptacular/protein.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-07-13 00:21:14.000000 peptacular-0.0.8/src/peptacular/refseq.py
--rw-r--r--   0 runner    (1001) docker     (123)    24967 2023-07-13 00:21:14.000000 peptacular-0.0.8/src/peptacular/sequence.py
--rw-r--r--   0 runner    (1001) docker     (123)      893 2023-07-13 00:21:14.000000 peptacular-0.0.8/src/peptacular/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:21:30.507984 peptacular-0.0.8/src/peptacular.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-13 00:21:30.000000 peptacular-0.0.8/src/peptacular.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-13 00:21:30.000000 peptacular-0.0.8/src/peptacular.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-13 00:21:30.000000 peptacular-0.0.8/src/peptacular.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-13 00:21:30.000000 peptacular-0.0.8/src/peptacular.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-13 00:21:30.000000 peptacular-0.0.8/src/peptacular.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-13 00:21:30.507984 peptacular-0.0.8/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    15094 2023-07-13 00:21:14.000000 peptacular-0.0.8/tests/test_peptide.py
--rw-r--r--   0 runner    (1001) docker     (123)     4412 2023-07-13 00:21:14.000000 peptacular-0.0.8/tests/test_protein.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-07-13 00:21:14.000000 peptacular-0.0.8/tests/test_refstring.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:50:49.383376 peptacular-0.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-17 22:50:36.000000 peptacular-0.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-17 22:50:49.383376 peptacular-0.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-07-17 22:50:36.000000 peptacular-0.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      862 2023-07-17 22:50:36.000000 peptacular-0.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 22:50:49.383376 peptacular-0.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-17 22:50:36.000000 peptacular-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:50:49.379376 peptacular-0.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:50:49.383376 peptacular-0.1.0/src/peptacular/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-17 22:50:36.000000 peptacular-0.1.0/src/peptacular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4711 2023-07-17 22:50:36.000000 peptacular-0.1.0/src/peptacular/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7990 2023-07-17 22:50:36.000000 peptacular-0.1.0/src/peptacular/mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-17 22:50:36.000000 peptacular-0.1.0/src/peptacular/protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18920 2023-07-17 22:50:36.000000 peptacular-0.1.0/src/peptacular/sequence.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13130 2023-07-17 22:50:36.000000 peptacular-0.1.0/src/peptacular/spans.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:50:49.383376 peptacular-0.1.0/src/peptacular.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3070 2023-07-17 22:50:49.000000 peptacular-0.1.0/src/peptacular.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-07-17 22:50:49.000000 peptacular-0.1.0/src/peptacular.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 22:50:49.000000 peptacular-0.1.0/src/peptacular.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-17 22:50:49.000000 peptacular-0.1.0/src/peptacular.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-17 22:50:49.000000 peptacular-0.1.0/src/peptacular.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 22:50:49.383376 peptacular-0.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-17 22:50:36.000000 peptacular-0.1.0/tests/test_mass.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10639 2023-07-17 22:50:36.000000 peptacular-0.1.0/tests/test_peptide.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4569 2023-07-17 22:50:36.000000 peptacular-0.1.0/tests/test_protein.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7174 2023-07-17 22:50:36.000000 peptacular-0.1.0/tests/test_spans.py
```

### Comparing `peptacular-0.0.8/LICENSE` & `peptacular-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.8/PKG-INFO` & `peptacular-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptacular
-Version: 0.0.8
+Version: 0.1.0
 Summary: Utility package for handling peptide and protein sequences
 Author-email: Patrick Garrett <pgarrett@scripps.edu>
 License: MIT License
         
         Copyright (c) 2023 Patrick Garrett
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `peptacular-0.0.8/README.md` & `peptacular-0.1.0/README.md`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.8/pyproject.toml` & `peptacular-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.8/src/peptacular/constants.py` & `peptacular-0.1.0/src/peptacular/constants.py`

 * *Files identical despite different names*

### Comparing `peptacular-0.0.8/src/peptacular/protein.py` & `peptacular-0.1.0/src/peptacular/protein.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
     Returns:
         list[int]: List of indexes where the peptide sequence starts in the protein sequence.
     """
     return [i.start() for i in re.finditer(peptide, protein)]
 
 
-def calculate_protein_coverage(protein: str, peptides: List[int]) -> List[int]:
+def calculate_protein_coverage(protein: str, peptides: List[str]) -> List[int]:
     """
     Calculate the coverage of a protein sequence by a list of peptides.
 
     The coverage is represented as a binary list where each position in the protein sequence is marked as 1 if it
     is covered by at least one peptide and 0 otherwise.
 
     Args:
```

### Comparing `peptacular-0.0.8/src/peptacular.egg-info/PKG-INFO` & `peptacular-0.1.0/src/peptacular.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: peptacular
-Version: 0.0.8
+Version: 0.1.0
 Summary: Utility package for handling peptide and protein sequences
 Author-email: Patrick Garrett <pgarrett@scripps.edu>
 License: MIT License
         
         Copyright (c) 2023 Patrick Garrett
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `peptacular-0.0.8/tests/test_protein.py` & `peptacular-0.1.0/tests/test_protein.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,70 +16,71 @@
 
         sites = [23, 31, 35, 42, 45, 47, 50, 56, 60, 62, 70, 73, 79, 88, 96]
 
         self.assertEqual(cleavage_sites, sites)
 
     def test_digest_protein(self):
         peptides = set(digest_sequence(sequence='TIDERTIDEKTIDE',
-                               enzyme_regexes=constants.PROTEASES['trypsin'],
-                               missed_cleavages=2,
-                               min_len=0,
-                               max_len=100,
-                               semi_enzymatic=False))
+                                       enzyme_regex=constants.PROTEASES['trypsin'],
+                                       missed_cleavages=2,
+                                       min_len=0,
+                                       max_len=100,
+                                       semi=False))
+
         self.assertEqual(peptides,
                          {'TIDER', 'TIDERTIDEK', 'TIDERTIDEKTIDE', 'TIDEK', 'TIDEKTIDE','TIDE'})
 
         peptides = set(digest_sequence(sequence='TIDERTIDEKTIDE',
-                               enzyme_regexes=constants.PROTEASES['trypsin'],
-                               missed_cleavages=1,
-                               min_len=0,
-                               max_len=100,
-                               semi_enzymatic=False))
+                                       enzyme_regex=constants.PROTEASES['trypsin'],
+                                       missed_cleavages=1,
+                                       min_len=0,
+                                       max_len=100,
+                                       semi=False))
         self.assertEqual(peptides, {'TIDER', 'TIDERTIDEK', 'TIDEK', 'TIDEKTIDE', 'TIDE'})
 
         peptides = set(digest_sequence(sequence='KTIDERTIDEKTIDE',
-                               enzyme_regexes=constants.PROTEASES['trypsin'],
-                               missed_cleavages=1,
-                               min_len=0,
-                               max_len=100,
-                               semi_enzymatic=False))
+                                       enzyme_regex=constants.PROTEASES['trypsin'],
+                                       missed_cleavages=1,
+                                       min_len=0,
+                                       max_len=100,
+                                       semi=False))
         self.assertEqual(peptides,
                          {'K', 'KTIDER', 'TIDER', 'TIDERTIDEK', 'TIDEK', 'TIDEKTIDE', 'TIDE'})
 
         peptides = set(digest_sequence(sequence='TIDERTIDEKTIDEK',
-                               enzyme_regexes=constants.PROTEASES['trypsin'],
-                               missed_cleavages=1,
-                               min_len=0,
-                               max_len=100,
-                               semi_enzymatic=False))
+                                       enzyme_regex=constants.PROTEASES['trypsin'],
+                                       missed_cleavages=1,
+                                       min_len=0,
+                                       max_len=100,
+                                       semi=False))
         self.assertEqual(peptides, {'TIDER', 'TIDERTIDEK', 'TIDEK', 'TIDEKTIDEK', 'TIDEK'})
 
         peptides = set(digest_sequence(sequence='TIDERTIDEKKTIDE',
-                               enzyme_regexes=constants.PROTEASES['trypsin'],
-                               missed_cleavages=1,
-                               min_len=0,
-                               max_len=100,
-                               semi_enzymatic=False))
+                                       enzyme_regex=constants.PROTEASES['trypsin'],
+                                       missed_cleavages=1,
+                                       min_len=0,
+                                       max_len=100,
+                                       semi=False))
         self.assertEqual(peptides,
                          {'TIDER', 'TIDERTIDEK', 'TIDEK', 'TIDEKK', 'K', 'KTIDE', 'TIDE'})
 
         peptides = set(digest_sequence(sequence='TIDERTIDEKTIDE',
-                                       enzyme_regexes=constants.PROTEASES['trypsin'],
+                                       enzyme_regex=constants.PROTEASES['trypsin'],
                                        missed_cleavages=0,
                                        min_len=0,
                                        max_len=100,
-                                       semi_enzymatic=False))
+                                       semi=False))
         self.assertEqual(peptides, {'TIDER', 'TIDEK', 'TIDE'})
 
         peptides = set(digest_sequence(sequence='TIDERTIDEKTIDE',
-                               enzyme_regexes=constants.PROTEASES['trypsin'],
-                               missed_cleavages=10,
-                               min_len=0,
-                               max_len=100,
-                               semi_enzymatic=False))
+                                       enzyme_regex=constants.PROTEASES['trypsin'],
+                                       missed_cleavages=10,
+                                       min_len=0,
+                                       max_len=100,
+                                       semi=False))
         self.assertEqual(peptides,
                          {'TIDER', 'TIDERTIDEK', 'TIDERTIDEKTIDE', 'TIDEK', 'TIDEKTIDE', 'TIDE'})
 
     def test_calculate_protein_coverage(self):
         protein_sequence = 'TIDERTIDEKTIDE'
         cov_arr = calculate_protein_coverage(protein=protein_sequence, peptides=['TIDER', 'TIDEK', 'TIDE'])
         self.assertEqual(sum(cov_arr), len(protein_sequence))
```

