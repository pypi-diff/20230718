# Comparing `tmp/cazomevolve-0.1.6.tar.gz` & `tmp/cazomevolve-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cazomevolve-0.1.6.tar", last modified: Mon Jul 17 13:10:08 2023, max compression
+gzip compressed data, was "cazomevolve-0.1.7.tar", last modified: Tue Jul 18 16:57:15 2023, max compression
```

## Comparing `cazomevolve-0.1.6.tar` & `cazomevolve-0.1.7.tar`

### file list

```diff
@@ -1,88 +1,108 @@
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.694312 cazomevolve-0.1.6/
--rw-rw-r--   0 em        (1000) em        (1000)     1067 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/LICENSE
--rw-rw-r--   0 em        (1000) em        (1000)    42471 2023-07-17 13:10:08.694312 cazomevolve-0.1.6/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)    41706 2023-07-17 12:58:11.000000 cazomevolve-0.1.6/README.md
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.606311 cazomevolve-0.1.6/cazomevolve/
--rw-rw-r--   0 em        (1000) em        (1000)     2094 2023-07-17 11:25:18.000000 cazomevolve-0.1.6/cazomevolve/__init__.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.610311 cazomevolve-0.1.6/cazomevolve/cazome/
--rw-rw-r--   0 em        (1000) em        (1000)     1517 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/__init__.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.610311 cazomevolve-0.1.6/cazomevolve/cazome/cazy/
--rw-rw-r--   0 em        (1000) em        (1000)     1548 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/cazy/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)     7022 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/cazy/get_cazy_cazymes.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.610311 cazomevolve-0.1.6/cazomevolve/cazome/dbcan/
--rw-rw-r--   0 em        (1000) em        (1000)     1548 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/dbcan/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)     6148 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py
--rw-rw-r--   0 em        (1000) em        (1000)     4889 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/dbcan/invoke_dbcan.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.626311 cazomevolve-0.1.6/cazomevolve/cazome/explore/
--rw-rw-r--   0 em        (1000) em        (1000)     1527 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)    17139 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/cazome_sizes.py
--rw-rw-r--   0 em        (1000) em        (1000)     6409 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/cazy_classes.py
--rw-rw-r--   0 em        (1000) em        (1000)    16877 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/cazy_families.py
--rw-rw-r--   0 em        (1000) em        (1000)    19882 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/cooccurring_families.py
--rw-rw-r--   0 em        (1000) em        (1000)    20664 2023-07-17 11:37:31.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/explore_cazomes.py
--rw-rw-r--   0 em        (1000) em        (1000)     8670 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/identify_families.py
--rw-rw-r--   0 em        (1000) em        (1000)    11913 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/parse_data.py
--rw-rw-r--   0 em        (1000) em        (1000)    17627 2023-07-17 11:18:55.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/pca.py
--rw-rw-r--   0 em        (1000) em        (1000)     3181 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/plot.py
--rw-rw-r--   0 em        (1000) em        (1000)     6041 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/cazome/explore/taxonomies.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.630311 cazomevolve-0.1.6/cazomevolve/genomes/
--rw-rw-r--   0 em        (1000) em        (1000)     1540 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/genomes/__init__.py
--rwxrwxr-x   0 em        (1000) em        (1000)    11300 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/genomes/download_genomes.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.642311 cazomevolve-0.1.6/cazomevolve/scripts/
--rw-rw-r--   0 em        (1000) em        (1000)     1492 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/__init__.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.646311 cazomevolve-0.1.6/cazomevolve/scripts/bash/
--rw-rw-r--   0 em        (1000) em        (1000)     1568 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/bash/build_cazy_db.sh
--rwxrwxr-x   0 em        (1000) em        (1000)     2401 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/bash/download_acc_genomes.sh
--rw-rw-r--   0 em        (1000) em        (1000)     2078 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/build_cazy_db.py
--rw-rw-r--   0 em        (1000) em        (1000)     2462 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/cazomevolve_script.py
--rw-rw-r--   0 em        (1000) em        (1000)     3135 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/download_acc_genomes.py
--rw-rw-r--   0 em        (1000) em        (1000)     3063 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/get_fam_seqs.py
--rw-rw-r--   0 em        (1000) em        (1000)     2064 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/run_fam_blast.py
--rw-rw-r--   0 em        (1000) em        (1000)     1969 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/run_fam_diamond.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.582310 cazomevolve-0.1.6/cazomevolve/scripts/tree/
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.650311 cazomevolve-0.1.6/cazomevolve/scripts/tree/ani/
--rw-rw-r--   0 em        (1000) em        (1000)     2123 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/ani/build_anim_tree.R
--rw-rw-r--   0 em        (1000) em        (1000)     1123 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/ani/run_anim.sh
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.662311 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/
--rw-rw-r--   0 em        (1000) em        (1000)     1863 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/align_scos.sh
--rw-rw-r--   0 em        (1000) em        (1000)     1928 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/annotate_genomes.sh
--rw-rw-r--   0 em        (1000) em        (1000)     1927 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/backtranslate.sh
--rw-rw-r--   0 em        (1000) em        (1000)     6330 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/concatenate_cds.py
--rw-rw-r--   0 em        (1000) em        (1000)     5189 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/extract_cds.py
--rw-rw-r--   0 em        (1000) em        (1000)     1718 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/find_orthologues.sh
--rw-rw-r--   0 em        (1000) em        (1000)     2073 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.666312 cazomevolve-0.1.6/cazomevolve/seq_diversity/
--rwxrwxr-x   0 em        (1000) em        (1000)     1790 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/seq_diversity/get_fam_seqs.sh
--rwxrwxr-x   0 em        (1000) em        (1000)     1724 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/seq_diversity/run_blastp.sh
--rwxrwxr-x   0 em        (1000) em        (1000)     2036 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/seq_diversity/run_diamond.sh
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.670312 cazomevolve-0.1.6/cazomevolve/taxs/
--rw-rw-r--   0 em        (1000) em        (1000)     1513 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/taxs/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)    11322 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/taxs/add_taxs.py
--rw-rw-r--   0 em        (1000) em        (1000)     6982 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/taxs/ncbi.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.674312 cazomevolve-0.1.6/cazomevolve/utilities/
--rw-rw-r--   0 em        (1000) em        (1000)     1517 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/__init__.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.694312 cazomevolve-0.1.6/cazomevolve/utilities/parsers/
--rw-rw-r--   0 em        (1000) em        (1000)     1529 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/__init__.py
--rw-rw-r--   0 em        (1000) em        (1000)     4914 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/add_taxs_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     2260 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/build_cazy_db_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     3133 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/common_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     6316 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     6780 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/download_genomes_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     6493 2023-07-17 11:40:52.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/explore_cazomes_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     3477 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/extract_prot_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     4021 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/get_cazy_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     3480 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/get_dbcan_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     2899 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/get_fam_seqs_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     3724 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/invoke_dbcan_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     4446 2023-07-17 11:38:28.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/parse_cmd.py
--rw-rw-r--   0 em        (1000) em        (1000)     2257 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/run_blast_parser.py
--rw-rw-r--   0 em        (1000) em        (1000)     2372 2023-07-17 08:43:37.000000 cazomevolve-0.1.6/cazomevolve/utilities/parsers/run_diamond_parser.py
-drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-17 13:10:08.610311 cazomevolve-0.1.6/cazomevolve.egg-info/
--rw-rw-r--   0 em        (1000) em        (1000)    42471 2023-07-17 13:10:08.000000 cazomevolve-0.1.6/cazomevolve.egg-info/PKG-INFO
--rw-rw-r--   0 em        (1000) em        (1000)     2828 2023-07-17 13:10:08.000000 cazomevolve-0.1.6/cazomevolve.egg-info/SOURCES.txt
--rw-rw-r--   0 em        (1000) em        (1000)        1 2023-07-17 13:10:08.000000 cazomevolve-0.1.6/cazomevolve.egg-info/dependency_links.txt
--rw-rw-r--   0 em        (1000) em        (1000)       76 2023-07-17 13:10:08.000000 cazomevolve-0.1.6/cazomevolve.egg-info/entry_points.txt
--rw-rw-r--   0 em        (1000) em        (1000)      157 2023-07-17 13:10:08.000000 cazomevolve-0.1.6/cazomevolve.egg-info/requires.txt
--rw-rw-r--   0 em        (1000) em        (1000)       12 2023-07-17 13:10:08.000000 cazomevolve-0.1.6/cazomevolve.egg-info/top_level.txt
--rw-rw-r--   0 em        (1000) em        (1000)       38 2023-07-17 13:10:08.694312 cazomevolve-0.1.6/setup.cfg
--rw-rw-r--   0 em        (1000) em        (1000)     4141 2023-07-17 11:39:25.000000 cazomevolve-0.1.6/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.097237 cazomevolve-0.1.7/
+-rw-rw-r--   0 em        (1000) em        (1000)     1067 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/LICENSE
+-rw-rw-r--   0 em        (1000) em        (1000)    42889 2023-07-18 16:57:15.097237 cazomevolve-0.1.7/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)    42124 2023-07-18 12:14:26.000000 cazomevolve-0.1.7/README.md
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.961232 cazomevolve-0.1.7/cazomevolve/
+-rw-rw-r--   0 em        (1000) em        (1000)     2094 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/__init__.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.977233 cazomevolve-0.1.7/cazomevolve/cazome/
+-rw-rw-r--   0 em        (1000) em        (1000)     1517 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/cazome/__init__.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.981233 cazomevolve-0.1.7/cazomevolve/cazome/cazy/
+-rw-rw-r--   0 em        (1000) em        (1000)     1548 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/cazome/cazy/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)     7022 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/cazome/cazy/get_cazy_cazymes.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.989233 cazomevolve-0.1.7/cazomevolve/cazome/dbcan/
+-rw-rw-r--   0 em        (1000) em        (1000)     1548 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/cazome/dbcan/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6237 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4895 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/cazome/dbcan/invoke_dbcan.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.993233 cazomevolve-0.1.7/cazomevolve/cazome/explore/
+-rw-rw-r--   0 em        (1000) em        (1000)     1527 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)    11615 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/cazome_sizes.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6409 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/cazy_classes.py
+-rw-rw-r--   0 em        (1000) em        (1000)    17152 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/cazy_families.py
+-rw-rw-r--   0 em        (1000) em        (1000)    19985 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/cooccurring_families.py
+-rw-rw-r--   0 em        (1000) em        (1000)    20862 2023-07-18 16:28:28.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/explore_cazomes.py
+-rw-rw-r--   0 em        (1000) em        (1000)     5445 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/parse_data.py
+-rw-rw-r--   0 em        (1000) em        (1000)    17853 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/cazome/explore/pca.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.993233 cazomevolve-0.1.7/cazomevolve/genomes/
+-rw-rw-r--   0 em        (1000) em        (1000)     1540 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/genomes/__init__.py
+-rwxrwxr-x   0 em        (1000) em        (1000)    11300 2023-07-18 11:44:58.000000 cazomevolve-0.1.7/cazomevolve/genomes/download_genomes.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.997233 cazomevolve-0.1.7/cazomevolve/scripts/
+-rw-rw-r--   0 em        (1000) em        (1000)     1492 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/__init__.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.009234 cazomevolve-0.1.7/cazomevolve/scripts/bash/
+-rw-rw-r--   0 em        (1000) em        (1000)     1568 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/bash/build_cazy_db.sh
+-rwxrwxr-x   0 em        (1000) em        (1000)     2401 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/bash/download_acc_genomes.sh
+-rw-rw-r--   0 em        (1000) em        (1000)     2078 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/build_cazy_db.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2462 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/cazomevolve_script.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3135 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/download_acc_genomes.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3063 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/get_fam_seqs.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2064 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/run_fam_blast.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1969 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/run_fam_diamond.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.953232 cazomevolve-0.1.7/cazomevolve/scripts/tree/
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.013234 cazomevolve-0.1.7/cazomevolve/scripts/tree/ani/
+-rw-rw-r--   0 em        (1000) em        (1000)     2123 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/ani/build_anim_tree.R
+-rw-rw-r--   0 em        (1000) em        (1000)     1123 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/ani/run_anim.sh
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.025235 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/
+-rw-rw-r--   0 em        (1000) em        (1000)     1863 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/align_scos.sh
+-rw-rw-r--   0 em        (1000) em        (1000)     1928 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/annotate_genomes.sh
+-rw-rw-r--   0 em        (1000) em        (1000)     1927 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/backtranslate.sh
+-rw-rw-r--   0 em        (1000) em        (1000)     6330 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/concatenate_cds.py
+-rw-rw-r--   0 em        (1000) em        (1000)     5189 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/extract_cds.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1718 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/find_orthologues.sh
+-rw-rw-r--   0 em        (1000) em        (1000)     2073 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.029235 cazomevolve-0.1.7/cazomevolve/seq_diversity/
+-rw-rw-r--   0 em        (1000) em        (1000)     1489 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/__init__.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.033235 cazomevolve-0.1.7/cazomevolve/seq_diversity/explore/
+-rw-rw-r--   0 em        (1000) em        (1000)     1489 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/explore/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6473 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/explore/cazy.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6192 2023-07-18 12:12:05.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/explore/parse.py
+-rw-rw-r--   0 em        (1000) em        (1000)    11125 2023-07-17 22:21:48.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/explore/plot.py
+-rwxrwxr-x   0 em        (1000) em        (1000)     1790 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/get_fam_seqs.sh
+-rwxrwxr-x   0 em        (1000) em        (1000)     1724 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/run_blastp.sh
+-rwxrwxr-x   0 em        (1000) em        (1000)     2036 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/seq_diversity/run_diamond.sh
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.041235 cazomevolve-0.1.7/cazomevolve/taxs/
+-rw-rw-r--   0 em        (1000) em        (1000)     1513 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/taxs/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)    11322 2023-07-17 20:40:22.000000 cazomevolve-0.1.7/cazomevolve/taxs/add_taxs.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6971 2023-07-18 12:11:27.000000 cazomevolve-0.1.7/cazomevolve/taxs/ncbi.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.045235 cazomevolve-0.1.7/cazomevolve/utilities/
+-rw-rw-r--   0 em        (1000) em        (1000)     1517 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/__init__.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.073236 cazomevolve-0.1.7/cazomevolve/utilities/parsers/
+-rw-rw-r--   0 em        (1000) em        (1000)     1529 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/__init__.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4914 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/add_taxs_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2260 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/build_cazy_db_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6316 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6780 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/download_genomes_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     6687 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/explore_cazomes_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4021 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/get_cazy_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3480 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/get_dbcan_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2899 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/get_fam_seqs_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3724 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/invoke_dbcan_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4427 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/parse_cmd.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2257 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/run_blast_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2372 2023-07-17 08:43:37.000000 cazomevolve-0.1.7/cazomevolve/utilities/parsers/run_diamond_parser.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:14.973233 cazomevolve-0.1.7/cazomevolve.egg-info/
+-rw-rw-r--   0 em        (1000) em        (1000)    42889 2023-07-18 16:57:14.000000 cazomevolve-0.1.7/cazomevolve.egg-info/PKG-INFO
+-rw-rw-r--   0 em        (1000) em        (1000)     3318 2023-07-18 16:57:14.000000 cazomevolve-0.1.7/cazomevolve.egg-info/SOURCES.txt
+-rw-rw-r--   0 em        (1000) em        (1000)        1 2023-07-18 16:57:14.000000 cazomevolve-0.1.7/cazomevolve.egg-info/dependency_links.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       76 2023-07-18 16:57:14.000000 cazomevolve-0.1.7/cazomevolve.egg-info/entry_points.txt
+-rw-rw-r--   0 em        (1000) em        (1000)      161 2023-07-18 16:57:14.000000 cazomevolve-0.1.7/cazomevolve.egg-info/requires.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       12 2023-07-18 16:57:14.000000 cazomevolve-0.1.7/cazomevolve.egg-info/top_level.txt
+-rw-rw-r--   0 em        (1000) em        (1000)       38 2023-07-18 16:57:15.097237 cazomevolve-0.1.7/setup.cfg
+-rw-rw-r--   0 em        (1000) em        (1000)     4157 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/setup.py
+drwxrwxr-x   0 em        (1000) em        (1000)        0 2023-07-18 16:57:15.093237 cazomevolve-0.1.7/tests/
+-rw-rw-r--   0 em        (1000) em        (1000)     5804 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_add_taxs.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1958 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_cazomevolve.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2585 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_explore_cazome_sizes.py
+-rw-rw-r--   0 em        (1000) em        (1000)    13133 2023-07-18 16:36:56.000000 cazomevolve-0.1.7/tests/test_explore_cazomes.py
+-rw-rw-r--   0 em        (1000) em        (1000)     1830 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_explore_classes.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2741 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_explore_cooccurring_families.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3625 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_explore_families.py
+-rw-rw-r--   0 em        (1000) em        (1000)     2562 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_explore_parse_data.py
+-rw-rw-r--   0 em        (1000) em        (1000)     5653 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_explore_pca.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4216 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_explore_upsetplot.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3373 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_genome_download.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4114 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_get_cazy.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3744 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_get_dbcan.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4157 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_invoke_dbcan.py
+-rw-rw-r--   0 em        (1000) em        (1000)     3712 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_ncbi.py
+-rw-rw-r--   0 em        (1000) em        (1000)     8722 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_parser.py
+-rw-rw-r--   0 em        (1000) em        (1000)     5843 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_scripts.py
+-rw-rw-r--   0 em        (1000) em        (1000)     4569 2023-07-18 12:06:27.000000 cazomevolve-0.1.7/tests/test_seq_diversity.py
```

### Comparing `cazomevolve-0.1.6/LICENSE` & `cazomevolve-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/PKG-INFO` & `cazomevolve-0.1.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,34 +1,14 @@
-Metadata-Version: 2.1
-Name: cazomevolve
-Version: 0.1.6
-Summary: A bioinforamtic package for investigating the evolution of CAZomes
-Author: Emma E. M. Hobbs
-Author-email: eemh1@st-andrews.ac.uk
-License: MIT
-Keywords: bioinforamtics protein
-Platform: Posix
-Platform: MacOS X
-Classifier: Development Status :: 3 - Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # cazomevolve
 
 [![DOI](https://zenodo.org/badge/367898306.svg)](https://zenodo.org/badge/latestdoi/367898306)
 [![Documentation Status](https://readthedocs.org/projects/cazomevolve/badge/?version=latest)](https://cazomevolve.readthedocs.io/en/latest/?badge=latest)
 [![licence](https://img.shields.io/badge/Licence-MIT-green)](https://github.com/HobnobMancer/cazomevolve/blob/master/LICENSE)  
+[![CircleCI](https://circleci.com/gh/HobnobMancer/cazomevolve.svg?style=shield)](https://circleci.com/gh/HobnobMancer/cazomevolve)
+[![codecov](https://codecov.io/gh/HobnobMancer/cazomevolve/branch/master/graph/badge.svg)](https://codecov.io/gh/HobnobMancer/cazomevolve)  
 ![Python](https://img.shields.io/badge/Python-v3.9.---orange)
 ![Research](https://img.shields.io/badge/Research-Bioinformatics-ff69b4)
 [![Funding BBSCR](https://img.shields.io/badge/Funding-EASTBio-blue)](http://www.eastscotbiodtp.ac.uk/)
 [![cazomevolve PyPi version](https://img.shields.io/pypi/v/cazomevolve "PyPI version")](https://pypi.python.org/pypi/cazomevolve)  
 [![Downloads](https://pepy.tech/badge/cazomevolve)](https://pepy.tech/project/cazomevolve)
 
 `cazomevolve` ('cazome-evolve') is an application and Python3 package for the automated annotation and exploratory analysis of CAZyme complements (CAZomes) for a set of species and/or genomes of interest. Carbohydrate Active enZymes are a subset of proteins that generate, modify and/or degrade carbohydrates. CAZy (www.cazy.org) is the most comprehensive CAZyme database, grouping proteins by sequence similarity into CAZy families.
@@ -82,15 +62,15 @@
 > Kozlov AM, Darriba D, Flouri T, Morel B, Stamatakis A. RAxML-NG: a fast, scalable and user-friendly tool for maximum likelihood phylogenetic inference. Bioinformatics. 2019 Nov 1;35(21):4453-4455. doi: 10.1093/bioinformatics/btz305.
 > Whelan FJ, Rusilowicz M, McInerney JO. Coinfinder: detecting significant associations and dissociations in pangenomes. Microb Genom. 2020 Mar;6(3):e000338. doi: 10.1099/mgen.0.000338. Epub 2020 Feb 24.
 
 ## Documentation
 
 `cazomevolve` uses bash-script based workflow management. A summary of this workflow is provided in this README.
 
-Please see the [full documeentation including tutorials at ReadTheDocs]().
+Please see the [full documeentation including tutorials at ReadTheDocs](https://cazomevolve.readthedocs.io/en/latest/?badge=latest).
 
 An analysis using `cazomevolve` can be found [here](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto), which includes a README-walkthrough and all output files.
 
 ## Contents
 
 1. [cazomevolve](#cazomevolve)
 2. [Documentation](#documentation)
@@ -666,14 +646,15 @@
   results/ \
   --genus \
   --species
 ```
 
 ### Optional
 
+* `--show_plots` - Display plots generated as the program is executing (default: False)
 * `--round_by` - ROUND_BY - Number of decimal places to round means and SDs to (default: 2)
 * `-f`, `--force` - Force file over writting (default: False)
 * `-l`, `--log` log file name - Defines log file name and/or path (default: None)
 * `-n`, `--nodelete` - enable/disable deletion of exisiting files (default: False)
 * `-v`, `--verbose` - Set logger level to 'INFO' (default: False)
 
 ## Full customisation of CAZome exploration
```

### Comparing `cazomevolve-0.1.6/README.md` & `cazomevolve-0.1.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,36 @@
+Metadata-Version: 2.1
+Name: cazomevolve
+Version: 0.1.7
+Summary: A bioinforamtic package for investigating the evolution of CAZomes
+Author: Emma E. M. Hobbs
+Author-email: eemh1@st-andrews.ac.uk
+License: MIT
+Keywords: bioinforamtics protein
+Platform: Posix
+Platform: MacOS X
+Classifier: Development Status :: 3 - Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # cazomevolve
 
 [![DOI](https://zenodo.org/badge/367898306.svg)](https://zenodo.org/badge/latestdoi/367898306)
 [![Documentation Status](https://readthedocs.org/projects/cazomevolve/badge/?version=latest)](https://cazomevolve.readthedocs.io/en/latest/?badge=latest)
 [![licence](https://img.shields.io/badge/Licence-MIT-green)](https://github.com/HobnobMancer/cazomevolve/blob/master/LICENSE)  
+[![CircleCI](https://circleci.com/gh/HobnobMancer/cazomevolve.svg?style=shield)](https://circleci.com/gh/HobnobMancer/cazomevolve)
+[![codecov](https://codecov.io/gh/HobnobMancer/cazomevolve/branch/master/graph/badge.svg)](https://codecov.io/gh/HobnobMancer/cazomevolve)  
 ![Python](https://img.shields.io/badge/Python-v3.9.---orange)
 ![Research](https://img.shields.io/badge/Research-Bioinformatics-ff69b4)
 [![Funding BBSCR](https://img.shields.io/badge/Funding-EASTBio-blue)](http://www.eastscotbiodtp.ac.uk/)
 [![cazomevolve PyPi version](https://img.shields.io/pypi/v/cazomevolve "PyPI version")](https://pypi.python.org/pypi/cazomevolve)  
 [![Downloads](https://pepy.tech/badge/cazomevolve)](https://pepy.tech/project/cazomevolve)
 
 `cazomevolve` ('cazome-evolve') is an application and Python3 package for the automated annotation and exploratory analysis of CAZyme complements (CAZomes) for a set of species and/or genomes of interest. Carbohydrate Active enZymes are a subset of proteins that generate, modify and/or degrade carbohydrates. CAZy (www.cazy.org) is the most comprehensive CAZyme database, grouping proteins by sequence similarity into CAZy families.
@@ -60,15 +84,15 @@
 > Kozlov AM, Darriba D, Flouri T, Morel B, Stamatakis A. RAxML-NG: a fast, scalable and user-friendly tool for maximum likelihood phylogenetic inference. Bioinformatics. 2019 Nov 1;35(21):4453-4455. doi: 10.1093/bioinformatics/btz305.
 > Whelan FJ, Rusilowicz M, McInerney JO. Coinfinder: detecting significant associations and dissociations in pangenomes. Microb Genom. 2020 Mar;6(3):e000338. doi: 10.1099/mgen.0.000338. Epub 2020 Feb 24.
 
 ## Documentation
 
 `cazomevolve` uses bash-script based workflow management. A summary of this workflow is provided in this README.
 
-Please see the [full documeentation including tutorials at ReadTheDocs]().
+Please see the [full documeentation including tutorials at ReadTheDocs](https://cazomevolve.readthedocs.io/en/latest/?badge=latest).
 
 An analysis using `cazomevolve` can be found [here](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto), which includes a README-walkthrough and all output files.
 
 ## Contents
 
 1. [cazomevolve](#cazomevolve)
 2. [Documentation](#documentation)
@@ -644,14 +668,15 @@
   results/ \
   --genus \
   --species
 ```
 
 ### Optional
 
+* `--show_plots` - Display plots generated as the program is executing (default: False)
 * `--round_by` - ROUND_BY - Number of decimal places to round means and SDs to (default: 2)
 * `-f`, `--force` - Force file over writting (default: False)
 * `-l`, `--log` log file name - Defines log file name and/or path (default: None)
 * `-n`, `--nodelete` - enable/disable deletion of exisiting files (default: False)
 * `-v`, `--verbose` - Set logger level to 'INFO' (default: False)
 
 ## Full customisation of CAZome exploration
```

### Comparing `cazomevolve-0.1.6/cazomevolve/__init__.py` & `cazomevolve-0.1.7/cazomevolve/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,15 +39,15 @@
 # SOFTWARE.
 """Bioinforamtic package for exploring the evolution of CAZomes"""
 
 
 import logging
 
 
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 
 __citation__ = "???"
 
 
 def closing_message(job, args):
     """Write closing messsage to terminal
```

### Comparing `cazomevolve-0.1.6/cazomevolve/cazome/__init__.py` & `cazomevolve-0.1.7/cazomevolve/cazome/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/cazome/cazy/__init__.py` & `cazomevolve-0.1.7/cazomevolve/cazome/cazy/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/cazome/cazy/get_cazy_cazymes.py` & `cazomevolve-0.1.7/cazomevolve/cazome/cazy/get_cazy_cazymes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/cazome/dbcan/__init__.py` & `cazomevolve-0.1.7/cazomevolve/cazome/dbcan/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py` & `cazomevolve-0.1.7/cazomevolve/cazome/dbcan/get_dbcan_cazymes.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,14 +134,15 @@
 
 def get_tool_fams(tool_data):
     """Get predicted CAZy family annotations for a specific tool
     
     :param tool_data: str, output from prediction tool
     
     Return set of CAZy family predictions"""
+    print(tool_data, '***')
     if tool_data == "-":
         return set()
     
     predicted_domains = tool_data.split("+")  # each predicted domain is separated b "+"
 
     fams = set()
 
@@ -158,16 +159,17 @@
 
     Hotpep == eCAMI - does not matter which verion of the dbCAN was used
     
     :param hmmer_fams: set of CAZy family annotations
     :param hotpep_fams: set of CAZy family annotations
     :param diamond_fams: set of CAZy family annotations
     
-    Return set
+    Return LIST
     """
+    print(hmmer_fams, hotpep_fams, diamond_fams, 'RESULTS')
     hmmer_hotpep = hmmer_fams & hotpep_fams
     hmmer_diamond = hmmer_fams & diamond_fams
     hotpep_diamond = hotpep_fams & diamond_fams
     all_tools = hmmer_fams & diamond_fams & hotpep_fams
 
     dbcan_consensus = list(all_tools.union(hmmer_hotpep, hmmer_diamond, hotpep_diamond))
```

### Comparing `cazomevolve-0.1.6/cazomevolve/cazome/dbcan/invoke_dbcan.py` & `cazomevolve-0.1.7/cazomevolve/cazome/dbcan/invoke_dbcan.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # (c) University of Strathclyde 2022
 # (c) James Hutton Institute 2022
 # Author:
 # Emma E. M. Hobbs
 
 # Contact
 # eemh1@st-andrews.ac.uk
-
+#
 # Emma E. M. Hobbs,
 # Biomolecular Sciences Building,
 # University of St Andrews,
 # North Haugh Campus,
 # St Andrews,
 # KY16 9ST
 # Scotland,
@@ -44,24 +44,24 @@
 import subprocess
 import logging
 
 from tqdm import tqdm
 from typing import List, Optional
 
 from saintBioutils.utilities.file_io import make_output_directory
-from saintBioutils.utilities.file_io import get_paths
+from saintBioutils.utilities.file_io.get_paths import get_file_paths
 
 from cazomevolve import closing_message
 
 
 def main(args: Optional[List[str]] = None, logger: Optional[logging.Logger] = None):
     make_output_directory(args.output_dir, args.force, args.nodelete)
 
     # get the path to every FASTA to be parsed by dbCAN
-    fasta_files_paths = list(set(get_paths.get_file_paths(args.input_dir, suffixes=['fasta', 'faa'])))
+    fasta_files_paths = list(set(get_file_paths(args.input_dir, suffixes=['fasta', 'faa'])))
     fasta_files_paths.sort()
     print(f"Retrieved {len(fasta_files_paths)} fasta files from {args.input_dir}")
 
     for fasta_path in tqdm(fasta_files_paths, desc="Running dbCAN"):
         # define path to output dir that will house output for this specific input FASTA file
         # extract genomic accession from the file name, and name output dir after the accession
         try:
```

### Comparing `cazomevolve-0.1.6/cazomevolve/cazome/explore/__init__.py` & `cazomevolve-0.1.7/cazomevolve/cazome/explore/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/cazome/explore/cazome_sizes.py` & `cazomevolve-0.1.7/cazomevolve/cazome/explore/cazome_sizes.py`

 * *Files 20% similar despite different names*

```diff
@@ -290,166 +290,7 @@
         new_row = [grp_name, mean_ratio, sd_ratio, num_genomes]
         cazyme_ratio_data.append(new_row)
     
     cols = [grp, 'MeanCAZymeToFamRatio', 'SdCAZymeToFamRatio', 'NumOfGenomes']
     cazome_ratio_df = pd.DataFrame(cazyme_ratio_data, columns=cols)
     
     return cazome_sizes, cazome_ratio_df
-
-
-#
-##
-#
-
-
-def get_cazome_size_df(cazomes_sizes, group_by):
-    """Build a df with the mean and SD number of CAZymes per group
-    
-    :param cazome_sizes: dict, {genome: {'CAZymes': int, 'proteins': int}}
-    :param group: str, 'genus' or 'species'
-    
-    Return pandas df
-    """
-    tax_cazome_sizes = {}  # {group: [num of cazymes]}
-
-    for genome in tqdm(cazome_sizes, desc=f"Getting num of CAZymes per {group_by}"):
-        group = gtdb_tax_dict[genome][group_by]
-        try:
-            num_of_cazymes = cazome_sizes[genome]['CAZymes']
-        except KeyError:
-            continue  # do not have any CAZome info for the genome
-
-        try:
-            tax_cazome_sizes[group].append(num_of_cazymes)
-        except KeyError:
-            tax_cazome_sizes[group] = [num_of_cazymes]
-
-    cazome_size_data = []
-    for group in tax_cazome_sizes:
-        group_name = group.strip()
-        group_name = f"{group_name[0].upper()}{group_name[1:]}"
-        mean_size = round(np.mean(tax_cazome_sizes[group]), 2)
-        sd_size = round(np.std(tax_cazome_sizes[group]), 2)
-        num_of_genomes = len(tax_cazome_sizes[group])
-        cazome_size_data.append([group_name, mean_size, sd_size, num_of_genomes])
-
-    column_names = ['Group', 'Mean number of CAZymes', 'SD', 'Number of genomes']
-
-    cazome_size_df = pd.DataFrame(cazome_size_data, columns=column_names)
-
-    return cazome_size_df
-
-
-def get_proteome_size(proteome_dir, cazome_sizes):
-    """Retrieve the number of proteins per proteomoe FASTA file and add the values to the cazome_sizes dict
-    
-    :param proteome_dir: Path, dir containing protein FASTA files
-    :param cazome_sizes: dict, {genome: {'CAZymes': int, 'proteins': int}}
-    
-    Return cazome_sizes with added proteome sizes
-    """
-    proteome_paths = get_file_paths(proteome_dir, suffixes=[".faa", '.fasta'])
-    print(f"Found {len(proteome_paths)} in the proteome dir")
-
-    # cazomesize = {genome: {'CAZymes': int, 'proteins': int}
-
-    for proteome_path in tqdm(proteome_paths, desc="Getting proteome sizes"):
-        genome = f"{proteome_path.name.split('_')[0]}_{proteome_path.name.split('_')[1]}"
-        protein_count = 0
-
-        for record in SeqIO.parse(proteome_path, 'fasta'):
-            protein_count += 1
-
-        try:
-            cazome_sizes[genome]
-        except KeyError:
-            cazome_sizes[genome] = {}
-
-        cazome_sizes[genome]['proteins'] = protein_count
-    
-    return cazome_sizes
-
-
-def get_cazome_proportion_df(cazome_sizes, group_by):
-    """Build a df with the mean and SD proportion of the proteomoe in the CAZome
-    
-    :param cazome_sizes: dict, {genome: {'CAZymes': int, 'proteins': int}}
-    :param group: str, 'genus' or 'species'
-    
-    Return pandas df
-    """
-    tax_cazome_proportion = {}  # {group: [percentage of proteome]}
-
-    for genome in tqdm(cazome_sizes, desc=f"Getting CAZome proporitions per {group_by}"):
-        group = gtdb_tax_dict[genome][group_by]
-        try:
-            num_of_cazymes = cazome_sizes[genome]['CAZymes']
-        except KeyError:
-            continue  # do not have any CAZome info for the genome
-
-        try:
-            num_of_proteins = cazome_sizes[genome]['proteins']
-        except KeyError:
-            continue  # do not have any proteome info for the genome
-            
-        cazome_proportion = (num_of_cazymes / num_of_proteins) * 100
-        
-        try:
-            tax_cazome_proportion[group].append(cazome_proportion)
-        except KeyError:
-            tax_cazome_proportion[group] = [cazome_proportion]
-
-    cazome_proportion_data = []
-    for group in tax_cazome_proportion:
-        group_name = group.strip()
-        group_name = f"{group_name[0].upper()}{group_name[1:]}"
-        mean_size = round(np.mean(tax_cazome_proportion[group]), 2)
-        sd_size = round(np.std(tax_cazome_proportion[group]), 2)
-        num_of_genomes = len(tax_cazome_proportion[group])
-        cazome_proportion_data.append([group_name, mean_size, sd_size, num_of_genomes])
-
-    column_names = ['Group', 'Mean perc of proteome in the CAZome', 'SD', 'Number of genomes']
-
-    cazome_proportion_df = pd.DataFrame(cazome_proportion_data, columns=column_names)
-
-    return cazome_proportion_df
-
-
-def get_num_of_fams_per_group(fam_freq_df, group_by):
-    """Retrieve the mean and SD of the number of fams per group
-    
-    :param fam_freq_df: df, rows=genome, cols=fam freqs
-    :param group_by: str, 'genus' or 'species'
-    
-    Return df: group, mean num of fams, SD
-    """
-    num_of_fams = {} # {group: [num of fams per genome]}
-
-    if group_by == 'genus':
-        group_num = 1
-    else:
-        group_num = 2
-
-    for ri in tqdm(range(len(fam_freq_df)), desc="Getting num of fams per genome"):
-        fams_count = 0
-        for fam in fam_freq_df.columns:
-            if fam_freq_df.iloc[ri][fam] > 0:
-                fams_count += 1
-
-        group = fam_freq_df.iloc[ri].name[group_num].strip()
-        group = f"{group[0].upper()}{group[1:]}"
-
-        try:
-            num_of_fams[group].append(fams_count)
-        except KeyError:
-            num_of_fams[group] = [fams_count]
-
-    fam_count_data = []
-    for group in num_of_fams:
-        fam_mean = round(np.mean(num_of_fams[group]), 2)
-        fam_std = round(np.std(num_of_fams[group]), 2)
-        fam_count_data.append([group, fam_mean, fam_std])
-
-    group_by = f"{group_by[0].upper()}{group_by[1:]}"
-    fam_count_df = pd.DataFrame(fam_count_data, columns=[group_by, 'Mean num of families', 'SD'])
-    
-    return fam_count_df
```

### Comparing `cazomevolve-0.1.6/cazomevolve/cazome/explore/cazy_classes.py` & `cazomevolve-0.1.7/cazomevolve/cazome/explore/cazy_classes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/cazome/explore/cazy_families.py` & `cazomevolve-0.1.7/cazomevolve/cazome/explore/cazy_families.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,22 +136,23 @@
     df,
     row_colours=None,
     fig_size=None,
     file_path=None,
     file_format='png',
     font_scale=1,
     dpi=300,
-    dendrogram_ratio=None,
+    dendrogram_ratio=0.2,
     lut=None,
     legend_title='',
     title_fontsize='2',
     legend_fontsize='2',
     bbox_to_anchor=(1,1),
     cmap=sns.cubehelix_palette(dark=1, light=0, reverse=True, as_cmap=True),
     cbar_pos=(0.02, 0.8, 0.05, 0.18),
+    show=False,
 ):
     """Build a clustermap of the CAZy family frequencies per genome
     
     :param df: df of CAZy family frequencies per genome
     :param row_colours: pandas map - used to define additional row colours. or list of maps for 
         multiple sets of row colours. If None, additional row colours are not plotted
     :param fig_size: tuple (width, height) of final figure. If None, decided by Seaborn
@@ -195,20 +196,24 @@
             title=legend_title,
             bbox_to_anchor=bbox_to_anchor,
             bbox_transform=plt.gcf().transFigure,
             loc='upper center',
             title_fontsize=title_fontsize,
             fontsize=legend_fontsize,
         )
-        
+    
+    if show:
+        plt.show();
+
     if file_path is not None:
         fam_clustermap.savefig(
             file_path,
             dpi=dpi,
             bbox_inches='tight',
+            format=file_format,
         )
 
     return fam_clustermap
 
 
 def build_family_clustermap_multi_legend(
     df,
@@ -218,15 +223,15 @@
     bbox_to_anchors,
     legend_cols=None,
     fig_size=None,
     file_path=None,
     file_format='png',
     font_scale=1,
     dpi=300,
-    dendrogram_ratio=None,
+    dendrogram_ratio=0.2,
     title_fontsize=2,
     legend_fontsize=2,
     cmap=sns.cubehelix_palette(dark=1, light=0, reverse=True, as_cmap=True),
     cbar_pos=(0.02, 0.8, 0.05, 0.18),
 ):
     """Build a clustermap of the CAZy family frequencies per genome
     
@@ -310,14 +315,15 @@
             )
         
     if file_path is not None:
         fam_clustermap.savefig(
             file_path,
             dpi=dpi,
             bbox_inches='tight',
+            format=file_format,
         )
 
     return fam_clustermap
 
 
 ## For the core CAZome
 
@@ -367,22 +373,23 @@
     for i in range(len(df)):
         row = df.iloc[i]
         for fam in df.columns:
             row_data = [fam, row[fam]]
             long_form_data.append(row_data)
     
     long_form_df = pd.DataFrame(long_form_data, columns=["Family", "Frequency"])
-    
+
     boxplot = sns.boxplot(x=long_form_df['Family'], y=long_form_df['Frequency'])
     
     if file_path is not None:
         boxplot.savefig(
             file_path,
             dpi=dpi,
             bbox_inches='tight',
+            format=file_format,
         )
 
 
 def build_fam_mean_freq_df(df, grp, round_by=None):
     """Build two dataframes of fam frequencies from a wide fam freq df
     
     DF 1: Family, tax rank (i.e. group), genome, freq
@@ -458,14 +465,16 @@
 
         try:
             group_fams[group]
         except KeyError:
             group_fams[group] = set()
 
         for fam in all_families:
+            if fam in ['Kingdom', 'Phylum', 'Class', 'Order', 'Family', 'Genus', 'Species', 'Genome', 'Genomes']:
+                continue
             if fam_freq_df.iloc[ri][fam] > 0:
                 group_fams[group].add(fam)
 
     # identify fams found in only one group
     unique_grp_fams = {}  # {grp: {fams}}
     for group in tqdm(group_fams, desc=f"Identifying {group_by} specific fams"):
         fams_in_grp = group_fams[group]
```

### Comparing `cazomevolve-0.1.6/cazomevolve/cazome/explore/cooccurring_families.py` & `cazomevolve-0.1.7/cazomevolve/cazome/explore/cooccurring_families.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,15 +126,15 @@
 
 
 # 
 # mannually parsing the df to identify co-occuring families
 # including the number of genomes containing each group of CAZy families - needed for an upset plot
 #
 
-def calc_cooccuring_fam_freqs(df, all_families, exclude_core_cazome=False):
+def calc_cooccuring_fam_freqs(df, all_families, exclude_core_cazome=False, core_cazome=[]):
     """Identify groups of CAZy families that are always present together, and count in 
     how many genomes the families are present together
     
     Initially calls another function to identify pairs of CAZy families that are always
     present together.
     
     Then identifies overlapping pairs of co-occurring CAZy families to identify grps 
@@ -143,14 +143,15 @@
     be present together because both are always present with fam1.
     
     :param df: fam freq df, pandas df, columns are CAZy families, rows are genomes, cells 
         contain CAZy fam frequency
     :param all_families: set of all CAZy families to be analysed
     :param exclude_core_cazome: whether to exlude the core cazome, default: False - 
         include the core CAZome
+    :param core_cazome: list of core CAZome families if to be excluded
         
     Return dict {grp_num: {'fams': {co-occurring fams}, 'freqs': {num of genomes}}
     - returns set of frequencies in case different numbers are produced for each inital pair 
     of co-occurring families
     """
     cooccuring_fams_dict = identify_cooccurring_fam_pairs(df, all_families, exclude_core_cazome=exclude_core_cazome)
     
@@ -184,15 +185,15 @@
     for grp in cooccurring_groups:
         if len(cooccurring_groups[grp]['freqs']) > 1:
             print(f':WARNING: differing freqs found for grp: {cooccurring_groups[grp]}')
     
     return cooccurring_groups
     
     
-def identify_cooccurring_fam_pairs(df, all_families, exclude_core_cazome=False):
+def identify_cooccurring_fam_pairs(df, all_families, exclude_core_cazome=False, core_cazome=[]):
     """Identify pairs of CAZy families that are always present together in the same genome
     
     :param df: fam freq df, pandas df, columns are CAZy families, rows are genomes, cells 
         contain CAZy fam frequency
     :param all_families: set of all CAZy families to be analysed
     :param exclude_core_cazome: whether to exlude the core cazome, default: False - 
         include the core CAZome
```

### Comparing `cazomevolve-0.1.6/cazomevolve/cazome/explore/explore_cazomes.py` & `cazomevolve-0.1.7/cazomevolve/cazome/explore/explore_cazomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -306,44 +306,45 @@
         index.append('Kingdom')
     if args.phylum:
         index.append('Phylum')
     if args.tax_class:
         index.append('Class')
     if args.tax_order:
         index.append('Order')
-    if args.tax_family_:
+    if args.tax_family:
         index.append('Family')
     if args.genus:
         index.append('Genus')
     if args.species:
         index.append('Species')
 
     fam_freq_df_ggs = fam_freq_df_ggs.set_index(index)
     # define a colour scheme to colour code rows by genus
     fam_freq_df_ggs[args.group_by] = list(fam_freq_df[args.group_by])  # add column to use for colour scheme, is removed
     fam_freq_genus_row_colours, fam_g_lut = build_row_colours(fam_freq_df_ggs, args.group_by, 'Set2')
 
     for file_format in args.formats:
-        outpath_cm = outdir / f"cazy_family_clustermap.{args.file_format}"
+        outpath_cm = outdir / f"cazy_family_clustermap.{file_format}"
         logger.warning(
             f"Writing out clustermap of CAZy family frequencies in {file_format} format to:\n"
             f"{outpath_cm}"
         )
         build_family_clustermap(
             fam_freq_df_ggs,
             row_colours=fam_freq_genus_row_colours,
-            fig_size=((len(fam_freq_df_ggs).columns)*0.4, len(fam_freq_df_ggs)*0.4),
+            fig_size=(len(fam_freq_df_ggs.columns)*0.4, len(fam_freq_df_ggs)*0.4),
             file_path=outpath_cm,
             file_format=format,
             lut=fam_g_lut,
             legend_title=args.group_by,
             dendrogram_ratio=(0.2, 0.05),
             title_fontsize=28,
             legend_fontsize=24,
             cbar_pos=(0, 0.95, 0.05, 0.05),
+            show=args.show_plots,
         )
 
     # find group specific families
     outpath_dic = outdir / f"{args.group_by}_specific_cazy_families.json"
     all_families = list(fam_freq_df.columns)[3:]
     unique_grp_fams, group_fams = get_group_specific_fams(fam_freq_df, args.group_by, all_families)
     for grp in unique_grp_fams:
@@ -373,15 +374,15 @@
         index.append('Kingdom')
     if args.phylum:
         index.append('Phylum')
     if args.tax_class:
         index.append('Class')
     if args.tax_order:
         index.append('Order')
-    if args.tax_family_:
+    if args.tax_family:
         index.append('Family')
     if args.genus:
         index.append('Genus')
     if args.species:
         index.append('Species')
 
     try:
@@ -432,27 +433,27 @@
 
     cooccurring_fams_dict = calc_cooccuring_fam_freqs(
         fam_freq_df,
         list(all_families),
         exclude_core_cazome=False,
     )
     with open(outpath_all, "w") as fh:
-        fh.write(cooccurring_fams_dict)
+        fh.write(str(cooccurring_fams_dict))
 
     grp_cooccuring_fams = {}  # {genus: cooccurring_fams_d
     for grp in set(fam_freq_df[args.group_by]):
         grp_fam_freq_df = fam_freq_df[fam_freq_df[args.group_by] == grp]
         grp_cooccurring_fams_dict = calc_cooccuring_fam_freqs(
             grp_fam_freq_df,
             list(all_families),
             exclude_core_cazome=False,
         )
         grp_cooccuring_fams[grp] = grp_cooccurring_fams_dict
     with open(outpath_grp, "w") as fh:
-        fh.write(grp_cooccuring_fams)
+        fh.write(str(grp_cooccuring_fams))
 
     upsetplot_membership = []
     upsetplot_membership = add_to_upsetplot_membership(upsetplot_membership, cooccurring_fams_dict)
 
     for genus in grp_cooccuring_fams:
         upsetplot_membership = add_to_upsetplot_membership(
             upsetplot_membership,
@@ -468,15 +469,15 @@
         build_upsetplot(
             upsetplot_membership,
             file_path=upset_path,
         )
 
     # calculate frequencies
     upset_plot_groups = get_upsetplot_grps(upsetplot_membership)
-
+    cooccurring_grp_freq_data = []
     cooccurring_grp_freq_data = add_upsetplot_grp_freqs(
         upset_plot_groups,
         cooccurring_grp_freq_data,
         grp_cooccuring_fams,
         args.group_by,
         grp_sep=True,
         include_none=True,
@@ -506,15 +507,15 @@
         index.append('Kingdom')
     if args.phylum:
         index.append('Phylum')
     if args.tax_class:
         index.append('Class')
     if args.tax_order:
         index.append('Order')
-    if args.tax_family_:
+    if args.tax_family:
         index.append('Family')
     if args.genus:
         index.append('Genus')
     if args.species:
         index.append('Species')
 
     for col in index:
@@ -542,26 +543,28 @@
             f"{out_cumvar}"
         ) 
         cumExpVar = plot_explained_variance(
             pca,
             num_of_components,
             file_path=out_cumvar,
             file_format=file_format,
+            show=args.show_plots,
         )
 
         out_scree = outdir / f"pca_scree_plot.{file_format}"
         logger.warning(
             f"Writing out scree plot from the PCA in {file_format} to \n:"
             f"{out_scree}"
         )
         plot_scree(
             pca,
             nComp=10,
             file_format=file_format,
             file_path=out_scree,
+            show=args.show_plots,
         )
 
     # plot PCS 1-4
     plot_pcs((1,2), fam_freq_df_ggs, pca, X_scaled, outdir, args)
     plot_pcs((1,3), fam_freq_df_ggs, pca, X_scaled, outdir, args)
     plot_pcs((1,4), fam_freq_df_ggs, pca, X_scaled, outdir, args)
     plot_pcs((2,3), fam_freq_df_ggs, pca, X_scaled, outdir, args)
@@ -589,26 +592,28 @@
             pca,
             X_scaled,
             fam_freq_df_ggs,
             pc_pair[0],
             pc_pair[1],
             args.group_by,
             style=args.group_by,
-            fig_size=(15,15),
+            figsize=(15,15),
             file_path=out,
             file_format=file_format,
+            show=args.show_plots,
         );
 
     logger.warning(f"PC{pc_pair[0]} vs PC{pc_pair[1]} - plotting loadings plot")
     for file_format in args.formats:
         out = pc_outdir / f'pca_pc{pc_pair[0]}_vs_pc{pc_pair[1]}-{args.group_by}-loadings.{file_format}'
-        g = plot_loadings(
+        plot_loadings(
             pca,
             fam_freq_df_ggs,
             pc_pair[0],
             pc_pair[1],
             threshold=0.3,
-            fig_size=(10,10),
+            figsize=(10,10),
             file_path=out,
             font_size=11,
             file_format=file_format,
+            show=args.show_plots,
         );
```

### Comparing `cazomevolve-0.1.6/cazomevolve/cazome/explore/pca.py` & `cazomevolve-0.1.7/cazomevolve/cazome/explore/pca.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,15 @@
     pca,
     nComp,
     threshold=0.95,
     figsize=(10, 5),
     file_path=None,
     file_format='png',
     dpi=300,
+    show=False,
 ):
     """Plot the cumlative explained variance.
     
     :param pca: sklearn pca object
     :param nComp: int, number of PCs
     :param threshold: int (float), calc the number of PCs needed to capture this degree of the variance 
         in the dataset
@@ -102,28 +103,29 @@
     )
 
     fig = plt.figure(figsize=figsize)
     im = plt.plot( range(nComp), cumExpVar )
     plt.xticks(np.arange(0,nComp,5));
     plt.xlabel( 'Number of PCs', fontsize=14);
     plt.ylabel('Cumulative explained variance', fontsize=14);
-    plt.show;
+    if show:
+        plt.show()
 
     if file_path is not None:
         plt.savefig(
             file_path,
             bbox_inches='tight',
             format=file_format,
             dpi=dpi,
         )
 
     return cumExpVar
     
     
-def plot_scree(pca, nComp=10, file_path=None, file_format='png', dpi=300):
+def plot_scree(pca, nComp=10, file_path=None, file_format='png', dpi=300, show=False):
     """Generate scree plot for PCA, plotting the amount of variance captured by each pc, for the
     first nComp PCs
     
     :param pca: sklearn pca object
     :param nComp: int, number of PCs to plot
     :param file_path: str/Path, path to write out figure. If none, image is not written to a file
     :param file_format: str, format to write out the image. Default, png
@@ -136,16 +138,18 @@
     plt.xlabel('Principal Component')
     plt.ylabel('Variance Explained')
     if file_path is not None:
         plt.savefig(
             file_path,
             bbox_inches='tight',
             dpi=dpi,
+            format=file_format,
         )
-    plt.show();
+    if show:
+        plt.show();
 
     for i in range(nComp):
         print(f"Explained variance for {i+1}PC: {pca.explained_variance_ratio_[i]}")
     
 
 def plot_pca(
     pca,
@@ -164,14 +168,15 @@
     xlim=None,
     ylim=None,
     dpi=300,
     loc='upper left',
     marker_size=100,
     markers=True,
     ax=None,
+    show=False,
 ):
     """Project genomes onto the PCs
     
     :param pca: sklearn PCA object
     :param X_scaled: obj from scaling data
     :param fam_df: df of cazy family freqs
     :param first_pc: int, number of the first PC
@@ -320,15 +325,16 @@
     if file_path is not None:
         plt.savefig(
             file_path,
             bbox_inches='tight',
             dpi=dpi,
             format=file_format,
         )
-    plt.show();
+    if show:
+        plt.show();
     
     return plt
 
 
 def plot_loadings(
     pca,
     fam_df,
@@ -340,14 +346,15 @@
     font_size=12,
     dpi=300,
     fig_size=(16,16),
     file_path=None,
     file_format='png',
     marker_size=100,
     ax=None,
+    show=False,
 ):
     """Build loadings plot
     
     :param pca: sklearn pca object
     :param fam_df: cazy family frequncy df
     :param first_pc: int, number of the first PC, e.g. PC1 == 1
     :param second_pc: int, number of the second PC e.g. PC2 == 2
@@ -365,22 +372,20 @@
     Return nothing"""
     sns.set(font_scale=font_scale)
 
     # calculate loading = variables x loadings, returns an array
     loadings = pca.components_.T * np.sqrt(pca.explained_variance_)
     # get labels of variables, i.e. cazy families
     loadings_labels = list(fam_df.columns)
-    try:
-        loadings_labels.remove('Species')
-    except (KeyError, ValueError):
-        pass
-    try:
-        loadings_labels.remove('Genus')
-    except (KeyError, ValueError):
-        pass
+
+    for col in ['Kingdom', 'Phylum', 'Class', 'Order', 'Tax_Family', 'Genus', 'Species', 'Genome', 'Genomes']:
+        try:
+            loadings_labels.remove(col)
+        except (KeyError, ValueError):
+            pass
 
     loadings_x = loadings[:,(first_pc-1)]
     loadings_y = loadings[:,(second_pc-1)]
 
     loadings_df = pd.DataFrame()
     loadings_df['loadings_x'] = loadings_x
     loadings_df['loadings_y'] = loadings_y
@@ -440,14 +445,17 @@
             loadings_x, loadings_y, loadings_labels
         ) if abs(xval) > threshold or abs(yval) > threshold
     ]
     adjustText.adjust_text(texts, arrowprops=dict(arrowstyle='-', color='black'));
 
     sns.move_legend(g, "lower center", bbox_to_anchor=(.5, 1), ncol=3, title=None, frameon=False);
     
+    if show:
+        plt.show();
+
     if file_path is not None:
         plt.savefig(file_path, dpi=dpi, bbox_inches='tight', format=file_format)
 
 
 def plot_ie_loadings(
     pca,
     fam_df,
@@ -482,23 +490,19 @@
     Return nothing"""
     sns.set(font_scale=font_scale)
 
     # calculate loading = variables x loadings, returns an array
     loadings = pca.components_.T * np.sqrt(pca.explained_variance_)
     # get labels of variables, i.e. cazy families
     loadings_labels = list(fam_df.columns)
-    try:
-        loadings_labels.remove('Species')
-    except (KeyError, ValueError):
-        pass
-    try:
-        loadings_labels.remove('Genus')
-    except (KeyError, ValueError):
-        pass
-
+    for col in ['Kingdom', 'Phylum', 'Class', 'Order', 'Tax_Family', 'Genus', 'Species', 'Genome', 'Genomes']:
+        try:
+            loadings_labels.remove(col)
+        except (KeyError, ValueError):
+            pass
     loadings_x = loadings[:,(first_pc-1)]
     loadings_y = loadings[:,(second_pc-1)]
 
     loadings_df = pd.DataFrame()
     loadings_df['loadings_x'] = loadings_x
     loadings_df['loadings_y'] = loadings_y
```

### Comparing `cazomevolve-0.1.6/cazomevolve/genomes/__init__.py` & `cazomevolve-0.1.7/cazomevolve/genomes/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/genomes/download_genomes.py` & `cazomevolve-0.1.7/cazomevolve/genomes/download_genomes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/__init__.py` & `cazomevolve-0.1.7/cazomevolve/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/bash/build_cazy_db.sh` & `cazomevolve-0.1.7/cazomevolve/scripts/bash/build_cazy_db.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/bash/download_acc_genomes.sh` & `cazomevolve-0.1.7/cazomevolve/scripts/bash/download_acc_genomes.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/build_cazy_db.py` & `cazomevolve-0.1.7/cazomevolve/scripts/build_cazy_db.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/cazomevolve_script.py` & `cazomevolve-0.1.7/cazomevolve/scripts/cazomevolve_script.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/download_acc_genomes.py` & `cazomevolve-0.1.7/cazomevolve/scripts/download_acc_genomes.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/get_fam_seqs.py` & `cazomevolve-0.1.7/cazomevolve/scripts/get_fam_seqs.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/run_fam_blast.py` & `cazomevolve-0.1.7/cazomevolve/scripts/run_fam_blast.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/run_fam_diamond.py` & `cazomevolve-0.1.7/cazomevolve/scripts/run_fam_diamond.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/tree/ani/build_anim_tree.R` & `cazomevolve-0.1.7/cazomevolve/scripts/tree/ani/build_anim_tree.R`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/tree/ani/run_anim.sh` & `cazomevolve-0.1.7/cazomevolve/scripts/tree/ani/run_anim.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/align_scos.sh` & `cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/align_scos.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/annotate_genomes.sh` & `cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/annotate_genomes.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/backtranslate.sh` & `cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/backtranslate.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/concatenate_cds.py` & `cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/concatenate_cds.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/extract_cds.py` & `cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/extract_cds.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/find_orthologues.sh` & `cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/find_orthologues.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh` & `cazomevolve-0.1.7/cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/seq_diversity/get_fam_seqs.sh` & `cazomevolve-0.1.7/cazomevolve/seq_diversity/get_fam_seqs.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/seq_diversity/run_blastp.sh` & `cazomevolve-0.1.7/cazomevolve/seq_diversity/run_blastp.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/seq_diversity/run_diamond.sh` & `cazomevolve-0.1.7/cazomevolve/seq_diversity/run_diamond.sh`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/taxs/__init__.py` & `cazomevolve-0.1.7/cazomevolve/taxs/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/taxs/add_taxs.py` & `cazomevolve-0.1.7/cazomevolve/taxs/add_taxs.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/taxs/ncbi.py` & `cazomevolve-0.1.7/cazomevolve/taxs/ncbi.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 
 
 import logging
 
 from Bio import Entrez
 
 from saintBioutils.genbank import entrez_retry
-from tqdm.notebook import tqdm
+from tqdm import tqdm
 
 
 def add_ncbi_taxs(genomes_tax_dict, genomes_to_query, col_names, args):
     """Query NCBI to get the taxonomic classification and add to {genome: f"{genome}_{tax}"}
 
     :param genomes_tax_dict: dict, {genome: f"{genome}_{tax}"}  - genomes with tax classification in gtdb
     :param genomes_to_query: set of genomic acc to query ncbi with to get tax classification
@@ -61,15 +61,15 @@
     taxids_genomes, failed_genomes = get_tax_ids(genomes_to_query, args)
 
     genomes_tax_dict, failed_genomes = get_ncbi_taxs(taxids_genomes, genomes_tax_dict, failed_genomes, col_names, args)
 
     for genome in failed_genomes:
         genomes_tax_dict[genome] = f"{genome}_"
         for name in col_names[1:]:
-            genomes_tax_dict[genome] += f"{NaN}_"
+            genomes_tax_dict[genome] += f"NaN_"
         genomes_tax_dict[genome] = genomes_tax_dict[genome][:-1]
 
     return genomes_tax_dict
 
 
 def get_tax_ids(genomes, args):
     """Get NCBI Tax IDs for  genomes.
```

### Comparing `cazomevolve-0.1.6/cazomevolve/utilities/__init__.py` & `cazomevolve-0.1.7/cazomevolve/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/utilities/parsers/__init__.py` & `cazomevolve-0.1.7/cazomevolve/utilities/parsers/__init__.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/utilities/parsers/add_taxs_parser.py` & `cazomevolve-0.1.7/cazomevolve/utilities/parsers/add_taxs_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/utilities/parsers/build_cazy_db_parser.py` & `cazomevolve-0.1.7/cazomevolve/utilities/parsers/build_cazy_db_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py` & `cazomevolve-0.1.7/cazomevolve/utilities/parsers/dl_acc_genomes_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/utilities/parsers/download_genomes_parser.py` & `cazomevolve-0.1.7/cazomevolve/utilities/parsers/download_genomes_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/utilities/parsers/explore_cazomes_parser.py` & `cazomevolve-0.1.7/cazomevolve/utilities/parsers/explore_cazomes_parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -171,14 +171,22 @@
         dest="species",
         action="store_true",
         default=False,
         help=" Taxonomy CSV file contains species lineage",
     )
 
     parser.add_argument(
+        "--show_plots",
+        dest="show_plots",
+        action="store_true",
+        default=False,
+        help="Display generated plots during run",
+    )
+
+    parser.add_argument(
         "--round_by",
         type=int,
         default=2,
         help="Number of decimal places to round means and SDs to",
     )
 
     parser.add_argument(
```

### Comparing `cazomevolve-0.1.6/cazomevolve/utilities/parsers/extract_prot_parser.py` & `cazomevolve-0.1.7/cazomevolve/utilities/parsers/get_cazy_parser.py`

 * *Files 17% similar despite different names*

```diff
@@ -33,55 +33,77 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 # IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
+"""Build args parser for get_cazy_cazymes.py"""
 
 
-import argparse
-
+from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser, _SubParsersAction
 from pathlib import Path
 from typing import List, Optional
 
+from cazomevolve.cazome.cazy import get_cazy_cazymes
+
 
-def build_parser(argv: Optional[List] = None):
+def build_parser(
+    subps: _SubParsersAction, parents: Optional[List[ArgumentParser]] = None
+) -> None:
     """Return ArgumentParser parser for script."""
     # Create parser object
-    parser = argparse.ArgumentParser(
-        prog="extract_prot_seqs",
-        description="Extract protein seqs from gbff genomic assemblies",
-        formatter_class=argparse.ArgumentDefaultsHelpFormatter,
+    parser = subps.add_parser(
+        "get_cazy_cazymes", formatter_class=ArgumentDefaultsHelpFormatter
     )
 
     # Add positional arguments to parser
 
     parser.add_argument(
-        "genome_dir",
+        "input_dir",
         type=Path,
-        help="Path to directory containing genomic assemblies",
+        help="Path to dir containing fasta files to retrieve CAZy annotations from",
+    )
+
+    parser.add_argument(
+        "database",
+        type=Path,
+        default=None,
+        help="Path to local CAZyme database (SQLite3) compiled by cazy_webscraper",
     )
 
     parser.add_argument(
-        "protein_dir",
+        "output_dir",
         type=Path,
-        help="Path to directory to write out multiseq FASTA files of protein seqs",
+        help="Directory to write out fasta files for parsing by dbCAN",
+    )
+
+    parser.add_argument(
+        "fam_genome_list",
+        type=Path,
+        default=None,
+        help="Path to write out tab deliminated list of fam and genome pairs",
+    )
+
+    parser.add_argument(
+        "fam_genome_protein_list",
+        type=Path,
+        default=None,
+        help="Path to write out tab deliminated list of fam, genome and protein annocations",
     )
 
-    # Add option to force file over writting
     parser.add_argument(
         "-f",
         "--force",
         dest="force",
         action="store_true",
         default=False,
         help="Force file over writting",
     )
-
+    
     parser.add_argument(
         "-l",
         "--log",
         type=Path,
         metavar="log file name",
         default=None,
         help="Defines log file name and/or path",
@@ -91,30 +113,25 @@
         "-n",
         "--nodelete",
         dest="nodelete",
         action="store_true",
         default=False,
         help="enable/disable deletion of exisiting files",
     )
+
     parser.add_argument(
-        "--prefix",
-        dest="prefix",
-        type=str,
-        default="",
-        help="Prefix for all output FASTA files",
-    )
-    # Add option to specify verbose logging
+        "--sql_echo",
+        dest="sql_echo",
+        action="store_true",
+        default=False,
+        help="Set verbose SQLite3 logging",
+    )    
+
     parser.add_argument(
         "-v",
         "--verbose",
         dest="verbose",
         action="store_true",
         default=False,
         help="Set logger level to 'INFO'",
     )
-
-    if argv is None:
-        # parse command-line
-        return parser
-    else:
-        # return namespace
-        return parser.parse_args(argv)
+    parser.set_defaults(func=get_cazy_cazymes.main)
```

### Comparing `cazomevolve-0.1.6/cazomevolve/utilities/parsers/get_cazy_parser.py` & `cazomevolve-0.1.7/cazomevolve/utilities/parsers/get_dbcan_parser.py`

 * *Files 6% similar despite different names*

```diff
@@ -35,50 +35,36 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
 # SOFTWARE.
 """Build args parser for get_cazy_cazymes.py"""
 
-
 from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser, _SubParsersAction
 from pathlib import Path
 from typing import List, Optional
 
-from cazomevolve.cazome.cazy import get_cazy_cazymes
+from cazomevolve.cazome.dbcan import get_dbcan_cazymes
 
 
 def build_parser(
     subps: _SubParsersAction, parents: Optional[List[ArgumentParser]] = None
 ) -> None:
     """Return ArgumentParser parser for script."""
     # Create parser object
     parser = subps.add_parser(
-        "get_cazy_cazymes", formatter_class=ArgumentDefaultsHelpFormatter
+        "get_dbcan_cazymes", formatter_class=ArgumentDefaultsHelpFormatter
     )
 
     # Add positional arguments to parser
 
     parser.add_argument(
-        "input_dir",
-        type=Path,
-        help="Path to dir containing fasta files to retrieve CAZy annotations from",
-    )
-
-    parser.add_argument(
-        "database",
+        "dbcan_dir",
         type=Path,
-        default=None,
-        help="Path to local CAZyme database (SQLite3) compiled by cazy_webscraper",
-    )
-
-    parser.add_argument(
-        "output_dir",
-        type=Path,
-        help="Directory to write out fasta files for parsing by dbCAN",
+        help="Path to dir containing output dirs from dbCAN",
     )
 
     parser.add_argument(
         "fam_genome_list",
         type=Path,
         default=None,
         help="Path to write out tab deliminated list of fam and genome pairs",
@@ -115,23 +101,16 @@
         dest="nodelete",
         action="store_true",
         default=False,
         help="enable/disable deletion of exisiting files",
     )
 
     parser.add_argument(
-        "--sql_echo",
-        dest="sql_echo",
-        action="store_true",
-        default=False,
-        help="Set verbose SQLite3 logging",
-    )    
-
-    parser.add_argument(
         "-v",
         "--verbose",
         dest="verbose",
         action="store_true",
         default=False,
         help="Set logger level to 'INFO'",
     )
-    parser.set_defaults(func=get_cazy_cazymes.main)
+
+    parser.set_defaults(func=get_dbcan_cazymes.main)
```

### Comparing `cazomevolve-0.1.6/cazomevolve/utilities/parsers/get_dbcan_parser.py` & `cazomevolve-0.1.7/cazomevolve/utilities/parsers/invoke_dbcan_parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,116 +1,128 @@
-#!/usr/bin/env python3
-# -*- coding: utf-8 -*-
-# (c) University of St Andrews 2022
-# (c) University of Strathclyde 2022
-# (c) James Hutton Institute 2022
-# Author:
-# Emma E. M. Hobbs
-
-# Contact
-# eemh1@st-andrews.ac.uk
-
-# Emma E. M. Hobbs,
-# Biomolecular Sciences Building,
-# University of St Andrews,
-# North Haugh Campus,
-# St Andrews,
-# KY16 9ST
-# Scotland,
-# UK
-
-# The MIT License
-#
-# Permission is hereby granted, free of charge, to any person obtaining a copy
-# of this software and associated documentation files (the "Software"), to deal
-# in the Software without restriction, including without limitation the rights
-# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-# copies of the Software, and to permit persons to whom the Software is
-# furnished to do so, subject to the following conditions:
-
-# The above copyright notice and this permission notice shall be included in all
-# copies or substantial portions of the Software.
-
-# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-# SOFTWARE.
-"""Build args parser for get_cazy_cazymes.py"""
-
-from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser, _SubParsersAction
-from pathlib import Path
-from typing import List, Optional
-
-from cazomevolve.cazome.dbcan import get_dbcan_cazymes
-
-
-def build_parser(
-    subps: _SubParsersAction, parents: Optional[List[ArgumentParser]] = None
-) -> None:
-    """Return ArgumentParser parser for script."""
-    # Create parser object
-    parser = subps.add_parser(
-        "get_dbcan_cazymes", formatter_class=ArgumentDefaultsHelpFormatter
-    )
-
-    # Add positional arguments to parser
-
-    parser.add_argument(
-        "dbcan_dir",
-        type=Path,
-        help="Path to dir containing output dirs from dbCAN",
-    )
-
-    parser.add_argument(
-        "fam_genome_list",
-        type=Path,
-        default=None,
-        help="Path to write out tab deliminated list of fam and genome pairs",
-    )
-
-    parser.add_argument(
-        "fam_genome_protein_list",
-        type=Path,
-        default=None,
-        help="Path to write out tab deliminated list of fam, genome and protein annocations",
-    )
-
-    parser.add_argument(
-        "-f",
-        "--force",
-        dest="force",
-        action="store_true",
-        default=False,
-        help="Force file over writting",
-    )
-    
-    parser.add_argument(
-        "-l",
-        "--log",
-        type=Path,
-        metavar="log file name",
-        default=None,
-        help="Defines log file name and/or path",
-    )
-    
-    parser.add_argument(
-        "-n",
-        "--nodelete",
-        dest="nodelete",
-        action="store_true",
-        default=False,
-        help="enable/disable deletion of exisiting files",
-    )
-
-    parser.add_argument(
-        "-v",
-        "--verbose",
-        dest="verbose",
-        action="store_true",
-        default=False,
-        help="Set logger level to 'INFO'",
-    )
-
-    parser.set_defaults(func=get_dbcan_cazymes.main)
+#!/usr/bin/env python3
+# -*- coding: utf-8 -*-
+# (c) University of St Andrews 2022
+# (c) University of Strathclyde 2022
+# (c) James Hutton Institute 2022
+# Author:
+# Emma E. M. Hobbs
+
+# Contact
+# eemh1@st-andrews.ac.uk
+
+# Emma E. M. Hobbs,
+# Biomolecular Sciences Building,
+# University of St Andrews,
+# North Haugh Campus,
+# St Andrews,
+# KY16 9ST
+# Scotland,
+# UK
+
+# The MIT License
+#
+# Permission is hereby granted, free of charge, to any person obtaining a copy
+# of this software and associated documentation files (the "Software"), to deal
+# in the Software without restriction, including without limitation the rights
+# to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+# copies of the Software, and to permit persons to whom the Software is
+# furnished to do so, subject to the following conditions:
+
+# The above copyright notice and this permission notice shall be included in all
+# copies or substantial portions of the Software.
+
+# THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+# IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+# FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+# AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+# LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+# OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+# SOFTWARE.
+"""Build CLI for invoke_dbcan.py"""
+
+
+import multiprocessing
+
+from argparse import ArgumentDefaultsHelpFormatter, ArgumentParser, _SubParsersAction
+from pathlib import Path
+from typing import List, Optional
+
+from cazomevolve.cazome.dbcan import invoke_dbcan
+
+
+def build_parser(
+    subps: _SubParsersAction, parents: Optional[List[ArgumentParser]] = None
+) -> None:
+    """Return ArgumentParser parser for script."""
+    # Create parser object
+    parser = subps.add_parser(
+        "run_dbcan", formatter_class=ArgumentDefaultsHelpFormatter
+    )
+
+    # Add positional arguments to parser
+
+    parser.add_argument(
+        "input_dir",
+        type=Path,
+        help="Path to directory containing FASTAs to be parsed by dbCAN",
+    )
+
+    parser.add_argument(
+        "output_dir",
+        type=Path,
+        help="Path to directory to write out genomic assemblies",
+    )
+
+    parser.add_argument(
+        "dbcan_version",
+        type=int,
+        help="Major version number of dbCAN being used (e.g. 2, 3, or 4)",
+    )
+
+    parser.add_argument(
+        "--cpu",
+        type=int,
+        default=multiprocessing.cpu_count(),
+        help="Number of CPU cores to use. Default all available cores",
+    )
+
+    # Add option to force file over writting
+    parser.add_argument(
+        "-f",
+        "--force",
+        dest="force",
+        action="store_true",
+        default=False,
+        help="Force file over writting",
+    )
+
+    # Add option to specific directory for log to be written out to
+    parser.add_argument(
+        "-l",
+        "--log",
+        type=Path,
+        metavar="log file name",
+        default=None,
+        help="Defines log file name and/or path",
+    )
+    # Add option to prevent over writing of existing files
+    # and cause addition of files to output directory
+    parser.add_argument(
+        "-n",
+        "--nodelete",
+        dest="nodelete",
+        action="store_true",
+        default=False,
+        help="enable/disable deletion of exisiting files",
+    )
+
+    # Add option to specify verbose logging
+    parser.add_argument(
+        "-v",
+        "--verbose",
+        dest="verbose",
+        action="store_true",
+        default=False,
+        help="Set logger level to 'INFO'",
+    )
+    parser.set_defaults(func=invoke_dbcan.main)
+
```

### Comparing `cazomevolve-0.1.6/cazomevolve/utilities/parsers/get_fam_seqs_parser.py` & `cazomevolve-0.1.7/cazomevolve/utilities/parsers/get_fam_seqs_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/utilities/parsers/parse_cmd.py` & `cazomevolve-0.1.7/cazomevolve/utilities/parsers/parse_cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,14 @@
     run_diamond_parser,
     dl_acc_genomes_parser,
     download_genomes_parser,
     build_cazy_db_parser,
     get_cazy_parser,
     invoke_dbcan_parser,
     get_dbcan_parser,
-    common_parser,
     add_taxs_parser,
     explore_cazomes_parser,
 )
 
 
 def build_parser(argv: Optional[List] = None) -> Namespace:
     """Parse command-line arguments for script.
```

### Comparing `cazomevolve-0.1.6/cazomevolve/utilities/parsers/run_blast_parser.py` & `cazomevolve-0.1.7/cazomevolve/utilities/parsers/run_blast_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve/utilities/parsers/run_diamond_parser.py` & `cazomevolve-0.1.7/cazomevolve/utilities/parsers/run_diamond_parser.py`

 * *Files identical despite different names*

### Comparing `cazomevolve-0.1.6/cazomevolve.egg-info/PKG-INFO` & `cazomevolve-0.1.7/cazomevolve.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cazomevolve
-Version: 0.1.6
+Version: 0.1.7
 Summary: A bioinforamtic package for investigating the evolution of CAZomes
 Author: Emma E. M. Hobbs
 Author-email: eemh1@st-andrews.ac.uk
 License: MIT
 Keywords: bioinforamtics protein
 Platform: Posix
 Platform: MacOS X
@@ -21,14 +21,16 @@
 License-File: LICENSE
 
 # cazomevolve
 
 [![DOI](https://zenodo.org/badge/367898306.svg)](https://zenodo.org/badge/latestdoi/367898306)
 [![Documentation Status](https://readthedocs.org/projects/cazomevolve/badge/?version=latest)](https://cazomevolve.readthedocs.io/en/latest/?badge=latest)
 [![licence](https://img.shields.io/badge/Licence-MIT-green)](https://github.com/HobnobMancer/cazomevolve/blob/master/LICENSE)  
+[![CircleCI](https://circleci.com/gh/HobnobMancer/cazomevolve.svg?style=shield)](https://circleci.com/gh/HobnobMancer/cazomevolve)
+[![codecov](https://codecov.io/gh/HobnobMancer/cazomevolve/branch/master/graph/badge.svg)](https://codecov.io/gh/HobnobMancer/cazomevolve)  
 ![Python](https://img.shields.io/badge/Python-v3.9.---orange)
 ![Research](https://img.shields.io/badge/Research-Bioinformatics-ff69b4)
 [![Funding BBSCR](https://img.shields.io/badge/Funding-EASTBio-blue)](http://www.eastscotbiodtp.ac.uk/)
 [![cazomevolve PyPi version](https://img.shields.io/pypi/v/cazomevolve "PyPI version")](https://pypi.python.org/pypi/cazomevolve)  
 [![Downloads](https://pepy.tech/badge/cazomevolve)](https://pepy.tech/project/cazomevolve)
 
 `cazomevolve` ('cazome-evolve') is an application and Python3 package for the automated annotation and exploratory analysis of CAZyme complements (CAZomes) for a set of species and/or genomes of interest. Carbohydrate Active enZymes are a subset of proteins that generate, modify and/or degrade carbohydrates. CAZy (www.cazy.org) is the most comprehensive CAZyme database, grouping proteins by sequence similarity into CAZy families.
@@ -82,15 +84,15 @@
 > Kozlov AM, Darriba D, Flouri T, Morel B, Stamatakis A. RAxML-NG: a fast, scalable and user-friendly tool for maximum likelihood phylogenetic inference. Bioinformatics. 2019 Nov 1;35(21):4453-4455. doi: 10.1093/bioinformatics/btz305.
 > Whelan FJ, Rusilowicz M, McInerney JO. Coinfinder: detecting significant associations and dissociations in pangenomes. Microb Genom. 2020 Mar;6(3):e000338. doi: 10.1099/mgen.0.000338. Epub 2020 Feb 24.
 
 ## Documentation
 
 `cazomevolve` uses bash-script based workflow management. A summary of this workflow is provided in this README.
 
-Please see the [full documeentation including tutorials at ReadTheDocs]().
+Please see the [full documeentation including tutorials at ReadTheDocs](https://cazomevolve.readthedocs.io/en/latest/?badge=latest).
 
 An analysis using `cazomevolve` can be found [here](https://github.com/HobnobMancer/SI_Hobbs_et_al_2023_Pecto), which includes a README-walkthrough and all output files.
 
 ## Contents
 
 1. [cazomevolve](#cazomevolve)
 2. [Documentation](#documentation)
@@ -666,14 +668,15 @@
   results/ \
   --genus \
   --species
 ```
 
 ### Optional
 
+* `--show_plots` - Display plots generated as the program is executing (default: False)
 * `--round_by` - ROUND_BY - Number of decimal places to round means and SDs to (default: 2)
 * `-f`, `--force` - Force file over writting (default: False)
 * `-l`, `--log` log file name - Defines log file name and/or path (default: None)
 * `-n`, `--nodelete` - enable/disable deletion of exisiting files (default: False)
 * `-v`, `--verbose` - Set logger level to 'INFO' (default: False)
 
 ## Full customisation of CAZome exploration
```

### Comparing `cazomevolve-0.1.6/cazomevolve.egg-info/SOURCES.txt` & `cazomevolve-0.1.7/cazomevolve.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -16,19 +16,16 @@
 cazomevolve/cazome/dbcan/invoke_dbcan.py
 cazomevolve/cazome/explore/__init__.py
 cazomevolve/cazome/explore/cazome_sizes.py
 cazomevolve/cazome/explore/cazy_classes.py
 cazomevolve/cazome/explore/cazy_families.py
 cazomevolve/cazome/explore/cooccurring_families.py
 cazomevolve/cazome/explore/explore_cazomes.py
-cazomevolve/cazome/explore/identify_families.py
 cazomevolve/cazome/explore/parse_data.py
 cazomevolve/cazome/explore/pca.py
-cazomevolve/cazome/explore/plot.py
-cazomevolve/cazome/explore/taxonomies.py
 cazomevolve/genomes/__init__.py
 cazomevolve/genomes/download_genomes.py
 cazomevolve/scripts/__init__.py
 cazomevolve/scripts/build_cazy_db.py
 cazomevolve/scripts/cazomevolve_script.py
 cazomevolve/scripts/download_acc_genomes.py
 cazomevolve/scripts/get_fam_seqs.py
@@ -41,29 +38,50 @@
 cazomevolve/scripts/tree/phylo/align_scos.sh
 cazomevolve/scripts/tree/phylo/annotate_genomes.sh
 cazomevolve/scripts/tree/phylo/backtranslate.sh
 cazomevolve/scripts/tree/phylo/concatenate_cds.py
 cazomevolve/scripts/tree/phylo/extract_cds.py
 cazomevolve/scripts/tree/phylo/find_orthologues.sh
 cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh
+cazomevolve/seq_diversity/__init__.py
 cazomevolve/seq_diversity/get_fam_seqs.sh
 cazomevolve/seq_diversity/run_blastp.sh
 cazomevolve/seq_diversity/run_diamond.sh
+cazomevolve/seq_diversity/explore/__init__.py
+cazomevolve/seq_diversity/explore/cazy.py
+cazomevolve/seq_diversity/explore/parse.py
+cazomevolve/seq_diversity/explore/plot.py
 cazomevolve/taxs/__init__.py
 cazomevolve/taxs/add_taxs.py
 cazomevolve/taxs/ncbi.py
 cazomevolve/utilities/__init__.py
 cazomevolve/utilities/parsers/__init__.py
 cazomevolve/utilities/parsers/add_taxs_parser.py
 cazomevolve/utilities/parsers/build_cazy_db_parser.py
-cazomevolve/utilities/parsers/common_parser.py
 cazomevolve/utilities/parsers/dl_acc_genomes_parser.py
 cazomevolve/utilities/parsers/download_genomes_parser.py
 cazomevolve/utilities/parsers/explore_cazomes_parser.py
-cazomevolve/utilities/parsers/extract_prot_parser.py
 cazomevolve/utilities/parsers/get_cazy_parser.py
 cazomevolve/utilities/parsers/get_dbcan_parser.py
 cazomevolve/utilities/parsers/get_fam_seqs_parser.py
 cazomevolve/utilities/parsers/invoke_dbcan_parser.py
 cazomevolve/utilities/parsers/parse_cmd.py
 cazomevolve/utilities/parsers/run_blast_parser.py
-cazomevolve/utilities/parsers/run_diamond_parser.py
+cazomevolve/utilities/parsers/run_diamond_parser.py
+tests/test_add_taxs.py
+tests/test_cazomevolve.py
+tests/test_explore_cazome_sizes.py
+tests/test_explore_cazomes.py
+tests/test_explore_classes.py
+tests/test_explore_cooccurring_families.py
+tests/test_explore_families.py
+tests/test_explore_parse_data.py
+tests/test_explore_pca.py
+tests/test_explore_upsetplot.py
+tests/test_genome_download.py
+tests/test_get_cazy.py
+tests/test_get_dbcan.py
+tests/test_invoke_dbcan.py
+tests/test_ncbi.py
+tests/test_parser.py
+tests/test_scripts.py
+tests/test_seq_diversity.py
```

### Comparing `cazomevolve-0.1.6/setup.py` & `cazomevolve-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 # get long description from README.md
 with Path("README.md").open("r") as long_description_handle:
     long_description = long_description_handle.read()
 
 
 setuptools.setup(
     name="cazomevolve",
-    version="0.1.6",
+    version="0.1.7",
     # Metadata
     author="Emma E. M. Hobbs",
     author_email="eemh1@st-andrews.ac.uk",
     description="".join(
         [
             (
                 "A bioinforamtic package for investigating the evolution of CAZomes"
@@ -87,14 +87,15 @@
         'cazomevolve/scripts/tree/phylo/find_orthologues.sh',
         'cazomevolve/scripts/tree/phylo/raxml_ng_build_tree.sh',
         'cazomevolve/scripts/tree/ani/run_anim.sh',
         'cazomevolve/scripts/tree/ani/build_anim_tree.R',
     ],
     install_requires=[
         "adjustText",
+        "bs4",
         "biopython",
         "cazy_webscraper",
         "matplotlib",
         "ncbi-genome-download",
         "numpy",
         "pandas",
         "saintbioutils",
```

