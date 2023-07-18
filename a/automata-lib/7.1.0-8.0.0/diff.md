# Comparing `tmp/automata-lib-7.1.0.tar.gz` & `tmp/automata-lib-8.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "automata-lib-7.1.0.tar", last modified: Sun Jan  8 23:27:14 2023, max compression
+gzip compressed data, was "automata-lib-8.0.0.tar", last modified: Tue Jul 18 19:15:38 2023, max compression
```

## Comparing `automata-lib-7.1.0.tar` & `automata-lib-8.0.0.tar`

### file list

```diff
@@ -1,51 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 23:27:14.274521 automata-lib-7.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-01-08 23:26:56.000000 automata-lib-7.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-01-08 23:27:14.274521 automata-lib-7.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-01-08 23:26:56.000000 automata-lib-7.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 23:27:14.266520 automata-lib-7.1.0/automata/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 23:27:14.270521 automata-lib-7.1.0/automata/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4823 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/base/automaton.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/base/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/base/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3412 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/base/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 23:27:14.270521 automata-lib-7.1.0/automata/fa/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/fa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52313 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/fa/dfa.py
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/fa/fa.py
--rw-r--r--   0 runner    (1001) docker     (123)    13363 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/fa/gnfa.py
--rw-r--r--   0 runner    (1001) docker     (123)    34624 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/fa/nfa.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 23:27:14.270521 automata-lib-7.1.0/automata/pda/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/pda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/pda/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6026 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/pda/dpda.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/pda/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4611 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/pda/npda.py
--rw-r--r--   0 runner    (1001) docker     (123)     3576 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/pda/pda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/pda/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 23:27:14.270521 automata-lib-7.1.0/automata/regex/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/regex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3399 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/regex/lexer.py
--rw-r--r--   0 runner    (1001) docker     (123)    13166 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/regex/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4582 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/regex/postfix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/regex/regex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 23:27:14.270521 automata-lib-7.1.0/automata/tm/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/tm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1889 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/tm/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     5630 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/tm/dtm.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/tm/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12493 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/tm/mntm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5840 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/tm/ntm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2716 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/tm/tape.py
--rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/tm/tm.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-01-08 23:26:56.000000 automata-lib-7.1.0/automata/tm/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-08 23:27:14.274521 automata-lib-7.1.0/automata_lib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3757 2023-01-08 23:27:14.000000 automata-lib-7.1.0/automata_lib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      961 2023-01-08 23:27:14.000000 automata-lib-7.1.0/automata_lib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-08 23:27:14.000000 automata-lib-7.1.0/automata_lib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-01-08 23:27:14.000000 automata-lib-7.1.0/automata_lib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-01-08 23:27:14.000000 automata-lib-7.1.0/automata_lib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-01-08 23:26:56.000000 automata-lib-7.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-08 23:27:14.274521 automata-lib-7.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-08 23:26:56.000000 automata-lib-7.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:15:38.474712 automata-lib-8.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-07-18 19:14:51.000000 automata-lib-8.0.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-18 19:15:38.474712 automata-lib-8.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-07-18 19:14:51.000000 automata-lib-8.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:15:38.462711 automata-lib-8.0.0/automata/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:15:38.466712 automata-lib-8.0.0/automata/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5996 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/base/automaton.py
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/base/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3725 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/base/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:15:38.466712 automata-lib-8.0.0/automata/fa/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/fa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63479 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/fa/dfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8441 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/fa/fa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13110 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/fa/gnfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40871 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/fa/nfa.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:15:38.466712 automata-lib-8.0.0/automata/pda/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/pda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/pda/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6731 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/pda/dpda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/pda/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5214 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/pda/npda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/pda/pda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1681 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/pda/stack.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:15:38.466712 automata-lib-8.0.0/automata/regex/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/regex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/regex/lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19669 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/regex/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/regex/postfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1676 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/regex/regex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:15:38.470712 automata-lib-8.0.0/automata/tm/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/tm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/tm/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/tm/dtm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/tm/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13080 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/tm/mntm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6575 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/tm/ntm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/tm/tape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1464 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/tm/tm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-07-18 19:14:51.000000 automata-lib-8.0.0/automata/tm/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:15:38.470712 automata-lib-8.0.0/automata_lib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4092 2023-07-18 19:15:38.000000 automata-lib-8.0.0/automata_lib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-07-18 19:15:38.000000 automata-lib-8.0.0/automata_lib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 19:15:38.000000 automata-lib-8.0.0/automata_lib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-18 19:15:38.000000 automata-lib-8.0.0/automata_lib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 19:15:38.000000 automata-lib-8.0.0/automata_lib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-07-18 19:14:51.000000 automata-lib-8.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 19:15:38.474712 automata-lib-8.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-18 19:14:51.000000 automata-lib-8.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 19:15:38.474712 automata-lib-8.0.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_automaton.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    88353 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_dfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12915 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_dpda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14199 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_dtm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3365 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_fa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17065 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_gnfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10381 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_lexer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18953 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_mntm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48749 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_nfa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14609 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_npda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11239 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_ntm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_pda.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_pdaconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_pdastack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_postfix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8566 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12341 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_tm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_tmconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_tmtape.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-07-18 19:14:51.000000 automata-lib-8.0.0/tests/test_tmtools.py
```

### Comparing `automata-lib-7.1.0/LICENSE.txt` & `automata-lib-8.0.0/LICENSE.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 The MIT License (MIT)
 
-Copyright (c) 2016-2022 Caleb Evans
+Copyright (c) 2016-2023 Caleb Evans
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `automata-lib-7.1.0/PKG-INFO` & `automata-lib-8.0.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: automata-lib
-Version: 7.1.0
+Version: 8.0.0
 Summary: A Python library for simulating finite automata, pushdown automata, and Turing machines
 Author-email: Caleb Evans <caleb@calebevans.me>
-Maintainer-email: Caleb Evans <caleb@calebevans.me>
+Maintainer-email: Caleb Evans <caleb@calebevans.me>, "Eliot W. Robson" <eliot.robson24@gmail.com>
 License: The MIT License (MIT)
         
-        Copyright (c) 2016-2022 Caleb Evans
+        Copyright (c) 2016-2023 Caleb Evans
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -27,59 +27,71 @@
         THE SOFTWARE.
         
 Project-URL: homepage, https://github.com/caleb531/automata
 Project-URL: documentation, https://github.com/caleb531/automata#readme
 Project-URL: repository, https://github.com/caleb531/automata
 Project-URL: changelog, https://github.com/caleb531/automata/releases
 Keywords: automata,finite,non-deterministic,pushdown,turing,machine,state
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: visual
 License-File: LICENSE.txt
 
 # Automata
 
-*Copyright 2016-2022 Caleb Evans*  
+*Copyright 2016-2023 Caleb Evans*  
 *Released under the MIT license*
 
 [![tests](https://github.com/caleb531/automata/actions/workflows/tests.yml/badge.svg)](https://github.com/caleb531/automata/actions/workflows/tests.yml)
 [![Coverage Status](https://coveralls.io/repos/caleb531/automata/badge.svg?branch=main)](https://coveralls.io/r/caleb531/automata?branch=main)
 
 Automata is a Python 3 library which implements the structures and algorithms
 for finite automata, pushdown automata, and Turing machines. The library
-requires Python 3.7 or newer.
+requires Python 3.8 or newer.
 
-Huge thanks to [@YtvwlD][YtvwlD], [@dengl11][dengl11], [@Tagl][Tagl],
-[@lewiuberg][lewiuberg], [@CamiloMartinezM][CamiloMartinezM],
-[@abhinavsinha‑adrino][abhinavsinha-adrino], and [@eliotwrobson][eliotwrobson]
-for their invaluable code contributions to this project! 🎉
+Huge thanks to [@eliotwrobson][eliotwrobson], [@YtvwlD][YtvwlD],
+[@dengl11][dengl11], [@Tagl][Tagl], [@lewiuberg][lewiuberg],
+[@CamiloMartinezM][CamiloMartinezM],
+[@abhinavsinha‑adrino][abhinavsinha-adrino],
+[@EduardoGoulart1][EduardoGoulart1], and
+[@khoda81][khoda81] for their invaluable code contributions to
+this project! 🎉
 
+[eliotwrobson]: https://github.com/eliotwrobson
 [YtvwlD]: https://github.com/YtvwlD
 [dengl11]: https://github.com/dengl11
 [Tagl]: https://github.com/Tagl
 [lewiuberg]: https://github.com/lewiuberg
 [CamiloMartinezM]: https://github.com/CamiloMartinezM
 [abhinavsinha-adrino]: https://github.com/abhinavsinha-adrino
-[eliotwrobson]: https://github.com/eliotwrobson
+[EduardoGoulart1]: https://github.com/EduardoGoulart1
+[khoda81]: https://github.com/khoda81
 
-## Migrating to v7
+## Migrating to v8
 
-If you wish to migrate to Automata v7 from an older version, please follow the
+If you wish to migrate to Automata v8 from an older version, please follow the
 [migration guide][migration].
 
 <!-- the below link must be an absolute URL to be functional in the PyPI README -->
 [migration]: https://github.com/caleb531/automata/blob/main/MIGRATION.md
 
 ## Installing
 
 You can install the latest version of Automata via pip:
 
 ```sh
 pip install automata-lib
 ```
 
+To install the optional visual dependencies, use the `visual` extra:
+
+```sh
+pip install 'automata-lib[visual]'
+```
+
 ## API
 
 Please refer to [the official API Documentation][docs] in the `docs/` directory
 of the GitHub repository.
 
 <!-- the below link must be an absolute URL to be functional in the PyPI README -->
 [docs]: https://github.com/caleb531/automata/blob/main/docs/README.md
```

### Comparing `automata-lib-7.1.0/README.md` & `automata-lib-8.0.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,48 +1,59 @@
 # Automata
 
-*Copyright 2016-2022 Caleb Evans*  
+*Copyright 2016-2023 Caleb Evans*  
 *Released under the MIT license*
 
 [![tests](https://github.com/caleb531/automata/actions/workflows/tests.yml/badge.svg)](https://github.com/caleb531/automata/actions/workflows/tests.yml)
 [![Coverage Status](https://coveralls.io/repos/caleb531/automata/badge.svg?branch=main)](https://coveralls.io/r/caleb531/automata?branch=main)
 
 Automata is a Python 3 library which implements the structures and algorithms
 for finite automata, pushdown automata, and Turing machines. The library
-requires Python 3.7 or newer.
+requires Python 3.8 or newer.
 
-Huge thanks to [@YtvwlD][YtvwlD], [@dengl11][dengl11], [@Tagl][Tagl],
-[@lewiuberg][lewiuberg], [@CamiloMartinezM][CamiloMartinezM],
-[@abhinavsinha‑adrino][abhinavsinha-adrino], and [@eliotwrobson][eliotwrobson]
-for their invaluable code contributions to this project! 🎉
+Huge thanks to [@eliotwrobson][eliotwrobson], [@YtvwlD][YtvwlD],
+[@dengl11][dengl11], [@Tagl][Tagl], [@lewiuberg][lewiuberg],
+[@CamiloMartinezM][CamiloMartinezM],
+[@abhinavsinha‑adrino][abhinavsinha-adrino],
+[@EduardoGoulart1][EduardoGoulart1], and
+[@khoda81][khoda81] for their invaluable code contributions to
+this project! 🎉
 
+[eliotwrobson]: https://github.com/eliotwrobson
 [YtvwlD]: https://github.com/YtvwlD
 [dengl11]: https://github.com/dengl11
 [Tagl]: https://github.com/Tagl
 [lewiuberg]: https://github.com/lewiuberg
 [CamiloMartinezM]: https://github.com/CamiloMartinezM
 [abhinavsinha-adrino]: https://github.com/abhinavsinha-adrino
-[eliotwrobson]: https://github.com/eliotwrobson
+[EduardoGoulart1]: https://github.com/EduardoGoulart1
+[khoda81]: https://github.com/khoda81
 
-## Migrating to v7
+## Migrating to v8
 
-If you wish to migrate to Automata v7 from an older version, please follow the
+If you wish to migrate to Automata v8 from an older version, please follow the
 [migration guide][migration].
 
 <!-- the below link must be an absolute URL to be functional in the PyPI README -->
 [migration]: https://github.com/caleb531/automata/blob/main/MIGRATION.md
 
 ## Installing
 
 You can install the latest version of Automata via pip:
 
 ```sh
 pip install automata-lib
 ```
 
+To install the optional visual dependencies, use the `visual` extra:
+
+```sh
+pip install 'automata-lib[visual]'
+```
+
 ## API
 
 Please refer to [the official API Documentation][docs] in the `docs/` directory
 of the GitHub repository.
 
 <!-- the below link must be an absolute URL to be functional in the PyPI README -->
 [docs]: https://github.com/caleb531/automata/blob/main/docs/README.md
```

### Comparing `automata-lib-7.1.0/automata/base/exceptions.py` & `automata-lib-8.0.0/automata/base/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,30 +56,34 @@
 
     pass
 
 
 @dataclass
 class LexerError(RegexException):
     """An exception raised for issues in lexing"""
+
     message: str
     position: int
 
 
 class InvalidRegexError(RegexException):
     """Regular expression is invalid"""
 
     pass
 
 
 class SymbolMismatchError(AutomatonException):
     """The input symbols between the given automata do not match"""
+
     pass
 
 
 class EmptyLanguageException(AutomatonException):
     """The operation cannot be performed because the language is empty"""
+
     pass
 
 
 class InfiniteLanguageException(AutomatonException):
     """The operation cannot be performed because the language is infinite"""
+
     pass
```

### Comparing `automata-lib-7.1.0/automata/base/utils.py` & `automata-lib-8.0.0/automata/base/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,82 +1,88 @@
 #!/usr/bin/env python3
 """Miscellaneous utility functions and classes."""
 
 from collections import defaultdict
+from itertools import count
+from typing import Any, Callable, Dict, Generic, Iterable, List, Set, Tuple, TypeVar
 
 from frozendict import frozendict
 
 
-def freeze_value(value):
+def freeze_value(value: Any) -> Any:
     """
     A helper function to convert the given value / structure into a fully
     immutable one by recursively processing said structure and any of its
     members, freezing them as well
     """
     if isinstance(value, (str, int)):
         return value
     if isinstance(value, dict):
-        return frozendict({
-            dict_key: freeze_value(dict_value)
-            for dict_key, dict_value in value.items()
-        })
+        return frozendict(
+            {
+                dict_key: freeze_value(dict_value)
+                for dict_key, dict_value in value.items()
+            }
+        )
     if isinstance(value, set):
         return frozenset(freeze_value(element) for element in value)
     if isinstance(value, list):
         return tuple(freeze_value(element) for element in value)
     return value
 
 
-def get_renaming_function(counter):
+def get_renaming_function(counter: count) -> Callable[[Any], int]:
     """
     A helper function that returns a renaming function to be used in the creation of
     other automata. The parameter counter should be an itertools count.
     This helper function will return the same distinct output taken from counter
     for each distinct input.
     """
 
-    new_state_name_dict = defaultdict(lambda: next(counter))
+    return defaultdict(counter.__next__).__getitem__
 
-    def renaming_function(item):
-        return new_state_name_dict[item]
 
-    return renaming_function
+T = TypeVar("T")
 
 
-class PartitionRefinement:
+class PartitionRefinement(Generic[T]):
     """Maintain and refine a partition of a set of items into subsets.
-    Space usage for a partition of n items is O(n), and each refine
-    operation takes time proportional to the size of its argument.
+    Space usage for a partition of n items is O(n), and each refine operation
+    takes time proportional to the size of its argument.
 
-    Adapted from code by D. Eppstein: https://www.ics.uci.edu/~eppstein/PADS/PartitionRefinement.py
+    Adapted from code by D. Eppstein:
+    https://www.ics.uci.edu/~eppstein/PADS/PartitionRefinement.py
     """
 
-    __slots__ = ('_sets', '_partition')
+    __slots__: Tuple[str, ...] = ("_sets", "_partition")
 
-    def __init__(self, items):
+    _sets: Dict[int, Set[T]]
+    _partition: Dict[T, int]
+
+    def __init__(self, items: Iterable[T]) -> None:
         """Create a new partition refinement data structure for the given
         items. Initially, all items belong to the same subset.
         """
         S = set(items)
         self._sets = {id(S): S}
         self._partition = {x: id(S) for x in S}
 
-    def get_set_by_id(self, id):
+    def get_set_by_id(self, id: int) -> Set[T]:
         """Return the set in the partition corresponding to id."""
         return self._sets[id]
 
-    def get_set_ids(self):
+    def get_set_ids(self) -> Iterable[int]:
         """Return set ids corresponding to the internal partition."""
         return self._sets.keys()
 
-    def get_sets(self):
+    def get_sets(self) -> Iterable[Set[T]]:
         """Return sets corresponding to the internal partition."""
         return self._sets.values()
 
-    def refine(self, S):
+    def refine(self, S: Iterable[T]) -> List[Tuple[int, int]]:
         """Refine each set A in the partition to the two sets
         A & S, A - S.  Return a list of pairs ids (id(A & S), id(A - S))
         for each changed set.  Within each pair, A & S will be
         a newly created set, while A - S will be a modified
         version of an existing set in the partition (retaining its old id).
         Not a generator because we need to perform the partition
         even if the caller doesn't iterate through the results.
@@ -86,15 +92,16 @@
 
         for x in S:
             hit[self._partition[x]].add(x)
 
         for Aid, AintS in hit.items():
             A = self._sets[Aid]
 
-            # Only need to check lengths, we already know AintS is a subset of A by construction
+            # Only need to check lengths, we already know AintS is a subset of A
+            # by construction
             if len(AintS) < len(A):
                 self._sets[id(AintS)] = AintS
                 for x in AintS:
                     self._partition[x] = id(AintS)
                 A -= AintS
                 output.append((id(AintS), Aid))
```

### Comparing `automata-lib-7.1.0/automata/fa/dfa.py` & `automata-lib-8.0.0/automata/fa/nfa.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,1321 +1,1077 @@
 #!/usr/bin/env python3
-"""Classes and methods for working with deterministic finite automata."""
+"""Classes and methods for working with nondeterministic finite automata."""
+from __future__ import annotations
 
-from collections import defaultdict, deque
-from itertools import chain, count
-from random import Random
+import string
+from collections import deque
+from itertools import chain, count, product, repeat
+from typing import (
+    AbstractSet,
+    Any,
+    Deque,
+    Dict,
+    FrozenSet,
+    Generator,
+    Iterable,
+    List,
+    Mapping,
+    Optional,
+    Set,
+    Tuple,
+    Type,
+)
 
 import networkx as nx
-from pydot import Dot, Edge, Node
+from cached_method import cached_method
+from frozendict import frozendict
+from typing_extensions import Self
 
 import automata.base.exceptions as exceptions
+import automata.fa.dfa as dfa
 import automata.fa.fa as fa
-from automata.base.utils import PartitionRefinement, get_renaming_function
+from automata.regex.parser import RESERVED_CHARACTERS, parse_regex
 
+NFAStateT = fa.FAStateT
 
-class DFA(fa.FA):
-    """A deterministic finite automaton."""
-
-    __slots__ = ('states', 'input_symbols', 'transitions',
-                 'initial_state', 'final_states', 'allow_partial')
-
-    def __init__(self, *, states, input_symbols, transitions,
-                 initial_state, final_states, allow_partial=False):
-        """Initialize a complete DFA."""
+NFAPathT = Mapping[str, AbstractSet[NFAStateT]]
+NFATransitionsT = Mapping[NFAStateT, NFAPathT]
+InputPathListT = List[Tuple[NFAStateT, NFAStateT, str]]
+DEFAULT_REGEX_SYMBOLS = frozenset(chain(string.ascii_letters, string.digits))
+
+
+class NFA(fa.FA):
+    """A nondeterministic finite automaton."""
+
+    __slots__: Tuple[str, ...] = (
+        "states",
+        "input_symbols",
+        "transitions",
+        "initial_state",
+        "final_states",
+        # These two entries are to allow for caching methods
+        "__dict__",
+        "__weakref__",
+    )
+
+    transitions: NFATransitionsT
+
+    def __init__(
+        self,
+        *,
+        states: AbstractSet[NFAStateT],
+        input_symbols: AbstractSet[str],
+        transitions: NFATransitionsT,
+        initial_state: NFAStateT,
+        final_states: AbstractSet[NFAStateT],
+    ) -> None:
+        """Initialize a complete NFA."""
         super().__init__(
             states=states,
             input_symbols=input_symbols,
             transitions=transitions,
             initial_state=initial_state,
             final_states=final_states,
-            allow_partial=allow_partial
         )
-        object.__setattr__(self, '_word_cache', [])
-        object.__setattr__(self, '_count_cache', [])
 
-    def __eq__(self, other):
-        """
-        Return True if two DFAs are equivalent. Uses an optimized version of
-        the Hopcroft-Karp algorithm. See https://arxiv.org/abs/0907.5058
+    @cached_method
+    def _get_lambda_closures(self) -> Mapping[NFAStateT, FrozenSet[NFAStateT]]:
         """
+        Computes a dictionary of the lambda closures for this NFA, where each
+        key is the state name and the value is the lambda closure for that
+        corresponding state. This dictionary is cached for the lifetime of the
+        instance, and is available via the 'lambda_closures' attribute.
+
+        The lambda closure of a state q is the set containing q, along with
+        every state that can be reached from q by following only lambda
+        transitions.
+        """
+        lambda_graph = nx.DiGraph()
+        lambda_graph.add_nodes_from(self.states)
+        lambda_graph.add_edges_from(
+            (
+                (start_state, end_state)
+                for start_state, transition in self.transitions.items()
+                for char, end_states in transition.items()
+                if char == ""
+                for end_state in end_states
+            )
+        )
 
-        # Must be another DFA and have equal alphabets
-        if not isinstance(other, DFA) or self.input_symbols != other.input_symbols:
+        return frozendict(
+            {
+                state: frozenset(nx.descendants(lambda_graph, state) | {state})
+                for state in self.states
+            }
+        )
+
+    def __add__(self, other: NFA) -> Self:
+        """Return the concatenation of this NFA and another NFA."""
+        if isinstance(other, NFA):
+            return self.concatenate(other)
+        else:
             return NotImplemented
 
-        operand_dfas = (self, other)
-        initial_state_a = (self.initial_state, 0)
-        initial_state_b = (other.initial_state, 1)
-
-        def is_final_state(state_pair):
-            state, operand_index = state_pair
-            return state in operand_dfas[operand_index].final_states
+    def __or__(self, other: NFA) -> Self:
+        """Return the union of this NFA and another NFA."""
+        if isinstance(other, NFA):
+            return self.union(other)
+        else:
+            return NotImplemented
 
-        def transition(state_pair, symbol):
-            state, operand_index = state_pair
-            return (
-                operand_dfas[operand_index]._get_next_current_state(
-                    state, symbol),
-                operand_index
-            )
+    def __and__(self, other: NFA) -> Self:
+        """Return the union of this NFA and another NFA."""
+        if isinstance(other, NFA):
+            return self.intersection(other)
+        else:
+            return NotImplemented
 
-        # Get data structures
-        state_sets = nx.utils.union_find.UnionFind((initial_state_a, initial_state_b))
-        pair_stack = deque()
+    @classmethod
+    def from_dfa(cls: Type[Self], dfa: dfa.DFA) -> Self:
+        """Initialize this NFA as one equivalent to the given DFA."""
+        nfa_transitions = {
+            start_state: {
+                input_symbol: {end_state} for input_symbol, end_state in paths.items()
+            }
+            for start_state, paths in dfa.transitions.items()
+        }
 
-        # Do union find
-        state_sets.union(initial_state_a, initial_state_b)
-        pair_stack.append((initial_state_a, initial_state_b))
+        return cls(
+            states=dfa.states,
+            input_symbols=dfa.input_symbols,
+            transitions=nfa_transitions,
+            initial_state=dfa.initial_state,
+            final_states=dfa.final_states,
+        )
 
-        while pair_stack:
-            q_a, q_b = pair_stack.pop()
+    def _validate_transition_invalid_symbols(
+        self, start_state: NFAStateT, paths: NFAPathT
+    ) -> None:
+        """Raise an error if transition symbols are invalid."""
+        for input_symbol in paths.keys():
+            if input_symbol not in self.input_symbols and input_symbol != "":
+                raise exceptions.InvalidSymbolError(
+                    "state {} has invalid transition symbol {}".format(
+                        start_state, input_symbol
+                    )
+                )
 
-            if is_final_state(q_a) ^ is_final_state(q_b):
-                return False
+    @classmethod
+    def from_regex(
+        cls: Type[Self], regex: str, *, input_symbols: Optional[AbstractSet[str]] = None
+    ) -> Self:
+        """Initialize this NFA as one equivalent to the given regular expression"""
 
-            for symbol in self.input_symbols:
+        if input_symbols is None:
+            input_symbols = DEFAULT_REGEX_SYMBOLS
+        else:
+            conflicting_symbols = RESERVED_CHARACTERS & input_symbols
+            if conflicting_symbols:
+                raise exceptions.InvalidSymbolError(
+                    f"Invalid input symbols: {conflicting_symbols}"
+                )
 
-                r_1 = state_sets[transition(q_a, symbol)]
-                r_2 = state_sets[transition(q_b, symbol)]
+        nfa_builder = parse_regex(regex, input_symbols)
 
-                if r_1 != r_2:
-                    state_sets.union(r_1, r_2)
-                    pair_stack.append((r_1, r_2))
+        return cls(
+            states=frozenset(nfa_builder._transitions.keys()),
+            input_symbols=input_symbols,
+            transitions=nfa_builder._transitions,
+            initial_state=nfa_builder._initial_state,
+            final_states=nfa_builder._final_states,
+        )
 
-        return True
+    def _validate_transition_end_states(
+        self, start_state: NFAStateT, paths: NFAPathT
+    ) -> None:
+        """Raise an error if transition end states are invalid."""
+        for end_states in paths.values():
+            for end_state in end_states:
+                if end_state not in self.states:
+                    raise exceptions.InvalidStateError(
+                        "end state {} for transition on {} is "
+                        "not valid".format(end_state, start_state)
+                    )
 
-    def __le__(self, other):
-        """Return True if this DFA is a subset of (or equal to) another DFA."""
-        if isinstance(other, DFA):
-            return self.issubset(other)
-        else:
-            return NotImplemented
+    def validate(self) -> None:
+        """Return True if this NFA is internally consistent."""
+        for start_state, paths in self.transitions.items():
+            self._validate_transition_invalid_symbols(start_state, paths)
+            self._validate_transition_end_states(start_state, paths)
+        self._validate_initial_state()
+        self._validate_initial_state_transitions()
+        self._validate_final_states()
 
-    def __ge__(self, other):
-        """Return True if this DFA is a superset of another DFA."""
-        if isinstance(other, DFA):
-            return self.issuperset(other)
-        else:
-            return NotImplemented
+    def _iterate_through_symbol_path_pairs(
+        self, current_states: AbstractSet[NFAStateT]
+    ) -> Generator[Tuple[str, FrozenSet[NFAStateT]], None, None]:
+        """
+        Iterate through input symbols with set of end transitions which are nonempty.
+        """
+
+        lambda_closures = self._get_lambda_closures()
+        res_dict: Dict[str, Set[NFAStateT]] = {}
+
+        for input_symbol, next_states in chain.from_iterable(
+            self.transitions.get(state, {}).items() for state in current_states
+        ):
+            # Ignore empty string and empty end states
+            if input_symbol and next_states:
+                input_symbol_set = res_dict.setdefault(input_symbol, set())
+                for end_state in next_states:
+                    input_symbol_set.update(lambda_closures[end_state])
+
+        for input_symbol, next_states in res_dict.items():
+            yield (input_symbol, frozenset(next_states))
+
+    def _get_next_current_states(
+        self, current_states: AbstractSet[NFAStateT], input_symbol: str
+    ) -> FrozenSet[NFAStateT]:
+        """Return the next set of current states given the current set."""
+        next_current_states: Set[NFAStateT] = set()
+        lambda_closures = self._get_lambda_closures()
 
-    def __lt__(self, other):
-        """Return True if this DFA is a strict subset of another DFA."""
-        if isinstance(other, DFA):
-            return self <= other and self != other
-        else:
-            return NotImplemented
+        for current_state in current_states:
+            if current_state not in self.transitions:
+                continue
+            current_transition = self.transitions[current_state]
+            for end_state in current_transition.get(input_symbol, {}):
+                next_current_states.update(lambda_closures[end_state])
+
+        return frozenset(next_current_states)
+
+    @staticmethod
+    def _compute_reachable_states(
+        initial_state: NFAStateT, transitions: NFATransitionsT
+    ) -> Set[NFAStateT]:
+        """Compute the states which are reachable from the initial state."""
 
-    def __gt__(self, other):
-        """Return True if this DFA is a strict superset of another DFA."""
-        if isinstance(other, DFA):
-            return self >= other and self != other
-        else:
-            return NotImplemented
+        visited_set: Set[NFAStateT] = set()
+        queue: Deque[NFAStateT] = deque()
 
-    def __sub__(self, other):
-        """Return a DFA that is the difference of this DFA and another DFA."""
-        if isinstance(other, DFA):
-            return self.difference(other)
-        else:
-            return NotImplemented
+        queue.append(initial_state)
+        visited_set.add(initial_state)
 
-    def __or__(self, other):
-        """Return the union of this DFA and another DFA."""
-        if isinstance(other, DFA):
-            return self.union(other)
-        else:
-            return NotImplemented
+        while queue:
+            state = queue.popleft()
+            state_dict = transitions.get(state)
 
-    def __and__(self, other):
-        """Return the intersection of this DFA and another DFA."""
-        if isinstance(other, DFA):
-            return self.intersection(other)
-        else:
-            return NotImplemented
+            if state_dict:
+                for next_state in chain.from_iterable(
+                    dest for dest in state_dict.values()
+                ):
+                    if next_state not in visited_set:
+                        visited_set.add(next_state)
+                        queue.append(next_state)
 
-    def __xor__(self, other):
-        """Return the symmetric difference of this DFA and another DFA."""
-        if isinstance(other, DFA):
-            return self.symmetric_difference(other)
-        else:
-            return NotImplemented
+        return visited_set
 
-    def __invert__(self):
-        """Return the complement of this DFA and another DFA."""
-        return self.complement()
-
-    def __iter__(self):
-        """
-        Iterates through all words in the language represented by the DFA.
-        The words are ordered first by length and then by the order of the input symbol set.
-        """
-        i = self.minimum_word_length()
-        limit = self.maximum_word_length()
-        while limit is None or i <= limit:
-            yield from self.words_of_length(i)
-            i += 1
-
-    def __len__(self):
-        """Returns the cardinality of the language represented by the DFA."""
-        return self.cardinality()
-
-    def _validate_transition_missing_symbols(self, start_state, paths):
-        """Raise an error if the transition input_symbols are missing."""
-        if self.allow_partial:
-            return
-        for input_symbol in self.input_symbols:
-            if input_symbol not in paths:
-                raise exceptions.MissingSymbolError(
-                    'state {} is missing transitions for symbol {}'.format(
-                        start_state, input_symbol))
+    def _eliminate_lambda(
+        self,
+    ) -> Tuple[AbstractSet[NFAStateT], NFATransitionsT, AbstractSet[NFAStateT]]:
+        """Internal helper function for eliminate lambda. Doesn't create final NFA."""
 
-    def _validate_transition_invalid_symbols(self, start_state, paths):
-        """Raise an error if transition input symbols are invalid."""
-        for input_symbol in paths.keys():
-            if input_symbol not in self.input_symbols:
-                raise exceptions.InvalidSymbolError(
-                    'state {} has invalid transition symbol {}'.format(
-                        start_state, input_symbol))
+        # Create new transitions and final states for running this algorithm
+        new_transitions = {
+            state: {symbol: set(dest) for symbol, dest in paths.items()}
+            for state, paths in self.transitions.items()
+        }
+        new_final_states = set(self.final_states)
+        lambda_closures = self._get_lambda_closures()
 
-    def _validate_transition_start_states(self):
-        """Raise an error if transition start states are missing."""
-        if self.allow_partial:
-            return
         for state in self.states:
-            if state not in self.transitions:
-                raise exceptions.MissingStateError(
-                    'transition start state {} is missing'.format(
-                        state))
+            lambda_enclosure = lambda_closures[state] - {state}
+            for input_symbol in self.input_symbols:
+                next_current_states = set(
+                    self._get_next_current_states(lambda_enclosure, input_symbol)
+                )
 
-    def _validate_transition_end_states(self, start_state, paths):
-        """Raise an error if transition end states are invalid."""
-        for end_state in paths.values():
-            if end_state not in self.states:
-                raise exceptions.InvalidStateError(
-                    'end state {} for transition on {} is not valid'.format(
-                        end_state, start_state))
-
-    def _validate_transitions(self, start_state, paths):
-        """Raise an error if transitions are missing or invalid."""
-        self._validate_transition_missing_symbols(start_state, paths)
-        self._validate_transition_invalid_symbols(start_state, paths)
-        self._validate_transition_end_states(start_state, paths)
-
-    def validate(self):
-        """Return True if this DFA is internally consistent."""
-        self._validate_transition_start_states()
-        for start_state, paths in self.transitions.items():
-            self._validate_transitions(start_state, paths)
-        self._validate_initial_state()
-        self._validate_final_states()
-        return True
+                # Don't do anything if no new current states
+                if next_current_states:
+                    state_transition_dict = new_transitions.setdefault(state, {})
 
-    def _get_next_current_state(self, current_state, input_symbol):
-        """
-        Follow the transition for the given input symbol on the current state.
+                    if input_symbol in state_transition_dict:
+                        state_transition_dict[input_symbol].update(next_current_states)
+                    else:
+                        state_transition_dict[input_symbol] = next_current_states
 
-        Raise an error if the transition does not exist.
-        """
-        if current_state is not None and input_symbol in self.transitions[current_state]:
-            return self.transitions[current_state][input_symbol]
-        return None
+            if not new_final_states.isdisjoint(lambda_enclosure):
+                new_final_states.add(state)
+
+            if state in new_transitions:
+                new_transitions[state].pop("", None)
+
+        # Remove unreachable states
+        reachable_states = self.__class__._compute_reachable_states(
+            self.initial_state, new_transitions
+        )
+        reachable_final_states = reachable_states & new_final_states
+
+        for state in self.states - reachable_states:
+            new_transitions.pop(state, None)
+
+        return reachable_states, new_transitions, reachable_final_states
+
+    def eliminate_lambda(self) -> Self:
+        """Removes epsilon transitions from the NFA which recognizes the same
+        language."""
+
+        (
+            reachable_states,
+            new_transitions,
+            reachable_final_states,
+        ) = self._eliminate_lambda()
+
+        return self.__class__(
+            states=reachable_states,
+            input_symbols=self.input_symbols,
+            transitions=new_transitions,
+            initial_state=self.initial_state,
+            final_states=reachable_final_states,
+        )
 
-    def _check_for_input_rejection(self, current_state):
+    def _check_for_input_rejection(
+        self, current_states: AbstractSet[NFAStateT]
+    ) -> None:
         """Raise an error if the given config indicates rejected input."""
-        if current_state not in self.final_states:
+        if current_states.isdisjoint(self.final_states):
             raise exceptions.RejectionException(
-                'the DFA stopped on a non-final state ({})'.format(
-                    current_state))
+                "the NFA stopped on all non-final states ({})".format(
+                    ", ".join(str(state) for state in current_states)
+                )
+            )
 
-    def read_input_stepwise(self, input_str, ignore_rejection=False):
+    def read_input_stepwise(
+        self, input_str: str
+    ) -> Generator[AbstractSet[NFAStateT], None, None]:
         """
-        Check if the given string is accepted by this DFA.
+        Check if the given string is accepted by this NFA.
 
-        Yield the current configuration of the DFA at each step.
+        Yield the current configuration of the NFA at each step.
         """
-        current_state = self.initial_state
+        current_states = self._get_lambda_closures()[self.initial_state]
 
-        yield current_state
+        yield current_states
         for input_symbol in input_str:
-            current_state = self._get_next_current_state(
-                current_state, input_symbol)
-            yield current_state
-
-        if not ignore_rejection:
-            self._check_for_input_rejection(current_state)
-
-    def _get_digraph(self):
-        """Return a digraph corresponding to this DFA with transition symbols ignored"""
-        return nx.DiGraph([
-            (start_state, end_state)
-            for start_state, transition in self.transitions.items()
-            for end_state in transition.values()
-        ])
+            current_states = self._get_next_current_states(current_states, input_symbol)
+            yield current_states
 
-    def _compute_reachable_states(self):
-        """Compute the states which are reachable from the initial state."""
-        visited_set = set()
-        queue = deque()
+        self._check_for_input_rejection(current_states)
 
-        queue.append(self.initial_state)
-        visited_set.add(self.initial_state)
+    @staticmethod
+    def _get_state_maps(
+        state_set_a: AbstractSet[NFAStateT],
+        state_set_b: AbstractSet[NFAStateT],
+        *,
+        start: int = 0,
+    ) -> Tuple[Dict[NFAStateT, int], Dict[NFAStateT, int]]:
+        """
+        Generate state map dicts from given sets. Useful when the state set has
+        to be a union of the state sets of component FAs.
+        """
 
-        while queue:
-            state = queue.popleft()
+        state_name_counter = count(start)
 
-            for next_state in self.transitions[state].values():
-                if next_state not in visited_set:
-                    visited_set.add(next_state)
-                    queue.append(next_state)
+        state_map_a = dict(zip(state_set_a, state_name_counter))
+        state_map_b = dict(zip(state_set_b, state_name_counter))
 
-        return visited_set
+        return (state_map_a, state_map_b)
 
-    def minify(self, retain_names=False):
+    def union(self, other: NFA) -> Self:
         """
-        Create a minimal DFA which accepts the same inputs as this DFA.
-
-        First, non-reachable states are removed.
-        Then, similiar states are merged using Hopcroft's Algorithm.
-            retain_names: If True, merged states retain names.
-                          If False, new states will be named 0, ..., n-1.
+        Given two NFAs, M1 and M2, which accept the languages
+        L1 and L2 respectively, returns an NFA which accepts
+        the union of L1 and L2.
         """
 
-        # Compute reachable states and final states
-        reachable_states = self._compute_reachable_states()
-        reachable_final_states = self.final_states & reachable_states
+        # Starting at 1 because 0 is for the initial state
+        (state_map_a, state_map_b) = self.__class__._get_state_maps(
+            self.states, other.states, start=1
+        )
 
-        return self._minify(
-            reachable_states=reachable_states,
-            input_symbols=self.input_symbols,
-            transitions=self.transitions,
-            initial_state=self.initial_state,
-            reachable_final_states=reachable_final_states,
-            retain_names=retain_names)
+        new_states = frozenset(chain(state_map_a.values(), state_map_b.values(), [0]))
+        new_transitions: Dict[NFAStateT, Dict[str, Set[NFAStateT]]] = {
+            state: {} for state in new_states
+        }
 
-    @classmethod
-    def _minify(cls, *, reachable_states, input_symbols, transitions, initial_state,
-                reachable_final_states, retain_names):
-        """Minify helper function. DFA data passed in must have no unreachable states."""
-
-        # First, assemble backmap and equivalence class data structure
-        eq_classes = PartitionRefinement(reachable_states)
-        refinement = eq_classes.refine(reachable_final_states)
-
-        final_states_id = refinement[0][0] if refinement else next(iter(eq_classes.get_set_ids()))
-
-        transition_back_map = {
-            symbol: {
-                end_state: list()
-                for end_state in reachable_states
-            }
-            for symbol in input_symbols
+        # Connect new initial state to both branch
+        new_transitions[0] = {
+            "": {state_map_a[self.initial_state], state_map_b[other.initial_state]}
         }
 
-        for start_state, path in transitions.items():
-            if start_state in reachable_states:
-                for symbol, end_state in path.items():
-                    transition_back_map[symbol][end_state].append(start_state)
-
-        origin_dicts = tuple(transition_back_map.values())
-        processing = {final_states_id}
-
-        while processing:
-            # Save a copy of the set, since it could get modified while executing
-            active_state = tuple(eq_classes.get_set_by_id(processing.pop()))
-            for origin_dict in origin_dicts:
-                states_that_move_into_active_state = chain.from_iterable(
-                    origin_dict[end_state] for end_state in active_state
-                )
+        # Transitions of self
+        self.__class__._load_new_transition_dict(
+            state_map_a, self.transitions, new_transitions
+        )
+        # Transitions of other
+        self.__class__._load_new_transition_dict(
+            state_map_b, other.transitions, new_transitions
+        )
 
-                # Refine set partition by states moving into current active one
-                new_eq_class_pairs = eq_classes.refine(states_that_move_into_active_state)
+        # Final states
+        new_final_states = frozenset(
+            chain(
+                (state_map_a[state] for state in self.final_states),
+                (state_map_b[state] for state in other.final_states),
+            )
+        )
 
-                for (YintX_id, YdiffX_id) in new_eq_class_pairs:
-                    # Only adding one id to processing, since the other is already there
-                    if YdiffX_id in processing:
-                        processing.add(YintX_id)
-                    else:
-                        if len(eq_classes.get_set_by_id(YintX_id)) <= len(eq_classes.get_set_by_id(YdiffX_id)):
-                            processing.add(YintX_id)
-                        else:
-                            processing.add(YdiffX_id)
-
-        # now eq_classes are good to go, make them a list for ordering
-        eq_class_name_pairs = (
-            [(frozenset(eq), eq) for eq in eq_classes.get_sets()] if retain_names else
-            list(enumerate(eq_classes.get_sets()))
-        )
-
-        # need a backmap to prevent constant calls to index
-        back_map = {
-            state: name
-            for name, eq in eq_class_name_pairs
-            for state in eq
-        }
+        return self.__class__(
+            states=new_states,
+            input_symbols=self.input_symbols | other.input_symbols,
+            transitions=new_transitions,
+            initial_state=0,
+            final_states=new_final_states,
+        )
 
-        new_input_symbols = input_symbols
-        new_states = frozenset(back_map.values())
-        new_initial_state = back_map[initial_state]
-        new_final_states = frozenset(back_map[acc] for acc in reachable_final_states)
-        new_transitions = {
-            name: {
-                letter: back_map[transitions[next(iter(eq))][letter]]
-                for letter in input_symbols
-            }
-            for name, eq in eq_class_name_pairs
+    def concatenate(self, other: NFA) -> Self:
+        """
+        Given two NFAs, M1 and M2, which accept the languages
+        L1 and L2 respectively, returns an NFA which accepts
+        the languages L1 concatenated with L2.
+        """
+
+        (state_map_a, state_map_b) = self.__class__._get_state_maps(
+            self.states, other.states
+        )
+
+        new_states = frozenset(chain(state_map_a.values(), state_map_b.values()))
+        new_transitions: Dict[NFAStateT, Dict[str, Set[NFAStateT]]] = {
+            state: {} for state in new_states
         }
 
-        return cls(
+        # Transitions of self
+        self.__class__._load_new_transition_dict(
+            state_map_a, self.transitions, new_transitions
+        )
+        # Transitions of other
+        self.__class__._load_new_transition_dict(
+            state_map_b, other.transitions, new_transitions
+        )
+
+        # Transitions from self to other
+        for state in self.final_states:
+            new_transitions[state_map_a[state]].setdefault("", set()).add(
+                state_map_b[other.initial_state]
+            )
+
+        # Final states of other
+        new_final_states = frozenset(state_map_b[state] for state in other.final_states)
+
+        return self.__class__(
             states=new_states,
-            input_symbols=new_input_symbols,
+            input_symbols=self.input_symbols | other.input_symbols,
             transitions=new_transitions,
-            initial_state=new_initial_state,
+            initial_state=state_map_a[self.initial_state],
             final_states=new_final_states,
         )
 
-    def union(self, other, *, retain_names=False, minify=True):
+    def kleene_star(self) -> Self:
         """
-        Takes as input two DFAs M1 and M2 which
-        accept languages L1 and L2 respectively.
-        Returns a DFA which accepts the union of L1 and L2.
-        """
-
-        def union_function(state_pair):
-            q_a, q_b = state_pair
-            return q_a in self.final_states or q_b in other.final_states
-
-        new_states, new_transitions, new_initial_state, new_final_states = self._cross_product(
-            other,
-            union_function,
-            should_construct_dfa=True,
-            retain_names=retain_names
-        )
-
-        if minify:
-            return self._minify(
-                reachable_states=new_states,
-                input_symbols=self.input_symbols,
-                transitions=new_transitions,
-                initial_state=new_initial_state,
-                reachable_final_states=new_final_states,
-                retain_names=retain_names)
+        Given an NFA which accepts the language L returns
+        an NFA which accepts L repeated 0 or more times.
+        """
+        new_states = set(self.states)
+        new_initial_state = self.__class__._add_new_state(new_states)
+
+        # Transitions are the same with a few additions.
+        new_transitions: Dict[NFAStateT, Dict[str, Set[NFAStateT]]] = dict(
+            self.transitions
+        )
+        # We add epsilon transition from new initial state
+        # to old initial state
+        new_transitions[new_initial_state] = {"": {self.initial_state}}
+        # For each final state in original NFA we add epsilon
+        # transition to the old initial state
+        for state in self.final_states:
+            new_transitions[state] = dict(new_transitions.get(state, {}))
+            transition = new_transitions[state]
+            transition[""] = set(transition.get("", set()))
+            transition[""].add(self.initial_state)
 
         return self.__class__(
             states=new_states,
             input_symbols=self.input_symbols,
             transitions=new_transitions,
             initial_state=new_initial_state,
-            final_states=new_final_states
+            final_states=self.final_states | {new_initial_state},
         )
 
-    def intersection(self, other, *, retain_names=False, minify=True):
+    def option(self) -> Self:
         """
-        Takes as input two DFAs M1 and M2 which
-        accept languages L1 and L2 respectively.
-        Returns a DFA which accepts the intersection of L1 and L2.
+        Given an NFA which accepts the language L returns
+        an NFA which accepts L repeated 0 or 1 times. (option - ?)
+        Note: still you cannot pass empty string to the machine.
         """
+        new_states = set(self.states)
+        new_initial_state = self.__class__._add_new_state(new_states)
 
-        def intersection_function(state_pair):
-            q_a, q_b = state_pair
-            return q_a in self.final_states and q_b in other.final_states
+        # Transitions are the same with a few additions.
+        new_transitions = dict(self.transitions)
+        # We add epsilon transition from new initial state
+        # to old initial state
+        new_transitions[new_initial_state] = {"": {self.initial_state}}
 
-        new_states, new_transitions, new_initial_state, new_final_states = self._cross_product(
-            other,
-            intersection_function,
-            should_construct_dfa=True,
-            retain_names=retain_names
+        return self.__class__(
+            states=new_states,
+            input_symbols=self.input_symbols,
+            transitions=new_transitions,
+            initial_state=new_initial_state,
+            final_states=self.final_states | {new_initial_state},
         )
 
-        if minify:
-            return self._minify(
-                reachable_states=new_states,
-                input_symbols=self.input_symbols,
-                transitions=new_transitions,
-                initial_state=new_initial_state,
-                reachable_final_states=new_final_states,
-                retain_names=retain_names)
+    def reverse(self) -> Self:
+        """
+        Given an NFA which accepts the language L this function
+        returns an NFA which accepts the reverse of L.
+        """
+        new_states = set(self.states)
+        new_initial_state = self.__class__._add_new_state(new_states)
+
+        # Transitions are the same except reversed
+        new_transitions: Dict[NFAStateT, Dict[str, Set[NFAStateT]]] = {
+            state: {} for state in new_states
+        }
+
+        for state_a, transitions in self.transitions.items():
+            for symbol, states in transitions.items():
+                for state_b in states:
+                    new_transitions[state_b].setdefault(symbol, set()).add(state_a)
+
+        # And we additionally have epsilon transitions from
+        # new initial state to each old final state.
+        new_transitions[new_initial_state][""] = set(self.final_states)
+        new_final_states = {self.initial_state}
 
         return self.__class__(
             states=new_states,
             input_symbols=self.input_symbols,
             transitions=new_transitions,
             initial_state=new_initial_state,
-            final_states=new_final_states
+            final_states=new_final_states,
         )
 
-    def difference(self, other, *, retain_names=False, minify=True):
+    def intersection(self, other: NFA) -> Self:
         """
-        Takes as input two DFAs M1 and M2 which
-        accept languages L1 and L2 respectively.
-        Returns a DFA which accepts the difference of L1 and L2.
+        Given two NFAs, M1 and M2, which accept the languages
+        L1 and L2 respectively, returns an NFA which accepts
+        the intersection of L1 and L2.
         """
 
-        def difference_function(state_pair):
-            q_a, q_b = state_pair
-            return q_a in self.final_states and q_b not in other.final_states
+        new_states = set()
+        new_input_symbols = self.input_symbols | other.input_symbols
+        new_transitions: Dict[NFAStateT, Dict[str, Set[NFAStateT]]] = {}
+        new_initial_state = (self.initial_state, other.initial_state)
 
-        new_states, new_transitions, new_initial_state, new_final_states = self._cross_product(
-            other,
-            difference_function,
-            should_construct_dfa=True,
-            retain_names=retain_names
-        )
+        queue: Deque[NFAStateT] = deque()
+
+        queue.append(new_initial_state)
+        new_states.add(new_initial_state)
+
+        while queue:
+            curr_state = queue.popleft()
+            q_a, q_b = curr_state
+
+            # States we will consider adding to the queue
+            next_states_iterables: List[Iterable[NFAStateT]] = list()
+
+            # Get transition dict for states in self
+            transitions_a = self.transitions.get(q_a, {})
+            # Add epsilon transitions for first set of transitions
+            epsilon_transitions_a = transitions_a.get("")
+            if epsilon_transitions_a is not None:
+                state_dict = new_transitions.setdefault(curr_state, {})
+                state_dict.setdefault("", set()).update(
+                    zip(epsilon_transitions_a, repeat(q_b))
+                )
+                next_states_iterables.append(zip(epsilon_transitions_a, repeat(q_b)))
 
-        if minify:
-            return self._minify(
-                reachable_states=new_states,
-                input_symbols=self.input_symbols,
-                transitions=new_transitions,
-                initial_state=new_initial_state,
-                reachable_final_states=new_final_states,
-                retain_names=retain_names)
+            # Get transition dict for states in other
+            transitions_b = other.transitions.get(q_b, {})
+            # Add epsilon transitions for second set of transitions
+            epsilon_transitions_b = transitions_b.get("")
+            if epsilon_transitions_b is not None:
+                state_dict = new_transitions.setdefault(curr_state, {})
+                state_dict.setdefault("", set()).update(
+                    zip(repeat(q_a), epsilon_transitions_b)
+                )
+                next_states_iterables.append(zip(repeat(q_a), epsilon_transitions_b))
+
+            # Add all transitions moving over same input symbols
+            for symbol in new_input_symbols:
+                end_states_a = transitions_a.get(symbol)
+                end_states_b = transitions_b.get(symbol)
+
+                if end_states_a is not None and end_states_b is not None:
+                    state_dict = new_transitions.setdefault(curr_state, {})
+                    state_dict.setdefault(symbol, set()).update(
+                        product(end_states_a, end_states_b)
+                    )
+                    next_states_iterables.append(product(end_states_a, end_states_b))
+
+            # Finally, try visiting every state we found.
+            for product_state in chain.from_iterable(next_states_iterables):
+                if product_state not in new_states:
+                    new_states.add(product_state)
+                    queue.append(product_state)
+
+        new_final_states = frozenset(
+            (state_a, state_b)
+            for (state_a, state_b) in new_states
+            if state_a in self.final_states and state_b in other.final_states
+        )
 
         return self.__class__(
             states=new_states,
-            input_symbols=self.input_symbols,
+            input_symbols=new_input_symbols,
             transitions=new_transitions,
             initial_state=new_initial_state,
-            final_states=new_final_states
+            final_states=new_final_states,
         )
 
-    def symmetric_difference(self, other, *, retain_names=False, minify=True):
+    def shuffle_product(self, other: NFA) -> Self:
         """
-        Takes as input two DFAs M1 and M2 which
-        accept languages L1 and L2 respectively.
-        Returns a DFA which accepts the symmetric difference of L1 and L2.
+        Given two NFAs, M1 and M2, which accept the languages
+        L1 and L2 respectively, returns an NFA which accepts
+        the shuffle of L1 and L2.
         """
+        if not isinstance(other, NFA):
+            raise TypeError(f"other must be an NFA, not {other.__class__.__name__}")
 
-        def symmetric_difference_function(state_pair):
-            q_a, q_b = state_pair
-            return (q_a in self.final_states) ^ (q_b in other.final_states)
+        new_input_symbols = self.input_symbols | other.input_symbols
+        new_initial_state = (self.initial_state, other.initial_state)
+        new_states = frozenset(product(self.states, other.states))
 
-        new_states, new_transitions, new_initial_state, new_final_states = self._cross_product(
-            other,
-            symmetric_difference_function,
-            should_construct_dfa=True,
-            retain_names=retain_names
-        )
+        new_transitions: Dict[NFAStateT, Dict[str, Set[NFAStateT]]] = {}
+
+        for curr_state in new_states:
+            state_dict = new_transitions.setdefault(curr_state, {})
+            q_a, q_b = curr_state
 
-        if minify:
-            return self._minify(
-                reachable_states=new_states,
-                input_symbols=self.input_symbols,
-                transitions=new_transitions,
-                initial_state=new_initial_state,
-                reachable_final_states=new_final_states,
-                retain_names=retain_names)
+            transitions_a = self.transitions.get(q_a, {})
+            for symbol, end_states in transitions_a.items():
+                state_dict.setdefault(symbol, set()).update(
+                    zip(end_states, repeat(q_b))
+                )
+
+            transitions_b = other.transitions.get(q_b, {})
+            for symbol, end_states in transitions_b.items():
+                state_dict.setdefault(symbol, set()).update(
+                    zip(repeat(q_a), end_states)
+                )
 
         return self.__class__(
             states=new_states,
-            input_symbols=self.input_symbols,
+            input_symbols=new_input_symbols,
             transitions=new_transitions,
             initial_state=new_initial_state,
-            final_states=new_final_states
+            final_states=frozenset(product(self.final_states, other.final_states)),
+        )
+
+    def right_quotient(self, other: NFA) -> Self:
+        """
+        Given two NFAs, M1 and M2, which accept the languages
+        L1 and L2 respectively, returns an NFA which accepts
+        the right quotient of L1 with respect to L2 (L1 / L2).
+
+        Construction is based off of the one described here:
+        https://cs.stackexchange.com/a/102043
+        """
+
+        if not isinstance(other, NFA):
+            raise TypeError(f"other must be an NFA, not {other.__class__.__name__}")
+
+        # First, eliminate lambdas because they cause problems with this algorithm
+        (
+            self_reachable_states,
+            self_new_transitions,
+            self_reachable_final_states,
+        ) = self._eliminate_lambda()
+        (
+            other_reachable_states,
+            other_new_transitions,
+            other_reachable_final_states,
+        ) = other._eliminate_lambda()
+
+        new_input_symbols = self.input_symbols | other.input_symbols
+        new_initial_state = (self.initial_state, other.initial_state, False)
+        new_final_states = frozenset(
+            product(self_reachable_final_states, other_reachable_final_states, [True])
+        )
+        new_states = frozenset(
+            chain(
+                product(self_reachable_states, [other.initial_state], [False]),
+                product(self_reachable_states, other_reachable_states, [True]),
+            )
         )
 
-    def complement(self, *, retain_names=False, minify=True):
-        """Return the complement of this DFA."""
+        new_transitions: Dict[NFAStateT, Dict[str, Set[NFAStateT]]] = {}
 
-        if minify:
-            reachable_states = self._compute_reachable_states()
-            reachable_final_states = self.final_states & reachable_states
-
-            return self._minify(
-                reachable_states=reachable_states,
-                input_symbols=self.input_symbols,
-                transitions=self.transitions,
-                initial_state=self.initial_state,
-                reachable_final_states=reachable_states - reachable_final_states,
-                retain_names=retain_names)
+        # Populate transitions for before reading the suffix
+        for state in self_reachable_states:
+            new_state = (state, other.initial_state, False)
+            new_state_dict = new_transitions.setdefault(new_state, {})
+            old_transitions_dict = self_new_transitions.get(state)
+
+            if old_transitions_dict:
+                for symbol, end_states in old_transitions_dict.items():
+                    new_state_dict[symbol] = {
+                        (end_state, other.initial_state, False)
+                        for end_state in end_states
+                    }
+
+            new_state_dict[""] = {(state, other.initial_state, True)}
+
+        # Start reading after the suffix
+        for q_a, q_b in product(self_reachable_states, other_reachable_states):
+            curr_state = (q_a, q_b, True)
+
+            transitions_a = self_new_transitions.get(q_a, {})
+            transitions_b = other_new_transitions.get(q_b, {})
+
+            # Add all transitions moving over same input symbols
+            for symbol in new_input_symbols:
+                end_states_a = transitions_a.get(symbol)
+                end_states_b = transitions_b.get(symbol)
+
+                if end_states_a is not None and end_states_b is not None:
+                    state_dict = new_transitions.setdefault(curr_state, {})
+                    state_dict.setdefault("", set()).update(
+                        product(end_states_a, end_states_b, [True])
+                    )
 
         return self.__class__(
-            states=self.states,
-            input_symbols=self.input_symbols,
-            transitions=self.transitions,
-            initial_state=self.initial_state,
-            final_states=self.states - self.final_states,
-            allow_partial=self.allow_partial
+            states=new_states,
+            input_symbols=new_input_symbols,
+            transitions=new_transitions,
+            initial_state=new_initial_state,
+            final_states=new_final_states,
         )
 
-    def _cross_product(self, other, state_target_fn, *, should_construct_dfa, retain_names=False):
+    def left_quotient(self, other: NFA) -> Self:
         """
-        Search reachable states corresponding to product graph between self and other.
+        Given two NFAs, M1 and M2, which accept the languages
+        L1 and L2 respectively, returns an NFA which accepts
+        the left quotient of L1 with respect to L2 (L2 \\ L1).
+
+        Construction is based off of the one described here:
+        https://cs.stackexchange.com/a/102043
+        """
+
+        if not isinstance(other, NFA):
+            raise TypeError(f"other must be an NFA, not {other.__class__.__name__}")
+
+        # First, eliminate lambdas because they cause problems with this algorithm
+        (
+            self_reachable_states,
+            self_new_transitions,
+            self_reachable_final_states,
+        ) = self._eliminate_lambda()
+        (
+            other_reachable_states,
+            other_new_transitions,
+            other_reachable_final_states,
+        ) = other._eliminate_lambda()
+
+        new_input_symbols = self.input_symbols | other.input_symbols
+        new_initial_state = (self.initial_state, other.initial_state, False)
+        new_final_states = frozenset(
+            product(self_reachable_final_states, other_reachable_final_states, [True])
+        )
+        new_states = frozenset(
+            chain(
+                product(self_reachable_states, other_reachable_states, [False]),
+                product(self_reachable_states, other_reachable_final_states, [True]),
+            )
+        )
 
-        The function state_target_fn should return True for states that should be
-        final (when the new DFA is being constructed explicitly) or for states that
-        are being searched for (if the DFA is not being constructed).
+        new_transitions: Dict[NFAStateT, Dict[str, Set[NFAStateT]]] = {}
 
-        If should_construct_dfa is False, then this function returns a boolean corresponding
-        to whether any target states are reachable. Otherwise, constructs the given DFA. If
-        retain_names is set to False, states are renamed.
-        """
-        if self.input_symbols != other.input_symbols:
-            raise exceptions.SymbolMismatchError('The input symbols between the two given DFAs do not match')
+        # Start reading the prefix
+        for q_a, q_b in product(self_reachable_states, other_reachable_states):
+            curr_state = (q_a, q_b, False)
+
+            transitions_a = self_new_transitions.get(q_a, {})
+            transitions_b = other_new_transitions.get(q_b, {})
+
+            # Add all transitions moving over same input symbols
+            for symbol in new_input_symbols:
+                end_states_a = transitions_a.get(symbol)
+                end_states_b = transitions_b.get(symbol)
+
+                if end_states_a is not None and end_states_b is not None:
+                    state_dict = new_transitions.setdefault(curr_state, {})
+                    state_dict.setdefault("", set()).update(
+                        product(end_states_a, end_states_b, [False])
+                    )
+
+            # Add lambda transition from final state, flipping third entry to true
+            if q_b in other_reachable_final_states:
+                state_dict = new_transitions.setdefault(curr_state, {})
+                state_dict.setdefault("", set()).add((q_a, q_b, True))
+
+        # Populate transitions for after reading the prefix
+        for state_a, state_b in product(
+            self_reachable_states, other_reachable_final_states
+        ):
+            new_state = (state_a, state_b, True)
+            new_state_dict = new_transitions.setdefault(new_state, {})
+            old_transitions_dict = self_new_transitions.get(state_a)
+
+            if old_transitions_dict:
+                for symbol, end_states in old_transitions_dict.items():
+                    new_state_dict[symbol] = set(
+                        zip(end_states, repeat(state_b), repeat(True))
+                    )
+
+        return self.__class__(
+            states=new_states,
+            input_symbols=new_input_symbols,
+            transitions=new_transitions,
+            initial_state=new_initial_state,
+            final_states=new_final_states,
+        )
 
-        def get_name_original(state):
-            return state
+    @staticmethod
+    def _load_new_transition_dict(
+        state_map_dict: Mapping[NFAStateT, NFAStateT],
+        old_transition_dict: NFATransitionsT,
+        new_transition_dict: Dict[NFAStateT, Dict[str, Set[NFAStateT]]],
+    ) -> None:
+        """
+        Load the new_transition_dict with the old transitions corresponding to
+        the given state_map_dict.
+        """
 
-        get_name = get_name_original if retain_names else get_renaming_function(count(0))
+        for state_a, transitions in old_transition_dict.items():
+            for symbol, states in transitions.items():
+                new_transition_dict[state_map_dict[state_a]][symbol] = {
+                    state_map_dict[state_b] for state_b in states
+                }
 
-        product_transitions = {} if should_construct_dfa else None
-        final_states = set() if should_construct_dfa else None
+    def __eq__(self, other: Any) -> bool:
+        """
+        Return True if two NFAs are equivalent. Uses an optimized version of
+        the extended Hopcroft-Karp algorithm (HKe). See
+        https://arxiv.org/abs/0907.5058
+        """
 
-        visited_set = set()
-        queue = deque()
+        NFAStatesPairT = Tuple[FrozenSet[NFAStateT], int]
 
-        product_initial_state = (self.initial_state, other.initial_state)
-        product_initial_state_name = get_name(product_initial_state)
+        # Must be another NFA and have equal alphabets
+        if not isinstance(other, NFA) or self.input_symbols != other.input_symbols:
+            return NotImplemented
 
-        queue.append(product_initial_state)
-        visited_set.add(product_initial_state_name)
+        operand_nfas = (self, other)
+        initial_state_a = (self._get_lambda_closures()[self.initial_state], 0)
+        initial_state_b = (other._get_lambda_closures()[other.initial_state], 1)
+
+        def is_final_state(states_pair: NFAStatesPairT) -> bool:
+            states, operand_index = states_pair
+            nfa = operand_nfas[operand_index]
+            # If at least one of the current states is a final state, the
+            # condition should satisfy
+            return any(
+                not nfa.final_states.isdisjoint(nfa._get_lambda_closures()[state])
+                for state in states
+            )
 
-        while queue:
-            # Get next state in BFS queue
-            curr_state = queue.popleft()
+        def transition(states_pair: NFAStatesPairT, symbol: str) -> NFAStatesPairT:
+            states, operand_index = states_pair
+            return (
+                operand_nfas[operand_index]._get_next_current_states(states, symbol),
+                operand_index,
+            )
 
-            # Add state to the transition dict if constructing DFA
-            if should_construct_dfa:
-                curr_state_name = get_name(curr_state)
-                state_transitions = product_transitions.setdefault(curr_state_name, {})
-
-                if state_target_fn(curr_state):
-                    final_states.add(curr_state_name)
-
-            # Otherwise, just check the target function
-            elif state_target_fn(curr_state):
-                return True
+        # Get data structures
+        state_sets = nx.utils.union_find.UnionFind([initial_state_a, initial_state_b])
+        pair_stack: Deque[Tuple[NFAStatesPairT, NFAStatesPairT]] = deque()
 
-            # Unpack state and get transitions
-            q_a, q_b = curr_state
-            transitions_a = self.transitions[q_a]
-            transitions_b = other.transitions[q_b]
+        # Do union find
+        state_sets.union(initial_state_a, initial_state_b)
+        pair_stack.append((initial_state_a, initial_state_b))
 
-            for chr in self.input_symbols:
-                product_state = (transitions_a[chr], transitions_b[chr])
-                product_state_name = get_name(product_state)
-
-                if should_construct_dfa:
-                    state_transitions[chr] = product_state_name
-
-                # If next state is new, add to queue
-                if product_state_name not in visited_set:
-                    visited_set.add(product_state_name)
-                    queue.append(product_state)
+        while pair_stack:
+            q_a, q_b = pair_stack.pop()
 
-        if should_construct_dfa:
-            return visited_set, product_transitions, product_initial_state_name, final_states
+            if is_final_state(q_a) ^ is_final_state(q_b):
+                return False
 
-        return False
+            for symbol in self.input_symbols:
+                r_1 = state_sets[transition(q_a, symbol)]
+                r_2 = state_sets[transition(q_b, symbol)]
 
-    def issubset(self, other):
-        """Return True if this DFA is a subset of another DFA."""
+                if r_1 != r_2:
+                    state_sets.union(r_1, r_2)
+                    pair_stack.append((r_1, r_2))
 
-        def subset_state_fn(state_pair):
-            """Check for reachable state that is counterexample to subset"""
-            q_a, q_b = state_pair
-            return q_a in self.final_states and q_b not in other.final_states
-
-        return not self._cross_product(other, subset_state_fn, should_construct_dfa=False)
-
-    def issuperset(self, other):
-        """Return True if this DFA is a superset of another DFA."""
-        return other.issubset(self)
-
-    def isdisjoint(self, other):
-        """Return True if this DFA has no common elements with another DFA."""
-
-        def disjoint_state_fn(state_pair):
-            """Check for reachable state that is counterexample to disjointness"""
-            q_a, q_b = state_pair
-            return q_a in self.final_states and q_b in other.final_states
-
-        return not self._cross_product(other, disjoint_state_fn, should_construct_dfa=False)
-
-    def isempty(self):
-        """Return True if this DFA is completely empty."""
-        return len(self._compute_reachable_states() & self.final_states) == 0
-
-    def isfinite(self):
-        """
-        Returns True if the DFA accepts a finite language, False otherwise.
-        """
-        try:
-            return self.maximum_word_length() is not None
-        except exceptions.EmptyLanguageException:
-            return True
-
-    def random_word(self, k, *, seed=None):
-        self._populate_count_cache_up_to_len(k)
-        state = self.initial_state
-        if self._count_cache[k][state] == 0:
-            raise ValueError(f"Language has no words of length {k}")
-
-        result = []
-        rng = Random(seed)
-        for remaining in range(k, 0, -1):
-            total = self._count_cache[remaining][state]
-            choice = rng.randint(0, total-1)
-            for symbol, next_state in self.transitions[state].items():  # pragma: no branch
-                next_state_count = self._count_cache[remaining - 1][next_state]
-                if choice < next_state_count:
-                    result.append(symbol)
-                    state = next_state
-                    break
-                choice -= next_state_count
-
-        assert state in self.final_states
-        return ''.join(result)
-
-    def predecessor(self, input_str, *, strict=True, key=None):
-        """
-        Returns the first string accepted by the DFA that comes before
-        the input string in lexicographical order.
-        Passing in None will generate the lexicographically last word.
-        If strict is set to False and input_str is accepted by the DFA then
-        it will be returned.
-        The value of key can be set to define a custom lexicographical ordering.
-        """
-        for word in self.predecessors(input_str, strict=strict, key=key):
-            return word
-        return None
-
-    def predecessors(self, input_str, *, strict=True, key=None):
-        """
-        Generates all strings that come before the input string
-        in lexicographical order.
-        Passing in None will generate all words.
-        If strict is set to False and input_str is accepted by the DFA then
-        it will be included in the output.
-        The value of key can be set to define a custom lexicographical ordering.
-        Raises an InfiniteLanguageException for infinite languages.
-        """
-        yield from self.successors(input_str, strict=strict, reverse=True, key=key)
-
-    def successor(self, input_str, *, strict=True, key=None):
-        """
-        Returns the first string accepted by the DFA that comes after
-        the input string in lexicographical order.
-        Passing in None will generate the lexicographically first word.
-        If strict is set to False and input_str is accepted by the DFA then
-        it will be returned.
-        The value of key can be set to define a custom lexicographical ordering.
-        """
-        for word in self.successors(input_str, strict=strict, key=key):
-            return word
-        return None
-
-    def successors(self, input_str, *, strict=True, key=None, reverse=False):
-        """
-        Generates all strings that come after the input string
-        in lexicographical order.
-        Passing in None will generate all words.
-        If strict is set to False and input_str is accepted by the DFA then
-        it will be included in the output.
-        If reverse is set to True then predecessors will be generated instead. See the DFA.predecessors method.
-        The value of key can be set to define a custom lexicographical ordering.
-        """
-        # A predecessor for a finite string may be infinite but a successor for a finite string is always finite
-        if reverse and not self.isfinite():
-            raise exceptions.InfiniteLanguageException('Predecessors cannot be computed for infinite languages')
-        graph = self._get_digraph()
-        coaccessible_nodes = self.final_states.union(*(
-            nx.ancestors(graph, state)
-            for state in self.final_states
-        ))
-
-        # Precomputations and setup
-        include_input = not strict
-        sorted_symbols = sorted(self.input_symbols, reverse=reverse, key=key)
-        symbol_succ = {symbol_a: symbol_b
-                       for symbol_a, symbol_b in zip(sorted_symbols, sorted_symbols[1:])}
-        symbol_succ[sorted_symbols[-1]] = None
-        # Special case for None
-        state_stack = deque([self.initial_state]
-                            if input_str is None
-                            else self.read_input_stepwise(input_str, ignore_rejection=True))
-        char_stack = [] if input_str is None else list(input_str)
-        first_symbol = sorted_symbols[0]
-        # For predecessors we need to special case the input string None
-        candidate = None if reverse and input_str is not None else first_symbol
-        # If input_str is None then we yield on first value found no matter the value of include_input
-        should_yield = include_input or input_str is None
-
-        # Iterative preorder/postorder (depends on reverse) traversal that yields on final states
-        while char_stack or candidate is not None:
-            state = state_stack[-1]
-            # Successors yield here
-            if not reverse and should_yield and candidate == first_symbol and state in self.final_states:
-                yield ''.join(char_stack)
-            candidate_state = None if candidate is None else self._get_next_current_state(state, candidate)
-            # Traverse to child if candidate is viable
-            if candidate_state in coaccessible_nodes:
-                state_stack.append(candidate_state)
-                char_stack.append(candidate)
-                candidate = first_symbol
-            else:
-                # Predecessors yield here
-                if reverse and should_yield and candidate is None and state in self.final_states:
-                    yield ''.join(char_stack)
-                # Candidate is None means no more children to explore, so traverse to parent
-                if candidate is None:
-                    state = state_stack.pop()
-                    candidate = char_stack.pop()
-                candidate = symbol_succ[candidate]
-            should_yield = True
-        # Predecessor yields here for empty string
-        if reverse and should_yield and candidate is None and state in self.final_states:
-            yield ''.join(char_stack)
-
-    def count_words_of_length(self, k):
-        """
-        Counts words of length `k` accepted by the DFA
-        """
-        self._populate_count_cache_up_to_len(k)
-        return self._count_cache[k][self.initial_state]
-
-    def _populate_count_cache_up_to_len(self, k):
-        """
-        Populate count cache up to length k
-        """
-        while len(self._count_cache) <= k:
-            i = len(self._count_cache)
-            self._count_cache.append(defaultdict(int))
-            level = self._count_cache[i]
-            if i == 0:
-                level.update({state: 1 for state in self.final_states})
-            else:
-                prev_level = self._count_cache[i-1]
-                level.update({
-                    state: sum(prev_level[suffix_state] for suffix_state in self.transitions[state].values())
-                    for state in self.states
-                })
-
-    def words_of_length(self, k):
-        """
-        Generates all words of size k in the language represented by the DFA
-        """
-        self._populate_word_cache_up_to_len(k)
-        for word in self._word_cache[k][self.initial_state]:
-            yield word
-
-    def _populate_word_cache_up_to_len(self, k):
-        """
-        Populate word cache up to length k
-        """
-        sorted_symbols = sorted(self.input_symbols)
-        while len(self._word_cache) <= k:
-            i = len(self._word_cache)
-            self._word_cache.append(defaultdict(list))
-            level = self._word_cache[i]
-            if i == 0:
-                level.update({state: [''] for state in self.final_states})
-            else:
-                prev_level = self._word_cache[i-1]
-                level.update({
-                    state: [symbol+word
-                            for symbol in sorted_symbols
-                            for word in prev_level[self.transitions[state][symbol]]]
-                    for state in self.states
-                })
-
-    def cardinality(self):
-        """Returns the cardinality of the language represented by the DFA."""
-        try:
-            i = self.minimum_word_length()
-        except exceptions.EmptyLanguageException:
-            return 0
-        limit = self.maximum_word_length()
-        if limit is None:
-            raise exceptions.InfiniteLanguageException("The language represented by the DFA is infinite.")
-        return sum(self.count_words_of_length(j) for j in range(i, limit+1))
-
-    def minimum_word_length(self):
-        """
-        Returns the length of the shortest word in the language represented by the DFA
-        """
-        queue = deque()
-        distances = defaultdict(lambda: None)
-        distances[self.initial_state] = 0
-        queue.append(self.initial_state)
-        while queue:
-            state = queue.popleft()
-            if state in self.final_states:
-                return distances[state]
-            for next_state in self.transitions[state].values():
-                if distances[next_state] is None:
-                    distances[next_state] = distances[state] + 1
-                    queue.append(next_state)
-        raise exceptions.EmptyLanguageException('The language represented by the DFA is empty')
-
-    def maximum_word_length(self):
-        """
-        Returns the length of the longest word in the language represented by the DFA
-        In the case of infinite languages, `None` is returned
-        """
-        if self.isempty():
-            raise exceptions.EmptyLanguageException('The language represented by the DFA is empty')
-        graph = self._get_digraph()
-
-        accessible_nodes = nx.descendants(graph, self.initial_state) | {self.initial_state}
-
-        coaccessible_nodes = self.final_states.union(*(
-            nx.ancestors(graph, state)
-            for state in self.final_states
-        ))
-
-        important_nodes = accessible_nodes.intersection(coaccessible_nodes)
-        subgraph = graph.subgraph(important_nodes)
-        try:
-            return nx.dag_longest_path_length(subgraph)
-        except nx.exception.NetworkXUnfeasible:
-            return None
+        return True
 
     @classmethod
-    def from_prefix(cls, input_symbols, prefix, *, contains=True):
-        """
-        Directly computes the minimal DFA recognizing strings with the
-        given prefix.
-        If contains is set to False then the complement is constructed instead.
-        """
-        err_state = -1
-        last_state = len(prefix)
-        transitions = {i: {symbol: i+1 if symbol == char else err_state
-                           for symbol in input_symbols}
-                       for i, char in enumerate(prefix)}
-        transitions[last_state] = {symbol: last_state for symbol in input_symbols}
-        transitions[err_state] = {symbol: err_state for symbol in input_symbols}
+    def edit_distance(
+        cls: Type[Self],
+        input_symbols: AbstractSet[str],
+        reference_str: str,
+        max_edit_distance: int,
+        *,
+        insertion: bool = True,
+        deletion: bool = True,
+        substitution: bool = True,
+    ) -> Self:
+        """
+        Constructs the Levenshtein NFA for the given reference_str and given
+        Levenshtein distance. This NFA recognizes strings within the given
+        Levenshtein distance (commonly called edit distance) of the
+        reference_str. Parameters control which error types the NFA will
+        recognize (insertions, deletions, or substitutions). At least one error
+        type must be set.
+
+        If insertion and deletion are False and substitution is True, then this
+        is the same as Hamming distance.
+
+        If insertion and deletion are True and substitution is False, then this
+        is the same as LCS distance.
+
+        insertion, deletion, and substitution all default to True.
+
+        Code adapted from:
+        http://blog.notdot.net/2010/07/Damn-Cool-Algorithms-Levenshtein-Automata
+        """
+        if max_edit_distance < 0:
+            raise ValueError("max_edit_distance must be greater than zero")
+        if not (insertion or deletion or substitution):
+            raise ValueError(
+                "At least one of insertion, deletion, or substitution must be enabled."
+            )
 
-        states = frozenset(transitions.keys())
-        final_states = {last_state}
-        return cls(
-            states=states,
-            input_symbols=input_symbols,
-            transitions=transitions,
-            initial_state=0,
-            final_states=final_states if contains else states - final_states
+        states = frozenset(
+            product(range(len(reference_str) + 1), range(max_edit_distance + 1))
         )
 
-    @classmethod
-    def from_suffix(cls, input_symbols, suffix, *, contains=True):
-        """
-        Directly computes the minimal DFA recognizing strings with the
-        given prefix.
-        If contains is set to False then the complement is constructed instead.
-        """
-        return cls.from_substring(input_symbols, suffix, contains=contains, must_be_suffix=True)
-
-    @classmethod
-    def from_substring(cls, input_symbols, substring, *, contains=True, must_be_suffix=False):
-        """
-        Directly computes the minimal DFA recognizing strings containing the
-        given substring.
-        If contains is set to False then the complement is constructed instead.
-        If must_be_suffix is set to True, then the substring must be a suffix instead.
-        """
-        transitions = {i: {} for i in range(len(substring))}
-        transitions[len(substring)] = {
-            symbol: len(substring) for symbol in input_symbols
-        }
+        transitions: Dict[NFAStateT, Dict[str, Set[NFAStateT]]] = {}
+        final_states = set()
 
-        # Computing failure function for partial matches as is done in the
-        # Knuth-Morris-Pratt string algorithm so we can quickly compute the
-        # next state from another state
-        kmp_table = [-1 for _ in substring]
-        candidate = 0
-        for i, char in enumerate(substring):
-            if i == 0:
-                continue
-            elif char == substring[candidate]:
-                kmp_table[i] = kmp_table[candidate]
-            else:
-                kmp_table[i] = candidate
-                while candidate >= 0 and char != substring[candidate]:
-                    candidate = kmp_table[candidate]
-            candidate += 1
-        kmp_table.append(candidate)
-
-        limit = len(substring)+1 if must_be_suffix else len(substring)
-        for i in range(limit):
-            prefix_dict = transitions.setdefault(i, {})
+        def add_transition(
+            start_state_dict: Dict[str, Set[NFAStateT]],
+            end_state: NFAStateT,
+            symbol: str,
+        ) -> None:
+            """Add transition between start and end state on symbol"""
+            start_state_dict.setdefault(symbol, set()).add(end_state)
+
+        def add_any_transition(
+            start_state_dict: Dict[str, Set[NFAStateT]], end_state: NFAStateT
+        ) -> None:
+            """Add transition on all symbols between start and end state"""
             for symbol in input_symbols:
-                # Look for next state after reading in the given input symbol
-                candidate = i if i < len(substring) else kmp_table[i]
-                while candidate != -1 and substring[candidate] != symbol:
-                    candidate = kmp_table[candidate]
-                candidate += 1
-                prefix_dict[symbol] = candidate
-
-        states = frozenset(transitions.keys())
-        final_states = {len(substring)}
-        return cls(
-            states=states,
-            input_symbols=input_symbols,
-            transitions=transitions,
-            initial_state=0,
-            final_states=final_states if contains else states - final_states,
-        )
+                add_transition(start_state_dict, end_state, symbol)
 
-    @classmethod
-    def from_subsequence(cls, input_symbols, subsequence, *, contains=True):
-        """
-        Directly computes the minimal DFA recognizing strings containing the
-        given subsequence.
-        If contains is set to False then the complement is constructed instead.
-        """
-        transitions = {0: {symbol: 0 for symbol in input_symbols}}
+        for (i, symbol), e in product(
+            enumerate(reference_str), range(max_edit_distance + 1)
+        ):
+            state_transition_dict = transitions.setdefault((i, e), {})
+
+            # Correct character
+            add_transition(state_transition_dict, (i + 1, e), symbol)
+            if e < max_edit_distance:
+                if insertion:
+                    # Insertion
+                    add_any_transition(state_transition_dict, (i, e + 1))
+
+                if deletion:
+                    # Deletion
+                    add_transition(state_transition_dict, (i + 1, e + 1), "")
+
+                if substitution:
+                    # Substitution
+                    add_any_transition(state_transition_dict, (i + 1, e + 1))
+
+        for e in range(max_edit_distance + 1):
+            state_transition_dict = transitions.setdefault((len(reference_str), e), {})
+            if insertion and e < max_edit_distance:
+                add_any_transition(state_transition_dict, (len(reference_str), e + 1))
 
-        for prev_state, char in enumerate(subsequence):
-            next_state = prev_state + 1
-            transitions[next_state] = {symbol: next_state for symbol in input_symbols}
-            transitions[prev_state][char] = next_state
+            final_states.add((len(reference_str), e))
 
-        states = frozenset(transitions.keys())
-        final_states = {len(subsequence)}
         return cls(
             states=states,
             input_symbols=input_symbols,
             transitions=transitions,
-            initial_state=0,
-            final_states=final_states if contains else states - final_states,
-        )
-
-    @classmethod
-    def of_length(cls, input_symbols, *, min_length=0, max_length=None, symbols_to_count=None):
-        """
-        Directly computes the minimal DFA recognizing strings whose length
-        is between `min_length` and `max_length`, inclusive.
-        To allow infinitely long words the value `None` can be passed in for `max_length`.
-        """
-        if symbols_to_count is None:
-            symbols_to_count = input_symbols
-
-        transitions = {}
-        length_range = range(min_length) if max_length is None else range(max_length+1)
-        for prev_state in length_range:
-            next_state = prev_state + 1
-            transitions[prev_state] = {
-                symbol: next_state if symbol in symbols_to_count else prev_state
-                for symbol in input_symbols
-            }
-        last_state = len(transitions)
-        transitions[last_state] = {symbol: last_state for symbol in input_symbols}
-        final_states = frozenset((last_state,)) if max_length is None else frozenset(range(min_length, max_length+1))
-
-        return cls(
-            states=frozenset(transitions.keys()),
-            input_symbols=input_symbols,
-            transitions=transitions,
-            initial_state=0,
+            initial_state=(0, 0),
             final_states=final_states,
         )
 
-    @classmethod
-    def count_mod(cls, input_symbols, k, *, remainders=None, symbols_to_count=None):
-        """
-        Directly computes a DFA that counts given symbols and accepts all strings where
-        the remainder of division by k is in the set of remainders given.
-        The default value of remainders is {0} and all symbols are counted by default.
-        """
-        if k <= 0:
-            raise ValueError("Integer must be positive")
-        if symbols_to_count is None:
-            symbols_to_count = input_symbols
-        if remainders is None:
-            remainders = {0}
-        transitions = {i: {symbol: (i + 1) % k if symbol in symbols_to_count else i
-                           for symbol in input_symbols}
-                       for i in range(k)}
-
-        return cls(
-            states=frozenset(transitions.keys()),
-            input_symbols=input_symbols,
-            transitions=transitions,
-            initial_state=0,
-            final_states=remainders
-        )
-
-    @classmethod
-    def universal_language(cls, input_symbols):
-        """
-        Directly computes the minimal DFA accepting all strings.
-        """
-        return cls(
-            states={0},
-            input_symbols=input_symbols,
-            transitions={0: {symbol: 0 for symbol in input_symbols}},
-            initial_state=0,
-            final_states={0}
-        )
-
-    @classmethod
-    def empty_language(cls, input_symbols):
-        """
-        Directly computes the minimal DFA rejecting all strings.
-        """
-        return cls(
-            states={0},
-            input_symbols=input_symbols,
-            transitions={0: {symbol: 0 for symbol in input_symbols}},
-            initial_state=0,
-            final_states=frozenset()
+    def iter_transitions(
+        self,
+    ) -> Generator[Tuple[NFAStateT, NFAStateT, str], None, None]:
+        return (
+            (from_, to_, symbol)
+            for from_, lookup in self.transitions.items()
+            for symbol, to_lookup in lookup.items()
+            for to_ in to_lookup
         )
 
-    @classmethod
-    def nth_from_start(cls, input_symbols, symbol, n):
+    def _get_input_path(self, input_str: str) -> Tuple[InputPathListT, bool]:
         """
-        Directly computes the minimal DFA which accepts all words whose `n`-th
-        character from the start is `symbol`, where `n` is a positive integer.
-        """
-        if n < 1:
-            raise ValueError("Integer must be positive")
-        if symbol not in input_symbols:
-            raise exceptions.InvalidSymbolError("Desired symbol is not in the set of input symbols")
-        if len(input_symbols) == 1:
-            return cls.of_length(input_symbols, min_length=n)
-        transitions = {i: {symbol: i+1 for symbol in input_symbols} for i in range(n)}
-        transitions[n-1][symbol] = n+1
-        transitions[n] = {symbol: n for symbol in input_symbols}
-        transitions[n+1] = {symbol: n+1 for symbol in input_symbols}
+        Get best input path. A path is better if (with priority):
 
-        return cls(
-            states=frozenset(transitions.keys()),
-            input_symbols=input_symbols,
-            transitions=transitions,
-            initial_state=0,
-            final_states={n+1}
-        )
+        1. It is an accepting path (ends in a final state)
+        2. It reads more of the input (if the input is not accepted we
+            select the path such that we can stay on the nfa the longest)
+        3. It has the fewest jumps (uses less lambda symbols)
 
-    @classmethod
-    def nth_from_end(cls, input_symbols, symbol, n):
+        Returns a tuple of:
+        1. the path taken
+        2. whether the path was accepting
         """
-        Directly computes the minimal DFA which accepts all words whose `n`-th
-        character from the end is `symbol`, where `n` is a positive integer.
-        """
-        if n < 1:
-            raise ValueError("Integer must be positive")
-        if symbol not in input_symbols:
-            raise exceptions.InvalidSymbolError("Desired symbol is not in the set of input symbols")
-        if len(input_symbols) == 1:
-            return cls.of_length(input_symbols, min_length=n)
-        # Consider the states to be labelled with bitstrings of size n
-        # The bitstring represents how the current suffix in this state matches our desired symbol
-        # A 1 means the character at this position is the desired symbol and a 0 means it is not
-        # For transitions this is effectively doubling the label value and then adding 1 if the desired symbol is read
-        # Finally we trim the label to n bits with a modulo operation.
-        state_count = 2**n
 
-        return cls(
-            states=frozenset(range(state_count)),
-            input_symbols=input_symbols,
-            transitions={state: {sym: (2 * state + 1) % state_count
-                                 if symbol == sym else (2 * state) % state_count
-                                 for sym in input_symbols}
-                         for state in range(state_count)},
-            initial_state=0,
-            final_states=frozenset(range(state_count//2, state_count)),
+        visited = set()
+        work_queue: Deque[Tuple[InputPathListT, NFAStateT, str]] = deque(
+            [([], self.initial_state, input_str)]
         )
 
-    @classmethod
-    def from_finite_language(cls, input_symbols, language):
-        """
-        Directly computes the minimal DFA corresponding to a finite language.
-        Uses the algorithm described in Finite-State Techniques by Mihov and Schulz,
-        Chapter 10
-        """
-
-        if not language:
-            return DFA.empty_language(input_symbols)
+        last_non_accepting_input: InputPathListT = []
+        least_input_remaining = len(input_str)
 
-        transitions = {}
-        back_map = {'': set()}
-        final_states = set()
-        signatures_dict = {}
+        while work_queue:
+            visited_states, curr_state, remaining_input = work_queue.popleft()
 
-        def compute_signature(state):
-            """Computes signature for input state"""
-            return (state in final_states, frozenset(transitions[state].items()))
-
-        def longest_common_prefix_length(string_1, string_2):
-            """Returns length of longest common prefix."""
-            for i, (chr_1, chr_2) in enumerate(zip(string_1, string_2)):
-                if chr_1 != chr_2:
-                    return i
-
-            return min(len(string_1), len(string_2))
-
-        def add_to_trie(word):
-            """Add word to the trie represented by transitions"""
-            prefix = ''
-            for chr in word:
-                next_prefix = prefix + chr
-
-                # Extend the trie only if necessary
-                prefix_dict = transitions.setdefault(prefix, {})
-                prefix_dict.setdefault(chr, next_prefix)
-                back_map.setdefault(next_prefix, set()).add(prefix)
-
-                prefix = next_prefix
-
-            # Mark the finished prefix as a final state
-            transitions[prefix] = {}
-            final_states.add(prefix)
-
-        def compress(word, next_word):
-            """Compress prefixes of word, newly added to the DFA"""
-
-            # Compress along all prefixes that are _not_ prefixes of the next word
-            lcp_len = longest_common_prefix_length(word, next_word)
-
-            # Compression in order of reverse length
-            for i in range(len(word), lcp_len, -1):
-                prefix = word[:i]
-
-                # Compute signature for comparison
-                prefix_signature = compute_signature(prefix)
-                identical_state = signatures_dict.get(prefix_signature)
-
-                if identical_state is not None:
-                    # If identical state exists, remove prefix since it's redundant
-                    final_states.discard(prefix)
-                    transitions.pop(prefix)
-
-                    # Change transition for prefix
-                    for parent_state in back_map[prefix]:
-                        path = transitions[parent_state]
-                        for chr in path:
-                            if path[chr] == prefix:
-                                path[chr] = identical_state
-                        back_map[identical_state].add(parent_state)
-
-                        # No need to recompute signatures here, since we will
-                        # recompute when handling parents in later iterations
-                else:
-                    signatures_dict[prefix_signature] = prefix
-
-        # Construct initial trie
-        prev_word, *rest_words = sorted(language)
-        add_to_trie(prev_word)
-
-        for curr_word in rest_words:
-            # For each word, compress from the previous iteration and continue
-            compress(prev_word, curr_word)
-            add_to_trie(curr_word)
-            prev_word = curr_word
-
-        compress(prev_word, '')
-
-        # Add dump state. Always needed since dict is finite
-        dump_state = 0
-        transitions[dump_state] = {chr: dump_state for chr in input_symbols}
-
-        for path in transitions.values():
-            for chr in input_symbols:
-                path.setdefault(chr, dump_state)
+            # First final state we hit is the best according to desired criteria
+            if curr_state in self.final_states and not remaining_input:
+                return visited_states, True
 
-        return cls(
-            states=frozenset(transitions.keys()),
-            input_symbols=input_symbols,
-            transitions=transitions,
-            initial_state='',
-            final_states=final_states,
-        )
+            # Otherwise, update longest non-accepting input
+            if len(remaining_input) < least_input_remaining:
+                least_input_remaining = len(remaining_input)
+                last_non_accepting_input = visited_states
 
-    @classmethod
-    def from_nfa(cls, target_nfa, *, retain_names=False, minify=True):
-        """Initialize this DFA as one equivalent to the given NFA."""
-        # Data structures for state renaming
-
-        def get_name_original(states):
-            return states
-
-        get_name = get_name_original if retain_names else get_renaming_function(count(0))
-
-        # equivalent DFA states states
-        nfa_initial_states = frozenset(target_nfa._lambda_closures[target_nfa.initial_state])
-        dfa_initial_state = get_name(nfa_initial_states)
-        dfa_final_states = set()
-
-        dfa_states = {dfa_initial_state}
-        dfa_symbols = target_nfa.input_symbols
-        dfa_transitions = {}
-
-        state_queue = deque()
-        state_queue.append(nfa_initial_states)
-        while state_queue:
-            current_states = state_queue.popleft()
-            current_state_name = get_name(current_states)
-
-            # Add NFA states to DFA as it is constructed from NFA.
-            dfa_transitions[current_state_name] = {}
-            if (current_states & target_nfa.final_states):
-                dfa_final_states.add(current_state_name)
-
-            # Enqueue the next set of current states for the generated DFA.
-            for input_symbol in target_nfa.input_symbols:
-                next_current_states = target_nfa._get_next_current_states(
-                    current_states, input_symbol)
-
-                next_current_states_name = get_name(next_current_states)
-                dfa_transitions[current_state_name][input_symbol] = next_current_states_name
-
-                # Only enqueue a state if it has not been seen yet.
-                if next_current_states_name not in dfa_states:
-                    dfa_states.add(next_current_states_name)
-                    state_queue.append(next_current_states)
-
-        if minify:
-            return cls._minify(
-                reachable_states=dfa_states,
-                input_symbols=dfa_symbols,
-                transitions=dfa_transitions,
-                initial_state=dfa_initial_state,
-                reachable_final_states=dfa_final_states,
-                retain_names=retain_names)
+            # First, get next states that result from reading from input
+            if remaining_input:
+                next_symbol = remaining_input[0]
+                rest = remaining_input[1:] if remaining_input else ""
 
-        return cls(
-            states=dfa_states,
-            input_symbols=dfa_symbols,
-            transitions=dfa_transitions,
-            initial_state=dfa_initial_state,
-            final_states=dfa_final_states)
+                next_states_from_symbol = self.transitions[curr_state].get(
+                    next_symbol, set()
+                )
 
-    def show_diagram(self, path=None):
-        """
-            Creates the graph associated with this DFA
-        """
-        # Nodes are set of states
+                for next_state in next_states_from_symbol:
+                    if (next_state, rest) not in visited:
+                        next_visited_states = visited_states.copy()
+                        next_visited_states.append(
+                            (curr_state, next_state, next_symbol)
+                        )
+                        visited.add((next_state, rest))
+                        work_queue.append((next_visited_states, next_state, rest))
+
+            # Next, get next states resulting from lambda transition
+            next_states_from_lambda = self.transitions[curr_state].get("", set())
+
+            for next_state in next_states_from_lambda:
+                if (next_state, remaining_input) not in visited:
+                    next_visited_states = visited_states.copy()
+                    next_visited_states.append((curr_state, next_state, ""))
+                    visited.add((next_state, remaining_input))
+                    work_queue.append(
+                        (next_visited_states, next_state, remaining_input)
+                    )
 
-        graph = Dot(graph_type='digraph', rankdir='LR')
-        nodes = {}
-        for state in self.states:
-            if state == self.initial_state:
-                # color start state with green
-                if state in self.final_states:
-                    initial_state_node = Node(
-                        state,
-                        style='filled',
-                        peripheries=2,
-                        fillcolor='#66cc33')
-                else:
-                    initial_state_node = Node(
-                        state, style='filled', fillcolor='#66cc33')
-                nodes[state] = initial_state_node
-                graph.add_node(initial_state_node)
-            else:
-                if state in self.final_states:
-                    state_node = Node(state, peripheries=2)
-                else:
-                    state_node = Node(state)
-                nodes[state] = state_node
-                graph.add_node(state_node)
-        # adding edges
-        for from_state, lookup in self.transitions.items():
-            for to_label, to_state in lookup.items():
-                graph.add_edge(Edge(
-                    nodes[from_state],
-                    nodes[to_state],
-                    label=to_label
-                ))
-        if path:
-            graph.write_png(path)
-        return graph
+        return last_non_accepting_input, False
```

### Comparing `automata-lib-7.1.0/automata/fa/gnfa.py` & `automata-lib-8.0.0/automata/fa/gnfa.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,311 +1,347 @@
 #!/usr/bin/env python3
-"""Classes and methods for working with generalized non-deterministic finite automata."""
+"""Classes and methods for working with generalized non-deterministic finite
+automata."""
+from __future__ import annotations
 
 from itertools import product
+from typing import (
+    AbstractSet,
+    Dict,
+    Generator,
+    Mapping,
+    Optional,
+    Set,
+    Tuple,
+    Type,
+    cast,
+)
 
-from frozendict import frozendict
-from pydot import Dot, Edge, Node
+from typing_extensions import NoReturn, Self
 
 import automata.base.exceptions as exceptions
+import automata.fa.dfa as dfa
 import automata.fa.fa as fa
 import automata.fa.nfa as nfa
 import automata.regex.regex as re
 
+GNFAStateT = fa.AutomatonStateT
 
-class GNFA(nfa.NFA):
+GNFAPathT = Mapping[GNFAStateT, Optional[str]]
+GNFATransitionsT = Mapping[GNFAStateT, GNFAPathT]
+
+
+class GNFA(fa.FA):
     """A generalized nondeterministic finite automaton."""
 
-    # The conventions of using __slots__ state that subclasses automatically
-    # inherit __slots__ from parent classes, so there's no need to redeclare
-    # slotted attributes for each subclass; however, because NFA has a
-    # 'final_states' attribute but GNFA has a 'final_state' attribute, we must
-    # redeclare them below to exclude 'final_states'
-    __slots__ = ('states', 'input_symbols', 'transitions',
-                 'initial_state', 'final_state')
-
-    def __init__(self, *, states, input_symbols, transitions,
-                 initial_state, final_state):
-        """Initialize a complete NFA."""
+    # Add __dict__ to deal with inheritance issue and the final_states attribute.
+    __slots__ = (
+        "states",
+        "input_symbols",
+        "transitions",
+        "initial_state",
+        "final_state",
+        "__dict__",
+    )
+
+    final_state: GNFAStateT
+
+    def __init__(
+        self,
+        *,
+        states: AbstractSet[GNFAStateT],
+        input_symbols: AbstractSet[str],
+        transitions: GNFATransitionsT,
+        initial_state: GNFAStateT,
+        final_state: GNFAStateT,
+    ) -> None:
+        """Initialize a complete GNFA."""
         super(fa.FA, self).__init__(
-            states=frozenset(states),
-            input_symbols=frozenset(input_symbols),
-            transitions=frozendict({
-                state: frozendict(paths)
-                for state, paths in transitions.items()
-            }),
+            states=states,
+            input_symbols=input_symbols,
+            transitions=transitions,
             initial_state=initial_state,
-            final_state=final_state
+            final_state=final_state,
+            final_states={final_state},
         )
 
     # GNFA should NOT create the lambda closures via NFA.__post_init__()
-    def __post_init__(self):
+    def __post_init__(self) -> None:
         self.validate()
 
     @classmethod
-    def from_dfa(cls, dfa):
+    def from_dfa(cls: Type[Self], dfa: dfa.DFA) -> Self:
         """Initialize this GNFA as one equivalent to the given DFA."""
         new_gnfa_transitions = dict()
         gnfa_states = set(dfa.states)
 
         for state in dfa.states:
-            gnfa_transitions = dict()
+            gnfa_transitions: Dict[GNFAStateT, Optional[str]] = dict()
             if state in dfa.transitions:
                 for input_symbol, to_state in dfa.transitions[state].items():
                     if to_state in gnfa_transitions.keys():
-                        gnfa_transitions[to_state] = f"{gnfa_transitions[to_state]}|{input_symbol}"
+                        gnfa_transitions[
+                            to_state
+                        ] = f"{gnfa_transitions[to_state]}|{input_symbol}"
                     else:
                         gnfa_transitions[to_state] = input_symbol
                 new_gnfa_transitions[state] = gnfa_transitions
             else:
                 new_gnfa_transitions[state] = dict()
 
         new_initial_state = GNFA._add_new_state(gnfa_states)
         new_final_state = GNFA._add_new_state(gnfa_states, new_initial_state)
 
-        new_gnfa_transitions[new_initial_state] = {dfa.initial_state: ''}
+        new_gnfa_transitions[new_initial_state] = {dfa.initial_state: ""}
 
         for state in dfa.final_states:
-            new_gnfa_transitions[state][new_final_state] = ''
+            new_gnfa_transitions[state][new_final_state] = ""
 
         for state in gnfa_states - {new_final_state}:  # pragma: no branch
             if gnfa_states - new_gnfa_transitions[state].keys():  # pragma: no branch
                 for leftover_state in gnfa_states - new_gnfa_transitions[state].keys():
                     if leftover_state is not new_initial_state:
                         new_gnfa_transitions[state][leftover_state] = None
 
         return cls(
-            states=gnfa_states, input_symbols=dfa.input_symbols,
-            transitions=new_gnfa_transitions, initial_state=new_initial_state,
-            final_state=new_final_state)
+            states=gnfa_states,
+            input_symbols=dfa.input_symbols,
+            transitions=new_gnfa_transitions,
+            initial_state=new_initial_state,
+            final_state=new_final_state,
+        )
 
     @classmethod
-    def from_nfa(cls, nfa):
+    def from_nfa(cls: Type[Self], nfa: nfa.NFA) -> Self:
         """Initialize this GNFA as one equivalent to the given NFA."""
-        new_gnfa_transitions = dict()
+        new_gnfa_transitions: Dict[GNFAStateT, Dict[GNFAStateT, Optional[str]]] = dict()
         gnfa_states = set(nfa.states)
 
         for state in nfa.states:
-            gnfa_transitions = dict()
+            gnfa_transitions: Dict[GNFAStateT, str] = dict()
             if state in nfa.transitions:
                 for input_symbol, to_states in nfa.transitions[state].items():
                     for to_state in to_states:
                         if to_state in gnfa_transitions.keys():
-                            if gnfa_transitions[to_state] == '' and input_symbol != '':
-                                gnfa_transitions[to_state] = f'{input_symbol}?'
-                            elif gnfa_transitions[to_state] != '' and input_symbol == '':
+                            if gnfa_transitions[to_state] == "" and input_symbol != "":
+                                gnfa_transitions[to_state] = f"{input_symbol}?"
+                            elif (
+                                gnfa_transitions[to_state] != "" and input_symbol == ""
+                            ):
                                 if cls._isbracket_req(gnfa_transitions[to_state]):
-                                    gnfa_transitions[to_state] = f'({gnfa_transitions[to_state]})?'
+                                    gnfa_transitions[
+                                        to_state
+                                    ] = f"({gnfa_transitions[to_state]})?"
                                 else:
-                                    gnfa_transitions[to_state] = f'{gnfa_transitions[to_state]}?'
+                                    gnfa_transitions[
+                                        to_state
+                                    ] = f"{gnfa_transitions[to_state]}?"
                             else:
-                                gnfa_transitions[to_state] = f"{gnfa_transitions[to_state]}|{input_symbol}"
+                                gnfa_transitions[
+                                    to_state
+                                ] = f"{gnfa_transitions[to_state]}|{input_symbol}"
                         else:
                             gnfa_transitions[to_state] = input_symbol
-                new_gnfa_transitions[state] = gnfa_transitions
+                new_gnfa_transitions[state] = cast(
+                    Dict[GNFAStateT, Optional[str]], gnfa_transitions
+                )
             else:
                 new_gnfa_transitions[state] = dict()
 
         new_initial_state = GNFA._add_new_state(gnfa_states)
         new_final_state = GNFA._add_new_state(gnfa_states, new_initial_state)
 
-        new_gnfa_transitions[new_initial_state] = {nfa.initial_state: ''}
+        new_gnfa_transitions[new_initial_state] = {nfa.initial_state: ""}
 
         for state in nfa.final_states:
-            new_gnfa_transitions[state][new_final_state] = ''
+            new_gnfa_transitions[state][new_final_state] = ""
 
         for state in gnfa_states - {new_final_state}:  # pragma: no branch
             if gnfa_states - new_gnfa_transitions[state].keys():  # pragma: no branch
                 for leftover_state in gnfa_states - new_gnfa_transitions[state].keys():
                     if leftover_state is not new_initial_state:
                         new_gnfa_transitions[state][leftover_state] = None
 
         return cls(
-            states=gnfa_states, input_symbols=nfa.input_symbols,
-            transitions=new_gnfa_transitions, initial_state=new_initial_state,
-            final_state=new_final_state)
+            states=gnfa_states,
+            input_symbols=nfa.input_symbols,
+            transitions=new_gnfa_transitions,
+            initial_state=new_initial_state,
+            final_state=new_final_state,
+        )
 
-    def _validate_transition_invalid_symbols(self, start_state, paths):
+    def _validate_transition_invalid_symbols(
+        self, start_state: GNFAStateT, paths: GNFAPathT
+    ) -> None:
         """Raise an error if transition symbols are invalid."""
-        check = self.input_symbols | {'*', '|', '(', ')', '?'}
+        check = self.input_symbols | {"*", "|", "(", ")", "?"}
 
         for regex in paths.values():
-            if regex is not None and (set(regex) - check and regex != '' or not re._validate(regex)):
+            if regex is not None and (
+                set(regex) - check and regex != "" or not re._validate(regex)
+            ):
                 raise exceptions.InvalidRegexError(
-                    'state {} has invalid transition expression {}'.format(
-                        start_state, regex))
-
-    def _validate_transition_end_states(self, start_state, paths):
+                    "state {} has invalid transition expression {}".format(
+                        start_state, regex
+                    )
+                )
+
+    def _validate_transition_end_states(
+        self, start_state: GNFAStateT, paths: GNFAPathT
+    ) -> None:
         """Raise an error if transition end states are invalid or missing"""
         if start_state == self.final_state:
             if len(paths) != 0:  # pragma: no branch
                 raise exceptions.InvalidStateError(
-                    'No transitions should be defined for '
-                    'final state {}'.format(start_state))
-        elif start_state == self.initial_state and self.states - paths.keys() - {self.initial_state} != set():
+                    "No transitions should be defined for "
+                    "final state {}".format(start_state)
+                )
+        elif (
+            start_state == self.initial_state
+            and self.states - paths.keys() - {self.initial_state} != set()
+        ):
             raise exceptions.MissingStateError(
-                'state {} does not have transitions defined for states {}'.format(
-                    start_state, str(self.states - paths.keys() - {self.initial_state})))
-        elif start_state != self.initial_state and self.states - paths.keys() - {self.initial_state} != set():
+                "state {} does not have transitions defined for states {}".format(
+                    start_state, str(self.states - paths.keys() - {self.initial_state})
+                )
+            )
+        elif (
+            start_state != self.initial_state
+            and self.states - paths.keys() - {self.initial_state} != set()
+        ):
             raise exceptions.MissingStateError(
-                'state {} does not have transitions defined for states {}'.format(
-                    start_state, str(self.states - paths.keys() - {self.initial_state})))
+                "state {} does not have transitions defined for states {}".format(
+                    start_state, str(self.states - paths.keys() - {self.initial_state})
+                )
+            )
         for end_state in paths.keys():  # pragma: no branch
             if end_state not in self.states:
                 raise exceptions.InvalidStateError(
-                    'end state {} for transition on {} is '
-                    'not valid'.format(end_state, start_state))
+                    "end state {} for transition on {} is "
+                    "not valid".format(end_state, start_state)
+                )
 
-    def _validate_final_state(self):
+    def _validate_final_state(self) -> None:
         """Raise an error if the initial state is invalid."""
         if self.final_state not in self.states:
             raise exceptions.InvalidStateError(
-                '{} is not a valid final state'.format(self.final_state))
+                "{} is not a valid final state".format(self.final_state)
+            )
 
-    def validate(self):
+    def validate(self) -> None:
         """Return True if this NFA is internally consistent."""
         self._validate_initial_state()
         self._validate_final_state()
         for start_state, paths in self.transitions.items():
             self._validate_transition_invalid_symbols(start_state, paths)
             self._validate_transition_end_states(start_state, paths)
         self._validate_initial_state_transitions()
-        return True
 
     @staticmethod
-    def _isbracket_req(regex):
+    def _isbracket_req(regex: str) -> bool:
         bracket_open = 0
         for symbol in regex:
-            if symbol == '(':
+            if symbol == "(":
                 bracket_open += 1
-            elif symbol == ')':
+            elif symbol == ")":
                 bracket_open -= 1
-            if bracket_open == 0 and symbol == '|':
+            if bracket_open == 0 and symbol == "|":
                 return True
 
         return False
 
     @staticmethod
-    def _find_min_connected_node(states, transitions, initial_state, final_state):
+    def _find_min_connected_node(
+        states: Set[GNFAStateT],
+        transitions: GNFATransitionsT,
+        initial_state: GNFAStateT,
+        final_state: GNFAStateT,
+    ) -> GNFAStateT:
         state_set = states - {initial_state, final_state}
         state_degree = dict.fromkeys(state_set, 0)
 
         for state in states - {final_state}:
             for to_state, label in transitions[state].items():
                 if label is not None:
                     if state != initial_state:
                         state_degree[state] += 1
                     if to_state != final_state:
                         state_degree[to_state] += 1
 
-        return min(state_degree, key=state_degree.get)
+        return min(state_degree, key=lambda x: state_degree.get(x, -1))
 
-    def to_regex(self):
+    def to_regex(self) -> str:
         """
         Convert GNFA to regular expression.
         """
         new_states = set(self.states)
         new_transitions = {
-            state: dict(paths)
-            for state, paths in self.transitions.items()
+            state: dict(paths) for state, paths in self.transitions.items()
         }
 
         while len(new_states) > 2:
-            q_rip = self._find_min_connected_node(new_states, new_transitions, self.initial_state, self.final_state)
+            q_rip = self._find_min_connected_node(
+                new_states, new_transitions, self.initial_state, self.final_state
+            )
             new_states.remove(q_rip)
-            for q_i, q_j in product(new_states - {self.final_state}, new_states - {self.initial_state}):
+            for q_i, q_j in product(
+                new_states - {self.final_state}, new_states - {self.initial_state}
+            ):
                 r1 = new_transitions[q_i][q_rip]
                 r2 = new_transitions[q_rip][q_rip]
                 r3 = new_transitions[q_rip][q_j]
                 r4 = new_transitions[q_i][q_j]
 
                 if r1 is None or r3 is None:
                     new_transitions[q_i][q_j] = r4
                 else:
                     # check if putting brackets around r1 is necessary
                     if self._isbracket_req(r1):
-                        r1 = f'({r1})'
+                        r1 = f"({r1})"
 
                     if r2 is None:
-                        r2 = ''
+                        r2 = ""
                     elif len(r2) == 1:
-                        r2 = f'{r2}*'
+                        r2 = f"{r2}*"
                     else:
-                        r2 = f'({r2})*'
+                        r2 = f"({r2})*"
 
                     if self._isbracket_req(r3):
-                        r3 = f'({r3})'
+                        r3 = f"({r3})"
 
                     if r4 is None:
-                        r4 = ''
+                        r4 = ""
                     elif self._isbracket_req(r4):
-                        r4 = f'|({r4})'
-                    elif r4 == '':
-                        r4 = '?'
+                        r4 = f"|({r4})"
+                    elif r4 == "":
+                        r4 = "?"
                     else:
-                        r4 = f'|{r4}'
+                        r4 = f"|{r4}"
 
-                    if r4 == '?' and len(r1) + len(r2) + len(r3) > 1:
-                        new_transitions[q_i][q_j] = f'({r1}{r2}{r3}){r4}'
+                    if r4 == "?" and len(r1) + len(r2) + len(r3) > 1:
+                        new_transitions[q_i][q_j] = f"({r1}{r2}{r3}){r4}"
                     else:
-                        new_transitions[q_i][q_j] = f'{r1}{r2}{r3}{r4}'
+                        new_transitions[q_i][q_j] = f"{r1}{r2}{r3}{r4}"
 
             del new_transitions[q_rip]
-            for state in new_states-{self.final_state}:
+            for state in new_states - {self.final_state}:
                 del new_transitions[state][q_rip]
 
         return new_transitions[self.initial_state][self.final_state]
 
-    def __eq__(self, other):
-        return NotImplemented
+    def read_input_stepwise(self, input_str: str) -> NoReturn:
+        raise NotImplementedError
 
-    # The following NFA methods are not supported on GNFA instances because
-    # they are out of scope for the purpose of the GNFA class (which is focused
-    # on regular expression conversion)
-    def read_input_stepwise(self, input_str): raise NotImplementedError
-    def union(self, other): raise NotImplementedError
-    def concatenate(self, other): raise NotImplementedError
-    def kleene_star(self): raise NotImplementedError
-    def option(self): raise NotImplementedError
-    def reverse(self): raise NotImplementedError
-
-    def show_diagram(self, path=None, show_None=True):
-        """
-            Creates the graph associated with this DFA
-        """
-        # Nodes are set of states
+    def iter_transitions(
+        self,
+    ) -> Generator[Tuple[GNFAStateT, GNFAStateT, str], None, None]:
+        return (
+            (from_, to_, symbol)
+            for from_, lookup in self.transitions.items()
+            for to_, symbol in lookup.items()
+            if symbol is not None
+        )
 
-        graph = Dot(graph_type='digraph', rankdir='LR')
-        nodes = {}
-        for state in self.states:
-            if state == self.initial_state:
-                # color start state with green
-                initial_state_node = Node(
-                    state, style='filled', fillcolor='#66cc33')
-                nodes[state] = initial_state_node
-                graph.add_node(initial_state_node)
-            else:
-                if state == self.final_state:
-                    state_node = Node(state, peripheries=2)
-                else:
-                    state_node = Node(state)
-                nodes[state] = state_node
-                graph.add_node(state_node)
-        # adding edges
-        for from_state, lookup in self.transitions.items():
-            for to_state, to_label in lookup.items():  # pragma: no branch
-                if to_label is None and show_None:
-                    to_label = "ø"
-                    graph.add_edge(Edge(
-                        nodes[from_state],
-                        nodes[to_state],
-                        label=to_label
-                    ))
-                elif to_label is not None:
-                    graph.add_edge(Edge(
-                        nodes[from_state],
-                        nodes[to_state],
-                        label=to_label
-                    ))
-        if path:
-            graph.write_png(path)
-        return graph
+    def _get_input_path(self, input_str: str) -> NoReturn:
+        raise NotImplementedError(
+            f"_get_input_path is not implemented for {self.__class__}"
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `automata-lib-7.1.0/automata/pda/dpda.py` & `automata-lib-8.0.0/automata/tm/dtm.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,145 +1,167 @@
 #!/usr/bin/env python3
-"""Classes and methods for working with deterministic pushdown automata."""
+"""Classes and methods for working with deterministic Turing machines."""
+
+from typing import AbstractSet, Generator, Mapping, Optional, Tuple
 
 import automata.base.exceptions as exceptions
-import automata.pda.exceptions as pda_exceptions
-import automata.pda.pda as pda
-from automata.pda.configuration import PDAConfiguration
-from automata.pda.stack import PDAStack
-
-
-class DPDA(pda.PDA):
-    """A deterministic pushdown automaton."""
-
-    __slots__ = ('states', 'input_symbols', 'stack_symbols',
-                 'transitions', 'initial_state',
-                 'initial_stack_symbol', 'final_states', 'acceptance_mode')
-
-    def __init__(self, *, states, input_symbols, stack_symbols,
-                 transitions, initial_state,
-                 initial_stack_symbol, final_states, acceptance_mode='both'):
-        """Initialize a complete DPDA."""
+import automata.tm.exceptions as tm_exceptions
+import automata.tm.tm as tm
+from automata.tm.configuration import TMConfiguration
+from automata.tm.tape import TMTape
+
+DTMStateT = tm.TMStateT
+DTMPathResultT = Tuple[DTMStateT, str, tm.TMDirectionT]
+DTMPathT = Mapping[str, DTMPathResultT]
+DTMTransitionsT = Mapping[DTMStateT, DTMPathT]
+
+
+class DTM(tm.TM):
+    """A deterministic Turing machine."""
+
+    __slots__ = (
+        "states",
+        "input_symbols",
+        "tape_symbols",
+        "transitions",
+        "initial_state",
+        "blank_symbol",
+        "final_states",
+    )
+
+    def __init__(
+        self,
+        *,
+        states: AbstractSet[DTMStateT],
+        input_symbols: AbstractSet[str],
+        tape_symbols: AbstractSet[str],
+        transitions: DTMTransitionsT,
+        initial_state: DTMStateT,
+        blank_symbol: str,
+        final_states: AbstractSet[DTMStateT],
+    ) -> None:
+        """Initialize a complete Turing machine."""
         super().__init__(
             states=states,
             input_symbols=input_symbols,
-            stack_symbols=stack_symbols,
+            tape_symbols=tape_symbols,
             transitions=transitions,
             initial_state=initial_state,
-            initial_stack_symbol=initial_stack_symbol,
+            blank_symbol=blank_symbol,
             final_states=final_states,
-            acceptance_mode=acceptance_mode,
         )
 
-    def _validate_transition_invalid_symbols(self, start_state, paths):
-        """Raise an error if transition symbols are invalid."""
-        for input_symbol, symbol_paths in paths.items():
-            self._validate_transition_invalid_input_symbols(
-                start_state, input_symbol)
-            for stack_symbol in symbol_paths:
-                self._validate_transition_isolated_lambda_transitions(
-                    start_state, input_symbol, stack_symbol)
-                self._validate_transition_invalid_stack_symbols(
-                    start_state, stack_symbol)
-
-    def _validate_transition_lambda_transition_sibling(self, start_state,
-                                                       sib_path):
-        """Check the given sibling path for adjacent lambda transitions."""
-        for other_stack_symbol in sib_path:
-            if (other_stack_symbol in
-                    self.transitions[start_state]['']):
-                raise pda_exceptions.NondeterminismError(
-                    'A symbol transition is adjacent to a '
-                    'lambda transition for this DPDA.')
-
-    def _validate_transition_isolated_lambda_transitions(self, start_state,
-                                                         input_symbol,
-                                                         stack_symbol):
-        """Raise an error if a lambda transition has no sibling transitions."""
-        if input_symbol == '':
-            sib_transitions = self.transitions[start_state]
-            for sib_input_symbol, sib_path in sib_transitions.items():
-                if sib_input_symbol != '':
-                    self._validate_transition_lambda_transition_sibling(
-                        start_state, sib_path)
-
-    def _get_transition(self, state, input_symbol, stack_symbol):
-        """Get the transiton tuple for the given state and symbols."""
-        if (state in self.transitions and
-                input_symbol in self.transitions[state] and
-                stack_symbol in self.transitions[state][input_symbol]):
-            return (
-                input_symbol,
-            ) + self.transitions[state][input_symbol][stack_symbol]
-
-    def _check_for_input_rejection(self, current_configuration):
-        """Raise an error if the given config indicates rejected input."""
-        if not self._has_accepted(current_configuration):
-            raise exceptions.RejectionException(
-                'the DPDA stopped in a non-accepting configuration '
-                '({state}, {stack})'
-                .format(**current_configuration._asdict())
+    def _validate_transition_state(self, transition_state: DTMStateT) -> None:
+        if transition_state not in self.states:
+            raise exceptions.InvalidStateError(
+                "transition state is not valid ({})".format(transition_state)
             )
 
-    def _get_next_configuration(self, old_config):
-        """Advance to the next configuration."""
-        transitions = set()
-        if old_config.remaining_input:
-            transitions.add(self._get_transition(
-                old_config.state,
-                old_config.remaining_input[0],
-                old_config.stack.top()
-            ))
-        transitions.add(self._get_transition(
-            old_config.state,
-            '',
-            old_config.stack.top()
-        ))
-        if None in transitions:
-            transitions.remove(None)
-        if len(transitions) == 0:
-            raise exceptions.RejectionException(
-                'The automaton entered a configuration for which no '
-                'transition is defined ({}, {}, {})'.format(
-                    old_config.state,
-                    old_config.remaining_input[0],
-                    old_config.stack.top()
+    def _validate_transition_symbols(
+        self, state: DTMStateT, paths: DTMTransitionsT
+    ) -> None:
+        for tape_symbol in paths.keys():
+            if tape_symbol not in self.tape_symbols:
+                raise exceptions.InvalidSymbolError(
+                    "transition symbol {} for state {} is not valid".format(
+                        tape_symbol, state
+                    )
                 )
+
+    def _validate_transition_result_direction(
+        self, result_direction: tm.TMDirectionT
+    ) -> None:
+        if result_direction not in ("L", "N", "R"):
+            raise tm_exceptions.InvalidDirectionError(
+                "result direction is not valid ({})".format(result_direction)
             )
-        input_symbol, new_state, new_stack_top = transitions.pop()
-        remaining_input = old_config.remaining_input
-        if input_symbol:
-            remaining_input = remaining_input[1:]
-        new_config = PDAConfiguration(
-            new_state,
-            remaining_input,
-            self._replace_stack_top(old_config.stack, new_stack_top)
+
+    def _validate_transition_result(self, result: DTMPathResultT) -> None:
+        result_state, result_symbol, result_direction = result
+        if result_state not in self.states:
+            raise exceptions.InvalidStateError(
+                "result state is not valid ({})".format(result_state)
+            )
+        if result_symbol not in self.tape_symbols:
+            raise exceptions.InvalidSymbolError(
+                "result symbol is not valid ({})".format(result_symbol)
+            )
+        self._validate_transition_result_direction(result_direction)
+
+    def _validate_transition_results(self, paths: DTMPathT) -> None:
+        for result in paths.values():
+            self._validate_transition_result(result)
+
+    def _validate_transitions(self) -> None:
+        for state, paths in self.transitions.items():
+            self._validate_transition_state(state)
+            self._validate_transition_symbols(state, paths)
+            self._validate_transition_results(paths)
+
+    def _validate_final_state_transitions(self) -> None:
+        for final_state in self.final_states:
+            if final_state in self.transitions:
+                raise exceptions.FinalStateError(
+                    "final state {} has transitions defined".format(final_state)
+                )
+
+    def validate(self) -> None:
+        """Return True if this DTM is internally consistent."""
+        self._read_input_symbol_subset()
+        self._validate_blank_symbol()
+        self._validate_transitions()
+        self._validate_initial_state()
+        self._validate_initial_state_transitions()
+        self._validate_nonfinal_initial_state()
+        self._validate_final_states()
+        self._validate_final_state_transitions()
+
+    def _get_transition(
+        self, state: DTMStateT, tape_symbol: str
+    ) -> Optional[DTMPathResultT]:
+        """Get the transiton tuple for the given state and tape symbol."""
+        if state in self.transitions and tape_symbol in self.transitions[state]:
+            return self.transitions[state][tape_symbol]
+        else:
+            return None
+
+    def _has_accepted(self, configuration: TMConfiguration) -> bool:
+        """Check whether the given config indicates accepted input."""
+        return configuration.state in self.final_states
+
+    def _get_next_configuration(self, old_config: TMConfiguration) -> TMConfiguration:
+        """Advance to the next configuration."""
+        next_transition = self._get_transition(
+            old_config.state, old_config.tape.read_symbol()
         )
-        return new_config
 
-    def read_input_stepwise(self, input_str):
+        if next_transition is None:
+            raise exceptions.RejectionException(
+                "The machine entered a non-final configuration for which no "
+                "transition is defined ({}, {})".format(
+                    old_config.state, old_config.tape.read_symbol()
+                )
+            )
+        tape = old_config.tape
+        (new_state, new_tape_symbol, direction) = next_transition
+        tape = tape.write_symbol(new_tape_symbol)
+        tape = tape.move(direction)
+        return TMConfiguration(new_state, tape)
+
+    def read_input_stepwise(
+        self, input_str: str
+    ) -> Generator[TMConfiguration, None, None]:
         """
-        Check if the given string is accepted by this DPDA.
+        Check if the given string is accepted by this Turing machine.
 
-        Yield the DPDA's current configuration at each step.
+        Yield the current configuration of the machine at each step.
         """
-        current_configuration = PDAConfiguration(
-            self.initial_state,
-            input_str,
-            PDAStack([self.initial_stack_symbol])
+        current_configuration = TMConfiguration(
+            self.initial_state, TMTape(input_str, blank_symbol=self.blank_symbol)
         )
-
         yield current_configuration
-        while (
-            current_configuration.remaining_input
-            or self._has_lambda_transition(
-                current_configuration.state,
-                current_configuration.stack.top()
-            )
-        ):
-            current_configuration = self._get_next_configuration(
-                current_configuration
-            )
+
+        # The initial state cannot be a final state for a DTM, so the first
+        # iteration is always guaranteed to run (as it should)
+        while not self._has_accepted(current_configuration):
+            current_configuration = self._get_next_configuration(current_configuration)
             yield current_configuration
-            if self._has_accepted(current_configuration):
-                return
-        self._check_for_input_rejection(current_configuration)
```

### Comparing `automata-lib-7.1.0/automata/pda/npda.py` & `automata-lib-8.0.0/automata/pda/npda.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,122 +1,146 @@
 #!/usr/bin/env python3
 """Classes and methods for working with nondeterministic pushdown automata."""
 
+from typing import AbstractSet, Generator, Mapping, Set, Tuple, Union
+
 import automata.base.exceptions as exceptions
 import automata.pda.pda as pda
 from automata.pda.configuration import PDAConfiguration
 from automata.pda.stack import PDAStack
 
+NPDAStateT = pda.PDAStateT
+
+NPDAPathT = Mapping[
+    str,
+    Mapping[str, AbstractSet[Tuple[NPDAStateT, Union[str, Tuple[str, ...]]]]],
+]
+NPDATransitionsT = Mapping[NPDAStateT, NPDAPathT]
+
 
 class NPDA(pda.PDA):
     """A nondeterministic pushdown automaton."""
 
-    __slots__ = ('states', 'input_symbols', 'stack_symbols',
-                 'transitions', 'initial_state',
-                 'initial_stack_symbol', 'final_states', 'acceptance_mode')
-
-    def __init__(self, *, states, input_symbols, stack_symbols,
-                 transitions, initial_state,
-                 initial_stack_symbol, final_states, acceptance_mode='both'):
+    __slots__ = (
+        "states",
+        "input_symbols",
+        "stack_symbols",
+        "transitions",
+        "initial_state",
+        "initial_stack_symbol",
+        "final_states",
+        "acceptance_mode",
+    )
+
+    def __init__(
+        self,
+        *,
+        states: AbstractSet[NPDAStateT],
+        input_symbols: AbstractSet[str],
+        stack_symbols: AbstractSet[str],
+        transitions: NPDATransitionsT,
+        initial_state: NPDAStateT,
+        initial_stack_symbol: str,
+        final_states: AbstractSet[NPDAStateT],
+        acceptance_mode: pda.PDAAcceptanceModeT = "both",
+    ) -> None:
         """Initialize a complete NPDA."""
         super().__init__(
             states=states,
             input_symbols=input_symbols,
             stack_symbols=stack_symbols,
             transitions=transitions,
             initial_state=initial_state,
             initial_stack_symbol=initial_stack_symbol,
             final_states=final_states,
-            acceptance_mode=acceptance_mode
+            acceptance_mode=acceptance_mode,
         )
 
-    def _validate_transition_invalid_symbols(self, start_state, paths):
+    def _validate_transition_invalid_symbols(
+        self, start_state: NPDAStateT, paths: NPDATransitionsT
+    ) -> None:
         """Raise an error if transition symbols are invalid."""
         for input_symbol, symbol_paths in paths.items():
-            self._validate_transition_invalid_input_symbols(
-                start_state, input_symbol)
+            self._validate_transition_invalid_input_symbols(start_state, input_symbol)
             for stack_symbol in symbol_paths:
                 self._validate_transition_invalid_stack_symbols(
-                    start_state, stack_symbol)
+                    start_state, stack_symbol
+                )
 
-    def _get_transitions(self, state, input_symbol, stack_symbol):
+    def _get_transitions(
+        self, state: NPDAStateT, input_symbol: str, stack_symbol: str
+    ) -> Set[Tuple[str, NPDAStateT, str]]:
         """Get the transition tuples for the given state and symbols."""
         transitions = set()
-        if (state in self.transitions and
-                input_symbol in self.transitions[state] and
-                stack_symbol in self.transitions[state][input_symbol]):
-            for (
-                dest_state,
-                new_stack_top
-            ) in self.transitions[state][input_symbol][stack_symbol]:
-                transitions.add((
-                    input_symbol,
-                    dest_state,
-                    new_stack_top
-                ))
+        if (
+            state in self.transitions
+            and input_symbol in self.transitions[state]
+            and stack_symbol in self.transitions[state][input_symbol]
+        ):
+            for dest_state, new_stack_top in self.transitions[state][input_symbol][
+                stack_symbol
+            ]:
+                transitions.add((input_symbol, dest_state, new_stack_top))
         return transitions
 
-    def _get_next_configurations(self, old_config):
+    def _get_next_configurations(
+        self, old_config: PDAConfiguration
+    ) -> Set[PDAConfiguration]:
         """Advance to the next configurations."""
-        transitions = set()
+        transitions: Set[Tuple[str, NPDAStateT, str]] = set()
         if old_config.remaining_input:
-            transitions.update(self._get_transitions(
-                old_config.state,
-                old_config.remaining_input[0],
-                old_config.stack.top()
-            ))
-        transitions.update(self._get_transitions(
-            old_config.state,
-            '',
-            old_config.stack.top()
-        ))
+            transitions.update(
+                self._get_transitions(
+                    old_config.state,
+                    old_config.remaining_input[0],
+                    old_config.stack.top(),
+                )
+            )
+        transitions.update(
+            self._get_transitions(old_config.state, "", old_config.stack.top())
+        )
         new_configs = set()
-        for input_symbol, new_state, new_stack_top in transitions:
+        for input_symbol, new_state, new_stack_top in transitions:  # type: ignore
             remaining_input = old_config.remaining_input
             if input_symbol:
                 remaining_input = remaining_input[1:]
             new_config = PDAConfiguration(
                 new_state,
                 remaining_input,
-                self._replace_stack_top(old_config.stack, new_stack_top)
+                self._replace_stack_top(old_config.stack, new_stack_top),
             )
             new_configs.add(new_config)
         return new_configs
 
-    def read_input_stepwise(self, input_str):
+    def read_input_stepwise(
+        self, input_str: str
+    ) -> Generator[Set[PDAConfiguration], None, None]:
         """
         Check if the given string is accepted by this NPDA.
 
         Yield the NPDA's current configurations at each step.
         """
         current_configurations = set()
-        current_configurations.add(PDAConfiguration(
-            self.initial_state,
-            input_str,
-            PDAStack([self.initial_stack_symbol])
-        ))
+        current_configurations.add(
+            PDAConfiguration(
+                self.initial_state, input_str, PDAStack([self.initial_stack_symbol])
+            )
+        )
 
         yield current_configurations
 
         while current_configurations:
             new_configurations = set()
             for config in current_configurations:
                 if self._has_accepted(config):
                     # One accepting configuration is enough.
                     return
                 if config.remaining_input:
-                    new_configurations.update(
-                        self._get_next_configurations(config)
-                    )
-                elif self._has_lambda_transition(
-                    config.state,
-                    config.stack.top()
-                ):
-                    new_configurations.update(
-                        self._get_next_configurations(config)
-                    )
+                    new_configurations.update(self._get_next_configurations(config))
+                elif self._has_lambda_transition(config.state, config.stack.top()):
+                    new_configurations.update(self._get_next_configurations(config))
             current_configurations = new_configurations
             yield current_configurations
 
         raise exceptions.RejectionException(
-            'the NPDA did not reach an accepting configuration'
+            "the NPDA did not reach an accepting configuration"
         )
```

### Comparing `automata-lib-7.1.0/automata/pda/pda.py` & `automata-lib-8.0.0/automata/pda/pda.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,82 +1,108 @@
 #!/usr/bin/env python3
 """Classes and methods for working with all pushdown automata."""
 
 import abc
+from typing import AbstractSet, Literal
 
 import automata.base.exceptions as exceptions
 import automata.pda.exceptions as pda_exceptions
-from automata.base.automaton import Automaton
+from automata.base.automaton import Automaton, AutomatonStateT, AutomatonTransitionsT
+from automata.pda.configuration import PDAConfiguration
+from automata.pda.stack import PDAStack
+
+PDAStateT = AutomatonStateT
+PDATransitionsT = AutomatonTransitionsT
+PDAAcceptanceModeT = Literal["final_state", "empty_stack", "both"]
 
 
 class PDA(Automaton, metaclass=abc.ABCMeta):
     """An abstract base class for pushdown automata."""
 
-    def _validate_transition_invalid_input_symbols(self, start_state,
-                                                   input_symbol):
+    __slots__ = tuple()
+
+    stack_symbols: AbstractSet[str]
+    initial_stack_symbol: str
+    acceptance_mode: PDAAcceptanceModeT
+
+    def _validate_transition_invalid_input_symbols(
+        self, start_state: PDAStateT, input_symbol: str
+    ) -> None:
         """Raise an error if transition input symbols are invalid."""
-        if input_symbol not in self.input_symbols and input_symbol != '':
+        if input_symbol not in self.input_symbols and input_symbol != "":
             raise exceptions.InvalidSymbolError(
-                'state {} has invalid transition input symbol {}'.format(
-                    start_state, input_symbol))
-
-    def _validate_transition_invalid_stack_symbols(self, start_state,
-                                                   stack_symbol):
+                "state {} has invalid transition input symbol {}".format(
+                    start_state, input_symbol
+                )
+            )
+
+    def _validate_transition_invalid_stack_symbols(
+        self, start_state: PDAStateT, stack_symbol: str
+    ) -> None:
         """Raise an error if transition stack symbols are invalid."""
         if stack_symbol not in self.stack_symbols:
             raise exceptions.InvalidSymbolError(
-                'state {} has invalid transition stack symbol {}'.format(
-                    start_state, stack_symbol))
+                "state {} has invalid transition stack symbol {}".format(
+                    start_state, stack_symbol
+                )
+            )
 
-    def _validate_initial_stack_symbol(self):
+    def _validate_initial_stack_symbol(self) -> None:
         """Raise an error if initial stack symbol is invalid."""
         if self.initial_stack_symbol not in self.stack_symbols:
             raise exceptions.InvalidSymbolError(
-                'initial stack symbol {} is invalid'.format(
-                    self.initial_stack_symbol))
+                "initial stack symbol {} is invalid".format(self.initial_stack_symbol)
+            )
 
-    def _validate_acceptance(self):
+    def _validate_acceptance(self) -> None:
         """Raise an error if the acceptance mode is invalid."""
-        if self.acceptance_mode not in ('final_state', 'empty_stack', 'both'):
+        if self.acceptance_mode not in ("final_state", "empty_stack", "both"):
             raise pda_exceptions.InvalidAcceptanceModeError(
-                'acceptance mode {} is invalid'.format(
-                    self.acceptance_mode))
+                "acceptance mode {} is invalid".format(self.acceptance_mode)
+            )
+
+    @abc.abstractmethod
+    def _validate_transition_invalid_symbols(
+        self, start_state: PDAStateT, paths: PDATransitionsT
+    ) -> None:
+        pass
 
-    def validate(self):
+    def validate(self) -> None:
         """Return True if this PDA is internally consistent."""
         for start_state, paths in self.transitions.items():
             self._validate_transition_invalid_symbols(start_state, paths)
         self._validate_initial_state()
         self._validate_initial_stack_symbol()
         self._validate_final_states()
         self._validate_acceptance()
-        return True
 
-    def _has_lambda_transition(self, state, stack_symbol):
+    def _has_lambda_transition(self, state: PDAStateT, stack_symbol: str) -> bool:
         """Return True if the current config has any lambda transitions."""
-        return (state in self.transitions and
-                '' in self.transitions[state] and
-                stack_symbol in self.transitions[state][''])
+        return (
+            state in self.transitions
+            and "" in self.transitions[state]
+            and stack_symbol in self.transitions[state][""]
+        )
 
-    def _replace_stack_top(self, stack, new_stack_top):
+    def _replace_stack_top(self, stack: PDAStack, new_stack_top: str) -> PDAStack:
         """Replace the top of the PDA stack with another symbol"""
-        if new_stack_top == '':
+        if new_stack_top == "":
             new_stack = stack.pop()
         else:
             new_stack = stack.replace(new_stack_top)
         return new_stack
 
-    def _has_accepted(self, current_configuration):
+    def _has_accepted(self, current_configuration: PDAConfiguration) -> bool:
         """Check whether the given config indicates accepted input."""
         # If there's input left, we're not finished.
         if current_configuration.remaining_input:
             return False
-        if self.acceptance_mode in ('empty_stack', 'both'):
+        if self.acceptance_mode in ("empty_stack", "both"):
             # If the stack is empty, we accept.
             if not current_configuration.stack:
                 return True
-        if self.acceptance_mode in ('final_state', 'both'):
+        if self.acceptance_mode in ("final_state", "both"):
             # If current state is a final state, we accept.
             if current_configuration.state in self.final_states:
                 return True
         # Otherwise, not.
         return False
```

### Comparing `automata-lib-7.1.0/automata/regex/lexer.py` & `automata-lib-8.0.0/automata/regex/lexer.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,110 +3,144 @@
 Classes and methods for lexing expressions into lists of tokens.
 
 Adapted from code in the tdparser library: https://github.com/rbarrois/tdparser
 """
 
 import abc
 import re
+from typing import (
+    AbstractSet,
+    Callable,
+    FrozenSet,
+    Generator,
+    Generic,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+)
+
+from typing_extensions import Self
 
 import automata.base.exceptions as exceptions
 
+ResultT = TypeVar("ResultT")
+
 
-class Token(metaclass=abc.ABCMeta):
+class Token(Generic[ResultT], metaclass=abc.ABCMeta):
     """Base class for tokens."""
 
-    __slots__ = ('text',)
+    __slots__: Tuple[str, ...] = ("text",)
 
-    def __init__(self, text):
+    text: str
+
+    def __init__(self, text: str) -> None:
         self.text = text
 
-    def get_precedence(self):
-        raise NotImplementedError
+    @classmethod
+    def from_match(cls: Type[Self], match: re.Match) -> Self:
+        return cls(match.group())
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         return f"<{self.__class__.__name__}: {self.text}>"
 
 
-class TokenRegistry():
+TokenFactoryT = Callable[[re.Match], Token[ResultT]]
+
+
+class TokenRegistry(Generic[ResultT]):
     """Registry holding token rules."""
 
-    __slots__ = ('_tokens',)
+    __slots__: Tuple[str, ...] = ("_tokens",)
+
+    _tokens: List[Tuple[TokenFactoryT, re.Pattern]]
 
-    def __init__(self):
+    def __init__(self) -> None:
         self._tokens = []
 
-    def register(self, token_factory_fn, token_regex):
+    def register(self, token_factory_fn: TokenFactoryT, token_regex: str) -> None:
         """
         Register a token that can be produced by token_factory_fn (a function
-        taking in a string returning the final token) and recognized by the
+        taking in a regex match and returning the final token) and recognized by the
         token_regex pattern.
         """
         self._tokens.append((token_factory_fn, re.compile(token_regex)))
 
-    def matching_tokens(self, text, start):
+    def matching_tokens(
+        self, text: str, start: int
+    ) -> Generator[Tuple[TokenFactoryT, re.Match], None, None]:
         """Retrieve all token definitions matching text starting at start."""
 
         for token_factory_fn, regexp in self._tokens:
             match = regexp.match(text, pos=start)
             if match:
                 yield (token_factory_fn, match)
 
-    def get_token(self, text, start=0):
+    def get_token(
+        self, text: str, start: int = 0
+    ) -> Optional[Tuple[TokenFactoryT, re.Match]]:
         """
         Retrieve the next token from some text. Computes the best match by
         length. Returns None if there is no match in the token registry.
         """
         best_token_match = None
         best_match = None
 
         for token_factory_fn, match in self.matching_tokens(text, start):
             if not best_match or best_match.end() < match.end():
                 best_token_match = (token_factory_fn, match)
                 best_match = match
 
         return best_token_match
 
-    def __len__(self):
+    def __len__(self) -> int:
         return len(self._tokens)
 
 
-class Lexer():
+class Lexer(Generic[ResultT]):
     """
     The core lexer. First, tokens are registered with their factory functions and regex
     patterns. The lexer can then take in a string and splits it into a list of token
     classes (in infix ordering) matching the regex patterns.
     """
 
-    __slots__ = ('tokens', 'blank_chars')
+    __slots__: Tuple[str, ...] = ("tokens", "blank_chars")
+
+    tokens: TokenRegistry[ResultT]
+    blank_chars: FrozenSet[str]
 
-    def __init__(self, blank_chars={' ', '\t'}):
+    def __init__(self, blank_chars: Optional[AbstractSet] = None) -> None:
         self.tokens = TokenRegistry()
-        self.blank_chars = blank_chars
+        self.blank_chars = (
+            frozenset((" ", "\t")) if blank_chars is None else frozenset(blank_chars)
+        )
 
-    def register_token(self, token_factory_fn, token_regex):
+    def register_token(self, token_factory_fn: TokenFactoryT, token_regex: str) -> None:
         """
         Register a token class. The token_factory_fn must taken in a
-        string and return an instance of the desired token, and token_regex
+        match object and return an instance of the desired token, and token_regex
         is used by the lexer to match tokens in the input text.
         """
 
         self.tokens.register(token_factory_fn, token_regex)
 
-    def lex(self, text):
+    def lex(self, text: str) -> List[Token[ResultT]]:
         """Split text into a list of tokens in infix notation."""
 
         pos = 0
         res = []
 
         while pos < len(text):
             token_match = self.tokens.get_token(text, start=pos)
             if token_match is not None:
                 token_factory_fn, match = token_match
-                matched_text = match.group(0)
-                res.append(token_factory_fn(matched_text))
-                pos += len(matched_text)
+                res.append(token_factory_fn(match))
+                pos += len(match.group())
             elif text[pos] in self.blank_chars:
                 pos += 1
             else:
-                raise exceptions.LexerError(f"Invalid character '{text[pos]}' in '{text}'", position=pos)
+                raise exceptions.LexerError(
+                    f"Invalid character '{text[pos]}' in '{text}'", position=pos
+                )
 
         return res
```

### Comparing `automata-lib-7.1.0/automata/regex/postfix.py` & `automata-lib-8.0.0/automata/regex/postfix.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,136 +1,185 @@
 #!/usr/bin/env python3
 """Classes and methods for converting lists of tokens to postfix ordering."""
 
 import abc
 from collections import deque
 from itertools import zip_longest
+from typing import Deque, List, Optional, Tuple, TypeVar, cast
 
 import automata.base.exceptions as exceptions
 from automata.regex.lexer import Token
 
+ExpressionResultT = TypeVar("ExpressionResultT")
 
-class Operator(Token):
+
+class Operator(Token[ExpressionResultT]):
     """Subclass of token defining an operator."""
 
+    __slots__: Tuple[str, ...] = tuple()
+
     @abc.abstractmethod
-    def get_precedence(self):
+    def get_precedence(self) -> int:
         raise NotImplementedError
 
 
-class InfixOperator(Operator):
+class InfixOperator(Operator[ExpressionResultT]):
     """Subclass of operator defining an infix operator."""
 
+    __slots__: Tuple[str, ...] = tuple()
+
     @abc.abstractmethod
-    def op(self, left, right):
+    def op(
+        self, left: ExpressionResultT, right: ExpressionResultT
+    ) -> ExpressionResultT:
         raise NotImplementedError
 
 
-class PostfixOperator(Operator):
+class PostfixOperator(Operator[ExpressionResultT]):
     """Subclass of operator defining an postfix operator."""
 
+    __slots__: Tuple[str, ...] = tuple()
+
     @abc.abstractmethod
-    def op(self, left):
+    def op(self, left: ExpressionResultT) -> ExpressionResultT:
         raise NotImplementedError
 
 
-class Literal(Token):
+class Literal(Token[ExpressionResultT]):
     """Subclass of token defining a literal."""
 
+    __slots__: Tuple[str, ...] = tuple()
+
     @abc.abstractmethod
-    def val(self):
+    def val(self) -> ExpressionResultT:
         raise NotImplementedError
 
 
 class RightParen(Token):
     """Subclass of token defining a right parenthesis."""
 
-    def __repr__(self):
-        return '<)>'
+    __slots__: Tuple[str, ...] = tuple()
+
+    def __repr__(self) -> str:
+        return "<)>"
 
 
 class LeftParen(Token):
     """Subclass of token defining a left parenthesis."""
 
-    def __repr__(self):
-        return '<(>'
+    __slots__: Tuple[str, ...] = tuple()
 
+    def __repr__(self) -> str:
+        return "<(>"
 
-def validate_tokens(token_list):
+
+def validate_tokens(token_list: List[Token]) -> None:
     """Validate the inputted tokens list (in infix ordering)."""
 
-    token_list_prev = [None] + token_list
+    token_list_prev: List[Optional[Token]] = [None] + token_list
 
     paren_counter = 0
 
     for prev_token, curr_token in zip_longest(token_list_prev, token_list):
         # No postfix or infix operators at the beginning
-        if prev_token is None and isinstance(curr_token, (InfixOperator, PostfixOperator)):
-            raise exceptions.InvalidRegexError(f"'{curr_token}' cannot appear at the start of a statement.")
+        if prev_token is None and isinstance(
+            curr_token, (InfixOperator, PostfixOperator)
+        ):
+            raise exceptions.InvalidRegexError(
+                f"'{curr_token}' cannot appear at the start of a statement."
+            )
 
-        # No postfix operators at the end of a statement or right before another operator or right paren
+        # No postfix operators at the end of a statement or right before another
+        # operator or right paren
         elif isinstance(prev_token, InfixOperator):
             if curr_token is None:
-                raise exceptions.InvalidRegexError(f"'{prev_token}' cannot appear at the end of a statement.")
+                raise exceptions.InvalidRegexError(
+                    f"'{prev_token}' cannot appear at the end of a statement."
+                )
             elif isinstance(curr_token, (InfixOperator, PostfixOperator, RightParen)):
-                raise exceptions.InvalidRegexError(f"'{prev_token}' cannot appear immediately before '{curr_token}'.")
+                raise exceptions.InvalidRegexError(
+                    f"'{prev_token}' cannot appear immediately before '{curr_token}'."
+                )
 
-        # No left parens right before infix or postfix operators, or right before a right paren
+        # No left parens right before infix or postfix operators, or right
+        # before a right paren
         elif isinstance(prev_token, LeftParen):
-            if isinstance(curr_token, (InfixOperator, PostfixOperator, RightParen)):
-                raise exceptions.InvalidRegexError(f"'{prev_token}' cannot appear immediately before '{curr_token}'.")
+            if isinstance(curr_token, (InfixOperator, PostfixOperator)):
+                raise exceptions.InvalidRegexError(
+                    f"'{prev_token}' cannot appear immediately before '{curr_token}'."
+                )
 
             # Track open/closed parens
             paren_counter += 1
 
         elif isinstance(prev_token, RightParen):
             paren_counter -= 1
 
             if paren_counter < 0:
-                raise exceptions.InvalidRegexError("Token list has mismatched parethesis.")
+                raise exceptions.InvalidRegexError(
+                    "Token list has mismatched parethesis."
+                )
 
     if paren_counter != 0:
         raise exceptions.InvalidRegexError("Token list has unclosed parethesis.")
 
 
-def tokens_to_postfix(tokens):
+def tokens_to_postfix(
+    tokens: List[Token[ExpressionResultT]],
+) -> List[Token[ExpressionResultT]]:
     """Takes in a list of tokens and changes them to postfix ordering."""
-    stack = deque()
-    res = []
 
-    def comp_precedence(a, b):
+    stack: Deque[Token[ExpressionResultT]] = deque()
+    res: List[Token[ExpressionResultT]] = []
+
+    def comp_precedence(
+        a: Token[ExpressionResultT], b: Token[ExpressionResultT]
+    ) -> bool:
         """Compare precedence of operators (two tokens)."""
-        return a.get_precedence() <= b.get_precedence()
+        return (
+            cast(Operator[ExpressionResultT], a).get_precedence()
+            <= cast(Operator[ExpressionResultT], b).get_precedence()
+        )
 
     for c in tokens:
         if isinstance(c, Literal):
             res.append(c)
         elif isinstance(c, RightParen):
             while len(stack) > 0 and not isinstance(stack[-1], LeftParen):
                 res.append(stack.pop())
             stack.pop()
         elif isinstance(c, LeftParen):
             stack.append(c)
-        elif not stack or isinstance(stack[-1], LeftParen) or not comp_precedence(c, stack[-1]):
+        elif (
+            not stack
+            or isinstance(stack[-1], LeftParen)
+            or not comp_precedence(c, stack[-1])
+        ):
             stack.append(c)
         else:
-            while stack and not isinstance(stack[-1], LeftParen) and comp_precedence(c, stack[-1]):
+            while (
+                stack
+                and not isinstance(stack[-1], LeftParen)
+                and comp_precedence(c, stack[-1])
+            ):
                 res.append(stack.pop())
             stack.append(c)
 
     while stack:
         res.append(stack.pop())
 
     return res
 
 
-def parse_postfix_tokens(postfix_tokens):
-    """Parse list of postfix tokens to produce value of expression."""
+def parse_postfix_tokens(
+    postfix_tokens: List[Token[ExpressionResultT]],
+) -> ExpressionResultT:
+    """Parse list of postfix tokens to produce value of expression"""
 
-    stack = deque()
+    stack: Deque[ExpressionResultT] = deque()
 
     for token in postfix_tokens:
         if isinstance(token, InfixOperator):
             right = stack.pop()
             left = stack.pop()
             stack.append(token.op(left, right))
         elif isinstance(token, PostfixOperator):
```

### Comparing `automata-lib-7.1.0/automata/regex/regex.py` & `automata-lib-8.0.0/automata/regex/regex.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,54 +1,60 @@
 #!/usr/bin/env python3
 """Methods for working with regular expressions"""
 
+from itertools import count
+from typing import AbstractSet, Optional
+
 import automata.base.exceptions as exceptions
 from automata.fa.nfa import NFA
-from automata.regex.parser import (RESERVED_CHARACTERS, get_regex_lexer,
-                                   validate_tokens)
+from automata.regex.parser import RESERVED_CHARACTERS, get_regex_lexer, validate_tokens
 
 
-def _validate(regex):
+def _validate(regex: str) -> bool:
     """Return True if the regular expression is valid"""
 
     try:
         validate(regex)
     except exceptions.InvalidRegexError:
         return False
 
     return True
 
 
-def validate(regex):
+def validate(regex: str) -> None:
     """Raise an error if the regular expression is invalid"""
     input_symbols = set(regex) - RESERVED_CHARACTERS
 
-    validate_tokens(get_regex_lexer(input_symbols).lex(regex))
-
-    return True
+    validate_tokens(get_regex_lexer(input_symbols, count(0)).lex(regex))
 
 
-def isequal(re1, re2, *, input_symbols=None):
+def isequal(
+    re1: str, re2: str, *, input_symbols: Optional[AbstractSet[str]] = None
+) -> bool:
     """Return True if both regular expressions are equivalent"""
 
     nfa1 = NFA.from_regex(re1, input_symbols=input_symbols)
     nfa2 = NFA.from_regex(re2, input_symbols=input_symbols)
 
     return nfa1 == nfa2
 
 
-def issubset(re1, re2, *, input_symbols=None):
+def issubset(
+    re1: str, re2: str, *, input_symbols: Optional[AbstractSet[str]] = None
+) -> bool:
     """Return True if re1 is a subset of re2"""
 
     nfa1 = NFA.from_regex(re1, input_symbols=input_symbols)
     nfa2 = NFA.from_regex(re2, input_symbols=input_symbols)
 
     return nfa1.union(nfa2) == nfa2
 
 
-def issuperset(re1, re2, *, input_symbols=None):
+def issuperset(
+    re1: str, re2: str, *, input_symbols: Optional[AbstractSet[str]] = None
+) -> bool:
     """Return True if re1 is a subset of re2"""
 
     nfa1 = NFA.from_regex(re1, input_symbols=input_symbols)
     nfa2 = NFA.from_regex(re2, input_symbols=input_symbols)
 
     return nfa1.union(nfa2) == nfa1
```

### Comparing `automata-lib-7.1.0/automata/tm/dtm.py` & `automata-lib-8.0.0/automata/tm/ntm.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,139 +1,176 @@
 #!/usr/bin/env python3
-"""Classes and methods for working with deterministic Turing machines."""
+"""Classes and methods for working with nondeterministic Turing machines."""
+
+from typing import AbstractSet, Generator, Mapping, Set, Tuple
 
 import automata.base.exceptions as exceptions
 import automata.tm.exceptions as tm_exceptions
 import automata.tm.tm as tm
 from automata.tm.configuration import TMConfiguration
 from automata.tm.tape import TMTape
 
-
-class DTM(tm.TM):
-    """A deterministic Turing machine."""
-
-    __slots__ = ('states', 'input_symbols', 'tape_symbols',
-                 'transitions', 'initial_state', 'blank_symbol',
-                 'final_states')
-
-    def __init__(self, *, states, input_symbols, tape_symbols,
-                 transitions, initial_state, blank_symbol,
-                 final_states):
+NTMStateT = tm.TMStateT
+NTMPathResultT = Tuple[NTMStateT, str, tm.TMDirectionT]
+NTMPathT = Mapping[str, AbstractSet[NTMPathResultT]]
+NTMTransitionsT = Mapping[NTMStateT, NTMPathT]
+
+
+class NTM(tm.TM):
+    """A nondeterministic Turing machine."""
+
+    __slots__ = (
+        "states",
+        "input_symbols",
+        "tape_symbols",
+        "transitions",
+        "initial_state",
+        "blank_symbol",
+        "final_states",
+    )
+
+    def __init__(
+        self,
+        *,
+        states: AbstractSet[NTMStateT],
+        input_symbols: AbstractSet[str],
+        tape_symbols: AbstractSet[str],
+        transitions: NTMTransitionsT,
+        initial_state: NTMStateT,
+        blank_symbol: str,
+        final_states: AbstractSet[NTMStateT],
+    ):
         """Initialize a complete Turing machine."""
         super().__init__(
             states=states,
             input_symbols=input_symbols,
             tape_symbols=tape_symbols,
             transitions=transitions,
             initial_state=initial_state,
             blank_symbol=blank_symbol,
-            final_states=final_states
+            final_states=final_states,
         )
 
-    def _validate_transition_state(self, transition_state):
+    def _validate_transition_state(self, transition_state: NTMStateT) -> None:
         if transition_state not in self.states:
             raise exceptions.InvalidStateError(
-                'transition state is not valid ({})'.format(transition_state))
+                "transition state is not valid ({})".format(transition_state)
+            )
 
-    def _validate_transition_symbols(self, state, paths):
+    def _validate_transition_symbols(
+        self, state: NTMStateT, paths: NTMTransitionsT
+    ) -> None:
         for tape_symbol in paths.keys():
             if tape_symbol not in self.tape_symbols:
                 raise exceptions.InvalidSymbolError(
-                    'transition symbol {} for state {} is not valid'.format(
-                        tape_symbol, state))
-
-    def _validate_transition_result_direction(self, result_direction):
-        if result_direction not in ('L', 'N', 'R'):
+                    "transition symbol {} for state {} is not valid".format(
+                        tape_symbol, state
+                    )
+                )
+
+    def _validate_transition_result_direction(
+        self, result_direction: tm.TMDirectionT
+    ) -> None:
+        if result_direction not in ("L", "N", "R"):
             raise tm_exceptions.InvalidDirectionError(
-                'result direction is not valid ({})'.format(
-                    result_direction))
+                "result direction is not valid ({})".format(result_direction)
+            )
 
-    def _validate_transition_result(self, result):
+    def _validate_transition_result(self, result: NTMPathResultT) -> None:
         result_state, result_symbol, result_direction = result
         if result_state not in self.states:
             raise exceptions.InvalidStateError(
-                'result state is not valid ({})'.format(result_state))
+                "result state is not valid ({})".format(result_state)
+            )
         if result_symbol not in self.tape_symbols:
             raise exceptions.InvalidSymbolError(
-                'result symbol is not valid ({})'.format(result_symbol))
+                "result symbol is not valid ({})".format(result_symbol)
+            )
         self._validate_transition_result_direction(result_direction)
 
-    def _validate_transition_results(self, paths):
-        for result in paths.values():
-            self._validate_transition_result(result)
+    def _validate_transition_results(self, paths: NTMPathT) -> None:
+        for results in paths.values():
+            for result in results:
+                self._validate_transition_result(result)
 
-    def _validate_transitions(self):
+    def _validate_transitions(self) -> None:
         for state, paths in self.transitions.items():
             self._validate_transition_state(state)
             self._validate_transition_symbols(state, paths)
             self._validate_transition_results(paths)
 
-    def _validate_final_state_transitions(self):
+    def _validate_final_state_transitions(self) -> None:
         for final_state in self.final_states:
             if final_state in self.transitions:
                 raise exceptions.FinalStateError(
-                    'final state {} has transitions defined'.format(
-                        final_state))
+                    "final state {} has transitions defined".format(final_state)
+                )
 
-    def validate(self):
-        """Return True if this DTM is internally consistent."""
+    def validate(self) -> None:
+        """Return True if this NTM is internally consistent."""
         self._read_input_symbol_subset()
         self._validate_blank_symbol()
         self._validate_transitions()
         self._validate_initial_state()
         self._validate_initial_state_transitions()
         self._validate_nonfinal_initial_state()
         self._validate_final_states()
         self._validate_final_state_transitions()
-        return True
 
-    def _get_transition(self, state, tape_symbol):
-        """Get the transiton tuple for the given state and tape symbol."""
-        if (state in self.transitions and
-                tape_symbol in self.transitions[state]):
+    def _get_transitions(
+        self, state: NTMStateT, tape_symbol: str
+    ) -> Set[NTMPathResultT]:
+        """Get the transition tuples for the given state and tape symbol."""
+        if state in self.transitions and tape_symbol in self.transitions[state]:
             return self.transitions[state][tape_symbol]
         else:
-            return None
+            return set()
 
-    def _has_accepted(self, configuration):
+    def _has_accepted(self, configuration: TMConfiguration) -> bool:
         """Check whether the given config indicates accepted input."""
         return configuration.state in self.final_states
 
-    def _get_next_configuration(self, old_config):
-        """Advance to the next configuration."""
-        transitions = {self._get_transition(
-            old_config.state,
-            old_config.tape.read_symbol()
-        )}
-        if None in transitions:
-            transitions.remove(None)
-        if len(transitions) == 0:
-            raise exceptions.RejectionException(
-                'The machine entered a non-final configuration for which no '
-                'transition is defined ({}, {})'.format(
-                    old_config.state, old_config.tape.read_symbol()))
-        tape = old_config.tape
-        (new_state, new_tape_symbol,
-            direction) = transitions.pop()
-        tape = tape.write_symbol(new_tape_symbol)
-        tape = tape.move(direction)
-        return TMConfiguration(new_state, tape)
-
-    def read_input_stepwise(self, input_str):
+    def _get_next_configurations(
+        self, old_config: TMConfiguration
+    ) -> Set[TMConfiguration]:
+        """Advance to the next configurations."""
+        transitions = self._get_transitions(
+            old_config.state, old_config.tape.read_symbol()
+        )
+        new_configs = set()
+        for new_state, new_tape_symbol, direction in transitions:
+            tape = old_config.tape
+            tape = tape.write_symbol(new_tape_symbol)
+            tape = tape.move(direction)
+            new_configs.add(TMConfiguration(new_state, tape))
+        return new_configs
+
+    def read_input_stepwise(
+        self, input_str: str
+    ) -> Generator[Set[TMConfiguration], None, None]:
         """
         Check if the given string is accepted by this Turing machine.
 
-        Yield the current configuration of the machine at each step.
+        Yield the current configurations of the machine at each step.
         """
-        current_configuration = TMConfiguration(
-            self.initial_state,
-            TMTape(input_str, blank_symbol=self.blank_symbol)
-        )
-        yield current_configuration
+        current_configurations = {
+            TMConfiguration(
+                self.initial_state, TMTape(input_str, blank_symbol=self.blank_symbol)
+            )
+        }
+        yield current_configurations
 
-        # The initial state cannot be a final state for a DTM, so the first
+        # The initial state cannot be a final state for a NTM, so the first
         # iteration is always guaranteed to run (as it should)
-        while not self._has_accepted(current_configuration):
-            current_configuration = self._get_next_configuration(
-                current_configuration
-            )
-            yield current_configuration
+        while current_configurations:
+            new_configurations = set()
+            for config in current_configurations:
+                if self._has_accepted(config):
+                    # One accepting configuration is enough.
+                    return
+                new_configurations.update(self._get_next_configurations(config))
+            current_configurations = new_configurations
+            yield current_configurations
+
+        raise exceptions.RejectionException(
+            "the NTM did not reach an accepting configuration"
+        )
```

### Comparing `automata-lib-7.1.0/automata/tm/exceptions.py` & `automata-lib-8.0.0/automata/tm/exceptions.py`

 * *Files identical despite different names*

### Comparing `automata-lib-7.1.0/automata/tm/mntm.py` & `automata-lib-8.0.0/automata/tm/mntm.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,301 +1,333 @@
 #!/usr/bin/env python3
 """Classes and methods for working with multitape nondeterministic Turing
 machines."""
 
 from collections import deque
+from itertools import chain
+from typing import AbstractSet, Any, Generator, Mapping, Optional, Sequence, Tuple
 
 import automata.base.exceptions as exceptions
 import automata.tm.exceptions as tm_exceptions
 import automata.tm.ntm as ntm
 import automata.tm.tm as tm
 from automata.tm.configuration import MTMConfiguration, TMConfiguration
 from automata.tm.tape import TMTape
 
+MNTMStateT = ntm.NTMStateT
+MNTMPathResultT = Tuple[str, Tuple[Tuple[str, tm.TMDirectionT], ...]]
+MNTMPathT = Mapping[Tuple[str, ...], Sequence[MNTMPathResultT]]
+MNTMTransitionsT = Mapping[str, MNTMPathT]
+
 
 class MNTM(ntm.NTM):
     """A multitape nondeterministic Turing machine."""
 
-    __slots__ = ('states', 'input_symbols', 'tape_symbols', 'n_tapes',
-                 'transitions', 'initial_state', 'blank_symbol', 'final_states')
-
-    def __init__(self, *, states, input_symbols, tape_symbols, n_tapes,
-                 transitions, initial_state, blank_symbol, final_states):
+    __slots__ = (
+        "states",
+        "input_symbols",
+        "tape_symbols",
+        "n_tapes",
+        "transitions",
+        "initial_state",
+        "blank_symbol",
+        "final_states",
+    )
+
+    transitions: MNTMTransitionsT  # type: ignore
+    n_tapes: int
+
+    def __init__(
+        self,
+        *,
+        states: AbstractSet[MNTMStateT],
+        input_symbols: AbstractSet[str],
+        tape_symbols: AbstractSet[str],
+        n_tapes: int,
+        transitions: MNTMTransitionsT,
+        initial_state: MNTMStateT,
+        blank_symbol: str,
+        final_states: AbstractSet[MNTMStateT],
+    ):
         """Initialize a complete Turing machine."""
         super(tm.TM, self).__init__(
             states=states,
             input_symbols=input_symbols,
             tape_symbols=tape_symbols,
             transitions=transitions,
             initial_state=initial_state,
             blank_symbol=blank_symbol,
             final_states=final_states,
-            n_tapes=n_tapes
+            n_tapes=n_tapes,
         )
 
-    def _validate_transition_symbols(self, state, paths):
-        for tape_symbol in [tape_symbol
-                            for symbol in paths.keys() for tape_symbol in
-                            symbol]:
+    def _validate_transition_symbols(self, state: MNTMStateT, paths: Mapping) -> None:
+        for tape_symbol in [
+            tape_symbol for symbol in paths.keys() for tape_symbol in symbol
+        ]:
             if tape_symbol not in self.tape_symbols:
                 raise exceptions.InvalidSymbolError(
-                    'transition symbol {} for state {} is not valid'.format(
+                    "transition symbol {} for state {} is not valid".format(
                         tape_symbol, state
                     )
                 )
 
-    def _validate_transition_state(self, transition_state):
+    def _validate_transition_state(self, transition_state: MNTMStateT) -> None:
         if transition_state not in self.states:
             raise exceptions.InvalidStateError(
-                'transition state is not valid ({})'.format(transition_state)
+                "transition state is not valid ({})".format(transition_state)
             )
 
-    def _validate_transition_results(self, paths):
+    def _validate_transition_results(self, paths: Mapping) -> None:
         for results in paths.values():
             for result in results:
                 state, moves = result
                 for move in moves:
                     symbol, direction = move
                     possible_result = (state, symbol, direction)
                     self._validate_transition_result(possible_result)
 
-    def _validate_tapes_consistency(self):
+    def _validate_tapes_consistency(self) -> None:
         for state in self.transitions:
             for read_tape_symbols in self.transitions[state]:
                 if len(read_tape_symbols) != self.n_tapes:
                     error = (
-                        'tapes symbols {} inconsistent with the number of '
-                        'tapes defined. Expected {} symbols, got {}'
-                    ).format(
-                        read_tape_symbols,
-                        self.n_tapes,
-                        len(read_tape_symbols)
-                    )
-                    raise tm_exceptions.InconsistentTapesException(
-                        error
-                    )
+                        "tapes symbols {} inconsistent with the number of "
+                        "tapes defined. Expected {} symbols, got {}"
+                    ).format(read_tape_symbols, self.n_tapes, len(read_tape_symbols))
+                    raise tm_exceptions.InconsistentTapesException(error)
                 for transition in self.transitions[state][read_tape_symbols]:
                     _, moves = transition
                     if len(moves) != self.n_tapes:
                         error = (
-                            'transition {} has inconsistent operations on '
-                            'tapes. Expected {} write/move operations, '
-                            'got {}'
-                        ).format(
-                            transition,
-                            self.n_tapes,
-                            len(moves)
-                        )
-                        raise tm_exceptions.InconsistentTapesException(
-                            error
-                        )
+                            "transition {} has inconsistent operations on "
+                            "tapes. Expected {} write/move operations, "
+                            "got {}"
+                        ).format(transition, self.n_tapes, len(moves))
+                        raise tm_exceptions.InconsistentTapesException(error)
 
-    def validate(self):
+    def validate(self) -> None:
         """Return True if this MNTM is internally consistent."""
         super().validate()
         self._validate_tapes_consistency()
-        return True
 
-    def _get_tapes_for_input_str(self, input_str):
+    def _get_tapes_for_input_str(self, input_str: str) -> Tuple[TMTape, ...]:
         """Produce a new list of tapes based on an input string to be read."""
-        return [
+        return (
             # Input is saved on first tape
             TMTape(input_str, blank_symbol=self.blank_symbol),
             # The rest of the tapes have blanks
             *(
-                TMTape(self.blank_symbol,
-                       blank_symbol=self.blank_symbol,
-                       current_position=0)
+                TMTape(
+                    self.blank_symbol,
+                    blank_symbol=self.blank_symbol,
+                    current_position=0,
+                )
                 for _ in range(self.n_tapes - 1)
-            )
-        ]
+            ),
+        )
 
-    def _read_current_tape_symbols(self, tapes):
+    def _read_current_tape_symbols(self, tapes: Tuple[TMTape, ...]) -> Tuple[str, ...]:
         """Reads the current tape symbols in each of the tapes and their
         corresponding heads."""
         return tuple(tape.read_symbol() for tape in tapes)
 
-    def _get_transition(self, current_state, tapes):
+    def _get_transition(
+        self, current_state: MNTMStateT, tapes: Tuple[TMTape, ...]
+    ) -> Optional[Sequence[MNTMPathResultT]]:
         """Get the transition tuple for the given state and tape symbols in
         each tape."""
         current_tape_symbols = self._read_current_tape_symbols(tapes)
-        if current_state in self.transitions and current_tape_symbols in \
-                self.transitions[current_state]:
+        if (
+            current_state in self.transitions
+            and current_tape_symbols in self.transitions[current_state]
+        ):
             return self.transitions[current_state][
                 self._read_current_tape_symbols(tapes)
             ]
         else:
             return None
 
-    def _get_next_configuration(self, transition, current_tapes):
+    def _get_next_configuration(
+        self, transition: MNTMPathResultT, current_tapes: Tuple[TMTape, ...]
+    ) -> MTMConfiguration:
         """Advances to the next configuration."""
         current_state, moves = transition
-        tapes = current_tapes.copy()
-        for i, move in enumerate(moves):
-            symbol, direction = move
-            tapes[i] = tapes[i].write_symbol(symbol)
-            tapes[i] = tapes[i].move(direction)
+        tapes = tuple(
+            tape.write_symbol(symbol).move(direction)
+            for (symbol, direction), tape in zip(moves, current_tapes)
+        )
 
         return MTMConfiguration(state=current_state, tapes=tapes)
 
-    def _has_accepted(self, current_config):
-        return current_config.state in self.final_states
-
-    def read_input_stepwise(self, input_str):
+    def read_input_stepwise(self, input_str: str) -> Generator[Any, None, Any]:
+        # TODO Any type above should be Set[MTMConfiguration], refactor required
         """Checks if the given string is accepted by this Turing machine,
         using a BFS of every possible configuration from each configuration.
         Yields the current configuration of the machine at each step.
         """
         tapes = self._get_tapes_for_input_str(input_str)
-        queue = deque([(
-            MTMConfiguration(state=self.initial_state, tapes=tapes[:])
-        )])
+        queue = deque([(MTMConfiguration(state=self.initial_state, tapes=tapes))])
         while len(queue) > 0:
             current_config = queue.popleft()
-            yield {MTMConfiguration(current_config.state, tuple(current_config.tapes))}
+            yield {MTMConfiguration(current_config.state, current_config.tapes)}
 
-            possible_transitions = self._get_transition(current_config.state, current_config.tapes)
+            possible_transitions = self._get_transition(
+                current_config.state, current_config.tapes
+            )
             if possible_transitions is None:
-                if self._has_accepted(current_config):
-                    return {MTMConfiguration(current_config.state,
-                                             tuple(current_config.tapes))}
+                if current_config.state in self.final_states:
+                    return {
+                        MTMConfiguration(current_config.state, current_config.tapes)
+                    }
             else:
                 for transition in possible_transitions[1:]:
-                    queue.append(self._get_next_configuration(
-                        transition,
-                        current_tapes=current_config.tapes))
-
-                queue.append(self._get_next_configuration(
-                    possible_transitions[0],
-                    current_tapes=current_config.tapes))
+                    queue.append(
+                        self._get_next_configuration(
+                            transition, current_tapes=current_config.tapes
+                        )
+                    )
+
+                queue.append(
+                    self._get_next_configuration(
+                        possible_transitions[0], current_tapes=current_config.tapes
+                    )
+                )
 
         raise exceptions.RejectionException(
-            'the multitape MNTM did not reach an accepting configuration'
+            "the multitape MNTM did not reach an accepting configuration"
         )
 
     @staticmethod
-    def _read_extended_tape(tape: str, head_symbol: str = '^',
-                            tape_separator_symbol: str = '_'):
+    def _read_extended_tape(
+        tape: str, head_symbol: str = "^", tape_separator_symbol: str = "_"
+    ) -> Tuple[str, ...]:
         """Returns a tuple with the symbols extracted from the given
         tape, that are the virtual heads for their corresponding
         virtual tape."""
         virtual_heads = []
         heads_found = 0
         separators_found = 0
         for i, symbol in enumerate(tape):
             if symbol == head_symbol:
                 if i - 1 < 0:
                     raise tm_exceptions.MalformedExtendedTapeError(
-                        'head symbol was found on leftmost end of the '
-                        'extended tape'
+                        "head symbol was found on leftmost end of the " "extended tape"
                     )
                 else:
                     previous_symbol = tape[i - 1]
                     virtual_heads.append(previous_symbol)
                     heads_found += 1
             elif symbol == tape_separator_symbol:
                 if heads_found == 0:
                     raise tm_exceptions.MalformedExtendedTapeError(
-                        'no head symbol found on one of the virtual tapes'
+                        "no head symbol found on one of the virtual tapes"
                     )
                 elif heads_found > 1:
                     raise tm_exceptions.MalformedExtendedTapeError(
-                        'more than one head symbol found on one of the '
-                        'virtual tapes'
+                        "more than one head symbol found on one of the " "virtual tapes"
                     )
                 else:
                     heads_found = 0
                     separators_found += 1
 
         if len(virtual_heads) != separators_found:
             raise tm_exceptions.MalformedExtendedTapeError(
-                'there must be 1 virtual head for every tape separator symbol'
+                "there must be 1 virtual head for every tape separator symbol"
             )
 
         return tuple(virtual_heads)
 
-    def read_input_as_ntm(self, input_str):
+    def read_input_as_ntm(
+        self, input_str: str
+    ) -> Generator[AbstractSet[TMConfiguration], None, None]:
         """Simulates the machine as a single-tape Turing machine.
         Yields the configuration at each step."""
         tapes = self._get_tapes_for_input_str(input_str)
-        head_symbol = '^'
-        tape_separator_symbol = '_'
-        extended_tape = ''
-        tapes_copy = tapes.copy()
-        for tape_copy in tapes_copy:
-            tape_str = tape_copy.get_symbols_as_str()
-            extended_tape += tape_str[0] + head_symbol + \
-                tape_str[1:] + tape_separator_symbol
+        head_symbol = "^"
+        tape_separator_symbol = "_"
+
+        # Make string from all tapes
+        extended_tape = "".join(
+            chain.from_iterable(
+                (tape.tape[0], head_symbol, *tape.tape[1:], tape_separator_symbol)
+                for tape in tapes
+            )
+        )
 
         current_state = self.initial_state
         yield {
-            TMConfiguration(current_state,
-                            TMTape(extended_tape,
-                                   blank_symbol=self.blank_symbol,
-                                   current_position=0)
-                            )
+            TMConfiguration(
+                current_state,
+                TMTape(
+                    extended_tape, blank_symbol=self.blank_symbol, current_position=0
+                ),
+            )
         }
 
         # If the machine has not reached an accepting state.
         while current_state not in self.final_states:
             i = 0  # current position
-            virtual_heads = self._read_extended_tape(extended_tape,
-                                                     head_symbol,
-                                                     tape_separator_symbol)
+            virtual_heads = self._read_extended_tape(
+                extended_tape, head_symbol, tape_separator_symbol
+            )
             try:
                 next_config = self.transitions[current_state][virtual_heads]
             except KeyError:
                 raise exceptions.RejectionException(
-                    'the multitape NTM did not reach an accepting '
-                    'configuration')
+                    "the multitape NTM did not reach an accepting " "configuration"
+                )
             next_state, moves = next_config[0]
             for move in moves:
                 new_head, direction = move
                 executing_changes = True
 
                 while executing_changes:
                     if extended_tape[i] == head_symbol:
                         # Head has been found (previous symbol is the head).
                         # This replaces the previous symbol with the new_head.
                         extended_tape = (
-                            extended_tape[: i - 1] +
-                            new_head + extended_tape[i:]
+                            extended_tape[: i - 1] + new_head + extended_tape[i:]
                         )
-                        extended_tape = extended_tape[:i] + \
-                            '' + extended_tape[i + 1:]
+                        extended_tape = extended_tape[:i] + "" + extended_tape[i + 1 :]
 
                         # After replacing, the machine must change the
                         # position of the virtual head of the current virtual
                         # tape.
-                        if direction == 'R':
+                        if direction == "R":
                             i += 1
-                        elif direction == 'L':
+                        elif direction == "L":
                             i -= 1
                         else:  # direction == 'N'
                             i += 0
 
                         if extended_tape[i - 1] == tape_separator_symbol:
                             i -= 1
-                            extended_tape = extended_tape[:i] + \
-                                self.blank_symbol + \
-                                head_symbol + extended_tape[i:]
+                            extended_tape = (
+                                extended_tape[:i]
+                                + self.blank_symbol
+                                + head_symbol
+                                + extended_tape[i:]
+                            )
 
                             i += 1
                         else:
                             extended_tape = (
-                                extended_tape[:i] +
-                                head_symbol + extended_tape[i:]
+                                extended_tape[:i] + head_symbol + extended_tape[i:]
                             )
 
                     elif extended_tape[i] == tape_separator_symbol:
                         executing_changes = False
 
                     i += 1
 
             current_state = next_state
             yield {
-                TMConfiguration(current_state,
-                                TMTape(extended_tape,
-                                       blank_symbol=self.blank_symbol,
-                                       current_position=i-1)
-                                )
+                TMConfiguration(
+                    current_state,
+                    TMTape(
+                        extended_tape,
+                        blank_symbol=self.blank_symbol,
+                        current_position=i - 1,
+                    ),
+                )
             }
```

### Comparing `automata-lib-7.1.0/automata/tm/ntm.py` & `automata-lib-8.0.0/automata/pda/dpda.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,148 +1,174 @@
 #!/usr/bin/env python3
-"""Classes and methods for working with nondeterministic Turing machines."""
+"""Classes and methods for working with deterministic pushdown automata."""
 
-import automata.base.exceptions as exceptions
-import automata.tm.exceptions as tm_exceptions
-import automata.tm.tm as tm
-from automata.tm.configuration import TMConfiguration
-from automata.tm.tape import TMTape
-
-
-class NTM(tm.TM):
-    """A nondeterministic Turing machine."""
+from typing import AbstractSet, Generator, Mapping, Optional, Set, Tuple, Union
 
-    __slots__ = ('states', 'input_symbols', 'tape_symbols', 'transitions',
-                 'initial_state', 'blank_symbol', 'final_states')
+import automata.base.exceptions as exceptions
+import automata.pda.exceptions as pda_exceptions
+import automata.pda.pda as pda
+from automata.pda.configuration import PDAConfiguration
+from automata.pda.stack import PDAStack
+
+DPDAStateT = pda.PDAStateT
+
+DPDAPathT = Mapping[str, Mapping[str, Tuple[DPDAStateT, Union[str, Tuple[str, ...]]]]]
+DPDATransitionsT = Mapping[DPDAStateT, DPDAPathT]
+
+
+class DPDA(pda.PDA):
+    """A deterministic pushdown automaton."""
+
+    __slots__ = (
+        "states",
+        "input_symbols",
+        "stack_symbols",
+        "transitions",
+        "initial_state",
+        "initial_stack_symbol",
+        "final_states",
+        "acceptance_mode",
+    )
 
     def __init__(
-            self, *, states, input_symbols, tape_symbols, transitions,
-            initial_state, blank_symbol, final_states):
-        """Initialize a complete Turing machine."""
+        self,
+        *,
+        states: AbstractSet[DPDAStateT],
+        input_symbols: AbstractSet[str],
+        stack_symbols: AbstractSet[str],
+        transitions: DPDATransitionsT,
+        initial_state: DPDAStateT,
+        initial_stack_symbol: str,
+        final_states: AbstractSet[DPDAStateT],
+        acceptance_mode: pda.PDAAcceptanceModeT = "both",
+    ) -> None:
+        """Initialize a complete DPDA."""
         super().__init__(
             states=states,
             input_symbols=input_symbols,
-            tape_symbols=tape_symbols,
+            stack_symbols=stack_symbols,
             transitions=transitions,
             initial_state=initial_state,
-            blank_symbol=blank_symbol,
-            final_states=final_states
+            initial_stack_symbol=initial_stack_symbol,
+            final_states=final_states,
+            acceptance_mode=acceptance_mode,
         )
 
-    def _validate_transition_state(self, transition_state):
-        if transition_state not in self.states:
-            raise exceptions.InvalidStateError(
-                'transition state is not valid ({})'.format(transition_state)
-            )
+    def _validate_transition_invalid_symbols(
+        self, start_state: DPDAStateT, paths: DPDATransitionsT
+    ) -> None:
+        """Raise an error if transition symbols are invalid."""
+        for input_symbol, symbol_paths in paths.items():
+            self._validate_transition_invalid_input_symbols(start_state, input_symbol)
+            for stack_symbol in symbol_paths:
+                self._validate_transition_isolated_lambda_transitions(
+                    start_state, input_symbol, stack_symbol
+                )
+                self._validate_transition_invalid_stack_symbols(
+                    start_state, stack_symbol
+                )
 
-    def _validate_transition_symbols(self, state, paths):
-        for tape_symbol in paths.keys():
-            if tape_symbol not in self.tape_symbols:
-                raise exceptions.InvalidSymbolError(
-                    'transition symbol {} for state {} is not valid'.format(
-                        tape_symbol, state
-                    )
+    def _validate_transition_lambda_transition_sibling(
+        self, start_state: DPDAStateT, sib_path: DPDAPathT
+    ) -> None:
+        """Check the given sibling path for adjacent lambda transitions."""
+        for other_stack_symbol in sib_path:
+            if other_stack_symbol in self.transitions[start_state][""]:
+                raise pda_exceptions.NondeterminismError(
+                    "A symbol transition is adjacent to a "
+                    "lambda transition for this DPDA."
                 )
 
-    def _validate_transition_result_direction(self, result_direction):
-        if result_direction not in ("L", "N", "R"):
-            raise tm_exceptions.InvalidDirectionError(
-                'result direction is not valid ({})'.format(result_direction)
+    def _validate_transition_isolated_lambda_transitions(
+        self, start_state: DPDAStateT, input_symbol: str, stack_symbol: str
+    ) -> None:
+        """Raise an error if a lambda transition has no sibling transitions."""
+        if input_symbol == "":
+            sib_transitions = self.transitions[start_state]
+            for sib_input_symbol, sib_path in sib_transitions.items():
+                if sib_input_symbol != "":
+                    self._validate_transition_lambda_transition_sibling(
+                        start_state, sib_path
+                    )
+
+    def _get_transition(
+        self, state: DPDAStateT, input_symbol: str, stack_symbol: str
+    ) -> Optional[DPDAPathT]:
+        """Get the transiton tuple for the given state and symbols."""
+        if (
+            state in self.transitions
+            and input_symbol in self.transitions[state]
+            and stack_symbol in self.transitions[state][input_symbol]
+        ):
+            return (input_symbol,) + self.transitions[state][input_symbol][stack_symbol]
+        else:
+            return None
+
+    def _check_for_input_rejection(
+        self, current_configuration: PDAConfiguration
+    ) -> None:
+        """Raise an error if the given config indicates rejected input."""
+        if not self._has_accepted(current_configuration):
+            raise exceptions.RejectionException(
+                "the DPDA stopped in a non-accepting configuration "
+                "({}, {})".format(
+                    current_configuration.state, current_configuration.stack
+                )
             )
 
-    def _validate_transition_result(self, result):
-        result_state, result_symbol, result_direction = result
-        if result_state not in self.states:
-            raise exceptions.InvalidStateError(
-                'result state is not valid ({})'.format(result_state)
+    def _get_next_configuration(self, old_config: PDAConfiguration) -> PDAConfiguration:
+        """Advance to the next configuration."""
+        transitions: Set[Optional[DPDAPathT]] = set()
+        if old_config.remaining_input:
+            transitions.add(
+                self._get_transition(
+                    old_config.state,
+                    old_config.remaining_input[0],
+                    old_config.stack.top(),
+                )
             )
-        if result_symbol not in self.tape_symbols:
-            raise exceptions.InvalidSymbolError(
-                'result symbol is not valid ({})'.format(result_symbol)
+        transitions.add(
+            self._get_transition(old_config.state, "", old_config.stack.top())
+        )
+        if None in transitions:
+            transitions.remove(None)
+        if len(transitions) == 0:
+            raise exceptions.RejectionException(
+                "The automaton entered a configuration for which no "
+                "transition is defined ({}, {}, {})".format(
+                    old_config.state,
+                    old_config.remaining_input[0],
+                    old_config.stack.top(),
+                )
             )
-        self._validate_transition_result_direction(result_direction)
-
-    def _validate_transition_results(self, paths):
-        for results in paths.values():
-            for result in results:
-                self._validate_transition_result(result)
-
-    def _validate_transitions(self):
-        for state, paths in self.transitions.items():
-            self._validate_transition_state(state)
-            self._validate_transition_symbols(state, paths)
-            self._validate_transition_results(paths)
-
-    def _validate_final_state_transitions(self):
-        for final_state in self.final_states:
-            if final_state in self.transitions:
-                raise exceptions.FinalStateError(
-                    'final state {} has transitions defined'.format(
-                        final_state))
-
-    def validate(self):
-        """Return True if this NTM is internally consistent."""
-        self._read_input_symbol_subset()
-        self._validate_blank_symbol()
-        self._validate_transitions()
-        self._validate_initial_state()
-        self._validate_initial_state_transitions()
-        self._validate_nonfinal_initial_state()
-        self._validate_final_states()
-        self._validate_final_state_transitions()
-        return True
-
-    def _get_transitions(self, state, tape_symbol):
-        """Get the transition tuples for the given state and tape symbol."""
-        if state in self.transitions and tape_symbol in self.transitions[
-                state]:
-            return self.transitions[state][tape_symbol]
-        else:
-            return set()
-
-    def _has_accepted(self, configuration):
-        """Check whether the given config indicates accepted input."""
-        return configuration.state in self.final_states
-
-    def _get_next_configurations(self, old_config):
-        """Advance to the next configurations."""
-        transitions = self._get_transitions(
-            old_config.state, old_config.tape.read_symbol()
+        input_symbol, new_state, new_stack_top = transitions.pop()  # type: ignore
+        remaining_input = old_config.remaining_input
+        if input_symbol:
+            remaining_input = remaining_input[1:]
+        new_config = PDAConfiguration(
+            new_state,
+            remaining_input,
+            self._replace_stack_top(old_config.stack, new_stack_top),
         )
-        new_configs = set()
-        for new_state, new_tape_symbol, direction in transitions:
-            tape = old_config.tape
-            tape = tape.write_symbol(new_tape_symbol)
-            tape = tape.move(direction)
-            new_configs.add(TMConfiguration(new_state, tape))
-        return new_configs
+        return new_config
 
-    def read_input_stepwise(self, input_str):
+    def read_input_stepwise(
+        self, input_str: str
+    ) -> Generator[PDAConfiguration, None, None]:
         """
-        Check if the given string is accepted by this Turing machine.
+        Check if the given string is accepted by this DPDA.
 
-        Yield the current configurations of the machine at each step.
+        Yield the DPDA's current configuration at each step.
         """
-        current_configurations = {
-            TMConfiguration(
-                self.initial_state,
-                TMTape(
-                    input_str,
-                    blank_symbol=self.blank_symbol))}
-        yield current_configurations
-
-        # The initial state cannot be a final state for a NTM, so the first
-        # iteration is always guaranteed to run (as it should)
-        while current_configurations:
-            new_configurations = set()
-            for config in current_configurations:
-                if self._has_accepted(config):
-                    # One accepting configuration is enough.
-                    return
-                new_configurations.update(
-                    self._get_next_configurations(config))
-            current_configurations = new_configurations
-            yield current_configurations
-
-        raise exceptions.RejectionException(
-            "the NTM did not reach an accepting configuration"
+        current_configuration = PDAConfiguration(
+            self.initial_state, input_str, PDAStack([self.initial_stack_symbol])
         )
+
+        yield current_configuration
+        while current_configuration.remaining_input or self._has_lambda_transition(
+            current_configuration.state, current_configuration.stack.top()
+        ):
+            current_configuration = self._get_next_configuration(current_configuration)
+            yield current_configuration
+            if self._has_accepted(current_configuration):
+                return
+        self._check_for_input_rejection(current_configuration)
```

### Comparing `automata-lib-7.1.0/automata/tm/tape.py` & `automata-lib-8.0.0/automata/tm/tape.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,81 +1,94 @@
 #!/usr/bin/env python3
 """Classes and methods for working with Turing machine tapes."""
 
-import collections
+from dataclasses import dataclass
+from typing import Iterator, Sequence, Tuple
 
+from typing_extensions import Self
 
-class TMTape(collections.namedtuple(
-    'TMTape',
-    ['tape', 'blank_symbol', 'current_position']
-)):
+from automata.tm.tm import TMDirectionT
+
+
+@dataclass(frozen=True)
+class TMTape:
     """A Turing machine tape."""
 
-    def __new__(cls, tape, *, blank_symbol, current_position=0):
+    __slots__ = ("tape", "blank_symbol", "current_position")
+
+    tape: Tuple[str]
+    blank_symbol: str
+    current_position: int
+
+    def __init__(
+        self, tape: Sequence[str], blank_symbol: str, current_position: int = 0
+    ) -> None:
         """Initialize a new Turing machine tape."""
         tape = list(tape)
         # Make sure that there's something under the cursor.
         while len(tape) <= current_position:
             tape.append(blank_symbol)
-        tape = tuple(tape)
-        return super(TMTape, cls).__new__(
-            cls, tape, blank_symbol, current_position
-        )
+        object.__setattr__(self, "tape", tuple(tape))
+        object.__setattr__(self, "blank_symbol", blank_symbol)
+        object.__setattr__(self, "current_position", current_position)
 
-    def read_symbol(self):
+    def read_symbol(self) -> str:
         """Read the symbol at the current position in the tape."""
         return self.tape[self.current_position]
 
-    def write_symbol(self, new_tape_symbol):
+    def write_symbol(self, new_tape_symbol: str) -> Self:
         """Write the given symbol at the current position in the tape."""
         tape_elements = list(self.tape)
         tape_elements[self.current_position] = new_tape_symbol
-        return TMTape(
+        return self.__class__(
             tape_elements,
             blank_symbol=self.blank_symbol,
-            current_position=self.current_position
+            current_position=self.current_position,
         )
 
-    def move(self, direction):
+    def move(self, direction: TMDirectionT) -> Self:
         """Move the tape to the next symbol in the given direction."""
         # Copy stuff.
         new_tape = list(self.tape)
         new_position = self.current_position
-        if direction == 'R':
+        if direction == "R":
             new_position += 1
-        elif direction == 'N':
+        elif direction == "N":
             pass
-        elif direction == 'L':  # pragma: no branch
+        elif direction == "L":  # pragma: no branch
             new_position -= 1
         # Make sure that the cursor doesn't run off the end of the tape.
         if new_position == -1:
             new_tape.insert(0, self.blank_symbol)
             new_position += 1
         if new_position == len(new_tape):
             new_tape.append(self.blank_symbol)
-        return TMTape(
-            new_tape,
-            blank_symbol=self.blank_symbol,
-            current_position=new_position
+        return self.__class__(
+            new_tape, blank_symbol=self.blank_symbol, current_position=new_position
         )
 
-    def copy(self):
-        return TMTape(list(self.tape).copy(),
-                      blank_symbol=self.blank_symbol,
-                      current_position=self.current_position)
+    def copy(self) -> Self:
+        return self.__class__(
+            list(self.tape).copy(),
+            blank_symbol=self.blank_symbol,
+            current_position=self.current_position,
+        )
 
-    def get_symbols_as_str(self):
+    def get_symbols_as_str(self) -> str:
         return "".join(self.tape)
 
-    def __len__(self):
+    def __len__(self) -> int:
         """Return the number of symbols on the tape."""
         return len(self.tape)  # TODO: do we count the blank symbols?
 
-    def __iter__(self):
+    def __iter__(self) -> Iterator[str]:
         """Return an interator for the tape."""
         return iter(self.tape)
 
-    def __repr__(self):
+    def __repr__(self) -> str:
         """Return a string representation of the tape."""
-        return '{}(\'{}\', {})'.format(
-            self.__class__.__name__, ''.join(self.tape), self.current_position
+        return "{}({!r}, {!r}, {!r})".format(
+            self.__class__.__name__,
+            "".join(self.tape),
+            self.blank_symbol,
+            self.current_position,
         )
```

### Comparing `automata-lib-7.1.0/automata/tm/tm.py` & `automata-lib-8.0.0/automata/tm/tm.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,41 @@
 #!/usr/bin/env python3
 """Classes and methods for working with all Turing machines."""
 
 import abc
+from typing import AbstractSet, Literal
 
 import automata.base.exceptions as exceptions
-from automata.base.automaton import Automaton
+from automata.base.automaton import Automaton, AutomatonStateT
+
+TMStateT = AutomatonStateT
+TMDirectionT = Literal["L", "R", "N"]
 
 
 class TM(Automaton, metaclass=abc.ABCMeta):
     """An abstract base class for Turing machines."""
 
-    def _read_input_symbol_subset(self):
+    __slots__ = tuple()
+
+    tape_symbols: AbstractSet[str]
+    blank_symbol: str
+
+    def _read_input_symbol_subset(self) -> None:
         if not (self.input_symbols < self.tape_symbols):
             raise exceptions.MissingSymbolError(
-                'The set of tape symbols is missing symbols from the input '
-                'symbol set ({})'.format(
-                    self.tape_symbols - self.input_symbols))
+                "The set of tape symbols is missing symbols from the input "
+                "symbol set ({})".format(self.tape_symbols - self.input_symbols)
+            )
 
-    def _validate_blank_symbol(self):
+    def _validate_blank_symbol(self) -> None:
         """Raise an error if blank symbol is not a tape symbol."""
         if self.blank_symbol not in self.tape_symbols:
             raise exceptions.InvalidSymbolError(
-                'blank symbol {} is not a tape symbol'.format(
-                    self.blank_symbol))
+                "blank symbol {} is not a tape symbol".format(self.blank_symbol)
+            )
 
-    def _validate_nonfinal_initial_state(self):
+    def _validate_nonfinal_initial_state(self) -> None:
         """Raise an error if the initial state is a final state."""
         if self.initial_state in self.final_states:
             raise exceptions.InitialStateError(
-                'initial state {} cannot be a final state'.format(
-                    self.initial_state))
+                "initial state {} cannot be a final state".format(self.initial_state)
+            )
```

### Comparing `automata-lib-7.1.0/automata_lib.egg-info/PKG-INFO` & `automata-lib-8.0.0/automata_lib.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: automata-lib
-Version: 7.1.0
+Version: 8.0.0
 Summary: A Python library for simulating finite automata, pushdown automata, and Turing machines
 Author-email: Caleb Evans <caleb@calebevans.me>
-Maintainer-email: Caleb Evans <caleb@calebevans.me>
+Maintainer-email: Caleb Evans <caleb@calebevans.me>, "Eliot W. Robson" <eliot.robson24@gmail.com>
 License: The MIT License (MIT)
         
-        Copyright (c) 2016-2022 Caleb Evans
+        Copyright (c) 2016-2023 Caleb Evans
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
         copies of the Software, and to permit persons to whom the Software is
         furnished to do so, subject to the following conditions:
@@ -27,59 +27,71 @@
         THE SOFTWARE.
         
 Project-URL: homepage, https://github.com/caleb531/automata
 Project-URL: documentation, https://github.com/caleb531/automata#readme
 Project-URL: repository, https://github.com/caleb531/automata
 Project-URL: changelog, https://github.com/caleb531/automata/releases
 Keywords: automata,finite,non-deterministic,pushdown,turing,machine,state
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Provides-Extra: visual
 License-File: LICENSE.txt
 
 # Automata
 
-*Copyright 2016-2022 Caleb Evans*  
+*Copyright 2016-2023 Caleb Evans*  
 *Released under the MIT license*
 
 [![tests](https://github.com/caleb531/automata/actions/workflows/tests.yml/badge.svg)](https://github.com/caleb531/automata/actions/workflows/tests.yml)
 [![Coverage Status](https://coveralls.io/repos/caleb531/automata/badge.svg?branch=main)](https://coveralls.io/r/caleb531/automata?branch=main)
 
 Automata is a Python 3 library which implements the structures and algorithms
 for finite automata, pushdown automata, and Turing machines. The library
-requires Python 3.7 or newer.
+requires Python 3.8 or newer.
 
-Huge thanks to [@YtvwlD][YtvwlD], [@dengl11][dengl11], [@Tagl][Tagl],
-[@lewiuberg][lewiuberg], [@CamiloMartinezM][CamiloMartinezM],
-[@abhinavsinha‑adrino][abhinavsinha-adrino], and [@eliotwrobson][eliotwrobson]
-for their invaluable code contributions to this project! 🎉
+Huge thanks to [@eliotwrobson][eliotwrobson], [@YtvwlD][YtvwlD],
+[@dengl11][dengl11], [@Tagl][Tagl], [@lewiuberg][lewiuberg],
+[@CamiloMartinezM][CamiloMartinezM],
+[@abhinavsinha‑adrino][abhinavsinha-adrino],
+[@EduardoGoulart1][EduardoGoulart1], and
+[@khoda81][khoda81] for their invaluable code contributions to
+this project! 🎉
 
+[eliotwrobson]: https://github.com/eliotwrobson
 [YtvwlD]: https://github.com/YtvwlD
 [dengl11]: https://github.com/dengl11
 [Tagl]: https://github.com/Tagl
 [lewiuberg]: https://github.com/lewiuberg
 [CamiloMartinezM]: https://github.com/CamiloMartinezM
 [abhinavsinha-adrino]: https://github.com/abhinavsinha-adrino
-[eliotwrobson]: https://github.com/eliotwrobson
+[EduardoGoulart1]: https://github.com/EduardoGoulart1
+[khoda81]: https://github.com/khoda81
 
-## Migrating to v7
+## Migrating to v8
 
-If you wish to migrate to Automata v7 from an older version, please follow the
+If you wish to migrate to Automata v8 from an older version, please follow the
 [migration guide][migration].
 
 <!-- the below link must be an absolute URL to be functional in the PyPI README -->
 [migration]: https://github.com/caleb531/automata/blob/main/MIGRATION.md
 
 ## Installing
 
 You can install the latest version of Automata via pip:
 
 ```sh
 pip install automata-lib
 ```
 
+To install the optional visual dependencies, use the `visual` extra:
+
+```sh
+pip install 'automata-lib[visual]'
+```
+
 ## API
 
 Please refer to [the official API Documentation][docs] in the `docs/` directory
 of the GitHub repository.
 
 <!-- the below link must be an absolute URL to be functional in the PyPI README -->
 [docs]: https://github.com/caleb531/automata/blob/main/docs/README.md
```

