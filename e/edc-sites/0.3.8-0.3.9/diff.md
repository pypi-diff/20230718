# Comparing `tmp/edc-sites-0.3.8.tar.gz` & `tmp/edc-sites-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-sites-0.3.8.tar", last modified: Tue Aug 23 02:27:56 2022, max compression
+gzip compressed data, was "edc-sites-0.3.9.tar", last modified: Sun Sep 25 22:22:59 2022, max compression
```

## Comparing `edc-sites-0.3.8.tar` & `edc-sites-0.3.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:27:56.978334 edc-sites-0.3.8/
--rw-r--r--   0 erikvw     (501) staff       (20)       86 2020-03-04 22:50:09.000000 edc-sites-0.3.8/.coveragerc
--rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-06 15:29:02.000000 edc-sites-0.3.8/.editorconfig
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:27:56.969151 edc-sites-0.3.8/.github/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:27:56.972414 edc-sites-0.3.8/.github/workflows/
--rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-23 02:27:49.000000 edc-sites-0.3.8/.github/workflows/build.yml
--rw-r--r--   0 erikvw     (501) staff       (20)     1271 2022-06-01 23:42:07.000000 edc-sites-0.3.8/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-08-23 02:27:49.000000 edc-sites-0.3.8/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-23 02:27:49.000000 edc-sites-0.3.8/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)       37 2022-06-01 23:42:07.000000 edc-sites-0.3.8/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:42:07.000000 edc-sites-0.3.8/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35149 2020-03-04 22:50:09.000000 edc-sites-0.3.8/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 23:42:07.000000 edc-sites-0.3.8/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)     4649 2022-08-23 02:27:56.978443 edc-sites-0.3.8/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     3650 2021-02-06 15:29:02.000000 edc-sites-0.3.8/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-08-23 02:27:49.000000 edc-sites-0.3.8/VERSION
--rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-23 02:27:49.000000 edc-sites-0.3.8/codecov.yml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:27:56.975664 edc-sites-0.3.8/edc_sites/
--rw-r--r--   0 erikvw     (501) staff       (20)      462 2021-02-06 15:29:02.000000 edc-sites-0.3.8/edc_sites/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2871 2021-05-15 15:45:13.000000 edc-sites-0.3.8/edc_sites/add_or_update_django_sites.py
--rw-r--r--   0 erikvw     (501) staff       (20)      324 2022-08-23 02:27:49.000000 edc-sites-0.3.8/edc_sites/admin.py
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2022-08-21 22:11:00.000000 edc-sites-0.3.8/edc_sites/admin_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1110 2022-08-21 22:11:00.000000 edc-sites-0.3.8/edc_sites/apps.py
--rw-r--r--   0 erikvw     (501) staff       (20)      114 2021-02-06 15:29:02.000000 edc-sites-0.3.8/edc_sites/forms.py
--rw-r--r--   0 erikvw     (501) staff       (20)      165 2020-03-28 22:53:39.000000 edc-sites-0.3.8/edc_sites/get_all_sites.py
--rw-r--r--   0 erikvw     (501) staff       (20)      435 2020-06-15 18:01:58.000000 edc-sites-0.3.8/edc_sites/get_country.py
--rw-r--r--   0 erikvw     (501) staff       (20)      425 2020-12-04 11:49:26.000000 edc-sites-0.3.8/edc_sites/get_site_by_attr.py
--rw-r--r--   0 erikvw     (501) staff       (20)      752 2021-02-06 15:29:02.000000 edc-sites-0.3.8/edc_sites/get_site_id.py
--rw-r--r--   0 erikvw     (501) staff       (20)      492 2021-02-06 15:29:02.000000 edc-sites-0.3.8/edc_sites/get_site_name.py
--rw-r--r--   0 erikvw     (501) staff       (20)      496 2020-05-12 20:35:06.000000 edc-sites-0.3.8/edc_sites/get_sites_by_country.py
--rw-r--r--   0 erikvw     (501) staff       (20)      491 2020-12-04 11:49:26.000000 edc-sites-0.3.8/edc_sites/get_sites_from_model.py
--rw-r--r--   0 erikvw     (501) staff       (20)      530 2021-02-06 15:29:02.000000 edc-sites-0.3.8/edc_sites/get_sites_module.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:27:56.977151 edc-sites-0.3.8/edc_sites/migrations/
--rw-r--r--   0 erikvw     (501) staff       (20)     1336 2021-02-06 15:29:02.000000 edc-sites-0.3.8/edc_sites/migrations/0001_initial.py
--rw-r--r--   0 erikvw     (501) staff       (20)      377 2020-03-04 22:50:09.000000 edc-sites-0.3.8/edc_sites/migrations/0002_auto_20190922_0452.py
--rw-r--r--   0 erikvw     (501) staff       (20)      405 2020-03-22 23:17:29.000000 edc-sites-0.3.8/edc_sites/migrations/0003_siteprofile_country.py
--rw-r--r--   0 erikvw     (501) staff       (20)      410 2020-03-22 23:17:29.000000 edc-sites-0.3.8/edc_sites/migrations/0004_siteprofile_country_code.py
--rw-r--r--   0 erikvw     (501) staff       (20)      418 2022-08-23 02:27:49.000000 edc-sites-0.3.8/edc_sites/migrations/0005_auto_20210423_1451.py
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:50:09.000000 edc-sites-0.3.8/edc_sites/migrations/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1571 2022-04-22 23:19:18.000000 edc-sites-0.3.8/edc_sites/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)     2279 2020-12-04 11:49:26.000000 edc-sites-0.3.8/edc_sites/single_site.py
--rw-r--r--   0 erikvw     (501) staff       (20)      699 2021-02-06 15:29:02.000000 edc-sites-0.3.8/edc_sites/sites.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:27:56.978130 edc-sites-0.3.8/edc_sites/tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       60 2020-03-04 22:50:09.000000 edc-sites-0.3.8/edc_sites/tests/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      266 2021-02-06 15:29:02.000000 edc-sites-0.3.8/edc_sites/tests/models.py
--rw-r--r--   0 erikvw     (501) staff       (20)      293 2021-02-06 15:29:02.000000 edc-sites-0.3.8/edc_sites/tests/site_test_case_mixin.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1278 2021-02-06 15:29:02.000000 edc-sites-0.3.8/edc_sites/tests/sites.py
--rw-r--r--   0 erikvw     (501) staff       (20)     5882 2021-05-15 16:32:45.000000 edc-sites-0.3.8/edc_sites/tests/test_sites.py
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-01 23:42:07.000000 edc-sites-0.3.8/edc_sites/tests/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      281 2022-08-21 22:11:00.000000 edc-sites-0.3.8/edc_sites/urls.py
--rw-r--r--   0 erikvw     (501) staff       (20)      595 2020-03-28 22:53:39.000000 edc-sites-0.3.8/edc_sites/view_mixins.py
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-08-23 02:27:56.976429 edc-sites-0.3.8/edc_sites.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)     4649 2022-08-23 02:27:56.000000 edc-sites-0.3.8/edc_sites.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1289 2022-08-23 02:27:56.000000 edc-sites-0.3.8/edc_sites.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-08-23 02:27:56.000000 edc-sites-0.3.8/edc_sites.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-05 13:01:53.000000 edc-sites-0.3.8/edc_sites.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)       10 2022-08-23 02:27:56.000000 edc-sites-0.3.8/edc_sites.egg-info/top_level.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1720 2022-08-23 02:27:49.000000 edc-sites-0.3.8/pyproject.toml
--rw-r--r--   0 erikvw     (501) staff       (20)     1668 2021-05-15 16:32:45.000000 edc-sites-0.3.8/runtests.py
--rw-r--r--   0 erikvw     (501) staff       (20)     1260 2022-08-23 02:27:56.978791 edc-sites-0.3.8/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:22:59.637497 edc-sites-0.3.9/
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2020-03-04 22:50:09.000000 edc-sites-0.3.9/.coveragerc
+-rw-r--r--   0 erikvw     (501) staff       (20)      436 2021-02-06 15:29:02.000000 edc-sites-0.3.9/.editorconfig
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:22:59.628829 edc-sites-0.3.9/.github/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:22:59.631955 edc-sites-0.3.9/.github/workflows/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1935 2022-08-23 02:27:49.000000 edc-sites-0.3.9/.github/workflows/build.yml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1271 2022-06-01 23:42:07.000000 edc-sites-0.3.9/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2022-09-25 22:22:51.000000 edc-sites-0.3.9/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-23 02:27:49.000000 edc-sites-0.3.9/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)       37 2022-06-01 23:42:07.000000 edc-sites-0.3.9/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-06-01 23:42:07.000000 edc-sites-0.3.9/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35149 2020-03-04 22:50:09.000000 edc-sites-0.3.9/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)       74 2022-06-01 23:42:07.000000 edc-sites-0.3.9/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)     4649 2022-09-25 22:22:59.637583 edc-sites-0.3.9/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     3650 2021-02-06 15:29:02.000000 edc-sites-0.3.9/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2022-09-25 22:22:51.000000 edc-sites-0.3.9/VERSION
+-rw-r--r--   0 erikvw     (501) staff       (20)      168 2022-08-23 02:27:49.000000 edc-sites-0.3.9/codecov.yml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:22:59.635104 edc-sites-0.3.9/edc_sites/
+-rw-r--r--   0 erikvw     (501) staff       (20)      462 2021-02-06 15:29:02.000000 edc-sites-0.3.9/edc_sites/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2871 2021-05-15 15:45:13.000000 edc-sites-0.3.9/edc_sites/add_or_update_django_sites.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      324 2022-08-23 02:27:49.000000 edc-sites-0.3.9/edc_sites/admin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2022-08-21 22:11:00.000000 edc-sites-0.3.9/edc_sites/admin_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1110 2022-08-21 22:11:00.000000 edc-sites-0.3.9/edc_sites/apps.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      114 2021-02-06 15:29:02.000000 edc-sites-0.3.9/edc_sites/forms.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      165 2020-03-28 22:53:39.000000 edc-sites-0.3.9/edc_sites/get_all_sites.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      435 2020-06-15 18:01:58.000000 edc-sites-0.3.9/edc_sites/get_country.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      425 2020-12-04 11:49:26.000000 edc-sites-0.3.9/edc_sites/get_site_by_attr.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      752 2021-02-06 15:29:02.000000 edc-sites-0.3.9/edc_sites/get_site_id.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      492 2021-02-06 15:29:02.000000 edc-sites-0.3.9/edc_sites/get_site_name.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      496 2020-05-12 20:35:06.000000 edc-sites-0.3.9/edc_sites/get_sites_by_country.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      491 2020-12-04 11:49:26.000000 edc-sites-0.3.9/edc_sites/get_sites_from_model.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      530 2021-02-06 15:29:02.000000 edc-sites-0.3.9/edc_sites/get_sites_module.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:22:59.636520 edc-sites-0.3.9/edc_sites/migrations/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1336 2021-02-06 15:29:02.000000 edc-sites-0.3.9/edc_sites/migrations/0001_initial.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      377 2020-03-04 22:50:09.000000 edc-sites-0.3.9/edc_sites/migrations/0002_auto_20190922_0452.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      405 2020-03-22 23:17:29.000000 edc-sites-0.3.9/edc_sites/migrations/0003_siteprofile_country.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      410 2020-03-22 23:17:29.000000 edc-sites-0.3.9/edc_sites/migrations/0004_siteprofile_country_code.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      418 2022-08-23 02:27:49.000000 edc-sites-0.3.9/edc_sites/migrations/0005_auto_20210423_1451.py
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-03-04 22:50:09.000000 edc-sites-0.3.9/edc_sites/migrations/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1571 2022-04-22 23:19:18.000000 edc-sites-0.3.9/edc_sites/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     2279 2020-12-04 11:49:26.000000 edc-sites-0.3.9/edc_sites/single_site.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      699 2021-02-06 15:29:02.000000 edc-sites-0.3.9/edc_sites/sites.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:22:59.637291 edc-sites-0.3.9/edc_sites/tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       60 2020-03-04 22:50:09.000000 edc-sites-0.3.9/edc_sites/tests/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      266 2021-02-06 15:29:02.000000 edc-sites-0.3.9/edc_sites/tests/models.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      293 2021-02-06 15:29:02.000000 edc-sites-0.3.9/edc_sites/tests/site_test_case_mixin.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1278 2021-02-06 15:29:02.000000 edc-sites-0.3.9/edc_sites/tests/sites.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     5882 2021-05-15 16:32:45.000000 edc-sites-0.3.9/edc_sites/tests/test_sites.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2022-06-01 23:42:07.000000 edc-sites-0.3.9/edc_sites/tests/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      281 2022-08-21 22:11:00.000000 edc-sites-0.3.9/edc_sites/urls.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      574 2022-09-25 22:22:51.000000 edc-sites-0.3.9/edc_sites/view_mixins.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2022-09-25 22:22:59.635658 edc-sites-0.3.9/edc_sites.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)     4649 2022-09-25 22:22:59.000000 edc-sites-0.3.9/edc_sites.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1289 2022-09-25 22:22:59.000000 edc-sites-0.3.9/edc_sites.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-09-25 22:22:59.000000 edc-sites-0.3.9/edc_sites.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2020-03-05 13:01:53.000000 edc-sites-0.3.9/edc_sites.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)       10 2022-09-25 22:22:59.000000 edc-sites-0.3.9/edc_sites.egg-info/top_level.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1720 2022-08-23 02:27:49.000000 edc-sites-0.3.9/pyproject.toml
+-rw-r--r--   0 erikvw     (501) staff       (20)     1668 2021-05-15 16:32:45.000000 edc-sites-0.3.9/runtests.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     1260 2022-09-25 22:22:59.637875 edc-sites-0.3.9/setup.cfg
```

### Comparing `edc-sites-0.3.8/.github/workflows/build.yml` & `edc-sites-0.3.9/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/.gitignore` & `edc-sites-0.3.9/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/.pre-commit-config.yaml` & `edc-sites-0.3.9/.pre-commit-config.yaml`

 * *Files 7% similar despite different names*

```diff
@@ -9,15 +9,15 @@
         args:
           - "-x *test*.py"
 
   - repo: https://github.com/psf/black
     rev: 22.6.0
     hooks:
       - id: black
-        language_version: python3.8
+        language_version: python3.9
 
   - repo: https://github.com/pycqa/flake8
     rev: 5.0.4
     hooks:
       - id: flake8
         args:
           - "--config=setup.cfg"
```

### Comparing `edc-sites-0.3.8/LICENSE` & `edc-sites-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/PKG-INFO` & `edc-sites-0.3.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-sites
-Version: 0.3.8
+Version: 0.3.9
 Summary: Simple classes related to the django sites framework for clinicedc projects
 Home-page: https://github.com/clinicedc/edc-sites
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc sites,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-sites-0.3.8/README.rst` & `edc-sites-0.3.9/README.rst`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/edc_sites/add_or_update_django_sites.py` & `edc-sites-0.3.9/edc_sites/add_or_update_django_sites.py`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/edc_sites/apps.py` & `edc-sites-0.3.9/edc_sites/apps.py`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/edc_sites/get_site_id.py` & `edc-sites-0.3.9/edc_sites/get_site_id.py`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/edc_sites/get_sites_module.py` & `edc-sites-0.3.9/edc_sites/get_sites_module.py`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/edc_sites/migrations/0001_initial.py` & `edc-sites-0.3.9/edc_sites/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/edc_sites/models.py` & `edc-sites-0.3.9/edc_sites/models.py`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/edc_sites/single_site.py` & `edc-sites-0.3.9/edc_sites/single_site.py`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/edc_sites/sites.py` & `edc-sites-0.3.9/edc_sites/sites.py`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/edc_sites/tests/sites.py` & `edc-sites-0.3.9/edc_sites/tests/sites.py`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/edc_sites/tests/test_sites.py` & `edc-sites-0.3.9/edc_sites/tests/test_sites.py`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/edc_sites/view_mixins.py` & `edc-sites-0.3.9/edc_sites/view_mixins.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+from __future__ import annotations
+
 from django.core.exceptions import ObjectDoesNotExist
-from django.views.generic.base import ContextMixin
 
 from .models import SiteProfile
 
 
-class SiteViewMixin(ContextMixin):
-    def get_context_data(self, **kwargs):
+class SiteViewMixin:
+    def get_context_data(self, **kwargs) -> dict:
         context = super().get_context_data(**kwargs)
         try:
             site_profile = SiteProfile.objects.get(site__id=self.request.site.id)
         except ObjectDoesNotExist:
             context.update(site_profile=None)
         else:
             context.update(site_title=site_profile.title)
```

### Comparing `edc-sites-0.3.8/edc_sites.egg-info/PKG-INFO` & `edc-sites-0.3.9/edc_sites.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc-sites
-Version: 0.3.8
+Version: 0.3.9
 Summary: Simple classes related to the django sites framework for clinicedc projects
 Home-page: https://github.com/clinicedc/edc-sites
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django Edc sites,clinicedc,clinical trials
 Classifier: Environment :: Web Environment
```

### Comparing `edc-sites-0.3.8/edc_sites.egg-info/SOURCES.txt` & `edc-sites-0.3.9/edc_sites.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/pyproject.toml` & `edc-sites-0.3.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/runtests.py` & `edc-sites-0.3.9/runtests.py`

 * *Files identical despite different names*

### Comparing `edc-sites-0.3.8/setup.cfg` & `edc-sites-0.3.9/setup.cfg`

 * *Files identical despite different names*

