# Comparing `tmp/tkapi-0.9.7.tar.gz` & `tmp/tkapi-0.9.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkapi-0.9.7.tar", last modified: Sat Jul  8 13:37:15 2023, max compression
+gzip compressed data, was "tkapi-0.9.8.tar", last modified: Tue Jul 18 17:36:03 2023, max compression
```

## Comparing `tkapi-0.9.7.tar` & `tkapi-0.9.8.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2023-07-08 13:37:15.977025 tkapi-0.9.7/
--rw-rw-r--   0 bart      (1000) bart      (1000)     1089 2023-07-04 18:25:05.000000 tkapi-0.9.7/LICENSE.md
--rw-rw-r--   0 bart      (1000) bart      (1000)     3892 2023-07-08 13:37:15.977025 tkapi-0.9.7/PKG-INFO
--rw-rw-r--   0 bart      (1000) bart      (1000)     3416 2023-07-04 18:43:30.000000 tkapi-0.9.7/README.md
--rw-rw-r--   0 bart      (1000) bart      (1000)       38 2023-07-08 13:37:15.977025 tkapi-0.9.7/setup.cfg
--rw-rw-r--   0 bart      (1000) bart      (1000)      790 2023-07-08 13:30:26.000000 tkapi-0.9.7/setup.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2023-07-08 13:37:15.973025 tkapi-0.9.7/tests/
--rw-rw-r--   0 bart      (1000) bart      (1000)     5251 2023-07-04 19:08:18.000000 tkapi-0.9.7/tests/test_activiteit.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      908 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_agendapunt.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      544 2023-07-04 19:18:37.000000 tkapi-0.9.7/tests/test_api.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2786 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_besluit.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    10543 2023-07-04 19:50:01.000000 tkapi-0.9.7/tests/test_commissie.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8527 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_document.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     7735 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_dossier.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      628 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_filter.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     5067 2023-07-04 19:45:35.000000 tkapi-0.9.7/tests/test_fractie.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     4298 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_kamervraag.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2515 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_metadata.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1743 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_order.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    10095 2023-07-04 19:04:13.000000 tkapi-0.9.7/tests/test_persoon.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     4826 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_stemming.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     5688 2023-07-04 19:42:49.000000 tkapi-0.9.7/tests/test_util.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2023 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_vergadering.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1542 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_verslag.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8328 2023-07-04 18:25:05.000000 tkapi-0.9.7/tests/test_zaak.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2023-07-08 13:37:15.977025 tkapi-0.9.7/tkapi/
--rw-rw-r--   0 bart      (1000) bart      (1000)       25 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     7420 2023-07-04 18:32:51.000000 tkapi-0.9.7/tkapi/activiteit.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1808 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/agendapunt.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1779 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/besluit.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     6452 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/commissie.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     5390 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/core.py
--rw-rw-r--   0 bart      (1000) bart      (1000)    12973 2023-07-04 18:47:45.000000 tkapi-0.9.7/tkapi/document.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1951 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/dossier.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     3193 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/filter.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     5852 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/fractie.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      723 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/info.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1175 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/kamervraag.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      845 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/order.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8757 2023-07-04 19:03:47.000000 tkapi-0.9.7/tkapi/persoon.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2010 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/stemming.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     8500 2023-07-04 19:42:02.000000 tkapi-0.9.7/tkapi/tkapi.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2023-07-08 13:37:15.977025 tkapi-0.9.7/tkapi/util/
--rw-rw-r--   0 bart      (1000) bart      (1000)        0 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/util/__init__.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     2431 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/util/document.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     6653 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/util/queries.py
--rw-rw-r--   0 bart      (1000) bart      (1000)      766 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/util/util.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1929 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/vergadering.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     1146 2023-07-04 18:25:05.000000 tkapi-0.9.7/tkapi/verslag.py
--rw-rw-r--   0 bart      (1000) bart      (1000)     9224 2023-07-04 18:55:53.000000 tkapi-0.9.7/tkapi/zaak.py
-drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2023-07-08 13:37:15.977025 tkapi-0.9.7/tkapi.egg-info/
--rw-rw-r--   0 bart      (1000) bart      (1000)     3892 2023-07-08 13:37:15.000000 tkapi-0.9.7/tkapi.egg-info/PKG-INFO
--rw-rw-r--   0 bart      (1000) bart      (1000)      988 2023-07-08 13:37:15.000000 tkapi-0.9.7/tkapi.egg-info/SOURCES.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        1 2023-07-08 13:37:15.000000 tkapi-0.9.7/tkapi.egg-info/dependency_links.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)       38 2023-07-08 13:37:15.000000 tkapi-0.9.7/tkapi.egg-info/requires.txt
--rw-rw-r--   0 bart      (1000) bart      (1000)        6 2023-07-08 13:37:15.000000 tkapi-0.9.7/tkapi.egg-info/top_level.txt
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2023-07-18 17:36:03.474095 tkapi-0.9.8/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1089 2018-04-06 12:01:44.000000 tkapi-0.9.8/LICENSE.md
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3981 2023-07-18 17:36:03.474095 tkapi-0.9.8/PKG-INFO
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3505 2023-07-18 15:51:51.000000 tkapi-0.9.8/README.md
+-rw-rw-r--   0 bart      (1000) bart      (1000)       38 2023-07-18 17:36:03.474095 tkapi-0.9.8/setup.cfg
+-rw-rw-r--   0 bart      (1000) bart      (1000)      790 2023-07-18 17:31:32.000000 tkapi-0.9.8/setup.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2023-07-18 17:36:03.470095 tkapi-0.9.8/tests/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5989 2023-07-18 17:18:24.000000 tkapi-0.9.8/tests/test_activiteit.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      908 2019-12-20 15:26:25.000000 tkapi-0.9.8/tests/test_agendapunt.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      544 2019-09-27 22:31:06.000000 tkapi-0.9.8/tests/test_api.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2786 2019-11-29 16:10:59.000000 tkapi-0.9.8/tests/test_besluit.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    10543 2023-07-18 15:51:51.000000 tkapi-0.9.8/tests/test_commissie.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     8527 2019-12-22 14:03:25.000000 tkapi-0.9.8/tests/test_document.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     7735 2019-12-22 14:11:05.000000 tkapi-0.9.8/tests/test_dossier.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      628 2019-07-05 09:28:47.000000 tkapi-0.9.8/tests/test_filter.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5067 2023-07-18 15:51:51.000000 tkapi-0.9.8/tests/test_fractie.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4298 2019-12-22 13:52:57.000000 tkapi-0.9.8/tests/test_kamervraag.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2515 2019-12-05 20:47:06.000000 tkapi-0.9.8/tests/test_metadata.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1743 2019-07-05 13:20:18.000000 tkapi-0.9.8/tests/test_order.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    10095 2023-07-18 15:51:51.000000 tkapi-0.9.8/tests/test_persoon.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     4826 2019-09-27 17:43:37.000000 tkapi-0.9.8/tests/test_stemming.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5688 2023-07-18 15:51:51.000000 tkapi-0.9.8/tests/test_util.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2023 2023-07-18 15:51:51.000000 tkapi-0.9.8/tests/test_vergadering.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1542 2019-09-27 20:16:24.000000 tkapi-0.9.8/tests/test_verslag.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     8328 2020-04-25 14:15:25.000000 tkapi-0.9.8/tests/test_zaak.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2023-07-18 17:36:03.474095 tkapi-0.9.8/tkapi/
+-rw-rw-r--   0 bart      (1000) bart      (1000)       25 2019-12-13 22:59:19.000000 tkapi-0.9.8/tkapi/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     7496 2023-07-18 17:16:58.000000 tkapi-0.9.8/tkapi/activiteit.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1808 2019-12-22 14:11:05.000000 tkapi-0.9.8/tkapi/agendapunt.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1779 2019-12-13 23:38:51.000000 tkapi-0.9.8/tkapi/besluit.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     6452 2019-12-22 14:11:05.000000 tkapi-0.9.8/tkapi/commissie.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5390 2019-12-14 11:43:11.000000 tkapi-0.9.8/tkapi/core.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)    13004 2023-07-18 15:51:51.000000 tkapi-0.9.8/tkapi/document.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1951 2019-12-13 23:34:14.000000 tkapi-0.9.8/tkapi/dossier.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3193 2019-12-22 14:11:05.000000 tkapi-0.9.8/tkapi/filter.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     5852 2019-12-22 14:11:05.000000 tkapi-0.9.8/tkapi/fractie.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      723 2019-12-13 22:46:47.000000 tkapi-0.9.8/tkapi/info.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1175 2019-12-13 23:16:18.000000 tkapi-0.9.8/tkapi/kamervraag.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      845 2019-09-27 13:55:07.000000 tkapi-0.9.8/tkapi/order.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     8757 2023-07-18 15:51:51.000000 tkapi-0.9.8/tkapi/persoon.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2010 2019-12-13 23:18:42.000000 tkapi-0.9.8/tkapi/stemming.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     8500 2023-07-18 15:51:51.000000 tkapi-0.9.8/tkapi/tkapi.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2023-07-18 17:36:03.474095 tkapi-0.9.8/tkapi/util/
+-rw-rw-r--   0 bart      (1000) bart      (1000)        0 2018-10-26 17:21:37.000000 tkapi-0.9.8/tkapi/util/__init__.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     2431 2019-12-08 11:39:14.000000 tkapi-0.9.8/tkapi/util/document.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     6653 2019-12-13 22:46:47.000000 tkapi-0.9.8/tkapi/util/queries.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)      766 2019-12-13 22:56:31.000000 tkapi-0.9.8/tkapi/util/util.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1929 2023-07-18 15:51:51.000000 tkapi-0.9.8/tkapi/vergadering.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     1146 2020-01-18 18:24:28.000000 tkapi-0.9.8/tkapi/verslag.py
+-rw-rw-r--   0 bart      (1000) bart      (1000)     9224 2023-07-18 15:51:51.000000 tkapi-0.9.8/tkapi/zaak.py
+drwxrwxr-x   0 bart      (1000) bart      (1000)        0 2023-07-18 17:36:03.474095 tkapi-0.9.8/tkapi.egg-info/
+-rw-rw-r--   0 bart      (1000) bart      (1000)     3981 2023-07-18 17:36:03.000000 tkapi-0.9.8/tkapi.egg-info/PKG-INFO
+-rw-rw-r--   0 bart      (1000) bart      (1000)      988 2023-07-18 17:36:03.000000 tkapi-0.9.8/tkapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)        1 2023-07-18 17:36:03.000000 tkapi-0.9.8/tkapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)       38 2023-07-18 17:36:03.000000 tkapi-0.9.8/tkapi.egg-info/requires.txt
+-rw-rw-r--   0 bart      (1000) bart      (1000)        6 2023-07-18 17:36:03.000000 tkapi-0.9.8/tkapi.egg-info/top_level.txt
```

### Comparing `tkapi-0.9.7/LICENSE.md` & `tkapi-0.9.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/PKG-INFO` & `tkapi-0.9.8/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tkapi
-Version: 0.9.7
+Version: 0.9.8
 Summary: Python bindings and ORM for the Tweede Kamer OData API
 Home-page: https://github.com/openkamer/tkapi
 Author: Open Kamer
 Author-email: info@openkamer.org
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # tkapi
-[![PyPI version](https://badge.fury.io/py/tkapi.svg)](https://badge.fury.io/py/tkapi)  
+[![PyPI version](https://badge.fury.io/py/tkapi.svg)](https://badge.fury.io/py/tkapi) ![CI/CD status](https://github.com/openkamer/tkapi/actions/workflows/main.yml/badge.svg)  
 Python ORM and bindings for the [Tweede Kamer](https://tweedekamer.nl) [Open Data Portaal](https://opendata.tweedekamer.nl) OData API.
 
 A pure Python interface for the Tweede Kamer API with type annotations for easy data model discovery.
 
 Requires Python 3.5+.
 
 Please create an issue if you have any problems, questions or suggestions.
```

### Comparing `tkapi-0.9.7/README.md` & `tkapi-0.9.8/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # tkapi
-[![PyPI version](https://badge.fury.io/py/tkapi.svg)](https://badge.fury.io/py/tkapi)  
+[![PyPI version](https://badge.fury.io/py/tkapi.svg)](https://badge.fury.io/py/tkapi) ![CI/CD status](https://github.com/openkamer/tkapi/actions/workflows/main.yml/badge.svg)  
 Python ORM and bindings for the [Tweede Kamer](https://tweedekamer.nl) [Open Data Portaal](https://opendata.tweedekamer.nl) OData API.
 
 A pure Python interface for the Tweede Kamer API with type annotations for easy data model discovery.
 
 Requires Python 3.5+.
 
 Please create an issue if you have any problems, questions or suggestions.
```

### Comparing `tkapi-0.9.7/setup.py` & `tkapi-0.9.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 setup(
     name='tkapi',
     description='Python bindings and ORM for the Tweede Kamer OData API',
     long_description=long_description,
     long_description_content_type="text/markdown",
-    version='0.9.7',
+    version='0.9.8',
     url='https://github.com/openkamer/tkapi',
     author='Open Kamer',
     author_email='info@openkamer.org',
     license='MIT',
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
```

### Comparing `tkapi-0.9.7/tests/test_activiteit.py` & `tkapi-0.9.8/tests/test_activiteit.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from tkapi.activiteit import Activiteit
 from tkapi.activiteit import ActiviteitActor
 from tkapi.activiteit import ActiviteitSoort
 from tkapi.activiteit import ActiviteitRelatieSoort
 from tkapi.activiteit import ActiviteitStatus
 from tkapi.activiteit import Reservering
 from tkapi.activiteit import Zaal
+from tkapi.filter import PropertyFilter
 from tkapi.util import queries
 
 from .core import TKApiTestCase
 
 
 class TestActiviteit(TKApiTestCase):
     start_datetime = datetime.datetime(year=2017, month=1, day=1)
@@ -126,7 +127,24 @@
         actors = self.api.get_items(ActiviteitActor, max_items=1)
         self.assertEqual(1, len(actors))
         actor = actors[0]
         self.assertIsNotNone(actor.volgorde)
         self.assertIn(actor.relatie, ActiviteitRelatieSoort)
         print(actor.activiteit.id, actor.persoon, actor.fractie, actor.commissie, actor.fractie_naam, actor.naam, actor.spreektijd)
 
+
+class TestActiviteitActorRelatieSoort(TKApiTestCase):
+
+    def test_activiteit_actor_relatie_soort_enum(self):
+        max_items = 1
+        for soort in ActiviteitRelatieSoort:
+            filter = PropertyFilter()
+            filter.filter_property(property_name='relatie', value=soort, is_or=False)
+            actors = self.api.get_items(ActiviteitActor, filter=filter, max_items=max_items)
+            self.assertEqual(max_items, len(actors))
+            self.assertEqual(soort, actors[0].relatie)
+
+    def test_get_items(self):
+        actors = self.api.get_items(ActiviteitActor, max_items=500)
+        for actor in actors:
+            self.assertIn(actor.relatie, ActiviteitRelatieSoort)
+
```

### Comparing `tkapi-0.9.7/tests/test_agendapunt.py` & `tkapi-0.9.8/tests/test_agendapunt.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_api.py` & `tkapi-0.9.8/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_besluit.py` & `tkapi-0.9.8/tests/test_besluit.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_commissie.py` & `tkapi-0.9.8/tests/test_commissie.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_document.py` & `tkapi-0.9.8/tests/test_document.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_dossier.py` & `tkapi-0.9.8/tests/test_dossier.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_filter.py` & `tkapi-0.9.8/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_fractie.py` & `tkapi-0.9.8/tests/test_fractie.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_kamervraag.py` & `tkapi-0.9.8/tests/test_kamervraag.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_metadata.py` & `tkapi-0.9.8/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_order.py` & `tkapi-0.9.8/tests/test_order.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_persoon.py` & `tkapi-0.9.8/tests/test_persoon.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_stemming.py` & `tkapi-0.9.8/tests/test_stemming.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_util.py` & `tkapi-0.9.8/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_vergadering.py` & `tkapi-0.9.8/tests/test_vergadering.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_verslag.py` & `tkapi-0.9.8/tests/test_verslag.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tests/test_zaak.py` & `tkapi-0.9.8/tests/test_zaak.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/activiteit.py` & `tkapi-0.9.8/tkapi/activiteit.py`

 * *Files 4% similar despite different names*

```diff
@@ -218,16 +218,18 @@
 
     @property
     def naam(self):
         return self.get_property_or_empty_string('Naam')
 
 
 class ActiviteitRelatieSoort(Enum):
+    AANVRAGER = 'Aanvrager'
     AFGEMELD = 'Afgemeld'
     BEWINDSPERSOON = 'Bewindspersoon c.a.'
+    DEELNEMENDE_FRACTIE = 'Deelnemende fractie'
     DEELNEMER = 'Deelnemer'
     INITIATIEFNEMER = 'Initiatiefnemer'
     INTERPELLANT = 'Interpellant'
     VOLGCOMMISSIE = 'Volgcommissie'
 
 
 class ActiviteitActor(TKItem):
```

### Comparing `tkapi-0.9.7/tkapi/agendapunt.py` & `tkapi-0.9.8/tkapi/agendapunt.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/besluit.py` & `tkapi-0.9.8/tkapi/besluit.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/commissie.py` & `tkapi-0.9.8/tkapi/commissie.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/core.py` & `tkapi-0.9.8/tkapi/core.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/document.py` & `tkapi-0.9.8/tkapi/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -292,15 +292,15 @@
     @property
     def commissie(self):
         from tkapi.commissie import Commissie
         return self.related_item(Commissie)
 
 
 class VerslagAlgemeenOverleg(Document):
-    filter_param = "Soort eq 'Verslag van een algemeen overleg'"
+    filter_param = "Soort eq '{}'".format(DocumentSoort.VERSLAG_VAN_EEN_ALGEMEEN_OVERLEG.value)
 
     @property
     def voortouwcommissie_namen(self):
         names = []
         for zaak in self.zaken:
             for zaak_actor in zaak.actors:
                 if zaak_actor.is_voortouwcommissie:
```

### Comparing `tkapi-0.9.7/tkapi/dossier.py` & `tkapi-0.9.8/tkapi/dossier.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/filter.py` & `tkapi-0.9.8/tkapi/filter.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/fractie.py` & `tkapi-0.9.8/tkapi/fractie.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/info.py` & `tkapi-0.9.8/tkapi/info.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/kamervraag.py` & `tkapi-0.9.8/tkapi/kamervraag.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/order.py` & `tkapi-0.9.8/tkapi/order.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/persoon.py` & `tkapi-0.9.8/tkapi/persoon.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/stemming.py` & `tkapi-0.9.8/tkapi/stemming.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/tkapi.py` & `tkapi-0.9.8/tkapi/tkapi.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/util/document.py` & `tkapi-0.9.8/tkapi/util/document.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/util/queries.py` & `tkapi-0.9.8/tkapi/util/queries.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/util/util.py` & `tkapi-0.9.8/tkapi/util/util.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/vergadering.py` & `tkapi-0.9.8/tkapi/vergadering.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/verslag.py` & `tkapi-0.9.8/tkapi/verslag.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi/zaak.py` & `tkapi-0.9.8/tkapi/zaak.py`

 * *Files identical despite different names*

### Comparing `tkapi-0.9.7/tkapi.egg-info/PKG-INFO` & `tkapi-0.9.8/tkapi.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tkapi
-Version: 0.9.7
+Version: 0.9.8
 Summary: Python bindings and ORM for the Tweede Kamer OData API
 Home-page: https://github.com/openkamer/tkapi
 Author: Open Kamer
 Author-email: info@openkamer.org
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
 # tkapi
-[![PyPI version](https://badge.fury.io/py/tkapi.svg)](https://badge.fury.io/py/tkapi)  
+[![PyPI version](https://badge.fury.io/py/tkapi.svg)](https://badge.fury.io/py/tkapi) ![CI/CD status](https://github.com/openkamer/tkapi/actions/workflows/main.yml/badge.svg)  
 Python ORM and bindings for the [Tweede Kamer](https://tweedekamer.nl) [Open Data Portaal](https://opendata.tweedekamer.nl) OData API.
 
 A pure Python interface for the Tweede Kamer API with type annotations for easy data model discovery.
 
 Requires Python 3.5+.
 
 Please create an issue if you have any problems, questions or suggestions.
```

### Comparing `tkapi-0.9.7/tkapi.egg-info/SOURCES.txt` & `tkapi-0.9.8/tkapi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

