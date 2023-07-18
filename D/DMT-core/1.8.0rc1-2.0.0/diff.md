# Comparing `tmp/DMT_core-1.8.0rc1.tar.gz` & `tmp/DMT_core-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DMT_core-1.8.0rc1.tar", last modified: Fri Nov 11 13:33:32 2022, max compression
+gzip compressed data, was "DMT_core-2.0.0.tar", last modified: Tue Jul 18 12:49:35 2023, max compression
```

## Comparing `DMT_core-1.8.0rc1.tar` & `DMT_core-2.0.0.tar`

### file list

```diff
@@ -1,421 +1,78 @@
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.923809 DMT_core-1.8.0rc1/
--rw-rw-r--   0 mario     (1000) mario     (1000)     5072 2022-08-03 12:19:02.000000 DMT_core-1.8.0rc1/.gitignore
--rw-rw-r--   0 mario     (1000) mario     (1000)     5033 2022-11-10 10:13:28.000000 DMT_core-1.8.0rc1/.gitlab-ci.yml
--rw-rw-r--   0 mario     (1000) mario     (1000)     6339 2022-11-10 10:14:12.000000 DMT_core-1.8.0rc1/CHANGELOG
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.831808 DMT_core-1.8.0rc1/DMT/
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.835809 DMT_core-1.8.0rc1/DMT/Hdev/
--rw-rw-r--   0 mario     (1000) mario     (1000)      954 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/Hdev/__init__.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    37670 2022-08-03 20:23:08.000000 DMT_core-1.8.0rc1/DMT/Hdev/dut_hdev.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.835809 DMT_core-1.8.0rc1/DMT/config/
--rw-rw-r--   0 mario     (1000) mario     (1000)     2859 2022-08-03 20:06:56.000000 DMT_core-1.8.0rc1/DMT/config/DMT_config.yaml
--rw-rw-r--   0 mario     (1000) mario     (1000)     6996 2022-08-03 20:06:56.000000 DMT_core-1.8.0rc1/DMT/config/__init__.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.839809 DMT_core-1.8.0rc1/DMT/core/
--rw-rw-r--   0 mario     (1000) mario     (1000)     4451 2022-11-10 10:13:28.000000 DMT_core-1.8.0rc1/DMT/core/__init__.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     9005 2022-08-17 17:57:57.000000 DMT_core-1.8.0rc1/DMT/core/circuit.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     3205 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/core/constants.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    88265 2022-08-04 10:47:59.000000 DMT_core-1.8.0rc1/DMT/core/data_frame.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    34649 2022-11-10 10:13:28.000000 DMT_core-1.8.0rc1/DMT/core/data_processor.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    27465 2022-08-03 12:19:02.000000 DMT_core-1.8.0rc1/DMT/core/data_reader.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     7597 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/core/database_manager.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    10000 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/core/df_to_sweep.py
--rw-rw-r--   0 mario     (1000) mario     (1000)      107 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/DMT/core/dmt_units.txt
--rw-rw-r--   0 mario     (1000) mario     (1000)    42174 2022-08-03 20:06:56.000000 DMT_core-1.8.0rc1/DMT/core/docu_dut_lib.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     7708 2022-08-03 12:19:02.000000 DMT_core-1.8.0rc1/DMT/core/dut_circuit.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     4676 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/core/dut_dummy.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    66690 2022-08-17 17:57:51.000000 DMT_core-1.8.0rc1/DMT/core/dut_lib.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    13116 2022-08-03 12:19:02.000000 DMT_core-1.8.0rc1/DMT/core/dut_meas.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     5791 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/core/dut_tcad.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     9887 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/core/dut_type.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    33993 2022-08-03 20:06:56.000000 DMT_core-1.8.0rc1/DMT/core/dut_view.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     2452 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/core/hasher.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    49221 2022-08-17 17:57:51.000000 DMT_core-1.8.0rc1/DMT/core/mc_parameter.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     7171 2022-08-17 17:57:51.000000 DMT_core-1.8.0rc1/DMT/core/mc_skywater.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    36109 2022-11-10 10:13:28.000000 DMT_core-1.8.0rc1/DMT/core/mcard.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    36630 2022-11-10 13:35:48.000000 DMT_core-1.8.0rc1/DMT/core/naming.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    80705 2022-11-10 10:13:28.000000 DMT_core-1.8.0rc1/DMT/core/plot.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    22294 2022-08-03 20:06:56.000000 DMT_core-1.8.0rc1/DMT/core/plot_2yaxis.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    11669 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/core/plot_smith.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    35276 2022-11-10 10:13:28.000000 DMT_core-1.8.0rc1/DMT/core/sim_con.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     2859 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/core/singleton.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    31680 2022-08-17 17:57:51.000000 DMT_core-1.8.0rc1/DMT/core/sweep.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    14191 2022-08-03 12:19:02.000000 DMT_core-1.8.0rc1/DMT/core/sweep_def.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     7319 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/core/technology.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     2319 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/core/utils.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    11630 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/core/va_file.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.839809 DMT_core-1.8.0rc1/DMT/exceptions/
--rw-rw-r--   0 mario     (1000) mario     (1000)     3007 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/exceptions/__init__.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.843809 DMT_core-1.8.0rc1/DMT/external/
--rw-rw-r--   0 mario     (1000) mario     (1000)      883 2022-11-11 13:19:18.000000 DMT_core-1.8.0rc1/DMT/external/__init__.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    10075 2022-11-10 10:13:28.000000 DMT_core-1.8.0rc1/DMT/external/latex.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     3201 2022-11-10 10:13:28.000000 DMT_core-1.8.0rc1/DMT/external/os.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     5532 2022-11-10 10:13:28.000000 DMT_core-1.8.0rc1/DMT/external/pylatex.py
--rwxrwxr-x   0 mario     (1000) mario     (1000)     4128 2022-11-10 10:13:28.000000 DMT_core-1.8.0rc1/DMT/external/pypi.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     5111 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/external/verilogae.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.843809 DMT_core-1.8.0rc1/DMT/libautodoc_template/
--rw-rw-r--   0 mario     (1000) mario     (1000)     2926 2022-08-03 20:06:56.000000 DMT_core-1.8.0rc1/DMT/libautodoc_template/.gitignore
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.843809 DMT_core-1.8.0rc1/DMT/libautodoc_template/base/
--rw-rw-r--   0 mario     (1000) mario     (1000)      848 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/DMT/libautodoc_template/base/acronyms.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)     4056 2022-08-03 20:06:56.000000 DMT_core-1.8.0rc1/DMT/libautodoc_template/base/header.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)        6 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/DMT/libautodoc_template/bib.bib
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.843809 DMT_core-1.8.0rc1/DMT/libautodoc_template/content/
--rw-rw-r--   0 mario     (1000) mario     (1000)      789 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/DMT/libautodoc_template/content/conclusion.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)     1262 2022-08-03 20:06:56.000000 DMT_core-1.8.0rc1/DMT/libautodoc_template/content/deckblatt.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)     1317 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/DMT/libautodoc_template/content/introduction.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)      341 2022-08-03 20:00:33.000000 DMT_core-1.8.0rc1/DMT/libautodoc_template/documentation-blx.bib
--rw-rw-r--   0 mario     (1000) mario     (1000)     1236 2022-08-03 12:19:02.000000 DMT_core-1.8.0rc1/DMT/libautodoc_template/documentation.tex
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.843809 DMT_core-1.8.0rc1/DMT/libautodoc_template/figures/
--rw-rw-r--   0 mario     (1000) mario     (1000)        0 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/DMT/libautodoc_template/figures/.gitkeep
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.843809 DMT_core-1.8.0rc1/DMT/ngspice/
--rw-rw-r--   0 mario     (1000) mario     (1000)      891 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/ngspice/__init__.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    38091 2022-08-17 17:57:51.000000 DMT_core-1.8.0rc1/DMT/ngspice/dut_ngspice.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.843809 DMT_core-1.8.0rc1/DMT/xyce/
--rw-rw-r--   0 mario     (1000) mario     (1000)      980 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/DMT/xyce/__init__.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    36135 2022-08-03 12:19:02.000000 DMT_core-1.8.0rc1/DMT/xyce/dut_xyce.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.843809 DMT_core-1.8.0rc1/DMT_core.egg-info/
--rwxrwxrwx   0 mario     (1000) mario     (1000)     5824 2022-11-11 13:33:32.000000 DMT_core-1.8.0rc1/DMT_core.egg-info/PKG-INFO
--rwxrwxrwx   0 mario     (1000) mario     (1000)    16916 2022-11-11 13:33:32.000000 DMT_core-1.8.0rc1/DMT_core.egg-info/SOURCES.txt
--rwxrwxrwx   0 mario     (1000) mario     (1000)        1 2022-11-11 13:33:32.000000 DMT_core-1.8.0rc1/DMT_core.egg-info/dependency_links.txt
--rwxrwxrwx   0 mario     (1000) mario     (1000)      453 2022-11-11 13:33:32.000000 DMT_core-1.8.0rc1/DMT_core.egg-info/requires.txt
--rwxrwxrwx   0 mario     (1000) mario     (1000)        4 2022-11-11 13:33:32.000000 DMT_core-1.8.0rc1/DMT_core.egg-info/top_level.txt
--rw-rw-r--   0 mario     (1000) mario     (1000)    35330 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/LICENSE
--rw-rw-r--   0 mario     (1000) mario     (1000)     5824 2022-11-11 13:33:32.923809 DMT_core-1.8.0rc1/PKG-INFO
--rw-rw-r--   0 mario     (1000) mario     (1000)     4646 2022-08-03 12:19:02.000000 DMT_core-1.8.0rc1/README.md
--rw-rw-r--   0 mario     (1000) mario     (1000)     1411 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/codemeta.json
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.843809 DMT_core-1.8.0rc1/doc/
--rw-rw-r--   0 mario     (1000) mario     (1000)      604 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/Makefile
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.843809 DMT_core-1.8.0rc1/doc/logo/
--rw-rw-r--   0 mario     (1000) mario     (1000)    23279 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/logo/DMT_Logo_wText.png
--rw-rw-r--   0 mario     (1000) mario     (1000)      811 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/make.bat
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.847808 DMT_core-1.8.0rc1/doc/public_release_paper/
--rw-rw-r--   0 mario     (1000) mario     (1000)     2020 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/public_release_paper/DMT-interface.drawio
--rw-rw-r--   0 mario     (1000) mario     (1000)    30731 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/public_release_paper/DMT-interface.pdf
--rw-rw-r--   0 mario     (1000) mario     (1000)    45874 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/public_release_paper/F_TJ_C.pdf
--rw-rw-r--   0 mario     (1000) mario     (1000)     7420 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/public_release_paper/F_TJ_C.tex
--rwxrwxrwx   0 mario     (1000) mario     (1000)      147 2022-02-10 14:01:46.000000 DMT_core-1.8.0rc1/doc/public_release_paper/build_paper.sh
--rw-rw-r--   0 mario     (1000) mario     (1000)    10975 2022-06-24 19:21:54.000000 DMT_core-1.8.0rc1/doc/public_release_paper/paper.bib
--rw-rw-r--   0 mario     (1000) mario     (1000)     8954 2022-06-13 15:44:21.000000 DMT_core-1.8.0rc1/doc/public_release_paper/paper.md
--rw-rw-r--   0 mario     (1000) mario     (1000)   215699 2022-06-24 19:21:54.000000 DMT_core-1.8.0rc1/doc/public_release_paper/paper.pdf
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.847808 DMT_core-1.8.0rc1/doc/source/
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.847808 DMT_core-1.8.0rc1/doc/source/_static/
--rw-rw-r--   0 mario     (1000) mario     (1000)    25156 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/HBT_vbc.elpa
--rw-rw-r--   0 mario     (1000) mario     (1000)    62097 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/I_CV_BE.pdf
--rw-rw-r--   0 mario     (1000) mario     (1000)   105166 2022-04-25 21:52:09.000000 DMT_core-1.8.0rc1/doc/source/_static/I_CV_BE.pdf.png
--rw-rw-r--   0 mario     (1000) mario     (1000)     8598 2022-05-10 12:30:21.000000 DMT_core-1.8.0rc1/doc/source/_static/I_CV_BE.tex
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.851809 DMT_core-1.8.0rc1/doc/source/_static/intro/
--rw-rw-r--   0 mario     (1000) mario     (1000)    52646 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/intro/F_TI_C.pdf
--rw-rw-r--   0 mario     (1000) mario     (1000)   106149 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/intro/F_TI_C.png
--rw-rw-r--   0 mario     (1000) mario     (1000)     2453 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/intro/F_TI_C.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    51514 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/intro/I_CV_BE.pdf
--rw-rw-r--   0 mario     (1000) mario     (1000)    93317 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/intro/I_CV_BE.png
--rw-rw-r--   0 mario     (1000) mario     (1000)     2280 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/intro/I_CV_BE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    61709 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/intro/Y_21I_C.pdf
--rw-rw-r--   0 mario     (1000) mario     (1000)   107014 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/intro/Y_21I_C.png
--rw-rw-r--   0 mario     (1000) mario     (1000)     2479 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/intro/Y_21I_C.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)      751 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/intro/bjt.lib
--rw-rw-r--   0 mario     (1000) mario     (1000)    24424 2022-08-03 20:06:56.000000 DMT_core-1.8.0rc1/doc/source/_static/intro/meas_data_300K.csv
--rw-rw-r--   0 mario     (1000) mario     (1000)    22747 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/intro/sgp_v1p0.va
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.851809 DMT_core-1.8.0rc1/doc/source/_static/running_a_simulation/
--rw-rw-r--   0 mario     (1000) mario     (1000)     1940 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/running_a_simulation/DMT-interface.drawio
--rw-rw-r--   0 mario     (1000) mario     (1000)    22456 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/running_a_simulation/DMT-interface.png
--rw-rw-r--   0 mario     (1000) mario     (1000)    56168 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/running_a_simulation/F_TJ_C.pdf
--rw-rw-r--   0 mario     (1000) mario     (1000)    91098 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/running_a_simulation/F_TJ_C.png
--rw-rw-r--   0 mario     (1000) mario     (1000)     6005 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_static/running_a_simulation/F_TJ_C.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    54279 2022-05-02 09:27:17.000000 DMT_core-1.8.0rc1/doc/source/_static/running_a_simulation/J_CV_BE.pdf
--rw-rw-r--   0 mario     (1000) mario     (1000)    83073 2022-05-02 09:27:17.000000 DMT_core-1.8.0rc1/doc/source/_static/running_a_simulation/J_CV_BE.png
--rw-rw-r--   0 mario     (1000) mario     (1000)     4921 2022-05-02 09:27:17.000000 DMT_core-1.8.0rc1/doc/source/_static/running_a_simulation/J_CV_BE.tex
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.831808 DMT_core-1.8.0rc1/doc/source/_theme/
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.851809 DMT_core-1.8.0rc1/doc/source/_theme/scipy/
--rw-rw-r--   0 mario     (1000) mario     (1000)     8643 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/layout.html
--rw-rw-r--   0 mario     (1000) mario     (1000)      425 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/searchbox.html
--rw-rw-r--   0 mario     (1000) mario     (1000)      224 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/sourcelink.html
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.851809 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.851809 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/css/
--rw-rw-r--   0 mario     (1000) mario     (1000)     1975 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/css/extend.css
--rw-rw-r--   0 mario     (1000) mario     (1000)     3916 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/css/pygments.css
--rw-rw-r--   0 mario     (1000) mario     (1000)    16285 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/css/scipy-central.css
--rw-rw-r--   0 mario     (1000) mario     (1000)   178781 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/css/spc-bootstrap.css
--rw-rw-r--   0 mario     (1000) mario     (1000)     1865 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/css/spc-extend.css
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.855809 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/img/
--rw-rw-r--   0 mario     (1000) mario     (1000)     8777 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/img/glyphicons-halflings-white.png
--rw-rw-r--   0 mario     (1000) mario     (1000)    12799 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/img/glyphicons-halflings.png
--rw-rw-r--   0 mario     (1000) mario     (1000)     2933 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/img/scipy_org_logo.gif
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.855809 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/js/
--rw-rw-r--   0 mario     (1000) mario     (1000)     2950 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/js/copybutton.js
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.855809 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.859809 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/
--rw-rw-r--   0 mario     (1000) mario     (1000)      636 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/accordion.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     1369 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/alerts.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     1489 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/bootstrap.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      431 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/breadcrumbs.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     5709 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/button-groups.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     4766 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/buttons.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     2482 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/carousel.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      644 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/close.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     1282 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/code.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      306 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/component-animations.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     5493 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/dropdowns.less
--rw-rw-r--   0 mario     (1000) mario     (1000)    15866 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/forms.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      429 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/grid.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      521 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/hero-unit.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     1884 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/labels-badges.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      329 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/layouts.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      860 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/media.less
--rw-rw-r--   0 mario     (1000) mario     (1000)    23042 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/mixins.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     1978 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/modals.less
--rw-rw-r--   0 mario     (1000) mario     (1000)    12002 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/navbar.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     8163 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/navs.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      760 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/pager.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     2678 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/pagination.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     3077 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/popovers.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     2858 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/progress-bars.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     4201 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/reset.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      565 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/responsive-1200px-min.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     3920 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/responsive-767px-max.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      463 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/responsive-768px-979px.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     4328 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/responsive-navbar.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     1602 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/responsive-utilities.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     1069 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/responsive.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      885 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/scaffolding.less
--rw-rw-r--   0 mario     (1000) mario     (1000)    10841 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/sprites.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     6255 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/tables.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     1192 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/thumbnails.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     1684 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/tooltip.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     4857 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/type.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      335 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/utilities.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     9142 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/variables.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      552 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/bootstrap/wells.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      451 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/spc-bootstrap.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      832 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/spc-content.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      365 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/spc-extend.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      154 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/spc-footer.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      441 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/spc-header.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      259 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/spc-rightsidebar.less
--rw-rw-r--   0 mario     (1000) mario     (1000)      425 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/less/spc-utils.less
--rw-rw-r--   0 mario     (1000) mario     (1000)     5134 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/static/scipy.css_t
--rw-rw-r--   0 mario     (1000) mario     (1000)      173 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/_theme/scipy/theme.conf
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.859809 DMT_core-1.8.0rc1/doc/source/automatic_testing/
--rw-rw-r--   0 mario     (1000) mario     (1000)     4355 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/automatic_testing/automated_test.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      421 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/automatic_testing/index.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)     1745 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/automatic_testing/updating_docker.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)     1819 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/automatic_testing/windows_installer.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)     9945 2022-08-03 12:19:07.000000 DMT_core-1.8.0rc1/doc/source/conf.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.863808 DMT_core-1.8.0rc1/doc/source/core/
--rw-rw-r--   0 mario     (1000) mario     (1000)      127 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/circuit.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      124 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/constants.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      145 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/data_frame.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      257 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/data_processor.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      139 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/data_reader.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      144 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/database_manager.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      155 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/df_to_sweep.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      144 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/docu_dut_lib.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      143 2022-08-03 12:19:07.000000 DMT_core-1.8.0rc1/doc/source/core/dut_lib.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      905 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/dut_view.rst
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.863808 DMT_core-1.8.0rc1/doc/source/core/duts_circuit/
--rw-rw-r--   0 mario     (1000) mario     (1000)      325 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/duts_circuit/dut_circuit.rst
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.863808 DMT_core-1.8.0rc1/doc/source/core/duts_circuit/interfaces/
--rw-rw-r--   0 mario     (1000) mario     (1000)      160 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/duts_circuit/interfaces/dut_ngspice.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      148 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/duts_circuit/interfaces/dut_xyce.rst
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.863808 DMT_core-1.8.0rc1/doc/source/core/duts_meas/
--rw-rw-r--   0 mario     (1000) mario     (1000)      133 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/duts_meas/dut_meas.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      123 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/duts_meas/dut_type.rst
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.863808 DMT_core-1.8.0rc1/doc/source/core/duts_tcad/
--rw-rw-r--   0 mario     (1000) mario     (1000)      520 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/duts_tcad/dut_tcad.rst
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.863808 DMT_core-1.8.0rc1/doc/source/core/duts_tcad/interfaces/
--rw-rw-r--   0 mario     (1000) mario     (1000)      149 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/duts_tcad/interfaces/dut_hdev.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      116 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/hasher.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      178 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/mc_parameter.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      351 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/mcard.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      598 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/naming.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      132 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/plot.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      655 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/sim_con.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      129 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/singleton.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      135 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/sweep.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      136 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/technology.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      127 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/utils.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      135 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/core/va_file.rst
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.863808 DMT_core-1.8.0rc1/doc/source/diagrams/
--rw-rw-r--   0 mario     (1000) mario     (1000)     3684 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/diagrams/classes_dut.dot
--rw-rw-r--   0 mario     (1000) mario     (1000)     1998 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/diagrams/classes_sim_con.dot
--rw-rw-r--   0 mario     (1000) mario     (1000)     2748 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/diagrams/many_simulations.drawio
--rw-rw-r--   0 mario     (1000) mario     (1000)    57207 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/diagrams/many_simulations.png
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.867809 DMT_core-1.8.0rc1/doc/source/examples/
--rw-rw-r--   0 mario     (1000) mario     (1000)     2178 2022-05-10 12:30:21.000000 DMT_core-1.8.0rc1/doc/source/examples/basic_data_handling.py
--rw-rw-r--   0 mario     (1000) mario     (1000)      315 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/examples/basic_data_handling.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      527 2022-08-03 12:19:07.000000 DMT_core-1.8.0rc1/doc/source/examples/index.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)     6284 2022-06-01 19:52:52.000000 DMT_core-1.8.0rc1/doc/source/examples/introduction.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     2030 2022-04-26 08:17:54.000000 DMT_core-1.8.0rc1/doc/source/examples/read_in_measurement_data.py
--rw-rw-r--   0 mario     (1000) mario     (1000)      241 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/examples/read_in_measurement_data.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)     5674 2022-08-03 12:19:02.000000 DMT_core-1.8.0rc1/doc/source/examples/running_a_simulation.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     2387 2022-08-03 12:19:07.000000 DMT_core-1.8.0rc1/doc/source/examples/running_a_simulation.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)     1766 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/examples/test_cases.rst
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.867809 DMT_core-1.8.0rc1/doc/source/external/
--rw-rw-r--   0 mario     (1000) mario     (1000)      401 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/external/latex.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      190 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/external/os.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      376 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/external/pylatex.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      399 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/external/verilogae.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)     4120 2022-08-03 12:19:07.000000 DMT_core-1.8.0rc1/doc/source/index.rst
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.867809 DMT_core-1.8.0rc1/doc/source/installation/
--rw-rw-r--   0 mario     (1000) mario     (1000)    10612 2022-11-10 10:13:28.000000 DMT_core-1.8.0rc1/doc/source/installation/install_dmt.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      711 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/installation/known_mac_issues.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)     1869 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/installation/remote.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)    17401 2022-08-03 20:06:56.000000 DMT_core-1.8.0rc1/doc/source/introduction.rst
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.867809 DMT_core-1.8.0rc1/doc/source/technical_documentation/
--rw-rw-r--   0 mario     (1000) mario     (1000)      371 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/technical_documentation/dmt.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      291 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/technical_documentation/exceptions.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      195 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/technical_documentation/external.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)     1397 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/technical_documentation/hdev.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)      244 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/technical_documentation/index.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)     1097 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/technical_documentation/ngspice.rst
--rw-rw-r--   0 mario     (1000) mario     (1000)     3674 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/doc/source/technical_documentation/xyce.rst
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.867809 DMT_core-1.8.0rc1/logs/
--rw-rw-r--   0 mario     (1000) mario     (1000)        0 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/logs/.gitkeep
--rw-rw-r--   0 mario     (1000) mario     (1000)       99 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/pyproject.toml
--rw-rw-r--   0 mario     (1000) mario     (1000)       38 2022-11-11 13:33:32.923809 DMT_core-1.8.0rc1/setup.cfg
--rw-rw-r--   0 mario     (1000) mario     (1000)     2161 2022-11-11 13:33:18.000000 DMT_core-1.8.0rc1/setup.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.831808 DMT_core-1.8.0rc1/test/
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.871809 DMT_core-1.8.0rc1/test/test_core_no_interfaces/
--rw-rw-r--   0 mario     (1000) mario     (1000)    85841 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/HBT_vbc.elpa
--rw-rw-r--   0 mario     (1000) mario     (1000)   114401 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/HBT_vce.elpa
--rw-rw-r--   0 mario     (1000) mario     (1000)     6007 2022-08-03 12:19:02.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_MCard.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     3784 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_circuit.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     4302 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_create_potential.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.875809 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.831808 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.895809 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/
--rwxrwxrwx   0 mario     (1000) mario     (1000)  2930509 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/Spar_vb.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)  3039043 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/Spar_vc.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)     5828 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/fgummel_vbc_0.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)     4491 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/fgummel_vbc_0p1.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)     4491 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/fgummel_vbc_0p2.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)     4492 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/fgummel_vbc_0p25.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)     4491 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/fgummel_vbc_0p3.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)     4491 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/fgummel_vbc_0p5.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)     4490 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/fgummel_vbc_m0p1.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)     4490 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/fgummel_vbc_m0p2.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)     4491 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/fgummel_vbc_m0p25.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)     4490 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/fgummel_vbc_m0p3.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)     4490 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/fgummel_vbc_m0p5.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)    12334 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/fgummel_vce.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)    59500 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/foutput_ib.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)    43849 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/foutput_vb.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)   537657 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/freq_vbc_0.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)   537660 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/freq_vbc_0p1.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)   761291 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/freq_vbc_0p25.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)   537660 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/freq_vbc_0p3.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)   537660 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/freq_vbc_0p4.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)   537660 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/freq_vbc_0p5.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)   537659 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/freq_vbc_m0p1.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)   537659 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/freq_vbc_m0p2.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)   537659 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/freq_vbc_m0p3.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)   537659 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/freq_vbc_m0p4.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)   537659 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/freq_vbc_m0p5.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)   470563 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/freq_vce_0.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)    11456 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/rev_gummel.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)    11723 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/0p25x10x1_full/298/sub_dio.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)   314029 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/Spar_vb.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)     8255 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/dummy_open_cold.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)     8249 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/dummy_open_freq.mdm
--rwxrwxrwx   0 mario     (1000) mario     (1000)     8249 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/dummy_short_freq.mdm
--rw-rw-r--   0 mario     (1000) mario     (1000)   128904 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/idc1
--rw-rw-r--   0 mario     (1000) mario     (1000)     8071 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/short_dc.mdm
--rw-rw-r--   0 mario     (1000) mario     (1000)    27716 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data/short_freq.mdm
--rw-rw-r--   0 mario     (1000) mario     (1000)    11320 2022-06-22 15:57:40.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_data_processor.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     4756 2022-05-10 12:30:21.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_database_manager.py
--rw-rw-r--   0 mario     (1000) mario     (1000)      618 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_dataframe.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     6716 2022-04-25 19:05:43.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_df_to_sweep.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     3989 2022-05-10 12:30:21.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_dut_lib.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     1265 2022-05-10 12:30:21.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_dut_type.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     4676 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_get_nodes.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     1929 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_hasher.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     6988 2022-11-10 10:13:28.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_manager_processor_and_plotter.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    14217 2022-05-10 12:30:21.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_mc_parameter_composition.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.895809 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_modelcards/
--rw-rw-r--   0 mario     (1000) mario     (1000)     6355 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_modelcards/IHP_ECE704_03_para_D21.mat
--rwxrwxrwx   0 mario     (1000) mario     (1000)     6117 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_modelcards/ITRS_N5.mat
--rw-rw-r--   0 mario     (1000) mario     (1000)    43499 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_modelcards/N3_MCard_v1.json
--rw-rw-r--   0 mario     (1000) mario     (1000)     2235 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_modelcards/internal_transistor_example_mcard.lib
--rw-rw-r--   0 mario     (1000) mario     (1000)     2235 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_modelcards/npn_1D.lib
--rw-rw-r--   0 mario     (1000) mario     (1000)     2355 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_modelcards/npn_full.lib
--rw-rw-r--   0 mario     (1000) mario     (1000)     1145 2022-05-10 12:30:21.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_plot.py
--rw-rw-r--   0 mario     (1000) mario     (1000)      674 2022-04-25 19:05:43.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_read_elpa.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     3696 2022-08-17 17:57:51.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_read_mdm.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     1675 2022-08-03 12:19:02.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_sim_con.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     3976 2022-04-25 19:05:33.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_simple_data_clean.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     1008 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_singleton.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     5415 2022-08-03 12:19:02.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_specifiers.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    10437 2022-08-03 12:19:02.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_sweep.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     2272 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_utilities.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.831808 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_va_code/
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.899809 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_va_code/diode_cmc_160823/
--rw-rw-r--   0 mario     (1000) mario     (1000)    17781 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_va_code/diode_cmc_160823/DIODE_CMC_InitModel.include
--rw-rw-r--   0 mario     (1000) mario     (1000)     6063 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_va_code/diode_cmc_160823/DIODE_CMC_SIMKIT_macrodefs.include
--rw-rw-r--   0 mario     (1000) mario     (1000)    29257 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_va_code/diode_cmc_160823/DIODE_CMC_macrodefs.include
--rw-rw-r--   0 mario     (1000) mario     (1000)    17354 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_va_code/diode_cmc_160823/DIODE_CMC_parlist.include
--rw-rw-r--   0 mario     (1000) mario     (1000)     5475 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_va_code/diode_cmc_160823/DIODE_CMC_varlist1.include
--rw-rw-r--   0 mario     (1000) mario     (1000)     5203 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_va_code/diode_cmc_160823/DIODE_CMC_varlist2.include
--rw-rw-r--   0 mario     (1000) mario     (1000)     6223 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_va_code/diode_cmc_160823/Updates.txt
--rw-rw-r--   0 mario     (1000) mario     (1000)    26591 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_va_code/diode_cmc_160823/diode_cmc.va
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.899809 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_va_code/hicuml2/
--rwxrwxrwx   0 mario     (1000) mario     (1000)    86851 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_va_code/hicuml2/hicumL2V2p4p0_release.va
--rw-rw-r--   0 mario     (1000) mario     (1000)     3727 2022-04-25 19:05:33.000000 DMT_core-1.8.0rc1/test/test_core_no_interfaces/test_va_files.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.899809 DMT_core-1.8.0rc1/test/test_interface_hdev/
--rw-rw-r--   0 mario     (1000) mario     (1000)     2545 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_hdev/test_dut_hdev.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.911809 DMT_core-1.8.0rc1/test/test_interface_ngspice/
--rw-rw-r--   0 mario     (1000) mario     (1000)     1007 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/check_nqs_transient.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    10014 2022-05-10 12:30:21.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/compare_ADS.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    12212 2022-05-10 12:30:21.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/compare_ADS_many_sweeps.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    12592 2022-05-10 12:30:21.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/compare_ADS_real_modelcard.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    15097 2022-05-10 12:30:21.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/compare_ads_nqs.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    21070 2022-05-10 12:30:21.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/compare_ads_systematic.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     3631 2022-05-10 12:30:21.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/convergence2.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     4022 2022-05-10 12:30:21.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/convergence_sh.py
--rw-rw-r--   0 mario     (1000) mario     (1000)     1876 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/dietmar_full_sh.lib
--rw-rw-r--   0 mario     (1000) mario     (1000)     2126 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/dietmar_output.lib
--rw-rw-r--   0 mario     (1000) mario     (1000)     1876 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/dietmar_output_convergence.lib
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.915809 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/
--rw-rw-r--   0 mario     (1000) mario     (1000)   424903 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/comparison_ngspice_ads.pdf
--rw-rw-r--   0 mario     (1000) mario     (1000)     1270 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/comparison_ngspice_ads.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)   270113 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/comparison_ngspice_ads_nqs.pdf
--rw-rw-r--   0 mario     (1000) mario     (1000)     2086 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/comparison_ngspice_ads_nqs.tex
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.919809 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/
--rw-rw-r--   0 mario     (1000) mario     (1000)    37198 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/CBCVBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    36977 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/CBEVBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    36924 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/CCEVBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    30225 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/FTVBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    36520 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/ITVBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    46446 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/IV_mathrmBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    36935 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/ImY11VBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    36896 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/ImY12VBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    36913 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/ImY21VBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)   128902 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/ImY21f.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    37027 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/ImY22VBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)   128686 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/MagY21f.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)   111418 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/PhaseY21f.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    37068 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/ReY11VBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    38324 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/ReY12VBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    35627 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/ReY21VBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)   129232 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/ReY21f.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    36949 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/ReY22VBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    32606 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/VBICIVBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    32423 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/VBIEIVBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    22480 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/dTVBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)    30993 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/documentation/figs/rbiVBE.tex
--rw-rw-r--   0 mario     (1000) mario     (1000)     2903 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/hic2_tran.sp
--rw-rw-r--   0 mario     (1000) mario     (1000)     1704 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/hicum_test_modelcard.lib
--rw-rw-r--   0 mario     (1000) mario     (1000)     9622 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/model-card-examples.lib
--rw-rw-r--   0 mario     (1000) mario     (1000)     2701 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/ngspice_example_modelcard.lib
--rwxrwxrwx   0 mario     (1000) mario     (1000)     2349 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/npn_full_sh.lib
--rw-rw-r--   0 mario     (1000) mario     (1000)  7703465 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/output_tran
--rwxrwxrwx   0 mario     (1000) mario     (1000)    25777 2022-02-10 12:44:46.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/real_mcard.mcard
--rw-rw-r--   0 mario     (1000) mario     (1000)    10946 2022-08-03 12:19:02.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/test_dut_ngspice.py
--rw-rw-r--   0 mario     (1000) mario     (1000)   867244 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_ngspice/transient_data_ads.csv
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.919809 DMT_core-1.8.0rc1/test/test_interface_xyce/
--rw-rw-r--   0 mario     (1000) mario     (1000)      751 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_xyce/bjt.lib
--rw-rw-r--   0 mario     (1000) mario     (1000)     5695 2022-05-10 12:30:21.000000 DMT_core-1.8.0rc1/test/test_interface_xyce/compare_spectre_buildIns_vs_VA.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    86722 2022-06-28 21:50:50.000000 DMT_core-1.8.0rc1/test/test_interface_xyce/hicuml2v2p4p0_xyce.va
--rw-rw-r--   0 mario     (1000) mario     (1000)    22747 2022-04-24 21:05:59.000000 DMT_core-1.8.0rc1/test/test_interface_xyce/sgp_v1p0.va
--rw-rw-r--   0 mario     (1000) mario     (1000)    14546 2022-05-10 12:30:55.000000 DMT_core-1.8.0rc1/test/test_interface_xyce/test_xyce_HICUM_buildIn_vs_VA.py
--rw-rw-r--   0 mario     (1000) mario     (1000)    12885 2022-05-10 12:30:55.000000 DMT_core-1.8.0rc1/test/test_interface_xyce/test_xyce_SGP_buildIn_vs_VA.py
-drwxrwxr-x   0 mario     (1000) mario     (1000)        0 2022-11-11 13:33:32.923809 DMT_core-1.8.0rc1/test/test_verilogae/
--rwxrwxrwx   0 mario     (1000) mario     (1000)    86359 2022-02-23 15:33:21.000000 DMT_core-1.8.0rc1/test/test_verilogae/hicumL2V2p4p0.va
--rw-rw-r--   0 mario     (1000) mario     (1000)     2171 2022-08-03 12:19:02.000000 DMT_core-1.8.0rc1/test/test_verilogae/test_get_param_list.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.381547 DMT_core-2.0.0/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.369547 DMT_core-2.0.0/DMT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.370547 DMT_core-2.0.0/DMT/Hdev/
+-rw-rw-rw-   0 root         (0) root         (0)      954 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/Hdev/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    42089 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/Hdev/dut_hdev.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.371547 DMT_core-2.0.0/DMT/config/
+-rw-rw-rw-   0 root         (0) root         (0)     2932 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/config/DMT_config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)     6905 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/config/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.377547 DMT_core-2.0.0/DMT/core/
+-rw-rw-rw-   0 root         (0) root         (0)     4425 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8634 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/circuit.py
+-rw-rw-rw-   0 root         (0) root         (0)     3205 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)    90055 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/data_frame.py
+-rw-rw-rw-   0 root         (0) root         (0)    34879 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/data_processor.py
+-rw-rw-rw-   0 root         (0) root         (0)    27057 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/data_reader.py
+-rw-rw-rw-   0 root         (0) root         (0)     8779 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/database_manager.py
+-rw-rw-rw-   0 root         (0) root         (0)     9998 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/df_to_sweep.py
+-rw-rw-rw-   0 root         (0) root         (0)      159 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dmt_units.txt
+-rw-rw-rw-   0 root         (0) root         (0)    42237 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/docu_dut_lib.py
+-rw-rw-rw-   0 root         (0) root         (0)    10578 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dut_circuit.py
+-rw-rw-rw-   0 root         (0) root         (0)     4676 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dut_dummy.py
+-rw-rw-rw-   0 root         (0) root         (0)    71359 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dut_lib.py
+-rw-rw-rw-   0 root         (0) root         (0)    12163 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dut_meas.py
+-rw-rw-rw-   0 root         (0) root         (0)     8116 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dut_tcad.py
+-rw-rw-rw-   0 root         (0) root         (0)    13057 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dut_type.py
+-rw-rw-rw-   0 root         (0) root         (0)    41817 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/dut_view.py
+-rw-rw-rw-   0 root         (0) root         (0)     2452 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/hasher.py
+-rw-rw-rw-   0 root         (0) root         (0)    50056 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/mc_parameter.py
+-rw-rw-rw-   0 root         (0) root         (0)     7171 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/mc_skywater.py
+-rw-rw-rw-   0 root         (0) root         (0)    28046 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/mcard.py
+-rw-rw-rw-   0 root         (0) root         (0)    38026 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/naming.py
+-rw-rw-rw-   0 root         (0) root         (0)    82840 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/plot.py
+-rw-rw-rw-   0 root         (0) root         (0)    22847 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/plot_2yaxis.py
+-rw-rw-rw-   0 root         (0) root         (0)    11669 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/plot_smith.py
+-rw-rw-rw-   0 root         (0) root         (0)    36689 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/sim_con.py
+-rw-rw-rw-   0 root         (0) root         (0)     2859 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/singleton.py
+-rw-rw-rw-   0 root         (0) root         (0)    31475 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/sweep.py
+-rw-rw-rw-   0 root         (0) root         (0)    18223 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/sweep_def.py
+-rw-rw-rw-   0 root         (0) root         (0)     8298 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/technology.py
+-rw-rw-rw-   0 root         (0) root         (0)     2319 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    11995 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/core/va_file.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.377547 DMT_core-2.0.0/DMT/exceptions/
+-rw-rw-rw-   0 root         (0) root         (0)     3007 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/exceptions/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.378547 DMT_core-2.0.0/DMT/external/
+-rw-rw-rw-   0 root         (0) root         (0)      883 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/external/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10703 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/external/latex.py
+-rw-rw-rw-   0 root         (0) root         (0)     3201 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/external/os.py
+-rw-rw-rw-   0 root         (0) root         (0)     5532 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/external/pylatex.py
+-rwxrwxrwx   0 root         (0) root         (0)     5331 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/external/pypi.py
+-rw-rw-rw-   0 root         (0) root         (0)     5111 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/external/verilogae.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.378547 DMT_core-2.0.0/DMT/libautodoc_template/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.378547 DMT_core-2.0.0/DMT/libautodoc_template/base/
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/libautodoc_template/base/acronyms.tex
+-rw-rw-rw-   0 root         (0) root         (0)     4056 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/libautodoc_template/base/header.tex
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/libautodoc_template/bib.bib
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.379546 DMT_core-2.0.0/DMT/libautodoc_template/content/
+-rw-rw-rw-   0 root         (0) root         (0)      789 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/libautodoc_template/content/conclusion.tex
+-rw-rw-rw-   0 root         (0) root         (0)     1262 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/libautodoc_template/content/deckblatt.tex
+-rw-rw-rw-   0 root         (0) root         (0)     1317 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/libautodoc_template/content/introduction.tex
+-rw-rw-rw-   0 root         (0) root         (0)     1236 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/libautodoc_template/documentation.tex
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.379546 DMT_core-2.0.0/DMT/ngspice/
+-rw-rw-rw-   0 root         (0) root         (0)      891 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/ngspice/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    46941 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/ngspice/dut_ngspice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.379546 DMT_core-2.0.0/DMT/xyce/
+-rw-rw-rw-   0 root         (0) root         (0)      980 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/xyce/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    38969 2023-07-18 12:49:29.000000 DMT_core-2.0.0/DMT/xyce/dut_xyce.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 12:49:35.380546 DMT_core-2.0.0/DMT_core.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5865 2023-07-18 12:49:35.000000 DMT_core-2.0.0/DMT_core.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1547 2023-07-18 12:49:35.000000 DMT_core-2.0.0/DMT_core.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 12:49:35.000000 DMT_core-2.0.0/DMT_core.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      478 2023-07-18 12:49:35.000000 DMT_core-2.0.0/DMT_core.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        4 2023-07-18 12:49:35.000000 DMT_core-2.0.0/DMT_core.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)    35333 2023-07-18 12:49:29.000000 DMT_core-2.0.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     5865 2023-07-18 12:49:35.380546 DMT_core-2.0.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     4646 2023-07-18 12:49:29.000000 DMT_core-2.0.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)       99 2023-07-18 12:49:29.000000 DMT_core-2.0.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 12:49:35.381547 DMT_core-2.0.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     2182 2023-07-18 12:49:34.000000 DMT_core-2.0.0/setup.py
```

### Comparing `DMT_core-1.8.0rc1/DMT/Hdev/__init__.py` & `DMT_core-2.0.0/DMT/Hdev/__init__.py`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/Hdev/dut_hdev.py` & `DMT_core-2.0.0/DMT/Hdev/dut_hdev.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,25 +28,32 @@
 import os
 import numpy as np
 import pandas as pd
 import logging
 import h5py
 from typing import cast
 import shutil
+from typing import List, Dict
+
+try:
+    from semver.version import Version as VersionInfo
+except ImportError:
+    from semver import VersionInfo
 
 from DMT.core import (
     DutTcad,
     DataFrame,
     specifiers,
     sub_specifiers,
     Sweep,
     read_data,
     get_specifier_from_string,
     constants,
     DutType,
+    Technology,
 )
 from DMT.config import DATA_CONFIG
 
 from DMT.exceptions import SimulationUnsuccessful
 from DMT.config import COMMANDS
 from hdevpy.tools import makeinp, turn_off_recombination
 
@@ -57,14 +64,16 @@
 
 # Hdev iv output columns not needed in current DMT framework
 hdev_iv_fallback = {
     "T_LATTICE": None,
     "T_CPU": None,
 }
 
+SEMVER_DUTHDEV_CURRENT = VersionInfo(major=1, minor=0)
+
 
 class DutHdev(DutTcad):
     r"""Manages simulations and simulation data with Hdev.
 
     Parameters
     ----------
     database_dir : str
@@ -88,29 +97,92 @@
     sim_name : str
         DEVICE simulation title. Sort of a DUT-Name.
 
     """
     inited = False
 
     def __init__(
-        self, database_dir, dut_type, inp_structure, name="hdev_", simulator_command=None, **kwargs
+        self,
+        database_dir,
+        dut_type,
+        inp_structure,
+        name="hdev_",
+        simulator_command=None,
+        inp_name="hdev_inp.din",
+        **kwargs
     ):
         if simulator_command is None:
             simulator_command = COMMANDS["Hdev"]
 
         super().__init__(
             database_dir,
             name,
             dut_type,
             inp_structure,
             simulator_command=simulator_command,
-            inp_name="hdev_inp.din",
+            inp_name=inp_name,
             **kwargs,
         )
 
+    def info_json(self, **_kwargs) -> Dict:
+        """Returns a dict with serializeable content for the json file to create.
+
+        The topmost dict MUST have only one key: The string casted class name.
+        Inside the parameters are:
+
+            * A version key,
+            * all extra parameters of DutHdev compared to DutTcad and
+            * the info_json of DutTcad.
+
+        Returns
+        -------
+        dict
+            str(DutHdev): serialized content
+        """
+
+        return {
+            str(DutHdev): {
+                "__DutHdev__": str(SEMVER_DUTHDEV_CURRENT),
+                "parent": super(DutHdev, self).info_json(**_kwargs),
+            }
+        }
+
+    @classmethod
+    def from_json(
+        cls,
+        json_content: Dict,
+        classes_technology: List[type[Technology]],
+        subclass_kwargs: Dict = None,
+    ) -> "DutHdev":
+        """Static class method. Loads a DutHdev object from a json or pickle file with full path save_dir.
+
+        Calls the from_json method of DutView with all dictionary inside the "parent" keyword. Afterwards the additional parameters are set correctly.
+
+        Parameters
+        ----------
+        json_content  :  dict
+            Readed dictionary from a saved json DutHdev.
+        classes_technology : List[type[Technology]]
+            All possible technologies this loaded DutHdev can have. One will be choosen according to the serialized technology loaded from the file.
+        subclass_kwargs : Dict, optional
+            Additional kwargs necessary to create the concrete subclassed DutView.
+
+        Returns
+        -------
+        DutHdev
+            Loaded object.
+        """
+        if json_content["__DutHdev__"] != SEMVER_DUTHDEV_CURRENT:
+            raise NotImplementedError("DMT.DutHdev: Unknown version of DutHdev to load!")
+
+        dut_view = super().from_json(
+            json_content["parent"], classes_technology, subclass_kwargs=subclass_kwargs
+        )
+        return dut_view
+
     def create_inp_header(self, inp_):
         """Creates the inp_header from the given parameters.
 
         All parameters are taken from obj_inp_device.
 
         Parameters
         ----------
@@ -229,14 +301,29 @@
                 # add sweep definition to inp file
                 bias_str = (
                     "&AC_INFO "
                     + "".join([name + "=" + str(value) + " " for name, value in ac_info.items()])
                     + "/"
                 )
                 inp_str = inp_str + "\n" + bias_str
+            elif sub_sweep.sweep_type == "LOG":
+                bias_fun = "'LOG'"
+                ac_info = {
+                    "port1": "'" + self.ac_ports[0] + "'",
+                    "port2": "'" + self.ac_ports[1] + "'",
+                    "sweep_type": bias_fun,
+                    "freq_val": " ".join(["{0:3.2e}".format(val) for val in sub_sweep.value_def]),
+                }
+                # add sweep definition to inp file
+                bias_str = (
+                    "&AC_INFO "
+                    + "".join([name + "=" + str(value) + " " for name, value in ac_info.items()])
+                    + "/"
+                )
+                inp_str = inp_str + "\n" + bias_str
             else:
                 raise NotImplementedError
 
         if not has_t_def:
             bias_str = (
                 "&BIAS_INFO "
                 + "".join([name + "=" + str(value) + " " for name, value in temp_bias_info.items()])
@@ -473,23 +560,27 @@
             except KeyError:
                 pass
 
             if (
                 ac and len(dfs_inqu) > 0
             ):  # only one frequency simulated => post process (maybe also check for 1D)
                 if not len(freqs) == 2:
-                    raise IOError
+                    # use lowest frequency neq 0
+                    # freq_i = np.min(freqs[freqs>0])
+                    # df_iv = df
+                    pass
+
                 # post processing
                 # 1 general stuff
                 x = dfs_inqu[0]["X"].to_numpy()
                 d = dfs_inqu[0][specifiers.NET_DOPING].to_numpy()
                 junctions = (
                     np.where(np.sign(d[:-1]) != np.sign(d[1:]))[0] + 1
                 )  # detect sign changes
-                if junctions != []:  # no junction found
+                if junctions.size > 0:  # no junction found
                     xje = x[junctions[0]]
                     xjc = x[junctions[1]]
 
                     # sum of charge
                     qp = np.zeros(len(df_iv))
                     qn = np.zeros(len(df_iv))
                     for i_row, _row in enumerate(df_iv.iterrows()):
@@ -513,59 +604,73 @@
                     tau_e = np.ones(len(df_iv))
                     tau_be = np.ones(len(df_iv))
                     tau_b = np.ones(len(df_iv))
                     tau_c = np.ones(len(df_iv))
                     tau_bc = np.ones(len(df_iv))
 
                     try:
-
                         for i_row, row in enumerate(df_iv.iterrows()):
                             key_inqu = next(
                                 _key
                                 for _key in self.data.keys()
                                 if "_inqu" in _key and "op" + str(i_row + 1) in _key
                             )
                             key_ac_inqu = next(
                                 _key
                                 for _key in self.data.keys()
                                 if "acinqu" in _key
                                 and "op" + str(i_row + 1) in _key
-                                and "port1" in _key
+                                and "dVb" in _key
                             )
 
                             # get the necessary data
                             df_ac_inqu_i = self.data[key_ac_inqu]
                             dn_dic = df_ac_inqu_i["re_d_n_x"].to_numpy() / gm[i_row + 1]
+                            try:
+                                dn2_dic = df_ac_inqu_i["re_d_n2_x"].to_numpy() / gm[i_row + 1]
+                            except KeyError:
+                                dn2_dic = df_ac_inqu_i["re_d_n_x"].to_numpy() / gm[i_row + 1]
+
                             dp_dic = df_ac_inqu_i["re_d_p_x"].to_numpy() / gm[i_row + 1]
                             droh_dic = dp_dic - dn_dic
                             # transit time
                             changes = (
                                 np.where(np.sign(droh_dic[:-1]) != np.sign(droh_dic[1:]))[0] + 1
                             )
                             index_be = changes[np.argmin(np.abs(changes - junctions[0]))]
                             index_bc = changes[np.argmin(np.abs(changes - junctions[1]))]
                             xbe = x[index_be]
                             xbc = x[index_bc]
 
                             tau = np.zeros(len(x))
+                            taup = np.zeros(len(x))
+                            taun = np.zeros(len(x))
+                            taun2 = np.zeros(len(x))
                             for j, x_ in enumerate(x):
                                 if x_ <= xbe:
                                     tau[j] += np.trapz(dp_dic[:j], x[:j])
                                     tau[j] += np.trapz(dn_dic[:j], x[:j]) - np.trapz(
                                         dp_dic[:j], x[:j]
                                     )
                                 elif x_ <= xbc:
                                     tau[j] += np.trapz(dn_dic[:j], x[:j])
                                 else:
                                     tau[j] += np.trapz(dp_dic[:j], x[:j])
                                     tau[j] += np.trapz(dn_dic[:j], x[:j]) - np.trapz(
                                         dp_dic[:j], x[:j]
                                     )
 
+                                taun[j] = np.trapz(dn_dic[:j], x[:j])
+                                taup[j] = np.trapz(dp_dic[:j], x[:j])
+                                taun2[j] = np.trapz(dn2_dic[:j], x[:j])
+
                             tau = tau * constants.P_Q
+                            taun = taun * constants.P_Q
+                            taun2 = taun2 * constants.P_Q
+                            taup = taup * constants.P_Q
 
                             tau_e[i_row] = np.trapz(dp_dic[:index_be], x[:index_be]) * constants.P_Q
                             tau_be[i_row] = (
                                 np.trapz(dn_dic[:index_be], x[:index_be]) * constants.P_Q
                                 - tau_e[i_row]
                             )
                             tau_b[i_row] = (
@@ -580,14 +685,17 @@
 
                             dm_dic = np.where(dn_dic < dp_dic, dn_dic, dn_dic)
 
                             # for j in range(len(tau)):
                             #     tau[j] = constants.P_Q * np.trapz(dm_dic[:j], x[:j])
 
                             self.data[key_inqu][specifiers.TRANSIT_TIME] = tau
+                            self.data[key_inqu]["TAUP"] = taup
+                            self.data[key_inqu]["TAUN"] = taun
+                            self.data[key_inqu]["TAUN2"] = taun2
 
                         df_iv["tau_e"] = tau_e
                         df_iv["tau_be"] = tau_be
                         df_iv["tau_b"] = tau_b
                         df_iv["tau_bc"] = tau_bc
                         df_iv["tau_c"] = tau_c
 
@@ -831,26 +939,38 @@
                         0,
                         -doping,
                         grading,
                     )
 
         return mob
 
-    def get_intervalley_rate(self, semiconductor, valley_1, valley_2, field, temperature, doping):
+    def get_intervalley_rate(
+        self, semiconductor, valley_1, valley_2, field, temperature, doping, grad=0
+    ):
         if not DutHdev.inited:
             self.init_()
 
         rec = np.zeros_like(field)
         for i in range(len(field)):
             rec[i] = hdev_py.get_intervalley_rate_py(
-                semiconductor, valley_1, valley_2, field[i], doping, temperature
+                semiconductor, valley_1, valley_2, field[i], doping, temperature, grad
             )
 
         return rec
 
+    def get_pop(self, semiconductor, temperature, doping):
+        if not DutHdev.inited:
+            self.init_()
+
+        pop = np.zeros_like(doping)
+        for i in range(len(doping)):
+            pop[i] = hdev_py.get_pop_py(semiconductor, temperature, doping[i])
+
+        return pop
+
     def get_mobility_paras(self, semi, valley):
         if not DutHdev.inited:
             self.init_()
 
         paras = hdev_py.get_mobility_paras_py(semi, valley)
         return paras
```

### Comparing `DMT_core-1.8.0rc1/DMT/config/DMT_config.yaml` & `DMT_core-2.0.0/DMT/config/DMT_config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,15 @@
     DEVICE:     device # Command to execute the TCAD simulator DEVICE.
     Hdev:       hdev # Command to execute the TCAD simulator Hdev.
     TRADICA:    tradica  # Command to execute the device geometry scaling software TRADICA.
     ADS:        hpeesofsim # Command to execute the circuit simulator of ADS.
     SPECTRE:    spectre # Command to execute the circuit simulator of Cadence spectre.
     SIMU:       simul # Command to execute the circuit simulator SIMU.
     NGSPICE:    ngspice # Command to execute the circuit simulator ngspice.
+    OPENVAF:    null # Command to execute the veriloga compiler OpenVAF.
     XYCE:       Xyce # Command to execute the circuit simulator Xyce.
     VMC:        vmc # Command to execute the MCBTE simulator VMC
     TEX:        pdflatex # Tex Compiler of your system
     TEXARGS:    #arguments for Tex Compiler
         - --shell-escape
         - --interaction=nonstopmode
 backend_remote: no # with yes, the simulations are run on the specified server, per default.
```

### Comparing `DMT_core-1.8.0rc1/DMT/config/__init__.py` & `DMT_core-2.0.0/DMT/config/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,73 +33,75 @@
 
 import os
 import platform
 import pkgutil
 import warnings
 import yaml
 from pathlib import Path
+from DMT.external.os import recursive_copy
 
 # dmt default config
 path_config = Path(__file__).resolve().parent
 default_config_file = path_config / "DMT_config.yaml"
-with open(default_config_file) as yaml_data_file:
-    DATA_CONFIG = yaml.safe_load(yaml_data_file)
+DATA_CONFIG = yaml.safe_load(default_config_file.read_text())
 
 # dmt user config
-data_user = {}
 
 if platform.system() == "Windows":
-    user_config = Path(os.getenv("LOCALAPPDATA")).expanduser()
+    user_config = os.getenv("LOCALAPPDATA")
 elif platform.system() == "Linux":
-    user_config = Path(
-        os.getenv("XDG_CONFIG_HOME") if os.getenv("XDG_CONFIG_HOME", False) else "~/.config"
-    ).expanduser()
+    user_config = os.getenv("XDG_CONFIG_HOME")
 elif platform.system() == "Darwin":
-    user_config = Path(
-        os.getenv("XDG_CONFIG_HOME") if os.getenv("XDG_CONFIG_HOME", False) else "~/.config"
-    ).expanduser()
+    user_config = os.getenv("XDG_CONFIG_HOME")
 else:
     raise OSError(
-        f"Unknown platform:{platform.system()}. Currently only Windows, Linux and MacOS are recognized"
+        f"Unknown platform:{platform.system()}. Currently only Windows, Linux and MacOS (Darwin) are recognized"
     )
 
-user_config = user_config / "DMT" / "DMT_config.yaml"
+if user_config:
+    user_config = Path(user_config).expanduser() / "DMT" / "DMT_config.yaml"
+else:
+    user_config = Path.home() / ".config" / "DMT" / "DMT_config.yaml"
+
+data_user = {}
 try:
-    with user_config.open() as yaml_data_file:
-        data_user = yaml.safe_load(yaml_data_file)
+    data_user = yaml.safe_load(user_config.read_text())
 except FileNotFoundError:
     try:
-        user_config = Path.home() / ".DMT" / "DMT_config.yaml"
-        with user_config.open() as yaml_data_file:
-            data_user = yaml.safe_load(yaml_data_file)
-        # warnings.warn(
-        #     "The DMT user configuration file is moved. The new paths are:",
-        #     "Windows: %LOCALAPPDATA%\DMT\DMT_config.yaml",
-        #     "Linux and MacOS: $XDG_CONFIG_HOME/DMT/DMT_config.yaml, defaulting to ~/.config/DMT/DMT_config.yaml",
-        #     category=DeprecationWarning,
-        # )
+        user_config_old = Path.home() / ".DMT" / "DMT_config.yaml"
+        data_user = yaml.safe_load(user_config_old.read_text())
+        warnings.warn(
+            (
+                "The DMT user configuration file has been moved. The new paths are:\n"
+                + "Windows: %LOCALAPPDATA%\DMT\DMT_config.yaml\n"
+                + "Linux and MacOS: $XDG_CONFIG_HOME/DMT/DMT_config.yaml\n"
+                + "Defaulting to ~/.config/DMT/DMT_config.yaml"
+            ),
+            category=DeprecationWarning,
+        )
     except FileNotFoundError:
         pass
 
+    user_config.parent.mkdir(exist_ok=True, parents=True)
+    user_config.write_text(yaml.safe_dump(data_user))
+
 if data_user:
     for key, value in DATA_CONFIG.items():
         if key in data_user.keys():
             if hasattr(DATA_CONFIG[key], "update"):
                 DATA_CONFIG[key].update(data_user[key])
             else:
                 if isinstance(DATA_CONFIG[key], list):  # lists are appended.
                     DATA_CONFIG[key] = DATA_CONFIG[key] + data_user[key]
                 else:
                     DATA_CONFIG[key] = data_user[key]
 
 # finally workspace path
 try:
-    local_config = Path("DMT_config.yaml")
-    with local_config.open() as yaml_data_file:
-        data_folder = yaml.safe_load(yaml_data_file)
+    data_folder = yaml.safe_load(Path("DMT_config.yaml").read_text())
 
     for key, value in DATA_CONFIG.items():
         if key in data_folder.keys():
             try:
                 DATA_CONFIG[key].update(data_folder[key])
             except AttributeError:
                 if isinstance(DATA_CONFIG[key], list):  # lists are appended.
@@ -156,17 +158,14 @@
     """
     if file_path is None:
         print(DATA_CONFIG)
     else:
         yaml.safe_dump(DATA_CONFIG, file_path)
 
 
-from DMT.external.os import recursive_copy
-
-
 def generate_libdoc_template(directory):
     """Copies the DMT template for the DutLib documentation into the given directory. This allows to change the template according to your needs.
 
     Parameters
     ----------
     directory : str
         Path to copy to.
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/__init__.py` & `DMT_core-2.0.0/DMT/core/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,57 +13,48 @@
 # DMT_core is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
-
+import pkgutil
 from pint import UnitRegistry
 from pathlib import Path
-from pkg_resources import get_distribution
+from importlib.metadata import version
+from packaging.version import Version as PyPIVersion
 
-version_pkg = get_distribution("DMT-core").version.split(".")
+version_pkg = PyPIVersion(version("DMT-core"))
 try:
     from semver.version import Version as VersionInfo
 except ImportError:
     from semver import VersionInfo
 
-if "rc" in version_pkg[2]:
-    _patch = version_pkg[2].split("rc")[0]
-    _rc = version_pkg[2][len(_patch) + 2 :]
-    __version__ = VersionInfo(
-        major=version_pkg[0],
-        minor=version_pkg[1],
-        patch=_patch,
-        prerelease="rc." + _rc,
-    )
-else:
-    __version__ = VersionInfo(major=version_pkg[0], minor=version_pkg[1], patch=version_pkg[2])
+version_pre = None
+if version_pkg.pre:
+    version_pre = ".".join(version_pkg.pre)
+
+__version__ = VersionInfo(*version_pkg.release, prerelease=version_pre, build=version_pkg.dev)
 
 # to get the next version:
 # __version__.next_version(x) - with x = "major", "minor", "patch", "prerelease"
 # or
 # __version__.bump_x() - with x = "major", "minor", "patch", "prerelease"
 
 name = "core"
 
-
 from . import constants
 
 # Helper
 from .singleton import Singleton
 from .hasher import create_md5_hash
+from DMT.config import DATA_CONFIG
 
 # one unit registry for all of DMT
-
 unit_registry = UnitRegistry()
-from DMT.config import DATA_CONFIG
-
-
 path_core = Path(__file__).resolve().parent
 unit_registry.load_definitions(str(path_core / "dmt_units.txt"))
 
 # helper for model equations and mcard memoization
 from .utils import print_progress_bar
 from .utils import enumerate_reversed
 
@@ -75,16 +66,16 @@
 from .naming import get_nodes
 from .naming import set_col_name
 from .naming import SpecifierStr
 from .naming import get_sub_specifiers
 from .naming import natural_scales
 
 # compact modelling stuff
-from .mc_parameter import McParameter, McParameterCollection, McParameterComposition
-from .va_file import VAFile
+from .mc_parameter import McParameter, McParameterCollection
+from .va_file import VAFileMap
 from .mcard import MCard
 from .technology import Technology
 from .circuit import Circuit, CircuitElement
 from .mc_skywater import McSkywater
 
 # plotting
 from .plot import Plot
@@ -107,37 +98,38 @@
     read_DEVICE_bin,
     read_elpa,
     read_mdm,
     read_hdf,
     read_feather,
 )
 
-
 # Simulation management
 from .sim_con import SimCon
 
 # DutView tree
+from .dut_type import DutType, DutTypeFlag, DutTypeInt
 from .dut_view import DutView
-from .dut_type import DutType
 from .dut_lib import DutLib
 
 from .dut_meas import DutMeas
 from .dut_dummy import DutDummy
 
 from .dut_circuit import DutCircuit
 
 from .dut_tcad import DutTcad
 
+_DEFAULT_DUT_VIEWS = [DutView, DutMeas, DutDummy, DutCircuit, DutTcad]
 # docu
 from .docu_dut_lib import DocuDutLib
 
 # determine which modules are present
 core_exists = True  # always, without DMT is not possible
 try:
-    import DMT.extraction
+    pkgutil.find_loader("DMT.extraction")
+    # import DMT.extraction
 
     extraction_exists = True
 except ImportError:
     extraction_exists = False
 
 
 if core_exists and not extraction_exists:
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/circuit.py` & `DMT_core-2.0.0/DMT/core/circuit.py`

 * *Files 4% similar despite different names*

```diff
@@ -53,44 +53,38 @@
 DIODE = "diode"
 """ Indicates a diode in a circuit. """
 
 
 class CircuitElement(object):
     """Class that is used to describe netlist elements such as resistors, capacitors or inductors.
 
-    The possible CircuitElements define the DMT netlist format. Circuit simulators need to convert the DMT netlist format to their respective one.
-    This class has a special emphasis on good error messages and typesetting.
-
-    Possible element types:
+    The possible CircuitElements define the DMT netlist format. Circuit simulator interfaces need to convert the DMT netlist format to their respective one.
 
-    * :py:const:`RESISTANCE`
-    * :py:const:`CAPACITANCE`Sequence
-    * :py:const:`SHORT`
-    * va_module -> could be a transistor
+    This class has a special emphasis on good error messages and typesetting.
 
     Parameters
     ----------
-    element_type
-        Element type, for example: 'R' for resistor. possible values: 'V_Source', 'I_Source', 'R', 'C', 'L', 'Short' ,'va_module'
-    name
+    element_type : str
+        Element type, possible values see are :py:attr:`CircuitElement.possible_types`.
+    name : str
         Element name, for example: 'R1' for resistor 1. Names should be unique within their netlist.
-    contact_nodes
+    contact_nodes : tuple[str]
         Contact nodes of the element, for example: ('n__1', 'n__2')
-    parameters
+    parameters : list[tuple[str]]
         Parameters of the element, for example: [('R', '1k')]
 
     Attributes
     ----------
-    element_type
-        Element type, for example: 'R' for resistor
-    name
+    element_type : str
+        Element type, possible values see are :py:attr:`CircuitElement.possible_types`.
+    name : str
         Element name, for example: 'R1' for resistor 1
-    contact_nodes
+    contact_nodes : tuple[str]
         Contact nodes of the element, for example: ('n__1', 'n__2')
-    parameters
+    parameters : list[tuple[str]]
         Parameters of the element, for example: [('R', '1k')]
     """
 
     possible_types = [
         VOLTAGE,
         CURRENT,
         RESISTANCE,
@@ -125,15 +119,14 @@
 
     def __init__(
         self,
         element_type: str,
         name: str,
         contact_nodes: Iterable[str],
         parameters: Optional[Union[List[Tuple[str, str]], MCard, McParameterCollection]] = None,
-        method: Optional[Callable] = None,
     ):
         if isinstance(parameters, MCard) or isinstance(parameters, McParameterCollection):
             CircuitElement.possible_types.append(parameters.default_module_name)  # type: ignore
 
         if isinstance(element_type, str):
             if element_type in self.possible_types:
                 self.element_type = element_type
@@ -209,46 +202,39 @@
             raise TypeError(
                 "The parameters have to be a list of tuple of strings or a modelcard! Given was a "
                 + type(parameters)
             )
 
         self.parameters = parameters
 
-        if method is not None:
-            warnings.warn(
-                "method will be deprecated in future DMT releases. This feature is not needed anymore since VAE is mature.",
-                category=DeprecationWarning,
-            )
-        self.method = method
-
     def __repr__(self):
         str_nodes = ",".join(self.contact_nodes)
         return f"DMT.CircuitElement:{self.name:s} model {self.element_type:s} nodes {str_nodes:s}"
 
 
 class Circuit(object):
     """Circuit description as a list of :class:`CircuitElement`
 
     Parameters
     ----------
-    circuit_elements
+    circuit_elements : List[Union[str, CircuitElement]]
         Either directly the netlist elements as a list of CircuitElements or strings (for equations)
 
     Attributes
     ----------
-    netlist
+    netlist : List[Union[str, CircuitElement]]
         Either directly the netlist elements as a list of CircuitElements or strings (for equations)
+
+    Raises
+    ------
+    TypeError
+        If one element of the circuit to create is neither a :class:`~DMT.core.circuit.CircuitElement` nor a simple str.
     """
 
     def __init__(self, circuit_elements: List[Union[str, CircuitElement]]):
-        if isinstance(circuit_elements, str):
-            raise NotImplementedError(
-                "The default circuit has been moved into the corresponding module. Access the circuit from there!"
-            )
-
         for i_element, element in enumerate(circuit_elements):
             if not isinstance(element, (CircuitElement, str)):
                 raise TypeError(
                     "The netlist has to be a list of CircuitElement or str! At position "
                     + str(i_element)
                     + " is a entry of type "
                     + type(element)
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/constants.py` & `DMT_core-2.0.0/DMT/core/constants.py`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/core/data_frame.py` & `DMT_core-2.0.0/DMT/core/data_frame.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,15 @@
     flatten,
     DataProcessor,
 )
 import pandas as pd
 
 # pylint: disable = too-many-lines
 
+
 # helper functions for Y Parameter smoothing
 def fun_re(freq, a1, a2, a3):
     """Fit function for real Y Parameters normalized."""
     omega_sq = (2 * np.pi * freq) ** 2
     return (a1 + a2 * omega_sq) / (1 + a3 * omega_sq)
 
 
@@ -55,15 +56,14 @@
     """Fit function for imaginary Y Parameters normalized to omega."""
     omega = 2 * np.pi * freq
     omega_sq = omega**2
     return (a2) / (1 + a3 * omega_sq)
 
 
 class Series(pd.Series):
-
     _metadata = ["processor"]
 
     @property
     def _constructor(self):
         return Series
 
     @property
@@ -376,15 +376,15 @@
 
         if fallback is None:
             fallback = {}
         fallback[specifier_temperature] = specifiers.TEMPERATURE
         fallback[specifier_frequency] = specifiers.FREQUENCY
 
         # rename columns that are specified by fallback
-        new_df = DataFrame()
+        data = {}
         unknown_columns = []
         for col in self.columns:
             if col in fallback.keys():
                 # the complete column name is in the fallback. So use it!
                 if fallback[col] is None:
                     if warnings:
                         logging.warning(
@@ -394,22 +394,22 @@
                 elif fallback[col]:
                     if warnings:
                         logging.warning(
                             "The column %s is kept as %s according to the fallback dictionary!",
                             col,
                             fallback[col],
                         )
-                    new_df[fallback[col]] = self[col]
+                    data[fallback[col]] = self[col].to_numpy()
                 else:
                     if warnings:
                         logging.warning(
                             "The column %s is kept it was according to the fallback dictionary!",
                             col,
                         )
-                    new_df[col] = self[col]
+                    data[col] = self[col].to_numpy()
 
                 continue
 
             if re.search(r"deemb", col, re.IGNORECASE):
                 raise IOError(
                     "Found a possible already deembeded column. This column must be dropped for DMT! To do that add the following to the fallback: {{'{0:s}': None}}".format(
                         col
@@ -427,15 +427,15 @@
                         "DMT->DataFrame->clean_data: The column"
                         + str(col[0])
                         + " was identified as a small-signal parameter but the ac_ports argument was not specified."
                     )
 
             elif col[0] not in "VIC":
                 # only rename the names of values which can be identified
-                new_df[col] = self[col]
+                data[col] = self[col].to_numpy()
                 continue
 
             nodes_in_col = get_nodes(col, nodes, fallback=fallback)
             sub_specifiers_in_col = get_sub_specifiers(col)
             # if more than 3 nodes, something is weird and we dont do anything
             # if len(nodes_in_col)>2:
             #     # only rename the names of values which can be identified
@@ -445,36 +445,36 @@
                 continue
             elif nodes_in_col:
                 # new_column_name = col[0] + r'_' + ''.join(nodes_in_col)
                 new_column_name = SpecifierStr(
                     col[0], *nodes_in_col, sub_specifiers=sub_specifiers_in_col
                 )
                 # self  =  self.rename(columns={ self.columns[i]:new_column_name })
-                if new_column_name in new_df.columns:  # pylint: disable=unsupported-membership-test
+                if new_column_name in data:
                     raise IOError(
                         "Column is already in the dataframe. Maybe it should be deleted? (fallback: {"
                         + new_column_name
                         + " :None})"
                     )
-                new_df[new_column_name] = self[col]
+                data[new_column_name] = self[col].to_numpy()
             else:
                 unknown_columns.append(col)
 
         if len(unknown_columns) > 1:
             str_columns = ""
             for col in unknown_columns:
                 str_columns += " " + str(col) + " "
 
             raise UnknownColumnError(
                 "The columns "
                 + str_columns
                 + " is unknown to this DuT as the nodes can not be extracted! Either a fallback behavior or different DuT nodes for this column are needed."
             )
 
-        self = new_df
+        self = DataFrame(data)
 
         # convert voltages, potentials and maybe in the future to SpecifierStr
         to_rename = {}
         temp_nodes = nodes + [
             key for key, value in fallback.items() if value == ""
         ]  # for this case also the "keep"-nodes from the fallback are possible
         for column in self.columns:  # pylint: disable=not-an-iterable
@@ -700,15 +700,15 @@
             col_complex = SpecifierStr(
                 specifier,
                 *nodes,
                 sub_specifiers=sub_specifiers_in_col - sub_specifiers.REAL.sub_specifiers,
             )
             self.ensure_specifier_column(col_complex, ports=ports)
             self[col] = np.real(self[col_complex].to_numpy())
-
+            return
         elif (
             sub_specifiers.IMAG.sub_specifiers <= sub_specifiers_in_col
         ):  # [1:] to cut off the | for a correct string compare
             col_complex = SpecifierStr(
                 specifier,
                 *nodes,
                 sub_specifiers=sub_specifiers_in_col - sub_specifiers.IMAG.sub_specifiers,
@@ -722,15 +722,15 @@
             col_complex = SpecifierStr(
                 specifier,
                 *nodes,
                 sub_specifiers=sub_specifiers_in_col - sub_specifiers.MAG.sub_specifiers,
             )
             self.ensure_specifier_column(col_complex, ports=ports)
             self[col] = np.abs(self[col_complex].to_numpy())
-
+            return
         elif (
             sub_specifiers.PHASE.sub_specifiers <= sub_specifiers_in_col
         ):  # [1:] to cut off the | for a correct string compare
             col_complex = SpecifierStr(
                 specifier,
                 *nodes,
                 sub_specifiers=sub_specifiers_in_col - sub_specifiers.PHASE.sub_specifiers,
@@ -773,35 +773,34 @@
                 self[specifiers.CURRENT + nodes[0]] / area
             )
         elif (specifier == specifiers.CAPACITANCE) and (len(nodes) == 2):
             if ports is None:
                 raise IOError(
                     'DMT -> DataFrame -> ensure_specifier_column: Calculation of a capacitance requires the specification of the "ports" keyword argument.'
                 )
-            if any(
-                sub_specifier_poa.sub_specifiers <= sub_specifiers_in_col
-                for sub_specifier_poa in [
-                    sub_specifiers.PERIMETER,
-                    sub_specifiers.AREA,
-                    sub_specifiers.CORNER,
-                    sub_specifiers.LENGTH,
-                    sub_specifiers.WIDTH,
-                ]
-            ):
+            if sub_specifiers_in_col & {
+                sub_specifiers.PERIMETER,
+                sub_specifiers.AREA,
+                sub_specifiers.CORNER,
+                sub_specifiers.LENGTH,
+                sub_specifiers.WIDTH,
+            }:
                 raise IOError(
                     "DMT -> DataFrame -> ensure_specifier_column: Can not calculate a PoA capacitance. This needs to be done by a XQ Step."
                 )
 
             try:
                 if nodes[0] == "B" and nodes[1] == "E":  # CBE
                     self = self.calc_cbe(port_1=ports[0], port_2=ports[1])
                 elif nodes[0] == "C" and nodes[1] == "E":  # CCE
                     self = self.calc_cce(port_1=ports[0], port_2=ports[1])
                 elif nodes[0] == "B" and nodes[1] == "C":  # CBC
                     self = self.calc_cbc(port_1=ports[0], port_2=ports[1])
+                elif nodes[0] == "G" and nodes[1] == "S":  # CGS
+                    self = self.calc_cgs(port_1=ports[0], port_2=ports[1])
                 else:
                     raise KeyError("The " + "".join(nodes) + " capacitance can not be calculated.")
             except IOError as err:
                 raise KeyError(
                     "The " + "".join(nodes) + " capacitance could not be calculated."
                 ) from err
 
@@ -867,14 +866,21 @@
         elif specifier == specifiers.TRANSCONDUCTANCE:
             try:
                 self = self.calc_gm()
             except IOError as err:
                 raise KeyError(
                     "The transconductance is missing in the given data frame and can not be calculated."
                 ) from err
+        elif specifier == specifiers.OUTPUT_CONDUCTANCE:
+            try:
+                self = self.calc_go()
+            except IOError as err:
+                raise KeyError(
+                    "The transconductance is missing in the given data frame and can not be calculated."
+                ) from err
         elif specifier in specifiers_ss_para:
             try:  # try tog et from S paras
                 self = self.convert_n_port_para(p_from="S", p_to=specifier, ports=ports)
             except IOError as err:  # try to get from Y paras
                 try:
                     self = self.convert_n_port_para(p_from="Y", p_to=specifier, ports=ports)
                 except:
@@ -1436,17 +1442,15 @@
         -------
         dict
             A dict of resistances Rb,m, Rc,m, and Re,m.
 
         """
 
         if forced_current:
-
             try:
-
                 df_RC = self.loc[np.isclose(self[specifiers.CURRENT + "B"], 0.0, atol=1e-6)]
                 df_RB = self.loc[np.isclose(self[specifiers.CURRENT + "C"], 0.0, atol=1e-6)]
             except KeyError:
                 raise IOError
 
             mres = {}
 
@@ -1526,15 +1530,16 @@
 
         """
         for col in self.columns:  # pylint: disable=not-an-iterable
             try:
                 if col.specifier == para:
                     return True
             except AttributeError:
-                if col[0:2] == para + "_":  # we should no allow this :(
+                if col.startswith(str(para) + "_"):
+                    # we should no allow this :(
                     return True
 
         return False
 
     def get_ss_para(self, para, port_1, *ports_n):
         """Return an array of the small signal (ss) parameters para in df.
 
@@ -1550,66 +1555,73 @@
         Returns
         -------
         np.ndarray()
             Numpy array containing the values of the ss parameter para with shape [n_freq,n_port_in,n_port_out].
         """
         # check existence of the paras
         para_desired = para
-        try:
-            para_avail = [
-                ss_para
-                for ss_para in [para] + [speci for speci in specifiers_ss_para]
-                if self.check_ss_cols(ss_para)
-            ]
-            if len(para_avail) == 0:
-                raise StopIteration
-            elif len(para_avail) == 1:
-                para_avail = para_avail[0]
-            else:
-                if para_desired in para_avail:
-                    para_avail = para_desired
-                else:
-                    para_avail = para_avail[0]
-        except StopIteration:
+        paras_avail = [
+            ss_para for ss_para in {para} | set(specifiers_ss_para) if self.check_ss_cols(ss_para)
+        ]
+        if len(paras_avail) == 0:
             logging.warning("Warning: DMT->DataFrame: No SS-Parameters were found in DataFrame.")
-            raise StopIteration
+            raise StopIteration("DMT->DataFrame: No SS-Parameters were found in DataFrame.")
+
+        if para_desired in paras_avail:
+            paras_avail.remove(para_desired)
+            paras_avail.insert(0, para_desired)
+
+        columns = set(self.columns)
+        ports_wanted = [port_1] + list(ports_n)
+        ports_of_para = []
+        para_found = None
+        for para_test in paras_avail:
+            spec_test = SpecifierStr(para_test.upper())
+            if (spec_test + [port_1, port_1]) not in columns:
+                continue
 
-        list_ports = [port_1]
-        columns = self.columns
-        for node in ports_n:
-            # check if full set of this parameter is here for this node
-            col_0 = SpecifierStr(para_avail.upper(), port_1, node)
-            col_1 = SpecifierStr(para_avail.upper(), node, port_1)
-            col_2 = SpecifierStr(para_avail.upper(), node, node)
-
-            # did not check for node[i], node[j] on purpose, because node[j] may be not part of the full set..
-            if (
-                col_0 in columns and col_1 in columns and col_2 in columns
-            ):  # pylint: disable=unsupported-membership-test
-                list_ports.append(node)
+            ports_of_para = [port_1]
+            for node in ports_n:
+                # check if full set of this parameter is here for this node
+                col_0 = spec_test + [port_1, node]
+                col_1 = spec_test + [node, port_1]
+                col_2 = spec_test + [node, node]
+                # did not check for node[i], node[j] on purpose, because node[j] may be not part of the full set..
+
+                if len({col_0, col_1, col_2} & columns) == 3:
+                    ports_of_para.append(node)
+
+            if ports_of_para == ports_wanted:
+                para_found = spec_test
+                break
+
+        if not para_found:
+            raise IOError(
+                "DMT-DataFrame->get_ss_para: I found some SS-Paras but none with full set for all required ports."
+            )
 
         # get the existing parameters from df and put them into a numpy array
         try:
             n_freq = len(self[specifiers.FREQUENCY])
         except KeyError:
-            raise IOError("DMT -> data_frame -> get_ss_para: no column FREQ in data frame.")
+            raise IOError("DMT->DataFrame->get_ss_para: no column FREQ in data frame.")
 
-        n_port = len(list_ports)
+        n_port = len(ports_of_para)
 
         para_values = np.zeros((n_freq, n_port, n_port), dtype=np.complex128)
         for i in range(n_port):
             for j in range(n_port):
                 para_values[:, i, j] = self.loc[
-                    :, SpecifierStr(para_avail.upper(), list_ports[i], list_ports[j])
+                    :, para_found + [ports_of_para[i], ports_of_para[j]]
                 ]
 
         # we found some parameters, however not the desired ones. Try converting
-        if para_avail != para_desired:
+        if para_found != para_desired:
             para_values = self.processor.convert_n_port_para(
-                para_values, p_from=str(para_avail), p_to=str(para_desired)
+                para_values, p_from=str(para_found), p_to=str(para_desired)
             )
 
         return para_values
 
     def set_ss_para(self, para, para_values, port_1, *ports_n):
         """Create or update the columns corresponding to small signal (ss) parameters para in df using the values in para_values.
 
@@ -1635,15 +1647,15 @@
         for i in range(n_port):
             for j in range(n_port):
                 para_str = SpecifierStr(para, list_nodes[i], list_nodes[j])
                 self[para_str] = para_values[:, i, j]
 
         return self
 
-    def strip_ss_para(self, keep="S"):
+    def strip_ss_para(self, keep=specifiers_ss_para.SS_PARA_S):
         """Throw away all but keep small signal parameters.
 
         Parameters
         ----------
         keep  :  string
             Default='S'. SS Para that shall be kept.
 
@@ -1651,15 +1663,15 @@
         -------
         :class:`DMT.core.DataFrame`
             The initial DataFrame without all ss parameters except keep.
         """
         ss_paras = self.get_all_ss_para()
         drop = []
         for para in ss_paras:
-            if para.specifier != keep:
+            if para.specifier != str(keep):
                 drop.append(para)
 
         return self.drop(columns=drop)
 
     def get_all_ss_para(self):
         """Return a list of strings of all small signal parameters (ss) in df.
 
@@ -1723,23 +1735,25 @@
         # put values in col of self
         self.loc[:, specifiers.TRANSIT_TIME] = self.processor.calc_tfit2(
             self[specifiers.FREQUENCY], s_para_values, "S"
         )
         return self
 
     def calc_tfit(self, tfit_kind: int, ports):
-        port1 = ports[0]
-        port2 = ports[1]
         if tfit_kind == 1:
-            return self.calc_tfit1(port1, port2)
+            return self.calc_tfit1(*ports)
         elif tfit_kind == 2:
-            return self.calc_tfit2(port1, port2)
+            return self.calc_tfit2(*ports)
         elif tfit_kind == 3:
             self.ensure_specifier_column(specifiers.TRANSIT_TIME, ports=ports)
             return self
+        else:
+            raise NotImplementedError(
+                "DMT-DataFrame-calc_tfit: Only kind 1,2 and 3 is implemented!"
+            )
 
     def calc_tfit1(self, port_1, port_2):
         """Calculates the transit frequency FT using the spot frequency method.
 
         Parameters
         ----------
         port_1        : string
@@ -1869,45 +1883,84 @@
         # get values
         s_para_values = self.get_ss_para("S", port_1, port_2)
 
         # put values in col of self
         self["K"] = self.processor.calc_k(self["FREQ"], s_para_values, "S")
         return self
 
+    def calc_cgs(self, port_1="B", port_2="C"):
+        """Calculates the gate-source capacitance CGS assuming PI equivalent circuit and common source configuration.
+
+        Returns
+        -------
+        :class:`DMT.core.DataFrame`
+            Dataframe that contains CBE.
+        """
+        # get values
+        s_para_values = self.get_ss_para("Y", port_1, port_2)
+
+        sp_cgs = specifiers.CAPACITANCE + ["G", "S"]
+
+        # put values in col of self
+        pd.options.mode.chained_assignment = (
+            None  # default='warn' , Markus: This should not warn here.
+        )
+        if port_1 == "G" and port_2 == "D":
+            self[sp_cgs] = self.processor.calc_cap_shunt_port_1(self["FREQ"], s_para_values, "Y")
+        elif port_1 == "D" and port_2 == "G":
+            self[sp_cgs] = self.processor.calc_cap_shunt_port_2(self["FREQ"], s_para_values, "Y")
+        elif port_1 == "G" and port_2 == "S":
+            self[sp_cgs] = self.processor.calc_cap_series_thru(self["FREQ"], s_para_values, "Y")
+        elif port_1 == "S" and port_2 == "B":
+            self[sp_cgs] = self.processor.calc_cap_series_thru(self["FREQ"], s_para_values, "Y")
+        elif port_1 == "S" and port_2 == "D":  # common base
+            self[sp_cgs] = self.processor.calc_cap_shunt_port_1(self["FREQ"], s_para_values, "Y")
+        elif port_1 == "S" and port_2 == "D":  # common base
+            self[sp_cgs] = self.processor.calc_cap_shunt_port_2(self["FREQ"], s_para_values, "Y")
+        elif port_1 == "D" and port_2 == "S":  # common base
+            self[sp_cgs] = self.processor.calc_cap_shunt_port_1(self["FREQ"], s_para_values, "Y")
+        else:
+            raise NotImplementedError(
+                "DMT -> DataFrame -> calc_cgs: transistor configuration not implemented."
+            )
+
+        pd.options.mode.chained_assignment = "warn"
+        return self
+
     def calc_cbe(self, port_1="B", port_2="C"):
         """Calculates the base-emitter junction capacitance CBE assuming PI equivalent circuit and common emitter configuration.
 
         Returns
         -------
         :class:`DMT.core.DataFrame`
             Dataframe that contains CBE.
         """
         # get values
-        s_para_values = self.get_ss_para("S", port_1, port_2)
+        s_para_values = self.get_ss_para("Y", port_1, port_2)
 
         sp_cbe = specifiers.CAPACITANCE + ["B", "E"]
 
         # put values in col of self
         pd.options.mode.chained_assignment = (
             None  # default='warn' , Markus: This should not warn here.
         )
         if port_1 == "B" and port_2 == "C":
-            self[sp_cbe] = self.processor.calc_cap_shunt_port_1(self["FREQ"], s_para_values, "S")
+            self[sp_cbe] = self.processor.calc_cap_shunt_port_1(self["FREQ"], s_para_values, "Y")
         elif port_1 == "C" and port_2 == "B":
-            self[sp_cbe] = self.processor.calc_cap_shunt_port_2(self["FREQ"], s_para_values, "S")
+            self[sp_cbe] = self.processor.calc_cap_shunt_port_2(self["FREQ"], s_para_values, "Y")
         elif port_1 == "B" and port_2 == "E":
-            self[sp_cbe] = self.processor.calc_cap_series_thru(self["FREQ"], s_para_values, "S")
+            self[sp_cbe] = self.processor.calc_cap_series_thru(self["FREQ"], s_para_values, "Y")
         elif port_1 == "E" and port_2 == "B":
-            self[sp_cbe] = self.processor.calc_cap_series_thru(self["FREQ"], s_para_values, "S")
+            self[sp_cbe] = self.processor.calc_cap_series_thru(self["FREQ"], s_para_values, "Y")
         elif port_1 == "E" and port_2 == "C":  # common base
-            self[sp_cbe] = self.processor.calc_cap_shunt_port_1(self["FREQ"], s_para_values, "S")
+            self[sp_cbe] = self.processor.calc_cap_shunt_port_1(self["FREQ"], s_para_values, "Y")
         elif port_1 == "E" and port_2 == "C":  # common base
-            self[sp_cbe] = self.processor.calc_cap_shunt_port_2(self["FREQ"], s_para_values, "S")
+            self[sp_cbe] = self.processor.calc_cap_shunt_port_2(self["FREQ"], s_para_values, "Y")
         elif port_1 == "C" and port_2 == "E":  # common base
-            self[sp_cbe] = self.processor.calc_cap_shunt_port_1(self["FREQ"], s_para_values, "S")
+            self[sp_cbe] = self.processor.calc_cap_shunt_port_1(self["FREQ"], s_para_values, "Y")
         else:
             raise NotImplementedError(
                 "DMT -> DataFrame -> calc_cbe: transistor configuration not implemented."
             )
 
         pd.options.mode.chained_assignment = "warn"
         return self
@@ -1917,52 +1970,58 @@
 
         Returns
         -------
         :class:`DMT.core.DataFrame`
             Dataframe that contains CCE.
         """
         # get values
-        s_para_values = self.get_ss_para("S", port_1, port_2)
+        s_para_values = self.get_ss_para("Y", port_1, port_2)
 
         # put values in col of self
         pd.options.mode.chained_assignment = (
             None  # default='warn' , Markus: This should not warn here.
         )
-        self[specifiers.CAPACITANCE + ["C", "E"]] = self.processor.calc_cap_shunt_port_2(
-            self["FREQ"], s_para_values, "S"
-        )
+        if port_1 == "B" and port_2 == "C":
+            self[specifiers.CAPACITANCE + ["C", "E"]] = self.processor.calc_cap_shunt_port_2(
+                self["FREQ"], s_para_values, "Y"
+            )
+        else:
+            raise NotImplementedError(
+                "DMT -> DataFrame -> calc_cce: transistor configuration not implemented."
+            )
+
         pd.options.mode.chained_assignment = "warn"
         return self
 
     def calc_cbc(self, port_1="B", port_2="C"):
         """Calculates the base-collector junction capacitance CBC.
 
         Returns
         -------
         :class:`DMT.core.DataFrame`
             Dataframe that contains CBE.
         """
         # get values
-        s_para_values = self.get_ss_para("S", port_1, port_2)
+        s_para_values = self.get_ss_para("Y", port_1, port_2)
 
         sp_cbc = specifiers.CAPACITANCE + ["B", "C"]
 
         # put values in col of self
         if port_1 == "B" and port_2 == "C":
-            self[sp_cbc] = self.processor.calc_cap_series_thru(self["FREQ"], s_para_values, "S")
+            self[sp_cbc] = self.processor.calc_cap_series_thru(self["FREQ"], s_para_values, "Y")
         elif port_1 == "C" and port_2 == "B":
-            self[sp_cbc] = self.processor.calc_cap_series_thru(self["FREQ"], s_para_values, "S")
+            self[sp_cbc] = self.processor.calc_cap_series_thru(self["FREQ"], s_para_values, "Y")
         elif port_1 == "B" and port_2 == "E":
-            self[sp_cbc] = self.processor.calc_cap_shunt_port_1(self["FREQ"], s_para_values, "S")
+            self[sp_cbc] = self.processor.calc_cap_shunt_port_1(self["FREQ"], s_para_values, "Y")
         elif port_1 == "E" and port_2 == "B":
-            self[sp_cbc] = self.processor.calc_cap_shunt_port_2(self["FREQ"], s_para_values, "S")
+            self[sp_cbc] = self.processor.calc_cap_shunt_port_2(self["FREQ"], s_para_values, "Y")
         elif port_1 == "C" and port_2 == "E":
-            self[sp_cbc] = self.processor.calc_cap_shunt_port_1(self["FREQ"], s_para_values, "S")
+            self[sp_cbc] = self.processor.calc_cap_shunt_port_1(self["FREQ"], s_para_values, "Y")
         elif port_1 == "E" and port_2 == "C":
-            self[sp_cbc] = self.processor.calc_cap_shunt_port_2(self["FREQ"], s_para_values, "S")
+            self[sp_cbc] = self.processor.calc_cap_shunt_port_2(self["FREQ"], s_para_values, "Y")
         else:
             raise NotImplementedError(
                 "DMT -> DataFrame -> calc_cbe: transistor configuration not implemented."
             )
         return self
 
     def calc_beta(self):
@@ -2014,14 +2073,35 @@
         except KeyError:
             self.loc[:, specifiers.TRANSCONDUCTANCE] = self.processor.calc_gm(
                 self[col_ic].to_numpy(), self[col_vbe].to_numpy()
             )
 
         return self
 
+    def calc_go(self):
+        """Calculates the DC output condutance of a BJT.
+
+        Returns
+        -------
+        :class:`DMT.core.DataFrame`
+            Dataframe that contains the TRANSCONDUCTANCE
+        """
+        col_ic = specifiers.CURRENT + "C"
+        col_vce_forced = specifiers.VOLTAGE + "C" + "E" + sub_specifiers.FORCED
+
+        # get voltages
+        self.ensure_specifier_column(col_vce_forced)
+        self.ensure_specifier_column(col_ic)
+
+        self.loc[:, specifiers.OUTPUT_CONDUCTANCE] = self.processor.calc_go(
+            self[col_ic].to_numpy(), self[col_vce_forced].to_numpy()
+        )
+
+        return self
+
     def smooth_SS_para(self, ports, fmin):
         """Smooth the Small signal parameters in self and return a new dataframe.
 
         Method from:
         B. Saha et al.,
         "Reliable Technology Evaluation of SiGe HBTs and MOSFETs: fMAX Estimation From Measured Data,"
         in IEEE Electron Device Letters, vol. 42, no. 1, pp. 14-17, Jan. 2021, doi: 10.1109/LED.2020.3040891.
@@ -2042,15 +2122,15 @@
             Dataframe that contains the smoothed Y Parameters
         """
         # make sure we have all Y parameters available
         for port1 in ports:
             for port2 in ports:
                 for kind in [sub_specifiers.REAL, sub_specifiers.IMAG]:
                     self.ensure_specifier_column(
-                        specifiers_ss_para.SS_PARA_Y + port1 + port2 + kind,
+                        specifiers_ss_para.SS_PARA_Y + [port1, port2] + kind,
                         ports=["B", "C"],
                     )
 
         # assume this is real measurement data: freq is strictly increasing and we can just always get next N_FREQ values
         freq = np.unique(self[specifiers.FREQUENCY].to_numpy())
         n_freq = len(freq)
         n_rows = len(self.index)
@@ -2059,22 +2139,22 @@
         df_new = copy.deepcopy(self)
         # remove all small signal parameters in df_new and prepare new columns
         df_new = df_new.strip_ss_para(keep="S")
         df_new = df_new.strip_ss_para(keep="Y")
         for port1 in ports:
             for port2 in ports:
                 for kind in [sub_specifiers.REAL, sub_specifiers.IMAG]:
-                    y_para = specifiers_ss_para.SS_PARA_Y + port1 + port2 + kind
+                    y_para = specifiers_ss_para.SS_PARA_Y + [port1, port2] + kind
                     df_new[y_para] = 0
 
         # actual smoothing
         for port1 in ports:
             for port2 in ports:
                 for kind in [sub_specifiers.REAL, sub_specifiers.IMAG]:
-                    y_para = specifiers_ss_para.SS_PARA_Y + port1 + port2 + kind
+                    y_para = specifiers_ss_para.SS_PARA_Y + [port1, port2] + kind
                     for i in range(n_slices):
                         i_low = n_freq * i
                         i_upp = n_freq * (i + 1)
 
                         freq_i = self.iloc[i_low:i_upp][specifiers.FREQUENCY].to_numpy()
                         indices = freq_i > fmin
 
@@ -2100,17 +2180,17 @@
                         df_new.iloc[i_low:i_upp, df_new.columns.get_loc(y_para)] = (
                             fun(np.log10(freq_i), *popt) * norm
                         )
 
         # merge real and complex part, remove afterwards
         for port1 in ["B", "C"]:
             for port2 in ["B", "C"]:
-                y_para = specifiers_ss_para.SS_PARA_Y + port1 + port2
-                y_para_re = specifiers_ss_para.SS_PARA_Y + port1 + port2 + sub_specifiers.REAL
-                y_para_im = specifiers_ss_para.SS_PARA_Y + port1 + port2 + sub_specifiers.IMAG
+                y_para = specifiers_ss_para.SS_PARA_Y + [port1, port2]
+                y_para_re = specifiers_ss_para.SS_PARA_Y + [port1, port2] + sub_specifiers.REAL
+                y_para_im = specifiers_ss_para.SS_PARA_Y + [port1, port2] + sub_specifiers.IMAG
                 df_new[y_para] = df_new[y_para_re] + 1j * df_new[y_para_im]
                 df_new.drop(columns=[y_para_im, y_para_re])
 
         return df_new
 
     def iter_unique_col(self, column, decimals=5):
         """Allows iteration over the unique values and their slices of a column
@@ -2118,18 +2198,22 @@
         Parameters
         ----------
         column : :class:`DMT.core.SpecifierStr` or str
             Column name to iterate over
         decimals : int, optional
             Rounding precision for the unique, None to turn off, by default 5
 
-        Returns
-        -------
-        :class:`DMT.core.data_frame.IterUniqueRoundColumn`
-            Iterator over all unique values of this column
+        Yields
+        ------
+        int
+            Index of current iteration
+        float
+            Value of the uniqued column
+        :class:`DMT.core.Dataframe`
+            Slice of the dataframe with the unique value
 
         Examples
         --------
         We want to replace:
 
         >>> for vbc in np.unique(np.round(df[col_vbc], decimals=5)):
                 data = df[np.isclose(df[col_vbc], atol=1e-5)]
@@ -2137,86 +2221,26 @@
 
         with
 
         >>> for index, vbc, data in df.iter_unique_col(col_vbc, decimals=5):
                 ... # user action
 
         """
-        return IterUniqueRoundColumn(self, column, decimals=decimals)
-
-
-class IterUniqueRoundColumn(object):
-    """Iterator to iterate over rounded unique values of a column
-
-    Parameters
-    ----------
-    dataframe : :class:`DMT.core.Dataframe`
-        DMT (or parandas) dataframe with data including the column to iterate over.
-    column : :class:`DMT.core.SpecifierStr` or str
-        Column name to iterate over
-    decimals : int, optional
-        Rounding precision for the unique, None to turn off, by default 5
-
-    """
-
-    def __init__(self, dataframe, column, decimals=5):
-        self.index = 0  # start at 0
-        self.dataframe = dataframe
-        self.column = column
+        index = 0
 
         if decimals is None:
-            self.val_unique = np.unique(dataframe[column])
-            self.atol = None
+            val_unique = np.unique(self[column])
+            atol = None
         else:
-            self.val_unique = np.unique(np.round(dataframe[column], decimals=decimals))
-            self.atol = 5 * np.float_power(10, -(decimals + 1))
-
-    def __len__(self):
-        """Convenience to so len(iterator) can be used.
-
-        Returns
-        -------
-        int
-            Length of the uniqued values
-        """
-        return len(self.val_unique)
-
-    def __iter__(self):
-        """Here self is returned -> this class itself is an iterator.
-
-        Returns
-        -------
-        :class:`DMT.core.data_frame.IterUniqueRoundColumn`
-            Iterator over all unique values of this column
-        """
-        return self
-
-    def __next__(self):
-        """This routine is magic and sets the iteration behavior.
+            val_unique = np.unique(np.round(self[column], decimals=decimals))
+            atol = 5 * np.float_power(10, -(decimals + 1))
 
-        Returns
-        -------
-        int
-            Index of current iteration
-        float
-            Value of the uniqued column
-        :class:`DMT.core.Dataframe`
-            Slice of the dataframe with the value
+        while index < len(val_unique):
+            val = val_unique[index]
 
-        Raises
-        ------
-        StopIteration
-            As soon as all values are iterated
-        """
-        if self.index == len(self):
-            # end reached
-            raise StopIteration
-
-        val = self.val_unique[self.index]
-
-        if self.atol is None:
-            dataframe = self.dataframe[self.dataframe[self.column] == val]
-        else:
-            dataframe = self.dataframe[np.isclose(self.dataframe[self.column], val, atol=self.atol)]
+            if atol is None:
+                dataframe = self[self[column] == val]
+            else:
+                dataframe = self[np.isclose(self[column], val, atol=atol)]
 
-        self.index += 1
-        return self.index - 1, val, dataframe
+            yield index, val, dataframe
+            index += 1
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/data_processor.py` & `DMT_core-2.0.0/DMT/core/data_processor.py`

 * *Files 2% similar despite different names*

```diff
@@ -345,48 +345,47 @@
                 "DMT -> DataProcessor: You specified an n-port Conversion that is not implemented or makes no sense."
             )
 
         return para_new
 
     def y2a(self, y):
         """My own y2a routine since scikit rf does not have one. What a shame!"""
+        det_y = np.linalg.det(y)
         a = np.zeros(y.shape, dtype="complex")
-        for fidx in range(y.shape[0]):
-            det_y = np.linalg.det(y[fidx, :, :])
 
-            a[fidx, 0, 0] = -y[fidx, 1, 1] / y[fidx, 1, 0]
-            a[fidx, 0, 1] = -1.0 / y[fidx, 1, 0]
-            a[fidx, 1, 0] = -det_y / y[fidx, 1, 0]
-            a[fidx, 1, 1] = -y[fidx, 0, 0] / y[fidx, 1, 0]
+        a[:, 0, 0] = -y[:, 1, 1] / y[:, 1, 0]
+        a[:, 0, 1] = -1.0 / y[:, 1, 0]
+        a[:, 1, 0] = -det_y / y[:, 1, 0]
+        a[:, 1, 1] = -y[:, 0, 0] / y[:, 1, 0]
 
         return a
 
     def y2h(self, y):
         """My own y2h routine since scikit rf does not have one. What a shame!"""
         h = np.zeros(y.shape, dtype="complex")
-        for fidx in range(y.shape[0]):
-            det_y = np.linalg.det(y[fidx, :, :])
+        det_y = np.linalg.det(y)
+        inv_y_00 = 1.0 / y[:, 0, 0]
 
-            h[fidx, 0, 0] = 1
-            h[fidx, 1, 1] = det_y
-            h[fidx, 0, 1] = -y[fidx, 0, 1]
-            h[fidx, 1, 0] = y[fidx, 1, 0]
-            h[fidx, :, :] = h[fidx, :, :] / y[fidx, 0, 0]
+        h[:, 0, 0] = 1
+        h[:, 1, 1] = det_y
+        h[:, 0, 1] = -y[:, 0, 1]
+        h[:, 1, 0] = y[:, 1, 0]
+        h[:, :, :] = h[:, :, :] * inv_y_00[:, None, None]
 
         return h
 
     def a2y(self, a):
         """My own a2y routine since scikit rf does not have one. What a shame!"""
         y = np.zeros(a.shape, dtype="complex")
-        for fidx in range(a.shape[0]):
-            det_a = np.linalg.det(a[fidx, :, :])
-            y[fidx, 0, 0] = 1.0 / a[fidx, 0, 1] * a[fidx, 1, 1]
-            y[fidx, 1, 1] = 1.0 / a[fidx, 0, 1] * a[fidx, 0, 0]
-            y[fidx, 0, 1] = -1.0 / a[fidx, 0, 1] * det_a
-            y[fidx, 1, 0] = -1.0 / a[fidx, 0, 1]
+        inv_a_01 = 1.0 / a[:, 0, 1]
+        det_a = np.linalg.det(a)
+        y[:, 0, 0] = inv_a_01 * a[:, 1, 1]
+        y[:, 1, 1] = inv_a_01 * a[:, 0, 0]
+        y[:, 0, 1] = -inv_a_01 * det_a
+        y[:, 1, 0] = -inv_a_01
 
         return y
 
     def parallel_norm(self, s_para_values, ndevices):
         """Normalize the measured S parameters in s_para_values to the number of parallel devices.
 
         Parameters
@@ -626,15 +625,15 @@
 
     def calc_ft(self, freq, para_values, p_type):
         """Calculate the transit frequency F_T using the spot frequency method.
 
         Parameters
         ----------
         freq         :  np.ndarray()
-            Frequencys that correspond to para_values.
+            Frequencies that correspond to para_values.
         para_values  :  np.ndarray()
             Small signal parameters of type p_type with shape [n_freq, n_port, n_port]
         p_type       :  string
             Type of the small signal parameters in para_values.
 
         Returns
         -------
@@ -648,15 +647,15 @@
 
     def calc_tfit1(self, freq, para_values, p_type):
         """Calculate the transit frequency F_T using the spot frequency method.
 
         Parameters
         ----------
         freq         :  np.ndarray()
-            Frequencys that correspond to para_values.
+            Frequencies that correspond to para_values.
         para_values  :  np.ndarray()
             Small signal parameters of type p_type with shape [n_freq, n_port, n_port]
         p_type       :  string
             Type of the small signal parameters in para_values.
 
         Returns
         -------
@@ -672,15 +671,15 @@
 
     def calc_tfit2(self, freq, para_values, p_type):
         """Calculate the transit frequency F_T using the spot frequency method.
 
         Parameters
         ----------
         freq         :  np.ndarray()
-            Frequencys that correspond to para_values.
+            Frequencies that correspond to para_values.
         para_values  :  np.ndarray()
             Small signal parameters of type p_type with shape [n_freq, n_port, n_port]
         p_type       :  string
             Type of the small signal parameters in para_values.
 
         Returns
         -------
@@ -696,15 +695,15 @@
 
     def calc_fmax(self, freq, para_values, p_type):
         """Calculate the maximum frequency of oscillation from the unilateral gain.
 
         Parameters
         ----------
         freq         :  np.ndarray()
-            Frequencys that correspond to para_values.
+            Frequencies that correspond to para_values.
         para_values  :  np.ndarray()
             Small signal parameters of type p_type with shape [n_freq, n_port, n_port]
         p_type       :  string
             Type of the small signal parameters in para_values.
 
         Returns
         -------
@@ -721,15 +720,15 @@
     def calc_unilateral_gain(self, freq, para_values, p_type):
         """Calculates the unilateral gain `GU <https://www2.eecs.berkeley.edu/Pubs/TechRpts/2016/EECS-2016-15.pdf>`_ .
         | https://ieeexplore.ieee.org/stamp/stamp.jsp?arnumber=1083579
 
         Parameters
         ----------
         freq         :  np.ndarray()
-            Frequencys that correspond to para_values.
+            Frequencies that correspond to para_values.
         para_values  :  np.ndarray()
             Small signal parameters of type p_type with shape [n_freq, n_port, n_port]
         p_type       :  string
             Type of the small signal parameters in para_values.
 
         Returns
         -------
@@ -983,7 +982,28 @@
 
         else:
             raise NotImplementedError(
                 "DMT data_processor -> combination of arguments not yet implemented."
             )
 
         return np.where(gm <= 0.0, np.nan, gm)
+
+    def calc_go(self, ic, vce):
+        """Calculates the output conductance of a bjt or mosfet.
+
+        Parameters
+        ----------
+        ic  :  np.ndarray()
+            DC Collector current.
+        vc  :  np.ndarray()
+            c or d voltage
+
+        Returns
+        -------
+        go  :  np.ndarray()
+            The output conductance
+        """
+
+        go = np.zeros_like(ic)
+        go = np.gradient(ic, vce)
+
+        return np.where(go <= 0.0, np.nan, go)
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/data_reader.py` & `DMT_core-2.0.0/DMT/core/data_reader.py`

 * *Files 4% similar despite different names*

```diff
@@ -98,15 +98,15 @@
     elif extension == ".p":
         with filename.open("rb") as pickle_file:
             df = pickle.load(pickle_file)
     elif extension == ".h5":
         if key is None:
             key = "/df"
         df = read_hdf(filename, key)
-    elif extension == ".feather":
+    elif extension in [".feather", ".fth"]:
         df = read_feather(filename)
     else:
         raise IOError(
             "Error: DMT can not open file "
             + filename
             + " since extension "
             + extension
@@ -156,19 +156,16 @@
         DMT DataFrame that stores the mdm data.
     """
     return pd.read_hdf(str(filename), key=key)
 
 
 def read_mdm_blocks(block, n_row, n_col, n_iccap_vars, iccap_vars):
     data_raw = np.zeros([n_row, n_col + n_iccap_vars], dtype=np.float64)
-    # read in raw data
-    for i in range(n_row):
-        data_raw[i, :n_col] = block[n_col * i : n_col * (i + 1)]
-        data_raw[i, n_col : n_col + n_iccap_vars] = iccap_vars
-
+    data_raw[:, :n_col] = block.reshape(n_row, n_col)
+    data_raw[:, n_col : n_col + n_iccap_vars] = iccap_vars
     return data_raw
 
 
 def read_mdm(filename):
     """Read .mdm file and generate a DMT dataframe from it.
 
     Parameters
@@ -226,19 +223,14 @@
         data_raw = read_mdm_blocks(
             block,
             n_row,
             n_col,
             n_iccap_vars,
             np.array([value for key, value in iccap_vars.items()]),
         )
-        # read in raw data
-        # data_raw      =  np.zeros([n_row, n_col + n_iccap_vars ])
-        # for i in range(n_row):
-        #     data_raw[i,       :n_col             ]  =  block[ n_col*i : n_col*(i+1) ]
-        #     data_raw[i,  n_col:n_col+n_iccap_vars]  =  [value  for key,value in iccap_vars.items()]
 
         cols.extend([key for key, value in iccap_vars.items()])
         block_data.append(data_raw)
 
     if block_data:
         all_data = np.concatenate(block_data)
         df = DataFrame(all_data, columns=cols)
@@ -302,17 +294,15 @@
                 filename, n_row
             )
         )
 
     n_row = int(n_row)  # but force it anyways!
 
     # fill the data into the 2-dimensional array data_raw
-    data_raw = np.empty([n_row, n_col])
-    for i in range(n_row):
-        data_raw[i, :] = list_lines[n_col * i : n_col * (i + 1)]
+    data_raw = np.array(list_lines).reshape(n_row, n_col)
 
     # initalize pd.Dataframe() and return it
     return DataFrame(data_raw, columns=columns)
 
 
 def read_csv(filename, **kwargs):
     """Read .csv file and generate a DMT dataframe from it.
@@ -509,15 +499,16 @@
                 )
 
             df[col_name] = read_vals
             i_record = i_record + 1
 
     # check if pseudo 2D simulation
     if "y" in df.columns:
-        if all((df["y"] == 0.0) | (df["y"] == df["y"].to_numpy()[-1])):
+        # if all((df["y"] == 0.0) | (df["y"] == df["y"].to_numpy()[-1])):
+        if len(df["y"].unique()) == 2:
             # all 'y' are either 0.0 or 1.0 -> 1D simulation: cut off the df
             df = df[df["y"] == 0.0]
             del df["y"]
 
     return df
 
 
@@ -668,15 +659,14 @@
                 sim["data"] = data.transpose()
                 # prepare for next iteration
                 # old_line = line
                 # print('b: ' + str(line))
                 line = line[offset:]
 
         elif str_format == "Flags: complex":
-
             data = np.zeros((num_var, num_points), dtype=np.complex128)
             offset = 0
 
             # fortran order, 1h of bugfix Oo
             for ndi_data in np.nditer(data, order="F", op_flags=["writeonly"]):
                 while len(line) < offset + 16:
                     line = line + bin_content.pop()
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/database_manager.py` & `DMT_core-2.0.0/DMT/core/database_manager.py`

 * *Files 19% similar despite different names*

```diff
@@ -27,19 +27,20 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 import pandas as pd
 import warnings
 import _pickle as cpickle
 from pathlib import Path
+from pyarrow.lib import ArrowInvalid
 
 from DMT.config import DATA_CONFIG
 from DMT.core.data_frame import DataFrame
 from DMT.core.singleton import Singleton
-from DMT.core.naming import SpecifierStr
+from DMT.core.naming import SpecifierStr, get_specifier_from_string
 
 
 class DatabaseManager(object, metaclass=Singleton):
     """Class responsible for data management in DMT.
 
     Methods
     -------
@@ -101,15 +102,15 @@
                     for col in df.columns:
                         dict_reconvert[col] = SpecifierStr.string_from_load(col)
 
                     df.rename(columns=dict_reconvert, inplace=True)
                     # prevent invisible column bug:
                     df = df.loc[:, ~df.columns.duplicated()]
                     if not df.columns.is_unique:
-                        raise IOError
+                        raise IOError()
 
                     data[key] = df
                 db.close()
             except (OSError, RuntimeError):
                 with db_dir.open(mode="rb") as my_db:
                     data = cpickle.load(my_db)
 
@@ -172,41 +173,36 @@
                         pass
                 df = df.rename(columns=dict_convert)
 
                 with warnings.catch_warnings():
                     warnings.simplefilter("ignore")
                     db.put(key, df)
 
-                # cast back
-                # for col in df.columns:
-                #     df = df.rename(columns={SpecifierStr.string_from_load(col):col})
-
                 df = df.rename(columns=dict_reconvert)
             db.close()
         else:
             with db_dir.open(mode="wb") as my_db:
                 cpickle.dump(data, my_db)
 
         # convert back
         for key, df in data.items():
             df.__class__ = DataFrame
 
     def del_db(self, db_dir):
-        """Delete the .h5 database for dut.
+        """Delete the database file for a dut.
 
         Parameters
         ----------
         db_dir   :  string or os.Pathlike
             Full path to the database.
         """
         if not isinstance(db_dir, Path):
             db_dir = Path(db_dir)
 
-        if db_dir.exists():
-            db_dir.unlink()
+        db_dir.unlink(missing_ok=True)
 
     def save_df(self, df, file_name):
         """Save the data stored in df as file_name, where file_name is the direct path to the file.
 
         Parameters
         ----------
         df  :  DMT.core.DataFrame
@@ -215,25 +211,56 @@
             Direct path to the file
         """
         if not isinstance(file_name, Path):
             file_name = Path(file_name)
 
         file_name.parent.mkdir(parents=True, exist_ok=True)
 
-        df.to_pickle(str(file_name))
+        dict_convert = {}
+        for col in df.columns:
+            try:
+                dict_convert[col] = col.string_to_save()
+            except AttributeError:
+                pass
+        df_save = df.rename(columns=dict_convert, inplace=False)
+        df_save.to_feather(str(file_name), version=2, compression="lz4")
 
-    def load_df(self, file_name):
+    def load_df(self, file_name, to_specifier=True):
         """Load the data stored in file_name, where file_name is the direct path to the file.
 
         Parameters
         ----------
         file_name  :  str
             Direct path to the file
+        to_specifier : bool
+            If True, the column names are cast to specifiers. Only neeeded for feather files. Default is True.
 
         Returns
         -------
         df  :  DMT.core.DataFrame
             Loaded dataframe object.
         """
-        df = pd.read_pickle(str(file_name))
-        df.__class__ = DataFrame
+        try:
+            df = pd.read_feather(str(file_name))
+            df.__class__ = DataFrame
+
+            if to_specifier:
+                # here we should cast
+                dict_reconvert = {}
+                for col in df.columns:
+                    specifier = SpecifierStr.string_from_load(col)
+                    if not isinstance(specifier, SpecifierStr):
+                        # did not work so try default cast
+                        specifier = get_specifier_from_string(col)
+
+                    dict_reconvert[col] = specifier
+
+                df.rename(columns=dict_reconvert, inplace=True)
+                # prevent invisible column bug:
+                df = df.loc[:, ~df.columns.duplicated()]
+                if not df.columns.is_unique:
+                    raise IOError()
+
+        except ArrowInvalid:
+            df = pd.read_pickle(str(file_name))
+            df.__class__ = DataFrame
         return df
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/df_to_sweep.py` & `DMT_core-2.0.0/DMT/core/df_to_sweep.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         if len(np.unique(np.round(df_to_convert[potential].to_numpy(), decimals_potentials))) == 1:
             potential_common = potential  # use this one! Even if more than one would exist.
             break
 
     if not potential_common:  # no potential found
         # did not find anything :(
         raise IOError(
-            "DMT -> df_to_sweep: The user supplied voltages do not define unambiguous sweep conditions for the transistor. No common reference potential was found."
+            "DMT->df_to_sweep: The user supplied voltages do not define unambiguous sweep conditions for the transistor. No common reference potential was found."
         )
 
     def_sweep = [
         {"var_name": potential_common, "sweep_order": 0, "sweep_type": "CON", "value_def": [0]},
     ]  # 0 because the other Sweepdefs are added as voltages.
     sweep_order = 1
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/docu_dut_lib.py` & `DMT_core-2.0.0/DMT/core/docu_dut_lib.py`

 * *Files 0% similar despite different names*

```diff
@@ -311,15 +311,17 @@
                             if not val in dut_property:
                                 ok = False
                         elif isinstance(val, float):
                             dut_property = getattr(dut, device_spec)
                             try:
                                 if not np.isclose(dut_property, val):
                                     ok = False
-                            except ValueError:  # tetrodes will not work like this (tuple dut_property)
+                            except (
+                                ValueError
+                            ):  # tetrodes will not work like this (tuple dut_property)
                                 pass
 
                     if ok:
                         print("Found device " + dut.name + ".")
                         self.duts.append(dut)
 
         if not self.duts:
@@ -518,15 +520,14 @@
                 # find temperatures
                 temps = []
                 for key in dut.data.keys():
                     temps.append(dut.get_key_temperature(key))
                 temps = list(set(temps))
 
                 for temp in temps:
-
                     y_scale = 1
                     x_label = None  # autolabel
                     y_label = None
                     if (
                         quantity_y.specifier in specifiers.SS_PARA_Y
                     ):  # special cases that I do not want in DMT
                         y_scale = 1e3 / (1e6 * 1e6)  # mS/um^2
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/dut_circuit.py` & `DMT_core-2.0.0/DMT/core/dut_tcad.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,10 @@
-""" Provdes a class for cirtuit DuTs
-
-Provides a interface superclass. Here all methods which must be implemented by all circuit simulator interfaces are collected.
-
-A DuT can be supplied using the input_circuit parameter. This parameter can be:
-
-* :class:`~DMT.core.circuit.Circuit`
-* String with path to a netlist of a circuit
-* String with the netlist of a circuit
-* List with paths to netlists or strings with netlists, these will be combined into the netlist to simulate.
+""" Provdes a class for TCAD DuTs
 
+Provides a interface superclass. Here all methods which must be implemented by all TCAD interfaces are collected.
 
 Author: Mario Krattenmacher | Mario.Krattenmacher@semimod.de
 """
 # DMT_core
 # Copyright (C) from 2022  SemiMod
 # Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
 # <https://gitlab.com/dmt-development/dmt-core>
@@ -28,194 +20,202 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 import copy
-from collections import OrderedDict
-from DMT.core import create_md5_hash, DutView, McParameterCollection, DutType
-from DMT.core.mcard import MCard
+import logging
+from typing import List, Dict
+from DMT.core import create_md5_hash, DutView, Technology
 
+try:
+    from semver.version import Version as VersionInfo
+except ImportError:
+    from semver import VersionInfo
 
-class DutCircuit(DutView):
-    """Superclass for common methods and attributes of cirtuit DuTs
+SEMVER_DUTTCAD_CURRENT = VersionInfo(major=1, minor=0)
 
-    Makes a circuit simulator like ADS or XYCE useable by DMT
+
+class DutTcad(DutView):
+    """Superclass for common methods and attributes of TCAD DuTs
+
+    Makes a TCAD simulator like DEVICE or Hdev useable by DMT
 
     Parameters
     ----------
     database_dir    : string
         This is the directory were the DUT will create its database.
-    name      :  string
+    name      : string
         Prefix for the database
     dut_type   : :class:`~DMT.core.dut_type.DutType`
         Type of the DUT.
     nodes     : string
         Strings with comma separated node names of DUT. If nodes is None, nodes will be requested from Dut_type class.
-    inp_header : str, list[str] or :class:`~DMT.classes.circuit.Circuit`
-        Depending of the used simulator, here different options are possible.
-    simulator_options : OrderedDict
-
+    inp_structure : str or InpTcad
+        One of 3 different possibilities: special obj for create_inp_header(), string with path to file or direct input file string
+    simulator_command : str
+        Command to start the correct TCAD simulator
+    simulator_arguments : list[str]
+        List of arguments for the simulator command, will be added one by one before the input file.
 
     Attributes
     ----------
     sim_command : str
-        Command to start the correct circuit simulator
+        Command to start the correct TCAD simulator
     sim_args : list[str]
         List of arguments for the simulator command, will be added one by one before the input file.
+
+    Methods
+    -------
+    inp_header(value)
+        Returns input header of a simulation input file, or sets it to a new value, removing attached files.
+    inp_structure(value)
+        Returns input structure for DUT, or sets it while automatically creating a new header.
+    get_hash()
+        Returns hash if inp_header is set.
+    get_start_sim_command()
+        Returns command to start a specific type of simulation (DEVICE, Hdev, ...).
+    run_sim(sweep)
+        Starts a simulation.
+    create_inp_header(inp_structure)
+        Creates an inp_header for a given inp_structure. Has to be set by inheriting class.
+    set_param()
+        Enables setting model parameters for a simulation. Has to be set by in heriting class.
+    get_param()
+        Enables getting model parameters for a simulation. Has to be set by in heriting class.
     """
 
-    def __init__(
-        self,
-        database_dir: str,
-        name: str,
-        dut_type: DutType,
-        inp_circuit,
-        simulator_options: dict = None,
-        get_circuit_arguments: dict = None,
-        **kwargs
-    ):
-        self._inp_header = ""
+    def __init__(self, database_dir, name, dut_type, inp_structure, **kwargs):
+        # use the property setter method to analyze inp_structure.
+        self._inp_header = None
+        self._inp_structure = None
 
         super().__init__(database_dir, name, dut_type, **kwargs)
 
-        if simulator_options is None:
-            self.simulator_options = OrderedDict()
-        else:
-            self.simulator_options = OrderedDict(sorted(simulator_options.items()))
-
-        if get_circuit_arguments is None:
-            self.get_circuit_arguments = OrderedDict()
-        else:
-            self.get_circuit_arguments = OrderedDict(sorted(get_circuit_arguments.items()))
-
-        # save for later use
-        self._inp_circuit = None
-        self._modelcard = None
-        self.inp_header = inp_circuit
+        # set the input structure to the input header property and let it handle it.
+        self.inp_header = inp_structure
 
     @property
     def inp_header(self):
         """Getter method for the input header of the simulation input file"""
         return self._inp_header
 
     @inp_header.setter
     def inp_header(self, value):
-        """Setter method for the input header. This removes any stored data from the object, as it is not valid anymore! Automatically calls create_inp_header, if it is not a string or a list of strings.
+        """Setter method for the input header. This removes any stored data from the object, as it is not valid anymore!
+        Automatically recalls create_inp_header, if it is not a string.
 
         Parameters
         ----------
-        value : str, list[string] or valid for create_inp_header
+        value : str or anything fitting for overwritten create_inp_header
         """
-        value = copy.deepcopy(value)
-        self._inp_circuit = None  # is set in create_inp_header
-        self._data = {}  # empty the data dict!
+        self._data = {}
+        self._inp_structure = None
+
         if isinstance(value, str):
             try:
                 with open(value, "r") as inp_file:
                     self._inp_header = inp_file.read()
             except IOError:
-                # could not open input file. Assume it is already a netlist
+                # could not open input file. Assume it is the already read string
                 self._inp_header = value
-        elif isinstance(value, (list, tuple)):
-            # list of files and/or netlist strings. They are all joined into one input header.
-            inp_header = ""
-            for netlist in value:
-                try:
-                    with open(netlist, "r") as inp_file:
-                        inp_header = inp_header + "\n" + inp_file.read()
-                except IOError:
-                    # could not open input file. Assume it is already a netlist
-                    inp_header = inp_header + "\n" + netlist
-
-            self._inp_header = inp_header
         else:
+            self._inp_structure = copy.deepcopy(value)
             self._inp_header = self.create_inp_header(value)
 
-    @property
-    def modelcard(self):
-        """Returns the saved modelcard"""
-        return self._modelcard
-
-    @modelcard.setter
-    def modelcard(self, modelcard):
-        """Forces a new inp_header!
+        logging.info(
+            "Successfully created input header of dut %s%s!", self.name, str(self.get_hash())
+        )
+        logging.debug("Content:\n%s", self._inp_header)
+
+    def info_json(self, **_kwargs) -> Dict:
+        """Returns a dict with serializeable content for the json file to create.
+
+        The topmost dict MUST have only one key: The string casted class name.
+        Inside the parameters are:
+
+            * A version key,
+            * all extra parameters of DutTcad compared to DutView and
+            * the info_json of DutView.
+
+        Returns
+        -------
+        dict
+            str(DutTcad): serialized content
+        """
+        return {
+            "__DutTcad__": str(SEMVER_DUTTCAD_CURRENT),
+            "parent": super(DutTcad, self).info_json(**_kwargs),
+            "inp_header": self.inp_header,
+        }
+
+    @classmethod
+    def from_json(
+        cls,
+        json_content: Dict,
+        classes_technology: List[type[Technology]],
+        subclass_kwargs: Dict = None,
+    ) -> "DutTcad":
+        """Static class method. Loads a DutTcad object from a pickle file with full path save_dir.
+
+        Calls the from_json method of DutView with all dictionary inside the "parent" keyword. Afterwards the additional parameters are set correctly.
 
         Parameters
         ----------
-        modelcard : MCard
+        json_content  :  dict
+            Readed dictionary from a saved json DutTcad.
+        classes_technology : List[type[Technology]]
+            All possible technologies this loaded DutTcad can have. One will be choosen according to the serialized technology loaded from the file.
+        subclass_kwargs : Dict, optional
+            Additional kwargs necessary to create the concrete subclassed DutView.
+
+        Returns
+        -------
+        DutTcad
+            Loaded object.
         """
-        if isinstance(modelcard, MCard) or isinstance(modelcard, McParameterCollection):
-            self._modelcard = modelcard
-            self.inp_header = modelcard
-        else:
-            raise OSError("The modelcard has to be a instance of MCard or its children!")
+        if json_content["__DutTcad__"] != SEMVER_DUTTCAD_CURRENT:
+            raise NotImplementedError("DMT.DutTcad: Unknown version of DutTcad to load!")
+
+        if subclass_kwargs is None:
+            subclass_kwargs = {}
+        subclass_kwargs["inp_structure"] = json_content["inp_header"]
+
+        dut_view = super().from_json(
+            json_content["parent"], classes_technology, subclass_kwargs=subclass_kwargs
+        )
+
+        return dut_view
 
     def get_hash(self):
         """Returns a md5 hash generated from self.inp_header, if it is not set, this will return False!
 
-        Is overwritten here, to include the imported and appended files!
+        In case a InpStructure is set, this always recreates the inp_header :/.
 
         Returns
         -------
         str or False
-
-        Notes
-        -----
-        Also account for dut.name?
         """
         if self.inp_header is None:
             return False
 
-        if self._list_va_file_contents:
-            list_va = [
-                vafile.get_tree_hash() for vafile in self._list_va_file_contents
-            ]  # directly use the hash here - hash of hash should be ok :)
-        else:
-            list_va = []
-        return create_md5_hash(self.inp_header, *self.list_copy, *list_va)
+        # i have to ensure always correct hash for a dut... sorry
+        if self._inp_structure is not None:
+            self._inp_header = self.create_inp_header(self._inp_structure)
 
-    def create_inp_header(self, inp_circuit):
-        """Creates the inp_header from the given circuit.
+        return create_md5_hash(self._inp_header + self.sim_command)
 
-        Parameters
-        ----------
-        inp_circuit
-            Type and content depends on implementation of inheriting class!
-
-        Returns
-        -------
-        str
-            input header
-        """
-        raise NotImplementedError("create_inp_file() must be implemented in inheriting class!")
-
-    def _convert_CircuitElement_netlist(self, circuit_element):
-        """Transforms a :class:`~DMT.classes.circuit.CircuitElement` into a string fitting for the inheriting DutCircuit.
+    def create_inp_header(self, inp_structure):
+        """Creates the inp_header from the given parameter object.
 
         Parameters
         ----------
-        circuit_element
-            CircuitElement to transform
+        inp_structure
+            Type and content depends on implementation of inheriting class!
 
         Returns
         -------
         str
-            Netlist line
+            Input circuit
         """
-        raise NotImplementedError(
-            "_convert_CircuitElement_netlist() must be implemented in inheriting class!"
-        )
-
-    def scale_modelcard(self):
-        """Scales the given modelcard to the actual size of the dut."""
-        if self.technology is None or not hasattr(self.technology, "scale_modelcard"):
-            self.modelcard = self.modelcard
-        else:
-            self.modelcard = self.technology.scale_modelcard(
-                self.modelcard,
-                self.length,
-                self.width,
-                self.nfinger,
-                self.contact_config,
-            )
+        raise NotImplementedError("create_inp_header() must be implemented in inheriting class!")
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/dut_dummy.py` & `DMT_core-2.0.0/DMT/core/dut_dummy.py`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/core/dut_lib.py` & `DMT_core-2.0.0/DMT/core/dut_lib.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,25 +20,34 @@
 import os
 import _pickle as cpickle
 import shutil
 import copy
 import re
 import filecmp
 import numpy as np
+import json
 from pathlib import Path
 from joblib import Parallel, delayed
-from DMT.core import DutType, print_progress_bar, DutView
+from typing import List
+from DMT.core import DutType, DutTypeFlag, print_progress_bar, DutView, Technology
 from DMT.exceptions import NoOpenDeembeddingDut, NoShortDeembeddingDut
 
 try:
+    from semver.version import Version as VersionInfo
+except ImportError:
+    from semver import VersionInfo
+
+try:
     from pylatex import Section, Subsection, SmallText, Tabular, NoEscape, Center
     from DMT.external.pylatex import Tex
 except ImportError:
     pass
 
+SEMVER_DUTLIB_CURRENT = VersionInfo(major=1, minor=0)
+
 
 class __Filter(object):
     """Superclass for all implemented filters. Is used to compare specified properties of devices and deembedding structures.
 
     Parameters
     ----------
     devProp     : 'str'
@@ -212,17 +221,17 @@
 
         self.AC_filter_names = AC_filter_names
         self.DC_filter_names = DC_filter_names
         self.is_deembedded_AC = is_deembedded_AC
         self.is_deembedded_DC = is_deembedded_DC
 
         self.deem_open = (
-            DutType.flag_open
+            DutTypeFlag.flag_open
         )  # deem_open_bjt # look only for the flag not for the device!
-        self.deem_short = DutType.flag_short  # deem_short_bjt
+        self.deem_short = DutTypeFlag.flag_short  # deem_short_bjt
 
         self.duts = []  # The devices that shall be managed by this dut
         self._dut_ref = None  # The reference device of this technology
         self.dut_ref_dut_dir = None
         self._dut_intrinsic = None  # The intrinsic dut of the reference dut (without rbi)
         self.dut_intrinsic_dut_dir = None  # The intrinsic dut of the reference dut (without rbi)
         self._dut_internal = None  # The internal dut of the reference dut (with rbi)
@@ -299,18 +308,22 @@
         """Just return save dir"""
         return self._save_dir
 
     @save_dir.setter
     def save_dir(self, path):
         """Ensures an empty folder for the DutLib"""
         path = Path(path).resolve()
-        if (path / "dut_lib.p").is_file():
+        if (path / "dut_lib.json").is_file():
             raise FileExistsError(
                 "The path you chose is already used by an other library! Either delete the already existing library or load it."
             )
+        if (path / "dut_lib.p").is_file():
+            raise FileExistsError(
+                "The path you chose is already used by an older library! Either delete the already existing library or load it."
+            )
 
         self._save_dir = path
 
     def find_devices(self, devtype):
         """Searches the list of duts read in from the specified folder previously for the specified dut_type and adds all identified devices to a new list.
 
         Parameters
@@ -445,33 +458,41 @@
             if duts.name in [dut_a.name for dut_a in self.duts]:
                 raise IOError(
                     "DutLib: A DuT of this name already exists. Dut names must be unique!"
                 )
             self.duts.append(duts)
 
     def save(self):
-        """Save the DutLib to save_dir."""
+        """Save the DutLib to save_dir.
+
+        The DutLib will be saved as a json file and in the folder "duts" there will be the DutViews.
+        It will save all the DutViews including the ignored ones.
+
+        """
         assert self.save_dir is not None
 
-        if not os.path.isabs(self.save_dir):
-            self._save_dir = os.path.abspath(self.save_dir)
+        if not self.save_dir.is_absolute():
+            self._save_dir = self.save_dir.absolute()
 
-        if not os.path.exists(self.save_dir):
-            os.makedirs(self.save_dir)
+        self.save_dir.mkdir(parents=True, exist_ok=True)
 
         ignore_duts = copy.deepcopy(self.ignore_duts)
         self.ignore_duts = []  # save all duts, even the one who were ignored
         for dut in self.duts:
-            if dut.database_dir != os.path.join(self.save_dir, "duts"):
+            if dut.database_dir != self.save_dir / "duts":
                 try:  # if enough data available, sort by wafer and dies
-                    directory = os.path.join(
-                        self.save_dir, "duts", "wafer_" + str(dut.wafer), "die_" + str(dut.die)
+                    directory = (
+                        self.save_dir
+                        / "duts"
+                        / ("wafer_" + str(dut.wafer))
+                        / ("die_" + str(dut.die))
                     )
+
                 except:
-                    directory = os.path.join(self.save_dir, "duts")
+                    directory = self.save_dir / "duts"
                 dut.database_dir = directory
 
             dut.save()
 
         if self._dut_ref is not None:
             path_abs = Path(self.dut_ref.dut_dir).resolve()
             if filecmp.cmp(path_abs, self.dut_ref.dut_dir):
@@ -496,53 +517,129 @@
                 self.dut_intrinsic_dut_dir = path_abs
             else:
                 raise IOError(
                     "DMT->DutLib->Save: I can not convert the relative dut path of dut_intrinsic into an absolute path!"
                 )
 
         self.ignore_duts = ignore_duts  # but save the list ignore
-        with open(os.path.join(self.save_dir, "dut_lib.p"), "wb") as handle:
-            cpickle.dump(self, handle)
+
+        dict_content = {
+            "deem_types": [deem_type.serialize() for deem_type in self.deem_types],
+            "AC_filter_names": self.AC_filter_names,
+            "DC_filter_names": self.DC_filter_names,
+            "is_deembedded_AC": self.is_deembedded_AC,
+            "is_deembedded_DC": self.is_deembedded_DC,
+            "deem_open": self.deem_open.serialize(),
+            "deem_short": self.deem_short.serialize(),
+            # self.duts = []  # the Duts will be loaded from the saved files not by saving the list here.
+            "dut_ref_dut_dir": str(self.dut_ref_dut_dir),
+            "dut_intrinsic_dut_dir": str(self.dut_intrinsic_dut_dir),
+            "dut_internal_dut_dir": str(self.dut_internal_dut_dir),
+            "ignore_duts": "["
+            + ",".join(dut_name for dut_name in self.ignore_duts)
+            + "]",  # list of names which are not returned while iteration
+            "n_jobs": self.n_jobs,
+            "wafer": self.wafer,
+            "date_tapeout": self.date_tapeout,
+            "date_received": self.date_received,
+            "__DutLib__": str(
+                SEMVER_DUTLIB_CURRENT
+            ),  # make versions, so we can introduce compatibility here!}
+        }
+
+        file_path = self.save_dir / "dut_lib.json"
+        file_path.write_text(json.dumps(dict_content, indent=4), encoding="utf8")
 
     @staticmethod
-    def load(lib_directory):
-        """Static class method. Loads a DutLib object from a pickle file with full path lib_directory.
+    def load(
+        lib_directory,
+        classes_technology: List[type[Technology]] = None,
+        classes_dut_view: List[type["DutView"]] = None,
+    ) -> "DutLib":
+        """Static class method. Loads a DutLib object from a pickle or json file with full path lib_directory.
 
         Parameters
         ----------
         lib_directory  :  str or os.Pathlike
             Path to the direcotry that contains a pickled DutLib object that shall be loaded.
+        classes_technology : List[type[Technology]]
+            All possible technologies this loaded DutView can have. One will be choosen according to the serialized technology loaded from the file.
+        classes_dut_view : List[type[DutView]]
+            All possible DutViews this loaded DutView can be. One will be choosen according to the serialized dutview class name loaded from the file.
+
+
 
         Returns
         -------
-        obj  :  DutLib()
-            Loaded object from the pickle file.
+        DutLib
+            Loaded object from the json or pickle file.
         """
         # pylint: disable=unused-variable
         lib_directory = Path(lib_directory).resolve()
-        with (lib_directory / "dut_lib.p").open(mode="rb") as handle:
-            dut_lib = cpickle.load(handle)
-            dut_lib._save_dir = Path(dut_lib.save_dir)  # pylint: disable=protected-access
+        if (lib_directory / "dut_lib.json").exists():
+            with (lib_directory / "dut_lib.json").open("r", encoding="utf8") as file_json:
+                json_content = json.load(file_json)
+            if not json_content["__DutLib__"] == SEMVER_DUTLIB_CURRENT:
+                raise IOError("DMT.DutLib: Tried to load a DutLib with unkown version.")
+
+            deem_types = [
+                DutType.deserialize(deem_type) for deem_type in json_content["deem_types"]
+            ]
+            dut_lib = DutLib(
+                deem_types=deem_types,
+                AC_filter_names=json_content["AC_filter_names"],
+                DC_filter_names=json_content["DC_filter_names"],
+                is_deembedded_DC=json_content["is_deembedded_DC"],
+                is_deembedded_AC=json_content["is_deembedded_AC"],
+                n_jobs=json_content["n_jobs"],
+            )
+
+            dut_lib.deem_short = DutType.deserialize(json_content["deem_short"])
+            dut_lib.deem_open = DutType.deserialize(json_content["deem_open"])
+
+            dut_lib.dut_ref_dut_dir = json_content["dut_ref_dut_dir"]
+            dut_lib.dut_intrinsic_dut_dir = json_content["dut_intrinsic_dut_dir"]
+            dut_lib.dut_internal_dut_dir = json_content["dut_internal_dut_dir"]
+
+            dut_lib.ignore_duts = json_content["ignore_duts"]
+            dut_lib.wafer = json_content["wafer"]
+            dut_lib.date_tapeout = json_content["date_tapeout"]
+            dut_lib.date_received = json_content["date_received"]
+
+        elif (lib_directory / "dut_lib.p").exists():
+            with (lib_directory / "dut_lib.p").open(mode="rb") as handle:
+                dut_lib = cpickle.load(handle)
+                dut_lib._save_dir = Path(dut_lib.save_dir)  # pylint: disable=protected-access
+        else:
+            raise IOError(
+                "DMT.DutLib: Loading failed since no DutLib file was found (supported are json and pickle)."
+            )
 
         save_dir_old = ""
         # need to cast paths? This is needed when the machine is changed -> new absolute paths...
         if (
             lib_directory != dut_lib.save_dir
         ):  # dut_lib.save_dir is the old absolute path of the lib
             save_dir_old = str(dut_lib.save_dir)
             # write to internal value to avoid consistency check
             dut_lib._save_dir = lib_directory  # pylint: disable=protected-access
 
         # load all duts
         ignore_duts = copy.deepcopy(dut_lib.ignore_duts)
         dut_lib.ignore_duts = []  # load all duts, even the one who were ignored
-        for dir_name, dir_list, file_list in os.walk(dut_lib.save_dir / "duts"):  # find the duts
-            for file_dut in file_list:
-                if file_dut.endswith(".p"):
-                    dut_lib.duts.append(DutView.load_dut(os.path.join(dir_name, file_dut)))
+        # for dir_name, dir_list, file_list in os.walk(dut_lib.save_dir / "duts"):  # find the duts
+        #     for file_dut in file_list:
+        #         if file_dut.endswith(".json") or file_dut.endswith(".p"):
+        #             dut_lib.duts.append(DutView.load_dut(os.path.join(dir_name, file_dut)))
+        for file_dut in (dut_lib.save_dir / "duts").glob("**/*.json"):
+            dut_lib.duts.append(
+                DutView.load_dut(file_dut, classes_technology, classes_dut_view=classes_dut_view)
+            )
+        for file_dut in (dut_lib.save_dir / "duts").glob("**/*.p"):
+            dut_lib.duts.append(DutView.load_dut(file_dut))
 
         # correct dut paths:
         if dut_lib.dut_ref_dut_dir is not None:
             dut_lib.dut_ref_dut_dir = Path(dut_lib.dut_ref_dut_dir)
             if not dut_lib.dut_ref_dut_dir.exists():
                 dut_lib.dut_ref_dut_dir = Path(
                     str(dut_lib.dut_ref_dut_dir).replace(save_dir_old, str(lib_directory))
@@ -926,20 +1023,20 @@
 
         # Go through all available filters and find dfs matching their values
         for key in dut.data.keys():
             requires_deemb = False
             deembedded = False
 
             # first find out, if any filter applies here. if yes, likely this data needs deembedding
-            for (meas_filter, deem_filter) in self.AC_filter_names:
+            for meas_filter, deem_filter in self.AC_filter_names:
                 if re.search(meas_filter, key, re.IGNORECASE):
                     requires_deemb = True
                     break
 
-            for (meas_filter, deem_filter) in self.AC_filter_names:
+            for meas_filter, deem_filter in self.AC_filter_names:
                 # check if df needs to be AC deembedded & find O&S structure
                 if re.search(meas_filter, key, re.IGNORECASE):
                     short_keys = []
                     open_keys = []
 
                     # find all possible opens
                     for open_key in dut_open.data.keys():
@@ -956,15 +1053,15 @@
                     # if only one suitable short or open has been found we just take it
                     if len(short_keys) == 1 and len(open_keys) == 1:
                         df_open = dut_open.data[open_keys[0]]
                         df_short = dut_short.data[short_keys[0]]
                         dut.data[key] = dut.data[key].deembed(
                             df_open,
                             df_short,
-                            ports=dut.nodes,
+                            ports=dut.ac_ports,
                             ndevices=dut.ndevices,
                             ndevices_open=dut_open.ndevices,
                             ndevices_short=dut_short.ndevices,
                         )
                         # we get the number of deembedded dirty...
                         # times = dut.ndevices/dut_open.ndevices # not implemented anymore
                         times = 1
@@ -984,15 +1081,15 @@
 
                         df_open = dut_open.data[open_key]
                         df_short = dut_short.data[short_key]
                         try:
                             dut.data[key] = dut.data[key].deembed(
                                 df_open,
                                 df_short,
-                                ports=dut.nodes,
+                                ports=dut.ac_ports,
                                 ndevices=dut.ndevices,
                                 ndevices_open=dut_open.ndevices,
                                 ndevices_short=dut_short.ndevices,
                             )
                         except ValueError as err:
                             raise IOError(
                                 "The dataframes with keys "
@@ -1122,15 +1219,15 @@
                 print(key)
                 dut.data[key] = dut.data[key].deembed_DC(
                     mres=mres_tref, forced_current=forced_current
                 )
         else:
             mres_tref = None
 
-            for (meas_filter, deem_filter) in self.DC_filter_names:
+            for meas_filter, deem_filter in self.DC_filter_names:
                 # get the short keys
                 short_keys = []
                 for short_key in dut_short.data.keys():
                     if re.search(deem_filter, short_key, re.IGNORECASE):
                         short_keys.append(short_key)
 
                 if len(short_keys) == 1:
@@ -1141,15 +1238,14 @@
                         mres_tref = df_short.determine_mres(forced_current=forced_current)
                     else:
                         mres_tref = function_df(dut_short)
 
                 for key in dut.data.keys():
                     # check if df needs to be DC deembedded
                     if re.search(meas_filter, key, re.IGNORECASE):
-
                         if len(short_keys) == 1:
                             mres = mres_tref
                         else:  # NOT TESTED!!!!
                             # bad news...try to find matching temperatures. #TODO: Does not work if no keys are found
                             key_temperature = dut.get_key_temperature(key)
                             for short_key in short_keys:
                                 if np.isclose(
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/dut_meas.py` & `DMT_core-2.0.0/DMT/core/dut_meas.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,18 +19,27 @@
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 
 import logging
 import re
-from DMT.core import print_progress_bar
+from typing import List, Dict
+from DMT.core import Technology
 from DMT.core.dut_view import DutView
 
 
+try:
+    from semver.version import Version as VersionInfo
+except ImportError:
+    from semver import VersionInfo
+
+SEMVER_DUTMEAS_CURRENT = VersionInfo(major=1, minor=0)
+
+
 class DutMeas(DutView):
     """Subclass of DutView that is used to capture relevant methods and properties of measured data.
 
     Parameters
     ----------
     database_dir         :  string
         Root directory for saving duts and databases of this project.
@@ -66,58 +75,101 @@
         Die identification string of this object.
     ndevices       :  integer
         Number of physically parallel devices of this measurement.
 
     Methods
     -------
     run_simulation(sweep)
-        Return a NotImplemented exception. Measurements can not be simulated!
+        Raises NotImplementedError since measurements can not be simulated!
     get_hash()
         Return a unique hash based on some attributes of the DutMeas object.
     add_short(short, key='/dummies/short', force=True)
         Add a short dummy to the database of this DutMeas object.
     add_open(short, key='/dummies/short', force=True)
         Add an open dummy to the database of this DutMeas object.
-    deembed(filter_func, short_key='/dummies/short', open_key='/dummies/open')
-        Deembed some dataframes of this DutMeas object using a user supplied filter function.
-    clean_data()
-        Clean the dataframe columns of the DataFrame objects in this DutMeas objects database.
     get_output_data(sweep)
         Raises NotImplementedError since a measurement can not return its output files.
-
     """
 
     def __init__(
         self,
         database_dir,
         name,
         dut_type,
-        force=False,
         wafer=None,
         die=None,
         ndevices=1,
         deemb_name=None,
         **kwargs,
     ):
-        super().__init__(database_dir, name, dut_type, nodes=None, force=force, **kwargs)
+        super().__init__(database_dir, name, dut_type, **kwargs)
         self.wafer = wafer
         self.die = die
         self.ndevices = ndevices
 
         if deemb_name is None:
             self.deemb_name = self.name
         else:
             self.deemb_name = deemb_name
 
-        if self.width is not None:
-            try:
-                self.perimeter = (self.width + self.length) * 2
-                self.area = self.width * self.length
-            except TypeError:
-                pass  # if either spacer is None or width or length are tuples.
+    def info_json(self, **_kwargs) -> Dict:
+        """Returns a dict with serializeable content for the json file to create.
+
+        The topmost dict MUST have only one key: The string casted class name.
+        Inside the parameters are:
+
+            * A version key,
+            * all extra parameters of DutMeas compared to DutView and
+            * the info_json of DutView.
+
+        Returns
+        -------
+        dict
+            str(DutMeas): serialized content
+        """
+        return {
+            str(DutMeas): {
+                "__DutMeas__": str(SEMVER_DUTMEAS_CURRENT),
+                "parent": super(DutMeas, self).info_json(**_kwargs),
+                "wafer": self.wafer,
+                "die": self.die,
+                "ndevices": self.ndevices,
+                "deemb_name": self.deemb_name,
+            }
+        }
+
+    @classmethod
+    def from_json(cls, json_content: Dict, classes_technology: List[type[Technology]]) -> "DutMeas":
+        """Static class method. Loads a DutMeas object from a pickle file with full path save_dir.
+
+        Calls the from_json method of DutView with all dictionary inside the "parent" keyword. Afterwards the additional parameters are set correctly.
+
+        Parameters
+        ----------
+        json_content  :  dict
+            Readed dictionary from a saved json DutMeas.
+        classes_technology : List[type[Technology]]
+            All possible technologies this loaded DutMeas can have. One will be choosen according to the serialized technology loaded from the file.
+
+        Returns
+        -------
+        DutMeas
+            Loaded object.
+        """
+        if json_content["__DutMeas__"] != SEMVER_DUTMEAS_CURRENT:
+            raise NotImplementedError("DMT.DutMeas: Unknown version of DutMeas to load!")
+
+        dut_view = super().from_json(json_content["parent"], classes_technology)
+
+        dut_view.wafer = json_content["wafer"]
+        dut_view.die = json_content["die"]
+        dut_view.ndevices = json_content["ndevices"]
+        dut_view.deemb_name = json_content["deemb_name"]
+
+        return dut_view
 
     def run_simulation(self, sweep):
         """Raise a OSError. Measurements can not be simulated!
 
         Raises
         ------
         OSError
@@ -189,80 +241,14 @@
         key    :  string
             Key that will be used to save the short dummy in the database. Default='/dummies/short'
 
         """
         self.add_data(open_, key, force=True)
         logging.info("DMT -> DutMeas -> add_open(): Added an open to the DUT")
 
-    def deembed(self, filter_func, short_key="dummies/short", open_key="dummies/open"):
-        """Deembed some dataframes of this DutMeas object using a user supplied filter function.
-
-        Parameters
-        ----------
-        filter_func  :  callable object
-            This used supplied callable object, e.g. function, is called with each key in the DutView's database.
-            If True is returned, the dataframe corresponding to key is deembedded.
-        short_key    :  string
-            Default='/dummies/short'. Key that corresponds to the short dummy in the database.
-        open_key     :  string
-            Default='/dummies/open'. Key that corresponds to the open dummy in the database.
-
-        Returns
-        -------
-        self  :  DutMeas
-            The updated DutMeas object.
-
-        Notes
-        -----
-        todo: Delete this method since this functionality will be taken over by DutLib!
-        """
-        raise IOError("Obsolete")
-
-        # retrieve the short and open dummies
-        no_dummies = False
-        try:
-            df_short = self.data[short_key]
-            df_open = self.data[open_key]
-        except:
-            no_dummies = True
-
-        # find keys of dataframes that need to be deembedded
-        keys = [key for key in self.data.keys() if filter_func(key)]
-
-        if len(keys) > 0 and no_dummies:
-            raise IOError(
-                "DMT -> DutMeas -> deembed: Found keys that require deembedding, however no short or open dummies are present in this Dut."
-            )
-
-        if len(keys) == 0:  # some DUTs are only DC
-            return self
-
-        # go through each DataFrame where the function filter returns true and deembed()
-        i = 0
-        n_frames = len(self.data)
-        print_progress_bar(i, n_frames, prefix="Deembedding:", suffix="Complete\n", length=50)
-        for key in self.data.keys():
-            if filter_func(key):
-                i = i + 1
-                df = self.data[key]
-                self.data[key] = df.deembed(df_open, df_short, ports=self.nodes)
-                logging.info("DMT -> DutMeas -> deembed(): Deembedded dataframe with key %s.", key)
-                print_progress_bar(
-                    i, n_frames, prefix="Deembedding:", suffix="Complete\n", length=50
-                )
-
-        if (
-            self.ndevices > 1
-        ):  # if we have more than one device in parallel, normalize the currents to the area of one device
-            for key in self.data.keys():
-                df = self.data[key]
-                self.data[key] = df.parallel_norm(self.ndevices)
-
-        return self
-
     def get_output_data(self, sweep):
         raise NotImplementedError(
             "DMT -> DutMeas -> get_output_data(): DutMeas does not implement this method on purpose!"
         )
 
     def join_key_temperature(self, *key_parts, temperature_converter=None):
         """Collects the temperature from key_parts and replaces it by a proper temperature key part.
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/dut_view.py` & `DMT_core-2.0.0/DMT/core/dut_view.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,22 +17,39 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 import os
 import re
 import shutil
 import _pickle as cpickle  # type: ignore
-
-# import pickle as cpickle
+import json
 import copy
 import logging
-from DMT.core import DatabaseManager, read_data, DataFrame, VAFile
-from DMT.config import DATA_CONFIG
 from pathlib import Path
 import pandas as pd
+from typing import List, Dict
+
+try:
+    from semver.version import Version as VersionInfo
+except ImportError:
+    from semver import VersionInfo
+
+from DMT.core import (
+    DatabaseManager,
+    read_data,
+    DataFrame,
+    VAFileMap,
+    DutTypeFlag,
+    DutTypeInt,
+    DutType,
+    Technology,
+)
+from DMT.config import DATA_CONFIG
+
+SEMVER_DUTVIEW_CURRENT = VersionInfo(major=1, minor=0)
 
 
 class DutView(object):
     """DutView is the parent class of all DUTs in DMT.
 
     All simulation back-end classes must inherit from this class and overwrite the methods that raise NotImplemented errors.
     This ensures that all classes in DMT work independent of the concrete simulation back-end.
@@ -136,62 +153,79 @@
     """
 
     def __init__(
         self,
         database_dir,
         name,
         dut_type,
+        *,
+        reference_node,
         copy_va_files=True,
         force=False,
+        loading=False,
         separate_databases=False,
         list_copy=None,
         t_max=None,
+        sim_dir=DATA_CONFIG["directories"]["simulation"],
         simulate_on_server=None,
         simulator_command="",
         simulator_arguments=None,
         technology=None,
         width=None,
         length=None,
         nfinger=None,
         contact_config=None,
         flavor=None,
         ac_ports=None,
-        reference_node=None,
         nodes=None,
         inp_name=None,
         va_code_filter=None,
     ):
+        if database_dir is None:
+            self._database_dir = DATA_CONFIG["directories"]["database"]
+        else:
+            if isinstance(database_dir, Path):
+                self._database_dir = database_dir.expanduser().resolve()
+            else:
+                self._database_dir = Path(database_dir).expanduser().resolve()
+
+        if os.path.isabs(name):
+            raise IOError(
+                "DMT.DutView: The DutView name must not be a valid absolute directory path!"
+            )
+        self.name = name
         self._copy_va_files = copy_va_files
         # files to be copied into simulation directory
         if list_copy is None:
             self.list_copy = []
         else:
             if not isinstance(list_copy, list):
                 self.list_copy = [list_copy]
             else:
                 self.list_copy = list_copy
+        self._list_va_file_contents: list[VAFileMap] = []
 
-        self._list_va_file_contents: list[VAFile] = []
+        # if the dut already exists and no force -> error!
+        if self.save_dir:
+            if force:
+                # delete the saved database
+                self.del_db()
+                self.del_dut()
+            elif loading:
+                pass
+            else:
+                raise IOError(
+                    "DMT.DutView: Created a DutView with a save_dir which already exists. Better load that one or remove it."
+                )
 
         # attributes for data management
         self._separate_databases = separate_databases
         self._data = {}  # this is now hidden
-        if database_dir is None:
-            self._database_dir = DATA_CONFIG["directories"]["database"]
-        else:
-            if isinstance(database_dir, Path):
-                self._database_dir = database_dir.expanduser().resolve()
-            else:
-                self._database_dir = Path(database_dir).expanduser().resolve()
-
-        self.dut_type = dut_type
 
-        if os.path.isabs(name):
-            raise IOError("The DuT name must not be a valid absolute directory path!")
-        self.name = name
+        self.dut_type: DutTypeFlag | DutTypeInt = dut_type
 
         self.manager = DatabaseManager()
         if nodes is None:
             self.nodes = dut_type.get_nodes()
         else:
             if isinstance(nodes, str):
                 self.nodes = nodes.split(",")
@@ -213,45 +247,26 @@
         self.va_code_filter = va_code_filter
 
         if simulator_arguments is None:
             self.sim_args = []
         else:
             self.sim_args = simulator_arguments
 
-        if force:
-            # delete the saved database
-            if self.save_dir is not None:
-                self.del_db()
-                self.del_dut()
-
-        # try to reload this Dut if it already exists!
-        if self.save_dir and not force:
-            pickle = Path(self.dut_dir)
-            if pickle.is_file():
-                existing_dut = DutView.load_dut(self.dut_dir)
-                self.__dict__.update(existing_dut.__dict__)
-
-        self.sim_dir = DATA_CONFIG["directories"]["simulation"]
+        self.sim_dir = sim_dir
 
         self.technology = technology
         self.contact_config = contact_config
         self.flavor = flavor
         self.width = width
         self.length = length
         self.nfinger = nfinger
         try:
-            # if ( # was
-            #     (width is not None)
-            #     and (length is not None)
-            #     and (not isinstance(length, tuple) and (not isinstance(width, tuple)))
-            # ):
             self.perimeter = (self.width + self.length) * 2  # type: ignore
             self.area = self.width * self.length  # type: ignore
         except TypeError:
-            # else:
             self.perimeter = None
             self.area = None
 
         # simulation attributes
         self.t_max = t_max
         if simulate_on_server is None:
             self.simulate_on_server = DATA_CONFIG["backend_remote"]
@@ -275,46 +290,45 @@
             self.get_hash(),
             sweep.get_hash(),
         )
 
         # set the simulation folder
         sim_folder = self.get_sim_folder(sweep)
 
-        inp_content = self.make_input(sweep)
-
         try:
             sim_folder.mkdir(parents=True)
         except OSError:
             logging.debug("Folder already existed! Will be deleted")
             try:
                 shutil.rmtree(str(sim_folder))
                 sim_folder.mkdir(parents=True, exist_ok=True)
             except FileNotFoundError:
                 raise OSError(
                     "Simulation folder exists but can not be deleted. Is the location mounted correctly? Hint: Shut down Windows correctly."
                 )
 
-        (sim_folder / self.inp_name).write_text(inp_content)
-        if DATA_CONFIG["server"]["use_pbs"] and DATA_CONFIG["backend_remote"]:
-            pbs_content = self.make_pbs(sweep)  # needs to be implemented by the DUT
-            (sim_folder / "pbs_job").write_text(pbs_content)
-
-        # copy va files?
+        # copy va files into simulation folder?
         sim_folder = self.get_sim_folder(sweep)
         if self._copy_va_files:
             for vafile in self._list_va_file_contents:
                 vafile.write_files(sim_folder, filter=self.va_code_filter)
         else:
             # write the files into a separate folder in simulations/va_files/HASH/
             va_files_dir = self.sim_dir / "VA_codes"
             for vafile in self._list_va_file_contents:
                 dir_code = va_files_dir / vafile.get_tree_hash()
                 if not dir_code.is_dir():
                     vafile.write_files(dir_code, filter=self.va_code_filter)
 
+        inp_content = self.make_input(sweep)
+        (sim_folder / self.inp_name).write_text(inp_content)
+        if DATA_CONFIG["server"]["use_pbs"] and DATA_CONFIG["backend_remote"]:
+            pbs_content = self.make_pbs(sweep)  # needs to be implemented by the DUT
+            (sim_folder / "pbs_job").write_text(pbs_content)
+
         for data_copy in self.list_copy:
             try:
                 if os.path.isfile(data_copy):
                     filename = os.path.basename(data_copy)
                     shutil.copyfile(data_copy, os.path.join(sim_folder, filename))
                 else:
                     # filename ??? Setting default file name... seems crazy here
@@ -429,15 +443,15 @@
 
     def get_db_dir(self, name="db"):
         """Returns the name for a db, either use 'db' for regular behavior or use 'sweep.get_hash()' for a db per sweep."""
         return self.save_dir / (name + ".h5")
 
     @property
     def dut_dir(self):
-        return self.save_dir / "dut.p"
+        return self.save_dir / "dut.json"
 
     @property
     def data(self):
         """data is a property to ensure loading before usage.
 
         As _data is a dict, the getter is also called before setting. So the separate setter is not necessary.
         If someone tries to set dut.data an attribute error occurs, but setting dict entries is possible directly.
@@ -482,27 +496,72 @@
 
         logging.info(
             "The simulation data of the sweep %s with the hash %s was deleted",
             sweep.name,
             sweep.get_hash(),
         )
 
-    def save(self):
-        """Save this DutView as a pickled .p file and the also the data into the database on the hard drive."""
+    def save(self, **kwargs):
+        """Save this DutView as a json file and the also the data into the database on the hard drive. The kwargs are passed on to :py:method::`DMT.core.dut_view.DutView.info_json()` or the overwritten method."""
         self.save_dir.mkdir(parents=True, exist_ok=True)
         self._database_dir = self._database_dir.resolve()  # convert to absolute path
 
         self.save_db()
-        with open(self.dut_dir, "wb") as handle:
-            cpickle.dump(self, handle)
-        # with warnings.catch_warnings():
-        # warnings.simplefilter('ignore', tb.NaturalNameWarning)
+
+        self.dut_dir.write_text(json.dumps(self.info_json(**kwargs), indent=4), encoding="utf8")
+
+    def info_json(self, **_kwargs):
+        """Returns a dict with serializeable content for the json file to create.
+
+        Add the info about the concrete subclass to create here! See :py:method::`DMT.core.dut_meas.DutMeas.info_json()` for an example implementation.
+
+        Returns
+        -------
+        dict
+            serialized dictionary ready to be dumped to json.
+        """
+        if self.technology is None:
+            tech = self.technology
+        else:
+            tech = self.technology.serialize()
+        return {
+            "__DutView__": str(SEMVER_DUTVIEW_CURRENT),
+            "copy_va_files": self._copy_va_files,
+            "list_copy": [str(to_copy) for to_copy in self.list_copy],
+            "list_va_file_contents": [
+                va_file.export_dict() for va_file in self._list_va_file_contents
+            ],
+            "separate_databases": self._separate_databases,
+            "database_dir": str(self._database_dir),
+            "dut_type": self.dut_type.serialize(),
+            "name": self.name,
+            "nodes": self.nodes,
+            "ac_ports": self.ac_ports,
+            "reference_node": self.reference_node,
+            "inp_name": self.inp_name,
+            "sim_command": self.sim_command,
+            "va_code_filter": self.va_code_filter,
+            "sim_args": self.sim_args,
+            "sim_dir": str(self.sim_dir),
+            "technology": tech,
+            "contact_config": self.contact_config,
+            "flavor": self.flavor,
+            "width": self.width,
+            "length": self.length,
+            "nfinger": self.nfinger,
+            "t_max": self.t_max,
+            "simulate_on_server": self.simulate_on_server,
+            "zip_result": self.zip_result,
+            "open_deembedded_with": self.open_deembedded_with,
+            "short_deembedded_with": self.short_deembedded_with,
+        }
 
     def __getstate__(self):
         """Return state values to be pickled. Implemented according `to <https://www.ibm.com/developerworks/library/l-pypers/index.html>`_ .
+
         Notes
         -----
         ..todo:
             iterate through all properties and throw away the HDFStore objects.
         """
         d = copy.copy(self.__dict__)
 
@@ -513,46 +572,160 @@
 
     def __setstate__(self, state):
         """Return state values to be pickled. Implemented according `to <https://www.ibm.com/developerworks/library/l-pypers/index.html>`_ ."""
         self.__dict__ = state  # pylint: disable=attribute-defined-outside-init
         self.__dict__["_data"] = {}
 
     @staticmethod
-    def load_dut(file_dut):
+    def load_dut(
+        file_dut,
+        classes_technology: List[type[Technology]] = None,
+        classes_dut_view: List[type["DutView"]] = None,
+    ) -> "DutView":
         """Static class method. Loads a DutView object from a pickle file with full path save_dir.
 
         Parameters
         ----------
         file_dut  :  str or os.Pathlike
-            Path to the pickled DutView object that shall be loaded.
+            Path to the json or pickle DutView file that shall be loaded.
+        classes_technology : List[type[Technology]]
+            All possible technologies this loaded DutView can have. One will be choosen according to the serialized technology loaded from the file.
+        classes_dut_view : List[type[DutView]]
+            All possible DutViews this loaded DutView can be. One will be choosen according to the serialized dutview class name loaded from the file.
 
         Returns
         -------
-        obj  :  DutView()
-            Loaded object from the pickle file.
+        DutView
+            Loaded object.
         """
         if not isinstance(file_dut, Path):
             file_dut = Path(file_dut)
 
-        with file_dut.open(mode="rb") as handle:
-            dut = cpickle.load(handle)
+        if file_dut.suffix == ".json":
+            from DMT.core import _DEFAULT_DUT_VIEWS
+
+            if classes_dut_view is None:
+                classes_dut_view = _DEFAULT_DUT_VIEWS
+            else:
+                classes_dut_view += _DEFAULT_DUT_VIEWS
+
+            with file_dut.open("r", encoding="utf8") as file_json:
+                json_content = json.load(file_json)
+
+            # the key on the first dictionary is the class
+            clsstr_dut_view = list(json_content.keys())[0]
+            cls_dut_view = next(
+                cls_dv for cls_dv in classes_dut_view if str(cls_dv) == clsstr_dut_view
+            )
+
+            dut = cls_dut_view.from_json(json_content[clsstr_dut_view], classes_technology)
+
+        elif file_dut.suffix == ".p":
+            with file_dut.open(mode="rb") as handle:
+                dut = cpickle.load(handle)
+        else:
+            raise IOError("DMT.DutView: I can not load an file ending on " + file_dut.suffix)
 
         # check the dirs:
         # obtain database_dir from file_dut
         database_dir = file_dut.parent.parent
 
         # check if equal, if not -> changed machine -> broken absolute path
         if database_dir != dut._database_dir:  # pylint: disable=protected-access
             dut._database_dir = database_dir  # pylint: disable=protected-access
 
         if not os.path.exists(dut.sim_dir):
             dut.sim_dir = DATA_CONFIG["directories"]["simulation"]
 
         return dut
 
+    @classmethod
+    def from_json(
+        cls,
+        json_content: Dict,
+        classes_technology: List[type[Technology]],
+        subclass_kwargs: Dict = None,
+    ) -> "DutView":
+        """Static class method. Loads a DutView object from a pickle file with full path save_dir.
+
+        Parameters
+        ----------
+        json_content  :  dict
+            Readed dictionary from a saved json DutView.
+        classes_technology : List[type[Technology]]
+            All possible technologies this loaded DutView can have. One will be choosen according to the serialized technology loaded from the file.
+        subclass_args: List = None,
+            Positional arguments needed
+        subclass_kwargs: Dict = None,
+
+        Returns
+        -------
+        DutView
+            Loaded object.
+        """
+        if json_content["__DutView__"] != SEMVER_DUTVIEW_CURRENT:
+            raise NotImplementedError("DMT.DutView: Unknown version of DutView to load!")
+
+        serialized_technology = json_content["technology"]
+        if serialized_technology is None:
+            tech = None
+        else:
+            cls_technology = next(
+                cls_tech
+                for cls_tech in classes_technology
+                if str(cls_tech) == serialized_technology["class"]
+            )
+            args = serialized_technology.get("args", [])
+            kwargs = serialized_technology.get("kwargs", {})
+            if serialized_technology.get("constructor", None) is None:
+                tech = cls_technology(*args, **kwargs)
+            else:
+                tech = getattr(cls_technology, serialized_technology["constructor"])(
+                    *args, **kwargs
+                )
+
+        if subclass_kwargs is None:
+            subclass_kwargs = {}
+
+        dut_view = cls(
+            database_dir=json_content["database_dir"],
+            name=json_content["name"],
+            dut_type=DutType.deserialize(json_content["dut_type"]),
+            **subclass_kwargs,
+            reference_node=json_content["reference_node"],
+            copy_va_files=json_content["copy_va_files"],
+            force=False,
+            loading=True,
+            separate_databases=json_content["separate_databases"],
+            list_copy=json_content["list_copy"],
+            t_max=json_content["t_max"],
+            sim_dir=json_content["sim_dir"],
+            simulate_on_server=json_content["simulate_on_server"],
+            simulator_command=json_content["sim_command"],
+            simulator_arguments=json_content["sim_args"],
+            technology=tech,
+            width=json_content["width"],
+            length=json_content["length"],
+            nfinger=json_content["nfinger"],
+            contact_config=json_content["contact_config"],
+            flavor=json_content["flavor"],
+            ac_ports=json_content["ac_ports"],
+            nodes=json_content["nodes"],
+            inp_name=json_content["inp_name"],
+            va_code_filter=json_content["va_code_filter"],
+        )
+
+        dut_view._list_va_file_contents = [
+            VAFileMap.import_dict(va_file) for va_file in json_content["list_va_file_contents"]
+        ]
+        dut_view.zip_result = json_content["zip_result"]
+        dut_view.open_deembedded_with = json_content["open_deembedded_with"]
+        dut_view.short_deembedded_with = json_content["short_deembedded_with"]
+        return dut_view
+
     def add_data(self, data, key=None, force=True, **kwargs):
         """Add a measurement or simulation data to the DutView's data.
 
         Parameters
         ----------
         data   :   DataFrame, sweep or str
             If DataFrame: Directly added to the data using the given key.
@@ -692,27 +865,35 @@
                     fallback=fallback,
                     ac_ports=self.ac_ports,
                     **kwargs,
                 )
 
             self.data[key] = df
 
-    def save_db(self):
-        """Write a database for this dut. If it already exists it is overwritten. Does NOT save all keys starting with '_'"""
+    def save_db(self, sweep_keys=None):
+        """Write a database for this dut. If it already exists it is overwritten. Does NOT save all keys starting with '_'
+
+        Parameters
+        ----------
+        sweep_keys : list[str], optional
+            List of sweeps to save to database. Usefull if a lot of data is loaded but only a part should be saved to the hard drive database.
+
+        """
         if not self._data:
             return  # nothing to do here
 
         if self._separate_databases:
-            # find all sweeps in self.data
-            sweep_keys = []
-            for key in self._data.keys():
-                ## key is equal except for the last part -> same sweep
-                sweep_key = self.join_key(*self.split_key(key)[0:-1])
-                if sweep_key not in sweep_keys:
-                    sweep_keys.append(sweep_key)
+            if sweep_keys is None:
+                # find all sweeps in self.data
+                sweep_keys = []
+                for key in self._data.keys():
+                    ## key is equal except for the last part -> same sweep
+                    sweep_key = self.join_key(*self.split_key(key)[0:-1])
+                    if sweep_key not in sweep_keys:
+                        sweep_keys.append(sweep_key)
 
             for sweep_key in sweep_keys:
                 data_to_save = {}
                 for key, data in self._data.items():
                     if (
                         not key.startswith("_")
                         and self.join_key(*self.split_key(key)[0:-1]) == sweep_key
@@ -734,33 +915,50 @@
         If the complete dictionary is reloaded, here it is set directly to self._data.
         if separate databases is activated it loads only the given sweep (and it has to be given then!)
 
         Parameters
         ----------
         sweep : Sweep or str, optional
             In case of separate databases, the sweep must be given either directly or as string name
+
+        Returns
+        -------
+        bool
+            Is True if the database was loaded successfully
         """
         if self._separate_databases:
             if sweep is None:
-                return
+                return True
+                # raise IOError(
+                #     "DMT->DutView: If a separated database should be loaded, the sweep/databasefilename has to be given"
+                # )
 
             if isinstance(sweep, str):
-                name = sweep
+                if sweep == "all":
+                    # iter throuh self.save_dir and load all .h5
+                    for file_db in self.save_dir.glob("**/*.h5"):
+                        self._data.update(self.manager.load_db(file_db))
+
+                    return True
+                else:
+                    name = sweep
             else:
                 name = self.get_sweep_key(sweep)
 
             try:
                 self._data.update(self.manager.load_db(self.get_db_dir(name)))
             except FileNotFoundError:
-                pass
+                return False
         else:
             try:
                 self._data = self.manager.load_db(self.get_db_dir())
             except FileNotFoundError:
-                pass
+                return False
+
+        return True
 
     def check_existence_sweep(self, sweep):
         """Return true, if the combination dut+sweep has already been simulated.
 
         If self.data is None, the database is loaded first.
 
         Parameters
@@ -848,17 +1046,17 @@
         Returns
         -------
         temp : float
             The temperature at which the measurement "key" has been conducted in Kelvin.
         """
         key_parts = self.split_key(key)
 
-        # first check the best and most usefull way for a single temperature
+        # first check the best and most useful way for a single temperature
         for key_part in key_parts:
-            re_temp = re.search(r"T([0-9p\.]+)K", key_part)
+            re_temp = re.search(r"T?([0-9p\.]+)K", key_part)
             if re_temp:
                 try:
                     # always replace "p" with ".", if it is already with ".", it doesnt matter
                     return round(float(re_temp.group(1).replace("p", ".")), 3)
                 except ValueError:
                     # if a value error in the except clause happens, try the next key part.
                     pass
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/hasher.py` & `DMT_core-2.0.0/DMT/core/hasher.py`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/core/mc_parameter.py` & `DMT_core-2.0.0/DMT/core/mc_parameter.py`

 * *Files 2% similar despite different names*

```diff
@@ -144,18 +144,21 @@
         inc_min: bool = True,
         inc_max: bool = True,
         exclude: Union[List[Union[float, int]], float, int, None] = None,
         group: str = "",
         unit: Unit = unit_registry.dimensionless,
         description: str = "",
     ):
-
         if not isinstance(name, str):
-            raise IOError("DMT -> McParameter: Parameter name not a string.")
-        self.name = name.lower()  # always lower case...
+            raise IOError("DMT->McParameter: Parameter name not a string.")
+        if any(char.isupper() for char in name):
+            # always lower case...
+            raise IOError("DMT->McParameter: Parameter name must be all lower case.")
+
+        self.name = name
         self.inc_min = inc_min
         self.inc_max = inc_max
         if value_type == int:
             self._val_type = int
         elif value_type == float:
             self._val_type = float
         else:
@@ -685,32 +688,37 @@
             "possible_groups": self.possible_groups,
             "__McParameterCollection__": str(SEMVER_MCPARAMETER_Collection_CURRENT),
         }  # make versions, so we can introduce compatibility here!
 
     def dump_json(self, file_path, **kwargs):
         """Writes itself and the parameters in the collection to a file.
 
-        To manipulate what is written to the file, change :py:method::`DMT.core.mc_parameter.McParameterCollection.dumps_json()`
+        To manipulate what is written to the file, change :py:method::`DMT.core.mc_parameter.McParameterCollection.info_json()` and inherited methods
         """
         if not isinstance(file_path, Path):
             file_path = Path(file_path)
 
+        str_content = self.dumps_json(**kwargs)
+
+        file_path.write_text(str_content, encoding="utf8")
+
+    def dumps_json(self, **kwargs):
         content = []
         for para in sorted(self.paras, key=lambda x: (x.group, x.name)):
             content.append(para.dict_json())
         content.append(self.info_json(**kwargs))
 
         str_content = "["
         for subdict in content:
             str_content += "\n    " + json.dumps(subdict) + ","
         # remove trailing ,
         str_content = str_content[:-1]
         str_content += "]"
 
-        file_path.write_text(str_content, encoding="utf8")
+        return str_content
 
     @classmethod
     def load_json(
         cls,
         file_path: Union[str, Path],
         directory_va_file: Union[str, Path, None] = None,
         ignore_checksum: bool = False,
@@ -737,16 +745,51 @@
         ------
         IOError
             If the collection dictionary is not found in the json file.
         """
         if not isinstance(file_path, Path):
             file_path = Path(file_path)
 
-        with file_path.open("r", encoding="utf8") as file_json:
-            content = json.load(file_json)
+        return cls.loads_json(
+            file_path.read_text(encoding="utf8"),
+            directory_va_file=directory_va_file,
+            ignore_checksum=ignore_checksum,
+        )
+
+    @classmethod
+    def loads_json(
+        cls,
+        s: str,
+        directory_va_file: Union[str, Path, None] = None,
+        ignore_checksum: bool = False,
+    ) -> McParameterCollection:
+        """Loads the json string, creates the McParameterCollection (or inherited) and adds the McParameters.
+
+        Parameters
+        ----------
+        file_path : Union[str, Path]
+            string with the json.
+        directory_va_file : Union[str, Path, None], optional
+            If a relative path to a va_file is set in the modelcard, pass the absolute path to the start folder here, by default None.
+            This can be used to load old json modelcards from before saving the full code with the parameters.
+        ignore_checksum : bool, optional
+            When the code is saved compressed, a checksum is saved with it. If you want to ignore the checksum set this to true, by default False
+
+
+        Returns
+        -------
+        McParameterCollection
+            The loaded collection
+
+        Raises
+        ------
+        IOError
+            If the collection dictionary is not found in the json file.
+        """
+        content = json.loads(s)
 
         collection = None
         for dict_content in content:
             if (
                 "__McParameterCollection__" in dict_content
                 or "__McParameterComposition__" in dict_content
             ):
@@ -879,15 +922,15 @@
             The policy for missing parameters to set, defaults to "error"
 
         Raises
         ------
         KeyError
             If the para was not in self.
         """
-        for name, value in dict_parameters.items():
+        for name, value in list(dict_parameters.items()):
             name = name.lower()
             try:
                 index = self.name.index(name)
             except ValueError as err:
                 if policy_missing == "ignore":
                     # nothing to do here
                     continue
@@ -906,17 +949,15 @@
                 if force:
                     para = self.get(name)
                     para._set_forced(value)  # type: ignore
                     self.set(para, update=False)
                 else:
                     raise
 
-            dict_parameters[name] = self._paras[index].val_type(value)
-
-        self._values.update(dict_parameters)
+            self._values[name] = self._paras[index].val_type(value)
 
     def get_values(self, parameters):
         """Returns a list of the values of parameters.
 
         Returns
         -------
         {name:value}
@@ -1338,25 +1379,7 @@
     def __eq__(self, other):
         """Allows comparing 2 model cards using mc1 == mc2"""
         if isinstance(other, McParameterCollection):
             # can only compare to other collections
             return self.eq_paras(other)
 
         return NotImplemented
-
-
-class McParameterComposition(McParameterCollection):
-    """Deprecated name for the mc parameter collection"""
-
-    def __init__(
-        self,
-        __McParameterComposition__: Union[
-            VersionInfo, str, float
-        ] = "1.0.0",  # as until now there is only v1.0.0 around we have no issues here.
-        **kwargs,
-    ):
-        warnings.warn(
-            "McParameterComposition is deprecated. It was renamed to McParameterCollection to avoid confusion with the composition design pattern.\nMcParameterCompostion will be deleted in the next major release.",
-            category=DeprecationWarning,
-        )
-
-        super().__init__(**kwargs)
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/mc_skywater.py` & `DMT_core-2.0.0/DMT/core/mc_skywater.py`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/core/mcard.py` & `DMT_core-2.0.0/DMT/core/mcard.py`

 * *Files 19% similar despite different names*

```diff
@@ -39,63 +39,90 @@
 try:
     from semver.version import Version as VersionInfo
 except ImportError:
     from semver import VersionInfo
 
 import verilogae
 
-from DMT.core import unit_registry, VAFile
+from DMT.core import unit_registry, VAFileMap
 from DMT.core.mc_parameter import McParameterCollection, McParameter
 
 
 unit_converter = {
     "s": unit_registry.second,
     "sec": unit_registry.second,
     "A": unit_registry.ampere,
     "A^2s": unit_registry.ampere * unit_registry.ampere * unit_registry.second,
+    "A/V^3": unit_registry.ampere / unit_registry.volt / unit_registry.volt / unit_registry.volt,
     "V": unit_registry.volt,
     "1/V": 1 / unit_registry.volt,
+    "V^-1": 1 / unit_registry.volt,
+    "V^-1/m^2": 1 / unit_registry.volt / unit_registry.meter / unit_registry.meter,
+    "V^-1/m^4": 1
+    / unit_registry.volt
+    / unit_registry.meter
+    / unit_registry.meter
+    / unit_registry.meter
+    / unit_registry.meter,
+    "V^-0.5": 1 / unit_registry.volt,  # TODO
     "K": unit_registry.kelvin,
+    "J/K": unit_registry.joule / unit_registry.kelvin,
     "1/K": 1 / unit_registry.kelvin,
     "K^-1": 1 / unit_registry.kelvin,
     "C": unit_registry.celsius,
     "ohm": unit_registry.ohm,
     "Ohm": unit_registry.ohm,
+    "Ohm/sq": unit_registry.ohm,  # TODO
+    "Ohm m^2": unit_registry.ohm * unit_registry.meter * unit_registry.meter,
     "F": unit_registry.farad,
     "Coul": unit_registry.coulomb,
     "K/W": unit_registry.kelvin / unit_registry.watt,
     "J/W": unit_registry.joule / unit_registry.watt,
     "V/K": unit_registry.volt / unit_registry.kelvin,
     "1/K^2": 1 / unit_registry.kelvin / unit_registry.kelvin,
     "Ws/K": unit_registry.watt * unit_registry.second / unit_registry.kelvin,
     "M^(1-AF)": unit_registry.dimensionless,
+    "m/V": unit_registry.meter / unit_registry.volt,
     "m": unit_registry.meter,
     "m^2": unit_registry.meter * unit_registry.meter,
+    "m^2/V/s": unit_registry.meter
+    * unit_registry.meter
+    / unit_registry.volt
+    / unit_registry.second,
     "Am^-1": unit_registry.ampere / unit_registry.meter,
     "Am^-2": unit_registry.ampere / unit_registry.meter / unit_registry.meter,
     "Am^-3": unit_registry.ampere / unit_registry.meter / unit_registry.meter / unit_registry.meter,
     "AV^-3": unit_registry.ampere / unit_registry.volt / unit_registry.volt / unit_registry.volt,
     "AV^-3m": unit_registry.ampere
     / unit_registry.volt
     / unit_registry.volt
     / unit_registry.volt
     * unit_registry.meter,
     "Fm^-1": unit_registry.farad / unit_registry.meter,
     "Fm^-2": unit_registry.farad / unit_registry.meter / unit_registry.meter,
     "cm^-3": 1 / unit_registry.meter / unit_registry.meter / unit_registry.meter,  # mhm centi ?
     "Vm^-1": unit_registry.volt / unit_registry.meter,
+    "m^-3": 1 / unit_registry.meter / unit_registry.meter / unit_registry.meter,
+    "Vm": unit_registry.volt * unit_registry.meter,
     "VA^-1m": unit_registry.volt / unit_registry.ampere * unit_registry.meter,
     "VA^-1m^2": unit_registry.volt
     / unit_registry.ampere
     * unit_registry.meter
     * unit_registry.meter,
     "": unit_registry.dimensionless,
+    # TODO: PSP units that do not make sense
+    "m^LLODKUO": unit_registry.meter,
+    "m^WLODKUO": unit_registry.meter,
+    "m^(LLODKUO+WLODKUO)": unit_registry.meter,
+    "m^LLODVTH": unit_registry.meter,
+    "m^WLODVTH": unit_registry.meter,
+    "m^(LLODVTH+WLODVTH)": unit_registry.meter,
 }
 
-SEMVER_MCARD_CURRENT = VersionInfo(major=2, minor=2)
+SEMVER_MCARD_CURRENT = VersionInfo(major=2, minor=3)
 
 
 class MCard(McParameterCollection):
     """DMT class that implements attributes and methods that are common between all ModelCards such as HICUM and BSIM.
 
     Parameters
     ----------
@@ -147,14 +174,15 @@
         va_codes=None,
         vae_module=None,
         directory_va_file: Optional[Union[str, os.PathLike]] = None,
         __MCard__=SEMVER_MCARD_CURRENT,
         ignore_checksum: bool = False,
         pdk_path: str = "",
         pdk_corner: str = "",
+        op_vars: Optional[list[str]] = None,
         **kwargs,
     ):
         super().__init__(**kwargs)
 
         if not isinstance(__MCard__, VersionInfo):
             try:
                 __MCard__ = VersionInfo.parse(__MCard__)
@@ -187,64 +215,59 @@
                     print("No directory for the va-file is set. No VA-Code is set by core!")
                     print(
                         "To set the directory use: MCard.load_json(path_to_json, directory_va_file=path_to_directory)"
                     )
                     va_file = None  # delete file name to escape error while try to load
 
             if vae_module is not None:
-                raise NotImplementedError
+                raise NotImplementedError()
 
         elif __MCard__ == VersionInfo(major=2, minor=0):
             pass  # nothing to do here?!
         elif __MCard__ == VersionInfo(major=2, minor=1):
             pass  # nothing to do here?!
+        elif __MCard__ == VersionInfo(major=2, minor=2):
+            pass  # nothing to do here: Only added op_vars
         elif __MCard__ != SEMVER_MCARD_CURRENT:
             raise NotImplementedError("DMT->MCard: Unknown version of MCard to create!")
 
         self.nodes_list = nodes_list
         self.default_subckt_name = default_subckt_name
         self.default_module_name = default_module_name
         self.version = version
         self.pdk_path = pdk_path
         self.pdk_corner = pdk_corner
+        if op_vars is None:
+            self.op_vars = []
+        else:
+            self.op_vars = op_vars
 
         self._va_codes = None
         if va_codes is not None:
             if isinstance(va_codes, dict):
-                self._va_codes = VAFile.import_dict(va_codes, ignore_checksum=ignore_checksum)
+                self._va_codes = VAFileMap.import_dict(va_codes, ignore_checksum=ignore_checksum)
             else:
                 self._va_codes = va_codes
         elif va_file is not None:
             self.set_va_codes(va_file)
 
         if self._va_codes:
             self.update_from_vae()
 
     @property
-    def va_codes(self) -> Union[VAFile, None]:
+    def va_codes(self) -> Union[VAFileMap, None]:
         """Return the attribute directly
 
         Returns
         -------
-        VAFile
+        VAFileMap
 
         """
         return self._va_codes
 
-    # @va_codes.setter
-    # def va_codes(self, va_codes_new: VAFile):
-    #     """Set the va_codes
-
-    #     Parameters
-    #     ----------
-    #     va_codes_new : VAFile
-    #         New rel paths with codes
-    #     """
-    #     self._va_codes = va_codes_new
-
     def set_va_codes(
         self, path_to_main_code: Union[os.PathLike, str], version: Union[str, float] = None
     ):
         """Sets self._va_codes by extracting all included files from the main file down the include tree.
 
         Parameters
         ----------
@@ -257,15 +280,15 @@
         ------
         NotImplementedError
             If a file is included via absolute path.
         """
         if not isinstance(path_to_main_code, Path):
             path_to_main_code = Path(path_to_main_code)
 
-        self._va_codes = VAFile(path_to_main_code.name)
+        self._va_codes = VAFileMap(path_to_main_code.name)
         self._va_codes.read_structure(path_to_main_code.parent)
 
         if version is not None:
             self.version = version
 
     def get_verilogae_model(self) -> ModuleType:
         """Returns the Verilogae Model for this modelcard
@@ -294,32 +317,33 @@
         remove_old_parameters : bool, optional
             Deletes parameters which are not part of the VA-Code, by default False
         """
         vae_module = self.get_verilogae_model()
         paras_new = []
         # Updated parameter properties
         for para_name, para_properties in vae_module.modelcard.items():
+            para_name = para_name.lower()
             try:
                 # para = next(para for para in self._paras if para.name == para_name)
                 para = self.get(para_name)
                 self.remove(para_name)
                 ty = type(para_properties.default)
+                para.val_type = ty  # type: ignore
 
                 if para.min > para_properties.min:
                     para.min = para_properties.min
                     para.inc_min = para_properties.min_inclusive  # type: ignore
 
                 if para.max < para_properties.max:
                     para.max = para_properties.max
                     para.inc_max = para_properties.max_inclusive  # type: ignore
 
                 para.unit = unit_converter[para_properties.unit]  # type: ignore
                 para.description = para_properties.description  # type: ignore
                 para.group = para_properties.group  # type: ignore
-                para.val_type = ty  # type: ignore
             except KeyError:
                 para = McParameter(
                     para_name,
                     value=para_properties.default,
                     minval=para_properties.min,
                     maxval=para_properties.max,
                     value_type=type(para_properties.default),
@@ -338,207 +362,15 @@
         for para in paras_new:
             self.add(para, update=False)
 
         self.update_values()
 
         self.default_module_name = vae_module.module_name
         self.nodes_list = vae_module.nodes
-        # self.version = ?? -> can be set in the submodules according to some model specific stuff
-
-    def read_va_file_boundaries(self, remove_old_parameters=True):
-        """Reads the parameter boundaries and possible OPvars from a Verilog-AMS-File
-
-        Needs only to be done once per VA-File, as the boundaries then can
-        be saved/loaded from a json (see dump_json)
-
-        Parameters
-        ----------
-        remove_old_parameters : {True, False}, optional
-            If False, parameters which are not found in the VA-File are not removed.
-        """
-        print(
-            "DMT.MCard: Reading from VA-File using this Method is deprecated. Use update_from_vae!"
-        )
-        paras_new = []
-
-        if self.va_codes is None:
-            return
-
-        for va_file, va_code in self.va_codes.iter_codes():
-            logging.info(
-                "Reading parameter boundaries and operation point variables from %s", va_file
-            )
-
-            lines = va_code.code.split("\n")
-            group = None
-            for line in lines:
-                if re.match(r"\s*module", line):
-                    # module hic0_full (c,b,e,s,tnode);
-                    # module hicumL2va (c,b,e,s,tnode);
-                    mo_module_name = re.search(r"module\s(\S+?)\s*\((.+?)\)", line)
-                    self.default_module_name = mo_module_name.group(1)
-                    self.nodes_list = mo_module_name.group(2).split(",")
-                elif line.startswith(r"//"):
-                    # only commented lines
-                    comment = line.replace("//", "").strip()
-                    try:
-                        group = self.possible_groups[comment]
-                        dummy = 1
-                    except KeyError:
-                        group = None
-
-                elif re.search(r"parameter", line):
-                    # found a parameter line
-                    mo_parameter = re.search(
-                        r"parameter\s+(real|integer)\s+(\w+)\s*=\s*(\S+)", line
-                    )
-
-                    if mo_parameter is None:
-                        continue
-
-                    parameter_type = mo_parameter.group(1)
-                    parameter_name = mo_parameter.group(2)
-                    parameter_default = mo_parameter.group(3)
-
-                    parameter_default = parameter_default.replace(";", "")
-                    if parameter_type == "integer":
-                        parameter_type = int
-                        parameter_default = int(parameter_default)
-                    elif parameter_type == "real":
-                        parameter_type = float
-                        if parameter_default == "`INF":
-                            parameter_default = np.inf
-                        else:
-                            parameter_default = float(parameter_default)
-                    else:
-                        raise NotImplementedError("Type unknown")
-
-                    tuple_parameter_boundaries = re.findall(r"from\s+(\S+)", line)
-                    if tuple_parameter_boundaries:
-                        parameter_boundaries = tuple_parameter_boundaries[0].split(":")
-                        # at the moment only 1st group is used, if VA-Code with
-                        # parameter real a = 1 from 0:10 from 20:30
-                        # is analyzed this needs to be extended!
-
-                        if "(" in parameter_boundaries[0]:
-                            parameter_include_min = False
-                        else:  # else should be "[", not checked now
-                            parameter_include_min = True
-
-                        if ")" in parameter_boundaries[1]:
-                            parameter_include_max = False
-                        else:  # else should be "]", not checked now
-                            parameter_include_max = True
-
-                        if parameter_type == int:
-                            parameter_min = int(
-                                re.search(r"([-.0-9e]+)", parameter_boundaries[0]).group(1)
-                            )
-                            parameter_max = int(
-                                re.search(r"([-.0-9e]+)", parameter_boundaries[1]).group(1)
-                            )
-                        elif parameter_type == float:
-                            try:
-                                parameter_min = float(
-                                    re.search(r"([-.0-9e]+)", parameter_boundaries[0]).group(1)
-                                )
-                            except (AttributeError, ValueError):
-                                if "INF" in parameter_boundaries[0].upper():
-                                    parameter_min = -np.inf
-                                else:
-                                    raise
-                            try:
-                                parameter_max = float(
-                                    re.search(r"([-.0-9e]+)", parameter_boundaries[1]).group(1)
-                                )
-                            except (AttributeError, ValueError):
-                                if "INF" in parameter_boundaries[1].upper():
-                                    parameter_max = np.inf
-                                else:
-                                    raise
-                            # if more are added also add them to the validity checker!!
-                        else:  # is impossible, only possibilities are real or integer (see 1st RegExp)
-                            raise NotImplementedError(
-                                "This parameter type is not implemented: " + str(parameter_type)
-                            )
-                    else:
-                        if parameter_type == float:
-                            parameter_min = -np.inf
-                            parameter_max = np.inf
-                        elif parameter_type == int:  # inf not possible in integer...
-                            parameter_min = np.iinfo(int).min
-                            parameter_max = np.iinfo(int).max
-                        else:
-                            raise NotImplementedError()
-                        parameter_include_min = True
-                        parameter_include_max = True
-
-                    tuple_parameter_excludes = re.findall(r"exclude\s+([0-9:.]+)", line)
-                    # at the moment only 1st group is used, if VA-Code with
-                    # parameter integer a = 1 from -1:2 exclude 0 exclude 1
-                    # parameter integer a = 1 from -1:2 exclude 0:1
-                    # is analyzed this needs to be extended!
-
-                    search_unit = re.search(r"unit\s*=\s*\"(.+?)\"", line)
-                    if search_unit:
-                        # convert from VA to pint...
-                        unit = unit_converter[search_unit.group(1)]
-                    else:
-                        unit = unit_registry.dimensionless
-
-                    search_desc = re.search(
-                        r"(desc|info)\s*=\s*\"(.+?)\"", line
-                    )  # 'desc' is VA standard, 'info' is ADMS standard
-                    if search_desc:
-                        desc = search_desc.group(2)
-                    else:
-                        desc = None
-
-                    try:
-                        para = self.get(parameter_name)
-                        self.remove(parameter_name)
-                    except KeyError:
-                        para = McParameter(
-                            parameter_name, value=parameter_default, value_type=parameter_type
-                        )
-
-                    para.val_type = parameter_type
-                    para.max = parameter_max
-                    para.min = parameter_min
-                    para.inc_max = parameter_include_max
-                    para.inc_min = parameter_include_min
-                    para.exclude = None
-                    #     warnings.warn('The group of the parameter {:s} is unknown from the VA-File'.format(para))
-                    # else:
-                    if group is not None:
-                        para.group = group
-
-                    if desc is not None:
-                        para.description = desc
-
-                    if unit is not None:
-                        para.unit = unit
-                    if tuple_parameter_excludes:  # just assume it is the type parameter...
-                        para.exclude = [
-                            parameter_type(exclude) for exclude in tuple_parameter_excludes
-                        ]
-
-                    paras_new.append(para)
-                    # if para in self:
-                    #     self.set(para)
-                    # else:
-                    #     self.add(para)
-
-        if remove_old_parameters:
-            self._paras = []  # remove the old parameters fast...
-
-        for para in paras_new:
-            self.add(para, update=False)
-
-        self.update_values()
+        self.op_vars = vae_module.op_vars
 
     def info_json(self, save_va_code=True, compress_va_code=False, **kwargs):
         """Returns a dict with serializeable content for the json file to create. Add the info about the concrete subclass to create here!
 
         Parameters
         ----------
         save_va_code : {True, False}, optional
@@ -555,14 +387,15 @@
 
         info_dict["nodes_list"] = self.nodes_list
         info_dict["default_subckt_name"] = self.default_subckt_name
         info_dict["default_module_name"] = self.default_module_name
         info_dict["version"] = self.version
         info_dict["pdk_path"] = self.pdk_path
         info_dict["pdk_corner"] = self.pdk_corner
+        info_dict["op_vars"] = self.op_vars
 
         if save_va_code and self.va_codes is not None:
             info_dict["va_codes"] = self.va_codes.export_dict(compressed_code=compress_va_code)
 
         return info_dict
 
     @classmethod
@@ -668,22 +501,14 @@
                 # class, version and parameters equal is enough in most cases!
                 return self.eq_paras(other)
             else:
                 return False
 
         return NotImplemented
 
-    def load_model(self, path_to_file, force=True):
-        """deprecated method, will be removed soon. See load_model_parameters for documentation."""
-        warnings.warn(
-            "load_model is deprecated and will be renamed in future major releases to load_model_parameters.\n",
-            category=DeprecationWarning,
-        )
-        self.load_model_parameters(path_to_file, force=force)
-
     def load_model_parameters(self, path_to_file, force=True):
         """Loads the model from a file
 
         The loading method is determined according to the file ending (last 3 characters!!)
         Possible is "mcp" (see save_model), "txt" or "mat" (planned)
 
         Parameters
@@ -722,15 +547,15 @@
             str_modelcard = path_to_file.read_text()
 
             # split it
             re_object = re.findall(r"[a-zA-Z0-9]+\s*=\s*\S+", str_modelcard)
 
             for param_value in re_object:
                 param_value = param_value.split("=")
-                modcard.append((param_value.strip(), float(param_value[1].strip())))
+                modcard.append((param_value[0].strip(), float(param_value[1].strip())))
         elif file_ending == ".lib" or file_ending == "":
             logging.info("Loading model parameters from a TRADICA lib-File: %s", str(path_to_file))
 
             modcard = []
             str_lib = path_to_file.read_text()
 
             # get the model part
@@ -775,15 +600,15 @@
                 "Was not able to load parameters from given file!\nGiven was: " + str(path_to_file)
             )
 
         if modcard is None:
             raise IOError("Loading from file did not work!")
 
         if isinstance(modcard, list):
-            for (parameter_name, parameter_value) in modcard:
+            for parameter_name, parameter_value in modcard:
                 try:
                     # do not reset the limits if parameter is already in modelcard
                     self.set_values({parameter_name: parameter_value}, force=force)
                 except KeyError:
                     self.add(McParameter(parameter_name, value=parameter_value))
                 except ValueError:
                     # if force==False and parameter value is out of bounds -> do not set the value...
@@ -805,15 +630,15 @@
                     para.group = None
 
                 try:
                     self.set(para)
                 except KeyError:
                     self.add(para)
         elif isinstance(modcard, dict):
-            for (parameter_name, parameter_value) in modcard.items():
+            for parameter_name, parameter_value in modcard.items():
                 if not parameter_name.startswith("__"):
                     try:
                         # do not reset the limits if parameter is already in modelcard
                         self.set_values({parameter_name: parameter_value}, force=force)
                     except KeyError:
                         self.add(McParameter(parameter_name, value=parameter_value))
                     except ValueError:
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/naming.py` & `DMT_core-2.0.0/DMT/core/naming.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,19 +23,18 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 
 from __future__ import annotations
 import copy
 import numpy as np
 import warnings
 from typing import List, Union, Set, FrozenSet
+from pint import Unit
 from pint.formatting import siunitx_format_unit
-from more_itertools import unique_everseen
 from DMT.config import DATA_CONFIG
 from DMT.core import Singleton, unit_registry
-import pint
 
 UNIT_PREFIX = {
     1e-12: r"\tera",
     1e-9: r"\giga",
     1e-6: r"\mega",
     1e-3: r"\kilo",
     1: r"",
@@ -47,15 +46,15 @@
 }
 UNIT_PREFIX_MIX = {
     "J": {  # current density-> they are all over the place :/
         1e-9: r"\milli\ampere\per\square\micro\meter",
         1e-6: r"\micro\ampere\per\square\micro\meter",
         1e-3: r"\milli\ampere\per\square\micro\meter",
         1e-0: r"\ampere\per\square\micro\meter",
-        1e+3: r"\milli\ampere\per\square\micro\meter",
+        1e3: r"\milli\ampere\per\square\micro\meter",
     },
     "F": {
         1: r"\volt\per\meter",
         1e-5: r"\kilo\volt\per\centi\meter",
     },  # field
 }
 UNIT_PREFIX_DENOMINATOR = {
@@ -312,15 +311,18 @@
         """Generates a SpecifierStr from a string if the string was generated using :meth:`~DMT.core.specifiers.SpecifierStr.string_to_save`."""
         if string.startswith("$"):  # SpecifierStr
             splitted = string[1:].split("#")
             spec = splitted[0]
             splitted = splitted[1].split("!")
 
             nodes = splitted[0].split("?")
-            sub_specifiers = splitted[1].split("|")
+            try:
+                sub_specifiers = splitted[1].split("|")
+            except IndexError:
+                sub_specifiers = None
             return SpecifierStr(spec, *nodes, sub_specifiers=sub_specifiers)
         else:  # it was just a regular str
             return string
 
     def __add__(
         self: SpecifierStr, other: Union[SpecifierStr, str, list[Union[str, SpecifierStr]]]
     ) -> SpecifierStr:
@@ -404,15 +406,15 @@
 
         # return str(other) in str(self)
         return False
 
     def __hash__(self):
         return hash(str(self))
 
-    def get_pint_unit(self) -> pint.Unit:
+    def get_pint_unit(self) -> Unit:
         """Declaration of function, to be set later
 
         Returns
         -------
         pint.UnitRegistry
             [description]
 
@@ -434,26 +436,28 @@
         Raises
         ------
         NotImplementedError
             [description]
         """
         raise NotImplementedError
 
-    def to_tex(self) -> str:
-        """Declaration of function, to be set later
+    def to_tex(self, subscript="", superscript="") -> str:
+        """Return a Tex representation of this specifier. If subscript is not None the string in subscript will be appended. If superscript is not None, a superscript will be added.
+
+        Parameters
+        ----------
+        subscript : str
+            Subscript to add to the specifier's Tex representation
+        superscript : str
+            Superscript to add to the specifier's Tex representation
 
         Returns
         -------
-        str
-            [description]
-
-        Raises
-        ------
-        NotImplementedError
-            [description]
+        tex : str
+                A Tex representation fo the specifier.
         """
         raise NotImplementedError
 
 
 class GlobalObj(object):
     """A simple class used to store class variables that are global. Also one can iterate over the class attributes in a sorted way."""
 
@@ -478,15 +482,14 @@
         self._MEMBERS = sorted(members, key=len, reverse=True)
 
 
 #############################################
 # HOLY DEFINITION OF DMT NAMING CONVENTIONS #
 #############################################
 class _sub_specifiers(GlobalObj, metaclass=Singleton):
-
     PERIMETER = SpecifierStr("", sub_specifiers="PERI")
     AREA = SpecifierStr("", sub_specifiers="AREA")
     LENGTH = SpecifierStr("", sub_specifiers="LENGTH")
     WIDTH = SpecifierStr("", sub_specifiers="WIDTH")
     CORNER = SpecifierStr("", sub_specifiers="CORNER")
     FORCED = SpecifierStr("", sub_specifiers="FORCED")
     AC_BASE = SpecifierStr("", sub_specifiers="AC_BASE")
@@ -494,25 +497,27 @@
     AC_GATE = SpecifierStr("", sub_specifiers="AC_GATE")
     AC_DRAIN = SpecifierStr("", sub_specifiers="AC_DRAIN")
     AC = SpecifierStr("", sub_specifiers="AC")
     REAL = SpecifierStr("", sub_specifiers="REAL")
     IMAG = SpecifierStr("", sub_specifiers="IMAG")
     MAG = SpecifierStr("", sub_specifiers="MAG")
     PHASE = SpecifierStr("", sub_specifiers="PHASE")
+    DELTA = SpecifierStr("", sub_specifiers="DELTA")
     NOISE = SpecifierStr("", sub_specifiers="NOISE")
     QUASISTATIC = SpecifierStr("", sub_specifiers="QUASISTATIC")
     JUNCTION = SpecifierStr("", sub_specifiers="JUNCTION")
     MINORITY = SpecifierStr("", sub_specifiers="MINORITY")
     MAJORITY = SpecifierStr("", sub_specifiers="MAJORITY")
     ELECTRONS = SpecifierStr("", sub_specifiers="ELECTRONS")
     HOLES = SpecifierStr("", sub_specifiers="HOLES")
     CHANNEL = SpecifierStr("", sub_specifiers="CHANNEL")
     MAX = SpecifierStr("", sub_specifiers="MAX")
     MIN = SpecifierStr("", sub_specifiers="MIN")
     MID = SpecifierStr("", sub_specifiers="MID")
+    MEAN = SpecifierStr("", sub_specifiers="MEAN")
     TRAPS = SpecifierStr("", sub_specifiers="TRAPS")
     YDIR = SpecifierStr("", sub_specifiers="YDIR")
     XDIR = SpecifierStr("", sub_specifiers="XDIR")
     ZDIR = SpecifierStr("", sub_specifiers="ZDIR")
 
     def add_members(self, members):
         for name, value in members:
@@ -526,18 +531,20 @@
 class _specifiers(GlobalObj, metaclass=Singleton):
     # Only Natural Quantities here
     VOLTAGE = SpecifierStr("V")
     FIELD = SpecifierStr("F")
     VELOCITY = SpecifierStr("VELO")
     GRADING = SpecifierStr("GRADING")
     RESISTANCE = SpecifierStr("R")
+    CONDUCTANCE = SpecifierStr("G")
     POWER = SpecifierStr("P")
     CURRENT = SpecifierStr("I")
     CAPACITANCE = SpecifierStr("C")
     CHARGE = SpecifierStr("Q")
+    CHARGE_DENSITY = SpecifierStr("Q''")
     INDUCTANCE = SpecifierStr("L")
     TEMPERATURE = SpecifierStr("TEMP")
     TIME = SpecifierStr("TIME")
     FREQUENCY = SpecifierStr("FREQ")
     VOLTAGE = SpecifierStr("V")
     ELECTRONS = SpecifierStr("N")
     CONDUCTION_BAND_EDGE = SpecifierStr("EC")
@@ -555,14 +562,15 @@
     Y = SpecifierStr("y")
     Z = SpecifierStr("z")
     ENERGY = SpecifierStr("E")
 
     # only derived quantities here
     DC_CURRENT_AMPLIFICATION = SpecifierStr("BETA")
     TRANSCONDUCTANCE = SpecifierStr("GM")
+    OUTPUT_CONDUCTANCE = SpecifierStr("GO")
     TRANSIT_FREQUENCY = SpecifierStr("F_T")
     MAXIMUM_OSCILLATION_FREQUENCY = SpecifierStr("F_MAX")
     MAXIMUM_AVAILABLE_GAIN = SpecifierStr("MAG")
     MAXIMUM_STABLE_GAIN = SpecifierStr("MSG")
     TRANSIT_TIME = SpecifierStr("TAU_F")
     UNILATERAL_GAIN = SpecifierStr("GU")
 
@@ -657,48 +665,53 @@
 
     else:
         return NotImplemented
 
 
 SpecifierStr.__add__ = add
 
+unit_converter = {
+    specifiers_ss_para.SS_PARA_Y: unit_registry.siemens,
+    specifiers_ss_para.SS_PARA_H: unit_registry.dimensionless,
+    specifiers_ss_para.SS_PARA_S: unit_registry.dimensionless,
+    specifiers.UNILATERAL_GAIN: unit_registry.dimensionless,
+    specifiers.VOLTAGE: unit_registry.volt,
+    specifiers.CAPACITANCE: unit_registry.farad,
+    specifiers.CHARGE: unit_registry.coulomb,
+    specifiers.CHARGE_DENSITY: unit_registry.coulomb_per_square_meter,
+    specifiers.FREQUENCY: unit_registry.hertz,
+    specifiers.CURRENT: unit_registry.ampere,
+    specifiers.CURRENT_DENSITY: unit_registry.ampere_per_square_meter,
+    specifiers.TEMPERATURE: unit_registry.kelvin,
+    specifiers.RESISTANCE: unit_registry.ohm,
+    specifiers.CONDUCTANCE: unit_registry.siemens,
+    specifiers.POWER: unit_registry.watt,
+    specifiers.TIME: unit_registry.second,
+    specifiers.X: unit_registry.meter,
+    specifiers.TRANSIT_FREQUENCY: unit_registry.hertz,
+    specifiers.MAXIMUM_OSCILLATION_FREQUENCY: unit_registry.hertz,
+    specifiers.TRANSIT_TIME: unit_registry.second,
+    specifiers.TRANSCONDUCTANCE: unit_registry.siemens,
+    specifiers.ENERGY: unit_registry.volt,
+    specifiers.FIELD: unit_registry.volt / unit_registry.meter,
+    specifiers.DC_CURRENT_AMPLIFICATION: unit_registry.dimensionless,
+    specifiers.MAXIMUM_STABLE_GAIN: unit_registry.dimensionless,
+    specifiers.NET_DOPING: 1 / unit_registry.meter / unit_registry.meter / unit_registry.meter,
+    specifiers.ACCEPTORS: 1 / unit_registry.meter / unit_registry.meter / unit_registry.meter,
+    specifiers.DONNORS: 1 / unit_registry.meter / unit_registry.meter / unit_registry.meter,
+    specifiers.ELECTRONS: 1 / unit_registry.meter / unit_registry.meter / unit_registry.meter,
+    specifiers.HOLES: 1 / unit_registry.meter / unit_registry.meter / unit_registry.meter,
+}  # type: dict[SpecifierStr, Unit]
 
-def get_pint_unit(self) -> pint.Unit:
+
+def get_pint_unit(self) -> Unit:
     """Return the DMT base unit of this specifier as a pint unit"""
     if sub_specifiers.PHASE.sub_specifiers <= self.sub_specifiers:
         return unit_registry.degree
 
-    unit_converter = {
-        specifiers_ss_para.SS_PARA_Y: unit_registry.siemens,
-        specifiers_ss_para.SS_PARA_H: unit_registry.dimensionless,
-        specifiers_ss_para.SS_PARA_S: unit_registry.dimensionless,
-        specifiers.UNILATERAL_GAIN: unit_registry.dimensionless,
-        specifiers.VOLTAGE: unit_registry.volt,
-        specifiers.CAPACITANCE: unit_registry.farad,
-        specifiers.CHARGE: unit_registry.coulomb,
-        specifiers.FREQUENCY: unit_registry.hertz,
-        specifiers.CURRENT: unit_registry.ampere,
-        specifiers.CURRENT_DENSITY: unit_registry.ampere_per_square_meter,
-        specifiers.TEMPERATURE: unit_registry.kelvin,
-        specifiers.RESISTANCE: unit_registry.ohm,
-        specifiers.POWER: unit_registry.watt,
-        specifiers.TIME: unit_registry.second,
-        specifiers.X: unit_registry.meter,
-        specifiers.TRANSIT_FREQUENCY: unit_registry.hertz,
-        specifiers.MAXIMUM_OSCILLATION_FREQUENCY: unit_registry.hertz,
-        specifiers.TRANSIT_TIME: unit_registry.second,
-        specifiers.TRANSCONDUCTANCE: unit_registry.siemens,
-        specifiers.ENERGY: unit_registry.volt,
-        specifiers.FIELD: unit_registry.volt / unit_registry.meter,
-        specifiers.DC_CURRENT_AMPLIFICATION: unit_registry.dimensionless,
-        specifiers.MAXIMUM_STABLE_GAIN: unit_registry.dimensionless,
-        specifiers.NET_DOPING: 1 / unit_registry.meter / unit_registry.meter / unit_registry.meter,
-        specifiers.ACCEPTORS: 1 / unit_registry.meter / unit_registry.meter / unit_registry.meter,
-        specifiers.DONNORS: 1 / unit_registry.meter / unit_registry.meter / unit_registry.meter,
-    }  # type: dict[SpecifierStr, pint.Unit]
     try:
         return unit_converter[self.specifier]
     except KeyError as err:
         raise IOError(
             "DMT -> Naming: no unit defined for specifier " + self.specifier + "."
         ) from err
 
@@ -710,14 +723,15 @@
     """Can be generalized using the _specifiers class."""
     descriptor = {
         specifiers.CURRENT: "current",
         specifiers.CURRENT_DENSITY: "current density",
         specifiers.CAPACITANCE: "capacitance",
         specifiers.VOLTAGE: "voltage",
         specifiers.RESISTANCE: "resistance",
+        specifiers.CONDUCTANCE: "conductance",
         specifiers.POWER: "power",
         specifiers.ENERGY: "energy",
     }
     return descriptor[self.specifier]
 
 
 SpecifierStr.get_descriptor = get_descriptor
@@ -776,20 +790,22 @@
         tex = r"f_{\mathrm{max" + subscript + r"}}"
     elif self.specifier == specifiers.TRANSIT_TIME:
         tex = r"\tau_{\mathrm{f" + subscript + r"}}"
     elif self.specifier == specifiers.FREQUENCY:
         tex = r"f_{\mathrm{" + subscript + r"}}"
     elif self.specifier == specifiers.TRANSCONDUCTANCE:
         tex = r"g_{\mathrm{m," + subscript + r"}}"
+    elif self.specifier == specifiers.OUTPUT_CONDUCTANCE:
+        tex = r"g_{\mathrm{o," + subscript + r"}}"
     elif self.specifier == specifiers.TEMPERATURE:
         tex = r"T_{\mathrm{" + subscript + r"}}"
     elif self.specifier == specifiers.NET_DOPING:
         tex = r"N_{\mathrm{net}}"
     elif self.specifier == specifiers.ACCEPTORS:
-        tex = r"N_{\mathrm{A}}"
+        tex = r"N_{\mathrm{A}}col_ib"
     elif self.specifier == specifiers.DONNORS:
         tex = r"N_{\mathrm{D}}"
     elif self.specifier == specifiers.TIME:
         if subscript:
             tex = r"t_{\mathrm{" + subscript + r"}}"
         else:
             tex = r"t"
@@ -815,25 +831,29 @@
         tex = r"\Re\{" + tex + r"\}"
     elif sub_specifiers.IMAG.sub_specifiers <= self.sub_specifiers:
         tex = r"\Im\{" + tex + r"\}"
     elif sub_specifiers.MAG.sub_specifiers <= self.sub_specifiers:
         tex = r"|" + tex + r"|"
     elif sub_specifiers.PHASE.sub_specifiers <= self.sub_specifiers:
         tex = r"\angle\{" + tex + r"\}"
+    elif sub_specifiers.DELTA.sub_specifiers <= self.sub_specifiers:
+        tex = r"\Delta " + tex
+    elif sub_specifiers.MEAN.sub_specifiers <= self.sub_specifiers:
+        tex = r"\overline{" + tex + r"}"
 
     # add specifiers that are appended to the string
-    for specifier in self.sub_specifiers:
-        if "|" + specifier in [
-            sub_specifiers.PERIMETER,
-            sub_specifiers.AREA,
-            sub_specifiers.CORNER,
-            sub_specifiers.LENGTH,
-            sub_specifiers.WIDTH,
-        ]:
-            tex = tex + "|" + specifier
+    sub_spec_append = (
+        sub_specifiers.PERIMETER.sub_specifiers
+        | sub_specifiers.AREA.sub_specifiers
+        | sub_specifiers.CORNER.sub_specifiers
+        | sub_specifiers.LENGTH.sub_specifiers
+        | sub_specifiers.WIDTH.sub_specifiers
+    )
+    for append in self.sub_specifiers & sub_spec_append:
+        tex = tex + "|" + append
 
     return tex
 
 
 SpecifierStr.to_tex = to_tex
 
 
@@ -1010,27 +1030,31 @@
         return string
     else:
         return specifier
 
 
 # a dict that holds natural scaling for a few specifiers. Convenient for Plotting.
 natural_scales = {
+    specifiers.TIME: 1e12,  # ps
     specifiers.VOLTAGE: 1,
     specifiers.MAXIMUM_STABLE_GAIN: 1,
     specifiers.CURRENT: 1e3,  # mA
     specifiers.CURRENT_DENSITY: 1e3 / (1e6 * 1e6),  # mA/um^2
     specifiers.MAXIMUM_OSCILLATION_FREQUENCY: 1e-9,
     specifiers.TRANSCONDUCTANCE: 1,
+    specifiers.OUTPUT_CONDUCTANCE: 1,
     specifiers.TRANSIT_FREQUENCY: 1e-9,
     specifiers.CAPACITANCE: 1e15,
     specifiers.CHARGE: 1e15,
+    specifiers.CHARGE_DENSITY: 1e15 / (1e6 * 1e6),  # fF/um^2
     specifiers.SS_PARA_Y: 1e3,
     specifiers.DC_CURRENT_AMPLIFICATION: 1,
     specifiers.FREQUENCY: 1e-9,  # GHz
     specifiers.TEMPERATURE: 1,
     specifiers.X: 1e9,
     specifiers.POWER: 1e3,  # mW
     specifiers.RESISTANCE: 1,  # Ohm
+    specifiers.CONDUCTANCE: 1,  # Siemens
     specifiers.ENERGY: 1,  # eV
     specifiers.UNILATERAL_GAIN: 1,
     specifiers.NET_DOPING: 1e-6,  # 1/cm^3
 }
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/plot.py` & `DMT_core-2.0.0/DMT/core/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,22 +30,23 @@
 import numpy as np
 from pathlib import Path
 from cycler import cycler
 from colormath.color_objects import sRGBColor
 from DMT.core import natural_scales, sub_specifiers
 from DMT.external import tex_to_text, build_tex, build_svg, clean_tex_files, build_png, slugify
 
-if "PYQTGRAPH_QT_LIB" not in os.environ:  # user did not choose Backend. Try to force PySide2
-    # OLD: add PYQTGRAPH_QT_LIB environment variable.
-    # os.environ["PYQTGRAPH_QT_LIB"] = "PySide2"
-    # https://pyqtgraph.readthedocs.io/en/latest/how_to_use.html#pyqt-and-pyside
-    try:
-        import PySide2
-    except ImportError:
-        pass
+# if "PYQTGRAPH_QT_LIB" not in os.environ:
+#     # user did not choose Backend. Try to force PySide6 (best tested)
+#     try:
+#         import PySide6
+#     except ImportError:
+#         try:
+#             import PySide2
+#         except ImportError:
+#             pass
 
 try:
     import pyqtgraph
     from pyqtgraph.Qt import QtCore
 
     if hasattr(pyqtgraph, "QtWidgets"):
         pyqt_widgets = pyqtgraph.QtWidgets
@@ -128,14 +129,32 @@
 XTRACTION_INTERPOLATED = "xtraction_interpolated"
 PLOT_STYLES.append(XTRACTION_INTERPOLATED)
 XTRACTION_INTERPOLATED_COLOR = "xtraction_interpolated_color"
 PLOT_STYLES.append(XTRACTION_INTERPOLATED_COLOR)
 MIX = "mix"
 PLOT_STYLES.append(MIX)
 
+CYCLER_MARKERS = cycler(marker=[char for char in "x+v^*<>.so"])
+CYCLER_LINESTYLES = cycler(linestyle=["-", "--", "-.", ":"])
+CYCLER_COLORS = cycler(
+    color=[
+        "#006400",  # darkgreen
+        "#00008b",  # darkblue
+        "#b03060",  # maroon3
+        "#ff0000",  # red
+        "#9467bd",  # yellow -> replaced by violett/brown combo
+        "#deb887",  # curlywood
+        "#00ff00",  # lime
+        "#00ffff",  # aqua
+        "#ff00ff",  # fuchsia
+        "#6495ed",  # cornflower
+    ]
+)
+
+
 ### Translation dictionaries from matplotlib to tikz
 _DICT_MARKERS_MPL_TO_PGF = {
     ".": r"mark=*, mark options={solid, fill}, ",
     # ',',# do not know how to translate them ...
     "o": r"mark=o, mark options={solid, fill}, ",
     "ö": r"mark=*, mark options={solid, fill=black}, text mark as node=true, ",  # cheat: mark points in plots with this marker
     "v": r"mark=triangle, mark options={solid, rotate=180}, ",
@@ -425,15 +444,14 @@
         style : str
             Style for plotting of the lines. Possible are:
             'color', 'bw', 'markers_color', 'markers', 'markers_lines',
             'xtraction', 'xtraction_color', 'xtraction_interpolated', 'xtraction_interpolated_color',
         """
         markers = [char for char in "x+v^*<>.so"]
         linestyles = ["-", "--", "-.", ":"]
-        dashed = ["--"]
         # MM: replaced grey1 (#7f7f7f) with black(#) and grey2 with dark blue #1012d5. Does this cause problems?
         # MK: introduced completely new palette from https://mokole.com/palette.html (settings: 10 colors, 1% min, 80% max, 15000 loops, score 65.49)
         colors = [
             # "#1f77b4",
             # "#ff7f0e",
             # "#2ca02c",
             # "#d62728",
@@ -460,15 +478,15 @@
                 cycler("color", ["black"]) * cycler("linestyle", "-") * cycler("marker", markers)
             )
 
         elif style == BLACK_SOLID:
             self._cycler = cycler("color", ["black"]) * cycler("linestyle", "-")
 
         elif style == BLACK_DASHED:
-            self._cycler = cycler("color", ["black"]) * cycler("linestyle", dashed)
+            self._cycler = cycler("color", ["black"]) * cycler("linestyle", "--")
 
         elif style == BLACK_LINESTYLE:
             self._cycler = cycler("color", ["black"]) * cycler("linestyle", linestyles)
 
         elif style == COLOR:
             # colors from default matplotlibrc
             self._cycler = cycler("color", colors) * cycler("linestyle", "-")
@@ -731,41 +749,51 @@
             }
         )
 
     def remove_legend(self):
         for line in self.data:
             line["label"] = None
 
-    def add_data_set_multiple_y(self, x, *y, label=None):
+    def add_data_set_multiple_y(self, x, *y, label=None, style=None):
         """Add y(x) to the plot
 
         Each data set is a tuple with five entries, no need to create a dictionary, keeps it simple
 
         Parameters
         ----------
         x : array-like
         *y : array-likes
             multiple y arrays to plot versus x
         label : str or list(str), optional
             Legend entry/ies
+        style : list(str), optional
+            List of styles
         """
         if label is None or not label:  # no or empty label
             label = []
             for _i in range(len(y)):
                 label.append(None)
         elif isinstance(label, str):
             label = [label]
 
         if len(y) != len(label):
             raise IOError(
                 "To set multiple y(x) at the same time, the number of labels must be equal to the number of y datas"
             )
 
-        for y_a, label_a in zip(y, label):
-            self.add_data_set(x, y_a, label=label_a)
+        if style is None:
+            for y_a, label_a in zip(y, label):
+                self.add_data_set(x, y_a, label=label_a)
+        else:
+            if len(y) != len(style):
+                raise IOError(
+                    "If you want to set the style manually, the number of styles must be equal to the number of y datas"
+                )
+            for y_a, label_a, style_a in zip(y, label, style):
+                self.add_data_set(x, y_a, label=label_a, style=style_a)
 
     def plot_py(
         self,
         show=True,
         font_size=None,
         allow_grid=False,
         tight_layout=True,
@@ -1013,22 +1041,22 @@
         # actual plotting of the data
         for i_line, dict_line in enumerate(self.data):
             # x and y should be numpy vectors, stable conversion is given (more tests necessary)
             x = dict_line["x"]
             y = dict_line["y"]
 
             if self.x_axis_scale == "log":
-                x = np.abs(x)
+                x = np.array(np.abs(x))
             else:
-                x = np.real(x)
+                x = np.array(np.real(x))
 
             if self.y_axis_scale == "log":
-                y = np.abs(y)
+                y = np.array(np.abs(y))
             else:
-                y = np.real(y)
+                y = np.array(np.real(y))
 
             label = dict_line["label"]
             if label is not None:
                 # workaround since siunitx is not supported yet in pandoc
                 label = tex_to_text(label)
                 # insert space after <p>, so that label is not ON the symbol
                 label = label.replace("\n", "")
@@ -1067,15 +1095,15 @@
                 x_min = np.nanmin(
                     [
                         np.nanmin(dict_line["x"])
                         for dict_line in self.data
                         if not len(dict_line["x"]) == 0
                     ]
                 )
-                x_min = 0.9 * x_min if x_min > 0 else 1.1 * x_min
+                x_min = 0.95 * x_min if x_min > 0 else 1.05 * x_min
                 x_min_set = x_min * self.x_scale
             else:
                 x_min = 0
                 x_min_set = x_min
         else:
             x_min = self.x_limits[0]
             x_min_set = x_min
@@ -1086,15 +1114,15 @@
                 x_max = np.nanmax(
                     [
                         np.nanmax(dict_line["x"])
                         for dict_line in self.data
                         if not len(dict_line["x"]) == 0
                     ]
                 )
-                x_max = 1.1 * x_max if x_max > 0 else 0.9 * x_max
+                x_max = 1.05 * x_max if x_max > 0 else 0.95 * x_max
                 # x_max = np.ceil(1.1*x_max) if x_max > 0 else np.ceil(0.9*x_max)
                 x_max_set = x_max * self.x_scale
             else:
                 x_max = 1
                 x_max_set = x_max
         else:
             x_max = self.x_limits[1]
@@ -1122,15 +1150,17 @@
                             dict_line["x"] < x_max,
                         )
                         y_min_local = np.min(dict_line["y"][y_filter])
                         y_min = np.min([y_min, y_min_local])
                     # y_min = (
                     #     np.min([np.min(dict_line["y"]) for dict_line in self.data])
                     # )
-                    y_min = 0.9 * y_min * self.y_scale if y_min > 0 else 1.1 * y_min * self.y_scale
+                    y_min = (
+                        0.95 * y_min * self.y_scale if y_min > 0 else 1.05 * y_min * self.y_scale
+                    )
                 except ValueError:
                     y_min = 0.0
                 # y_min = np.floor(0.9*y_min) if y_min > 0 else np.floor(1.1*y_min)
             else:
                 y_min = 0.0
         else:
             y_min = self.y_limits[0]
@@ -1146,15 +1176,17 @@
                             dict_line["x"] < x_max,
                         )
                         y_max_local = np.max(dict_line["y"][y_filter])
                         y_max = np.max([y_max, y_max_local])
                     # y_max = (
                     #     np.max([np.max(dict_line["y"]) for dict_line in self.data])
                     # )
-                    y_max = 1.1 * y_max * self.y_scale if y_max > 0 else 0.9 * y_max * self.y_scale
+                    y_max = (
+                        1.05 * y_max * self.y_scale if y_max > 0 else 0.95 * y_max * self.y_scale
+                    )
                 except ValueError:
                     y_max = 1.0
             else:
                 y_max = 1.0
         else:
             y_max = self.y_limits[1]
             padding = 0.0
@@ -1173,26 +1205,26 @@
 
         if self.mw_pg is not None:
             self.mw_pg.show()
 
         ## Start Qt event loop unless running in interactive mode or using pyside.
         if show:
             if sys.flags.interactive != 1 or not hasattr(pyqtgraph.Qt.QtCore, "PYQT_VERSION"):
-                pyqt_widgets.QApplication.exec_()  # type: ignore
+                pyqt_widgets.QApplication.exec()  # type: ignore
 
         if only_widget:
             return self.pw_pg
         elif qt_layout is not None:
             return qt_layout
 
     def show_pyqtgraph(self):
         """Reshows the PyQtGraph main window and startes the Qt event loop"""
         if self.mw_pg is not None:
             self.mw_pg.show()
-            pyqt_widgets.QApplication.exec_()  # type: ignore
+            pyqt_widgets.QApplication.exec()  # type: ignore
 
     def _convert_mpl_to_pyqt(self, mpl_style):
         """Returns a corresponding PyQtGraph style for a given matplotlib style.
 
         This can be very complicated as PyQtGraph directly uses a QtPen/QtBrush...
 
         Parameters
@@ -1365,32 +1397,35 @@
 
         return dict_style
 
     def save_tikz(
         self,
         directory,
         file_name=None,
-        width="\\textwidth",
+        width=None,
         height=None,
         mark_repeat=1,
         restrict=True,
         standalone=False,
         build=False,
         clean=False,
         fontsize="normalsize",
+        line_width="very thick",
         svg=False,
         png=False,
         extension=None,
         nth=1,
         mark_delta=1,
         skip_every=lambda x: x,
         n_ticks_x=None,
         n_ticks_y=None,
+        show_legend=True,
         legend_location=None,
         legend_to_name=None,
+        legend_columns=4,
         **kwargs,
     ):
         """Save plot in directory and return name of the tikz file.
 
         The name of the tikz file will be the figure attribute self.num, if not given.
 
         Parameters
@@ -1415,14 +1450,16 @@
             Create standalone tikz figure, by default False
         build : bool, optional
             Build the latex file (only possible for standalone), by default False
         clean : bool, optional
             Remove all files except the rendered picture after build, by default False
         fontsize : str, optional
             Latex fontsize, by default 'normalsize'.
+        line_width : str, optional
+            Pgfplots line width, by default 'very thick'.
         svg : bool, optional
             Build the figure to svg (suited for FrameMaker), by default False
         png : bool, optional
             Build the figure to png.
         extension : str, optional
             Extension for the saved tikz file, if not given extension == "tex".
         skip_every : callable, optional
@@ -1453,41 +1490,60 @@
         legend_pos = {
             "lower left": "at={(0.02,0.02)}, anchor=south west,",
             "upper left": "at={(0.02,0.98)}, anchor=north west,",
             "lower right": "at={(0.98,0.02)}, anchor=south east,",
             "upper right": "at={(0.98,0.98)}, anchor=north east,",
             "upper right outer": "at={(1.02,1.00)}, anchor=north west,",
             "right mid": "at={(0.98,0.70)}, anchor=north east,",
+            "below": f"at={{(0.5,-0.18)}}, anchor=north, legend columns={legend_columns},",
+            "above": f"at={{(0.5,1.03)}}, anchor=south, legend columns={legend_columns},",
             None: "at={(0.98,0.98)}, anchor=north east,",
         }
         if legend_location is None:
             legend_location = legend_pos[self.legend_location]
         else:
             legend_location = legend_pos[legend_location]
+
         if standalone:
             str_tikz_picture = (
                 "\\begin{tikzpicture}[font=\\"
                 + fontsize
                 + "]\n"
-                + "\\pgfplotsset{every axis/.append style={ultra thick},compat=1.5},\n"
+                + "\\pgfplotsset{every axis/.append style={"
+                + line_width
+                + "},compat=1.5},\n"
             )
         else:  # if this figure is used in other tex documents, the axis are trimed so that figures with different y-labels and ticks get displayed nicely
             str_tikz_picture = (
                 "\\begin{tikzpicture}[font=\\"
                 + fontsize
-                + ",trim axis left, trim axis right]\n"
-                + "\\pgfplotsset{every axis/.append style={very thick},compat=1.5},\n"
+                + ",trim axis left, trim axis right,tight background]\n"
+                + "\\pgfplotsset{every axis/.append style={"
+                + line_width
+                + "},compat=1.5},\n"
             )
         str_height = "" if height is None else "height=" + height + ",\n"
         if width is None:
             str_width = ""
         elif width == "\\textwidth":
             str_width = "width=0.951*\\figurewidth,\n"
         else:
             str_width = "width=" + width + ",\n"
+
+        if self.pw_pg is not None:
+            if self.pw_pg.plotItem.ctrl.logXCheck.isChecked():
+                self.x_axis_scale = "log"
+            else:
+                self.x_axis_scale = "linear"
+
+            if self.pw_pg.plotItem.ctrl.logYCheck.isChecked():
+                self.y_axis_scale = "log"
+            else:
+                self.y_axis_scale = "linear"
+
         str_x_log = "" if self.x_axis_scale == "linear" else "xmode=log,\n"
         str_y_log = "" if self.y_axis_scale == "linear" else "ymode=log,\n"
 
         if self.legend_frame:
             str_legend_frame = ""
         else:
             str_legend_frame = ", fill=none, draw=none"
@@ -1695,14 +1751,18 @@
             print("using pgf")
 
         if legend_to_name is None:
             legend_to_name = ""
         else:
             legend_to_name = "legend to name={},\n".format(legend_to_name)
 
+        str_shift_labels = ""
+        if fontsize == "normalsize":
+            str_shift_labels = "xlabel shift = -5 pt,\n ylabel shift = -5 pt,\n"
+
         ### header
         str_axis = (
             "\n\\begin{axis}[scale only axis,ytick pos=left,\n"
             # + fontsize+",\n"
             + str_width
             + str_height
             + "xlabel={"
@@ -1712,14 +1772,15 @@
             + self.y_label
             + "},\n"
             + str_x_log
             + str_y_log
             + str_limits
             + str_x_ticks
             + str_y_ticks
+            + str_shift_labels
             + "xmajorgrids,\n"
             + "enlargelimits=false,\n"
             + "scaled ticks=true,\n"
             + "ymajorgrids,\n"
             + "x tick style={color=black},\n"
             + "y tick style={color=black},\n"
             + "x grid style={white!69.01960784313725!black},\n"
@@ -1737,24 +1798,24 @@
             + "]\n"
         )
 
         ### Lines
         str_lines = ""
         colors = []
         # try:
-        #     mark_delta = np.int(mark_repeat/len(self.data[::nth]))
+        #     mark_delta = int(mark_repeat/len(self.data[::nth]))
         # except ZeroDivisionError:
         #     mark_delta = 1
         #     print("DMT->plot->{:s}: Plot has no data, generating axis anyways.".format(self.name))
 
         for nr_line, dict_line in enumerate(self.data[::nth]):
             if len(dict_line["x"]) == 0:
                 continue
             str_addplot, colors = self._tikz_addplot(
-                dict_line, nr_line, colors=colors, mark_delta=mark_delta
+                dict_line, nr_line, colors=colors, mark_delta=mark_delta, show_label=show_legend
             )
             if str_addplot is not None:
                 str_lines += str_addplot
 
         ### footer
         str_footer = "\\end{axis}\n\n\\end{tikzpicture}\n"
 
@@ -1830,15 +1891,15 @@
             if clean:
                 clean_tex_files(
                     directory, file_name.replace(ext_file, ""), keep=(ending_to_keep, ".tex")
                 )
 
         return file_name
 
-    def _tikz_addplot(self, dict_line, nr_line, colors=None, mark_delta=None):
+    def _tikz_addplot(self, dict_line, nr_line, colors=None, mark_delta=None, show_label=True):
         """Transforms a line into a pgfplots addplot command.
 
         Parameters
         ----------
         dict_line : (x_data, y_data, label, style)
             See the description in Plot.add_data .
         nr_line : int
@@ -1864,15 +1925,15 @@
         if style is None:
             opts_style, colors = self._get_pgfplotset_for_line_nr(nr_line, colors)
         else:
             opts_style, colors = self._convert_mpl_to_pfg(style, colors)
 
         if "mark phase" not in opts_style:
             # Markus: what was this?
-            # mark_phase = np.int(nr_line)*mark_delta if (mark_delta is not None) else np.int(1)
+            # mark_phase = int(nr_line)*mark_delta if (mark_delta is not None) else int(1)
             opts_style += "mark phase={:d}, ".format(mark_delta)
 
         if line_width is not None:
             opts_style += "line width={0:f}pt, ".format(line_width)
 
         if mark_size is not None:
             opts_style += "mark size={0:f}pt, ".format(mark_size)
@@ -1903,16 +1964,18 @@
                     + ". Check that the data are 1D arrays."
                 )
 
         str_addplot += "};\n"
 
         if label is None:
             str_addplot += "% \\addlegendentry{}\n"
-        else:
+        elif show_label:
             str_addplot += "\\addlegendentry{" + label + "}\n"
+        else:
+            str_addplot += "% \\addlegendentry{" + label + "}\n"
 
         return str_addplot, colors
 
     def _convert_mpl_to_pfg(self, mpl_style, colors):
         """Converts a matplotlib style text to a valid pgfplots options string."""
         pgf_color = "color=black, "
         pgf_line = "only marks, "
@@ -1924,15 +1987,15 @@
                     if mpl_color.startswith("#"):
                         try:
                             # is it already there?
                             pgf_color = "color=color" + str(colors.index(mpl_color)) + ", "
                         except ValueError:
                             # if not add it
                             pgf_color = "color=color" + str(len(colors)) + ", "
-                            colors.append(colors)
+                            colors.append(mpl_color)
                     else:
                         pgf_color = "color=" + _DICT_COLORS_MPL[mpl_color] + ", "
 
                     mpl_style = mpl_style.replace(mpl_color, "")
                     break
 
         if mpl_style:
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/plot_2yaxis.py` & `DMT_core-2.0.0/DMT/core/plot_2yaxis.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
 class Plot2YAxis(object):
     """Provides a plot with 2 y-Axes
 
     WARNING: Legend does not work with cyclers :(. You have to set the styles manually.
 
     """
 
-    def __init__(self, name, plot_left, plot_right, legend_location="upper right"):
+    def __init__(self, name, plot_left, plot_right, legend_location=None):
         self.name = name
 
         # do not check anything here!
 
         self.plot_left = plot_left
         self.plot_right = plot_right
 
@@ -306,14 +306,16 @@
         # legend ( only once ! )
         if self.legend_location in [
             "upper right outer",
             "right mid",
         ]:  # not supported in matplotlib
             self.ax_left.legend(loc="upper right", frameon=self.legend_frame)
             self.ax_right.legend(loc="upper right", frameon=self.legend_frame)
+        elif self.legend_location is None:
+            pass  # do nothing, legend location is set in the child plots.
         else:
             self.ax_left.legend(loc=self.legend_location, frameon=self.legend_frame)
             self.ax_right.legend(loc=self.legend_location, frameon=self.legend_frame)
 
         if allowGrid:
             # Don't allow the axis to be on top of your data
             self.ax_left.set_axisbelow(True)
@@ -341,23 +343,27 @@
     def show_pyqtgraph(self, *args, **kwargs):
         self.plot_left.show_pyqtgraph(*args, **kwargs)
 
     def save_tikz(
         self,
         directory,
         file_name=None,
-        width="\\textwidth",
+        width=None,
         fontsize="normalsize",
+        line_width="very thick",
         height=None,
         mark_repeat=1,
         extension=None,
         restrict_left=True,
         restrict_right=True,
         hide_second_ticks=False,
         hide_second_axis=False,
+        show_legend=True,
+        legend_location=None,
+        legend_columns=4,
         standalone=False,
         build=False,
         clean=False,
         svg=False,
         png=False,
     ):
         """Save plot in directory and return name of the tikz file. The name of the tikz file will be the figure attribute self.name if not given.
@@ -388,31 +394,40 @@
         num_old_right = self.plot_right.num
 
         self.plot_left.name = name_old_left + "_tmp"
         self.plot_left.num = num_old_left + "_tmp"
         self.plot_right.name = name_old_right + "_tmp"
         self.plot_right.num = num_old_right + "_tmp"
 
+        if legend_location is None:
+            legend_location = self.legend_location
+
         file_tikz_left = self.plot_left.save_tikz(
             directory,
             width=width,
             height=height,
             mark_repeat=mark_repeat,
             standalone=standalone,
             restrict=restrict_left,
             extension=extension,
+            show_legend=show_legend,
+            legend_location=legend_location,
+            legend_columns=legend_columns,
         )
         file_tikz_right = self.plot_right.save_tikz(
             directory,
             width=width,
             height=height,
             mark_repeat=mark_repeat,
             standalone=standalone,
             restrict=restrict_right,
             extension=extension,
+            show_legend=show_legend,
+            legend_location=legend_location,
+            legend_columns=legend_columns,
         )
 
         # open, read and delete the tikz files
         path_file_left = directory / file_tikz_left
         str_tikz_left = path_file_left.read_text()
         path_file_left.unlink()
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/plot_smith.py` & `DMT_core-2.0.0/DMT/core/plot_smith.py`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/core/sim_con.py` & `DMT_core-2.0.0/DMT/core/sim_con.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,42 +154,66 @@
         if force:
             logging.info("Simulations forced!")
             sims_to_simulate = self.sim_list
             run_sims = True
 
         with Parallel(n_jobs=n_jobs, verbose=10) as parallel:
             if not force:
-                # check which simulations really need to be run
-                n_tot = len(self.sim_list)
-                if parallel_read:
-                    print("Checking which simulations need to be run in parallel:")
-                    sims_checked = parallel(
-                        delayed(_check_simulation_needed)(i_sim, n_tot, **sim)
-                        for i_sim, sim in enumerate(self.sim_list)
-                    )
-                else:
-                    print("Checking which simulations need to be run:")
-                    # parallel not working with VAE modelcard currently since get_circuit is monkey patched
-                    sims_checked = [
-                        _check_simulation_needed(i_sim, n_tot, **sim)
-                        for i_sim, sim in enumerate(self.sim_list)
-                    ]
+                # check which simulations are already loaded into dut.data or saved as a database file
+                n_tot = 0
+                for sim in self.sim_list:
+                    dut = sim["dut"]
+                    sweep = sim["sweep"]
+                    dut_name = dut.name + str(dut.get_hash())
+                    sim_name = sweep.name + "_" + sweep.get_hash()
+                    if dut.check_existence_sweep(sweep):
+                        print(
+                            f"Simulation of DuT {dut_name} with sweep {sim_name} loaded from database.",
+                        )
+                        logging.info(
+                            "Simulation of DuT %s with sweep %s loaded from database.",
+                            dut_name,
+                            sim_name,
+                        )
+                        sim["sweep_exists"] = True
+                    else:
+                        n_tot += 1
+                        sim["sweep_exists"] = False
 
-                print_progress_bar(n_tot, n_tot, prefix="Finish", length=50)
-                print("\n")  # new line after the progress bar
+                # remove all simulations which are already exist
+                self.sim_list = [sim for sim in self.sim_list if not sim["sweep_exists"]]
 
                 sims_to_simulate = []
-                # add data to the duts and filter simulations to do
-                for sim_to_do, sim_checked in zip(
-                    self.sim_list, sims_checked
-                ):  # as we are keeping the order, we can copy the data over
-                    if sim_checked is None:
-                        sims_to_simulate.append(sim_to_do)
+                if n_tot > 0:
+                    # check which simulations are already run in the past but not imported
+                    if parallel_read:
+                        print("Checking which simulations need to be run in parallel:")
+                        sims_checked = parallel(
+                            delayed(_check_simulation_needed)(i_sim, n_tot, **sim)
+                            for i_sim, sim in enumerate(self.sim_list)
+                        )
                     else:
-                        sim_to_do["dut"].data.update(sim_checked)
+                        print("Checking which simulations need to be run:")
+                        # parallel not working with VAE modelcard currently since get_circuit is monkey patched
+                        sims_checked = [
+                            _check_simulation_needed(i_sim, n_tot, **sim)
+                            for i_sim, sim in enumerate(self.sim_list)
+                        ]
+
+                    print_progress_bar(n_tot, n_tot, prefix="Finish", length=50)
+                    print("\n")  # new line after the progress bar
+
+                    # add dalta to the duts and filter simuations to do
+                    for sim_to_do, sim_checked in zip(
+                        self.sim_list, sims_checked
+                    ):  # as we are keeping the order, we can copy the data over
+                        if sim_checked is None:
+                            sims_to_simulate.append(sim_to_do)
+                        else:
+                            sim_to_do["dut"].data.update(sim_checked)
 
                 run_sims = bool(sims_to_simulate)  # will be False if list is empty
 
             # remote simulations ?
             if any([sim for sim in sims_to_simulate if sim["dut"].simulate_on_server]):
                 self.create_ssh_client()
 
@@ -308,16 +332,19 @@
         # delete possible old directories:
         for sim_to_zip in sims_to_zip:
             sim_folder = sim_to_zip["dut"].get_sim_folder(sim_to_zip["sweep"])
             dut_folder = sim_folder.parts[-2]
             sweep_folder = sim_folder.parts[-1]
             commands.append("rm -rf " + str(sim_path_on_server / dut_folder / sweep_folder))
 
+        # https://stackoverflow.com/questions/34181078/execute-command-and-wait-for-it-to-finish-with-python-paramiko?noredirect=1&lq=1
         for command in commands:
-            self.ssh_client.exec_command(command)
+            _stdin, stdout, _stderr = self.ssh_client.exec_command(command)
+            stdout.channel.set_combine_stderr(True)
+            _output = stdout.readlines()
 
         with NamedTemporaryFile() as path_zip:  # dut.get_sim_folder(sweep).relative_to(dut.sim_dir)
             with ZipFile(path_zip, "w") as zip_ref:
                 for sim_to_zip in sims_to_zip:
                     add_to_zip(
                         sim_to_zip["dut"].get_sim_folder(sim_to_zip["sweep"]),
                         sim_to_zip["dut"].sim_dir,
@@ -382,15 +409,15 @@
             try:
                 self.scp_client.get(
                     str(DATA_CONFIG["server"]["simulation_path"] / dut_folder / sweep_folder)
                     + ".zip",
                     local_path=str(root),
                 )
             except (SCPException, paramiko.SSHException, TimeoutError) as err:
-                raise FileNotFoundError from err
+                raise FileNotFoundError() from err
 
             path_zip = sim_folder.with_suffix(".zip")
             with ZipFile(path_zip, "r") as zip_ref:
                 zip_ref.extractall(root)
 
             path_zip.unlink()
         else:
@@ -398,15 +425,15 @@
                 self.scp_client.get(
                     str(DATA_CONFIG["server"]["simulation_path"] / dut_folder / sweep_folder),
                     local_path=str(root),
                     recursive=True,
                 )
             except (SCPException, paramiko.SSHException) as err:
                 # reraise it in order to allow run_and_read to go on and try again in 2 seconds
-                raise FileNotFoundError from err
+                raise FileNotFoundError() from err
 
     def copy_log_from_server(self, dut, sweep):
         """Collects the simulation log file from the server.
 
         Parameters
         ----------
         dut : DutView
@@ -422,15 +449,15 @@
                     DATA_CONFIG["server"]["simulation_path"] / dut_folder / sweep_folder / "sim.log"
                 ),
                 local_path=str(root / sweep_folder),
                 recursive=True,
             )
         except (SCPException, paramiko.SSHException) as err:
             # reraise it in order to allow run_and_read to go on and try again in 2 seconds
-            raise FileNotFoundError from err
+            raise FileNotFoundError() from err
 
     def run_simulations(self, sim_list):
         """Runs all given simulations in parallel.
 
         Parameters
         ----------
         sim_list :  [{}]
@@ -754,15 +781,15 @@
             id_ = "".join([n for n in str(output).split(".")[0] if n.isdigit()])
             try:
                 return int(id_)
             except ValueError:
                 return 0
 
 
-def _check_simulation_needed(i_sim, n_tot, dut=None, sweep=None):
+def _check_simulation_needed(i_sim, n_tot, dut=None, sweep=None, sweep_exists=None):
     """Function to check if the simulation is needed or already present in the database
 
     Parameter
     -----------
     dut : DMT.core.DutView
     sweep : DMT.core.Sweep
 
@@ -773,38 +800,37 @@
     None
         In case the simulation must be done.
     """
     dut_name = dut.name + str(dut.get_hash())
     sim_name = sweep.name + "_" + sweep.get_hash()
     # print("Check: dut: {:s}, sweep: {:s}".format(dut_name, sim_name))
     print_progress_bar(i_sim, n_tot, prefix="Progress", length=50)
-    if dut.check_existence_sweep(sweep):
-        logging.info("Simulation of DuT %s with sweep %s loaded from database.", dut_name, sim_name)
-    else:
-        # if not in dut.data and not in dut.db
-        try:
-            # was it simulated already successfully ?
-            dut.validate_simulation_successful(sweep)
-            logging.info(
-                "Simulation of DuT %s with sweep %s already done and results are valid, only data needs to be read.",
-                dut_name,
-                sim_name,
-            )
-            logging.debug(
-                "The simulation folder of this simulation was %s", dut.get_sim_folder(sweep)
-            )
-            dut.add_data(sweep)
-        except SimulationFail:
-            print("Simulation of DuT %s with sweep %s already done and failed!", dut_name, sim_name)
-        # except (SimulationUnsuccessful, FileNotFoundError, IndexError, struct.error):
-        except:  # all exceptions should be re-simulated
-            # ok simulate it!
-            dut.delete_sim_results(sweep, ignore_errors=True)  # remove for safety
-            logging.info("Simulation of DuT %s with sweep %s needed.", dut_name, sim_name)
-            return None
+    try:
+        # was it simulated already successfully ?
+        dut.validate_simulation_successful(sweep)
+        print(
+            f"\n Simulation of DuT {dut_name} with sweep {sim_name} already done and results are valid, only data needs to be read.",
+        )
+        logging.info(
+            "Simulation of DuT %s with sweep %s already done and results are valid, only data needs to be read.",
+            dut_name,
+            sim_name,
+        )
+        logging.debug("The simulation folder of this simulation was %s", dut.get_sim_folder(sweep))
+        dut.add_data(sweep)
+    except SimulationFail:
+        print(
+            f"\n Simulation of DuT {dut_name} with sweep {sim_name} already done and failed.",
+        )
+    # except (SimulationUnsuccessful, FileNotFoundError, IndexError, struct.error):
+    except:  # all exceptions should be re-simulated
+        # ok simulate it!
+        dut.delete_sim_results(sweep, ignore_errors=True)  # remove for safety
+        logging.info("Simulation of DuT %s with sweep %s needed.", dut_name, sim_name)
+        return None
 
     return dut.data
 
 
 def _read_process_results(success, dut, sweep):
     """Read the process results
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/singleton.py` & `DMT_core-2.0.0/DMT/core/singleton.py`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/core/sweep.py` & `DMT_core-2.0.0/DMT/core/sweep.py`

 * *Files 8% similar despite different names*

```diff
@@ -21,28 +21,42 @@
 # DMT_core is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
+from __future__ import annotations
 import logging
 import copy
 from typing import Dict, List, Mapping, Type, Optional, Union, Set
 import numpy as np
 from itertools import product
 from DMT.core import create_md5_hash, specifiers, sub_specifiers, SpecifierStr, DataFrame, SweepDef
+from DMT.core.sweep_def import (
+    SweepDefLinear,
+    SweepDefList,
+    SweepDefLog,
+    SweepDefSync,
+    SweepDefConst,
+)
+
+_SPEC_VOLTAGE = specifiers.VOLTAGE
+_SPEC_CURRENT = specifiers.CURRENT
+_SPEC_TEMPERATURE = specifiers.TEMPERATURE
+_SPEC_FREQUENCY = specifiers.FREQUENCY
+_SSPEC_FORCED = sub_specifiers.FORCED
 
 
 def get_sweepdef(
     data: DataFrame,
     inner_sweep_voltage: Optional[SpecifierStr] = None,
     outer_sweep_voltage: Optional[SpecifierStr] = None,
     decimals_potentials: int = 3,
-):
+) -> List[Dict]:
     """Given a dataframe, one inner sweep_voltage and one outer sweep voltage, this method tries to create a SweepDefinition that can be used to re-simulate the data.
 
     Parameters
     ----------
     data : DataFrame
         Frame to extract the sweepdefs from
     inner_sweep_voltage : SpecifierStr | None, optional
@@ -71,48 +85,48 @@
     """
     if not data.columns.is_unique:
         data = data.loc[:, ~data.columns.duplicated()]  # type: ignore
 
     if inner_sweep_voltage is None and outer_sweep_voltage is None:
         from_forced = False
         for col in data.columns:
-            if sub_specifiers.FORCED in col:
+            if _SSPEC_FORCED in col:
                 from_forced = True
                 break  # found one -> do from forced
 
         potentials_forced = []  # list of forced voltages
         for col in data.columns:
             try:
                 if (
-                    (col.specifier == specifiers.VOLTAGE)
+                    (col.specifier == _SPEC_VOLTAGE)
                     and len(col.nodes) == 1
-                    and (not from_forced or (sub_specifiers.FORCED in col))
+                    and (not from_forced or (_SSPEC_FORCED in col))
                 ):  # forced voltages are needed to create sweepdef
                     potentials_forced.append(col)
             except AttributeError:  # can only analyze specifiers
                 pass
 
         if not potentials_forced:
             raise IOError(
-                "DMT->df_to_sweep: No forced potentials in the columns. Make sure all forced potentials in the columns are SpecifierStr!"
+                "DMT->get_sweepdef: No forced potentials in the columns. Make sure all forced potentials in the columns are SpecifierStr!"
             )
 
         # find one potential with only one value and set it as reference potential!
         potential_common = ""
         for potential in sorted(
             potentials_forced, key=lambda x: x.nodes[0]
         ):  # sort to make sure everytime the same is found.
             if len(np.unique(np.round(data[potential].to_numpy(), decimals_potentials))) == 1:
                 potential_common = potential  # use this one! Even if more than one would exist.
                 break
 
         if not potential_common:  # no potential found
             # did not find anything :(
             raise IOError(
-                "DMT -> df_to_sweep: The user supplied voltages do not define unambiguous sweep conditions for the transistor. No common reference potential was found."
+                "DMT->get_sweepdef: The user supplied voltages do not define unambiguous sweep conditions for the transistor. No common reference potential was found."
             )
 
         # now we need all sweep potentials with regard to one reference potential or other synced sweeps.
         potentials_sweep = [
             potential for potential in set(potentials_forced) if potential != potential_common
         ]
 
@@ -121,18 +135,18 @@
         for potential in sorted(potentials_sweep, key=lambda x: x.nodes[0]):
             # against all other:
             for potential_other in sorted(potentials_forced, key=lambda x: x.nodes[0]):
                 if potential_other == potential:
                     continue  # not against self
 
                 if from_forced:
-                    if potential_other + potential.nodes[0] + sub_specifiers.FORCED in count_ops:
+                    if potential_other + potential.nodes[0] + _SSPEC_FORCED in count_ops:
                         continue  # not V_BC and V_CB, only one of those..
 
-                    voltage = potential + potential_other.nodes[0] + sub_specifiers.FORCED
+                    voltage = potential + potential_other.nodes[0] + _SSPEC_FORCED
                 else:
                     if potential_other + potential.nodes[0] in count_ops:
                         continue  # not V_BC and V_CB, only one of those..
 
                     voltage = potential + potential_other.nodes[0]
 
                 data.ensure_specifier_column(voltage)
@@ -144,183 +158,149 @@
         ):  # last of the sorted list is the one we don't need
             data.ensure_specifier_column(voltage)
             if i_voltage == 0:
                 outer_sweep_voltage = voltage
             elif i_voltage == 1:
                 inner_sweep_voltage = voltage
             else:
-                raise OSError("only two stage voltages allowed :(")
+                raise OSError("DMT->get_sweepdef: only two stage voltages allowed :(")
 
     elif inner_sweep_voltage is None or outer_sweep_voltage is None:
         raise NotImplementedError(
             "DMT->get_sweepdef: Either set both or no sweep specifier for now!"
         )
 
     assert inner_sweep_voltage is not None
     assert outer_sweep_voltage is not None
 
-    if specifiers.VOLTAGE in inner_sweep_voltage and specifiers.VOLTAGE in outer_sweep_voltage:
+    if _SPEC_VOLTAGE in inner_sweep_voltage and _SPEC_VOLTAGE in outer_sweep_voltage:
         # classical decision: Efficient short code vs cryptic. Not sure which is better here.
         # -> try general code: transform voltage definition into appropriate "coordinate" system, where the voltages become independent from each other.
         potential_one_inner = (
-            specifiers.VOLTAGE + inner_sweep_voltage.nodes[0] + inner_sweep_voltage.sub_specifiers
+            _SPEC_VOLTAGE + inner_sweep_voltage.nodes[0] + inner_sweep_voltage.sub_specifiers
         )
         potential_two_inner = (
-            specifiers.VOLTAGE + inner_sweep_voltage.nodes[1] + inner_sweep_voltage.sub_specifiers
+            _SPEC_VOLTAGE + inner_sweep_voltage.nodes[1] + inner_sweep_voltage.sub_specifiers
         )
 
         potential_one_outer = (
-            specifiers.VOLTAGE + outer_sweep_voltage.nodes[0] + outer_sweep_voltage.sub_specifiers
+            _SPEC_VOLTAGE + outer_sweep_voltage.nodes[0] + outer_sweep_voltage.sub_specifiers
         )
         potential_two_outer = (
-            specifiers.VOLTAGE + outer_sweep_voltage.nodes[1] + outer_sweep_voltage.sub_specifiers
+            _SPEC_VOLTAGE + outer_sweep_voltage.nodes[1] + outer_sweep_voltage.sub_specifiers
         )
 
         # find common potential between voltages and set it as reference potential
         common_potential = [
             potential
             for potential in [potential_one_inner, potential_two_inner]
             if potential in [potential_one_outer, potential_two_outer]
         ]
         if len(common_potential) != 1:
             raise IOError(
-                "DMT -> Sweep -> get_sweep: the supplied voltages do not define unambiguous sweep conditions for the data."
+                "DMT->get_sweepdef: the supplied voltages do not define unambiguous sweep conditions for the data."
             )
 
         # now we just need two sweeps and one reference potential. wuhu...
         reference_potential = common_potential[0]
-        inner_sweep_potential = next(
+        inner_potential_name = next(
             potential
             for potential in [potential_one_inner, potential_two_inner]
             if potential != reference_potential
         )
-        outer_sweep_potential = next(
+        outer_potential_name = next(
             potential
             for potential in [potential_one_outer, potential_two_outer]
             if potential != reference_potential
         )
 
         # find list values for the two swept potentials with respect to the new reference node.
-        outer_sweep_potential_vals = (
-            data[outer_sweep_potential].to_numpy() - data[reference_potential].to_numpy()
+        outer_potentials = (
+            data[outer_potential_name].to_numpy() - data[reference_potential].to_numpy()
         )
-        outer_sweep_potential_vals = np.round(
-            outer_sweep_potential_vals, decimals=decimals_potentials
-        )
-        outer_sweep_potential_vals = np.unique(outer_sweep_potential_vals)
+        outer_potentials = np.unique(np.round(outer_potentials, decimals=decimals_potentials))
 
-        inner_sweep_potential_vals = (
-            data[inner_sweep_potential].to_numpy() - data[reference_potential].to_numpy()
+        inner_potentials = (
+            data[inner_potential_name].to_numpy() - data[reference_potential].to_numpy()
         )
-        inner_sweep_potential_vals = np.unique(inner_sweep_potential_vals)
+        inner_potentials = np.unique(inner_potentials)
 
         # the circuit only allows to sweep VB VC VE, which are forced due to the circuit topology
         sweepdef = [
-            {
-                "var_name": specifiers.VOLTAGE + reference_potential.nodes[0],
-                "sweep_order": 1,
-                "sweep_type": "CON",
-                "value_def": [0],
-            },
-            {
-                "var_name": specifiers.VOLTAGE + outer_sweep_potential.nodes[0],
-                "sweep_order": 2,
-                "sweep_type": "LIST",
-                "value_def": outer_sweep_potential_vals,
-            },
-            {
-                "var_name": specifiers.VOLTAGE + inner_sweep_potential.nodes[0],
-                "sweep_order": 3,
-                "sweep_type": "LIST",
-                "value_def": inner_sweep_potential_vals,
-            },
+            SweepDefConst(_SPEC_VOLTAGE + reference_potential.nodes[0], sweep_order=0, value_def=0),
+            SweepDefList(
+                _SPEC_VOLTAGE + outer_potential_name.nodes[0],
+                sweep_order=1,
+                value_def=outer_potentials,
+            ),
+            SweepDefList(
+                _SPEC_VOLTAGE + inner_potential_name.nodes[0],
+                sweep_order=2,
+                value_def=inner_potentials,
+            ),
         ]
     else:
-        if specifiers.CURRENT in inner_sweep_voltage and specifiers.CURRENT in outer_sweep_voltage:
+        if _SPEC_CURRENT in inner_sweep_voltage and _SPEC_CURRENT in outer_sweep_voltage:
             # two currents forced
             raise OSError("Only one forced current at the moment!")
-        if specifiers.CURRENT in inner_sweep_voltage:
+        if _SPEC_CURRENT in inner_sweep_voltage:
             # one current forced, one voltage
-            inner_sweep_potential_vals = +data[inner_sweep_voltage].to_numpy()
-            reference_potential = specifiers.VOLTAGE + outer_sweep_voltage.nodes[1]
-            outer_sweep_potential_vals = data[outer_sweep_voltage].to_numpy()
-            outer_sweep_potential_vals = np.unique(outer_sweep_potential_vals)
+            inner_potentials = +data[inner_sweep_voltage].to_numpy()
+            reference_potential = _SPEC_VOLTAGE + outer_sweep_voltage.nodes[1]
+            outer_potentials = data[outer_sweep_voltage].to_numpy()
+            outer_potentials = np.unique(outer_potentials)
             sweepdef = [
-                {
-                    "var_name": reference_potential,
-                    "sweep_order": 1,
-                    "sweep_type": "CON",
-                    "value_def": [0],
-                },
-                {
-                    "var_name": specifiers.VOLTAGE + outer_sweep_voltage.nodes[0],
-                    "sweep_order": 2,
-                    "sweep_type": "CON",
-                    "value_def": outer_sweep_potential_vals,
-                },
-                {
-                    "var_name": inner_sweep_voltage,
-                    "sweep_order": 3,
-                    "sweep_type": "LIST",
-                    "value_def": inner_sweep_potential_vals,
-                },
+                SweepDefConst(reference_potential, sweep_order=0, value_def=0),
+                SweepDefConst(
+                    _SPEC_VOLTAGE + outer_sweep_voltage.nodes[0],
+                    sweep_order=1,
+                    value_def=outer_potentials,
+                ),
+                SweepDefList(inner_sweep_voltage, sweep_order=2, value_def=inner_potentials),
             ]
-        elif specifiers.CURRENT in outer_sweep_voltage:
+        elif _SPEC_CURRENT in outer_sweep_voltage:
             potential_one_inner = (
-                specifiers.VOLTAGE
-                + inner_sweep_voltage.nodes[0]
-                + inner_sweep_voltage.sub_specifiers
+                _SPEC_VOLTAGE + inner_sweep_voltage.nodes[0] + inner_sweep_voltage.sub_specifiers
             )
             potential_two_inner = (
-                specifiers.VOLTAGE
-                + inner_sweep_voltage.nodes[1]
-                + inner_sweep_voltage.sub_specifiers
+                _SPEC_VOLTAGE + inner_sweep_voltage.nodes[1] + inner_sweep_voltage.sub_specifiers
             )
 
             # find common potential between voltages and set it as reference potential
             common_potential = [potential_two_inner]
 
             # now we just need two sweeps and one reference potential. wuhu...
             reference_potential = common_potential[0]
-            inner_sweep_potential = next(
+            inner_potential_name = next(
                 potential
                 for potential in [potential_one_inner, potential_two_inner]
                 if potential != reference_potential
             )
 
-            outer_sweep_potential_vals = np.unique(data[outer_sweep_voltage].to_numpy())
+            outer_potentials = np.unique(data[outer_sweep_voltage].to_numpy())
 
-            inner_sweep_potential_vals = (
-                data[inner_sweep_potential].to_numpy() - data[reference_potential].to_numpy()
+            inner_potentials = (
+                data[inner_potential_name].to_numpy() - data[reference_potential].to_numpy()
             )
-            inner_sweep_potential_vals = np.unique(inner_sweep_potential_vals)
+            inner_potentials = np.unique(inner_potentials)
 
             # the circuit only allows to sweep VB VC VE, which are forced due to the circuit topology
             sweepdef = [
-                {
-                    "var_name": specifiers.VOLTAGE + reference_potential.nodes[0],
-                    "sweep_order": 1,
-                    "sweep_type": "CON",
-                    "value_def": [0],
-                },
-                {
-                    "var_name": outer_sweep_voltage,
-                    "sweep_order": 2,
-                    "sweep_type": "CON",
-                    "value_def": outer_sweep_potential_vals,
-                },
-                {
-                    "var_name": specifiers.VOLTAGE + inner_sweep_potential.nodes[0],
-                    "sweep_order": 3,
-                    "sweep_type": "LIST",
-                    "value_def": inner_sweep_potential_vals,
-                },
+                SweepDefConst(
+                    _SPEC_VOLTAGE + reference_potential.nodes[0], sweep_order=0, value_def=0
+                ),
+                SweepDefConst(outer_sweep_voltage, sweep_order=1, value_def=outer_potentials),
+                SweepDefList(
+                    _SPEC_VOLTAGE + inner_potential_name.nodes[0],
+                    sweep_order=2,
+                    value_def=inner_potentials,
+                ),
             ]
         else:
-            raise NotImplementedError
+            raise NotImplementedError()
 
     return sweepdef
 
 
 class Sweep(object):
     r"""Creates a sweep.
 
@@ -503,15 +483,15 @@
         if isinstance(outputdef_new, (list, set)):
             # cast and copy to be save
             # sort to save some repeatings
             self._outputdef = sorted(list(copy.deepcopy(outputdef_new)))
         else:
             raise IOError("sweep.outputdef must to be a list or a set.")
 
-    def create_df(self):
+    def create_df(self) -> DataFrame:
         """Fill the dataframe according to the sweepdefinition
 
         Returns
         -------
         :class:`DMT.core.DataFrame`
             A pandas dataframe object that corresponds to the specified sweep. Values that need to be calculated are filled with numpy.nan .
         """
@@ -522,17 +502,18 @@
         # create concrete values for each sweepvariable---------------------------------------------------
         self.set_values()
 
         # add the concrete sweep values into the df -------------------------------------------------------
         columns = []
         values_per_subsweep = []
         for subsweep in self.sweepdef:
-            if not subsweep.sweep_type == "SYNC":
-                columns.append(subsweep.var_name)
-                values_per_subsweep.append(list(subsweep.values))
+            if subsweep.sweep_type in ["SYNC"]:
+                continue
+            columns.append(subsweep.var_name)
+            values_per_subsweep.append(list(subsweep.values))
 
         # sweepdefs are a tree...
         # use itertools product to generate all possible combinations in the correct order
         # https://docs.python.org/3.6/library/itertools.html#itertools.product
         values = product(*values_per_subsweep)
         self.df = DataFrame(values, columns=columns)
 
@@ -571,19 +552,14 @@
         check_sweep() has the following features:
 
         - checks the specified sweep type and converts it to a non-misunderstandable format.
         - corrects the sweep_order
         - sets offset for SYNC
         - checks if non-optional variables are specified
         - corrects the variable names according to DMT format
-
-        Returns
-        -------
-        :class:`DMT.core.Sweep`
-            corrected and checked Sweep object.
         """
 
         # correct sweeporder------------------------------------
         if any([swd.sweep_order is None for swd in self.sweepdef]):
             # no extra ordering given, set it automatically
             # also set some stuff of synced sweeps here
             sweep_order = 1
@@ -631,57 +607,78 @@
                 # if it uses a variable as offset find the sweepdef for this!
                 if swd.offset_var is not None:
                     self.sweepdef[i_swd].offset = next(
                         swd_ for swd_ in self.sweepdef if swd_.var_name == swd.offset_var
                     )
 
         # check if non-optional variables are specified
-        if specifiers.TEMPERATURE not in self.othervar:
-            if specifiers.TEMPERATURE not in [element.var_name for element in self.sweepdef]:
+        if _SPEC_TEMPERATURE not in self.othervar:
+            if _SPEC_TEMPERATURE not in [element.var_name for element in self.sweepdef]:
                 raise IOError(
                     "Non optional variable TEMP is not specified. TEMP is the temperature of the transistor."
                 )
 
         # make sure that every variable is only once in in sweepdef and also othervar
         vars_all = [element.var_name for element in self.sweepdef] + list(self.othervar.keys())
         if len(vars_all) != len(set(vars_all)):
             raise IOError(
-                "The Variable TEMP is specified more than once, this is forbidden for DMT. TEMP is the temperature of the transistor."
+                "One sweep variable is specified more than once, this is forbidden for DMT. The defined variable are:"
+                + " ".join(vars_all)
             )
 
-    def get_temperature(self):
+        # correct amp phase contact if set
+        for i_swd, swd in enumerate(self.sweepdef):
+            if swd.amp is not None:
+                if not isinstance(swd.amp, (float, int)):
+                    raise IOError(
+                        "DMT->Sweep: If an transient amplitude is set, is has to be of type float or int."
+                    )
+
+            if swd.phase is not None:
+                if not isinstance(swd.phase, (float, int)):
+                    raise IOError(
+                        "DMT->Sweep: If an transient phase is set, is has to be of type float or int."
+                    )
+
+            if swd.contact is not None:
+                if not isinstance(swd.contact, str):
+                    raise IOError(
+                        "DMT->Sweep: If an transient contact is set, is has to be of type str."
+                    )
+
+    def get_temperature(self) -> str:
         """Returns the temperature of the sweep as a string. Use this to set the key of a dut.
 
         Returns
         -------
         str
             - Single temperature: "Txxx.xxK"
             - List of temperatures: "T(xxx.xx,yyy.yy,...)K"
             - Range of temperatures: "T[xxx.xx-sss.ss-yyy.yy]K", s is the step
         """
-        if specifiers.TEMPERATURE in self.othervar:  # would be the easieast...
-            return "T{0:.2f}K".format(self.othervar[specifiers.TEMPERATURE])
+        if _SPEC_TEMPERATURE in self.othervar:  # would be the easieast...
+            return "T{0:.2f}K".format(self.othervar[_SPEC_TEMPERATURE])
 
         # search sweep for temperature
         for swd in self.sweepdef:
-            if swd.var_name == specifiers.TEMPERATURE:
+            if swd.var_name == _SPEC_TEMPERATURE:
                 if swd.sweep_type == "CON":
                     return "T{0:.2f}K".format(swd.value_def[0])
                 elif swd.sweep_type == "LIN":
                     return "T[{0:.2f}-{2:.2f}-{1:.2f}]K".format(*swd.value_def)
                 elif swd.sweep_type == "LIST":
                     return "T(" + ",".join(["{0:.2f}".format(val) for val in swd.value_def]) + ")K"
                 else:
                     raise NotImplementedError(
                         "The temperature of a sweep of type "
                         + swd.sweep_type
                         + " can not be converted into a valid key part until now."
                     )
 
-    def get_hash(self):
+    def get_hash(self) -> str:
         """Returns a hash for this sweep.
 
         Returns
         -------
         str
             MD5 hash that corresponds to this sweep.
         """
@@ -691,15 +688,15 @@
     def set_values(self):
         """Set the values of sweep according to the DMT definition."""
         for subsweep in self.sweepdef:
             subsweep.set_values()
 
         return self
 
-    def __eq__(self, other):
+    def __eq__(self, other: Sweep) -> bool:
         """Comparing two sweeps"""
         try:
             return self.get_hash() == other.get_hash()
         except AttributeError:
             return NotImplemented
 
     @classmethod
@@ -708,16 +705,16 @@
         data: DataFrame,
         temperature: Optional[float] = None,
         name: str = "sweep",
         outputdef: Optional[List[str]] = None,
         othervar: Optional[Dict[str, float]] = None,
         SweepDefClass: Type = SweepDef,
         decimals_potentials: int = 3,
-        **kwargs
-    ):
+        **kwargs,
+    ) -> Sweep:
         """Create a Sweep from a DataFrame
 
         Parameters
         ----------
         data : DataFrame
             data to create a Sweep from.
         temperature : float | None, optional
@@ -745,23 +742,18 @@
 
         if outputdef is None:
             outputdef = []
 
         sweepdefs = get_sweepdef(data, decimals_potentials=decimals_potentials, **kwargs)
 
         ### grab definition for the frequency, if possible
-        if specifiers.FREQUENCY in data.columns:
-            freq = np.unique(np.round(data[specifiers.FREQUENCY].to_numpy(), decimals_potentials))
+        if _SPEC_FREQUENCY in data.columns:
+            freq = np.unique(np.round(data[_SPEC_FREQUENCY].to_numpy(), decimals_potentials))
             sweepdefs.append(
-                {
-                    "var_name": specifiers.FREQUENCY,
-                    "sweep_order": len(sweepdefs) + 1,
-                    "sweep_type": "LIST",
-                    "value_def": freq,
-                },
+                SweepDefList(_SPEC_FREQUENCY, value_def=freq, sweep_order=len(sweepdefs))
             )
 
         return cls(
             name,
             sweepdef=sweepdefs,
             outputdef=outputdef,
             othervar=othervar,
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/sweep_def.py` & `DMT_core-2.0.0/DMT/core/sweep_def.py`

 * *Files 27% similar despite different names*

```diff
@@ -25,15 +25,17 @@
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 from __future__ import annotations
 from typing import Dict, List, Mapping, Type, Optional, Union, Tuple
 import numpy as np
 from DMT.core import (
+    specifiers,
     get_specifier_from_string,
+    flatten,
     SpecifierStr,
 )
 
 
 class SweepDef(object):
     """One sweep definition
 
@@ -63,25 +65,31 @@
         var_name: SpecifierStr,
         sweep_type: str,
         sweep_order: Optional[int] = None,
         value_def: Optional[Union[List, np.array]] = None,
         master: Optional[SpecifierStr] = None,
         offset: Optional[Union[int, float, SpecifierStr]] = None,
         sync: Optional[Union[SpecifierStr, SweepDef]] = None,
+        amp: Optional[Union[int, float]] = None,
+        phase: Optional[Union[int, float]] = None,
+        contact: Optional[str] = None,
     ):
         # needed names for repr
         self._attr_repr = [
             "var_name",
             "sweep_type",
             "sweep_order",
             "value_def",
             "master_var",
             "sync_var",
             "offset_var",
             "offset_value",
+            "amp",
+            "contact",
+            "phase",
         ]
 
         self.var_name = get_specifier_from_string(var_name)
         if not isinstance(self.var_name, SpecifierStr):
             raise IOError(
                 "DMT->Sweep: Automatic conversion from var_name string to SpecifierStr failed for the variable: "
                 + var_name
@@ -116,14 +124,19 @@
 
         self._offset_var = None
         self._offset_swd = None
         self._offset_value = None
         self.offset = offset
 
         self.values = None
+
+        self.amp = amp
+        self.phase = phase
+        self.contact = contact
+
         self.set_values()
 
     @property
     def sweep_type(self):
         """Directly return the sweep type"""
         return self._sweep_type
 
@@ -156,14 +169,18 @@
             return "LOG"
         elif "CON" in sweep_type_new:
             return "CON"
         elif "SYNC" in sweep_type_new:
             return "SYNC"
         elif "LIST" in sweep_type_new:
             return "LIST"
+        elif "SIN" in sweep_type_new:
+            return "SINUS"
+        elif "SMOOTH_RAMP" in sweep_type_new:
+            return "SMOOTH_RAMP"
         else:
             raise IOError(
                 'DMT->Sweep: specified sweeptype:"' + sweep_type_new + '" is unknown to DMT.'
             )
 
     @property
     def master(self):
@@ -251,27 +268,27 @@
         Raises
         ------
         OSError
             If the sweep type is not known.
         """
         if self.sweep_type == "LIN":
             self.values = np.linspace(
-                self.value_def[0], self.value_def[1], self.value_def[2], dtype=np.float64
+                self.value_def[0], self.value_def[1], int(self.value_def[2]), dtype=np.float64
             )
 
         elif self.sweep_type == "CON":
             self.values = np.array(self.value_def, dtype=np.float64)
             if self.values.size > 1:
                 raise IOError(
                     "DMT->SweepDef: Constant sweeps must have only one value in value_def!"
                 )
 
         elif self.sweep_type == "LOG":
             self.values = np.logspace(
-                self.value_def[0], self.value_def[1], self.value_def[2], dtype=np.float64
+                self.value_def[0], self.value_def[1], int(self.value_def[2]), dtype=np.float64
             )
 
         elif self.sweep_type == "LIST":
             self.values = np.array(self.value_def, dtype=np.float64)
 
         elif self.sweep_type == "SYNC":
             if self.master is None:  # master has not been replaced jet..
@@ -281,14 +298,52 @@
                 self.values = self.master.values + self.offset
             except TypeError:
                 self.values = np.zeros((self.offset.values.size, self.master.values.size))
                 for i_col in range(self.values.shape[0]):
                     self.values[i_col, :] = self.master.values + self.offset.values[i_col]
                 self.values = np.concatenate(self.values)
 
+        elif self.sweep_type == "SINUS":
+            # 3 periods with 40 points per period
+            self.values = np.array(
+                list(flatten(np.linspace(0, 3 / freq, 121) for freq in self.value_def))
+            )
+        elif self.sweep_type == "SMOOTH_RAMP":
+            # 3 periods with 40 points per period
+            self.values = np.array(
+                list(flatten(np.linspace(0, 3 / freq, 121) for freq in self.value_def))
+            )
+        else:
+            raise OSError(
+                'DMT->Sweep: specified sweeptype:"' + self.sweep_type + '" is unknown to DMT.'
+            )
+
+    def get_input_signal(self):
+        """Returns the transient input signal for the SweepDef (without DC!)"""
+        self.set_values()
+        if self.sweep_type == "SINUS":
+            signal = []
+            for i_freq, freq in enumerate(self.value_def):
+                t = self.values[i_freq * 121 : (i_freq + 1) * 121]
+                signal += list(
+                    self.amp * (np.sin(2 * np.pi * t * freq - self.phase) - np.sin(self.phase))
+                )
+            return np.array(list(flatten(signal)))
+        elif self.sweep_type == "SMOOTH_RAMP":
+            signal = []
+            for i_freq, freq in enumerate(self.value_def):
+                t = self.values[i_freq * 121 : (i_freq + 1) * 121]
+                tau = np.sqrt(2) * np.exp(-1 / 2) / (2 * np.pi * freq)
+                signal += list(self.amp * (1 - np.exp(-((t / tau) ** 2))))
+            return np.array(list(flatten(signal)))
+        else:
+            raise OSError(
+                'DMT->Sweep: specified sweeptype:"' + self.sweep_type + '" is unknown to DMT.'
+            )
+
 
 class SweepDefConst(SweepDef):
     """Constant sweep definition
 
     Parameters
     ----------
     var_name : SpecifierStr
@@ -450,7 +505,75 @@
         super().__init__(
             var_name=var_name,
             sweep_type="SYNC",
             sweep_order=sweep_order,
             master=master,
             offset=offset,
         )
+
+
+class SweepDefTransSinus(SweepDef):
+    """Sinusoidal transient sweep definition
+
+    Parameters
+    ----------
+    amp : Union[int, float], optional
+        _description_, by default None
+    phase : Union[int, float], optional
+        _description_, by default None
+    contact : Union[Tuple[str], str], optional
+        _description_, by default None
+    sweep_order : Optional[int], optional
+        _description_, by default None
+    """
+
+    def __init__(
+        self,
+        value_def: Union[List, np.array] = None,
+        amp: Union[int, float] = None,
+        phase: Union[int, float] = None,
+        contact: str = None,
+        sweep_order: Optional[int] = None,
+    ):
+        super().__init__(
+            value_def=value_def,
+            var_name=specifiers.TIME,
+            sweep_type="SINUS",
+            sweep_order=sweep_order,
+            amp=amp,
+            phase=phase,
+            contact=contact,
+        )
+
+
+class SweepDefTransRamp(SweepDef):
+    """smooth ramp transient sweep definition
+
+    Parameters
+    ----------
+    amp : Union[int, float], optional
+        _description_, by default None
+    phase : Union[int, float], optional
+        _description_, by default None
+    contact : Union[Tuple[str], str], optional
+        _description_, by default None
+    sweep_order : Optional[int], optional
+        _description_, by default None
+    """
+
+    def __init__(
+        self,
+        value_def: Union[List, np.array] = None,
+        amp: Union[int, float] = None,
+        phase: Union[int, float] = None,
+        contact: str = None,
+        sweep_order: Optional[int] = None,
+    ):
+        super().__init__(
+            value_def=value_def,
+            var_name=specifiers.TIME,
+            sweep_type="SMOOTH_RAMP",
+            sweep_order=sweep_order,
+            amp=amp,
+            phase=phase,
+            contact=contact,
+        )
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/technology.py` & `DMT_core-2.0.0/DMT/core/technology.py`

 * *Files 12% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # DMT_core is distributed in the hope that it will be useful,
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 # GNU General Public License for more details.
 #
 # You should have received a copy of the GNU General Public License
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
+import abc
 from DMT.core.dut_type import DutType
 
 try:
     from pylatex import Section
     from DMT.external.pylatex import Tex
 except ImportError:
     pass
@@ -43,18 +44,18 @@
     ----------
     name : str
         Name of the technology
 
     """
     name = ""
 
-    def __init__(self, name, scaling_builder=None):
+    def __init__(self, name):
         self.name = name
-        self.scaling_builder = scaling_builder
 
+    @abc.abstractmethod
     def print_tex(self, dut_ref, mcard):
         """Prints a technology description, mainly used for autodocumentation reasons.
 
         Parameters
         ----------
         dut_ref : :class:`~DMT.core.DutView`
             Can be used to obtain tech quanties... (or to generate a TRADICA input file :) )
@@ -62,18 +63,45 @@
             A Modelcard that contains all parameters that are required for scaling, as well as the parameters that shall be scaled.
         """
         doc = Tex()
         with doc.create(Section("Technology :" + self.name)):
             doc.append("Technology description missing")
         return doc
 
+    @abc.abstractmethod
     def get_bib_entries(self):
         """bibliograpy entries of a technology"""
         return ""
 
+    @abc.abstractmethod
+    def serialize(self):
+        """Return a dict which makes a constructor of the class callable
+
+        Returns
+        -------
+        dict
+            Has 1 required ("class") and 3 optional keys
+
+                * "class": always str(self.__class__), this is used to identify the correct technology during loading!
+                * "constructor": Name of the STATIC constructor method to call to create the technology. If not set, __init__ is used.
+                * "args": List of arguments to pass to the constructor
+                * "kwargs": List of keyword arguments to pass to the constructor
+
+            While loading a DutView the deserializiaton will be called like::
+
+                tech = getattr(cls_technology, serialized_technology["constructor"])(*args, **kwargs)
+
+        """
+        return {
+            "class": str(self.__class__),
+            "args": [self.name],
+            "kwargs": {},
+            "constructor": None,
+        }
+
     def create_mcard_library(self, lib, mcard, path, dut_type=DutType.npn):
         """Creates a file containing model cards for all sizes of duts present in the lib.
 
         Parameters
         ----------
         lib : :class:`~DMT.core.DutLib`
         path : str
```

### Comparing `DMT_core-1.8.0rc1/DMT/core/utils.py` & `DMT_core-2.0.0/DMT/core/utils.py`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/core/va_file.py` & `DMT_core-2.0.0/DMT/core/va_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,14 @@
 
 
 class VACode(object):  # Storage
     """Base file for VA-Codes
 
     Parameters
     ----------
-    name : str
-        Name of the code file (should include a relative path to the file which includes this one)
     code : str, optional
         Code of the file
     code_compressed : (str, int), optional
         Compressed code as loaded from a json modelcard file.
     ignore_checksum: bool, optional
         If True, the checksum is ignored, defaults to False.
     """
@@ -62,16 +60,16 @@
         return self.code
 
     def __eq__(self, other: VACode) -> bool:
         """Compare two Files. Equal if both name and codes are equal
 
         Parameters
         ----------
-        other : VAFileBase
-            Other VAFile to compare
+        other : VACode
+            Other VACode to compare
 
         Returns
         -------
         bool
             True if both have the same name and code...
         """
         if isinstance(other, VACode):
@@ -119,16 +117,16 @@
             raise OSError(
                 "Saved checksum and checksum of decompressed code do not match",
                 "MCard load compressed va_codes failed. VA-Codes not loaded, manual reset needed!",
             )  # Raise an error here??
         self.code = zlib.decompress(code).decode("utf-8")
 
 
-class VAFile(object):
-    """Tree VA-File for VA-Code. The tree is chosen to correctly mirror possible file structures of multi-file VA-Codes
+class VAFileMap(object):
+    """Mapping for VA-Code. The mapping data type is chosen to correctly use possible file structures of multi-file VA-Codes
 
     Parameters
     ----------
     name : Union[str, Path]
         Absolute or relative path to file or just name of the root file.
     files : dict, optional
         Dictionary with {file_name: VACode}. One of the keys must be the same as the name, by default None
@@ -151,15 +149,14 @@
         self.files: dict[str, VACode] = {}
 
         if not isinstance(name, Path):
             name = Path(name)
 
         self.root: str = name.name
         if files is None:
-
             if name.is_file():
                 self.read_structure(name.parent)
             elif code:
                 if isinstance(code, VACode):
                     self.files[self.root] = code
                 else:
                     self.files[self.root] = VACode(code=code)
@@ -263,64 +260,72 @@
         Returns
         -------
         dict
             [description]
         """
         export = {"__root__": self.root}  # this should be not used somewhere!
         for name, vafile in self.iter_codes():
+            if name == "__root__":
+                raise IOError(
+                    "DMT.VACode: Error in exporting the VA-Code to dict because one file is named '__root__'."
+                )
             if compressed_code:
                 export[name] = vafile.code_compressed  # type: ignore
             else:
                 export[name] = vafile.code
 
         return export
 
     @classmethod
-    def import_dict(cls, data_import: dict, ignore_checksum: bool = False) -> VAFile:
-        """Imports a VAFile inclusive children from a (serialized) dictionary
+    def import_dict(cls, data_import: dict, ignore_checksum: bool = False) -> VAFileMap:
+        """Imports a full VAFileMap from a (serialized) dictionary
 
         Parameters
         ----------
         data_import : dict
             [description]
         ignore_checksum: bool, optional
             If True, the checksum is ignored, defaults to False.
 
         Returns
         -------
-        VAFile
+        VAFileMap
             [description]
         """
         root = data_import.pop("__root__")
         files = {}
 
         for name, code in data_import.items():
             if isinstance(code, str):
                 files[name] = VACode(code=code)
             else:
                 files[name] = VACode(code_compressed=code, ignore_checksum=ignore_checksum)
 
-        return VAFile(name=root, files=files)
+        return VAFileMap(name=root, files=files)
 
     def write_files(
         self, path_to_target: Union[str, Path], filter: Optional[Callable[[str], str]] = None
     ):
-        """Writes the VAFile and all its descendants into the given target path. The file structure is written as read from the "original"
+        """Writes the all Verilog-A files from this mapping into the given target path. The file structure is written as read from the "original"
 
         Parameters
         ----------
         path_to_target : Union[str, Path]
             Path to target directory
         filter : callable, optional
+            Called with each code file as an argument. Can be used to filter out "non-compiling" additional code parts.
+            For example to remove VAE language extensions (spectre)::
+
+                lambda code: re.sub(r"\(\*.+\*\)", "", code)
 
         """
         if not isinstance(path_to_target, Path):
             path_to_target = Path(path_to_target)
 
-        for (name, code) in self.iter_codes():
+        for name, code in self.iter_codes():
             path_to_vafile = path_to_target / name
             path_to_vafile.parent.mkdir(exist_ok=True, parents=True)
             if filter is not None:
                 text = filter(code.code)
             else:
                 text = code.code
             path_to_vafile.write_text(text)
@@ -336,23 +341,23 @@
         -------
         int
             Length of tree
         """
         return len(self.files)
 
     def __eq__(self, other: object) -> bool:
-        """Allows comparing two VAFiles
+        """Allows comparing two VAFileMap objects
 
         Parameters
         ----------
         other : object
-            Only possible for other VAFiles.
+            Only possible for other VAFileMap objects.
 
         Returns
         -------
         bool
-            True if other VAFile has same root and same files.
+            True if other VAFileMap has same root and same files.
         """
-        if isinstance(other, VAFile):
+        if isinstance(other, VAFileMap):
             return self.root == other.root and self.files == other.files
 
         return NotImplemented
```

### Comparing `DMT_core-1.8.0rc1/DMT/exceptions/__init__.py` & `DMT_core-2.0.0/DMT/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/external/__init__.py` & `DMT_core-2.0.0/DMT/external/__init__.py`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/external/latex.py` & `DMT_core-2.0.0/DMT/external/latex.py`

 * *Files 3% similar despite different names*

```diff
@@ -107,34 +107,35 @@
     ----
     somehow this does not work so nice...
     """
     if not isinstance(full_path_to_file, Path):
         full_path_to_file = Path(full_path_to_file)
     directory = full_path_to_file.parent
     file_name = full_path_to_file.name.replace(".tex", "")
+    file_name = file_name.replace(".png", "")
 
     with cd(directory):
         # call latex to compile dvi
-        command = ["latex", "--interaction=nonstopmode", file_name + ".tex"]
+        command = ["latex", "--interaction=nonstopmode", full_path_to_file.name]
         try:
             output = subprocess.check_output(command, stderr=subprocess.STDOUT)
         except (OSError, IOError, subprocess.CalledProcessError) as e:
             # For all these errors print the output and raise the error
             print(e.output.decode())
             # raise
         else:
             print(output.decode())
 
         # call dvisvgm to compile dvi to svg
-        command = ["pdftoppm", file_name + ".pdf", "outpuname", "-png", file_name + ".png"]
+        command = ["pdftoppm", "-png", file_name + ".pdf"]
         # pdftoppm input.pdf outputname -png
         # command = ['convert ', file_name+'.dvi','-quality 90', file_name+'.png']
         # convert -density 300 F_TJ_C.pdf -quality 90 F_TJ_C.png
         try:
-            output = subprocess.check_output(command, stderr=subprocess.STDOUT)
+            output = subprocess.check_output(command, stderr=subprocess.PIPE)
         except (OSError, IOError, subprocess.CalledProcessError) as e:
             # For all these errors print the output and raise the error
             print(e.output.decode())
             # raise
         else:
             print(output.decode())
 
@@ -235,14 +236,16 @@
 }
 
 
 def resolve_siunitx(label):
     """This function tries to remove siunitx expressions from given Tex expression."""
     regex_si = r"\\si({.*?})"
     regex_SI = r"\\SI({.*?})({.*?})"
+    regex_qty = r"\\qty({.*?})({.*?})"
+
     if "si" in label:
         pattern = re.compile(regex_si)
         for match in pattern.findall(label):
             units = match[1:-1]
             # todo: resolve unit after unit, then for each unit the scaler (milli and so on), than stuff like per. Only then per can be correctly replaced.
             for key in SI_UNITS_CONVERTER:
                 units = units.replace(key, SI_UNITS_CONVERTER[key])
@@ -259,34 +262,50 @@
             # match 1 is unit
             units = match_unit[1:-1]
             for key in SI_UNITS_CONVERTER:
                 units = units.replace(key, SI_UNITS_CONVERTER[key])
 
             label = label.replace(match_unit, units)
 
+    if "qty" in label:
+        pattern = re.compile(regex_qty)
+        for match_number, match_unit in pattern.findall(label):
+            # match 0 is number
+            number = match_number[1:-1]
+            label = label.replace(match_number, number)
+
+            # match 1 is unit
+            units = match_unit[1:-1]
+            for key in SI_UNITS_CONVERTER:
+                units = units.replace(key, SI_UNITS_CONVERTER[key])
+
+            label = label.replace(match_unit, units)
+
     if "underline" in label:
         regex_underline = r"(\\underline{)([^{}]+)(})"
         pattern = re.compile(regex_underline)
         for match in pattern.findall(label):
             label = label.replace(match[0], "")
             label = label.replace(match[1] + match[2], match[1])
 
     # drop some tex things that are not understood by pandoc
     label = label.replace("\\si", "")
     label = label.replace("\\SI", "")
+    label = label.replace("\\qty", "")
     label = label.replace("\\,", " ")
 
     return label
 
 
 def tex_to_text(tex):
     """Return a text representation of a tex label."""
     tex = resolve_siunitx(tex)
     tex = tex.replace("\\num", "")
     tex = tex.replace("\\mathrm", "")
     tex = tex.replace("\\quad", "  ")
     tex = tex.replace("\\left(", "(")
     tex = tex.replace("\\right)", ")")
+    tex = tex.replace("\\overline", "mean ")
     tex = tex.replace("{", "")
     tex = tex.replace("}", "")
     tex = tex.replace("$", "")
     return tex
```

### Comparing `DMT_core-1.8.0rc1/DMT/external/os.py` & `DMT_core-2.0.0/DMT/external/os.py`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/external/pylatex.py` & `DMT_core-2.0.0/DMT/external/pylatex.py`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/external/verilogae.py` & `DMT_core-2.0.0/DMT/external/verilogae.py`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/libautodoc_template/base/acronyms.tex` & `DMT_core-2.0.0/DMT/libautodoc_template/base/acronyms.tex`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/libautodoc_template/base/header.tex` & `DMT_core-2.0.0/DMT/libautodoc_template/base/header.tex`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/libautodoc_template/content/conclusion.tex` & `DMT_core-2.0.0/DMT/libautodoc_template/content/conclusion.tex`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/libautodoc_template/content/deckblatt.tex` & `DMT_core-2.0.0/DMT/libautodoc_template/content/deckblatt.tex`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/libautodoc_template/content/introduction.tex` & `DMT_core-2.0.0/DMT/libautodoc_template/content/introduction.tex`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/libautodoc_template/documentation.tex` & `DMT_core-2.0.0/DMT/libautodoc_template/documentation.tex`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/ngspice/__init__.py` & `DMT_core-2.0.0/DMT/ngspice/__init__.py`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/ngspice/dut_ngspice.py` & `DMT_core-2.0.0/DMT/ngspice/dut_ngspice.py`

 * *Files 15% similar despite different names*

```diff
@@ -36,30 +36,43 @@
 # along with this program.  If not, see <http://www.gnu.org/licenses/>
 from typing import Union
 import os
 import logging
 import copy
 import re
 import numpy as np
+import pandas as pd
+import subprocess
+from pathlib import Path
+from typing import List, Dict
+
+try:
+    from semver.version import Version as VersionInfo
+except ImportError:
+    from semver import VersionInfo
 
 from DMT.config import COMMANDS
 from DMT.core import (
     DutCircuit,
     Circuit,
     MCard,
     constants,
     DataFrame,
     specifiers,
     sub_specifiers,
     McParameterCollection,
+    SweepDef,
+    Technology,
 )
 from DMT.core.circuit import SGP_BJT, VOLTAGE, CURRENT, HICUML2_HBT, SHORT, DIODE
 
 from DMT.exceptions import SimulationUnsuccessful
 
+SEMVER_DUTNGSPICE_CURRENT = VersionInfo(major=1, minor=0)
+
 
 class DutNgspice(DutCircuit):
     """Class description and methods
 
     Parameters
     ----------
     database_dir    : string
@@ -75,20 +88,23 @@
         If True, all given VA-files are copied to the simulation directory and compiled there. If False, the VA-Files have to be given as a global path.
     """
 
     def __init__(
         self,
         database_dir,
         dut_type,
-        input_circuit,
+        inp_circuit,
         name="ngspice_",
         simulator_options=None,
         simulator_command=None,
         simulator_arguments=None,
         initial_conditions={},
+        command_openvaf=COMMANDS["OPENVAF"],
+        copy_va_files=False,
+        inp_name="ngspice_circuit.ckt",
         **kwargs,
     ):
         if simulator_command is None:
             simulator_command = COMMANDS["NGSPICE"]
 
         if simulator_arguments is None:
             simulator_arguments = ["-r raw.raw", "-b "]
@@ -98,97 +114,182 @@
         }
         if simulator_options is not None:
             default_options.update(simulator_options)
 
         simulator_options = default_options
 
         self.initial_conditions = initial_conditions
-
-        # set temperature to find it easily later!
-        # simulator_options['Temp'] = r'{TEMP}'
+        self.devices_op_vars = []
+        self._osdi_imports = []
+        self.command_openvaf = command_openvaf
 
         super().__init__(
             database_dir,
             name,
             dut_type,
-            input_circuit,
+            inp_circuit,
             simulator_command=simulator_command,
             simulator_options=simulator_options,
             simulator_arguments=simulator_arguments,
-            inp_name="ngspice_circuit.ckt",
+            inp_name=inp_name,
+            copy_va_files=copy_va_files,
             **kwargs,
         )
 
+    def info_json(self, **_kwargs) -> Dict:
+        """Returns a dict with serializeable content for the json file to create.
+
+        The topmost dict MUST have only one key: The string casted class name.
+        Inside the parameters are:
+
+            * A version key,
+            * all extra parameters of DutNgspice compared to DutCircuit and
+            * the info_json of DutCircuit.
+
+        Returns
+        -------
+        dict
+            str(DutNgspice): serialized content
+        """
+
+        return {
+            str(DutNgspice): {
+                "__DutNgspice__": str(SEMVER_DUTNGSPICE_CURRENT),
+                "parent": super(DutNgspice, self).info_json(**_kwargs),
+                "initial_conditions": self.initial_conditions,
+                "devices_op_vars": self.devices_op_vars,
+                "_osdi_imports": self._osdi_imports,
+                "command_openvaf": self.command_openvaf,
+            }
+        }
+
+    @classmethod
+    def from_json(
+        cls,
+        json_content: Dict,
+        classes_technology: List[type[Technology]],
+        subclass_kwargs: Dict = None,
+    ) -> "DutNgspice":
+        """Static class method. Loads a DutNgspice object from a json or pickle file with full path save_dir.
+
+        Calls the from_json method of DutView with all dictionary inside the "parent" keyword. Afterwards the additional parameters are set correctly.
+
+        Parameters
+        ----------
+        json_content  :  dict
+            Readed dictionary from a saved json DutNgspice.
+        classes_technology : List[type[Technology]]
+            All possible technologies this loaded DutNgspice can have. One will be choosen according to the serialized technology loaded from the file.
+        subclass_kwargs : Dict, optional
+            Additional kwargs necessary to create the concrete subclassed DutView.
+
+        Returns
+        -------
+        DutNgspice
+            Loaded object.
+        """
+        if json_content["__DutNgspice__"] != SEMVER_DUTNGSPICE_CURRENT:
+            raise NotImplementedError("DMT.DutNgspice: Unknown version of DutNgspice to load!")
+
+        dut_view = super().from_json(
+            json_content["parent"], classes_technology, subclass_kwargs=subclass_kwargs
+        )
+        dut_view.initial_conditions = json_content["initial_conditions"]
+        dut_view.devices_op_vars = json_content["devices_op_vars"]
+        dut_view._osdi_imports = json_content["_osdi_imports"]
+        dut_view.command_openvaf = json_content["command_openvaf"]
+
+        return dut_view
+
     def create_inp_header(self, inp_circuit: Union[MCard, McParameterCollection, Circuit]):
         """Creates the input header of the given circuit description and returns it.
 
         Parameters
         ----------
         input : MCard or Circuit
             If a HICUM modelcard is given, a common emitter Circuit is created from it.
 
         Returns
         -------
         netlist : str
         """
+        use_osdi = bool(self.command_openvaf)  # False if None/null
+
         if isinstance(inp_circuit, MCard) or isinstance(inp_circuit, McParameterCollection):
             # save the modelcard, in case it was set inderectly via the input header!
             self._modelcard = copy.deepcopy(inp_circuit)
             # generate inp_circuit for netlist generation
-            inp_circuit = inp_circuit.get_circuit(**self.get_circuit_arguments)  # type: ignore
+            self._inp_circuit = inp_circuit.get_circuit(**self.get_circuit_arguments)  # type: ignore
+            if (
+                "use_build_in" in self.get_circuit_arguments
+                and self.get_circuit_arguments["use_build_in"]
+            ):
+                use_osdi = False
             # in case a standard circuit is used, this is the real input circuit
-            self._inp_circuit = inp_circuit
         elif isinstance(inp_circuit, Circuit):
             self._modelcard = None
             self._inp_circuit = copy.deepcopy(inp_circuit)
         else:
             raise OSError(
                 "For ADS circuits netlist generation is only possible from object of class DMT.classes.Circuit"
             )
 
+        self.devices_op_vars = []
         str_netlist = "DMT generated netlist\n"
         str_netlist += ".Options " + self._convert_dict_to_inp_line(self.simulator_options) + "\n"
 
-        # is a modelcard inside the netlist?
-        list_va_files = []
-        for element in inp_circuit.netlist:
-            try:
-                if (
-                    isinstance(inp_circuit, MCard)
-                    or isinstance(inp_circuit, McParameterCollection)
-                    and element.parameters.va_file is not None
-                ):
-                    list_va_files.append(element.parameters.va_file)
-            except AttributeError:
-                pass
+        if use_osdi:
+            # is a modelcard inside the netlist?
+            list_va_files = list()
+            for element in self._inp_circuit.netlist:
+                try:
+                    list_va_files.append(element.parameters.va_codes)
+                except AttributeError:
+                    # element does not have a va_file.
+                    pass
 
-        # load va files:
-        for va_file in list_va_files:
-            if self._copy_va_files:
-                self._list_va_file_contents.append(va_file)
-            else:
-                raise NotImplementedError("Absolute path of VA-File for NGSpice...")
-                if os.path.isfile(va_file):
-                    # file is relative to current cwd -> transform to absolute path
-                    va_file = os.path.abspath(va_file)
-                # else: file must be relative to simulation cwd -> nothing to do! Possible error is raised in simulation...
+            # pre_osdi strings
+            self._osdi_imports = []
+            for vafile in list_va_files:
+                if vafile is None:
+                    continue
+
+                self._list_va_file_contents.append(vafile)
+
+                if self._copy_va_files:
+                    # always add the relative path to va -> compile and use relative import in netlist
+                    self._osdi_imports.append(vafile.root)
+                else:
+                    # check if compiled file is already there and if yes, directly add ".osdi", else add ".va"
 
+                    va_hash = vafile.get_tree_hash()  # hash file content
+                    # check if plugin is already compiled and in the folder
+                    path_va = self.sim_dir / "VA_codes" / va_hash / vafile.root
+                    path_osdi = path_va.with_suffix(".osdi")
+
+                    if path_osdi.is_file():
+                        self._osdi_imports.append(path_osdi)
+                    else:
+                        # if not: add to "to_compile"
+                        self._osdi_imports.append(path_va)
+
+        self._osdi_imports = list(set(self._osdi_imports))  # unique...
         str_netlist += "\n* Netlist\n"
 
         # add elements:
-        for element in inp_circuit.netlist:
+        for index, element in enumerate(self._inp_circuit.netlist):
             if isinstance(element, str):
                 # pass
                 if re.match(r"^[\w_]+=", element):
                     # filters Variables -> ngspice does not need those
                     continue
 
                 str_netlist += element + "\n"
             else:
-                str_netlist += self._convert_CircuitElement_netlist(element)
+                str_netlist += self._convert_CircuitElement_netlist(element, index)
 
         logging.info("Successfully created input header of dut %s!", self.name)
         logging.debug("Content:\n%s", str_netlist)
 
         return str_netlist
 
     def make_input(self, sweep):
@@ -243,204 +344,230 @@
             # sorry :(, could be possible as soon as temperature sweeps are implemented. See add_temperature_sweep
             raise NotImplementedError("For ADS a temperature sweep has to be the outermost sweep!")
         else:
             # add the correct temperature sweep and remove it from sweepdefs
             str_netlist = self.inp_header + self.add_temperature_sweep(sweepdefs[0])
             del sweepdefs[0]
 
-        # output def
-        # TODO: dirty fix to debug ngspice..
-        # this is really messy...
-        # device_out = [
-        #     "temp",
-        #     "m",
-        #     "vbe",
-        #     "vbc",
-        #     "vce",
-        #     "vsc",
-        #     "vbbp",
-        #     "ic",
-        #     "ib",
-        #     "ie",
-        #     "iavl",
-        #     "is",
-        #     "ibei",
-        #     "ibci",
-        #     "it",
-        #     "vbiei",
-        #     "vbpbi",
-        #     "vbici",
-        #     "vciei",
-        #     "rcx_t",
-        #     "re_t",
-        #     "rbi",
-        #     "rb",
-        #     "betadc",
-        #     "gmi",
-        #     "gms",
-        #     "rpii",
-        #     "rpix",
-        #     "rmui",
-        #     "rmux",
-        #     "roi",
-        #     "cpii",
-        #     "cpix",
-        #     "cmui",
-        #     "cmux",
-        #     "ccs",
-        #     "betaac",
-        #     "crbi",
-        #     "tf",
-        #     "ft",
-        #     "ick",
-        #     "p",
-        #     "tk",
-        #     "dtsh",
-        # ]
-        # str_netlist += ".save all " + " ".join(["@Q_Q_H[{:s}]".format(out) for out in device_out])
-
         # ngspice control statement
         str_netlist += "\n\n.control\n"
 
+        # add pre_osdi
+        if self._osdi_imports:
+            print("\nPreparing OSDI Sources if needed.\n")
+
+        for osdi in self._osdi_imports:
+            try:
+                if osdi.suffix != ".osdi":
+                    # compile needed ? Could be compiled by a "parallel" simulation
+                    if not osdi.with_suffix(".osdi").is_file():
+                        process = subprocess.run(
+                            [self.command_openvaf, osdi.name], shell=False, cwd=osdi.parent
+                        )
+                        if process.returncode != 0:
+                            raise OSError(
+                                "DMT.DutNgspice: Run of OpenVAF failed!",
+                                f"The file to compile was {osdi}",
+                            )
+                    osdi = osdi.with_suffix(".osdi")
+
+                # import from common "VA_codes" folder
+                str_netlist += f"pre_osdi {osdi}\n"
+            except AttributeError:
+                # import from relative location
+                # compile always needed
+                process = subprocess.run(
+                    [self.command_openvaf, osdi], shell=False, cwd=self.get_sim_folder(sweep)
+                )
+                if process.returncode != 0:
+                    raise OSError(
+                        "DMT.DutNgspice: Run of OpenVAF failed!",
+                        f"The file to compile was {osdi} in {self.get_sim_folder(sweep)}",
+                    )
+
+                osdi = Path(osdi).with_suffix(".osdi")
+
+                # relative import
+                str_netlist += f"pre_osdi {osdi.name}\n"
+
+        # output def
+        str_netlist += "\nsave alli allv "
+        str_dc_output = ""
+        if tmp_sweep.outputdef:
+            if "OpVar" in tmp_sweep.outputdef:
+                str_dc_output += " ".join(self.devices_op_vars) + " "
+                tmp_sweep.outputdef.remove("OpVar")
+
+            # TODO find better way to use outputdef for ngspice
+            # current way does not work...
+            # str_dc_output += " ".join(tmp_sweep.outputdef)
+        str_netlist += str_dc_output
+
         # output settings
         str_netlist += (
-            "set filetype=ascii\n"
+            "\n\nset filetype=ascii\n"
             + "set appendwrite\n"
             + "set wr_vecnames\n"
             + "set wr_singlescale\n"
         )
 
         df = tmp_sweep.create_df()
-        ac = True
-        if not specifiers.FREQUENCY in df.columns:
-            # ac = False
-            df[specifiers.FREQUENCY] = 1e9
-
-        # from ngspice manual
-        # .ac dec nd fstart fstop-
-        # .ac oct no fstart fstop
-        # .ac lin np fstart fstop
+
+        # for AC use a table and only linear sweeps since:
+        # from ngspice manual ONLY lin can have only 1 freqency
 
         # find the AC sweep definition
         ac_statements = []
-        if ac:
-            for swd in sweepdefs:
-                if swd.var_name == specifiers.FREQUENCY:
-                    swd_type = swd.sweep_type
-                    swd_value_def = swd.value_def
-                    nfreq = swd_value_def[-1]
-                    if swd_type == "LOG":
-                        ac_statements.append(
-                            "ac dec {0:2.0f} {1:2.5e} {2:2.5e} \n".format(
-                                nfreq, 10 ** swd_value_def[0], 10 ** swd_value_def[1]
-                            )
-                        )
-                    elif swd_type == "CON":
-                        ac_statements.append(
-                            "ac dec 1 {0:2.5e} {0:2.5e} \n".format(swd_value_def[0])
-                        )
-                    elif swd_type == "LIN":
-                        ac_statements.append(
-                            "ac lin {0:2.0f} {1:2.5e} {2:2.5e} \n".format(
-                                nfreq, swd_value_def[0], swd_value_def[1]
-                            )
-                        )
-                    elif swd_type == "LIST":
-                        for val in swd_value_def:
-                            ac_statements.append("ac dec 1 {0:2.5e} {0:2.5e} \n".format(val))
-                    else:
-                        raise NotImplementedError
+        for swd in sweepdefs:
+            if swd.var_name == specifiers.FREQUENCY:
+                if swd.sweep_type == "LIN":  # TODO: more nice
+                    ac_statements.append(
+                        f"ac lin {swd.value_def[2]:g} {swd.value_def[0]:g} {swd.value_def[1]:g}\n"
+                    )
+                else:
+                    for freq in swd.values:
+                        ac_statements.append(f"ac lin 1 {freq:g} {freq:g}\n")
 
-            # remove all but one frequency from DF. We can then later put the "ac_statement" behind every DC point.
+        if ac_statements:
+            # remove all but one frequency from DF. We later put the "ac_statement" behind every DC point.
             freqs = df[specifiers.FREQUENCY]
             df = df[df[specifiers.FREQUENCY] == freqs[0]]
+        else:
+            df[specifiers.FREQUENCY] = 1e9  # default frequency...
+            ac_statements.append("ac lin 1 1e9 1e9 \n")
 
-        if not ac_statements:
-            ac_statements.append("ac dec 1 {0:2.5e} {0:2.5e} \n".format(1e9))
+        try:
+            # currently only 1 transient sweepdef per ngspice simulation (?)
+            swd_tran = next(swd for swd in sweepdefs if swd.var_name == specifiers.TIME)
+            if len(list(swd for swd in sweepdefs if swd.var_name == specifiers.TIME)) > 1:
+                raise IOError("Currently only one transient sweepdef per sweep in DutNgspice")
+            if len(swd_tran.value_def) > 1:
+                raise IOError("Currently only one transient simulation per sweep in DutNgspice")
+
+            # remove all but one time point from DF. We later let ngspice make the transient at every DC point.
+            time = df[specifiers.TIME]
+            df = df[df[specifiers.TIME] == time[0]]
+            df = df.drop(specifiers.TIME, axis=1)
+
+            # add transient signal to the correct voltage source
+            source_old = "V_V_{0} n_{0}X 0".format(swd_tran.contact)
+            if source_old not in str_netlist:
+                raise IOError(
+                    "DMT->DutNgspice: Did not find voltage source for transient signal input."
+                )
+
+            # if swd_tran.
+
+            sources_new = (
+                "V_V_{0} n_{0}_DC 0\n".format(swd_tran.contact)
+                + "V_V_{0}_tr n_{0}X n_{0}_DC ".format(swd_tran.contact)
+                + self._convert_swd_trans_to_pwl(swd_tran)
+                + " r=-1"
+            )
+            str_netlist = str_netlist.replace(source_old, sources_new)
+        except StopIteration:
+            swd_tran = False
+
+        # create vectors for each voltage
+        one_ele_array = False
+        for voltage_source in voltage_sources:
+            vals = df[voltage_source.name].to_numpy()
+            if (
+                len(vals) == 1
+            ):  # Ngspice does not support 1 element arrays ... so we just extend it.
+                vals = np.append(vals, vals)
+                one_ele_array = True
+            str_vec = (
+                "compose V_"
+                + voltage_source.name
+                + "_vec values "
+                + "".join(["(" + str(val) + ") " for val in vals])
+            )
+            str_netlist += str_vec + "\n"
 
-        # # #try to cast the analysis into a dc sweep ... convergence -> need to iterate over DMT sweepdef
-        # if not ac:
-        #     n_lin = 0
-        #     n_con = 0
-        #     for swd in sweepdefs:
-        #         if swd.sweep_type == 'CON':
-        #             n_con += 1
-        #         elif swd.sweep_type == 'LIN':
-        #             n_lin += 1
-        #         else:
-        #             continue
-
-        #     if n_lin == 1:
-        #         #only one linear sweep and no AC ... cast to ngspice sweep
-        #         sweepvar = None
-        #         for col in df.columns:
-        #             if 'V_' in col:
-        #                 vals = df[col].to_numpy()
-        #                 if len(np.unique(vals)) == 1:
-        #                     continue
-        #                 else:
-        #                     if all(np.diff(vals)==np.diff(vals)[0]):
-        #                         sweepvar = col
+            # compose ve_vec values 0 0 0 0 0 0 0 0 0 0 0
 
-        # so we have VOLTAGE sources and CURRENT sources and Frequency for every operating point.
-        for _index, row in df.iterrows():
-            for voltage_source in voltage_sources:
-                voltage_name = voltage_source.name
-                try:
-                    voltage = row[voltage_name]
-                except KeyError:
-                    voltage = 0
-                str_netlist += "alter V_" + str(voltage_name) + " = " + str(voltage) + "\n"
+        # TODO create vectors for each current source
 
-            for current_source in current_sources:
-                current_name = current_source.name.replace("S", "_")
-                try:
-                    current = row[current_name]
-                except KeyError:
-                    current = 0
-                str_netlist += "alter I_" + str(current_name) + " = " + str(current) + "\n"
-
-            # DC operating point analysis
-            # str_netlist += 'load\n' #try to find previous analysis results
-            str_netlist += "op\n"
-            # dc output statement
-
-            # #write to output
-            str_netlist += "wrdata output_ngspice_dc.ngspice all\n"
-
-            # #if we also need ac, lets go
-            if ac:
-                # set all ac magnitudes to zero
-                for voltage_source in voltage_sources:
-                    str_netlist += "alter V_" + voltage_source.name + " ac=0\n"
-
-                # turn on one voltage source at a time and save the results of ac analysis
-                for ac_statement in ac_statements:
-                    # turn on source
-
-                    # ac analysis statement
-                    # ngspice ac format: dec n_points f_start f_stop
-                    # dmt sweep format : log_10(fstart) log_10(fstop) n_points
-                    for voltage_source in voltage_sources:
-                        str_netlist += "alter V_" + voltage_source.name + " ac=1\n"
-                        str_netlist += ac_statement
-                        # ac output statement -> move to end?
-                        str_netlist += (
-                            "wrdata output_ngspice_ac_"
-                            + voltage_source.name
-                            + ".ngspice alli allv\n"
-                        )
-
-                        # turn off source
-                        str_netlist += "alter V_" + voltage_source.name + " ac=0\n"
+        n_bias = len(vals)
+        if one_ele_array:  # special case: just one OP to simulate
+            n_bias = n_bias - 1
+        str_netlist += "let index=0\n"
+        str_netlist += "while index<" + str(int(n_bias)) + "\n"
 
-                    str_netlist += "unset wr_vecnames\n"
+        # so we have VOLTAGE sources and CURRENT sources and Frequency for every operating point.
+        str_netlist += "    *set value of all voltage sources:\n"
+        for voltage_source in voltage_sources:
+            voltage_name = voltage_source.name
+            str_netlist += (
+                "    alter V_" + str(voltage_name) + " = V_" + str(voltage_name) + "_vec[index]\n"
+            )
+            # alter V_V_E = ve_vec[index]
 
-            str_netlist += "unset wr_vecnames\n"
+        # for current_source in current_sources:
+        #     current_name = current_source.name.replace("S", "_")
+        #     try:
+        #         current = row[current_name]
+        #     except KeyError:
+        #         current = 0
+        #     str_netlist += "alter I_" + str(current_name) + " = " + str(current) + "\n"
+
+        str_netlist += "    let index=index+1\n"
+
+        # DC operating point analysis
+        # str_netlist += 'load\n' #try to find previous analysis results
+        str_netlist += "    *perform DC analysis and write output:\n"
+        str_netlist += "    op\n"
+        # dc output statement
+
+        # #write to output
+        str_netlist += f"    wrdata output_ngspice_dc.ngspice alli allv {str_dc_output}\n"
+
+        # Add AC
+        # set all ac magnitudes to zero
+        str_netlist += "    *set AC mag of all sources equal zero\n"
+        for voltage_source in voltage_sources:
+            str_netlist += "    alter V_" + voltage_source.name + " ac=0\n"
+
+        # turn on one voltage source at a time and save the results of ac analysis
+        str_netlist += "    *turn on one AC source at a time and perform analysis\n"
+        for i_ac_statement, ac_statement in enumerate(ac_statements):
+            # turn on source
+
+            # ac analysis statement
+            # ngspice ac format: dec n_points f_start f_stop
+            # dmt sweep format : log_10(fstart) log_10(fstop) n_points
+            for voltage_source in voltage_sources:
+                str_netlist += "    alter V_" + voltage_source.name + " ac=1\n"
+                str_netlist += "    " + ac_statement
+                # ac output statement -> move to end?
+                str_netlist += (
+                    "    wrdata output_ngspice_ac_" + voltage_source.name + ".ngspice alli allv\n"
+                )
+
+                # turn off source
+                str_netlist += "    alter V_" + voltage_source.name + " ac=0\n"
+
+            if i_ac_statement == 0:
+                str_netlist += "    unset wr_vecnames\n"
+
+        # Add transients
+        if swd_tran:
+            for i_tr, freq in enumerate(swd_tran.value_def):
+                tau = 1 / freq
+
+                str_netlist += (
+                    "set wr_vecnames\n"
+                    + f"tran {tau/40} {3*tau}\n"
+                    + f"wrdata output_ngspice_tr_{i_row}_{i_tr}.ngspice_tr alli allv\n"
+                    + "unset wr_vecnames\n"
+                )
 
+        str_netlist += "    unset wr_vecnames\n"
+        str_netlist += "end\n"
         str_netlist += ".endc\n" + ".end\n"
 
         logging.info("Added sweepdefs to input header.")
         logging.debug("\n%s", str_netlist)
         return str_netlist
 
     def add_temperature_sweep(self, temp_def):
@@ -475,27 +602,43 @@
 
         # find .ngspice file
         for my_file in os.listdir(sim_folder):
             filename = os.fsdecode(my_file)
             if filename.endswith(".ngspice"):
                 break
 
-        # find .ngspice file
-        dfs = []
-        for root, _dors, files in os.walk(sim_folder):  # . filter
-            for my_file in files:
-                filename = my_file
-                if filename.endswith(".ngspice"):
-                    df = self.read_ngspice(os.path.join(root, filename))
-                    dfs.append(self.clean_df(df, filename))
-
-        df_joined = self.join(dfs)
+        # find .ngspice files (these are DC and AC)
+        files_dc_ac = [sim_file for sim_file in sim_folder.glob("*.ngspice")]
+        # are there transient simulations?
+        files_tran = sorted(sim_file for sim_file in sim_folder.glob("*.ngspice_tr"))
 
         key = self.join_key(self.get_sweep_key(sweep), "iv")
-        self.data[key] = df_joined
+        dfs_dc_ac = [
+            _read_clean_ngspice_df(
+                sim_file,
+                self.nodes,
+                self.reference_node,
+                self.ac_ports,
+            )
+            for sim_file in files_dc_ac
+        ]
+        self.data[key] = self.join(dfs_dc_ac)
+
+        keys_tr = [
+            self.join_key(self.get_sweep_key(sweep), sim_tr_file.stem[15:])
+            for sim_tr_file in files_tran
+        ]
+        dfs_tr = [
+            _read_clean_ngspice_df_transient(sim_tr_file, self.reference_node, self.ac_ports)
+            for sim_tr_file in files_tran
+        ]
+
+        for key, df in zip(keys_tr, dfs_tr):
+            self.data[key] = df
+
         logging.info(
             "Read the NGSpice simulation output data of the sweep %s. \nThe simulation folder is %s",
             sweep.name,
             sim_folder,
         )
 
         sim_log = os.path.join(sim_folder, "sim.log")
@@ -503,190 +646,14 @@
             log_content = my_log.read()
         search_obj_time = re.search(
             r"User time(.+?)Total stopwatch time", log_content, flags=re.IGNORECASE | re.DOTALL
         )
         if search_obj_time:
             logging.info("Simulation times: %s.", search_obj_time.group(1))
 
-    def read_ngspice(self, filename):
-        """read the ngspice output file"""
-        # open file
-        with open(filename) as my_file:
-            list_lines = my_file.readlines()
-
-        # this seems to be printed for verilog modules... probably bracnh currents, however node is missing?
-        list_lines[0] = list_lines[0].replace("#no info", "#no_info")
-
-        # get column names
-        list_lines = [line.strip() for line in list_lines]
-        split_header = list_lines[0].split()
-        is_ac = False
-        if "frequency" in split_header:
-            is_ac = True  # this ia an ac simulation
-
-        # put all numeric values in large array and fill row by row taking n_data chunks
-        # this omits the issue with line breaks produced e.g. by DEVICE
-        list_lines = " ".join(list_lines[1:])
-        list_lines = list_lines.split()
-        list_lines = np.array([float(i) for i in list_lines])
-        n_col = float(len(split_header))
-        n_row = float(len(list_lines) / n_col)
-
-        # check if n_row is an integer
-        if n_row.is_integer():
-            n_row = int(n_row)
-        else:
-            raise IOError(
-                "DMT -> Data_reader: Encountered a weird number of rows in "
-                + filename
-                + ". Contact Markus Mueller."
-            )
-
-        # check if n_col is an integer
-        if n_col.is_integer():
-            n_col = int(n_col)
-        else:
-            raise IOError(
-                "DMT -> Data_reader: Encountered a weird number of cols in "
-                + filename
-                + ". Contact Markus Mueller."
-            )
-
-        # need to cast real valued stuff to complex...headache
-        if is_ac:
-            # cast values to complex...simpler later
-            n_col = int((n_col - 1) / 2 + 1)
-            list_lines_cmplx = np.zeros(n_row * n_col, dtype=np.complex128)
-            index_cmplx = 0  # index to list_lines_cmplx
-            index_real = 0  # index to list_lines
-            for n in range(n_row):
-                for i in range(n_col):
-                    if i == 0:
-                        list_lines_cmplx[index_cmplx] = list_lines[index_real]
-                        index_real += 1
-                    else:
-                        list_lines_cmplx[index_cmplx] = (
-                            list_lines[index_real] + 1j * list_lines[index_real + 1]
-                        )
-                        index_real += 2
-
-                    index_cmplx += 1
-
-            if index_cmplx != len(list_lines_cmplx):
-                raise IOError("DMT -> NGSPICE: error during ac import.")
-
-            list_lines = list_lines_cmplx
-
-            # now cast split_header
-            new_header = []
-            new_header.append(split_header[0])
-            for n in range(n_col - 1):
-                new_header.append(split_header[1 + n * 2])
-
-            split_header = new_header
-
-        # fill the data into the 2-dimensional array data_raw
-        data_raw = np.empty([n_row, n_col], dtype=np.complex128)
-        for i in range(n_row):
-            data_raw[i, :] = list_lines[n_col * i : n_col * (i + 1)]
-
-        # initalize pd.Dataframe() and return it
-        return DataFrame(data_raw, columns=split_header)
-
-    def clean_df(self, df, filename):
-        """From the df as read directly from ngspice, create a df that has DMT specifiers and is suitable for modeling."""
-        df = df.loc[:, ~df.columns.duplicated()]  # drop duplicate columns
-        cols = df.columns
-        nodes = [col[2:].upper() for col in cols if col[0:2] == "n_"]
-
-        is_ac = False
-        if "frequency" in cols:
-            is_ac = True
-
-        new_df = DataFrame()
-        op_vars = []
-        for col in cols:
-            col_raw = col.upper()
-            if "#BRANCH" in col_raw:  # current that we should save
-                col_raw = col_raw.replace("#BRANCH", "")
-                node = next(node for node in nodes if node in col_raw)
-                new_df[specifiers.CURRENT + node] = -df[col]  # we want the other current direction
-            elif col_raw[0:2] == "N_":  # found a node, will take the voltage
-                node = col_raw[2:]
-                if "_FORCED" in node:
-                    new_df[
-                        specifiers.VOLTAGE + node.replace("_FORCED", "") + sub_specifiers.FORCED
-                    ] = df[col]
-                else:
-                    new_df[specifiers.VOLTAGE + node] = df[col]
-            elif col_raw == "FREQUENCY":
-                new_df[specifiers.FREQUENCY] = np.real(df["frequency"].to_numpy())
-
-            # add opvars
-            regexp = r"\[(.*)\]"
-            m = re.search(regexp, col_raw)
-            if m:
-                op_var = m.groups()[0]
-                new_df[op_var] = np.real(df[col].to_numpy())
-                op_vars.append(op_var)
-
-        # dirty: add the Y Parameters
-        if is_ac:
-            # step one: find which port is begin excited
-            node_excited = re.search(r"V_(\w+?)\.ngspice", filename).group(1)
-            col_v_ne = specifiers.VOLTAGE + node_excited
-            ac_voltage = 1  # fallback
-
-            try:
-                ac_voltage = new_df[col_v_ne].to_numpy()
-                ac_voltage = new_df[col_v_ne + sub_specifiers.FORCED].to_numpy()
-            except KeyError:
-                pass
-            try:
-                new_df.drop(axis=1, columns=col_v_ne, inplace=True)
-            except KeyError:
-                pass
-            try:
-                new_df.drop(axis=1, columns=col_v_ne + sub_specifiers.FORCED, inplace=True)
-            except KeyError:
-                pass
-
-            # delete the AC voltages, because why would anyone need them.
-            for node in self.nodes:
-                col_v_n = specifiers.VOLTAGE + node
-                try:
-                    new_df.drop(axis=1, columns=col_v_n, inplace=True)
-                except KeyError:
-                    pass
-                try:
-                    new_df.drop(axis=1, columns=col_v_n + sub_specifiers.FORCED, inplace=True)
-                except KeyError:
-                    pass
-
-            # step2: now calculate the y parameters Y(X,node)
-            for node_2 in self.nodes:
-                col_i_n = specifiers.CURRENT + node_2
-                if col_i_n in new_df.columns:
-                    ac_current = new_df[col_i_n].to_numpy()
-                    new_df.drop(axis=1, columns=col_i_n, inplace=True)
-
-                    y_para = specifiers.SS_PARA_Y + [node_2, node_excited]
-                    new_df[y_para] = ac_current / ac_voltage
-
-        fallback_dict = {}
-        for op_var in op_vars:
-            fallback_dict[op_var] = op_var
-        return new_df.clean_data(
-            nodes,
-            self.reference_node,
-            ac_ports=self.ac_ports,
-            fallback=fallback_dict,
-            warnings=False,
-        )
-
     def validate_simulation_successful(self, sweep):
         """Checks if the simulation of the given sweep was successful.
 
         Parameters
         ----------
         sweep  :  :class:`DMT.core.sweep.Sweep`
             Sweep that has been simulated.
@@ -762,15 +729,15 @@
         Returns
         -------
         str
             Line to add into input file
         """
         str_return = ""
 
-        for (key, param) in dict_key_para.items():
+        for key, param in dict_key_para.items():
             if isinstance(param, str):
                 str_add = key + "=" + param + " "
             elif isinstance(param, (list, tuple)):
                 str_add = key + "=" + " ".join([str(nr) for nr in param]) + " "
             elif isinstance(param, bool):
                 str_add = "yes" if param else "no"
                 str_add = key + "=" + str_add
@@ -779,15 +746,15 @@
             else:
                 str_add = key + "=" + str(param) + " "
 
             str_return = str_return + str_add
 
         return str_return
 
-    def _convert_CircuitElement_netlist(self, circuit_element):
+    def _convert_CircuitElement_netlist(self, circuit_element, index):
         """Transforms a :class:`~DMT.classes.circuit.CircuitElement` into a string fitting for NGspice.
 
         Parameters
         ----------
         circuit_element
             CircuitElement to transform
 
@@ -803,133 +770,140 @@
         #     )
 
         # map dmt circuit element_type to ngspice element types
         # only those that differ between DMT definiton and NGspice definition are listed here
         element_types = {
             VOLTAGE: "V",
             CURRENT: "I",
-            "hicumL2va": "Q",
-            "hicumL2_test": "Q",
             HICUML2_HBT: "Q",
             SGP_BJT: "Q",
             "bjtn": "Q",
         }
         if circuit_element.element_type in element_types.keys():
             element_type = element_types[circuit_element.element_type]
         elif circuit_element.element_type == SHORT:
             element_type = "V"
             circuit_element.name = "V_" + circuit_element.name.replace("I", "V")
             circuit_element.parameters = [("dc", str(0)), ("ac", str(0))]
             circuit_element.contact_nodes = (
                 circuit_element.contact_nodes[1],
                 circuit_element.contact_nodes[0],
             )
+        elif (
+            isinstance(circuit_element.parameters, MCard)
+            and circuit_element.parameters.va_codes is not None
+        ):
+            element_type = "N"
         else:
             element_type = circuit_element.element_type
 
         str_netlist = f"{element_type}_{circuit_element.name} " + " ".join(
             circuit_element.contact_nodes
         )
         if circuit_element.parameters is not None:
             if isinstance(circuit_element.parameters, MCard):
                 str_temp = "+ "
+                mcard = circuit_element.parameters
 
-                if circuit_element.element_type in ["hicumL2va", HICUML2_HBT, "hicumL2_test"]:
-                    mcard = circuit_element.parameters
+                if circuit_element.element_type == HICUML2_HBT:
                     str_instance_parameters = ""
                     str_model_parameters = ""
                     str_type = "NPN"
                     for para in sorted(mcard.paras, key=lambda x: (x.group, x.name)):
                         if para.name == "type":
                             str_type = "NPN" if (para.value == 1) else "PNP"
                         elif para.name in [
                             "dt",
                         ]:  # here all instance parameters
                             str_instance_parameters += "{0:s}={0:10.10e} ".format(para)
                         else:  # here all model parameters
                             str_model_parameters += "{0:s}={0:10.10e} ".format(para)
 
-                    for (key, val) in self.initial_conditions.items():
+                    for key, val in self.initial_conditions.items():
                         # dirty to allow debugging ngspice
                         str_model_parameters += "{0:s}={1:10.10e} ".format(key, val)
                     str_temp = (
-                        f"hicum_va {str_instance_parameters}\n"  # we should count here somehow the models
-                        + f".model hicum_va {str_type} level=8\n"
-                        + f"+ {str_model_parameters}"
+                        f"hicum_build_in{index:d} {str_instance_parameters}\n"  # we should count here somehow the models
+                        + f".model hicum_build_in{index:d} {str_type} level=8 {str_model_parameters}"
                     )
                 elif circuit_element.element_type in [SGP_BJT, "bjtn"]:
-                    mcard = circuit_element.parameters
                     str_instance_parameters = ""
                     str_model_parameters = ""
                     str_type = "NPN"
                     for para in sorted(mcard.paras, key=lambda x: (x.group, x.name)):
                         if para.name == "type":
                             str_type = "NPN" if (para.value == 1) else "PNP"
                         elif para.name in []:  # here all instance parameters
                             str_instance_parameters += "{0:s}={0:10.10e} ".format(para)
                         else:  # here all model parameters
                             str_model_parameters += "{0:s}={0:10.10e} ".format(para)
 
-                    for (key, val) in self.initial_conditions.items():
+                    for key, val in self.initial_conditions.items():
                         # dirty to allow debugging ngspice
                         str_model_parameters += "{0:s}={1:10.10e} ".format(key, val)
                     str_temp = (
-                        f"QMOD {str_instance_parameters}\n"  # we should count here somehow the models
-                        + f".model QMOD {str_type} level=1\n"
-                        + f"+ {str_model_parameters}"
+                        f"QMOD{index:d} {str_instance_parameters}\n"  # we should count here somehow the models
+                        + f".model QMOD{index:d} {str_type} level=1 {str_model_parameters}"
                     )
-                elif circuit_element.element_type in [DIODE]:
-                    mcard = circuit_element.parameters
-                    str_instance_parameters = ""
-                    str_model_parameters = ""
-                    str_type = "NPN"
-                    additional_str = ""
-                    for para in sorted(mcard.paras, key=lambda x: (x.group, x.name)):
-                        if para.name == "osdi":
-                            if para - value == 1:
-                                additional_str = " osdi " + circuit_element.name
-                        str_model_parameters += "{0:s}={0:10.10e} ".format(para)
-
-                    str_temp = f"\n.model dmod {additional_str} d( {str_model_parameters} )"  # we should count here somehow the models
                 elif "sky130_fd_pr" in circuit_element.element_type:
                     # skywater 130 device
-                    mcard = circuit_element.parameters
                     str_instance_parameters = ""
 
                     for para in sorted(mcard.paras, key=lambda x: (x.group, x.name)):
                         str_instance_parameters += "{0:s}={0:10.10e} ".format(para)
 
                     str_netlist = (
                         f'.lib "{mcard.pdk_path}" {mcard.pdk_corner}\n'
                         + f"{circuit_element.name} "
                         + " ".join(circuit_element.contact_nodes)
                     )
                     str_temp = f"{circuit_element.element_type} {str_instance_parameters}"
+                elif circuit_element.parameters.va_codes is not None:
+                    str_instance_parameters = ""
+                    str_model_parameters = ""
+                    for para in sorted(mcard.paras, key=lambda x: (x.group, x.name)):
+                        if (
+                            para.name in []
+                        ):  # here all instance parameters TODO after next verilogae release
+                            str_instance_parameters += "{0:s}={0:10.10e} ".format(para)
+                        else:  # here all model parameters
+                            str_model_parameters += "{0:s}={0:10.10e} ".format(para)
+
+                    str_temp = (
+                        f"model_va{index:d} {str_instance_parameters}\n"  # we should count here somehow the models
+                        + f".model model_va{index:d} {circuit_element.parameters.default_module_name} {str_model_parameters}"
+                    )
                 else:
                     raise NotImplementedError(
                         f"The element type {circuit_element.element_type} is not implemented for ngspice.",
                         "Check the ngspice manual if this type needs special treatment and implement it accordingly.",
                     )
+
+                self.devices_op_vars += [
+                    f"@{element_type}_{circuit_element.name}[{op_var:s}]"
+                    for op_var in mcard.op_vars
+                ]
+
             else:
                 str_temp = []
-                for (para, value) in circuit_element.parameters:
+                for para, value in circuit_element.parameters:
                     if para in ["C", "R", "L"]:  # rename according to ngspice manual
                         str_temp.append(value)
-                    elif para in ["Vdc", "Vac"] and not isinstance(
+                    elif para in ["Vdc", "Vac", "Idc", "Iac"] and not isinstance(
                         value, float
                     ):  # just leave voltages from lines, as ngpsice directly changes the sources and not the parameters
                         pass
                     else:
                         str_temp.append(para + "=" + value)
 
                 str_temp = " ".join(str_temp)
 
                 # find sim paras
                 sim_paras = ""
-                for (para, value) in circuit_element.parameters:
+                for para, value in circuit_element.parameters:
                     try:
                         float(value)
                     except ValueError:
                         sim_paras = sim_paras + value + "=0 "
 
                 if sim_paras != "":
                     sim_paras = "\n.param " + sim_paras
@@ -944,14 +918,20 @@
             str_temp = str_temp.replace("Iac=", "ac ")
         else:
             str_temp = ""
 
         str_netlist = str_netlist.replace("IS", "I_")
         return str_netlist + " " + str_temp + "\n"
 
+    def _convert_swd_trans_to_pwl(self, swd_tran: SweepDef):
+        time = swd_tran.values
+        signal = swd_tran.get_input_signal()
+        pwl = " ".join([f"{t:g} {s:g}" for t, s in zip(time, signal)])
+        return " PWL(" + pwl + ")"
+
     def join(self, dfs):
         """Join DC and AC dataframes into one dataframe"""
         dfs_ac = [df for df in dfs if "FREQ" in df.columns]
         df_dc = next(df for df in dfs if not "FREQ" in df.columns)
         if not dfs_ac:
             return df_dc
 
@@ -960,20 +940,261 @@
         for freq in freqs:
             if (freq == freqs[0]).all():
                 continue
             else:
                 raise IOError("DMT -> NGspice: frequencies of AC simulation data do not match.")
 
         # join the ac dataframes into one ac dataframe dfs_ac[0]
-        df_ac = dfs_ac[0]
-        for df in dfs_ac[1:]:
-            for y_param in [col for col in df.columns if col.specifier == specifiers.SS_PARA_Y]:
-                df_ac[y_param] = df[y_param].to_numpy()
+        for i_df in range(len(dfs_ac)):
+            df = dfs_ac[i_df]
+            if i_df == 0:
+                y_cols = [specifiers.FREQUENCY]
+            else:
+                y_cols = []
+
+            for col in df.columns:
+                try:
+                    if col.specifier == specifiers.SS_PARA_Y:
+                        y_cols.append(col)
+                except AttributeError:
+                    pass  # from AC dataframes ONLY the SS paras are copied other, rest is ignored
+
+            dfs_ac[i_df] = df[y_cols]
+
+        df_ac = pd.concat(dfs_ac, axis=1)
 
         # join the dc data to the ac data
         n_freq = len(np.unique(freqs[0]))
-        for col in df_dc.columns:
-            vals = df_dc[col].to_numpy()
-            vals = np.repeat(vals, n_freq)
-            df_ac[col] = vals
+        df_dc = DataFrame(df_dc.values.repeat(n_freq, axis=0), columns=df_dc.columns)
+
+        df_dc.reset_index(drop=True, inplace=True)
+        df_ac.reset_index(drop=True, inplace=True)
+        return pd.concat([df_dc, df_ac], axis=1)
+
+
+def _read_ngspice(filename):
+    """read the ngspice output file"""
+    # open file
+    with open(filename) as my_file:
+        list_lines = my_file.readlines()
+
+    # this seems to be printed for verilog modules... probably branch currents, however node is missing?
+    list_lines[0] = list_lines[0].replace("#no info", "#no_info")
+
+    # get column names
+    list_lines = [line.strip() for line in list_lines]
+    split_header = list_lines[0].split()
+    is_ac = False
+    if "frequency" in split_header:
+        is_ac = True  # this ia an ac simulation
+
+    # put all numeric values in large array and fill row by row taking n_data chunks
+    # this omits the issue with line breaks produced e.g. by DEVICE
+    list_lines = " ".join(list_lines[1:])
+    list_lines = list_lines.split()
+    list_lines = np.array(list_lines, dtype=np.float64)
+    n_col = float(len(split_header))
+    n_row = float(len(list_lines) / n_col)
+
+    # check if n_row is an integer
+    if n_row.is_integer():
+        n_row = int(n_row)
+    else:
+        raise IOError("DMT -> Data_reader: Encountered a weird number of rows in " + filename + ".")
+
+    # check if n_col is an integer
+    if n_col.is_integer():
+        n_col = int(n_col)
+    else:
+        raise IOError("DMT -> Data_reader: Encountered a weird number of cols in " + filename + ".")
+
+    # need to cast real valued stuff to complex...headache
+    if is_ac:
+        # cast values to complex...simpler later
+        n_col = int((n_col - 1) / 2 + 1)
+        list_lines_cmplx = np.zeros(n_row * n_col, dtype=np.complex128)
+        index_cmplx = 0  # index to list_lines_cmplx
+        index_real = 0  # index to list_lines
+        for n in range(n_row):
+            for i in range(n_col):
+                if i == 0:
+                    list_lines_cmplx[index_cmplx] = list_lines[index_real]
+                    index_real += 1
+                else:
+                    list_lines_cmplx[index_cmplx] = (
+                        list_lines[index_real] + 1j * list_lines[index_real + 1]
+                    )
+                    index_real += 2
+
+                index_cmplx += 1
+
+        if index_cmplx != len(list_lines_cmplx):
+            raise IOError("DMT -> NGSPICE: error during ac import.")
+
+        list_lines = list_lines_cmplx
+
+        # now cast split_header
+        new_header = []
+        new_header.append(split_header[0])
+        for n in range(n_col - 1):
+            new_header.append(split_header[1 + n * 2])
+
+        split_header = new_header
+
+    # fill the data into the 2-dimensional array data_raw
+    data_raw = np.empty([n_row, n_col], dtype=np.complex128)
+    for i in range(n_row):
+        data_raw[i, :] = list_lines[n_col * i : n_col * (i + 1)]
+
+    # initalize pd.Dataframe() and return it
+    return DataFrame(data_raw, columns=split_header)
+
+
+def _read_clean_ngspice_df(filepath, nodes, reference_node, ac_ports):
+    """From the df as read directly from ngspice, create a df that has DMT specifiers and is suitable for modeling."""
+    df = _read_ngspice(filepath)
+    df = df.loc[:, ~df.columns.duplicated()]  # drop duplicate columns
+    cols = df.columns
+    nodes = [col[2:].upper() for col in cols if col[0:2] == "n_"]
+
+    is_ac = False
+    if "frequency" in cols:
+        is_ac = True
+
+    # check if more than one device has OpVars
+    op_vars = []
+    op_var_devices = set()
+    for col in cols:
+        if col.startswith("@"):
+            i_bracket = col.find("[")
+            op_var_devices.add(col[1:i_bracket].upper())
+
+    if len(op_var_devices) > 1:
+        op_var_multi = True
+    else:
+        op_var_multi = False
+
+    data = {}
+    for col in cols:
+        col_raw = col.upper()
+        if "#BRANCH" in col_raw:  # current that we should save
+            col_raw = col_raw.replace("#BRANCH", "")
+            node = next(node for node in nodes if node in col_raw)
+            data[specifiers.CURRENT + node] = -df[col]  # we want the other current direction
+        elif col_raw[0:2] == "N_":  # found a node, will take the voltage
+            node = col_raw[2:]
+            if "_FORCED" in node:
+                data[specifiers.VOLTAGE + node.replace("_FORCED", "") + sub_specifiers.FORCED] = df[
+                    col
+                ]
+            else:
+                data[specifiers.VOLTAGE + node] = df[col]
+        elif col_raw == "FREQUENCY":
+            data[specifiers.FREQUENCY] = np.real(df["frequency"].to_numpy())
+
+        # add opvars
+        if col_raw.startswith("@"):
+            if op_var_multi:
+                dev_op_var = re.search(r"@(.*)\[(.*)\]", col_raw)
+                op_var = "{0}.{1}".format(*dev_op_var.groups()).upper()
+                data[op_var] = np.real(df[col].to_numpy())
+                op_vars.append(op_var)
+            else:
+                op_var = re.search(r"\[(.*)\]", col_raw).groups()[0].upper()
+                data[op_var] = np.real(df[col].to_numpy())
+                op_vars.append(op_var)
 
-        return df_ac
+    new_df = DataFrame(data)
+
+    # dirty: add the Y Parameters
+    if is_ac:
+        # step one: find which port is begin excited
+        node_excited = re.search(r"V_(\w+?)$", filepath.stem).group(1)
+        col_v_ne = specifiers.VOLTAGE + node_excited
+        ac_voltage = 1  # fallback
+
+        try:
+            ac_voltage = new_df[col_v_ne].to_numpy()
+            ac_voltage = new_df[col_v_ne + sub_specifiers.FORCED].to_numpy()
+        except KeyError:
+            pass
+        try:
+            new_df.drop(axis=1, columns=col_v_ne, inplace=True)
+        except KeyError:
+            pass
+        try:
+            new_df.drop(axis=1, columns=col_v_ne + sub_specifiers.FORCED, inplace=True)
+        except KeyError:
+            pass
+
+        # delete the AC voltages, because why would anyone need them.
+        for node in nodes:
+            col_v_n = specifiers.VOLTAGE + node
+            try:
+                new_df.drop(axis=1, columns=col_v_n, inplace=True)
+            except KeyError:
+                pass
+            try:
+                new_df.drop(axis=1, columns=col_v_n + sub_specifiers.FORCED, inplace=True)
+            except KeyError:
+                pass
+
+        # step2: now calculate the y parameters Y(X,node)
+        for node_2 in nodes:
+            col_i_n = specifiers.CURRENT + node_2
+            if col_i_n in new_df.columns:
+                ac_current = new_df[col_i_n].to_numpy()
+                new_df.drop(axis=1, columns=col_i_n, inplace=True)
+
+                y_para = specifiers.SS_PARA_Y + [node_2, node_excited]
+                new_df[y_para] = ac_current / ac_voltage
+
+    fallback_dict = {}
+    for op_var in op_vars:
+        fallback_dict[op_var] = op_var
+    return new_df.clean_data(
+        nodes,
+        reference_node,
+        ac_ports=ac_ports,
+        fallback=fallback_dict,
+        warnings=False,
+    )
+
+
+def _read_clean_ngspice_df_transient(filepath, reference_node, ac_ports):
+    """From the df as read directly from ngspice, create a df that has DMT specifiers and is suitable for modeling."""
+    df = _read_ngspice(filepath)
+    df = df.loc[:, ~df.columns.duplicated()]  # drop duplicate columns
+    cols = df.columns
+    nodes = [col[2:].upper() for col in cols if col[0:2] == "n_"]
+
+    new_df = DataFrame()
+    for col in cols:
+        # opvars are not set transient..
+        if col.startswith("@"):
+            continue
+
+        col_raw = col.upper()
+        if "#BRANCH" in col_raw:  # current that we should save
+            col_raw = col_raw.replace("#BRANCH", "")
+            node = next(node for node in nodes if node in col_raw)
+            new_df[specifiers.CURRENT + node] = -df[col]  # we want the other current direction
+        elif col_raw[0:2] == "N_":  # found a node, will take the voltage
+            node = col_raw[2:]
+            if "_FORCED" in node:
+                new_df[
+                    specifiers.VOLTAGE + node.replace("_FORCED", "") + sub_specifiers.FORCED
+                ] = df[col]
+            else:
+                new_df[specifiers.VOLTAGE + node] = df[col]
+        elif col_raw == "FREQUENCY":
+            new_df[specifiers.FREQUENCY] = np.real(df["frequency"].to_numpy())
+        elif col_raw == "TIME":
+            new_df[specifiers.TIME] = np.real(df["time"].to_numpy())
+
+    return new_df.clean_data(
+        nodes,
+        reference_node,
+        ac_ports=ac_ports,
+        fallback={specifiers.TIME: specifiers.TIME},
+        warnings=False,
+    )
```

### Comparing `DMT_core-1.8.0rc1/DMT/xyce/__init__.py` & `DMT_core-2.0.0/DMT/xyce/__init__.py`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/DMT/xyce/dut_xyce.py` & `DMT_core-2.0.0/DMT/xyce/dut_xyce.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,58 +24,68 @@
 import re
 import subprocess
 import warnings
 import numpy as np
 import pandas as pd
 import time
 from pathlib import Path
+from typing import List, Dict
+
+try:
+    from semver.version import Version as VersionInfo
+except ImportError:
+    from semver import VersionInfo
 
 from DMT.config import DATA_CONFIG
 from DMT.core import (
     DutCircuit,
     DutType,
     McParameterCollection,
     MCard,
     Sweep,
     SweepDef,
     specifiers,
     sub_specifiers,
     SpecifierStr,
     DataFrame,
-    create_md5_hash,
     constants,
     print_progress_bar,
+    Technology,
+    VAFileMap,
 )
 from DMT.core.circuit import (
     Circuit,
     RESISTANCE,
     INDUCTANCE,
     CAPACITANCE,
     VOLTAGE,
     CURRENT,
     SHORT,
     HICUML2_HBT,
     SGP_BJT,
 )
 from DMT.exceptions import SimulationUnsuccessful, SimulationFail
 
+SEMVER_DUTXYCE_CURRENT = VersionInfo(major=1, minor=0)
+
 
 class DutXyce(DutCircuit):
     """Class to interface the Xyce circuit simulator"""
 
     def __init__(
         self,
         database_dir,
         dut_type,
-        input_circuit,
+        inp_circuit,
         name="xyce_",
         simulator_command=None,
         simulator_arguments=None,
         simulator_options=None,
         build_xyce_plugin_command="buildxyceplugin",
+        inp_name="xyce_circuit.cir",
         **kwargs,
     ):
         if simulator_command is None:
             simulator_command = DATA_CONFIG["commands"]["XYCE"]
 
         default_options = {}
         if simulator_options is not None:
@@ -88,29 +98,96 @@
         self.build_xyce_plugin_command = build_xyce_plugin_command
         self._va_plugins_to_compile = []
 
         super().__init__(
             database_dir,
             name,
             dut_type,
-            input_circuit,
+            inp_circuit,
             simulator_command=simulator_command,
             simulator_options=simulator_options,
             simulator_arguments=simulator_arguments,
-            inp_name="xyce_circuit.cir",
+            inp_name=inp_name,
             **kwargs,
         )
 
         if self.simulate_on_server:
             raise NotImplementedError(
                 "Running Xyce on a Server is not implemented at the moment.",
                 "It could work for non-VA Duts, but needs testing.",
                 "Verilog Xyce does not work for sure.",
             )
 
+    def info_json(self, **_kwargs) -> Dict:
+        """Returns a dict with serializeable content for the json file to create.
+
+        The topmost dict MUST have only one key: The string casted class name.
+        Inside the parameters are:
+
+            * A version key,
+            * all extra parameters of DutXyce compared to DutCircuit and
+            * the info_json of DutCircuit.
+
+        Returns
+        -------
+        dict
+            str(DutXyce): serialized content
+        """
+        va_plugins_to_compile = []
+        for path, va_file in self._va_plugins_to_compile:
+            va_plugins_to_compile.append((str(path), va_file.export_dict()))
+
+        return {
+            str(DutXyce): {
+                "__DutXyce__": str(SEMVER_DUTXYCE_CURRENT),
+                "parent": super(DutXyce, self).info_json(**_kwargs),
+                "build_xyce_plugin_command": self.build_xyce_plugin_command,
+                "_va_plugins_to_compile": va_plugins_to_compile,
+            }
+        }
+
+    @classmethod
+    def from_json(
+        cls,
+        json_content: Dict,
+        classes_technology: List[type[Technology]],
+        subclass_kwargs: Dict = None,
+    ) -> "DutXyce":
+        """Static class method. Loads a DutXyce object from a json or pickle file with full path save_dir.
+
+        Calls the from_json method of DutView with all dictionary inside the "parent" keyword. Afterwards the additional parameters are set correctly.
+
+        Parameters
+        ----------
+        json_content  :  dict
+            Readed dictionary from a saved json DutNgspice.
+        classes_technology : List[type[Technology]]
+            All possible technologies this loaded DutNgspice can have. One will be choosen according to the serialized technology loaded from the file.
+        subclass_kwargs : Dict, optional
+            Additional kwargs necessary to create the concrete subclassed DutView.
+
+        Returns
+        -------
+        DutXyce
+            Loaded object.
+        """
+        if json_content["__DutXyce__"] != SEMVER_DUTXYCE_CURRENT:
+            raise NotImplementedError("DMT.DutXyce: Unknown version of DutXyce to load!")
+
+        dut_view = super().from_json(
+            json_content["parent"], classes_technology, subclass_kwargs=subclass_kwargs
+        )
+        dut_view.build_xyce_plugin_command = json_content["build_xyce_plugin_command"]
+        dut_view._va_plugins_to_compile = []
+
+        for path, va_file in json_content["_va_plugins_to_compile"]:
+            dut_view._va_plugins_to_compile.append((Path(path), VAFileMap.import_dict(va_file)))
+
+        return dut_view
+
     def create_inp_header(self, inp_circuit):
         """Creates the input header of the given circuit description and returns it.
 
         Parameters
         ----------
         input : DMT.core.Circuit or DMT.core.MCard
             If a MCard is given, the circuit is created from it.
@@ -817,24 +894,23 @@
 
                 # repeat each line in df_dc by number of frequencies
                 len_frequencies = np.unique(df_ac[specifiers.FREQUENCY].to_numpy()).size
                 df_main = df_dc.repeat_rows(len_frequencies)
                 df_main = df_main.join(df_ac)
 
         if col_ac_switch in df_main.columns:
-
             # get all AC columns, except frequency and ac_switch
             cols_ac_old = [
                 col for col in df_ac.columns if col not in [specifiers.FREQUENCY, col_ac_switch]
             ]
 
             #  the AC columns to account for forward and backward simulation
-            if self.dut_type.is_subtype(DutType.flag_bjt):
+            if self.dut_type.is_subtype(DutType.bjt):
                 ports = ["B", "C"]
-            elif self.dut_type.is_subtype(DutType.flag_mos):
+            elif self.dut_type.is_subtype(DutType.mos):
                 ports = ["G", "D"]
             else:
                 raise NotImplementedError("DutType not known!")
             cols_ac_forward = []
             cols_ac_backward = []
             for col_old in cols_ac_old:
                 cols_ac_forward.append(
```

### Comparing `DMT_core-1.8.0rc1/DMT_core.egg-info/PKG-INFO` & `DMT_core-2.0.0/DMT_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: DMT-core
-Version: 1.8.0rc1
+Version: 2.0.0
 Summary: Device Modeling Toolkit Core
 Home-page: https://gitlab.com/dmt-development/dmt
 Author: M.Mueller, M.Krattenmacher
 Author-email: markus.mueller@semimod.de, mario.krattenmacher@semimod.de
 License: GNU GPLv3+
 Project-URL: Bug Tracker, https://gitlab.com/dmt-development/dmt
 Project-URL: Documentation, https://dmt-development.gitlab.io/dmt-core/
 Project-URL: Source Code, https://gitlab.com/dmt-development/dmt
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Description-Content-Type: text/markdown
 Provides-Extra: HDF5
-Provides-Extra: pyqtgraph
-Provides-Extra: matplotlib
-Provides-Extra: pyside2
-Provides-Extra: pyqt5
-Provides-Extra: smithplot
 Provides-Extra: develop
+Provides-Extra: full
 Provides-Extra: latex
+Provides-Extra: matplotlib
+Provides-Extra: pyqt5
+Provides-Extra: pyqtgraph
+Provides-Extra: pyside2
+Provides-Extra: pyside6
 Provides-Extra: remote
-Provides-Extra: full
+Provides-Extra: smithplot
 License-File: LICENSE
 
 # DMT-core
 
 [![pyversion](https://img.shields.io/pypi/pyversions/DMT-core)](https://pypi.org/project/DMT-core/)
 [![Build Status](https://gitlab.com/dmt-development/dmt-core/badges/main/pipeline.svg)](https://gitlab.com/dmt-development/dmt-core/-/pipelines)
 [![Coverage](https://gitlab.com/dmt-development/dmt-core/-/jobs/artifacts/main/raw/badge_coverage.svg?job=test_DMT)](https://gitlab.com/dmt-development/dmt-core/-/jobs/artifacts/main/file/htmlcov/index.html?job=test_DMT)
@@ -100,7 +102,9 @@
 6. Format the code using `black`
 7. Update the CHANGELOG with your changes and increase the version numbers in the changed files to the new version that this Pull Request would represent. The versioning scheme we use is [SemVer](http://semver.org/).
 
 
 ## License
 
 This project is licensed under GLP-v3-or-later
+
+
```

### Comparing `DMT_core-1.8.0rc1/LICENSE` & `DMT_core-2.0.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
                     GNU GENERAL PUBLIC LICENSE
                        Version 3, 29 June 2007
 
- Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
+ Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
 
                             Preamble
 
   The GNU General Public License is a free, copyleft license for
 software and other kinds of works.
@@ -643,15 +643,15 @@
 
     This program is distributed in the hope that it will be useful,
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU General Public License for more details.
 
     You should have received a copy of the GNU General Public License
-    along with this program.  If not, see <http://www.gnu.org/licenses/>.
+    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 
 Also add information on how to contact you by electronic and paper mail.
 
   If the program does terminal interaction, make it output a short
 notice like this when it starts in an interactive mode:
 
     DMT
@@ -659,22 +659,22 @@
     Copyright (C) until 2021  Markus Müller, Mario Krattenmacher and Pascal Kuthe
     <https://gitlab.com/dmt-development/dmt-core>
 
     This program comes with ABSOLUTELY NO WARRANTY; for details type `show w'.
     This is free software, and you are welcome to redistribute it
     under certain conditions; type `show c' for details.
 
-The hypothetical commands `show w' and`show c' should show the appropriate
+The hypothetical commands `show w' and `show c' should show the appropriate
 parts of the General Public License.  Of course, your program's commands
 might be different; for a GUI interface, you would use an "about box".
 
   You should also get your employer (if you work as a programmer) or school,
 if any, to sign a "copyright disclaimer" for the program, if necessary.
 For more information on this, and how to apply and follow the GNU GPL, see
-<http://www.gnu.org/licenses/>.
+<https://www.gnu.org/licenses/>.
 
   The GNU General Public License does not permit incorporating your program
 into proprietary programs.  If your program is a subroutine library, you
 may consider it more useful to permit linking proprietary applications with
 the library.  If this is what you want to do, use the GNU Lesser General
 Public License instead of this License.  But first, please read
-<http://www.gnu.org/philosophy/why-not-lgpl.html>.
+<https://www.gnu.org/licenses/why-not-lgpl.html>.
```

### Comparing `DMT_core-1.8.0rc1/PKG-INFO` & `DMT_core-2.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,36 +1,38 @@
 Metadata-Version: 2.1
 Name: DMT_core
-Version: 1.8.0rc1
+Version: 2.0.0
 Summary: Device Modeling Toolkit Core
 Home-page: https://gitlab.com/dmt-development/dmt
 Author: M.Mueller, M.Krattenmacher
 Author-email: markus.mueller@semimod.de, mario.krattenmacher@semimod.de
 License: GNU GPLv3+
 Project-URL: Bug Tracker, https://gitlab.com/dmt-development/dmt
 Project-URL: Documentation, https://dmt-development.gitlab.io/dmt-core/
 Project-URL: Source Code, https://gitlab.com/dmt-development/dmt
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Description-Content-Type: text/markdown
 Provides-Extra: HDF5
-Provides-Extra: pyqtgraph
-Provides-Extra: matplotlib
-Provides-Extra: pyside2
-Provides-Extra: pyqt5
-Provides-Extra: smithplot
 Provides-Extra: develop
+Provides-Extra: full
 Provides-Extra: latex
+Provides-Extra: matplotlib
+Provides-Extra: pyqt5
+Provides-Extra: pyqtgraph
+Provides-Extra: pyside2
+Provides-Extra: pyside6
 Provides-Extra: remote
-Provides-Extra: full
+Provides-Extra: smithplot
 License-File: LICENSE
 
 # DMT-core
 
 [![pyversion](https://img.shields.io/pypi/pyversions/DMT-core)](https://pypi.org/project/DMT-core/)
 [![Build Status](https://gitlab.com/dmt-development/dmt-core/badges/main/pipeline.svg)](https://gitlab.com/dmt-development/dmt-core/-/pipelines)
 [![Coverage](https://gitlab.com/dmt-development/dmt-core/-/jobs/artifacts/main/raw/badge_coverage.svg?job=test_DMT)](https://gitlab.com/dmt-development/dmt-core/-/jobs/artifacts/main/file/htmlcov/index.html?job=test_DMT)
@@ -100,7 +102,9 @@
 6. Format the code using `black`
 7. Update the CHANGELOG with your changes and increase the version numbers in the changed files to the new version that this Pull Request would represent. The versioning scheme we use is [SemVer](http://semver.org/).
 
 
 ## License
 
 This project is licensed under GLP-v3-or-later
+
+
```

### Comparing `DMT_core-1.8.0rc1/README.md` & `DMT_core-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `DMT_core-1.8.0rc1/setup.py` & `DMT_core-2.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,26 +5,27 @@
     long_description = fh.read()
 
 EXTRAS_REQUIRE = {
     "HDF5": ["tables"],
     "pyqtgraph": ["pyqtgraph"],
     "matplotlib": ["matplotlib"],
     "pyside2": ["PySide2"],
+    "pyside6": ["PySide6"],
     "pyqt5": ["PyQt5"],
     "smithplot": ["matplotlib", "pysmithplot-3.10"],
     "develop": ["pylint", "black"],
     "latex": ["pylatex", "pylatexenc"],
     "remote": ["paramiko", "scp"],
 }
 EXTRAS_REQUIRE["full"] = list(set(chain(*EXTRAS_REQUIRE.values())))
 EXTRAS_REQUIRE["full"].remove("PyQt5")  # not always needed
 
 setuptools.setup(
     name="DMT_core",
-    version="1.8.0-rc.1",
+    version="2.0.0",
     author="M.Mueller, M.Krattenmacher",
     author_email="markus.mueller@semimod.de, mario.krattenmacher@semimod.de",
     description="Device Modeling Toolkit Core",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/dmt-development/dmt",
     project_urls={
@@ -47,20 +48,20 @@
     include_package_data=True,
     install_requires=[
         "scipy",
         "numpy",
         "scikit-rf",
         "reprint",
         "pandas",
+        "pyarrow",
         "joblib",
         "pytest",
         "pint",
         "pyyaml",
         "more_itertools",
-        "colormath",
         "semver",
         "verilogae>=0.9b4",
         "h5py",
         "cycler",
         "colormath",
     ],
     extras_require=EXTRAS_REQUIRE,
```

