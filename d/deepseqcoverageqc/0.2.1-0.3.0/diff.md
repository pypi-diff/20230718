# Comparing `tmp/deepseqcoverageqc-0.2.1.tar.gz` & `tmp/deepseqcoverageqc-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deepseqcoverageqc-0.2.1.tar", max compression
+gzip compressed data, was "deepseqcoverageqc-0.3.0.tar", max compression
```

## Comparing `deepseqcoverageqc-0.2.1.tar` & `deepseqcoverageqc-0.3.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      596 2023-06-30 06:17:16.322444 deepseqcoverageqc-0.2.1/LICENSE
--rw-r--r--   0        0        0     8345 2023-06-30 06:17:16.322444 deepseqcoverageqc-0.2.1/README.md
--rw-r--r--   0        0        0        0 2023-06-30 06:17:16.322444 deepseqcoverageqc-0.2.1/deepseqcoverageqc/__init__.py
--rw-r--r--   0        0        0    10274 2023-06-30 06:17:16.322444 deepseqcoverageqc-0.2.1/deepseqcoverageqc/coverageQC.py
--rw-r--r--   0        0        0     3661 2023-06-30 06:17:16.322444 deepseqcoverageqc-0.2.1/deepseqcoverageqc/panelIndexer.py
--rw-r--r--   0        0        0     2614 2023-06-30 06:17:16.326445 deepseqcoverageqc-0.2.1/deepseqcoverageqc/panelQC.py
--rw-r--r--   0        0        0      875 2023-06-30 06:17:16.326445 deepseqcoverageqc-0.2.1/pyproject.toml
--rw-r--r--   0        0        0     8973 1970-01-01 00:00:00.000000 deepseqcoverageqc-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0      596 2023-07-18 18:21:44.492392 deepseqcoverageqc-0.3.0/LICENSE
+-rw-r--r--   0        0        0     8402 2023-07-18 18:21:44.492392 deepseqcoverageqc-0.3.0/README.md
+-rw-r--r--   0        0        0       22 2023-07-18 18:21:44.496392 deepseqcoverageqc-0.3.0/deepseqcoverageqc/__init__.py
+-rw-r--r--   0        0        0    10274 2023-07-18 18:21:44.496392 deepseqcoverageqc-0.3.0/deepseqcoverageqc/coverageQC.py
+-rw-r--r--   0        0        0     3661 2023-07-18 18:21:44.496392 deepseqcoverageqc-0.3.0/deepseqcoverageqc/panelIndexer.py
+-rw-r--r--   0        0        0     2614 2023-07-18 18:21:44.496392 deepseqcoverageqc-0.3.0/deepseqcoverageqc/panelQC.py
+-rw-r--r--   0        0        0     1296 2023-07-18 18:21:44.496392 deepseqcoverageqc-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     9030 1970-01-01 00:00:00.000000 deepseqcoverageqc-0.3.0/PKG-INFO
```

### Comparing `deepseqcoverageqc-0.2.1/LICENSE` & `deepseqcoverageqc-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deepseqcoverageqc-0.2.1/README.md` & `deepseqcoverageqc-0.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
 ---
 ## Quick Start
 
 ### Using [Docker](https://www.docker.com/)
 
 ```bash
-docker run -it pskolekar/deepseqcoverageqc --help
+docker run -it pskolekar/deepseqcoverageqc:0.3.0 --help
 ```
 
 ### Using [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
 
 ```bash
 conda create --name DeepSeqCoverageQC python==3.9
 conda activate DeepSeqCoverageQC
@@ -148,12 +148,13 @@
 
 ## Publication
 
 Manuscript under preparation
 
 ## Contact
 
-- [Pandurang Kolekar](mailto:pandurang.kolekar@gmail.com)
+- [Dr. Pandurang Kolekar](mailto:pandurang.kolekar@gmail.com)
+- [Dr. Xiaotu Ma](mailto:Xiaotu.Ma@stjude.org)
 
 ## COPYRIGHT
 
 Copyright © 2023 Pandurang Kolekar, St. Jude Children's Research Hospital
```

#### html2text {}

```diff
@@ -5,16 +5,16 @@
 
                              Explore_the_docs_Â»
 
 
                          Request_Feature | Report_Bug
                      â­ Consider starring the repo! â­
 --- ## Quick Start ### Using [Docker](https://www.docker.com/) ```bash docker
-run -it pskolekar/deepseqcoverageqc --help ``` ### Using [Miniconda](https://
-docs.conda.io/en/latest/miniconda.html) ```bash conda create --name
+run -it pskolekar/deepseqcoverageqc:0.3.0 --help ``` ### Using [Miniconda]
+(https://docs.conda.io/en/latest/miniconda.html) ```bash conda create --name
 DeepSeqCoverageQC python==3.9 conda activate DeepSeqCoverageQC python -m pip
 install deepseqcoverageqc DeepSeqCoverageQC --help ``` ### Using Pip > **Note**
 > Requires [Python](https://www.python.org/) version >=3.9 ```bash pip install
 deepseqcoverageqc ``` ## Usage Please refer to the _detailed documentation_
 [here](https://pandurang-kolekar.github.io/DeepSeqCoverageQC/
 ) `DeepSeqCoverageQC` is a command line interface (CLI) app with the following
 commands ```bash $ DeepSeqCoverageQC --help Usage: DeepSeqCoverageQC [OPTIONS]
@@ -49,10 +49,11 @@
 generated by buildIndex â â command. â â [required] â â * --
 countFile PATH Count file(s) generated by SequencErr â â program. File(s)
 should've seven â â columns: Chr, Pos, A_Q_30, C_Q_30, â â G_Q_30,
 T_Q_30, N_Q_30 â â [required] â â --outdir PATH Output directory path.
 â â --outSummary/--no-outSummary Output counts at summary positions â â
 --help Show this message and exit. â
 â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
-``` ## Publication Manuscript under preparation ## Contact - [Pandurang
-Kolekar](mailto:pandurang.kolekar@gmail.com) ## COPYRIGHT Copyright Â© 2023
-Pandurang Kolekar, St. Jude Children's Research Hospital
+``` ## Publication Manuscript under preparation ## Contact - [Dr. Pandurang
+Kolekar](mailto:pandurang.kolekar@gmail.com) - [Dr. Xiaotu Ma](mailto:
+Xiaotu.Ma@stjude.org) ## COPYRIGHT Copyright Â© 2023 Pandurang Kolekar, St.
+Jude Children's Research Hospital
```

### Comparing `deepseqcoverageqc-0.2.1/deepseqcoverageqc/coverageQC.py` & `deepseqcoverageqc-0.3.0/deepseqcoverageqc/coverageQC.py`

 * *Files identical despite different names*

### Comparing `deepseqcoverageqc-0.2.1/deepseqcoverageqc/panelIndexer.py` & `deepseqcoverageqc-0.3.0/deepseqcoverageqc/panelIndexer.py`

 * *Files identical despite different names*

### Comparing `deepseqcoverageqc-0.2.1/deepseqcoverageqc/panelQC.py` & `deepseqcoverageqc-0.3.0/deepseqcoverageqc/panelQC.py`

 * *Files identical despite different names*

### Comparing `deepseqcoverageqc-0.2.1/PKG-INFO` & `deepseqcoverageqc-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deepseqcoverageqc
-Version: 0.2.1
+Version: 0.3.0
 Summary: Compute coverage QC metrics for deep targeted sequencing data
 Author: Pandurang Kolekar
 Author-email: pandurang.kolekar@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -64,15 +64,15 @@
 
 ---
 ## Quick Start
 
 ### Using [Docker](https://www.docker.com/)
 
 ```bash
-docker run -it pskolekar/deepseqcoverageqc --help
+docker run -it pskolekar/deepseqcoverageqc:0.3.0 --help
 ```
 
 ### Using [Miniconda](https://docs.conda.io/en/latest/miniconda.html)
 
 ```bash
 conda create --name DeepSeqCoverageQC python==3.9
 conda activate DeepSeqCoverageQC
@@ -165,13 +165,14 @@
 
 ## Publication
 
 Manuscript under preparation
 
 ## Contact
 
-- [Pandurang Kolekar](mailto:pandurang.kolekar@gmail.com)
+- [Dr. Pandurang Kolekar](mailto:pandurang.kolekar@gmail.com)
+- [Dr. Xiaotu Ma](mailto:Xiaotu.Ma@stjude.org)
 
 ## COPYRIGHT
 
 Copyright © 2023 Pandurang Kolekar, St. Jude Children's Research Hospital
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: deepseqcoverageqc Version: 0.2.1 Summary: Compute
+Metadata-Version: 2.1 Name: deepseqcoverageqc Version: 0.3.0 Summary: Compute
 coverage QC metrics for deep targeted sequencing data Author: Pandurang Kolekar
 Author-email: pandurang.kolekar@gmail.com Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: click
 (>=8.1.3,<9.0.0) Requires-Dist: pandas (>=2.0.1,<3.0.0) Requires-Dist: rich-
 click (>=1.6.1,<2.0.0) Requires-Dist: tqdm (>=4.65.0,<5.0.0) Description-
@@ -14,16 +14,16 @@
 
                              Explore_the_docs_Â»
 
 
                          Request_Feature | Report_Bug
                      â­ Consider starring the repo! â­
 --- ## Quick Start ### Using [Docker](https://www.docker.com/) ```bash docker
-run -it pskolekar/deepseqcoverageqc --help ``` ### Using [Miniconda](https://
-docs.conda.io/en/latest/miniconda.html) ```bash conda create --name
+run -it pskolekar/deepseqcoverageqc:0.3.0 --help ``` ### Using [Miniconda]
+(https://docs.conda.io/en/latest/miniconda.html) ```bash conda create --name
 DeepSeqCoverageQC python==3.9 conda activate DeepSeqCoverageQC python -m pip
 install deepseqcoverageqc DeepSeqCoverageQC --help ``` ### Using Pip > **Note**
 > Requires [Python](https://www.python.org/) version >=3.9 ```bash pip install
 deepseqcoverageqc ``` ## Usage Please refer to the _detailed documentation_
 [here](https://pandurang-kolekar.github.io/DeepSeqCoverageQC/
 ) `DeepSeqCoverageQC` is a command line interface (CLI) app with the following
 commands ```bash $ DeepSeqCoverageQC --help Usage: DeepSeqCoverageQC [OPTIONS]
@@ -58,10 +58,11 @@
 generated by buildIndex â â command. â â [required] â â * --
 countFile PATH Count file(s) generated by SequencErr â â program. File(s)
 should've seven â â columns: Chr, Pos, A_Q_30, C_Q_30, â â G_Q_30,
 T_Q_30, N_Q_30 â â [required] â â --outdir PATH Output directory path.
 â â --outSummary/--no-outSummary Output counts at summary positions â â
 --help Show this message and exit. â
 â°ââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââââ¯
-``` ## Publication Manuscript under preparation ## Contact - [Pandurang
-Kolekar](mailto:pandurang.kolekar@gmail.com) ## COPYRIGHT Copyright Â© 2023
-Pandurang Kolekar, St. Jude Children's Research Hospital
+``` ## Publication Manuscript under preparation ## Contact - [Dr. Pandurang
+Kolekar](mailto:pandurang.kolekar@gmail.com) - [Dr. Xiaotu Ma](mailto:
+Xiaotu.Ma@stjude.org) ## COPYRIGHT Copyright Â© 2023 Pandurang Kolekar, St.
+Jude Children's Research Hospital
```
