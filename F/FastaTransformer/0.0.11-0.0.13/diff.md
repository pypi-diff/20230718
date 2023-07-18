# Comparing `tmp/FastaTransformer-0.0.11.tar.gz` & `tmp/FastaTransformer-0.0.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FastaTransformer-0.0.11.tar", last modified: Thu Jun 15 18:11:40 2023, max compression
+gzip compressed data, was "FastaTransformer-0.0.13.tar", last modified: Tue Jul 18 21:41:29 2023, max compression
```

## Comparing `FastaTransformer-0.0.11.tar` & `FastaTransformer-0.0.13.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-15 18:11:40.884285 FastaTransformer-0.0.11/
--rw-rw-rw-   0        0        0     4241 2023-06-15 18:11:40.885290 FastaTransformer-0.0.11/PKG-INFO
--rw-rw-rw-   0        0        0     3672 2023-06-15 18:00:21.000000 FastaTransformer-0.0.11/README.md
--rw-rw-rw-   0        0        0      150 2023-05-30 20:49:19.000000 FastaTransformer-0.0.11/pyproject.toml
--rw-rw-rw-   0        0        0      729 2023-06-15 18:11:40.893304 FastaTransformer-0.0.11/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-15 18:11:40.846190 FastaTransformer-0.0.11/src/
-drwxrwxrwx   0        0        0        0 2023-06-15 18:11:40.855214 FastaTransformer-0.0.11/src/CigarBreaker/
--rw-rw-rw-   0        0        0     7061 2023-06-15 17:45:36.000000 FastaTransformer-0.0.11/src/CigarBreaker/CigarBreaker.py
--rw-rw-rw-   0        0        0       39 2023-06-15 16:53:41.000000 FastaTransformer-0.0.11/src/CigarBreaker/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:11:40.860225 FastaTransformer-0.0.11/src/FastaTransformer/
--rw-rw-rw-   0        0        0    49409 2023-06-14 19:52:04.000000 FastaTransformer-0.0.11/src/FastaTransformer/FastaTransformer.py
--rw-rw-rw-   0        0        0       99 2023-06-15 16:54:04.000000 FastaTransformer-0.0.11/src/FastaTransformer/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-15 18:11:40.883282 FastaTransformer-0.0.11/src/FastaTransformer.egg-info/
--rw-rw-rw-   0        0        0     4241 2023-06-15 18:11:40.000000 FastaTransformer-0.0.11/src/FastaTransformer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      346 2023-06-15 18:11:40.000000 FastaTransformer-0.0.11/src/FastaTransformer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-15 18:11:40.000000 FastaTransformer-0.0.11/src/FastaTransformer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2023-06-15 18:11:40.000000 FastaTransformer-0.0.11/src/FastaTransformer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-18 21:41:29.380398 FastaTransformer-0.0.13/
+-rw-rw-rw-   0        0        0     4272 2023-07-18 21:41:29.381415 FastaTransformer-0.0.13/PKG-INFO
+-rw-rw-rw-   0        0        0     3703 2023-06-15 18:18:59.000000 FastaTransformer-0.0.13/README.md
+-rw-rw-rw-   0        0        0      150 2023-05-30 20:49:19.000000 FastaTransformer-0.0.13/pyproject.toml
+-rw-rw-rw-   0        0        0      729 2023-07-18 21:41:29.389429 FastaTransformer-0.0.13/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-07-18 21:41:29.336400 FastaTransformer-0.0.13/src/
+drwxrwxrwx   0        0        0        0 2023-07-18 21:41:29.347400 FastaTransformer-0.0.13/src/CigarBreaker/
+-rw-rw-rw-   0        0        0     7061 2023-06-15 17:45:36.000000 FastaTransformer-0.0.13/src/CigarBreaker/CigarBreaker.py
+-rw-rw-rw-   0        0        0       39 2023-06-15 16:53:41.000000 FastaTransformer-0.0.13/src/CigarBreaker/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:41:29.352396 FastaTransformer-0.0.13/src/FastaTransformer/
+-rw-rw-rw-   0        0        0    50118 2023-07-18 21:36:59.000000 FastaTransformer-0.0.13/src/FastaTransformer/FastaTransformer.py
+-rw-rw-rw-   0        0        0       99 2023-06-15 16:54:04.000000 FastaTransformer-0.0.13/src/FastaTransformer/__init__.py
+drwxrwxrwx   0        0        0        0 2023-07-18 21:41:29.378397 FastaTransformer-0.0.13/src/FastaTransformer.egg-info/
+-rw-rw-rw-   0        0        0     4272 2023-07-18 21:41:29.000000 FastaTransformer-0.0.13/src/FastaTransformer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      346 2023-07-18 21:41:29.000000 FastaTransformer-0.0.13/src/FastaTransformer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 21:41:29.000000 FastaTransformer-0.0.13/src/FastaTransformer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2023-07-18 21:41:29.000000 FastaTransformer-0.0.13/src/FastaTransformer.egg-info/top_level.txt
```

### Comparing `FastaTransformer-0.0.11/PKG-INFO` & `FastaTransformer-0.0.13/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastaTransformer
-Version: 0.0.11
+Version: 0.0.13
 Summary: This package helps resolve bioprogramming problems
 Home-page: https://github.com/Global-ASFV-Research-Alliance/FastaTransformer
 Author: MDinhobl
 Author-email: markdinhobl@gmail.com
 Project-URL: Bug Tracker, https://github.com/Global-ASFV-Research-Alliance/FastaTransformer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 
 # FastaTransformer
 FastaTransformer is a python toolset containing fucntions to simplify the usage of .fasta files in analysis as well as transform them into useful states for other tools.
 
 ### Authors
 
-The primary author of the FastaTransformer package is MDinhobl.
+The primary author of the FastaTransformer package is [MDinhobl](https://github.com/MDinhobl).
 
 ## Major Functions
 The following list contains the most useful functions of FastaTransformer.
 
 ### Creating Data Folders
 
 1. **MakeGeneBank** - Take a CSV or pandas Dataframe with columns representing Genomes, Gene (or other category), and Sequence and create a folder of .fasta files for each Gene (or chosen category).
```

### Comparing `FastaTransformer-0.0.11/README.md` & `FastaTransformer-0.0.13/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # FastaTransformer
 FastaTransformer is a python toolset containing fucntions to simplify the usage of .fasta files in analysis as well as transform them into useful states for other tools.
 
 ### Authors
 
-The primary author of the FastaTransformer package is MDinhobl.
+The primary author of the FastaTransformer package is [MDinhobl](https://github.com/MDinhobl).
 
 ## Major Functions
 The following list contains the most useful functions of FastaTransformer.
 
 ### Creating Data Folders
 
 1. **MakeGeneBank** - Take a CSV or pandas Dataframe with columns representing Genomes, Gene (or other category), and Sequence and create a folder of .fasta files for each Gene (or chosen category).
```

### Comparing `FastaTransformer-0.0.11/setup.cfg` & `FastaTransformer-0.0.13/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2046 6173 7461 5472 616e 7366 6f72   = FastaTransfor
 00000020: 6d65 720d 0a76 6572 7369 6f6e 203d 2030  mer..version = 0
-00000030: 2e30 2e31 310d 0a61 7574 686f 7220 3d20  .0.11..author = 
+00000030: 2e30 2e31 330d 0a61 7574 686f 7220 3d20  .0.13..author = 
 00000040: 4d44 696e 686f 626c 0d0a 6175 7468 6f72  MDinhobl..author
 00000050: 5f65 6d61 696c 203d 206d 6172 6b64 696e  _email = markdin
 00000060: 686f 626c 4067 6d61 696c 2e63 6f6d 0d0a  hobl@gmail.com..
 00000070: 6465 7363 7269 7074 696f 6e20 3d20 5468  description = Th
 00000080: 6973 2070 6163 6b61 6765 2068 656c 7073  is package helps
 00000090: 2072 6573 6f6c 7665 2062 696f 7072 6f67   resolve bioprog
 000000a0: 7261 6d6d 696e 6720 7072 6f62 6c65 6d73  ramming problems
```

### Comparing `FastaTransformer-0.0.11/src/CigarBreaker/CigarBreaker.py` & `FastaTransformer-0.0.13/src/CigarBreaker/CigarBreaker.py`

 * *Files identical despite different names*

### Comparing `FastaTransformer-0.0.11/src/FastaTransformer/FastaTransformer.py` & `FastaTransformer-0.0.13/src/FastaTransformer/FastaTransformer.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,18 +124,27 @@
     keys = Groups.groups.keys()
 
     FastaBank = FolderPathFixer(FastaBank)
 
     BugBank = pd.DataFrame(columns=[Seq, Grouping, ID])
     for name, group in Groups:
         
-        if len(group[group.duplicated([ID], keep=False)]) > 0:
+        try:
+            if len(group[group.duplicated([ID], keep=False)]) > 0:
                 print(group[group.duplicated([ID], keep=False)].drop(['Unnamed: 0'], axis=1))
                 BugBank = pd.concat([BugBank,(group[group.duplicated([ID], keep=False)]).drop(['Unnamed: 0'], axis=1)])
-
+        except:
+            try:
+                if len(group[group.duplicated([ID], keep=False)]) > 0:
+                    BugBank = pd.concat([BugBank,group[group.duplicated([ID], keep = False)]])
+                    group = group.drop_duplicates([ID], keep=False)
+            except:
+                print("Failed to run, likely duplicates with " + name + " , skipping")
+                continue
+            
         for index, row in group.iterrows():        
             outputname_fasta = FastaBank + str(name).replace('/', '-') + ".fasta"
             try:
                 if DeleteStar == True:
                     row[Seq] = row[Seq].split('*', 1)[0]
 
                 with open(outputname_fasta, "a") as f:
@@ -184,15 +193,14 @@
     """
     FastaBank = FolderPathFixer(FastaBank)
     AlignmentBank = FolderPathFixer(AlignmentBank)
     
     import glob
     my_files = glob.glob(FastaBank + '*')
     for fasta in my_files:
-        #fasta = fasta.replace("\\", "/")
         ouputfasta = fasta.replace(FastaBank, AlignmentBank)
         FastaToAlignment(fasta, ouputfasta, musclepath, gapextpenalty = gapextpenalty,gapopenpenalty = gapopenpenalty)
 
 def InputToList(Object, Keyword = None):
 
     """Take a list, a pd.Series, or a pd.DataFrame with a specific keyword and return a list of unique strings in that list. Used in this package to prevent failures caused by different uplaod types. Used as a starting function in other functions to help put parameters into a correct format.
     
@@ -360,32 +368,40 @@
 
         AllSequences = []
         for sequence in list(map(''.join, zip(*Old_df['sequence']))):
             AllSequences.append('.'.join([i + "#" + str(sequence.count(i)) for i in set(sequence)]))
         
         def FindFlaw(Sequence, CompareSequences, Spec_Seq = None):
             Flaw = []
-            for i in range(len(Sequence)):
-                if Sequence[i] not in CompareSequences[i]:
-                    
-                    if Spec_Seq == None:
-                        SSinfo = ""
-                    else:
-                        SSinfo =  "(RefAA)"+Spec_Seq[i] + " " + "(RefPos)"+str(len(Spec_Seq[:i+1].replace("-",""))) + " "
-
-                    Flaw.append(SSinfo + "(Old)" + CompareSequences[i]+ " " + "(AlignPos)" + str(i+1) + " " + "(SelfPos)" + str(len(Sequence[:i+1].replace("-",""))) + " " + "(SelfAA)" + Sequence[i])
-            if len(Sequence) == 0:
-                return "NA"
-            if len(Flaw) == 0:
-                return ""
-            return Flaw
+            try:
+                for i in range(len(Sequence)):
+                    if Sequence[i] not in CompareSequences[i]:
+                        
+                        if Spec_Seq == None:
+                            SSinfo = ""
+                        else:
+                            SSinfo =  "(RefAA)"+Spec_Seq[i] + " " + "(RefPos)"+str(len(Spec_Seq[:i+1].replace("-",""))) + " "
+
+                        Flaw.append(SSinfo + "(Old)" + CompareSequences[i]+ " " + "(AlignPos)" + str(i+1) + " " + "(SelfPos)" + str(len(Sequence[:i+1].replace("-",""))) + " " + "(SelfAA)" + Sequence[i])
+                if len(Sequence) == 0:
+                    return "NA"
+                if len(Flaw) == 0:
+                    return ""
+                return Flaw
+            except:
+                print("Failed At FindFlaw on " + fasta)
+                return "ERROR"
         
-        results = pd.DataFrame()
-        results[str(gene)] = New_df['sequence'].map(lambda x: FindFlaw(x, AllSequences, Spec_Seq))
-        FinalFrame = pd.concat([FinalFrame,results], axis=1)
+        try:
+            results = pd.DataFrame()
+            results[str(gene)] = New_df['sequence'].map(lambda x: FindFlaw(x, AllSequences, Spec_Seq))
+            FinalFrame = pd.concat([FinalFrame,results], axis=1)
+        except:
+            print("Failed at Final Frame Concatonation at " + fasta)
+            continue
 
     return FinalFrame
 
 def AlignmentChangeFinderSelector(df, GeneList = None, DropNA = True):
     
     """
     A function that selects the specific outputs of the :func:`AlignmentChangeFinder` that are desired.
```

### Comparing `FastaTransformer-0.0.11/src/FastaTransformer.egg-info/PKG-INFO` & `FastaTransformer-0.0.13/src/FastaTransformer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FastaTransformer
-Version: 0.0.11
+Version: 0.0.13
 Summary: This package helps resolve bioprogramming problems
 Home-page: https://github.com/Global-ASFV-Research-Alliance/FastaTransformer
 Author: MDinhobl
 Author-email: markdinhobl@gmail.com
 Project-URL: Bug Tracker, https://github.com/Global-ASFV-Research-Alliance/FastaTransformer
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -13,15 +13,15 @@
 Description-Content-Type: text/markdown
 
 # FastaTransformer
 FastaTransformer is a python toolset containing fucntions to simplify the usage of .fasta files in analysis as well as transform them into useful states for other tools.
 
 ### Authors
 
-The primary author of the FastaTransformer package is MDinhobl.
+The primary author of the FastaTransformer package is [MDinhobl](https://github.com/MDinhobl).
 
 ## Major Functions
 The following list contains the most useful functions of FastaTransformer.
 
 ### Creating Data Folders
 
 1. **MakeGeneBank** - Take a CSV or pandas Dataframe with columns representing Genomes, Gene (or other category), and Sequence and create a folder of .fasta files for each Gene (or chosen category).
```

