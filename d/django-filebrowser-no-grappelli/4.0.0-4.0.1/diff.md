# Comparing `tmp/django-filebrowser-no-grappelli-4.0.0.tar.gz` & `tmp/django-filebrowser-no-grappelli-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-filebrowser-no-grappelli-4.0.0.tar", last modified: Wed Feb  2 10:29:48 2022, max compression
+gzip compressed data, was "django-filebrowser-no-grappelli-4.0.1.tar", last modified: Wed Mar  2 11:50:53 2022, max compression
```

## Comparing `django-filebrowser-no-grappelli-4.0.0.tar` & `django-filebrowser-no-grappelli-4.0.1.tar`

### file list

```diff
@@ -1,247 +1,247 @@
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.653782 django-filebrowser-no-grappelli-4.0.0/
--rw-r--r--   0 smacker    (501) staff       (20)      204 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/AUTHORS
--rw-r--r--   0 smacker    (501) staff       (20)     1539 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/LICENSE
--rw-r--r--   0 smacker    (501) staff       (20)      265 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/MANIFEST.in
--rw-r--r--   0 smacker    (501) staff       (20)     3484 2022-02-02 10:29:48.653622 django-filebrowser-no-grappelli-4.0.0/PKG-INFO
--rw-r--r--   0 smacker    (501) staff       (20)     2335 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.0/README.rst
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.619667 django-filebrowser-no-grappelli-4.0.0/django_filebrowser_no_grappelli.egg-info/
--rw-r--r--   0 smacker    (501) staff       (20)     3484 2022-02-02 10:29:48.000000 django-filebrowser-no-grappelli-4.0.0/django_filebrowser_no_grappelli.egg-info/PKG-INFO
--rw-r--r--   0 smacker    (501) staff       (20)     6988 2022-02-02 10:29:48.000000 django-filebrowser-no-grappelli-4.0.0/django_filebrowser_no_grappelli.egg-info/SOURCES.txt
--rw-r--r--   0 smacker    (501) staff       (20)        1 2022-02-02 10:29:48.000000 django-filebrowser-no-grappelli-4.0.0/django_filebrowser_no_grappelli.egg-info/dependency_links.txt
--rw-r--r--   0 smacker    (501) staff       (20)        1 2022-02-02 10:29:48.000000 django-filebrowser-no-grappelli-4.0.0/django_filebrowser_no_grappelli.egg-info/not-zip-safe
--rw-r--r--   0 smacker    (501) staff       (20)        4 2022-02-02 10:29:48.000000 django-filebrowser-no-grappelli-4.0.0/django_filebrowser_no_grappelli.egg-info/requires.txt
--rw-r--r--   0 smacker    (501) staff       (20)       12 2022-02-02 10:29:48.000000 django-filebrowser-no-grappelli-4.0.0/django_filebrowser_no_grappelli.egg-info/top_level.txt
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.622562 django-filebrowser-no-grappelli-4.0.0/docs/
--rw-r--r--   0 smacker    (501) staff       (20)     4626 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/docs/Makefile
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.622683 django-filebrowser-no-grappelli-4.0.0/docs/_static/
--rw-r--r--   0 smacker    (501) staff       (20)    51594 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/docs/_static/Screenshot.png
--rw-r--r--   0 smacker    (501) staff       (20)    10823 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.0/docs/admin.rst
--rw-r--r--   0 smacker    (501) staff       (20)      145 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/docs/api.rst
--rw-r--r--   0 smacker    (501) staff       (20)     1758 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.0/docs/changelog.rst
--rw-r--r--   0 smacker    (501) staff       (20)     7396 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/docs/conf.py
--rw-r--r--   0 smacker    (501) staff       (20)     1833 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/docs/faq.rst
--rw-r--r--   0 smacker    (501) staff       (20)     4199 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.0/docs/fieldswidgets.rst
--rw-r--r--   0 smacker    (501) staff       (20)     4439 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/docs/filelisting.rst
--rw-r--r--   0 smacker    (501) staff       (20)     8942 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/docs/fileobject.rst
--rw-r--r--   0 smacker    (501) staff       (20)      175 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/docs/help.rst
--rw-r--r--   0 smacker    (501) staff       (20)     2387 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/docs/index.rst
--rw-r--r--   0 smacker    (501) staff       (20)     1838 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.0/docs/quickstart.rst
--rw-r--r--   0 smacker    (501) staff       (20)     1016 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/docs/releasenotes.rst
--rw-r--r--   0 smacker    (501) staff       (20)     9270 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/docs/settings.rst
--rw-r--r--   0 smacker    (501) staff       (20)      407 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/docs/testing.rst
--rw-r--r--   0 smacker    (501) staff       (20)      345 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/docs/translation.rst
--rw-r--r--   0 smacker    (501) staff       (20)     1698 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/docs/troubleshooting.rst
--rw-r--r--   0 smacker    (501) staff       (20)     6820 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/docs/versions.rst
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.624699 django-filebrowser-no-grappelli-4.0.0/filebrowser/
--rw-r--r--   0 smacker    (501) staff       (20)       18 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/__init__.py
--rw-r--r--   0 smacker    (501) staff       (20)     2770 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/actions.py
--rw-r--r--   0 smacker    (501) staff       (20)      992 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/admin.py
--rw-r--r--   0 smacker    (501) staff       (20)    17801 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/base.py
--rw-r--r--   0 smacker    (501) staff       (20)      191 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/compat.py
--rw-r--r--   0 smacker    (501) staff       (20)     2576 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/decorators.py
--rw-r--r--   0 smacker    (501) staff       (20)    11082 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/fields.py
--rw-r--r--   0 smacker    (501) staff       (20)     3597 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/forms.py
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.617419 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.615247 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/az/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.626608 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/az/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     5090 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/az/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    11150 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/az/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.615342 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/bg_BG/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.627078 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/bg_BG/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     3473 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/bg_BG/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    13097 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/bg_BG/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.615439 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/cs/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.627376 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/cs/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6523 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/cs/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    11900 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/cs/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.615528 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/de/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.627667 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/de/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6693 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    11943 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.615626 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/en/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.627951 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/en/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     4353 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    10889 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.615747 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/es/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.628224 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/es/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6471 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    11853 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.615840 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/fa/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.628512 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/fa/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     7031 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/fa/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    12373 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/fa/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.615941 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/fr/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.629026 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/fr/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6898 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    12180 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.616047 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/is/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.629324 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/is/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6281 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/is/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    11616 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/is/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.616155 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/it/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.629587 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/it/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6256 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    11649 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.616250 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ja/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.629836 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ja/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6763 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ja/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    12683 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ja/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.616347 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ja_JP/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.630098 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ja_JP/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)      515 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    12625 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ja_JP/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.616442 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/mn/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.630344 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/mn/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     7635 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/mn/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    12997 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/mn/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.616532 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/nb/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.630769 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/nb/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6479 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    11693 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/nb/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.616629 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/nl/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.630908 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/nl/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     9648 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/nl/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.616720 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/pl_PL/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.631171 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/pl_PL/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6376 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/pl_PL/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    11775 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/pl_PL/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.616813 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/pt_BR/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.631450 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/pt_BR/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6386 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    11724 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/pt_BR/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.616903 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ru_RU/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.631730 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ru_RU/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     8012 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ru_RU/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    13428 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ru_RU/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.616995 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sk/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.632004 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sk/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6689 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sk/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    11938 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sk/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.617083 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sl_SI/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.632405 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sl_SI/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6047 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sl_SI/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    11583 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sl_SI/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.617173 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sv/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.632781 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sv/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6399 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sv/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    11611 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sv/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.617262 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/tr_TR/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.633142 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/tr_TR/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6180 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    11594 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/tr_TR/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.617354 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/vi/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.633421 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/vi/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6682 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/vi/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    11899 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/vi/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.617453 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/zh_Hans/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.633718 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/zh_Hans/LC_MESSAGES/
--rw-r--r--   0 smacker    (501) staff       (20)     6234 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/zh_Hans/LC_MESSAGES/django.mo
--rw-r--r--   0 smacker    (501) staff       (20)    11501 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/zh_Hans/LC_MESSAGES/django.po
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.633847 django-filebrowser-no-grappelli-4.0.0/filebrowser/management/
--rw-r--r--   0 smacker    (501) staff       (20)        0 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/management/__init__.py
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.633939 django-filebrowser-no-grappelli-4.0.0/filebrowser/management/__pycache__/
--rw-r--r--   0 smacker    (501) staff       (20)      176 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/management/__pycache__/__init__.cpython-38.pyc
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.634426 django-filebrowser-no-grappelli-4.0.0/filebrowser/management/commands/
--rw-r--r--   0 smacker    (501) staff       (20)        0 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/management/commands/__init__.py
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.634805 django-filebrowser-no-grappelli-4.0.0/filebrowser/management/commands/__pycache__/
--rw-r--r--   0 smacker    (501) staff       (20)      185 2022-02-02 09:06:44.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/management/commands/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)     2414 2022-02-02 09:06:44.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/management/commands/__pycache__/fb_version_generate.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)     3739 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/management/commands/fb_version_generate.py
--rw-r--r--   0 smacker    (501) staff       (20)     5126 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/management/commands/fb_version_remove.py
--rw-r--r--   0 smacker    (501) staff       (20)      246 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/models.py
--rw-r--r--   0 smacker    (501) staff       (20)     3088 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/namers.py
--rw-r--r--   0 smacker    (501) staff       (20)     6230 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/settings.py
--rw-r--r--   0 smacker    (501) staff       (20)     1740 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/signals.py
--rw-r--r--   0 smacker    (501) staff       (20)    26150 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/sites.py
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.617780 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.617917 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.635168 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/css/
--rw-r--r--   0 smacker    (501) staff       (20)     6969 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/css/filebrowser.css
--rw-r--r--   0 smacker    (501) staff       (20)     4778 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/css/uploadfield.css
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.642140 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/
--rw-r--r--   0 smacker    (501) staff       (20)   870037 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/TEST_IMAGE_000.jpg
--rw-r--r--   0 smacker    (501) staff       (20)      236 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/cancel.png
--rw-r--r--   0 smacker    (501) staff       (20)      236 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/cancel_hover.png
--rw-r--r--   0 smacker    (501) staff       (20)     1122 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/completed.png
--rw-r--r--   0 smacker    (501) staff       (20)     3027 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/fb-upload-spinner.gif
--rw-r--r--   0 smacker    (501) staff       (20)     1090 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/fb-upload.png
--rw-r--r--   0 smacker    (501) staff       (20)     1091 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/fb-upload_hover.png
--rw-r--r--   0 smacker    (501) staff       (20)      427 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/filebrowser_icon_show.gif
--rw-r--r--   0 smacker    (501) staff       (20)      426 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/filebrowser_icon_show_hover.gif
--rw-r--r--   0 smacker    (501) staff       (20)      165 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/icon-pulldown-versions-active.png
--rw-r--r--   0 smacker    (501) staff       (20)      165 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/icon-pulldown-versions-hover.png
--rw-r--r--   0 smacker    (501) staff       (20)      165 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/icon-pulldown-versions.png
--rw-r--r--   0 smacker    (501) staff       (20)      367 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/progress-bar-content.png
--rw-r--r--   0 smacker    (501) staff       (20)       13 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/test_not_an_image.jpg
--rw-r--r--   0 smacker    (501) staff       (20)   870037 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/testimage.jpg
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.645393 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/
--rw-r--r--   0 smacker    (501) staff       (20)     1478 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/AddFileBrowser.js
--rw-r--r--   0 smacker    (501) staff       (20)      622 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/FB_CKEditor.js
--rw-r--r--   0 smacker    (501) staff       (20)     1351 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/FB_FileBrowseField.js
--rw-r--r--   0 smacker    (501) staff       (20)      942 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/FB_TinyMCE.js
--rw-r--r--   0 smacker    (501) staff       (20)      647 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/FB_TinyMCEv4.js
--rw-r--r--   0 smacker    (501) staff       (20)      197 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/FB_TinyMCEv5.js
--rw-r--r--   0 smacker    (501) staff       (20)     5651 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/TinyMCEAdmin.js
--rw-r--r--   0 smacker    (501) staff       (20)     1478 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/TinyMCEv4Admin.js
--rw-r--r--   0 smacker    (501) staff       (20)     1287 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/TinyMCEv5Admin.js
--rw-r--r--   0 smacker    (501) staff       (20)    40071 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/fileuploader.js
--rw-r--r--   0 smacker    (501) staff       (20)     5481 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/storage.py
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.618009 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.646502 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/
--rw-r--r--   0 smacker    (501) staff       (20)     2433 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/createdir.html
--rw-r--r--   0 smacker    (501) staff       (20)     1741 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/custom_field.html
--rw-r--r--   0 smacker    (501) staff       (20)     5165 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/custom_upload_field.html
--rw-r--r--   0 smacker    (501) staff       (20)     1298 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/delete_confirm.html
--rw-r--r--   0 smacker    (501) staff       (20)     6583 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/detail.html
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.647703 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/include/
--rw-r--r--   0 smacker    (501) staff       (20)       14 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/include/_response.html
--rw-r--r--   0 smacker    (501) staff       (20)     1058 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/include/breadcrumbs.html
--rw-r--r--   0 smacker    (501) staff       (20)     6766 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/include/filelisting.html
--rw-r--r--   0 smacker    (501) staff       (20)     1757 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/include/filter.html
--rw-r--r--   0 smacker    (501) staff       (20)      824 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/include/paginator.html
--rw-r--r--   0 smacker    (501) staff       (20)     5605 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/include/tableheader.html
--rw-r--r--   0 smacker    (501) staff       (20)     2063 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/include/toolbar.html
--rw-r--r--   0 smacker    (501) staff       (20)     7866 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/index.html
--rw-r--r--   0 smacker    (501) staff       (20)     7296 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/upload.html
--rw-r--r--   0 smacker    (501) staff       (20)     2425 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/version.html
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.648520 django-filebrowser-no-grappelli-4.0.0/filebrowser/templatetags/
--rw-r--r--   0 smacker    (501) staff       (20)        0 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templatetags/__init__.py
--rw-r--r--   0 smacker    (501) staff       (20)      563 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templatetags/fb_compat.py
--rw-r--r--   0 smacker    (501) staff       (20)     1041 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templatetags/fb_csrf.py
--rw-r--r--   0 smacker    (501) staff       (20)     1740 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templatetags/fb_pagination.py
--rw-r--r--   0 smacker    (501) staff       (20)     4473 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templatetags/fb_tags.py
--rw-r--r--   0 smacker    (501) staff       (20)     4341 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/templatetags/fb_versions.py
--rw-r--r--   0 smacker    (501) staff       (20)     2878 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/filebrowser/utils.py
--rw-r--r--   0 smacker    (501) staff       (20)       38 2022-02-02 10:29:48.653823 django-filebrowser-no-grappelli-4.0.0/setup.cfg
--rw-r--r--   0 smacker    (501) staff       (20)     1454 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.0/setup.py
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.650729 django-filebrowser-no-grappelli-4.0.0/tests/
--rw-r--r--   0 smacker    (501) staff       (20)     2305 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/tests/__init__.py
-drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-02-02 10:29:48.653264 django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/
--rw-r--r--   0 smacker    (501) staff       (20)     2256 2022-02-02 09:06:42.000000 django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)     2420 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/base.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)      336 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/models.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)     2021 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/settings.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)    16138 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_base.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)     1504 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_commands.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)     3177 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_decorators.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)     1205 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_fields.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)     3494 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_namers.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)      164 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_settings.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)    11801 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_sites.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)     1271 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_templatetags.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)    20105 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_versions.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)      623 2022-02-02 09:08:55.000000 django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/urls.cpython-38.pyc
--rw-r--r--   0 smacker    (501) staff       (20)     2671 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/tests/base.py
--rw-r--r--   0 smacker    (501) staff       (20)      202 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/tests/models.py
--rw-r--r--   0 smacker    (501) staff       (20)      142 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/tests/requirements.txt
--rw-r--r--   0 smacker    (501) staff       (20)     2783 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/tests/settings.py
--rw-r--r--   0 smacker    (501) staff       (20)    21290 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/tests/test_base.py
--rw-r--r--   0 smacker    (501) staff       (20)     1011 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/tests/test_commands.py
--rw-r--r--   0 smacker    (501) staff       (20)     1953 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/tests/test_decorators.py
--rw-r--r--   0 smacker    (501) staff       (20)     1230 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/tests/test_fields.py
--rw-r--r--   0 smacker    (501) staff       (20)     3478 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/tests/test_namers.py
--rw-r--r--   0 smacker    (501) staff       (20)     3451 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/tests/test_settings.py
--rw-r--r--   0 smacker    (501) staff       (20)    13383 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/tests/test_sites.py
--rw-r--r--   0 smacker    (501) staff       (20)      806 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/tests/test_templatetags.py
--rw-r--r--   0 smacker    (501) staff       (20)    22385 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.0/tests/test_versions.py
--rw-r--r--   0 smacker    (501) staff       (20)      587 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.0/tests/urls.py
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.168066 django-filebrowser-no-grappelli-4.0.1/
+-rw-r--r--   0 smacker    (501) staff       (20)      204 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/AUTHORS
+-rw-r--r--   0 smacker    (501) staff       (20)     1539 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/LICENSE
+-rw-r--r--   0 smacker    (501) staff       (20)      265 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/MANIFEST.in
+-rw-r--r--   0 smacker    (501) staff       (20)     3481 2022-03-02 11:50:53.167874 django-filebrowser-no-grappelli-4.0.1/PKG-INFO
+-rw-r--r--   0 smacker    (501) staff       (20)     2332 2022-03-02 11:46:13.000000 django-filebrowser-no-grappelli-4.0.1/README.rst
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.130755 django-filebrowser-no-grappelli-4.0.1/django_filebrowser_no_grappelli.egg-info/
+-rw-r--r--   0 smacker    (501) staff       (20)     3481 2022-03-02 11:50:52.000000 django-filebrowser-no-grappelli-4.0.1/django_filebrowser_no_grappelli.egg-info/PKG-INFO
+-rw-r--r--   0 smacker    (501) staff       (20)     6988 2022-03-02 11:50:53.000000 django-filebrowser-no-grappelli-4.0.1/django_filebrowser_no_grappelli.egg-info/SOURCES.txt
+-rw-r--r--   0 smacker    (501) staff       (20)        1 2022-03-02 11:50:52.000000 django-filebrowser-no-grappelli-4.0.1/django_filebrowser_no_grappelli.egg-info/dependency_links.txt
+-rw-r--r--   0 smacker    (501) staff       (20)        1 2022-02-02 10:29:48.000000 django-filebrowser-no-grappelli-4.0.1/django_filebrowser_no_grappelli.egg-info/not-zip-safe
+-rw-r--r--   0 smacker    (501) staff       (20)        4 2022-03-02 11:50:53.000000 django-filebrowser-no-grappelli-4.0.1/django_filebrowser_no_grappelli.egg-info/requires.txt
+-rw-r--r--   0 smacker    (501) staff       (20)       12 2022-03-02 11:50:53.000000 django-filebrowser-no-grappelli-4.0.1/django_filebrowser_no_grappelli.egg-info/top_level.txt
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.135369 django-filebrowser-no-grappelli-4.0.1/docs/
+-rw-r--r--   0 smacker    (501) staff       (20)     4626 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/docs/Makefile
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.135622 django-filebrowser-no-grappelli-4.0.1/docs/_static/
+-rw-r--r--   0 smacker    (501) staff       (20)    51594 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/docs/_static/Screenshot.png
+-rw-r--r--   0 smacker    (501) staff       (20)    10823 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.1/docs/admin.rst
+-rw-r--r--   0 smacker    (501) staff       (20)      145 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/docs/api.rst
+-rw-r--r--   0 smacker    (501) staff       (20)     1862 2022-03-02 11:47:44.000000 django-filebrowser-no-grappelli-4.0.1/docs/changelog.rst
+-rw-r--r--   0 smacker    (501) staff       (20)     7396 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/docs/conf.py
+-rw-r--r--   0 smacker    (501) staff       (20)     1833 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/docs/faq.rst
+-rw-r--r--   0 smacker    (501) staff       (20)     4199 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.1/docs/fieldswidgets.rst
+-rw-r--r--   0 smacker    (501) staff       (20)     4439 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/docs/filelisting.rst
+-rw-r--r--   0 smacker    (501) staff       (20)     8942 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/docs/fileobject.rst
+-rw-r--r--   0 smacker    (501) staff       (20)      175 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/docs/help.rst
+-rw-r--r--   0 smacker    (501) staff       (20)     2387 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/docs/index.rst
+-rw-r--r--   0 smacker    (501) staff       (20)     1838 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.1/docs/quickstart.rst
+-rw-r--r--   0 smacker    (501) staff       (20)     1016 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/docs/releasenotes.rst
+-rw-r--r--   0 smacker    (501) staff       (20)     9270 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/docs/settings.rst
+-rw-r--r--   0 smacker    (501) staff       (20)      407 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/docs/testing.rst
+-rw-r--r--   0 smacker    (501) staff       (20)      345 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/docs/translation.rst
+-rw-r--r--   0 smacker    (501) staff       (20)     1698 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/docs/troubleshooting.rst
+-rw-r--r--   0 smacker    (501) staff       (20)     6820 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/docs/versions.rst
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.138842 django-filebrowser-no-grappelli-4.0.1/filebrowser/
+-rw-r--r--   0 smacker    (501) staff       (20)       18 2022-03-02 11:47:50.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/__init__.py
+-rw-r--r--   0 smacker    (501) staff       (20)     2770 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/actions.py
+-rw-r--r--   0 smacker    (501) staff       (20)      992 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/admin.py
+-rw-r--r--   0 smacker    (501) staff       (20)    17801 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/base.py
+-rw-r--r--   0 smacker    (501) staff       (20)      191 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/compat.py
+-rw-r--r--   0 smacker    (501) staff       (20)     2576 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/decorators.py
+-rw-r--r--   0 smacker    (501) staff       (20)    11082 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/fields.py
+-rw-r--r--   0 smacker    (501) staff       (20)     3597 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/forms.py
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.127903 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.125458 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/az/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.139259 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/az/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     5090 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/az/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    11150 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/az/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.125563 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/bg_BG/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.139719 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/bg_BG/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     3473 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/bg_BG/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    13097 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/bg_BG/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.125665 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/cs/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.140007 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/cs/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6523 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    11900 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/cs/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.125767 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/de/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.140273 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/de/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6693 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    11943 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.125867 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/en/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.140550 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/en/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     4353 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    10889 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.125970 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/es/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.140833 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/es/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6471 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    11853 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.126067 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/fa/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.141112 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/fa/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     7031 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/fa/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    12373 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/fa/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.126177 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/fr/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.141564 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6898 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    12180 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.126300 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/is/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.141841 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/is/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6281 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/is/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    11616 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/is/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.126405 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/it/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.142112 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/it/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6256 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    11649 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.126520 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ja/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.142390 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ja/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6763 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ja/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    12683 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ja/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.126624 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ja_JP/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.142661 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)      515 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    12625 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ja_JP/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.126729 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/mn/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.142937 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/mn/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     7635 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/mn/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    12997 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/mn/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.126844 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/nb/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.143386 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/nb/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6479 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    11693 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/nb/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.126950 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/nl/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.143519 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/nl/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     9648 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/nl/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.127059 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/pl_PL/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.143795 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/pl_PL/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6376 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/pl_PL/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    11775 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/pl_PL/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.127174 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/pt_BR/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.144121 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6386 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    11724 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/pt_BR/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.127285 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ru_RU/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.144395 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     8012 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ru_RU/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    13428 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ru_RU/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.127393 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sk/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.144660 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sk/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6689 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sk/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    11938 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sk/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.127498 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sl_SI/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.144922 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sl_SI/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6047 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sl_SI/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    11583 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sl_SI/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.127600 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sv/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.145314 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sv/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6399 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sv/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    11611 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sv/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.127712 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/tr_TR/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.145593 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6180 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    11594 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/tr_TR/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.127818 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/vi/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.145863 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/vi/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6682 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/vi/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    11899 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/vi/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.127972 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/zh_Hans/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.146134 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/zh_Hans/LC_MESSAGES/
+-rw-r--r--   0 smacker    (501) staff       (20)     6234 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/zh_Hans/LC_MESSAGES/django.mo
+-rw-r--r--   0 smacker    (501) staff       (20)    11501 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/zh_Hans/LC_MESSAGES/django.po
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.146263 django-filebrowser-no-grappelli-4.0.1/filebrowser/management/
+-rw-r--r--   0 smacker    (501) staff       (20)        0 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/management/__init__.py
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.146352 django-filebrowser-no-grappelli-4.0.1/filebrowser/management/__pycache__/
+-rw-r--r--   0 smacker    (501) staff       (20)      176 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/management/__pycache__/__init__.cpython-38.pyc
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.146838 django-filebrowser-no-grappelli-4.0.1/filebrowser/management/commands/
+-rw-r--r--   0 smacker    (501) staff       (20)        0 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/management/commands/__init__.py
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.147252 django-filebrowser-no-grappelli-4.0.1/filebrowser/management/commands/__pycache__/
+-rw-r--r--   0 smacker    (501) staff       (20)      185 2022-02-02 09:06:44.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/management/commands/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)     2414 2022-02-02 09:06:44.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/management/commands/__pycache__/fb_version_generate.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)     3739 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/management/commands/fb_version_generate.py
+-rw-r--r--   0 smacker    (501) staff       (20)     5126 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/management/commands/fb_version_remove.py
+-rw-r--r--   0 smacker    (501) staff       (20)      246 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/models.py
+-rw-r--r--   0 smacker    (501) staff       (20)     3088 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/namers.py
+-rw-r--r--   0 smacker    (501) staff       (20)     6230 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/settings.py
+-rw-r--r--   0 smacker    (501) staff       (20)     1740 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/signals.py
+-rw-r--r--   0 smacker    (501) staff       (20)    26150 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/sites.py
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.128354 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.128517 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.147637 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/css/
+-rw-r--r--   0 smacker    (501) staff       (20)     6969 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/css/filebrowser.css
+-rw-r--r--   0 smacker    (501) staff       (20)     4778 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/css/uploadfield.css
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.152920 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/
+-rw-r--r--   0 smacker    (501) staff       (20)   870037 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/TEST_IMAGE_000.jpg
+-rw-r--r--   0 smacker    (501) staff       (20)      236 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/cancel.png
+-rw-r--r--   0 smacker    (501) staff       (20)      236 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/cancel_hover.png
+-rw-r--r--   0 smacker    (501) staff       (20)     1122 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/completed.png
+-rw-r--r--   0 smacker    (501) staff       (20)     3027 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/fb-upload-spinner.gif
+-rw-r--r--   0 smacker    (501) staff       (20)     1090 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/fb-upload.png
+-rw-r--r--   0 smacker    (501) staff       (20)     1091 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/fb-upload_hover.png
+-rw-r--r--   0 smacker    (501) staff       (20)      427 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/filebrowser_icon_show.gif
+-rw-r--r--   0 smacker    (501) staff       (20)      426 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/filebrowser_icon_show_hover.gif
+-rw-r--r--   0 smacker    (501) staff       (20)      165 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/icon-pulldown-versions-active.png
+-rw-r--r--   0 smacker    (501) staff       (20)      165 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/icon-pulldown-versions-hover.png
+-rw-r--r--   0 smacker    (501) staff       (20)      165 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/icon-pulldown-versions.png
+-rw-r--r--   0 smacker    (501) staff       (20)      367 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/progress-bar-content.png
+-rw-r--r--   0 smacker    (501) staff       (20)       13 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/test_not_an_image.jpg
+-rw-r--r--   0 smacker    (501) staff       (20)   870037 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/testimage.jpg
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.156176 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/
+-rw-r--r--   0 smacker    (501) staff       (20)     1478 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/AddFileBrowser.js
+-rw-r--r--   0 smacker    (501) staff       (20)      622 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/FB_CKEditor.js
+-rw-r--r--   0 smacker    (501) staff       (20)     1351 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/FB_FileBrowseField.js
+-rw-r--r--   0 smacker    (501) staff       (20)      942 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/FB_TinyMCE.js
+-rw-r--r--   0 smacker    (501) staff       (20)      647 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/FB_TinyMCEv4.js
+-rw-r--r--   0 smacker    (501) staff       (20)      197 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/FB_TinyMCEv5.js
+-rw-r--r--   0 smacker    (501) staff       (20)     5651 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/TinyMCEAdmin.js
+-rw-r--r--   0 smacker    (501) staff       (20)     1478 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/TinyMCEv4Admin.js
+-rw-r--r--   0 smacker    (501) staff       (20)     1287 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/TinyMCEv5Admin.js
+-rw-r--r--   0 smacker    (501) staff       (20)    40071 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/fileuploader.js
+-rw-r--r--   0 smacker    (501) staff       (20)     5481 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/storage.py
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.128635 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.157659 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/
+-rw-r--r--   0 smacker    (501) staff       (20)     2433 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/createdir.html
+-rw-r--r--   0 smacker    (501) staff       (20)     1741 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/custom_field.html
+-rw-r--r--   0 smacker    (501) staff       (20)     5165 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/custom_upload_field.html
+-rw-r--r--   0 smacker    (501) staff       (20)     1298 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/delete_confirm.html
+-rw-r--r--   0 smacker    (501) staff       (20)     6583 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/detail.html
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.158751 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/include/
+-rw-r--r--   0 smacker    (501) staff       (20)       14 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/include/_response.html
+-rw-r--r--   0 smacker    (501) staff       (20)     1058 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/include/breadcrumbs.html
+-rw-r--r--   0 smacker    (501) staff       (20)     6766 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/include/filelisting.html
+-rw-r--r--   0 smacker    (501) staff       (20)     1757 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/include/filter.html
+-rw-r--r--   0 smacker    (501) staff       (20)      824 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/include/paginator.html
+-rw-r--r--   0 smacker    (501) staff       (20)     5605 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/include/tableheader.html
+-rw-r--r--   0 smacker    (501) staff       (20)     2063 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/include/toolbar.html
+-rw-r--r--   0 smacker    (501) staff       (20)     7866 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/index.html
+-rw-r--r--   0 smacker    (501) staff       (20)     7292 2022-03-02 11:45:27.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/upload.html
+-rw-r--r--   0 smacker    (501) staff       (20)     2425 2022-02-02 10:26:54.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/version.html
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.159603 django-filebrowser-no-grappelli-4.0.1/filebrowser/templatetags/
+-rw-r--r--   0 smacker    (501) staff       (20)        0 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templatetags/__init__.py
+-rw-r--r--   0 smacker    (501) staff       (20)      563 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templatetags/fb_compat.py
+-rw-r--r--   0 smacker    (501) staff       (20)     1041 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templatetags/fb_csrf.py
+-rw-r--r--   0 smacker    (501) staff       (20)     1740 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templatetags/fb_pagination.py
+-rw-r--r--   0 smacker    (501) staff       (20)     4473 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templatetags/fb_tags.py
+-rw-r--r--   0 smacker    (501) staff       (20)     4341 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/templatetags/fb_versions.py
+-rw-r--r--   0 smacker    (501) staff       (20)     2878 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/filebrowser/utils.py
+-rw-r--r--   0 smacker    (501) staff       (20)       38 2022-03-02 11:50:53.168122 django-filebrowser-no-grappelli-4.0.1/setup.cfg
+-rw-r--r--   0 smacker    (501) staff       (20)     1454 2022-03-02 11:47:56.000000 django-filebrowser-no-grappelli-4.0.1/setup.py
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.161654 django-filebrowser-no-grappelli-4.0.1/tests/
+-rw-r--r--   0 smacker    (501) staff       (20)     2305 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/tests/__init__.py
+drwxr-xr-x   0 smacker    (501) staff       (20)        0 2022-03-02 11:50:53.164707 django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/
+-rw-r--r--   0 smacker    (501) staff       (20)     2256 2022-02-02 09:06:42.000000 django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)     2420 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/base.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)      336 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/models.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)     2021 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/settings.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)    16138 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_base.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)     1504 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_commands.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)     3177 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_decorators.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)     1205 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_fields.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)     3494 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_namers.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)      164 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_settings.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)    11801 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_sites.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)     1271 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_templatetags.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)    20105 2022-02-02 09:06:43.000000 django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_versions.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)      623 2022-02-02 09:08:55.000000 django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/urls.cpython-38.pyc
+-rw-r--r--   0 smacker    (501) staff       (20)     2671 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/tests/base.py
+-rw-r--r--   0 smacker    (501) staff       (20)      202 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/tests/models.py
+-rw-r--r--   0 smacker    (501) staff       (20)      142 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/tests/requirements.txt
+-rw-r--r--   0 smacker    (501) staff       (20)     2783 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/tests/settings.py
+-rw-r--r--   0 smacker    (501) staff       (20)    21290 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/tests/test_base.py
+-rw-r--r--   0 smacker    (501) staff       (20)     1011 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/tests/test_commands.py
+-rw-r--r--   0 smacker    (501) staff       (20)     1953 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/tests/test_decorators.py
+-rw-r--r--   0 smacker    (501) staff       (20)     1230 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/tests/test_fields.py
+-rw-r--r--   0 smacker    (501) staff       (20)     3478 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/tests/test_namers.py
+-rw-r--r--   0 smacker    (501) staff       (20)     3451 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/tests/test_settings.py
+-rw-r--r--   0 smacker    (501) staff       (20)    13383 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/tests/test_sites.py
+-rw-r--r--   0 smacker    (501) staff       (20)      806 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/tests/test_templatetags.py
+-rw-r--r--   0 smacker    (501) staff       (20)    22385 2021-11-14 07:26:45.000000 django-filebrowser-no-grappelli-4.0.1/tests/test_versions.py
+-rw-r--r--   0 smacker    (501) staff       (20)      587 2022-02-02 10:06:30.000000 django-filebrowser-no-grappelli-4.0.1/tests/urls.py
```

### Comparing `django-filebrowser-no-grappelli-4.0.0/LICENSE` & `django-filebrowser-no-grappelli-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/PKG-INFO` & `django-filebrowser-no-grappelli-4.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filebrowser-no-grappelli
-Version: 4.0.0
+Version: 4.0.1
 Summary: Media-Management no Grappelli
 Home-page: https://github.com/smacker/django-filebrowser-no-grappelli
 Download-URL: 
 Author: Patrick Kranzlmueller, Axel Swoboda (vonautomatisch)
 Author-email: office@vonautomatisch.at
 Maintainer: Maxim Sukharev
 Maintainer-email: max@smacker.ru
@@ -89,15 +89,15 @@
 -----------
 
 https://www.transifex.com/projects/p/django-filebrowser/
 
 Releases
 --------
 
-* FileBrowser 4.0.0 (February 2nd, 2022): Compatible with Django 3/4
+* FileBrowser 4.0.1 (March 2nd, 2022): Compatible with Django 3/4
 * FileBrowser 3.8.0 (November 4th, 2019): Compatible with Django 1.11/2.0/2.1/2.2/3.0
 * FileBrowser 3.7.9 (November 3rd, 2019): Compatible with Django 1.8/1.9/1.10/1.11/2.0/2.1/2.2
 * FileBrowser 3.6.2 (March 7th, 2016): Compatible with Django 1.4/1.5/1.6/1.7/1.8/1.9
 
 Older versions are available at GitHub, but are not supported anymore.
```

### Comparing `django-filebrowser-no-grappelli-4.0.0/README.rst` & `django-filebrowser-no-grappelli-4.0.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -59,13 +59,13 @@
 -----------
 
 https://www.transifex.com/projects/p/django-filebrowser/
 
 Releases
 --------
 
-* FileBrowser 4.0.0 (February 2nd, 2022): Compatible with Django 3/4
+* FileBrowser 4.0.1 (March 2nd, 2022): Compatible with Django 3/4
 * FileBrowser 3.8.0 (November 4th, 2019): Compatible with Django 1.11/2.0/2.1/2.2/3.0
 * FileBrowser 3.7.9 (November 3rd, 2019): Compatible with Django 1.8/1.9/1.10/1.11/2.0/2.1/2.2
 * FileBrowser 3.6.2 (March 7th, 2016): Compatible with Django 1.4/1.5/1.6/1.7/1.8/1.9
 
 Older versions are available at GitHub, but are not supported anymore.
```

### Comparing `django-filebrowser-no-grappelli-4.0.0/django_filebrowser_no_grappelli.egg-info/PKG-INFO` & `django-filebrowser-no-grappelli-4.0.1/django_filebrowser_no_grappelli.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-filebrowser-no-grappelli
-Version: 4.0.0
+Version: 4.0.1
 Summary: Media-Management no Grappelli
 Home-page: https://github.com/smacker/django-filebrowser-no-grappelli
 Download-URL: 
 Author: Patrick Kranzlmueller, Axel Swoboda (vonautomatisch)
 Author-email: office@vonautomatisch.at
 Maintainer: Maxim Sukharev
 Maintainer-email: max@smacker.ru
@@ -89,15 +89,15 @@
 -----------
 
 https://www.transifex.com/projects/p/django-filebrowser/
 
 Releases
 --------
 
-* FileBrowser 4.0.0 (February 2nd, 2022): Compatible with Django 3/4
+* FileBrowser 4.0.1 (March 2nd, 2022): Compatible with Django 3/4
 * FileBrowser 3.8.0 (November 4th, 2019): Compatible with Django 1.11/2.0/2.1/2.2/3.0
 * FileBrowser 3.7.9 (November 3rd, 2019): Compatible with Django 1.8/1.9/1.10/1.11/2.0/2.1/2.2
 * FileBrowser 3.6.2 (March 7th, 2016): Compatible with Django 1.4/1.5/1.6/1.7/1.8/1.9
 
 Older versions are available at GitHub, but are not supported anymore.
```

### Comparing `django-filebrowser-no-grappelli-4.0.0/django_filebrowser_no_grappelli.egg-info/SOURCES.txt` & `django-filebrowser-no-grappelli-4.0.1/django_filebrowser_no_grappelli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/docs/Makefile` & `django-filebrowser-no-grappelli-4.0.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/docs/_static/Screenshot.png` & `django-filebrowser-no-grappelli-4.0.1/docs/_static/Screenshot.png`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/docs/admin.rst` & `django-filebrowser-no-grappelli-4.0.1/docs/admin.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/docs/changelog.rst` & `django-filebrowser-no-grappelli-4.0.1/docs/changelog.rst`

 * *Files 17% similar despite different names*

```diff
@@ -4,27 +4,32 @@
 .. |filebrowser| replace:: FileBrowser
 
 .. _changelog:
 
 Changelog
 =========
 
+4.0.1 (Match 2nd, 2022)
+---------------------------
+
+* Use unminified js files. #76 Thanks to @andylolz.
+
 4.0.0 (February 2nd, 2022)
 ---------------------------
 
 * Django 4.0 support, drop Django <3. Thanks to @pulse-mind.
 * Support for TinyMCE v5. Thanks to @rmaceissoft.
 * Dropbox storage support. Thanks to @rmaceissoft.
 
-3.8.0 (Novermber 4th, 2019)
+3.8.0 (November 4th, 2019)
 ---------------------------
 
 * Django 3.0 support, drop Django <1.11. Thanks to @lpomfrey.
 
-3.7.9 (Novermber 3rd, 2019)
+3.7.9 (November 3rd, 2019)
 ---------------------------
 
 * FileObject should implement os.PathLike protocol
 
 3.7.8 (Match 25th, 2019)
 ------------------------
```

### Comparing `django-filebrowser-no-grappelli-4.0.0/docs/conf.py` & `django-filebrowser-no-grappelli-4.0.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/docs/faq.rst` & `django-filebrowser-no-grappelli-4.0.1/docs/faq.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/docs/fieldswidgets.rst` & `django-filebrowser-no-grappelli-4.0.1/docs/fieldswidgets.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/docs/filelisting.rst` & `django-filebrowser-no-grappelli-4.0.1/docs/filelisting.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/docs/fileobject.rst` & `django-filebrowser-no-grappelli-4.0.1/docs/fileobject.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/docs/index.rst` & `django-filebrowser-no-grappelli-4.0.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/docs/quickstart.rst` & `django-filebrowser-no-grappelli-4.0.1/docs/quickstart.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/docs/releasenotes.rst` & `django-filebrowser-no-grappelli-4.0.1/docs/releasenotes.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/docs/settings.rst` & `django-filebrowser-no-grappelli-4.0.1/docs/settings.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/docs/troubleshooting.rst` & `django-filebrowser-no-grappelli-4.0.1/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/docs/versions.rst` & `django-filebrowser-no-grappelli-4.0.1/docs/versions.rst`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/actions.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/actions.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/admin.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/admin.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/base.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/base.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/decorators.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/decorators.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/fields.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/fields.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/forms.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/forms.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/az/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/az/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/az/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/az/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/bg_BG/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/bg_BG/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/bg_BG/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/bg_BG/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/cs/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/cs/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/cs/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/cs/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/de/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/de/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/en/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/en/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/es/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/es/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/fa/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/fa/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/fa/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/fa/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/fr/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/fr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/fr/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/is/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/is/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/is/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/is/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/it/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/it/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/it/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ja/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ja/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ja/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ja/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ja_JP/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ja_JP/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ja_JP/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/mn/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/mn/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/mn/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/mn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/nb/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/nb/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/nb/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/nl/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/nl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/pl_PL/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/pl_PL/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/pl_PL/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/pl_PL/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/pt_BR/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/pt_BR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/pt_BR/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/pt_BR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ru_RU/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ru_RU/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/ru_RU/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/ru_RU/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sk/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sk/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sl_SI/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sl_SI/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sl_SI/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sl_SI/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sv/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sv/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/sv/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/sv/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/tr_TR/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/tr_TR/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/tr_TR/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/vi/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/vi/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/vi/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/vi/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/zh_Hans/LC_MESSAGES/django.mo` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/zh_Hans/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/locale/zh_Hans/LC_MESSAGES/django.po` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/locale/zh_Hans/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/management/commands/__pycache__/fb_version_generate.cpython-38.pyc` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/management/commands/__pycache__/fb_version_generate.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/management/commands/fb_version_generate.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/management/commands/fb_version_generate.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/management/commands/fb_version_remove.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/management/commands/fb_version_remove.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/namers.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/namers.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/settings.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/settings.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/signals.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/signals.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/sites.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/sites.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/css/filebrowser.css` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/css/filebrowser.css`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/css/uploadfield.css` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/css/uploadfield.css`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/TEST_IMAGE_000.jpg` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/TEST_IMAGE_000.jpg`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/completed.png` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/completed.png`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/fb-upload-spinner.gif` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/fb-upload-spinner.gif`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/fb-upload.png` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/fb-upload.png`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/fb-upload_hover.png` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/fb-upload_hover.png`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/img/testimage.jpg` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/img/testimage.jpg`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/AddFileBrowser.js` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/AddFileBrowser.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/FB_CKEditor.js` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/FB_CKEditor.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/FB_FileBrowseField.js` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/FB_FileBrowseField.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/FB_TinyMCE.js` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/FB_TinyMCE.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/FB_TinyMCEv4.js` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/FB_TinyMCEv4.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/TinyMCEAdmin.js` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/TinyMCEAdmin.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/TinyMCEv4Admin.js` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/TinyMCEv4Admin.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/TinyMCEv5Admin.js` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/TinyMCEv5Admin.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/static/filebrowser/js/fileuploader.js` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/static/filebrowser/js/fileuploader.js`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/storage.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/storage.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/createdir.html` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/createdir.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/custom_field.html` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/custom_field.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/custom_upload_field.html` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/custom_upload_field.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/delete_confirm.html` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/delete_confirm.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/detail.html` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/detail.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/include/breadcrumbs.html` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/include/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/include/filelisting.html` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/include/filelisting.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/include/filter.html` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/include/filter.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/include/paginator.html` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/include/paginator.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/include/tableheader.html` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/include/tableheader.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/include/toolbar.html` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/include/toolbar.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/index.html` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/index.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/upload.html` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/upload.html`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {% endblock %}
 
 <!-- JAVASCRIPTS -->
 {% block extrahead %}
     {{ block.super }}
     <script type="text/javascript" src="{% static_jquery %}"></script>
     <script type="text/javascript" src="{% static "admin/js/jquery.init.js" %}"></script>
-    <script type="text/javascript" src="{% static "admin/js/collapse.min.js" %}"></script>
+    <script type="text/javascript" src="{% static "admin/js/collapse.js" %}"></script>
     <script type="text/javascript" src="../../jsi18n/"></script>
     <script type="text/javascript" src="{% static "filebrowser/js/fileuploader.js" %}"></script>
     <script type="text/javascript">
     (function($){
         $(document).ready(function() {
             var uploader = new qq.FileUploader({
                 element: $('#file-uploader > div').get(0),
```

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templates/filebrowser/version.html` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templates/filebrowser/version.html`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templatetags/fb_compat.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templatetags/fb_compat.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templatetags/fb_csrf.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templatetags/fb_csrf.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templatetags/fb_pagination.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templatetags/fb_pagination.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templatetags/fb_tags.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templatetags/fb_tags.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/templatetags/fb_versions.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/templatetags/fb_versions.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/filebrowser/utils.py` & `django-filebrowser-no-grappelli-4.0.1/filebrowser/utils.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/setup.py` & `django-filebrowser-no-grappelli-4.0.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 def read(fname):
     return open(os.path.join(os.path.dirname(__file__), fname)).read()
 
 
 setup(
     name='django-filebrowser-no-grappelli',
-    version='4.0.0',
+    version='4.0.1',
     description='Media-Management no Grappelli',
     long_description=read('README.rst'),
     url='https://github.com/smacker/django-filebrowser-no-grappelli',
     download_url='',
     author='Patrick Kranzlmueller, Axel Swoboda (vonautomatisch)',
     author_email='office@vonautomatisch.at',
     maintainer='Maxim Sukharev',
```

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/__init__.py` & `django-filebrowser-no-grappelli-4.0.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/__init__.cpython-38.pyc` & `django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/__init__.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/base.cpython-38.pyc` & `django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/base.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/settings.cpython-38.pyc` & `django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/settings.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_base.cpython-38.pyc` & `django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_base.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_commands.cpython-38.pyc` & `django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_commands.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_decorators.cpython-38.pyc` & `django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_decorators.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_fields.cpython-38.pyc` & `django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_fields.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_namers.cpython-38.pyc` & `django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_namers.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_sites.cpython-38.pyc` & `django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_sites.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_templatetags.cpython-38.pyc` & `django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_templatetags.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/test_versions.cpython-38.pyc` & `django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/test_versions.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/__pycache__/urls.cpython-38.pyc` & `django-filebrowser-no-grappelli-4.0.1/tests/__pycache__/urls.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/base.py` & `django-filebrowser-no-grappelli-4.0.1/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/settings.py` & `django-filebrowser-no-grappelli-4.0.1/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/test_base.py` & `django-filebrowser-no-grappelli-4.0.1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/test_commands.py` & `django-filebrowser-no-grappelli-4.0.1/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/test_decorators.py` & `django-filebrowser-no-grappelli-4.0.1/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/test_fields.py` & `django-filebrowser-no-grappelli-4.0.1/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/test_namers.py` & `django-filebrowser-no-grappelli-4.0.1/tests/test_namers.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/test_settings.py` & `django-filebrowser-no-grappelli-4.0.1/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/test_sites.py` & `django-filebrowser-no-grappelli-4.0.1/tests/test_sites.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/test_templatetags.py` & `django-filebrowser-no-grappelli-4.0.1/tests/test_templatetags.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/test_versions.py` & `django-filebrowser-no-grappelli-4.0.1/tests/test_versions.py`

 * *Files identical despite different names*

### Comparing `django-filebrowser-no-grappelli-4.0.0/tests/urls.py` & `django-filebrowser-no-grappelli-4.0.1/tests/urls.py`

 * *Files identical despite different names*

