# Comparing `tmp/nomenklatura-3.3.1.tar.gz` & `tmp/nomenklatura-3.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomenklatura-3.3.1.tar", last modified: Sat Jul 15 09:19:55 2023, max compression
+gzip compressed data, was "nomenklatura-3.3.2.tar", last modified: Tue Jul 18 14:29:00 2023, max compression
```

## Comparing `nomenklatura-3.3.1.tar` & `nomenklatura-3.3.2.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.069988 nomenklatura-3.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-15 09:19:55.069988 nomenklatura-3.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.061987 nomenklatura-3.3.1/nomenklatura/
--rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.061987 nomenklatura-3.3.1/nomenklatura/data/
--rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/data/regression-v1.pkl
--rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/data/regression-v2.pkl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.061987 nomenklatura-3.3.1/nomenklatura/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/dataset/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/dataset/coverage.py
--rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/dataset/publisher.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/dataset/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/dataset/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.061987 nomenklatura-3.3.1/nomenklatura/enrich/
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5614 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/aleph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5629 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/nominatim.py
--rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/opencorporates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.061987 nomenklatura-3.3.1/nomenklatura/enrich/wikidata/
--rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/wikidata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/wikidata/lang.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/wikidata/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/wikidata/props.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/wikidata/qualified.py
--rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/wikidata/value.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/enrich/yente.py
--rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.061987 nomenklatura-3.3.1/nomenklatura/index/
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/index/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/index/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/index/index.py
--rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/index/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/judgement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/matching/
--rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/matching/heuristic/
--rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/heuristic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2468 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/heuristic/logic.py
--rw-r--r--   0 runner    (1001) docker     (123)     1230 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/pairs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2630 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/matching/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v1/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v1/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v1/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v1/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v1/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v1/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/matching/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v2/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v2/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v2/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v2/names.py
--rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v2/train.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/matching/v2/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/publish/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/publish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/publish/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/publish/edges.py
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/publish/names.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/resolver/
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/resolver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/resolver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/resolver/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/resolver/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/resolver/resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/senzing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/statement/
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/statement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/statement/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/statement/statement.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.065988 nomenklatura-3.3.1/nomenklatura/store/
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/store/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4010 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/store/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/store/level.py
--rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/store/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/store/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.069988 nomenklatura-3.3.1/nomenklatura/tui/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/tui/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/tui/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/tui/comparison.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/tui/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/nomenklatura/xref.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-15 09:19:55.061987 nomenklatura-3.3.1/nomenklatura.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-15 09:19:55.000000 nomenklatura-3.3.1/nomenklatura.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-15 09:19:55.000000 nomenklatura-3.3.1/nomenklatura.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 09:19:55.000000 nomenklatura-3.3.1/nomenklatura.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-15 09:19:55.000000 nomenklatura-3.3.1/nomenklatura.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 09:19:55.000000 nomenklatura-3.3.1/nomenklatura.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-15 09:19:08.000000 nomenklatura-3.3.1/nomenklatura.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-15 09:19:55.000000 nomenklatura-3.3.1/nomenklatura.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-15 09:19:55.000000 nomenklatura-3.3.1/nomenklatura.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-15 09:19:55.069988 nomenklatura-3.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-15 09:17:26.000000 nomenklatura-3.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.220611 nomenklatura-3.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-18 14:29:00.220611 nomenklatura-3.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4613 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.216611 nomenklatura-3.3.2/nomenklatura/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5473 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.216611 nomenklatura-3.3.2/nomenklatura/data/
+-rw-r--r--   0 runner    (1001) docker     (123)     2271 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/data/regression-v1.pkl
+-rw-r--r--   0 runner    (1001) docker     (123)     2076 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/data/regression-v2.pkl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.216611 nomenklatura-3.3.2/nomenklatura/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1922 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/dataset/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/dataset/coverage.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5021 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1345 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/dataset/publisher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/dataset/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/dataset/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      861 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.216611 nomenklatura-3.3.2/nomenklatura/enrich/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/enrich/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5613 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/enrich/aleph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5596 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/enrich/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2381 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/enrich/nominatim.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10087 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/enrich/opencorporates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.216611 nomenklatura-3.3.2/nomenklatura/enrich/wikidata/
+-rw-r--r--   0 runner    (1001) docker     (123)     9872 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/enrich/wikidata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2380 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/enrich/wikidata/lang.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/enrich/wikidata/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/enrich/wikidata/props.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/enrich/wikidata/qualified.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1915 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/enrich/wikidata/value.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4671 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/enrich/yente.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15265 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.216611 nomenklatura-3.3.2/nomenklatura/index/
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/index/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/index/entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5011 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/index/index.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/index/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/judgement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.216611 nomenklatura-3.3.2/nomenklatura/matching/
+-rw-r--r--   0 runner    (1001) docker     (123)     1032 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.216611 nomenklatura-3.3.2/nomenklatura/matching/heuristic/
+-rw-r--r--   0 runner    (1001) docker     (123)     5942 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/heuristic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2472 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/heuristic/logic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/pairs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.220611 nomenklatura-3.3.2/nomenklatura/matching/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/v1/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/v1/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3859 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/v1/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2346 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/v1/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/v1/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/v1/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.220611 nomenklatura-3.3.2/nomenklatura/matching/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1289 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/v2/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/v2/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3741 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/v2/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/v2/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3220 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/v2/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/matching/v2/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.220611 nomenklatura-3.3.2/nomenklatura/publish/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/publish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/publish/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/publish/edges.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/publish/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.220611 nomenklatura-3.3.2/nomenklatura/resolver/
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/resolver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/resolver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1854 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/resolver/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/resolver/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12467 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/resolver/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5038 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/senzing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.220611 nomenklatura-3.3.2/nomenklatura/statement/
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/statement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6283 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/statement/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7731 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/statement/statement.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.220611 nomenklatura-3.3.2/nomenklatura/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/store/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4014 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/store/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5548 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/store/level.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3751 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/store/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/store/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.220611 nomenklatura-3.3.2/nomenklatura/tui/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/tui/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4909 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/tui/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/tui/comparison.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/tui/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4705 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3229 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/nomenklatura/xref.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 14:29:00.216611 nomenklatura-3.3.2/nomenklatura.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-07-18 14:29:00.000000 nomenklatura-3.3.2/nomenklatura.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-07-18 14:29:00.000000 nomenklatura-3.3.2/nomenklatura.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:29:00.000000 nomenklatura-3.3.2/nomenklatura.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-18 14:29:00.000000 nomenklatura-3.3.2/nomenklatura.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:29:00.000000 nomenklatura-3.3.2/nomenklatura.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 14:28:15.000000 nomenklatura-3.3.2/nomenklatura.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-07-18 14:29:00.000000 nomenklatura-3.3.2/nomenklatura.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 14:29:00.000000 nomenklatura-3.3.2/nomenklatura.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 14:29:00.220611 nomenklatura-3.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-07-18 14:26:42.000000 nomenklatura-3.3.2/setup.py
```

### Comparing `nomenklatura-3.3.1/LICENSE` & `nomenklatura-3.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/PKG-INFO` & `nomenklatura-3.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.3.1
+Version: 3.3.2
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Platform: UNKNOWN
```

### Comparing `nomenklatura-3.3.1/README.md` & `nomenklatura-3.3.2/README.md`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/cache.py` & `nomenklatura-3.3.2/nomenklatura/cache.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/cli.py` & `nomenklatura-3.3.2/nomenklatura/cli.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/data/regression-v1.pkl` & `nomenklatura-3.3.2/nomenklatura/data/regression-v1.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/data/regression-v2.pkl` & `nomenklatura-3.3.2/nomenklatura/data/regression-v2.pkl`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/dataset/catalog.py` & `nomenklatura-3.3.2/nomenklatura/dataset/catalog.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,16 +39,16 @@
     def has(self, name: str) -> bool:
         return name in self.names
 
     @property
     def names(self) -> Set[str]:
         return {d.name for d in self.datasets}
 
-    def __repr__(self) -> str:
-        return f"<DataCatalog[{self.dataset_type.__name__}]({self.names!r})>"  # pragma: no cover
+    def __repr__(self) -> str:  # pragma: no cover
+        return f"<DataCatalog[{self.dataset_type.__name__}]({self.names!r})>"
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "datasets": [d.to_dict() for d in self.datasets],
             "updated_at": self.updated_at,
         }
```

### Comparing `nomenklatura-3.3.1/nomenklatura/dataset/coverage.py` & `nomenklatura-3.3.2/nomenklatura/dataset/coverage.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/dataset/dataset.py` & `nomenklatura-3.3.2/nomenklatura/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/dataset/publisher.py` & `nomenklatura-3.3.2/nomenklatura/dataset/publisher.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/dataset/resource.py` & `nomenklatura-3.3.2/nomenklatura/dataset/resource.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/dataset/util.py` & `nomenklatura-3.3.2/nomenklatura/dataset/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/db.py` & `nomenklatura-3.3.2/nomenklatura/db.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/enrich/__init__.py` & `nomenklatura-3.3.2/nomenklatura/enrich/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/enrich/aleph.py` & `nomenklatura-3.3.2/nomenklatura/enrich/aleph.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
     #             search_api = res.get("next")
     #             if search_api is None:
     #                 break
 
     def match(self, entity: CE) -> Generator[CE, None, None]:
         if not entity.schema.matchable:
             return
-        url = urljoin(self._base_url, f"match")
+        url = urljoin(self._base_url, "match")
         if self.collection_id is not None:
             url = normalize_url(url, {"collection_ids": self.collection_id})
         query = {
             "schema": entity.schema.name,
             "properties": entity.properties,
         }
         cache_id = entity.id or hash_data(query)
```

### Comparing `nomenklatura-3.3.1/nomenklatura/enrich/common.py` & `nomenklatura-3.3.2/nomenklatura/enrich/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 import json
 import logging
 from banal import as_bool
 from typing import Union, Any, Dict, Optional, Generator
 from abc import ABC, abstractmethod
 from requests import Session
 from requests.exceptions import RequestException
-from followthemoney import model
 
 from nomenklatura import __version__
 from nomenklatura.entity import CE
 from nomenklatura.dataset import DS
 from nomenklatura.cache import Cache
 from nomenklatura.util import ParamsType, normalize_url
```

### Comparing `nomenklatura-3.3.1/nomenklatura/enrich/nominatim.py` & `nomenklatura-3.3.2/nomenklatura/enrich/nominatim.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/enrich/opencorporates.py` & `nomenklatura-3.3.2/nomenklatura/enrich/opencorporates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/enrich/wikidata/__init__.py` & `nomenklatura-3.3.2/nomenklatura/enrich/wikidata/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/enrich/wikidata/lang.py` & `nomenklatura-3.3.2/nomenklatura/enrich/wikidata/lang.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/enrich/wikidata/model.py` & `nomenklatura-3.3.2/nomenklatura/enrich/wikidata/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/enrich/wikidata/props.py` & `nomenklatura-3.3.2/nomenklatura/enrich/wikidata/props.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/enrich/wikidata/qualified.py` & `nomenklatura-3.3.2/nomenklatura/enrich/wikidata/qualified.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/enrich/wikidata/value.py` & `nomenklatura-3.3.2/nomenklatura/enrich/wikidata/value.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/enrich/yente.py` & `nomenklatura-3.3.2/nomenklatura/enrich/yente.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,14 +22,15 @@
 
     def __init__(self, dataset: DS, cache: Cache, config: EnricherConfig):
         super().__init__(dataset, cache, config)
         self._api: str = config.pop("api")
         self._dataset: str = config.pop("dataset", "default")
         self._threshold: Optional[float] = config.pop("threshold", None)
         self._nested: bool = config.pop("expand_nested", True)
+        self._fuzzy: bool = config.pop("fuzzy", False)
         self._ns: Optional[Namespace] = None
         if self.get_config_bool("strip_namespace"):
             self._ns = Namespace()
 
         api_key: Optional[str] = os.path.expandvars(config.pop("api_key", "")).strip()
         if api_key is None or not len(api_key):
             api_key = os.environ.get("YENTE_API_KEY")
@@ -43,16 +44,18 @@
     def make_url(self, entity: CE) -> str:
         return urljoin(self._api, f"entities/{entity.id}")
 
     def match(self, entity: CE) -> Generator[CE, None, None]:
         if not entity.schema.matchable:
             return
         url = urljoin(self._api, f"match/{self._dataset}")
+        params: Dict[str, Any] = {"fuzzy": self._fuzzy}
         if self._threshold is not None:
-            url = normalize_url(url, {"threshold": self._threshold})
+            params["threshold"] = self._threshold
+        url = normalize_url(url, params)
         cache_key = f"{url}:{entity.id}"
         props: Dict[str, List[str]] = {}
         for prop in entity.iterprops():
             if prop.type == registry.entity:
                 continue
             if prop.matchable:
                 props[prop.name] = entity.get(prop)
```

### Comparing `nomenklatura-3.3.1/nomenklatura/entity.py` & `nomenklatura-3.3.2/nomenklatura/entity.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/index/entry.py` & `nomenklatura-3.3.2/nomenklatura/index/entry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import math
-from typing import Any, Dict, Generator, Tuple, cast
+from typing import Any, Dict, Generator, Tuple
 
 from nomenklatura.resolver import Identifier
 
 
 class Entry(object):
     """A set of entities and a weight associated with a given term in the index."""
```

### Comparing `nomenklatura-3.3.1/nomenklatura/index/index.py` & `nomenklatura-3.3.2/nomenklatura/index/index.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/index/tokenizer.py` & `nomenklatura-3.3.2/nomenklatura/index/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from normality import normalize, WS
-from typing import Generic, Generator, Generic, Tuple
+from typing import Generic, Generator, Tuple
 from followthemoney.types import registry
 from followthemoney.types.common import PropertyType
 
 from nomenklatura.dataset import DS
 from nomenklatura.entity import CE
 from nomenklatura.util import fingerprint_name
```

### Comparing `nomenklatura-3.3.1/nomenklatura/judgement.py` & `nomenklatura-3.3.2/nomenklatura/judgement.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/__init__.py` & `nomenklatura-3.3.2/nomenklatura/matching/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/heuristic/__init__.py` & `nomenklatura-3.3.2/nomenklatura/matching/heuristic/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 from nomenklatura.matching.heuristic.logic import soundex_name_parts, jaro_name_parts
 from nomenklatura.matching.heuristic.logic import is_disjoint, compare_identifiers
 from nomenklatura.matching.util import make_github_url, dates_precision
 from nomenklatura.matching.util import props_pair, type_pair, compare_sets
 
 
 class NameMatcher(ScoringAlgorithm):
-    """An algorithm that matches on entity name, using phonetic comparisons and edit distance
-    to generate potential matches. This implementation is vaguely based on the behaviour
-    proposed by the US OFAC documentation (FAQ #249)."""
+    """An algorithm that matches on entity name, using phonetic comparisons and edit
+    distance to generate potential matches. This implementation is vaguely based on
+    the behaviour proposed by the US OFAC documentation (FAQ #249)."""
 
     # Try to re-produce results from: https://sanctionssearch.ofac.treas.gov/
     # cf. https://ofac.treasury.gov/faqs/topic/1636
 
     NAME = "name-based"
 
     @classmethod
@@ -53,17 +53,17 @@
         }
         # score = (jaro_score + soundex_score + full_name_score) / 3.0
         score = (jaro_score + soundex_score) / 2.0
         return MatchingResult(score=score, features=features)
 
 
 class NameQualifiedMatcher(ScoringAlgorithm):
-    """Same as the name-based algorithm, but scores will be reduced if a mis-match of birth
-    dates and nationalities is found for persons, or different tax/registration identifiers
-    are included for organizations and companies."""
+    """Same as the name-based algorithm, but scores will be reduced if a mis-match
+    of birth dates and nationalities is found for persons, or different
+    tax/registration identifiers are included for organizations and companies."""
 
     NAME = "name-qualified"
     COUNTRIES_DISJOINT = "countries_disjoint"
     DOB_DAY_DISJOINT = "dob_day_disjoint"
     DOB_YEAR_DISJOINT = "dob_year_disjoint"
     ID_DISJOINT = "identifier_disjoint"
```

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/heuristic/logic.py` & `nomenklatura-3.3.2/nomenklatura/matching/heuristic/logic.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,16 @@
         part_soundex = soundex(part)
         soundex_score = 1.0 if part_soundex in result_soundex else 0.0
         similiarities.append(soundex_score)
     return sum(similiarities) / float(max(1.0, len(similiarities)))
 
 
 def jaro_name_parts(query: List[str], result: List[str]) -> float:
-    """Compare two sets of name parts using the Jaro-Winkler string similarity algorithm."""
+    """Compare two sets of name parts using the Jaro-Winkler string similarity
+    algorithm."""
     result_parts = name_words(result)
     similiarities: List[float] = []
     for part in name_words(query):
         best = 0.0
 
         for other in result_parts:
             part_similarity = jaro_winkler_similarity(part, other)
```

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/pairs.py` & `nomenklatura-3.3.2/nomenklatura/matching/pairs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 import json
 from typing import Generator
 from followthemoney import model
 from followthemoney.proxy import EntityProxy
 
-from nomenklatura.entity import CompositeEntity
 from nomenklatura.judgement import Judgement
 from nomenklatura.util import PathLike
 
 
 class JudgedPair(object):
     """A pair of two entities which have been judged to be the same
     (or not) by a user."""
```

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/types.py` & `nomenklatura-3.3.2/nomenklatura/matching/types.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/util.py` & `nomenklatura-3.3.2/nomenklatura/matching/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -58,18 +58,18 @@
     left: Iterable[Optional[V]],
     right: Iterable[Optional[V]],
     compare_func: Callable[[V, V], float],
     select_func: Callable[[Iterable[float]], float] = max,
 ) -> float:
     """Compare two sets of values pair-wise and select the highest-scored result."""
     results: List[float] = []
-    for (l, r) in product(left, right):
-        if l is None or r is None:
+    for (le, ri) in product(left, right):
+        if le is None or ri is None:
             continue
-        results.append(compare_func(l, r))
+        results.append(compare_func(le, ri))
     if not len(results):
         return 0.0
     return select_func(results)
 
 
 def make_github_url(func: Callable[..., Any]) -> str:
     """Make a URL to the source code of a matching function."""
```

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/v1/dates.py` & `nomenklatura-3.3.2/nomenklatura/matching/v1/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/v1/misc.py` & `nomenklatura-3.3.2/nomenklatura/matching/v1/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/v1/model.py` & `nomenklatura-3.3.2/nomenklatura/matching/v1/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/v1/names.py` & `nomenklatura-3.3.2/nomenklatura/matching/v1/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/v1/train.py` & `nomenklatura-3.3.2/nomenklatura/matching/v1/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/v1/util.py` & `nomenklatura-3.3.2/nomenklatura/matching/v1/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/v2/dates.py` & `nomenklatura-3.3.2/nomenklatura/matching/v2/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/v2/misc.py` & `nomenklatura-3.3.2/nomenklatura/matching/v2/misc.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/v2/model.py` & `nomenklatura-3.3.2/nomenklatura/matching/v2/model.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/v2/names.py` & `nomenklatura-3.3.2/nomenklatura/matching/v2/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/v2/train.py` & `nomenklatura-3.3.2/nomenklatura/matching/v2/train.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/matching/v2/util.py` & `nomenklatura-3.3.2/nomenklatura/matching/v2/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/publish/dates.py` & `nomenklatura-3.3.2/nomenklatura/publish/dates.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/publish/edges.py` & `nomenklatura-3.3.2/nomenklatura/publish/edges.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/publish/names.py` & `nomenklatura-3.3.2/nomenklatura/publish/names.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/resolver/edge.py` & `nomenklatura-3.3.2/nomenklatura/resolver/edge.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/resolver/identifier.py` & `nomenklatura-3.3.2/nomenklatura/resolver/identifier.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/resolver/resolver.py` & `nomenklatura-3.3.2/nomenklatura/resolver/resolver.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/senzing.py` & `nomenklatura-3.3.2/nomenklatura/senzing.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/statement/serialize.py` & `nomenklatura-3.3.2/nomenklatura/statement/serialize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import csv
-import _csv
 import click
 import orjson
 from pathlib import Path
 from io import TextIOWrapper
 from types import TracebackType
 from typing import Optional, Dict, Any, List
-from typing import BinaryIO, TextIO, Generator, Iterable, Type
+from typing import BinaryIO, Generator, Iterable, Type
 from followthemoney.cli.util import MAX_LINE
 
 from nomenklatura.statement.statement import S
 from nomenklatura.util import pack_prop, unpack_prop
 
 JSON = "json"
 CSV = "csv"
```

### Comparing `nomenklatura-3.3.1/nomenklatura/statement/statement.py` & `nomenklatura-3.3.2/nomenklatura/statement/statement.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,17 +160,17 @@
         external: Optional[bool],
     ) -> Optional[str]:
         """Hash the key properties of a statement record to make a unique ID."""
         if entity_id is None or prop is None:
             return None
         key = f"{dataset}.{entity_id}.{prop}.{value}"
         if external:
-            # We consider the external flag in key composition to avoid race conditions where
-            # a certain entity might be emitted as external while it is already linked in to
-            # the graph via another route.
+            # We consider the external flag in key composition to avoid race conditions
+            # where a certain entity might be emitted as external while it is already
+            # linked in to the graph via another route.
             key = f"{key}.ext"
         return hashlib.sha1(key.encode("utf-8")).hexdigest()
 
     @classmethod
     def from_dict(cls: Type[S], data: StatementDict) -> S:
         return cls(
             entity_id=data["entity_id"],
```

### Comparing `nomenklatura-3.3.1/nomenklatura/store/__init__.py` & `nomenklatura-3.3.2/nomenklatura/store/__init__.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/store/base.py` & `nomenklatura-3.3.2/nomenklatura/store/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from nomenklatura.dataset import DS
 from nomenklatura.resolver import Resolver, StrIdent
 from nomenklatura.statement import Statement
 from nomenklatura.entity import CE, CompositeEntity
 
 
 class Store(Generic[DS, CE]):
-    """A data storage and retrieval mechanism for statement-based entity data. Essentially,
-    this is a triple store which can be implemented using various backends."""
+    """A data storage and retrieval mechanism for statement-based entity data.
+    Essentially, this is a triple store which can be implemented using various
+    backends."""
 
     def __init__(self, dataset: DS, resolver: Resolver[CE]):
         self.dataset = dataset
         self.resolver = resolver
         self.entity_class = cast(Type[CE], CompositeEntity)
 
     def writer(self) -> "Writer[DS, CE]":
```

### Comparing `nomenklatura-3.3.1/nomenklatura/store/level.py` & `nomenklatura-3.3.2/nomenklatura/store/level.py`

 * *Files 4% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                 if entity is None:
                     continue
                 for prop, value in entity.itervalues():
                     if value == id and prop.reverse is not None:
                         yield prop.reverse, entity
 
     def entities(self) -> Generator[CE, None, None]:
-        prefix = f"e:".encode("utf-8")
+        prefix = b"e:"
         with self.store.db.iterator(prefix=prefix, include_value=False) as it:
             current_id: Optional[str] = None
             current_match = False
             for k in it:
                 _, entity_id, dataset = k.decode("utf-8").split(":", 2)
                 if entity_id != current_id:
                     current_id = entity_id
```

### Comparing `nomenklatura-3.3.1/nomenklatura/store/memory.py` & `nomenklatura-3.3.2/nomenklatura/store/memory.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/store/util.py` & `nomenklatura-3.3.2/nomenklatura/store/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/tui/app.py` & `nomenklatura-3.3.2/nomenklatura/tui/app.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/tui/comparison.py` & `nomenklatura-3.3.2/nomenklatura/tui/comparison.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/tui/util.py` & `nomenklatura-3.3.2/nomenklatura/tui/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/util.py` & `nomenklatura-3.3.2/nomenklatura/util.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura/xref.py` & `nomenklatura-3.3.2/nomenklatura/xref.py`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/nomenklatura.egg-info/PKG-INFO` & `nomenklatura-3.3.2/nomenklatura.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomenklatura
-Version: 3.3.1
+Version: 3.3.2
 Summary: Make record linkages in followthemoney data.
 Home-page: https://github.com/opensanctions/nomenklatura
 Author: Friedrich Lindenberg
 Author-email: friedrich@pudo.org
 License: MIT
 Keywords: data mapping identity followthemoney linkage record
 Platform: UNKNOWN
```

### Comparing `nomenklatura-3.3.1/nomenklatura.egg-info/SOURCES.txt` & `nomenklatura-3.3.2/nomenklatura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nomenklatura-3.3.1/setup.py` & `nomenklatura-3.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md") as f:
     long_description = f.read()
 
 
 setup(
     name="nomenklatura",
-    version="3.3.1",
+    version="3.3.2",
     description="Make record linkages in followthemoney data.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="data mapping identity followthemoney linkage record",
     author="Friedrich Lindenberg",
     author_email="friedrich@pudo.org",
     url="https://github.com/opensanctions/nomenklatura",
@@ -23,15 +23,15 @@
     install_requires=[
         "followthemoney >= 3.3.0, < 4.0.0",
         "shortuuid >= 1.0.11, < 2.0.0",
         "jellyfish >= 1.0.0, < 2.0.0",
         "rich >= 10.9.0, < 14.0.0",
         "textual >= 0.19.0, < 1.0.0",
         "scikit-learn == 1.2.2",
-        "click >= 8.0.0, < 8.1.4",
+        "click >= 8.0.0, < 8.1.6",
     ],
     tests_require=[],
     entry_points={
         "console_scripts": [
             "nk = nomenklatura.cli:cli",
             "nomenklatura = nomenklatura.cli:cli",
         ],
```

