# Comparing `tmp/cardtool-0.0.4.tar.gz` & `tmp/cardtool-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardtool-0.0.4.tar", last modified: Mon Jul 17 18:57:35 2023, max compression
+gzip compressed data, was "cardtool-0.0.5.tar", last modified: Tue Jul 18 21:31:35 2023, max compression
```

## Comparing `cardtool-0.0.4.tar` & `cardtool-0.0.5.tar`

### file list

```diff
@@ -1,118 +1,118 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.801725 cardtool-0.0.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.769725 cardtool-0.0.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.777725 cardtool-0.0.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-17 18:57:20.000000 cardtool-0.0.4/.github/workflows/publish-develop.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-17 18:57:20.000000 cardtool-0.0.4/.github/workflows/publish-master.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-17 18:57:20.000000 cardtool-0.0.4/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.781726 cardtool-0.0.4/.idea/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-17 18:57:20.000000 cardtool-0.0.4/.idea/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-17 18:57:20.000000 cardtool-0.0.4/.idea/cardtool.iml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.781726 cardtool-0.0.4/.idea/inspectionProfiles/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-17 18:57:20.000000 cardtool-0.0.4/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-17 18:57:20.000000 cardtool-0.0.4/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-17 18:57:20.000000 cardtool-0.0.4/.idea/jsonSchemas.xml
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-17 18:57:20.000000 cardtool-0.0.4/.idea/misc.xml
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-17 18:57:20.000000 cardtool-0.0.4/.idea/modules.xml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-17 18:57:20.000000 cardtool-0.0.4/.idea/vcs.xml
--rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-17 18:57:20.000000 cardtool-0.0.4/.idea/webResources.xml
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-17 18:57:20.000000 cardtool-0.0.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-17 18:57:20.000000 cardtool-0.0.4/.travis.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-17 18:57:20.000000 cardtool-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-17 18:57:20.000000 cardtool-0.0.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-17 18:57:35.801725 cardtool-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-17 18:57:20.000000 cardtool-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-17 18:57:20.000000 cardtool-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-17 18:57:20.000000 cardtool-0.0.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-17 18:57:35.801725 cardtool-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.769725 cardtool-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.781726 cardtool-0.0.4/src/cardtool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.785725 cardtool-0.0.4/src/cardtool/card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/card/bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      533 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/card/cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/card/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/card/dump.py
--rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/card/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/card/pin.py
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/card/tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.785725 cardtool-0.0.4/src/cardtool/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/command/gen_card.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/command/main_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/command/tr31_decrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.789725 cardtool-0.0.4/src/cardtool/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/config/card-config.json
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/config/load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.789725 cardtool-0.0.4/src/cardtool/dukpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/dukpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1776 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/dukpt/cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/dukpt/key.py
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/dukpt/key_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/dukpt/key_variant.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.789725 cardtool-0.0.4/src/cardtool/log/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/log/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.789725 cardtool-0.0.4/src/cardtool/tr31/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/tr31/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/tr31/decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/tr31/key_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.793725 cardtool-0.0.4/src/cardtool/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/util/common.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/util/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/util/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.793725 cardtool-0.0.4/src/cardtool/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/validation/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-17 18:57:20.000000 cardtool-0.0.4/src/cardtool/validation/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.785725 cardtool-0.0.4/src/cardtool.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-17 18:57:35.000000 cardtool-0.0.4/src/cardtool.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-17 18:57:35.000000 cardtool-0.0.4/src/cardtool.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 18:57:35.000000 cardtool-0.0.4/src/cardtool.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-17 18:57:35.000000 cardtool-0.0.4/src/cardtool.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-17 18:57:35.000000 cardtool-0.0.4/src/cardtool.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-17 18:57:35.000000 cardtool-0.0.4/src/cardtool.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.793725 cardtool-0.0.4/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.793725 cardtool-0.0.4/tests/cardtool/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.797726 cardtool-0.0.4/tests/cardtool/card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/card/test_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)      925 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/card/test_cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/card/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/card/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/card/test_pin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.797726 cardtool-0.0.4/tests/cardtool/command/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/command/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/command/test_gen_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/command/test_main_group.py
--rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/command/test_tr31_decrypt.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.797726 cardtool-0.0.4/tests/cardtool/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/config/test_load.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.797726 cardtool-0.0.4/tests/cardtool/dukpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/dukpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2852 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/dukpt/test_cipher.py
--rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/dukpt/test_key.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.797726 cardtool-0.0.4/tests/cardtool/tr31/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/tr31/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/tr31/test_decrypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/tr31/test_key_block.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.801725 cardtool-0.0.4/tests/cardtool/util/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/util/test_common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/util/test_serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.801725 cardtool-0.0.4/tests/cardtool/validation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/validation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/validation/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/cardtool/validation/test_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.801725 cardtool-0.0.4/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/data/bad-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/data/card-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:35.801725 cardtool-0.0.4/tests/helper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/helper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-17 18:57:20.000000 cardtool-0.0.4/tests/helper/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-17 18:57:20.000000 cardtool-0.0.4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.368526 cardtool-0.0.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.324527 cardtool-0.0.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.336526 cardtool-0.0.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-07-18 21:31:19.000000 cardtool-0.0.5/.github/workflows/publish-develop.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-07-18 21:31:19.000000 cardtool-0.0.5/.github/workflows/publish-master.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-07-18 21:31:19.000000 cardtool-0.0.5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.340526 cardtool-0.0.5/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-18 21:31:19.000000 cardtool-0.0.5/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-07-18 21:31:19.000000 cardtool-0.0.5/.idea/cardtool.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.340526 cardtool-0.0.5/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-07-18 21:31:19.000000 cardtool-0.0.5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-07-18 21:31:19.000000 cardtool-0.0.5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-18 21:31:19.000000 cardtool-0.0.5/.idea/jsonSchemas.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-07-18 21:31:19.000000 cardtool-0.0.5/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-07-18 21:31:19.000000 cardtool-0.0.5/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-07-18 21:31:19.000000 cardtool-0.0.5/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      379 2023-07-18 21:31:19.000000 cardtool-0.0.5/.idea/webResources.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-07-18 21:31:19.000000 cardtool-0.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-07-18 21:31:19.000000 cardtool-0.0.5/.travis.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-07-18 21:31:19.000000 cardtool-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-07-18 21:31:19.000000 cardtool-0.0.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-18 21:31:35.368526 cardtool-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-18 21:31:19.000000 cardtool-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-07-18 21:31:19.000000 cardtool-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1204 2023-07-18 21:31:19.000000 cardtool-0.0.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-07-18 21:31:35.372526 cardtool-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.324527 cardtool-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.340526 cardtool-0.0.5/src/cardtool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.348526 cardtool-0.0.5/src/cardtool/card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/card/bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/card/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/card/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1215 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/card/dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1853 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/card/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/card/pin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/card/tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.348526 cardtool-0.0.5/src/cardtool/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/command/gen_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/command/main_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1424 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/command/tr31_decrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.348526 cardtool-0.0.5/src/cardtool/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3022 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/config/card-config.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/config/load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.352526 cardtool-0.0.5/src/cardtool/dukpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/dukpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/dukpt/cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/dukpt/key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/dukpt/key_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/dukpt/key_variant.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.352526 cardtool-0.0.5/src/cardtool/log/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/log/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.356526 cardtool-0.0.5/src/cardtool/tr31/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/tr31/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3531 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/tr31/decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2502 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/tr31/key_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.356526 cardtool-0.0.5/src/cardtool/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/util/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/util/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/util/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.356526 cardtool-0.0.5/src/cardtool/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/validation/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-07-18 21:31:19.000000 cardtool-0.0.5/src/cardtool/validation/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.344526 cardtool-0.0.5/src/cardtool.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3290 2023-07-18 21:31:35.000000 cardtool-0.0.5/src/cardtool.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-07-18 21:31:35.000000 cardtool-0.0.5/src/cardtool.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 21:31:35.000000 cardtool-0.0.5/src/cardtool.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-07-18 21:31:35.000000 cardtool-0.0.5/src/cardtool.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-18 21:31:35.000000 cardtool-0.0.5/src/cardtool.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-07-18 21:31:35.000000 cardtool-0.0.5/src/cardtool.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.356526 cardtool-0.0.5/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.356526 cardtool-0.0.5/tests/cardtool/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.360526 cardtool-0.0.5/tests/cardtool/card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/card/test_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1045 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/card/test_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/card/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2463 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/card/test_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/card/test_pin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.360526 cardtool-0.0.5/tests/cardtool/command/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/command/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/command/test_gen_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/command/test_main_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3436 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/command/test_tr31_decrypt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.364526 cardtool-0.0.5/tests/cardtool/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2616 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/config/test_load.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.364526 cardtool-0.0.5/tests/cardtool/dukpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/dukpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/dukpt/test_cipher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2626 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/dukpt/test_key.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.364526 cardtool-0.0.5/tests/cardtool/tr31/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/tr31/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/tr31/test_decrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/tr31/test_key_block.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.368526 cardtool-0.0.5/tests/cardtool/util/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/util/test_common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/util/test_serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.368526 cardtool-0.0.5/tests/cardtool/validation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/validation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/validation/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/cardtool/validation/test_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.368526 cardtool-0.0.5/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/data/bad-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/data/card-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:35.368526 cardtool-0.0.5/tests/helper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/helper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-18 21:31:19.000000 cardtool-0.0.5/tests/helper/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      890 2023-07-18 21:31:19.000000 cardtool-0.0.5/tox.ini
```

### Comparing `cardtool-0.0.4/.github/workflows/publish-develop.yml` & `cardtool-0.0.5/.github/workflows/publish-develop.yml`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/.github/workflows/publish-master.yml` & `cardtool-0.0.5/.github/workflows/publish-master.yml`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/.gitignore` & `cardtool-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/.idea/cardtool.iml` & `cardtool-0.0.5/.idea/cardtool.iml`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/.idea/jsonSchemas.xml` & `cardtool-0.0.5/.idea/jsonSchemas.xml`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/.pre-commit-config.yaml` & `cardtool-0.0.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/.travis.yml` & `cardtool-0.0.5/.travis.yml`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/LICENSE` & `cardtool-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/Makefile` & `cardtool-0.0.5/Makefile`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/PKG-INFO` & `cardtool-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardtool
-Version: 0.0.4
+Version: 0.0.5
 Summary: An encrypted card generator tool
 Author: Daniel Aucatoma
 Keywords: DUKPT,credit,card,tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cardtool-0.0.4/README.md` & `cardtool-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/pyproject.toml` & `cardtool-0.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/requirements.txt` & `cardtool-0.0.5/requirements.txt`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/card/bootstrap.py` & `cardtool-0.0.5/src/cardtool/card/bootstrap.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/card/cipher.py` & `cardtool-0.0.5/src/cardtool/card/cipher.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 from cardtool.card.model import CardReadingData
 from cardtool.dukpt.cipher import Cipher
 from cardtool.dukpt.key_type import KeyType
 
+TRACK2_PAD = 0xFF
+DEFAULT_PAD = 0x00
+
 
 def encrypt_card(cipher: Cipher, card: CardReadingData) -> CardReadingData:
-    enc_tlv = cipher.encrypt(card.tlv, KeyType.DATA)
-    enc_track1 = cipher.encrypt(card.track1, KeyType.DATA)
-    enc_track2 = cipher.encrypt(card.track2, KeyType.DATA)
-    enc_pin_block = cipher.encrypt(card.pin_block, KeyType.PIN)
+    enc_tlv = cipher.encrypt(card.tlv, KeyType.DATA, DEFAULT_PAD)
+    enc_track1 = cipher.encrypt(card.track1, KeyType.DATA, DEFAULT_PAD)
+    enc_track2 = cipher.encrypt(card.track2, KeyType.DATA, TRACK2_PAD)
+    enc_pin_block = cipher.encrypt(card.pin_block, KeyType.PIN, DEFAULT_PAD)
     return CardReadingData(enc_tlv, enc_track1, enc_track2, enc_pin_block, card.label)
```

### Comparing `cardtool-0.0.4/src/cardtool/card/data.py` & `cardtool-0.0.5/src/cardtool/card/data.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/card/dump.py` & `cardtool-0.0.5/src/cardtool/card/dump.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/card/model.py` & `cardtool-0.0.5/src/cardtool/card/model.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/card/pin.py` & `cardtool-0.0.5/src/cardtool/card/pin.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/card/tags.py` & `cardtool-0.0.5/src/cardtool/card/tags.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/command/gen_card.py` & `cardtool-0.0.5/src/cardtool/command/gen_card.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/command/main_group.py` & `cardtool-0.0.5/src/cardtool/command/main_group.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/command/tr31_decrypt.py` & `cardtool-0.0.5/src/cardtool/command/tr31_decrypt.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/config/card-config.json` & `cardtool-0.0.5/src/cardtool/config/card-config.json`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/config/load.py` & `cardtool-0.0.5/src/cardtool/config/load.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/dukpt/cipher.py` & `cardtool-0.0.5/src/cardtool/dukpt/cipher.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,15 +5,17 @@
 from Crypto.Cipher import DES3
 
 from cardtool.dukpt.key_type import KeyType
 
 
 class Cipher(ABC):
     @abstractmethod
-    def encrypt(self, data: str, key: KeyType) -> str:  # pragma: no cover
+    def encrypt(
+        self, data: str, key: KeyType, pad: int = 0x00
+    ) -> str:  # pragma: no cover
         pass
 
     @abstractmethod
     def decrypt(self, data: str, key: KeyType) -> str:  # pragma: no cover
         pass
 
 
@@ -21,25 +23,25 @@
     def __init__(
         self, bdk: str, ksn: str, derive_key: Callable[[str, str, KeyType], str]
     ):
         self.__derive_key_ = derive_key
         self.__bdk_ = bdk
         self.__ksn_ = ksn
 
-    def encrypt(self, data: str, key: KeyType) -> str:
+    def encrypt(self, data: str, key: KeyType, pad: int = 0x00) -> str:
         key = self.__get_key_(key)
 
         encrypt = DES3.new(
             bytes.fromhex(key), DES3.MODE_CBC, IV=bytes.fromhex("0" * 16)
         )
         raw_data = bytes.fromhex(data)
         data_to_encrypt = (
             raw_data
             if (len(raw_data) % 8 == 0)
-            else DUKPTCipher.__append_bytes_(raw_data, 8 - (len(raw_data) % 8))
+            else DUKPTCipher.__append_bytes_(raw_data, 8 - (len(raw_data) % 8), pad)
         )
 
         encrypted = encrypt.encrypt(data_to_encrypt)
 
         return encrypted.hex().upper()
 
     def decrypt(self, data: str, key: KeyType) -> str:
@@ -50,16 +52,16 @@
         )
 
         encrypted = decrypt.decrypt(bytes.fromhex(data))
 
         return encrypted.hex().upper()
 
     @staticmethod
-    def __append_bytes_(data: bytes, n: int) -> bytes:
+    def __append_bytes_(data: bytes, n: int, pad: int) -> bytes:
         bt = bytearray(data)
-        [bt.append(0x00) for _ in range(n)]
+        [bt.append(pad) for _ in range(n)]
         return bytes(bt)
 
     @cache
     def __get_key_(self, key_type: KeyType) -> str:
         key = self.__derive_key_(self.__bdk_, self.__ksn_, key_type)
         return key
```

### Comparing `cardtool-0.0.4/src/cardtool/dukpt/key.py` & `cardtool-0.0.5/src/cardtool/dukpt/key.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/log/logger.py` & `cardtool-0.0.5/src/cardtool/log/logger.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/tr31/decrypt.py` & `cardtool-0.0.5/src/cardtool/tr31/decrypt.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/tr31/key_block.py` & `cardtool-0.0.5/src/cardtool/tr31/key_block.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/util/common.py` & `cardtool-0.0.5/src/cardtool/util/common.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/util/serialize.py` & `cardtool-0.0.5/src/cardtool/util/serialize.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/validation/command.py` & `cardtool-0.0.5/src/cardtool/validation/command.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool/validation/rules.py` & `cardtool-0.0.5/src/cardtool/validation/rules.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/src/cardtool.egg-info/PKG-INFO` & `cardtool-0.0.5/src/cardtool.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cardtool
-Version: 0.0.4
+Version: 0.0.5
 Summary: An encrypted card generator tool
 Author: Daniel Aucatoma
 Keywords: DUKPT,credit,card,tool
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
```

### Comparing `cardtool-0.0.4/src/cardtool.egg-info/SOURCES.txt` & `cardtool-0.0.5/src/cardtool.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/cardtool/card/test_cipher.py` & `cardtool-0.0.5/tests/cardtool/card/test_cipher.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,30 @@
 from dataclasses import asdict
 from unittest.mock import Mock, call
 
+import pydash
 from hamcrest import assert_that, equal_to
 
 from cardtool.card.cipher import encrypt_card
 from cardtool.card.model import CardReadingData
 from cardtool.dukpt.cipher import Cipher
 from cardtool.dukpt.key_type import KeyType
 
 
 def test_should_cipher_card_data_successfully_when_called():
     cipher = Mock(spec=Cipher)
     cipher.encrypt.return_value = "encrypt"
     card_data = CardReadingData("tlv", "track1", "track2", "pin", "test")
     encrypted_data = encrypt_card(cipher, card_data)
     expected_data = CardReadingData("encrypt", "encrypt", "encrypt", "encrypt", "test")
+    padding = {"track2": 0xFF}
 
     keys = [KeyType.DATA, KeyType.DATA, KeyType.DATA, KeyType.PIN]
     data_values = asdict(card_data).values()
 
     cipher.encrypt.assert_has_calls(
-        [call(data, key) for data, key in zip(data_values, keys)]
+        [
+            call(data, key, pydash.objects.get(padding, data, 0x00))
+            for data, key in zip(data_values, keys)
+        ]
     )
     assert_that(encrypted_data, equal_to(expected_data))
```

### Comparing `cardtool-0.0.4/tests/cardtool/card/test_data.py` & `cardtool-0.0.5/tests/cardtool/card/test_data.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/cardtool/card/test_dump.py` & `cardtool-0.0.5/tests/cardtool/card/test_dump.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/cardtool/card/test_pin.py` & `cardtool-0.0.5/tests/cardtool/card/test_pin.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/cardtool/command/test_gen_card.py` & `cardtool-0.0.5/tests/cardtool/command/test_gen_card.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/cardtool/command/test_main_group.py` & `cardtool-0.0.5/tests/cardtool/command/test_main_group.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/cardtool/command/test_tr31_decrypt.py` & `cardtool-0.0.5/tests/cardtool/command/test_tr31_decrypt.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/cardtool/config/test_load.py` & `cardtool-0.0.5/tests/cardtool/config/test_load.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/cardtool/dukpt/test_cipher.py` & `cardtool-0.0.5/tests/cardtool/dukpt/test_cipher.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,33 +1,43 @@
 from unittest.mock import Mock
 
+import pydash
 import pytest
 from hamcrest import assert_that, equal_to
 
 from cardtool.dukpt.cipher import DUKPTCipher
 from cardtool.dukpt.key_type import KeyType
 from helper.common import KSN, PLAINTEXT_KEY
 
 
 class TestDUKPTCipher:
     @pytest.mark.parametrize(
-        "data,expected",
+        "data,pad,expected",
         [
-            ("F" * 16, "1BFC569203335B41"),
-            ("F" * 18, "1BFC569203335B4156FA8D87902CF18F"),
+            (
+                "5477820000001234D2412201123400001230",
+                None,
+                "9076A0E140E525196648A60566D7A7D40276A2742A5C54E6",
+            ),
+            (
+                "5477820000001234D2412201123400001230",
+                0xFF,
+                "9076A0E140E525196648A60566D7A7D4D6A98F2875E99D15",
+            ),
         ],
         ids=["called with complete data", "called with data to be padded"],
     )
     def test_cipher_should_encrypt_data_successfully_when_(
-        self, data: str, expected: str
+        self, data: str, pad: int, expected: str
     ):
         derive_key = Mock()
         derive_key.return_value = "CA7091701C616F92697955B77E723D27"
         cipher = DUKPTCipher(PLAINTEXT_KEY, KSN, derive_key)
-        encrypted = cipher.encrypt(data, KeyType.DATA)
+        pad_byte = pydash.default_to(pad, 0x00)
+        encrypted = cipher.encrypt(data, KeyType.DATA, pad_byte)
 
         derive_key.assert_called_with(PLAINTEXT_KEY, KSN, KeyType.DATA)
         assert_that(encrypted, equal_to(expected))
 
     @pytest.mark.parametrize(
         "data,expected",
         [
```

### Comparing `cardtool-0.0.4/tests/cardtool/dukpt/test_key.py` & `cardtool-0.0.5/tests/cardtool/dukpt/test_key.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/cardtool/tr31/test_decrypt.py` & `cardtool-0.0.5/tests/cardtool/tr31/test_decrypt.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/cardtool/tr31/test_key_block.py` & `cardtool-0.0.5/tests/cardtool/tr31/test_key_block.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/cardtool/util/test_common.py` & `cardtool-0.0.5/tests/cardtool/util/test_common.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/cardtool/util/test_serialize.py` & `cardtool-0.0.5/tests/cardtool/util/test_serialize.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/cardtool/validation/test_command.py` & `cardtool-0.0.5/tests/cardtool/validation/test_command.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/cardtool/validation/test_rules.py` & `cardtool-0.0.5/tests/cardtool/validation/test_rules.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/conftest.py` & `cardtool-0.0.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tests/helper/common.py` & `cardtool-0.0.5/tests/helper/common.py`

 * *Files identical despite different names*

### Comparing `cardtool-0.0.4/tox.ini` & `cardtool-0.0.5/tox.ini`

 * *Files identical despite different names*

