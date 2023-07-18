# Comparing `tmp/featurExtract-0.2.5.6.tar.gz` & `tmp/featurExtract-0.2.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/featurExtract-0.2.5.6.tar", last modified: Tue Jun 20 08:00:30 2023, max compression
+gzip compressed data, was "dist/featurExtract-0.2.5.7.tar", last modified: Tue Jul 18 11:54:18 2023, max compression
```

## Comparing `featurExtract-0.2.5.6.tar` & `featurExtract-0.2.5.7.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/
--rw-r--r--   0 zhusitao   (501) staff       (20)       18 2021-08-20 08:13:20.000000 featurExtract-0.2.5.6/MANIFEST.in
--rw-r--r--   0 zhusitao   (501) staff       (20)     3472 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/PKG-INFO
--rw-r--r--   0 zhusitao   (501) staff       (20)     3117 2022-08-04 14:50:42.000000 featurExtract-0.2.5.6/README.md
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract/
--rw-r--r--   0 zhusitao   (501) staff       (20)      248 2021-07-22 09:50:56.000000 featurExtract-0.2.5.6/featurExtract/__init__.py
--rw-r--r--   0 zhusitao   (501) staff       (20)      272 2021-12-19 03:41:05.000000 featurExtract-0.2.5.6/featurExtract/a.py
--rw-r--r--   0 zhusitao   (501) staff       (20)      690 2023-06-15 02:49:42.000000 featurExtract-0.2.5.6/featurExtract/b.py
--rw-r--r--   0 zhusitao   (501) staff       (20)      439 2023-06-15 02:52:56.000000 featurExtract-0.2.5.6/featurExtract/c.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     1928 2021-08-20 07:44:38.000000 featurExtract-0.2.5.6/featurExtract/command_gb.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     2364 2021-08-24 01:51:44.000000 featurExtract-0.2.5.6/featurExtract/command_gff.py
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract/commands/
--rw-r--r--   0 zhusitao   (501) staff       (20)        0 2021-08-20 09:48:06.000000 featurExtract-0.2.5.6/featurExtract/commands/__init__.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     8211 2023-06-09 11:34:14.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_CDS.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     4655 2022-08-10 09:02:03.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_IGR.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     5090 2023-06-09 11:30:09.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_UTR.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)    13110 2022-07-12 14:15:50.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_cdna.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)    15340 2023-06-20 06:45:18.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_dORF.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     4035 2022-07-14 04:14:36.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_exon.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     3353 2022-07-14 04:20:57.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_gene.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     3342 2022-07-14 06:23:32.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_intron.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     7533 2022-07-14 06:48:00.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_mRNA.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     5160 2022-07-14 07:14:56.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_promoter.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     1361 2021-08-20 09:54:37.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_rRNA.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     1360 2021-08-20 09:54:58.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_tRNA.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     5576 2022-07-14 07:30:41.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_terminator.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)    28563 2023-06-20 06:50:08.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_uORF.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)    32658 2023-06-15 02:27:15.000000 featurExtract-0.2.5.6/featurExtract/commands/extract_uORF_back.py
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract/database/
--rwxr-xr-x   0 zhusitao   (501) staff       (20)      572 2021-07-22 09:50:56.000000 featurExtract-0.2.5.6/featurExtract/database/database.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)    18014 2023-06-20 02:34:25.000000 featurExtract-0.2.5.6/featurExtract/feature_extract.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     7561 2021-08-20 07:50:44.000000 featurExtract-0.2.5.6/featurExtract/genBank_extract.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)     3152 2021-07-22 09:50:56.000000 featurExtract-0.2.5.6/featurExtract/parameter.py
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract/utils/
--rw-r--r--   0 zhusitao   (501) staff       (20)        0 2021-08-20 03:25:23.000000 featurExtract-0.2.5.6/featurExtract/utils/__init__.py
--rw-r--r--   0 zhusitao   (501) staff       (20)      125 2021-08-20 09:23:21.000000 featurExtract-0.2.5.6/featurExtract/utils/coverage.py
--rw-r--r--   0 zhusitao   (501) staff       (20)     2326 2021-08-20 03:52:32.000000 featurExtract-0.2.5.6/featurExtract/utils/util.py
--rw-r--r--   0 zhusitao   (501) staff       (20)    16597 2023-06-20 06:34:08.000000 featurExtract-0.2.5.6/featurExtract/utils/visualize.py
--rwxr-xr-x   0 zhusitao   (501) staff       (20)       24 2023-06-20 07:59:58.000000 featurExtract-0.2.5.6/featurExtract/version.py
-drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract.egg-info/
--rw-r--r--   0 zhusitao   (501) staff       (20)     3472 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract.egg-info/PKG-INFO
--rw-r--r--   0 zhusitao   (501) staff       (20)     1306 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract.egg-info/SOURCES.txt
--rw-r--r--   0 zhusitao   (501) staff       (20)        1 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract.egg-info/dependency_links.txt
--rw-r--r--   0 zhusitao   (501) staff       (20)      113 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract.egg-info/entry_points.txt
--rw-r--r--   0 zhusitao   (501) staff       (20)       80 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract.egg-info/requires.txt
--rw-r--r--   0 zhusitao   (501) staff       (20)       14 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/featurExtract.egg-info/top_level.txt
--rw-r--r--   0 zhusitao   (501) staff       (20)       38 2023-06-20 08:00:30.000000 featurExtract-0.2.5.6/setup.cfg
--rw-r--r--   0 zhusitao   (501) staff       (20)     1283 2021-08-20 10:06:18.000000 featurExtract-0.2.5.6/setup.py
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-07-18 11:54:18.000000 featurExtract-0.2.5.7/
+-rw-r--r--   0 zhusitao   (501) staff       (20)       18 2021-08-20 08:13:20.000000 featurExtract-0.2.5.7/MANIFEST.in
+-rw-r--r--   0 zhusitao   (501) staff       (20)     3472 2023-07-18 11:54:18.000000 featurExtract-0.2.5.7/PKG-INFO
+-rw-r--r--   0 zhusitao   (501) staff       (20)     3117 2022-08-04 14:50:42.000000 featurExtract-0.2.5.7/README.md
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-07-18 11:54:18.000000 featurExtract-0.2.5.7/featurExtract/
+-rw-r--r--   0 zhusitao   (501) staff       (20)      248 2021-07-22 09:50:56.000000 featurExtract-0.2.5.7/featurExtract/__init__.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)      272 2021-12-19 03:41:05.000000 featurExtract-0.2.5.7/featurExtract/a.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)      690 2023-06-15 02:49:42.000000 featurExtract-0.2.5.7/featurExtract/b.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)      439 2023-06-15 02:52:56.000000 featurExtract-0.2.5.7/featurExtract/c.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     1928 2021-08-20 07:44:38.000000 featurExtract-0.2.5.7/featurExtract/command_gb.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     2376 2023-07-18 11:52:09.000000 featurExtract-0.2.5.7/featurExtract/command_gff.py
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-07-18 11:54:18.000000 featurExtract-0.2.5.7/featurExtract/commands/
+-rw-r--r--   0 zhusitao   (501) staff       (20)        0 2021-08-20 09:48:06.000000 featurExtract-0.2.5.7/featurExtract/commands/__init__.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     6926 2023-06-21 10:10:54.000000 featurExtract-0.2.5.7/featurExtract/commands/extract_CDS.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     4655 2022-08-10 09:02:03.000000 featurExtract-0.2.5.7/featurExtract/commands/extract_IGR.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     4529 2023-06-23 02:34:56.000000 featurExtract-0.2.5.7/featurExtract/commands/extract_UTR.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)    13835 2023-06-21 11:30:00.000000 featurExtract-0.2.5.7/featurExtract/commands/extract_dORF.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     3703 2023-06-23 02:38:56.000000 featurExtract-0.2.5.7/featurExtract/commands/extract_exon.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     3353 2022-07-14 04:20:57.000000 featurExtract-0.2.5.7/featurExtract/commands/extract_gene.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     3342 2022-07-14 06:23:32.000000 featurExtract-0.2.5.7/featurExtract/commands/extract_intron.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     7533 2022-07-14 06:48:00.000000 featurExtract-0.2.5.7/featurExtract/commands/extract_mRNA.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     3577 2023-06-21 13:24:24.000000 featurExtract-0.2.5.7/featurExtract/commands/extract_promoter.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     1361 2021-08-20 09:54:37.000000 featurExtract-0.2.5.7/featurExtract/commands/extract_rRNA.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     1360 2021-08-20 09:54:58.000000 featurExtract-0.2.5.7/featurExtract/commands/extract_tRNA.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     5576 2022-07-14 07:30:41.000000 featurExtract-0.2.5.7/featurExtract/commands/extract_terminator.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)    10831 2023-07-18 11:39:38.000000 featurExtract-0.2.5.7/featurExtract/commands/extract_transcript.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)    26977 2023-06-21 10:11:57.000000 featurExtract-0.2.5.7/featurExtract/commands/extract_uORF.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)    32658 2023-06-15 02:27:15.000000 featurExtract-0.2.5.7/featurExtract/commands/extract_uORF_back.py
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-07-18 11:54:18.000000 featurExtract-0.2.5.7/featurExtract/database/
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)      518 2023-06-21 13:26:48.000000 featurExtract-0.2.5.7/featurExtract/database/database.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)    20128 2023-07-18 11:38:11.000000 featurExtract-0.2.5.7/featurExtract/feature_extract.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     7561 2021-08-20 07:50:44.000000 featurExtract-0.2.5.7/featurExtract/genBank_extract.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)     3152 2021-07-22 09:50:56.000000 featurExtract-0.2.5.7/featurExtract/parameter.py
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-07-18 11:54:18.000000 featurExtract-0.2.5.7/featurExtract/utils/
+-rw-r--r--   0 zhusitao   (501) staff       (20)        0 2021-08-20 03:25:23.000000 featurExtract-0.2.5.7/featurExtract/utils/__init__.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)      125 2021-08-20 09:23:21.000000 featurExtract-0.2.5.7/featurExtract/utils/coverage.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)     3887 2023-06-23 02:33:02.000000 featurExtract-0.2.5.7/featurExtract/utils/util.py
+-rw-r--r--   0 zhusitao   (501) staff       (20)    16597 2023-06-20 06:34:08.000000 featurExtract-0.2.5.7/featurExtract/utils/visualize.py
+-rwxr-xr-x   0 zhusitao   (501) staff       (20)       24 2023-07-18 11:54:04.000000 featurExtract-0.2.5.7/featurExtract/version.py
+drwxr-xr-x   0 zhusitao   (501) staff       (20)        0 2023-07-18 11:54:18.000000 featurExtract-0.2.5.7/featurExtract.egg-info/
+-rw-r--r--   0 zhusitao   (501) staff       (20)     3472 2023-07-18 11:54:18.000000 featurExtract-0.2.5.7/featurExtract.egg-info/PKG-INFO
+-rw-r--r--   0 zhusitao   (501) staff       (20)     1312 2023-07-18 11:54:18.000000 featurExtract-0.2.5.7/featurExtract.egg-info/SOURCES.txt
+-rw-r--r--   0 zhusitao   (501) staff       (20)        1 2023-07-18 11:54:18.000000 featurExtract-0.2.5.7/featurExtract.egg-info/dependency_links.txt
+-rw-r--r--   0 zhusitao   (501) staff       (20)      113 2023-07-18 11:54:18.000000 featurExtract-0.2.5.7/featurExtract.egg-info/entry_points.txt
+-rw-r--r--   0 zhusitao   (501) staff       (20)       80 2023-07-18 11:54:18.000000 featurExtract-0.2.5.7/featurExtract.egg-info/requires.txt
+-rw-r--r--   0 zhusitao   (501) staff       (20)       14 2023-07-18 11:54:18.000000 featurExtract-0.2.5.7/featurExtract.egg-info/top_level.txt
+-rw-r--r--   0 zhusitao   (501) staff       (20)       38 2023-07-18 11:54:18.000000 featurExtract-0.2.5.7/setup.cfg
+-rw-r--r--   0 zhusitao   (501) staff       (20)     1283 2021-08-20 10:06:18.000000 featurExtract-0.2.5.7/setup.py
```

### Comparing `featurExtract-0.2.5.6/PKG-INFO` & `featurExtract-0.2.5.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurExtract
-Version: 0.2.5.6
+Version: 0.2.5.7
 Summary: Extract genome ferature sequence for biologists
 Home-page: https://github.com/SitaoZ/featurExtract.git
 Author: zhusitao
 Author-email: zhusitao1990@163.com
 License: MIT
 Keywords: genome feature,extract
 Platform: UNKNOWN
```

### Comparing `featurExtract-0.2.5.6/README.md` & `featurExtract-0.2.5.7/README.md`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.6/featurExtract/b.py` & `featurExtract-0.2.5.7/featurExtract/b.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.6/featurExtract/command_gb.py` & `featurExtract-0.2.5.7/featurExtract/command_gb.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.6/featurExtract/command_gff.py` & `featurExtract-0.2.5.7/featurExtract/command_gff.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,34 +13,34 @@
     print("\033[1;33;40mVersion: \033[0m\033[1;32;40m %s\033[0m"%(__version__))
     print("\033[1;33;40mContact: \033[0m\033[1;32;40m Sitao Zhu <zhusitao1990@163.com>\033[0m")
     print("\033[1;33;40mUsage  : \033[0m\033[1;35;40m featurExtract\033[0m \033[1;31;40m<command> [parameters] \033[0m")
     print("\033[1;33;40mCommand: \033[0m")
     sub_usage(["create    ", "create database for GTF or GFF"])
     sub_usage(["coverage  ", "read coverage by transcript models"])
     sub_usage(["CDS       ", "extract CDS for gene or genome"])
-    sub_usage(["cdna      ", "extract cdna (refMrna) sequence fo gene or genome"])
     sub_usage(["dORF      ", "extract downstream (dORF) for gene or genome"])
     sub_usage(["exon      ", "extract exon for transcript"])
     sub_usage(["gene      ", "extract gene sequence fo gene or genome"])
     sub_usage(["intron    ", "extract intron for transcript"])
     sub_usage(["IGR       ", "extract intergenic region (IGR) between genes"])
     sub_usage(["mRNA      ", "extract mature messager RNA for transcript"])
     sub_usage(["promoter  ", "extract promoter for gene or genome"])
     sub_usage(["terminator", "extract terminator for gene or genome"])
+    sub_usage(["transcript", "extract transcript (refMrna) sequence fo gene or genome"])
     sub_usage(["uORF      ", "extract upstream ORF (uORF) for gene or genome"])
     sub_usage(["UTR       ", "extract untranslated region (UTR) for gene or genome"])
     
     sys.exit(1)
 
 
 def main():
     if len(sys.argv) == 1:
         main_usage()
     elif len(sys.argv) >= 2:
-        if sys.argv[1] in ['create','gene','mRNA','cdna','IGR','promoter','terminator','UTR','uORF','CDS','dORF','exon','intron']:
+        if sys.argv[1] in ['create','gene','mRNA','transcript','IGR','promoter','terminator','UTR','uORF','CDS','dORF','exon','intron']:
             # import 就执行feature_extract()
             # 安装后，系统存在featurExtract包
             from featurExtract import feature_extract
             #import feature_extract
         else:
             main_usage()
```

### Comparing `featurExtract-0.2.5.6/featurExtract/commands/extract_CDS.py` & `featurExtract-0.2.5.7/featurExtract/commands/extract_mRNA.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,178 +1,168 @@
 # -*- coding: utf-8 -*-
-import os
 import sys
 import gffutils
 import pandas as pd 
-from tqdm import tqdm
+from tqdm import tqdm 
 from Bio import SeqIO
 from Bio.Seq import Seq
+from collections import deque
 from Bio.SeqRecord import SeqRecord
-from collections import defaultdict, deque
+from collections import defaultdict
 from featurExtract.database.database import create_db
-from featurExtract.utils.util import add_stop_codon,mRNA_type
+from featurExtract.utils.util import utr3_type, utr5_type, mRNA_type
+from featurExtract.utils.util import stop_codon_seq, add_stop_codon
 
 '''
 https://www.ncbi.nlm.nih.gov/genbank/genomes_gff/
 '''
-def stop_codon(db, transcript, genome):
-    s = ''
-    for codon in db.children(transcript, featuretype='stop_codon', order_by='start'):
-        s = codon.sequence(genome, use_strand=False) # 不反向互补,序列全部连接后再互补
-    return s
 
+_CSV_HEADER = ['TranscriptID','Chrom','Start','End','Strand','mRNA']
 
-_CSV_HEADER = ['TranscriptID','Chrom','Start','End','Strand','CDS']
+def plus_strand():
+    pass
 
-def get_cds(args):
+def minus_strand():
+    pass
+
+
+def get_mRNA(args):
     '''
     parameters:
         args: parse from argparse
     return:
         elements write to a file or stdout
     '''
-    # print(args)
     db = gffutils.FeatureDB(args.database, keep_order=True) # load database
-    feature_types = db.featuretypes()
-    # dict
-    cds_seq_list = deque()
-    # cds_seq = pd.DataFrame(columns=['TranscriptID','Chrom','Start','End','Strand','CDS'])
-    cds_record = deque()
+    # mrna_seq = pd.DataFrame(columns=_CSV_HEADER)
+    mrna_seq_list = deque()
+    mrna_record = []
     index = 0
     # assert GTF or GFF
-    if args.rna_feature == 'mRNA':
-        mRNA_str = mRNA_type(args.style)
-    else:
-        mRNA_str = tuple(x for x in list(feature_types) if 'RNA' in x or 'transcript' in x)
-    # loop all transcript in genome
+    mRNA_str = mRNA_type(args.style)
+    utr3_t = utr3_type(args.style)
+    utr5_t = utr5_type(args.style)
+    
     if not args.transcript:
+        # loop all transcript 
         for t in tqdm(db.features_of_type(mRNA_str, order_by='start'), \
-                                   total = len(list(db.features_of_type(mRNA_str, order_by='start'))),\
-                                   ncols = 80, desc="CDS Processing :"):
-            seq = ''
-            cds_start_transcript = 0
-            cds_end_transcript = 0
+                      total = len(list(db.features_of_type(mRNA_str, order_by='start'))), \
+                      ncols = 80, desc = "mRNA Processing:"):
+            utr5, cds , utr3 = '', '', ''
+            for u in db.children(t, featuretype=utr5_t, order_by='start'):
+                utr5 += u.sequence(args.genome, use_strand=False)
+            for u in db.children(t, featuretype=utr3_t, order_by='start'):
+                utr3 += u.sequence(args.genome, use_strand=False)
             for c in db.children(t, featuretype='CDS', order_by='start'):
-                # 不反向互补，对于负链要得到全部的cds后再一次性反向>互补
-                s = c.sequence(args.genome, use_strand=False)
-                seq += s
-                if not cds_start_transcript :
-                    cds_start_transcript = c.start - t.start
-                cds_end_transcript += len(s)
-            cds_end_transcript = cds_end_transcript + cds_start_transcript
-            
+                # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
+                cds += c.sequence(args.genome, use_strand=False)
             if args.style == 'GTF':
-                stop_codon_seq = stop_codon(db, t, args.genome)
-                seq = add_stop_codon(seq, t.strand, stop_codon_seq)
+                stop_codon_s = stop_codon_seq(db, t, args.genome)
+                cds = add_stop_codon(cds, t.strand, stop_codon_s)
+            if args.upper:
+                if t.strand == '-':
+                    seq = utr3.lower() + cds.upper() + utr5.lower()
+                else:
+                    seq = utr5.lower() + cds.upper() + utr3.lower()
+            else:
+                if t.strand == '-':
+                    seq = utr3 + cds + utr5
+                else:
+                    seq = utr5 + cds + utr3
+            
             seq = Seq(seq)
             if t.strand == '-':
                 seq = seq.reverse_complement()
             # csv output
             if args.output_format == 'csv':
-                # dict 
-                # cds_seq.loc[index] = [t.id,t.chrom,t.start,t.end,t.strand,seq]
+                # mrna_seq.loc[index] = [t.id.replace('transcript:',''),t.chrom,t.start,t.end,t.strand,seq]
                 # index += 1
-                it = [t.id,t.chrom,t.start,t.end,t.strand,seq]
-                cds_seq_list.append(dict((_CSV_HEADER[i], it[i]) for i in range(len(_CSV_HEADER))))
-            # defalut fasta
-            else:
-                desc='strand:%s start:%d end:%d length=%d CDS=%d-%d'%(t.strand,
-                                                                      t.start,
-                                                                      t.end,
-                                                                      len(seq),
-                                                                      cds_start_transcript,
-                                                                      cds_end_transcript)
-                cdsRecord = SeqRecord(seq, id=t.id.replace('transcript:',''), description=desc)
-                cds_record.append(cdsRecord)
-            # break 
-        # csv
+                it = [t.id.replace('transcript:',''),t.chrom,t.start,t.end,t.strand,seq]
+                mrna_seq_list.append(dict((_CSV_HEADER[i], it[i]) for i in range(len(_CSV_HEADER))))
+            # fasta 
+            elif args.output_format == 'fasta':
+                desc='strand:%s start:%d end:%d length=%d CDS=%d-%d'%(t.strand,t.start,t.end,len(seq),
+                                                                      len(utr5)+1 ,
+                                                                      len(utr5) + len(cds))
+                mrnaRecord = SeqRecord(seq, id=t.id.replace('transcript:',''), description=desc)
+                mrna_record.append(mrnaRecord)
         if args.output_format == 'csv':
-            cds_seq = pd.DataFrame.from_dict(cds_seq_list)
-            cds_seq.to_csv(args.output, sep=',', index=False)
-        # default fasta
-        elif args.output_format == 'fasta': 
-            with open(args.output,'w') as handle:
-                SeqIO.write(cds_record, handle, "fasta") 
-        else:
-            sys.exit('output format not be specified')
+            mrna_seq = pd.DataFrame.from_dict(mrna_seq_list)
+            mrna_seq.to_csv(args.output, sep=',', index=False)
+        elif args.output_format == 'fasta':
+            SeqIO.write(mrna_record, args.output, "fasta")
     else:
-        # only one transcript
         for t in db.features_of_type(mRNA_str, order_by='start'):
             if args.transcript in t.id:
-                seq = ''
+                utr5, cds , utr3 = '', '', ''
+                for u in db.children(t, featuretype=utr5_t, order_by='start'):
+                    utr5 += u.sequence(args.genome, use_strand=False)
+                for u in db.children(t, featuretype=utr3_t, order_by='start'):
+                    utr3 += u.sequence(args.genome, use_strand=False)
                 for c in db.children(t, featuretype='CDS', order_by='start'):
-                    # 不反向互补，对于负链要得到全部的cds后再一次性>反向互补
-                    s = c.sequence(args.genome, use_strand=False)
-                    seq += s
+                    # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
+                    cds += c.sequence(args.genome, use_strand=False)
                 if args.style == 'GTF':
-                    stop_codon_seq = stop_codon(db, t, args.genome)
-                    seq = add_stop_codon(seq, t.strand, stop_codon_seq)
+                    stop_codon_s = stop_codon_seq(db, t, args.genome)
+                    cds = add_stop_codon(cds, t.strand, stop_codon_s)
+
+                if args.upper:
+                    if t.strand == '-':
+                        seq = utr3.lower() + cds.upper() + utr5.lower()
+                    else:
+                        seq = utr5.lower() + cds.upper() + utr3.lower()
+                else:
+                    if t.strand == '-':
+                        seq = utr3 + cds + utr5
+                    else:
+                        seq = utr5 + cds + utr3
                 seq = Seq(seq)
                 if t.strand == '-':
                     seq= seq.reverse_complement()
-                # cds_seq.loc[index] = [t.id,t.chrom,t.start,t.end,t.strand,seq]
-                # index += 1
-                desc='strand %s start %d end %d length=%d'%(t.strand,t.start,t.end,len(seq))
-                cdsRecord = SeqRecord(seq, id=t.id, description=desc)
+                desc='strand:%s start:%d end:%d length=%d CDS=%d-%d'%(t.strand,t.start,t.end,len(seq),
+                                                                      len(utr5)+1 ,
+                                                                      len(utr5) + len(cds))
+                mrnaRecord = SeqRecord(seq, id=t.id.replace('transcript:', ''), description=desc)
                 if args.print:
-                    SeqIO.write([cdsRecord], sys.stdout, "fasta") 
+                    SeqIO.write([mrnaRecord], sys.stdout, "fasta") 
                 else:
-                    SeqIO.write([cdsRecord], args.output, "fasta") 
+                    SeqIO.write([mrnaRecord], args.output, "fasta") 
                 break 
 
 
 # GenBank 基因组文件，是每条染色体一个LOCUS
 
-def get_cds_gb(args):
+def get_mRNA_gb(args):
     '''
     '''
-    cds = []
-    proteins = []
+    cdna = []
     for record in create_db(args.genbank):
         for feature in record.features:
-            if feature.type == 'CDS': # CDS promoter UTR 
-                cds_seq = ''
+            if feature.type == 'exon': # CDS promoter UTR 
+                cdna_seq = ''
                 #for part in feature.location.parts:
                 #    cds_seq += part.extract(record.seq)
-                cds_seq = feature.location.extract(record).seq
-                if len(cds_seq)%3 != 0:
-                    continue # reject not triple 
+                cdna_seq = feature.location.extract(record).seq
                 # part.strand 会将FeatureLocation -1的反向互补
                 # geneid or locus_tag 
                 if 'locus_tag' in feature.qualifiers:
                     gene_id = feature.qualifiers['locus_tag'][0]
                 elif 'gene' in feature.qualifiers:
                     gene_id = feature.qualifiers['gene'][0]
                 else:
                     gene_id = "Null"
-                if 'transl_table' in feature.qualifiers:
-                    table_translate = feature.qualifiers['transl_table'][0] 
-                else:
-                    table_translate = 1
-                if str(cds_seq)[:3] in ['AAT','ATA','GTG','TTG','ATT','ACG','TCA','AGG']:
-                    # ATA, GTG and TTG (Yokobori et al. 1999). 
-                    # ATT is the start codon for the CytB gene
-                    # in Halocynthia roretzi (Gissi and Pesole, 2003).
-                    pep = Seq(feature.qualifiers['translation'][0])
-                else:
-                    pep = cds_seq.translate(table=table_translate, cds=True)
-                #pep = cds_seq.translate(to_stop=True)
-                # 判断提取的和已知的是否一致
-                if 'translation' in feature.qualifiers:
-                    assert(str(pep) == feature.qualifiers['translation'][0])
+                # protein id  
                 if 'protein_id' in feature.qualifiers:
-                    protein_id = feature.qualifiers['protein_id'][0] 
+                    protein_id = feature.qualifiers['protein_id'][0]
                 else:
                     protein_id = 'Null'
-                cds_seq_record = SeqRecord(cds_seq,id='gene:%s protein:%s'%(gene_id, protein_id), 
+
+                cdna_seq_record = SeqRecord(cds_seq,id='gene:%s protein:%s'%(gene_id, protein_id),
                                  description='strand %s length %d'%(feature.strand, len(cds_seq)))
-                pep_record = SeqRecord(pep,id='gene:%s protein:%s'%(gene_id, protein_id),
-                             description='strand %s length %d'%(feature.strand, len(pep)))
-                cds.append(cds_seq_record)
-                proteins.append(pep_record)
+                cdna.append(cds_seq_record)
                 break 
         break     
     if args.print and args.format == 'dna':
         SeqIO.write(cds, sys.stdout, 'fasta')
     elif args.print and args.format == 'protein':
         SeqIO.write(proteins, sys.stdout, 'fasta')
     elif args.output and args.format == 'dna':
```

### Comparing `featurExtract-0.2.5.6/featurExtract/commands/extract_IGR.py` & `featurExtract-0.2.5.7/featurExtract/commands/extract_IGR.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.6/featurExtract/commands/extract_cdna.py` & `featurExtract-0.2.5.7/featurExtract/commands/extract_transcript.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 import sys
 import gffutils
 import pandas as pd 
 from tqdm import tqdm 
 from Bio import SeqIO
 from Bio.Seq import Seq
+from multiprocessing import Pool
 from Bio.SeqRecord import SeqRecord
-from collections import defaultdict
+from collections import defaultdict, deque
 from featurExtract.database.database import create_db
-from featurExtract.utils.util import add_stop_codon,mRNA_type,seq_upper_lower
+from featurExtract.utils.util import add_stop_codon, mRNA_type, seq_upper_lower, parse_output
 
 '''
 https://www.ncbi.nlm.nih.gov/genbank/genomes_gff/
 '''
 def stop_codon(db, transcript, genome):
     s = ''
     for codon in db.children(transcript, featuretype='stop_codon', order_by='start'):
@@ -110,176 +111,138 @@
                     stop_codon_e = i.start - 1
                     break 
                 else:
                     print('three_prime_UTR does not exist')
         
         return start_codon_s, stop_codon_e, cds_len
 
-def plus_strand():
-    pass
-
-def minus_strand():
-    pass
 
 _CSV_HEADER = ['TranscriptID', 'Chrom', 'Start_genome', \
                'End_genome','Start_transcript', \
                'End_transcript','Strand','CDS']
 
-def get_cdna(args):
+def sub_transcript(params):
+    """
+    parameters:
+        params: argparse
+    return:
+        transcript_seq_list, a deque
+    """
+    t, database, genome, style, upper, output_format = params
+    db = gffutils.FeatureDB(database, keep_order=True) # load database
+    transcript_seq_list = deque()
+    start_codon_s, stop_codon_e, cds_len = anchor_CDS(db, genome, t, style)
+    atg2firstexon = 0
+    seq = ''
+    for e in db.children(t, featuretype='exon', order_by='start'):
+        # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
+        s = e.sequence(genome, use_strand=False)
+        seq += s
+        if t.strand == '-':
+            if start_codon_s == 0:
+                # five prime_UTR not exist
+                atg2firstexon = 0
+            else:
+                if e.start >= start_codon_s :
+                    atg2firstexon += len(s)
+                elif e.start < start_codon_s < e.end:
+                    truncated = e.end - start_codon_s #  反向减法
+                    atg2firstexon += truncated
+        else:
+            # contain + .
+            if start_codon_s == 0:
+                # five prime_UTR not exist
+                atg2firstexon = 0
+            else:
+                if start_codon_s >= e.end:
+                    atg2firstexon += len(s)
+                elif e.end > start_codon_s > e.start:
+                    truncated = start_codon_s - e.start
+                    atg2firstexon += truncated
+    seq = Seq(seq)
+    if t.strand == '-':
+        seq = seq.reverse_complement()
+    if upper:
+        seq = seq_upper_lower(seq, atg2firstexon, atg2firstexon + cds_len)
+    # position in transcript 1 based 
+    cds_start_transcript = atg2firstexon + 1
+    cds_end_transcript = atg2firstexon + cds_len
+    if output_format == 'fasta':
+        desc='strand:%s start:%d end:%d length=%d CDS=%d-%d'%(t.strand,t.start,t.end,len(seq),
+                                                              cds_start_transcript,
+                                                              cds_end_transcript)
+        transcriptRecord = SeqRecord(seq, id=t.id.replace('transcript:',''), description=desc)
+        transcript_seq_list.append(transcriptRecord)
+    else:
+        it = [t.id.replace('transcript:',''), t.chrom, t.start, t.end,\
+              cds_start_transcript, cds_end_transcript, t.strand, seq]
+        transcript_seq_list.append(dict((_CSV_HEADER[i], it[i]) for i in range(len(_CSV_HEADER))))
+    return transcript_seq_list
+
+    
+def get_transcript(args):
     '''
     parameters:
         args: parse from argparse
     return:
         elements write to a file or stdout
     '''
     db = gffutils.FeatureDB(args.database, keep_order=True) # load database
-    # cdna_seq = pd.DataFrame(columns=_CSV_HEADER)
-    # dict fastest way 
-    cdna_seq_list = []
-    cdna_record = []
-    index = 0
+    feature_types = db.featuretypes()
     # assert GTF or GFF
-    mRNA_str = mRNA_type(args.style)
+    if args.rna_feature == 'mRNA':
+        mRNA_str = mRNA_type(args.style)
+    else:
+        mRNA_str = tuple(x for x in list(feature_types) if 'RNA' in x or 'transcript' in x)
     if not args.transcript:
         # loop all cdns in genome
-        for t in tqdm(db.features_of_type(mRNA_str, order_by='start'), 
-                      total = len(list(db.features_of_type(mRNA_str, order_by='start'))),
-                      ncols = 80, desc = "cDNA Processing :"):
-            #            start_codon, stop_codon = anchor_CDS(db, args.genome, t, args.style)
-            start_codon_s, stop_codon_e, cds_len = anchor_CDS(db, args.genome, t, args.style)
-            atg2firstexon = 0
-            seq = ''
-            for e in db.children(t, featuretype='exon', order_by='start'):
-                # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-                s = e.sequence(args.genome, use_strand=False)
-                seq += s
-                if t.strand == '-':
-                    if start_codon_s == 0:
-                        # five prime_UTR not exist
-                        atg2firstexon = 0
-                    else:
-                        if e.start >= start_codon_s :
-                            atg2firstexon += len(s)
-                        elif e.start < start_codon_s < e.end:
-                            truncated = e.end - start_codon_s #  反向减法
-                            atg2firstexon += truncated
-                else:
-                    # contain + .
-                    if start_codon_s == 0:
-                        # five prime_UTR not exist
-                        atg2firstexon = 0
-                    else:
-                        if start_codon_s >= e.end:
-                            atg2firstexon += len(s)
-                        elif e.end > start_codon_s > e.start:
-                            truncated = start_codon_s - e.start 
-                            atg2firstexon += truncated
-            seq = Seq(seq)
-            if t.strand == '-':
-                seq = seq.reverse_complement()
-            if args.upper:
-                seq = seq_upper_lower(seq,atg2firstexon,atg2firstexon + cds_len)
-            # position in transcript 1 based 
-            cds_start_transcript = atg2firstexon + 1
-            cds_end_transcript = atg2firstexon + cds_len
-            # csv output
-            if args.output_format == 'csv':
-                # cdna_seq.loc[index] = [t.id.replace('transcript:',''),t.chrom,t.start,t.end,
-                #                        cds_start_transcript,cds_end_transcript,t.strand,seq]
-                # index += 1
-                it = [t.id.replace('transcript:',''),t.chrom,t.start,t.end,\
-                      cds_start_transcript,cds_end_transcript,t.strand,seq]
-                cdna_seq_list.append(dict((_CSV_HEADER[i], it[i]) for i in range(len(_CSV_HEADER))))
-            # fasta output
-            elif args.output_format == 'fasta':
-                desc='strand:%s start:%d end:%d length=%d CDS=%d-%d'%(t.strand,t.start,t.end,len(seq),
-                                                                      cds_start_transcript,
-                                                                      cds_end_transcript)
-                cdnaRecord = SeqRecord(seq, id=t.id.replace('transcript:',''), description=desc)
-                cdna_record.append(cdnaRecord)
-        
-        if args.output_format == 'csv':
-            cdna_seq = pd.DataFrame.from_dict(cdna_seq_list)
-            cdna_seq.to_csv(args.output, sep=',', index=False)
-        elif args.output_format == 'fasta':
-            SeqIO.write(cdna_record, args.output, "fasta")
+        param_list = [(t, args.database, args.genome, args.style, args.upper, args.output_format) for t in db.features_of_type(mRNA_str, order_by='start')]
+        with Pool(processes=args.process) as p:
+            transcript_seq_list = list(tqdm(p.imap(sub_transcript, param_list), total=len(param_list), ncols = 80, desc='cDNA Processing:'))
+        transcript_seq_list = [d for de in transcript_seq_list if de != None for d in de]
+        parse_output(args, transcript_seq_list)
     else:
         for t in db.features_of_type(mRNA_str, order_by='start'):
             if args.transcript in t.id:
-                start_codon_s, stop_codon_e, cds_len = anchor_CDS(db, args.genome, t, args.style)
-                atg2firstexon = 0
-                seq = ''
-                for e in db.children(t, featuretype='exon', order_by='start'):
-                    # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-                    s = e.sequence(args.genome, use_strand=False)
-                    seq += s
-                    
-                    if t.strand == '-':
-                        if start_codon_s == 0:
-                            # five prime_UTR not exist
-                            atg2firstexon = 0
-                        else:
-                            if e.start >= start_codon_s :
-                                atg2firstexon += len(s) 
-                            elif e.start < start_codon_s < e.end:
-                                truncated = e.end - start_codon_s  # 反向减法
-                                atg2firstexon += truncated
-                    else:
-                        # contain + .
-                        if start_codon_s >= e.end:
-                            atg2firstexon += len(s)
-                        elif e.end > start_codon_s > e.start:
-                            truncated = start_codon_s - e.start
-                            atg2firstexon += truncated
-                seq = Seq(seq)
-                if t.strand == '-':
-                    seq= seq.reverse_complement()
-                desc='strand:%s start:%d end:%d length=%d CDS=%d-%d'%(t.strand,t.start,t.end,len(seq),
-                                                                      atg2firstexon + 1,
-                                                                      atg2firstexon + cds_len)
-                if args.upper:
-                    seq = seq_upper_lower(seq,atg2firstexon,atg2firstexon + cds_len)
-                cdnaRecord = SeqRecord(seq, id=t.id.replace('transcript:',''), description=desc)
-                if args.print:
-                    SeqIO.write([cdnaRecord], sys.stdout, "fasta") 
-                else:
-                    SeqIO.write([cdnaRecord], args.output, "fasta") 
+                param = (t, args.database, args.genome, args.style, args.upper, args.output_format)
+                transcript_seq_list = sub_transcript(param)
+                parse_output(args, transcript_seq_list)
                 break 
 
 
 # GenBank 基因组文件，是每条染色体一个LOCUS
 
-def get_cdna_gb(args):
+def get_transcript_gb(args):
     '''
     '''
-    cdna = []
+    transcript = []
     for record in create_db(args.genbank):
         for feature in record.features:
             if feature.type == 'exon': # CDS promoter UTR 
-                cdna_seq = ''
+                transcript_seq = ''
                 #for part in feature.location.parts:
                 #    cds_seq += part.extract(record.seq)
-                cdna_seq = feature.location.extract(record).seq
+                transcript_seq = feature.location.extract(record).seq
                 # part.strand 会将FeatureLocation -1的反向互补
                 # geneid or locus_tag 
                 if 'locus_tag' in feature.qualifiers:
                     gene_id = feature.qualifiers['locus_tag'][0]
                 elif 'gene' in feature.qualifiers:
                     gene_id = feature.qualifiers['gene'][0]
                 else:
                     gene_id = "Null"
                 # protein id  
                 if 'protein_id' in feature.qualifiers:
                     protein_id = feature.qualifiers['protein_id'][0]
                 else:
                     protein_id = 'Null'
 
-                cdna_seq_record = SeqRecord(cds_seq,id='gene:%s protein:%s'%(gene_id, protein_id),
+                transcript_seq_record = SeqRecord(cds_seq,id='gene:%s protein:%s'%(gene_id, protein_id),
                                  description='strand %s length %d'%(feature.strand, len(cds_seq)))
-                cdna.append(cds_seq_record)
+                transcript.append(cds_seq_record)
                 break 
         break     
     if args.print and args.format == 'dna':
         SeqIO.write(cds, sys.stdout, 'fasta')
     elif args.print and args.format == 'protein':
         SeqIO.write(proteins, sys.stdout, 'fasta')
     elif args.output and args.format == 'dna':
```

### Comparing `featurExtract-0.2.5.6/featurExtract/commands/extract_dORF.py` & `featurExtract-0.2.5.7/featurExtract/commands/extract_dORF.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 # -*- coding: utf-8 -*-
 import sys
 import gffutils
 import pandas as pd 
 from tqdm import tqdm 
 from Bio.Seq import Seq
+from Bio.SeqRecord import SeqRecord
 from multiprocessing import Pool
 from collections import defaultdict, deque
-from featurExtract.utils.util import utr3_type, utr5_type, mRNA_type
-from featurExtract.utils.util import stop_codon_seq, add_stop_codon 
 from featurExtract.commands.extract_uORF import GFF
+from featurExtract.utils.util import utr3_type, utr5_type, mRNA_type
+from featurExtract.utils.util import stop_codon_seq, add_stop_codon, parse_output
 from featurExtract.utils.visualize import visual_transcript, visual_transcript_genome
 
 # table header 
 _dORF_csv_header = ['TranscriptID', 'Chrom', 'Strand', \
                     'CDS Interval', 'dORF Start', 'dORF End', \
                     'dORF Type', 'dORF Length', 'dORF']
 
@@ -200,20 +201,15 @@
         # print(key,len(dORF_dict[key]))
         for it in dORF_dict[key]:
             # dORF length filter 
             if len(it[8]) <= length:
                 # default: 6
                 continue
             # csv output format 
-            if output_format == 'csv':
-                # dORF_seq.loc[index] = it
-                # dict 
-                dORF_seq_list.append(dict(zip(_dORF_csv_header, it)))
-                index += 1
-            elif output_format == 'fasta':
+            if output_format == 'fasta':
                 uorf_id = ".".join(map(str,[it[0], it[4], it[5], it[6]]))
                 seq = it[8] # it[8] is s Seq type
                 desc='strand:%s dORF=%d-%d %s length=%d CDS=%s-%s'%(it[2],
                                                               it[4],
                                                               it[5],
                                                               it[6],
                                                               len(seq),
@@ -253,43 +249,29 @@
     else:
         mRNA_str = tuple(x for x in list(feature_types) if 'RNA' in x or 'transcript' in x)
     error_count = 0
     total_transcript_number = len(list(db.features_of_type(mRNA_str, order_by='start')))
     # loop all transcripts in genome
     if not args.transcript:
         param_list = [(t, args.database, args.genome, args.style, args.length, args.output_format) for t in db.features_of_type(mRNA_str, order_by='start')]
-        print('length :', len(param_list))
         with Pool(processes=args.process) as p:
-            dORF_seq_list = list(tqdm(p.imap(dorf_filter_output, param_list), total=len(param_list), desc='dORF Processing:'))
+            dORF_seq_list = list(tqdm(p.imap(dorf_filter_output, param_list), total=len(param_list), ncols = 80, desc='dORF Processing:'))
         dORF_seq_list = [d for de in dORF_seq_list if de != None for d in de]
         # output file 
-        if args.output_format == 'csv':
-            dORF_seq = pd.DataFrame.from_dict(dORF_seq_list)
-            dORF_seq.to_csv(args.output, sep=',', index=False)
-        elif args.output_format == 'gff':
-            with open(args.output,'w') as handle:
-                for record in dORF_seq_list:
-                    handle.write(record+'\n')
-        elif args.output_format == 'fasta':
-            with open(args.output,'w') as handle:
-                SeqIO.write(dORF_seq_list, handle, "fasta")
-        else:
-            dORF_seq = pd.DataFrame.from_dict(dORF_seq_list)
-            dORF_seq.to_csv(args.output, sep=',', index=False)
+        parse_output(args, dORF_seq_list)
     else:
         # specify the transcript id; only one transcript
         for t in db.features_of_type(mRNA_str, order_by='start'):
             # primary transcript (pt) 是基因组上的转录本的序列，
             # 有的会包括intron，所以提取的序列和matural transcript 不一致
             # id specify
             if args.transcript in t.id:
                 params = (t, args.database, args.genome, args.style, args.length, args.output_format)
                 dORF_seq_list = dorf_filter_output(params)
                 mt, cds, exons_list, cds_list = get_mt_cds_seq(t, db, args.genome, args.style)
-                print(args)
                 dORF_ = dORF(t.id, args.length, t.chrom, t.strand, mt, cds)
                 dORF_dict = dORF_.dorf_parse()
                 dorf_location_genome = [] # for schematic on genome # 3D list 
                 for key in sorted(dORF_dict.keys()):
                     for it in dORF_dict[key]:
                         # dORF length filter 
                         if len(it[8]) <= args.length:
@@ -316,21 +298,9 @@
                                                       args.transcript,
                                                       exons_list,
                                                       cds_list,
                                                       dorf_location_genome,# 3D list 
                                                       'dORF')
                     figure.draw()
                 # file out
-                if args.output_format == 'csv':
-                    dORF_seq = pd.DataFrame.from_dict(dORF_seq_list)
-                    dORF_seq.to_csv(args.output, sep=',', index=False)
-                elif args.output_format == 'gff':
-                    with open(args.output,'w') as handle:
-                        for record in dORF_seq_list:
-                            handle.write(record+'\n')
-                elif args.output_format == 'fasta':
-                    with open(args.output,'w') as handle:
-                        SeqIO.write(dORF_seq_list, handle, "fasta")
-                else:
-                    dORF_seq = pd.DataFrame.from_dict(dORF_seq_list)
-                    dORF_seq.to_csv(args.output, sep=',', index=False)
+                parse_output(args, dORF_seq_list)
                 break
```

### Comparing `featurExtract-0.2.5.6/featurExtract/commands/extract_exon.py` & `featurExtract-0.2.5.7/featurExtract/commands/extract_exon.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,83 @@
 # -*- coding: utf-8 -*-
 import sys
 import gffutils
 import pandas as pd 
 from tqdm import tqdm 
 from Bio import SeqIO
 from Bio.Seq import Seq
+from multiprocessing import Pool
 from Bio.SeqRecord import SeqRecord
-from collections import defaultdict
-from featurExtract.utils.util import mRNA_type
+from collections import defaultdict, deque
+from featurExtract.utils.util import mRNA_type, parse_output
 from featurExtract.database.database import create_db
 
-_CSV_HEADER = ['TranscriptID','Chrom','Start','End','Strand','Exon']
+_CSV_HEADER = ['TranscriptID','Chrom','Start','End','Strand','Exon', 'Exon_length', 'Exon_index']
+
+def sub_exon(params):
+    """
+    parameters:
+        params:
+    return:
+        exon_seq_list, a deque class 
+    """
+    t, database, genome, output_format = params
+    db = gffutils.FeatureDB(database, keep_order=True)
+    exon_seq_list = deque()
+    exon_index = 0
+    for e in db.children(t, featuretype='exon', order_by='start'):
+        if output_format == 'gff':
+            exon_seq_list.append(e)
+            continue
+        exon = e.sequence(genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
+        exon = Seq(exon)
+        if t.strand == '-':
+            exon = exon.reverse_complement()
+        exon_index += 1
+        # fasta
+        if output_format == 'fasta':
+            exonRecord = SeqRecord(exon,id=t.id,
+                                description='strand %s exon %d start %d end %d length=%d'%(t.strand,
+                                exon_index, e.start, e.end, len(exon)))
+            exon_seq_list.append(exonRecord)
+    
+        else:
+            it = [t.id.replace('transcript:',''), t.chrom, e.start, e.end, t.strand,\
+                  exon, len(exon), exon_index]
+            exon_seq_list.append(dict(zip(_CSV_HEADER, it)))
+    return exon_seq_list    
+
+
 
 def get_exon(args):
     '''
     parameters:
      
     '''
     db = gffutils.FeatureDB(args.database, keep_order=True) # load database
-    # exon_seq = pd.DataFrame(columns=['TranscriptID','Chrom','Start','End','Strand','Exon']) # header
-    exon_seq_list = []
-    mRNA_str = mRNA_type(args.style)
+    feature_types = db.featuretypes()
+    if args.rna_feature == 'mRNA':
+        mRNA_str = mRNA_type(args.style)
+    else:
+        mRNA_str = tuple(x for x in list(feature_types) if 'RNA' in x or 'transcript' in x)
     if args.transcript:
-        # return a specific transcript
-        out = [] 
-        for t in tqdm(db.features_of_type(mRNA_str, order_by='start'), \
-                      total = len(list(db.features_of_type(mRNA_str, order_by='start'))), \
-                      ncols = 80, desc = "Exon Processing:"):
+        for t in db.features_of_type(mRNA_str, order_by='start'):
             if args.transcript in t.id:
-                # exon
-                exon_index = 1
-                for e in db.children(t, featuretype='exon', order_by='start'):
-                    exon = e.sequence(args.genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-                    exon = Seq(exon)
-                    if t.strand == '-':
-                        exon = exon.reverse_complement()
-                    exonRecord = SeqRecord(exon,id=args.transcript, 
-                                 description='strand %s exon %d start %d end %d length=%d'%(t.strand, 
-                                             exon_index, e.start, e.end, len(exon)))
-                    out.append(exonRecord)
-                    exon_index += 1
+                param = (t, args.database, args.genome, args.output_format)
+                exon_seq_list = sub_exon(param)
+                parse_output(args, exon_seq_list)
                 break 
-        if not args.print:
-            SeqIO.write(out, args.output, "fasta")
-        elif args.output:
-            SeqIO.write(out, args.output, "fasta")
-        else:
-            SeqIO.write(out, sys.stdout, "fasta")
     else:
-        whole_exons = []
-        for t in tqdm(db.features_of_type(mRNA_str, order_by='start'), \
-                      total = len(list(db.features_of_type(mRNA_str, order_by='start'))), \
-                      ncols = 80, desc = "Exon Processing:"):
-            exon_index = 1
-            for e in db.children(t, featuretype='exon', order_by='start'):
-                exon = e.sequence(args.genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-                exon = Seq(exon)
-                if t.strand == '-':
-                    exon = exon.reverse_complement()
-                exonRecord = SeqRecord(exon,id=t.id,
-                             description='strand %s exon %d start %d end %d length=%d'%(t.strand,
-                                        exon_index, e.start, e.end, len(exon)))
-                whole_exons.append(exonRecord)
-                exon_index += 1
-        if not args.print:
-            SeqIO.write(whole_exons, args.output, "fasta")
-        elif args.output:
-            SeqIO.write(whole_exons, args.output, "fasta")
-        else:
-            SeqIO.write(whole_exons, sys.stdout, "fasta")
-        
+        param_list = [(t, args.database, args.genome, args.output_format) for t in db.features_of_type(mRNA_str, order_by='start')]
+        param_list = param_list[:10]
+        with Pool(processes=args.process) as p:
+            exon_seq_list = list(tqdm(p.imap(sub_exon, param_list), total=len(param_list), ncols = 80, desc='Exon Processing:'))
+        exon_seq_list = [d for de in exon_seq_list if de != None for d in de]
+        # output
+        parse_output(args, exon_seq_list)
 
 def get_exon_gb(args):
     exons = []
     for record in create_db(args.genbank):
         index = 1
         print(type(record))
         for feature in record.features:
```

### Comparing `featurExtract-0.2.5.6/featurExtract/commands/extract_gene.py` & `featurExtract-0.2.5.7/featurExtract/commands/extract_gene.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.6/featurExtract/commands/extract_intron.py` & `featurExtract-0.2.5.7/featurExtract/commands/extract_intron.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.6/featurExtract/commands/extract_mRNA.py` & `featurExtract-0.2.5.7/featurExtract/commands/extract_CDS.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,168 +1,158 @@
 # -*- coding: utf-8 -*-
+import os
 import sys
 import gffutils
 import pandas as pd 
-from tqdm import tqdm 
+from tqdm import tqdm
 from Bio import SeqIO
 from Bio.Seq import Seq
-from collections import deque
+from io import StringIO
+from multiprocessing import Pool
 from Bio.SeqRecord import SeqRecord
-from collections import defaultdict
+from collections import defaultdict, deque
 from featurExtract.database.database import create_db
-from featurExtract.utils.util import utr3_type, utr5_type, mRNA_type
-from featurExtract.utils.util import stop_codon_seq, add_stop_codon
+from featurExtract.utils.util import add_stop_codon, mRNA_type, parse_output
 
 '''
 https://www.ncbi.nlm.nih.gov/genbank/genomes_gff/
 '''
+def stop_codon(db, transcript, genome):
+    s = ''
+    for codon in db.children(transcript, featuretype='stop_codon', order_by='start'):
+        s = codon.sequence(genome, use_strand=False) # 不反向互补,序列全部连接后再互补
+    return s
+
+
+_CSV_HEADER = ['TranscriptID','Chrom','Start','End','Strand','CDS']
+
+def sub_cds(params):
+    t, database, genome, style, output_format = params
+    db = gffutils.FeatureDB(database, keep_order=True)
+    cds_seq_list = deque()
+    seq = ''
+    cds_start_transcript = 0
+    cds_end_transcript = 0
+    cds_gff_lines = deque()
+    for c in db.children(t, featuretype='CDS', order_by='start'):
+        cds_gff_lines.append(c)
+        # 不反向互补，对于负链要得到全部的cds后再一次性反向>互补
+        s = c.sequence(genome, use_strand=False)
+        seq += s
+        if not cds_start_transcript :
+            cds_start_transcript = c.start - t.start
+        cds_end_transcript += len(s)
+    cds_end_transcript = cds_end_transcript + cds_start_transcript
+    
+    if style == 'GTF':
+        stop_codon_seq = stop_codon(db, t, genome)
+        seq = add_stop_codon(seq, t.strand, stop_codon_seq)
+    seq = Seq(seq)
+    if t.strand == '-':
+        seq = seq.reverse_complement()
+    # csv output
+    if output_format == 'gff':
+        for line in cds_gff_lines:
+            cds_seq_list.append(line)
+    # defalut fasta
+    elif output_format == 'fasta':
+        desc='strand:%s start:%d end:%d length=%d CDS=%d-%d'%(t.strand,
+                                                              t.start,
+                                                              t.end,
+                                                              len(seq),
+                                                              cds_start_transcript,
+                                                              cds_end_transcript)
+        cdsRecord = SeqRecord(seq, id=t.id.replace('transcript:',''), description=desc)
+        cds_seq_list.append(cdsRecord)
+    else:
+        it = [t.id,t.chrom,t.start,t.end,t.strand,seq]
+        cds_seq_list.append(dict((_CSV_HEADER[i], it[i]) for i in range(len(_CSV_HEADER))))
+    return cds_seq_list
 
-_CSV_HEADER = ['TranscriptID','Chrom','Start','End','Strand','mRNA']
-
-def plus_strand():
-    pass
-
-def minus_strand():
-    pass
-
-
-def get_mRNA(args):
+def get_cds(args):
     '''
     parameters:
         args: parse from argparse
     return:
         elements write to a file or stdout
     '''
+    # print(args)
     db = gffutils.FeatureDB(args.database, keep_order=True) # load database
-    # mrna_seq = pd.DataFrame(columns=_CSV_HEADER)
-    mrna_seq_list = deque()
-    mrna_record = []
-    index = 0
+    feature_types = db.featuretypes()
     # assert GTF or GFF
-    mRNA_str = mRNA_type(args.style)
-    utr3_t = utr3_type(args.style)
-    utr5_t = utr5_type(args.style)
-    
+    if args.rna_feature == 'mRNA':
+        mRNA_str = mRNA_type(args.style)
+    else:
+        mRNA_str = tuple(x for x in list(feature_types) if 'RNA' in x or 'transcript' in x)
+    # loop all transcript in genome
     if not args.transcript:
-        # loop all transcript 
-        for t in tqdm(db.features_of_type(mRNA_str, order_by='start'), \
-                      total = len(list(db.features_of_type(mRNA_str, order_by='start'))), \
-                      ncols = 80, desc = "mRNA Processing:"):
-            utr5, cds , utr3 = '', '', ''
-            for u in db.children(t, featuretype=utr5_t, order_by='start'):
-                utr5 += u.sequence(args.genome, use_strand=False)
-            for u in db.children(t, featuretype=utr3_t, order_by='start'):
-                utr3 += u.sequence(args.genome, use_strand=False)
-            for c in db.children(t, featuretype='CDS', order_by='start'):
-                # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-                cds += c.sequence(args.genome, use_strand=False)
-            if args.style == 'GTF':
-                stop_codon_s = stop_codon_seq(db, t, args.genome)
-                cds = add_stop_codon(cds, t.strand, stop_codon_s)
-            if args.upper:
-                if t.strand == '-':
-                    seq = utr3.lower() + cds.upper() + utr5.lower()
-                else:
-                    seq = utr5.lower() + cds.upper() + utr3.lower()
-            else:
-                if t.strand == '-':
-                    seq = utr3 + cds + utr5
-                else:
-                    seq = utr5 + cds + utr3
-            
-            seq = Seq(seq)
-            if t.strand == '-':
-                seq = seq.reverse_complement()
-            # csv output
-            if args.output_format == 'csv':
-                # mrna_seq.loc[index] = [t.id.replace('transcript:',''),t.chrom,t.start,t.end,t.strand,seq]
-                # index += 1
-                it = [t.id.replace('transcript:',''),t.chrom,t.start,t.end,t.strand,seq]
-                mrna_seq_list.append(dict((_CSV_HEADER[i], it[i]) for i in range(len(_CSV_HEADER))))
-            # fasta 
-            elif args.output_format == 'fasta':
-                desc='strand:%s start:%d end:%d length=%d CDS=%d-%d'%(t.strand,t.start,t.end,len(seq),
-                                                                      len(utr5)+1 ,
-                                                                      len(utr5) + len(cds))
-                mrnaRecord = SeqRecord(seq, id=t.id.replace('transcript:',''), description=desc)
-                mrna_record.append(mrnaRecord)
-        if args.output_format == 'csv':
-            mrna_seq = pd.DataFrame.from_dict(mrna_seq_list)
-            mrna_seq.to_csv(args.output, sep=',', index=False)
-        elif args.output_format == 'fasta':
-            SeqIO.write(mrna_record, args.output, "fasta")
+        param_list = [(t, args.database, args.genome, args.style, args.output_format) for t in db.features_of_type(mRNA_str, order_by='start')]
+        with Pool(processes=args.process) as p:
+            cds_seq_list = list(tqdm(p.imap(sub_cds, param_list), total=len(param_list), ncols = 80, desc='CDS Processing:'))
+        cds_seq_list = [d for de in cds_seq_list if de != None for d in de]
+        parse_output(args, cds_seq_list)
     else:
+        # only one transcript
         for t in db.features_of_type(mRNA_str, order_by='start'):
             if args.transcript in t.id:
-                utr5, cds , utr3 = '', '', ''
-                for u in db.children(t, featuretype=utr5_t, order_by='start'):
-                    utr5 += u.sequence(args.genome, use_strand=False)
-                for u in db.children(t, featuretype=utr3_t, order_by='start'):
-                    utr3 += u.sequence(args.genome, use_strand=False)
-                for c in db.children(t, featuretype='CDS', order_by='start'):
-                    # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-                    cds += c.sequence(args.genome, use_strand=False)
-                if args.style == 'GTF':
-                    stop_codon_s = stop_codon_seq(db, t, args.genome)
-                    cds = add_stop_codon(cds, t.strand, stop_codon_s)
-
-                if args.upper:
-                    if t.strand == '-':
-                        seq = utr3.lower() + cds.upper() + utr5.lower()
-                    else:
-                        seq = utr5.lower() + cds.upper() + utr3.lower()
-                else:
-                    if t.strand == '-':
-                        seq = utr3 + cds + utr5
-                    else:
-                        seq = utr5 + cds + utr3
-                seq = Seq(seq)
-                if t.strand == '-':
-                    seq= seq.reverse_complement()
-                desc='strand:%s start:%d end:%d length=%d CDS=%d-%d'%(t.strand,t.start,t.end,len(seq),
-                                                                      len(utr5)+1 ,
-                                                                      len(utr5) + len(cds))
-                mrnaRecord = SeqRecord(seq, id=t.id.replace('transcript:', ''), description=desc)
-                if args.print:
-                    SeqIO.write([mrnaRecord], sys.stdout, "fasta") 
-                else:
-                    SeqIO.write([mrnaRecord], args.output, "fasta") 
+                param = (t, args.database, args.genome, args.style, args.output_format)
+                cds_seq_list = sub_cds(param) 
+                parse_output(args, cds_seq_list)
                 break 
 
 
 # GenBank 基因组文件，是每条染色体一个LOCUS
 
-def get_mRNA_gb(args):
+def get_cds_gb(args):
     '''
     '''
-    cdna = []
+    cds = []
+    proteins = []
     for record in create_db(args.genbank):
         for feature in record.features:
-            if feature.type == 'exon': # CDS promoter UTR 
-                cdna_seq = ''
+            if feature.type == 'CDS': # CDS promoter UTR 
+                cds_seq = ''
                 #for part in feature.location.parts:
                 #    cds_seq += part.extract(record.seq)
-                cdna_seq = feature.location.extract(record).seq
+                cds_seq = feature.location.extract(record).seq
+                if len(cds_seq)%3 != 0:
+                    continue # reject not triple 
                 # part.strand 会将FeatureLocation -1的反向互补
                 # geneid or locus_tag 
                 if 'locus_tag' in feature.qualifiers:
                     gene_id = feature.qualifiers['locus_tag'][0]
                 elif 'gene' in feature.qualifiers:
                     gene_id = feature.qualifiers['gene'][0]
                 else:
                     gene_id = "Null"
-                # protein id  
+                if 'transl_table' in feature.qualifiers:
+                    table_translate = feature.qualifiers['transl_table'][0] 
+                else:
+                    table_translate = 1
+                if str(cds_seq)[:3] in ['AAT','ATA','GTG','TTG','ATT','ACG','TCA','AGG']:
+                    # ATA, GTG and TTG (Yokobori et al. 1999). 
+                    # ATT is the start codon for the CytB gene
+                    # in Halocynthia roretzi (Gissi and Pesole, 2003).
+                    pep = Seq(feature.qualifiers['translation'][0])
+                else:
+                    pep = cds_seq.translate(table=table_translate, cds=True)
+                #pep = cds_seq.translate(to_stop=True)
+                # 判断提取的和已知的是否一致
+                if 'translation' in feature.qualifiers:
+                    assert(str(pep) == feature.qualifiers['translation'][0])
                 if 'protein_id' in feature.qualifiers:
-                    protein_id = feature.qualifiers['protein_id'][0]
+                    protein_id = feature.qualifiers['protein_id'][0] 
                 else:
                     protein_id = 'Null'
-
-                cdna_seq_record = SeqRecord(cds_seq,id='gene:%s protein:%s'%(gene_id, protein_id),
+                cds_seq_record = SeqRecord(cds_seq,id='gene:%s protein:%s'%(gene_id, protein_id), 
                                  description='strand %s length %d'%(feature.strand, len(cds_seq)))
-                cdna.append(cds_seq_record)
+                pep_record = SeqRecord(pep,id='gene:%s protein:%s'%(gene_id, protein_id),
+                             description='strand %s length %d'%(feature.strand, len(pep)))
+                cds.append(cds_seq_record)
+                proteins.append(pep_record)
                 break 
         break     
     if args.print and args.format == 'dna':
         SeqIO.write(cds, sys.stdout, 'fasta')
     elif args.print and args.format == 'protein':
         SeqIO.write(proteins, sys.stdout, 'fasta')
     elif args.output and args.format == 'dna':
```

### Comparing `featurExtract-0.2.5.6/featurExtract/commands/extract_rRNA.py` & `featurExtract-0.2.5.7/featurExtract/commands/extract_rRNA.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.6/featurExtract/commands/extract_tRNA.py` & `featurExtract-0.2.5.7/featurExtract/commands/extract_tRNA.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.6/featurExtract/commands/extract_terminator.py` & `featurExtract-0.2.5.7/featurExtract/commands/extract_terminator.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.6/featurExtract/commands/extract_uORF.py` & `featurExtract-0.2.5.7/featurExtract/commands/extract_uORF_back.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # -*- coding: utf-8 -*-
 import sys
 import gffutils
 import pandas as pd 
-from multiprocessing import Pool
-from multiprocessing import get_context
+import multiprocessing
 from tqdm import tqdm 
 from Bio import SeqIO
 from Bio.Seq import Seq
 from Bio.SeqRecord import SeqRecord
 from collections import defaultdict, deque
-from concurrent.futures import ProcessPoolExecutor
 from featurExtract.utils.util import utr3_type, utr5_type, mRNA_type
 from featurExtract.utils.util import stop_codon_seq, add_stop_codon
 from featurExtract.utils.visualize import visual_transcript, visual_transcript_genome
 
 # table header 
 _uORF_csv_header = ['TranscriptID', 'Chrom', 'Strand', 
                     'CDS Interval', 'uORF Start', 'uORF End', 
@@ -401,17 +399,15 @@
     for e in db.children(t, featuretype='exon', order_by='start'):
         exons_list.append((e.start, e.end))
         mt += e.sequence(genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
     mt = Seq(mt)
     if t.strand == '-':
         mt = mt.reverse_complement()
     # CDS 提取的是编码区 ATG ... TAG
-    cds_list = []
     for c in db.children(t, featuretype='CDS', order_by='start'):
-        cds_list.append((c.start, c.end))
         cds += c.sequence(genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
     if style == 'GTF':
         sc_seq = stop_codon_seq(db, t, genome)
         cds = add_stop_codon(cds, t.strand, sc_seq)
     cds = Seq(cds)
     ## 需要确定exon和mRNA的位置是否一致，不一致以mRNA为准
     # mt from utr5/3 and cds
@@ -422,173 +418,234 @@
     if t.strand == '-':
         mt_from_utr_cds = mt_from_utr_cds.reverse_complement()
     if mt != mt_from_utr_cds:
         mt = mt_from_utr_cds
         # error_count += 1
     if t.strand == '-':
         cds = cds.reverse_complement()
-    return mt, cds, exons_list, cds_list
+    return mt, cds, exons_list
     
-def uorf_filter_output(params):
-    t, database, genome, style, length, output_format = params
-    db = gffutils.FeatureDB(database, keep_order=True)
-    index = 0 
-    uORF_seq_list = deque()
-    # 可以多进程,但是多进程会导致和SQLite数据库的交互产生错误
-    mt, cds, exons_list, cds_list = get_mt_cds_seq(t, db, genome, style)
-    # objected-oriented
-    if mt == cds: # not contain uORF
-        return 
-    if len(cds) % 3 != 0: # CDS error
-        return 
-    uORF_ = uORF(t.id, t.chrom, t.strand, mt, cds)
-    uORF_dict = uORF_.uorf_parse()
-    if len(uORF_dict) == 0: # CDS error
-        return 
-    # loop for type1, type2 and type3
-    for key in sorted(uORF_dict.keys()):
-        # print(key,len(uORF_dict[key]))
-        for it in uORF_dict[key]:
-            # uORF length filter 
-            if len(it[8]) <= length:
-                # default: 6
-                continue
-            # csv output format 
-            if output_format == 'csv':
-                # uORF_seq.loc[index] = it
-                # dict 
-                uORF_seq_list.append(dict(zip(_uORF_csv_header, it)))
-                index += 1
-            elif output_format == 'fasta':
-                uorf_id = ".".join(map(str,[it[0], it[4], it[5], it[6]]))
-                seq = it[8] # it[8] is s Seq type
-                desc='strand:%s uORF=%d-%d %s length=%d CDS=%s-%s'%(it[2],
-                                                              it[4],
-                                                              it[5],
-                                                              it[6],
-                                                              len(seq),
-                                                              it[3].split('-')[0],
-                                                              it[3].split('-')[1])
-                uorfRecord = SeqRecord(seq, id=uorf_id.replace('transcript:',''), description=desc)
-                uORF_seq_list.append(uorfRecord)
-
-            elif output_format == 'gff':
-                gff = GFF(exons_list, it, 'uORF')
-                uorf_gff_line,features_gff_lines = gff.parse()
-                # print(uorf_gff_line)
-                # uORF_gff.write(uorf_gff_line+"\n")
-                uORF_seq_list.append(uorf_gff_line)
-                for feature_line in features_gff_lines:
-                    # print(feature_line)
-                    uORF_seq_list.append(feature_line)
-                    # uORF_gff.write(feature_line+"\n")
-            else:
-                # csv output_format
-                uORF_seq_list.append(dict(zip(_uORF_csv_header, it)))
-                index += 1
-    return uORF_seq_list
-
 
 def get_uorf(args):
     """ Get uORF main command line entry
     parameters:
         args: parse from argparse
     return:
         elements write to a file or stdout
     """
     db = gffutils.FeatureDB(args.database, keep_order=True)
     feature_types = db.featuretypes()
     # csv
     # uORF_seq = pd.DataFrame(columns=_uORF_csv_header)
     # uORF_seq_list = []
-    # uORF_seq_list = deque()
+    uORF_seq_list = deque()
+    # gff
+    uORF_gff = open(args.output,'w')
     # fasta
+    # uorf_record = []
     uorf_record = deque()
-    # gff 
-    uorf_gff_record = deque()
-    # index = 0
+    index = 0
     if args.rna_feature == 'mRNA':
         mRNA_str = mRNA_type(args.style)
     else:
         mRNA_str = tuple(x for x in list(feature_types) if 'RNA' in x or 'transcript' in x)
     error_count = 0
     total_transcript_number = len(list(db.features_of_type(mRNA_str, order_by='start')))
     # loop all transcripts in genome
     if not args.transcript:
-        param_list = [(t, args.database, args.genome, args.style, args.length, args.output_format) for t in db.features_of_type(mRNA_str, order_by='start')]
-        print('length :', len(param_list))
-        with Pool(processes=args.process) as p:
-            uORF_seq_list = list(tqdm(p.imap(uorf_filter_output, param_list), total=len(param_list), desc='多进程提取uORF:'))
-        uORF_seq_list = [d for de in uORF_seq_list if de != None for d in de]
+        for t in tqdm(db.features_of_type(mRNA_str, order_by='start'), \
+                      total = total_transcript_number, \
+                      ncols = 80, desc = "uORF Processing :"):
+            # 可以多进程,但是多进程会导致和SQLite数据库的交互产生错误
+            # mt, cds, exons_list = get_mt_cds_seq(t, db, args.genome, args.style)
+            mt, cds = '', ''
+            exons_list = []
+            for e in db.children(t, featuretype='exon', order_by='start'):
+                exons_list.append((e.start, e.end))
+                mt += e.sequence(args.genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
+            mt = Seq(mt)
+            if t.strand == '-':
+                mt = mt.reverse_complement()
+            # CDS 提取的是编码区 ATG ... TAG
+            for c in db.children(t, featuretype='CDS', order_by='start'):
+                cds += c.sequence(args.genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
+            if args.style == 'GTF':
+                sc_seq = stop_codon_seq(db, t, args.genome)
+                cds = add_stop_codon(cds, t.strand, sc_seq)
+            cds = Seq(cds)
+            ## 需要确定exon和mRNA的位置是否一致，不一致以mRNA为准
+            # mt from utr5/3 and cds
+            mt_from_utr_cds = ''
+            for e in db.children(t, featuretype=['five_prime_UTR', 'CDS', 'three_prime_UTR'], order_by='start'):
+                mt_from_utr_cds += e.sequence(args.genome, use_strand=False)
+            mt_from_utr_cds = Seq(mt_from_utr_cds)
+            if t.strand == '-':
+                mt_from_utr_cds = mt_from_utr_cds.reverse_complement()
+            if mt != mt_from_utr_cds:
+                mt = mt_from_utr_cds
+                # error_count += 1
+            if t.strand == '-':
+                cds = cds.reverse_complement()
+            # procedure-oriented
+            # uORF_dict = uorf_procedure_oriented(t.id, t.chrom, t.strand, mt, cds)
+            # objected-oriented
+            if mt == cds: # not contain uORF
+                continue
+            if len(cds) % 3 != 0: # CDS error
+                continue
+            uORF_ = uORF(t.id, t.chrom, t.strand, mt, cds)
+            uORF_dict = uORF_.uorf_parse()
+            if len(uORF_dict) == 0: # CDS error
+                continue
+            # loop for type1, type2 and type3
+            for key in sorted(uORF_dict.keys()):
+                # print(key,len(uORF_dict[key]))
+                for it in uORF_dict[key]:
+                    # uORF length filter 
+                    if len(it[8]) <= args.length:
+                        # default: 6
+                        continue
+                    # csv output format 
+                    if args.output_format == 'csv':
+                        # uORF_seq.loc[index] = it
+                        # dict 
+                        uORF_seq_list.append(dict(zip(_uORF_csv_header, it)))
+                        index += 1
+                    elif args.output_format == 'fasta':
+                        uorf_id = ".".join(map(str,[it[0], it[4], it[5], it[6]]))
+                        seq = it[8] # it[8] is s Seq type
+                        desc='strand:%s uORF=%d-%d %s length=%d CDS=%s-%s'%(it[2],
+                                                                      it[4],
+                                                                      it[5],
+                                                                      it[6],
+                                                                      len(seq),
+                                                                      it[3].split('-')[0],
+                                                                      it[3].split('-')[1])
+                        uorfRecord = SeqRecord(seq, id=uorf_id.replace('transcript:',''), description=desc)
+                        uorf_record.append(uorfRecord)
+                        
+                    elif args.output_format == 'gff':
+                        gff = GFF(exons_list, it, 'uORF')
+                        uorf_gff_line,features_gff_lines = gff.parse() 
+                        # print(uorf_gff_line)
+                        uORF_gff.write(uorf_gff_line+"\n") 
+                        for feature_line in features_gff_lines:
+                            # print(feature_line)
+                            uORF_gff.write(feature_line+"\n")
+                    else:
+                        # csv output_format
+                        uORF_seq_list.append(dict(zip(_uORF_csv_header, it)))
+                        index += 1 
         # output file 
         if args.output_format == 'csv':
             uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
             uORF_seq.to_csv(args.output, sep=',', index=False)
         elif args.output_format == 'gff':
-            with open(args.output,'w') as handle:
-                for record in uORF_seq_list:
-                    handle.write(record+'\n')
+            uORF_gff.close()
         elif args.output_format == 'fasta':
             with open(args.output,'w') as handle:
-                SeqIO.write(uORF_seq_list, handle, "fasta")
+                SeqIO.write(uorf_record, handle, "fasta")
         else:
             uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
             uORF_seq.to_csv(args.output, sep=',', index=False)
     else:
+        mRNA_str = tuple(x for x in list(feature_types) if 'RNA' in x or 'transcript' in x)
         # specify the transcript id; only one transcript
         for t in db.features_of_type(mRNA_str, order_by='start'):
             # primary transcript (pt) 是基因组上的转录本的序列，
             # 有的会包括intron，所以提取的序列和matural transcript 不一致
             # id specify
             if args.transcript in t.id:
-                params = (t, args.database, args.genome, args.style, args.length, args.output_format)
-                uORF_seq_list = uorf_filter_output(params)
-                mt, cds, exons_list, cds_list = get_mt_cds_seq(t, db, args.genome, args.style)
+                mt, cds, exons_list = get_mt_cds_seq(t, db, args.genome, args.style)
+                # procedure-oriented 
+                # uORF_dict = uorf_procedure_oriented(t.id, t.chrom, t.strand, mt, cds)
+                # objected-oriented
+                if mt == cds:  # not contain uORF
+                    continue
+                if len(cds) % 3 != 0: # CDS error
+                    continue
                 uORF_ = uORF(t.id, t.chrom, t.strand, mt, cds)
-                print(args)
-                # figure the schametic 
                 uORF_dict = uORF_.uorf_parse()
+                if len(uORF_dict) == 0:  # CDS error
+                    continue
                 uorf_location_genome = [] # for schematic on genome # 3D list 
                 for key in sorted(uORF_dict.keys()):
+                    # print(key,len(uORF_dict[key]))
                     for it in uORF_dict[key]:
                         # uORF length filter 
                         if len(it[8]) <= args.length:
                             # default: 6
                             continue
-                        # for schematic on genome
-                        gff = GFF(exons_list, it, 'uORF')
-                        ex_locations = gff.uorf_exons_location()
-                        uorf_location_genome.append(ex_locations)
+                        # csv output format 
+                        if args.output_format == 'csv':
+                            # uORF_seq.loc[index] = it
+                            # dict is fastest way 
+                            uORF_seq_list.append(dict((_uORF_csv_header[i],it[i]) for i in range(len(_uORF_csv_header))))
+                            index += 1
+                            # for schematic on genome
+                            gff = GFF(exons_list, it, 'uORF')
+                            ex_locations = gff.uorf_exons_location()
+                            uorf_location_genome.append(ex_locations)
+                        elif args.output_format == 'fasta':
+                            uorf_id = ".".join(map(str,[it[0], it[4], it[5], it[6]]))
+                            seq = it[8] # it[8] is a Seq type
+                            desc='strand:%s uORF=%d-%d %s length=%d CDS=%s-%s'%(it[2],
+                                                                        it[4],
+                                                                        it[5],
+                                                                        it[6],
+                                                                        len(seq),
+                                                                        it[3].split('-')[0],
+                                                                        it[3].split('-')[1])
+                            uorfRecord = SeqRecord(seq, id=uorf_id.replace('transcript:',''), description=desc)
+                            uorf_record.append(uorfRecord)
+                            # for schematic on genome
+                            gff = GFF(exons_list, it, 'uORF')
+                            ex_locations = gff.uorf_exons_location()
+                            uorf_location_genome.append(ex_locations) 
+                        elif args.output_format == 'gff':
+                            # for schematic on genome
+                            gff = GFF(exons_list, it, 'uORF')
+                            uorf_gff_line,features_gff_lines = gff.parse()
+                            ex_locations = gff.uorf_exons_location()
+                            uorf_location_genome.append(ex_locations) # for schematic on genome
+                            uORF_gff.write(uorf_gff_line+"\n")
+                            for feature_line in features_gff_lines:
+                                uORF_gff.write(feature_line+"\n")
+                        else:
+                            uORF_seq_list.append(dict((_uORF_csv_header[i],it[i]) for i in range(len(_uORF_csv_header))))
+                            index += 1
+                            gff = GFF(exons_list, it, 'uORF')
+                            ex_locations = gff.uorf_exons_location()
+                            uorf_location_genome.append(ex_locations)
+                # figure the schametic 
                 # without intron 
-                if args.schematic_without_intron == True:
+                if args.schematic_without_intron:
                     figure = visual_transcript(args.schematic_without_intron, 
                                                args.transcript, 
                                                uORF_.transcript_location(),
                                                uORF_.cds_location_transcript(),
                                                uORF_.uorf_location_transcript(),
                                                'uORF')
                     figure.draw()
                 # with intron
-                if args.schematic_with_intron == True:
+                if args.schematic_with_intron:
                     figure = visual_transcript_genome(t.strand, 
                                                       args.schematic_with_intron, 
                                                       args.transcript, 
                                                       exons_list, 
                                                       cds_list,
                                                       uorf_location_genome,# 3D list 
                                                       'uORF')
                     figure.draw() 
                 # file out
                 if args.output_format == 'csv':
                     uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
                     uORF_seq.to_csv(args.output, sep=',', index=False)
                 elif args.output_format == 'gff':
-                    with open(args.output,'w') as handle:
-                        for record in uORF_seq_list:
-                            handle.write(record+'\n')
+                    uORF_gff.close()
                 elif args.output_format == 'fasta':
                     with open(args.output,'w') as handle:
-                        SeqIO.write(uORF_seq_list, handle, "fasta")
+                        SeqIO.write(uorf_record, handle, "fasta")
                 else:
                     uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
                     uORF_seq.to_csv(args.output, sep=',', index=False)
                 break
```

### Comparing `featurExtract-0.2.5.6/featurExtract/commands/extract_uORF_back.py` & `featurExtract-0.2.5.7/featurExtract/commands/extract_uORF.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 # -*- coding: utf-8 -*-
 import sys
 import gffutils
 import pandas as pd 
-import multiprocessing
 from tqdm import tqdm 
 from Bio import SeqIO
 from Bio.Seq import Seq
+from multiprocessing import Pool
 from Bio.SeqRecord import SeqRecord
 from collections import defaultdict, deque
+from concurrent.futures import ProcessPoolExecutor
 from featurExtract.utils.util import utr3_type, utr5_type, mRNA_type
-from featurExtract.utils.util import stop_codon_seq, add_stop_codon
+from featurExtract.utils.util import stop_codon_seq, add_stop_codon, parse_output
 from featurExtract.utils.visualize import visual_transcript, visual_transcript_genome
 
 # table header 
 _uORF_csv_header = ['TranscriptID', 'Chrom', 'Strand', 
                     'CDS Interval', 'uORF Start', 'uORF End', 
                     'uORF Type', 'uORF Length', 'uORF']
 
@@ -399,15 +400,17 @@
     for e in db.children(t, featuretype='exon', order_by='start'):
         exons_list.append((e.start, e.end))
         mt += e.sequence(genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
     mt = Seq(mt)
     if t.strand == '-':
         mt = mt.reverse_complement()
     # CDS 提取的是编码区 ATG ... TAG
+    cds_list = []
     for c in db.children(t, featuretype='CDS', order_by='start'):
+        cds_list.append((c.start, c.end))
         cds += c.sequence(genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
     if style == 'GTF':
         sc_seq = stop_codon_seq(db, t, genome)
         cds = add_stop_codon(cds, t.strand, sc_seq)
     cds = Seq(cds)
     ## 需要确定exon和mRNA的位置是否一致，不一致以mRNA为准
     # mt from utr5/3 and cds
@@ -418,234 +421,141 @@
     if t.strand == '-':
         mt_from_utr_cds = mt_from_utr_cds.reverse_complement()
     if mt != mt_from_utr_cds:
         mt = mt_from_utr_cds
         # error_count += 1
     if t.strand == '-':
         cds = cds.reverse_complement()
-    return mt, cds, exons_list
+    return mt, cds, exons_list, cds_list
     
+def uorf_filter_output(params):
+    t, database, genome, style, length, output_format = params
+    db = gffutils.FeatureDB(database, keep_order=True)
+    index = 0 
+    uORF_seq_list = deque()
+    # 可以多进程,但是多进程会导致和SQLite数据库的交互产生错误
+    mt, cds, exons_list, cds_list = get_mt_cds_seq(t, db, genome, style)
+    # objected-oriented
+    if mt == cds: # not contain uORF
+        return 
+    if len(cds) % 3 != 0: # CDS error
+        return 
+    uORF_ = uORF(t.id, t.chrom, t.strand, mt, cds)
+    uORF_dict = uORF_.uorf_parse()
+    if len(uORF_dict) == 0: # CDS error
+        return 
+    # loop for type1, type2 and type3
+    for key in sorted(uORF_dict.keys()):
+        # print(key,len(uORF_dict[key]))
+        for it in uORF_dict[key]:
+            # uORF length filter 
+            if len(it[8]) <= length:
+                # default: 6
+                continue
+            # csv output format 
+            if output_format == 'fasta':
+                uorf_id = ".".join(map(str,[it[0], it[4], it[5], it[6]]))
+                seq = it[8] # it[8] is s Seq type
+                desc='strand:%s uORF=%d-%d %s length=%d CDS=%s-%s'%(it[2],
+                                                              it[4],
+                                                              it[5],
+                                                              it[6],
+                                                              len(seq),
+                                                              it[3].split('-')[0],
+                                                              it[3].split('-')[1])
+                uorfRecord = SeqRecord(seq, id=uorf_id.replace('transcript:',''), description=desc)
+                uORF_seq_list.append(uorfRecord)
+
+            elif output_format == 'gff':
+                gff = GFF(exons_list, it, 'uORF')
+                uorf_gff_line,features_gff_lines = gff.parse()
+                # print(uorf_gff_line)
+                # uORF_gff.write(uorf_gff_line+"\n")
+                uORF_seq_list.append(uorf_gff_line)
+                for feature_line in features_gff_lines:
+                    # print(feature_line)
+                    uORF_seq_list.append(feature_line)
+                    # uORF_gff.write(feature_line+"\n")
+            else:
+                # csv output_format
+                uORF_seq_list.append(dict(zip(_uORF_csv_header, it)))
+                index += 1
+    return uORF_seq_list
 
 def get_uorf(args):
     """ Get uORF main command line entry
     parameters:
         args: parse from argparse
     return:
         elements write to a file or stdout
     """
     db = gffutils.FeatureDB(args.database, keep_order=True)
     feature_types = db.featuretypes()
     # csv
     # uORF_seq = pd.DataFrame(columns=_uORF_csv_header)
     # uORF_seq_list = []
-    uORF_seq_list = deque()
-    # gff
-    uORF_gff = open(args.output,'w')
+    # uORF_seq_list = deque()
     # fasta
-    # uorf_record = []
     uorf_record = deque()
-    index = 0
+    # gff 
+    uorf_gff_record = deque()
+    # index = 0
     if args.rna_feature == 'mRNA':
         mRNA_str = mRNA_type(args.style)
     else:
         mRNA_str = tuple(x for x in list(feature_types) if 'RNA' in x or 'transcript' in x)
     error_count = 0
     total_transcript_number = len(list(db.features_of_type(mRNA_str, order_by='start')))
     # loop all transcripts in genome
     if not args.transcript:
-        for t in tqdm(db.features_of_type(mRNA_str, order_by='start'), \
-                      total = total_transcript_number, \
-                      ncols = 80, desc = "uORF Processing :"):
-            # 可以多进程,但是多进程会导致和SQLite数据库的交互产生错误
-            # mt, cds, exons_list = get_mt_cds_seq(t, db, args.genome, args.style)
-            mt, cds = '', ''
-            exons_list = []
-            for e in db.children(t, featuretype='exon', order_by='start'):
-                exons_list.append((e.start, e.end))
-                mt += e.sequence(args.genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-            mt = Seq(mt)
-            if t.strand == '-':
-                mt = mt.reverse_complement()
-            # CDS 提取的是编码区 ATG ... TAG
-            for c in db.children(t, featuretype='CDS', order_by='start'):
-                cds += c.sequence(args.genome, use_strand=False) # 不反向互补，对于负链要得到全部的cds后再一次性反向互补
-            if args.style == 'GTF':
-                sc_seq = stop_codon_seq(db, t, args.genome)
-                cds = add_stop_codon(cds, t.strand, sc_seq)
-            cds = Seq(cds)
-            ## 需要确定exon和mRNA的位置是否一致，不一致以mRNA为准
-            # mt from utr5/3 and cds
-            mt_from_utr_cds = ''
-            for e in db.children(t, featuretype=['five_prime_UTR', 'CDS', 'three_prime_UTR'], order_by='start'):
-                mt_from_utr_cds += e.sequence(args.genome, use_strand=False)
-            mt_from_utr_cds = Seq(mt_from_utr_cds)
-            if t.strand == '-':
-                mt_from_utr_cds = mt_from_utr_cds.reverse_complement()
-            if mt != mt_from_utr_cds:
-                mt = mt_from_utr_cds
-                # error_count += 1
-            if t.strand == '-':
-                cds = cds.reverse_complement()
-            # procedure-oriented
-            # uORF_dict = uorf_procedure_oriented(t.id, t.chrom, t.strand, mt, cds)
-            # objected-oriented
-            if mt == cds: # not contain uORF
-                continue
-            if len(cds) % 3 != 0: # CDS error
-                continue
-            uORF_ = uORF(t.id, t.chrom, t.strand, mt, cds)
-            uORF_dict = uORF_.uorf_parse()
-            if len(uORF_dict) == 0: # CDS error
-                continue
-            # loop for type1, type2 and type3
-            for key in sorted(uORF_dict.keys()):
-                # print(key,len(uORF_dict[key]))
-                for it in uORF_dict[key]:
-                    # uORF length filter 
-                    if len(it[8]) <= args.length:
-                        # default: 6
-                        continue
-                    # csv output format 
-                    if args.output_format == 'csv':
-                        # uORF_seq.loc[index] = it
-                        # dict 
-                        uORF_seq_list.append(dict(zip(_uORF_csv_header, it)))
-                        index += 1
-                    elif args.output_format == 'fasta':
-                        uorf_id = ".".join(map(str,[it[0], it[4], it[5], it[6]]))
-                        seq = it[8] # it[8] is s Seq type
-                        desc='strand:%s uORF=%d-%d %s length=%d CDS=%s-%s'%(it[2],
-                                                                      it[4],
-                                                                      it[5],
-                                                                      it[6],
-                                                                      len(seq),
-                                                                      it[3].split('-')[0],
-                                                                      it[3].split('-')[1])
-                        uorfRecord = SeqRecord(seq, id=uorf_id.replace('transcript:',''), description=desc)
-                        uorf_record.append(uorfRecord)
-                        
-                    elif args.output_format == 'gff':
-                        gff = GFF(exons_list, it, 'uORF')
-                        uorf_gff_line,features_gff_lines = gff.parse() 
-                        # print(uorf_gff_line)
-                        uORF_gff.write(uorf_gff_line+"\n") 
-                        for feature_line in features_gff_lines:
-                            # print(feature_line)
-                            uORF_gff.write(feature_line+"\n")
-                    else:
-                        # csv output_format
-                        uORF_seq_list.append(dict(zip(_uORF_csv_header, it)))
-                        index += 1 
+        param_list = [(t, args.database, args.genome, args.style, args.length, args.output_format) for t in db.features_of_type(mRNA_str, order_by='start')]
+        with Pool(processes=args.process) as p:
+            uORF_seq_list = list(tqdm(p.imap(uorf_filter_output, param_list), total=len(param_list), ncols = 80, desc='uORF Processing:'))
+        uORF_seq_list = [d for de in uORF_seq_list if de != None for d in de]
         # output file 
-        if args.output_format == 'csv':
-            uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
-            uORF_seq.to_csv(args.output, sep=',', index=False)
-        elif args.output_format == 'gff':
-            uORF_gff.close()
-        elif args.output_format == 'fasta':
-            with open(args.output,'w') as handle:
-                SeqIO.write(uorf_record, handle, "fasta")
-        else:
-            uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
-            uORF_seq.to_csv(args.output, sep=',', index=False)
+        parse_output(args, uORF_seq_list)
     else:
-        mRNA_str = tuple(x for x in list(feature_types) if 'RNA' in x or 'transcript' in x)
         # specify the transcript id; only one transcript
         for t in db.features_of_type(mRNA_str, order_by='start'):
             # primary transcript (pt) 是基因组上的转录本的序列，
             # 有的会包括intron，所以提取的序列和matural transcript 不一致
             # id specify
             if args.transcript in t.id:
-                mt, cds, exons_list = get_mt_cds_seq(t, db, args.genome, args.style)
-                # procedure-oriented 
-                # uORF_dict = uorf_procedure_oriented(t.id, t.chrom, t.strand, mt, cds)
-                # objected-oriented
-                if mt == cds:  # not contain uORF
-                    continue
-                if len(cds) % 3 != 0: # CDS error
-                    continue
+                params = (t, args.database, args.genome, args.style, args.length, args.output_format)
+                uORF_seq_list = uorf_filter_output(params)
+                mt, cds, exons_list, cds_list = get_mt_cds_seq(t, db, args.genome, args.style)
                 uORF_ = uORF(t.id, t.chrom, t.strand, mt, cds)
+                # figure the schametic 
                 uORF_dict = uORF_.uorf_parse()
-                if len(uORF_dict) == 0:  # CDS error
-                    continue
                 uorf_location_genome = [] # for schematic on genome # 3D list 
                 for key in sorted(uORF_dict.keys()):
-                    # print(key,len(uORF_dict[key]))
                     for it in uORF_dict[key]:
                         # uORF length filter 
                         if len(it[8]) <= args.length:
                             # default: 6
                             continue
-                        # csv output format 
-                        if args.output_format == 'csv':
-                            # uORF_seq.loc[index] = it
-                            # dict is fastest way 
-                            uORF_seq_list.append(dict((_uORF_csv_header[i],it[i]) for i in range(len(_uORF_csv_header))))
-                            index += 1
-                            # for schematic on genome
-                            gff = GFF(exons_list, it, 'uORF')
-                            ex_locations = gff.uorf_exons_location()
-                            uorf_location_genome.append(ex_locations)
-                        elif args.output_format == 'fasta':
-                            uorf_id = ".".join(map(str,[it[0], it[4], it[5], it[6]]))
-                            seq = it[8] # it[8] is a Seq type
-                            desc='strand:%s uORF=%d-%d %s length=%d CDS=%s-%s'%(it[2],
-                                                                        it[4],
-                                                                        it[5],
-                                                                        it[6],
-                                                                        len(seq),
-                                                                        it[3].split('-')[0],
-                                                                        it[3].split('-')[1])
-                            uorfRecord = SeqRecord(seq, id=uorf_id.replace('transcript:',''), description=desc)
-                            uorf_record.append(uorfRecord)
-                            # for schematic on genome
-                            gff = GFF(exons_list, it, 'uORF')
-                            ex_locations = gff.uorf_exons_location()
-                            uorf_location_genome.append(ex_locations) 
-                        elif args.output_format == 'gff':
-                            # for schematic on genome
-                            gff = GFF(exons_list, it, 'uORF')
-                            uorf_gff_line,features_gff_lines = gff.parse()
-                            ex_locations = gff.uorf_exons_location()
-                            uorf_location_genome.append(ex_locations) # for schematic on genome
-                            uORF_gff.write(uorf_gff_line+"\n")
-                            for feature_line in features_gff_lines:
-                                uORF_gff.write(feature_line+"\n")
-                        else:
-                            uORF_seq_list.append(dict((_uORF_csv_header[i],it[i]) for i in range(len(_uORF_csv_header))))
-                            index += 1
-                            gff = GFF(exons_list, it, 'uORF')
-                            ex_locations = gff.uorf_exons_location()
-                            uorf_location_genome.append(ex_locations)
-                # figure the schametic 
+                        # for schematic on genome
+                        gff = GFF(exons_list, it, 'uORF')
+                        ex_locations = gff.uorf_exons_location()
+                        uorf_location_genome.append(ex_locations)
                 # without intron 
-                if args.schematic_without_intron:
+                if args.schematic_without_intron == True:
                     figure = visual_transcript(args.schematic_without_intron, 
                                                args.transcript, 
                                                uORF_.transcript_location(),
                                                uORF_.cds_location_transcript(),
                                                uORF_.uorf_location_transcript(),
                                                'uORF')
                     figure.draw()
                 # with intron
-                if args.schematic_with_intron:
+                if args.schematic_with_intron == True:
                     figure = visual_transcript_genome(t.strand, 
                                                       args.schematic_with_intron, 
                                                       args.transcript, 
                                                       exons_list, 
                                                       cds_list,
                                                       uorf_location_genome,# 3D list 
                                                       'uORF')
                     figure.draw() 
                 # file out
-                if args.output_format == 'csv':
-                    uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
-                    uORF_seq.to_csv(args.output, sep=',', index=False)
-                elif args.output_format == 'gff':
-                    uORF_gff.close()
-                elif args.output_format == 'fasta':
-                    with open(args.output,'w') as handle:
-                        SeqIO.write(uorf_record, handle, "fasta")
-                else:
-                    uORF_seq = pd.DataFrame.from_dict(uORF_seq_list)
-                    uORF_seq.to_csv(args.output, sep=',', index=False)
-                break 
+                parse_output(args, uORF_seq_list)
+                break
```

### Comparing `featurExtract-0.2.5.6/featurExtract/database/database.py` & `featurExtract-0.2.5.7/featurExtract/database/database.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 # -*- coding: utf-8 -*-
 import os 
 from Bio import SeqIO
+from pyfaidx import Fasta
 
 def genome_dict(genome_fasta_path):
     '''
     parameters:
      genome_fasta_path: genome reference of organism
     return:
      genome fasta dict
     '''
-    genome = dict()
-    for record in SeqIO.parse(genome_fasta_path, 'fasta'):
-        genome[record.id] = record.seq
+    genome = Fasta(genome_fasta_path)
     return genome
 
 def create_db(genbank_path):
     if not os.path.exists(genbank_path):
         print('args.genbank path not exist; please check.')
         sys.exit(1)
     for record in SeqIO.parse(genbank_path,'gb'):
```

### Comparing `featurExtract-0.2.5.6/featurExtract/feature_extract.py` & `featurExtract-0.2.5.7/featurExtract/feature_extract.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,22 +14,25 @@
 from featurExtract.commands.extract_CDS import get_cds
 from featurExtract.commands.extract_promoter import get_promoter
 from featurExtract.commands.extract_terminator import get_terminator
 from featurExtract.commands.extract_exon import get_exon
 from featurExtract.commands.extract_intron import get_intron
 from featurExtract.commands.extract_gene import get_gene
 from featurExtract.commands.extract_IGR import get_IGR
-from featurExtract.commands.extract_cdna import get_cdna
+from featurExtract.commands.extract_transcript import get_transcript
 from featurExtract.commands.extract_mRNA import get_mRNA
 
 
 def create(args):
     '''
     parameters:
      args: arguments from argparse
+     This is a time- and memory-intense procedure, but it needs to be done only once for a given genome.
+    return:
+     a db object
     '''
     fn = args.genomefeature
     database_id = args.output_prefix +'.'+ args.file_type
     db = gffutils.create_db(fn, dbfn=database_id, force=True, keep_order=True,\
         disable_infer_genes=True, disable_infer_transcripts=True,\
         merge_strategy='merge', sort_attribute_values=True)
     return db
@@ -118,20 +121,20 @@
 def mRNA(args):
     '''
     parameters:
      args: arguments from argparse
     '''
     get_mRNA(args)
 
-def cdna(args):
+def transcript(args):
     '''
     parameters:
      args: arguments from argparse
     '''
-    get_cdna(args)
+    get_transcript(args)
 
 def IGR(args):
     '''
     parameters:
      args: arguments from argparse
     '''
     get_IGR(args)
@@ -148,28 +151,30 @@
                            help='database absolute path')
 parser_create.set_defaults(func=create)
 
 # promoter subcommand
 parser_promoter = subparsers.add_parser('promoter', help='extract promoter in genome or gene')
 parser_promoter.add_argument('-d', '--database', type=str, required=True, 
                              help='database generated by subcommand create')
-parser_promoter.add_argument('-f', '--output_format', type=str, choices=['csv','fasta'],
+parser_promoter.add_argument('-f', '--output_format', type=str, choices=['csv','fasta'], default='csv',
                              help = 'output format')
 parser_promoter.add_argument('-g', '--genome', type=str, required=True,
                              help='genome fasta path')
 parser_promoter.add_argument('-i', '--gene', type=str, 
                              help='specific gene; if not given, return whole genes')
 parser_promoter.add_argument('-l', '--promoter_length', type=int, default=100,
                              help='promoter length before TSS (default: 100)')
 parser_promoter.add_argument('-o', '--output', type=str, 
                              help = 'output file path')
-parser_promoter.add_argument('-p', '--print', action="store_true", 
-                             help = 'output to stdout')
+parser_promoter.add_argument('-p', '--process', type=int, default=4,
+                             help='number of promoter extract process, (default: 4)')
 parser_promoter.add_argument('-u', '--utr5_upper_length', type=int, default=10,
                              help='5\' utr length after TSS (default: 10)')
+parser_promoter.add_argument('-v', '--print', action="store_true",
+                             help = 'output to stdout')
 parser_promoter.set_defaults(func=promoter)
 
 
 # terminator 
 parser_terminator = subparsers.add_parser('terminator', help='extract terminator in genome or gene')
 parser_terminator.add_argument('-d', '--database', type=str, required=True,
                              help='database generated by subcommand create')
@@ -203,15 +208,15 @@
                          help='output to stdout')
 parser_gene.set_defaults(func=gene)
 
 # mRNA subcommand 
 parser_mRNA = subparsers.add_parser('mRNA', help='extract mature messager RNA in genome or gene')
 parser_mRNA.add_argument('-d', '--database', type=str, required=True, 
                          help='database generated by subcommand create')
-parser_mRNA.add_argument('-f', '--output_format', type=str, choices=['csv','fasta'],
+parser_mRNA.add_argument('-f', '--output_format', type=str, choices=['csv','fasta'], default='csv',
                          help = 'output format')
 parser_mRNA.add_argument('-g', '--genome', type=str, required=True, 
                          help='genome fasta')
 parser_mRNA.add_argument('-i', '--transcript', type=str, 
                          help='specific transcript; if not given, return whole transcripts')
 parser_mRNA.add_argument('-o', '--output', type=str, 
                          help = 'output file path')
@@ -220,33 +225,37 @@
 parser_mRNA.add_argument('-s', '--style', choices=['GFF','GTF'],
                          help = 'GTF database or GFF database')
 parser_mRNA.add_argument('-u', '--upper', action="store_true", 
                          help='upper CDS and lower utr')
 parser_mRNA.set_defaults(func=mRNA)
 
 
-# cdna subcommand 
-parser_cdna = subparsers.add_parser('cdna', help='extract cdna (or refMrna) in genome or gene')
-parser_cdna.add_argument('-d', '--database', type=str, required=True, 
+# transcript subcommand 
+parser_transcript = subparsers.add_parser('transcript', help='extract transcript (or refMrna) in genome or gene')
+parser_transcript.add_argument('-d', '--database', type=str, required=True, 
                          help='database generated by subcommand create')
-parser_cdna.add_argument('-f', '--output_format', type=str, choices=['csv','fasta'],
+parser_transcript.add_argument('-f', '--output_format', type=str, choices=['csv','fasta'], default='csv',
                          help = 'output format')
-parser_cdna.add_argument('-g', '--genome', type=str, required=True, 
+parser_transcript.add_argument('-g', '--genome', type=str, required=True, 
                          help='genome fasta')
-parser_cdna.add_argument('-i', '--transcript', type=str, 
+parser_transcript.add_argument('-i', '--transcript', type=str, 
                          help='specific transcript; if not given, return whole transcripts')
-parser_cdna.add_argument('-o', '--output', type=str, 
+parser_transcript.add_argument('-o', '--output', type=str, 
                          help = 'output file path')
-parser_cdna.add_argument('-p', '--print', action="store_true", 
-                         help='output to stdout')
-parser_cdna.add_argument('-s', '--style', choices=['GFF','GTF'],
+parser_transcript.add_argument('-p', '--process', type=int, default=4,
+                         help='number of cDNA extract process, (default: 4)')
+parser_transcript.add_argument('-r', '--rna_feature', choices=['mRNA', 'all'], default='mRNA',
+                         help='The type of RNA used to extract cDNA, (default: mRNA)')
+parser_transcript.add_argument('-s', '--style', choices=['GFF','GTF'],
                          help = 'GTF database or GFF database')
-parser_cdna.add_argument('-u', '--upper', action="store_true", 
+parser_transcript.add_argument('-u', '--upper', action="store_true", 
                          help='upper CDS and lower utr')
-parser_cdna.set_defaults(func=cdna)
+parser_transcript.add_argument('-v', '--print', action="store_true",
+                         help='output to stdout')
+parser_transcript.set_defaults(func=transcript)
 
 
 # IGR subcommand 
 parser_IGR = subparsers.add_parser('IGR', help='extract IGR in genome or gene')
 parser_IGR.add_argument('-d', '--database', type=str, required=True,
                         help='database generated by subcommand create')
 parser_IGR.add_argument('-g', '--genome', type=str, required=True, 
@@ -262,119 +271,135 @@
                        protein genes, while GFF database contain protein genes and nocoding genes')
 parser_IGR.set_defaults(func=IGR)
 
 # UTR subcommand
 parser_utr = subparsers.add_parser('UTR', help='extract untranslated region sequence in genome or gene')
 parser_utr.add_argument('-d', '--database', type=str, required=True, 
                         help='database generated by subcommand create')
+parser_utr.add_argument('-f', '--output_format', choices=['csv','fasta','gff'], default='csv',
+                        help='output format (default: csv)')
 parser_utr.add_argument('-g', '--genome', type=str, required=True,
                         help='genome fasta file')
 parser_utr.add_argument('-i', '--transcript', type=str, 
                         help='specific transcript id; if not given, \
                         whole transcript will return')
 parser_utr.add_argument('-o', '--output', type=str, 
                         help='output file path')
-parser_utr.add_argument('-p', '--print', action="store_true", 
-                        help='output to stdout')
+parser_utr.add_argument('-p', '--process', type=int, default=4,
+                         help='number of UTR extract process, (default: 4)')
 parser_utr.add_argument('-r', '--rna_feature', choices=['mRNA', 'all'], default='mRNA',
                          help='The type of RNA used to extract UTR, (default: mRNA)')
 parser_utr.add_argument('-s', '--style', choices=['GFF','GTF'], 
                         help = 'GTF database or GFF database')
+parser_utr.add_argument('-v', '--print', action="store_true", 
+                        help='output to stdout. -v and -o option are mutually exclusive')
 parser_utr.set_defaults(func=UTR)
 
 # uORF subcommand
 parser_uORF = subparsers.add_parser('uORF', help='extract upper stream open reading sequence in genome or gene')
 parser_uORF.add_argument('-d', '--database', type=str, required=True, 
                          help='database generated by subcommand create')
-parser_uORF.add_argument('-f', '--output_format', choices=['csv','fasta','gff'],
+parser_uORF.add_argument('-f', '--output_format', choices=['csv','fasta','gff'], default='csv',
                         help='output format (default: csv)')
 parser_uORF.add_argument('-g', '--genome', type=str, required=True,
                          help='genome fasta')
 parser_uORF.add_argument('-i', '--transcript', type=str, 
                          help='specific transcript id; if not given, \
                                whole transcript will return')
 parser_uORF.add_argument('-l', '--length', type=int, default=6,
                          help='uORF length, (default: 6)')
 parser_uORF.add_argument('-m', '--schematic_without_intron', action='store_true',
                          help='schematic figure file for uORF, CDS and transcript without intron')
 parser_uORF.add_argument('-n', '--schematic_with_intron', action='store_true',
                          help='schematic figure file for uORF, CDS and transcript with intron')
 parser_uORF.add_argument('-o', '--output', type=str, 
                          help='output file path')
-parser_uORF.add_argument('-p', '--process', type=int, default=1,
-                         help='number of uORF extract process, (default: 1)')
+parser_uORF.add_argument('-p', '--process', type=int, default=4,
+                         help='number of uORF extract process, (default: 4)')
 parser_uORF.add_argument('-r', '--rna_feature', choices=['mRNA', 'all'], default='mRNA',
                          help='The type of RNA used to make uORF identification (default: mRNA)')
 parser_uORF.add_argument('-s', '--style', choices=['GFF','GTF'], 
                          help = 'GTF database or GFF database')
+parser_uORF.add_argument('-v', '--print', action="store_true",
+                        help='output to stdout. -v and -o option are mutually exclusive')
 parser_uORF.set_defaults(func=uORF)
 
 # CDS subcommand
 parser_cds = subparsers.add_parser('CDS', help='extract coding sequence in genome or gene')
 parser_cds.add_argument('-d', '--database', type=str, required=True, 
                         help='database generated by subcommand create')
-parser_cds.add_argument('-f', '--output_format', type=str, choices=['csv','fasta'],
+parser_cds.add_argument('-f', '--output_format', type=str, choices=['csv','fasta','gff'], default='csv',
                          help = 'output format')
 parser_cds.add_argument('-g', '--genome', type=str, required=True,
                         help='genome fasta')
 parser_cds.add_argument('-i', '--transcript', type=str, 
                         help='specific transcript id; if not given, \
                         whole transcript will return')
 parser_cds.add_argument('-o', '--output', type=str, 
                         help='output file path')
-parser_cds.add_argument('-p', '--print', action="store_true", 
-                        help='output to stdout')
+parser_cds.add_argument('-p', '--process', type=int, default=4,
+                        help='number of CDS extract process, (default: 4)')
 parser_cds.add_argument('-r', '--rna_feature', choices=['mRNA', 'all'], default='mRNA',
                          help='The type of RNA used to extract CDS, (default: mRNA)')
 parser_cds.add_argument('-s', '--style', choices=['GFF','GTF'], 
                         help = 'GTF database or GFF database')
+parser_cds.add_argument('-v', '--print', action="store_true",
+                        help='output to stdout. -v and -o option are mutually exclusive')
 parser_cds.set_defaults(func=CDS)
 
 # dORF subcommand 
 parser_dORF = subparsers.add_parser('dORF', help='extract down stream open reading frame sequence in a genome or gene')
 parser_dORF.add_argument('-d', '--database', type=str, required=True,
                          help='database generated by subcommand create')
-parser_dORF.add_argument('-f', '--output_format', choices=['csv','fasta','gff'],
+parser_dORF.add_argument('-f', '--output_format', choices=['csv','fasta','gff'], default='csv',
                         help='output format')
 parser_dORF.add_argument('-g', '--genome', type=str, required=True, 
                          help='genome fasta')
 parser_dORF.add_argument('-i', '--transcript', type=str, 
                          help='specific transcript id; if not given, \
                                whole transcript will return')
 parser_dORF.add_argument('-l', '--length', type=int, default=6,
                          help='dORF length, (default: 6)')
 parser_dORF.add_argument('-m', '--schematic_without_intron', action='store_true',
                          help='schematic figure file for dORF, CDS and transcript without intron')
 parser_dORF.add_argument('-n', '--schematic_with_intron', action='store_true',
                          help='schematic figure file for dORF, CDS and transcript with intron')
 parser_dORF.add_argument('-o', '--output', type=str, 
                          help='output file path')
-parser_dORF.add_argument('-p', '--process', type=int, default=1,
-                         help='number of dORF extract process, (default: 1)')
+parser_dORF.add_argument('-p', '--process', type=int, default=4,
+                         help='number of dORF extract process, (default: 4)')
 parser_dORF.add_argument('-r', '--rna_feature', choices=['mRNA', 'all'], default='mRNA',
                          help='The type of RNA used to make dORF identification (default: mRNA)')
 parser_dORF.add_argument('-s', '--style', choices=['GFF','GTF'], 
                          help = 'GTF database or GFF database')
+parser_dORF.add_argument('-v', '--print', action="store_true",
+                        help='output to stdout. -v and -o option are mutually exclusive')
 parser_dORF.set_defaults(func=dORF)
 
 
 # exon 
 parser_exon = subparsers.add_parser('exon', help='extract exon sequence for a given transcript')
 parser_exon.add_argument('-d', '--database', type=str, required=True, 
                          help='database generated by subcommand create')
+parser_exon.add_argument('-f', '--output_format', choices=['csv','fasta','gff'], default='csv',
+                        help='output format')
 parser_exon.add_argument('-g', '--genome', type=str, required=True, 
                          help='genome fasta')
 parser_exon.add_argument('-i', '--transcript', type=str, 
                          help='specific transcript id; needed')
 parser_exon.add_argument('-o', '--output', type=str, 
                          help='output file path')
-parser_exon.add_argument('-p', '--print', action="store_true", 
-                         help='output to stdout')
+parser_exon.add_argument('-p', '--process', type=int, default=4,
+                         help='number of exon extract process, (default: 4)')
+parser_exon.add_argument('-r', '--rna_feature', choices=['mRNA', 'all'], default='mRNA',
+                         help='The type of RNA used to make exon extraction (default: mRNA)')
 parser_exon.add_argument('-s', '--style', choices=['GFF','GTF'], 
                          help = 'GTF database or GFF database')
+parser_exon.add_argument('-v', '--print', action="store_true", 
+                         help='output to stdout')
 parser_exon.set_defaults(func=exon)
 
 # intron 
 parser_intron = subparsers.add_parser('intron', help='extract exon sequence for a given transcript')
 parser_intron.add_argument('-d', '--database', type=str, required=True, 
                            help='database generated by subcommand create')
 parser_intron.add_argument('-g', '--genome', type=str, required=True,
```

### Comparing `featurExtract-0.2.5.6/featurExtract/genBank_extract.py` & `featurExtract-0.2.5.7/featurExtract/genBank_extract.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.6/featurExtract/parameter.py` & `featurExtract-0.2.5.7/featurExtract/parameter.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.6/featurExtract/utils/visualize.py` & `featurExtract-0.2.5.7/featurExtract/utils/visualize.py`

 * *Files identical despite different names*

### Comparing `featurExtract-0.2.5.6/featurExtract.egg-info/PKG-INFO` & `featurExtract-0.2.5.7/featurExtract.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: featurExtract
-Version: 0.2.5.6
+Version: 0.2.5.7
 Summary: Extract genome ferature sequence for biologists
 Home-page: https://github.com/SitaoZ/featurExtract.git
 Author: zhusitao
 Author-email: zhusitao1990@163.com
 License: MIT
 Keywords: genome feature,extract
 Platform: UNKNOWN
```

### Comparing `featurExtract-0.2.5.6/featurExtract.egg-info/SOURCES.txt` & `featurExtract-0.2.5.7/featurExtract.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -17,24 +17,24 @@
 featurExtract.egg-info/entry_points.txt
 featurExtract.egg-info/requires.txt
 featurExtract.egg-info/top_level.txt
 featurExtract/commands/__init__.py
 featurExtract/commands/extract_CDS.py
 featurExtract/commands/extract_IGR.py
 featurExtract/commands/extract_UTR.py
-featurExtract/commands/extract_cdna.py
 featurExtract/commands/extract_dORF.py
 featurExtract/commands/extract_exon.py
 featurExtract/commands/extract_gene.py
 featurExtract/commands/extract_intron.py
 featurExtract/commands/extract_mRNA.py
 featurExtract/commands/extract_promoter.py
 featurExtract/commands/extract_rRNA.py
 featurExtract/commands/extract_tRNA.py
 featurExtract/commands/extract_terminator.py
+featurExtract/commands/extract_transcript.py
 featurExtract/commands/extract_uORF.py
 featurExtract/commands/extract_uORF_back.py
 featurExtract/database/database.py
 featurExtract/utils/__init__.py
 featurExtract/utils/coverage.py
 featurExtract/utils/util.py
 featurExtract/utils/visualize.py
```

### Comparing `featurExtract-0.2.5.6/setup.py` & `featurExtract-0.2.5.7/setup.py`

 * *Files identical despite different names*

