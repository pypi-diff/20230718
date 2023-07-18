# Comparing `tmp/idessem-0.0.7.tar.gz` & `tmp/idessem-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idessem-0.0.7.tar", last modified: Mon Jul 10 19:16:35 2023, max compression
+gzip compressed data, was "idessem-0.0.8.tar", last modified: Tue Jul 18 21:09:10 2023, max compression
```

## Comparing `idessem-0.0.7.tar` & `idessem-0.0.8.tar`

### file list

```diff
@@ -1,107 +1,113 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.171421 idessem-0.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-10 19:14:47.000000 idessem-0.0.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-10 19:16:35.171421 idessem-0.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-10 19:14:47.000000 idessem-0.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.143421 idessem-0.0.7/examples/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.143421 idessem-0.0.7/idessem/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.151421 idessem-0.0.7/idessem/dessem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/avl_estatfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/avl_fpha1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/dessemarq.py
--rw-r--r--   0 runner    (1001) docker     (123)    67135 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/entdados.py
--rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/log_matriz.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.155421 idessem-0.0.7/idessem/dessem/modelos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.155421 idessem-0.0.7/idessem/dessem/modelos/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/arquivos/arquivocsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/avl_fpha1.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.159421 idessem-0.0.7/idessem/dessem/modelos/blocos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/blocos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/blocos/dataestudo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/blocos/tabelacsv.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/blocos/versaomodelo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)    29829 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/dessemarq.py
--rw-r--r--   0 runner    (1001) docker     (123)   142870 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/entdados.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/log_matriz.py
--rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/operut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/pdo_eco_fcfcortes.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/pdo_eco_usih_polin.py
--rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/modelos/renovaveis.py
--rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/operut.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/pdo_eco_fcfcortes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/pdo_eco_usih_polin.py
--rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/dessem/renovaveis.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/idessem/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.143421 idessem-0.0.7/idessem.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-10 19:16:35.000000 idessem-0.0.7/idessem.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3003 2023-07-10 19:16:35.000000 idessem-0.0.7/idessem.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-10 19:16:35.000000 idessem-0.0.7/idessem.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-10 19:16:35.000000 idessem-0.0.7/idessem.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-10 19:16:35.000000 idessem-0.0.7/idessem.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-10 19:16:35.171421 idessem-0.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-10 19:14:47.000000 idessem-0.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.159421 idessem-0.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.163421 idessem-0.0.7/tests/dessem/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_avl_fpha1.py
--rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_dessemarq.py
--rw-r--r--   0 runner    (1001) docker     (123)    12140 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_entdados.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_log_matriz.py
--rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_operut.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_pdo_eco_fcfcortes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_pdo_eco_usih_polin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/dessem/test_renovaveis.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.163421 idessem-0.0.7/tests/mocks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-10 19:16:35.167421 idessem-0.0.7/tests/mocks/arquivos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/avl_altqueda.py
--rw-r--r--   0 runner    (1001) docker     (123)    35283 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/avl_desvfpha.py
--rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/avl_fpha1.py
--rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/des_log_relato.py
--rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/dessemarq.py
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/entdados.py
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/log_matriz.py
--rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/operut.py
--rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/pdo_eco_fcfcortes.py
--rw-r--r--   0 runner    (1001) docker     (123)    27569 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/pdo_eco_usih.py
--rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/pdo_eco_usih_polin.py
--rw-r--r--   0 runner    (1001) docker     (123)    36491 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/pdo_hidr.py
--rw-r--r--   0 runner    (1001) docker     (123)   254946 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/pdo_oper_uct.py
--rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/pdo_sist.py
--rw-r--r--   0 runner    (1001) docker     (123)    22170 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/polinjus.py
--rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/arquivos/renovaveis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-10 19:14:47.000000 idessem-0.0.7/tests/mocks/mock_open.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.458173 idessem-0.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 21:06:13.000000 idessem-0.0.8/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-18 21:09:10.458173 idessem-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-07-18 21:06:13.000000 idessem-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.438173 idessem-0.0.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.438173 idessem-0.0.8/idessem/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.442173 idessem-0.0.8/idessem/dessem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/avl_estatfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/avl_fpha1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13741 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71544 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12203 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/log_matriz.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.446173 idessem-0.0.8/idessem/dessem/modelos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.446173 idessem-0.0.8/idessem/dessem/modelos/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/arquivos/arquivocsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4700 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/avl_fpha1.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.446173 idessem-0.0.8/idessem/dessem/modelos/blocos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/blocos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/blocos/dataestudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/blocos/tabelacsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/blocos/versaomodelo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.446173 idessem-0.0.8/idessem/dessem/modelos/componentes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/componentes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/componentes/stagedatefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29829 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)   159757 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/log_matriz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24254 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1129 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3473 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2453 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2011 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8916 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/modelos/renovaveis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11548 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2643 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2138 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13265 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/dessem/renovaveis.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/idessem/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.438173 idessem-0.0.8/idessem.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-07-18 21:09:10.000000 idessem-0.0.8/idessem.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-18 21:09:10.000000 idessem-0.0.8/idessem.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 21:09:10.000000 idessem-0.0.8/idessem.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-18 21:09:10.000000 idessem-0.0.8/idessem.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-18 21:09:10.000000 idessem-0.0.8/idessem.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 21:09:10.458173 idessem-0.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-07-18 21:06:13.000000 idessem-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.446173 idessem-0.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.454173 idessem-0.0.8/tests/dessem/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.454173 idessem-0.0.8/tests/dessem/componentes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/componentes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/componentes/test_stagedatefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_avl_fpha1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4332 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20824 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29439 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2251 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_log_matriz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19608 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4015 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3372 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2863 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9336 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5182 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/dessem/test_renovaveis.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.454173 idessem-0.0.8/tests/mocks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:09:10.458173 idessem-0.0.8/tests/mocks/arquivos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12864 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/avl_altqueda.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35283 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/avl_desvfpha.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17085 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/avl_fpha1.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3084 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/des_log_relato.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8768 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/dessemarq.py
+-rw-r--r--   0 runner    (1001) docker     (123)   348001 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/entdados.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/log_matriz.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11746 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/operut.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8660 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/pdo_eco_fcfcortes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27569 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/pdo_eco_usih.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12961 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/pdo_eco_usih_polin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36491 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/pdo_hidr.py
+-rw-r--r--   0 runner    (1001) docker     (123)   254946 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/pdo_oper_uct.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8115 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/pdo_sist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22170 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/polinjus.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15204 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/arquivos/renovaveis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-07-18 21:06:13.000000 idessem-0.0.8/tests/mocks/mock_open.py
```

### Comparing `idessem-0.0.7/LICENSE.md` & `idessem-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/PKG-INFO` & `idessem-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idessem
-Version: 0.0.7
+Version: 0.0.8
 Summary: Interface para arquivos do DESSEM
 Home-page: https://github.com/rjmalves/idessem
 Author: Rogerio Alves, Mariana Noel
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `idessem-0.0.7/README.md` & `idessem-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/avl_altqueda.py` & `idessem-0.0.8/idessem/dessem/avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/avl_desvfpha.py` & `idessem-0.0.8/idessem/dessem/avl_desvfpha.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/avl_fpha1.py` & `idessem-0.0.8/idessem/dessem/avl_fpha1.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/des_log_relato.py` & `idessem-0.0.8/idessem/dessem/des_log_relato.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/dessemarq.py` & `idessem-0.0.8/idessem/dessem/dessemarq.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/entdados.py` & `idessem-0.0.8/idessem/dessem/entdados.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,36 @@
-from idessem.dessem.modelos.entdados import UH, SIST, REE, TM, RIVAR, RD
+from idessem.dessem.modelos.entdados import (
+    UH,
+    SIST,
+    REE,
+    TM,
+    RIVAR,
+    RD,
+    TVIAG,
+    UT,
+    USIE,
+    DP,
+    DE,
+    CD,
+    PQ,
+    IT,
+    RI,
+    IA,
+    GP,
+    ACVTFUGA,
+    ACVOLMAX,
+    ACVOLMIN,
+    ACVSVERT,
+    ACVMDESV,
+    ACCOTVAZ,
+)
 import pandas as pd  # type: ignore
 from cfinterface.files.registerfile import RegisterFile
 from cfinterface.components.register import Register
-from typing import Type, List, Optional, TypeVar, Union
+from typing import Type, List, Optional, TypeVar, Union, Any
 
 # Para compatibilidade - até versão 1.0.0
 from os.path import join
 import warnings
 
 
 class Entdados(RegisterFile):
@@ -21,15 +45,40 @@
     método `le_arquivo()` e escreve um novo arquivo a partir do método
     `escreve_arquivo()`.
 
     """
 
     T = TypeVar("T")
 
-    REGISTERS = [UH]
+    AC = Union[ACVTFUGA, ACVOLMAX, ACVOLMIN, ACVSVERT, ACVMDESV, ACCOTVAZ]
+
+    REGISTERS = [
+        UH,
+        SIST,
+        REE,
+        TM,
+        RIVAR,
+        RD,
+        TVIAG,
+        UT,
+        USIE,
+        DP,
+        DE,
+        CD,
+        IT,
+        RI,
+        IA,
+        GP,
+        ACVTFUGA,
+        ACVOLMAX,
+        ACVOLMIN,
+        ACVSVERT,
+        ACVMDESV,
+        ACCOTVAZ,
+    ]
 
     def __init__(self, data=...) -> None:
         super().__init__(data)
 
     @classmethod
     def le_arquivo(
         cls, diretorio: str, nome_arquivo="entdados.dat"
@@ -132,46 +181,23 @@
 
         Este método existe para retrocompatibilidade e deve ser substituído
         quando for suportado na classe :class:`RegisterFile`.
         """
         self.data.preppend(registro)
 
     @property
-    def rd(
-        self,
-        df: bool = False,
-    ) -> Optional[Union[RD, List[RD], pd.DataFrame]]:
+    def rd(self) -> Optional[RD]:
         """
-        Obtém um registro que define as opções de representação da
+        Obtém o (único) registro que define as opções de representação da
         rede elétrica no estudo descrito pelo :class:`Entdados`.
 
-        :param variaveis_de_folga: inclusão de variáveis de folga
-        :type variaveis_de_folga: int | None
-        :param maximo_circuitos_violados: número máximo de circuitos violados
-        :type maximo_circuitos_violados: int | None
-        :param carga_registro_dbar: consideração cargas do bloco DBAR
-        :type carga_registro_dbar: int | None
-        :param limites_circuitos_transformadores_elevadores: consideração de limites
-        em transformadores elevadores
-        :type limites_circuitos_transformadores_elevadores: int | None
-        :param limites_circuitos_e_drefs: consideração de limites de fluxo
-        :type limites_circuitos_e_drefs: int | None
-        :param consideracao_perdas: consideração de perdas
-        :type consideracao_perdas: int | None
-        :param formato_arquivos_rede: formato dos arquivos de rede elétrica
-        :type formato_arquivos_rede: int | None
-        :return: Um ou mais registros, se existirem.
-        :rtype: :class:`RIVAR` | list[:class:`RIVAR`] | :class:`pd.DataFrame` | None
+        :return: Um registro, se existir.
+        :rtype: :class:`RD` | None
         """
-        if df:
-            return self._as_df(RD)
-        else:
-            return self.__obtem_registros_com_filtros(
-                RD,
-            )
+        return self.__obtem_registro(RD)
 
     def rivar(
         self,
         codigo_entidade: Optional[int] = None,
         tipo_variavel: Optional[int] = None,
         df: bool = False,
     ) -> Optional[Union[RIVAR, List[RIVAR], pd.DataFrame]]:
@@ -235,16 +261,14 @@
                 hora_inicial=hora_inicial,
                 meia_hora_inicial=meia_hora_inicial,
             )
 
     def sist(
         self,
         codigo: Optional[int] = None,
-        mnemonico: Optional[str] = None,
-        ficticio: Optional[int] = None,
         nome: Optional[str] = None,
         df: bool = False,
     ) -> Optional[Union[SIST, List[SIST], pd.DataFrame]]:
         """
         Obtém um registro que define os submercados existentes
         no estudo descrito pelo :class:`Entdados`.
 
@@ -286,15 +310,15 @@
         :return: Um ou mais registros, se existirem.
         :rtype: :class:`REE` | list[:class:`REE`] | :class:`pd.DataFrame` | None
         """
         if df:
             return self._as_df(REE)
         else:
             return self.__obtem_registros_com_filtros(
-                REE, codigo=codigo, nome=nome
+                REE, codigo=codigo, submercado=submercado, nome=nome
             )
 
     def uh(
         self,
         codigo: Optional[int] = None,
         nome: Optional[str] = None,
         ree: Optional[int] = None,
@@ -331,212 +355,383 @@
                 codigo=codigo,
                 nome=nome,
                 ree=ree,
                 volume_inicial=volume_inicial,
                 evaporacao=evaporacao,
             )
 
-    # def ct(
-    #     self,
-    #     codigo: Optional[int] = None,
-    #     estagio: Optional[int] = None,
-    #     subsistema: Optional[int] = None,
-    #     nome: Optional[str] = None,
-    #     df: bool = False,
-    # ) -> Optional[Union[CT, List[CT], pd.DataFrame]]:
-    #     """
-    #     Obtém um registro que define uma usina termelétrica existente
-    #     no estudo descrito pelo :class:`Dadger`.
+    def tviag(
+        self,
+        uhe_montante: Optional[int] = None,
+        elemento_jusante: Optional[int] = None,
+        tipo_elemento_jusante: Optional[str] = None,
+        duracao: Optional[int] = None,
+        tipo_tempo_viagem: Optional[int] = None,
+        df: bool = False,
+    ) -> Optional[Union[TVIAG, List[TVIAG], pd.DataFrame]]:
+        """
+        Obtém um registro que especifica os tempos de viagem da
+        água entre uma UHE existente e um elemento a jusante
+        no estudo descrito pelo :class:`Entdados`.
 
-    #     :param codigo: código que especifica o registro da UTE
-    #     :type codigo: int | None
-    #     :param estagio: estágio associado ao registro
-    #     :type estagio: int | None
-    #     :param subsistema: subsistema da UTE
-    #     :type subsistema: str | None
-    #     :param df: ignorar os filtros e retornar
-    #         todos os dados de registros como um DataFrame
-    #     :type df: bool
+        :param uhe_montante: Índice da UHE a montante com tempo de viagem
+        :type uhe_montante: int | None
+        :param elemento_jusante: Índice do elemento a jusante
+        :type elemento_jusante: int | None
+        :param tipo_elemento_jusante: Tipo do elemento a jusante (seção ou UHE)
+        :type tipo_elemento_jusante: str | None
+        :param duracao: duração, em horas, da viagem da água
+        :type duracao: int | None
+        :param tipo_tempo_viagem: ìndice do tipo do tempo de viagem (translação ou propagação)
+        :type tipo_tempo_viagem: int | None
+        :param df: ignorar os filtros e retornar
+            todos os dados de registros como um DataFrame
+        :type df: bool
 
-    #     :return: Um ou mais registros, se existirem.
-    #     :rtype: :class:`CT` | list[:class:`CT`] | :class:`pd.DataFrame` | None
-    #     """
-    #     if df:
-    #         return self._as_df(CT)
-    #     else:
-    #         return self.__obtem_registros_com_filtros(
-    #             CT,
-    #             codigo=codigo,
-    #             estagio=estagio,
-    #             subsistema=subsistema,
-    #             nome=nome,
-    #         )
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`TVIAG` | list[:class:`TVIAG`] | :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(TVIAG)
+        else:
+            return self.__obtem_registros_com_filtros(
+                TVIAG,
+                uhe_montante=uhe_montante,
+                elemento_jusante=elemento_jusante,
+                tipo_elemento_jusante=tipo_elemento_jusante,
+                duracao=duracao,
+                tipo_tempo_viagem=tipo_tempo_viagem,
+            )
 
-    # def dp(
-    #     self,
-    #     estagio: Optional[int] = None,
-    #     subsistema: Optional[int] = None,
-    #     num_patamares: Optional[int] = None,
-    #     df: bool = False,
-    # ) -> Optional[Union[DP, List[DP], pd.DataFrame]]:
-    #     """
-    #     Obtém um registro que define as durações dos patamares
-    #     no estudo descrito pelo :class:`Dadger`.
+    def ut(
+        self,
+        codigo: Optional[int] = None,
+        nome: Optional[str] = None,
+        submercado: Optional[int] = None,
+        tipo_restricao: Optional[int] = None,
+        geracao_minima: Optional[float] = None,
+        geracao_maxima: Optional[float] = None,
+        df: bool = False,
+    ) -> Optional[Union[UT, List[UT], pd.DataFrame]]:
+        """
+        Obtém um registro que define uma usina termelétrica existente
+        no estudo descrito pelo :class:`Entdados`.
 
-    #     :param estagio: estágio sobre o qual serão
-    #         definidas as durações dos patamares
-    #     :type estagio: int | None
-    #     :param subsistema: subsistema para o qual
-    #         valerão os patamares.
-    #     :type subsistema: int | None
-    #     :param num_patamares: número de patamares
-    #     :type num_patamares: int | None
-    #     :param df: ignorar os filtros e retornar
-    #         todos os dados de registros como um DataFrame
-    #     :type df: bool
+        :param codigo: índice do código que especifica o registro da UTE
+        :type codigo: int | None
+        :param nome: nome da UTE
+        :type nome: str | None
+        :param submercado: índice do submercado da UTE
+        :type submercado: int | None
+        :param tipo_restricao: tipo de restrição
+        :type tipo_restricao: int | None
+        :param geracao_minima: limite de geração mínima (ou, caso restrição de rampa,
+            valor da variação máxima para decréscimo de geração)
+        :type geracao_minima: float | None
+        :param geracao_maxima: limite de geração máxima (ou, caso restrição de rampa,
+            valor da variação máxima para acréscimo de geração)
+        :type geracao_maxima: float | None
+        :param df: ignorar os filtros e retornar
+            todos os dados de registros como um DataFrame
+        :type df: bool
 
-    #     :return: Um ou mais registros, se existirem.
-    #     :rtype: :class:`DP` | list[:class:`DP`] |
-    #         :class:`pd.DataFrame` | None
-    #     """
-    #     if df:
-    #         return self._as_df(DP)
-    #     else:
-    #         return self.__obtem_registros_com_filtros(
-    #             DP,
-    #             estagio=estagio,
-    #             subsistema=subsistema,
-    #             num_patamares=num_patamares,
-    #         )
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`UT` | list[:class:`UT`] | :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(UT)
+        else:
+            return self.__obtem_registros_com_filtros(
+                UT,
+                codigo=codigo,
+                nome=nome,
+                submercado=submercado,
+                tipo_restricao=tipo_restricao,
+                geracao_minima=geracao_minima,
+                geracao_maxima=geracao_maxima,
+            )
 
-    # def pq(
-    #     self,
-    #     nome: Optional[str] = None,
-    #     subsistema: Optional[int] = None,
-    #     estagio: Optional[int] = None,
-    #     df: bool = False,
-    # ) -> Optional[Union[PQ, List[PQ], pd.DataFrame]]:
-    #     """
-    #     Obtém um registro que define as gerações das pequenas usinas
-    #     no estudo descrito pelo :class:`Dadger`.
+    def usie(
+        self,
+        codigo: Optional[int] = None,
+        submercado: Optional[int] = None,
+        nome: Optional[str] = None,
+        uhe_montante: Optional[int] = None,
+        uhe_jusante: Optional[int] = None,
+        df: bool = False,
+    ) -> Optional[Union[USIE, List[USIE], pd.DataFrame]]:
+        """
+        Obtém um registro que define as usinas elevatórias da configuração
+        e seus principais dados físicos no estudo descrito pelo :class:`Entdados`.
 
-    #     :param nome: o nome das gerações
-    #     :param subsistema: subsistema para o qual
-    #         valerão as gerações
-    #     :param estagio: estágio sobre o qual serão
-    #         definidas as gerações
-    #     :type estagio: int | None
-    #     :type subsistema: int | None
-    #     :param df: ignorar os filtros e retornar
-    #         todos os dados de registros como um DataFrame
-    #     :type df: bool
+        :param codigo: código que especifica a usina elevatória
+        :type codigo: int | None
+        :param submercado: código do submercado correspondente
+        :type submercado: str | None
+        :param nome: nome da usina elevatória
+        :type nome: int | None
+        :param uhe_montante: código da usina a montante
+        :type uhe_montante: int | None
+        :param uhe_jusante: código da usina a jusante
+        :type uhe_jusante: int | None
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`USIE` | list[:class:`USIE`] | :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(USIE)
+        else:
+            return self.__obtem_registros_com_filtros(
+                USIE,
+                codigo=codigo,
+                submercado=submercado,
+                nome=nome,
+                uhe_montante=uhe_montante,
+                uhe_jusante=uhe_jusante,
+            )
 
-    #     :return: Um ou mais registros, se existirem.
-    #     :rtype: :class:`PQ` | list[:class:`PQ`] | :class:`pd.DataFrame` | None
-    #     """
-    #     if df:
-    #         return self._as_df(PQ)
-    #     else:
-    #         return self.__obtem_registros_com_filtros(
-    #             PQ,
-    #             nome=nome,
-    #             estagio=estagio,
-    #             subsistema=subsistema,
-    #         )
+    def dp(
+        self,
+        submercado: Optional[int] = None,
+        df: bool = False,
+    ) -> Optional[Union[DP, List[DP], pd.DataFrame]]:
+        """
+        Obtém um registro que define os dados de demanda para
+        os submercados que serão consideradas para os períodos
+        que não se considerada a rede elétrica no estudo descrito
+        pelo :class:`Entdados`.
+
+        :param submercado: subsistema para o qual
+            valerão os patamares.
+        :type submercado: int | None
+        :param df: ignorar os filtros e retornar
+            todos os dados de registros como um DataFrame
+        :type df: bool
 
-    # def ac(
-    #     self,
-    #     uhe: int,
-    #     modificacao: Any,
-    #     df: bool = False,
-    #     **kwargs,
-    # ) -> Optional[Union[AC, List[AC], pd.DataFrame]]:
-    #     """
-    #     Obtém um registro que define modificações nos parâmetros
-    #     das UHE em um :class:`Dadger`.
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`DP` | list[:class:`DP`] |
+            :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(DP)
+        else:
+            return self.__obtem_registros_com_filtros(
+                DP,
+                submercado=submercado,
+            )
 
-    #     :param uhe: código da UHE modificada
-    #     :type uhe: int
-    #     :param modificacao: classe da modificação realizada
-    #     :type modificacao: subtipos do tipo `AC`
-    #     :param df: ignorar os filtros e retornar
-    #         todos os dados de registros como um DataFrame
-    #     :type df: bool
+    def de(
+        self,
+        codigo: Optional[int] = None,
+        df: bool = False,
+    ) -> Optional[Union[DE, List[DE], pd.DataFrame]]:
+        """
+        Obtém um registro que define uma demanda especial para
+        serem representadas em restrições elétricas no estudo descrito
+        pelo :class:`Entdados`.
 
-    #     :return: Um ou mais registros, se existirem.
-    #     :rtype: `AC` | list[`AC`] | :class:`pd.DataFrame` | None
-    #     """
-    #     if df:
-    #         return self._as_df(modificacao)
-    #     else:
-    #         return self.__obtem_registros_com_filtros(
-    #             modificacao, **{"uhe": uhe, **kwargs}
-    #         )
+        :param codigo: código da demanda especial.
+        :type codigo: int | None
+        :param df: ignorar os filtros e retornar
+            todos os dados de registros como um DataFrame
+        :type df: bool
 
-    # def cd(
-    #     self,
-    #     numero_curva: Optional[int] = None,
-    #     subsistema: Optional[int] = None,
-    #     nome_curva: Optional[str] = None,
-    #     estagio: Optional[int] = None,
-    #     df: bool = False,
-    # ) -> Optional[Union[CD, List[CD], pd.DataFrame]]:
-    #     """
-    #     Obtém um registro que define as curvas de déficit
-    #     no estudo descrito pelo :class:`Dadger`.
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`DE` | list[:class:`DE`] |
+            :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(DE)
+        else:
+            return self.__obtem_registros_com_filtros(
+                DE,
+                codigo=codigo,
+            )
 
-    #     :param numero_curva: Índice da curva de déficit descrita
-    #     :type numero_curva: int | None
-    #     :param subsistema: subsistema para o qual valerá a curva.
-    #     :type subsistema: int | None
-    #     :param nome_curva: nome da curva.
-    #     :type nome_curva: str | None
-    #     :param estagio: estagio para o qual valerá a curva.
-    #     :type estagio: int | None
-    #     :param df: ignorar os filtros e retornar
-    #         todos os dados de registros como um DataFrame
-    #     :type df: bool
+    def cd(
+        self,
+        submercado: Optional[int] = None,
+        numero_curva: Optional[int] = None,
+        df: bool = False,
+    ) -> Optional[Union[CD, List[CD], pd.DataFrame]]:
+        """
+        Obtém um registro que define as curvas de déficit
+        no estudo descrito pelo :class:`Entdados`.
 
-    #     :return: Um ou mais registros, se existirem.
-    #     :rtype: :class:`LU` | list[:class:`LU`] | :class:`pd.DataFrame` | None
-    #     """
-    #     if df:
-    #         return self._as_df(CD)
-    #     else:
-    #         return self.__obtem_registros_com_filtros(
-    #             CD,
-    #             numero_curva=numero_curva,
-    #             subsistema=subsistema,
-    #             nome_curva=nome_curva,
-    #             estagio=estagio,
-    #         )
+        :param submercado: submercado para o qual valerá a curva
+        :type submercado: int | None
+        :param numero_curva: índice da curva de déficit descrita
+        :type numero_curva: int | None
+        :param df: ignorar os filtros e retornar
+            todos os dados de registros como um DataFrame
+        :type df: bool
+
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`CD` | list[:class:`CD`] | :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(CD)
+        else:
+            return self.__obtem_registros_com_filtros(
+                CD,
+                submercado=submercado,
+                numero_curva=numero_curva,
+            )
+
+    def pq(
+        self,
+        codigo: Optional[int] = None,
+        nome: Optional[str] = None,
+        localizacao: Optional[int] = None,
+        df: bool = False,
+    ) -> Optional[Union[PQ, List[PQ], pd.DataFrame]]:
+        """
+        Obtém um registro que define as gerações das pequenas usinas
+        no estudo descrito pelo :class:`Entdados`.
+
+        :param codigo: o código das gerações
+        :type codigo: str | None
+        :param nome: o nome das gerações
+        :type nome: str | None
+        :param localizacao: índice do subsistema ou barra
+            associado à geração
+        :type localizacao: int | None
+        :param df: ignorar os filtros e retornar
+            todos os dados de registros como um DataFrame
+        :type df: bool
+
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`PQ` | list[:class:`PQ`] | :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(PQ)
+        else:
+            return self.__obtem_registros_com_filtros(
+                PQ,
+                codigo=codigo,
+                nome=nome,
+                localizacao=localizacao,
+            )
+
+    @property
+    def it(self) -> Optional[IT]:
+        """
+        Obtém o (único) registro que contém os coeficientes
+        do polinômio do canal de fuga de Itaipu em função
+        da vazão na Régua 11, para casos sem FPHA Libs
+        no estudo definido no :class:`Entdados`
+
+        :return: Um registro, se existir.
+        :rtype: :class:`IT` | None.
+        """
+        return self.__obtem_registro(IT)
+
+    def ri(
+        self,
+        df: bool = False,
+    ) -> Optional[Union[RI, List[RI], pd.DataFrame]]:
+        """
+        Obtém um registro que define restrições de Itaipu
+        no estudo descrito pelo :class:`Entdados`.
+
+        :param df: ignorar os filtros e retornar
+            todos os dados de registros como um DataFrame
+        :type df: bool
+
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`RI` | list[:class:`RI`] | :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(RI)
+        else:
+            return self.__obtem_registros_com_filtros(
+                RI,
+            )
+
+    def ia(
+        self,
+        submercado_de: Optional[str] = None,
+        submercado_para: Optional[str] = None,
+        df: bool = False,
+    ) -> Optional[Union[IA, List[IA], pd.DataFrame]]:
+        """
+        Obtém um registro que define as capacidades de intercâmbio
+        no estudo descrito pelo :class:`Entdados`.
+
+        :param submercado_de: mnemônico do submercado de origem (de).
+        :type submercado_de: str | None
+        :param submercado_para: mnemônico do submercado de destino (para).
+        :type submercado_para: str | None
+        :param df: ignorar os filtros e retornar
+            todos os dados de registros como um DataFrame
+        :type df: bool
+
+        :return: Um ou mais registros, se existirem.
+        :rtype: :class:`IA` | list[:class:`IA`] | :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(IA)
+        else:
+            return self.__obtem_registros_com_filtros(
+                IA,
+                submercado_de=submercado_de,
+                submercado_para=submercado_para,
+            )
+
+    @property
+    def gp(self) -> Optional[GP]:
+        """
+        Obtém o (único) registro que define o gap de convergência
+        no estudo definido no :class:`Entdados`
+
+        :return: Um registro, se existir.
+        :rtype: :class:`GP` | None.
+        """
+        return self.__obtem_registro(GP)
+
+    def ac(
+        self,
+        uhe: int,
+        modificacao: Any,
+        df: bool = False,
+        **kwargs,
+    ) -> Optional[Union[AC, List[AC], pd.DataFrame]]:
+        """
+        Obtém um registro que define modificações nos parâmetros
+        das UHE em um :class:`Entdados`.
+
+        :param uhe: código da UHE modificada
+        :type uhe: int
+        :param modificacao: classe da modificação realizada
+        :type modificacao: subtipos do tipo `AC`
+        :param df: ignorar os filtros e retornar
+            todos os dados de registros como um DataFrame
+        :type df: bool
+
+        :return: Um ou mais registros, se existirem.
+        :rtype: `AC` | list[`AC`] | :class:`pd.DataFrame` | None
+        """
+        if df:
+            return self._as_df(modificacao)
+        else:
+            return self.__obtem_registros_com_filtros(
+                modificacao, **{"uhe": uhe, **kwargs}
+            )
 
     # @property
     # def tx(self) -> Optional[TX]:
     #     """
     #     Obtém o (único) registro que define a taxa de desconto
     #     aplicada no estudo definido no :class:`Dadger`
 
     #     :return: Um registro, se existir.
     #     :rtype: :class:`TX` | None.
     #     """
     #     return self.__obtem_registro(TX)
 
     # @property
-    # def gp(self) -> Optional[GP]:
-    #     """
-    #     Obtém o (único) registro que define o gap para convergência
-    #     considerado no estudo definido no :class:`Dadger`
-
-    #     :return: Um registro, se existir.
-    #     :rtype: :class:`GP` | None.
-    #     """
-    #     return self.__obtem_registro(GP)
-
-    # @property
     # def ni(self) -> Optional[NI]:
     #     """
     #     Obtém o (único) registro que define o número máximo de iterações
     #     do DECOMP no estudo definido no :class:`Dadger`
 
     #     :return: Um registro, se existir.
     #     :rtype: :class:`NI` | None.
@@ -803,43 +998,14 @@
     #             restricao=restricao,
     #             estagio=estagio,
     #             de=de,
     #             para=para,
     #             coeficiente=coeficiente,
     #         )
 
-    # def vi(
-    #     self,
-    #     uhe: Optional[int] = None,
-    #     duracao: Optional[int] = None,
-    #     df: bool = False,
-    # ) -> Optional[Union[VI, List[VI], pd.DataFrame]]:
-    #     """
-    #     Obtém um registro que especifica os tempos de viagem da
-    #     água em uma UHE existente no no estudo descrito
-    #     pelo :class:`Dadger`.
-
-    #     :param uhe: Índice da UHE associada aos tempos de viagem
-    #     :type uhe: int | None
-    #     :param duracao: duração, em horas, da viagem da água
-    #     :type duracao: int | None
-    #     :param df: ignorar os filtros e retornar
-    #         todos os dados de registros como um DataFrame
-    #     :type df: bool
-
-    #     :return: Um ou mais registros, se existirem.
-    #     :rtype: :class:`VI` | list[:class:`VI`] | :class:`pd.DataFrame` | None
-    #     """
-    #     if df:
-    #         return self._as_df(VI)
-    #     else:
-    #         return self.__obtem_registros_com_filtros(
-    #             VI, uhe=uhe, duracao=duracao
-    #         )
-
     # def ir(
     #     self, tipo: Optional[str] = None, df: bool = False
     # ) -> Optional[Union[IR, List[IR], pd.DataFrame]]:
     #     """
     #     Obtém um registro que especifica os relatórios de saída
     #     a serem produzidos pelo DECOMP após a execução do estudo
     #     descrito no :class:`Dadger`.
```

### Comparing `idessem-0.0.7/idessem/dessem/hidr.py` & `idessem-0.0.8/idessem/dessem/hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/log_matriz.py` & `idessem-0.0.8/idessem/dessem/log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/arquivos/arquivocsv.py` & `idessem-0.0.8/idessem/dessem/modelos/arquivos/arquivocsv.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/avl_altqueda.py` & `idessem-0.0.8/idessem/dessem/modelos/avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/avl_desvfpha.py` & `idessem-0.0.8/idessem/dessem/modelos/avl_desvfpha.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/avl_fpha1.py` & `idessem-0.0.8/idessem/dessem/modelos/avl_fpha1.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/blocos/dataestudo.py` & `idessem-0.0.8/idessem/dessem/modelos/blocos/dataestudo.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/blocos/tabelacsv.py` & `idessem-0.0.8/idessem/dessem/modelos/blocos/tabelacsv.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/blocos/versaomodelo.py` & `idessem-0.0.8/idessem/dessem/modelos/blocos/versaomodelo.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/des_log_relato.py` & `idessem-0.0.8/idessem/dessem/modelos/des_log_relato.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/dessemarq.py` & `idessem-0.0.8/idessem/dessem/modelos/dessemarq.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/entdados.py` & `idessem-0.0.8/idessem/dessem/modelos/entdados.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from cfinterface.components.register import Register
 from cfinterface.components.line import Line
 from cfinterface.components.integerfield import IntegerField
 from cfinterface.components.literalfield import LiteralField
 from cfinterface.components.floatfield import FloatField
-from typing import Optional, Union
+from idessem.dessem.modelos.componentes.stagedatefield import StageDateField
+from typing import Optional, Union, IO
 
 
 class RD(Register):
     """
     Registro que contém opções de representação da rede elétrica.
     """
 
@@ -455,17 +456,15 @@
     LINE = Line(
         [
             IntegerField(3, 4),
             LiteralField(12, 9),
             IntegerField(2, 24),
             FloatField(10, 29, 2),
             IntegerField(1, 39),
-            LiteralField(2, 41),
-            IntegerField(2, 44),
-            IntegerField(1, 47),
+            StageDateField(starting_position=41, special_day_character="I"),
             FloatField(10, 49, 2),
             IntegerField(1, 64),
             IntegerField(1, 69),
         ]
     )
 
     @property
@@ -537,761 +536,1910 @@
     @evaporacao.setter
     def evaporacao(self, e: int):
         self.data[4] = e
 
     @property
     def dia_inicial(self) -> Optional[Union[str, int]]:
         """
-        O dia inicial de operação.
+        O dia inicial.
 
         :return: O dia.
         :rtype: str | int | None
         """
 
-        dia = self.data[5]
-        if (dia == "I") or (dia is None):
-            return dia
-        else:
-            return int(dia)
+        return self.data[5][0]
 
     @dia_inicial.setter
     def dia_inicial(self, n: Union[str, int]):
-        if isinstance(n, int):
-            self.data[5] = str(n)
-        else:
-            self.data[5] = n
+        self.data[5][0] = n
 
     @property
     def hora_inicial(self) -> Optional[int]:
         """
-        A hora inicial de operação.
+        A hora inicial.
 
         :return: A hora.
         :rtype: int | None
         """
-        return self.data[6]
+        return self.data[5][1]
 
     @hora_inicial.setter
     def hora_inicial(self, n: int):
-        self.data[6] = n
+        self.data[5][1] = n
 
     @property
     def meia_hora_inicial(self) -> Optional[int]:
         """
-        A meia-hora inicial de operação.
+        A meia-hora inicial.
 
         :return: A meia-hora.
         :rtype: int | None
         """
-        return self.data[7]
+        return self.data[5][2]
 
     @meia_hora_inicial.setter
     def meia_hora_inicial(self, n: int):
-        self.data[7] = n
+        self.data[5][2] = n
 
     @property
     def volume_morto_inicial(self) -> Optional[float]:
         """
         Volume morto inicial da usina.
 
         :return: O volume em hm3.
         :rtype: float | None
         """
-        return self.data[8]
+        return self.data[6]
 
     @volume_morto_inicial.setter
     def volume_morto_inicial(self, e: float):
-        self.data[8] = e
+        self.data[6] = e
 
     @property
     def produtividade(self) -> Optional[int]:
         """
         O tipo de produtividade considerada.
 
         :return: O flag.
         :rtype: int | None
         """
-        return self.data[9]
+        return self.data[7]
 
     @produtividade.setter
     def produtividade(self, n: int):
-        self.data[9] = n
+        self.data[7] = n
 
     @property
     def penaliza_restricao_geracao(self) -> Optional[int]:
         """
         O flag que indica penalização de restrições de geração.
 
         :return: O flag.
         :rtype: int | None
         """
-        return self.data[10]
+        return self.data[8]
 
     @penaliza_restricao_geracao.setter
     def penaliza_restricao_geracao(self, n: int):
-        self.data[10] = n
+        self.data[8] = n
 
 
-# class CT(Register):
-#     """
-#     Registro que contém o cadastro das usinas termelétricas com
-#     os seus custos e capacidades.
+class TVIAG(Register):
+    """
+    Registro que contém os tempos de viagem da água entre usinas.
+    """
 
-#     *OBS: Suporta apenas 3 patamares no momento*
-#     """
+    IDENTIFIER = "TVIAG "
+    IDENTIFIER_DIGITS = 6
+    LINE = Line(
+        [
+            IntegerField(3, 6),
+            IntegerField(3, 10),
+            LiteralField(1, 14),
+            IntegerField(3, 19),
+            IntegerField(1, 24),
+        ]
+    )
 
-#     IDENTIFIER = "CT  "
-#     IDENTIFIER_DIGITS = 4
-#     LINE = Line(
-#         [
-#             IntegerField(3, 4),
-#             IntegerField(2, 9),
-#             LiteralField(10, 14),
-#             IntegerField(2, 24),
-#             FloatField(5, 29, 2),
-#             FloatField(5, 34, 2),
-#             FloatField(10, 39, 2),
-#             FloatField(5, 49, 2),
-#             FloatField(5, 54, 2),
-#             FloatField(10, 59, 2),
-#             FloatField(5, 69, 2),
-#             FloatField(5, 74, 2),
-#             FloatField(10, 79, 2),
-#         ]
-#     )
+    @property
+    def uhe_montante(self) -> Optional[int]:
+        """
+        O código da UHE a montante a partir do qual é contabilizado
+        o tempo de viagem.
 
-#     def __atualiza_dados_lista(
-#         self,
-#         novos_dados: list,
-#         indice_inicial: int,
-#         espacamento: int,
-#     ):
-#         atuais = len(self.data)
-#         ultimo_indice = indice_inicial + espacamento * len(novos_dados)
-#         diferenca = (ultimo_indice - atuais) // espacamento
-#         if diferenca > 0:
-#             self.data += [None] * (ultimo_indice - atuais)
-#             diferenca -= 1
-#         novos_dados += [None] * abs(diferenca)
-#         self.data[indice_inicial::espacamento] = novos_dados
+        :return: O código
+        :rtype: int | None
+        """
+        return self.data[0]
 
-#     @property
-#     def codigo(self) -> Optional[int]:
-#         """
-#         O código de cadastro da UTE.
+    @uhe_montante.setter
+    def uhe_montante(self, u: int):
+        self.data[0] = u
 
-#         :return: O código.
-#         :rtype: int | None
-#         """
-#         return self.data[0]
+    @property
+    def elemento_jusante(self) -> Optional[int]:
+        """
+        O código do elemento a jusante do qual é contabilizado
+        o tempo de viagem.
 
-#     @codigo.setter
-#     def codigo(self, codigo: int):
-#         self.data[0] = codigo
+        :return: O código
+        :rtype: int | None
+        """
+        return self.data[1]
 
-#     @property
-#     def subsistema(self) -> Optional[int]:
-#         """
-#         O subsistema de cadastro da UTE.
+    @elemento_jusante.setter
+    def elemento_jusante(self, u: int):
+        self.data[1] = u
 
-#         :return: O subsistema.
-#         :rtype: int | None
-#         """
-#         return self.data[1]
+    @property
+    def tipo_elemento_jusante(self) -> Optional[str]:
+        """
+        O tipo de elemento de jusante (S=seção de rio, H=usina).
 
-#     @subsistema.setter
-#     def subsistema(self, subsistema: int):
-#         self.data[1] = subsistema
+        :return: O código
+        :rtype: str | None
+        """
+        return self.data[2]
 
-#     @property
-#     def nome(self) -> Optional[str]:
-#         """
-#         O nome de cadastro da UTE.
+    @tipo_elemento_jusante.setter
+    def tipo_elemento_jusante(self, u: str):
+        self.data[2] = u
 
-#         :return: O nome como uma `str`.
-#         :rtype: str | None
-#         """
-#         return self.data[2]
+    @property
+    def duracao(self) -> Optional[int]:
+        """
+        A duração da viagem da água (em horas) entre a UHE a montante e
+        o elemento à jusante.
 
-#     @nome.setter
-#     def nome(self, nome: str):
-#         self.data[2] = nome
+        :return: A duração
+        :rtype: int | None
+        """
+        return self.data[3]
 
-#     @property
-#     def estagio(self) -> Optional[str]:
-#         """
-#         O estágio associado às propriedades cadastradas.
+    @duracao.setter
+    def duracao(self, d: int):
+        self.data[3] = d
 
-#         :return: O estágio.
-#         :rtype: int | None
-#         """
-#         return self.data[3]
+    @property
+    def tipo_tempo_viagem(self) -> Optional[int]:
+        """
+        O código referente ao tipo de tempo de viagem considerado
+        (1=translação; 2=propagação).
 
-#     @estagio.setter
-#     def estagio(self, estagio: int):
-#         self.data[3] = estagio
+        :return: O código do tipo.
+        :rtype: int | None
+        """
+        return self.data[4]
 
-#     @property
-#     def inflexibilidades(self) -> Optional[List[float]]:
-#         """
-#         As inflexibilidades da UTE por patamar.
+    @tipo_tempo_viagem.setter
+    def tipo_tempo_viagem(self, d: int):
+        self.data[4] = d
 
-#         :return: As inflexibilidades.
-#         :rtype: list[float] | None
-#         """
-#         return [v for v in self.data[4::3] if v is not None]
 
-#     @inflexibilidades.setter
-#     def inflexibilidades(self, inflex: List[float]):
-#         self.__atualiza_dados_lista(inflex, 4, 3)
+class UT(Register):
+    """
+    Registro que contém as usinas termelétricas e suas restrições
+    de geração.
 
-#     @property
-#     def disponibilidades(self) -> Optional[List[float]]:
-#         """
-#         As disponibilidades da UTE por patamar.
+    """
 
-#         :return: As disponibilidades.
-#         :rtype: list[float] | None
-#         """
-#         return [v for v in self.data[5::3] if v is not None]
+    IDENTIFIER = "UT  "
+    IDENTIFIER_DIGITS = 4
+    LINE = Line(
+        [
+            IntegerField(3, 4),
+            LiteralField(12, 9),
+            IntegerField(2, 22),
+            IntegerField(1, 25),
+            StageDateField(starting_position=27, special_day_character="I"),
+            StageDateField(starting_position=35, special_day_character="F"),
+            IntegerField(1, 46),
+            FloatField(10, 47, 3),
+            FloatField(10, 57, 3),
+        ]
+    )
 
-#     @disponibilidades.setter
-#     def disponibilidades(self, disp: List[float]):
-#         self.__atualiza_dados_lista(disp, 5, 3)
+    @property
+    def codigo(self) -> Optional[int]:
+        """
+        O código de cadastro da UTE.
 
-#     @property
-#     def cvus(self) -> Optional[List[float]]:
-#         """
-#         Os CVUs da UTE por patamar.
+        :return: O código.
+        :rtype: int | None
+        """
+        return self.data[0]
 
-#         :return: Os CVUs.
-#         :rtype: list[float] | None
-#         """
-#         return [v for v in self.data[6::3] if v is not None]
+    @codigo.setter
+    def codigo(self, codigo: int):
+        self.data[0] = codigo
 
-#     @cvus.setter
-#     def cvus(self, cvu: List[float]):
-#         self.__atualiza_dados_lista(cvu, 6, 3)
+    @property
+    def nome(self) -> Optional[str]:
+        """
+        O nome de cadastro da UTE.
 
+        :return: O nome como uma `str`.
+        :rtype: str | None
+        """
+        return self.data[1]
 
-# class UE(Register):
-#     """
-#     Registro que contém o cadastro das estações de bombeamento
-#     (usinas elevatórias).
-#     """
+    @nome.setter
+    def nome(self, nome: str):
+        self.data[1] = nome
 
-#     IDENTIFIER = "UE  "
-#     IDENTIFIER_DIGITS = 4
-#     LINE = Line(
-#         [
-#             IntegerField(3, 4),
-#             IntegerField(2, 9),
-#             LiteralField(12, 14),
-#             IntegerField(3, 29),
-#             IntegerField(3, 34),
-#             FloatField(10, 39, 1),
-#             FloatField(10, 49, 1),
-#             FloatField(10, 59, 2),
-#         ]
-#     )
+    @property
+    def submercado(self) -> Optional[int]:
+        """
+        O submercado de cadastro da UTE.
 
-#     @property
-#     def codigo(self) -> Optional[int]:
-#         """
-#         O código de cadastro da UE.
+        :return: O submercado.
+        :rtype: int | None
+        """
+        return self.data[2]
 
-#         :return: O código.
-#         :rtype: int | None
-#         """
-#         return self.data[0]
+    @submercado.setter
+    def submercado(self, submercado: int):
+        self.data[2] = submercado
 
-#     @codigo.setter
-#     def codigo(self, cod: int):
-#         self.data[0] = cod
+    @property
+    def tipo_restricao(self) -> Optional[int]:
+        """
+        O flag para indicar tipo de restrição.
 
-#     @property
-#     def subsistema(self) -> Optional[int]:
-#         """
-#         O subsistema de cadastro da UE, conforme registro SB.
+        :return: O flag.
+        :rtype: int | None
+        """
+        return self.data[3]
 
-#         :return: O subsistema.
-#         :rtype: int | None
-#         """
-#         return self.data[1]
+    @tipo_restricao.setter
+    def tipo_restricao(self, tipo_restricao: int):
+        self.data[3] = tipo_restricao
 
-#     @subsistema.setter
-#     def subsistema(self, n: int):
-#         self.data[1] = n
+    @property
+    def dia_inicial(self) -> Optional[Union[str, int]]:
+        """
+        O dia inicial.
 
-#     @property
-#     def nome(self) -> Optional[str]:
-#         """
-#         O nome da estação de bombeamento.
+        :return: O dia.
+        :rtype: str | int | None
+        """
 
-#         :return: O nome.
-#         :rtype: str | None
-#         """
-#         return self.data[2]
+        return self.data[4][0]
 
-#     @nome.setter
-#     def nome(self, v: str):
-#         self.data[2] = v
+    @dia_inicial.setter
+    def dia_inicial(self, n: Union[str, int]):
+        self.data[4][0] = n
 
-#     @property
-#     def uhe_montante(self) -> Optional[int]:
-#         """
-#         O código da UHE a montante, conforme registro UH.
+    @property
+    def hora_inicial(self) -> Optional[int]:
+        """
+        A hora inicial.
 
-#         :return: O código.
-#         :rtype: int | None
-#         """
-#         return self.data[3]
+        :return: A hora.
+        :rtype: int | None
+        """
+        return self.data[4][1]
 
-#     @uhe_montante.setter
-#     def uhe_montante(self, v: int):
-#         self.data[3] = v
+    @hora_inicial.setter
+    def hora_inicial(self, n: int):
+        self.data[4][1] = n
 
-#     @property
-#     def uhe_jusante(self) -> Optional[int]:
-#         """
-#         O código da UHE a jusante, conforme registro UH.
+    @property
+    def meia_hora_inicial(self) -> Optional[int]:
+        """
+        A meia-hora inicial.
 
-#         :return: O código.
-#         :rtype: int | None
-#         """
-#         return self.data[4]
+        :return: A meia-hora.
+        :rtype: int | None
+        """
+        return self.data[4][2]
 
-#     @uhe_jusante.setter
-#     def uhe_jusante(self, e: int):
-#         self.data[4] = e
+    @meia_hora_inicial.setter
+    def meia_hora_inicial(self, n: int):
+        self.data[4][2] = n
 
-#     @property
-#     def vazao_minima_bombeavel(self) -> Optional[float]:
-#         """
-#         A vazão mínima bombeável.
+    @property
+    def dia_final(self) -> Optional[Union[str, int]]:
+        """
+        O dia final.
 
-#         :return: A vazão em m3/s
-#         :rtype: float | None
-#         """
-#         return self.data[5]
+        :return: O dia.
+        :rtype: str | int | None
+        """
 
-#     @vazao_minima_bombeavel.setter
-#     def vazao_minima_bombeavel(self, e: float):
-#         self.data[5] = e
+        return self.data[5][0]
 
-#     @property
-#     def vazao_maxima_bombeavel(self) -> Optional[float]:
-#         """
-#         A vazão mínima bombeável.
+    @dia_final.setter
+    def dia_final(self, n: Union[str, int]):
+        self.data[5][0] = n
 
-#         :return: A vazão em m3/s
-#         :rtype: float | None
-#         """
-#         return self.data[6]
+    @property
+    def hora_final(self) -> Optional[int]:
+        """
+        A hora final.
 
-#     @vazao_maxima_bombeavel.setter
-#     def vazao_maxima_bombeavel(self, e: float):
-#         self.data[6] = e
+        :return: A hora.
+        :rtype: int | None
+        """
+        return self.data[5][1]
 
-#     @property
-#     def taxa_consumo(self) -> Optional[float]:
-#         """
-#         A taxa de consumo.
+    @hora_final.setter
+    def hora_final(self, n: int):
+        self.data[5][1] = n
 
-#         :return: A taxa em MWmed/m3/s.
-#         :rtype: float | None
-#         """
-#         return self.data[7]
+    @property
+    def meia_hora_final(self) -> Optional[int]:
+        """
+        A meia-hora final.
 
-#     @taxa_consumo.setter
-#     def taxa_consumo(self, e: float):
-#         self.data[7] = e
+        :return: A meia-hora.
+        :rtype: int | None
+        """
+        return self.data[5][2]
 
+    @meia_hora_final.setter
+    def meia_hora_final(self, n: int):
+        self.data[5][2] = n
 
-# class DP(Register):
-#     """
-#     Registro que contém o cadastro das durações dos patamares.
+    @property
+    def unidade_restricao(self) -> Optional[int]:
+        """
+        O flag para indicar a unidade da restrição de rampa.
 
-#     *OBS: Suporta apenas 3 patamares no momento*
-#     """
+        :return: O flag.
+        :rtype: int | None
+        """
+        return self.data[6]
 
-#     IDENTIFIER = "DP  "
-#     IDENTIFIER_DIGITS = 4
-#     LINE = Line(
-#         [
-#             IntegerField(2, 4),
-#             IntegerField(2, 9),
-#             IntegerField(1, 14),
-#             FloatField(10, 19, 1),
-#             FloatField(10, 29, 1),
-#             FloatField(10, 39, 1),
-#             FloatField(10, 49, 1),
-#             FloatField(10, 59, 1),
-#             FloatField(10, 69, 1),
-#         ]
-#     )
+    @unidade_restricao.setter
+    def unidade_restricao(self, unidade_restricao: int):
+        self.data[6] = unidade_restricao
 
-#     def __atualiza_dados_lista(
-#         self,
-#         novos_dados: list,
-#         indice_inicial: int,
-#         espacamento: int,
-#     ):
-#         atuais = len(self.data)
-#         ultimo_indice = indice_inicial + espacamento * len(novos_dados)
-#         diferenca = (ultimo_indice - atuais) // espacamento
-#         if diferenca > 0:
-#             self.data += [None] * (ultimo_indice - atuais)
-#             diferenca -= 1
-#         novos_dados += [None] * abs(diferenca)
-#         self.data[indice_inicial::espacamento] = novos_dados
+    @property
+    def geracao_minima(self) -> Optional[float]:
+        """
+        O valor do limite de geracao minima
+        (caso restrição de rampa, é o valor da variação
+        máxima para decréscimo de geração).
 
-#     @property
-#     def estagio(self) -> Optional[int]:
-#         """
-#         O estágio associado às durações especificadas.
+        :return: O valor.
+        :rtype: float | None
+        """
+        return self.data[7]
 
-#         :return: O estágio.
-#         :rtype: int | None
-#         """
-#         return self.data[0]
+    @geracao_minima.setter
+    def geracao_minima(self, geracao_minima: float):
+        self.data[7] = geracao_minima
 
-#     @estagio.setter
-#     def estagio(self, e: int):
-#         self.data[0] = e
+    @property
+    def geracao_maxima(self) -> Optional[float]:
+        """
+        O valor do limite de geracao máxima
+        (caso restrição de rampa, é o valor da variação
+        máxima para acréscimo de geração).
 
-#     @property
-#     def subsistema(self) -> Optional[int]:
-#         """
-#         O subsistema associado às durações especificadas.
+        :return: O valor.
+        :rtype: float | None
+        """
+        return self.data[8]
 
-#         :return: O subsistema.
-#         :rtype: int | None
-#         """
-#         return self.data[1]
+    @geracao_maxima.setter
+    def geracao_maxima(self, geracao_maxima: float):
+        self.data[8] = geracao_maxima
 
-#     @subsistema.setter
-#     def subsistema(self, sub: int):
-#         self.data[1] = sub
 
-#     @property
-#     def num_patamares(self) -> Optional[int]:
-#         """
-#         O número de patamares.
+class USIE(Register):
+    """
+    Registro que contém o cadastro das usinas elevatórias.
+    """
 
-#         :return: O número de patamares.
-#         :rtype: int | None
-#         """
-#         return self.data[2]
+    IDENTIFIER = "USIE "
+    IDENTIFIER_DIGITS = 5
+    LINE = Line(
+        [
+            IntegerField(3, 5),
+            IntegerField(2, 9),
+            LiteralField(12, 14),
+            IntegerField(3, 29),
+            IntegerField(3, 34),
+            FloatField(10, 39, 3),
+            FloatField(10, 49, 3),
+            FloatField(10, 59, 3),
+        ]
+    )
 
-#     @num_patamares.setter
-#     def num_patamares(self, n: int):
-#         self.data[2] = n
+    @property
+    def codigo(self) -> Optional[int]:
+        """
+        O código de cadastro da UE.
 
-#     @property
-#     def cargas(self) -> Optional[List[float]]:
-#         """
-#         As cargas em Mwmed pata cada patamar de carga
+        :return: O código.
+        :rtype: int | None
+        """
+        return self.data[0]
 
-#         :return: As cargas.
-#         :rtype: list[float] | None
-#         """
-#         return [v for v in self.data[3::2] if v is not None]
+    @codigo.setter
+    def codigo(self, cod: int):
+        self.data[0] = cod
 
-#     @cargas.setter
-#     def cargas(self, c: List[float]):
-#         self.__atualiza_dados_lista(c, 3, 2)
+    @property
+    def submercado(self) -> Optional[int]:
+        """
+        O submercado de cadastro da UE.
 
-#     @property
-#     def duracoes(self) -> Optional[List[float]]:
-#         """
-#         As durações de cada patamar de carga em horas
+        :return: O submercado.
+        :rtype: int | None
+        """
+        return self.data[1]
 
-#         :return: As durações em horas.
-#         :rtype: list[float] | None
-#         """
-#         return [v for v in self.data[4::2] if v is not None]
+    @submercado.setter
+    def submercado(self, n: int):
+        self.data[1] = n
 
-#     @duracoes.setter
-#     def duracoes(self, d: List[float]):
-#         self.__atualiza_dados_lista(d, 4, 2)
+    @property
+    def nome(self) -> Optional[str]:
+        """
+        O nome da usina elevatória.
 
+        :return: O nome.
+        :rtype: str | None
+        """
+        return self.data[2]
 
-# class PQ(Register):
-#     """
-#     Registro que contém o cadastro da geração por pequenas usinas.
+    @nome.setter
+    def nome(self, v: str):
+        self.data[2] = v
 
-#     *OBS: Suporta apenas 3 patamares no momento*
-#     """
+    @property
+    def uhe_montante(self) -> Optional[int]:
+        """
+        O código da UHE a montante, conforme registro UH.
 
-#     IDENTIFIER = "PQ  "
-#     IDENTIFIER_DIGITS = 4
-#     LINE = Line(
-#         [
-#             LiteralField(10, 4),
-#             IntegerField(2, 14),
-#             IntegerField(2, 19),
-#             FloatField(5, 24, 0),
-#             FloatField(5, 29, 0),
-#             FloatField(5, 34, 0),
-#         ]
-#     )
+        :return: O código.
+        :rtype: int | None
+        """
+        return self.data[3]
 
-#     def __atualiza_dados_lista(
-#         self,
-#         novos_dados: list,
-#         indice_inicial: int,
-#         espacamento: int,
-#     ):
-#         atuais = len(self.data)
-#         ultimo_indice = indice_inicial + espacamento * len(novos_dados)
-#         diferenca = (ultimo_indice - atuais) // espacamento
-#         if diferenca > 0:
-#             self.data += [None] * (ultimo_indice - atuais)
-#             diferenca -= 1
-#         novos_dados += [None] * abs(diferenca)
-#         self.data[indice_inicial::espacamento] = novos_dados
+    @uhe_montante.setter
+    def uhe_montante(self, v: int):
+        self.data[3] = v
 
-#     @property
-#     def nome(self) -> Optional[str]:
-#         """
-#         O nome da geração.
+    @property
+    def uhe_jusante(self) -> Optional[int]:
+        """
+        O código da UHE a jusante, conforme registro UH.
 
-#         :return: O nome.
-#         :rtype: str | None
-#         """
-#         return self.data[0]
+        :return: O código.
+        :rtype: int | None
+        """
+        return self.data[4]
 
-#     @nome.setter
-#     def nome(self, nome: str):
-#         self.data[0] = nome
+    @uhe_jusante.setter
+    def uhe_jusante(self, e: int):
+        self.data[4] = e
 
-#     @property
-#     def subsistema(self) -> Optional[int]:
-#         """
-#         O subsistema associado à geração.
+    @property
+    def vazao_minima_bombeavel(self) -> Optional[float]:
+        """
+        A vazão mínima bombeável.
 
-#         :return: O subsistema.
-#         :rtype: int | None
-#         """
-#         return self.data[1]
+        :return: A vazão em m3/s
+        :rtype: float | None
+        """
+        return self.data[5]
 
-#     @subsistema.setter
-#     def subsistema(self, sub: int):
-#         self.data[1] = sub
+    @vazao_minima_bombeavel.setter
+    def vazao_minima_bombeavel(self, e: float):
+        self.data[5] = e
 
-#     @property
-#     def estagio(self) -> Optional[int]:
-#         """
-#         O estágio associado à geração.
+    @property
+    def vazao_maxima_bombeavel(self) -> Optional[float]:
+        """
+        A vazão mínima bombeável.
 
-#         :return: O estágio.
-#         :rtype: int | None
-#         """
-#         return self.data[2]
+        :return: A vazão em m3/s
+        :rtype: float | None
+        """
+        return self.data[6]
 
-#     @estagio.setter
-#     def estagio(self, e: int):
-#         self.data[2] = e
+    @vazao_maxima_bombeavel.setter
+    def vazao_maxima_bombeavel(self, e: float):
+        self.data[6] = e
 
-#     @property
-#     def geracoes(self) -> Optional[List[float]]:
-#         """
-#         As gerações em Mwmed para cada patamar de carga.
+    @property
+    def taxa_consumo(self) -> Optional[float]:
+        """
+        A taxa de consumo.
 
-#         :return: As gerações.
-#         :rtype: list[float] | None
-#         """
-#         return [v for v in self.data[3:6] if v is not None]
+        :return: A taxa em MWmed/m3/s.
+        :rtype: float | None
+        """
+        return self.data[7]
 
-#     @geracoes.setter
-#     def geracoes(self, c: List[float]):
-#         self.__atualiza_dados_lista(c, 3, 1)
+    @taxa_consumo.setter
+    def taxa_consumo(self, e: float):
+        self.data[7] = e
 
 
-# class CD(Register):
-#     """
-#     Registro que contém o cadastro dos custos de déficit.
+class DP(Register):
+    """
+    Registro que as demandas para os submercados que serão consideradas
+    para os períodos em que não se considerada a rede elétrica.
 
-#     *OBS: Suporta apenas 3 patamares no momento*
-#     """
+    """
 
-#     IDENTIFIER = "CD  "
-#     IDENTIFIER_DIGITS = 4
-#     LINE = Line(
-#         [
-#             IntegerField(2, 4),
-#             IntegerField(2, 9),
-#             LiteralField(10, 14),
-#             IntegerField(2, 24),
-#             FloatField(5, 29, 1),
-#             FloatField(10, 34, 2),
-#             FloatField(5, 44, 1),
-#             FloatField(10, 49, 2),
-#             FloatField(5, 59, 1),
-#             FloatField(10, 64, 2),
-#         ]
-#     )
+    IDENTIFIER = "DP  "
+    IDENTIFIER_DIGITS = 4
+    LINE = Line(
+        [
+            IntegerField(2, 4),
+            StageDateField(starting_position=8, special_day_character="I"),
+            StageDateField(starting_position=16, special_day_character="F"),
+            FloatField(10, 24, 1),
+        ]
+    )
 
-#     def __atualiza_dados_lista(
-#         self,
-#         novos_dados: list,
-#         indice_inicial: int,
-#         espacamento: int,
-#     ):
-#         atuais = len(self.data)
-#         ultimo_indice = indice_inicial + espacamento * len(novos_dados)
-#         diferenca = (ultimo_indice - atuais) // espacamento
-#         if diferenca > 0:
-#             self.data += [None] * (ultimo_indice - atuais)
-#             diferenca -= 1
-#         novos_dados += [None] * abs(diferenca)
-#         self.data[indice_inicial::espacamento] = novos_dados
+    @property
+    def submercado(self) -> Optional[int]:
+        """
+        O submercado associado à demanada especificada.
 
-#     @property
-#     def numero_curva(self) -> Optional[int]:
-#         """
-#         O número da curva de déficit.
+        :return: O submercado.
+        :rtype: int | None
+        """
+        return self.data[0]
 
-#         :return: O índice da curva.
-#         :rtype: int | None
-#         """
-#         return self.data[0]
+    @submercado.setter
+    def submercado(self, sub: int):
+        self.data[0] = sub
 
-#     @numero_curva.setter
-#     def numero_curva(self, n: int):
-#         self.data[0] = n
+    @property
+    def dia_inicial(self) -> Optional[Union[str, int]]:
+        """
+        O dia inicial.
 
-#     @property
-#     def subsistema(self) -> Optional[int]:
-#         """
-#         O índice do subsistema associado.
+        :return: O dia.
+        :rtype: str | int | None
+        """
 
-#         :return: O subsistema.
-#         :rtype: int | None
-#         """
-#         return self.data[1]
+        return self.data[1][0]
 
-#     @subsistema.setter
-#     def subsistema(self, s: int):
-#         self.data[1] = s
+    @dia_inicial.setter
+    def dia_inicial(self, n: Union[str, int]):
+        self.data[1][0] = n
 
-#     @property
-#     def nome_curva(self) -> Optional[str]:
-#         """
-#         O nome da curva de défitict
+    @property
+    def hora_inicial(self) -> Optional[int]:
+        """
+        A hora inicial.
 
-#         :return: O nome.
-#         :rtype: str | None
-#         """
-#         return self.data[2]
+        :return: A hora.
+        :rtype: int | None
+        """
+        return self.data[1][1]
 
-#     @nome_curva.setter
-#     def nome_curva(self, n: str):
-#         self.data[2] = n
+    @hora_inicial.setter
+    def hora_inicial(self, n: int):
+        self.data[1][1] = n
 
-#     @property
-#     def estagio(self) -> Optional[int]:
-#         """
-#         O estágio de vigência do custo de déficit
+    @property
+    def meia_hora_inicial(self) -> Optional[int]:
+        """
+        A meia-hora inicial.
 
-#         :return: O estágio.
-#         :rtype: int | None
-#         """
-#         return self.data[3]
+        :return: A meia-hora.
+        :rtype: int | None
+        """
+        return self.data[1][2]
 
-#     @estagio.setter
-#     def estagio(self, e: int):
-#         self.data[3] = e
+    @meia_hora_inicial.setter
+    def meia_hora_inicial(self, n: int):
+        self.data[1][2] = n
 
-#     @property
-#     def limites_superiores(self) -> Optional[List[float]]:
-#         """
-#         Os limites superiores para consideração dos custos.
+    @property
+    def dia_final(self) -> Optional[Union[str, int]]:
+        """
+        O dia final.
 
-#         :return: Os limites.
-#         :rtype: list[float] | None
-#         """
-#         return [v for v in self.data[4::2] if v is not None]
+        :return: O dia.
+        :rtype: str | int | None
+        """
 
-#     @limites_superiores.setter
-#     def limites_superiores(self, lim: List[float]):
-#         self.__atualiza_dados_lista(lim, 4, 2)
+        return self.data[2][0]
 
-#     @property
-#     def custos(self) -> Optional[List[float]]:
-#         """
-#         Os custos de déficit.
+    @dia_final.setter
+    def dia_final(self, n: Union[str, int]):
+        self.data[2][0] = n
 
-#         :return: Os custos.
-#         :rtype: list[float] | None
-#         """
-#         return [v for v in self.data[5::2] if v is not None]
+    @property
+    def hora_final(self) -> Optional[int]:
+        """
+        A hora final.
 
-#     @custos.setter
-#     def custos(self, cus: List[float]):
-#         self.__atualiza_dados_lista(cus, 5, 2)
+        :return: A hora.
+        :rtype: int | None
+        """
+        return self.data[2][1]
 
+    @hora_final.setter
+    def hora_final(self, n: int):
+        self.data[2][1] = n
 
-# class RI(Register):
-#     """
-#     Registro que contém as restrições de Itaipu.
+    @property
+    def meia_hora_final(self) -> Optional[int]:
+        """
+        A meia-hora final.
 
-#     *OBS: Suporta apenas 3 patamares no momento*
-#     """
+        :return: A meia-hora.
+        :rtype: int | None
+        """
+        return self.data[2][2]
 
-#     IDENTIFIER = "RI  "
-#     IDENTIFIER_DIGITS = 4
-#     LINE = Line(
-#         [
-#             IntegerField(3, 4),
-#             IntegerField(3, 8),
-#             IntegerField(3, 12),
-#             FloatField(7, 16, 0),
-#             FloatField(7, 23, 0),
-#             FloatField(7, 30, 0),
-#             FloatField(7, 37, 0),
-#             FloatField(7, 44, 0),
-#             FloatField(7, 51, 0),
-#             FloatField(7, 58, 0),
-#             FloatField(7, 65, 0),
-#             FloatField(7, 72, 0),
-#             FloatField(7, 79, 0),
-#             FloatField(7, 86, 0),
-#             FloatField(7, 93, 0),
-#             FloatField(7, 100, 0),
-#             FloatField(7, 107, 0),
-#             FloatField(7, 114, 0),
-#         ]
-#     )
+    @meia_hora_final.setter
+    def meia_hora_final(self, n: int):
+        self.data[2][2] = n
 
+    @property
+    def demanda(self) -> Optional[float]:
+        """
+        A demanda em Mwmed para o período especificado
 
-# class IA(Register):
-#     """
-#     Registro que contém os limites de intercâmbio entre os subsistemas.
+        :return: A demanda.
+        :rtype: float | None
+        """
+        return self.data[3]
 
-#     *OBS: Suporta apenas 3 patamares no momento*
-#     """
+    @demanda.setter
+    def demanda(self, demanda: float):
+        self.data[3] = demanda
 
-#     IDENTIFIER = "IA  "
-#     IDENTIFIER_DIGITS = 4
-#     LINE = Line(
-#         [
-#             IntegerField(2, 4),
-#             LiteralField(2, 9),
-#             LiteralField(2, 14),
-#             IntegerField(1, 17),
-#             FloatField(10, 19, 0),
-#             FloatField(10, 29, 0),
-#             FloatField(10, 39, 0),
-#             FloatField(10, 49, 0),
-#             FloatField(10, 59, 0),
-#             FloatField(10, 69, 0),
-#         ]
-#     )
+
+class DE(Register):
+    """
+    Registro que as demandas especiais para serem representadas em
+    restrições elétricas do tipo RE.
+
+    """
+
+    IDENTIFIER = "DE  "
+    IDENTIFIER_DIGITS = 4
+    LINE = Line(
+        [
+            IntegerField(2, 4),
+            StageDateField(starting_position=8, special_day_character="I"),
+            StageDateField(starting_position=16, special_day_character="F"),
+            FloatField(10, 24, 1),
+            LiteralField(10, 35),
+        ]
+    )
+
+    @property
+    def codigo(self) -> Optional[int]:
+        """
+        O código da demanda especial.
+
+        :return: O código.
+        :rtype: int | None
+        """
+        return self.data[0]
+
+    @codigo.setter
+    def codigo(self, sub: int):
+        self.data[0] = sub
+
+    @property
+    def dia_inicial(self) -> Optional[Union[str, int]]:
+        """
+        O dia inicial.
+
+        :return: O dia.
+        :rtype: str | int | None
+        """
+        return self.data[1][0]
+
+    @dia_inicial.setter
+    def dia_inicial(self, n: Union[str, int]):
+        self.data[1][0] = n
+
+    @property
+    def hora_inicial(self) -> Optional[int]:
+        """
+        A hora inicial.
+
+        :return: A hora.
+        :rtype: int | None
+        """
+        return self.data[1][1]
+
+    @hora_inicial.setter
+    def hora_inicial(self, n: int):
+        self.data[1][1] = n
+
+    @property
+    def meia_hora_inicial(self) -> Optional[int]:
+        """
+        A meia-hora inicial.
+
+        :return: A meia-hora.
+        :rtype: int | None
+        """
+        return self.data[1][2]
+
+    @meia_hora_inicial.setter
+    def meia_hora_inicial(self, n: int):
+        self.data[1][2] = n
+
+    @property
+    def dia_final(self) -> Optional[Union[str, int]]:
+        """
+        O dia final.
+
+        :return: O dia.
+        :rtype: str | int | None
+        """
+        return self.data[2][0]
+
+    @dia_final.setter
+    def dia_final(self, n: Union[str, int]):
+        self.data[2][0] = n
+
+    @property
+    def hora_final(self) -> Optional[int]:
+        """
+        A hora final.
+
+        :return: A hora.
+        :rtype: int | None
+        """
+        return self.data[2][1]
+
+    @hora_final.setter
+    def hora_final(self, n: int):
+        self.data[2][1] = n
+
+    @property
+    def meia_hora_final(self) -> Optional[int]:
+        """
+        A meia-hora final.
+
+        :return: A meia-hora.
+        :rtype: int | None
+        """
+        return self.data[2][2]
+
+    @meia_hora_final.setter
+    def meia_hora_final(self, n: int):
+        self.data[2][2] = n
+
+    @property
+    def demanda(self) -> Optional[float]:
+        """
+        A demanda em Mwmed para o período especificado
+
+        :return: A demanda.
+        :rtype: float | None
+        """
+        return self.data[3]
+
+    @demanda.setter
+    def demanda(self, demanda: float):
+        self.data[3] = demanda
+
+    @property
+    def justificativa(self) -> Optional[str]:
+        """
+        A descrição ou justificativa.
+
+        :return: A justificativa.
+        :rtype: str | None
+        """
+        return self.data[4]
+
+    @justificativa.setter
+    def justificativa(self, justificativa: str):
+        self.data[4] = justificativa
+
+
+class CD(Register):
+    """
+    Registro que contém o cadastro dos custos de déficit.
+
+    """
+
+    IDENTIFIER = "CD "
+    IDENTIFIER_DIGITS = 3
+    LINE = Line(
+        [
+            IntegerField(2, 4),
+            IntegerField(2, 6),
+            StageDateField(starting_position=9, special_day_character="I"),
+            StageDateField(starting_position=17, special_day_character="F"),
+            FloatField(10, 25, 2),
+            FloatField(10, 35, 2),
+        ]
+    )
+
+    @property
+    def submercado(self) -> Optional[int]:
+        """
+        O índice do submercado associado.
+
+        :return: O submercado.
+        :rtype: int | None
+        """
+        return self.data[0]
+
+    @submercado.setter
+    def submercado(self, s: int):
+        self.data[0] = s
+
+    @property
+    def numero_curva(self) -> Optional[int]:
+        """
+        O número da curva de déficit.
+
+        :return: O índice da curva.
+        :rtype: int | None
+        """
+        return self.data[1]
+
+    @numero_curva.setter
+    def numero_curva(self, n: int):
+        self.data[1] = n
+
+    @property
+    def dia_inicial(self) -> Optional[Union[str, int]]:
+        """
+        O dia inicial.
+
+        :return: O dia.
+        :rtype: str | int | None
+        """
+
+        return self.data[2][0]
+
+    @dia_inicial.setter
+    def dia_inicial(self, n: Union[str, int]):
+        self.data[2][0] = n
+
+    @property
+    def hora_inicial(self) -> Optional[int]:
+        """
+        A hora inicial.
+
+        :return: A hora.
+        :rtype: int | None
+        """
+        return self.data[2][1]
+
+    @hora_inicial.setter
+    def hora_inicial(self, n: int):
+        self.data[2][1] = n
+
+    @property
+    def meia_hora_inicial(self) -> Optional[int]:
+        """
+        A meia-hora inicial.
+
+        :return: A meia-hora.
+        :rtype: int | None
+        """
+        return self.data[2][2]
+
+    @meia_hora_inicial.setter
+    def meia_hora_inicial(self, n: int):
+        self.data[2][2] = n
+
+    @property
+    def dia_final(self) -> Optional[Union[str, int]]:
+        """
+        O dia final.
+
+        :return: O dia.
+        :rtype: str | int | None
+        """
+
+        return self.data[3][0]
+
+    @dia_final.setter
+    def dia_final(self, n: Union[str, int]):
+        self.data[3][0] = n
+
+    @property
+    def hora_final(self) -> Optional[int]:
+        """
+        A hora final.
+
+        :return: A hora.
+        :rtype: int | None
+        """
+        return self.data[3][1]
+
+    @hora_final.setter
+    def hora_final(self, n: int):
+        self.data[3][1] = n
+
+    @property
+    def meia_hora_final(self) -> Optional[int]:
+        """
+        A meia-hora final.
+
+        :return: A meia-hora.
+        :rtype: int | None
+        """
+        return self.data[3][2]
+
+    @meia_hora_final.setter
+    def meia_hora_final(self, n: int):
+        self.data[3][2] = n
+
+    @property
+    def custo(self) -> Optional[float]:
+        """
+        O custo de déficit.
+
+        :return: O custo.
+        :rtype: float | None
+        """
+        return self.data[4]
+
+    @custo.setter
+    def custo(self, cus: float):
+        self.data[4] = cus
+
+    @property
+    def limite_superior(self) -> Optional[float]:
+        """
+        O limite superior para consideração dos custos.
+
+        :return: O limite.
+        :rtype: float | None
+        """
+        return self.data[5]
+
+    @limite_superior.setter
+    def limite_superior(self, lim: float):
+        self.data[5] = lim
+
+
+class PQ(Register):
+    """
+    Registro que contém o cadastro da geração por pequenas usinas.
+
+    """
+
+    IDENTIFIER = "PQ  "
+    IDENTIFIER_DIGITS = 4
+    LINE = Line(
+        [
+            IntegerField(3, 4),
+            LiteralField(10, 9),
+            IntegerField(5, 19),
+            StageDateField(starting_position=24, special_day_character="I"),
+            StageDateField(starting_position=32, special_day_character="F"),
+            FloatField(10, 40, 1),
+        ]
+    )
+
+    @property
+    def codigo(self) -> Optional[str]:
+        """
+        O código da pequena usina.
+
+        :return: O código.
+        :rtype: str | None
+        """
+        return self.data[0]
+
+    @codigo.setter
+    def codigo(self, nome: str):
+        self.data[0] = nome
+
+    @property
+    def nome(self) -> Optional[str]:
+        """
+        O nome da pequena usina.
+
+        :return: O nome.
+        :rtype: str | None
+        """
+        return self.data[1]
+
+    @nome.setter
+    def nome(self, nome: str):
+        self.data[1] = nome
+
+    @property
+    def localizacao(self) -> Optional[int]:
+        """
+        O indice do subsistema  ou barra associado à geração.
+
+        :return: O índice da localização.
+        :rtype: int | None
+        """
+        return self.data[2]
+
+    @localizacao.setter
+    def localizacao(self, sub: int):
+        self.data[2] = sub
+
+    @property
+    def dia_inicial(self) -> Optional[Union[str, int]]:
+        """
+        O dia inicial.
+
+        :return: O dia.
+        :rtype: str | int | None
+        """
+
+        return self.data[3][0]
+
+    @dia_inicial.setter
+    def dia_inicial(self, n: Union[str, int]):
+        self.data[3][0] = n
+
+    @property
+    def hora_inicial(self) -> Optional[int]:
+        """
+        A hora inicial.
+
+        :return: A hora.
+        :rtype: int | None
+        """
+        return self.data[3][1]
+
+    @hora_inicial.setter
+    def hora_inicial(self, n: int):
+        self.data[3][1] = n
+
+    @property
+    def meia_hora_inicial(self) -> Optional[int]:
+        """
+        A meia-hora inicial.
+
+        :return: A meia-hora.
+        :rtype: int | None
+        """
+        return self.data[3][2]
+
+    @meia_hora_inicial.setter
+    def meia_hora_inicial(self, n: int):
+        self.data[3][2] = n
+
+    @property
+    def dia_final(self) -> Optional[Union[str, int]]:
+        """
+        O dia final.
+
+        :return: O dia.
+        :rtype: str | int | None
+        """
+
+        return self.data[4][0]
+
+    @dia_final.setter
+    def dia_final(self, n: Union[str, int]):
+        self.data[4][0] = n
+
+    @property
+    def hora_final(self) -> Optional[int]:
+        """
+        A hora final.
+
+        :return: A hora.
+        :rtype: int | None
+        """
+        return self.data[4][1]
+
+    @hora_final.setter
+    def hora_final(self, n: int):
+        self.data[4][1] = n
+
+    @property
+    def meia_hora_final(self) -> Optional[int]:
+        """
+        A meia-hora final.
+
+        :return: A meia-hora.
+        :rtype: int | None
+        """
+        return self.data[4][2]
+
+    @meia_hora_final.setter
+    def meia_hora_final(self, n: int):
+        self.data[4][2] = n
+
+    @property
+    def geracao(self) -> Optional[float]:
+        """
+        A geração da pequena usina.
+
+        :return: A geração.
+        :rtype: float | None
+        """
+        return self.data[5]
+
+    @geracao.setter
+    def geracao(self, ger: float):
+        self.data[5] = ger
+
+
+class IT(Register):
+    """
+    Registro que contém os coeficientes do polinômio do canal de fuga
+    de Itaipu em função da vazão na Régua 11, para casos sem FPHA Libs.
+    """
+
+    IDENTIFIER = "IT  "
+    IDENTIFIER_DIGITS = 4
+    LINE = Line(
+        [
+            IntegerField(2, 4),
+            FloatField(15, 9, 7, format="E"),
+            FloatField(15, 24, 7, format="E"),
+            FloatField(15, 39, 7, format="E"),
+            FloatField(15, 54, 7, format="E"),
+            FloatField(15, 69, 7, format="E"),
+        ]
+    )
+
+    @property
+    def ree(self) -> Optional[int]:
+        """
+        O código do REE em que se encontra a usina
+        de Itaipu.
+
+        :return: O ree.
+        :rtype: int | None
+        """
+
+        return self.data[0]
+
+    @ree.setter
+    def ree(self, n: int):
+        self.data[0] = n
+
+    @property
+    def coeficiente_a0(self) -> Optional[float]:
+        """
+        O coeficiente de grau 0 do polinômio.
+
+        :return: O coeficiente.
+        :rtype: float | None
+        """
+
+        return self.data[1]
+
+    @coeficiente_a0.setter
+    def coeficiente_a0(self, c: float):
+        self.data[1] = c
+
+    @property
+    def coeficiente_a1(self) -> Optional[float]:
+        """
+        O coeficiente de grau 1 do polinômio.
+
+        :return: O coeficiente.
+        :rtype: float | None
+        """
+
+        return self.data[2]
+
+    @coeficiente_a1.setter
+    def coeficiente_a1(self, c: float):
+        self.data[2] = c
+
+    @property
+    def coeficiente_a2(self) -> Optional[float]:
+        """
+        O coeficiente de grau 2 do polinômio.
+
+        :return: O coeficiente.
+        :rtype: float | None
+        """
+
+        return self.data[3]
+
+    @coeficiente_a2.setter
+    def coeficiente_a2(self, c: float):
+        self.data[3] = c
+
+    @property
+    def coeficiente_a3(self) -> Optional[float]:
+        """
+        O coeficiente de grau 3 do polinômio.
+
+        :return: O coeficiente.
+        :rtype: float | None
+        """
+
+        return self.data[4]
+
+    @coeficiente_a3.setter
+    def coeficiente_a3(self, c: float):
+        self.data[4] = c
+
+    @property
+    def coeficiente_a4(self) -> Optional[float]:
+        """
+        O coeficiente de grau 4 do polinômio.
+
+        :return: O coeficiente.
+        :rtype: float | None
+        """
+
+        return self.data[5]
+
+    @coeficiente_a4.setter
+    def coeficiente_a4(self, c: float):
+        self.data[5] = c
+
+
+class RI(Register):
+    """
+    Registro que contém as restrições de Itaipu.
+
+    """
+
+    IDENTIFIER = "RI  "
+    IDENTIFIER_DIGITS = 4
+    LINE = Line(
+        [
+            StageDateField(starting_position=8, special_day_character="I"),
+            StageDateField(starting_position=16, special_day_character="F"),
+            FloatField(10, 26, 2),
+            FloatField(10, 36, 2),
+            FloatField(10, 46, 2),
+            FloatField(10, 56, 2),
+            FloatField(10, 66, 2),
+        ]
+    )
+
+    @property
+    def dia_inicial(self) -> Optional[Union[str, int]]:
+        """
+        O dia inicial.
+
+        :return: O dia.
+        :rtype: str | int | None
+        """
+
+        return self.data[0][0]
+
+    @dia_inicial.setter
+    def dia_inicial(self, n: Union[str, int]):
+        self.data[0][0] = n
+
+    @property
+    def hora_inicial(self) -> Optional[int]:
+        """
+        A hora inicial.
+
+        :return: A hora.
+        :rtype: int | None
+        """
+        return self.data[0][1]
+
+    @hora_inicial.setter
+    def hora_inicial(self, n: int):
+        self.data[0][1] = n
+
+    @property
+    def meia_hora_inicial(self) -> Optional[int]:
+        """
+        A meia-hora inicial.
+
+        :return: A meia-hora.
+        :rtype: int | None
+        """
+        return self.data[0][2]
+
+    @meia_hora_inicial.setter
+    def meia_hora_inicial(self, n: int):
+        self.data[0][2] = n
+
+    @property
+    def dia_final(self) -> Optional[Union[str, int]]:
+        """
+        O dia final.
+
+        :return: O dia.
+        :rtype: str | int | None
+        """
+
+        return self.data[1][0]
+
+    @dia_final.setter
+    def dia_final(self, n: Union[str, int]):
+        self.data[1][0] = n
+
+    @property
+    def hora_final(self) -> Optional[int]:
+        """
+        A hora final.
+
+        :return: A hora.
+        :rtype: int | None
+        """
+        return self.data[1][1]
+
+    @hora_final.setter
+    def hora_final(self, n: int):
+        self.data[1][1] = n
+
+    @property
+    def meia_hora_final(self) -> Optional[int]:
+        """
+        A meia-hora final.
+
+        :return: A meia-hora.
+        :rtype: int | None
+        """
+        return self.data[1][2]
+
+    @meia_hora_final.setter
+    def meia_hora_final(self, n: int):
+        self.data[1][2] = n
+
+    @property
+    def geracao_minima_50hz(self) -> Optional[float]:
+        """
+        O limite inferior para a geração 50 Hz de Itaipu.
+
+        :return: O limite.
+        :rtype: float | None
+        """
+        return self.data[2]
+
+    @geracao_minima_50hz.setter
+    def geracao_minima_50hz(self, n: float):
+        self.data[2] = n
+
+    @property
+    def geracao_maxima_50hz(self) -> Optional[float]:
+        """
+        O limite superior para a geração 50 Hz de Itaipu.
+
+        :return: O limite.
+        :rtype: float | None
+        """
+        return self.data[3]
+
+    @geracao_maxima_50hz.setter
+    def geracao_maxima_50hz(self, n: float):
+        self.data[3] = n
+
+    @property
+    def geracao_minima_60hz(self) -> Optional[float]:
+        """
+        O limite inferior para a geração 60 Hz de Itaipu.
+
+        :return: O limite.
+        :rtype: float | None
+        """
+        return self.data[4]
+
+    @geracao_minima_60hz.setter
+    def geracao_minima_60hz(self, n: float):
+        self.data[4] = n
+
+    @property
+    def geracao_maxima_60hz(self) -> Optional[float]:
+        """
+        O limite superior para a geração 60 Hz de Itaipu.
+
+        :return: O limite.
+        :rtype: float | None
+        """
+        return self.data[5]
+
+    @geracao_maxima_60hz.setter
+    def geracao_maxima_60hz(self, n: float):
+        self.data[5] = n
+
+    @property
+    def carga_ande(self) -> Optional[float]:
+        """
+        A carga da ANDE.
+
+        :return: A carga.
+        :rtype: float | None
+        """
+        return self.data[6]
+
+    @carga_ande.setter
+    def carga_ande(self, n: float):
+        self.data[6] = n
+
+
+class IA(Register):
+    """
+    Registro que contém os limites de intercâmbio entre os subsistemas.
+
+    """
+
+    IDENTIFIER = "IA  "
+    IDENTIFIER_DIGITS = 4
+    LINE = Line(
+        [
+            LiteralField(2, 4),
+            LiteralField(2, 9),
+            StageDateField(starting_position=13, special_day_character="I"),
+            StageDateField(starting_position=21, special_day_character="F"),
+            FloatField(10, 29, 1),
+            FloatField(10, 39, 1),
+        ]
+    )
+
+    @property
+    def submercado_de(self) -> Optional[str]:
+        """
+        O submercado de origem (de).
+
+        :return: O submercado.
+        :rtype: str | None
+        """
+
+        return self.data[0]
+
+    @submercado_de.setter
+    def submercado_de(self, n: str):
+        self.data[0] = n
+
+    @property
+    def submercado_para(self) -> Optional[str]:
+        """
+        O submercado de destino (para).
+
+        :return: O submercado.
+        :rtype: str | None
+        """
+
+        return self.data[1]
+
+    @submercado_para.setter
+    def submercado_para(self, n: str):
+        self.data[1] = n
+
+    @property
+    def dia_inicial(self) -> Optional[Union[str, int]]:
+        """
+        O dia inicial.
+
+        :return: O dia.
+        :rtype: str | int | None
+        """
+
+        return self.data[2][0]
+
+    @dia_inicial.setter
+    def dia_inicial(self, n: Union[str, int]):
+        self.data[2][0] = n
+
+    @property
+    def hora_inicial(self) -> Optional[int]:
+        """
+        A hora inicial.
+
+        :return: A hora.
+        :rtype: int | None
+        """
+        return self.data[2][1]
+
+    @hora_inicial.setter
+    def hora_inicial(self, n: int):
+        self.data[2][1] = n
+
+    @property
+    def meia_hora_inicial(self) -> Optional[int]:
+        """
+        A meia-hora inicial.
+
+        :return: A meia-hora.
+        :rtype: int | None
+        """
+        return self.data[2][2]
+
+    @meia_hora_inicial.setter
+    def meia_hora_inicial(self, n: int):
+        self.data[2][2] = n
+
+    @property
+    def dia_final(self) -> Optional[Union[str, int]]:
+        """
+        O dia final.
+
+        :return: O dia.
+        :rtype: str | int | None
+        """
+
+        return self.data[3][0]
+
+    @dia_final.setter
+    def dia_final(self, n: Union[str, int]):
+        self.data[3][0] = n
+
+    @property
+    def hora_final(self) -> Optional[int]:
+        """
+        A hora final.
+
+        :return: A hora.
+        :rtype: int | None
+        """
+        return self.data[3][1]
+
+    @hora_final.setter
+    def hora_final(self, n: int):
+        self.data[3][1] = n
+
+    @property
+    def meia_hora_final(self) -> Optional[int]:
+        """
+        A meia-hora final.
+
+        :return: A meia-hora.
+        :rtype: int | None
+        """
+        return self.data[3][2]
+
+    @meia_hora_final.setter
+    def meia_hora_final(self, n: int):
+        self.data[3][2] = n
+
+    @property
+    def capacidade_de(self) -> Optional[float]:
+        """
+        A capacidade do intercâmbio do submercado de ao submercado para.
+
+        :return: A capacidade.
+        :rtype: float | None
+        """
+        return self.data[4]
+
+    @capacidade_de.setter
+    def capacidade_de(self, n: float):
+        self.data[4] = n
+
+    @property
+    def capacidade_para(self) -> Optional[float]:
+        """
+        A capacidade do intercâmbio do submercado para ao submercado de.
+
+        :return: A capacidade.
+        :rtype: float | None
+        """
+        return self.data[5]
+
+    @capacidade_para.setter
+    def capacidade_para(self, n: float):
+        self.data[5] = n
+
+
+class GP(Register):
+    """
+    Registro que contém os gaps de tolerância para convergência
+    para os métodos PDD ou MILP.
+    """
+
+    IDENTIFIER = "GP  "
+    IDENTIFIER_DIGITS = 4
+    LINE = Line([FloatField(10, 4, 8), FloatField(10, 15, 8)])
+
+    @property
+    def gap_pdd(self) -> Optional[float]:
+        """
+        O gap de convergência do processo iterativo de
+        programação dinâmica dual (PDD).
+
+        :return: O gap.
+        :rtype: float | None
+        """
+
+        return self.data[0]
+
+    @gap_pdd.setter
+    def gap_pdd(self, n: float):
+        self.data[0] = n
+
+    @property
+    def gap_milp(self) -> Optional[float]:
+        """
+        O gap de convergência do problema por programação
+        linear inteira mista (MILP).
+
+        :return: O gap.
+        :rtype: float | None
+        """
+
+        return self.data[1]
+
+    @gap_milp.setter
+    def gap_milp(self, n: float):
+        self.data[1] = n
+
+
+class ACVTFUGA(Register):
+    """
+    Registro AC específico para consideração da influência do vertimento
+    no canal de fuga.
+    """
+
+    IDENTIFIER = r"AC  ([\d ]{1,3})  VTFUGA"
+    IDENTIFIER_DIGITS = 15
+    LINE = Line(
+        [
+            IntegerField(3, 4),
+            IntegerField(5, 19),
+        ]
+    )
+
+    # Override
+    def write(self, file: IO, storage: str = "", *args, **kwargs) -> bool:
+        line = self.__class__.LINE.write(self.data)
+        line = (
+            self.__class__.IDENTIFIER[:2]  # type: ignore
+            + line[2:9]
+            + self.__class__.IDENTIFIER[18:]
+            + line[15:]
+        )
+        file.write(line)
+        return True
+
+    @property
+    def uhe(self) -> Optional[int]:
+        return self.data[0]
+
+    @uhe.setter
+    def uhe(self, u: int):
+        self.data[0] = u
+
+    @property
+    def influi(self) -> Optional[int]:
+        return self.data[1]
+
+    @influi.setter
+    def influi(self, u: int):
+        self.data[1] = u
+
+
+class ACVOLMAX(Register):
+    """
+    Registro AC específico para alteração de volume máximo.
+    """
+
+    IDENTIFIER = r"AC  ([\d ]{1,3})  VOLMAX"
+    IDENTIFIER_DIGITS = 15
+    LINE = Line(
+        [
+            IntegerField(3, 4),
+            FloatField(10, 19, 3),
+        ]
+    )
+
+    # Override
+    def write(self, file: IO, storage: str = "", *args, **kwargs) -> bool:
+        line = self.__class__.LINE.write(self.data)
+        line = (
+            self.__class__.IDENTIFIER[:2]  # type: ignore
+            + line[2:9]
+            + self.__class__.IDENTIFIER[18:]
+            + line[15:]
+        )
+        file.write(line)
+        return True
+
+    @property
+    def uhe(self) -> Optional[int]:
+        return self.data[0]
+
+    @uhe.setter
+    def uhe(self, u: int):
+        self.data[0] = u
+
+    @property
+    def volume(self) -> Optional[float]:
+        return self.data[1]
+
+    @volume.setter
+    def volume(self, u: float):
+        self.data[1] = u
+
+
+class ACVOLMIN(Register):
+    """
+    Registro AC específico para alteração de volume mínimo.
+    """
+
+    IDENTIFIER = r"AC  ([\d ]{1,3})  VOLMIN"
+    IDENTIFIER_DIGITS = 15
+    LINE = Line(
+        [
+            IntegerField(3, 4),
+            FloatField(10, 19, 3),
+        ]
+    )
+
+    # Override
+    def write(self, file: IO, storage: str = "", *args, **kwargs) -> bool:
+        line = self.__class__.LINE.write(self.data)
+        line = (
+            self.__class__.IDENTIFIER[:2]  # type: ignore
+            + line[2:9]
+            + self.__class__.IDENTIFIER[18:]
+            + line[15:]
+        )
+        file.write(line)
+        return True
+
+    @property
+    def uhe(self) -> Optional[int]:
+        return self.data[0]
+
+    @uhe.setter
+    def uhe(self, u: int):
+        self.data[0] = u
+
+    @property
+    def volume(self) -> Optional[float]:
+        return self.data[1]
+
+    @volume.setter
+    def volume(self, u: float):
+        self.data[1] = u
+
+
+class ACVSVERT(Register):
+    """
+    Registro AC específico para alteração do volume mínimo para operação
+    do vertedor.
+    """
+
+    IDENTIFIER = r"AC  ([\d ]{1,3})  VSVERT"
+    IDENTIFIER_DIGITS = 15
+    LINE = Line(
+        [
+            IntegerField(3, 4),
+            FloatField(10, 19, 3),
+        ]
+    )
+
+    # Override
+    def write(self, file: IO, storage: str = "", *args, **kwargs) -> bool:
+        line = self.__class__.LINE.write(self.data)
+        line = (
+            self.__class__.IDENTIFIER[:2]  # type: ignore
+            + line[2:9]
+            + self.__class__.IDENTIFIER[18:]
+            + line[15:]
+        )
+        file.write(line)
+        return True
+
+    @property
+    def uhe(self) -> Optional[int]:
+        return self.data[0]
+
+    @uhe.setter
+    def uhe(self, u: int):
+        self.data[0] = u
+
+    @property
+    def volume(self) -> Optional[float]:
+        return self.data[1]
+
+    @volume.setter
+    def volume(self, u: float):
+        self.data[1] = u
+
+
+class ACVMDESV(Register):
+    """
+    Registro AC específico para alteração do volume mínimo para operação
+    do canal de desvio.
+    """
+
+    IDENTIFIER = r"AC  ([\d ]{1,3})  VMDESV"
+    IDENTIFIER_DIGITS = 15
+    LINE = Line(
+        [
+            IntegerField(3, 4),
+            FloatField(10, 19, 3),
+        ]
+    )
+
+    # Override
+    def write(self, file: IO, storage: str = "", *args, **kwargs) -> bool:
+        line = self.__class__.LINE.write(self.data)
+        line = (
+            self.__class__.IDENTIFIER[:2]  # type: ignore
+            + line[2:9]
+            + self.__class__.IDENTIFIER[18:]
+            + line[15:]
+        )
+        file.write(line)
+        return True
+
+    @property
+    def uhe(self) -> Optional[int]:
+        return self.data[0]
+
+    @uhe.setter
+    def uhe(self, u: int):
+        self.data[0] = u
+
+    @property
+    def volume(self) -> Optional[float]:
+        return self.data[1]
+
+    @volume.setter
+    def volume(self, u: float):
+        self.data[1] = u
+
+
+class ACCOTVAZ(Register):
+    """
+    Registro AC específico para alteração de um coeficiente do
+    polinômio cota-vazão.
+    """
+
+    IDENTIFIER = r"AC  ([\d ]{1,3})  COTVAZ"
+    IDENTIFIER_DIGITS = 15
+    LINE = Line(
+        [
+            IntegerField(3, 4),
+            IntegerField(5, 19),
+            FloatField(15, 24, 8, format="E"),
+            IntegerField(5, 39),
+        ]
+    )
+
+    # Override
+    def write(self, file: IO, storage: str = "", *args, **kwargs) -> bool:
+        line = self.__class__.LINE.write(self.data)
+        line = (
+            self.__class__.IDENTIFIER[:2]  # type: ignore
+            + line[2:9]
+            + self.__class__.IDENTIFIER[18:]
+            + line[15:]
+        )
+        file.write(line)
+        return True
+
+    @property
+    def uhe(self) -> Optional[int]:
+        return self.data[0]
+
+    @uhe.setter
+    def uhe(self, u: int):
+        self.data[0] = u
+
+    @property
+    def ordem(self) -> Optional[int]:
+        return self.data[1]
+
+    @ordem.setter
+    def ordem(self, u: int):
+        self.data[1] = u
+
+    @property
+    def coeficiente(self) -> Optional[float]:
+        return self.data[2]
+
+    @coeficiente.setter
+    def coeficiente(self, u: float):
+        self.data[2] = u
+
+    @property
+    def polimonio(self) -> Optional[int]:
+        return self.data[3]
+
+    @polimonio.setter
+    def polimonio(self, u: int):
+        self.data[3] = u
 
 
 # class TX(Register):
 #     """
 #     Registro que contém a taxa de desconto anual do modelo.
 #     """
 
@@ -1314,27 +2462,14 @@
 #         return self.data[0]
 
 #     @taxa.setter
 #     def taxa(self, t: float):
 #         self.data[0] = t
 
 
-# class GP(Register):
-#     """
-#     Registro que contém o gap de tolerância para convergência.
-#     """
-
-#     IDENTIFIER = "GP  "
-#     IDENTIFIER_DIGITS = 4
-#     LINE = Line(
-#         [
-#             FloatField(10, 4, 6),
-#         ]
-#     )
-
 #     @property
 #     def gap(self) -> Optional[float]:
 #         """
 #         O gap considerado para convergência no estudo
 
 #         :return: O gap.
 #         :rtype: float | None
@@ -2006,99 +3141,14 @@
 #         return self.data[4]
 
 #     @coeficiente.setter
 #     def coeficiente(self, f: float):
 #         self.data[4] = f
 
 
-# class VI(Register):
-#     """
-#     Registro que contém os tempos de viagem da água entre usinas.
-#     """
-
-#     IDENTIFIER = "VI  "
-#     IDENTIFIER_DIGITS = 4
-#     LINE = Line(
-#         [
-#             IntegerField(3, 4),
-#             IntegerField(3, 9),
-#             FloatField(5, 14, 0),
-#             FloatField(5, 19, 0),
-#             FloatField(5, 24, 0),
-#             FloatField(5, 29, 0),
-#             FloatField(5, 34, 0),
-#             FloatField(5, 39, 0),
-#             FloatField(5, 44, 0),
-#             FloatField(5, 49, 0),
-#             FloatField(5, 54, 0),
-#         ]
-#     )
-
-#     def __atualiza_dados_lista(
-#         self,
-#         novos_dados: list,
-#         indice_inicial: int,
-#         espacamento: int,
-#     ):
-#         atuais = len(self.data)
-#         ultimo_indice = indice_inicial + espacamento * len(novos_dados)
-#         diferenca = (ultimo_indice - atuais) // espacamento
-#         if diferenca > 0:
-#             self.data += [None] * (ultimo_indice - atuais)
-#             diferenca -= 1
-#         novos_dados += [None] * abs(diferenca)
-#         self.data[indice_inicial::espacamento] = novos_dados
-
-#     @property
-#     def uhe(self) -> Optional[int]:
-#         """
-#         O código da UHE a partir do qual é contabilizado
-#         o tempo de viagem.
-
-#         :return: O código
-#         :rtype: int | None
-#         """
-#         return self.data[0]
-
-#     @uhe.setter
-#     def uhe(self, u: int):
-#         self.data[0] = u
-
-#     @property
-#     def duracao(self) -> Optional[int]:
-#         """
-#         A duração da viagem da água (em horas) entre a UHE do
-#         código informado e sua usina à jusante segundo o hidr.
-
-#         :return: A duração
-#         :rtype: int | None
-#         """
-#         return self.data[1]
-
-#     @duracao.setter
-#     def duracao(self, d: int):
-#         self.data[1] = d
-
-#     @property
-#     def vazoes(self) -> Optional[List[float]]:
-#         """
-#         As vazões defluentes das semanas passadas para a usina
-#         do código informado. A posição da vazão na lista indica
-#         a qual semana passada se refere [s-1, s-2, s-3, ...].
-
-#         :return: As vazões
-#         :rtype: list[float] | None
-#         """
-#         return [v for v in self.data[2::] if v is not None]
-
-#     @vazoes.setter
-#     def vazoes(self, v: List[float]):
-#         self.__atualiza_dados_lista(v, 2, 1)
-
-
 # class IR(Register):
 #     """
 #     Registro que contém as configurações de
 #     geração de relatórios de saída.
 #     """
 
 #     IDENTIFIER = "IR  "
@@ -4341,84 +5391,14 @@
 #         return self.data[-1]
 
 #     @ano.setter
 #     def ano(self, m: int):
 #         self.data[-1] = m
 
 
-# class ACVOLMAX(Register):
-#     """
-#     Registro AC específico para alteração de volume máximo.
-#     """
-
-#     IDENTIFIER = r"AC  ([\d ]{1,3})  VOLMAX"
-#     IDENTIFIER_DIGITS = 15
-#     LINE = Line(
-#         [
-#             IntegerField(3, 4),
-#             FloatField(10, 19, 2),
-#             LiteralField(3, 69),
-#             IntegerField(2, 73),
-#             IntegerField(4, 76),
-#         ]
-#     )
-
-#     # Override
-#     def write(self, file: IO, storage: str = "") -> bool:
-#         line = self.__class__.LINE.write(self.data)
-#         line = (
-#             self.__class__.IDENTIFIER[:2]  # type: ignore
-#             + line[2:9]
-#             + self.__class__.IDENTIFIER[18:]
-#             + line[15:]
-#         )
-#         file.write(line)
-#         return True
-
-#     @property
-#     def uhe(self) -> Optional[int]:
-#         return self.data[0]
-
-#     @uhe.setter
-#     def uhe(self, u: int):
-#         self.data[0] = u
-
-#     @property
-#     def volume(self) -> Optional[float]:
-#         return self.data[1]
-
-#     @volume.setter
-#     def volume(self, u: float):
-#         self.data[1] = u
-
-#     @property
-#     def mes(self) -> Optional[str]:
-#         return self.data[-3]
-
-#     @mes.setter
-#     def mes(self, m: str):
-#         self.data[-3] = m
-
-#     @property
-#     def semana(self) -> Optional[int]:
-#         return self.data[-2]
-
-#     @semana.setter
-#     def semana(self, s: int):
-#         self.data[-2] = s
-
-#     @property
-#     def ano(self) -> Optional[int]:
-#         return self.data[-1]
-
-#     @ano.setter
-#     def ano(self, m: int):
-#         self.data[-1] = m
-
-
 # class ACCOTVOL(Register):
 #     """
 #     Registro AC específico para alteração de um coeficiente do
 #     polinômio cota-volume.
 #     """
 
 #     IDENTIFIER = r"AC  ([\d ]{1,3})  COTVOL"
@@ -5388,85 +6368,14 @@
 #         self.data[1] = u
 
 #     @property
 #     def mes(self) -> Optional[str]:
 #         return self.data[-3]
 
 #     @mes.setter
-#     def mes(self, m: str):
-#         self.data[-3] = m
-
-#     @property
-#     def semana(self) -> Optional[int]:
-#         return self.data[-2]
-
-#     @semana.setter
-#     def semana(self, s: int):
-#         self.data[-2] = s
-
-#     @property
-#     def ano(self) -> Optional[int]:
-#         return self.data[-1]
-
-#     @ano.setter
-#     def ano(self, m: int):
-#         self.data[-1] = m
-
-
-# class ACVERTJU(Register):
-#     """
-#     Registro AC específico para consideração da influência do vertimento
-#     no canal de fuga.
-#     """
-
-#     IDENTIFIER = r"AC  ([\d ]{1,3})  VERTJU"
-#     IDENTIFIER_DIGITS = 15
-#     LINE = Line(
-#         [
-#             IntegerField(3, 4),
-#             IntegerField(5, 19),
-#             LiteralField(3, 69),
-#             IntegerField(2, 73),
-#             IntegerField(4, 76),
-#         ]
-#     )
-
-#     # Override
-#     def write(self, file: IO, storage: str = "") -> bool:
-#         line = self.__class__.LINE.write(self.data)
-#         line = (
-#             self.__class__.IDENTIFIER[:2]  # type: ignore
-#             + line[2:9]
-#             + self.__class__.IDENTIFIER[18:]
-#             + line[15:]
-#         )
-#         file.write(line)
-#         return True
-
-#     @property
-#     def uhe(self) -> Optional[int]:
-#         return self.data[0]
-
-#     @uhe.setter
-#     def uhe(self, u: int):
-#         self.data[0] = u
-
-#     @property
-#     def influi(self) -> Optional[int]:
-#         return self.data[1]
-
-#     @influi.setter
-#     def influi(self, u: int):
-#         self.data[1] = u
-
-#     @property
-#     def mes(self) -> Optional[str]:
-#         return self.data[-3]
-
-#     @mes.setter
 #     def mes(self, m: str):
 #         self.data[-3] = m
 
 #     @property
 #     def semana(self) -> Optional[int]:
 #         return self.data[-2]
```

### Comparing `idessem-0.0.7/idessem/dessem/modelos/hidr.py` & `idessem-0.0.8/idessem/dessem/modelos/hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/log_matriz.py` & `idessem-0.0.8/idessem/dessem/modelos/log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/operut.py` & `idessem-0.0.8/idessem/dessem/modelos/operut.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/pdo_eco_fcfcortes.py` & `idessem-0.0.8/idessem/dessem/modelos/pdo_eco_fcfcortes.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/pdo_eco_usih.py` & `idessem-0.0.8/idessem/dessem/modelos/pdo_eco_usih.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/pdo_eco_usih_polin.py` & `idessem-0.0.8/idessem/dessem/modelos/pdo_eco_usih_polin.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/pdo_hidr.py` & `idessem-0.0.8/idessem/dessem/modelos/pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/pdo_oper_uct.py` & `idessem-0.0.8/idessem/dessem/modelos/pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/pdo_sist.py` & `idessem-0.0.8/idessem/dessem/modelos/pdo_sist.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/polinjus.py` & `idessem-0.0.8/idessem/dessem/modelos/polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/modelos/renovaveis.py` & `idessem-0.0.8/idessem/dessem/modelos/renovaveis.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/operut.py` & `idessem-0.0.8/idessem/dessem/operut.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/pdo_eco_fcfcortes.py` & `idessem-0.0.8/idessem/dessem/pdo_eco_fcfcortes.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/pdo_eco_usih.py` & `idessem-0.0.8/idessem/dessem/pdo_eco_usih.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/pdo_eco_usih_polin.py` & `idessem-0.0.8/idessem/dessem/pdo_eco_usih_polin.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/pdo_hidr.py` & `idessem-0.0.8/idessem/dessem/pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/pdo_oper_uct.py` & `idessem-0.0.8/idessem/dessem/pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/pdo_sist.py` & `idessem-0.0.8/idessem/dessem/pdo_sist.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/polinjus.py` & `idessem-0.0.8/idessem/dessem/polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem/dessem/renovaveis.py` & `idessem-0.0.8/idessem/dessem/renovaveis.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/idessem.egg-info/PKG-INFO` & `idessem-0.0.8/idessem.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idessem
-Version: 0.0.7
+Version: 0.0.8
 Summary: Interface para arquivos do DESSEM
 Home-page: https://github.com/rjmalves/idessem
 Author: Rogerio Alves, Mariana Noel
 Author-email: rogerioalves.ee@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `idessem-0.0.7/idessem.egg-info/SOURCES.txt` & `idessem-0.0.8/idessem.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -49,14 +49,16 @@
 idessem/dessem/modelos/renovaveis.py
 idessem/dessem/modelos/arquivos/__init__.py
 idessem/dessem/modelos/arquivos/arquivocsv.py
 idessem/dessem/modelos/blocos/__init__.py
 idessem/dessem/modelos/blocos/dataestudo.py
 idessem/dessem/modelos/blocos/tabelacsv.py
 idessem/dessem/modelos/blocos/versaomodelo.py
+idessem/dessem/modelos/componentes/__init__.py
+idessem/dessem/modelos/componentes/stagedatefield.py
 tests/__init__.py
 tests/dessem/__init__.py
 tests/dessem/test_avl_altqueda.py
 tests/dessem/test_avl_desvfpha.py
 tests/dessem/test_avl_fpha1.py
 tests/dessem/test_des_log_relato.py
 tests/dessem/test_dessemarq.py
@@ -68,14 +70,16 @@
 tests/dessem/test_pdo_eco_usih.py
 tests/dessem/test_pdo_eco_usih_polin.py
 tests/dessem/test_pdo_hidr.py
 tests/dessem/test_pdo_oper_uct.py
 tests/dessem/test_pdo_sist.py
 tests/dessem/test_polinjus.py
 tests/dessem/test_renovaveis.py
+tests/dessem/componentes/__init__.py
+tests/dessem/componentes/test_stagedatefield.py
 tests/mocks/__init__.py
 tests/mocks/mock_open.py
 tests/mocks/arquivos/__init__.py
 tests/mocks/arquivos/avl_altqueda.py
 tests/mocks/arquivos/avl_desvfpha.py
 tests/mocks/arquivos/avl_fpha1.py
 tests/mocks/arquivos/des_log_relato.py
```

### Comparing `idessem-0.0.7/setup.py` & `idessem-0.0.8/setup.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_avl_altqueda.py` & `idessem-0.0.8/tests/dessem/test_avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_avl_desvfpha.py` & `idessem-0.0.8/tests/dessem/test_avl_desvfpha.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_avl_fpha1.py` & `idessem-0.0.8/tests/dessem/test_avl_fpha1.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_des_log_relato.py` & `idessem-0.0.8/tests/dessem/test_des_log_relato.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_dessemarq.py` & `idessem-0.0.8/tests/dessem/test_dessemarq.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_hidr.py` & `idessem-0.0.8/tests/dessem/test_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_log_matriz.py` & `idessem-0.0.8/tests/dessem/test_log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_operut.py` & `idessem-0.0.8/tests/dessem/test_operut.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_pdo_eco_fcfcortes.py` & `idessem-0.0.8/tests/dessem/test_pdo_eco_fcfcortes.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_pdo_eco_usih.py` & `idessem-0.0.8/tests/dessem/test_pdo_eco_usih.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_pdo_eco_usih_polin.py` & `idessem-0.0.8/tests/dessem/test_pdo_eco_usih_polin.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_pdo_hidr.py` & `idessem-0.0.8/tests/dessem/test_pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_pdo_oper_uct.py` & `idessem-0.0.8/tests/dessem/test_pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_pdo_sist.py` & `idessem-0.0.8/tests/dessem/test_pdo_sist.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_polinjus.py` & `idessem-0.0.8/tests/dessem/test_polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/dessem/test_renovaveis.py` & `idessem-0.0.8/tests/dessem/test_renovaveis.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/arquivos/avl_altqueda.py` & `idessem-0.0.8/tests/mocks/arquivos/avl_altqueda.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/arquivos/avl_desvfpha.py` & `idessem-0.0.8/tests/mocks/arquivos/avl_desvfpha.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/arquivos/avl_fpha1.py` & `idessem-0.0.8/tests/mocks/arquivos/avl_fpha1.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/arquivos/des_log_relato.py` & `idessem-0.0.8/tests/mocks/arquivos/des_log_relato.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/arquivos/dessemarq.py` & `idessem-0.0.8/tests/mocks/arquivos/dessemarq.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/arquivos/log_matriz.py` & `idessem-0.0.8/tests/mocks/arquivos/log_matriz.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/arquivos/operut.py` & `idessem-0.0.8/tests/mocks/arquivos/operut.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/arquivos/pdo_eco_fcfcortes.py` & `idessem-0.0.8/tests/mocks/arquivos/pdo_eco_fcfcortes.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/arquivos/pdo_eco_usih.py` & `idessem-0.0.8/tests/mocks/arquivos/pdo_eco_usih.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/arquivos/pdo_eco_usih_polin.py` & `idessem-0.0.8/tests/mocks/arquivos/pdo_eco_usih_polin.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/arquivos/pdo_hidr.py` & `idessem-0.0.8/tests/mocks/arquivos/pdo_hidr.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/arquivos/pdo_oper_uct.py` & `idessem-0.0.8/tests/mocks/arquivos/pdo_oper_uct.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/arquivos/pdo_sist.py` & `idessem-0.0.8/tests/mocks/arquivos/pdo_sist.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/arquivos/polinjus.py` & `idessem-0.0.8/tests/mocks/arquivos/polinjus.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/arquivos/renovaveis.py` & `idessem-0.0.8/tests/mocks/arquivos/renovaveis.py`

 * *Files identical despite different names*

### Comparing `idessem-0.0.7/tests/mocks/mock_open.py` & `idessem-0.0.8/tests/mocks/mock_open.py`

 * *Files identical despite different names*

