# Comparing `tmp/ZODB-5.8.0.tar.gz` & `tmp/ZODB-5.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ZODB-5.8.0.tar", last modified: Wed Nov  9 11:37:51 2022, max compression
+gzip compressed data, was "ZODB-5.8.1.tar", last modified: Tue Jul 18 07:29:35 2023, max compression
```

## Comparing `ZODB-5.8.0.tar` & `ZODB-5.8.1.tar`

### file list

```diff
@@ -1,285 +1,285 @@
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.493431 ZODB-5.8.0/
--rw-r--r--   0 jens       (501) staff       (20)     1801 2021-11-02 08:52:39.000000 ZODB-5.8.0/3.11.txt
--rw-r--r--   0 jens       (501) staff       (20)    19729 2022-11-09 10:19:23.000000 ZODB-5.8.0/CHANGES.rst
--rw-r--r--   0 jens       (501) staff       (20)      804 2022-11-03 13:31:34.000000 ZODB-5.8.0/CONTRIBUTING.md
--rw-r--r--   0 jens       (501) staff       (20)       91 2021-11-02 08:52:39.000000 ZODB-5.8.0/COPYING
--rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:52:39.000000 ZODB-5.8.0/COPYRIGHT.txt
--rw-r--r--   0 jens       (501) staff       (20)     1621 2021-11-02 08:52:39.000000 ZODB-5.8.0/DEVELOPERS.rst
--rw-r--r--   0 jens       (501) staff       (20)   169467 2021-11-02 08:52:39.000000 ZODB-5.8.0/HISTORY.rst
--rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:52:39.000000 ZODB-5.8.0/LICENSE.txt
--rw-r--r--   0 jens       (501) staff       (20)      558 2022-11-03 13:31:34.000000 ZODB-5.8.0/MANIFEST.in
--rw-r--r--   0 jens       (501) staff       (20)    22864 2022-11-09 11:37:51.493553 ZODB-5.8.0/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     1636 2021-11-02 08:52:39.000000 ZODB-5.8.0/README.rst
--rw-r--r--   0 jens       (501) staff       (20)     1378 2021-11-02 08:52:39.000000 ZODB-5.8.0/buildout.cfg
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.452547 ZODB-5.8.0/docs/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.452684 ZODB-5.8.0/docs/.static/
--rw-r--r--   0 jens       (501) staff       (20)     1150 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/.static/zodb.ico
--rw-r--r--   0 jens       (501) staff       (20)       48 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/ConflictResolution.rst
--rw-r--r--   0 jens       (501) staff       (20)     2346 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/Makefile
--rw-r--r--   0 jens       (501) staff       (20)      498 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/README.rst
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.445401 ZODB-5.8.0/docs/_build/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.445951 ZODB-5.8.0/docs/_build/html/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.445491 ZODB-5.8.0/docs/_build/html/_downloads/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.452834 ZODB-5.8.0/docs/_build/html/_downloads/a852e204dabe563a61c6c5c3b217f268/
--rw-r--r--   0 jens       (501) staff       (20)     3568 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_downloads/a852e204dabe563a61c6c5c3b217f268/chatter.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.453064 ZODB-5.8.0/docs/_build/html/_images/
--rw-r--r--   0 jens       (501) staff       (20)    36863 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_images/zeo-diagram.png
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.455989 ZODB-5.8.0/docs/_build/html/_sources/
--rw-r--r--   0 jens       (501) staff       (20)       48 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/ConflictResolution.rst.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.457072 ZODB-5.8.0/docs/_build/html/_sources/articles/
--rw-r--r--   0 jens       (501) staff       (20)     7797 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/articles/ZODB-overview.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    14992 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/articles/ZODB1.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    14723 2022-11-09 08:17:08.000000 ZODB-5.8.0/docs/_build/html/_sources/articles/ZODB2.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      491 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/articles/index.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     7088 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/articles/multi-zodb-gc.rst.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.458975 ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/
--rw-r--r--   0 jens       (501) staff       (20)    18369 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/gfdl.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      513 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/index.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     8544 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/introduction.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      672 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/links.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    19400 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/modules.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    20905 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/prog-zodb.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     8300 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/transactions.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    10700 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/zeo.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)       57 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/changelog.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     6047 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/collaborations.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)       55 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/cross-database-references.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)       31 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/developers.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)      412 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/event.rst.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.459840 ZODB-5.8.0/docs/_build/html/_sources/guide/
--rw-r--r--   0 jens       (501) staff       (20)      563 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/guide/index.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     7965 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/guide/install-and-run.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    16034 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/guide/transactions-and-threading.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)    25148 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/guide/writing-persistent-objects.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)       53 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/historical_connections.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     3618 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/index.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     6867 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/introduction.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)       45 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/persistentclass.rst.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.460936 ZODB-5.8.0/docs/_build/html/_sources/reference/
--rw-r--r--   0 jens       (501) staff       (20)      139 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/reference/index.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     5763 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/reference/storages.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     1231 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/reference/transaction.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     3800 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/reference/zodb.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)     9052 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/tutorial.rst.txt
--rw-r--r--   0 jens       (501) staff       (20)       35 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_sources/utils.rst.txt
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.461986 ZODB-5.8.0/docs/_build/html/_static/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.446061 ZODB-5.8.0/docs/_build/html/_static/css/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.462218 ZODB-5.8.0/docs/_build/html/_static/css/fonts/
--rw-r--r--   0 jens       (501) staff       (20)   444379 2022-11-09 09:31:25.000000 ZODB-5.8.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
--rw-r--r--   0 jens       (501) staff       (20)      286 2022-11-09 09:31:25.000000 ZODB-5.8.0/docs/_build/html/_static/file.png
--rw-r--r--   0 jens       (501) staff       (20)       90 2022-11-09 09:31:25.000000 ZODB-5.8.0/docs/_build/html/_static/minus.png
--rw-r--r--   0 jens       (501) staff       (20)       90 2022-11-09 09:31:25.000000 ZODB-5.8.0/docs/_build/html/_static/plus.png
--rw-r--r--   0 jens       (501) staff       (20)     1150 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_static/zodb.ico
--rw-r--r--   0 jens       (501) staff       (20)     5020 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/_build/html/_static/zodb.png
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.463850 ZODB-5.8.0/docs/articles/
--rw-r--r--   0 jens       (501) staff       (20)     7797 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/ZODB-overview.rst
--rw-r--r--   0 jens       (501) staff       (20)    14992 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/ZODB1.rst
--rw-r--r--   0 jens       (501) staff       (20)    14723 2022-11-09 08:17:08.000000 ZODB-5.8.0/docs/articles/ZODB2.rst
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.463969 ZODB-5.8.0/docs/articles/images/
--rw-r--r--   0 jens       (501) staff       (20)    36863 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/images/zeo-diagram.png
--rw-r--r--   0 jens       (501) staff       (20)      491 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/index.rst
--rw-r--r--   0 jens       (501) staff       (20)     7088 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/multi-zodb-gc.rst
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.466058 ZODB-5.8.0/docs/articles/old-guide/
--rw-r--r--   0 jens       (501) staff       (20)      348 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/old-guide/README.txt
--rw-r--r--   0 jens       (501) staff       (20)      105 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/old-guide/TODO.txt
--rw-r--r--   0 jens       (501) staff       (20)     3568 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/old-guide/chatter.py
--rw-r--r--   0 jens       (501) staff       (20)      811 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/old-guide/convert_zodb_guide.py
--rw-r--r--   0 jens       (501) staff       (20)    18369 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/old-guide/gfdl.rst
--rw-r--r--   0 jens       (501) staff       (20)      513 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/old-guide/index.rst
--rw-r--r--   0 jens       (501) staff       (20)     8544 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/old-guide/introduction.rst
--rw-r--r--   0 jens       (501) staff       (20)      672 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/old-guide/links.rst
--rw-r--r--   0 jens       (501) staff       (20)    19400 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/old-guide/modules.rst
--rw-r--r--   0 jens       (501) staff       (20)    20905 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/old-guide/prog-zodb.rst
--rw-r--r--   0 jens       (501) staff       (20)     8300 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/old-guide/transactions.rst
--rw-r--r--   0 jens       (501) staff       (20)    10700 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/articles/old-guide/zeo.rst
--rw-r--r--   0 jens       (501) staff       (20)       57 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/changelog.rst
--rw-r--r--   0 jens       (501) staff       (20)     6047 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/collaborations.rst
--rw-r--r--   0 jens       (501) staff       (20)     6886 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/conf.py
--rw-r--r--   0 jens       (501) staff       (20)       55 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/cross-database-references.rst
--rw-r--r--   0 jens       (501) staff       (20)       31 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/developers.rst
--rw-r--r--   0 jens       (501) staff       (20)      412 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/event.rst
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.466620 ZODB-5.8.0/docs/guide/
--rw-r--r--   0 jens       (501) staff       (20)      563 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/guide/index.rst
--rw-r--r--   0 jens       (501) staff       (20)     7965 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/guide/install-and-run.rst
--rw-r--r--   0 jens       (501) staff       (20)    16034 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/guide/transactions-and-threading.rst
--rw-r--r--   0 jens       (501) staff       (20)    25148 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/guide/writing-persistent-objects.rst
--rw-r--r--   0 jens       (501) staff       (20)       53 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/historical_connections.rst
--rw-r--r--   0 jens       (501) staff       (20)     3618 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/index.rst
--rw-r--r--   0 jens       (501) staff       (20)     6867 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/introduction.rst
--rw-r--r--   0 jens       (501) staff       (20)       45 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/persistentclass.rst
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.467187 ZODB-5.8.0/docs/reference/
--rw-r--r--   0 jens       (501) staff       (20)      139 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/reference/index.rst
--rw-r--r--   0 jens       (501) staff       (20)     5763 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/reference/storages.rst
--rw-r--r--   0 jens       (501) staff       (20)     1231 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/reference/transaction.rst
--rw-r--r--   0 jens       (501) staff       (20)     3800 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/reference/zodb.rst
--rw-r--r--   0 jens       (501) staff       (20)      166 2022-03-17 08:03:17.000000 ZODB-5.8.0/docs/requirements.txt
--rw-r--r--   0 jens       (501) staff       (20)     9052 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/tutorial.rst
--rw-r--r--   0 jens       (501) staff       (20)       35 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/utils.rst
--rw-r--r--   0 jens       (501) staff       (20)     5020 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/zodb.png
--rw-r--r--   0 jens       (501) staff       (20)     1479 2022-03-16 13:46:04.000000 ZODB-5.8.0/docs/zodb.svg
--rw-r--r--   0 jens       (501) staff       (20)      687 2022-11-09 11:37:51.493872 ZODB-5.8.0/setup.cfg
--rw-r--r--   0 jens       (501) staff       (20)     3208 2022-11-09 10:19:42.000000 ZODB-5.8.0/setup.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.446555 ZODB-5.8.0/src/
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.473693 ZODB-5.8.0/src/ZODB/
--rw-r--r--   0 jens       (501) staff       (20)     3610 2022-03-16 13:46:04.000000 ZODB-5.8.0/src/ZODB/ActivityMonitor.py
--rw-r--r--   0 jens       (501) staff       (20)    13003 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/BaseStorage.py
--rw-r--r--   0 jens       (501) staff       (20)    11081 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/ConflictResolution.py
--rw-r--r--   0 jens       (501) staff       (20)    20243 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/ConflictResolution.rst
--rw-r--r--   0 jens       (501) staff       (20)    50905 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/Connection.py
--rw-r--r--   0 jens       (501) staff       (20)    40353 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/DB.py
--rw-r--r--   0 jens       (501) staff       (20)    16292 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/DemoStorage.py
--rw-r--r--   0 jens       (501) staff       (20)    12421 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/DemoStorage.test
--rw-r--r--   0 jens       (501) staff       (20)     7117 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/ExportImport.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.476668 ZODB-5.8.0/src/ZODB/FileStorage/
--rw-r--r--   0 jens       (501) staff       (20)    77753 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/FileStorage/FileStorage.py
--rw-r--r--   0 jens       (501) staff       (20)      358 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/FileStorage/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     9503 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/FileStorage/format.py
--rw-r--r--   0 jens       (501) staff       (20)     4950 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/FileStorage/fsdump.py
--rw-r--r--   0 jens       (501) staff       (20)     8265 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/FileStorage/fsoids.py
--rw-r--r--   0 jens       (501) staff       (20)    24592 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/FileStorage/fspack.py
--rw-r--r--   0 jens       (501) staff       (20)     2752 2022-03-16 13:46:04.000000 ZODB-5.8.0/src/ZODB/FileStorage/interfaces.py
--rw-r--r--   0 jens       (501) staff       (20)     5013 2022-06-14 06:12:01.000000 ZODB-5.8.0/src/ZODB/FileStorage/iterator.test
--rw-r--r--   0 jens       (501) staff       (20)     9315 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/FileStorage/tests.py
--rw-r--r--   0 jens       (501) staff       (20)     5561 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/FileStorage/zconfig.txt
--rw-r--r--   0 jens       (501) staff       (20)    11710 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/MappingStorage.py
--rw-r--r--   0 jens       (501) staff       (20)    11964 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/POSException.py
--rw-r--r--   0 jens       (501) staff       (20)     1548 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/UndoLogCompatible.py
--rw-r--r--   0 jens       (501) staff       (20)     1072 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     5293 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/_compat.py
--rw-r--r--   0 jens       (501) staff       (20)    36296 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/blob.py
--rw-r--r--   0 jens       (501) staff       (20)    10345 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/broken.py
--rw-r--r--   0 jens       (501) staff       (20)    13074 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/component.xml
--rw-r--r--   0 jens       (501) staff       (20)     9012 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/config.py
--rw-r--r--   0 jens       (501) staff       (20)      171 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/config.xml
--rw-r--r--   0 jens       (501) staff       (20)     1074 2022-03-16 13:46:04.000000 ZODB-5.8.0/src/ZODB/conversionhack.py
--rw-r--r--   0 jens       (501) staff       (20)     6278 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/cross-database-references.rst
--rw-r--r--   0 jens       (501) staff       (20)      729 2022-03-16 13:46:04.000000 ZODB-5.8.0/src/ZODB/event.py
--rw-r--r--   0 jens       (501) staff       (20)     8759 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/fsIndex.py
--rw-r--r--   0 jens       (501) staff       (20)    10435 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/fsrecover.py
--rw-r--r--   0 jens       (501) staff       (20)     4919 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/fstools.py
--rw-r--r--   0 jens       (501) staff       (20)    10449 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/historical_connections.rst
--rw-r--r--   0 jens       (501) staff       (20)    55001 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/interfaces.py
--rw-r--r--   0 jens       (501) staff       (20)     1777 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/loglevels.py
--rw-r--r--   0 jens       (501) staff       (20)     9669 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/mvccadapter.py
--rw-r--r--   0 jens       (501) staff       (20)     6690 2022-03-16 13:46:04.000000 ZODB-5.8.0/src/ZODB/persistentclass.py
--rw-r--r--   0 jens       (501) staff       (20)     7641 2022-03-17 08:24:21.000000 ZODB-5.8.0/src/ZODB/persistentclass.rst
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.479237 ZODB-5.8.0/src/ZODB/scripts/
--rw-r--r--   0 jens       (501) staff       (20)     3540 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/scripts/README.txt
--rw-r--r--   0 jens       (501) staff       (20)        2 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/scripts/__init__.py
--rwxr-xr-x   0 jens       (501) staff       (20)     4505 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/analyze.py
--rwxr-xr-x   0 jens       (501) staff       (20)     3223 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/checkbtrees.py
--rw-r--r--   0 jens       (501) staff       (20)     2390 2022-03-16 13:46:04.000000 ZODB-5.8.0/src/ZODB/scripts/fsoids.py
--rw-r--r--   0 jens       (501) staff       (20)     6915 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/fsrefs.py
--rwxr-xr-x   0 jens       (501) staff       (20)     6005 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/fsstats.py
--rwxr-xr-x   0 jens       (501) staff       (20)     1728 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/fstail.py
--rw-r--r--   0 jens       (501) staff       (20)     6865 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/fstest.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.479526 ZODB-5.8.0/src/ZODB/scripts/manual_tests/
--rw-r--r--   0 jens       (501) staff       (20)      802 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/scripts/manual_tests/test-checker.fs
--rw-r--r--   0 jens       (501) staff       (20)     5452 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/manual_tests/testfstest.py
--rwxr-xr-x   0 jens       (501) staff       (20)    11258 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/migrate.py
--rw-r--r--   0 jens       (501) staff       (20)     2784 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/migrateblobs.py
--rw-r--r--   0 jens       (501) staff       (20)     3474 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/netspace.py
--rw-r--r--   0 jens       (501) staff       (20)      991 2022-03-16 13:46:04.000000 ZODB-5.8.0/src/ZODB/scripts/referrers.py
--rwxr-xr-x   0 jens       (501) staff       (20)    28001 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/repozo.py
--rw-r--r--   0 jens       (501) staff       (20)     1680 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/space.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.480388 ZODB-5.8.0/src/ZODB/scripts/tests/
--rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/scripts/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     1260 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/scripts/tests/fstail.txt
--rw-r--r--   0 jens       (501) staff       (20)     1348 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/scripts/tests/referrers.txt
--rw-r--r--   0 jens       (501) staff       (20)     1895 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/tests/test_doc.py
--rw-r--r--   0 jens       (501) staff       (20)     2307 2022-03-16 13:46:04.000000 ZODB-5.8.0/src/ZODB/scripts/tests/test_fsdump_fsstats.py
--rw-r--r--   0 jens       (501) staff       (20)     1780 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/tests/test_fstest.py
--rw-r--r--   0 jens       (501) staff       (20)    51535 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/tests/test_repozo.py
--rwxr-xr-x   0 jens       (501) staff       (20)    32739 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/scripts/zodbload.py
--rw-r--r--   0 jens       (501) staff       (20)    24295 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/serialize.py
--rw-r--r--   0 jens       (501) staff       (20)      104 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/storage.xml
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.493210 ZODB-5.8.0/src/ZODB/tests/
--rw-r--r--   0 jens       (501) staff       (20)    14715 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/BasicStorage.py
--rw-r--r--   0 jens       (501) staff       (20)     5899 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/ConflictResolution.py
--rw-r--r--   0 jens       (501) staff       (20)     2345 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/Corruption.py
--rw-r--r--   0 jens       (501) staff       (20)     2132 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/HistoryStorage.py
--rw-r--r--   0 jens       (501) staff       (20)     3691 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/IExternalGC.test
--rw-r--r--   0 jens       (501) staff       (20)    10962 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/IteratorStorage.py
--rw-r--r--   0 jens       (501) staff       (20)     7382 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/MTStorage.py
--rw-r--r--   0 jens       (501) staff       (20)     4741 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/MVCCMappingStorage.py
--rw-r--r--   0 jens       (501) staff       (20)     1618 2022-03-16 13:46:04.000000 ZODB-5.8.0/src/ZODB/tests/MinPO.py
--rw-r--r--   0 jens       (501) staff       (20)    29330 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/PackableStorage.py
--rw-r--r--   0 jens       (501) staff       (20)     1807 2022-03-16 13:46:04.000000 ZODB-5.8.0/src/ZODB/tests/PersistentStorage.py
--rw-r--r--   0 jens       (501) staff       (20)     2248 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/ReadOnlyStorage.py
--rw-r--r--   0 jens       (501) staff       (20)     7910 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/RecoveryStorage.py
--rw-r--r--   0 jens       (501) staff       (20)     6905 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/RevisionStorage.py
--rw-r--r--   0 jens       (501) staff       (20)     6302 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/StorageTestBase.py
--rw-r--r--   0 jens       (501) staff       (20)     4379 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/Synchronization.py
--rw-r--r--   0 jens       (501) staff       (20)    28100 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/TransactionalUndoStorage.py
--rw-r--r--   0 jens       (501) staff       (20)       38 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/__init__.py
--rw-r--r--   0 jens       (501) staff       (20)     4814 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/blob_basic.txt
--rw-r--r--   0 jens       (501) staff       (20)     2777 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/blob_connection.txt
--rw-r--r--   0 jens       (501) staff       (20)     3797 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/blob_consume.txt
--rw-r--r--   0 jens       (501) staff       (20)     1986 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/blob_importexport.txt
--rw-r--r--   0 jens       (501) staff       (20)    10572 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/blob_layout.txt
--rw-r--r--   0 jens       (501) staff       (20)     3195 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/blob_packing.txt
--rw-r--r--   0 jens       (501) staff       (20)     1566 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/blob_tempdir.txt
--rw-r--r--   0 jens       (501) staff       (20)    11898 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/blob_transaction.txt
--rw-r--r--   0 jens       (501) staff       (20)     5292 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/blobstorage_packing.txt
--rw-r--r--   0 jens       (501) staff       (20)      475 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/component.xml
--rwxr-xr-x   0 jens       (501) staff       (20)     1811 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/dangle.py
--rw-r--r--   0 jens       (501) staff       (20)    10571 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/dbopen.txt
--rw-r--r--   0 jens       (501) staff       (20)      797 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/fix84.rst
--rw-r--r--   0 jens       (501) staff       (20)     5439 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/hexstorage.py
--rw-r--r--   0 jens       (501) staff       (20)     3555 2022-06-14 06:12:01.000000 ZODB-5.8.0/src/ZODB/tests/loggingsupport.py
--rw-r--r--   0 jens       (501) staff       (20)     5913 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/multidb.txt
--rw-r--r--   0 jens       (501) staff       (20)    17956 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/racetest.py
--rw-r--r--   0 jens       (501) staff       (20)    10698 2022-03-16 13:46:04.000000 ZODB-5.8.0/src/ZODB/tests/sampledm.py
--rw-r--r--   0 jens       (501) staff       (20)     3843 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/speed.py
--rw-r--r--   0 jens       (501) staff       (20)     2621 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/synchronizers.txt
--rw-r--r--   0 jens       (501) staff       (20)     3177 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testActivityMonitor.py
--rw-r--r--   0 jens       (501) staff       (20)     2660 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testBroken.py
--rw-r--r--   0 jens       (501) staff       (20)    18797 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testCache.py
--rw-r--r--   0 jens       (501) staff       (20)     5469 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testConfig.py
--rw-r--r--   0 jens       (501) staff       (20)    44671 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testConnection.py
--rw-r--r--   0 jens       (501) staff       (20)     6435 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testConnectionSavepoint.py
--rw-r--r--   0 jens       (501) staff       (20)     5272 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/testConnectionSavepoint.txt
--rw-r--r--   0 jens       (501) staff       (20)    15317 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testDB.py
--rw-r--r--   0 jens       (501) staff       (20)     8967 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testDemoStorage.py
--rw-r--r--   0 jens       (501) staff       (20)    27030 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testFileStorage.py
--rw-r--r--   0 jens       (501) staff       (20)     6728 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testMVCCMappingStorage.py
--rw-r--r--   0 jens       (501) staff       (20)     3157 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testMappingStorage.py
--rw-r--r--   0 jens       (501) staff       (20)     6039 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testPersistentList.py
--rw-r--r--   0 jens       (501) staff       (20)     5099 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testPersistentMapping.py
--rw-r--r--   0 jens       (501) staff       (20)     7446 2022-03-16 13:46:04.000000 ZODB-5.8.0/src/ZODB/tests/testPersistentWeakref.py
--rw-r--r--   0 jens       (501) staff       (20)     7901 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testRecover.py
--rw-r--r--   0 jens       (501) staff       (20)     8870 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testSerialize.py
--rw-r--r--   0 jens       (501) staff       (20)     1825 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/testThreadedShutdown.py
--rw-r--r--   0 jens       (501) staff       (20)     6239 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testUtils.py
--rw-r--r--   0 jens       (501) staff       (20)    16839 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testZODB.py
--rw-r--r--   0 jens       (501) staff       (20)     4849 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/test_TransactionMetaData.py
--rw-r--r--   0 jens       (501) staff       (20)     7135 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/test_cache.py
--rw-r--r--   0 jens       (501) staff       (20)     1809 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/test_doctest_files.py
--rw-r--r--   0 jens       (501) staff       (20)     3011 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/test_fsdump.py
--rw-r--r--   0 jens       (501) staff       (20)     1718 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/tests/test_mvccadapter.py
--rw-r--r--   0 jens       (501) staff       (20)     1653 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/test_prefetch.py
--rw-r--r--   0 jens       (501) staff       (20)     4942 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/test_storage.py
--rw-r--r--   0 jens       (501) staff       (20)    25678 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testblob.py
--rw-r--r--   0 jens       (501) staff       (20)    12057 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testconflictresolution.py
--rw-r--r--   0 jens       (501) staff       (20)     5821 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testcrossdatabasereferences.py
--rw-r--r--   0 jens       (501) staff       (20)     1716 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testdocumentation.py
--rw-r--r--   0 jens       (501) staff       (20)     6981 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testfsIndex.py
--rw-r--r--   0 jens       (501) staff       (20)     7060 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testfsoids.py
--rw-r--r--   0 jens       (501) staff       (20)     1002 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testhistoricalconnections.py
--rw-r--r--   0 jens       (501) staff       (20)    13153 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testmvcc.py
--rw-r--r--   0 jens       (501) staff       (20)     2618 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/testpersistentclass.py
--rw-r--r--   0 jens       (501) staff       (20)    13113 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/tests/util.py
--rw-r--r--   0 jens       (501) staff       (20)     2123 2022-03-16 13:46:04.000000 ZODB-5.8.0/src/ZODB/tests/warnhook.py
--rw-r--r--   0 jens       (501) staff       (20)     2194 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/transact.py
--rw-r--r--   0 jens       (501) staff       (20)    11923 2022-11-09 08:17:08.000000 ZODB-5.8.0/src/ZODB/utils.py
--rw-r--r--   0 jens       (501) staff       (20)     5967 2021-11-02 08:52:39.000000 ZODB-5.8.0/src/ZODB/utils.rst
--rw-r--r--   0 jens       (501) staff       (20)      336 2022-03-16 13:46:04.000000 ZODB-5.8.0/src/ZODB/valuedoc.py
-drwxr-xr-x   0 jens       (501) staff       (20)        0 2022-11-09 11:37:51.474790 ZODB-5.8.0/src/ZODB.egg-info/
--rw-r--r--   0 jens       (501) staff       (20)    22864 2022-11-09 11:37:51.000000 ZODB-5.8.0/src/ZODB.egg-info/PKG-INFO
--rw-r--r--   0 jens       (501) staff       (20)     8236 2022-11-09 11:37:51.000000 ZODB-5.8.0/src/ZODB.egg-info/SOURCES.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2022-11-09 11:37:51.000000 ZODB-5.8.0/src/ZODB.egg-info/dependency_links.txt
--rw-r--r--   0 jens       (501) staff       (20)      192 2022-11-09 11:37:51.000000 ZODB-5.8.0/src/ZODB.egg-info/entry_points.txt
--rw-r--r--   0 jens       (501) staff       (20)        1 2022-03-17 07:57:32.000000 ZODB-5.8.0/src/ZODB.egg-info/not-zip-safe
--rw-r--r--   0 jens       (501) staff       (20)      275 2022-11-09 11:37:51.000000 ZODB-5.8.0/src/ZODB.egg-info/requires.txt
--rw-r--r--   0 jens       (501) staff       (20)        5 2022-11-09 11:37:51.000000 ZODB-5.8.0/src/ZODB.egg-info/top_level.txt
--rw-r--r--   0 jens       (501) staff       (20)     1735 2022-11-09 08:17:08.000000 ZODB-5.8.0/tox.ini
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.791643 ZODB-5.8.1/
+-rw-r--r--   0 jens       (501) staff       (20)     1801 2021-11-02 08:52:39.000000 ZODB-5.8.1/3.11.txt
+-rw-r--r--   0 jens       (501) staff       (20)    20019 2023-07-18 06:59:19.000000 ZODB-5.8.1/CHANGES.rst
+-rw-r--r--   0 jens       (501) staff       (20)      804 2022-11-03 13:31:34.000000 ZODB-5.8.1/CONTRIBUTING.md
+-rw-r--r--   0 jens       (501) staff       (20)       91 2021-11-02 08:52:39.000000 ZODB-5.8.1/COPYING
+-rw-r--r--   0 jens       (501) staff       (20)       32 2021-11-02 08:52:39.000000 ZODB-5.8.1/COPYRIGHT.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1621 2021-11-02 08:52:39.000000 ZODB-5.8.1/DEVELOPERS.rst
+-rw-r--r--   0 jens       (501) staff       (20)   169467 2021-11-02 08:52:39.000000 ZODB-5.8.1/HISTORY.rst
+-rw-r--r--   0 jens       (501) staff       (20)     2070 2021-11-02 08:52:39.000000 ZODB-5.8.1/LICENSE.txt
+-rw-r--r--   0 jens       (501) staff       (20)      558 2022-11-03 13:31:34.000000 ZODB-5.8.1/MANIFEST.in
+-rw-r--r--   0 jens       (501) staff       (20)    23196 2023-07-18 07:29:35.791757 ZODB-5.8.1/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     1678 2023-04-14 10:27:25.000000 ZODB-5.8.1/README.rst
+-rw-r--r--   0 jens       (501) staff       (20)     1378 2021-11-02 08:52:39.000000 ZODB-5.8.1/buildout.cfg
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.754123 ZODB-5.8.1/docs/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.754262 ZODB-5.8.1/docs/.static/
+-rw-r--r--   0 jens       (501) staff       (20)     1150 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/.static/zodb.ico
+-rw-r--r--   0 jens       (501) staff       (20)       48 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/ConflictResolution.rst
+-rw-r--r--   0 jens       (501) staff       (20)     2346 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/Makefile
+-rw-r--r--   0 jens       (501) staff       (20)      498 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/README.rst
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.747825 ZODB-5.8.1/docs/_build/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.748313 ZODB-5.8.1/docs/_build/html/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.747915 ZODB-5.8.1/docs/_build/html/_downloads/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.754414 ZODB-5.8.1/docs/_build/html/_downloads/a852e204dabe563a61c6c5c3b217f268/
+-rw-r--r--   0 jens       (501) staff       (20)     3568 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_downloads/a852e204dabe563a61c6c5c3b217f268/chatter.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.754640 ZODB-5.8.1/docs/_build/html/_images/
+-rw-r--r--   0 jens       (501) staff       (20)    36863 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_images/zeo-diagram.png
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.757171 ZODB-5.8.1/docs/_build/html/_sources/
+-rw-r--r--   0 jens       (501) staff       (20)       48 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/ConflictResolution.rst.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.758174 ZODB-5.8.1/docs/_build/html/_sources/articles/
+-rw-r--r--   0 jens       (501) staff       (20)     7797 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/articles/ZODB-overview.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    14992 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/articles/ZODB1.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    14723 2022-11-09 08:17:08.000000 ZODB-5.8.1/docs/_build/html/_sources/articles/ZODB2.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      491 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/articles/index.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     7088 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/articles/multi-zodb-gc.rst.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.760005 ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/
+-rw-r--r--   0 jens       (501) staff       (20)    18369 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/gfdl.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      513 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/index.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     8544 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/introduction.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      672 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/links.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    19400 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/modules.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    20905 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/prog-zodb.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     8300 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/transactions.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    10700 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/zeo.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)       57 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/changelog.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     6047 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/collaborations.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)       55 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/cross-database-references.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)       31 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/developers.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)      412 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/event.rst.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.760856 ZODB-5.8.1/docs/_build/html/_sources/guide/
+-rw-r--r--   0 jens       (501) staff       (20)      563 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/guide/index.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     7965 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/guide/install-and-run.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    16034 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/guide/transactions-and-threading.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)    25148 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/guide/writing-persistent-objects.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)       53 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/historical_connections.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     3618 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/index.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     6867 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/introduction.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)       45 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/persistentclass.rst.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.761839 ZODB-5.8.1/docs/_build/html/_sources/reference/
+-rw-r--r--   0 jens       (501) staff       (20)      139 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/reference/index.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     5763 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/reference/storages.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1231 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/reference/transaction.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     3800 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/reference/zodb.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)     9052 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/tutorial.rst.txt
+-rw-r--r--   0 jens       (501) staff       (20)       35 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_sources/utils.rst.txt
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.762674 ZODB-5.8.1/docs/_build/html/_static/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.748412 ZODB-5.8.1/docs/_build/html/_static/css/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.762903 ZODB-5.8.1/docs/_build/html/_static/css/fonts/
+-rw-r--r--   0 jens       (501) staff       (20)   444379 2022-11-09 09:31:25.000000 ZODB-5.8.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg
+-rw-r--r--   0 jens       (501) staff       (20)      286 2022-11-09 09:31:25.000000 ZODB-5.8.1/docs/_build/html/_static/file.png
+-rw-r--r--   0 jens       (501) staff       (20)       90 2022-11-09 09:31:25.000000 ZODB-5.8.1/docs/_build/html/_static/minus.png
+-rw-r--r--   0 jens       (501) staff       (20)       90 2022-11-09 09:31:25.000000 ZODB-5.8.1/docs/_build/html/_static/plus.png
+-rw-r--r--   0 jens       (501) staff       (20)     1150 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_static/zodb.ico
+-rw-r--r--   0 jens       (501) staff       (20)     5020 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/_build/html/_static/zodb.png
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.764492 ZODB-5.8.1/docs/articles/
+-rw-r--r--   0 jens       (501) staff       (20)     7797 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/ZODB-overview.rst
+-rw-r--r--   0 jens       (501) staff       (20)    14992 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/ZODB1.rst
+-rw-r--r--   0 jens       (501) staff       (20)    14723 2022-11-09 08:17:08.000000 ZODB-5.8.1/docs/articles/ZODB2.rst
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.764615 ZODB-5.8.1/docs/articles/images/
+-rw-r--r--   0 jens       (501) staff       (20)    36863 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/images/zeo-diagram.png
+-rw-r--r--   0 jens       (501) staff       (20)      491 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)     7088 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/multi-zodb-gc.rst
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.766466 ZODB-5.8.1/docs/articles/old-guide/
+-rw-r--r--   0 jens       (501) staff       (20)      348 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/old-guide/README.txt
+-rw-r--r--   0 jens       (501) staff       (20)      105 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/old-guide/TODO.txt
+-rw-r--r--   0 jens       (501) staff       (20)     3568 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/old-guide/chatter.py
+-rw-r--r--   0 jens       (501) staff       (20)      811 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/old-guide/convert_zodb_guide.py
+-rw-r--r--   0 jens       (501) staff       (20)    18369 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/old-guide/gfdl.rst
+-rw-r--r--   0 jens       (501) staff       (20)      513 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/old-guide/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)     8544 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/old-guide/introduction.rst
+-rw-r--r--   0 jens       (501) staff       (20)      672 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/old-guide/links.rst
+-rw-r--r--   0 jens       (501) staff       (20)    19400 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/old-guide/modules.rst
+-rw-r--r--   0 jens       (501) staff       (20)    20905 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/old-guide/prog-zodb.rst
+-rw-r--r--   0 jens       (501) staff       (20)     8300 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/old-guide/transactions.rst
+-rw-r--r--   0 jens       (501) staff       (20)    10700 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/articles/old-guide/zeo.rst
+-rw-r--r--   0 jens       (501) staff       (20)       57 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/changelog.rst
+-rw-r--r--   0 jens       (501) staff       (20)     6047 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/collaborations.rst
+-rw-r--r--   0 jens       (501) staff       (20)     6886 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/conf.py
+-rw-r--r--   0 jens       (501) staff       (20)       55 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/cross-database-references.rst
+-rw-r--r--   0 jens       (501) staff       (20)       31 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/developers.rst
+-rw-r--r--   0 jens       (501) staff       (20)      412 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/event.rst
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.766963 ZODB-5.8.1/docs/guide/
+-rw-r--r--   0 jens       (501) staff       (20)      563 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/guide/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)     7965 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/guide/install-and-run.rst
+-rw-r--r--   0 jens       (501) staff       (20)    16034 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/guide/transactions-and-threading.rst
+-rw-r--r--   0 jens       (501) staff       (20)    25148 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/guide/writing-persistent-objects.rst
+-rw-r--r--   0 jens       (501) staff       (20)       53 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/historical_connections.rst
+-rw-r--r--   0 jens       (501) staff       (20)     3618 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)     6867 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/introduction.rst
+-rw-r--r--   0 jens       (501) staff       (20)       45 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/persistentclass.rst
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.767490 ZODB-5.8.1/docs/reference/
+-rw-r--r--   0 jens       (501) staff       (20)      139 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/reference/index.rst
+-rw-r--r--   0 jens       (501) staff       (20)     5763 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/reference/storages.rst
+-rw-r--r--   0 jens       (501) staff       (20)     1231 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/reference/transaction.rst
+-rw-r--r--   0 jens       (501) staff       (20)     3800 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/reference/zodb.rst
+-rw-r--r--   0 jens       (501) staff       (20)      166 2022-03-17 08:03:17.000000 ZODB-5.8.1/docs/requirements.txt
+-rw-r--r--   0 jens       (501) staff       (20)     8718 2023-07-18 06:56:15.000000 ZODB-5.8.1/docs/tutorial.rst
+-rw-r--r--   0 jens       (501) staff       (20)       35 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/utils.rst
+-rw-r--r--   0 jens       (501) staff       (20)     5020 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/zodb.png
+-rw-r--r--   0 jens       (501) staff       (20)     1479 2022-03-16 13:46:04.000000 ZODB-5.8.1/docs/zodb.svg
+-rw-r--r--   0 jens       (501) staff       (20)      687 2023-07-18 07:29:35.792075 ZODB-5.8.1/setup.cfg
+-rw-r--r--   0 jens       (501) staff       (20)     3208 2023-07-18 06:56:46.000000 ZODB-5.8.1/setup.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.748839 ZODB-5.8.1/src/
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.773493 ZODB-5.8.1/src/ZODB/
+-rw-r--r--   0 jens       (501) staff       (20)     3610 2022-03-16 13:46:04.000000 ZODB-5.8.1/src/ZODB/ActivityMonitor.py
+-rw-r--r--   0 jens       (501) staff       (20)    13003 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/BaseStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)    11081 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/ConflictResolution.py
+-rw-r--r--   0 jens       (501) staff       (20)    20243 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/ConflictResolution.rst
+-rw-r--r--   0 jens       (501) staff       (20)    50580 2023-07-18 06:56:15.000000 ZODB-5.8.1/src/ZODB/Connection.py
+-rw-r--r--   0 jens       (501) staff       (20)    40353 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/DB.py
+-rw-r--r--   0 jens       (501) staff       (20)    16292 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/DemoStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)    12421 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/DemoStorage.test
+-rw-r--r--   0 jens       (501) staff       (20)     7117 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/ExportImport.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.776239 ZODB-5.8.1/src/ZODB/FileStorage/
+-rw-r--r--   0 jens       (501) staff       (20)    77753 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/FileStorage/FileStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)      358 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/FileStorage/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     9503 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/FileStorage/format.py
+-rw-r--r--   0 jens       (501) staff       (20)     4950 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/FileStorage/fsdump.py
+-rw-r--r--   0 jens       (501) staff       (20)     8265 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/FileStorage/fsoids.py
+-rw-r--r--   0 jens       (501) staff       (20)    24592 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/FileStorage/fspack.py
+-rw-r--r--   0 jens       (501) staff       (20)     2752 2022-03-16 13:46:04.000000 ZODB-5.8.1/src/ZODB/FileStorage/interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)     5013 2022-06-14 06:12:01.000000 ZODB-5.8.1/src/ZODB/FileStorage/iterator.test
+-rw-r--r--   0 jens       (501) staff       (20)     9315 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/FileStorage/tests.py
+-rw-r--r--   0 jens       (501) staff       (20)     5561 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/FileStorage/zconfig.txt
+-rw-r--r--   0 jens       (501) staff       (20)    11710 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/MappingStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)    11964 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/POSException.py
+-rw-r--r--   0 jens       (501) staff       (20)     1548 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/UndoLogCompatible.py
+-rw-r--r--   0 jens       (501) staff       (20)     1072 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     5293 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/_compat.py
+-rw-r--r--   0 jens       (501) staff       (20)    36296 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/blob.py
+-rw-r--r--   0 jens       (501) staff       (20)    10345 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/broken.py
+-rw-r--r--   0 jens       (501) staff       (20)    13074 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/component.xml
+-rw-r--r--   0 jens       (501) staff       (20)     9012 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/config.py
+-rw-r--r--   0 jens       (501) staff       (20)      171 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/config.xml
+-rw-r--r--   0 jens       (501) staff       (20)     1074 2022-03-16 13:46:04.000000 ZODB-5.8.1/src/ZODB/conversionhack.py
+-rw-r--r--   0 jens       (501) staff       (20)     6370 2023-07-18 06:56:15.000000 ZODB-5.8.1/src/ZODB/cross-database-references.rst
+-rw-r--r--   0 jens       (501) staff       (20)      729 2022-03-16 13:46:04.000000 ZODB-5.8.1/src/ZODB/event.py
+-rw-r--r--   0 jens       (501) staff       (20)     8759 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/fsIndex.py
+-rw-r--r--   0 jens       (501) staff       (20)    10435 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/fsrecover.py
+-rw-r--r--   0 jens       (501) staff       (20)     4919 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/fstools.py
+-rw-r--r--   0 jens       (501) staff       (20)    10449 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/historical_connections.rst
+-rw-r--r--   0 jens       (501) staff       (20)    55001 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/interfaces.py
+-rw-r--r--   0 jens       (501) staff       (20)     1777 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/loglevels.py
+-rw-r--r--   0 jens       (501) staff       (20)     9669 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/mvccadapter.py
+-rw-r--r--   0 jens       (501) staff       (20)     6690 2022-03-16 13:46:04.000000 ZODB-5.8.1/src/ZODB/persistentclass.py
+-rw-r--r--   0 jens       (501) staff       (20)     7641 2022-03-17 08:24:21.000000 ZODB-5.8.1/src/ZODB/persistentclass.rst
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.778277 ZODB-5.8.1/src/ZODB/scripts/
+-rw-r--r--   0 jens       (501) staff       (20)     3540 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/scripts/README.txt
+-rw-r--r--   0 jens       (501) staff       (20)        2 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/scripts/__init__.py
+-rwxr-xr-x   0 jens       (501) staff       (20)     4505 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/scripts/analyze.py
+-rwxr-xr-x   0 jens       (501) staff       (20)     3223 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/scripts/checkbtrees.py
+-rw-r--r--   0 jens       (501) staff       (20)     2390 2022-03-16 13:46:04.000000 ZODB-5.8.1/src/ZODB/scripts/fsoids.py
+-rw-r--r--   0 jens       (501) staff       (20)     6915 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/scripts/fsrefs.py
+-rwxr-xr-x   0 jens       (501) staff       (20)     6005 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/scripts/fsstats.py
+-rwxr-xr-x   0 jens       (501) staff       (20)     1728 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/scripts/fstail.py
+-rw-r--r--   0 jens       (501) staff       (20)     6865 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/scripts/fstest.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.778727 ZODB-5.8.1/src/ZODB/scripts/manual_tests/
+-rw-r--r--   0 jens       (501) staff       (20)      802 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/scripts/manual_tests/test-checker.fs
+-rw-r--r--   0 jens       (501) staff       (20)     5452 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/scripts/manual_tests/testfstest.py
+-rwxr-xr-x   0 jens       (501) staff       (20)    11258 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/scripts/migrate.py
+-rw-r--r--   0 jens       (501) staff       (20)     2784 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/scripts/migrateblobs.py
+-rw-r--r--   0 jens       (501) staff       (20)     3474 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/scripts/netspace.py
+-rw-r--r--   0 jens       (501) staff       (20)      991 2022-03-16 13:46:04.000000 ZODB-5.8.1/src/ZODB/scripts/referrers.py
+-rwxr-xr-x   0 jens       (501) staff       (20)    27989 2023-07-18 06:56:15.000000 ZODB-5.8.1/src/ZODB/scripts/repozo.py
+-rw-r--r--   0 jens       (501) staff       (20)     1680 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/scripts/space.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.779724 ZODB-5.8.1/src/ZODB/scripts/tests/
+-rw-r--r--   0 jens       (501) staff       (20)        0 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/scripts/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     1260 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/scripts/tests/fstail.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1348 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/scripts/tests/referrers.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1895 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/scripts/tests/test_doc.py
+-rw-r--r--   0 jens       (501) staff       (20)     2307 2022-03-16 13:46:04.000000 ZODB-5.8.1/src/ZODB/scripts/tests/test_fsdump_fsstats.py
+-rw-r--r--   0 jens       (501) staff       (20)     1780 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/scripts/tests/test_fstest.py
+-rw-r--r--   0 jens       (501) staff       (20)    51535 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/scripts/tests/test_repozo.py
+-rwxr-xr-x   0 jens       (501) staff       (20)    32753 2023-04-14 10:27:25.000000 ZODB-5.8.1/src/ZODB/scripts/zodbload.py
+-rw-r--r--   0 jens       (501) staff       (20)    24295 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/serialize.py
+-rw-r--r--   0 jens       (501) staff       (20)      104 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/storage.xml
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.791481 ZODB-5.8.1/src/ZODB/tests/
+-rw-r--r--   0 jens       (501) staff       (20)    14715 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/BasicStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)     5899 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/ConflictResolution.py
+-rw-r--r--   0 jens       (501) staff       (20)     2345 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/Corruption.py
+-rw-r--r--   0 jens       (501) staff       (20)     2132 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/HistoryStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)     3691 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/IExternalGC.test
+-rw-r--r--   0 jens       (501) staff       (20)    10962 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/IteratorStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)     7382 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/MTStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)     4741 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/MVCCMappingStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)     1618 2022-03-16 13:46:04.000000 ZODB-5.8.1/src/ZODB/tests/MinPO.py
+-rw-r--r--   0 jens       (501) staff       (20)    29330 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/PackableStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)     1807 2022-03-16 13:46:04.000000 ZODB-5.8.1/src/ZODB/tests/PersistentStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)     2248 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/ReadOnlyStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)     7910 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/RecoveryStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)     6905 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/RevisionStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)     6302 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/StorageTestBase.py
+-rw-r--r--   0 jens       (501) staff       (20)     4379 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/Synchronization.py
+-rw-r--r--   0 jens       (501) staff       (20)    28100 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/TransactionalUndoStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)       38 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/__init__.py
+-rw-r--r--   0 jens       (501) staff       (20)     4814 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/blob_basic.txt
+-rw-r--r--   0 jens       (501) staff       (20)     2777 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/blob_connection.txt
+-rw-r--r--   0 jens       (501) staff       (20)     3797 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/blob_consume.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1986 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/blob_importexport.txt
+-rw-r--r--   0 jens       (501) staff       (20)    10572 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/blob_layout.txt
+-rw-r--r--   0 jens       (501) staff       (20)     3195 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/blob_packing.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1566 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/blob_tempdir.txt
+-rw-r--r--   0 jens       (501) staff       (20)    11898 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/blob_transaction.txt
+-rw-r--r--   0 jens       (501) staff       (20)     5292 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/blobstorage_packing.txt
+-rw-r--r--   0 jens       (501) staff       (20)      475 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/component.xml
+-rwxr-xr-x   0 jens       (501) staff       (20)     1811 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/dangle.py
+-rw-r--r--   0 jens       (501) staff       (20)    10571 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/dbopen.txt
+-rw-r--r--   0 jens       (501) staff       (20)      797 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/fix84.rst
+-rw-r--r--   0 jens       (501) staff       (20)     5439 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/hexstorage.py
+-rw-r--r--   0 jens       (501) staff       (20)     3555 2022-06-14 06:12:01.000000 ZODB-5.8.1/src/ZODB/tests/loggingsupport.py
+-rw-r--r--   0 jens       (501) staff       (20)     5982 2023-07-18 06:56:15.000000 ZODB-5.8.1/src/ZODB/tests/multidb.txt
+-rw-r--r--   0 jens       (501) staff       (20)    21700 2023-04-20 08:25:48.000000 ZODB-5.8.1/src/ZODB/tests/racetest.py
+-rw-r--r--   0 jens       (501) staff       (20)    10698 2022-03-16 13:46:04.000000 ZODB-5.8.1/src/ZODB/tests/sampledm.py
+-rw-r--r--   0 jens       (501) staff       (20)     3843 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/speed.py
+-rw-r--r--   0 jens       (501) staff       (20)     2621 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/synchronizers.txt
+-rw-r--r--   0 jens       (501) staff       (20)     3177 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testActivityMonitor.py
+-rw-r--r--   0 jens       (501) staff       (20)     2660 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testBroken.py
+-rw-r--r--   0 jens       (501) staff       (20)    18797 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testCache.py
+-rw-r--r--   0 jens       (501) staff       (20)     5469 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testConfig.py
+-rw-r--r--   0 jens       (501) staff       (20)    44671 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testConnection.py
+-rw-r--r--   0 jens       (501) staff       (20)     6435 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testConnectionSavepoint.py
+-rw-r--r--   0 jens       (501) staff       (20)     5272 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/testConnectionSavepoint.txt
+-rw-r--r--   0 jens       (501) staff       (20)    15317 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testDB.py
+-rw-r--r--   0 jens       (501) staff       (20)     8967 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testDemoStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)    27030 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testFileStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)     6728 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testMVCCMappingStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)     3157 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testMappingStorage.py
+-rw-r--r--   0 jens       (501) staff       (20)     6039 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testPersistentList.py
+-rw-r--r--   0 jens       (501) staff       (20)     5099 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testPersistentMapping.py
+-rw-r--r--   0 jens       (501) staff       (20)     7446 2022-03-16 13:46:04.000000 ZODB-5.8.1/src/ZODB/tests/testPersistentWeakref.py
+-rw-r--r--   0 jens       (501) staff       (20)     7901 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testRecover.py
+-rw-r--r--   0 jens       (501) staff       (20)     8870 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testSerialize.py
+-rw-r--r--   0 jens       (501) staff       (20)     1825 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/testThreadedShutdown.py
+-rw-r--r--   0 jens       (501) staff       (20)     6239 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testUtils.py
+-rw-r--r--   0 jens       (501) staff       (20)    16839 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testZODB.py
+-rw-r--r--   0 jens       (501) staff       (20)     4849 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/test_TransactionMetaData.py
+-rw-r--r--   0 jens       (501) staff       (20)     7135 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/test_cache.py
+-rw-r--r--   0 jens       (501) staff       (20)     1809 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/test_doctest_files.py
+-rw-r--r--   0 jens       (501) staff       (20)     3011 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/test_fsdump.py
+-rw-r--r--   0 jens       (501) staff       (20)     1718 2021-11-02 08:52:39.000000 ZODB-5.8.1/src/ZODB/tests/test_mvccadapter.py
+-rw-r--r--   0 jens       (501) staff       (20)     1653 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/test_prefetch.py
+-rw-r--r--   0 jens       (501) staff       (20)     3560 2023-04-20 08:25:48.000000 ZODB-5.8.1/src/ZODB/tests/test_racetest.py
+-rw-r--r--   0 jens       (501) staff       (20)     4942 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/test_storage.py
+-rw-r--r--   0 jens       (501) staff       (20)    25678 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testblob.py
+-rw-r--r--   0 jens       (501) staff       (20)    12057 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testconflictresolution.py
+-rw-r--r--   0 jens       (501) staff       (20)     5867 2023-07-18 06:56:15.000000 ZODB-5.8.1/src/ZODB/tests/testcrossdatabasereferences.py
+-rw-r--r--   0 jens       (501) staff       (20)     1716 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testdocumentation.py
+-rw-r--r--   0 jens       (501) staff       (20)     6981 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testfsIndex.py
+-rw-r--r--   0 jens       (501) staff       (20)     7060 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testfsoids.py
+-rw-r--r--   0 jens       (501) staff       (20)     1002 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testhistoricalconnections.py
+-rw-r--r--   0 jens       (501) staff       (20)    13153 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testmvcc.py
+-rw-r--r--   0 jens       (501) staff       (20)     2618 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/testpersistentclass.py
+-rw-r--r--   0 jens       (501) staff       (20)    13113 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/tests/util.py
+-rw-r--r--   0 jens       (501) staff       (20)     2194 2022-11-09 08:17:08.000000 ZODB-5.8.1/src/ZODB/transact.py
+-rw-r--r--   0 jens       (501) staff       (20)    11155 2023-07-18 06:56:15.000000 ZODB-5.8.1/src/ZODB/utils.py
+-rw-r--r--   0 jens       (501) staff       (20)     5969 2023-04-14 10:27:25.000000 ZODB-5.8.1/src/ZODB/utils.rst
+-rw-r--r--   0 jens       (501) staff       (20)      336 2022-03-16 13:46:04.000000 ZODB-5.8.1/src/ZODB/valuedoc.py
+drwxr-xr-x   0 jens       (501) staff       (20)        0 2023-07-18 07:29:35.774550 ZODB-5.8.1/src/ZODB.egg-info/
+-rw-r--r--   0 jens       (501) staff       (20)    23196 2023-07-18 07:29:35.000000 ZODB-5.8.1/src/ZODB.egg-info/PKG-INFO
+-rw-r--r--   0 jens       (501) staff       (20)     8241 2023-07-18 07:29:35.000000 ZODB-5.8.1/src/ZODB.egg-info/SOURCES.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2023-07-18 07:29:35.000000 ZODB-5.8.1/src/ZODB.egg-info/dependency_links.txt
+-rw-r--r--   0 jens       (501) staff       (20)      192 2023-07-18 07:29:35.000000 ZODB-5.8.1/src/ZODB.egg-info/entry_points.txt
+-rw-r--r--   0 jens       (501) staff       (20)        1 2022-03-17 07:57:32.000000 ZODB-5.8.1/src/ZODB.egg-info/not-zip-safe
+-rw-r--r--   0 jens       (501) staff       (20)      275 2023-07-18 07:29:35.000000 ZODB-5.8.1/src/ZODB.egg-info/requires.txt
+-rw-r--r--   0 jens       (501) staff       (20)        5 2023-07-18 07:29:35.000000 ZODB-5.8.1/src/ZODB.egg-info/top_level.txt
+-rw-r--r--   0 jens       (501) staff       (20)     1735 2022-11-09 08:17:08.000000 ZODB-5.8.1/tox.ini
```

### Comparing `ZODB-5.8.0/3.11.txt` & `ZODB-5.8.1/3.11.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/CHANGES.rst` & `ZODB-5.8.1/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,21 @@
 ================
  Change History
 ================
 
+5.8.1 (2023-07-18)
+==================
+
+- Fix ``racetest`` problems.
+  For details see `#376 <https://github.com/zopefoundation/ZODB/pull/376>`_.
+
+- Fix ``--with-verify`` argument in script repozo ``--recover``.
+  For details see `#381 <https://github.com/zopefoundation/ZODB/pull/381>`_.
+
+
 5.8.0 (2022-11-09)
 ==================
 
 - Add support for Python 3.11.
 
 - Expand and refactor tests for race conditions.
```

### Comparing `ZODB-5.8.0/CONTRIBUTING.md` & `ZODB-5.8.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/DEVELOPERS.rst` & `ZODB-5.8.1/DEVELOPERS.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/HISTORY.rst` & `ZODB-5.8.1/HISTORY.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/LICENSE.txt` & `ZODB-5.8.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/MANIFEST.in` & `ZODB-5.8.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/PKG-INFO` & `ZODB-5.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZODB
-Version: 5.8.0
+Version: 5.8.1
 Summary: ZODB, a Python object-oriented database
 Home-page: http://zodb-docs.readthedocs.io
 Author: Jim Fulton
 Author-email: jim@zope.com
 Maintainer: Zope Foundation and Contributors
 Maintainer-email: zodb-dev@zope.org
 License: ZPL 2.1
@@ -44,16 +44,16 @@
    :target: https://pypi.org/project/ZODB/
    :alt: Latest release
 
 .. image:: https://img.shields.io/pypi/pyversions/ZODB.svg
    :target: https://pypi.org/project/ZODB/
    :alt: Supported Python versions
 
-.. image:: https://travis-ci.com/zopefoundation/ZODB.svg?branch=master
-   :target: https://travis-ci.com/zopefoundation/ZODB
+.. image:: https://github.com/zopefoundation/ZODB/actions/workflows/tests.yml/badge.svg
+   :target: https://github.com/zopefoundation/ZODB/actions/workflows/tests.yml
    :alt: Build status
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/ZODB/badge.svg
    :target: https://coveralls.io/github/zopefoundation/ZODB
    :alt: Coverage status
 
 .. image:: https://readthedocs.org/projects/zodb-docs/badge/?version=latest
@@ -86,14 +86,24 @@
 <https://github.com/zopefoundation/ZODB/blob/master/DEVELOPERS.rst>`_.
 
 
 ================
  Change History
 ================
 
+5.8.1 (2023-07-18)
+==================
+
+- Fix ``racetest`` problems.
+  For details see `#376 <https://github.com/zopefoundation/ZODB/pull/376>`_.
+
+- Fix ``--with-verify`` argument in script repozo ``--recover``.
+  For details see `#381 <https://github.com/zopefoundation/ZODB/pull/381>`_.
+
+
 5.8.0 (2022-11-09)
 ==================
 
 - Add support for Python 3.11.
 
 - Expand and refactor tests for race conditions.
```

### Comparing `ZODB-5.8.0/README.rst` & `ZODB-5.8.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -6,16 +6,16 @@
    :target: https://pypi.org/project/ZODB/
    :alt: Latest release
 
 .. image:: https://img.shields.io/pypi/pyversions/ZODB.svg
    :target: https://pypi.org/project/ZODB/
    :alt: Supported Python versions
 
-.. image:: https://travis-ci.com/zopefoundation/ZODB.svg?branch=master
-   :target: https://travis-ci.com/zopefoundation/ZODB
+.. image:: https://github.com/zopefoundation/ZODB/actions/workflows/tests.yml/badge.svg
+   :target: https://github.com/zopefoundation/ZODB/actions/workflows/tests.yml
    :alt: Build status
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/ZODB/badge.svg
    :target: https://coveralls.io/github/zopefoundation/ZODB
    :alt: Coverage status
 
 .. image:: https://readthedocs.org/projects/zodb-docs/badge/?version=latest
```

### Comparing `ZODB-5.8.0/buildout.cfg` & `ZODB-5.8.1/buildout.cfg`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/.static/zodb.ico` & `ZODB-5.8.1/docs/.static/zodb.ico`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/Makefile` & `ZODB-5.8.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_downloads/a852e204dabe563a61c6c5c3b217f268/chatter.py` & `ZODB-5.8.1/docs/_build/html/_downloads/a852e204dabe563a61c6c5c3b217f268/chatter.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_images/zeo-diagram.png` & `ZODB-5.8.1/docs/_build/html/_images/zeo-diagram.png`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/articles/ZODB-overview.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/articles/ZODB-overview.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/articles/ZODB1.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/articles/ZODB1.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/articles/ZODB2.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/articles/ZODB2.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/articles/multi-zodb-gc.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/articles/multi-zodb-gc.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/gfdl.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/gfdl.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/index.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/index.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/introduction.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/introduction.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/links.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/links.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/modules.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/modules.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/prog-zodb.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/prog-zodb.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/transactions.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/transactions.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/articles/old-guide/zeo.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/articles/old-guide/zeo.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/collaborations.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/collaborations.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/guide/index.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/guide/index.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/guide/install-and-run.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/guide/install-and-run.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/guide/transactions-and-threading.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/guide/transactions-and-threading.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/guide/writing-persistent-objects.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/guide/writing-persistent-objects.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/index.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/index.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/introduction.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/introduction.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/reference/storages.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/reference/storages.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/reference/transaction.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/reference/transaction.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/reference/zodb.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/reference/zodb.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_sources/tutorial.rst.txt` & `ZODB-5.8.1/docs/_build/html/_sources/tutorial.rst.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg` & `ZODB-5.8.1/docs/_build/html/_static/css/fonts/fontawesome-webfont.svg`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_static/zodb.ico` & `ZODB-5.8.1/docs/_build/html/_static/zodb.ico`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/_build/html/_static/zodb.png` & `ZODB-5.8.1/docs/_build/html/_static/zodb.png`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/articles/ZODB-overview.rst` & `ZODB-5.8.1/docs/articles/ZODB-overview.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/articles/ZODB1.rst` & `ZODB-5.8.1/docs/articles/ZODB1.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/articles/ZODB2.rst` & `ZODB-5.8.1/docs/articles/ZODB2.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/articles/images/zeo-diagram.png` & `ZODB-5.8.1/docs/articles/images/zeo-diagram.png`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/articles/multi-zodb-gc.rst` & `ZODB-5.8.1/docs/articles/multi-zodb-gc.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/articles/old-guide/chatter.py` & `ZODB-5.8.1/docs/articles/old-guide/chatter.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/articles/old-guide/convert_zodb_guide.py` & `ZODB-5.8.1/docs/articles/old-guide/convert_zodb_guide.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/articles/old-guide/gfdl.rst` & `ZODB-5.8.1/docs/articles/old-guide/gfdl.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/articles/old-guide/index.rst` & `ZODB-5.8.1/docs/articles/old-guide/index.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/articles/old-guide/introduction.rst` & `ZODB-5.8.1/docs/articles/old-guide/introduction.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/articles/old-guide/links.rst` & `ZODB-5.8.1/docs/articles/old-guide/links.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/articles/old-guide/modules.rst` & `ZODB-5.8.1/docs/articles/old-guide/modules.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/articles/old-guide/prog-zodb.rst` & `ZODB-5.8.1/docs/articles/old-guide/prog-zodb.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/articles/old-guide/transactions.rst` & `ZODB-5.8.1/docs/articles/old-guide/transactions.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/articles/old-guide/zeo.rst` & `ZODB-5.8.1/docs/articles/old-guide/zeo.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/collaborations.rst` & `ZODB-5.8.1/docs/collaborations.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/conf.py` & `ZODB-5.8.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/guide/index.rst` & `ZODB-5.8.1/docs/guide/index.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/guide/install-and-run.rst` & `ZODB-5.8.1/docs/guide/install-and-run.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/guide/transactions-and-threading.rst` & `ZODB-5.8.1/docs/guide/transactions-and-threading.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/guide/writing-persistent-objects.rst` & `ZODB-5.8.1/docs/guide/writing-persistent-objects.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/index.rst` & `ZODB-5.8.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/introduction.rst` & `ZODB-5.8.1/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/reference/storages.rst` & `ZODB-5.8.1/docs/reference/storages.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/reference/transaction.rst` & `ZODB-5.8.1/docs/reference/transaction.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/reference/zodb.rst` & `ZODB-5.8.1/docs/reference/zodb.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/tutorial.rst` & `ZODB-5.8.1/docs/tutorial.rst`

 * *Files 4% similar despite different names*

```diff
@@ -162,18 +162,15 @@
 objects in ZODB is by traversing (accessing attributes or items, or
 calling methods) other objects.  Object traversal is typically much
 faster than search.
 
 You can use BTrees to build indexes for efficient search, when
 necessary.  If your application is search centric, or if you prefer to
 approach data access that way, then ZODB might not be the best
-technology for you. Before you turn your back on the ZODB, it
-may be worth checking out the up-and-coming Newt DB [#newtdb]_ project, 
-which combines the ZODB with Postgresql for indexing, search and access 
-from non-Python applications.
+technology for you.
 
 Transactions
 ============
 
 You now have objects in your root object and in your database.
 However, they are not permanently stored yet. The ZODB uses
 transactions and to make your changes permanent, you have to commit
@@ -244,10 +241,7 @@
    previously committed can't be rolled back because there's no
    previous state to roll back to.
 
 .. [#eviction]
    Objects aren't actually evicted, but their state is released, so
    they take up much less memory and any objects they referenced can
    be removed from memory.
-
-.. [#newtdb]
-   Here is an overview of the Newt DB architecture: http://www.newtdb.org/en/latest/how-it-works.html
```

### Comparing `ZODB-5.8.0/docs/zodb.png` & `ZODB-5.8.1/docs/zodb.png`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/docs/zodb.svg` & `ZODB-5.8.1/docs/zodb.svg`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/setup.cfg` & `ZODB-5.8.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/setup.py` & `ZODB-5.8.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # FOR A PARTICULAR PURPOSE.
 #
 ##############################################################################
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = '5.8.0'
+version = '5.8.1'
 
 classifiers = """\
 Intended Audience :: Developers
 License :: OSI Approved :: Zope Public License
 Programming Language :: Python
 Programming Language :: Python :: 2
 Programming Language :: Python :: 2.7
```

### Comparing `ZODB-5.8.0/src/ZODB/ActivityMonitor.py` & `ZODB-5.8.1/src/ZODB/ActivityMonitor.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/BaseStorage.py` & `ZODB-5.8.1/src/ZODB/BaseStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/ConflictResolution.py` & `ZODB-5.8.1/src/ZODB/ConflictResolution.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/ConflictResolution.rst` & `ZODB-5.8.1/src/ZODB/ConflictResolution.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/Connection.py` & `ZODB-5.8.1/src/ZODB/Connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,14 @@
 from ZODB.POSException import ReadConflictError
 from ZODB.POSException import ReadOnlyHistoryError
 from ZODB.POSException import Unsupported
 from ZODB.serialize import ObjectReader
 from ZODB.serialize import ObjectWriter
 from ZODB.utils import oid_repr
 from ZODB.utils import p64
-from ZODB.utils import positive_id
 from ZODB.utils import u64
 from ZODB.utils import z64
 
 from . import valuedoc
 from ._compat import _protocol
 from ._compat import dumps
 from ._compat import loads
@@ -944,23 +943,14 @@
             if c._storage is not None:
                 c._storage.release()
             c._storage = c._normal_storage = None
             c._cache = PickleCache(self, 0, 0)
             c.close(False)
 
     ##########################################################################
-    # Python protocol
-
-    def __repr__(self):
-        return '<Connection at %08x>' % (positive_id(self),)
-
-    # Python protocol
-    ##########################################################################
-
-    ##########################################################################
     # DEPRECATION candidates
 
     __getitem__ = get
 
     def exchange(self, old, new):
         # called by a ZClasses method that isn't executed by the test suite
         oid = old._p_oid
```

### Comparing `ZODB-5.8.0/src/ZODB/DB.py` & `ZODB-5.8.1/src/ZODB/DB.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/DemoStorage.py` & `ZODB-5.8.1/src/ZODB/DemoStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/DemoStorage.test` & `ZODB-5.8.1/src/ZODB/DemoStorage.test`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/ExportImport.py` & `ZODB-5.8.1/src/ZODB/ExportImport.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/FileStorage/FileStorage.py` & `ZODB-5.8.1/src/ZODB/FileStorage/FileStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/FileStorage/format.py` & `ZODB-5.8.1/src/ZODB/FileStorage/format.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/FileStorage/fsdump.py` & `ZODB-5.8.1/src/ZODB/FileStorage/fsdump.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/FileStorage/fsoids.py` & `ZODB-5.8.1/src/ZODB/FileStorage/fsoids.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/FileStorage/fspack.py` & `ZODB-5.8.1/src/ZODB/FileStorage/fspack.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/FileStorage/interfaces.py` & `ZODB-5.8.1/src/ZODB/FileStorage/interfaces.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/FileStorage/iterator.test` & `ZODB-5.8.1/src/ZODB/FileStorage/iterator.test`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/FileStorage/tests.py` & `ZODB-5.8.1/src/ZODB/FileStorage/tests.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/FileStorage/zconfig.txt` & `ZODB-5.8.1/src/ZODB/FileStorage/zconfig.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/MappingStorage.py` & `ZODB-5.8.1/src/ZODB/MappingStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/POSException.py` & `ZODB-5.8.1/src/ZODB/POSException.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/UndoLogCompatible.py` & `ZODB-5.8.1/src/ZODB/UndoLogCompatible.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/__init__.py` & `ZODB-5.8.1/src/ZODB/__init__.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/_compat.py` & `ZODB-5.8.1/src/ZODB/_compat.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/blob.py` & `ZODB-5.8.1/src/ZODB/blob.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/broken.py` & `ZODB-5.8.1/src/ZODB/broken.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/component.xml` & `ZODB-5.8.1/src/ZODB/component.xml`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/config.py` & `ZODB-5.8.1/src/ZODB/config.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/conversionhack.py` & `ZODB-5.8.1/src/ZODB/conversionhack.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/cross-database-references.rst` & `ZODB-5.8.1/src/ZODB/cross-database-references.rst`

 * *Files 4% similar despite different names*

```diff
@@ -59,15 +59,15 @@
 
     >>> p2.p3 = p3
     >>> tm.commit() # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
     Traceback (most recent call last):
     ...
     InvalidObjectReference:
       ('Attempt to store an object from a foreign database connection',
-       <Connection at ...>,
+       <ZODB.Connection.Connection object at ...>,
        <ZODB.tests.testcrossdatabasereferences.MyClass...>)
 
     >>> tm.abort()
 
 Databases for new objects
 =========================
 
@@ -88,15 +88,15 @@
 
     >>> tm.commit() # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
     Traceback (most recent call last):
     ...
     InvalidObjectReference:
     ("A new object is reachable from multiple databases. Won't try to
     guess which one was correct!",
-    <Connection at ...>,
+    <ZODB.Connection.Connection object at ...>,
     <ZODB.tests.testcrossdatabasereferences.MyClass...>)
 
     >>> tm.abort()
 
 To resolve this ambiguity, we can commit before an object becomes
 reachable from multiple databases.
 
@@ -116,15 +116,15 @@
     >>> p2.p5 = p5
     >>> tm.commit() # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
     Traceback (most recent call last):
     ...
     InvalidObjectReference:
     ("A new object is reachable from multiple databases. Won't try to guess
     which one was correct!",
-    <Connection at ...>,
+    <ZODB.Connection.Connection object at ...>,
     <ZODB.tests.testcrossdatabasereferences.MyClass...>)
 
     >>> tm.abort()
 
 (Maybe it should.)
 
 We can disambiguate this situation by using the connection add method
@@ -163,15 +163,15 @@
     >>> transaction.commit()
     >>> c2.root.x = c1.root()
     >>> transaction.commit() # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
     Traceback (most recent call last):
     ...
     InvalidObjectReference:
     ("Database '2' doesn't allow implicit cross-database references",
-    <Connection at ...>,
+    <ZODB.Connection.Connection object at ...>,
     {'x': {}})
 
     >>> transaction.abort()
 
 NOTE
 ====
```

### Comparing `ZODB-5.8.0/src/ZODB/event.py` & `ZODB-5.8.1/src/ZODB/event.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/fsIndex.py` & `ZODB-5.8.1/src/ZODB/fsIndex.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/fsrecover.py` & `ZODB-5.8.1/src/ZODB/fsrecover.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/fstools.py` & `ZODB-5.8.1/src/ZODB/fstools.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/historical_connections.rst` & `ZODB-5.8.1/src/ZODB/historical_connections.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/interfaces.py` & `ZODB-5.8.1/src/ZODB/interfaces.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/loglevels.py` & `ZODB-5.8.1/src/ZODB/loglevels.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/mvccadapter.py` & `ZODB-5.8.1/src/ZODB/mvccadapter.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/persistentclass.py` & `ZODB-5.8.1/src/ZODB/persistentclass.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/persistentclass.rst` & `ZODB-5.8.1/src/ZODB/persistentclass.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/README.txt` & `ZODB-5.8.1/src/ZODB/scripts/README.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/analyze.py` & `ZODB-5.8.1/src/ZODB/scripts/analyze.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/checkbtrees.py` & `ZODB-5.8.1/src/ZODB/scripts/checkbtrees.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/fsoids.py` & `ZODB-5.8.1/src/ZODB/scripts/fsoids.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/fsrefs.py` & `ZODB-5.8.1/src/ZODB/scripts/fsrefs.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/fsstats.py` & `ZODB-5.8.1/src/ZODB/scripts/fsstats.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/fstail.py` & `ZODB-5.8.1/src/ZODB/scripts/fstail.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/fstest.py` & `ZODB-5.8.1/src/ZODB/scripts/fstest.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/manual_tests/test-checker.fs` & `ZODB-5.8.1/src/ZODB/scripts/manual_tests/test-checker.fs`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/manual_tests/testfstest.py` & `ZODB-5.8.1/src/ZODB/scripts/manual_tests/testfstest.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/migrate.py` & `ZODB-5.8.1/src/ZODB/scripts/migrate.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/migrateblobs.py` & `ZODB-5.8.1/src/ZODB/scripts/migrateblobs.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/netspace.py` & `ZODB-5.8.1/src/ZODB/scripts/netspace.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/referrers.py` & `ZODB-5.8.1/src/ZODB/scripts/referrers.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/repozo.py` & `ZODB-5.8.1/src/ZODB/scripts/repozo.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
         Write recovered ZODB to given file.  By default, the file is
         written to stdout.
 
         Note:  for the stdout case, the index file will **not** be restored
         automatically.
 
     -w
-    --with-verification
+    --with-verify
         Verify on the fly the backup files on recovering. This option runs
         the same checks as when repozo is run in -V/--verify mode, and
         allows to verify and recover a backup in one single step. If a sanity
         check fails, the partially recovered ZODB will be left in place.
 
 Options for -V/--verify:
     -Q / --quick
@@ -175,15 +175,15 @@
                                     'file=',
                                     'full',
                                     'quick',
                                     'gzip',
                                     'kill-old-on-full',
                                     'date=',
                                     'output=',
-                                    'with-verification',
+                                    'with-verify',
                                     ])
     except getopt.error as msg:
         usage(1, msg)
 
     class Options(object):
         mode = None         # BACKUP, RECOVER or VERIFY
         file = None         # name of input Data.fs file
```

### Comparing `ZODB-5.8.0/src/ZODB/scripts/space.py` & `ZODB-5.8.1/src/ZODB/scripts/space.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/tests/fstail.txt` & `ZODB-5.8.1/src/ZODB/scripts/tests/fstail.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/tests/referrers.txt` & `ZODB-5.8.1/src/ZODB/scripts/tests/referrers.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/tests/test_doc.py` & `ZODB-5.8.1/src/ZODB/scripts/tests/test_doc.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/tests/test_fsdump_fsstats.py` & `ZODB-5.8.1/src/ZODB/scripts/tests/test_fsdump_fsstats.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/tests/test_fstest.py` & `ZODB-5.8.1/src/ZODB/scripts/tests/test_fstest.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/tests/test_repozo.py` & `ZODB-5.8.1/src/ZODB/scripts/tests/test_repozo.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/scripts/zodbload.py` & `ZODB-5.8.1/src/ZODB/scripts/zodbload.py`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
 
     try:
         with open('/proc/%s/status' % os.getpid()) as f:
             lines = f.readlines()
     except:  # noqa: E722 do not use bare 'except'
         return 0
     else:
-        l_ = list(filter(lambda l: l[:7] == 'VmSize:', lines))
+        l_ = list(filter(lambda l: l[:7] == 'VmSize:', lines))  # noqa: E741
         if l_:
             l_ = l_[0][7:].strip().split()[0]
             return int(l_)
     return 0
 
 
 def setup(lib_python):
```

### Comparing `ZODB-5.8.0/src/ZODB/serialize.py` & `ZODB-5.8.1/src/ZODB/serialize.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/BasicStorage.py` & `ZODB-5.8.1/src/ZODB/tests/BasicStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/ConflictResolution.py` & `ZODB-5.8.1/src/ZODB/tests/ConflictResolution.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/Corruption.py` & `ZODB-5.8.1/src/ZODB/tests/Corruption.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/HistoryStorage.py` & `ZODB-5.8.1/src/ZODB/tests/HistoryStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/IExternalGC.test` & `ZODB-5.8.1/src/ZODB/tests/IExternalGC.test`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/IteratorStorage.py` & `ZODB-5.8.1/src/ZODB/tests/IteratorStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/MTStorage.py` & `ZODB-5.8.1/src/ZODB/tests/MTStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/MVCCMappingStorage.py` & `ZODB-5.8.1/src/ZODB/tests/MVCCMappingStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/MinPO.py` & `ZODB-5.8.1/src/ZODB/tests/MinPO.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/PackableStorage.py` & `ZODB-5.8.1/src/ZODB/tests/PackableStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/PersistentStorage.py` & `ZODB-5.8.1/src/ZODB/tests/PersistentStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/ReadOnlyStorage.py` & `ZODB-5.8.1/src/ZODB/tests/ReadOnlyStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/RecoveryStorage.py` & `ZODB-5.8.1/src/ZODB/tests/RecoveryStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/RevisionStorage.py` & `ZODB-5.8.1/src/ZODB/tests/RevisionStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/StorageTestBase.py` & `ZODB-5.8.1/src/ZODB/tests/StorageTestBase.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/Synchronization.py` & `ZODB-5.8.1/src/ZODB/tests/Synchronization.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/TransactionalUndoStorage.py` & `ZODB-5.8.1/src/ZODB/tests/TransactionalUndoStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/blob_basic.txt` & `ZODB-5.8.1/src/ZODB/tests/blob_basic.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/blob_connection.txt` & `ZODB-5.8.1/src/ZODB/tests/blob_connection.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/blob_consume.txt` & `ZODB-5.8.1/src/ZODB/tests/blob_consume.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/blob_importexport.txt` & `ZODB-5.8.1/src/ZODB/tests/blob_importexport.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/blob_layout.txt` & `ZODB-5.8.1/src/ZODB/tests/blob_layout.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/blob_packing.txt` & `ZODB-5.8.1/src/ZODB/tests/blob_packing.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/blob_tempdir.txt` & `ZODB-5.8.1/src/ZODB/tests/blob_tempdir.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/blob_transaction.txt` & `ZODB-5.8.1/src/ZODB/tests/blob_transaction.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/blobstorage_packing.txt` & `ZODB-5.8.1/src/ZODB/tests/blobstorage_packing.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/dangle.py` & `ZODB-5.8.1/src/ZODB/tests/dangle.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/dbopen.txt` & `ZODB-5.8.1/src/ZODB/tests/dbopen.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/fix84.rst` & `ZODB-5.8.1/src/ZODB/tests/fix84.rst`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/hexstorage.py` & `ZODB-5.8.1/src/ZODB/tests/hexstorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/loggingsupport.py` & `ZODB-5.8.1/src/ZODB/tests/loggingsupport.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/multidb.txt` & `ZODB-5.8.1/src/ZODB/tests/multidb.txt`

 * *Files 1% similar despite different names*

```diff
@@ -82,28 +82,28 @@
 
 You can (still) get a connection to a database this way:
 
     >>> import transaction
     >>> tm = transaction.TransactionManager()
     >>> cn = db.open(transaction_manager=tm)
     >>> cn                  # doctest: +ELLIPSIS
-    <Connection at ...>
+    <ZODB.Connection.Connection object at ...>
 
 This is the only connection in this collection right now:
 
     >>> cn.connections      # doctest: +ELLIPSIS
-    {'root': <Connection at ...>}
+    {'root': <ZODB.Connection.Connection object at ...>}
 
 Getting a connection to a different database from an existing connection in the
 same database collection (this enables 'connection binding' within a given
 thread/transaction/context ...):
 
     >>> cn2 = cn.get_connection('notroot')
     >>> cn2                  # doctest: +ELLIPSIS
-    <Connection at ...>
+    <ZODB.Connection.Connection object at ...>
 
 The second connection gets the same transaction manager as the first:
 
     >>> cn2.transaction_manager is tm
     True
 
 Now there are two connections in that collection:
```

### Comparing `ZODB-5.8.0/src/ZODB/tests/racetest.py` & `ZODB-5.8.1/src/ZODB/tests/racetest.py`

 * *Files 16% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 shared storage connection, where one thread repeatedly modifies the database,
 and the other thread repeatedly checks the database for breakage of the model
 invariant. This checker verifies storages and ZODB.Connection for races in
 between load/open and local invalidations to catch bugs similar to
 https://github.com/zopefoundation/ZODB/issues/290 and
 https://github.com/zopefoundation/ZEO/issues/166.
 """
+from __future__ import print_function
 
 import threading
 from random import randint
 
 import transaction
 from zope.interface import Interface
 from zope.interface import implementer
@@ -76,15 +77,15 @@
 
 
 @implementer(IModelSpec)
 class T2ObjectsInc:
     """T2ObjectsInc is specification with behaviour where two objects obj1
     and obj2 are incremented synchronously.
 
-    It is used in tests where bugs can be immedeately observed after the race.
+    It is used in tests where bugs can be immediately observed after the race.
 
     invariant:  obj1 == obj2
     """
     def init(_, root):
         root['obj1'] = MinPO(0)
         root['obj2'] = MinPO(0)
 
@@ -155,80 +156,65 @@
 
         # `verify` accesses objects in the database and verifies spec
         # invariant.
         #
         # Access to half of the objects is organized to always trigger loading
         # from zstor. Access to the other half goes through zconn cache and so
         # verifies whether the cache is not stale.
-        failed = threading.Event()
-        failure = [None]
-
-        def verify():
+        def verify(tg):
             transaction.begin()
             zconn = db.open()
             root = zconn.root()
 
             # reload some objects from zstor, while getting others from
             # zconn cache
             _state_invalidate_half1(root)
 
             try:
                 spec.assertStateOK(root)
             except AssertionError as e:
                 msg = "verify: %s\n" % e
                 msg += _state_details(root)
-                failure[0] = msg
-                failed.set()
+                tg.fail(msg)
 
             # we did not changed anything; also fails with commit:
             transaction.abort()
             zconn.close()
 
         # `modify` changes objects in the database by executing "next" step.
         #
         # Spec invariant should be preserved.
-        def modify():
+        def modify(tg):
             transaction.begin()
             zconn = db.open()
 
             root = zconn.root()
             spec.next(root)
             spec.assertStateOK(root)
 
             transaction.commit()
             zconn.close()
 
         # `xrun` runs f in a loop until either N iterations, or until failed is
         # set.
-        def xrun(f, N):
-            try:
-                for i in range(N):
-                    # print('%s.%d' % (f.__name__, i))
-                    f()
-                    if failed.is_set():
-                        break
-            except:  # noqa: E722 do not use bare 'except'
-                failed.set()
-                raise
+        def xrun(tg, tx, f, N):
+            for i in range(N):
+                # print('%s.%d' % (f.__name__, i))
+                f(tg)
+                if tg.failed():
+                    break
 
         # loop verify and modify concurrently.
         init()
 
         N = 500
-        tverify = threading.Thread(
-            name='Tverify', target=xrun, args=(verify, N))
-        tmodify = threading.Thread(
-            name='Tmodify', target=xrun, args=(modify, N))
-        tverify.start()
-        tmodify.start()
-        tverify.join(60)
-        tmodify.join(60)
-
-        if failed.is_set():
-            self.fail(failure[0])
+        tg = TestWorkGroup(self)
+        tg.go(xrun, verify, N, name='Tverify')
+        tg.go(xrun, modify, N, name='Tmodify')
+        tg.wait(120)
 
     # client-server storages like ZEO, NEO and RelStorage allow several storage
     # clients to be connected to single storage server.
     #
     # For client-server storages test subclasses should implement
     # _new_storage_client to return new storage client that is connected to the
     # same storage server self._storage is connected to.
@@ -281,18 +267,15 @@
         #
         # Access to half of the objects is organized to always trigger loading
         # from zstor. Access to the other half goes through zconn cache and so
         # verifies whether the cache is not stale.
         #
         # Once in a while T tries to modify the database executing spec "next"
         # as test source of changes for other workers.
-        failed = threading.Event()
-        failure = [None] * nwork  # [tx] is failure from T(tx)
-
-        def T(tx, N):
+        def T(tg, tx, N):
             db = self.dbopen()
 
             def t_():
                 transaction.begin()
                 zconn = db.open()
                 root = zconn.root()
 
@@ -301,16 +284,15 @@
                 _state_invalidate_half1(root)
 
                 try:
                     spec.assertStateOK(root)
                 except AssertionError as e:
                     msg = "T%s: %s\n" % (tx, e)
                     msg += _state_details(root)
-                    failure[tx] = msg
-                    failed.set()
+                    tg.fail(msg)
 
                 # change objects once in a while
                 if randint(0, 4) == 0:
                     # print("T%s: modify" % tx)
                     spec.next(root)
                     spec.assertStateOK(root)
 
@@ -322,44 +304,34 @@
 
                 zconn.close()
 
             try:
                 for i in range(N):
                     # print('T%s.%d' % (tx, i))
                     t_()
-                    if failed.is_set():
+                    if tg.failed():
                         break
-            except:  # noqa: E722 do not use bare 'except'
-                failed.set()
-                raise
             finally:
                 db.close()
 
         # run the workers concurrently.
         init()
 
         N = 100
-        tg = []
-        for x in range(nwork):
-            t = threading.Thread(name='T%d' % x, target=T, args=(x, N))
-            t.start()
-            tg.append(t)
-
-        for t in tg:
-            t.join(60)
-
-        if failed.is_set():
-            self.fail('\n\n'.join([_ for _ in failure if _]))
+        tg = TestWorkGroup(self)
+        for _ in range(nwork):
+            tg.go(T, N)
+        tg.wait(120)
 
     # verify storage for race in between client disconnect and external
     # invalidations. https://github.com/zopefoundation/ZEO/issues/209
     #
-    # This test is simlar to check_race_load_vs_external_invalidate, but
+    # This test is similar to check_race_load_vs_external_invalidate, but
     # increases the number of workers and also makes every worker to repeatedly
-    # reconnect to the storage, so that the probability of disconection is
+    # reconnect to the storage, so that the probability of disconnection is
     # high. It also uses T2ObjectsInc2Phase instead of T2ObjectsInc because if
     # an invalidation is skipped due to the disconnect/invalidation race,
     # T2ObjectsInc won't catch the bug as both objects will be either in old
     # state, or in new state after the next transaction. Contrary to that, with
     # T2ObjectsInc2Phase the invariant will be detected to be broken on the
     # next transaction.
     @long_test
@@ -377,18 +349,15 @@
             _state_init(db, spec)
             db.close()
 
         nwork = 8*8   # nwork^2 from _check_race_load_vs_external_invalidate
 
         # `T` is similar to the T from _check_race_load_vs_external_invalidate
         # but reconnects to the database often.
-        failed = threading.Event()
-        failure = [None] * nwork  # [tx] is failure from T(tx)
-
-        def T(tx, N):
+        def T(tg, tx, N):
             def t_():
                 def work1(db):
                     transaction.begin()
                     zconn = db.open()
                     root = zconn.root()
 
                     # reload some objects from zstor, while getting others from
@@ -396,16 +365,15 @@
                     _state_invalidate_half1(root)
 
                     try:
                         spec.assertStateOK(root)
                     except AssertionError as e:
                         msg = "T%s: %s\n" % (tx, e)
                         msg += _state_details(root)
-                        failure[tx] = msg
-                        failed.set()
+                        tg.fail(msg)
 
                         zconn.close()
                         transaction.abort()
                         return
 
                     # change objects once in a while
                     if randint(0, 4) == 0:
@@ -420,59 +388,48 @@
                         transaction.abort()
 
                     zconn.close()
 
                 db = self.dbopen()
                 try:
                     for i in range(4):
-                        if failed.is_set():
+                        if tg.failed():
                             break
                         work1(db)
                 finally:
                     db.close()
 
-            try:
-                for i in range(N):
-                    # print('T%s.%d' % (tx, i))
-                    if failed.is_set():
-                        break
-                    t_()
-            except:  # noqa: E722 do not use bare 'except'
-                failed.set()
-                raise
+            for i in range(N):
+                # print('T%s.%d' % (tx, i))
+                if tg.failed():
+                    break
+                t_()
 
         # run the workers concurrently.
         init()
 
         N = 100 // (2*4)  # N reduced to save time
-        tg = []
-        for x in range(nwork):
-            t = threading.Thread(name='T%d' % x, target=T, args=(x, N))
-            t.start()
-            tg.append(t)
-
-        for t in tg:
-            t.join(60)
-
-        if failed.is_set():
-            self.fail('\n\n'.join([_ for _ in failure if _]))
+        tg = TestWorkGroup(self)
+        for _ in range(nwork):
+            tg.go(T, N)
+        tg.wait(120)
 
 
 # `_state_init` initializes the database according to the spec.
 def _state_init(db, spec):
     transaction.begin()
     zconn = db.open()
     root = zconn.root()
     spec.init(root)
     spec.assertStateOK(root)
     transaction.commit()
     zconn.close()
 
 
-# `_state_invalidate_half1` invalidatates first 50% of database objects, so
+# `_state_invalidate_half1` invalidates first 50% of database objects, so
 # that the next time they are accessed, they are reloaded from the storage.
 def _state_invalidate_half1(root):
     keys = list(sorted(root.keys()))
     for k in keys[:len(keys)//2]:
         obj = root[k]
         obj._p_invalidate()
 
@@ -520,7 +477,162 @@
     if zcache is not None:
         zcache.clear()
         txt += 'zstor._cache.clear()\n'
         for k in keys:
             txt += load(k)
 
     return txt
+
+
+class TestWorkGroup(object):
+    """TestWorkGroup represents group of threads that run together to verify
+       something.
+
+       - .go() adds test thread to the group.
+       - .wait() waits for all spawned threads to finish and reports all
+         collected failures to containing testcase.
+       - a test should indicate failure by call to .fail(), it
+         can check for a failure with .failed()
+    """
+
+    def __init__(self, testcase):
+        self.testcase = testcase
+        self.failed_event = threading.Event()
+        self.fail_mu = threading.Lock()
+        self.failv = []           # failures registered by .fail
+        self.threadv = []         # spawned threads
+        self.waitg = WaitGroup()  # to wait for spawned threads
+
+    def fail(self, msg):
+        """fail adds failure to test result."""
+        with self.fail_mu:
+            self.failv.append(msg)
+        self.failed_event.set()
+
+    def failed(self):
+        """did the test already fail."""
+        return self.failed_event.is_set()
+
+    def go(self, f, *argv, **kw):
+        """go spawns f(self, #thread, *argv, **kw) in new test thread."""
+        self.waitg.add(1)
+        tx = len(self.threadv)
+        tname = kw.pop('name', 'T%d' % tx)
+        t = Daemon(name=tname, target=self._run, args=(f, tx, argv, kw))
+        self.threadv.append(t)
+        t.start()
+
+    def _run(self, f, tx, argv, kw):
+        tname = self.threadv[tx].name
+        try:
+            f(self, tx, *argv, **kw)
+        except Exception as e:
+            self.fail("Unhandled exception %r in thread %s"
+                      % (e, tname))
+            raise
+        finally:
+            self.waitg.done()
+
+    def wait(self, timeout):
+        """wait waits for all test threads to complete and reports all
+           collected failures to containing testcase."""
+        if not self.waitg.wait(timeout):
+            self.fail("test did not finish within %s seconds" % timeout)
+
+        failed_to_finish = []
+        for t in self.threadv:
+            try:
+                t.join(1)
+            except AssertionError:
+                self.failed_event.set()
+                failed_to_finish.append(t.name)
+        if failed_to_finish:
+            self.fail("threads did not finish: %s" % failed_to_finish)
+        del self.threadv  # avoid cyclic garbage
+
+        if self.failed():
+            self.testcase.fail('\n\n'.join(self.failv))
+
+
+class Daemon(threading.Thread):
+    """auxiliary class to create daemon threads and fail if not stopped.
+
+    In addition, the class ensures that reports for uncaught exceptions
+    are output holding a lock. This prevents that concurrent reports
+    get intermixed and facilitates the exception analysis.
+    """
+    def __init__(self, **kw):
+        super(Daemon, self).__init__(**kw)
+        self.daemon = True
+        if hasattr(self, "_invoke_excepthook"):
+            # Python 3.8+
+            ori_invoke_excepthook = self._invoke_excepthook
+
+            def invoke_excepthook(*args, **kw):
+                with exc_lock:
+                    return ori_invoke_excepthook(*args, **kw)
+
+            self._invoke_excepthook = invoke_excepthook
+        else:
+            # old Python
+            ori_run = self.run
+
+            def run():
+                from threading import _format_exc
+                from threading import _sys
+                try:
+                    ori_run()
+                except SystemExit:
+                    pass
+                except BaseException:
+                    if _sys and _sys.stderr is not None:
+                        with exc_lock:
+                            print("Exception in thread %s:\n%s" %
+                                  (self.name, _format_exc()),
+                                  file=_sys.stderr)
+                    else:
+                        raise
+                finally:
+                    del self.run
+
+            self.run = run
+
+    def join(self, *args, **kw):
+        super(Daemon, self).join(*args, **kw)
+        if self.is_alive():
+            raise AssertionError("Thread %s did not stop" % self.name)
+
+
+# lock to ensure that Daemon exception reports are output atomically
+exc_lock = threading.Lock()
+
+
+class WaitGroup(object):
+    """WaitGroup provides service to wait for spawned workers to be done.
+
+       - .add() adds workers
+       - .done() indicates that one worker is done
+       - .wait() waits until all workers are done
+    """
+    def __init__(self):
+        self.n = 0
+        self.condition = threading.Condition()
+
+    def add(self, delta):
+        with self.condition:
+            self.n += delta
+            if self.n < 0:
+                raise AssertionError("#workers is negative")
+            if self.n == 0:
+                self.condition.notify_all()
+
+    def done(self):
+        self.add(-1)
+
+    def wait(self, timeout):  # -> ok
+        with self.condition:
+            if self.n == 0:
+                return True
+            ok = self.condition.wait(timeout)
+            if ok is None:  # py2
+                ok = (self.n == 0)
+            return ok
```

### Comparing `ZODB-5.8.0/src/ZODB/tests/sampledm.py` & `ZODB-5.8.1/src/ZODB/tests/sampledm.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/speed.py` & `ZODB-5.8.1/src/ZODB/tests/speed.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/synchronizers.txt` & `ZODB-5.8.1/src/ZODB/tests/synchronizers.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testActivityMonitor.py` & `ZODB-5.8.1/src/ZODB/tests/testActivityMonitor.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testBroken.py` & `ZODB-5.8.1/src/ZODB/tests/testBroken.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testCache.py` & `ZODB-5.8.1/src/ZODB/tests/testCache.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testConfig.py` & `ZODB-5.8.1/src/ZODB/tests/testConfig.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testConnection.py` & `ZODB-5.8.1/src/ZODB/tests/testConnection.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testConnectionSavepoint.py` & `ZODB-5.8.1/src/ZODB/tests/testConnectionSavepoint.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testConnectionSavepoint.txt` & `ZODB-5.8.1/src/ZODB/tests/testConnectionSavepoint.txt`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testDB.py` & `ZODB-5.8.1/src/ZODB/tests/testDB.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testDemoStorage.py` & `ZODB-5.8.1/src/ZODB/tests/testDemoStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testFileStorage.py` & `ZODB-5.8.1/src/ZODB/tests/testFileStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testMVCCMappingStorage.py` & `ZODB-5.8.1/src/ZODB/tests/testMVCCMappingStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testMappingStorage.py` & `ZODB-5.8.1/src/ZODB/tests/testMappingStorage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testPersistentList.py` & `ZODB-5.8.1/src/ZODB/tests/testPersistentList.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testPersistentMapping.py` & `ZODB-5.8.1/src/ZODB/tests/testPersistentMapping.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testPersistentWeakref.py` & `ZODB-5.8.1/src/ZODB/tests/testPersistentWeakref.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testRecover.py` & `ZODB-5.8.1/src/ZODB/tests/testRecover.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testSerialize.py` & `ZODB-5.8.1/src/ZODB/tests/testSerialize.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testThreadedShutdown.py` & `ZODB-5.8.1/src/ZODB/tests/testThreadedShutdown.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testUtils.py` & `ZODB-5.8.1/src/ZODB/tests/testUtils.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testZODB.py` & `ZODB-5.8.1/src/ZODB/tests/testZODB.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/test_TransactionMetaData.py` & `ZODB-5.8.1/src/ZODB/tests/test_TransactionMetaData.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/test_cache.py` & `ZODB-5.8.1/src/ZODB/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/test_doctest_files.py` & `ZODB-5.8.1/src/ZODB/tests/test_doctest_files.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/test_fsdump.py` & `ZODB-5.8.1/src/ZODB/tests/test_fsdump.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/test_mvccadapter.py` & `ZODB-5.8.1/src/ZODB/tests/test_mvccadapter.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/test_prefetch.py` & `ZODB-5.8.1/src/ZODB/tests/test_prefetch.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/test_storage.py` & `ZODB-5.8.1/src/ZODB/tests/test_storage.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testblob.py` & `ZODB-5.8.1/src/ZODB/tests/testblob.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testconflictresolution.py` & `ZODB-5.8.1/src/ZODB/tests/testconflictresolution.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testcrossdatabasereferences.py` & `ZODB-5.8.1/src/ZODB/tests/testcrossdatabasereferences.py`

 * *Files 2% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     >>> p2.p1 = p1
     >>> tm.commit() # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
     Traceback (most recent call last):
     ...
     InvalidObjectReference:
     ('Attempt to store a reference to an object from a separate connection to
     the same database or multidatabase',
-    <Connection at ...>,
+    <ZODB.Connection.Connection object at ...>,
     <ZODB.tests.testcrossdatabasereferences.MyClass object at ...>)
 
     >>> tm.abort()
 
 Even without multi-databases, a common mistake is to mix objects in
 different connections to the same database.
 
@@ -76,15 +76,15 @@
     >>> p2.p1 = p1
     >>> tm.commit() # doctest: +NORMALIZE_WHITESPACE +ELLIPSIS
     Traceback (most recent call last):
     ...
     InvalidObjectReference:
     ('Attempt to store a reference to an object from a separate connection
     to the same database or multidatabase',
-    <Connection at ...>,
+    <ZODB.Connection.Connection object at ...>,
     <ZODB.tests.testcrossdatabasereferences.MyClass object at ...>)
 
     >>> tm.abort()
 
 """
```

### Comparing `ZODB-5.8.0/src/ZODB/tests/testdocumentation.py` & `ZODB-5.8.1/src/ZODB/tests/testdocumentation.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testfsIndex.py` & `ZODB-5.8.1/src/ZODB/tests/testfsIndex.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testfsoids.py` & `ZODB-5.8.1/src/ZODB/tests/testfsoids.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testhistoricalconnections.py` & `ZODB-5.8.1/src/ZODB/tests/testhistoricalconnections.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testmvcc.py` & `ZODB-5.8.1/src/ZODB/tests/testmvcc.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/testpersistentclass.py` & `ZODB-5.8.1/src/ZODB/tests/testpersistentclass.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/tests/util.py` & `ZODB-5.8.1/src/ZODB/tests/util.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/transact.py` & `ZODB-5.8.1/src/ZODB/transact.py`

 * *Files identical despite different names*

### Comparing `ZODB-5.8.0/src/ZODB/utils.py` & `ZODB-5.8.1/src/ZODB/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -37,15 +37,14 @@
            'U64',
            'cp',
            'maxtid',
            'newTid',
            'oid_repr',
            'serial_repr',
            'tid_repr',
-           'positive_id',
            'readable_tid_repr',
            'get_pickle_metadata',
            'locked',
            ]
 
 
 if PY2:
@@ -180,36 +179,14 @@
 
 def readable_tid_repr(tid):
     result = tid_repr(tid)
     if isinstance(tid, bytes) and len(tid) == 8:
         result = "%s %s" % (result, TimeStamp(tid))
     return result
 
-# Addresses can "look negative" on some boxes, some of the time.  If you
-# feed a "negative address" to an %x format, Python 2.3 displays it as
-# unsigned, but produces a FutureWarning, because Python 2.4 will display
-# it as signed.  So when you want to prodce an address, use positive_id() to
-# obtain it.
-# _ADDRESS_MASK is 2**(number_of_bits_in_a_native_pointer).  Adding this to
-# a negative address gives a positive int with the same hex representation as
-# the significant bits in the original.
-
-
-_ADDRESS_MASK = 256 ** struct.calcsize('P')
-
-
-def positive_id(obj):
-    """Return id(obj) as a non-negative integer."""
-
-    result = id(obj)
-    if result < 0:
-        result += _ADDRESS_MASK
-        assert result > 0
-    return result
-
 # Given a ZODB pickle, return pair of strings (module_name, class_name).
 # Do this without importing the module or class object.
 # See ZODB/serialize.py's module docstring for the only docs that exist about
 # ZODB pickle format.  If the code here gets smarter, please update those
 # docs to be at least as smart.  The code here doesn't appear to make sense
 # for what serialize.py calls formats 5 and 6.
```

### Comparing `ZODB-5.8.0/src/ZODB/utils.rst` & `ZODB-5.8.1/src/ZODB/utils.rst`

 * *Files 0% similar despite different names*

```diff
@@ -11,36 +11,36 @@
 more.
 
 64-bit integers and strings
 ===========================
 
 ZODB uses 64-bit transaction ids that are typically represented as
 strings, but are sometimes manipulated as integers.  Object ids are
-strings too and it is common to ise 64-bit strings that are just
+strings too and it is common to use 64-bit strings that are just
 packed integers.
 
 Functions p64 and u64 pack and unpack integers as strings:
 
     >>> ZODB.utils.p64(250347764455111456)
     '\x03yi\xf7"\xa8\xfb '
 
     >>> print(ZODB.utils.u64(b'\x03yi\xf7"\xa8\xfb '))
     250347764455111456
 
-The contant z64 has zero packed as a 64-bit string:
+The constant z64 has zero packed as a 64-bit string:
 
     >>> ZODB.utils.z64
     '\x00\x00\x00\x00\x00\x00\x00\x00'
 
 Transaction id generation
 =========================
 
 Storages assign transaction ids as transactions are committed.  These
 are based on UTC time, but must be strictly increasing.  The
-newTid function akes this pretty easy.
+newTid function makes this pretty easy.
 
 To see this work (in a predictable way), we'll first hack time.time:
 
     >>> import time
     >>> old_time = time.time
     >>> time_value = 1224825068.12
     >>> faux_time = lambda: time_value
```

### Comparing `ZODB-5.8.0/src/ZODB.egg-info/PKG-INFO` & `ZODB-5.8.1/src/ZODB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ZODB
-Version: 5.8.0
+Version: 5.8.1
 Summary: ZODB, a Python object-oriented database
 Home-page: http://zodb-docs.readthedocs.io
 Author: Jim Fulton
 Author-email: jim@zope.com
 Maintainer: Zope Foundation and Contributors
 Maintainer-email: zodb-dev@zope.org
 License: ZPL 2.1
@@ -44,16 +44,16 @@
    :target: https://pypi.org/project/ZODB/
    :alt: Latest release
 
 .. image:: https://img.shields.io/pypi/pyversions/ZODB.svg
    :target: https://pypi.org/project/ZODB/
    :alt: Supported Python versions
 
-.. image:: https://travis-ci.com/zopefoundation/ZODB.svg?branch=master
-   :target: https://travis-ci.com/zopefoundation/ZODB
+.. image:: https://github.com/zopefoundation/ZODB/actions/workflows/tests.yml/badge.svg
+   :target: https://github.com/zopefoundation/ZODB/actions/workflows/tests.yml
    :alt: Build status
 
 .. image:: https://coveralls.io/repos/github/zopefoundation/ZODB/badge.svg
    :target: https://coveralls.io/github/zopefoundation/ZODB
    :alt: Coverage status
 
 .. image:: https://readthedocs.org/projects/zodb-docs/badge/?version=latest
@@ -86,14 +86,24 @@
 <https://github.com/zopefoundation/ZODB/blob/master/DEVELOPERS.rst>`_.
 
 
 ================
  Change History
 ================
 
+5.8.1 (2023-07-18)
+==================
+
+- Fix ``racetest`` problems.
+  For details see `#376 <https://github.com/zopefoundation/ZODB/pull/376>`_.
+
+- Fix ``--with-verify`` argument in script repozo ``--recover``.
+  For details see `#381 <https://github.com/zopefoundation/ZODB/pull/381>`_.
+
+
 5.8.0 (2022-11-09)
 ==================
 
 - Add support for Python 3.11.
 
 - Expand and refactor tests for race conditions.
```

### Comparing `ZODB-5.8.0/src/ZODB.egg-info/SOURCES.txt` & `ZODB-5.8.1/src/ZODB.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -237,19 +237,19 @@
 src/ZODB/tests/testZODB.py
 src/ZODB/tests/test_TransactionMetaData.py
 src/ZODB/tests/test_cache.py
 src/ZODB/tests/test_doctest_files.py
 src/ZODB/tests/test_fsdump.py
 src/ZODB/tests/test_mvccadapter.py
 src/ZODB/tests/test_prefetch.py
+src/ZODB/tests/test_racetest.py
 src/ZODB/tests/test_storage.py
 src/ZODB/tests/testblob.py
 src/ZODB/tests/testconflictresolution.py
 src/ZODB/tests/testcrossdatabasereferences.py
 src/ZODB/tests/testdocumentation.py
 src/ZODB/tests/testfsIndex.py
 src/ZODB/tests/testfsoids.py
 src/ZODB/tests/testhistoricalconnections.py
 src/ZODB/tests/testmvcc.py
 src/ZODB/tests/testpersistentclass.py
-src/ZODB/tests/util.py
-src/ZODB/tests/warnhook.py
+src/ZODB/tests/util.py
```

### Comparing `ZODB-5.8.0/tox.ini` & `ZODB-5.8.1/tox.ini`

 * *Files identical despite different names*

