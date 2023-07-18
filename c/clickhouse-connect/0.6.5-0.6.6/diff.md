# Comparing `tmp/clickhouse-connect-0.6.5.tar.gz` & `tmp/clickhouse-connect-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clickhouse-connect-0.6.5.tar", last modified: Thu Jul  6 12:26:25 2023, max compression
+gzip compressed data, was "clickhouse-connect-0.6.6.tar", last modified: Fri Jul  7 11:57:19 2023, max compression
```

## Comparing `clickhouse-connect-0.6.5.tar` & `clickhouse-connect-0.6.6.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.827916 clickhouse-connect-0.6.5/clickhouse_connect/
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.827916 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.827916 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.827916 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/ddl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/dialect.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/inspector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.827916 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/sql/
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/common.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    11281 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/registry.py
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/special.py
--rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/string.py
--rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/datatypes/temporal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/clickhouse_connect/dbapi/
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/dbapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/dbapi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/dbapi/cursor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/clickhouse_connect/driver/
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/buffer.py
--rw-r--r--   0 runner    (1001) docker     (123)    39597 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/compression.py
--rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/dataconv.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/ddl.py
--rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/external.py
--rw-r--r--   0 runner    (1001) docker     (123)    21919 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/httpclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/httputil.py
--rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/insert.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/npconv.py
--rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/npquery.py
--rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/options.py
--rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    20571 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driver/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/clickhouse_connect/driverc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/driverc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/entry_points.py
--rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/json_impl.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/clickhouse_connect/tools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/tools/datagen.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect/tools/testing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-06 12:26:25.827916 clickhouse-connect-0.6.5/clickhouse_connect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/clickhouse_connect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-06 12:26:25.831916 clickhouse-connect-0.6.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-06 12:26:25.000000 clickhouse-connect-0.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.772791 clickhouse-connect-0.6.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-07 11:57:19.772791 clickhouse-connect-0.6.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1521 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.764790 clickhouse-connect-0.6.6/clickhouse_connect/
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4798 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/datatypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13547 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/ddl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/ddl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/ddl/custom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7649 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/dialect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/inspector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/sql/
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/sql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/sql/preparer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2655 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/common.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14783 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11364 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2568 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4686 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11285 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2358 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/registry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/special.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4459 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8422 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/datatypes/temporal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/dbapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/dbapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/dbapi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/dbapi/cursor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/buffer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39597 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1756 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/compression.py
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2769 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/dataconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/ddl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5286 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/external.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21919 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/httpclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8153 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/httputil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8780 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/insert.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/npconv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4240 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/npquery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5720 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20571 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      885 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driver/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect/driverc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/driverc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/entry_points.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1306 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/json_impl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.772791 clickhouse-connect-0.6.6/clickhouse_connect/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/tools/datagen.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect/tools/testing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-07 11:57:19.768791 clickhouse-connect-0.6.6/clickhouse_connect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/clickhouse_connect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-07 11:57:19.772791 clickhouse-connect-0.6.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-07-07 11:57:19.000000 clickhouse-connect-0.6.6/setup.py
```

### Comparing `clickhouse-connect-0.6.5/LICENSE` & `clickhouse-connect-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/PKG-INFO` & `clickhouse-connect-0.6.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect
-Version: 0.6.5
+Version: 0.6.6
 Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Platform: UNKNOWN
```

### Comparing `clickhouse-connect-0.6.5/README.md` & `clickhouse-connect-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/datatypes/base.py` & `clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py` & `clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/datatypes/sqltypes.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/ddl/custom.py` & `clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/ddl/custom.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py` & `clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/ddl/tableengine.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/dialect.py` & `clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/dialect.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/inspector.py` & `clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/inspector.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py` & `clickhouse-connect-0.6.6/clickhouse_connect/cc_sqlalchemy/sql/ddlcompiler.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/common.py` & `clickhouse-connect-0.6.6/clickhouse_connect/common.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/base.py` & `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/base.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/container.py` & `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/container.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/format.py` & `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/format.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/network.py` & `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/network.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/numeric.py` & `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/numeric.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,15 +216,15 @@
         if self.read_format(ctx) == 'int':
             return column
         lookup = self._int_map.get
         return [lookup(x, None) for x in column]
 
     def _write_column_binary(self, column: Union[Sequence, MutableSequence], dest: bytearray, _ctx):
         first = self._first_value(column)
-        if first is None or isinstance(first, int):
+        if first is None or not isinstance(first, str):
             if self.nullable:
                 column = [0 if not x else x for x in column]
             write_array(self._array_type, column, dest)
         else:
             lookup = self._name_map.get
             write_array(self._array_type, [lookup(x, 0) for x in column], dest)
```

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/registry.py` & `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/registry.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/special.py` & `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/special.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/string.py` & `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/string.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/datatypes/temporal.py` & `clickhouse-connect-0.6.6/clickhouse_connect/datatypes/temporal.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/dbapi/__init__.py` & `clickhouse-connect-0.6.6/clickhouse_connect/dbapi/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/dbapi/connection.py` & `clickhouse-connect-0.6.6/clickhouse_connect/dbapi/connection.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/dbapi/cursor.py` & `clickhouse-connect-0.6.6/clickhouse_connect/dbapi/cursor.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/__init__.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/__init__.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/buffer.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/buffer.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/client.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/client.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/common.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/common.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/compression.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/compression.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/context.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/context.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/ctypes.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/ctypes.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/dataconv.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/dataconv.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/ddl.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/ddl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/exceptions.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/exceptions.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/external.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/external.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/httpclient.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/httpclient.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/httputil.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/httputil.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/insert.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/insert.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/models.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/models.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/npquery.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/npquery.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/options.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/options.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/parser.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/parser.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/query.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/query.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/summary.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/summary.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/tools.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/tools.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/transform.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/transform.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/driver/types.py` & `clickhouse-connect-0.6.6/clickhouse_connect/driver/types.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/entry_points.py` & `clickhouse-connect-0.6.6/clickhouse_connect/entry_points.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/json_impl.py` & `clickhouse-connect-0.6.6/clickhouse_connect/json_impl.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/tools/datagen.py` & `clickhouse-connect-0.6.6/clickhouse_connect/tools/datagen.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect/tools/testing.py` & `clickhouse-connect-0.6.6/clickhouse_connect/tools/testing.py`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect.egg-info/PKG-INFO` & `clickhouse-connect-0.6.6/clickhouse_connect.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clickhouse-connect
-Version: 0.6.5
+Version: 0.6.6
 Summary: ClickHouse Database Core Driver for Python, Pandas, and Superset
 Home-page: https://github.com/ClickHouse/clickhouse-connect
 Author: ClickHouse Inc.
 Author-email: clients@clickhouse.com
 License: Apache License 2.0
 Keywords: clickhouse,superset,sqlalchemy,http,driver
 Platform: UNKNOWN
```

### Comparing `clickhouse-connect-0.6.5/clickhouse_connect.egg-info/SOURCES.txt` & `clickhouse-connect-0.6.6/clickhouse_connect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `clickhouse-connect-0.6.5/setup.py` & `clickhouse-connect-0.6.6/setup.py`

 * *Files identical despite different names*

