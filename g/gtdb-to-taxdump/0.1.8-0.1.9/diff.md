# Comparing `tmp/gtdb_to_taxdump-0.1.8.tar.gz` & `tmp/gtdb_to_taxdump-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gtdb_to_taxdump-0.1.8.tar", last modified: Mon Jul 25 06:38:28 2022, max compression
+gzip compressed data, was "gtdb_to_taxdump-0.1.9.tar", last modified: Tue Jul 18 21:00:11 2023, max compression
```

## Comparing `gtdb_to_taxdump-0.1.8.tar` & `gtdb_to_taxdump-0.1.9.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 06:38:28.095505 gtdb_to_taxdump-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1071 2022-07-25 06:38:13.000000 gtdb_to_taxdump-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-07-25 06:38:28.095505 gtdb_to_taxdump-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4807 2022-07-25 06:38:13.000000 gtdb_to_taxdump-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 06:38:28.095505 gtdb_to_taxdump-0.1.8/bin/
--rw-r--r--   0 runner    (1001) docker     (121)       22 2022-07-25 06:38:13.000000 gtdb_to_taxdump-0.1.8/bin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4296 2022-07-25 06:38:13.000000 gtdb_to_taxdump-0.1.8/bin/acc2gtdb_tax.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5546 2022-07-25 06:38:13.000000 gtdb_to_taxdump-0.1.8/bin/gtdb_to_diamond.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4729 2022-07-25 06:38:13.000000 gtdb_to_taxdump-0.1.8/bin/gtdb_to_taxdump.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4976 2022-07-25 06:38:13.000000 gtdb_to_taxdump-0.1.8/bin/lineage2taxid.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    25068 2022-07-25 06:38:13.000000 gtdb_to_taxdump-0.1.8/bin/ncbi-gtdb_map.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 06:38:28.095505 gtdb_to_taxdump-0.1.8/gtdb2td/
--rw-r--r--   0 runner    (1001) docker     (121)     3576 2022-07-25 06:38:13.000000 gtdb_to_taxdump-0.1.8/gtdb2td/Dmp.py
--rw-r--r--   0 runner    (1001) docker     (121)     8437 2022-07-25 06:38:13.000000 gtdb_to_taxdump-0.1.8/gtdb2td/Graph.py
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-07-25 06:38:13.000000 gtdb_to_taxdump-0.1.8/gtdb2td/IO.py
--rw-r--r--   0 runner    (1001) docker     (121)      889 2022-07-25 06:38:13.000000 gtdb_to_taxdump-0.1.8/gtdb2td/Utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      168 2022-07-25 06:38:13.000000 gtdb_to_taxdump-0.1.8/gtdb2td/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-25 06:38:28.095505 gtdb_to_taxdump-0.1.8/gtdb_to_taxdump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      342 2022-07-25 06:38:28.000000 gtdb_to_taxdump-0.1.8/gtdb_to_taxdump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      427 2022-07-25 06:38:28.000000 gtdb_to_taxdump-0.1.8/gtdb_to_taxdump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-25 06:38:28.000000 gtdb_to_taxdump-0.1.8/gtdb_to_taxdump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-07-25 06:38:28.000000 gtdb_to_taxdump-0.1.8/gtdb_to_taxdump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-07-25 06:38:28.000000 gtdb_to_taxdump-0.1.8/gtdb_to_taxdump.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-07-25 06:38:28.095505 gtdb_to_taxdump-0.1.8/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (121)     1334 2022-07-25 06:38:13.000000 gtdb_to_taxdump-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:00:10.997816 gtdb_to_taxdump-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-07-18 20:59:57.000000 gtdb_to_taxdump-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-18 21:00:10.997816 gtdb_to_taxdump-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4807 2023-07-18 20:59:57.000000 gtdb_to_taxdump-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:00:10.997816 gtdb_to_taxdump-0.1.9/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 20:59:57.000000 gtdb_to_taxdump-0.1.9/bin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4379 2023-07-18 20:59:57.000000 gtdb_to_taxdump-0.1.9/bin/acc2gtdb_tax.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5881 2023-07-18 20:59:57.000000 gtdb_to_taxdump-0.1.9/bin/gtdb_to_diamond.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5022 2023-07-18 20:59:57.000000 gtdb_to_taxdump-0.1.9/bin/gtdb_to_taxdump.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5408 2023-07-18 20:59:57.000000 gtdb_to_taxdump-0.1.9/bin/lineage2taxid.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    25132 2023-07-18 20:59:57.000000 gtdb_to_taxdump-0.1.9/bin/ncbi-gtdb_map.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:00:10.997816 gtdb_to_taxdump-0.1.9/gtdb2td/
+-rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-07-18 20:59:57.000000 gtdb_to_taxdump-0.1.9/gtdb2td/Dmp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8437 2023-07-18 20:59:57.000000 gtdb_to_taxdump-0.1.9/gtdb2td/Graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-07-18 20:59:57.000000 gtdb_to_taxdump-0.1.9/gtdb2td/IO.py
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-07-18 20:59:57.000000 gtdb_to_taxdump-0.1.9/gtdb2td/Utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-07-18 20:59:57.000000 gtdb_to_taxdump-0.1.9/gtdb2td/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:00:10.997816 gtdb_to_taxdump-0.1.9/gtdb_to_taxdump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-07-18 21:00:10.000000 gtdb_to_taxdump-0.1.9/gtdb_to_taxdump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-07-18 21:00:10.000000 gtdb_to_taxdump-0.1.9/gtdb_to_taxdump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 21:00:10.000000 gtdb_to_taxdump-0.1.9/gtdb_to_taxdump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 21:00:10.000000 gtdb_to_taxdump-0.1.9/gtdb_to_taxdump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 21:00:10.000000 gtdb_to_taxdump-0.1.9/gtdb_to_taxdump.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 21:00:10.997816 gtdb_to_taxdump-0.1.9/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1334 2023-07-18 20:59:57.000000 gtdb_to_taxdump-0.1.9/setup.py
```

### Comparing `gtdb_to_taxdump-0.1.8/LICENSE` & `gtdb_to_taxdump-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `gtdb_to_taxdump-0.1.8/README.md` & `gtdb_to_taxdump-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `gtdb_to_taxdump-0.1.8/bin/acc2gtdb_tax.py` & `gtdb_to_taxdump-0.1.9/bin/acc2gtdb_tax.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 #!/usr/bin/env python
-
 from bin import __version__
+import os
+import re
 import argparse
 import gzip
 import logging
-import os
-from tqdm.contrib.concurrent import thread_map
-from tqdm import tqdm
-import re
 from functools import partial
 from pathlib import Path
+from tqdm import tqdm
+from tqdm.contrib.concurrent import thread_map
 
 
 # argparse
 desc = "Create Sequence accession to TAXID mapping file"
 epi = """DESCRIPTION:
 Creates a compressed acc2tax mapping file to retrieve the TAXID
 from a sequence accession.
@@ -47,30 +46,30 @@
     help="Output acc2tax file (Default: %(default)s)",
 )
 parser.add_argument("--version", action="version", version=__version__)
 
 logging.basicConfig(format="%(asctime)s - %(message)s", level=logging.DEBUG)
 
 
-def get_all_genomes(genome_dir):
+def get_all_genomes(genome_dir: str) -> list:
     """Get path to all genomes in GTDB directory
     Args:
         genome_dir (str): Path to GTDB genome directory
     Returns:
         list: List of paths to all genomes
     """
     genome_paths = []
     for root, dirs, files in os.walk(genome_dir):
         for f in files:
             if f.endswith(".fna.gz"):
                 genome_paths.append(os.path.join(root, f))
     return genome_paths
 
 
-def genome_acc2tax(names):
+def genome_acc2tax(names: str) -> dict:
     """Get genome accession to taxid mapping
     Args:
         names (str): Path to GTDB names.dmp file
     Returns:
         dict: genome_accession2taxid dict
     """
     genome_acc2taxid = {}
@@ -78,15 +77,15 @@
         for line in f:
             line = line.rstrip().strip().replace("\t", "").split("|")
             genome_acc2taxid[line[1]] = line[0]
 
     return genome_acc2taxid
 
 
-def seq_acc2tax(genome_file, genome_acc2taxid, seq_acc2taxid):
+def seq_acc2tax(genome_file: str, genome_acc2taxid: dict, seq_acc2taxid: dict) -> None:
     """
     Creates the sequence accession2taxid mappings
     Args:
         genome_file(str): Path to one of the GTDB genomes
         genome_acc2taxid(dict): genome_accesion2taxid dict
         seq_acc2tax(dict): sequence_accession2taxid dict
     """
@@ -111,22 +110,22 @@
                 except KeyError:
                     print(line)
                     pass
             else:
                 continue
 
 
-def write_acc2tax(seq_acc2taxid, outfile):
+def write_acc2tax(seq_acc2taxid: dict, outfile: str) -> None:
     with gzip.open(outfile, "wb") as f:
         f.write("accession\taccession.version\ttaxid\n".encode())
         for acc in tqdm(seq_acc2taxid):
             f.write(f"{acc.split('.')[0]}\t{acc}\t{seq_acc2taxid[acc]}\n".encode())
 
 
-def main(args):
+def main(args: dict) -> None:
     logging.debug("Reading GTDB names.dmp file")
     genome_acc2taxid = genome_acc2tax(args.names_dmp)
 
     logging.debug("Listing all GTDB genomes")
     print(args.gtdb_genome_dir)
     gtdb_genomes = get_all_genomes(args.gtdb_genome_dir)
```

### Comparing `gtdb_to_taxdump-0.1.8/bin/gtdb_to_diamond.py` & `gtdb_to_taxdump-0.1.9/bin/gtdb_to_diamond.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,29 +1,21 @@
 #!/usr/bin/env python
 # import
 from __future__ import print_function
 ## batteries
 import os
-import re
-import sys
-import gzip
-import glob
 import shutil
 import argparse
 import logging
-import urllib.request
-import codecs
-import tarfile
-from collections import OrderedDict
 ## package
 from bin import __version__
 import gtdb2td
 
 # argparse
-desc = 'Converting GTDB taxonomy to input for "diamond makedb --taxonmap"'
+desc = 'Convert GTDB taxonomy to input for "diamond makedb --taxonmap"'
 epi = """DESCRIPTION:
 Convert Genome Taxonomy Database (GTDB) representative genome
 gene amino acid sequences to the input files required for 
 "diamond makedb --taxonmap", with allows for taxonomic identification
 with diamond (LCA-based method).
 
 Example of getting a GTDB faa fasta tarball:
@@ -63,17 +55,23 @@
 parser.add_argument('--version', action='version', version=__version__)
 
 # logging
 logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.DEBUG)
 
 
 # functions
-def accession2taxid(names_dmp, faa_files, outdir):
+def accession2taxid(names_dmp: dict, faa_files: dict, outdir: str) -> None:
     """ 
-    Creating accession2taxid table
+    Creating accession2taxid table.
+    Params:
+      names_dmp: dict of taxdump names.dmp file
+      faa_files: dict of faa file paths and accessions 
+      outdir: str output directory
+    Returns:
+      None (writes accession2taxid.tsv file)
     """
     outfile = os.path.join(outdir, 'accession2taxid.tsv')    
     logging.info('Creating accession2taxid table...')
     with open(outfile, 'w') as outF:
         header = ['accession', 'accession.version', 'taxid', 'gi']
         outF.write('\t'.join(header) + '\n')
         for accession,faa_file in faa_files.items():
@@ -83,17 +81,23 @@
                 msg = 'Cannot find {} accession in names.dmp'
                 raise KeyError(msg.format(accession))
             acc_base = os.path.splitext(accession)[0]
             line = [acc_base, accession, str(taxID), '']
             outF.write('\t'.join(line) + '\n')
     logging.info('  File written: {}'.format(outfile))
     
-def faa_merge(faa_files, outdir, gzip_out=False):
+def faa_merge(faa_files: dict, outdir: str, gzip_out: bool=False) -> None:
     """ 
-    Reading in, formatting, and merging all faa files
+    Reading in, formatting, and merging all faa files.
+    Params:
+      faa_files: dict of faa file paths and accessions  
+      outdir: str output directory
+      gzip_out: bool gzip output fasta?
+    Returns:
+      None (writes gtdb_all.faa file)
     """
     outfile = os.path.join(outdir, 'gtdb_all.faa')
     if gzip_out:
         outfile += '.gz'
     
     logging.info('Formating & merging faa files...')
     seq_cnt = 0
@@ -111,15 +115,15 @@
                     if gzip_out:
                         line = line.encode('utf-8')
                     outF.write(line)
     logging.info('  File written: {}'.format(outfile))
     logging.info('  No. of seqs. written: {}'.format(seq_cnt))
 
 ## main interface
-def main(args):
+def main(args: dict) -> None:
     """ 
     Main interface
     """
     if not os.path.isdir(args.outdir):
         os.makedirs(args.outdir)        
     # copying nodes
     gtdb2td.Dmp.copy_nodes(args.nodes_dmp, args.outdir)
```

### Comparing `gtdb_to_taxdump-0.1.8/bin/gtdb_to_taxdump.py` & `gtdb_to_taxdump-0.1.9/bin/gtdb_to_taxdump.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 import codecs
 from collections import OrderedDict
 ## package
 from bin import __version__
 import gtdb2td
 
 # argparse
-desc = 'Converting GTDB taxonomy to NCBI taxdump format'
+desc = 'Convert GTDB taxonomy to NCBI taxdump format'
 epi = """DESCRIPTION:
 Convert Genome Taxonomy Database (GTDB) taxonomy files
 to NCBI taxdump format (names.dmp & nodes.dmp).
 
 The input can be >=1 tsv file with the GTDB taxonomy
 or >=1 url to the tsv file(s). Input can be uncompressed
 or gzip'ed.
 
 The input table format should be >=2 columns,
 (Column1 = accession, Column2 = gtdb_taxonomy),
-and no header
+and no header.
 
 The *.dmp files are written to `--outdir`.
 A tab-delim table of taxID info is written to STDOUT.
 
 If `--table` is provided, then the taxID info is appended
 to the provided table file (also see `--column`). The table
 must be tab-delimited.
@@ -54,17 +54,22 @@
 parser.add_argument('-c', '--column', type=str, default='accession',
                     help='Column in --table that contains genome accessions (Default: %(default)s)')
 parser.add_argument('--version', action='version', version=__version__)
 
 logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.DEBUG)
 
         
-def load_gtdb_tax(infile, graph):
+def load_gtdb_tax(infile: str, graph) -> None:
     """
-    loading gtdb taxonomy & adding to DAG
+    Load gtdb taxonomy & adding to DAG
+    Params:
+      infile: input file url or path
+      graph: graph object
+    Returns:
+      None
     """
     # url or file download/open
     try:        
         inF = gtdb2td.Utils.get_url_data(infile)
     except (OSError,ValueError) as e:
         try:
             ftpstream = urllib.request.urlopen(infile)
@@ -98,22 +103,30 @@
             else:
                 graph.add_edge(tax[ii-1], cls)
     try:
         inF.close()
     except AttributeError:
         pass
 
-def write_blank_dmp(outfile, outdir=None):
+def write_blank_dmp(outfile: str, outdir: str=None) -> None:
+    """
+    Write a blank taxdump file.
+    Params:
+      outfile: filename
+      outdir: output directory (Default: current dir)
+    Returns:
+      None
+    """
     if outdir is not None:
         outfile = os.path.join(outdir, outfile)
     with open(outfile, 'w') as outF:
         outF.write('#\n')
-    logging.info('File written: {}'.format(outfile))
+    logging.info(f'File written: {outfile}')
     
-def main(args):
+def main(args: dict) -> None:
     # creating DAG
     graph = gtdb2td.Graph()
     graph.add_vertex('root')
     for F in args.tax_file:
         logging.info('Loading: {}'.format(F))
         load_gtdb_tax(F, graph)
     # output
```

### Comparing `gtdb_to_taxdump-0.1.8/bin/lineage2taxid.py` & `gtdb_to_taxdump-0.1.9/bin/lineage2taxid.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 #!/usr/bin/env python
 # import
 ## batteries
 from __future__ import print_function
-import os
-import sys
-import re
-import gzip
-import bz2
 import argparse
 import logging
 ## 3rd party
 import networkx as nx
 from networkx.algorithms.dag import descendants
 from networkx.algorithms.lowest_common_ancestors import lowest_common_ancestor
 from networkx.algorithms.shortest_paths.unweighted import bidirectional_shortest_path
@@ -64,55 +59,69 @@
 parser.add_argument('--taxid-column', type=str, default='taxid',
                     help='Name of taxid column that will be appended to the input table')
 parser.add_argument('--taxid-rank-column', type=str, default='taxid_rank',
                     help='Name of taxid-rank column that will be appended to the input table')
 parser.add_argument('--version', action='version', version=__version__)
 
 # functions
-def lineage2taxid(lineage, G):    
+def lineage2taxid(lineage: str, G) -> list:
+    """
+    Convert taxonomy lineage string to list of taxids
+    Params:
+      lineage: taxonomy lineage string
+      G: graph object containing NCBI taxonomy
+    Return:
+      List of taxids (or [NA,NA] if no taxid could be mapped)
+    """
     lineage = lineage.split(';')    
     for cls in lineage[::-1]:
         cls = cls.lower()
         nodes = [x for x,y in G.nodes(data=True) if y['name'] == cls]
         if len(nodes) == 1:
             return [nodes[0], G.nodes[nodes[0]]['rank']]
     msg = 'Could not find a taxid for lineage: {}'
     logging.warning(msg.format(';'.join(lineage)))
     return ['NA', 'NA']            
 
-def parse_lineage_table(table_file, lineage_column, G,
-                        taxid_column, taxid_rank_column):
+def parse_lineage_table(table_file: str, lineage_column: str, G, 
+                        taxid_column: str, taxid_rank_column: str) -> None:
     """
-    Parsing lineage and finding taxid
+    Parse lineage and finding taxid.
+    Params:
+      table_file: input table file
+      lineage_column: column containing lineages
+      G: graph containing NCBI taxonomy
+      taxid_column: column name to write taxids
+      taxid_rank_column: column name to write taxid ranks
+    Return:
+      None
     """
-    logging.info('Parsing file: {}'.format(table_file))
+    logging.info(f'Parsing file: {table_file}')
     header = {}
     with gtdb2td.Utils.Open(table_file) as inF:
         for i,line in enumerate(inF):
             line = gtdb2td.Utils.Decode(line).rstrip().split('\t')
             # header
             if i == 0:
                 header = {x:ii for ii,x in enumerate(line)}
                 try:
                     _ = header[lineage_column]
                 except KeyError:
-                    msg = 'Cannot find column: {}'
-                    raise KeyError(msg.format(lineage_column))
+                    raise KeyError(f'Cannot find column: {lineage_column}')
                 print('\t'.join(line + [taxid_column, taxid_rank_column]))
                 continue
             # body
             lineage = line[header[lineage_column]]
             taxid,rank = lineage2taxid(lineage, G)
             print('\t'.join(line + [str(taxid), str(rank)]))
             # status
             if i > 0 and (i+1) % 100 == 0:
-                logging.info('  Records processed: {}'.format(i+1))
+                logging.info(f'  Records processed: {i+1}')
 
-## main interface
-def main(args):
+def main(args: dict) -> None:
     """
     Main interface
     """
     # loading dmp as DAG
     G = gtdb2td.Dmp.load_dmp(args.names_dmp, args.nodes_dmp)
     # lineage2taxid
     parse_lineage_table(args.table_file, args.lineage_column, G=G,
```

### Comparing `gtdb_to_taxdump-0.1.8/bin/ncbi-gtdb_map.py` & `gtdb_to_taxdump-0.1.9/bin/ncbi-gtdb_map.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,39 +1,34 @@
 #!/usr/bin/env python
 from __future__ import print_function
 # import
 ## batteries
 import os
-import sys
 import re
-import gzip
-import bz2
 import shutil
 import tarfile
 import argparse
 import logging
 import random
-import csv
 import urllib.request
-import codecs
 import functools
 import multiprocessing as mp
 from collections import Counter
 ## 3rd party
 import networkx as nx
 from networkx.algorithms.dag import descendants
 from networkx.algorithms.dag import ancestors
 from networkx.algorithms.lowest_common_ancestors import lowest_common_ancestor
 from networkx.algorithms.shortest_paths.unweighted import bidirectional_shortest_path
 from bin import __version__
 ## package
 import gtdb2td
 
 # argparse
-desc = 'Mapping between NCBI & GTDB taxonomies'
+desc = 'Map between NCBI & GTDB taxonomies'
 epi = """DESCRIPTION:
 Using the GTDB metadata table (which contains both NCBI and GTDB taxonomies)
 to map taxonomic classifications between the 2 taxonomies.
 
 For example, determine GTDB equivalent of the NCBI taxonomic classifications:
 * g__Bacillus
 * s__Xanthomonas oryzae
@@ -54,14 +49,15 @@
   * If no match in reference taxonomy or no LCA that is >= (--fraction), then the 
     target LCA is "unclassified"
 
 Notes:
 * The input table of queries should be tab-delimited (select the column with --column).
 * Query-target matching is caps-invariant (all converted to lower case for matching)!
 * The table can have a header (see --header) and can be compressed via gzip or bzip2.
+* See https://github.com/nick-youngblut/gtdb_to_taxdump/tree/master/tests/data/ncbi-gtdb for example queries.
 
 Output:
 * Output written to --outdir
 * `taxonomy_map_summary.tsv`
   * ncbi_taxonomy
     * NCBI taxonomy name
   * gtdb_taxonomy
@@ -132,72 +128,24 @@
                     help='Verbose output (Default: %(default)s)')
 parser.add_argument('--version', action='version', version=__version__)
 logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.DEBUG)
 
 
 # functions
 
-# def load_dmp(names_dmp_file, nodes_dmp_file, no_prefix=False):
-#     """
-#     Loading NCBI names/nodes dmp files as DAG
-#     Arguments:
-#       names_dmp_file : str, names.dmp file
-#       nodes_dmp_file : str, nodes.dmp file 
-#     Return:
-#       network.DiGraph object
-#     """
-#     regex = re.compile(r'\t\|\t')
-#     # nodes
-#     logging.info('Loading file: {}'.format(names_dmp_file))
-#     idx = {}    # {taxid : name}
-#     with open(names_dmp_file) as inF:
-#         for line in inF:
-#             line = line.rstrip()
-#             if line == '':
-#                 continue
-#             line = regex.split(line)
-#             idx[int(line[0])] = line[1]
-#     # names
-#     logging.info('Loading file: {}'.format(nodes_dmp_file))
-#     G = nx.DiGraph()
-#     G.add_node(0, rank = 'root', name = 'root')
-#     with open(nodes_dmp_file) as inF:
-#         for line in inF:
-#             line = line.rstrip()
-#             if line == '':
-#                 continue
-#             line = regex.split(line)
-#             taxid_child = int(line[0])
-#             taxid_parent = int(line[1])
-#             rank_child = line[2]
-#             name_child = idx[taxid_child]
-#             name_parent = idx[taxid_parent]
-#             if rank_child == 'species':
-#                 name_child = 's__' + name_child
-#             # adding node
-#             G.add_node(taxid_child, rank=rank_child, name=name_child)
-#             # adding edge
-#             if taxid_parent == 1:
-#                 G.add_edge(0, taxid_child)
-#             else:
-#                 G.add_edge(taxid_parent, taxid_child)
-#     idx.clear()
-#     logging.info('  No. of nodes: {}'.format(G.number_of_nodes()))
-#     logging.info('  No. of edges: {}'.format(G.number_of_edges()))
-#     return G
-
-def format_taxonomy(T, hierarchy, acc, no_prefix=False):
+def format_taxonomy(T, hierarchy: list, acc: str, no_prefix=False) -> list:
     """
     Formatting taxonomy to conform to a set hierarchy
-    Arguments:
-      T : iterable, taxonomy
-      hierarchy : taxonomic hierarchy 
-      acc : accession
+    Params:
+      T: iterable, taxonomy
+      hierarchy: taxonomic hierarchy 
+      acc: accession
+      no_prefix: strip taxonomic prefixes?
     Return:
-      [taxonomy_level1, taxonomy_level2, ...]
+      List of taxonomic names in the hierarchy; [taxonomy_level1, taxonomy_level2, ...]
     """
     regex = re.compile(r'^[dpcofgs]__$')
     regex2 = re.compile(r'^X*[dpcofgs]__')    
     Tx = ['' for i in range(len(hierarchy))]
     for i,x in enumerate(hierarchy[:-1]):
         if len(T) < i + 1 or T[i] == '' or T[i] == 'unclassified' \
            or regex.search(T[i]):
@@ -205,65 +153,75 @@
         else:
             Tx[i] = T[i]
         if no_prefix is True:
             Tx[i] = regex2.sub('', Tx[i])
     Tx[-1] = acc
     return Tx
 
-def add_taxonomy(line, line_num, header, G, tax='ncbi_taxonomy', no_prefix=False):
+def add_taxonomy(line: list, line_num: int, header: dict, G, 
+                 tax='ncbi_taxonomy', no_prefix=False) -> None:
     """
-    Adding taxonomy nodes/edits to the graph
-    Arguments:
-      line : iterable, line of metadata file
-      line_num : int, line number of metadata file
+    Add taxonomy nodes/edits to the graph.
+    Params:
+      line: iterable, line of metadata file
+      line_num: int, line number of metadata file
       header : dict, index of header for metadata file
       G : taxonomy graph
       tax : ncbi or gtdb?
     Return:
-      In-place edit of G
+      None; in-place edit of G
     """
     hierarchy = ['domain', 'phylum', 'class', 'order',
                  'family', 'genus', 'species', 'strain']
-    # checking taxonomy format
+    # check taxonomy format
     acc = line[header['accession']]
     T = line[header[tax]].split(';')
     T = format_taxonomy(T, hierarchy, acc, no_prefix=no_prefix)
-    # adding taxonomy to graph
+    # add taxonomy to graph
     for i in range(len(hierarchy)):        
-        # adding node
+        # add node
         G[tax].add_node(T[i].lower(), taxonomy=hierarchy[i], orig_name=T[i])
-        # adding edge
+        # add edge
         if i == 0:
             G[tax].add_edge('root', T[i].lower())
         else:
             G[tax].add_edge(T[i-1].lower(), T[i].lower())
 
-def dl_uncomp(url):
+def dl_uncomp(url: str) -> tuple:
     """
-    Downloading and extracting GTDB metadata tarball
-    Arguments:
-      url : str, url of GTDB metadata tarball
+    Download and extracting GTDB metadata tarball.
+    Params:
+      url: str, url of GTDB metadata tarball
     Return: 
-      (metadata_filehandle, output_directory)
+      Tuple of (metadata_filehandle, output_directory)
     """
     file_tmp = urllib.request.urlretrieve(url, filename=None)[0]
     tmpdir = os.path.dirname(file_tmp)
     outdir = os.path.basename(url)
     outdir = re.sub(r'\.tar.gz$', '', outdir)
     outdir = os.path.join(tmpdir, outdir)
     tar = tarfile.open(file_tmp)
     tar.extract(tar.getmembers()[0], outdir)
     inF = open(os.path.join(outdir, tar.getnames()[0]))
     return inF,outdir
             
-def load_gtdb_metadata(infile, G, completeness, contamination, no_prefix=False):
+def load_gtdb_metadata(infile: str, G, completeness: float, 
+                       contamination: float, no_prefix: bool=False):
     """
-    Loading gtdb taxonomy & adding to DAG 
+    Load gtdb taxonomy & adding to DAG.
+    Params:
+      infile: input file url or path
+      G: graph object
+      completeness: min completeness
+      contamination: max contamination
+      no_prefix: strip taxonomic prefixes?
+    Return:
+      Graph object (DAG)
     """
-    logging.info('Loading: {}'.format(infile))
+    logging.info(f'Loading: {infile}')
     # input as file or url
     try:
         inF,tmpdir = dl_uncomp(infile)
     except ValueError:
         inF = gtdb2td.Utils.Open(infile)
         tmpdir = None
     # reading
@@ -277,40 +235,39 @@
             line = line.rstrip()
         except AttributeError:
             line = line[0].rstrip()
         if line == '':
             continue
         line = line.split('\t')
         if len(line) < 2:
-            msg = 'Line{} does not contain >=2 columns'
-            raise ValueError(msg.format(i+1))
+            raise ValueError(f'Line{i+1} does not contain >=2 columns')
         # header
         if i == 0:
             header = {x:ii for ii,x in enumerate(line)}
             continue
         # filtering out records lacking an NCBI taxonomy
         try:
             X = line[header['ncbi_taxonomy']]
         except KeyError:
-            raise KeyError('Cannot find "ncbi_taxonomy"')
+            raise KeyError(f'Cannot find the "ncbi_taxonomy" column in {infile}')
         if X == 'none':
             stats['no ncbi tax'] += 1
             continue
         # filtering by checkM stats
         try:
             X = line[header['checkm_completeness']]
         except KeyError:
-            raise KeyError('Cannot find "checkm_completeness"')
+            raise KeyError(f'Cannot find the "checkm_completeness" column in {infile}')
         if float(X) < completeness:
             stats['completeness'] += 1
             continue
         try:
             X = line[header['checkm_contamination']]
         except KeyError:
-            raise KeyError('Cannot find "checkm_contamination"')
+            raise KeyError(f'Cannot find the "checkm_contamination" column in {infile}')
         if float(X) >= contamination:
             stats['contamination'] += 1
             continue
         # Adding taxonomies to graphs        
         add_taxonomy(line, i, header, G, tax='gtdb_taxonomy',
                      no_prefix=no_prefix)
         add_taxonomy(line, i, header, G, tax='ncbi_taxonomy',
@@ -326,34 +283,36 @@
     # stats
     msg = '  Entries lacking an NCBI taxonomy: {}'
     logging.info(msg.format(stats['no ncbi tax']))
     msg = '  Completeness-filtered entries: {}'
     logging.info(msg.format(stats['completeness']))
     msg = '  Contamination-filtered entries: {}'
     logging.info(msg.format(stats['contamination']))
-    logging.info('  Entries used: {}'.format(stats['passed']))    
+    logging.info(f'  Entries used: {stats["passed"]}')
     return G
 
 def DiGraph_w_root():
     """
     Create directed  graph with a root node
     """
     G = nx.DiGraph()
     G.add_node('root')
     return G
 
-def lca_frac_pass(D, lca_frac):
+def lca_frac_pass(D: dict, lca_frac: float) -> None:
     """
     Determine which, if any, of the LCAs pass the homogeneity cutoff.
     "homogeneity" means the fraction of tips with the target LCA 
       (eg., 90% of all tips have this LCA).
     If the cutoff is not passed, then returning [None,None]
-    Arguments:
-      D : dict, LCA dict
-      lca_frac : float, fraction of decendents that must have the same taxonomy
+    Params:
+      D: LCA dict
+      lca_frac: fraction of decendents that must have the same taxonomy
+    Return:
+      None
     """
     D = Counter(D)
     try:
         mc = D.most_common(1)
     except IndexError:
         return [None,None]
     if re.search(r'^[Xx][pcofgs]__', mc[0][0]):
@@ -363,48 +322,63 @@
     except IndexError:
         return [None,None]
     if frac >= lca_frac:
         return [mc[0][0], str(round(frac, 3))]
     else:
         return [None,None]
 
-def lca_many_nodes(G, nodes, lca_frac=1.0):
+def lca_many_nodes(G, nodes: list, lca_frac: float=1.0) -> list:
     """
-    algorithm: using closest distance to 'root'
+    Algorithm: using closest distance to 'root'
+    Params:
+      G: graph object
+      nodes: list of nodes
+      lca_frac: fraction of decendents that must have the same taxonomy
+    Return:
+      List of LCAs that pass the homogeneity cutoff
     """
     hierarchy = ['root', 'domain', 'phylum', 'class', 'order',
                  'family', 'genus', 'species', 'strain']    
     T = [{} for x in hierarchy]
-    # getting path from nodes to root
+    # Get path from nodes to root
     for n in nodes:
         path = bidirectional_shortest_path(G, 'root', n)
         for i,node in enumerate(path):
             try:
                 T[i][node] += 1
             except KeyError:
                 T[i][node] = 1
-    ## from finest to coarsest, does any classification pass the lca_frac?
+    ## From finest to coarsest, does any classification pass the lca_frac?
     ### note: species is lowest possible level
     for i in range(len(T)-1)[::-1]:
         lca = lca_frac_pass(T[i], lca_frac)
         if lca[0] is not None and lca[0] != 'root':
             try:
                 lca[0] = G.nodes[lca[0]]['orig_name']
             except KeyError:
                 msg = 'Cannot find "orig_name" for "{}"'
                 raise KeyError(msg.format(lca[0]))
             lineage = [[y for y in x.keys()][0] for x in T[:i+1]]
             return lca + [hierarchy[i], ';'.join(lineage[1:])]
     logging.warning('Cannot find LCA for nodes: {}'.format(','.join(nodes)))
     return ['unclassified', 'NA', 'NA', 'NA']
 
-def _query_tax(tax_queries, G, qtax, ttax, lca_frac=1.0, max_tips=100,
-               verbose=False):
+def _query_tax(tax_queries: list, G, qtax: str, ttax: str, 
+               lca_frac: float=1.0, max_tips: int=100,
+               verbose: bool=False) -> dict:
     """
-    Querying list of taxonomic names
+    Querying list of taxonomic names.
+    Params:
+      tax_queries: list of taxonomic names to query
+      G: graph containing taxonomy
+      qtax: query taxonomy column name
+      ttax: target taxonomy column name
+      lca_frac: fraction of decendents that must have the same taxonomy
+      max_tips: maximum number of tips to consider
+      verbose: print progress updates?
     Return:
       {query : [new_taxname, lca_score, rank]}
     """
     pid = os.getpid()
     idx = {}
     status = {'hit' : 0, 'no hit': 0}
     # iterating queries
@@ -435,17 +409,22 @@
     # status
     msg = 'PID{}: Finished! Queries={}, Hits={}, No-Hits={}'
     logging.info(msg.format(pid, status['hit'] + status['no hit'],
                             status['hit'], status['no hit']))
     # return
     return idx
 
-def queries_taxid2species(queries, tax_graph):
+def queries_taxid2species(queries: dict, tax_graph) -> dict:
     """
-    If queries were taxids, getting taxonomic classification for each query
+    If queries were taxids, getting taxonomic classification for each query.
+    Params:
+      queries: dict of {query_id: taxid}
+      tax_graph: networkx graph of taxonomy
+    Return:
+      {query_id: [taxname, rank]}
     """
     logging.info('Converting query taxids to species-level classifications')
     queries_new = {}
     for q,cnt in queries.items():
         try:
             q = int(list(q)[0])
         except ValueError:
@@ -466,35 +445,36 @@
         if rank == 'species':
             queries_new[(node['name'].lower(), node['name'])] = cnt        
     queries.clear()
     logging.info('  No. of queries: {}'.format(sum(queries_new.values())))
     logging.info('  No. of de-rep queries: {}'.format(len(queries_new.keys())))
     return queries_new
                 
-def query_tax(tax_queries, G, tax, lca_frac=1.0, max_tips=100,
-              column=1, header=False, tax_graph=None, prefix='',
-              procs=1, verbose=False):
-    """
-    Querying list of taxonomic names    
-    Params:
-      tax_queries : str, text file of taxonomic queries
-      G : nx.graph, graphs for each of the 2 taxonomies
-      tax : str, either 'ncbi_taxonomy' or 'gtdb_taxonomy'
-      lca_frac : float, taxonomic "purity" of node required to consider it the LCA
-      max_tips : int, the max number of tips considered for determining the LCA
-      column : the column in the tax_queries file that contains the taxonomic classifications
-      header : does the tax_queries file contain a header?
-      tax_graph : a graph that will be used for converting NCBI taxids to species-level queries
-      prefix : add a prefix to all of the queries (eg., "s__")?      
+def query_tax(tax_queries: str, G, tax: str, lca_frac: float=1.0, 
+              max_tips: int=100, column: int=1, header: bool=False, 
+              tax_graph=None, prefix: str='',
+              procs: int=1, verbose: bool=False) -> dict:
+    """
+    Querying list of taxonomic names.   
+    Params:
+      tax_queries: text file of taxonomic queries
+      G: nx.graph, graphs for each of the 2 taxonomies
+      tax: either 'ncbi_taxonomy' or 'gtdb_taxonomy'
+      lca_frac: taxonomic "purity" of node required to consider it the LCA
+      max_tips: the max number of tips considered for determining the LCA
+      column: the column in the tax_queries file that contains the taxonomic classifications
+      header: does the tax_queries file contain a header?
+      tax_graph: a graph that will be used for converting NCBI taxids to species-level queries
+      prefix: add a prefix to all of the queries (eg., "s__")?      
     Return:
       {(node_name_lowercase, node_name) : count}   
     """
     ttax = 'ncbi_taxonomy' if tax == 'gtdb_taxonomy' else 'gtdb_taxonomy'
     # loading & batching queries
-    logging.info('Reading in queries: {}'.format(tax_queries))
+    logging.info(f'Reading in queries: {tax_queries}')
     n_queries = 0
     queries = {}
     with gtdb2td.Utils.Open(tax_queries) as inF:
         for i,line in enumerate(inF):
             if i == 0 and header:
                 continue
             line = gtdb2td.Utils.Decode(line)
@@ -516,55 +496,70 @@
         queries = queries_taxid2species(queries, tax_graph)
     # batching
     logging.info('Batching queries...')
     q_batch = [[] for i in range(procs)]
     for i,q in enumerate(queries):
         q_batch[i % procs].append(q)
     queries = None
-    logging.info('  No. of batches: {}'.format(len(q_batch)))
-    logging.info('  Queries per batch: {}'.format(len(q_batch[0])))
+    logging.info(f'  No. of batches: {len(q_batch)}')
+    logging.info(f'  Queries per batch: {len(q_batch[0])}')
     # query graphs
     logging.info('Querying taxonomies...')
     func = functools.partial(_query_tax, G=G, qtax=tax, ttax=ttax,
                              lca_frac = lca_frac, max_tips=max_tips,
                              verbose=verbose)
     if procs > 1:
         P = mp.Pool(procs)
         idx = P.map(func, q_batch)
     else:
         idx = map(func, q_batch)    
     return idx
 
-def write_table(idx, outdir, qtax):
+def write_table(idx: dict, outdir: str, qtax: str) -> None:
     """
-    Writing tab-delim table of taxonomy mappings to STDOUT
+    Write tab-delim table of taxonomy mappings to STDOUT.
+    Params:
+      idx: dict of {query_id: [taxname, count]}
+      outdir: output directory
+      qtax: either 'ncbi_taxonomy' or 'gtdb_taxonomy'
+    Return:
+      None
     """
     if not os.path.isdir(outdir):
         os.makedirs(outdir)
     outfile = os.path.join(outdir, 'taxonomy_map_summary.tsv')
     ttax = 'ncbi_taxonomy' if qtax == 'gtdb_taxonomy' else 'gtdb_taxonomy'
     with open(outfile, 'w') as outF:
         outF.write('\t'.join([qtax, ttax, 'lca_frac',
                               'target_tax_level', 'lineage']) + '\n')
         for x in idx:
             for k,v in x.items():
                 outF.write('\t'.join([k] + v) + '\n')
-    logging.info('File written: {}'.format(outfile))
+    logging.info(f'File written: {outfile}')
 
-def rename(tax_idx, tax_queries, outdir, column=1, header=False):
+def rename(tax_idx: list, tax_queries: str, outdir: str, 
+           column: int=1, header: bool=False) -> None:
     """
-    Renaming queries with new taxonomic classifications.
+    Rename queries with new taxonomic classifications.
     All entries that cannot be re-named will be excluded in the output.
+    Params:
+      tax_idx: list of dicts of {query_id: [taxname, count]}
+      tax_queries: text file of taxonomic queries
+      outdir: output directory
+      column: the column in the tax_queries file that contains the taxonomic classifications
+      header: does the tax_queries file contain a header?
+    Return:
+      None
     """
-    # converting tax_idx to a simple index
+    # Convert tax_idx to a simple index
     idx = {}  # {old_tax : new_tax}
     for x in tax_idx:
         for k,v in x.items():
             idx[k] = v[0]
-    # renaming queries
+    # Rename queries
     if not os.path.isdir(outdir):
         os.makedirs(outdir)
     outfile = os.path.join(outdir, 'queries_renamed.tsv')
     status = {'renamed' : 0, 'excluded' : 0}
     with gtdb2td.Utils.Open(tax_queries) as inF, open(outfile, 'w') as outF:
         for i,line in enumerate(inF):
             try:
@@ -583,48 +578,48 @@
                     continue
                 if line[column-1].lower() == 'unclassified':
                     status['renamed'] -= 1
                     status['excluded'] += 1
                     continue
             outF.write('\t'.join(line) + '\n')
     # status
-    logging.info('File written: {}'.format(outfile))
-    logging.info('  No. of queries renamed: {}'.format(status['renamed']))
-    logging.info('  No. of queries excluded: {}'.format(status['excluded']))
+    logging.info(f'File written: {outfile}')
+    logging.info(f'  No. of queries renamed: {status["renamed"]}')
+    logging.info(f'  No. of queries excluded: {status["excluded"]}')
             
-def main(args):
+def main(args: dict) -> None:
     """
     Main interface
     """
-    # loading ncbi dmp files if provided
+    # Load ncbi dmp files, if provided
     if args.names_dmp is not None and args.nodes_dmp is not None:
         ncbi_tax = gtdb2td.Dmp.load_dmp(args.names_dmp, args.nodes_dmp)
     else:
         ncbi_tax = None    
-    # loading the metadata as graphs
+    # Load the metadata as graphs
     G = {'ncbi_taxonomy' : DiGraph_w_root(),
          'gtdb_taxonomy' : DiGraph_w_root()}
     for F in args.gtdb_metadata:
        load_gtdb_metadata(F, G, args.completeness, args.contamination,
                           no_prefix=args.no_prefix)
-    # querying
+    # Query taxonomy
     idx = query_tax(args.tax_queries, G,
                     tax=args.query_taxonomy,
                     lca_frac = args.fraction,
                     max_tips = args.max_tips,
                     column = args.column,
                     header = args.header,
                     tax_graph = ncbi_tax,
                     prefix = args.prefix,
                     procs = args.procs, 
                     verbose = args.verbose)
-    # re-naming taxa
+    # Rename taxa
     if args.rename:
         rename(idx, args.tax_queries, args.outdir,
                column = args.column, header = args.header)
-    # writing results
+    # Write results
     write_table(idx, args.outdir, qtax=args.query_taxonomy)
              
 if __name__ == '__main__':
     args = parser.parse_args()
     main(args)
```

### Comparing `gtdb_to_taxdump-0.1.8/gtdb2td/Dmp.py` & `gtdb_to_taxdump-0.1.9/gtdb2td/Dmp.py`

 * *Files identical despite different names*

### Comparing `gtdb_to_taxdump-0.1.8/gtdb2td/Graph.py` & `gtdb_to_taxdump-0.1.9/gtdb2td/Graph.py`

 * *Files identical despite different names*

### Comparing `gtdb_to_taxdump-0.1.8/gtdb2td/IO.py` & `gtdb_to_taxdump-0.1.9/gtdb2td/IO.py`

 * *Files identical despite different names*

### Comparing `gtdb_to_taxdump-0.1.8/gtdb2td/Utils.py` & `gtdb_to_taxdump-0.1.9/gtdb2td/Utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import os
 import sys
 import gzip
 import bz2
 import argparse
 import logging
-import csv
 import urllib.request
-import codecs
 from collections import OrderedDict
 
 
 def Decode(x):
     """
     Decoding input, if needed
     """
```

### Comparing `gtdb_to_taxdump-0.1.8/setup.py` & `gtdb_to_taxdump-0.1.9/setup.py`

 * *Files identical despite different names*

