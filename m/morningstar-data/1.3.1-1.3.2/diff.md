# Comparing `tmp/morningstar_data-1.3.1.tar.gz` & `tmp/morningstar_data-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morningstar_data-1.3.1.tar", max compression
+gzip compressed data, was "morningstar_data-1.3.2.tar", max compression
```

## Comparing `morningstar_data-1.3.1.tar` & `morningstar_data-1.3.2.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0      558 2023-07-11 19:45:18.025249 morningstar_data-1.3.1/LICENSE
--rw-r--r--   0        0        0    11379 2023-07-11 19:45:18.029249 morningstar_data-1.3.1/README.md
--rw-r--r--   0        0        0      207 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/__init__.py
--rw-r--r--   0        0        0      599 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/_base.py
--rw-r--r--   0        0        0     3056 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/_utils.py
--rw-r--r--   0        0        0       82 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/_version.py
--rw-r--r--   0        0        0       61 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/__init__.py
--rw-r--r--   0        0        0       62 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/__init__.py
--rw-r--r--   0        0        0      556 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/_file.py
--rw-r--r--   0        0        0      762 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/_table.py
--rw-r--r--   0        0        0      996 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/csvfile.py
--rw-r--r--   0        0        0     2163 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/temptable.py
--rw-r--r--   0        0        0      552 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/_error_messages.py
--rw-r--r--   0        0        0      936 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/_exceptions.py
--rw-r--r--   0        0        0     5620 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/datalake/base.py
--rw-r--r--   0        0        0      939 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/__init__.py
--rw-r--r--   0        0        0     2433 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_api.py
--rw-r--r--   0        0        0      179 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_backend_apis/__init__.py
--rw-r--r--   0        0        0     1845 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_backend_apis/_delivery_backend.py
--rw-r--r--   0        0        0     4801 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_backend_apis/_holdings_backend.py
--rw-r--r--   0        0        0     3361 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_backend_apis/_signed_url_backend.py
--rw-r--r--   0        0        0     3762 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_base_api.py
--rw-r--r--   0        0        0     4947 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_config.py
--rw-r--r--   0        0        0     1999 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_config_key.py
--rw-r--r--   0        0        0     7434 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_core_api.py
--rw-r--r--   0        0        0      197 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_data_objects/__init__.py
--rw-r--r--   0        0        0     2298 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_data_objects/_custom_data_points_types.py
--rw-r--r--   0        0        0    26357 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_data_objects/_data_points_object.py
--rw-r--r--   0        0        0     7532 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_data_objects/_investments_object.py
--rw-r--r--   0        0        0     2572 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_data_point.py
--rw-r--r--   0        0        0     1051 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_data_type.py
--rw-r--r--   0        0        0     1593 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_decorator.py
--rw-r--r--   0        0        0    13892 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_error_messages.py
--rw-r--r--   0        0        0     3463 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_exceptions.py
--rw-r--r--   0        0        0        0 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_investment/__init__.py
--rw-r--r--   0        0        0     4288 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_investment/_asset_flow_data.py
--rw-r--r--   0        0        0     1546 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_investment/_common.py
--rw-r--r--   0        0        0     6085 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_investment/_data.py
--rw-r--r--   0        0        0     8369 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_investment/_normal_data.py
--rw-r--r--   0        0        0     5023 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_investment/_peer_group_data.py
--rw-r--r--   0        0        0      162 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_portfolio/__init__.py
--rw-r--r--   0        0        0     1272 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_common.py
--rw-r--r--   0        0        0     7859 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
--rw-r--r--   0        0        0     7913 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_portfolio_settings.py
--rw-r--r--   0        0        0      955 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_portfolio_type.py
--rw-r--r--   0        0        0    10975 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_portfolio_data_set.py
--rw-r--r--   0        0        0     3357 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/_utils.py
--rw-r--r--   0        0        0    13061 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/asset_flow.py
--rw-r--r--   0        0        0    16274 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/custom_database.py
--rw-r--r--   0        0        0     1236 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/data_type.py
--rw-r--r--   0        0        0    42528 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/holdings.py
--rw-r--r--   0        0        0    13577 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/investment.py
--rw-r--r--   0        0        0    32223 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/lookup.py
--rw-r--r--   0        0        0     6040 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/peer_group.py
--rw-r--r--   0        0        0    19389 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/performance_report.py
--rw-r--r--   0        0        0    37181 2023-07-11 19:45:18.037248 morningstar_data-1.3.1/morningstar_data/direct/portfolio.py
--rw-r--r--   0        0        0    12562 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/direct/returns.py
--rw-r--r--   0        0        0      413 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/direct/user_items/__init__.py
--rw-r--r--   0        0        0      742 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/direct/user_items/_utils.py
--rw-r--r--   0        0        0     7888 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/direct/user_items/data_set.py
--rw-r--r--   0        0        0    12981 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/direct/user_items/investment_lists.py
--rw-r--r--   0        0        0    11145 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/direct/user_items/portfolio.py
--rw-r--r--   0        0        0    10308 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/direct/user_items/search_criteria.py
--rw-r--r--   0        0        0     4752 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/lookup.py
--rw-r--r--   0        0        0      157 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/utils/__init__.py
--rw-r--r--   0        0        0     6359 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/utils/_delivery_config.py
--rw-r--r--   0        0        0     7752 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/utils/_helpers.py
--rw-r--r--   0        0        0    10435 2023-07-11 19:45:18.041248 morningstar_data-1.3.1/morningstar_data/utils/delivery.py
--rw-r--r--   0        0        0     2530 2023-07-11 19:46:06.420424 morningstar_data-1.3.1/pyproject.toml
--rw-r--r--   0        0        0    12488 1970-01-01 00:00:00.000000 morningstar_data-1.3.1/PKG-INFO
+-rw-r--r--   0        0        0      558 2023-07-18 18:11:01.506964 morningstar_data-1.3.2/LICENSE
+-rw-r--r--   0        0        0    11417 2023-07-18 18:11:01.506964 morningstar_data-1.3.2/README.md
+-rw-r--r--   0        0        0      207 2023-07-18 18:11:01.514964 morningstar_data-1.3.2/morningstar_data/__init__.py
+-rw-r--r--   0        0        0      599 2023-07-18 18:11:01.514964 morningstar_data-1.3.2/morningstar_data/_base.py
+-rw-r--r--   0        0        0     3056 2023-07-18 18:11:01.514964 morningstar_data-1.3.2/morningstar_data/_utils.py
+-rw-r--r--   0        0        0       82 2023-07-18 18:11:01.514964 morningstar_data-1.3.2/morningstar_data/_version.py
+-rw-r--r--   0        0        0       61 2023-07-18 18:11:01.514964 morningstar_data-1.3.2/morningstar_data/datalake/__init__.py
+-rw-r--r--   0        0        0       62 2023-07-18 18:11:01.514964 morningstar_data-1.3.2/morningstar_data/datalake/_data_objects/__init__.py
+-rw-r--r--   0        0        0      556 2023-07-18 18:11:01.514964 morningstar_data-1.3.2/morningstar_data/datalake/_data_objects/_file.py
+-rw-r--r--   0        0        0      762 2023-07-18 18:11:01.514964 morningstar_data-1.3.2/morningstar_data/datalake/_data_objects/_table.py
+-rw-r--r--   0        0        0      996 2023-07-18 18:11:01.514964 morningstar_data-1.3.2/morningstar_data/datalake/_data_objects/csvfile.py
+-rw-r--r--   0        0        0     2163 2023-07-18 18:11:01.514964 morningstar_data-1.3.2/morningstar_data/datalake/_data_objects/temptable.py
+-rw-r--r--   0        0        0      552 2023-07-18 18:11:01.514964 morningstar_data-1.3.2/morningstar_data/datalake/_error_messages.py
+-rw-r--r--   0        0        0      936 2023-07-18 18:11:01.514964 morningstar_data-1.3.2/morningstar_data/datalake/_exceptions.py
+-rw-r--r--   0        0        0     5620 2023-07-18 18:11:01.514964 morningstar_data-1.3.2/morningstar_data/datalake/base.py
+-rw-r--r--   0        0        0      939 2023-07-18 18:11:01.514964 morningstar_data-1.3.2/morningstar_data/direct/__init__.py
+-rw-r--r--   0        0        0     2433 2023-07-18 18:11:01.514964 morningstar_data-1.3.2/morningstar_data/direct/_api.py
+-rw-r--r--   0        0        0      179 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_backend_apis/__init__.py
+-rw-r--r--   0        0        0     1845 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_backend_apis/_delivery_backend.py
+-rw-r--r--   0        0        0     4801 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_backend_apis/_holdings_backend.py
+-rw-r--r--   0        0        0     3361 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_backend_apis/_signed_url_backend.py
+-rw-r--r--   0        0        0     3762 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_base_api.py
+-rw-r--r--   0        0        0     4947 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_config.py
+-rw-r--r--   0        0        0     1999 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_config_key.py
+-rw-r--r--   0        0        0     7434 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_core_api.py
+-rw-r--r--   0        0        0      197 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_data_objects/__init__.py
+-rw-r--r--   0        0        0     2298 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_data_objects/_custom_data_points_types.py
+-rw-r--r--   0        0        0    26357 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_data_objects/_data_points_object.py
+-rw-r--r--   0        0        0     7532 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_data_objects/_investments_object.py
+-rw-r--r--   0        0        0     2572 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_data_point.py
+-rw-r--r--   0        0        0     1051 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_data_type.py
+-rw-r--r--   0        0        0     1593 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_decorator.py
+-rw-r--r--   0        0        0    13892 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_error_messages.py
+-rw-r--r--   0        0        0     3463 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_exceptions.py
+-rw-r--r--   0        0        0        0 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_investment/__init__.py
+-rw-r--r--   0        0        0     4288 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_investment/_asset_flow_data.py
+-rw-r--r--   0        0        0     1546 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_investment/_common.py
+-rw-r--r--   0        0        0     6085 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_investment/_data.py
+-rw-r--r--   0        0        0     8369 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_investment/_normal_data.py
+-rw-r--r--   0        0        0     5023 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_investment/_peer_group_data.py
+-rw-r--r--   0        0        0      162 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_portfolio/__init__.py
+-rw-r--r--   0        0        0     1272 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_portfolio/_common.py
+-rw-r--r--   0        0        0     7859 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
+-rw-r--r--   0        0        0     7913 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_portfolio/_portfolio_settings.py
+-rw-r--r--   0        0        0      955 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_portfolio/_portfolio_type.py
+-rw-r--r--   0        0        0    10975 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_portfolio_data_set.py
+-rw-r--r--   0        0        0     3357 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/_utils.py
+-rw-r--r--   0        0        0    13061 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/asset_flow.py
+-rw-r--r--   0        0        0    16274 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/custom_database.py
+-rw-r--r--   0        0        0     1236 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/data_type.py
+-rw-r--r--   0        0        0    42539 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/holdings.py
+-rw-r--r--   0        0        0    13577 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/investment.py
+-rw-r--r--   0        0        0    32223 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/lookup.py
+-rw-r--r--   0        0        0     6040 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/peer_group.py
+-rw-r--r--   0        0        0    19389 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/performance_report.py
+-rw-r--r--   0        0        0    37181 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/portfolio.py
+-rw-r--r--   0        0        0    12562 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/returns.py
+-rw-r--r--   0        0        0      413 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/user_items/__init__.py
+-rw-r--r--   0        0        0      742 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/user_items/_utils.py
+-rw-r--r--   0        0        0     7888 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/user_items/data_set.py
+-rw-r--r--   0        0        0    12981 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/user_items/investment_lists.py
+-rw-r--r--   0        0        0    11145 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/user_items/portfolio.py
+-rw-r--r--   0        0        0    10308 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/direct/user_items/search_criteria.py
+-rw-r--r--   0        0        0     4752 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/lookup.py
+-rw-r--r--   0        0        0      157 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/utils/__init__.py
+-rw-r--r--   0        0        0     6359 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/utils/_delivery_config.py
+-rw-r--r--   0        0        0     7752 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/utils/_helpers.py
+-rw-r--r--   0        0        0    10435 2023-07-18 18:11:01.518964 morningstar_data-1.3.2/morningstar_data/utils/delivery.py
+-rw-r--r--   0        0        0     2530 2023-07-18 18:12:22.357586 morningstar_data-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0    12526 1970-01-01 00:00:00.000000 morningstar_data-1.3.2/PKG-INFO
```

### Comparing `morningstar_data-1.3.1/LICENSE` & `morningstar_data-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/README.md` & `morningstar_data-1.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -33,18 +33,19 @@
 `export MD_AUTH_TOKEN="paste copied token here"`
 
 #### Within a Python (.py) File
 
 ```
 # testing_morningstar_data.py
 import os
+import morningstar_data as md
 
 os.environ['MD_AUTH_TOKEN']="paste copied token here"
 
-import morningstar_data as md
+md.direct.get_morningstar_data_sets()
 ```
 
 ## Requirements
 
 The morningstar_data package is tested with
 
 |             | Main version (latest)
```

### Comparing `morningstar_data-1.3.1/morningstar_data/_base.py` & `morningstar_data-1.3.2/morningstar_data/_base.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/_utils.py` & `morningstar_data-1.3.2/morningstar_data/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/_file.py` & `morningstar_data-1.3.2/morningstar_data/datalake/_data_objects/_file.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/_table.py` & `morningstar_data-1.3.2/morningstar_data/datalake/_data_objects/_table.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/csvfile.py` & `morningstar_data-1.3.2/morningstar_data/datalake/_data_objects/csvfile.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/datalake/_data_objects/temptable.py` & `morningstar_data-1.3.2/morningstar_data/datalake/_data_objects/temptable.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/datalake/_error_messages.py` & `morningstar_data-1.3.2/morningstar_data/datalake/_error_messages.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/datalake/_exceptions.py` & `morningstar_data-1.3.2/morningstar_data/datalake/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/datalake/base.py` & `morningstar_data-1.3.2/morningstar_data/datalake/base.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/__init__.py` & `morningstar_data-1.3.2/morningstar_data/direct/__init__.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_api.py` & `morningstar_data-1.3.2/morningstar_data/direct/_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_backend_apis/_delivery_backend.py` & `morningstar_data-1.3.2/morningstar_data/direct/_backend_apis/_delivery_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_backend_apis/_holdings_backend.py` & `morningstar_data-1.3.2/morningstar_data/direct/_backend_apis/_holdings_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_backend_apis/_signed_url_backend.py` & `morningstar_data-1.3.2/morningstar_data/direct/_backend_apis/_signed_url_backend.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_base_api.py` & `morningstar_data-1.3.2/morningstar_data/direct/_base_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_config.py` & `morningstar_data-1.3.2/morningstar_data/direct/_config.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_config_key.py` & `morningstar_data-1.3.2/morningstar_data/direct/_config_key.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_core_api.py` & `morningstar_data-1.3.2/morningstar_data/direct/_core_api.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_data_objects/_custom_data_points_types.py` & `morningstar_data-1.3.2/morningstar_data/direct/_data_objects/_custom_data_points_types.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_data_objects/_data_points_object.py` & `morningstar_data-1.3.2/morningstar_data/direct/_data_objects/_data_points_object.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_data_objects/_investments_object.py` & `morningstar_data-1.3.2/morningstar_data/direct/_data_objects/_investments_object.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_data_point.py` & `morningstar_data-1.3.2/morningstar_data/direct/_data_point.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_data_type.py` & `morningstar_data-1.3.2/morningstar_data/direct/_data_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_decorator.py` & `morningstar_data-1.3.2/morningstar_data/direct/_decorator.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_error_messages.py` & `morningstar_data-1.3.2/morningstar_data/direct/_error_messages.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_exceptions.py` & `morningstar_data-1.3.2/morningstar_data/direct/_exceptions.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_investment/_asset_flow_data.py` & `morningstar_data-1.3.2/morningstar_data/direct/_investment/_asset_flow_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_investment/_common.py` & `morningstar_data-1.3.2/morningstar_data/direct/_investment/_common.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_investment/_data.py` & `morningstar_data-1.3.2/morningstar_data/direct/_investment/_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_investment/_normal_data.py` & `morningstar_data-1.3.2/morningstar_data/direct/_investment/_normal_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_investment/_peer_group_data.py` & `morningstar_data-1.3.2/morningstar_data/direct/_investment/_peer_group_data.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_common.py` & `morningstar_data-1.3.2/morningstar_data/direct/_portfolio/_common.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py` & `morningstar_data-1.3.2/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_portfolio_settings.py` & `morningstar_data-1.3.2/morningstar_data/direct/_portfolio/_portfolio_settings.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_portfolio/_portfolio_type.py` & `morningstar_data-1.3.2/morningstar_data/direct/_portfolio/_portfolio_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_portfolio_data_set.py` & `morningstar_data-1.3.2/morningstar_data/direct/_portfolio_data_set.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/_utils.py` & `morningstar_data-1.3.2/morningstar_data/direct/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/asset_flow.py` & `morningstar_data-1.3.2/morningstar_data/direct/asset_flow.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/custom_database.py` & `morningstar_data-1.3.2/morningstar_data/direct/custom_database.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/data_type.py` & `morningstar_data-1.3.2/morningstar_data/direct/data_type.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/holdings.py` & `morningstar_data-1.3.2/morningstar_data/direct/holdings.py`

 * *Files 0% similar despite different names*

```diff
@@ -694,15 +694,15 @@
 def get_lookthrough_holdings(portfolio_id: str) -> DataFrame:
     """
     :bdg-ref-danger:`Upcoming Feature <../upcoming_feature>`
 
     Returns look-through holdings for a user-created portfolio.
 
     Args:
-        portfolio_id (:obj:`str`): Portfolio ID. Use the `get_portfolios <./portfolio_list.html#morningstar_data.direct.user_items.get_portfolios>`_ function to discover saved portfolios.
+        portfolio_id (:obj:`str`): Portfolio ID. Use the `get_portfolios <../portfolio/portfolio_list.html#morningstar_data.direct.user_items.get_portfolios>`_ function to discover saved portfolios.
 
     Returns:
         DataFrame: A DataFrame object with holdings data. DataFrame columns include
 
         * investment_id
         * isin
         * cusip
```

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/investment.py` & `morningstar_data-1.3.2/morningstar_data/direct/investment.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/lookup.py` & `morningstar_data-1.3.2/morningstar_data/direct/lookup.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/peer_group.py` & `morningstar_data-1.3.2/morningstar_data/direct/peer_group.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/performance_report.py` & `morningstar_data-1.3.2/morningstar_data/direct/performance_report.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/portfolio.py` & `morningstar_data-1.3.2/morningstar_data/direct/portfolio.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/returns.py` & `morningstar_data-1.3.2/morningstar_data/direct/returns.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/user_items/_utils.py` & `morningstar_data-1.3.2/morningstar_data/direct/user_items/_utils.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/user_items/data_set.py` & `morningstar_data-1.3.2/morningstar_data/direct/user_items/data_set.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/user_items/investment_lists.py` & `morningstar_data-1.3.2/morningstar_data/direct/user_items/investment_lists.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/user_items/portfolio.py` & `morningstar_data-1.3.2/morningstar_data/direct/user_items/portfolio.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/direct/user_items/search_criteria.py` & `morningstar_data-1.3.2/morningstar_data/direct/user_items/search_criteria.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/lookup.py` & `morningstar_data-1.3.2/morningstar_data/lookup.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/utils/_delivery_config.py` & `morningstar_data-1.3.2/morningstar_data/utils/_delivery_config.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/utils/_helpers.py` & `morningstar_data-1.3.2/morningstar_data/utils/_helpers.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/morningstar_data/utils/delivery.py` & `morningstar_data-1.3.2/morningstar_data/utils/delivery.py`

 * *Files identical despite different names*

### Comparing `morningstar_data-1.3.1/pyproject.toml` & `morningstar_data-1.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "morningstar_data"
-version = "1.3.1"
+version = "1.3.2"
 description = "Morningstar Data"
 authors = ["Morningstar, Inc."]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://www.morningstar.com/products/md-python-package"
 documentation = "https://docs-analyticslab.morningstar.com/latest/index.html"
```

### Comparing `morningstar_data-1.3.1/PKG-INFO` & `morningstar_data-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: morningstar-data
-Version: 1.3.1
+Version: 1.3.2
 Summary: Morningstar Data
 Home-page: https://www.morningstar.com/products/md-python-package
 License: Apache-2.0
 Author: Morningstar, Inc.
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
@@ -61,18 +61,19 @@
 `export MD_AUTH_TOKEN="paste copied token here"`
 
 #### Within a Python (.py) File
 
 ```
 # testing_morningstar_data.py
 import os
+import morningstar_data as md
 
 os.environ['MD_AUTH_TOKEN']="paste copied token here"
 
-import morningstar_data as md
+md.direct.get_morningstar_data_sets()
 ```
 
 ## Requirements
 
 The morningstar_data package is tested with
 
 |             | Main version (latest)
```

