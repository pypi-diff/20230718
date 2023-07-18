# Comparing `tmp/sqlalchemy_exasol-4.5.1.tar.gz` & `tmp/sqlalchemy_exasol-4.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlalchemy_exasol-4.5.1.tar", max compression
+gzip compressed data, was "sqlalchemy_exasol-4.6.0.tar", max compression
```

## Comparing `sqlalchemy_exasol-4.5.1.tar` & `sqlalchemy_exasol-4.6.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0    15150 2023-05-25 12:18:28.298003 sqlalchemy_exasol-4.5.1/CHANGELOG.rst
--rw-r--r--   0        0        0     1395 2023-05-25 12:18:28.298003 sqlalchemy_exasol-4.5.1/LICENSE
--rw-r--r--   0        0        0    10489 2023-05-25 12:18:28.298003 sqlalchemy_exasol-4.5.1/README.rst
--rw-r--r--   0        0        0        0 2023-05-25 12:18:28.346004 sqlalchemy_exasol-4.5.1/exasol/driver/__init__.py
--rw-r--r--   0        0        0     1715 2023-05-25 12:18:28.346004 sqlalchemy_exasol-4.5.1/exasol/driver/odbc.py
--rw-r--r--   0        0        0        0 2023-05-25 12:18:28.346004 sqlalchemy_exasol-4.5.1/exasol/driver/websocket/__init__.py
--rw-r--r--   0        0        0     4477 2023-05-25 12:18:28.346004 sqlalchemy_exasol-4.5.1/exasol/driver/websocket/_connection.py
--rw-r--r--   0        0        0     8336 2023-05-25 12:18:28.346004 sqlalchemy_exasol-4.5.1/exasol/driver/websocket/_cursor.py
--rw-r--r--   0        0        0     2328 2023-05-25 12:18:28.346004 sqlalchemy_exasol-4.5.1/exasol/driver/websocket/_errors.py
--rw-r--r--   0        0        0    11135 2023-05-25 12:18:28.346004 sqlalchemy_exasol-4.5.1/exasol/driver/websocket/_protocols.py
--rw-r--r--   0        0        0     2668 2023-05-25 12:18:28.346004 sqlalchemy_exasol-4.5.1/exasol/driver/websocket/_types.py
--rw-r--r--   0        0        0     2311 2023-05-25 12:18:28.346004 sqlalchemy_exasol-4.5.1/exasol/driver/websocket/dbapi2.py
--rw-r--r--   0        0        0     3491 2023-05-25 12:18:28.350004 sqlalchemy_exasol-4.5.1/pyproject.toml
--rw-r--r--   0        0        0      413 2023-05-25 12:18:28.350004 sqlalchemy_exasol-4.5.1/sqlalchemy_exasol/__init__.py
--rw-r--r--   0        0        0    33919 2023-05-25 12:18:28.350004 sqlalchemy_exasol-4.5.1/sqlalchemy_exasol/base.py
--rw-r--r--   0        0        0      165 2023-05-25 12:18:28.350004 sqlalchemy_exasol-4.5.1/sqlalchemy_exasol/constraints.py
--rw-r--r--   0        0        0    11765 2023-05-25 12:18:28.350004 sqlalchemy_exasol-4.5.1/sqlalchemy_exasol/pyodbc.py
--rw-r--r--   0        0        0     7522 2023-05-25 12:18:28.350004 sqlalchemy_exasol-4.5.1/sqlalchemy_exasol/requirements.py
--rw-r--r--   0        0        0     4262 2023-05-25 12:18:28.350004 sqlalchemy_exasol-4.5.1/sqlalchemy_exasol/turbodbc.py
--rw-r--r--   0        0        0     1646 2023-05-25 12:18:28.350004 sqlalchemy_exasol-4.5.1/sqlalchemy_exasol/util.py
--rw-r--r--   0        0        0      235 2023-05-25 12:18:28.350004 sqlalchemy_exasol-4.5.1/sqlalchemy_exasol/version.py
--rw-r--r--   0        0        0     4689 2023-05-25 12:18:28.350004 sqlalchemy_exasol-4.5.1/sqlalchemy_exasol/websocket.py
--rw-r--r--   0        0        0    12016 1970-01-01 00:00:00.000000 sqlalchemy_exasol-4.5.1/setup.py
--rw-r--r--   0        0        0    12487 1970-01-01 00:00:00.000000 sqlalchemy_exasol-4.5.1/PKG-INFO
+-rw-r--r--   0        0        0    15726 2023-07-18 09:10:53.414712 sqlalchemy_exasol-4.6.0/CHANGELOG.rst
+-rw-r--r--   0        0        0     1395 2023-07-18 09:10:53.414712 sqlalchemy_exasol-4.6.0/LICENSE
+-rw-r--r--   0        0        0     7523 2023-07-18 09:10:53.414712 sqlalchemy_exasol-4.6.0/README.rst
+-rw-r--r--   0        0        0        0 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/exasol/driver/__init__.py
+-rw-r--r--   0        0        0     1715 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/exasol/driver/odbc.py
+-rw-r--r--   0        0        0        0 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/exasol/driver/websocket/__init__.py
+-rw-r--r--   0        0        0     4477 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/exasol/driver/websocket/_connection.py
+-rw-r--r--   0        0        0    10207 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/exasol/driver/websocket/_cursor.py
+-rw-r--r--   0        0        0     2328 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/exasol/driver/websocket/_errors.py
+-rw-r--r--   0        0        0    11135 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/exasol/driver/websocket/_protocols.py
+-rw-r--r--   0        0        0     2668 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/exasol/driver/websocket/_types.py
+-rw-r--r--   0        0        0     2311 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/exasol/driver/websocket/dbapi2.py
+-rw-r--r--   0        0        0     3491 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/pyproject.toml
+-rw-r--r--   0        0        0      413 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/sqlalchemy_exasol/__init__.py
+-rw-r--r--   0        0        0    33919 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/sqlalchemy_exasol/base.py
+-rw-r--r--   0        0        0      165 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/sqlalchemy_exasol/constraints.py
+-rw-r--r--   0        0        0    11765 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/sqlalchemy_exasol/pyodbc.py
+-rw-r--r--   0        0        0     7522 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/sqlalchemy_exasol/requirements.py
+-rw-r--r--   0        0        0     4262 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/sqlalchemy_exasol/turbodbc.py
+-rw-r--r--   0        0        0     1646 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/sqlalchemy_exasol/util.py
+-rw-r--r--   0        0        0      235 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/sqlalchemy_exasol/version.py
+-rw-r--r--   0        0        0     4738 2023-07-18 09:10:53.466714 sqlalchemy_exasol-4.6.0/sqlalchemy_exasol/websocket.py
+-rw-r--r--   0        0        0     9025 1970-01-01 00:00:00.000000 sqlalchemy_exasol-4.6.0/setup.py
+-rw-r--r--   0        0        0     9521 1970-01-01 00:00:00.000000 sqlalchemy_exasol-4.6.0/PKG-INFO
```

### Comparing `sqlalchemy_exasol-4.5.1/CHANGELOG.rst` & `sqlalchemy_exasol-4.6.0/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,30 @@
 .. _changelog-unreleased:
 
 Unreleased
 ==========
 
+.. _changelog-4.6.0:
+
+4.6.0 — 2023-07-18
+==================
+
+🚀 Feature
+-----------
+
+- Websocket based dialect have been stabilized and is officially supported now
+
+    📘 Note: Inserting multiple empty row's, facilitating default settings currently isn't supported.
+
+🐞 Fixed
+---------
+
+- Fixed `prepared statements send the wrong types as parameters to the server <https://github.com/exasol/sqlalchemy-exasol/issues/341>`_
+- Fixed `Various SQLA compliance tests are failing for the websocket based dialect <https://github.com/exasol/sqlalchemy-exasol/issues/342>`_
+
 .. _changelog-4.5.1:
 
 4.5.1 — 2023-05-25
 ==================
 
 🐞 Fixed
 ---------
```

### Comparing `sqlalchemy_exasol-4.5.1/LICENSE` & `sqlalchemy_exasol-4.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.5.1/README.rst` & `sqlalchemy_exasol-4.6.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,233 +1,46 @@
-SQLAlchemy Dialect for EXASOL DB
-================================
+# -*- coding: utf-8 -*-
+from setuptools import setup
 
+packages = \
+['exasol', 'exasol.driver', 'exasol.driver.websocket', 'sqlalchemy_exasol']
 
-.. image:: https://github.com/exasol/sqlalchemy_exasol/workflows/CI/badge.svg?branch=master
-    :target: https://github.com/exasol/sqlalchemy_exasol/actions?query=workflow%3ACI
-     :alt: CI Status
+package_data = \
+{'': ['*']}
 
-.. image:: https://img.shields.io/pypi/v/sqlalchemy_exasol
-     :target: https://pypi.org/project/sqlalchemy-exasol/
-     :alt: PyPI Version
+install_requires = \
+['packaging>=21.3',
+ 'pyexasol>=0.25.1,<0.26.0',
+ 'pyodbc>=4.0.34,<5.0.0',
+ 'sqlalchemy>=1.4,<1.4.45']
+
+extras_require = \
+{'turbodbc': ['turbodbc==4.5.4']}
+
+entry_points = \
+{'sqlalchemy.dialects': ['exa.pyodbc = '
+                         'sqlalchemy_exasol.pyodbc:EXADialect_pyodbc',
+                         'exa.turbodbc = '
+                         'sqlalchemy_exasol.turbodbc:EXADialect_turbodbc',
+                         'exa.websocket = '
+                         'sqlalchemy_exasol.websocket:EXADialect_websocket']}
+
+setup_kwargs = {
+    'name': 'sqlalchemy-exasol',
+    'version': '4.6.0',
+    'description': 'EXASOL dialect for SQLAlchemy',
+    'long_description': 'SQLAlchemy Dialect for EXASOL DB\n================================\n\n\n.. image:: https://github.com/exasol/sqlalchemy-exasol/actions/workflows/ci-cd.yml/badge.svg?branch=master&event=push\n    :target: https://github.com/exasol/sqlalchemy-exasol/actions/workflows/ci-cd.yml\n     :alt: CI Status\n\n.. image:: https://img.shields.io/pypi/v/sqlalchemy_exasol\n     :target: https://pypi.org/project/sqlalchemy-exasol/\n     :alt: PyPI Version\n\n.. image:: https://img.shields.io/pypi/pyversions/sqlalchemy-exasol\n    :target: https://pypi.org/project/sqlalchemy-exasol\n    :alt: PyPI - Python Version\n\n.. image:: https://img.shields.io/badge/exasol-7.1.9%20%7C%207.0.18-green\n    :target: https://www.exasol.com/\n    :alt: Exasol - Supported Version(s)\n\n.. image:: https://img.shields.io/badge/code%20style-black-000000.svg\n    :target: https://github.com/psf/black\n    :alt: Formatter - Black\n\n.. image:: https://img.shields.io/badge/imports-isort-ef8336.svg\n    :target: https://pycqa.github.io/isort/\n    :alt: Formatter - Isort\n\n.. image:: https://img.shields.io/badge/pylint-6.4-yellowgreen\n    :target: https://github.com/PyCQA/pylint\n    :alt: Pylint\n\n.. image:: https://img.shields.io/pypi/l/sqlalchemy-exasol\n     :target: https://opensource.org/licenses/BSD-2-Clause\n     :alt: License\n\n.. image:: https://img.shields.io/github/last-commit/exasol/sqlalchemy-exasol\n     :target: https://pypi.org/project/sqlalchemy-exasol/\n     :alt: Last Commit\n\n.. image:: https://img.shields.io/pypi/dm/sqlalchemy-exasol\n    :target: https://pypi.org/project/sqlalchemy-exasol\n    :alt: PyPI - Downloads\n\n\nHow to get started\n------------------\n\nCurrently, sqlalchemy-exasol supports multiple dialects. The core difference\nbeing if the dialect is :code:`odbc` or :code:`websocket` based.\n\nGenerally, we advise to use the websocket based Dialect, because odbc\nbased dialects require a good understanding of (unix)ODBC and the setup is\nsignificant more complicated.\n\n\nTurbodbc support\n````````````````\n\n.. warning::\n\n    Maintenance of this feature is on hold. Also it is very likely that turbodbc support will be dropped in future versions.\n\n- You can use Turbodbc with sqlalchemy_exasol if you use a python version >= 3.8.\n- Multi row update is not supported, see\n  `test/test_update.py <test/test_update.py>`_ for an example\n\n\nMeet the system requirements\n````````````````````````````\n- Python\n- An Exasol DB (e.g. `docker-db <test_docker_image_>`_ or a `cloud instance <test_drive_>`_)\n\nODBC-based dialects additionally require the following to be available and set up:\n\n- The packages unixODBC and unixODBC-dev >= 2.2.14\n- The Exasol `ODBC driver <odbc_driver_>`_\n- The ODBC.ini and ODBCINST.ini configurations files setup\n\n\nSetup your python project and install sqlalchemy-exasol\n```````````````````````````````````````````````````````\n\n.. code-block:: shell\n\n    $ pip install sqlalchemy-exasol\n\nfor turbodbc support:\n\n.. code-block:: shell\n\n    $ pip install sqlalchemy-exasol[turbodbc]\n\nTalk to the EXASOL DB using SQLAlchemy\n``````````````````````````````````````\n\n**Websocket based Dialect:**\n\nFor more details regarding the websocket support checkout the section: "What is Websocket support?"\n\n.. code-block:: python\n\n\tfrom sqlalchemy import create_engine\n\turl = "exa+websocket://A_USER:A_PASSWORD@192.168.1.2..8:1234/my_schema?CONNECTIONLCALL=en_US.UTF-8"\n\te = create_engine(url)\n\tr = e.execute("select 42 from dual").fetchall()\n\n\n**Pyodbc (ODBC based Dialect):**\n\n.. code-block:: python\n\n\tfrom sqlalchemy import create_engine\n\turl = "exa+pyodbc://A_USER:A_PASSWORD@192.168.1.2..8:1234/my_schema?CONNECTIONLCALL=en_US.UTF-8&driver=EXAODBC"\n\te = create_engine(url)\n\tr = e.execute("select 42 from dual").fetchall()\n\n**Turbodbc (ODBC based Dialect):**\n\n.. code-block:: python\n\n\tfrom sqlalchemy import create_engine\n\turl = "exa+turbodbc://A_USER:A_PASSWORD@192.168.1.2..8:1234/my_schema?CONNECTIONLCALL=en_US.UTF-8&driver=EXAODBC"\n\te = create_engine(url)\n\tr = e.execute("select 42 from dual").fetchall()\n\n\nThe dialect supports two types of connection urls creating an engine. A DSN (Data Source Name) mode and a host mode:\n\n.. list-table::\n\n    * - Type\n      - Example\n    * - DSN URL\n      - \'exa+pyodbc://USER:PWD@exa_test\'\n    * - HOST URL\n      - \'exa+pyodbc://USER:PWD@192.168.14.227..228:1234/my_schema?parameter\'\n\nFeatures\n++++++++\n\n- SELECT, INSERT, UPDATE, DELETE statements\n\nNotes\n+++++\n\n- Schema name and parameters are optional for the host url\n- At least on Linux/Unix systems it has proven valuable to pass \'CONNECTIONLCALL=en_US.UTF-8\' as a url parameter. This will make sure that the client process (Python) and the EXASOL driver (UTF-8 internal) know how to interpret code pages correctly.\n- Always use all lower-case identifiers for schema, table and column names. SQLAlchemy treats all lower-case identifiers as case-insensitive, the dialect takes care of transforming the identifier into a case-insensitive representation of the specific database (in case of EXASol this is upper-case as for Oracle)\n- As of Exasol client driver version 4.1.2 you can pass the flag \'INTTYPESINRESULTSIFPOSSIBLE=y\' in the connection string (or configure it in your DSN). This will convert DECIMAL data types to Integer-like data types. Creating integers is a factor three faster in Python than creating Decimals.\n\n.. _developer guide: https://github.com/exasol/sqlalchemy-exasol/blob/master/doc/developer_guide/developer_guide.rst\n.. _odbc_driver: https://docs.exasol.com/db/latest/connect_exasol/drivers/odbc/odbc_linux.htm\n.. _test_drive: https://www.exasol.com/test-it-now/cloud/\n.. _test_docker_image: https://github.com/exasol/docker-db\n\nDevelopment & Testing\n`````````````````````\nSee `developer guide`_\n\nWhat is Websocket support?\n``````````````````````````\nIn the context of SQLA and Exasol, Websocket support means that an SQLA dialect\nsupporting the `Exasol Websocket Protocol <https://github.com/exasol/websocket-api>`_\nis provided.\n\nUsing the websocket based protocol instead over ODBC will provide various advantages:\n\n* Less System Dependencies\n* Easier to use than ODBC based driver(s)\n* Lock free metadata calls etc.\n\nFor further details `Why a Websockets API  <https://github.com/exasol/websocket-api#why-a-websockets-api>`_.\n\nExample Usage(s)\n++++++++++++++++++\n\n.. code-block:: python\n\n    from sqla import create_engine\n\n    engine = create_engine("exa+websocket://sys:exasol@127.0.0.1:8888")\n    with engine.connect() as con:\n        ...\n\n.. code-block:: python\n\n    from sqla import create_engine\n\n    # ATTENTION:\n    # In terms of security it is NEVER a good idea to turn of certificate validation!!\n    # In rare cases it may be handy for non-security related reasons.\n    # That said, if you are not a 100% sure about your scenario, stick with the\n    # secure defaults.\n    # In most cases, having a valid certificate and/or configuring the truststore(s)\n    # appropriately is the best/correct solution.\n    engine = create_engine("exa+websocket://sys:exasol@127.0.0.1:8888?SSLCertificate=SSL_VERIFY_NONE")\n    with engine.connect() as con:\n        ...\n\nSupported Connection Parameters\n+++++++++++++++++++++++++++++++\n.. list-table::\n\n   * - Parameter\n     - Values\n     - Comment\n   * - ENCRYPTION\n     - Y, Yes, N, No\n     - Y or Yes Enable Encryption (TLS) default, N or No disable Encryption\n   * - SSLCertificate\n     - SSL_VERIFY_NONE\n     - Disable certificate validation\n\n\nKnown Issues\n++++++++++++\n* Insert\n    - Insert multiple empty rows via prepared statements does not work in all cases\n',
+    'author': 'Exasol AG',
+    'author_email': 'opensource@exasol.com',
+    'maintainer': 'None',
+    'maintainer_email': 'None',
+    'url': 'None',
+    'packages': packages,
+    'package_data': package_data,
+    'install_requires': install_requires,
+    'extras_require': extras_require,
+    'entry_points': entry_points,
+    'python_requires': '>=3.8,<4.0',
+}
 
-.. image:: https://img.shields.io/pypi/pyversions/sqlalchemy-exasol
-    :target: https://pypi.org/project/sqlalchemy-exasol
-    :alt: PyPI - Python Version
 
-.. image:: https://img.shields.io/badge/exasol-7.1.9%20%7C%207.0.18-green
-    :target: https://www.exasol.com/
-    :alt: Exasol - Supported Version(s)
-
-.. image:: https://img.shields.io/badge/code%20style-black-000000.svg
-    :target: https://github.com/psf/black
-    :alt: Formatter - Black
-
-.. image:: https://img.shields.io/badge/imports-isort-ef8336.svg
-    :target: https://pycqa.github.io/isort/
-    :alt: Formatter - Isort
-
-.. image:: https://img.shields.io/badge/pylint-6.4-yellowgreen
-    :target: https://github.com/PyCQA/pylint
-    :alt: Pylint
-
-.. image:: https://img.shields.io/pypi/l/sqlalchemy-exasol
-     :target: https://opensource.org/licenses/BSD-2-Clause
-     :alt: License
-
-.. image:: https://img.shields.io/github/last-commit/exasol/sqlalchemy-exasol
-     :target: https://pypi.org/project/sqlalchemy-exasol/
-     :alt: Last Commit
-
-.. image:: https://img.shields.io/pypi/dm/sqlalchemy-exasol
-    :target: https://pypi.org/project/sqlalchemy-exasol
-    :alt: PyPI - Downloads
-
-
-How to get started
-------------------
-
-We assume you have a good understanding of (unix)ODBC. If not, make sure you
-read their documentation carefully - there are lot's of traps 🪤 to step into.
-
-Turbodbc support
-````````````````
-
-.. warning::
-
-    Maintenance of this feature is on hold. Also it is very likely that turbodbc support will be dropped in future versions.
-
-- You can use Turbodbc with sqlalchemy_exasol if you use a python version >= 3.8.
-- Multi row update is not supported, see
-  `test/test_update.py <test/test_update.py>`_ for an example
-
-
-
-Meet the system requirements
-````````````````````````````
-
-On Linux/Unix like systems you need:
-
-- Python
-- An Exasol DB (e.g. `docker-db <test_docker_image_>`_ or a `cloud instance <test_drive_>`_)
-- The packages unixODBC and unixODBC-dev >= 2.2.14
-- The Exasol `ODBC driver <odbc_driver_>`_
-- The ODBC.ini and ODBCINST.ini configurations files setup
-
-Setup your python project and install sqlalchemy-exasol
-```````````````````````````````````````````````````````
-
-.. code-block:: shell
-
-    $ pip install sqlalchemy-exasol
-
-for turbodbc support:
-
-.. code-block:: shell
-
-    $ pip install sqlalchemy-exasol[turbodbc]
-
-Talk to the EXASOL DB using SQLAlchemy
-``````````````````````````````````````
-
-.. code-block:: python
-
-	from sqlalchemy import create_engine
-	url = "exa+pyodbc://A_USER:A_PASSWORD@192.168.1.2..8:1234/my_schema?CONNECTIONLCALL=en_US.UTF-8&driver=EXAODBC"
-	e = create_engine(url)
-	r = e.execute("select 42 from dual").fetchall()
-
-to use turbodbc as driver:
-
-.. code-block:: python
-
-	from sqlalchemy import create_engine
-	url = "exa+turbodbc://A_USER:A_PASSWORD@192.168.1.2..8:1234/my_schema?CONNECTIONLCALL=en_US.UTF-8&driver=EXAODBC"
-	e = create_engine(url)
-	r = e.execute("select 42 from dual").fetchall()
-
-
-The dialect supports two types of connection urls creating an engine. A DSN (Data Source Name) mode and a host mode:
-
-.. list-table::
-
-    * - Type
-      - Example
-    * - DSN URL
-      - 'exa+pyodbc://USER:PWD@exa_test'
-    * - HOST URL
-      - 'exa+pyodbc://USER:PWD@192.168.14.227..228:1234/my_schema?parameter'
-
-Features
-++++++++
-
-- SELECT, INSERT, UPDATE, DELETE statements
-
-Notes
-+++++
-
-- Schema name and parameters are optional for the host url
-- At least on Linux/Unix systems it has proven valuable to pass 'CONNECTIONLCALL=en_US.UTF-8' as a url parameter. This will make sure that the client process (Python) and the EXASOL driver (UTF-8 internal) know how to interpret code pages correctly.
-- Always use all lower-case identifiers for schema, table and column names. SQLAlchemy treats all lower-case identifiers as case-insensitive, the dialect takes care of transforming the identifier into a case-insensitive representation of the specific database (in case of EXASol this is upper-case as for Oracle)
-- As of Exasol client driver version 4.1.2 you can pass the flag 'INTTYPESINRESULTSIFPOSSIBLE=y' in the connection string (or configure it in your DSN). This will convert DECIMAL data types to Integer-like data types. Creating integers is a factor three faster in Python than creating Decimals.
-
-.. _developer guide: https://github.com/exasol/sqlalchemy-exasol/blob/master/doc/developer_guide/developer_guide.rst
-.. _odbc_driver: https://docs.exasol.com/db/latest/connect_exasol/drivers/odbc/odbc_linux.htm
-.. _test_drive: https://www.exasol.com/test-it-now/cloud/
-.. _test_docker_image: https://github.com/exasol/docker-db
-
-Development & Testing
-`````````````````````
-See `developer guide`_
-
-Websocket support
------------------
-
-.. attention::
-
-    The Websocket support is currently in Beta, therefore it should not be used in production.
-    We also recommend to have a look into the known issues, before you start using it.
-
-    If you encounter any issue, please `create an issue <https://github.com/exasol/sqlalchemy-exasol/issues/new?assignees=&labels=bug&projects=&template=bug.md&title=%F0%9F%90%9E+%3CInsert+Title%3E>`_.
-    With your feedback, we will be able to stabilize this feature more quickly.
-
-What is Websocket support?
-``````````````````````````
-In the context of SQLA and Exasol, Websocket support means that an SQLA dialect
-supporting the `Exasol Websocket Protocol <https://github.com/exasol/websocket-api>`_
-is provided.
-
-Using the websocket based protocol instead over ODBC will provide various advantages:
-
-* Less System Dependencies
-* Easier to use than ODBC based driver(s)
-* Lock free metadata calls etc.
-
-For further details `Why a Websockets API  <https://github.com/exasol/websocket-api#why-a-websockets-api>`_.
-
-Examples Usage(s)
-`````````````````
-
-.. code-block:: python
-
-    from sqla import create_engine
-
-    engine = create_engine("exa+websocket://sys:exasol@127.0.0.1:8888")
-    with engine.connect() as con:
-        ...
-
-.. code-block:: python
-
-    from sqla import create_engine
-
-    # ATTENTION:
-    # In terms of security it is NEVER a good idea to turn of certificate validation!!
-    # In rare cases it may be handy for non-security related reasons.
-    # That said, if you are not a 100% sure about your scenario, stick with the
-    # secure defaults.
-    # In most cases, having a valid certificate and/or configuring the truststore(s)
-    # appropriately is the best/correct solution.
-    engine = create_engine("exa+websocket://sys:exasol@127.0.0.1:8888?SSLCertificate=SSL_VERIFY_NONE")
-    with engine.connect() as con:
-        ...
-
-Supported Connection Parameters
-```````````````````````````````
-.. list-table::
-
-   * - Parameter
-     - Values
-     - Comment
-   * - ENCRYPTION
-     - Y, Yes, N, No
-     - Y or Yes Enable Encryption (TLS) default, N or No disable Encryption
-   * - SSLCertificate
-     - SSL_VERIFY_NONE
-     - Disable certificate validation
-
-
-Known Issues
-````````````
-
-* Literal casts within prepared statements do not work
-    - :code:`INSERT INTO t (x) VALUES (CAST(? AS VARCHAR(50)));`
-* Various conversions regarding float, decimals
-    - Certain scenarios still yield a :code:`string` type instead :code:`float` or :code:`decimal` type.
-* Insert
-    - Insert multiple rows via prepared statements does not work in all cases
-    - Insert from SELECT does not work
-* For some prepared statements, the wss protocol type conversion does not work properly
-    - Error messages usually state some JSON type mismatch, e.g.: '... getString: JSON value is not a string ...'
-* Known failing tests of the SQLA compliance test suite
-    - FAILED test/integration/sqlalchemy/test_suite.py::CastTypeDecoratorTest_exasol+exasol_driver_websocket_dbapi2::test_special_type - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::ExistsTest_exasol+exasol_driver_websocket_dbapi2::test_select_exists - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::ExistsTest_exasol+exasol_driver_websocket_dbapi2::test_select_exists_false - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::InsertBehaviorTest_exasol+exasol_driver_websocket_dbapi2::test_empty_insert_multiple - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - ERROR  test/integration/sqlalchemy/test_suite.py::InsertBehaviorTest_exasol+exasol_driver_websocket_dbapi2::test_empty_insert_multiple_teardown - ERROR
-    - FAILED test/integration/sqlalchemy/test_suite.py::InsertBehaviorTest_exasol+exasol_driver_websocket_dbapi2::test_insert_from_select - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::InsertBehaviorTest_exasol+exasol_driver_websocket_dbapi2::test_insert_from_select_with_defaults - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::NumericTest_exasol+exasol_driver_websocket_dbapi2::test_float_as_decimal - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::NumericTest_exasol+exasol_driver_websocket_dbapi2::test_float_as_float - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::NumericTest_exasol+exasol_driver_websocket_dbapi2::test_float_coerce_round_trip - AssertionError: '15.7563' != 15.7563
-    - FAILED test/integration/sqlalchemy/test_suite.py::NumericTest_exasol+exasol_driver_websocket_dbapi2::test_float_custom_scale - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::NumericTest_exasol+exasol_driver_websocket_dbapi2::test_numeric_as_float - AssertionError: {'15.7563'} != {15.7563}
-    - FAILED test/integration/sqlalchemy/test_suite.py::NumericTest_exasol+exasol_driver_websocket_dbapi2::test_render_literal_numeric_asfloat - AssertionError: assert '15.7563' in [15.7563]
+setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sqlalchemy_exasol-4.5.1/exasol/driver/odbc.py` & `sqlalchemy_exasol-4.6.0/exasol/driver/odbc.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.5.1/exasol/driver/websocket/_connection.py` & `sqlalchemy_exasol-4.6.0/exasol/driver/websocket/_connection.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.5.1/exasol/driver/websocket/_cursor.py` & `sqlalchemy_exasol-4.6.0/exasol/driver/websocket/_cursor.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 This module provides `PEP-249`_ DBAPI compliant cursor implementation.
 (see also `PEP-249-cursor`_)
 
 .. _PEP-249-cursor: https://peps.python.org/pep-0249/#cursor-objects
 """
 import datetime
 import decimal
-import time
 from collections import defaultdict
 from dataclasses import (
     astuple,
     dataclass,
 )
 from functools import wraps
 from typing import Optional
@@ -227,22 +226,81 @@
 
         connection = self._connection.connection
         try:
             self._cursor = connection.execute(operation)
         except pyexasol.exceptions.ExaError as ex:
             raise Error() from ex
 
+    @staticmethod
+    def _adapt_to_requested_db_types(parameters, db_response):
+        """
+        Adapt parameter types to match the types requested by the DB in the
+        `createPreparedStatement <https://github.com/exasol/websocket-api/blob/master/docs/commands/createPreparedStatementV1.md>`_
+        response.
+
+        Args:
+
+            parameters: which will be passed/send to the database.
+            db_response: contains the DB response including the required types.
+
+
+        Attention:
+
+            This shim method currently only patches the following types:
+
+                * VARCHAR
+                * DOUBLE
+
+            therefore it the future it may be necessary to improve or extend this.
+
+            A hint that patching of a specific type is required, could be and
+            error message similar to this one:
+
+            .. code-block::
+
+                pyexasol.exceptions.ExaRequestError:
+                ...
+                message  => getString: JSON value is not a string. (...)
+                ...
+        """
+
+        def varchar(value):
+            if value is None:
+                return None
+            return str(value)
+
+        def double(value):
+            if value is None:
+                return None
+            return float(value)
+
+        converters = defaultdict(
+            lambda: _identity, {"VARCHAR": varchar, "DOUBLE": double}
+        )
+        selected_converters = (
+            converters[column["dataType"]["type"]] for column in db_response["columns"]
+        )
+        parameters = zip(selected_converters, parameters)
+        parameters = [converter(value) for converter, value in parameters]
+        return parameters
+
     @_is_not_closed
     def executemany(self, operation, seq_of_parameters):
         """See also :py:meth: `Cursor.executemany`"""
         parameters = [
             [_dbapi2pyexasol(p) for p in params] for params in seq_of_parameters
         ]
         connection = self._connection.connection
         self._cursor = connection.cls_statement(connection, operation, prepare=True)
+
+        parameter_data = self._cursor.parameter_data
+        parameters = [
+            Cursor._adapt_to_requested_db_types(params, parameter_data)
+            for params in parameters
+        ]
         try:
             self._cursor.execute_prepared(parameters)
         except pyexasol.exceptions.ExaError as ex:
             raise Error() from ex
 
     def _convert(self, rows):
         if rows is None:
```

### Comparing `sqlalchemy_exasol-4.5.1/exasol/driver/websocket/_errors.py` & `sqlalchemy_exasol-4.6.0/exasol/driver/websocket/_errors.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.5.1/exasol/driver/websocket/_protocols.py` & `sqlalchemy_exasol-4.6.0/exasol/driver/websocket/_protocols.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.5.1/exasol/driver/websocket/_types.py` & `sqlalchemy_exasol-4.6.0/exasol/driver/websocket/_types.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.5.1/exasol/driver/websocket/dbapi2.py` & `sqlalchemy_exasol-4.6.0/exasol/driver/websocket/dbapi2.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.5.1/pyproject.toml` & `sqlalchemy_exasol-4.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [tool.poetry]
 name = "sqlalchemy_exasol"
 packages = [
     { include = "sqlalchemy_exasol" },
     { include = "exasol" }
 ]
-version = "4.5.1"
+version = "4.6.0"
 description = "EXASOL dialect for SQLAlchemy"
 readme = "README.rst"
 authors = [
     "Exasol AG <opensource@exasol.com>",
     "Blue Yonder GmbH",
 ]
 license = "BSD"
```

### Comparing `sqlalchemy_exasol-4.5.1/sqlalchemy_exasol/base.py` & `sqlalchemy_exasol-4.6.0/sqlalchemy_exasol/base.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.5.1/sqlalchemy_exasol/pyodbc.py` & `sqlalchemy_exasol-4.6.0/sqlalchemy_exasol/pyodbc.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.5.1/sqlalchemy_exasol/requirements.py` & `sqlalchemy_exasol-4.6.0/sqlalchemy_exasol/requirements.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.5.1/sqlalchemy_exasol/turbodbc.py` & `sqlalchemy_exasol-4.6.0/sqlalchemy_exasol/turbodbc.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.5.1/sqlalchemy_exasol/util.py` & `sqlalchemy_exasol-4.6.0/sqlalchemy_exasol/util.py`

 * *Files identical despite different names*

### Comparing `sqlalchemy_exasol-4.5.1/sqlalchemy_exasol/websocket.py` & `sqlalchemy_exasol-4.6.0/sqlalchemy_exasol/websocket.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 class Decimal(sqltypes.DECIMAL):
     def bind_processor(self, dialect):
         return super().bind_processor(dialect)
 
     def result_processor(self, dialect, coltype):
         if not self.asdecimal:
-            return None
+            return lambda value: None if value is None else float(value)
 
         fstring = "%%.%df" % self._effective_decimal_return_scale
 
         def to_decimal(value):
             if value is None:
                 return None
             elif isinstance(value, decimal.Decimal):
```

### Comparing `sqlalchemy_exasol-4.5.1/PKG-INFO` & `sqlalchemy_exasol-4.6.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlalchemy-exasol
-Version: 4.5.1
+Version: 4.6.0
 Summary: EXASOL dialect for SQLAlchemy
 License: BSD
 Keywords: exasol,sql,sqlalchemy,data science,database
 Author: Exasol AG
 Author-email: opensource@exasol.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -42,16 +42,16 @@
 Project-URL: Source, https://github.com/exasol/sqlalchemy-exasol
 Description-Content-Type: text/x-rst
 
 SQLAlchemy Dialect for EXASOL DB
 ================================
 
 
-.. image:: https://github.com/exasol/sqlalchemy_exasol/workflows/CI/badge.svg?branch=master
-    :target: https://github.com/exasol/sqlalchemy_exasol/actions?query=workflow%3ACI
+.. image:: https://github.com/exasol/sqlalchemy-exasol/actions/workflows/ci-cd.yml/badge.svg?branch=master&event=push
+    :target: https://github.com/exasol/sqlalchemy-exasol/actions/workflows/ci-cd.yml
      :alt: CI Status
 
 .. image:: https://img.shields.io/pypi/v/sqlalchemy_exasol
      :target: https://pypi.org/project/sqlalchemy-exasol/
      :alt: PyPI Version
 
 .. image:: https://img.shields.io/pypi/pyversions/sqlalchemy-exasol
@@ -86,41 +86,46 @@
     :target: https://pypi.org/project/sqlalchemy-exasol
     :alt: PyPI - Downloads
 
 
 How to get started
 ------------------
 
-We assume you have a good understanding of (unix)ODBC. If not, make sure you
-read their documentation carefully - there are lot's of traps 🪤 to step into.
+Currently, sqlalchemy-exasol supports multiple dialects. The core difference
+being if the dialect is :code:`odbc` or :code:`websocket` based.
+
+Generally, we advise to use the websocket based Dialect, because odbc
+based dialects require a good understanding of (unix)ODBC and the setup is
+significant more complicated.
+
 
 Turbodbc support
 ````````````````
 
 .. warning::
 
     Maintenance of this feature is on hold. Also it is very likely that turbodbc support will be dropped in future versions.
 
 - You can use Turbodbc with sqlalchemy_exasol if you use a python version >= 3.8.
 - Multi row update is not supported, see
   `test/test_update.py <test/test_update.py>`_ for an example
 
 
-
 Meet the system requirements
 ````````````````````````````
-
-On Linux/Unix like systems you need:
-
 - Python
 - An Exasol DB (e.g. `docker-db <test_docker_image_>`_ or a `cloud instance <test_drive_>`_)
+
+ODBC-based dialects additionally require the following to be available and set up:
+
 - The packages unixODBC and unixODBC-dev >= 2.2.14
 - The Exasol `ODBC driver <odbc_driver_>`_
 - The ODBC.ini and ODBCINST.ini configurations files setup
 
+
 Setup your python project and install sqlalchemy-exasol
 ```````````````````````````````````````````````````````
 
 .. code-block:: shell
 
     $ pip install sqlalchemy-exasol
 
@@ -129,22 +134,36 @@
 .. code-block:: shell
 
     $ pip install sqlalchemy-exasol[turbodbc]
 
 Talk to the EXASOL DB using SQLAlchemy
 ``````````````````````````````````````
 
+**Websocket based Dialect:**
+
+For more details regarding the websocket support checkout the section: "What is Websocket support?"
+
+.. code-block:: python
+
+	from sqlalchemy import create_engine
+	url = "exa+websocket://A_USER:A_PASSWORD@192.168.1.2..8:1234/my_schema?CONNECTIONLCALL=en_US.UTF-8"
+	e = create_engine(url)
+	r = e.execute("select 42 from dual").fetchall()
+
+
+**Pyodbc (ODBC based Dialect):**
+
 .. code-block:: python
 
 	from sqlalchemy import create_engine
 	url = "exa+pyodbc://A_USER:A_PASSWORD@192.168.1.2..8:1234/my_schema?CONNECTIONLCALL=en_US.UTF-8&driver=EXAODBC"
 	e = create_engine(url)
 	r = e.execute("select 42 from dual").fetchall()
 
-to use turbodbc as driver:
+**Turbodbc (ODBC based Dialect):**
 
 .. code-block:: python
 
 	from sqlalchemy import create_engine
 	url = "exa+turbodbc://A_USER:A_PASSWORD@192.168.1.2..8:1234/my_schema?CONNECTIONLCALL=en_US.UTF-8&driver=EXAODBC"
 	e = create_engine(url)
 	r = e.execute("select 42 from dual").fetchall()
@@ -179,41 +198,30 @@
 .. _test_drive: https://www.exasol.com/test-it-now/cloud/
 .. _test_docker_image: https://github.com/exasol/docker-db
 
 Development & Testing
 `````````````````````
 See `developer guide`_
 
-Websocket support
------------------
-
-.. attention::
-
-    The Websocket support is currently in Beta, therefore it should not be used in production.
-    We also recommend to have a look into the known issues, before you start using it.
-
-    If you encounter any issue, please `create an issue <https://github.com/exasol/sqlalchemy-exasol/issues/new?assignees=&labels=bug&projects=&template=bug.md&title=%F0%9F%90%9E+%3CInsert+Title%3E>`_.
-    With your feedback, we will be able to stabilize this feature more quickly.
-
 What is Websocket support?
 ``````````````````````````
 In the context of SQLA and Exasol, Websocket support means that an SQLA dialect
 supporting the `Exasol Websocket Protocol <https://github.com/exasol/websocket-api>`_
 is provided.
 
 Using the websocket based protocol instead over ODBC will provide various advantages:
 
 * Less System Dependencies
 * Easier to use than ODBC based driver(s)
 * Lock free metadata calls etc.
 
 For further details `Why a Websockets API  <https://github.com/exasol/websocket-api#why-a-websockets-api>`_.
 
-Examples Usage(s)
-`````````````````
+Example Usage(s)
+++++++++++++++++++
 
 .. code-block:: python
 
     from sqla import create_engine
 
     engine = create_engine("exa+websocket://sys:exasol@127.0.0.1:8888")
     with engine.connect() as con:
@@ -231,48 +239,26 @@
     # In most cases, having a valid certificate and/or configuring the truststore(s)
     # appropriately is the best/correct solution.
     engine = create_engine("exa+websocket://sys:exasol@127.0.0.1:8888?SSLCertificate=SSL_VERIFY_NONE")
     with engine.connect() as con:
         ...
 
 Supported Connection Parameters
-```````````````````````````````
++++++++++++++++++++++++++++++++
 .. list-table::
 
    * - Parameter
      - Values
      - Comment
    * - ENCRYPTION
      - Y, Yes, N, No
      - Y or Yes Enable Encryption (TLS) default, N or No disable Encryption
    * - SSLCertificate
      - SSL_VERIFY_NONE
      - Disable certificate validation
 
 
 Known Issues
-````````````
-
-* Literal casts within prepared statements do not work
-    - :code:`INSERT INTO t (x) VALUES (CAST(? AS VARCHAR(50)));`
-* Various conversions regarding float, decimals
-    - Certain scenarios still yield a :code:`string` type instead :code:`float` or :code:`decimal` type.
+++++++++++++
 * Insert
-    - Insert multiple rows via prepared statements does not work in all cases
-    - Insert from SELECT does not work
-* For some prepared statements, the wss protocol type conversion does not work properly
-    - Error messages usually state some JSON type mismatch, e.g.: '... getString: JSON value is not a string ...'
-* Known failing tests of the SQLA compliance test suite
-    - FAILED test/integration/sqlalchemy/test_suite.py::CastTypeDecoratorTest_exasol+exasol_driver_websocket_dbapi2::test_special_type - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::ExistsTest_exasol+exasol_driver_websocket_dbapi2::test_select_exists - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::ExistsTest_exasol+exasol_driver_websocket_dbapi2::test_select_exists_false - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::InsertBehaviorTest_exasol+exasol_driver_websocket_dbapi2::test_empty_insert_multiple - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - ERROR  test/integration/sqlalchemy/test_suite.py::InsertBehaviorTest_exasol+exasol_driver_websocket_dbapi2::test_empty_insert_multiple_teardown - ERROR
-    - FAILED test/integration/sqlalchemy/test_suite.py::InsertBehaviorTest_exasol+exasol_driver_websocket_dbapi2::test_insert_from_select - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::InsertBehaviorTest_exasol+exasol_driver_websocket_dbapi2::test_insert_from_select_with_defaults - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::NumericTest_exasol+exasol_driver_websocket_dbapi2::test_float_as_decimal - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::NumericTest_exasol+exasol_driver_websocket_dbapi2::test_float_as_float - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::NumericTest_exasol+exasol_driver_websocket_dbapi2::test_float_coerce_round_trip - AssertionError: '15.7563' != 15.7563
-    - FAILED test/integration/sqlalchemy/test_suite.py::NumericTest_exasol+exasol_driver_websocket_dbapi2::test_float_custom_scale - sqlalchemy.exc.DBAPIError: (exasol.driver.websocket._errors.Error)
-    - FAILED test/integration/sqlalchemy/test_suite.py::NumericTest_exasol+exasol_driver_websocket_dbapi2::test_numeric_as_float - AssertionError: {'15.7563'} != {15.7563}
-    - FAILED test/integration/sqlalchemy/test_suite.py::NumericTest_exasol+exasol_driver_websocket_dbapi2::test_render_literal_numeric_asfloat - AssertionError: assert '15.7563' in [15.7563]
+    - Insert multiple empty rows via prepared statements does not work in all cases
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

