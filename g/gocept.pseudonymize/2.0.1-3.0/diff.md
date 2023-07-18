# Comparing `tmp/gocept.pseudonymize-2.0.1.tar.gz` & `tmp/gocept.pseudonymize-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gocept.pseudonymize-2.0.1.tar", last modified: Wed Mar 22 08:36:40 2017, max compression
+gzip compressed data, was "gocept.pseudonymize-3.0.tar", last modified: Tue Jul 18 05:43:59 2023, max compression
```

## Comparing `gocept.pseudonymize-2.0.1.tar` & `gocept.pseudonymize-3.0.tar`

### file list

```diff
@@ -1,26 +1,25 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2017-03-22 08:36:40.000000 gocept.pseudonymize-2.0.1/
--rw-r--r--   0 mac        (501) staff       (20)     2749 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/CHANGES.rst
--rw-r--r--   0 mac        (501) staff       (20)      682 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/HACKING.rst
--rw-r--r--   0 mac        (501) staff       (20)     1065 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)    10198 2017-03-22 08:36:40.000000 gocept.pseudonymize-2.0.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     3353 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/README.rst
--rw-r--r--   0 mac        (501) staff       (20)       59 2017-03-22 08:36:40.000000 gocept.pseudonymize-2.0.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     2055 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2017-03-22 08:36:40.000000 gocept.pseudonymize-2.0.1/src/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2017-03-22 08:36:40.000000 gocept.pseudonymize-2.0.1/src/gocept/
--rw-r--r--   0 mac        (501) staff       (20)       56 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/src/gocept/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2017-03-22 08:36:40.000000 gocept.pseudonymize-2.0.1/src/gocept/pseudonymize/
--rw-r--r--   0 mac        (501) staff       (20)      262 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/src/gocept/pseudonymize/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     6317 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/src/gocept/pseudonymize/pseudonymize.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2017-03-22 08:36:40.000000 gocept.pseudonymize-2.0.1/src/gocept/pseudonymize/tests/
--rw-r--r--   0 mac        (501) staff       (20)        0 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/src/gocept/pseudonymize/tests/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     7726 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/src/gocept/pseudonymize/tests/test_pseudonymize.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2017-03-22 08:36:40.000000 gocept.pseudonymize-2.0.1/src/gocept.pseudonymize.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)        1 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/src/gocept.pseudonymize.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)       20 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/src/gocept.pseudonymize.egg-info/entry_points.txt
--rw-r--r--   0 mac        (501) staff       (20)        7 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/src/gocept.pseudonymize.egg-info/namespace_packages.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/src/gocept.pseudonymize.egg-info/not-zip-safe
--rw-r--r--   0 mac        (501) staff       (20)    10198 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/src/gocept.pseudonymize.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)       24 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/src/gocept.pseudonymize.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)      633 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/src/gocept.pseudonymize.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        7 2017-03-22 08:36:39.000000 gocept.pseudonymize-2.0.1/src/gocept.pseudonymize.egg-info/top_level.txt
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:43:59.697018 gocept.pseudonymize-3.0/
+-rw-r--r--   0 mac        (513) staff       (20)     2991 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      686 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/HACKING.rst
+-rw-r--r--   0 mac        (513) staff       (20)     1071 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/LICENSE.txt
+-rw-r--r--   0 mac        (513) staff       (20)     8894 2023-07-18 05:43:59.697161 gocept.pseudonymize-3.0/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)     3973 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      213 2023-07-18 05:43:59.697669 gocept.pseudonymize-3.0/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     2177 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:43:59.690494 gocept.pseudonymize-3.0/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:43:59.693101 gocept.pseudonymize-3.0/src/gocept/
+-rw-r--r--   0 mac        (513) staff       (20)       56 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/src/gocept/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:43:59.696090 gocept.pseudonymize-3.0/src/gocept/pseudonymize/
+-rw-r--r--   0 mac        (513) staff       (20)     1118 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/src/gocept/pseudonymize/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     6305 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/src/gocept/pseudonymize/pseudonymize.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:43:59.696718 gocept.pseudonymize-3.0/src/gocept/pseudonymize/tests/
+-rw-r--r--   0 mac        (513) staff       (20)        0 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/src/gocept/pseudonymize/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)     7922 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/src/gocept/pseudonymize/tests/test_pseudonymize.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-07-18 05:43:59.695442 gocept.pseudonymize-3.0/src/gocept.pseudonymize.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)     8894 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/src/gocept.pseudonymize.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      593 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/src/gocept.pseudonymize.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/src/gocept.pseudonymize.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)        7 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/src/gocept.pseudonymize.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/src/gocept.pseudonymize.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)       24 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/src/gocept.pseudonymize.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        7 2023-07-18 05:43:59.000000 gocept.pseudonymize-3.0/src/gocept.pseudonymize.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gocept.pseudonymize-2.0.1/CHANGES.rst` & `gocept.pseudonymize-3.0/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,11 +1,22 @@
 ==========
 Change log
 ==========
 
+3.0 (2023-07-18)
+================
+
+- Drop support for Python 2.7, 3.3, 3.4, 3.5, 3.6.
+
+- Add support for Python 3.7, 3.8, 3.9, 3.10, 3.11.
+
+- Drop support for PyPy implementation. The ``crypt`` module is currently not
+  working with PyPy3.
+
+
 2.0.1 (2017-03-22)
 ==================
 
 - Fix ``phone()`` so it does not break if the input is only one character long.
   (https://bitbucket.org/gocept/gocept.pseudonymize/issues/1)
```

### Comparing `gocept.pseudonymize-2.0.1/HACKING.rst` & `gocept.pseudonymize-3.0/HACKING.rst`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,14 @@
 :Online documentation:
     http://pythonhosted.org/gocept.pseudonymize/
 
 :PyPI page:
     http://pypi.python.org/pypi/gocept.pseudonymize/
 
 :Issues:
-    https://bitbucket.org/gocept/gocept.pseudonymize/issues
+    https://github.com/gocept/gocept.pseudonymize/issues
 
 :Source code:
-    https://bitbucket.org/gocept/gocept.pseudonymize/
+    https://github.com/gocept/gocept.pseudonymize
 
 :Current change log:
-    https://bitbucket.org/gocept/gocept.pseudonymize/raw/tip/CHANGES.txt
+    https://raw.githubusercontent.com/gocept/gocept.pseudonymize/master/CHANGES.rst
```

### Comparing `gocept.pseudonymize-2.0.1/LICENSE.txt` & `gocept.pseudonymize-3.0/LICENSE.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2013-2017 gocept gmbh & co. kg
+Copyright 2013-2021, 2020 gocept gmbh & co. kg
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
 
 The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `gocept.pseudonymize-2.0.1/README.rst` & `gocept.pseudonymize-3.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,24 @@
 ===================
 gocept.pseudonymize
 ===================
 
+.. image:: https://img.shields.io/pypi/v/gocept.pseudonymize.svg
+    :target: https://pypi.org/project/gocept.pseudonymize/
+
+.. image:: https://img.shields.io/pypi/pyversions/gocept.pseudonymize.svg
+    :target: https://pypi.org/project/gocept.pseudonymize/
+
+.. image:: https://github.com/gocept/gocept.pseudonymize/workflows/tests/badge.svg
+    :target: https://github.com/gocept/gocept.pseudonymize/actions?query=workflow%3Atests
+
+.. image:: https://coveralls.io/repos/github/gocept/gocept.pseudonymize/badge.svg?branch=master
+    :target: https://coveralls.io/github/gocept/gocept.pseudonymize?branch=master
+
+
 This package provides helper functions to pseudonymize data like text,
 integers, email addresses or license tags.
 
 It uses the ``crypt.crypt()`` function for pseudonymization, which means,
 longer text blocks require multiple ``crypt.crypt()`` calls.
 
 
@@ -25,15 +38,15 @@
     'u7YJWz RqdYkfNUFgZii2Y'
 
 The result has always the same string length as the input. But there is no
 guaranty that it is still valid in the domain of the input value. For
 example the checksum of the pseudonymized IBAN is not correct.
 
 
-This package is tested to be compatible with Python version 2.7 and 3.3.
+This package is tested to be compatible with Python version 2.7, 3.5 up to 3.8.
 
 
 Detailed usage examples
 =======================
 
 There are different pseudonymization function because it is not always
 possible to guess the correct one by looking at the input data.
```

### Comparing `gocept.pseudonymize-2.0.1/setup.py` & `gocept.pseudonymize-3.0/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,28 +1,29 @@
-# Copyright (c) 2013-2017 gocept gmbh & co. kg
+# Copyright (c) 2013-2023 gocept gmbh & co. kg
 # See also LICENSE.txt
 
 # This should be only one line. If it must be multi-line, indent the second
 # line onwards to keep the PKG-INFO file format intact.
 """Pseudonymize data like text, email addresses or license tags.
 """
 
-from setuptools import setup, find_packages
+from setuptools import find_packages
+from setuptools import setup
 
 
 def read(name):
     """Read a file."""
     with open(name) as f:
         return f.read()
 
 
 setup(
     name='gocept.pseudonymize',
-    version='2.0.1',
-
+    version='3.0',
+    python_requires='>=3.7',
     install_requires=[
         'setuptools',
     ],
 
     extras_require={
         'test': [
             'mock',
@@ -34,38 +35,36 @@
             # 'binary-name = gocept.pseudonymize.module:function'
         ],
     },
 
     author='gocept <mail@gocept.com>',
     author_email='mail@gocept.com',
     license='MIT',
-    url='https://bitbucket.org/gocept/gocept.pseudonymize/',
+    url='https://github.com/gocept/gocept.pseudonymize',
 
     keywords='Pseudonymization',
-    classifiers="""\
-Development Status :: 5 - Production/Stable
-Intended Audience :: Developers
-Intended Audience :: System Administrators
-Operating System :: OS Independent
-Topic :: Security :: Cryptography
-Topic :: Software Development :: Libraries :: Python Modules
-Topic :: Text Processing :: Filters
-Topic :: Utilities
-License :: OSI Approved :: MIT License
-Natural Language :: German
-Programming Language :: Python :: 2
-Programming Language :: Python :: 2.7
-Programming Language :: Python :: 3
-Programming Language :: Python :: 3.3
-Programming Language :: Python :: 3.4
-Programming Language :: Python :: 3.5
-Programming Language :: Python :: 3.6
-Programming Language :: Python :: Implementation :: CPython
-Programming Language :: Python :: Implementation :: PyPy
-"""[:-1].split('\n'),
+    classifiers=[
+        'Development Status :: 5 - Production/Stable',
+        'Intended Audience :: Developers',
+        'Intended Audience :: System Administrators',
+        'Operating System :: OS Independent',
+        'Topic :: Security :: Cryptography',
+        'Topic :: Software Development :: Libraries :: Python Modules',
+        'Topic :: Text Processing :: Filters',
+        'Topic :: Utilities',
+        'License :: OSI Approved :: MIT License',
+        'Natural Language :: German',
+        'Programming Language :: Python :: 3',
+        'Programming Language :: Python :: 3.7',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: Implementation :: CPython',
+    ],
     description=__doc__.strip(),
     long_description='\n\n'.join([
         '.. contents::',
         read('README.rst'),
         read('HACKING.rst'),
         read('CHANGES.rst'),
     ]),
```

### Comparing `gocept.pseudonymize-2.0.1/src/gocept/pseudonymize/pseudonymize.py` & `gocept.pseudonymize-3.0/src/gocept/pseudonymize/pseudonymize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-# -*- coding: utf-8 -*-
 # Copyright (c) 2013 gocept gmbh & co. kg
 # See also LICENSE.txt
 
 from decimal import Decimal
 import crypt
 import datetime
 
@@ -83,17 +82,17 @@
 
 
 def email(value, secret, size=None):
     """Return something what could be an e-mail address."""
     if not value:
         return value
     local, at, domain = value.partition('@')
-    return '%s%s%s.de' % (string(local, secret, len(local)).lower(),
-                          at,
-                          string(domain, secret, len(domain) - 3).lower())
+    return '{}{}{}.de'.format(string(local, secret, len(local)).lower(),
+                              at,
+                              string(domain, secret, len(domain) - 3).lower())
 
 
 def iban(value, secret, size=None):
     if not value:
         return value
     return 'DE%s' % str(integer(value[2:], secret, len(value)))[:20]
```

### Comparing `gocept.pseudonymize-2.0.1/src/gocept/pseudonymize/tests/test_pseudonymize.py` & `gocept.pseudonymize-3.0/src/gocept/pseudonymize/tests/test_pseudonymize.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,19 @@
-# -*- coding: utf-8 -*-
+from unittest import mock
+import doctest
 import gocept.pseudonymize
-import mock
 import pytest
 
 
+def test_suite():
+    """Test doctest as unittest."""
+    # This should help with https://github.com/pytest-dev/pytest/issues/1862
+    return doctest.DocFileSuite('../../../../README.rst')
+
+
 def pseudo(value, pseudonymizer, secret=None, length=None, **kw):
     secret = 'ML' if secret is None else secret
     if isinstance(value, str):
         length = len(value) if length is None else length
     return pseudonymizer(value, secret, length, **kw)
 
 
@@ -168,24 +174,24 @@
     from decimal import Decimal
     from gocept.pseudonymize import decimal as p
     assert Decimal('47.9010') == pseudo(Decimal('12.3456'), p)
     assert Decimal('-8799.11') == pseudo(Decimal('-123.45'), p)
 
 
 def test_time():
-    from gocept.pseudonymize import time as pseudo_time
     from datetime import time
+    from gocept.pseudonymize import time as pseudo_time
     assert time(16, 36, 37) == pseudo(time(12, 34, 56), pseudo_time)
     assert time(11, 46, 49) == pseudo(time(23, 59, 59), pseudo_time)
     assert time(17, 10, 21) == pseudo(time(1, 1, 0), pseudo_time)
 
 
 def test_date():
-    from gocept.pseudonymize import date as p
     from datetime import date
+    from gocept.pseudonymize import date as p
     assert date(7676, 1, 25) == pseudo(date(1983, 1, 11), p)
 
 
 def test_pseudonymize__day__1():
     """It makes sure that the pseudonymized day is not bigger than 28."""
     from gocept.pseudonymize import day
     assert 19 == pseudo(10, day)
```

### Comparing `gocept.pseudonymize-2.0.1/src/gocept.pseudonymize.egg-info/SOURCES.txt` & `gocept.pseudonymize-3.0/src/gocept.pseudonymize.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 CHANGES.rst
 HACKING.rst
 LICENSE.txt
 README.rst
+setup.cfg
 setup.py
 src/gocept/__init__.py
 src/gocept.pseudonymize.egg-info/PKG-INFO
 src/gocept.pseudonymize.egg-info/SOURCES.txt
 src/gocept.pseudonymize.egg-info/dependency_links.txt
-src/gocept.pseudonymize.egg-info/entry_points.txt
 src/gocept.pseudonymize.egg-info/namespace_packages.txt
 src/gocept.pseudonymize.egg-info/not-zip-safe
 src/gocept.pseudonymize.egg-info/requires.txt
 src/gocept.pseudonymize.egg-info/top_level.txt
 src/gocept/pseudonymize/__init__.py
 src/gocept/pseudonymize/pseudonymize.py
 src/gocept/pseudonymize/tests/__init__.py
```

