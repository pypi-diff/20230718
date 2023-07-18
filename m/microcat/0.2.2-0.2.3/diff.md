# Comparing `tmp/microcat-0.2.2.tar.gz` & `tmp/microcat-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "microcat-0.2.2.tar", last modified: Sat Jul 15 11:59:05 2023, max compression
+gzip compressed data, was "microcat-0.2.3.tar", last modified: Tue Jul 18 07:31:40 2023, max compression
```

## Comparing `microcat-0.2.2.tar` & `microcat-0.2.3.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.344248 microcat-0.2.2/
--rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.2.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      396 2023-07-08 04:52:18.000000 microcat-0.2.2/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-15 11:59:05.344248 microcat-0.2.2/PKG-INFO
--rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.2.2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.340248 microcat-0.2.2/microcat/
--rwxrwxr-x   0 root         (0) root         (0)       73 2023-07-15 11:59:01.000000 microcat-0.2.2/microcat/__about__.py
--rwxrwxr-x   0 root         (0) root         (0)      968 2023-07-15 11:56:59.000000 microcat-0.2.2/microcat/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13920 2023-07-13 13:02:07.000000 microcat-0.2.2/microcat/chemistry_defs.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.340248 microcat-0.2.2/microcat/config/
--rw-r--r--   0 root         (0) root         (0)     3300 2023-07-13 12:54:29.000000 microcat-0.2.2/microcat/config/config.yaml
--rwxr-xr-x   0 root         (0) root         (0)     9364 2023-07-09 15:21:44.000000 microcat-0.2.2/microcat/configer.py
--rwxr-xr-x   0 root         (0) root         (0)    35789 2023-07-15 11:49:55.000000 microcat-0.2.2/microcat/corer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.340248 microcat-0.2.2/microcat/envs/
--rw-r--r--   0 root         (0) root         (0)      125 2023-07-13 08:58:40.000000 microcat-0.2.2/microcat/envs/kmer_python.yaml
--rw-r--r--   0 root         (0) root         (0)      388 2023-07-13 08:58:14.000000 microcat-0.2.2/microcat/envs/kmer_qc.yaml
--rw-rw-r--   0 root         (0) root         (0)      164 2023-06-14 02:38:19.000000 microcat-0.2.2/microcat/envs/kraken2.yaml
--rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.2.2/microcat/envs/krakenuniq.yaml
--rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.2.2/microcat/envs/metaphlan.yaml
--rwxr-xr-x   0 root         (0) root         (0)      145 2023-07-06 06:38:14.000000 microcat-0.2.2/microcat/envs/pathseq.yaml
--rw-r--r--   0 root         (0) root         (0)      110 2023-07-03 07:57:02.000000 microcat-0.2.2/microcat/envs/star.yaml
--rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.2.2/microcat/envs/trimming.yaml
--rwxr-xr-x   0 root         (0) root         (0)     5065 2023-07-08 04:34:53.000000 microcat-0.2.2/microcat/prepare.py
--rwxr-xr-x   0 root         (0) root         (0)    21400 2023-06-16 11:13:16.000000 microcat-0.2.2/microcat/rich_agrpase.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.340248 microcat-0.2.2/microcat/rules/
--rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.2.2/microcat/rules/ERCC.smk
--rw-r--r--   0 root         (0) root         (0)     2225 2023-06-10 01:41:24.000000 microcat-0.2.2/microcat/rules/build.smk
--rw-r--r--   0 root         (0) root         (0)    40959 2023-06-25 01:22:49.000000 microcat-0.2.2/microcat/rules/classfier.smk
--rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.2.2/microcat/rules/database.smk
--rw-r--r--   0 root         (0) root         (0)    38249 2023-07-15 11:51:50.000000 microcat-0.2.2/microcat/rules/host.smk
--rwxr-xr-x   0 root         (0) root         (0)    11923 2023-07-13 09:56:14.000000 microcat-0.2.2/microcat/sample.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.344248 microcat-0.2.2/microcat/scripts/
--rwxrwxrwx   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.2.2/microcat/scripts/INVADEseq.py
--rwxrwxrwx   0 root         (0) root         (0)     2002 2023-06-20 08:08:16.000000 microcat-0.2.2/microcat/scripts/add_tags_to_PathSeq_bam.py
--rwxrwxrwx   0 root         (0) root         (0)     1947 2023-06-20 08:42:02.000000 microcat-0.2.2/microcat/scripts/create_hdf5.py
--rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.2.2/microcat/scripts/extract_kraken_reads.py
--rwxrwxrwx   0 root         (0) root         (0)     3850 2023-06-26 01:17:41.000000 microcat-0.2.2/microcat/scripts/extract_microbiome_output.R
--rw-r--r--   0 root         (0) root         (0)     1931 2023-07-13 06:06:55.000000 microcat-0.2.2/microcat/scripts/generate_PE_manifest_file.py
--rwxrwxrwx   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.2.2/microcat/scripts/get_ncbi_domains.py
--rwxrwxrwx   0 root         (0) root         (0)     1186 2023-06-26 01:14:49.000000 microcat-0.2.2/microcat/scripts/krak2_output_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.2.2/microcat/scripts/kraken2mpa.py
--rwxrwxrwx   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.2.2/microcat/scripts/kraken2sc.py
--rwxrwxrwx   0 root         (0) root         (0)     2421 2023-06-21 06:28:42.000000 microcat-0.2.2/microcat/scripts/microcat_bam_handle.Rmd
--rwxrwxrwx   0 root         (0) root         (0)     4698 2023-06-26 01:13:57.000000 microcat-0.2.2/microcat/scripts/sample_denosing.R
--rwxrwxrwx   0 root         (0) root         (0)    15666 2023-06-26 01:14:02.000000 microcat-0.2.2/microcat/scripts/sckmer_unpaired.R
--rwxrwxrwx   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.2.2/microcat/scripts/spilt_bam_by_tag.py
--rwxrwxrwx   0 root         (0) root         (0)     3082 2023-07-13 06:04:44.000000 microcat-0.2.2/microcat/scripts/split_Starsolo_BAM_by_RG.py
--rw-r--r--   0 root         (0) root         (0)    13555 2023-07-15 04:01:31.000000 microcat-0.2.2/microcat/scripts/starsolo_tenX_auto.sh
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.344248 microcat-0.2.2/microcat/snakefiles/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.2.2/microcat/snakefiles/bulk_wf.smk
--rw-r--r--   0 root         (0) root         (0)     1941 2023-07-13 07:09:46.000000 microcat-0.2.2/microcat/snakefiles/scRNA_wf.smk
--rw-r--r--   0 root         (0) root         (0)    21138 2023-07-13 07:08:00.000000 microcat-0.2.2/microcat/snakefiles/scRNA_wf_test.smk
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.2.2/microcat/snakefiles/spatial_wf.smk
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-15 11:59:05.340248 microcat-0.2.2/microcat.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1298 2023-07-15 11:59:05.000000 microcat-0.2.2/microcat.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1552 2023-07-15 11:59:05.000000 microcat-0.2.2/microcat.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-15 11:59:05.000000 microcat-0.2.2/microcat.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       49 2023-07-15 11:59:05.000000 microcat-0.2.2/microcat.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       70 2023-07-15 11:59:05.000000 microcat-0.2.2/microcat.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-07-15 11:59:05.000000 microcat-0.2.2/microcat.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       71 2023-07-06 07:41:48.000000 microcat-0.2.2/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-15 11:59:05.344248 microcat-0.2.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2273 2023-07-08 04:52:22.000000 microcat-0.2.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:31:40.666035 microcat-0.2.3/
+-rw-r--r--   0 root         (0) root         (0)    34599 2023-06-09 02:02:59.000000 microcat-0.2.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      396 2023-07-08 04:52:18.000000 microcat-0.2.3/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-18 07:31:40.666035 microcat-0.2.3/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)      383 2023-05-18 11:49:26.000000 microcat-0.2.3/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:31:40.398038 microcat-0.2.3/microcat/
+-rwxrwxr-x   0 root         (0) root         (0)       73 2023-07-18 07:31:28.000000 microcat-0.2.3/microcat/__about__.py
+-rwxrwxr-x   0 root         (0) root         (0)      968 2023-07-15 12:02:38.000000 microcat-0.2.3/microcat/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13920 2023-07-13 13:02:07.000000 microcat-0.2.3/microcat/chemistry_defs.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:31:40.406038 microcat-0.2.3/microcat/config/
+-rw-r--r--   0 root         (0) root         (0)     3559 2023-07-18 07:31:22.000000 microcat-0.2.3/microcat/config/config.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     9364 2023-07-18 06:32:17.000000 microcat-0.2.3/microcat/configer.py
+-rwxr-xr-x   0 root         (0) root         (0)    39553 2023-07-18 07:30:58.000000 microcat-0.2.3/microcat/corer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:31:40.466037 microcat-0.2.3/microcat/envs/
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-18 02:54:51.000000 microcat-0.2.3/microcat/envs/kmer_python.yaml
+-rw-r--r--   0 root         (0) root         (0)      388 2023-07-18 07:31:19.000000 microcat-0.2.3/microcat/envs/kmer_qc.yaml
+-rw-rw-r--   0 root         (0) root         (0)      164 2023-06-14 02:38:19.000000 microcat-0.2.3/microcat/envs/kraken2.yaml
+-rw-r--r--   0 root         (0) root         (0)      133 2023-05-31 02:41:36.000000 microcat-0.2.3/microcat/envs/krakenuniq.yaml
+-rw-r--r--   0 root         (0) root         (0)      109 2023-06-03 12:24:08.000000 microcat-0.2.3/microcat/envs/metaphlan.yaml
+-rwxr-xr-x   0 root         (0) root         (0)      145 2023-07-06 06:38:14.000000 microcat-0.2.3/microcat/envs/pathseq.yaml
+-rw-r--r--   0 root         (0) root         (0)      110 2023-07-03 07:57:02.000000 microcat-0.2.3/microcat/envs/star.yaml
+-rw-r--r--   0 root         (0) root         (0)      140 2023-05-31 02:41:36.000000 microcat-0.2.3/microcat/envs/trimming.yaml
+-rwxr-xr-x   0 root         (0) root         (0)     5065 2023-07-08 04:34:53.000000 microcat-0.2.3/microcat/prepare.py
+-rwxr-xr-x   0 root         (0) root         (0)    21400 2023-06-16 11:13:16.000000 microcat-0.2.3/microcat/rich_agrpase.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:31:40.502037 microcat-0.2.3/microcat/rules/
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-06-09 02:29:19.000000 microcat-0.2.3/microcat/rules/ERCC.smk
+-rw-r--r--   0 root         (0) root         (0)     2225 2023-06-10 01:41:24.000000 microcat-0.2.3/microcat/rules/build.smk
+-rw-r--r--   0 root         (0) root         (0)    41057 2023-07-18 05:58:37.000000 microcat-0.2.3/microcat/rules/classfier.smk
+-rw-r--r--   0 root         (0) root         (0)     3981 2023-06-07 01:22:00.000000 microcat-0.2.3/microcat/rules/database.smk
+-rw-r--r--   0 root         (0) root         (0)    38996 2023-07-18 05:58:43.000000 microcat-0.2.3/microcat/rules/host.smk
+-rwxr-xr-x   0 root         (0) root         (0)    11923 2023-07-13 09:56:14.000000 microcat-0.2.3/microcat/sample.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:31:40.662035 microcat-0.2.3/microcat/scripts/
+-rwxrwxrwx   0 root         (0) root         (0)    15479 2023-06-08 03:30:56.000000 microcat-0.2.3/microcat/scripts/INVADEseq.py
+-rwxrwxrwx   0 root         (0) root         (0)     2002 2023-06-20 08:08:16.000000 microcat-0.2.3/microcat/scripts/add_tags_to_PathSeq_bam.py
+-rwxrwxrwx   0 root         (0) root         (0)     1947 2023-06-20 08:42:02.000000 microcat-0.2.3/microcat/scripts/create_hdf5.py
+-rwxrwxrwx   0 root         (0) root         (0)    19072 2023-06-07 07:14:07.000000 microcat-0.2.3/microcat/scripts/extract_kraken_reads.py
+-rwxrwxrwx   0 root         (0) root         (0)     3776 2023-07-18 02:36:09.000000 microcat-0.2.3/microcat/scripts/extract_microbiome_output.R
+-rw-r--r--   0 root         (0) root         (0)     1931 2023-07-13 06:06:55.000000 microcat-0.2.3/microcat/scripts/generate_PE_manifest_file.py
+-rwxrwxrwx   0 root         (0) root         (0)     7896 2023-06-03 12:24:08.000000 microcat-0.2.3/microcat/scripts/get_ncbi_domains.py
+-rwxrwxrwx   0 root         (0) root         (0)     1112 2023-07-17 14:48:20.000000 microcat-0.2.3/microcat/scripts/krak2_output_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)     6942 2023-06-07 07:15:43.000000 microcat-0.2.3/microcat/scripts/kraken2mpa.py
+-rwxrwxrwx   0 root         (0) root         (0)    14784 2023-06-07 07:15:24.000000 microcat-0.2.3/microcat/scripts/kraken2sc.py
+-rwxrwxrwx   0 root         (0) root         (0)     2421 2023-06-21 06:28:42.000000 microcat-0.2.3/microcat/scripts/microcat_bam_handle.Rmd
+-rwxrwxrwx   0 root         (0) root         (0)     4624 2023-07-17 14:25:46.000000 microcat-0.2.3/microcat/scripts/sample_denosing.R
+-rwxrwxrwx   0 root         (0) root         (0)    15592 2023-07-17 14:25:42.000000 microcat-0.2.3/microcat/scripts/sckmer_unpaired.R
+-rwxrwxrwx   0 root         (0) root         (0)     2367 2023-06-03 12:24:08.000000 microcat-0.2.3/microcat/scripts/spilt_bam_by_tag.py
+-rwxrwxrwx   0 root         (0) root         (0)     3082 2023-07-13 06:04:44.000000 microcat-0.2.3/microcat/scripts/split_Starsolo_BAM_by_RG.py
+-rw-r--r--   0 root         (0) root         (0)    13281 2023-07-18 02:03:42.000000 microcat-0.2.3/microcat/scripts/starsolo_tenX_auto.sh
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:31:40.666035 microcat-0.2.3/microcat/snakefiles/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:37:58.000000 microcat-0.2.3/microcat/snakefiles/bulk_wf.smk
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-07-15 12:05:17.000000 microcat-0.2.3/microcat/snakefiles/scRNA_wf.smk
+-rw-r--r--   0 root         (0) root         (0)    21138 2023-07-13 07:08:00.000000 microcat-0.2.3/microcat/snakefiles/scRNA_wf_test.smk
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-18 11:38:06.000000 microcat-0.2.3/microcat/snakefiles/spatial_wf.smk
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 07:31:40.406038 microcat-0.2.3/microcat.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1298 2023-07-18 07:31:40.000000 microcat-0.2.3/microcat.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1552 2023-07-18 07:31:40.000000 microcat-0.2.3/microcat.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 07:31:40.000000 microcat-0.2.3/microcat.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       49 2023-07-18 07:31:40.000000 microcat-0.2.3/microcat.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       70 2023-07-18 07:31:40.000000 microcat-0.2.3/microcat.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-07-18 07:31:40.000000 microcat-0.2.3/microcat.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       71 2023-07-06 07:41:48.000000 microcat-0.2.3/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 07:31:40.666035 microcat-0.2.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2273 2023-07-08 04:52:22.000000 microcat-0.2.3/setup.py
```

### Comparing `microcat-0.2.2/LICENSE` & `microcat-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/PKG-INFO` & `microcat-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.2.2
+Version: 0.2.3
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.2.2/microcat/__init__.py` & `microcat-0.2.3/microcat/__init__.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/chemistry_defs.json` & `microcat-0.2.3/microcat/chemistry_defs.json`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/config/config.yaml` & `microcat-0.2.3/microcat/config/config.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 
   host:
     cellranger:
       do: false
       reference: "/data/database/refdata-gex-GRCh38-2020-A"
       variousParams: ""
-      threads: 40
     starsolo:
       do: True
       reference: "/data/database/STAR_refdata-gex-GRCh38-2020-A"
       barcode:
         soloCBwhitelist:
         soloCBstart:
         soloCBlen:
@@ -35,48 +34,40 @@
         clipAdapterType:
         outFilterScoreMin:
         soloMultiMappers:
       soloType: 
       soloAdapterSequence: ""
       soloStrand:
       variousParams: ""
-      threads: 40
 
   classifier:
     kraken2uniq:
       do: true
       kraken2_database: "/data/database/kraken2_RefSeqV217_Complete_Chrom_nont"
       threads: 40
-      mem_mb: 200000
     pathseq:
       do: false
       microbe_bwa_image: /data/database/pathseq_database/refv218/microbiome_RefseqV218_Compelete-Chromon.fasta.img
       microbe_dict: /data/database/pathseq_database/refv218/microbiome_RefseqV218_Compelete-Chromon.dict
       host_bfi: /data/database/pathseq_database/refv218/pathseq_resources_pathseq_host.bfi
       taxonomy_db: /data/database/pathseq_database/refv218/microbiome_RefseqV218_Compelete-Chromon.db
       host_bwa_image: /data/database/pathseq_database/refv218/pathseq_resources_pathseq_host.fa.img
-      threads: 24
-      mem_mb: 200000
     pathseqscore: ""
     
     metaphlan:
       do: false
-      threads: 24
       sequence_type: fastq
       analysis_type: "rel_ab_w_read_stats"
       bowtie2db: "/data/database/metaphlan_database/"
       db_index: "mpa_vOct22_CHOCOPhlAnSGB_202212"
       metaphlan_other_params: ''
-
     krakenuniq:
       do: false
       krakenuniq_database: "/data/database/krakenuniq_database/krakuniq_refseqV218/"
-      threads: 40
       estimate_precision: 12
-      mem_mb: 200000
     sckmer:
       cb_len: 16
       umi_len: 10
       min_frac: 0.5
       kmer_len: 35
       nsample: 1000
 
@@ -106,15 +97,40 @@
   krakenuniq: ../envs/krakenuniq.yaml
   pathseq: ../envs/pathseq.yaml
   metaphlan: ../envs/metaphlan.yaml
   kmer_qc: ../envs/kmer_qc.yaml
   kmer_python: ../envs/kmer_python.yaml
   star: ../envs/star.yaml
 
-
+resources:
+  cellranger:
+    threads: 40
+    mem_mb: 100000
+  starsolo:
+    threads: 40
+    mem_mb: 100000
+  samtools_extract:
+    threads: 20
+    mem_mb: 40000
+  paired_bam_to_fastq:
+    threads: 20
+    mem_mb: 40000
+  kraken2uniq:
+    threads: 40
+    mem_mb: 300000
+  krakenuniq:
+    threads: 40
+    mem_mb: 100000
+  metaphlan:
+    threads: 20
+    mem_mb: 100000
+  pathseq:
+    threads: 24
+    mem_mb: 200000
+  
 
 
 scripts:
   extract_microbiome_output: scripts/extract_microbiome_output.R
   kraken2mpa: scripts/kraken2mpa.py
   kraken2sc: scripts/kraken2sc.py
   extract_kraken_reads: scripts/extract_kraken_reads.py
```

### Comparing `microcat-0.2.2/microcat/configer.py` & `microcat-0.2.3/microcat/configer.py`

 * *Files 0% similar despite different names*

```diff
@@ -138,15 +138,15 @@
                         print("Skip updating this dir.")
                         continue
                 # Otherwise copy the source directory to the target directory
                 else:
                     shutil.copytree(os.path.join(self.profiles_dir, i), dest_dir)
         else:
             # Handle the case when 'profiles' directory does not exist
-            print("\033[93mWarning: The 'profiles' directory does not exist in the original folder.")
+            print("\033[93mWARNING: The 'profiles' directory does not exist in the original folder.")
             print("You can only run the program locally using the --run-local option.")
             print("If you want to run it on a cluster, please refer to the documentation for the 'cluster run' section.\033[0m")
             print("Skipping the profiles directory.")
 
     def get_config(self):
         """
         Reads the default configuration file config.yaml and returns the parsed configuration
```

### Comparing `microcat-0.2.2/microcat/corer.py` & `microcat-0.2.3/microcat/corer.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import argparse
 import os
 import subprocess
 import sys
 import textwrap
 from io import StringIO
 import pandas as pd
+import psutil
 import json
 import microcat
 import re
 import sys
 from typing import TYPE_CHECKING, Callable, ClassVar, Iterable, Iterator
 
 # rich is only used to display help. It is imported inside the functions in order
@@ -479,15 +480,15 @@
     if args.workdir:
         # Create a MicrocatConfig object using the provided working directory
         project = microcat.MicrocatConfig(args.workdir)
 
 
         # Check if the working directory already exists
         if os.path.exists(args.workdir):
-            print(f"Warning: The working directory '{args.workdir}' already exists.")
+            print(f"WARNING: The working directory '{args.workdir}' already exists.")
             proceed = input("Do you want to proceed? (y/n): ").lower()
             if proceed != 'y':
                 print("Aborted.")
                 sys.exit(1)
 
         # Print the project structure and create the necessary subdirectories
         print(project.__str__())
@@ -524,15 +525,15 @@
         microcat.update_config(
             project.config_file, project.new_config_file, conf, remove=False
         )
 
         print("\033[32mNOTE: \nCongfig.yaml reset to default values.\033[0m")
     else:
         # If the user didn't provide a working directory, print an error message and exit
-        print("Please supply a workdir!")
+        print("\033[91mERROR:Please supply a workdir!\033[0m")
         sys.exit(-1)
 
 
 def run_snakemake(args, unknown, snakefile, workflow):
     """
     Use subprocess.Popen to run the MicroCAT workflow.
 
@@ -540,15 +541,15 @@
         args (argparse.Namespace): An object containing parsed command-line arguments.
     """
     # Parse the YAML configuration file
     conf = microcat.parse_yaml(args.config)
 
     # Check if the sample list is provided, exit if not
     if not os.path.exists(conf["params"]["samples"]):
-        print("Please specific samples list on init step or change config.yaml manualy")
+        print("\033[91mERROR:Please specific samples list on init step or change config.yaml manualy.\033[0m")
         sys.exit(1)
 
     # Prepare the command list for running Snakemake
     cmd = [
         "snakemake",
         "--snakefile",
         snakefile,
@@ -583,17 +584,91 @@
         
         # Add flags for listing tasks
         if args.list:
             cmd += ["--list"]
 
         # Add flags for running tasks locally
         elif args.run_local:
+            # Get the system's available resources
+            num_cores = psutil.cpu_count(logical=False)
+            mem_usage = round((float(psutil.virtual_memory().total)/1024/1024),2)
+            # Adjust the resource parameters based on available resources
+            cores_limit = int(num_cores * 0.75)
+            mem_limit = int(mem_usage * 0.75)
+
+            # Compare the requested resources with the limits
+            if args.cores > num_cores:
+                print("\033[93mWARNING: Maximum allowable cores is exceeded. Automatically set to 75% of the current available cores ({0}).\033[0m".format(cores_limit))
+                args.cores = cores_limit
+
+            # # Check if "--resources" is present in unknown arguments
+            # resources_index = unknown.index("--resources") if "--resources" in unknown else -1
+            # if resources_index != -1:
+            #     resources_args = unknown[resources_index + 1]
+            #     resources = {}
+            #     # Split the resources_args into key-value pairs and extract mem_mb value
+            #     for item in resources_args.split(" "):
+            #         key, value = item.split("=")
+            #         resources[key] = value
+                    
+            #         # Get user setting mem_mb
+            #         if key == "mem_mb":
+            #             user_mem_mb = value
+
+            #     if "mem_mb" not in resources:
+            #         user_mem_mb = None
+            # else:
+            #     user_mem_mb = None
+            # Check if "--resources" is present in unknown arguments
+            resources_index = None
+            for index, arg in enumerate(unknown):
+                if arg == "--resources":
+                    resources_index = index
+                    break
+
+            if resources_index is not None:
+                resources_args = unknown[resources_index + 1]
+                resources = {}
+
+                # Split the resources_args into key-value pairs
+                resources_items = resources_args.split()
+                
+                # Find the index of the next parameter after resources_args
+                next_parameter_index = resources_index + 2 if resources_index + 2 < len(unknown) else None
+                
+                # If there is a next parameter and it doesn't start with "--", include it in resources_items
+                if next_parameter_index is not None and not unknown[next_parameter_index].startswith("--"):
+                    resources_items.append(unknown[next_parameter_index])
+
+                # Extract key-value pairs from resources_items
+                for item in resources_items:
+                    key, value = item.split("=")
+                    resources[key] = value
+
+                    # Get user setting mem_mb
+                    if key == "mem_mb":
+                        user_mem_mb = value
+
+                if "mem_mb" not in resources:
+                    user_mem_mb = None
+            else:
+                user_mem_mb = None
+
+            # Check if mem_mb_value exceeds mem_usage or is None, and adjust it if necessary
+            if user_mem_mb is None or (int(user_mem_mb) > mem_limit or int(user_mem_mb) <= 0):
+                print("\033[93mWARNING: Maximum allowable memory is not set or exceeded. Automatically set to 75% of the current memory ({0}MB).\033[0m".format(mem_limit))
+                user_mem_mb = mem_limit
+                resources["mem_mb"] = user_mem_mb
+
+            # Create a string representation of the resources dictionary
+            resources_str = " ".join(["{0}={1}".format(key, value) for key, value in resources.items()])
             cmd += ["--cores", str(args.cores),
                     "--local-cores", str(args.local_cores),
-                    "--jobs", str(args.jobs)]
+                    "--jobs", str(args.jobs),
+                    "--resources", str(resources_str)]
         elif args.run_remote:
             profile_path = os.path.join("./profiles", args.cluster_engine)
             cmd += ["--profile", profile_path,
                     "--local-cores", str(args.local_cores),
                     "--jobs", str(args.jobs)]
         
         # Add flags for running tasks remotely
@@ -866,15 +941,15 @@
         required=False,
         choices=["starsolo","cellranger"],
         help="Which rmhoster used",
     )
     parser_init.add_argument(
         "--chemistry",
         type=str,
-        default="tenx_auto",
+        default=None,
         choices=["smartseq", "smartseq2", "tenx_3pv1", "tenx_3pv2", "tenx_3pv3","seqwell","tenx_auto","dropseq","tenx_multiome","tenx_5ppe","seqwell","celseq2"],
         help="Sequencing chemistry option, required when host is starsolo",
     )
     
     parser_init.add_argument(
         "--classifier",
         nargs="+",
@@ -933,15 +1008,15 @@
     parser_scrna_wf.add_argument(
         "task",
         metavar="TASK",
         nargs="?",
         type=str,
         default="all",
         choices=WORKFLOWS_SCRNA,
-        help="pipeline end point. Allowed values are " + ", ".join(WORKFLOWS_MAG),
+        help="pipeline end point. Allowed values are " + ", ".join(WORKFLOWS_SCRNA),
     )
     parser_scrna_wf.set_defaults(func=scRNA_wf)
 
     args, unknown = parser.parse_known_args()
         
     if hasattr(args, 'host') and args.host == "starsolo" and args.chemistry is None:
         parser_init.error("--chemistry option is required when host is starsolo")
```

### Comparing `microcat-0.2.2/microcat/prepare.py` & `microcat-0.2.3/microcat/prepare.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/rich_agrpase.py` & `microcat-0.2.3/microcat/rich_agrpase.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/rules/ERCC.smk` & `microcat-0.2.3/microcat/rules/ERCC.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/rules/build.smk` & `microcat-0.2.3/microcat/rules/build.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/rules/classfier.smk` & `microcat-0.2.3/microcat/rules/classfier.smk`

 * *Files 1% similar despite different names*

```diff
@@ -81,18 +81,18 @@
         unmapped_bam_sorted_file =os.path.join(
         config["output"]["host"],
         "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam")
     output:
         unmapped_fastq = os.path.join(
             config["output"]["host"],
             "unmapped_host/{sample}/{sample}_unmappped2human_bam.fastq")
-    # threads:
-    #     16
+    threads:
+        config["resources"]["paired_bam_to_fastq"]["threads"]
     resources:
-        mem_mb=100000
+        mem_mb=config["resources"]["paired_bam_to_fastq"]["mem_mb"]
     priority: 11
     conda:
         config["envs"]["star"]
     shell:
         '''
         samtools fastq --threads {threads}  -n {input.unmapped_bam_sorted_file}  > {output.unmapped_fastq}
         '''
@@ -129,20 +129,19 @@
             #since kraken2 acquire specific input fomrat "#fq",so we put it it params
             # krak2_classified_output=os.path.join(
             #     config["output"]["classifier"],
             #     "classified_output/{sample}/{sample}_kraken2_classified#.fq"),
             # krak2_unclassified_output=os.path.join(
             #     config["output"]["classifier"],
             #     "unclassified_output/{sample}/{sample}_kraken2_unclassified#.fq")
-
         resources:
-            mem_mb=config["params"]["classifier"]["kraken2uniq"]["mem_mb"]
+            mem_mb=config["resources"]["kraken2uniq"]["mem_mb"]
         priority: 12
         threads: 
-            config["params"]["classifier"]["kraken2uniq"]["threads"]
+            config["resources"]["kraken2uniq"]["threads"]
         benchmark:
             os.path.join(config["benchmarks"]["classifier"],
                         "rmhost_kraken2uniq/{sample}_kraken2uniq_classifier_benchmark.log")
         log:
             os.path.join(config["logs"]["classifier"],
                         "rmhost_kraken2uniq/{sample}_kraken2uniq_classifier.log")
         conda:
@@ -227,15 +226,14 @@
             8
         priority: 
             14
         conda:
             config["envs"]["kmer_qc"]
         shell:
             '''
-            pwd
             Rscript {params.extract_microbiome_output_script} \
             --output_file {input.krak2_output} \
             --kraken_report {input.krak2_report} \
             --mpa_report {input.krak2_mpa_report} \
             --extract_file {output.krak2_extracted_output}\
             --cores {threads} \
             --ntaxid 6000 \
@@ -405,24 +403,24 @@
                 config["output"]["classifier"],
                 "rmhost_krakenuniq_classified_output/{sample}/{sample}_krakenuniq_classified.fq"),
             krakenuniq_unclassified_output = os.path.join(
                 config["output"]["classifier"],
                 "rmhost_krakenuniq_unclassified_output/{sample}/{sample}_krakenuniq_unclassified.fq")
         params:
             database = config["params"]["classifier"]["krakenuniq"]["krakenuniq_database"],
-            threads=config["params"]["classifier"]["krakenuniq"]["threads"],
+            threads=config["resources"]["krakenuniq"]["threads"],
             estimate_precision=config["params"]["classifier"]["krakenuniq"]["estimate_precision"]
         benchmark:
             os.path.join(config["benchmarks"]["classifier"],
                         "rmhost_krakenuniq/{sample}_kraken2uniq_classifier_benchmark.tsv")
         log:
             os.path.join(config["logs"]["classifier"],
                         "rmhost_krakenuniq/{sample}_krakenuniq_classifier.log")
         resources:
-            mem_mb=config["params"]["classifier"]["krakenuniq"]["mem_mb"]
+            mem_mb=config["resources"]["krakenuniq"]["mem_mb"]
         conda:
             config["envs"]["krakenuniq"]
         # message:
         #     "Classifier: Performing Taxonomic Classifcation of Sample {sample} with krakenuniq."
         shell:
             '''
             krakenuniq --db {params.database} \
@@ -528,18 +526,18 @@
             microbe_dict_file = config["params"]["classifier"]["pathseq"]["microbe_dict"],
             host_hss_file = config["params"]["classifier"]["pathseq"]["host_bfi"],
             taxonomy_db = config["params"]["classifier"]["pathseq"]["taxonomy_db"],
             pathseq_output_dir = os.path.join(
                 config["output"]["classifier"],
                 "pathseq_classified_output/{sample}/")
         resources:
-            mem_mb=config["params"]["classifier"]["pathseq"]["mem_mb"]
+            mem_mb=config["resources"]["pathseq"]["mem_mb"]
         priority: 12
         threads: 
-            config["params"]["classifier"]["pathseq"]["threads"]
+            config["resources"]["pathseq"]["threads"]
         conda:
             config["envs"]["pathseq"]
         benchmark:
             os.path.join(config["benchmarks"]["classifier"],
                         "rmhost_pathseq/{sample}_pathseq_classifier_benchmark.log")
         log:
             os.path.join(config["logs"]["classifier"],
@@ -604,14 +602,16 @@
                 "pathseq_classified_output/{sample}/{sample}_pathseq_classified.bam"),
         output:
             pathseq_classified_unpaired_bam_file = temp(os.path.join(
                 config["output"]["classifier"],
                 "pathseq_classified_output/{sample}/{sample}_pathseq_unpaired_classified.bam"))
         params:
             threads=8
+        resources:
+            mem_mb=config["resources"]["samtools_extract"]["mem_mb"]
         conda:
             config["envs"]["star"]
         shell:
             '''
             samtools view --threads {params.threads} -h -b -F 1 -o {output.pathseq_classified_unpaired_bam_file} {input.pathseq_classified_bam_file}
             '''
```

### Comparing `microcat-0.2.2/microcat/rules/database.smk` & `microcat-0.2.3/microcat/rules/database.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/rules/host.smk` & `microcat-0.2.3/microcat/rules/host.smk`

 * *Files 2% similar despite different names*

```diff
@@ -121,14 +121,16 @@
                     os.path.join(config["logs"]["host"],
                                 "starsolo/{sample}_starsolo_count.log")
                 benchmark:
                     os.path.join(config["benchmarks"]["host"],
                                 "starsolo/{sample}_starsolo_count.benchmark")
                 conda:
                     config["envs"]["star"]
+                resources:
+                    mem_mb=config["resources"]["starsolo"]["mem_mb"]
                 shell:
                     '''
                     mkdir -p {params.starsolo_out}; 
                     cd {params.starsolo_out} ;
 
                     bash {params.starsolo_10X_auto} \
                     --barcode_reads {params.barcode_reads} \
@@ -190,17 +192,17 @@
                     outFilterScoreMin = config["params"]["host"]["starsolo"]["algorithm"]["outFilterScoreMin"],
                     soloMultiMappers = config["params"]["host"]["starsolo"]["algorithm"]["soloMultiMappers"],
                     barcode_list =  os.path.join(config["datas"]["barcode_list_dirs"]["tenX"],
                                                 config["params"]["host"]["starsolo"]["barcode"]["soloCBwhitelist"]),
                     outSAMattributes = config["params"]["host"]["starsolo"]["outSAMattributes"],
                     outSAMtype = config["params"]["host"]["starsolo"]["outSAMtype"],
                     variousParams = config["params"]["host"]["starsolo"]["variousParams"],
-                    threads = config["params"]["host"]["starsolo"]["threads"],
+                    threads =config["resources"]["starsolo"]["threads"],
                 resources:
-                    mem_mb=100000  # This rule needs 100 GB of memory
+                    mem_mb=config["resources"]["starsolo"]["mem_mb"]
                 log:
                     os.path.join(config["logs"]["host"],
                                 "starsolo/{sample}_starsolo_count.log")
                 benchmark:
                     os.path.join(config["benchmarks"]["host"],
                                 "starsolo/{sample}_starsolo_count.benchmark")
                 conda:
@@ -246,21 +248,23 @@
                     config["output"]["host"],
                     "starsolo_count/{sample}/Aligned_sortedByCoord_out.bam")
             output:
                 unmapped_bam_sorted_file = os.path.join(
                     config["output"]["host"],
                     "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam")
             params:
-                threads=16,
+                threads=config["resources"]["samtools_extract"]["threads"],
                 unmapped_bam_unsorted_file = os.path.join(
                     config["output"]["host"],
                     "unmapped_host/{sample}/Aligned_sortedByCoord_unmapped_out.bam")
             ## because bam is sorted by Coord,it's necessary to sort it by read name
             conda:
                 config["envs"]["star"]
+            resources:
+                mem_mb=config["resources"]["samtools_extract"]["mem_mb"],
             shell:
                 '''
                 samtools view --threads  {params.threads}  -b -f 4   {input.mapped_bam_file}  >  {params.unmapped_bam_unsorted_file};\
                 samtools sort -n  --threads  {params.threads} {params.unmapped_bam_unsorted_file} -o {output.unmapped_bam_sorted_file}
                 '''
         rule starsolo_CB_UMI_Simple_all:
             input:
@@ -314,23 +318,25 @@
                 soloCellFilter = config["params"]["host"]["starsolo"]["algorithm"]["soloCellFilter"],
                 soloStrand = config["params"]["host"]["starsolo"]["soloStrand"],
                 # SAMattrRGline = microcat.get_SAMattrRGline_from_manifest(config["params"]["host"]["starsolo"]["manifest"]),
                 SAMattrRGline = lambda wildcards: microcat.get_SAMattrRGline_by_sample(SAMPLES, wildcards),
                 # Additional parameters for STAR
                 variousParams = config["params"]["host"]["starsolo"]["variousParams"],
                 # Number of threads for STAR
-                threads = config["params"]["host"]["starsolo"]["threads"]
+                threads =config["resources"]["starsolo"]["threads"]
             log:
                 os.path.join(config["logs"]["host"],
                             "starsolo/{sample}/starsolo_count_smartseq2.log")
             benchmark:
                 os.path.join(config["benchmarks"]["host"],
                             "starsolo/{sample}/starsolo_count_smartseq2.benchmark")
             conda:
                 config["envs"]["star"]
+            resources:
+                mem_mb=config["resources"]["starsolo"]["mem_mb"]
             shell:
                 '''
                 if echo {params.cdna_reads} | grep -q "\.gz" ; then
                     file_command='--readFilesCommand zcat'
                 else
                     file_command=''
                 fi
@@ -362,17 +368,19 @@
                     config["output"]["host"],
                     "starsolo_count/{sample}/Aligned_out.bam")
             output:
                 unmapped_bam_unsorted_file = os.path.join(
                     config["output"]["host"],
                     "unmapped_host/{sample}/Aligned_out_unmapped.bam")
             params:
-                threads=16
+                threads=config["resources"]["samtools_extract"]["threads"],
             conda:
                 config["envs"]["star"]
+            resources:
+                mem_mb=config["resources"]["samtools_extract"]["mem_mb"],
             shell:
                 '''
                 samtools view --threads  {params.threads}  -b -f 4   {input.mapped_bam_file}  >  {output.unmapped_bam_unsorted_file}
                 '''
 
         # rule starsolo_SmartSeq_unmapped_sorted_bam:
         #     input:
@@ -404,22 +412,24 @@
                     config["output"]["host"],
                     "unmapped_host/{sample}/Aligned_out_unmapped.bam")
             output:
                 unmapped_sorted_bam = os.path.join(
                     config["output"]["host"],
                     "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam"),
             params:
-                threads=40,
+                threads=config["resources"]["samtools_extract"]["threads"],
                 tag="RG"
             log:
                 os.path.join(config["logs"]["host"],
                             "starsolo/{sample}/unmapped_sorted_bam.log")
             benchmark:
                 os.path.join(config["benchmarks"]["host"],
                             "starsolo/{sample}/unmapped_sorted_bam.benchmark")
+            resources:
+                mem_mb=config["resources"]["samtools_extract"]["mem_mb"],
             conda:
                 config["envs"]["star"]
             shell:
                 '''
                 samtools sort -n  --threads  {params.threads} {input.unmapped_bam_unsorted_file} -o {output.unmapped_sorted_bam}
                 '''
         # checkpoint starsolo_smartseq_demultiplex_bam_by_read_group:
@@ -523,15 +533,15 @@
                     barcode_list =  os.path.join(config["datas"]["barcode_list_dirs"]["tenX"],
                                                 config["params"]["host"]["starsolo"]["barcode"]["soloCBwhitelist"]),
                     outSAMattributes = config["params"]["host"]["starsolo"]["outSAMattributes"],
                     outSAMtype = config["params"]["host"]["starsolo"]["outSAMtype"],
                     variousParams = config["params"]["host"]["starsolo"]["variousParams"],
                     threads = config["params"]["host"]["starsolo"]["threads"],
                 resources:
-                    mem_mb=100000  # This rule needs 100 GB of memory
+                    mem_mb=config["resources"]["starsolo"]["mem_mb"]
                 log:
                     os.path.join(config["logs"]["host"],
                                 "starsolo/{sample}_starsolo_count.log")
                 benchmark:
                     os.path.join(config["benchmarks"]["host"],
                                 "starsolo/{sample}_starsolo_count.benchmark")
                 conda:
@@ -624,18 +634,17 @@
                 "cellranger_count/{sample}/{sample}.web_summary.html"),
             SampleID="{sample}",
             variousParams = config["params"]["host"]["cellranger"]["variousParams"],
         # resources:
         #     mem_mb=config["tools"]["cellranger_count"]["mem_mb"],
         #     runtime=config["tools"]["cellranger_count"]["runtime"],
         threads: 
-            config["params"]["host"]["cellranger"]["threads"]
+            config["resources"]["cellranger"]["threads"]
         resources:
-            mem_mb=102400,
-            disk_mb=10000
+            mem_mb=config["resources"]["cellranger"]["mem_mb"]
         conda:
             config["envs"]["star"]
         log:
             os.path.join(config["logs"]["host"],
                         "cellranger/{sample}_cellranger_count.log")
         benchmark:
             os.path.join(config["benchmarks"]["host"],
@@ -675,19 +684,21 @@
             config["output"]["host"],
             "cellranger_count/{sample}/{sample}_mappped2human_bam.bam")
         output:
             unmapped_bam_sorted_file = os.path.join(
                     config["output"]["host"],
                     "unmapped_host/{sample}/Aligned_sortedByName_unmapped_out.bam")
         params:
-            threads=16,
+            threads=config["resources"]["samtools_extract"]["threads"],
             unmapped_bam_unsorted_file = os.path.join(
                 config["output"]["host"],
                 "unmapped_host/{sample}/Aligned_sortedByCoord_unmapped_out.bam")
         ## because bam is sorted by Coord,it's necessary to sort it by read name
+        resources:
+            mem_mb=config["resources"]["samtools_extract"]["mem_mb"]
         conda:
             config["envs"]["star"]
         shell:
             '''
             samtools view --threads  {params.threads}  -b -f 4   {input.mapped_bam_file}  >  {params.unmapped_bam_unsorted_file};\
             samtools sort -n  --threads  {params.threads} {params.unmapped_bam_unsorted_file} -o {output.unmapped_bam_sorted_file}
             '''
```

### Comparing `microcat-0.2.2/microcat/sample.py` & `microcat-0.2.3/microcat/sample.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/scripts/INVADEseq.py` & `microcat-0.2.3/microcat/scripts/INVADEseq.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/scripts/add_tags_to_PathSeq_bam.py` & `microcat-0.2.3/microcat/scripts/add_tags_to_PathSeq_bam.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/scripts/create_hdf5.py` & `microcat-0.2.3/microcat/scripts/create_hdf5.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/scripts/extract_kraken_reads.py` & `microcat-0.2.3/microcat/scripts/extract_kraken_reads.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/scripts/extract_microbiome_output.R` & `microcat-0.2.3/microcat/scripts/extract_microbiome_output.R`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-library(optparse)
 library(tidyverse)
+library(optparse)
 library(dplyr)
 library(stringr)
 library(foreach)
 library(doParallel)
 
 option_list = list(
   make_option(c("--output_file"), action="store", help = "path to kraken output file"),
@@ -16,15 +16,14 @@
 )
 
 ## ntaxid: There is a certain limit on the length of command line in Linux system. The maximum length of the command line is determined by the system kernel parameter `ARG_MAX`, 
 ## which is usually several thousand or tens of thousands of characters. If you enter more characters than this limit on the command line, the system will not be able 
 ## to handle the command properly. Therefore, when searching for a large number of tax IDs, it is important to avoid exceeding the limit of command line length for 
 ## successful execution of the command.
 
-setwd("/home/microcat-sucx/project/scRNA-analysis/benchmark/Galeano2022")
 opt = parse_args(OptionParser(option_list = option_list))
 
 kr = read.delim(opt$kraken_report, header = F)
 # removing root and unclassified taxa
 kr = kr[-c(1:2), ]
 mpa = read.delim(opt$mpa_report, header = F)
```

### Comparing `microcat-0.2.2/microcat/scripts/generate_PE_manifest_file.py` & `microcat-0.2.3/microcat/scripts/generate_PE_manifest_file.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/scripts/get_ncbi_domains.py` & `microcat-0.2.3/microcat/scripts/get_ncbi_domains.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/scripts/kraken2mpa.py` & `microcat-0.2.3/microcat/scripts/kraken2mpa.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/scripts/kraken2sc.py` & `microcat-0.2.3/microcat/scripts/kraken2sc.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/scripts/microcat_bam_handle.Rmd` & `microcat-0.2.3/microcat/scripts/microcat_bam_handle.Rmd`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/scripts/sample_denosing.R` & `microcat-0.2.3/microcat/scripts/sample_denosing.R`

 * *Files 6% similar despite different names*

```diff
@@ -49,15 +49,14 @@
               help = "Minimum number of reads per taxon"),
   make_option(c("-u", "--min_uniq"), type = "integer", default = 2,
               help = "Minimum number of unique sequences per taxon")           
 )
 opt_parser <- OptionParser(option_list = option_list)
 opt <- parse_args(opt_parser)
 
-setwd("/home/microcat-sucx/project/scRNA-analysis/benchmark/Galeano2022")
 
 files <- list.files(opt$path,recursive = TRUE)
 stopifnot(length(files) > 0) # make sure the input dir path is set correctly
 min_reads <- opt$min_reads
 min_uniq <- opt$min_uniq
 
 kraken_report_sample <- read_kraken_reports(files = files,
```

### Comparing `microcat-0.2.2/microcat/scripts/sckmer_unpaired.R` & `microcat-0.2.3/microcat/scripts/sckmer_unpaired.R`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
   make_option(c("--kmer_len"), action="store", default = 35, help = "Kraken kmer length"),
   make_option(c("--nsample"), action="store", default = 1000, help = "Max number of barcodes to sample per taxa"),
   make_option(c("--kmer_test_file"), action="store", help = "kmer test output filename"),
   make_option(c("--kmer_file"), action="store", help = "output kmer filename")
 )
 
 opt = parse_args(OptionParser(option_list = option_list))
-setwd("/home/microcat-sucx/project/scRNA-analysis/benchmark/Galeano2022")
 # opt = list(fa1 = '/data/scRNA/EarlyGastricCancer-EGC/results/03.classifier/rmhost_extracted_classified_output/SRR9713114/SRR9713114_kraken2_extracted_classified.fq',
 #            microbiome_output_file = '/data/scRNA/EarlyGastricCancer-EGC/results/03.classifier/rmhost_extracted_classified_output/SRR9713114/SRR9713114_kraken2_extracted_classified_output.txt',
 #            cb_len = 16,
 #            umi_len = 10,
 #            kraken_report = '/data/scRNA/EarlyGastricCancer-EGC/results/03.classifier/rmhost_kraken2_report/custom/SRR9713114/SRR9713114_kraken2_report.txt',
 #            mpa_report = '/data/scRNA/EarlyGastricCancer-EGC/results/03.classifier/rmhost_kraken2_report/mpa/SRR9713114/SRR9713114_kraken2_mpa_report.txt',
 #            ranks = c('G', 'S'),
```

### Comparing `microcat-0.2.2/microcat/scripts/spilt_bam_by_tag.py` & `microcat-0.2.3/microcat/scripts/spilt_bam_by_tag.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/scripts/split_Starsolo_BAM_by_RG.py` & `microcat-0.2.3/microcat/scripts/split_Starsolo_BAM_by_RG.py`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/scripts/starsolo_tenX_auto.sh` & `microcat-0.2.3/microcat/scripts/starsolo_tenX_auto.sh`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,8 @@
 #!/bin/bash 
-
-
-# barcode_reads=$1
-# cdna_reads=$2
-# barcode_data_dir=$3
-# sample=$4
-# threads=$5
-# reference=$6
-# soloUMIdedup=$7
-# soloCBmatchWLtype=$8
-# soloUMIfiltering=$9
-# soloCellFilter={$10}
-# outFilterScoreMin={$11}
-# soloMultiMappers={$12}
-# clipAdapterType={$13}
 # default
 barcode_reads=""
 cdna_reads=""
 barcode_data_dir=""
 sample=""
 threads=""
 reference=""
@@ -388,15 +373,17 @@
 message="Finished work"
 
 printf "%s %s %s %-${alignment}s\n" "${green}${current_date}" "${current_time}" "${state}" "${blue}${message}${reset}"
 
 
 rm -rf {$sample}.test.R1.fastq
 rm -rf {$sample}.test.R2.fastq
-rm -rf {$sample}_test_strand
+rm -rf $report_dir
+
+sleep 15
 
 cd $sample/
 
 current_date=$(date +%Y-%m-%d)
 current_time=$(date +%H:%M:%S)
 state="[runtime] (run)"
 message="Proprecess output"
@@ -404,18 +391,19 @@
 printf "%s %s %s %-${alignment}s\n" "${green}${current_date}" "${current_time}" "${state}" "${blue}${message}${reset}"
 
 
 features_file="${sample}_features.tsv"
 matrix_file="${sample}_matrix.mtx"
 barcodes_file="${sample}_barcodes.tsv"
 mapped_bam_file="Aligned_sortedByCoord_out.bam"
-ln -sr "Solo.out/Gene/filtered/features.tsv" "$features_file" ;
-ln -sr "Solo.out/Gene/filtered/matrix.mtx" "$matrix_file" ; 
-ln -sr "Solo.out/Gene/filtered/barcodes.tsv" "$barcodes_file" ;\
+ln -sr "Solo.out/Gene/raw/features.tsv" "$features_file" ;
+ln -sr "Solo.out/Gene/raw/matrix.mtx" "$matrix_file" ; 
+ln -sr "Solo.out/Gene/raw/barcodes.tsv" "$barcodes_file" ;\
 mv "Aligned.sortedByCoord.out.bam" "$mapped_bam_file";\
 
+
 current_date=$(date +%Y-%m-%d)
 current_time=$(date +%H:%M:%S)
 state="[runtime] (ready)"
 message="Sucessfully proprecessed output"
 
 printf "%s %s %s %-${alignment}s\n" "${green}${current_date}" "${current_time}" "${state}" "${blue}${message}${reset}"
```

### Comparing `microcat-0.2.2/microcat/snakefiles/scRNA_wf.smk` & `microcat-0.2.3/microcat/snakefiles/scRNA_wf.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat/snakefiles/scRNA_wf_test.smk` & `microcat-0.2.3/microcat/snakefiles/scRNA_wf_test.smk`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/microcat.egg-info/PKG-INFO` & `microcat-0.2.3/microcat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microcat
-Version: 0.2.2
+Version: 0.2.3
 Summary: a computational toolbox to identificated microbiome from Omics
 Home-page: https://github.com/ChangxingSu/MicroCAT
 Author: Changxing Su
 Author-email: changxingsu42@gmail.com
 License: GPLv3+
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `microcat-0.2.2/microcat.egg-info/SOURCES.txt` & `microcat-0.2.3/microcat.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `microcat-0.2.2/setup.py` & `microcat-0.2.3/setup.py`

 * *Files identical despite different names*

