# Comparing `tmp/accelerator-2023.3.10.dev1.tar.gz` & `tmp/accelerator-2023.7.18.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "accelerator-2023.3.10.dev1.tar", last modified: Fri Mar 10 12:23:15 2023, max compression
+gzip compressed data, was "accelerator-2023.7.18.dev1.tar", last modified: Tue Jul 18 11:54:30 2023, max compression
```

## Comparing `accelerator-2023.3.10.dev1.tar` & `accelerator-2023.7.18.dev1.tar`

### file list

```diff
@@ -1,230 +1,238 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 12:23:15.424142 accelerator-2023.3.10.dev1/
--rw-r--r--   0 root         (0) root         (0)    11339 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2304 2023-03-10 12:23:15.424142 accelerator-2023.3.10.dev1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1299 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 12:23:15.400142 accelerator-2023.3.10.dev1/accelerator/
--rw-r--r--   0 root         (0) root         (0)     4967 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/OVERVIEW.txt
--rw-r--r--   0 root         (0) root         (0)     3591 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1589 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/autoflush.py
--rw-r--r--   0 root         (0) root         (0)     1471 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/blob.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 12:23:15.404142 accelerator-2023.3.10.dev1/accelerator/board/
--rw-r--r--   0 root         (0) root         (0)     3925 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/board/dataset.tpl
--rw-r--r--   0 root         (0) root         (0)     8360 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/board/head.tpl
--rw-r--r--   0 root         (0) root         (0)     4124 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/board/job.tpl
--rw-r--r--   0 root         (0) root         (0)      209 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/board/job_method_list.tpl
--rw-r--r--   0 root         (0) root         (0)      383 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/board/last_error.tpl
--rw-r--r--   0 root         (0) root         (0)     8682 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/board/main.tpl
--rw-r--r--   0 root         (0) root         (0)      731 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/board/method.tpl
--rw-r--r--   0 root         (0) root         (0)      446 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/board/methods.tpl
--rw-r--r--   0 root         (0) root         (0)      784 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/board/status.tpl
--rw-r--r--   0 root         (0) root         (0)      308 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/board/urd.tpl
--rw-r--r--   0 root         (0) root         (0)      899 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/board/urditem.tpl
--rw-r--r--   0 root         (0) root         (0)      207 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/board/urdlist.tpl
--rw-r--r--   0 root         (0) root         (0)     2129 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/board/workdir.tpl
--rw-r--r--   0 root         (0) root         (0)    14198 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/board.py
--rw-r--r--   0 root         (0) root         (0)    27671 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/build.py
--rw-r--r--   0 root         (0) root         (0)     9232 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/colourwrapper.py
--rw-r--r--   0 root         (0) root         (0)     5284 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/compat.py
--rw-r--r--   0 root         (0) root         (0)     9299 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/configfile.py
--rw-r--r--   0 root         (0) root         (0)     7965 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/control.py
--rw-r--r--   0 root         (0) root         (0)     6648 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/database.py
--rw-r--r--   0 root         (0) root         (0)    67890 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/dataset.py
--rw-r--r--   0 root         (0) root         (0)     4832 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/dependency.py
--rw-r--r--   0 root         (0) root         (0)     8907 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/deptree.py
--rw-r--r--   0 root         (0) root         (0)     4986 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/dispatch.py
--rw-r--r--   0 root         (0) root         (0)     6733 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/dsutil.py
--rw-r--r--   0 root         (0) root         (0)     3349 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/error.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 12:23:15.408142 accelerator-2023.3.10.dev1/accelerator/examples/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/__init__.py
--rw-r--r--   0 root         (0) root         (0)      425 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_dsexample_aggandmergedata.py
--rw-r--r--   0 root         (0) root         (0)      339 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_dsexample_appendcolumn.py
--rw-r--r--   0 root         (0) root         (0)      379 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_dsexample_createdataset.py
--rw-r--r--   0 root         (0) root         (0)      324 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_dsexample_iterateandmerge.py
--rw-r--r--   0 root         (0) root         (0)      479 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_dsexample_iteratechain.py
--rw-r--r--   0 root         (0) root         (0)      459 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_dsexample_multipledatasets.py
--rw-r--r--   0 root         (0) root         (0)      125 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_example_buildsubjob.py
--rw-r--r--   0 root         (0) root         (0)      266 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_example_dependextra.py
--rw-r--r--   0 root         (0) root         (0)      176 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_example_dummyjob.py
--rw-r--r--   0 root         (0) root         (0)      125 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_example_equivalenthashes.py
--rw-r--r--   0 root         (0) root         (0)      644 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_example_options.py
--rw-r--r--   0 root         (0) root         (0)      288 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_example_readjobwithfile.py
--rw-r--r--   0 root         (0) root         (0)      429 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_example_returnconcatinput.py
--rw-r--r--   0 root         (0) root         (0)      328 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_example_returnhelloworld.py
--rw-r--r--   0 root         (0) root         (0)      394 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_example_returninprepanasyn.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/a_example_writeslicedfile.py
--rw-r--r--   0 root         (0) root         (0)      553 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_dsexample-append.py
--rw-r--r--   0 root         (0) root         (0)     1128 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_dsexample-chain.py
--rw-r--r--   0 root         (0) root         (0)      534 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_dsexample-create.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_dsexample-import_csv.py
--rw-r--r--   0 root         (0) root         (0)      373 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_dsexample-iterate.py
--rw-r--r--   0 root         (0) root         (0)      592 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_dsexample-many_ds.py
--rw-r--r--   0 root         (0) root         (0)      564 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_example-build_job.py
--rw-r--r--   0 root         (0) root         (0)      460 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_example-depend_extra.py
--rw-r--r--   0 root         (0) root         (0)     1308 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_example-equiv_hashes.py
--rw-r--r--   0 root         (0) root         (0)     1238 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_example-files.py
--rw-r--r--   0 root         (0) root         (0)      560 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_example-link_jobs.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_example-options.py
--rw-r--r--   0 root         (0) root         (0)      408 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_example-return_values.py
--rw-r--r--   0 root         (0) root         (0)      418 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_example-subjobs.py
--rw-r--r--   0 root         (0) root         (0)     1784 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_tutorial01.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_tutorial02.py
--rw-r--r--   0 root         (0) root         (0)     2447 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_tutorial03.py
--rw-r--r--   0 root         (0) root         (0)     1935 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_tutorial04.py
--rw-r--r--   0 root         (0) root         (0)     2679 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_tutorial05.py
--rw-r--r--   0 root         (0) root         (0)     1999 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_urdexample-basic.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/build_urdexample-many_items.py
--rw-r--r--   0 root         (0) root         (0)       87 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/data.csv
--rw-r--r--   0 root         (0) root         (0)       84 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/data2.csv
--rw-r--r--   0 root         (0) root         (0)       91 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/data3.csv
--rw-r--r--   0 root         (0) root         (0)       74 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/mydependency.py
--rw-r--r--   0 root         (0) root         (0)       60 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/mydependencyfile.txt
--rw-r--r--   0 root         (0) root         (0)     1663 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/examples/printer.py
--rw-r--r--   0 root         (0) root         (0)    17742 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/extras.py
--rw-r--r--   0 root         (0) root         (0)     1539 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/g.py
--rw-r--r--   0 root         (0) root         (0)     7188 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/iowrapper.py
--rw-r--r--   0 root         (0) root         (0)    13441 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/job.py
--rw-r--r--   0 root         (0) root         (0)    15069 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/launch.py
--rw-r--r--   0 root         (0) root         (0)    10168 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/methods.py
--rw-r--r--   0 root         (0) root         (0)     9753 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/mp.py
--rw-r--r--   0 root         (0) root         (0)    19307 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/runner.py
--rw-r--r--   0 root         (0) root         (0)    17085 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/server.py
--rw-r--r--   0 root         (0) root         (0)     6435 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/setupfile.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 12:23:15.408142 accelerator-2023.3.10.dev1/accelerator/shell/
--rw-r--r--   0 root         (0) root         (0)    16893 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/shell/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11847 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/shell/ds.py
--rw-r--r--   0 root         (0) root         (0)    41679 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/shell/grep.py
--rw-r--r--   0 root         (0) root         (0)     9787 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/shell/init.py
--rw-r--r--   0 root         (0) root         (0)     7817 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/shell/job.py
--rw-r--r--   0 root         (0) root         (0)     6731 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/shell/lined.py
--rw-r--r--   0 root         (0) root         (0)     4060 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/shell/method.py
--rw-r--r--   0 root         (0) root         (0)     9559 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/shell/parser.py
--rw-r--r--   0 root         (0) root         (0)     3208 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/shell/script.py
--rw-r--r--   0 root         (0) root         (0)     5584 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/shell/urd.py
--rw-r--r--   0 root         (0) root         (0)     4009 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/shell/workdir.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 12:23:15.412142 accelerator-2023.3.10.dev1/accelerator/standard_methods/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19437 2023-03-10 12:23:15.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/_generated_csvimport.c
--rw-r--r--   0 root         (0) root         (0)   469969 2023-03-10 12:23:15.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/_generated_dataset_type.c
--rw-r--r--   0 root         (0) root         (0)     7854 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/a_csvexport.py
--rw-r--r--   0 root         (0) root         (0)    12774 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/a_csvimport.py
--rw-r--r--   0 root         (0) root         (0)     7675 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/a_csvimport_zip.py
--rw-r--r--   0 root         (0) root         (0)     4390 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_checksum.py
--rw-r--r--   0 root         (0) root         (0)     2287 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_checksum_chain.py
--rw-r--r--   0 root         (0) root         (0)     2537 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_concat.py
--rw-r--r--   0 root         (0) root         (0)     4519 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_fanout.py
--rw-r--r--   0 root         (0) root         (0)     1847 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_fanout_collect.py
--rw-r--r--   0 root         (0) root         (0)     2318 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_filter_columns.py
--rw-r--r--   0 root         (0) root         (0)     4988 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_hashpart.py
--rw-r--r--   0 root         (0) root         (0)     2030 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_merge.py
--rw-r--r--   0 root         (0) root         (0)     1535 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_rename_columns.py
--rw-r--r--   0 root         (0) root         (0)     8000 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_sort.py
--rw-r--r--   0 root         (0) root         (0)    24241 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_type.py
--rw-r--r--   0 root         (0) root         (0)     3755 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_unroundrobin.py
--rw-r--r--   0 root         (0) root         (0)     5305 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/c_backend_support.py
--rw-r--r--   0 root         (0) root         (0)    20329 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/csvimport.py
--rw-r--r--   0 root         (0) root         (0)    72126 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/dataset_type.py
--rw-r--r--   0 root         (0) root         (0)      253 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/standard_methods/methods.conf
--rw-r--r--   0 root         (0) root         (0)     9282 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/statmsg.py
--rw-r--r--   0 root         (0) root         (0)     2895 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/subjobs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 12:23:15.424142 accelerator-2023.3.10.dev1/accelerator/test_methods/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1520 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_analysis_died.py
--rw-r--r--   0 root         (0) root         (0)     2885 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_arg_lists.py
--rw-r--r--   0 root         (0) root         (0)     1713 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_build_kws.py
--rw-r--r--   0 root         (0) root         (0)     2050 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_compare_datasets.py
--rw-r--r--   0 root         (0) root         (0)     4782 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvexport_all_coltypes.py
--rw-r--r--   0 root         (0) root         (0)     2851 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvexport_chains.py
--rw-r--r--   0 root         (0) root         (0)     2402 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvexport_naming.py
--rw-r--r--   0 root         (0) root         (0)     4150 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvexport_quoting.py
--rw-r--r--   0 root         (0) root         (0)     2830 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvexport_separators.py
--rw-r--r--   0 root         (0) root         (0)    13349 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvimport_corner_cases.py
--rw-r--r--   0 root         (0) root         (0)     5144 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvimport_separators.py
--rw-r--r--   0 root         (0) root         (0)     6492 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvimport_zip.py
--rw-r--r--   0 root         (0) root         (0)     7733 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_callbacks.py
--rw-r--r--   0 root         (0) root         (0)     4115 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_checksum.py
--rw-r--r--   0 root         (0) root         (0)     4271 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_column_names.py
--rw-r--r--   0 root         (0) root         (0)     5464 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_concat.py
--rw-r--r--   0 root         (0) root         (0)     3808 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_empty_colname.py
--rw-r--r--   0 root         (0) root         (0)     8478 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_fanout.py
--rw-r--r--   0 root         (0) root         (0)     3049 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_filter_columns.py
--rw-r--r--   0 root         (0) root         (0)     1959 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_in_prepare.py
--rw-r--r--   0 root         (0) root         (0)     6682 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_merge.py
--rw-r--r--   0 root         (0) root         (0)     2421 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_names.py
--rw-r--r--   0 root         (0) root         (0)     2922 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_nan.py
--rw-r--r--   0 root         (0) root         (0)     2285 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_overwrite.py
--rw-r--r--   0 root         (0) root         (0)     4530 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_parsing_writer.py
--rw-r--r--   0 root         (0) root         (0)     4778 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_range.py
--rw-r--r--   0 root         (0) root         (0)     4975 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_rename_columns.py
--rw-r--r--   0 root         (0) root         (0)     2727 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_roundrobin.py
--rw-r--r--   0 root         (0) root         (0)     4452 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_slice.py
--rw-r--r--   0 root         (0) root         (0)     5832 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_type_chaining.py
--rw-r--r--   0 root         (0) root         (0)    57963 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_type_corner_cases.py
--rw-r--r--   0 root         (0) root         (0)    13565 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_type_hashing.py
--rw-r--r--   0 root         (0) root         (0)    10777 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_type_minmax.py
--rw-r--r--   0 root         (0) root         (0)     4121 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_unroundrobin.py
--rw-r--r--   0 root         (0) root         (0)     4168 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_unroundrobin_trigger.py
--rw-r--r--   0 root         (0) root         (0)     3546 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datasetwriter.py
--rw-r--r--   0 root         (0) root         (0)     3390 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datasetwriter_copy.py
--rw-r--r--   0 root         (0) root         (0)     4121 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datasetwriter_default.py
--rw-r--r--   0 root         (0) root         (0)     2211 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datasetwriter_missing_slices.py
--rw-r--r--   0 root         (0) root         (0)     3695 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datasetwriter_parent.py
--rw-r--r--   0 root         (0) root         (0)     3966 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datasetwriter_parsed.py
--rw-r--r--   0 root         (0) root         (0)     3061 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datasetwriter_verify.py
--rw-r--r--   0 root         (0) root         (0)     2334 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datetime.py
--rw-r--r--   0 root         (0) root         (0)     2355 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_finish_early.py
--rw-r--r--   0 root         (0) root         (0)     9790 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_hashlabel.py
--rw-r--r--   0 root         (0) root         (0)     7924 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_hashpart.py
--rw-r--r--   0 root         (0) root         (0)     2553 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_jobchain.py
--rw-r--r--   0 root         (0) root         (0)     3500 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_jobwithfile.py
--rw-r--r--   0 root         (0) root         (0)     4575 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_json.py
--rw-r--r--   0 root         (0) root         (0)     4040 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_number.py
--rw-r--r--   0 root         (0) root         (0)     3323 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_optionenum.py
--rw-r--r--   0 root         (0) root         (0)     1767 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_options_dict_order.py
--rw-r--r--   0 root         (0) root         (0)     1581 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_options_rebuild.py
--rw-r--r--   0 root         (0) root         (0)     4346 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output.py
--rw-r--r--   0 root         (0) root         (0)     1597 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output_a.py
--rw-r--r--   0 root         (0) root         (0)     1675 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output_as.py
--rw-r--r--   0 root         (0) root         (0)     2409 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output_on_error.py
--rw-r--r--   0 root         (0) root         (0)     1671 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output_pa.py
--rw-r--r--   0 root         (0) root         (0)     1753 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output_pas.py
--rw-r--r--   0 root         (0) root         (0)     1662 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output_ps.py
--rw-r--r--   0 root         (0) root         (0)     1588 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output_s.py
--rw-r--r--   0 root         (0) root         (0)     3563 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_rechain.py
--rw-r--r--   0 root         (0) root         (0)     5317 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_selfchain.py
--rw-r--r--   0 root         (0) root         (0)     5594 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_shell_commands.py
--rw-r--r--   0 root         (0) root         (0)     3381 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_shell_config.py
--rw-r--r--   0 root         (0) root         (0)     2081 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_shell_data.py
--rw-r--r--   0 root         (0) root         (0)     2099 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_shell_ds.py
--rw-r--r--   0 root         (0) root         (0)    46310 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_shell_grep.py
--rw-r--r--   0 root         (0) root         (0)     2448 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_shell_job.py
--rw-r--r--   0 root         (0) root         (0)     3100 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_sort_chaining.py
--rw-r--r--   0 root         (0) root         (0)     2582 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_sort_stability.py
--rw-r--r--   0 root         (0) root         (0)     2826 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_sort_trigger.py
--rw-r--r--   0 root         (0) root         (0)     4131 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_sorting.py
--rw-r--r--   0 root         (0) root         (0)     1761 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_sorting_gendata.py
--rw-r--r--   0 root         (0) root         (0)     3961 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_status_in_exceptions.py
--rw-r--r--   0 root         (0) root         (0)     1852 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_subjobs_nesting.py
--rw-r--r--   0 root         (0) root         (0)     2123 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_subjobs_type.py
--rw-r--r--   0 root         (0) root         (0)     2098 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_summary.py
--rw-r--r--   0 root         (0) root         (0)    15247 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/build_tests.py
--rw-r--r--   0 root         (0) root         (0)     1709 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/methods.conf
--rw-r--r--   0 root         (0) root         (0)     4900 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/test_data.py
--rw-r--r--   0 root         (0) root         (0)      144 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/test_methods/test_shell_commands.txt
--rw-r--r--   0 root         (0) root         (0)     5191 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/unixhttp.py
--rw-r--r--   0 root         (0) root         (0)    16964 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/urd.py
--rw-r--r--   0 root         (0) root         (0)       56 2023-03-10 12:23:15.000000 accelerator-2023.3.10.dev1/accelerator/version.txt
--rw-r--r--   0 root         (0) root         (0)     4899 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/web.py
--rw-r--r--   0 root         (0) root         (0)     4039 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/workarounds.py
--rw-r--r--   0 root         (0) root         (0)     4677 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/accelerator/workspace.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 12:23:15.400142 accelerator-2023.3.10.dev1/accelerator.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2304 2023-03-10 12:23:15.000000 accelerator-2023.3.10.dev1/accelerator.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     8985 2023-03-10 12:23:15.000000 accelerator-2023.3.10.dev1/accelerator.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-10 12:23:15.000000 accelerator-2023.3.10.dev1/accelerator.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-03-10 12:23:15.000000 accelerator-2023.3.10.dev1/accelerator.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-03-10 12:23:15.000000 accelerator-2023.3.10.dev1/accelerator.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-03-10 12:23:15.000000 accelerator-2023.3.10.dev1/accelerator.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-10 12:23:15.424142 accelerator-2023.3.10.dev1/dsutil/
--rw-r--r--   0 root         (0) root         (0)    86599 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/dsutil/dsutilmodule.c
--rw-r--r--   0 root         (0) root         (0)     5400 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/dsutil/siphash24.c
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-10 12:23:15.424142 accelerator-2023.3.10.dev1/setup.cfg
--rwxr-xr-x   0 root         (0) root         (0)     5982 2023-03-10 12:23:14.000000 accelerator-2023.3.10.dev1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:54:30.404718 accelerator-2023.7.18.dev1/
+-rw-r--r--   0 root         (0) root         (0)    11339 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2304 2023-07-18 11:54:30.400719 accelerator-2023.7.18.dev1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1299 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:54:30.384719 accelerator-2023.7.18.dev1/accelerator/
+-rw-r--r--   0 root         (0) root         (0)     4967 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/OVERVIEW.txt
+-rw-r--r--   0 root         (0) root         (0)     3591 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1589 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/autoflush.py
+-rw-r--r--   0 root         (0) root         (0)     1471 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/blob.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:54:30.384719 accelerator-2023.7.18.dev1/accelerator/board/
+-rw-r--r--   0 root         (0) root         (0)     3920 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board/dataset.tpl
+-rw-r--r--   0 root         (0) root         (0)      404 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board/head.tpl
+-rw-r--r--   0 root         (0) root         (0)     4563 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board/job.tpl
+-rw-r--r--   0 root         (0) root         (0)      231 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board/job_method_list.tpl
+-rw-r--r--   0 root         (0) root         (0)      383 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board/last_error.tpl
+-rw-r--r--   0 root         (0) root         (0)    10671 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board/main.tpl
+-rw-r--r--   0 root         (0) root         (0)      731 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board/method.tpl
+-rw-r--r--   0 root         (0) root         (0)      457 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board/methods.tpl
+-rw-r--r--   0 root         (0) root         (0)     4720 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board/script.js
+-rw-r--r--   0 root         (0) root         (0)      992 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board/status.tpl
+-rw-r--r--   0 root         (0) root         (0)     9684 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board/style.css
+-rw-r--r--   0 root         (0) root         (0)      341 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board/urd.tpl
+-rw-r--r--   0 root         (0) root         (0)     1148 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board/urditem.tpl
+-rw-r--r--   0 root         (0) root         (0)      705 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board/urdlist.tpl
+-rw-r--r--   0 root         (0) root         (0)     3522 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board/workdir.tpl
+-rw-r--r--   0 root         (0) root         (0)    17214 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/board.py
+-rw-r--r--   0 root         (0) root         (0)    27671 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/build.py
+-rw-r--r--   0 root         (0) root         (0)     9232 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/colourwrapper.py
+-rw-r--r--   0 root         (0) root         (0)     5284 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/compat.py
+-rw-r--r--   0 root         (0) root         (0)     9319 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/configfile.py
+-rw-r--r--   0 root         (0) root         (0)     8067 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/control.py
+-rw-r--r--   0 root         (0) root         (0)     7196 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/database.py
+-rw-r--r--   0 root         (0) root         (0)    67967 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     4832 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/dependency.py
+-rw-r--r--   0 root         (0) root         (0)     8907 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/deptree.py
+-rw-r--r--   0 root         (0) root         (0)     4986 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/dispatch.py
+-rw-r--r--   0 root         (0) root         (0)     6733 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/dsutil.py
+-rw-r--r--   0 root         (0) root         (0)     3349 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/error.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:54:30.388718 accelerator-2023.7.18.dev1/accelerator/examples/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      425 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_dsexample_aggandmergedata.py
+-rw-r--r--   0 root         (0) root         (0)      339 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_dsexample_appendcolumn.py
+-rw-r--r--   0 root         (0) root         (0)      379 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_dsexample_createdataset.py
+-rw-r--r--   0 root         (0) root         (0)      324 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_dsexample_iterateandmerge.py
+-rw-r--r--   0 root         (0) root         (0)      479 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_dsexample_iteratechain.py
+-rw-r--r--   0 root         (0) root         (0)      459 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_dsexample_multipledatasets.py
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_example_buildsubjob.py
+-rw-r--r--   0 root         (0) root         (0)      266 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_example_dependextra.py
+-rw-r--r--   0 root         (0) root         (0)      176 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_example_dummyjob.py
+-rw-r--r--   0 root         (0) root         (0)      125 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_example_equivalenthashes.py
+-rw-r--r--   0 root         (0) root         (0)      644 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_example_options.py
+-rw-r--r--   0 root         (0) root         (0)      288 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_example_readjobwithfile.py
+-rw-r--r--   0 root         (0) root         (0)      429 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_example_returnconcatinput.py
+-rw-r--r--   0 root         (0) root         (0)      328 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_example_returnhelloworld.py
+-rw-r--r--   0 root         (0) root         (0)      394 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_example_returninprepanasyn.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/a_example_writeslicedfile.py
+-rw-r--r--   0 root         (0) root         (0)      553 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_dsexample-append.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_dsexample-chain.py
+-rw-r--r--   0 root         (0) root         (0)      534 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_dsexample-create.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_dsexample-import_csv.py
+-rw-r--r--   0 root         (0) root         (0)      373 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_dsexample-iterate.py
+-rw-r--r--   0 root         (0) root         (0)      592 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_dsexample-many_ds.py
+-rw-r--r--   0 root         (0) root         (0)      564 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_example-build_job.py
+-rw-r--r--   0 root         (0) root         (0)      460 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_example-depend_extra.py
+-rw-r--r--   0 root         (0) root         (0)     1308 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_example-equiv_hashes.py
+-rw-r--r--   0 root         (0) root         (0)     1238 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_example-files.py
+-rw-r--r--   0 root         (0) root         (0)      560 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_example-link_jobs.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_example-options.py
+-rw-r--r--   0 root         (0) root         (0)      408 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_example-return_values.py
+-rw-r--r--   0 root         (0) root         (0)      418 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_example-subjobs.py
+-rw-r--r--   0 root         (0) root         (0)     1784 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_tutorial01.py
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_tutorial02.py
+-rw-r--r--   0 root         (0) root         (0)     2447 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_tutorial03.py
+-rw-r--r--   0 root         (0) root         (0)     1935 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_tutorial04.py
+-rw-r--r--   0 root         (0) root         (0)     2679 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_tutorial05.py
+-rw-r--r--   0 root         (0) root         (0)     1999 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_urdexample-basic.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/build_urdexample-many_items.py
+-rw-r--r--   0 root         (0) root         (0)       87 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/data.csv
+-rw-r--r--   0 root         (0) root         (0)       84 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/data2.csv
+-rw-r--r--   0 root         (0) root         (0)       91 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/data3.csv
+-rw-r--r--   0 root         (0) root         (0)       74 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/mydependency.py
+-rw-r--r--   0 root         (0) root         (0)       60 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/mydependencyfile.txt
+-rw-r--r--   0 root         (0) root         (0)     1663 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/examples/printer.py
+-rw-r--r--   0 root         (0) root         (0)    20960 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/extras.py
+-rw-r--r--   0 root         (0) root         (0)     1539 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/g.py
+-rw-r--r--   0 root         (0) root         (0)     7188 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/iowrapper.py
+-rw-r--r--   0 root         (0) root         (0)    14546 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/job.py
+-rw-r--r--   0 root         (0) root         (0)    15433 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/launch.py
+-rw-r--r--   0 root         (0) root         (0)    10168 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/methods.py
+-rw-r--r--   0 root         (0) root         (0)     9753 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/mp.py
+-rw-r--r--   0 root         (0) root         (0)    19765 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/runner.py
+-rw-r--r--   0 root         (0) root         (0)    17441 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/server.py
+-rw-r--r--   0 root         (0) root         (0)     6435 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/setupfile.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:54:30.392718 accelerator-2023.7.18.dev1/accelerator/shell/
+-rw-r--r--   0 root         (0) root         (0)    17369 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/shell/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11847 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/shell/ds.py
+-rw-r--r--   0 root         (0) root         (0)     2348 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/shell/gc.py
+-rw-r--r--   0 root         (0) root         (0)    41679 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/shell/grep.py
+-rw-r--r--   0 root         (0) root         (0)     9792 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/shell/init.py
+-rw-r--r--   0 root         (0) root         (0)     9472 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/shell/job.py
+-rw-r--r--   0 root         (0) root         (0)     6731 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/shell/lined.py
+-rw-r--r--   0 root         (0) root         (0)     4060 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/shell/method.py
+-rw-r--r--   0 root         (0) root         (0)    11624 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/shell/parser.py
+-rw-r--r--   0 root         (0) root         (0)     3208 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/shell/script.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/shell/status.py
+-rw-r--r--   0 root         (0) root         (0)     5896 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/shell/urd.py
+-rw-r--r--   0 root         (0) root         (0)     4032 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/shell/workdir.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:54:30.392718 accelerator-2023.7.18.dev1/accelerator/standard_methods/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20209 2023-07-18 11:54:30.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/_generated_csvimport.c
+-rw-r--r--   0 root         (0) root         (0)   469969 2023-07-18 11:54:30.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/_generated_dataset_type.c
+-rw-r--r--   0 root         (0) root         (0)     7854 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/a_csvexport.py
+-rw-r--r--   0 root         (0) root         (0)    13501 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/a_csvimport.py
+-rw-r--r--   0 root         (0) root         (0)     7675 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/a_csvimport_zip.py
+-rw-r--r--   0 root         (0) root         (0)     4390 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_checksum.py
+-rw-r--r--   0 root         (0) root         (0)     2287 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_checksum_chain.py
+-rw-r--r--   0 root         (0) root         (0)     2537 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_concat.py
+-rw-r--r--   0 root         (0) root         (0)     4519 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_fanout.py
+-rw-r--r--   0 root         (0) root         (0)     1847 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_fanout_collect.py
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_filter_columns.py
+-rw-r--r--   0 root         (0) root         (0)     4988 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_hashpart.py
+-rw-r--r--   0 root         (0) root         (0)     2030 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_merge.py
+-rw-r--r--   0 root         (0) root         (0)     1535 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_rename_columns.py
+-rw-r--r--   0 root         (0) root         (0)     8000 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_sort.py
+-rw-r--r--   0 root         (0) root         (0)    24241 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_type.py
+-rw-r--r--   0 root         (0) root         (0)     3755 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_unroundrobin.py
+-rw-r--r--   0 root         (0) root         (0)     5305 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/c_backend_support.py
+-rw-r--r--   0 root         (0) root         (0)    21118 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/csvimport.py
+-rw-r--r--   0 root         (0) root         (0)    72126 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/dataset_type.py
+-rw-r--r--   0 root         (0) root         (0)      253 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/standard_methods/methods.conf
+-rw-r--r--   0 root         (0) root         (0)     9282 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/statmsg.py
+-rw-r--r--   0 root         (0) root         (0)     2895 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/subjobs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:54:30.400719 accelerator-2023.7.18.dev1/accelerator/test_methods/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1520 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_analysis_died.py
+-rw-r--r--   0 root         (0) root         (0)     2885 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_arg_lists.py
+-rw-r--r--   0 root         (0) root         (0)     1713 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_build_kws.py
+-rw-r--r--   0 root         (0) root         (0)     2050 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_compare_datasets.py
+-rw-r--r--   0 root         (0) root         (0)     4782 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvexport_all_coltypes.py
+-rw-r--r--   0 root         (0) root         (0)     2851 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvexport_chains.py
+-rw-r--r--   0 root         (0) root         (0)     2402 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvexport_naming.py
+-rw-r--r--   0 root         (0) root         (0)     4150 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvexport_quoting.py
+-rw-r--r--   0 root         (0) root         (0)     2830 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvexport_separators.py
+-rw-r--r--   0 root         (0) root         (0)    13854 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvimport_corner_cases.py
+-rw-r--r--   0 root         (0) root         (0)     5144 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvimport_separators.py
+-rw-r--r--   0 root         (0) root         (0)     4436 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvimport_slicing.py
+-rw-r--r--   0 root         (0) root         (0)     6472 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvimport_zip.py
+-rw-r--r--   0 root         (0) root         (0)     7733 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_callbacks.py
+-rw-r--r--   0 root         (0) root         (0)     4115 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_checksum.py
+-rw-r--r--   0 root         (0) root         (0)     4271 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_column_names.py
+-rw-r--r--   0 root         (0) root         (0)     5464 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_concat.py
+-rw-r--r--   0 root         (0) root         (0)     3808 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_empty_colname.py
+-rw-r--r--   0 root         (0) root         (0)     8478 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_fanout.py
+-rw-r--r--   0 root         (0) root         (0)     3049 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_filter_columns.py
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_in_prepare.py
+-rw-r--r--   0 root         (0) root         (0)     6682 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_merge.py
+-rw-r--r--   0 root         (0) root         (0)     2421 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_names.py
+-rw-r--r--   0 root         (0) root         (0)     2922 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_nan.py
+-rw-r--r--   0 root         (0) root         (0)     2285 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_overwrite.py
+-rw-r--r--   0 root         (0) root         (0)     4530 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_parsing_writer.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_range.py
+-rw-r--r--   0 root         (0) root         (0)     4975 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_rename_columns.py
+-rw-r--r--   0 root         (0) root         (0)     2727 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_roundrobin.py
+-rw-r--r--   0 root         (0) root         (0)     4452 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_slice.py
+-rw-r--r--   0 root         (0) root         (0)     5832 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_type_chaining.py
+-rw-r--r--   0 root         (0) root         (0)    57963 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_type_corner_cases.py
+-rw-r--r--   0 root         (0) root         (0)    13565 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_type_hashing.py
+-rw-r--r--   0 root         (0) root         (0)    10777 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_type_minmax.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_unroundrobin.py
+-rw-r--r--   0 root         (0) root         (0)     4168 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_unroundrobin_trigger.py
+-rw-r--r--   0 root         (0) root         (0)     3546 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datasetwriter.py
+-rw-r--r--   0 root         (0) root         (0)     3390 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datasetwriter_copy.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datasetwriter_default.py
+-rw-r--r--   0 root         (0) root         (0)     2211 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datasetwriter_missing_slices.py
+-rw-r--r--   0 root         (0) root         (0)     3695 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datasetwriter_parent.py
+-rw-r--r--   0 root         (0) root         (0)     3966 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datasetwriter_parsed.py
+-rw-r--r--   0 root         (0) root         (0)     3061 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datasetwriter_verify.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datetime.py
+-rw-r--r--   0 root         (0) root         (0)     2355 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_finish_early.py
+-rw-r--r--   0 root         (0) root         (0)     9790 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_hashlabel.py
+-rw-r--r--   0 root         (0) root         (0)     7924 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_hashpart.py
+-rw-r--r--   0 root         (0) root         (0)     2499 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_job_save.py
+-rw-r--r--   0 root         (0) root         (0)     5513 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_job_save_background.py
+-rw-r--r--   0 root         (0) root         (0)     2553 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_jobchain.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_jobwithfile.py
+-rw-r--r--   0 root         (0) root         (0)     4575 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_json.py
+-rw-r--r--   0 root         (0) root         (0)     4040 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_number.py
+-rw-r--r--   0 root         (0) root         (0)     3323 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_optionenum.py
+-rw-r--r--   0 root         (0) root         (0)     1767 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_options_dict_order.py
+-rw-r--r--   0 root         (0) root         (0)     1581 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_options_rebuild.py
+-rw-r--r--   0 root         (0) root         (0)     4346 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output.py
+-rw-r--r--   0 root         (0) root         (0)     1597 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output_a.py
+-rw-r--r--   0 root         (0) root         (0)     1675 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output_as.py
+-rw-r--r--   0 root         (0) root         (0)     2409 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output_on_error.py
+-rw-r--r--   0 root         (0) root         (0)     1671 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output_pa.py
+-rw-r--r--   0 root         (0) root         (0)     1753 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output_pas.py
+-rw-r--r--   0 root         (0) root         (0)     1662 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output_ps.py
+-rw-r--r--   0 root         (0) root         (0)     1588 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output_s.py
+-rw-r--r--   0 root         (0) root         (0)     3563 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_rechain.py
+-rw-r--r--   0 root         (0) root         (0)     5317 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_selfchain.py
+-rw-r--r--   0 root         (0) root         (0)     5982 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_shell_commands.py
+-rw-r--r--   0 root         (0) root         (0)     3381 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_shell_config.py
+-rw-r--r--   0 root         (0) root         (0)     2081 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_shell_data.py
+-rw-r--r--   0 root         (0) root         (0)     2099 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_shell_ds.py
+-rw-r--r--   0 root         (0) root         (0)    46433 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_shell_grep.py
+-rw-r--r--   0 root         (0) root         (0)     2447 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_shell_job.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_sort_chaining.py
+-rw-r--r--   0 root         (0) root         (0)     2582 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_sort_stability.py
+-rw-r--r--   0 root         (0) root         (0)     2826 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_sort_trigger.py
+-rw-r--r--   0 root         (0) root         (0)     4131 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_sorting.py
+-rw-r--r--   0 root         (0) root         (0)     1761 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_sorting_gendata.py
+-rw-r--r--   0 root         (0) root         (0)     3961 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_status_in_exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_subjobs_nesting.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_subjobs_type.py
+-rw-r--r--   0 root         (0) root         (0)     2248 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_summary.py
+-rw-r--r--   0 root         (0) root         (0)     7516 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_urd.py
+-rw-r--r--   0 root         (0) root         (0)    15471 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/build_tests.py
+-rw-r--r--   0 root         (0) root         (0)     1780 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/methods.conf
+-rw-r--r--   0 root         (0) root         (0)     4900 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/test_data.py
+-rw-r--r--   0 root         (0) root         (0)      144 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/test_methods/test_shell_commands.txt
+-rw-r--r--   0 root         (0) root         (0)     5481 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/unixhttp.py
+-rw-r--r--   0 root         (0) root         (0)    17556 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/urd.py
+-rw-r--r--   0 root         (0) root         (0)       56 2023-07-18 11:54:30.000000 accelerator-2023.7.18.dev1/accelerator/version.txt
+-rw-r--r--   0 root         (0) root         (0)     4988 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/web.py
+-rw-r--r--   0 root         (0) root         (0)     4039 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/workarounds.py
+-rw-r--r--   0 root         (0) root         (0)     4677 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/accelerator/workspace.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:54:30.384719 accelerator-2023.7.18.dev1/accelerator.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2304 2023-07-18 11:54:30.000000 accelerator-2023.7.18.dev1/accelerator.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9284 2023-07-18 11:54:30.000000 accelerator-2023.7.18.dev1/accelerator.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 11:54:30.000000 accelerator-2023.7.18.dev1/accelerator.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       46 2023-07-18 11:54:30.000000 accelerator-2023.7.18.dev1/accelerator.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2023-07-18 11:54:30.000000 accelerator-2023.7.18.dev1/accelerator.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-18 11:54:30.000000 accelerator-2023.7.18.dev1/accelerator.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:54:30.400719 accelerator-2023.7.18.dev1/dsutil/
+-rw-r--r--   0 root         (0) root         (0)    86599 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/dsutil/dsutilmodule.c
+-rw-r--r--   0 root         (0) root         (0)     5400 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/dsutil/siphash24.c
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 11:54:30.404718 accelerator-2023.7.18.dev1/setup.cfg
+-rwxr-xr-x   0 root         (0) root         (0)     6011 2023-07-18 11:54:29.000000 accelerator-2023.7.18.dev1/setup.py
```

### Comparing `accelerator-2023.3.10.dev1/LICENSE` & `accelerator-2023.7.18.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/PKG-INFO` & `accelerator-2023.7.18.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelerator
-Version: 2023.3.10.dev1
+Version: 2023.7.18.dev1
 Summary: A tool for fast and reproducible processing of large amounts of data.
 Home-page: https://exax.org/
 Author: Carl Drougge
 Author-email: bearded@longhaired.org
 Project-URL: Source, https://github.com/eBay/accelerator
 Project-URL: Reference manual, https://berkeman.github.io/pdf/acc_manual.pdf
 Classifier: Development Status :: 4 - Beta
```

### Comparing `accelerator-2023.3.10.dev1/README.md` & `accelerator-2023.7.18.dev1/README.md`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/OVERVIEW.txt` & `accelerator-2023.7.18.dev1/accelerator/OVERVIEW.txt`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/__init__.py` & `accelerator-2023.7.18.dev1/accelerator/__init__.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/autoflush.py` & `accelerator-2023.7.18.dev1/accelerator/autoflush.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/blob.py` & `accelerator-2023.7.18.dev1/accelerator/blob.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/board/dataset.tpl` & `accelerator-2023.7.18.dev1/accelerator/board/dataset.tpl`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 {{ ! template('head', title=ds) }}
 
-% import json
 % def tdif(k, v):
 	% if v:
 		<tr><td>{{ k }}</td><td>{{ ! ax_link(v) }}</td></tr>
 	% end
 % end
 
 	<h1>{{ ds.job }}/{{ ds.name }}</h1>
@@ -36,15 +35,15 @@
 	</table>
 	% cols, lines = ds.shape
 	{{ cols }} columns<br>
 	{{ lines }} lines {{ ds.lines }}<br>
 	<h2>contents:</h2>
 	<script language="javascript">
 		const lines = {{ lines }};
-		const columns = {{! json.dumps(sorted(ds.columns)) }};
+		const columns = {{! js_quote(sorted(ds.columns)) }};
 		function toggle() {
 			const checks = [];
 			for (let ix = 0; ix < columns.length; ix++) {
 				checks.push(document.getElementById('wantCol' + ix))
 			}
 			const value = !checks.every(el => el.checked);
 			checks.forEach(el => el.checked = value);
@@ -67,15 +66,15 @@
 					const td = document.createElement('TD');
 					td.className = 'not-loaded';
 					tr.appendChild(td);
 				}
 				tbody.appendChild(tr);
 				return tr;
 			};
-			const url = '/dataset/{{ ds }}?lines=' + want_lines + '&column='
+			const url = '/dataset/{{ url_quote(ds) }}?lines=' + want_lines + '&column='
 			for (let col = 0; col < columns.length; col++) {
 				if (!document.getElementById('wantCol' + col).checked) continue;
 				const td = document.getElementById('col' + col);
 				if (td.dataset.lines >= want_lines) continue;
 				const spinner = document.createElement('DIV');
 				spinner.className = 'spinner';
 				td.appendChild(spinner);
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/board/job.tpl` & `accelerator-2023.7.18.dev1/accelerator/board/job.tpl`

 * *Files 7% similar despite different names*

```diff
@@ -15,24 +15,31 @@
 			% end
 			</table>
 			}
 		</div>
 	% end
 % end
 
-	<h1>{{ job }}</h1>
+	<div class="prevnext">
+		<h1>{{ job }}</h1>
+		% if job.number > 0:
+			<a accesskey="p" href="/job/{{ url_quote('%s-%d' % (job.workdir, job.number - 1,)) }}">⇦ prev</a>
+		% end
+		<a accesskey="n" href="/job/{{ url_quote('%s-%d' % (job.workdir, job.number + 1,)) }}">next ⇨</a>
+		<a accesskey="l" href="/job/{{ url_quote('%s-LATEST' % (job.workdir,)) }}">LATEST ⇉</a>
+	</div>
 	% if aborted:
 		<div class="warning">WARNING: Job didn't finish, information may be incomplete.</div>
 	% elif not current:
 		<div class="warning">Job is not current.</div>
 	% end
 	<h2>setup</h2>
 	<div class="box">
-		<a href="/method/{{ params.method }}">{{ params.package }}.{{ params.method }}</a><br>
-		<a href="/job/{{ job }}/method.tar.gz/">Source</a>
+		<a href="/method/{{ url_quote(params.method) }}">{{ params.package }}.{{ params.method }}</a><br>
+		<a href="/job/{{ url_quote(job) }}/method.tar.gz/">Source</a>
 		<div class="box" id="other-params">
 			% blacklist = {
 			%     'package', 'method', 'options', 'datasets', 'jobs', 'params',
 			%     'starttime', 'endtime', 'exectime', '_typing', 'versions',
 			% }
 			<table>
 				<tr><td>starttime</td><td>=</td><td>{{ datetime.fromtimestamp(params['starttime']) }}</td></tr>
@@ -68,39 +75,39 @@
 		% paramspart('jobs')
 	</div>
 	% if datasets:
 		<h2>datasets</h2>
 		<div class="box">
 			<ul>
 				% for ds in datasets:
-					<li><a href="/dataset/{{ ds }}">{{ ds }}</a> {{ '%d columns, %d lines' % ds.shape }}</li>
+					<li><a href="/dataset/{{ url_quote(ds) }}">{{ ds }}</a> {{ '%d columns, %d lines' % ds.shape }}</li>
 				% end
 			</ul>
 		</div>
 	% end
 	% if subjobs:
 		<h2>subjobs</h2>
 		<div class="box">
 			<ul>
 				% for j, is_current in subjobs:
-					<li><a href="/job/{{ j }}">{{ j }}</a> {{ j.method }}
+					<li><a href="/job/{{ url_quote(j) }}">{{ j }}</a> {{ j.method }}
 					% if not is_current:
 						<span class="warning">not current</span>
 					% end
 					</li>
 				% end
 			</ul>
 		</div>
 	% end
 	% if files:
 		<h2>files</h2>
 		<div class="box">
 			<ul>
 				% for fn in sorted(files):
-					<li><a target="_blank" href="/job/{{ job }}/{{ fn }}">{{ fn }}</a></li>
+					<li><a target="_blank" href="/job/{{ url_quote(job) }}/{{ url_quote(fn) }}">{{ fn }}</a></li>
 				% end
 			</ul>
 		</div>
 	% end
 	% if output:
 		<h2>output</h2>
 		<div class="box" id="output">
@@ -114,27 +121,27 @@
 					const el = document.createElement('DIV');
 					el.id = displayname;
 					el.className = 'spinner';
 					output.appendChild(el);
 					const h3 = document.createElement('H3');
 					h3.innerText = displayname;
 					const pre = document.createElement('PRE');
-					fetch('/job/{{ job }}/OUTPUT/' + name, {headers: {Accept: 'text/plain'}})
+					fetch('/job/{{! url_quote(job) }}/OUTPUT/' + name, {headers: {Accept: 'text/plain'}})
 					.then(res => {
 						if (res.status == 404) {
 							el.remove();
 						} else if (!res.ok) {
 							throw new Error(displayname + ' got ' + res.status)
 						} else {
 							return res.text();
 						}
 					})
 					.then(text => {
 						el.appendChild(h3);
-						pre.innerText = text;
+						parseANSI(pre, text);
 						el.appendChild(pre);
 						el.className = '';
 					})
 					.catch(error => {
 						console.log(error);
 						el.appendChild(h3);
 						pre.innerText = 'FETCH ERROR';
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/board/main.tpl` & `accelerator-2023.7.18.dev1/accelerator/board/main.tpl`

 * *Files 16% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 {{ ! template('head', title='') }}
 
 	<div id="bonus-info">
 		<table id="workdirs">
 			% for workdir in sorted(workdirs):
 				<tr>
-					<td><a target="_blank" href="/workdir/{{ workdir }}">{{ workdir }}</a></td>
-					<td><a target="_blank" href="/job/{{ workdir }}-LATEST">latest</a></td>
+					<td><a target="_blank" href="/workdir/{{ url_quote(workdir) }}">{{ workdir }}</a></td>
+					<td><a target="_blank" href="/job/{{ url_quote(workdir) }}-LATEST">latest</a></td>
 				</tr>
 			% end
 			<tr>
 				<td><a target="_blank" href="/workdir/">ALL</a></td>
 			</tr>
 		</table>
 		<ul>
 			<li><a target="_blank" href="/methods">methods</a></li>
 			<li><a target="_blank" href="/urd">urd</a></li>
 		</ul>
 		<input type="submit" value="show all" id="show-all" disabled>
 	</div>
-	<h1 id="header">ax board: {{ project }}</h1>
+	<h1 id="header">
+		ax board: {{ project }}
+		<span id="path">{{ path[8:] }}</span>
+	</h1>
 	<div id="status">
 		<a target="_blank" href="/status">status</a>: <span></span>
 	</div>
+	<div id="dirs"><ul></ul></div>
 	<div id="missing"></div>
 	<div id="waiting"><div class="spinner"></div></div>
 <script language="javascript">
 (function () {
 	const imageExts = new Set(['jpg', 'jpeg', 'gif', 'png', 'apng', 'svg', 'bmp', 'webp']);
 	const videoExts = new Set(['mp4', 'mov', 'mpg', 'mpeg', 'mkv', 'avi', 'webm']);
 	const waitingEl = document.getElementById('waiting');
@@ -34,15 +38,18 @@
 	show_all.onclick = function() {
 		show_all.disabled = true;
 		for (const el of document.querySelectorAll('.result.hidden')) {
 			el.classList.remove('hidden');
 		}
 	}
 	const status = function () {
-		if (document.body.className === 'error') return;
+		if (document.body.className === 'error') {
+			setTimeout(status, 1500);
+			return;
+		}
 		fetch('/status?short', {headers: {Accept: 'text/plain'}})
 		.then(res => {
 			if (res.ok) return res.text();
 			throw new Error('error response');
 		})
 		.then(res => {
 			statusEl.innerText = res;
@@ -51,15 +58,15 @@
 		.catch(error => {
 			console.log(error);
 			statusEl.innerText = '???';
 			setTimeout(status, 1500);
 		});
 	};
 	const update = function (try_num) {
-		fetch('/results', {headers: {Accept: 'application/json'}})
+		fetch('{{ url_path }}', {headers: {Accept: 'application/json'}})
 		.then(res => {
 			if (res.ok) return res.json();
 			throw new Error('error response');
 		})
 		.then(res => {
 			const missing = document.getElementById('missing');
 			if (res.missing) {
@@ -68,21 +75,43 @@
 			} else {
 				missing.className = '';
 			}
 			const existing = {};
 			for (const el of document.querySelectorAll('.result')) {
 				if (el.dataset.name) existing[el.dataset.name] = el;
 			};
+
+			const dirs_ul = document.querySelector('#dirs ul');
+			const dirs_els = {};
+			for (const el of dirs_ul.querySelectorAll('li')) {
+				dirs_els[el.dataset.name] = el;
+				el.remove();
+			}
+			const dirs = Object.entries(res.dirs).sort();
+			for (const [name, href] of dirs) {
+				let el = dirs_els[name];
+				if (!el) {
+					el = document.createElement('LI');
+					el.dataset.name = name;
+					const a = document.createElement('A');
+					a.innerText = name;
+					a.href = encodeURI(href);
+					el.appendChild(a);
+				}
+				dirs_ul.appendChild(el);
+			}
+
 			const items = Object.entries(res.files);
 			if (items.length) {
 				waitingEl.style.display = 'none';
 			} else {
 				waitingEl.style.display = 'block';
 			}
-			items.sort((a, b) => b[1].ts - a[1].ts);
+			// sort files on ts, but fall back to (link) name for files with the same time
+			items.sort((a, b) => b[1].ts - a[1].ts || a[0].localeCompare(b[0]));
 			let prev = waitingEl;
 			for (const [name, data] of items) {
 				const oldEl = existing[name];
 				if (oldEl) {
 					delete existing[name];
 					if (oldEl.dataset.ts == data.ts) {
 						update_date(oldEl);
@@ -103,22 +132,46 @@
 					a.href = href;
 					a.target = '_blank';
 					resultEl.appendChild(a);
 				}
 				resultEl.className = 'result';
 				resultEl.dataset.name = name;
 				resultEl.dataset.ts = data.ts;
-				a(name, data.jobid, data.name);
-				txt(' from ');
-				a(data.jobid, data.jobid);
-				txt(' (');
+				if (data.jobid) {
+					a(name, data.jobid, data.name);
+					txt(' from ');
+					a(data.jobid, data.jobid);
+					txt(' (');
+					const methodEl = document.createElement('SPAN')
+					methodEl.className = 'method'
+					resultEl.appendChild(methodEl);
+					txt(')');
+					fetch('/job/' + encodeURIComponent(data.jobid), {headers: {Accept: 'application/json'}})
+					.then(res => {
+						if (res.ok) return res.json();
+						throw new Error('error response');
+					})
+					.then(res => {
+						const a = document.createElement('A');
+						a.innerText = res.params.method;
+						a.href = '/method/' + encodeURIComponent(res.params.method);
+						a.target = '_blank';
+						methodEl.appendChild(a);
+					});
+				} else {
+					txt(name + ' ');
+					const el = document.createElement('SPAN');
+					el.className = 'unknown';
+					el.appendChild(document.createTextNode('from UNKNOWN'));
+					resultEl.appendChild(el);
+				}
+				txt(' ');
 				const dateEl = document.createElement('SPAN');
 				dateEl.className = 'date';
 				resultEl.appendChild(dateEl)
-				txt(')');
 				update_date(resultEl);
 				const size = document.createElement('INPUT');
 				size.type = 'submit';
 				size.value = 'big';
 				size.disabled = true;
 				resultEl.appendChild(size);
 				const hide = document.createElement('INPUT');
@@ -140,15 +193,27 @@
 		})
 		.catch(error => {
 			console.log(error);
 			if (try_num === 4) {
 				document.body.className = 'error';
 				waitingEl.style.display = 'none';
 				const header = document.getElementById('header');
+				const goodHTML = header.innerHTML;
 				header.innerText = 'ERROR - updates stopped at ' + fmtdate();
+				const btn = document.createElement('INPUT');
+				btn.type = 'button';
+				btn.value = 'restart';
+				btn.id = 'restart';
+				btn.onclick = function () {
+					document.body.className = '';
+					waitingEl.style.display = 'block';
+					header.innerHTML = goodHTML;
+					update();
+				};
+				header.appendChild(btn);
 			} else {
 				waitingEl.style.display = 'block';
 				setTimeout(() => update((try_num || 0) + 1), 1500);
 			}
 		});
 	};
 	const remove = function (el) {
@@ -175,15 +240,15 @@
 		let ext = parts.pop().toLowerCase();
 		if (ext === 'gz' && parts.length > 1) {
 			ext = parts.pop().toLowerCase();
 		}
 		return ext;
 	}
 	const load = function (name, data, size) {
-		const fileUrl = '/results/' + encodeURIComponent(name) + '?ts=' + data.ts;
+		const fileUrl = '{{ url_path }}/' + encodeURIComponent(name) + '?ts=' + data.ts;
 		const ext = name2ext(name);
 		const container = document.createElement('DIV');
 		const spinner = document.createElement('DIV');
 		spinner.className = 'spinner';
 		container.appendChild(spinner);
 		const onerror = function () {
 			spinner.remove();
@@ -247,15 +312,15 @@
 				if (res.ok) return res.text();
 				throw new Error('error response');
 			})
 			.then(res => {
 				if (ext === 'html') {
 					fileEl.innerHTML = res;
 				} else {
-					pre.innerText = res;
+					parseANSI(pre, res);
 				}
 				spinner.remove();
 			})
 			.catch(error => {
 				console.log(error);
 				onerror();
 			});
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/board/method.tpl` & `accelerator-2023.7.18.dev1/accelerator/board/method.tpl`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/board/status.tpl` & `accelerator-2023.7.18.dev1/accelerator/board/status.tpl`

 * *Files 24% similar despite different names*

```diff
@@ -6,44 +6,57 @@
 00000050: 2069 646c 653a 0a09 093c 703e 6964 6c65   idle:...<p>idle
 00000060: 3c2f 703e 0a09 2520 656c 7365 3a0a 0909  </p>..% else:...
 00000070: 3c74 6162 6c65 2069 643d 2273 7461 7475  <table id="statu
 00000080: 732d 7374 6163 6b73 223e 0a09 0909 2520  s-stacks">....% 
 00000090: 666f 7220 6a6f 622c 2070 6964 2c20 696e  for job, pid, in
 000000a0: 6465 6e74 2c20 7061 7274 2c20 6d73 672c  dent, part, msg,
 000000b0: 2074 2069 6e20 7472 6565 3a0a 0909 0909   t in tree:.....
-000000c0: 3c74 723e 3c74 643e 7b7b 206a 6f62 207d  <tr><td>{{ job }
-000000d0: 7d3c 2f74 643e 3c74 643e 7b7b 2070 6964  }</td><td>{{ pid
-000000e0: 207d 7d3c 2f74 643e 0a09 0909 0925 2069   }}</td>.....% i
-000000f0: 6620 696e 6465 6e74 203c 2030 3a0a 0909  f indent < 0:...
-00000100: 0909 093c 7464 3e3c 6469 7620 636c 6173  ...<td><div clas
-00000110: 733d 226f 7574 7075 7422 3e0a 0909 0909  s="output">.....
-00000120: 0909 5461 696c 206f 6620 6f75 7470 7574  ..Tail of output
-00000130: 2028 7b7b 2074 207d 7d20 6167 6f29 0a09   ({{ t }} ago)..
-00000140: 0909 0909 093c 6120 6872 6566 3d22 2f6a  .....<a href="/j
-00000150: 6f62 2f7b 7b20 6a6f 6220 7d7d 2f4f 5554  ob/{{ job }}/OUT
-00000160: 5055 542f 7b7b 2070 6172 7420 7d7d 223e  PUT/{{ part }}">
-00000170: 7669 6577 2066 756c 6c3c 2f61 3e0a 0909  view full</a>...
-00000180: 0909 0909 3c70 7265 3e7b 7b20 275c 6e27  ....<pre>{{ '\n'
-00000190: 2e6a 6f69 6e28 6d73 6729 207d 7d3c 2f70  .join(msg) }}</p
-000001a0: 7265 3e0a 0909 0909 093c 2f64 6976 3e3c  re>......</div><
-000001b0: 2f74 643e 0a09 0909 0925 2065 6c73 653a  /td>.....% else:
-000001c0: 0a09 0909 0909 3c74 6420 7374 796c 653d  ......<td style=
-000001d0: 2270 6164 6469 6e67 2d6c 6566 743a 207b  "padding-left: {
-000001e0: 7b20 696e 6465 6e74 202a 2032 207d 7d2e  { indent * 2 }}.
-000001f0: 3565 6d22 3e0a 0909 0909 0909 7b7b 206d  5em">.......{{ m
-00000200: 7367 207d 7d0a 0909 0909 0909 287b 7b20  sg }}.......({{ 
-00000210: 7420 7d7d 290a 0909 0909 093c 2f74 643e  t }})......</td>
-00000220: 0a09 0909 0925 2065 6e64 0a09 0909 093c  .....% end.....<
-00000230: 2f74 723e 0a09 0909 2520 656e 640a 0909  /tr>....% end...
-00000240: 3c2f 7461 626c 653e 0a09 2520 656e 640a  </table>..% end.
-00000250: 0925 2069 6620 6765 7428 276c 6173 745f  .% if get('last_
-00000260: 6572 726f 725f 7469 6d65 2729 3a0a 0909  error_time'):...
-00000270: 3c70 3e3c 6120 6872 6566 3d22 6c61 7374  <p><a href="last
-00000280: 5f65 7272 6f72 3f74 3d7b 7b20 6c61 7374  _error?t={{ last
-00000290: 5f65 7272 6f72 5f74 696d 6520 7d7d 223e  _error_time }}">
-000002a0: 4c61 7374 2065 7272 6f72 2061 740a 0909  Last error at...
-000002b0: 097b 7b20 6461 7465 7469 6d65 2e66 726f  .{{ datetime.fro
-000002c0: 6d74 696d 6573 7461 6d70 286c 6173 745f  mtimestamp(last_
-000002d0: 6572 726f 725f 7469 6d65 292e 7265 706c  error_time).repl
-000002e0: 6163 6528 6d69 6372 6f73 6563 6f6e 643d  ace(microsecond=
-000002f0: 3029 207d 7d0a 0909 3c2f 613e 3c2f 703e  0) }}...</a></p>
-00000300: 0a09 2520 656e 640a 3c2f 626f 6479 3e0a  ..% end.</body>.
+000000c0: 3c74 723e 3c74 643e 3c61 2068 7265 663d  <tr><td><a href=
+000000d0: 222f 6a6f 622f 7b7b 2075 726c 5f71 756f  "/job/{{ url_quo
+000000e0: 7465 286a 6f62 2920 7d7d 223e 7b7b 206a  te(job) }}">{{ j
+000000f0: 6f62 207d 7d3c 2f61 3e3c 2f74 643e 3c74  ob }}</a></td><t
+00000100: 643e 7b7b 2070 6964 207d 7d3c 2f74 643e  d>{{ pid }}</td>
+00000110: 0a09 0909 0925 2069 6620 696e 6465 6e74  .....% if indent
+00000120: 203c 2030 3a0a 0909 0909 093c 7464 3e3c   < 0:......<td><
+00000130: 6469 7620 636c 6173 733d 226f 7574 7075  div class="outpu
+00000140: 7422 3e0a 0909 0909 0909 5461 696c 206f  t">.......Tail o
+00000150: 6620 6f75 7470 7574 2028 7b7b 2074 207d  f output ({{ t }
+00000160: 7d20 6167 6f29 0a09 0909 0909 093c 6120  } ago).......<a 
+00000170: 6872 6566 3d22 2f6a 6f62 2f7b 7b20 7572  href="/job/{{ ur
+00000180: 6c5f 7175 6f74 6528 6a6f 6229 207d 7d2f  l_quote(job) }}/
+00000190: 4f55 5450 5554 2f7b 7b20 7061 7274 207d  OUTPUT/{{ part }
+000001a0: 7d22 3e76 6965 7720 6675 6c6c 3c2f 613e  }">view full</a>
+000001b0: 0a09 0909 0909 093c 7072 653e 7b7b 2027  .......<pre>{{ '
+000001c0: 5c6e 272e 6a6f 696e 286d 7367 2920 7d7d  \n'.join(msg) }}
+000001d0: 3c2f 7072 653e 0a09 0909 0909 3c2f 6469  </pre>......</di
+000001e0: 763e 3c2f 7464 3e0a 0909 0909 2520 656c  v></td>.....% el
+000001f0: 7365 3a0a 0909 0909 093c 7464 2073 7479  se:......<td sty
+00000200: 6c65 3d22 7061 6464 696e 672d 6c65 6674  le="padding-left
+00000210: 3a20 7b7b 2069 6e64 656e 7420 2a20 3220  : {{ indent * 2 
+00000220: 7d7d 2e35 656d 223e 0a09 0909 0909 097b  }}.5em">.......{
+00000230: 7b20 6d73 6720 7d7d 0a09 0909 0909 0928  { msg }}.......(
+00000240: 7b7b 2074 207d 7d29 0a09 0909 0909 3c2f  {{ t }})......</
+00000250: 7464 3e0a 0909 0909 2520 656e 640a 0909  td>.....% end...
+00000260: 0909 3c2f 7472 3e0a 0909 0925 2065 6e64  ..</tr>....% end
+00000270: 0a09 093c 2f74 6162 6c65 3e0a 0925 2065  ...</table>..% e
+00000280: 6e64 0a09 2520 6966 2067 6574 2827 6c61  nd..% if get('la
+00000290: 7374 5f65 7272 6f72 5f74 696d 6527 293a  st_error_time'):
+000002a0: 0a09 093c 703e 3c61 2068 7265 663d 226c  ...<p><a href="l
+000002b0: 6173 745f 6572 726f 723f 743d 7b7b 206c  ast_error?t={{ l
+000002c0: 6173 745f 6572 726f 725f 7469 6d65 207d  ast_error_time }
+000002d0: 7d22 3e4c 6173 7420 6572 726f 7220 6174  }">Last error at
+000002e0: 0a09 0909 7b7b 2064 6174 6574 696d 652e  ....{{ datetime.
+000002f0: 6672 6f6d 7469 6d65 7374 616d 7028 6c61  fromtimestamp(la
+00000300: 7374 5f65 7272 6f72 5f74 696d 6529 2e72  st_error_time).r
+00000310: 6570 6c61 6365 286d 6963 726f 7365 636f  eplace(microseco
+00000320: 6e64 3d30 2920 7d7d 0a09 093c 2f61 3e3c  nd=0) }}...</a><
+00000330: 2f70 3e0a 0925 2065 6e64 0a3c 7363 7269  /p>..% end.<scri
+00000340: 7074 206c 616e 6775 6167 653d 226a 6176  pt language="jav
+00000350: 6173 6372 6970 7422 3e0a 2866 756e 6374  ascript">.(funct
+00000360: 696f 6e28 2920 7b0a 0966 6f72 2028 636f  ion() {..for (co
+00000370: 6e73 7420 656c 206f 6620 646f 6375 6d65  nst el of docume
+00000380: 6e74 2e71 7565 7279 5365 6c65 6374 6f72  nt.querySelector
+00000390: 416c 6c28 272e 6f75 7470 7574 2070 7265  All('.output pre
+000003a0: 2729 2920 7b0a 0909 7061 7273 6541 4e53  ')) {...parseANS
+000003b0: 4928 656c 2c20 656c 2e69 6e6e 6572 5465  I(el, el.innerTe
+000003c0: 7874 293b 0a09 7d0a 7d29 2829 3b0a 3c2f  xt);..}.})();.</
+000003d0: 7363 7269 7074 3e0a 3c2f 626f 6479 3e0a  script>.</body>.
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/board.py` & `accelerator-2023.7.18.dev1/accelerator/board.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ############################################################################
 #                                                                          #
-# Copyright (c) 2020-2022 Carl Drougge                                     #
+# Copyright (c) 2020-2023 Carl Drougge                                     #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
 #                                                                          #
@@ -12,40 +12,37 @@
 # distributed under the License is distributed on an "AS IS" BASIS,        #
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. #
 # See the License for the specific language governing permissions and      #
 # limitations under the License.                                           #
 #                                                                          #
 ############################################################################
 
+from __future__ import print_function
+
 import bottle
 import json
 import sys
 import os
 import tarfile
 import itertools
 import collections
 import functools
+from stat import S_ISDIR, S_ISLNK
 
 from accelerator.job import Job, JobWithFile
 from accelerator.dataset import Dataset
 from accelerator.unixhttp import call, WaitressServer
 from accelerator.build import fmttime
 from accelerator.configfile import resolve_listen
 from accelerator.error import NoSuchWhateverError
-from accelerator.shell.parser import ArgumentParser
+from accelerator.shell.parser import ArgumentParser, name2job, name2ds
 from accelerator.shell.workdir import job_data, workdir_jids
 from accelerator.compat import setproctitle, url_quote, urlencode
 from accelerator import __version__ as ax_version
 
-def get_job(jobid):
-	if jobid.endswith('-LATEST'):
-		base = jobid.rsplit('-', 1)[0]
-		jobid = os.readlink(Job(base + '-0').path[:-2] + '-LATEST')
-	return Job(jobid)
-
 # why wasn't Accept specified in a sane manner (like sending it in preference order)?
 def get_best_accept(*want):
 	d = {want[0]: -1} # fallback to first specified
 	# {'a/*': 'a/exact'}, reversed() so earlier win
 	want_short = {w.split('/', 1)[0] + '/*': w for w in reversed(want)}
 	want = set(want)
 	want.update(want_short)
@@ -117,29 +114,62 @@
 	elif isinstance(v, list):
 		return '[%s]' % (', '.join(ax_link(vv) for vv in v),)
 	elif v:
 		ev = bottle.html_escape(v)
 		if isinstance(v, Dataset):
 			job = bottle.html_escape(v.job)
 			name = bottle.html_escape(v.name)
-			return '<a href="/job/%s">%s</a>/<a href="/dataset/%s">%s</a>' % (job, job, ev, name,)
+			return '<a href="/job/%s">%s</a>/<a href="/dataset/%s">%s</a>' % (url_quote(v.job), job, url_quote(v), name,)
 		elif isinstance(v, Job):
-			return '<a href="/job/%s">%s</a>' % (ev, ev,)
+			return '<a href="/job/%s">%s</a>' % (url_quote(v), ev,)
 		else:
 			return ev
 	else:
 		return ''
 
+name2hashed = {}
+hashed = {}
+
+# Make contents-based names so that the files can be cached forever
+def populate_hashed():
+	from hashlib import sha1
+	from base64 import b64encode
+	dirname = os.path.join(os.path.dirname(__file__), 'board')
+	for filename, ctype in [
+		('style.css', 'text/css; charset=UTF-8'),
+		('script.js', 'text/javascript; charset=UTF-8'),
+	]:
+		try:
+			with open(os.path.join(dirname, filename), 'rb') as fh:
+				data = fh.read()
+			h = b64encode(sha1(data).digest(), b'_-').rstrip(b'=').decode('ascii')
+			h_name = h + '/' + filename
+			name2hashed[filename] = '/h/' + h_name
+			hashed[h_name] = (data, ctype,)
+		except OSError as e:
+			name2hashed[filename] = '/h/ERROR'
+			print(e, file=sys.stderr)
+
+
+def js_quote(obj):
+	# If the string contains '</script>' that will end the script, even if
+	# it's in the middle of a string. Escape < to avoid problems like that.
+	return json.dumps(obj).replace('<', '\\074')
+
+
 def template(tpl_name, **kw):
 	return bottle.template(
 		tpl_name,
 		ax_repr=ax_repr,
 		ax_link=ax_link,
 		ax_version=ax_version,
+		js_quote=js_quote,
+		name2hashed=name2hashed,
 		template=template,
+		url_quote=url_quote,
 		**kw
 	)
 
 
 def view(name, subkey=None):
 	def view_decorator(func):
 		@functools.wraps(func)
@@ -212,14 +242,22 @@
 		sys.argv[2:] = [cfg.board_listen]
 	run(cfg, from_shell=True)
 
 def run(cfg, from_shell=False):
 	project = os.path.split(cfg.project_directory)[1]
 	setproctitle('ax board-server for %s on %s' % (project, cfg.board_listen,))
 
+	# The default path filter (i.e. <something:path>) does not match newlines,
+	# but we want it to do so (e.g. in case someone names a dataset with one).
+	def pathfilter(config):
+		return r'(?:.|\n)+?', None, None
+	bottle.default_app[0].router.add_filter('path', pathfilter)
+
+	populate_hashed()
+
 	def call_s(*path, **kw):
 		if kw:
 			data = urlencode(kw).encode('utf-8')
 		else:
 			data = None
 		return call(os.path.join(cfg.url, *map(url_quote, path)), data=data)
 
@@ -227,52 +265,108 @@
 		url = os.path.join(cfg.urd, *map(url_quote, path))
 		if kw:
 			url = url + '?' + urlencode(kw)
 		return call(url, server_name='urd')
 
 	@bottle.get('/')
 	@view('main')
-	def main_page():
+	def main_page(path='/results'):
 		return dict(
 			project=project,
 			workdirs=cfg.workdirs,
+			path=path,
+			url_path=url_quote(path),
 		)
 
-	@bottle.get('/results')
-	def results():
-		files = {}
-		res = {'files': files}
-		filenames = ()
+	# Look for actual workdirs, so things like /workdirs/foo/foo-37/foo-1/bar
+	# resolves to ('foo-37', 'foo-1/bar') and not ('foo-1', 'bar').
+	path2wd = {v: k for k, v in cfg.workdirs.items()}
+	def job_and_file(path, default_name):
+		wd = ''
+		path = iter(path.split('/'))
+		for name in path:
+			if not name:
+				continue
+			wd = wd + '/' + name
+			if wd in path2wd:
+				break
+		else:
+			return None, default_name
 		try:
-			filenames = os.listdir(cfg.result_directory)
-		except KeyError:
-			res['missing'] = 'result directory not configured'
-		except OSError:
-			res['missing'] = 'result directory %r missing' % (cfg.result_directory,)
+			jobid = Job(next(path))
+		except (StopIteration, NoSuchWhateverError):
+			return None, default_name
+		return jobid, '/'.join(path) or default_name
+
+	def results_contents(path):
+		files = {}
+		dirs = {}
+		res = {'files': files, 'dirs': dirs}
+		default_jobid = None
+		default_prefix = ''
+		prefix = cfg.result_directory
+		for part in path.strip('/').split('/'):
+			prefix = os.path.join(prefix, part)
+			if not default_jobid:
+				try:
+					default_jobid, default_prefix = job_and_file(os.readlink(prefix), '')
+					if default_jobid and default_prefix:
+						default_prefix += '/'
+				except OSError:
+					pass
+			elif default_prefix:
+				default_prefix += part + '/'
+		filenames = os.listdir(prefix)
 		for fn in filenames:
-			if fn.endswith('_'):
+			if fn.startswith('.') or fn.endswith('_'):
 				continue
-			ffn = os.path.join(cfg.result_directory, fn)
+			ffn = os.path.join(prefix, fn)
 			try:
-				jobid, name = os.readlink(ffn).split('/')[-2:]
+				lstat = os.lstat(ffn)
+				if S_ISLNK(lstat.st_mode):
+					link_dest = os.readlink(ffn)
+					stat = os.stat(link_dest)
+					jobid, name = job_and_file(link_dest, fn)
+				else:
+					stat = lstat
+					jobid = default_jobid
+					name = default_prefix + fn
+			except OSError:
+				continue
+			if S_ISDIR(stat.st_mode):
+				dirs[fn] = os.path.join('/results', path, fn, '')
+			else:
 				files[fn] = dict(
 					jobid=jobid,
 					name=name,
-					ts=os.lstat(ffn).st_mtime,
-					size=os.stat(ffn).st_size,
+					ts=lstat.st_mtime,
+					size=stat.st_size,
 				)
-			except OSError:
-				continue
-		bottle.response.content_type = 'application/json; charset=UTF-8'
-		bottle.response.set_header('Cache-Control', 'no-cache')
-		return json.dumps(res)
-
-	@bottle.get('/results/<name>')
-	def file(name):
-		return bottle.static_file(name, root=cfg.result_directory)
+		if path:
+			a, b = os.path.split(path)
+			dirs['..'] = os.path.join('/results', a, '') if a else '/'
+		return res
+
+	@bottle.get('/results')
+	@bottle.get('/results/')
+	@bottle.get('/results/<path:path>')
+	def results(path=''):
+		path = path.strip('/')
+		if os.path.isdir(os.path.join(cfg.result_directory, path)):
+			accept = get_best_accept('text/html', 'application/json', 'text/json')
+			if accept == 'text/html':
+				return main_page(path=os.path.join('/results', path).rstrip('/'))
+			else:
+				bottle.response.content_type = accept + '; charset=UTF-8'
+				bottle.response.set_header('Cache-Control', 'no-cache')
+				return json.dumps(results_contents(path))
+		elif path:
+			return bottle.static_file(path, root=cfg.result_directory)
+		else:
+			return {'missing': 'result directory %r missing' % (cfg.result_directory,)}
 
 	@bottle.get('/status')
 	@view('status')
 	def status():
 		status = call_s('status/full')
 		if 'short' in bottle.request.query:
 			if status.idle:
@@ -288,41 +382,41 @@
 	@view('last_error')
 	def last_error():
 		return call_s('last_error')
 
 	@bottle.get('/job/<jobid>/method.tar.gz/')
 	@bottle.get('/job/<jobid>/method.tar.gz/<name:path>')
 	def job_method(jobid, name=None):
-		job = get_job(jobid)
+		job = name2job(cfg, jobid)
 		with tarfile.open(job.filename('method.tar.gz'), 'r:gz') as tar:
 			if name:
 				info = tar.getmember(name)
 			else:
 				members = [info for info in tar.getmembers() if info.isfile()]
 				if len(members) == 1 and not name:
 					info = members[0]
 				else:
 					return template('job_method_list', members=members, job=job)
 			bottle.response.content_type = 'text/plain; charset=UTF-8'
 			return tar.extractfile(info).read()
 
 	@bottle.get('/job/<jobid>/<name:path>')
 	def job_file(jobid, name):
-		job = get_job(jobid)
+		job = name2job(cfg, jobid)
 		res = bottle.static_file(name, root=job.path)
 		if not res.content_type and res.status_code < 400:
 			# bottle default is text/html, which is probably wrong.
 			res.content_type = 'text/plain'
 		return res
 
 	@bottle.get('/job/<jobid>')
 	@bottle.get('/job/<jobid>/')
 	@view('job')
 	def job(jobid):
-		job = get_job(jobid)
+		job = name2job(cfg, jobid)
 		try:
 			post = job.post
 		except IOError:
 			post = None
 		if post:
 			aborted = False
 			files = [fn for fn in job.files() if fn[0] != '/']
@@ -346,15 +440,15 @@
 			subjobs=subjobs,
 			files=files,
 		)
 
 	@bottle.get('/dataset/<dsid:path>')
 	@view('dataset', ds_json)
 	def dataset(dsid):
-		ds = Dataset(dsid.rstrip('/'))
+		ds = name2ds(cfg, dsid.rstrip('/'))
 		q = bottle.request.query
 		if q.column:
 			lines = int(q.lines or 10)
 			it = ds.iterate(None, q.column)
 			it = itertools.islice(it, lines)
 			t = ds.columns[q.column].type
 			if t in ('datetime', 'date', 'time',):
@@ -365,25 +459,16 @@
 			bottle.response.content_type = 'application/json; charset=UTF-8'
 			return json.dumps(res)
 		else:
 			return dict(ds=ds)
 
 	def load_workdir(jobs, name):
 		known = call_s('workdir', name)
-		jobs[name + '-LATEST'] = None # Sorts first
-		try:
-			latest = os.readlink(os.path.join(cfg.workdirs[name], name + '-LATEST'))
-		except OSError:
-			latest = None
 		for jid in workdir_jids(cfg, name):
 			jobs[jid] = job_data(known, jid)
-		if latest in jobs:
-			jobs[name + '-LATEST'] = jobs[latest]
-		else:
-			del jobs[name + '-LATEST']
 		return jobs
 
 	@bottle.get('/workdir/<name>')
 	@view('workdir', 'jobs')
 	def workdir(name):
 		return dict(name=name, jobs=load_workdir(collections.OrderedDict(), name))
 
@@ -436,14 +521,23 @@
 	@bottle.get('/urd/<user>/<build>/<ts>')
 	@view('urditem', 'entry')
 	def urditem(user, build, ts):
 		key = user + '/' + build + '/' + ts
 		d = call_u(key)
 		return dict(key=key, entry=d)
 
+	@bottle.get('/h/<name:path>')
+	def hashed_file(name):
+		if name not in hashed:
+			return bottle.HTTPError(404, 'Not Found')
+		data, ctype = hashed[name]
+		bottle.response.content_type = ctype
+		bottle.response.set_header('Cache-Control', 'max-age=604800, immutable')
+		return data
+
 	@bottle.error(500)
 	def error(e):
 		tpl = bottle.ERROR_PAGE_TEMPLATE
 		if isinstance(e.exception, NoSuchWhateverError):
 			e.body = str(e.exception)
 		else:
 			# awful hack: replace DEBUG with something that will be true,
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/build.py` & `accelerator-2023.7.18.dev1/accelerator/build.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/colourwrapper.py` & `accelerator-2023.7.18.dev1/accelerator/colourwrapper.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/compat.py` & `accelerator-2023.7.18.dev1/accelerator/compat.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/configfile.py` & `accelerator-2023.7.18.dev1/accelerator/configfile.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 		url = None
 	return listen, url
 
 def fixup_listen(project_directory, listen):
 	listen, url = listen
 	if not isinstance(listen, tuple):
 		socket = os.path.join(project_directory, listen)
-		url = 'unixhttp://' + quote_plus(os.path.realpath(socket))
+		url = 'unixhttp://' + quote_plus(os.path.realpath(socket)).replace('+', '%20')
 	return listen, url
 
 
 def load_config(filename):
 	from accelerator.error import UserError
 
 	multivalued = {'workdirs', 'method packages', 'interpreters'}
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/control.py` & `accelerator-2023.7.18.dev1/accelerator/control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ############################################################################
 #                                                                          #
 # Copyright (c) 2017 eBay Inc.                                             #
-# Modifications copyright (c) 2018-2022 Carl Drougge                       #
+# Modifications copyright (c) 2018-2023 Carl Drougge                       #
 # Modifications copyright (c) 2020-2021 Anders Berkeman                    #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
@@ -31,14 +31,15 @@
 from accelerator import dependency
 from accelerator import dispatch
 
 from accelerator import workspace
 from accelerator import database
 from accelerator import methods
 from accelerator.colourwrapper import colour
+from accelerator.compat import FileNotFoundError
 from accelerator.setupfile import update_setup
 from accelerator.job import WORKDIRS, Job
 from accelerator.extras import json_save, DotDict
 from accelerator.error import BuildError
 
 
 
@@ -182,15 +183,18 @@
 		setup = update_setup(jobid, starttime=t0)
 		prof = setup.get('exectime', DotDict())
 		new_prof, files, subjobs = dispatch.launch(W.path, setup, self.config, self.Methods, active_workdirs, slices, concurrency, self.server_url, subjob_cookie, parent_pid)
 		prefix = join(W.path, jobid) + '/'
 		if not self.keep_temp_files:
 			for filename, temp in list(files.items()):
 				if temp:
-					unlink(join(prefix, filename))
+					try:
+						unlink(join(prefix, filename))
+					except FileNotFoundError:
+						pass
 					del files[filename]
 		prof.update(new_prof)
 		prof.total = 0
 		prof.total = sum(v for v in prof.values() if isinstance(v, (float, int)))
 		if concurrency:
 			prof.concurrency = concurrency
 		data = dict(
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/database.py` & `accelerator-2023.7.18.dev1/accelerator/database.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ############################################################################
 #                                                                          #
 # Copyright (c) 2017 eBay Inc.                                             #
-# Modifications copyright (c) 2019-2022 Carl Drougge                       #
+# Modifications copyright (c) 2019-2023 Carl Drougge                       #
 # Modifications copyright (c) 2020 Anders Berkeman                         #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
@@ -18,15 +18,14 @@
 #                                                                          #
 ############################################################################
 
 from __future__ import print_function
 from __future__ import division
 
 from collections import defaultdict
-from operator import attrgetter
 from collections import namedtuple
 from traceback import print_exc
 import sys
 
 from accelerator.compat import iteritems, itervalues
 
 from accelerator.extras import _job_params, job_post, OptionEnum, OptionDefault
@@ -93,15 +92,17 @@
 
 	def _update_begin(self):
 		self._fsjid = set()
 
 	def add_single_jobid(self, jobid):
 		setup = _paramsdict[jobid][0]
 		job = _mkjob(setup)
-		self.db_by_method[job.method].insert(0, job)
+		self.db[job.id] = job
+		self.db_by_method[job.method].append(job.id)
+		self.all_by_method[job.method].append(job.id)
 		self.db_by_workdir[job.id.rsplit('-', 1)[0]][job.id] = _mklistinfo(setup)
 		return job
 
 	def _update_workspace(self, WorkSpace, pool, verbose=False):
 		"""Insert all items in WorkSpace in database (call update_finish too)"""
 		if verbose:
 			print("DATABASE:  update for \"%s\"" % WorkSpace.name)
@@ -125,20 +126,24 @@
 		for j in set(_paramsdict) - self._fsjid:
 			del _paramsdict[j]
 		discarded_due_to_hash_list = []
 		self.db_by_workdir = defaultdict(dict) # includes all known jobs, not just current ones.
 
 		# Keep only jobs with valid hashes.
 		job_candidates = {}
+		# Keep separate lists per method of just jobids for all (finished) jobs,
+		# to support the relative job-specs ("method~" and such).
+		self.all_by_method = defaultdict(list)
 		for setup, subjobs in itervalues(_paramsdict):
 			if setup.hash in dict_of_hashes.get(setup.method, ()):
 				job_candidates[setup.jobid] = (setup, subjobs)
 			else:
 				discarded_due_to_hash_list.append(setup.jobid)
 			self.db_by_workdir[setup.jobid.rsplit('-', 1)[0]][setup.jobid] = _mklistinfo(setup)
+			self.all_by_method[setup.method].append(setup.jobid)
 
 		# Keep only jobs where all subjobs are kept.
 		discarded_due_to_subjobs = []
 		done = False
 		while not done:
 			done = True
 			for setup, subjobs in list(itervalues(job_candidates)):
@@ -150,35 +155,42 @@
 						break
 
 		for d in self.db_by_workdir.values():
 			for jid, li in d.items():
 				if jid not in job_candidates:
 					li['current'] = False
 
+		# {jobid: Job} (the local Job tuple type, not the user-visible one)
+		self.db = {}
 		# Keep lists of jobs per method, only with valid hashes and subjobs.
 		self.db_by_method = defaultdict(list)
 		for setup, _ in itervalues(job_candidates):
 			job = _mkjob(setup)
-			self.db_by_method[job.method].append(job)
+			self.db[job.id] = job
+			self.db_by_method[job.method].append(job.id)
 		# Newest first
 		for l in itervalues(self.db_by_method):
-			l.sort(key=attrgetter('time'), reverse=True)
+			l.sort(key=lambda jid: self.db[jid].time)
+		for l in itervalues(self.all_by_method):
+			l.sort(key=lambda jid: _paramsdict[jid][0].starttime)
 		if verbose:
 			if discarded_due_to_hash_list:
 				print("DATABASE:  discarding due to unknown hash: %s" % ', '.join(discarded_due_to_hash_list))
 			print("DATABASE:  Full database contains %d items" % (sum(len(v) for v in itervalues(self.db_by_method)),))
 
 	def match_complex(self, reqlist):
 		for method, uid, opttuple in reqlist:
 			# These are already sorted newest to oldest.
-			for job in self.db_by_method[method]:
+			for job in reversed(self.db_by_method[method]):
+				job = self.db[job]
 				if opttuple.issubset(job.optset):
 					yield uid, job
 					break
 
 	def match_exact(self, reqlist):
 		for method, uid, opttuple in reqlist:
 			# These are already sorted newest to oldest.
-			for job in self.db_by_method[method]:
+			for job in reversed(self.db_by_method[method]):
+				job = self.db[job]
 				if opttuple == job.optset:
 					yield uid, job
 					break
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/dataset.py` & `accelerator-2023.7.18.dev1/accelerator/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 ############################################################################
 #                                                                          #
 # Copyright (c) 2017 eBay Inc.                                             #
-# Modifications copyright (c) 2018-2022 Carl Drougge                       #
+# Modifications copyright (c) 2018-2023 Carl Drougge                       #
 # Modifications copyright (c) 2019-2020 Anders Berkeman                    #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
@@ -473,16 +473,14 @@
 	def column_filename(self, colname, sliceno=None):
 		dc = self.columns[colname]
 		jid, name = dc.location.split('/', 1)
 		jid = Job(jid)
 		if dc.offsets:
 			return jid.filename(name)
 		else:
-			if sliceno is None:
-				sliceno = '%s'
 			return jid.filename(name % (sliceno,))
 
 	def _chain(self, length, reverse, stop):
 		chain = DatasetChain()
 		current = self
 		while length != len(chain) and not stop(current):
 			chain.append(current)
@@ -809,15 +807,15 @@
 			def update_status(ix, d, sliceno, rehash):
 				pass
 		else:
 			msg_head = 'Iterating %s to %s' % (fmt_dsname(*to_iter[0]), fmt_dsname(*to_iter[-1]),)
 			def update_status(ix, d, sliceno, rehash):
 				update('%s, %d/%d (%s)' % (msg_head, ix, len(to_iter), fmt_dsname(d, sliceno, rehash)))
 		with status(msg_head) as update:
-			update_status._line_report = update._line_report
+			update_status._line_report = getattr(update, '_line_report', None)
 			yield update_status
 
 	@staticmethod
 	def _iterate_datasets(to_iter, columns, pre_callback, post_callback, filter_func, translation_func, translators, want_tuple, range, status_reporting, copy_mode):
 		skip_ds = None
 		def argfixup(func, is_post):
 			if func:
@@ -1037,52 +1035,53 @@
 				self._data['cache'] = tuple((unicode(d), d._data) for d in chain[:-1])
 			self._data['cache_distance'] = cache_distance
 
 	def _maybe_merge(self, n):
 		from accelerator.g import slices
 		if slices < 2:
 			return
-		fn = self.column_filename(n)
+		fn = partial(self.column_filename, n)
 		def getsize(sliceno):
 			try:
 				if self.lines[sliceno] == 0:
 					# if it's not used it shouldn't exist, so make sure it doesn't
-					os.unlink(fn % (sliceno,))
+					os.unlink(fn(sliceno))
 					return None
-				return os.path.getsize(fn % (sliceno,))
+				return os.path.getsize(fn(sliceno))
 			except FileNotFoundError:
 				return None
 		sizes = [(sliceno, getsize(sliceno)) for sliceno, cnt in enumerate(self.lines)]
 		bare_sizes = [z for _, z in sizes if z]
 		if sum(bare_sizes) / (len(bare_sizes) or 1) > 524288: # arbitrary guess of good size
 			return
 		if sum(bare_sizes) == 0:
 			# dataset is empty, so it needs no location
 			self._data.columns[n] = self._data.columns[n]._replace(location=None)
 			return
 		offsets = []
 		pos = 0
-		with open(fn % ('m',), 'wb') as m_fh:
+		with open(fn('m'), 'wb') as m_fh:
 			for sliceno, size in sizes:
 				if size:
-					with open(fn % (sliceno,), 'rb') as p_fh:
+					with open(fn(sliceno), 'rb') as p_fh:
 						data = p_fh.read()
 					assert len(data) == size, "Slice %d is %d bytes, not %d?" % (sliceno, len(data), size,)
 					m_fh.write(data)
 					offsets.append(pos)
 				else:
 					# no need to waste space storing an offset that won't be used
 					offsets.append(False)
 				if size is not None:
-					os.unlink(fn % (sliceno,))
+					os.unlink(fn(sliceno))
 					pos += size
 		c = self._data.columns[n]
+		location = c.location.split('/', 1) # the jobid might have % in it, so split it off
 		self._data.columns[n] = c._replace(
 			offsets=offsets,
-			location=c.location % ('m',),
+			location='%s/%s' % (location[0], location[1] % ('m',)),
 		)
 
 	def _maybe_merge_fully(self, columns):
 		z = 0
 		compressions = set()
 		for n in columns:
 			dc = self._data.columns[n]
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/dependency.py` & `accelerator-2023.7.18.dev1/accelerator/dependency.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/deptree.py` & `accelerator-2023.7.18.dev1/accelerator/deptree.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/dispatch.py` & `accelerator-2023.7.18.dev1/accelerator/dispatch.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/dsutil.py` & `accelerator-2023.7.18.dev1/accelerator/dsutil.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/error.py` & `accelerator-2023.7.18.dev1/accelerator/error.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/a_example_options.py` & `accelerator-2023.7.18.dev1/accelerator/examples/a_example_options.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/a_example_writeslicedfile.py` & `accelerator-2023.7.18.dev1/accelerator/examples/a_example_writeslicedfile.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_dsexample-append.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_dsexample-append.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_dsexample-chain.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_dsexample-chain.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_dsexample-create.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_dsexample-create.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_dsexample-import_csv.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_dsexample-import_csv.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_dsexample-many_ds.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_dsexample-many_ds.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_example-build_job.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_example-build_job.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_example-equiv_hashes.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_example-equiv_hashes.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_example-files.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_example-files.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_example-link_jobs.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_example-link_jobs.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_example-options.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_example-options.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_tutorial01.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_tutorial01.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_tutorial02.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_tutorial02.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_tutorial03.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_tutorial03.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_tutorial04.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_tutorial04.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_tutorial05.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_tutorial05.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_urdexample-basic.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_urdexample-basic.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/build_urdexample-many_items.py` & `accelerator-2023.7.18.dev1/accelerator/examples/build_urdexample-many_items.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/examples/printer.py` & `accelerator-2023.7.18.dev1/accelerator/examples/printer.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/extras.py` & `accelerator-2023.7.18.dev1/accelerator/extras.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from __future__ import division
 
 import os
 import datetime
 import json
 from traceback import print_exc
 from collections import OrderedDict
+from functools import partial
 import sys
 
 from accelerator.compat import PY2, PY3, pickle, izip, iteritems, first_value
 from accelerator.compat import num_types, uni, unicode, str_types
 
 from accelerator.error import AcceleratorError
 from accelerator.job import Job, JobWithFile
@@ -55,14 +56,111 @@
 
 def _job_params(jobid):
 	from accelerator.setupfile import load_setup
 	d = load_setup(jobid)
 	_apply_typing(d.options, d.get('_typing', ()))
 	return d
 
+
+# _SavedFile isn't really intended to pickle safely, so only allow it
+# in the automatic pickling of analysis results.
+_SavedFile_allow_pickle = False
+
+class _SavedFile(object):
+	__slots__ = ('_filename', '_sliceno', '_loader',)
+
+	def __init__(self, filename, sliceno, loader):
+		self._filename = filename
+		self._sliceno = sliceno
+		self._loader = loader
+
+	def wait(self):
+		pass
+
+	def load(self):
+		self.wait()
+		return self._loader(self._filename, sliceno=self._sliceno)
+
+	@property
+	def filename(self):
+		return _fn(self._filename, None, self._sliceno)
+
+	@property
+	def path(self):
+		if self._filename.startswith('/'):
+			job = None
+		else:
+			from accelerator import g
+			job = g.job
+		return _fn(self._filename, job, self._sliceno)
+
+	def jobwithfile(self, extra=None):
+		from accelerator import g
+		return JobWithFile(g.job, self._filename, self._sliceno is not None, extra)
+
+	def remove(self):
+		# mark file as temp, so it will be deleted later (unless --keep-temp-files)
+		saved_files[self.filename] = True
+
+	def __getstate__(self):
+		if _SavedFile_allow_pickle:
+			return self._filename, self._sliceno, self._loader
+		else:
+			raise TypeError('Cannot pickle _SavedFile')
+
+	def __setstate__(self, state):
+		self._filename, self._sliceno, self._loader = state
+
+
+_backgrounded = []
+
+class _BackgroundSavedFile(_SavedFile):
+	__slots__ = ('_ok', '_process',)
+
+	def __init__(self, filename, sliceno, loader, saver, args, temp, hidden=False):
+		_SavedFile.__init__(self, filename, sliceno, loader)
+		if hidden:
+			self._ok = bool # dummy function
+		else:
+			self._ok = partial(saved_files.__setitem__, self.filename, temp)
+		from accelerator.mp import SimplifiedProcess
+		self._process = SimplifiedProcess(target=self._run, args=(saver, args,))
+		_backgrounded.append(self)
+
+	def _run(self, func, args):
+		from accelerator import g
+		g.running = 'server' # Hack to disable status messages from this process
+		func(*args)
+
+	def wait(self):
+		if self._process:
+			with status("Waiting for background save of " + self.filename):
+				self._wait()
+
+	def _wait(self):
+		if self._process:
+			self._process.join()
+			rc = self._process.exitcode
+			self._process = None
+			if rc:
+				raise IOError('Failed to save ' + self.filename)
+			self._ok()
+
+	def __setstate__(self, state):
+		_SavedFile.__setstate__(self, state)
+		self._process = None
+
+def _backgrounded_wait():
+	if _backgrounded:
+		with status("Waiting for background save(s)"):
+			for bs in _backgrounded:
+				bs._wait()
+			_backgrounded[:] = ()
+
+
 def job_params(jobid=None, default_empty=False):
 	if default_empty and not jobid:
 		return DotDict(
 			options=DotDict(),
 			datasets=DotDict(),
 			jobs=DotDict(),
 		)
@@ -83,20 +181,27 @@
 		prefix = job.path + '/'
 		d.files = sorted(fn[len(prefix):] if fn.startswith(prefix) else fn for fn in d.files)
 		version = 1
 	if version != 1:
 		raise AcceleratorError("Don't know how to load post.json version %d (in %s)" % (d.version, jobid,))
 	return d
 
-def pickle_save(variable, filename='result.pickle', sliceno=None, temp=None, _hidden=False):
-	filename = _fn(filename, None, sliceno)
+def _pickle_save(variable, filename, temp, _hidden):
 	with FileWriteMove(filename, temp, _hidden=_hidden) as fh:
 		# use protocol version 2 so python2 can read the pickles too.
 		pickle.dump(variable, fh, 2)
 
+def pickle_save(variable, filename='result.pickle', sliceno=None, temp=None, background=False, _hidden=False):
+	args = (variable, _fn(filename, None, sliceno), temp, _hidden)
+	if background:
+		return _BackgroundSavedFile(filename, sliceno, pickle_load, _pickle_save, args, temp, _hidden)
+	else:
+		_pickle_save(*args)
+		return _SavedFile(filename, sliceno, pickle_load)
+
 # default to encoding='bytes' because datetime.* (and probably other types
 # too) saved in python 2 fail to unpickle in python 3 otherwise. (Official
 # default is 'ascii', which is pretty terrible too.)
 def pickle_load(filename='result.pickle', jobid=None, sliceno=None, encoding='bytes'):
 	filename = _fn(filename, jobid, sliceno)
 	with status('Loading ' + filename):
 		with open(filename, 'rb') as fh:
@@ -111,14 +216,16 @@
 
 	You can pass tuples and sets (saved as lists).
 	On py2 you can also pass bytes that will be passed through compat.uni.
 
 	If you set sort_keys=False you can use OrderedDict to get whatever
 	order you like.
 	"""
+	# make sure to evaluate sort_keys only once, for test_job_save_background
+	sort_keys = bool(sort_keys)
 	if sort_keys:
 		dict_type = dict
 	else:
 		dict_type = OrderedDict
 	def typefix(e):
 		if isinstance(e, dict):
 			return dict_type((typefix(k), typefix(v)) for k, v in iteritems(e))
@@ -130,20 +237,27 @@
 			return e
 	variable = typefix(variable)
 	res = json.dumps(variable, indent=4, sort_keys=sort_keys)
 	if PY3 and not as_str:
 		res = res.encode('ascii')
 	return res
 
-def json_save(variable, filename='result.json', sliceno=None, sort_keys=True, _encoder=json_encode, temp=False):
-	filename = _fn(filename, None, sliceno)
+def _json_save(variable, filename, sort_keys, _encoder, temp):
 	with FileWriteMove(filename, temp) as fh:
 		fh.write(_encoder(variable, sort_keys=sort_keys))
 		fh.write(b'\n')
 
+def json_save(variable, filename='result.json', sliceno=None, sort_keys=True, _encoder=json_encode, temp=False, background=False):
+	args = (variable, _fn(filename, None, sliceno), sort_keys, _encoder, temp)
+	if background:
+		return _BackgroundSavedFile(filename, sliceno, json_load, _json_save, args, temp)
+	else:
+		_json_save(*args)
+		return _SavedFile(filename, sliceno, json_load)
+
 def _unicode_as_utf8bytes(obj):
 	if isinstance(obj, unicode):
 		return obj.encode('utf-8')
 	elif isinstance(obj, dict):
 		return DotDict((_unicode_as_utf8bytes(k), _unicode_as_utf8bytes(v)) for k, v in iteritems(obj))
 	elif isinstance(obj, list):
 		return [_unicode_as_utf8bytes(v) for v in obj]
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/g.py` & `accelerator-2023.7.18.dev1/accelerator/g.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/iowrapper.py` & `accelerator-2023.7.18.dev1/accelerator/iowrapper.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/job.py` & `accelerator-2023.7.18.dev1/accelerator/job.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ############################################################################
 #                                                                          #
 # Copyright (c) 2017 eBay Inc.                                             #
-# Modifications copyright (c) 2019-2022 Carl Drougge                       #
+# Modifications copyright (c) 2019-2023 Carl Drougge                       #
 # Modifications copyright (c) 2019-2020 Anders Berkeman                    #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
@@ -17,31 +17,39 @@
 # limitations under the License.                                           #
 #                                                                          #
 ############################################################################
 
 import os
 import re
 
-from collections import namedtuple
+from collections import namedtuple, OrderedDict
 from functools import wraps
 
 from accelerator.compat import unicode, PY2, PY3, open, iteritems, FileNotFoundError
-from accelerator.error import NoSuchJobError, NoSuchWorkdirError, NoSuchDatasetError
+from accelerator.error import NoSuchJobError, NoSuchWorkdirError, NoSuchDatasetError, AcceleratorError
 
 
 # WORKDIRS should live in the Automata class, but only for callers
 # (methods read it too, though hopefully only through the functions in this module)
 
 WORKDIRS = {}
 
 
 def dirnamematcher(name):
 	return re.compile(re.escape(name) + r'-[0-9]+$').match
 
 
+def _assert_is_normrelpath(path, dirtype):
+	norm = os.path.normpath(path)
+	if (norm != path and norm + '/' != path) or norm.startswith('/'):
+		raise AcceleratorError('%r is not a normalised relative path' % (path,))
+	if norm == '..' or norm.startswith('../'):
+		raise AcceleratorError('%r is above the %s dir' % (path, dirtype))
+
+
 def _cachedprop(meth):
 	@property
 	@wraps(meth)
 	def wrapper(self):
 		if meth.__name__ not in self._cache:
 			self._cache[meth.__name__] = meth(self)
 		return self._cache[meth.__name__]
@@ -171,48 +179,69 @@
 
 	@_cachedprop
 	def datasets(self):
 		from accelerator.dataset import job_datasets
 		return job_datasets(self)
 
 	def output(self, what=None):
+		if what == 'parts':
+			as_parts = True
+			what = None
+		else:
+			as_parts = False
 		if isinstance(what, int):
-			fns = [str(what)]
+			fns = [what]
 		else:
 			assert what in (None, 'prepare', 'analysis', 'synthesis'), 'Unknown output %r' % (what,)
 			if what in (None, 'analysis'):
-				fns = [str(sliceno) for sliceno in range(self.params.slices)]
+				fns = list(range(self.params.slices))
 				if what is None:
 					fns = ['prepare'] + fns + ['synthesis']
 			else:
 				fns = [what]
-		res = []
-		for fn in fns:
-			fn = self.filename('OUTPUT/' + fn)
+		res = OrderedDict()
+		for k in fns:
+			fn = self.filename('OUTPUT/' + str(k))
 			if os.path.exists(fn):
 				with open(fn, 'rt', encoding='utf-8', errors='backslashreplace') as fh:
-					res.append(fh.read())
-		return ''.join(res)
+					res[k] = fh.read()
+		if as_parts:
+			return res
+		else:
+			return ''.join(res.values())
 
 	def link_result(self, filename='result.pickle', linkname=None):
 		"""Put a symlink to filename in result_directory
 		Only use this in a build script."""
 		from accelerator.g import running
 		assert running == 'build', "Only link_result from a build script"
 		from accelerator.shell import cfg
+		_assert_is_normrelpath(filename, 'job')
 		if linkname is None:
-			linkname = filename
+			linkname = os.path.basename(filename.rstrip('/'))
+		_assert_is_normrelpath(linkname, 'result')
+		if linkname.endswith('/'):
+			if filename.endswith('/'):
+				linkname = linkname.rstrip('/')
+			else:
+				linkname += os.path.basename(filename)
+		source_fn = os.path.join(self.path, filename)
+		assert os.path.exists(source_fn), "Filename \"%s\" does not exist in jobdir \"%s\"!" % (filename, self.path)
 		result_directory = cfg['result_directory']
-		dest_fn = os.path.join(result_directory, linkname)
+		dest_fn = result_directory
+		for part in linkname.split('/'):
+			if not os.path.exists(dest_fn):
+				os.mkdir(dest_fn)
+			elif dest_fn != result_directory and os.path.islink(dest_fn):
+				raise AcceleratorError("Refusing to create link %r: %r is a symlink" % (linkname, dest_fn))
+			dest_fn = os.path.join(dest_fn, part)
 		try:
 			os.remove(dest_fn + '_')
 		except OSError:
 			pass
-		source_fn = os.path.join(self.path, filename)
-		assert os.path.exists(source_fn), "Filename \"%s\" does not exist in jobdir \"%s\"!" % (filename, self.path)
 		os.symlink(source_fn, dest_fn + '_')
 		os.rename(dest_fn + '_', dest_fn)
 
 	def chain(self, length=-1, reverse=False, stop_job=None):
 		"""Like Dataset.chain but for jobs."""
 		if isinstance(stop_job, dict):
 			assert len(stop_job) == 1, "Only pass a single stop_job={job: name}"
@@ -246,21 +275,21 @@
 		return obj
 
 	def finish_early(self, result=None):
 		"""Finish job (successfully) without running later stages"""
 		from accelerator.launch import _FinishJob
 		raise _FinishJob(result)
 
-	def save(self, obj, filename='result.pickle', sliceno=None, temp=None):
+	def save(self, obj, filename='result.pickle', sliceno=None, temp=None, background=False):
 		from accelerator.extras import pickle_save
-		pickle_save(obj, filename, sliceno, temp=temp)
+		return pickle_save(obj, filename, sliceno, temp=temp, background=background)
 
-	def json_save(self, obj, filename='result.json', sliceno=None, sort_keys=True, temp=None):
+	def json_save(self, obj, filename='result.json', sliceno=None, sort_keys=True, temp=None, background=False):
 		from accelerator.extras import json_save
-		json_save(obj, filename, sliceno, sort_keys=sort_keys, temp=temp)
+		return json_save(obj, filename, sliceno, sort_keys=sort_keys, temp=temp, background=background)
 
 	def datasetwriter(self, columns={}, filename=None, hashlabel=None, hashlabel_override=False, caption=None, previous=None, name='default', parent=None, meta_only=False, for_single_slice=None, copy_mode=False, allow_missing_slices=False):
 		from accelerator.dataset import DatasetWriter
 		return DatasetWriter(columns=columns, filename=filename, hashlabel=hashlabel, hashlabel_override=hashlabel_override, caption=caption, previous=previous, name=name, parent=parent, meta_only=meta_only, for_single_slice=for_single_slice, copy_mode=copy_mode, allow_missing_slices=allow_missing_slices)
 
 	def open(self, filename, mode='r', sliceno=None, encoding=None, errors=None, temp=None):
 		"""Mostly like standard open with sliceno and temp,
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/launch.py` & `accelerator-2023.7.18.dev1/accelerator/launch.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ############################################################################
 #                                                                          #
 # Copyright (c) 2017 eBay Inc.                                             #
-# Modifications copyright (c) 2018-2022 Carl Drougge                       #
+# Modifications copyright (c) 2018-2023 Carl Drougge                       #
 # Modifications copyright (c) 2020 Anders Berkeman                         #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
@@ -82,14 +82,16 @@
 		os.dup2(output_fds[sliceno_], 1)
 		os.dup2(output_fds[sliceno_], 2)
 		for fd in output_fds:
 			os.close(fd)
 		os.close(_prof_fd)
 		slicename = 'analysis(%d)' % (sliceno_,)
 		setproctitle(slicename)
+		from accelerator.extras import saved_files, _backgrounded_wait
+		saved_files.clear() # don't inherit (and then return) the files from prepare
 		if delayed_start:
 			os.close(delayed_start[1])
 			update = statmsg._start('waiting for concurrency limit (%d)' % (sliceno_,), parent_pid, True)
 			if os.read(delayed_start[0], 1) != b'a':
 				raise AcceleratorError('bad delayed_start, giving up')
 			update(slicename)
 			os.close(delayed_start[0])
@@ -123,36 +125,41 @@
 					if isinstance(v, defaultdict) and not picklable(v.default_factory):
 						return {k: fixup(v) for k, v in iteritems(d)}
 					else:
 						return dict(d)
 				else:
 					return d
 			def save(item, name):
-				blob.save(fixup(item), name, sliceno=sliceno_, temp=True)
+				from accelerator import extras
+				try:
+					extras._SavedFile_allow_pickle = True
+					blob.save(fixup(item), name, sliceno=sliceno_, temp=True)
+				finally:
+					extras._SavedFile_allow_pickle = False
 			if isinstance(res, tuple):
 				if sliceno_ == 0:
 					blob.save(len(res), "Analysis.tuple", temp=True)
 				for ix, item in enumerate(res):
 					save(item, "Analysis.%d." % (ix,))
 			else:
 				if sliceno_ == 0:
 					blob.save(False, "Analysis.tuple", temp=True)
 				save(res, "Analysis.")
-		from accelerator.extras import saved_files
 		dw_lens = {}
 		dw_minmax = {}
 		dw_compressions = {}
 		for name, dw in dataset._datasetwriters.items():
 			if dw._for_single_slice or sliceno_ == 0:
 				dw_compressions[name] = dw._compressions
 			if dw._for_single_slice in (None, sliceno_,):
 				dw.close()
 				dw_lens[name] = dw._lens
 				dw_minmax[name] = dw._minmax
 		c_fflush()
+		_backgrounded_wait()
 		q.put((sliceno_, monotonic(), saved_files, dw_lens, dw_minmax, dw_compressions, None, finishjob,))
 		q.close()
 	except:
 		c_fflush()
 		msg = fmt_tb(1)
 		print(msg)
 		q.put((sliceno_, monotonic(), {}, {}, {}, {}, msg, False,))
@@ -282,14 +289,16 @@
 				msg.append(' reached line %d' % (line_report[0].count,))
 			msg.append("\n")
 	msg.extend(format_exception_only(e_type, e))
 	return ''.join(msg)
 
 
 def execute_process(workdir, jobid, slices, concurrency, index=None, workdirs=None, server_url=None, subjob_cookie=None, parent_pid=0):
+	from accelerator.extras import _backgrounded_wait
+
 	WORKDIRS.update(workdirs)
 
 	g.job = jobid
 	setproctitle('launch')
 	path = os.path.join(workdir, jobid)
 	try:
 		os.chdir(path)
@@ -372,14 +381,15 @@
 					blob.save(finish.result, temp=False)
 			to_finish = [dw.name for dw in dataset._datasetwriters.values() if dw._started]
 			if to_finish:
 				with statmsg.status("Finishing datasets"):
 					for name in sorted(to_finish, key=dw_sortnum):
 						dataset._datasetwriters[name].finish()
 		c_fflush()
+		_backgrounded_wait()
 		prof['prepare'] = monotonic() - t
 	switch_output()
 	setproctitle('launch')
 	from accelerator.extras import saved_files
 	if analysis_func is dummy:
 		prof['per_slice'] = []
 		prof['analysis'] = 0
@@ -409,14 +419,15 @@
 		if dataset._datasetwriters:
 			with statmsg.status("Finishing datasets"):
 				for name in sorted(dataset._datasetwriters, key=dw_sortnum):
 					dataset._datasetwriters[name].finish()
 	if dataset._datasets_written:
 		blob.save(dataset._datasets_written, 'DS/LIST', temp=False, _hidden=True)
 	c_fflush()
+	_backgrounded_wait()
 	t = monotonic() - t
 	prof['synthesis'] = t
 
 	from accelerator.subjobs import _record
 	return None, (prof, saved_files, _record)
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/methods.py` & `accelerator-2023.7.18.dev1/accelerator/methods.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/mp.py` & `accelerator-2023.7.18.dev1/accelerator/mp.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/runner.py` & `accelerator-2023.7.18.dev1/accelerator/runner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ############################################################################
 #                                                                          #
 # Copyright (c) 2017 eBay Inc.                                             #
-# Modifications copyright (c) 2018-2022 Carl Drougge                       #
+# Modifications copyright (c) 2018-2023 Carl Drougge                       #
 # Modifications copyright (c) 2020 Anders Berkeman                         #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
@@ -38,15 +38,17 @@
 import struct
 import json
 import io
 import tarfile
 import resource
 import gc
 import re
-from threading import Thread, Lock
+from threading import Thread, Lock as TLock
+from multiprocessing import Lock as MPLock
+from accelerator.mp import SimplifiedProcess
 
 archives = {}
 
 def mod2filename(mod):
 	if isinstance(mod, ModuleType):
 		filename = getattr(mod, '__file__', None)
 		if filename and filename[-4:] in ('.pyc', '.pyo',):
@@ -396,15 +398,15 @@
 class Runner(object):
 	def __init__(self, pid, sock, python):
 		self.pid = pid
 		self.sock = sock
 		self.python = python
 		self.cookie = 0
 		self._waiters = {}
-		self._lock = Lock()
+		self._lock = TLock()
 		self._thread = Thread(
 			target=self._receiver,
 			name="%d receiver" % (pid,),
 		)
 		self._thread.daemon = True
 		self._thread.start()
 
@@ -534,15 +536,15 @@
 	from accelerator.autoflush import AutoFlush
 	from accelerator.compat import pickle
 	from accelerator.dispatch import update_valid_fds
 
 	sys.stdout = AutoFlush(sys.stdout)
 	sys.stderr = AutoFlush(sys.stderr)
 	sock = socket.fromfd(int(sys.argv[1]), socket.AF_UNIX, socket.SOCK_STREAM)
-	sock_lock = Lock()
+	sock_lock = MPLock()
 	update_valid_fds()
 
 	# Set the highest open file limit we can.
 	# At least OS X seems to like claiming no limit as max without
 	# allowing that to be set, so let's do some retrying.
 	r1, r2 = resource.getrlimit(resource.RLIMIT_NOFILE)
 	limits = [500000, 100000, 50000, 10000, 5000, 1000, r1, r2]
@@ -555,32 +557,41 @@
 			pass
 	r1, r2 = resource.getrlimit(resource.RLIMIT_NOFILE)
 	if r1 < r2:
 		print("WARNING: Failed to raise RLIMIT_NOFILE to %d. Set to %d." % (r2, r1,))
 	if r1 < 5000:
 		print("WARNING: RLIMIT_NOFILE is %d, that's not much." % (r1,))
 
-	while True:
-		op, length = struct.unpack('<cI', recvall(sock, 5, True))
-		data = recvall(sock, length, True)
-		cookie, data = pickle.loads(data)
-		if op == b'm':
-			res = load_methods(*data)
-			respond(cookie, res)
-		elif op == b's':
-			res = launch_start(data)
-			respond(cookie, res)
-		elif op == b'f':
-			# waits until job is done, so must run on a separate thread
-			Thread(
-				target=launch_finish,
-				args=(cookie, data,),
-				name=data[3], # jobid
-			).start()
-		elif op == b'w':
-			# It would be nice to be able to just ignore children
-			# (set SIGCHLD to SIG_IGN), but the server might want to
-			# killpg the child, so we need it to stick around.
-			os.waitpid(data, 0)
-			respond(cookie, None)
-		elif op == b'v':
-			respond(cookie, ax_version)
+	try:
+		while True:
+			op, length = struct.unpack('<cI', recvall(sock, 5, True))
+			data = recvall(sock, length, True)
+			cookie, data = pickle.loads(data)
+			if op == b'm':
+				res = load_methods(*data)
+				respond(cookie, res)
+			elif op == b's':
+				res = launch_start(data)
+				respond(cookie, res)
+			elif op == b'f':
+				# waits until job is done, so must run in a separate process
+				SimplifiedProcess(
+					target=launch_finish,
+					args=(cookie, data,),
+					name=data[3], # jobid
+				)
+				os.close(data[1]) # close prof_r in the parent
+			elif op == b'w':
+				# It would be nice to be able to just ignore children
+				# (set SIGCHLD to SIG_IGN), but the server might want to
+				# killpg the child, so we need it to stick around.
+				os.waitpid(data, 0)
+				respond(cookie, None)
+			elif op == b'v':
+				respond(cookie, ax_version)
+	except KeyboardInterrupt:
+		# Exiting with KeyboardInterrupt causes python to print a traceback,
+		# but let's not.
+		signal.signal(signal.SIGINT, signal.SIG_DFL)
+		os.kill(os.getpid(), signal.SIGINT)
+		# If that didn't work let's re-raise the KeyboardInterrupt.
+		raise
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/server.py` & `accelerator-2023.7.18.dev1/accelerator/server.py`

 * *Files 2% similar despite different names*

```diff
@@ -154,34 +154,45 @@
 			tokill = list(children)
 			print('Force abort', tokill)
 			for child in tokill:
 				os.killpg(child, signal.SIGKILL)
 			self.do_response(200, 'text/json', {'killed': len(tokill)})
 
 		elif path[0] == 'method2job':
-			method, num = path[1:]
-			jobs = self.ctrl.DataBase.db_by_method.get(method, ())
-			start_ix = 0
+			method = path[1]
+			if args.get('current', 'False') != 'False':
+				jobs = self.ctrl.DataBase.db_by_method.get(method, ())
+				typ = 'current'
+			else:
+				jobs = self.ctrl.DataBase.all_by_method.get(method, ())
+				typ = 'known'
 			start_from = args.get('start_from')
 			if start_from:
-				for start_ix, job in enumerate(jobs):
-					if job.id == start_from:
-						break
-				else:
+				try:
+					start_ix = jobs.index(start_from)
+				except ValueError:
 					start_ix = None
+			else:
+				start_ix = len(jobs) - 1
 			if start_ix is None:
-				res = {'error': '%s is not a current %s job' % (start_from, method,)}
+				res = {'error': '%s is not a %s %s job' % (start_from, typ, method,)}
 			else:
-				num = int(num)
+				num = int(args.get('offset', 0))
 				if not jobs:
-					res = {'error': 'no current jobs with method %s available' % (method,)}
-				elif num + start_ix >= len(jobs):
-					res = {'error': 'tried to go %d jobs back from %s, but only %d earlier (current) jobs available' % (num, jobs[start_ix].id, len(jobs) - start_ix - 1,)}
+					res = {'error': 'no %s jobs with method %s available' % (typ, method,)}
+				elif 0 <= start_ix + num < len(jobs):
+					res = {'id': jobs[start_ix + num]}
 				else:
-					res = {'id': jobs[num + start_ix].id}
+					if num < 0:
+						direction, kind = 'back', 'earlier'
+						available = start_ix
+					else:
+						direction, kind = 'forward', 'later'
+						available = len(jobs) - start_ix - 1
+					res = {'error': 'tried to go %d jobs %s from %s, but only %d %s %s %s jobs available' % (abs(num), direction, jobs[start_ix], available, kind, typ, method,)}
 			self.do_response(200, 'text/json', res)
 
 		elif path[0] == 'job_is_current':
 			job = Job(path[1])
 			job = self.ctrl.DataBase.db_by_workdir[job.workdir].get(job)
 			self.do_response(200, 'text/json', bool(job and job['current']))
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/setupfile.py` & `accelerator-2023.7.18.dev1/accelerator/setupfile.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/shell/__init__.py` & `accelerator-2023.7.18.dev1/accelerator/shell/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 from __future__ import unicode_literals
 
 import sys
 import errno
 import os
 from os.path import dirname, basename, realpath, join
 import locale
+from collections import namedtuple
 from glob import glob
 import re
 import shlex
 import signal
 from argparse import RawDescriptionHelpFormatter
 
 from accelerator.colourwrapper import colour
@@ -102,54 +103,87 @@
 		WORKDIRS[k] = v
 	return cfg
 
 def unpath(path):
 	while path in sys.path:
 		sys.path.pop(sys.path.index(path))
 
+# This is used as "cfg" when no config is found (or parsing fails).
+# Once the command tries to use cfg the original exception from loading the
+# config is raised. But if the command doesn't use the cfg no exception is
+# raised, so e.g. --help works.
+class NoConfig(object):
+	def __init__(self, e, user_cwd):
+		self._e = e
+		self.user_cwd = user_cwd
+		self.project_directory = user_cwd
+
+	def __getattr__(self, name):
+		raise self._e
+
+	def __getitem__(self, name):
+		return getattr(self, name)
+
 def setup(config_fn=None, debug_cmd=False):
+	global cfg
 	try:
 		locale.resetlocale()
 	except locale.Error:
 		print("WARNING: Broken locale", file=sys.stderr)
 	# Make sure the accelerator dir in not in sys.path
 	# (as it might be if running without installing.)
 	unpath(dirname(__file__))
 	if config_fn is False:
 		return
 	user_cwd = os.getcwd()
 	if config_fn:
 		load_cfg(config_fn)
 	else:
-		load_some_cfg(all=debug_cmd)
+		try:
+			load_some_cfg(all=debug_cmd)
+		except UserError as e:
+			cfg = NoConfig(e, user_cwd)
 	cfg.user_cwd = user_cwd
 	if not debug_cmd:
 		# We want the project directory to be first in sys.path.
 		unpath(cfg['project_directory'])
 		sys.path.insert(0, cfg['project_directory'])
 		# For consistency we also always want the project dir
 		# as working directory.
 		os.chdir(cfg['project_directory'])
 
-def cmd_grep(argv):
-	from accelerator.shell.grep import main
-	return main(argv, cfg)
-cmd_grep.help = '''search for a pattern in one or more datasets'''
-cmd_grep.is_debug = True
-
-def cmd_ds(argv):
-	from accelerator.shell.ds import main
-	return main(argv, cfg)
-cmd_ds.help = '''display information about datasets'''
-cmd_ds.is_debug = True
-
-def cmd_run(argv):
-	from accelerator.build import main
-	return main(argv, cfg)
-cmd_run.help = '''run a build script'''
+
+class Command(namedtuple('Command', 'name help is_debug modname')):
+	def __call__(self, argv):
+		from importlib import import_module
+		mod = import_module(self.modname)
+		return mod.main(argv, cfg)
+
+_COMMANDS = {}
+
+def add_command(name, help, is_debug=False, modname=None):
+	if not modname:
+		modname = 'accelerator.shell.' + name.replace('-', '_')
+	assert name not in _COMMANDS, name
+	_COMMANDS[name] = Command(name, help, is_debug, modname)
+
+add_command('board-server', '''runs a webserver for displaying results''',      modname='accelerator.board')
+add_command('ds',           '''display information about datasets''',           is_debug=True)
+add_command('gc',           '''delete stale and unused jobs''')
+add_command('grep',         '''search for a pattern in one or more datasets''', is_debug=True)
+add_command('init',         '''create a project directory''')
+add_command('job',          '''information about a job''',                      is_debug=True)
+add_command('method',       '''information about methods''')
+add_command('run',          '''run a build script''',                           modname='accelerator.build')
+add_command('script',       '''information about build scripts''')
+add_command('status',       '''server status (like ^T when building)''')
+add_command('urd',          '''inspect urd contents''')
+add_command('urd-server',   '''run the urd server''',                           modname='accelerator.urd')
+add_command('workdir',      '''information about workdirs''', is_debug=True)
+
 
 def cmd_abort(argv):
 	parser = ArgumentParser(prog=argv.pop(0))
 	parser.add_argument('-q', '--quiet', action='store_true', negation='not', help="no output")
 	args = parser.parse_intermixed_args(argv)
 	from accelerator.build import Automata
 	a = Automata(cfg.url)
@@ -180,56 +214,14 @@
 	from accelerator.methods import MethodLoadException
 	try:
 		main(argv, cfg)
 	except MethodLoadException as e:
 		print(e)
 cmd_server.help = '''run the main server'''
 
-def cmd_script(argv):
-	from accelerator.shell.script import main
-	return main(argv, cfg)
-cmd_script.help = '''information about build scripts'''
-
-def cmd_init(argv):
-	from accelerator.shell.init import main
-	main(argv)
-cmd_init.help = '''create a project directory'''
-
-def cmd_urd(argv):
-	from accelerator.shell.urd import main
-	return main(argv, cfg)
-cmd_urd.help = '''inspect urd contents'''
-
-def cmd_urd_server(argv):
-	from accelerator.urd import main
-	main(argv, cfg)
-cmd_urd_server.help = '''run the urd server'''
-
-def cmd_method(argv):
-	from accelerator.shell.method import main
-	main(argv, cfg)
-cmd_method.help = '''information about methods'''
-
-def cmd_workdir(argv):
-	from accelerator.shell.workdir import main
-	main(argv, cfg)
-cmd_workdir.help = '''information about workdirs'''
-cmd_workdir.is_debug = True
-
-def cmd_job(argv):
-	from accelerator.shell.job import main
-	return main(argv, cfg)
-cmd_job.help = '''information about a job'''
-cmd_job.is_debug = True
-
-def cmd_board_server(argv):
-	from accelerator.board import main
-	main(argv, cfg)
-cmd_board_server.help = '''runs a webserver for displaying results'''
-
 def cmd_intro(argv):
 	parser = ArgumentParser(prog=argv.pop(0))
 	parser.parse_intermixed_args(argv)
 	from accelerator import __version__ as ax_version
 	def cmd(txt, *a):
 		print('  ' + colour(txt, 'intro/highlight', *a))
 	def msg(txt='', c='intro/info'):
@@ -279,32 +271,14 @@
 			impl_version = '.'.join(map(str, sys.implementation.version))
 			py_version = '%s %s' % (py_version, impl_version,)
 		except Exception:
 			pass
 		print('Running on ' + py_version + suffix)
 cmd_version.help = '''show installed accelerator version'''
 
-COMMANDS = {
-	'abort': cmd_abort,
-	'alias': cmd_alias,
-	'board-server': cmd_board_server,
-	'ds': cmd_ds,
-	'grep': cmd_grep,
-	'init': cmd_init,
-	'intro': cmd_intro,
-	'job': cmd_job,
-	'method': cmd_method,
-	'run': cmd_run,
-	'server': cmd_server,
-	'script': cmd_script,
-	'urd': cmd_urd,
-	'urd-server': cmd_urd_server,
-	'version': cmd_version,
-	'workdir': cmd_workdir,
-}
 
 def split_args(argv):
 	prev = None
 	for ix, arg in enumerate(argv):
 		if not arg.startswith('-') and prev != '--config':
 			return argv[:ix], argv[ix:]
 		prev = arg
@@ -488,14 +462,24 @@
 		'oddlines': ('BLACK', 'BRIGHTWHITEBG',),
 	}
 	parse_user_config(aliases, colour_d)
 	colour._names.update(colour_d)
 
 	main_argv, argv = expand_aliases(main_argv, argv)
 
+	# any function cmd_* in this file is a command
+	COMMANDS = {
+		k[4:].replace('_', '-'): v
+		for k, v in globals().items()
+		if k.startswith('cmd_') and callable(v)
+	}
+	# as is anything in _COMMANDS (i.e. from add_command)
+	assert not set(COMMANDS).intersection(_COMMANDS)
+	COMMANDS.update(_COMMANDS)
+
 	epilog = ['commands:', '']
 	cmdlen = max(len(cmd) for cmd in COMMANDS)
 	template = '  %%%ds  %%s' % (cmdlen,)
 	for cmd, func in sorted(COMMANDS.items()):
 		epilog.append(template % (cmd, func.help,))
 	epilog.append('')
 	epilog.append('aliases:')
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/shell/ds.py` & `accelerator-2023.7.18.dev1/accelerator/shell/ds.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/shell/grep.py` & `accelerator-2023.7.18.dev1/accelerator/shell/grep.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/shell/init.py` & `accelerator-2023.7.18.dev1/accelerator/shell/init.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ############################################################################
 #                                                                          #
-# Copyright (c) 2019-2022 Carl Drougge                                     #
+# Copyright (c) 2019-2023 Carl Drougge                                     #
 # Modifications copyright (c) 2020 Anders Berkeman                         #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
@@ -148,15 +148,15 @@
 		fh.write('/workdirs\n')
 		fh.write('/results\n')
 		fh.write('__pycache__\n')
 		fh.write('*.pyc\n')
 	check_call(['git', 'add', '--', 'accelerator.conf', '.gitignore', method_dir])
 
 
-def main(argv):
+def main(argv, cfg):
 	from os import makedirs, listdir, chdir
 	from os.path import exists, join, realpath, dirname
 	from sys import version_info
 	from argparse import RawTextHelpFormatter
 	from accelerator.shell.parser import ArgumentParser
 	from accelerator.compat import shell_quote
 	from accelerator.error import UserError
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/shell/job.py` & `accelerator-2023.7.18.dev1/accelerator/shell/job.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ############################################################################
 #                                                                          #
-# Copyright (c) 2020-2022 Carl Drougge                                     #
+# Copyright (c) 2020-2023 Carl Drougge                                     #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
 #                                                                          #
@@ -19,74 +19,103 @@
 from __future__ import print_function
 from __future__ import division
 from __future__ import unicode_literals
 
 from traceback import print_exc
 from datetime import datetime
 import errno
+import json
 from argparse import RawTextHelpFormatter
 import os
 import sys
 
+from accelerator.build import fmttime
 from accelerator.colourwrapper import colour
 from accelerator.error import NoSuchJobError
 from accelerator.setupfile import encode_setup
 from accelerator.compat import FileNotFoundError, url_quote, urlencode
 from accelerator.unixhttp import call
 from .parser import name2job, ArgumentParser
 
-def show(url, job, show_output):
-	print(job.path)
-	print('=' * len(job.path))
+def show(url, job, verbose, show_output):
 	setup = job.json_load('setup.json')
-	setup.pop('_typing', None)
-	setup.starttime = str(datetime.fromtimestamp(setup.starttime))
-	if 'endtime' in setup:
-		setup.endtime = str(datetime.fromtimestamp(setup.endtime))
-	print(encode_setup(setup, as_str=True))
-	if job.datasets:
+	if verbose:
+		print(colour(job.path, 'job/header'))
+		print(colour('=' * len(job.path), 'job/header'))
+		setup.pop('_typing', None)
+		setup.starttime = str(datetime.fromtimestamp(setup.starttime))
+		if 'endtime' in setup:
+			setup.endtime = str(datetime.fromtimestamp(setup.endtime))
+		print(encode_setup(setup, as_str=True))
+	else:
+		starttime = datetime.fromtimestamp(setup.starttime).replace(microsecond=0)
+		hdr = '%s (%s) at %s' % (job, job.method, starttime,)
+		if 'exectime' in setup:
+			hdr = '%s in %s' % (hdr, fmttime(setup.exectime.total),)
+		print(colour(hdr, 'job/header'))
+		things = []
+		def opt_thing(name):
+			value = setup[name]
+			if value:
+				if isinstance(value, dict) and len(value) > 1:
+					value = json.dumps(value, indent=4, sort_keys=True).replace('\n', '\n    ')
+				else:
+					value = json.dumps(value)
+				things.append((name, value,))
+		opt_thing('caption')
+		opt_thing('options')
+		opt_thing('datasets')
+		opt_thing('jobs')
+		for k, v in things:
+			print('    %s: %s' % (k, v,))
+	def list_of_things(name, things):
+		total = len(things)
+		if total > 5 and not verbose:
+			things = things[:3]
 		print()
-		print('datasets:')
-		for ds in job.datasets:
-			print('   ', ds.quoted)
+		print(colour('%s:' % (name,), 'job/header'))
+		for thing in things:
+			print('   ', thing)
+		if total > len(things):
+			print('    ... and %d more' % (total - len(things),))
+	if job.datasets:
+		list_of_things('datasets', [ds.quoted for ds in job.datasets])
 	try:
 		post = job.json_load('post.json')
 	except FileNotFoundError:
 		print(colour('WARNING: Job did not finish', 'job/warning'))
 		post = None
 	if post and post.subjobs:
-		print()
-		print('subjobs:')
 		postdata = urlencode({'jobs': '\0'.join(post.subjobs)}).encode('utf-8')
 		subjobs = call(url + '/jobs_are_current', data=postdata)
+		fmted_subjobs = []
 		for sj, is_current in sorted(subjobs.items()):
-			print('   ', sj, end='')
 			if not is_current:
-				print('', colour('(not current)', 'job/info'), end='')
-			print()
+				sj += ' ' + colour('(not current)', 'job/info')
+			fmted_subjobs.append(sj)
+		list_of_things('subjobs', fmted_subjobs)
 	if post and post.files:
-		print()
-		print('files:')
-		for fn in sorted(post.files):
-			print('   ', job.filename(fn))
+		files = sorted(post.files)
+		if verbose:
+			files = [job.filename(fn) for fn in files]
+		list_of_things('files', files)
 	if post and not call(url + '/job_is_current/' + url_quote(job)):
 		print(colour('Job is not current', 'job/info'))
 	print()
-	out = job.output()
+	out = job.output('parts')
 	if show_output:
 		if out:
-			print('output (use --just-output/-O to see only the output):')
-			print(out)
-			if not out.endswith('\n'):
-				print()
+			if not verbose: # verbose prints section headers in show_output_d()
+				print(colour('output:', 'job/header'))
+			show_output_d(out, verbose)
 		else:
 			print(job, 'produced no output')
 			print()
 	elif out:
-		print('%s produced %d bytes of output, use --output/-o to see it' % (job, len(out),))
+		print('%s produced %d bytes of output, use --output/-o to see it' % (job, sum(len(v) for v in out.values()),))
 		print()
 
 def show_source(job, pattern='*'):
 	import tarfile
 	from fnmatch import fnmatch
 	with tarfile.open(job.filename('method.tar.gz'), 'r:gz') as tar:
 		all_members = [info for info in tar.getmembers() if info.isfile()]
@@ -154,61 +183,76 @@
 			data = data[os.write(1, data):]
 		if not has_nl:
 			os.write(1, b'\n')
 		if ix < len(files):
 			os.write(1, b'\n')
 	return 0
 
+def show_output_d(d, verbose):
+	first = True
+	for k, out in d.items():
+		if out:
+			if verbose:
+				if first:
+					first = False
+				else:
+					print()
+				if isinstance(k, int):
+					k = 'analysis(%d)' % (k,)
+				print(colour(k, 'job/header'))
+				print(colour('=' * len(k), 'job/header'))
+			print(out, end='' if out.endswith('\n') else '\n')
+
 def main(argv, cfg):
 	descr = 'show setup.json, dataset list, etc for jobs'
 	parser = ArgumentParser(
 		prog=argv.pop(0),
 		description=descr,
 		formatter_class=RawTextHelpFormatter,
 	)
+	parser.add_argument('-v', '--verbose', action='store_true', negation='not', help='more output (e.g the whole setup.json)')
 	group = parser.add_mutually_exclusive_group()
 	group.add_argument('-o', '--output', action='store_true', help='show job output')
 	group.add_argument('-O', '--just-output', action='store_true', help='show only job output')
 	group.add_argument('-P', '--just-path', action='store_true', help='show only job path')
 	group.add_argument('-s', '--source', action='store_true', help='show source used to produce job')
 	group.add_argument('-S', '--source-file', metavar='PATTERN', nargs='?', const='', help='show specified file(s) from source used to produce job')
 	group.add_argument('-f', '--file', metavar='PATTERN', nargs='?', const='', help='show specified file(s) produced by job')
 	parser.add_argument(
 		'jobid',
 		nargs='+', metavar='jobid/jobspec',
 		help='jobid is just a jobid.\n' +
 		     'you can also use path, method or :urdlist:[entry].\n' +
 		     'path is to a jobdir (with setup.json in it).\n' +
-		     'method is the latest (current) job with that method (i.e\n' +
-		     'the latest finished job with current source code).\n' +
+		     'method is the latest job with that method.\n' +
 		     ':urdlist:[entry] looks up jobs in urd. details are in the\n' +
 		     'urd help, except here entry defaults to -1 and you can\'t\n' +
 		     'list things (no .../ or .../since/x).\n' +
-		     'you can use spec~ or spec~N to go back N current jobs\n' +
-		     'with that method or spec^ or spec^N to follow .previous'
+		     'you can use spec~ or spec~N to go back N jobs\n' +
+		     'with that method or spec^ or spec^N to follow .previous\n' +
+		     'use spec! to only consider current jobs.\n' +
+		     'you can also do things like spec.source.'
 	)
 	args = parser.parse_intermixed_args(argv)
 	res = 0
 	for path in args.jobid:
 		try:
 			job = name2job(cfg, path)
 			if args.just_output:
-				out = job.output()
-				if out:
-					print(out, end='' if out.endswith('\n') else '\n')
+				show_output_d(job.output('parts'), args.verbose)
 			elif args.just_path:
 				print(job.path)
 			elif args.source:
 				res |= show_source(job)
 			elif args.source_file is not None:
 				res |= show_source(job, args.source_file)
 			elif args.file is not None:
 				res |= show_file(job, args.file)
 			else:
-				show(cfg.url, job, args.output)
+				show(cfg.url, job, args.verbose, args.output)
 		except NoSuchJobError as e:
 			print(e)
 			res = 1
 		except Exception as e:
 			if isinstance(e, OSError) and e.errno == errno.EPIPE:
 				raise
 			print_exc(file=sys.stderr)
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/shell/lined.py` & `accelerator-2023.7.18.dev1/accelerator/shell/lined.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/shell/method.py` & `accelerator-2023.7.18.dev1/accelerator/shell/method.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/shell/parser.py` & `accelerator-2023.7.18.dev1/accelerator/shell/parser.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,59 +25,59 @@
 
 import argparse
 import sys
 from os.path import join, exists, realpath, split
 from os import readlink, environ
 import re
 
+from accelerator.dataset import Dataset
 from accelerator.job import WORKDIRS
 from accelerator.job import Job
 from accelerator.error import NoSuchJobError, NoSuchDatasetError, NoSuchWorkdirError, UrdError
 from accelerator.unixhttp import call
-from accelerator.compat import url_quote, PY3
+from accelerator.compat import url_quote, urlencode, PY3
 
 class JobNotFound(NoSuchJobError):
 	pass
 
 class DatasetNotFound(NoSuchDatasetError):
 	pass
 
 def _groups(tildes):
 	def char_and_count(buf):
-		char, count = re.match(r'([~^]+)(\d*)$', ''.join(buf)).groups()
+		char, count = re.match(r'([~+<>^]+)(\d*)$', ''.join(buf)).groups()
 		count = int(count or 1) - 1
 		return char[0], len(char) + count
 	i = iter(tildes)
 	buf = [next(i)]
 	for c in i:
-		if c in '~^' and buf[-1] != c:
+		if c in '~+<>^' and buf[-1] != c:
 			yield char_and_count(buf)
 			buf = [c]
 		else:
 			buf.append(c)
 	yield char_and_count(buf)
 
 # "foo~~^3" -> "foo", [("~", 2), ("^", 3)]
-def split_tildes(n, allow_empty=False):
-	m = re.match(r'(.*?)([~^][~^\d]*)$', n)
+def split_tildes(n, allow_empty=False, extended=False):
+	if extended:
+		m = re.match(r'(.*?)([~+<>^][~+<>^\d]*)$', n)
+	else:
+		m = re.match(r'(.*?)([~^][~^\d]*)$', n)
 	if m:
 		n, tildes = m.groups()
 		lst = list(_groups(tildes))
 	else:
 		lst = []
 	assert n or allow_empty, "empty job id"
 	return n, lst
 
-def method2job(cfg, method, count=0, start_from=None):
-	def get(count):
-		url ='%s/method2job/%s/%s' % (cfg.url, url_quote(method), count)
-		if start_from:
-			url += '?start_from=' + url_quote(start_from)
-		return call(url)
-	found = get(count)
+def method2job(cfg, method, **kw):
+	url ='%s/method2job/%s?%s' % (cfg.url, url_quote(method), urlencode(kw))
+	found = call(url)
 	if 'error' in found:
 		raise JobNotFound(found.error)
 	return Job(found.id)
 
 # follow jobs.previous (or datasets.previous.job if that is unavailable) count times.
 def job_up(job, count):
 	err_job = job
@@ -104,26 +104,87 @@
 			pos = timestamps.index(res.timestamp) + tildes
 			if pos < 0 or pos >= len(timestamps):
 				return None
 			res = call(cfg.urd + '/' + key + '/' + timestamps[pos], server_name='urd', retries=0, quiet=True)
 	return res
 
 def name2job(cfg, n):
-	n, tildes = split_tildes(n)
-	job = _name2job(cfg, n)
+	if '.' in n:
+		n, dotted = n.split('.', 1)
+		dotted = iter(dotted.split('.'))
+	else:
+		dotted = None
+	def split(n, what):
+		n, tildes = split_tildes(n, extended=True, allow_empty=True)
+		if n.endswith('!'):
+			current = True
+			n = n[:-1]
+		else:
+			current = False
+		assert n, "empty " + what
+		return n, current, tildes
+	n, current, tildes = split(n, "job id")
+	job = _name2job(cfg, n, current)
+	job = _name2job_do_tildes(cfg, job, current, tildes)
+	if dotted:
+		for n in dotted:
+			n, current, tildes = split(n, "param")
+			p = job.params
+			k = None
+			if n in ('jobs', 'datasets'):
+				k = n
+				try:
+					n = next(dotted)
+				except StopIteration:
+					raise JobNotFound("%s.%s.what?" % (job, k,))
+			elif n in p.jobs and n in p.datasets:
+				raise JobNotFound("Job %s (%s) has %s in both .jobs and .datasets, please specify." % (job, job.method, n,))
+			if k:
+				if n not in p[k]:
+					raise JobNotFound("Job %s (%s) does not have a %r." % (job, job.method, k + '.' + n,))
+			else:
+				if n in p.jobs:
+					k = 'jobs'
+				elif n in p.datasets:
+					k = 'datasets'
+				else:
+					raise JobNotFound("Job %s (%s) does not have a %r." % (job, job.method, n,))
+			if not p[k][n]:
+				raise JobNotFound("%s.%s.%s is None" % (job, k, n,))
+			job = p[k][n]
+			if isinstance(job, list):
+				if len(job) != 1:
+					raise JobNotFound("Job %s (%s) has %d %s in %r." % (job, job.method, len(job), k, n,))
+				job = job[0]
+			if isinstance(job, Dataset):
+				job = job.job
+			job = _name2job_do_tildes(cfg, job, current, tildes)
+	return job
+
+def _name2job_do_tildes(cfg, job, current, tildes):
 	for char, count in tildes:
 		if char == '~':
-			job = method2job(cfg, job.method, count, start_from=job)
-		else:
+			job = method2job(cfg, job.method, offset=-count, start_from=job, current=current)
+		elif char == '+':
+			job = method2job(cfg, job.method, offset=count, start_from=job, current=current)
+		elif char == '^':
 			job = job_up(job, count)
+		elif char == '<':
+			if count > job.number:
+				raise JobNotFound('Tried to go %d jobs back from %s.' % (count, job,))
+			job = Job._create(job.workdir, job.number - count)
+		elif char == '>':
+			job = Job._create(job.workdir, job.number + count)
+		else:
+			raise Exception("BUG: split_tildes should not give %r as a char" % (char,))
 	if not exists(job.filename('setup.json')):
 		raise JobNotFound('Job resolved to %r but that job does not exist' % (job,))
 	return job
 
-def _name2job(cfg, n):
+def _name2job(cfg, n, current):
 	if n.startswith(':'):
 		# resolve through urd
 		assert cfg.urd, 'No urd configured'
 		a = n[1:].rsplit(':', 1)
 		if len(a) == 1:
 			raise JobNotFound('looks like a partial :urdlist:[entry] spec')
 		entry = a[1] or '-1'
@@ -164,15 +225,15 @@
 		try:
 			n = readlink(path)
 		except OSError as e:
 			raise JobNotFound('Failed to read %s: %s' % (path, e,))
 		return Job(n)
 	if n not in ('.', '..') and '/' not in n:
 		# Must be a method then
-		return method2job(cfg, n)
+		return method2job(cfg, n, current=current)
 	if exists(join(n, 'setup.json')):
 		# Looks like the path to a jobdir
 		path, jid = split(realpath(n))
 		job = Job(jid)
 		if WORKDIRS.get(job.workdir, path) != path:
 			print("### Overriding workdir %s to %s" % (job.workdir, path,))
 		WORKDIRS[job.workdir] = path
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/shell/script.py` & `accelerator-2023.7.18.dev1/accelerator/shell/script.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/shell/urd.py` & `accelerator-2023.7.18.dev1/accelerator/shell/urd.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ############################################################################
 #                                                                          #
-# Copyright (c) 2021 Carl Drougge                                          #
+# Copyright (c) 2021-2023 Carl Drougge                                     #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
 #                                                                          #
@@ -118,39 +118,45 @@
 		if not res:
 			continue
 		print(fmt(res, entry))
 
 def fmt(res, entry):
 	if not res:
 		return ''
-	def fmt_caption(path, caption):
-		return template % (path, caption,) if caption else path
+	def fix_caption(caption, indent):
+		caption = caption.replace('\r', '').strip()
+		if '\x1b' in caption:
+			caption += '\x1b[m'
+		caption = caption.replace('\n', '\n   ' + ' ' * indent)
+		return caption
+	def fmt_caption(path, caption, indent):
+		return template % (path, fix_caption(caption, indent),) if caption else path
 	if isinstance(res, list):
 		if isinstance(res[0], list):
 			tlen = max(len(ts) for ts, _ in res)
 			template = '%%-%ds : %%s' % (tlen,)
-			return '\n'.join(fmt_caption(*item) for item in res)
+			return '\n'.join(fmt_caption(*item, indent=tlen + 3) for item in res)
 		else:
 			return '\n'.join(res)
 	joblist = JobList(Job(j, m) for m, j in res['joblist'])
 	if entry is not None:
 		return joblist.get(entry, '')
 	if res['deps']:
 		deps = sorted(
 			('%s/%s' % (k, v['timestamp'],), v['caption'],)
 			for k, v in res['deps'].items()
 		)
 		if len(deps) > 1:
 			plen = max(len(path) for path, _ in deps)
 			template = '%%-%ds : %%s' % (plen,)
-			deps = '\n           '.join(fmt_caption(*dep) for dep in deps)
+			deps = '\n           '.join(fmt_caption(*dep, indent=11 + plen) for dep in deps)
 		else:
 			template = '%s : %s'
-			deps = fmt_caption(*deps[0])
+			deps = fmt_caption(*deps[0], indent=11 + len(deps[0][0]))
 	else:
 		deps = ''
 	return "timestamp: %s\ncaption  : %s\ndeps     : %s\n%s" % (
 		res['timestamp'],
-		res['caption'],
+		fix_caption(res['caption'], 8),
 		deps,
 		joblist.pretty,
 	)
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/shell/workdir.py` & `accelerator-2023.7.18.dev1/accelerator/shell/workdir.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ############################################################################
 #                                                                          #
-# Copyright (c) 2020-2022 Carl Drougge                                     #
+# Copyright (c) 2020-2023 Carl Drougge                                     #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
 #                                                                          #
@@ -40,15 +40,17 @@
 			setup = load_setup(jid)
 			data.method = setup.method
 			if 'exectime' in setup:
 				data.totaltime = setup.exectime.total
 		except Exception:
 			pass
 	if isinstance(data.totaltime, (float, int)):
-		data.totaltime = fmttime(data.totaltime)
+		data.humantime = fmttime(data.totaltime)
+	else:
+		data.humantime = ''
 	if data.totaltime is None:
 		data.klass = 'unfinished'
 	elif data.current:
 		data.klass = 'current'
 	else:
 		data.klass = 'old'
 	if not data.get('path'):
@@ -59,15 +61,15 @@
 	return data
 
 def show_job(args, known, jid, as_latest=False):
 	data = job_data(known, jid, args.full_path)
 	path = data.path
 	if as_latest:
 		path = path.rsplit('-', 1)[0] + '-LATEST'
-	print('\t'.join((path, data.klass, data.method, data.totaltime or '')))
+	print('\t'.join((path, data.klass, data.method, data.humantime)))
 
 def workdir_jids(cfg, name):
 	jidlist = []
 	for jid in os.listdir(cfg.workdirs[name]):
 		if '-' in jid:
 			wd, num = jid.rsplit('-', 1)
 			if wd == name and num.isdigit():
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/_generated_csvimport.c` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/_generated_csvimport.c`

 * *Files 5% similar despite different names*

```diff
@@ -169,32 +169,45 @@
 #define FLUSH_WRITES(i) do { \
 	if (slicebuf_lens[i]) { \
 		err1(writeall(outfds[i], slicebufs[i], slicebuf_lens[i])); \
 		slicebuf_lens[i] = 0; \
 	} \
 } while(0)
 
-// smallest int32
-#define LABELS_DONE_MARKER -2147483648
+struct __attribute__ ((__packed__)) line_data {
+	uint64_t lineno;
+	int32_t  len; // negative for comments
+};
 
-static int reader(const char *fn, const int slices, uint64_t skip_lines, const int skip_empty_lines, const int outfds[], int labels_fd, int status_fd, const int comment_char, const int lf_char)
+static int reader(const char *fn, const int slices, uint64_t skip_lines, const int skip_empty_lines, const int outfds[], int labels_fd, int label_lines, int status_fd, const int comment_char, const int lf_char)
 {
 	int res = 1;
-	int sliceno = 0;
+	int normal_sliceno = 0;
+	int comment_sliceno = 0;
+	int sliceno;
+	int *sliceno_ptr;
 	pthread_t thread;
 	read_fh = 0;
 	char *slicebufs[slices];
 	int32_t slicebuf_lens[slices];
 	const int rl_lf_char = (lf_char == 256 ? '\n' : lf_char);
 	uint64_t linecnt = 0;
 	uint64_t comments_before_labels = 0;
 	uint64_t comments_capacity = 0;
 	char **comments = 0;
 	int32_t *comment_lens = 0;
 
+	if (sizeof(struct line_data) != 12) {
+		// errors on stderr get propagated to an exception, but unfortunately
+		// this doesn't work before the labels have been read.
+		FILE *err_fd = (labels_fd == -1 ? stderr : stdout);
+		fprintf(err_fd, "struct line_data should be 12 bytes, not %ld bytes. What happened?\n", (long) sizeof(struct line_data));
+		exit(1);
+	}
+
 	for (int i = 0; i < slices; i++) {
 		slicebufs[i] = 0;
 		slicebuf_lens[i] = 0;
 	}
 	for (int i = 0; i < slices; i++) {
 		slicebufs[i] = malloc(SLICEBUF_Z);
 		err1(!slicebufs[i]);
@@ -232,71 +245,70 @@
 			}
 		} else if (ptr[len - 1] == lf_char) {
 			len--;
 		}
 		if (skip_lines || *ptr == comment_char || (skip_empty_lines && len == 0)) {
 			if (skip_lines) skip_lines--;
 			claim_len = -len - 1;
+			sliceno_ptr = &comment_sliceno;
+			sliceno = comment_sliceno;
 		} else {
 			claim_len = len;
+			sliceno_ptr = &normal_sliceno;
+			sliceno = normal_sliceno;
 		}
+		struct line_data line_data = {linecnt, claim_len};
 		if (labels_fd == -1) {
 			if (len > SLICEBUF_THRESH) {
 				FLUSH_WRITES(sliceno);
-				memcpy(ptr - 4, &claim_len, 4);
-				err1(writeall(outfds[sliceno], ptr - 4, len + 4));
+				memcpy(ptr - sizeof(line_data), &line_data, sizeof(line_data));
+				err1(writeall(outfds[sliceno], ptr - sizeof(line_data), len + sizeof(line_data)));
 			} else {
-				if (slicebuf_lens[sliceno] + len + 4 > SLICEBUF_Z) {
+				if (slicebuf_lens[sliceno] + len + sizeof(line_data) > SLICEBUF_Z) {
 					FLUSH_WRITES(sliceno);
 				}
 				char *sptr = slicebufs[sliceno] + slicebuf_lens[sliceno];
-				memcpy(sptr, &claim_len, 4);
-				memcpy(sptr + 4, ptr, len);
-				slicebuf_lens[sliceno] += len + 4;
+				memcpy(sptr, &line_data, sizeof(line_data));
+				memcpy(sptr + sizeof(line_data), ptr, len);
+				slicebuf_lens[sliceno] += len + sizeof(line_data);
 			}
-			sliceno = (sliceno + 1) % slices;
+			*sliceno_ptr = (*sliceno_ptr + 1) % slices;
 		} else if (claim_len < 0) {
 			// No writers yet, so trying to write to the outfd might block forever.
-			const int32_t tmp_len = len + 4;
+			const int32_t tmp_len = len + sizeof(line_data);
 			char *tmp = malloc(tmp_len);
 			err1(!tmp);
-			memcpy(tmp, &claim_len, 4);
-			memcpy(tmp + 4, ptr, len);
+			memcpy(tmp, &line_data, sizeof(line_data));
+			memcpy(tmp + sizeof(line_data), ptr, len);
 			if (comments_before_labels == comments_capacity) {
 				comments_capacity = (comments_capacity + 10) * 2;
 				comments = realloc(comments, comments_capacity * sizeof(*comments));
 				err1(!comments);
 				comment_lens = realloc(comment_lens, comments_capacity * sizeof(*comment_lens));
 				err1(!comment_lens);
 			}
 			comments[comments_before_labels] = tmp;
 			comment_lens[comments_before_labels] = tmp_len;
 			comments_before_labels++;
 		} else {
-			// Only happens once anyway, so no need to optimize
-			err1(writeall(labels_fd, &len, 4));
-			err1(writeall(labels_fd, ptr, len));
+			memcpy(ptr - sizeof(line_data), &line_data, sizeof(line_data));
+			err1(writeall(labels_fd, ptr - sizeof(line_data), len + sizeof(line_data)));
+			if (--label_lines) continue;
 			close(labels_fd);
 			labels_fd = -1;
 			// Presumably there are not all that many of these, so one write each it is.
 			if (comments_before_labels) {
 				for (uint64_t i = 0; i < comments_before_labels; i++) {
-					err1(writeall(outfds[sliceno], comments[i], comment_lens[i]));
-					sliceno = (sliceno + 1) % slices;
+					err1(writeall(outfds[comment_sliceno], comments[i], comment_lens[i]));
 					free(comments[i]);
+					comment_sliceno = (comment_sliceno + 1) % slices;
 				}
 				free(comments);
 				free(comment_lens);
 			}
-			// Let all slices know the labels are done so they can add 1 to lineno.
-			const int32_t labels_done_marker = LABELS_DONE_MARKER;
-			for (int i = 0; i < slices; i++) {
-				memcpy(slicebufs[i], &labels_done_marker, 4);
-				slicebuf_lens[i] = 4;
-			}
 		}
 	}
 	for (int i = 0; i < slices; i++) {
 		FLUSH_WRITES(i);
 	}
 	res = 0;
 err:
@@ -387,55 +399,52 @@
 		// For storing unquoted fields (extra room for a short length)
 		qbuf = malloc(BIG_Z + 1);
 		err1(!qbuf);
 		qbuf++; // Room for a short length before
 	}
 	int eof = 0;
 	int32_t len;
-	uint64_t lineno = sliceno + 1;
+	uint64_t lineno;
 	int field;
 	int skip_line = 0;
 	char *bufptr;
+	struct line_data line_data;
 	// Do this first so we can skip opening output files if we are empty.
-	if (bufread(fd, buf, 4, &eof, &bufptr)) {
+	if (bufread(fd, buf, sizeof(line_data), &eof, &bufptr)) {
 		if (eof) goto done;
 		goto err;
 	}
 	for (int i = 0; i < full_field_count; i++) {
 		if (out_fns[i]) {
 			outfh[i] = gzopen(out_fns[i], gzip_mode);
 			err1(!outfh[i]);
 		}
 	}
 	goto buf_prefilled;
 keep_going:
 	while (1) {
-		if (bufread(fd, buf, 4, &eof, &bufptr)) {
+		if (bufread(fd, buf, sizeof(line_data), &eof, &bufptr)) {
 			if (eof) break;
 			goto err;
 		}
 buf_prefilled:
-		memcpy(&len, bufptr, 4);
+		memcpy(&line_data, bufptr, sizeof(line_data));
+		lineno = line_data.lineno;
+		len = line_data.len;
 		if (len < 0) {
-			if (len == LABELS_DONE_MARKER) {
-				// labels are done, so we are now offset one line
-				lineno++;
-				continue;
-			}
 			len = -(len + 1);
 			skip_line = 1;
 		}
 		err1(bufread(fd, buf, len, &eof, &bufptr));
 		if (skip_line) {
 			minmax_lineno(7);
 			err1(gzwrite(outfh[real_field_count + 2], &lineno, 8) != 8);
 			err1(field_write(outfh[real_field_count + 3], bufptr, len));
 			r_num[2]++;
 			skip_line = 0;
-			lineno += slices;
 			continue;
 		}
 		int32_t pos = 0;
 		int32_t qpos = 0;
 		field = 0;
 		while (pos < len) {
 			int last = 0;
@@ -527,15 +536,18 @@
 						}
 						badline_reported = 1;
 						goto bad_line;
 					}
 				}
 			}
 		}
-		if (!parsing_labels) {
+		if (parsing_labels) {
+			// Write None after each line
+			err1(gzwrite(outfh[field], "\xff\x00\x00\x00\x00", 5) != 5);
+		} else {
 			if (field == real_field_count - 1) {
 				// The last field was empty (we can't reach here if it was totally missing)
 				field_lens[field] = 0;
 				field_ptrs[field] = bufptr + len;
 				field++;
 			}
 			if (field != real_field_count) goto bad_line; // Happens if the line is empty
@@ -546,15 +558,14 @@
 			}
 			if (save_lineno) {
 				minmax_lineno(3);
 				err1(gzwrite(outfh[real_field_count + 4], &lineno, 8) != 8);
 			}
 		}
 		num++;
-		lineno += slices;
 	}
 done:
 	*r_num = num;
 	res = 0;
 err:
 	if (res && errno) perror("import_slice");
 	for (int i = 0; i < full_field_count; i++) {
@@ -575,15 +586,14 @@
 	r_num[1]++;
 	if (allow_bad) {
 		if (outfh[real_field_count]) {
 			minmax_lineno(5);
 			err1(gzwrite(outfh[real_field_count], &lineno, 8) != 8);
 			err1(field_write(outfh[real_field_count + 1], bufptr, len));
 		}
-		lineno += slices;
 		goto keep_going;
 	} else {
 		goto err;
 	}
 }
 
 // This is easier than using a type of known signedness above.
@@ -598,24 +608,26 @@
 	const char *fn;
 	int slices;
 	PY_LONG_LONG skip_lines;
 	int skip_empty_lines;
 	PyObject *o_outfds;
 	int *outfds = 0;
 	int labels_fd;
+	int label_lines;
 	int status_fd;
 	int comment_char;
 	int lf_char;
-	if (!PyArg_ParseTuple(args, "etiLiOiiii",
+	if (!PyArg_ParseTuple(args, "etiLiOiiiii",
 		DEFAULT_ENCODING, &fn,
 		&slices,
 		&skip_lines,
 		&skip_empty_lines,
 		&o_outfds,
 		&labels_fd,
+		&label_lines,
 		&status_fd,
 		&comment_char,
 		&lf_char
 	)) {
 		return 0;
 	}
 	err1(!PyList_Check(o_outfds));
@@ -626,15 +638,15 @@
 		PyObject *tmp = PyList_GET_ITEM(o_outfds, i);
 		outfds[i] = PyLong_AsLong(tmp);
 		if (PyErr_Occurred()) {
 			free(outfds);
 			return 0;
 		}
 	}
-	fail = reader(fn, slices, skip_lines, skip_empty_lines, outfds, labels_fd, status_fd, comment_char, lf_char);
+	fail = reader(fn, slices, skip_lines, skip_empty_lines, outfds, labels_fd, label_lines, status_fd, comment_char, lf_char);
 	fflush(stderr);
 err:
 	if (outfds) free(outfds);
 	if (fail) Py_RETURN_TRUE;
 	Py_RETURN_FALSE;
 }
 
@@ -698,15 +710,15 @@
 static PyObject *py_char2int(PyObject *dummy, PyObject *o_charstr)
 {
 	const char *charstr;
 	if (str_or_0(o_charstr, &charstr)) return 0;
 	if (!charstr) Py_RETURN_NONE;
 	return PyLong_FromLong(char2int(*charstr));
 }
-static char source_hash[] = "98a0352726b31cfda8996c61d7c89a6331c11724";
+static char source_hash[] = "14b834ce2c49dca2ddf9f61853cb5dcbc9967d81";
 
 static PyMethodDef module_methods[] = {
 	{"set_null", py_set_null, METH_O, 0},
 	{"reader", py_reader, METH_VARARGS, 0},
 	{"import_slice", py_import_slice, METH_VARARGS, 0},
 	{"char2int", py_char2int, METH_O, 0},
 	{NULL, NULL, 0, NULL}
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/_generated_dataset_type.c` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/_generated_dataset_type.c`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/a_csvexport.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/a_csvexport.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/a_csvimport.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/a_csvimport.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ############################################################################
 #                                                                          #
-# Copyright (c) 2019-2022 Carl Drougge                                     #
+# Copyright (c) 2019-2023 Carl Drougge                                     #
 # Modifications copyright (c) 2020 Anders Berkeman                         #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
@@ -57,16 +57,17 @@
 
 options = dict(
 	filename          = OptionString,
 	separator         = ',',   # Single iso-8859-1 character or empty for a single field.
 	comment           = '',    # Single iso-8859-1 character or empty, lines beginning with this character are ignored.
 	newline           = '',    # Empty means \n or \r\n, or you can specify any single iso-8859-1 character.
 	quotes            = '',    # Empty or False means no quotes, True means both ' and ", any other character means itself.
-	labelsonfirstline = True,
-	labels            = [],    # Mandatory if not labelsonfirstline, always sets labels if set.
+	label_lines       = int,   # Number of lines with labels on them. Multi-line labels are space-separated.
+	                           # Defaults to 1 unless labels is set.
+	labels            = [],    # Mandatory if label_lines = 0, always sets labels if set.
 	strip_labels      = False, # Do .strip() on all labels (happens before rename).
 	rename            = {},    # Labels to replace (if they are in the file) (happens before discard).
 	discard           = set(), # Labels to not include (if they are in the file)
 	lineno_label      = "",    # Label of column to store line number in (not stored if empty).
 	allow_bad         = False, # Still succeed if some lines have too few/many fields or bad quotes
 	                           # creates a "bad" dataset containing lineno and data from the bad lines.
 	allow_extra_empty = False, # Still consider a line good if it has extra empty fields at the end.
@@ -90,15 +91,15 @@
 	while True:
 		update('{0:n} lines read'.format(count))
 		data = os.read(status_fd, 8)
 		if not data:
 			break
 		count = struct.unpack("=Q", data)[0]
 
-def reader_process(slices, filename, write_fds, labels_fd, success_fd, status_fd, comment_char, lf_char):
+def reader_process(slices, filename, write_fds, labels_fd, success_fd, status_fd, comment_char, lf_char, label_lines):
 	# Terrible hack - try to close FDs we didn't want in this process.
 	# (This is important, if the main process dies this won't be
 	# detected if we still have these open.)
 	keep_fds = set(write_fds)
 	keep_fds.add(labels_fd)
 	keep_fds.add(success_fd)
 	keep_fds.add(status_fd)
@@ -109,15 +110,15 @@
 				os.close(fd)
 			except OSError:
 				pass
 	setproctitle("reader")
 	os.dup2(success_fd, 2) # reader writes errors to stderr
 	os.close(success_fd)
 	success_fd = 2
-	res = cstuff.backend.reader(filename.encode("utf-8"), slices, options.skip_lines, options.skip_empty_lines, write_fds, labels_fd, status_fd, comment_char, lf_char)
+	res = cstuff.backend.reader(filename.encode("utf-8"), slices, options.skip_lines, options.skip_empty_lines, write_fds, labels_fd, label_lines, status_fd, comment_char, lf_char)
 	if not res:
 		os.write(success_fd, b"\0")
 	os.close(success_fd)
 
 def char2int(name, empty_value, specials="empty"):
 	char = options.get(name)
 	if not char:
@@ -169,42 +170,56 @@
 	# To get a more useful error if the file doesn't exist or similar
 	open(filename, 'rb').close()
 
 	fds = [os.pipe() for _ in range(slices)]
 	read_fds = [t[0] for t in fds]
 	write_fds = [t[1] for t in fds]
 
-	if options.labelsonfirstline:
+	label_lines = options.label_lines
+	if label_lines is None:
+		label_lines = 0 if options.labels else 1
+
+	if label_lines:
+		assert label_lines > 0
 		labels_rfd, labels_wfd = os.pipe()
 	else:
 		labels_wfd = -1
 	success_fh = open("reader.success", "wb+")
 	status_rfd, status_wfd = os.pipe()
 
-	p = Process(target=reader_process, name="reader", args=(slices, filename, write_fds, labels_wfd, success_fh.fileno(), status_wfd, comment_char, lf_char))
+	p = Process(target=reader_process, name="reader", args=(slices, filename, write_fds, labels_wfd, success_fh.fileno(), status_wfd, comment_char, lf_char, label_lines))
 	p.start()
 	for fd in write_fds:
 		os.close(fd)
 	os.close(status_wfd)
 
-	if options.labelsonfirstline:
+	if label_lines:
 		os.close(labels_wfd)
 		# re-use import logic
 		out_fns = ["labels"]
 		r_num = cstuff.mk_uint64(9)
 		try:
 			import_slice("c backend failed in label parsing", labels_rfd, -1, -1, -1, out_fns, b"wb1", separator, r_num, quote_char, lf_char, 0, 0)
 		finally:
 			os.close(labels_rfd)
+		labels_from_file = []
 		if os.path.exists("labels"):
+			# This is one item per field with lines separated with None
 			with typed_reader("bytes")("labels") as fh:
-				labels_from_file = [lab.decode("utf-8", "backslashreplace") for lab in fh]
+				labels = list(fh)
+			while None in labels:
+				ix = labels.index(None)
+				labels_from_file.append([lab.decode("utf-8", "backslashreplace") for lab in labels[:ix]])
+				labels = labels[ix + 1:]
+			assert labels == []
+			assert len(labels_from_file) == r_num[0]
+			if len(set(len(labs) for labs in labels_from_file)) != 1:
+				raise Exception("Not all label lines had the same number of fields")
+			labels_from_file = [' '.join(labs) for labs in zip(*labels_from_file)]
 			os.unlink("labels")
-		else:
-			labels_from_file = []
 	else:
 		labels_from_file = None
 
 	labels = options.labels or labels_from_file
 	if options.allow_extra_empty:
 		while labels and labels[-1] == '':
 			labels.pop()
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/a_csvimport_zip.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/a_csvimport_zip.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_checksum.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_checksum.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_checksum_chain.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_checksum_chain.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_concat.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_concat.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_fanout.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_fanout.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_fanout_collect.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_fanout_collect.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_filter_columns.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_filter_columns.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_hashpart.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_hashpart.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_merge.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_merge.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_rename_columns.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_rename_columns.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_sort.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_sort.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_type.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_type.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/a_dataset_unroundrobin.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/a_dataset_unroundrobin.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/c_backend_support.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/c_backend_support.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/csvimport.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/csvimport.py`

 * *Files 4% similar despite different names*

```diff
@@ -171,32 +171,45 @@
 #define FLUSH_WRITES(i) do { \
 	if (slicebuf_lens[i]) { \
 		err1(writeall(outfds[i], slicebufs[i], slicebuf_lens[i])); \
 		slicebuf_lens[i] = 0; \
 	} \
 } while(0)
 
-// smallest int32
-#define LABELS_DONE_MARKER -2147483648
+struct __attribute__ ((__packed__)) line_data {
+	uint64_t lineno;
+	int32_t  len; // negative for comments
+};
 
-static int reader(const char *fn, const int slices, uint64_t skip_lines, const int skip_empty_lines, const int outfds[], int labels_fd, int status_fd, const int comment_char, const int lf_char)
+static int reader(const char *fn, const int slices, uint64_t skip_lines, const int skip_empty_lines, const int outfds[], int labels_fd, int label_lines, int status_fd, const int comment_char, const int lf_char)
 {
 	int res = 1;
-	int sliceno = 0;
+	int normal_sliceno = 0;
+	int comment_sliceno = 0;
+	int sliceno;
+	int *sliceno_ptr;
 	pthread_t thread;
 	read_fh = 0;
 	char *slicebufs[slices];
 	int32_t slicebuf_lens[slices];
 	const int rl_lf_char = (lf_char == 256 ? '\n' : lf_char);
 	uint64_t linecnt = 0;
 	uint64_t comments_before_labels = 0;
 	uint64_t comments_capacity = 0;
 	char **comments = 0;
 	int32_t *comment_lens = 0;
 
+	if (sizeof(struct line_data) != 12) {
+		// errors on stderr get propagated to an exception, but unfortunately
+		// this doesn't work before the labels have been read.
+		FILE *err_fd = (labels_fd == -1 ? stderr : stdout);
+		fprintf(err_fd, "struct line_data should be 12 bytes, not %ld bytes. What happened?\n", (long) sizeof(struct line_data));
+		exit(1);
+	}
+
 	for (int i = 0; i < slices; i++) {
 		slicebufs[i] = 0;
 		slicebuf_lens[i] = 0;
 	}
 	for (int i = 0; i < slices; i++) {
 		slicebufs[i] = malloc(SLICEBUF_Z);
 		err1(!slicebufs[i]);
@@ -234,71 +247,70 @@
 			}
 		} else if (ptr[len - 1] == lf_char) {
 			len--;
 		}
 		if (skip_lines || *ptr == comment_char || (skip_empty_lines && len == 0)) {
 			if (skip_lines) skip_lines--;
 			claim_len = -len - 1;
+			sliceno_ptr = &comment_sliceno;
+			sliceno = comment_sliceno;
 		} else {
 			claim_len = len;
+			sliceno_ptr = &normal_sliceno;
+			sliceno = normal_sliceno;
 		}
+		struct line_data line_data = {linecnt, claim_len};
 		if (labels_fd == -1) {
 			if (len > SLICEBUF_THRESH) {
 				FLUSH_WRITES(sliceno);
-				memcpy(ptr - 4, &claim_len, 4);
-				err1(writeall(outfds[sliceno], ptr - 4, len + 4));
+				memcpy(ptr - sizeof(line_data), &line_data, sizeof(line_data));
+				err1(writeall(outfds[sliceno], ptr - sizeof(line_data), len + sizeof(line_data)));
 			} else {
-				if (slicebuf_lens[sliceno] + len + 4 > SLICEBUF_Z) {
+				if (slicebuf_lens[sliceno] + len + sizeof(line_data) > SLICEBUF_Z) {
 					FLUSH_WRITES(sliceno);
 				}
 				char *sptr = slicebufs[sliceno] + slicebuf_lens[sliceno];
-				memcpy(sptr, &claim_len, 4);
-				memcpy(sptr + 4, ptr, len);
-				slicebuf_lens[sliceno] += len + 4;
+				memcpy(sptr, &line_data, sizeof(line_data));
+				memcpy(sptr + sizeof(line_data), ptr, len);
+				slicebuf_lens[sliceno] += len + sizeof(line_data);
 			}
-			sliceno = (sliceno + 1) % slices;
+			*sliceno_ptr = (*sliceno_ptr + 1) % slices;
 		} else if (claim_len < 0) {
 			// No writers yet, so trying to write to the outfd might block forever.
-			const int32_t tmp_len = len + 4;
+			const int32_t tmp_len = len + sizeof(line_data);
 			char *tmp = malloc(tmp_len);
 			err1(!tmp);
-			memcpy(tmp, &claim_len, 4);
-			memcpy(tmp + 4, ptr, len);
+			memcpy(tmp, &line_data, sizeof(line_data));
+			memcpy(tmp + sizeof(line_data), ptr, len);
 			if (comments_before_labels == comments_capacity) {
 				comments_capacity = (comments_capacity + 10) * 2;
 				comments = realloc(comments, comments_capacity * sizeof(*comments));
 				err1(!comments);
 				comment_lens = realloc(comment_lens, comments_capacity * sizeof(*comment_lens));
 				err1(!comment_lens);
 			}
 			comments[comments_before_labels] = tmp;
 			comment_lens[comments_before_labels] = tmp_len;
 			comments_before_labels++;
 		} else {
-			// Only happens once anyway, so no need to optimize
-			err1(writeall(labels_fd, &len, 4));
-			err1(writeall(labels_fd, ptr, len));
+			memcpy(ptr - sizeof(line_data), &line_data, sizeof(line_data));
+			err1(writeall(labels_fd, ptr - sizeof(line_data), len + sizeof(line_data)));
+			if (--label_lines) continue;
 			close(labels_fd);
 			labels_fd = -1;
 			// Presumably there are not all that many of these, so one write each it is.
 			if (comments_before_labels) {
 				for (uint64_t i = 0; i < comments_before_labels; i++) {
-					err1(writeall(outfds[sliceno], comments[i], comment_lens[i]));
-					sliceno = (sliceno + 1) % slices;
+					err1(writeall(outfds[comment_sliceno], comments[i], comment_lens[i]));
 					free(comments[i]);
+					comment_sliceno = (comment_sliceno + 1) % slices;
 				}
 				free(comments);
 				free(comment_lens);
 			}
-			// Let all slices know the labels are done so they can add 1 to lineno.
-			const int32_t labels_done_marker = LABELS_DONE_MARKER;
-			for (int i = 0; i < slices; i++) {
-				memcpy(slicebufs[i], &labels_done_marker, 4);
-				slicebuf_lens[i] = 4;
-			}
 		}
 	}
 	for (int i = 0; i < slices; i++) {
 		FLUSH_WRITES(i);
 	}
 	res = 0;
 err:
@@ -389,55 +401,52 @@
 		// For storing unquoted fields (extra room for a short length)
 		qbuf = malloc(BIG_Z + 1);
 		err1(!qbuf);
 		qbuf++; // Room for a short length before
 	}
 	int eof = 0;
 	int32_t len;
-	uint64_t lineno = sliceno + 1;
+	uint64_t lineno;
 	int field;
 	int skip_line = 0;
 	char *bufptr;
+	struct line_data line_data;
 	// Do this first so we can skip opening output files if we are empty.
-	if (bufread(fd, buf, 4, &eof, &bufptr)) {
+	if (bufread(fd, buf, sizeof(line_data), &eof, &bufptr)) {
 		if (eof) goto done;
 		goto err;
 	}
 	for (int i = 0; i < full_field_count; i++) {
 		if (out_fns[i]) {
 			outfh[i] = gzopen(out_fns[i], gzip_mode);
 			err1(!outfh[i]);
 		}
 	}
 	goto buf_prefilled;
 keep_going:
 	while (1) {
-		if (bufread(fd, buf, 4, &eof, &bufptr)) {
+		if (bufread(fd, buf, sizeof(line_data), &eof, &bufptr)) {
 			if (eof) break;
 			goto err;
 		}
 buf_prefilled:
-		memcpy(&len, bufptr, 4);
+		memcpy(&line_data, bufptr, sizeof(line_data));
+		lineno = line_data.lineno;
+		len = line_data.len;
 		if (len < 0) {
-			if (len == LABELS_DONE_MARKER) {
-				// labels are done, so we are now offset one line
-				lineno++;
-				continue;
-			}
 			len = -(len + 1);
 			skip_line = 1;
 		}
 		err1(bufread(fd, buf, len, &eof, &bufptr));
 		if (skip_line) {
 			minmax_lineno(7);
 			err1(gzwrite(outfh[real_field_count + 2], &lineno, 8) != 8);
 			err1(field_write(outfh[real_field_count + 3], bufptr, len));
 			r_num[2]++;
 			skip_line = 0;
-			lineno += slices;
 			continue;
 		}
 		int32_t pos = 0;
 		int32_t qpos = 0;
 		field = 0;
 		while (pos < len) {
 			int last = 0;
@@ -529,15 +538,18 @@
 						}
 						badline_reported = 1;
 						goto bad_line;
 					}
 				}
 			}
 		}
-		if (!parsing_labels) {
+		if (parsing_labels) {
+			// Write None after each line
+			err1(gzwrite(outfh[field], "\xff\x00\x00\x00\x00", 5) != 5);
+		} else {
 			if (field == real_field_count - 1) {
 				// The last field was empty (we can't reach here if it was totally missing)
 				field_lens[field] = 0;
 				field_ptrs[field] = bufptr + len;
 				field++;
 			}
 			if (field != real_field_count) goto bad_line; // Happens if the line is empty
@@ -548,15 +560,14 @@
 			}
 			if (save_lineno) {
 				minmax_lineno(3);
 				err1(gzwrite(outfh[real_field_count + 4], &lineno, 8) != 8);
 			}
 		}
 		num++;
-		lineno += slices;
 	}
 done:
 	*r_num = num;
 	res = 0;
 err:
 	if (res && errno) perror("import_slice");
 	for (int i = 0; i < full_field_count; i++) {
@@ -577,15 +588,14 @@
 	r_num[1]++;
 	if (allow_bad) {
 		if (outfh[real_field_count]) {
 			minmax_lineno(5);
 			err1(gzwrite(outfh[real_field_count], &lineno, 8) != 8);
 			err1(field_write(outfh[real_field_count + 1], bufptr, len));
 		}
-		lineno += slices;
 		goto keep_going;
 	} else {
 		goto err;
 	}
 }
 
 // This is easier than using a type of known signedness above.
@@ -603,24 +613,26 @@
 	const char *fn;
 	int slices;
 	PY_LONG_LONG skip_lines;
 	int skip_empty_lines;
 	PyObject *o_outfds;
 	int *outfds = 0;
 	int labels_fd;
+	int label_lines;
 	int status_fd;
 	int comment_char;
 	int lf_char;
-	if (!PyArg_ParseTuple(args, "etiLiOiiii",
+	if (!PyArg_ParseTuple(args, "etiLiOiiiii",
 		DEFAULT_ENCODING, &fn,
 		&slices,
 		&skip_lines,
 		&skip_empty_lines,
 		&o_outfds,
 		&labels_fd,
+		&label_lines,
 		&status_fd,
 		&comment_char,
 		&lf_char
 	)) {
 		return 0;
 	}
 	err1(!PyList_Check(o_outfds));
@@ -631,15 +643,15 @@
 		PyObject *tmp = PyList_GET_ITEM(o_outfds, i);
 		outfds[i] = PyLong_AsLong(tmp);
 		if (PyErr_Occurred()) {
 			free(outfds);
 			return 0;
 		}
 	}
-	fail = reader(fn, slices, skip_lines, skip_empty_lines, outfds, labels_fd, status_fd, comment_char, lf_char);
+	fail = reader(fn, slices, skip_lines, skip_empty_lines, outfds, labels_fd, label_lines, status_fd, comment_char, lf_char);
 	fflush(stderr);
 err:
 	if (outfds) free(outfds);
 	if (fail) Py_RETURN_TRUE;
 	Py_RETURN_FALSE;
 }
 
@@ -716,12 +728,12 @@
 ]
 
 
 c_module_code, c_module_hash = c_backend_support.make_source('csvimport', all_c_functions, [], extra_c_functions, extra_method_defs, None)
 
 def init():
 	protos = [
-		'static int reader(const char *fn, const int slices, uint64_t skip_lines, const int skip_empty_lines, const int outfds[], int labels_fd, int status_fd, const int comment_char, const int lf_char);',
+		'static int reader(const char *fn, const int slices, uint64_t skip_lines, const int skip_empty_lines, const int outfds[], int labels_fd, int label_lines, int status_fd, const int comment_char, const int lf_char);',
 		'static int import_slice(const int fd, const int sliceno, const int slices, const int field_count, const char *out_fns[], const char *gzip_mode, const int separator, uint64_t *r_num, const int quote_char, const int lf_char, const int allow_bad, const int allow_extra_empty);',
 		'static int char2int(const char c);',
 	]
 	return c_backend_support.init('csvimport', c_module_hash, [], protos, all_c_functions)
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/standard_methods/dataset_type.py` & `accelerator-2023.7.18.dev1/accelerator/standard_methods/dataset_type.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/statmsg.py` & `accelerator-2023.7.18.dev1/accelerator/statmsg.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/subjobs.py` & `accelerator-2023.7.18.dev1/accelerator/subjobs.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_analysis_died.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_analysis_died.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_arg_lists.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_arg_lists.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_build_kws.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_build_kws.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_compare_datasets.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_compare_datasets.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvexport_all_coltypes.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvexport_all_coltypes.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvexport_chains.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvexport_chains.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvexport_naming.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvexport_naming.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvexport_quoting.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvexport_quoting.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvexport_separators.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvexport_separators.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvimport_corner_cases.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvimport_corner_cases.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ############################################################################
 #                                                                          #
-# Copyright (c) 2019-2022 Carl Drougge                                     #
+# Copyright (c) 2019-2023 Carl Drougge                                     #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
 #                                                                          #
@@ -48,29 +48,30 @@
 			else:
 				d[ix] = data
 			ix = str(ix).encode("ascii")
 			fh.write(ix + b"," + data + b"," + data + b"\n")
 	options.update(
 		filename=job.filename(filename),
 		allow_bad=bool(bad_lines),
-		labelsonfirstline=False,
 		labels=["ix", "0", "1"],
 	)
 	verify_ds(options, d, d_bad, {}, filename)
 
-def verify_ds(options, d, d_bad, d_skipped, filename):
+def verify_ds(options, d, d_bad, d_skipped, filename, d_columns=None):
 	jid = subjobs.build("csvimport", options=options)
 	ds = Dataset(jid)
-	expected_columns = {"ix", "0", "1"}
+	if not d_columns:
+		d_columns = ["ix", "0", "1"]
+	expected_columns = set(d_columns)
 	if options.get("lineno_label"):
 		expected_columns.add(options["lineno_label"])
-		lineno_want = {ix: int(ix) for ix in ds.iterate(None, "ix")}
+		lineno_want = {ix: int(ix) for ix in ds.iterate(None, d_columns[0])}
 	assert set(ds.columns) == expected_columns
 	# Order varies depending on slice count, so we use a dict {ix: data}
-	for ix, a, b in ds.iterate(None, ["ix", "0", "1"]):
+	for ix, a, b in ds.iterate(None, d_columns):
 		try:
 			ix = int(ix)
 		except ValueError:
 			# We have a few non-numeric ones
 			pass
 		assert ix in d, "Bad index %r in %r (%s)" % (ix, filename, jid,)
 		assert a == b == d[ix], "Wrong data for line %r in %r (%s)" % (ix, filename, jid,)
@@ -91,15 +92,15 @@
 			assert ix in d_skipped, "Bad skipped_lineno %d in %r (%s/skipped) %r" % (ix, filename, jid, data,)
 			assert data == d_skipped[ix], "Wrong saved skipped line %d in %r (%s/skipped).\nWanted %r.\nGot    %r." % (ix, filename, jid, d_skipped[ix], data,)
 			del d_skipped[ix]
 		verify_minmax(skipped_ds, "lineno")
 	assert not d_skipped, "Not all bad lines returned from %r (%s), %r missing" % (filename, jid, set(d_skipped.keys()),)
 
 	if options.get("lineno_label"):
-		lineno_got = dict(ds.iterate(None, ["ix", options.get("lineno_label")]))
+		lineno_got = dict(ds.iterate(None, [d_columns[0], options.get("lineno_label")]))
 		assert lineno_got == lineno_want, "%r != %r" % (lineno_got, lineno_want,)
 		verify_minmax(ds, options["lineno_label"])
 
 def verify_minmax(ds, colname):
 	data = list(ds.iterate(None, colname))
 	minmax_want = (min(data) , max(data),) if data else (None, None,)
 	col = ds.columns[colname]
@@ -158,30 +159,29 @@
 					write(byteline(splitpoint, 256, nl, q))
 			try:
 				jid = subjobs.build("csvimport", options=dict(
 					filename=job.filename(filename),
 					quotes=q_b.decode("iso-8859-1"),
 					newline=nl_b.decode("iso-8859-1"),
 					separator='',
-					labelsonfirstline=False,
 					labels=["data"],
 				))
 			except JobError:
 				raise Exception("Importing %r failed" % (filename,))
 			got_c = Counter(Dataset(jid).iterate(None, "data"))
 			assert got_c == wrote_c, "Importing %r (%s) gave wrong contents" % (filename, jid,)
 
-def check_good_file(job, name, data, d, d_bad={}, d_skipped={}, **options):
+def check_good_file(job, name, data, d, d_bad={}, d_skipped={}, d_columns=None, **options):
 	filename = name + ".txt"
 	with openx(filename) as fh:
 		fh.write(data)
 	options.update(
 		filename=job.filename(filename),
 	)
-	verify_ds(options, d, d_bad, d_skipped, filename)
+	verify_ds(options, d, d_bad, d_skipped, filename, d_columns)
 
 def synthesis(job):
 	check_good_file(job, "mixed line endings", b"ix,0,1\r\n1,a,a\n2,b,b\r\n3,c,c", {1: b"a", 2: b"b", 3: b"c"})
 	check_good_file(job, "ignored quotes", b"ix,0,1\n1,'a,'a\n2,'b','b'\n3,\"c\",\"c\"\n4,d',d'\n", {1: b"'a", 2: b"'b'", 3: b'"c"', 4: b"d'"})
 	check_good_file(job, "ignored quotes and extra fields", b"ix,0,1\n1,\"a,\"a\n2,'b,c',d\n3,d\",d\"\n", {1: b'"a', 3: b'd"'}, allow_bad=True, d_bad={3: b"2,'b,c',d"})
 	check_good_file(job, "spaces and quotes", b"ix,0,1\none,a,a\ntwo, b, b\n three,c,c\n4,\"d\"\"\",d\"\n5, 'e',\" 'e'\"\n", {b"one": b"a", b"two": b" b", b" three": b"c", 4: b'd"', 5: b" 'e'"}, quotes=True)
 	check_good_file(job, "empty fields", b"ix,0,1\n1,,''\n2,,\n3,'',\n4,\"\",", {1: b"", 2: b"", 3: b"", 4: b""}, quotes=True)
@@ -189,28 +189,30 @@
 	check_good_file(job, "discarded field", b"ix,0,no,1\n0,yes,no,yes\n1,a,'foo,bar',a", {0: b"yes", 1: b"a"}, quotes=True, discard={"no"})
 	check_good_file(job, "bad quotes", b"""ix,0,1\n1,a,a\n2,"b,"b\n\n3,'c'c','c'c'\n4,"d",'d'\n""", {1: b"a", 4: b"d"}, quotes=True, allow_bad=True, d_bad={3: b'2,"b,"b', 4: b"", 5: b"3,'c'c','c'c'"})
 	check_good_file(job, "comments", b"""# blah\nix,0,1\n1,a,a\n2,b,b\n#3,c,c\n4,#d,#d\n""", {1: b"a", 2: b"b", 4: b"#d"}, comment="#", d_skipped={1: b"# blah", 5: b"#3,c,c"})
 	check_good_file(job, "not comments", b"""ix,0,1\n1,a,a\n2,b,b\n#3,c,c\n4,#d,#d\n""", {1: b"a", 2: b"b", b"#3": b"c", 4: b"#d"})
 	check_good_file(job, "a little of everything", b""";not,1,labels\na,2,1\n;a,3,;a\n";b",4,;b\n'c,5,c'\r\n d,6,' d'\ne,7,e,\n,8,""", {4: b";b", 6: b" d", 8: b""}, allow_bad=True, rename={"a": "0", "2": "ix"}, quotes=True, comment=";", d_bad={5: b"'c,5,c'", 7: b"e,7,e,"}, d_skipped={1: b";not,1,labels", 3: b";a,3,;a"})
 	check_good_file(job, "skipped lines", b"""just some text\n\nix,0,1\n1,a,a\n2,b,b""", {1: b"a", 2: b"b"}, skip_lines=2, d_skipped={1: b"just some text", 2: b""})
 	check_good_file(job, "skipped and bad lines", b"""not data here\nnor here\nix,0,1\n1,a,a\n2,b\n3,c,c""", {1: b"a", 3: b"c"}, skip_lines=2, allow_bad=True, d_bad={5: b"2,b"}, d_skipped={1: b"not data here", 2: b"nor here"})
-	check_good_file(job, "override labels", b"""a,b,c\n0,foo,foo""", {0: b"foo"}, labels=["ix", "0", "1"])
+	check_good_file(job, "override labels", b"""a,b,c\n0,foo,foo""", {0: b"foo"}, labels=["ix", "0", "1"], label_lines=1)
 	check_good_file(job, "only labels", b"""ix,0,1""", {})
 	check_good_file(job, "empty file", b"", {}, labels=["ix", "0", "1"])
 	check_good_file(job, "empty file with lineno+skip+bad", b"", {}, labels=["ix", "0", "1"], lineno_label="num", comment="#", allow_bad=True)
 	check_good_file(job, "lineno with bad lines", b"ix,0,1\n2,a,a\n3,b\nc\n5,d,d\n6,e,e\n7\n8,g,g\n\n", {2: b"a", 5: b"d", 6: b"e", 8: b"g"}, d_bad={3: b"3,b", 4: b"c", 7: b"7", 9: b""}, allow_bad=True, lineno_label="num")
-	check_good_file(job, "lineno with skipped lines", b"a\nb\n3,c,c\n4,d,d", {3: b"c", 4: b"d"}, lineno_label="l", labels=["ix", "0", "1"], labelsonfirstline=False, skip_lines=2, d_skipped={1: b"a", 2: b"b"})
+	check_good_file(job, "lineno with skipped lines", b"a\nb\n3,c,c\n4,d,d", {3: b"c", 4: b"d"}, lineno_label="l", labels=["ix", "0", "1"], skip_lines=2, d_skipped={1: b"a", 2: b"b"})
 	check_good_file(job, "lineno with comment lines", b"ix,0,1\n2,a,a\n3,b,b\n#4,c,c\n5,d,d", {2: b"a", 3: b"b", 5: b"d"}, lineno_label="another name", comment="#", d_skipped={4: b"#4,c,c"})
 	check_good_file(job, "strip labels", b" ix , 0 , 1 \n1,a,a\n2,b ,b ", {1: b"a", 2: b"b "}, strip_labels=True)
 	check_good_file(job, "allow extra empty", b"ix,0,1,,,,\n1,a,a\n2,b,b,,\n3,,,", {1: b"a", 2: b"b", 3: b""}, allow_extra_empty=True)
 	check_good_file(job, "allow extra empty quoted", b"ix,_0_,1,,,__,\n1,a,a\n_2_,b,b,__,\n3,c,c,__", {1: b"a", 2: b"b", 3: b"c"}, allow_extra_empty=True, quotes='_')
 	check_good_file(job, "allow extra empty quoted bad", b"ix,0,1,,,'',\"\"\n1,a,a\n'2',b,b,'',\n3,c,c,\"\"\n4,d,d,'\"\n5,'',\"\",'", {1: b"a", 2: b"b", 3: b"c"}, allow_extra_empty=True, quotes=True, allow_bad=True, d_bad={5: b"4,d,d,'\"", 6: b"5,'',\"\",'"})
 	check_good_file(job, "skip empty lines", b"\nix,0,1\n\n\n1,a,a\n", {1: b"a"}, skip_empty_lines=True)
 	check_good_file(job, "skip empty lines and comments", b"\r\nix,0,1\n\n\n5,a,a\n#6,b,b\n7,c,c\n#", {5: b"a", 7: b"c"}, skip_empty_lines=True, comment="#", d_skipped={1: b"", 3: b"", 4: b"", 6: b"#6,b,b", 8: b"#"}, lineno_label="line")
 	check_good_file(job, "skip empty lines and bad", b"\n\nix,0,1\n4,a,a\n \n6,b,b\n\r\n", {4: b"a", 6: b"b"}, skip_empty_lines=True, comment="#", d_skipped={1: b"", 2: b"", 7: b""}, d_bad={5: b" "}, allow_bad=True, lineno_label="line")
+	check_good_file(job, "two label lines", b"a,b,c\nx,y,z\n3,a,a\n4,b,b\n", {3: b"a", 4: b"b"}, label_lines=2, lineno_label="line", d_columns=["a x", "b y", "c z"])
+	check_good_file(job, "three label lines with comments between", b"a,b,c\n#2,2,2\nfoo,bar,blutti\n#4,4,4\nd,e,f\n6,a,a\n#7,7,7\n8,b,b\n", {6: b"a", 8: b"b"}, label_lines=3, lineno_label="line", comment="#", d_skipped={2: b"#2,2,2", 4: b"#4,4,4", 7: b"#7,7,7"}, d_columns=["a foo d", "b bar e", "c blutti f"])
 
 	bad_lines = [
 		b"bad,bad",
 		b",",
 		b"bad,",
 		b",bad",
 		b"',',",
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvimport_separators.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvimport_separators.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_csvimport_zip.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_csvimport_zip.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ############################################################################
 #                                                                          #
-# Copyright (c) 2019-2022 Carl Drougge                                     #
+# Copyright (c) 2019-2023 Carl Drougge                                     #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
 #                                                                          #
@@ -55,15 +55,15 @@
 	for dsn, want_data in want_ds.items():
 		got_data = list(Dataset(jid, dsn).iterate(None, '0'))
 		assert got_data == want_data, "%s/%s from %s didn't contain %r, instead contained %r" % (jid, dsn, zipname, want_data, got_data)
 
 def verify_order(want_order, namemap={}, **kw):
 	opts=dict(
 		filename=g.job.filename('many files.zip'),
-		labelsonfirstline=False,
+		label_lines=0,
 		labels=['0'],
 	)
 	opts.update(kw)
 	jid = subjobs.build('csvimport_zip', options=opts)
 	want_order = list(want_order)
 	for dsn in want_order:
 		b = b'contents of ' + namemap.get(dsn, dsn).encode('ascii')
@@ -115,15 +115,15 @@
 	verify('both.zip', {'a': 'foo', 'b': 'bar'}, {'foo': list_a, 'bar': list_b})
 	verify('both.zip', {}, {'a': list_a, 'b': list_b})
 	verify('both.zip', {'a': 'foo'}, {'foo': list_a, 'default': list_a})
 	verify('both, b compressed.zip', {'a': 'foo', 'b': 'bar'}, {'foo': list_a, 'bar': list_b})
 	verify('both, b compressed.zip', {}, {'a': list_a, 'b': list_b})
 	verify('both called a.zip', {}, {'a': list_a, 'a_': list_b})
 	verify('both called a, first compressed.zip', {}, {'a': list_a, 'a_': list_b})
-	verify('many files.zip', {}, manyfiles, labelsonfirstline=False, labels=['0'])
+	verify('many files.zip', {}, manyfiles, label_lines=0, labels=['0'])
 	verify('named default.zip', {}, {'default': list_b})
 	# Use inside_filenames to test this again in a different way.
 	verify('a.zip', {'a': 'default'}, {'default': list_a})
 
 	# check all the different orders chaining can be done in
 	verify_order('BACDEFGHIJKLMOPQRSTUVWXYZ') # implicitly 'on', i.e. 'by_ziporder'
 	inside_filenames = OrderedDict([
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_callbacks.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_callbacks.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_checksum.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_checksum.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_column_names.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_column_names.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_concat.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_concat.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_empty_colname.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_empty_colname.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_fanout.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_fanout.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_filter_columns.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_filter_columns.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_in_prepare.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_in_prepare.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_merge.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_merge.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_names.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_names.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_nan.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_nan.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_overwrite.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_overwrite.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_parsing_writer.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_parsing_writer.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_range.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_range.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_rename_columns.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_rename_columns.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_roundrobin.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_roundrobin.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_slice.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_slice.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_type_chaining.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_type_chaining.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_type_corner_cases.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_type_corner_cases.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_type_hashing.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_type_hashing.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_type_minmax.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_type_minmax.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_unroundrobin.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_unroundrobin.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_dataset_unroundrobin_trigger.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_dataset_unroundrobin_trigger.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datasetwriter.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datasetwriter.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datasetwriter_copy.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datasetwriter_copy.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datasetwriter_default.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datasetwriter_default.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datasetwriter_missing_slices.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datasetwriter_missing_slices.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datasetwriter_parent.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datasetwriter_parent.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datasetwriter_parsed.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datasetwriter_parsed.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datasetwriter_verify.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datasetwriter_verify.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_datetime.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_datetime.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_finish_early.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_finish_early.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_hashlabel.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_hashlabel.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_hashpart.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_hashpart.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_jobchain.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_jobchain.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_jobwithfile.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_jobwithfile.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_json.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_json.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_number.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_number.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_optionenum.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_optionenum.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_options_dict_order.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_options_dict_order.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_options_rebuild.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_options_rebuild.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output_a.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output_a.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output_as.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output_as.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output_on_error.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output_on_error.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output_pa.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output_pa.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output_pas.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output_pas.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output_ps.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output_ps.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_output_s.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_output_s.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_rechain.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_rechain.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_selfchain.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_selfchain.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_shell_commands.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_shell_commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ############################################################################
 #                                                                          #
-# Copyright (c) 2022 Carl Drougge                                          #
+# Copyright (c) 2022-2023 Carl Drougge                                     #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
 #                                                                          #
@@ -72,14 +72,15 @@
 	os.putenv('XDG_CONFIG_HOME', job.path) # make sure we can't be messed up by config
 	os.unsetenv('CLICOLOR_FORCE')
 	chk(['-h'], want_in_help=['\ncommands:\n', '\naliases:\n'])
 	chk(['abort'], want_in_help=['--quiet'])
 	chk(['alias', 'cat'], want_in_help=['shows all aliases'], want_in_call=["grep -e ''"])
 	chk(['board-server'], want_in_help=['localhost:8520'])
 	chk(['ds', '--', ds], want_in_help=['--list'], want_in_call=['Columns:', 'this is a column'])
+	chk(['gc'], want_in_help=['--dry-run'])
 	chk(['grep', '--', '', ds], want_in_help=['--tab-length'], want_in_call=['this is a value'])
 	chk(['init', '--no-git', job.filename('projdir')], want_in_help=['--no-git'], want_in_call=[''])
 	assert os.path.isdir('projdir/workdirs')
 	chk(['intro'], want_in_call=['ax init --examples', 'ax script'])
 	chk(['job', '--', job], want_in_help=['--just-output', ':urdlist:[entry]'], want_in_call=['"command_prefix":'])
 	chk(['job', '--just-output', '--', job], want_in_call=['look for this later'], dont_want_in_call=['most other things'])
 	in_this_file = 'this string is only here, and will be found here'
@@ -88,21 +89,26 @@
 	chk(['job', '--source', '--', job], want_in_call=[in_this_file, in_extra, extra_hdr]),
 	chk(['job', '--source-file=*.txt', '--', job], want_in_call=[in_extra], dont_want_in_call=[extra_hdr, in_this_file]),
 	chk(['job', '--file=filename', '--', job], want_in_call=[in_written_file], dont_want_in_call=['===', in_this_file]),
 	chk(['method', 'csvimport'], want_in_help=['lists methods'], want_in_call=['filename'])
 	chk(['run'], want_in_help=['[script]', 'WORKDIR'])
 	chk(['script', 'build_tests'], want_in_help=['describes build scripts'], want_in_call=['Needs at least 3 slices to work.'])
 	chk(['server'], want_in_help=['--debuggable'])
+	chk(['status'], want_in_help=['--short'], want_in_call=['test_shell_commands (', 'synthesis (', 'TAIL OF OUTPUT:'])
+	chk(['status', '--short'], want_in_call=['test_shell_commands synthesis ('])
 	chk(['urd'], want_in_help=[':urdlist:[entry]'], want_in_call=['/tests_urd'])
 	chk(['urd', 'tests_urd/'], want_in_call=['2021-09-27T03:14'])
 	chk(['urd', 'tests_urd/2021-09-27T03:14'], want_in_call=['test_shell_data'])
 	chk(['urd-server'], want_in_help=['--allow-passwordless'])
 	chk(['version'], want_in_call=['Running on '])
 	chk(['workdir'], want_in_help=['--full-path'], want_in_call=[job.workdir])
 	chk(['workdir', '--', job.workdir], want_in_call=[job, 'test_shell_commands'])
 
 	ax_help = ax(['--help'])
 	cmd_list = ax_help.split('\ncommands:\n', 1)[1].split('\naliases:\n', 1)[0]
 	cmd_list = {cmd.split()[0] for cmd in cmd_list.strip().split('\n')}
 	missed = cmd_list - all_checked
 	if missed:
 		raise Exception("Didn't check the following commands: " + ' '.join(sorted(missed)))
+	not_in_help = all_checked - cmd_list - {'-h', '--help'}
+	if not_in_help:
+		raise Exception("Missing in help output: " + ' '.join(sorted(not_in_help)))
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_shell_config.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_shell_config.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_shell_data.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_shell_data.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_shell_ds.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_shell_ds.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_shell_grep.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_shell_grep.py`

 * *Files 0% similar despite different names*

```diff
@@ -428,15 +428,17 @@
 	grep_text(['-l', '-c', '', previous], [[ds] for ds, _ in header_test])
 	want = [[ds, str(sliceno)] for ds, sliceno in header_test]
 	grep_text(['-l', '-c', '-S', '', previous], want)
 	grep_text(['-l', '-c', '-S', '-H', '', previous], [['[DATASET]', '[SLICE]']] + want)
 	grep_json(['-l', '-c', '', previous], [{'dataset': ds} for ds, _ in header_test])
 	grep_json(['-l', '-c', '-S', '', previous], [{'dataset': ds, 'sliceno': sliceno} for ds, sliceno in header_test])
 	# test escaping
-	grep_text(['-l', '-t', '/', '-S', '', previous], [['"%s"/%d' % header_test[-1]]])
+	unescaped, sliceno = header_test[-1]
+	escaped = unescaped.replace('\n', '\\n').replace('\r', '\\r').replace('"', '""')
+	grep_text(['-l', '-t', '/', '-S', '', previous], [['"%s"/%d' % (escaped, sliceno)]])
 
 	# more escaping
 	escapy = mk_ds('escapy',
 		[('ascii', 'spaced name'), ('unicode', 'tabbed\tname')],
 		['comma', 'foo,bar'],
 		['tab', 'foo\tbar'],
 		['newline', 'a brand new\nline'],
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_shell_job.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_shell_job.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ############################################################################
 #                                                                          #
-# Copyright (c) 2021 Carl Drougge                                          #
+# Copyright (c) 2021-2023 Carl Drougge                                     #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
 #                                                                          #
@@ -40,18 +40,18 @@
 	print(res)
 	return res.split('\n')
 
 def synthesis(job):
 	os.putenv('XDG_CONFIG_HOME', job.path) # make sure we can't be messed up by config
 	os.putenv('CLICOLOR_FORCE', '1')
 	res = ax_job(job)
-	assert res[0] == job.path, res[0]
+	assert job in res[0], res[0]
 	assert '\x1b[31mWARNING: Job did not finish\x1b[39m' in res
 	os.unsetenv('CLICOLOR_FORCE')
 	os.putenv('NO_COLOR', '')
 	res = ax_job(job)
-	assert res[0] == job.path, res[0]
+	assert job in res[0], res[0]
 	assert 'WARNING: Job did not finish' in res
 	for spec, jobid in options.want.items():
 		res = ax_job(spec)
 		got_jobid = res[0].split('/')[-1]
-		assert jobid == got_jobid, 'Spec %r should have given %r but gave %r' % (spec, jobid, got_jobid,)
+		assert got_jobid.startswith(jobid), 'Spec %r should have given %r but gave %r' % (spec, jobid, got_jobid,)
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_sort_chaining.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_sort_chaining.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_sort_stability.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_sort_stability.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_sort_trigger.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_sort_trigger.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_sorting.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_sorting.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_sorting_gendata.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_sorting_gendata.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_status_in_exceptions.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_status_in_exceptions.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_subjobs_nesting.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_subjobs_nesting.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_subjobs_type.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_subjobs_type.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/a_test_summary.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/a_test_summary.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ############################################################################
 #                                                                          #
-# Copyright (c) 2020 Carl Drougge                                          #
+# Copyright (c) 2020-2023 Carl Drougge                                     #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
 #                                                                          #
@@ -22,20 +22,24 @@
 
 description = r'''
 Produce a summary that build_tests can put in the result directory.
 '''
 
 from accelerator.job import Job
 from accelerator.build import fmttime
+from accelerator.compat import url_quote
 
 options = {'joblist': []}
 
+def html_quote(s):
+	return s.replace('&', '&amp;').replace('<', '&lt;').replace('>', '&gt;')
+
 def synthesis(job):
 	joblist = [Job(j) for j in options.joblist]
 	total = sum(j.params.exectime.total for j in joblist)
 	with job.open('summary.html', 'w', encoding='utf-8') as fh:
 		fh.write('<h2>Test built these jobs in ' + fmttime(total) + '</h2>\n')
 		fh.write('<ol>\n')
-		list_item = '<li><a href="/job/{job}" target="_blank">{job}</a> {job.method} {time}</li>\n'
+		list_item = '<li><a href="/job/%s" target="_blank">%s</a> %s %s</li>\n'
 		for j in joblist:
-			fh.write(list_item.format(job=j, time=fmttime(j.params.exectime.total)))
+			fh.write(list_item % (url_quote(j), html_quote(j), html_quote(j.method), fmttime(j.params.exectime.total)))
 		fh.write('</ol>\n')
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/build_tests.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/build_tests.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 ############################################################################
 #                                                                          #
-# Copyright (c) 2019-2022 Carl Drougge                                     #
+# Copyright (c) 2019-2023 Carl Drougge                                     #
 # Modifications copyright (c) 2020 Anders Berkeman                         #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
@@ -34,14 +34,19 @@
 description = '''
 Run the tests. Needs at least 3 slices to work.
 '''
 
 def main(urd):
 	assert urd.info.slices >= 3, "The tests don't work with less than 3 slices (you have %d)." % (urd.info.slices,)
 
+	from accelerator.shell import cfg
+	# sys.argv[0] is absolute for unqualified commands ("ax"), but exactly what
+	# the user wrote otherwise ("./venv/bin/ax"). This makes either absolute.
+	command_prefix = [os.path.join(cfg.user_cwd, sys.argv[0]), '--config', cfg.config_filename]
+
 	print()
 	print("Testing urd.build and job.load")
 	want = ({'foo': 'foo', 'a': 'a'}, {'foo': '', 'b': ''}, {'foo': '', 'c': ''})
 	job = urd.build("test_build_kws")
 	assert job.load() == want
 	bad = None
 	try:
@@ -61,14 +66,15 @@
 	want[0]['foo'] = 'foo'
 	want[2]['c'] = job
 	job = urd.build("test_build_kws", a='A', b=None, c=job, datasets=dict(b='overridden'))
 	assert job.load() == want
 
 	print()
 	print("Testing urd.begin/end/truncate/get/peek/latest/first/since")
+	urd.build('test_urd', command_prefix=command_prefix)
 	urd.truncate("tests_urd", 0)
 	assert not urd.peek_latest("tests_urd").joblist
 	urd.begin("tests_urd", 1, caption="first")
 	urd.build("test_build_kws")
 	fin = urd.finish("tests_urd")
 	assert fin == {'new': True, 'changed': False, 'is_ghost': False}, fin
 	urd.begin("tests_urd", 1)
@@ -220,14 +226,15 @@
 		joblist=[None, source, ''],
 	)
 
 	print()
 	print("Testing csvimport with more difficult files")
 	urd.build("test_csvimport_corner_cases")
 	urd.build("test_csvimport_separators")
+	urd.build("test_csvimport_slicing")
 
 	print()
 	print("Testing csvexport with all column types, strange separators, ...")
 	urd.build("test_csvexport_naming")
 	urd.build("test_csvexport_all_coltypes")
 	urd.build("test_csvexport_separators")
 	urd.build("test_csvexport_chains")
@@ -296,27 +303,26 @@
 	print("Test datetime types in options")
 	urd.build("test_datetime")
 
 	print()
 	print("Test various utility functions")
 	urd.build("test_optionenum")
 	urd.build("test_json")
+	urd.build("test_job_save")
+	bgsave = urd.build("test_job_save_background")
+	assert len(bgsave.files()) == 10 + 4 * urd.info.slices
 	urd.build("test_jobwithfile")
 	urd.build("test_jobchain")
 
 	print()
 	print("Testing that the status stack is correct in exceptions from job building")
 	urd.build("test_status_in_exceptions")
 
 	print()
 	print("Test shell commands")
-	from accelerator.shell import cfg
-	# sys.argv[0] is absolute for unqualified commands ("ax"), but exactly what
-	# the user wrote otherwise ("./venv/bin/ax"). This makes either absolute.
-	command_prefix = [os.path.join(cfg.user_cwd, sys.argv[0]), '--config', cfg.config_filename]
 	urd.truncate("tests_urd", 0)
 	# These have to be rebuilt every time, or the resolving might give other jobs.
 	urd.begin("tests_urd", 1)
 	a = urd.build('test_shell_data', force_build=True)
 	b = urd.build('test_shell_data', force_build=True)
 	c = urd.build('test_shell_data', datasets={'previous': a})
 	urd.finish("tests_urd")
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/methods.conf` & `accelerator-2023.7.18.dev1/accelerator/test_methods/methods.conf`

 * *Files 2% similar despite different names*

```diff
@@ -44,25 +44,28 @@
 test_sorting_gendata
 test_sort_stability
 test_sort_chaining
 test_sort_trigger
 test_hashpart
 test_csvimport_separators
 test_csvimport_corner_cases
+test_csvimport_slicing
 test_csvimport_zip
 test_csvexport_all_coltypes
 test_csvexport_separators
 test_csvexport_chains
 test_csvexport_naming
 test_csvexport_quoting
 test_hashlabel
 test_json
 test_optionenum
 test_options_dict_order
 test_options_rebuild
+test_job_save
+test_job_save_background
 test_jobwithfile
 test_jobchain
 test_output
 test_output_s
 test_output_ps
 test_output_pas
 test_output_pa
@@ -72,9 +75,10 @@
 test_datetime
 test_shell_commands
 test_shell_data
 test_shell_job
 test_shell_ds
 test_shell_grep
 test_shell_config
+test_urd
 test_status_in_exceptions
 test_summary
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/test_methods/test_data.py` & `accelerator-2023.7.18.dev1/accelerator/test_methods/test_data.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/unixhttp.py` & `accelerator-2023.7.18.dev1/accelerator/unixhttp.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 ############################################################################
 #                                                                          #
 # Copyright (c) 2017 eBay Inc.                                             #
-# Modifications copyright (c) 2019-2021 Carl Drougge                       #
+# Modifications copyright (c) 2019-2023 Carl Drougge                       #
+# Modifications copyright (c) 2023 Pablo Correa Gómez                      #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
 #                                                                          #
@@ -16,15 +17,15 @@
 # limitations under the License.                                           #
 #                                                                          #
 ############################################################################
 
 from __future__ import print_function
 from __future__ import division
 
-from accelerator.compat import PY3, unquote_plus
+from accelerator.compat import PY3
 from accelerator.compat import urlopen, Request, URLError, HTTPError
 from accelerator.extras import json_encode, json_decode
 from accelerator.error import ServerError, UrdError, UrdPermissionError, UrdConflictError
 from accelerator import g, __version__ as ax_version
 
 if PY3:
 	from urllib.request import install_opener, build_opener, AbstractHTTPHandler
@@ -36,15 +37,15 @@
 import sys
 import time
 import socket
 
 class UnixHTTPConnection(HTTPConnection):
 	def __init__(self, host, *a, **kw):
 		HTTPConnection.__init__(self, 'localhost', *a, **kw)
-		self.unix_path = unquote_plus(host.split(':', 1)[0])
+		self.unix_path = host
 
 	def connect(self):
 		s = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
 		s.connect(self.unix_path)
 		self.sock = s
 
 class UnixHTTPHandler(AbstractHTTPHandler):
@@ -70,14 +71,19 @@
 		server.run()
 
 
 def call(url, data=None, fmt=json_decode, headers={}, server_name='server', retries=4, quiet=False):
 	if data is not None and not isinstance(data, bytes):
 		data = json_encode(data)
 	err = None
+	if url.startswith('unixhttp://'):
+		# The path ends up in the Host-header if we don't override it, and
+		# if the path contains characters that aren't in latin-1 that breaks.
+		headers = dict(headers)
+		headers['Host'] = server_name
 	req = Request(url, data=data, headers=headers)
 	for attempt in range(1, retries + 2):
 		resp = None
 		try:
 			r = urlopen(req)
 			try:
 				resp = r.read()
@@ -109,21 +115,21 @@
 				if e.code == 401:
 					err = UrdPermissionError()
 				if e.code == 409:
 					err = UrdConflictError()
 				break
 			if server_name == 'server' and e.code != 503 and resp:
 				return fmt(resp)
-		except URLError:
+		except URLError as e:
 			# Don't say anything the first times, because the output
 			# tests get messed up if this happens during them.
 			if attempt < retries - 1:
 				msg = None
 			else:
-				msg = 'error contacting ' + server_name
+				msg = 'error contacting %s: %s' % (server_name, e.reason)
 		except ValueError as e:
 			msg = 'Bad data from %s, %s: %s' % (server_name, type(e).__name__, e,)
 		if msg and not quiet:
 			print(msg, file=sys.stderr)
 		if attempt < retries + 1:
 			time.sleep(attempt / 15)
 			if msg and not quiet:
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/urd.py` & `accelerator-2023.7.18.dev1/accelerator/urd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ############################################################################
 #                                                                          #
 # Copyright (c) 2017 eBay Inc.                                             #
-# Modifications copyright (c) 2018-2022 Carl Drougge                       #
+# Modifications copyright (c) 2018-2023 Carl Drougge                       #
 # Modifications copyright (c) 2020 Anders Berkeman                         #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
@@ -39,15 +39,15 @@
 
 from accelerator.compat import iteritems, itervalues, unicode
 from accelerator.colourwrapper import colour
 from accelerator.extras import DotDict, PY3
 from accelerator.shell.parser import ArgumentParser
 from accelerator.unixhttp import WaitressServer
 
-LOGFILEVERSION = '3'
+LOGFILEVERSION = '4'
 
 lock = Lock()
 
 def locked(func):
 	def inner(*a, **kw):
 		with lock:
 			return func(*a, **kw)
@@ -171,18 +171,26 @@
 		else:
 			print("Creating directory \"%s\"." % (path,))
 			os.makedirs(path)
 		self._lasttime = None
 		self._initialised = True
 
 	def _parse(self, line):
-		line = line.rstrip('\n').split('|')
+		line = line.rstrip('\n')
+		if line[:2] == '3|':
+			line = line.split('|')
+		else:
+			line = line.split('\t')
 		logfileversion, writets = line[:2]
-		assert logfileversion == '3'
 		assert writets not in self._parsed
+		if logfileversion == '3':
+			if line[2] == 'add':
+				line[-1] = json.dumps(line[-1]) # caption is json encoded in v4
+		else:
+			assert logfileversion == '4', logfileversion
 		self._parsed[writets] = line[2:]
 
 	def _playback_parsed(self):
 		for _writets, line in sorted(iteritems(self._parsed)):
 			action = line.pop(0)
 			assert action in ('add', 'truncate',)
 			if action == 'add':
@@ -198,15 +206,15 @@
 		flags = line[4].split(',') if line[4] else []
 		data = DotDict(timestamp=line[0],
 			user=user,
 			build=build,
 			deps=json.loads(line[2]),
 			joblist=json.loads(line[3]),
 			flags=flags,
-			caption=line[5],
+			caption=json.loads(line[5]),
 		)
 		self.add(data)
 
 	def _parse_truncate(self, line):
 		timestamp, key = line
 		self.truncate(key, timestamp)
 
@@ -227,30 +235,32 @@
 		data.timestamp = TimeStamp(data.timestamp)
 
 	def _serialise(self, action, data):
 		if action == 'add':
 			self._validate_data(data)
 			json_deps = json.dumps(data.deps)
 			json_joblist = json.dumps(data.joblist)
+			json_caption = json.dumps(data.caption)
 			key = '%s/%s' % (data.user, data.build,)
 			flags = ','.join(data.flags)
-			for s in json_deps, json_joblist, data.caption, data.user, data.build, data.timestamp, flags:
-				assert '|' not in s, s
-			logdata = [json_deps, json_joblist, flags, data.caption,]
+			for s in key, json_deps, json_joblist, json_caption, data.user, data.build, data.timestamp, flags:
+				assert '\t' not in s, s
+				assert '\n' not in s, s
+			logdata = [json_deps, json_joblist, flags, json_caption,]
 		elif action == 'truncate':
 			key = data.key
 			logdata = []
 		else:
 			assert "can't happen"
 		data.timestamp = TimeStamp(data.timestamp)
 		while True: # paranoia
 			now = datetime.utcnow().strftime("%Y-%m-%dT%H:%M:%S.%f")
 			if now != self._lasttime: break
 		self._lasttime = now
-		s = '|'.join([LOGFILEVERSION, now, action, data.timestamp, key,] + logdata)
+		s = '\t'.join([LOGFILEVERSION, now, action, data.timestamp, key,] + logdata)
 		return s
 
 	def _is_ghost(self, data):
 		for key, data in iteritems(data.deps):
 			db = self.db[key]
 			ts = data['timestamp']
 			if ts not in db:
@@ -560,35 +570,41 @@
 def main(argv, cfg):
 	global authdict, allow_passwordless, db
 
 	parser = ArgumentParser(prog=argv.pop(0))
 	parser.add_argument('--path', type=str, default='urd.db',
 		help='database directory (can be relative to project directory) (default: urd.db)',
 	)
+	parser.add_argument('--listen', help='[host]:port or socket path, overrides config')
 	parser.add_argument('--allow-passwordless', action='store_true', negation='dont', help='accept any pass for users not in passwd.')
 	parser.add_argument('--quiet',              action='store_true', negation='not',  help='less chatty.')
 	args = parser.parse_intermixed_args(argv)
-	if not args.quiet:
-		print('-'*79)
-		print(args)
-		print()
+
+	if args.listen is None:
+		listen = cfg.urd_listen
+		if not listen:
+			raise Exception('urd not configured in this project')
+	else:
+		from accelerator.configfile import resolve_listen
+		listen = resolve_listen(args.listen)[0]
 
 	auth_fn = os.path.join(args.path, 'passwd')
 	authdict = readauth(auth_fn)
 	allow_passwordless = args.allow_passwordless
 	if not authdict and not args.allow_passwordless:
 		raise Exception('No users in %r and --allow-passwordless not specified.' % (auth_fn,))
 	db = DB(args.path, not args.quiet)
 
+	# The standard DotDict is now ordered, but that doesn't suit urd.
+	DotDict.__eq__ = dict.__eq__
+	DotDict.__ne__ = dict.__ne__
+
 	bottle.install(jsonify)
 
 	kw = dict(debug=False, reloader=False, quiet=args.quiet, server=WaitressServer)
-	listen = cfg.urd_listen
-	if not listen:
-		raise Exception('urd not configured in this project')
 	if isinstance(listen, tuple):
 		kw['host'], kw['port'] = listen
 	else:
 		from accelerator.server import check_socket
 		check_socket(listen)
 		kw['host'] = listen
 		kw['port'] = 0
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/web.py` & `accelerator-2023.7.18.dev1/accelerator/web.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 ############################################################################
 #                                                                          #
 # Copyright (c) 2017 eBay Inc.                                             #
-# Modifications copyright (c) 2019-2021 Carl Drougge                       #
+# Modifications copyright (c) 2019-2023 Carl Drougge                       #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
 #                                                                          #
@@ -76,14 +76,16 @@
 		bare_ctype = ctype.split(";", 1)[0].strip()
 		if bare_ctype in ("application/x-www-form-urlencoded", "multipart/form-data"):
 			env = {"CONTENT_LENGTH": length,
 			       "CONTENT_TYPE"  : ctype,
 			       "REQUEST_METHOD": "POST"
 			      }
 			cgi_args = cgi.parse(self.rfile, environ=env, keep_blank_values=True)
+			if PY3:
+				cgi_args = {k: [v[-1].encode('iso-8859-1')] for k, v in cgi_args.items()}
 		else:
 			cgi_args = {None: [self.rfile.read(int(length))]}
 		self.is_head = False
 		self._do_req2(self.path, cgi_args)
 
 	def _do_req(self):
 		path = self.path.split("?")
```

### Comparing `accelerator-2023.3.10.dev1/accelerator/workarounds.py` & `accelerator-2023.7.18.dev1/accelerator/workarounds.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator/workspace.py` & `accelerator-2023.7.18.dev1/accelerator/workspace.py`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/accelerator.egg-info/PKG-INFO` & `accelerator-2023.7.18.dev1/accelerator.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: accelerator
-Version: 2023.3.10.dev1
+Version: 2023.7.18.dev1
 Summary: A tool for fast and reproducible processing of large amounts of data.
 Home-page: https://exax.org/
 Author: Carl Drougge
 Author-email: bearded@longhaired.org
 Project-URL: Source, https://github.com/eBay/accelerator
 Project-URL: Reference manual, https://berkeman.github.io/pdf/acc_manual.pdf
 Classifier: Development Status :: 4 - Beta
```

### Comparing `accelerator-2023.3.10.dev1/accelerator.egg-info/SOURCES.txt` & `accelerator-2023.7.18.dev1/accelerator.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,17 @@
 accelerator/board/head.tpl
 accelerator/board/job.tpl
 accelerator/board/job_method_list.tpl
 accelerator/board/last_error.tpl
 accelerator/board/main.tpl
 accelerator/board/method.tpl
 accelerator/board/methods.tpl
+accelerator/board/script.js
 accelerator/board/status.tpl
+accelerator/board/style.css
 accelerator/board/urd.tpl
 accelerator/board/urditem.tpl
 accelerator/board/urdlist.tpl
 accelerator/board/workdir.tpl
 accelerator/examples/__init__.py
 accelerator/examples/a_dsexample_aggandmergedata.py
 accelerator/examples/a_dsexample_appendcolumn.py
@@ -97,21 +99,23 @@
 accelerator/examples/data2.csv
 accelerator/examples/data3.csv
 accelerator/examples/mydependency.py
 accelerator/examples/mydependencyfile.txt
 accelerator/examples/printer.py
 accelerator/shell/__init__.py
 accelerator/shell/ds.py
+accelerator/shell/gc.py
 accelerator/shell/grep.py
 accelerator/shell/init.py
 accelerator/shell/job.py
 accelerator/shell/lined.py
 accelerator/shell/method.py
 accelerator/shell/parser.py
 accelerator/shell/script.py
+accelerator/shell/status.py
 accelerator/shell/urd.py
 accelerator/shell/workdir.py
 accelerator/standard_methods/__init__.py
 accelerator/standard_methods/_generated_csvimport.c
 accelerator/standard_methods/_generated_dataset_type.c
 accelerator/standard_methods/a_csvexport.py
 accelerator/standard_methods/a_csvimport.py
@@ -140,14 +144,15 @@
 accelerator/test_methods/a_test_csvexport_all_coltypes.py
 accelerator/test_methods/a_test_csvexport_chains.py
 accelerator/test_methods/a_test_csvexport_naming.py
 accelerator/test_methods/a_test_csvexport_quoting.py
 accelerator/test_methods/a_test_csvexport_separators.py
 accelerator/test_methods/a_test_csvimport_corner_cases.py
 accelerator/test_methods/a_test_csvimport_separators.py
+accelerator/test_methods/a_test_csvimport_slicing.py
 accelerator/test_methods/a_test_csvimport_zip.py
 accelerator/test_methods/a_test_dataset_callbacks.py
 accelerator/test_methods/a_test_dataset_checksum.py
 accelerator/test_methods/a_test_dataset_column_names.py
 accelerator/test_methods/a_test_dataset_concat.py
 accelerator/test_methods/a_test_dataset_empty_colname.py
 accelerator/test_methods/a_test_dataset_fanout.py
@@ -175,14 +180,16 @@
 accelerator/test_methods/a_test_datasetwriter_parent.py
 accelerator/test_methods/a_test_datasetwriter_parsed.py
 accelerator/test_methods/a_test_datasetwriter_verify.py
 accelerator/test_methods/a_test_datetime.py
 accelerator/test_methods/a_test_finish_early.py
 accelerator/test_methods/a_test_hashlabel.py
 accelerator/test_methods/a_test_hashpart.py
+accelerator/test_methods/a_test_job_save.py
+accelerator/test_methods/a_test_job_save_background.py
 accelerator/test_methods/a_test_jobchain.py
 accelerator/test_methods/a_test_jobwithfile.py
 accelerator/test_methods/a_test_json.py
 accelerator/test_methods/a_test_number.py
 accelerator/test_methods/a_test_optionenum.py
 accelerator/test_methods/a_test_options_dict_order.py
 accelerator/test_methods/a_test_options_rebuild.py
@@ -207,13 +214,14 @@
 accelerator/test_methods/a_test_sort_trigger.py
 accelerator/test_methods/a_test_sorting.py
 accelerator/test_methods/a_test_sorting_gendata.py
 accelerator/test_methods/a_test_status_in_exceptions.py
 accelerator/test_methods/a_test_subjobs_nesting.py
 accelerator/test_methods/a_test_subjobs_type.py
 accelerator/test_methods/a_test_summary.py
+accelerator/test_methods/a_test_urd.py
 accelerator/test_methods/build_tests.py
 accelerator/test_methods/methods.conf
 accelerator/test_methods/test_data.py
 accelerator/test_methods/test_shell_commands.txt
 dsutil/dsutilmodule.c
 dsutil/siphash24.c
```

### Comparing `accelerator-2023.3.10.dev1/dsutil/dsutilmodule.c` & `accelerator-2023.7.18.dev1/dsutil/dsutilmodule.c`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/dsutil/siphash24.c` & `accelerator-2023.7.18.dev1/dsutil/siphash24.c`

 * *Files identical despite different names*

### Comparing `accelerator-2023.3.10.dev1/setup.py` & `accelerator-2023.7.18.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 #!/usr/bin/env python
 
 ############################################################################
 #                                                                          #
-# Copyright (c) 2019-2022 Carl Drougge                                     #
+# Copyright (c) 2019-2023 Carl Drougge                                     #
 # Modifications copyright (c) 2020 Anders Berkeman                         #
 #                                                                          #
 # Licensed under the Apache License, Version 2.0 (the "License");          #
 # you may not use this file except in compliance with the License.         #
 # You may obtain a copy of the License at                                  #
 #                                                                          #
 #  http://www.apache.org/licenses/LICENSE-2.0                              #
@@ -138,15 +138,15 @@
 		'selectors2>=2.0; python_version<"3"',
 	],
 	python_requires=">=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, <4",
 
 	ext_modules=[dsutilmodule, dataset_typemodule, csvimportmodule],
 
 	package_data={
-		'': ['*.txt', 'methods.conf', 'board/*.tpl', 'examples/*.csv'],
+		'': ['*.txt', 'methods.conf', 'board/*.tpl', 'board/*.css', 'board/*.js', 'examples/*.csv'],
 	},
 
 	author="Carl Drougge",
 	author_email="bearded@longhaired.org",
 	url="https://exax.org/",
 	description="A tool for fast and reproducible processing of large amounts of data.",
 	long_description=long_description,
```

