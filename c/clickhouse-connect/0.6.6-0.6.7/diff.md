# Comparing `tmp/clickhouse-connect-0.6.6.tar.gz` & `tmp/clickhouse-connect-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-connect-0.6.6.tar", last modified: Fri Jul  7 11:57:19 2023, max compression
+gzip compressed data, was "clickhouse-connect-0.6.7.tar", last modified: Tue Jul 18 09:50:00 2023, max compression
```

## Comparing `clickhouse-connect-0.6.6.tar` & `clickhouse-connect-0.6.7.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.772791 clickhouse-connect-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-07 11:57:19.772791 clickhouse-connect-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.764790 clickhouse-connect-0.6.6/clickhouse_connect/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/ddl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/dialect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/special.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/temporal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/dbapi/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/dbapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/dbapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/dbapi/cursor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/driver/
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    39597 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/dataconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/ddl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/external.py
--rw-r--r--   0 runner    (1001) docker     (123)    21919 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/httputil.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/npconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/npquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20571 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/driverc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driverc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/json_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.772791 clickhouse-connect-0.6.6/clickhouse_connect/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/tools/datagen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/tools/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 11:57:19.772791 clickhouse-connect-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:50:00.031917 clickhouse-connect-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-18 09:50:00.031917 clickhouse-connect-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:50:00.011916 clickhouse-connect-0.6.7/clickhouse_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:50:00.015916 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:50:00.015916 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:50:00.015916 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/ddl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:50:00.019917 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:50:00.019917 clickhouse-connect-0.6.7/clickhouse_connect/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/datatypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/datatypes/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/datatypes/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/datatypes/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/datatypes/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/datatypes/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/datatypes/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/datatypes/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/datatypes/temporal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:50:00.019917 clickhouse-connect-0.6.7/clickhouse_connect/dbapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/dbapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/dbapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/dbapi/cursor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:50:00.027917 clickhouse-connect-0.6.7/clickhouse_connect/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39597 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4090 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/dataconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/ddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21938 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/httputil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/npconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/npquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20571 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4984 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driver/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:50:00.027917 clickhouse-connect-0.6.7/clickhouse_connect/driverc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/driverc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/json_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:50:00.031917 clickhouse-connect-0.6.7/clickhouse_connect/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/tools/datagen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect/tools/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 09:50:00.015916 clickhouse-connect-0.6.7/clickhouse_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-18 09:50:00.000000 clickhouse-connect-0.6.7/clickhouse_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/clickhouse_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 09:50:00.031917 clickhouse-connect-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-07-18 09:49:59.000000 clickhouse-connect-0.6.7/setup.py
```

### Comparing `clickhouse-connect-0.6.6/LICENSE` & `clickhouse-connect-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/PKG-INFO` & `clickhouse-connect-0.6.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect
-Version: 0.6.6
+Version: 0.6.7
 Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Platform: UNKNOWN
```

### Comparing `clickhouse-connect-0.6.6/README.md` & `clickhouse-connect-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/datatypes/base.py` & `clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py` & `clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/ddl/custom.py` & `clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/ddl/custom.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py` & `clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/dialect.py` & `clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/inspector.py` & `clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/inspector.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py` & `clickhouse-connect-0.6.7/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/common.py` & `clickhouse-connect-0.6.7/clickhouse_connect/common.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/base.py` & `clickhouse-connect-0.6.7/clickhouse_connect/datatypes/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -217,68 +217,68 @@
             self._write_column_binary(column, dest, ctx)
 
     # pylint: disable=no-member
     def _read_low_card_column(self, source: ByteSource, num_rows: int, ctx: QueryContext):
         if num_rows == 0:
             return []
         key_data = source.read_uint64()
-        index_sz = 2 ** (key_data & 0xff)
-        key_cnt = source.read_uint64()
-        keys = self._read_column_binary(source, key_cnt, ctx)
+        key_sz = 2 ** (key_data & 0xff)
         index_cnt = source.read_uint64()
-        index = source.read_array(array_type(index_sz, False), index_cnt)
+        index = self._read_column_binary(source, index_cnt, ctx)
+        key_cnt = source.read_uint64()
+        keys = source.read_array(array_type(key_sz, False), key_cnt)
         if self.nullable:
-            return self._build_lc_nullable_column(keys, index, ctx)
-        return self._build_lc_column(keys, index, ctx)
+            return self._build_lc_nullable_column(index, keys, ctx)
+        return self._build_lc_column(index, keys, ctx)
 
-    def _build_lc_column(self, keys: Sequence, index: array.array, _ctx: QueryContext):
-        return [keys[ix] for ix in index]
+    def _build_lc_column(self, index: Sequence, keys: array.array, _ctx: QueryContext):
+        return [index[key] for key in keys]
 
-    def _build_lc_nullable_column(self, keys: Sequence, index: array.array, ctx: QueryContext):
-        return data_conv.build_lc_nullable_column(keys, index, self._active_null(ctx))
+    def _build_lc_nullable_column(self, index: Sequence, keys: array.array, ctx: QueryContext):
+        return data_conv.build_lc_nullable_column(index, keys, self._active_null(ctx))
 
     def _write_column_low_card(self, column: Sequence, dest: bytearray, ctx: InsertContext):
         if len(column) == 0:
             return
-        index = []
         keys = []
+        index = []
         rev_map = {}
         rmg = rev_map.get
         if self.nullable:
-            keys.append(None)
+            index.append(None)
             key = 1
             for x in column:
                 if x is None:
-                    index.append(0)
+                    keys.append(0)
                 else:
                     ix = rmg(x)
                     if ix is None:
-                        index.append(key)
-                        keys.append(x)
+                        keys.append(key)
+                        index.append(x)
                         rev_map[x] = key
                         key += 1
                     else:
-                        index.append(ix)
+                        keys.append(ix)
         else:
             key = 0
             for x in column:
                 ix = rmg(x)
                 if ix is None:
-                    index.append(key)
-                    keys.append(x)
+                    keys.append(key)
+                    index.append(x)
                     rev_map[x] = key
                     key += 1
                 else:
-                    index.append(ix)
-        ix_type = int(log(len(keys), 2)) >> 3  # power of two bytes needed to store the total number of keys
+                    keys.append(ix)
+        ix_type = int(log(len(index), 2)) >> 3  # power of two bytes needed to store the total number of keys
         write_uint64((1 << 9) | (1 << 10) | ix_type, dest)  # Index type plus new dictionary (9) and additional keys(10)
-        write_uint64(len(keys), dest)
-        self._write_column_binary(keys, dest, ctx)
         write_uint64(len(index), dest)
-        write_array(array_type(1 << ix_type, False), index, dest)
+        self._write_column_binary(index, dest, ctx)
+        write_uint64(len(keys), dest)
+        write_array(array_type(1 << ix_type, False), keys, dest)
 
     def _active_null(self, _ctx: QueryContext) -> Any:
         return None
 
     def _first_value(self, column: Sequence) -> Optional[Any]:
         if self.nullable:
             return next((x for x in column if x is not None), None)
@@ -317,18 +317,18 @@
         if ctx.use_numpy:
             return numpy_conv.read_numpy_array(source, self.np_type, num_rows)
         return source.read_array(self._array_type, num_rows)
 
     def _read_nullable_column(self, source: ByteSource, num_rows: int, ctx: QueryContext) -> Sequence:
         return data_conv.read_nullable_array(source, self._array_type, num_rows, self._active_null(ctx))
 
-    def _build_lc_column(self, keys: Sequence, index: array.array, ctx: QueryContext):
+    def _build_lc_column(self, index: Sequence, keys: array.array, ctx: QueryContext):
         if ctx.use_numpy:
-            return np.fromiter((keys[ix] for ix in index), dtype=keys.dtype, count=len(index))
-        return super()._build_lc_column(keys, index, ctx)
+            return np.fromiter((index[key] for key in keys), dtype=index.dtype, count=len(index))
+        return super()._build_lc_column(index, keys, ctx)
 
     def _finalize_column(self, column: Sequence, ctx: QueryContext) -> Sequence:
         if self.read_format(ctx) == 'string':
             return [str(x) for x in column]
         if ctx.use_extended_dtypes and self.nullable:
             return pd.array(column, dtype=self.base_type)
         if ctx.use_numpy and self.nullable and (not ctx.use_none):
```

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/container.py` & `clickhouse-connect-0.6.7/clickhouse_connect/datatypes/container.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/format.py` & `clickhouse-connect-0.6.7/clickhouse_connect/datatypes/format.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/network.py` & `clickhouse-connect-0.6.7/clickhouse_connect/datatypes/network.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/numeric.py` & `clickhouse-connect-0.6.7/clickhouse_connect/datatypes/numeric.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/registry.py` & `clickhouse-connect-0.6.7/clickhouse_connect/datatypes/registry.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/special.py` & `clickhouse-connect-0.6.7/clickhouse_connect/datatypes/special.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/string.py` & `clickhouse-connect-0.6.7/clickhouse_connect/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/temporal.py` & `clickhouse-connect-0.6.7/clickhouse_connect/datatypes/temporal.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/dbapi/__init__.py` & `clickhouse-connect-0.6.7/clickhouse_connect/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/dbapi/connection.py` & `clickhouse-connect-0.6.7/clickhouse_connect/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/dbapi/cursor.py` & `clickhouse-connect-0.6.7/clickhouse_connect/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/__init__.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,14 +96,17 @@
     settings = settings or {}
     if interface.startswith('http'):
         if generic_args:
             client_params = signature(HttpClient).parameters
             for name, value in generic_args.items():
                 if name in client_params:
                     kwargs[name] = value
+                elif name == 'compression':
+                    if 'compress' not in kwargs:
+                        kwargs['compress'] = value
                 else:
                     if name.startswith('ch_'):
                         name = name[3:]
                     settings[name] = value
         return HttpClient(interface, host, port, username, password, database, settings=settings, **kwargs)
     raise ProgrammingError(f'Unrecognized client type {interface}')
```

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/buffer.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/buffer.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/client.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/client.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/common.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/common.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/compression.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/compression.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/context.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/context.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/ctypes.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/ctypes.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/dataconv.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/dataconv.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,21 +86,21 @@
     return [null_obj if null_map[ix] else column[ix] for ix in range(num_rows)]
 
 
 def build_nullable_column(source: Sequence, null_map: bytes, null_obj: Any):
     return [source[ix] if null_map[ix] == 0 else null_obj for ix in range(len(source))]
 
 
-def build_lc_nullable_column(keys: Sequence, index: array.array, null_obj: Any):
+def build_lc_nullable_column(index: Sequence, keys: array.array, null_obj: Any):
     column = []
-    for ix in index:
-        if ix == 0:
+    for key in keys:
+        if key == 0:
             column.append(null_obj)
         else:
-            column.append(keys[ix])
+            column.append(index[key])
     return column
 
 
 def to_numpy_array(column: Sequence):
     arr = np.empty((len(column),), dtype=np.object)
     arr[:] = column
     return arr
```

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/ddl.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/ddl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/exceptions.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/external.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/external.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/httpclient.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/httpclient.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,15 +405,15 @@
                     # We should be safe to retry, as ClickHouse should not have processed anything on a connection
                     # that it killed.  We also only retry this once, as multiple disconnects are unlikely to be
                     # related to the Keep Alive settings
                     if attempts == 1:
                         logger.debug('Retrying remotely closed connection')
                         continue
                 logger.warning('Unexpected Http Driver Exception')
-                raise OperationalError(f'Error {ex} executing HTTP request {self.url}') from ex
+                raise OperationalError(f'Error {ex} executing HTTP request attempt {attempts} {self.url}') from ex
             finally:
                 if query_session:
                     self._active_session = None  # Make sure we always clear this
             if 200 <= response.status < 300:
                 return response
             if response.status in (429, 503, 504):
                 if attempts > retries:
```

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/httputil.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/httputil.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/insert.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/insert.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/models.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/models.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/npquery.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/npquery.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/options.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/options.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/parser.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/parser.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/query.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/query.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/summary.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/summary.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/tools.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/tools.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/transform.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/transform.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,17 +36,20 @@
                     type_name = source.read_leb128_str()
                     if block_num == 0:
                         names.append(name)
                         col_type = registry.get_from_name(type_name)
                         col_types.append(col_type)
                     else:
                         col_type = col_types[col_num]
-                    context.start_column(name)
-                    column = col_type.read_column(source, num_rows, context)
-                    result_block.append(column)
+                    if num_rows == 0:
+                        result_block.append(tuple())
+                    else:
+                        context.start_column(name)
+                        column = col_type.read_column(source, num_rows, context)
+                        result_block.append(column)
             except Exception as ex:
                 source.close()
                 if isinstance(ex, StreamCompleteException):
                     # We ran out of data before it was expected, this could be ClickHouse reporting an error
                     # in the response
                     message = source.last_message
                     if len(message) > 1024:
```

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/driver/types.py` & `clickhouse-connect-0.6.7/clickhouse_connect/driver/types.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/entry_points.py` & `clickhouse-connect-0.6.7/clickhouse_connect/entry_points.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/json_impl.py` & `clickhouse-connect-0.6.7/clickhouse_connect/json_impl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/tools/datagen.py` & `clickhouse-connect-0.6.7/clickhouse_connect/tools/datagen.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect/tools/testing.py` & `clickhouse-connect-0.6.7/clickhouse_connect/tools/testing.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect.egg-info/PKG-INFO` & `clickhouse-connect-0.6.7/clickhouse_connect.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect
-Version: 0.6.6
+Version: 0.6.7
 Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Platform: UNKNOWN
```

### Comparing `clickhouse-connect-0.6.6/clickhouse_connect.egg-info/SOURCES.txt` & `clickhouse-connect-0.6.7/clickhouse_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.6/setup.py` & `clickhouse-connect-0.6.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 c_modules = []
 
 try:
     from Cython.Build import cythonize
     from Cython import __version__ as cython_version
 
-    print(f'Using Cython {cython_version}to build cython modules')
+    print(f'Using Cython {cython_version} to build cython modules')
     c_modules = cythonize('clickhouse_connect/driverc/*.pyx', language_level='3str')
 except ImportError as ex:
     print('Cython Install Failed, Not Building C Extensions: ', ex)
     cythonize = None
 except Exception as ex:
     print('Cython Build Failed, Not Building C Extensions: ', ex)
     cythonize = None
```

