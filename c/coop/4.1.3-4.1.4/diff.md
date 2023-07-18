# Comparing `tmp/coop-4.1.3.tar.gz` & `tmp/coop-4.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coop-4.1.3.tar", last modified: Wed Feb 22 04:27:24 2023, max compression
+gzip compressed data, was "coop-4.1.4.tar", last modified: Tue Jul 18 01:40:08 2023, max compression
```

## Comparing `coop-4.1.3.tar` & `coop-4.1.4.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 04:27:24.146912 coop-4.1.3/
--rw-rw-rw-   0 root         (0) root         (0)      184 2023-02-22 04:27:12.000000 coop-4.1.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2049 2023-02-22 04:27:24.146912 coop-4.1.3/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1243 2023-02-22 04:27:12.000000 coop-4.1.3/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 04:27:24.122911 coop-4.1.3/coop/
--rw-rw-rw-   0 root         (0) root         (0)      123 2023-02-22 04:27:12.000000 coop-4.1.3/coop/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       68 2023-02-22 04:27:12.000000 coop-4.1.3/coop/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1893 2023-02-22 04:27:12.000000 coop-4.1.3/coop/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)     3623 2023-02-22 04:27:12.000000 coop-4.1.3/coop/factories.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 04:27:24.127911 coop-4.1.3/coop/form_builder/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-22 04:27:12.000000 coop-4.1.3/coop/form_builder/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5193 2023-02-22 04:27:12.000000 coop-4.1.3/coop/form_builder/blocks.py
--rw-rw-rw-   0 root         (0) root         (0)     2618 2023-02-22 04:27:12.000000 coop-4.1.3/coop/form_builder/factories.py
--rw-rw-rw-   0 root         (0) root         (0)      254 2023-02-22 04:27:12.000000 coop-4.1.3/coop/form_builder/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1168 2023-02-22 04:27:12.000000 coop-4.1.3/coop/form_builder/page.py
--rw-rw-rw-   0 root         (0) root         (0)     2468 2023-02-22 04:27:12.000000 coop-4.1.3/coop/form_builder/views.py
--rw-rw-rw-   0 root         (0) root         (0)      238 2023-02-22 04:27:12.000000 coop-4.1.3/coop/forms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 04:27:24.113910 coop-4.1.3/coop/jinja2/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 04:27:24.127911 coop-4.1.3/coop/jinja2/coop/
--rw-rw-rw-   0 root         (0) root         (0)      477 2023-02-22 04:27:12.000000 coop-4.1.3/coop/jinja2/coop/analytics_warning.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 04:27:24.127911 coop-4.1.3/coop/jinja2tags/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-22 04:27:12.000000 coop-4.1.3/coop/jinja2tags/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     9390 2023-02-22 04:27:12.000000 coop-4.1.3/coop/jinja2tags/core.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-02-22 04:27:12.000000 coop-4.1.3/coop/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 04:27:24.128911 coop-4.1.3/coop/management/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-22 04:27:12.000000 coop-4.1.3/coop/management/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 04:27:24.129912 coop-4.1.3/coop/management/commands/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-22 04:27:12.000000 coop-4.1.3/coop/management/commands/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1761 2023-02-22 04:27:12.000000 coop-4.1.3/coop/management/commands/phone_home.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 04:27:24.130911 coop-4.1.3/coop/migrations/
--rw-rw-rw-   0 root         (0) root         (0)      863 2023-02-22 04:27:12.000000 coop-4.1.3/coop/migrations/0001_remove_site.py
--rw-rw-rw-   0 root         (0) root         (0)      949 2023-02-22 04:27:12.000000 coop-4.1.3/coop/migrations/0002_analyticssettings.py
--rw-rw-rw-   0 root         (0) root         (0)      767 2023-02-22 04:27:12.000000 coop-4.1.3/coop/migrations/0003_tag_manager_settings.py
--rw-rw-rw-   0 root         (0) root         (0)      822 2023-02-22 04:27:12.000000 coop-4.1.3/coop/migrations/0004_increase_analytics_length.py
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-22 04:27:12.000000 coop-4.1.3/coop/migrations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      508 2023-02-22 04:27:12.000000 coop-4.1.3/coop/models.py
--rw-rw-rw-   0 root         (0) root         (0)     3103 2023-02-22 04:27:12.000000 coop-4.1.3/coop/page.py
--rw-rw-rw-   0 root         (0) root         (0)     5157 2023-02-22 04:27:12.000000 coop-4.1.3/coop/settings.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 04:27:24.131912 coop-4.1.3/coop/styleguide/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-22 04:27:12.000000 coop-4.1.3/coop/styleguide/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-02-22 04:27:12.000000 coop-4.1.3/coop/styleguide/urls.py
--rw-rw-rw-   0 root         (0) root         (0)      188 2023-02-22 04:27:12.000000 coop-4.1.3/coop/styleguide/views.py
--rw-rw-rw-   0 root         (0) root         (0)     4637 2023-02-22 04:27:12.000000 coop-4.1.3/coop/test.py
--rw-rw-rw-   0 root         (0) root         (0)     2087 2023-02-22 04:27:12.000000 coop-4.1.3/coop/urls.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 04:27:24.134912 coop-4.1.3/coop/utils/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-02-22 04:27:12.000000 coop-4.1.3/coop/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1591 2023-02-22 04:27:12.000000 coop-4.1.3/coop/utils/forms.py
--rw-rw-rw-   0 root         (0) root         (0)     1039 2023-02-22 04:27:12.000000 coop-4.1.3/coop/utils/mailchimp.py
--rw-rw-rw-   0 root         (0) root         (0)      628 2023-02-22 04:27:12.000000 coop-4.1.3/coop/utils/migrations.py
--rw-rw-rw-   0 root         (0) root         (0)      578 2023-02-22 04:27:12.000000 coop-4.1.3/coop/utils/pagination.py
--rw-rw-rw-   0 root         (0) root         (0)      699 2023-02-22 04:27:12.000000 coop-4.1.3/coop/utils/rich_text_example.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 04:27:24.135912 coop-4.1.3/coop/utils/test_documents/
--rw-rw-rw-   0 root         (0) root         (0)   504692 2023-02-22 04:27:12.000000 coop-4.1.3/coop/utils/test_documents/magazine-article.pdf
--rw-rw-rw-   0 root         (0) root         (0)   515133 2023-02-22 04:27:12.000000 coop-4.1.3/coop/utils/test_documents/nj-logos.pdf
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 04:27:24.145913 coop-4.1.3/coop/utils/test_images/
--rw-rw-rw-   0 root         (0) root         (0)  3653229 2023-02-22 04:27:12.000000 coop-4.1.3/coop/utils/test_images/landscape-large.jpg
--rw-rw-rw-   0 root         (0) root         (0)    11487 2023-02-22 04:27:12.000000 coop-4.1.3/coop/utils/test_images/landscape-small.jpeg
--rw-rw-rw-   0 root         (0) root         (0)  2821960 2023-02-22 04:27:12.000000 coop-4.1.3/coop/utils/test_images/portrait-large.jpg
--rw-rw-rw-   0 root         (0) root         (0)     6608 2023-02-22 04:27:12.000000 coop-4.1.3/coop/utils/test_images/portrait-small.jpeg
--rw-rw-rw-   0 root         (0) root         (0)     8126 2023-02-22 04:27:12.000000 coop-4.1.3/coop/utils/testdata.py
--rw-rw-rw-   0 root         (0) root         (0)     2025 2023-02-22 04:27:12.000000 coop-4.1.3/coop/utils/views.py
--rw-rw-rw-   0 root         (0) root         (0)     1421 2023-02-22 04:27:12.000000 coop-4.1.3/coop/wagtail_hooks.py
--rw-rw-rw-   0 root         (0) root         (0)      129 2023-02-22 04:27:12.000000 coop-4.1.3/coop/wsgi.py
--rw-rw-rw-   0 root         (0) root         (0)      159 2023-02-22 04:27:12.000000 coop-4.1.3/coop/wsgi_dev.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 04:27:24.124911 coop-4.1.3/coop.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2049 2023-02-22 04:27:24.000000 coop-4.1.3/coop.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1615 2023-02-22 04:27:24.000000 coop-4.1.3/coop.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-22 04:27:24.000000 coop-4.1.3/coop.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-22 04:27:24.000000 coop-4.1.3/coop.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      352 2023-02-22 04:27:24.000000 coop-4.1.3/coop.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-02-22 04:27:24.000000 coop-4.1.3/coop.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      237 2023-02-22 04:27:24.147913 coop-4.1.3/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1821 2023-02-22 04:27:12.000000 coop-4.1.3/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-22 04:27:24.146912 coop-4.1.3/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1658 2023-02-22 04:27:12.000000 coop-4.1.3/tests/test_analytics_panel.py
--rw-rw-rw-   0 root         (0) root         (0)     2813 2023-02-22 04:27:12.000000 coop-4.1.3/tests/test_jinja2tags.py
--rw-rw-rw-   0 root         (0) root         (0)     1259 2023-02-22 04:27:12.000000 coop-4.1.3/tests/test_page.py
--rw-rw-rw-   0 root         (0) root         (0)      703 2023-02-22 04:27:12.000000 coop-4.1.3/tests/test_test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:40:08.320377 coop-4.1.4/
+-rw-rw-rw-   0 root         (0) root         (0)      184 2023-07-18 01:39:59.000000 coop-4.1.4/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-07-18 01:40:08.320377 coop-4.1.4/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1243 2023-07-18 01:39:59.000000 coop-4.1.4/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:40:08.305377 coop-4.1.4/coop/
+-rw-rw-rw-   0 root         (0) root         (0)      123 2023-07-18 01:39:59.000000 coop-4.1.4/coop/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       68 2023-07-18 01:39:59.000000 coop-4.1.4/coop/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1893 2023-07-18 01:39:59.000000 coop-4.1.4/coop/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)     3623 2023-07-18 01:39:59.000000 coop-4.1.4/coop/factories.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:40:08.307377 coop-4.1.4/coop/form_builder/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 01:39:59.000000 coop-4.1.4/coop/form_builder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5193 2023-07-18 01:39:59.000000 coop-4.1.4/coop/form_builder/blocks.py
+-rw-rw-rw-   0 root         (0) root         (0)     2618 2023-07-18 01:39:59.000000 coop-4.1.4/coop/form_builder/factories.py
+-rw-rw-rw-   0 root         (0) root         (0)      254 2023-07-18 01:39:59.000000 coop-4.1.4/coop/form_builder/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)     1168 2023-07-18 01:39:59.000000 coop-4.1.4/coop/form_builder/page.py
+-rw-rw-rw-   0 root         (0) root         (0)     2468 2023-07-18 01:39:59.000000 coop-4.1.4/coop/form_builder/views.py
+-rw-rw-rw-   0 root         (0) root         (0)      238 2023-07-18 01:39:59.000000 coop-4.1.4/coop/forms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:40:08.298377 coop-4.1.4/coop/jinja2/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:40:08.307377 coop-4.1.4/coop/jinja2/coop/
+-rw-rw-rw-   0 root         (0) root         (0)      477 2023-07-18 01:39:59.000000 coop-4.1.4/coop/jinja2/coop/analytics_warning.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:40:08.308377 coop-4.1.4/coop/jinja2tags/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 01:39:59.000000 coop-4.1.4/coop/jinja2tags/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9390 2023-07-18 01:39:59.000000 coop-4.1.4/coop/jinja2tags/core.py
+-rw-rw-rw-   0 root         (0) root         (0)      527 2023-07-18 01:39:59.000000 coop-4.1.4/coop/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:40:08.308377 coop-4.1.4/coop/management/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 01:39:59.000000 coop-4.1.4/coop/management/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:40:08.308377 coop-4.1.4/coop/management/commands/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 01:39:59.000000 coop-4.1.4/coop/management/commands/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1761 2023-07-18 01:39:59.000000 coop-4.1.4/coop/management/commands/phone_home.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:40:08.310377 coop-4.1.4/coop/migrations/
+-rw-rw-rw-   0 root         (0) root         (0)      863 2023-07-18 01:39:59.000000 coop-4.1.4/coop/migrations/0001_remove_site.py
+-rw-rw-rw-   0 root         (0) root         (0)      949 2023-07-18 01:39:59.000000 coop-4.1.4/coop/migrations/0002_analyticssettings.py
+-rw-rw-rw-   0 root         (0) root         (0)      767 2023-07-18 01:39:59.000000 coop-4.1.4/coop/migrations/0003_tag_manager_settings.py
+-rw-rw-rw-   0 root         (0) root         (0)      822 2023-07-18 01:39:59.000000 coop-4.1.4/coop/migrations/0004_increase_analytics_length.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 01:39:59.000000 coop-4.1.4/coop/migrations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      508 2023-07-18 01:39:59.000000 coop-4.1.4/coop/models.py
+-rw-rw-rw-   0 root         (0) root         (0)     3103 2023-07-18 01:39:59.000000 coop-4.1.4/coop/page.py
+-rw-rw-rw-   0 root         (0) root         (0)     5152 2023-07-18 01:39:59.000000 coop-4.1.4/coop/settings.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:40:08.310377 coop-4.1.4/coop/styleguide/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 01:39:59.000000 coop-4.1.4/coop/styleguide/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      206 2023-07-18 01:39:59.000000 coop-4.1.4/coop/styleguide/urls.py
+-rw-rw-rw-   0 root         (0) root         (0)      188 2023-07-18 01:39:59.000000 coop-4.1.4/coop/styleguide/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     4637 2023-07-18 01:39:59.000000 coop-4.1.4/coop/test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2087 2023-07-18 01:39:59.000000 coop-4.1.4/coop/urls.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:40:08.312377 coop-4.1.4/coop/utils/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-07-18 01:39:59.000000 coop-4.1.4/coop/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1591 2023-07-18 01:39:59.000000 coop-4.1.4/coop/utils/forms.py
+-rw-rw-rw-   0 root         (0) root         (0)      931 2023-07-18 01:39:59.000000 coop-4.1.4/coop/utils/mailchimp.py
+-rw-rw-rw-   0 root         (0) root         (0)      628 2023-07-18 01:39:59.000000 coop-4.1.4/coop/utils/migrations.py
+-rw-rw-rw-   0 root         (0) root         (0)      578 2023-07-18 01:39:59.000000 coop-4.1.4/coop/utils/pagination.py
+-rw-rw-rw-   0 root         (0) root         (0)      699 2023-07-18 01:39:59.000000 coop-4.1.4/coop/utils/rich_text_example.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:40:08.313377 coop-4.1.4/coop/utils/test_documents/
+-rw-rw-rw-   0 root         (0) root         (0)   504692 2023-07-18 01:39:59.000000 coop-4.1.4/coop/utils/test_documents/magazine-article.pdf
+-rw-rw-rw-   0 root         (0) root         (0)   515133 2023-07-18 01:39:59.000000 coop-4.1.4/coop/utils/test_documents/nj-logos.pdf
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:40:08.319377 coop-4.1.4/coop/utils/test_images/
+-rw-rw-rw-   0 root         (0) root         (0)  3653229 2023-07-18 01:39:59.000000 coop-4.1.4/coop/utils/test_images/landscape-large.jpg
+-rw-rw-rw-   0 root         (0) root         (0)    11487 2023-07-18 01:39:59.000000 coop-4.1.4/coop/utils/test_images/landscape-small.jpeg
+-rw-rw-rw-   0 root         (0) root         (0)  2821960 2023-07-18 01:39:59.000000 coop-4.1.4/coop/utils/test_images/portrait-large.jpg
+-rw-rw-rw-   0 root         (0) root         (0)     6608 2023-07-18 01:39:59.000000 coop-4.1.4/coop/utils/test_images/portrait-small.jpeg
+-rw-rw-rw-   0 root         (0) root         (0)     8126 2023-07-18 01:39:59.000000 coop-4.1.4/coop/utils/testdata.py
+-rw-rw-rw-   0 root         (0) root         (0)     2025 2023-07-18 01:39:59.000000 coop-4.1.4/coop/utils/views.py
+-rw-rw-rw-   0 root         (0) root         (0)     1421 2023-07-18 01:39:59.000000 coop-4.1.4/coop/wagtail_hooks.py
+-rw-rw-rw-   0 root         (0) root         (0)      129 2023-07-18 01:39:59.000000 coop-4.1.4/coop/wsgi.py
+-rw-rw-rw-   0 root         (0) root         (0)      159 2023-07-18 01:39:59.000000 coop-4.1.4/coop/wsgi_dev.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:40:08.306377 coop-4.1.4/coop.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2049 2023-07-18 01:40:08.000000 coop-4.1.4/coop.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1615 2023-07-18 01:40:08.000000 coop-4.1.4/coop.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 01:40:08.000000 coop-4.1.4/coop.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-07-18 01:40:08.000000 coop-4.1.4/coop.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      350 2023-07-18 01:40:08.000000 coop-4.1.4/coop.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-07-18 01:40:08.000000 coop-4.1.4/coop.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      237 2023-07-18 01:40:08.320377 coop-4.1.4/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1819 2023-07-18 01:39:59.000000 coop-4.1.4/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-07-18 01:40:08.319377 coop-4.1.4/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1658 2023-07-18 01:39:59.000000 coop-4.1.4/tests/test_analytics_panel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2813 2023-07-18 01:39:59.000000 coop-4.1.4/tests/test_jinja2tags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1259 2023-07-18 01:39:59.000000 coop-4.1.4/tests/test_page.py
+-rw-rw-rw-   0 root         (0) root         (0)      703 2023-07-18 01:39:59.000000 coop-4.1.4/tests/test_test.py
```

### Comparing `coop-4.1.3/PKG-INFO` & `coop-4.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coop
-Version: 4.1.3
+Version: 4.1.4
 Summary: Standard base to build Wagtail sites from
 Home-page: https://gitlab.com/neonjungle/coop
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `coop-4.1.3/README.rst` & `coop-4.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/blocks.py` & `coop-4.1.4/coop/blocks.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/factories.py` & `coop-4.1.4/coop/factories.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/form_builder/blocks.py` & `coop-4.1.4/coop/form_builder/blocks.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/form_builder/factories.py` & `coop-4.1.4/coop/form_builder/factories.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/form_builder/page.py` & `coop-4.1.4/coop/form_builder/page.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/form_builder/views.py` & `coop-4.1.4/coop/form_builder/views.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/jinja2tags/core.py` & `coop-4.1.4/coop/jinja2tags/core.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/management/commands/phone_home.py` & `coop-4.1.4/coop/management/commands/phone_home.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/migrations/0001_remove_site.py` & `coop-4.1.4/coop/migrations/0001_remove_site.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/migrations/0002_analyticssettings.py` & `coop-4.1.4/coop/migrations/0002_analyticssettings.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/migrations/0003_tag_manager_settings.py` & `coop-4.1.4/coop/migrations/0003_tag_manager_settings.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/migrations/0004_increase_analytics_length.py` & `coop-4.1.4/coop/migrations/0004_increase_analytics_length.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/page.py` & `coop-4.1.4/coop/page.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/settings.py` & `coop-4.1.4/coop/settings.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,188 +1,179 @@
 import posixpath
 
 # Misc rubbish
 SITE_ID = 1
 DEFAULT_PER_PAGE = 20
 
 # Sites built on coop all share a common URL structure and WSGI application
-ROOT_URLCONF = 'coop.urls'
-WSGI_APPLICATION = 'coop.wsgi.application'
+ROOT_URLCONF = "coop.urls"
+WSGI_APPLICATION = "coop.wsgi.application"
 
 
 # URLs for assets
-ASSETS_URL = '/assets/'
-MEDIA_URL = posixpath.join(ASSETS_URL, 'media/')
-STATIC_URL = posixpath.join(ASSETS_URL, 'static/')
+ASSETS_URL = "/assets/"
+MEDIA_URL = posixpath.join(ASSETS_URL, "media/")
+STATIC_URL = posixpath.join(ASSETS_URL, "static/")
 
-STATICFILES_STORAGE = 'django.contrib.staticfiles.storage.ManifestStaticFilesStorage'
+STATICFILES_STORAGE = "django.contrib.staticfiles.storage.ManifestStaticFilesStorage"
 
 
 # What is installed by default
 INSTALLED_APPS = [
-    'coop',
-
+    "coop",
     # Third party apps
-    'taggit',
-    'modelcluster',
-    'wagtailmetadata',
-    'wagtailcache',
-    'wagtailfontawesome',
-    'webpack_loader',
-    'honeypot',
-
+    "taggit",
+    "modelcluster",
+    "wagtailmetadata",
+    "wagtailcache",
+    "wagtailfontawesome",
+    "webpack_loader",
+    "honeypot",
     # Django apps
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.messages',
-    'django.contrib.staticfiles',
-    'django.contrib.admin',
-    'django.contrib.sitemaps.views',
-
+    "django.contrib.auth",
+    "django.contrib.contenttypes",
+    "django.contrib.sessions",
+    "django.contrib.messages",
+    "django.contrib.staticfiles",
+    "django.contrib.admin",
+    "django.contrib.sitemaps.views",
     # Wagtail apps
-    'wagtail',
-    'wagtail.admin',
-    'wagtail.documents',
-    'wagtail.snippets',
-    'wagtail.sites',
-    'wagtail.users',
-    'wagtail.images',
-    'wagtail.embeds',
-    'wagtail.search',
-    'wagtail.contrib.redirects',
-    'wagtail.contrib.settings',
-    'wagtail.contrib.table_block',
+    "wagtail",
+    "wagtail.admin",
+    "wagtail.documents",
+    "wagtail.snippets",
+    "wagtail.sites",
+    "wagtail.users",
+    "wagtail.images",
+    "wagtail.embeds",
+    "wagtail.search",
+    "wagtail.contrib.redirects",
+    "wagtail.contrib.settings",
+    "wagtail.contrib.table_block",
 ]
 
 try:
     import diskcache  # noqa
-    INSTALLED_APPS.append('diskcache')
+
+    INSTALLED_APPS.append("diskcache")
 
     DISK_CACHE = {
-        'BACKEND': 'diskcache.DjangoCache',
-        'LOCATION': '/srv/cache',
-        'TIMEOUT': 300,
+        "BACKEND": "diskcache.DjangoCache",
+        "LOCATION": "/srv/cache",
+        "TIMEOUT": 300,
         # ^-- Django setting for default timeout of each key.
-        'SHARDS': 8,
-        'DATABASE_TIMEOUT': 0.010,  # 10 milliseconds
+        "SHARDS": 8,
+        "DATABASE_TIMEOUT": 0.010,  # 10 milliseconds
         # ^-- Timeout for each DjangoCache database transaction.
-        'OPTIONS': {
-            'size_limit': 2 ** 30   # 1 gigabyte
-        },
-    }
-    CACHES = {
-        'default': DISK_CACHE,
-        'renditions': DISK_CACHE
+        "OPTIONS": {"size_limit": 2**30},  # 1 gigabyte
     }
+    CACHES = {"default": DISK_CACHE, "renditions": DISK_CACHE}
 except ImportError:
     pass
 
 
 # Localisation - most sites are Australian
-TIME_ZONE = 'Australia/Hobart'
-LANGUAGE_CODE = 'en-au'
+TIME_ZONE = "Australia/Hobart"
+LANGUAGE_CODE = "en-au"
 
 USE_I18N = True
 USE_L10N = False
 USE_TZ = True
 
 
 # Standard middleware required by Wagtail
 MIDDLEWARE = [
-    'bugsnag.django.middleware.BugsnagMiddleware',
-    'wagtailcache.cache.UpdateCacheMiddleware',
-
-    'django.middleware.common.CommonMiddleware',
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.middleware.csrf.CsrfViewMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',
-    'django.middleware.clickjacking.XFrameOptionsMiddleware',
-
-    'wagtail.contrib.redirects.middleware.RedirectMiddleware',
-    'wagtailcache.cache.FetchFromCacheMiddleware',
+    "wagtailcache.cache.UpdateCacheMiddleware",
+    "django.middleware.common.CommonMiddleware",
+    "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.middleware.csrf.CsrfViewMiddleware",
+    "django.contrib.auth.middleware.AuthenticationMiddleware",
+    "django.contrib.messages.middleware.MessageMiddleware",
+    "django.middleware.clickjacking.XFrameOptionsMiddleware",
+    "wagtail.contrib.redirects.middleware.RedirectMiddleware",
+    "wagtailcache.cache.FetchFromCacheMiddleware",
 ]
 
 
 # Wagtail uses Django templates, but we use Jinja templates.
 # Some common Jinja extensions are used that cover most use-cases we need.
 TEMPLATES_DJANGO = {
-    'BACKEND': 'django.template.backends.django.DjangoTemplates',
-    'APP_DIRS': True,
-    'OPTIONS': {
-        'context_processors': [
-            'django.contrib.auth.context_processors.auth',
-            'django.template.context_processors.debug',
-            'django.template.context_processors.i18n',
-            'django.template.context_processors.media',
-            'django.template.context_processors.static',
-            'django.template.context_processors.tz',
-            'django.contrib.messages.context_processors.messages',
-            'django.template.context_processors.request',
-            'wagtail.contrib.settings.context_processors.settings',
+    "BACKEND": "django.template.backends.django.DjangoTemplates",
+    "APP_DIRS": True,
+    "OPTIONS": {
+        "context_processors": [
+            "django.contrib.auth.context_processors.auth",
+            "django.template.context_processors.debug",
+            "django.template.context_processors.i18n",
+            "django.template.context_processors.media",
+            "django.template.context_processors.static",
+            "django.template.context_processors.tz",
+            "django.contrib.messages.context_processors.messages",
+            "django.template.context_processors.request",
+            "wagtail.contrib.settings.context_processors.settings",
         ]
-    }
+    },
 }
 TEMPLATES_JINJA = {
-    'BACKEND': 'django.template.backends.jinja2.Jinja2',
-    'APP_DIRS': True,
-    'OPTIONS': {
-        'extensions': [
-            'wagtail.jinja2tags.core',
-            'wagtail.admin.jinja2tags.userbar',
-            'wagtail.images.jinja2tags.images',
-            'wagtail.contrib.settings.jinja2tags.settings',
-            'coop.jinja2tags.core.Extension',
-            'wagtailmetadata.jinja2tags.WagtailMetadataExtension',
+    "BACKEND": "django.template.backends.jinja2.Jinja2",
+    "APP_DIRS": True,
+    "OPTIONS": {
+        "extensions": [
+            "wagtail.jinja2tags.core",
+            "wagtail.admin.jinja2tags.userbar",
+            "wagtail.images.jinja2tags.images",
+            "wagtail.contrib.settings.jinja2tags.settings",
+            "coop.jinja2tags.core.Extension",
+            "wagtailmetadata.jinja2tags.WagtailMetadataExtension",
         ],
     },
 }
 
 TEMPLATES = [TEMPLATES_DJANGO, TEMPLATES_JINJA]
 WAGTAIL_CACHE = True
 
 
 # Who to email when things break
 ADMINS = [
-    ('Django debug', 'django@neonjungle.studio'),
+    ("Django debug", "django@neonjungle.studio"),
 ]
 LOGGING = {
-    'version': 1,
-    'disable_existing_loggers': False,
-    'filters': {
-        'require_debug_false': {
-            '()': 'django.utils.log.RequireDebugFalse'
+    "version": 1,
+    "disable_existing_loggers": False,
+    "filters": {
+        "require_debug_false": {"()": "django.utils.log.RequireDebugFalse"},
+        "bugsnag_filter": {
+            "()": "coop.logging.RequireNoBugsnagSetting",
+        },
+        "sentry_filter": {
+            "()": "coop.logging.RequireNoSentryInstalled",
         },
-        'bugsnag_filter': {
-            '()': 'coop.logging.RequireNoBugsnagSetting'
-        }
     },
-    'handlers': {
-        'mail_admins': {
-            'level': 'ERROR',
-            'filters': ['require_debug_false', 'bugsnag_filter'],
-            'class': 'django.utils.log.AdminEmailHandler'
+    "handlers": {
+        "mail_admins": {
+            "level": "ERROR",
+            "filters": ["require_debug_false", "bugsnag_filter", "sentry_filter"],
+            "class": "django.utils.log.AdminEmailHandler",
         }
     },
-    'loggers': {
-        'django.request': {
-            'handlers': ['mail_admins'],
-            'level': 'ERROR',
-            'propagate': False,
+    "loggers": {
+        "django.request": {
+            "handlers": ["mail_admins"],
+            "level": "ERROR",
+            "propagate": False,
         },
-    }
+    },
 }
 
 # Stop us from getting moderation emails by default
 WAGTAILADMIN_NOTIFICATION_INCLUDE_SUPERUSERS = False
 
 # Max image upload size
 WAGTAILIMAGES_MAX_UPLOAD_SIZE = 100 * 1024 * 1024  # 100mb
 
 # Add the 'responsive-object' class to embeds by default
 WAGTAILEMBEDS_RESPONSIVE_HTML = True
 
 # Override if you actually need a zip_code
-HONEYPOT_FIELD_NAME = 'zip_code'
+HONEYPOT_FIELD_NAME = "zip_code"
 
-DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
+DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
```

### Comparing `coop-4.1.3/coop/test.py` & `coop-4.1.4/coop/test.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/urls.py` & `coop-4.1.4/coop/urls.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/utils/forms.py` & `coop-4.1.4/coop/utils/forms.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/utils/migrations.py` & `coop-4.1.4/coop/utils/migrations.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/utils/pagination.py` & `coop-4.1.4/coop/utils/pagination.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/utils/rich_text_example.html` & `coop-4.1.4/coop/utils/rich_text_example.html`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/utils/test_documents/magazine-article.pdf` & `coop-4.1.4/coop/utils/test_documents/magazine-article.pdf`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/utils/test_documents/nj-logos.pdf` & `coop-4.1.4/coop/utils/test_documents/nj-logos.pdf`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/utils/test_images/landscape-large.jpg` & `coop-4.1.4/coop/utils/test_images/landscape-large.jpg`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/utils/test_images/landscape-small.jpeg` & `coop-4.1.4/coop/utils/test_images/landscape-small.jpeg`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/utils/test_images/portrait-large.jpg` & `coop-4.1.4/coop/utils/test_images/portrait-large.jpg`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/utils/test_images/portrait-small.jpeg` & `coop-4.1.4/coop/utils/test_images/portrait-small.jpeg`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/utils/testdata.py` & `coop-4.1.4/coop/utils/testdata.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/utils/views.py` & `coop-4.1.4/coop/utils/views.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop/wagtail_hooks.py` & `coop-4.1.4/coop/wagtail_hooks.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/coop.egg-info/PKG-INFO` & `coop-4.1.4/coop.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coop
-Version: 4.1.3
+Version: 4.1.4
 Summary: Standard base to build Wagtail sites from
 Home-page: https://gitlab.com/neonjungle/coop
 Author: Neon Jungle
 Author-email: developers@neonjungle.studio
 License: BSD License
 Classifier: Environment :: Web Environment
 Classifier: Intended Audience :: Developers
```

### Comparing `coop-4.1.3/coop.egg-info/SOURCES.txt` & `coop-4.1.4/coop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/setup.py` & `coop-4.1.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,17 +28,17 @@
         "pytz>=0",
         "Jinja2~=3.1.0",
         "django-honeypot~=1.0.0",
         "django-webpack-loader~=1.8.0",
         "wagtail-metadata~=4.0.0",
         "wagtailfontawesome~=1.0",
         "wagtail-icomoon",
-        "bugsnag~=4.0",
         "wagtail-cache~=2.2.0",
         "wagtail-factories~=4.0.0",
+        "sentry-sdk",
     ],
     extras_require={
         "all": [
             "mailchimp3~=3.0.0",
             "diskcache~=5.2.0",
         ],
         "cache": ["diskcache~=5.2.0"],
```

### Comparing `coop-4.1.3/tests/test_analytics_panel.py` & `coop-4.1.4/tests/test_analytics_panel.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/tests/test_jinja2tags.py` & `coop-4.1.4/tests/test_jinja2tags.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/tests/test_page.py` & `coop-4.1.4/tests/test_page.py`

 * *Files identical despite different names*

### Comparing `coop-4.1.3/tests/test_test.py` & `coop-4.1.4/tests/test_test.py`

 * *Files identical despite different names*

