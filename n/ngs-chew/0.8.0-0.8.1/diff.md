# Comparing `tmp/ngs-chew-0.8.0.tar.gz` & `tmp/ngs-chew-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ngs-chew-0.8.0.tar", last modified: Mon Jan 16 19:49:58 2023, max compression
+gzip compressed data, was "ngs-chew-0.8.1.tar", last modified: Tue Jul 18 10:28:41 2023, max compression
```

## Comparing `ngs-chew-0.8.0.tar` & `ngs-chew-0.8.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 19:49:58.319854 ngs-chew-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3581 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-01-16 19:49:58.319854 ngs-chew-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 19:49:58.319854 ngs-chew-0.8.0/chew/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/chew/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-01-16 19:49:58.319854 ngs-chew-0.8.0/chew/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/chew/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/chew/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/chew/compare.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 19:49:58.315854 ngs-chew-0.8.0/chew/data/
--rw-r--r--   0 runner    (1001) docker     (123)   152073 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/chew/data/GRCh37_sites.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/chew/data/GRCh37_sitesX.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)   152277 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/chew/data/GRCh38_sites.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)     6666 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/chew/data/GRCh38_sitesX.bed.gz
--rw-r--r--   0 runner    (1001) docker     (123)    12174 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/chew/fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)      606 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/chew/plot_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/chew/plot_var_het.py
--rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/chew/roh.py
--rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/chew/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 19:49:58.315854 ngs-chew-0.8.0/ngs_chew.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-01-16 19:49:58.000000 ngs-chew-0.8.0/ngs_chew.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-01-16 19:49:58.000000 ngs-chew-0.8.0/ngs_chew.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 19:49:58.000000 ngs-chew-0.8.0/ngs_chew.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-16 19:49:58.000000 ngs-chew-0.8.0/ngs_chew.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-16 19:49:58.000000 ngs-chew-0.8.0/ngs_chew.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-16 19:49:58.000000 ngs-chew-0.8.0/ngs_chew.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-01-16 19:49:58.000000 ngs-chew-0.8.0/ngs_chew.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 19:49:58.315854 ngs-chew-0.8.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-01-16 19:49:58.319854 ngs-chew-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-16 19:49:58.319854 ngs-chew-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      817 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/tests/test_run_fingerprint.py
--rw-r--r--   0 runner    (1001) docker     (123)    68448 2023-01-16 19:49:56.000000 ngs-chew-0.8.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:28:41.224705 ngs-chew-0.8.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-18 10:28:41.224705 ngs-chew-0.8.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:28:41.224705 ngs-chew-0.8.1/chew/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/chew/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-18 10:28:41.224705 ngs-chew-0.8.1/chew/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5543 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/chew/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/chew/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/chew/compare.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:28:41.224705 ngs-chew-0.8.1/chew/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   152073 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/chew/data/GRCh37_sites.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/chew/data/GRCh37_sitesX.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)   152241 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/chew/data/GRCh38_sites.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     7607 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/chew/data/GRCh38_sitesX.bed.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    12052 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/chew/fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/chew/plot_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/chew/plot_var_het.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4032 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/chew/roh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4425 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/chew/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:28:41.224705 ngs-chew-0.8.1/ngs_chew.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-18 10:28:41.000000 ngs-chew-0.8.1/ngs_chew.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-07-18 10:28:41.000000 ngs-chew-0.8.1/ngs_chew.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:28:41.000000 ngs-chew-0.8.1/ngs_chew.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-07-18 10:28:41.000000 ngs-chew-0.8.1/ngs_chew.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 10:28:41.000000 ngs-chew-0.8.1/ngs_chew.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 10:28:41.000000 ngs-chew-0.8.1/ngs_chew.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-18 10:28:41.000000 ngs-chew-0.8.1/ngs_chew.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:28:41.224705 ngs-chew-0.8.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-18 10:28:41.224705 ngs-chew-0.8.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 10:28:41.224705 ngs-chew-0.8.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/tests/test_run_fingerprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68448 2023-07-18 10:28:37.000000 ngs-chew-0.8.1/versioneer.py
```

### Comparing `ngs-chew-0.8.0/CHANGELOG.md` & `ngs-chew-0.8.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+### [0.8.1](https://www.github.com/bihealth/ngs-chew/compare/v0.8.0...v0.8.1) (2023-07-18)
+
+
+### Bug Fixes
+
+* sites for GRCh38 ([#24](https://www.github.com/bihealth/ngs-chew/issues/24)) ([#39](https://www.github.com/bihealth/ngs-chew/issues/39)) ([79773ef](https://www.github.com/bihealth/ngs-chew/commit/79773ef0e829184e763aee61373ae46f6ea83ed5))
+
 ## [0.8.0](https://www.github.com/bihealth/ngs-chew/compare/v0.7.1...v0.8.0) (2023-01-16)
 
 
 ### Features
 
 * roh calling with "bcftools roh" ([#25](https://www.github.com/bihealth/ngs-chew/issues/25)) ([a4af62c](https://www.github.com/bihealth/ngs-chew/commit/a4af62ced20bee37b4342d58aca48aaf9d269e68))
```

### Comparing `ngs-chew-0.8.0/PKG-INFO` & `ngs-chew-0.8.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngs-chew
-Version: 0.8.0
+Version: 0.8.1
 Summary: NGS Chew
 Home-page: https://github.com/bihealth/ngs-chew
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bih-charite.de
 License: MIT license
 Keywords: bioinformatics
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -43,14 +43,21 @@
     --input-bam INPUT.bam \
     --genome-release GRCh37
 ```
 
 
 # Changelog
 
+### [0.8.1](https://www.github.com/bihealth/ngs-chew/compare/v0.8.0...v0.8.1) (2023-07-18)
+
+
+### Bug Fixes
+
+* sites for GRCh38 ([#24](https://www.github.com/bihealth/ngs-chew/issues/24)) ([#39](https://www.github.com/bihealth/ngs-chew/issues/39)) ([79773ef](https://www.github.com/bihealth/ngs-chew/commit/79773ef0e829184e763aee61373ae46f6ea83ed5))
+
 ## [0.8.0](https://www.github.com/bihealth/ngs-chew/compare/v0.7.1...v0.8.0) (2023-01-16)
 
 
 ### Features
 
 * roh calling with "bcftools roh" ([#25](https://www.github.com/bihealth/ngs-chew/issues/25)) ([a4af62c](https://www.github.com/bihealth/ngs-chew/commit/a4af62ced20bee37b4342d58aca48aaf9d269e68))
```

### Comparing `ngs-chew-0.8.0/README.md` & `ngs-chew-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `ngs-chew-0.8.0/chew/cli.py` & `ngs-chew-0.8.1/chew/cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 @click.pass_context
 def cli(ctx: click.Context, verbose: bool):
     """Main entry point for CLI via click."""
     ctx.ensure_object(dict)
     ctx.obj["verbose"] = verbose
 
 
-@cli.command("fingerprint", help="Compute fingerprint to numpy .npz files.")
+@cli.command("fingerprint", help="Compute fingerprint to numpy .npz files.")  # type: ignore[attr-defined]
 @click.option("--min-coverage", type=int, default=5, help="Minimal required coverage.")
 @click.option("--reference", required=True, help="Path to reference FASTA file.")
 @click.option(
     "--output-fingerprint",
     required=True,
     help="Path to output .npz file (extension will be added automatically if necessary)",
 )
@@ -83,15 +83,15 @@
         step_samtools_idxstats=step_samtools_idxstats,
         step_bcftools_roh=step_bcftools_roh,
         write_vcf=write_vcf,
     )
     fingerprint.run(config)
 
 
-@cli.command("compare", help="Perform fingeprint comparison.")
+@cli.command("compare", help="Perform fingeprint comparison.")  # type: ignore[attr-defined]
 @click.option(
     "--output-prefix", type=str, default="chew-comparison", help="Path to comparison file."
 )
 @click.option("--min-mask-ones", type=int, help="Minimal number of ones in mask.")
 @click.option("--max-mask-ones", type=int, help="Maximal number of ones in mask.")
 @click.argument("fingerprints", nargs=-1)
 @click.pass_context
@@ -108,15 +108,15 @@
         min_mask_ones=min_mask_ones,
         max_mask_ones=max_mask_ones,
         fingerprints=fingerprints,
     )
     compare.run(config)
 
 
-@cli.command("stats", help="Compute statistics from fingerprint .npz files.")
+@cli.command("stats", help="Compute statistics from fingerprint .npz files.")  # type: ignore[attr-defined]
 @click.option("--output", default="chew-stats.txt", help="Path to output file.")
 @click.argument("fingerprints", nargs=-1)
 @click.pass_context
 def cli_stats(
     ctx: click.Context,
     output: str,
     fingerprints: typing.List[str],
@@ -125,15 +125,15 @@
         verbosity=2 if ctx.obj["verbose"] else 1,
         output=output,
         fingerprints=fingerprints,
     )
     stats.run(config)
 
 
-@cli.command("plot-compare", help="Plot result of 'ngs-chew compare'.")
+@cli.command("plot-compare", help="Plot result of 'ngs-chew compare'.")  # type: ignore[attr-defined]
 @click.option(
     "--title", default="NGS Chew Comparison Plot", help="title to use for the output HTML file."
 )
 @click.argument("compare-out")
 @click.argument("out_html")
 @click.pass_context
 def cli_plot_compare(
@@ -147,15 +147,15 @@
         compare_out=compare_out,
         out_html=out_html,
         title=title,
     )
     plot_compare.run(config)
 
 
-@cli.command("plot-var-het", help="Plot var(het) metric from .npz files.")
+@cli.command("plot-var-het", help="Plot var(het) metric from .npz files.")  # type: ignore[attr-defined]
 @click.option(
     "--title", default="NGS Chew var(het) Plot", help="title to use for the output HTML file."
 )
 @click.argument("stats_out")
 @click.argument("out_html")
 @click.pass_context
 def cli_plot_var_het(
```

### Comparing `ngs-chew-0.8.0/chew/compare.py` & `ngs-chew-0.8.1/chew/compare.py`

 * *Files identical despite different names*

### Comparing `ngs-chew-0.8.0/chew/data/GRCh37_sites.bed.gz` & `ngs-chew-0.8.1/chew/data/GRCh37_sites.bed.gz`

 * *Files identical despite different names*

### Comparing `ngs-chew-0.8.0/chew/data/GRCh37_sitesX.bed.gz` & `ngs-chew-0.8.1/chew/data/GRCh37_sitesX.bed.gz`

 * *Files identical despite different names*

### Comparing `ngs-chew-0.8.0/chew/fingerprint.py` & `ngs-chew-0.8.1/chew/fingerprint.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,20 @@
 import numpy as np
 import numpy.typing
 import pysam
 import vcfpy
 
 import chew
 from chew import roh
-from chew.common import CHROM_LENS_GRCH37, CHROM_LENS_GRCH38, CHROM_LENS_HG19
+from chew.common import (
+    CHROM_LENS_GRCH37,
+    CHROM_LENS_GRCH38,
+    CHROM_LENS_HG19,
+    load_sites,
+)
 
 #: Key to use for GRCh37 release.
 RELEASE_37 = "GRCh37"
 
 #: Key to use for GRCh38 release.
 RELEASE_38 = "GRCh38"
 
@@ -151,20 +156,18 @@
     genome_release: str,
     sites_suffix: str,
     path_calls: str,
     prefix_fingerprint: typing.Optional[str],
 ):
     bed_file = f"{genome_release}_{sites_suffix}.bed.gz"
     logger.info("Reading sites BED (%s)...", bed_file)
-    path_gz = os.path.join(os.path.dirname(__file__), "data", bed_file)
-    with gzip.open(path_gz, "rt") as inputf:
-        sites = {}
-        for line in inputf:
-            arr = line.strip().split("\t")
-            sites["%s%s:%s" % (chr_prefix, arr[0], int(arr[1]) + 1)] = (0, 0, float("nan"))
+    sites = {
+        "%s%s:%s" % (chr_prefix, site.chrom, site.pos): (0, 0, float("nan"))
+        for site in load_sites(genome_release)
+    }
     logger.info("Converting VCF to fingerprint...")
     with vcfpy.Reader.from_path(path_calls) as vcf_reader:
         if prefix_fingerprint:
             logger.info("Writing VCF to %s", f"{prefix_fingerprint}.vcf.gz")
             out_vcf = vcfpy.Writer.from_path(
                 f"{prefix_fingerprint}.{sites_suffix}.vcf.gz", vcf_reader.header
             )
```

### Comparing `ngs-chew-0.8.0/chew/plot_compare.py` & `ngs-chew-0.8.1/chew/plot_compare.py`

 * *Files identical despite different names*

### Comparing `ngs-chew-0.8.0/chew/plot_var_het.py` & `ngs-chew-0.8.1/chew/plot_var_het.py`

 * *Files identical despite different names*

### Comparing `ngs-chew-0.8.0/chew/roh.py` & `ngs-chew-0.8.1/chew/roh.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-import gzip
 import os
 import shlex
 import subprocess
-import typing
 
 import attrs
 from logzero import logger
 import numpy.typing as npt
 import vcfpy
 
-from chew.common import CHROM_LENS_GRCH37, CHROM_LENS_GRCH38
+from chew.common import CHROM_LENS_GRCH37, CHROM_LENS_GRCH38, load_sites
 
 #: Use this value for genotype likelyhood (FORMAT/PL)
 BCFTOOLS_ROH_PL = 30
 
 #: Use this value for assumed allele frequency
 BCFTOOLS_ROH_AF = 0.05
 
@@ -39,35 +37,14 @@
 class Site:
     chrom: str
     pos: int
     ref: str
     alt: str
 
 
-def load_sites(genome_release: str) -> typing.List[Site]:
-    logger.info("Loading sites .bed.gz")
-    path_gz = os.path.join(os.path.dirname(__file__), "data", f"{genome_release}_sites.bed.gz")
-    result = []
-    with gzip.open(path_gz, "rt") as inputf:
-        for lineno, line in enumerate(inputf):
-            arr = line.split("\t")
-            # We construct sites with arbitrary REF/ALT as bcftools roh does not
-            # interpret them but only GT.
-            result.append(
-                Site(
-                    chrom=arr[0],
-                    pos=int(arr[1]) + 1,
-                    ref="N",
-                    alt="A",
-                )
-            )
-    logger.info("  finished reading %d sites", len(result))
-    return result
-
-
 def create_vcf_header(sample: str, release: str) -> vcfpy.Header:
     if release == "GRCh37":
         chrom_lens = CHROM_LENS_GRCH37
     elif release == "GRCh38":
         chrom_lens = CHROM_LENS_GRCH38
     else:
         raise RuntimeError(f"Invalid release {release}")
```

### Comparing `ngs-chew-0.8.0/chew/stats.py` & `ngs-chew-0.8.1/chew/stats.py`

 * *Files identical despite different names*

### Comparing `ngs-chew-0.8.0/ngs_chew.egg-info/PKG-INFO` & `ngs-chew-0.8.1/ngs_chew.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ngs-chew
-Version: 0.8.0
+Version: 0.8.1
 Summary: NGS Chew
 Home-page: https://github.com/bihealth/ngs-chew
 Author: Manuel Holtgrewe
 Author-email: manuel.holtgrewe@bih-charite.de
 License: MIT license
 Keywords: bioinformatics
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -43,14 +43,21 @@
     --input-bam INPUT.bam \
     --genome-release GRCh37
 ```
 
 
 # Changelog
 
+### [0.8.1](https://www.github.com/bihealth/ngs-chew/compare/v0.8.0...v0.8.1) (2023-07-18)
+
+
+### Bug Fixes
+
+* sites for GRCh38 ([#24](https://www.github.com/bihealth/ngs-chew/issues/24)) ([#39](https://www.github.com/bihealth/ngs-chew/issues/39)) ([79773ef](https://www.github.com/bihealth/ngs-chew/commit/79773ef0e829184e763aee61373ae46f6ea83ed5))
+
 ## [0.8.0](https://www.github.com/bihealth/ngs-chew/compare/v0.7.1...v0.8.0) (2023-01-16)
 
 
 ### Features
 
 * roh calling with "bcftools roh" ([#25](https://www.github.com/bihealth/ngs-chew/issues/25)) ([a4af62c](https://www.github.com/bihealth/ngs-chew/commit/a4af62ced20bee37b4342d58aca48aaf9d269e68))
```

### Comparing `ngs-chew-0.8.0/ngs_chew.egg-info/SOURCES.txt` & `ngs-chew-0.8.1/ngs_chew.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ngs-chew-0.8.0/setup.cfg` & `ngs-chew-0.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ngs-chew-0.8.0/setup.py` & `ngs-chew-0.8.1/setup.py`

 * *Files identical despite different names*

### Comparing `ngs-chew-0.8.0/tests/test_run_fingerprint.py` & `ngs-chew-0.8.1/tests/test_run_fingerprint.py`

 * *Files identical despite different names*

### Comparing `ngs-chew-0.8.0/versioneer.py` & `ngs-chew-0.8.1/versioneer.py`

 * *Files identical despite different names*

