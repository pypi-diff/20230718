# Comparing `tmp/omni-pro-0.0.0.tar.gz` & `tmp/omni-pro-0.1.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omni-pro-0.0.0.tar", last modified: Tue Jul 18 17:05:51 2023, max compression
+gzip compressed data, was "omni-pro-0.1.10.tar", last modified: Tue Jul 18 21:06:01 2023, max compression
```

## Comparing `omni-pro-0.0.0.tar` & `omni-pro-0.1.10.tar`

### file list

```diff
@@ -1,307 +1,307 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.153094 omni-pro-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-18 17:05:39.000000 omni-pro-0.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-18 17:05:51.153094 omni-pro-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-18 17:05:39.000000 omni-pro-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.121094 omni-pro-0.0.0/omni/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.125094 omni-pro-0.0.0/omni/pro/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/aws.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/cloudmap.py
--rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.125094 omni-pro-0.0.0/omni/pro/data/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/data/models.user.csv
--rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/database.py
--rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/initial.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.125094 omni-pro-0.0.0/omni/pro/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.125094 omni-pro-0.0.0/omni/pro/models/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/common/ms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.125094 omni-pro-0.0.0/omni/pro/models/sql/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.125094 omni-pro-0.0.0/omni/pro/models/sql/catalog/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/catalog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/catalog/category.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.125094 omni-pro-0.0.0/omni/pro/models/sql/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/common/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.125094 omni-pro-0.0.0/omni/pro/models/sql/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/rules/calendar.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_category.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_category_category.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_locality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_method_ref.py
--rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_method_warehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/rules/schedule_work.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/rules/schedule_work_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/rules/warehouse_hierarchy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.125094 omni-pro-0.0.0/omni/pro/models/sql/stock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/stock/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.125094 omni-pro-0.0.0/omni/pro/models/sql/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/utilities/country.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/utilities/territory_matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/sql/utilities/territory_matrix_values.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.129094 omni-pro-0.0.0/omni/pro/models/stock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/stock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/stock/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/stock/carrier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/stock/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/stock/picking.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/stock/picking_type.py
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/stock/procurement_group.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/stock/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/stock/uom.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/stock/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/stock/warehouse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.129094 omni-pro-0.0.0/omni/pro/models/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/models/utilities/country.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.129094 omni-pro-0.0.0/omni/pro/protos/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.129094 omni-pro-0.0.0/omni/pro/protos/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/common/base_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/common/base_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/common/base_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/common/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/common/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/grpc_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/response.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.129094 omni-pro-0.0.0/omni/pro/protos/v1/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.129094 omni-pro-0.0.0/omni/pro/protos/v1/catalogs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/catalogs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/catalogs/family_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/catalogs/family_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    29775 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/catalogs/family_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11381 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/catalogs/template_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/catalogs/template_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/catalogs/template_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.133094 omni-pro-0.0.0/omni/pro/protos/v1/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/clients/address_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/clients/address_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/clients/address_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/clients/client_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/clients/client_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/clients/client_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.141094 omni-pro-0.0.0/omni/pro/protos/v1/rules/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/calendar_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/calendar_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/calendar_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/category_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/category_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/category_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_category_category_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_category_category_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_category_category_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_category_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_category_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_locality_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_schedule_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_shipper_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/location_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/location_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/location_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.145094 omni-pro-0.0.0/omni/pro/protos/v1/sales/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/address_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/address_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/address_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/carrier_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/carrier_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/carrier_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/channel_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/channel_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/channel_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/client_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/client_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/client_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/country_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/currency_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/currency_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/currency_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/delivery_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/delivery_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/order_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/order_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/order_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/order_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/order_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/order_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/payment_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/payment_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/picking_order_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/picking_order_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/picking_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/picking_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/picking_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/product_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/product_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/product_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/sale_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/sale_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/sale_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/tax_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/tax_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/tax_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/uom_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/uom_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/uom_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/user_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/warehouse_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/warehouse_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.149094 omni-pro-0.0.0/omni/pro/protos/v1/stock/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/stock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22478 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/stock/picking_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    31851 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/stock/picking_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    36632 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/stock/picking_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_move_line_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_move_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_move_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    34277 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    53054 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    56000 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.149094 omni-pro-0.0.0/omni/pro/protos/v1/users/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19903 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/users/user_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    27451 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/users/user_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    33602 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/users/user_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.153094 omni-pro-0.0.0/omni/pro/protos/v1/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/country_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/country_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/country_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/currency_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/currency_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/currency_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/document_type_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/document_type_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/language_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/language_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/language_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/model_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/model_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/model_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/payment_method_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/payment_method_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/tax_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/tax_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/tax_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/territory_matrix_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/timezone_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/timezone_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/redis.py
--rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/stack.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.153094 omni-pro-0.0.0/omni/pro/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/user/access.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-18 17:05:39.000000 omni-pro-0.0.0/omni/pro/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 17:05:51.153094 omni-pro-0.0.0/omni_pro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-07-18 17:05:51.000000 omni-pro-0.0.0/omni_pro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-07-18 17:05:51.000000 omni-pro-0.0.0/omni_pro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 17:05:51.000000 omni-pro-0.0.0/omni_pro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-18 17:05:51.000000 omni-pro-0.0.0/omni_pro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 17:05:51.000000 omni-pro-0.0.0/omni_pro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 17:05:51.153094 omni-pro-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1482 2023-07-18 17:05:39.000000 omni-pro-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.248546 omni-pro-0.1.10/
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-18 21:05:35.000000 omni-pro-0.1.10/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-18 21:06:01.248546 omni-pro-0.1.10/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2523 2023-07-18 21:05:35.000000 omni-pro-0.1.10/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.212546 omni-pro-0.1.10/omni/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.212546 omni-pro-0.1.10/omni/pro/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/cloudmap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1027 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.216546 omni-pro-0.1.10/omni/pro/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/data/models.user.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    21259 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)      892 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.216546 omni-pro-0.1.10/omni/pro/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6258 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.216546 omni-pro-0.1.10/omni/pro/models/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/common/ms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.216546 omni-pro-0.1.10/omni/pro/models/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.216546 omni-pro-0.1.10/omni/pro/models/sql/catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/catalog/category.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.216546 omni-pro-0.1.10/omni/pro/models/sql/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/common/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.216546 omni-pro-0.1.10/omni/pro/models/sql/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/rules/calendar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_category_category.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_locality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2722 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_method_ref.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1044 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_method_warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/rules/schedule_work.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/rules/schedule_work_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/rules/warehouse_hierarchy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.216546 omni-pro-0.1.10/omni/pro/models/sql/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/stock/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.216546 omni-pro-0.1.10/omni/pro/models/sql/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/utilities/country.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/utilities/territory_matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/sql/utilities/territory_matrix_values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.220546 omni-pro-0.1.10/omni/pro/models/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/stock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/stock/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/stock/carrier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/stock/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/stock/picking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/stock/picking_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/stock/procurement_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/stock/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      563 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/stock/uom.py
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/stock/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/stock/warehouse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.220546 omni-pro-0.1.10/omni/pro/models/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/models/utilities/country.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.220546 omni-pro-0.1.10/omni/pro/protos/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.220546 omni-pro-0.1.10/omni/pro/protos/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4241 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/common/base_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6203 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/common/base_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/common/base_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4932 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/common/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/common/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/grpc_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3852 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/response.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.220546 omni-pro-0.1.10/omni/pro/protos/v1/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.220546 omni-pro-0.1.10/omni/pro/protos/v1/catalogs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/catalogs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18444 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/catalogs/family_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25046 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/catalogs/family_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    29775 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/catalogs/family_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11381 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/catalogs/template_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14622 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/catalogs/template_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    17751 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/catalogs/template_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.224546 omni-pro-0.1.10/omni/pro/protos/v1/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4753 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/clients/address_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/clients/address_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/clients/address_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5500 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/clients/client_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6860 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/clients/client_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/clients/client_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.232546 omni-pro-0.1.10/omni/pro/protos/v1/rules/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4876 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/calendar_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5243 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/calendar_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/calendar_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/category_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/category_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/category_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6066 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_category_category_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6200 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_category_category_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_category_category_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5687 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_category_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6032 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_category_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10342 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5714 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_locality_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6641 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8595 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11016 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8804 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6566 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6650 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10742 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6561 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7042 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6339 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10242 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6572 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7804 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5914 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6039 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_schedule_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6633 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9004 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6698 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6662 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10942 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6421 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10442 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6677 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_shipper_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7870 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8904 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6195 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6298 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10133 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6380 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7710 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5845 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6069 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9564 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5843 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6100 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9491 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6052 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6192 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9873 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4818 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/location_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/location_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/location_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6189 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9064 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5664 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6403 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6316 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6404 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10402 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5921 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6151 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9764 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6161 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7023 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4967 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.240546 omni-pro-0.1.10/omni/pro/protos/v1/sales/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5109 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/address_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5927 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/address_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/address_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/carrier_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5691 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/carrier_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/carrier_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4815 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/channel_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5419 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/channel_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/channel_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4785 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/client_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5458 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/client_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7944 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/client_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4854 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5503 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/currency_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5736 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/currency_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8144 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/currency_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5401 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/delivery_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5666 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/delivery_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8832 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/order_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7435 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/order_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/order_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5275 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/order_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/order_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7844 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/order_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5341 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/payment_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5961 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/payment_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8704 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/picking_order_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5871 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/picking_order_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8604 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6580 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/picking_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10533 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/picking_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/picking_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4904 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/product_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/product_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/product_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/sale_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8086 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/sale_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/sale_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/tax_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/tax_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/tax_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4562 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/uom_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/uom_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7644 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/uom_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4589 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5372 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/user_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4977 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/warehouse_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5678 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/warehouse_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8244 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.240546 omni-pro-0.1.10/omni/pro/protos/v1/stock/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/stock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22478 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/stock/picking_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31851 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/stock/picking_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    36632 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/stock/picking_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_move_line_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8408 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8719 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5560 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_move_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7224 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_move_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8304 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34277 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53054 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    56000 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.244547 omni-pro-0.1.10/omni/pro/protos/v1/users/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19903 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/users/user_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27451 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/users/user_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    33602 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/users/user_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.244547 omni-pro-0.1.10/omni/pro/protos/v1/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/country_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10030 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/country_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8184 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/country_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5805 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/currency_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7711 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/currency_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/currency_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5675 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/document_type_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6397 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/document_type_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8705 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/language_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7939 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/language_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/language_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4959 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/model_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5648 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/model_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7997 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/model_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5532 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/payment_method_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6095 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/payment_method_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8805 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5043 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/tax_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/tax_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7745 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/tax_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5755 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/territory_matrix_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6464 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6220 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6551 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     9574 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5293 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/timezone_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6181 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/timezone_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/redis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3243 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/stack.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.248546 omni-pro-0.1.10/omni/pro/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/user/access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-07-18 21:05:35.000000 omni-pro-0.1.10/omni/pro/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 21:06:01.248546 omni-pro-0.1.10/omni_pro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3073 2023-07-18 21:06:01.000000 omni-pro-0.1.10/omni_pro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12559 2023-07-18 21:06:01.000000 omni-pro-0.1.10/omni_pro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 21:06:01.000000 omni-pro-0.1.10/omni_pro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-07-18 21:06:01.000000 omni-pro-0.1.10/omni_pro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 21:06:01.000000 omni-pro-0.1.10/omni_pro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 21:06:01.248546 omni-pro-0.1.10/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-07-18 21:05:53.000000 omni-pro-0.1.10/setup.py
```

### Comparing `omni-pro-0.0.0/LICENSE` & `omni-pro-0.1.10/LICENSE`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/PKG-INFO` & `omni-pro-0.1.10/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omni-pro
-Version: 0.0.0
+Version: 0.1.10
 Summary: Python library designed to be a utility for OMS microservices
 Home-page: https://github.com/Omnipro-Solutions/saas-ms-library
 Author: OMNI.PRO
 Author-email: development@omni.pro
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `omni-pro-0.0.0/README.md` & `omni-pro-0.1.10/README.md`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/aws.py` & `omni-pro-0.1.10/omni/pro/aws.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/cloudmap.py` & `omni-pro-0.1.10/omni/pro/cloudmap.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/config.py` & `omni-pro-0.1.10/omni/pro/config.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/database.py` & `omni-pro-0.1.10/omni/pro/database.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/decorators.py` & `omni-pro-0.1.10/omni/pro/decorators.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/initial.py` & `omni-pro-0.1.10/omni/pro/initial.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/logger.py` & `omni-pro-0.1.10/omni/pro/logger.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/base.py` & `omni-pro-0.1.10/omni/pro/models/base.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/sql/common/country.py` & `omni-pro-0.1.10/omni/pro/models/sql/common/country.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_category.py` & `omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_category.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_category_category.py` & `omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_category_category.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_locality.py` & `omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_locality.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py` & `omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_locality_territory_matrix_values.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_method.py` & `omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_method.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_method_ref.py` & `omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_method_ref.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_method_warehouse.py` & `omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_method_warehouse.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/sql/rules/delivery_schedule.py` & `omni-pro-0.1.10/omni/pro/models/sql/rules/delivery_schedule.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py` & `omni-pro-0.1.10/omni/pro/models/sql/rules/schedule_warehouse_hierarchy.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/sql/rules/schedule_work.py` & `omni-pro-0.1.10/omni/pro/models/sql/rules/schedule_work.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/sql/rules/schedule_work_line.py` & `omni-pro-0.1.10/omni/pro/models/sql/rules/schedule_work_line.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py` & `omni-pro-0.1.10/omni/pro/models/sql/rules/schedule_work_schedule_work_line.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/sql/rules/warehouse_hierarchy.py` & `omni-pro-0.1.10/omni/pro/models/sql/rules/warehouse_hierarchy.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/stock/attachment.py` & `omni-pro-0.1.10/omni/pro/models/stock/attachment.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/stock/location.py` & `omni-pro-0.1.10/omni/pro/models/stock/location.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/stock/picking.py` & `omni-pro-0.1.10/omni/pro/models/stock/picking.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/stock/picking_type.py` & `omni-pro-0.1.10/omni/pro/models/stock/picking_type.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/stock/procurement_group.py` & `omni-pro-0.1.10/omni/pro/models/stock/procurement_group.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/stock/product.py` & `omni-pro-0.1.10/omni/pro/models/stock/product.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/stock/uom.py` & `omni-pro-0.1.10/omni/pro/models/stock/uom.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/stock/user.py` & `omni-pro-0.1.10/omni/pro/models/stock/user.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/stock/warehouse.py` & `omni-pro-0.1.10/omni/pro/models/stock/warehouse.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/models/utilities/country.py` & `omni-pro-0.1.10/omni/pro/models/utilities/country.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/common/base_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/common/base_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/common/base_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/common/base_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/common/country_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/common/country_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/common/country_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/common/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/grpc_connector.py` & `omni-pro-0.1.10/omni/pro/protos/grpc_connector.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/response.py` & `omni-pro-0.1.10/omni/pro/protos/response.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/util.py` & `omni-pro-0.1.10/omni/pro/protos/util.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/catalogs/family_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/catalogs/family_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/catalogs/family_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/catalogs/family_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/catalogs/family_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/catalogs/family_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/catalogs/template_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/catalogs/template_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/catalogs/template_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/catalogs/template_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/catalogs/template_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/catalogs/template_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/clients/address_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/clients/address_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/clients/address_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/clients/address_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/clients/address_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/clients/address_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/clients/client_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/clients/client_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/clients/client_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/clients/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/clients/client_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/clients/client_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/calendar_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/calendar_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/calendar_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/calendar_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/calendar_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/calendar_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/category_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/category_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/category_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/category_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/category_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/category_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_category_category_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_category_category_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_category_category_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_category_category_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_category_category_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_category_category_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_category_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_category_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_category_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_category_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_category_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_locality_matrix_values_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_locality_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_locality_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_locality_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_locality_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_warehouse_hierarchy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_method_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_price_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_schedule_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_schedule_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_schedule_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_schedule_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_schedule_warehouse_hierarchy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_shipper_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_shipper_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_shipper_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_shipper_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_shipper_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_time_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delivery_warehouse_ref_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/delviery_shipper_warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/location_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/location_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/location_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/location_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/location_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/location_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_line_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_line_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/schedule_work_schedule_work_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_hierarchy_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/rules/warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/address_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/address_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/address_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/address_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/address_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/address_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/carrier_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/carrier_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/carrier_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/carrier_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/carrier_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/carrier_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/channel_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/channel_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/channel_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/channel_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/channel_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/channel_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/client_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/client_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/client_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/client_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/client_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/client_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/country_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/country_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/country_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/country_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/country_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/currency_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/currency_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/currency_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/currency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/currency_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/currency_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/delivery_method_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/delivery_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/delivery_method_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/delivery_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/delivery_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/order_line_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/order_line_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/order_line_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/order_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/order_line_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/order_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/order_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/order_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/order_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/order_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/order_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/order_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/payment_method_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/payment_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/payment_method_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/payment_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/payment_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/picking_order_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/picking_order_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/picking_order_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/picking_order_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/picking_order_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/picking_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/picking_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/picking_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/picking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/picking_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/picking_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/product_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/product_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/product_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/product_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/product_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/product_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/sale_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/sale_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/sale_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/sale_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/sale_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/sale_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/tax_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/tax_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/tax_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/tax_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/tax_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/tax_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/uom_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/uom_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/uom_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/uom_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/uom_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/uom_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/user_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/user_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/user_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/user_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/warehouse_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/warehouse_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/warehouse_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/warehouse_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/sales/warehouse_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/stock/picking_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/stock/picking_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/stock/picking_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/stock/picking_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/stock/picking_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/stock/picking_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_move_line_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_move_line_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_move_line_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_move_line_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_move_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_move_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_move_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_move_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_move_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/stock/stock_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/stock/stock_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/users/user_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/users/user_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/users/user_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/users/user_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/users/user_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/users/user_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/country_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/country_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/country_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/country_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/country_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/country_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/currency_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/currency_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/currency_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/currency_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/currency_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/currency_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/document_type_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/document_type_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/document_type_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/document_type_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/document_type_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/language_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/language_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/language_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/language_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/language_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/language_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/model_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/model_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/model_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/model_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/model_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/model_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/payment_method_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/payment_method_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/payment_method_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/payment_method_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/payment_method_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/tax_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/tax_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/tax_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/tax_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/tax_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/tax_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/territory_matrix_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/territory_matrix_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/territory_matrix_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/territory_matrix_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/territory_matrix_value_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/territory_matrix_value_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/timezone_pb2.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/timezone_pb2.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/timezone_pb2.pyi` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/timezone_pb2.pyi`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py` & `omni-pro-0.1.10/omni/pro/protos/v1/utilities/timezone_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/stack.py` & `omni-pro-0.1.10/omni/pro/stack.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/user/access.py` & `omni-pro-0.1.10/omni/pro/user/access.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/util.py` & `omni-pro-0.1.10/omni/pro/util.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni/pro/validators.py` & `omni-pro-0.1.10/omni/pro/validators.py`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/omni_pro.egg-info/PKG-INFO` & `omni-pro-0.1.10/omni_pro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omni-pro
-Version: 0.0.0
+Version: 0.1.10
 Summary: Python library designed to be a utility for OMS microservices
 Home-page: https://github.com/Omnipro-Solutions/saas-ms-library
 Author: OMNI.PRO
 Author-email: development@omni.pro
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `omni-pro-0.0.0/omni_pro.egg-info/SOURCES.txt` & `omni-pro-0.1.10/omni_pro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `omni-pro-0.0.0/setup.py` & `omni-pro-0.1.10/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 # The directory containing this file
 HERE = Path(__file__).parent
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 DESCRIPTION = "Python library designed to be a utility for OMS microservices"
-VERSION = "0.0.0"
+VERSION = "0.1.10"
 PACKAGE_NAME = "omni-pro"
 AUTHOR = "OMNI.PRO"
 AUTHOR_EMAIL = "development@omni.pro"
 URL = "https://github.com/Omnipro-Solutions/saas-ms-library"
 
 INSTALL_REQUIRES = [
     "protobuf==4.23.4",
```

