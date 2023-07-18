# Comparing `tmp/RNA-seq-0.0.0.tar.gz` & `tmp/RNA-seq-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RNA-seq-0.0.0.tar", last modified: Tue Jul 18 17:38:38 2023, max compression
+gzip compressed data, was "RNA-seq-0.0.1.tar", last modified: Tue Jul 18 17:23:10 2023, max compression
```

## Comparing `RNA-seq-0.0.0.tar` & `RNA-seq-0.0.1.tar`

### file list

```diff
@@ -1,10 +1,11 @@
-drwxrwxrwx   0        0        0        0 2023-07-18 17:38:38.212241 RNA-seq-0.0.0/
--rw-rw-rw-   0        0        0      432 2023-07-18 17:38:38.212241 RNA-seq-0.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-07-18 17:38:38.212241 RNA-seq-0.0.0/RNA_seq.egg-info/
--rw-rw-rw-   0        0        0      432 2023-07-18 17:38:37.000000 RNA-seq-0.0.0/RNA_seq.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      150 2023-07-18 17:38:38.000000 RNA-seq-0.0.0/RNA_seq.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 17:38:37.000000 RNA-seq-0.0.0/RNA_seq.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-07-18 17:38:38.000000 RNA-seq-0.0.0/RNA_seq.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       60 2023-07-16 17:03:05.000000 RNA-seq-0.0.0/package_runner.py
--rw-rw-rw-   0        0        0       42 2023-07-18 17:38:38.212241 RNA-seq-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      693 2023-07-18 17:37:57.000000 RNA-seq-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-18 17:23:10.892289 RNA-seq-0.0.1/
+-rw-rw-rw-   0        0        0      432 2023-07-18 17:23:10.891278 RNA-seq-0.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-07-18 17:23:10.888864 RNA-seq-0.0.1/RNA_seq.egg-info/
+-rw-rw-rw-   0        0        0      432 2023-07-18 17:23:10.000000 RNA-seq-0.0.1/RNA_seq.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      180 2023-07-18 17:23:10.000000 RNA-seq-0.0.1/RNA_seq.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 17:23:10.000000 RNA-seq-0.0.1/RNA_seq.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       20 2023-07-18 17:23:10.000000 RNA-seq-0.0.1/RNA_seq.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        1 2023-07-18 17:23:10.000000 RNA-seq-0.0.1/RNA_seq.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       60 2023-07-16 17:03:05.000000 RNA-seq-0.0.1/package_runner.py
+-rw-rw-rw-   0        0        0       42 2023-07-18 17:23:10.892289 RNA-seq-0.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      839 2023-07-18 17:21:51.000000 RNA-seq-0.0.1/setup.py
```

