# Comparing `tmp/ckanext-ckanpackager-2.2.9.tar.gz` & `tmp/ckanext-ckanpackager-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-ckanpackager-2.2.9.tar", last modified: Mon Jul 17 08:14:00 2023, max compression
+gzip compressed data, was "ckanext-ckanpackager-3.0.0.tar", last modified: Tue Jul 18 08:53:40 2023, max compression
```

## Comparing `ckanext-ckanpackager-2.2.9.tar` & `ckanext-ckanpackager-3.0.0.tar`

### file list

```diff
@@ -1,56 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/interfaces.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/lib/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8425 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/lib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/logic/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/logic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/logic/action.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/logic/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/model/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/model/stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     2060 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/routes/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/routes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3048 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/routes/packager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/less/
--rw-r--r--   0 runner    (1001) docker     (123)      927 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/less/ckanpackager.less
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/scripts/modules/
--rw-r--r--   0 runner    (1001) docker     (123)    13051 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/scripts/modules/ckanpackager-download-link.js
--rwxr-xr-x   0 runner    (1001) docker     (123)      302 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/assets/webassets.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/templates/ajax_snippets/
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/templates/ajax_snippets/ckanpackager_form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/templates/ckanpackager/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/templates/ckanpackager/snippets/
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/theme/templates/ckanpackager/snippets/package_resource.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-07-17 08:14:00.000000 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-07-17 08:14:00.000000 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:14:00.000000 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-17 08:14:00.000000 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-17 08:14:00.000000 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-17 08:14:00.000000 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-17 08:14:00.000000 ckanext-ckanpackager-2.2.9/ckanext_ckanpackager.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.400229 ckanext-ckanpackager-2.2.9/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/docs/_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/docs/_scripts/gen_api_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      210 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-17 08:14:00.404229 ckanext-ckanpackager-2.2.9/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1514 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2174 2023-07-17 08:13:48.000000 ckanext-ckanpackager-2.2.9/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:53:40.417113 ckanext-ckanpackager-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-07-18 08:53:29.000000 ckanext-ckanpackager-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-18 08:53:40.417113 ckanext-ckanpackager-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-07-18 08:53:29.000000 ckanext-ckanpackager-3.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:53:40.413113 ckanext-ckanpackager-3.0.0/ckanext/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-18 08:53:29.000000 ckanext-ckanpackager-3.0.0/ckanext/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:53:40.417113 ckanext-ckanpackager-3.0.0/ckanext/ckanpackager/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-07-18 08:53:29.000000 ckanext-ckanpackager-3.0.0/ckanext/ckanpackager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-07-18 08:53:29.000000 ckanext-ckanpackager-3.0.0/ckanext/ckanpackager/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:53:40.417113 ckanext-ckanpackager-3.0.0/ckanext/ckanpackager/model/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-07-18 08:53:29.000000 ckanext-ckanpackager-3.0.0/ckanext/ckanpackager/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-07-18 08:53:29.000000 ckanext-ckanpackager-3.0.0/ckanext/ckanpackager/model/stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-18 08:53:29.000000 ckanext-ckanpackager-3.0.0/ckanext/ckanpackager/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:53:40.417113 ckanext-ckanpackager-3.0.0/ckanext_ckanpackager.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-07-18 08:53:40.000000 ckanext-ckanpackager-3.0.0/ckanext_ckanpackager.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-18 08:53:40.000000 ckanext-ckanpackager-3.0.0/ckanext_ckanpackager.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:53:40.000000 ckanext-ckanpackager-3.0.0/ckanext_ckanpackager.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-07-18 08:53:40.000000 ckanext-ckanpackager-3.0.0/ckanext_ckanpackager.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 08:53:40.000000 ckanext-ckanpackager-3.0.0/ckanext_ckanpackager.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-07-18 08:53:40.000000 ckanext-ckanpackager-3.0.0/ckanext_ckanpackager.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 08:53:40.000000 ckanext-ckanpackager-3.0.0/ckanext_ckanpackager.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:53:40.413113 ckanext-ckanpackager-3.0.0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 08:53:40.417113 ckanext-ckanpackager-3.0.0/docs/_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-07-18 08:53:29.000000 ckanext-ckanpackager-3.0.0/docs/_scripts/gen_api_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-07-18 08:53:29.000000 ckanext-ckanpackager-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 08:53:40.417113 ckanext-ckanpackager-3.0.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      210 2023-07-18 08:53:29.000000 ckanext-ckanpackager-3.0.0/setup.py
```

### Comparing `ckanext-ckanpackager-2.2.9/LICENSE` & `ckanext-ckanpackager-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.9/PKG-INFO` & `ckanext-ckanpackager-3.0.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ckanext-ckanpackager
-Version: 2.2.9
-Summary: A CKAN extension that provides a user interface to download resources with ckanpackager.
+Version: 3.0.0
+Summary: A CKAN extension that stores legacy download statistics from the deprecated service ckanpackager.
 Author-email: Natural History Museum <data@nhm.ac.uk>
 License: GPL-3.0-or-later
 Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager
 Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager/blob/main/CHANGELOG.md
 Keywords: CKAN,data,ckanpackager
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -15,41 +15,44 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
+<!--notices-start-->
+> **Warning**
+> ## Version 3 of ckanext-ckanpackager removes support for ckanpackager.
+>
+> [ckanpackager](http://github.com/NaturalHistoryMuseum/ckanpackager) is being deprecated, and so v3 of this extension will no longer support connecting to it.
+>
+> **All** functionality is being removed _except for the database tables_, to allow other extensions continuing access to legacy data without having to maintain a ckanpackager instance.
+>
+> If you are still using ckanpackager and wish to use this extension with your instance, you will have to use v2 or earlier.
+
+<!--notices-end-->
+
 <!--header-start-->
 <img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-ckanpackager
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-ckanpackager/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-ckanpackager/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-ckanpackager)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
 [![Docs](https://img.shields.io/readthedocs/ckanext-ckanpackager?style=flat-square)](https://ckanext-ckanpackager.readthedocs.io)
 
-_A CKAN extension that provides a user interface to download resources with ckanpackager._
+_A CKAN extension that stores legacy download statistics from the deprecated service ckanpackager._
 
 <!--header-end-->
 
 # Overview
 
 <!--overview-start-->
-**This extension will not work without [ckanpackager](http://github.com/NaturalHistoryMuseum/ckanpackager).**
-
-Ckanpackager is a stand-alone service that can be instructed to fetch data on a [CKAN](http://ckan.org) site using the datastore API, pack the data in a ZIP file and email the link to a given address. See the [ckanpackager github page](http://github.com/NaturalHistoryMuseum/ckanpackager) for more information.
-
-The extension provides an HTML snippet that can be used to replace the Download button on resources. The new button will:
-- Provide an overlay explaining the link will be sent later on;
-- Provide a form for users to enter the destination email address;
-- On resource pages, the button will ensure that currently applied filters and searches are forwarded on to the ckanpackager service.
-
 This extension uses a database table in the CKAN database to store stats about packaging events.
 
 <!--overview-end-->
 
 # Installation
 
 <!--installation-start-->
@@ -103,67 +106,40 @@
    ```
 
 <!--installation-end-->
 
 # Configuration
 
 <!--configuration-start-->
-There are two options that _must_ be specified in your .ini config file.
-
-## **[REQUIRED]**
-
-| Name                  | Description                                  | Options |
-|-----------------------|----------------------------------------------|---------|
-| `ckanpackager.url`    | URL to the ckanpackager endpoint             |         |
-| `ckanpackager.secret` | Shared secret with the ckanpackager instance |         |
+All configuration options have been removed.
 
 <!--configuration-end-->
 
 # Usage
 
 <!--usage-start-->
 ## Actions
 
 ### `packager_stats`
-Provides statistical information about the download requests made to the packager. All of the items in the `data_dict` are optional.
-
-```python
-from ckan.plugins import toolkit
-
-data_dict = {
-                'resource_id': RESOURCE_ID,
-                'offset': 0,
-                'limit': 100,
-                'email': REQUESTER_EMAIL
-            }
-
-toolkit.get_action('packager_stats')(
-    context,
-    data_dict
-)
-```
+**REMOVED**
 
 ## Commands
 
 ### `initdb`
 Initialises the ckanpackager database tables.
 
+_This command is still valid, but if you don't already have these database tables, there may not be much point._
+
   ```bash
   ckan -c $CONFIG_FILE ckanpackager initdb
   ```
 
 ## Templates
 
-Add the following snippet to templates where you want the button to appear:
-
-```html+jinja
-{% snippet 'ckanpackager/snippets/package_resource.html',
-   res=res, pkg=pkg, bt_class="fas fa-download", bt_text=_('Download')
-%}
-```
+**REMOVED**
 
 <!--usage-end-->
 
 # Testing
 
 <!--testing-start-->
 There is a Docker compose configuration available in this repository to make it easier to run tests. The ckan image uses the Dockerfile in the `docker/` folder.
```

### Comparing `ckanext-ckanpackager-2.2.9/README.md` & `ckanext-ckanpackager-3.0.0/ckanext_ckanpackager.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,58 @@
+Metadata-Version: 2.1
+Name: ckanext-ckanpackager
+Version: 3.0.0
+Summary: A CKAN extension that stores legacy download statistics from the deprecated service ckanpackager.
+Author-email: Natural History Museum <data@nhm.ac.uk>
+License: GPL-3.0-or-later
+Project-URL: repository, https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager
+Project-URL: changelog, https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager/blob/main/CHANGELOG.md
+Keywords: CKAN,data,ckanpackager
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: test
+License-File: LICENSE
+
+<!--notices-start-->
+> **Warning**
+> ## Version 3 of ckanext-ckanpackager removes support for ckanpackager.
+>
+> [ckanpackager](http://github.com/NaturalHistoryMuseum/ckanpackager) is being deprecated, and so v3 of this extension will no longer support connecting to it.
+>
+> **All** functionality is being removed _except for the database tables_, to allow other extensions continuing access to legacy data without having to maintain a ckanpackager instance.
+>
+> If you are still using ckanpackager and wish to use this extension with your instance, you will have to use v2 or earlier.
+
+<!--notices-end-->
+
 <!--header-start-->
 <img src="https://data.nhm.ac.uk/images/nhm_logo.svg" align="left" width="150px" height="100px" hspace="40"/>
 
 # ckanext-ckanpackager
 
 [![Tests](https://img.shields.io/github/actions/workflow/status/NaturalHistoryMuseum/ckanext-ckanpackager/main.yml?style=flat-square)](https://github.com/NaturalHistoryMuseum/ckanext-ckanpackager/actions/workflows/main.yml)
 [![Coveralls](https://img.shields.io/coveralls/github/NaturalHistoryMuseum/ckanext-ckanpackager/main?style=flat-square)](https://coveralls.io/github/NaturalHistoryMuseum/ckanext-ckanpackager)
 [![CKAN](https://img.shields.io/badge/ckan-2.9.7-orange.svg?style=flat-square)](https://github.com/ckan/ckan)
 [![Python](https://img.shields.io/badge/python-3.6%20%7C%203.7%20%7C%203.8-blue.svg?style=flat-square)](https://www.python.org/)
 [![Docs](https://img.shields.io/readthedocs/ckanext-ckanpackager?style=flat-square)](https://ckanext-ckanpackager.readthedocs.io)
 
-_A CKAN extension that provides a user interface to download resources with ckanpackager._
+_A CKAN extension that stores legacy download statistics from the deprecated service ckanpackager._
 
 <!--header-end-->
 
 # Overview
 
 <!--overview-start-->
-**This extension will not work without [ckanpackager](http://github.com/NaturalHistoryMuseum/ckanpackager).**
-
-Ckanpackager is a stand-alone service that can be instructed to fetch data on a [CKAN](http://ckan.org) site using the datastore API, pack the data in a ZIP file and email the link to a given address. See the [ckanpackager github page](http://github.com/NaturalHistoryMuseum/ckanpackager) for more information.
-
-The extension provides an HTML snippet that can be used to replace the Download button on resources. The new button will:
-- Provide an overlay explaining the link will be sent later on;
-- Provide a form for users to enter the destination email address;
-- On resource pages, the button will ensure that currently applied filters and searches are forwarded on to the ckanpackager service.
-
 This extension uses a database table in the CKAN database to store stats about packaging events.
 
 <!--overview-end-->
 
 # Installation
 
 <!--installation-start-->
@@ -82,67 +106,40 @@
    ```
 
 <!--installation-end-->
 
 # Configuration
 
 <!--configuration-start-->
-There are two options that _must_ be specified in your .ini config file.
-
-## **[REQUIRED]**
-
-| Name                  | Description                                  | Options |
-|-----------------------|----------------------------------------------|---------|
-| `ckanpackager.url`    | URL to the ckanpackager endpoint             |         |
-| `ckanpackager.secret` | Shared secret with the ckanpackager instance |         |
+All configuration options have been removed.
 
 <!--configuration-end-->
 
 # Usage
 
 <!--usage-start-->
 ## Actions
 
 ### `packager_stats`
-Provides statistical information about the download requests made to the packager. All of the items in the `data_dict` are optional.
-
-```python
-from ckan.plugins import toolkit
-
-data_dict = {
-                'resource_id': RESOURCE_ID,
-                'offset': 0,
-                'limit': 100,
-                'email': REQUESTER_EMAIL
-            }
-
-toolkit.get_action('packager_stats')(
-    context,
-    data_dict
-)
-```
+**REMOVED**
 
 ## Commands
 
 ### `initdb`
 Initialises the ckanpackager database tables.
 
+_This command is still valid, but if you don't already have these database tables, there may not be much point._
+
   ```bash
   ckan -c $CONFIG_FILE ckanpackager initdb
   ```
 
 ## Templates
 
-Add the following snippet to templates where you want the button to appear:
-
-```html+jinja
-{% snippet 'ckanpackager/snippets/package_resource.html',
-   res=res, pkg=pkg, bt_class="fas fa-download", bt_text=_('Download')
-%}
-```
+**REMOVED**
 
 <!--usage-end-->
 
 # Testing
 
 <!--testing-start-->
 There is a Docker compose configuration available in this repository to make it easier to run tests. The ckan image uses the Dockerfile in the `docker/` folder.
```

### Comparing `ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/cli.py` & `ckanext-ckanpackager-3.0.0/ckanext/ckanpackager/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.9/ckanext/ckanpackager/model/stat.py` & `ckanext-ckanpackager-3.0.0/ckanext/ckanpackager/model/stat.py`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.9/docs/_scripts/gen_api_pages.py` & `ckanext-ckanpackager-3.0.0/docs/_scripts/gen_api_pages.py`

 * *Files identical despite different names*

### Comparing `ckanext-ckanpackager-2.2.9/pyproject.toml` & `ckanext-ckanpackager-3.0.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "ckanext-ckanpackager"
-version = "2.2.9"
-description = "A CKAN extension that provides a user interface to download resources with ckanpackager."
+version = "3.0.0"
+description = "A CKAN extension that stores legacy download statistics from the deprecated service ckanpackager."
 readme = "README.md"
 requires-python = ">=3.6"
 license = { text = "GPL-3.0-or-later" }
 authors = [
     { name = "Natural History Museum", email = "data@nhm.ac.uk" }
 ]
 keywords = ["CKAN", "data", "ckanpackager"]
@@ -15,15 +15,14 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8"
 ]
 dependencies = [
-    "requests>=1.1.0",
     "ckantools>=0.3.0"
 ]
 
 [project.optional-dependencies]
 test = [
     "mock",
     "pytest>=4.6.5",
@@ -47,20 +46,17 @@
 [tool]
 [tool.setuptools]
 zip-safe = false
 
 [tool.setuptools.packages.find]
 exclude = ["tests", "docs"]
 
-[tool.setuptools.package-data]
-"ckanext.ckanpackager.theme" = ["*", "**/*"]
-
 [tool.commitizen]
 name = "cz_nhm"
-version = "2.2.9"
+version = "3.0.0"
 tag_format = "v$version"
 update_changelog_on_bump = true
 changelog_incremental = true
 version_files = [
     "pyproject.toml:version"
 ]
```

