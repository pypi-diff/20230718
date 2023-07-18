# Comparing `tmp/django-advanced-report-builder-0.4.0.tar.gz` & `tmp/django-advanced-report-builder-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-advanced-report-builder-0.4.0.tar", last modified: Wed Jun 21 09:39:30 2023, max compression
+gzip compressed data, was "django-advanced-report-builder-0.4.1.tar", last modified: Tue Jul 18 16:43:04 2023, max compression
```

## Comparing `django-advanced-report-builder-0.4.0.tar` & `django-advanced-report-builder-0.4.1.tar`

### file list

```diff
@@ -1,203 +1,204 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.979401 django-advanced-report-builder-0.4.0/
--rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/LICENSE
--rw-r--r--   0 tom        (501) staff       (20)       91 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)      683 2023-06-21 09:39:30.979218 django-advanced-report-builder-0.4.0/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      171 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.899229 django-advanced-report-builder-0.4.0/advanced_report_builder/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     4012 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/admin.py
--rw-r--r--   0 tom        (501) staff       (20)      218 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/apps.py
--rw-r--r--   0 tom        (501) staff       (20)     3394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/columns.py
--rw-r--r--   0 tom        (501) staff       (20)       40 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/customise.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.903054 django-advanced-report-builder-0.4.0/advanced_report_builder/data_merge/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/data_merge/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3830 2023-03-06 12:34:46.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/data_merge/utils.py
--rw-r--r--   0 tom        (501) staff       (20)      951 2023-03-29 16:03:43.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/data_merge/widget.py
--rw-r--r--   0 tom        (501) staff       (20)     5477 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/duplicate.py
--rw-r--r--   0 tom        (501) staff       (20)      192 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/exceptions.py
--rw-r--r--   0 tom        (501) staff       (20)    10853 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/field_types.py
--rw-r--r--   0 tom        (501) staff       (20)    13799 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/filter_query.py
--rw-r--r--   0 tom        (501) staff       (20)      439 2023-06-21 09:07:31.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/generate_series.py
--rw-r--r--   0 tom        (501) staff       (20)     8337 2023-06-21 09:29:22.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/globals.py
--rw-r--r--   0 tom        (501) staff       (20)     1308 2023-04-17 09:39:11.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/includes.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.911180 django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/
--rw-r--r--   0 tom        (501) staff       (20)    14109 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0001_initial.py
--rw-r--r--   0 tom        (501) staff       (20)      591 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0002_auto_20220209_1657.py
--rw-r--r--   0 tom        (501) staff       (20)     1734 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0003_auto_20220215_1219.py
--rw-r--r--   0 tom        (501) staff       (20)      955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0004_customreport.py
--rw-r--r--   0 tom        (501) staff       (20)     3623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0005_auto_20220303_0958.py
--rw-r--r--   0 tom        (501) staff       (20)      914 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0006_auto_20220310_1147.py
--rw-r--r--   0 tom        (501) staff       (20)      607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0007_auto_20220322_1939.py
--rw-r--r--   0 tom        (501) staff       (20)      827 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0008_auto_20220404_1144.py
--rw-r--r--   0 tom        (501) staff       (20)     2485 2023-04-28 15:54:41.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0009_auto_20230428_1554.py
--rw-r--r--   0 tom        (501) staff       (20)      596 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0010_auto_20230428_2033.py
--rw-r--r--   0 tom        (501) staff       (20)      659 2023-06-20 14:49:09.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0011_auto_20230620_1449.py
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    19881 2023-06-20 16:10:09.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/models.py
--rw-r--r--   0 tom        (501) staff       (20)      532 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/report_builder.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.877100 django-advanced-report-builder-0.4.0/advanced_report_builder/static/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.880507 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.877313 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.916806 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/
--rw-r--r--   0 tom        (501) staff       (20)   334540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js
--rw-r--r--   0 tom        (501) staff       (20)   405847 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js
--rw-r--r--   0 tom        (501) staff       (20)   193925 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js
--rw-r--r--   0 tom        (501) staff       (20)     1430 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js
--rw-r--r--   0 tom        (501) staff       (20)    12893 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.922617 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/
--rw-r--r--   0 tom        (501) staff       (20)    72125 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js
--rw-r--r--   0 tom        (501) staff       (20)     2352 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.877926 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/d3/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.926961 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/d3/js/
--rw-r--r--   0 tom        (501) staff       (20)   575002 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js
--rw-r--r--   0 tom        (501) staff       (20)   275533 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.877690 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.923985 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/
--rw-r--r--   0 tom        (501) staff       (20)   205600 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js
--rw-r--r--   0 tom        (501) staff       (20)    58945 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.878160 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dashboard/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.928042 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dashboard/js/
--rw-r--r--   0 tom        (501) staff       (20)      563 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.878399 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.932034 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/
--rwxr-xr-x   0 tom        (501) staff       (20)      578 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore
--rwxr-xr-x   0 tom        (501) staff       (20)      122 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/.travis.yml
--rwxr-xr-x   0 tom        (501) staff       (20)     1176 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt
--rwxr-xr-x   0 tom        (501) staff       (20)     3291 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/README.md
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.932426 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/bin/
--rwxr-xr-x   0 tom        (501) staff       (20)     1442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer
--rwxr-xr-x   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/bower.json
--rwxr-xr-x   0 tom        (501) staff       (20)     5175 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3374 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1758 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js
--rwxr-xr-x   0 tom        (501) staff       (20)     5190 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/index.js
--rwxr-xr-x   0 tom        (501) staff       (20)      920 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/package.json
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.880235 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.933918 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/
--rwxr-xr-x   0 tom        (501) staff       (20)     4390 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1324 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.881815 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.935842 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/
--rwxr-xr-x   0 tom        (501) staff       (20)     3765 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css
--rwxr-xr-x   0 tom        (501) staff       (20)     3253 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css
--rwxr-xr-x   0 tom        (501) staff       (20)     3756 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css
--rwxr-xr-x   0 tom        (501) staff       (20)     3248 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.947481 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/
--rwxr-xr-x   0 tom        (501) staff       (20)     2962 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3082 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2494 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1431 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2309 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3273 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2672 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2662 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3216 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2917 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2952 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2522 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2299 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1412 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2645 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2787 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2451 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js
--rwxr-xr-x   0 tom        (501) staff       (20)     1310 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2627 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2782 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js
--rwxr-xr-x   0 tom        (501) staff       (20)     3062 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js
--rwxr-xr-x   0 tom        (501) staff       (20)     2503 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.951481 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.881454 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.952313 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/
--rwxr-xr-x   0 tom        (501) staff       (20)     1212 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js
--rwxr-xr-x   0 tom        (501) staff       (20)   191499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js
--rwxr-xr-x   0 tom        (501) staff       (20)    72607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js
--rwxr-xr-x   0 tom        (501) staff       (20)   201158 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js
--rwxr-xr-x   0 tom        (501) staff       (20)    77072 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.953950 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/
--rwxr-xr-x   0 tom        (501) staff       (20)      442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/dark.scss
--rwxr-xr-x   0 tom        (501) staff       (20)     3887 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.958471 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/
--rwxr-xr-x   0 tom        (501) staff       (20)      266 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-checkbox.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-tooltip-errors.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss
--rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_invert.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      469 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_sortable.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/bt-tooltip-errors.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss
--rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/invert.scss
--rwxr-xr-x   0 tom        (501) staff       (20)      465 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/sortable.scss
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.882808 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.959428 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.961135 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.961557 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/bar/
--rw-r--r--   0 tom        (501) staff       (20)     5295 2023-06-21 09:32:32.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.962362 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/
--rw-r--r--   0 tom        (501) staff       (20)     1362 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html
--rw-r--r--   0 tom        (501) staff       (20)     1007 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.962808 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/line/
--rw-r--r--   0 tom        (501) staff       (20)     4020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      486 2023-04-26 11:14:19.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/modal.html
--rw-r--r--   0 tom        (501) staff       (20)      270 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/modal_field.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.963266 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/pie/
--rw-r--r--   0 tom        (501) staff       (20)     2084 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      858 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/report.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.963634 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/data_merge/
--rw-r--r--   0 tom        (501) staff       (20)     2975 2023-03-29 15:59:37.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.965697 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/datatables/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.966395 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/
--rw-r--r--   0 tom        (501) staff       (20)      254 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/modal.html
--rw-r--r--   0 tom        (501) staff       (20)     3320 2023-04-26 11:10:44.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html
--rw-r--r--   0 tom        (501) staff       (20)      377 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/datatables/modal.html
--rw-r--r--   0 tom        (501) staff       (20)      593 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html
--rw-r--r--   0 tom        (501) staff       (20)      256 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/datatables/query_modal.html
--rw-r--r--   0 tom        (501) staff       (20)     1127 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/datatables/report.html
--rw-r--r--   0 tom        (501) staff       (20)     8185 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.967909 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/kanban/
--rw-r--r--   0 tom        (501) staff       (20)      499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/kanban/description_modal.html
--rw-r--r--   0 tom        (501) staff       (20)     2038 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      308 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/kanban/modal.html
--rw-r--r--   0 tom        (501) staff       (20)     1961 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/kanban/report.html
--rw-r--r--   0 tom        (501) staff       (20)     3467 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/query_builder.html
--rw-r--r--   0 tom        (501) staff       (20)    10552 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/select_column.html
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.968876 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/single_values/
--rw-r--r--   0 tom        (501) staff       (20)     1896 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html
--rw-r--r--   0 tom        (501) staff       (20)      623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html
--rw-r--r--   0 tom        (501) staff       (20)     1643 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/single_values/report.html
--rw-r--r--   0 tom        (501) staff       (20)      327 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/toggle.py
--rw-r--r--   0 tom        (501) staff       (20)     4223 2023-06-07 08:15:03.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/urls.py
--rw-r--r--   0 tom        (501) staff       (20)     4446 2023-06-21 08:33:34.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/utils.py
--rw-r--r--   0 tom        (501) staff       (20)    12521 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/variable_date.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.974514 django-advanced-report-builder-0.4.0/advanced_report_builder/views/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)    25874 2023-06-21 09:37:24.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/bar_charts.py
--rw-r--r--   0 tom        (501) staff       (20)    18240 2023-04-28 15:13:27.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/charts_base.py
--rw-r--r--   0 tom        (501) staff       (20)     3020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/custom.py
--rw-r--r--   0 tom        (501) staff       (20)     8659 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/dashboard.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.976034 django-advanced-report-builder-0.4.0/advanced_report_builder/views/datatables/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/datatables/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     6801 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/datatables/datatables.py
--rw-r--r--   0 tom        (501) staff       (20)    25731 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/datatables/modal.py
--rw-r--r--   0 tom        (501) staff       (20)    11394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/datatables/utils.py
--rw-r--r--   0 tom        (501) staff       (20)     8792 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/funnel_charts.py
--rw-r--r--   0 tom        (501) staff       (20)    32161 2023-03-29 16:04:49.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/kanban.py
--rw-r--r--   0 tom        (501) staff       (20)    13046 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/line_charts.py
--rw-r--r--   0 tom        (501) staff       (20)    21031 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/modals_base.py
--rw-r--r--   0 tom        (501) staff       (20)     8753 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/pie_charts.py
--rw-r--r--   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/report.py
--rw-r--r--   0 tom        (501) staff       (20)     8210 2023-04-28 13:58:37.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/report_utils_mixin.py
--rw-r--r--   0 tom        (501) staff       (20)     4750 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/reports.py
--rw-r--r--   0 tom        (501) staff       (20)    22923 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/single_values.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.977099 django-advanced-report-builder-0.4.0/advanced_report_builder/views/targets/
--rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/targets/__init__.py
--rw-r--r--   0 tom        (501) staff       (20)     3021 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/targets/utils.py
--rw-r--r--   0 tom        (501) staff       (20)      898 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.0/advanced_report_builder/views/targets/views.py
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-06-21 09:39:30.978843 django-advanced-report-builder-0.4.0/django_advanced_report_builder.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)      683 2023-06-21 09:39:30.000000 django-advanced-report-builder-0.4.0/django_advanced_report_builder.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)    11063 2023-06-21 09:39:30.000000 django-advanced-report-builder-0.4.0/django_advanced_report_builder.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        1 2023-06-21 09:39:30.000000 django-advanced-report-builder-0.4.0/django_advanced_report_builder.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)      149 2023-06-21 09:39:30.000000 django-advanced-report-builder-0.4.0/django_advanced_report_builder.egg-info/requires.txt
--rw-r--r--   0 tom        (501) staff       (20)       24 2023-06-21 09:39:30.000000 django-advanced-report-builder-0.4.0/django_advanced_report_builder.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)       38 2023-06-21 09:39:30.979463 django-advanced-report-builder-0.4.0/setup.cfg
--rw-r--r--   0 tom        (501) staff       (20)      974 2023-06-21 09:39:19.000000 django-advanced-report-builder-0.4.0/setup.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.975604 django-advanced-report-builder-0.4.1/
+-rw-r--r--   0 tom        (501) staff       (20)     1069 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/LICENSE
+-rw-r--r--   0 tom        (501) staff       (20)       91 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)      683 2023-07-18 16:43:04.975478 django-advanced-report-builder-0.4.1/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      171 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.949686 django-advanced-report-builder-0.4.1/advanced_report_builder/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     4012 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/admin.py
+-rw-r--r--   0 tom        (501) staff       (20)      218 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/apps.py
+-rw-r--r--   0 tom        (501) staff       (20)     3394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/columns.py
+-rw-r--r--   0 tom        (501) staff       (20)       40 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/customise.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.950242 django-advanced-report-builder-0.4.1/advanced_report_builder/data_merge/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/data_merge/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3830 2023-03-06 12:34:46.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/data_merge/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)      951 2023-03-29 16:03:43.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/data_merge/widget.py
+-rw-r--r--   0 tom        (501) staff       (20)     5477 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/duplicate.py
+-rw-r--r--   0 tom        (501) staff       (20)      192 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/exceptions.py
+-rw-r--r--   0 tom        (501) staff       (20)    10853 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/field_types.py
+-rw-r--r--   0 tom        (501) staff       (20)    13799 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/filter_query.py
+-rw-r--r--   0 tom        (501) staff       (20)      439 2023-06-21 09:07:31.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/generate_series.py
+-rw-r--r--   0 tom        (501) staff       (20)     8337 2023-06-21 09:29:22.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/globals.py
+-rw-r--r--   0 tom        (501) staff       (20)     1308 2023-04-17 09:39:11.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/includes.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.952369 django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/
+-rw-r--r--   0 tom        (501) staff       (20)    14109 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0001_initial.py
+-rw-r--r--   0 tom        (501) staff       (20)      591 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0002_auto_20220209_1657.py
+-rw-r--r--   0 tom        (501) staff       (20)     1734 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0003_auto_20220215_1219.py
+-rw-r--r--   0 tom        (501) staff       (20)      955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0004_customreport.py
+-rw-r--r--   0 tom        (501) staff       (20)     3623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0005_auto_20220303_0958.py
+-rw-r--r--   0 tom        (501) staff       (20)      914 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0006_auto_20220310_1147.py
+-rw-r--r--   0 tom        (501) staff       (20)      607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0007_auto_20220322_1939.py
+-rw-r--r--   0 tom        (501) staff       (20)      827 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0008_auto_20220404_1144.py
+-rw-r--r--   0 tom        (501) staff       (20)     2485 2023-04-28 15:54:41.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0009_auto_20230428_1554.py
+-rw-r--r--   0 tom        (501) staff       (20)      596 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0010_auto_20230428_2033.py
+-rw-r--r--   0 tom        (501) staff       (20)      659 2023-06-20 14:49:09.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0011_auto_20230620_1449.py
+-rw-r--r--   0 tom        (501) staff       (20)      767 2023-07-18 16:42:15.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0012_auto_20230718_1642.py
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    19894 2023-07-18 16:42:07.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/models.py
+-rw-r--r--   0 tom        (501) staff       (20)      532 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/report_builder.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.943520 django-advanced-report-builder-0.4.1/advanced_report_builder/static/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.944337 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.943603 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.954696 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/
+-rw-r--r--   0 tom        (501) staff       (20)   334540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js
+-rw-r--r--   0 tom        (501) staff       (20)   405847 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js
+-rw-r--r--   0 tom        (501) staff       (20)   193925 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js
+-rw-r--r--   0 tom        (501) staff       (20)     1430 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js
+-rw-r--r--   0 tom        (501) staff       (20)    12893 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.954886 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/
+-rw-r--r--   0 tom        (501) staff       (20)    72125 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js
+-rw-r--r--   0 tom        (501) staff       (20)     2352 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.943880 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/d3/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.956740 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/d3/js/
+-rw-r--r--   0 tom        (501) staff       (20)   575002 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js
+-rw-r--r--   0 tom        (501) staff       (20)   275533 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.943776 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.955462 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/
+-rw-r--r--   0 tom        (501) staff       (20)   205600 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js
+-rw-r--r--   0 tom        (501) staff       (20)    58945 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.943986 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dashboard/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.957388 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dashboard/js/
+-rw-r--r--   0 tom        (501) staff       (20)      563 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.944095 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.958713 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/
+-rwxr-xr-x   0 tom        (501) staff       (20)      578 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore
+-rwxr-xr-x   0 tom        (501) staff       (20)      122 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/.travis.yml
+-rwxr-xr-x   0 tom        (501) staff       (20)     1176 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt
+-rwxr-xr-x   0 tom        (501) staff       (20)     3291 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/README.md
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.958852 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/bin/
+-rwxr-xr-x   0 tom        (501) staff       (20)     1442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer
+-rwxr-xr-x   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/bower.json
+-rwxr-xr-x   0 tom        (501) staff       (20)     5175 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3374 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1758 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     5190 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/index.js
+-rwxr-xr-x   0 tom        (501) staff       (20)      920 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/package.json
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.944270 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.959128 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/
+-rwxr-xr-x   0 tom        (501) staff       (20)     4390 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1324 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.944666 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.959684 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/
+-rwxr-xr-x   0 tom        (501) staff       (20)     3765 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css
+-rwxr-xr-x   0 tom        (501) staff       (20)     3253 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css
+-rwxr-xr-x   0 tom        (501) staff       (20)     3756 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css
+-rwxr-xr-x   0 tom        (501) staff       (20)     3248 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.962988 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/
+-rwxr-xr-x   0 tom        (501) staff       (20)     2962 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2540 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3082 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2494 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1431 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2309 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3273 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2672 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2662 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3216 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2917 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2952 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2522 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2299 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1412 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2645 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2787 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2451 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     1310 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2955 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2627 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2782 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     3062 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js
+-rwxr-xr-x   0 tom        (501) staff       (20)     2503 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.964587 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.944605 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.964823 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/
+-rwxr-xr-x   0 tom        (501) staff       (20)     1212 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js
+-rwxr-xr-x   0 tom        (501) staff       (20)   191499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js
+-rwxr-xr-x   0 tom        (501) staff       (20)    72607 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js
+-rwxr-xr-x   0 tom        (501) staff       (20)   201158 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js
+-rwxr-xr-x   0 tom        (501) staff       (20)    77072 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.965090 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/
+-rwxr-xr-x   0 tom        (501) staff       (20)      442 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/dark.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)     3887 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.966596 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/
+-rwxr-xr-x   0 tom        (501) staff       (20)      266 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-checkbox.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_bt-tooltip-errors.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_invert.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      469 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_sortable.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      194 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/bt-tooltip-errors.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      616 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)       83 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/invert.scss
+-rwxr-xr-x   0 tom        (501) staff       (20)      465 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/sortable.scss
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.944836 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.966972 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.967513 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.967775 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/bar/
+-rw-r--r--   0 tom        (501) staff       (20)     5295 2023-06-21 09:32:32.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.968154 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/funnel/
+-rw-r--r--   0 tom        (501) staff       (20)     1362 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)     1007 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.968341 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/line/
+-rw-r--r--   0 tom        (501) staff       (20)     4020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      486 2023-04-26 11:14:19.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)      270 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/modal_field.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.968504 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/pie/
+-rw-r--r--   0 tom        (501) staff       (20)     2084 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      858 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/report.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.968665 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/data_merge/
+-rw-r--r--   0 tom        (501) staff       (20)     2975 2023-03-29 15:59:37.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.969505 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/datatables/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.969820 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/datatables/fields/
+-rw-r--r--   0 tom        (501) staff       (20)      254 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/datatables/fields/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     3320 2023-04-26 11:10:44.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html
+-rw-r--r--   0 tom        (501) staff       (20)      377 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/datatables/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)      593 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html
+-rw-r--r--   0 tom        (501) staff       (20)      256 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/datatables/query_modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     1127 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/datatables/report.html
+-rw-r--r--   0 tom        (501) staff       (20)     8185 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.970508 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/kanban/
+-rw-r--r--   0 tom        (501) staff       (20)      499 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/kanban/description_modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     2038 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      308 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/kanban/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     1961 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/kanban/report.html
+-rw-r--r--   0 tom        (501) staff       (20)     3467 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/query_builder.html
+-rw-r--r--   0 tom        (501) staff       (20)    10552 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/select_column.html
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.970947 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/single_values/
+-rw-r--r--   0 tom        (501) staff       (20)     1896 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html
+-rw-r--r--   0 tom        (501) staff       (20)      623 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html
+-rw-r--r--   0 tom        (501) staff       (20)     1643 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/single_values/report.html
+-rw-r--r--   0 tom        (501) staff       (20)      327 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/toggle.py
+-rw-r--r--   0 tom        (501) staff       (20)     4223 2023-06-07 08:15:03.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/urls.py
+-rw-r--r--   0 tom        (501) staff       (20)     4446 2023-06-21 08:33:34.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)    12521 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/variable_date.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.973761 django-advanced-report-builder-0.4.1/advanced_report_builder/views/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)    25874 2023-06-21 09:37:24.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/bar_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)    18240 2023-04-28 15:13:27.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/charts_base.py
+-rw-r--r--   0 tom        (501) staff       (20)     3020 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/custom.py
+-rw-r--r--   0 tom        (501) staff       (20)     8659 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/dashboard.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.974371 django-advanced-report-builder-0.4.1/advanced_report_builder/views/datatables/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/datatables/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     6801 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/datatables/datatables.py
+-rw-r--r--   0 tom        (501) staff       (20)    25731 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/datatables/modal.py
+-rw-r--r--   0 tom        (501) staff       (20)    11394 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/datatables/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)     8792 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/funnel_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)    32161 2023-03-29 16:04:49.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/kanban.py
+-rw-r--r--   0 tom        (501) staff       (20)    13046 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/line_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)    21031 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/modals_base.py
+-rw-r--r--   0 tom        (501) staff       (20)     8753 2023-06-06 20:57:13.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/pie_charts.py
+-rw-r--r--   0 tom        (501) staff       (20)      443 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/report.py
+-rw-r--r--   0 tom        (501) staff       (20)     8210 2023-04-28 13:58:37.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/report_utils_mixin.py
+-rw-r--r--   0 tom        (501) staff       (20)     4750 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/reports.py
+-rw-r--r--   0 tom        (501) staff       (20)    22873 2023-07-18 16:39:40.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/single_values.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.974752 django-advanced-report-builder-0.4.1/advanced_report_builder/views/targets/
+-rw-r--r--   0 tom        (501) staff       (20)        0 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/targets/__init__.py
+-rw-r--r--   0 tom        (501) staff       (20)     3021 2023-01-17 17:02:06.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/targets/utils.py
+-rw-r--r--   0 tom        (501) staff       (20)      786 2023-07-18 16:39:39.000000 django-advanced-report-builder-0.4.1/advanced_report_builder/views/targets/views.py
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2023-07-18 16:43:04.975303 django-advanced-report-builder-0.4.1/django_advanced_report_builder.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)      683 2023-07-18 16:43:04.000000 django-advanced-report-builder-0.4.1/django_advanced_report_builder.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)    11125 2023-07-18 16:43:04.000000 django-advanced-report-builder-0.4.1/django_advanced_report_builder.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        1 2023-07-18 16:43:04.000000 django-advanced-report-builder-0.4.1/django_advanced_report_builder.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)      149 2023-07-18 16:43:04.000000 django-advanced-report-builder-0.4.1/django_advanced_report_builder.egg-info/requires.txt
+-rw-r--r--   0 tom        (501) staff       (20)       24 2023-07-18 16:43:04.000000 django-advanced-report-builder-0.4.1/django_advanced_report_builder.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)       38 2023-07-18 16:43:04.975645 django-advanced-report-builder-0.4.1/setup.cfg
+-rw-r--r--   0 tom        (501) staff       (20)      974 2023-07-18 16:42:37.000000 django-advanced-report-builder-0.4.1/setup.py
```

### Comparing `django-advanced-report-builder-0.4.0/LICENSE` & `django-advanced-report-builder-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/PKG-INFO` & `django-advanced-report-builder-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-report-builder
-Version: 0.4.0
+Version: 0.4.1
 Summary: Django app that allows you to build reports from modals
 Home-page: https://github.com/django-advance-utils/django-advanced-report-builder
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/admin.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/admin.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/columns.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/columns.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/data_merge/utils.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/data_merge/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/data_merge/widget.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/data_merge/widget.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/duplicate.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/duplicate.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/field_types.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/field_types.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/filter_query.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/filter_query.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/globals.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/globals.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/includes.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/includes.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0001_initial.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0002_auto_20220209_1657.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0002_auto_20220209_1657.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0003_auto_20220215_1219.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0003_auto_20220215_1219.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0004_customreport.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0004_customreport.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0005_auto_20220303_0958.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0005_auto_20220303_0958.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0006_auto_20220310_1147.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0006_auto_20220310_1147.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0007_auto_20220322_1939.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0007_auto_20220322_1939.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0008_auto_20220404_1144.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0008_auto_20220404_1144.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0009_auto_20230428_1554.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0009_auto_20230428_1554.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0010_auto_20230428_2033.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0010_auto_20230428_2033.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/migrations/0011_auto_20230620_1449.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/migrations/0011_auto_20230620_1449.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/models.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 from django.utils.dates import MONTHS
 from django_datatables.columns import DatatableColumn, NoHeadingColumn, ManyToManyColumn
 from django_datatables.model_def import DatatableModel
 from time_stamped_model.models import TimeStampedModel
+from django_modals.model_fields.colour import ColourField
 
 from advanced_report_builder.globals import DISPLAY_OPTION_CHOICES, DISPLAY_OPTION_2_PER_ROW, DISPLAY_OPTION_NONE, \
     DISPLAY_OPTION_CLASSES, ANNOTATION_VALUE_CHOICES, ANNOTATIONS_CHOICES, ANNOTATION_CHOICE_COUNT, \
     ANNOTATION_CHART_SCALE
 
 
 class Target(TimeStampedModel):
@@ -20,16 +21,16 @@
         (TARGET_TYPE_MONEY, 'Money'),
         (TARGET_TYPE_PERCENTAGE, 'Percentage'),
     )
 
     slug = models.SlugField(unique=True)
     name = models.CharField(max_length=64)
     target_type = models.PositiveSmallIntegerField(choices=TARGET_TYPE_CHOICES)
-    colour = models.CharField(max_length=10, null=True, blank=True,
-                              help_text='The colour when it gets displayed on a report')
+    colour = ColourField(null=True, blank=True,
+                         help_text='The colour when it gets displayed on a report')
     default_value = models.IntegerField(blank=True, null=True)
     default_percentage = models.FloatField(blank=True, null=True)
     overridden = models.BooleanField(default=False)
     override_data = models.JSONField(null=True, blank=True)
 
     def get_value(self):
         if self.target_type == self.TARGET_TYPE_PERCENTAGE:
@@ -244,15 +245,15 @@
         (SINGLE_VALUE_TYPE_COUNT_AND_SUM, 'Count & Sum'),
         (SINGLE_VALUE_TYPE_PERCENT, 'Percent'),
         (SINGLE_VALUE_TYPE_PERCENT_FROM_COUNT, 'Percent from Count'),
         (SINGLE_VALUE_TYPE_AVERAGE_SUM_FROM_COUNT, 'Average Sum from Count'),
         (SINGLE_VALUE_TYPE_AVERAGE_SUM_OVER_TIME, 'Average Sum over Time')
     )
 
-    tile_colour = models.CharField(max_length=10, blank=True, null=True)
+    tile_colour = ColourField(blank=True, null=True)
     field = models.CharField(max_length=200, blank=True, null=True)  # denominator
     numerator = models.CharField(max_length=200, blank=True, null=True)
     single_value_type = models.PositiveSmallIntegerField(choices=SINGLE_VALUE_TYPE_CHOICES,
                                                          default=SINGLE_VALUE_TYPE_COUNT)
     prefix = models.CharField(max_length=64, blank=True, null=True)
     decimal_places = models.IntegerField(default=0)
     show_breakdown = models.BooleanField(default=False)
```

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/report_builder.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/report_builder.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/chunks/helpers.segment.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/d3/js/d3.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/d3/js/d3.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/d3-funnel/js/d3-funnel.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dashboard/js/dashboard.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/.gitignore`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/LICENSE-DOT.txt`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/README.md` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/README.md`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/bin/dot-packer`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/doT.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/doT.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/doU.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/index.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/index.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/dot/js/package.json` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/dot/js/package.json`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/jquery_extendext/js/jQuery.extendext.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.dark.min.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/css/query-builder.default.min.css`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ar.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.az.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.bg.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.cs.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.da.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.de.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.el.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.en.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.es.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fa-IR.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.fr.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.he.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.it.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.nl.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.no.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pl.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-BR.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.pt-PT.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ro.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ru.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.sq.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.tr.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.ua.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/i18n/query-builder.zh-CN.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/plugins/currency/plugin.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/js/query-builder.standalone.min.js`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/default.scss`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/_filter-description.scss`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss` & `django-advanced-report-builder-0.4.1/advanced_report_builder/static/advanced_report_builder/query_builder/scss/plugins/filter-description.scss`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/bar/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/funnel/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/funnel/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/line/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/pie/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/charts/report.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/charts/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/data_merge/data_merge.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/datatables/fields/single_query_builder.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/datatables/onclick_menu.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/datatables/report.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/datatables/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/datatables/select_pivot.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/kanban/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/kanban/report.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/kanban/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/query_builder.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/query_builder.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/select_column.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/select_column.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/single_values/middle.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/single_values/modal.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/templates/advanced_report_builder/single_values/report.html` & `django-advanced-report-builder-0.4.1/advanced_report_builder/templates/advanced_report_builder/single_values/report.html`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/urls.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/urls.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/utils.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/variable_date.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/variable_date.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/bar_charts.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/bar_charts.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/charts_base.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/charts_base.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/custom.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/custom.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/dashboard.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/dashboard.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/datatables/datatables.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/datatables/datatables.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/datatables/modal.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/datatables/modal.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/datatables/utils.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/datatables/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/funnel_charts.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/funnel_charts.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/kanban.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/kanban.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/line_charts.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/line_charts.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/modals_base.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/modals_base.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/pie_charts.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/pie_charts.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/report_utils_mixin.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/report_utils_mixin.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/reports.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/reports.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/single_values.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/single_values.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,16 +259,15 @@
 
 
 class SingleValueModal(QueryBuilderModalBase):
     template_name = 'advanced_report_builder/single_values/modal.html'
     process = PROCESS_EDIT_DELETE
     permission_delete = PERMISSION_OFF
     model = SingleValueReport
-    widgets = {'tile_colour': ColourPickerWidget,
-               'report_tags': Select2Multiple,
+    widgets = {'report_tags': Select2Multiple,
                'show_breakdown': Toggle(attrs={'data-onstyle': 'success', 'data-on': 'YES', 'data-off': 'NO'})}
 
     form_fields = ['name',
                    'notes',
                    'report_type',
                    'report_tags',
                    ('single_value_type', {'label': 'Value type'}),
```

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/targets/utils.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/targets/utils.py`

 * *Files identical despite different names*

### Comparing `django-advanced-report-builder-0.4.0/advanced_report_builder/views/targets/views.py` & `django-advanced-report-builder-0.4.1/advanced_report_builder/views/targets/views.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,23 +1,21 @@
+from django.conf import settings
 from django.urls import reverse
 from django_modals.modals import ModelFormModal
 from django_modals.processes import PROCESS_EDIT_DELETE, PERMISSION_OFF
-from django_modals.widgets.colour_picker import ColourPickerWidget
 
 from advanced_report_builder.models import Target
-from django.conf import settings
 
 
 class TargetModal(ModelFormModal):
     model = Target
     form_fields = ['name',
                    'target_type',
                    'colour',
                    'default_value']
-    widgets = {'colour': ColourPickerWidget}
 
     process = PROCESS_EDIT_DELETE
     permission_delete = PERMISSION_OFF
 
     def post_save(self, created, form):
         if created:
             url_name = getattr(settings, 'REPORT_BUILDER_TARGET_URL_NAME', '')
```

### Comparing `django-advanced-report-builder-0.4.0/django_advanced_report_builder.egg-info/PKG-INFO` & `django-advanced-report-builder-0.4.1/django_advanced_report_builder.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-advanced-report-builder
-Version: 0.4.0
+Version: 0.4.1
 Summary: Django app that allows you to build reports from modals
 Home-page: https://github.com/django-advance-utils/django-advanced-report-builder
 Author: Thomas Turner
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `django-advanced-report-builder-0.4.0/django_advanced_report_builder.egg-info/SOURCES.txt` & `django-advanced-report-builder-0.4.1/django_advanced_report_builder.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 advanced_report_builder/migrations/0005_auto_20220303_0958.py
 advanced_report_builder/migrations/0006_auto_20220310_1147.py
 advanced_report_builder/migrations/0007_auto_20220322_1939.py
 advanced_report_builder/migrations/0008_auto_20220404_1144.py
 advanced_report_builder/migrations/0009_auto_20230428_1554.py
 advanced_report_builder/migrations/0010_auto_20230428_2033.py
 advanced_report_builder/migrations/0011_auto_20230620_1449.py
+advanced_report_builder/migrations/0012_auto_20230718_1642.py
 advanced_report_builder/migrations/__init__.py
 advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.esm.js
 advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.js
 advanced_report_builder/static/advanced_report_builder/chart-js/js/chart.min.js
 advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-adapter-moment.min.js
 advanced_report_builder/static/advanced_report_builder/chart-js/js/chartjs-plugin-datalabels.min.js
 advanced_report_builder/static/advanced_report_builder/chart-js/js/helpers.esm.js
```

### Comparing `django-advanced-report-builder-0.4.0/setup.py` & `django-advanced-report-builder-0.4.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="django-advanced-report-builder",
-    version="0.4.0",
+    version="0.4.1",
     author="Thomas Turner",
     description="Django app that allows you to build reports from modals",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/django-advance-utils/django-advanced-report-builder",
     include_package_data=True,
     packages=['advanced_report_builder'],
```

