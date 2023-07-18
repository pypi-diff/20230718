# Comparing `tmp/ora2-5.1.1.tar.gz` & `tmp/ora2-5.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ora2-5.1.1.tar", last modified: Wed Jul 12 07:38:46 2023, max compression
+gzip compressed data, was "ora2-5.2.0.tar", last modified: Tue Jul 18 18:44:56 2023, max compression
```

## Comparing `ora2-5.1.1.tar` & `ora2-5.2.0.tar`

### file list

```diff
@@ -1,558 +1,558 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.305351 ora2-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)    35135 2023-07-12 07:38:42.000000 ora2-5.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      682 2023-07-12 07:38:42.000000 ora2-5.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-07-12 07:38:46.305351 ora2-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-07-12 07:38:42.000000 ora2-5.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.189349 ora2-5.1.1/openassessment/
--rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.193349 ora2-5.1.1/openassessment/assessment/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5633 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.193349 ora2-5.1.1/openassessment/assessment/api/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    39052 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/api/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/api/self.py
--rw-r--r--   0 runner    (1001) docker     (122)    16433 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/api/staff.py
--rw-r--r--   0 runner    (1001) docker     (122)    16864 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/api/student_training.py
--rw-r--r--   0 runner    (1001) docker     (122)    12955 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/api/teams.py
--rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/data_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.193349 ora2-5.1.1/openassessment/assessment/errors/
--rw-r--r--   0 runner    (1001) docker     (122)      182 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      189 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/errors/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/errors/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/errors/self.py
--rw-r--r--   0 runner    (1001) docker     (122)      821 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/errors/staff.py
--rw-r--r--   0 runner    (1001) docker     (122)      440 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/errors/student_training.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.193349 ora2-5.1.1/openassessment/assessment/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     9361 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/migrations/0002_staffworkflow.py
--rw-r--r--   0 runner    (1001) docker     (122)      750 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/migrations/0003_expand_course_id.py
--rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py
--rw-r--r--   0 runner    (1001) docker     (122)      618 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py
--rw-r--r--   0 runner    (1001) docker     (122)      744 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/migrations/0006_TeamWorkflows.py
--rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/migrations/0007_staff_workflow_blank.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.193349 ora2-5.1.1/openassessment/assessment/models/
--rw-r--r--   0 runner    (1001) docker     (122)      205 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    32191 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/models/base.py
--rw-r--r--   0 runner    (1001) docker     (122)    22340 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/models/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)     8558 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/models/staff.py
--rw-r--r--   0 runner    (1001) docker     (122)     8200 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/models/student_training.py
--rw-r--r--   0 runner    (1001) docker     (122)     4991 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/models/training.py
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/score_type_constants.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.197349 ora2-5.1.1/openassessment/assessment/serializers/
--rw-r--r--   0 runner    (1001) docker     (122)      151 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/serializers/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/serializers/peer.py
--rw-r--r--   0 runner    (1001) docker     (122)     6217 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/serializers/training.py
--rw-r--r--   0 runner    (1001) docker     (122)      376 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/signals.py
--rw-r--r--   0 runner    (1001) docker     (122)      265 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)     1874 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/assessment/views.py
--rw-r--r--   0 runner    (1001) docker     (122)    58992 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.197349 ora2-5.1.1/openassessment/fileupload/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/fileupload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    23578 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/fileupload/api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.197349 ora2-5.1.1/openassessment/fileupload/backends/
--rw-r--r--   0 runner    (1001) docker     (122)      849 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/fileupload/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5253 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/fileupload/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/fileupload/backends/django_storage.py
--rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/fileupload/backends/filesystem.py
--rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/fileupload/backends/s3.py
--rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/fileupload/backends/swift.py
--rw-r--r--   0 runner    (1001) docker     (122)      740 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/fileupload/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      412 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/fileupload/urls.py
--rw-r--r--   0 runner    (1001) docker     (122)      498 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/fileupload/views_django_storage.py
--rw-r--r--   0 runner    (1001) docker     (122)     5105 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/fileupload/views_filesystem.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.197349 ora2-5.1.1/openassessment/locale/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.197349 ora2-5.1.1/openassessment/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    82260 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   137572 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ar/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29332 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ar/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/ar_SA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.197349 ora2-5.1.1/openassessment/locale/ar_SA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9218 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28056 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/de_DE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.201350 ora2-5.1.1/openassessment/locale/de_DE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    64223 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   124947 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8402 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27871 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/el/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.201350 ora2-5.1.1/openassessment/locale/el/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    35998 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/el/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   116285 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/el/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/el/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26850 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/el/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.201350 ora2-5.1.1/openassessment/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    84892 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      425 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/en/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27184 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/en/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/eo/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.205350 ora2-5.1.1/openassessment/locale/eo/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)   145884 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/eo/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   186603 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/eo/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    22487 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/eo/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    42004 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/eo/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/es_419/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.205350 ora2-5.1.1/openassessment/locale/es_419/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81996 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/es_419/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   133250 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/es_419/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11545 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29006 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/es_419/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/es_AR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.205350 ora2-5.1.1/openassessment/locale/es_AR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    11444 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28411 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/es_ES/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.205350 ora2-5.1.1/openassessment/locale/es_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    82594 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/es_ES/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   133560 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/es_ES/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11635 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29042 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/eu_ES/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.205350 ora2-5.1.1/openassessment/locale/eu_ES/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    14552 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/eu_ES/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   100050 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/eu_ES/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25057 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/fa_IR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.205350 ora2-5.1.1/openassessment/locale/fa_IR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    92564 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/fa_IR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   142763 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/fa_IR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    13499 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    30711 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.209350 ora2-5.1.1/openassessment/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81340 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   133090 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/fr/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/fr/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/fr_CA/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.209350 ora2-5.1.1/openassessment/locale/fr_CA/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    82568 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/fr_CA/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   136626 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/fr_CA/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    31089 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/he/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.209350 ora2-5.1.1/openassessment/locale/he/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    48842 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/he/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   117773 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/he/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     7008 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/he/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27047 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/he/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/hi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.209350 ora2-5.1.1/openassessment/locale/hi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/hi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95113 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/hi/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/hi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24633 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/hi/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/id/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.209350 ora2-5.1.1/openassessment/locale/id/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    40204 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/id/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   112010 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/id/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6748 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/id/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26550 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/id/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/it_IT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.213350 ora2-5.1.1/openassessment/locale/it_IT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81986 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/it_IT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   132727 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/it_IT/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11586 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28920 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/ja_JP/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.213350 ora2-5.1.1/openassessment/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    50706 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   118496 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ja_JP/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     7079 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27020 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/ka/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.213350 ora2-5.1.1/openassessment/locale/ka/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    77213 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ka/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   144721 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ka/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8953 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ka/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ka/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/lt_LT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.213350 ora2-5.1.1/openassessment/locale/lt_LT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    19263 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/lt_LT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   102318 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/lt_LT/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24738 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/lv/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.213350 ora2-5.1.1/openassessment/locale/lv/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/lv/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    94833 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/lv/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      962 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/lv/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23895 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/lv/LC_MESSAGES/djangojs.po
--rw-r--r--   0 runner    (1001) docker     (122)     6039 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/messages.mo
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/mn/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.217350 ora2-5.1.1/openassessment/locale/mn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/mn/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95311 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/mn/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/mn/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    22473 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/mn/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/nb/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.217350 ora2-5.1.1/openassessment/locale/nb/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     7793 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    97392 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6672 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/nb/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26384 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/nb/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.217350 ora2-5.1.1/openassessment/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    51135 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   117244 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/pl/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26637 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/pl/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/pt_BR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.217350 ora2-5.1.1/openassessment/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    32487 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   109420 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     5663 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26740 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/pt_PT/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.221350 ora2-5.1.1/openassessment/locale/pt_PT/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    81743 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/pt_PT/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   132378 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/pt_PT/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)    11556 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    29200 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/ro/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.221350 ora2-5.1.1/openassessment/locale/ro/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95431 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ro/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    24522 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ro/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.221350 ora2-5.1.1/openassessment/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    59971 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   128218 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8622 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ru/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28603 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/ru/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/sk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.221350 ora2-5.1.1/openassessment/locale/sk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     4054 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/sk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25387 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/sk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.221350 ora2-5.1.1/openassessment/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/sq/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    95372 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/sq/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/sq/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    23998 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/sq/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.185349 ora2-5.1.1/openassessment/locale/sw_KE/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.225350 ora2-5.1.1/openassessment/locale/sw_KE/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    43322 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/sw_KE/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   111947 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/sw_KE/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6441 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26486 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.189349 ora2-5.1.1/openassessment/locale/th/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.225350 ora2-5.1.1/openassessment/locale/th/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    27854 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/th/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   111076 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/th/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/th/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26116 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/th/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.189349 ora2-5.1.1/openassessment/locale/tr_TR/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.225350 ora2-5.1.1/openassessment/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    49577 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   116193 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     9435 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    27701 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.189349 ora2-5.1.1/openassessment/locale/uk/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.225350 ora2-5.1.1/openassessment/locale/uk/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    96047 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     8504 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/uk/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    28734 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/uk/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.189349 ora2-5.1.1/openassessment/locale/vi/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.229350 ora2-5.1.1/openassessment/locale/vi/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)    99390 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/vi/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/vi/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25235 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/vi/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.189349 ora2-5.1.1/openassessment/locale/zh_CN/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.229350 ora2-5.1.1/openassessment/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    46566 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   112823 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     6189 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    26173 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.189349 ora2-5.1.1/openassessment/locale/zh_TW/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.229350 ora2-5.1.1/openassessment/locale/zh_TW/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (122)    25222 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (122)   104144 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/zh_TW/LC_MESSAGES/django.po
--rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo
--rw-r--r--   0 runner    (1001) docker     (122)    25922 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.po
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.229350 ora2-5.1.1/openassessment/management/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.229350 ora2-5.1.1/openassessment/management/commands/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2422 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/management/commands/collect_ora2_data.py
--rw-r--r--   0 runner    (1001) docker     (122)     6882 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/management/commands/create_oa_submissions.py
--rw-r--r--   0 runner    (1001) docker     (122)    17900 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/management/commands/create_oa_submissions_from_file.py
--rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/management/commands/upload_oa_data.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.229350 ora2-5.1.1/openassessment/runtime_imports/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/runtime_imports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/runtime_imports/classes.py
--rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/runtime_imports/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.229350 ora2-5.1.1/openassessment/staffgrader/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/staffgrader/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      691 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/staffgrader/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.229350 ora2-5.1.1/openassessment/staffgrader/errors/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/staffgrader/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/staffgrader/errors/submission_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.233350 ora2-5.1.1/openassessment/staffgrader/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)      809 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/staffgrader/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/staffgrader/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.233350 ora2-5.1.1/openassessment/staffgrader/models/
--rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/staffgrader/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/staffgrader/models/submission_lock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.233350 ora2-5.1.1/openassessment/staffgrader/serializers/
--rw-r--r--   0 runner    (1001) docker     (122)      474 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/staffgrader/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/staffgrader/serializers/assessments.py
--rw-r--r--   0 runner    (1001) docker     (122)     6089 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/staffgrader/serializers/submission_list.py
--rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/staffgrader/serializers/submission_lock.py
--rw-r--r--   0 runner    (1001) docker     (122)    19964 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/staffgrader/staff_grader_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.189349 ora2-5.1.1/openassessment/templates/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.233350 ora2-5.1.1/openassessment/templates/openassessmentblock/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.237350 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/
--rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit.html
--rw-r--r--   0 runner    (1001) docker     (122)      854 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html
--rw-r--r--   0 runner    (1001) docker     (122)    10626 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
--rw-r--r--   0 runner    (1001) docker     (122)     3932 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
--rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html
--rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_option.html
--rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
--rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html
--rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html
--rw-r--r--   0 runner    (1001) docker     (122)     3437 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html
--rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html
--rw-r--r--   0 runner    (1001) docker     (122)      717 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)     2415 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
--rw-r--r--   0 runner    (1001) docker     (122)      197 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_settings.html
--rw-r--r--   0 runner    (1001) docker     (122)      785 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)     2942 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html
--rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html
--rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_training_example.html
--rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.237350 ora2-5.1.1/openassessment/templates/openassessmentblock/grade/
--rw-r--r--   0 runner    (1001) docker     (122)     1437 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html
--rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html
--rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)    17846 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html
--rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.237350 ora2-5.1.1/openassessment/templates/openassessmentblock/icons/
--rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/icons/warning_filled.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.237350 ora2-5.1.1/openassessment/templates/openassessmentblock/instructor_dashboard/
--rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html
--rw-r--r--   0 runner    (1001) docker     (122)      966 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html
--rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html
--rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/instructor_dashboard/open-response-assessment-summary.underscore
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.237350 ora2-5.1.1/openassessment/templates/openassessmentblock/leaderboard/
--rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html
--rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.241350 ora2-5.1.1/openassessment/templates/openassessmentblock/message/
--rw-r--r--   0 runner    (1001) docker     (122)      743 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)      660 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/message/oa_message_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)      708 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/message/oa_message_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     4279 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/message/oa_message_no_team.html
--rw-r--r--   0 runner    (1001) docker     (122)      951 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/message/oa_message_open.html
--rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/message/oa_message_unavailable.html
--rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/oa_base.html
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/oa_error.html
--rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/oa_latex_preview.html
--rw-r--r--   0 runner    (1001) docker     (122)     6927 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/oa_rubric.html
--rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/oa_submission_answer.html
--rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html
--rw-r--r--   0 runner    (1001) docker     (122)     2830 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/oa_uploaded_file.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.241350 ora2-5.1.1/openassessment/templates/openassessmentblock/peer/
--rw-r--r--   0 runner    (1001) docker     (122)     5758 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)      709 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     3855 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html
--rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
--rw-r--r--   0 runner    (1001) docker     (122)      633 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html
--rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.241350 ora2-5.1.1/openassessment/templates/openassessmentblock/response/
--rw-r--r--   0 runner    (1001) docker     (122)    21492 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/response/oa_response.html
--rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/response/oa_response_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/response/oa_response_graded.html
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/response/oa_response_studio_preview.html
--rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/response/oa_response_submitted.html
--rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html
--rw-r--r--   0 runner    (1001) docker     (122)      628 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.241350 ora2-5.1.1/openassessment/templates/openassessmentblock/self/
--rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/self/oa_self_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)      752 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/self/oa_self_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)      730 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/self/oa_self_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)      676 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.241350 ora2-5.1.1/openassessment/templates/openassessmentblock/staff/
--rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.241350 ora2-5.1.1/openassessment/templates/openassessmentblock/staff_area/
--rw-r--r--   0 runner    (1001) docker     (122)     8449 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
--rw-r--r--   0 runner    (1001) docker     (122)      887 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_count.html
--rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
--rw-r--r--   0 runner    (1001) docker     (122)    16404 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
--rw-r--r--   0 runner    (1001) docker     (122)     3732 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.245350 ora2-5.1.1/openassessment/templates/openassessmentblock/student_training/
--rw-r--r--   0 runner    (1001) docker     (122)    11281 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/student_training/student_training.html
--rw-r--r--   0 runner    (1001) docker     (122)      652 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html
--rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/student_training/student_training_closed.html
--rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/student_training/student_training_complete.html
--rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/student_training/student_training_error.html
--rw-r--r--   0 runner    (1001) docker     (122)      599 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.245350 ora2-5.1.1/openassessment/templatetags/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      886 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/templatetags/oa_extras.py
--rw-r--r--   0 runner    (1001) docker     (122)      758 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.245350 ora2-5.1.1/openassessment/workflow/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/workflow/admin.py
--rw-r--r--   0 runner    (1001) docker     (122)    19932 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/workflow/api.py
--rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/workflow/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.245350 ora2-5.1.1/openassessment/workflow/migrations/
--rw-r--r--   0 runner    (1001) docker     (122)     3111 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/workflow/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (122)      383 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/workflow/migrations/0002_remove_django_extensions.py
--rw-r--r--   0 runner    (1001) docker     (122)      826 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/workflow/migrations/0003_TeamWorkflows.py
--rw-r--r--   0 runner    (1001) docker     (122)      412 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/workflow/migrations/0004_assessmentworkflowstep_skipped.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/workflow/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    44741 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/workflow/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/workflow/serializers.py
--rw-r--r--   0 runner    (1001) docker     (122)     8350 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/workflow/team_api.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.249350 ora2-5.1.1/openassessment/xblock/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5880 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/config_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)      914 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/course_items_listing_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     7889 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/data_conversion.py
--rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/defaults.py
--rw-r--r--   0 runner    (1001) docker     (122)      622 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/editor_config.py
--rw-r--r--   0 runner    (1001) docker     (122)    30777 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/grade_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/leaderboard_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/lms_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/load_static.py
--rw-r--r--   0 runner    (1001) docker     (122)     9846 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/message_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/mobile.py
--rw-r--r--   0 runner    (1001) docker     (122)     3708 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/openassesment_template_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    50871 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/openassessmentblock.py
--rw-r--r--   0 runner    (1001) docker     (122)    14943 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/peer_assessment_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    10329 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/resolve_dates.py
--rw-r--r--   0 runner    (1001) docker     (122)     4560 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/rubric_reuse_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/schema.py
--rw-r--r--   0 runner    (1001) docker     (122)     7825 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/self_assessment_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    34259 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/staff_area_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     9317 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/staff_assessment_mixin.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.189349 ora2-5.1.1/openassessment/xblock/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.189349 ora2-5.1.1/openassessment/xblock/static/css/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.189349 ora2-5.1.1/openassessment/xblock/static/css/lib/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.249350 ora2-5.1.1/openassessment/xblock/static/css/lib/backgrid/
--rw-r--r--   0 runner    (1001) docker     (122)     5382 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/css/lib/backgrid/backgrid.css
--rw-r--r--   0 runner    (1001) docker     (122)     4414 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.293351 ora2-5.1.1/openassessment/xblock/static/dist/
--rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/manifest.json
--rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-editor-textarea.b8f866ba96a1d2ad92a4.js
--rw-r--r--   0 runner    (1001) docker     (122)    38550 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-editor-textarea.js
--rw-r--r--   0 runner    (1001) docker     (122)     2973 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-editor-tinymce.2cc0cab55c3be729265e.js
--rw-r--r--   0 runner    (1001) docker     (122)    47578 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-editor-tinymce.js
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-lms.967dad15c001a5dc6a5e.css
--rw-r--r--   0 runner    (1001) docker     (122)  1350843 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-lms.967dad15c001a5dc6a5e.js
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-lms.css
--rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.css
--rw-r--r--   0 runner    (1001) docker     (122)  1350596 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.js
--rw-r--r--   0 runner    (1001) docker     (122) 28868716 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-lms.js
--rw-r--r--   0 runner    (1001) docker     (122)   757135 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.css
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.js
--rw-r--r--   0 runner    (1001) docker     (122)   757664 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-ltr.b9eeb00dfc7524a80658.css
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-ltr.b9eeb00dfc7524a80658.js
--rw-r--r--   0 runner    (1001) docker     (122)   851349 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-ltr.css
--rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-ltr.js
--rw-r--r--   0 runner    (1001) docker     (122)   757164 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.css
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.js
--rw-r--r--   0 runner    (1001) docker     (122)   851378 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-rtl.css
--rw-r--r--   0 runner    (1001) docker     (122)   757693 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-rtl.ef543a27286a069bd958.css
--rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-rtl.ef543a27286a069bd958.js
--rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-rtl.js
--rw-r--r--   0 runner    (1001) docker     (122)   235851 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-studio.13c817d25360969539ff.js
--rw-r--r--   0 runner    (1001) docker     (122)   235846 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-studio.1ef78b4390a9cfa2e9b1.js
--rw-r--r--   0 runner    (1001) docker     (122)  2305380 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/dist/openassessment-studio.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.189349 ora2-5.1.1/openassessment/xblock/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.189349 ora2-5.1.1/openassessment/xblock/static/js/lib/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.297351 ora2-5.1.1/openassessment/xblock/static/js/lib/backgrid/
--rw-r--r--   0 runner    (1001) docker     (122)    87583 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/lib/backgrid/backgrid.js
--rw-r--r--   0 runner    (1001) docker     (122)    26169 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.297351 ora2-5.1.1/openassessment/xblock/static/js/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.301351 ora2-5.1.1/openassessment/xblock/static/js/src/lms/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.301351 ora2-5.1.1/openassessment/xblock/static/js/src/lms/api/
--rw-r--r--   0 runner    (1001) docker     (122)      817 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.301351 ora2-5.1.1/openassessment/xblock/static/js/src/lms/editors/
--rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js
--rw-r--r--   0 runner    (1001) docker     (122)     3741 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js
--rw-r--r--   0 runner    (1001) docker     (122)    18084 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_base.js
--rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js
--rw-r--r--   0 runner    (1001) docker     (122)    10567 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
--rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_datefactory.js
--rw-r--r--   0 runner    (1001) docker     (122)     2013 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_file_upload.js
--rw-r--r--   0 runner    (1001) docker     (122)     8877 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_grade.js
--rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_leaderboard.js
--rw-r--r--   0 runner    (1001) docker     (122)      910 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_message.js
--rw-r--r--   0 runner    (1001) docker     (122)     9796 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_peer.js
--rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_prompts.js
--rw-r--r--   0 runner    (1001) docker     (122)    32903 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_response.js
--rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_response_editor.js
--rw-r--r--   0 runner    (1001) docker     (122)     7024 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_rubric.js
--rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_self.js
--rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_staff.js
--rw-r--r--   0 runner    (1001) docker     (122)    24786 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_staff_area.js
--rw-r--r--   0 runner    (1001) docker     (122)     5267 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_training.js
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/lms_index.js
--rw-r--r--   0 runner    (1001) docker     (122)    26171 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/oa_server.js
--rw-r--r--   0 runner    (1001) docker     (122)      963 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/oa_shared.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.301351 ora2-5.1.1/openassessment/xblock/static/js/src/studio/
--rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_container.js
--rw-r--r--   0 runner    (1001) docker     (122)    20684 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_container_item.js
--rw-r--r--   0 runner    (1001) docker     (122)    12727 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit.js
--rw-r--r--   0 runner    (1001) docker     (122)    15956 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js
--rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js
--rw-r--r--   0 runner    (1001) docker     (122)    11441 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_fields.js
--rw-r--r--   0 runner    (1001) docker     (122)    13033 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
--rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js
--rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js
--rw-r--r--   0 runner    (1001) docker     (122)    13149 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js
--rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js
--rw-r--r--   0 runner    (1001) docker     (122)    15272 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_settings.js
--rw-r--r--   0 runner    (1001) docker     (122)     3746 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js
--rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/static/js/src/studio_index.js
--rw-r--r--   0 runner    (1001) docker     (122)    11859 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/student_training_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    20538 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/studio_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    41983 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/submission_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     8743 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/team_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/team_workflow_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)      675 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/user_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    15746 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/validation.py
--rw-r--r--   0 runner    (1001) docker     (122)     8409 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/workflow_mixin.py
--rw-r--r--   0 runner    (1001) docker     (122)    35842 2023-07-12 07:38:42.000000 ora2-5.1.1/openassessment/xblock/xml.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.301351 ora2-5.1.1/ora2.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-07-12 07:38:46.000000 ora2-5.1.1/ora2.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    23584 2023-07-12 07:38:46.000000 ora2-5.1.1/ora2.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-12 07:38:46.000000 ora2-5.1.1/ora2.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-12 07:38:46.000000 ora2-5.1.1/ora2.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      289 2023-07-12 07:38:46.000000 ora2-5.1.1/ora2.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-12 07:38:46.000000 ora2-5.1.1/ora2.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-12 07:38:46.305351 ora2-5.1.1/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-07-12 07:38:42.000000 ora2-5.1.1/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (122)       40 2023-07-12 07:38:42.000000 ora2-5.1.1/requirements/ci.in
--rw-r--r--   0 runner    (1001) docker     (122)      179 2023-07-12 07:38:42.000000 ora2-5.1.1/requirements/pip-tools.in
--rw-r--r--   0 runner    (1001) docker     (122)       91 2023-07-12 07:38:42.000000 ora2-5.1.1/requirements/pip.in
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-07-12 07:38:42.000000 ora2-5.1.1/requirements/quality.in
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-12 07:38:42.000000 ora2-5.1.1/requirements/test-acceptance.in
--rw-r--r--   0 runner    (1001) docker     (122)      685 2023-07-12 07:38:42.000000 ora2-5.1.1/requirements/test.in
--rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-12 07:38:42.000000 ora2-5.1.1/requirements/tox.in
--rw-r--r--   0 runner    (1001) docker     (122)      318 2023-07-12 07:38:46.305351 ora2-5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-07-12 07:38:42.000000 ora2-5.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.654133 ora2-5.2.0/
+-rw-r--r--   0 runner    (1001) docker     (122)    35135 2023-07-18 18:44:53.000000 ora2-5.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      682 2023-07-18 18:44:53.000000 ora2-5.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-07-18 18:44:56.658133 ora2-5.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2038 2023-07-18 18:44:53.000000 ora2-5.2.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.542132 ora2-5.2.0/openassessment/
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.542132 ora2-5.2.0/openassessment/assessment/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5633 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.550132 ora2-5.2.0/openassessment/assessment/api/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    39563 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/api/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11936 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/api/self.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16495 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/api/staff.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16864 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/api/student_training.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13017 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/api/teams.py
+-rw-r--r--   0 runner    (1001) docker     (122)      442 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/data_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.554132 ora2-5.2.0/openassessment/assessment/errors/
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      189 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/errors/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1117 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/errors/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/errors/self.py
+-rw-r--r--   0 runner    (1001) docker     (122)      821 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/errors/staff.py
+-rw-r--r--   0 runner    (1001) docker     (122)      440 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/errors/student_training.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.558132 ora2-5.2.0/openassessment/assessment/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     9361 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1333 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/migrations/0002_staffworkflow.py
+-rw-r--r--   0 runner    (1001) docker     (122)      750 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/migrations/0003_expand_course_id.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3459 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py
+-rw-r--r--   0 runner    (1001) docker     (122)      618 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py
+-rw-r--r--   0 runner    (1001) docker     (122)      744 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/migrations/0006_TeamWorkflows.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1218 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/migrations/0007_staff_workflow_blank.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.558132 ora2-5.2.0/openassessment/assessment/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      205 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32191 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22340 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/models/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8558 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/models/staff.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8200 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/models/student_training.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4991 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/models/training.py
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/score_type_constants.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.562132 ora2-5.2.0/openassessment/assessment/serializers/
+-rw-r--r--   0 runner    (1001) docker     (122)      151 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10553 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/serializers/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2021 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/serializers/peer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6217 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/serializers/training.py
+-rw-r--r--   0 runner    (1001) docker     (122)      376 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)      265 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1874 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/assessment/views.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58992 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.562132 ora2-5.2.0/openassessment/fileupload/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/fileupload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23578 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/fileupload/api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.562132 ora2-5.2.0/openassessment/fileupload/backends/
+-rw-r--r--   0 runner    (1001) docker     (122)      849 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/fileupload/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5253 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/fileupload/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2411 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/fileupload/backends/django_storage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4122 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/fileupload/backends/filesystem.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3309 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/fileupload/backends/s3.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3392 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/fileupload/backends/swift.py
+-rw-r--r--   0 runner    (1001) docker     (122)      740 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/fileupload/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/fileupload/urls.py
+-rw-r--r--   0 runner    (1001) docker     (122)      498 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/fileupload/views_django_storage.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5105 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/fileupload/views_filesystem.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.562132 ora2-5.2.0/openassessment/locale/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.530131 ora2-5.2.0/openassessment/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.562132 ora2-5.2.0/openassessment/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    82260 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   137572 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    10517 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ar/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29332 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ar/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.530131 ora2-5.2.0/openassessment/locale/ar_SA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.562132 ora2-5.2.0/openassessment/locale/ar_SA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9218 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28056 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.530131 ora2-5.2.0/openassessment/locale/de_DE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.566132 ora2-5.2.0/openassessment/locale/de_DE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    64223 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   124947 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8402 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27871 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.530131 ora2-5.2.0/openassessment/locale/el/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.566132 ora2-5.2.0/openassessment/locale/el/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    35998 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   116285 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/el/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     5045 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/el/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26850 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/el/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.530131 ora2-5.2.0/openassessment/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.566132 ora2-5.2.0/openassessment/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)      382 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    84892 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      425 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/en/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27184 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/en/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.530131 ora2-5.2.0/openassessment/locale/eo/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.566132 ora2-5.2.0/openassessment/locale/eo/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)   145884 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/eo/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   186603 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/eo/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    22487 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/eo/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    42004 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/eo/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.534131 ora2-5.2.0/openassessment/locale/es_419/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.570132 ora2-5.2.0/openassessment/locale/es_419/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81996 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/es_419/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   133250 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/es_419/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11545 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29006 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/es_419/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.534131 ora2-5.2.0/openassessment/locale/es_AR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.570132 ora2-5.2.0/openassessment/locale/es_AR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    11444 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28411 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.534131 ora2-5.2.0/openassessment/locale/es_ES/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.570132 ora2-5.2.0/openassessment/locale/es_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    82594 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/es_ES/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   133560 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/es_ES/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11635 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29042 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.534131 ora2-5.2.0/openassessment/locale/eu_ES/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.570132 ora2-5.2.0/openassessment/locale/eu_ES/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    14552 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/eu_ES/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   100050 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/eu_ES/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     3947 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25057 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.534131 ora2-5.2.0/openassessment/locale/fa_IR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.570132 ora2-5.2.0/openassessment/locale/fa_IR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    92564 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/fa_IR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   142763 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/fa_IR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    13499 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    30711 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.534131 ora2-5.2.0/openassessment/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.570132 ora2-5.2.0/openassessment/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81340 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   133090 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11874 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/fr/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/fr/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/fr_CA/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.574132 ora2-5.2.0/openassessment/locale/fr_CA/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    82568 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/fr_CA/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   136626 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/fr_CA/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11820 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    31089 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/he/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.574132 ora2-5.2.0/openassessment/locale/he/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    48842 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/he/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   117773 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/he/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     7008 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/he/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27047 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/he/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/hi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.574132 ora2-5.2.0/openassessment/locale/hi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/hi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95113 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/hi/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1753 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/hi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24633 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/hi/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/id/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.574132 ora2-5.2.0/openassessment/locale/id/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    40204 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/id/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   112010 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/id/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6748 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/id/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26550 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/id/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/it_IT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.574132 ora2-5.2.0/openassessment/locale/it_IT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81986 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/it_IT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   132727 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/it_IT/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11586 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28920 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/ja_JP/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.578132 ora2-5.2.0/openassessment/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    50706 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   118496 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ja_JP/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     7079 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27020 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/ka/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.578132 ora2-5.2.0/openassessment/locale/ka/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    77213 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ka/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   144721 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ka/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8953 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ka/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29444 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ka/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/lt_LT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.578132 ora2-5.2.0/openassessment/locale/lt_LT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    19263 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/lt_LT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   102318 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/lt_LT/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2764 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24738 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/lv/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.578132 ora2-5.2.0/openassessment/locale/lv/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1383 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/lv/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    94833 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/lv/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      962 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/lv/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23895 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/lv/LC_MESSAGES/djangojs.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6039 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/messages.mo
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/mn/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.578132 ora2-5.2.0/openassessment/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1741 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/mn/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95311 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/mn/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)      559 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/mn/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    22473 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/mn/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/nb/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.578132 ora2-5.2.0/openassessment/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     7793 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    97392 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6672 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/nb/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26384 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/nb/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.582132 ora2-5.2.0/openassessment/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    51135 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   117244 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6823 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/pl/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26637 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/pl/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/pt_BR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.582132 ora2-5.2.0/openassessment/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    32487 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   109420 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     5663 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26740 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/pt_PT/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.582132 ora2-5.2.0/openassessment/locale/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    81743 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/pt_PT/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   132378 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/pt_PT/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)    11556 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    29200 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/ro/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.582132 ora2-5.2.0/openassessment/locale/ro/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2590 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95431 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2234 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ro/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    24522 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ro/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.582132 ora2-5.2.0/openassessment/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    59971 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   128218 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8622 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ru/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28603 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/ru/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/sk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.582132 ora2-5.2.0/openassessment/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     4054 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/sk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25387 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/sk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.586132 ora2-5.2.0/openassessment/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     2554 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    95372 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/sq/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     1106 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/sq/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    23998 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/sq/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/sw_KE/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.586132 ora2-5.2.0/openassessment/locale/sw_KE/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    43322 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/sw_KE/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   111947 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/sw_KE/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6441 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26486 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/th/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.586132 ora2-5.2.0/openassessment/locale/th/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    27854 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/th/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   111076 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/th/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/th/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26116 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/th/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/tr_TR/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.586132 ora2-5.2.0/openassessment/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    49577 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   116193 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     9435 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    27701 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/uk/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.586132 ora2-5.2.0/openassessment/locale/uk/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     1984 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    96047 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     8504 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/uk/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    28734 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/uk/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.538131 ora2-5.2.0/openassessment/locale/vi/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.586132 ora2-5.2.0/openassessment/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)     9677 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    99390 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/vi/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     2756 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/vi/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25235 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/vi/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.542132 ora2-5.2.0/openassessment/locale/zh_CN/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.590132 ora2-5.2.0/openassessment/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    46566 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   112823 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     6189 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    26173 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.542132 ora2-5.2.0/openassessment/locale/zh_TW/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.590132 ora2-5.2.0/openassessment/locale/zh_TW/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (122)    25222 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (122)   104144 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/zh_TW/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (122)     5023 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo
+-rw-r--r--   0 runner    (1001) docker     (122)    25922 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.po
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.590132 ora2-5.2.0/openassessment/management/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.590132 ora2-5.2.0/openassessment/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2422 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/management/commands/collect_ora2_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6886 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/management/commands/create_oa_submissions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17908 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/management/commands/create_oa_submissions_from_file.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5269 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/management/commands/upload_oa_data.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.590132 ora2-5.2.0/openassessment/runtime_imports/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/runtime_imports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1220 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/runtime_imports/classes.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1324 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/runtime_imports/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.590132 ora2-5.2.0/openassessment/staffgrader/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/staffgrader/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      691 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/staffgrader/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.590132 ora2-5.2.0/openassessment/staffgrader/errors/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/staffgrader/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      297 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/staffgrader/errors/submission_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.590132 ora2-5.2.0/openassessment/staffgrader/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)      809 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/staffgrader/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/staffgrader/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.590132 ora2-5.2.0/openassessment/staffgrader/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      132 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/staffgrader/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3511 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/staffgrader/models/submission_lock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.590132 ora2-5.2.0/openassessment/staffgrader/serializers/
+-rw-r--r--   0 runner    (1001) docker     (122)      474 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/staffgrader/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1751 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/staffgrader/serializers/assessments.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6089 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/staffgrader/serializers/submission_list.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1593 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/staffgrader/serializers/submission_lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19964 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/staffgrader/staff_grader_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.542132 ora2-5.2.0/openassessment/templates/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.594132 ora2-5.2.0/openassessment/templates/openassessmentblock/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.594132 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/
+-rw-r--r--   0 runner    (1001) docker     (122)     1179 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit.html
+-rw-r--r--   0 runner    (1001) docker     (122)      854 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html
+-rw-r--r--   0 runner    (1001) docker     (122)    10626 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3932 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2818 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2499 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_option.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4017 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1358 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1095 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3437 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2921 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html
+-rw-r--r--   0 runner    (1001) docker     (122)      717 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2415 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_settings.html
+-rw-r--r--   0 runner    (1001) docker     (122)      785 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2942 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2343 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1531 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_training_example.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1174 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.594132 ora2-5.2.0/openassessment/templates/openassessmentblock/grade/
+-rw-r--r--   0 runner    (1001) docker     (122)     1437 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1328 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2342 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)    17846 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1779 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.594132 ora2-5.2.0/openassessment/templates/openassessmentblock/icons/
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/icons/warning_filled.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.598132 ora2-5.2.0/openassessment/templates/openassessmentblock/instructor_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (122)     1471 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html
+-rw-r--r--   0 runner    (1001) docker     (122)      966 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1225 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html
+-rw-r--r--   0 runner    (1001) docker     (122)      454 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/instructor_dashboard/open-response-assessment-summary.underscore
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.598132 ora2-5.2.0/openassessment/templates/openassessmentblock/leaderboard/
+-rw-r--r--   0 runner    (1001) docker     (122)     2008 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1276 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.598132 ora2-5.2.0/openassessment/templates/openassessmentblock/message/
+-rw-r--r--   0 runner    (1001) docker     (122)      743 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)      660 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/message/oa_message_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/message/oa_message_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     4279 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/message/oa_message_no_team.html
+-rw-r--r--   0 runner    (1001) docker     (122)      951 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/message/oa_message_open.html
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/message/oa_message_unavailable.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2414 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/oa_base.html
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/oa_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1026 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/oa_latex_preview.html
+-rw-r--r--   0 runner    (1001) docker     (122)     6927 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/oa_rubric.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1519 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/oa_submission_answer.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2107 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2830 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/oa_uploaded_file.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.598132 ora2-5.2.0/openassessment/templates/openassessmentblock/peer/
+-rw-r--r--   0 runner    (1001) docker     (122)     5758 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)      709 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1930 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2330 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3855 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1932 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html
+-rw-r--r--   0 runner    (1001) docker     (122)      633 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1937 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.598132 ora2-5.2.0/openassessment/templates/openassessmentblock/response/
+-rw-r--r--   0 runner    (1001) docker     (122)    21492 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/response/oa_response.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2577 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1597 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/response/oa_response_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/response/oa_response_graded.html
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/response/oa_response_studio_preview.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3728 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/response/oa_response_submitted.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1625 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html
+-rw-r--r--   0 runner    (1001) docker     (122)      628 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.598132 ora2-5.2.0/openassessment/templates/openassessmentblock/self/
+-rw-r--r--   0 runner    (1001) docker     (122)     4593 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/self/oa_self_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)      752 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1503 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/self/oa_self_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)      730 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/self/oa_self_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)      676 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.598132 ora2-5.2.0/openassessment/templates/openassessmentblock/staff/
+-rw-r--r--   0 runner    (1001) docker     (122)     1707 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.602132 ora2-5.2.0/openassessment/templates/openassessmentblock/staff_area/
+-rw-r--r--   0 runner    (1001) docker     (122)     8449 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html
+-rw-r--r--   0 runner    (1001) docker     (122)      887 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)      407 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_count.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3167 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html
+-rw-r--r--   0 runner    (1001) docker     (122)    16404 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html
+-rw-r--r--   0 runner    (1001) docker     (122)     3732 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.602132 ora2-5.2.0/openassessment/templates/openassessmentblock/student_training/
+-rw-r--r--   0 runner    (1001) docker     (122)    11281 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/student_training/student_training.html
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1371 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/student_training/student_training_closed.html
+-rw-r--r--   0 runner    (1001) docker     (122)      653 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/student_training/student_training_complete.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1137 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/student_training/student_training_error.html
+-rw-r--r--   0 runner    (1001) docker     (122)      599 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.602132 ora2-5.2.0/openassessment/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      886 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/templatetags/oa_extras.py
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.602132 ora2-5.2.0/openassessment/workflow/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/workflow/admin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20327 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/workflow/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1589 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/workflow/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.602132 ora2-5.2.0/openassessment/workflow/migrations/
+-rw-r--r--   0 runner    (1001) docker     (122)     3111 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/workflow/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (122)      383 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/workflow/migrations/0002_remove_django_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      826 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/workflow/migrations/0003_TeamWorkflows.py
+-rw-r--r--   0 runner    (1001) docker     (122)      412 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/workflow/migrations/0004_assessmentworkflowstep_skipped.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/workflow/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    45497 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/workflow/models.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1660 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/workflow/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8517 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/workflow/team_api.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.606133 ora2-5.2.0/openassessment/xblock/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5880 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/config_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      914 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/course_items_listing_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7889 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/data_conversion.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6829 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (122)      622 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/editor_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30876 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/grade_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5837 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/leaderboard_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3827 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/lms_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2101 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/load_static.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9846 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/message_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      770 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/mobile.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3708 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/openassesment_template_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    51118 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/openassessmentblock.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14943 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/peer_assessment_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10329 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/resolve_dates.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4560 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/rubric_reuse_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5369 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7825 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/self_assessment_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34490 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/staff_area_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9337 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/staff_assessment_mixin.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.542132 ora2-5.2.0/openassessment/xblock/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.542132 ora2-5.2.0/openassessment/xblock/static/css/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.542132 ora2-5.2.0/openassessment/xblock/static/css/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.606133 ora2-5.2.0/openassessment/xblock/static/css/lib/backgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)     5382 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/css/lib/backgrid/backgrid.css
+-rw-r--r--   0 runner    (1001) docker     (122)     4414 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.646133 ora2-5.2.0/openassessment/xblock/static/dist/
+-rw-r--r--   0 runner    (1001) docker     (122)     1617 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1834 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-editor-textarea.b8f866ba96a1d2ad92a4.js
+-rw-r--r--   0 runner    (1001) docker     (122)    38550 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-editor-textarea.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2973 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-editor-tinymce.2cc0cab55c3be729265e.js
+-rw-r--r--   0 runner    (1001) docker     (122)    47578 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-editor-tinymce.js
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-lms.967dad15c001a5dc6a5e.css
+-rw-r--r--   0 runner    (1001) docker     (122)  1350843 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-lms.967dad15c001a5dc6a5e.js
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-lms.css
+-rw-r--r--   0 runner    (1001) docker     (122)       72 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.css
+-rw-r--r--   0 runner    (1001) docker     (122)  1350596 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.js
+-rw-r--r--   0 runner    (1001) docker     (122) 28868716 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-lms.js
+-rw-r--r--   0 runner    (1001) docker     (122)   757135 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.js
+-rw-r--r--   0 runner    (1001) docker     (122)   757664 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-ltr.b9eeb00dfc7524a80658.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-ltr.b9eeb00dfc7524a80658.js
+-rw-r--r--   0 runner    (1001) docker     (122)   851349 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-ltr.css
+-rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-ltr.js
+-rw-r--r--   0 runner    (1001) docker     (122)   757164 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.js
+-rw-r--r--   0 runner    (1001) docker     (122)   851378 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-rtl.css
+-rw-r--r--   0 runner    (1001) docker     (122)   757693 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-rtl.ef543a27286a069bd958.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-rtl.ef543a27286a069bd958.js
+-rw-r--r--   0 runner    (1001) docker     (122)    32672 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-rtl.js
+-rw-r--r--   0 runner    (1001) docker     (122)   235851 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-studio.13c817d25360969539ff.js
+-rw-r--r--   0 runner    (1001) docker     (122)   235846 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-studio.1ef78b4390a9cfa2e9b1.js
+-rw-r--r--   0 runner    (1001) docker     (122)  2305380 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/dist/openassessment-studio.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.542132 ora2-5.2.0/openassessment/xblock/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.542132 ora2-5.2.0/openassessment/xblock/static/js/lib/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.650133 ora2-5.2.0/openassessment/xblock/static/js/lib/backgrid/
+-rw-r--r--   0 runner    (1001) docker     (122)    87583 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/lib/backgrid/backgrid.js
+-rw-r--r--   0 runner    (1001) docker     (122)    26169 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.650133 ora2-5.2.0/openassessment/xblock/static/js/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.654133 ora2-5.2.0/openassessment/xblock/static/js/src/lms/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.654133 ora2-5.2.0/openassessment/xblock/static/js/src/lms/api/
+-rw-r--r--   0 runner    (1001) docker     (122)      817 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.654133 ora2-5.2.0/openassessment/xblock/static/js/src/lms/editors/
+-rw-r--r--   0 runner    (1001) docker     (122)     1368 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3741 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js
+-rw-r--r--   0 runner    (1001) docker     (122)    18084 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_base.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1878 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js
+-rw-r--r--   0 runner    (1001) docker     (122)    10567 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1994 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_datefactory.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2013 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_file_upload.js
+-rw-r--r--   0 runner    (1001) docker     (122)     8877 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_grade.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_leaderboard.js
+-rw-r--r--   0 runner    (1001) docker     (122)      910 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_message.js
+-rw-r--r--   0 runner    (1001) docker     (122)     9796 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_peer.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1882 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_prompts.js
+-rw-r--r--   0 runner    (1001) docker     (122)    32903 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_response.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1860 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_response_editor.js
+-rw-r--r--   0 runner    (1001) docker     (122)     7024 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_rubric.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5344 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_self.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1351 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_staff.js
+-rw-r--r--   0 runner    (1001) docker     (122)    24786 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_staff_area.js
+-rw-r--r--   0 runner    (1001) docker     (122)     5267 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_training.js
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/lms_index.js
+-rw-r--r--   0 runner    (1001) docker     (122)    26171 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/oa_server.js
+-rw-r--r--   0 runner    (1001) docker     (122)      963 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/oa_shared.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.654133 ora2-5.2.0/openassessment/xblock/static/js/src/studio/
+-rw-r--r--   0 runner    (1001) docker     (122)     7705 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_container.js
+-rw-r--r--   0 runner    (1001) docker     (122)    20684 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_container_item.js
+-rw-r--r--   0 runner    (1001) docker     (122)    12727 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit.js
+-rw-r--r--   0 runner    (1001) docker     (122)    15956 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js
+-rw-r--r--   0 runner    (1001) docker     (122)     6121 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js
+-rw-r--r--   0 runner    (1001) docker     (122)    11441 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_fields.js
+-rw-r--r--   0 runner    (1001) docker     (122)    13033 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js
+-rw-r--r--   0 runner    (1001) docker     (122)     1282 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3277 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js
+-rw-r--r--   0 runner    (1001) docker     (122)    13149 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4349 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js
+-rw-r--r--   0 runner    (1001) docker     (122)    15272 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_settings.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3746 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js
+-rw-r--r--   0 runner    (1001) docker     (122)     2654 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/static/js/src/studio_index.js
+-rw-r--r--   0 runner    (1001) docker     (122)    11859 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/student_training_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20538 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/studio_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    41983 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/submission_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8743 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/team_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4631 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/team_workflow_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)      675 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/user_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15746 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9205 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/workflow_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (122)    35842 2023-07-18 18:44:53.000000 ora2-5.2.0/openassessment/xblock/xml.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.654133 ora2-5.2.0/ora2.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2643 2023-07-18 18:44:56.000000 ora2-5.2.0/ora2.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    23584 2023-07-18 18:44:56.000000 ora2-5.2.0/ora2.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-07-18 18:44:56.000000 ora2-5.2.0/ora2.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       92 2023-07-18 18:44:56.000000 ora2-5.2.0/ora2.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      281 2023-07-18 18:44:56.000000 ora2-5.2.0/ora2.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-07-18 18:44:56.000000 ora2-5.2.0/ora2.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-07-18 18:44:56.654133 ora2-5.2.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)      405 2023-07-18 18:44:53.000000 ora2-5.2.0/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (122)       40 2023-07-18 18:44:53.000000 ora2-5.2.0/requirements/ci.in
+-rw-r--r--   0 runner    (1001) docker     (122)      179 2023-07-18 18:44:53.000000 ora2-5.2.0/requirements/pip-tools.in
+-rw-r--r--   0 runner    (1001) docker     (122)       91 2023-07-18 18:44:53.000000 ora2-5.2.0/requirements/pip.in
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-07-18 18:44:53.000000 ora2-5.2.0/requirements/quality.in
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-07-18 18:44:53.000000 ora2-5.2.0/requirements/test-acceptance.in
+-rw-r--r--   0 runner    (1001) docker     (122)      685 2023-07-18 18:44:53.000000 ora2-5.2.0/requirements/test.in
+-rw-r--r--   0 runner    (1001) docker     (122)       23 2023-07-18 18:44:53.000000 ora2-5.2.0/requirements/tox.in
+-rw-r--r--   0 runner    (1001) docker     (122)      318 2023-07-18 18:44:56.658133 ora2-5.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     2593 2023-07-18 18:44:53.000000 ora2-5.2.0/setup.py
```

### Comparing `ora2-5.1.1/LICENSE` & `ora2-5.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/MANIFEST.in` & `ora2-5.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/PKG-INFO` & `ora2-5.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ora2
-Version: 5.1.1
+Version: 5.2.0
 Summary: edx-ora2
 Home-page: http://github.com/openedx/edx-ora2
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ora2-5.1.1/README.rst` & `ora2-5.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/admin.py` & `ora2-5.2.0/openassessment/assessment/admin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/api/peer.py` & `ora2-5.2.0/openassessment/assessment/api/peer.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,25 @@
 
 PEER_TYPE = "PE"
 
 FLEXIBLE_PEER_GRADING_REQUIRED_SUBMISSION_AGE_IN_DAYS = 7
 FLEXIBLE_PEER_GRADING_GRADED_BY_PERCENTAGE = 30
 
 
-def required_peer_grades(submission_uuid, peer_requirements):
+def flexible_peer_grading_enabled(peer_requirements, course_settings):
+    """
+    Is flexible peer grading turned on? Either at the course override
+    level or the block level?
+    """
+    if course_settings.get('force_on_flexible_peer_openassessments'):
+        return True
+    return peer_requirements.get("enable_flexible_grading")
+
+
+def required_peer_grades(submission_uuid, peer_requirements, course_settings):
     """
     Given a submission id, finds how many peer assessment required.
 
     Args:
         submission_uuid (str): The UUID of the submission being tracked.
         peer_requirements (dict): Dictionary with the key "must_grade" indicating
             the required number of submissions the student must grade
@@ -41,15 +51,15 @@
         int
     """
 
     submission = sub_api.get_submission(submission_uuid)
 
     must_grade = peer_requirements["must_be_graded_by"]
 
-    if peer_requirements.get("enable_flexible_grading"):
+    if flexible_peer_grading_enabled(peer_requirements, course_settings):
 
         # find how many days elapsed since subimitted
         days_elapsed = (timezone.now().date() - submission['submitted_at'].date()).days
 
         # check if flexible grading applies. if it does, then update must_grade
         if days_elapsed >= FLEXIBLE_PEER_GRADING_REQUIRED_SUBMISSION_AGE_IN_DAYS:
             must_grade = int(must_grade * FLEXIBLE_PEER_GRADING_GRADED_BY_PERCENTAGE / 100)
@@ -121,15 +131,15 @@
     scored_items = workflow.graded_by.filter(
         assessment__submission_uuid=submission_uuid,
         assessment__score_type=PEER_TYPE
     )
     return scored_items.count()
 
 
-def assessment_is_finished(submission_uuid, peer_requirements):
+def assessment_is_finished(submission_uuid, peer_requirements, course_settings):
     """
     Check whether the submitter has received enough assessments
     to get a score.
 
     If the requirements dict is None (because we're being updated
     asynchronously or when the workflow is first created),
     then automatically return False.
@@ -147,15 +157,15 @@
     if not peer_requirements:
         return False
 
     count = get_graded_by_count(submission_uuid)
     if count is None:
         return False
 
-    return count >= required_peer_grades(submission_uuid, peer_requirements)
+    return count >= required_peer_grades(submission_uuid, peer_requirements, course_settings)
 
 
 def on_start(submission_uuid):
     """Create a new peer workflow for a student item and submission.
 
     Creates a unique peer workflow for a student item, associated with a
     submission.
@@ -192,23 +202,24 @@
             "workflow for submission {}"
             .format(submission_uuid)
         )
         logger.exception(error_message)
         raise PeerAssessmentInternalError(error_message) from ex
 
 
-def get_score(submission_uuid, peer_requirements):
+def get_score(submission_uuid, peer_requirements, course_settings):
     """
     Retrieve a score for a submission if requirements have been satisfied.
 
     Args:
         submission_uuid (str): The UUID of the submission.
         requirements (dict): Dictionary with the key "must_be_graded_by"
             indicating the required number of assessments the student
             must receive to get a score.
+        course_settings (dict): Dictionary with course-level settings
 
     Returns:
         A dictionary with the points earned, points possible, and
         contributing_assessments information, along with a None staff_id.
 
     """
 
@@ -228,15 +239,15 @@
     # because we want to use the *first* one(s) for the score.
     items = workflow.graded_by.filter(
         assessment__submission_uuid=submission_uuid,
         assessment__score_type=PEER_TYPE
     ).order_by('-assessment')
 
     # Check if enough peers have graded this submission
-    num_required_peer_grades = required_peer_grades(submission_uuid, peer_requirements)
+    num_required_peer_grades = required_peer_grades(submission_uuid, peer_requirements, course_settings)
     if items.count() < num_required_peer_grades:
         return None
 
     # Unfortunately, we cannot use update() after taking a slice,
     # so we need to update the and save the items individually.
     # One might be tempted to first query for the first n assessments,
     # then select items that have those assessments.
```

### Comparing `ora2-5.1.1/openassessment/assessment/api/self.py` & `ora2-5.2.0/openassessment/assessment/api/self.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
         True
     """
     return Assessment.objects.filter(
         score_type=SELF_TYPE, submission_uuid=submission_uuid
     ).exists()
 
 
-def assessment_is_finished(submission_uuid, self_requirements):
+def assessment_is_finished(submission_uuid, self_requirements, _):
     """
     Check whether a self-assessment has been completed. For self-assessment,
     this function is synonymous with submitter_is_finished.
 
     Args:
         submission_uuid (str): The unique identifier of the submission.
         self_requirements (dict): Any attributes of the assessment module required
@@ -52,21 +52,22 @@
     Examples:
         >>> assessment_is_finished('222bdf3d-a88e-11e3-859e-040ccee02800', {})
         True
     """
     return submitter_is_finished(submission_uuid, self_requirements)
 
 
-def get_score(submission_uuid, self_requirements):  # pylint: disable=unused-argument
+def get_score(submission_uuid, self_requirements, course_settings):  # pylint: disable=unused-argument
     """
     Get the score for this particular assessment.
 
     Args:
         submission_uuid (str): The unique identifier for the submission
         self_requirements (dict): Not used.
+        course_settings (dict): Not used.
     Returns:
         A dictionary with the points earned, points possible, and
         contributing_assessments information, along with a None staff_id.
     Examples:
         >>> get_score('222bdf3d-a88e-11e3-859e-040ccee02800', {})
         {
             'points_earned': 5,
```

### Comparing `ora2-5.1.1/openassessment/assessment/api/staff.py` & `ora2-5.2.0/openassessment/assessment/api/staff.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     Returns:
         True
 
     """
     return True
 
 
-def assessment_is_finished(submission_uuid, staff_requirements):
+def assessment_is_finished(submission_uuid, staff_requirements, _):
     """
     Determine if the staff assessment step of the given submission is completed.
     This checks to see if staff have completed the assessment.
 
     Args:
         submission_uuid (str): The UUID of the submission being graded.
         staff_requirements (dict): Any variables that may effect this state.
@@ -123,23 +123,24 @@
             "workflow for submission {}"
             .format(submission_uuid)
         )
         logger.exception(error_message)
         raise StaffAssessmentInternalError(error_message) from ex
 
 
-def get_score(submission_uuid, staff_requirements):  # pylint: disable=unused-argument
+def get_score(submission_uuid, staff_requirements, course_settings):  # pylint: disable=unused-argument
     """
     Generate a score based on a completed assessment for the given submission.
     If no assessment has been completed for this submission, this will return
     None.
 
     Args:
         submission_uuid (str): The UUID for the submission to get a score for.
         staff_requirements (dict): Not used.
+        course_settings (dict): Not used.
 
     Returns:
         A dictionary with the points earned, points possible,
         contributing_assessments, and staff_id information.
 
     """
     assessment = get_latest_staff_assessment(submission_uuid)
```

### Comparing `ora2-5.1.1/openassessment/assessment/api/student_training.py` & `ora2-5.2.0/openassessment/assessment/api/student_training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/api/teams.py` & `ora2-5.2.0/openassessment/assessment/api/teams.py`

 * *Files 0% similar despite different names*

```diff
@@ -31,15 +31,15 @@
     Returns:
         True
 
     """
     return True
 
 
-def assessment_is_finished(team_submission_uuid, staff_requirements):
+def assessment_is_finished(team_submission_uuid, staff_requirements, _):
     """
     Determine if the staff assessment step of the given team submission is completed.
     This checks to see if staff have completed the assessment.
 
     Args:
         team_submission_uuid (str): The UUID of the submission being graded.
         staff_requirements (dict): Any variables that may effect this state.
@@ -122,23 +122,24 @@
         error_message = (
             "An internal error occurred while cancelling the team staff workflow for submission {}"
         ).format(team_submission_uuid)
         logger.exception(error_message)
         raise StaffAssessmentInternalError(error_message) from ex
 
 
-def get_score(team_submission_uuid, staff_requirements):  # pylint: disable=unused-argument
+def get_score(team_submission_uuid, staff_requirements, course_settings):  # pylint: disable=unused-argument
     """
     Generate a score based on a completed assessment for the given team submission.
     If no assessment has been completed for this submission, this will return
     None.
 
     Args:
         team_submission_uuid (str): The UUID for the submission to get a score for.
         staff_requirements (dict): Not used.
+        course_settings (dict): Not used.
 
     Returns:
         A dictionary with the points earned, points possible,
         contributing_assessments, and staff_id information.
 
     """
     assessment = get_latest_staff_assessment(team_submission_uuid)
```

### Comparing `ora2-5.1.1/openassessment/assessment/errors/peer.py` & `ora2-5.2.0/openassessment/assessment/errors/peer.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/errors/self.py` & `ora2-5.2.0/openassessment/assessment/errors/self.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/errors/staff.py` & `ora2-5.2.0/openassessment/assessment/errors/staff.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/migrations/0001_initial.py` & `ora2-5.2.0/openassessment/assessment/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/migrations/0002_staffworkflow.py` & `ora2-5.2.0/openassessment/assessment/migrations/0002_staffworkflow.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/migrations/0003_expand_course_id.py` & `ora2-5.2.0/openassessment/assessment/migrations/0003_expand_course_id.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py` & `ora2-5.2.0/openassessment/assessment/migrations/0004_historicalsharedfileupload_sharedfileupload.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py` & `ora2-5.2.0/openassessment/assessment/migrations/0005_add_filename_to_sharedupload.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/migrations/0006_TeamWorkflows.py` & `ora2-5.2.0/openassessment/assessment/migrations/0006_TeamWorkflows.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/migrations/0007_staff_workflow_blank.py` & `ora2-5.2.0/openassessment/assessment/migrations/0007_staff_workflow_blank.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/models/base.py` & `ora2-5.2.0/openassessment/assessment/models/base.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/models/peer.py` & `ora2-5.2.0/openassessment/assessment/models/peer.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/models/staff.py` & `ora2-5.2.0/openassessment/assessment/models/staff.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/models/student_training.py` & `ora2-5.2.0/openassessment/assessment/models/student_training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/models/training.py` & `ora2-5.2.0/openassessment/assessment/models/training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/serializers/base.py` & `ora2-5.2.0/openassessment/assessment/serializers/base.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/serializers/peer.py` & `ora2-5.2.0/openassessment/assessment/serializers/peer.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/serializers/training.py` & `ora2-5.2.0/openassessment/assessment/serializers/training.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/assessment/views.py` & `ora2-5.2.0/openassessment/assessment/views.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/data.py` & `ora2-5.2.0/openassessment/data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/fileupload/api.py` & `ora2-5.2.0/openassessment/fileupload/api.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/fileupload/backends/__init__.py` & `ora2-5.2.0/openassessment/fileupload/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/fileupload/backends/base.py` & `ora2-5.2.0/openassessment/fileupload/backends/base.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/fileupload/backends/django_storage.py` & `ora2-5.2.0/openassessment/fileupload/backends/django_storage.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/fileupload/backends/filesystem.py` & `ora2-5.2.0/openassessment/fileupload/backends/filesystem.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/fileupload/backends/s3.py` & `ora2-5.2.0/openassessment/fileupload/backends/s3.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/fileupload/backends/swift.py` & `ora2-5.2.0/openassessment/fileupload/backends/swift.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/fileupload/exceptions.py` & `ora2-5.2.0/openassessment/fileupload/exceptions.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/fileupload/views_filesystem.py` & `ora2-5.2.0/openassessment/fileupload/views_filesystem.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ar/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ar/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ar/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/ar/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ar/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/ar/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/ar_SA/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/de_DE/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/de_DE/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/de_DE/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/de_DE/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/el/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/el/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/el/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/el/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/el/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/el/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/el/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/el/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/en/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/en/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/en/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/eo/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/eo/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/eo/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/eo/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/eo/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/eo/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/eo/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/eo/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/es_419/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/es_419/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/es_419/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/es_419/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/es_419/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/es_419/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/es_419/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/es_AR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/es_AR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/es_ES/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/es_ES/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/es_ES/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/es_ES/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/es_ES/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/es_ES/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/eu_ES/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/eu_ES/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/eu_ES/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/eu_ES/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/eu_ES/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/fa_IR/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/fa_IR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/fa_IR/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/fa_IR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/fa_IR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/fr/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/fr/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/fr/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/fr/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/fr/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/fr/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/fr_CA/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/fr_CA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/fr_CA/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/fr_CA/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/fr_CA/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/he/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/he/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/he/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/he/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/he/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/he/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/he/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/he/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/hi/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/hi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/hi/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/hi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/hi/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/hi/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/hi/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/hi/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/id/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/id/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/id/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/id/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/id/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/id/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/id/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/id/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/it_IT/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/it_IT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/it_IT/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/it_IT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/it_IT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/it_IT/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ja_JP/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/ja_JP/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ja_JP/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/ja_JP/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ka/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/ka/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ka/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/ka/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ka/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/ka/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ka/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/ka/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/lt_LT/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/lt_LT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/lt_LT/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/lt_LT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/lt_LT/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/lv/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/lv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/lv/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/lv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/lv/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/lv/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/lv/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/lv/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/messages.mo` & `ora2-5.2.0/openassessment/locale/messages.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/mn/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/mn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/mn/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/mn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/mn/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/mn/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/mn/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/mn/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/nb/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/nb/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/nb/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/nb/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/nb/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/nb/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/pl/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/pl/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/pl/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/pl/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/pl/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/pl/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/pt_BR/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/pt_BR/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/pt_BR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/pt_PT/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/pt_PT/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/pt_PT/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/pt_PT/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/pt_PT/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ro/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ro/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/ro/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ro/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/ro/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ro/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/ro/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ru/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ru/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ru/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/ru/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/ru/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/ru/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/sk/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/sk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/sk/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/sk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/sq/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/sq/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/sq/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/sq/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/sq/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/sq/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/sq/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/sq/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/sw_KE/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/sw_KE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/sw_KE/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/sw_KE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/sw_KE/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/th/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/th/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/th/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/th/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/th/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/th/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/th/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/th/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/tr_TR/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/tr_TR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/tr_TR/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/tr_TR/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/uk/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/uk/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/uk/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/uk/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/uk/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/uk/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/vi/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/vi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/vi/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/vi/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/vi/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/vi/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/vi/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/zh_CN/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/zh_CN/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/zh_CN/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/zh_TW/LC_MESSAGES/django.mo` & `ora2-5.2.0/openassessment/locale/zh_TW/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/zh_TW/LC_MESSAGES/django.po` & `ora2-5.2.0/openassessment/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo` & `ora2-5.2.0/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.mo`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.po` & `ora2-5.2.0/openassessment/locale/zh_TW/LC_MESSAGES/djangojs.po`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/management/commands/collect_ora2_data.py` & `ora2-5.2.0/openassessment/management/commands/collect_ora2_data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/management/commands/create_oa_submissions.py` & `ora2-5.2.0/openassessment/management/commands/create_oa_submissions.py`

 * *Files 0% similar despite different names*

```diff
@@ -150,15 +150,15 @@
         Returns:
             str: submission UUID
         """
         answer = {'text': "  ".join(loremipsum.get_paragraphs(5))}
         submission = sub_api.create_submission(student_item, answer)
         workflow_api.create_workflow(submission['uuid'], STEPS)
         workflow_api.update_from_assessments(
-            submission['uuid'], {'peer': {'must_grade': 1, 'must_be_graded_by': 1}}
+            submission['uuid'], {'peer': {'must_grade': 1, 'must_be_graded_by': 1}}, {}
         )
         return submission['uuid']
 
     def _dummy_rubric(self):
         """
         Randomly generate a rubric and select options from it.
```

### Comparing `ora2-5.1.1/openassessment/management/commands/create_oa_submissions_from_file.py` & `ora2-5.2.0/openassessment/management/commands/create_oa_submissions_from_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -300,15 +300,15 @@
                     course_id,
                     ora_config['displayName']
                 )
                 # Submissions consist of username, a line break, and then some lorem
                 text_response = submission_config['username'] + '\n' + generate_lorem_sentences()
                 submission = sub_api.create_submission(student_item, {'parts': [{'text': text_response}]})
                 workflow_api.create_workflow(submission['uuid'], ['staff'])
-                workflow_api.update_from_assessments(submission['uuid'], None)
+                workflow_api.update_from_assessments(submission['uuid'], None, {})
                 log.info("Created submission %s for user %s", submission['uuid'], submission_config['username'])
 
                 if submission_config['lockOwner']:
                     log.info(
                         "Creating lock on submission %s owned by %s",
                         submission['uuid'],
                         submission_config['lockOwner']
@@ -332,15 +332,15 @@
                         submission['uuid'],
                         self.username_to_anonymous_user_id[grade_data['gradedBy']],
                         options_selected,
                         criterion_feedback,
                         grade_data['overallFeedback'],
                         rubric_dict,
                     )
-                    workflow_api.update_from_assessments(submission['uuid'], None)
+                    workflow_api.update_from_assessments(submission['uuid'], None, {})
 
     def student_item(self, username, course_id, ora_display_name):
         """Helper for creating student item dicts"""
         return {
             'student_id': self.username_to_anonymous_user_id[username],
             'course_id': str(course_id),
             'item_id': str(self.display_name_to_block[ora_display_name].location),
```

### Comparing `ora2-5.1.1/openassessment/management/commands/upload_oa_data.py` & `ora2-5.2.0/openassessment/management/commands/upload_oa_data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/runtime_imports/classes.py` & `ora2-5.2.0/openassessment/runtime_imports/classes.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/runtime_imports/functions.py` & `ora2-5.2.0/openassessment/runtime_imports/functions.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/staffgrader/admin.py` & `ora2-5.2.0/openassessment/staffgrader/admin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/staffgrader/migrations/0001_initial.py` & `ora2-5.2.0/openassessment/staffgrader/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/staffgrader/models/submission_lock.py` & `ora2-5.2.0/openassessment/staffgrader/models/submission_lock.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/staffgrader/serializers/assessments.py` & `ora2-5.2.0/openassessment/staffgrader/serializers/assessments.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/staffgrader/serializers/submission_list.py` & `ora2-5.2.0/openassessment/staffgrader/serializers/submission_list.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/staffgrader/serializers/submission_lock.py` & `ora2-5.2.0/openassessment/staffgrader/serializers/submission_lock.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/staffgrader/staff_grader_mixin.py` & `ora2-5.2.0/openassessment/staffgrader/staff_grader_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_assessment_steps.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_basic_settings_list.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_criterion.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_header_and_validation.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_option.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_option.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_peer_assessment_schedule.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_prompt.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_prompts.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_rubric.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_schedule.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_self_assessment_schedule.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_staff_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_edit_student_training.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_rubric_reuse.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_training_example.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_training_example.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/edit/oa_training_example_criterion.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/grade/oa_assessment_feedback.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/grade/oa_assessment_title.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/grade/oa_grade_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/grade/oa_grade_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/grade/oa_grade_incomplete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/grade/oa_grade_not_started.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/grade/oa_grade_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_grade_available_responses.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_listing.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/instructor_dashboard/oa_waiting_step_details.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_show.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/leaderboard/oa_leaderboard_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/message/oa_message_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/message/oa_message_closed.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/message/oa_message_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/message/oa_message_complete.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/message/oa_message_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/message/oa_message_incomplete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/message/oa_message_no_team.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/message/oa_message_no_team.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/message/oa_message_open.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/message/oa_message_open.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/oa_base.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/oa_base.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/oa_latex_preview.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/oa_latex_preview.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/oa_rubric.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/oa_rubric.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/oa_submission_answer.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/oa_submission_answer.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/oa_team_uploaded_files.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/oa_uploaded_file.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/oa_uploaded_file.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_turbo_mode_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/peer/oa_peer_waiting.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/response/oa_response.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/response/oa_response.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/response/oa_response_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/response/oa_response_closed.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/response/oa_response_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/response/oa_response_graded.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/response/oa_response_graded.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/response/oa_response_submitted.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/response/oa_response_submitted.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/response/oa_response_team_already_submitted.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/response/oa_response_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/self/oa_self_assessment.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/self/oa_self_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/self/oa_self_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/self/oa_self_closed.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/self/oa_self_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/self/oa_self_complete.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/self/oa_self_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/self/oa_self_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/staff/oa_staff_grade.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_area.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_grade_learners_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/staff_area/oa_staff_override_assessment.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/staff_area/oa_student_info.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/staff_area/oa_student_info_assessment_detail.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/student_training/student_training.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/student_training/student_training.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/student_training/student_training_cancelled.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/student_training/student_training_closed.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/student_training/student_training_closed.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/student_training/student_training_complete.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/student_training/student_training_complete.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/student_training/student_training_error.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/student_training/student_training_error.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html` & `ora2-5.2.0/openassessment/templates/openassessmentblock/student_training/student_training_unavailable.html`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/templatetags/oa_extras.py` & `ora2-5.2.0/openassessment/templatetags/oa_extras.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/test_utils.py` & `ora2-5.2.0/openassessment/test_utils.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/workflow/admin.py` & `ora2-5.2.0/openassessment/workflow/admin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/workflow/api.py` & `ora2-5.2.0/openassessment/workflow/api.py`

 * *Files 5% similar despite different names*

```diff
@@ -96,15 +96,15 @@
             "An unexpected error occurred while creating "
             "the workflow for submission UUID {}"
         ).format(submission_uuid)
         logger.exception(err_msg)
         raise AssessmentWorkflowInternalError(err_msg) from ex
 
 
-def get_workflow_for_submission(submission_uuid, assessment_requirements):
+def get_workflow_for_submission(submission_uuid, assessment_requirements, course_settings):
     """Returns Assessment Workflow information
 
     This will implicitly call `update_from_assessments()` to make sure we
     give the most current information. Unlike `create_workflow()`, this function
     will check our assessment sequences to see if they are complete. We pass
     in the `assessment_requirements` each time we make the request because the
     canonical requirements are stored in the `OpenAssessmentBlock` problem
@@ -171,18 +171,23 @@
                 'self': {
                     'complete': False
                 }
             }
         }
 
     """
-    return update_from_assessments(submission_uuid, assessment_requirements)
+    return update_from_assessments(submission_uuid, assessment_requirements, course_settings)
 
 
-def update_from_assessments(submission_uuid, assessment_requirements, override_submitter_requirements=False):
+def update_from_assessments(
+    submission_uuid,
+    assessment_requirements,
+    course_settings,
+    override_submitter_requirements=False
+):
     """
     Update our workflow status based on the status of the underlying assessments.
 
     We pass in the `assessment_requirements` each time we make the request
     because the canonical requirements are stored in the `OpenAssessmentBlock`
     problem definition and may change over time. Because this method also
     returns a copy of the `WorkflowAssessment` information as a convenience,
@@ -266,19 +271,24 @@
             }
         }
 
     """
     workflow = _get_workflow_model(submission_uuid)
 
     try:
-        workflow.update_from_assessments(assessment_requirements, override_submitter_requirements)
+        workflow.update_from_assessments(
+            assessment_requirements,
+            course_settings,
+            override_submitter_requirements
+        )
         logger.info(
-            "Updated workflow for submission UUID %s with requirements %s",
+            "Updated workflow for submission UUID %s with requirements %s and course setttings %s",
             submission_uuid,
-            assessment_requirements
+            assessment_requirements,
+            course_settings
         )
         return _serialized_with_details(workflow)
     except PeerAssessmentError as err:
         err_msg = "Could not update assessment workflow: %s"
         logger.exception(err_msg, err)
         raise AssessmentWorkflowInternalError(err_msg % err) from err
 
@@ -380,15 +390,15 @@
     Given a workflow, return its serialized version with added status details.
     """
     data_dict = AssessmentWorkflowSerializer(workflow).data
     data_dict["status_details"] = workflow.status_details()
     return data_dict
 
 
-def cancel_workflow(submission_uuid, comments, cancelled_by_id, assessment_requirements):
+def cancel_workflow(submission_uuid, comments, cancelled_by_id, assessment_requirements, course_settings):
     """
     Add an entry in AssessmentWorkflowCancellation table for a AssessmentWorkflow.
 
     AssessmentWorkflow which has been cancelled is no longer included in the
     peer grading pool.
 
     Args:
@@ -399,16 +409,23 @@
             `{"peer": {"must_grade": <int>, "must_be_graded_by": <int>}}`
             `must_grade` is the number of assessments a student must complete.
             `must_be_graded_by` is the number of assessments a submission must
             receive to be scored. `must_grade` should be greater than
             `must_be_graded_by` to ensure that everyone will get scored.
             The intention is to eventually pass in more assessment sequence
             specific requirements in this dict.
+        course_settings (dict): Dictionary that contains course-level settings that
+                                impact workflow steps
     """
-    AssessmentWorkflow.cancel_workflow(submission_uuid, comments, cancelled_by_id, assessment_requirements)
+    AssessmentWorkflow.cancel_workflow(
+        submission_uuid,
+        comments, cancelled_by_id,
+        assessment_requirements,
+        course_settings
+    )
 
 
 def get_assessment_workflow_cancellation(submission_uuid):
     """
     Get cancellation information for an assessment workflow.
 
     Args:
```

### Comparing `ora2-5.1.1/openassessment/workflow/errors.py` & `ora2-5.2.0/openassessment/workflow/errors.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/workflow/migrations/0001_initial.py` & `ora2-5.2.0/openassessment/workflow/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/workflow/migrations/0003_TeamWorkflows.py` & `ora2-5.2.0/openassessment/workflow/migrations/0003_TeamWorkflows.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/workflow/models.py` & `ora2-5.2.0/openassessment/workflow/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,14 @@
             SubmissionNotFoundError
             SubmissionRequestError
             SubmissionInternalError
             DatabaseError
             Assessment-module specific errors
         """
         submission_dict = sub_api.get_submission_and_student(submission_uuid)
-
         staff_auto_added = False
         if 'staff' not in step_names:
             staff_auto_added = True
             new_list = ['staff']
             new_list.extend(step_names)
             step_names = new_list
 
@@ -199,15 +198,15 @@
 
                     # Remember that we've already started the first step
                     has_started_first_step = True
 
         # Update the workflow (in case some of the assessment modules are automatically complete)
         # We do NOT pass in requirements, on the assumption that any assessment module
         # that accepts requirements would NOT automatically complete.
-        workflow.update_from_assessments(None)
+        workflow.update_from_assessments(None, {})
 
         # Return the newly created workflow
         return workflow
 
     @property
     def score(self):
         """Latest score for the submission we're tracking.
@@ -243,15 +242,15 @@
                 # the number passed here is arbitrary and ignored
                 _, peers_graded_count = step.api().has_finished_required_evaluating(self.submission_uuid, 1)
                 graded_by_count = step.api().get_graded_by_count(self.submission_uuid)
                 status_dict[step.name]['peers_graded_count'] = peers_graded_count
                 status_dict[step.name]['graded_by_count'] = graded_by_count
         return status_dict
 
-    def get_score(self, assessment_requirements, step_for_name):
+    def get_score(self, assessment_requirements, course_settings, step_for_name):
         """Iterate through the assessment APIs in priority order
          and return the first reported score.
 
         Args:
             assessment_requirements (dict): Dictionary passed to the assessment API.
                 This defines the requirements for each assessment step; the APIs
                 can refer to this to decide whether the requirements have been
@@ -275,24 +274,29 @@
                 # Check if the assessment API defines a score function at all
                 get_score_func = getattr(assessment_step.api(), 'get_score', None)
                 if get_score_func is not None:
                     if assessment_requirements is None:
                         step_requirements = None
                     else:
                         step_requirements = assessment_requirements.get(assessment_step_name, {})
-                    score = get_score_func(self.identifying_uuid, step_requirements)
+                    score = get_score_func(self.identifying_uuid, step_requirements, course_settings)
                     if not score and assessment_step.is_staff_step():
                         if step_requirements and step_requirements.get('required', False):
                             break  # A staff score was not found, and one is required. Return None
                         continue  # A staff score was not found, but it is not required, so try the next type of score
                     break
 
         return score
 
-    def update_from_assessments(self, assessment_requirements, override_submitter_requirements=False):
+    def update_from_assessments(
+        self,
+        assessment_requirements,
+        course_settings,
+        override_submitter_requirements=False
+    ):
         """Query assessment APIs and change our status if appropriate.
 
         If the status is done, we do nothing. Once something is done, we never
         move back to any other status.
 
         If an assessment API says that our submitter's requirements are met, or if
         current assessment step can be skipped, then move to the next assessment.
@@ -323,28 +327,31 @@
 
         Args:
             assessment_requirements (dict): Dictionary passed to the assessment API.
                 This defines the requirements for each assessment step; the APIs
                 can refer to this to decide whether the requirements have been
                 met.  Note that the requirements could change if the author
                 updates the problem definition.
+            course_settings (dict): Any course-level settings that may impact the
+                workflow update process.
             override_submitter_requirements (bool): If True, the presence of a new
                 staff score will cause all of the submitter's requirements to be
                 fulfilled, moving the workflow to DONE and exposing their grade.
         """
         if self.status == self.STATUS.cancelled:
             return
 
         # Update our AssessmentWorkflowStep models with the latest from our APIs
         steps = self._get_steps()
 
         step_for_name = {step.name: step for step in steps}
 
         new_staff_score = self.get_score(
             assessment_requirements,
+            course_settings,
             {self.STAFF_STEP_NAME: step_for_name.get(self.STAFF_STEP_NAME, None)}
         )
         if new_staff_score:
             # new_staff_score is just the most recent staff score, it may already be recorded in sub_api
             old_score = sub_api.get_latest_score_for_submission(self.submission_uuid)
             if (
                     # Does a prior score exist? Is it a staff score? Do the points earned match?
@@ -371,15 +378,15 @@
                     step.save()
 
         if self.status == self.STATUS.done:
             return
 
         # Go through each step and update its status.
         for step in steps:
-            step.update(self.submission_uuid, assessment_requirements)
+            step.update(self.submission_uuid, assessment_requirements, course_settings)
 
         possible_statuses = []
         skipped_statuses = []
         all_statuses = []
 
         # find which are the next unskippable steps and steps that can be skipped
         for step in steps:
@@ -416,18 +423,24 @@
 
         # If the submitter is beginning the next assessment, notify the
         # appropriate assessment API.
         new_step = step_for_name.get(new_status)
         if new_step is not None:
             new_step.start(self.submission_uuid)
 
+        # If the submitter is beginning the next assessment, notify the
+        # appropriate assessment API.
+        new_step = step_for_name.get(new_status)
+        if new_step is not None:
+            new_step.start(self.submission_uuid)
+
         # If the submitter has done all they need to do, let's check to see if
         # all steps have been fully assessed (i.e. we can score it).
         if new_status == self.STATUS.waiting and all(step.assessment_completed_at for step in steps):
-            score = self.get_score(assessment_requirements, step_for_name)
+            score = self.get_score(assessment_requirements, course_settings, step_for_name)
             # If we found a score, then we're done
             if score is not None:
                 # Only set the score if it's not a staff score, in which case it will have already been set above
                 if score.get("staff_id") is None:
                     self.set_score(score)
                 new_status = self.STATUS.done
 
@@ -538,15 +551,15 @@
             get_latest_func = getattr(staff_step.api(), 'get_latest_assessment', None)
             if get_latest_func is not None:
                 staff_assessment = get_latest_func(self.submission_uuid)
                 if staff_assessment is not None:
                     return True
         return False
 
-    def cancel(self, assessment_requirements):
+    def cancel(self, assessment_requirements, course_settings):
         """
         Cancel workflow for all steps.
 
         Set the points earned to 0 and workflow status to cancelled.
 
         Args:
             assessment_requirements (dict): Dictionary that currently looks like:
@@ -564,15 +577,15 @@
         # Cancel the workflow for each step.
         for step in steps:
             on_cancel_func = getattr(step.api(), 'on_cancel', None)
             if on_cancel_func is not None:
                 on_cancel_func(self.identifying_uuid)
 
         try:
-            score = self.get_score(assessment_requirements, step_for_name)
+            score = self.get_score(assessment_requirements, course_settings, step_for_name)
         except AssessmentError as exc:
             logger.info("TNL-5799, exception in get_score during cancellation. %s", exc)
             score = None
 
         # Set the points_earned to 0.
         if score is not None:
             score['points_earned'] = 0
@@ -585,15 +598,15 @@
             logger.info(
                 "Workflow for submission UUID %s has updated status to %s",
                 self.submission_uuid,
                 self.STATUS.cancelled
             )
 
     @classmethod
-    def cancel_workflow(cls, submission_uuid, comments, cancelled_by_id, assessment_requirements):
+    def cancel_workflow(cls, submission_uuid, comments, cancelled_by_id, assessment_requirements, course_settings):
         """
         Add an entry in AssessmentWorkflowCancellation table for a AssessmentWorkflow.
 
         AssessmentWorkflow which has been cancelled is no longer included in the
         peer grading pool.
 
         Args:
@@ -604,20 +617,22 @@
             `{"peer": {"must_grade": <int>, "must_be_graded_by": <int>}}`
             `must_grade` is the number of assessments a student must complete.
             `must_be_graded_by` is the number of assessments a submission must
             receive to be scored. `must_grade` should be greater than
             `must_be_graded_by` to ensure that everyone will get scored.
             The intention is to eventually pass in more assessment sequence
             specific requirements in this dict.
+            course_settings (dict): Dictionary that contains course-level settings that
+            impact workflow steps
         """
         try:
             workflow = cls.objects.get(submission_uuid=submission_uuid)
             AssessmentWorkflowCancellation.create(workflow=workflow, comments=comments, cancelled_by_id=cancelled_by_id)
             # Cancel the related step's workflow.
-            workflow.cancel(assessment_requirements)
+            workflow.cancel(assessment_requirements, course_settings)
         except (cls.DoesNotExist, cls.MultipleObjectsReturned) as ex:
             error_message = f"Error finding workflow for submission UUID {submission_uuid}."
             logger.exception(error_message)
             raise AssessmentWorkflowError(error_message) from ex
         except DatabaseError as ex:
             error_message = "Error creating assessment workflow cancellation for submission UUID {}.".format(
                 submission_uuid)
@@ -767,15 +782,15 @@
         Update the workflow with potential new scores from assessments.
         """
         if self.status == self.STATUS.cancelled:
             return
 
         team_staff_step = self._team_staff_step
         team_staff_api = team_staff_step.api()
-        new_score = team_staff_api.get_score(self.team_submission_uuid, self.REQUIREMENTS)
+        new_score = team_staff_api.get_score(self.team_submission_uuid, self.REQUIREMENTS, {})
         if new_score:
             # new_score is just the most recent team score, it may already be recorded in sub_api
             old_score = sub_api.get_latest_score_for_submission(self.submission_uuid)
             if (
                     # Does a prior score exist?  Do the points earned match?
                     not old_score or self.STAFF_ANNOTATION_TYPE not in [
                         annotation['annotation_type'] for annotation in old_score['annotations']
@@ -790,15 +805,15 @@
                 )
                 common_now = now()
                 team_staff_step.assessment_completed_at = common_now
                 team_staff_step.save()
 
             if override_submitter_requirements:
                 team_staff_step.submitter_completed_at = common_now
-            team_staff_step.update(self.team_submission_uuid, self.REQUIREMENTS)
+            team_staff_step.update(self.team_submission_uuid, self.REQUIREMENTS, {})
             self.status = self.STATUS.done
             self.save()
 
     def _set_team_staff_score(self, score):
         reason = "A staff member has defined the score for this submission"
         sub_team_api.set_score(
             self.team_submission_uuid,
@@ -916,15 +931,15 @@
             msg = (
                 "No assessment configured for '{name}'.  "
                 "Check the ORA2_ASSESSMENTS Django setting."
             ).format(name=self.name)
             logger.warning(msg)
             return None
 
-    def update(self, submission_uuid, assessment_requirements):
+    def update(self, submission_uuid, assessment_requirements, course_settings):
         """
         Updates the AssessmentWorkflowStep models with the requirements
         specified from the Workflow API.
 
         Intended for internal use by update_from_assessments(). See
         update_from_assessments() documentation for more details.
         """
@@ -943,15 +958,15 @@
 
         # Has the user completed their obligations for this step?
         if not self.is_submitter_complete() and submitter_finished(submission_uuid, step_reqs):
             self.submitter_completed_at = now()
             step_changed = True
 
         # Has the step received a score?
-        if not self.is_assessment_complete() and assessment_finished(submission_uuid, step_reqs):
+        if not self.is_assessment_complete() and assessment_finished(submission_uuid, step_reqs, course_settings):
             self.assessment_completed_at = now()
             step_changed = True
 
         if step_changed:
             self.save()
 
 
@@ -975,15 +990,15 @@
     submission_uuid = kwargs.get('submission_uuid')
     if submission_uuid is None:
         logger.error("Update workflow signal called without a submission UUID")
         return
 
     try:
         workflow = AssessmentWorkflow.objects.get(submission_uuid=submission_uuid)
-        workflow.update_from_assessments(None)
+        workflow.update_from_assessments(None, {})
     except AssessmentWorkflow.DoesNotExist:
         msg = f"Could not retrieve workflow for submission with UUID {submission_uuid}"
         logger.exception(msg)
     except DatabaseError:
         msg = (
             "Database error occurred while updating "
             "the workflow for submission UUID {}"
```

### Comparing `ora2-5.1.1/openassessment/workflow/serializers.py` & `ora2-5.2.0/openassessment/workflow/serializers.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/workflow/team_api.py` & `ora2-5.2.0/openassessment/workflow/team_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -63,14 +63,17 @@
 def update_from_assessments(team_submission_uuid, override_submitter_requirements=False):
     """
         Like `api.update_from_assessments`, but for teams.  We don't need
         an analogous `assessment_requirements` parameter, because team submissions
         are only assessible by staff (where requirements like "must_grade" and
         "must_be_graded_by" are not supported).
 
+        We also don't need an analogous `course_settings` parameter because there are
+        currently no course settings that impact staff grading.
+
         Raises:
             AssessmentWorkflowInternalError on error
         """
     # Get the wokflow for this submission
     team_workflow = _get_workflow_model(team_submission_uuid)
 
     # Update the workflow status based on the underlying assessments
@@ -183,15 +186,16 @@
     """
     try:
         submission_uuid = _get_workflow_model(team_submission_uuid).submission_uuid
         TeamAssessmentWorkflow.cancel_workflow(
             submission_uuid,
             comments,
             cancelled_by_id,
-            TeamAssessmentWorkflow.REQUIREMENTS
+            TeamAssessmentWorkflow.REQUIREMENTS,
+            {}
         )
     except Exception as exc:
         err_msg = (
             "Could not cancel team assessment workflow with team_submission_uuid {uuid} due to error: {exc}"
         ).format(uuid=team_submission_uuid, exc=exc)
         logger.exception(err_msg)
         raise AssessmentWorkflowInternalError(err_msg) from exc
```

### Comparing `ora2-5.1.1/openassessment/xblock/config_mixin.py` & `ora2-5.2.0/openassessment/xblock/config_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/course_items_listing_mixin.py` & `ora2-5.2.0/openassessment/xblock/course_items_listing_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/data_conversion.py` & `ora2-5.2.0/openassessment/xblock/data_conversion.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/defaults.py` & `ora2-5.2.0/openassessment/xblock/defaults.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/editor_config.py` & `ora2-5.2.0/openassessment/xblock/editor_config.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/grade_mixin.py` & `ora2-5.2.0/openassessment/xblock/grade_mixin.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,19 @@
         staff_assessment = None
         self_assessment = None
         feedback = None
         peer_assessments = []
         has_submitted_feedback = False
 
         if "peer-assessment" in assessment_steps:
-            peer_api.get_score(submission_uuid, self.workflow_requirements()["peer"])
+            peer_api.get_score(
+                submission_uuid,
+                self.workflow_requirements()["peer"],
+                self.get_course_workflow_settings()
+            )
             feedback = peer_api.get_assessment_feedback(submission_uuid)
             peer_assessments = [
                 self._assessment_grade_context(peer_assessment)
                 for peer_assessment in peer_api.get_assessments(submission_uuid)
             ]
             has_submitted_feedback = feedback is not None
```

### Comparing `ora2-5.1.1/openassessment/xblock/leaderboard_mixin.py` & `ora2-5.2.0/openassessment/xblock/leaderboard_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/lms_mixin.py` & `ora2-5.2.0/openassessment/xblock/lms_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/load_static.py` & `ora2-5.2.0/openassessment/xblock/load_static.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/message_mixin.py` & `ora2-5.2.0/openassessment/xblock/message_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/mobile.py` & `ora2-5.2.0/openassessment/xblock/mobile.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/openassesment_template_mixin.py` & `ora2-5.2.0/openassessment/xblock/openassesment_template_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/openassessmentblock.py` & `ora2-5.2.0/openassessment/xblock/openassessmentblock.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """An XBlock where students can read a question and compose their response"""
 
 import copy
 import datetime as dt
+from functools import cached_property
 import json
 import logging
 import os
 import re
 
 import pkg_resources
 import pytz
@@ -306,14 +307,20 @@
         help="Should the rubric be visible to learners in the response section?"
     )
 
     @property
     def course_id(self):
         return str(self.xmodule_runtime.course_id)  # pylint: disable=no-member
 
+    @cached_property
+    def course(self):
+        if not hasattr(self.runtime, "modulestore"):
+            return None
+        return self.runtime.modulestore.get_course(self.scope_ids.usage_id.context_key)
+
     @property
     def text_response(self):
         """
         Backward compatibility for existing blocks that were created without text_response
         or file_upload_response fields. These blocks will be treated as required text.
         """
         if not self.file_upload_response_raw and not self.text_response_raw:
```

### Comparing `ora2-5.1.1/openassessment/xblock/peer_assessment_mixin.py` & `ora2-5.2.0/openassessment/xblock/peer_assessment_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/resolve_dates.py` & `ora2-5.2.0/openassessment/xblock/resolve_dates.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/rubric_reuse_mixin.py` & `ora2-5.2.0/openassessment/xblock/rubric_reuse_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/schema.py` & `ora2-5.2.0/openassessment/xblock/schema.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/self_assessment_mixin.py` & `ora2-5.2.0/openassessment/xblock/self_assessment_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/staff_area_mixin.py` & `ora2-5.2.0/openassessment/xblock/staff_area_mixin.py`

 * *Files 2% similar despite different names*

```diff
@@ -522,15 +522,19 @@
         grade_exists = workflow.get('status') == "done"
         grade_utils = self.runtime._services.get('grade_utils')  # pylint: disable=protected-access
 
         if "peer-assessment" in assessment_steps:
             peer_assessments = peer_api.get_assessments(submission_uuid)
             submitted_assessments = peer_api.get_submitted_assessments(submission_uuid)
             if grade_exists:
-                peer_api.get_score(submission_uuid, self.workflow_requirements()["peer"])
+                peer_api.get_score(
+                    submission_uuid,
+                    self.workflow_requirements()["peer"],
+                    self.get_course_workflow_settings()
+                )
                 peer_assessments_grade_context = [
                     self._assessment_grade_context(peer_assessment)
                     for peer_assessment in peer_assessments
                 ]
 
         if "self-assessment" in assessment_steps:
             self_assessment = self_api.get_assessment(submission_uuid)
@@ -702,22 +706,24 @@
 
         If requesting_user is not provided, we will use the user to which this xblock is currently bound.
         """
         # Import is placed here to avoid model import at project startup.
         from openassessment.workflow import api as workflow_api
         try:
             assessment_requirements = self.workflow_requirements()
+            course_settings = self.get_course_workflow_settings()
             if requesting_user_id is None:
                 # The student_id is actually the bound user, which is the staff user in this context.
                 requesting_user_id = self.get_student_item_dict()["student_id"]
             # Cancel the related workflow.
             workflow_api.cancel_workflow(
                 submission_uuid=submission_uuid, comments=comments,
                 cancelled_by_id=requesting_user_id,
-                assessment_requirements=assessment_requirements
+                assessment_requirements=assessment_requirements,
+                course_settings=course_settings,
             )
             return {
                 "success": True,
                 'msg': self._(
                     "The learner submission has been removed from peer assessment. "
                     "The learner receives a grade of zero unless you delete "
                     "the learner's state for the problem to allow them to "
```

### Comparing `ora2-5.1.1/openassessment/xblock/staff_assessment_mixin.py` & `ora2-5.2.0/openassessment/xblock/staff_assessment_mixin.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
                 create_rubric_dict(self.prompts, self.rubric_criteria_with_labels)
             )
             assess_type = data.get('assess_type', 'regrade')
             self.publish_assessment_event("openassessmentblock.staff_assess", assessment, type=assess_type)
             workflow_api.update_from_assessments(
                 assessment["submission_uuid"],
                 None,
+                {},
                 override_submitter_requirements=(assess_type == 'regrade')
             )
         except StaffAssessmentRequestError:
             logger.warning(
                 "An error occurred while submitting a staff assessment "
                 "for the submission %s",
                 data['submission_uuid'],
```

### Comparing `ora2-5.1.1/openassessment/xblock/static/css/lib/backgrid/backgrid.css` & `ora2-5.2.0/openassessment/xblock/static/css/lib/backgrid/backgrid.css`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css` & `ora2-5.2.0/openassessment/xblock/static/css/lib/backgrid/backgrid.min.css`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/manifest.json` & `ora2-5.2.0/openassessment/xblock/static/dist/manifest.json`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-editor-textarea.b8f866ba96a1d2ad92a4.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-editor-textarea.b8f866ba96a1d2ad92a4.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-editor-textarea.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-editor-textarea.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-editor-tinymce.2cc0cab55c3be729265e.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-editor-tinymce.2cc0cab55c3be729265e.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-editor-tinymce.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-editor-tinymce.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-lms.967dad15c001a5dc6a5e.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-lms.967dad15c001a5dc6a5e.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-lms.e009f195cfd3e23b44e3.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-lms.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-lms.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.css` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.css`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-ltr.af4f203c872dac1a24b5.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-ltr.b9eeb00dfc7524a80658.css` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-ltr.b9eeb00dfc7524a80658.css`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-ltr.b9eeb00dfc7524a80658.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-ltr.b9eeb00dfc7524a80658.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-ltr.css` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-ltr.css`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-ltr.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-ltr.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.css` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.css`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-rtl.b8d173da7a201af6385c.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-rtl.css` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-rtl.css`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-rtl.ef543a27286a069bd958.css` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-rtl.ef543a27286a069bd958.css`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-rtl.ef543a27286a069bd958.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-rtl.ef543a27286a069bd958.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-rtl.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-rtl.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-studio.13c817d25360969539ff.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-studio.13c817d25360969539ff.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-studio.1ef78b4390a9cfa2e9b1.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-studio.1ef78b4390a9cfa2e9b1.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/dist/openassessment-studio.js` & `ora2-5.2.0/openassessment/xblock/static/dist/openassessment-studio.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/lib/backgrid/backgrid.js` & `ora2-5.2.0/openassessment/xblock/static/js/lib/backgrid/backgrid.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js` & `ora2-5.2.0/openassessment/xblock/static/js/lib/backgrid/backgrid.min.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/api/waiting_step_details.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/editors/oa_editor_textarea.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/editors/oa_editor_tinymce.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_base.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_base.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_confirmation_alert.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_course_items_listing.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_datefactory.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_datefactory.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_file_upload.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_file_upload.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_grade.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_grade.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_leaderboard.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_leaderboard.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_message.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_message.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_peer.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_peer.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_prompts.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_prompts.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_response.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_response.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_response_editor.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_response_editor.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_rubric.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_rubric.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_self.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_self.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_staff.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_staff.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_staff_area.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_staff_area.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/lms/oa_training.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/lms/oa_training.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/oa_server.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/oa_server.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/oa_shared.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/oa_shared.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_container.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_container.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_container_item.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_container_item.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_assessment.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_assessments_steps.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_fields.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_fields.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_listeners.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_notifier.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_prompts.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_rubric.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_schedule.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_settings.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_settings.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_edit_validation_alert.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js` & `ora2-5.2.0/openassessment/xblock/static/js/src/studio/oa_tiny_mce.js`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/student_training_mixin.py` & `ora2-5.2.0/openassessment/xblock/student_training_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/studio_mixin.py` & `ora2-5.2.0/openassessment/xblock/studio_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/submission_mixin.py` & `ora2-5.2.0/openassessment/xblock/submission_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/team_mixin.py` & `ora2-5.2.0/openassessment/xblock/team_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/team_workflow_mixin.py` & `ora2-5.2.0/openassessment/xblock/team_workflow_mixin.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/user_data.py` & `ora2-5.2.0/openassessment/xblock/user_data.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/validation.py` & `ora2-5.2.0/openassessment/xblock/validation.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/openassessment/xblock/workflow_mixin.py` & `ora2-5.2.0/openassessment/xblock/workflow_mixin.py`

 * *Files 5% similar despite different names*

```diff
@@ -84,14 +84,31 @@
         if staff_assessment_module:
             requirements["staff"] = {
                 "required": staff_assessment_module["required"]
             }
 
         return requirements
 
+    def get_course_workflow_settings(self):
+        """
+        Retrieve any course-level information that may be needed for workflow updates
+
+        Returns:
+        {
+            'force_on_flexible_peer_openassessments': (bool) the value of the field of the same name on the course
+        }
+        """
+        course_settings = {}
+        peer_assessment_module = self.get_assessment_module('peer-assessment')
+        if peer_assessment_module and self.course is not None:
+            course_settings['force_on_flexible_peer_openassessments'] = \
+                self.course.force_on_flexible_peer_openassessments
+
+        return course_settings
+
     def update_workflow_status(self, submission_uuid=None):
         """
         Update the status of a workflow.  For example, change the status
         from peer-assessment to self-assessment.  Creates a score
         if the student has completed all requirements.
 
         Keyword Arguments:
@@ -105,15 +122,16 @@
             AssessmentWorkflowError
         """
         if submission_uuid is None:
             submission_uuid = self.submission_uuid
 
         if submission_uuid is not None:
             requirements = self.workflow_requirements()
-            workflow_api.update_from_assessments(submission_uuid, requirements)
+            course_settings = self.get_course_workflow_settings()
+            workflow_api.update_from_assessments(submission_uuid, requirements, course_settings)
 
     def get_workflow_info(self, submission_uuid=None):
         """
         Retrieve a description of the student's progress in a workflow.
         Note that this *may* update the workflow status if it's changed.
 
         Keyword Arguments:
@@ -135,15 +153,17 @@
 
         if submission_uuid is None:
             submission_uuid = self.get_submission_uuid()
 
         if submission_uuid is None:
             return {}
         return workflow_api.get_workflow_for_submission(
-            submission_uuid, self.workflow_requirements()
+            submission_uuid,
+            self.workflow_requirements(),
+            self.get_course_workflow_settings()
         )
 
     def get_submission_uuid(self):
         """ Submission UUIDs can be in multiple spots based on the submission type,
             try the various locations to try to find it.
 
             No submission ID will be found if a learner has not submitted a response
```

### Comparing `ora2-5.1.1/openassessment/xblock/xml.py` & `ora2-5.2.0/openassessment/xblock/xml.py`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/ora2.egg-info/PKG-INFO` & `ora2-5.2.0/ora2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ora2
-Version: 5.1.1
+Version: 5.2.0
 Summary: edx-ora2
 Home-page: http://github.com/openedx/edx-ora2
 Author: edX
 Author-email: oscm@edx.org
 License: AGPL
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `ora2-5.1.1/ora2.egg-info/SOURCES.txt` & `ora2-5.2.0/ora2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/requirements/test.in` & `ora2-5.2.0/requirements/test.in`

 * *Files identical despite different names*

### Comparing `ora2-5.1.1/setup.py` & `ora2-5.2.0/setup.py`

 * *Files identical despite different names*

