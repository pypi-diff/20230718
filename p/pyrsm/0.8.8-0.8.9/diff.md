# Comparing `tmp/pyrsm-0.8.8.tar.gz` & `tmp/pyrsm-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrsm-0.8.8.tar", last modified: Sun Jul 16 08:56:03 2023, max compression
+gzip compressed data, was "pyrsm-0.8.9.tar", last modified: Tue Jul 18 20:36:37 2023, max compression
```

## Comparing `pyrsm-0.8.8.tar` & `pyrsm-0.8.9.tar`

### file list

```diff
@@ -1,137 +1,140 @@
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:56:03.029744 pyrsm-0.8.8/
--rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.8/LICENSE
--rw-r--r--   0 root         (0) staff       (20)      540 2023-07-16 08:48:48.000000 pyrsm-0.8.8/MANIFEST.in
--rw-r--r--   0 root         (0) staff       (20)      592 2023-07-16 08:56:03.029825 pyrsm-0.8.8/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.8.8/README.md
--rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.8/pyproject.toml
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:56:03.000013 pyrsm-0.8.8/pyrsm/
--rw-r--r--   0 root         (0) staff       (20)      311 2023-07-16 08:55:14.000000 pyrsm-0.8.8/pyrsm/__init__.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:56:03.004664 pyrsm-0.8.8/pyrsm/basics/
--rw-r--r--   0 root         (0) staff       (20)      264 2023-07-08 18:41:11.000000 pyrsm-0.8.8/pyrsm/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3940 2023-07-08 22:38:30.000000 pyrsm-0.8.8/pyrsm/basics/central_limit_theorem.py
--rw-r--r--   0 root         (0) staff       (20)     8826 2023-07-16 07:35:07.000000 pyrsm-0.8.8/pyrsm/basics/compare_means.py
--rw-r--r--   0 root         (0) staff       (20)     5267 2023-07-14 07:42:24.000000 pyrsm-0.8.8/pyrsm/basics/compare_props.py
--rw-r--r--   0 root         (0) staff       (20)     7515 2023-07-11 07:24:13.000000 pyrsm-0.8.8/pyrsm/basics/correlation.py
--rw-r--r--   0 root         (0) staff       (20)     9615 2023-07-14 07:43:27.000000 pyrsm-0.8.8/pyrsm/basics/cross_tabs.py
--rw-r--r--   0 root         (0) staff       (20)     9503 2023-07-11 07:20:45.000000 pyrsm-0.8.8/pyrsm/basics/goodness.py
--rw-r--r--   0 root         (0) staff       (20)     8394 2023-07-08 22:20:36.000000 pyrsm-0.8.8/pyrsm/basics/probability_calculator.py
--rw-r--r--   0 root         (0) staff       (20)     3939 2023-07-11 07:25:07.000000 pyrsm-0.8.8/pyrsm/basics/single_mean.py
--rw-r--r--   0 root         (0) staff       (20)     3180 2023-07-14 07:43:44.000000 pyrsm-0.8.8/pyrsm/basics/single_prop.py
--rw-r--r--   0 root         (0) staff       (20)      428 2023-07-08 18:24:21.000000 pyrsm-0.8.8/pyrsm/basics/utils.py
--rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.8/pyrsm/bins.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:56:03.005145 pyrsm-0.8.8/pyrsm/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.8/pyrsm/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)      724 2023-07-03 00:26:15.000000 pyrsm-0.8.8/pyrsm/data/__radiant-data-convert.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:56:03.008056 pyrsm-0.8.8/pyrsm/data/basics/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.8/pyrsm/data/basics/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7745 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/basics/consider.parquet
--rw-r--r--   0 root         (0) staff       (20)      785 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/basics/consider_description.md
--rw-r--r--   0 root         (0) staff       (20)    13018 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/basics/demand_uk.parquet
--rw-r--r--   0 root         (0) staff       (20)      421 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/basics/demand_uk_description.md
--rw-r--r--   0 root         (0) staff       (20)     6360 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/basics/newspaper.parquet
--rw-r--r--   0 root         (0) staff       (20)      564 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/basics/newspaper_description.md
--rw-r--r--   0 root         (0) staff       (20)     8202 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/basics/salary.parquet
--rw-r--r--   0 root         (0) staff       (20)      821 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/basics/salary_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:56:03.010670 pyrsm-0.8.8/pyrsm/data/data/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.8/pyrsm/data/data/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     3424 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/data/avengers.parquet
--rw-r--r--   0 root         (0) staff       (20)      252 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/data/avengers_description.md
--rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/data/diamonds.parquet
--rw-r--r--   0 root         (0) staff       (20)      915 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/data/diamonds_description.md
--rw-r--r--   0 root         (0) staff       (20)     2273 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/data/publishers.parquet
--rw-r--r--   0 root         (0) staff       (20)      214 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/data/publishers_description.md
--rw-r--r--   0 root         (0) staff       (20)     3415 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/data/superheroes.parquet
--rw-r--r--   0 root         (0) staff       (20)      257 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/data/superheroes_description.md
--rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/data/titanic.parquet
--rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/data/titanic_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:56:03.011180 pyrsm-0.8.8/pyrsm/data/design/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.8/pyrsm/data/design/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     4036 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/design/rndnames.parquet
--rw-r--r--   0 root         (0) staff       (20)      435 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/design/rndnames_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:56:03.016207 pyrsm-0.8.8/pyrsm/data/model/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.8/pyrsm/data/model/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     7213 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/model/catalog.parquet
--rw-r--r--   0 root         (0) staff       (20)      631 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/model/catalog_description.md
--rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-15 18:51:48.000000 pyrsm-0.8.8/pyrsm/data/model/diamonds.parquet
--rw-r--r--   0 root         (0) staff       (20)      915 2023-07-15 18:51:48.000000 pyrsm-0.8.8/pyrsm/data/model/diamonds_description.md
--rw-r--r--   0 root         (0) staff       (20)    23229 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/model/direct_marketing.parquet
--rw-r--r--   0 root         (0) staff       (20)     3198 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/model/direct_marketing_description.md
--rw-r--r--   0 root         (0) staff       (20)    39933 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/model/dvd.parquet
--rw-r--r--   0 root         (0) staff       (20)     1373 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/model/dvd_description.md
--rw-r--r--   0 root         (0) staff       (20)     1304 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/model/fraud_data_description.md
--rw-r--r--   0 root         (0) staff       (20)     6016 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/model/houseprices.parquet
--rw-r--r--   0 root         (0) staff       (20)      591 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/model/houseprices_description.md
--rw-r--r--   0 root         (0) staff       (20)    40516 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/model/ideal.parquet
--rw-r--r--   0 root         (0) staff       (20)      211 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/model/ideal_description.md
--rw-r--r--   0 root         (0) staff       (20)    26089 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/model/ketchup.parquet
--rw-r--r--   0 root         (0) staff       (20)      658 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/model/ketchup_description.md
--rw-r--r--   0 root         (0) staff       (20)     3835 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/model/ratings.parquet
--rw-r--r--   0 root         (0) staff       (20)      366 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/model/ratings_description.md
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:56:03.020389 pyrsm-0.8.8/pyrsm/data/multivariate/
--rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.8/pyrsm/data/multivariate/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     5217 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/carpet.parquet
--rw-r--r--   0 root         (0) staff       (20)      787 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/carpet_description.md
--rw-r--r--   0 root         (0) staff       (20)     3093 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/city.parquet
--rw-r--r--   0 root         (0) staff       (20)     4319 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/city2.parquet
--rw-r--r--   0 root         (0) staff       (20)      339 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/city2_description.md
--rw-r--r--   0 root         (0) staff       (20)      424 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/city_description.md
--rw-r--r--   0 root         (0) staff       (20)     6424 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/computer.parquet
--rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/computer_description.md
--rw-r--r--   0 root         (0) staff       (20)     5522 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/movie.parquet
--rw-r--r--   0 root         (0) staff       (20)      941 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/movie_description.md
--rw-r--r--   0 root         (0) staff       (20)     5226 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/mp3.parquet
--rw-r--r--   0 root         (0) staff       (20)      561 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/mp3_description.md
--rw-r--r--   0 root         (0) staff       (20)     8125 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/retailers.parquet
--rw-r--r--   0 root         (0) staff       (20)     1424 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/retailers_description.md
--rw-r--r--   0 root         (0) staff       (20)     5135 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/shopping.parquet
--rw-r--r--   0 root         (0) staff       (20)      639 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/shopping_description.md
--rw-r--r--   0 root         (0) staff       (20)     7565 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/toothpaste.parquet
--rw-r--r--   0 root         (0) staff       (20)     1080 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/toothpaste_description.md
--rw-r--r--   0 root         (0) staff       (20)     4526 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/tpbrands.parquet
--rw-r--r--   0 root         (0) staff       (20)      721 2023-07-03 00:26:28.000000 pyrsm-0.8.8/pyrsm/data/multivariate/tpbrands_description.md
--rw-r--r--   0 root         (0) staff       (20)     3617 2023-07-09 01:28:41.000000 pyrsm-0.8.8/pyrsm/example_data.py
--rw-r--r--   0 root         (0) staff       (20)     9526 2023-07-10 08:03:17.000000 pyrsm-0.8.8/pyrsm/logistic.py
--rw-r--r--   0 root         (0) staff       (20)    25699 2023-07-15 19:24:16.000000 pyrsm-0.8.8/pyrsm/model.py
--rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.8.8/pyrsm/notebook.py
--rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.8/pyrsm/perf.py
--rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.8/pyrsm/props.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:56:03.023471 pyrsm-0.8.8/pyrsm/radiant/
--rw-r--r--   0 root         (0) staff       (20)      153 2023-07-16 07:42:42.000000 pyrsm-0.8.8/pyrsm/radiant/__init__.py
--rw-r--r--   0 root         (0) staff       (20)     9387 2023-07-16 07:42:19.000000 pyrsm-0.8.8/pyrsm/radiant/compare_means.py
--rw-r--r--   0 root         (0) staff       (20)     5829 2023-07-14 07:44:09.000000 pyrsm-0.8.8/pyrsm/radiant/cross_tabs.py
--rw-r--r--   0 root         (0) staff       (20)     6284 2023-07-12 20:32:35.000000 pyrsm-0.8.8/pyrsm/radiant/goodness.py
--rw-r--r--   0 root         (0) staff       (20)     5158 2023-07-15 20:25:11.000000 pyrsm-0.8.8/pyrsm/radiant/logistic.py
--rw-r--r--   0 root         (0) staff       (20)    11074 2023-07-15 21:26:00.000000 pyrsm-0.8.8/pyrsm/radiant/model_utils.py
--rw-r--r--   0 root         (0) staff       (20)     4841 2023-07-15 20:20:45.000000 pyrsm-0.8.8/pyrsm/radiant/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5376 2023-07-15 21:24:23.000000 pyrsm-0.8.8/pyrsm/radiant/single_mean.py
--rw-r--r--   0 root         (0) staff       (20)    19570 2023-07-15 23:38:49.000000 pyrsm-0.8.8/pyrsm/radiant/utils.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:56:03.024195 pyrsm-0.8.8/pyrsm/radiant/www/
--rw-r--r--   0 root         (0) staff       (20)     6148 2023-07-15 22:58:10.000000 pyrsm-0.8.8/pyrsm/radiant/www/.DS_Store
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:56:03.025081 pyrsm-0.8.8/pyrsm/radiant/www/imgs/
--rw-r--r--   0 root         (0) staff       (20)     2374 2022-02-13 01:26:49.000000 pyrsm-0.8.8/pyrsm/radiant/www/imgs/by-nc-sa.png
--rw-r--r--   0 root         (0) staff       (20)     2284 2022-02-13 01:26:49.000000 pyrsm-0.8.8/pyrsm/radiant/www/imgs/by-sa.png
--rw-r--r--   0 root         (0) staff       (20)    82500 2022-02-13 01:26:49.000000 pyrsm-0.8.8/pyrsm/radiant/www/imgs/icon.png
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:56:03.026254 pyrsm-0.8.8/pyrsm/radiant/www/js/
--rw-r--r--   0 root         (0) staff       (20)      343 2023-07-14 07:45:06.000000 pyrsm-0.8.8/pyrsm/radiant/www/js/radiantUI.js
--rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.8.8/pyrsm/radiant/www/js/returnTextAreaBinding.js
--rw-r--r--   0 root         (0) staff       (20)     3674 2023-07-10 20:38:11.000000 pyrsm-0.8.8/pyrsm/radiant/www/js/screenshot.js
--rw-r--r--   0 root         (0) staff       (20)      550 2023-07-10 19:04:28.000000 pyrsm-0.8.8/pyrsm/radiant/www/style.css
--rw-r--r--   0 root         (0) staff       (20)     9338 2023-07-15 19:22:58.000000 pyrsm-0.8.8/pyrsm/regress.py
--rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.8/pyrsm/stats.py
--rw-r--r--   0 root         (0) staff       (20)    10294 2023-07-08 18:36:49.000000 pyrsm-0.8.8/pyrsm/utils.py
--rw-r--r--   0 root         (0) staff       (20)    22924 2023-07-14 20:26:15.000000 pyrsm-0.8.8/pyrsm/visualize.py
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:56:03.000931 pyrsm-0.8.8/pyrsm.egg-info/
--rw-r--r--   0 root         (0) staff       (20)      592 2023-07-16 08:56:02.000000 pyrsm-0.8.8/pyrsm.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) staff       (20)     3860 2023-07-16 08:56:02.000000 pyrsm-0.8.8/pyrsm.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) staff       (20)        1 2023-07-16 08:56:02.000000 pyrsm-0.8.8/pyrsm.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) staff       (20)      242 2023-07-16 08:56:02.000000 pyrsm-0.8.8/pyrsm.egg-info/requires.txt
--rw-r--r--   0 root         (0) staff       (20)        6 2023-07-16 08:56:02.000000 pyrsm-0.8.8/pyrsm.egg-info/top_level.txt
--rw-r--r--   0 root         (0) staff       (20)     1055 2023-07-16 08:56:03.030166 pyrsm-0.8.8/setup.cfg
-drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-16 08:56:03.029468 pyrsm-0.8.8/tests/
--rw-r--r--   0 root         (0) staff       (20)      841 2023-07-08 23:53:25.000000 pyrsm-0.8.8/tests/test_basics.py
--rw-r--r--   0 root         (0) staff       (20)     1183 2023-07-08 23:55:37.000000 pyrsm-0.8.8/tests/test_bins.py
--rw-r--r--   0 root         (0) staff       (20)     1027 2023-07-09 01:01:03.000000 pyrsm-0.8.8/tests/test_example_data.py
--rw-r--r--   0 root         (0) staff       (20)     3110 2023-07-08 23:57:42.000000 pyrsm-0.8.8/tests/test_perf.py
--rw-r--r--   0 root         (0) staff       (20)      670 2023-07-08 23:58:12.000000 pyrsm-0.8.8/tests/test_regression.py
--rw-r--r--   0 root         (0) staff       (20)     2223 2023-07-08 23:58:59.000000 pyrsm-0.8.8/tests/test_stats.py
--rw-r--r--   0 root         (0) staff       (20)     2230 2023-07-08 23:59:24.000000 pyrsm-0.8.8/tests/test_utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.211748 pyrsm-0.8.9/
+-rw-r--r--   0 root         (0) staff       (20)    34523 2022-03-19 20:23:12.000000 pyrsm-0.8.9/LICENSE
+-rw-r--r--   0 root         (0) staff       (20)      540 2023-07-16 08:48:48.000000 pyrsm-0.8.9/MANIFEST.in
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-18 20:36:37.211828 pyrsm-0.8.9/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     2625 2023-05-16 19:42:31.000000 pyrsm-0.8.9/README.md
+-rw-r--r--   0 root         (0) staff       (20)       80 2022-02-19 01:02:39.000000 pyrsm-0.8.9/pyproject.toml
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.183797 pyrsm-0.8.9/pyrsm/
+-rw-r--r--   0 root         (0) staff       (20)      311 2023-07-18 20:35:29.000000 pyrsm-0.8.9/pyrsm/__init__.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.185945 pyrsm-0.8.9/pyrsm/basics/
+-rw-r--r--   0 root         (0) staff       (20)      264 2023-07-18 03:05:59.000000 pyrsm-0.8.9/pyrsm/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3940 2023-07-08 22:38:30.000000 pyrsm-0.8.9/pyrsm/basics/central_limit_theorem.py
+-rw-r--r--   0 root         (0) staff       (20)     8603 2023-07-16 18:57:36.000000 pyrsm-0.8.9/pyrsm/basics/compare_means.py
+-rw-r--r--   0 root         (0) staff       (20)     5267 2023-07-14 07:42:24.000000 pyrsm-0.8.9/pyrsm/basics/compare_props.py
+-rw-r--r--   0 root         (0) staff       (20)     7515 2023-07-11 07:24:13.000000 pyrsm-0.8.9/pyrsm/basics/correlation.py
+-rw-r--r--   0 root         (0) staff       (20)     9615 2023-07-14 07:43:27.000000 pyrsm-0.8.9/pyrsm/basics/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     9503 2023-07-11 07:20:45.000000 pyrsm-0.8.9/pyrsm/basics/goodness.py
+-rw-r--r--   0 root         (0) staff       (20)     3771 2023-07-18 20:34:24.000000 pyrsm-0.8.9/pyrsm/basics/probability_calculator.py
+-rw-r--r--   0 root         (0) staff       (20)    60884 2023-07-18 20:31:46.000000 pyrsm-0.8.9/pyrsm/basics/probability_calculator_functions.py
+-rw-r--r--   0 root         (0) staff       (20)     3939 2023-07-11 07:25:07.000000 pyrsm-0.8.9/pyrsm/basics/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)     3180 2023-07-14 07:43:44.000000 pyrsm-0.8.9/pyrsm/basics/single_prop.py
+-rw-r--r--   0 root         (0) staff       (20)      428 2023-07-08 18:24:21.000000 pyrsm-0.8.9/pyrsm/basics/utils.py
+-rw-r--r--   0 root         (0) staff       (20)     2843 2023-01-31 17:36:18.000000 pyrsm-0.8.9/pyrsm/bins.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.186162 pyrsm-0.8.9/pyrsm/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.9/pyrsm/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)      724 2023-07-03 00:26:15.000000 pyrsm-0.8.9/pyrsm/data/__radiant-data-convert.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.188817 pyrsm-0.8.9/pyrsm/data/basics/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.9/pyrsm/data/basics/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7745 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/consider.parquet
+-rw-r--r--   0 root         (0) staff       (20)      785 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/consider_description.md
+-rw-r--r--   0 root         (0) staff       (20)    13018 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/demand_uk.parquet
+-rw-r--r--   0 root         (0) staff       (20)      421 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/demand_uk_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6360 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/newspaper.parquet
+-rw-r--r--   0 root         (0) staff       (20)      564 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/newspaper_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8202 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/salary.parquet
+-rw-r--r--   0 root         (0) staff       (20)      821 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/basics/salary_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.191452 pyrsm-0.8.9/pyrsm/data/data/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.9/pyrsm/data/data/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     3424 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/avengers.parquet
+-rw-r--r--   0 root         (0) staff       (20)      252 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/avengers_description.md
+-rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/diamonds.parquet
+-rw-r--r--   0 root         (0) staff       (20)      915 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/diamonds_description.md
+-rw-r--r--   0 root         (0) staff       (20)     2273 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/publishers.parquet
+-rw-r--r--   0 root         (0) staff       (20)      214 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/publishers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3415 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/superheroes.parquet
+-rw-r--r--   0 root         (0) staff       (20)      257 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/superheroes_description.md
+-rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/titanic.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/data/titanic_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.191897 pyrsm-0.8.9/pyrsm/data/design/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.9/pyrsm/data/design/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     4036 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/design/rndnames.parquet
+-rw-r--r--   0 root         (0) staff       (20)      435 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/design/rndnames_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.199981 pyrsm-0.8.9/pyrsm/data/model/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.9/pyrsm/data/model/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     7213 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/catalog.parquet
+-rw-r--r--   0 root         (0) staff       (20)      631 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/catalog_description.md
+-rw-r--r--   0 root         (0) staff       (20)    49024 2023-07-15 18:51:48.000000 pyrsm-0.8.9/pyrsm/data/model/diamonds.parquet
+-rw-r--r--   0 root         (0) staff       (20)      915 2023-07-15 18:51:48.000000 pyrsm-0.8.9/pyrsm/data/model/diamonds_description.md
+-rw-r--r--   0 root         (0) staff       (20)    23229 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/direct_marketing.parquet
+-rw-r--r--   0 root         (0) staff       (20)     3198 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/direct_marketing_description.md
+-rw-r--r--   0 root         (0) staff       (20)    39933 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/dvd.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1373 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/dvd_description.md
+-rw-r--r--   0 root         (0) staff       (20)     1304 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/fraud_data_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6016 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/houseprices.parquet
+-rw-r--r--   0 root         (0) staff       (20)      591 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/houseprices_description.md
+-rw-r--r--   0 root         (0) staff       (20)    40516 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/ideal.parquet
+-rw-r--r--   0 root         (0) staff       (20)      211 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/ideal_description.md
+-rw-r--r--   0 root         (0) staff       (20)    26089 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/ketchup.parquet
+-rw-r--r--   0 root         (0) staff       (20)      658 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/ketchup_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3835 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/ratings.parquet
+-rw-r--r--   0 root         (0) staff       (20)      366 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/model/ratings_description.md
+-rw-r--r--   0 root         (0) staff       (20)    32882 2023-07-16 09:06:55.000000 pyrsm-0.8.9/pyrsm/data/model/titanic.parquet
+-rw-r--r--   0 root         (0) staff       (20)     2061 2023-07-16 09:06:55.000000 pyrsm-0.8.9/pyrsm/data/model/titanic_description.md
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.206963 pyrsm-0.8.9/pyrsm/data/multivariate/
+-rw-r--r--   0 root         (0) staff       (20)        0 2022-02-13 01:24:09.000000 pyrsm-0.8.9/pyrsm/data/multivariate/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     5217 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/carpet.parquet
+-rw-r--r--   0 root         (0) staff       (20)      787 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/carpet_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3093 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/city.parquet
+-rw-r--r--   0 root         (0) staff       (20)     4319 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/city2.parquet
+-rw-r--r--   0 root         (0) staff       (20)      339 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/city2_description.md
+-rw-r--r--   0 root         (0) staff       (20)      424 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/city_description.md
+-rw-r--r--   0 root         (0) staff       (20)     6424 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/computer.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1038 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/computer_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5522 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/movie.parquet
+-rw-r--r--   0 root         (0) staff       (20)      941 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/movie_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5226 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/mp3.parquet
+-rw-r--r--   0 root         (0) staff       (20)      561 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/mp3_description.md
+-rw-r--r--   0 root         (0) staff       (20)     8125 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/retailers.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1424 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/retailers_description.md
+-rw-r--r--   0 root         (0) staff       (20)     5135 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/shopping.parquet
+-rw-r--r--   0 root         (0) staff       (20)      639 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/shopping_description.md
+-rw-r--r--   0 root         (0) staff       (20)     7565 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/toothpaste.parquet
+-rw-r--r--   0 root         (0) staff       (20)     1080 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/toothpaste_description.md
+-rw-r--r--   0 root         (0) staff       (20)     4526 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/tpbrands.parquet
+-rw-r--r--   0 root         (0) staff       (20)      721 2023-07-03 00:26:28.000000 pyrsm-0.8.9/pyrsm/data/multivariate/tpbrands_description.md
+-rw-r--r--   0 root         (0) staff       (20)     3617 2023-07-09 01:28:41.000000 pyrsm-0.8.9/pyrsm/example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     9375 2023-07-16 14:05:24.000000 pyrsm-0.8.9/pyrsm/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    25699 2023-07-16 14:04:41.000000 pyrsm-0.8.9/pyrsm/model.py
+-rw-r--r--   0 root         (0) staff       (20)     2214 2023-05-15 20:48:14.000000 pyrsm-0.8.9/pyrsm/notebook.py
+-rw-r--r--   0 root         (0) staff       (20)    37519 2023-04-16 05:51:16.000000 pyrsm-0.8.9/pyrsm/perf.py
+-rw-r--r--   0 root         (0) staff       (20)     1835 2022-02-13 01:24:09.000000 pyrsm-0.8.9/pyrsm/props.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.208649 pyrsm-0.8.9/pyrsm/radiant/
+-rw-r--r--   0 root         (0) staff       (20)      153 2023-07-16 07:42:42.000000 pyrsm-0.8.9/pyrsm/radiant/__init__.py
+-rw-r--r--   0 root         (0) staff       (20)     9504 2023-07-16 19:29:31.000000 pyrsm-0.8.9/pyrsm/radiant/compare_means.py
+-rw-r--r--   0 root         (0) staff       (20)     5566 2023-07-16 19:32:27.000000 pyrsm-0.8.9/pyrsm/radiant/cross_tabs.py
+-rw-r--r--   0 root         (0) staff       (20)     6572 2023-07-16 14:22:47.000000 pyrsm-0.8.9/pyrsm/radiant/goodness.py
+-rw-r--r--   0 root         (0) staff       (20)     5163 2023-07-16 14:13:07.000000 pyrsm-0.8.9/pyrsm/radiant/logistic.py
+-rw-r--r--   0 root         (0) staff       (20)    11194 2023-07-16 19:20:46.000000 pyrsm-0.8.9/pyrsm/radiant/model_utils.py
+-rw-r--r--   0 root         (0) staff       (20)     4841 2023-07-15 20:20:45.000000 pyrsm-0.8.9/pyrsm/radiant/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5376 2023-07-15 21:24:23.000000 pyrsm-0.8.9/pyrsm/radiant/single_mean.py
+-rw-r--r--   0 root         (0) staff       (20)    19570 2023-07-15 23:38:49.000000 pyrsm-0.8.9/pyrsm/radiant/utils.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.209192 pyrsm-0.8.9/pyrsm/radiant/www/
+-rw-r--r--   0 root         (0) staff       (20)     6148 2023-07-15 22:58:10.000000 pyrsm-0.8.9/pyrsm/radiant/www/.DS_Store
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.209989 pyrsm-0.8.9/pyrsm/radiant/www/imgs/
+-rw-r--r--   0 root         (0) staff       (20)     2374 2022-02-13 01:26:49.000000 pyrsm-0.8.9/pyrsm/radiant/www/imgs/by-nc-sa.png
+-rw-r--r--   0 root         (0) staff       (20)     2284 2022-02-13 01:26:49.000000 pyrsm-0.8.9/pyrsm/radiant/www/imgs/by-sa.png
+-rw-r--r--   0 root         (0) staff       (20)    82500 2022-02-13 01:26:49.000000 pyrsm-0.8.9/pyrsm/radiant/www/imgs/icon.png
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.210807 pyrsm-0.8.9/pyrsm/radiant/www/js/
+-rw-r--r--   0 root         (0) staff       (20)      343 2023-07-14 07:45:06.000000 pyrsm-0.8.9/pyrsm/radiant/www/js/radiantUI.js
+-rw-r--r--   0 root         (0) staff       (20)     1964 2023-05-23 02:45:36.000000 pyrsm-0.8.9/pyrsm/radiant/www/js/returnTextAreaBinding.js
+-rw-r--r--   0 root         (0) staff       (20)     3674 2023-07-10 20:38:11.000000 pyrsm-0.8.9/pyrsm/radiant/www/js/screenshot.js
+-rw-r--r--   0 root         (0) staff       (20)      550 2023-07-10 19:04:28.000000 pyrsm-0.8.9/pyrsm/radiant/www/style.css
+-rw-r--r--   0 root         (0) staff       (20)     9391 2023-07-16 14:02:08.000000 pyrsm-0.8.9/pyrsm/regress.py
+-rw-r--r--   0 root         (0) staff       (20)     5411 2023-03-27 22:17:11.000000 pyrsm-0.8.9/pyrsm/stats.py
+-rw-r--r--   0 root         (0) staff       (20)    10294 2023-07-08 18:36:49.000000 pyrsm-0.8.9/pyrsm/utils.py
+-rw-r--r--   0 root         (0) staff       (20)    22924 2023-07-14 20:26:15.000000 pyrsm-0.8.9/pyrsm/visualize.py
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.184442 pyrsm-0.8.9/pyrsm.egg-info/
+-rw-r--r--   0 root         (0) staff       (20)      592 2023-07-18 20:36:37.000000 pyrsm-0.8.9/pyrsm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) staff       (20)     3982 2023-07-18 20:36:37.000000 pyrsm-0.8.9/pyrsm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) staff       (20)        1 2023-07-18 20:36:37.000000 pyrsm-0.8.9/pyrsm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) staff       (20)      242 2023-07-18 20:36:37.000000 pyrsm-0.8.9/pyrsm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) staff       (20)        6 2023-07-18 20:36:37.000000 pyrsm-0.8.9/pyrsm.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) staff       (20)     1055 2023-07-18 20:36:37.212166 pyrsm-0.8.9/setup.cfg
+drwxr-xr-x   0 root         (0) staff       (20)        0 2023-07-18 20:36:37.211639 pyrsm-0.8.9/tests/
+-rw-r--r--   0 root         (0) staff       (20)      841 2023-07-08 23:53:25.000000 pyrsm-0.8.9/tests/test_basics.py
+-rw-r--r--   0 root         (0) staff       (20)     1183 2023-07-08 23:55:37.000000 pyrsm-0.8.9/tests/test_bins.py
+-rw-r--r--   0 root         (0) staff       (20)     1027 2023-07-09 01:01:03.000000 pyrsm-0.8.9/tests/test_example_data.py
+-rw-r--r--   0 root         (0) staff       (20)     3110 2023-07-08 23:57:42.000000 pyrsm-0.8.9/tests/test_perf.py
+-rw-r--r--   0 root         (0) staff       (20)      670 2023-07-08 23:58:12.000000 pyrsm-0.8.9/tests/test_regression.py
+-rw-r--r--   0 root         (0) staff       (20)     2223 2023-07-08 23:58:59.000000 pyrsm-0.8.9/tests/test_stats.py
+-rw-r--r--   0 root         (0) staff       (20)     2230 2023-07-08 23:59:24.000000 pyrsm-0.8.9/tests/test_utils.py
```

### Comparing `pyrsm-0.8.8/LICENSE` & `pyrsm-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/MANIFEST.in` & `pyrsm-0.8.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/PKG-INFO` & `pyrsm-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.8
+Version: 0.8.9
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.8/README.md` & `pyrsm-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/basics/central_limit_theorem.py` & `pyrsm-0.8.9/pyrsm/basics/central_limit_theorem.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/basics/compare_means.py` & `pyrsm-0.8.9/pyrsm/basics/compare_means.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,48 +200,44 @@
         print(f"Confidence: {self.conf}")
         print(f"Adjustment: {self.adjust}")
 
         print(self.descriptive_stats.round(dec).to_string(index=False))
 
         comp_stats = self.comp_stats.copy()
         if not extra:
-            # comp_stats = comp_stats.drop(columns=["se", "t.value", "df"])
             comp_stats = comp_stats.iloc[:, [0, 1, 2, 3, -1]]
 
         comp_stats["p.value"] = ifelse(
             comp_stats["p.value"] < 0.001, "< .001", comp_stats["p.value"]
         )
         print(comp_stats.round(dec).to_string(index=False))
 
-    def plot(self, plots: str = "hist") -> None:
+    def plot(self, plots: str = "scatter") -> None:
         if plots == "scatter":
-            sns.stripplot(data=self.data, x=self.var1, y=self.var2)
-
-            # Add horizontal lines for mean values
-            # for category, mean_value in mean_values.items():
-            #     plt.axhline(mean_value, color="blue", linestyle="--")
+            sns.swarmplot(data=self.data, x=self.var1, y=self.var2)
 
             # Get the unique categories and their indices
             categories = self.data[self.var1].cat.categories
             category_indices = {category: i for i, category in enumerate(categories)}
 
             category_means = self.data.groupby(self.var1)[self.var2].mean()
 
             # Add a horizontal line for each category at the mean of the value for that category
             for category, mean in category_means.items():
                 plt.hlines(
                     y=mean,
-                    xmin=category_indices[category] - 0.2,
-                    xmax=category_indices[category] + 0.2,
+                    xmin=category_indices[category] - 0.3,
+                    xmax=category_indices[category] + 0.3,
                     color="red",
                     linestyle="--",
+                    linewidth=3,
                 )
 
         elif plots == "box":
-            self.data.boxplot(column=self.var2, by=self.var1)
+            sns.boxplot(data=self.data, x=self.var1, y=self.var2)
         elif plots == "density":
             sns.kdeplot(data=self.data, x=self.var2, hue=self.var1)
         elif plots == "bar":
             sns.barplot(
                 data=self.data, y=self.var2, x=self.var1, errorbar=("ci", self.conf)
             )
         else:
```

### Comparing `pyrsm-0.8.8/pyrsm/basics/compare_props.py` & `pyrsm-0.8.9/pyrsm/basics/compare_props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/basics/correlation.py` & `pyrsm-0.8.9/pyrsm/basics/correlation.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/basics/cross_tabs.py` & `pyrsm-0.8.9/pyrsm/basics/cross_tabs.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/basics/goodness.py` & `pyrsm-0.8.9/pyrsm/basics/goodness.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/basics/single_mean.py` & `pyrsm-0.8.9/pyrsm/basics/single_mean.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/basics/single_prop.py` & `pyrsm-0.8.9/pyrsm/basics/single_prop.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/bins.py` & `pyrsm-0.8.9/pyrsm/bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/__radiant-data-convert.py` & `pyrsm-0.8.9/pyrsm/data/__radiant-data-convert.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/basics/consider.parquet` & `pyrsm-0.8.9/pyrsm/data/basics/consider.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/basics/consider_description.md` & `pyrsm-0.8.9/pyrsm/data/basics/consider_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/basics/demand_uk.parquet` & `pyrsm-0.8.9/pyrsm/data/basics/demand_uk.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/basics/newspaper.parquet` & `pyrsm-0.8.9/pyrsm/data/basics/newspaper.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/basics/newspaper_description.md` & `pyrsm-0.8.9/pyrsm/data/basics/newspaper_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/basics/salary.parquet` & `pyrsm-0.8.9/pyrsm/data/basics/salary.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/basics/salary_description.md` & `pyrsm-0.8.9/pyrsm/data/basics/salary_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/data/avengers.parquet` & `pyrsm-0.8.9/pyrsm/data/data/avengers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/data/diamonds.parquet` & `pyrsm-0.8.9/pyrsm/data/data/diamonds.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/data/diamonds_description.md` & `pyrsm-0.8.9/pyrsm/data/data/diamonds_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/data/publishers.parquet` & `pyrsm-0.8.9/pyrsm/data/data/publishers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/data/superheroes.parquet` & `pyrsm-0.8.9/pyrsm/data/data/superheroes.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/data/titanic.parquet` & `pyrsm-0.8.9/pyrsm/data/data/titanic.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/data/titanic_description.md` & `pyrsm-0.8.9/pyrsm/data/data/titanic_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/design/rndnames.parquet` & `pyrsm-0.8.9/pyrsm/data/design/rndnames.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/model/catalog.parquet` & `pyrsm-0.8.9/pyrsm/data/model/catalog.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/model/catalog_description.md` & `pyrsm-0.8.9/pyrsm/data/model/catalog_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/model/diamonds.parquet` & `pyrsm-0.8.9/pyrsm/data/model/diamonds.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/model/diamonds_description.md` & `pyrsm-0.8.9/pyrsm/data/model/diamonds_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/model/direct_marketing.parquet` & `pyrsm-0.8.9/pyrsm/data/model/direct_marketing.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/model/direct_marketing_description.md` & `pyrsm-0.8.9/pyrsm/data/model/direct_marketing_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/model/dvd.parquet` & `pyrsm-0.8.9/pyrsm/data/model/dvd.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/model/dvd_description.md` & `pyrsm-0.8.9/pyrsm/data/model/dvd_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/model/fraud_data_description.md` & `pyrsm-0.8.9/pyrsm/data/model/fraud_data_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/model/houseprices.parquet` & `pyrsm-0.8.9/pyrsm/data/model/houseprices.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/model/houseprices_description.md` & `pyrsm-0.8.9/pyrsm/data/model/houseprices_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/model/ideal.parquet` & `pyrsm-0.8.9/pyrsm/data/model/ideal.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/model/ketchup.parquet` & `pyrsm-0.8.9/pyrsm/data/model/ketchup.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/model/ketchup_description.md` & `pyrsm-0.8.9/pyrsm/data/model/ketchup_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/model/ratings.parquet` & `pyrsm-0.8.9/pyrsm/data/model/ratings.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/carpet.parquet` & `pyrsm-0.8.9/pyrsm/data/multivariate/carpet.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/carpet_description.md` & `pyrsm-0.8.9/pyrsm/data/multivariate/carpet_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/city.parquet` & `pyrsm-0.8.9/pyrsm/data/multivariate/city.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/city2.parquet` & `pyrsm-0.8.9/pyrsm/data/multivariate/city2.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/computer.parquet` & `pyrsm-0.8.9/pyrsm/data/multivariate/computer.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/computer_description.md` & `pyrsm-0.8.9/pyrsm/data/multivariate/computer_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/movie.parquet` & `pyrsm-0.8.9/pyrsm/data/multivariate/movie.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/movie_description.md` & `pyrsm-0.8.9/pyrsm/data/multivariate/movie_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/mp3.parquet` & `pyrsm-0.8.9/pyrsm/data/multivariate/mp3.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/mp3_description.md` & `pyrsm-0.8.9/pyrsm/data/multivariate/mp3_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/retailers.parquet` & `pyrsm-0.8.9/pyrsm/data/multivariate/retailers.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/retailers_description.md` & `pyrsm-0.8.9/pyrsm/data/multivariate/retailers_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/shopping.parquet` & `pyrsm-0.8.9/pyrsm/data/multivariate/shopping.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/shopping_description.md` & `pyrsm-0.8.9/pyrsm/data/multivariate/shopping_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/toothpaste.parquet` & `pyrsm-0.8.9/pyrsm/data/multivariate/toothpaste.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/toothpaste_description.md` & `pyrsm-0.8.9/pyrsm/data/multivariate/toothpaste_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/tpbrands.parquet` & `pyrsm-0.8.9/pyrsm/data/multivariate/tpbrands.parquet`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/data/multivariate/tpbrands_description.md` & `pyrsm-0.8.9/pyrsm/data/multivariate/tpbrands_description.md`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/example_data.py` & `pyrsm-0.8.9/pyrsm/example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/logistic.py` & `pyrsm-0.8.9/pyrsm/logistic.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,46 +1,41 @@
 from typing import Union, Optional
 import re
 import pandas as pd
 import numpy as np
 import matplotlib.pyplot as plt
 import matplotlib.ticker as ticker
-import statsmodels as sm
 from statsmodels.genmod.families import Binomial
-from statsmodels.genmod.families.links import logit
+from statsmodels.genmod.families.links import Logit
 import statsmodels.formula.api as smf
-from statsmodels.stats.outliers_influence import variance_inflation_factor
 from scipy import stats
-from scipy.special import expit
-from .utils import ifelse, setdiff, odir
-from .stats import weighted_mean, weighted_sd
-from .perf import auc
-from .model import sig_stars, model_fit, or_ci, or_plot, sim_prediction
+from .utils import ifelse, setdiff
+from .model import sig_stars, model_fit, or_ci, or_plot, sim_prediction, predict_ci
 from .model import vif as calc_vif
 
 # from statsmodels.regression.linear_model import RegressionResults as rrs
 from .visualize import pred_plot_sm, vimp_plot_sm, extract_evars, extract_rvar
 
 
 class logistic:
     def __init__(
         self,
-        data,
+        data: Union[pd.DataFrame, dict[str, pd.DataFrame]],
         rvar: Optional[str] = None,
         lev: Optional[str] = None,
         evar: Optional[list[str]] = None,
         ivar: Optional[list[str]] = None,
         form: Optional[str] = None,
     ) -> None:
         """
         Initialize logistic regression model
 
         Parameters
         ----------
-        dataset: pandas DataFrame; dataset
+        data: pandas DataFrame; dataset
         evar: List of strings; contains the names of the columns of data to be used as explanatory variables
         lev: String; name of the level in the response variable
         rvar: String; name of the column to be used as the response variable
         form: String; formula for the regression equation to use if evar and rvar are not provided
         """
         if isinstance(data, dict):
             self.name = list(data.keys())[0]
@@ -55,29 +50,29 @@
         self.form = form
 
         if self.lev is not None and self.rvar is not None:
             self.data[self.rvar] = (self.data[self.rvar] == lev).astype(int)
 
         if self.form:
             self.fitted = smf.glm(
-                formula=self.form, data=self.data, family=Binomial(link=logit())
+                formula=self.form, data=self.data, family=Binomial(link=Logit())
             ).fit()
             self.evar = extract_evars(self.fitted.model, self.data.columns)
             self.rvar = extract_rvar(self.fitted.model, self.data.columns)
             if self.lev is None:
                 self.lev = self.data.at[0, self.rvar]
         else:
             if self.evar is None or len(self.evar) == 0:
                 self.form = f"{self.rvar} ~ 1"
             else:
                 self.form = f"{self.rvar} ~ {' + '.join(self.evar)}"
             if self.ivar:
                 self.form += f" + {' + '.join(self.ivar)}"
             self.fitted = smf.glm(
-                formula=self.form, data=self.data, family=Binomial(link=logit())
+                formula=self.form, data=self.data, family=Binomial(link=Logit())
             ).fit()
         df = pd.DataFrame(np.exp(self.fitted.params), columns=["OR"]).dropna()
         df["OR%"] = 100 * ifelse(df["OR"] < 1, -(1 - df["OR"]), df["OR"] - 1)
         df["coefficient"] = self.fitted.params
         df["std.error"] = self.fitted.params / self.fitted.tvalues
         # wierd but this is what statsmodels uses in summary
         df["z.value"] = self.fitted.tvalues
@@ -242,15 +237,15 @@
         # pvalue = ifelse(out.pvalue < 0.001, "< .001", round(out.pvalue, dec))
         # print(
         #     f"Chi-squared: {round(out.statistic, dec)} df ({out.df_denom:.0f}), p.value {pvalue}"
         # )
 
         # LR test of competing models (slower but more accurate)
         sub_fitted = smf.glm(
-            formula=form, data=self.data, family=Binomial(link=logit())
+            formula=form, data=self.data, family=Binomial(link=Logit())
         ).fit()
 
         lrtest = -2 * (sub_fitted.llf - self.fitted.llf)
         df = self.fitted.df_model - sub_fitted.df_model
         pvalue = stats.chi2.sf(lrtest, df)
 
         # calculate pseudo R-squared values for both models
```

### Comparing `pyrsm-0.8.8/pyrsm/model.py` & `pyrsm-0.8.9/pyrsm/model.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/notebook.py` & `pyrsm-0.8.9/pyrsm/notebook.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/perf.py` & `pyrsm-0.8.9/pyrsm/perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/props.py` & `pyrsm-0.8.9/pyrsm/props.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/radiant/compare_means.py` & `pyrsm-0.8.9/pyrsm/radiant/compare_means.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,21 +246,25 @@
             show_code,
             estimate,
             ret="cm",
             sum_fun=rsm.basics.compare_means.summary,
             sc=summary_code,
         )
 
+        def plot_code():
+            return f"""ct.plot(output="{input.plots()}")"""
+
         mu.make_plot(
             self,
             input,
             output,
             show_code,
             estimate,
             ret="cm",
+            pc=plot_code,
         )
 
         # --- section standard for all apps ---
         # stops returning code if moved to utils
         @reactive.Effect
         @reactive.event(input.stop, ignore_none=True)
         async def stop_app():
@@ -278,15 +282,15 @@
     log_level: str = "warning",
 ):
     """
     Launch a Radiant-for-Python app for compare means hypothesis testing
     """
     if data_dct is None:
         data_dct, descriptions_dct = ru.get_dfs(pkg="basics", name="salary")
-    rc = basics_compare_means(data_dct, descriptions_dct, open)
+    rc = basics_compare_means(data_dct, descriptions_dct, open=open)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
```

### Comparing `pyrsm-0.8.8/pyrsm/radiant/cross_tabs.py` & `pyrsm-0.8.9/pyrsm/radiant/single_mean.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,179 +1,173 @@
 from shiny import App, render, ui, reactive, Inputs, Outputs, Session
 import webbrowser, nest_asyncio, uvicorn
-import io
+import signal, os
 import pyrsm as rsm
-from contextlib import redirect_stdout, redirect_stderr
 import pyrsm.radiant.utils as ru
-
-choices = {
-    "observed": "Observed",
-    "expected": "Expected",
-    "chisq": "Chi-squared",
-    "dev_std": "Deviation std.",
-    "perc_row": "Row percentages",
-    "perc_col": "Column percentages",
-    "perc": "Table percentages",
-}
+import pyrsm.radiant.model_utils as mu
 
 
 def ui_summary():
-    return ui.panel_conditional(
-        "input.tabs == 'Summary'",
-        ui.panel_well(
-            ui.output_ui("ui_var1"),
-            ui.output_ui("ui_var2"),
-            ui.input_checkbox_group(
-                id="select_output",
-                label="Select output tables:",
-                choices=choices,
+    return (
+        ui.panel_conditional(
+            "input.tabs == 'Summary'",
+            ui.panel_well(
+                ui.output_ui("ui_var"),
+                ui.input_select(
+                    id="alt_hyp",
+                    label="Alternative hypothesis:",
+                    selected="two-sided",
+                    choices={
+                        "two-sided": "Two sided",
+                        "greater": "Greater than",
+                        "less": "Less than",
+                    },
+                ),
+                ui.input_slider(
+                    id="conf",
+                    label="Confidence level:",
+                    min=0,
+                    max=1,
+                    value=0.95,
+                ),
+                ui.input_numeric(
+                    id="comp_value",
+                    label="Comparison value:",
+                    value=0,
+                ),
             ),
         ),
     )
 
 
-plots = {"None": "None"}
-plots.update(choices)
+choices = {
+    # "None": "None",
+    "hist": "Histogram",
+    # "sim": "Simulate",
+}
 
 
-class basics_cross_tabs:
+class basics_single_mean:
     def __init__(self, datasets: dict, descriptions=None, open=True) -> None:
         ru.init(self, datasets, descriptions=descriptions, open=open)
 
     def shiny_ui(self):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
-                "Basics > Cross-tabs",
+                "Basics > Single mean",
                 ui.row(
                     ui.column(
                         3,
                         ru.ui_data(self),
                         ui_summary(),
-                        ru.ui_plot(plots),
+                        ru.ui_plot(choices),
                     ),
                     ui.column(8, ru.ui_main_basics()),
                 ),
             ),
             ru.ui_help(
-                "https://github.com/vnijs/pyrsm/blob/main/examples/basics-cross-tabs.ipynb",
-                "Cross-tabs example notebook",
+                "https://github.com/vnijs/pyrsm/blob/main/examples/basics-single-mean.ipynb",
+                "Single mean example notebook",
             ),
             ru.ui_stop(),
             title="Radiant for Python",
             inverse=True,
             id="navbar_id",
         )
 
     def shiny_server(self, input: Inputs, output: Outputs, session: Session):
         # --- section standard for all apps ---
-        get_data, stop_app = ru.standard_reactives(self, input, session)
-        ru.make_data_outputs(self, input, output)
+        get_data = ru.make_data_elements(self, input, output)
 
         # --- section unique to each app ---
-        @output(id="ui_var1")
+        @output(id="ui_var")
         @render.ui
-        def ui_var1():
-            isCat = get_data()["var_types"]["isCat"]
+        def ui_var():
+            isNum = get_data()["var_types"]["isNum"]
             return ui.input_select(
-                id="var1",
-                label="Select a categorical variable:",
+                id="var",
+                label="Variable (select one)",
                 selected=None,
-                choices=isCat,
-            )
-
-        @output(id="ui_var2")
-        @render.ui
-        def ui_var2():
-            isCat = get_data()["var_types"]["isCat"]
-            if (input.var1() is not None) and (input.var1() in isCat):
-                del isCat[input.var1()]
-
-            return ui.input_select(
-                id="var2",
-                label="Select a categorical variable:",
-                selected=None,
-                choices=isCat,
+                choices=isNum,
             )
 
         def estimation_code():
             data_name, code = (get_data()[k] for k in ["data_name", "code"])
 
             args = {
                 "data": f"""{{"{data_name}": {data_name}}}""",
-                "var1": input.var1(),
-                "var2": input.var2(),
+                "var": input.var(),
+                "alt_hyp": input.alt_hyp(),
+                "conf": input.conf(),
+                "comp_value": input.comp_value(),
             }
 
-            args_string = ru.drop_default_args(args, rsm.basics.cross_tabs)
-            return f"""rsm.basics.cross_tabs({args_string})""", code
+            args_string = ru.drop_default_args(args, rsm.basics.single_mean)
+            return f"""rsm.basics.single_mean({args_string})""", code
 
-        def show_code():
-            sc = estimation_code()
-            return f"""{sc[1]}\nct = {sc[0]}"""
-
-        @reactive.Calc
-        def estimate():
-            locals()[input.datasets()] = self.datasets[
-                input.datasets()
-            ]  # get data into local scope
-            return eval(estimation_code()[0])
+        show_code, estimate = mu.make_estimate(
+            self,
+            input,
+            output,
+            get_data,
+            fun="basics.single_mean",
+            ret="sm",
+            ec=estimation_code,
+            run=False,
+            debug=True,
+        )
 
         def summary_code():
-            args = [c for c in input.select_output()]
-            return f"""ct.summary(output={args})"""
+            return f"""sm.summary()"""
+
+        mu.make_summary(
+            self,
+            input,
+            output,
+            show_code,
+            estimate,
+            ret="sm",
+            sum_fun=rsm.basics.single_mean.summary,
+            sc=summary_code,
+        )
 
-        @output(id="show_summary_code")
-        @render.text
-        def show_summary_code():
-            cmd = f"""{show_code()}\n{summary_code()}"""
-            return ru.code_formatter(cmd, self)
-
-        @output(id="summary")
-        @render.text
-        def summary():
-            out = io.StringIO()
-            with redirect_stdout(out), redirect_stderr(out):
-                ct = cross_tabs()  # get the reactive object into local scope
-                eval(summary_code())
-            return out.getvalue()
-
-        def plot_code():
-            return f"""ct.plot(output="{input.plots()}")"""
-
-        @output(id="show_plot_code")
-        @render.text
-        def show_plot_code():
-            plots = input.plots()
-            if plots != "None":
-                cmd = f"""{show_code()}\n{plot_code()}"""
-                return ru.code_formatter(cmd, self)
-
-        @output(id="plot")
-        @render.plot
-        def plot():
-            plots = input.plots()
-            if plots != "None":
-                ct = cross_tabs()  # get reactive object into local scope
-                cmd = f"""{plot_code()}"""
-                return eval(cmd)
+        mu.make_plot(
+            self,
+            input,
+            output,
+            show_code,
+            estimate,
+            ret="sm",
+        )
 
+        # --- section standard for all apps ---
+        # stops returning code if moved to utils
+        @reactive.Effect
+        @reactive.event(input.stop, ignore_none=True)
+        async def stop_app():
+            rsm.md(f"```python\n{self.stop_code}\n```")
+            await session.app.stop()
+            os.kill(os.getpid(), signal.SIGTERM)
 
-def cross_tabs(
-    data_dct: dict,
+
+def single_mean(
+    data_dct: dict = None,
     descriptions_dct: dict = None,
     open: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
 ):
     """
-    Launch a Radiant-for-Python app for linear regression analysis
+    Launch a Radiant-for-Python app for single_mean hypothesis testing
     """
-    rc = basics_cross_tabs(data_dct, descriptions_dct, open=open)
+    if data_dct is None:
+        data_dct, descriptions_dct = ru.get_dfs(pkg="basics", name="demand_uk")
+    rc = basics_single_mean(data_dct, descriptions_dct, open)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
@@ -181,12 +175,11 @@
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
     import pyrsm as rsm
 
-    newspaper, newspaper_description = rsm.load_data(pkg="basics", name="newspaper")
-    rc = cross_tabs(
-        {"newspaper": newspaper}, {"newspaper": newspaper_description}, open=True
-    )
-    app = App(rc.shiny_ui(), rc.shiny_server)
+    # demand_uk, demand_uk_description = rsm.load_data(pkg="basics", name="demand_uk")
+    # data_dct, descriptions_dct = ru.get_dfs(name="demand_uk")
+    # single_mean(data_dct, descriptions_dct, open=True)
+    single_mean()
```

### Comparing `pyrsm-0.8.8/pyrsm/radiant/goodness.py` & `pyrsm-0.8.9/pyrsm/radiant/goodness.py`

 * *Files 5% similar despite different names*

```diff
@@ -94,16 +94,15 @@
             title="Radiant for Python",
             inverse=True,
             id="navbar_id",
         )
 
     def shiny_server(self, input: Inputs, output: Outputs, session: Session):
         # --- section standard for all apps ---
-        get_data, stop_app = ru.standard_reactives(self, input, session)
-        ru.make_data_outputs(self, input, output)
+        get_data = ru.make_data_elements(self, input, output)
 
         # --- section unique to each app ---
         @output(id="ui_var")
         @render.ui
         def ui_var1():
             isCat = get_data()["var_types"]["isCat"]
             return ui.input_select(
@@ -171,14 +170,23 @@
         def plot():
             plots = input.select_plot()
             if plots != "None":
                 gf = estimate()  # get reactive object into local scope
                 cmd = f"""{plot_code()}"""
                 return eval(cmd)
 
+        # --- section standard for all apps ---
+        # stops returning code if moved to utils
+        @reactive.Effect
+        @reactive.event(input.stop, ignore_none=true)
+        async def stop_app():
+            rsm.md(f"```python\n{self.stop_code}\n```")
+            await session.app.stop()
+            os.kill(os.getpid(), signal.sigterm)
+
 
 def goodness(
     data_dct: dict,
     descriptions_dct: dict = None,
     open: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
```

### Comparing `pyrsm-0.8.8/pyrsm/radiant/logistic.py` & `pyrsm-0.8.9/pyrsm/radiant/logistic.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 import webbrowser, nest_asyncio, uvicorn, os, signal
 import pyrsm as rsm
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
 choices = {
     "None": "None",
-    "dist": "Distribution",
-    "corr": "Correlation",
-    "pred": "Prediction plot",
+    # "dist": "Distribution",
+    # "corr": "Correlation",
+    "pred": "Prediction plots",
     "vimp": "Permutation importance",
     "or": "OR plot",
 }
 
 controls = {
     "ci": "Confidence intervals",
     "vif": "VIF",
```

### Comparing `pyrsm-0.8.8/pyrsm/radiant/model_utils.py` & `pyrsm-0.8.9/pyrsm/radiant/model_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -291,29 +291,35 @@
                 summary += " (100K rows shown)"
 
             return render.DataTable(pred.round(3), summary=summary)
         else:
             return None
 
 
-def make_plot(self, input, output, show_code, estimate, ret):
-    def plot_code():
-        plots = input.plots()
-        if plots == "pred":
-            incl = list(input.incl_evar())
-            incl_int = list(input.incl_interactions())
-            cmd = f""", incl={incl}"""
-            if len(incl_int) > 0:
-                cmd += f""", incl_int={incl_int}"""
-            cmd = f"""{ret}.plot(plots="{plots}" {cmd})"""
-        elif plots == "corr":
-            cmd = f"""{ret}.plot(plots="{plots}", nobs={input.nobs()})"""
-        else:
-            cmd = f"""{ret}.plot(plots="{plots}")"""
-        return cmd
+def make_plot(self, input, output, show_code, estimate, ret, pc=None):
+
+    if pc is None:
+
+        def plot_code():
+            plots = input.plots()
+            if plots == "pred":
+                incl = list(input.incl_evar())
+                incl_int = list(input.incl_interactions())
+                cmd = f""", incl={incl}"""
+                if len(incl_int) > 0:
+                    cmd += f""", incl_int={incl_int}"""
+                cmd = f"""{ret}.plot(plots="{plots}" {cmd})"""
+            elif plots == "corr":
+                cmd = f"""{ret}.plot(plots="{plots}", nobs={input.nobs()})"""
+            else:
+                cmd = f"""{ret}.plot(plots="{plots}")"""
+            return cmd
+
+    else:
+        plot_code = pc
 
     @output(id="show_plot_code")
     @render.text
     def show_plot_code():
         plots = input.plots()
         if plots != "None":
             cmd = f"""{show_code()}\n{plot_code()}"""
```

### Comparing `pyrsm-0.8.8/pyrsm/radiant/regress.py` & `pyrsm-0.8.9/pyrsm/radiant/regress.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/radiant/single_mean.py` & `pyrsm-0.8.9/pyrsm/radiant/cross_tabs.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,173 +1,180 @@
 from shiny import App, render, ui, reactive, Inputs, Outputs, Session
 import webbrowser, nest_asyncio, uvicorn
-import signal, os
+import io, os, signal
 import pyrsm as rsm
+from contextlib import redirect_stdout, redirect_stderr
 import pyrsm.radiant.utils as ru
 import pyrsm.radiant.model_utils as mu
 
+choices = {
+    "observed": "Observed",
+    "expected": "Expected",
+    "chisq": "Chi-squared",
+    "dev_std": "Deviation std.",
+    "perc_row": "Row percentages",
+    "perc_col": "Column percentages",
+    "perc": "Table percentages",
+}
+
 
 def ui_summary():
-    return (
-        ui.panel_conditional(
-            "input.tabs == 'Summary'",
-            ui.panel_well(
-                ui.output_ui("ui_var"),
-                ui.input_select(
-                    id="alt_hyp",
-                    label="Alternative hypothesis:",
-                    selected="two-sided",
-                    choices={
-                        "two-sided": "Two sided",
-                        "greater": "Greater than",
-                        "less": "Less than",
-                    },
-                ),
-                ui.input_slider(
-                    id="conf",
-                    label="Confidence level:",
-                    min=0,
-                    max=1,
-                    value=0.95,
-                ),
-                ui.input_numeric(
-                    id="comp_value",
-                    label="Comparison value:",
-                    value=0,
-                ),
+    return ui.panel_conditional(
+        "input.tabs == 'Summary'",
+        ui.panel_well(
+            ui.output_ui("ui_var1"),
+            ui.output_ui("ui_var2"),
+            ui.input_checkbox_group(
+                id="select_output",
+                label="Select output tables:",
+                choices=choices,
             ),
         ),
     )
 
 
-choices = {
-    # "None": "None",
-    "hist": "Histogram",
-    # "sim": "Simulate",
-}
+plots = {"None": "None"}
+plots.update(choices)
 
 
-class basics_single_mean:
+class basics_cross_tabs:
     def __init__(self, datasets: dict, descriptions=None, open=True) -> None:
         ru.init(self, datasets, descriptions=descriptions, open=open)
 
     def shiny_ui(self):
         return ui.page_navbar(
             ru.head_content(),
             ui.nav(
-                "Basics > Single mean",
+                "Basics > Cross-tabs",
                 ui.row(
                     ui.column(
                         3,
                         ru.ui_data(self),
                         ui_summary(),
-                        ru.ui_plot(choices),
+                        ru.ui_plot(plots),
                     ),
                     ui.column(8, ru.ui_main_basics()),
                 ),
             ),
             ru.ui_help(
-                "https://github.com/vnijs/pyrsm/blob/main/examples/basics-single-mean.ipynb",
-                "Single mean example notebook",
+                "https://github.com/vnijs/pyrsm/blob/main/examples/basics-cross-tabs.ipynb",
+                "Cross-tabs example notebook",
             ),
             ru.ui_stop(),
             title="Radiant for Python",
             inverse=True,
             id="navbar_id",
         )
 
     def shiny_server(self, input: Inputs, output: Outputs, session: Session):
         # --- section standard for all apps ---
         get_data = ru.make_data_elements(self, input, output)
 
         # --- section unique to each app ---
-        @output(id="ui_var")
+        @output(id="ui_var1")
         @render.ui
-        def ui_var():
-            isNum = get_data()["var_types"]["isNum"]
+        def ui_var1():
+            isCat = get_data()["var_types"]["isCat"]
             return ui.input_select(
-                id="var",
-                label="Variable (select one)",
+                id="var1",
+                label="Select a categorical variable:",
                 selected=None,
-                choices=isNum,
+                choices=isCat,
+            )
+
+        @output(id="ui_var2")
+        @render.ui
+        def ui_var2():
+            isCat = get_data()["var_types"]["isCat"]
+            if (input.var1() is not None) and (input.var1() in isCat):
+                del isCat[input.var1()]
+
+            return ui.input_select(
+                id="var2",
+                label="Select a categorical variable:",
+                selected=None,
+                choices=isCat,
             )
 
         def estimation_code():
             data_name, code = (get_data()[k] for k in ["data_name", "code"])
 
             args = {
                 "data": f"""{{"{data_name}": {data_name}}}""",
-                "var": input.var(),
-                "alt_hyp": input.alt_hyp(),
-                "conf": input.conf(),
-                "comp_value": input.comp_value(),
+                "var1": input.var1(),
+                "var2": input.var2(),
             }
 
-            args_string = ru.drop_default_args(args, rsm.basics.single_mean)
-            return f"""rsm.basics.single_mean({args_string})""", code
+            args_string = ru.drop_default_args(args, rsm.basics.cross_tabs)
+            return f"""rsm.basics.cross_tabs({args_string})""", code
 
         show_code, estimate = mu.make_estimate(
             self,
             input,
             output,
             get_data,
-            fun="basics.single_mean",
-            ret="sm",
+            fun="basics.cross_tabs",
+            ret="ct",
             ec=estimation_code,
             run=False,
             debug=True,
         )
 
         def summary_code():
-            return f"""sm.summary()"""
+            args = [c for c in input.select_output()]
+            return f"""ct.summary(output={args})"""
 
         mu.make_summary(
             self,
             input,
             output,
             show_code,
             estimate,
-            ret="sm",
-            sum_fun=rsm.basics.single_mean.summary,
+            ret="ct",
+            sum_fun=rsm.basics.cross_tabs.summary,
             sc=summary_code,
         )
 
+        def plot_code():
+            return f"""ct.plot(output="{input.plots()}")"""
+
         mu.make_plot(
             self,
             input,
             output,
             show_code,
             estimate,
-            ret="sm",
+            ret="ct",
+            pc=plot_code,
         )
 
         # --- section standard for all apps ---
         # stops returning code if moved to utils
         @reactive.Effect
         @reactive.event(input.stop, ignore_none=True)
         async def stop_app():
             rsm.md(f"```python\n{self.stop_code}\n```")
             await session.app.stop()
             os.kill(os.getpid(), signal.SIGTERM)
 
 
-def single_mean(
+def cross_tabs(
     data_dct: dict = None,
     descriptions_dct: dict = None,
     open: bool = True,
     host: str = "0.0.0.0",
     port: int = 8000,
     log_level: str = "warning",
 ):
     """
-    Launch a Radiant-for-Python app for single_mean hypothesis testing
+    Launch a Radiant-for-Python app for cross-tabs hypothesis testing
     """
     if data_dct is None:
-        data_dct, descriptions_dct = ru.get_dfs(pkg="basics", name="demand_uk")
-    rc = basics_single_mean(data_dct, descriptions_dct, open)
+        data_dct, descriptions_dct = ru.get_dfs(pkg="basics", name="newspaper")
+    rc = basics_cross_tabs(data_dct, descriptions_dct, open=open)
     nest_asyncio.apply()
     webbrowser.open(f"http://{host}:{port}")
     print(f"Listening on http://{host}:{port}")
     ru.message()
     uvicorn.run(
         App(rc.shiny_ui(), rc.shiny_server),
         host=host,
@@ -175,11 +182,11 @@
         log_level=log_level,
     )
 
 
 if __name__ == "__main__":
     import pyrsm as rsm
 
-    # demand_uk, demand_uk_description = rsm.load_data(pkg="basics", name="demand_uk")
-    # data_dct, descriptions_dct = ru.get_dfs(name="demand_uk")
-    # single_mean(data_dct, descriptions_dct, open=True)
-    single_mean()
+    # newspaper, newspaper_description = rsm.load_data(pkg="basics", name="newspaper")
+    # data_dct, descriptions_dct = ru.get_dfs(name="newspaper")
+    # cross_tabs(data_dct, descriptions_dct, open=True)
+    # cross_tabs()
```

### Comparing `pyrsm-0.8.8/pyrsm/radiant/utils.py` & `pyrsm-0.8.9/pyrsm/radiant/utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/radiant/www/.DS_Store` & `pyrsm-0.8.9/pyrsm/radiant/www/.DS_Store`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/radiant/www/imgs/by-nc-sa.png` & `pyrsm-0.8.9/pyrsm/radiant/www/imgs/by-nc-sa.png`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/radiant/www/imgs/by-sa.png` & `pyrsm-0.8.9/pyrsm/radiant/www/imgs/by-sa.png`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/radiant/www/imgs/icon.png` & `pyrsm-0.8.9/pyrsm/radiant/www/imgs/icon.png`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/radiant/www/js/returnTextAreaBinding.js` & `pyrsm-0.8.9/pyrsm/radiant/www/js/returnTextAreaBinding.js`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/radiant/www/js/screenshot.js` & `pyrsm-0.8.9/pyrsm/radiant/www/js/screenshot.js`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/radiant/www/style.css` & `pyrsm-0.8.9/pyrsm/radiant/www/style.css`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/regress.py` & `pyrsm-0.8.9/pyrsm/regress.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import pandas as pd
 import re
 import statsmodels.formula.api as smf
-from typing import Optional
+from typing import Optional, Union
 from statsmodels.regression.linear_model import RegressionResults as rrs
 from .utils import ifelse, format_nr, setdiff
 from .visualize import pred_plot_sm, vimp_plot_sm
 from .model import (
     sig_stars,
     model_fit,
     extract_evars,
@@ -22,15 +22,15 @@
 from .visualize import distr_plot
 from .basics.correlation import correlation
 
 
 class regress:
     def __init__(
         self,
-        data,
+        data: Union[pd.DataFrame, dict[str, pd.DataFrame]],
         rvar: Optional[str] = None,
         evar: Optional[list[str]] = None,
         ivar: Optional[list[str]] = None,
         form: Optional[str] = None,
     ) -> None:
 
         """
```

### Comparing `pyrsm-0.8.8/pyrsm/stats.py` & `pyrsm-0.8.9/pyrsm/stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/utils.py` & `pyrsm-0.8.9/pyrsm/utils.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm/visualize.py` & `pyrsm-0.8.9/pyrsm/visualize.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/pyrsm.egg-info/PKG-INFO` & `pyrsm-0.8.9/pyrsm.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrsm
-Version: 0.8.8
+Version: 0.8.9
 Summary: Python functions for Customer Analytics at the Rady School of Management (RSM)
 Author: Vincent Nijs <vnijs@ucsd.edu>, Vikram Jambulapati <vikjam@ucsd.edu>, Suhas Goutham <sgoutham@ucsd.edu>, Raghav Prasad <rprasad@ucsd.edu>
 Author-email: vnijs@ucsd.edu
 License: AGPL-3.0-only
 Project-URL: Bug Reports, https://github.com/vnijs/pyrsm/issues
 Project-URL: Source, https://github.com/vnijs/pyrsm
 Description-Content-Type: text/markdown
```

### Comparing `pyrsm-0.8.8/pyrsm.egg-info/SOURCES.txt` & `pyrsm-0.8.9/pyrsm.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 pyrsm/basics/central_limit_theorem.py
 pyrsm/basics/compare_means.py
 pyrsm/basics/compare_props.py
 pyrsm/basics/correlation.py
 pyrsm/basics/cross_tabs.py
 pyrsm/basics/goodness.py
 pyrsm/basics/probability_calculator.py
+pyrsm/basics/probability_calculator_functions.py
 pyrsm/basics/single_mean.py
 pyrsm/basics/single_prop.py
 pyrsm/basics/utils.py
 pyrsm/data/__init__.py
 pyrsm/data/__radiant-data-convert.py
 pyrsm/data/basics/__init__.py
 pyrsm/data/basics/consider.parquet
@@ -70,14 +71,16 @@
 pyrsm/data/model/houseprices_description.md
 pyrsm/data/model/ideal.parquet
 pyrsm/data/model/ideal_description.md
 pyrsm/data/model/ketchup.parquet
 pyrsm/data/model/ketchup_description.md
 pyrsm/data/model/ratings.parquet
 pyrsm/data/model/ratings_description.md
+pyrsm/data/model/titanic.parquet
+pyrsm/data/model/titanic_description.md
 pyrsm/data/multivariate/__init__.py
 pyrsm/data/multivariate/carpet.parquet
 pyrsm/data/multivariate/carpet_description.md
 pyrsm/data/multivariate/city.parquet
 pyrsm/data/multivariate/city2.parquet
 pyrsm/data/multivariate/city2_description.md
 pyrsm/data/multivariate/city_description.md
```

### Comparing `pyrsm-0.8.8/setup.cfg` & `pyrsm-0.8.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/tests/test_basics.py` & `pyrsm-0.8.9/tests/test_basics.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/tests/test_bins.py` & `pyrsm-0.8.9/tests/test_bins.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/tests/test_example_data.py` & `pyrsm-0.8.9/tests/test_example_data.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/tests/test_perf.py` & `pyrsm-0.8.9/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/tests/test_regression.py` & `pyrsm-0.8.9/tests/test_regression.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/tests/test_stats.py` & `pyrsm-0.8.9/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `pyrsm-0.8.8/tests/test_utils.py` & `pyrsm-0.8.9/tests/test_utils.py`

 * *Files identical despite different names*

