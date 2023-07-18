# Comparing `tmp/Supplier API tester-2.0.5.tar.gz` & `tmp/Supplier API tester-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/supplier-api/supplier-api/supplier_api_tester/dist/.tmp-oo828n0f/Supplier API tester-2.0.5.tar", last modified: Fri Jul 14 09:28:20 2023, max compression
+gzip compressed data, was "/home/runner/work/supplier-api/supplier-api/supplier_api_tester/dist/.tmp-mpzbblgv/Supplier API tester-2.0.6.tar", last modified: Tue Jul 18 07:56:34 2023, max compression
```

## Comparing `Supplier API tester-2.0.5.tar` & `Supplier API tester-2.0.6.tar`

### file list

```diff
@@ -1,66 +1,66 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/Supplier_API_tester.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/Supplier_API_tester.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/Supplier_API_tester.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/Supplier_API_tester.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/Supplier_API_tester.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/Supplier_API_tester.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/Supplier_API_tester.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/supplier_api_tester/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/tests/availability_timeslots.py
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/tests/availability_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/tests/booking.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/tests/product_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/tests/reservation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/utils/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/utils/availability.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/utils/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/utils/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v1/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/printer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/tester.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/tests/availability_variants.py
--rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/tests/booking.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/tests/product_catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/tests/reservation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:20.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7878 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/utils/adapters.py
--rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/utils/availability.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/utils/catalog.py
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/utils/conversions.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/utils/date.py
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/utils/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/v2/utils/reservation.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 09:28:06.000000 Supplier API tester-2.0.5/supplier_api_tester/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7071 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/Supplier_API_tester.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7563 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/Supplier_API_tester.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2104 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/Supplier_API_tester.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/Supplier_API_tester.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/Supplier_API_tester.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/Supplier_API_tester.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/Supplier_API_tester.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/supplier_api_tester/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2545 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2415 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4099 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5892 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/tests/availability_timeslots.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/tests/availability_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10679 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/tests/booking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/tests/product_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9280 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/tests/reservation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7983 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/utils/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12061 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/utils/availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/utils/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1035 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/utils/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v1/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/printer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/tester.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1423 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4741 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/tests/availability_variants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10477 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/tests/booking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/tests/product_catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/tests/reservation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:34.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/utils/adapters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11085 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/utils/availability.py
+-rw-r--r--   0 runner    (1001) docker     (123)      781 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/utils/catalog.py
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/utils/conversions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/utils/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/utils/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/v2/utils/reservation.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 07:56:22.000000 Supplier API tester-2.0.6/supplier_api_tester/version.py
```

### Comparing `Supplier API tester-2.0.5/PKG-INFO` & `Supplier API tester-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Supplier API tester
-Version: 2.0.5
+Version: 2.0.6
 Summary: Console tool for validating the Supplier API implementation
 Author: Tiqets Team
 Author-email: connections@tiqets.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Supplier API tester-2.0.5/README.md` & `Supplier API tester-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/Supplier_API_tester.egg-info/PKG-INFO` & `Supplier API tester-2.0.6/Supplier_API_tester.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Supplier-API-tester
-Version: 2.0.5
+Version: 2.0.6
 Summary: Console tool for validating the Supplier API implementation
 Author: Tiqets Team
 Author-email: connections@tiqets.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `Supplier API tester-2.0.5/Supplier_API_tester.egg-info/SOURCES.txt` & `Supplier API tester-2.0.6/Supplier_API_tester.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/setup.py` & `Supplier API tester-2.0.6/setup.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/cli.py` & `Supplier API tester-2.0.6/supplier_api_tester/cli.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/cli.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/cli.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/client.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/client.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/decorators.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/decorators.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/models.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/models.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/printer.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/printer.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/tester.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/tester.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/tests/__init__.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/tests/availability_timeslots.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/tests/availability_timeslots.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/tests/availability_variants.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/tests/availability_variants.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/tests/booking.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/tests/booking.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/tests/product_catalog.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/tests/product_catalog.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/tests/reservation.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/tests/reservation.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/utils/adapters.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/utils/adapters.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/utils/availability.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/utils/availability.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/utils/errors.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v1/utils/reservation.py` & `Supplier API tester-2.0.6/supplier_api_tester/v1/utils/reservation.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/cli.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/cli.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/client.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/client.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/decorators.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/decorators.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/models.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/models.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/printer.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/printer.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/tester.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/tester.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/tests/__init__.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/tests/availability_variants.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/tests/availability_variants.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/tests/booking.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/tests/booking.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/tests/product_catalog.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/tests/product_catalog.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/tests/reservation.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/tests/reservation.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/utils/adapters.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/utils/adapters.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,14 +196,20 @@
         )
     return booking
 
 
 def get_api_error(raw_response: Response, response) -> ApiError:
     """Unpacking 400 error JSON structure"""
     if raw_response.ok:
+        if type(response) is not dict:
+            raise FailedTest(
+                message='400 error response should be a JSON Object',
+                response=raw_response,
+            )
+
         raise FailedTest(
             message=f'Expected HTTP 400 but got HTTP {response.get("status_code")} instead.',
             response=raw_response,
         )
     if type(response) is not dict:
         raise FailedTest(
             message='400 error response should be a JSON Object',
```

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/utils/availability.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/utils/availability.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/utils/catalog.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/utils/catalog.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/utils/errors.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/utils/errors.py`

 * *Files identical despite different names*

### Comparing `Supplier API tester-2.0.5/supplier_api_tester/v2/utils/reservation.py` & `Supplier API tester-2.0.6/supplier_api_tester/v2/utils/reservation.py`

 * *Files identical despite different names*

