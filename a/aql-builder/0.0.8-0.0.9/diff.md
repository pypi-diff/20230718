# Comparing `tmp/aql-builder-0.0.8.tar.gz` & `tmp/aql-builder-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aql-builder-0.0.8.tar", last modified: Fri Jul 14 00:47:03 2023, max compression
+gzip compressed data, was "aql-builder-0.0.9.tar", last modified: Fri Jul 14 06:07:40 2023, max compression
```

## Comparing `aql-builder-0.0.8.tar` & `aql-builder-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:47:03.957038 aql-builder-0.0.8/
--rw-rw-rw-   0 root         (0) root         (0)    11341 2022-12-20 01:01:18.000000 aql-builder-0.0.8/LICENSE.txt
--rw-r--r--   0 root         (0) root         (0)     4286 2023-07-14 00:47:03.957038 aql-builder-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     3375 2023-07-14 00:36:37.000000 aql-builder-0.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:47:03.949038 aql-builder-0.0.8/aql_builder/
--rw-rw-rw-   0 root         (0) root         (0)     2995 2023-07-14 00:46:02.000000 aql-builder-0.0.8/aql_builder/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5676 2022-12-20 01:01:18.000000 aql-builder-0.0.8/aql_builder/assumptions.py
--rw-rw-rw-   0 root         (0) root         (0)       33 2022-12-20 01:01:18.000000 aql-builder-0.0.8/aql_builder/errors.py
--rw-rw-rw-   0 root         (0) root         (0)    33324 2023-07-14 00:36:37.000000 aql-builder-0.0.8/aql_builder/types.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:47:03.957038 aql-builder-0.0.8/aql_builder.egg-info/
--rw-r--r--   0 root         (0) root         (0)     4286 2023-07-14 00:47:03.000000 aql-builder-0.0.8/aql_builder.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      320 2023-07-14 00:47:03.000000 aql-builder-0.0.8/aql_builder.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 00:47:03.000000 aql-builder-0.0.8/aql_builder.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       29 2023-07-14 00:47:03.000000 aql-builder-0.0.8/aql_builder.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2023-07-14 00:47:03.000000 aql-builder-0.0.8/aql_builder.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 00:47:03.957038 aql-builder-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1156 2023-07-11 03:33:38.000000 aql-builder-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 00:47:03.957038 aql-builder-0.0.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)    31682 2023-07-14 00:36:37.000000 aql-builder-0.0.8/tests/test_builder.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 06:07:40.628640 aql-builder-0.0.9/
+-rw-rw-rw-   0 root         (0) root         (0)    11341 2022-12-20 01:01:18.000000 aql-builder-0.0.9/LICENSE.txt
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-07-14 06:07:40.628640 aql-builder-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     3375 2023-07-14 00:36:37.000000 aql-builder-0.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 06:07:40.624640 aql-builder-0.0.9/aql_builder/
+-rw-rw-rw-   0 root         (0) root         (0)     2995 2023-07-14 06:03:33.000000 aql-builder-0.0.9/aql_builder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5676 2022-12-20 01:01:18.000000 aql-builder-0.0.9/aql_builder/assumptions.py
+-rw-rw-rw-   0 root         (0) root         (0)       33 2022-12-20 01:01:18.000000 aql-builder-0.0.9/aql_builder/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)    33591 2023-07-14 05:54:23.000000 aql-builder-0.0.9/aql_builder/types.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 06:07:40.628640 aql-builder-0.0.9/aql_builder.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4286 2023-07-14 06:07:40.000000 aql-builder-0.0.9/aql_builder.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      320 2023-07-14 06:07:40.000000 aql-builder-0.0.9/aql_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-14 06:07:40.000000 aql-builder-0.0.9/aql_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2023-07-14 06:07:40.000000 aql-builder-0.0.9/aql_builder.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2023-07-14 06:07:40.000000 aql-builder-0.0.9/aql_builder.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-07-14 06:07:40.628640 aql-builder-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1131 2023-07-14 05:54:23.000000 aql-builder-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-14 06:07:40.628640 aql-builder-0.0.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    32191 2023-07-14 05:54:23.000000 aql-builder-0.0.9/tests/test_builder.py
```

### Comparing `aql-builder-0.0.8/LICENSE.txt` & `aql-builder-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aql-builder-0.0.8/PKG-INFO` & `aql-builder-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aql-builder
-Version: 0.0.8
+Version: 0.0.9
 Summary: ArangoDB AQL builder
 Home-page: https://foss.heptapod.net/aquapenguin/aql-builder
 Maintainer: Aqua Penguin
 Maintainer-email: aqua.penguin.34@gmail.com
 Project-URL: Source, https://foss.heptapod.net/aquapenguin/aql-builder
 Project-URL: Tracker, https://foss.heptapod.net/aquapenguin/aql-builder/-/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aql-builder-0.0.8/README.md` & `aql-builder-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `aql-builder-0.0.8/aql_builder/__init__.py` & `aql-builder-0.0.9/aql_builder/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from aql_builder import types
 
 # pylint: disable=protected-access
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 
 
 class _AQLBuilderMeta(type):
 
 	def __call__(cls, obj=None):
 		return types.auto_cast_token(obj)
```

### Comparing `aql-builder-0.0.8/aql_builder/assumptions.py` & `aql-builder-0.0.9/aql_builder/assumptions.py`

 * *Files identical despite different names*

### Comparing `aql-builder-0.0.8/aql_builder/types.py` & `aql-builder-0.0.9/aql_builder/types.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,30 @@
 import json
 import math
 import re
 from math import inf
 from numbers import Number
 from typing import Optional
 
-from arango.collection import Collection as ArangoCollection  # type: ignore
-
 from .assumptions import builtins as functions
 from .assumptions import keywords, keywords_not_reserved
 from .errors import AqlError
 
 # pylint: disable=too-many-lines
 
 
+def _seems_arango_collection(obj):
+	# Introspect the object to avoid having an external dependency.
+	# Do not use hasattr() because it return always True
+	# on others expressions, due to the wrapper for the
+	# functions on the AQLBuilder.
+	attrs = set(dir(obj))
+	return "statuses" in attrs and "delete_index" in attrs and "name" in attrs
+
+
 def flat_list(*args):
 	vals = []
 	for arg in args:
 		if isinstance(arg, (list, tuple)):
 			vals.extend(flat_list(*arg))
 		else:
 			vals.append(arg)
@@ -58,15 +65,15 @@
 		return RangeExpression(match.group(1), match.group(2))
 	if Identifier.match(string):
 		return Identifier(string)
 	return SimpleReference(string)
 
 
 def cast_object(obj):
-	if isinstance(obj, ArangoCollection):
+	if _seems_arango_collection(obj):
 		return Identifier(obj.name)
 	if isinstance(obj, list):
 		return ListLiteral(obj)
 	return ObjectLiteral(obj)
 
 
 def auto_cast_token(token):
@@ -76,15 +83,15 @@
 		return token
 	if isinstance(token, bool):
 		return cast_boolean(token)
 	if isinstance(token, Number):
 		return cast_number(token)
 	if isinstance(token, str):
 		return cast_string(token)
-	if isinstance(token, (ArangoCollection, list, dict)):
+	if isinstance(token, (list, dict)) or _seems_arango_collection(token):
 		return cast_object(token)
 	raise AqlError(f"Invalid AQL value: ({type(token)}) {token}")
 
 
 class _Definitions:
 
 	__slots__ = ["_dfns"]
@@ -415,15 +422,15 @@
 class Identifier(_Expression):
 	_pattern = re.compile(r"^[_@a-z][-_@0-9a-z]*$", flags=re.RegexFlag.IGNORECASE)
 
 	__slots__ = ["_value"]
 
 	def __init__(self, value):
 		super().__init__()
-		if isinstance(value, ArangoCollection):
+		if _seems_arango_collection(value):
 			value = value.name
 		if isinstance(value, Identifier):
 			value = value._value
 		if value is None or not isinstance(value, str):
 			raise AqlError(f"Expected value to be a string: {repr(value)}")
 		if not self.match(value):
 			raise AqlError(f"Not a valid identifier: {value}")
@@ -445,15 +452,15 @@
 		flags=re.RegexFlag.IGNORECASE
 	)
 
 	__slots__ = ["_value"]
 
 	def __init__(self, value):
 		super().__init__()
-		if isinstance(value, ArangoCollection):
+		if _seems_arango_collection(value):
 			value = value.name
 		if isinstance(value, SimpleReference):
 			value = value._value
 		if value is None or not isinstance(value, str):
 			raise AqlError(f"Expected value to be a string: {repr(value)}")
 		if not self.match(value):
 			raise AqlError(f"Not a valid simple reference: {value}")
```

### Comparing `aql-builder-0.0.8/aql_builder.egg-info/PKG-INFO` & `aql-builder-0.0.9/aql_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aql-builder
-Version: 0.0.8
+Version: 0.0.9
 Summary: ArangoDB AQL builder
 Home-page: https://foss.heptapod.net/aquapenguin/aql-builder
 Maintainer: Aqua Penguin
 Maintainer-email: aqua.penguin.34@gmail.com
 Project-URL: Source, https://foss.heptapod.net/aquapenguin/aql-builder
 Project-URL: Tracker, https://foss.heptapod.net/aquapenguin/aql-builder/-/issues
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `aql-builder-0.0.8/setup.py` & `aql-builder-0.0.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import os
 
 from setuptools import find_packages, setup
 
 install_requires = [
-	"pip>=21",
-	"python-arango>=6.0.0"
+	"pip>=21"
 ]
 
 setup(
 	name='aql-builder',
 	version=__import__('aql_builder').__version__,
 	python_requires='>=3.7',
 	url='https://foss.heptapod.net/aquapenguin/aql-builder',
```

### Comparing `aql-builder-0.0.8/tests/test_builder.py` & `aql-builder-0.0.9/tests/test_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,43 @@
 import unittest
 
-from arango.collection import Collection
-
 from aql_builder import AQLBuilder as AB
 from aql_builder import types
 from aql_builder.errors import AqlError
 
 
+class _FakeArangoCollection:
+	statuses = {
+		1: "new",
+		2: "unloaded",
+		3: "loaded",
+		4: "unloading",
+		5: "deleted",
+		6: "loading",
+	}
+
+	def __init__(self, name: str) -> None:
+		self._name = name
+
+	def delete_index(self):
+		pass
+
+	@property
+	def name(self) -> str:
+		return self._name
+
+
+class AQLBuilderFakeArangoCollectionTest(unittest.TestCase):
+
+	def test_instance_is_detected(self):
+		obj = _FakeArangoCollection('test')
+		self.assertTrue(types._seems_arango_collection(obj))
+		self.assertFalse(types._seems_arango_collection(AB.str("test")))
+
+
 class AQLBuilderCastTest(unittest.TestCase):
 
 	def _test_auto_cast(self, token, should):
 		self.assertIsInstance(types.auto_cast_token(token), should)
 
 	def test_cast_none(self):
 		self._test_auto_cast(None, types.NullLiteral)
@@ -33,15 +60,15 @@
 		self._test_auto_cast('5.5', types.NumberLiteral)
 		self._test_auto_cast('"abcd"', types.StringLiteral)
 		self._test_auto_cast('5..10', types.RangeExpression)
 		self._test_auto_cast('filter', types.Identifier)
 		self._test_auto_cast('abcd.efgh', types.SimpleReference)
 
 	def test_cast_obj(self):
-		self._test_auto_cast(Collection(None, None, 'abcd'), types.Identifier)
+		self._test_auto_cast(_FakeArangoCollection('abcd'), types.Identifier)
 		self._test_auto_cast([1,2,3,4], types.ListLiteral)
 		self._test_auto_cast({'1': 2, '3': 4}, types.ObjectLiteral)
 
 
 class AQLBuilderStaticsTest(unittest.TestCase):
 
 	def _test_static(self, ab, should):
@@ -129,21 +156,21 @@
 	def test_static_range(self):
 		self._test_static(AB.range(10, 20), '10..20')
 		self._test_static(AB.range('10', '20'), '10..20')
 
 	def test_static_ref(self):
 		self._test_static(AB.ref('abcd'), 'abcd')
 		self._test_static(AB.ref('abcd.efgh'), 'abcd.efgh')
-		self._test_static(AB.ref(Collection(None, None, 'abcd')), 'abcd')
+		self._test_static(AB.ref(_FakeArangoCollection('abcd')), 'abcd')
 		self._test_static(AB.ref(types.SimpleReference('abcd')), 'abcd')
 
 	def test_static_for(self):
 		self._test_static(AB.for_('abcd').in_('efgh'), 'FOR abcd IN efgh')
 		self._test_static(AB.for_('ab-cd').in_('ef-gh'), 'FOR `ab-cd` IN `ef-gh`')
-		self._test_static(AB.for_(Collection(None, None, 'abcd')).in_('efgh'), 'FOR abcd IN efgh')
+		self._test_static(AB.for_(_FakeArangoCollection('abcd')).in_('efgh'), 'FOR abcd IN efgh')
 		self._test_static(
 			AB.for_('abcd').in_('efgh').options({'ijkl': 'mnop'}),
 			'FOR abcd IN efgh OPTIONS {"ijkl": mnop}'
 		)
 
 	def test_static_filter(self):
 		self._test_static(AB.filter('abcd'), 'FILTER abcd')
```

