# Comparing `tmp/logilab-database-1.8.1.tar.gz` & `tmp/logilab-database-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/logilab-database-1.8.1.tar", last modified: Tue Dec 13 09:46:59 2011, max compression
+gzip compressed data, was "logilab-database-1.9.0.tar", last modified: Wed Dec 19 16:59:32 2012, max compression, from Unix
```

## Comparing `logilab-database-1.8.1.tar` & `logilab-database-1.9.0.tar`

### file list

```diff
@@ -1,37 +1,28 @@
-drwxr-xr-x   0 arthur    (1000) arthur    (1000)        0 2011-12-13 09:46:59.000000 logilab-database-1.8.1/
--rw-r--r--   0 arthur    (1000) arthur    (1000)    35025 2011-12-13 09:37:33.000000 logilab-database-1.8.1/__init__.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)      714 2011-12-13 09:46:59.000000 logilab-database-1.8.1/PKG-INFO
--rw-r--r--   0 arthur    (1000) arthur    (1000)    17137 2011-12-13 09:37:33.000000 logilab-database-1.8.1/postgres.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)      327 2010-10-11 12:47:47.000000 logilab-database-1.8.1/ftiparser.g
--rw-r--r--   0 arthur    (1000) arthur    (1000)    17987 2010-10-11 12:47:47.000000 logilab-database-1.8.1/COPYING
--rw-r--r--   0 arthur    (1000) arthur    (1000)     6223 2011-12-13 09:37:33.000000 logilab-database-1.8.1/setup.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)     5832 2011-10-18 14:42:02.000000 logilab-database-1.8.1/ftiquery.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)     2547 2011-10-18 14:42:02.000000 logilab-database-1.8.1/ftiparser.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)      390 2011-12-13 09:37:33.000000 logilab-database-1.8.1/README
--rw-r--r--   0 arthur    (1000) arthur    (1000)     9713 2011-10-18 14:42:02.000000 logilab-database-1.8.1/sqlgen.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)       77 2011-10-18 14:42:02.000000 logilab-database-1.8.1/MANIFEST.in
--rw-r--r--   0 arthur    (1000) arthur    (1000)     3773 2011-12-13 09:38:09.000000 logilab-database-1.8.1/ChangeLog
-drwxr-xr-x   0 arthur    (1000) arthur    (1000)        0 2011-12-13 09:46:59.000000 logilab-database-1.8.1/test/
--rw-r--r--   0 arthur    (1000) arthur    (1000)     4175 2011-10-18 14:42:02.000000 logilab-database-1.8.1/test/unittest_sqlserver2005.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)     3238 2011-10-18 14:42:02.000000 logilab-database-1.8.1/test/unittest_postgres.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)     2174 2011-10-18 14:42:02.000000 logilab-database-1.8.1/test/unittest_mysql.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)    14313 2011-10-18 14:42:02.000000 logilab-database-1.8.1/test/unittest_db.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)     5574 2011-10-18 14:42:02.000000 logilab-database-1.8.1/test/unittest_fti.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)     1475 2011-06-07 15:45:32.000000 logilab-database-1.8.1/test/unittest_sqlite.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)    12934 2011-10-18 14:42:02.000000 logilab-database-1.8.1/mysql.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)     1558 2011-10-18 14:42:02.000000 logilab-database-1.8.1/sqlserver2000.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)    26527 2010-10-11 12:47:47.000000 logilab-database-1.8.1/COPYING.LESSER
--rw-r--r--   0 arthur    (1000) arthur    (1000)    15546 2011-12-13 09:38:09.000000 logilab-database-1.8.1/sqlserver2005.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)     9074 2011-10-18 14:42:02.000000 logilab-database-1.8.1/sqlserver.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)    12714 2011-10-18 14:42:02.000000 logilab-database-1.8.1/sqlite.py
-drwxr-xr-x   0 arthur    (1000) arthur    (1000)        0 2011-12-13 09:46:59.000000 logilab-database-1.8.1/logilab_database.egg-info/
--rw-r--r--   0 arthur    (1000) arthur    (1000)        1 2011-12-13 09:46:58.000000 logilab-database-1.8.1/logilab_database.egg-info/dependency_links.txt
--rw-r--r--   0 arthur    (1000) arthur    (1000)      714 2011-12-13 09:46:58.000000 logilab-database-1.8.1/logilab_database.egg-info/PKG-INFO
--rw-r--r--   0 arthur    (1000) arthur    (1000)        8 2011-12-13 09:46:58.000000 logilab-database-1.8.1/logilab_database.egg-info/namespace_packages.txt
--rw-r--r--   0 arthur    (1000) arthur    (1000)       24 2011-12-13 09:46:58.000000 logilab-database-1.8.1/logilab_database.egg-info/requires.txt
--rw-r--r--   0 arthur    (1000) arthur    (1000)        8 2011-12-13 09:46:58.000000 logilab-database-1.8.1/logilab_database.egg-info/top_level.txt
--rw-r--r--   0 arthur    (1000) arthur    (1000)      667 2011-12-13 09:46:58.000000 logilab-database-1.8.1/logilab_database.egg-info/SOURCES.txt
--rw-r--r--   0 arthur    (1000) arthur    (1000)     8250 2011-10-18 14:42:02.000000 logilab-database-1.8.1/fti.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)     1594 2011-10-18 14:42:02.000000 logilab-database-1.8.1/sqlserver2008.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)     1413 2011-12-13 09:38:09.000000 logilab-database-1.8.1/__pkginfo__.py
--rw-r--r--   0 arthur    (1000) arthur    (1000)       59 2011-12-13 09:46:59.000000 logilab-database-1.8.1/setup.cfg
+drwxrwxr-x   0 narval     (105) narval     (109)        0 2012-12-19 16:59:32.000000 logilab-database-1.9.0/
+-rw-------   0 narval     (105) narval     (109)     1594 2012-12-19 16:47:13.000000 logilab-database-1.9.0/sqlserver2008.py
+-rw-------   0 narval     (105) narval     (109)    12216 2012-12-19 16:47:13.000000 logilab-database-1.9.0/sqlite.py
+drwxrwxr-x   0 narval     (105) narval     (109)        0 2012-12-19 16:59:32.000000 logilab-database-1.9.0/test/
+-rw-------   0 narval     (105) narval     (109)     4175 2012-12-19 16:47:13.000000 logilab-database-1.9.0/test/unittest_sqlserver2005.py
+-rw-------   0 narval     (105) narval     (109)     3238 2012-12-19 16:47:13.000000 logilab-database-1.9.0/test/unittest_postgres.py
+-rw-------   0 narval     (105) narval     (109)     1475 2012-12-19 16:47:13.000000 logilab-database-1.9.0/test/unittest_sqlite.py
+-rw-------   0 narval     (105) narval     (109)     2174 2012-12-19 16:47:13.000000 logilab-database-1.9.0/test/unittest_mysql.py
+-rw-------   0 narval     (105) narval     (109)    14313 2012-12-19 16:47:13.000000 logilab-database-1.9.0/test/unittest_db.py
+-rw-------   0 narval     (105) narval     (109)     5574 2012-12-19 16:47:13.000000 logilab-database-1.9.0/test/unittest_fti.py
+-rw-------   0 narval     (105) narval     (109)     3985 2012-12-19 16:47:13.000000 logilab-database-1.9.0/ChangeLog
+-rw-------   0 narval     (105) narval     (109)     8250 2012-12-19 16:47:13.000000 logilab-database-1.9.0/fti.py
+-rw-------   0 narval     (105) narval     (109)     9074 2012-12-19 16:47:13.000000 logilab-database-1.9.0/sqlserver.py
+-rw-------   0 narval     (105) narval     (109)      327 2012-12-19 16:47:13.000000 logilab-database-1.9.0/ftiparser.g
+-rw-------   0 narval     (105) narval     (109)    12934 2012-12-19 16:47:13.000000 logilab-database-1.9.0/mysql.py
+-rw-------   0 narval     (105) narval     (109)     5832 2012-12-19 16:47:13.000000 logilab-database-1.9.0/ftiquery.py
+-rw-------   0 narval     (105) narval     (109)     2547 2012-12-19 16:47:13.000000 logilab-database-1.9.0/ftiparser.py
+-rw-------   0 narval     (105) narval     (109)      390 2012-12-19 16:47:13.000000 logilab-database-1.9.0/README
+-rw-------   0 narval     (105) narval     (109)    15383 2012-12-19 16:47:13.000000 logilab-database-1.9.0/sqlserver2005.py
+-rw-rw-r--   0 narval     (105) narval     (109)      714 2012-12-19 16:59:32.000000 logilab-database-1.9.0/PKG-INFO
+-rw-------   0 narval     (105) narval     (109)    26527 2012-12-19 16:47:13.000000 logilab-database-1.9.0/COPYING.LESSER
+-rw-------   0 narval     (105) narval     (109)    36514 2012-12-19 16:47:13.000000 logilab-database-1.9.0/__init__.py
+-rw-------   0 narval     (105) narval     (109)     1413 2012-12-19 16:47:13.000000 logilab-database-1.9.0/__pkginfo__.py
+-rw-------   0 narval     (105) narval     (109)    18061 2012-12-19 16:47:13.000000 logilab-database-1.9.0/postgres.py
+-rw-------   0 narval     (105) narval     (109)     9713 2012-12-19 16:47:13.000000 logilab-database-1.9.0/sqlgen.py
+-rw-------   0 narval     (105) narval     (109)    17987 2012-12-19 16:47:13.000000 logilab-database-1.9.0/COPYING
+-rw-------   0 narval     (105) narval     (109)     1558 2012-12-19 16:47:13.000000 logilab-database-1.9.0/sqlserver2000.py
+-rw-------   0 narval     (105) narval     (109)     6223 2012-12-19 16:47:13.000000 logilab-database-1.9.0/setup.py
```

### Comparing `logilab-database-1.8.1/__init__.py` & `logilab-database-1.9.0/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2003-2011 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2012 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of logilab-database.
 #
 # logilab-database is free software: you can redistribute it and/or modify it
 # under the terms of the GNU Lesser General Public License as published by the
 # Free Software Foundation, either version 2.1 of the License, or (at your
@@ -19,44 +19,51 @@
 database connection whatever the database and client lib used.
 
 Currently support:
 
 - postgresql (pgdb, psycopg, psycopg2, pyPgSQL)
 - mysql (MySQLdb)
 - sqlite (pysqlite2, sqlite, sqlite3)
+- sqlserver 2000, 2005, 2008 (pyodbc, adodbapi)
 
 just use the `get_connection` function from this module to get a
 wrapped connection.  If multiple drivers for a database are available,
 you can control which one you want to use using the
 `set_prefered_driver` function.
 
 Additional helpers are also provided for advanced functionalities such
 as listing existing users or databases, creating database... Get the
 helper for your database using the `get_db_helper` function.
 """
+from __future__ import with_statement
 
 __docformat__ = "restructuredtext en"
 
 import sys
+import threading
 import logging
 from datetime import datetime, time
 
 from logilab.common.modutils import load_module_from_name
 from logilab.common.date import utcdatetime, utctime
 
 _LOGGER = logging.getLogger('logilab.database')
 
 USE_MX_DATETIME = False
 
+_LOAD_MODULES_LOCK = threading.Lock()
+
 _PREFERED_DRIVERS = {}
 _ADV_FUNC_HELPER_DIRECTORY = {}
 
 def _ensure_module_loaded(driver):
     if driver in ('postgres', 'sqlite', 'mysql', 'sqlserver2005'):
-        __import__('logilab.database.%s' % driver)
+        with _LOAD_MODULES_LOCK:
+            __import__('logilab.database.%s' % driver)
+
 # main functions ###############################################################
 
 def get_db_helper(driver):
     """returns an advanced function helper for the given driver"""
     _ensure_module_loaded(driver)
     return _ADV_FUNC_HELPER_DIRECTORY[driver]()
 
@@ -79,15 +86,15 @@
     """return a db connection according to given arguments"""
     _ensure_module_loaded(driver)
     module, modname = _import_driver_module(driver, drivers)
     try:
         adapter = _ADAPTER_DIRECTORY.get_adapter(driver, modname)
     except NoAdapterFound, err:
         if not quiet:
-            msg = 'No Adapter found for %s, using default one' 
+            msg = 'No Adapter found for %s, using default one'
             _LOGGER.warning(msg, err.objname)
         adapted_module = DBAPIAdapter(module, pywrap)
     else:
         adapted_module = adapter(module, pywrap)
     if host and not port:
         try:
             host, port = host.split(':', 1)
@@ -102,24 +109,25 @@
     """sets the preferred driver module for driver
     driver is the name of the db engine (postgresql, mysql...)
     module is the name of the module providing the connect function
     syntax is (params_func, post_process_func_or_None)
     _drivers is a optional dictionary of drivers
     """
     _ensure_module_loaded(driver)
-    try:
-        modules = _drivers[driver]
-    except KeyError:
-        raise UnknownDriver('Unknown driver %s' % driver)
-    # Remove module from modules list, and re-insert it in first position
-    try:
-        modules.remove(module)
-    except ValueError:
-        raise UnknownDriver('Unknown module %s for %s' % (module, driver))
-    modules.insert(0, module)
+    with _LOAD_MODULES_LOCK:
+        try:
+            modules = _drivers[driver]
+        except KeyError:
+            raise UnknownDriver('Unknown driver %s' % driver)
+        # Remove module from modules list, and re-insert it in first position
+        try:
+            modules.remove(module)
+        except ValueError:
+            raise UnknownDriver('Unknown module %s for %s' % (module, driver))
+        modules.insert(0, module)
 
 
 # unified db api ###############################################################
 
 class UnknownDriver(Exception):
     """raised when a unknown driver is given to get connection"""
 
@@ -171,26 +179,27 @@
 
     :rtype: tuple
     :returns: the tuple module_object, module_name where module_object
               is the dbapi module, and modname the module's name
     """
     if not driver in drivers:
         raise UnknownDriver(driver)
-    for modname in drivers[driver]:
-        try:
-            if not quiet:
-                _LOGGER.info('Trying %s', modname)
-            module = load_module_from_name(modname, use_sys=False)
-            break
-        except ImportError:
-            if not quiet:
-                _LOGGER.warning('%s is not available', modname)
-            continue
-    else:
-        raise ImportError('Unable to import a %s module' % driver)
+    with _LOAD_MODULES_LOCK:
+        for modname in drivers[driver]:
+            try:
+                if not quiet:
+                    _LOGGER.info('Trying %s', modname)
+                module = load_module_from_name(modname, use_sys=False)
+                break
+            except ImportError:
+                if not quiet:
+                    _LOGGER.warning('%s is not available', modname)
+                continue
+        else:
+            raise ImportError('Unable to import a %s module' % driver)
     return module, modname
 
 
 ## base connection and cursor wrappers #####################
 
 class _SimpleConnectionWrapper(object):
     """A simple connection wrapper in python to decorated C-level connections
@@ -272,14 +281,16 @@
 class DBAPIAdapter(object):
     """Base class for all DBAPI adapters"""
     UNKNOWN = None
     # True if the fetch*() methods return a mutable structure (i.e. not a tuple)
     row_is_mutable = False
     # True if the fetch*() methods return unicode and not binary strings
     returns_unicode = False
+    # True is the backend support COPY FROM method
+    support_copy_from = False
 
     def __init__(self, native_module, pywrap=False):
         """
         :type native_module: module
         :param native_module: the database's driver adapted module
         """
         self._native_module = native_module
@@ -320,14 +331,16 @@
         transform = None
         if typecode == self.STRING and not self.returns_unicode:
             transform = lambda v: unicode(v, encoding, 'replace')
         elif typecode == self.BOOLEAN:
             transform = bool
         elif typecode == self.BINARY and binarywrap is not None:
             transform = binarywrap
+        elif typecode == self.DATETIME: # XXX only for TZDatetime w/ backend returning some tzinfo
+            transform = lambda v: utcdatetime(v) if isinstance(v, datetime) else v
         elif typecode == self.UNKNOWN:
             # may occurs on constant selection for instance (e.g. SELECT 'hop')
             # with postgresql at least
             transform = lambda v: unicode(v, encoding, 'replace') if isinstance(v, str) else v
         return transform
 
     def process_cursor(self, cursor, encoding, binarywrap=None):
@@ -363,15 +376,15 @@
         returned by the dbapi module to standard python objects (e.g.
         unicode, bool, etc.)
         """
         transformations = []
         for i, coldescr in enumerate(description):
             transform = self._transformation_callback(coldescr, encoding, binarywrap)
             if transform is not None:
-                transformations.append((i, transform))
+                transformations.append( (i, transform) )
         return transformations
 
     def process_value(self, value, description, encoding='utf-8',
                       binarywrap=None):
         # if the dbapi module isn't supporting type codes, override to return
         # value directly
         transform = self._transformation_callback(description,
@@ -527,14 +540,20 @@
 
 class MINUTE(ExtractDateField):
     field = 'MINUTE'
 
 class SECOND(ExtractDateField):
     field = 'SECOND'
 
+class EPOCH(ExtractDateField):
+    """Return EPOCH timestamp from a datetime/date ;
+    return number of seconds for an interval.
+    """
+    field = 'EPOCH'
+
 class WEEKDAY(FunctionDescr):
     """Return the day of the week represented by the date.
 
     Sunday == 1, Saturday = 7
 
     (pick those values since that's what mysql and sqlserver do, and what's in
     the ODBC standard)
@@ -618,15 +637,15 @@
 for func_class in (
     # aggregate functions
     MIN, MAX, SUM, COUNT, AVG,
     # transformation functions
     ABS, RANDOM,
     UPPER, LOWER, SUBSTRING, LENGTH,
     DATE,
-    YEAR, MONTH, DAY, HOUR, MINUTE, SECOND, WEEKDAY, AT_TZ,
+    YEAR, MONTH, DAY, HOUR, MINUTE, SECOND, WEEKDAY, EPOCH, AT_TZ,
     # cast functions
     CAST,
     # keyword function
     IN):
     SQL_FUNCTIONS_REGISTRY.register_function(func_class())
 
 def register_function(funcdef):
@@ -747,45 +766,64 @@
 
     def system_database(self):
         """return the system database for the given driver"""
         raise NotImplementedError('not supported by this DBMS')
 
     def backup_commands(self, backupfile, keepownership=True,
                         dbname=None, dbhost=None, dbport=None, dbuser=None):
-        """return a list of commands to backup the given database.
+        """Return a list of commands to backup the given database.
 
         Each command may be given as a list or as a string. In the latter case,
         expected to be used with a subshell (for instance using `os.system(cmd)`
         or `subprocess.call(cmd, shell=True)`
         """
         raise NotImplementedError('not supported by this DBMS')
 
     def restore_commands(self, backupfile, keepownership=True, drop=True,
                          dbname=None, dbhost=None, dbport=None, dbuser=None,
                          dbencoding=None):
-        """return a list of commands to restore a backup of the given database
+        """Return a list of commands to restore a backup of the given database.
 
 
         Each command may be given as a list or as a string. In the latter case,
         expected to be used with a subshell (for instance using `os.system(cmd)`
         or `subprocess.call(cmd, shell=True)`
         """
         raise NotImplementedError('not supported by this DBMS')
 
-    # helpers to standardize SQL according to the database
+    # helpers to standardize SQL according to the database #####################
+
     def sql_current_date(self):
+        """Return sql for the current date.
+
+        Take care default implementation return date at the beginning of the
+        transaction on some backend (eg postgres)
+        """
         return 'CURRENT_DATE'
 
     def sql_current_time(self):
+        """Return sql for the current time.
+
+        Take care default implementation return time at the beginning of the
+        transaction on some backend (eg postgres)
+        """
         return 'CURRENT_TIME'
 
     def sql_current_timestamp(self):
+        """Return sql for the current date and time.
+
+        Take care default implementation return date and time at the beginning
+        of the transaction on some backend (eg postgres)
+        """
         return 'CURRENT_TIMESTAMP'
 
     def sql_concat_string(self, lhs, rhs):
+        """Return sql for concatenating given arguments (expected to be
+        evaluated as string when executing the query).
+        """
         return '%s || %s' % (lhs, rhs)
 
     def sql_regexp_match_expression(self, pattern):
         """pattern matching using regexp"""
         raise NotImplementedError('not supported by this DBMS')
 
     def sql_create_index(self, table, column, unique=False):
```

### Comparing `logilab-database-1.8.1/PKG-INFO` & `logilab-database-1.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.0
 Name: logilab-database
-Version: 1.8.1
+Version: 1.9.0
 Summary: true unified database access
 Home-page: http://www.logilab.org/project/logilab-database
 Author: Logilab
 Author-email: contact@logilab.fr
 License: LGPL
 Description: logilab-database provides some classes to make unified access to different
         RDBMS possible:
```

### Comparing `logilab-database-1.8.1/postgres.py` & `logilab-database-1.9.0/postgres.py`

 * *Files 10% similar despite different names*

```diff
@@ -88,19 +88,26 @@
 class _Psycopg2Adapter(_PsycopgAdapter):
     """Simple Psycopg2 Adapter to DBAPI (cnx_string differs from classical ones)
     """
     # not defined in psycopg2.extensions
     # "select typname from pg_type where oid=705";
     UNKNOWN = 705
     returns_unicode = True
+    # True is the backend support COPY FROM method
+    support_copy_from = True
 
     def __init__(self, native_module, pywrap=False):
         from psycopg2 import extensions
         extensions.register_type(extensions.UNICODE)
-        extensions.register_type(extensions.UNICODEARRAY)
+        try:
+            unicodearray = extensions.UNICODEARRAY
+        except AttributeError:
+            from psycopg2 import _psycopg
+            unicodearray = _psycopg.UNICODEARRAY
+        extensions.register_type(unicodearray)
         self.BOOLEAN = extensions.BOOLEAN
         db.DBAPIAdapter.__init__(self, native_module, pywrap)
         self._init_psycopg2()
 
     def _init_psycopg2(self):
         """initialize psycopg2 to use mx.DateTime for date and timestamps
         instead for datetime.datetime"""
@@ -123,14 +130,25 @@
             #    return psycopg2.Binary(stringio.getvalue())
             #import StringIO
             #extensions.register_adapter(StringIO.StringIO, adapt_stringio)
             #import cStringIO
             #extensions.register_adapter(cStringIO.StringIO, adapt_stringio)
 
 
+class _Psycopg2CtypesAdapter(_Psycopg2Adapter):
+    """psycopg2-ctypes adapter
+
+    cf. https://github.com/mvantellingen/psycopg2-ctypes
+    """
+    def __init__(self, native_module, pywrap=False):
+        # install psycopg2 compatibility
+        from psycopg2ct import compat
+        compat.register()
+        _Psycopg2Adapter.__init__(self, native_module, pywrap)
+
 class _PgsqlAdapter(db.DBAPIAdapter):
     """Simple pyPgSQL Adapter to DBAPI
     """
     def connect(self, host='', database='', user='', password='', port='', extra_args=None):
         """Handles psycopg connection format"""
         kwargs = {'host' : host, 'port': port or None,
                   'database' : database,
@@ -146,20 +164,21 @@
     def __getattr__(self, attrname):
         # __import__('pyPgSQL.PgSQL', ...) imports the toplevel package
         return getattr(self._native_module, attrname)
 
 
 db._PREFERED_DRIVERS['postgres'] = [
     #'logilab.database._pyodbcwrap',
-    'psycopg2', 'psycopg', 'pgdb', 'pyPgSQL.PgSQL',
+    'psycopg2', 'psycopg2ct', 'psycopg', 'pgdb', 'pyPgSQL.PgSQL',
     ]
 db._ADAPTER_DIRECTORY['postgres'] = {
     'pgdb' : _PgdbAdapter,
     'psycopg' : _PsycopgAdapter,
     'psycopg2' : _Psycopg2Adapter,
+    'psycopg2ct' : _Psycopg2CtypesAdapter,
     'pyPgSQL.PgSQL' : _PgsqlAdapter,
     }
 
 
 
 class _PGAdvFuncHelper(db._GenericAdvFuncHelper):
     """Postgres helper, taking advantage of postgres SEQUENCE support
@@ -215,14 +234,23 @@
         cmd.append(dbname)
         if not keepownership:
             cmd.append('--no-owner')
         cmd.append(backupfile)
         cmds.append(cmd)
         return cmds
 
+    def sql_current_date(self):
+        return 'CAST(clock_timestamp() AS DATE)'
+
+    def sql_current_time(self):
+        return 'CAST(clock_timestamp() AS TIME)'
+
+    def sql_current_timestamp(self):
+        return 'clock_timestamp()'
+
     def sql_regexp_match_expression(self, pattern):
         """pattern matching using regexp"""
         return "~ %s" % (pattern)
 
     def sql_create_sequence(self, seq_name):
         return 'CREATE SEQUENCE %s;' % seq_name
 
@@ -406,21 +434,22 @@
             self.logger.info('tsearch2.sql installed')
 
     def sql_init_fti(self):
         """Return the sql definition of table()s used by the full text index.
 
         Require extensions to be already in.
         """
-        # XXX create GIN or GIST index, see FTS wiki
         return """
 CREATE table appears(
   uid     INTEGER PRIMARY KEY NOT NULL,
   words   tsvector,
   weight  FLOAT
 );
+
+CREATE INDEX appears_words_idx ON appears USING gin(words);
 """
 
     def sql_drop_fti(self):
         """Drop tables used by the full text index."""
         return 'DROP TABLE appears;'
 
     def sql_grant_user_on_fti(self, user):
```

### Comparing `logilab-database-1.8.1/COPYING` & `logilab-database-1.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/setup.py` & `logilab-database-1.9.0/setup.py`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/ftiquery.py` & `logilab-database-1.9.0/ftiquery.py`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/ftiparser.py` & `logilab-database-1.9.0/ftiparser.py`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/sqlgen.py` & `logilab-database-1.9.0/sqlgen.py`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/ChangeLog` & `logilab-database-1.9.0/ChangeLog`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 Changelog for logilab database package
 ======================================
 
+2012-02-03  --  1.8.2
+    * don't use CURRENT_DATETIME for postgresql (#83892)
+
+    * sqlserver: sql_current_[date|timestamp] shouldn't return date[time] objects (#88279)
+
+    * process_cursor fixes (#88281)
+
+
+
 2011-12-01  --  1.8.1
     * implement db helper date manipulation helpers for sqlserver  (closes
 	#83603)
 
 
+
 2011-11-07  --  1.8.0
     * new process_cursor method (closes #77769)
 
     * new "at_tz" function to get back a timestamp at a given time-zone (closes #81267)
 
     * dropped support for posgres < 8.3 (closes #76944)
```

### Comparing `logilab-database-1.8.1/test/unittest_sqlserver2005.py` & `logilab-database-1.9.0/test/unittest_sqlserver2005.py`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/test/unittest_postgres.py` & `logilab-database-1.9.0/test/unittest_postgres.py`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/test/unittest_mysql.py` & `logilab-database-1.9.0/test/unittest_mysql.py`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/test/unittest_db.py` & `logilab-database-1.9.0/test/unittest_db.py`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/test/unittest_fti.py` & `logilab-database-1.9.0/test/unittest_fti.py`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/test/unittest_sqlite.py` & `logilab-database-1.9.0/test/unittest_sqlite.py`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/mysql.py` & `logilab-database-1.9.0/mysql.py`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/sqlserver2000.py` & `logilab-database-1.9.0/sqlserver2000.py`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/COPYING.LESSER` & `logilab-database-1.9.0/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/sqlserver2005.py` & `logilab-database-1.9.0/sqlserver2005.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,14 @@
 - pyodbc (recommended, others are not well tested)
 - adodbapi
 """
 
 import os
 import sys
 import shutil
-import datetime
 
 from logilab import database as db
 from logilab.database.sqlserver import _PyodbcAdapter, _AdodbapiAdapter
 import StringIO
 
 class _PyodbcSqlServer2005Adapter(_PyodbcAdapter):
     driver = "SQL Server Native Client 10.0"
@@ -54,20 +53,14 @@
     TYPE_MAPPING['Boolean'] =  'bit'
     TYPE_MAPPING['Date'] =     'smalldatetime'
     TYPE_MAPPING['Datetime'] = 'datetime'
     TYPE_MAPPING['Password'] = 'varbinary(255)'
     TYPE_MAPPING['Bytes'] =    'varbinary(max)'
     TYPE_MAPPING['SizeConstrainedString'] = 'nvarchar(%s)'
 
-    def sql_current_date(self):
-        return datetime.date.today()
-
-    def sql_current_timestamp(self):
-        return datetime.datetime.now()
-
     def boolean_value(self, value):
         if value:
             return 1
         else:
             return 0
 
     def list_tables(self, cursor):
```

### Comparing `logilab-database-1.8.1/sqlserver.py` & `logilab-database-1.9.0/sqlserver.py`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/sqlite.py` & `logilab-database-1.9.0/sqlite.py`

 * *Files 2% similar despite different names*

```diff
@@ -186,30 +186,19 @@
         def _transform(value):
             if binarywrap is not None and isinstance(value, self._native_module.Binary):
                 return binarywrap(value)
             return value # no type code support, can't do anything
         return _transform
 
 
-class _SqliteAdapter(db.DBAPIAdapter):
-    """Simple sqlite Adapter to DBAPI
-    """
-    def __init__(self, native_module, pywrap=False):
-        db.DBAPIAdapter.__init__(self, native_module, pywrap)
-        self.DATETIME = native_module.TIMESTAMP
-
-    def connect(self, host='', database='', user='', password='', port='', extra_args=None):
-        """Handles sqlite connection format"""
-        return self._wrap_if_needed(self._native_module.connect(database))
-
-
-db._PREFERED_DRIVERS['sqlite'] = ['pysqlite2.dbapi2', 'sqlite', 'sqlite3']
+db._PREFERED_DRIVERS['sqlite'] = [
+    'pysqlite2.dbapi2',
+    'sqlite3']
 db._ADAPTER_DIRECTORY['sqlite'] = {
     'pysqlite2.dbapi2' : _PySqlite2Adapter,
-    'sqlite' : _SqliteAdapter,
     'sqlite3' : _PySqlite2Adapter,
     }
 
 
 class _SqliteAdvFuncHelper(db._GenericAdvFuncHelper):
     """Generic helper, trying to provide generic way to implement
     specific functionalities from others DBMS
```

### Comparing `logilab-database-1.8.1/fti.py` & `logilab-database-1.9.0/fti.py`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/sqlserver2008.py` & `logilab-database-1.9.0/sqlserver2008.py`

 * *Files identical despite different names*

### Comparing `logilab-database-1.8.1/__pkginfo__.py` & `logilab-database-1.9.0/__pkginfo__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# copyright 2003-2011 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
+# copyright 2003-2012 LOGILAB S.A. (Paris, FRANCE), all rights reserved.
 # contact http://www.logilab.fr/ -- mailto:contact@logilab.fr
 #
 # This file is part of logilab-database.
 #
 # logilab-database is free software: you can redistribute it and/or modify it
 # under the terms of the GNU Lesser General Public License as published by the
 # Free Software Foundation, either version 2.1 of the License, or (at your
@@ -15,15 +15,15 @@
 #
 # You should have received a copy of the GNU Lesser General Public License along
 # with logilab-database. If not, see <http://www.gnu.org/licenses/>.
 """logilab.database packaging information."""
 
 distname = 'logilab-database'
 modname = 'database'
-numversion = (1, 8, 1)
+numversion = (1, 9, 0)
 version = '.'.join([str(num) for num in numversion])
 license = 'LGPL'
 
 author = "Logilab"
 author_email = "contact@logilab.fr"
 
 description = "true unified database access"
```

