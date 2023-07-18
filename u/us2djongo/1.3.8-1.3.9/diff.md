# Comparing `tmp/us2djongo-1.3.8.tar.gz` & `tmp/us2djongo-1.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "us2djongo-1.3.8.tar", last modified: Thu Jun 17 03:54:26 2021, max compression
+gzip compressed data, was "us2djongo-1.3.9.tar", last modified: Thu Jun 17 06:33:47 2021, max compression
```

## Comparing `us2djongo-1.3.8.tar` & `us2djongo-1.3.9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxrwxrwx   0        0        0        0 2021-06-17 03:54:26.589232 us2djongo-1.3.8/
--rw-rw-rw-   0        0        0      271 2021-05-26 08:19:57.000000 us2djongo-1.3.8/MANIFEST.in
--rw-rw-rw-   0        0        0     2101 2021-06-17 03:54:26.589232 us2djongo-1.3.8/PKG-INFO
--rw-rw-rw-   0        0        0     3525 2021-05-26 08:19:57.000000 us2djongo-1.3.8/README.md
-drwxrwxrwx   0        0        0        0 2021-06-17 03:54:26.538578 us2djongo-1.3.8/djongo/
--rw-rw-rw-   0        0        0      234 2021-06-17 03:53:55.000000 us2djongo-1.3.8/djongo/__init__.py
--rw-rw-rw-   0        0        0      887 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/admin.py
--rw-rw-rw-   0        0        0     6868 2021-06-07 08:22:49.000000 us2djongo-1.3.8/djongo/base.py
--rw-rw-rw-   0        0        0      167 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/compiler.py
--rw-rw-rw-   0        0        0     1055 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/creation.py
--rw-rw-rw-   0        0        0     2104 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/cursor.py
--rw-rw-rw-   0        0        0      859 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/database.py
-drwxrwxrwx   0        0        0        0 2021-06-17 03:54:26.541579 us2djongo-1.3.8/djongo/dynamic_formsets/
--rw-rw-rw-   0        0        0        0 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/dynamic_formsets/__init__.py
--rw-rw-rw-   0        0        0      157 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/dynamic_formsets/apps.py
-drwxrwxrwx   0        0        0        0 2021-06-17 03:54:26.510583 us2djongo-1.3.8/djongo/dynamic_formsets/static/
-drwxrwxrwx   0        0        0        0 2021-06-17 03:54:26.511579 us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/
-drwxrwxrwx   0        0        0        0 2021-06-17 03:54:26.544580 us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/images/
--rw-rw-rw-   0        0        0      733 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/images/add.png
--rw-rw-rw-   0        0        0      715 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/images/delete.png
-drwxrwxrwx   0        0        0        0 2021-06-17 03:54:26.511579 us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/
-drwxrwxrwx   0        0        0        0 2021-06-17 03:54:26.555579 us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/
--rw-rw-rw-   0        0        0   282115 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.js
--rw-rw-rw-   0        0        0    86929 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.min.js
--rw-rw-rw-   0        0        0   132370 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.min.map
--rw-rw-rw-   0        0        0   227166 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.slim.js
--rw-rw-rw-   0        0        0    69919 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.slim.min.js
--rw-rw-rw-   0        0        0   105346 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.slim.min.map
-drwxrwxrwx   0        0        0        0 2021-06-17 03:54:26.558577 us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery-formset/
--rw-rw-rw-   0        0        0     7958 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery-formset/jquery.formset.js
--rw-rw-rw-   0        0        0     3557 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery-formset/jquery.formset.min.js
-drwxrwxrwx   0        0        0        0 2021-06-17 03:54:26.512578 us2djongo-1.3.8/djongo/dynamic_formsets/templates/
-drwxrwxrwx   0        0        0        0 2021-06-17 03:54:26.559580 us2djongo-1.3.8/djongo/dynamic_formsets/templates/admin/
--rw-rw-rw-   0        0        0     1337 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/dynamic_formsets/templates/admin/change_form.html
-drwxrwxrwx   0        0        0        0 2021-06-17 03:54:26.562579 us2djongo-1.3.8/djongo/dynamic_formsets/templatetags/
--rw-rw-rw-   0        0        0        0 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/dynamic_formsets/templatetags/__init__.py
--rw-rw-rw-   0        0        0      329 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/dynamic_formsets/templatetags/formset_tags.py
--rw-rw-rw-   0        0        0     1202 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/exceptions.py
--rw-rw-rw-   0        0        0      448 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/features.py
--rw-rw-rw-   0        0        0     3605 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/introspection.py
-drwxrwxrwx   0        0        0        0 2021-06-17 03:54:26.567579 us2djongo-1.3.8/djongo/models/
--rw-rw-rw-   0        0        0      413 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/models/__init__.py
--rw-rw-rw-   0        0        0    41685 2021-06-17 03:53:13.000000 us2djongo-1.3.8/djongo/models/fields.py
--rw-rw-rw-   0        0        0       51 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/models/indexes.py
--rw-rw-rw-   0        0        0      590 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/models/json.py
--rw-rw-rw-   0        0        0     4539 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/operations.py
--rw-rw-rw-   0        0        0      627 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/schema.py
-drwxrwxrwx   0        0        0        0 2021-06-17 03:54:26.581234 us2djongo-1.3.8/djongo/sql2mongo/
--rw-rw-rw-   0        0        0        0 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/sql2mongo/__init__.py
--rw-rw-rw-   0        0        0       92 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/sql2mongo/aggregation.py
--rw-rw-rw-   0        0        0      219 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/sql2mongo/constraints.py
--rw-rw-rw-   0        0        0    16236 2021-06-07 08:22:49.000000 us2djongo-1.3.8/djongo/sql2mongo/converters.py
--rw-rw-rw-   0        0        0     3964 2021-06-03 06:22:34.000000 us2djongo-1.3.8/djongo/sql2mongo/functions.py
--rw-rw-rw-   0        0        0    17564 2021-06-17 03:53:13.000000 us2djongo-1.3.8/djongo/sql2mongo/operators.py
--rw-rw-rw-   0        0        0    31960 2021-06-07 08:22:49.000000 us2djongo-1.3.8/djongo/sql2mongo/query.py
--rw-rw-rw-   0        0        0    13095 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/sql2mongo/sql_tokens.py
--rw-rw-rw-   0        0        0      197 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/sql2mongo/validation.py
--rw-rw-rw-   0        0        0     6371 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/storage.py
--rw-rw-rw-   0        0        0      221 2021-05-26 08:19:57.000000 us2djongo-1.3.8/djongo/transaction.py
--rw-rw-rw-   0        0        0      744 2021-06-13 14:22:29.000000 us2djongo-1.3.8/djongo/utils.py
--rw-rw-rw-   0        0        0       86 2021-06-17 03:54:26.590233 us2djongo-1.3.8/setup.cfg
--rw-rw-rw-   0        0        0     2888 2021-06-13 15:03:14.000000 us2djongo-1.3.8/setup.py
-drwxrwxrwx   0        0        0        0 2021-06-17 03:54:26.588232 us2djongo-1.3.8/us2djongo.egg-info/
--rw-rw-rw-   0        0        0     2101 2021-06-17 03:54:26.000000 us2djongo-1.3.8/us2djongo.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1824 2021-06-17 03:54:26.000000 us2djongo-1.3.8/us2djongo.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-06-17 03:54:26.000000 us2djongo-1.3.8/us2djongo.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2021-06-17 03:54:26.000000 us2djongo-1.3.8/us2djongo.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2021-06-17 03:54:26.000000 us2djongo-1.3.8/us2djongo.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-06-17 06:33:47.013065 us2djongo-1.3.9/
+-rw-rw-rw-   0        0        0      271 2021-05-26 08:19:57.000000 us2djongo-1.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2101 2021-06-17 06:33:47.014065 us2djongo-1.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3525 2021-05-26 08:19:57.000000 us2djongo-1.3.9/README.md
+drwxrwxrwx   0        0        0        0 2021-06-17 06:33:46.945066 us2djongo-1.3.9/djongo/
+-rw-rw-rw-   0        0        0      234 2021-06-17 06:33:28.000000 us2djongo-1.3.9/djongo/__init__.py
+-rw-rw-rw-   0        0        0      887 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/admin.py
+-rw-rw-rw-   0        0        0     6868 2021-06-07 08:22:49.000000 us2djongo-1.3.9/djongo/base.py
+-rw-rw-rw-   0        0        0      167 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/compiler.py
+-rw-rw-rw-   0        0        0     1055 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/creation.py
+-rw-rw-rw-   0        0        0     2104 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/cursor.py
+-rw-rw-rw-   0        0        0      859 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/database.py
+drwxrwxrwx   0        0        0        0 2021-06-17 06:33:46.949066 us2djongo-1.3.9/djongo/dynamic_formsets/
+-rw-rw-rw-   0        0        0        0 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/dynamic_formsets/__init__.py
+-rw-rw-rw-   0        0        0      157 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/dynamic_formsets/apps.py
+drwxrwxrwx   0        0        0        0 2021-06-17 06:33:46.912066 us2djongo-1.3.9/djongo/dynamic_formsets/static/
+drwxrwxrwx   0        0        0        0 2021-06-17 06:33:46.913066 us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/
+drwxrwxrwx   0        0        0        0 2021-06-17 06:33:46.952065 us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/images/
+-rw-rw-rw-   0        0        0      733 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/images/add.png
+-rw-rw-rw-   0        0        0      715 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/images/delete.png
+drwxrwxrwx   0        0        0        0 2021-06-17 06:33:46.913066 us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/
+drwxrwxrwx   0        0        0        0 2021-06-17 06:33:46.974067 us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/
+-rw-rw-rw-   0        0        0   282115 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.js
+-rw-rw-rw-   0        0        0    86929 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.min.js
+-rw-rw-rw-   0        0        0   132370 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.min.map
+-rw-rw-rw-   0        0        0   227166 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.slim.js
+-rw-rw-rw-   0        0        0    69919 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.slim.min.js
+-rw-rw-rw-   0        0        0   105346 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.slim.min.map
+drwxrwxrwx   0        0        0        0 2021-06-17 06:33:46.978067 us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery-formset/
+-rw-rw-rw-   0        0        0     7958 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery-formset/jquery.formset.js
+-rw-rw-rw-   0        0        0     3557 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery-formset/jquery.formset.min.js
+drwxrwxrwx   0        0        0        0 2021-06-17 06:33:46.914065 us2djongo-1.3.9/djongo/dynamic_formsets/templates/
+drwxrwxrwx   0        0        0        0 2021-06-17 06:33:46.981065 us2djongo-1.3.9/djongo/dynamic_formsets/templates/admin/
+-rw-rw-rw-   0        0        0     1337 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/dynamic_formsets/templates/admin/change_form.html
+drwxrwxrwx   0        0        0        0 2021-06-17 06:33:46.984065 us2djongo-1.3.9/djongo/dynamic_formsets/templatetags/
+-rw-rw-rw-   0        0        0        0 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/dynamic_formsets/templatetags/__init__.py
+-rw-rw-rw-   0        0        0      329 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/dynamic_formsets/templatetags/formset_tags.py
+-rw-rw-rw-   0        0        0     1202 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/exceptions.py
+-rw-rw-rw-   0        0        0      448 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/features.py
+-rw-rw-rw-   0        0        0     3605 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/introspection.py
+drwxrwxrwx   0        0        0        0 2021-06-17 06:33:46.990065 us2djongo-1.3.9/djongo/models/
+-rw-rw-rw-   0        0        0      413 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/models/__init__.py
+-rw-rw-rw-   0        0        0    41685 2021-06-17 03:53:13.000000 us2djongo-1.3.9/djongo/models/fields.py
+-rw-rw-rw-   0        0        0       51 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/models/indexes.py
+-rw-rw-rw-   0        0        0      590 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/models/json.py
+-rw-rw-rw-   0        0        0     4539 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/operations.py
+-rw-rw-rw-   0        0        0      627 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/schema.py
+drwxrwxrwx   0        0        0        0 2021-06-17 06:33:47.004068 us2djongo-1.3.9/djongo/sql2mongo/
+-rw-rw-rw-   0        0        0        0 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/sql2mongo/__init__.py
+-rw-rw-rw-   0        0        0       92 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/sql2mongo/aggregation.py
+-rw-rw-rw-   0        0        0      219 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/sql2mongo/constraints.py
+-rw-rw-rw-   0        0        0    16202 2021-06-17 06:33:14.000000 us2djongo-1.3.9/djongo/sql2mongo/converters.py
+-rw-rw-rw-   0        0        0     3964 2021-06-03 06:22:34.000000 us2djongo-1.3.9/djongo/sql2mongo/functions.py
+-rw-rw-rw-   0        0        0    17564 2021-06-17 03:53:13.000000 us2djongo-1.3.9/djongo/sql2mongo/operators.py
+-rw-rw-rw-   0        0        0    31966 2021-06-17 06:33:02.000000 us2djongo-1.3.9/djongo/sql2mongo/query.py
+-rw-rw-rw-   0        0        0    13095 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/sql2mongo/sql_tokens.py
+-rw-rw-rw-   0        0        0      197 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/sql2mongo/validation.py
+-rw-rw-rw-   0        0        0     6371 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/storage.py
+-rw-rw-rw-   0        0        0      221 2021-05-26 08:19:57.000000 us2djongo-1.3.9/djongo/transaction.py
+-rw-rw-rw-   0        0        0      744 2021-06-13 14:22:29.000000 us2djongo-1.3.9/djongo/utils.py
+-rw-rw-rw-   0        0        0       86 2021-06-17 06:33:47.015067 us2djongo-1.3.9/setup.cfg
+-rw-rw-rw-   0        0        0     2888 2021-06-13 15:03:14.000000 us2djongo-1.3.9/setup.py
+drwxrwxrwx   0        0        0        0 2021-06-17 06:33:47.012067 us2djongo-1.3.9/us2djongo.egg-info/
+-rw-rw-rw-   0        0        0     2101 2021-06-17 06:33:46.000000 us2djongo-1.3.9/us2djongo.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1824 2021-06-17 06:33:46.000000 us2djongo-1.3.9/us2djongo.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-06-17 06:33:46.000000 us2djongo-1.3.9/us2djongo.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2021-06-17 06:33:46.000000 us2djongo-1.3.9/us2djongo.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2021-06-17 06:33:46.000000 us2djongo-1.3.9/us2djongo.egg-info/top_level.txt
```

### Comparing `us2djongo-1.3.8/PKG-INFO` & `us2djongo-1.3.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: us2djongo
-Version: 1.3.8
+Version: 1.3.9
 Summary: Driver for allowing Django to use MongoDB as the database backend.
 Home-page: https://github.com/morbitech1/djongo
 Author: nesdis
 Author-email: nesdis@gmail.com
 License: AGPL
 Description:
```

### Comparing `us2djongo-1.3.8/README.md` & `us2djongo-1.3.9/README.md`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/admin.py` & `us2djongo-1.3.9/djongo/admin.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/base.py` & `us2djongo-1.3.9/djongo/base.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/creation.py` & `us2djongo-1.3.9/djongo/creation.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/cursor.py` & `us2djongo-1.3.9/djongo/cursor.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/database.py` & `us2djongo-1.3.9/djongo/database.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/images/add.png` & `us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/images/add.png`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/images/delete.png` & `us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/images/delete.png`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.js` & `us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.min.js` & `us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.min.js`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.min.map` & `us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.min.map`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.slim.js` & `us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.slim.js`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.slim.min.js` & `us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.slim.min.js`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.slim.min.map` & `us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery/jquery.slim.min.map`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery-formset/jquery.formset.js` & `us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery-formset/jquery.formset.js`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery-formset/jquery.formset.min.js` & `us2djongo-1.3.9/djongo/dynamic_formsets/static/dynamic_formsets/js/jquery-formset/jquery.formset.min.js`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/dynamic_formsets/templates/admin/change_form.html` & `us2djongo-1.3.9/djongo/dynamic_formsets/templates/admin/change_form.html`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/exceptions.py` & `us2djongo-1.3.9/djongo/exceptions.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/introspection.py` & `us2djongo-1.3.9/djongo/introspection.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/models/fields.py` & `us2djongo-1.3.9/djongo/models/fields.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/models/json.py` & `us2djongo-1.3.9/djongo/models/json.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/operations.py` & `us2djongo-1.3.9/djongo/operations.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/schema.py` & `us2djongo-1.3.9/djongo/schema.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/sql2mongo/converters.py` & `us2djongo-1.3.9/djongo/sql2mongo/converters.py`

 * *Files 1% similar despite different names*

```diff
@@ -489,17 +489,16 @@
 
     def __init__(self, *args):
         self.sql_tokens: List[SQLToken] = []
         super().__init__(*args)
 
     def parse(self):
         tok = self.statement.next()
-        if not tok.match(tokens.Keyword, 'BY'):
-            raise SQLDecodeError
-        tok = self.statement.next()
+        if tok.match(tokens.Keyword, 'BY'):
+            tok = self.statement.next()
         self.sql_tokens.extend(SQLToken.tokens2sql(tok, self.query))
 
     def to_mongo(self):
         _id = self.to_id()
 
         group = {
             '_id': _id
```

### Comparing `us2djongo-1.3.8/djongo/sql2mongo/functions.py` & `us2djongo-1.3.9/djongo/sql2mongo/functions.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/sql2mongo/operators.py` & `us2djongo-1.3.9/djongo/sql2mongo/operators.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/sql2mongo/query.py` & `us2djongo-1.3.9/djongo/sql2mongo/query.py`

 * *Files 0% similar despite different names*

```diff
@@ -144,15 +144,15 @@
                 converter = InnerJoinConverter(self, statement)
                 self.joins.append(converter)
 
             elif tok.match(tokens.Keyword, 'LEFT OUTER JOIN'):
                 converter = OuterJoinConverter(self, statement)
                 self.joins.append(converter)
 
-            elif tok.match(tokens.Keyword, 'GROUP'):
+            elif tok.match(tokens.Keyword, ['GROUP', 'GROUP BY']):
                 self.groupby = GroupbyConverter(self, statement)
 
             elif tok.match(tokens.Keyword, 'HAVING'):
                 self.having = HavingConverter(self, statement)
 
             elif isinstance(tok, Where):
                 self.where = WhereConverter(self, statement)
@@ -958,11 +958,8 @@
         'SELECT': _select,
         'UPDATE': _update,
         'INSERT': _insert,
         'DELETE': _delete,
         'CREATE': _create,
         'DROP': _drop,
         'ALTER': _alter
-    }
-
-
-
+    }
```

### Comparing `us2djongo-1.3.8/djongo/sql2mongo/sql_tokens.py` & `us2djongo-1.3.9/djongo/sql2mongo/sql_tokens.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/storage.py` & `us2djongo-1.3.9/djongo/storage.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/djongo/utils.py` & `us2djongo-1.3.9/djongo/utils.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/setup.py` & `us2djongo-1.3.9/setup.py`

 * *Files identical despite different names*

### Comparing `us2djongo-1.3.8/us2djongo.egg-info/PKG-INFO` & `us2djongo-1.3.9/us2djongo.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: us2djongo
-Version: 1.3.8
+Version: 1.3.9
 Summary: Driver for allowing Django to use MongoDB as the database backend.
 Home-page: https://github.com/morbitech1/djongo
 Author: nesdis
 Author-email: nesdis@gmail.com
 License: AGPL
 Description:
```

### Comparing `us2djongo-1.3.8/us2djongo.egg-info/SOURCES.txt` & `us2djongo-1.3.9/us2djongo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

