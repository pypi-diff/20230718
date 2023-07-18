# Comparing `tmp/ingenannot-0.0.7.tar.gz` & `tmp/ingenannot-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ingenannot-0.0.7.tar", last modified: Mon Feb 20 14:34:37 2023, max compression
+gzip compressed data, was "ingenannot-0.0.8.tar", last modified: Tue Jul 18 07:38:58 2023, max compression
```

## Comparing `ingenannot-0.0.7.tar` & `ingenannot-0.0.8.tar`

### file list

```diff
@@ -1,64 +1,58 @@
-drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-02-20 14:34:37.177397 ingenannot-0.0.7/
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     7652 2022-11-02 13:47:42.000000 ingenannot-0.0.7/LICENSE
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     9912 2023-02-20 14:34:37.177397 ingenannot-0.0.7/PKG-INFO
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     9339 2022-11-09 10:34:03.000000 ingenannot-0.0.7/README.md
-drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-02-20 14:34:37.177397 ingenannot-0.0.7/ingenannot/
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)        0 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/__init__.py
-drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-02-20 14:34:37.177397 ingenannot-0.0.7/ingenannot/commands/
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    37134 2023-02-20 14:31:58.000000 ingenannot-0.0.7/ingenannot/commands/AddIsoforms.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2187 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/commands/StringtieFilter.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     6051 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/commands/StringtieJaclip.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1753 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/commands/StringtieRefine.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     6532 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/commands/StringtieStats.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    18817 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/commands/SupportIsoformFilter.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1415 2022-11-09 07:30:49.000000 ingenannot-0.0.7/ingenannot/commands/__init__.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     5847 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/commands/add_sqanti3_isoforms.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     5980 2022-11-09 07:30:49.000000 ingenannot-0.0.7/ingenannot/commands/aed.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     3068 2023-02-20 14:31:58.000000 ingenannot-0.0.7/ingenannot/commands/aed_compare.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2396 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/commands/clusterize.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       78 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/commands/command.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    14938 2022-11-09 07:30:49.000000 ingenannot-0.0.7/ingenannot/commands/compare.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)      838 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/commands/effector_predictor_cmd.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4236 2022-11-09 07:30:49.000000 ingenannot-0.0.7/ingenannot/commands/exonerate_to_gff.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4746 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/commands/filter.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    34343 2022-11-09 07:30:49.000000 ingenannot-0.0.7/ingenannot/commands/isoform_ranking.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    13587 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/commands/reduce.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     7153 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/commands/rename.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    15953 2022-11-09 07:30:49.000000 ingenannot-0.0.7/ingenannot/commands/rescue_effectors.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    18497 2023-02-20 14:31:58.000000 ingenannot-0.0.7/ingenannot/commands/select.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     3263 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/commands/so_classification.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4193 2022-11-09 07:30:49.000000 ingenannot-0.0.7/ingenannot/commands/strand_annotation_filter.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    12869 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/commands/utr_refine.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4581 2022-12-14 14:37:30.000000 ingenannot-0.0.7/ingenannot/commands/validate.py
-drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-02-20 14:34:37.177397 ingenannot-0.0.7/ingenannot/entities/
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)        0 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/entities/__init__.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1823 2022-11-09 07:30:49.000000 ingenannot-0.0.7/ingenannot/entities/cds.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     3672 2022-11-09 07:30:49.000000 ingenannot-0.0.7/ingenannot/entities/cluster.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2520 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/entities/exon.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4464 2023-02-20 14:31:58.000000 ingenannot-0.0.7/ingenannot/entities/gene.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)      290 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/entities/intron.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     5929 2022-11-09 07:30:49.000000 ingenannot-0.0.7/ingenannot/entities/metagene.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    18396 2023-02-20 14:31:58.000000 ingenannot-0.0.7/ingenannot/entities/transcript.py
--rwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)    38433 2023-02-20 14:31:58.000000 ingenannot-0.0.7/ingenannot/main.py
-drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-02-20 14:34:37.177397 ingenannot-0.0.7/ingenannot/utils/
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    27112 2023-02-20 14:31:58.000000 ingenannot-0.0.7/ingenannot/utils/__init__.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     8947 2023-02-20 14:31:58.000000 ingenannot-0.0.7/ingenannot/utils/annot_edit_distance.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    11180 2022-11-09 07:30:49.000000 ingenannot-0.0.7/ingenannot/utils/effector_predictor.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2111 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/utils/em_operators.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    15370 2023-02-20 14:31:58.000000 ingenannot-0.0.7/ingenannot/utils/gene_builder.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    11417 2022-12-14 10:01:33.000000 ingenannot-0.0.7/ingenannot/utils/gff_reader.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    11247 2022-11-09 07:30:49.000000 ingenannot-0.0.7/ingenannot/utils/graphics.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2835 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/utils/so_splicing_classifier.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2742 2023-02-20 14:31:58.000000 ingenannot-0.0.7/ingenannot/utils/statistics.py
--rwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)     8495 2023-02-02 08:36:33.000000 ingenannot-0.0.7/ingenannot/utils/stats.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1673 2022-11-02 13:47:42.000000 ingenannot-0.0.7/ingenannot/utils/tool_checker.py
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       48 2023-02-20 14:34:09.000000 ingenannot-0.0.7/ingenannot/version.py
-drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-02-20 14:34:37.177397 ingenannot-0.0.7/ingenannot.egg-info/
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     9912 2023-02-20 14:34:37.000000 ingenannot-0.0.7/ingenannot.egg-info/PKG-INFO
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1813 2023-02-20 14:34:37.000000 ingenannot-0.0.7/ingenannot.egg-info/SOURCES.txt
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)        1 2023-02-20 14:34:37.000000 ingenannot-0.0.7/ingenannot.egg-info/dependency_links.txt
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       52 2023-02-20 14:34:37.000000 ingenannot-0.0.7/ingenannot.egg-info/entry_points.txt
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       59 2023-02-20 14:34:37.000000 ingenannot-0.0.7/ingenannot.egg-info/requires.txt
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       11 2023-02-20 14:34:37.000000 ingenannot-0.0.7/ingenannot.egg-info/top_level.txt
--rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       38 2023-02-20 14:34:37.177397 ingenannot-0.0.7/setup.cfg
--rwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)     1831 2023-02-16 15:51:39.000000 ingenannot-0.0.7/setup.py
+drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-18 07:38:58.572254 ingenannot-0.0.8/
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     7652 2022-11-02 13:47:42.000000 ingenannot-0.0.8/LICENSE
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     9860 2023-07-18 07:38:58.572254 ingenannot-0.0.8/PKG-INFO
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     9287 2023-07-18 07:37:47.000000 ingenannot-0.0.8/README.md
+drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-18 07:38:58.572254 ingenannot-0.0.8/ingenannot/
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)        0 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/__init__.py
+drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-18 07:38:58.572254 ingenannot-0.0.8/ingenannot/commands/
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1465 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/__init__.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     5847 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/commands/add_sqanti3_isoforms.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     5621 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/aed.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     3432 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/aed_compare.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2396 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/commands/clusterize.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       78 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/commands/command.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    14938 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/commands/compare.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     7949 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/curation.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)      838 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/commands/effector_predictor_cmd.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4236 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/commands/exonerate_to_gff.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4746 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/commands/filter.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    30896 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/isoform_ranking.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     7161 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/rename.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    15953 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/commands/rescue_effectors.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    18638 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/select.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     3263 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/commands/so_classification.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4193 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/commands/strand_annotation_filter.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    11578 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/commands/utr_refine.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4581 2022-12-14 14:37:30.000000 ingenannot-0.0.8/ingenannot/commands/validate.py
+drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-18 07:38:58.572254 ingenannot-0.0.8/ingenannot/entities/
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)        0 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/entities/__init__.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1823 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/entities/cds.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     3672 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/entities/cluster.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2520 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/entities/exon.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     4464 2023-02-20 14:31:58.000000 ingenannot-0.0.8/ingenannot/entities/gene.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)      290 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/entities/intron.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     5929 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/entities/metagene.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    18396 2023-02-20 14:31:58.000000 ingenannot-0.0.8/ingenannot/entities/transcript.py
+-rwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)    39864 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/main.py
+drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-18 07:38:58.572254 ingenannot-0.0.8/ingenannot/utils/
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    27171 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/utils/__init__.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     8947 2023-02-20 14:31:58.000000 ingenannot-0.0.8/ingenannot/utils/annot_edit_distance.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    11180 2022-11-09 07:30:49.000000 ingenannot-0.0.8/ingenannot/utils/effector_predictor.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2111 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/utils/em_operators.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    15370 2023-02-20 14:31:58.000000 ingenannot-0.0.8/ingenannot/utils/gene_builder.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    11417 2022-12-14 10:01:33.000000 ingenannot-0.0.8/ingenannot/utils/gff_reader.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)    13268 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/utils/graphics.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2835 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/utils/so_splicing_classifier.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     2743 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/utils/statistics.py
+-rwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)     8495 2023-02-02 08:36:33.000000 ingenannot-0.0.8/ingenannot/utils/stats.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1673 2022-11-02 13:47:42.000000 ingenannot-0.0.8/ingenannot/utils/tool_checker.py
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       48 2023-07-18 07:37:47.000000 ingenannot-0.0.8/ingenannot/version.py
+drwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)        0 2023-07-18 07:38:58.572254 ingenannot-0.0.8/ingenannot.egg-info/
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     9860 2023-07-18 07:38:58.000000 ingenannot-0.0.8/ingenannot.egg-info/PKG-INFO
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)     1581 2023-07-18 07:38:58.000000 ingenannot-0.0.8/ingenannot.egg-info/SOURCES.txt
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)        1 2023-07-18 07:38:58.000000 ingenannot-0.0.8/ingenannot.egg-info/dependency_links.txt
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       52 2023-07-18 07:38:58.000000 ingenannot-0.0.8/ingenannot.egg-info/entry_points.txt
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       59 2023-07-18 07:38:58.000000 ingenannot-0.0.8/ingenannot.egg-info/requires.txt
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       11 2023-07-18 07:38:58.000000 ingenannot-0.0.8/ingenannot.egg-info/top_level.txt
+-rw-r--r--   0 nlapalu   (1000) nlapalu   (1000)       38 2023-07-18 07:38:58.572254 ingenannot-0.0.8/setup.cfg
+-rwxr-xr-x   0 nlapalu   (1000) nlapalu   (1000)     1831 2023-02-16 15:51:39.000000 ingenannot-0.0.8/setup.py
```

### Comparing `ingenannot-0.0.7/LICENSE` & `ingenannot-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/PKG-INFO` & `ingenannot-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingenannot
-Version: 0.0.7
+Version: 0.0.8
 Summary: InGenAnnot: Inspection of Gene Annotation
 Home-page: https://forgemia.inra.fr/bioger/ingenannot
 Author: Nicolas Lapalu
 Author-email: nicolas.lapalu@inrae.fr
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
@@ -37,15 +37,15 @@
 clusterize genes, to propose new loci sharing a list of transcripts.
 We define these new loci as 'meta-gene' and propose several options
 to clusterize them. We tried to summarize the pro and cons of classification feature type in the following table.
 
 ||pros|cons|
 |:--:|--|--|
 |`--clu-type gene`|detect problem of missens predictions|overlaps of UTR merge different genes, not suitable for compact genomes|
-|`--clu-type cds`|detect problem of missens predictions|could not correct splitted CDS|
+|`--clu-type cds`|detect problem of missens predictions|could not correct split CDS|
 |`--clu-type gene` `--clu-stranded`|resolve conflict between genes and possible non-coding RNA on the opposite strand|will not detect severe problem due to divergent prediction on opposite strand, overlaps of UTR merge different genes|
 |`--clu-type cds` `--clu-stranded`|resolve conflict between genes and possible non-coding RNA on the opposite strand|will not detect severe problem due to divergent prediction on opposite strand|
 
 In most cases, we recommended to use `--clu-type cds` with `--clu-stranded` to avoid gene merge. A post-process is implemented to remove overlapping CDS, keeping gene models with the best AED scores.
 
 
 ## Selection of best gene structures, evidence-driven with Annotation Edit Distance (AED)
@@ -89,17 +89,15 @@
 |0:N:N|All transcript-pairs share sequence in common and some share exon boundaries|![0:N:N](https://forgemia.inra.fr/bioger/ingenannot/raw/master/docs/img/0_N_N.png)|
 |0:0:N|All transcript-pairs share some exons in common|![0:0:N](https://forgemia.inra.fr/bioger/ingenannot/raw/master/docs/img/0_0_N.png)|
 
 As described above, the SO classification was originally based on exon boundaries,
 that could be highly problematic for de-novo annotations with poorly
 defined UTR parts. To avoid such problem, you can choose to perform
 the same classification based on CDS coordinates. In this case you 
-will obtained less biased results.  We tried
-to summarize the pro and cons of classification feature type in
-the following table.
+will obtained less biased results (See table above for pros/cons of clustering).
 
 
 ## Documentation: install, tools and use cases 
 
 `InGenAnnot` comes with multiple tools allowing analysis of your gene prediction datasets. You will be able to compare, select and annotate your genes with different tools [(link to documentation)](https://bioger.pages.mia.inra.fr/ingenannot/index.html). Full use cases are described step by step, such as:
 
 * [best gene selection](https://bioger.pages.mia.inra.fr/ingenannot/usecases/select_best_gene_models.html)
```

### Comparing `ingenannot-0.0.7/README.md` & `ingenannot-0.0.8/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 clusterize genes, to propose new loci sharing a list of transcripts.
 We define these new loci as 'meta-gene' and propose several options
 to clusterize them. We tried to summarize the pro and cons of classification feature type in the following table.
 
 ||pros|cons|
 |:--:|--|--|
 |`--clu-type gene`|detect problem of missens predictions|overlaps of UTR merge different genes, not suitable for compact genomes|
-|`--clu-type cds`|detect problem of missens predictions|could not correct splitted CDS|
+|`--clu-type cds`|detect problem of missens predictions|could not correct split CDS|
 |`--clu-type gene` `--clu-stranded`|resolve conflict between genes and possible non-coding RNA on the opposite strand|will not detect severe problem due to divergent prediction on opposite strand, overlaps of UTR merge different genes|
 |`--clu-type cds` `--clu-stranded`|resolve conflict between genes and possible non-coding RNA on the opposite strand|will not detect severe problem due to divergent prediction on opposite strand|
 
 In most cases, we recommended to use `--clu-type cds` with `--clu-stranded` to avoid gene merge. A post-process is implemented to remove overlapping CDS, keeping gene models with the best AED scores.
 
 
 ## Selection of best gene structures, evidence-driven with Annotation Edit Distance (AED)
@@ -73,17 +73,15 @@
 |0:N:N|All transcript-pairs share sequence in common and some share exon boundaries|![0:N:N](https://forgemia.inra.fr/bioger/ingenannot/raw/master/docs/img/0_N_N.png)|
 |0:0:N|All transcript-pairs share some exons in common|![0:0:N](https://forgemia.inra.fr/bioger/ingenannot/raw/master/docs/img/0_0_N.png)|
 
 As described above, the SO classification was originally based on exon boundaries,
 that could be highly problematic for de-novo annotations with poorly
 defined UTR parts. To avoid such problem, you can choose to perform
 the same classification based on CDS coordinates. In this case you 
-will obtained less biased results.  We tried
-to summarize the pro and cons of classification feature type in
-the following table.
+will obtained less biased results (See table above for pros/cons of clustering).
 
 
 ## Documentation: install, tools and use cases 
 
 `InGenAnnot` comes with multiple tools allowing analysis of your gene prediction datasets. You will be able to compare, select and annotate your genes with different tools [(link to documentation)](https://bioger.pages.mia.inra.fr/ingenannot/index.html). Full use cases are described step by step, such as:
 
 * [best gene selection](https://bioger.pages.mia.inra.fr/ingenannot/usecases/select_best_gene_models.html)
```

### Comparing `ingenannot-0.0.7/ingenannot/commands/__init__.py` & `ingenannot-0.0.8/ingenannot/commands/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,7 +18,8 @@
 from ingenannot.commands.isoform_ranking import IsoformRanking
 from ingenannot.commands.rescue_effectors import RescueEffectors
 from ingenannot.commands.add_sqanti3_isoforms import AddSqanti3Isoforms
 from ingenannot.commands.effector_predictor_cmd import EffectorPredictorCmd
 from ingenannot.commands.exonerate_to_gff import ExonerateToGff
 from ingenannot.commands.rename import Rename
 from ingenannot.commands.clusterize import Clusterize
+from ingenannot.commands.curation import Curation
```

### Comparing `ingenannot-0.0.7/ingenannot/commands/add_sqanti3_isoforms.py` & `ingenannot-0.0.8/ingenannot/commands/add_sqanti3_isoforms.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/commands/aed_compare.py` & `ingenannot-0.0.8/ingenannot/commands/aed_compare.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,30 @@
 #!/usr/bin/env python3
 
+'''This module contains AEDCompare class'''
+
 import logging
 import numpy as np
 import pandas as pd
 from ingenannot.utils import Utils
 from ingenannot.utils.graphics import Graphics
 from ingenannot.utils.statistics import Statistics
 from ingenannot.commands.command import Command
 
 
 class AEDCompare(Command):
+    '''
+    The AEDCompare is a Command running AED comparison.
+
+    Attributes:
+    -----------
+    fof : list of files to compare
+    statistics : perfom statistics
+    ncol : number of columns in graph legend
+    '''
 
     def __init__(self, args):
 
         self.fof = args.fof
         self.statistics = args.statistics
         self.ncol = 6
 
@@ -33,15 +44,18 @@
         return 0
 
     def perform_stats(self, sources, genes):
         """run statistics"""
 
         logging.info("Running statistics")
 
-        dfstats = pd.DataFrame(columns=['mean (tr)','median (tr)','stdev (tr)','mean (pr)','median (pr)','stdev (pr)', 'median_geom_x','median_geom_y','mean_distance', 'mean_distance_to_0','median_distance', 'median_distance_to_0'],index=sources, dtype='float64')
+        dfstats = pd.DataFrame(columns=['mean (tr)','median (tr)','stdev (tr)',
+            'mean (pr)','median (pr)','stdev (pr)', 'median_geom_x','median_geom_y',
+            'mean_distance', 'mean_distance_to_0','median_distance',
+            'median_distance_to_0'],index=sources, dtype='float64')
         for src in sources:
             # extract data
             aed_scores_tmp = []
             for gene in [x for x in genes if x.source == src]:
                 for trans in gene.lTranscripts:
                     aed_scores_tmp.append((trans.best_tr_evidence[1],trans.best_bx_evidence[1]))
             aed_scores = np.array([[i[0] for i in aed_scores_tmp],[i[1] for i in aed_scores_tmp]])
@@ -57,14 +71,17 @@
             dfstats['stdev (tr)'][src] = round(std[0],3)
             dfstats['stdev (pr)'][src] = round(std[1],3)
 
             # geometric median
             geom_median = Statistics.geometric_median(aed_scores)
             dfstats['median_geom_x'][src] = round(geom_median[0],3)
             dfstats['median_geom_y'][src] = round(geom_median[1],3)
-            dfstats['mean_distance'][src] = round(Statistics.mean_median_distance(aed_scores, geom_median)[0],3) 
-            dfstats['mean_distance_to_0'][src] = round(Statistics.mean_median_distance(np.array([[0],[0]]), geom_median)[0],3) 
-            dfstats['median_distance'][src] = round(Statistics.mean_median_distance(aed_scores, geom_median)[1],3) 
-            dfstats['median_distance_to_0'][src] = round(Statistics.mean_median_distance(np.array([[0],[0]]), geom_median)[1],3) 
-
+            dfstats['mean_distance'][src] = round(Statistics.mean_median_distance(aed_scores,
+                geom_median)[0],3)
+            dfstats['mean_distance_to_0'][src] = round(Statistics.mean_median_distance(
+                np.array([[0],[0]]), geom_median)[0],3)
+            dfstats['median_distance'][src] = round(Statistics.mean_median_distance(aed_scores,
+                geom_median)[1],3)
+            dfstats['median_distance_to_0'][src] = round(Statistics.mean_median_distance(
+                np.array([[0],[0]]), geom_median)[1],3)
 
         return dfstats
```

### Comparing `ingenannot-0.0.7/ingenannot/commands/clusterize.py` & `ingenannot-0.0.8/ingenannot/commands/clusterize.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/commands/compare.py` & `ingenannot-0.0.8/ingenannot/commands/compare.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/commands/effector_predictor_cmd.py` & `ingenannot-0.0.8/ingenannot/commands/effector_predictor_cmd.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/commands/exonerate_to_gff.py` & `ingenannot-0.0.8/ingenannot/commands/exonerate_to_gff.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/commands/filter.py` & `ingenannot-0.0.8/ingenannot/commands/filter.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/commands/isoform_ranking.py` & `ingenannot-0.0.8/ingenannot/commands/isoform_ranking.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,44 @@
 #!/usr/bin/env python3
 
+'''This module contains IsoformRanking class'''
+
 import logging
-import math
 import re
-import pysam
 import multiprocessing
 
 from distutils.util import strtobool
-import numpy as np
 from collections import OrderedDict
 from collections import Counter
 from pathlib import Path
 
+import numpy as np
+import pysam
+
 from ingenannot.commands.command import Command
 from ingenannot.utils import Utils
 
 class IsoformRanking(Command):
+    '''
+    The AED is a Command running AED annotation.
 
+    Attributes:
+    -----------
+    gff_transcripts : Gff_transcripts
+    bam : bam
+    prefix : prefix
+    paired : paired
+    stranded : stranded
+    sj_threshold : sj_threshold
+    cov_threshold : cov_threshold
+    alt_threshold : alt_threshold
+    rescue : rescue
+    sj_full : sj_full
+    bam_fof : fof
+    '''
 
     def __init__(self, args):
 
         self.gff_transcripts = args.Gff_transcripts
         self.bam = args.bam
         self.prefix = args.prefix
         self.paired = args.paired
@@ -28,215 +46,200 @@
         self.sj_threshold = args.sj_threshold
         self.cov_threshold = args.cov_threshold
         self.alt_threshold = args.alt_threshold
         self.rescue = args.rescue
         self.sj_full = args.sj_full
         self.bam_fof = args.fof
 
-
     def get_intron_coordinates(self, tr):
-        """
-        todo
-        """
+        '''Return intron coordinates'''
 
         introns = []
         for i,e in enumerate(tr.lExons[:-1]):
             introns.append((e.end+1,tr.lExons[i+1].start-1))
 
         return introns
 
+    def get_support_junction(self,chrom,start,end,strand,bam_file,paired,stranded,transcripts):
+        '''Get support of annotated junctions'''
 
-    def get_support_junction(self,chr,start,end,strand,bam_file,paired,stranded,transcripts):
-
-        junctions = self.junction_counter(chr,start,end,strand,bam_file,paired,stranded)
+        junctions = self.junction_counter(chrom,start,end,strand,bam_file,paired,stranded)
         junctions = self._remove_spurious_junctions_not_in_annotations(junctions,transcripts)
-        for j in junctions:
-            nb_start = self.base_counter(chr,j[0]-2,j[0]-1,strand,bam_file,paired, stranded)
-            nb_stop = self.base_counter(chr,j[1]+1,j[1]+2,strand,bam_file,paired, stranded)
-            ratio = (junctions[j]/nb_start + junctions[j]/nb_stop)/2
-            #print(j[0], j[1],junctions[j], ratio, nb_start, nb_stop)
-            junctions[j] = (junctions[j],ratio)
+        for junc, counts in junctions.items():
+            nb_start = self.base_counter(chrom,junc[0]-2,junc[0]-1,strand,bam_file,paired, stranded)
+            nb_stop = self.base_counter(chrom,junc[1]+1,junc[1]+2,strand,bam_file,paired, stranded)
+            ratio = (counts/nb_start + counts/nb_stop)/2
+            junctions[junc] = (counts,ratio)
         return junctions
 
-
-    def base_counter(self,chr,start,end,strand, bam_file, paired, stranded):
-        """
-        getting all reads crossing this position, in a SJ
-        or not.
-        """
-
+    def base_counter(self,chrom,start,end,strand, bam_file, paired, stranded):
+        '''Get all reads crossing this position, in a SJ or not.'''
 
         reads = []
         sam_file = pysam.AlignmentFile(bam_file, "rb")
 
         if stranded:
             if paired:
                 if strand == -1:
-                    reads = [read for read in sam_file.fetch(chr,start,end) if (read.is_reverse and read.is_read2 and read.is_proper_pair and not read.is_secondary and not read.is_supplementary) or (not read.is_reverse and read.is_read1 and read.is_proper_pair and not read.is_secondary and not read.is_supplementary)]
+                    reads = [read for read in sam_file.fetch(chrom,start,end)
+                            if (read.is_reverse and read.is_read2 and read.is_proper_pair
+                                and not read.is_secondary and not read.is_supplementary)
+                            or (not read.is_reverse and read.is_read1 and read.is_proper_pair
+                                and not read.is_secondary and not read.is_supplementary)]
                 else:
-                    reads = [read for read in sam_file.fetch(chr,start,end) if (read.is_reverse and read.is_read1 and read.is_proper_pair and not read.is_secondary and not read.is_supplementary) or (not read.is_reverse and read.is_read2 and read.is_proper_pair and not read.is_secondary and not read.is_supplementary)]
+                    reads = [read for read in sam_file.fetch(chrom,start,end)
+                            if (read.is_reverse and read.is_read1 and read.is_proper_pair
+                                and not read.is_secondary and not read.is_supplementary)
+                            or (not read.is_reverse and read.is_read2 and read.is_proper_pair
+                                and not read.is_secondary and not read.is_supplementary)]
             else: #single
                 if strand == -1:
-                    reads = [read for read in sam_file.fetch(chr,start,end) if not read.is_reverse and not read.is_secondary and not read.is_supplementary]
+                    reads = [read for read in sam_file.fetch(chrom,start,end)
+                            if not read.is_reverse and not read.is_secondary
+                            and not read.is_supplementary]
                 else:
-                    reads = [read for read in sam_file.fetch(chr,start,end) if read.is_reverse and not read.is_secondary and not read.is_supplementary]
+                    reads = [read for read in sam_file.fetch(chrom,start,end)
+                            if read.is_reverse and not read.is_secondary
+                            and not read.is_supplementary]
         else:
             if paired:
-                reads = [read for read in sam_file.fetch(chr,start,end)if not read.is_secondary and not read.is_supplementary and read.is_proper_pair]
+                reads = [read for read in sam_file.fetch(chrom,start,end)
+                        if not read.is_secondary and not read.is_supplementary
+                        and read.is_proper_pair]
             else:
-                reads = [read for read in sam_file.fetch(chr,start,end) if not read.is_secondary and not read.is_supplementary]
+                reads = [read for read in sam_file.fetch(chrom,start,end)
+                        if not read.is_secondary and not read.is_supplementary]
 
         return len(reads)
 
-
-
-
-    def junction_counter(self,chr,start,end,strand, bam_file, paired, stranded):
+    def junction_counter(self,chrom,start,end,strand, bam_file, paired, stranded):
+        '''get count per junction'''
 
         junctions = None
         sam_file = pysam.AlignmentFile(bam_file, "rb")
         if stranded:
             if paired:
                 if strand == -1:
-                    junctions = sam_file.find_introns((read for read in sam_file.fetch(chr,start,end) if (read.is_reverse and read.is_read2 and read.is_proper_pair and not read.is_secondary and not read.is_supplementary) or (not read.is_reverse and read.is_read1 and read.is_proper_pair and not read.is_secondary and not read.is_supplementary) ))
+                    junctions = sam_file.find_introns((
+                        read for read in sam_file.fetch(chrom,start,end)
+                        if (read.is_reverse and read.is_read2 and read.is_proper_pair
+                            and not read.is_secondary and not read.is_supplementary)
+                        or (not read.is_reverse and read.is_read1 and read.is_proper_pair
+                            and not read.is_secondary and not read.is_supplementary) ))
                 else:
-                    junctions = sam_file.find_introns((read for read in sam_file.fetch(chr,start,end) if (read.is_reverse and read.is_read1 and read.is_proper_pair and not read.is_secondary and not read.is_supplementary) or (not read.is_reverse and read.is_read2 and read.is_proper_pair and not read.is_secondary and not read.is_supplementary) ))
-
+                    junctions = sam_file.find_introns((
+                        read for read in sam_file.fetch(chrom,start,end)
+                        if (read.is_reverse and read.is_read1 and read.is_proper_pair
+                            and not read.is_secondary and not read.is_supplementary)
+                        or (not read.is_reverse and read.is_read2 and read.is_proper_pair
+                            and not read.is_secondary and not read.is_supplementary) ))
             else: #single
                 if strand == -1:
-                    junctions = sam_file.find_introns((read for read in sam_file.fetch(chr,start,end) if not read.is_reverse and not read.is_secondary and not read.is_supplementary))
+                    junctions = sam_file.find_introns((
+                        read for read in sam_file.fetch(chrom,start,end)
+                        if not read.is_reverse and not read.is_secondary
+                        and not read.is_supplementary))
                 else:
-                    junctions = sam_file.find_introns((read for read in sam_file.fetch(chr,start,end) if read.is_reverse and not read.is_secondary and not read.is_supplementary))
+                    junctions = sam_file.find_introns((
+                        read for read in sam_file.fetch(chrom,start,end)
+                        if read.is_reverse and not read.is_secondary
+                        and not read.is_supplementary))
         else:
             if paired:
-                junctions = sam_file.find_introns((read for read in sam_file.fetch(chr,start,end)if not read.is_secondary and not read.is_supplementary and read.is_proper_pair))
+                junctions = sam_file.find_introns((
+                    read for read in sam_file.fetch(chrom,start,end)
+                    if not read.is_secondary and not read.is_supplementary and read.is_proper_pair))
             else:
-                junctions = sam_file.find_introns((read for read in sam_file.fetch(chr,start,end) if not read.is_secondary and not read.is_supplementary))
+                junctions = sam_file.find_introns((
+                    read for read in sam_file.fetch(chrom,start,end)
+                    if not read.is_secondary and not read.is_supplementary))
 
-#        print(junctions)
         return junctions
 
-
     def rank_junctions(self, junctions):
+        '''rank junction per coverage'''
 
-        return OrderedDict({j[0]:j[1] for j in sorted(junctions.items(), key=lambda x: x[1][1], reverse=True) if j[1][1] > self.sj_threshold})
-
-
-#    def _junction_overlap(self, d1,d2):
-
-#        if (d1[0] > d2[0] and d1[0] < d2[1]) or (d1[1] > d2[0] and d1[1] < d2[1]):
-#            return True
-#        else:
-#            return False
-
+        return OrderedDict({j[0]:j[1] for j in sorted(junctions.items(),
+            key=lambda x: x[1][1], reverse=True) if j[1][1] > self.sj_threshold})
 
     def get_top_expressed_based_on_shared_SJ(self, transcripts, junctions):
+        '''get expression level based on junction support'''
 
         scores_all = {tr.id:[] for tr in transcripts}
         nb_shared_junctions = 0
-#        print(junctions)
         for i,j in enumerate(junctions):
             shared_junction = True
             tr_validate = []
 
             for tr in transcripts:
                 if self.sj_full:
-#                    print("ici")
                     if not (j[0] > tr.start and j[1] < tr.end):
                         shared_junction = False
-#                        print("la")
                         break
                 else:
-#                    print("ici2")
-#                    if (j[0] > tr.start and j[1] < tr.end) or (j[0] > tr.start and j[1] > tr.end) or (j[0]< tr.start and j[1] < tr.end):
-                    if (j[0] > tr.start and j[1] < tr.end) or (j[0] > tr.start and j[0]<tr.end and j[1] > tr.end) or (j[0]< tr.start and j[1] > tr.start and j[1] < tr.end):
+                    if (j[0] > tr.start and j[1] < tr.end)\
+                    or (j[0] > tr.start and j[0]<tr.end and j[1] > tr.end)\
+                    or (j[0]< tr.start and j[1] > tr.start and j[1] < tr.end):
                         pass
                     else:
                         shared_junction = False
                         break
 
             if shared_junction:
                 nb_shared_junctions += 1
                 for tr in transcripts:
                     if (j[0]+1,j[1]) in self.get_intron_coordinates(tr):
-                        logging.debug("intron {} found in {} {}".format(j, tr.id, self.get_intron_coordinates(tr)))
+                        logging.debug(f"intron {j} found in {tr.id}"
+                        f"{self.get_intron_coordinates(tr)}")
                         scores_all[tr.id].append(junctions[j][1])
                     else:
-                        logging.debug("intron {} not found in {} {}".format(j, tr.id, self.get_intron_coordinates(tr)))
+                        logging.debug(f"intron {j} not found in {tr.id}"
+                        f"{self.get_intron_coordinates(tr)}")
                         overlapping_junctions = []
                         for ju in junctions:
                             if (ju[0]!= j[0]) or (ju[1] != j[1]):
-                                if (ju[0]<j[0] and ju[1]>j[1]) or (ju[0]>j[0] and ju[1]<j[1]) or (ju[0]>=j[0] and ju[0]<j[1]) or (ju[1]<=j[1] and ju[1]>j[0]):
-                                   overlapping_junctions.append(ju)
+                                if (ju[0]<j[0] and ju[1]>j[1]) \
+                                or (ju[0]>j[0] and ju[1]<j[1]) \
+                                or (ju[0]>=j[0] and ju[0]<j[1]) \
+                                or (ju[1]<=j[1] and ju[1]>j[0]):
+                                    overlapping_junctions.append(ju)
                         if overlapping_junctions:
-#                            print ("overalpping junction for {}".format(j))
                             injunction = []
                             for jo in overlapping_junctions:
                                 if (jo[0]+1, jo[1]) in self.get_intron_coordinates(tr):
                                     injunction.append(junctions[jo][1])
                             if not injunction:
-#                                print(junctions[j][1])
-#                                print([junctions[jo][1] for jo in overlapping_junctions])
-
-                                total = sum([junctions[jo][1] for jo in overlapping_junctions]) + junctions[j][1]
+                                total = sum(junctions[jo][1] for jo
+                                    in overlapping_junctions) + junctions[j][1]
                                 scores_all[tr.id].append(max(1-total,0))
                             else:
                                 scores_all[tr.id].append(min(injunction))
 
                         if not overlapping_junctions:
-#                            print ("no overalpping junction for {}".format(j))
                             scores_all[tr.id].append(1-junctions[j][1])
-
-
-#        print(scores_all)
         if nb_shared_junctions:
             mean = {}
             max_mean = 0
             for tr_id in scores_all:
-#               mean[tr_id] = np.mean(scores_all[tr_id])
-#               mean[tr_id] = min(scores_all[tr_id])
-               mean[tr_id] = (min(scores_all[tr_id]),np.mean(scores_all[tr_id]))
-               #max_mean = max(mean[tr_id],max_mean)
-#            print(mean)
-#               print(tr_id, mean[tr_id], scores_all[tr_id])
+                mean[tr_id] = (min(scores_all[tr_id]),np.mean(scores_all[tr_id]))
             classif = []
             alternatives_filtered = []
             for m in sorted(set(mean.values()), reverse=True):
                 classif_mean = []
                 for tr in transcripts:
                     if mean[tr.id] == m:
                         classif_mean.append(tr)
                         if m[0] < self.alt_threshold:
                             alternatives_filtered.append(tr.id)
                 classif.append(classif_mean)
             return classif, alternatives_filtered
-        else:
-            return [transcripts], []
-
-
-
-#    def get_exon_coverage(self, transcripts, bam):
-#
-#        samfile = pysam.AlignmentFile(bam, "r")
-#
-#         # get all exons to compute one time coverage
-#        exon_coverage = {}
-#        seqid = transcripts[0][0].seqid
-#        self.working_tr_strand = transcripts[0][0].strand
-#        for g_tr in transcripts:
-#            for tr in g_tr:
-#                for ex in sorted(tr.lExons,key=lambda x: x.start):
-#                    exon_coverage[(ex.start-1,ex.end)] = 0
-#        for ex in exon_coverage:
-#            cov =  samfile.count_coverage(seqid,ex[0],ex[1], read_callback=self.callback_filter_read)
-#            exon_coverage[ex] = list(map(sum, zip(cov[0],cov[1],cov[2],cov[3])))
-#        return exon_coverage
-#
+        return [transcripts], []
 
     def new_get_exon_coverage(self, transcripts, bam):
+        '''get exon coverage'''
 
         samfile = pysam.AlignmentFile(bam, "r")
 
          # get all exons to compute one time coverage
         exon_coverage = {}
         seqid = transcripts[0][0].seqid
         self.working_tr_strand = transcripts[0][0].strand
@@ -254,21 +257,20 @@
         cov =  samfile.count_coverage(seqid,start, end, read_callback=self.callback_filter_read)
         pos_cov = list(map(sum, zip(cov[0],cov[1],cov[2],cov[3])))
         for ex in exon_coverage:
             exon_coverage[ex] = pos_cov[ex[0]-start:ex[1]-start]
 
         return exon_coverage
 
-
     def get_top_expressed_based_on_coverage(self, transcripts, exon_coverage, idx):
+        '''get top expressed transcript based oncoverage'''
 
         ranked_tr = []
         unranked_tr = []
 
-
         start = min([x.get_min_exon_start() for x in transcripts])
         end = max([x.get_max_exon_end() for x in transcripts])
         tr_positions = []
 
 
         # get coverage for each transcript/exons
         for tr in transcripts:
@@ -279,488 +281,405 @@
             tr_positions.append(positions)
 
         # compute mean coverage on shared bases
         shared_bases = []
         for pos in range(start-1,end):
             shared = True
             for i,tr in enumerate(transcripts):
-                if tr_positions[i][pos] == None:
+                if tr_positions[i][pos] is None:
                     shared = False
                     break
             if shared:
                 shared_bases.append(tr_positions[0][pos])
 
         # shared bases null if fragmented isoform, non overlaping
         if len(shared_bases) == 0:
-            logging.debug("rescue shared bases for {}".format(transcripts[0].gene_id))
-            shared_bases = self.rescue_shared_bases_non_overlapping_isoforms(transcripts, tr_positions, start, end)
+            logging.debug(f"rescue shared bases for {transcripts[0].gene_id}")
+            shared_bases = self.rescue_shared_bases_non_overlapping_isoforms(
+                    transcripts, tr_positions, start, end)
 
         median = np.median(shared_bases)
         threshold = median * self.cov_threshold
 
         if median == 0:
             unranked_tr = transcripts
             return ranked_tr, unranked_tr
 
         scores = {}
 
         for i,tr in enumerate(transcripts):
             positions = []
             for ex in sorted(tr.lExons,key=lambda x: x.start):
                 positions.extend(range(ex.start-1,ex.end))
-            score = len([tr_positions[i][x] for x in positions if tr_positions[i][x] > threshold]) - \
-                    len([tr_positions[i][x] for x in positions if tr_positions[i][x] < threshold])
+            score = len([tr_positions[i][x] for x in positions \
+                        if tr_positions[i][x] > threshold]) -  \
+                    len([tr_positions[i][x] for x in positions \
+                        if tr_positions[i][x] < threshold])
             scores[tr.id] = score
 
 
         for i,s in enumerate(sorted(set(scores.values()), reverse=True)):
             for tr in transcripts:
                 if scores[tr.id] == s:
                     # add median cov for weigth sum in case multiple bam
                     # add idx + rank for weigh in case multiple bam
                     ranked_tr.append((tr,median,idx+i*0.01))
 
         return ranked_tr, unranked_tr
 
-
-
-
     def rescue_shared_bases_non_overlapping_isoforms(self, transcripts, tr_positions, start, end):
+        '''todo'''
 
         shared_bases = [None]*(end-start+1)
         shared_nb_transcripts = [0]*(end-start+1)
         for i,pos in enumerate(range(start-1,end)):
             for j,tr in enumerate(transcripts):
-                if tr_positions[j][pos] !=  None:
+                if tr_positions[j][pos] is not None:
                     shared_nb_transcripts[i] += 1
                     shared_bases[i] = tr_positions[j][pos]
         max_tr = max(shared_nb_transcripts)
         return [x for i,x in enumerate(shared_bases) if shared_nb_transcripts[i] == max_tr]
 
     def callback_filter_read(self,read):
-        """
+        '''
            callback function to filter count_coverage
            pysam function. Take into account, pairing and
            strand specificity
-        """
-
+        '''
 
         if self.working_bam_is_stranded:
             if self.working_bam_is_paired:
                 if self.working_tr_strand == -1:
-                    if (read.is_reverse and read.is_read2) or ((not read.is_reverse) and read.is_read1):
+                    if (read.is_reverse and read.is_read2) \
+                    or ((not read.is_reverse) and read.is_read1):
                         return True
                 else:
-                    if (read.is_reverse and read.is_read1) or ((not read.is_reverse) and read.is_read2):
+                    if (read.is_reverse and read.is_read1) \
+                    or ((not read.is_reverse) and read.is_read2):
                         return True
             else: #single
                 if self.working_tr_strand == -1:
-                     if not read.is_reverse :
-                         return True
+                    if not read.is_reverse :
+                        return True
                 else:
-                     if read.is_reverse :
-                         return True
+                    if read.is_reverse :
+                        return True
         else:
             return True
         return False
 
-
-
     def get_bam_files_to_analyze(self):
-        """
+        '''
         return the list of bam files
         to analyze
-        """
+        '''
 
         bams = []
 
         if self.bam_fof:
             with open(self.bam_fof, 'r') as f:
                 for line in f:
                     if not re.match("^#",line):
                         values = line.rstrip().split("\t")
                         fh = values[0]
                         if not Path(fh).is_file():
-                            logging.error("Problem conf, Missing bam file: {}".format(fh))
-                            raise Exception("Missing bam file: {}".format(fh))
-                        if not Path("{}.bai".format(fh)).is_file():
-                            logging.error("Problem conf, Missing index (.bai) of bam file: {}".format(fh))
-                            raise Exception("Missing index (.bai) of bam file: {}".format(fh))
+                            logging.error(f"Problem conf, Missing bam file: {fh}")
+                            raise Exception(f"Missing bam file: {fh}")
+                        if not Path(f"{fh}.bai").is_file():
+                            logging.error(f"Problem conf, Missing index (.bai) of bam file: {fh}")
+                            raise Exception(f"Missing index (.bai) of bam file: {fh}")
                         paired = bool(strtobool(values[1]))
                         stranded = bool(strtobool(values[2]))
                         bams.append((fh,paired,stranded))
         elif self.bam:
             if not Path(self.bam).is_file():
-                logging.error("Problem conf, Missing bam file: {}".format(self.bam))
-                raise Exception("Missing bam file: {}".format(self.bam))
-            if not Path("{}.bai".format(self.bam)).is_file():
-                logging.error("Problem conf, Missing index (.bai) of bam file: {}".format(self.bam))
-                raise Exception("Missing index (.bai) of bam file: {}".format(self.bam))
+                logging.error(f"Problem conf, Missing bam file: {self.bam}")
+                raise Exception(f"Missing bam file: {self.bam}")
+            if not Path(f"{self.bam}.bai").is_file():
+                logging.error(f"Problem conf, Missing index (.bai) of bam file: {self.bam}")
+                raise Exception(f"Missing index (.bai) of bam file: {self.bam}")
             bams.append((self.bam,self.paired,self.stranded))
         else:
             raise Exception("Missing at least one bam file to analyze")
 
-        logging.info("{} bam files to analyze".format(len(bams)))
+        logging.info(f"{len(bams)} bam files to analyze")
 
         return bams
 
     def _remove_spurious_junctions_not_in_annotations(self, junctions,transcripts):
+        '''remove new annotations not in assembled transcripts'''
 
         introns = []
         selected_junctions = {}
         for tr in transcripts:
             introns.extend([(i[0]-1, i[1]) for i in self.get_intron_coordinates(tr)])
         for j in junctions:
             if j in introns:
                 selected_junctions[j] = junctions[j]
         return selected_junctions
 
     def ranking_transcripts(self, genes, bam_file, paired, stranded):
+        '''rank transcripts'''
 
-#            top_selected_transcripts = []
-            ranked_transcripts = []
-            ranked_transcripts_raw = []
-            unclassified_transcripts = []
-            alternatives_transcripts_filtered = []
-            for g in genes:
-#            for g in genes[0:100]:
-                logging.debug("ranking gene {}".format(g.gene_id))
-                junctions = self.get_support_junction(g.seqid,g.start,g.end,g.strand,bam_file, paired, stranded,g.lTranscripts)
-#                print(junctions)
-                # remove junctions without enough support
-                junctions = self.rank_junctions(junctions)
-
-                transcripts = [] # list of working transcripts
-                untranscripts = [] # list of working unclassified transcripts
-#                junctions = self.remove_spurious_junctions_not_in_annotations(junctions,g.lTranscripts)
-                # remove transcript if less supported than RNA-seq !!! bad iso !
-                for tr in g.lTranscripts:
-                   introns = self.get_intron_coordinates(tr)
-                   introns_status_ok = True
-                   for i in introns:
-                       if (i[0]-1, i[1]) not in junctions:
-                           logging.debug("transcript {} not ranked, introns not supported with rna-seq data".format(tr.id))
-                           introns_status_ok = False
-                   if introns_status_ok:
-                       transcripts.append(tr)
-                   else:
-                       untranscripts.append(tr)
-
-
-#                print(junctions)
-                # rescue transcripts if no transcripts selected with introns (ex 2 introns, 1 not supported)
-                if self.rescue and len(transcripts) == 0:
-                    logging.debug("No transcripts \"junction reliable\" for gene {}, all transcripts rescued".format(g.gene_id))
-                    transcripts = g.lTranscripts
-                    untranscripts = []
-
-                if len(transcripts) == 0: # no reliable transcript and no rescue
-                    unclassified_transcripts.append(untranscripts)
-                    continue
-                top_transcripts_intermediate, alternatives_filtered = self.get_top_expressed_based_on_shared_SJ(transcripts,junctions)
-#                if len(top_transcripts_intermediate) == 0: # transcript with major splicing
-    #                continue
-    #            print("OK 1")
-#                    print(transcripts)
-#                    seqid = top_transcripts_intermediate[0][0].seqid
-                alternatives_transcripts_filtered.extend(alternatives_filtered)
-                alternatives_transcripts_filtered.extend([t.id for t in untranscripts])
-                #print("bam")
-               # print(alternatives_transcripts_filtered)
-               # print([t.id for t in untranscripts])
-               # print(top_transcripts_intermediate)
-
-
-                exon_coverage = self.new_get_exon_coverage(top_transcripts_intermediate, bam_file)
-
-                g_ranked_tr = []
-                g_ranked_tr_raw = []
-                for idx,group_tr in enumerate(top_transcripts_intermediate):
-                    #gr_ranked_tr = self.get_top_expressed_based_on_coverage(group_tr, bam_file)
-#                    print(idx, [tr.id for tr in group_tr])
-
-    #                print("OK GR {}".format(i))
-#                    ranked_tr, unranked_tr = self.get_top_expressed_based_on_coverage(group_tr, bam_file)
-                    ranked_tr, unranked_tr = self.get_top_expressed_based_on_coverage(group_tr, exon_coverage, idx)
-                    g_ranked_tr.extend(ranked_tr)
-                    g_ranked_tr_raw.append(ranked_tr)
-                    untranscripts.extend(unranked_tr)
-    #            print("OK 2")
-
-#                selected_tr = None
-#                if len(top_transcripts_intermediate) > 1:
-#                    selected_tr = self.get_top_expressed_based_on_coverage(top_transcripts_intermediate, bam_file)
-#                else:
-#                    selected_tr = top_transcripts_intermediate[0]
-
-#                logging.debug("selected {} as best transcript for gene {}".format(selected_tr.id, g.gene_id))
-#                top_selected_transcripts.append(selected_tr)
-                if g_ranked_tr:
-                    logging.debug("selected {} as best transcript for gene {}".format(g_ranked_tr[0][0].id, g.gene_id))
-                ranked_transcripts.append(g_ranked_tr)
-                ranked_transcripts_raw.append(g_ranked_tr_raw)
-                unclassified_transcripts.append(untranscripts)
-#            return top_selected_transcripts
+        ranked_transcripts = []
+        ranked_transcripts_raw = []
+        unclassified_transcripts = []
+        alternatives_transcripts_filtered = []
+        for g in genes:
+            logging.debug(f"ranking gene {g.gene_id}")
+            junctions = self.get_support_junction(
+                    g.seqid,g.start,g.end,g.strand,bam_file, paired, stranded,g.lTranscripts)
+            # remove junctions without enough support
+            junctions = self.rank_junctions(junctions)
+
+            transcripts = [] # list of working transcripts
+            untranscripts = [] # list of working unclassified transcripts
+            # remove transcript if less supported than RNA-seq !!! bad iso !
+            for tr in g.lTranscripts:
+                introns = self.get_intron_coordinates(tr)
+                introns_status_ok = True
+                for i in introns:
+                    if (i[0]-1, i[1]) not in junctions:
+                        logging.debug(f"transcript {tr.id} not ranked,"
+                        f"introns not supported with rna-seq data")
+                        introns_status_ok = False
+                if introns_status_ok:
+                    transcripts.append(tr)
+                else:
+                    untranscripts.append(tr)
 
-            #print(ranked_transcripts)
-            return ranked_transcripts, unclassified_transcripts, ranked_transcripts_raw, alternatives_transcripts_filtered
+            # rescue transcripts if no transcripts selected
+            # with introns (ex 2 introns, 1 not supported)
+            if self.rescue and len(transcripts) == 0:
+                logging.debug(f"No transcripts \"junction reliable\" for gene {g.gene_id},"
+                              f"all transcripts rescued")
+                transcripts = g.lTranscripts
+                untranscripts = []
 
+            if len(transcripts) == 0: # no reliable transcript and no rescue
+                unclassified_transcripts.append(untranscripts)
+                continue
+            top_transcripts_intermediate, alternatives_filtered = \
+                    self.get_top_expressed_based_on_shared_SJ(transcripts,junctions)
+            alternatives_transcripts_filtered.extend(alternatives_filtered)
+            alternatives_transcripts_filtered.extend([t.id for t in untranscripts])
+
+            exon_coverage = self.new_get_exon_coverage(top_transcripts_intermediate, bam_file)
+
+            g_ranked_tr = []
+            g_ranked_tr_raw = []
+            for idx,group_tr in enumerate(top_transcripts_intermediate):
+                ranked_tr, unranked_tr = \
+                        self.get_top_expressed_based_on_coverage(group_tr, exon_coverage, idx)
+                g_ranked_tr.extend(ranked_tr)
+                g_ranked_tr_raw.append(ranked_tr)
+                untranscripts.extend(unranked_tr)
+            if g_ranked_tr:
+                logging.debug(f"selected {g_ranked_tr[0][0].id}"
+                              f"as best transcript for gene {g.gene_id}")
+            ranked_transcripts.append(g_ranked_tr)
+            ranked_transcripts_raw.append(g_ranked_tr_raw)
+            unclassified_transcripts.append(untranscripts)
+
+        return ranked_transcripts, unclassified_transcripts,\
+               ranked_transcripts_raw, alternatives_transcripts_filtered
 
     def run(self):
 
-        """
+        '''
         Suppose file with gene_id and transcript_id
         no clustering. Selection /ranking at tr level for
         each gene
-        """
+        '''
 
         bam_files = self.get_bam_files_to_analyze()
 
         genes = Utils.extract_genes(self.gff_transcripts)
-        references = set([g.seqid for g in genes])
-
-#        genes = genes[231:233]
-
         ranked_transcripts = []
         ranked_transcripts_raw = []
         unclassified_transcripts = []
         alternatives_transcripts_filtered = []
         for bam in bam_files:
 
             ranked_transcripts_bam = []
             ranked_transcripts_raw_bam = []
             unclassified_transcripts_bam = []
             alternatives_transcripts_filtered_bam = []
             self.working_bam_is_paired = bam[1]
             self.working_bam_is_stranded = bam[2]
-            logging.info("Analyzing bam file: {}, paired: {}, stranded: {}".format(bam[0],bam[1],bam[2]))
+            logging.info("Analyzing bam file: {bam[0]}, paired: {bam[1]}, stranded: {bam[2]}")
 
             if Command.NB_CPUS > 1:
                 ratio = 100
                 if len(genes) < 100:
                     ratio = 5
-                logging.info("{} subprocesses to run:".format(len(range(0,len(genes),ratio))))
+                logging.info(f"{len(range(0,len(genes),ratio))} subprocesses to run:")
                 pool = multiprocessing.Pool(Command.NB_CPUS)
-                results = [pool.apply_async(self.ranking_transcripts, (genes[i:i + ratio], bam[0], bam[1], bam[2])) for idx,i in enumerate(range(0, len(genes), ratio))]
+                results = [pool.apply_async(self.ranking_transcripts,\
+                        (genes[i:i + ratio], bam[0], bam[1], bam[2]))\
+                        for idx,i in enumerate(range(0, len(genes), ratio))]
                 for i,r in enumerate(results):
                     r_ranking, r_unclassif, r_ranking_raw, r_alt_filtered = r.get()
-                    logging.info("Analysis done: {}/{}".format(i+1,len(results)))
+                    logging.info(f"Analysis done: {i+1}/{len(results)}")
                     ranked_transcripts_bam.extend(r_ranking)
                     ranked_transcripts_raw_bam.extend(r_ranking_raw)
                     unclassified_transcripts_bam.extend(r_unclassif)
                     alternatives_transcripts_filtered_bam.extend(r_alt_filtered)
                 pool.close()
                 pool.join()
             else:
-                ranked_transcripts_bam, unclassified_transcripts_bam, ranked_transcripts_raw_bam, alternatives_transcripts_filtered_bam = self.ranking_transcripts(genes, bam[0], bam[1], bam[2])
+                ranked_transcripts_bam, unclassified_transcripts_bam,\
+                ranked_transcripts_raw_bam, alternatives_transcripts_filtered_bam = \
+                self.ranking_transcripts(genes, bam[0], bam[1], bam[2])
 
             ranked_transcripts.append(ranked_transcripts_bam)
             ranked_transcripts_raw.append(ranked_transcripts_raw_bam)
             unclassified_transcripts.append(unclassified_transcripts_bam)
             alternatives_transcripts_filtered.extend(alternatives_transcripts_filtered_bam)
 
         # deduplicate alternatives_transcripts_filtered and keep only if filtered in all bam
-        dedup_alternatives_transcripts_filtered = self._dedup_alt_tr(alternatives_transcripts_filtered, len(bam_files))
-        #print(dedup_alternatives_transcripts_filtered)
-
-
+        dedup_alternatives_transcripts_filtered = \
+                self._dedup_alt_tr(alternatives_transcripts_filtered, len(bam_files))
 
         if len(bam_files) > 1:
             ranked_bam_results = self.rank_separate_bam_results(genes, ranked_transcripts)
-            self.export(ranked_bam_results, "{}.ranking.gff".format(self.prefix),True)
-            self.export(ranked_bam_results, "{}.top.gff".format(self.prefix),True, True)
-            alt_iso = self.get_best_alternative_isoform(genes, ranked_transcripts_raw, dedup_alternatives_transcripts_filtered)
-            self.export(alt_iso, "{}.alternatives.gff".format(self.prefix),True)
-
-            unclassif_bam_results = self.unclassif_separate_bam_results(genes, ranked_bam_results, unclassified_transcripts)
-            self.export(unclassif_bam_results, "{}.unclassif.gff".format(self.prefix),False)
+            self.export(ranked_bam_results, f"{self.prefix}.ranking.gff",True)
+            self.export(ranked_bam_results, f"{self.prefix}.top.gff",True, True)
+            alt_iso = self.get_best_alternative_isoform(genes,\
+                    ranked_transcripts_raw, dedup_alternatives_transcripts_filtered)
+            self.export(alt_iso, f"{self.prefix}.alternatives.gff",True)
+
+            unclassif_bam_results = self.unclassif_separate_bam_results(genes,\
+                    ranked_bam_results, unclassified_transcripts)
+            self.export(unclassif_bam_results, f"{self.prefix}.unclassif.gff",False)
         else: #direct export
-            self.export(ranked_transcripts[0], "{}.ranking.gff".format(self.prefix),True)
-            self.export(ranked_transcripts[0], "{}.top.gff".format(self.prefix),True, True)
-            self.export(unclassified_transcripts[0], "{}.unclassif.gff".format(self.prefix),False)
-            alt_iso = self.get_best_alternative_isoform(genes, ranked_transcripts_raw, dedup_alternatives_transcripts_filtered)
-            self.export(alt_iso, "{}.alternatives.gff".format(self.prefix),True)
-
+            self.export(ranked_transcripts[0], f"{self.prefix}.ranking.gff",True)
+            self.export(ranked_transcripts[0], f"{self.prefix}.top.gff",True, True)
+            self.export(unclassified_transcripts[0], f"{self.prefix}.unclassif.gff",False)
+            alt_iso = self.get_best_alternative_isoform(genes, ranked_transcripts_raw,\
+                    dedup_alternatives_transcripts_filtered)
+            self.export(alt_iso, f"{self.prefix}.alternatives.gff",True)
 
         return 0
 
     def _dedup_alt_tr(self, transcripts, nb_bam):
-       
+        '''dedup transcripts'''
+
         c = Counter(transcripts)
         return [tr for tr in c if c[tr] == nb_bam]
 
-
-#    def get_best_alternative_isoform_old(self, ranked_transcripts):
-#
-#        transcripts = []
-#
-#        for bam in ranked_transcripts:
-#            for g in bam:
-#                group = []
-#                for g_tr in g:
-#                    #print(g_tr[0], "=>", len(g_tr))
-#                    if g_tr:
-#                        group.append(g_tr[0])
-#                transcripts.append(group)
-#
-#        return transcripts
-#
-    def get_best_alternative_isoform(self, genes, ranked_transcripts, alternatives_transcripts_filtered):
+    def get_best_alternative_isoform(self, genes, ranked_transcripts, \
+            alternatives_transcripts_filtered):
+        '''return ranked best isoforms'''
 
         transcripts = []
-        #print(alternatives_transcripts_filtered)
-#        for g in ranked_transcripts:
-#            for bam in g:
-#                print("bam")
-#                for ltrs in bam:
-#                   print([tr[0].id for tr in ltrs])
-
-
         if len(ranked_transcripts) == 1:
-
             for bam in ranked_transcripts:
                 for g in bam:
                     group = []
                     for g_tr in g:
-                        #print(g_tr[0], "=>", len(g_tr))
                         if g_tr and g_tr[0][0].id not in alternatives_transcripts_filtered:
                             group.append(g_tr[0])
                     transcripts.append(group)
-
             return transcripts
 
-        else:
-
-            select_ranked = []
-            rank = {g.gene_id:[] for g in genes}
+        select_ranked = []
+        rank = {g.gene_id:[] for g in genes}
+        for bam in ranked_transcripts:
+            for ltrs in bam:
+                if ltrs:
+                    if ltrs[0]:
+                        rank[ltrs[0][0][0].gene_id].append(ltrs)
+        s_ranked = {}
+        # select most supported
+        for g in rank:
+            max_coverage = -1
+            selected_ranking = None
+            for i,ltr in enumerate(rank[g]):
+                median_max_cov = -1
+                tmp_select = []
+                for u in ltr:
+                    if u:
+                        median_max_cov = max(median_max_cov,max(j[1] for j in u))
+                        tmp_select.append(u[0])
+                if median_max_cov > max_coverage and median_max_cov > -1:
+                    max_coverage = median_max_cov
+                    selected_ranking = tmp_select
+            if selected_ranking:
+                s_ranked[g] = selected_ranking
 
-            for bam in ranked_transcripts:
-                for ltrs in bam:
-                    if ltrs:
-                        if ltrs[0]:
-                            rank[ltrs[0][0][0].gene_id].append(ltrs)
-#                        print(ltrs[0])
-
-#            for g in rank:
-#                max_coverage = -1
-#                selected_ranking = None
-#                for i,ltr in enumerate(rank[g]):
-#                    print(ltr)
-
-            s_ranked = {}
-            # select most supported
-            for g in rank:
-                max_coverage = -1
-                selected_ranking = None
-                for i,ltr in enumerate(rank[g]):
-
-                    median_max_cov = -1
-                    tmp_select = []
-                    for u in ltr:
-                        if u:
-                            median_max_cov = max(median_max_cov,max([j[1] for j in u]))
-                            tmp_select.append(u[0])
-                    if median_max_cov > max_coverage and median_max_cov > -1:
-                        max_coverage = median_max_cov
-                        selected_ranking = tmp_select
-                if selected_ranking:
-#                    select_ranked.append(selected_ranking)
-                    s_ranked[g] = selected_ranking
-
-            # add new iso (need to be implemented)
-            for g in rank:
-                l_selected_tr = []
-                for i,ltr in enumerate(rank[g]):
-                    for u in ltr:
+        # add new iso (need to be implemented)
+        for g in rank:
+            l_selected_tr = []
+            for i,ltr in enumerate(rank[g]):
+                for u in ltr:
+                    if g in s_ranked:
+                        l_selected_tr = [t[0] for t in s_ranked[g]]
+                    find = False
+                    for tr in u:
+                        if tr[0].id in [t.id for t in l_selected_tr]:
+                            find = True
+                            break
+                    if find is False and len(u) > 0:
                         if g in s_ranked:
-                            l_selected_tr = [t[0] for t in s_ranked[g]]
-                        find = False
-                        for tr in u:
-#                            print(tr[0], "______", l_selected_tr)
-#                            print(tr[0] in l_selected_tr)
-                            if tr[0].id in [t.id for t in l_selected_tr]:
-#                            for t in l_selected_tr:
- #                               print(tr[0].id==t.id)
- #                               if tr[0] == t:
-                                find = True
-                                break
-                        if find == False and len(u) > 0:
-                            if g in s_ranked:
-                                s_ranked[g].append(u[0])
-                            else:
-                                s_ranked[g] = [u[0]]
-                if g in s_ranked:
-                    select_ranked.append(s_ranked[g])
-
-#
-
-
-            select_ranked_filtered = []
-            for ltr in select_ranked:
-                l = []
-                for tr in ltr:
-                    if tr[0].id not in alternatives_transcripts_filtered:
-                        l.append(tr)
-                select_ranked_filtered.append(l)
-            return select_ranked_filtered
-
+                            s_ranked[g].append(u[0])
+                        else:
+                            s_ranked[g] = [u[0]]
+            if g in s_ranked:
+                select_ranked.append(s_ranked[g])
+
+        select_ranked_filtered = []
+        for ltr in select_ranked:
+            l = []
+            for tr in ltr:
+                if tr[0].id not in alternatives_transcripts_filtered:
+                    l.append(tr)
+            select_ranked_filtered.append(l)
+        return select_ranked_filtered
 
     def unclassif_separate_bam_results(self, genes, ranked_transcripts, unclassified_transcripts):
         """
         return unclassified transcripts if unclassified in all
         bam files
         """
 
         ranked_tr = []
-#        for bam in ranked_transcripts:
-#            for ltrs in bam:
-#                for tr in ltrs:
-#                    ranked_tr.append(tr[0].id)
-#        ranked_tr_id = list(set(ranked_tr))
-
         for g in ranked_transcripts:
             for tr in g:
-                    ranked_tr.append(tr[0].id)
+                ranked_tr.append(tr[0].id)
         ranked_tr_id = list(set(ranked_tr))
 
         select_unclassified = set()
         rank = {g.gene_id:[] for g in genes}
 
         l = []
         for i,bam in enumerate(unclassified_transcripts):
-#            l = []
             for ltrs in bam:
                 for tr in ltrs:
                     l.append(tr.id)
 
-#            if i == 0:
-#                select_unclassified = set(l)
-#            else:
-#                select_unclassified = select_unclassified.intersection(set(l))
-
         select_unclassified = set(l)
-
         unclassified = []
+
         for g in genes:
             l_tr = []
             for tr in g.lTranscripts:
                 if tr.id in select_unclassified and tr.id not in ranked_tr_id:
                     l_tr.append(tr)
             unclassified.append(l_tr)
 
         return unclassified
 
-
     def rank_separate_bam_results(self, genes, ranked_transcripts):
         """
         rank the expression level based on the highest coverage
         level
         need to implement weigth based on position (available in
         ranked_transcripts, third row for each bam)
-        WARNING: need to deal with missing isoforms 
+        WARNING: need to deal with missing isoforms
         in some bams.
         """
 
         select_ranked = []
         rank = {g.gene_id:[] for g in genes}
 
         for bam in ranked_transcripts:
@@ -769,45 +688,40 @@
                     rank[ltrs[0][0].gene_id].append(ltrs)
 
 
         for g in rank:
             max_coverage = -1
             selected_ranking = None
             for i,ltr in enumerate(rank[g]):
-                median_max_cov = (max([j[1] for j in ltr]))
+                median_max_cov = (max(j[1] for j in ltr))
                 if median_max_cov > max_coverage:
                     max_coverage = median_max_cov
                     selected_ranking = ltr
             if selected_ranking:
                 select_ranked.append(selected_ranking)
-#            else:
-#                print(g)
-
         return select_ranked
 
-
-
-
     def export(self, g_transcripts, fname, classified=True, top=False):
+        '''export isoforms'''
 
         # export same CDS
         with open(fname, 'w') as f:
-            logging.info("Writing: {}".format(fname))
+            logging.info(f"Writing: {fname}")
             source = "ingenannot-isoform-ranking"
             for g_tr in g_transcripts:
                 for idx,tr_median in enumerate(g_tr):
                     if top and idx > 0:
                         break
                     if classified:
                         tr = tr_median[0] # tr and median in tuple
                         tr.source = source
-                        f.write(tr.to_gtf(atts={"gene_id":[tr.gene_id],"transcript_id":[tr.id], "rank":[str(idx+1)]}))
+                        f.write(tr.to_gtf(atts={"gene_id":[tr.gene_id],
+                            "transcript_id":[tr.id], "rank":[str(idx+1)]}))
                     else:
                         tr = tr_median # only tr
                         tr.source = source
-                        f.write(tr.to_gtf(atts={"gene_id":[tr.gene_id],"transcript_id":[tr.id], "rank":["unclassifed"]}))
+                        f.write(tr.to_gtf(atts={"gene_id":[tr.gene_id],
+                            "transcript_id":[tr.id], "rank":["unclassifed"]}))
                     for i, exon in enumerate(tr.lExons):
                         exon.source = source
                         f.write(exon.to_gtf(tr.gene_id, tr.id))
         f.close()
-
-
```

### Comparing `ingenannot-0.0.7/ingenannot/commands/rename.py` & `ingenannot-0.0.8/ingenannot/commands/rename.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,16 +143,16 @@
                                 uatts['locus_tag'] = ["{}".format(gene_id)]
                             str_atts = ''
                             for att in uatts:
                                 str_atts += '{}={};'.format(att,",".join(uatts[att]))
                             print("{}\t{}\tthree_prime_UTR\t{}\t{}\t.\t{}\t.\t{}\n".format(tr.seqid,source,utr[0],utr[1],strand,str_atts))
 
 
-                gene_ok.append(tr.gene_id)
-                mapping_gene_table[tr.gene_id] = gene_id
+                    gene_ok.append(tr.gene_id)
+                    mapping_gene_table[tr.gene_id] = gene_id
 
         if self.mapping:
             logging.info("Exporting gene mapping in mapping_gene.txt")
             with open("mapping_gene.txt", 'w') as fh:
                 fh.write("oldID\tnewID\n")
                 for k in mapping_gene_table:
                     fh.write("{}\t{}\n".format(k,mapping_gene_table[k]))
```

### Comparing `ingenannot-0.0.7/ingenannot/commands/rescue_effectors.py` & `ingenannot-0.0.8/ingenannot/commands/rescue_effectors.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/commands/select.py` & `ingenannot-0.0.8/ingenannot/commands/select.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,62 @@
 #!/usr/bin/env python3
 
+'''This module contains Select class'''
+
 import logging
-import multiprocessing
-import math
-import pysam
-import sys
-import re
-import numpy as np
-import matplotlib
-import pandas as pd
 import copy
 
-import matplotlib.pyplot as plt
-
-from matplotlib.backends.backend_agg import FigureCanvasAgg
-
 from ingenannot.utils import Utils
-from ingenannot.utils.gff_reader import GFF3Reader, GTFReader
-from ingenannot.utils.gene_builder import GeneBuilder
 from ingenannot.utils.annot_edit_distance import AnnotEditDistance
 from ingenannot.commands.command import Command
 from ingenannot.utils.graphics import Graphics
 
 class Select(Command):
+    '''
+    The Select is a Command running annotation selection.
+
+    Attributes:
+    -----------
+    fof : list of files
+    output : output file
+    clutype : clustering type
+    clustranded : clustering stranded
+    noaed : do not perform aed
+    nb_sources_filtering : nbsrc_filter
+    nbsrc_absolute : nbsrc_absolute
+    transcript_gff_file : evtr
+    transcript_gff_file_source : evtr_source
+    transcript_gff_file_stranded : evtrstranded
+    protein_gff_file : evpr
+    protein_gff_file_source : evpr_source
+    protein_gff_file_stranded : evprstranded
+    aed_tr_cds_only : aed_tr_cds_only
+    penalty_overflow : penalty_overflow
+    aedtr_filtering : aedtr
+    aedpr_filtering : aedpr
+    use_ev_lg : use_ev_lg
+    min_CDS_length : min_cds_len
+    no_partial : no_partial
+    genome_fasta_file : genome
+    longread_gff_file : longreads
+    longread_gff_file_source : longreads_source
+    longread_penalty_overflow : longread_penalty_overflow
+    gaeval : use gaeval
+    prefix : prefix
+    no_export : export
+    no_cds_overlap : do not export cds with overlap
+    '''
 
     def __init__(self, args):
 
         self.fof = args.fof
         self.output = args.Output
         self.clutype = args.clutype
         self.clustranded = args.clustranded
         self.noaed = args.noaed
-#        self.nb_sources = args.nbsrc
         self.nb_sources_filtering = args.nbsrc_filter
         self.nbsrc_absolute = args.nbsrc_absolute
         self.transcript_gff_file = args.evtr
         self.transcript_gff_file_source = args.evtr_source
         self.transcript_gff_file_stranded = args.evtrstranded
         self.protein_gff_file = args.evpr
         self.protein_gff_file_source = args.evpr_source
@@ -60,71 +81,86 @@
             raise Exception("genome in fasta format required with no_partial genes")
 
 
     def filter_metagenes_required_number_sources(self, metagenes):
         '''filter metagenes with a minimum nb of sources'''
 
         logging.info("## Filtering metagenes for a required number of sources")
-        logging.info("## required number of sources at least : {}".format(self.nbsrc_absolute))
-        logging.info("## number of metagenes before filtering of nb sources: {}".format(len(metagenes)))
+        logging.info(f"## required number of sources at least : {self.nbsrc_absolute}")
+        logging.info(f"## number of metagenes before filtering of nb sources: {len(metagenes)}")
 
         filtered_metagenes = []
         for mg in metagenes:
             if mg.get_number_of_src() >= self.nbsrc_absolute:
                 filtered_metagenes.append(mg)
 
-        logging.info("## number of metagenes after filtering of nb sources: {}".format(len(filtered_metagenes)))
+        logging.info(f"## number of metagenes after filtering of nb sources: \
+                {len(filtered_metagenes)}")
 
         return filtered_metagenes
 
 
     def _remove_small_cds_included(self, ltr):
-        '''In some cases, a small CDS was defined
+        '''
+        In some cases, a small CDS was defined
         when a longer one was predicted by another method
         This could be due to a very small fragmented transcript
         So, in case where no protein evidence support this,
         we remove the small CDS and keep the longest, if
         no penalty CDS structure
-        By default only the next tr is analyzed. This prevent 
+        By default only the next tr is analyzed. This prevent
         multi deletion of protein well supported by other method
-        Remove orphan model'''
+        Remove orphan model
+        '''
 
         new_tr = []
         for i, tr in enumerate(ltr[:-1]):
             to_keep = True
-            if tr.best_bx_evidence[1] == 1.0 and (tr.tr_penalty != 'yes' and tr.lg_penalty != 'yes') and (tr.best_tr_evidence[1] != 1.0 or tr.best_lg_evidence[1] != 1.0):
+            if tr.best_bx_evidence[1] == 1.0 and (tr.tr_penalty != 'yes' \
+                and tr.lg_penalty != 'yes') and (tr.best_tr_evidence[1] != 1.0 \
+                or tr.best_lg_evidence[1] != 1.0):
                 for tr2 in ltr[i+1:i+2]:
-                    if tr2.best_bx_evidence[1] == 1.0 and (tr2.tr_penalty != 'yes' and tr2.lg_penalty != 'yes') and (tr2.best_tr_evidence[1] != 1.0 or tr2.best_lg_evidence[1] != 1.0):
-                        if tr2.get_min_cds_start() < tr.get_min_cds_start() or tr2.get_max_cds_end() > tr.get_max_cds_end():
+                    if tr2.best_bx_evidence[1] == 1.0 and (tr2.tr_penalty != 'yes' \
+                        and tr2.lg_penalty != 'yes') and (tr2.best_tr_evidence[1] != 1.0 \
+                        or tr2.best_lg_evidence[1] != 1.0):
+                        if tr2.get_min_cds_start() < tr.get_min_cds_start() \
+                            or tr2.get_max_cds_end() > tr.get_max_cds_end():
                             if tr.is_cds_included_in_other_cds(tr2):
                                 if self.no_partial:
                                     if not tr2.is_cds_partial(self.genome_fasta_file):
-                                        logging.debug("CDS of TR: {}, {}, {} is in CDS of TR2: {}, {}, {}, removed".format(tr.id, tr.seqid, tr.start, tr2.id, tr2.seqid, tr2.start))
+                                        logging.debug(f"CDS of TR: {tr.id}, {tr.seqid}, \
+                                        {tr.start} is in CDS of TR2: {tr2.id}, {tr2.seqid}, \
+                                        {tr2.start}, removed")
                                         to_keep = False
                                 else:
-                                    logging.debug("CDS of TR: {}, {}, {} is in CDS of TR2: {}, {}, {}, removed".format(tr.id, tr.seqid, tr.start, tr2.id, tr2.seqid, tr2.start))
+                                    logging.debug("CDS of TR: {tr.id}, {tr.seqid}, {tr.start} \
+                                    is in CDS of TR2: {tr2.id}, {tr2.seqid}, {tr2.start}, removed")
                                     to_keep = False
             if to_keep:
                 new_tr.append(tr)
         # add last tr
         new_tr.append(ltr[-1])
         return new_tr
 
 
     def filter(self, metagenes, nb_not_exported, coords=None):
+        '''filter '''
 
         export_tr = []
         not_exported_tr = []
 
-        for mg in metagenes:
+        for nb, mg in enumerate(metagenes):
+
+            if nb%1000 == 0:
+                logging.info(f"{nb} metagenes analyzed on {len(metagenes)}")
+
             current_mg_export_tr = []
             current_mg_not_export_tr = []
             lsorted_tmp = Utils.rank_transcripts(mg.lTranscripts, self.gaeval)
 
-
             # limit potential transcripts to coordinates (use for rescue overlapping CDS)
             lsorted = []
             if coords:
                 for tr in lsorted_tmp:
                     if tr.get_min_cds_start() > coords[0] and tr.get_max_cds_end() < coords[1]:
                         lsorted.append(tr)
                 lsorted_tmp = lsorted
@@ -144,21 +180,21 @@
             lsorted = []
             if self.no_partial:
                 #for tr in lsorted_tmp:
                 for tr in lfilteredlen:
                     if not tr.is_cds_partial(self.genome_fasta_file):
                         lsorted.append(tr)
                     else:
-                        logging.debug("Partial CDS for {}".format(tr.id))
+                        logging.debug(f"Partial CDS for {tr.id}")
             else:
                 lsorted = lfilteredlen
 
 
             if len(lsorted) == 0:
-                logging.debug("No complete CDS for MetaGene {}, not exported".format(mg.id))
+                logging.debug(f"No complete CDS for MetaGene {mg.id}, not exported")
                 nb_not_exported += 1
                 continue
 
             # keep first CDS (tr)
             tr = lsorted[0]
             if mg.get_number_of_src() < self.nb_sources_filtering:
                 aed_tr = tr.best_tr_evidence[1]
@@ -176,147 +212,148 @@
                 export_tr.append(tr)
                 current_mg_export_tr.append(tr)
 
             if len(current_mg_export_tr) > 0:
                 # try to rescue other CDS  if no overlap
                 for i,tr in enumerate(lsorted[1::]):
                     overlap = False
-                    #for j in range(0,i+1): # modif1
-                    for j in current_mg_export_tr: #modif2
-                        #if tr.overlap_cds_with_other_transcript_cds(lsorted[j]): #modif1
-                        if tr.overlap_cds_with_other_transcript_cds(j):  #modif
+                    for j in current_mg_export_tr:
+                        if tr.overlap_cds_with_other_transcript_cds(j):
                             overlap = True
                             break
-                    if overlap:
-                        #break #modif1
-                        continue  # modif2
-                    else:
-                        # DEBUG
+                    if not overlap:
                         if mg.get_number_of_src_overlapping_tr(tr) < self.nb_sources_filtering:
-                        # DEBUG: nb source at tr level , too many filtered
-#                        if mg.get_number_of_src_overlapping_tr_with_tr_restrictions(tr, current_mg_export_tr) < self.nb_sources_filtering:
-                          # DEBUG : too many conserved 
-#                        if mg.get_number_of_src() < self.nb_sources_filtering:
                             aed_tr = tr.best_tr_evidence[1]
                             if self.use_ev_lg:
                                 aed_tr = min(tr.best_tr_evidence[1],tr.best_lg_evidence[1])
-                            if aed_tr <= self.aedtr_filtering or tr.best_bx_evidence[1] <= self.aedpr_filtering:
+                            if aed_tr <= self.aedtr_filtering \
+                                or tr.best_bx_evidence[1] <= self.aedpr_filtering:
                                 export_tr.append(tr)
                                 current_mg_export_tr.append(tr)
-#                            else:
-#                                for y in current_mg_not_export_tr:
-#                                    if tr.overlap_cds_with_other_transcript_cds(y):  #modif
-#                                        not_exported_tr.append(tr)
-#                                        current_mg_not_export_tr.append(tr)
                         else:
                             export_tr.append(tr)
                             current_mg_export_tr.append(tr)
 
-        logging.debug("{} metagenes not exported".format(nb_not_exported))
+        logging.debug(f"{nb_not_exported} metagenes not exported")
 
         return export_tr, not_exported_tr
 
 
     def export(self,allgenes, export_tr, fh):
+        '''export selection in gff'''
 
         source = "ingenannot"
         references = list(set([x.seqid for x in allgenes]))
         Utils.natural_sort(references)
 
         with open(fh, 'w') as f:
             ID = 0
             for ref in references:
                 seq_genes = [g for g in allgenes if g.seqid == ref]
-                for tr in sorted([ t for t in export_tr if t.seqid == ref], key=lambda x: x.get_min_cds_start()):
+                for tr in sorted([ t for t in export_tr if t.seqid == ref],
+                        key=lambda x: x.get_min_cds_start()):
                     for gene in seq_genes:
 
                         if gene.gene_id == tr.gene_id and gene.source == tr.source:
                             ID += 1
-                            #atts = {'ID':['gene:{}'.format(gene.gene_id)],'source':[gene.source]}
-                            atts = {'ID':['{}_{:05}'.format(self.prefix,ID)],'gene_source':[gene.gene_id],'source':['{}'.format(gene.source)]}
+                            atts = {'ID':[f'{self.prefix}_{ID:05}'],
+                                    'gene_source':[gene.gene_id],
+                                    'source':[f'{gene.source}']}
 
-                            # change gene coordinates in case of selection of one isoform 
+                            # change gene coordinates in case of selection of one isoform
                             gene.start = tr.start
                             gene.end = tr.end
 
                             f.write(gene.to_gff3(atts=atts, source=source))
                             if not tr.best_tr_evidence[0]:
                                 ev_tr = "None"
                             else:
                                 ev_tr = tr.best_tr_evidence[0]
                             if not tr.best_bx_evidence[0]:
                                 ev_bx = "None"
                             else:
-                                #ev_bx = tr.best_bx_evidence[0].id
                                 ev_bx = tr.best_bx_evidence[0]
-    
-                            #atts = {'ID':['mRNA:{}'.format(tr.id)], 'source':[gene.source],'Parent':['gene:{}'.format(gene.gene_id)], 'ev_tr': [ev_tr], 'aed_ev_tr':['{:.4f}'.format(tr.best_tr_evidence[1])], 'ev_tr_penalty': [tr.tr_penalty], 'ev_pr' : [ev_bx], 'aed_ev_pr' : ['{:.4f}'.format(tr.best_bx_evidence[1])]}
-                            atts = {'ID':['{}_{:05}.1'.format(self.prefix,ID)], 'transcript_source':[tr.id],'source':[gene.source],'Parent':['{}_{:05}'.format(self.prefix,ID)],'ev_tr': [ev_tr], 'aed_ev_tr':['{:.4f}'.format(tr.best_tr_evidence[1])], 'ev_tr_penalty': [tr.tr_penalty], 'ev_pr' : [ev_bx], 'aed_ev_pr' : ['{:.4f}'.format(tr.best_bx_evidence[1])]}
-    
+
+                            atts = {'ID':[f'{self.prefix}_{ID:05}.1'],
+                                    'transcript_source':[tr.id],'source':[gene.source],
+                                    'Parent':[f'{self.prefix}_{ID:05}'],'ev_tr': [ev_tr],
+                                    'aed_ev_tr':[f'{tr.best_tr_evidence[1]:.4f}'],
+                                    'ev_tr_penalty': [tr.tr_penalty], 'ev_pr' : [ev_bx],
+                                    'aed_ev_pr' : [f'{tr.best_bx_evidence[1]:.4f}']}
+
                             #if self.longread_gff_file:
                             if not tr.best_lg_evidence[0]:
                                 ev_lg = "None"
                             else:
                                 #ev_lg = tr.best_lg_evidence[0].id
                                 ev_lg = tr.best_lg_evidence[0]
-                            atts_lg = {'ev_lg': [ev_lg], 'aed_ev_lg':['{:.4f}'.format(tr.best_lg_evidence[1])],'ev_lg_penalty':[tr.lg_penalty]}
+                            atts_lg = {'ev_lg': [ev_lg],
+                                    'aed_ev_lg':[f'{tr.best_lg_evidence[1]:.4f}'],
+                                    'ev_lg_penalty':[tr.lg_penalty]}
                             atts.update(atts_lg)
-    
+
                             f.write(tr.to_gff3(atts=atts,source=source))
-    
+
                             for i,exon in enumerate(tr.lExons):
-                                #atts = {'ID':['exon:{}.{}'.format(gene.gene_id,i+1)], 'source':[gene.source],'Parent':['mRNA:{}'.format(tr.id)]}
-                                atts = {'ID':['exon:{}_{:05}.{}'.format(self.prefix,ID,i+1)],'Parent':['{}_{:05}.1'.format(self.prefix,ID)]}
+                                atts = {'ID':[f'exon:{self.prefix}_{ID:05}.{i+1}'],
+                                        'Parent':[f'{self.prefix}_{ID:05}.1']}
                                 f.write(exon.to_gff3(atts=atts,source=source))
                             for i,cds in enumerate(tr.lCDS):
-                                #atts = {'ID':['cds:{}'.format(tr.id)], 'source':[gene.source],'Parent':['mRNA:{}'.format(tr.id)]}
-                                atts = { 'ID':['cds:{}_{:05}.1'.format(self.prefix,ID)],'Parent':['{}_{:05}.1'.format(self.prefix,ID)]}
+                                atts = { 'ID':[f'cds:{self.prefix}_{ID:05}.1'],
+                                        'Parent':[f'{self.prefix}_{ID:05}.1']}
                                 f.write(cds.to_gff3(atts=atts,source=source))
                             break
         f.close()
 
 
     def run(self):
         """"launch command"""
 
-        if not self.noaed:
+        genes = Utils.extract_genes_from_fof(self.fof)
+
+        if self.noaed:
+            Utils.get_aed_from_attributes(genes)
+        else:
             if not self.transcript_gff_file:
                 raise Exception("missing transcript evidence file: set --evtr parameter")
             if not self.protein_gff_file:
                 raise Exception("missing protein evidence file: set --evpr parameter")
 
-
-        sources = Utils.get_sources_from_fof(self.fof)
-        genes = Utils.extract_genes_from_fof(self.fof)
-
-        if self.noaed:
-            Utils.get_aed_from_attributes(genes)
         if self.gaeval:
             gaeval_infos = Utils.extract_gaeval_from_fof(self.fof)
             Utils.add_gaeval_infos_to_transcripts(genes, gaeval_infos)
 
-
-        clusters = Utils.clusterize(genes, cltype=self.clutype, stranded=self.clustranded, procs=Command.NB_CPUS)
+        clusters = Utils.clusterize(genes, cltype=self.clutype,
+                stranded=self.clustranded, procs=Command.NB_CPUS)
         metagenes = Utils.get_metagenes_from_clusters(clusters)
         nb_metagenes = len(metagenes)
         ##debug
         if self.nbsrc_absolute > 1:
             metagenes = self.filter_metagenes_required_number_sources(metagenes)
         nb_removed_metagenes = nb_metagenes - len(metagenes)
         if not self.noaed:
             for metag in metagenes:
-                metag.genes = AnnotEditDistance.compute_aed(metag.genes, self.transcript_gff_file, self.transcript_gff_file_stranded, self.transcript_gff_file_source, self.penalty_overflow, evtype="tr", cds_only=self.aed_tr_cds_only, procs=Command.NB_CPUS)
-
-                metag.genes = AnnotEditDistance.compute_aed(metag.genes, self.protein_gff_file, self.protein_gff_file_stranded, self.protein_gff_file_source, 0.0, evtype="pr", procs=Command.NB_CPUS)
+                metag.genes = AnnotEditDistance.compute_aed(metag.genes,
+                        self.transcript_gff_file, self.transcript_gff_file_stranded,
+                        self.transcript_gff_file_source, self.penalty_overflow, evtype="tr",
+                        cds_only=self.aed_tr_cds_only, procs=Command.NB_CPUS)
+
+                metag.genes = AnnotEditDistance.compute_aed(metag.genes,
+                        self.protein_gff_file, self.protein_gff_file_stranded,
+                        self.protein_gff_file_source, 0.0, evtype="pr", procs=Command.NB_CPUS)
 
                 if self.longread_gff_file:
-                    metag.genes = AnnotEditDistance.compute_aed(metag.genes, self.longread_gff_file, True, self.longread_gff_file_source, self.longread_penalty_overflow, evtype="lg", cds_only=self.aed_tr_cds_only, procs=Command.NB_CPUS)
+                    metag.genes = AnnotEditDistance.compute_aed(metag.genes,
+                            self.longread_gff_file, True, self.longread_gff_file_source,
+                            self.longread_penalty_overflow, evtype="lg",
+                            cds_only=self.aed_tr_cds_only, procs=Command.NB_CPUS)
 
+        print("ici")
         transcripts, transcripts_not_exported = self.filter(metagenes, nb_removed_metagenes)
-
+        print("la")
         if self.no_cds_overlap:
             logging.info("Analyzing CDS overlap")
             transcripts, strfr_transcripts_not_exported = self.aed_strand_filter(transcripts)
             nb_rescue = 0
             for strfr in strfr_transcripts_not_exported:
                 rescue_tr = self.rescue_tr_overlapping_cds(strfr, metagenes, transcripts)
                 if rescue_tr:
@@ -325,71 +362,82 @@
                     transcripts.append(rescue_tr[0])
                 else:
 
                     transcripts_not_exported.append(strfr)
 
             # rescue transcript if a non-overlapp
 
-            logging.info("{} transcripts rescued after overlapping with other CDS".format(nb_rescue))
+            logging.info(f"{nb_rescue} transcripts rescued after overlapping with other CDS")
 
 
-        l_aed_tr, l_aed_tr_no_penalty, l_aed_pr, l_aed_pr_no_penalty = Graphics.get_values_for_aed_scatter_hist(transcripts,self.use_ev_lg)
+        l_aed_tr, l_aed_tr_no_penalty, l_aed_pr, l_aed_pr_no_penalty = \
+        Graphics.get_values_for_aed_scatter_hist(transcripts,self.use_ev_lg)
 
+        graph_output = f"{self.output}.scatter_hist_aed.png"
+        Graphics.plot_aed_scatter_hist([l_aed_tr, l_aed_pr, l_aed_tr_no_penalty,
+            l_aed_pr_no_penalty], self.aedtr_filtering, self.aedpr_filtering,
+            graph_output ,legend=['aed_tr','aed_pr'], title="all runs - density of aed")
+        logging.info(f"Scatter plot exported in {graph_output}")
 
-        graph_output = "{}.scatter_hist_aed.png".format(self.output)
-        Graphics.plot_aed_scatter_hist([l_aed_tr, l_aed_pr, l_aed_tr_no_penalty, l_aed_pr_no_penalty], self.aedtr_filtering, self.aedpr_filtering, graph_output ,legend=['aed_tr','aed_pr'], title="all runs - density of aed")
-        logging.info("Scatter plot exported in {}".format(graph_output))
-        
         self.export(genes,transcripts,self.output)
         if self.no_export :
             self.export(genes,transcripts_not_exported,"no-export.{}".format(self.output))
 
         return 0
 
 
     def aed_strand_filter(self, transcripts):
+        '''filter overlapping CDS based on AED'''
 
         transcripts_not_exported = []
 
         list_to_remove = Utils.aed_strand_filter_transcripts(transcripts)
 
         new_transcripts = []
         for tr in transcripts:
             if tr not in list_to_remove:
                 new_transcripts.append(tr)
             else:
                 transcripts_not_exported.append(tr)
 
-        logging.info("{} transcripts removed due to overlapping with other CDS".format(len(transcripts_not_exported)))
+        logging.info(f"{len(transcripts_not_exported)} transcripts \
+                removed due to overlapping with other CDS")
 
         return new_transcripts, transcripts_not_exported
 
 
     def rescue_tr_overlapping_cds(self, tr, metagenes, transcripts):
+        '''rescue gene in case of overlaps '''
 
         tr_before = None
         tr_after = None
 
-        transcripts_sorted = sorted([ tt for tt in transcripts if tt.seqid == tr.seqid ], key=lambda x: x.get_min_cds_start()) 
+        transcripts_sorted = sorted([ tt for tt in transcripts if tt.seqid == tr.seqid ],
+                                      key=lambda x: x.get_min_cds_start())
 
         for i,t in enumerate(transcripts_sorted[:-1]):
-            if tr.get_min_cds_start() > transcripts_sorted[i].get_min_cds_start() and tr.get_max_cds_end() < transcripts_sorted[i+1].get_max_cds_end():
+            if tr.get_min_cds_start() > transcripts_sorted[i].get_min_cds_start() \
+                and tr.get_max_cds_end() < transcripts_sorted[i+1].get_max_cds_end():
                 tr_before = transcripts_sorted[i]
                 tr_after = transcripts_sorted[i+1]
         if not tr_before or not tr_after:
             return None
         meta = None
         for m in metagenes:
             if tr in m.lTranscripts:
                 meta = copy.deepcopy(m)
                 break
         filtered_tr = []
-        for tr in meta.lTranscripts:
-            if tr.get_min_cds_start() > tr_before.get_max_cds_end() and tr.get_max_cds_end() < tr_after.get_min_cds_start():
+        for tran in meta.lTranscripts:
+            if tran.get_min_cds_start() > tr_before.get_max_cds_end() \
+                and tran.get_max_cds_end() < tr_after.get_min_cds_start():
                 filtered_tr.append(tr)
 
         if len(filtered_tr) == 0:
             return None
 
-        tr_filt, tr_filt_not_exported = self.filter([meta], 0, coords=(tr_before.get_max_cds_end(),tr_after.get_min_cds_start()))
+        tr_filt, tr_filt_not_exported = self.filter([meta], 0,
+                coords=(tr_before.get_max_cds_end(),tr_after.get_min_cds_start()))
         if tr_filt:
             return tr_filt
+
+        return None
```

### Comparing `ingenannot-0.0.7/ingenannot/commands/so_classification.py` & `ingenannot-0.0.8/ingenannot/commands/so_classification.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/commands/strand_annotation_filter.py` & `ingenannot-0.0.8/ingenannot/commands/strand_annotation_filter.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/commands/utr_refine.py` & `ingenannot-0.0.8/ingenannot/commands/utr_refine.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,52 @@
 #/usr/bin/env python3
 
+'''This module contains UTRRefine class'''
+
 import logging
 import copy
 
 from ingenannot.commands.command import Command
 from ingenannot.utils import Utils
 from ingenannot.entities.exon import Exon
 
 class UTRRefine(Command):
+    '''
+    The UTRRefine is a Command running utr inference 
+
+    Attributes:
+    -----------
+    gff_gene : Gff_genes
+    gff_transcripts : Gff_transcripts
+    gff_output : Output
+    utr_mode : utr_mode
+    erase : erase
+    onlynew : onlynew
+    '''
 
     def __init__(self, args):
 
         self.gff_gene = args.Gff_genes
         self.gff_transcripts = args.Gff_transcripts
         self.gff_output = args.Output
         self.utr_mode = args.utr_mode
         self.erase = args.erase
         self.onlynew = args.onlynew
 
     def get_best_evidence(self, tr, tr_tps):
+        '''get best isoform for UTR coordinates with mode'''
 
         t = None
         if self.utr_mode == "shortest":
             len_utrs = 1000000
             for tr_tp in tr_tps:
                 l = tr_tp.getExonTotalLength() - tr.getCDSTotalLength()
                 if l < len_utrs:
                     len_utrs = l
                     t = tr_tp
-                    print(t, len_utrs)
         elif self.utr_mode == "rank": #rank tag in gff3
             rank = 10000
             for tr_tp in tr_tps:
                 if 'rank' not in tr_tp.dAttributes:
                     raise Exception("Cannot clasified with rank, missing tag rank in gff3")
                 if int(tr_tp.dAttributes['rank'][0]) < rank:
                     rank = int(tr_tp.dAttributes['rank'][0])
@@ -44,193 +58,168 @@
                 if l > len_utrs:
                     len_utrs = l
                     t = tr_tp
         return t
 
 
     def update_transcript_coords(self, tr, tr_tp):
+        '''update transcript coords'''
 
         tr.lExons = copy.deepcopy(tr_tp.lExons)
         for e in tr.lExons:
             e.lTranscript_ids = []
-        tr.start = min([x.start for x in tr.lExons])
-        tr.end = max([x.end for x in tr.lExons])
-
-#        if self.erase: # replace exons
-#            print(tr.lExons)
-#            print(tr_tp.lExons)
-#            tr.lExons = copy.deepcopy(tr_tp.lExons)
-#            for e in tr.lExons:
-#                e.lTranscript_ids = []
-#            tr.start = min([x.start for x in tr.lExons])
-#            tr.end = max([x.end for x in tr.lExons])
-#            print(tr.lExons)
-#            print(tr_tp.lExons)
-#
-#        else: # update exons
-#            print(tr.lExons)
-#            print(tr_tp.lExons)
+        tr.start = min(x.start for x in tr.lExons)
+        tr.end = max(x.end for x in tr.lExons)
 
     def update_gene_coords(self, g):
+        '''update gene coords'''
 
-        g.start = min([x.start for x in g.lTranscripts])
-        g.end = max([x.end for x in g.lTranscripts])
+        g.start = min(x.start for x in g.lTranscripts)
+        g.end = max(x.end for x in g.lTranscripts)
 
     def update_cds_transcript(self, tr):
+        '''update CDS coords'''
 
         for cds in tr.lCDS:
-            cds.cds_id = "cds_{}".format(tr.id)
+            cds.cds_id = f"cds_{tr.id}"
 
 
     def update_exon_transcripts(self, g):
+        '''update exons coords'''
 
         lExons = {}
         for tr in g.lTranscripts:
-#            print("TRRRRRR", g.gene_id, tr.id)
             tr_exons = []
             for e in tr.lExons:
                 if (e.start, e.end) in lExons:
                     tr_exons.append(lExons[(e.start, e.end)])
                     lExons[(e.start, e.end)].add_transcript(tr.id)
                 else:
                     e.add_transcript(tr.id)
                     tr_exons.append(e)
                     lExons[(e.start, e.end)] = e
             tr.lExons = tr_exons
 
         for i,e in enumerate(sorted(lExons.values(), key=lambda x: x.start)):
-#            print("ICI")
-#            print(e.exon_id)
-            e.exon_id = "{}_exon{:03}".format(g.gene_id, i+1)
-#            print(e.exon_id)
+            e.exon_id = f"{g.gene_id}_exon{i+1:03}"
 
     def export(self, genes, updated_transcripts):
         """export to Gff3"""
 
-        logging.info("exporting genes in {}".format(self.gff_output))
+        logging.info(f"exporting genes in {self.gff_output}")
 
         with open(self.gff_output, 'w') as f:
-                for gene in genes :
-                    atts = {'ID':[gene.gene_id],'source':[gene.source]}
-                    f.write(gene.to_gff3(atts))
-
-                    for tr in gene.lTranscripts:
-                        #atts = {'ID':[tr.id], 'source':[gene.source],'Parent':[gene.gene_id]}
-#                        print(tr.id)
-                        atts = tr.dAttributes
-                        if tr.id in updated_transcripts:
-                            atts['ID'] = [tr.id]
-                            atts['utr_refine_evidence'] = [updated_transcripts[tr.id]]
-                            #atts = {'ID':[tr.id],'Parent':[gene.gene_id],'utr_refine_evidence':[updated_transcripts[tr.id]]}
-                        f.write(tr.to_gff3(atts=atts))
- #                       print(tr.to_gff3(atts=atts))
-                    #dedup exons
-                    lExons = []
-                    for tr in gene.lTranscripts:
-                        for i,exon in enumerate(tr.lExons):
-                            atts = {'ID':[exon.exon_id], 'source':[gene.source],'Parent':[",".join(exon.lTranscript_ids)]}
-                            #tr.add_cds(CDS('cds:{}_{}-{}'.format(exon.seqid,exon.start,exon.end),exon.seqid,exon.start,exon.end,exon.strand,'.',tr.id))
-                            if exon.exon_id not in lExons:
-                                f.write(exon.to_gff3(atts=atts))
-                                lExons.append(exon.exon_id)
-                    for tr in gene.lTranscripts:
-                        for i,cds in enumerate(tr.lCDS):
-                            atts = {'ID':[cds.cds_id], 'source':[gene.source],'Parent':[tr.id]}
-                            f.write(cds.to_gff3(atts=atts))
-
-                    for tr in gene.lTranscripts:
-                        strand = '+'
-                        if tr.strand == -1:
-                           strand = '-'
-                        five_prime_utrs = tr.infer_five_prime_utrs()
-                        for i,utr in enumerate(five_prime_utrs):
-                            atts = {'ID':['five_prime_UTR_{}_{:03}'.format(tr.id,i+1)], 'source':[gene.source],'Parent':[tr.id]}
-                            str_atts = ''
-                            for att in atts:
-                                str_atts += '{}={};'.format(att,",".join(atts[att]))
-                            f.write("{}\t{}\tfive_prime_UTR\t{}\t{}\t.\t{}\t.\t{}\n".format(tr.seqid,'ingenannot',utr[0],utr[1],strand,str_atts))
-                        three_prime_utrs = tr.infer_three_prime_utrs()
-                        for i,utr in enumerate(three_prime_utrs):
-                            atts = {'ID':['three_prime_UTR_{}_{:03}'.format(tr.id,i+1)], 'source':[gene.source],'Parent':[tr.id]}
-                            str_atts = ''
-                            for att in atts:
-                                str_atts += '{}={};'.format(att,",".join(atts[att]))
-                            f.write("{}\t{}\tthree_prime_UTR\t{}\t{}\t.\t{}\t.\t{}\n".format(tr.seqid,'ingenannot',utr[0],utr[1],strand,str_atts))
-
-
+            for gene in genes :
+                atts = {'ID':[gene.gene_id],'source':[gene.source]}
+                f.write(gene.to_gff3(atts))
+
+                for tr in gene.lTranscripts:
+                    atts = tr.dAttributes
+                    if tr.id in updated_transcripts:
+                        atts['ID'] = [tr.id]
+                        atts['utr_refine_evidence'] = [updated_transcripts[tr.id]]
+                    f.write(tr.to_gff3(atts=atts))
+                #dedup exons
+                lExons = []
+                for tr in gene.lTranscripts:
+                    for i,exon in enumerate(tr.lExons):
+                        atts = {'ID':[exon.exon_id], 'source':[gene.source],
+                                'Parent':[",".join(exon.lTranscript_ids)]}
+                        if exon.exon_id not in lExons:
+                            f.write(exon.to_gff3(atts=atts))
+                            lExons.append(exon.exon_id)
+                for tr in gene.lTranscripts:
+                    for i,cds in enumerate(tr.lCDS):
+                        atts = {'ID':[cds.cds_id], 'source':[gene.source],'Parent':[tr.id]}
+                        f.write(cds.to_gff3(atts=atts))
+
+                for tr in gene.lTranscripts:
+                    strand = '+'
+                    if tr.strand == -1:
+                        strand = '-'
+                    five_prime_utrs = tr.infer_five_prime_utrs()
+                    for i,utr in enumerate(five_prime_utrs):
+                        atts = {'ID':[f'five_prime_UTR_{tr.id}_{i+1:03}'],
+                                'source':[gene.source],'Parent':[tr.id]}
+                        str_atts = ''
+                        for att in atts:
+                            str_atts += f"{att}={','.join(atts[att])};"
+                        f.write(f"{tr.seqid}\tingenannot\tfive_prime_UTR\t" \
+                                f"{utr[0]}\t{utr[1]}\t.\t{strand}\t.\t{str_atts}\n")
+                    three_prime_utrs = tr.infer_three_prime_utrs()
+                    for i,utr in enumerate(three_prime_utrs):
+                        atts = {'ID':[f'three_prime_UTR_{tr.id}_{i+1:03}'],
+                                'source':[gene.source],'Parent':[tr.id]}
+                        str_atts = ''
+                        for att in atts:
+                            str_atts += f"{att}={','.join(atts[att])};"
+                        f.write(f"{tr.seqid}\tingenannot\tthree_prime_UTR\t" \
+                                f"{utr[0]}\t{utr[1]}\t.\t{strand}\t.\t{str_atts}\n")
         f.close()
 
-        logging.info("{} genes exported".format(len(genes)))
-
-
+        logging.info(f"{len(genes)} genes exported")
 
     def run(self):
         """"launch command"""
 
         tr_to_genes = {}
         selected_tr_tp = set()
         tr_tp_to_remove = set()
         genes = Utils.extract_genes(self.gff_gene)
         tr_templates = Utils.extract_genes(self.gff_transcripts)
 
-
         if self.erase:
             for g in genes:
-#                if len(g.lTranscripts) > 1:
-#                    print(g.gene_id) 
-#                    raise ("Excpetion multi transcript not yt implemented")
                 for t in g.lTranscripts:
                     exons = []
                     for idx,cds in enumerate(t.lCDS):
-                        exons.append(Exon("exon:{}.{}".format(g.gene_id,idx),g.seqid,cds.start,cds.end,cds.strand,[]))
+                        exons.append(Exon(f"exon:{g.gene_id}.{idx}",
+                            g.seqid,cds.start,cds.end,cds.strand,[]))
                     t.lExons = exons
 
-                    t.start = min([x.start for x in t.lExons])
-                    t.end = max([x.end for x in t.lExons])
+                    t.start = min(x.start for x in t.lExons)
+                    t.end = max(x.end for x in t.lExons)
                 self.update_gene_coords(g)
                 self.update_exon_transcripts(g)
 
-
         for g in genes:
-            for g_tp in [gene for gene in tr_templates if (gene.seqid == g.seqid) & (gene.strand == g.strand)]:
+            for g_tp in [gene for gene in tr_templates \
+                if (gene.seqid == g.seqid) & (gene.strand == g.strand)]:
                 if g.is_feature_spanning(g_tp):
                     for tr in g.lTranscripts:
                         tr_to_genes[tr.id] = []
                         for tr_tp in g_tp.lTranscripts:
                             # check no specific CDS bases
                             if tr.get_nb_specific_bases_vs_another_transcript(tr_tp,True,False) == 0:
                                 # check bases in introns
                                 if tr_tp.get_nb_specific_bases_vs_another_transcript_specific_positions(tr,tr.get_min_cds_start(), tr.get_max_cds_end(), False, False) == 0:
                                     # check new specific bases (not same coord = same UTRs)
                                     if tr_tp.get_nb_specific_bases_vs_another_transcript(tr,False,False) > 0:
-        #                                print("OK: ", tr.id, tr_tp.id)
                                         tr_to_genes[tr.id].append(tr_tp)
                                         if tr_tp.id in selected_tr_tp:
                                             tr_tp_to_remove.add(tr_tp.id)
                                         selected_tr_tp.add(tr_tp.id)
-         #                               print(tr_tp.id)
                                     else:
-                                        logging.debug("NOK 3: no changes same UTRs {} - {}".format(tr.id, tr_tp.id))
+                                        logging.debug(f"NOK 3: no changes same UTRs {tr.id} - {tr_tp.id}")
                                 else:
-                                    logging.debug("NOK 2: not same CDS coordinates, false intron in annotation {} - {}".format(tr.id, tr_tp.id))
+                                    logging.debug(f"NOK 2: not same CDS coordinates, false intron in annotation {tr.id} - {tr_tp.id}")
                             else:
-                                logging.debug("NOK 1: not same CDS coordinates, missing intron in annotation {} - {}".format(tr.id, tr_tp.id))
+                                logging.debug(f"NOK 1: not same CDS coordinates, missing intron in annotation {tr.id} - {tr_tp.id}")
 
           #2: control overlap on adjacent genes
           # if a transcript span several gene possible bug
           # or readthrought = to remove
-        logging.info("removing {} transcripts before UTR definition, overlapping multiple CDS".format(len(tr_tp_to_remove)))
+        logging.info(f"removing {len(tr_tp_to_remove)} transcripts before \
+                UTR definition, overlapping multiple CDS")
         for tr_id in tr_to_genes:
             l = []
             for tr_tp in tr_to_genes[tr_id]:
                 if tr_tp.id not in tr_tp_to_remove:
                     l.append(tr_tp)
             tr_to_genes[tr_id] = l
-#        print("### TO REMOVE ###")
-#        print(tr_tp_to_remove)
 
         # change utr
         updated_transcripts = {}
         for g in genes:
             replaced_transcripts = []
             created_transcripts = []
             utr_change_flag = False
@@ -242,42 +231,38 @@
                     if len(tr_to_genes[tr.id]) > 0:
                     #write function to add utr with mode
                         if self.utr_mode == 'all':
                             #self.update_transcript_coords(tr, start, end)
                             if len(tr_to_genes[tr.id]) == 1:
                                 t = tr_to_genes[tr.id][0]
                                 self.update_transcript_coords(tr, t)
-                                logging.info("{} UTRs changed with {}".format(tr.id, t.id))
+                                logging.info(f"{tr.id} UTRs changed with {t.id}")
                                 updated_transcripts[tr.id] = t.id
                             else:
                                 for i,tr_tp in enumerate(tr_to_genes[tr.id]):
                                     tr_iso = copy.deepcopy(tr) # exon deepcopied too will be removed in update_exons (to refactor)
                                     # need implementation tr copy method
-                                    tr_iso.id = "{}_utr_isoform{:03}".format(tr.id,i+1)
-                               #     print("REEE",tr_tp)
+                                    tr_iso.id = f"{tr.id}_utr_isoform{i+1:03}"
                                     self.update_transcript_coords(tr_iso, tr_tp)
-                                    logging.info("{} UTRs changed with {}".format(tr_iso.id, tr_tp.id))
+                                    logging.info(f"{tr_iso.id} UTRs changed with {tr_tp.id}")
                                     updated_transcripts[tr_iso.id] = tr_tp.id
                                     created_transcripts.append(tr_iso)
                                 replaced_transcripts.append(tr)
                         else:
                             t = self.get_best_evidence(tr, tr_to_genes[tr.id])
                             self.update_transcript_coords(tr, t)
-                            logging.info("{} UTRs changed with {}".format(tr.id, t.id))
+                            logging.info(f"{tr.id} UTRs changed with {t.id}")
                             updated_transcripts[tr.id] = t.id
                         utr_change_flag = True
             if utr_change_flag:
                 if self.utr_mode == 'all':
                     for xtr in replaced_transcripts:
                         g.remove_transcript(xtr.id)
                     for xtr in created_transcripts:
                         g.add_transcript(xtr)
                         self.update_cds_transcript(xtr)
                 self.update_gene_coords(g)
                 self.update_exon_transcripts(g)
-        #        self.add_utrs(g)
-        #        print(g)
-        #        print(g.lTranscripts[0].lExons)
 
         self.export(genes, updated_transcripts)
 
         return 0
```

### Comparing `ingenannot-0.0.7/ingenannot/commands/validate.py` & `ingenannot-0.0.8/ingenannot/commands/validate.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/entities/cds.py` & `ingenannot-0.0.8/ingenannot/entities/cds.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/entities/cluster.py` & `ingenannot-0.0.8/ingenannot/entities/cluster.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/entities/exon.py` & `ingenannot-0.0.8/ingenannot/entities/exon.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/entities/gene.py` & `ingenannot-0.0.8/ingenannot/entities/gene.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/entities/metagene.py` & `ingenannot-0.0.8/ingenannot/entities/metagene.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/entities/transcript.py` & `ingenannot-0.0.8/ingenannot/entities/transcript.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/main.py` & `ingenannot-0.0.8/ingenannot/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,39 +39,39 @@
         )
         self.subparsers = self.parser.add_subparsers(help="sub-command help")
 
 
     def load_all_subparsers(self):
         """Load all subparsers"""
 
-        self.subparser_validate()
-        self.subparser_compare()
-        self.subparser_select()
-        self.subparser_aed_strand_annotation_filter()
-        self.subparser_aed()
-        self.subparser_isoform_ranking() # coverage test
-        self.subparser_filter() # code
-        self.subparser_rescue_effectors() # code
-        self.subparser_effector_predictor() # code
-        self.subparser_utr_refine()
         self.subparser_add_sqanti3_isoforms()
+        self.subparser_aed()
         self.subparser_aed_compare() # code and test to do and validate
+        self.subparser_aed_strand_annotation_filter()
+        self.subparser_clusterize()
+        self.subparser_compare()
+        self.subparser_curation()
+        self.subparser_effector_predictor() # code
         self.subparser_exonerate_to_gff()
+        self.subparser_filter() # code
+        self.subparser_isoform_ranking() # coverage test
         self.subparser_rename()
-        self.subparser_clusterize()
+        self.subparser_rescue_effectors() # code
+        self.subparser_select()
         self.subparser_soclassif()
-
+        self.subparser_utr_refine()
+        self.subparser_validate()
 
 
     def subparser_soclassif(self):
         """Add subparser for SOClassification cmd"""
 
         sbp = self.subparsers.add_parser(
                 'soclassif',
-                help='soclassif help'
+                help='Classify transcripts based on SO classification'
         )
         sbp.add_argument(
                 "fof",
                 help="File of files, <GFF/GTF>TAB<source>",
                 type=str
         )
         sbp.add_argument(
@@ -99,15 +99,15 @@
 
 
     def subparser_add_sqanti3_isoforms(self):
         """Add subparser for AddSqanti3Isoforms cmd"""
 
         sbp = self.subparsers.add_parser(
                 'add_sqanti3_isoforms',
-                help='add_sqanti3_isoforms help'
+                help='Add Isoforms from sqanti3 outputs'
         )
         sbp.add_argument(
                 "Gff_genes",
                 help="Gene Annotation file in GFF/GTF file format",
                 type=str
         )
         sbp.add_argument(
@@ -138,15 +138,15 @@
 
 
     def subparser_rescue_effectors(self):
         """Add subparser for RescueEffectors cmd"""
 
         sbp = self.subparsers.add_parser(
                 'rescue_effectors',
-                help='rescue_effectors help'
+                help='Perform rescue of effector genes'
         )
         sbp.add_argument(
                 "Gff_genes",
                 help="Gene Annotation file in GFF/GTF file format",
                 type=str
         )
         sbp.add_argument(
@@ -158,37 +158,37 @@
         sbp.add_argument(
                 "Genome",
                 help="Genome in fasta format or compressed in bgzip format",
                 type=str
         )
         sbp.add_argument(
                 "--signalp",
-                help="Path to signalp, default={} (from system lookup)"\
-                     .format(shutil.which('signalp')),
+                help=f"Path to signalp, default={shutil.which('signalp')} \
+                        (from system lookup)",
                 type=str,
                 default=shutil.which('signalp')
         )
         sbp.add_argument(
                 "--tmhmm",
-                help="Path to tmhmm, default={} (from system lookup)"\
-                     .format(shutil.which('tmhmm')),
+                help=f"Path to tmhmm, default={shutil.which('tmhmm')} \
+                        (from system lookup)",
                 type=str,
                 default=shutil.which('tmhmm')
         )
         sbp.add_argument(
                 "--targetp",
-                help="Path to targetp, default={} (from system lookup)"\
-                     .format(shutil.which('targetp')),
+                help=f"Path to targetp, default={shutil.which('targetp')} \
+                        (from system lookup)",
                 type=str,
                 default=shutil.which('targetp')
         )
         sbp.add_argument(
                 "--effectorp",
-                help="Path to signalp, default={} (from system lookup)"\
-                     .format(shutil.which('EffectorP')),
+                help=f"Path to signalp, default={shutil.which('EffectorP')} \
+                        (from system lookup)",
                 type=str,
                 default=shutil.which('EffectorP')
         )
         sbp.add_argument(
                 "--signalp_cpos",
                 help="Maximal position of signal peptide cleavage site, \
                       default=25",
@@ -243,46 +243,46 @@
 
 
     def subparser_effector_predictor(self):
         """Add subparser for EffectorPredictor cmd"""
 
         sbp = self.subparsers.add_parser(
                 'effector_predictor',
-                help='effector_predictor help'
+                help='Predict effector genes'
         )
         sbp.add_argument(
                 "fasta",
                 help="Fasta file of proteins",
                 type=str
         )
         sbp.add_argument(
                 "--signalp",
-                help="Path to signalp, default={} (from system lookup)"\
-                     .format(shutil.which('signalp')),
+                help=f"Path to signalp, default={shutil.which('signalp')} \
+                        (from system lookup)",
                 type=str,
                 default=shutil.which('signalp')
         )
         sbp.add_argument(
                 "--tmhmm",
-                help="Path to tmhmm, default={} (from system lookup)"\
-                     .format(shutil.which('tmhmm')),
+                help=f"Path to tmhmm, default={shutil.which('tmhmm')} \
+                        (from system lookup)",
                 type=str,
                 default=shutil.which('tmhmm')
         )
         sbp.add_argument(
                 "--targetp",
-                help="Path to targetp, default={} (from system lookup)"\
-                     .format(shutil.which('targetp')),
+                help=f"Path to targetp, default={shutil.which('targetp')} \
+                        (from system lookup)",
                 type=str,
                 default=shutil.which('targetp')
              )
         sbp.add_argument(
                 "--effectorp",
-                help="Path to signalp, default={} (from system lookup)"\
-                     .format(shutil.which('EffectorP')),
+                help=f"Path to signalp, default={shutil.which('EffectorP')} \
+                        (from system lookup)",
                 type=str, default=shutil.which('EffectorP')
         )
         sbp.add_argument(
                 "--signalp_cpos",
                 help="Maximal position of signal peptide cleavage site, \
                       default=25",
                 default=25, type=int
@@ -311,15 +311,15 @@
 
 
     def subparser_validate(self):
         """Add subparser for Validate cmd"""
 
         parser_validate = self.subparsers.add_parser(
                 'validate',
-                help='validate help'
+                help='Validate expected GTF/GFF file formats'
         )
         parser_validate.add_argument(
                 "Gff_genes",
                 help="Gene Annotation file in GFF/GTF file format",
                 type=str
         )
         parser_validate.add_argument(
@@ -366,15 +366,15 @@
 
 
     def subparser_isoform_ranking(self):
         """Add subparser for IsoformRanking cmd"""
 
         sbp = self.subparsers.add_parser(
                 'isoform_ranking',
-                help='isoform_ranking help'
+                help='Rank isoform based on junction and read coverages'
         )
         sbp.add_argument(
                 "Gff_transcripts",
                 help="Gff file of transcripts",
                 type=str
         )
         sbp.add_argument(
@@ -451,15 +451,15 @@
 
 
     def subparser_compare(self):
         """Add subparser for Compare cmd"""
 
         sbp = self.subparsers.add_parser(
                 'compare',
-                help='compare help'
+                help='Compare gene content between several annotations'
         )
         sbp.add_argument(
                 "fof",
                 help="File of files, <GFF/GTF>TAB<source>",
                 type=str
         )
         sbp.add_argument(
@@ -527,15 +527,15 @@
 
 
     def subparser_select(self):
         """Add subparser for Select cmd"""
 
         sbp = self.subparsers.add_parser(
                 'select',
-                help='select help'
+                help='Select best gene model'
         )
         sbp.add_argument(
                 "fof",
                 help="File of files, <GFF/GTF>TAB<source>",
                 type=str
         )
         sbp.add_argument(
@@ -724,15 +724,15 @@
 
 
     def subparser_aed(self):
         """Add subparser for AED cmd"""
 
         sbp = self.subparsers.add_parser(
                 'aed',
-                help='aed help'
+                help='Compute AED'
         )
         sbp.add_argument(
                 "Input",
                 help="GFF/GTF File",
                 type=str
         )
         sbp.add_argument(
@@ -842,15 +842,15 @@
 
 
     def subparser_filter(self):
         """Add subparser for Filter cmd"""
 
         sbp = self.subparsers.add_parser(
                 'filter',
-                help='filter help'
+                help='Filter annotations'
         )
         sbp.add_argument(
                 "Gff_genes",
                 help="Gene Annotation file in GFF/GTF file format",
                 type=str
         )
         sbp.add_argument(
@@ -895,15 +895,15 @@
 
 
     def subparser_utr_refine(self):
         """Add subparser for UTRREfine cmd"""
 
         sbp = self.subparsers.add_parser(
                 'utr_refine',
-                help='utr_refine help'
+                help='Refine UTR boundaries'
         )
         sbp.add_argument(
                 "Gff_genes",
                 help="Gene Annotation file in GFF/GTF file format to \
                       add/correct UTRs",
                 type=str
         )
@@ -947,15 +947,15 @@
 
 
     def subparser_aed_compare(self):
         """Add subparser for AEDCompare cmd"""
 
         sbp = self.subparsers.add_parser(
                 'aed_compare',
-                help='aed help'
+                help='Compare annotation sets based on their AED scores'
         )
         sbp.add_argument(
                 "fof",
                 help="File of files, <GFF with AED tags>TAB<source>",
                 type=str
         )
         sbp.add_argument(
@@ -971,15 +971,15 @@
 
 
     def subparser_aed_strand_annotation_filter(self):
         """Add subparser for StrandAnnotationFilter cmd"""
 
         sbp = self.subparsers.add_parser(
                 'aed_strand_annotation_filter',
-                help='aed help'
+                help='Remove opposite overlapping annotations based on AED scores'
         )
         sbp.add_argument(
                 "Input",
                 help="GFF File with AED tags",
                 type=str
         )
         sbp.add_argument(
@@ -993,15 +993,15 @@
 
 
     def subparser_exonerate_to_gff(self):
         """Add subparser for ExonerateToGff cmd"""
 
         sbp = self.subparsers.add_parser(
                 'exonerate_to_gff',
-                help='transform exonerate output to gff format',
+                help='Transform exonerate output to gff format',
                 description="RUN exonerate with:\
                              exonerate --model p2g --showvulgar no \
                              --showalignment no --showquerygff no \
                              --showtargetgff yes --percent 80 --ryo \
                              \"AveragePercentIdentity: %pi\n\" \
                              protein_db.pep target_genome.fasta"
         )
@@ -1029,15 +1029,15 @@
         return sbp
 
     def subparser_rename(self):
         """Add subparser for Rename cmd"""
 
         sbp = self.subparsers.add_parser(
                 'rename',
-                help='rename gene name with pattern'
+                help='Rename gene name with pattern'
         )
         sbp.add_argument(
                 "Gff_genes",
                 help="Gene Annotation file in GFF/GTF file",
                 type=str
         )
         sbp.add_argument(
@@ -1116,14 +1116,49 @@
                 default=0.6,
                 type=float
         )
         sbp.set_defaults(command=cmd.Clusterize)
 
         return sbp
 
+    def subparser_curation(self):
+        """Add subparser for Curation cmd"""
+
+        sbp = self.subparsers.add_parser(
+                'curation',
+                help='Define priorities, classify genes for manual \
+                        control or modification'
+        )
+        sbp.add_argument(
+                "Input",
+                help="GFF File with AED tags",
+                type=str
+        )
+        sbp.add_argument(
+                "Output",
+                help="GFF File with new curation tag",
+                type=str
+        )
+        sbp.add_argument(
+                "--graphout",
+                help="output filename of the graph, default=curation.png",
+                type=str,
+                default='curation.png'
+        )
+        sbp.add_argument(
+                "--graphtitle",
+                help="output title of the graph, default=AED categories \
+                      for manual curation",
+                type=str,
+                default='AED categories for manual curation'
+        )
+        sbp.set_defaults(command=cmd.Curation)
+
+        return sbp
+
 
 def main():
     """script entry point"""
 
     i = ArgParse()
     i.load_all_subparsers()
     args = i.parser.parse_args()
@@ -1138,22 +1173,25 @@
     logging.getLogger().setLevel(log_level)
 
     if args.procs > 1:
         cmd.Command.NB_CPUS = min(args.procs, multiprocessing.cpu_count()-1)
         logging.info("Multi-processs requested: %s procs will be used",
                      cmd.Command.NB_CPUS)
 
+    if 'command' not in args:
+        i.parser.print_help()
+        sys.exit(1)
+
     try:
         command = args.command(args)
         command.run()
-    except Exception as e:
-        print(e)
+    except RuntimeError as error:
+        #print(error)
         i.parser.print_help()
         sys.exit(1)
-#        raise
 
 
 
 def exe():
     """Delegate to script or class"""
 
     if __name__ == "__main__":
```

### Comparing `ingenannot-0.0.7/ingenannot/utils/__init__.py` & `ingenannot-0.0.8/ingenannot/utils/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -375,14 +375,15 @@
             transcripts = []
             for gene in cl.genes:
                 transcripts.extend(gene.lTranscripts)
             m = MetaGene(i,seqid, start, end, transcripts)
             # DEBUG add for comapre (test recursif !!!)
             m.genes = cl.genes
             lMetagenes.append(m)
+        logging.info(f"{len(lMetagenes)} metagenes built")
         return lMetagenes
 
 
 
     @staticmethod
     def statistics(genes, genome=''):
         '''Compute gene metrics'''
```

### Comparing `ingenannot-0.0.7/ingenannot/utils/annot_edit_distance.py` & `ingenannot-0.0.8/ingenannot/utils/annot_edit_distance.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/utils/effector_predictor.py` & `ingenannot-0.0.8/ingenannot/utils/effector_predictor.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/utils/em_operators.py` & `ingenannot-0.0.8/ingenannot/utils/em_operators.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/utils/gene_builder.py` & `ingenannot-0.0.8/ingenannot/utils/gene_builder.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/utils/gff_reader.py` & `ingenannot-0.0.8/ingenannot/utils/gff_reader.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/utils/graphics.py` & `ingenannot-0.0.8/ingenannot/utils/graphics.py`

 * *Files 9% similar despite different names*

```diff
@@ -93,30 +93,25 @@
                     if evidence == "pr":
                         laed.append(tr.best_bx_evidence[1])
                     if evidence == "best":
                         laed.append(min(tr.best_tr_evidence[1],tr.best_bx_evidence[1]))
             bins = np.arange(0.0,1.001,0.001)
             ax_histraw.hist(laed, bins=bins, cumulative=True, histtype="step", color = colors[i], label=src, linewidth=1.5)
             u = ax_histdensity.hist(laed, bins=bins, cumulative=True, histtype="step", density=True, color = colors[i], label=src, linewidth=1.5)
-            logging.info("{} with {} evidences, value at 0.5 AED: {}".format(src, evidence, u[0][500]))
+            logging.info("{} with {} evidence, value at 0.5 AED: {}".format(src, evidence, u[0][500]))
 
         h,l=ax_histraw.get_legend_handles_labels() # get labels and handles from histx  
         ax_legend.legend(h,l, fontsize=20, ncol=ncol, mode="expand", loc="lower center")
         ax_legend.grid(False)
         ax_legend.set_facecolor('w')
         ax_legend.axis('off')
         canvas = FigureCanvasAgg(fig)
         canvas.print_figure(out, dpi=80)
 
 
-
-
-
-
-
     @staticmethod
     def plot_distribution(lxs, lys, out="", title="", xax="", yax="",
             color="blue", legend="", grid=None):
         """Draw a simple Distribution"""
 
         fig = plt.Figure(figsize=(20,20))
         fig.suptitle(title, fontsize=32)
@@ -201,29 +196,23 @@
             ax.text(aedtr_filtering/2,1-((1-aedpr_filtering)/2)-0.05,lt_no_penalty,size=20,ha="center", va="center", bbox=dict(boxstyle="round",ec=(0,0,0), fc=(.5, 1., 1.)))
             ax.text(1-((1-aedtr_filtering)/2),1-((1-aedpr_filtering)/2)-0.05,rt_no_penalty,size=20,ha="center", va="center", bbox=dict(boxstyle="round",ec=(0.0,0,0), fc=(.5, 1., 1.)))
 
         ax.set_xlabel("AED with transcript evidence", fontsize=20)
         ax.set_ylabel("AED with protein evidence", fontsize=20)
         ax.tick_params(labelsize=15)
 
-        #ax.margins(0.02)
-        #ax.set_xlim((0,1))
-        #ax.set_ylim((0,1))
-
         bins = np.arange(0.0,1.01,0.01)
         ax_histx.hist(laed[0], bins=bins, color = '#36953a', edgecolor = 'black', label="AED transcripts")
         ax_histx.vlines(aedtr_filtering, 0, 1, transform=ax_histx.get_xaxis_transform(), colors='r', linestyle="dashed")
         ax_histx.tick_params(labelsize=12)
         ax_histx.set_ylabel("Nb. Transcripts (transcript evidence)", fontsize=20)
-        #ax_histx.legend(fontsize=20)
         ax_histy.hist(laed[1], bins=bins, color = '#fc4b67', edgecolor = 'black', orientation='horizontal', label="AED proteins")
         ax_histy.hlines(aedpr_filtering, 0, 1, transform=ax_histy.get_yaxis_transform(), colors='r', linestyle="dashed")
         ax_histy.tick_params(labelsize=12)
         ax_histy.set_xlabel("Nb. Transcripts (protein evidence)", fontsize=20)
-        #ax_histy.legend(fontsize=20)
 
         h,l=ax_histx.get_legend_handles_labels() # get labels and handles from histx  
         hy,ly=ax_histy.get_legend_handles_labels() # get labels and handles from histy
         h.extend(hy)
         l.extend(ly)
         ax_legend.legend(h,l, fontsize=20)
         # Hide grid lines
@@ -233,7 +222,51 @@
         #ax_legend.set_yticks([])
         # change background color
         ax_legend.set_facecolor('w')
         ax_legend.axis('off')
 
         canvas = FigureCanvasAgg(fig)
         canvas.print_figure(out, dpi=80)
+
+
+    @staticmethod
+    def plot_curation_scatter_hist(laed, out="", legend="", title=""):
+        """scatter plot of AEDs with histograms"""
+
+        plt.style.use('bmh')
+
+        fig = plt.Figure(figsize=(20,20))
+        # add gridspec
+        gs = fig.add_gridspec(3,2,width_ratios=(7, 2), height_ratios=(2, 7,2),
+                                      left=0.06, right=0.96, bottom=0.0, top=0.96,
+                                                            wspace=0.1, hspace=0.1)
+        ax = fig.add_subplot(gs[1, 0])
+        ax_histx = fig.add_subplot(gs[0, 0], sharex=ax)
+        ax_histy = fig.add_subplot(gs[1, 1], sharey=ax)
+        ax_legend = fig.add_subplot(gs[2, 0])
+
+        colors=['blue','red','green','maroon','black','orange','purple']
+        for idx,area in enumerate(laed):
+            ax.scatter(area[0],area[1], color=colors[idx], alpha=0.5)
+        # By using ``transform=vax.get_xaxis_transform()`` the y coordinates are scaled
+        ax.set_xlabel("AED with transcript evidence", fontsize=14)
+        ax.set_ylabel("AED with protein evidence", fontsize=14)
+        ax.tick_params(labelsize=15)
+
+        bins = np.arange(0.0,1.01,0.01)
+        colors=['blue','red','green','maroon','black','orange','purple']
+        ax_histx.hist([i[0] for i in laed], bins=bins, color = colors, edgecolor = 'black', label=legend, stacked=True)
+        ax_histx.tick_params(labelsize=12)
+        ax_histx.set_ylabel("Nb. Transcripts (transcript evidence)", fontsize=14)
+        ax_histx.set_title(title,fontsize=22)
+        ax_histy.hist([i[1] for i in laed], bins=bins, color = colors, edgecolor = 'black',orientation='horizontal', label="AED proteins", stacked=True)
+        ax_histy.tick_params(labelsize=12)
+        ax_histy.set_xlabel("Nb. Transcripts (protein evidence)", fontsize=14)
+        h,l=ax_histx.get_legend_handles_labels() # get labels and handles from histx  
+        ax_legend.legend(h,l,fontsize=15, loc='center left')
+        # Hide grid lines
+        ax_legend.grid(False)
+        # change background color
+        ax_legend.set_facecolor('w')
+        ax_legend.axis('off')
+        canvas = FigureCanvasAgg(fig)
+        canvas.print_figure(out, dpi=80)
```

### Comparing `ingenannot-0.0.7/ingenannot/utils/so_splicing_classifier.py` & `ingenannot-0.0.8/ingenannot/utils/so_splicing_classifier.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/utils/statistics.py` & `ingenannot-0.0.8/ingenannot/utils/statistics.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,11 +76,11 @@
 
     @staticmethod
     def mean_median_distance(points,center):
 
         d = [] 
 
         for i,x in enumerate(points[0]):
-           d.append(math.sqrt(pow((points[0][i]-center[0]),2) + pow((points[1][i]-center[1]),2)))
+            d.append(math.sqrt(pow((points[0][i]-center[0]),2) + pow((points[1][i]-center[1]),2)))
         return np.mean(d), np.median(d)
```

### Comparing `ingenannot-0.0.7/ingenannot/utils/stats.py` & `ingenannot-0.0.8/ingenannot/utils/stats.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot/utils/tool_checker.py` & `ingenannot-0.0.8/ingenannot/utils/tool_checker.py`

 * *Files identical despite different names*

### Comparing `ingenannot-0.0.7/ingenannot.egg-info/PKG-INFO` & `ingenannot-0.0.8/ingenannot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ingenannot
-Version: 0.0.7
+Version: 0.0.8
 Summary: InGenAnnot: Inspection of Gene Annotation
 Home-page: https://forgemia.inra.fr/bioger/ingenannot
 Author: Nicolas Lapalu
 Author-email: nicolas.lapalu@inrae.fr
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX
@@ -37,15 +37,15 @@
 clusterize genes, to propose new loci sharing a list of transcripts.
 We define these new loci as 'meta-gene' and propose several options
 to clusterize them. We tried to summarize the pro and cons of classification feature type in the following table.
 
 ||pros|cons|
 |:--:|--|--|
 |`--clu-type gene`|detect problem of missens predictions|overlaps of UTR merge different genes, not suitable for compact genomes|
-|`--clu-type cds`|detect problem of missens predictions|could not correct splitted CDS|
+|`--clu-type cds`|detect problem of missens predictions|could not correct split CDS|
 |`--clu-type gene` `--clu-stranded`|resolve conflict between genes and possible non-coding RNA on the opposite strand|will not detect severe problem due to divergent prediction on opposite strand, overlaps of UTR merge different genes|
 |`--clu-type cds` `--clu-stranded`|resolve conflict between genes and possible non-coding RNA on the opposite strand|will not detect severe problem due to divergent prediction on opposite strand|
 
 In most cases, we recommended to use `--clu-type cds` with `--clu-stranded` to avoid gene merge. A post-process is implemented to remove overlapping CDS, keeping gene models with the best AED scores.
 
 
 ## Selection of best gene structures, evidence-driven with Annotation Edit Distance (AED)
@@ -89,17 +89,15 @@
 |0:N:N|All transcript-pairs share sequence in common and some share exon boundaries|![0:N:N](https://forgemia.inra.fr/bioger/ingenannot/raw/master/docs/img/0_N_N.png)|
 |0:0:N|All transcript-pairs share some exons in common|![0:0:N](https://forgemia.inra.fr/bioger/ingenannot/raw/master/docs/img/0_0_N.png)|
 
 As described above, the SO classification was originally based on exon boundaries,
 that could be highly problematic for de-novo annotations with poorly
 defined UTR parts. To avoid such problem, you can choose to perform
 the same classification based on CDS coordinates. In this case you 
-will obtained less biased results.  We tried
-to summarize the pro and cons of classification feature type in
-the following table.
+will obtained less biased results (See table above for pros/cons of clustering).
 
 
 ## Documentation: install, tools and use cases 
 
 `InGenAnnot` comes with multiple tools allowing analysis of your gene prediction datasets. You will be able to compare, select and annotate your genes with different tools [(link to documentation)](https://bioger.pages.mia.inra.fr/ingenannot/index.html). Full use cases are described step by step, such as:
 
 * [best gene selection](https://bioger.pages.mia.inra.fr/ingenannot/usecases/select_best_gene_models.html)
```

### Comparing `ingenannot-0.0.7/ingenannot.egg-info/SOURCES.txt` & `ingenannot-0.0.8/ingenannot.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -6,32 +6,26 @@
 ingenannot/version.py
 ingenannot.egg-info/PKG-INFO
 ingenannot.egg-info/SOURCES.txt
 ingenannot.egg-info/dependency_links.txt
 ingenannot.egg-info/entry_points.txt
 ingenannot.egg-info/requires.txt
 ingenannot.egg-info/top_level.txt
-ingenannot/commands/AddIsoforms.py
-ingenannot/commands/StringtieFilter.py
-ingenannot/commands/StringtieJaclip.py
-ingenannot/commands/StringtieRefine.py
-ingenannot/commands/StringtieStats.py
-ingenannot/commands/SupportIsoformFilter.py
 ingenannot/commands/__init__.py
 ingenannot/commands/add_sqanti3_isoforms.py
 ingenannot/commands/aed.py
 ingenannot/commands/aed_compare.py
 ingenannot/commands/clusterize.py
 ingenannot/commands/command.py
 ingenannot/commands/compare.py
+ingenannot/commands/curation.py
 ingenannot/commands/effector_predictor_cmd.py
 ingenannot/commands/exonerate_to_gff.py
 ingenannot/commands/filter.py
 ingenannot/commands/isoform_ranking.py
-ingenannot/commands/reduce.py
 ingenannot/commands/rename.py
 ingenannot/commands/rescue_effectors.py
 ingenannot/commands/select.py
 ingenannot/commands/so_classification.py
 ingenannot/commands/strand_annotation_filter.py
 ingenannot/commands/utr_refine.py
 ingenannot/commands/validate.py
```

### Comparing `ingenannot-0.0.7/setup.py` & `ingenannot-0.0.8/setup.py`

 * *Files identical despite different names*

