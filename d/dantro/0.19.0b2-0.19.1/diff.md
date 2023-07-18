# Comparing `tmp/dantro-0.19.0b2.tar.gz` & `tmp/dantro-0.19.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dantro-0.19.0b2.tar", last modified: Fri Dec  9 16:49:32 2022, max compression
+gzip compressed data, was "dantro-0.19.1.tar", last modified: Tue Jul 18 11:59:50 2023, max compression
```

## Comparing `dantro-0.19.0b2.tar` & `dantro-0.19.1.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.579645 dantro-0.19.0b2/
--rw-rw-rw-   0 root         (0) root         (0)    35149 2022-12-09 16:49:20.000000 dantro-0.19.0b2/COPYING
--rw-rw-rw-   0 root         (0) root         (0)     7633 2022-12-09 16:49:20.000000 dantro-0.19.0b2/COPYING.LESSER
--rw-r--r--   0 root         (0) root         (0)     3220 2022-12-09 16:49:32.579645 dantro-0.19.0b2/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)    15686 2022-12-09 16:49:20.000000 dantro-0.19.0b2/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.555643 dantro-0.19.0b2/dantro/
--rw-rw-rw-   0 root         (0) root         (0)     1007 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      889 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/_copy.py
--rw-rw-rw-   0 root         (0) root         (0)    30886 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/_dag_utils.py
--rw-rw-rw-   0 root         (0) root         (0)      922 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/_hash.py
--rw-rw-rw-   0 root         (0) root         (0)    14740 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/_import_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     7267 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     9390 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/_yaml.py
--rw-rw-rw-   0 root         (0) root         (0)    15796 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/abc.py
--rw-rw-rw-   0 root         (0) root         (0)    44192 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.557643 dantro-0.19.0b2/dantro/cfg/
--rw-rw-rw-   0 root         (0) root         (0)    22021 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/cfg/base_plots.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.559643 dantro-0.19.0b2/dantro/containers/
--rw-rw-rw-   0 root         (0) root         (0)      545 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/containers/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3675 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/containers/_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     3223 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/containers/general.py
--rw-rw-rw-   0 root         (0) root         (0)     1302 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/containers/link.py
--rw-rw-rw-   0 root         (0) root         (0)     3409 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/containers/numeric.py
--rw-rw-rw-   0 root         (0) root         (0)     3489 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/containers/path.py
--rw-rw-rw-   0 root         (0) root         (0)    13561 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/containers/xr.py
--rw-rw-rw-   0 root         (0) root         (0)   131976 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/dag.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.562644 dantro-0.19.0b2/dantro/data_loaders/
--rw-rw-rw-   0 root         (0) root         (0)     2963 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6739 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     3786 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/fspath.py
--rw-rw-rw-   0 root         (0) root         (0)    19584 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)     2009 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/numpy.py
--rw-rw-rw-   0 root         (0) root         (0)     4230 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/pandas.py
--rw-rw-rw-   0 root         (0) root         (0)     1180 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/pickle.py
--rw-rw-rw-   0 root         (0) root         (0)      993 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/text.py
--rw-rw-rw-   0 root         (0) root         (0)     3442 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/xarray.py
--rw-rw-rw-   0 root         (0) root         (0)     2165 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_loaders/yaml.py
--rw-rw-rw-   0 root         (0) root         (0)    64943 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_mngr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.565644 dantro-0.19.0b2/dantro/data_ops/
--rw-rw-rw-   0 root         (0) root         (0)      454 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      979 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/_base_ops.py
--rw-rw-rw-   0 root         (0) root         (0)     2807 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/apply.py
--rw-rw-rw-   0 root         (0) root         (0)    28398 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/arr_ops.py
--rw-rw-rw-   0 root         (0) root         (0)     2716 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/ctrl_ops.py
--rw-rw-rw-   0 root         (0) root         (0)    16685 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/db.py
--rw-rw-rw-   0 root         (0) root         (0)     8250 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/db_tools.py
--rw-rw-rw-   0 root         (0) root         (0)     9010 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/expr_ops.py
--rw-rw-rw-   0 root         (0) root         (0)     3947 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/data_ops/hooks.py
--rw-rw-rw-   0 root         (0) root         (0)    12931 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/exceptions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.568644 dantro-0.19.0b2/dantro/groups/
--rw-rw-rw-   0 root         (0) root         (0)      601 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3497 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/_registry.py
--rw-rw-rw-   0 root         (0) root         (0)     2787 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/dirpath.py
--rw-rw-rw-   0 root         (0) root         (0)    38203 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/graph.py
--rw-rw-rw-   0 root         (0) root         (0)    46441 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/labelled.py
--rw-rw-rw-   0 root         (0) root         (0)     5143 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/ordered.py
--rw-rw-rw-   0 root         (0) root         (0)    25069 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/psp.py
--rw-rw-rw-   0 root         (0) root         (0)     2500 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/groups/time_series.py
--rw-rw-rw-   0 root         (0) root         (0)     1899 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.570644 dantro-0.19.0b2/dantro/mixins/
--rw-rw-rw-   0 root         (0) root         (0)      613 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/mixins/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    13225 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/mixins/base.py
--rw-rw-rw-   0 root         (0) root         (0)     3054 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/mixins/general.py
--rw-rw-rw-   0 root         (0) root         (0)     6696 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/mixins/indexing.py
--rw-rw-rw-   0 root         (0) root         (0)     7862 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/mixins/numeric.py
--rw-rw-rw-   0 root         (0) root         (0)     7694 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/mixins/proxy_support.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.571644 dantro-0.19.0b2/dantro/plot/
--rw-rw-rw-   0 root         (0) root         (0)      295 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10615 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/_cfg.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.572644 dantro-0.19.0b2/dantro/plot/creators/
--rw-rw-rw-   0 root         (0) root         (0)      556 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/creators/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    45845 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/creators/base.py
--rw-rw-rw-   0 root         (0) root         (0)    37576 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/creators/psp.py
--rw-rw-rw-   0 root         (0) root         (0)    24018 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/creators/pyplot.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.575645 dantro-0.19.0b2/dantro/plot/funcs/
--rw-rw-rw-   0 root         (0) root         (0)      248 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/funcs/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    10598 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/funcs/_multiplot.py
--rw-rw-rw-   0 root         (0) root         (0)     2886 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/funcs/_utils.py
--rw-rw-rw-   0 root         (0) root         (0)     1445 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/funcs/basic.py
--rw-rw-rw-   0 root         (0) root         (0)    53862 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/funcs/generic.py
--rw-rw-rw-   0 root         (0) root         (0)     9313 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/funcs/graph.py
--rw-rw-rw-   0 root         (0) root         (0)     6939 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/funcs/multiplot.py
--rw-rw-rw-   0 root         (0) root         (0)    90282 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/plot_helper.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.576645 dantro-0.19.0b2/dantro/plot/utils/
--rw-rw-rw-   0 root         (0) root         (0)      220 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3870 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/utils/_file_writer.py
--rw-rw-rw-   0 root         (0) root         (0)    41637 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/utils/color_mngr.py
--rw-rw-rw-   0 root         (0) root         (0)    11757 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/utils/mpl.py
--rw-rw-rw-   0 root         (0) root         (0)    13223 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot/utils/plot_func.py
--rw-rw-rw-   0 root         (0) root         (0)    58440 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/plot_mngr.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.577645 dantro-0.19.0b2/dantro/proxy/
--rw-rw-rw-   0 root         (0) root         (0)      142 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/proxy/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     6545 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/proxy/hdf5.py
--rw-rw-rw-   0 root         (0) root         (0)    23632 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/tools.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.579645 dantro-0.19.0b2/dantro/utils/
--rw-rw-rw-   0 root         (0) root         (0)      315 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)    21012 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/utils/coords.py
--rw-rw-rw-   0 root         (0) root         (0)     7146 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/utils/link.py
--rw-rw-rw-   0 root         (0) root         (0)    15838 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/utils/nx.py
--rw-rw-rw-   0 root         (0) root         (0)    16382 2022-12-09 16:49:20.000000 dantro-0.19.0b2/dantro/utils/ordereddict.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-12-09 16:49:32.556643 dantro-0.19.0b2/dantro.egg-info/
--rw-r--r--   0 root         (0) root         (0)     3220 2022-12-09 16:49:32.000000 dantro-0.19.0b2/dantro.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2301 2022-12-09 16:49:32.000000 dantro-0.19.0b2/dantro.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-12-09 16:49:32.000000 dantro-0.19.0b2/dantro.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      371 2022-12-09 16:49:32.000000 dantro-0.19.0b2/dantro.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2022-12-09 16:49:32.000000 dantro-0.19.0b2/dantro.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     1723 2022-12-09 16:49:20.000000 dantro-0.19.0b2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2022-12-09 16:49:32.579645 dantro-0.19.0b2/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     6012 2022-12-09 16:49:20.000000 dantro-0.19.0b2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:59:50.521653 dantro-0.19.1/
+-rw-rw-rw-   0 root         (0) root         (0)    35149 2023-07-18 11:59:39.000000 dantro-0.19.1/COPYING
+-rw-rw-rw-   0 root         (0) root         (0)     7633 2023-07-18 11:59:39.000000 dantro-0.19.1/COPYING.LESSER
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-07-18 11:59:50.521653 dantro-0.19.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)    15686 2023-07-18 11:59:39.000000 dantro-0.19.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:59:50.507653 dantro-0.19.1/dantro/
+-rw-rw-rw-   0 root         (0) root         (0)     1005 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      889 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/_copy.py
+-rw-rw-rw-   0 root         (0) root         (0)    30886 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/_dag_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)      922 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/_hash.py
+-rw-rw-rw-   0 root         (0) root         (0)    14740 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/_import_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     7267 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     9390 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/_yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)    15796 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/abc.py
+-rw-rw-rw-   0 root         (0) root         (0)    44192 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:59:50.508653 dantro-0.19.1/dantro/cfg/
+-rw-rw-rw-   0 root         (0) root         (0)    22040 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/cfg/base_plots.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:59:50.510653 dantro-0.19.1/dantro/containers/
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/containers/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3675 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/containers/_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3223 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/containers/general.py
+-rw-rw-rw-   0 root         (0) root         (0)     1302 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/containers/link.py
+-rw-rw-rw-   0 root         (0) root         (0)     3409 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/containers/numeric.py
+-rw-rw-rw-   0 root         (0) root         (0)     3489 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/containers/path.py
+-rw-rw-rw-   0 root         (0) root         (0)    13561 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/containers/xr.py
+-rw-rw-rw-   0 root         (0) root         (0)   131976 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/dag.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:59:50.512653 dantro-0.19.1/dantro/data_loaders/
+-rw-rw-rw-   0 root         (0) root         (0)     2963 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_loaders/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6739 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_loaders/_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     3786 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_loaders/fspath.py
+-rw-rw-rw-   0 root         (0) root         (0)    19584 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_loaders/hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)     2009 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_loaders/numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)     4230 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_loaders/pandas.py
+-rw-rw-rw-   0 root         (0) root         (0)     1180 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_loaders/pickle.py
+-rw-rw-rw-   0 root         (0) root         (0)      993 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_loaders/text.py
+-rw-rw-rw-   0 root         (0) root         (0)     3442 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_loaders/xarray.py
+-rw-rw-rw-   0 root         (0) root         (0)     2165 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_loaders/yaml.py
+-rw-rw-rw-   0 root         (0) root         (0)    64943 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_mngr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:59:50.513653 dantro-0.19.1/dantro/data_ops/
+-rw-rw-rw-   0 root         (0) root         (0)      454 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_ops/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1817 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_ops/_base_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)     2807 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_ops/apply.py
+-rw-rw-rw-   0 root         (0) root         (0)    28398 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_ops/arr_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)     2716 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_ops/ctrl_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)    16700 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_ops/db.py
+-rw-rw-rw-   0 root         (0) root         (0)     8250 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_ops/db_tools.py
+-rw-rw-rw-   0 root         (0) root         (0)     9010 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_ops/expr_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)     3947 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/data_ops/hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)    12931 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/exceptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:59:50.515653 dantro-0.19.1/dantro/groups/
+-rw-rw-rw-   0 root         (0) root         (0)      601 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/groups/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3497 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/groups/_registry.py
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/groups/dirpath.py
+-rw-rw-rw-   0 root         (0) root         (0)    38203 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/groups/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)    46441 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/groups/labelled.py
+-rw-rw-rw-   0 root         (0) root         (0)     5143 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/groups/ordered.py
+-rw-rw-rw-   0 root         (0) root         (0)    25069 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/groups/psp.py
+-rw-rw-rw-   0 root         (0) root         (0)     2500 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/groups/time_series.py
+-rw-rw-rw-   0 root         (0) root         (0)     1899 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:59:50.516653 dantro-0.19.1/dantro/mixins/
+-rw-rw-rw-   0 root         (0) root         (0)      613 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/mixins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    13225 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/mixins/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     3054 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/mixins/general.py
+-rw-rw-rw-   0 root         (0) root         (0)     6696 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/mixins/indexing.py
+-rw-rw-rw-   0 root         (0) root         (0)     7862 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/mixins/numeric.py
+-rw-rw-rw-   0 root         (0) root         (0)     7694 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/mixins/proxy_support.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:59:50.517653 dantro-0.19.1/dantro/plot/
+-rw-rw-rw-   0 root         (0) root         (0)      295 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10615 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/_cfg.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:59:50.517653 dantro-0.19.1/dantro/plot/creators/
+-rw-rw-rw-   0 root         (0) root         (0)      556 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/creators/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    45845 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/creators/base.py
+-rw-rw-rw-   0 root         (0) root         (0)    37576 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/creators/psp.py
+-rw-rw-rw-   0 root         (0) root         (0)    24018 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/creators/pyplot.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:59:50.519653 dantro-0.19.1/dantro/plot/funcs/
+-rw-rw-rw-   0 root         (0) root         (0)      248 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/funcs/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    10598 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/funcs/_multiplot.py
+-rw-rw-rw-   0 root         (0) root         (0)     2886 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/funcs/_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/funcs/basic.py
+-rw-rw-rw-   0 root         (0) root         (0)    53862 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/funcs/generic.py
+-rw-rw-rw-   0 root         (0) root         (0)     9313 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/funcs/graph.py
+-rw-rw-rw-   0 root         (0) root         (0)     6939 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/funcs/multiplot.py
+-rw-rw-rw-   0 root         (0) root         (0)    90275 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/plot_helper.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:59:50.520653 dantro-0.19.1/dantro/plot/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      220 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3870 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/utils/_file_writer.py
+-rw-rw-rw-   0 root         (0) root         (0)    41637 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/utils/color_mngr.py
+-rw-rw-rw-   0 root         (0) root         (0)    11758 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/utils/mpl.py
+-rw-rw-rw-   0 root         (0) root         (0)    13223 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot/utils/plot_func.py
+-rw-rw-rw-   0 root         (0) root         (0)    58440 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/plot_mngr.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:59:50.520653 dantro-0.19.1/dantro/proxy/
+-rw-rw-rw-   0 root         (0) root         (0)      142 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/proxy/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     6545 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/proxy/hdf5.py
+-rw-rw-rw-   0 root         (0) root         (0)    23632 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/tools.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:59:50.521653 dantro-0.19.1/dantro/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      315 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)    21012 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/utils/coords.py
+-rw-rw-rw-   0 root         (0) root         (0)     7146 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/utils/link.py
+-rw-rw-rw-   0 root         (0) root         (0)    15838 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/utils/nx.py
+-rw-rw-rw-   0 root         (0) root         (0)    16382 2023-07-18 11:59:39.000000 dantro-0.19.1/dantro/utils/ordereddict.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 11:59:50.508653 dantro-0.19.1/dantro.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-07-18 11:59:50.000000 dantro-0.19.1/dantro.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-07-18 11:59:50.000000 dantro-0.19.1/dantro.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 11:59:50.000000 dantro-0.19.1/dantro.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      375 2023-07-18 11:59:50.000000 dantro-0.19.1/dantro.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-07-18 11:59:50.000000 dantro-0.19.1/dantro.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     1723 2023-07-18 11:59:39.000000 dantro-0.19.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-18 11:59:50.521653 dantro-0.19.1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     6068 2023-07-18 11:59:39.000000 dantro-0.19.1/setup.py
```

### Comparing `dantro-0.19.0b2/COPYING` & `dantro-0.19.1/COPYING`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/COPYING.LESSER` & `dantro-0.19.1/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/PKG-INFO` & `dantro-0.19.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: dantro
-Version: 0.19.0b2
+Version: 0.19.1
 Summary: Handle, transform, and visualize hierarchically structured data
 Home-page: https://gitlab.com/utopia-project/dantro
 Author: dantro developers
 Author-email: dantro-dev@iup.uni.heidelberg.de
 License: LGPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.8
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: dev
 License-File: COPYING
```

### Comparing `dantro-0.19.0b2/README.md` & `dantro-0.19.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
 
 
 ### Dependencies
 `dantro` is implemented and tested for [Python >= 3.8][Python3] and depends on the following packages:
 
 | Package Name                  | Purpose                                     |
 | ----------------------------- | ------------------------------------------- |
-| [numpy][numpy]                | For fast and versatile array operations |
+| [numpy][numpy] < 2.0          | For fast and versatile array operations |
 | [xarray][xarray]              | For labelled N-dimensional arrays |
 | [dask][dask]                  | To work with large data |
 | [toolz][toolz]                | For [dask.delayed][dask-delayed]
 | [distributed][distributed]    | For distributed computing |
 | [scipy][scipy]                | As engine for NetCDF files |
 | [sympy][sympy]                | For symbolic math operations |
 | [h5py][h5py]                  | For reading HDF5 datasets |
@@ -141,15 +141,15 @@
 For more information on commit hooks, see [the commit hooks section below](#commit-hooks).
 
 
 ### Testing framework
 To assert correct functionality, tests are written alongside all features.
 The [`pytest`][pytest] and [`tox`][tox] packages are used as testing frameworks.
 
-All tests are carried out for Python 3.7 through 3.10 using the GitLab CI/CD and the newest versions of all [dependencies](#dependencies).
+All tests are carried out for Python 3.7 through 3.11 using the GitLab CI/CD and the newest versions of all [dependencies](#dependencies).
 When merging to the master branch, `dantro` is additionally tested against the specified _minimum_ versions.
 
 Test coverage and pipeline status can be seen on [the project page][dantro-project].
 
 
 #### Running tests
 To run all [defined tests](tests/), call:
@@ -232,15 +232,15 @@
 
 ## Copyright
 dantro is licensed under the [GNU Lesser General Public License Version 3][LGPLv3] or any later version.
 
 ### Copyright Notice
 
     dantro -- a python package for handling and plotting hierarchical data
-    Copyright (C) 2018 – 2022  dantro developers
+    Copyright (C) 2018 – 2023  dantro developers
 
     This program is free software: you can redistribute it and/or modify
     it under the terms of the GNU Lesser General Public License as published by
     the Free Software Foundation, either version 3 of the License, or
     (at your option) any later version.
 
     This program is distributed in the hope that it will be useful,
```

### Comparing `dantro-0.19.0b2/dantro/__init__.py` & `dantro-0.19.1/dantro/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 Together, these stages constitute a **data processing pipeline**:
 an automated sequence of predefined, configurable operations.
 
 See :ref:`the user manual <welcome>` for more information.
 """
 
-__version__ = "0.19.0b2"
+__version__ = "0.19.1"
 """Package version"""
 
 # Set up the root logger such that the logging configuration is applied
 from .logging import getLogger as _getLogger
 
 _log = _getLogger(__name__)
```

### Comparing `dantro-0.19.0b2/dantro/_copy.py` & `dantro-0.19.1/dantro/_copy.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/_dag_utils.py` & `dantro-0.19.1/dantro/_dag_utils.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/_hash.py` & `dantro-0.19.1/dantro/_hash.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/_import_tools.py` & `dantro-0.19.1/dantro/_import_tools.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/_registry.py` & `dantro-0.19.1/dantro/_registry.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/_yaml.py` & `dantro-0.19.1/dantro/_yaml.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/abc.py` & `dantro-0.19.1/dantro/abc.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/base.py` & `dantro-0.19.1/dantro/base.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/cfg/base_plots.yml` & `dantro-0.19.1/dantro/cfg/base_plots.yml`

 * *Files 0% similar despite different names*

```diff
@@ -177,14 +177,16 @@
   kind: imshow
 
 # .. Specializations: working on xr.Dataset ...................................
 .plot.facet_grid.scatter:
   based_on: .plot.facet_grid
   kind: scatter
 
+  edgecolor: none
+
 .plot.facet_grid.scatter3d:
   based_on:
     - .plot.facet_grid
     - .hlpr.projection.3d
   kind: scatter3d
 
   # For faceting, projection needs to be set via xr.plot.FacetGrid.
```

### Comparing `dantro-0.19.0b2/dantro/containers/__init__.py` & `dantro-0.19.1/dantro/containers/__init__.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/containers/_registry.py` & `dantro-0.19.1/dantro/containers/_registry.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/containers/general.py` & `dantro-0.19.1/dantro/containers/general.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/containers/link.py` & `dantro-0.19.1/dantro/containers/link.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/containers/numeric.py` & `dantro-0.19.1/dantro/containers/numeric.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/containers/path.py` & `dantro-0.19.1/dantro/containers/path.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/containers/xr.py` & `dantro-0.19.1/dantro/containers/xr.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/dag.py` & `dantro-0.19.1/dantro/dag.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_loaders/__init__.py` & `dantro-0.19.1/dantro/data_loaders/__init__.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_loaders/_registry.py` & `dantro-0.19.1/dantro/data_loaders/_registry.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_loaders/fspath.py` & `dantro-0.19.1/dantro/data_loaders/fspath.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_loaders/hdf5.py` & `dantro-0.19.1/dantro/data_loaders/hdf5.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_loaders/numpy.py` & `dantro-0.19.1/dantro/data_loaders/numpy.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_loaders/pandas.py` & `dantro-0.19.1/dantro/data_loaders/pandas.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_loaders/pickle.py` & `dantro-0.19.1/dantro/data_loaders/pickle.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_loaders/text.py` & `dantro-0.19.1/dantro/data_loaders/text.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_loaders/xarray.py` & `dantro-0.19.1/dantro/data_loaders/xarray.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_loaders/yaml.py` & `dantro-0.19.1/dantro/data_loaders/yaml.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_mngr.py` & `dantro-0.19.1/dantro/data_mngr.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_ops/apply.py` & `dantro-0.19.1/dantro/data_ops/apply.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_ops/arr_ops.py` & `dantro-0.19.1/dantro/data_ops/arr_ops.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_ops/ctrl_ops.py` & `dantro-0.19.1/dantro/data_ops/ctrl_ops.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_ops/db.py` & `dantro-0.19.1/dantro/data_ops/db.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """This module holds the data operations database"""
 
 import logging
 import math
 import operator
-from typing import Any, Callable, Dict, Iterable, List, Sequence, Tuple, Union
 
 import numpy as np
 
 from .._import_tools import (
     LazyLoader,
     get_from_module,
     import_module_or_object,
 )
 from ..exceptions import *
 from ..tools import recursive_getitem
 from ..utils.coords import extract_coords_from_attrs, extract_dim_names
 from ..utils.ordereddict import KeyOrderedDict
+from ._base_ops import BOOLEAN_OPERATORS, _make_passthrough
 from .arr_ops import *
 from .ctrl_ops import *
 from .expr_ops import *
 
 log = logging.getLogger(__name__)
 
 xr = LazyLoader("xarray")
@@ -82,21 +82,21 @@
     "complex":              complex,
     "bool":                 bool,
     "str":                  str,
 
     # Item access and manipulation
     "[]":                   lambda d, k:    d[k],
     "getitem":              lambda d, k:    d[k],
-    "setitem":              lambda d, k, v: d.__setitem__(k, v),
+    "setitem":              _make_passthrough(lambda d, *a: d.__setitem__(*a)),
     "recursive_getitem":    recursive_getitem,
 
     # Attribute-related
     ".":                    getattr,
     "getattr":              getattr,
-    "setattr":              setattr,
+    "setattr":              _make_passthrough(setattr),
     ".()":                  lambda d, attr, *a, **k: getattr(d, attr)(*a, **k),
     "callattr":             lambda d, attr, *a, **k: getattr(d, attr)(*a, **k),
 
     # Other common Python builtins
     "all":                  all,
     "any":                  any,
     "len":                  len,
```

### Comparing `dantro-0.19.0b2/dantro/data_ops/db_tools.py` & `dantro-0.19.1/dantro/data_ops/db_tools.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_ops/expr_ops.py` & `dantro-0.19.1/dantro/data_ops/expr_ops.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/data_ops/hooks.py` & `dantro-0.19.1/dantro/data_ops/hooks.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/exceptions.py` & `dantro-0.19.1/dantro/exceptions.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/groups/__init__.py` & `dantro-0.19.1/dantro/groups/__init__.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/groups/_registry.py` & `dantro-0.19.1/dantro/groups/_registry.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/groups/dirpath.py` & `dantro-0.19.1/dantro/groups/dirpath.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/groups/graph.py` & `dantro-0.19.1/dantro/groups/graph.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/groups/labelled.py` & `dantro-0.19.1/dantro/groups/labelled.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/groups/ordered.py` & `dantro-0.19.1/dantro/groups/ordered.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/groups/psp.py` & `dantro-0.19.1/dantro/groups/psp.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/groups/time_series.py` & `dantro-0.19.1/dantro/groups/time_series.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/logging.py` & `dantro-0.19.1/dantro/logging.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/mixins/__init__.py` & `dantro-0.19.1/dantro/mixins/__init__.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/mixins/base.py` & `dantro-0.19.1/dantro/mixins/base.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/mixins/general.py` & `dantro-0.19.1/dantro/mixins/general.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/mixins/indexing.py` & `dantro-0.19.1/dantro/mixins/indexing.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/mixins/numeric.py` & `dantro-0.19.1/dantro/mixins/numeric.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/mixins/proxy_support.py` & `dantro-0.19.1/dantro/mixins/proxy_support.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/plot/_cfg.py` & `dantro-0.19.1/dantro/plot/_cfg.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/plot/creators/__init__.py` & `dantro-0.19.1/dantro/plot/creators/__init__.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/plot/creators/base.py` & `dantro-0.19.1/dantro/plot/creators/base.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/plot/creators/psp.py` & `dantro-0.19.1/dantro/plot/creators/psp.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/plot/creators/pyplot.py` & `dantro-0.19.1/dantro/plot/creators/pyplot.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/plot/funcs/_multiplot.py` & `dantro-0.19.1/dantro/plot/funcs/_multiplot.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/plot/funcs/_utils.py` & `dantro-0.19.1/dantro/plot/funcs/_utils.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/plot/funcs/basic.py` & `dantro-0.19.1/dantro/plot/funcs/basic.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/plot/funcs/generic.py` & `dantro-0.19.1/dantro/plot/funcs/generic.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/plot/funcs/graph.py` & `dantro-0.19.1/dantro/plot/funcs/graph.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/plot/funcs/multiplot.py` & `dantro-0.19.1/dantro/plot/funcs/multiplot.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/plot/plot_helper.py` & `dantro-0.19.1/dantro/plot/plot_helper.py`

 * *Files 0% similar despite different names*

```diff
@@ -3731,1913 +3731,1913 @@
 0000e920: 2062 6520 7369 6c65 6e74 6c79 2069 676e   be silently ign
 0000e930: 6f72 6564 2e0a 2020 2020 2020 2020 2020  ored..          
 0000e940: 2020 6f6e 6c79 5f6c 6162 656c 5f6f 7574    only_label_out
 0000e950: 6572 2028 626f 6f6c 2c20 6f70 7469 6f6e  er (bool, option
 0000e960: 616c 293a 2049 6620 5472 7565 2c20 6361  al): If True, ca
 0000e970: 6c6c 0a20 2020 2020 2020 2020 2020 2020  ll.             
 0000e980: 2020 203a 7079 3a6d 6574 683a 606d 6174     :py:meth:`mat
-0000e990: 706c 6f74 6c69 622e 6178 6573 2e53 7562  plotlib.axes.Sub
-0000e9a0: 706c 6f74 4261 7365 2e6c 6162 656c 5f6f  plotBase.label_o
-0000e9b0: 7574 6572 6020 7375 6368 2074 6861 740a  uter` such that.
-0000e9c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000e9d0: 6f6e 6c79 2074 6963 6b20 6c61 6265 6c73  only tick labels
-0000e9e0: 206f 6e20 226f 7574 6572 2220 6178 6573   on "outer" axes
-0000e9f0: 2061 7265 2076 6973 6962 6c65 3a0a 2020   are visible:.  
-0000ea00: 2020 2020 2020 2020 2020 2020 2020 782d                x-
-0000ea10: 6c61 6265 6c73 2061 7265 206f 6e6c 7920  labels are only 
-0000ea20: 6b65 7074 2066 6f72 2073 7562 706c 6f74  kept for subplot
-0000ea30: 7320 6f6e 2074 6865 206c 6173 7420 726f  s on the last ro
-0000ea40: 773b 2079 2d6c 6162 656c 730a 2020 2020  w; y-labels.    
-0000ea50: 2020 2020 2020 2020 2020 2020 6f6e 6c79              only
-0000ea60: 2066 6f72 2073 7562 706c 6f74 7320 6f6e   for subplots on
-0000ea70: 2074 6865 2066 6972 7374 2063 6f6c 756d   the first colum
-0000ea80: 6e2e 204e 6f74 6520 7468 6174 2074 6869  n. Note that thi
-0000ea90: 7320 6170 706c 6965 730a 2020 2020 2020  s applies.      
-0000eaa0: 2020 2020 2020 2020 2020 746f 2062 6f74            to bot
-0000eab0: 6820 6178 6573 2061 6e64 206d 6179 206c  h axes and may l
-0000eac0: 6561 6420 746f 2065 7869 7374 696e 6720  ead to existing 
-0000ead0: 6178 6573 2062 6569 6e67 2068 6964 6465  axes being hidde
-0000eae0: 6e2e 0a20 2020 2020 2020 2020 2020 2072  n..            r
-0000eaf0: 6f74 6174 655f 7a5f 6c61 6265 6c20 2862  otate_z_label (b
-0000eb00: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
-0000eb10: 4966 2067 6976 656e 2c20 7365 7473 0a20  If given, sets. 
-0000eb20: 2020 2020 2020 2020 2020 2020 2020 203a                 :
-0000eb30: 7079 3a6d 6574 683a 606d 706c 5f74 6f6f  py:meth:`mpl_too
-0000eb40: 6c6b 6974 732e 6d70 6c6f 7433 642e 6178  lkits.mplot3d.ax
-0000eb50: 6973 3364 2e41 7869 732e 7365 745f 726f  is3d.Axis.set_ro
-0000eb60: 7461 7465 5f6c 6162 656c 602e 0a20 2020  tate_label`..   
-0000eb70: 2020 2020 2020 2020 2020 2020 2049 6620               If 
-0000eb80: 7468 6572 6520 6973 206e 6f20 7a2d 6178  there is no z-ax
-0000eb90: 6973 2c20 7468 6973 2077 696c 6c20 6265  is, this will be
-0000eba0: 2073 696c 656e 746c 7920 6967 6e6f 7265   silently ignore
-0000ebb0: 642e 0a20 2020 2020 2020 2022 2222 0a0a  d..        """..
-0000ebc0: 2020 2020 2020 2020 6465 6620 7365 745f          def set_
-0000ebd0: 6c61 6265 6c28 6675 6e63 3a20 4361 6c6c  label(func: Call
-0000ebe0: 6162 6c65 2c20 2a2c 206c 6162 656c 3a20  able, *, label: 
-0000ebf0: 7374 7220 3d20 4e6f 6e65 2c20 2a2a 6c61  str = None, **la
-0000ec00: 6265 6c5f 6b77 6172 6773 293a 0a20 2020  bel_kwargs):.   
-0000ec10: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000ec20: 6675 6e63 286c 6162 656c 2c20 2a2a 6c61  func(label, **la
-0000ec30: 6265 6c5f 6b77 6172 6773 290a 0a20 2020  bel_kwargs)..   
-0000ec40: 2020 2020 2069 6620 783a 0a20 2020 2020       if x:.     
-0000ec50: 2020 2020 2020 2078 203d 2078 2069 6620         x = x if 
-0000ec60: 6e6f 7420 6973 696e 7374 616e 6365 2878  not isinstance(x
-0000ec70: 2c20 7374 7229 2065 6c73 6520 6469 6374  , str) else dict
-0000ec80: 286c 6162 656c 3d78 290a 2020 2020 2020  (label=x).      
-0000ec90: 2020 2020 2020 7365 745f 6c61 6265 6c28        set_label(
-0000eca0: 7365 6c66 2e61 782e 7365 745f 786c 6162  self.ax.set_xlab
-0000ecb0: 656c 2c20 2a2a 7829 0a0a 2020 2020 2020  el, **x)..      
-0000ecc0: 2020 6966 2079 3a0a 2020 2020 2020 2020    if y:.        
-0000ecd0: 2020 2020 7920 3d20 7920 6966 206e 6f74      y = y if not
-0000ece0: 2069 7369 6e73 7461 6e63 6528 792c 2073   isinstance(y, s
-0000ecf0: 7472 2920 656c 7365 2064 6963 7428 6c61  tr) else dict(la
-0000ed00: 6265 6c3d 7929 0a20 2020 2020 2020 2020  bel=y).         
-0000ed10: 2020 2073 6574 5f6c 6162 656c 2873 656c     set_label(sel
-0000ed20: 662e 6178 2e73 6574 5f79 6c61 6265 6c2c  f.ax.set_ylabel,
-0000ed30: 202a 2a79 290a 0a20 2020 2020 2020 2069   **y)..        i
-0000ed40: 6620 6861 7361 7474 7228 7365 6c66 2e61  f hasattr(self.a
-0000ed50: 782c 2022 7a61 7869 7322 293a 0a20 2020  x, "zaxis"):.   
-0000ed60: 2020 2020 2020 2020 2069 6620 7a3a 0a20           if z:. 
-0000ed70: 2020 2020 2020 2020 2020 2020 2020 207a                 z
-0000ed80: 203d 207a 2069 6620 6e6f 7420 6973 696e   = z if not isin
-0000ed90: 7374 616e 6365 287a 2c20 7374 7229 2065  stance(z, str) e
-0000eda0: 6c73 6520 6469 6374 286c 6162 656c 3d7a  lse dict(label=z
-0000edb0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000edc0: 2020 7365 745f 6c61 6265 6c28 7365 6c66    set_label(self
-0000edd0: 2e61 782e 7365 745f 7a6c 6162 656c 2c20  .ax.set_zlabel, 
-0000ede0: 2a2a 7a29 0a0a 2020 2020 2020 2020 2020  **z)..          
-0000edf0: 2020 6966 2072 6f74 6174 655f 7a5f 6c61    if rotate_z_la
-0000ee00: 6265 6c20 6973 206e 6f74 204e 6f6e 653a  bel is not None:
-0000ee10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000ee20: 2073 656c 662e 6178 2e7a 6178 6973 2e73   self.ax.zaxis.s
-0000ee30: 6574 5f72 6f74 6174 655f 6c61 6265 6c28  et_rotate_label(
-0000ee40: 726f 7461 7465 5f7a 5f6c 6162 656c 290a  rotate_z_label).
-0000ee50: 0a20 2020 2020 2020 2069 6620 6f6e 6c79  .        if only
-0000ee60: 5f6c 6162 656c 5f6f 7574 6572 3a0a 2020  _label_outer:.  
-0000ee70: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
-0000ee80: 782e 6c61 6265 6c5f 6f75 7465 7228 290a  x.label_outer().
-0000ee90: 0a20 2020 2064 6566 205f 686c 7072 5f73  .    def _hlpr_s
-0000eea0: 6574 5f6c 696d 6974 7328 0a20 2020 2020  et_limits(.     
-0000eeb0: 2020 2073 656c 662c 0a20 2020 2020 2020     self,.       
-0000eec0: 202a 2c0a 2020 2020 2020 2020 783a 2055   *,.        x: U
-0000eed0: 6e69 6f6e 5b53 6571 7565 6e63 655b 556e  nion[Sequence[Un
-0000eee0: 696f 6e5b 666c 6f61 742c 2073 7472 5d5d  ion[float, str]]
-0000eef0: 2c20 6469 6374 5d20 3d20 4e6f 6e65 2c0a  , dict] = None,.
-0000ef00: 2020 2020 2020 2020 793a 2055 6e69 6f6e          y: Union
-0000ef10: 5b53 6571 7565 6e63 655b 556e 696f 6e5b  [Sequence[Union[
-0000ef20: 666c 6f61 742c 2073 7472 5d5d 2c20 6469  float, str]], di
-0000ef30: 6374 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ct] = None,.    
-0000ef40: 2020 2020 7a3a 2055 6e69 6f6e 5b53 6571      z: Union[Seq
-0000ef50: 7565 6e63 655b 556e 696f 6e5b 666c 6f61  uence[Union[floa
-0000ef60: 742c 2073 7472 5d5d 2c20 6469 6374 5d20  t, str]], dict] 
-0000ef70: 3d20 4e6f 6e65 2c0a 2020 2020 293a 0a20  = None,.    ):. 
-0000ef80: 2020 2020 2020 2022 2222 5365 7473 2074         """Sets t
-0000ef90: 6865 2078 2c20 792c 2061 6e64 207a 206c  he x, y, and z l
-0000efa0: 696d 6974 7320 666f 7220 7468 6520 6375  imits for the cu
-0000efb0: 7272 656e 7420 6178 6973 2e20 416c 6c6f  rrent axis. Allo
-0000efc0: 7773 2073 6f6d 650a 2020 2020 2020 2020  ws some.        
-0000efd0: 636f 6e76 656e 6965 6e63 6520 6465 6669  convenience defi
-0000efe0: 6e69 7469 6f6e 7320 666f 7220 7468 6520  nitions for the 
-0000eff0: 6172 6775 6d65 6e74 7320 616e 6420 7468  arguments and th
-0000f000: 656e 2063 616c 6c73 0a20 2020 2020 2020  en calls.       
-0000f010: 203a 7079 3a6d 6574 683a 606d 6174 706c   :py:meth:`matpl
-0000f020: 6f74 6c69 622e 6178 6573 2e41 7865 732e  otlib.axes.Axes.
-0000f030: 7365 745f 786c 696d 6020 616e 642f 6f72  set_xlim` and/or
-0000f040: 0a20 2020 2020 2020 203a 7079 3a6d 6574  .        :py:met
-0000f050: 683a 606d 6174 706c 6f74 6c69 622e 6178  h:`matplotlib.ax
-0000f060: 6573 2e41 7865 732e 7365 745f 796c 696d  es.Axes.set_ylim
-0000f070: 602e 0a20 2020 2020 2020 203a 7079 3a6d  `..        :py:m
-0000f080: 6574 683a 606d 706c 5f74 6f6f 6c6b 6974  eth:`mpl_toolkit
-0000f090: 732e 6d70 6c6f 7433 642e 6178 6573 3364  s.mplot3d.axes3d
-0000f0a0: 2e41 7865 7333 442e 7365 745f 7a6c 696d  .Axes3D.set_zlim
-0000f0b0: 602e 0a0a 2020 2020 2020 2020 5468 6520  `...        The 
-0000f0c0: 6060 7860 602c 2060 6079 6060 2c20 616e  ``x``, ``y``, an
-0000f0d0: 6420 6060 7a60 6020 6172 6775 6d65 6e74  d ``z`` argument
-0000f0e0: 7320 6361 6e20 6861 7665 2074 6865 2066  s can have the f
-0000f0f0: 6f6c 6c6f 7769 6e67 2066 6f72 6d3a 0a0a  ollowing form:..
-0000f100: 2020 2020 2020 2020 2020 2020 2d20 4e6f              - No
-0000f110: 6e65 3a20 2020 2020 2020 2020 4c69 6d69  ne:         Limi
-0000f120: 7473 2061 7265 206e 6f74 2073 6574 0a20  ts are not set. 
-0000f130: 2020 2020 2020 2020 2020 202d 2073 6571             - seq
-0000f140: 7565 6e63 653a 2020 2020 2053 7065 6369  uence:     Speci
-0000f150: 6679 206c 6f77 6572 2061 6e64 2075 7070  fy lower and upp
-0000f160: 6572 2076 616c 7565 730a 2020 2020 2020  er values.      
-0000f170: 2020 2020 2020 2d20 6469 6374 3a20 2020        - dict:   
-0000f180: 2020 2020 2020 4578 7065 6374 696e 6720        Expecting 
-0000f190: 6b65 7973 2060 606c 6f77 6572 6060 2061  keys ``lower`` a
-0000f1a0: 6e64 2f6f 7220 6060 7570 7065 7260 600a  nd/or ``upper``.
-0000f1b0: 0a20 2020 2020 2020 2054 6865 2073 6571  .        The seq
-0000f1c0: 7565 6e63 6520 6f72 2064 6963 7420 7661  uence or dict va
-0000f1d0: 6c75 6573 2063 616e 2062 653a 0a0a 2020  lues can be:..  
-0000f1e0: 2020 2020 2020 2020 2020 2d20 4e6f 6e65            - None
-0000f1f0: 2020 2020 2020 2020 2020 5365 7420 6175            Set au
-0000f200: 746f 6d61 7469 6361 6c6c 7920 2f20 646f  tomatically / do
-0000f210: 206e 6f74 2073 6574 0a20 2020 2020 2020   not set.       
-0000f220: 2020 2020 202d 206e 756d 6572 6963 2020       - numeric  
-0000f230: 2020 2020 2053 6574 2074 6f20 7468 6973       Set to this
-0000f240: 2076 616c 7565 2065 7870 6c69 6369 746c   value explicitl
-0000f250: 790a 2020 2020 2020 2020 2020 2020 2d20  y.            - 
-0000f260: 6060 6d69 6e60 6020 2020 2020 2020 5365  ``min``       Se
-0000f270: 7420 746f 2074 6865 2064 6174 6120 6d69  t to the data mi
-0000f280: 6e69 6d75 6d20 7661 6c75 6520 6f6e 2074  nimum value on t
-0000f290: 6861 7420 6178 6973 0a20 2020 2020 2020  hat axis.       
-0000f2a0: 2020 2020 202d 2060 606d 6178 6060 2020       - ``max``  
-0000f2b0: 2020 2020 2053 6574 2074 6f20 7468 6520       Set to the 
-0000f2c0: 6461 7461 206d 6178 696d 756d 2076 616c  data maximum val
-0000f2d0: 7565 206f 6e20 7468 6174 2061 7869 730a  ue on that axis.
-0000f2e0: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-0000f2f0: 2020 2020 2020 2020 2020 2078 2028 556e             x (Un
-0000f300: 696f 6e5b 5365 7175 656e 6365 5b55 6e69  ion[Sequence[Uni
-0000f310: 6f6e 5b66 6c6f 6174 2c20 7374 725d 5d2c  on[float, str]],
-0000f320: 2064 6963 745d 2c20 6f70 7469 6f6e 616c   dict], optional
-0000f330: 293a 2054 6865 206c 696d 6974 730a 2020  ): The limits.  
-0000f340: 2020 2020 2020 2020 2020 2020 2020 746f                to
-0000f350: 2073 6574 206f 6e20 7468 6520 782d 6178   set on the x-ax
-0000f360: 6973 0a20 2020 2020 2020 2020 2020 2079  is.            y
-0000f370: 2028 556e 696f 6e5b 5365 7175 656e 6365   (Union[Sequence
-0000f380: 5b55 6e69 6f6e 5b66 6c6f 6174 2c20 7374  [Union[float, st
-0000f390: 725d 5d2c 2064 6963 745d 2c20 6f70 7469  r]], dict], opti
-0000f3a0: 6f6e 616c 293a 2054 6865 206c 696d 6974  onal): The limit
-0000f3b0: 730a 2020 2020 2020 2020 2020 2020 2020  s.              
-0000f3c0: 2020 746f 2073 6574 206f 6e20 7468 6520    to set on the 
-0000f3d0: 792d 6178 6973 0a20 2020 2020 2020 2020  y-axis.         
-0000f3e0: 2020 207a 2028 556e 696f 6e5b 5365 7175     z (Union[Sequ
-0000f3f0: 656e 6365 5b55 6e69 6f6e 5b66 6c6f 6174  ence[Union[float
-0000f400: 2c20 7374 725d 5d2c 2064 6963 745d 2c20  , str]], dict], 
-0000f410: 6f70 7469 6f6e 616c 293a 2054 6865 206c  optional): The l
-0000f420: 696d 6974 730a 2020 2020 2020 2020 2020  imits.          
-0000f430: 2020 2020 2020 746f 2073 6574 206f 6e20        to set on 
-0000f440: 7468 6520 7a2d 6178 6973 0a20 2020 2020  the z-axis.     
-0000f450: 2020 2020 2020 2020 2020 2049 6620 7468             If th
-0000f460: 6572 6520 6973 206e 6f20 7a2d 6178 6973  ere is no z-axis
-0000f470: 2c20 7468 6973 2077 696c 6c20 6265 2073  , this will be s
-0000f480: 696c 656e 746c 7920 6967 6e6f 7265 642e  ilently ignored.
-0000f490: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-0000f4a0: 2020 2020 2020 6465 6620 7061 7273 655f        def parse_
-0000f4b0: 6172 6773 280a 2020 2020 2020 2020 2020  args(.          
-0000f4c0: 2020 6172 6773 3a20 556e 696f 6e5b 5365    args: Union[Se
-0000f4d0: 7175 656e 6365 5b55 6e69 6f6e 5b66 6c6f  quence[Union[flo
-0000f4e0: 6174 2c20 7374 725d 5d2c 2064 6963 745d  at, str]], dict]
-0000f4f0: 2c20 2a2c 2061 780a 2020 2020 2020 2020  , *, ax.        
-0000f500: 2920 2d3e 2054 7570 6c65 5b66 6c6f 6174  ) -> Tuple[float
-0000f510: 2c20 666c 6f61 745d 3a0a 2020 2020 2020  , float]:.      
-0000f520: 2020 2020 2020 2222 2250 6172 7365 7320        """Parses 
-0000f530: 7468 6520 6c69 6d69 7420 6172 6775 6d65  the limit argume
-0000f540: 6e74 732e 2222 220a 0a20 2020 2020 2020  nts."""..       
-0000f550: 2020 2020 2064 6566 2070 6172 7365 5f61       def parse_a
-0000f560: 7267 2861 7267 3a20 556e 696f 6e5b 666c  rg(arg: Union[fl
-0000f570: 6f61 742c 2073 7472 5d29 202d 3e20 556e  oat, str]) -> Un
-0000f580: 696f 6e5b 666c 6f61 742c 204e 6f6e 655d  ion[float, None]
-0000f590: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-0000f5a0: 2020 2222 2250 6172 7365 7320 6120 7369    """Parses a si
-0000f5b0: 6e67 6c65 206c 696d 6974 2061 7267 756d  ngle limit argum
-0000f5c0: 656e 7420 746f 2065 6974 6865 7220 6265  ent to either be
-0000f5d0: 2066 6c6f 6174 206f 7220 4e6f 6e65 2222   float or None""
-0000f5e0: 220a 2020 2020 2020 2020 2020 2020 2020  ".              
-0000f5f0: 2020 6966 206e 6f74 2069 7369 6e73 7461    if not isinsta
-0000f600: 6e63 6528 6172 672c 2073 7472 293a 0a20  nce(arg, str):. 
-0000f610: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f620: 2020 2023 204e 6f74 6869 6e67 2074 6f20     # Nothing to 
-0000f630: 7061 7273 650a 2020 2020 2020 2020 2020  parse.          
-0000f640: 2020 2020 2020 2020 2020 7265 7475 726e            return
-0000f650: 2061 7267 0a0a 2020 2020 2020 2020 2020   arg..          
-0000f660: 2020 2020 2020 6966 2061 7267 203d 3d20        if arg == 
-0000f670: 226d 696e 223a 0a20 2020 2020 2020 2020  "min":.         
-0000f680: 2020 2020 2020 2020 2020 2061 7267 203d             arg =
-0000f690: 2061 782e 6765 745f 6461 7461 5f69 6e74   ax.get_data_int
-0000f6a0: 6572 7661 6c28 295b 305d 0a20 2020 2020  erval()[0].     
-0000f6b0: 2020 2020 2020 2020 2020 2065 6c69 6620             elif 
-0000f6c0: 6172 6720 3d3d 2022 6d61 7822 3a0a 2020  arg == "max":.  
-0000f6d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f6e0: 2020 6172 6720 3d20 6178 2e67 6574 5f64    arg = ax.get_d
-0000f6f0: 6174 615f 696e 7465 7276 616c 2829 5b31  ata_interval()[1
-0000f700: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
-0000f710: 2020 656c 7365 3a0a 2020 2020 2020 2020    else:.        
-0000f720: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000f730: 6520 506c 6f74 436f 6e66 6967 4572 726f  e PlotConfigErro
-0000f740: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-0000f750: 2020 2020 2020 2020 2020 2066 2247 6f74             f"Got
-0000f760: 2061 6e20 696e 7661 6c69 6420 7374 722d   an invalid str-
-0000f770: 7479 7065 2061 7267 756d 656e 7420 277b  type argument '{
-0000f780: 6172 677d 2720 746f 2074 6865 2022 0a20  arg}' to the ". 
+0000e990: 706c 6f74 6c69 622e 6178 6573 2e41 7865  plotlib.axes.Axe
+0000e9a0: 732e 6c61 6265 6c5f 6f75 7465 7260 2073  s.label_outer` s
+0000e9b0: 7563 6820 7468 6174 0a20 2020 2020 2020  uch that.       
+0000e9c0: 2020 2020 2020 2020 206f 6e6c 7920 7469           only ti
+0000e9d0: 636b 206c 6162 656c 7320 6f6e 2022 6f75  ck labels on "ou
+0000e9e0: 7465 7222 2061 7865 7320 6172 6520 7669  ter" axes are vi
+0000e9f0: 7369 626c 653a 0a20 2020 2020 2020 2020  sible:.         
+0000ea00: 2020 2020 2020 2078 2d6c 6162 656c 7320         x-labels 
+0000ea10: 6172 6520 6f6e 6c79 206b 6570 7420 666f  are only kept fo
+0000ea20: 7220 7375 6270 6c6f 7473 206f 6e20 7468  r subplots on th
+0000ea30: 6520 6c61 7374 2072 6f77 3b20 792d 6c61  e last row; y-la
+0000ea40: 6265 6c73 0a20 2020 2020 2020 2020 2020  bels.           
+0000ea50: 2020 2020 206f 6e6c 7920 666f 7220 7375       only for su
+0000ea60: 6270 6c6f 7473 206f 6e20 7468 6520 6669  bplots on the fi
+0000ea70: 7273 7420 636f 6c75 6d6e 2e20 4e6f 7465  rst column. Note
+0000ea80: 2074 6861 7420 7468 6973 2061 7070 6c69   that this appli
+0000ea90: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+0000eaa0: 2020 2074 6f20 626f 7468 2061 7865 7320     to both axes 
+0000eab0: 616e 6420 6d61 7920 6c65 6164 2074 6f20  and may lead to 
+0000eac0: 6578 6973 7469 6e67 2061 7865 7320 6265  existing axes be
+0000ead0: 696e 6720 6869 6464 656e 2e0a 2020 2020  ing hidden..    
+0000eae0: 2020 2020 2020 2020 726f 7461 7465 5f7a          rotate_z
+0000eaf0: 5f6c 6162 656c 2028 626f 6f6c 2c20 6f70  _label (bool, op
+0000eb00: 7469 6f6e 616c 293a 2049 6620 6769 7665  tional): If give
+0000eb10: 6e2c 2073 6574 730a 2020 2020 2020 2020  n, sets.        
+0000eb20: 2020 2020 2020 2020 3a70 793a 6d65 7468          :py:meth
+0000eb30: 3a60 6d70 6c5f 746f 6f6c 6b69 7473 2e6d  :`mpl_toolkits.m
+0000eb40: 706c 6f74 3364 2e61 7869 7333 642e 4178  plot3d.axis3d.Ax
+0000eb50: 6973 2e73 6574 5f72 6f74 6174 655f 6c61  is.set_rotate_la
+0000eb60: 6265 6c60 2e0a 2020 2020 2020 2020 2020  bel`..          
+0000eb70: 2020 2020 2020 4966 2074 6865 7265 2069        If there i
+0000eb80: 7320 6e6f 207a 2d61 7869 732c 2074 6869  s no z-axis, thi
+0000eb90: 7320 7769 6c6c 2062 6520 7369 6c65 6e74  s will be silent
+0000eba0: 6c79 2069 676e 6f72 6564 2e0a 2020 2020  ly ignored..    
+0000ebb0: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
+0000ebc0: 2064 6566 2073 6574 5f6c 6162 656c 2866   def set_label(f
+0000ebd0: 756e 633a 2043 616c 6c61 626c 652c 202a  unc: Callable, *
+0000ebe0: 2c20 6c61 6265 6c3a 2073 7472 203d 204e  , label: str = N
+0000ebf0: 6f6e 652c 202a 2a6c 6162 656c 5f6b 7761  one, **label_kwa
+0000ec00: 7267 7329 3a0a 2020 2020 2020 2020 2020  rgs):.          
+0000ec10: 2020 7265 7475 726e 2066 756e 6328 6c61    return func(la
+0000ec20: 6265 6c2c 202a 2a6c 6162 656c 5f6b 7761  bel, **label_kwa
+0000ec30: 7267 7329 0a0a 2020 2020 2020 2020 6966  rgs)..        if
+0000ec40: 2078 3a0a 2020 2020 2020 2020 2020 2020   x:.            
+0000ec50: 7820 3d20 7820 6966 206e 6f74 2069 7369  x = x if not isi
+0000ec60: 6e73 7461 6e63 6528 782c 2073 7472 2920  nstance(x, str) 
+0000ec70: 656c 7365 2064 6963 7428 6c61 6265 6c3d  else dict(label=
+0000ec80: 7829 0a20 2020 2020 2020 2020 2020 2073  x).            s
+0000ec90: 6574 5f6c 6162 656c 2873 656c 662e 6178  et_label(self.ax
+0000eca0: 2e73 6574 5f78 6c61 6265 6c2c 202a 2a78  .set_xlabel, **x
+0000ecb0: 290a 0a20 2020 2020 2020 2069 6620 793a  )..        if y:
+0000ecc0: 0a20 2020 2020 2020 2020 2020 2079 203d  .            y =
+0000ecd0: 2079 2069 6620 6e6f 7420 6973 696e 7374   y if not isinst
+0000ece0: 616e 6365 2879 2c20 7374 7229 2065 6c73  ance(y, str) els
+0000ecf0: 6520 6469 6374 286c 6162 656c 3d79 290a  e dict(label=y).
+0000ed00: 2020 2020 2020 2020 2020 2020 7365 745f              set_
+0000ed10: 6c61 6265 6c28 7365 6c66 2e61 782e 7365  label(self.ax.se
+0000ed20: 745f 796c 6162 656c 2c20 2a2a 7929 0a0a  t_ylabel, **y)..
+0000ed30: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
+0000ed40: 7472 2873 656c 662e 6178 2c20 227a 6178  tr(self.ax, "zax
+0000ed50: 6973 2229 3a0a 2020 2020 2020 2020 2020  is"):.          
+0000ed60: 2020 6966 207a 3a0a 2020 2020 2020 2020    if z:.        
+0000ed70: 2020 2020 2020 2020 7a20 3d20 7a20 6966          z = z if
+0000ed80: 206e 6f74 2069 7369 6e73 7461 6e63 6528   not isinstance(
+0000ed90: 7a2c 2073 7472 2920 656c 7365 2064 6963  z, str) else dic
+0000eda0: 7428 6c61 6265 6c3d 7a29 0a20 2020 2020  t(label=z).     
+0000edb0: 2020 2020 2020 2020 2020 2073 6574 5f6c             set_l
+0000edc0: 6162 656c 2873 656c 662e 6178 2e73 6574  abel(self.ax.set
+0000edd0: 5f7a 6c61 6265 6c2c 202a 2a7a 290a 0a20  _zlabel, **z).. 
+0000ede0: 2020 2020 2020 2020 2020 2069 6620 726f             if ro
+0000edf0: 7461 7465 5f7a 5f6c 6162 656c 2069 7320  tate_z_label is 
+0000ee00: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000ee10: 2020 2020 2020 2020 2020 7365 6c66 2e61            self.a
+0000ee20: 782e 7a61 7869 732e 7365 745f 726f 7461  x.zaxis.set_rota
+0000ee30: 7465 5f6c 6162 656c 2872 6f74 6174 655f  te_label(rotate_
+0000ee40: 7a5f 6c61 6265 6c29 0a0a 2020 2020 2020  z_label)..      
+0000ee50: 2020 6966 206f 6e6c 795f 6c61 6265 6c5f    if only_label_
+0000ee60: 6f75 7465 723a 0a20 2020 2020 2020 2020  outer:.         
+0000ee70: 2020 2073 656c 662e 6178 2e6c 6162 656c     self.ax.label
+0000ee80: 5f6f 7574 6572 2829 0a0a 2020 2020 6465  _outer()..    de
+0000ee90: 6620 5f68 6c70 725f 7365 745f 6c69 6d69  f _hlpr_set_limi
+0000eea0: 7473 280a 2020 2020 2020 2020 7365 6c66  ts(.        self
+0000eeb0: 2c0a 2020 2020 2020 2020 2a2c 0a20 2020  ,.        *,.   
+0000eec0: 2020 2020 2078 3a20 556e 696f 6e5b 5365       x: Union[Se
+0000eed0: 7175 656e 6365 5b55 6e69 6f6e 5b66 6c6f  quence[Union[flo
+0000eee0: 6174 2c20 7374 725d 5d2c 2064 6963 745d  at, str]], dict]
+0000eef0: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
+0000ef00: 2079 3a20 556e 696f 6e5b 5365 7175 656e   y: Union[Sequen
+0000ef10: 6365 5b55 6e69 6f6e 5b66 6c6f 6174 2c20  ce[Union[float, 
+0000ef20: 7374 725d 5d2c 2064 6963 745d 203d 204e  str]], dict] = N
+0000ef30: 6f6e 652c 0a20 2020 2020 2020 207a 3a20  one,.        z: 
+0000ef40: 556e 696f 6e5b 5365 7175 656e 6365 5b55  Union[Sequence[U
+0000ef50: 6e69 6f6e 5b66 6c6f 6174 2c20 7374 725d  nion[float, str]
+0000ef60: 5d2c 2064 6963 745d 203d 204e 6f6e 652c  ], dict] = None,
+0000ef70: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
+0000ef80: 2222 2253 6574 7320 7468 6520 782c 2079  """Sets the x, y
+0000ef90: 2c20 616e 6420 7a20 6c69 6d69 7473 2066  , and z limits f
+0000efa0: 6f72 2074 6865 2063 7572 7265 6e74 2061  or the current a
+0000efb0: 7869 732e 2041 6c6c 6f77 7320 736f 6d65  xis. Allows some
+0000efc0: 0a20 2020 2020 2020 2063 6f6e 7665 6e69  .        conveni
+0000efd0: 656e 6365 2064 6566 696e 6974 696f 6e73  ence definitions
+0000efe0: 2066 6f72 2074 6865 2061 7267 756d 656e   for the argumen
+0000eff0: 7473 2061 6e64 2074 6865 6e20 6361 6c6c  ts and then call
+0000f000: 730a 2020 2020 2020 2020 3a70 793a 6d65  s.        :py:me
+0000f010: 7468 3a60 6d61 7470 6c6f 746c 6962 2e61  th:`matplotlib.a
+0000f020: 7865 732e 4178 6573 2e73 6574 5f78 6c69  xes.Axes.set_xli
+0000f030: 6d60 2061 6e64 2f6f 720a 2020 2020 2020  m` and/or.      
+0000f040: 2020 3a70 793a 6d65 7468 3a60 6d61 7470    :py:meth:`matp
+0000f050: 6c6f 746c 6962 2e61 7865 732e 4178 6573  lotlib.axes.Axes
+0000f060: 2e73 6574 5f79 6c69 6d60 2e0a 2020 2020  .set_ylim`..    
+0000f070: 2020 2020 3a70 793a 6d65 7468 3a60 6d70      :py:meth:`mp
+0000f080: 6c5f 746f 6f6c 6b69 7473 2e6d 706c 6f74  l_toolkits.mplot
+0000f090: 3364 2e61 7865 7333 642e 4178 6573 3344  3d.axes3d.Axes3D
+0000f0a0: 2e73 6574 5f7a 6c69 6d60 2e0a 0a20 2020  .set_zlim`...   
+0000f0b0: 2020 2020 2054 6865 2060 6078 6060 2c20       The ``x``, 
+0000f0c0: 6060 7960 602c 2061 6e64 2060 607a 6060  ``y``, and ``z``
+0000f0d0: 2061 7267 756d 656e 7473 2063 616e 2068   arguments can h
+0000f0e0: 6176 6520 7468 6520 666f 6c6c 6f77 696e  ave the followin
+0000f0f0: 6720 666f 726d 3a0a 0a20 2020 2020 2020  g form:..       
+0000f100: 2020 2020 202d 204e 6f6e 653a 2020 2020       - None:    
+0000f110: 2020 2020 204c 696d 6974 7320 6172 6520       Limits are 
+0000f120: 6e6f 7420 7365 740a 2020 2020 2020 2020  not set.        
+0000f130: 2020 2020 2d20 7365 7175 656e 6365 3a20      - sequence: 
+0000f140: 2020 2020 5370 6563 6966 7920 6c6f 7765      Specify lowe
+0000f150: 7220 616e 6420 7570 7065 7220 7661 6c75  r and upper valu
+0000f160: 6573 0a20 2020 2020 2020 2020 2020 202d  es.            -
+0000f170: 2064 6963 743a 2020 2020 2020 2020 2045   dict:         E
+0000f180: 7870 6563 7469 6e67 206b 6579 7320 6060  xpecting keys ``
+0000f190: 6c6f 7765 7260 6020 616e 642f 6f72 2060  lower`` and/or `
+0000f1a0: 6075 7070 6572 6060 0a0a 2020 2020 2020  `upper``..      
+0000f1b0: 2020 5468 6520 7365 7175 656e 6365 206f    The sequence o
+0000f1c0: 7220 6469 6374 2076 616c 7565 7320 6361  r dict values ca
+0000f1d0: 6e20 6265 3a0a 0a20 2020 2020 2020 2020  n be:..         
+0000f1e0: 2020 202d 204e 6f6e 6520 2020 2020 2020     - None       
+0000f1f0: 2020 2053 6574 2061 7574 6f6d 6174 6963     Set automatic
+0000f200: 616c 6c79 202f 2064 6f20 6e6f 7420 7365  ally / do not se
+0000f210: 740a 2020 2020 2020 2020 2020 2020 2d20  t.            - 
+0000f220: 6e75 6d65 7269 6320 2020 2020 2020 5365  numeric       Se
+0000f230: 7420 746f 2074 6869 7320 7661 6c75 6520  t to this value 
+0000f240: 6578 706c 6963 6974 6c79 0a20 2020 2020  explicitly.     
+0000f250: 2020 2020 2020 202d 2060 606d 696e 6060         - ``min``
+0000f260: 2020 2020 2020 2053 6574 2074 6f20 7468         Set to th
+0000f270: 6520 6461 7461 206d 696e 696d 756d 2076  e data minimum v
+0000f280: 616c 7565 206f 6e20 7468 6174 2061 7869  alue on that axi
+0000f290: 730a 2020 2020 2020 2020 2020 2020 2d20  s.            - 
+0000f2a0: 6060 6d61 7860 6020 2020 2020 2020 5365  ``max``       Se
+0000f2b0: 7420 746f 2074 6865 2064 6174 6120 6d61  t to the data ma
+0000f2c0: 7869 6d75 6d20 7661 6c75 6520 6f6e 2074  ximum value on t
+0000f2d0: 6861 7420 6178 6973 0a0a 2020 2020 2020  hat axis..      
+0000f2e0: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+0000f2f0: 2020 2020 7820 2855 6e69 6f6e 5b53 6571      x (Union[Seq
+0000f300: 7565 6e63 655b 556e 696f 6e5b 666c 6f61  uence[Union[floa
+0000f310: 742c 2073 7472 5d5d 2c20 6469 6374 5d2c  t, str]], dict],
+0000f320: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+0000f330: 6c69 6d69 7473 0a20 2020 2020 2020 2020  limits.         
+0000f340: 2020 2020 2020 2074 6f20 7365 7420 6f6e         to set on
+0000f350: 2074 6865 2078 2d61 7869 730a 2020 2020   the x-axis.    
+0000f360: 2020 2020 2020 2020 7920 2855 6e69 6f6e          y (Union
+0000f370: 5b53 6571 7565 6e63 655b 556e 696f 6e5b  [Sequence[Union[
+0000f380: 666c 6f61 742c 2073 7472 5d5d 2c20 6469  float, str]], di
+0000f390: 6374 5d2c 206f 7074 696f 6e61 6c29 3a20  ct], optional): 
+0000f3a0: 5468 6520 6c69 6d69 7473 0a20 2020 2020  The limits.     
+0000f3b0: 2020 2020 2020 2020 2020 2074 6f20 7365             to se
+0000f3c0: 7420 6f6e 2074 6865 2079 2d61 7869 730a  t on the y-axis.
+0000f3d0: 2020 2020 2020 2020 2020 2020 7a20 2855              z (U
+0000f3e0: 6e69 6f6e 5b53 6571 7565 6e63 655b 556e  nion[Sequence[Un
+0000f3f0: 696f 6e5b 666c 6f61 742c 2073 7472 5d5d  ion[float, str]]
+0000f400: 2c20 6469 6374 5d2c 206f 7074 696f 6e61  , dict], optiona
+0000f410: 6c29 3a20 5468 6520 6c69 6d69 7473 0a20  l): The limits. 
+0000f420: 2020 2020 2020 2020 2020 2020 2020 2074                 t
+0000f430: 6f20 7365 7420 6f6e 2074 6865 207a 2d61  o set on the z-a
+0000f440: 7869 730a 2020 2020 2020 2020 2020 2020  xis.            
+0000f450: 2020 2020 4966 2074 6865 7265 2069 7320      If there is 
+0000f460: 6e6f 207a 2d61 7869 732c 2074 6869 7320  no z-axis, this 
+0000f470: 7769 6c6c 2062 6520 7369 6c65 6e74 6c79  will be silently
+0000f480: 2069 676e 6f72 6564 2e0a 2020 2020 2020   ignored..      
+0000f490: 2020 2222 220a 0a20 2020 2020 2020 2064    """..        d
+0000f4a0: 6566 2070 6172 7365 5f61 7267 7328 0a20  ef parse_args(. 
+0000f4b0: 2020 2020 2020 2020 2020 2061 7267 733a             args:
+0000f4c0: 2055 6e69 6f6e 5b53 6571 7565 6e63 655b   Union[Sequence[
+0000f4d0: 556e 696f 6e5b 666c 6f61 742c 2073 7472  Union[float, str
+0000f4e0: 5d5d 2c20 6469 6374 5d2c 202a 2c20 6178  ]], dict], *, ax
+0000f4f0: 0a20 2020 2020 2020 2029 202d 3e20 5475  .        ) -> Tu
+0000f500: 706c 655b 666c 6f61 742c 2066 6c6f 6174  ple[float, float
+0000f510: 5d3a 0a20 2020 2020 2020 2020 2020 2022  ]:.            "
+0000f520: 2222 5061 7273 6573 2074 6865 206c 696d  ""Parses the lim
+0000f530: 6974 2061 7267 756d 656e 7473 2e22 2222  it arguments."""
+0000f540: 0a0a 2020 2020 2020 2020 2020 2020 6465  ..            de
+0000f550: 6620 7061 7273 655f 6172 6728 6172 673a  f parse_arg(arg:
+0000f560: 2055 6e69 6f6e 5b66 6c6f 6174 2c20 7374   Union[float, st
+0000f570: 725d 2920 2d3e 2055 6e69 6f6e 5b66 6c6f  r]) -> Union[flo
+0000f580: 6174 2c20 4e6f 6e65 5d3a 0a20 2020 2020  at, None]:.     
+0000f590: 2020 2020 2020 2020 2020 2022 2222 5061             """Pa
+0000f5a0: 7273 6573 2061 2073 696e 676c 6520 6c69  rses a single li
+0000f5b0: 6d69 7420 6172 6775 6d65 6e74 2074 6f20  mit argument to 
+0000f5c0: 6569 7468 6572 2062 6520 666c 6f61 7420  either be float 
+0000f5d0: 6f72 204e 6f6e 6522 2222 0a20 2020 2020  or None""".     
+0000f5e0: 2020 2020 2020 2020 2020 2069 6620 6e6f             if no
+0000f5f0: 7420 6973 696e 7374 616e 6365 2861 7267  t isinstance(arg
+0000f600: 2c20 7374 7229 3a0a 2020 2020 2020 2020  , str):.        
+0000f610: 2020 2020 2020 2020 2020 2020 2320 4e6f              # No
+0000f620: 7468 696e 6720 746f 2070 6172 7365 0a20  thing to parse. 
+0000f630: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f640: 2020 2072 6574 7572 6e20 6172 670a 0a20     return arg.. 
+0000f650: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+0000f660: 6620 6172 6720 3d3d 2022 6d69 6e22 3a0a  f arg == "min":.
+0000f670: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f680: 2020 2020 6172 6720 3d20 6178 2e67 6574      arg = ax.get
+0000f690: 5f64 6174 615f 696e 7465 7276 616c 2829  _data_interval()
+0000f6a0: 5b30 5d0a 2020 2020 2020 2020 2020 2020  [0].            
+0000f6b0: 2020 2020 656c 6966 2061 7267 203d 3d20      elif arg == 
+0000f6c0: 226d 6178 223a 0a20 2020 2020 2020 2020  "max":.         
+0000f6d0: 2020 2020 2020 2020 2020 2061 7267 203d             arg =
+0000f6e0: 2061 782e 6765 745f 6461 7461 5f69 6e74   ax.get_data_int
+0000f6f0: 6572 7661 6c28 295b 315d 0a20 2020 2020  erval()[1].     
+0000f700: 2020 2020 2020 2020 2020 2065 6c73 653a             else:
+0000f710: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f720: 2020 2020 2072 6169 7365 2050 6c6f 7443       raise PlotC
+0000f730: 6f6e 6669 6745 7272 6f72 280a 2020 2020  onfigError(.    
+0000f740: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f750: 2020 2020 6622 476f 7420 616e 2069 6e76      f"Got an inv
+0000f760: 616c 6964 2073 7472 2d74 7970 6520 6172  alid str-type ar
+0000f770: 6775 6d65 6e74 2027 7b61 7267 7d27 2074  gument '{arg}' t
+0000f780: 6f20 7468 6520 220a 2020 2020 2020 2020  o the ".        
 0000f790: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7a0: 2020 2020 2020 2022 7365 745f 6c69 6d69         "set_limi
-0000f7b0: 7473 2068 656c 7065 722e 2041 6c6c 6f77  ts helper. Allow
-0000f7c0: 6564 3a20 276d 696e 272c 2027 6d61 7827  ed: 'min', 'max'
-0000f7d0: 2c20 4e6f 6e65 2c20 6f72 2061 2022 0a20  , None, or a ". 
+0000f7a0: 2273 6574 5f6c 696d 6974 7320 6865 6c70  "set_limits help
+0000f7b0: 6572 2e20 416c 6c6f 7765 643a 2027 6d69  er. Allowed: 'mi
+0000f7c0: 6e27 2c20 276d 6178 272c 204e 6f6e 652c  n', 'max', None,
+0000f7d0: 206f 7220 6120 220a 2020 2020 2020 2020   or a ".        
 0000f7e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f7f0: 2020 2020 2020 2022 6e75 6d65 7269 6361         "numerica
-0000f800: 6c20 7661 6c75 6520 7370 6563 6966 7969  l value specifyi
-0000f810: 6e67 2074 6865 206c 6f77 6572 206f 7220  ng the lower or 
-0000f820: 7570 7065 7220 6c69 6d69 742e 220a 2020  upper limit.".  
-0000f830: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f840: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
-0000f850: 2020 2020 2023 2043 6865 636b 2074 6861       # Check tha
-0000f860: 7420 6974 2069 7320 6669 6e69 7465 0a20  t it is finite. 
-0000f870: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-0000f880: 6620 6e6f 7420 6e70 2e69 7366 696e 6974  f not np.isfinit
-0000f890: 6528 6172 6729 3a0a 2020 2020 2020 2020  e(arg):.        
-0000f8a0: 2020 2020 2020 2020 2020 2020 7261 6973              rais
-0000f8b0: 6520 506c 6f74 436f 6e66 6967 4572 726f  e PlotConfigErro
-0000f8c0: 7228 0a20 2020 2020 2020 2020 2020 2020  r(.             
-0000f8d0: 2020 2020 2020 2020 2020 2022 436f 756c             "Coul
-0000f8e0: 6420 6e6f 7420 6765 7420 6120 6669 6e69  d not get a fini
-0000f8f0: 7465 2076 616c 7565 2066 726f 6d20 7468  te value from th
-0000f900: 6520 6178 6973 2064 6174 6120 746f 2022  e axis data to "
-0000f910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f920: 2020 2020 2020 2020 2022 7573 6520 666f           "use fo
-0000f930: 7220 7365 7474 696e 6720 6178 6973 206c  r setting axis l
-0000f940: 696d 6974 7320 746f 2027 6d69 6e27 206f  imits to 'min' o
-0000f950: 7220 276d 6178 272c 2022 0a20 2020 2020  r 'max', ".     
-0000f960: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000f970: 2020 2022 7072 6573 756d 6162 6c79 2062     "presumably b
-0000f980: 6563 6175 7365 2074 6865 2061 7869 7320  ecause the axis 
-0000f990: 6973 2073 7469 6c6c 2065 6d70 7479 2e22  is still empty."
-0000f9a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-0000f9b0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-0000f9c0: 2020 2020 2020 2020 7265 7475 726e 2061          return a
-0000f9d0: 7267 0a0a 2020 2020 2020 2020 2020 2020  rg..            
-0000f9e0: 2320 5370 6563 6961 6c20 6361 7365 3a20  # Special case: 
-0000f9f0: 6469 6374 0a20 2020 2020 2020 2020 2020  dict.           
-0000fa00: 2069 6620 6973 696e 7374 616e 6365 2861   if isinstance(a
-0000fa10: 7267 732c 2064 6963 7429 3a0a 2020 2020  rgs, dict):.    
-0000fa20: 2020 2020 2020 2020 2020 2020 2320 4d61              # Ma
-0000fa30: 6b65 2073 7572 6520 7468 6572 6520 6172  ke sure there ar
-0000fa40: 6520 6f6e 6c79 2061 6c6c 6f77 6564 206b  e only allowed k
-0000fa50: 6579 730a 2020 2020 2020 2020 2020 2020  eys.            
-0000fa60: 2020 2020 6966 205b 6b20 666f 7220 6b20      if [k for k 
-0000fa70: 696e 2061 7267 732e 6b65 7973 2829 2069  in args.keys() i
-0000fa80: 6620 6b20 6e6f 7420 696e 2028 226c 6f77  f k not in ("low
-0000fa90: 6572 222c 2022 7570 7065 7222 295d 3a0a  er", "upper")]:.
-0000faa0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fab0: 2020 2020 7261 6973 6520 506c 6f74 436f      raise PlotCo
-0000fac0: 6e66 6967 4572 726f 7228 0a20 2020 2020  nfigError(.     
-0000fad0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-0000fae0: 2020 2022 5468 6572 6520 6172 6520 696e     "There are in
-0000faf0: 7661 6c69 6420 6b65 7973 2070 7265 7365  valid keys prese
-0000fb00: 6e74 2069 6e20 6120 6469 6374 2d74 7970  nt in a dict-typ
-0000fb10: 6520 220a 2020 2020 2020 2020 2020 2020  e ".            
-0000fb20: 2020 2020 2020 2020 2020 2020 2261 7267              "arg
-0000fb30: 756d 656e 7420 746f 2073 6574 5f6c 696d  ument to set_lim
-0000fb40: 6974 7321 204f 6e6c 7920 6163 6365 7074  its! Only accept
-0000fb50: 696e 6720 6b65 7973 2027 6c6f 7765 7227  ing keys 'lower'
-0000fb60: 2022 0a20 2020 2020 2020 2020 2020 2020   ".             
-0000fb70: 2020 2020 2020 2020 2020 2066 2261 6e64             f"and
-0000fb80: 2027 7570 7065 7227 2c20 6275 7420 676f   'upper', but go
-0000fb90: 743a 207b 6172 6773 7d22 0a20 2020 2020  t: {args}".     
-0000fba0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
-0000fbb0: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
-0000fbc0: 2020 6c6f 7765 7220 3d20 6172 6773 2e67    lower = args.g
-0000fbd0: 6574 2822 6c6f 7765 7222 2c20 4e6f 6e65  et("lower", None
-0000fbe0: 290a 2020 2020 2020 2020 2020 2020 2020  ).              
-0000fbf0: 2020 7570 7065 7220 3d20 6172 6773 2e67    upper = args.g
-0000fc00: 6574 2822 7570 7065 7222 2c20 4e6f 6e65  et("upper", None
-0000fc10: 290a 0a20 2020 2020 2020 2020 2020 2065  )..            e
-0000fc20: 6c73 653a 0a20 2020 2020 2020 2020 2020  lse:.           
-0000fc30: 2020 2020 206c 6f77 6572 2c20 7570 7065       lower, uppe
-0000fc40: 7220 3d20 6172 6773 2020 2320 2e2e 2e20  r = args  # ... 
-0000fc50: 6173 7375 6d69 6e67 2073 6571 7565 6e63  assuming sequenc
-0000fc60: 6520 6f66 206c 656e 6774 6820 320a 0a20  e of length 2.. 
-0000fc70: 2020 2020 2020 2020 2020 2023 2050 6172             # Par
-0000fc80: 7365 2069 6e64 6976 6964 7561 6c6c 792c  se individually,
-0000fc90: 2074 6865 6e20 7265 7475 726e 0a20 2020   then return.   
-0000fca0: 2020 2020 2020 2020 2072 6574 7572 6e20           return 
-0000fcb0: 2870 6172 7365 5f61 7267 286c 6f77 6572  (parse_arg(lower
-0000fcc0: 292c 2070 6172 7365 5f61 7267 2875 7070  ), parse_arg(upp
-0000fcd0: 6572 2929 0a0a 2020 2020 2020 2020 2320  er))..        # 
-0000fce0: 4e6f 7720 7365 7420 7468 6520 6c69 6d69  Now set the limi
-0000fcf0: 7473 2c20 7573 696e 6720 7468 6520 6865  ts, using the he
-0000fd00: 6c70 6572 2066 756e 6374 696f 6e73 2064  lper functions d
-0000fd10: 6566 696e 6564 2061 626f 7665 0a20 2020  efined above.   
-0000fd20: 2020 2020 2069 6620 7820 6973 206e 6f74       if x is not
-0000fd30: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-0000fd40: 2020 2073 656c 662e 6178 2e73 6574 5f78     self.ax.set_x
-0000fd50: 6c69 6d28 2a70 6172 7365 5f61 7267 7328  lim(*parse_args(
-0000fd60: 782c 2061 783d 7365 6c66 2e61 782e 7861  x, ax=self.ax.xa
-0000fd70: 7869 7329 290a 0a20 2020 2020 2020 2069  xis))..        i
-0000fd80: 6620 7920 6973 206e 6f74 204e 6f6e 653a  f y is not None:
-0000fd90: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
-0000fda0: 662e 6178 2e73 6574 5f79 6c69 6d28 2a70  f.ax.set_ylim(*p
-0000fdb0: 6172 7365 5f61 7267 7328 792c 2061 783d  arse_args(y, ax=
-0000fdc0: 7365 6c66 2e61 782e 7961 7869 7329 290a  self.ax.yaxis)).
-0000fdd0: 0a20 2020 2020 2020 2069 6620 6861 7361  .        if hasa
-0000fde0: 7474 7228 7365 6c66 2e61 782c 2022 7a61  ttr(self.ax, "za
-0000fdf0: 7869 7322 293a 0a20 2020 2020 2020 2020  xis"):.         
-0000fe00: 2020 2069 6620 7a20 6973 206e 6f74 204e     if z is not N
-0000fe10: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
-0000fe20: 2020 2020 2073 656c 662e 6178 2e73 6574       self.ax.set
-0000fe30: 5f7a 6c69 6d28 2a70 6172 7365 5f61 7267  _zlim(*parse_arg
-0000fe40: 7328 7a2c 2061 783d 7365 6c66 2e61 782e  s(z, ax=self.ax.
-0000fe50: 7a61 7869 7329 290a 0a20 2020 2064 6566  zaxis))..    def
-0000fe60: 205f 686c 7072 5f73 6574 5f6d 6172 6769   _hlpr_set_margi
-0000fe70: 6e73 280a 2020 2020 2020 2020 7365 6c66  ns(.        self
-0000fe80: 2c0a 2020 2020 2020 2020 2a2c 0a20 2020  ,.        *,.   
-0000fe90: 2020 2020 206d 6172 6769 6e73 3a20 556e       margins: Un
-0000fea0: 696f 6e5b 666c 6f61 742c 2054 7570 6c65  ion[float, Tuple
-0000feb0: 5b66 6c6f 6174 2c20 666c 6f61 745d 5d20  [float, float]] 
-0000fec0: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-0000fed0: 783a 2066 6c6f 6174 203d 204e 6f6e 652c  x: float = None,
-0000fee0: 0a20 2020 2020 2020 2079 3a20 666c 6f61  .        y: floa
-0000fef0: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
-0000ff00: 2020 7469 6768 743a 2062 6f6f 6c20 3d20    tight: bool = 
-0000ff10: 5472 7565 2c0a 2020 2020 293a 0a20 2020  True,.    ):.   
-0000ff20: 2020 2020 2022 2222 5365 7473 2074 6865       """Sets the
-0000ff30: 2061 7865 7327 206d 6172 6769 6e73 2076   axes' margins v
-0000ff40: 6961 203a 7079 3a6d 6574 683a 606d 6174  ia :py:meth:`mat
-0000ff50: 706c 6f74 6c69 622e 6178 6573 2e41 7865  plotlib.axes.Axe
-0000ff60: 732e 6d61 7267 696e 7360 2e0a 0a20 2020  s.margins`...   
-0000ff70: 2020 2020 2054 6865 2070 6164 6469 6e67       The padding
-0000ff80: 2061 6464 6564 2074 6f20 6561 6368 206c   added to each l
-0000ff90: 696d 6974 206f 6620 7468 6520 4178 6573  imit of the Axes
-0000ffa0: 2069 7320 7468 6520 6d61 7267 696e 2074   is the margin t
-0000ffb0: 696d 6573 2074 6865 0a20 2020 2020 2020  imes the.       
-0000ffc0: 2064 6174 6120 696e 7465 7276 616c 2e0a   data interval..
-0000ffd0: 2020 2020 2020 2020 416c 6c20 696e 7075          All inpu
-0000ffe0: 7420 7061 7261 6d65 7465 7273 206d 7573  t parameters mus
-0000fff0: 7420 6265 2066 6c6f 6174 7320 7769 7468  t be floats with
-00010000: 696e 2074 6865 2072 616e 6765 205b 302c  in the range [0,
-00010010: 2031 5d2e 0a0a 2020 2020 2020 2020 5370   1]...        Sp
-00010020: 6563 6966 7969 6e67 2061 6e79 206d 6172  ecifying any mar
-00010030: 6769 6e20 6368 616e 6765 7320 6f6e 6c79  gin changes only
-00010040: 2074 6865 2061 7574 6f73 6361 6c69 6e67   the autoscaling
-00010050: 3b20 666f 7220 6578 616d 706c 652c 2069  ; for example, i
-00010060: 660a 2020 2020 2020 2020 6060 786d 6172  f.        ``xmar
-00010070: 6769 6e60 6020 6973 206e 6f74 204e 6f6e  gin`` is not Non
-00010080: 652c 2074 6865 6e20 6060 786d 6172 6769  e, then ``xmargi
-00010090: 6e60 6020 7469 6d65 7320 7468 6520 5820  n`` times the X 
-000100a0: 6461 7461 2069 6e74 6572 7661 6c0a 2020  data interval.  
-000100b0: 2020 2020 2020 7769 6c6c 2062 6520 6164        will be ad
-000100c0: 6465 6420 746f 2065 6163 6820 656e 6420  ded to each end 
-000100d0: 6f66 2074 6861 7420 696e 7465 7276 616c  of that interval
-000100e0: 2062 6566 6f72 6520 6974 2069 7320 7573   before it is us
-000100f0: 6564 2069 6e0a 2020 2020 2020 2020 6175  ed in.        au
-00010100: 746f 7363 616c 696e 672e 0a0a 2020 2020  toscaling...    
-00010110: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00010120: 2020 2020 2020 6d61 7267 696e 7320 2855        margins (U
-00010130: 6e69 6f6e 5b66 6c6f 6174 2c20 5475 706c  nion[float, Tupl
-00010140: 655b 666c 6f61 742c 2066 6c6f 6174 5d5d  e[float, float]]
-00010150: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
-00010160: 6120 7363 616c 6172 0a20 2020 2020 2020  a scalar.       
-00010170: 2020 2020 2020 2020 2061 7267 756d 656e           argumen
-00010180: 7420 6973 2070 726f 7669 6465 642c 2069  t is provided, i
-00010190: 7420 7370 6563 6966 6965 7320 626f 7468  t specifies both
-000101a0: 206d 6172 6769 6e73 206f 6620 7468 6520   margins of the 
-000101b0: 782d 6178 6973 0a20 2020 2020 2020 2020  x-axis.         
-000101c0: 2020 2020 2020 2061 6e64 2079 2d61 7869         and y-axi
-000101d0: 7320 6c69 6d69 7473 2e20 4966 2061 206c  s limits. If a l
-000101e0: 6973 742d 206f 7220 7475 706c 652d 6c69  ist- or tuple-li
-000101f0: 6b65 2070 6f73 6974 696f 6e61 6c0a 2020  ke positional.  
-00010200: 2020 2020 2020 2020 2020 2020 2020 6172                ar
-00010210: 6775 6d65 6e74 2069 7320 7072 6f76 6964  gument is provid
-00010220: 6564 2c20 7468 6579 2077 696c 6c20 6265  ed, they will be
-00010230: 2069 6e74 6572 7072 6574 6564 2061 7320   interpreted as 
-00010240: 6060 786d 6172 6769 6e60 602c 0a20 2020  ``xmargin``,.   
-00010250: 2020 2020 2020 2020 2020 2020 2061 6e64               and
-00010260: 2060 6079 6d61 7267 696e 6060 2e20 4966   ``ymargin``. If
-00010270: 2073 6574 7469 6e67 2074 6865 206d 6172   setting the mar
-00010280: 6769 6e20 6f6e 2061 2073 696e 676c 6520  gin on a single 
-00010290: 6178 6973 2069 730a 2020 2020 2020 2020  axis is.        
-000102a0: 2020 2020 2020 2020 6465 7369 7265 642c          desired,
-000102b0: 2075 7365 2074 6865 206b 6579 776f 7264   use the keyword
-000102c0: 2061 7267 756d 656e 7473 2064 6573 6372   arguments descr
-000102d0: 6962 6564 2062 656c 6f77 2e0a 2020 2020  ibed below..    
-000102e0: 2020 2020 2020 2020 782c 2079 2028 666c          x, y (fl
-000102f0: 6f61 742c 206f 7074 696f 6e61 6c29 3a20  oat, optional): 
-00010300: 5370 6563 6966 6963 206d 6172 6769 6e20  Specific margin 
-00010310: 7661 6c75 6573 2066 6f72 2074 6865 2078  values for the x
-00010320: 2d61 7869 7320 616e 640a 2020 2020 2020  -axis and.      
-00010330: 2020 2020 2020 2020 2020 792d 6178 6973            y-axis
-00010340: 2c20 7265 7370 6563 7469 7665 6c79 2e20  , respectively. 
-00010350: 5468 6573 6520 6361 6e6e 6f74 2062 6520  These cannot be 
-00010360: 7573 6564 2069 6e20 636f 6d62 696e 6174  used in combinat
-00010370: 696f 6e20 7769 7468 0a20 2020 2020 2020  ion with.       
-00010380: 2020 2020 2020 2020 2074 6865 2060 606d           the ``m
-00010390: 6172 6769 6e73 6060 2061 7267 756d 656e  argins`` argumen
-000103a0: 742c 2062 7574 2063 616e 2062 6520 7573  t, but can be us
-000103b0: 6564 2069 6e64 6976 6964 7561 6c6c 7920  ed individually 
-000103c0: 746f 0a20 2020 2020 2020 2020 2020 2020  to.             
-000103d0: 2020 2061 6c74 6572 206f 6e20 652e 672e     alter on e.g.
-000103e0: 2c20 6f6e 6c79 2074 6865 2079 2d61 7869  , only the y-axi
-000103f0: 732e 0a20 2020 2020 2020 2020 2020 2074  s..            t
-00010400: 6967 6874 2028 626f 6f6c 2c20 6f70 7469  ight (bool, opti
-00010410: 6f6e 616c 293a 2054 6865 2074 6967 6874  onal): The tight
-00010420: 2070 6172 616d 6574 6572 2069 7320 7061   parameter is pa
-00010430: 7373 6564 2074 6f0a 2020 2020 2020 2020  ssed to.        
-00010440: 2020 2020 2020 2020 3a70 793a 6d65 7468          :py:meth
-00010450: 3a60 6d61 7470 6c6f 746c 6962 2e61 7865  :`matplotlib.axe
-00010460: 732e 4178 6573 2e61 7574 6f73 6361 6c65  s.Axes.autoscale
-00010470: 5f76 6965 7760 2c20 7768 6963 6820 6973  _view`, which is
-00010480: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00010490: 2065 7865 6375 7465 6420 6166 7465 7220   executed after 
-000104a0: 6120 6d61 7267 696e 2069 7320 6368 616e  a margin is chan
-000104b0: 6765 643b 2074 6865 2064 6566 6175 6c74  ged; the default
-000104c0: 2068 6572 6520 6973 2054 7275 652c 0a20   here is True,. 
-000104d0: 2020 2020 2020 2020 2020 2020 2020 206f                 o
-000104e0: 6e20 7468 6520 6173 7375 6d70 7469 6f6e  n the assumption
-000104f0: 2074 6861 7420 7768 656e 206d 6172 6769   that when margi
-00010500: 6e73 2061 7265 2073 7065 6369 6669 6564  ns are specified
-00010510: 2c20 6e6f 0a20 2020 2020 2020 2020 2020  , no.           
-00010520: 2020 2020 2061 6464 6974 696f 6e61 6c20       additional 
-00010530: 7061 6464 696e 6720 746f 206d 6174 6368  padding to match
-00010540: 2074 6963 6b20 6d61 726b 7320 6973 2075   tick marks is u
-00010550: 7375 616c 6c79 2064 6573 6972 6564 2e20  sually desired. 
-00010560: 5365 740a 2020 2020 2020 2020 2020 2020  Set.            
-00010570: 2020 2020 7469 6768 7420 746f 204e 6f6e      tight to Non
-00010580: 6520 7769 6c6c 2070 7265 7365 7276 6520  e will preserve 
-00010590: 7468 6520 7072 6576 696f 7573 2073 6574  the previous set
-000105a0: 7469 6e67 2e0a 2020 2020 2020 2020 2222  ting..        ""
-000105b0: 220a 2020 2020 2020 2020 6b77 6172 6773  ".        kwargs
-000105c0: 203d 2064 6963 7428 783d 782c 2079 3d79   = dict(x=x, y=y
-000105d0: 2c20 7469 6768 743d 7469 6768 7429 0a0a  , tight=tight)..
-000105e0: 2020 2020 2020 2020 6966 206d 6172 6769          if margi
-000105f0: 6e73 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ns is not None:.
-00010600: 2020 2020 2020 2020 2020 2020 6966 2078              if x
-00010610: 2069 7320 6e6f 7420 4e6f 6e65 206f 7220   is not None or 
-00010620: 7920 6973 206e 6f74 204e 6f6e 653a 0a20  y is not None:. 
-00010630: 2020 2020 2020 2020 2020 2020 2020 2072                 r
-00010640: 6169 7365 2054 7970 6545 7272 6f72 280a  aise TypeError(.
-00010650: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010660: 2020 2020 2243 616e 6e6f 7420 7061 7373      "Cannot pass
-00010670: 2062 6f74 6820 606d 6172 6769 6e73 6020   both `margins` 
-00010680: 616e 6420 6078 602f 6079 6020 6172 6775  and `x`/`y` argu
-00010690: 6d65 6e74 7321 220a 2020 2020 2020 2020  ments!".        
-000106a0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-000106b0: 2020 2020 2020 2069 6620 6973 696e 7374         if isinst
-000106c0: 616e 6365 286d 6172 6769 6e73 2c20 2866  ance(margins, (f
-000106d0: 6c6f 6174 2c20 696e 7429 293a 0a20 2020  loat, int)):.   
-000106e0: 2020 2020 2020 2020 2020 2020 2073 656c               sel
-000106f0: 662e 6178 2e6d 6172 6769 6e73 286d 6172  f.ax.margins(mar
-00010700: 6769 6e73 2c20 2a2a 6b77 6172 6773 290a  gins, **kwargs).
-00010710: 2020 2020 2020 2020 2020 2020 656c 7365              else
-00010720: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-00010730: 2020 7365 6c66 2e61 782e 6d61 7267 696e    self.ax.margin
-00010740: 7328 2a6d 6172 6769 6e73 2c20 2a2a 6b77  s(*margins, **kw
-00010750: 6172 6773 290a 2020 2020 2020 2020 656c  args).        el
-00010760: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00010770: 7365 6c66 2e61 782e 6d61 7267 696e 7328  self.ax.margins(
-00010780: 2a2a 6b77 6172 6773 290a 0a20 2020 2064  **kwargs)..    d
-00010790: 6566 205f 686c 7072 5f73 6574 5f6c 6567  ef _hlpr_set_leg
-000107a0: 656e 6428 0a20 2020 2020 2020 2073 656c  end(.        sel
-000107b0: 662c 0a20 2020 2020 2020 202a 2c0a 2020  f,.        *,.  
-000107c0: 2020 2020 2020 7573 655f 6c65 6765 6e64        use_legend
-000107d0: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
-000107e0: 2020 2020 2020 2067 6174 6865 725f 6672         gather_fr
-000107f0: 6f6d 5f66 6967 3a20 626f 6f6c 203d 2046  om_fig: bool = F
-00010800: 616c 7365 2c0a 2020 2020 2020 2020 6375  alse,.        cu
-00010810: 7374 6f6d 5f6c 6162 656c 733a 2053 6571  stom_labels: Seq
-00010820: 7565 6e63 655b 7374 725d 203d 2028 292c  uence[str] = (),
-00010830: 0a20 2020 2020 2020 2068 6964 696e 675f  .        hiding_
-00010840: 7468 7265 7368 6f6c 643a 2069 6e74 203d  threshold: int =
-00010850: 204e 6f6e 652c 0a20 2020 2020 2020 202a   None,.        *
-00010860: 2a6c 6567 656e 645f 6b77 6172 6773 2c0a  *legend_kwargs,.
-00010870: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-00010880: 2222 5365 7473 2061 206c 6567 656e 6420  ""Sets a legend 
-00010890: 666f 7220 7468 6520 6375 7272 656e 7420  for the current 
-000108a0: 6178 6973 2e0a 0a20 2020 2020 2020 2041  axis...        A
-000108b0: 7320 6120 6669 7273 7420 7374 6570 2c20  s a first step, 
-000108c0: 7468 6973 2068 656c 7065 7220 7472 6965  this helper trie
-000108d0: 7320 746f 2065 7874 7261 6374 2061 6c6c  s to extract all
-000108e0: 2072 656c 6576 616e 7420 6c65 6765 6e64   relevant legend
-000108f0: 0a20 2020 2020 2020 2068 616e 646c 6573  .        handles
-00010900: 2061 6e64 206c 6162 656c 732e 2049 6620   and labels. If 
-00010910: 6120 6c65 6765 6e64 2077 6173 2073 6574  a legend was set
-00010920: 2070 7265 7669 6f75 736c 7920 616e 6420   previously and 
-00010930: 2a6e 6f2a 2068 616e 646c 6573 2061 6e64  *no* handles and
-00010940: 0a20 2020 2020 2020 206c 6162 656c 7320  .        labels 
-00010950: 636f 756c 6420 6265 2065 7874 7261 6374  could be extract
-00010960: 6564 2069 6e20 7468 6520 7479 7069 6361  ed in the typica
-00010970: 6c20 7761 7920 2869 2e65 2e2c 2075 7369  l way (i.e., usi
-00010980: 6e67 2074 6865 0a20 2020 2020 2020 2060  ng the.        `
-00010990: 6061 782e 6765 745f 6c65 6765 6e64 5f68  `ax.get_legend_h
-000109a0: 616e 646c 6573 5f6c 6162 656c 7360 6020  andles_labels`` 
-000109b0: 6d65 7468 6f64 2920 6974 2077 696c 6c20  method) it will 
-000109c0: 6265 2061 7474 656d 7074 6564 2074 6f0a  be attempted to.
-000109d0: 2020 2020 2020 2020 7265 7472 6965 7665          retrieve
-000109e0: 2074 6865 6d20 6672 6f6d 2065 7869 7374   them from exist
-000109f0: 696e 6720 3a70 793a 636c 6173 733a 606d  ing :py:class:`m
-00010a00: 6174 706c 6f74 6c69 622e 6c65 6765 6e64  atplotlib.legend
-00010a10: 2e4c 6567 656e 6460 0a20 2020 2020 2020  .Legend`.       
-00010a20: 206f 626a 6563 7473 206f 6e20 7468 6520   objects on the 
-00010a30: 6375 7272 656e 7420 6178 6973 2e0a 2020  current axis..  
-00010a40: 2020 2020 2020 4966 2060 6067 6174 6865        If ``gathe
-00010a50: 725f 6672 6f6d 5f66 6967 6060 2069 7320  r_from_fig`` is 
-00010a60: 6769 7665 6e2c 2074 6865 202a 7768 6f6c  given, the *whol
-00010a70: 652a 2066 6967 7572 6520 7769 6c6c 2062  e* figure will b
-00010a80: 6520 696e 7370 6563 7465 642c 0a20 2020  e inspected,.   
-00010a90: 2020 2020 2072 6567 6172 646c 6573 7320       regardless 
-00010aa0: 6f66 2077 6865 7468 6572 2068 616e 646c  of whether handl
-00010ab0: 6573 2077 6572 6520 666f 756e 6420 7072  es were found pr
-00010ac0: 6576 696f 7573 6c79 2e0a 0a20 2020 2020  eviously...     
-00010ad0: 2020 2041 6464 6974 696f 6e61 6c6c 792c     Additionally,
-00010ae0: 2061 6c6c 2061 7869 732d 7370 6563 6966   all axis-specif
-00010af0: 6963 2068 616e 646c 6573 2061 6e64 206c  ic handles and l
-00010b00: 6162 656c 7320 7472 6163 6b65 6420 7669  abels tracked vi
-00010b10: 610a 2020 2020 2020 2020 3a70 793a 6d65  a.        :py:me
-00010b20: 7468 3a60 2e74 7261 636b 5f68 616e 646c  th:`.track_handl
-00010b30: 6573 5f6c 6162 656c 7360 2077 696c 6c20  es_labels` will 
-00010b40: 616c 7761 7973 2062 6520 6164 6465 642e  always be added.
-00010b50: 0a0a 2020 2020 2020 2020 2e2e 206e 6f74  ..        .. not
-00010b60: 653a 3a0a 0a20 2020 2020 2020 2020 2020  e::..           
-00010b70: 202d 2049 6620 6e6f 2068 616e 646c 6573   - If no handles
-00010b80: 2063 616e 2062 6520 666f 756e 642c 2074   can be found, t
-00010b90: 6865 206c 6567 656e 6420 6973 2068 6964  he legend is hid
-00010ba0: 6465 6e2c 2061 6c73 6f20 6d65 616e 696e  den, also meanin
-00010bb0: 670a 2020 2020 2020 2020 2020 2020 2020  g.              
-00010bc0: 7468 6174 2074 6865 2060 606c 6567 656e  that the ``legen
-00010bd0: 645f 6b77 6172 6773 6060 2077 696c 6c20  d_kwargs`` will 
-00010be0: 6e6f 7420 6265 2070 6173 7365 6420 6f6e  not be passed on
-00010bf0: 2e0a 2020 2020 2020 2020 2020 2020 2d20  ..            - 
-00010c00: 4475 7269 6e67 2067 6174 6865 7269 6e67  During gathering
-00010c10: 206f 6620 6861 6e64 6c65 7320 616e 6420   of handles and 
-00010c20: 6c61 6265 6c73 2066 726f 6d20 7468 6520  labels from the 
-00010c30: 6375 7272 656e 7420 6178 6973 206f 720a  current axis or.
-00010c40: 2020 2020 2020 2020 2020 2020 2020 7468                th
-00010c50: 6520 6669 6775 7265 2c20 6475 706c 6963  e figure, duplic
-00010c60: 6174 6573 2077 696c 6c20 6265 2072 656d  ates will be rem
-00010c70: 6f76 6564 3b20 6475 706c 6963 6174 6573  oved; duplicates
-00010c80: 2061 7265 2064 6574 6563 7465 640a 2020   are detected.  
-00010c90: 2020 2020 2020 2020 2020 2020 7669 6120              via 
-00010ca0: 7468 6569 7220 6c61 6265 6c20 7374 7269  their label stri
-00010cb0: 6e67 732c 202a 6e6f 742a 2076 6961 2074  ngs, *not* via t
-00010cc0: 6865 6972 2068 616e 646c 652e 0a0a 2020  heir handle...  
-00010cd0: 2020 2020 2020 2e2e 2068 696e 743a 3a0a        .. hint::.
-00010ce0: 0a20 2020 2020 2020 2020 2020 2054 6f20  .            To 
-00010cf0: 7365 7420 6120 6669 6775 7265 2d6c 6576  set a figure-lev
-00010d00: 656c 206c 6567 656e 642c 2075 7365 2074  el legend, use t
-00010d10: 6865 2060 6073 6574 5f66 6967 6c65 6765  he ``set_figlege
-00010d20: 6e64 6060 2068 656c 7065 722e 0a0a 2020  nd`` helper...  
-00010d30: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00010d40: 2020 2020 2020 2020 7573 655f 6c65 6765          use_lege
-00010d50: 6e64 2028 626f 6f6c 2c20 6f70 7469 6f6e  nd (bool, option
-00010d60: 616c 293a 2057 6865 7468 6572 2074 6f20  al): Whether to 
-00010d70: 7365 7420 6120 6c65 6765 6e64 206f 7220  set a legend or 
-00010d80: 6e6f 742e 2049 660a 2020 2020 2020 2020  not. If.        
-00010d90: 2020 2020 2020 2020 4661 6c73 652c 2074          False, t
-00010da0: 6865 206c 6567 656e 6420 7769 6c6c 2062  he legend will b
-00010db0: 6520 7265 6d6f 7665 642e 0a20 2020 2020  e removed..     
-00010dc0: 2020 2020 2020 2067 6174 6865 725f 6672         gather_fr
-00010dd0: 6f6d 5f66 6967 2028 626f 6f6c 2c20 6f70  om_fig (bool, op
-00010de0: 7469 6f6e 616c 293a 2049 6620 7365 742c  tional): If set,
-00010df0: 2077 696c 6c20 6761 7468 6572 206c 6567   will gather leg
-00010e00: 656e 640a 2020 2020 2020 2020 2020 2020  end.            
-00010e10: 2020 2020 6861 6e64 6c65 7320 616e 6420      handles and 
-00010e20: 6c61 6265 6c73 2066 726f 6d20 7468 6520  labels from the 
-00010e30: 7768 6f6c 6520 6669 6775 7265 2e20 5468  whole figure. Th
-00010e40: 6973 2063 616e 2062 6520 7573 6566 756c  is can be useful
-00010e50: 2074 6f0a 2020 2020 2020 2020 2020 2020   to.            
-00010e60: 2020 2020 7365 7420 6966 2074 6865 2072      set if the r
-00010e70: 656c 6576 616e 7420 696e 666f 726d 6174  elevant informat
-00010e80: 696f 6e20 6973 2066 6f75 6e64 206f 6e20  ion is found on 
-00010e90: 616e 6f74 6865 7220 6178 6973 206f 7220  another axis or 
-00010ea0: 696e 0a20 2020 2020 2020 2020 2020 2020  in.             
-00010eb0: 2020 2061 2066 6967 7572 6520 6c65 6765     a figure lege
-00010ec0: 6e64 2e0a 2020 2020 2020 2020 2020 2020  nd..            
-00010ed0: 6375 7374 6f6d 5f6c 6162 656c 7320 2853  custom_labels (S
-00010ee0: 6571 7565 6e63 655b 7374 725d 2c20 6f70  equence[str], op
-00010ef0: 7469 6f6e 616c 293a 2049 6620 6769 7665  tional): If give
-00010f00: 6e2c 2075 7365 2074 6865 7365 206c 6162  n, use these lab
-00010f10: 656c 730a 2020 2020 2020 2020 2020 2020  els.            
-00010f20: 2020 2020 616e 6420 6173 736f 6369 6174      and associat
-00010f30: 6520 7468 656d 2077 6974 6820 6578 6973  e them with exis
-00010f40: 7469 6e67 206c 6162 656c 732e 204e 6f74  ting labels. Not
-00010f50: 6520 7468 6174 2069 6620 6665 7765 720a  e that if fewer.
-00010f60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00010f70: 6c61 6265 6c73 2061 7265 2067 6976 656e  labels are given
-00010f80: 2074 6861 6e20 6861 6e64 6c65 7320 6172   than handles ar
-00010f90: 6520 6176 6169 6c61 626c 652c 2074 686f  e available, tho
-00010fa0: 7365 2077 6974 686f 7574 2061 0a20 2020  se without a.   
-00010fb0: 2020 2020 2020 2020 2020 2020 206c 6162               lab
-00010fc0: 656c 2077 696c 6c20 6e6f 7420 6265 2064  el will not be d
-00010fd0: 7261 776e 2e0a 2020 2020 2020 2020 2020  rawn..          
-00010fe0: 2020 6869 6469 6e67 5f74 6872 6573 686f    hiding_thresho
-00010ff0: 6c64 2028 696e 742c 206f 7074 696f 6e61  ld (int, optiona
-00011000: 6c29 3a20 4966 2067 6976 656e 2c20 7769  l): If given, wi
-00011010: 6c6c 2068 6964 6520 6c65 6765 6e64 730a  ll hide legends.
-00011020: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011030: 7468 6174 2068 6176 6520 6d6f 7265 2074  that have more t
-00011040: 6861 6e20 7468 6973 206e 756d 6265 7220  han this number 
-00011050: 6f66 2068 616e 646c 6573 2072 6567 6973  of handles regis
-00011060: 7465 7265 642e 0a20 2020 2020 2020 2020  tered..         
-00011070: 2020 202a 2a6c 6567 656e 645f 6b77 6172     **legend_kwar
-00011080: 6773 3a20 5061 7373 6564 206f 6e20 746f  gs: Passed on to
-00011090: 2060 6061 782e 6c65 6765 6e64 6060 0a20   ``ax.legend``. 
-000110a0: 2020 2020 2020 2022 2222 0a0a 2020 2020         """..    
-000110b0: 2020 2020 6465 6620 6869 6465 5f6c 6567      def hide_leg
-000110c0: 656e 6428 293a 0a20 2020 2020 2020 2020  end():.         
-000110d0: 2020 206c 6567 656e 6420 3d20 7365 6c66     legend = self
-000110e0: 2e61 782e 6c65 6765 6e64 2828 292c 2066  .ax.legend((), f
-000110f0: 616e 6379 626f 783d 4661 6c73 652c 2066  ancybox=False, f
-00011100: 7261 6d65 6f6e 3d46 616c 7365 290a 2020  rameon=False).  
-00011110: 2020 2020 2020 2020 2020 6c65 6765 6e64            legend
-00011120: 2e73 6574 5f76 6973 6962 6c65 2846 616c  .set_visible(Fal
-00011130: 7365 290a 0a20 2020 2020 2020 2023 2057  se)..        # W
-00011140: 6172 6e20 6162 6f75 7420 7573 6167 6520  arn about usage 
-00011150: 6f66 2074 6865 206f 6c64 2069 6e74 6572  of the old inter
-00011160: 6661 6365 2e0a 2020 2020 2020 2020 2320  face..        # 
-00011170: 544f 444f 2052 656d 6f76 6520 696e 2056  TODO Remove in V
-00011180: 6572 7369 6f6e 2031 2e30 0a20 2020 2020  ersion 1.0.     
-00011190: 2020 2069 6620 6c65 6765 6e64 5f6b 7761     if legend_kwa
-000111a0: 7267 732e 706f 7028 2275 7365 5f66 6967  rgs.pop("use_fig
-000111b0: 6c65 6765 6e64 222c 204e 6f6e 6529 3a0a  legend", None):.
-000111c0: 2020 2020 2020 2020 2020 2020 6c6f 672e              log.
-000111d0: 7761 726e 696e 6728 0a20 2020 2020 2020  warning(.       
-000111e0: 2020 2020 2020 2020 2022 5468 6520 6075           "The `u
-000111f0: 7365 5f66 6967 6c65 6765 6e64 6020 6172  se_figlegend` ar
-00011200: 6775 6d65 6e74 2069 7320 6e6f 206c 6f6e  gument is no lon
-00011210: 6765 7220 7375 7070 6f72 7465 6420 220a  ger supported ".
-00011220: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011230: 2266 6f72 2074 6865 2060 7365 745f 6c65  "for the `set_le
-00011240: 6765 6e64 6020 6865 6c70 6572 2e20 5573  gend` helper. Us
-00011250: 6520 6073 6574 5f66 6967 6c65 6765 6e64  e `set_figlegend
-00011260: 6020 696e 7374 6561 642e 220a 2020 2020  ` instead.".    
-00011270: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
-00011280: 2020 2023 2044 6f20 6578 706c 6963 6974     # Do explicit
-00011290: 2068 6964 696e 6720 6669 7273 742c 2064   hiding first, d
-000112a0: 6f6e 2774 206e 6565 6420 746f 2064 6f20  on't need to do 
-000112b0: 616c 6c20 7468 6520 7265 7374 2069 6e20  all the rest in 
-000112c0: 7468 6973 2063 6173 650a 2020 2020 2020  this case.      
-000112d0: 2020 6966 206e 6f74 2075 7365 5f6c 6567    if not use_leg
-000112e0: 656e 643a 0a20 2020 2020 2020 2020 2020  end:.           
-000112f0: 206c 6f67 2e72 656d 6172 6b28 2248 6964   log.remark("Hid
-00011300: 696e 6720 6c65 6765 6e64 202e 2e2e 2229  ing legend ...")
-00011310: 0a20 2020 2020 2020 2020 2020 2068 6964  .            hid
-00011320: 655f 6c65 6765 6e64 2829 0a20 2020 2020  e_legend().     
-00011330: 2020 2020 2020 2072 6574 7572 6e0a 0a20         return.. 
-00011340: 2020 2020 2020 2023 2054 7279 2074 6f20         # Try to 
-00011350: 6765 7420 2864 616e 676c 696e 6729 2068  get (dangling) h
-00011360: 616e 646c 6573 2061 6e64 206c 6162 656c  andles and label
-00011370: 7320 6672 6f6d 2074 6865 2061 7869 730a  s from the axis.
-00011380: 2020 2020 2020 2020 682c 206c 203d 2073          h, l = s
-00011390: 656c 662e 6178 2e67 6574 5f6c 6567 656e  elf.ax.get_legen
-000113a0: 645f 6861 6e64 6c65 735f 6c61 6265 6c73  d_handles_labels
-000113b0: 2829 0a20 2020 2020 2020 2023 204e 4f54  ().        # NOT
-000113c0: 4520 5769 6c6c 2062 6520 656d 7074 7920  E Will be empty 
-000113d0: 6966 2061 782e 6c65 6765 6e64 2829 2077  if ax.legend() w
-000113e0: 6173 2063 616c 6c65 6420 616c 7265 6164  as called alread
-000113f0: 790a 0a20 2020 2020 2020 2023 2041 6464  y..        # Add
-00011400: 2074 686f 7365 2074 6861 7420 6861 7665   those that have
-00011410: 2062 6565 6e20 7472 6163 6b65 6420 6578   been tracked ex
-00011420: 706c 6963 6974 6c79 0a20 2020 2020 2020  plicitly.       
-00011430: 205f 682c 205f 6c20 3d20 7365 6c66 2e61   _h, _l = self.a
-00011440: 7869 735f 6861 6e64 6c65 735f 6c61 6265  xis_handles_labe
-00011450: 6c73 0a20 2020 2020 2020 2068 202b 3d20  ls.        h += 
-00011460: 5f68 0a20 2020 2020 2020 206c 202b 3d20  _h.        l += 
-00011470: 5f6c 0a0a 2020 2020 2020 2020 2320 4966  _l..        # If
-00011480: 2074 6865 7265 2077 6572 6520 6e6f 2068   there were no h
-00011490: 616e 646c 6573 2061 7661 696c 6162 6c65  andles available
-000114a0: 2069 6e20 7468 6973 2077 6179 2c20 7472   in this way, tr
-000114b0: 7920 746f 2067 6174 6865 7220 7468 650a  y to gather the.
-000114c0: 2020 2020 2020 2020 2320 696e 666f 726d          # inform
-000114d0: 6174 696f 6e20 6672 6f6d 2074 6865 2063  ation from the c
-000114e0: 7572 7265 6e74 2061 7869 7320 6f72 2074  urrent axis or t
-000114f0: 6865 2077 686f 6c65 2066 6967 7572 650a  he whole figure.
-00011500: 2020 2020 2020 2020 6966 206e 6f74 2068          if not h
-00011510: 206f 7220 6761 7468 6572 5f66 726f 6d5f   or gather_from_
-00011520: 6669 673a 0a20 2020 2020 2020 2020 2020  fig:.           
-00011530: 205f 682c 205f 6c20 3d20 6761 7468 6572   _h, _l = gather
-00011540: 5f68 616e 646c 6573 5f6c 6162 656c 7328  _handles_labels(
-00011550: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011560: 2073 656c 662e 6669 6720 6966 2067 6174   self.fig if gat
-00011570: 6865 725f 6672 6f6d 5f66 6967 2065 6c73  her_from_fig els
-00011580: 6520 7365 6c66 2e61 780a 2020 2020 2020  e self.ax.      
-00011590: 2020 2020 2020 290a 2020 2020 2020 2020        ).        
-000115a0: 2020 2020 6c6f 672e 6465 6275 6728 0a20      log.debug(. 
-000115b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000115c0: 4761 7468 6572 6564 2025 6420 6861 6e64  Gathered %d hand
-000115d0: 6c65 7320 616e 6420 6c61 6265 6c73 2066  les and labels f
-000115e0: 726f 6d20 2573 2e22 2c0a 2020 2020 2020  rom %s.",.      
-000115f0: 2020 2020 2020 2020 2020 6c65 6e28 5f68            len(_h
-00011600: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-00011610: 2020 2022 7468 6520 7768 6f6c 6520 6669     "the whole fi
-00011620: 6775 7265 220a 2020 2020 2020 2020 2020  gure".          
-00011630: 2020 2020 2020 6966 2028 6e6f 7420 6820        if (not h 
-00011640: 616e 6420 6761 7468 6572 5f66 726f 6d5f  and gather_from_
-00011650: 6669 6729 0a20 2020 2020 2020 2020 2020  fig).           
-00011660: 2020 2020 2065 6c73 6520 2263 7572 7265       else "curre
-00011670: 6e74 2061 7869 7322 2c0a 2020 2020 2020  nt axis",.      
-00011680: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-00011690: 2020 2020 2068 202b 3d20 5f68 0a20 2020       h += _h.   
-000116a0: 2020 2020 2020 2020 206c 202b 3d20 5f6c           l += _l
-000116b0: 0a0a 2020 2020 2020 2020 2320 5265 6d6f  ..        # Remo
-000116c0: 7665 2070 6f74 656e 7469 616c 2064 7570  ve potential dup
-000116d0: 6c69 6361 7465 2068 616e 646c 6573 2028  licate handles (
-000116e0: 6964 656e 7469 6669 6564 2062 7920 7468  identified by th
-000116f0: 6520 6c61 6265 6c73 290a 2020 2020 2020  e labels).      
-00011700: 2020 682c 206c 203d 2072 656d 6f76 655f    h, l = remove_
-00011710: 6475 706c 6963 6174 655f 6861 6e64 6c65  duplicate_handle
-00011720: 735f 6c61 6265 6c73 2868 2c20 6c29 0a0a  s_labels(h, l)..
-00011730: 2020 2020 2020 2020 2320 2e2e 2e20 616e          # ... an
-00011740: 6420 6576 616c 7561 7465 2074 6865 2063  d evaluate the c
-00011750: 7573 746f 6d20 6c61 6265 6c73 2061 6e64  ustom labels and
-00011760: 2068 6964 696e 6720 7468 7265 7368 6f6c   hiding threshol
-00011770: 640a 2020 2020 2020 2020 682c 206c 2c20  d.        h, l, 
-00011780: 7061 7374 5f74 6872 6573 6820 3d20 7072  past_thresh = pr
-00011790: 6570 6172 655f 6c65 6765 6e64 5f61 7267  epare_legend_arg
-000117a0: 7328 0a20 2020 2020 2020 2020 2020 2068  s(.            h
-000117b0: 2c0a 2020 2020 2020 2020 2020 2020 6c2c  ,.            l,
-000117c0: 0a20 2020 2020 2020 2020 2020 2063 7573  .            cus
-000117d0: 746f 6d5f 6c61 6265 6c73 3d63 7573 746f  tom_labels=custo
-000117e0: 6d5f 6c61 6265 6c73 2c0a 2020 2020 2020  m_labels,.      
-000117f0: 2020 2020 2020 6869 6469 6e67 5f74 6872        hiding_thr
-00011800: 6573 686f 6c64 3d68 6964 696e 675f 7468  eshold=hiding_th
-00011810: 7265 7368 6f6c 642c 0a20 2020 2020 2020  reshold,.       
-00011820: 2029 0a0a 2020 2020 2020 2020 2320 4869   )..        # Hi
-00011830: 6465 206f 7220 6472 6177 2074 6865 206c  de or draw the l
-00011840: 6567 656e 640a 2020 2020 2020 2020 6966  egend.        if
-00011850: 2070 6173 745f 7468 7265 7368 206f 7220   past_thresh or 
-00011860: 6e6f 7420 683a 0a20 2020 2020 2020 2020  not h:.         
-00011870: 2020 2068 6964 655f 6c65 6765 6e64 2829     hide_legend()
-00011880: 0a0a 2020 2020 2020 2020 656c 7365 3a0a  ..        else:.
-00011890: 2020 2020 2020 2020 2020 2020 7365 6c66              self
-000118a0: 2e61 782e 6c65 6765 6e64 2868 2c20 6c2c  .ax.legend(h, l,
-000118b0: 202a 2a6c 6567 656e 645f 6b77 6172 6773   **legend_kwargs
-000118c0: 290a 0a20 2020 2064 6566 205f 686c 7072  )..    def _hlpr
-000118d0: 5f73 6574 5f74 6578 7473 2873 656c 662c  _set_texts(self,
-000118e0: 202a 2c20 7465 7874 733a 2053 6571 7565   *, texts: Seque
-000118f0: 6e63 655b 6469 6374 5d29 3a0a 2020 2020  nce[dict]):.    
-00011900: 2020 2020 2222 2253 6574 7320 6d75 6c74      """Sets mult
-00011910: 6970 6c65 2074 6578 7420 656c 656d 656e  iple text elemen
-00011920: 7473 2066 6f72 2074 6865 2063 7572 7265  ts for the curre
-00011930: 6e74 2061 7869 732e 0a0a 2020 2020 2020  nt axis...      
-00011940: 2020 4578 616d 706c 6520 636f 6e66 6967    Example config
-00011950: 7572 6174 696f 6e3a 0a0a 2020 2020 2020  uration:..      
-00011960: 2020 2e2e 2063 6f64 652d 626c 6f63 6b3a    .. code-block:
-00011970: 3a20 7961 6d6c 0a0a 2020 2020 2020 2020  : yaml..        
-00011980: 2020 2020 7365 745f 7465 7874 733a 0a20      set_texts:. 
-00011990: 2020 2020 2020 2020 2020 2020 2074 6578               tex
-000119a0: 7473 3a0a 2020 2020 2020 2020 2020 2020  ts:.            
-000119b0: 2020 2020 2d20 783a 2030 0a20 2020 2020      - x: 0.     
-000119c0: 2020 2020 2020 2020 2020 2020 2079 3a20               y: 
-000119d0: 310a 2020 2020 2020 2020 2020 2020 2020  1.              
-000119e0: 2020 2020 733a 2073 6f6d 6520 7465 7874      s: some text
-000119f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011a00: 2020 2023 202e 2e2e 206d 6f72 6520 6172     # ... more ar
-00011a10: 6775 6d65 6e74 7320 746f 2070 6c74 2e74  guments to plt.t
-00011a20: 6578 740a 0a20 2020 2020 2020 2041 7267  ext..        Arg
-00011a30: 733a 0a20 2020 2020 2020 2020 2020 2074  s:.            t
-00011a40: 6578 7473 2028 5365 7175 656e 6365 5b64  exts (Sequence[d
-00011a50: 6963 745d 293a 2041 2073 6571 7565 6e63  ict]): A sequenc
-00011a60: 6520 6f66 2074 6578 7420 7370 6563 6966  e of text specif
-00011a70: 6963 6174 696f 6e73 2c20 7468 6174 2061  ications, that a
-00011a80: 7265 0a20 2020 2020 2020 2020 2020 2020  re.             
-00011a90: 2020 2070 6173 7365 6420 746f 203a 7079     passed to :py
-00011aa0: 3a66 756e 633a 606d 6174 706c 6f74 6c69  :func:`matplotli
-00011ab0: 622e 7079 706c 6f74 2e74 6578 7460 0a20  b.pyplot.text`. 
-00011ac0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
-00011ad0: 2020 2066 6f72 206b 7761 7267 7320 696e     for kwargs in
-00011ae0: 2074 6578 7473 3a0a 2020 2020 2020 2020   texts:.        
-00011af0: 2020 2020 7365 6c66 2e61 782e 7465 7874      self.ax.text
-00011b00: 282a 2a6b 7761 7267 7329 0a0a 2020 2020  (**kwargs)..    
-00011b10: 6465 6620 5f68 6c70 725f 616e 6e6f 7461  def _hlpr_annota
-00011b20: 7465 2873 656c 662c 202a 2c20 616e 6e6f  te(self, *, anno
-00011b30: 7461 7469 6f6e 733a 2053 6571 7565 6e63  tations: Sequenc
-00011b40: 655b 6469 6374 5d29 3a0a 2020 2020 2020  e[dict]):.      
-00011b50: 2020 2222 2253 6574 7320 6d75 6c74 6970    """Sets multip
-00011b60: 6c65 2061 6e6e 6f74 6174 696f 6e73 2066  le annotations f
-00011b70: 6f72 2074 6865 2063 7572 7265 6e74 2061  or the current a
-00011b80: 7869 732e 0a0a 2020 2020 2020 2020 4578  xis...        Ex
-00011b90: 616d 706c 6520 636f 6e66 6967 7572 6174  ample configurat
-00011ba0: 696f 6e3a 0a0a 2020 2020 2020 2020 2e2e  ion:..        ..
-00011bb0: 2063 6f64 652d 626c 6f63 6b3a 3a20 7961   code-block:: ya
-00011bc0: 6d6c 0a0a 2020 2020 2020 2020 2020 2020  ml..            
-00011bd0: 616e 6e6f 7461 7465 3a0a 2020 2020 2020  annotate:.      
-00011be0: 2020 2020 2020 2020 616e 6e6f 7461 7469          annotati
-00011bf0: 6f6e 733a 0a20 2020 2020 2020 2020 2020  ons:.           
-00011c00: 2020 2020 202d 2078 793a 205b 312c 2033       - xy: [1, 3
-00011c10: 2e31 3431 3539 5d0a 2020 2020 2020 2020  .14159].        
-00011c20: 2020 2020 2020 2020 2020 7465 7874 3a20            text: 
-00011c30: 7468 6973 2069 7320 cf80 0a20 2020 2020  this is ...     
-00011c40: 2020 2020 2020 2020 2020 2020 2078 7963               xyc
-00011c50: 6f6f 7264 733a 2064 6174 610a 2020 2020  oords: data.    
-00011c60: 2020 2020 2020 2020 2020 2020 2020 2320                # 
-00011c70: 2e2e 2e20 6d6f 7265 2061 7267 756d 656e  ... more argumen
-00011c80: 7473 2074 6f20 706c 742e 616e 6e6f 7461  ts to plt.annota
-00011c90: 7465 0a20 2020 2020 2020 2020 2020 2020  te.             
-00011ca0: 2020 202d 2078 793a 205b 302c 2030 5d0a     - xy: [0, 0].
-00011cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011cc0: 2020 7879 636f 6f72 6473 3a20 6461 7461    xycoords: data
-00011cd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00011ce0: 2020 2074 6578 743a 2074 6869 7320 6973     text: this is
-00011cf0: 207a 6572 6f0a 2020 2020 2020 2020 2020   zero.          
-00011d00: 2020 2020 2020 2020 7879 7465 7874 3a20          xytext: 
-00011d10: 5b30 2e31 2c20 302e 315d 0a20 2020 2020  [0.1, 0.1].     
-00011d20: 2020 2020 2020 2020 2020 2020 2061 7272               arr
-00011d30: 6f77 7072 6f70 733a 0a20 2020 2020 2020  owprops:.       
-00011d40: 2020 2020 2020 2020 2020 2020 2066 6163               fac
-00011d50: 6563 6f6c 6f72 3a20 626c 6163 6b0a 2020  ecolor: black.  
-00011d60: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00011d70: 2020 7368 7269 6e6b 3a20 302e 3035 0a0a    shrink: 0.05..
-00011d80: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
-00011d90: 2020 2020 2020 2020 2020 616e 6e6f 7461            annota
-00011da0: 7469 6f6e 7320 2853 6571 7565 6e63 655b  tions (Sequence[
-00011db0: 6469 6374 5d29 3a20 4120 7365 7175 656e  dict]): A sequen
-00011dc0: 6365 206f 6620 616e 6e6f 7461 7469 6f6e  ce of annotation
-00011dd0: 2070 6172 616d 6574 6572 730a 2020 2020   parameters.    
-00011de0: 2020 2020 2020 2020 2020 2020 7768 6963              whic
-00011df0: 6820 7769 6c6c 2062 6520 7061 7373 6564  h will be passed
-00011e00: 2074 6f20 3a70 793a 6675 6e63 3a60 6d61   to :py:func:`ma
-00011e10: 7470 6c6f 746c 6962 2e70 7970 6c6f 742e  tplotlib.pyplot.
-00011e20: 616e 6e6f 7461 7465 600a 2020 2020 2020  annotate`.      
-00011e30: 2020 2222 220a 2020 2020 2020 2020 666f    """.        fo
-00011e40: 7220 6b77 6172 6773 2069 6e20 616e 6e6f  r kwargs in anno
-00011e50: 7461 7469 6f6e 733a 0a20 2020 2020 2020  tations:.       
-00011e60: 2020 2020 2073 656c 662e 6178 2e61 6e6e       self.ax.ann
-00011e70: 6f74 6174 6528 2a2a 6b77 6172 6773 290a  otate(**kwargs).
-00011e80: 0a20 2020 2064 6566 205f 686c 7072 5f73  .    def _hlpr_s
-00011e90: 6574 5f68 765f 6c69 6e65 7328 7365 6c66  et_hv_lines(self
-00011ea0: 2c20 2a2c 2068 6c69 6e65 733a 206c 6973  , *, hlines: lis
-00011eb0: 7420 3d20 4e6f 6e65 2c20 766c 696e 6573  t = None, vlines
-00011ec0: 3a20 6c69 7374 203d 204e 6f6e 6529 3a0a  : list = None):.
-00011ed0: 2020 2020 2020 2020 2222 2253 6574 7320          """Sets 
-00011ee0: 6f6e 6520 6f72 206d 756c 7469 706c 6520  one or multiple 
-00011ef0: 686f 7269 7a6f 6e74 616c 206f 7220 7665  horizontal or ve
-00011f00: 7274 6963 616c 206c 696e 6573 2075 7369  rtical lines usi
-00011f10: 6e67 0a20 2020 2020 2020 203a 7079 3a6d  ng.        :py:m
-00011f20: 6574 683a 606d 6174 706c 6f74 6c69 622e  eth:`matplotlib.
-00011f30: 6178 6573 2e41 7865 732e 6178 686c 696e  axes.Axes.axhlin
-00011f40: 6560 2061 6e64 202f 206f 720a 2020 2020  e` and / or.    
-00011f50: 2020 2020 3a70 793a 6d65 7468 3a60 6d61      :py:meth:`ma
-00011f60: 7470 6c6f 746c 6962 2e61 7865 732e 4178  tplotlib.axes.Ax
-00011f70: 6573 2e61 7876 6c69 6e65 602e 0a0a 2020  es.axvline`...  
-00011f80: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
-00011f90: 2020 2020 2020 2020 686c 696e 6573 2028          hlines (
-00011fa0: 6c69 7374 2c20 6f70 7469 6f6e 616c 293a  list, optional):
-00011fb0: 206c 6973 7420 6f66 206e 756d 6572 6963   list of numeric
-00011fc0: 2070 6f73 6974 696f 6e73 206f 6620 7468   positions of th
-00011fd0: 6520 6c69 6e65 7320 6f72 0a20 2020 2020  e lines or.     
-00011fe0: 2020 2020 2020 2020 2020 206f 7220 6c69             or li
-00011ff0: 7374 206f 6620 6469 6374 7320 7769 7468  st of dicts with
-00012000: 206b 6579 2060 6070 6f73 6060 2064 6574   key ``pos`` det
-00012010: 6572 6d69 6e69 6e67 2074 6865 2070 6f73  ermining the pos
-00012020: 6974 696f 6e2c 206b 6579 0a20 2020 2020  ition, key.     
-00012030: 2020 2020 2020 2020 2020 2060 606c 696d             ``lim
-00012040: 6974 7360 6020 6465 7465 726d 696e 696e  its`` determinin
-00012050: 6720 7468 6520 7265 6c61 7469 7665 206c  g the relative l
-00012060: 696d 6974 7320 6f66 2074 6865 206c 696e  imits of the lin
-00012070: 652c 2061 6e64 2061 6c6c 0a20 2020 2020  e, and all.     
-00012080: 2020 2020 2020 2020 2020 2061 6464 6974             addit
-00012090: 696f 6e61 6c20 6172 6775 6d65 6e74 7320  ional arguments 
-000120a0: 6265 696e 6720 7061 7373 6564 206f 6e20  being passed on 
-000120b0: 746f 2074 6865 206d 6174 706c 6f74 6c69  to the matplotli
-000120c0: 620a 2020 2020 2020 2020 2020 2020 2020  b.              
-000120d0: 2020 6675 6e63 7469 6f6e 2e0a 2020 2020    function..    
-000120e0: 2020 2020 2020 2020 766c 696e 6573 2028          vlines (
-000120f0: 6c69 7374 2c20 6f70 7469 6f6e 616c 293a  list, optional):
-00012100: 206c 6973 7420 6f66 206e 756d 6572 6963   list of numeric
-00012110: 2070 6f73 6974 696f 6e73 206f 6620 7468   positions of th
-00012120: 6520 6c69 6e65 7320 6f72 0a20 2020 2020  e lines or.     
-00012130: 2020 2020 2020 2020 2020 206f 7220 6c69             or li
-00012140: 7374 206f 6620 6469 6374 7320 7769 7468  st of dicts with
-00012150: 206b 6579 2060 6070 6f73 6060 2064 6574   key ``pos`` det
-00012160: 6572 6d69 6e69 6e67 2074 6865 2070 6f73  ermining the pos
-00012170: 6974 696f 6e2c 206b 6579 0a20 2020 2020  ition, key.     
-00012180: 2020 2020 2020 2020 2020 2060 606c 696d             ``lim
-00012190: 6974 7360 6020 6465 7465 726d 696e 696e  its`` determinin
-000121a0: 6720 7468 6520 7265 6c61 7469 7665 206c  g the relative l
-000121b0: 696d 6974 7320 6f66 2074 6865 206c 696e  imits of the lin
-000121c0: 652c 2061 6e64 2061 6c6c 0a20 2020 2020  e, and all.     
-000121d0: 2020 2020 2020 2020 2020 2061 6464 6974             addit
-000121e0: 696f 6e61 6c20 6172 6775 6d65 6e74 7320  ional arguments 
-000121f0: 6265 696e 6720 7061 7373 6564 206f 6e20  being passed on 
-00012200: 746f 2074 6865 206d 6174 706c 6f74 6c69  to the matplotli
-00012210: 620a 2020 2020 2020 2020 2020 2020 2020  b.              
-00012220: 2020 6675 6e63 7469 6f6e 2e0a 2020 2020    function..    
-00012230: 2020 2020 2222 220a 0a20 2020 2020 2020      """..       
-00012240: 2064 6566 2073 6574 5f6c 696e 6528 0a20   def set_line(. 
-00012250: 2020 2020 2020 2020 2020 2066 756e 633a             func:
-00012260: 2043 616c 6c61 626c 652c 0a20 2020 2020   Callable,.     
-00012270: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
-00012280: 2020 2020 2020 706f 733a 2066 6c6f 6174        pos: float
-00012290: 2c0a 2020 2020 2020 2020 2020 2020 6c69  ,.            li
-000122a0: 6d69 7473 3a20 7475 706c 6520 3d20 2830  mits: tuple = (0
-000122b0: 2e30 2c20 312e 3029 2c0a 2020 2020 2020  .0, 1.0),.      
-000122c0: 2020 2020 2020 2a2a 6c69 6e65 5f6b 7761        **line_kwa
-000122d0: 7267 732c 0a20 2020 2020 2020 2029 3a0a  rgs,.        ):.
-000122e0: 2020 2020 2020 2020 2020 2020 7472 793a              try:
-000122f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00012300: 2070 6f73 203d 2066 6c6f 6174 2870 6f73   pos = float(pos
-00012310: 290a 0a20 2020 2020 2020 2020 2020 2065  )..            e
-00012320: 7863 6570 7420 4578 6365 7074 696f 6e20  xcept Exception 
-00012330: 6173 2065 7272 3a0a 2020 2020 2020 2020  as err:.        
-00012340: 2020 2020 2020 2020 7261 6973 6520 506c          raise Pl
-00012350: 6f74 436f 6e66 6967 4572 726f 7228 0a20  otConfigError(. 
-00012360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00012370: 2020 2066 2247 6f74 206e 6f6e 2d6e 756d     f"Got non-num
-00012380: 6572 6963 2076 616c 7565 2027 7b70 6f73  eric value '{pos
-00012390: 7d27 2066 6f72 2060 706f 7360 2061 7267  }' for `pos` arg
-000123a0: 756d 656e 7420 696e 2022 0a20 2020 2020  ument in ".     
-000123b0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-000123c0: 7365 745f 6876 5f6c 696e 6573 2068 656c  set_hv_lines hel
-000123d0: 7065 7221 220a 2020 2020 2020 2020 2020  per!".          
-000123e0: 2020 2020 2020 290a 0a20 2020 2020 2020        )..       
-000123f0: 2020 2020 2066 756e 6328 706f 732c 202a       func(pos, *
-00012400: 6c69 6d69 7473 2c20 2a2a 6c69 6e65 5f6b  limits, **line_k
-00012410: 7761 7267 7329 0a0a 2020 2020 2020 2020  wargs)..        
-00012420: 6966 2068 6c69 6e65 7320 6973 206e 6f74  if hlines is not
-00012430: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00012440: 2020 2066 6f72 206c 696e 655f 7370 6563     for line_spec
-00012450: 2069 6e20 686c 696e 6573 3a0a 2020 2020   in hlines:.    
-00012460: 2020 2020 2020 2020 2020 2020 6966 2069              if i
-00012470: 7369 6e73 7461 6e63 6528 6c69 6e65 5f73  sinstance(line_s
-00012480: 7065 632c 2064 6963 7429 3a0a 2020 2020  pec, dict):.    
-00012490: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124a0: 7365 745f 6c69 6e65 2873 656c 662e 6178  set_line(self.ax
-000124b0: 2e61 7868 6c69 6e65 2c20 2a2a 6c69 6e65  .axhline, **line
-000124c0: 5f73 7065 6329 0a20 2020 2020 2020 2020  _spec).         
-000124d0: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-000124e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000124f0: 2073 6574 5f6c 696e 6528 7365 6c66 2e61   set_line(self.a
-00012500: 782e 6178 686c 696e 652c 2070 6f73 3d6c  x.axhline, pos=l
-00012510: 696e 655f 7370 6563 290a 0a20 2020 2020  ine_spec)..     
-00012520: 2020 2069 6620 766c 696e 6573 2069 7320     if vlines is 
-00012530: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00012540: 2020 2020 2020 666f 7220 6c69 6e65 5f73        for line_s
-00012550: 7065 6320 696e 2076 6c69 6e65 733a 0a20  pec in vlines:. 
-00012560: 2020 2020 2020 2020 2020 2020 2020 2069                 i
-00012570: 6620 6973 696e 7374 616e 6365 286c 696e  f isinstance(lin
-00012580: 655f 7370 6563 2c20 6469 6374 293a 0a20  e_spec, dict):. 
-00012590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125a0: 2020 2073 6574 5f6c 696e 6528 7365 6c66     set_line(self
-000125b0: 2e61 782e 6178 766c 696e 652c 202a 2a6c  .ax.axvline, **l
-000125c0: 696e 655f 7370 6563 290a 2020 2020 2020  ine_spec).      
-000125d0: 2020 2020 2020 2020 2020 656c 7365 3a0a            else:.
-000125e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000125f0: 2020 2020 7365 745f 6c69 6e65 2873 656c      set_line(sel
-00012600: 662e 6178 2e61 7876 6c69 6e65 2c20 706f  f.ax.axvline, po
-00012610: 733d 6c69 6e65 5f73 7065 6329 0a0a 2020  s=line_spec)..  
-00012620: 2020 6465 6620 5f68 6c70 725f 7365 745f    def _hlpr_set_
-00012630: 7363 616c 6573 280a 2020 2020 2020 2020  scales(.        
-00012640: 7365 6c66 2c0a 2020 2020 2020 2020 2a2c  self,.        *,
-00012650: 0a20 2020 2020 2020 2078 3a20 556e 696f  .        x: Unio
-00012660: 6e5b 7374 722c 2064 6963 745d 203d 204e  n[str, dict] = N
-00012670: 6f6e 652c 0a20 2020 2020 2020 2079 3a20  one,.        y: 
-00012680: 556e 696f 6e5b 7374 722c 2064 6963 745d  Union[str, dict]
-00012690: 203d 204e 6f6e 652c 0a20 2020 2020 2020   = None,.       
-000126a0: 207a 3a20 556e 696f 6e5b 7374 722c 2064   z: Union[str, d
-000126b0: 6963 745d 203d 204e 6f6e 652c 0a20 2020  ict] = None,.   
-000126c0: 2029 3a0a 2020 2020 2020 2020 2222 2253   ):.        """S
-000126d0: 6574 7320 7468 6520 7363 616c 6573 2066  ets the scales f
-000126e0: 6f72 2074 6865 2063 7572 7265 6e74 2061  or the current a
-000126f0: 7869 730a 0a20 2020 2020 2020 2054 6865  xis..        The
-00012700: 2061 7267 756d 656e 7473 2061 7265 2075   arguments are u
-00012710: 7365 6420 746f 2063 616c 6c0a 2020 2020  sed to call.    
-00012720: 2020 2020 3a70 793a 6d65 7468 3a60 6d61      :py:meth:`ma
-00012730: 7470 6c6f 746c 6962 2e61 7865 732e 4178  tplotlib.axes.Ax
-00012740: 6573 2e73 6574 5f78 7363 616c 6560 2061  es.set_xscale` a
-00012750: 6e64 2f6f 720a 2020 2020 2020 2020 3a70  nd/or.        :p
-00012760: 793a 6d65 7468 3a60 6d61 7470 6c6f 746c  y:meth:`matplotl
-00012770: 6962 2e61 7865 732e 4178 6573 2e73 6574  ib.axes.Axes.set
-00012780: 5f79 7363 616c 6560 2061 6e64 0a20 2020  _yscale` and.   
-00012790: 2020 2020 203a 7079 3a6d 6574 683a 606d       :py:meth:`m
-000127a0: 706c 5f74 6f6f 6c6b 6974 732e 6d70 6c6f  pl_toolkits.mplo
-000127b0: 7433 642e 6178 6573 3364 2e41 7865 7333  t3d.axes3d.Axes3
-000127c0: 442e 7365 745f 7a73 6361 6c65 602c 2072  D.set_zscale`, r
-000127d0: 6573 7065 6374 6976 656c 792e 0a20 2020  espectively..   
-000127e0: 2020 2020 2046 6f72 2073 7472 696e 672d       For string-
-000127f0: 6c69 6b65 2061 7267 756d 656e 7473 2c20  like arguments, 
-00012800: 7468 6520 7661 6c75 6520 6973 2064 6972  the value is dir
-00012810: 6563 746c 7920 7573 6564 2074 6f20 7365  ectly used to se
-00012820: 7420 7468 6520 7363 616c 650a 2020 2020  t the scale.    
-00012830: 2020 2020 666f 7220 7468 6174 2061 7869      for that axi
-00012840: 732c 2065 2e67 2e20 6060 6c69 6e65 6172  s, e.g. ``linear
-00012850: 6060 2c20 6060 6c6f 6760 602c 2060 6073  ``, ``log``, ``s
-00012860: 796d 6c6f 6760 602e 0a20 2020 2020 2020  ymlog``..       
-00012870: 204f 7468 6572 7769 7365 2c20 6469 6374   Otherwise, dict
-00012880: 2d6c 696b 6520 6172 6775 6d65 6e74 7320  -like arguments 
-00012890: 6172 6520 6578 7065 6374 6564 2077 6865  are expected whe
-000128a0: 7265 2061 2060 6073 6361 6c65 6060 206b  re a ``scale`` k
-000128b0: 6579 2069 730a 2020 2020 2020 2020 7072  ey is.        pr
-000128c0: 6573 656e 7420 616e 6420 6465 6669 6e65  esent and define
-000128d0: 7320 7768 6963 6820 7479 7065 206f 6620  s which type of 
-000128e0: 7363 616c 6520 746f 2075 7365 2e20 416c  scale to use. Al
-000128f0: 6c20 6675 7274 6865 7220 6172 6775 6d65  l further argume
-00012900: 6e74 730a 2020 2020 2020 2020 6172 6520  nts.        are 
-00012910: 7061 7373 6564 206f 6e3b 2074 6865 7365  passed on; these
-00012920: 2061 7265 2072 656c 6576 616e 7420 666f   are relevant fo
-00012930: 7220 7468 6520 7379 6d6d 6574 7269 6361  r the symmetrica
-00012940: 6c20 6c6f 6761 7269 7468 6d69 630a 2020  l logarithmic.  
-00012950: 2020 2020 2020 7363 616c 652c 2066 6f72        scale, for
-00012960: 2065 7861 6d70 6c65 2e0a 0a20 2020 2020   example...     
-00012970: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00012980: 2020 2020 2078 2028 556e 696f 6e5b 7374       x (Union[st
-00012990: 722c 2064 6963 745d 2c20 6f70 7469 6f6e  r, dict], option
-000129a0: 616c 293a 2054 6865 2073 6361 6c65 7320  al): The scales 
-000129b0: 746f 2075 7365 206f 6e20 7468 6520 782d  to use on the x-
-000129c0: 6178 6973 0a20 2020 2020 2020 2020 2020  axis.           
-000129d0: 2079 2028 556e 696f 6e5b 7374 722c 2064   y (Union[str, d
-000129e0: 6963 745d 2c20 6f70 7469 6f6e 616c 293a  ict], optional):
-000129f0: 2054 6865 2073 6361 6c65 7320 746f 2075   The scales to u
-00012a00: 7365 206f 6e20 7468 6520 792d 6178 6973  se on the y-axis
-00012a10: 0a20 2020 2020 2020 2020 2020 207a 2028  .            z (
-00012a20: 556e 696f 6e5b 7374 722c 2064 6963 745d  Union[str, dict]
-00012a30: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
-00012a40: 2073 6361 6c65 7320 746f 2075 7365 206f   scales to use o
-00012a50: 6e20 7468 6520 7a2d 6178 6973 2e0a 2020  n the z-axis..  
-00012a60: 2020 2020 2020 2020 2020 2020 2020 4966                If
-00012a70: 2074 6865 7265 2069 7320 6e6f 207a 2d61   there is no z-a
-00012a80: 7869 732c 2074 6869 7320 7769 6c6c 2062  xis, this will b
-00012a90: 6520 7369 6c65 6e74 6c79 2069 676e 6f72  e silently ignor
-00012aa0: 6564 2e0a 2020 2020 2020 2020 2222 220a  ed..        """.
-00012ab0: 0a20 2020 2020 2020 2064 6566 2073 6574  .        def set
-00012ac0: 5f73 6361 6c65 2866 756e 633a 2043 616c  _scale(func: Cal
-00012ad0: 6c61 626c 652c 202a 2c20 7363 616c 653a  lable, *, scale:
-00012ae0: 2073 7472 203d 204e 6f6e 652c 202a 2a73   str = None, **s
-00012af0: 6361 6c65 5f6b 7761 7267 7329 3a0a 2020  cale_kwargs):.  
-00012b00: 2020 2020 2020 2020 2020 6675 6e63 2873            func(s
-00012b10: 6361 6c65 2c20 2a2a 7363 616c 655f 6b77  cale, **scale_kw
-00012b20: 6172 6773 290a 0a20 2020 2020 2020 2069  args)..        i
-00012b30: 6620 783a 0a20 2020 2020 2020 2020 2020  f x:.           
-00012b40: 2078 203d 2078 2069 6620 6e6f 7420 6973   x = x if not is
-00012b50: 696e 7374 616e 6365 2878 2c20 7374 7229  instance(x, str)
-00012b60: 2065 6c73 6520 6469 6374 2873 6361 6c65   else dict(scale
-00012b70: 3d78 290a 2020 2020 2020 2020 2020 2020  =x).            
-00012b80: 7365 745f 7363 616c 6528 7365 6c66 2e61  set_scale(self.a
-00012b90: 782e 7365 745f 7873 6361 6c65 2c20 2a2a  x.set_xscale, **
-00012ba0: 7829 0a0a 2020 2020 2020 2020 6966 2079  x)..        if y
-00012bb0: 3a0a 2020 2020 2020 2020 2020 2020 7920  :.            y 
-00012bc0: 3d20 7920 6966 206e 6f74 2069 7369 6e73  = y if not isins
-00012bd0: 7461 6e63 6528 792c 2073 7472 2920 656c  tance(y, str) el
-00012be0: 7365 2064 6963 7428 7363 616c 653d 7929  se dict(scale=y)
-00012bf0: 0a20 2020 2020 2020 2020 2020 2073 6574  .            set
-00012c00: 5f73 6361 6c65 2873 656c 662e 6178 2e73  _scale(self.ax.s
-00012c10: 6574 5f79 7363 616c 652c 202a 2a79 290a  et_yscale, **y).
-00012c20: 0a20 2020 2020 2020 2069 6620 6861 7361  .        if hasa
-00012c30: 7474 7228 7365 6c66 2e61 782c 2022 7a61  ttr(self.ax, "za
-00012c40: 7869 7322 293a 0a20 2020 2020 2020 2020  xis"):.         
-00012c50: 2020 2069 6620 7a3a 0a20 2020 2020 2020     if z:.       
-00012c60: 2020 2020 2020 2020 207a 203d 207a 2069           z = z i
-00012c70: 6620 6e6f 7420 6973 696e 7374 616e 6365  f not isinstance
-00012c80: 287a 2c20 7374 7229 2065 6c73 6520 6469  (z, str) else di
-00012c90: 6374 2873 6361 6c65 3d7a 290a 2020 2020  ct(scale=z).    
-00012ca0: 2020 2020 2020 2020 2020 2020 7365 745f              set_
-00012cb0: 7363 616c 6528 7365 6c66 2e61 782e 7365  scale(self.ax.se
-00012cc0: 745f 7a73 6361 6c65 2c20 2a2a 7a29 0a0a  t_zscale, **z)..
-00012cd0: 2020 2020 6465 6620 5f68 6c70 725f 7365      def _hlpr_se
-00012ce0: 745f 7469 636b 7328 0a20 2020 2020 2020  t_ticks(.       
-00012cf0: 2073 656c 662c 0a20 2020 2020 2020 202a   self,.        *
-00012d00: 2c0a 2020 2020 2020 2020 783a 2055 6e69  ,.        x: Uni
-00012d10: 6f6e 5b6c 6973 742c 2064 6963 745d 203d  on[list, dict] =
-00012d20: 204e 6f6e 652c 0a20 2020 2020 2020 2079   None,.        y
-00012d30: 3a20 556e 696f 6e5b 6c69 7374 2c20 6469  : Union[list, di
-00012d40: 6374 5d20 3d20 4e6f 6e65 2c0a 2020 2020  ct] = None,.    
-00012d50: 2020 2020 7a3a 2055 6e69 6f6e 5b6c 6973      z: Union[lis
-00012d60: 742c 2064 6963 745d 203d 204e 6f6e 652c  t, dict] = None,
-00012d70: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00012d80: 2222 2253 6574 7320 7468 6520 7469 636b  """Sets the tick
-00012d90: 7320 666f 7220 7468 6520 6375 7272 656e  s for the curren
-00012da0: 7420 6178 6973 0a0a 2020 2020 2020 2020  t axis..        
-00012db0: 5468 6520 6172 6775 6d65 6e74 7320 6172  The arguments ar
-00012dc0: 6520 7573 6564 2074 6f20 6361 6c6c 0a20  e used to call. 
-00012dd0: 2020 2020 2020 203a 7079 3a6d 6574 683a         :py:meth:
-00012de0: 606d 6174 706c 6f74 6c69 622e 6178 6573  `matplotlib.axes
-00012df0: 2e41 7865 732e 7365 745f 7874 6963 6b73  .Axes.set_xticks
-00012e00: 6020 6f72 0a20 2020 2020 2020 203a 7079  ` or.        :py
-00012e10: 3a6d 6574 683a 606d 6174 706c 6f74 6c69  :meth:`matplotli
-00012e20: 622e 6178 6573 2e41 7865 732e 7365 745f  b.axes.Axes.set_
-00012e30: 7974 6963 6b73 6020 6f72 0a20 2020 2020  yticks` or.     
-00012e40: 2020 203a 7079 3a6d 6574 683a 606d 706c     :py:meth:`mpl
-00012e50: 5f74 6f6f 6c6b 6974 732e 6d70 6c6f 7433  _toolkits.mplot3
-00012e60: 642e 6178 6573 3364 2e41 7865 7333 442e  d.axes3d.Axes3D.
-00012e70: 7365 745f 7a74 6963 6b73 602c 0a20 2020  set_zticks`,.   
-00012e80: 2020 2020 2061 6e64 203a 7079 3a6d 6574       and :py:met
-00012e90: 683a 606d 6174 706c 6f74 6c69 622e 6178  h:`matplotlib.ax
-00012ea0: 6573 2e41 7865 732e 7365 745f 7874 6963  es.Axes.set_xtic
-00012eb0: 6b6c 6162 656c 7360 206f 720a 2020 2020  klabels` or.    
-00012ec0: 2020 2020 3a70 793a 6d65 7468 3a60 6d61      :py:meth:`ma
-00012ed0: 7470 6c6f 746c 6962 2e61 7865 732e 4178  tplotlib.axes.Ax
-00012ee0: 6573 2e73 6574 5f79 7469 636b 6c61 6265  es.set_yticklabe
-00012ef0: 6c73 6020 6f72 0a20 2020 2020 2020 203a  ls` or.        :
-00012f00: 7079 3a6d 6574 683a 606d 706c 5f74 6f6f  py:meth:`mpl_too
-00012f10: 6c6b 6974 732e 6d70 6c6f 7433 642e 6178  lkits.mplot3d.ax
-00012f20: 6573 3364 2e41 7865 7333 442e 7365 745f  es3d.Axes3D.set_
-00012f30: 7a74 6963 6b6c 6162 656c 7360 2c0a 2020  zticklabels`,.  
-00012f40: 2020 2020 2020 7265 7370 6563 7469 7665        respective
-00012f50: 6c79 2e0a 0a20 2020 2020 2020 2054 6865  ly...        The
-00012f60: 2064 6963 742d 6c69 6b65 2061 7267 756d   dict-like argum
-00012f70: 656e 7473 206d 6179 2063 6f6e 7461 696e  ents may contain
-00012f80: 2074 6865 206b 6579 7320 6060 6d61 6a6f   the keys ``majo
-00012f90: 7260 6020 616e 642f 6f72 0a20 2020 2020  r`` and/or.     
-00012fa0: 2020 2060 606d 696e 6f72 6060 2c20 7265     ``minor``, re
-00012fb0: 6665 7272 696e 6720 746f 206d 616a 6f72  ferring to major
-00012fc0: 206f 7220 6d69 6e6f 7220 7469 636b 206c   or minor tick l
-00012fd0: 6f63 6174 696f 6e73 2061 6e64 206c 6162  ocations and lab
-00012fe0: 656c 732c 0a20 2020 2020 2020 2072 6573  els,.        res
-00012ff0: 7065 6374 6976 656c 792e 0a20 2020 2020  pectively..     
-00013000: 2020 2054 6865 7920 7368 6f75 6c64 2065     They should e
-00013010: 6974 6865 7220 6265 206c 6973 742d 6c69  ither be list-li
-00013020: 6b65 2c20 6469 7265 6374 6c79 2073 7065  ke, directly spe
-00013030: 6369 6679 696e 6720 7468 6520 7469 636b  cifying the tick
-00013040: 7327 0a20 2020 2020 2020 206c 6f63 6174  s'.        locat
-00013050: 696f 6e73 2c20 6f72 2064 6963 742d 6c69  ions, or dict-li
-00013060: 6b65 2072 6571 7569 7269 6e67 2061 2060  ke requiring a `
-00013070: 606c 6f63 7360 6020 6b65 7920 7468 6174  `locs`` key that
-00013080: 2063 6f6e 7461 696e 7320 7468 650a 2020   contains the.  
-00013090: 2020 2020 2020 7469 636b 7327 206c 6f63        ticks' loc
-000130a0: 6174 696f 6e73 2061 6e64 2069 7320 7061  ations and is pa
-000130b0: 7373 6564 206f 6e20 746f 2074 6865 2060  ssed on to the `
-000130c0: 6073 6574 5f3c 782f 792f 7a3e 7469 636b  `set_<x/y/z>tick
-000130d0: 7360 6020 6361 6c6c 2e0a 2020 2020 2020  s`` call..      
-000130e0: 2020 6173 2060 6074 6963 6b73 6060 2061    as ``ticks`` a
-000130f0: 7267 756d 656e 742e 2046 7572 7468 6572  rgument. Further
-00013100: 206b 7761 7267 7320 7375 6368 2061 7320   kwargs such as 
-00013110: 6060 6c61 6265 6c73 6060 2063 616e 2062  ``labels`` can b
-00013120: 6520 6769 7665 6e0a 2020 2020 2020 2020  e given.        
-00013130: 616e 6420 6172 6520 7061 7373 6564 206f  and are passed o
-00013140: 6e20 746f 2074 6865 2060 6073 6574 5f3c  n to the ``set_<
-00013150: 782f 792f 7a3e 7469 636b 6c61 6265 6c73  x/y/z>ticklabels
-00013160: 6060 2063 616c 6c2e 0a0a 2020 2020 2020  `` call...      
-00013170: 2020 4578 616d 706c 653a 0a0a 2020 2020    Example:..    
-00013180: 2020 2020 2e2e 2063 6f64 652d 626c 6f63      .. code-bloc
-00013190: 6b3a 3a20 7961 6d6c 0a0a 2020 2020 2020  k:: yaml..      
-000131a0: 2020 2020 2020 7365 745f 7469 636b 733a        set_ticks:
-000131b0: 0a20 2020 2020 2020 2020 2020 2020 2078  .              x
-000131c0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
-000131d0: 2020 6d61 6a6f 723a 205b 322c 2034 2c20    major: [2, 4, 
-000131e0: 362c 2038 5d0a 2020 2020 2020 2020 2020  6, 8].          
-000131f0: 2020 2020 2020 6d69 6e6f 723a 0a20 2020        minor:.   
-00013200: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00013210: 6f63 733a 205b 312c 2033 2c20 352c 2037  ocs: [1, 3, 5, 7
-00013220: 2c20 395d 0a20 2020 2020 2020 2020 2020  , 9].           
-00013230: 2020 2079 3a0a 2020 2020 2020 2020 2020     y:.          
-00013240: 2020 2020 2020 6d61 6a6f 723a 0a20 2020        major:.   
-00013250: 2020 2020 2020 2020 2020 2020 2020 206c                 l
-00013260: 6f63 733a 205b 302c 2031 3030 302c 2032  ocs: [0, 1000, 2
-00013270: 3030 302c 2033 3030 305d 0a20 2020 2020  000, 3000].     
-00013280: 2020 2020 2020 2020 2020 2020 206c 6162               lab
-00013290: 656c 733a 205b 302c 2031 6b2c 2032 6b2c  els: [0, 1k, 2k,
-000132a0: 2033 6b5d 0a20 2020 2020 2020 2020 2020   3k].           
-000132b0: 2020 2020 2020 2023 202e 2e2e 2066 7572         # ... fur
-000132c0: 7468 6572 206b 7761 7267 7320 6865 7265  ther kwargs here
-000132d0: 2073 7065 6369 6679 206c 6162 656c 2061   specify label a
-000132e0: 6573 7468 6574 6963 730a 0a20 2020 2020  esthetics..     
-000132f0: 2020 2020 2020 2020 207a 3a20 5b2d 312c           z: [-1,
-00013300: 2030 2c20 2b31 5d20 2023 2073 616d 6520   0, +1]  # same 
-00013310: 6173 207a 3a20 7b6d 616a 6f72 3a20 7b6c  as z: {major: {l
-00013320: 6f63 733a 205b 2d31 2c20 302c 202b 315d  ocs: [-1, 0, +1]
-00013330: 7d7d 0a0a 2020 2020 2020 2020 4172 6773  }}..        Args
-00013340: 3a0a 2020 2020 2020 2020 2020 2020 7820  :.            x 
-00013350: 2855 6e69 6f6e 5b6c 6973 742c 2064 6963  (Union[list, dic
-00013360: 745d 2c20 6f70 7469 6f6e 616c 293a 2054  t], optional): T
-00013370: 6865 2074 6963 6b73 2061 6e64 206f 7074  he ticks and opt
-00013380: 696f 6e61 6c6c 7920 7468 6569 720a 2020  ionally their.  
-00013390: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-000133a0: 6265 6c73 2074 6f20 7365 7420 6f6e 2074  bels to set on t
-000133b0: 6865 2078 2d61 7869 730a 2020 2020 2020  he x-axis.      
-000133c0: 2020 2020 2020 7920 2855 6e69 6f6e 5b6c        y (Union[l
-000133d0: 6973 742c 2064 6963 745d 2c20 6f70 7469  ist, dict], opti
-000133e0: 6f6e 616c 293a 2054 6865 2074 6963 6b73  onal): The ticks
-000133f0: 2061 6e64 206f 7074 696f 6e61 6c6c 7920   and optionally 
-00013400: 7468 6569 720a 2020 2020 2020 2020 2020  their.          
-00013410: 2020 2020 2020 6c61 6265 6c73 2074 6f20        labels to 
-00013420: 7365 7420 6f6e 2074 6865 2079 2d61 7869  set on the y-axi
-00013430: 730a 2020 2020 2020 2020 2020 2020 7a20  s.            z 
-00013440: 2855 6e69 6f6e 5b6c 6973 742c 2064 6963  (Union[list, dic
-00013450: 745d 2c20 6f70 7469 6f6e 616c 293a 2054  t], optional): T
-00013460: 6865 2074 6963 6b73 2061 6e64 206f 7074  he ticks and opt
-00013470: 696f 6e61 6c6c 7920 7468 6569 720a 2020  ionally their.  
-00013480: 2020 2020 2020 2020 2020 2020 2020 6c61                la
-00013490: 6265 6c73 2074 6f20 7365 7420 6f6e 2074  bels to set on t
-000134a0: 6865 207a 2d61 7869 732e 0a20 2020 2020  he z-axis..     
-000134b0: 2020 2020 2020 2020 2020 2049 6620 7468             If th
-000134c0: 6572 6520 6973 206e 6f20 7a2d 6178 6973  ere is no z-axis
-000134d0: 2c20 7468 6973 2077 696c 6c20 6265 2073  , this will be s
-000134e0: 696c 656e 746c 7920 6967 6e6f 7265 642e  ilently ignored.
-000134f0: 0a20 2020 2020 2020 2022 2222 0a0a 2020  .        """..  
-00013500: 2020 2020 2020 6465 6620 7365 745f 7469        def set_ti
-00013510: 636b 7328 0a20 2020 2020 2020 2020 2020  cks(.           
-00013520: 2066 756e 633a 2043 616c 6c61 626c 652c   func: Callable,
-00013530: 0a20 2020 2020 2020 2020 2020 202a 2c0a  .            *,.
-00013540: 2020 2020 2020 2020 2020 2020 7469 636b              tick
-00013550: 733a 206c 6973 742c 0a20 2020 2020 2020  s: list,.       
-00013560: 2020 2020 206d 696e 6f72 3a20 626f 6f6c       minor: bool
-00013570: 2c0a 2020 2020 2020 2020 293a 0a20 2020  ,.        ):.   
-00013580: 2020 2020 2020 2020 2066 756e 6328 7469           func(ti
-00013590: 636b 732c 206d 696e 6f72 3d6d 696e 6f72  cks, minor=minor
-000135a0: 290a 0a20 2020 2020 2020 2064 6566 2073  )..        def s
-000135b0: 6574 5f74 6963 6b6c 6162 656c 7328 0a20  et_ticklabels(. 
-000135c0: 2020 2020 2020 2020 2020 2066 756e 633a             func:
-000135d0: 2043 616c 6c61 626c 652c 202a 2c20 6c61   Callable, *, la
-000135e0: 6265 6c73 3a20 6c69 7374 2c20 2a2a 7469  bels: list, **ti
-000135f0: 636b 6c61 6265 6c73 5f6b 7761 7267 730a  cklabels_kwargs.
-00013600: 2020 2020 2020 2020 293a 0a20 2020 2020          ):.     
-00013610: 2020 2020 2020 2066 756e 6328 6c61 6265         func(labe
-00013620: 6c73 2c20 2a2a 7469 636b 6c61 6265 6c73  ls, **ticklabels
-00013630: 5f6b 7761 7267 7329 0a0a 2020 2020 2020  _kwargs)..      
-00013640: 2020 6465 6620 7365 745f 7469 636b 735f    def set_ticks_
-00013650: 616e 645f 6c61 6265 6c73 280a 2020 2020  and_labels(.    
-00013660: 2020 2020 2020 2020 2a2c 2061 7869 733a          *, axis:
-00013670: 2073 7472 2c20 6d69 6e6f 723a 2062 6f6f   str, minor: boo
-00013680: 6c2c 2061 7869 735f 6366 673a 2055 6e69  l, axis_cfg: Uni
-00013690: 6f6e 5b64 6963 742c 206c 6973 742c 2074  on[dict, list, t
-000136a0: 7570 6c65 5d0a 2020 2020 2020 2020 293a  uple].        ):
-000136b0: 0a20 2020 2020 2020 2020 2020 2061 7869  .            axi
-000136c0: 735f 6366 6720 3d20 280a 2020 2020 2020  s_cfg = (.      
-000136d0: 2020 2020 2020 2020 2020 6178 6973 5f63            axis_c
-000136e0: 6667 0a20 2020 2020 2020 2020 2020 2020  fg.             
-000136f0: 2020 2069 6620 6e6f 7420 6973 696e 7374     if not isinst
-00013700: 616e 6365 2861 7869 735f 6366 672c 2028  ance(axis_cfg, (
-00013710: 6c69 7374 2c20 7475 706c 6529 290a 2020  list, tuple)).  
-00013720: 2020 2020 2020 2020 2020 2020 2020 656c                el
-00013730: 7365 2064 6963 7428 6c6f 6373 3d61 7869  se dict(locs=axi
-00013740: 735f 6366 6729 0a20 2020 2020 2020 2020  s_cfg).         
-00013750: 2020 2029 0a0a 2020 2020 2020 2020 2020     )..          
-00013760: 2020 6966 2061 7869 735f 6366 672e 6765    if axis_cfg.ge
-00013770: 7428 226c 6162 656c 7322 2920 616e 6420  t("labels") and 
-00013780: 6e6f 7420 6178 6973 5f63 6667 2e67 6574  not axis_cfg.get
-00013790: 2822 6c6f 6373 2229 3a0a 2020 2020 2020  ("locs"):.      
-000137a0: 2020 2020 2020 2020 2020 7261 6973 6520            raise 
-000137b0: 506c 6f74 436f 6e66 6967 4572 726f 7228  PlotConfigError(
-000137c0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000137d0: 2020 2020 2022 4c61 6265 6c73 2063 616e       "Labels can
-000137e0: 206f 6e6c 7920 6265 2073 6574 2074 6872   only be set thr
-000137f0: 6f75 6768 2074 6865 2060 6c61 6265 6c73  ough the `labels
-00013800: 6020 6172 6775 6d65 6e74 2022 0a20 2020  ` argument ".   
-00013810: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013820: 2022 6966 2074 6865 6972 206c 6f63 6174   "if their locat
-00013830: 696f 6e20 6973 2061 6c73 6f20 6769 7665  ion is also give
-00013840: 6e20 7468 726f 7567 6820 7468 6520 606c  n through the `l
-00013850: 6f63 7360 2022 0a20 2020 2020 2020 2020  ocs` ".         
-00013860: 2020 2020 2020 2020 2020 2022 6172 6775             "argu
-00013870: 6d65 6e74 2e20 486f 7765 7665 722c 2060  ment. However, `
-00013880: 6c6f 6373 6020 6973 206e 6f74 2067 6976  locs` is not giv
-00013890: 656e 2e22 0a20 2020 2020 2020 2020 2020  en.".           
-000138a0: 2020 2020 2029 0a0a 2020 2020 2020 2020       )..        
-000138b0: 2020 2020 2320 4765 7420 7468 6520 6178      # Get the ax
-000138c0: 6973 2073 7065 6369 6669 630a 2020 2020  is specific.    
-000138d0: 2020 2020 2020 2020 6966 2061 7869 7320          if axis 
-000138e0: 3d3d 2022 7822 3a0a 2020 2020 2020 2020  == "x":.        
-000138f0: 2020 2020 2020 2020 7469 636b 735f 6675          ticks_fu
-00013900: 6e63 203d 2073 656c 662e 6178 2e73 6574  nc = self.ax.set
-00013910: 5f78 7469 636b 730a 2020 2020 2020 2020  _xticks.        
-00013920: 2020 2020 2020 2020 7469 636b 736c 6162          tickslab
-00013930: 656c 5f66 756e 6320 3d20 7365 6c66 2e61  el_func = self.a
-00013940: 782e 7365 745f 7874 6963 6b6c 6162 656c  x.set_xticklabel
-00013950: 730a 2020 2020 2020 2020 2020 2020 656c  s.            el
-00013960: 6966 2061 7869 7320 3d3d 2022 7922 3a0a  if axis == "y":.
-00013970: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00013980: 7469 636b 735f 6675 6e63 203d 2073 656c  ticks_func = sel
-00013990: 662e 6178 2e73 6574 5f79 7469 636b 730a  f.ax.set_yticks.
-000139a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000139b0: 7469 636b 736c 6162 656c 5f66 756e 6320  tickslabel_func 
-000139c0: 3d20 7365 6c66 2e61 782e 7365 745f 7974  = self.ax.set_yt
-000139d0: 6963 6b6c 6162 656c 730a 2020 2020 2020  icklabels.      
-000139e0: 2020 2020 2020 656c 6966 2061 7869 7320        elif axis 
-000139f0: 3d3d 2022 7a22 3a0a 2020 2020 2020 2020  == "z":.        
-00013a00: 2020 2020 2020 2020 7469 636b 735f 6675          ticks_fu
-00013a10: 6e63 203d 2073 656c 662e 6178 2e73 6574  nc = self.ax.set
-00013a20: 5f7a 7469 636b 730a 2020 2020 2020 2020  _zticks.        
-00013a30: 2020 2020 2020 2020 7469 636b 736c 6162          tickslab
-00013a40: 656c 5f66 756e 6320 3d20 7365 6c66 2e61  el_func = self.a
-00013a50: 782e 7365 745f 7a74 6963 6b6c 6162 656c  x.set_zticklabel
-00013a60: 730a 0a20 2020 2020 2020 2020 2020 2023  s..            #
-00013a70: 2053 6574 2074 6865 2074 6963 6b73 0a20   Set the ticks. 
-00013a80: 2020 2020 2020 2020 2020 2073 6574 5f74             set_t
-00013a90: 6963 6b73 2874 6963 6b73 5f66 756e 632c  icks(ticks_func,
-00013aa0: 2074 6963 6b73 3d61 7869 735f 6366 672e   ticks=axis_cfg.
-00013ab0: 706f 7028 226c 6f63 7322 292c 206d 696e  pop("locs"), min
-00013ac0: 6f72 3d6d 696e 6f72 290a 0a20 2020 2020  or=minor)..     
-00013ad0: 2020 2020 2020 2023 2053 6574 2074 6865         # Set the
-00013ae0: 2074 6963 6b20 6c61 6265 6c73 2c20 7061   tick labels, pa
-00013af0: 7373 696e 6720 6f6e 2074 6865 2061 6464  ssing on the add
-00013b00: 6974 696f 6e61 6c20 6b77 6172 6773 0a20  itional kwargs. 
-00013b10: 2020 2020 2020 2020 2020 2069 6620 6178             if ax
-00013b20: 6973 5f63 6667 2e67 6574 2822 6c61 6265  is_cfg.get("labe
-00013b30: 6c73 2229 3a0a 2020 2020 2020 2020 2020  ls"):.          
-00013b40: 2020 2020 2020 7365 745f 7469 636b 6c61        set_tickla
-00013b50: 6265 6c73 2874 6963 6b73 6c61 6265 6c5f  bels(tickslabel_
-00013b60: 6675 6e63 2c20 6d69 6e6f 723d 6d69 6e6f  func, minor=mino
-00013b70: 722c 202a 2a61 7869 735f 6366 6729 0a0a  r, **axis_cfg)..
-00013b80: 2020 2020 2020 2020 6966 2078 3a0a 2020          if x:.  
-00013b90: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
-00013ba0: 6e73 7461 6e63 6528 782c 2028 6c69 7374  nstance(x, (list
-00013bb0: 2c20 7475 706c 6529 293a 0a20 2020 2020  , tuple)):.     
-00013bc0: 2020 2020 2020 2020 2020 2078 203d 2064             x = d
-00013bd0: 6963 7428 6d61 6a6f 723d 6469 6374 286c  ict(major=dict(l
-00013be0: 6f63 733d 7829 290a 0a20 2020 2020 2020  ocs=x))..       
-00013bf0: 2020 2020 2069 6620 782e 6765 7428 226d       if x.get("m
-00013c00: 616a 6f72 2229 2069 7320 6e6f 7420 4e6f  ajor") is not No
-00013c10: 6e65 3a0a 2020 2020 2020 2020 2020 2020  ne:.            
-00013c20: 2020 2020 7365 745f 7469 636b 735f 616e      set_ticks_an
-00013c30: 645f 6c61 6265 6c73 280a 2020 2020 2020  d_labels(.      
-00013c40: 2020 2020 2020 2020 2020 2020 2020 6178                ax
-00013c50: 6973 3d22 7822 2c20 6d69 6e6f 723d 4661  is="x", minor=Fa
-00013c60: 6c73 652c 2061 7869 735f 6366 673d 785b  lse, axis_cfg=x[
-00013c70: 226d 616a 6f72 225d 0a20 2020 2020 2020  "major"].       
-00013c80: 2020 2020 2020 2020 2029 0a0a 2020 2020           )..    
-00013c90: 2020 2020 2020 2020 6966 2078 2e67 6574          if x.get
-00013ca0: 2822 6d69 6e6f 7222 2920 6973 206e 6f74  ("minor") is not
-00013cb0: 204e 6f6e 653a 0a20 2020 2020 2020 2020   None:.         
-00013cc0: 2020 2020 2020 2073 6574 5f74 6963 6b73         set_ticks
-00013cd0: 5f61 6e64 5f6c 6162 656c 7328 6178 6973  _and_labels(axis
-00013ce0: 3d22 7822 2c20 6d69 6e6f 723d 5472 7565  ="x", minor=True
-00013cf0: 2c20 6178 6973 5f63 6667 3d78 5b22 6d69  , axis_cfg=x["mi
-00013d00: 6e6f 7222 5d29 0a0a 2020 2020 2020 2020  nor"])..        
-00013d10: 6966 2079 3a0a 2020 2020 2020 2020 2020  if y:.          
-00013d20: 2020 6966 2069 7369 6e73 7461 6e63 6528    if isinstance(
-00013d30: 792c 2028 6c69 7374 2c20 7475 706c 6529  y, (list, tuple)
-00013d40: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
-00013d50: 2020 2079 203d 2064 6963 7428 6d61 6a6f     y = dict(majo
-00013d60: 723d 6469 6374 286c 6f63 733d 7929 290a  r=dict(locs=y)).
-00013d70: 0a20 2020 2020 2020 2020 2020 2069 6620  .            if 
-00013d80: 792e 6765 7428 226d 616a 6f72 2229 2069  y.get("major") i
-00013d90: 7320 6e6f 7420 4e6f 6e65 3a0a 2020 2020  s not None:.    
-00013da0: 2020 2020 2020 2020 2020 2020 7365 745f              set_
-00013db0: 7469 636b 735f 616e 645f 6c61 6265 6c73  ticks_and_labels
-00013dc0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
-00013dd0: 2020 2020 2020 6178 6973 3d22 7922 2c20        axis="y", 
-00013de0: 6d69 6e6f 723d 4661 6c73 652c 2061 7869  minor=False, axi
-00013df0: 735f 6366 673d 795b 226d 616a 6f72 225d  s_cfg=y["major"]
-00013e00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00013e10: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
-00013e20: 6966 2079 2e67 6574 2822 6d69 6e6f 7222  if y.get("minor"
-00013e30: 2920 6973 206e 6f74 204e 6f6e 653a 0a20  ) is not None:. 
-00013e40: 2020 2020 2020 2020 2020 2020 2020 2073                 s
-00013e50: 6574 5f74 6963 6b73 5f61 6e64 5f6c 6162  et_ticks_and_lab
-00013e60: 656c 7328 6178 6973 3d22 7922 2c20 6d69  els(axis="y", mi
-00013e70: 6e6f 723d 5472 7565 2c20 6178 6973 5f63  nor=True, axis_c
-00013e80: 6667 3d79 5b22 6d69 6e6f 7222 5d29 0a0a  fg=y["minor"])..
-00013e90: 2020 2020 2020 2020 6966 2068 6173 6174          if hasat
-00013ea0: 7472 2873 656c 662e 6178 2c20 227a 6178  tr(self.ax, "zax
-00013eb0: 6973 2229 3a0a 2020 2020 2020 2020 2020  is"):.          
-00013ec0: 2020 6966 207a 3a0a 2020 2020 2020 2020    if z:.        
-00013ed0: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
-00013ee0: 7461 6e63 6528 7a2c 2028 6c69 7374 2c20  tance(z, (list, 
-00013ef0: 7475 706c 6529 293a 0a20 2020 2020 2020  tuple)):.       
-00013f00: 2020 2020 2020 2020 2020 2020 207a 203d               z =
-00013f10: 2064 6963 7428 6d61 6a6f 723d 6469 6374   dict(major=dict
-00013f20: 286c 6f63 733d 7a29 290a 0a20 2020 2020  (locs=z))..     
-00013f30: 2020 2020 2020 2020 2020 2069 6620 7a2e             if z.
-00013f40: 6765 7428 226d 616a 6f72 2229 2069 7320  get("major") is 
-00013f50: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
-00013f60: 2020 2020 2020 2020 2020 2020 2020 7365                se
-00013f70: 745f 7469 636b 735f 616e 645f 6c61 6265  t_ticks_and_labe
-00013f80: 6c73 280a 2020 2020 2020 2020 2020 2020  ls(.            
-00013f90: 2020 2020 2020 2020 2020 2020 6178 6973              axis
-00013fa0: 3d22 7a22 2c20 6d69 6e6f 723d 4661 6c73  ="z", minor=Fals
-00013fb0: 652c 2061 7869 735f 6366 673d 7a5b 226d  e, axis_cfg=z["m
-00013fc0: 616a 6f72 225d 0a20 2020 2020 2020 2020  ajor"].         
-00013fd0: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
-00013fe0: 2020 2020 2020 2020 2020 2020 2020 6966                if
-00013ff0: 207a 2e67 6574 2822 6d69 6e6f 7222 2920   z.get("minor") 
-00014000: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
-00014010: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014020: 2073 6574 5f74 6963 6b73 5f61 6e64 5f6c   set_ticks_and_l
-00014030: 6162 656c 7328 0a20 2020 2020 2020 2020  abels(.         
-00014040: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00014050: 7869 733d 227a 222c 206d 696e 6f72 3d54  xis="z", minor=T
-00014060: 7275 652c 2061 7869 735f 6366 673d 7a5b  rue, axis_cfg=z[
-00014070: 226d 696e 6f72 225d 0a20 2020 2020 2020  "minor"].       
-00014080: 2020 2020 2020 2020 2020 2020 2029 0a0a               )..
-00014090: 2020 2020 6465 6620 5f68 6c70 725f 7365      def _hlpr_se
-000140a0: 745f 7469 636b 5f6c 6f63 6174 6f72 7328  t_tick_locators(
-000140b0: 0a20 2020 2020 2020 2073 656c 662c 202a  .        self, *
-000140c0: 2c20 783a 2064 6963 7420 3d20 4e6f 6e65  , x: dict = None
-000140d0: 2c20 793a 2064 6963 7420 3d20 4e6f 6e65  , y: dict = None
-000140e0: 2c20 7a3a 2064 6963 7420 3d20 4e6f 6e65  , z: dict = None
-000140f0: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-00014100: 2222 2253 6574 7320 7468 6520 7469 636b  """Sets the tick
-00014110: 206c 6f63 6174 6f72 7320 666f 7220 7468   locators for th
-00014120: 6520 6375 7272 656e 7420 6178 6973 0a0a  e current axis..
-00014130: 2020 2020 2020 2020 5468 6520 6172 6775          The argu
-00014140: 6d65 6e74 7320 6172 6520 7573 6564 2074  ments are used t
-00014150: 6f20 6361 6c6c 0a20 2020 2020 2020 2060  o call.        `
-00014160: 6061 782e 7b78 2c79 2c20 7a7d 6178 6973  `ax.{x,y, z}axis
-00014170: 2e73 6574 5f7b 6d61 6a6f 722f 6d69 6e6f  .set_{major/mino
-00014180: 727d 5f6c 6f63 6174 6f72 6060 2c20 7265  r}_locator``, re
-00014190: 7370 6563 7469 7665 6c79 2e0a 2020 2020  spectively..    
-000141a0: 2020 2020 5468 6520 6469 6374 2d6c 696b      The dict-lik
-000141b0: 6520 6172 6775 6d65 6e74 7320 6d75 7374  e arguments must
-000141c0: 2063 6f6e 7461 696e 2074 6865 206b 6579   contain the key
-000141d0: 7320 6060 6d61 6a6f 7260 6020 616e 642f  s ``major`` and/
-000141e0: 6f72 0a20 2020 2020 2020 2060 606d 696e  or.        ``min
-000141f0: 6f72 6060 2c20 7265 6665 7272 696e 6720  or``, referring 
-00014200: 746f 206d 616a 6f72 206f 7220 6d69 6e6f  to major or mino
-00014210: 7220 7469 636b 206c 6f63 6174 6f72 732e  r tick locators.
-00014220: 2054 6865 7365 206e 6565 6420 746f 0a20   These need to. 
-00014230: 2020 2020 2020 2073 7065 6369 6679 2061         specify a
-00014240: 206e 616d 6520 7468 6174 2069 7320 6c6f   name that is lo
-00014250: 6f6b 6564 2075 7020 696e 203a 7079 3a6d  oked up in :py:m
-00014260: 6f64 3a60 6d61 7470 6c6f 746c 6962 2e74  od:`matplotlib.t
-00014270: 6963 6b65 7260 2e0a 2020 2020 2020 2020  icker`..        
-00014280: 5468 6579 2063 616e 2063 6f6e 7461 696e  They can contain
-00014290: 2061 206c 6973 742d 6c69 6b65 2060 6061   a list-like ``a
-000142a0: 7267 7360 6020 6b65 7977 6f72 6420 6172  rgs`` keyword ar
-000142b0: 6775 6d65 6e74 2074 6861 7420 6465 6669  gument that defi
-000142c0: 6e65 730a 2020 2020 2020 2020 7468 6520  nes.        the 
-000142d0: 6172 6775 6d65 6e74 7320 746f 2070 6173  arguments to pas
-000142e0: 7320 6f6e 2061 7320 706f 7369 7469 6f6e  s on as position
-000142f0: 616c 2061 7267 7320 746f 2074 6865 2063  al args to the c
-00014300: 616c 6c65 6420 6675 6e63 7469 6f6e 2e0a  alled function..
-00014310: 2020 2020 2020 2020 4675 7274 6865 7220          Further 
-00014320: 6b77 6172 6773 2061 7265 2070 6173 7365  kwargs are passe
-00014330: 6420 6f6e 2074 6f0a 2020 2020 2020 2020  d on to.        
-00014340: 6060 6178 2e7b 782c 792c 207a 7d61 7869  ``ax.{x,y, z}axi
-00014350: 732e 7365 745f 7b6d 616a 6f72 2f6d 696e  s.set_{major/min
-00014360: 6f72 7d5f 6c6f 6361 746f 7260 602e 0a0a  or}_locator``...
-00014370: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
-00014380: 0a0a 2020 2020 2020 2020 2e2e 2063 6f64  ..        .. cod
-00014390: 652d 626c 6f63 6b3a 3a20 7961 6d6c 0a0a  e-block:: yaml..
-000143a0: 2020 2020 2020 2020 2020 2020 7365 745f              set_
-000143b0: 7469 636b 5f6c 6f63 6174 6f72 733a 0a20  tick_locators:. 
-000143c0: 2020 2020 2020 2020 2020 2020 2078 3a0a               x:.
-000143d0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000143e0: 6d61 6a6f 723a 0a20 2020 2020 2020 2020  major:.         
-000143f0: 2020 2020 2020 2020 206e 616d 653a 204d           name: M
-00014400: 6178 4e4c 6f63 6174 6f72 2020 2020 2320  axNLocator    # 
-00014410: 6c6f 6f6b 6564 2075 7020 6672 6f6d 206d  looked up from m
-00014420: 6174 706c 6f74 6c69 622e 7469 636b 6572  atplotlib.ticker
-00014430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014440: 2020 206e 6269 6e73 3a20 360a 2020 2020     nbins: 6.    
-00014450: 2020 2020 2020 2020 2020 2020 2020 696e                in
-00014460: 7465 6765 723a 2074 7275 650a 2020 2020  teger: true.    
-00014470: 2020 2020 2020 2020 2020 2020 2020 6d69                mi
-00014480: 6e5f 6e5f 7469 636b 733a 2033 0a20 2020  n_n_ticks: 3.   
-00014490: 2020 2020 2020 2020 2020 2079 3a0a 2020             y:.  
-000144a0: 2020 2020 2020 2020 2020 2020 2020 6d61                ma
-000144b0: 6a6f 723a 0a20 2020 2020 2020 2020 2020  jor:.           
-000144c0: 2020 2020 2020 206e 616d 653a 204d 756c         name: Mul
-000144d0: 7469 706c 654c 6f63 6174 6f72 0a20 2020  tipleLocator.   
-000144e0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-000144f0: 7267 733a 205b 325d 0a0a 0a20 2020 2020  rgs: [2]...     
-00014500: 2020 2046 6f72 206d 6f72 6520 696e 666f     For more info
-00014510: 726d 6174 696f 6e2c 2073 6565 3a0a 0a20  rmation, see:.. 
-00014520: 2020 2020 2020 2020 2020 202d 2068 7474             - htt
-00014530: 7073 3a2f 2f6d 6174 706c 6f74 6c69 622e  ps://matplotlib.
-00014540: 6f72 672f 6761 6c6c 6572 792f 7469 636b  org/gallery/tick
-00014550: 735f 616e 645f 7370 696e 6573 2f74 6963  s_and_spines/tic
-00014560: 6b2d 6c6f 6361 746f 7273 2e68 746d 6c0a  k-locators.html.
-00014570: 2020 2020 2020 2020 2020 2020 2d20 6874              - ht
-00014580: 7470 733a 2f2f 6d61 7470 6c6f 746c 6962  tps://matplotlib
-00014590: 2e6f 7267 2f61 7069 2f5f 6173 5f67 656e  .org/api/_as_gen
-000145a0: 2f6d 6174 706c 6f74 6c69 622e 6178 6973  /matplotlib.axis
-000145b0: 2e41 7869 732e 7365 745f 6d61 6a6f 725f  .Axis.set_major_
-000145c0: 6c6f 6361 746f 722e 6874 6d6c 0a20 2020  locator.html.   
-000145d0: 2020 2020 2020 2020 202d 2068 7474 7073           - https
-000145e0: 3a2f 2f6d 6174 706c 6f74 6c69 622e 6f72  ://matplotlib.or
-000145f0: 672f 6170 692f 5f61 735f 6765 6e2f 6d61  g/api/_as_gen/ma
-00014600: 7470 6c6f 746c 6962 2e61 7869 732e 4178  tplotlib.axis.Ax
-00014610: 6973 2e73 6574 5f6d 696e 6f72 5f6c 6f63  is.set_minor_loc
-00014620: 6174 6f72 2e68 746d 6c0a 0a20 2020 2020  ator.html..     
-00014630: 2020 2041 7267 733a 0a20 2020 2020 2020     Args:.       
-00014640: 2020 2020 2078 2028 6469 6374 2c20 6f70       x (dict, op
-00014650: 7469 6f6e 616c 293a 2054 6865 2063 6f6e  tional): The con
-00014660: 6669 6775 7261 7469 6f6e 206f 6620 7468  figuration of th
-00014670: 6520 782d 6178 6973 2074 6963 6b20 6c6f  e x-axis tick lo
-00014680: 6361 746f 720a 2020 2020 2020 2020 2020  cator.          
-00014690: 2020 7920 2864 6963 742c 206f 7074 696f    y (dict, optio
-000146a0: 6e61 6c29 3a20 5468 6520 636f 6e66 6967  nal): The config
-000146b0: 7572 6174 696f 6e20 6f66 2074 6865 2079  uration of the y
-000146c0: 2d61 7869 7320 7469 636b 206c 6f63 6174  -axis tick locat
-000146d0: 6f72 0a20 2020 2020 2020 2020 2020 207a  or.            z
-000146e0: 2028 6469 6374 2c20 6f70 7469 6f6e 616c   (dict, optional
-000146f0: 293a 2054 6865 2063 6f6e 6669 6775 7261  ): The configura
-00014700: 7469 6f6e 206f 6620 7468 6520 7a2d 6178  tion of the z-ax
-00014710: 6973 2074 6963 6b20 6c6f 6361 746f 722e  is tick locator.
-00014720: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014730: 2049 6620 7468 6572 6520 6973 206e 6f20   If there is no 
-00014740: 7a2d 6178 6973 2c20 7468 6973 2077 696c  z-axis, this wil
-00014750: 6c20 6265 2073 696c 656e 746c 7920 6967  l be silently ig
-00014760: 6e6f 7265 642e 0a20 2020 2020 2020 2022  nored..        "
-00014770: 2222 0a20 2020 2020 2020 2073 6574 5f74  "".        set_t
-00014780: 6963 6b5f 6c6f 6361 746f 7273 5f6f 725f  ick_locators_or_
-00014790: 666f 726d 6174 7465 7273 280a 2020 2020  formatters(.    
-000147a0: 2020 2020 2020 2020 6178 3d73 656c 662e          ax=self.
-000147b0: 6178 2c20 6b69 6e64 3d22 6c6f 6361 746f  ax, kind="locato
-000147c0: 7222 2c20 783d 782c 2079 3d79 2c20 7a3d  r", x=x, y=y, z=
-000147d0: 7a0a 2020 2020 2020 2020 290a 0a20 2020  z.        )..   
-000147e0: 2064 6566 205f 686c 7072 5f73 6574 5f74   def _hlpr_set_t
-000147f0: 6963 6b5f 666f 726d 6174 7465 7273 280a  ick_formatters(.
-00014800: 2020 2020 2020 2020 7365 6c66 2c20 2a2c          self, *,
-00014810: 2078 3a20 6469 6374 203d 204e 6f6e 652c   x: dict = None,
-00014820: 2079 3a20 6469 6374 203d 204e 6f6e 652c   y: dict = None,
-00014830: 207a 3a20 6469 6374 203d 204e 6f6e 650a   z: dict = None.
-00014840: 2020 2020 293a 0a20 2020 2020 2020 2022      ):.        "
-00014850: 2222 5365 7473 2074 6865 2074 6963 6b20  ""Sets the tick 
-00014860: 666f 726d 6174 7465 7273 2066 6f72 2074  formatters for t
-00014870: 6865 2063 7572 7265 6e74 2061 7869 730a  he current axis.
-00014880: 0a20 2020 2020 2020 2054 6865 2061 7267  .        The arg
-00014890: 756d 656e 7473 2061 7265 2075 7365 6420  uments are used 
-000148a0: 746f 2063 616c 6c0a 2020 2020 2020 2020  to call.        
-000148b0: 6060 6178 2e7b 782c 792c 207a 7d61 7869  ``ax.{x,y, z}axi
-000148c0: 732e 7365 745f 7b6d 616a 6f72 2f6d 696e  s.set_{major/min
-000148d0: 6f72 7d5f 666f 726d 6174 7465 7260 602c  or}_formatter``,
-000148e0: 2072 6573 7065 6374 6976 656c 792e 2054   respectively. T
-000148f0: 6865 0a20 2020 2020 2020 2064 6963 742d  he.        dict-
-00014900: 6c69 6b65 2061 7267 756d 656e 7473 206d  like arguments m
-00014910: 7573 7420 636f 6e74 6169 6e20 7468 6520  ust contain the 
-00014920: 6b65 7973 2060 606d 616a 6f72 6060 2061  keys ``major`` a
-00014930: 6e64 2f6f 7220 6060 6d69 6e6f 7260 602c  nd/or ``minor``,
-00014940: 0a20 2020 2020 2020 2072 6566 6572 7269  .        referri
-00014950: 6e67 2074 6f20 6d61 6a6f 7220 6f72 206d  ng to major or m
-00014960: 696e 6f72 2074 6963 6b20 666f 726d 6174  inor tick format
-00014970: 7465 7273 2e20 5468 6573 6520 6e65 6564  ters. These need
-00014980: 2074 6f20 7370 6563 6966 7920 610a 2020   to specify a.  
-00014990: 2020 2020 2020 6e61 6d65 2074 6861 7420        name that 
-000149a0: 6973 206c 6f6f 6b65 6420 7570 2069 6e20  is looked up in 
-000149b0: 3a70 793a 6d6f 643a 606d 6174 706c 6f74  :py:mod:`matplot
-000149c0: 6c69 622e 7469 636b 6572 602e 0a20 2020  lib.ticker`..   
-000149d0: 2020 2020 2054 6865 7920 6361 6e20 636f       They can co
-000149e0: 6e74 6169 6e20 6120 6c69 7374 2d6c 696b  ntain a list-lik
-000149f0: 6520 6060 6172 6773 6060 206b 6579 776f  e ``args`` keywo
-00014a00: 7264 2061 7267 756d 656e 7420 7468 6174  rd argument that
-00014a10: 2064 6566 696e 6573 0a20 2020 2020 2020   defines.       
-00014a20: 2074 6865 2061 7267 756d 656e 7473 2074   the arguments t
-00014a30: 6f20 7061 7373 206f 6e20 6173 2070 6f73  o pass on as pos
-00014a40: 6974 696f 6e61 6c20 6172 6773 2074 6f20  itional args to 
-00014a50: 7468 6520 6361 6c6c 6564 2066 756e 6374  the called funct
-00014a60: 696f 6e2e 0a20 2020 2020 2020 2046 7572  ion..        Fur
-00014a70: 7468 6572 206b 7761 7267 7320 6172 6520  ther kwargs are 
-00014a80: 7061 7373 6564 206f 6e20 746f 0a20 2020  passed on to.   
-00014a90: 2020 2020 2060 6061 782e 7b78 2c79 2c20       ``ax.{x,y, 
-00014aa0: 7a7d 6178 6973 2e73 6574 5f7b 6d61 6a6f  z}axis.set_{majo
-00014ab0: 722f 6d69 6e6f 727d 5f66 6f72 6d61 7474  r/minor}_formatt
-00014ac0: 6572 6060 2e0a 0a20 2020 2020 2020 2045  er``...        E
-00014ad0: 7861 6d70 6c65 3a0a 0a20 2020 2020 2020  xample:..       
-00014ae0: 202e 2e20 636f 6465 2d62 6c6f 636b 3a3a   .. code-block::
-00014af0: 2079 616d 6c0a 0a20 2020 2020 2020 2020   yaml..         
-00014b00: 2020 2073 6574 5f74 6963 6b5f 666f 726d     set_tick_form
-00014b10: 6174 7465 7273 3a0a 2020 2020 2020 2020  atters:.        
-00014b20: 2020 2020 2020 783a 0a20 2020 2020 2020        x:.       
-00014b30: 2020 2020 2020 2020 206d 616a 6f72 3a0a           major:.
-00014b40: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014b50: 2020 6e61 6d65 3a20 5374 724d 6574 686f    name: StrMetho
-00014b60: 6446 6f72 6d61 7474 6572 0a20 2020 2020  dFormatter.     
-00014b70: 2020 2020 2020 2020 2020 2020 2061 7267               arg
-00014b80: 733a 205b 277b 783a 2e33 677d 275d 0a20  s: ['{x:.3g}']. 
-00014b90: 2020 2020 2020 2020 2020 2020 2079 3a0a               y:.
-00014ba0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00014bb0: 6d61 6a6f 723a 0a20 2020 2020 2020 2020  major:.         
-00014bc0: 2020 2020 2020 2020 206e 616d 653a 2046           name: F
-00014bd0: 756e 6346 6f72 6d61 7474 6572 0a20 2020  uncFormatter.   
-00014be0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00014bf0: 7267 733a 205b 2164 6167 5f72 6573 756c  rgs: [!dag_resul
-00014c00: 7420 6d79 5f66 6f72 6d61 7474 6572 5f6c  t my_formatter_l
-00014c10: 616d 6264 615d 0a20 2020 2020 2020 2020  ambda].         
-00014c20: 2020 2020 2020 2020 2023 2061 6e79 206b           # any k
-00014c30: 7761 7267 7320 6865 7265 2070 6173 7365  wargs here passe
-00014c40: 6420 616c 736f 2074 6f20 4675 6e63 466f  d also to FuncFo
-00014c50: 726d 6174 7465 720a 0a20 2020 2020 2020  rmatter..       
-00014c60: 2020 2020 2020 207a 3a0a 2020 2020 2020         z:.      
-00014c70: 2020 2020 2020 2020 2020 6d61 6a6f 723a            major:
-00014c80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00014c90: 2020 206e 616d 653a 2044 6174 6546 6f72     name: DateFor
-00014ca0: 6d61 7474 6572 2020 2320 6c6f 6f6b 6564  matter  # looked
-00014cb0: 2075 7020 6672 6f6d 206d 6174 706c 6f74   up from matplot
-00014cc0: 6c69 622e 6461 7465 730a 2020 2020 2020  lib.dates.      
-00014cd0: 2020 2020 2020 2020 2020 2020 6172 6773              args
-00014ce0: 3a20 5b22 2548 3a25 4d3a 2553 225d 2020  : ["%H:%M:%S"]  
-00014cf0: 2320 6f72 2022 2559 2d25 6d2d 2564 220a  # or "%Y-%m-%d".
-00014d00: 0a20 2020 2020 2020 2046 6f72 206d 6f72  .        For mor
-00014d10: 6520 696e 666f 726d 6174 696f 6e2c 2073  e information, s
-00014d20: 6565 3a0a 0a20 2020 2020 2020 2020 2020  ee:..           
-00014d30: 202d 2068 7474 7073 3a2f 2f6d 6174 706c   - https://matpl
-00014d40: 6f74 6c69 622e 6f72 672f 6761 6c6c 6572  otlib.org/galler
-00014d50: 792f 7469 636b 735f 616e 645f 7370 696e  y/ticks_and_spin
-00014d60: 6573 2f74 6963 6b2d 666f 726d 6174 7465  es/tick-formatte
-00014d70: 7273 2e68 746d 6c0a 2020 2020 2020 2020  rs.html.        
-00014d80: 2020 2020 2d20 6874 7470 733a 2f2f 6d61      - https://ma
-00014d90: 7470 6c6f 746c 6962 2e6f 7267 2f61 7069  tplotlib.org/api
-00014da0: 2f5f 6173 5f67 656e 2f6d 6174 706c 6f74  /_as_gen/matplot
-00014db0: 6c69 622e 6178 6973 2e41 7869 732e 7365  lib.axis.Axis.se
-00014dc0: 745f 6d61 6a6f 725f 666f 726d 6174 7465  t_major_formatte
-00014dd0: 722e 6874 6d6c 0a20 2020 2020 2020 2020  r.html.         
-00014de0: 2020 202d 2068 7474 7073 3a2f 2f6d 6174     - https://mat
-00014df0: 706c 6f74 6c69 622e 6f72 672f 6170 692f  plotlib.org/api/
-00014e00: 5f61 735f 6765 6e2f 6d61 7470 6c6f 746c  _as_gen/matplotl
-00014e10: 6962 2e61 7869 732e 4178 6973 2e73 6574  ib.axis.Axis.set
-00014e20: 5f6d 696e 6f72 5f66 6f72 6d61 7474 6572  _minor_formatter
-00014e30: 2e68 746d 6c0a 0a20 2020 2020 2020 2041  .html..        A
-00014e40: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
-00014e50: 2078 2028 6469 6374 2c20 6f70 7469 6f6e   x (dict, option
-00014e60: 616c 293a 2054 6865 2063 6f6e 6669 6775  al): The configu
-00014e70: 7261 7469 6f6e 206f 6620 7468 6520 782d  ration of the x-
-00014e80: 6178 6973 2074 6963 6b20 666f 726d 6174  axis tick format
-00014e90: 7465 720a 2020 2020 2020 2020 2020 2020  ter.            
-00014ea0: 7920 2864 6963 742c 206f 7074 696f 6e61  y (dict, optiona
-00014eb0: 6c29 3a20 5468 6520 636f 6e66 6967 7572  l): The configur
-00014ec0: 6174 696f 6e20 6f66 2074 6865 2079 2d61  ation of the y-a
-00014ed0: 7869 7320 7469 636b 2066 6f72 6d61 7474  xis tick formatt
-00014ee0: 6572 0a20 2020 2020 2020 2020 2020 207a  er.            z
-00014ef0: 2028 6469 6374 2c20 6f70 7469 6f6e 616c   (dict, optional
-00014f00: 293a 2054 6865 2063 6f6e 6669 6775 7261  ): The configura
-00014f10: 7469 6f6e 206f 6620 7468 6520 7a2d 6178  tion of the z-ax
-00014f20: 6973 2074 6963 6b20 666f 726d 6174 7465  is tick formatte
-00014f30: 722e 0a20 2020 2020 2020 2020 2020 2020  r..             
-00014f40: 2020 2049 6620 7468 6572 6520 6973 206e     If there is n
-00014f50: 6f20 7a2d 6178 6973 2c20 7468 6973 2077  o z-axis, this w
-00014f60: 696c 6c20 6265 2073 696c 656e 746c 7920  ill be silently 
-00014f70: 6967 6e6f 7265 642e 0a20 2020 2020 2020  ignored..       
-00014f80: 2022 2222 0a20 2020 2020 2020 2073 6574   """.        set
-00014f90: 5f74 6963 6b5f 6c6f 6361 746f 7273 5f6f  _tick_locators_o
-00014fa0: 725f 666f 726d 6174 7465 7273 280a 2020  r_formatters(.  
-00014fb0: 2020 2020 2020 2020 2020 6178 3d73 656c            ax=sel
-00014fc0: 662e 6178 2c20 6b69 6e64 3d22 666f 726d  f.ax, kind="form
-00014fd0: 6174 7465 7222 2c20 783d 782c 2079 3d79  atter", x=x, y=y
-00014fe0: 2c20 7a3d 7a0a 2020 2020 2020 2020 290a  , z=z.        ).
-00014ff0: 0a20 2020 2064 6566 205f 686c 7072 5f63  .    def _hlpr_c
-00015000: 616c 6c28 0a20 2020 2020 2020 2073 656c  all(.        sel
-00015010: 662c 0a20 2020 2020 2020 202a 2c0a 2020  f,.        *,.  
-00015020: 2020 2020 2020 6675 6e63 7469 6f6e 733a        functions:
-00015030: 2053 6571 7565 6e63 655b 6469 6374 5d2c   Sequence[dict],
-00015040: 0a20 2020 2020 2020 2066 756e 6373 5f6c  .        funcs_l
-00015050: 6f6f 6b75 705f 6469 6374 3a20 4469 6374  ookup_dict: Dict
-00015060: 5b73 7472 2c20 4361 6c6c 6162 6c65 5d20  [str, Callable] 
-00015070: 3d20 4e6f 6e65 2c0a 2020 2020 2020 2020  = None,.        
-00015080: 2a2a 7368 6172 6564 5f6b 7761 7267 732c  **shared_kwargs,
-00015090: 0a20 2020 2029 3a0a 2020 2020 2020 2020  .    ):.        
-000150a0: 2222 2241 7869 732d 6c65 7665 6c20 6865  """Axis-level he
-000150b0: 6c70 6572 2074 6861 7420 6361 6e20 6265  lper that can be
-000150c0: 2075 7365 6420 746f 2063 616c 6c20 6d75   used to call mu
-000150d0: 6c74 6970 6c65 2066 756e 6374 696f 6e73  ltiple functions
-000150e0: 2e0a 0a20 2020 2020 2020 2046 756e 6374  ...        Funct
-000150f0: 696f 6e73 2063 616e 2062 6520 7370 6563  ions can be spec
-00015100: 6966 6965 6420 696e 2074 6872 6565 2077  ified in three w
-00015110: 6179 733a 0a0a 2020 2020 2020 2020 2020  ays:..          
-00015120: 2020 2d20 6173 2073 7472 696e 672c 2062    - as string, b
-00015130: 6569 6e67 206c 6f6f 6b65 6420 7570 2066  eing looked up f
-00015140: 726f 6d20 6120 7072 652d 6465 6669 6e65  rom a pre-define
-00015150: 6420 6469 6374 0a20 2020 2020 2020 2020  d dict.         
-00015160: 2020 202d 2061 7320 322d 7475 706c 6520     - as 2-tuple 
-00015170: 6060 286d 6f64 756c 652c 206e 616d 6529  ``(module, name)
-00015180: 6060 2077 6869 6368 2077 696c 6c20 6265  `` which will be
-00015190: 2069 6d70 6f72 7465 6420 6f6e 2074 6865   imported on the
-000151a0: 2066 6c79 0a20 2020 2020 2020 2020 2020   fly.           
-000151b0: 202d 2061 7320 6361 6c6c 6162 6c65 2c20   - as callable, 
-000151c0: 7768 6963 6820 7769 6c6c 2062 6520 7573  which will be us
-000151d0: 6564 2064 6972 6563 746c 790a 0a20 2020  ed directly..   
-000151e0: 2020 2020 2054 6865 2069 6d70 6c65 6d65       The impleme
-000151f0: 6e74 6174 696f 6e20 6f66 2074 6869 7320  ntation of this 
-00015200: 6973 2073 6861 7265 6420 7769 7468 2074  is shared with t
-00015210: 6865 2070 6c6f 7420 6675 6e63 7469 6f6e  he plot function
-00015220: 0a20 2020 2020 2020 203a 7079 3a66 756e  .        :py:fun
-00015230: 633a 607e 6461 6e74 726f 2e70 6c6f 742e  c:`~dantro.plot.
-00015240: 6675 6e63 732e 6d75 6c74 6970 6c6f 742e  funcs.multiplot.
-00015250: 6d75 6c74 6970 6c6f 7460 2e20 5365 650a  multiplot`. See.
-00015260: 2020 2020 2020 2020 7468 6572 6520 666f          there fo
-00015270: 7220 6d6f 7265 2069 6e66 6f72 6d61 7469  r more informati
-00015280: 6f6e 2e0a 0a20 2020 2020 2020 2054 6865  on...        The
-00015290: 2066 6967 7572 652d 6c65 7665 6c20 6865   figure-level he
-000152a0: 6c70 6572 2060 6066 6967 6361 6c6c 6060  lper ``figcall``
-000152b0: 2069 7320 6964 656e 7469 6361 6c20 746f   is identical to
-000152c0: 2074 6869 7320 6865 6c70 6572 2c20 6275   this helper, bu
-000152d0: 7420 6973 0a20 2020 2020 2020 2069 6e76  t is.        inv
-000152e0: 6f6b 6564 202a 6265 666f 7265 2a20 7468  oked *before* th
-000152f0: 6520 6178 6973 2d73 7065 6369 6669 6320  e axis-specific 
-00015300: 6865 6c70 6572 7320 6172 6520 696e 766f  helpers are invo
-00015310: 6b65 642e 0a0a 2020 2020 2020 2020 2e2e  ked...        ..
-00015320: 2068 696e 743a 3a0a 0a20 2020 2020 2020   hint::..       
-00015330: 2020 2020 2054 6f20 7061 7373 2063 7573       To pass cus
-00015340: 746f 6d20 6361 6c6c 6162 6c65 732c 2075  tom callables, u
-00015350: 7365 2074 6865 2064 6174 6120 7472 616e  se the data tran
-00015360: 7366 6f72 6d61 7469 6f6e 2066 7261 6d65  sformation frame
-00015370: 776f 726b 2061 6e64 0a20 2020 2020 2020  work and.       
-00015380: 2020 2020 2074 6865 2060 6021 6461 675f       the ``!dag_
-00015390: 7265 7375 6c74 6060 2070 6c61 6365 686f  result`` placeho
-000153a0: 6c64 6572 2c20 7365 6520 3a72 6566 3a60  lder, see :ref:`
-000153b0: 6461 675f 7265 7375 6c74 5f70 6c61 6365  dag_result_place
-000153c0: 686f 6c64 6572 602e 0a0a 2020 2020 2020  holder`...      
-000153d0: 2020 2e2e 206e 6f74 653a 3a0a 0a20 2020    .. note::..   
-000153e0: 2020 2020 2020 2020 2057 6869 6c65 206d           While m
-000153f0: 6f73 7420 6d61 7470 6c6f 746c 6962 2d62  ost matplotlib-b
-00015400: 6173 6564 2066 756e 6374 696f 6e73 2077  ased functions w
-00015410: 696c 6c20 6175 746f 6d61 7469 6361 6c6c  ill automaticall
-00015420: 7920 6f70 6572 6174 6520 6f6e 0a20 2020  y operate on.   
-00015430: 2020 2020 2020 2020 2074 6865 2063 7572           the cur
-00015440: 7265 6e74 2061 7869 732c 2073 6f6d 6520  rent axis, some 
-00015450: 6675 6e63 7469 6f6e 2063 616c 6c73 206d  function calls m
-00015460: 6179 2072 6571 7569 7265 2061 6e20 6178  ay require an ax
-00015470: 6973 206f 626a 6563 742e 0a20 2020 2020  is object..     
-00015480: 2020 2020 2020 2049 6620 736f 2c20 7573         If so, us
-00015490: 6520 7468 6520 6060 7061 7373 5f61 7869  e the ``pass_axi
-000154a0: 735f 6f62 6a65 6374 5f61 7360 6020 6172  s_object_as`` ar
-000154b0: 6775 6d65 6e74 2c20 7768 6963 6820 7370  gument, which sp
-000154c0: 6563 6966 6965 730a 2020 2020 2020 2020  ecifies.        
-000154d0: 2020 2020 7468 6520 6e61 6d65 206f 6620      the name of 
-000154e0: 7468 6520 6b65 7977 6f72 6420 6172 6775  the keyword argu
-000154f0: 6d65 6e74 2061 7320 7768 6963 6820 7468  ment as which th
-00015500: 6520 6375 7272 656e 7420 6178 6973 2069  e current axis i
-00015510: 730a 2020 2020 2020 2020 2020 2020 7061  s.            pa
-00015520: 7373 6564 2074 6f20 7468 6520 6675 6e63  ssed to the func
-00015530: 7469 6f6e 2063 616c 6c2e 0a0a 2020 2020  tion call...    
-00015540: 2020 2020 4578 616d 706c 653a 0a0a 2020      Example:..  
-00015550: 2020 2020 2020 2e2e 2063 6f64 652d 626c        .. code-bl
-00015560: 6f63 6b3a 3a20 7961 6d6c 0a0a 2020 2020  ock:: yaml..    
-00015570: 2020 2020 2020 2020 6361 6c6c 3a0a 2020          call:.  
-00015580: 2020 2020 2020 2020 2020 2020 6675 6e63              func
-00015590: 7469 6f6e 733a 0a20 2020 2020 2020 2020  tions:.         
-000155a0: 2020 2020 2020 2023 204c 6f6f 6b20 7570         # Look up
-000155b0: 2066 756e 6374 696f 6e20 6672 6f6d 2064   function from d
-000155c0: 6963 742c 2063 6f6e 7461 696e 696e 6720  ict, containing 
-000155d0: 636f 6d6d 6f6e 2073 6561 626f 726e 2061  common seaborn a
-000155e0: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
-000155f0: 2020 2023 2070 7970 6c6f 7420 706c 6f74     # pyplot plot
-00015600: 7469 6e67 2066 756e 6374 696f 6e73 2028  ting functions (
-00015610: 7365 6520 6d75 6c74 6970 6c6f 7420 666f  see multiplot fo
-00015620: 7220 6d6f 7265 2069 6e66 6f29 0a20 2020  r more info).   
-00015630: 2020 2020 2020 2020 2020 2020 202d 2066               - f
-00015640: 756e 6374 696f 6e3a 2073 6e73 2e6c 696e  unction: sns.lin
-00015650: 6570 6c6f 740a 2020 2020 2020 2020 2020  eplot.          
-00015660: 2020 2020 2020 2020 6461 7461 3a20 2164          data: !d
-00015670: 6167 5f72 6573 756c 7420 6d79 5f63 7573  ag_result my_cus
-00015680: 746f 6d5f 6461 7461 0a0a 2020 2020 2020  tom_data..      
-00015690: 2020 2020 2020 2020 2020 2320 496d 706f            # Impo
-000156a0: 7274 2066 756e 6374 696f 6e20 7669 6120  rt function via 
-000156b0: 6028 6d6f 6475 6c65 2c20 6e61 6d65 2960  `(module, name)`
-000156c0: 2073 7065 6369 6669 6361 7469 6f6e 0a20   specification. 
-000156d0: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-000156e0: 2066 756e 6374 696f 6e3a 205b 6d61 7470   function: [matp
-000156f0: 6c6f 746c 6962 2c20 7079 706c 6f74 2e73  lotlib, pyplot.s
-00015700: 7562 706c 6f74 735f 6164 6a75 7374 5d0a  ubplots_adjust].
-00015710: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015720: 2020 6c65 6674 3a20 302e 310a 2020 2020    left: 0.1.    
-00015730: 2020 2020 2020 2020 2020 2020 2020 7269                ri
-00015740: 6768 743a 2030 2e39 0a0a 2020 2020 2020  ght: 0.9..      
-00015750: 2020 2020 2020 2020 2020 2320 5061 7373            # Pass
-00015760: 2061 2063 7573 746f 6d20 6361 6c6c 6162   a custom callab
-00015770: 6c65 2c20 7365 6c65 6374 6564 2076 6961  le, selected via
-00015780: 2044 4147 2066 7261 6d65 776f 726b 0a20   DAG framework. 
-00015790: 2020 2020 2020 2020 2020 2020 2020 202d                 -
-000157a0: 2066 756e 6374 696f 6e3a 2021 6461 675f   function: !dag_
-000157b0: 7265 7375 6c74 206d 795f 6361 6c6c 6162  result my_callab
-000157c0: 6c65 0a20 2020 2020 2020 2020 2020 2020  le.             
-000157d0: 2020 2020 2061 7267 733a 205b 666f 6f2c       args: [foo,
-000157e0: 2062 6172 5d0a 2020 2020 2020 2020 2020   bar].          
-000157f0: 2020 2020 2020 2020 2320 2e2e 2e20 6b65          # ... ke
-00015800: 7977 6f72 6420 6172 6775 6d65 6e74 7320  yword arguments 
-00015810: 6865 7265 0a0a 2020 2020 2020 2020 2020  here..          
-00015820: 2020 2020 2020 2320 5061 7373 2063 7572        # Pass cur
-00015830: 7265 6e74 2061 7869 7320 6f62 6a65 6374  rent axis object
-00015840: 2061 7320 6b65 7977 6f72 6420 6172 6775   as keyword argu
-00015850: 6d65 6e74 0a20 2020 2020 2020 2020 2020  ment.           
-00015860: 2020 2020 202d 2066 756e 6374 696f 6e3a       - function:
-00015870: 2021 6461 675f 7265 7375 6c74 206d 795f   !dag_result my_
-00015880: 6361 6c6c 6162 6c65 5f6f 7065 7261 7469  callable_operati
-00015890: 6e67 5f6f 6e5f 6178 0a20 2020 2020 2020  ng_on_ax.       
-000158a0: 2020 2020 2020 2020 2020 2070 6173 735f             pass_
-000158b0: 6178 6973 5f6f 626a 6563 745f 6173 3a20  axis_object_as: 
-000158c0: 6178 0a0a 2020 2020 2020 2020 2020 2020  ax..            
-000158d0: 2020 2020 2320 5061 7373 2068 656c 7065      # Pass helpe
-000158e0: 7220 6f62 6a65 6374 2069 7473 656c 6620  r object itself 
-000158f0: 6173 206b 6579 776f 7264 2061 7267 756d  as keyword argum
-00015900: 656e 740a 2020 2020 2020 2020 2020 2020  ent.            
-00015910: 2020 2020 2d20 6675 6e63 7469 6f6e 3a20      - function: 
-00015920: 2164 6167 5f72 6573 756c 7420 6d79 5f63  !dag_result my_c
-00015930: 616c 6c61 626c 655f 6f70 6572 6174 696e  allable_operatin
-00015940: 675f 6f6e 5f68 656c 7065 720a 2020 2020  g_on_helper.    
-00015950: 2020 2020 2020 2020 2020 2020 2020 7061                pa
-00015960: 7373 5f68 656c 7065 723a 2074 7275 650a  ss_helper: true.
-00015970: 0a20 2020 2020 2020 2041 7267 733a 0a20  .        Args:. 
-00015980: 2020 2020 2020 2020 2020 2066 756e 6374             funct
-00015990: 696f 6e73 2028 5365 7175 656e 6365 5b64  ions (Sequence[d
-000159a0: 6963 745d 293a 2041 2073 6571 7565 6e63  ict]): A sequenc
-000159b0: 6520 6f66 2066 756e 6374 696f 6e20 6361  e of function ca
-000159c0: 6c6c 0a20 2020 2020 2020 2020 2020 2020  ll.             
-000159d0: 2020 2073 7065 6369 6669 6361 7469 6f6e     specification
-000159e0: 732e 2045 6163 6820 6469 6374 206e 6565  s. Each dict nee
-000159f0: 6473 2074 6f20 636f 6e74 6169 6e20 6174  ds to contain at
-00015a00: 206c 6561 7374 2074 6865 206b 6579 0a20   least the key. 
-00015a10: 2020 2020 2020 2020 2020 2020 2020 2060                 `
-00015a20: 6066 756e 6374 696f 6e60 6020 7768 6963  `function`` whic
-00015a30: 6820 6465 7465 726d 696e 6573 2077 6869  h determines whi
-00015a40: 6368 2066 756e 6374 696f 6e20 746f 2069  ch function to i
-00015a50: 6e76 6f6b 652e 2046 7572 7468 6572 0a20  nvoke. Further. 
-00015a60: 2020 2020 2020 2020 2020 2020 2020 2061                 a
-00015a70: 7267 756d 656e 7473 2061 7265 2070 6172  rguments are par
-00015a80: 7365 6420 696e 746f 2074 6865 2070 6f73  sed into the pos
-00015a90: 6974 696f 6e61 6c20 616e 6420 6b65 7977  itional and keyw
-00015aa0: 6f72 6420 6172 6775 6d65 6e74 730a 2020  ord arguments.  
-00015ab0: 2020 2020 2020 2020 2020 2020 2020 6f66                of
-00015ac0: 2074 6865 2074 6f2d 6265 2d69 6e76 6f6b   the to-be-invok
-00015ad0: 6564 2066 756e 6374 696f 6e2e 0a20 2020  ed function..   
-00015ae0: 2020 2020 2020 2020 2066 756e 6373 5f6c           funcs_l
-00015af0: 6f6f 6b75 705f 6469 6374 2028 4469 6374  ookup_dict (Dict
-00015b00: 5b73 7472 2c20 4361 6c6c 6162 6c65 5d2c  [str, Callable],
-00015b10: 206f 7074 696f 6e61 6c29 3a20 4966 2067   optional): If g
-00015b20: 6976 656e 2c20 7769 6c6c 0a20 2020 2020  iven, will.     
-00015b30: 2020 2020 2020 2020 2020 206c 6f6f 6b20             look 
-00015b40: 7570 2074 6865 2066 756e 6374 696f 6e20  up the function 
-00015b50: 6e61 6d65 7320 6672 6f6d 2074 6869 7320  names from this 
-00015b60: 6469 6374 2069 6e73 7465 6164 206f 6620  dict instead of 
-00015b70: 7468 650a 2020 2020 2020 2020 2020 2020  the.            
-00015b80: 2020 2020 6465 6661 756c 7420 6469 6374      default dict
-00015b90: 2e0a 2020 2020 2020 2020 2020 2020 2a2a  ..            **
-00015ba0: 7368 6172 6564 5f6b 7761 7267 733a 2050  shared_kwargs: P
-00015bb0: 6173 7365 6420 6f6e 2061 7320 6b65 7977  assed on as keyw
-00015bc0: 6f72 6420 6172 6775 6d65 6e74 7320 746f  ord arguments to
-00015bd0: 202a 616c 6c2a 2066 756e 6374 696f 6e0a   *all* function.
-00015be0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00015bf0: 6361 6c6c 7320 696e 2060 6066 756e 6374  calls in ``funct
-00015c00: 696f 6e73 6060 2e0a 2020 2020 2020 2020  ions``..        
-00015c10: 2222 220a 2020 2020 2020 2020 6672 6f6d  """.        from
-00015c20: 202e 6675 6e63 732e 5f6d 756c 7469 706c   .funcs._multipl
-00015c30: 6f74 2069 6d70 6f72 7420 7061 7273 655f  ot import parse_
-00015c40: 616e 645f 696e 766f 6b65 5f66 756e 6374  and_invoke_funct
-00015c50: 696f 6e0a 0a20 2020 2020 2020 2066 6f72  ion..        for
-00015c60: 2063 616c 6c5f 6e75 6d2c 2066 756e 635f   call_num, func_
-00015c70: 6b77 6172 6773 2069 6e20 656e 756d 6572  kwargs in enumer
-00015c80: 6174 6528 6675 6e63 7469 6f6e 7329 3a0a  ate(functions):.
-00015c90: 2020 2020 2020 2020 2020 2020 7061 7273              pars
-00015ca0: 655f 616e 645f 696e 766f 6b65 5f66 756e  e_and_invoke_fun
-00015cb0: 6374 696f 6e28 0a20 2020 2020 2020 2020  ction(.         
-00015cc0: 2020 2020 2020 2068 6c70 723d 7365 6c66         hlpr=self
-00015cd0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00015ce0: 2020 6675 6e63 733d 6675 6e63 735f 6c6f    funcs=funcs_lo
-00015cf0: 6f6b 7570 5f64 6963 742c 0a20 2020 2020  okup_dict,.     
-00015d00: 2020 2020 2020 2020 2020 2073 6861 7265             share
-00015d10: 645f 6b77 6172 6773 3d73 6861 7265 645f  d_kwargs=shared_
-00015d20: 6b77 6172 6773 2c0a 2020 2020 2020 2020  kwargs,.        
-00015d30: 2020 2020 2020 2020 6675 6e63 5f6b 7761          func_kwa
-00015d40: 7267 733d 6675 6e63 5f6b 7761 7267 732c  rgs=func_kwargs,
-00015d50: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00015d60: 2073 686f 775f 6869 6e74 733d 4661 6c73   show_hints=Fals
-00015d70: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
-00015d80: 2020 2063 616c 6c5f 6e75 6d3d 6361 6c6c     call_num=call
-00015d90: 5f6e 756d 2c0a 2020 2020 2020 2020 2020  _num,.          
-00015da0: 2020 290a 0a20 2020 2023 202e 2e2e 2e2e    )..    # .....
+0000f7f0: 226e 756d 6572 6963 616c 2076 616c 7565  "numerical value
+0000f800: 2073 7065 6369 6679 696e 6720 7468 6520   specifying the 
+0000f810: 6c6f 7765 7220 6f72 2075 7070 6572 206c  lower or upper l
+0000f820: 696d 6974 2e22 0a20 2020 2020 2020 2020  imit.".         
+0000f830: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+0000f840: 2020 2020 2020 2020 2020 2020 2020 2320                # 
+0000f850: 4368 6563 6b20 7468 6174 2069 7420 6973  Check that it is
+0000f860: 2066 696e 6974 650a 2020 2020 2020 2020   finite.        
+0000f870: 2020 2020 2020 2020 6966 206e 6f74 206e          if not n
+0000f880: 702e 6973 6669 6e69 7465 2861 7267 293a  p.isfinite(arg):
+0000f890: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f8a0: 2020 2020 2072 6169 7365 2050 6c6f 7443       raise PlotC
+0000f8b0: 6f6e 6669 6745 7272 6f72 280a 2020 2020  onfigError(.    
+0000f8c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f8d0: 2020 2020 2243 6f75 6c64 206e 6f74 2067      "Could not g
+0000f8e0: 6574 2061 2066 696e 6974 6520 7661 6c75  et a finite valu
+0000f8f0: 6520 6672 6f6d 2074 6865 2061 7869 7320  e from the axis 
+0000f900: 6461 7461 2074 6f20 220a 2020 2020 2020  data to ".      
+0000f910: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000f920: 2020 2275 7365 2066 6f72 2073 6574 7469    "use for setti
+0000f930: 6e67 2061 7869 7320 6c69 6d69 7473 2074  ng axis limits t
+0000f940: 6f20 276d 696e 2720 6f72 2027 6d61 7827  o 'min' or 'max'
+0000f950: 2c20 220a 2020 2020 2020 2020 2020 2020  , ".            
+0000f960: 2020 2020 2020 2020 2020 2020 2270 7265              "pre
+0000f970: 7375 6d61 626c 7920 6265 6361 7573 6520  sumably because 
+0000f980: 7468 6520 6178 6973 2069 7320 7374 696c  the axis is stil
+0000f990: 6c20 656d 7074 792e 220a 2020 2020 2020  l empty.".      
+0000f9a0: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+0000f9b0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+0000f9c0: 2072 6574 7572 6e20 6172 670a 0a20 2020   return arg..   
+0000f9d0: 2020 2020 2020 2020 2023 2053 7065 6369           # Speci
+0000f9e0: 616c 2063 6173 653a 2064 6963 740a 2020  al case: dict.  
+0000f9f0: 2020 2020 2020 2020 2020 6966 2069 7369            if isi
+0000fa00: 6e73 7461 6e63 6528 6172 6773 2c20 6469  nstance(args, di
+0000fa10: 6374 293a 0a20 2020 2020 2020 2020 2020  ct):.           
+0000fa20: 2020 2020 2023 204d 616b 6520 7375 7265       # Make sure
+0000fa30: 2074 6865 7265 2061 7265 206f 6e6c 7920   there are only 
+0000fa40: 616c 6c6f 7765 6420 6b65 7973 0a20 2020  allowed keys.   
+0000fa50: 2020 2020 2020 2020 2020 2020 2069 6620               if 
+0000fa60: 5b6b 2066 6f72 206b 2069 6e20 6172 6773  [k for k in args
+0000fa70: 2e6b 6579 7328 2920 6966 206b 206e 6f74  .keys() if k not
+0000fa80: 2069 6e20 2822 6c6f 7765 7222 2c20 2275   in ("lower", "u
+0000fa90: 7070 6572 2229 5d3a 0a20 2020 2020 2020  pper")]:.       
+0000faa0: 2020 2020 2020 2020 2020 2020 2072 6169               rai
+0000fab0: 7365 2050 6c6f 7443 6f6e 6669 6745 7272  se PlotConfigErr
+0000fac0: 6f72 280a 2020 2020 2020 2020 2020 2020  or(.            
+0000fad0: 2020 2020 2020 2020 2020 2020 2254 6865              "The
+0000fae0: 7265 2061 7265 2069 6e76 616c 6964 206b  re are invalid k
+0000faf0: 6579 7320 7072 6573 656e 7420 696e 2061  eys present in a
+0000fb00: 2064 6963 742d 7479 7065 2022 0a20 2020   dict-type ".   
+0000fb10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb20: 2020 2020 2022 6172 6775 6d65 6e74 2074       "argument t
+0000fb30: 6f20 7365 745f 6c69 6d69 7473 2120 4f6e  o set_limits! On
+0000fb40: 6c79 2061 6363 6570 7469 6e67 206b 6579  ly accepting key
+0000fb50: 7320 276c 6f77 6572 2720 220a 2020 2020  s 'lower' ".    
+0000fb60: 2020 2020 2020 2020 2020 2020 2020 2020                  
+0000fb70: 2020 2020 6622 616e 6420 2775 7070 6572      f"and 'upper
+0000fb80: 272c 2062 7574 2067 6f74 3a20 7b61 7267  ', but got: {arg
+0000fb90: 737d 220a 2020 2020 2020 2020 2020 2020  s}".            
+0000fba0: 2020 2020 2020 2020 290a 0a20 2020 2020          )..     
+0000fbb0: 2020 2020 2020 2020 2020 206c 6f77 6572             lower
+0000fbc0: 203d 2061 7267 732e 6765 7428 226c 6f77   = args.get("low
+0000fbd0: 6572 222c 204e 6f6e 6529 0a20 2020 2020  er", None).     
+0000fbe0: 2020 2020 2020 2020 2020 2075 7070 6572             upper
+0000fbf0: 203d 2061 7267 732e 6765 7428 2275 7070   = args.get("upp
+0000fc00: 6572 222c 204e 6f6e 6529 0a0a 2020 2020  er", None)..    
+0000fc10: 2020 2020 2020 2020 656c 7365 3a0a 2020          else:.  
+0000fc20: 2020 2020 2020 2020 2020 2020 2020 6c6f                lo
+0000fc30: 7765 722c 2075 7070 6572 203d 2061 7267  wer, upper = arg
+0000fc40: 7320 2023 202e 2e2e 2061 7373 756d 696e  s  # ... assumin
+0000fc50: 6720 7365 7175 656e 6365 206f 6620 6c65  g sequence of le
+0000fc60: 6e67 7468 2032 0a0a 2020 2020 2020 2020  ngth 2..        
+0000fc70: 2020 2020 2320 5061 7273 6520 696e 6469      # Parse indi
+0000fc80: 7669 6475 616c 6c79 2c20 7468 656e 2072  vidually, then r
+0000fc90: 6574 7572 6e0a 2020 2020 2020 2020 2020  eturn.          
+0000fca0: 2020 7265 7475 726e 2028 7061 7273 655f    return (parse_
+0000fcb0: 6172 6728 6c6f 7765 7229 2c20 7061 7273  arg(lower), pars
+0000fcc0: 655f 6172 6728 7570 7065 7229 290a 0a20  e_arg(upper)).. 
+0000fcd0: 2020 2020 2020 2023 204e 6f77 2073 6574         # Now set
+0000fce0: 2074 6865 206c 696d 6974 732c 2075 7369   the limits, usi
+0000fcf0: 6e67 2074 6865 2068 656c 7065 7220 6675  ng the helper fu
+0000fd00: 6e63 7469 6f6e 7320 6465 6669 6e65 6420  nctions defined 
+0000fd10: 6162 6f76 650a 2020 2020 2020 2020 6966  above.        if
+0000fd20: 2078 2069 7320 6e6f 7420 4e6f 6e65 3a0a   x is not None:.
+0000fd30: 2020 2020 2020 2020 2020 2020 7365 6c66              self
+0000fd40: 2e61 782e 7365 745f 786c 696d 282a 7061  .ax.set_xlim(*pa
+0000fd50: 7273 655f 6172 6773 2878 2c20 6178 3d73  rse_args(x, ax=s
+0000fd60: 656c 662e 6178 2e78 6178 6973 2929 0a0a  elf.ax.xaxis))..
+0000fd70: 2020 2020 2020 2020 6966 2079 2069 7320          if y is 
+0000fd80: 6e6f 7420 4e6f 6e65 3a0a 2020 2020 2020  not None:.      
+0000fd90: 2020 2020 2020 7365 6c66 2e61 782e 7365        self.ax.se
+0000fda0: 745f 796c 696d 282a 7061 7273 655f 6172  t_ylim(*parse_ar
+0000fdb0: 6773 2879 2c20 6178 3d73 656c 662e 6178  gs(y, ax=self.ax
+0000fdc0: 2e79 6178 6973 2929 0a0a 2020 2020 2020  .yaxis))..      
+0000fdd0: 2020 6966 2068 6173 6174 7472 2873 656c    if hasattr(sel
+0000fde0: 662e 6178 2c20 227a 6178 6973 2229 3a0a  f.ax, "zaxis"):.
+0000fdf0: 2020 2020 2020 2020 2020 2020 6966 207a              if z
+0000fe00: 2069 7320 6e6f 7420 4e6f 6e65 3a0a 2020   is not None:.  
+0000fe10: 2020 2020 2020 2020 2020 2020 2020 7365                se
+0000fe20: 6c66 2e61 782e 7365 745f 7a6c 696d 282a  lf.ax.set_zlim(*
+0000fe30: 7061 7273 655f 6172 6773 287a 2c20 6178  parse_args(z, ax
+0000fe40: 3d73 656c 662e 6178 2e7a 6178 6973 2929  =self.ax.zaxis))
+0000fe50: 0a0a 2020 2020 6465 6620 5f68 6c70 725f  ..    def _hlpr_
+0000fe60: 7365 745f 6d61 7267 696e 7328 0a20 2020  set_margins(.   
+0000fe70: 2020 2020 2073 656c 662c 0a20 2020 2020       self,.     
+0000fe80: 2020 202a 2c0a 2020 2020 2020 2020 6d61     *,.        ma
+0000fe90: 7267 696e 733a 2055 6e69 6f6e 5b66 6c6f  rgins: Union[flo
+0000fea0: 6174 2c20 5475 706c 655b 666c 6f61 742c  at, Tuple[float,
+0000feb0: 2066 6c6f 6174 5d5d 203d 204e 6f6e 652c   float]] = None,
+0000fec0: 0a20 2020 2020 2020 2078 3a20 666c 6f61  .        x: floa
+0000fed0: 7420 3d20 4e6f 6e65 2c0a 2020 2020 2020  t = None,.      
+0000fee0: 2020 793a 2066 6c6f 6174 203d 204e 6f6e    y: float = Non
+0000fef0: 652c 0a20 2020 2020 2020 2074 6967 6874  e,.        tight
+0000ff00: 3a20 626f 6f6c 203d 2054 7275 652c 0a20  : bool = True,. 
+0000ff10: 2020 2029 3a0a 2020 2020 2020 2020 2222     ):.        ""
+0000ff20: 2253 6574 7320 7468 6520 6178 6573 2720  "Sets the axes' 
+0000ff30: 6d61 7267 696e 7320 7669 6120 3a70 793a  margins via :py:
+0000ff40: 6d65 7468 3a60 6d61 7470 6c6f 746c 6962  meth:`matplotlib
+0000ff50: 2e61 7865 732e 4178 6573 2e6d 6172 6769  .axes.Axes.margi
+0000ff60: 6e73 602e 0a0a 2020 2020 2020 2020 5468  ns`...        Th
+0000ff70: 6520 7061 6464 696e 6720 6164 6465 6420  e padding added 
+0000ff80: 746f 2065 6163 6820 6c69 6d69 7420 6f66  to each limit of
+0000ff90: 2074 6865 2041 7865 7320 6973 2074 6865   the Axes is the
+0000ffa0: 206d 6172 6769 6e20 7469 6d65 7320 7468   margin times th
+0000ffb0: 650a 2020 2020 2020 2020 6461 7461 2069  e.        data i
+0000ffc0: 6e74 6572 7661 6c2e 0a20 2020 2020 2020  nterval..       
+0000ffd0: 2041 6c6c 2069 6e70 7574 2070 6172 616d   All input param
+0000ffe0: 6574 6572 7320 6d75 7374 2062 6520 666c  eters must be fl
+0000fff0: 6f61 7473 2077 6974 6869 6e20 7468 6520  oats within the 
+00010000: 7261 6e67 6520 5b30 2c20 315d 2e0a 0a20  range [0, 1]... 
+00010010: 2020 2020 2020 2053 7065 6369 6679 696e         Specifyin
+00010020: 6720 616e 7920 6d61 7267 696e 2063 6861  g any margin cha
+00010030: 6e67 6573 206f 6e6c 7920 7468 6520 6175  nges only the au
+00010040: 746f 7363 616c 696e 673b 2066 6f72 2065  toscaling; for e
+00010050: 7861 6d70 6c65 2c20 6966 0a20 2020 2020  xample, if.     
+00010060: 2020 2060 6078 6d61 7267 696e 6060 2069     ``xmargin`` i
+00010070: 7320 6e6f 7420 4e6f 6e65 2c20 7468 656e  s not None, then
+00010080: 2060 6078 6d61 7267 696e 6060 2074 696d   ``xmargin`` tim
+00010090: 6573 2074 6865 2058 2064 6174 6120 696e  es the X data in
+000100a0: 7465 7276 616c 0a20 2020 2020 2020 2077  terval.        w
+000100b0: 696c 6c20 6265 2061 6464 6564 2074 6f20  ill be added to 
+000100c0: 6561 6368 2065 6e64 206f 6620 7468 6174  each end of that
+000100d0: 2069 6e74 6572 7661 6c20 6265 666f 7265   interval before
+000100e0: 2069 7420 6973 2075 7365 6420 696e 0a20   it is used in. 
+000100f0: 2020 2020 2020 2061 7574 6f73 6361 6c69         autoscali
+00010100: 6e67 2e0a 0a20 2020 2020 2020 2041 7267  ng...        Arg
+00010110: 733a 0a20 2020 2020 2020 2020 2020 206d  s:.            m
+00010120: 6172 6769 6e73 2028 556e 696f 6e5b 666c  argins (Union[fl
+00010130: 6f61 742c 2054 7570 6c65 5b66 6c6f 6174  oat, Tuple[float
+00010140: 2c20 666c 6f61 745d 5d2c 206f 7074 696f  , float]], optio
+00010150: 6e61 6c29 3a20 4966 2061 2073 6361 6c61  nal): If a scala
+00010160: 720a 2020 2020 2020 2020 2020 2020 2020  r.              
+00010170: 2020 6172 6775 6d65 6e74 2069 7320 7072    argument is pr
+00010180: 6f76 6964 6564 2c20 6974 2073 7065 6369  ovided, it speci
+00010190: 6669 6573 2062 6f74 6820 6d61 7267 696e  fies both margin
+000101a0: 7320 6f66 2074 6865 2078 2d61 7869 730a  s of the x-axis.
+000101b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000101c0: 616e 6420 792d 6178 6973 206c 696d 6974  and y-axis limit
+000101d0: 732e 2049 6620 6120 6c69 7374 2d20 6f72  s. If a list- or
+000101e0: 2074 7570 6c65 2d6c 696b 6520 706f 7369   tuple-like posi
+000101f0: 7469 6f6e 616c 0a20 2020 2020 2020 2020  tional.         
+00010200: 2020 2020 2020 2061 7267 756d 656e 7420         argument 
+00010210: 6973 2070 726f 7669 6465 642c 2074 6865  is provided, the
+00010220: 7920 7769 6c6c 2062 6520 696e 7465 7270  y will be interp
+00010230: 7265 7465 6420 6173 2060 6078 6d61 7267  reted as ``xmarg
+00010240: 696e 6060 2c0a 2020 2020 2020 2020 2020  in``,.          
+00010250: 2020 2020 2020 616e 6420 6060 796d 6172        and ``ymar
+00010260: 6769 6e60 602e 2049 6620 7365 7474 696e  gin``. If settin
+00010270: 6720 7468 6520 6d61 7267 696e 206f 6e20  g the margin on 
+00010280: 6120 7369 6e67 6c65 2061 7869 7320 6973  a single axis is
+00010290: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000102a0: 2064 6573 6972 6564 2c20 7573 6520 7468   desired, use th
+000102b0: 6520 6b65 7977 6f72 6420 6172 6775 6d65  e keyword argume
+000102c0: 6e74 7320 6465 7363 7269 6265 6420 6265  nts described be
+000102d0: 6c6f 772e 0a20 2020 2020 2020 2020 2020  low..           
+000102e0: 2078 2c20 7920 2866 6c6f 6174 2c20 6f70   x, y (float, op
+000102f0: 7469 6f6e 616c 293a 2053 7065 6369 6669  tional): Specifi
+00010300: 6320 6d61 7267 696e 2076 616c 7565 7320  c margin values 
+00010310: 666f 7220 7468 6520 782d 6178 6973 2061  for the x-axis a
+00010320: 6e64 0a20 2020 2020 2020 2020 2020 2020  nd.             
+00010330: 2020 2079 2d61 7869 732c 2072 6573 7065     y-axis, respe
+00010340: 6374 6976 656c 792e 2054 6865 7365 2063  ctively. These c
+00010350: 616e 6e6f 7420 6265 2075 7365 6420 696e  annot be used in
+00010360: 2063 6f6d 6269 6e61 7469 6f6e 2077 6974   combination wit
+00010370: 680a 2020 2020 2020 2020 2020 2020 2020  h.              
+00010380: 2020 7468 6520 6060 6d61 7267 696e 7360    the ``margins`
+00010390: 6020 6172 6775 6d65 6e74 2c20 6275 7420  ` argument, but 
+000103a0: 6361 6e20 6265 2075 7365 6420 696e 6469  can be used indi
+000103b0: 7669 6475 616c 6c79 2074 6f0a 2020 2020  vidually to.    
+000103c0: 2020 2020 2020 2020 2020 2020 616c 7465              alte
+000103d0: 7220 6f6e 2065 2e67 2e2c 206f 6e6c 7920  r on e.g., only 
+000103e0: 7468 6520 792d 6178 6973 2e0a 2020 2020  the y-axis..    
+000103f0: 2020 2020 2020 2020 7469 6768 7420 2862          tight (b
+00010400: 6f6f 6c2c 206f 7074 696f 6e61 6c29 3a20  ool, optional): 
+00010410: 5468 6520 7469 6768 7420 7061 7261 6d65  The tight parame
+00010420: 7465 7220 6973 2070 6173 7365 6420 746f  ter is passed to
+00010430: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010440: 203a 7079 3a6d 6574 683a 606d 6174 706c   :py:meth:`matpl
+00010450: 6f74 6c69 622e 6178 6573 2e41 7865 732e  otlib.axes.Axes.
+00010460: 6175 746f 7363 616c 655f 7669 6577 602c  autoscale_view`,
+00010470: 2077 6869 6368 2069 730a 2020 2020 2020   which is.      
+00010480: 2020 2020 2020 2020 2020 6578 6563 7574            execut
+00010490: 6564 2061 6674 6572 2061 206d 6172 6769  ed after a margi
+000104a0: 6e20 6973 2063 6861 6e67 6564 3b20 7468  n is changed; th
+000104b0: 6520 6465 6661 756c 7420 6865 7265 2069  e default here i
+000104c0: 7320 5472 7565 2c0a 2020 2020 2020 2020  s True,.        
+000104d0: 2020 2020 2020 2020 6f6e 2074 6865 2061          on the a
+000104e0: 7373 756d 7074 696f 6e20 7468 6174 2077  ssumption that w
+000104f0: 6865 6e20 6d61 7267 696e 7320 6172 6520  hen margins are 
+00010500: 7370 6563 6966 6965 642c 206e 6f0a 2020  specified, no.  
+00010510: 2020 2020 2020 2020 2020 2020 2020 6164                ad
+00010520: 6469 7469 6f6e 616c 2070 6164 6469 6e67  ditional padding
+00010530: 2074 6f20 6d61 7463 6820 7469 636b 206d   to match tick m
+00010540: 6172 6b73 2069 7320 7573 7561 6c6c 7920  arks is usually 
+00010550: 6465 7369 7265 642e 2053 6574 0a20 2020  desired. Set.   
+00010560: 2020 2020 2020 2020 2020 2020 2074 6967               tig
+00010570: 6874 2074 6f20 4e6f 6e65 2077 696c 6c20  ht to None will 
+00010580: 7072 6573 6572 7665 2074 6865 2070 7265  preserve the pre
+00010590: 7669 6f75 7320 7365 7474 696e 672e 0a20  vious setting.. 
+000105a0: 2020 2020 2020 2022 2222 0a20 2020 2020         """.     
+000105b0: 2020 206b 7761 7267 7320 3d20 6469 6374     kwargs = dict
+000105c0: 2878 3d78 2c20 793d 792c 2074 6967 6874  (x=x, y=y, tight
+000105d0: 3d74 6967 6874 290a 0a20 2020 2020 2020  =tight)..       
+000105e0: 2069 6620 6d61 7267 696e 7320 6973 206e   if margins is n
+000105f0: 6f74 204e 6f6e 653a 0a20 2020 2020 2020  ot None:.       
+00010600: 2020 2020 2069 6620 7820 6973 206e 6f74       if x is not
+00010610: 204e 6f6e 6520 6f72 2079 2069 7320 6e6f   None or y is no
+00010620: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00010630: 2020 2020 2020 2020 7261 6973 6520 5479          raise Ty
+00010640: 7065 4572 726f 7228 0a20 2020 2020 2020  peError(.       
+00010650: 2020 2020 2020 2020 2020 2020 2022 4361               "Ca
+00010660: 6e6e 6f74 2070 6173 7320 626f 7468 2060  nnot pass both `
+00010670: 6d61 7267 696e 7360 2061 6e64 2060 7860  margins` and `x`
+00010680: 2f60 7960 2061 7267 756d 656e 7473 2122  /`y` arguments!"
+00010690: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000106a0: 2029 0a0a 2020 2020 2020 2020 2020 2020   )..            
+000106b0: 6966 2069 7369 6e73 7461 6e63 6528 6d61  if isinstance(ma
+000106c0: 7267 696e 732c 2028 666c 6f61 742c 2069  rgins, (float, i
+000106d0: 6e74 2929 3a0a 2020 2020 2020 2020 2020  nt)):.          
+000106e0: 2020 2020 2020 7365 6c66 2e61 782e 6d61        self.ax.ma
+000106f0: 7267 696e 7328 6d61 7267 696e 732c 202a  rgins(margins, *
+00010700: 2a6b 7761 7267 7329 0a20 2020 2020 2020  *kwargs).       
+00010710: 2020 2020 2065 6c73 653a 0a20 2020 2020       else:.     
+00010720: 2020 2020 2020 2020 2020 2073 656c 662e             self.
+00010730: 6178 2e6d 6172 6769 6e73 282a 6d61 7267  ax.margins(*marg
+00010740: 696e 732c 202a 2a6b 7761 7267 7329 0a20  ins, **kwargs). 
+00010750: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
+00010760: 2020 2020 2020 2020 2073 656c 662e 6178           self.ax
+00010770: 2e6d 6172 6769 6e73 282a 2a6b 7761 7267  .margins(**kwarg
+00010780: 7329 0a0a 2020 2020 6465 6620 5f68 6c70  s)..    def _hlp
+00010790: 725f 7365 745f 6c65 6765 6e64 280a 2020  r_set_legend(.  
+000107a0: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+000107b0: 2020 2020 2a2c 0a20 2020 2020 2020 2075      *,.        u
+000107c0: 7365 5f6c 6567 656e 643a 2062 6f6f 6c20  se_legend: bool 
+000107d0: 3d20 5472 7565 2c0a 2020 2020 2020 2020  = True,.        
+000107e0: 6761 7468 6572 5f66 726f 6d5f 6669 673a  gather_from_fig:
+000107f0: 2062 6f6f 6c20 3d20 4661 6c73 652c 0a20   bool = False,. 
+00010800: 2020 2020 2020 2063 7573 746f 6d5f 6c61         custom_la
+00010810: 6265 6c73 3a20 5365 7175 656e 6365 5b73  bels: Sequence[s
+00010820: 7472 5d20 3d20 2829 2c0a 2020 2020 2020  tr] = (),.      
+00010830: 2020 6869 6469 6e67 5f74 6872 6573 686f    hiding_thresho
+00010840: 6c64 3a20 696e 7420 3d20 4e6f 6e65 2c0a  ld: int = None,.
+00010850: 2020 2020 2020 2020 2a2a 6c65 6765 6e64          **legend
+00010860: 5f6b 7761 7267 732c 0a20 2020 2029 3a0a  _kwargs,.    ):.
+00010870: 2020 2020 2020 2020 2222 2253 6574 7320          """Sets 
+00010880: 6120 6c65 6765 6e64 2066 6f72 2074 6865  a legend for the
+00010890: 2063 7572 7265 6e74 2061 7869 732e 0a0a   current axis...
+000108a0: 2020 2020 2020 2020 4173 2061 2066 6972          As a fir
+000108b0: 7374 2073 7465 702c 2074 6869 7320 6865  st step, this he
+000108c0: 6c70 6572 2074 7269 6573 2074 6f20 6578  lper tries to ex
+000108d0: 7472 6163 7420 616c 6c20 7265 6c65 7661  tract all releva
+000108e0: 6e74 206c 6567 656e 640a 2020 2020 2020  nt legend.      
+000108f0: 2020 6861 6e64 6c65 7320 616e 6420 6c61    handles and la
+00010900: 6265 6c73 2e20 4966 2061 206c 6567 656e  bels. If a legen
+00010910: 6420 7761 7320 7365 7420 7072 6576 696f  d was set previo
+00010920: 7573 6c79 2061 6e64 202a 6e6f 2a20 6861  usly and *no* ha
+00010930: 6e64 6c65 7320 616e 640a 2020 2020 2020  ndles and.      
+00010940: 2020 6c61 6265 6c73 2063 6f75 6c64 2062    labels could b
+00010950: 6520 6578 7472 6163 7465 6420 696e 2074  e extracted in t
+00010960: 6865 2074 7970 6963 616c 2077 6179 2028  he typical way (
+00010970: 692e 652e 2c20 7573 696e 6720 7468 650a  i.e., using the.
+00010980: 2020 2020 2020 2020 6060 6178 2e67 6574          ``ax.get
+00010990: 5f6c 6567 656e 645f 6861 6e64 6c65 735f  _legend_handles_
+000109a0: 6c61 6265 6c73 6060 206d 6574 686f 6429  labels`` method)
+000109b0: 2069 7420 7769 6c6c 2062 6520 6174 7465   it will be atte
+000109c0: 6d70 7465 6420 746f 0a20 2020 2020 2020  mpted to.       
+000109d0: 2072 6574 7269 6576 6520 7468 656d 2066   retrieve them f
+000109e0: 726f 6d20 6578 6973 7469 6e67 203a 7079  rom existing :py
+000109f0: 3a63 6c61 7373 3a60 6d61 7470 6c6f 746c  :class:`matplotl
+00010a00: 6962 2e6c 6567 656e 642e 4c65 6765 6e64  ib.legend.Legend
+00010a10: 600a 2020 2020 2020 2020 6f62 6a65 6374  `.        object
+00010a20: 7320 6f6e 2074 6865 2063 7572 7265 6e74  s on the current
+00010a30: 2061 7869 732e 0a20 2020 2020 2020 2049   axis..        I
+00010a40: 6620 6060 6761 7468 6572 5f66 726f 6d5f  f ``gather_from_
+00010a50: 6669 6760 6020 6973 2067 6976 656e 2c20  fig`` is given, 
+00010a60: 7468 6520 2a77 686f 6c65 2a20 6669 6775  the *whole* figu
+00010a70: 7265 2077 696c 6c20 6265 2069 6e73 7065  re will be inspe
+00010a80: 6374 6564 2c0a 2020 2020 2020 2020 7265  cted,.        re
+00010a90: 6761 7264 6c65 7373 206f 6620 7768 6574  gardless of whet
+00010aa0: 6865 7220 6861 6e64 6c65 7320 7765 7265  her handles were
+00010ab0: 2066 6f75 6e64 2070 7265 7669 6f75 736c   found previousl
+00010ac0: 792e 0a0a 2020 2020 2020 2020 4164 6469  y...        Addi
+00010ad0: 7469 6f6e 616c 6c79 2c20 616c 6c20 6178  tionally, all ax
+00010ae0: 6973 2d73 7065 6369 6669 6320 6861 6e64  is-specific hand
+00010af0: 6c65 7320 616e 6420 6c61 6265 6c73 2074  les and labels t
+00010b00: 7261 636b 6564 2076 6961 0a20 2020 2020  racked via.     
+00010b10: 2020 203a 7079 3a6d 6574 683a 602e 7472     :py:meth:`.tr
+00010b20: 6163 6b5f 6861 6e64 6c65 735f 6c61 6265  ack_handles_labe
+00010b30: 6c73 6020 7769 6c6c 2061 6c77 6179 7320  ls` will always 
+00010b40: 6265 2061 6464 6564 2e0a 0a20 2020 2020  be added...     
+00010b50: 2020 202e 2e20 6e6f 7465 3a3a 0a0a 2020     .. note::..  
+00010b60: 2020 2020 2020 2020 2020 2d20 4966 206e            - If n
+00010b70: 6f20 6861 6e64 6c65 7320 6361 6e20 6265  o handles can be
+00010b80: 2066 6f75 6e64 2c20 7468 6520 6c65 6765   found, the lege
+00010b90: 6e64 2069 7320 6869 6464 656e 2c20 616c  nd is hidden, al
+00010ba0: 736f 206d 6561 6e69 6e67 0a20 2020 2020  so meaning.     
+00010bb0: 2020 2020 2020 2020 2074 6861 7420 7468           that th
+00010bc0: 6520 6060 6c65 6765 6e64 5f6b 7761 7267  e ``legend_kwarg
+00010bd0: 7360 6020 7769 6c6c 206e 6f74 2062 6520  s`` will not be 
+00010be0: 7061 7373 6564 206f 6e2e 0a20 2020 2020  passed on..     
+00010bf0: 2020 2020 2020 202d 2044 7572 696e 6720         - During 
+00010c00: 6761 7468 6572 696e 6720 6f66 2068 616e  gathering of han
+00010c10: 646c 6573 2061 6e64 206c 6162 656c 7320  dles and labels 
+00010c20: 6672 6f6d 2074 6865 2063 7572 7265 6e74  from the current
+00010c30: 2061 7869 7320 6f72 0a20 2020 2020 2020   axis or.       
+00010c40: 2020 2020 2020 2074 6865 2066 6967 7572         the figur
+00010c50: 652c 2064 7570 6c69 6361 7465 7320 7769  e, duplicates wi
+00010c60: 6c6c 2062 6520 7265 6d6f 7665 643b 2064  ll be removed; d
+00010c70: 7570 6c69 6361 7465 7320 6172 6520 6465  uplicates are de
+00010c80: 7465 6374 6564 0a20 2020 2020 2020 2020  tected.         
+00010c90: 2020 2020 2076 6961 2074 6865 6972 206c       via their l
+00010ca0: 6162 656c 2073 7472 696e 6773 2c20 2a6e  abel strings, *n
+00010cb0: 6f74 2a20 7669 6120 7468 6569 7220 6861  ot* via their ha
+00010cc0: 6e64 6c65 2e0a 0a20 2020 2020 2020 202e  ndle...        .
+00010cd0: 2e20 6869 6e74 3a3a 0a0a 2020 2020 2020  . hint::..      
+00010ce0: 2020 2020 2020 546f 2073 6574 2061 2066        To set a f
+00010cf0: 6967 7572 652d 6c65 7665 6c20 6c65 6765  igure-level lege
+00010d00: 6e64 2c20 7573 6520 7468 6520 6060 7365  nd, use the ``se
+00010d10: 745f 6669 676c 6567 656e 6460 6020 6865  t_figlegend`` he
+00010d20: 6c70 6572 2e0a 0a20 2020 2020 2020 2041  lper...        A
+00010d30: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00010d40: 2075 7365 5f6c 6567 656e 6420 2862 6f6f   use_legend (boo
+00010d50: 6c2c 206f 7074 696f 6e61 6c29 3a20 5768  l, optional): Wh
+00010d60: 6574 6865 7220 746f 2073 6574 2061 206c  ether to set a l
+00010d70: 6567 656e 6420 6f72 206e 6f74 2e20 4966  egend or not. If
+00010d80: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00010d90: 2046 616c 7365 2c20 7468 6520 6c65 6765   False, the lege
+00010da0: 6e64 2077 696c 6c20 6265 2072 656d 6f76  nd will be remov
+00010db0: 6564 2e0a 2020 2020 2020 2020 2020 2020  ed..            
+00010dc0: 6761 7468 6572 5f66 726f 6d5f 6669 6720  gather_from_fig 
+00010dd0: 2862 6f6f 6c2c 206f 7074 696f 6e61 6c29  (bool, optional)
+00010de0: 3a20 4966 2073 6574 2c20 7769 6c6c 2067  : If set, will g
+00010df0: 6174 6865 7220 6c65 6765 6e64 0a20 2020  ather legend.   
+00010e00: 2020 2020 2020 2020 2020 2020 2068 616e               han
+00010e10: 646c 6573 2061 6e64 206c 6162 656c 7320  dles and labels 
+00010e20: 6672 6f6d 2074 6865 2077 686f 6c65 2066  from the whole f
+00010e30: 6967 7572 652e 2054 6869 7320 6361 6e20  igure. This can 
+00010e40: 6265 2075 7365 6675 6c20 746f 0a20 2020  be useful to.   
+00010e50: 2020 2020 2020 2020 2020 2020 2073 6574               set
+00010e60: 2069 6620 7468 6520 7265 6c65 7661 6e74   if the relevant
+00010e70: 2069 6e66 6f72 6d61 7469 6f6e 2069 7320   information is 
+00010e80: 666f 756e 6420 6f6e 2061 6e6f 7468 6572  found on another
+00010e90: 2061 7869 7320 6f72 2069 6e0a 2020 2020   axis or in.    
+00010ea0: 2020 2020 2020 2020 2020 2020 6120 6669              a fi
+00010eb0: 6775 7265 206c 6567 656e 642e 0a20 2020  gure legend..   
+00010ec0: 2020 2020 2020 2020 2063 7573 746f 6d5f           custom_
+00010ed0: 6c61 6265 6c73 2028 5365 7175 656e 6365  labels (Sequence
+00010ee0: 5b73 7472 5d2c 206f 7074 696f 6e61 6c29  [str], optional)
+00010ef0: 3a20 4966 2067 6976 656e 2c20 7573 6520  : If given, use 
+00010f00: 7468 6573 6520 6c61 6265 6c73 0a20 2020  these labels.   
+00010f10: 2020 2020 2020 2020 2020 2020 2061 6e64               and
+00010f20: 2061 7373 6f63 6961 7465 2074 6865 6d20   associate them 
+00010f30: 7769 7468 2065 7869 7374 696e 6720 6c61  with existing la
+00010f40: 6265 6c73 2e20 4e6f 7465 2074 6861 7420  bels. Note that 
+00010f50: 6966 2066 6577 6572 0a20 2020 2020 2020  if fewer.       
+00010f60: 2020 2020 2020 2020 206c 6162 656c 7320           labels 
+00010f70: 6172 6520 6769 7665 6e20 7468 616e 2068  are given than h
+00010f80: 616e 646c 6573 2061 7265 2061 7661 696c  andles are avail
+00010f90: 6162 6c65 2c20 7468 6f73 6520 7769 7468  able, those with
+00010fa0: 6f75 7420 610a 2020 2020 2020 2020 2020  out a.          
+00010fb0: 2020 2020 2020 6c61 6265 6c20 7769 6c6c        label will
+00010fc0: 206e 6f74 2062 6520 6472 6177 6e2e 0a20   not be drawn.. 
+00010fd0: 2020 2020 2020 2020 2020 2068 6964 696e             hidin
+00010fe0: 675f 7468 7265 7368 6f6c 6420 2869 6e74  g_threshold (int
+00010ff0: 2c20 6f70 7469 6f6e 616c 293a 2049 6620  , optional): If 
+00011000: 6769 7665 6e2c 2077 696c 6c20 6869 6465  given, will hide
+00011010: 206c 6567 656e 6473 0a20 2020 2020 2020   legends.       
+00011020: 2020 2020 2020 2020 2074 6861 7420 6861           that ha
+00011030: 7665 206d 6f72 6520 7468 616e 2074 6869  ve more than thi
+00011040: 7320 6e75 6d62 6572 206f 6620 6861 6e64  s number of hand
+00011050: 6c65 7320 7265 6769 7374 6572 6564 2e0a  les registered..
+00011060: 2020 2020 2020 2020 2020 2020 2a2a 6c65              **le
+00011070: 6765 6e64 5f6b 7761 7267 733a 2050 6173  gend_kwargs: Pas
+00011080: 7365 6420 6f6e 2074 6f20 6060 6178 2e6c  sed on to ``ax.l
+00011090: 6567 656e 6460 600a 2020 2020 2020 2020  egend``.        
+000110a0: 2222 220a 0a20 2020 2020 2020 2064 6566  """..        def
+000110b0: 2068 6964 655f 6c65 6765 6e64 2829 3a0a   hide_legend():.
+000110c0: 2020 2020 2020 2020 2020 2020 6c65 6765              lege
+000110d0: 6e64 203d 2073 656c 662e 6178 2e6c 6567  nd = self.ax.leg
+000110e0: 656e 6428 2829 2c20 6661 6e63 7962 6f78  end((), fancybox
+000110f0: 3d46 616c 7365 2c20 6672 616d 656f 6e3d  =False, frameon=
+00011100: 4661 6c73 6529 0a20 2020 2020 2020 2020  False).         
+00011110: 2020 206c 6567 656e 642e 7365 745f 7669     legend.set_vi
+00011120: 7369 626c 6528 4661 6c73 6529 0a0a 2020  sible(False)..  
+00011130: 2020 2020 2020 2320 5761 726e 2061 626f        # Warn abo
+00011140: 7574 2075 7361 6765 206f 6620 7468 6520  ut usage of the 
+00011150: 6f6c 6420 696e 7465 7266 6163 652e 0a20  old interface.. 
+00011160: 2020 2020 2020 2023 2054 4f44 4f20 5265         # TODO Re
+00011170: 6d6f 7665 2069 6e20 5665 7273 696f 6e20  move in Version 
+00011180: 312e 300a 2020 2020 2020 2020 6966 206c  1.0.        if l
+00011190: 6567 656e 645f 6b77 6172 6773 2e70 6f70  egend_kwargs.pop
+000111a0: 2822 7573 655f 6669 676c 6567 656e 6422  ("use_figlegend"
+000111b0: 2c20 4e6f 6e65 293a 0a20 2020 2020 2020  , None):.       
+000111c0: 2020 2020 206c 6f67 2e77 6172 6e69 6e67       log.warning
+000111d0: 280a 2020 2020 2020 2020 2020 2020 2020  (.              
+000111e0: 2020 2254 6865 2060 7573 655f 6669 676c    "The `use_figl
+000111f0: 6567 656e 6460 2061 7267 756d 656e 7420  egend` argument 
+00011200: 6973 206e 6f20 6c6f 6e67 6572 2073 7570  is no longer sup
+00011210: 706f 7274 6564 2022 0a20 2020 2020 2020  ported ".       
+00011220: 2020 2020 2020 2020 2022 666f 7220 7468           "for th
+00011230: 6520 6073 6574 5f6c 6567 656e 6460 2068  e `set_legend` h
+00011240: 656c 7065 722e 2055 7365 2060 7365 745f  elper. Use `set_
+00011250: 6669 676c 6567 656e 6460 2069 6e73 7465  figlegend` inste
+00011260: 6164 2e22 0a20 2020 2020 2020 2020 2020  ad.".           
+00011270: 2029 0a0a 2020 2020 2020 2020 2320 446f   )..        # Do
+00011280: 2065 7870 6c69 6369 7420 6869 6469 6e67   explicit hiding
+00011290: 2066 6972 7374 2c20 646f 6e27 7420 6e65   first, don't ne
+000112a0: 6564 2074 6f20 646f 2061 6c6c 2074 6865  ed to do all the
+000112b0: 2072 6573 7420 696e 2074 6869 7320 6361   rest in this ca
+000112c0: 7365 0a20 2020 2020 2020 2069 6620 6e6f  se.        if no
+000112d0: 7420 7573 655f 6c65 6765 6e64 3a0a 2020  t use_legend:.  
+000112e0: 2020 2020 2020 2020 2020 6c6f 672e 7265            log.re
+000112f0: 6d61 726b 2822 4869 6469 6e67 206c 6567  mark("Hiding leg
+00011300: 656e 6420 2e2e 2e22 290a 2020 2020 2020  end ...").      
+00011310: 2020 2020 2020 6869 6465 5f6c 6567 656e        hide_legen
+00011320: 6428 290a 2020 2020 2020 2020 2020 2020  d().            
+00011330: 7265 7475 726e 0a0a 2020 2020 2020 2020  return..        
+00011340: 2320 5472 7920 746f 2067 6574 2028 6461  # Try to get (da
+00011350: 6e67 6c69 6e67 2920 6861 6e64 6c65 7320  ngling) handles 
+00011360: 616e 6420 6c61 6265 6c73 2066 726f 6d20  and labels from 
+00011370: 7468 6520 6178 6973 0a20 2020 2020 2020  the axis.       
+00011380: 2068 2c20 6c20 3d20 7365 6c66 2e61 782e   h, l = self.ax.
+00011390: 6765 745f 6c65 6765 6e64 5f68 616e 646c  get_legend_handl
+000113a0: 6573 5f6c 6162 656c 7328 290a 2020 2020  es_labels().    
+000113b0: 2020 2020 2320 4e4f 5445 2057 696c 6c20      # NOTE Will 
+000113c0: 6265 2065 6d70 7479 2069 6620 6178 2e6c  be empty if ax.l
+000113d0: 6567 656e 6428 2920 7761 7320 6361 6c6c  egend() was call
+000113e0: 6564 2061 6c72 6561 6479 0a0a 2020 2020  ed already..    
+000113f0: 2020 2020 2320 4164 6420 7468 6f73 6520      # Add those 
+00011400: 7468 6174 2068 6176 6520 6265 656e 2074  that have been t
+00011410: 7261 636b 6564 2065 7870 6c69 6369 746c  racked explicitl
+00011420: 790a 2020 2020 2020 2020 5f68 2c20 5f6c  y.        _h, _l
+00011430: 203d 2073 656c 662e 6178 6973 5f68 616e   = self.axis_han
+00011440: 646c 6573 5f6c 6162 656c 730a 2020 2020  dles_labels.    
+00011450: 2020 2020 6820 2b3d 205f 680a 2020 2020      h += _h.    
+00011460: 2020 2020 6c20 2b3d 205f 6c0a 0a20 2020      l += _l..   
+00011470: 2020 2020 2023 2049 6620 7468 6572 6520       # If there 
+00011480: 7765 7265 206e 6f20 6861 6e64 6c65 7320  were no handles 
+00011490: 6176 6169 6c61 626c 6520 696e 2074 6869  available in thi
+000114a0: 7320 7761 792c 2074 7279 2074 6f20 6761  s way, try to ga
+000114b0: 7468 6572 2074 6865 0a20 2020 2020 2020  ther the.       
+000114c0: 2023 2069 6e66 6f72 6d61 7469 6f6e 2066   # information f
+000114d0: 726f 6d20 7468 6520 6375 7272 656e 7420  rom the current 
+000114e0: 6178 6973 206f 7220 7468 6520 7768 6f6c  axis or the whol
+000114f0: 6520 6669 6775 7265 0a20 2020 2020 2020  e figure.       
+00011500: 2069 6620 6e6f 7420 6820 6f72 2067 6174   if not h or gat
+00011510: 6865 725f 6672 6f6d 5f66 6967 3a0a 2020  her_from_fig:.  
+00011520: 2020 2020 2020 2020 2020 5f68 2c20 5f6c            _h, _l
+00011530: 203d 2067 6174 6865 725f 6861 6e64 6c65   = gather_handle
+00011540: 735f 6c61 6265 6c73 280a 2020 2020 2020  s_labels(.      
+00011550: 2020 2020 2020 2020 2020 7365 6c66 2e66            self.f
+00011560: 6967 2069 6620 6761 7468 6572 5f66 726f  ig if gather_fro
+00011570: 6d5f 6669 6720 656c 7365 2073 656c 662e  m_fig else self.
+00011580: 6178 0a20 2020 2020 2020 2020 2020 2029  ax.            )
+00011590: 0a20 2020 2020 2020 2020 2020 206c 6f67  .            log
+000115a0: 2e64 6562 7567 280a 2020 2020 2020 2020  .debug(.        
+000115b0: 2020 2020 2020 2020 2247 6174 6865 7265          "Gathere
+000115c0: 6420 2564 2068 616e 646c 6573 2061 6e64  d %d handles and
+000115d0: 206c 6162 656c 7320 6672 6f6d 2025 732e   labels from %s.
+000115e0: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
+000115f0: 2020 206c 656e 285f 6829 2c0a 2020 2020     len(_h),.    
+00011600: 2020 2020 2020 2020 2020 2020 2274 6865              "the
+00011610: 2077 686f 6c65 2066 6967 7572 6522 0a20   whole figure". 
+00011620: 2020 2020 2020 2020 2020 2020 2020 2069                 i
+00011630: 6620 286e 6f74 2068 2061 6e64 2067 6174  f (not h and gat
+00011640: 6865 725f 6672 6f6d 5f66 6967 290a 2020  her_from_fig).  
+00011650: 2020 2020 2020 2020 2020 2020 2020 656c                el
+00011660: 7365 2022 6375 7272 656e 7420 6178 6973  se "current axis
+00011670: 222c 0a20 2020 2020 2020 2020 2020 2029  ",.            )
+00011680: 0a0a 2020 2020 2020 2020 2020 2020 6820  ..            h 
+00011690: 2b3d 205f 680a 2020 2020 2020 2020 2020  += _h.          
+000116a0: 2020 6c20 2b3d 205f 6c0a 0a20 2020 2020    l += _l..     
+000116b0: 2020 2023 2052 656d 6f76 6520 706f 7465     # Remove pote
+000116c0: 6e74 6961 6c20 6475 706c 6963 6174 6520  ntial duplicate 
+000116d0: 6861 6e64 6c65 7320 2869 6465 6e74 6966  handles (identif
+000116e0: 6965 6420 6279 2074 6865 206c 6162 656c  ied by the label
+000116f0: 7329 0a20 2020 2020 2020 2068 2c20 6c20  s).        h, l 
+00011700: 3d20 7265 6d6f 7665 5f64 7570 6c69 6361  = remove_duplica
+00011710: 7465 5f68 616e 646c 6573 5f6c 6162 656c  te_handles_label
+00011720: 7328 682c 206c 290a 0a20 2020 2020 2020  s(h, l)..       
+00011730: 2023 202e 2e2e 2061 6e64 2065 7661 6c75   # ... and evalu
+00011740: 6174 6520 7468 6520 6375 7374 6f6d 206c  ate the custom l
+00011750: 6162 656c 7320 616e 6420 6869 6469 6e67  abels and hiding
+00011760: 2074 6872 6573 686f 6c64 0a20 2020 2020   threshold.     
+00011770: 2020 2068 2c20 6c2c 2070 6173 745f 7468     h, l, past_th
+00011780: 7265 7368 203d 2070 7265 7061 7265 5f6c  resh = prepare_l
+00011790: 6567 656e 645f 6172 6773 280a 2020 2020  egend_args(.    
+000117a0: 2020 2020 2020 2020 682c 0a20 2020 2020          h,.     
+000117b0: 2020 2020 2020 206c 2c0a 2020 2020 2020         l,.      
+000117c0: 2020 2020 2020 6375 7374 6f6d 5f6c 6162        custom_lab
+000117d0: 656c 733d 6375 7374 6f6d 5f6c 6162 656c  els=custom_label
+000117e0: 732c 0a20 2020 2020 2020 2020 2020 2068  s,.            h
+000117f0: 6964 696e 675f 7468 7265 7368 6f6c 643d  iding_threshold=
+00011800: 6869 6469 6e67 5f74 6872 6573 686f 6c64  hiding_threshold
+00011810: 2c0a 2020 2020 2020 2020 290a 0a20 2020  ,.        )..   
+00011820: 2020 2020 2023 2048 6964 6520 6f72 2064       # Hide or d
+00011830: 7261 7720 7468 6520 6c65 6765 6e64 0a20  raw the legend. 
+00011840: 2020 2020 2020 2069 6620 7061 7374 5f74         if past_t
+00011850: 6872 6573 6820 6f72 206e 6f74 2068 3a0a  hresh or not h:.
+00011860: 2020 2020 2020 2020 2020 2020 6869 6465              hide
+00011870: 5f6c 6567 656e 6428 290a 0a20 2020 2020  _legend()..     
+00011880: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+00011890: 2020 2020 2073 656c 662e 6178 2e6c 6567       self.ax.leg
+000118a0: 656e 6428 682c 206c 2c20 2a2a 6c65 6765  end(h, l, **lege
+000118b0: 6e64 5f6b 7761 7267 7329 0a0a 2020 2020  nd_kwargs)..    
+000118c0: 6465 6620 5f68 6c70 725f 7365 745f 7465  def _hlpr_set_te
+000118d0: 7874 7328 7365 6c66 2c20 2a2c 2074 6578  xts(self, *, tex
+000118e0: 7473 3a20 5365 7175 656e 6365 5b64 6963  ts: Sequence[dic
+000118f0: 745d 293a 0a20 2020 2020 2020 2022 2222  t]):.        """
+00011900: 5365 7473 206d 756c 7469 706c 6520 7465  Sets multiple te
+00011910: 7874 2065 6c65 6d65 6e74 7320 666f 7220  xt elements for 
+00011920: 7468 6520 6375 7272 656e 7420 6178 6973  the current axis
+00011930: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
+00011940: 6c65 2063 6f6e 6669 6775 7261 7469 6f6e  le configuration
+00011950: 3a0a 0a20 2020 2020 2020 202e 2e20 636f  :..        .. co
+00011960: 6465 2d62 6c6f 636b 3a3a 2079 616d 6c0a  de-block:: yaml.
+00011970: 0a20 2020 2020 2020 2020 2020 2073 6574  .            set
+00011980: 5f74 6578 7473 3a0a 2020 2020 2020 2020  _texts:.        
+00011990: 2020 2020 2020 7465 7874 733a 0a20 2020        texts:.   
+000119a0: 2020 2020 2020 2020 2020 2020 202d 2078               - x
+000119b0: 3a20 300a 2020 2020 2020 2020 2020 2020  : 0.            
+000119c0: 2020 2020 2020 793a 2031 0a20 2020 2020        y: 1.     
+000119d0: 2020 2020 2020 2020 2020 2020 2073 3a20               s: 
+000119e0: 736f 6d65 2074 6578 740a 2020 2020 2020  some text.      
+000119f0: 2020 2020 2020 2020 2020 2020 2320 2e2e              # ..
+00011a00: 2e20 6d6f 7265 2061 7267 756d 656e 7473  . more arguments
+00011a10: 2074 6f20 706c 742e 7465 7874 0a0a 2020   to plt.text..  
+00011a20: 2020 2020 2020 4172 6773 3a0a 2020 2020        Args:.    
+00011a30: 2020 2020 2020 2020 7465 7874 7320 2853          texts (S
+00011a40: 6571 7565 6e63 655b 6469 6374 5d29 3a20  equence[dict]): 
+00011a50: 4120 7365 7175 656e 6365 206f 6620 7465  A sequence of te
+00011a60: 7874 2073 7065 6369 6669 6361 7469 6f6e  xt specification
+00011a70: 732c 2074 6861 7420 6172 650a 2020 2020  s, that are.    
+00011a80: 2020 2020 2020 2020 2020 2020 7061 7373              pass
+00011a90: 6564 2074 6f20 3a70 793a 6675 6e63 3a60  ed to :py:func:`
+00011aa0: 6d61 7470 6c6f 746c 6962 2e70 7970 6c6f  matplotlib.pyplo
+00011ab0: 742e 7465 7874 600a 2020 2020 2020 2020  t.text`.        
+00011ac0: 2222 220a 2020 2020 2020 2020 666f 7220  """.        for 
+00011ad0: 6b77 6172 6773 2069 6e20 7465 7874 733a  kwargs in texts:
+00011ae0: 0a20 2020 2020 2020 2020 2020 2073 656c  .            sel
+00011af0: 662e 6178 2e74 6578 7428 2a2a 6b77 6172  f.ax.text(**kwar
+00011b00: 6773 290a 0a20 2020 2064 6566 205f 686c  gs)..    def _hl
+00011b10: 7072 5f61 6e6e 6f74 6174 6528 7365 6c66  pr_annotate(self
+00011b20: 2c20 2a2c 2061 6e6e 6f74 6174 696f 6e73  , *, annotations
+00011b30: 3a20 5365 7175 656e 6365 5b64 6963 745d  : Sequence[dict]
+00011b40: 293a 0a20 2020 2020 2020 2022 2222 5365  ):.        """Se
+00011b50: 7473 206d 756c 7469 706c 6520 616e 6e6f  ts multiple anno
+00011b60: 7461 7469 6f6e 7320 666f 7220 7468 6520  tations for the 
+00011b70: 6375 7272 656e 7420 6178 6973 2e0a 0a20  current axis... 
+00011b80: 2020 2020 2020 2045 7861 6d70 6c65 2063         Example c
+00011b90: 6f6e 6669 6775 7261 7469 6f6e 3a0a 0a20  onfiguration:.. 
+00011ba0: 2020 2020 2020 202e 2e20 636f 6465 2d62         .. code-b
+00011bb0: 6c6f 636b 3a3a 2079 616d 6c0a 0a20 2020  lock:: yaml..   
+00011bc0: 2020 2020 2020 2020 2061 6e6e 6f74 6174           annotat
+00011bd0: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00011be0: 2061 6e6e 6f74 6174 696f 6e73 3a0a 2020   annotations:.  
+00011bf0: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00011c00: 7879 3a20 5b31 2c20 332e 3134 3135 395d  xy: [1, 3.14159]
+00011c10: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00011c20: 2020 2074 6578 743a 2074 6869 7320 6973     text: this is
+00011c30: 20cf 800a 2020 2020 2020 2020 2020 2020   ...            
+00011c40: 2020 2020 2020 7879 636f 6f72 6473 3a20        xycoords: 
+00011c50: 6461 7461 0a20 2020 2020 2020 2020 2020  data.           
+00011c60: 2020 2020 2020 2023 202e 2e2e 206d 6f72         # ... mor
+00011c70: 6520 6172 6775 6d65 6e74 7320 746f 2070  e arguments to p
+00011c80: 6c74 2e61 6e6e 6f74 6174 650a 2020 2020  lt.annotate.    
+00011c90: 2020 2020 2020 2020 2020 2020 2d20 7879              - xy
+00011ca0: 3a20 5b30 2c20 305d 0a20 2020 2020 2020  : [0, 0].       
+00011cb0: 2020 2020 2020 2020 2020 2078 7963 6f6f             xycoo
+00011cc0: 7264 733a 2064 6174 610a 2020 2020 2020  rds: data.      
+00011cd0: 2020 2020 2020 2020 2020 2020 7465 7874              text
+00011ce0: 3a20 7468 6973 2069 7320 7a65 726f 0a20  : this is zero. 
+00011cf0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00011d00: 2078 7974 6578 743a 205b 302e 312c 2030   xytext: [0.1, 0
+00011d10: 2e31 5d0a 2020 2020 2020 2020 2020 2020  .1].            
+00011d20: 2020 2020 2020 6172 726f 7770 726f 7073        arrowprops
+00011d30: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00011d40: 2020 2020 2020 6661 6365 636f 6c6f 723a        facecolor:
+00011d50: 2062 6c61 636b 0a20 2020 2020 2020 2020   black.         
+00011d60: 2020 2020 2020 2020 2020 2073 6872 696e             shrin
+00011d70: 6b3a 2030 2e30 350a 0a20 2020 2020 2020  k: 0.05..       
+00011d80: 2041 7267 733a 0a20 2020 2020 2020 2020   Args:.         
+00011d90: 2020 2061 6e6e 6f74 6174 696f 6e73 2028     annotations (
+00011da0: 5365 7175 656e 6365 5b64 6963 745d 293a  Sequence[dict]):
+00011db0: 2041 2073 6571 7565 6e63 6520 6f66 2061   A sequence of a
+00011dc0: 6e6e 6f74 6174 696f 6e20 7061 7261 6d65  nnotation parame
+00011dd0: 7465 7273 0a20 2020 2020 2020 2020 2020  ters.           
+00011de0: 2020 2020 2077 6869 6368 2077 696c 6c20       which will 
+00011df0: 6265 2070 6173 7365 6420 746f 203a 7079  be passed to :py
+00011e00: 3a66 756e 633a 606d 6174 706c 6f74 6c69  :func:`matplotli
+00011e10: 622e 7079 706c 6f74 2e61 6e6e 6f74 6174  b.pyplot.annotat
+00011e20: 6560 0a20 2020 2020 2020 2022 2222 0a20  e`.        """. 
+00011e30: 2020 2020 2020 2066 6f72 206b 7761 7267         for kwarg
+00011e40: 7320 696e 2061 6e6e 6f74 6174 696f 6e73  s in annotations
+00011e50: 3a0a 2020 2020 2020 2020 2020 2020 7365  :.            se
+00011e60: 6c66 2e61 782e 616e 6e6f 7461 7465 282a  lf.ax.annotate(*
+00011e70: 2a6b 7761 7267 7329 0a0a 2020 2020 6465  *kwargs)..    de
+00011e80: 6620 5f68 6c70 725f 7365 745f 6876 5f6c  f _hlpr_set_hv_l
+00011e90: 696e 6573 2873 656c 662c 202a 2c20 686c  ines(self, *, hl
+00011ea0: 696e 6573 3a20 6c69 7374 203d 204e 6f6e  ines: list = Non
+00011eb0: 652c 2076 6c69 6e65 733a 206c 6973 7420  e, vlines: list 
+00011ec0: 3d20 4e6f 6e65 293a 0a20 2020 2020 2020  = None):.       
+00011ed0: 2022 2222 5365 7473 206f 6e65 206f 7220   """Sets one or 
+00011ee0: 6d75 6c74 6970 6c65 2068 6f72 697a 6f6e  multiple horizon
+00011ef0: 7461 6c20 6f72 2076 6572 7469 6361 6c20  tal or vertical 
+00011f00: 6c69 6e65 7320 7573 696e 670a 2020 2020  lines using.    
+00011f10: 2020 2020 3a70 793a 6d65 7468 3a60 6d61      :py:meth:`ma
+00011f20: 7470 6c6f 746c 6962 2e61 7865 732e 4178  tplotlib.axes.Ax
+00011f30: 6573 2e61 7868 6c69 6e65 6020 616e 6420  es.axhline` and 
+00011f40: 2f20 6f72 0a20 2020 2020 2020 203a 7079  / or.        :py
+00011f50: 3a6d 6574 683a 606d 6174 706c 6f74 6c69  :meth:`matplotli
+00011f60: 622e 6178 6573 2e41 7865 732e 6178 766c  b.axes.Axes.axvl
+00011f70: 696e 6560 2e0a 0a20 2020 2020 2020 2041  ine`...        A
+00011f80: 7267 733a 0a20 2020 2020 2020 2020 2020  rgs:.           
+00011f90: 2068 6c69 6e65 7320 286c 6973 742c 206f   hlines (list, o
+00011fa0: 7074 696f 6e61 6c29 3a20 6c69 7374 206f  ptional): list o
+00011fb0: 6620 6e75 6d65 7269 6320 706f 7369 7469  f numeric positi
+00011fc0: 6f6e 7320 6f66 2074 6865 206c 696e 6573  ons of the lines
+00011fd0: 206f 720a 2020 2020 2020 2020 2020 2020   or.            
+00011fe0: 2020 2020 6f72 206c 6973 7420 6f66 2064      or list of d
+00011ff0: 6963 7473 2077 6974 6820 6b65 7920 6060  icts with key ``
+00012000: 706f 7360 6020 6465 7465 726d 696e 696e  pos`` determinin
+00012010: 6720 7468 6520 706f 7369 7469 6f6e 2c20  g the position, 
+00012020: 6b65 790a 2020 2020 2020 2020 2020 2020  key.            
+00012030: 2020 2020 6060 6c69 6d69 7473 6060 2064      ``limits`` d
+00012040: 6574 6572 6d69 6e69 6e67 2074 6865 2072  etermining the r
+00012050: 656c 6174 6976 6520 6c69 6d69 7473 206f  elative limits o
+00012060: 6620 7468 6520 6c69 6e65 2c20 616e 6420  f the line, and 
+00012070: 616c 6c0a 2020 2020 2020 2020 2020 2020  all.            
+00012080: 2020 2020 6164 6469 7469 6f6e 616c 2061      additional a
+00012090: 7267 756d 656e 7473 2062 6569 6e67 2070  rguments being p
+000120a0: 6173 7365 6420 6f6e 2074 6f20 7468 6520  assed on to the 
+000120b0: 6d61 7470 6c6f 746c 6962 0a20 2020 2020  matplotlib.     
+000120c0: 2020 2020 2020 2020 2020 2066 756e 6374             funct
+000120d0: 696f 6e2e 0a20 2020 2020 2020 2020 2020  ion..           
+000120e0: 2076 6c69 6e65 7320 286c 6973 742c 206f   vlines (list, o
+000120f0: 7074 696f 6e61 6c29 3a20 6c69 7374 206f  ptional): list o
+00012100: 6620 6e75 6d65 7269 6320 706f 7369 7469  f numeric positi
+00012110: 6f6e 7320 6f66 2074 6865 206c 696e 6573  ons of the lines
+00012120: 206f 720a 2020 2020 2020 2020 2020 2020   or.            
+00012130: 2020 2020 6f72 206c 6973 7420 6f66 2064      or list of d
+00012140: 6963 7473 2077 6974 6820 6b65 7920 6060  icts with key ``
+00012150: 706f 7360 6020 6465 7465 726d 696e 696e  pos`` determinin
+00012160: 6720 7468 6520 706f 7369 7469 6f6e 2c20  g the position, 
+00012170: 6b65 790a 2020 2020 2020 2020 2020 2020  key.            
+00012180: 2020 2020 6060 6c69 6d69 7473 6060 2064      ``limits`` d
+00012190: 6574 6572 6d69 6e69 6e67 2074 6865 2072  etermining the r
+000121a0: 656c 6174 6976 6520 6c69 6d69 7473 206f  elative limits o
+000121b0: 6620 7468 6520 6c69 6e65 2c20 616e 6420  f the line, and 
+000121c0: 616c 6c0a 2020 2020 2020 2020 2020 2020  all.            
+000121d0: 2020 2020 6164 6469 7469 6f6e 616c 2061      additional a
+000121e0: 7267 756d 656e 7473 2062 6569 6e67 2070  rguments being p
+000121f0: 6173 7365 6420 6f6e 2074 6f20 7468 6520  assed on to the 
+00012200: 6d61 7470 6c6f 746c 6962 0a20 2020 2020  matplotlib.     
+00012210: 2020 2020 2020 2020 2020 2066 756e 6374             funct
+00012220: 696f 6e2e 0a20 2020 2020 2020 2022 2222  ion..        """
+00012230: 0a0a 2020 2020 2020 2020 6465 6620 7365  ..        def se
+00012240: 745f 6c69 6e65 280a 2020 2020 2020 2020  t_line(.        
+00012250: 2020 2020 6675 6e63 3a20 4361 6c6c 6162      func: Callab
+00012260: 6c65 2c0a 2020 2020 2020 2020 2020 2020  le,.            
+00012270: 2a2c 0a20 2020 2020 2020 2020 2020 2070  *,.            p
+00012280: 6f73 3a20 666c 6f61 742c 0a20 2020 2020  os: float,.     
+00012290: 2020 2020 2020 206c 696d 6974 733a 2074         limits: t
+000122a0: 7570 6c65 203d 2028 302e 302c 2031 2e30  uple = (0.0, 1.0
+000122b0: 292c 0a20 2020 2020 2020 2020 2020 202a  ),.            *
+000122c0: 2a6c 696e 655f 6b77 6172 6773 2c0a 2020  *line_kwargs,.  
+000122d0: 2020 2020 2020 293a 0a20 2020 2020 2020        ):.       
+000122e0: 2020 2020 2074 7279 3a0a 2020 2020 2020       try:.      
+000122f0: 2020 2020 2020 2020 2020 706f 7320 3d20            pos = 
+00012300: 666c 6f61 7428 706f 7329 0a0a 2020 2020  float(pos)..    
+00012310: 2020 2020 2020 2020 6578 6365 7074 2045          except E
+00012320: 7863 6570 7469 6f6e 2061 7320 6572 723a  xception as err:
+00012330: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00012340: 2072 6169 7365 2050 6c6f 7443 6f6e 6669   raise PlotConfi
+00012350: 6745 7272 6f72 280a 2020 2020 2020 2020  gError(.        
+00012360: 2020 2020 2020 2020 2020 2020 6622 476f              f"Go
+00012370: 7420 6e6f 6e2d 6e75 6d65 7269 6320 7661  t non-numeric va
+00012380: 6c75 6520 277b 706f 737d 2720 666f 7220  lue '{pos}' for 
+00012390: 6070 6f73 6020 6172 6775 6d65 6e74 2069  `pos` argument i
+000123a0: 6e20 220a 2020 2020 2020 2020 2020 2020  n ".            
+000123b0: 2020 2020 2020 2020 2273 6574 5f68 765f          "set_hv_
+000123c0: 6c69 6e65 7320 6865 6c70 6572 2122 0a20  lines helper!". 
+000123d0: 2020 2020 2020 2020 2020 2020 2020 2029                 )
+000123e0: 0a0a 2020 2020 2020 2020 2020 2020 6675  ..            fu
+000123f0: 6e63 2870 6f73 2c20 2a6c 696d 6974 732c  nc(pos, *limits,
+00012400: 202a 2a6c 696e 655f 6b77 6172 6773 290a   **line_kwargs).
+00012410: 0a20 2020 2020 2020 2069 6620 686c 696e  .        if hlin
+00012420: 6573 2069 7320 6e6f 7420 4e6f 6e65 3a0a  es is not None:.
+00012430: 2020 2020 2020 2020 2020 2020 666f 7220              for 
+00012440: 6c69 6e65 5f73 7065 6320 696e 2068 6c69  line_spec in hli
+00012450: 6e65 733a 0a20 2020 2020 2020 2020 2020  nes:.           
+00012460: 2020 2020 2069 6620 6973 696e 7374 616e       if isinstan
+00012470: 6365 286c 696e 655f 7370 6563 2c20 6469  ce(line_spec, di
+00012480: 6374 293a 0a20 2020 2020 2020 2020 2020  ct):.           
+00012490: 2020 2020 2020 2020 2073 6574 5f6c 696e           set_lin
+000124a0: 6528 7365 6c66 2e61 782e 6178 686c 696e  e(self.ax.axhlin
+000124b0: 652c 202a 2a6c 696e 655f 7370 6563 290a  e, **line_spec).
+000124c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000124d0: 656c 7365 3a0a 2020 2020 2020 2020 2020  else:.          
+000124e0: 2020 2020 2020 2020 2020 7365 745f 6c69            set_li
+000124f0: 6e65 2873 656c 662e 6178 2e61 7868 6c69  ne(self.ax.axhli
+00012500: 6e65 2c20 706f 733d 6c69 6e65 5f73 7065  ne, pos=line_spe
+00012510: 6329 0a0a 2020 2020 2020 2020 6966 2076  c)..        if v
+00012520: 6c69 6e65 7320 6973 206e 6f74 204e 6f6e  lines is not Non
+00012530: 653a 0a20 2020 2020 2020 2020 2020 2066  e:.            f
+00012540: 6f72 206c 696e 655f 7370 6563 2069 6e20  or line_spec in 
+00012550: 766c 696e 6573 3a0a 2020 2020 2020 2020  vlines:.        
+00012560: 2020 2020 2020 2020 6966 2069 7369 6e73          if isins
+00012570: 7461 6e63 6528 6c69 6e65 5f73 7065 632c  tance(line_spec,
+00012580: 2064 6963 7429 3a0a 2020 2020 2020 2020   dict):.        
+00012590: 2020 2020 2020 2020 2020 2020 7365 745f              set_
+000125a0: 6c69 6e65 2873 656c 662e 6178 2e61 7876  line(self.ax.axv
+000125b0: 6c69 6e65 2c20 2a2a 6c69 6e65 5f73 7065  line, **line_spe
+000125c0: 6329 0a20 2020 2020 2020 2020 2020 2020  c).             
+000125d0: 2020 2065 6c73 653a 0a20 2020 2020 2020     else:.       
+000125e0: 2020 2020 2020 2020 2020 2020 2073 6574               set
+000125f0: 5f6c 696e 6528 7365 6c66 2e61 782e 6178  _line(self.ax.ax
+00012600: 766c 696e 652c 2070 6f73 3d6c 696e 655f  vline, pos=line_
+00012610: 7370 6563 290a 0a20 2020 2064 6566 205f  spec)..    def _
+00012620: 686c 7072 5f73 6574 5f73 6361 6c65 7328  hlpr_set_scales(
+00012630: 0a20 2020 2020 2020 2073 656c 662c 0a20  .        self,. 
+00012640: 2020 2020 2020 202a 2c0a 2020 2020 2020         *,.      
+00012650: 2020 783a 2055 6e69 6f6e 5b73 7472 2c20    x: Union[str, 
+00012660: 6469 6374 5d20 3d20 4e6f 6e65 2c0a 2020  dict] = None,.  
+00012670: 2020 2020 2020 793a 2055 6e69 6f6e 5b73        y: Union[s
+00012680: 7472 2c20 6469 6374 5d20 3d20 4e6f 6e65  tr, dict] = None
+00012690: 2c0a 2020 2020 2020 2020 7a3a 2055 6e69  ,.        z: Uni
+000126a0: 6f6e 5b73 7472 2c20 6469 6374 5d20 3d20  on[str, dict] = 
+000126b0: 4e6f 6e65 2c0a 2020 2020 293a 0a20 2020  None,.    ):.   
+000126c0: 2020 2020 2022 2222 5365 7473 2074 6865       """Sets the
+000126d0: 2073 6361 6c65 7320 666f 7220 7468 6520   scales for the 
+000126e0: 6375 7272 656e 7420 6178 6973 0a0a 2020  current axis..  
+000126f0: 2020 2020 2020 5468 6520 6172 6775 6d65        The argume
+00012700: 6e74 7320 6172 6520 7573 6564 2074 6f20  nts are used to 
+00012710: 6361 6c6c 0a20 2020 2020 2020 203a 7079  call.        :py
+00012720: 3a6d 6574 683a 606d 6174 706c 6f74 6c69  :meth:`matplotli
+00012730: 622e 6178 6573 2e41 7865 732e 7365 745f  b.axes.Axes.set_
+00012740: 7873 6361 6c65 6020 616e 642f 6f72 0a20  xscale` and/or. 
+00012750: 2020 2020 2020 203a 7079 3a6d 6574 683a         :py:meth:
+00012760: 606d 6174 706c 6f74 6c69 622e 6178 6573  `matplotlib.axes
+00012770: 2e41 7865 732e 7365 745f 7973 6361 6c65  .Axes.set_yscale
+00012780: 6020 616e 640a 2020 2020 2020 2020 3a70  ` and.        :p
+00012790: 793a 6d65 7468 3a60 6d70 6c5f 746f 6f6c  y:meth:`mpl_tool
+000127a0: 6b69 7473 2e6d 706c 6f74 3364 2e61 7865  kits.mplot3d.axe
+000127b0: 7333 642e 4178 6573 3344 2e73 6574 5f7a  s3d.Axes3D.set_z
+000127c0: 7363 616c 6560 2c20 7265 7370 6563 7469  scale`, respecti
+000127d0: 7665 6c79 2e0a 2020 2020 2020 2020 466f  vely..        Fo
+000127e0: 7220 7374 7269 6e67 2d6c 696b 6520 6172  r string-like ar
+000127f0: 6775 6d65 6e74 732c 2074 6865 2076 616c  guments, the val
+00012800: 7565 2069 7320 6469 7265 6374 6c79 2075  ue is directly u
+00012810: 7365 6420 746f 2073 6574 2074 6865 2073  sed to set the s
+00012820: 6361 6c65 0a20 2020 2020 2020 2066 6f72  cale.        for
+00012830: 2074 6861 7420 6178 6973 2c20 652e 672e   that axis, e.g.
+00012840: 2060 606c 696e 6561 7260 602c 2060 606c   ``linear``, ``l
+00012850: 6f67 6060 2c20 6060 7379 6d6c 6f67 6060  og``, ``symlog``
+00012860: 2e0a 2020 2020 2020 2020 4f74 6865 7277  ..        Otherw
+00012870: 6973 652c 2064 6963 742d 6c69 6b65 2061  ise, dict-like a
+00012880: 7267 756d 656e 7473 2061 7265 2065 7870  rguments are exp
+00012890: 6563 7465 6420 7768 6572 6520 6120 6060  ected where a ``
+000128a0: 7363 616c 6560 6020 6b65 7920 6973 0a20  scale`` key is. 
+000128b0: 2020 2020 2020 2070 7265 7365 6e74 2061         present a
+000128c0: 6e64 2064 6566 696e 6573 2077 6869 6368  nd defines which
+000128d0: 2074 7970 6520 6f66 2073 6361 6c65 2074   type of scale t
+000128e0: 6f20 7573 652e 2041 6c6c 2066 7572 7468  o use. All furth
+000128f0: 6572 2061 7267 756d 656e 7473 0a20 2020  er arguments.   
+00012900: 2020 2020 2061 7265 2070 6173 7365 6420       are passed 
+00012910: 6f6e 3b20 7468 6573 6520 6172 6520 7265  on; these are re
+00012920: 6c65 7661 6e74 2066 6f72 2074 6865 2073  levant for the s
+00012930: 796d 6d65 7472 6963 616c 206c 6f67 6172  ymmetrical logar
+00012940: 6974 686d 6963 0a20 2020 2020 2020 2073  ithmic.        s
+00012950: 6361 6c65 2c20 666f 7220 6578 616d 706c  cale, for exampl
+00012960: 652e 0a0a 2020 2020 2020 2020 4172 6773  e...        Args
+00012970: 3a0a 2020 2020 2020 2020 2020 2020 7820  :.            x 
+00012980: 2855 6e69 6f6e 5b73 7472 2c20 6469 6374  (Union[str, dict
+00012990: 5d2c 206f 7074 696f 6e61 6c29 3a20 5468  ], optional): Th
+000129a0: 6520 7363 616c 6573 2074 6f20 7573 6520  e scales to use 
+000129b0: 6f6e 2074 6865 2078 2d61 7869 730a 2020  on the x-axis.  
+000129c0: 2020 2020 2020 2020 2020 7920 2855 6e69            y (Uni
+000129d0: 6f6e 5b73 7472 2c20 6469 6374 5d2c 206f  on[str, dict], o
+000129e0: 7074 696f 6e61 6c29 3a20 5468 6520 7363  ptional): The sc
+000129f0: 616c 6573 2074 6f20 7573 6520 6f6e 2074  ales to use on t
+00012a00: 6865 2079 2d61 7869 730a 2020 2020 2020  he y-axis.      
+00012a10: 2020 2020 2020 7a20 2855 6e69 6f6e 5b73        z (Union[s
+00012a20: 7472 2c20 6469 6374 5d2c 206f 7074 696f  tr, dict], optio
+00012a30: 6e61 6c29 3a20 5468 6520 7363 616c 6573  nal): The scales
+00012a40: 2074 6f20 7573 6520 6f6e 2074 6865 207a   to use on the z
+00012a50: 2d61 7869 732e 0a20 2020 2020 2020 2020  -axis..         
+00012a60: 2020 2020 2020 2049 6620 7468 6572 6520         If there 
+00012a70: 6973 206e 6f20 7a2d 6178 6973 2c20 7468  is no z-axis, th
+00012a80: 6973 2077 696c 6c20 6265 2073 696c 656e  is will be silen
+00012a90: 746c 7920 6967 6e6f 7265 642e 0a20 2020  tly ignored..   
+00012aa0: 2020 2020 2022 2222 0a0a 2020 2020 2020       """..      
+00012ab0: 2020 6465 6620 7365 745f 7363 616c 6528    def set_scale(
+00012ac0: 6675 6e63 3a20 4361 6c6c 6162 6c65 2c20  func: Callable, 
+00012ad0: 2a2c 2073 6361 6c65 3a20 7374 7220 3d20  *, scale: str = 
+00012ae0: 4e6f 6e65 2c20 2a2a 7363 616c 655f 6b77  None, **scale_kw
+00012af0: 6172 6773 293a 0a20 2020 2020 2020 2020  args):.         
+00012b00: 2020 2066 756e 6328 7363 616c 652c 202a     func(scale, *
+00012b10: 2a73 6361 6c65 5f6b 7761 7267 7329 0a0a  *scale_kwargs)..
+00012b20: 2020 2020 2020 2020 6966 2078 3a0a 2020          if x:.  
+00012b30: 2020 2020 2020 2020 2020 7820 3d20 7820            x = x 
+00012b40: 6966 206e 6f74 2069 7369 6e73 7461 6e63  if not isinstanc
+00012b50: 6528 782c 2073 7472 2920 656c 7365 2064  e(x, str) else d
+00012b60: 6963 7428 7363 616c 653d 7829 0a20 2020  ict(scale=x).   
+00012b70: 2020 2020 2020 2020 2073 6574 5f73 6361           set_sca
+00012b80: 6c65 2873 656c 662e 6178 2e73 6574 5f78  le(self.ax.set_x
+00012b90: 7363 616c 652c 202a 2a78 290a 0a20 2020  scale, **x)..   
+00012ba0: 2020 2020 2069 6620 793a 0a20 2020 2020       if y:.     
+00012bb0: 2020 2020 2020 2079 203d 2079 2069 6620         y = y if 
+00012bc0: 6e6f 7420 6973 696e 7374 616e 6365 2879  not isinstance(y
+00012bd0: 2c20 7374 7229 2065 6c73 6520 6469 6374  , str) else dict
+00012be0: 2873 6361 6c65 3d79 290a 2020 2020 2020  (scale=y).      
+00012bf0: 2020 2020 2020 7365 745f 7363 616c 6528        set_scale(
+00012c00: 7365 6c66 2e61 782e 7365 745f 7973 6361  self.ax.set_ysca
+00012c10: 6c65 2c20 2a2a 7929 0a0a 2020 2020 2020  le, **y)..      
+00012c20: 2020 6966 2068 6173 6174 7472 2873 656c    if hasattr(sel
+00012c30: 662e 6178 2c20 227a 6178 6973 2229 3a0a  f.ax, "zaxis"):.
+00012c40: 2020 2020 2020 2020 2020 2020 6966 207a              if z
+00012c50: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00012c60: 2020 7a20 3d20 7a20 6966 206e 6f74 2069    z = z if not i
+00012c70: 7369 6e73 7461 6e63 6528 7a2c 2073 7472  sinstance(z, str
+00012c80: 2920 656c 7365 2064 6963 7428 7363 616c  ) else dict(scal
+00012c90: 653d 7a29 0a20 2020 2020 2020 2020 2020  e=z).           
+00012ca0: 2020 2020 2073 6574 5f73 6361 6c65 2873       set_scale(s
+00012cb0: 656c 662e 6178 2e73 6574 5f7a 7363 616c  elf.ax.set_zscal
+00012cc0: 652c 202a 2a7a 290a 0a20 2020 2064 6566  e, **z)..    def
+00012cd0: 205f 686c 7072 5f73 6574 5f74 6963 6b73   _hlpr_set_ticks
+00012ce0: 280a 2020 2020 2020 2020 7365 6c66 2c0a  (.        self,.
+00012cf0: 2020 2020 2020 2020 2a2c 0a20 2020 2020          *,.     
+00012d00: 2020 2078 3a20 556e 696f 6e5b 6c69 7374     x: Union[list
+00012d10: 2c20 6469 6374 5d20 3d20 4e6f 6e65 2c0a  , dict] = None,.
+00012d20: 2020 2020 2020 2020 793a 2055 6e69 6f6e          y: Union
+00012d30: 5b6c 6973 742c 2064 6963 745d 203d 204e  [list, dict] = N
+00012d40: 6f6e 652c 0a20 2020 2020 2020 207a 3a20  one,.        z: 
+00012d50: 556e 696f 6e5b 6c69 7374 2c20 6469 6374  Union[list, dict
+00012d60: 5d20 3d20 4e6f 6e65 2c0a 2020 2020 293a  ] = None,.    ):
+00012d70: 0a20 2020 2020 2020 2022 2222 5365 7473  .        """Sets
+00012d80: 2074 6865 2074 6963 6b73 2066 6f72 2074   the ticks for t
+00012d90: 6865 2063 7572 7265 6e74 2061 7869 730a  he current axis.
+00012da0: 0a20 2020 2020 2020 2054 6865 2061 7267  .        The arg
+00012db0: 756d 656e 7473 2061 7265 2075 7365 6420  uments are used 
+00012dc0: 746f 2063 616c 6c0a 2020 2020 2020 2020  to call.        
+00012dd0: 3a70 793a 6d65 7468 3a60 6d61 7470 6c6f  :py:meth:`matplo
+00012de0: 746c 6962 2e61 7865 732e 4178 6573 2e73  tlib.axes.Axes.s
+00012df0: 6574 5f78 7469 636b 7360 206f 720a 2020  et_xticks` or.  
+00012e00: 2020 2020 2020 3a70 793a 6d65 7468 3a60        :py:meth:`
+00012e10: 6d61 7470 6c6f 746c 6962 2e61 7865 732e  matplotlib.axes.
+00012e20: 4178 6573 2e73 6574 5f79 7469 636b 7360  Axes.set_yticks`
+00012e30: 206f 720a 2020 2020 2020 2020 3a70 793a   or.        :py:
+00012e40: 6d65 7468 3a60 6d70 6c5f 746f 6f6c 6b69  meth:`mpl_toolki
+00012e50: 7473 2e6d 706c 6f74 3364 2e61 7865 7333  ts.mplot3d.axes3
+00012e60: 642e 4178 6573 3344 2e73 6574 5f7a 7469  d.Axes3D.set_zti
+00012e70: 636b 7360 2c0a 2020 2020 2020 2020 616e  cks`,.        an
+00012e80: 6420 3a70 793a 6d65 7468 3a60 6d61 7470  d :py:meth:`matp
+00012e90: 6c6f 746c 6962 2e61 7865 732e 4178 6573  lotlib.axes.Axes
+00012ea0: 2e73 6574 5f78 7469 636b 6c61 6265 6c73  .set_xticklabels
+00012eb0: 6020 6f72 0a20 2020 2020 2020 203a 7079  ` or.        :py
+00012ec0: 3a6d 6574 683a 606d 6174 706c 6f74 6c69  :meth:`matplotli
+00012ed0: 622e 6178 6573 2e41 7865 732e 7365 745f  b.axes.Axes.set_
+00012ee0: 7974 6963 6b6c 6162 656c 7360 206f 720a  yticklabels` or.
+00012ef0: 2020 2020 2020 2020 3a70 793a 6d65 7468          :py:meth
+00012f00: 3a60 6d70 6c5f 746f 6f6c 6b69 7473 2e6d  :`mpl_toolkits.m
+00012f10: 706c 6f74 3364 2e61 7865 7333 642e 4178  plot3d.axes3d.Ax
+00012f20: 6573 3344 2e73 6574 5f7a 7469 636b 6c61  es3D.set_ztickla
+00012f30: 6265 6c73 602c 0a20 2020 2020 2020 2072  bels`,.        r
+00012f40: 6573 7065 6374 6976 656c 792e 0a0a 2020  espectively...  
+00012f50: 2020 2020 2020 5468 6520 6469 6374 2d6c        The dict-l
+00012f60: 696b 6520 6172 6775 6d65 6e74 7320 6d61  ike arguments ma
+00012f70: 7920 636f 6e74 6169 6e20 7468 6520 6b65  y contain the ke
+00012f80: 7973 2060 606d 616a 6f72 6060 2061 6e64  ys ``major`` and
+00012f90: 2f6f 720a 2020 2020 2020 2020 6060 6d69  /or.        ``mi
+00012fa0: 6e6f 7260 602c 2072 6566 6572 7269 6e67  nor``, referring
+00012fb0: 2074 6f20 6d61 6a6f 7220 6f72 206d 696e   to major or min
+00012fc0: 6f72 2074 6963 6b20 6c6f 6361 7469 6f6e  or tick location
+00012fd0: 7320 616e 6420 6c61 6265 6c73 2c0a 2020  s and labels,.  
+00012fe0: 2020 2020 2020 7265 7370 6563 7469 7665        respective
+00012ff0: 6c79 2e0a 2020 2020 2020 2020 5468 6579  ly..        They
+00013000: 2073 686f 756c 6420 6569 7468 6572 2062   should either b
+00013010: 6520 6c69 7374 2d6c 696b 652c 2064 6972  e list-like, dir
+00013020: 6563 746c 7920 7370 6563 6966 7969 6e67  ectly specifying
+00013030: 2074 6865 2074 6963 6b73 270a 2020 2020   the ticks'.    
+00013040: 2020 2020 6c6f 6361 7469 6f6e 732c 206f      locations, o
+00013050: 7220 6469 6374 2d6c 696b 6520 7265 7175  r dict-like requ
+00013060: 6972 696e 6720 6120 6060 6c6f 6373 6060  iring a ``locs``
+00013070: 206b 6579 2074 6861 7420 636f 6e74 6169   key that contai
+00013080: 6e73 2074 6865 0a20 2020 2020 2020 2074  ns the.        t
+00013090: 6963 6b73 2720 6c6f 6361 7469 6f6e 7320  icks' locations 
+000130a0: 616e 6420 6973 2070 6173 7365 6420 6f6e  and is passed on
+000130b0: 2074 6f20 7468 6520 6060 7365 745f 3c78   to the ``set_<x
+000130c0: 2f79 2f7a 3e74 6963 6b73 6060 2063 616c  /y/z>ticks`` cal
+000130d0: 6c2e 0a20 2020 2020 2020 2061 7320 6060  l..        as ``
+000130e0: 7469 636b 7360 6020 6172 6775 6d65 6e74  ticks`` argument
+000130f0: 2e20 4675 7274 6865 7220 6b77 6172 6773  . Further kwargs
+00013100: 2073 7563 6820 6173 2060 606c 6162 656c   such as ``label
+00013110: 7360 6020 6361 6e20 6265 2067 6976 656e  s`` can be given
+00013120: 0a20 2020 2020 2020 2061 6e64 2061 7265  .        and are
+00013130: 2070 6173 7365 6420 6f6e 2074 6f20 7468   passed on to th
+00013140: 6520 6060 7365 745f 3c78 2f79 2f7a 3e74  e ``set_<x/y/z>t
+00013150: 6963 6b6c 6162 656c 7360 6020 6361 6c6c  icklabels`` call
+00013160: 2e0a 0a20 2020 2020 2020 2045 7861 6d70  ...        Examp
+00013170: 6c65 3a0a 0a20 2020 2020 2020 202e 2e20  le:..        .. 
+00013180: 636f 6465 2d62 6c6f 636b 3a3a 2079 616d  code-block:: yam
+00013190: 6c0a 0a20 2020 2020 2020 2020 2020 2073  l..            s
+000131a0: 6574 5f74 6963 6b73 3a0a 2020 2020 2020  et_ticks:.      
+000131b0: 2020 2020 2020 2020 783a 0a20 2020 2020          x:.     
+000131c0: 2020 2020 2020 2020 2020 206d 616a 6f72             major
+000131d0: 3a20 5b32 2c20 342c 2036 2c20 385d 0a20  : [2, 4, 6, 8]. 
+000131e0: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+000131f0: 696e 6f72 3a0a 2020 2020 2020 2020 2020  inor:.          
+00013200: 2020 2020 2020 2020 6c6f 6373 3a20 5b31          locs: [1
+00013210: 2c20 332c 2035 2c20 372c 2039 5d0a 2020  , 3, 5, 7, 9].  
+00013220: 2020 2020 2020 2020 2020 2020 793a 0a20              y:. 
+00013230: 2020 2020 2020 2020 2020 2020 2020 206d                 m
+00013240: 616a 6f72 3a0a 2020 2020 2020 2020 2020  ajor:.          
+00013250: 2020 2020 2020 2020 6c6f 6373 3a20 5b30          locs: [0
+00013260: 2c20 3130 3030 2c20 3230 3030 2c20 3330  , 1000, 2000, 30
+00013270: 3030 5d0a 2020 2020 2020 2020 2020 2020  00].            
+00013280: 2020 2020 2020 6c61 6265 6c73 3a20 5b30        labels: [0
+00013290: 2c20 316b 2c20 326b 2c20 336b 5d0a 2020  , 1k, 2k, 3k].  
+000132a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000132b0: 2320 2e2e 2e20 6675 7274 6865 7220 6b77  # ... further kw
+000132c0: 6172 6773 2068 6572 6520 7370 6563 6966  args here specif
+000132d0: 7920 6c61 6265 6c20 6165 7374 6865 7469  y label aestheti
+000132e0: 6373 0a0a 2020 2020 2020 2020 2020 2020  cs..            
+000132f0: 2020 7a3a 205b 2d31 2c20 302c 202b 315d    z: [-1, 0, +1]
+00013300: 2020 2320 7361 6d65 2061 7320 7a3a 207b    # same as z: {
+00013310: 6d61 6a6f 723a 207b 6c6f 6373 3a20 5b2d  major: {locs: [-
+00013320: 312c 2030 2c20 2b31 5d7d 7d0a 0a20 2020  1, 0, +1]}}..   
+00013330: 2020 2020 2041 7267 733a 0a20 2020 2020       Args:.     
+00013340: 2020 2020 2020 2078 2028 556e 696f 6e5b         x (Union[
+00013350: 6c69 7374 2c20 6469 6374 5d2c 206f 7074  list, dict], opt
+00013360: 696f 6e61 6c29 3a20 5468 6520 7469 636b  ional): The tick
+00013370: 7320 616e 6420 6f70 7469 6f6e 616c 6c79  s and optionally
+00013380: 2074 6865 6972 0a20 2020 2020 2020 2020   their.         
+00013390: 2020 2020 2020 206c 6162 656c 7320 746f         labels to
+000133a0: 2073 6574 206f 6e20 7468 6520 782d 6178   set on the x-ax
+000133b0: 6973 0a20 2020 2020 2020 2020 2020 2079  is.            y
+000133c0: 2028 556e 696f 6e5b 6c69 7374 2c20 6469   (Union[list, di
+000133d0: 6374 5d2c 206f 7074 696f 6e61 6c29 3a20  ct], optional): 
+000133e0: 5468 6520 7469 636b 7320 616e 6420 6f70  The ticks and op
+000133f0: 7469 6f6e 616c 6c79 2074 6865 6972 0a20  tionally their. 
+00013400: 2020 2020 2020 2020 2020 2020 2020 206c                 l
+00013410: 6162 656c 7320 746f 2073 6574 206f 6e20  abels to set on 
+00013420: 7468 6520 792d 6178 6973 0a20 2020 2020  the y-axis.     
+00013430: 2020 2020 2020 207a 2028 556e 696f 6e5b         z (Union[
+00013440: 6c69 7374 2c20 6469 6374 5d2c 206f 7074  list, dict], opt
+00013450: 696f 6e61 6c29 3a20 5468 6520 7469 636b  ional): The tick
+00013460: 7320 616e 6420 6f70 7469 6f6e 616c 6c79  s and optionally
+00013470: 2074 6865 6972 0a20 2020 2020 2020 2020   their.         
+00013480: 2020 2020 2020 206c 6162 656c 7320 746f         labels to
+00013490: 2073 6574 206f 6e20 7468 6520 7a2d 6178   set on the z-ax
+000134a0: 6973 2e0a 2020 2020 2020 2020 2020 2020  is..            
+000134b0: 2020 2020 4966 2074 6865 7265 2069 7320      If there is 
+000134c0: 6e6f 207a 2d61 7869 732c 2074 6869 7320  no z-axis, this 
+000134d0: 7769 6c6c 2062 6520 7369 6c65 6e74 6c79  will be silently
+000134e0: 2069 676e 6f72 6564 2e0a 2020 2020 2020   ignored..      
+000134f0: 2020 2222 220a 0a20 2020 2020 2020 2064    """..        d
+00013500: 6566 2073 6574 5f74 6963 6b73 280a 2020  ef set_ticks(.  
+00013510: 2020 2020 2020 2020 2020 6675 6e63 3a20            func: 
+00013520: 4361 6c6c 6162 6c65 2c0a 2020 2020 2020  Callable,.      
+00013530: 2020 2020 2020 2a2c 0a20 2020 2020 2020        *,.       
+00013540: 2020 2020 2074 6963 6b73 3a20 6c69 7374       ticks: list
+00013550: 2c0a 2020 2020 2020 2020 2020 2020 6d69  ,.            mi
+00013560: 6e6f 723a 2062 6f6f 6c2c 0a20 2020 2020  nor: bool,.     
+00013570: 2020 2029 3a0a 2020 2020 2020 2020 2020     ):.          
+00013580: 2020 6675 6e63 2874 6963 6b73 2c20 6d69    func(ticks, mi
+00013590: 6e6f 723d 6d69 6e6f 7229 0a0a 2020 2020  nor=minor)..    
+000135a0: 2020 2020 6465 6620 7365 745f 7469 636b      def set_tick
+000135b0: 6c61 6265 6c73 280a 2020 2020 2020 2020  labels(.        
+000135c0: 2020 2020 6675 6e63 3a20 4361 6c6c 6162      func: Callab
+000135d0: 6c65 2c20 2a2c 206c 6162 656c 733a 206c  le, *, labels: l
+000135e0: 6973 742c 202a 2a74 6963 6b6c 6162 656c  ist, **ticklabel
+000135f0: 735f 6b77 6172 6773 0a20 2020 2020 2020  s_kwargs.       
+00013600: 2029 3a0a 2020 2020 2020 2020 2020 2020   ):.            
+00013610: 6675 6e63 286c 6162 656c 732c 202a 2a74  func(labels, **t
+00013620: 6963 6b6c 6162 656c 735f 6b77 6172 6773  icklabels_kwargs
+00013630: 290a 0a20 2020 2020 2020 2064 6566 2073  )..        def s
+00013640: 6574 5f74 6963 6b73 5f61 6e64 5f6c 6162  et_ticks_and_lab
+00013650: 656c 7328 0a20 2020 2020 2020 2020 2020  els(.           
+00013660: 202a 2c20 6178 6973 3a20 7374 722c 206d   *, axis: str, m
+00013670: 696e 6f72 3a20 626f 6f6c 2c20 6178 6973  inor: bool, axis
+00013680: 5f63 6667 3a20 556e 696f 6e5b 6469 6374  _cfg: Union[dict
+00013690: 2c20 6c69 7374 2c20 7475 706c 655d 0a20  , list, tuple]. 
+000136a0: 2020 2020 2020 2029 3a0a 2020 2020 2020         ):.      
+000136b0: 2020 2020 2020 6178 6973 5f63 6667 203d        axis_cfg =
+000136c0: 2028 0a20 2020 2020 2020 2020 2020 2020   (.             
+000136d0: 2020 2061 7869 735f 6366 670a 2020 2020     axis_cfg.    
+000136e0: 2020 2020 2020 2020 2020 2020 6966 206e              if n
+000136f0: 6f74 2069 7369 6e73 7461 6e63 6528 6178  ot isinstance(ax
+00013700: 6973 5f63 6667 2c20 286c 6973 742c 2074  is_cfg, (list, t
+00013710: 7570 6c65 2929 0a20 2020 2020 2020 2020  uple)).         
+00013720: 2020 2020 2020 2065 6c73 6520 6469 6374         else dict
+00013730: 286c 6f63 733d 6178 6973 5f63 6667 290a  (locs=axis_cfg).
+00013740: 2020 2020 2020 2020 2020 2020 290a 0a20              ).. 
+00013750: 2020 2020 2020 2020 2020 2069 6620 6178             if ax
+00013760: 6973 5f63 6667 2e67 6574 2822 6c61 6265  is_cfg.get("labe
+00013770: 6c73 2229 2061 6e64 206e 6f74 2061 7869  ls") and not axi
+00013780: 735f 6366 672e 6765 7428 226c 6f63 7322  s_cfg.get("locs"
+00013790: 293a 0a20 2020 2020 2020 2020 2020 2020  ):.             
+000137a0: 2020 2072 6169 7365 2050 6c6f 7443 6f6e     raise PlotCon
+000137b0: 6669 6745 7272 6f72 280a 2020 2020 2020  figError(.      
+000137c0: 2020 2020 2020 2020 2020 2020 2020 224c                "L
+000137d0: 6162 656c 7320 6361 6e20 6f6e 6c79 2062  abels can only b
+000137e0: 6520 7365 7420 7468 726f 7567 6820 7468  e set through th
+000137f0: 6520 606c 6162 656c 7360 2061 7267 756d  e `labels` argum
+00013800: 656e 7420 220a 2020 2020 2020 2020 2020  ent ".          
+00013810: 2020 2020 2020 2020 2020 2269 6620 7468            "if th
+00013820: 6569 7220 6c6f 6361 7469 6f6e 2069 7320  eir location is 
+00013830: 616c 736f 2067 6976 656e 2074 6872 6f75  also given throu
+00013840: 6768 2074 6865 2060 6c6f 6373 6020 220a  gh the `locs` ".
+00013850: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013860: 2020 2020 2261 7267 756d 656e 742e 2048      "argument. H
+00013870: 6f77 6576 6572 2c20 606c 6f63 7360 2069  owever, `locs` i
+00013880: 7320 6e6f 7420 6769 7665 6e2e 220a 2020  s not given.".  
+00013890: 2020 2020 2020 2020 2020 2020 2020 290a                ).
+000138a0: 0a20 2020 2020 2020 2020 2020 2023 2047  .            # G
+000138b0: 6574 2074 6865 2061 7869 7320 7370 6563  et the axis spec
+000138c0: 6966 6963 0a20 2020 2020 2020 2020 2020  ific.           
+000138d0: 2069 6620 6178 6973 203d 3d20 2278 223a   if axis == "x":
+000138e0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+000138f0: 2074 6963 6b73 5f66 756e 6320 3d20 7365   ticks_func = se
+00013900: 6c66 2e61 782e 7365 745f 7874 6963 6b73  lf.ax.set_xticks
+00013910: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013920: 2074 6963 6b73 6c61 6265 6c5f 6675 6e63   tickslabel_func
+00013930: 203d 2073 656c 662e 6178 2e73 6574 5f78   = self.ax.set_x
+00013940: 7469 636b 6c61 6265 6c73 0a20 2020 2020  ticklabels.     
+00013950: 2020 2020 2020 2065 6c69 6620 6178 6973         elif axis
+00013960: 203d 3d20 2279 223a 0a20 2020 2020 2020   == "y":.       
+00013970: 2020 2020 2020 2020 2074 6963 6b73 5f66           ticks_f
+00013980: 756e 6320 3d20 7365 6c66 2e61 782e 7365  unc = self.ax.se
+00013990: 745f 7974 6963 6b73 0a20 2020 2020 2020  t_yticks.       
+000139a0: 2020 2020 2020 2020 2074 6963 6b73 6c61           ticksla
+000139b0: 6265 6c5f 6675 6e63 203d 2073 656c 662e  bel_func = self.
+000139c0: 6178 2e73 6574 5f79 7469 636b 6c61 6265  ax.set_yticklabe
+000139d0: 6c73 0a20 2020 2020 2020 2020 2020 2065  ls.            e
+000139e0: 6c69 6620 6178 6973 203d 3d20 227a 223a  lif axis == "z":
+000139f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013a00: 2074 6963 6b73 5f66 756e 6320 3d20 7365   ticks_func = se
+00013a10: 6c66 2e61 782e 7365 745f 7a74 6963 6b73  lf.ax.set_zticks
+00013a20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013a30: 2074 6963 6b73 6c61 6265 6c5f 6675 6e63   tickslabel_func
+00013a40: 203d 2073 656c 662e 6178 2e73 6574 5f7a   = self.ax.set_z
+00013a50: 7469 636b 6c61 6265 6c73 0a0a 2020 2020  ticklabels..    
+00013a60: 2020 2020 2020 2020 2320 5365 7420 7468          # Set th
+00013a70: 6520 7469 636b 730a 2020 2020 2020 2020  e ticks.        
+00013a80: 2020 2020 7365 745f 7469 636b 7328 7469      set_ticks(ti
+00013a90: 636b 735f 6675 6e63 2c20 7469 636b 733d  cks_func, ticks=
+00013aa0: 6178 6973 5f63 6667 2e70 6f70 2822 6c6f  axis_cfg.pop("lo
+00013ab0: 6373 2229 2c20 6d69 6e6f 723d 6d69 6e6f  cs"), minor=mino
+00013ac0: 7229 0a0a 2020 2020 2020 2020 2020 2020  r)..            
+00013ad0: 2320 5365 7420 7468 6520 7469 636b 206c  # Set the tick l
+00013ae0: 6162 656c 732c 2070 6173 7369 6e67 206f  abels, passing o
+00013af0: 6e20 7468 6520 6164 6469 7469 6f6e 616c  n the additional
+00013b00: 206b 7761 7267 730a 2020 2020 2020 2020   kwargs.        
+00013b10: 2020 2020 6966 2061 7869 735f 6366 672e      if axis_cfg.
+00013b20: 6765 7428 226c 6162 656c 7322 293a 0a20  get("labels"):. 
+00013b30: 2020 2020 2020 2020 2020 2020 2020 2073                 s
+00013b40: 6574 5f74 6963 6b6c 6162 656c 7328 7469  et_ticklabels(ti
+00013b50: 636b 736c 6162 656c 5f66 756e 632c 206d  ckslabel_func, m
+00013b60: 696e 6f72 3d6d 696e 6f72 2c20 2a2a 6178  inor=minor, **ax
+00013b70: 6973 5f63 6667 290a 0a20 2020 2020 2020  is_cfg)..       
+00013b80: 2069 6620 783a 0a20 2020 2020 2020 2020   if x:.         
+00013b90: 2020 2069 6620 6973 696e 7374 616e 6365     if isinstance
+00013ba0: 2878 2c20 286c 6973 742c 2074 7570 6c65  (x, (list, tuple
+00013bb0: 2929 3a0a 2020 2020 2020 2020 2020 2020  )):.            
+00013bc0: 2020 2020 7820 3d20 6469 6374 286d 616a      x = dict(maj
+00013bd0: 6f72 3d64 6963 7428 6c6f 6373 3d78 2929  or=dict(locs=x))
+00013be0: 0a0a 2020 2020 2020 2020 2020 2020 6966  ..            if
+00013bf0: 2078 2e67 6574 2822 6d61 6a6f 7222 2920   x.get("major") 
+00013c00: 6973 206e 6f74 204e 6f6e 653a 0a20 2020  is not None:.   
+00013c10: 2020 2020 2020 2020 2020 2020 2073 6574               set
+00013c20: 5f74 6963 6b73 5f61 6e64 5f6c 6162 656c  _ticks_and_label
+00013c30: 7328 0a20 2020 2020 2020 2020 2020 2020  s(.             
+00013c40: 2020 2020 2020 2061 7869 733d 2278 222c         axis="x",
+00013c50: 206d 696e 6f72 3d46 616c 7365 2c20 6178   minor=False, ax
+00013c60: 6973 5f63 6667 3d78 5b22 6d61 6a6f 7222  is_cfg=x["major"
+00013c70: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00013c80: 2020 290a 0a20 2020 2020 2020 2020 2020    )..           
+00013c90: 2069 6620 782e 6765 7428 226d 696e 6f72   if x.get("minor
+00013ca0: 2229 2069 7320 6e6f 7420 4e6f 6e65 3a0a  ") is not None:.
+00013cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013cc0: 7365 745f 7469 636b 735f 616e 645f 6c61  set_ticks_and_la
+00013cd0: 6265 6c73 2861 7869 733d 2278 222c 206d  bels(axis="x", m
+00013ce0: 696e 6f72 3d54 7275 652c 2061 7869 735f  inor=True, axis_
+00013cf0: 6366 673d 785b 226d 696e 6f72 225d 290a  cfg=x["minor"]).
+00013d00: 0a20 2020 2020 2020 2069 6620 793a 0a20  .        if y:. 
+00013d10: 2020 2020 2020 2020 2020 2069 6620 6973             if is
+00013d20: 696e 7374 616e 6365 2879 2c20 286c 6973  instance(y, (lis
+00013d30: 742c 2074 7570 6c65 2929 3a0a 2020 2020  t, tuple)):.    
+00013d40: 2020 2020 2020 2020 2020 2020 7920 3d20              y = 
+00013d50: 6469 6374 286d 616a 6f72 3d64 6963 7428  dict(major=dict(
+00013d60: 6c6f 6373 3d79 2929 0a0a 2020 2020 2020  locs=y))..      
+00013d70: 2020 2020 2020 6966 2079 2e67 6574 2822        if y.get("
+00013d80: 6d61 6a6f 7222 2920 6973 206e 6f74 204e  major") is not N
+00013d90: 6f6e 653a 0a20 2020 2020 2020 2020 2020  one:.           
+00013da0: 2020 2020 2073 6574 5f74 6963 6b73 5f61       set_ticks_a
+00013db0: 6e64 5f6c 6162 656c 7328 0a20 2020 2020  nd_labels(.     
+00013dc0: 2020 2020 2020 2020 2020 2020 2020 2061                 a
+00013dd0: 7869 733d 2279 222c 206d 696e 6f72 3d46  xis="y", minor=F
+00013de0: 616c 7365 2c20 6178 6973 5f63 6667 3d79  alse, axis_cfg=y
+00013df0: 5b22 6d61 6a6f 7222 5d0a 2020 2020 2020  ["major"].      
+00013e00: 2020 2020 2020 2020 2020 290a 0a20 2020            )..   
+00013e10: 2020 2020 2020 2020 2069 6620 792e 6765           if y.ge
+00013e20: 7428 226d 696e 6f72 2229 2069 7320 6e6f  t("minor") is no
+00013e30: 7420 4e6f 6e65 3a0a 2020 2020 2020 2020  t None:.        
+00013e40: 2020 2020 2020 2020 7365 745f 7469 636b          set_tick
+00013e50: 735f 616e 645f 6c61 6265 6c73 2861 7869  s_and_labels(axi
+00013e60: 733d 2279 222c 206d 696e 6f72 3d54 7275  s="y", minor=Tru
+00013e70: 652c 2061 7869 735f 6366 673d 795b 226d  e, axis_cfg=y["m
+00013e80: 696e 6f72 225d 290a 0a20 2020 2020 2020  inor"])..       
+00013e90: 2069 6620 6861 7361 7474 7228 7365 6c66   if hasattr(self
+00013ea0: 2e61 782c 2022 7a61 7869 7322 293a 0a20  .ax, "zaxis"):. 
+00013eb0: 2020 2020 2020 2020 2020 2069 6620 7a3a             if z:
+00013ec0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00013ed0: 2069 6620 6973 696e 7374 616e 6365 287a   if isinstance(z
+00013ee0: 2c20 286c 6973 742c 2074 7570 6c65 2929  , (list, tuple))
+00013ef0: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00013f00: 2020 2020 2020 7a20 3d20 6469 6374 286d        z = dict(m
+00013f10: 616a 6f72 3d64 6963 7428 6c6f 6373 3d7a  ajor=dict(locs=z
+00013f20: 2929 0a0a 2020 2020 2020 2020 2020 2020  ))..            
+00013f30: 2020 2020 6966 207a 2e67 6574 2822 6d61      if z.get("ma
+00013f40: 6a6f 7222 2920 6973 206e 6f74 204e 6f6e  jor") is not Non
+00013f50: 653a 0a20 2020 2020 2020 2020 2020 2020  e:.             
+00013f60: 2020 2020 2020 2073 6574 5f74 6963 6b73         set_ticks
+00013f70: 5f61 6e64 5f6c 6162 656c 7328 0a20 2020  _and_labels(.   
+00013f80: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013f90: 2020 2020 2061 7869 733d 227a 222c 206d       axis="z", m
+00013fa0: 696e 6f72 3d46 616c 7365 2c20 6178 6973  inor=False, axis
+00013fb0: 5f63 6667 3d7a 5b22 6d61 6a6f 7222 5d0a  _cfg=z["major"].
+00013fc0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00013fd0: 2020 2020 290a 0a20 2020 2020 2020 2020      )..         
+00013fe0: 2020 2020 2020 2069 6620 7a2e 6765 7428         if z.get(
+00013ff0: 226d 696e 6f72 2229 2069 7320 6e6f 7420  "minor") is not 
+00014000: 4e6f 6e65 3a0a 2020 2020 2020 2020 2020  None:.          
+00014010: 2020 2020 2020 2020 2020 7365 745f 7469            set_ti
+00014020: 636b 735f 616e 645f 6c61 6265 6c73 280a  cks_and_labels(.
+00014030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014040: 2020 2020 2020 2020 6178 6973 3d22 7a22          axis="z"
+00014050: 2c20 6d69 6e6f 723d 5472 7565 2c20 6178  , minor=True, ax
+00014060: 6973 5f63 6667 3d7a 5b22 6d69 6e6f 7222  is_cfg=z["minor"
+00014070: 5d0a 2020 2020 2020 2020 2020 2020 2020  ].              
+00014080: 2020 2020 2020 290a 0a20 2020 2064 6566        )..    def
+00014090: 205f 686c 7072 5f73 6574 5f74 6963 6b5f   _hlpr_set_tick_
+000140a0: 6c6f 6361 746f 7273 280a 2020 2020 2020  locators(.      
+000140b0: 2020 7365 6c66 2c20 2a2c 2078 3a20 6469    self, *, x: di
+000140c0: 6374 203d 204e 6f6e 652c 2079 3a20 6469  ct = None, y: di
+000140d0: 6374 203d 204e 6f6e 652c 207a 3a20 6469  ct = None, z: di
+000140e0: 6374 203d 204e 6f6e 650a 2020 2020 293a  ct = None.    ):
+000140f0: 0a20 2020 2020 2020 2022 2222 5365 7473  .        """Sets
+00014100: 2074 6865 2074 6963 6b20 6c6f 6361 746f   the tick locato
+00014110: 7273 2066 6f72 2074 6865 2063 7572 7265  rs for the curre
+00014120: 6e74 2061 7869 730a 0a20 2020 2020 2020  nt axis..       
+00014130: 2054 6865 2061 7267 756d 656e 7473 2061   The arguments a
+00014140: 7265 2075 7365 6420 746f 2063 616c 6c0a  re used to call.
+00014150: 2020 2020 2020 2020 6060 6178 2e7b 782c          ``ax.{x,
+00014160: 792c 207a 7d61 7869 732e 7365 745f 7b6d  y, z}axis.set_{m
+00014170: 616a 6f72 2f6d 696e 6f72 7d5f 6c6f 6361  ajor/minor}_loca
+00014180: 746f 7260 602c 2072 6573 7065 6374 6976  tor``, respectiv
+00014190: 656c 792e 0a20 2020 2020 2020 2054 6865  ely..        The
+000141a0: 2064 6963 742d 6c69 6b65 2061 7267 756d   dict-like argum
+000141b0: 656e 7473 206d 7573 7420 636f 6e74 6169  ents must contai
+000141c0: 6e20 7468 6520 6b65 7973 2060 606d 616a  n the keys ``maj
+000141d0: 6f72 6060 2061 6e64 2f6f 720a 2020 2020  or`` and/or.    
+000141e0: 2020 2020 6060 6d69 6e6f 7260 602c 2072      ``minor``, r
+000141f0: 6566 6572 7269 6e67 2074 6f20 6d61 6a6f  eferring to majo
+00014200: 7220 6f72 206d 696e 6f72 2074 6963 6b20  r or minor tick 
+00014210: 6c6f 6361 746f 7273 2e20 5468 6573 6520  locators. These 
+00014220: 6e65 6564 2074 6f0a 2020 2020 2020 2020  need to.        
+00014230: 7370 6563 6966 7920 6120 6e61 6d65 2074  specify a name t
+00014240: 6861 7420 6973 206c 6f6f 6b65 6420 7570  hat is looked up
+00014250: 2069 6e20 3a70 793a 6d6f 643a 606d 6174   in :py:mod:`mat
+00014260: 706c 6f74 6c69 622e 7469 636b 6572 602e  plotlib.ticker`.
+00014270: 0a20 2020 2020 2020 2054 6865 7920 6361  .        They ca
+00014280: 6e20 636f 6e74 6169 6e20 6120 6c69 7374  n contain a list
+00014290: 2d6c 696b 6520 6060 6172 6773 6060 206b  -like ``args`` k
+000142a0: 6579 776f 7264 2061 7267 756d 656e 7420  eyword argument 
+000142b0: 7468 6174 2064 6566 696e 6573 0a20 2020  that defines.   
+000142c0: 2020 2020 2074 6865 2061 7267 756d 656e       the argumen
+000142d0: 7473 2074 6f20 7061 7373 206f 6e20 6173  ts to pass on as
+000142e0: 2070 6f73 6974 696f 6e61 6c20 6172 6773   positional args
+000142f0: 2074 6f20 7468 6520 6361 6c6c 6564 2066   to the called f
+00014300: 756e 6374 696f 6e2e 0a20 2020 2020 2020  unction..       
+00014310: 2046 7572 7468 6572 206b 7761 7267 7320   Further kwargs 
+00014320: 6172 6520 7061 7373 6564 206f 6e20 746f  are passed on to
+00014330: 0a20 2020 2020 2020 2060 6061 782e 7b78  .        ``ax.{x
+00014340: 2c79 2c20 7a7d 6178 6973 2e73 6574 5f7b  ,y, z}axis.set_{
+00014350: 6d61 6a6f 722f 6d69 6e6f 727d 5f6c 6f63  major/minor}_loc
+00014360: 6174 6f72 6060 2e0a 0a20 2020 2020 2020  ator``...       
+00014370: 2045 7861 6d70 6c65 3a0a 0a20 2020 2020   Example:..     
+00014380: 2020 202e 2e20 636f 6465 2d62 6c6f 636b     .. code-block
+00014390: 3a3a 2079 616d 6c0a 0a20 2020 2020 2020  :: yaml..       
+000143a0: 2020 2020 2073 6574 5f74 6963 6b5f 6c6f       set_tick_lo
+000143b0: 6361 746f 7273 3a0a 2020 2020 2020 2020  cators:.        
+000143c0: 2020 2020 2020 783a 0a20 2020 2020 2020        x:.       
+000143d0: 2020 2020 2020 2020 206d 616a 6f72 3a0a           major:.
+000143e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000143f0: 2020 6e61 6d65 3a20 4d61 784e 4c6f 6361    name: MaxNLoca
+00014400: 746f 7220 2020 2023 206c 6f6f 6b65 6420  tor    # looked 
+00014410: 7570 2066 726f 6d20 6d61 7470 6c6f 746c  up from matplotl
+00014420: 6962 2e74 6963 6b65 720a 2020 2020 2020  ib.ticker.      
+00014430: 2020 2020 2020 2020 2020 2020 6e62 696e              nbin
+00014440: 733a 2036 0a20 2020 2020 2020 2020 2020  s: 6.           
+00014450: 2020 2020 2020 2069 6e74 6567 6572 3a20         integer: 
+00014460: 7472 7565 0a20 2020 2020 2020 2020 2020  true.           
+00014470: 2020 2020 2020 206d 696e 5f6e 5f74 6963         min_n_tic
+00014480: 6b73 3a20 330a 2020 2020 2020 2020 2020  ks: 3.          
+00014490: 2020 2020 793a 0a20 2020 2020 2020 2020      y:.         
+000144a0: 2020 2020 2020 206d 616a 6f72 3a0a 2020         major:.  
+000144b0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000144c0: 6e61 6d65 3a20 4d75 6c74 6970 6c65 4c6f  name: MultipleLo
+000144d0: 6361 746f 720a 2020 2020 2020 2020 2020  cator.          
+000144e0: 2020 2020 2020 2020 6172 6773 3a20 5b32          args: [2
+000144f0: 5d0a 0a0a 2020 2020 2020 2020 466f 7220  ]...        For 
+00014500: 6d6f 7265 2069 6e66 6f72 6d61 7469 6f6e  more information
+00014510: 2c20 7365 653a 0a0a 2020 2020 2020 2020  , see:..        
+00014520: 2020 2020 2d20 6874 7470 733a 2f2f 6d61      - https://ma
+00014530: 7470 6c6f 746c 6962 2e6f 7267 2f67 616c  tplotlib.org/gal
+00014540: 6c65 7279 2f74 6963 6b73 5f61 6e64 5f73  lery/ticks_and_s
+00014550: 7069 6e65 732f 7469 636b 2d6c 6f63 6174  pines/tick-locat
+00014560: 6f72 732e 6874 6d6c 0a20 2020 2020 2020  ors.html.       
+00014570: 2020 2020 202d 2068 7474 7073 3a2f 2f6d       - https://m
+00014580: 6174 706c 6f74 6c69 622e 6f72 672f 6170  atplotlib.org/ap
+00014590: 692f 5f61 735f 6765 6e2f 6d61 7470 6c6f  i/_as_gen/matplo
+000145a0: 746c 6962 2e61 7869 732e 4178 6973 2e73  tlib.axis.Axis.s
+000145b0: 6574 5f6d 616a 6f72 5f6c 6f63 6174 6f72  et_major_locator
+000145c0: 2e68 746d 6c0a 2020 2020 2020 2020 2020  .html.          
+000145d0: 2020 2d20 6874 7470 733a 2f2f 6d61 7470    - https://matp
+000145e0: 6c6f 746c 6962 2e6f 7267 2f61 7069 2f5f  lotlib.org/api/_
+000145f0: 6173 5f67 656e 2f6d 6174 706c 6f74 6c69  as_gen/matplotli
+00014600: 622e 6178 6973 2e41 7869 732e 7365 745f  b.axis.Axis.set_
+00014610: 6d69 6e6f 725f 6c6f 6361 746f 722e 6874  minor_locator.ht
+00014620: 6d6c 0a0a 2020 2020 2020 2020 4172 6773  ml..        Args
+00014630: 3a0a 2020 2020 2020 2020 2020 2020 7820  :.            x 
+00014640: 2864 6963 742c 206f 7074 696f 6e61 6c29  (dict, optional)
+00014650: 3a20 5468 6520 636f 6e66 6967 7572 6174  : The configurat
+00014660: 696f 6e20 6f66 2074 6865 2078 2d61 7869  ion of the x-axi
+00014670: 7320 7469 636b 206c 6f63 6174 6f72 0a20  s tick locator. 
+00014680: 2020 2020 2020 2020 2020 2079 2028 6469             y (di
+00014690: 6374 2c20 6f70 7469 6f6e 616c 293a 2054  ct, optional): T
+000146a0: 6865 2063 6f6e 6669 6775 7261 7469 6f6e  he configuration
+000146b0: 206f 6620 7468 6520 792d 6178 6973 2074   of the y-axis t
+000146c0: 6963 6b20 6c6f 6361 746f 720a 2020 2020  ick locator.    
+000146d0: 2020 2020 2020 2020 7a20 2864 6963 742c          z (dict,
+000146e0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+000146f0: 636f 6e66 6967 7572 6174 696f 6e20 6f66  configuration of
+00014700: 2074 6865 207a 2d61 7869 7320 7469 636b   the z-axis tick
+00014710: 206c 6f63 6174 6f72 2e0a 2020 2020 2020   locator..      
+00014720: 2020 2020 2020 2020 2020 4966 2074 6865            If the
+00014730: 7265 2069 7320 6e6f 207a 2d61 7869 732c  re is no z-axis,
+00014740: 2074 6869 7320 7769 6c6c 2062 6520 7369   this will be si
+00014750: 6c65 6e74 6c79 2069 676e 6f72 6564 2e0a  lently ignored..
+00014760: 2020 2020 2020 2020 2222 220a 2020 2020          """.    
+00014770: 2020 2020 7365 745f 7469 636b 5f6c 6f63      set_tick_loc
+00014780: 6174 6f72 735f 6f72 5f66 6f72 6d61 7474  ators_or_formatt
+00014790: 6572 7328 0a20 2020 2020 2020 2020 2020  ers(.           
+000147a0: 2061 783d 7365 6c66 2e61 782c 206b 696e   ax=self.ax, kin
+000147b0: 643d 226c 6f63 6174 6f72 222c 2078 3d78  d="locator", x=x
+000147c0: 2c20 793d 792c 207a 3d7a 0a20 2020 2020  , y=y, z=z.     
+000147d0: 2020 2029 0a0a 2020 2020 6465 6620 5f68     )..    def _h
+000147e0: 6c70 725f 7365 745f 7469 636b 5f66 6f72  lpr_set_tick_for
+000147f0: 6d61 7474 6572 7328 0a20 2020 2020 2020  matters(.       
+00014800: 2073 656c 662c 202a 2c20 783a 2064 6963   self, *, x: dic
+00014810: 7420 3d20 4e6f 6e65 2c20 793a 2064 6963  t = None, y: dic
+00014820: 7420 3d20 4e6f 6e65 2c20 7a3a 2064 6963  t = None, z: dic
+00014830: 7420 3d20 4e6f 6e65 0a20 2020 2029 3a0a  t = None.    ):.
+00014840: 2020 2020 2020 2020 2222 2253 6574 7320          """Sets 
+00014850: 7468 6520 7469 636b 2066 6f72 6d61 7474  the tick formatt
+00014860: 6572 7320 666f 7220 7468 6520 6375 7272  ers for the curr
+00014870: 656e 7420 6178 6973 0a0a 2020 2020 2020  ent axis..      
+00014880: 2020 5468 6520 6172 6775 6d65 6e74 7320    The arguments 
+00014890: 6172 6520 7573 6564 2074 6f20 6361 6c6c  are used to call
+000148a0: 0a20 2020 2020 2020 2060 6061 782e 7b78  .        ``ax.{x
+000148b0: 2c79 2c20 7a7d 6178 6973 2e73 6574 5f7b  ,y, z}axis.set_{
+000148c0: 6d61 6a6f 722f 6d69 6e6f 727d 5f66 6f72  major/minor}_for
+000148d0: 6d61 7474 6572 6060 2c20 7265 7370 6563  matter``, respec
+000148e0: 7469 7665 6c79 2e20 5468 650a 2020 2020  tively. The.    
+000148f0: 2020 2020 6469 6374 2d6c 696b 6520 6172      dict-like ar
+00014900: 6775 6d65 6e74 7320 6d75 7374 2063 6f6e  guments must con
+00014910: 7461 696e 2074 6865 206b 6579 7320 6060  tain the keys ``
+00014920: 6d61 6a6f 7260 6020 616e 642f 6f72 2060  major`` and/or `
+00014930: 606d 696e 6f72 6060 2c0a 2020 2020 2020  `minor``,.      
+00014940: 2020 7265 6665 7272 696e 6720 746f 206d    referring to m
+00014950: 616a 6f72 206f 7220 6d69 6e6f 7220 7469  ajor or minor ti
+00014960: 636b 2066 6f72 6d61 7474 6572 732e 2054  ck formatters. T
+00014970: 6865 7365 206e 6565 6420 746f 2073 7065  hese need to spe
+00014980: 6369 6679 2061 0a20 2020 2020 2020 206e  cify a.        n
+00014990: 616d 6520 7468 6174 2069 7320 6c6f 6f6b  ame that is look
+000149a0: 6564 2075 7020 696e 203a 7079 3a6d 6f64  ed up in :py:mod
+000149b0: 3a60 6d61 7470 6c6f 746c 6962 2e74 6963  :`matplotlib.tic
+000149c0: 6b65 7260 2e0a 2020 2020 2020 2020 5468  ker`..        Th
+000149d0: 6579 2063 616e 2063 6f6e 7461 696e 2061  ey can contain a
+000149e0: 206c 6973 742d 6c69 6b65 2060 6061 7267   list-like ``arg
+000149f0: 7360 6020 6b65 7977 6f72 6420 6172 6775  s`` keyword argu
+00014a00: 6d65 6e74 2074 6861 7420 6465 6669 6e65  ment that define
+00014a10: 730a 2020 2020 2020 2020 7468 6520 6172  s.        the ar
+00014a20: 6775 6d65 6e74 7320 746f 2070 6173 7320  guments to pass 
+00014a30: 6f6e 2061 7320 706f 7369 7469 6f6e 616c  on as positional
+00014a40: 2061 7267 7320 746f 2074 6865 2063 616c   args to the cal
+00014a50: 6c65 6420 6675 6e63 7469 6f6e 2e0a 2020  led function..  
+00014a60: 2020 2020 2020 4675 7274 6865 7220 6b77        Further kw
+00014a70: 6172 6773 2061 7265 2070 6173 7365 6420  args are passed 
+00014a80: 6f6e 2074 6f0a 2020 2020 2020 2020 6060  on to.        ``
+00014a90: 6178 2e7b 782c 792c 207a 7d61 7869 732e  ax.{x,y, z}axis.
+00014aa0: 7365 745f 7b6d 616a 6f72 2f6d 696e 6f72  set_{major/minor
+00014ab0: 7d5f 666f 726d 6174 7465 7260 602e 0a0a  }_formatter``...
+00014ac0: 2020 2020 2020 2020 4578 616d 706c 653a          Example:
+00014ad0: 0a0a 2020 2020 2020 2020 2e2e 2063 6f64  ..        .. cod
+00014ae0: 652d 626c 6f63 6b3a 3a20 7961 6d6c 0a0a  e-block:: yaml..
+00014af0: 2020 2020 2020 2020 2020 2020 7365 745f              set_
+00014b00: 7469 636b 5f66 6f72 6d61 7474 6572 733a  tick_formatters:
+00014b10: 0a20 2020 2020 2020 2020 2020 2020 2078  .              x
+00014b20: 3a0a 2020 2020 2020 2020 2020 2020 2020  :.              
+00014b30: 2020 6d61 6a6f 723a 0a20 2020 2020 2020    major:.       
+00014b40: 2020 2020 2020 2020 2020 206e 616d 653a             name:
+00014b50: 2053 7472 4d65 7468 6f64 466f 726d 6174   StrMethodFormat
+00014b60: 7465 720a 2020 2020 2020 2020 2020 2020  ter.            
+00014b70: 2020 2020 2020 6172 6773 3a20 5b27 7b78        args: ['{x
+00014b80: 3a2e 3367 7d27 5d0a 2020 2020 2020 2020  :.3g}'].        
+00014b90: 2020 2020 2020 793a 0a20 2020 2020 2020        y:.       
+00014ba0: 2020 2020 2020 2020 206d 616a 6f72 3a0a           major:.
+00014bb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014bc0: 2020 6e61 6d65 3a20 4675 6e63 466f 726d    name: FuncForm
+00014bd0: 6174 7465 720a 2020 2020 2020 2020 2020  atter.          
+00014be0: 2020 2020 2020 2020 6172 6773 3a20 5b21          args: [!
+00014bf0: 6461 675f 7265 7375 6c74 206d 795f 666f  dag_result my_fo
+00014c00: 726d 6174 7465 725f 6c61 6d62 6461 5d0a  rmatter_lambda].
+00014c10: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00014c20: 2020 2320 616e 7920 6b77 6172 6773 2068    # any kwargs h
+00014c30: 6572 6520 7061 7373 6564 2061 6c73 6f20  ere passed also 
+00014c40: 746f 2046 756e 6346 6f72 6d61 7474 6572  to FuncFormatter
+00014c50: 0a0a 2020 2020 2020 2020 2020 2020 2020  ..              
+00014c60: 7a3a 0a20 2020 2020 2020 2020 2020 2020  z:.             
+00014c70: 2020 206d 616a 6f72 3a0a 2020 2020 2020     major:.      
+00014c80: 2020 2020 2020 2020 2020 2020 6e61 6d65              name
+00014c90: 3a20 4461 7465 466f 726d 6174 7465 7220  : DateFormatter 
+00014ca0: 2023 206c 6f6f 6b65 6420 7570 2066 726f   # looked up fro
+00014cb0: 6d20 6d61 7470 6c6f 746c 6962 2e64 6174  m matplotlib.dat
+00014cc0: 6573 0a20 2020 2020 2020 2020 2020 2020  es.             
+00014cd0: 2020 2020 2061 7267 733a 205b 2225 483a       args: ["%H:
+00014ce0: 254d 3a25 5322 5d20 2023 206f 7220 2225  %M:%S"]  # or "%
+00014cf0: 592d 256d 2d25 6422 0a0a 2020 2020 2020  Y-%m-%d"..      
+00014d00: 2020 466f 7220 6d6f 7265 2069 6e66 6f72    For more infor
+00014d10: 6d61 7469 6f6e 2c20 7365 653a 0a0a 2020  mation, see:..  
+00014d20: 2020 2020 2020 2020 2020 2d20 6874 7470            - http
+00014d30: 733a 2f2f 6d61 7470 6c6f 746c 6962 2e6f  s://matplotlib.o
+00014d40: 7267 2f67 616c 6c65 7279 2f74 6963 6b73  rg/gallery/ticks
+00014d50: 5f61 6e64 5f73 7069 6e65 732f 7469 636b  _and_spines/tick
+00014d60: 2d66 6f72 6d61 7474 6572 732e 6874 6d6c  -formatters.html
+00014d70: 0a20 2020 2020 2020 2020 2020 202d 2068  .            - h
+00014d80: 7474 7073 3a2f 2f6d 6174 706c 6f74 6c69  ttps://matplotli
+00014d90: 622e 6f72 672f 6170 692f 5f61 735f 6765  b.org/api/_as_ge
+00014da0: 6e2f 6d61 7470 6c6f 746c 6962 2e61 7869  n/matplotlib.axi
+00014db0: 732e 4178 6973 2e73 6574 5f6d 616a 6f72  s.Axis.set_major
+00014dc0: 5f66 6f72 6d61 7474 6572 2e68 746d 6c0a  _formatter.html.
+00014dd0: 2020 2020 2020 2020 2020 2020 2d20 6874              - ht
+00014de0: 7470 733a 2f2f 6d61 7470 6c6f 746c 6962  tps://matplotlib
+00014df0: 2e6f 7267 2f61 7069 2f5f 6173 5f67 656e  .org/api/_as_gen
+00014e00: 2f6d 6174 706c 6f74 6c69 622e 6178 6973  /matplotlib.axis
+00014e10: 2e41 7869 732e 7365 745f 6d69 6e6f 725f  .Axis.set_minor_
+00014e20: 666f 726d 6174 7465 722e 6874 6d6c 0a0a  formatter.html..
+00014e30: 2020 2020 2020 2020 4172 6773 3a0a 2020          Args:.  
+00014e40: 2020 2020 2020 2020 2020 7820 2864 6963            x (dic
+00014e50: 742c 206f 7074 696f 6e61 6c29 3a20 5468  t, optional): Th
+00014e60: 6520 636f 6e66 6967 7572 6174 696f 6e20  e configuration 
+00014e70: 6f66 2074 6865 2078 2d61 7869 7320 7469  of the x-axis ti
+00014e80: 636b 2066 6f72 6d61 7474 6572 0a20 2020  ck formatter.   
+00014e90: 2020 2020 2020 2020 2079 2028 6469 6374           y (dict
+00014ea0: 2c20 6f70 7469 6f6e 616c 293a 2054 6865  , optional): The
+00014eb0: 2063 6f6e 6669 6775 7261 7469 6f6e 206f   configuration o
+00014ec0: 6620 7468 6520 792d 6178 6973 2074 6963  f the y-axis tic
+00014ed0: 6b20 666f 726d 6174 7465 720a 2020 2020  k formatter.    
+00014ee0: 2020 2020 2020 2020 7a20 2864 6963 742c          z (dict,
+00014ef0: 206f 7074 696f 6e61 6c29 3a20 5468 6520   optional): The 
+00014f00: 636f 6e66 6967 7572 6174 696f 6e20 6f66  configuration of
+00014f10: 2074 6865 207a 2d61 7869 7320 7469 636b   the z-axis tick
+00014f20: 2066 6f72 6d61 7474 6572 2e0a 2020 2020   formatter..    
+00014f30: 2020 2020 2020 2020 2020 2020 4966 2074              If t
+00014f40: 6865 7265 2069 7320 6e6f 207a 2d61 7869  here is no z-axi
+00014f50: 732c 2074 6869 7320 7769 6c6c 2062 6520  s, this will be 
+00014f60: 7369 6c65 6e74 6c79 2069 676e 6f72 6564  silently ignored
+00014f70: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
+00014f80: 2020 2020 2020 7365 745f 7469 636b 5f6c        set_tick_l
+00014f90: 6f63 6174 6f72 735f 6f72 5f66 6f72 6d61  ocators_or_forma
+00014fa0: 7474 6572 7328 0a20 2020 2020 2020 2020  tters(.         
+00014fb0: 2020 2061 783d 7365 6c66 2e61 782c 206b     ax=self.ax, k
+00014fc0: 696e 643d 2266 6f72 6d61 7474 6572 222c  ind="formatter",
+00014fd0: 2078 3d78 2c20 793d 792c 207a 3d7a 0a20   x=x, y=y, z=z. 
+00014fe0: 2020 2020 2020 2029 0a0a 2020 2020 6465         )..    de
+00014ff0: 6620 5f68 6c70 725f 6361 6c6c 280a 2020  f _hlpr_call(.  
+00015000: 2020 2020 2020 7365 6c66 2c0a 2020 2020        self,.    
+00015010: 2020 2020 2a2c 0a20 2020 2020 2020 2066      *,.        f
+00015020: 756e 6374 696f 6e73 3a20 5365 7175 656e  unctions: Sequen
+00015030: 6365 5b64 6963 745d 2c0a 2020 2020 2020  ce[dict],.      
+00015040: 2020 6675 6e63 735f 6c6f 6f6b 7570 5f64    funcs_lookup_d
+00015050: 6963 743a 2044 6963 745b 7374 722c 2043  ict: Dict[str, C
+00015060: 616c 6c61 626c 655d 203d 204e 6f6e 652c  allable] = None,
+00015070: 0a20 2020 2020 2020 202a 2a73 6861 7265  .        **share
+00015080: 645f 6b77 6172 6773 2c0a 2020 2020 293a  d_kwargs,.    ):
+00015090: 0a20 2020 2020 2020 2022 2222 4178 6973  .        """Axis
+000150a0: 2d6c 6576 656c 2068 656c 7065 7220 7468  -level helper th
+000150b0: 6174 2063 616e 2062 6520 7573 6564 2074  at can be used t
+000150c0: 6f20 6361 6c6c 206d 756c 7469 706c 6520  o call multiple 
+000150d0: 6675 6e63 7469 6f6e 732e 0a0a 2020 2020  functions...    
+000150e0: 2020 2020 4675 6e63 7469 6f6e 7320 6361      Functions ca
+000150f0: 6e20 6265 2073 7065 6369 6669 6564 2069  n be specified i
+00015100: 6e20 7468 7265 6520 7761 7973 3a0a 0a20  n three ways:.. 
+00015110: 2020 2020 2020 2020 2020 202d 2061 7320             - as 
+00015120: 7374 7269 6e67 2c20 6265 696e 6720 6c6f  string, being lo
+00015130: 6f6b 6564 2075 7020 6672 6f6d 2061 2070  oked up from a p
+00015140: 7265 2d64 6566 696e 6564 2064 6963 740a  re-defined dict.
+00015150: 2020 2020 2020 2020 2020 2020 2d20 6173              - as
+00015160: 2032 2d74 7570 6c65 2060 6028 6d6f 6475   2-tuple ``(modu
+00015170: 6c65 2c20 6e61 6d65 2960 6020 7768 6963  le, name)`` whic
+00015180: 6820 7769 6c6c 2062 6520 696d 706f 7274  h will be import
+00015190: 6564 206f 6e20 7468 6520 666c 790a 2020  ed on the fly.  
+000151a0: 2020 2020 2020 2020 2020 2d20 6173 2063            - as c
+000151b0: 616c 6c61 626c 652c 2077 6869 6368 2077  allable, which w
+000151c0: 696c 6c20 6265 2075 7365 6420 6469 7265  ill be used dire
+000151d0: 6374 6c79 0a0a 2020 2020 2020 2020 5468  ctly..        Th
+000151e0: 6520 696d 706c 656d 656e 7461 7469 6f6e  e implementation
+000151f0: 206f 6620 7468 6973 2069 7320 7368 6172   of this is shar
+00015200: 6564 2077 6974 6820 7468 6520 706c 6f74  ed with the plot
+00015210: 2066 756e 6374 696f 6e0a 2020 2020 2020   function.      
+00015220: 2020 3a70 793a 6675 6e63 3a60 7e64 616e    :py:func:`~dan
+00015230: 7472 6f2e 706c 6f74 2e66 756e 6373 2e6d  tro.plot.funcs.m
+00015240: 756c 7469 706c 6f74 2e6d 756c 7469 706c  ultiplot.multipl
+00015250: 6f74 602e 2053 6565 0a20 2020 2020 2020  ot`. See.       
+00015260: 2074 6865 7265 2066 6f72 206d 6f72 6520   there for more 
+00015270: 696e 666f 726d 6174 696f 6e2e 0a0a 2020  information...  
+00015280: 2020 2020 2020 5468 6520 6669 6775 7265        The figure
+00015290: 2d6c 6576 656c 2068 656c 7065 7220 6060  -level helper ``
+000152a0: 6669 6763 616c 6c60 6020 6973 2069 6465  figcall`` is ide
+000152b0: 6e74 6963 616c 2074 6f20 7468 6973 2068  ntical to this h
+000152c0: 656c 7065 722c 2062 7574 2069 730a 2020  elper, but is.  
+000152d0: 2020 2020 2020 696e 766f 6b65 6420 2a62        invoked *b
+000152e0: 6566 6f72 652a 2074 6865 2061 7869 732d  efore* the axis-
+000152f0: 7370 6563 6966 6963 2068 656c 7065 7273  specific helpers
+00015300: 2061 7265 2069 6e76 6f6b 6564 2e0a 0a20   are invoked... 
+00015310: 2020 2020 2020 202e 2e20 6869 6e74 3a3a         .. hint::
+00015320: 0a0a 2020 2020 2020 2020 2020 2020 546f  ..            To
+00015330: 2070 6173 7320 6375 7374 6f6d 2063 616c   pass custom cal
+00015340: 6c61 626c 6573 2c20 7573 6520 7468 6520  lables, use the 
+00015350: 6461 7461 2074 7261 6e73 666f 726d 6174  data transformat
+00015360: 696f 6e20 6672 616d 6577 6f72 6b20 616e  ion framework an
+00015370: 640a 2020 2020 2020 2020 2020 2020 7468  d.            th
+00015380: 6520 6060 2164 6167 5f72 6573 756c 7460  e ``!dag_result`
+00015390: 6020 706c 6163 6568 6f6c 6465 722c 2073  ` placeholder, s
+000153a0: 6565 203a 7265 663a 6064 6167 5f72 6573  ee :ref:`dag_res
+000153b0: 756c 745f 706c 6163 6568 6f6c 6465 7260  ult_placeholder`
+000153c0: 2e0a 0a20 2020 2020 2020 202e 2e20 6e6f  ...        .. no
+000153d0: 7465 3a3a 0a0a 2020 2020 2020 2020 2020  te::..          
+000153e0: 2020 5768 696c 6520 6d6f 7374 206d 6174    While most mat
+000153f0: 706c 6f74 6c69 622d 6261 7365 6420 6675  plotlib-based fu
+00015400: 6e63 7469 6f6e 7320 7769 6c6c 2061 7574  nctions will aut
+00015410: 6f6d 6174 6963 616c 6c79 206f 7065 7261  omatically opera
+00015420: 7465 206f 6e0a 2020 2020 2020 2020 2020  te on.          
+00015430: 2020 7468 6520 6375 7272 656e 7420 6178    the current ax
+00015440: 6973 2c20 736f 6d65 2066 756e 6374 696f  is, some functio
+00015450: 6e20 6361 6c6c 7320 6d61 7920 7265 7175  n calls may requ
+00015460: 6972 6520 616e 2061 7869 7320 6f62 6a65  ire an axis obje
+00015470: 6374 2e0a 2020 2020 2020 2020 2020 2020  ct..            
+00015480: 4966 2073 6f2c 2075 7365 2074 6865 2060  If so, use the `
+00015490: 6070 6173 735f 6178 6973 5f6f 626a 6563  `pass_axis_objec
+000154a0: 745f 6173 6060 2061 7267 756d 656e 742c  t_as`` argument,
+000154b0: 2077 6869 6368 2073 7065 6369 6669 6573   which specifies
+000154c0: 0a20 2020 2020 2020 2020 2020 2074 6865  .            the
+000154d0: 206e 616d 6520 6f66 2074 6865 206b 6579   name of the key
+000154e0: 776f 7264 2061 7267 756d 656e 7420 6173  word argument as
+000154f0: 2077 6869 6368 2074 6865 2063 7572 7265   which the curre
+00015500: 6e74 2061 7869 7320 6973 0a20 2020 2020  nt axis is.     
+00015510: 2020 2020 2020 2070 6173 7365 6420 746f         passed to
+00015520: 2074 6865 2066 756e 6374 696f 6e20 6361   the function ca
+00015530: 6c6c 2e0a 0a20 2020 2020 2020 2045 7861  ll...        Exa
+00015540: 6d70 6c65 3a0a 0a20 2020 2020 2020 202e  mple:..        .
+00015550: 2e20 636f 6465 2d62 6c6f 636b 3a3a 2079  . code-block:: y
+00015560: 616d 6c0a 0a20 2020 2020 2020 2020 2020  aml..           
+00015570: 2063 616c 6c3a 0a20 2020 2020 2020 2020   call:.         
+00015580: 2020 2020 2066 756e 6374 696f 6e73 3a0a       functions:.
+00015590: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000155a0: 2320 4c6f 6f6b 2075 7020 6675 6e63 7469  # Look up functi
+000155b0: 6f6e 2066 726f 6d20 6469 6374 2c20 636f  on from dict, co
+000155c0: 6e74 6169 6e69 6e67 2063 6f6d 6d6f 6e20  ntaining common 
+000155d0: 7365 6162 6f72 6e20 616e 640a 2020 2020  seaborn and.    
+000155e0: 2020 2020 2020 2020 2020 2020 2320 7079              # py
+000155f0: 706c 6f74 2070 6c6f 7474 696e 6720 6675  plot plotting fu
+00015600: 6e63 7469 6f6e 7320 2873 6565 206d 756c  nctions (see mul
+00015610: 7469 706c 6f74 2066 6f72 206d 6f72 6520  tiplot for more 
+00015620: 696e 666f 290a 2020 2020 2020 2020 2020  info).          
+00015630: 2020 2020 2020 2d20 6675 6e63 7469 6f6e        - function
+00015640: 3a20 736e 732e 6c69 6e65 706c 6f74 0a20  : sns.lineplot. 
+00015650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015660: 2064 6174 613a 2021 6461 675f 7265 7375   data: !dag_resu
+00015670: 6c74 206d 795f 6375 7374 6f6d 5f64 6174  lt my_custom_dat
+00015680: 610a 0a20 2020 2020 2020 2020 2020 2020  a..             
+00015690: 2020 2023 2049 6d70 6f72 7420 6675 6e63     # Import func
+000156a0: 7469 6f6e 2076 6961 2060 286d 6f64 756c  tion via `(modul
+000156b0: 652c 206e 616d 6529 6020 7370 6563 6966  e, name)` specif
+000156c0: 6963 6174 696f 6e0a 2020 2020 2020 2020  ication.        
+000156d0: 2020 2020 2020 2020 2d20 6675 6e63 7469          - functi
+000156e0: 6f6e 3a20 5b6d 6174 706c 6f74 6c69 622c  on: [matplotlib,
+000156f0: 2070 7970 6c6f 742e 7375 6270 6c6f 7473   pyplot.subplots
+00015700: 5f61 646a 7573 745d 0a20 2020 2020 2020  _adjust].       
+00015710: 2020 2020 2020 2020 2020 206c 6566 743a             left:
+00015720: 2030 2e31 0a20 2020 2020 2020 2020 2020   0.1.           
+00015730: 2020 2020 2020 2072 6967 6874 3a20 302e         right: 0.
+00015740: 390a 0a20 2020 2020 2020 2020 2020 2020  9..             
+00015750: 2020 2023 2050 6173 7320 6120 6375 7374     # Pass a cust
+00015760: 6f6d 2063 616c 6c61 626c 652c 2073 656c  om callable, sel
+00015770: 6563 7465 6420 7669 6120 4441 4720 6672  ected via DAG fr
+00015780: 616d 6577 6f72 6b0a 2020 2020 2020 2020  amework.        
+00015790: 2020 2020 2020 2020 2d20 6675 6e63 7469          - functi
+000157a0: 6f6e 3a20 2164 6167 5f72 6573 756c 7420  on: !dag_result 
+000157b0: 6d79 5f63 616c 6c61 626c 650a 2020 2020  my_callable.    
+000157c0: 2020 2020 2020 2020 2020 2020 2020 6172                ar
+000157d0: 6773 3a20 5b66 6f6f 2c20 6261 725d 0a20  gs: [foo, bar]. 
+000157e0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000157f0: 2023 202e 2e2e 206b 6579 776f 7264 2061   # ... keyword a
+00015800: 7267 756d 656e 7473 2068 6572 650a 0a20  rguments here.. 
+00015810: 2020 2020 2020 2020 2020 2020 2020 2023                 #
+00015820: 2050 6173 7320 6375 7272 656e 7420 6178   Pass current ax
+00015830: 6973 206f 626a 6563 7420 6173 206b 6579  is object as key
+00015840: 776f 7264 2061 7267 756d 656e 740a 2020  word argument.  
+00015850: 2020 2020 2020 2020 2020 2020 2020 2d20                - 
+00015860: 6675 6e63 7469 6f6e 3a20 2164 6167 5f72  function: !dag_r
+00015870: 6573 756c 7420 6d79 5f63 616c 6c61 626c  esult my_callabl
+00015880: 655f 6f70 6572 6174 696e 675f 6f6e 5f61  e_operating_on_a
+00015890: 780a 2020 2020 2020 2020 2020 2020 2020  x.              
+000158a0: 2020 2020 7061 7373 5f61 7869 735f 6f62      pass_axis_ob
+000158b0: 6a65 6374 5f61 733a 2061 780a 0a20 2020  ject_as: ax..   
+000158c0: 2020 2020 2020 2020 2020 2020 2023 2050               # P
+000158d0: 6173 7320 6865 6c70 6572 206f 626a 6563  ass helper objec
+000158e0: 7420 6974 7365 6c66 2061 7320 6b65 7977  t itself as keyw
+000158f0: 6f72 6420 6172 6775 6d65 6e74 0a20 2020  ord argument.   
+00015900: 2020 2020 2020 2020 2020 2020 202d 2066               - f
+00015910: 756e 6374 696f 6e3a 2021 6461 675f 7265  unction: !dag_re
+00015920: 7375 6c74 206d 795f 6361 6c6c 6162 6c65  sult my_callable
+00015930: 5f6f 7065 7261 7469 6e67 5f6f 6e5f 6865  _operating_on_he
+00015940: 6c70 6572 0a20 2020 2020 2020 2020 2020  lper.           
+00015950: 2020 2020 2020 2070 6173 735f 6865 6c70         pass_help
+00015960: 6572 3a20 7472 7565 0a0a 2020 2020 2020  er: true..      
+00015970: 2020 4172 6773 3a0a 2020 2020 2020 2020    Args:.        
+00015980: 2020 2020 6675 6e63 7469 6f6e 7320 2853      functions (S
+00015990: 6571 7565 6e63 655b 6469 6374 5d29 3a20  equence[dict]): 
+000159a0: 4120 7365 7175 656e 6365 206f 6620 6675  A sequence of fu
+000159b0: 6e63 7469 6f6e 2063 616c 6c0a 2020 2020  nction call.    
+000159c0: 2020 2020 2020 2020 2020 2020 7370 6563              spec
+000159d0: 6966 6963 6174 696f 6e73 2e20 4561 6368  ifications. Each
+000159e0: 2064 6963 7420 6e65 6564 7320 746f 2063   dict needs to c
+000159f0: 6f6e 7461 696e 2061 7420 6c65 6173 7420  ontain at least 
+00015a00: 7468 6520 6b65 790a 2020 2020 2020 2020  the key.        
+00015a10: 2020 2020 2020 2020 6060 6675 6e63 7469          ``functi
+00015a20: 6f6e 6060 2077 6869 6368 2064 6574 6572  on`` which deter
+00015a30: 6d69 6e65 7320 7768 6963 6820 6675 6e63  mines which func
+00015a40: 7469 6f6e 2074 6f20 696e 766f 6b65 2e20  tion to invoke. 
+00015a50: 4675 7274 6865 720a 2020 2020 2020 2020  Further.        
+00015a60: 2020 2020 2020 2020 6172 6775 6d65 6e74          argument
+00015a70: 7320 6172 6520 7061 7273 6564 2069 6e74  s are parsed int
+00015a80: 6f20 7468 6520 706f 7369 7469 6f6e 616c  o the positional
+00015a90: 2061 6e64 206b 6579 776f 7264 2061 7267   and keyword arg
+00015aa0: 756d 656e 7473 0a20 2020 2020 2020 2020  uments.         
+00015ab0: 2020 2020 2020 206f 6620 7468 6520 746f         of the to
+00015ac0: 2d62 652d 696e 766f 6b65 6420 6675 6e63  -be-invoked func
+00015ad0: 7469 6f6e 2e0a 2020 2020 2020 2020 2020  tion..          
+00015ae0: 2020 6675 6e63 735f 6c6f 6f6b 7570 5f64    funcs_lookup_d
+00015af0: 6963 7420 2844 6963 745b 7374 722c 2043  ict (Dict[str, C
+00015b00: 616c 6c61 626c 655d 2c20 6f70 7469 6f6e  allable], option
+00015b10: 616c 293a 2049 6620 6769 7665 6e2c 2077  al): If given, w
+00015b20: 696c 6c0a 2020 2020 2020 2020 2020 2020  ill.            
+00015b30: 2020 2020 6c6f 6f6b 2075 7020 7468 6520      look up the 
+00015b40: 6675 6e63 7469 6f6e 206e 616d 6573 2066  function names f
+00015b50: 726f 6d20 7468 6973 2064 6963 7420 696e  rom this dict in
+00015b60: 7374 6561 6420 6f66 2074 6865 0a20 2020  stead of the.   
+00015b70: 2020 2020 2020 2020 2020 2020 2064 6566               def
+00015b80: 6175 6c74 2064 6963 742e 0a20 2020 2020  ault dict..     
+00015b90: 2020 2020 2020 202a 2a73 6861 7265 645f         **shared_
+00015ba0: 6b77 6172 6773 3a20 5061 7373 6564 206f  kwargs: Passed o
+00015bb0: 6e20 6173 206b 6579 776f 7264 2061 7267  n as keyword arg
+00015bc0: 756d 656e 7473 2074 6f20 2a61 6c6c 2a20  uments to *all* 
+00015bd0: 6675 6e63 7469 6f6e 0a20 2020 2020 2020  function.       
+00015be0: 2020 2020 2020 2020 2063 616c 6c73 2069           calls i
+00015bf0: 6e20 6060 6675 6e63 7469 6f6e 7360 602e  n ``functions``.
+00015c00: 0a20 2020 2020 2020 2022 2222 0a20 2020  .        """.   
+00015c10: 2020 2020 2066 726f 6d20 2e66 756e 6373       from .funcs
+00015c20: 2e5f 6d75 6c74 6970 6c6f 7420 696d 706f  ._multiplot impo
+00015c30: 7274 2070 6172 7365 5f61 6e64 5f69 6e76  rt parse_and_inv
+00015c40: 6f6b 655f 6675 6e63 7469 6f6e 0a0a 2020  oke_function..  
+00015c50: 2020 2020 2020 666f 7220 6361 6c6c 5f6e        for call_n
+00015c60: 756d 2c20 6675 6e63 5f6b 7761 7267 7320  um, func_kwargs 
+00015c70: 696e 2065 6e75 6d65 7261 7465 2866 756e  in enumerate(fun
+00015c80: 6374 696f 6e73 293a 0a20 2020 2020 2020  ctions):.       
+00015c90: 2020 2020 2070 6172 7365 5f61 6e64 5f69       parse_and_i
+00015ca0: 6e76 6f6b 655f 6675 6e63 7469 6f6e 280a  nvoke_function(.
+00015cb0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00015cc0: 686c 7072 3d73 656c 662c 0a20 2020 2020  hlpr=self,.     
+00015cd0: 2020 2020 2020 2020 2020 2066 756e 6373             funcs
+00015ce0: 3d66 756e 6373 5f6c 6f6f 6b75 705f 6469  =funcs_lookup_di
+00015cf0: 6374 2c0a 2020 2020 2020 2020 2020 2020  ct,.            
+00015d00: 2020 2020 7368 6172 6564 5f6b 7761 7267      shared_kwarg
+00015d10: 733d 7368 6172 6564 5f6b 7761 7267 732c  s=shared_kwargs,
+00015d20: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015d30: 2066 756e 635f 6b77 6172 6773 3d66 756e   func_kwargs=fun
+00015d40: 635f 6b77 6172 6773 2c0a 2020 2020 2020  c_kwargs,.      
+00015d50: 2020 2020 2020 2020 2020 7368 6f77 5f68            show_h
+00015d60: 696e 7473 3d46 616c 7365 2c0a 2020 2020  ints=False,.    
+00015d70: 2020 2020 2020 2020 2020 2020 6361 6c6c              call
+00015d80: 5f6e 756d 3d63 616c 6c5f 6e75 6d2c 0a20  _num=call_num,. 
+00015d90: 2020 2020 2020 2020 2020 2029 0a0a 2020             )..  
+00015da0: 2020 2320 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e    # ............
 00015db0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00015dc0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
 00015dd0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00015de0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e  ................
-00015df0: 2e2e 2e2e 0a20 2020 2023 202e 2e2e 2075  .....    # ... u
-00015e00: 7369 6e67 2073 6561 626f 726e 0a0a 2020  sing seaborn..  
-00015e10: 2020 6465 6620 5f68 6c70 725f 6465 7370    def _hlpr_desp
-00015e20: 696e 6528 7365 6c66 2c20 2a2a 6b77 6172  ine(self, **kwar
-00015e30: 6773 293a 0a20 2020 2020 2020 2022 2222  gs):.        """
-00015e40: 4465 7370 696e 6573 2074 6865 2063 7572  Despines the cur
-00015e50: 7265 6e74 202a 6178 6973 2a20 7573 696e  rent *axis* usin
-00015e60: 6720 3a70 793a 6675 6e63 3a60 7365 6162  g :py:func:`seab
-00015e70: 6f72 6e2e 6465 7370 696e 6560 2e0a 0a20  orn.despine`... 
-00015e80: 2020 2020 2020 2054 6f20 6465 7370 696e         To despin
-00015e90: 6520 7468 6520 7768 6f6c 6520 2a66 6967  e the whole *fig
-00015ea0: 7572 652a 2c20 6170 706c 7920 7468 6973  ure*, apply this
-00015eb0: 2068 656c 7065 7220 746f 2061 6c6c 2061   helper to all a
-00015ec0: 7865 732e 0a20 2020 2020 2020 2052 6566  xes..        Ref
-00015ed0: 6572 2074 6f20 7468 6520 7365 6162 6f72  er to the seabor
-00015ee0: 6e20 646f 6375 6d65 6e74 6174 696f 6e20  n documentation 
-00015ef0: 666f 7220 6176 6169 6c61 626c 6520 6172  for available ar
-00015f00: 6775 6d65 6e74 733a 0a20 2020 2020 2020  guments:.       
-00015f10: 2068 7474 7073 3a2f 2f73 6561 626f 726e   https://seaborn
-00015f20: 2e70 7964 6174 612e 6f72 672f 6765 6e65  .pydata.org/gene
-00015f30: 7261 7465 642f 7365 6162 6f72 6e2e 6465  rated/seaborn.de
-00015f40: 7370 696e 652e 6874 6d6c 0a0a 2020 2020  spine.html..    
-00015f50: 2020 2020 4172 6773 3a0a 2020 2020 2020      Args:.      
-00015f60: 2020 2020 2020 2a2a 6b77 6172 6773 3a20        **kwargs: 
-00015f70: 5061 7373 6564 206f 6e20 746f 2060 6073  Passed on to ``s
-00015f80: 6561 626f 726e 2e64 6573 7069 6e65 6060  eaborn.despine``
-00015f90: 2e0a 2020 2020 2020 2020 2222 220a 2020  ..        """.  
-00015fa0: 2020 2020 2020 6966 2022 6669 6722 2069        if "fig" i
-00015fb0: 6e20 6b77 6172 6773 3a0a 2020 2020 2020  n kwargs:.      
-00015fc0: 2020 2020 2020 7261 6973 6520 5661 6c75        raise Valu
-00015fd0: 6545 7272 6f72 280a 2020 2020 2020 2020  eError(.        
-00015fe0: 2020 2020 2020 2020 2247 6f74 2075 6e65          "Got une
-00015ff0: 7870 6563 7465 6420 6066 6967 6020 6172  xpected `fig` ar
-00016000: 6775 6d65 6e74 2120 546f 2061 7070 6c79  gument! To apply
-00016010: 2074 6865 2060 6465 7370 696e 6560 2068   the `despine` h
-00016020: 656c 7065 7220 220a 2020 2020 2020 2020  elper ".        
-00016030: 2020 2020 2020 2020 2274 6f20 616c 6c20          "to all 
-00016040: 6178 6573 2c20 696e 766f 6b65 2074 6865  axes, invoke the
-00016050: 2068 656c 7065 7220 6f6e 2065 6163 6820   helper on each 
-00016060: 6178 6973 2073 6570 6172 6174 656c 792e  axis separately.
-00016070: 220a 2020 2020 2020 2020 2020 2020 290a  ".            ).
-00016080: 2020 2020 2020 2020 736e 732e 6465 7370          sns.desp
-00016090: 696e 6528 6178 3d73 656c 662e 6178 2c20  ine(ax=self.ax, 
-000160a0: 2a2a 6b77 6172 6773 290a                 **kwargs).
+00015de0: 2e2e 2e2e 2e2e 2e2e 2e2e 2e2e 2e0a 2020  ..............  
+00015df0: 2020 2320 2e2e 2e20 7573 696e 6720 7365    # ... using se
+00015e00: 6162 6f72 6e0a 0a20 2020 2064 6566 205f  aborn..    def _
+00015e10: 686c 7072 5f64 6573 7069 6e65 2873 656c  hlpr_despine(sel
+00015e20: 662c 202a 2a6b 7761 7267 7329 3a0a 2020  f, **kwargs):.  
+00015e30: 2020 2020 2020 2222 2244 6573 7069 6e65        """Despine
+00015e40: 7320 7468 6520 6375 7272 656e 7420 2a61  s the current *a
+00015e50: 7869 732a 2075 7369 6e67 203a 7079 3a66  xis* using :py:f
+00015e60: 756e 633a 6073 6561 626f 726e 2e64 6573  unc:`seaborn.des
+00015e70: 7069 6e65 602e 0a0a 2020 2020 2020 2020  pine`...        
+00015e80: 546f 2064 6573 7069 6e65 2074 6865 2077  To despine the w
+00015e90: 686f 6c65 202a 6669 6775 7265 2a2c 2061  hole *figure*, a
+00015ea0: 7070 6c79 2074 6869 7320 6865 6c70 6572  pply this helper
+00015eb0: 2074 6f20 616c 6c20 6178 6573 2e0a 2020   to all axes..  
+00015ec0: 2020 2020 2020 5265 6665 7220 746f 2074        Refer to t
+00015ed0: 6865 2073 6561 626f 726e 2064 6f63 756d  he seaborn docum
+00015ee0: 656e 7461 7469 6f6e 2066 6f72 2061 7661  entation for ava
+00015ef0: 696c 6162 6c65 2061 7267 756d 656e 7473  ilable arguments
+00015f00: 3a0a 2020 2020 2020 2020 6874 7470 733a  :.        https:
+00015f10: 2f2f 7365 6162 6f72 6e2e 7079 6461 7461  //seaborn.pydata
+00015f20: 2e6f 7267 2f67 656e 6572 6174 6564 2f73  .org/generated/s
+00015f30: 6561 626f 726e 2e64 6573 7069 6e65 2e68  eaborn.despine.h
+00015f40: 746d 6c0a 0a20 2020 2020 2020 2041 7267  tml..        Arg
+00015f50: 733a 0a20 2020 2020 2020 2020 2020 202a  s:.            *
+00015f60: 2a6b 7761 7267 733a 2050 6173 7365 6420  *kwargs: Passed 
+00015f70: 6f6e 2074 6f20 6060 7365 6162 6f72 6e2e  on to ``seaborn.
+00015f80: 6465 7370 696e 6560 602e 0a20 2020 2020  despine``..     
+00015f90: 2020 2022 2222 0a20 2020 2020 2020 2069     """.        i
+00015fa0: 6620 2266 6967 2220 696e 206b 7761 7267  f "fig" in kwarg
+00015fb0: 733a 0a20 2020 2020 2020 2020 2020 2072  s:.            r
+00015fc0: 6169 7365 2056 616c 7565 4572 726f 7228  aise ValueError(
+00015fd0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00015fe0: 2022 476f 7420 756e 6578 7065 6374 6564   "Got unexpected
+00015ff0: 2060 6669 6760 2061 7267 756d 656e 7421   `fig` argument!
+00016000: 2054 6f20 6170 706c 7920 7468 6520 6064   To apply the `d
+00016010: 6573 7069 6e65 6020 6865 6c70 6572 2022  espine` helper "
+00016020: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00016030: 2022 746f 2061 6c6c 2061 7865 732c 2069   "to all axes, i
+00016040: 6e76 6f6b 6520 7468 6520 6865 6c70 6572  nvoke the helper
+00016050: 206f 6e20 6561 6368 2061 7869 7320 7365   on each axis se
+00016060: 7061 7261 7465 6c79 2e22 0a20 2020 2020  parately.".     
+00016070: 2020 2020 2020 2029 0a20 2020 2020 2020         ).       
+00016080: 2073 6e73 2e64 6573 7069 6e65 2861 783d   sns.despine(ax=
+00016090: 7365 6c66 2e61 782c 202a 2a6b 7761 7267  self.ax, **kwarg
+000160a0: 7329 0a                                  s).
```

### Comparing `dantro-0.19.0b2/dantro/plot/utils/_file_writer.py` & `dantro-0.19.1/dantro/plot/utils/_file_writer.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/plot/utils/color_mngr.py` & `dantro-0.19.1/dantro/plot/utils/color_mngr.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/plot/utils/mpl.py` & `dantro-0.19.1/dantro/plot/utils/mpl.py`

 * *Files 0% similar despite different names*

```diff
@@ -154,15 +154,15 @@
     """Uses ``.findobj`` to search a figure or axis for legend objects and
     returns lists of handles and (string) labels.
     """
     import matplotlib as mpl
 
     h, l = [], []
     for lg in mpo.findobj(mpl.legend.Legend):
-        h += [_h for _h in lg.legendHandles]
+        h += [_h for _h in lg.legend_handles]
         l += [_t.get_text() for _t in lg.texts]
 
     # Remove duplicates and return
     return remove_duplicate_handles_labels(h, l)
 
 
 def prepare_legend_args(
```

### Comparing `dantro-0.19.0b2/dantro/plot/utils/plot_func.py` & `dantro-0.19.1/dantro/plot/utils/plot_func.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/plot_mngr.py` & `dantro-0.19.1/dantro/plot_mngr.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/proxy/hdf5.py` & `dantro-0.19.1/dantro/proxy/hdf5.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/tools.py` & `dantro-0.19.1/dantro/tools.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/utils/coords.py` & `dantro-0.19.1/dantro/utils/coords.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/utils/link.py` & `dantro-0.19.1/dantro/utils/link.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/utils/nx.py` & `dantro-0.19.1/dantro/utils/nx.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro/utils/ordereddict.py` & `dantro-0.19.1/dantro/utils/ordereddict.py`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/dantro.egg-info/PKG-INFO` & `dantro-0.19.1/dantro.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: dantro
-Version: 0.19.0b2
+Version: 0.19.1
 Summary: Handle, transform, and visualize hierarchically structured data
 Home-page: https://gitlab.com/utopia-project/dantro
 Author: dantro developers
 Author-email: dantro-dev@iup.uni.heidelberg.de
 License: LGPL-3.0-or-later
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 or later (LGPLv3+)
 Requires-Python: >=3.8
 Provides-Extra: test
 Provides-Extra: doc
 Provides-Extra: dev
 License-File: COPYING
```

### Comparing `dantro-0.19.0b2/dantro.egg-info/SOURCES.txt` & `dantro-0.19.1/dantro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/pyproject.toml` & `dantro-0.19.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dantro-0.19.0b2/setup.py` & `dantro-0.19.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python3
 # fmt: off
 
 from setuptools import find_packages, setup
 
 # Dependencies for dantro itself
 install_deps = [
-    "numpy",
+    "numpy < 2.0",
     "xarray >= 2022.11",
     "dask",
     "toolz",             # For dask.delayed
     "distributed",       # For dask's distributed scheduler
     "scipy",             # Used as a netcdf4 storage engine for xarray
     "sympy",
     "h5py",
@@ -142,14 +142,15 @@
     license="LGPL-3.0-or-later",
     url="https://gitlab.com/utopia-project/dantro",
     classifiers=[
         "Intended Audience :: Science/Research",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Utilities",
         "License :: OSI Approved :: GNU Lesser General Public License v3 or"
         " later (LGPLv3+)",
     ],
     #
     # Distribution details, dependencies, ...
     packages=find_packages(exclude=["tests.*", "tests"]),
```

