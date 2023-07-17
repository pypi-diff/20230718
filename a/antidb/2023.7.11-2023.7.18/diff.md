# Comparing `tmp/antidb-2023.7.11.tar.gz` & `tmp/antidb-2023.7.18.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antidb-2023.7.11.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "antidb-2023.7.18.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `antidb-2023.7.11.tar` & `antidb-2023.7.18.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     8684 2023-07-10 17:52:40.419180 antidb-2023.7.11/README.md
--rw-r--r--   0        0        0     1066 2023-07-11 13:08:42.098621 antidb-2023.7.11/pyproject.toml
--rw-r--r--   0        0        0       22 2023-07-11 14:44:13.949302 antidb-2023.7.11/src/antidb/__init__.py
--rw-r--r--   0        0        0     9935 2023-07-11 11:48:19.703877 antidb-2023.7.11/src/antidb/antidb.py
--rw-r--r--   0        0        0     9550 1970-01-01 00:00:00.000000 antidb-2023.7.11/PKG-INFO
+-rw-r--r--   0        0        0     8780 2023-07-17 11:00:37.457990 antidb-2023.7.18/README.md
+-rw-r--r--   0        0        0     1066 2023-07-17 22:27:00.925968 antidb-2023.7.18/pyproject.toml
+-rw-r--r--   0        0        0       22 2023-07-15 21:58:28.636940 antidb-2023.7.18/src/antidb/__init__.py
+-rw-r--r--   0        0        0    10166 2023-07-17 21:55:16.895534 antidb-2023.7.18/src/antidb/antidb.py
+-rw-r--r--   0        0        0     9646 1970-01-01 00:00:00.000000 antidb-2023.7.18/PKG-INFO
```

### Comparing `antidb-2023.7.11/README.md` & `antidb-2023.7.18/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 # antidb
 ## Quick start
 ```
+pip3 install antidb
+```
+```
 from antidb import (Idx,
                     Prs,
                     count_exec_time)
 
 dbsnp_vcf_path = '/mnt/Storage/databases/dbSNP_platon/GCF_000001405.40.vcf'
 dbsnp_idx_prefix = 'all_rsids'
 
@@ -121,21 +124,23 @@
                     empty_res = True
                     ann_file_line = ann_file_line.rstrip()
                     ann_rsid = ann_file_line.split('\t')[args.rsids_col_num - 1]
                     for dbsnp_zst_line in dbsnp_prs.prs(ann_rsid):
                         empty_res = False
                         trg_file_opened.write(ann_file_line +
                                               dbsnp_zst_line)
+                        break
                     if empty_res:
                         for rsmerged_zst_line in rsmerged_prs.prs(ann_rsid):
                             ann_rsid_syns = parse_rsmerged_line.__wrapped__(rsmerged_zst_line)
                             for dbsnp_zst_line in dbsnp_prs.prs(ann_rsid_syns):
                                 empty_res = False
                                 trg_file_opened.write(ann_file_line +
                                                       dbsnp_zst_line)
+                                break
                             if not empty_res:
                                 break
                         else:
                             dump_file_opened.write(ann_file_line + '\n')
 
 
 res_files_crt_time = datetime.now()
```

### Comparing `antidb-2023.7.11/pyproject.toml` & `antidb-2023.7.18/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core>=3.9.0"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "antidb"
-version = "2023.7.11"
+version = "2023.7.18"
 authors = [
     { name="Platon Bykadorov", email="platon.work@gmail.com" },
 ]
 description = "The simplest index-and-search engine for huge multiline text files. Focused primarily on bioinformatics. Inspired by tabix, but isn't its replacement. Written in Python. Works on top of Zstandard Seekable & pyzstd SeekableZstdFile."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `antidb-2023.7.11/src/antidb/antidb.py` & `antidb-2023.7.18/src/antidb/antidb.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 from functools import wraps
 from decimal import Decimal
 from bisect import bisect
 from pyzstd import (CParameter,
                     SeekableZstdFile,
                     ZstdFile)
 
-__version__ = 'v1.3.3'
+__version__ = 'v1.4.0'
 __authors__ = [{'name': 'Platon Bykadorov',
                 'email': 'platon.work@gmail.com',
                 'years': '2023'}]
 
 
 def count_exec_time(any_func):
-    def wrapper(*args):
+    def wrapper(*args, **kwargs):
         exec_time_start = datetime.now()
-        any_func(*args)
+        any_func(*args, **kwargs)
         return (any_func.__name__,
                 str(datetime.now() -
                     exec_time_start))
     return wrapper
 
 
 class FileNotFoundError(Exception):
@@ -146,14 +146,15 @@
     @count_exec_time
     def crt_mem_idx(self):
         with TextIOWrapper(SeekableZstdFile(self.full_idx_path,
                                             mode='r')) as full_idx_opened:
             with TextIOWrapper(ZstdFile(self.mem_idx_path,
                                         mode='w',
                                         level_or_option=self.compr_settings)) as mem_idx_opened:
+                mem_idx_opened.write(f'unidx_lines_quan={self.unidx_lines_quan}\n')
                 while True:
                     full_idx_lstart = full_idx_opened.tell()
                     full_idx_line = full_idx_opened.readline()
                     if not full_idx_line:
                         break
                     full_idx_your_val = full_idx_line.split(',')[0]
                     mem_idx_opened.write(f'{full_idx_your_val},{full_idx_lstart}\n')
@@ -176,23 +177,24 @@
             self.full_idx_opened = TextIOWrapper(SeekableZstdFile(self.full_idx_path,
                                                                   mode='r'))
         if not os.path.exists(self.mem_idx_path):
             raise FileNotFoundError(self.mem_idx_path)
         else:
             self.mem_idx_opened = TextIOWrapper(ZstdFile(self.mem_idx_path,
                                                          mode='r'))
-        self.mem_idx_your_vals, self.full_idx_lstarts = self.read_mem_idx()
+        self.unidx_lines_quan, self.mem_idx_your_vals, self.full_idx_lstarts = self.read_mem_idx()
 
     def read_mem_idx(self):
+        unidx_lines_quan = int(self.mem_idx_opened.readline().rstrip().split('=')[1])
         mem_idx_your_vals, full_idx_lstarts = [], []
         for mem_idx_line in self.mem_idx_opened:
             mem_idx_row = mem_idx_line.rstrip().split(',')
             mem_idx_your_vals.append(mem_idx_row[0])
             full_idx_lstarts.append(int(mem_idx_row[1]))
-        return mem_idx_your_vals, full_idx_lstarts
+        return unidx_lines_quan, mem_idx_your_vals, full_idx_lstarts
 
     def prs(self, your_vals):
         if type(your_vals) in [str,
                                int,
                                float,
                                Decimal]:
             your_vals = [your_vals]
```

### Comparing `antidb-2023.7.11/PKG-INFO` & `antidb-2023.7.18/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antidb
-Version: 2023.7.11
+Version: 2023.7.18
 Summary: The simplest index-and-search engine for huge multiline text files. Focused primarily on bioinformatics. Inspired by tabix, but isn't its replacement. Written in Python. Works on top of Zstandard Seekable & pyzstd SeekableZstdFile.
 Keywords: python,search-engine,parser,performance,bioinformatics,big-data,dbms,indexer,zstd,zstandard,vigg,seekable,pyzstd
 Author-email: Platon Bykadorov <platon.work@gmail.com>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -12,14 +12,17 @@
 Requires-Dist: pyzstd >=0.15.9
 Project-URL: Bug Tracker, https://github.com/PlatonB/antidb/issues
 Project-URL: Homepage, https://github.com/PlatonB/antidb
 
 # antidb
 ## Quick start
 ```
+pip3 install antidb
+```
+```
 from antidb import (Idx,
                     Prs,
                     count_exec_time)
 
 dbsnp_vcf_path = '/mnt/Storage/databases/dbSNP_platon/GCF_000001405.40.vcf'
 dbsnp_idx_prefix = 'all_rsids'
 
@@ -136,21 +139,23 @@
                     empty_res = True
                     ann_file_line = ann_file_line.rstrip()
                     ann_rsid = ann_file_line.split('\t')[args.rsids_col_num - 1]
                     for dbsnp_zst_line in dbsnp_prs.prs(ann_rsid):
                         empty_res = False
                         trg_file_opened.write(ann_file_line +
                                               dbsnp_zst_line)
+                        break
                     if empty_res:
                         for rsmerged_zst_line in rsmerged_prs.prs(ann_rsid):
                             ann_rsid_syns = parse_rsmerged_line.__wrapped__(rsmerged_zst_line)
                             for dbsnp_zst_line in dbsnp_prs.prs(ann_rsid_syns):
                                 empty_res = False
                                 trg_file_opened.write(ann_file_line +
                                                       dbsnp_zst_line)
+                                break
                             if not empty_res:
                                 break
                         else:
                             dump_file_opened.write(ann_file_line + '\n')
 
 
 res_files_crt_time = datetime.now()
```

