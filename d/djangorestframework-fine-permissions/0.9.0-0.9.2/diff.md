# Comparing `tmp/djangorestframework-fine-permissions-0.9.0.tar.gz` & `tmp/djangorestframework-fine-permissions-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangorestframework-fine-permissions-0.9.0.tar", last modified: Thu Jul  1 12:30:22 2021, max compression
+gzip compressed data, was "dist/djangorestframework-fine-permissions-0.9.2.tar", last modified: Tue Jul 18 12:19:07 2023, max compression
```

## Comparing `djangorestframework-fine-permissions-0.9.0.tar` & `djangorestframework-fine-permissions-0.9.2.tar`

### file list

```diff
@@ -1,57 +1,58 @@
-drwxr-xr-x   0 karma     (1000) users      (100)        0 2021-07-01 12:30:22.117972 djangorestframework-fine-permissions-0.9.0/
--rw-r--r--   0 karma     (1000) users      (100)    18026 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/LICENSE
--rw-r--r--   0 karma     (1000) users      (100)      217 2021-07-01 12:25:51.000000 djangorestframework-fine-permissions-0.9.0/MANIFEST.in
--rw-r--r--   0 karma     (1000) users      (100)     7284 2021-07-01 12:30:22.117972 djangorestframework-fine-permissions-0.9.0/PKG-INFO
--rw-r--r--   0 karma     (1000) users      (100)     6156 2021-07-01 12:21:50.000000 djangorestframework-fine-permissions-0.9.0/README.rst
-drwxr-xr-x   0 karma     (1000) users      (100)        0 2021-07-01 12:30:22.114971 djangorestframework-fine-permissions-0.9.0/djangorestframework_fine_permissions.egg-info/
--rw-r--r--   0 karma     (1000) users      (100)     7284 2021-07-01 12:30:22.000000 djangorestframework-fine-permissions-0.9.0/djangorestframework_fine_permissions.egg-info/PKG-INFO
--rw-r--r--   0 karma     (1000) users      (100)     1624 2021-07-01 12:30:22.000000 djangorestframework-fine-permissions-0.9.0/djangorestframework_fine_permissions.egg-info/SOURCES.txt
--rw-r--r--   0 karma     (1000) users      (100)        1 2021-07-01 12:30:22.000000 djangorestframework-fine-permissions-0.9.0/djangorestframework_fine_permissions.egg-info/dependency_links.txt
--rw-r--r--   0 karma     (1000) users      (100)        4 2021-07-01 12:30:22.000000 djangorestframework-fine-permissions-0.9.0/djangorestframework_fine_permissions.egg-info/requires.txt
--rw-r--r--   0 karma     (1000) users      (100)       32 2021-07-01 12:30:22.000000 djangorestframework-fine-permissions-0.9.0/djangorestframework_fine_permissions.egg-info/top_level.txt
-drwxr-xr-x   0 karma     (1000) users      (100)        0 2021-07-01 12:30:22.114971 djangorestframework-fine-permissions-0.9.0/docs/
--rw-r--r--   0 karma     (1000) users      (100)    34281 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/docs/admin1.png
--rw-r--r--   0 karma     (1000) users      (100)    47625 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/docs/admin2.png
--rw-r--r--   0 karma     (1000) users      (100)        4 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/requirements.txt
-drwxr-xr-x   0 karma     (1000) users      (100)        0 2021-07-01 12:30:22.115971 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/
--rw-r--r--   0 karma     (1000) users      (100)        0 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/__init__.py
--rw-r--r--   0 karma     (1000) users      (100)     6256 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/admin.py
--rw-r--r--   0 karma     (1000) users      (100)     2317 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/fields.py
--rw-r--r--   0 karma     (1000) users      (100)     1170 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/filters.py
-drwxr-xr-x   0 karma     (1000) users      (100)        0 2021-07-01 12:30:22.115971 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/management/
--rw-r--r--   0 karma     (1000) users      (100)        0 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/management/__init__.py
-drwxr-xr-x   0 karma     (1000) users      (100)        0 2021-07-01 12:30:22.116971 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/management/commands/
--rw-r--r--   0 karma     (1000) users      (100)        0 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/management/commands/__init__.py
--rw-r--r--   0 karma     (1000) users      (100)     1694 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/management/commands/fine_permissions_dump.py
--rw-r--r--   0 karma     (1000) users      (100)     2393 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/management/commands/fine_permissions_load.py
-drwxr-xr-x   0 karma     (1000) users      (100)        0 2021-07-01 12:30:22.116971 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/migrations/
--rw-r--r--   0 karma     (1000) users      (100)     2502 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/migrations/0001_initial.py
--rw-r--r--   0 karma     (1000) users      (100)      778 2021-07-01 12:25:51.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/migrations/0002_swappable_user.py
--rw-r--r--   0 karma     (1000) users      (100)        0 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/migrations/__init__.py
--rw-r--r--   0 karma     (1000) users      (100)     1817 2021-07-01 12:25:51.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/models.py
--rw-r--r--   0 karma     (1000) users      (100)     2283 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/permissions.py
--rw-r--r--   0 karma     (1000) users      (100)     7231 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/serializers.py
-drwxr-xr-x   0 karma     (1000) users      (100)        0 2021-07-01 12:30:22.113971 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/templates/
-drwxr-xr-x   0 karma     (1000) users      (100)        0 2021-07-01 12:30:22.113971 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/templates/admin/
-drwxr-xr-x   0 karma     (1000) users      (100)        0 2021-07-01 12:30:22.113971 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/templates/admin/rest_framework_fine_permissions/
-drwxr-xr-x   0 karma     (1000) users      (100)        0 2021-07-01 12:30:22.116971 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/templates/admin/rest_framework_fine_permissions/userfieldpermissions/
--rw-r--r--   0 karma     (1000) users      (100)      781 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/templates/admin/rest_framework_fine_permissions/userfieldpermissions/change_form.html
--rw-r--r--   0 karma     (1000) users      (100)      403 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/urls.py
--rw-r--r--   0 karma     (1000) users      (100)     3123 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/utils.py
--rw-r--r--   0 karma     (1000) users      (100)     2802 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/views.py
--rw-r--r--   0 karma     (1000) users      (100)     2168 2021-07-01 12:21:50.000000 djangorestframework-fine-permissions-0.9.0/runtests.py
--rw-r--r--   0 karma     (1000) users      (100)       38 2021-07-01 12:30:22.117972 djangorestframework-fine-permissions-0.9.0/setup.cfg
--rw-r--r--   0 karma     (1000) users      (100)     1757 2021-07-01 12:25:51.000000 djangorestframework-fine-permissions-0.9.0/setup.py
-drwxr-xr-x   0 karma     (1000) users      (100)        0 2021-07-01 12:30:22.117972 djangorestframework-fine-permissions-0.9.0/tests/
--rw-r--r--   0 karma     (1000) users      (100)        0 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/tests/__init__.py
--rw-r--r--   0 karma     (1000) users      (100)      870 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/tests/models.py
--rw-r--r--   0 karma     (1000) users      (100)     1702 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/tests/serializers.py
--rw-r--r--   0 karma     (1000) users      (100)     1377 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/tests/test_admin.py
--rw-r--r--   0 karma     (1000) users      (100)     4608 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/tests/test_fields.py
--rw-r--r--   0 karma     (1000) users      (100)     6682 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/tests/test_qserializers.py
--rw-r--r--   0 karma     (1000) users      (100)     8200 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/tests/test_serializers.py
--rw-r--r--   0 karma     (1000) users      (100)     1925 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/tests/test_utils.py
--rw-r--r--   0 karma     (1000) users      (100)     7462 2021-07-01 12:21:50.000000 djangorestframework-fine-permissions-0.9.0/tests/test_views.py
--rw-r--r--   0 karma     (1000) users      (100)      235 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/tests/urls.py
--rw-r--r--   0 karma     (1000) users      (100)     1691 2021-05-12 14:01:54.000000 djangorestframework-fine-permissions-0.9.0/tests/utils.py
--rw-r--r--   0 karma     (1000) users      (100)      539 2021-07-01 12:21:50.000000 djangorestframework-fine-permissions-0.9.0/tox.ini
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-07-18 12:19:07.000000 djangorestframework-fine-permissions-0.9.2/
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-07-18 12:19:07.000000 djangorestframework-fine-permissions-0.9.2/tests/
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     6522 2022-07-20 19:49:49.000000 djangorestframework-fine-permissions-0.9.2/tests/test_qserializers.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     1692 2022-07-20 19:51:11.000000 djangorestframework-fine-permissions-0.9.2/tests/utils.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     1701 2022-07-20 19:48:31.000000 djangorestframework-fine-permissions-0.9.2/tests/serializers.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     4609 2022-07-20 19:58:56.000000 djangorestframework-fine-permissions-0.9.2/tests/test_fields.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     1927 2022-07-21 08:59:54.000000 djangorestframework-fine-permissions-0.9.2/tests/test_utils.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)      870 2019-11-15 15:53:05.000000 djangorestframework-fine-permissions-0.9.2/tests/models.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)      138 2022-07-20 21:37:24.000000 djangorestframework-fine-permissions-0.9.2/tests/apps.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     7520 2022-07-21 08:25:20.000000 djangorestframework-fine-permissions-0.9.2/tests/test_views.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     1352 2022-07-20 19:49:00.000000 djangorestframework-fine-permissions-0.9.2/tests/test_admin.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     8201 2022-07-20 19:50:13.000000 djangorestframework-fine-permissions-0.9.2/tests/test_serializers.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)      220 2022-07-20 19:52:52.000000 djangorestframework-fine-permissions-0.9.2/tests/urls.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)        0 2017-01-26 14:55:54.000000 djangorestframework-fine-permissions-0.9.2/tests/__init__.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)        0 2022-07-20 19:40:30.000000 djangorestframework-fine-permissions-0.9.2/requirements.txt
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     2614 2022-11-14 07:44:32.000000 djangorestframework-fine-permissions-0.9.2/runtests.py
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-07-18 12:19:07.000000 djangorestframework-fine-permissions-0.9.2/docs/
+-rw-r--r--   0 thierry   (1000) thierry   (1000)    34281 2017-01-26 14:56:16.000000 djangorestframework-fine-permissions-0.9.2/docs/admin1.png
+-rw-r--r--   0 thierry   (1000) thierry   (1000)    47625 2017-01-26 14:56:16.000000 djangorestframework-fine-permissions-0.9.2/docs/admin2.png
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-07-18 12:19:07.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     2259 2022-07-20 19:54:00.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/permissions.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     3035 2022-07-21 08:53:59.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/utils.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     2758 2022-07-20 20:44:28.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/views.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     2295 2022-07-21 09:01:00.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/fields.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     7207 2022-07-21 08:58:04.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/serializers.py
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-07-18 12:19:07.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/migrations/
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     2502 2020-11-06 14:51:34.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/migrations/0001_initial.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)        0 2017-01-26 14:55:54.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/migrations/__init__.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)      778 2022-07-21 08:13:54.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/migrations/0002_swappable_user.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     1791 2022-07-21 08:29:54.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/models.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)      228 2022-07-20 21:34:56.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/apps.py
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-07-18 12:19:07.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/management/
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-07-18 12:19:07.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/management/commands/
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     2366 2022-07-21 08:49:33.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/management/commands/fine_permissions_load.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     1693 2022-07-21 08:49:42.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/management/commands/fine_permissions_dump.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)        0 2017-01-26 14:55:54.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/management/commands/__init__.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)        0 2017-01-26 14:55:54.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/management/__init__.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)      388 2022-07-20 14:00:05.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/urls.py
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-07-18 12:19:07.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/templates/
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-07-18 12:19:07.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/templates/admin/
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-07-18 12:19:07.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/templates/admin/rest_framework_fine_permissions/
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-07-18 12:19:07.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/templates/admin/rest_framework_fine_permissions/userfieldpermissions/
+-rw-r--r--   0 thierry   (1000) thierry   (1000)      781 2017-01-26 14:55:54.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/templates/admin/rest_framework_fine_permissions/userfieldpermissions/change_form.html
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     1146 2022-07-20 19:41:54.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/filters.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     6231 2022-07-20 19:53:14.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/admin.py
+-rw-r--r--   0 thierry   (1000) thierry   (1000)        0 2017-01-26 14:55:54.000000 djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/__init__.py
+drwxrwxr-x   0 thierry   (1000) thierry   (1000)        0 2023-07-18 12:19:07.000000 djangorestframework-fine-permissions-0.9.2/djangorestframework_fine_permissions.egg-info/
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)       32 2023-07-18 12:19:06.000000 djangorestframework-fine-permissions-0.9.2/djangorestframework_fine_permissions.egg-info/top_level.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     1619 2023-07-18 12:19:07.000000 djangorestframework-fine-permissions-0.9.2/djangorestframework_fine_permissions.egg-info/SOURCES.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)        1 2023-07-18 12:19:06.000000 djangorestframework-fine-permissions-0.9.2/djangorestframework_fine_permissions.egg-info/dependency_links.txt
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     8827 2023-07-18 12:19:06.000000 djangorestframework-fine-permissions-0.9.2/djangorestframework_fine_permissions.egg-info/PKG-INFO
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)       38 2023-07-18 12:19:07.000000 djangorestframework-fine-permissions-0.9.2/setup.cfg
+-rw-r--r--   0 thierry   (1000) thierry   (1000)      217 2022-07-21 08:13:54.000000 djangorestframework-fine-permissions-0.9.2/MANIFEST.in
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     6142 2023-07-18 09:54:02.000000 djangorestframework-fine-permissions-0.9.2/README.rst
+-rw-r--r--   0 thierry   (1000) thierry   (1000)    18026 2017-01-26 14:55:54.000000 djangorestframework-fine-permissions-0.9.2/LICENSE
+-rw-r--r--   0 thierry   (1000) thierry   (1000)      352 2023-07-17 21:20:49.000000 djangorestframework-fine-permissions-0.9.2/tox.ini
+-rw-rw-r--   0 thierry   (1000) thierry   (1000)     8827 2023-07-18 12:19:07.000000 djangorestframework-fine-permissions-0.9.2/PKG-INFO
+-rw-r--r--   0 thierry   (1000) thierry   (1000)     1600 2023-07-18 12:15:47.000000 djangorestframework-fine-permissions-0.9.2/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `djangorestframework-fine-permissions-0.9.0/LICENSE` & `djangorestframework-fine-permissions-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `djangorestframework-fine-permissions-0.9.0/PKG-INFO` & `djangorestframework-fine-permissions-0.9.2/README.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,48 +1,20 @@
-Metadata-Version: 2.1
-Name: djangorestframework-fine-permissions
-Version: 0.9.0
-Summary: Field level permissions for Django REST Framework
-Home-page: https://github.com/unistra/django-rest-framework-fine-permissions
-Author: Arnaud Grausem
-Author-email: arnaud.grausem@unistra.fr
-Maintainer: Arnaud Grausem
-Maintainer-email: arnaud.grausem@unistra.fr
-License: UNKNOWN
-Download-URL: https://pypi.python.org/pypi/djangorestframework-fine-permissions
-Keywords: django,REST,rest_framework,permissions
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Web Environment
-Classifier: Framework :: Django
-Classifier: Intended Audience :: Developers
-Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.2
-Classifier: Framework :: Django :: 3.2
-License-File: LICENSE
-
 django-rest-framework-fine-permissions
 ======================================
 
 New permissions possibilities for rest-framework
 
 Compatibility
 -------------
 
 Works with :
 
-  * Python 3.5, 3.6, 3.7, 3.8
-  * Django 1.11, 2.2, 3.2
-  * Django Rest Framework >= 3.9
+  * Python 3.8, 3.9, 3.10
+  * Django 3.2
+  * Django Rest Framework >= 3.13
 
 .. image:: https://travis-ci.org/unistra/django-rest-framework-fine-permissions.svg?branch=master
     :target: https://travis-ci.org/unistra/django-rest-framework-fine-permissions
 
 .. image:: https://coveralls.io/repos/github/unistra/django-rest-framework-fine-permissions/badge.svg?branch=master
     :target: https://coveralls.io/github/unistra/django-rest-framework-fine-permissions?branch=master
 
@@ -235,9 +207,7 @@
 To export field's permissions, you can use the following command : ::
 
     python manage.py fine_permissions_dump myuser > /tmp/myuserfieldsperms.json
 
 To import field's permissions, you can use the following command : ::
 
     python manage.py fine_permissions_load -u anotheruser /tmp/myuserfieldsperms.json
-
-
```

### Comparing `djangorestframework-fine-permissions-0.9.0/README.rst` & `djangorestframework-fine-permissions-0.9.2/djangorestframework_fine_permissions.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,213 +1,237 @@
-django-rest-framework-fine-permissions
-======================================
-
-New permissions possibilities for rest-framework
-
-Compatibility
--------------
-
-Works with :
-
-  * Python 3.5, 3.6, 3.7, 3.8
-  * Django 1.11, 2.2, 3.2
-  * Django Rest Framework >= 3.9
-
-.. image:: https://travis-ci.org/unistra/django-rest-framework-fine-permissions.svg?branch=master
-    :target: https://travis-ci.org/unistra/django-rest-framework-fine-permissions
-
-.. image:: https://coveralls.io/repos/github/unistra/django-rest-framework-fine-permissions/badge.svg?branch=master
-    :target: https://coveralls.io/github/unistra/django-rest-framework-fine-permissions?branch=master
-
-.. image:: https://landscape.io/github/unistra/django-rest-framework-fine-permissions/master/landscape.svg?style=flat
-    :target: https://landscape.io/github/unistra/django-rest-framework-fine-permissions/master
-    :alt: Code Health
-
-
-Installation
-------------
-
-Install the package from pypi :
-
-.. code-block:: sh
-
-    pip install djangorestframework-fine-permissions
-
-Configure your `settings.py` module :
-
-.. code-block:: python
-
-    INSTALLED_APPS = (
-        ...
-        'rest_framework_fine_permissions',
-    )
-
-    REST_FRAMEWORK = {
-        'DEFAULT_FILTER_BACKENDS': (
-            # Enable the filter permission backend for all GenericAPIView
-            'rest_framework_fine_permissions.filters.FilterPermissionBackend',
-        ),
-
-        'DEFAULT_PERMISSION_CLASSES': (
-            # Enable the django model permissions (view,create,delete,modify)
-            'rest_framework_fine_permissions.permissions.FullDjangoModelPermissions',
-            # OPTIONAL if you use FilterPermissionBackend and GenericAPIView. Check filter permissions for objects.
-            'rest_framework_fine_permissions.permissions.FilterPermission',
-        )
-    }
-
-Sync the django's database :
-
-.. code-block:: sh
-
-    python manage.py syncdb
-
-Edit your `urls.py` module :
-
-.. code-block:: python
-
-    from django.conf.urls import url
-    from django.contrib import admin
-    from rest_framework_fine_permissions.urls import urlpatterns as drffp_urls
-
-    urlpatterns = [
-        url(r'^admin/', admin.site.urls),
-    ]
-    urlpatterns += drffp_urls
-
-Usage
------
-
- * Go to the django admin page
- * Add field's permissions to a user with the "User fields permissions" link
- * Add filter's permissions to a user with the "User filters permissions" link
-
-Example
--------
-
-``models.py`` :
-
-.. code-block:: python
-
-    from django.db import models
-    from django.db.models import Sum
-
-    class PollsChoice(models.Model):
-        id = models.IntegerField(primary_key=True)
-        choice_text = models.CharField(max_length=200)
-        votes = models.IntegerField()
-        question = models.ForeignKey('PollsQuestion')
-
-        class Meta:
-            permissions = (('view_pollschoice', 'Can view pollschoice'),)
-
-    class PollsQuestion(models.Model):
-        id = models.IntegerField(primary_key=True)
-        question_text = models.CharField(max_length=200)
-        pub_date = models.DateTimeField()
-
-        class Meta:
-            permissions = (('view_pollsquestion', 'Can view pollsquestion'),)
-
-        @property
-        def sum_votes(self):
-            return self.pollschoice_set.aggregate(total=Sum('votes'))['total']
-
-        @property
-        def choices(self):
-            return self.pollschoice_set.all()
-
-``serializers.py`` :
-
-.. code-block:: python
-
-    import datetime
-    from django.utils import timezone
-    from rest_framework import serializers
-    from rest_framework_fine_permissions.fields import ModelPermissionsField
-    from rest_framework_fine_permissions.serializers import ModelPermissionsSerializer
-
-    from . import models
-
-    class PollsChoiceSerializer(ModelPermissionsSerializer):
-        class Meta:
-            model = models.PollsChoice
-
-    class PollsQuestionSerializer(ModelPermissionsSerializer):
-        was_published_recently = serializers.SerializerMethodField()
-        votes = serializers.IntegerField(source='sum_votes')
-        choices = ModelPermissionsField(PollsChoiceSerializer)
-
-        class Meta:
-            model = models.PollsQuestion
-
-        def get_was_published_recently(self, obj):
-            return obj.pub_date >= timezone.now() - datetime.timedelta(days=1)
-
-``views.py`` :
-
-.. code-block:: python
-
-    from . import models
-    from . import serializers
-    from rest_framework import generics
-
-    class PollsChoiceDetail(generics.RetrieveUpdateDestroyAPIView):
-        queryset = models.PollsChoice.objects.all()
-        serializer_class = serializers.PollsChoiceSerializer
-
-``urls.py`` :
-
-.. code-block:: python
-
-    from django.conf.urls import patterns, url
-    from rest_framework.urlpatterns import format_suffix_patterns
-    from . import views
-
-    urlpatterns = [,
-        url(r'^pollsquestion/(?P<pk>\w+)$', views.PollsQuestionDetail.as_view(), name='pollsquestion-all-detail'),
-    ]
-    urlpatterns = format_suffix_patterns(urlpatterns, suffix_required=True)
-
-Create a user without the staff and superuser status, and add him permissions :
-
-.. image:: docs/admin1.png
-
-Then add user field permissions :
-
-.. image:: docs/admin2.png
-
-You can finally call your webservice :
-
-.. code-block:: sh
-
-    $ curl -X GET -H "Authorization: Token TOKEN" -H "Accept: application/json; indent=4" http://127.0.0.1/webservice/pollsquestion/1.json
-    {
-        "choices": [
+Metadata-Version: 1.2
+Name: djangorestframework-fine-permissions
+Version: 0.9.2
+Summary: Field level permissions for Django REST Framework
+Home-page: https://github.com/unistra/django-rest-framework-fine-permissions
+Author: dnum-dip-unistra
+Author-email: dnum-dip@unistra.fr
+Maintainer: dnum-dip-unistra
+Maintainer-email: dnum-dip@unistra.fr
+License: UNKNOWN
+Download-URL: https://pypi.python.org/pypi/djangorestframework-fine-permissions
+Description: django-rest-framework-fine-permissions
+        ======================================
+        
+        New permissions possibilities for rest-framework
+        
+        Compatibility
+        -------------
+        
+        Works with :
+        
+          * Python 3.8, 3.9, 3.10
+          * Django 3.2
+          * Django Rest Framework >= 3.13
+        
+        .. image:: https://travis-ci.org/unistra/django-rest-framework-fine-permissions.svg?branch=master
+            :target: https://travis-ci.org/unistra/django-rest-framework-fine-permissions
+        
+        .. image:: https://coveralls.io/repos/github/unistra/django-rest-framework-fine-permissions/badge.svg?branch=master
+            :target: https://coveralls.io/github/unistra/django-rest-framework-fine-permissions?branch=master
+        
+        .. image:: https://landscape.io/github/unistra/django-rest-framework-fine-permissions/master/landscape.svg?style=flat
+            :target: https://landscape.io/github/unistra/django-rest-framework-fine-permissions/master
+            :alt: Code Health
+        
+        
+        Installation
+        ------------
+        
+        Install the package from pypi :
+        
+        .. code-block:: sh
+        
+            pip install djangorestframework-fine-permissions
+        
+        Configure your `settings.py` module :
+        
+        .. code-block:: python
+        
+            INSTALLED_APPS = (
+                ...
+                'rest_framework_fine_permissions',
+            )
+        
+            REST_FRAMEWORK = {
+                'DEFAULT_FILTER_BACKENDS': (
+                    # Enable the filter permission backend for all GenericAPIView
+                    'rest_framework_fine_permissions.filters.FilterPermissionBackend',
+                ),
+        
+                'DEFAULT_PERMISSION_CLASSES': (
+                    # Enable the django model permissions (view,create,delete,modify)
+                    'rest_framework_fine_permissions.permissions.FullDjangoModelPermissions',
+                    # OPTIONAL if you use FilterPermissionBackend and GenericAPIView. Check filter permissions for objects.
+                    'rest_framework_fine_permissions.permissions.FilterPermission',
+                )
+            }
+        
+        Sync the django's database :
+        
+        .. code-block:: sh
+        
+            python manage.py syncdb
+        
+        Edit your `urls.py` module :
+        
+        .. code-block:: python
+        
+            from django.conf.urls import url
+            from django.contrib import admin
+            from rest_framework_fine_permissions.urls import urlpatterns as drffp_urls
+        
+            urlpatterns = [
+                url(r'^admin/', admin.site.urls),
+            ]
+            urlpatterns += drffp_urls
+        
+        Usage
+        -----
+        
+         * Go to the django admin page
+         * Add field's permissions to a user with the "User fields permissions" link
+         * Add filter's permissions to a user with the "User filters permissions" link
+        
+        Example
+        -------
+        
+        ``models.py`` :
+        
+        .. code-block:: python
+        
+            from django.db import models
+            from django.db.models import Sum
+        
+            class PollsChoice(models.Model):
+                id = models.IntegerField(primary_key=True)
+                choice_text = models.CharField(max_length=200)
+                votes = models.IntegerField()
+                question = models.ForeignKey('PollsQuestion')
+        
+                class Meta:
+                    permissions = (('view_pollschoice', 'Can view pollschoice'),)
+        
+            class PollsQuestion(models.Model):
+                id = models.IntegerField(primary_key=True)
+                question_text = models.CharField(max_length=200)
+                pub_date = models.DateTimeField()
+        
+                class Meta:
+                    permissions = (('view_pollsquestion', 'Can view pollsquestion'),)
+        
+                @property
+                def sum_votes(self):
+                    return self.pollschoice_set.aggregate(total=Sum('votes'))['total']
+        
+                @property
+                def choices(self):
+                    return self.pollschoice_set.all()
+        
+        ``serializers.py`` :
+        
+        .. code-block:: python
+        
+            import datetime
+            from django.utils import timezone
+            from rest_framework import serializers
+            from rest_framework_fine_permissions.fields import ModelPermissionsField
+            from rest_framework_fine_permissions.serializers import ModelPermissionsSerializer
+        
+            from . import models
+        
+            class PollsChoiceSerializer(ModelPermissionsSerializer):
+                class Meta:
+                    model = models.PollsChoice
+        
+            class PollsQuestionSerializer(ModelPermissionsSerializer):
+                was_published_recently = serializers.SerializerMethodField()
+                votes = serializers.IntegerField(source='sum_votes')
+                choices = ModelPermissionsField(PollsChoiceSerializer)
+        
+                class Meta:
+                    model = models.PollsQuestion
+        
+                def get_was_published_recently(self, obj):
+                    return obj.pub_date >= timezone.now() - datetime.timedelta(days=1)
+        
+        ``views.py`` :
+        
+        .. code-block:: python
+        
+            from . import models
+            from . import serializers
+            from rest_framework import generics
+        
+            class PollsChoiceDetail(generics.RetrieveUpdateDestroyAPIView):
+                queryset = models.PollsChoice.objects.all()
+                serializer_class = serializers.PollsChoiceSerializer
+        
+        ``urls.py`` :
+        
+        .. code-block:: python
+        
+            from django.conf.urls import patterns, url
+            from rest_framework.urlpatterns import format_suffix_patterns
+            from . import views
+        
+            urlpatterns = [,
+                url(r'^pollsquestion/(?P<pk>\w+)$', views.PollsQuestionDetail.as_view(), name='pollsquestion-all-detail'),
+            ]
+            urlpatterns = format_suffix_patterns(urlpatterns, suffix_required=True)
+        
+        Create a user without the staff and superuser status, and add him permissions :
+        
+        .. image:: docs/admin1.png
+        
+        Then add user field permissions :
+        
+        .. image:: docs/admin2.png
+        
+        You can finally call your webservice :
+        
+        .. code-block:: sh
+        
+            $ curl -X GET -H "Authorization: Token TOKEN" -H "Accept: application/json; indent=4" http://127.0.0.1/webservice/pollsquestion/1.json
             {
-                "choice_text": "Yes",
+                "choices": [
+                    {
+                        "choice_text": "Yes",
+                        "id": 1,
+                        "votes": 5
+                    },
+                    {
+                        "choice_text": "No",
+                        "id": 2,
+                        "votes": 2
+                    }
+                ],
                 "id": 1,
-                "votes": 5
-            },
-            {
-                "choice_text": "No",
-                "id": 2,
-                "votes": 2
+                "pub_date": "2017-01-08T09:00:00",
+                "question_text": "Is this a question ?",
+                "votes": 7,
+                "was_published_recently": false
             }
-        ],
-        "id": 1,
-        "pub_date": "2017-01-08T09:00:00",
-        "question_text": "Is this a question ?",
-        "votes": 7,
-        "was_published_recently": false
-    }
-
-Import/Export
--------------
-
-To export field's permissions, you can use the following command : ::
-
-    python manage.py fine_permissions_dump myuser > /tmp/myuserfieldsperms.json
-
-To import field's permissions, you can use the following command : ::
-
-    python manage.py fine_permissions_load -u anotheruser /tmp/myuserfieldsperms.json
+        
+        Import/Export
+        -------------
+        
+        To export field's permissions, you can use the following command : ::
+        
+            python manage.py fine_permissions_dump myuser > /tmp/myuserfieldsperms.json
+        
+        To import field's permissions, you can use the following command : ::
+        
+            python manage.py fine_permissions_load -u anotheruser /tmp/myuserfieldsperms.json
+        
+Keywords: django,REST,rest_framework,permissions
+Platform: UNKNOWN
+Classifier: Development Status :: 4 - Beta
+Classifier: Environment :: Web Environment
+Classifier: Framework :: Django
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Framework :: Django
+Classifier: Framework :: Django :: 3.2
```

### Comparing `djangorestframework-fine-permissions-0.9.0/djangorestframework_fine_permissions.egg-info/PKG-INFO` & `djangorestframework-fine-permissions-0.9.2/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,243 +1,237 @@
-Metadata-Version: 2.1
+Metadata-Version: 1.2
 Name: djangorestframework-fine-permissions
-Version: 0.9.0
+Version: 0.9.2
 Summary: Field level permissions for Django REST Framework
 Home-page: https://github.com/unistra/django-rest-framework-fine-permissions
-Author: Arnaud Grausem
-Author-email: arnaud.grausem@unistra.fr
-Maintainer: Arnaud Grausem
-Maintainer-email: arnaud.grausem@unistra.fr
+Author: dnum-dip-unistra
+Author-email: dnum-dip@unistra.fr
+Maintainer: dnum-dip-unistra
+Maintainer-email: dnum-dip@unistra.fr
 License: UNKNOWN
 Download-URL: https://pypi.python.org/pypi/djangorestframework-fine-permissions
+Description: django-rest-framework-fine-permissions
+        ======================================
+        
+        New permissions possibilities for rest-framework
+        
+        Compatibility
+        -------------
+        
+        Works with :
+        
+          * Python 3.8, 3.9, 3.10
+          * Django 3.2
+          * Django Rest Framework >= 3.13
+        
+        .. image:: https://travis-ci.org/unistra/django-rest-framework-fine-permissions.svg?branch=master
+            :target: https://travis-ci.org/unistra/django-rest-framework-fine-permissions
+        
+        .. image:: https://coveralls.io/repos/github/unistra/django-rest-framework-fine-permissions/badge.svg?branch=master
+            :target: https://coveralls.io/github/unistra/django-rest-framework-fine-permissions?branch=master
+        
+        .. image:: https://landscape.io/github/unistra/django-rest-framework-fine-permissions/master/landscape.svg?style=flat
+            :target: https://landscape.io/github/unistra/django-rest-framework-fine-permissions/master
+            :alt: Code Health
+        
+        
+        Installation
+        ------------
+        
+        Install the package from pypi :
+        
+        .. code-block:: sh
+        
+            pip install djangorestframework-fine-permissions
+        
+        Configure your `settings.py` module :
+        
+        .. code-block:: python
+        
+            INSTALLED_APPS = (
+                ...
+                'rest_framework_fine_permissions',
+            )
+        
+            REST_FRAMEWORK = {
+                'DEFAULT_FILTER_BACKENDS': (
+                    # Enable the filter permission backend for all GenericAPIView
+                    'rest_framework_fine_permissions.filters.FilterPermissionBackend',
+                ),
+        
+                'DEFAULT_PERMISSION_CLASSES': (
+                    # Enable the django model permissions (view,create,delete,modify)
+                    'rest_framework_fine_permissions.permissions.FullDjangoModelPermissions',
+                    # OPTIONAL if you use FilterPermissionBackend and GenericAPIView. Check filter permissions for objects.
+                    'rest_framework_fine_permissions.permissions.FilterPermission',
+                )
+            }
+        
+        Sync the django's database :
+        
+        .. code-block:: sh
+        
+            python manage.py syncdb
+        
+        Edit your `urls.py` module :
+        
+        .. code-block:: python
+        
+            from django.conf.urls import url
+            from django.contrib import admin
+            from rest_framework_fine_permissions.urls import urlpatterns as drffp_urls
+        
+            urlpatterns = [
+                url(r'^admin/', admin.site.urls),
+            ]
+            urlpatterns += drffp_urls
+        
+        Usage
+        -----
+        
+         * Go to the django admin page
+         * Add field's permissions to a user with the "User fields permissions" link
+         * Add filter's permissions to a user with the "User filters permissions" link
+        
+        Example
+        -------
+        
+        ``models.py`` :
+        
+        .. code-block:: python
+        
+            from django.db import models
+            from django.db.models import Sum
+        
+            class PollsChoice(models.Model):
+                id = models.IntegerField(primary_key=True)
+                choice_text = models.CharField(max_length=200)
+                votes = models.IntegerField()
+                question = models.ForeignKey('PollsQuestion')
+        
+                class Meta:
+                    permissions = (('view_pollschoice', 'Can view pollschoice'),)
+        
+            class PollsQuestion(models.Model):
+                id = models.IntegerField(primary_key=True)
+                question_text = models.CharField(max_length=200)
+                pub_date = models.DateTimeField()
+        
+                class Meta:
+                    permissions = (('view_pollsquestion', 'Can view pollsquestion'),)
+        
+                @property
+                def sum_votes(self):
+                    return self.pollschoice_set.aggregate(total=Sum('votes'))['total']
+        
+                @property
+                def choices(self):
+                    return self.pollschoice_set.all()
+        
+        ``serializers.py`` :
+        
+        .. code-block:: python
+        
+            import datetime
+            from django.utils import timezone
+            from rest_framework import serializers
+            from rest_framework_fine_permissions.fields import ModelPermissionsField
+            from rest_framework_fine_permissions.serializers import ModelPermissionsSerializer
+        
+            from . import models
+        
+            class PollsChoiceSerializer(ModelPermissionsSerializer):
+                class Meta:
+                    model = models.PollsChoice
+        
+            class PollsQuestionSerializer(ModelPermissionsSerializer):
+                was_published_recently = serializers.SerializerMethodField()
+                votes = serializers.IntegerField(source='sum_votes')
+                choices = ModelPermissionsField(PollsChoiceSerializer)
+        
+                class Meta:
+                    model = models.PollsQuestion
+        
+                def get_was_published_recently(self, obj):
+                    return obj.pub_date >= timezone.now() - datetime.timedelta(days=1)
+        
+        ``views.py`` :
+        
+        .. code-block:: python
+        
+            from . import models
+            from . import serializers
+            from rest_framework import generics
+        
+            class PollsChoiceDetail(generics.RetrieveUpdateDestroyAPIView):
+                queryset = models.PollsChoice.objects.all()
+                serializer_class = serializers.PollsChoiceSerializer
+        
+        ``urls.py`` :
+        
+        .. code-block:: python
+        
+            from django.conf.urls import patterns, url
+            from rest_framework.urlpatterns import format_suffix_patterns
+            from . import views
+        
+            urlpatterns = [,
+                url(r'^pollsquestion/(?P<pk>\w+)$', views.PollsQuestionDetail.as_view(), name='pollsquestion-all-detail'),
+            ]
+            urlpatterns = format_suffix_patterns(urlpatterns, suffix_required=True)
+        
+        Create a user without the staff and superuser status, and add him permissions :
+        
+        .. image:: docs/admin1.png
+        
+        Then add user field permissions :
+        
+        .. image:: docs/admin2.png
+        
+        You can finally call your webservice :
+        
+        .. code-block:: sh
+        
+            $ curl -X GET -H "Authorization: Token TOKEN" -H "Accept: application/json; indent=4" http://127.0.0.1/webservice/pollsquestion/1.json
+            {
+                "choices": [
+                    {
+                        "choice_text": "Yes",
+                        "id": 1,
+                        "votes": 5
+                    },
+                    {
+                        "choice_text": "No",
+                        "id": 2,
+                        "votes": 2
+                    }
+                ],
+                "id": 1,
+                "pub_date": "2017-01-08T09:00:00",
+                "question_text": "Is this a question ?",
+                "votes": 7,
+                "was_published_recently": false
+            }
+        
+        Import/Export
+        -------------
+        
+        To export field's permissions, you can use the following command : ::
+        
+            python manage.py fine_permissions_dump myuser > /tmp/myuserfieldsperms.json
+        
+        To import field's permissions, you can use the following command : ::
+        
+            python manage.py fine_permissions_load -u anotheruser /tmp/myuserfieldsperms.json
+        
 Keywords: django,REST,rest_framework,permissions
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 1.11
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.2
-License-File: LICENSE
-
-django-rest-framework-fine-permissions
-======================================
-
-New permissions possibilities for rest-framework
-
-Compatibility
--------------
-
-Works with :
-
-  * Python 3.5, 3.6, 3.7, 3.8
-  * Django 1.11, 2.2, 3.2
-  * Django Rest Framework >= 3.9
-
-.. image:: https://travis-ci.org/unistra/django-rest-framework-fine-permissions.svg?branch=master
-    :target: https://travis-ci.org/unistra/django-rest-framework-fine-permissions
-
-.. image:: https://coveralls.io/repos/github/unistra/django-rest-framework-fine-permissions/badge.svg?branch=master
-    :target: https://coveralls.io/github/unistra/django-rest-framework-fine-permissions?branch=master
-
-.. image:: https://landscape.io/github/unistra/django-rest-framework-fine-permissions/master/landscape.svg?style=flat
-    :target: https://landscape.io/github/unistra/django-rest-framework-fine-permissions/master
-    :alt: Code Health
-
-
-Installation
-------------
-
-Install the package from pypi :
-
-.. code-block:: sh
-
-    pip install djangorestframework-fine-permissions
-
-Configure your `settings.py` module :
-
-.. code-block:: python
-
-    INSTALLED_APPS = (
-        ...
-        'rest_framework_fine_permissions',
-    )
-
-    REST_FRAMEWORK = {
-        'DEFAULT_FILTER_BACKENDS': (
-            # Enable the filter permission backend for all GenericAPIView
-            'rest_framework_fine_permissions.filters.FilterPermissionBackend',
-        ),
-
-        'DEFAULT_PERMISSION_CLASSES': (
-            # Enable the django model permissions (view,create,delete,modify)
-            'rest_framework_fine_permissions.permissions.FullDjangoModelPermissions',
-            # OPTIONAL if you use FilterPermissionBackend and GenericAPIView. Check filter permissions for objects.
-            'rest_framework_fine_permissions.permissions.FilterPermission',
-        )
-    }
-
-Sync the django's database :
-
-.. code-block:: sh
-
-    python manage.py syncdb
-
-Edit your `urls.py` module :
-
-.. code-block:: python
-
-    from django.conf.urls import url
-    from django.contrib import admin
-    from rest_framework_fine_permissions.urls import urlpatterns as drffp_urls
-
-    urlpatterns = [
-        url(r'^admin/', admin.site.urls),
-    ]
-    urlpatterns += drffp_urls
-
-Usage
------
-
- * Go to the django admin page
- * Add field's permissions to a user with the "User fields permissions" link
- * Add filter's permissions to a user with the "User filters permissions" link
-
-Example
--------
-
-``models.py`` :
-
-.. code-block:: python
-
-    from django.db import models
-    from django.db.models import Sum
-
-    class PollsChoice(models.Model):
-        id = models.IntegerField(primary_key=True)
-        choice_text = models.CharField(max_length=200)
-        votes = models.IntegerField()
-        question = models.ForeignKey('PollsQuestion')
-
-        class Meta:
-            permissions = (('view_pollschoice', 'Can view pollschoice'),)
-
-    class PollsQuestion(models.Model):
-        id = models.IntegerField(primary_key=True)
-        question_text = models.CharField(max_length=200)
-        pub_date = models.DateTimeField()
-
-        class Meta:
-            permissions = (('view_pollsquestion', 'Can view pollsquestion'),)
-
-        @property
-        def sum_votes(self):
-            return self.pollschoice_set.aggregate(total=Sum('votes'))['total']
-
-        @property
-        def choices(self):
-            return self.pollschoice_set.all()
-
-``serializers.py`` :
-
-.. code-block:: python
-
-    import datetime
-    from django.utils import timezone
-    from rest_framework import serializers
-    from rest_framework_fine_permissions.fields import ModelPermissionsField
-    from rest_framework_fine_permissions.serializers import ModelPermissionsSerializer
-
-    from . import models
-
-    class PollsChoiceSerializer(ModelPermissionsSerializer):
-        class Meta:
-            model = models.PollsChoice
-
-    class PollsQuestionSerializer(ModelPermissionsSerializer):
-        was_published_recently = serializers.SerializerMethodField()
-        votes = serializers.IntegerField(source='sum_votes')
-        choices = ModelPermissionsField(PollsChoiceSerializer)
-
-        class Meta:
-            model = models.PollsQuestion
-
-        def get_was_published_recently(self, obj):
-            return obj.pub_date >= timezone.now() - datetime.timedelta(days=1)
-
-``views.py`` :
-
-.. code-block:: python
-
-    from . import models
-    from . import serializers
-    from rest_framework import generics
-
-    class PollsChoiceDetail(generics.RetrieveUpdateDestroyAPIView):
-        queryset = models.PollsChoice.objects.all()
-        serializer_class = serializers.PollsChoiceSerializer
-
-``urls.py`` :
-
-.. code-block:: python
-
-    from django.conf.urls import patterns, url
-    from rest_framework.urlpatterns import format_suffix_patterns
-    from . import views
-
-    urlpatterns = [,
-        url(r'^pollsquestion/(?P<pk>\w+)$', views.PollsQuestionDetail.as_view(), name='pollsquestion-all-detail'),
-    ]
-    urlpatterns = format_suffix_patterns(urlpatterns, suffix_required=True)
-
-Create a user without the staff and superuser status, and add him permissions :
-
-.. image:: docs/admin1.png
-
-Then add user field permissions :
-
-.. image:: docs/admin2.png
-
-You can finally call your webservice :
-
-.. code-block:: sh
-
-    $ curl -X GET -H "Authorization: Token TOKEN" -H "Accept: application/json; indent=4" http://127.0.0.1/webservice/pollsquestion/1.json
-    {
-        "choices": [
-            {
-                "choice_text": "Yes",
-                "id": 1,
-                "votes": 5
-            },
-            {
-                "choice_text": "No",
-                "id": 2,
-                "votes": 2
-            }
-        ],
-        "id": 1,
-        "pub_date": "2017-01-08T09:00:00",
-        "question_text": "Is this a question ?",
-        "votes": 7,
-        "was_published_recently": false
-    }
-
-Import/Export
--------------
-
-To export field's permissions, you can use the following command : ::
-
-    python manage.py fine_permissions_dump myuser > /tmp/myuserfieldsperms.json
-
-To import field's permissions, you can use the following command : ::
-
-    python manage.py fine_permissions_load -u anotheruser /tmp/myuserfieldsperms.json
-
-
```

### Comparing `djangorestframework-fine-permissions-0.9.0/djangorestframework_fine_permissions.egg-info/SOURCES.txt` & `djangorestframework-fine-permissions-0.9.2/djangorestframework_fine_permissions.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 requirements.txt
 runtests.py
 setup.py
 tox.ini
 djangorestframework_fine_permissions.egg-info/PKG-INFO
 djangorestframework_fine_permissions.egg-info/SOURCES.txt
 djangorestframework_fine_permissions.egg-info/dependency_links.txt
-djangorestframework_fine_permissions.egg-info/requires.txt
 djangorestframework_fine_permissions.egg-info/top_level.txt
 docs/admin1.png
 docs/admin2.png
 rest_framework_fine_permissions/__init__.py
 rest_framework_fine_permissions/admin.py
+rest_framework_fine_permissions/apps.py
 rest_framework_fine_permissions/fields.py
 rest_framework_fine_permissions/filters.py
 rest_framework_fine_permissions/models.py
 rest_framework_fine_permissions/permissions.py
 rest_framework_fine_permissions/serializers.py
 rest_framework_fine_permissions/urls.py
 rest_framework_fine_permissions/utils.py
@@ -27,14 +27,15 @@
 rest_framework_fine_permissions/management/commands/fine_permissions_dump.py
 rest_framework_fine_permissions/management/commands/fine_permissions_load.py
 rest_framework_fine_permissions/migrations/0001_initial.py
 rest_framework_fine_permissions/migrations/0002_swappable_user.py
 rest_framework_fine_permissions/migrations/__init__.py
 rest_framework_fine_permissions/templates/admin/rest_framework_fine_permissions/userfieldpermissions/change_form.html
 tests/__init__.py
+tests/apps.py
 tests/models.py
 tests/serializers.py
 tests/test_admin.py
 tests/test_fields.py
 tests/test_qserializers.py
 tests/test_serializers.py
 tests/test_utils.py
```

### Comparing `djangorestframework-fine-permissions-0.9.0/docs/admin1.png` & `djangorestframework-fine-permissions-0.9.2/docs/admin1.png`

 * *Files identical despite different names*

### Comparing `djangorestframework-fine-permissions-0.9.0/docs/admin2.png` & `djangorestframework-fine-permissions-0.9.2/docs/admin2.png`

 * *Files identical despite different names*

### Comparing `djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/admin.py` & `djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,20 @@
-# -*- coding: utf-8 -*-
-
 """
 """
 
 from django import forms
 from django.contrib import admin
 from django.contrib.admin.widgets import FilteredSelectMultiple
 from django.contrib.contenttypes.models import ContentType
 from django.db.models import Q
 from django.utils.html import format_html
 
 from .fields import ModelPermissionsField
 from .models import (
-    FieldPermission, UserFieldPermissions, FilterPermissionModel)
+    FieldPermission, FilterPermissionModel, UserFieldPermissions)
 from .utils import get_field_permissions
 from .serializers import QSerializer
 
 
 class UserFieldPermissionsForm(forms.ModelForm):
 
     """
```

### Comparing `djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/fields.py` & `djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/fields.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,20 @@
-# -*- coding: utf-8 -*-
-
 """
 """
 
-import logging
 import collections
+import logging
 
-from django.core.exceptions import ObjectDoesNotExist
-from django.db import models
-from django.utils.encoding import smart_text
 from rest_framework import serializers
 from rest_framework.fields import Field
 
+from django.core.exceptions import ObjectDoesNotExist
+from django.db import models
+from django.utils.encoding import smart_str
+
 from .serializers import ModelPermissionsSerializer
 from .utils import get_serializer
 
 logger = logging.getLogger(__name__)
 
 
 class ModelPermissionsField(Field):
@@ -44,19 +43,19 @@
             'override `get_queryset`, or set read_only=`True`.'
         )
 
         if data is not None:
             try:
                 return self.queryset.get(pk=data)
             except ObjectDoesNotExist:
-                self.fail('does_not_exist', value=smart_text(data))
+                self.fail('does_not_exist', value=smart_str(data))
 
     def to_representation(self, obj):
         """ Represent data for the field. """
-        many = isinstance(obj, collections.Iterable) \
+        many = isinstance(obj, collections.abc.Iterable) \
             or isinstance(obj, models.Manager) \
             and not isinstance(obj, dict)
 
         assert self.serializer is not None \
             and issubclass(self.serializer, serializers.ModelSerializer), (
                 "Bad serializer defined %s" % self.serializer
             )
```

### Comparing `djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/filters.py` & `djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/filters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,14 @@
-# -*- coding: utf-8 -*-
-
-from django.db.models import Q
-from django.core.exceptions import ObjectDoesNotExist
-from django.contrib.contenttypes.models import ContentType
+from rest_framework.filters import BaseFilterBackend
 from rest_framework_fine_permissions.serializers import QSerializer
 from rest_framework_fine_permissions.models import FilterPermissionModel
-from rest_framework.filters import BaseFilterBackend
+
+from django.contrib.contenttypes.models import ContentType
+from django.core.exceptions import ObjectDoesNotExist
+from django.db.models import Q
 from django.db.models.query import QuerySet
 
 
 class FilterPermissionBackend(BaseFilterBackend):
     """
     Filter permission backend
     """
```

### Comparing `djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/management/commands/fine_permissions_dump.py` & `djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/management/commands/fine_permissions_dump.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python
 
-from django.core.management.base import BaseCommand, CommandError
+import json
+
 from rest_framework_fine_permissions.models import UserFieldPermissions
+
 from django.contrib.auth.models import User
 from django.core.exceptions import ObjectDoesNotExist
-import json
+from django.core.management.base import BaseCommand, CommandError
 
 
 class Command(BaseCommand):
 
     help = ("Output the user's fieds permissions of the database as a fixture of the given user ")
     args = 'user'
 
@@ -25,16 +27,14 @@
 
         def get_fields_permissions(user):
             try:
                 return UserFieldPermissions.objects.get(user=user)
             except ObjectDoesNotExist as e:
                 raise CommandError("This user doesn't have fields permissions")
 
-
-
         if len(args) !=1:
             raise CommandError("Specifies a user")
         else:
             try:
                 self.stdout.ending = None
                 user = get_user(args[0])
                 fields_permissions  = get_fields_permissions(user)
@@ -43,8 +43,7 @@
                 jsoneatthat = {'username': user.username, 
                     'fields_permissions' : [ {'app_label': permission.content_type.app_label, 'model' : permission.content_type.model, 'name': permission.name } for permission in permissions]}
 
                 self.stdout.write(json.dumps(jsoneatthat))
 
             except:
                 raise
-
```

### Comparing `djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/management/commands/fine_permissions_load.py` & `djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/management/commands/fine_permissions_load.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 #!/usr/bin/env python
 
-from django.core import management
-from django.core.management.base import BaseCommand, CommandError
-from django.core import serializers
-from rest_framework_fine_permissions.models import UserFieldPermissions, FieldPermission
-from django.contrib.auth.models import User
-from django.core.exceptions import ObjectDoesNotExist
 import json
-from optparse import make_option
 import sys
+from optparse import make_option
+
+from rest_framework_fine_permissions.models import UserFieldPermissions, FieldPermission
+
+from django.contrib.auth.models import User
 from django.contrib.contenttypes.models import ContentType
+from django.core import management, serializers
+from django.core.exceptions import ObjectDoesNotExist
+from django.core.management.base import BaseCommand, CommandError
 
 
 
 class Command(BaseCommand):
 
     help = ("Loads the user's fieds permissions into the database from a fixture of the given user ")
     args = 'json file'
@@ -41,32 +42,26 @@
                 p = FieldPermission.objects.get(content_type=content_type, name=name)
             except ObjectDoesNotExist:
                 p = FieldPermission(content_type=content_type, name=name)
                 p.save()
             finally:
                 user_field_permissions.permissions.add(p)
 
-
-
         if len(args) !=1:
              raise CommandError("Specifies a json file created by the fine_permissions_dump command")
         else:
             try:
-
-
                 with open(args[0], 'r') as json_file:
                     myjson = json.load(json_file)
 
                     user = get_user(options.get('user')) if options['user'] else get_user(myjson['username'])
                     fields_permissions = myjson['fields_permissions']
 
                     user_field_permissions = UserFieldPermissions(user=user)
                     user_field_permissions.save()
 
                     for f in fields_permissions:
                         content_type = ContentType.objects.get(app_label=f["app_label"], model=f["model"])
                         add_permissions(user_field_permissions, content_type, f['name'])
 
-
             except Exception as e:
                 raise CommandError(e)
-
```

### Comparing `djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/migrations/0001_initial.py` & `djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/migrations/0002_swappable_user.py` & `djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/migrations/0002_swappable_user.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/models.py` & `djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/models.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# -*- coding: utf-8 -*-
-
 """
 """
 from django.conf import settings
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
-from django.utils.translation import ugettext_lazy as _
+from django.utils.translation import gettext_lazy as _
 
 
 class FieldPermission(models.Model):
     name = models.CharField(_('name'), max_length=255)
     content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
 
     class Meta:
```

### Comparing `djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/permissions.py` & `djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/permissions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-# -*- coding: utf-8 -*-
-
 """ Provides new permission policies for django-rest-framework
 """
 
-from rest_framework.permissions import DjangoModelPermissions, BasePermission
-from django.contrib.contenttypes.models import ContentType
+from rest_framework.permissions import BasePermission, DjangoModelPermissions
 from rest_framework_fine_permissions.models import FilterPermissionModel
-from django.core.exceptions import ObjectDoesNotExist
 from rest_framework_fine_permissions.serializers import QSerializer
 
+from django.contrib.contenttypes.models import ContentType
+from django.core.exceptions import ObjectDoesNotExist
+
 
 class FullDjangoModelPermissions(DjangoModelPermissions):
     """
     The request is authenticated using `django.contrib.auth` permissions.
     See: https://docs.djangoproject.com/en/dev/topics/auth/#permissions
 
     It ensures that the user is authenticated, and has the appropriate
```

### Comparing `djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/serializers.py` & `djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,22 @@
-# -*- coding: utf-8 -*-
-
 """
 """
 
 import base64
-from collections import OrderedDict
-from datetime import datetime, date
 import json
 import time
+from collections import OrderedDict
+from datetime import datetime, date
 
-from django.core.serializers.base import SerializationError
-from django.db.models import Q
 from rest_framework import serializers
 from rest_framework.utils.field_mapping import get_relation_kwargs
 
+from django.core.serializers.base import SerializationError
+from django.db.models import Q
+
 from .models import FieldPermission
 
 
 class ModelPermissionsSerializer(serializers.ModelSerializer):
 
     """ Permission on serializer's fields for an authenticated user. """
```

### Comparing `djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/templates/admin/rest_framework_fine_permissions/userfieldpermissions/change_form.html` & `djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/templates/admin/rest_framework_fine_permissions/userfieldpermissions/change_form.html`

 * *Files identical despite different names*

### Comparing `djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/utils.py` & `djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,37 +1,36 @@
-# -*- coding: utf-8 -*-
-
 """
 """
 
-from importlib import import_module
 import inspect
-from collections import OrderedDict
 import logging
+import string
+from collections import OrderedDict
+from importlib import import_module
+from itertools import chain
+
+from rest_framework.utils.model_meta import get_field_info
 
 from django.apps import apps
 from django.conf import settings
-from rest_framework.utils.model_meta import get_field_info
-from six import iterkeys, string_types
-from itertools import chain
 
 
 logger = logging.getLogger(__name__)
 APP_NAMES = None
 
 
 def get_application(app_label):
     """ Get an application. """
     app_config = apps.get_app_config(app_label)
     return app_config.module.__name__
 
 
 def get_serializer(serializer):
     """ Load a serializer. """
-    if isinstance(serializer, string_types):
+    if isinstance(serializer, str):
         try:
             app_label, serializer_name = serializer.split('.')
             app_package = get_application(app_label)
             serializer_module = import_module('%s.serializers' % app_package)
             serializer = getattr(serializer_module, serializer_name)
         except Exception as e:
             logger.error('Serializer %s not found: %s' % (serializer, e))
@@ -55,17 +54,17 @@
     fields_and_pk[pk.name] = pk
     fields_and_pk.update(fields)
     return fields_and_pk
 
 
 def get_model_fields(model):
     fields_info = get_field_info(model)
-    return chain(iterkeys(merge_fields_and_pk(fields_info.pk,
-                                              fields_info.fields)),
-                 iterkeys(fields_info.relations))
+    return chain((merge_fields_and_pk(
+                    fields_info.pk,fields_info.fields).keys()),
+                 fields_info.relations.keys())
 
 
 def get_permitted_fields(model, serializer):
     fields = get_model_fields(model)
     result = dict.fromkeys(fields, None)
     result.update(serializer._declared_fields)
     exclude = getattr(serializer.Meta, 'exclude', ())
```

### Comparing `djangorestframework-fine-permissions-0.9.0/rest_framework_fine_permissions/views.py` & `djangorestframework-fine-permissions-0.9.2/rest_framework_fine_permissions/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import json
 
+from rest_framework_fine_permissions.models import (
+    FieldPermission, UserFieldPermissions)
+
 from django.contrib import messages
 from django.contrib.admin.views.decorators import staff_member_required
-from django.contrib.contenttypes.models import ContentType
 from django.contrib.auth.models import User
+from django.contrib.contenttypes.models import ContentType
 from django.http import HttpResponse
 from django.shortcuts import get_object_or_404, redirect
-from rest_framework_fine_permissions.models import FieldPermission,\
-                                                   UserFieldPermissions
 
 
 @staff_member_required
 def permissions_export_json(request, ufp_id):
     ufp = get_object_or_404(UserFieldPermissions, pk=ufp_id)
     permissions = {
         'username': ufp.user.username,
```

### Comparing `djangorestframework-fine-permissions-0.9.0/runtests.py` & `djangorestframework-fine-permissions-0.9.2/runtests.py`

 * *Files 10% similar despite different names*

```diff
@@ -44,15 +44,31 @@
                     ],
                 },
             },
         ],
         ROOT_URLCONF='tests.urls',
         USE_TZ=False,
         SECRET_KEY='foobar',
-        DEFAULT_AUTO_FIELD = 'django.db.models.BigAutoField'
+        LOGGING = {
+            'version': 1,
+            'disable_existing_loggers': False,
+            'handlers': {
+                'null': {
+                    'level': 'DEBUG',
+                    'class': 'logging.NullHandler'
+                },
+            },
+            'loggers': {
+                'rest_framework_fine_permissions': {
+                    'handlers': ['null'],
+                    'level': 'DEBUG',
+                    'propagate': True
+                }
+            },
+        }
         # SILENCED_SYSTEM_CHECKS=['1_7.W001'],
     )
 
 
 def runtests():
     argv = sys.argv[:1] + ['test'] + sys.argv[1:]
     execute_from_command_line(argv)
```

### Comparing `djangorestframework-fine-permissions-0.9.0/setup.py` & `djangorestframework-fine-permissions-0.9.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 #!/usr/bin/env python
-# -*- coding: utf-8 -*-
 
 from setuptools import setup
 from setuptools import find_packages
 
 
 with open('README.rst') as readme:
     long_description = readme.read()
@@ -14,37 +13,34 @@
     libraries = [lib for lib in lines if not lib.startswith('-')]
     dependency_links = [link.split()[1] for link in lines if
         link.startswith('-f')]
 
 
 setup(
     name='djangorestframework-fine-permissions',
-    version='0.9.0',
+    version='0.9.2',
     packages=find_packages(exclude=["tests*"]),
     install_requires=libraries,
     dependency_links=dependency_links,
     include_package_data=True,
     long_description=long_description,
-    author='Arnaud Grausem',
-    author_email='arnaud.grausem@unistra.fr',
-    maintainer='Arnaud Grausem',
-    maintainer_email='arnaud.grausem@unistra.fr',
+    author='dnum-dip-unistra',
+    author_email='dnum-dip@unistra.fr',
+    maintainer='dnum-dip-unistra',
+    maintainer_email='dnum-dip@unistra.fr',
     description='Field level permissions for Django REST Framework',
     keywords=['django', 'REST', 'rest_framework', 'permissions'],
     url='https://github.com/unistra/django-rest-framework-fine-permissions',
     download_url='https://pypi.python.org/pypi/djangorestframework-fine-permissions',
     classifiers=[
         "Development Status :: 4 - Beta",
         "Environment :: Web Environment",
         "Framework :: Django",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: GNU General Public License v2 (GPLv2)",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
         'Framework :: Django',
-        'Framework :: Django :: 1.11',
-        'Framework :: Django :: 2.2',
         'Framework :: Django :: 3.2',
     ]
 )
```

### Comparing `djangorestframework-fine-permissions-0.9.0/tests/models.py` & `djangorestframework-fine-permissions-0.9.2/tests/models.py`

 * *Files identical despite different names*

### Comparing `djangorestframework-fine-permissions-0.9.0/tests/serializers.py` & `djangorestframework-fine-permissions-0.9.2/tests/serializers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-
+from rest_framework import serializers as drf_serializers
 from rest_framework_fine_permissions import serializers
 from rest_framework_fine_permissions import fields
-from rest_framework import serializers as drf_serializers
 
 from .models import Account, Card, Service
 
 
 class ServiceSerializer(serializers.ModelPermissionsSerializer):
 
     class Meta:
```

### Comparing `djangorestframework-fine-permissions-0.9.0/tests/test_admin.py` & `djangorestframework-fine-permissions-0.9.2/tests/test_admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,13 @@
-# -*- coding: utf-8 -*-
+from rest_framework_fine_permissions.admin import UserFieldPermissionsForm
+from rest_framework_fine_permissions.models import UserFieldPermissions
 
 from django.contrib.auth.models import User
 from django.test import TestCase
 
-from rest_framework_fine_permissions.admin import UserFieldPermissionsForm
-from rest_framework_fine_permissions.models import UserFieldPermissions
-
 
 class TestUserFieldPermissionsForm(TestCase):
 
     def setUp(self):
         self.user = User.objects.create_user('test_user')
 
     def test_user_field_permissions_form_save(self):
```

### Comparing `djangorestframework-fine-permissions-0.9.0/tests/test_fields.py` & `djangorestframework-fine-permissions-0.9.2/tests/test_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-from django.test import TestCase
-from django.http import HttpRequest
 from rest_framework.exceptions import ValidationError
 from rest_framework_fine_permissions.fields import (
     get_serializer, ModelPermissionsField)
 
+from django.http import HttpRequest
+from django.test import TestCase
+
 from . import models
 from . import serializers
 from . import utils
 
 
 class TestModelFieldPermissions(TestCase):
```

### Comparing `djangorestframework-fine-permissions-0.9.0/tests/test_qserializers.py` & `djangorestframework-fine-permissions-0.9.2/tests/test_qserializers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,19 @@
-# -*- coding: utf-8 -*-
+import datetime
 
-from django.test import TestCase
-from django.db.models import Q
+from rest_framework_fine_permissions.filters import FilterPermissionBackend
+from rest_framework_fine_permissions.models import FilterPermissionModel
+from rest_framework_fine_permissions.permissions import FilterPermission
 from rest_framework_fine_permissions.serializers import QSerializer
-import datetime
+
 from django.contrib.auth.models import User
 from django.contrib.contenttypes.models import ContentType
-from rest_framework_fine_permissions.models import FilterPermissionModel
-from rest_framework_fine_permissions.permissions import FilterPermission
+from django.db.models import Q
 from django.http import HttpRequest
-from rest_framework_fine_permissions.filters import FilterPermissionBackend
-
-"""
-
-Run this test under a django application, with the following command :
-
-python manage.py test rest_framework_fine_permissions
-
-"""
+from django.test import TestCase
 
 
 class TestQSerializer(TestCase):
     """
     test the q serializer
     """
```

### Comparing `djangorestframework-fine-permissions-0.9.0/tests/test_serializers.py` & `djangorestframework-fine-permissions-0.9.2/tests/test_serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import collections
-from django.test import TestCase
-from django.http import HttpRequest
-from rest_framework.utils.model_meta import get_field_info
 
+from rest_framework.utils.model_meta import get_field_info
 from rest_framework_fine_permissions import fields
 
+from django.http import HttpRequest
+from django.test import TestCase
+
 from . import utils
 from . import serializers
 
 
 class ModelSerializerTestMixin(object):
 
     """ Mixin for testing Serializer. """
```

### Comparing `djangorestframework-fine-permissions-0.9.0/tests/test_utils.py` & `djangorestframework-fine-permissions-0.9.2/tests/test_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
-from django.test import TestCase
 from rest_framework_fine_permissions import utils
+
+from django.test import TestCase
+
 from . import serializers as test_serializers
 from .models import Account
 
 
 class TestUtilities(TestCase):
 
     """ Test utility functions. """
```

### Comparing `djangorestframework-fine-permissions-0.9.0/tests/test_views.py` & `djangorestframework-fine-permissions-0.9.2/tests/test_views.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import json
 
+from rest_framework_fine_permissions.models import UserFieldPermissions
+
+from django.contrib import messages
 from django.contrib.messages.storage.cookie import (
     CookieStorage, MessageDecoder, MessageEncoder,
 )
-
 from django.contrib.messages import get_messages
-from django.contrib import messages
-
 from django.core.files.uploadedfile import SimpleUploadedFile
 from django.http import HttpRequest
 from django.test import TestCase
 
-from rest_framework_fine_permissions.models import UserFieldPermissions
 from . import utils
 
 
 class TestViews(TestCase):
 
     """ Test views. """
 
@@ -32,14 +31,15 @@
 
     def _get_messages(self, response):
         storage = self.storage_class(response)
         cookie = response.cookies.get(storage.cookie_name)
         if not cookie or cookie['max-age'] == 0:
             return []
 
+        # return list(get_messages(response.wsgi_request))
         return storage._decode(cookie.value)
 
 
     def test_permissions_export_json_unauthorized(self):
         self._add_field_perms('tests', 'account', 'id', 'user')
         self.client.login(username='test', password='pass')
         ufp = UserFieldPermissions.objects.get(user=self.user)
```

### Comparing `djangorestframework-fine-permissions-0.9.0/tests/utils.py` & `djangorestframework-fine-permissions-0.9.2/tests/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
+from rest_framework_fine_permissions import models
+
 from django.contrib.auth.models import User
 from django.contrib.contenttypes.models import ContentType
-from rest_framework_fine_permissions import models
 
-from .models import Card, Account, Service, TestUser
+from .models import Account, Card, Service, TestUser
 
 
 def create_user(username='test', password='pass', **kwargs):
     """ Create a user for tests. """
     return User.objects.create_user(username, password=password, **kwargs)
```

