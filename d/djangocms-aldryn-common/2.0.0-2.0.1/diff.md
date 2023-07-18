# Comparing `tmp/djangocms-aldryn-common-2.0.0.tar.gz` & `tmp/djangocms-aldryn-common-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-aldryn-common-2.0.0.tar", last modified: Tue Jul 18 07:38:26 2023, max compression
+gzip compressed data, was "djangocms-aldryn-common-2.0.1.tar", last modified: Tue Jul 18 08:33:37 2023, max compression
```

## Comparing `djangocms-aldryn-common-2.0.0.tar` & `djangocms-aldryn-common-2.0.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1474 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.0/LICENSE.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      137 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.0/MANIFEST.in
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1073 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1619 2023-07-18 07:06:59.000000 djangocms-aldryn-common-2.0.0/README.md
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/aldryn_common/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       22 2023-07-18 07:37:27.000000 djangocms-aldryn-common-2.0.0/aldryn_common/__init__.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/aldryn_common/admin_fields/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       81 2023-06-29 08:34:39.000000 djangocms-aldryn-common-2.0.0/aldryn_common/admin_fields/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4320 2023-07-18 07:06:59.000000 djangocms-aldryn-common-2.0.0/aldryn_common/admin_fields/sortedm2m.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.776441 djangocms-aldryn-common-2.0.0/aldryn_common/boilerplates/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.776441 djangocms-aldryn-common-2.0.0/aldryn_common/boilerplates/bootstrap3/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.776441 djangocms-aldryn-common-2.0.0/aldryn_common/boilerplates/bootstrap3/templates/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/aldryn_common/boilerplates/bootstrap3/templates/aldryn_common/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      903 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.0/aldryn_common/boilerplates/bootstrap3/templates/aldryn_common/paginator.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/aldryn_common/boilerplates/legacy/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/aldryn_common/boilerplates/legacy/templates/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/aldryn_common/boilerplates/legacy/templates/aldryn_common/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      523 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.0/aldryn_common/boilerplates/legacy/templates/aldryn_common/paginator.html
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    11582 2023-07-18 07:06:59.000000 djangocms-aldryn-common-2.0.0/aldryn_common/paginator.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2590 2023-07-18 07:06:59.000000 djangocms-aldryn-common-2.0.0/aldryn_common/slugs.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/aldryn_common/templates/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/aldryn_common/templates/admin/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/aldryn_common/templates/admin/aldryn_common/
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/aldryn_common/templates/admin/aldryn_common/widgets/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1201 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.0/aldryn_common/templates/admin/aldryn_common/widgets/sortedm2m_widget.html
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/aldryn_common/templatetags/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.0/aldryn_common/templatetags/__init__.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2018 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.0/aldryn_common/templatetags/date_range.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1547 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.0/aldryn_common/templatetags/html_filter_tags.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5620 2023-07-18 07:06:59.000000 djangocms-aldryn-common-2.0.0/aldryn_common/templatetags/query_string_tools.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      159 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.0/aldryn_common/templatetags/string_tags.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2933 2023-07-18 07:06:59.000000 djangocms-aldryn-common-2.0.0/aldryn_common/timesince.py
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      406 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.0/aldryn_common/tools.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/djangocms_aldryn_common.egg-info/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1073 2023-07-18 07:38:26.000000 djangocms-aldryn-common-2.0.0/djangocms_aldryn_common.egg-info/PKG-INFO
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1006 2023-07-18 07:38:26.000000 djangocms-aldryn-common-2.0.0/djangocms_aldryn_common.egg-info/SOURCES.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-18 07:38:26.000000 djangocms-aldryn-common-2.0.0/djangocms_aldryn_common.egg-info/dependency_links.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-18 07:30:25.000000 djangocms-aldryn-common-2.0.0/djangocms_aldryn_common.egg-info/not-zip-safe
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       29 2023-07-18 07:38:26.000000 djangocms-aldryn-common-2.0.0/djangocms_aldryn_common.egg-info/requires.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       14 2023-07-18 07:38:26.000000 djangocms-aldryn-common-2.0.0/djangocms_aldryn_common.egg-info/top_level.txt
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       99 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/setup.cfg
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1388 2023-07-18 07:33:27.000000 djangocms-aldryn-common-2.0.0/setup.py
-drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 07:38:26.780441 djangocms-aldryn-common-2.0.0/tests/
--rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      902 2023-07-18 07:06:59.000000 djangocms-aldryn-common-2.0.0/tests/test_templatetags.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1474 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.1/LICENSE.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      137 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.1/MANIFEST.in
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2696 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1622 2023-07-18 08:31:56.000000 djangocms-aldryn-common-2.0.1/README.md
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/aldryn_common/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       22 2023-07-18 08:31:56.000000 djangocms-aldryn-common-2.0.1/aldryn_common/__init__.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/aldryn_common/admin_fields/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       81 2023-06-29 08:34:39.000000 djangocms-aldryn-common-2.0.1/aldryn_common/admin_fields/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     4320 2023-07-18 07:06:59.000000 djangocms-aldryn-common-2.0.1/aldryn_common/admin_fields/sortedm2m.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/aldryn_common/boilerplates/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/aldryn_common/boilerplates/bootstrap3/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/aldryn_common/boilerplates/bootstrap3/templates/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/aldryn_common/boilerplates/bootstrap3/templates/aldryn_common/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      903 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.1/aldryn_common/boilerplates/bootstrap3/templates/aldryn_common/paginator.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/aldryn_common/boilerplates/legacy/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/aldryn_common/boilerplates/legacy/templates/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/aldryn_common/boilerplates/legacy/templates/aldryn_common/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      523 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.1/aldryn_common/boilerplates/legacy/templates/aldryn_common/paginator.html
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)    11582 2023-07-18 07:06:59.000000 djangocms-aldryn-common-2.0.1/aldryn_common/paginator.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2590 2023-07-18 07:06:59.000000 djangocms-aldryn-common-2.0.1/aldryn_common/slugs.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/aldryn_common/templates/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/aldryn_common/templates/admin/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/aldryn_common/templates/admin/aldryn_common/
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/aldryn_common/templates/admin/aldryn_common/widgets/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1201 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.1/aldryn_common/templates/admin/aldryn_common/widgets/sortedm2m_widget.html
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/aldryn_common/templatetags/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        0 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.1/aldryn_common/templatetags/__init__.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2018 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.1/aldryn_common/templatetags/date_range.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1547 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.1/aldryn_common/templatetags/html_filter_tags.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     5620 2023-07-18 07:06:59.000000 djangocms-aldryn-common-2.0.1/aldryn_common/templatetags/query_string_tools.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      159 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.1/aldryn_common/templatetags/string_tags.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2933 2023-07-18 07:06:59.000000 djangocms-aldryn-common-2.0.1/aldryn_common/timesince.py
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      406 2023-06-15 08:34:15.000000 djangocms-aldryn-common-2.0.1/aldryn_common/tools.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/djangocms_aldryn_common.egg-info/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     2696 2023-07-18 08:33:37.000000 djangocms-aldryn-common-2.0.1/djangocms_aldryn_common.egg-info/PKG-INFO
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1006 2023-07-18 08:33:37.000000 djangocms-aldryn-common-2.0.1/djangocms_aldryn_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-18 08:33:37.000000 djangocms-aldryn-common-2.0.1/djangocms_aldryn_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)        1 2023-07-18 07:30:25.000000 djangocms-aldryn-common-2.0.1/djangocms_aldryn_common.egg-info/not-zip-safe
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       29 2023-07-18 08:33:37.000000 djangocms-aldryn-common-2.0.1/djangocms_aldryn_common.egg-info/requires.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       14 2023-07-18 08:33:37.000000 djangocms-aldryn-common-2.0.1/djangocms_aldryn_common.egg-info/top_level.txt
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)       99 2023-07-18 08:33:37.891468 djangocms-aldryn-common-2.0.1/setup.cfg
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)     1435 2023-07-18 07:53:06.000000 djangocms-aldryn-common-2.0.1/setup.py
+drwxrwxr-x   0 zbohm     (1000) zbohm     (1000)        0 2023-07-18 08:33:37.887468 djangocms-aldryn-common-2.0.1/tests/
+-rw-rw-r--   0 zbohm     (1000) zbohm     (1000)      902 2023-07-18 07:06:59.000000 djangocms-aldryn-common-2.0.1/tests/test_templatetags.py
```

### Comparing `djangocms-aldryn-common-2.0.0/LICENSE.txt` & `djangocms-aldryn-common-2.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-common-2.0.0/README.md` & `djangocms-aldryn-common-2.0.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -20,9 +20,8 @@
 * handling slugs (cleaning, ensuring uniqueness)
 * managing times and dates
 
 as well as a variety of helpful templatetags and more.
 
 ## Settings:
 
-* ``ALDRYN_COMMON_PAGINATION_SOFTLIMIT``: Soft-limiting search results. If True, querying a page number larger than max.
- will not fail, but instead return the last available page. Default is True.
+* ``ALDRYN_COMMON_PAGINATION_SOFTLIMIT``: Soft-limiting search results. If True, querying a page number larger than max. will not fail, but instead return the last available page. Default is ``True``.
```

### Comparing `djangocms-aldryn-common-2.0.0/aldryn_common/admin_fields/sortedm2m.py` & `djangocms-aldryn-common-2.0.1/aldryn_common/admin_fields/sortedm2m.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-common-2.0.0/aldryn_common/boilerplates/bootstrap3/templates/aldryn_common/paginator.html` & `djangocms-aldryn-common-2.0.1/aldryn_common/boilerplates/bootstrap3/templates/aldryn_common/paginator.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-common-2.0.0/aldryn_common/boilerplates/legacy/templates/aldryn_common/paginator.html` & `djangocms-aldryn-common-2.0.1/aldryn_common/boilerplates/legacy/templates/aldryn_common/paginator.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-common-2.0.0/aldryn_common/paginator.py` & `djangocms-aldryn-common-2.0.1/aldryn_common/paginator.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-common-2.0.0/aldryn_common/slugs.py` & `djangocms-aldryn-common-2.0.1/aldryn_common/slugs.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-common-2.0.0/aldryn_common/templates/admin/aldryn_common/widgets/sortedm2m_widget.html` & `djangocms-aldryn-common-2.0.1/aldryn_common/templates/admin/aldryn_common/widgets/sortedm2m_widget.html`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-common-2.0.0/aldryn_common/templatetags/date_range.py` & `djangocms-aldryn-common-2.0.1/aldryn_common/templatetags/date_range.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-common-2.0.0/aldryn_common/templatetags/html_filter_tags.py` & `djangocms-aldryn-common-2.0.1/aldryn_common/templatetags/html_filter_tags.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-common-2.0.0/aldryn_common/templatetags/query_string_tools.py` & `djangocms-aldryn-common-2.0.1/aldryn_common/templatetags/query_string_tools.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-common-2.0.0/aldryn_common/timesince.py` & `djangocms-aldryn-common-2.0.1/aldryn_common/timesince.py`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-common-2.0.0/djangocms_aldryn_common.egg-info/SOURCES.txt` & `djangocms-aldryn-common-2.0.1/djangocms_aldryn_common.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-aldryn-common-2.0.0/setup.py` & `djangocms-aldryn-common-2.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,19 +26,20 @@
     'Programming Language :: Python :: 3.10',
 ]
 
 setup(
     name='djangocms-aldryn-common',
     version=__version__,
     description='Common utilities',
+    long_description=open('README.md').read(),
     author='Divio AG',
     author_email='info@divio.ch',
     url='https://github.com/CZ-NIC/djangocms-aldryn-common',
     packages=find_packages(exclude=['tests']),
-    license='LICENSE.txt',
+    license='BSD License',
     platforms=['OS Independent'],
     python_requires='>=3.7',
     install_requires=REQUIREMENTS,
     classifiers=CLASSIFIERS,
     include_package_data=True,
     zip_safe=False,
     test_suite='tests',
```

### Comparing `djangocms-aldryn-common-2.0.0/tests/test_templatetags.py` & `djangocms-aldryn-common-2.0.1/tests/test_templatetags.py`

 * *Files identical despite different names*

