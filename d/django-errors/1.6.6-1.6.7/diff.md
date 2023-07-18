# Comparing `tmp/django-errors-1.6.6.tar.gz` & `tmp/django-errors-1.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-errors-1.6.6.tar", last modified: Sun Jul 16 22:40:12 2023, max compression
+gzip compressed data, was "django-errors-1.6.7.tar", last modified: Tue Jul 18 11:53:13 2023, max compression
```

## Comparing `django-errors-1.6.6.tar` & `django-errors-1.6.7.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-16 22:39:59.000000 django-errors-1.6.6/.bumpversion.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-16 22:39:59.000000 django-errors-1.6.6/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-16 22:39:59.000000 django-errors-1.6.6/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-16 22:39:59.000000 django-errors-1.6.6/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-16 22:39:59.000000 django-errors-1.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-16 22:39:59.000000 django-errors-1.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-16 22:40:12.637911 django-errors-1.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-16 22:39:59.000000 django-errors-1.6.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-16 22:39:59.000000 django-errors-1.6.6/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-16 22:39:59.000000 django-errors-1.6.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.633911 django-errors-1.6.6/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/docs.in
--rw-r--r--   0 runner    (1001) docker     (123)    29701 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py310-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py310-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py311-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py311-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py38-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py38-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py39-django32.txt
--rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/py39-django42.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-16 22:39:59.000000 django-errors-1.6.6/requirements/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-16 22:39:59.000000 django-errors-1.6.6/runtests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-16 22:40:12.637911 django-errors-1.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-16 22:39:59.000000 django-errors-1.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.633911 django-errors-1.6.6/src/django_errors/
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/cn/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.633911 django-errors-1.6.6/src/django_errors/locale/cn/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/cn/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.633911 django-errors-1.6.6/src/django_errors/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/es/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/it/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/locale/it/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/it/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/lt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/locale/lt/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/lt/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/middleware/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/middleware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/middleware/handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.629911 django-errors-1.6.6/src/django_errors/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/src/django_errors/templates/errors/
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/templates/errors/400.html
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/templates/errors/403.html
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/templates/errors/404.html
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/templates/errors/405.html
--rw-r--r--   0 runner    (1001) docker     (123)      288 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/templates/errors/500.html
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-16 22:39:59.000000 django-errors-1.6.6/src/django_errors/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.633911 django-errors-1.6.6/src/django_errors.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-16 22:40:12.000000 django-errors-1.6.6/src/django_errors.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-16 22:40:12.000000 django-errors-1.6.6/src/django_errors.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 22:40:12.000000 django-errors-1.6.6/src/django_errors.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-16 22:40:12.000000 django-errors-1.6.6/src/django_errors.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-16 22:40:12.000000 django-errors-1.6.6/src/django_errors.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-16 22:40:12.000000 django-errors-1.6.6/src/django_errors.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-16 22:40:12.637911 django-errors-1.6.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-16 22:39:59.000000 django-errors-1.6.6/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-16 22:39:59.000000 django-errors-1.6.6/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-16 22:39:59.000000 django-errors-1.6.6/tests/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-16 22:39:59.000000 django-errors-1.6.6/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-16 22:39:59.000000 django-errors-1.6.6/tests/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-16 22:39:59.000000 django-errors-1.6.6/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.728794 django-errors-1.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-18 11:52:59.000000 django-errors-1.6.7/.bumpversion.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-07-18 11:52:59.000000 django-errors-1.6.7/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-07-18 11:52:59.000000 django-errors-1.6.7/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-07-18 11:52:59.000000 django-errors-1.6.7/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-07-18 11:52:59.000000 django-errors-1.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-07-18 11:52:59.000000 django-errors-1.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-18 11:53:13.728794 django-errors-1.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-18 11:52:59.000000 django-errors-1.6.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-07-18 11:52:59.000000 django-errors-1.6.7/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-07-18 11:52:59.000000 django-errors-1.6.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.724794 django-errors-1.6.7/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-07-18 11:52:59.000000 django-errors-1.6.7/requirements/docs.in
+-rw-r--r--   0 runner    (1001) docker     (123)    29701 2023-07-18 11:52:59.000000 django-errors-1.6.7/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8213 2023-07-18 11:52:59.000000 django-errors-1.6.7/requirements/py310-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8012 2023-07-18 11:52:59.000000 django-errors-1.6.7/requirements/py310-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7591 2023-07-18 11:52:59.000000 django-errors-1.6.7/requirements/py311-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7390 2023-07-18 11:52:59.000000 django-errors-1.6.7/requirements/py311-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-18 11:52:59.000000 django-errors-1.6.7/requirements/py38-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9847 2023-07-18 11:52:59.000000 django-errors-1.6.7/requirements/py38-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8645 2023-07-18 11:52:59.000000 django-errors-1.6.7/requirements/py39-django32.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     8444 2023-07-18 11:52:59.000000 django-errors-1.6.7/requirements/py39-django42.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-18 11:52:59.000000 django-errors-1.6.7/requirements/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-07-18 11:52:59.000000 django-errors-1.6.7/runtests.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-07-18 11:53:13.732794 django-errors-1.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1135 2023-07-18 11:52:59.000000 django-errors-1.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.720794 django-errors-1.6.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.724794 django-errors-1.6.7/src/django_errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-07-18 11:52:59.000000 django-errors-1.6.7/src/django_errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-07-18 11:52:59.000000 django-errors-1.6.7/src/django_errors/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.720794 django-errors-1.6.7/src/django_errors/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.720794 django-errors-1.6.7/src/django_errors/locale/cn/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.728794 django-errors-1.6.7/src/django_errors/locale/cn/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-18 11:52:59.000000 django-errors-1.6.7/src/django_errors/locale/cn/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.720794 django-errors-1.6.7/src/django_errors/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.728794 django-errors-1.6.7/src/django_errors/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-18 11:52:59.000000 django-errors-1.6.7/src/django_errors/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.720794 django-errors-1.6.7/src/django_errors/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.728794 django-errors-1.6.7/src/django_errors/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-07-18 11:52:59.000000 django-errors-1.6.7/src/django_errors/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.720794 django-errors-1.6.7/src/django_errors/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.728794 django-errors-1.6.7/src/django_errors/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-07-18 11:52:59.000000 django-errors-1.6.7/src/django_errors/locale/es/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.720794 django-errors-1.6.7/src/django_errors/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.728794 django-errors-1.6.7/src/django_errors/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1561 2023-07-18 11:52:59.000000 django-errors-1.6.7/src/django_errors/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.720794 django-errors-1.6.7/src/django_errors/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.728794 django-errors-1.6.7/src/django_errors/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-07-18 11:53:00.000000 django-errors-1.6.7/src/django_errors/locale/it/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.720794 django-errors-1.6.7/src/django_errors/locale/lt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.728794 django-errors-1.6.7/src/django_errors/locale/lt/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-18 11:53:00.000000 django-errors-1.6.7/src/django_errors/locale/lt/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.720794 django-errors-1.6.7/src/django_errors/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.728794 django-errors-1.6.7/src/django_errors/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-07-18 11:53:00.000000 django-errors-1.6.7/src/django_errors/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.728794 django-errors-1.6.7/src/django_errors/middleware/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:00.000000 django-errors-1.6.7/src/django_errors/middleware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-07-18 11:53:00.000000 django-errors-1.6.7/src/django_errors/middleware/handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.720794 django-errors-1.6.7/src/django_errors/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.728794 django-errors-1.6.7/src/django_errors/templates/errors/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-18 11:53:00.000000 django-errors-1.6.7/src/django_errors/templates/errors/400.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-18 11:53:00.000000 django-errors-1.6.7/src/django_errors/templates/errors/403.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-18 11:53:00.000000 django-errors-1.6.7/src/django_errors/templates/errors/404.html
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-18 11:53:00.000000 django-errors-1.6.7/src/django_errors/templates/errors/405.html
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-07-18 11:53:00.000000 django-errors-1.6.7/src/django_errors/templates/errors/500.html
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-07-18 11:53:00.000000 django-errors-1.6.7/src/django_errors/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-07-18 11:53:00.000000 django-errors-1.6.7/src/django_errors/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.724794 django-errors-1.6.7/src/django_errors.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-07-18 11:53:13.000000 django-errors-1.6.7/src/django_errors.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-07-18 11:53:13.000000 django-errors-1.6.7/src/django_errors.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:53:13.000000 django-errors-1.6.7/src/django_errors.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 11:53:13.000000 django-errors-1.6.7/src/django_errors.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-07-18 11:53:13.000000 django-errors-1.6.7/src/django_errors.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 11:53:13.000000 django-errors-1.6.7/src/django_errors.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:13.728794 django-errors-1.6.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 11:53:00.000000 django-errors-1.6.7/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-18 11:53:00.000000 django-errors-1.6.7/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2287 2023-07-18 11:53:00.000000 django-errors-1.6.7/tests/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-07-18 11:53:00.000000 django-errors-1.6.7/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-07-18 11:53:00.000000 django-errors-1.6.7/tests/views.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-18 11:53:00.000000 django-errors-1.6.7/tox.ini
```

### Comparing `django-errors-1.6.6/.pre-commit-config.yaml` & `django-errors-1.6.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/LICENSE` & `django-errors-1.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/PKG-INFO` & `django-errors-1.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-errors
-Version: 1.6.6
+Version: 1.6.7
 Summary: Django application for handling server errors.
 Home-page: https://github.com/DLRSP/django-errors
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,errors
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-errors-1.6.6/README.md` & `django-errors-1.6.7/README.md`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/mkdocs.yml` & `django-errors-1.6.7/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/pyproject.toml` & `django-errors-1.6.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 django_find_project = false
 
 [tool.towncrier]
 package = "django_errors"
 package_dir = "src"
 filename = "CHANGELOG.rst"
 directory = "news/"
-version = "1.6.6"
+version = "1.6.7"
 
 # For rendering properly for this project
 issue_format = "`#{issue} <https://github.com/DLRSP/django-errors/issues/{issue}>`_"
 # template = "tools/news/template.rst"
 
 # Grouping of entries, within our changelog
 type = [
```

### Comparing `django-errors-1.6.6/requirements/docs.txt` & `django-errors-1.6.7/requirements/docs.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/requirements/py310-django32.txt` & `django-errors-1.6.7/requirements/py310-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/requirements/py310-django42.txt` & `django-errors-1.6.7/requirements/py310-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/requirements/py311-django32.txt` & `django-errors-1.6.7/requirements/py311-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/requirements/py311-django42.txt` & `django-errors-1.6.7/requirements/py311-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/requirements/py38-django32.txt` & `django-errors-1.6.7/requirements/py38-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/requirements/py38-django42.txt` & `django-errors-1.6.7/requirements/py38-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/requirements/py39-django32.txt` & `django-errors-1.6.7/requirements/py39-django32.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/requirements/py39-django42.txt` & `django-errors-1.6.7/requirements/py39-django42.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/runtests.py` & `django-errors-1.6.7/runtests.py`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/setup.cfg` & `django-errors-1.6.7/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [bdist_wheel]
 universal = 1
 
 [metadata]
 name = django-errors
-version = 1.6.6
+version = 1.6.7
 url = https://github.com/DLRSP/django-errors
 author = DLRSP
 author_email = dlrsp.dev@gmail.com
 description = Django application for handling server errors.
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
```

### Comparing `django-errors-1.6.6/setup.py` & `django-errors-1.6.7/setup.py`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/src/django_errors/__init__.py` & `django-errors-1.6.7/src/django_errors/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 4. push to pypi + push to github
 5. bump the version, append '.dev0'
 6. git commit
 7. push to github (to avoid confusion)
 """
 import django
 
-__version__ = "1.6.6"
+__version__ = "1.6.7"
 __version_info__ = tuple(int(i) if i.isdigit() else i for i in __version__.split("."))
 __license__ = "MIT"
 __title__ = "django_errors"
 
 __author__ = "DLRSP"
 __copyright__ = "Copyright 2010-present DLRSP"
```

### Comparing `django-errors-1.6.6/src/django_errors/locale/cn/LC_MESSAGES/django.po` & `django-errors-1.6.7/src/django_errors/locale/cn/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/src/django_errors/locale/de/LC_MESSAGES/django.po` & `django-errors-1.6.7/src/django_errors/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/src/django_errors/locale/en/LC_MESSAGES/django.po` & `django-errors-1.6.7/src/django_errors/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/src/django_errors/locale/es/LC_MESSAGES/django.po` & `django-errors-1.6.7/src/django_errors/locale/es/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/src/django_errors/locale/fr/LC_MESSAGES/django.po` & `django-errors-1.6.7/src/django_errors/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/src/django_errors/locale/it/LC_MESSAGES/django.po` & `django-errors-1.6.7/src/django_errors/locale/it/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/src/django_errors/locale/lt/LC_MESSAGES/django.po` & `django-errors-1.6.7/src/django_errors/locale/lt/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/src/django_errors/locale/ru/LC_MESSAGES/django.po` & `django-errors-1.6.7/src/django_errors/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/src/django_errors/middleware/handler.py` & `django-errors-1.6.7/src/django_errors/middleware/handler.py`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/src/django_errors/views.py` & `django-errors-1.6.7/src/django_errors/views.py`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/src/django_errors.egg-info/PKG-INFO` & `django-errors-1.6.7/src/django_errors.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-errors
-Version: 1.6.6
+Version: 1.6.7
 Summary: Django application for handling server errors.
 Home-page: https://github.com/DLRSP/django-errors
 Author: DLRSP
 Author-email: dlrsp.dev@gmail.com
 License: MIT License
 Keywords: django,errors
 Classifier: Development Status :: 4 - Beta
```

### Comparing `django-errors-1.6.6/src/django_errors.egg-info/SOURCES.txt` & `django-errors-1.6.7/src/django_errors.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/tests/test_errors.py` & `django-errors-1.6.7/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/tests/views.py` & `django-errors-1.6.7/tests/views.py`

 * *Files identical despite different names*

### Comparing `django-errors-1.6.6/tox.ini` & `django-errors-1.6.7/tox.ini`

 * *Files identical despite different names*

