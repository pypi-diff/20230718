# Comparing `tmp/arviz-0.8.3.tar.gz` & `tmp/arviz-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/arviz-0.8.3.tar", last modified: Thu May 28 13:54:21 2020, max compression
+gzip compressed data, was "dist/arviz-0.9.0.tar", last modified: Tue Jun 23 14:08:54 2020, max compression
```

## Comparing `arviz-0.8.3.tar` & `arviz-0.9.0.tar`

### file list

```diff
@@ -1,163 +1,169 @@
-drwxr-xr-x   0 oriol     (1000) oriol     (1000)        0 2020-05-28 13:54:21.000000 arviz-0.8.3/
--rw-r--r--   0 oriol     (1000) oriol     (1000)      123 2019-12-08 19:17:10.000000 arviz-0.8.3/MANIFEST.in
-drwxr-xr-x   0 oriol     (1000) oriol     (1000)        0 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz.egg-info/
--rw-r--r--   0 oriol     (1000) oriol     (1000)     4839 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz.egg-info/SOURCES.txt
--rw-r--r--   0 oriol     (1000) oriol     (1000)        1 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz.egg-info/dependency_links.txt
--rw-r--r--   0 oriol     (1000) oriol     (1000)      110 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz.egg-info/requires.txt
--rw-r--r--   0 oriol     (1000) oriol     (1000)        6 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz.egg-info/top_level.txt
--rw-r--r--   0 oriol     (1000) oriol     (1000)     8697 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz.egg-info/PKG-INFO
--rw-r--r--   0 oriol     (1000) oriol     (1000)       84 2020-03-20 19:13:09.000000 arviz-0.8.3/requirements.txt
--rw-r--r--   0 oriol     (1000) oriol     (1000)     2555 2020-05-05 10:39:04.000000 arviz-0.8.3/setup.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     6256 2020-05-05 10:39:04.000000 arviz-0.8.3/README.md
-drwxr-xr-x   0 oriol     (1000) oriol     (1000)        0 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz/
-drwxr-xr-x   0 oriol     (1000) oriol     (1000)        0 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz/plots/
--rw-r--r--   0 oriol     (1000) oriol     (1000)     7347 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/jointplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1235 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/__init__.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    11884 2020-05-16 21:04:42.000000 arviz-0.8.3/arviz/plots/essplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     8402 2020-05-16 21:04:42.000000 arviz-0.8.3/arviz/plots/forestplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     6930 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/rankplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     5015 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/compareplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     4666 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/hdiplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     9651 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/densityplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    20776 2020-05-16 21:04:17.000000 arviz-0.8.3/arviz/plots/plot_utils.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    11558 2020-05-16 21:04:17.000000 arviz-0.8.3/arviz/plots/pairplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     5228 2020-04-03 16:06:59.000000 arviz-0.8.3/arviz/plots/energyplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     6297 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/parallelplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    11958 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/ppcplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    10647 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/loopitplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     6678 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/distplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     4982 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/autocorrplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     8158 2020-05-16 21:04:17.000000 arviz-0.8.3/arviz/plots/khatplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     7702 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/kdeplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    10840 2020-05-28 13:53:56.000000 arviz-0.8.3/arviz/plots/traceplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     7387 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/mcseplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     8019 2020-05-16 21:04:17.000000 arviz-0.8.3/arviz/plots/elpdplot.py
-drwxr-xr-x   0 oriol     (1000) oriol     (1000)        0 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz/plots/styles/
--rw-r--r--   0 oriol     (1000) oriol     (1000)      218 2019-12-08 19:17:10.000000 arviz-0.8.3/arviz/plots/styles/arviz-colors.mplstyle
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1036 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/styles/arviz-whitegrid.mplstyle
--rw-r--r--   0 oriol     (1000) oriol     (1000)      987 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/styles/arviz-grayscale.mplstyle
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1042 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/styles/arviz-darkgrid.mplstyle
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1047 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/styles/arviz-white.mplstyle
--rw-r--r--   0 oriol     (1000) oriol     (1000)     6314 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/violinplot.py
-drwxr-xr-x   0 oriol     (1000) oriol     (1000)        0 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz/plots/backends/
--rw-r--r--   0 oriol     (1000) oriol     (1000)     7491 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/backends/__init__.py
-drwxr-xr-x   0 oriol     (1000) oriol     (1000)        0 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/
--rw-r--r--   0 oriol     (1000) oriol     (1000)     2503 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/jointplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1465 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/__init__.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     4356 2020-04-03 16:06:59.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/essplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    19542 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/forestplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     2727 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/rankplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     2796 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/compareplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)      658 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/hdiplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     4821 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/densityplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    12033 2020-05-28 13:53:56.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/pairplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1958 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/energyplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1183 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/parallelplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    14474 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/ppcplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1897 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/loopitplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     2576 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/distplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1391 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/autocorrplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     4948 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/khatplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     4419 2020-04-03 16:06:59.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/kdeplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    13178 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/traceplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     4482 2020-04-03 16:06:59.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/mcseplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     5344 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/elpdplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     2919 2020-05-16 21:04:42.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/violinplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     7951 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/backends/matplotlib/posteriorplot.py
-drwxr-xr-x   0 oriol     (1000) oriol     (1000)        0 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz/plots/backends/bokeh/
--rw-r--r--   0 oriol     (1000) oriol     (1000)     3218 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/bokeh/jointplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1949 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/backends/bokeh/__init__.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     5148 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/bokeh/essplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    21244 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/backends/bokeh/forestplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     3935 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/bokeh/rankplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     3852 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/bokeh/compareplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1538 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/backends/bokeh/hdiplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     5846 2020-05-16 21:04:42.000000 arviz-0.8.3/arviz/plots/backends/bokeh/densityplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    11247 2020-05-16 21:04:17.000000 arviz-0.8.3/arviz/plots/backends/bokeh/pairplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     3120 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/bokeh/energyplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1973 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/bokeh/parallelplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     8860 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/backends/bokeh/ppcplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     4977 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/backends/bokeh/loopitplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     3384 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/backends/bokeh/distplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     2278 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/bokeh/autocorrplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     2682 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/bokeh/khatplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     8210 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/bokeh/kdeplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    11786 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/plots/backends/bokeh/traceplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     5428 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/bokeh/mcseplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     5830 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/plots/backends/bokeh/elpdplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     3517 2020-05-16 21:04:42.000000 arviz-0.8.3/arviz/plots/backends/bokeh/violinplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     7545 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/backends/bokeh/posteriorplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     9260 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/plots/posteriorplot.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     9714 2020-05-28 13:53:56.000000 arviz-0.8.3/arviz/__init__.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     6737 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/numeric_utils.py
-drwxr-xr-x   0 oriol     (1000) oriol     (1000)        0 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz/data/
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1190 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/data/__init__.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    15650 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/data/io_cmdstanpy.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     9562 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/data/datasets.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    13577 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/data/io_numpyro.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    12908 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/data/io_pyro.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    17999 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/data/io_emcee.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    23995 2020-05-28 13:53:56.000000 arviz-0.8.3/arviz/data/io_pymc3.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     9087 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/data/io_dict.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1500 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/data/io_netcdf.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    31888 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/data/inference_data.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     7835 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/data/converters.py
-drwxr-xr-x   0 oriol     (1000) oriol     (1000)        0 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz/data/_datasets/
--rw-r--r--   0 oriol     (1000) oriol     (1000)   776656 2019-12-08 19:17:10.000000 arviz-0.8.3/arviz/data/_datasets/non_centered_eight.nc
--rw-r--r--   0 oriol     (1000) oriol     (1000)   616237 2019-12-08 19:17:10.000000 arviz-0.8.3/arviz/data/_datasets/centered_eight.nc
--rw-r--r--   0 oriol     (1000) oriol     (1000)     8056 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/data/base.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    34555 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/data/io_cmdstan.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     7447 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/data/io_tfp.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    32624 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/data/io_pystan.py
-drwxr-xr-x   0 oriol     (1000) oriol     (1000)        0 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz/tests/
--rw-r--r--   0 oriol     (1000) oriol     (1000)       18 2019-12-08 19:17:10.000000 arviz-0.8.3/arviz/tests/__init__.py
-drwxr-xr-x   0 oriol     (1000) oriol     (1000)        0 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz/tests/base_tests/
--rw-r--r--   0 oriol     (1000) oriol     (1000)       23 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/tests/base_tests/__init__.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)      657 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/tests/base_tests/test_helpers.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1752 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/tests/base_tests/test_stats_numba.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    31947 2020-05-28 13:53:56.000000 arviz-0.8.3/arviz/tests/base_tests/test_plots_bokeh.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    24594 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/tests/base_tests/test_stats.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     3358 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/tests/base_tests/test_diagnostics_numba.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    38173 2020-05-28 13:53:56.000000 arviz-0.8.3/arviz/tests/base_tests/test_plots_matplotlib.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    13792 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/tests/base_tests/test_stats_utils.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    10297 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/tests/base_tests/test_rcparams.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     8761 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/tests/base_tests/test_utils.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    21634 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/tests/base_tests/test_diagnostics.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     3018 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/tests/base_tests/test_utils_numba.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     8210 2020-05-16 21:04:17.000000 arviz-0.8.3/arviz/tests/base_tests/test_plot_utils.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    36848 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/tests/base_tests/test_data.py
-drwxr-xr-x   0 oriol     (1000) oriol     (1000)        0 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz/tests/external_tests/
--rw-r--r--   0 oriol     (1000) oriol     (1000)       26 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/tests/external_tests/__init__.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     9423 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/tests/external_tests/test_data_numpyro.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    21641 2020-05-28 13:53:56.000000 arviz-0.8.3/arviz/tests/external_tests/test_data_pymc.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     4400 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/tests/external_tests/test_data_tfp.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     6306 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/tests/external_tests/test_data_emcee.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    10367 2020-05-16 21:04:17.000000 arviz-0.8.3/arviz/tests/external_tests/test_data_pystan.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     9605 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/tests/external_tests/test_data_pyro.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    15451 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/tests/external_tests/test_data_cmdstan.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     6715 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/tests/external_tests/test_data_cmdstanpy.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    22635 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/tests/helpers.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1269 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/tests/conftest.py
-drwxr-xr-x   0 oriol     (1000) oriol     (1000)        0 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz/wrappers/
--rw-r--r--   0 oriol     (1000) oriol     (1000)      163 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/wrappers/__init__.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     8065 2020-03-20 19:13:09.000000 arviz-0.8.3/arviz/wrappers/base.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     2430 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/wrappers/wrap_pystan.py
-drwxr-xr-x   0 oriol     (1000) oriol     (1000)        0 2020-05-28 13:54:21.000000 arviz-0.8.3/arviz/stats/
--rw-r--r--   0 oriol     (1000) oriol     (1000)    32251 2020-05-05 10:39:04.000000 arviz-0.8.3/arviz/stats/diagnostics.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)      549 2020-05-16 21:04:42.000000 arviz-0.8.3/arviz/stats/__init__.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    64292 2020-05-23 14:56:21.000000 arviz-0.8.3/arviz/stats/stats.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    19962 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/stats/stats_utils.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)     5409 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/stats/stats_refitting.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    23002 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/utils.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)    19182 2020-05-22 18:39:54.000000 arviz-0.8.3/arviz/rcparams.py
--rw-r--r--   0 oriol     (1000) oriol     (1000)       38 2020-05-28 13:54:21.000000 arviz-0.8.3/setup.cfg
--rw-r--r--   0 oriol     (1000) oriol     (1000)       31 2020-03-20 19:13:09.000000 arviz-0.8.3/pyproject.toml
--rw-r--r--   0 oriol     (1000) oriol     (1000)      135 2020-03-20 19:13:09.000000 arviz-0.8.3/requirements-external.txt
--rw-r--r--   0 oriol     (1000) oriol     (1000)    14337 2020-05-05 10:39:04.000000 arviz-0.8.3/CONTRIBUTING.md
--rw-r--r--   0 oriol     (1000) oriol     (1000)    11358 2019-12-08 19:17:10.000000 arviz-0.8.3/LICENSE
--rw-r--r--   0 oriol     (1000) oriol     (1000)    12537 2020-05-28 13:53:56.000000 arviz-0.8.3/CHANGELOG.md
--rw-r--r--   0 oriol     (1000) oriol     (1000)     8697 2020-05-28 13:54:21.000000 arviz-0.8.3/PKG-INFO
--rw-r--r--   0 oriol     (1000) oriol     (1000)       19 2020-03-20 19:13:09.000000 arviz-0.8.3/requirements-optional.txt
--rw-r--r--   0 oriol     (1000) oriol     (1000)     1817 2019-12-08 19:17:10.000000 arviz-0.8.3/CODE_OF_CONDUCT.md
--rw-r--r--   0 oriol     (1000) oriol     (1000)      122 2020-05-22 18:39:54.000000 arviz-0.8.3/requirements-docs.txt
--rw-r--r--   0 oriol     (1000) oriol     (1000)       99 2020-05-05 10:39:04.000000 arviz-0.8.3/requirements-dev.txt
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-23 14:08:54.882760 arviz-0.9.0/
+-rw-r--r--   0 vsts      (1001) docker     (116)    14516 2020-06-23 14:08:31.000000 arviz-0.9.0/CHANGELOG.md
+-rw-r--r--   0 vsts      (1001) docker     (116)     1817 2020-06-23 14:08:31.000000 arviz-0.9.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 vsts      (1001) docker     (116)    14337 2020-06-23 14:08:31.000000 arviz-0.9.0/CONTRIBUTING.md
+-rw-r--r--   0 vsts      (1001) docker     (116)    14035 2020-06-23 14:08:31.000000 arviz-0.9.0/GOVERNANCE.md
+-rw-r--r--   0 vsts      (1001) docker     (116)    11358 2020-06-23 14:08:31.000000 arviz-0.9.0/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (116)      123 2020-06-23 14:08:31.000000 arviz-0.9.0/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (116)     8697 2020-06-23 14:08:54.882760 arviz-0.9.0/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (116)     6256 2020-06-23 14:08:31.000000 arviz-0.9.0/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-23 14:08:54.870760 arviz-0.9.0/arviz/
+-rw-r--r--   0 vsts      (1001) docker     (116)     9714 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-23 14:08:54.870760 arviz-0.9.0/arviz/data/
+-rw-r--r--   0 vsts      (1001) docker     (116)     1244 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-23 14:08:54.870760 arviz-0.9.0/arviz/data/_datasets/
+-rw-r--r--   0 vsts      (1001) docker     (116)   616237 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/_datasets/centered_eight.nc
+-rw-r--r--   0 vsts      (1001) docker     (116)   776656 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/_datasets/non_centered_eight.nc
+-rw-r--r--   0 vsts      (1001) docker     (116)     8056 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/base.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     7835 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/converters.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     9562 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/datasets.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    34787 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/inference_data.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    34555 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/io_cmdstan.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    15650 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/io_cmdstanpy.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     9087 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/io_dict.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    17999 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/io_emcee.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1500 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/io_netcdf.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    13577 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/io_numpyro.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    12712 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/io_pyjags.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    24551 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/io_pymc3.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    13442 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/io_pyro.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    32624 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/io_pystan.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     7447 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/data/io_tfp.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     6740 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/numeric_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-23 14:08:54.874760 arviz-0.9.0/arviz/plots/
+-rw-r--r--   0 vsts      (1001) docker     (116)     1316 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4982 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/autocorrplot.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-23 14:08:54.874760 arviz-0.9.0/arviz/plots/backends/
+-rw-r--r--   0 vsts      (1001) docker     (116)     7491 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-23 14:08:54.878760 arviz-0.9.0/arviz/plots/backends/bokeh/
+-rw-r--r--   0 vsts      (1001) docker     (116)     1949 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2278 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/autocorrplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3852 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/compareplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     5846 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/densityplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      402 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/distcomparisonplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3384 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/distplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     5830 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/elpdplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3120 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/energyplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     5148 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/essplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    21244 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/forestplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      948 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/hdiplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3218 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/jointplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     8210 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/kdeplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2682 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/khatplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     5118 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/loopitplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     5428 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/mcseplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    11247 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/pairplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1973 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/parallelplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     7545 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/posteriorplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     8860 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/ppcplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3935 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/rankplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    11675 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/traceplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3517 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/bokeh/violinplot.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-23 14:08:54.878760 arviz-0.9.0/arviz/plots/backends/matplotlib/
+-rw-r--r--   0 vsts      (1001) docker     (116)     1465 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1391 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/autocorrplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2796 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/compareplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4821 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/densityplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1957 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/distcomparisonplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2576 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/distplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     5344 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/elpdplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1958 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/energyplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4356 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/essplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    19542 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/forestplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      625 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/hdiplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2503 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/jointplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4419 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/kdeplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4948 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/khatplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2130 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/loopitplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4482 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/mcseplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    12033 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/pairplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1183 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/parallelplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     7951 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/posteriorplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    14475 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/ppcplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2727 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/rankplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    13348 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/traceplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2919 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/backends/matplotlib/violinplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     5015 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/compareplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     9651 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/densityplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     6765 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/distcomparisonplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     6678 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/distplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     8019 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/elpdplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     5228 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/energyplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    11884 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/essplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     8402 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/forestplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     6888 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/hdiplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     7347 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/jointplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     7752 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/kdeplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     8158 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/khatplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    10324 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/loopitplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     7387 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/mcseplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    11631 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/pairplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     6297 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/parallelplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    21405 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/plot_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     9260 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/posteriorplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    11958 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/ppcplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     6930 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/rankplot.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-23 14:08:54.878760 arviz-0.9.0/arviz/plots/styles/
+-rw-r--r--   0 vsts      (1001) docker     (116)      218 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/styles/arviz-colors.mplstyle
+-rw-r--r--   0 vsts      (1001) docker     (116)     1078 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/styles/arviz-darkgrid.mplstyle
+-rw-r--r--   0 vsts      (1001) docker     (116)     1023 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/styles/arviz-grayscale.mplstyle
+-rw-r--r--   0 vsts      (1001) docker     (116)     1083 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/styles/arviz-white.mplstyle
+-rw-r--r--   0 vsts      (1001) docker     (116)     1072 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/styles/arviz-whitegrid.mplstyle
+-rw-r--r--   0 vsts      (1001) docker     (116)    11515 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/traceplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     6314 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/plots/violinplot.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    19182 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/rcparams.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-23 14:08:54.878760 arviz-0.9.0/arviz/stats/
+-rw-r--r--   0 vsts      (1001) docker     (116)      549 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/stats/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    32251 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/stats/diagnostics.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    64508 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/stats/stats.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     5409 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/stats/stats_refitting.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    19962 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/stats/stats_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-23 14:08:54.878760 arviz-0.9.0/arviz/tests/
+-rw-r--r--   0 vsts      (1001) docker     (116)       18 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-23 14:08:54.882760 arviz-0.9.0/arviz/tests/base_tests/
+-rw-r--r--   0 vsts      (1001) docker     (116)       23 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/base_tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    37831 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/base_tests/test_data.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    21634 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/base_tests/test_diagnostics.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3358 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/base_tests/test_diagnostics_numba.py
+-rw-r--r--   0 vsts      (1001) docker     (116)      657 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/base_tests/test_helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     8897 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/base_tests/test_plot_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    32461 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/base_tests/test_plots_bokeh.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    41622 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/base_tests/test_plots_matplotlib.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    10297 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/base_tests/test_rcparams.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    24594 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/base_tests/test_stats.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1752 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/base_tests/test_stats_numba.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    13792 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/base_tests/test_stats_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     8761 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/base_tests/test_utils.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     3018 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/base_tests/test_utils_numba.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     1269 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/conftest.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-23 14:08:54.882760 arviz-0.9.0/arviz/tests/external_tests/
+-rw-r--r--   0 vsts      (1001) docker     (116)       26 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/external_tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    15451 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/external_tests/test_data_cmdstan.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     6715 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/external_tests/test_data_cmdstanpy.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     6306 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/external_tests/test_data_emcee.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     9423 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/external_tests/test_data_numpyro.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     8193 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/external_tests/test_data_pyjags.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    26424 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/external_tests/test_data_pymc.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    10814 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/external_tests/test_data_pyro.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    10367 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/external_tests/test_data_pystan.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     4400 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/external_tests/test_data_tfp.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    22635 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/tests/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (116)    24139 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-23 14:08:54.882760 arviz-0.9.0/arviz/wrappers/
+-rw-r--r--   0 vsts      (1001) docker     (116)      163 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/wrappers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     8065 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/wrappers/base.py
+-rw-r--r--   0 vsts      (1001) docker     (116)     2430 2020-06-23 14:08:31.000000 arviz-0.9.0/arviz/wrappers/wrap_pystan.py
+drwxr-xr-x   0 vsts      (1001) docker     (116)        0 2020-06-23 14:08:54.870760 arviz-0.9.0/arviz.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (116)     8697 2020-06-23 14:08:54.000000 arviz-0.9.0/arviz.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (116)     5061 2020-06-23 14:08:54.000000 arviz-0.9.0/arviz.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        1 2020-06-23 14:08:54.000000 arviz-0.9.0/arviz.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)      110 2020-06-23 14:08:54.000000 arviz-0.9.0/arviz.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)        6 2020-06-23 14:08:54.000000 arviz-0.9.0/arviz.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       31 2020-06-23 14:08:31.000000 arviz-0.9.0/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (116)       99 2020-06-23 14:08:31.000000 arviz-0.9.0/requirements-dev.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)      122 2020-06-23 14:08:31.000000 arviz-0.9.0/requirements-docs.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)      142 2020-06-23 14:08:31.000000 arviz-0.9.0/requirements-external.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       19 2020-06-23 14:08:31.000000 arviz-0.9.0/requirements-optional.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       84 2020-06-23 14:08:31.000000 arviz-0.9.0/requirements.txt
+-rw-r--r--   0 vsts      (1001) docker     (116)       38 2020-06-23 14:08:54.882760 arviz-0.9.0/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (116)     2555 2020-06-23 14:08:31.000000 arviz-0.9.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `arviz-0.8.3/arviz.egg-info/SOURCES.txt` & `arviz-0.9.0/arviz.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 CHANGELOG.md
 CODE_OF_CONDUCT.md
 CONTRIBUTING.md
+GOVERNANCE.md
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements-docs.txt
 requirements-external.txt
@@ -27,24 +28,26 @@
 arviz/data/inference_data.py
 arviz/data/io_cmdstan.py
 arviz/data/io_cmdstanpy.py
 arviz/data/io_dict.py
 arviz/data/io_emcee.py
 arviz/data/io_netcdf.py
 arviz/data/io_numpyro.py
+arviz/data/io_pyjags.py
 arviz/data/io_pymc3.py
 arviz/data/io_pyro.py
 arviz/data/io_pystan.py
 arviz/data/io_tfp.py
 arviz/data/_datasets/centered_eight.nc
 arviz/data/_datasets/non_centered_eight.nc
 arviz/plots/__init__.py
 arviz/plots/autocorrplot.py
 arviz/plots/compareplot.py
 arviz/plots/densityplot.py
+arviz/plots/distcomparisonplot.py
 arviz/plots/distplot.py
 arviz/plots/elpdplot.py
 arviz/plots/energyplot.py
 arviz/plots/essplot.py
 arviz/plots/forestplot.py
 arviz/plots/hdiplot.py
 arviz/plots/jointplot.py
@@ -61,14 +64,15 @@
 arviz/plots/traceplot.py
 arviz/plots/violinplot.py
 arviz/plots/backends/__init__.py
 arviz/plots/backends/bokeh/__init__.py
 arviz/plots/backends/bokeh/autocorrplot.py
 arviz/plots/backends/bokeh/compareplot.py
 arviz/plots/backends/bokeh/densityplot.py
+arviz/plots/backends/bokeh/distcomparisonplot.py
 arviz/plots/backends/bokeh/distplot.py
 arviz/plots/backends/bokeh/elpdplot.py
 arviz/plots/backends/bokeh/energyplot.py
 arviz/plots/backends/bokeh/essplot.py
 arviz/plots/backends/bokeh/forestplot.py
 arviz/plots/backends/bokeh/hdiplot.py
 arviz/plots/backends/bokeh/jointplot.py
@@ -83,14 +87,15 @@
 arviz/plots/backends/bokeh/rankplot.py
 arviz/plots/backends/bokeh/traceplot.py
 arviz/plots/backends/bokeh/violinplot.py
 arviz/plots/backends/matplotlib/__init__.py
 arviz/plots/backends/matplotlib/autocorrplot.py
 arviz/plots/backends/matplotlib/compareplot.py
 arviz/plots/backends/matplotlib/densityplot.py
+arviz/plots/backends/matplotlib/distcomparisonplot.py
 arviz/plots/backends/matplotlib/distplot.py
 arviz/plots/backends/matplotlib/elpdplot.py
 arviz/plots/backends/matplotlib/energyplot.py
 arviz/plots/backends/matplotlib/essplot.py
 arviz/plots/backends/matplotlib/forestplot.py
 arviz/plots/backends/matplotlib/hdiplot.py
 arviz/plots/backends/matplotlib/jointplot.py
@@ -133,14 +138,15 @@
 arviz/tests/base_tests/test_utils.py
 arviz/tests/base_tests/test_utils_numba.py
 arviz/tests/external_tests/__init__.py
 arviz/tests/external_tests/test_data_cmdstan.py
 arviz/tests/external_tests/test_data_cmdstanpy.py
 arviz/tests/external_tests/test_data_emcee.py
 arviz/tests/external_tests/test_data_numpyro.py
+arviz/tests/external_tests/test_data_pyjags.py
 arviz/tests/external_tests/test_data_pymc.py
 arviz/tests/external_tests/test_data_pyro.py
 arviz/tests/external_tests/test_data_pystan.py
 arviz/tests/external_tests/test_data_tfp.py
 arviz/wrappers/__init__.py
 arviz/wrappers/base.py
 arviz/wrappers/wrap_pystan.py
```

### Comparing `arviz-0.8.3/arviz.egg-info/PKG-INFO` & `arviz-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arviz
-Version: 0.8.3
+Version: 0.9.0
 Summary: Exploratory analysis of Bayesian models
 Home-page: http://github.com/arviz-devs/arviz
 Author: ArviZ Developers
 License: Apache-2.0
 Description: <img src="https://arviz-devs.github.io/arviz/_static/logo.png" height=100></img>
         
         [![Azure Build Status](https://dev.azure.com/ArviZ/ArviZ/_apis/build/status/arviz-devs.arviz?branchName=master)](https://dev.azure.com/ArviZ/ArviZ/_build/latest?definitionId=1&branchName=master)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: arviz Version: 0.8.3 Summary: Exploratory analysis
+Metadata-Version: 2.1 Name: arviz Version: 0.9.0 Summary: Exploratory analysis
 of Bayesian models Home-page: http://github.com/arviz-devs/arviz Author: ArviZ
 Developers License: Apache-2.0 Description: [https://arviz-devs.github.io/
 arviz/_static/logo.png] [![Azure Build Status](https://dev.azure.com/ArviZ/
 ArviZ/_apis/build/status/arviz-devs.arviz?branchName=master)](https://
 dev.azure.com/ArviZ/ArviZ/_build/latest?definitionId=1&branchName=master) [!
 [codecov](https://codecov.io/gh/arviz-devs/arviz/branch/master/graph/
 badge.svg)](https://codecov.io/gh/arviz-devs/arviz) [![Code style: black]
```

### Comparing `arviz-0.8.3/setup.py` & `arviz-0.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/README.md` & `arviz-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/jointplot.py` & `arviz-0.9.0/arviz/plots/jointplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/__init__.py` & `arviz-0.9.0/arviz/plots/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .khatplot import plot_khat
 from .loopitplot import plot_loo_pit
 from .mcseplot import plot_mcse
 from .pairplot import plot_pair
 from .parallelplot import plot_parallel
 from .posteriorplot import plot_posterior
 from .ppcplot import plot_ppc
+from .distcomparisonplot import plot_dist_comparison
 from .rankplot import plot_rank
 from .traceplot import plot_trace
 from .violinplot import plot_violin
 from ..numeric_utils import _fast_kde_2d
 
 
 __all__ = [
@@ -40,11 +41,12 @@
     "plot_khat",
     "plot_loo_pit",
     "plot_mcse",
     "plot_pair",
     "plot_parallel",
     "plot_posterior",
     "plot_ppc",
+    "plot_dist_comparison",
     "plot_rank",
     "plot_trace",
     "plot_violin",
 ]
```

### Comparing `arviz-0.8.3/arviz/plots/essplot.py` & `arviz-0.9.0/arviz/plots/essplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     ----------
     * Vehtari et al. (2019) see https://arxiv.org/abs/1903.08008
 
     Examples
     --------
     Plot local ESS. This plot, together with the quantile ESS plot, is recommended to check
     that there are enough samples for all the explored regions of parameter space. Checking
-    local and quantile ESS is particularly relevant when working with hdi intervals as
+    local and quantile ESS is particularly relevant when working with HDI intervals as
     opposed to ESS bulk, which is relevant for point estimates.
 
     .. plot::
         :context: close-figs
 
         >>> import arviz as az
         >>> idata = az.load_arviz_data("centered_eight")
```

### Comparing `arviz-0.8.3/arviz/plots/forestplot.py` & `arviz-0.9.0/arviz/plots/forestplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,17 +32,17 @@
     ax=None,
     backend=None,
     backend_config=None,
     backend_kwargs=None,
     show=None,
     credible_interval=None,
 ):
-    """Forest plot to compare hdi intervals from a number of distributions.
+    """Forest plot to compare HDI intervals from a number of distributions.
 
-    Generates a forest plot of 100*(hdi_prob)% hdi intervals from
+    Generates a forest plot of 100*(hdi_prob)% HDI intervals from
     a trace or list of traces.
 
     Parameters
     ----------
     data: obj or list[obj]
         Any object that can be converted to an az.InferenceData object
         Refer to documentation of az.convert_to_dataset for details
```

### Comparing `arviz-0.8.3/arviz/plots/rankplot.py` & `arviz-0.9.0/arviz/plots/rankplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/compareplot.py` & `arviz-0.9.0/arviz/plots/compareplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/densityplot.py` & `arviz-0.9.0/arviz/plots/densityplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/plot_utils.py` & `arviz-0.9.0/arviz/plots/plot_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -659,17 +659,39 @@
     if args is None:
         return {}
     matplotlib_kwarg_dealiaser_dict = {
         "scatter": mpl.collections.PathCollection,
         "plot": mpl.lines.Line2D,
         "hist": mpl.patches.Patch,
         "hexbin": mpl.collections.PolyCollection,
+        "fill_between": mpl.collections.PolyCollection,
         "hlines": mpl.collections.LineCollection,
         "text": mpl.text.Text,
         "contour": mpl.contour.ContourSet,
         "pcolormesh": mpl.collections.QuadMesh,
     }
     if backend == "matplotlib":
         return cbook.normalize_kwargs(
             args, getattr(matplotlib_kwarg_dealiaser_dict[kind], "_alias_map", {})
         )
     return args
+
+
+def _dealiase_sel_kwargs(kwargs, prop_dict, idx):
+    """Generate kwargs dict from kwargs and prop_dict.
+
+    Gets property at position ``idx`` for each property in prop_dict and adds it to
+    ``kwargs``. Values in prop_dict are dealiased and overwrite values in
+    kwargs with the same key .
+
+    Parameters
+    ----------
+    kwargs : dict
+    prop_dict : dict of {str : array_like}
+    idx : int
+    """
+    return {
+        **kwargs,
+        **matplotlib_kwarg_dealiaser(
+            {prop: props[idx] for prop, props in prop_dict.items()}, "plot"
+        ),
+    }
```

### Comparing `arviz-0.8.3/arviz/plots/pairplot.py` & `arviz-0.9.0/arviz/plots/pairplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,15 +190,16 @@
         )
 
     if scatter_kwargs is None:
         scatter_kwargs = {}
 
     scatter_kwargs.setdefault("marker", ".")
     scatter_kwargs.setdefault("lw", 0)
-    scatter_kwargs.setdefault("zorder", 0)
+    # Sets the default zorder higher than zorder of grid, which is 0.5
+    scatter_kwargs.setdefault("zorder", 0.6)
 
     if kde_kwargs is None:
         kde_kwargs = {}
 
     if hexbin_kwargs is None:
         hexbin_kwargs = {}
```

### Comparing `arviz-0.8.3/arviz/plots/energyplot.py` & `arviz-0.9.0/arviz/plots/energyplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/parallelplot.py` & `arviz-0.9.0/arviz/plots/parallelplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/ppcplot.py` & `arviz-0.9.0/arviz/plots/ppcplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/loopitplot.py` & `arviz-0.9.0/arviz/plots/loopitplot.py`

 * *Files 16% similar despite different names*

```diff
@@ -61,17 +61,17 @@
         `Vehtari et al. (2019)`, `Appendix G <https://avehtari.github.io/rhat_ess/rhat_ess.html>`_.
     ecdf_fill : bool, optional
         Use fill_between to mark the area inside the credible interval. Otherwise, plot the
         border lines.
     n_unif : int, optional
         Number of datasets to simulate and overlay from the uniform distribution.
     use_hdi : bool, optional
-        Use plot_hdi to fill between hdi values instead of overlaying the uniform distributions.
+        Compute expected hdi values instead of overlaying the sampled uniform distributions.
     credible_interval : float, optional
-        Credible interval of the hdi or of the ECDF theoretical credible interval
+        Theoretical credible interval. Works with ``use_hdi=True`` or ``ecdf=True``.
     figsize : figure size tuple, optional
         If None, size is (8 + numvars, 8 + numvars)
     textsize: int, optional
         Text size for labels. If None it will be autoscaled based on figsize.
     color : str or array_like, optional
         Color of the LOO-PIT estimated pdf plot. If ``plot_unif_kwargs`` has no "color" key,
         an slightly lighter color than this argument will be used for the uniform kde lines.
@@ -82,15 +82,15 @@
         Matplotlib axes or bokeh figures.
     plot_kwargs : dict, optional
         Additional keywords passed to ax.plot for LOO-PIT line (kde or ECDF)
     plot_unif_kwargs : dict, optional
         Additional keywords passed to ax.plot for overlaid uniform distributions or
         for beta credible interval lines if ``ecdf=True``
     hdi_kwargs : dict, optional
-        Additional keywords passed to az.plot_hdi
+        Additional keywords passed to ax.axhspan
     fill_kwargs : dict, optional
         Additional kwargs passed to ax.fill_between
     backend: str, optional
         Select plotting backend {"matplotlib","bokeh"}. Default "matplotlib".
     backend_kwargs: bool, optional
         These are kwargs specific to the backend being used. For additional documentation
         check the plotting method of the backend.
@@ -164,16 +164,16 @@
     plot_unif_kwargs.setdefault("linewidth", 0.6 * linewidth)
 
     loo_pit_ecdf = None
     unif_ecdf = None
     p975 = None
     p025 = None
     loo_pit_kde = None
+    hdi_odds = None
     unif = None
-    unif_densities = None
     x_vals = None
 
     if credible_interval is None:
         credible_interval = rcParams["stats.hdi_prob"]
     else:
         if not 1 >= credible_interval > 0:
             raise ValueError("The value of credible_interval should be in the interval (0, 1]")
@@ -202,44 +202,43 @@
             fill_kwargs.setdefault("color", to_hex(hsv_to_rgb(light_color)))
             fill_kwargs.setdefault("alpha", 0.5)
             fill_kwargs.setdefault(
                 "step", "mid" if plot_kwargs["drawstyle"] == "steps-mid" else None
             )
             fill_kwargs.setdefault("label", "{:.3g}% credible interval".format(credible_interval))
     else:
-        loo_pit_kde, _, _ = _fast_kde(loo_pit, xmin=0, xmax=1)
+        loo_pit_kde, xmin, xmax = _fast_kde(loo_pit)
 
         unif = np.random.uniform(size=(n_unif, loo_pit.size))
-        x_vals = np.linspace(0, 1, len(loo_pit_kde))
+        x_vals = np.linspace(xmin, xmax, len(loo_pit_kde))
         if use_hdi:
+            n_obs = loo_pit.size
+            hdi_ = stats.beta(n_obs / 2, n_obs / 2).ppf((1 - credible_interval) / 2)
+            hdi_odds = (hdi_ / (1 - hdi_), (1 - hdi_) / hdi_)
             if hdi_kwargs is None:
                 hdi_kwargs = {}
             hdi_kwargs.setdefault("color", to_hex(hsv_to_rgb(light_color)))
-            hdi_fill_kwargs = hdi_kwargs.pop("fill_kwargs", {})
-            hdi_fill_kwargs.setdefault("label", "Uniform hdi")
-            hdi_kwargs["fill_kwargs"] = hdi_fill_kwargs
-            hdi_kwargs["credible_interval"] = credible_interval
-
-            unif_densities = np.empty((n_unif, len(loo_pit_kde)))
+            hdi_kwargs.setdefault("alpha", 0.35)
+            hdi_kwargs.setdefault("label", "Uniform HDI")
 
     loo_pit_kwargs = dict(
         ax=ax,
         figsize=figsize,
         ecdf=ecdf,
         loo_pit=loo_pit,
         loo_pit_ecdf=loo_pit_ecdf,
         unif_ecdf=unif_ecdf,
         p975=p975,
         p025=p025,
         fill_kwargs=fill_kwargs,
         ecdf_fill=ecdf_fill,
         use_hdi=use_hdi,
         x_vals=x_vals,
-        unif_densities=unif_densities,
         hdi_kwargs=hdi_kwargs,
+        hdi_odds=hdi_odds,
         n_unif=n_unif,
         unif=unif,
         plot_unif_kwargs=plot_unif_kwargs,
         loo_pit_kde=loo_pit_kde,
         xt_labelsize=xt_labelsize,
         legend=legend,
         credible_interval=credible_interval,
@@ -249,22 +248,16 @@
     )
 
     if backend is None:
         backend = rcParams["plot.backend"]
     backend = backend.lower()
 
     if backend == "bokeh":
-
-        if (
-            loo_pit_kwargs["hdi_kwargs"] is not None
-            and "fill_kwargs" in loo_pit_kwargs["hdi_kwargs"]
-            and loo_pit_kwargs["hdi_kwargs"]["fill_kwargs"] is not None
-            and "label" in loo_pit_kwargs["hdi_kwargs"]["fill_kwargs"]
-        ):
-            loo_pit_kwargs["hdi_kwargs"]["fill_kwargs"].pop("label")
+        if use_hdi:
+            loo_pit_kwargs["hdi_kwargs"].pop("label", None)
         loo_pit_kwargs.pop("legend")
         loo_pit_kwargs.pop("xt_labelsize")
         loo_pit_kwargs.pop("credible_interval")
 
     # TODO: Add backend kwargs
     plot = get_plotting_function("plot_loo_pit", "loopitplot", backend)
     axes = plot(**loo_pit_kwargs)
```

### Comparing `arviz-0.8.3/arviz/plots/distplot.py` & `arviz-0.9.0/arviz/plots/distplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/autocorrplot.py` & `arviz-0.9.0/arviz/plots/autocorrplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/khatplot.py` & `arviz-0.9.0/arviz/plots/khatplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/kdeplot.py` & `arviz-0.9.0/arviz/plots/kdeplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -178,15 +178,18 @@
     """
     if isinstance(values, xr.Dataset):
         raise ValueError(
             "Xarray dataset object detected.Use plot_posterior, plot_density, plot_joint"
             "or plot_pair instead of plot_kde"
         )
     if isinstance(values, InferenceData):
-        raise ValueError(" Inference Data object detected. Use plot_posterior instead of plot_kde")
+        raise ValueError(
+            " Inference Data object detected. Use plot_posterior "
+            "or plot_pair instead of plot_kde"
+        )
 
     if values2 is None:
         density, lower, upper = _fast_kde(values, cumulative, bw)
 
         if cumulative:
             density_q = density
         else:
```

### Comparing `arviz-0.8.3/arviz/plots/traceplot.py` & `arviz-0.9.0/arviz/plots/traceplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Plot kde or histograms and values from MCMC samples."""
 from itertools import cycle
 import warnings
-from typing import Callable, List, Optional, Tuple, Any
+from typing import Callable, List, Optional, Tuple, Any, Mapping, Union
 
 import matplotlib.pyplot as plt
 
 from .plot_utils import (
     get_plotting_function,
     xarray_var_iter,
     KwargSpec,
@@ -18,23 +18,23 @@
 
 def plot_trace(
     data: InferenceData,
     var_names: Optional[List[str]] = None,
     filter_vars: Optional[str] = None,
     transform: Optional[Callable] = None,
     coords: Optional[CoordSpec] = None,
-    divergences: Optional[str] = "bottom",
+    divergences: Optional[str] = "auto",
     kind: Optional[str] = "trace",
     figsize: Optional[Tuple[float, float]] = None,
     rug: bool = False,
     lines: Optional[List[Tuple[str, CoordSpec, Any]]] = None,
     compact: bool = False,
-    compact_prop: Optional[Tuple[str, Any]] = None,
+    compact_prop: Optional[Union[str, Mapping[str, Any]]] = None,
     combined: bool = False,
-    chain_prop: Optional[Tuple[str, Any]] = None,
+    chain_prop: Optional[Union[str, Mapping[str, Any]]] = None,
     legend: bool = False,
     plot_kwargs: Optional[KwargSpec] = None,
     fill_kwargs: Optional[KwargSpec] = None,
     rug_kwargs: Optional[KwargSpec] = None,
     hist_kwargs: Optional[KwargSpec] = None,
     trace_kwargs: Optional[KwargSpec] = None,
     rank_kwargs: Optional[KwargSpec] = None,
@@ -76,21 +76,21 @@
         If True adds a rugplot. Defaults to False. Ignored for 2D KDE.
         Only affects continuous variables.
     lines: list of tuple of (str, dict, array_like), optional
         List of (var_name, {'coord': selection}, [line, positions]) to be overplotted as
         vertical lines on the density and horizontal lines on the trace.
     compact: bool, optional
         Plot multidimensional variables in a single plot.
-    compact_prop: tuple of (str, array_like), optional
+    compact_prop: str or dict {str: array_like}, optional
         Tuple containing the property name and the property values to distinguish diferent
         dimensions with compact=True
     combined: bool, optional
         Flag for combining multiple chains into a single line. If False (default), chains will be
         plotted separately.
-    chain_prop: tuple of (str, array_like), optional
+    chain_prop: str or dict {str: array_like}, optional
         Tuple containing the property name and the property values to distinguish diferent chains
     legend: bool, optional
         Add a legend to the figure with the chain color code.
     plot_kwargs, fill_kwargs, rug_kwargs, hist_kwargs: dict, optional
         Extra keyword arguments passed to `arviz.plot_dist`. Only affects continuous variables.
     trace_kwargs: dict, optional
         Extra keyword arguments passed to `plt.plot`
@@ -152,14 +152,16 @@
         >>> lines = (('theta_t',{'school': "Choate"}, [-1]),)
         >>> az.plot_trace(data, var_names=('theta_t', 'theta'), coords=coords, lines=lines)
 
     """
     if kind not in {"trace", "rank_vlines", "rank_bars"}:
         raise ValueError("The value of kind must be either trace, rank_vlines or rank_bars.")
 
+    if divergences == "auto":
+        divergences = "top" if rug else "bottom"
     if divergences:
         try:
             divergence_data = convert_to_dataset(data, group="sample_stats").diverging
         except (ValueError, AttributeError):  # No sample_stats, or no `.diverging`
             divergences = False
 
     if coords is None:
@@ -182,50 +184,63 @@
     if lines is None:
         lines = ()
 
     num_chain_props = len(data.chain) + 1 if combined else len(data.chain)
     if not compact:
         if backend == "bokeh":
             chain_prop = (
-                ("line_color", plt.rcParams["axes.prop_cycle"].by_key()["color"])
+                {"line_color": plt.rcParams["axes.prop_cycle"].by_key()["color"]}
                 if chain_prop is None
                 else chain_prop
             )
         else:
             chain_prop = "color" if chain_prop is None else chain_prop
     else:
         chain_prop = (
-            (
-                "line_dash" if backend == "bokeh" else "linestyle",
-                ("solid", "dotted", "dashed", "dashdot"),
-            )
+            {
+                "line_dash"
+                if backend == "bokeh"
+                else "linestyle": ("solid", "dotted", "dashed", "dashdot"),
+            }
             if chain_prop is None
             else chain_prop
         )
         if backend == "bokeh":
             compact_prop = (
-                ("line_color", plt.rcParams["axes.prop_cycle"].by_key()["color"])
+                {"line_color": plt.rcParams["axes.prop_cycle"].by_key()["color"]}
                 if compact_prop is None
                 else compact_prop
             )
         else:
             compact_prop = "color" if compact_prop is None else compact_prop
 
     # TODO: matplotlib is always required by arviz. Can we get rid of it?
     # TODO: kind of related: move mpl specific code to backend and
     # define prop_cycle instead of only colors
     if isinstance(chain_prop, str):
-        chain_prop = (chain_prop, plt.rcParams["axes.prop_cycle"].by_key()[chain_prop])
-    chain_prop = (
-        chain_prop[0],
-        [prop for _, prop in zip(range(num_chain_props), cycle(chain_prop[1]))],
-    )
+        chain_prop = {chain_prop: plt.rcParams["axes.prop_cycle"].by_key()[chain_prop]}
+    if isinstance(chain_prop, tuple):
+        warnings.warn(
+            "chain_prop as a tuple will be deprecated in a future warning, use a dict instead",
+            FutureWarning,
+        )
+        chain_prop = {chain_prop[0]: chain_prop[1]}
+    chain_prop = {
+        prop_name: [prop for _, prop in zip(range(num_chain_props), cycle(props))]
+        for prop_name, props in chain_prop.items()
+    }
 
     if isinstance(compact_prop, str):
-        compact_prop = (compact_prop, plt.rcParams["axes.prop_cycle"].by_key()[compact_prop])
+        compact_prop = {compact_prop: plt.rcParams["axes.prop_cycle"].by_key()[compact_prop]}
+    if isinstance(compact_prop, tuple):
+        warnings.warn(
+            "compact_prop as a tuple will be deprecated in a future warning, use a dict instead",
+            FutureWarning,
+        )
+        compact_prop = {compact_prop[0]: compact_prop[1]}
 
     if compact:
         skip_dims = set(data.dims) - {"chain", "draw"}
     else:
         skip_dims = set()
 
     plotters = list(xarray_var_iter(data, var_names=var_names, combined=True, skip_dims=skip_dims))
```

### Comparing `arviz-0.8.3/arviz/plots/mcseplot.py` & `arviz-0.9.0/arviz/plots/mcseplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/elpdplot.py` & `arviz-0.9.0/arviz/plots/elpdplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/styles/arviz-whitegrid.mplstyle` & `arviz-0.9.0/arviz/plots/styles/arviz-whitegrid.mplstyle`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This style is based on Seaborn-whitegrid parameters, the main differences are
 # Default matplotlib font (no problem using Greek letters!)
 # Larger font size for several elements
 # Colorblind friendly color cycle
 figure.figsize: 7.2, 4.8
 figure.dpi: 100.0
 figure.facecolor: white
+figure.constrained_layout.use: True
 text.color: .15
 axes.labelcolor: .15
 legend.frameon: False
 legend.numpoints: 1
 legend.scatterpoints: 1
 xtick.direction: out
 ytick.direction: out
```

### Comparing `arviz-0.8.3/arviz/plots/styles/arviz-grayscale.mplstyle` & `arviz-0.9.0/arviz/plots/styles/arviz-grayscale.mplstyle`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # This style is based on Seaborn-white parameters, the main differences are
 # Default matplotlib font (no problem using Greek letters!)
 # Larger font size for several elements
 # Colorblind friendly color cycle
 figure.figsize: 7.2, 4.8
 figure.dpi: 100.0
 figure.facecolor: white
+figure.constrained_layout.use: True
 text.color: .15
 axes.labelcolor: .15
 legend.frameon: False
 legend.numpoints: 1
 legend.scatterpoints: 1
 xtick.direction: out
 ytick.direction: out
```

### Comparing `arviz-0.8.3/arviz/plots/styles/arviz-darkgrid.mplstyle` & `arviz-0.9.0/arviz/plots/styles/arviz-white.mplstyle`

 * *Files 11% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-# This style is based on Seaborn-darkgrid parameters, the main differences are
+# This style is based on Seaborn-white parameters, the main differences are
 # Default matplotlib font (no problem using Greek letters!)
 # Larger font size for several elements
 # Colorblind friendly color cycle
 figure.figsize: 7.2, 4.8
 figure.dpi: 100.0
 figure.facecolor: white
+figure.constrained_layout.use: True
 text.color: .15
 axes.labelcolor: .15
 legend.frameon: False
 legend.numpoints: 1
 legend.scatterpoints: 1
 xtick.direction: out
 ytick.direction: out
 xtick.color: .15
 ytick.color: .15
 axes.axisbelow: True
-grid.linestyle: -
 lines.solid_capstyle: round
 
 axes.labelsize: 15
 axes.titlesize: 16
 xtick.labelsize: 14
 ytick.labelsize: 14
 legend.fontsize: 14
 
-axes.grid: True
-axes.facecolor: eeeeee
-axes.edgecolor: white
-axes.linewidth: 0
-grid.color: white
+axes.grid: False
+axes.facecolor: white
+axes.edgecolor: 0
+axes.linewidth: 1
+axes.spines.top: False
+axes.spines.right: False
 image.cmap: viridis
 xtick.major.size: 0
 ytick.major.size: 0
 xtick.minor.size: 0
 ytick.minor.size: 0
 
 # color-blind friendly cycle designed using https://colorcyclepicker.mpetroff.net/
```

### Comparing `arviz-0.8.3/arviz/plots/styles/arviz-white.mplstyle` & `arviz-0.9.0/arviz/plots/styles/arviz-darkgrid.mplstyle`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,39 @@
-# This style is based on Seaborn-white parameters, the main differences are
+# This style is based on Seaborn-darkgrid parameters, the main differences are
 # Default matplotlib font (no problem using Greek letters!)
 # Larger font size for several elements
 # Colorblind friendly color cycle
 figure.figsize: 7.2, 4.8
 figure.dpi: 100.0
 figure.facecolor: white
+figure.constrained_layout.use: True
 text.color: .15
 axes.labelcolor: .15
 legend.frameon: False
 legend.numpoints: 1
 legend.scatterpoints: 1
 xtick.direction: out
 ytick.direction: out
 xtick.color: .15
 ytick.color: .15
 axes.axisbelow: True
+grid.linestyle: -
 lines.solid_capstyle: round
 
 axes.labelsize: 15
 axes.titlesize: 16
 xtick.labelsize: 14
 ytick.labelsize: 14
 legend.fontsize: 14
 
-axes.grid: False
-axes.facecolor: white
-axes.edgecolor: 0
-axes.linewidth: 1
-axes.spines.top: False
-axes.spines.right: False
+axes.grid: True
+axes.facecolor: eeeeee
+axes.edgecolor: white
+axes.linewidth: 0
+grid.color: white
 image.cmap: viridis
 xtick.major.size: 0
 ytick.major.size: 0
 xtick.minor.size: 0
 ytick.minor.size: 0
 
 # color-blind friendly cycle designed using https://colorcyclepicker.mpetroff.net/
```

### Comparing `arviz-0.8.3/arviz/plots/violinplot.py` & `arviz-0.9.0/arviz/plots/violinplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/__init__.py` & `arviz-0.9.0/arviz/plots/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/jointplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/jointplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/__init__.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/__init__.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/essplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/essplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/forestplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/forestplot.py`

 * *Files 1% similar despite different names*

```diff
@@ -337,15 +337,15 @@
                     y,
                     "o",
                     mfc=ax.get_facecolor(),
                     markersize=markersize * 0.75,
                     color=color,
                 )
         ax.tick_params(labelsize=xt_labelsize)
-        ax.set_title("{:.1%} hdi".format(hdi_prob), fontsize=titlesize, wrap=True)
+        ax.set_title("{:.1%} HDI".format(hdi_prob), fontsize=titlesize, wrap=True)
         if rope is None or isinstance(rope, dict):
             return
         elif len(rope) == 2:
             ax.axvspan(rope[0], rope[1], 0, self.y_max(), color="C2", alpha=0.5)
         else:
             raise ValueError(
                 "Argument `rope` must be None, a dictionary like"
```

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/rankplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/rankplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/compareplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/compareplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/hdiplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/hdiplot.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """Matplotlib hdiplot."""
-import warnings
 import matplotlib.pyplot as plt
 
-from . import backend_show
+from . import backend_kwarg_defaults, backend_show
 
 
 def plot_hdi(ax, x_data, y_data, plot_kwargs, fill_kwargs, backend_kwargs, show):
-    """Matplotlib hdi plot."""
-    if backend_kwargs is not None:
-        warnings.warn(
-            (
-                "Argument backend_kwargs has not effect in matplotlib.plot_hdi"
-                "Supplied value won't be used"
-            )
-        )
+    """Matplotlib HDI plot."""
+    if backend_kwargs is None:
+        backend_kwargs = {}
+
+    backend_kwargs = {
+        **backend_kwarg_defaults(),
+        **backend_kwargs,
+    }
     if ax is None:
-        ax = plt.gca()
+        _, ax = plt.subplots(1, 1, **backend_kwargs)
+
     ax.plot(x_data, y_data, **plot_kwargs)
     ax.fill_between(x_data, y_data[:, 0], y_data[:, 1], **fill_kwargs)
 
     if backend_show(show):
         plt.show()
 
     return ax
```

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/densityplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/densityplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/pairplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/pairplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/energyplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/energyplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/parallelplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/parallelplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/ppcplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/ppcplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-"""Matplotib Posterior predictive plot."""
+"""Matplotlib Posterior predictive plot."""
 import platform
 import logging
 from matplotlib import animation, get_backend
 import matplotlib.pyplot as plt
 import numpy as np
 
 from . import backend_show
```

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/loopitplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/loopitplot.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Matplotlib loopitplot."""
 import matplotlib.pyplot as plt
 import numpy as np
 
 from . import backend_kwarg_defaults, backend_show
 from ....numeric_utils import _fast_kde
-from ...hdiplot import plot_hdi
 
 
 def plot_loo_pit(
     ax,
     figsize,
     ecdf,
     loo_pit,
@@ -16,16 +15,16 @@
     unif_ecdf,
     p975,
     p025,
     fill_kwargs,
     ecdf_fill,
     use_hdi,
     x_vals,
-    unif_densities,
     hdi_kwargs,
+    hdi_odds,
     n_unif,
     unif,
     plot_unif_kwargs,
     loo_pit_kde,
     xt_labelsize,
     legend,
     credible_interval,
@@ -50,22 +49,28 @@
         )
 
         if ecdf_fill:
             ax.fill_between(unif_ecdf, p975 - unif_ecdf, p025 - unif_ecdf, **fill_kwargs)
         else:
             ax.plot(unif_ecdf, p975 - unif_ecdf, unif_ecdf, p025 - unif_ecdf, **plot_unif_kwargs)
     else:
+        x_ss = np.empty((n_unif, len(loo_pit_kde)))
+        u_dens = np.empty((n_unif, len(loo_pit_kde)))
         if use_hdi:
-            plot_hdi(x_vals, unif_densities, **hdi_kwargs)
+            ax.axhspan(*hdi_odds, **hdi_kwargs)
         else:
             for idx in range(n_unif):
-                unif_density, _, _ = _fast_kde(unif[idx, :], xmin=0, xmax=1)
-                ax.plot(x_vals, unif_density, **plot_unif_kwargs)
+                unif_density, xmin, xmax = _fast_kde(unif[idx, :])
+                x_s = np.linspace(xmin, xmax, len(unif_density))
+                x_ss[idx] = x_s
+                u_dens[idx] = unif_density
+            ax.plot(x_ss.T, u_dens.T, **plot_unif_kwargs)
         ax.plot(x_vals, loo_pit_kde, **plot_kwargs)
-
+        ax.set_xlim(0, 1)
+        ax.set_ylim(0, None)
     ax.tick_params(labelsize=xt_labelsize)
     if legend:
         if not (use_hdi or (ecdf and ecdf_fill)):
             label = "{:.3g}% credible interval".format(credible_interval) if ecdf else "Uniform"
             ax.plot([], label=label, **plot_unif_kwargs)
         ax.legend()
```

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/distplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/distplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/autocorrplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/autocorrplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/khatplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/khatplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/kdeplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/kdeplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/traceplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/traceplot.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import matplotlib.pyplot as plt
 from matplotlib.lines import Line2D
 import numpy as np
 
 from . import backend_kwarg_defaults, backend_show
 from ...distplot import plot_dist
 from ...rankplot import plot_rank
-from ...plot_utils import _scale_fig_size, make_label, format_coords_as_labels
+from ...plot_utils import _scale_fig_size, make_label, format_coords_as_labels, _dealiase_sel_kwargs
 from ....numeric_utils import get_bins
 
 
 def plot_trace(
     data,
     var_names,  # pylint: disable=unused-argument
     divergences,
@@ -154,82 +154,83 @@
             )
 
     for idx, (var_name, selection, value) in enumerate(plotters):
         value = np.atleast_2d(value)
 
         if len(value.shape) == 2:
             if compact_prop:
-                plot_kwargs[compact_prop[0]] = compact_prop[1][0]
-                trace_kwargs[compact_prop[0]] = compact_prop[1][0]
+                aux_plot_kwargs = _dealiase_sel_kwargs(plot_kwargs, compact_prop, 0)
+                aux_trace_kwargs = _dealiase_sel_kwargs(trace_kwargs, compact_prop, 0)
+            else:
+                aux_plot_kwargs = plot_kwargs
+                aux_trace_kwargs = trace_kwargs
             _plot_chains_mpl(
                 axes,
                 idx,
                 value,
                 data,
                 chain_prop,
                 combined,
                 xt_labelsize,
                 rug,
                 kind,
-                trace_kwargs,
+                aux_trace_kwargs,
                 hist_kwargs,
-                plot_kwargs,
+                aux_plot_kwargs,
                 fill_kwargs,
                 rug_kwargs,
                 rank_kwargs,
             )
-            if compact_prop:
-                plot_kwargs.pop(compact_prop[0])
-                trace_kwargs.pop(compact_prop[0])
         else:
             sub_data = data[var_name].sel(**selection)
             legend_labels = format_coords_as_labels(sub_data, skip_dims=("chain", "draw"))
             legend_title = ", ".join(
                 [
                     "{}".format(coord_name)
                     for coord_name in sub_data.coords
                     if coord_name not in {"chain", "draw"}
                 ]
             )
             value = value.reshape((value.shape[0], value.shape[1], -1))
-            compact_prop_cycle = cycle(compact_prop[1])
+            compact_prop_iter = {
+                prop_name: [prop for _, prop in zip(range(value.shape[2]), cycle(props))]
+                for prop_name, props in compact_prop.items()
+            }
             handles = []
-            for sub_idx, label, prop in zip(
-                range(value.shape[2]), legend_labels, compact_prop_cycle
-            ):
-                if compact_prop:
-                    plot_kwargs[compact_prop[0]] = prop
-                    trace_kwargs[compact_prop[0]] = prop
+            for sub_idx, label in zip(range(value.shape[2]), legend_labels):
+                aux_plot_kwargs = _dealiase_sel_kwargs(plot_kwargs, compact_prop_iter, sub_idx)
+                aux_trace_kwargs = _dealiase_sel_kwargs(trace_kwargs, compact_prop_iter, sub_idx)
                 _plot_chains_mpl(
                     axes,
                     idx,
                     value[..., sub_idx],
                     data,
                     chain_prop,
                     combined,
                     xt_labelsize,
                     rug,
                     kind,
-                    trace_kwargs,
+                    aux_trace_kwargs,
                     hist_kwargs,
-                    plot_kwargs,
+                    aux_plot_kwargs,
                     fill_kwargs,
                     rug_kwargs,
                     rank_kwargs,
                 )
                 if legend:
                     handles.append(
                         Line2D(
-                            [], [], label=label, **{chain_prop[0]: chain_prop[1][0]}, **plot_kwargs
+                            [],
+                            [],
+                            label=label,
+                            **_dealiase_sel_kwargs(aux_plot_kwargs, chain_prop, 0)
                         )
                     )
             if legend:
                 axes[idx, 0].legend(handles=handles, title=legend_title)
-            plot_kwargs.pop(compact_prop[0], None)
-            trace_kwargs.pop(compact_prop[0], None)
 
         if value[0].dtype.kind == "i":
             xticks = get_bins(value)
             axes[idx, 0].set_xticks(xticks[:-1])
         axes[idx, 0].set_yticks([])
         for col in (0, 1):
             axes[idx, col].set_title(make_label(var_name, selection), fontsize=titlesize, wrap=True)
@@ -260,27 +261,27 @@
                             np.zeros_like(div_idxs) + ylocs[1],
                             marker="|",
                             color="black",
                             markeredgewidth=1.5,
                             markersize=30,
                             linestyle="None",
                             alpha=hist_kwargs["alpha"],
-                            zorder=-5,
+                            zorder=0.6,
                         )
                         axes[idx, 1].set_ylim(*ylims[1])
                     axes[idx, 0].plot(
                         values,
                         np.zeros_like(values) + ylocs[0],
                         marker="|",
                         color="black",
                         markeredgewidth=1.5,
                         markersize=30,
                         linestyle="None",
                         alpha=trace_kwargs["alpha"],
-                        zorder=-5,
+                        zorder=0.6,
                     )
                     axes[idx, 0].set_ylim(*ylims[0])
 
         for _, _, vlines in (j for j in lines if j[0] == var_name and j[1] == selection):
             if isinstance(vlines, (float, int)):
                 line_values = [vlines]
             else:
@@ -294,32 +295,34 @@
                 axes[idx, 1].hlines(
                     line_values,
                     *xlims[1],
                     colors="black",
                     linewidth=1.5,
                     alpha=trace_kwargs["alpha"]
                 )
-        axes[idx, 0].set_ylim(bottom=0, top=ylims[0][1])
+        axes[idx, 0].set_ylim(ylims[0])
         if kind == "trace":
             axes[idx, 1].set_xlim(left=data.draw.min(), right=data.draw.max())
             axes[idx, 1].set_ylim(*ylims[1])
     if legend:
         legend_kwargs = trace_kwargs if combined else plot_kwargs
         handles = [
-            Line2D([], [], label=chain_id, **{chain_prop[0]: prop}, **legend_kwargs)
-            for chain_id, prop in zip(data.chain.values, chain_prop[1])
+            Line2D(
+                [], [], label=chain_id, **_dealiase_sel_kwargs(legend_kwargs, chain_prop, chain_id)
+            )
+            for chain_id in range(data.dims["chain"])
         ]
         if combined:
             handles.insert(
                 0,
                 Line2D(
-                    [], [], label="combined", **{chain_prop[0]: chain_prop[1][-1]}, **plot_kwargs
+                    [], [], label="combined", **_dealiase_sel_kwargs(plot_kwargs, chain_prop, -1)
                 ),
             )
-        axes[0, 0].legend(handles=handles, title="chain")
+        axes[0, 0].legend(handles=handles, title="chain", loc="upper right")
 
     if backend_show(show):
         plt.show()
 
     return axes
 
 
@@ -338,47 +341,44 @@
     plot_kwargs,
     fill_kwargs,
     rug_kwargs,
     rank_kwargs,
 ):
     for chain_idx, row in enumerate(value):
         if kind == "trace":
-            axes[idx, 1].plot(
-                data.draw.values, row, **{chain_prop[0]: chain_prop[1][chain_idx]}, **trace_kwargs
-            )
+            aux_kwargs = _dealiase_sel_kwargs(trace_kwargs, chain_prop, chain_idx)
+            axes[idx, 1].plot(data.draw.values, row, **aux_kwargs)
 
         if not combined:
-            plot_kwargs[chain_prop[0]] = chain_prop[1][chain_idx]
+            aux_kwargs = _dealiase_sel_kwargs(plot_kwargs, chain_prop, chain_idx)
             plot_dist(
                 values=row,
                 textsize=xt_labelsize,
                 rug=rug,
                 ax=axes[idx, 0],
                 hist_kwargs=hist_kwargs,
-                plot_kwargs=plot_kwargs,
+                plot_kwargs=aux_kwargs,
                 fill_kwargs=fill_kwargs,
                 rug_kwargs=rug_kwargs,
                 backend="matplotlib",
                 show=False,
             )
-            plot_kwargs.pop(chain_prop[0])
 
     if kind == "rank_bars":
         plot_rank(data=value, kind="bars", ax=axes[idx, 1], **rank_kwargs)
     elif kind == "rank_vlines":
         plot_rank(data=value, kind="vlines", ax=axes[idx, 1], **rank_kwargs)
 
     if combined:
-        plot_kwargs[chain_prop[0]] = chain_prop[1][-1]
+        aux_kwargs = _dealiase_sel_kwargs(plot_kwargs, chain_prop, -1)
         plot_dist(
             values=value.flatten(),
             textsize=xt_labelsize,
             rug=rug,
             ax=axes[idx, 0],
             hist_kwargs=hist_kwargs,
-            plot_kwargs=plot_kwargs,
+            plot_kwargs=aux_kwargs,
             fill_kwargs=fill_kwargs,
             rug_kwargs=rug_kwargs,
             backend="matplotlib",
             show=False,
         )
-        plot_kwargs.pop(chain_prop[0])
```

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/mcseplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/mcseplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/elpdplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/elpdplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/violinplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/violinplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/matplotlib/posteriorplot.py` & `arviz-0.9.0/arviz/plots/backends/matplotlib/posteriorplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/jointplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/jointplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/__init__.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/__init__.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/essplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/essplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/forestplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/forestplot.py`

 * *Files 0% similar despite different names*

```diff
@@ -413,15 +413,15 @@
                     ax.line(
                         [values[j], values[-(j + 1)]], [y, y], line_width=width, line_color=color
                     )
                 ax.circle(
                     x=values[mid], y=y, size=markersize * 0.75, fill_color=color,
                 )
         _title = Title()
-        _title.text = "{:.1%} hdi".format(hdi_prob)
+        _title.text = "{:.1%} HDI".format(hdi_prob)
         ax.title = _title
 
         return ax
 
     def plot_neff(self, ax, markersize):
         """Draw effective n for each plotter."""
         max_ess = 0
```

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/rankplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/rankplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/compareplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/compareplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/densityplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/densityplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/pairplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/pairplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/energyplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/energyplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/parallelplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/parallelplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/ppcplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/ppcplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/loopitplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/loopitplot.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Bokeh loopitplot."""
 import bokeh.plotting as bkp
+from bokeh.models import BoxAnnotation
 import numpy as np
 
 from . import backend_kwarg_defaults
 from .. import show_layout
-from ...hdiplot import plot_hdi
 from ...kdeplot import _fast_kde
 
 
 def plot_loo_pit(
     ax,
     figsize,
     ecdf,
@@ -17,16 +17,16 @@
     unif_ecdf,
     p975,
     p025,
     fill_kwargs,
     ecdf_fill,
     use_hdi,
     x_vals,
-    unif_densities,
     hdi_kwargs,
+    hdi_odds,
     n_unif,
     unif,
     plot_unif_kwargs,
     loo_pit_kde,
     plot_kwargs,
     backend_kwargs,
     show,
@@ -39,15 +39,15 @@
         **backend_kwarg_defaults(("dpi", "plot.bokeh.figure.dpi"),),
         **backend_kwargs,
     }
     dpi = backend_kwargs.pop("dpi")
     if ax is None:
         backend_kwargs.setdefault("width", int(figsize[0] * dpi))
         backend_kwargs.setdefault("height", int(figsize[1] * dpi))
-        ax = bkp.figure(**backend_kwargs)
+        ax = bkp.figure(x_range=(0, 1), **backend_kwargs)
 
     if ecdf:
         if plot_kwargs.get("drawstyle") == "steps-mid":
             ax.step(
                 np.hstack((0, loo_pit, 1)),
                 np.hstack((0, loo_pit - loo_pit_ecdf, 0)),
                 line_color=plot_kwargs.get("color", "black"),
@@ -111,28 +111,29 @@
                     p025 - unif_ecdf,
                     line_color=plot_unif_kwargs.get("color", "black"),
                     line_alpha=plot_unif_kwargs.get("alpha", 1.0),
                     line_width=plot_unif_kwargs.get("linewidth", 1.0),
                 )
     else:
         if use_hdi:
-            plot_hdi(
-                x_vals,
-                unif_densities,
-                backend="bokeh",
-                ax=ax,
-                backend_kwargs={},
-                show=False,
-                **hdi_kwargs
+            ax.add_layout(
+                BoxAnnotation(
+                    bottom=hdi_odds[1],
+                    top=hdi_odds[0],
+                    fill_alpha=hdi_kwargs.pop("alpha"),
+                    fill_color=hdi_kwargs.pop("color"),
+                    **hdi_kwargs
+                )
             )
         else:
             for idx in range(n_unif):
-                unif_density, _, _ = _fast_kde(unif[idx, :], xmin=0, xmax=1)
+                unif_density, xmin, xmax = _fast_kde(unif[idx, :])
+                x_s = np.linspace(xmin, xmax, len(unif_density))
                 ax.line(
-                    x_vals,
+                    x_s,
                     unif_density,
                     line_color=plot_unif_kwargs.get("color", "black"),
                     line_alpha=plot_unif_kwargs.get("alpha", 0.1),
                     line_width=plot_unif_kwargs.get("linewidth", 1.0),
                 )
         ax.line(
             x_vals,
```

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/distplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/distplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/autocorrplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/autocorrplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/khatplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/khatplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/kdeplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/kdeplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/traceplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/traceplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from bokeh.models.annotations import Title
 import numpy as np
 
 from . import backend_kwarg_defaults
 from .. import show_layout
 from ...distplot import plot_dist
 from ...rankplot import plot_rank
-from ...plot_utils import xarray_var_iter, make_label, _scale_fig_size
+from ...plot_utils import xarray_var_iter, make_label, _scale_fig_size, _dealiase_sel_kwargs
 from ....rcparams import rcParams
 
 
 def plot_trace(
     data,
     var_names,
     divergences,
@@ -296,63 +296,58 @@
         if kind == "trace":
             if legend:
                 trace_kwargs["legend_label"] = "chain {}".format(chain_idx)
             ax_trace.line(
                 x=x_name,
                 y=y_name,
                 source=cds,
-                **{chain_prop[0]: chain_prop[1][chain_idx]},
-                **trace_kwargs,
+                **_dealiase_sel_kwargs(trace_kwargs, chain_prop, chain_idx)
             )
             if marker:
                 ax_trace.circle(
                     x=x_name,
                     y=y_name,
                     source=cds,
                     radius=0.30,
                     alpha=0.5,
-                    **{chain_prop[0]: chain_prop[1][chain_idx],},
+                    **_dealiase_sel_kwargs({}, chain_prop, chain_idx)
                 )
         if not combined:
             rug_kwargs["cds"] = cds
             if legend:
                 plot_kwargs["legend_label"] = "chain {}".format(chain_idx)
-            plot_kwargs[chain_prop[0]] = chain_prop[1][chain_idx]
             plot_dist(
                 cds.data[y_name],
                 ax=ax_density,
                 rug=rug,
                 hist_kwargs=hist_kwargs,
-                plot_kwargs=plot_kwargs,
+                plot_kwargs=_dealiase_sel_kwargs(plot_kwargs, chain_prop, chain_idx),
                 fill_kwargs=fill_kwargs,
                 rug_kwargs=rug_kwargs,
                 backend="bokeh",
                 backend_kwargs={},
                 show=False,
             )
-            plot_kwargs.pop(chain_prop[0])
 
     if kind == "rank_bars":
         value = np.array([item.data[y_name] for item in data.values()])
         plot_rank(value, kind="bars", ax=ax_trace, backend="bokeh", show=False, **rank_kwargs)
     elif kind == "rank_vlines":
         value = np.array([item.data[y_name] for item in data.values()])
         plot_rank(value, kind="vlines", ax=ax_trace, backend="bokeh", show=False, **rank_kwargs)
 
     if combined:
         rug_kwargs["cds"] = data
         if legend:
             plot_kwargs["legend_label"] = "combined chains"
-        plot_kwargs[chain_prop[0]] = chain_prop[1][-1]
         plot_dist(
             np.concatenate([item.data[y_name] for item in data.values()]).flatten(),
             ax=ax_density,
             rug=rug,
             hist_kwargs=hist_kwargs,
-            plot_kwargs=plot_kwargs,
+            plot_kwargs=_dealiase_sel_kwargs(plot_kwargs, chain_prop, -1),
             fill_kwargs=fill_kwargs,
             rug_kwargs=rug_kwargs,
             backend="bokeh",
             backend_kwargs={},
             show=False,
         )
-        plot_kwargs.pop(chain_prop[0])
```

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/mcseplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/mcseplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/elpdplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/elpdplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/violinplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/violinplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/backends/bokeh/posteriorplot.py` & `arviz-0.9.0/arviz/plots/backends/bokeh/posteriorplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/plots/posteriorplot.py` & `arviz-0.9.0/arviz/plots/posteriorplot.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/__init__.py` & `arviz-0.9.0/arviz/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # pylint: disable=wildcard-import,invalid-name,wrong-import-position
 """ArviZ is a library for exploratory analysis of Bayesian models."""
-__version__ = "0.8.3"
+__version__ = "0.9.0"
 
 import os
 import logging
 from matplotlib.pyplot import style, register_cmap
 from matplotlib.colors import LinearSegmentedColormap
```

### Comparing `arviz-0.8.3/arviz/numeric_utils.py` & `arviz-0.9.0/arviz/numeric_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,15 +184,15 @@
     # Sturges histogram bin estimator
     bins_sturges = (x_max - x_min) / (np.log2(values.size) + 1)
 
     # The Freedman-Diaconis histogram bin estimator.
     iqr = np.subtract(*np.percentile(values, [75, 25]))  # pylint: disable=assignment-from-no-return
     bins_fd = 2 * iqr * values.size ** (-1 / 3)
 
-    width = round(np.max([1, bins_sturges, bins_fd])).astype(int)
+    width = np.round(np.max([1, bins_sturges, bins_fd])).astype(int)
 
     return np.arange(x_min, x_max + width + 1, width)
 
 
 def _sturges_formula(dataset, mult=1):
     """Use Sturges' formula to determine number of bins.
```

### Comparing `arviz-0.8.3/arviz/data/__init__.py` & `arviz-0.9.0/arviz/data/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from .io_netcdf import from_netcdf, to_netcdf
 from .datasets import load_arviz_data, list_datasets, clear_data_home
 from .base import numpy_to_data_array, dict_to_dataset, CoordSpec, DimSpec
 from .converters import convert_to_dataset, convert_to_inference_data
 from .io_cmdstan import from_cmdstan
 from .io_cmdstanpy import from_cmdstanpy
 from .io_dict import from_dict
+from .io_pyjags import from_pyjags
 from .io_pymc3 import from_pymc3, from_pymc3_predictions
 from .io_pystan import from_pystan
 from .io_emcee import from_emcee
 from .io_pyro import from_pyro
 from .io_numpyro import from_numpyro
 from .io_tfp import from_tfp
 
@@ -20,14 +21,15 @@
     "load_arviz_data",
     "list_datasets",
     "clear_data_home",
     "numpy_to_data_array",
     "dict_to_dataset",
     "convert_to_dataset",
     "convert_to_inference_data",
+    "from_pyjags",
     "from_pymc3",
     "from_pymc3_predictions",
     "from_pystan",
     "from_emcee",
     "from_cmdstan",
     "from_cmdstanpy",
     "from_dict",
```

### Comparing `arviz-0.8.3/arviz/data/io_cmdstanpy.py` & `arviz-0.9.0/arviz/data/io_cmdstanpy.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/data/datasets.py` & `arviz-0.9.0/arviz/data/datasets.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/data/io_numpyro.py` & `arviz-0.9.0/arviz/data/io_numpyro.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/data/io_pyro.py` & `arviz-0.9.0/arviz/data/io_pyro.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """Pyro-specific conversion code."""
 import logging
+import warnings
 import numpy as np
 from packaging import version
 import xarray as xr
 
 from .inference_data import InferenceData
 from .base import requires, dict_to_dataset, generate_dims_coords, make_attrs
 from .. import utils
@@ -22,14 +23,15 @@
 
     def __init__(
         self,
         *,
         posterior=None,
         prior=None,
         posterior_predictive=None,
+        log_likelihood=True,
         predictions=None,
         constant_data=None,
         predictions_constant_data=None,
         coords=None,
         dims=None,
         pred_dims=None,
         num_chains=1,
@@ -58,14 +60,15 @@
             Dims for predictions data. Map variable names to their coordinates.
         num_chains: int
             Number of chains used for sampling. Ignored if posterior is present.
         """
         self.posterior = posterior
         self.prior = prior
         self.posterior_predictive = posterior_predictive
+        self.log_likelihood = log_likelihood
         self.predictions = predictions
         self.constant_data = constant_data
         self.predictions_constant_data = predictions_constant_data
         self.coords = coords
         self.dims = dims
         self.pred_dims = pred_dims
         import pyro
@@ -126,27 +129,33 @@
         data = {"diverging": diverging}
         return dict_to_dataset(data, library=self.pyro, coords=self.coords, dims=None)
 
     @requires("posterior")
     @requires("model")
     def log_likelihood_to_xarray(self):
         """Extract log likelihood from Pyro posterior."""
+        if not self.log_likelihood:
+            return None
         data = {}
         if self.observations is not None:
             try:
                 samples = self.posterior.get_samples(group_by_chain=False)
                 predictive = self.pyro.infer.Predictive(self.model, samples)
                 vectorized_trace = predictive.get_vectorized_trace(*self._args, **self._kwargs)
                 for obs_name in self.observations.keys():
                     obs_site = vectorized_trace.nodes[obs_name]
                     log_like = obs_site["fn"].log_prob(obs_site["value"]).detach().cpu().numpy()
                     shape = (self.nchains, self.ndraws) + log_like.shape[1:]
                     data[obs_name] = np.reshape(log_like, shape)
             except:  # pylint: disable=bare-except
                 # cannot get vectorized trace
+                warnings.warn(
+                    "Could not get vectorized trace, log_likelihood group will be omitted. "
+                    "Check your model vectorization or set log_likelihood=False"
+                )
                 return None
         return dict_to_dataset(data, library=self.pyro, coords=self.coords, dims=self.dims)
 
     def translate_posterior_predictive_dict_to_xarray(self, dct, dims):
         """Convert posterior_predictive or prediction samples to xarray."""
         data = {}
         for k, ary in dct.items():
@@ -269,14 +278,15 @@
 
 
 def from_pyro(
     posterior=None,
     *,
     prior=None,
     posterior_predictive=None,
+    log_likelihood=True,
     predictions=None,
     constant_data=None,
     predictions_constant_data=None,
     coords=None,
     dims=None,
     pred_dims=None,
     num_chains=1,
@@ -290,14 +300,16 @@
     ----------
     posterior : pyro.infer.MCMC
         Fitted MCMC object from Pyro
     prior: dict
         Prior samples from a Pyro model
     posterior_predictive : dict
         Posterior predictive samples for the posterior
+    log_likelihood : bool, optional
+        Calculate and store pointwise log likelihood values.
     predictions: dict
         Out of sample predictions
     constant_data: dict
         Dictionary containing constant data variables mapped to their values.
     predictions_constant_data: dict
         Constant data used for out-of-sample predictions.
     coords : dict[str] -> list[str]
@@ -309,14 +321,15 @@
     num_chains: int
         Number of chains used for sampling. Ignored if posterior is present.
     """
     return PyroConverter(
         posterior=posterior,
         prior=prior,
         posterior_predictive=posterior_predictive,
+        log_likelihood=log_likelihood,
         predictions=predictions,
         constant_data=constant_data,
         predictions_constant_data=predictions_constant_data,
         coords=coords,
         dims=dims,
         pred_dims=pred_dims,
         num_chains=num_chains,
```

### Comparing `arviz-0.8.3/arviz/data/io_emcee.py` & `arviz-0.9.0/arviz/data/io_emcee.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/data/io_pymc3.py` & `arviz-0.9.0/arviz/data/io_pymc3.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """PyMC3-specific conversion code."""
 import logging
 import warnings
-from typing import Dict, List, Any, Optional, Iterable, Union, TYPE_CHECKING, Tuple
+from typing import Dict, List, Tuple, Any, Optional, Iterable, Union, TYPE_CHECKING
 from types import ModuleType
 
 import numpy as np
 import xarray as xr
 from .. import utils
 from .inference_data import InferenceData, concat
 from .base import requires, dict_to_dataset, generate_dims_coords, make_attrs, CoordSpec, DimSpec
@@ -82,15 +82,15 @@
             self.model = None
 
         if self.model is None:
             warnings.warn(
                 "Using `from_pymc3` without the model will be deprecated in a future release. "
                 "Not using the model will return less accurate and less useful results. "
                 "Make sure you use the model argument or call from_pymc3 within a model context.",
-                PendingDeprecationWarning,
+                FutureWarning,
             )
 
         # This next line is brittle and may not work forever, but is a secret
         # way to access the model from the trace.
         self.attrs = None
         if trace is not None:
             if self.model is None:
@@ -143,28 +143,38 @@
                     "When constructing InferenceData must have at least"
                     " one of trace, prior, posterior_predictive or predictions."
                 )
 
             aelem = arbitrary_element(get_from)
             self.ndraws = aelem.shape[0]
 
-        self.coords = coords
-        self.dims = dims
-        self.observations = self.find_observations()
+        self.coords = {} if coords is None else coords
+        if hasattr(self.model, "coords"):
+            self.coords = {**self.model.coords, **self.coords}
+
+        self.dims = {} if dims is None else dims
+        if hasattr(self.model, "RV_dims"):
+            model_dims = {k: list(v) for k, v in self.model.RV_dims.items()}
+            self.dims = {**model_dims, **self.dims}
 
-    def find_observations(self) -> Optional[Dict[str, Var]]:
+        self.observations, self.multi_observations = self.find_observations()
+
+    def find_observations(self) -> Tuple[Optional[Dict[str, Var]], Optional[Dict[str, Var]]]:
         """If there are observations available, return them as a dictionary."""
-        has_observations = False
-        if self.model is not None:
-            if any((hasattr(obs, "observations") for obs in self.model.observed_RVs)):
-                has_observations = True
-        if has_observations:
-            assert self.model is not None
-            return {obs.name: obs.observations for obs in self.model.observed_RVs}
-        return None
+        if self.model is None:
+            return (None, None)
+        observations = {}
+        multi_observations = {}
+        for obs in self.model.observed_RVs:
+            if hasattr(obs, "observations"):
+                observations[obs.name] = obs.observations
+            elif hasattr(obs, "data"):
+                for key, val in obs.data.items():
+                    multi_observations[key] = val.eval() if hasattr(val, "eval") else val
+        return observations, multi_observations
 
     def split_trace(self) -> Tuple[Union[None, MultiTrace], Union[None, MultiTrace]]:
         """Split MultiTrace object into posterior and warmup.
 
         Returns
         -------
         trace_posterior: pymc3.MultiTrace or None
@@ -357,26 +367,26 @@
                     library=self.pymc3,
                     coords=self.coords,
                     dims=self.dims,
                 )
             )
         return priors_dict
 
-    @requires("observations")
+    @requires(["observations", "multi_observations"])
     @requires("model")
     def observed_data_to_xarray(self):
         """Convert observed data to xarray."""
         if self.predictions:
             return None
         if self.dims is None:
             dims = {}
         else:
             dims = self.dims
         observed_data = {}
-        for name, vals in self.observations.items():
+        for name, vals in {**self.observations, **self.multi_observations}.items():
             if hasattr(vals, "get_value"):
                 vals = vals.get_value()
             vals = utils.one_de(vals)
             val_dims = dims.get(name)
             val_dims, coords = generate_dims_coords(
                 vals.shape, name, dims=val_dims, coords=self.coords
             )
```

### Comparing `arviz-0.8.3/arviz/data/io_dict.py` & `arviz-0.9.0/arviz/data/io_dict.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/data/io_netcdf.py` & `arviz-0.9.0/arviz/data/io_netcdf.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/data/inference_data.py` & `arviz-0.9.0/arviz/data/inference_data.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 """Data structure for using netcdf groups with xarray."""
 from collections import OrderedDict
 from collections.abc import Sequence
 from copy import copy as ccopy, deepcopy
 from datetime import datetime
+from html import escape
 import warnings
+import uuid
 
 import netCDF4 as nc
 import numpy as np
 import xarray as xr
+from xarray.core.options import OPTIONS
 
-from ..utils import _subset_list
+from ..utils import _subset_list, HtmlTemplate
 from ..rcparams import rcParams
 
 SUPPORTED_GROUPS = [
     "posterior",
     "posterior_predictive",
     "predictions",
     "log_likelihood",
@@ -121,22 +124,47 @@
             if save_warmup and dataset_warmup is not None:
                 if dataset_warmup:
                     key = "{}{}".format(WARMUP_TAG, key)
                     setattr(self, key, dataset_warmup)
                     self._groups_warmup.append(key)
 
     def __repr__(self):
-        """Make string representation of object."""
+        """Make string representation of InferenceData object."""
         msg = "Inference data with groups:\n\t> {options}".format(
             options="\n\t> ".join(self._groups)
         )
         if self._groups_warmup:
             msg += "\n\nWarmup iterations saved ({}*).".format(WARMUP_TAG)
         return msg
 
+    def _repr_html_(self):
+        """Make html representation of InferenceData object."""
+        display_style = OPTIONS["display_style"]
+        if display_style == "text":
+            html_repr = f"<pre>{escape(repr(self))}</pre>"
+        else:
+            elements = "".join(
+                [
+                    HtmlTemplate.element_template.format(
+                        group_id=group + str(uuid.uuid4()),
+                        group=group,
+                        xr_data=getattr(  # pylint: disable=protected-access
+                            self, group
+                        )._repr_html_(),
+                    )
+                    for group in self._groups_all
+                ]
+            )
+            formatted_html_template = HtmlTemplate.html_template.format(  # pylint: disable=possibly-unused-variable
+                elements
+            )
+            css_template = HtmlTemplate.css_template  # pylint: disable=possibly-unused-variable
+            html_repr = "%(formatted_html_template)s%(css_template)s" % locals()
+        return html_repr
+
     def __delattr__(self, group):
         """Delete a group from the InferenceData object."""
         if group in self._groups:
             self._groups.remove(group)
         elif group in self._groups_warmup:
             self._groups_warmup.remove(group)
         object.__delattr__(self, group)
@@ -342,28 +370,36 @@
             msg = " ".join(("groups:", f"{err}", "in InferenceData"))
             raise KeyError(msg)
         return group_names
 
     def map(self, fun, groups=None, filter_groups=None, inplace=False, args=None, **kwargs):
         """Apply a function to multiple groups.
 
+        Applies ``fun`` groupwise to the selected ``InferenceData`` groups and overwrites the
+        group with the result of the function.
+
         Parameters
         ----------
-        fun: callable
-            Function to be applied to each group.
-        groups: str or list of str, optional
+        fun : callable
+            Function to be applied to each group. Assumes the function is called as
+            ``fun(dataset, *args, **kwargs)``.
+        groups : str or list of str, optional
             Groups where the selection is to be applied. Can either be group names
             or metagroup names.
-        inplace: bool, optional
+        filter_groups : {None, "like", "regex"}, optional
+            If `None` (default), interpret var_names as the real variables names. If "like",
+            interpret var_names as substrings of the real variables names. If "regex",
+            interpret var_names as regular expressions on the real variables names. A la
+            `pandas.filter`.
+        inplace : bool, optional
             If ``True``, modify the InferenceData object inplace,
             otherwise, return the modified copy.
-        args: array_like, optional
-            Positional arguments passed to ``fun``. Assumes the function is called as
-            ``fun(dataset, *args, **kwargs)``.
-        **kwargs: mapping, optional
+        args : array_like, optional
+            Positional arguments passed to ``fun``.
+        **kwargs : mapping, optional
             Keyword arguments passed to ``fun``.
 
         Returns
         -------
         InferenceData
             A new InferenceData object by default.
             When `inplace==True` perform selection in place and return `None`
@@ -372,18 +408,48 @@
         --------
         Shift observed_data, prior_predictive and posterior_predictive.
 
         .. ipython::
 
             In [1]: import arviz as az
                ...: idata = az.load_arviz_data("non_centered_eight")
-               ...: idata_shifted_obs = idata.map(lambda x: x + 3, groups="observed_RVs")
+               ...: idata_shifted_obs = idata.map(lambda x: x + 3, groups="observed_vars")
                ...: print(idata_shifted_obs.observed_data)
                ...: print(idata_shifted_obs.posterior_predictive)
 
+        Rename and update the coordinate values in both posterior and prior groups.
+
+        .. ipython::
+
+            In [1]: idata = az.load_arviz_data("radon")
+               ...: idata = idata.map(
+               ...:     lambda ds: ds.rename({"gamma_dim_0": "uranium_coefs"}).assign(
+               ...:         uranium_coefs=["intercept", "u_slope", "xbar_slope"]
+               ...:     ),
+               ...:     groups=["posterior", "prior"]
+               ...: )
+               ...: idata.posterior
+
+        Add extra coordinates to all groups containing observed variables
+
+        .. ipython::
+
+            In [1]: idata = az.load_arviz_data("rugby")
+               ...: home_team, away_team = np.array([
+               ...:     m.split() for m in idata.observed_data.match.values
+               ...: ]).T
+               ...: idata = idata.map(
+               ...:     lambda ds, **kwargs: ds.assign_coords(**kwargs),
+               ...:     groups="observed_vars",
+               ...:     home_team=("match", home_team),
+               ...:     away_team=("match", away_team),
+               ...: )
+               ...: print(idata.posterior_predictive)
+               ...: print(idata.observed_data)
+
         """
         if args is None:
             args = []
         groups = self._group_names(groups, filter_groups)
 
         out = self if inplace else deepcopy(self)
         for group in groups:
@@ -423,15 +489,15 @@
         --------
         Compute the mean of `posterior_groups`:
 
         .. ipython::
 
             In [1]: import arviz as az
                ...: idata = az.load_arviz_data("non_centered_eight")
-               ...: idata_means = idata._wrap_xarray_method("mean", groups="latent_RVs")
+               ...: idata_means = idata._wrap_xarray_method("mean", groups="latent_vars")
                ...: print(idata_means.posterior)
                ...: print(idata_means.observed_data)
 
         .. ipython::
 
             In [1]: idata_stack = idata._wrap_xarray_method(
                ...:     "stack",
```

### Comparing `arviz-0.8.3/arviz/data/converters.py` & `arviz-0.9.0/arviz/data/converters.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/data/_datasets/non_centered_eight.nc` & `arviz-0.9.0/arviz/data/_datasets/non_centered_eight.nc`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/data/_datasets/centered_eight.nc` & `arviz-0.9.0/arviz/data/_datasets/centered_eight.nc`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/data/base.py` & `arviz-0.9.0/arviz/data/base.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/data/io_cmdstan.py` & `arviz-0.9.0/arviz/data/io_cmdstan.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/data/io_tfp.py` & `arviz-0.9.0/arviz/data/io_tfp.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/data/io_pystan.py` & `arviz-0.9.0/arviz/data/io_pystan.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/base_tests/test_helpers.py` & `arviz-0.9.0/arviz/tests/base_tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/base_tests/test_stats_numba.py` & `arviz-0.9.0/arviz/tests/base_tests/test_stats_numba.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/base_tests/test_plots_bokeh.py` & `arviz-0.9.0/arviz/tests/base_tests/test_plots_bokeh.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,19 +31,20 @@
     plot_khat,
     plot_loo_pit,
     plot_mcse,
     plot_pair,
     plot_parallel,
     plot_posterior,
     plot_ppc,
+    plot_dist_comparison,
     plot_rank,
     plot_trace,
     plot_violin,
 )
-from ...stats import compare, loo, waic  # pylint: disable=wrong-import-position
+from ...stats import compare, loo, waic, hdi  # pylint: disable=wrong-import-position
 
 # Skip tests if bokeh not installed
 bkp = importorskip("bokeh.plotting")  # pylint: disable=invalid-name
 
 
 rcParams["data.load"] = "eager"
 
@@ -122,16 +123,16 @@
 
 @pytest.mark.parametrize(
     "kwargs",
     [
         {},
         {"var_names": "mu"},
         {"var_names": ["mu", "tau"]},
-        {"combined": True},
-        {"compact": True},
+        {"combined": True, "rug": True},
+        {"compact": True, "legend": True},
         {"combined": True, "compact": True, "legend": True},
         {"divergences": "top"},
         {"divergences": False},
         {"kind": "rank_vlines"},
         {"kind": "rank_bars"},
         {"lines": [("mu", {}, [1, 2])]},
         {"lines": [("mu", {}, 8)]},
@@ -478,24 +479,28 @@
         )
 
 
 @pytest.mark.parametrize(
     "kwargs",
     [
         {"color": "C5", "circular": True},
-        {"fill_kwargs": {"alpha": 0}},
+        {"hdi_data": True, "fill_kwargs": {"alpha": 0}},
         {"plot_kwargs": {"alpha": 0}},
         {"smooth_kwargs": {"window_length": 33, "polyorder": 5, "mode": "mirror"}},
-        {"smooth": False},
+        {"hdi_data": True, "smooth": False, "color": "xkcd:jade"},
     ],
 )
 def test_plot_hdi(models, data, kwargs):
-    axis = plot_hdi(
-        data["y"], models.model_1.posterior["theta"], backend="bokeh", show=False, **kwargs
-    )
+    hdi_data = kwargs.pop("hdi_data", None)
+    y_data = models.model_1.posterior["theta"]
+    if hdi_data:
+        hdi_data = hdi(y_data)
+        axis = plot_hdi(data["y"], hdi_data=hdi_data, backend="bokeh", show=False, **kwargs)
+    else:
+        axis = plot_hdi(data["y"], y_data, backend="bokeh", show=False, **kwargs)
     assert axis
 
 
 @pytest.mark.parametrize("kind", ["scatter", "hexbin", "kde"])
 def test_plot_joint(models, kind):
     axes = plot_joint(
         models.model_1, var_names=("mu", "tau"), kind=kind, backend="bokeh", show=False
@@ -599,16 +604,16 @@
 
 @pytest.mark.parametrize(
     "kwargs",
     [
         {},
         {"n_unif": 50},
         {"use_hdi": True, "color": "gray"},
-        {"use_hdi": True, "credible_interval": 0.68, "plot_kwargs": {"alpha": 0.9}},
-        {"use_hdi": True, "hdi_kwargs": {"smooth": False}},
+        {"use_hdi": True, "credible_interval": 0.68},
+        {"use_hdi": True, "hdi_kwargs": {"line_dash": "dashed", "alpha": 0}},
         {"ecdf": True},
         {"ecdf": True, "ecdf_fill": False, "plot_unif_kwargs": {"line_dash": "--"}},
         {"ecdf": True, "credible_interval": 0.97, "fill_kwargs": {"color": "red"}},
     ],
 )
 def test_plot_loo_pit(models, kwargs):
     axes = plot_loo_pit(idata=models.model_1, y="y", backend="bokeh", show=False, **kwargs)
@@ -952,7 +957,12 @@
         {"var_names": "mu", "ref_line": False},
         {"var_names": "mu", "kind": "vlines"},
     ],
 )
 def test_plot_rank(models, kwargs):
     axes = plot_rank(models.model_1, backend="bokeh", show=False, **kwargs)
     assert axes.shape
+
+
+def test_plot_dist_comparison_warn(models):
+    with pytest.raises(NotImplementedError, match="The bokeh backend.+Use matplotlib bakend."):
+        plot_dist_comparison(models.model_1, backend="bokeh")
```

### Comparing `arviz-0.8.3/arviz/tests/base_tests/test_stats.py` & `arviz-0.9.0/arviz/tests/base_tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/base_tests/test_diagnostics_numba.py` & `arviz-0.9.0/arviz/tests/base_tests/test_diagnostics_numba.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/base_tests/test_plots_matplotlib.py` & `arviz-0.9.0/arviz/tests/base_tests/test_plots_matplotlib.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 """Tests use the default backend."""
 # pylint: disable=redefined-outer-name,too-many-lines
 import os
 from copy import deepcopy
 import matplotlib.pyplot as plt
+from matplotlib import animation
 from pandas import DataFrame
 from scipy.stats import gaussian_kde
 import numpy as np
 import pytest
 
 from ...data import from_dict, load_arviz_data
-from ...stats import compare, loo, waic
+from ...stats import compare, loo, waic, hdi
 from ..helpers import (  # pylint: disable=unused-import
     eight_schools_params,
     models,
     create_model,
     multidim_models,
     create_multidimensional_model,
 )
@@ -25,14 +26,15 @@
     plot_ess,
     plot_posterior,
     plot_autocorr,
     plot_forest,
     plot_parallel,
     plot_pair,
     plot_joint,
+    plot_dist_comparison,
     plot_ppc,
     plot_violin,
     plot_compare,
     plot_kde,
     plot_khat,
     plot_hdi,
     plot_dist,
@@ -204,14 +206,21 @@
     "bad_kwargs", [{"var_names": ["mu", "tau"], "lines": [("mu", {}, ["hey"])]}]
 )
 def test_plot_trace_bad_lines_value(models, bad_kwargs):
     with pytest.raises(ValueError, match="line-positions should be numeric"):
         plot_trace(models.model_1, **bad_kwargs)
 
 
+@pytest.mark.parametrize("prop", ["chain_prop", "compact_prop"])
+def test_plot_trace_futurewarning(models, prop):
+    with pytest.warns(FutureWarning, match=f"{prop} as a tuple.+deprecated"):
+        ax = plot_trace(models.model_1, **{prop: ("ls", ("-", "--"))})
+    assert ax.shape
+
+
 @pytest.mark.parametrize("model_fits", [["model_1"], ["model_1", "model_2"]])
 @pytest.mark.parametrize(
     "args_expected",
     [
         ({}, 1),
         ({"var_names": "mu", "transform": lambda x: x + 1}, 1),
         ({"var_names": "mu", "rope": (-1, 1)}, 1),
@@ -493,14 +502,16 @@
     assert ax.shape == (side, side)
 
 
 @pytest.mark.parametrize("kind", ["kde", "cumulative", "scatter"])
 @pytest.mark.parametrize("alpha", [None, 0.2, 1])
 @pytest.mark.parametrize("animated", [False, True])
 def test_plot_ppc(models, kind, alpha, animated):
+    if animation and not animation.writers.is_available("ffmpeg"):
+        pytest.skip("matplotlib animations within ArviZ require ffmpeg")
     animation_kwargs = {"blit": False}
     axes = plot_ppc(
         models.model_1,
         kind=kind,
         alpha=alpha,
         animated=animated,
         animation_kwargs=animation_kwargs,
@@ -512,14 +523,16 @@
     assert axes
 
 
 @pytest.mark.parametrize("kind", ["kde", "cumulative", "scatter"])
 @pytest.mark.parametrize("jitter", [None, 0, 0.1, 1, 3])
 @pytest.mark.parametrize("animated", [False, True])
 def test_plot_ppc_multichain(kind, jitter, animated):
+    if animation and not animation.writers.is_available("ffmpeg"):
+        pytest.skip("matplotlib animations within ArviZ require ffmpeg")
     data = from_dict(
         posterior_predictive={
             "x": np.random.randn(4, 100, 30),
             "y_hat": np.random.randn(4, 100, 3, 10),
         },
         observed_data={"x": np.random.randn(30), "y": np.random.randn(3, 10)},
     )
@@ -539,27 +552,33 @@
     else:
         assert np.all(axes)
 
 
 @pytest.mark.parametrize("kind", ["kde", "cumulative", "scatter"])
 @pytest.mark.parametrize("animated", [False, True])
 def test_plot_ppc_discrete(kind, animated):
+    if animation and not animation.writers.is_available("ffmpeg"):
+        pytest.skip("matplotlib animations within ArviZ require ffmpeg")
     data = from_dict(
         observed_data={"obs": np.random.randint(1, 100, 15)},
         posterior_predictive={"obs": np.random.randint(1, 300, (1, 20, 15))},
     )
 
     animation_kwargs = {"blit": False}
     axes = plot_ppc(data, kind=kind, animated=animated, animation_kwargs=animation_kwargs)
     if animated:
         assert np.all(axes[0])
         assert np.all(axes[1])
     assert axes
 
 
+@pytest.mark.skipif(
+    not animation.writers.is_available("ffmpeg"),
+    reason="matplotlib animations within ArviZ require ffmpeg",
+)
 @pytest.mark.parametrize("kind", ["kde", "cumulative", "scatter"])
 def test_plot_ppc_save_animation(models, kind):
     animation_kwargs = {"blit": False}
     axes, anim = plot_ppc(
         models.model_1,
         kind=kind,
         animated=True,
@@ -573,14 +592,18 @@
     os.makedirs(animations_folder, exist_ok=True)
     path = os.path.join(animations_folder, "ppc_{}_animation.mp4".format(kind))
     anim.save(path)
     assert os.path.exists(path)
     assert os.path.getsize(path)
 
 
+@pytest.mark.skipif(
+    not animation.writers.is_available("ffmpeg"),
+    reason="matplotlib animations within ArviZ require ffmpeg",
+)
 @pytest.mark.parametrize("kind", ["kde", "cumulative", "scatter"])
 def test_plot_ppc_discrete_save_animation(kind):
     data = from_dict(
         observed_data={"obs": np.random.randint(1, 100, 15)},
         posterior_predictive={"obs": np.random.randint(1, 300, (1, 20, 15))},
     )
     animation_kwargs = {"blit": False}
@@ -598,14 +621,18 @@
     os.makedirs(animations_folder, exist_ok=True)
     path = os.path.join(animations_folder, "ppc_discrete_{}_animation.mp4".format(kind))
     anim.save(path)
     assert os.path.exists(path)
     assert os.path.getsize(path)
 
 
+@pytest.mark.skipif(
+    not animation.writers.is_available("ffmpeg"),
+    reason="matplotlib animations within ArviZ require ffmpeg",
+)
 @pytest.mark.parametrize("system", ["Windows", "Darwin"])
 def test_non_linux_blit(models, monkeypatch, system, caplog):
     import platform
 
     def mock_system():
         return system
 
@@ -653,14 +680,18 @@
 def test_plot_ppc_ax(models, kind, fig_ax):
     """Test ax argument of plot_ppc."""
     _, ax = fig_ax
     axes = plot_ppc(models.model_1, kind=kind, ax=ax)
     assert axes[0] is ax
 
 
+@pytest.mark.skipif(
+    not animation.writers.is_available("ffmpeg"),
+    reason="matplotlib animations within ArviZ require ffmpeg",
+)
 def test_plot_ppc_bad_ax(models, fig_ax):
     _, ax = fig_ax
     _, ax2 = plt.subplots(1, 2)
     with pytest.raises(ValueError, match="same figure"):
         plot_ppc(
             models.model_1, ax=[ax, *ax2], flatten=[], coords={"obs_dim": [1, 2, 3]}, animated=True
         )
@@ -819,22 +850,51 @@
     assert "['loo', 'waic']" in str(err.value)
 
 
 @pytest.mark.parametrize(
     "kwargs",
     [
         {"color": "0.5", "circular": True},
-        {"fill_kwargs": {"alpha": 0}},
+        {"hdi_data": True, "fill_kwargs": {"alpha": 0}},
         {"plot_kwargs": {"alpha": 0}},
         {"smooth_kwargs": {"window_length": 33, "polyorder": 5, "mode": "mirror"}},
-        {"smooth": False},
+        {"hdi_data": True, "smooth": False},
     ],
 )
 def test_plot_hdi(models, data, kwargs):
-    plot_hdi(data["y"], models.model_1.posterior["theta"], **kwargs)
+    hdi_data = kwargs.pop("hdi_data", None)
+    if hdi_data:
+        hdi_data = hdi(models.model_1.posterior["theta"])
+        ax = plot_hdi(data["y"], hdi_data=hdi_data, **kwargs)
+    else:
+        ax = plot_hdi(data["y"], models.model_1.posterior["theta"], **kwargs)
+    assert ax
+
+
+def test_plot_hdi_warning():
+    """Check using both y and hdi_data sends a warning."""
+    x_data = np.random.normal(0, 1, 100)
+    y_data = np.random.normal(2 + x_data * 0.5, 0.5, (1, 200, 100))
+    hdi_data = hdi(y_data)
+    with pytest.warns(UserWarning, match="Both y and hdi_data"):
+        ax = plot_hdi(x_data, y=y_data, hdi_data=hdi_data)
+    assert ax
+
+
+def test_plot_hdi_missing_arg_error():
+    """Check that both y and hdi_data missing raises an error."""
+    with pytest.raises(ValueError, match="One of {y, hdi_data"):
+        plot_hdi(np.arange(20))
+
+
+def test_plot_hdi_dataset_error(models):
+    """Check hdi_data as multiple variable Dataset raises an error."""
+    hdi_data = hdi(models.model_1)
+    with pytest.raises(ValueError, match="Only single variable Dataset"):
+        plot_hdi(np.arange(8), hdi_data=hdi_data)
 
 
 @pytest.mark.parametrize("limits", [(-10.0, 10.0), (-5, 5), (None, None)])
 def test_fast_kde_scipy(limits):
     data = np.random.normal(0, 1, 10000)
     if limits[0] is None:
         x = np.linspace(data.min(), data.max(), 200)  # pylint: disable=no-member
@@ -1097,16 +1157,16 @@
 
 @pytest.mark.parametrize(
     "kwargs",
     [
         {},
         {"n_unif": 50, "legend": False},
         {"use_hdi": True, "color": "gray"},
-        {"use_hdi": True, "credible_interval": 0.68, "plot_kwargs": {"ls": "--"}},
-        {"use_hdi": True, "hdi_kwargs": {"smooth": False}},
+        {"use_hdi": True, "credible_interval": 0.68},
+        {"use_hdi": True, "hdi_kwargs": {"fill": 0.1}},
         {"ecdf": True},
         {"ecdf": True, "ecdf_fill": False, "plot_unif_kwargs": {"ls": "--"}},
         {"ecdf": True, "credible_interval": 0.97, "fill_kwargs": {"hatch": "/"}},
     ],
 )
 def test_plot_loo_pit(models, kwargs):
     axes = plot_loo_pit(idata=models.model_1, y="y", **kwargs)
@@ -1190,7 +1250,39 @@
 
 def test_plot_mcse_no_divergences(models):
     """Test error when rug=True, but the variable defined by rug_kind is missing."""
     idata = deepcopy(models.model_1)
     idata.sample_stats = idata.sample_stats.rename({"diverging": "diverging_missing"})
     with pytest.raises(ValueError, match="not contain diverging"):
         plot_mcse(idata, rug=True)
+
+
+@pytest.mark.parametrize(
+    "kwargs",
+    [
+        {},
+        {"var_names": ["theta"]},
+        {"var_names": ["theta"], "coords": {"theta_dim_0": [0, 1]}},
+        {"var_names": ["eta"], "posterior_kwargs": {"rug": True, "rug_kwargs": {"color": "r"}}},
+        {"var_names": ["mu"], "prior_kwargs": {"fill_kwargs": {"alpha": 0.5}}},
+        {
+            "var_names": ["tau"],
+            "prior_kwargs": {"plot_kwargs": {"color": "r"}},
+            "posterior_kwargs": {"plot_kwargs": {"color": "b"}},
+        },
+        {"var_names": ["y"], "kind": "observed"},
+    ],
+)
+def test_plot_dist_comparison(models, kwargs):
+    idata = models.model_1
+    ax = plot_dist_comparison(idata, **kwargs)
+    assert np.all(ax)
+
+
+def test_plot_dist_comparison_different_vars():
+    data = from_dict(
+        posterior={"x": np.random.randn(4, 100, 30),}, prior={"x_hat": np.random.randn(4, 100, 30)},
+    )
+    with pytest.raises(KeyError):
+        plot_dist_comparison(data, var_names="x")
+    ax = plot_dist_comparison(data, var_names=[["x_hat"], ["x"]])
+    assert np.all(ax)
```

### Comparing `arviz-0.8.3/arviz/tests/base_tests/test_stats_utils.py` & `arviz-0.9.0/arviz/tests/base_tests/test_stats_utils.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/base_tests/test_rcparams.py` & `arviz-0.9.0/arviz/tests/base_tests/test_rcparams.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/base_tests/test_utils.py` & `arviz-0.9.0/arviz/tests/base_tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/base_tests/test_diagnostics.py` & `arviz-0.9.0/arviz/tests/base_tests/test_diagnostics.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/base_tests/test_utils_numba.py` & `arviz-0.9.0/arviz/tests/base_tests/test_utils_numba.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/base_tests/test_plot_utils.py` & `arviz-0.9.0/arviz/tests/base_tests/test_plot_utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,14 +12,15 @@
     format_sig_figs,
     get_plotting_function,
     make_2d,
     matplotlib_kwarg_dealiaser,
     xarray_to_ndarray,
     xarray_var_iter,
     vectorized_to_hex,
+    _dealiase_sel_kwargs,
 )
 from ...rcparams import rc_context
 from ...numeric_utils import get_bins
 from ...utils import get_coords
 
 
 @pytest.mark.parametrize(
@@ -240,7 +241,26 @@
 
 @pytest.mark.parametrize(
     "c_values", [["blue", "blue"], ["blue", "#0000ff"], np.array([[0, 0, 1], [0, 0, 1]])]
 )
 def test_vectorized_to_hex_array(c_values):
     output = vectorized_to_hex(c_values)
     assert np.all([item == "#0000ff" for item in output])
+
+
+def test_dealiase_sel_kwargs():
+    """Check _dealiase_sel_kwargs behaviour.
+
+    Makes sure kwargs are overwritten when necessary even with alias involved and that
+    they are not modified when not included in props.
+    """
+    kwargs = {"linewidth": 3, "alpha": 0.4, "line_color": "red"}
+    props = {"lw": [1, 2, 4, 5], "linestyle": ["-", "--", ":"]}
+    res = _dealiase_sel_kwargs(kwargs, props, 2)
+    assert "linewidth" in res
+    assert res["linewidth"] == 4
+    assert "linestyle" in res
+    assert res["linestyle"] == ":"
+    assert "alpha" in res
+    assert res["alpha"] == 0.4
+    assert "line_color" in res
+    assert res["line_color"] == "red"
```

### Comparing `arviz-0.8.3/arviz/tests/base_tests/test_data.py` & `arviz-0.9.0/arviz/tests/base_tests/test_data.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # pylint: disable=no-member, invalid-name, redefined-outer-name
 # pylint: disable=too-many-lines
 from collections import namedtuple
 import os
 from typing import Dict
 from urllib.parse import urlunsplit
+from html import escape
 import numpy as np
 import pytest
 
 import xarray as xr
+from xarray.core.options import OPTIONS
 
 from arviz import (
     concat,
     convert_to_inference_data,
     convert_to_dataset,
     from_dict,
     from_netcdf,
@@ -452,14 +454,36 @@
             idata_map.observed_data.obs, fun(idata.observed_data.obs, *args, **kwargs)
         )
         assert np.allclose(
             idata_map.posterior_predictive.obs, fun(idata.posterior_predictive.obs, *args, **kwargs)
         )
         assert np.allclose(idata_map.posterior.mu, idata.posterior.mu)
 
+    def test_repr_html(self):
+        """Test if the function _repr_html is generating html."""
+        idata = load_arviz_data("centered_eight")
+        display_style = OPTIONS["display_style"]
+        xr.set_options(display_style="html")
+        html = idata._repr_html_()  # pylint: disable=protected-access
+
+        assert html is not None
+        assert "<div" in html
+        for group in idata._groups:  # pylint: disable=protected-access
+            assert group in html
+            xr_data = getattr(idata, group)
+            for item, _ in xr_data.items():
+                assert item in html
+        specific_style = ".xr-wrap{width:700px!important;}"
+        assert specific_style in html
+
+        xr.set_options(display_style="text")
+        html = idata._repr_html_()  # pylint: disable=protected-access
+        assert escape(idata.__repr__()) in html
+        xr.set_options(display_style=display_style)
+
 
 class TestNumpyToDataArray:
     def test_1d_dataset(self):
         size = 100
         dataset = convert_to_dataset(np.random.randn(size))
         assert len(dataset.data_vars) == 1
```

### Comparing `arviz-0.8.3/arviz/tests/external_tests/test_data_numpyro.py` & `arviz-0.9.0/arviz/tests/external_tests/test_data_numpyro.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/external_tests/test_data_pymc.py` & `arviz-0.9.0/arviz/tests/external_tests/test_data_pymc.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,14 @@
-# pylint: disable=no-member, invalid-name, redefined-outer-name, protected-access
+# pylint: disable=no-member, invalid-name, redefined-outer-name, protected-access, too-many-public-methods
 from sys import version_info
 from typing import Dict, Tuple
+import packaging
 
 import numpy as np
+import pandas as pd
 import pytest
 from numpy import ma
 
 from arviz import (
     from_pymc3,
     from_pymc3_predictions,
     InferenceData,
@@ -192,14 +194,87 @@
 
         records = caplog.records
         shape = inference_data.posterior_predictive.obs.shape
         assert np.all([obs_s == s for obs_s, s in zip(shape, (1, 370, eight_schools_params["J"]))])
         assert len(records) == 1
         assert records[0].levelname == "WARNING"
 
+    @pytest.mark.skipif(
+        packaging.version.Version(pm.__version__) < packaging.version.Version("3.9.0"),
+        reason="Requires PyMC3 >= 3.9.0",
+    )
+    @pytest.mark.parametrize("use_context", [True, False])
+    def test_autodetect_coords_from_model(self, use_context):
+        df_data = pd.DataFrame(columns=["date"]).set_index("date")
+        dates = pd.date_range(start="2020-05-01", end="2020-05-20")
+        for city, mu in {"Berlin": 15, "San Marino": 18, "Paris": 16}.items():
+            df_data[city] = np.random.normal(loc=mu, size=len(dates))
+        df_data.index = dates
+        df_data.index.name = "date"
+
+        coords = {"date": df_data.index, "city": df_data.columns}
+        with pm.Model(coords=coords) as model:
+            europe_mean = pm.Normal("europe_mean_temp", mu=15.0, sd=3.0)
+            city_offset = pm.Normal("city_offset", mu=0.0, sd=3.0, dims="city")
+            city_temperature = pm.Deterministic(
+                "city_temperature", europe_mean + city_offset, dims="city"
+            )
+
+            data_dims = ("date", "city")
+            data = pm.Data("data", df_data, dims=data_dims)
+            _ = pm.Normal("likelihood", mu=city_temperature, sd=0.5, observed=data, dims=data_dims)
+
+            trace = pm.sample(
+                return_inferencedata=False,
+                compute_convergence_checks=False,
+                cores=1,
+                chains=1,
+                tune=20,
+                draws=30,
+                step=pm.Metropolis(),
+            )
+            if use_context:
+                idata = from_pymc3(trace=trace)
+        if not use_context:
+            idata = from_pymc3(trace=trace, model=model)
+
+        assert "city" in list(idata.posterior.dims)
+        assert "city" in list(idata.observed_data.dims)
+        assert "date" in list(idata.observed_data.dims)
+        np.testing.assert_array_equal(idata.posterior.coords["city"], coords["city"])
+        np.testing.assert_array_equal(idata.observed_data.coords["date"], coords["date"])
+        np.testing.assert_array_equal(idata.observed_data.coords["city"], coords["city"])
+
+    def test_ovewrite_model_coords_dims(self):
+        """Check coords and dims from model object can be partially overwrited."""
+        dim1 = ["a", "b"]
+        new_dim1 = ["c", "d"]
+        coords = {"dim1": dim1, "dim2": ["c1", "c2"]}
+        x_data = np.arange(4).reshape((2, 2))
+        y = x_data + np.random.normal(size=(2, 2))
+        with pm.Model(coords=coords):
+            x = pm.Data("x", x_data, dims=("dim1", "dim2"))
+            beta = pm.Normal("beta", 0, 1, dims="dim1")
+            _ = pm.Normal("obs", x * beta, 1, observed=y, dims=("dim1", "dim2"))
+            trace = pm.sample(100, tune=100)
+            idata1 = from_pymc3(trace)
+            idata2 = from_pymc3(trace, coords={"dim1": new_dim1}, dims={"beta": ["dim2"]})
+
+        test_dict = {"posterior": ["beta"], "observed_data": ["obs"], "constant_data": ["x"]}
+        fails1 = check_multiple_attrs(test_dict, idata1)
+        assert not fails1
+        fails2 = check_multiple_attrs(test_dict, idata2)
+        assert not fails2
+        assert "dim1" in list(idata1.posterior.beta.dims)
+        assert "dim2" in list(idata2.posterior.beta.dims)
+        assert np.all(idata1.constant_data.x.dim1.values == np.array(dim1))
+        assert np.all(idata1.constant_data.x.dim2.values == np.array(["c1", "c2"]))
+        assert np.all(idata2.constant_data.x.dim1.values == np.array(new_dim1))
+        assert np.all(idata2.constant_data.x.dim2.values == np.array(["c1", "c2"]))
+
     def test_missing_data_model(self):
         # source pymc3/pymc3/tests/test_missing.py
         data = ma.masked_values([1, 2, -1, 4, -1], value=-1)
         model = pm.Model()
         with model:
             x = pm.Normal("x", 1, 1)
             pm.Normal("y", x, 1, observed=data)
@@ -223,42 +298,78 @@
             pm.Normal("y2", x, 1, observed=y2_data)
             trace = pm.sample(100, chains=2)
             inference_data = from_pymc3(trace=trace, log_likelihood=log_likelihood)
         test_dict = {
             "posterior": ["x"],
             "observed_data": ["y1", "y2"],
             "log_likelihood": ["y1", "y2"],
-            "sample_stats": ["diverging", "lp"],
+            "sample_stats": ["diverging", "lp", "~log_likelihood"],
         }
         if not log_likelihood:
             test_dict.pop("log_likelihood")
             test_dict["~log_likelihood"] = []
         if isinstance(log_likelihood, list):
             test_dict["log_likelihood"] = ["y1", "~y2"]
 
         fails = check_multiple_attrs(test_dict, inference_data)
         assert not fails
-        assert not hasattr(inference_data.sample_stats, "log_likelihood")
 
     @pytest.mark.skipif(
         version_info < (3, 6), reason="Requires updated PyMC3, which needs Python 3.6"
     )
     def test_multiple_observed_rv_without_observations(self):
         with pm.Model():
             mu = pm.Normal("mu")
             x = pm.DensityDist(  # pylint: disable=unused-variable
                 "x", pm.Normal.dist(mu, 1.0).logp, observed={"value": 0.1}
             )
             trace = pm.sample(100, chains=2)
             inference_data = from_pymc3(trace=trace)
-        assert inference_data
-        assert not hasattr(inference_data, "observed_data")
-        assert hasattr(inference_data, "posterior")
-        assert hasattr(inference_data, "sample_stats")
-        assert hasattr(inference_data, "log_likelihood")
+        test_dict = {
+            "posterior": ["mu"],
+            "sample_stats": ["lp"],
+            "log_likelihood": ["x"],
+            "observed_data": ["value", "~x"],
+        }
+        fails = check_multiple_attrs(test_dict, inference_data)
+        assert not fails
+        assert inference_data.observed_data.value.dtype.kind == "f"
+
+    def test_multiobservedrv_to_observed_data(self):
+        # fake regression data, with weights (W)
+        np.random.seed(2019)
+        N = 100
+        X = np.random.uniform(size=N)
+        W = 1 + np.random.poisson(size=N)
+        a, b = 5, 17
+        Y = a + np.random.normal(b * X)
+
+        with pm.Model():
+            a = pm.Normal("a", 0, 10)
+            b = pm.Normal("b", 0, 10)
+            mu = a + b * X
+            sigma = pm.HalfNormal("sigma", 1)
+
+            def weighted_normal(y, w):
+                return w * pm.Normal.dist(mu=mu, sd=sigma).logp(y)
+
+            y_logp = pm.DensityDist(  # pylint: disable=unused-variable
+                "y_logp", weighted_normal, observed={"y": Y, "w": W}
+            )
+            trace = pm.sample(20, tune=20)
+            idata = from_pymc3(trace)
+        test_dict = {
+            "posterior": ["a", "b", "sigma"],
+            "sample_stats": ["lp"],
+            "log_likelihood": ["y_logp"],
+            "observed_data": ["y", "w"],
+        }
+        fails = check_multiple_attrs(test_dict, idata)
+        assert not fails
+        assert idata.observed_data.y.dtype.kind == "f"
 
     def test_single_observation(self):
         with pm.Model():
             p = pm.Uniform("p", 0, 1)
             pm.Binomial("w", p=p, n=2, observed=1)
             trace = pm.sample(500, chains=2)
             inference_data = from_pymc3(trace=trace)
@@ -385,15 +496,15 @@
         with pm.Model():
             x = pm.Data("x", [1.0, 2.0, 3.0])
             y = pm.Data("y", [1.0, 2.0, 3.0])
             beta = pm.Normal("beta", 0, 1)
             obs = pm.Normal("obs", x * beta, 1, observed=y)  # pylint: disable=unused-variable
             prior = pm.sample_prior_predictive()
 
-        with pytest.warns(PendingDeprecationWarning, match="without the model"):
+        with pytest.warns(FutureWarning, match="without the model"):
             inference_data = from_pymc3(prior=prior)
         test_dict = {
             "prior": ["beta", "obs"],
             "~prior_predictive": [],
         }
         fails = check_multiple_attrs(test_dict, inference_data)
         assert not fails
```

### Comparing `arviz-0.8.3/arviz/tests/external_tests/test_data_tfp.py` & `arviz-0.9.0/arviz/tests/external_tests/test_data_tfp.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/external_tests/test_data_emcee.py` & `arviz-0.9.0/arviz/tests/external_tests/test_data_emcee.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/external_tests/test_data_pystan.py` & `arviz-0.9.0/arviz/tests/external_tests/test_data_pystan.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/external_tests/test_data_pyro.py` & `arviz-0.9.0/arviz/tests/external_tests/test_data_pyro.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     load_cached_models,
 )
 
 # Skip all tests if pyro or pytorch not installed
 torch = importorskip("torch")
 pyro = importorskip("pyro")
 Predictive = pyro.infer.Predictive
+dist = pyro.distributions
 
 
 class TestDataPyro:
     @pytest.fixture(scope="class")
     def data(self, eight_schools_params, draws, chains):
         class Data:
             obj = load_cached_models(eight_schools_params, draws, chains, "pyro")["pyro"]
@@ -160,53 +161,47 @@
     def test_inference_data_only_posterior_has_log_likelihood(self, data):
         idata = from_pyro(data.obj)
         test_dict = {"log_likelihood": ["obs"]}
         fails = check_multiple_attrs(test_dict, idata)
         assert not fails
 
     def test_multiple_observed_rv(self):
-        import pyro.distributions as dist
-        from pyro.infer import MCMC, NUTS
-
         y1 = torch.randn(10)
         y2 = torch.randn(10)
 
         def model_example_multiple_obs(y1=None, y2=None):
             x = pyro.sample("x", dist.Normal(1, 3))
             pyro.sample("y1", dist.Normal(x, 1), obs=y1)
             pyro.sample("y2", dist.Normal(x, 1), obs=y2)
 
-        nuts_kernel = NUTS(model_example_multiple_obs)
-        mcmc = MCMC(nuts_kernel, num_samples=10)
+        nuts_kernel = pyro.infer.NUTS(model_example_multiple_obs)
+        mcmc = pyro.infer.MCMC(nuts_kernel, num_samples=10)
         mcmc.run(y1=y1, y2=y2)
         inference_data = from_pyro(mcmc)
         test_dict = {
             "posterior": ["x"],
             "sample_stats": ["diverging"],
             "log_likelihood": ["y1", "y2"],
             "observed_data": ["y1", "y2"],
         }
         fails = check_multiple_attrs(test_dict, inference_data)
         assert not fails
         assert not hasattr(inference_data.sample_stats, "log_likelihood")
 
     def test_inference_data_constant_data(self):
-        import pyro.distributions as dist
-        from pyro.infer import MCMC, NUTS
-
         x1 = 10
         x2 = 12
         y1 = torch.randn(10)
 
         def model_constant_data(x, y1=None):
             _x = pyro.sample("x", dist.Normal(1, 3))
             pyro.sample("y1", dist.Normal(x * _x, 1), obs=y1)
 
-        nuts_kernel = NUTS(model_constant_data)
-        mcmc = MCMC(nuts_kernel, num_samples=10)
+        nuts_kernel = pyro.infer.NUTS(model_constant_data)
+        mcmc = pyro.infer.MCMC(nuts_kernel, num_samples=10)
         mcmc.run(x=x1, y1=y1)
         posterior = mcmc.get_samples()
         posterior_predictive = Predictive(model_constant_data, posterior)(x1)
         predictions = Predictive(model_constant_data, posterior)(x2)
         inference_data = from_pyro(
             mcmc,
             posterior_predictive=posterior_predictive,
@@ -228,7 +223,38 @@
         assert not fails
 
     def test_inference_data_num_chains(self, predictions_data, chains):
         predictions = predictions_data
         inference_data = from_pyro(predictions=predictions, num_chains=chains)
         nchains = inference_data.predictions.dims["chain"]
         assert nchains == chains
+
+    @pytest.mark.parametrize("log_likelihood", [True, False])
+    def test_log_likelihood(self, log_likelihood):
+        """Test behaviour when log likelihood cannot be retrieved.
+
+        If log_likelihood=True there is a warning to say log_likelihood group is skipped,
+        if log_likelihood=False there is no warning and log_likelihood is skipped.
+        """
+        x = torch.randn((10, 2))
+        y = torch.randn(10)
+
+        def model_constant_data(x, y=None):
+            beta = pyro.sample("beta", dist.Normal(torch.ones(2), 3))
+            pyro.sample("y", dist.Normal(x.matmul(beta), 1), obs=y)
+
+        nuts_kernel = pyro.infer.NUTS(model_constant_data)
+        mcmc = pyro.infer.MCMC(nuts_kernel, num_samples=10)
+        mcmc.run(x=x, y=y)
+        if log_likelihood:
+            with pytest.warns(UserWarning, match="Could not get vectorized trace"):
+                inference_data = from_pyro(mcmc, log_likelihood=log_likelihood)
+        else:
+            inference_data = from_pyro(mcmc, log_likelihood=log_likelihood)
+        test_dict = {
+            "posterior": ["beta"],
+            "sample_stats": ["diverging"],
+            "~log_likelihood": [],
+            "observed_data": ["y"],
+        }
+        fails = check_multiple_attrs(test_dict, inference_data)
+        assert not fails
```

### Comparing `arviz-0.8.3/arviz/tests/external_tests/test_data_cmdstan.py` & `arviz-0.9.0/arviz/tests/external_tests/test_data_cmdstan.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/external_tests/test_data_cmdstanpy.py` & `arviz-0.9.0/arviz/tests/external_tests/test_data_cmdstanpy.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/helpers.py` & `arviz-0.9.0/arviz/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/tests/conftest.py` & `arviz-0.9.0/arviz/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/wrappers/base.py` & `arviz-0.9.0/arviz/wrappers/base.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/wrappers/wrap_pystan.py` & `arviz-0.9.0/arviz/wrappers/wrap_pystan.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/stats/diagnostics.py` & `arviz-0.9.0/arviz/stats/diagnostics.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/stats/__init__.py` & `arviz-0.9.0/arviz/stats/__init__.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/stats/stats.py` & `arviz-0.9.0/arviz/stats/stats.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,23 +334,23 @@
     **kwargs,
 ):
     """Pending deprecation. Please refer to :func:`~arviz.hdi`."""
     # pylint: enable=unused-argument
     warnings.warn(("hpd will be deprecated " "Please replace hdi"),)
     return hdi(
         ary,
-        hdi_prob=None,
-        circular=False,
-        multimodal=False,
-        skipna=False,
-        group="posterior",
-        var_names=None,
-        filter_vars=None,
-        coords=None,
-        max_modes=10,
+        hdi_prob,
+        circular,
+        multimodal,
+        skipna,
+        group,
+        var_names,
+        filter_vars,
+        coords,
+        max_modes,
         **kwargs,
     )
 
 
 def hdi(
     ary,
     hdi_prob=None,
@@ -361,34 +361,34 @@
     var_names=None,
     filter_vars=None,
     coords=None,
     max_modes=10,
     **kwargs,
 ):
     """
-    Calculate highest density interval (HDI) of array for given percentage.
+    Calculate highest density interval (HDI) of array for given probability.
 
     The HDI is the minimum width Bayesian credible interval (BCI).
 
     Parameters
     ----------
     ary: obj
         object containing posterior samples.
         Any object that can be converted to an az.InferenceData object.
         Refer to documentation of az.convert_to_dataset for details.
     hdi_prob: float, optional
-        HDI prob for which interval will be computed. Defaults to 0.94.
+        HDI prob for which interval will be computed. Defaults to ``stats.hdi_prob`` rcParam.
     circular: bool, optional
         Whether to compute the hdi taking into account `x` is a circular variable
         (in the range [-np.pi, np.pi]) or not. Defaults to False (i.e non-circular variables).
         Only works if multimodal is False.
-    multimodal: bool
+    multimodal: bool, optional
         If true it may compute more than one hdi interval if the distribution is multimodal and the
         modes are well separated.
-    skipna: bool
+    skipna: bool, optional
         If true ignores nan values when computing the hdi interval. Defaults to false.
     group: str, optional
         Specifies which InferenceData group should be used to calculate hdi.
         Defaults to 'posterior'
     var_names: list, optional
         Names of variables to include in the hdi report. Prefix the variables by `~`
         when you want to exclude them from the report: `["~beta"]` instead of `["beta"]`
@@ -399,48 +399,52 @@
         interpret var_names as regular expressions on the real variables names. A la
         `pandas.filter`.
     coords: mapping, optional
         Specifies the subset over to calculate hdi.
     max_modes: int, optional
         Specifies the maximum number of modes for multimodal case.
     kwargs: dict, optional
-        Additional keywords passed to `wrap_xarray_ufunc`.
-        See the docstring of :obj:`wrap_xarray_ufunc method </.stats_utils.wrap_xarray_ufunc>`.
+        Additional keywords passed to :func:`~arviz.wrap_xarray_ufunc`.
 
     Returns
     -------
     np.ndarray or xarray.Dataset, depending upon input
         lower(s) and upper(s) values of the interval(s).
 
+    See Also
+    --------
+    plot_hdi : Plot HDI intervals for regression data.
+    xarray.Dataset.quantile : Calculate quantiles of array for given probabilities.
+
     Examples
     --------
-    Calculate the hdi of a Normal random variable:
+    Calculate the HDI of a Normal random variable:
 
     .. ipython::
 
         In [1]: import arviz as az
            ...: import numpy as np
            ...: data = np.random.normal(size=2000)
            ...: az.hdi(data, hdi_prob=.68)
 
-    Calculate the hdi of a dataset:
+    Calculate the HDI of a dataset:
 
     .. ipython::
 
         In [1]: import arviz as az
            ...: data = az.load_arviz_data('centered_eight')
            ...: az.hdi(data)
 
-    We can also calculate the hdi of some of the variables of dataset:
+    We can also calculate the HDI of some of the variables of dataset:
 
     .. ipython::
 
         In [1]: az.hdi(data, var_names=["mu", "theta"])
 
-    If we want to calculate the hdi over specified dimension of dataset,
+    If we want to calculate the HDI over specified dimension of dataset,
     we can pass `input_core_dims` by kwargs:
 
     .. ipython::
 
         In [1]: az.hdi(data, input_core_dims = [["chain"]])
 
     We can also calculate the hdi over a particular selection over all groups:
@@ -472,23 +476,31 @@
     isarray = isinstance(ary, np.ndarray)
     if isarray and ary.ndim <= 1:
         func_kwargs.pop("out_shape")
         hdi_data = func(ary, **func_kwargs)  # pylint: disable=unexpected-keyword-arg
         return hdi_data[~np.isnan(hdi_data).all(axis=1), :] if multimodal else hdi_data
 
     if isarray and ary.ndim == 2:
-        kwargs.setdefault("input_core_dims", [["chain"]])
+        warnings.warn(
+            "hdi currently interprets 2d data as (draw, shape) but this will change in "
+            "a future release to (chain, draw) for coherence with other functions",
+            FutureWarning,
+        )
+        ary = np.expand_dims(ary, 0)
 
     ary = convert_to_dataset(ary, group=group)
     if coords is not None:
         ary = get_coords(ary, coords)
     var_names = _var_names(var_names, ary, filter_vars)
     ary = ary[var_names] if var_names else ary
 
-    hdi_data = _wrap_xarray_ufunc(func, ary, func_kwargs=func_kwargs, **kwargs)
+    hdi_coord = xr.DataArray(["lower", "higher"], dims=["hdi"], attrs=dict(hdi_prob=hdi_prob))
+    hdi_data = _wrap_xarray_ufunc(func, ary, func_kwargs=func_kwargs, **kwargs).assign_coords(
+        {"hdi": hdi_coord}
+    )
     hdi_data = hdi_data.dropna("mode", how="all") if multimodal else hdi_data
     return hdi_data.x.values if isarray else hdi_data
 
 
 def _hdi(ary, hdi_prob, circular, skipna):
     """Compute hpi over the flattened array."""
     ary = ary.flatten()
@@ -523,15 +535,15 @@
 
     hdi_interval = np.array([hdi_min, hdi_max])
 
     return hdi_interval
 
 
 def _hdi_multimodal(ary, hdi_prob, skipna, max_modes):
-    """Compute hdi if the distribution is multimodal."""
+    """Compute HDI if the distribution is multimodal."""
     ary = ary.flatten()
     if skipna:
         ary = ary[~np.isnan(ary)]
 
     if ary.dtype.kind == "f":
         density, lower, upper = _fast_kde(ary)
         range_x = upper - lower
@@ -1025,15 +1037,15 @@
         The functions will be given one argument, the samples for a variable as an nD array,
         The functions should be in the style of a ufunc and return a single number. For example,
         `np.mean`, or `scipy.stats.var` would both work.
     extend: boolean
         If True, use the statistics returned by ``stat_funcs`` in addition to, rather than in place
         of, the default statistics. This is only meaningful when ``stat_funcs`` is not None.
     hdi_prob: float, optional
-        hdi interval to compute. Defaults to 0.94. This is only meaningful when ``stat_funcs`` is
+        HDI interval to compute. Defaults to 0.94. This is only meaningful when ``stat_funcs`` is
         None.
     order: {"C", "F"}
         If fmt is "wide", use either C or F unpacking order. Defaults to C.
     index_origin: int
         If fmt is "wide, select n-based indexing for multivariate parameters.
         Defaults to rcParam data.index.origin, which is 0.
     skipna: bool
@@ -1157,21 +1169,17 @@
                 extra_metric_names.append(stat_func.__name__)
 
     if extend and kind in ["all", "stats"]:
         mean = posterior.mean(dim=("chain", "draw"), skipna=skipna)
 
         sd = posterior.std(dim=("chain", "draw"), ddof=1, skipna=skipna)
 
-        hdi_lower, hdi_higher = xr.apply_ufunc(
-            _make_ufunc(hdi, n_output=2),
-            posterior,
-            kwargs=dict(hdi_prob=hdi_prob, multimodal=False, skipna=skipna),
-            input_core_dims=(("chain", "draw"),),
-            output_core_dims=tuple([] for _ in range(2)),
-        )
+        hdi_post = hdi(posterior, hdi_prob=hdi_prob, multimodal=False, skipna=skipna)
+        hdi_lower = hdi_post.sel(hdi="lower", drop=True)
+        hdi_higher = hdi_post.sel(hdi="higher", drop=True)
 
     if include_circ:
         nan_policy = "omit" if skipna else "propagate"
         circ_mean = xr.apply_ufunc(
             _make_ufunc(st.circmean),
             posterior,
             kwargs=dict(high=np.pi, low=-np.pi, nan_policy=nan_policy),
@@ -1195,21 +1203,17 @@
         circ_mcse = xr.apply_ufunc(
             _make_ufunc(_mc_error),
             posterior,
             kwargs=dict(circular=True),
             input_core_dims=(("chain", "draw"),),
         )
 
-        circ_hdi_lower, circ_hdi_higher = xr.apply_ufunc(
-            _make_ufunc(hdi, n_output=2),
-            posterior,
-            kwargs=dict(hdi_prob=hdi_prob, circular=True, skipna=skipna),
-            input_core_dims=(("chain", "draw"),),
-            output_core_dims=tuple([] for _ in range(2)),
-        )
+        circ_hdi = hdi(posterior, hdi_prob=hdi_prob, circular=True, skipna=skipna)
+        circ_hdi_lower = circ_hdi.sel(hdi="lower", drop=True)
+        circ_hdi_higher = circ_hdi.sel(hdi="higher", drop=True)
 
     if kind in ["all", "diagnostics"]:
         mcse_mean, mcse_sd, ess_mean, ess_sd, ess_bulk, ess_tail, r_hat = xr.apply_ufunc(
             _make_ufunc(_multichain_statistics, n_output=7, ravel=False),
             posterior,
             input_core_dims=(("chain", "draw"),),
             output_core_dims=tuple([] for _ in range(7)),
```

### Comparing `arviz-0.8.3/arviz/stats/stats_utils.py` & `arviz-0.9.0/arviz/stats/stats_utils.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/stats/stats_refitting.py` & `arviz-0.9.0/arviz/stats/stats_refitting.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/arviz/utils.py` & `arviz-0.9.0/arviz/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import importlib
 import functools
 import re
 import warnings
 
 import matplotlib.pyplot as plt
 import numpy as np
+import xarray as xr
 
 from numpy import newaxis
 from .rcparams import rcParams
 
 
 def _var_names(var_names, data, filter_vars=None):
     """Handle var_names input across arviz.
@@ -660,7 +661,36 @@
         raise Exception(
             "Both 'credible_interval' and 'hdi_prob' are in "
             "keyword arguments. Please remove 'credible_interval'"
         )
 
     hdi_prob = credible_interval
     return hdi_prob
+
+
+class HtmlTemplate:
+    """Contain html templates for InferenceData repr."""
+
+    html_template = """
+            <div>
+              <div class='xr-header'>
+                <div class="xr-obj-type">arviz.InferenceData</div>
+              </div>
+              <ul class="xr-sections">
+              {}
+              </ul>
+            </div>
+            """
+    element_template = """
+            <li class = "xr-section-item">
+                  <input id="idata_{group_id}" class="xr-section-summary-in" type="checkbox">
+                  <label for="idata_{group_id}" class = "xr-section-summary">{group}</label>
+                  <div class="xr-section-inline-details"></div>
+                  <div class="xr-section-details">
+                      <ul id="xr-dataset-coord-list" class="xr-var-list">
+                          <div style="padding-left:2rem;">{xr_data}<br></div>
+                      </ul>
+                  </div>
+            </li>
+            """
+    specific_style = ".xr-wrap{width:700px!important;}"
+    css_template = f"<style> {xr.core.formatting_html.CSS_STYLE}{specific_style} </style>"
```

### Comparing `arviz-0.8.3/arviz/rcparams.py` & `arviz-0.9.0/arviz/rcparams.py`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/CONTRIBUTING.md` & `arviz-0.9.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/LICENSE` & `arviz-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arviz-0.8.3/CHANGELOG.md` & `arviz-0.9.0/CHANGELOG.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,59 @@
 # Change Log
 
 ## v0.x.x Unreleased
-
 ### New features
 
 ### Maintenance and fixes
 
 ### Deprecation
 
 ### Documentation
 
+## v0.9.0 (2020 June 23)
+### New features
+* loo-pit plot. The kde is computed over the data interval (this could be shorter than [0, 1]). The HDI is computed analitically (#1215)
+* Added `html_repr` of InferenceData objects for jupyter notebooks. (#1217)
+* Added support for PyJAGS via the function `from_pyjags`. (#1219 and #1245)
+* `from_pymc3` can now retrieve `coords` and `dims` from model context (#1228, #1240 and #1249)
+* `plot_trace` now supports multiple aesthetics to identify chain and variable
+  shape and support matplotlib aliases (#1253)
+* `plot_hdi` can now take already computed HDI values (#1241)
+
+### Maintenance and fixes
+* Include data from `MultiObservedRV` to `observed_data` when using
+  `from_pymc3` (#1098)
+* Added a note on `plot_pair` when trying to use `plot_kde` on `InferenceData`
+  objects. (#1218)
+* Added `log_likelihood` argument to `from_pyro` and a warning if log likelihood cannot be obtained (#1227)
+* Skip tests on matplotlib animations if ffmpeg is not installed (#1227)
+* Fix hpd bug where arguments were being ignored (#1236)
+* Remove false positive warning in `plot_hdi` and fixed matplotlib axes generation (#1241)
+* Change the default `zorder` of scatter points from `0` to `0.6` in `plot_pair` (#1246)
+* Update `get_bins` for numpy 1.19 compatibility (#1256)
+* Fixes to `rug`, `divergences` arguments in `plot_trace` (#1253)
+
+### Deprecation
+* Using `from_pymc3` without a model context available now raises a
+  `FutureWarning` and will be deprecated in a future version (#1227)
+* In `plot_trace`, `chain_prop` and `compact_prop` as tuples will now raise a
+  `FutureWarning` (#1253)
+* `hdi` with 2d data raises a FutureWarning (#1241)
+
+### Documentation
+* A section has been added to the documentation at InferenceDataCookbook.ipynb illustrating the use of ArviZ in conjunction with PyJAGS. (#1219 and #1245)
+* Fixed inconsistent capitalization in `plot_hdi` docstring (#1221)
+* Fixed and extended `InferenceData.map` docs (#1255)
+
 ## v0.8.3 (2020 May 28)
 ### Maintenance and fixes
 * Restructured internals of `from_pymc3` to handle old pymc3 releases and
   sliced traces and to provide useful warnings (#1211)
 
+
 ## v0.8.2 (2020 May 25)
 ### Maintenance and fixes
 * Fixed bug in `from_pymc3` for sliced `pymc3.MultiTrace` input (#1209)
 
 ## v0.8.1 (2020 May 24)
 
 ### Maintenance and fixes
@@ -272,8 +307,7 @@
 
 ### Maintenance and fixes
 * Fix installation problem with release 0.3.0
 
 ## v0.3.0 (2018 Dec 14)
 
 * First Beta Release
-
```

### Comparing `arviz-0.8.3/PKG-INFO` & `arviz-0.9.0/arviz.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arviz
-Version: 0.8.3
+Version: 0.9.0
 Summary: Exploratory analysis of Bayesian models
 Home-page: http://github.com/arviz-devs/arviz
 Author: ArviZ Developers
 License: Apache-2.0
 Description: <img src="https://arviz-devs.github.io/arviz/_static/logo.png" height=100></img>
         
         [![Azure Build Status](https://dev.azure.com/ArviZ/ArviZ/_apis/build/status/arviz-devs.arviz?branchName=master)](https://dev.azure.com/ArviZ/ArviZ/_build/latest?definitionId=1&branchName=master)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: arviz Version: 0.8.3 Summary: Exploratory analysis
+Metadata-Version: 2.1 Name: arviz Version: 0.9.0 Summary: Exploratory analysis
 of Bayesian models Home-page: http://github.com/arviz-devs/arviz Author: ArviZ
 Developers License: Apache-2.0 Description: [https://arviz-devs.github.io/
 arviz/_static/logo.png] [![Azure Build Status](https://dev.azure.com/ArviZ/
 ArviZ/_apis/build/status/arviz-devs.arviz?branchName=master)](https://
 dev.azure.com/ArviZ/ArviZ/_build/latest?definitionId=1&branchName=master) [!
 [codecov](https://codecov.io/gh/arviz-devs/arviz/branch/master/graph/
 badge.svg)](https://codecov.io/gh/arviz-devs/arviz) [![Code style: black]
```

### Comparing `arviz-0.8.3/CODE_OF_CONDUCT.md` & `arviz-0.9.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

