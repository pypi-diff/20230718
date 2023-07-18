# Comparing `tmp/kabutobashi-0.7.0.tar.gz` & `tmp/kabutobashi-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kabutobashi-0.7.0.tar", last modified: Fri Jul 14 03:44:21 2023, max compression
+gzip compressed data, was "kabutobashi-0.7.1.tar", last modified: Tue Jul 18 04:50:54 2023, max compression
```

## Comparing `kabutobashi-0.7.0.tar` & `kabutobashi-0.7.1.tar`

### file list

```diff
@@ -1,81 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.728854 kabutobashi-0.7.0/kabutobashi/
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.728854 kabutobashi-0.7.0/kabutobashi/application/
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/application/applications.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/application/crawl_application.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/application/di_container.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/domain/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/aggregates/
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/domain/aggregates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/domain/aggregates/single_code.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/entity/
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-14 03:44:12.000000 kabutobashi-0.7.0/kabutobashi/domain/entity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14511 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/entity/stock.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/serialize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/services/
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/services/converter/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/converter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/converter/to_entity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/services/decode_html/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/decode_html/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/decode_html/html_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/decode_html/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/services/method/
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6473 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/adx.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/basic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/bollinger_bands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/fitting.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/ichimoku.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/industry_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/macd.py
--rw-r--r--   0 runner    (1001) docker     (123)    10642 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/momentum.py
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/pct_change.py
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/psycho_logical.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/sma.py
--rw-r--r--   0 runner    (1001) docker     (123)     5497 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/stochastics.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/services/method/volatility.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/domain/values/
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/values/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/values/decoded_html_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/values/raw_html_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/values/stock_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/domain/values/user_agent.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/example_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/infrastructure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/kabutobashi/infrastructure/repository/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/infrastructure/repository/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/infrastructure/repository/html_page_repository.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/kabutobashi/utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.728854 kabutobashi-0.7.0/kabutobashi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-14 03:44:21.000000 kabutobashi-0.7.0/kabutobashi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-07-14 03:44:21.000000 kabutobashi-0.7.0/kabutobashi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 03:44:21.000000 kabutobashi-0.7.0/kabutobashi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-14 03:44:21.000000 kabutobashi-0.7.0/kabutobashi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-14 03:44:21.000000 kabutobashi-0.7.0/kabutobashi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-14 03:44:21.736854 kabutobashi-0.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/test/test_application/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/test_application/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/test_application/test_crawl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:21.732854 kabutobashi-0.7.0/test/test_domain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/test_domain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/test_domain/test_entities.py
--rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/test_domain/test_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/test_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-14 03:44:13.000000 kabutobashi-0.7.0/test/test_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:54.010838 kabutobashi-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-18 04:50:54.010838 kabutobashi-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:53.998838 kabutobashi-0.7.1/kabutobashi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:54.002838 kabutobashi-0.7.1/kabutobashi/application/
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1101 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/application/applications.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/application/crawl_application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/application/di_container.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:54.002838 kabutobashi-0.7.1/kabutobashi/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:54.002838 kabutobashi-0.7.1/kabutobashi/domain/aggregates/
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/aggregates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4659 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/aggregates/single_code.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:54.002838 kabutobashi-0.7.1/kabutobashi/domain/entity/
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/entity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14511 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/entity/stock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/serialize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:54.006838 kabutobashi-0.7.1/kabutobashi/domain/services/
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:54.006838 kabutobashi-0.7.1/kabutobashi/domain/services/converter/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/converter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/converter/to_entity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:54.006838 kabutobashi-0.7.1/kabutobashi/domain/services/decode_html/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/decode_html/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7272 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/decode_html/html_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/decode_html/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:54.006838 kabutobashi-0.7.1/kabutobashi/domain/services/method/
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/method/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/method/adx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/method/basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/method/bollinger_bands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3045 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/method/fitting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2397 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/method/ichimoku.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3182 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/method/industry_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/method/macd.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10624 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/method/method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/method/momentum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1471 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/method/pct_change.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/method/psycho_logical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/method/sma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5415 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/method/stochastics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/services/method/volatility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:54.006838 kabutobashi-0.7.1/kabutobashi/domain/values/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/values/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4319 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/values/decoded_html_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/values/raw_html_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/values/stock_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/domain/values/user_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/example_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:54.006838 kabutobashi-0.7.1/kabutobashi/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/infrastructure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:54.006838 kabutobashi-0.7.1/kabutobashi/infrastructure/repository/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/infrastructure/repository/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3413 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/infrastructure/repository/html_page_repository.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/kabutobashi/utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:53.998838 kabutobashi-0.7.1/kabutobashi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3094 2023-07-18 04:50:53.000000 kabutobashi-0.7.1/kabutobashi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2394 2023-07-18 04:50:53.000000 kabutobashi-0.7.1/kabutobashi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 04:50:53.000000 kabutobashi-0.7.1/kabutobashi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-07-18 04:50:53.000000 kabutobashi-0.7.1/kabutobashi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-07-18 04:50:53.000000 kabutobashi-0.7.1/kabutobashi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-18 04:50:54.010838 kabutobashi-0.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:54.006838 kabutobashi-0.7.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      546 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:54.006838 kabutobashi-0.7.1/test/test_application/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/test/test_application/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/test/test_application/test_crawl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:54.010838 kabutobashi-0.7.1/test/test_domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/test/test_domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/test/test_domain/test_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14508 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/test/test_domain/test_entities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5775 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/test/test_domain/test_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/test/test_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1887 2023-07-18 04:50:43.000000 kabutobashi-0.7.1/test/test_utilities.py
```

### Comparing `kabutobashi-0.7.0/LICENSE` & `kabutobashi-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/PKG-INFO` & `kabutobashi-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kabutobashi
-Version: 0.7.0
+Version: 0.7.1
 Summary: Analyze stock
 Home-page: https://github.com/gsy0911/kabutobashi
 Author: gsy0911
 Author-email: yoshiki0911@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `kabutobashi-0.7.0/README.md` & `kabutobashi-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/__init__.py` & `kabutobashi-0.7.1/kabutobashi/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 # estimate filters
 sa_fundamental = SaFundamental()
 sa_volume = SaVolume()
 
 stock_analysis = [sa_fundamental, sa_volume]
 
 # comparable tuple
-VERSION = (0, 7, 0)
+VERSION = (0, 7, 1)
 # generate __version__ via VERSION tuple
 __version__ = ".".join(map(str, VERSION))
 
 # module level doc-string
 __doc__ = """
 kabutobashi
 ===========
```

### Comparing `kabutobashi-0.7.0/kabutobashi/application/applications.py` & `kabutobashi-0.7.1/kabutobashi/application/applications.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/application/crawl_application.py` & `kabutobashi-0.7.1/kabutobashi/application/crawl_application.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/application/di_container.py` & `kabutobashi-0.7.1/kabutobashi/application/di_container.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/aggregates/single_code.py` & `kabutobashi-0.7.1/kabutobashi/domain/aggregates/single_code.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/entity/stock.py` & `kabutobashi-0.7.1/kabutobashi/domain/entity/stock.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/errors.py` & `kabutobashi-0.7.1/kabutobashi/domain/errors.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/serialize.py` & `kabutobashi-0.7.1/kabutobashi/domain/serialize.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/analyze.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/analyze.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/converter/to_entity.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/converter/to_entity.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/decode_html/html_info.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/decode_html/html_info.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/decode_html/utils.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/decode_html/utils.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/method/__init__.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/method/__init__.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/method/adx.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/method/adx.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-from dataclasses import dataclass
-
 import pandas as pd
 
 from .method import Method, MethodType, ProcessMethod, VisualizeMethod
 
 
-@dataclass(frozen=True)
 class AdxProcess(ProcessMethod):
     """
     相場のトレンドの強さを見るための指標である`ADX`を計算するクラス。
 
     以下の指標を計算するクラス
 
     * +DI: 株価の上昇の大きさ
@@ -166,15 +163,14 @@
         return {
             "adx_dx": df_p["DX"].tail(3).mean(),
             "adx_adx": df_p["ADX"].tail(3).mean(),
             "adx_adxr": df_p["ADXR"].tail(3).mean(),
         }
 
 
-@dataclass(frozen=True)
 class AdxVisualize(VisualizeMethod):
     """
     相場のトレンドの強さを見るための指標である`ADX`を計算するクラス。
 
     以下の指標を計算するクラス
 
     * +DI: 株価の上昇の大きさ
```

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/method/basic.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/method/momentum.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,52 +1,51 @@
-from dataclasses import dataclass
-
 import pandas as pd
 
-from .method import Method, MethodType, ProcessMethod
+from .method import Method, MethodType, ProcessMethod, VisualizeMethod
 
 
-@dataclass(frozen=True)
-class BasicProcess(ProcessMethod):
+class MomentumProcess(ProcessMethod):
     """
-    株のvolumeやPBR, PSR, PERなどの値を返す。
-    parameterizeのみに利用される。
+    See Also:
+        https://www.sevendata.co.jp/shihyou/technical/momentum.html
     """
 
-    method_name: str = "basic"
-    method_type: MethodType = MethodType.PARAMETERIZE
+    term: int = 25
+    method_name: str = "momentum"
+    method_type: MethodType = MethodType.TECHNICAL_ANALYSIS
 
     def _apply(self, df: pd.DataFrame) -> pd.DataFrame:
+        df = df.assign(
+            momentum=df["close"].shift(10),
+        ).fillna(0)
+        df = df.assign(sma_momentum=lambda x: x["momentum"].rolling(self.term).mean())
         return df
 
     def _signal(self, df: pd.DataFrame) -> pd.DataFrame:
-        df_ = df.copy()
-        df_["diff"] = -1
-        # 正負が交差した点
-        df_ = df_.join(self._cross(df_["diff"]))
-        df_ = df_.rename(columns={"to_plus": "buy_signal", "to_minus": "sell_signal"})
-        return df_
+        df = df.join(self._cross(df["sma_momentum"]))
+        df = df.rename(columns={"to_plus": "buy_signal", "to_minus": "sell_signal"})
+        return df
 
     def _processed_columns(self) -> list:
-        return []
+        return ["momentum", "sma_momentum"]
 
     def _parameterize(self, df_x: pd.DataFrame, df_p: pd.DataFrame) -> dict:
-        try:
-            pbr = float(list(df_x["pbr"])[-1])
-        except ValueError:
-            pbr = 0
-        try:
-            per = float(list(df_x["per"])[-1])
-        except ValueError:
-            per = 0
-        try:
-            psr = float(list(df_x["psr"])[-1])
-        except ValueError:
-            psr = 0
-        try:
-            volume = float(list(df_x["volume"])[-1])
-        except ValueError:
-            volume = 0
-        return {"pbr": pbr, "psr": psr, "per": per, "volume": volume}
+        return {}
+
+
+class MomentumVisualize(VisualizeMethod):
+    """
+    See Also:
+        https://www.sevendata.co.jp/shihyou/technical/momentum.html
+    """
+
+    def _color_mapping(self) -> list:
+        return [
+            {"df_key": "momentum", "color": "", "label": "momentum"},
+            {"df_key": "sma_momentum", "color": "", "label": "sma_momentum"},
+        ]
+
+    def _visualize_option(self) -> dict:
+        return {"position": "lower"}
 
 
-basic = Method.of(process_method=BasicProcess(), visualize_method=None)
+momentum = Method.of(process_method=MomentumProcess(), visualize_method=MomentumVisualize())
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/method/bollinger_bands.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/method/bollinger_bands.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-from dataclasses import dataclass
-
 import pandas as pd
 
 from .method import Method, MethodType, ProcessMethod, VisualizeMethod
 
 
-@dataclass(frozen=True)
 class BollingerBandsProcess(ProcessMethod):
     """
     株価の勢いの変化や反転の目安、方向を見る ``BollingerBands`` を計算するクラス。
 
     See Also:
         * https://www.sevendata.co.jp/shihyou/technical/bori.html
     """
@@ -60,15 +57,14 @@
             "upper_1_sigma": df_p["upper_1_sigma"].tail(3).mean(),
             "lower_1_sigma": df_p["lower_1_sigma"].tail(3).mean(),
             "upper_2_sigma": df_p["upper_2_sigma"].tail(3).mean(),
             "lower_2_sigma": df_p["lower_2_sigma"].tail(3).mean(),
         }
 
 
-@dataclass(frozen=True)
 class BollingerBandsVisualize(VisualizeMethod):
     """
     株価の勢いの変化や反転の目安、方向を見る ``BollingerBands`` を計算するクラス。
 
     See Also:
         * https://www.sevendata.co.jp/shihyou/technical/bori.html
     """
```

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/method/fitting.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/method/fitting.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,17 +1,14 @@
-from dataclasses import dataclass
-
 import numpy as np
 import pandas as pd
 from scipy.optimize import curve_fit
 
 from .method import Method, MethodType, ProcessMethod, VisualizeMethod
 
 
-@dataclass(frozen=True)
 class FittingProcess(ProcessMethod):
     """
     1次、2次、3次の関数でfittingした値を返す
     """
 
     method_name: str = "fitting"
     method_type: MethodType = MethodType.TECHNICAL_ANALYSIS
@@ -69,15 +66,14 @@
             "cube_x_3": cube_param[0],
             "cube_x_2": cube_param[1],
             "cube_x_1": cube_param[2],
             "cube_x_0": cube_param[3],
         }
 
 
-@dataclass(frozen=True)
 class FittingVisualize(VisualizeMethod):
     """
     1次、2次、3次の関数でfittingした値を返す
     """
 
     def _color_mapping(self) -> list:
         return [
```

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/method/ichimoku.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/method/ichimoku.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-from dataclasses import dataclass
-
 import pandas as pd
 
 from .method import Method, MethodType, ProcessMethod, VisualizeMethod
 
 
-@dataclass(frozen=True)
 class IchimokuProcess(ProcessMethod):
     """
 
     See Also:
         https://kabu.com/investment/guide/technical/04.html
     """
 
@@ -55,15 +52,14 @@
     def _processed_columns(self) -> list:
         return ["line_change", "line_base", "proceeding_span_1", "proceeding_span_2", "delayed_span"]
 
     def _parameterize(self, df_x: pd.DataFrame, df_p: pd.DataFrame) -> dict:
         return {}
 
 
-@dataclass(frozen=True)
 class IchimokuVisualize(VisualizeMethod):
     """
 
     See Also:
         https://kabu.com/investment/guide/technical/04.html
     """
```

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/method/industry_cat.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/method/industry_cat.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,60 +1,22 @@
-from dataclasses import dataclass
-
 import pandas as pd
 
 from kabutobashi.domain.errors import KabutobashiMethodError
 
 from .method import Method, MethodType, ProcessMethod
 
 
-@dataclass(frozen=True)
 class IndustryCategoriesProcess(ProcessMethod):
     """
     株のvolumeやPBR, PSR, PERなどの値を返す。
     parameterizeのみに利用される。
     """
 
     method_name: str = "industry_categories"
     method_type: MethodType = MethodType.PARAMETERIZE
-    INDUSTRY_TYPE_MAPPING = {
-        "水産・農林業": "industry_fisheries_agriculture",
-        "鉱業": "industry_mining",
-        "建設業": "industry_construction",
-        "食料品": "industry_food",
-        "繊維製品": "industry_fiber",
-        "パルプ・紙": "industry_pulp_paper",
-        "化学": "industry_chemistry",
-        "医薬品": "industry_pharmaceuticals",
-        "石油・石炭製品": "industry_oil_coal",
-        "ゴム製品": "industry_rubber",
-        "ガラス・土石製品": "industry_glass",
-        "鉄鋼": "industry_steel",
-        "非鉄金属": "industry_non_ferrous_metals",
-        "金属製品": "industry_metal_products",
-        "機械": "industry_machine",
-        "電気機器": "industry_electric",
-        "輸送用機器": "industry_transportation",
-        "精密機器": "industry_mechanical_equipment",
-        "その他製品": "industry_other",
-        "電気・ガス業": "industry_electricity_gas",
-        "陸運業": "industry_land_transportation",
-        "海運業": "industry_shipping",
-        "空運業": "industry_air_freight",
-        "倉庫・運輸関連業": "industry_warehouse",
-        "情報・通信業": "industry_information",
-        "卸売業": "industry_wholesale",
-        "小売業": "industry_retail",
-        "銀行業": "industry_back",
-        "証券、商品先物取引業": "industry_stock_future",
-        "保険業": "industry_insurance",
-        "その他金融業": "industry_financial",
-        "不動産業": "industry_real_state",
-        "サービス業": "industry_service",
-    }
 
     def _apply(self, df: pd.DataFrame) -> pd.DataFrame:
         return df
 
     def _signal(self, df: pd.DataFrame) -> pd.DataFrame:
         df_ = df.copy()
         df_["diff"] = -1
@@ -63,18 +25,53 @@
         df_ = df_.rename(columns={"to_plus": "buy_signal", "to_minus": "sell_signal"})
         return df_
 
     def _processed_columns(self) -> list:
         return []
 
     def _parameterize(self, df_x: pd.DataFrame, df_p: pd.DataFrame) -> dict:
-        params = {v: 0 for v in self.INDUSTRY_TYPE_MAPPING.values()}
+        industry_type_mapping = {
+            "水産・農林業": "industry_fisheries_agriculture",
+            "鉱業": "industry_mining",
+            "建設業": "industry_construction",
+            "食料品": "industry_food",
+            "繊維製品": "industry_fiber",
+            "パルプ・紙": "industry_pulp_paper",
+            "化学": "industry_chemistry",
+            "医薬品": "industry_pharmaceuticals",
+            "石油・石炭製品": "industry_oil_coal",
+            "ゴム製品": "industry_rubber",
+            "ガラス・土石製品": "industry_glass",
+            "鉄鋼": "industry_steel",
+            "非鉄金属": "industry_non_ferrous_metals",
+            "金属製品": "industry_metal_products",
+            "機械": "industry_machine",
+            "電気機器": "industry_electric",
+            "輸送用機器": "industry_transportation",
+            "精密機器": "industry_mechanical_equipment",
+            "その他製品": "industry_other",
+            "電気・ガス業": "industry_electricity_gas",
+            "陸運業": "industry_land_transportation",
+            "海運業": "industry_shipping",
+            "空運業": "industry_air_freight",
+            "倉庫・運輸関連業": "industry_warehouse",
+            "情報・通信業": "industry_information",
+            "卸売業": "industry_wholesale",
+            "小売業": "industry_retail",
+            "銀行業": "industry_back",
+            "証券、商品先物取引業": "industry_stock_future",
+            "保険業": "industry_insurance",
+            "その他金融業": "industry_financial",
+            "不動産業": "industry_real_state",
+            "サービス業": "industry_service",
+        }
+        params = {v: 0 for v in industry_type_mapping.values()}
         industry_type_list = list(df_x["industry_type"].unique())
         if len(industry_type_list) > 1:
             raise KabutobashiMethodError("industry type should be 1")
         key = industry_type_list[0]
-        if key in self.INDUSTRY_TYPE_MAPPING.keys():
-            params.update({self.INDUSTRY_TYPE_MAPPING[key]: 1})
+        if key in industry_type_mapping.keys():
+            params.update({industry_type_mapping[key]: 1})
         return params
 
 
 industry_categories = Method.of(process_method=IndustryCategoriesProcess(), visualize_method=None)
```

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/method/macd.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/method/macd.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-from dataclasses import dataclass
-
 import pandas as pd
 
 from .method import Method, MethodType, ProcessMethod, VisualizeMethod
 
 
-@dataclass(frozen=True)
 class MacdProcess(ProcessMethod):
     """
     macdを基準として今後上昇するかどうかをスコアで返す。
     値が大きければその傾向が高いことを表している。
     最小値は0で、最大値は無限大である。
     """
 
@@ -41,15 +38,14 @@
     def _processed_columns(self) -> list:
         return ["ema_short", "ema_long", "signal", "macd", "histogram"]
 
     def _parameterize(self, df_x: pd.DataFrame, df_p: pd.DataFrame) -> dict:
         return {"signal": df_p["signal"].tail(3).mean(), "histogram": df_p["histogram"].tail(3).mean()}
 
 
-@dataclass(frozen=True)
 class MacdVisualize(VisualizeMethod):
     """
     macdを基準として今後上昇するかどうかをスコアで返す。
     値が大きければその傾向が高いことを表している。
     最小値は0で、最大値は無限大である。
     """
```

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/method/method.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/method/method.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,32 @@
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
 from enum import Enum, auto
 from typing import Optional
 
 import matplotlib.dates as mdates
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 from mplfinance.original_flavor import candlestick_ohlc
+from pydantic import BaseModel, ConfigDict
 
 from kabutobashi.domain.errors import KabutobashiEntityError
 from kabutobashi.domain.values import StockDataProcessed, StockDataVisualized
 
 __all__ = ["ProcessMethod", "VisualizeMethod", "Method", "MethodType"]
 
 
 class MethodType(Enum):
     TECHNICAL_ANALYSIS = auto()
     PARAMETERIZE = auto()
     CROSS_SECTION = auto()
     SIGNAL_PROCESSING = auto()
 
 
-@dataclass(frozen=True)  # type: ignore
-class ProcessMethod(ABC):
+class ProcessMethod(ABC, BaseModel):
     """
     株のテクニカル分析に関するメソッドを提供するクラス
 
     Examples:
         >>> import pandas as pd
         >>> import kabutobashi as kb
         >>> stock_df: pd.DataFrame = pd.DataFrame("path_to_stock_data")
@@ -41,14 +40,15 @@
         >>> sma_signal = stock_df.pipe(kb.macd, impact="true", influence=5, tail=5)
     """
 
     # 名前
     method_name: str
     # 種類:
     method_type: MethodType
+    model_config = ConfigDict(arbitrary_types_allowed=True)
 
     def process(self, df: pd.DataFrame, influence: int = 2, tail: int = 5) -> "StockDataProcessed":
         code_list = list(set(df["code"].values))
         if len(code_list) != 1:
             raise KabutobashiEntityError
         # 日時
         start_at = list(df["dt"])[0]
@@ -202,16 +202,15 @@
         df["buy_impact"] = df["buy_signal"].ewm(span=influence).mean()
         df["sell_impact"] = df["sell_signal"].ewm(span=influence).mean()
         buy_impact_index = df["buy_impact"].iloc[-tail:].sum()
         sell_impact_index = df["sell_impact"].iloc[-tail:].sum()
         return round(buy_impact_index - sell_impact_index, 5)
 
 
-@dataclass(frozen=True)  # type: ignore
-class VisualizeMethod(ABC):
+class VisualizeMethod(ABC, BaseModel):
     def color_mapping(self) -> list:
         return self._color_mapping()
 
     @abstractmethod
     def _color_mapping(self) -> list:
         raise NotImplementedError("please implement your code")  # pragma: no cover
 
@@ -305,15 +304,14 @@
             pass
         else:
             raise KabutobashiEntityError()
 
         return fig
 
 
-@dataclass(frozen=True)  # type: ignore
-class Method:
+class Method(BaseModel):
     process_method: ProcessMethod
     visualize_method: Optional[VisualizeMethod]
 
     @staticmethod
     def of(process_method: ProcessMethod, visualize_method: Optional[VisualizeMethod]):
         return Method(process_method=process_method, visualize_method=visualize_method)
```

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/method/pct_change.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/method/pct_change.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-from dataclasses import dataclass
-
 import pandas as pd
 
 from .method import Method, MethodType, ProcessMethod, VisualizeMethod
 
 
-@dataclass(frozen=True)
 class PctChangeProcess(ProcessMethod):
     """
     変化率を計算する
     """
 
     method_name: str = "pct_change"
     method_type: MethodType = MethodType.PARAMETERIZE
@@ -33,15 +30,14 @@
         pct_10 = df_x["close"].pct_change(10).mean()
         pct_20 = df_x["close"].pct_change(20).mean()
         pct_30 = df_x["close"].pct_change(30).mean()
         pct_40 = df_x["close"].pct_change(40).mean()
         return {"pct_05": pct_05, "pct_10": pct_10, "pct_20": pct_20, "pct_30": pct_30, "pct_40": pct_40}
 
 
-@dataclass(frozen=True)
 class PctChangeVisualize(VisualizeMethod):
     """
     変化率を計算する
     """
 
     def _color_mapping(self) -> list:
         return []
```

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/method/psycho_logical.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/method/psycho_logical.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-from dataclasses import dataclass
-
 import pandas as pd
 
 from .method import Method, MethodType, ProcessMethod, VisualizeMethod
 
 
-@dataclass(frozen=True)
 class PsychoLogicalProcess(ProcessMethod):
     """
     See Also:
         https://www.sevendata.co.jp/shihyou/technical/psycho.html
     """
 
     upper_threshold: float = 0.75
@@ -41,15 +38,14 @@
     def _processed_columns(self) -> list:
         return ["psycho_line", "bought_too_much", "sold_too_much"]
 
     def _parameterize(self, df_x: pd.DataFrame, df_p: pd.DataFrame) -> dict:
         return {"psycho_line": df_p["psycho_line"].tail(3).mean()}
 
 
-@dataclass(frozen=True)
 class PsychoLogicalVisualize(VisualizeMethod):
     """
     See Also:
         https://www.sevendata.co.jp/shihyou/technical/psycho.html
     """
 
     def _color_mapping(self) -> list:
```

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/method/sma.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/method/sma.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-from dataclasses import dataclass
-
 import pandas as pd
 
 from .method import Method, MethodType, ProcessMethod, VisualizeMethod
 
 
-@dataclass(frozen=True)
 class SmaProcess(ProcessMethod):
     """
     SMAを計算する
     """
 
     short_term: int = 5
     medium_term: int = 21
@@ -48,15 +45,14 @@
             "sma_medium_diff": df_p["sma_medium_diff"].tail(3).mean(),
             "sma_long_diff": df_p["sma_long_diff"].tail(3).mean(),
             "sma_long_short": df_p["sma_long_short"].tail(3).mean(),
             "sma_long_medium": df_p["sma_long_medium"].tail(3).mean(),
         }
 
 
-@dataclass(frozen=True)
 class SmaVisualize(VisualizeMethod):
     """
     SMAを計算する
     """
 
     short_term: int = 5
     medium_term: int = 21
```

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/method/stochastics.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/method/stochastics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 import math
-from dataclasses import dataclass
 
 import pandas as pd
 
 from .method import Method, MethodType, ProcessMethod, VisualizeMethod
 
 
-@dataclass(frozen=True)
 class StochasticsProcess(ProcessMethod):
     """
     買いのシグナルを計算で求める
 
     * %K・%D共に20％以下の時に、%Kが%Dを下から上抜いた時
     * %D・スロー%D共に20％以下の時に、%Dがスロー%Dを下から上抜いた時
 
@@ -113,15 +111,14 @@
         return {
             "stochastics_k": df_p["K"].tail(3).mean(),
             "stochastics_d": df_p["D"].tail(3).mean(),
             "stochastics_sd": df_p["SD"].tail(3).mean(),
         }
 
 
-@dataclass(frozen=True)
 class StochasticsVisualize(VisualizeMethod):
     """
     買いのシグナルを計算で求める
 
     * %K・%D共に20％以下の時に、%Kが%Dを下から上抜いた時
     * %D・スロー%D共に20％以下の時に、%Dがスロー%Dを下から上抜いた時
```

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/services/method/volatility.py` & `kabutobashi-0.7.1/kabutobashi/domain/services/method/volatility.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-from dataclasses import dataclass
-
 import pandas as pd
 
 from .method import Method, MethodType, ProcessMethod, VisualizeMethod
 
 
-@dataclass(frozen=True)
 class VolatilityProcess(ProcessMethod):
     """
     変動幅を計算する
     """
 
     method_name: str = "volatility"
     method_type: MethodType = MethodType.PARAMETERIZE
@@ -32,15 +29,14 @@
         df = df_x.copy()
         df["volatility"] = (df["high"] - df["low"]) / df["close"]
         volatility_ = df["volatility"].mean()
         close_volatility = max(df["close"]) - min(df["close"]) / df["close"].median()
         return {"volatility": volatility_, "close_volatility": close_volatility}
 
 
-@dataclass(frozen=True)
 class VolatilityVisualize(VisualizeMethod):
     def _color_mapping(self) -> list:
         return []
 
     def _visualize_option(self) -> dict:
         return {"position": "-"}
```

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/values/decoded_html_pages.py` & `kabutobashi-0.7.1/kabutobashi/domain/values/decoded_html_pages.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/values/raw_html_pages.py` & `kabutobashi-0.7.1/kabutobashi/domain/values/raw_html_pages.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/values/stock_data.py` & `kabutobashi-0.7.1/kabutobashi/domain/values/stock_data.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/domain/values/user_agent.py` & `kabutobashi-0.7.1/kabutobashi/domain/values/user_agent.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/example_data.py` & `kabutobashi-0.7.1/kabutobashi/example_data.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/infrastructure/repository/html_page_repository.py` & `kabutobashi-0.7.1/kabutobashi/infrastructure/repository/html_page_repository.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi/utilities.py` & `kabutobashi-0.7.1/kabutobashi/utilities.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/kabutobashi.egg-info/PKG-INFO` & `kabutobashi-0.7.1/kabutobashi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kabutobashi
-Version: 0.7.0
+Version: 0.7.1
 Summary: Analyze stock
 Home-page: https://github.com/gsy0911/kabutobashi
 Author: gsy0911
 Author-email: yoshiki0911@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `kabutobashi-0.7.0/kabutobashi.egg-info/SOURCES.txt` & `kabutobashi-0.7.1/kabutobashi.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -55,9 +55,10 @@
 test/__init__.py
 test/conftest.py
 test/test_page.py
 test/test_utilities.py
 test/test_application/__init__.py
 test/test_application/test_crawl.py
 test/test_domain/__init__.py
+test/test_domain/test_analysis.py
 test/test_domain/test_entities.py
 test/test_domain/test_methods.py
```

### Comparing `kabutobashi-0.7.0/pyproject.toml` & `kabutobashi-0.7.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kabutobashi"
-version = "0.7.0"
+version = "0.7.1"
 description = ""
 authors = ["yoshiki <yoshiki0911@gmail.com>"]
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 pandas = "^2.0.3"
 requests = "^2.31.0"
```

### Comparing `kabutobashi-0.7.0/setup.py` & `kabutobashi-0.7.1/setup.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/test/conftest.py` & `kabutobashi-0.7.1/test/conftest.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/test/test_application/test_crawl.py` & `kabutobashi-0.7.1/test/test_application/test_crawl.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/test/test_domain/test_entities.py` & `kabutobashi-0.7.1/test/test_domain/test_entities.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/test/test_domain/test_methods.py` & `kabutobashi-0.7.1/test/test_domain/test_methods.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/test/test_page.py` & `kabutobashi-0.7.1/test/test_page.py`

 * *Files identical despite different names*

### Comparing `kabutobashi-0.7.0/test/test_utilities.py` & `kabutobashi-0.7.1/test/test_utilities.py`

 * *Files identical despite different names*

