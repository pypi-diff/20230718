# Comparing `tmp/location-local-0.0.2.tar.gz` & `tmp/location-local-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "location-local-0.0.2.tar", last modified: Tue Jul 18 07:31:44 2023, max compression
+gzip compressed data, was "location-local-0.0.3.tar", last modified: Tue Jul 18 07:59:06 2023, max compression
```

## Comparing `location-local-0.0.2.tar` & `location-local-0.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:31:44.349122 location-local-0.0.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:31:44.349122 location-local-0.0.2/CirclesGetCountryName/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:31:32.000000 location-local-0.0.2/CirclesGetCountryName/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-18 07:31:32.000000 location-local-0.0.2/CirclesGetCountryName/opencage_get_country_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-18 07:31:44.349122 location-local-0.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:31:44.349122 location-local-0.0.2/location_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-18 07:31:44.000000 location-local-0.0.2/location_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-18 07:31:44.000000 location-local-0.0.2/location_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:31:44.000000 location-local-0.0.2/location_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 07:31:44.000000 location-local-0.0.2/location_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 07:31:44.349122 location-local-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-18 07:31:32.000000 location-local-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:59:06.194961 location-local-0.0.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:59:06.190961 location-local-0.0.3/CirclesGetCountryName/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 07:58:53.000000 location-local-0.0.3/CirclesGetCountryName/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-07-18 07:58:53.000000 location-local-0.0.3/CirclesGetCountryName/opencage_get_country_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-18 07:59:06.194961 location-local-0.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 07:59:06.190961 location-local-0.0.3/location_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-07-18 07:59:06.000000 location-local-0.0.3/location_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-07-18 07:59:06.000000 location-local-0.0.3/location_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 07:59:06.000000 location-local-0.0.3/location_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-18 07:59:06.000000 location-local-0.0.3/location_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-18 07:59:06.194961 location-local-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-07-18 07:58:53.000000 location-local-0.0.3/setup.py
```

### Comparing `location-local-0.0.2/CirclesGetCountryName/opencage_get_country_name.py` & `location-local-0.0.3/CirclesGetCountryName/opencage_get_country_name.py`

 * *Files identical despite different names*

### Comparing `location-local-0.0.2/setup.py` & `location-local-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import setuptools
 # used by python -m build
 # python -m build needs pyproject.toml or setup.py
 setuptools.setup(
      # TODO: Please update the name
      name='location-local',
-     version='0.0.2',
+     version='0.0.3',
      author="Circles",
      author_email="info@circles.life",
      description="PyPI Package for Circles Local OpenCage Python",
      long_description="This is a package for sharing common OpenCage function used in different repositories",
      long_description_content_type="text/markdown",
      url="https://github.com/javatechy/dokr",
      packages=setuptools.find_packages(),
```

