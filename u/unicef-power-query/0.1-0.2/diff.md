# Comparing `tmp/unicef-power-query-0.1.tar.gz` & `tmp/unicef-power-query-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unicef-power-query-0.1.tar", last modified: Tue Jul  4 08:15:07 2023, max compression
+gzip compressed data, was "unicef-power-query-0.2.tar", last modified: Tue Jul 18 09:19:09 2023, max compression
```

## Comparing `unicef-power-query-0.1.tar` & `unicef-power-query-0.2.tar`

### file list

```diff
@@ -1,184 +1,172 @@
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.455888 unicef-power-query-0.1/
--rw-r--r--   0 jojo       (501) staff       (20)       60 2023-05-05 13:28:14.000000 unicef-power-query-0.1/CHANGES
--rw-r--r--   0 jojo       (501) staff       (20)      546 2023-05-05 13:28:14.000000 unicef-power-query-0.1/LICENSE
--rwxr-xr-x   0 jojo       (501) staff       (20)      197 2023-05-05 13:23:06.000000 unicef-power-query-0.1/MANIFEST.in
--rw-r--r--   0 jojo       (501) staff       (20)      527 2023-07-04 08:15:07.456187 unicef-power-query-0.1/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     2190 2023-06-12 10:14:25.000000 unicef-power-query-0.1/README.rst
--rw-r--r--   0 jojo       (501) staff       (20)       82 2023-07-04 08:15:07.456986 unicef-power-query-0.1/setup.cfg
--rwxr-xr-x   0 jojo       (501) staff       (20)     1852 2023-06-05 09:29:59.000000 unicef-power-query-0.1/setup.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.229904 unicef-power-query-0.1/src/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.258900 unicef-power-query-0.1/src/power_query/
--rw-r--r--   0 jojo       (501) staff       (20)       58 2023-06-12 06:56:27.000000 unicef-power-query-0.1/src/power_query/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.296115 unicef-power-query-0.1/src/power_query/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)      248 2023-06-12 07:26:20.000000 unicef-power-query-0.1/src/power_query/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    27954 2023-06-12 07:29:10.000000 unicef-power-query-0.1/src/power_query/__pycache__/admin.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      522 2023-06-12 07:26:20.000000 unicef-power-query-0.1/src/power_query/__pycache__/apps.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     6185 2023-06-12 07:28:39.000000 unicef-power-query-0.1/src/power_query/__pycache__/celery_tasks.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1565 2023-06-12 07:29:10.000000 unicef-power-query-0.1/src/power_query/__pycache__/defaults.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1161 2023-06-12 07:26:20.000000 unicef-power-query-0.1/src/power_query/__pycache__/exceptions.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     2347 2023-06-12 07:28:39.000000 unicef-power-query-0.1/src/power_query/__pycache__/forms.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1519 2023-06-12 07:26:20.000000 unicef-power-query-0.1/src/power_query/__pycache__/json.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    29741 2023-06-12 08:48:39.000000 unicef-power-query-0.1/src/power_query/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      713 2023-06-12 07:30:31.000000 unicef-power-query-0.1/src/power_query/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     9981 2023-06-12 07:26:21.000000 unicef-power-query-0.1/src/power_query/__pycache__/utils.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1213 2023-06-12 07:26:21.000000 unicef-power-query-0.1/src/power_query/__pycache__/validators.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     5028 2023-06-12 07:30:31.000000 unicef-power-query-0.1/src/power_query/__pycache__/views.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     5600 2023-06-12 07:42:14.000000 unicef-power-query-0.1/src/power_query/__pycache__/widget.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    16001 2023-06-12 07:29:07.000000 unicef-power-query-0.1/src/power_query/admin.py
--rw-r--r--   0 jojo       (501) staff       (20)      119 2023-06-12 07:15:51.000000 unicef-power-query-0.1/src/power_query/apps.py
--rw-r--r--   0 jojo       (501) staff       (20)     3009 2023-06-12 07:25:57.000000 unicef-power-query-0.1/src/power_query/celery_tasks.py
--rw-r--r--   0 jojo       (501) staff       (20)     1051 2023-06-12 07:02:06.000000 unicef-power-query-0.1/src/power_query/defaults.py
--rw-r--r--   0 jojo       (501) staff       (20)      404 2023-06-12 07:00:27.000000 unicef-power-query-0.1/src/power_query/exceptions.py
--rw-r--r--   0 jojo       (501) staff       (20)     1438 2023-06-12 07:04:29.000000 unicef-power-query-0.1/src/power_query/forms.py
--rw-r--r--   0 jojo       (501) staff       (20)      572 2023-06-05 13:42:42.000000 unicef-power-query-0.1/src/power_query/json.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.297777 unicef-power-query-0.1/src/power_query/management/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-06-05 13:42:42.000000 unicef-power-query-0.1/src/power_query/management/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.299112 unicef-power-query-0.1/src/power_query/management/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)      188 2023-06-12 07:29:10.000000 unicef-power-query-0.1/src/power_query/management/__pycache__/__init__.cpython-311.pyc
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.301379 unicef-power-query-0.1/src/power_query/management/commands/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-06-05 13:42:42.000000 unicef-power-query-0.1/src/power_query/management/commands/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)     3595 2023-06-12 07:00:27.000000 unicef-power-query-0.1/src/power_query/management/commands/pq.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.317407 unicef-power-query-0.1/src/power_query/migrations/
--rw-r--r--   0 jojo       (501) staff       (20)     6822 2023-06-12 11:26:38.000000 unicef-power-query-0.1/src/power_query/migrations/0001_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)    15779 2023-06-12 11:26:46.000000 unicef-power-query-0.1/src/power_query/migrations/0001_migration_squashed_0014_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)      790 2023-06-12 11:26:38.000000 unicef-power-query-0.1/src/power_query/migrations/0002_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)     1847 2023-06-12 11:26:38.000000 unicef-power-query-0.1/src/power_query/migrations/0003_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)     7651 2023-06-12 11:26:38.000000 unicef-power-query-0.1/src/power_query/migrations/0004_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)      656 2023-06-12 11:26:38.000000 unicef-power-query-0.1/src/power_query/migrations/0005_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)      410 2023-06-12 11:26:38.000000 unicef-power-query-0.1/src/power_query/migrations/0006_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)      760 2023-06-12 11:26:38.000000 unicef-power-query-0.1/src/power_query/migrations/0007_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)     1132 2023-06-12 11:26:38.000000 unicef-power-query-0.1/src/power_query/migrations/0008_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)      484 2023-06-12 11:26:46.000000 unicef-power-query-0.1/src/power_query/migrations/0009_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)      544 2023-06-12 11:26:38.000000 unicef-power-query-0.1/src/power_query/migrations/0010_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)      702 2023-06-12 11:26:46.000000 unicef-power-query-0.1/src/power_query/migrations/0011_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)      863 2023-06-12 11:26:46.000000 unicef-power-query-0.1/src/power_query/migrations/0012_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)      968 2023-06-12 11:26:38.000000 unicef-power-query-0.1/src/power_query/migrations/0013_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)     1224 2023-06-12 11:26:46.000000 unicef-power-query-0.1/src/power_query/migrations/0014_migration.py
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/migrations/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.317896 unicef-power-query-0.1/src/power_query/migrations/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)      188 2023-06-12 07:29:10.000000 unicef-power-query-0.1/src/power_query/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      753 2023-06-12 07:00:27.000000 unicef-power-query-0.1/src/power_query/mixin.py
--rw-r--r--   0 jojo       (501) staff       (20)    17115 2023-06-12 08:13:36.000000 unicef-power-query-0.1/src/power_query/models.py
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/notify.py
--rw-r--r--   0 jojo       (501) staff       (20)       91 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/signals.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.327118 unicef-power-query-0.1/src/power_query/static/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.226109 unicef-power-query-0.1/src/power_query/static/admin/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.331884 unicef-power-query-0.1/src/power_query/static/admin/power_query/
--rw-r--r--   0 jojo       (501) staff       (20)     3628 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/code.css
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.368556 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/
--rw-r--r--   0 jojo       (501) staff       (20)     1969 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/abcdef.css
--rw-r--r--   0 jojo       (501) staff       (20)     2507 2023-05-08 13:33:06.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/active-line.js
--rw-r--r--   0 jojo       (501) staff       (20)     8706 2023-05-08 13:33:06.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/codemirror.css
--rw-r--r--   0 jojo       (501) staff       (20)   400161 2023-05-08 13:33:06.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/codemirror.js
--rw-r--r--   0 jojo       (501) staff       (20)    11792 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/django.js
--rw-r--r--   0 jojo       (501) staff       (20)     4983 2023-05-08 13:33:06.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/foldcode.js
--rw-r--r--   0 jojo       (501) staff       (20)      435 2023-05-08 13:33:06.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/foldgutter.css
--rw-r--r--   0 jojo       (501) staff       (20)     5368 2023-05-08 13:33:06.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/foldgutter.js
--rw-r--r--   0 jojo       (501) staff       (20)      118 2023-05-08 13:33:06.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/fullscreen.css
--rw-r--r--   0 jojo       (501) staff       (20)     1495 2023-05-08 13:33:06.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/fullscreen.js
--rw-r--r--   0 jojo       (501) staff       (20)     1674 2023-05-08 13:33:06.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/indent-fold.js
--rw-r--r--   0 jojo       (501) staff       (20)     6816 2023-05-08 13:33:06.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/matchbrackets.js
--rw-r--r--   0 jojo       (501) staff       (20)     1856 2023-05-08 13:33:06.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/midnight.css
--rw-r--r--   0 jojo       (501) staff       (20)     3241 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/overlay.js
--rw-r--r--   0 jojo       (501) staff       (20)    14924 2023-05-08 13:33:06.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/python.js
--rw-r--r--   0 jojo       (501) staff       (20)    13351 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/xml.js
--rw-r--r--   0 jojo       (501) staff       (20)     3733 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/yaml.js
--rw-r--r--   0 jojo       (501) staff       (20)     5122 2023-06-05 09:29:59.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/colorful.css
--rw-r--r--   0 jojo       (501) staff       (20)      760 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/diff.css
--rw-r--r--   0 jojo       (501) staff       (20)    16556 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/static/admin/power_query/editor.png
--rw-r--r--   0 jojo       (501) staff       (20)      292 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/static/power_query.css
--rw-r--r--   0 jojo       (501) staff       (20)      204 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/static/power_query.css.map
--rw-r--r--   0 jojo       (501) staff       (20)      355 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/static/power_query.scss
--rw-r--r--   0 jojo       (501) staff       (20)     6742 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/static/redo.png
--rw-r--r--   0 jojo       (501) staff       (20)     6554 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/static/undo.png
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.228472 unicef-power-query-0.1/src/power_query/templates/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.227119 unicef-power-query-0.1/src/power_query/templates/admin/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.228230 unicef-power-query-0.1/src/power_query/templates/admin/power_query/
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.370639 unicef-power-query-0.1/src/power_query/templates/admin/power_query/dataset/
--rw-r--r--   0 jojo       (501) staff       (20)      109 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templates/admin/power_query/dataset/change_form.html
--rw-r--r--   0 jojo       (501) staff       (20)      366 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templates/admin/power_query/dataset/export.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.373883 unicef-power-query-0.1/src/power_query/templates/admin/power_query/formatter/
--rw-r--r--   0 jojo       (501) staff       (20)     2750 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templates/admin/power_query/formatter/change_form.html
--rw-r--r--   0 jojo       (501) staff       (20)      360 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templates/admin/power_query/formatter/change_list.html
--rw-r--r--   0 jojo       (501) staff       (20)      489 2023-06-12 09:16:51.000000 unicef-power-query-0.1/src/power_query/templates/admin/power_query/formatter/test.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.378622 unicef-power-query-0.1/src/power_query/templates/admin/power_query/query/
--rw-r--r--   0 jojo       (501) staff       (20)      407 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templates/admin/power_query/query/change_form.html
--rw-r--r--   0 jojo       (501) staff       (20)      366 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templates/admin/power_query/query/export.html
--rw-r--r--   0 jojo       (501) staff       (20)      822 2023-06-06 10:54:17.000000 unicef-power-query-0.1/src/power_query/templates/admin/power_query/query/monitor.html
--rw-r--r--   0 jojo       (501) staff       (20)     2003 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templates/admin/power_query/query/preview.html
--rw-r--r--   0 jojo       (501) staff       (20)      490 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templates/admin/power_query/query/run_result.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.381171 unicef-power-query-0.1/src/power_query/templates/admin/power_query/queryargs/
--rw-r--r--   0 jojo       (501) staff       (20)     1559 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templates/admin/power_query/queryargs/change_form.html
--rw-r--r--   0 jojo       (501) staff       (20)      479 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templates/admin/power_query/queryargs/preview.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.383775 unicef-power-query-0.1/src/power_query/templates/admin/power_query/report/
--rw-r--r--   0 jojo       (501) staff       (20)      360 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templates/admin/power_query/report/change_list.html
--rw-r--r--   0 jojo       (501) staff       (20)      743 2023-06-06 10:54:17.000000 unicef-power-query-0.1/src/power_query/templates/admin/power_query/report/monitor.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.386655 unicef-power-query-0.1/src/power_query/templates/power_query/
--rw-r--r--   0 jojo       (501) staff       (20)      532 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templates/power_query/base.html
--rw-r--r--   0 jojo       (501) staff       (20)      762 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templates/power_query/detail.html
--rw-r--r--   0 jojo       (501) staff       (20)      339 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templates/power_query/list.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.387514 unicef-power-query-0.1/src/power_query/templates/power_query/widgets/
--rw-r--r--   0 jojo       (501) staff       (20)     1235 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templates/power_query/widgets/codewidget.html
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.389161 unicef-power-query-0.1/src/power_query/templatetags/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-06-05 09:31:55.000000 unicef-power-query-0.1/src/power_query/templatetags/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.391282 unicef-power-query-0.1/src/power_query/templatetags/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)      190 2023-06-12 07:30:31.000000 unicef-power-query-0.1/src/power_query/templatetags/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     2150 2023-06-12 07:30:31.000000 unicef-power-query-0.1/src/power_query/templatetags/__pycache__/power_query.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      814 2023-06-12 06:58:48.000000 unicef-power-query-0.1/src/power_query/templatetags/power_query.py
--rw-r--r--   0 jojo       (501) staff       (20)      368 2023-06-12 06:59:22.000000 unicef-power-query-0.1/src/power_query/urls.py
--rw-r--r--   0 jojo       (501) staff       (20)     5041 2023-06-12 07:01:08.000000 unicef-power-query-0.1/src/power_query/utils.py
--rw-r--r--   0 jojo       (501) staff       (20)      453 2023-06-12 06:58:01.000000 unicef-power-query-0.1/src/power_query/validators.py
--rw-r--r--   0 jojo       (501) staff       (20)     3360 2023-06-12 07:00:27.000000 unicef-power-query-0.1/src/power_query/views.py
--rw-r--r--   0 jojo       (501) staff       (20)     3111 2023-06-12 07:42:10.000000 unicef-power-query-0.1/src/power_query/widget.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.394583 unicef-power-query-0.1/src/unicef_power_query.egg-info/
--rw-r--r--   0 jojo       (501) staff       (20)      527 2023-07-04 08:15:07.000000 unicef-power-query-0.1/src/unicef_power_query.egg-info/PKG-INFO
--rw-r--r--   0 jojo       (501) staff       (20)     6889 2023-07-04 08:15:07.000000 unicef-power-query-0.1/src/unicef_power_query.egg-info/SOURCES.txt
--rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-04 08:15:07.000000 unicef-power-query-0.1/src/unicef_power_query.egg-info/dependency_links.txt
--rw-r--r--   0 jojo       (501) staff       (20)      319 2023-07-04 08:15:07.000000 unicef-power-query-0.1/src/unicef_power_query.egg-info/requires.txt
--rw-r--r--   0 jojo       (501) staff       (20)       12 2023-07-04 08:15:07.000000 unicef-power-query-0.1/src/unicef_power_query.egg-info/top_level.txt
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.408714 unicef-power-query-0.1/tests/
--rw-r--r--   0 jojo       (501) staff       (20)      214 2023-05-16 13:30:33.000000 unicef-power-query-0.1/tests/.coveragerc
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-31 15:42:34.000000 unicef-power-query-0.1/tests/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.421874 unicef-power-query-0.1/tests/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)      167 2023-06-12 07:29:10.000000 unicef-power-query-0.1/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    13091 2023-06-12 09:20:01.000000 unicef-power-query-0.1/tests/__pycache__/fixtures.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    36910 2023-06-12 09:22:39.000000 unicef-power-query-0.1/tests/__pycache__/test_admin.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     3607 2023-06-12 07:29:10.000000 unicef-power-query-0.1/tests/__pycache__/test_auth.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     7475 2023-06-12 07:29:10.000000 unicef-power-query-0.1/tests/__pycache__/test_celery.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1408 2023-06-12 07:29:10.000000 unicef-power-query-0.1/tests/__pycache__/test_params.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     4525 2023-06-12 07:29:10.000000 unicef-power-query-0.1/tests/__pycache__/test_queries.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     1502 2023-06-12 07:29:10.000000 unicef-power-query-0.1/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
--rw-r--r--   0 jojo       (501) staff       (20)    11905 2023-05-16 12:47:07.000000 unicef-power-query-0.1/tests/__pycache__/test_views.cpython-311-pytest-7.3.1.pyc
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.432197 unicef-power-query-0.1/tests/demoproject/
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-06-02 15:31:56.000000 unicef-power-query-0.1/tests/demoproject/__init__.py
--rw-r--r--   0 jojo       (501) staff       (20)   278528 2023-05-31 15:10:33.000000 unicef-power-query-0.1/tests/demoproject/db.sqlite3
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.444903 unicef-power-query-0.1/tests/demoproject/demo/
--rw-r--r--   0 jojo       (501) staff       (20)       65 2023-06-05 09:29:59.000000 unicef-power-query-0.1/tests/demoproject/demo/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.451812 unicef-power-query-0.1/tests/demoproject/demo/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)      267 2023-06-12 07:26:20.000000 unicef-power-query-0.1/tests/demoproject/demo/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      691 2023-06-12 07:26:20.000000 unicef-power-query-0.1/tests/demoproject/demo/__pycache__/celery.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      738 2023-05-16 12:44:40.000000 unicef-power-query-0.1/tests/demoproject/demo/__pycache__/models.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)     2690 2023-06-12 07:26:20.000000 unicef-power-query-0.1/tests/demoproject/demo/__pycache__/settings.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      525 2023-05-31 11:57:14.000000 unicef-power-query-0.1/tests/demoproject/demo/__pycache__/urls.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      699 2023-05-16 13:01:06.000000 unicef-power-query-0.1/tests/demoproject/demo/__pycache__/wsgi.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      245 2023-06-05 09:29:59.000000 unicef-power-query-0.1/tests/demoproject/demo/celery.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.453656 unicef-power-query-0.1/tests/demoproject/demo/migrations/
--rw-r--r--   0 jojo       (501) staff       (20)     5140 2023-05-05 13:23:06.000000 unicef-power-query-0.1/tests/demoproject/demo/migrations/0001_initial.py
--rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-power-query-0.1/tests/demoproject/demo/migrations/__init__.py
-drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-04 08:15:07.454719 unicef-power-query-0.1/tests/demoproject/demo/migrations/__pycache__/
--rw-r--r--   0 jojo       (501) staff       (20)     3923 2023-05-16 13:01:06.000000 unicef-power-query-0.1/tests/demoproject/demo/migrations/__pycache__/0001_initial.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      195 2023-05-16 13:01:06.000000 unicef-power-query-0.1/tests/demoproject/demo/migrations/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 jojo       (501) staff       (20)      142 2023-05-16 12:43:15.000000 unicef-power-query-0.1/tests/demoproject/demo/models.py
--rw-r--r--   0 jojo       (501) staff       (20)     2590 2023-06-05 09:29:59.000000 unicef-power-query-0.1/tests/demoproject/demo/settings.py
--rw-r--r--   0 jojo       (501) staff       (20)      194 2023-05-16 14:04:29.000000 unicef-power-query-0.1/tests/demoproject/demo/urls.py
--rw-r--r--   0 jojo       (501) staff       (20)      385 2023-05-05 13:23:06.000000 unicef-power-query-0.1/tests/demoproject/demo/wsgi.py
--rw-r--r--   0 jojo       (501) staff       (20)      475 2023-05-05 13:23:06.000000 unicef-power-query-0.1/tests/demoproject/factories.py
--rwxr-xr-x   0 jojo       (501) staff       (20)      246 2023-06-05 09:29:59.000000 unicef-power-query-0.1/tests/demoproject/manage.py
--rw-r--r--   0 jojo       (501) staff       (20)     5510 2023-06-12 09:23:35.000000 unicef-power-query-0.1/tests/fixtures.py
--rw-r--r--   0 jojo       (501) staff       (20)    10370 2023-06-12 09:23:35.000000 unicef-power-query-0.1/tests/test_admin.py
--rw-r--r--   0 jojo       (501) staff       (20)     1709 2023-06-05 09:29:59.000000 unicef-power-query-0.1/tests/test_auth.py
--rw-r--r--   0 jojo       (501) staff       (20)     2087 2023-06-05 09:29:59.000000 unicef-power-query-0.1/tests/test_celery.py
--rw-r--r--   0 jojo       (501) staff       (20)      430 2023-06-05 09:29:59.000000 unicef-power-query-0.1/tests/test_params.py
--rw-r--r--   0 jojo       (501) staff       (20)     1979 2023-06-05 09:29:59.000000 unicef-power-query-0.1/tests/test_queries.py
--rw-r--r--   0 jojo       (501) staff       (20)      829 2023-06-05 09:29:59.000000 unicef-power-query-0.1/tests/test_utils.py
--rw-r--r--   0 jojo       (501) staff       (20)     1022 2023-06-05 09:29:59.000000 unicef-power-query-0.1/tox.ini
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.585050 unicef-power-query-0.2/
+-rw-r--r--   0 jojo       (501) staff       (20)      142 2023-07-18 09:06:00.000000 unicef-power-query-0.2/CHANGES
+-rw-r--r--   0 jojo       (501) staff       (20)      546 2023-05-05 13:28:14.000000 unicef-power-query-0.2/LICENSE
+-rwxr-xr-x   0 jojo       (501) staff       (20)      197 2023-05-05 13:23:06.000000 unicef-power-query-0.2/MANIFEST.in
+-rw-r--r--   0 jojo       (501) staff       (20)      527 2023-07-18 09:19:09.585274 unicef-power-query-0.2/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     2190 2023-07-04 08:17:12.000000 unicef-power-query-0.2/README.rst
+-rw-r--r--   0 jojo       (501) staff       (20)       82 2023-07-18 09:19:09.586698 unicef-power-query-0.2/setup.cfg
+-rwxr-xr-x   0 jojo       (501) staff       (20)     1852 2023-07-04 08:17:12.000000 unicef-power-query-0.2/setup.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.305578 unicef-power-query-0.2/src/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.330578 unicef-power-query-0.2/src/power_query/
+-rw-r--r--   0 jojo       (501) staff       (20)       58 2023-07-18 09:06:00.000000 unicef-power-query-0.2/src/power_query/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.348126 unicef-power-query-0.2/src/power_query/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)      223 2023-07-13 10:19:44.000000 unicef-power-query-0.2/src/power_query/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    15713 2023-07-13 10:19:49.000000 unicef-power-query-0.2/src/power_query/__pycache__/admin.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      411 2023-07-13 10:19:44.000000 unicef-power-query-0.2/src/power_query/__pycache__/apps.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     3741 2023-07-13 10:19:49.000000 unicef-power-query-0.2/src/power_query/__pycache__/celery_tasks.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1105 2023-07-13 12:04:32.000000 unicef-power-query-0.2/src/power_query/__pycache__/defaults.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      816 2023-07-13 10:19:47.000000 unicef-power-query-0.2/src/power_query/__pycache__/exceptions.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     6621 2023-07-18 08:50:32.000000 unicef-power-query-0.2/src/power_query/__pycache__/fixtures.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1494 2023-07-13 10:19:49.000000 unicef-power-query-0.2/src/power_query/__pycache__/forms.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      947 2023-07-13 10:19:47.000000 unicef-power-query-0.2/src/power_query/__pycache__/json.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1130 2023-07-13 10:19:49.000000 unicef-power-query-0.2/src/power_query/__pycache__/mixin.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    16511 2023-07-13 10:19:47.000000 unicef-power-query-0.2/src/power_query/__pycache__/models.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      508 2023-07-13 10:20:35.000000 unicef-power-query-0.2/src/power_query/__pycache__/urls.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     5157 2023-07-13 10:19:47.000000 unicef-power-query-0.2/src/power_query/__pycache__/utils.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      840 2023-07-13 10:19:47.000000 unicef-power-query-0.2/src/power_query/__pycache__/validators.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     2800 2023-07-13 10:20:35.000000 unicef-power-query-0.2/src/power_query/__pycache__/views.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     3645 2023-07-13 10:19:49.000000 unicef-power-query-0.2/src/power_query/__pycache__/widget.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    16001 2023-07-13 09:21:20.000000 unicef-power-query-0.2/src/power_query/admin.py
+-rw-r--r--   0 jojo       (501) staff       (20)      119 2023-07-13 07:16:39.000000 unicef-power-query-0.2/src/power_query/apps.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3009 2023-07-13 07:25:13.000000 unicef-power-query-0.2/src/power_query/celery_tasks.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1051 2023-07-13 07:22:15.000000 unicef-power-query-0.2/src/power_query/defaults.py
+-rw-r--r--   0 jojo       (501) staff       (20)      404 2023-07-13 07:14:46.000000 unicef-power-query-0.2/src/power_query/exceptions.py
+-rw-r--r--   0 jojo       (501) staff       (20)     4351 2023-07-18 09:06:00.000000 unicef-power-query-0.2/src/power_query/fixtures.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1438 2023-07-13 07:24:44.000000 unicef-power-query-0.2/src/power_query/forms.py
+-rw-r--r--   0 jojo       (501) staff       (20)      572 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/json.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.348854 unicef-power-query-0.2/src/power_query/management/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/management/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.349710 unicef-power-query-0.2/src/power_query/management/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)      170 2023-07-17 14:18:07.000000 unicef-power-query-0.2/src/power_query/management/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.351107 unicef-power-query-0.2/src/power_query/management/commands/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/management/commands/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3595 2023-07-13 07:17:04.000000 unicef-power-query-0.2/src/power_query/management/commands/pq.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.352866 unicef-power-query-0.2/src/power_query/migrations/
+-rw-r--r--   0 jojo       (501) staff       (20)    15211 2023-07-18 09:06:00.000000 unicef-power-query-0.2/src/power_query/migrations/0001_migration_squashed_0014_migration.py
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/migrations/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.354160 unicef-power-query-0.2/src/power_query/migrations/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)     5436 2023-07-17 14:18:08.000000 unicef-power-query-0.2/src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      170 2023-07-17 14:18:08.000000 unicef-power-query-0.2/src/power_query/migrations/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      753 2023-07-13 07:18:11.000000 unicef-power-query-0.2/src/power_query/mixin.py
+-rw-r--r--   0 jojo       (501) staff       (20)    17115 2023-07-13 07:27:46.000000 unicef-power-query-0.2/src/power_query/models.py
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/notify.py
+-rw-r--r--   0 jojo       (501) staff       (20)       91 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/signals.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.361728 unicef-power-query-0.2/src/power_query/static/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.301923 unicef-power-query-0.2/src/power_query/static/admin/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.373095 unicef-power-query-0.2/src/power_query/static/admin/power_query/
+-rw-r--r--   0 jojo       (501) staff       (20)     3628 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/code.css
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.408072 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/
+-rw-r--r--   0 jojo       (501) staff       (20)     1969 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/abcdef.css
+-rw-r--r--   0 jojo       (501) staff       (20)     2507 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/active-line.js
+-rw-r--r--   0 jojo       (501) staff       (20)     8706 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/codemirror.css
+-rw-r--r--   0 jojo       (501) staff       (20)   400161 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/codemirror.js
+-rw-r--r--   0 jojo       (501) staff       (20)    11792 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/django.js
+-rw-r--r--   0 jojo       (501) staff       (20)     4983 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/foldcode.js
+-rw-r--r--   0 jojo       (501) staff       (20)      435 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/foldgutter.css
+-rw-r--r--   0 jojo       (501) staff       (20)     5368 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/foldgutter.js
+-rw-r--r--   0 jojo       (501) staff       (20)      118 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/fullscreen.css
+-rw-r--r--   0 jojo       (501) staff       (20)     1495 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/fullscreen.js
+-rw-r--r--   0 jojo       (501) staff       (20)     1674 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/indent-fold.js
+-rw-r--r--   0 jojo       (501) staff       (20)     6816 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/matchbrackets.js
+-rw-r--r--   0 jojo       (501) staff       (20)     1856 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/midnight.css
+-rw-r--r--   0 jojo       (501) staff       (20)     3241 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/overlay.js
+-rw-r--r--   0 jojo       (501) staff       (20)    14924 2023-05-08 13:33:06.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/python.js
+-rw-r--r--   0 jojo       (501) staff       (20)    13351 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/xml.js
+-rw-r--r--   0 jojo       (501) staff       (20)     3733 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/yaml.js
+-rw-r--r--   0 jojo       (501) staff       (20)     5122 2023-07-04 08:17:12.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/colorful.css
+-rw-r--r--   0 jojo       (501) staff       (20)      760 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/diff.css
+-rw-r--r--   0 jojo       (501) staff       (20)    16556 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/admin/power_query/editor.png
+-rw-r--r--   0 jojo       (501) staff       (20)      292 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/power_query.css
+-rw-r--r--   0 jojo       (501) staff       (20)      204 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/power_query.css.map
+-rw-r--r--   0 jojo       (501) staff       (20)      355 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/power_query.scss
+-rw-r--r--   0 jojo       (501) staff       (20)     6742 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/redo.png
+-rw-r--r--   0 jojo       (501) staff       (20)     6554 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/static/undo.png
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.304344 unicef-power-query-0.2/src/power_query/templates/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.302728 unicef-power-query-0.2/src/power_query/templates/admin/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.304049 unicef-power-query-0.2/src/power_query/templates/admin/power_query/
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.414609 unicef-power-query-0.2/src/power_query/templates/admin/power_query/dataset/
+-rw-r--r--   0 jojo       (501) staff       (20)      109 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/dataset/change_form.html
+-rw-r--r--   0 jojo       (501) staff       (20)      366 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/dataset/export.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.417010 unicef-power-query-0.2/src/power_query/templates/admin/power_query/formatter/
+-rw-r--r--   0 jojo       (501) staff       (20)     2750 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/formatter/change_form.html
+-rw-r--r--   0 jojo       (501) staff       (20)      360 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/formatter/change_list.html
+-rw-r--r--   0 jojo       (501) staff       (20)      489 2023-07-13 07:30:38.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/formatter/test.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.420961 unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/
+-rw-r--r--   0 jojo       (501) staff       (20)      407 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/change_form.html
+-rw-r--r--   0 jojo       (501) staff       (20)      366 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/export.html
+-rw-r--r--   0 jojo       (501) staff       (20)      822 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/monitor.html
+-rw-r--r--   0 jojo       (501) staff       (20)     2003 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/preview.html
+-rw-r--r--   0 jojo       (501) staff       (20)      490 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/run_result.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.423621 unicef-power-query-0.2/src/power_query/templates/admin/power_query/queryargs/
+-rw-r--r--   0 jojo       (501) staff       (20)     1559 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/queryargs/change_form.html
+-rw-r--r--   0 jojo       (501) staff       (20)      479 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/queryargs/preview.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.424819 unicef-power-query-0.2/src/power_query/templates/admin/power_query/report/
+-rw-r--r--   0 jojo       (501) staff       (20)      360 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/report/change_list.html
+-rw-r--r--   0 jojo       (501) staff       (20)      743 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/admin/power_query/report/monitor.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.427212 unicef-power-query-0.2/src/power_query/templates/power_query/
+-rw-r--r--   0 jojo       (501) staff       (20)      532 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/power_query/base.html
+-rw-r--r--   0 jojo       (501) staff       (20)      762 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/power_query/detail.html
+-rw-r--r--   0 jojo       (501) staff       (20)      339 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/power_query/list.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.433090 unicef-power-query-0.2/src/power_query/templates/power_query/widgets/
+-rw-r--r--   0 jojo       (501) staff       (20)     1235 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templates/power_query/widgets/codewidget.html
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.440788 unicef-power-query-0.2/src/power_query/templatetags/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2/src/power_query/templatetags/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.467201 unicef-power-query-0.2/src/power_query/templatetags/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)      172 2023-07-13 10:20:43.000000 unicef-power-query-0.2/src/power_query/templatetags/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1295 2023-07-13 10:20:43.000000 unicef-power-query-0.2/src/power_query/templatetags/__pycache__/power_query.cpython-39.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      814 2023-07-13 07:18:11.000000 unicef-power-query-0.2/src/power_query/templatetags/power_query.py
+-rw-r--r--   0 jojo       (501) staff       (20)      368 2023-07-13 07:19:25.000000 unicef-power-query-0.2/src/power_query/urls.py
+-rw-r--r--   0 jojo       (501) staff       (20)     5041 2023-07-13 07:19:03.000000 unicef-power-query-0.2/src/power_query/utils.py
+-rw-r--r--   0 jojo       (501) staff       (20)      453 2023-07-13 07:17:09.000000 unicef-power-query-0.2/src/power_query/validators.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3360 2023-07-13 09:21:39.000000 unicef-power-query-0.2/src/power_query/views.py
+-rw-r--r--   0 jojo       (501) staff       (20)     3111 2023-07-13 07:15:15.000000 unicef-power-query-0.2/src/power_query/widget.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.521110 unicef-power-query-0.2/src/unicef_power_query.egg-info/
+-rw-r--r--   0 jojo       (501) staff       (20)      527 2023-07-18 09:19:09.000000 unicef-power-query-0.2/src/unicef_power_query.egg-info/PKG-INFO
+-rw-r--r--   0 jojo       (501) staff       (20)     6379 2023-07-18 09:19:09.000000 unicef-power-query-0.2/src/unicef_power_query.egg-info/SOURCES.txt
+-rw-r--r--   0 jojo       (501) staff       (20)        1 2023-07-18 09:19:09.000000 unicef-power-query-0.2/src/unicef_power_query.egg-info/dependency_links.txt
+-rw-r--r--   0 jojo       (501) staff       (20)      319 2023-07-18 09:19:09.000000 unicef-power-query-0.2/src/unicef_power_query.egg-info/requires.txt
+-rw-r--r--   0 jojo       (501) staff       (20)       12 2023-07-18 09:19:09.000000 unicef-power-query-0.2/src/unicef_power_query.egg-info/top_level.txt
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.535034 unicef-power-query-0.2/tests/
+-rw-r--r--   0 jojo       (501) staff       (20)      214 2023-05-16 13:30:33.000000 unicef-power-query-0.2/tests/.coveragerc
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-07-13 07:05:45.000000 unicef-power-query-0.2/tests/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.548127 unicef-power-query-0.2/tests/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)    36910 2023-06-12 09:22:39.000000 unicef-power-query-0.2/tests/__pycache__/test_admin.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     3607 2023-06-12 07:29:10.000000 unicef-power-query-0.2/tests/__pycache__/test_auth.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     7475 2023-06-12 07:29:10.000000 unicef-power-query-0.2/tests/__pycache__/test_celery.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1408 2023-06-12 07:29:10.000000 unicef-power-query-0.2/tests/__pycache__/test_params.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     4525 2023-06-12 07:29:10.000000 unicef-power-query-0.2/tests/__pycache__/test_queries.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     1502 2023-06-12 07:29:10.000000 unicef-power-query-0.2/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)    11905 2023-05-16 12:47:07.000000 unicef-power-query-0.2/tests/__pycache__/test_views.cpython-311-pytest-7.3.1.pyc
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.560290 unicef-power-query-0.2/tests/demoproject/
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-06-02 15:31:56.000000 unicef-power-query-0.2/tests/demoproject/__init__.py
+-rw-r--r--   0 jojo       (501) staff       (20)   278528 2023-05-31 15:10:33.000000 unicef-power-query-0.2/tests/demoproject/db.sqlite3
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.575539 unicef-power-query-0.2/tests/demoproject/demo/
+-rw-r--r--   0 jojo       (501) staff       (20)       65 2023-07-04 08:17:12.000000 unicef-power-query-0.2/tests/demoproject/demo/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.580677 unicef-power-query-0.2/tests/demoproject/demo/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)      267 2023-06-12 07:26:20.000000 unicef-power-query-0.2/tests/demoproject/demo/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      691 2023-06-12 07:26:20.000000 unicef-power-query-0.2/tests/demoproject/demo/__pycache__/celery.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      738 2023-05-16 12:44:40.000000 unicef-power-query-0.2/tests/demoproject/demo/__pycache__/models.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)     2690 2023-06-12 07:26:20.000000 unicef-power-query-0.2/tests/demoproject/demo/__pycache__/settings.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      525 2023-05-31 11:57:14.000000 unicef-power-query-0.2/tests/demoproject/demo/__pycache__/urls.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      699 2023-05-16 13:01:06.000000 unicef-power-query-0.2/tests/demoproject/demo/__pycache__/wsgi.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      245 2023-07-04 08:17:12.000000 unicef-power-query-0.2/tests/demoproject/demo/celery.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.582694 unicef-power-query-0.2/tests/demoproject/demo/migrations/
+-rw-r--r--   0 jojo       (501) staff       (20)     5140 2023-05-05 13:23:06.000000 unicef-power-query-0.2/tests/demoproject/demo/migrations/0001_initial.py
+-rw-r--r--   0 jojo       (501) staff       (20)        0 2023-05-05 13:23:06.000000 unicef-power-query-0.2/tests/demoproject/demo/migrations/__init__.py
+drwxr-xr-x   0 jojo       (501) staff       (20)        0 2023-07-18 09:19:09.584208 unicef-power-query-0.2/tests/demoproject/demo/migrations/__pycache__/
+-rw-r--r--   0 jojo       (501) staff       (20)     3923 2023-05-16 13:01:06.000000 unicef-power-query-0.2/tests/demoproject/demo/migrations/__pycache__/0001_initial.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      195 2023-05-16 13:01:06.000000 unicef-power-query-0.2/tests/demoproject/demo/migrations/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 jojo       (501) staff       (20)      142 2023-05-16 12:43:15.000000 unicef-power-query-0.2/tests/demoproject/demo/models.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2590 2023-07-04 08:17:12.000000 unicef-power-query-0.2/tests/demoproject/demo/settings.py
+-rw-r--r--   0 jojo       (501) staff       (20)      194 2023-05-16 14:04:29.000000 unicef-power-query-0.2/tests/demoproject/demo/urls.py
+-rw-r--r--   0 jojo       (501) staff       (20)      385 2023-05-05 13:23:06.000000 unicef-power-query-0.2/tests/demoproject/demo/wsgi.py
+-rw-r--r--   0 jojo       (501) staff       (20)      475 2023-05-05 13:23:06.000000 unicef-power-query-0.2/tests/demoproject/factories.py
+-rwxr-xr-x   0 jojo       (501) staff       (20)      246 2023-07-04 08:17:12.000000 unicef-power-query-0.2/tests/demoproject/manage.py
+-rw-r--r--   0 jojo       (501) staff       (20)    10380 2023-07-18 09:06:00.000000 unicef-power-query-0.2/tests/test_admin.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1719 2023-07-18 09:06:00.000000 unicef-power-query-0.2/tests/test_auth.py
+-rw-r--r--   0 jojo       (501) staff       (20)     2097 2023-07-18 09:06:00.000000 unicef-power-query-0.2/tests/test_celery.py
+-rw-r--r--   0 jojo       (501) staff       (20)      441 2023-07-18 09:06:00.000000 unicef-power-query-0.2/tests/test_params.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1989 2023-07-18 09:06:00.000000 unicef-power-query-0.2/tests/test_queries.py
+-rw-r--r--   0 jojo       (501) staff       (20)      829 2023-07-13 09:09:33.000000 unicef-power-query-0.2/tests/test_utils.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1772 2023-07-18 09:06:00.000000 unicef-power-query-0.2/tests/test_views.py
+-rw-r--r--   0 jojo       (501) staff       (20)     1022 2023-07-04 08:17:12.000000 unicef-power-query-0.2/tox.ini
```

### Comparing `unicef-power-query-0.1/LICENSE` & `unicef-power-query-0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/PKG-INFO` & `unicef-power-query-0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicef-power-query
-Version: 0.1
+Version: 0.2
 Summary: Provides Basic UNICEF User model and integration with Azure
 Home-page: https://github.com/unicef/unicef-security
 Author: UNICEF
 License: Apache 2 License
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `unicef-power-query-0.1/README.rst` & `unicef-power-query-0.2/README.rst`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/setup.py` & `unicef-power-query-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/admin.py` & `unicef-power-query-0.2/src/power_query/admin.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/celery_tasks.py` & `unicef-power-query-0.2/src/power_query/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/defaults.py` & `unicef-power-query-0.2/src/power_query/defaults.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/forms.py` & `unicef-power-query-0.2/src/power_query/forms.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/json.py` & `unicef-power-query-0.2/src/power_query/json.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/management/commands/pq.py` & `unicef-power-query-0.2/src/power_query/management/commands/pq.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/migrations/0001_migration.py` & `unicef-power-query-0.2/tests/demoproject/demo/migrations/0001_initial.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,198 +1,137 @@
-# Generated by Django 2.2.16 on 2022-01-18 06:22
+# Generated by Django 3.2 on 2022-04-06 22:07
 
-import django.contrib.postgres.fields.jsonb
-import django.db.models.deletion
-from django.conf import settings
+import django.contrib.auth.models
+import django.contrib.auth.validators
+import django.utils.timezone
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     initial = True
 
     dependencies = [
-        migrations.swappable_dependency(settings.AUTH_USER_MODEL),
-        ("contenttypes", "0002_remove_content_type_name"),
+        ("auth", "0012_alter_user_first_name_max_length"),
     ]
 
     operations = [
         migrations.CreateModel(
-            name="Formatter",
+            name="User",
             fields=[
                 (
                     "id",
                     models.AutoField(
                         auto_created=True,
                         primary_key=True,
                         serialize=False,
                         verbose_name="ID",
                     ),
                 ),
+                ("password", models.CharField(max_length=128, verbose_name="password")),
                 (
-                    "name",
-                    models.CharField(
-                        blank=True, max_length=255, null=True, unique=True
+                    "last_login",
+                    models.DateTimeField(
+                        blank=True, null=True, verbose_name="last login"
                     ),
                 ),
                 (
-                    "content_type",
-                    models.CharField(
-                        choices=[
-                            ["xls", "application/vnd.ms-excel"],
-                            ["txt", "text/plain"],
-                            ["csv", "text/csv"],
-                            ["html", "text/html"],
-                            ["yaml", "text/yaml"],
-                            ["json", "application/json"],
-                        ],
-                        max_length=5,
-                    ),
-                ),
-                ("code", models.TextField(blank=True, null=True)),
-            ],
-        ),
-        migrations.CreateModel(
-            name="Query",
-            fields=[
-                (
-                    "id",
-                    models.AutoField(
-                        auto_created=True,
-                        primary_key=True,
-                        serialize=False,
-                        verbose_name="ID",
+                    "is_superuser",
+                    models.BooleanField(
+                        default=False,
+                        help_text="Designates that this user has all permissions without explicitly assigning them.",
+                        verbose_name="superuser status",
                     ),
                 ),
                 (
-                    "name",
+                    "username",
                     models.CharField(
-                        blank=True, max_length=255, null=True, unique=True
+                        error_messages={
+                            "unique": "A user with that username already exists."
+                        },
+                        help_text="Required. 150 characters or fewer. Letters, digits and @/./+/-/_ only.",
+                        max_length=150,
+                        unique=True,
+                        validators=[
+                            django.contrib.auth.validators.UnicodeUsernameValidator()
+                        ],
+                        verbose_name="username",
                     ),
                 ),
-                ("description", models.TextField(blank=True, null=True)),
-                ("code", models.TextField(blank=True, default="qs=conn.all()")),
                 (
-                    "info",
-                    django.contrib.postgres.fields.jsonb.JSONField(
-                        blank=True, default=dict
+                    "first_name",
+                    models.CharField(
+                        blank=True, max_length=150, verbose_name="first name"
                     ),
                 ),
                 (
-                    "query_args",
-                    django.contrib.postgres.fields.jsonb.JSONField(
-                        blank=True, default=dict
+                    "last_name",
+                    models.CharField(
+                        blank=True, max_length=150, verbose_name="last name"
                     ),
                 ),
-                ("error", models.CharField(blank=True, max_length=400, null=True)),
                 (
-                    "owner",
-                    models.ForeignKey(
-                        on_delete=django.db.models.deletion.CASCADE,
-                        related_name="power_queries",
-                        to=settings.AUTH_USER_MODEL,
+                    "email",
+                    models.EmailField(
+                        blank=True, max_length=254, verbose_name="email address"
                     ),
                 ),
                 (
-                    "target",
-                    models.ForeignKey(
-                        default="",
-                        on_delete=django.db.models.deletion.CASCADE,
-                        to="contenttypes.ContentType",
+                    "is_staff",
+                    models.BooleanField(
+                        default=False,
+                        help_text="Designates whether the user can log into this admin site.",
+                        verbose_name="staff status",
                     ),
                 ),
-            ],
-            options={
-                "verbose_name_plural": "Power Queries",
-                "ordering": ("name",),
-            },
-        ),
-        migrations.CreateModel(
-            name="Report",
-            fields=[
                 (
-                    "id",
-                    models.AutoField(
-                        auto_created=True,
-                        primary_key=True,
-                        serialize=False,
-                        verbose_name="ID",
+                    "is_active",
+                    models.BooleanField(
+                        default=True,
+                        help_text="Designates whether this user should be treated as active. Unselect this instead of deleting accounts.",
+                        verbose_name="active",
                     ),
                 ),
                 (
-                    "name",
-                    models.CharField(
-                        blank=True, max_length=255, null=True, unique=True
+                    "date_joined",
+                    models.DateTimeField(
+                        default=django.utils.timezone.now, verbose_name="date joined"
                     ),
                 ),
-                ("refresh", models.BooleanField(default=False)),
+                ("azure_id", models.UUIDField(blank=True, null=True, unique=True)),
+                ("job_title", models.CharField(blank=True, max_length=100, null=True)),
                 (
-                    "query_args",
-                    django.contrib.postgres.fields.jsonb.JSONField(
-                        blank=True, default=dict
-                    ),
+                    "display_name",
+                    models.CharField(blank=True, max_length=100, null=True),
                 ),
-                ("last_run", models.DateTimeField(blank=True, null=True)),
-                ("result", models.BinaryField(blank=True, null=True)),
                 (
-                    "available_to",
+                    "groups",
                     models.ManyToManyField(
                         blank=True,
-                        related_name="_report_available_to_+",
-                        to=settings.AUTH_USER_MODEL,
-                    ),
-                ),
-                (
-                    "formatter",
-                    models.ForeignKey(
-                        on_delete=django.db.models.deletion.CASCADE,
-                        to="power_query.Formatter",
+                        help_text="The groups this user belongs to. A user will get all permissions granted to each of their groups.",
+                        related_name="user_set",
+                        related_query_name="user",
+                        to="auth.Group",
+                        verbose_name="groups",
                     ),
                 ),
                 (
-                    "owner",
-                    models.ForeignKey(
+                    "user_permissions",
+                    models.ManyToManyField(
                         blank=True,
-                        null=True,
-                        on_delete=django.db.models.deletion.CASCADE,
-                        related_name="+",
-                        to=settings.AUTH_USER_MODEL,
-                    ),
-                ),
-                (
-                    "query",
-                    models.ForeignKey(
-                        on_delete=django.db.models.deletion.CASCADE,
-                        to="power_query.Query",
+                        help_text="Specific permissions for this user.",
+                        related_name="user_set",
+                        related_query_name="user",
+                        to="auth.Permission",
+                        verbose_name="user permissions",
                     ),
                 ),
             ],
-        ),
-        migrations.CreateModel(
-            name="Dataset",
-            fields=[
-                (
-                    "id",
-                    models.AutoField(
-                        auto_created=True,
-                        primary_key=True,
-                        serialize=False,
-                        verbose_name="ID",
-                    ),
-                ),
-                ("last_run", models.DateTimeField(blank=True, null=True)),
-                ("result", models.BinaryField(blank=True, null=True)),
-                (
-                    "info",
-                    django.contrib.postgres.fields.jsonb.JSONField(
-                        blank=True, default=dict
-                    ),
-                ),
-                (
-                    "query",
-                    models.OneToOneField(
-                        on_delete=django.db.models.deletion.CASCADE,
-                        to="power_query.Query",
-                    ),
-                ),
+            options={
+                "verbose_name": "user",
+                "verbose_name_plural": "users",
+                "abstract": False,
+            },
+            managers=[
+                ("objects", django.contrib.auth.models.UserManager()),
             ],
         ),
     ]
```

### Comparing `unicef-power-query-0.1/src/power_query/migrations/0001_migration_squashed_0014_migration.py` & `unicef-power-query-0.2/src/power_query/migrations/0001_migration_squashed_0014_migration.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,31 +17,14 @@
         arguments = dataset.info.get("arguments", {})
         query_id = dataset.query_id
         dataset.hash = dict_hash({"query": query_id, **arguments})
         dataset.save()
 
 
 class Migration(migrations.Migration):
-    replaces = [
-        ("power_query", "0001_migration"),
-        ("power_query", "0002_migration"),
-        ("power_query", "0003_migration"),
-        ("power_query", "0004_migration"),
-        ("power_query", "0005_migration"),
-        ("power_query", "0006_migration"),
-        ("power_query", "0007_migration"),
-        ("power_query", "0008_migration"),
-        ("power_query", "0009_migration"),
-        ("power_query", "0010_migration"),
-        ("power_query", "0011_migration"),
-        ("power_query", "0012_migration"),
-        ("power_query", "0013_migration"),
-        ("power_query", "0014_migration"),
-    ]
-
     dependencies = [
         migrations.swappable_dependency(settings.AUTH_USER_MODEL),
         ("contenttypes", "0002_remove_content_type_name"),
     ]
 
     operations = [
         migrations.CreateModel(
@@ -144,15 +127,16 @@
                 (
                     "description",
                     models.TextField(blank=True, max_length=255, null=True),
                 ),
                 (
                     "value",
                     models.JSONField(
-                        default=dict, validators=[power_query.models.validate_queryargs]
+                        default=dict,
+                        validators=[power_query.models.validate_queryargs],
                     ),
                 ),
                 (
                     "system",
                     models.BooleanField(blank=True, default=False, editable=False),
                 ),
             ],
@@ -364,15 +348,17 @@
             name="content_type",
             field=models.CharField(choices=[], max_length=5),
         ),
         migrations.AlterField(
             model_name="query",
             name="info",
             field=models.JSONField(
-                blank=True, default=dict, encoder=power_query.json.PQJSONEncoder
+                blank=True,
+                default=dict,
+                encoder=power_query.json.PQJSONEncoder,
             ),
         ),
         migrations.AddField(
             model_name="report",
             name="validity_days",
             field=models.IntegerField(default=365),
         ),
```

### Comparing `unicef-power-query-0.1/src/power_query/mixin.py` & `unicef-power-query-0.2/src/power_query/mixin.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/models.py` & `unicef-power-query-0.2/src/power_query/models.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/code.css` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/code.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/abcdef.css` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/abcdef.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/active-line.js` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/active-line.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/codemirror.css` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/codemirror.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/codemirror.js` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/codemirror.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/django.js` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/django.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/foldcode.js` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/foldcode.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/foldgutter.js` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/foldgutter.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/fullscreen.js` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/fullscreen.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/indent-fold.js` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/indent-fold.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/matchbrackets.js` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/matchbrackets.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/midnight.css` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/midnight.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/overlay.js` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/overlay.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/python.js` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/python.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/xml.js` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/xml.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/codemirror/yaml.js` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/codemirror/yaml.js`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/colorful.css` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/colorful.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/diff.css` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/diff.css`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/admin/power_query/editor.png` & `unicef-power-query-0.2/src/power_query/static/admin/power_query/editor.png`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/redo.png` & `unicef-power-query-0.2/src/power_query/static/redo.png`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/static/undo.png` & `unicef-power-query-0.2/src/power_query/static/undo.png`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/templates/admin/power_query/formatter/change_form.html` & `unicef-power-query-0.2/src/power_query/templates/admin/power_query/formatter/change_form.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/templates/admin/power_query/query/monitor.html` & `unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/monitor.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/templates/admin/power_query/query/preview.html` & `unicef-power-query-0.2/src/power_query/templates/admin/power_query/query/preview.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/templates/admin/power_query/queryargs/change_form.html` & `unicef-power-query-0.2/src/power_query/templates/admin/power_query/queryargs/change_form.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/templates/admin/power_query/report/monitor.html` & `unicef-power-query-0.2/src/power_query/templates/admin/power_query/report/monitor.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/templates/power_query/base.html` & `unicef-power-query-0.2/src/power_query/templates/power_query/base.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/templates/power_query/detail.html` & `unicef-power-query-0.2/src/power_query/templates/power_query/detail.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/templates/power_query/widgets/codewidget.html` & `unicef-power-query-0.2/src/power_query/templates/power_query/widgets/codewidget.html`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/templatetags/power_query.py` & `unicef-power-query-0.2/src/power_query/templatetags/power_query.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/utils.py` & `unicef-power-query-0.2/src/power_query/utils.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/views.py` & `unicef-power-query-0.2/src/power_query/views.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/power_query/widget.py` & `unicef-power-query-0.2/src/power_query/widget.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/src/unicef_power_query.egg-info/PKG-INFO` & `unicef-power-query-0.2/src/unicef_power_query.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unicef-power-query
-Version: 0.1
+Version: 0.2
 Summary: Provides Basic UNICEF User model and integration with Azure
 Home-page: https://github.com/unicef/unicef-security
 Author: UNICEF
 License: Apache 2 License
 Platform: any
 Classifier: Environment :: Web Environment
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `unicef-power-query-0.1/src/unicef_power_query.egg-info/SOURCES.txt` & `unicef-power-query-0.2/src/unicef_power_query.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -7,60 +7,50 @@
 tox.ini
 src/power_query/__init__.py
 src/power_query/admin.py
 src/power_query/apps.py
 src/power_query/celery_tasks.py
 src/power_query/defaults.py
 src/power_query/exceptions.py
+src/power_query/fixtures.py
 src/power_query/forms.py
 src/power_query/json.py
 src/power_query/mixin.py
 src/power_query/models.py
 src/power_query/notify.py
 src/power_query/signals.py
 src/power_query/urls.py
 src/power_query/utils.py
 src/power_query/validators.py
 src/power_query/views.py
 src/power_query/widget.py
-src/power_query/__pycache__/__init__.cpython-311.pyc
-src/power_query/__pycache__/admin.cpython-311.pyc
-src/power_query/__pycache__/apps.cpython-311.pyc
-src/power_query/__pycache__/celery_tasks.cpython-311.pyc
-src/power_query/__pycache__/defaults.cpython-311.pyc
-src/power_query/__pycache__/exceptions.cpython-311.pyc
-src/power_query/__pycache__/forms.cpython-311.pyc
-src/power_query/__pycache__/json.cpython-311.pyc
-src/power_query/__pycache__/models.cpython-311.pyc
-src/power_query/__pycache__/urls.cpython-311.pyc
-src/power_query/__pycache__/utils.cpython-311.pyc
-src/power_query/__pycache__/validators.cpython-311.pyc
-src/power_query/__pycache__/views.cpython-311.pyc
-src/power_query/__pycache__/widget.cpython-311.pyc
+src/power_query/__pycache__/__init__.cpython-39.pyc
+src/power_query/__pycache__/admin.cpython-39.pyc
+src/power_query/__pycache__/apps.cpython-39.pyc
+src/power_query/__pycache__/celery_tasks.cpython-39.pyc
+src/power_query/__pycache__/defaults.cpython-39.pyc
+src/power_query/__pycache__/exceptions.cpython-39.pyc
+src/power_query/__pycache__/fixtures.cpython-39.pyc
+src/power_query/__pycache__/forms.cpython-39.pyc
+src/power_query/__pycache__/json.cpython-39.pyc
+src/power_query/__pycache__/mixin.cpython-39.pyc
+src/power_query/__pycache__/models.cpython-39.pyc
+src/power_query/__pycache__/urls.cpython-39.pyc
+src/power_query/__pycache__/utils.cpython-39.pyc
+src/power_query/__pycache__/validators.cpython-39.pyc
+src/power_query/__pycache__/views.cpython-39.pyc
+src/power_query/__pycache__/widget.cpython-39.pyc
 src/power_query/management/__init__.py
-src/power_query/management/__pycache__/__init__.cpython-311.pyc
+src/power_query/management/__pycache__/__init__.cpython-39.pyc
 src/power_query/management/commands/__init__.py
 src/power_query/management/commands/pq.py
-src/power_query/migrations/0001_migration.py
 src/power_query/migrations/0001_migration_squashed_0014_migration.py
-src/power_query/migrations/0002_migration.py
-src/power_query/migrations/0003_migration.py
-src/power_query/migrations/0004_migration.py
-src/power_query/migrations/0005_migration.py
-src/power_query/migrations/0006_migration.py
-src/power_query/migrations/0007_migration.py
-src/power_query/migrations/0008_migration.py
-src/power_query/migrations/0009_migration.py
-src/power_query/migrations/0010_migration.py
-src/power_query/migrations/0011_migration.py
-src/power_query/migrations/0012_migration.py
-src/power_query/migrations/0013_migration.py
-src/power_query/migrations/0014_migration.py
 src/power_query/migrations/__init__.py
-src/power_query/migrations/__pycache__/__init__.cpython-311.pyc
+src/power_query/migrations/__pycache__/0001_migration_squashed_0014_migration.cpython-39.pyc
+src/power_query/migrations/__pycache__/__init__.cpython-39.pyc
 src/power_query/static/power_query.css
 src/power_query/static/power_query.css.map
 src/power_query/static/power_query.scss
 src/power_query/static/redo.png
 src/power_query/static/undo.png
 src/power_query/static/admin/power_query/code.css
 src/power_query/static/admin/power_query/colorful.css
@@ -99,32 +89,30 @@
 src/power_query/templates/admin/power_query/report/monitor.html
 src/power_query/templates/power_query/base.html
 src/power_query/templates/power_query/detail.html
 src/power_query/templates/power_query/list.html
 src/power_query/templates/power_query/widgets/codewidget.html
 src/power_query/templatetags/__init__.py
 src/power_query/templatetags/power_query.py
-src/power_query/templatetags/__pycache__/__init__.cpython-311.pyc
-src/power_query/templatetags/__pycache__/power_query.cpython-311.pyc
+src/power_query/templatetags/__pycache__/__init__.cpython-39.pyc
+src/power_query/templatetags/__pycache__/power_query.cpython-39.pyc
 src/unicef_power_query.egg-info/PKG-INFO
 src/unicef_power_query.egg-info/SOURCES.txt
 src/unicef_power_query.egg-info/dependency_links.txt
 src/unicef_power_query.egg-info/requires.txt
 src/unicef_power_query.egg-info/top_level.txt
 tests/.coveragerc
 tests/__init__.py
-tests/fixtures.py
 tests/test_admin.py
 tests/test_auth.py
 tests/test_celery.py
 tests/test_params.py
 tests/test_queries.py
 tests/test_utils.py
-tests/__pycache__/__init__.cpython-311.pyc
-tests/__pycache__/fixtures.cpython-311.pyc
+tests/test_views.py
 tests/__pycache__/test_admin.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_auth.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_celery.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_params.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_queries.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc
 tests/__pycache__/test_views.cpython-311-pytest-7.3.1.pyc
```

### Comparing `unicef-power-query-0.1/tests/__pycache__/test_admin.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.2/tests/__pycache__/test_admin.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tests/__pycache__/test_auth.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.2/tests/__pycache__/test_auth.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tests/__pycache__/test_celery.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.2/tests/__pycache__/test_celery.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tests/__pycache__/test_params.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.2/tests/__pycache__/test_params.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tests/__pycache__/test_queries.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.2/tests/__pycache__/test_queries.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.2/tests/__pycache__/test_utils.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tests/__pycache__/test_views.cpython-311-pytest-7.3.1.pyc` & `unicef-power-query-0.2/tests/__pycache__/test_views.cpython-311-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tests/demoproject/db.sqlite3` & `unicef-power-query-0.2/tests/demoproject/db.sqlite3`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tests/demoproject/demo/__pycache__/celery.cpython-311.pyc` & `unicef-power-query-0.2/tests/demoproject/demo/__pycache__/celery.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tests/demoproject/demo/__pycache__/models.cpython-311.pyc` & `unicef-power-query-0.2/tests/demoproject/demo/__pycache__/models.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tests/demoproject/demo/__pycache__/settings.cpython-311.pyc` & `unicef-power-query-0.2/tests/demoproject/demo/__pycache__/settings.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tests/demoproject/demo/__pycache__/urls.cpython-311.pyc` & `unicef-power-query-0.2/tests/demoproject/demo/__pycache__/urls.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tests/demoproject/demo/__pycache__/wsgi.cpython-311.pyc` & `unicef-power-query-0.2/tests/demoproject/demo/__pycache__/wsgi.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tests/demoproject/demo/migrations/__pycache__/0001_initial.cpython-311.pyc` & `unicef-power-query-0.2/tests/demoproject/demo/migrations/__pycache__/0001_initial.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tests/demoproject/demo/settings.py` & `unicef-power-query-0.2/tests/demoproject/demo/settings.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tests/fixtures.py` & `unicef-power-query-0.2/src/power_query/fixtures.py`

 * *Files 22% similar despite different names*

```diff
@@ -64,14 +64,29 @@
     code = "result=conn.all()"
 
     class Meta:
         model = Query
         # django_get_or_create = ("name",)
 
 
+class DatasetFactory(DjangoModelFactory):
+    query = factory.SubFactory(QueryFactory)
+
+    class Meta:
+        model = Dataset
+        # django_get_or_create = ("name",)
+
+    @classmethod
+    def create(cls, **kwargs: Dict) -> Dataset:
+        # ret = super().create(**kwargs)
+        q: Query = cls.query.get_factory().create()
+        q.run(persist=True)
+        return q.datasets.first()
+
+
 class FormatterFactory(DjangoModelFactory):
     name = factory.Sequence(lambda x: "Formatter%s" % x)
     content_type = "html"
 
     class Meta:
         model = Formatter
         django_get_or_create = ("name",)
@@ -96,14 +111,28 @@
     source = None
 
     class Meta:
         model = Parametrizer
         django_get_or_create = ("code",)
 
 
+class ReportDocumentFactory(DjangoModelFactory):
+    report = factory.SubFactory(ReportFactory)
+
+    class Meta:
+        model = ReportDocument
+
+    @classmethod
+    def create(cls, **kwargs: Dict) -> ReportDocument:
+        fmt = Formatter.objects.get(name="Queryset To HTML")
+        r: Report = ReportFactory(query=QueryFactory(), formatter=fmt)
+        r.execute(run_query=True)
+        return r.documents.first()
+
+
 def get_group(
     name: str = "Group1", permissions: Optional[List[Permission]] = None
 ) -> Group:
     group = GroupFactory(name)
     permission_names = permissions or []
     for permission_name in permission_names:
         try:
@@ -117,70 +146,7 @@
     except Permission.DoesNotExist:
         raise Permission.DoesNotExist(
             "Permission `{0}` does not exists", permission_name
         )
 
     group.permissions.add(permission)
     return group
-
-
-class user_grant_permission:
-    def __init__(
-        self, user: get_user_model(), permissions: Optional[List[Permission]] = None
-    ) -> None:
-        self.user = user
-        self.permissions = permissions
-        self.group: Optional[Group] = None
-
-    def __enter__(self) -> None:
-        if hasattr(self.user, "_group_perm_cache"):
-            del self.user._group_perm_cache
-        if hasattr(self.user, "_officepermissionchecker"):
-            del self.user._officepermissionchecker
-        if hasattr(self.user, "_perm_cache"):
-            del self.user._perm_cache
-        self.group = get_group(permissions=self.permissions or [])
-        self.user.groups.add(self.group)
-
-    def __exit__(self, e_typ: Any, e_val: Any, trcbak: Any) -> None:
-        if all((e_typ, e_val, trcbak)):
-            raise e_typ(e_val)
-        if self.group:
-            self.user.groups.remove(self.group)
-            self.group.delete()
-
-    def start(self) -> None:
-        """Activate a patch, returning any created mock."""
-        self.__enter__()
-
-    def stop(self) -> None:
-        """Stop an active patch."""
-        return self.__exit__(None, None, None)
-
-
-class DatasetFactory(DjangoModelFactory):
-    query = factory.SubFactory(QueryFactory)
-
-    class Meta:
-        model = Dataset
-        # django_get_or_create = ("name",)
-
-    @classmethod
-    def create(cls, **kwargs: Dict) -> Dataset:
-        # ret = super().create(**kwargs)
-        q: Query = cls.query.get_factory().create()
-        q.run(persist=True)
-        return q.datasets.first()
-
-
-class ReportDocumentFactory(DjangoModelFactory):
-    report = factory.SubFactory(ReportFactory)
-
-    class Meta:
-        model = ReportDocument
-
-    @classmethod
-    def create(cls, **kwargs: Dict) -> ReportDocument:
-        fmt = Formatter.objects.get(name="Queryset To HTML")
-        r: Report = ReportFactory(query=QueryFactory(), formatter=fmt)
-        r.execute(run_query=True)
-        return r.documents.first()
```

### Comparing `unicef-power-query-0.1/tests/test_admin.py` & `unicef-power-query-0.2/tests/test_admin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 from django.contrib.contenttypes.management import create_contenttypes
 from django.test import override_settings
 from django.urls import reverse
 
 from django_webtest import WebTest
 
 from power_query.defaults import create_defaults
-from power_query.models import Parametrizer, Query
-
-from .fixtures import (
+from power_query.fixtures import (
     DatasetFactory,
     FormatterFactory,
     ParametrizerFactory,
     QueryFactory,
     ReportDocumentFactory,
     ReportFactory,
     UserFactory,
 )
+from power_query.models import Parametrizer, Query
 
 
 @override_settings(POWER_QUERY_DB_ALIAS="default")
 class TestPowerQueryAdmin(WebTest):
     databases = {"default"}
 
     @classmethod
```

### Comparing `unicef-power-query-0.1/tests/test_auth.py` & `unicef-power-query-0.2/tests/test_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 from django.test import override_settings, TestCase
 from django.urls import reverse
 
 from power_query.defaults import create_defaults
-from power_query.models import Formatter, Query, Report
-
-from .fixtures import (
+from power_query.fixtures import (
     FormatterFactory,
     ParametrizerFactory,
     QueryFactory,
     ReportFactory,
     UserFactory,
 )
+from power_query.models import Formatter, Query, Report
 
 
 @override_settings(POWER_QUERY_DB_ALIAS="default")
 class TestPowerQuery(TestCase):
     databases = {"default"}
 
     @classmethod
```

### Comparing `unicef-power-query-0.1/tests/test_celery.py` & `unicef-power-query-0.2/tests/test_celery.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,23 +2,22 @@
 
 from power_query.celery_tasks import (
     refresh_report,
     refresh_reports,
     run_background_query,
 )
 from power_query.defaults import create_defaults
-from power_query.models import Formatter, Parametrizer, Query, Report
-
-from .fixtures import (
+from power_query.fixtures import (
     FormatterFactory,
     ParametrizerFactory,
     QueryFactory,
     ReportFactory,
     UserFactory,
 )
+from power_query.models import Formatter, Parametrizer, Query, Report
 
 
 @override_settings(POWER_QUERY_DB_ALIAS="default")
 class TestPowerQueryCelery(TestCase):
     databases = {"default"}
 
     @classmethod
```

### Comparing `unicef-power-query-0.1/tests/test_queries.py` & `unicef-power-query-0.2/tests/test_queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from django.test import override_settings, TestCase
 
 from power_query.defaults import create_defaults
-from power_query.models import Formatter, Query, Report
-
-from .fixtures import (
+from power_query.fixtures import (
     FormatterFactory,
     QueryFactory,
     ReportFactory,
     UserFactory,
 )
+from power_query.models import Formatter, Query, Report
 
 
 @override_settings(POWER_QUERY_DB_ALIAS="default")
 class TestPowerQuery(TestCase):
     databases = {"default"}
 
     @classmethod
```

### Comparing `unicef-power-query-0.1/tests/test_utils.py` & `unicef-power-query-0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `unicef-power-query-0.1/tox.ini` & `unicef-power-query-0.2/tox.ini`

 * *Files identical despite different names*

