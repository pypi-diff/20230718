# Comparing `tmp/exchange_currency-0.1.0.tar.gz` & `tmp/exchange_currency-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "exchange_currency-0.1.0.tar", max compression
+gzip compressed data, was "exchange_currency-0.2.0.tar", max compression
```

## Comparing `exchange_currency-0.1.0.tar` & `exchange_currency-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2023-07-18 10:27:18.950672 exchange_currency-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-07-18 10:27:18.950599 exchange_currency-0.1.0/exchange_currency/__init__.py
--rw-r--r--   0        0        0      448 2023-07-18 10:30:08.575993 exchange_currency-0.1.0/exchange_currency/cli.py
--rw-r--r--   0        0        0      267 2023-07-18 09:11:08.771175 exchange_currency-0.1.0/exchange_currency/config.py
--rw-r--r--   0        0        0      298 2023-07-18 10:32:08.190061 exchange_currency-0.1.0/exchange_currency/rates.py
--rw-r--r--   0        0        0      358 2023-07-18 10:33:20.676466 exchange_currency-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 exchange_currency-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-07-18 10:27:18.950672 exchange_currency-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-07-18 10:27:18.950599 exchange_currency-0.2.0/exchange_currency/__init__.py
+-rw-r--r--   0        0        0      448 2023-07-18 10:30:08.575993 exchange_currency-0.2.0/exchange_currency/cli.py
+-rw-r--r--   0        0        0      267 2023-07-18 09:11:08.771175 exchange_currency-0.2.0/exchange_currency/config.py
+-rw-r--r--   0        0        0      298 2023-07-18 10:32:08.190061 exchange_currency-0.2.0/exchange_currency/rates.py
+-rw-r--r--   0        0        0      437 2023-07-18 10:37:36.859227 exchange_currency-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      404 1970-01-01 00:00:00.000000 exchange_currency-0.2.0/PKG-INFO
```

