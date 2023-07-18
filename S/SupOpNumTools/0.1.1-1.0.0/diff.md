# Comparing `tmp/SupOpNumTools-0.1.1.tar.gz` & `tmp/SupOpNumTools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SupOpNumTools-0.1.1.tar", last modified: Mon Apr 24 16:07:51 2023, max compression
+gzip compressed data, was "SupOpNumTools-1.0.0.tar", last modified: Tue Jul 18 15:40:51 2023, max compression
```

## Comparing `SupOpNumTools-0.1.1.tar` & `SupOpNumTools-1.0.0.tar`

### file list

```diff
@@ -1,49 +1,178 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:07:51.812992 SupOpNumTools-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:07:51.804992 SupOpNumTools-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:07:51.808992 SupOpNumTools-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/.github/workflows/python-pipy.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-24 16:07:51.812992 SupOpNumTools-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-24 16:07:51.812992 SupOpNumTools-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:07:51.804992 SupOpNumTools-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:07:51.808992 SupOpNumTools-0.1.1/src/SupOpNumTools/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:07:51.808992 SupOpNumTools-0.1.1/src/SupOpNumTools/elec_modeling/
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/elec_modeling/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:07:51.808992 SupOpNumTools-0.1.1/src/SupOpNumTools/elec_modeling/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/elec_modeling/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/elec_modeling/__pycache__/elec_modeling_photodetection.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/elec_modeling/__pycache__/photodetection.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/elec_modeling/photodetection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:07:51.808992 SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:07:51.808992 SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/__pycache__/M2DFilesDatabase.cpython-37.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/__pycache__/M2DFilesDatabase.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      205 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/__pycache__/math_phys_methods.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/__pycache__/signal_processing.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/math_phys_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:07:51.808992 SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:07:51.812992 SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/__pycache__/
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/__pycache__/M2DFilesDatabase.cpython-37.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/__pycache__/M2DFilesDatabase.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0 runner    (1001) docker     (123)      491 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/__pycache__/signal_processing.cpython-37.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/__pycache__/signal_processing.cpython-39.pyc
--rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/signal_processing.py
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-24 16:07:37.000000 SupOpNumTools-0.1.1/src/SupOpNumTools/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 16:07:51.808992 SupOpNumTools-0.1.1/src/SupOpNumTools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-04-24 16:07:51.000000 SupOpNumTools-0.1.1/src/SupOpNumTools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-24 16:07:51.000000 SupOpNumTools-0.1.1/src/SupOpNumTools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 16:07:51.000000 SupOpNumTools-0.1.1/src/SupOpNumTools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-04-24 16:07:51.000000 SupOpNumTools-0.1.1/src/SupOpNumTools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-24 16:07:51.000000 SupOpNumTools-0.1.1/src/SupOpNumTools.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.637136 SupOpNumTools-1.0.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.609136 SupOpNumTools-1.0.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.617136 SupOpNumTools-1.0.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/.github/workflows/python-pipy.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/.github/workflows/python-sphinx.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6653 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/GitBestPractices.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4515 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/GitTips.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-18 15:40:51.637136 SupOpNumTools-1.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.617136 SupOpNumTools-1.0.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/.buildinfo
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.617136 SupOpNumTools-1.0.0/docs/.doctrees/
+-rw-r--r--   0 runner    (1001) docker     (123)    24676 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/.doctrees/environment.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)     6785 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/.doctrees/index.doctree
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.617136 SupOpNumTools-1.0.0/docs/.doctrees/whatsincluded/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/.doctrees/whatsincluded/whatsincluded.doctree
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/.nojekyll
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.617136 SupOpNumTools-1.0.0/docs/_sources/
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/_sources/index.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.617136 SupOpNumTools-1.0.0/docs/_sources/whatsincluded/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/_sources/whatsincluded/whatsincluded.rst.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.621136 SupOpNumTools-1.0.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14813 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/_static/basic.css
+-rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/_static/doctools.js
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/_static/documentation_options.js
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/_static/file.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/_static/language_data.js
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/_static/minus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     4208 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/_static/nature.css
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/_static/plus.png
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/_static/pygments.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18215 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/_static/searchtools.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4712 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/_static/sphinx_highlight.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2794 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/genindex.html
+-rw-r--r--   0 runner    (1001) docker     (123)     6487 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/objects.inv
+-rw-r--r--   0 runner    (1001) docker     (123)     3097 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/search.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1929 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/searchindex.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.621136 SupOpNumTools-1.0.0/docs/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1161 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/source/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.621136 SupOpNumTools-1.0.0/docs/source/whatsincluded/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/source/whatsincluded/whatsincluded.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.621136 SupOpNumTools-1.0.0/docs/whatsincluded/
+-rw-r--r--   0 runner    (1001) docker     (123)     4662 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/docs/whatsincluded/whatsincluded.html
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-07-18 15:40:51.637136 SupOpNumTools-1.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.609136 SupOpNumTools-1.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.621136 SupOpNumTools-1.0.0/src/SupOpNumTools/
+-rw-r--r--   0 runner    (1001) docker     (123)      524 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.625136 SupOpNumTools-1.0.0/src/SupOpNumTools/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/__pycache__/__init__.cpython-39.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.625136 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.625136 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/__pycache__/camera.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/__pycache__/camera.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    29360 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/__pycache__/cameraBasler.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    26088 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/__pycache__/cameraIDS.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    12451 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/__pycache__/cameraIDS.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    13349 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/__pycache__/cameraIDSdisplay.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    27765 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/__pycache__/cameraIDSdisplayQt6.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     6995 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/__pycache__/cameraIDSdisplayQt6.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/camera.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18336 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/cameraBasler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15520 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/cameraIDS.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7125 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/cameraIDSdisplay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/camera/cameraIDSdisplayQt6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.629136 SupOpNumTools-1.0.0/src/SupOpNumTools/drivers/
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/drivers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.629136 SupOpNumTools-1.0.0/src/SupOpNumTools/drivers/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/drivers/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     9185 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/drivers/__pycache__/piezoNucleo.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     7180 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/drivers/piezoNucleo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.629136 SupOpNumTools-1.0.0/src/SupOpNumTools/elecmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/elecmodel/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.629136 SupOpNumTools-1.0.0/src/SupOpNumTools/elecmodel/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/elecmodel/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/elecmodel/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/elecmodel/__pycache__/elec_modeling_photodetection.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/elecmodel/__pycache__/photodetection.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/elecmodel/__pycache__/photodetection.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/elecmodel/photodetection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/essai_TD10.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.629136 SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.629136 SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__pycache__/M2DFilesDatabase.cpython-37.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__pycache__/M2DFilesDatabase.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      205 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2747 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__pycache__/math_phys_methods.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__pycache__/math_phys_methods.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1849 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__pycache__/signal_processing.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/math_phys_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10000 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/physics_demo_systems_PHOTO.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13733 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/physics_demo_systems_ali.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.629136 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt5/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.629136 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt5/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt5/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt5/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    23817 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt5/__pycache__/widgets.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt5/__pycache__/widgets.cpython-39.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.629136 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt5/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    53448 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt5/data/logo_lense.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    13151 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt5/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.629136 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/
+-rw-r--r--   0 runner    (1001) docker     (123)    15091 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/CameraWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/HistWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9340 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/SliderBlock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2611 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/TimeChartWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/XYChartWidget.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.633136 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)    11467 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/__pycache__/HistWidget.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    16034 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/__pycache__/SliderBlock.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/__pycache__/TimeChartWidget.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2589 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/__pycache__/TimeChartWidget.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    10975 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/__pycache__/XYChartWidget.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     5529 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/__pycache__/XYChartWidget.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/__pycache__/widgets.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/__pycache__/widgets.cpython-39.pyc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.633136 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    53448 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/data/logo_lense.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)     6637 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/pyqt6/widgets.py
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.633136 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.633136 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/M2DFilesDatabase.cpython-37.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     4306 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/M2DFilesDatabase.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2952 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/main.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     3722 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/sig1D.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2953 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/sig1D.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/signal_processing.cpython-37.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2958 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/signal_processing.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/test_signal.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/sig1D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.633136 SupOpNumTools-1.0.0/src/SupOpNumTools/sig2D/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig2D/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.633136 SupOpNumTools-1.0.0/src/SupOpNumTools/sig2D/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig2D/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig2D/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig2D/__pycache__/main.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     2356 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig2D/__pycache__/sig2D.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig2D/__pycache__/sig2D.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/sig2D/sig2D.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.633136 SupOpNumTools-1.0.0/src/SupOpNumTools/systemSimu/
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/systemSimu/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.637136 SupOpNumTools-1.0.0/src/SupOpNumTools/systemSimu/__pycache__/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/systemSimu/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/systemSimu/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/systemSimu/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)    12164 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/systemSimu/__pycache__/systemSimu.cpython-311.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     8225 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/systemSimu/__pycache__/systemSimu.cpython-37.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     8214 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/systemSimu/__pycache__/systemSimu.cpython-39.pyc
+-rw-r--r--   0 runner    (1001) docker     (123)     7098 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/systemSimu/systemSimu.py
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-07-18 15:40:37.000000 SupOpNumTools-1.0.0/src/SupOpNumTools/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-18 15:40:51.625136 SupOpNumTools-1.0.0/src/SupOpNumTools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-07-18 15:40:51.000000 SupOpNumTools-1.0.0/src/SupOpNumTools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6683 2023-07-18 15:40:51.000000 SupOpNumTools-1.0.0/src/SupOpNumTools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-18 15:40:51.000000 SupOpNumTools-1.0.0/src/SupOpNumTools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-07-18 15:40:51.000000 SupOpNumTools-1.0.0/src/SupOpNumTools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-07-18 15:40:51.000000 SupOpNumTools-1.0.0/src/SupOpNumTools.egg-info/top_level.txt
```

### Comparing `SupOpNumTools-0.1.1/.github/workflows/python-pipy.yml` & `SupOpNumTools-1.0.0/.github/workflows/python-pipy.yml`

 * *Files identical despite different names*

### Comparing `SupOpNumTools-0.1.1/LICENCE` & `SupOpNumTools-1.0.0/LICENCE`

 * *Files identical despite different names*

### Comparing `SupOpNumTools-0.1.1/pyproject.toml` & `SupOpNumTools-1.0.0/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -3,21 +3,21 @@
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools_scm]
 
 
 [project]
 name = "SupOpNumTools"
-version = "0.1.1"
+version = "1.0.0"
 authors = [
   { name="Julien VILLEMEJANE", email="julien.villemejane@institutoptique.fr" },
 ]
 description = "Package for engineer in physics and photonics"
 readme = "README.md"
-requires-python = ">=3.7"
+requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License"
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/IOGS-Digital-Methods/SupOpNumTools"
```

### Comparing `SupOpNumTools-0.1.1/setup.cfg` & `SupOpNumTools-1.0.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -2,23 +2,23 @@
 name = SupOpNumTools
 description = Package for engineer in physics and photonics
 long_description_content_type = text/markdown
 url = https://github.com/IOGS-Digital-Methods/SupOpNumTools
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
-version = "0.1.1"
+version = "1.0.0"
 authors = { name="Example Author", email="author@example.com" }
 readme = "README.md"
 
 [options]
 package_dir = 
 	= src
 packages = find:
-python_requires = >=3.7
+python_requires = >=3.9
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	gha_python_packaging_demo = gha_python_packaging_demo.app:entry_point
```

### Comparing `SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/__pycache__/M2DFilesDatabase.cpython-37.pyc` & `SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__pycache__/M2DFilesDatabase.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/__pycache__/M2DFilesDatabase.cpython-38.pyc` & `SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__pycache__/M2DFilesDatabase.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/__pycache__/__init__.cpython-39.pyc` & `SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__pycache__/__init__.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Mon Apr 24 14:17:02 2023 UTC, .py size: 383 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 5e8f 4664 7f01 0000  a.......^.Fd....
+00000000: 610d 0d0a 0000 0000 f461 8764 7f01 0000  a........a.d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2400 0000 6400  .....@...s$...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6503  Z.d.d.l.m.Z...e.
 00000040: 6403 6b02 7220 6504 6404 8301 0100 6405  d.k.r e.d.....d.
 00000050: 5300 2906 7ae1 0a4e 756d 6572 6963 616c  S.).z..Numerical
 00000060: 204d 6574 686f 6473 2066 6f72 204d 6174   Methods for Mat
 00000070: 6873 2061 6e64 2050 6879 7369 6373 0a0a  hs and Physics..
@@ -21,14 +21,15 @@
 00000140: 6d61 7468 5f70 6879 735f 6d65 7468 6f64  math_phys_method
 00000150: 73da 085f 5f6d 6169 6e5f 5f7a 274e 756d  s..__main__z'Num
 00000160: 6572 6963 616c 204d 6574 686f 6473 2066  erical Methods f
 00000170: 6f72 204d 6174 6873 2061 6e64 2050 6879  or Maths and Phy
 00000180: 7369 6373 4e29 05da 075f 5f64 6f63 5f5f  sicsN)...__doc__
 00000190: da00 7202 0000 00da 085f 5f6e 616d 655f  ..r......__name_
 000001a0: 5fda 0570 7269 6e74 a900 7208 0000 0072  _..print..r....r
-000001b0: 0800 0000 fa4d 443a 5c74 6f6f 6c73 5c67  .....MD:\tools\g
-000001c0: 6974 5f72 6570 6f5c 5375 704f 7054 6f6f  it_repo\SupOpToo
-000001d0: 6c62 6f78 5c73 7263 5c53 7570 4f70 546f  lbox\src\SupOpTo
-000001e0: 6f6c 626f 785c 6d61 7468 5f70 6879 735f  olbox\math_phys_
-000001f0: 6d65 7468 6f64 735c 5f5f 696e 6974 5f5f  methods\__init__
-00000200: 2e70 79da 083c 6d6f 6475 6c65 3e02 0000  .py..<module>...
-00000210: 0073 0600 0000 040a 0c02 0801            .s..........
+000001b0: 0800 0000 fa5c 443a 5c74 6f6f 6c73 5c67  .....\D:\tools\g
+000001c0: 6974 5f72 6570 6f5c 6a76 696c 6c65 6d65  it_repo\jvilleme
+000001d0: 6a61 6e65 5c74 6573 7453 7570 4f70 4e75  jane\testSupOpNu
+000001e0: 6d54 6f6f 6c73 5c53 7570 4f70 4e75 6d54  mTools\SupOpNumT
+000001f0: 6f6f 6c73 5c6d 6174 685f 7068 7973 5f6d  ools\math_phys_m
+00000200: 6574 686f 6473 5c5f 5f69 6e69 745f 5f2e  ethods\__init__.
+00000210: 7079 da08 3c6d 6f64 756c 653e 0200 0000  py..<module>....
+00000220: 7306 0000 0004 0a0c 0208 01              s..........
```

### Comparing `SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/__pycache__/math_phys_methods.cpython-39.pyc` & `SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__pycache__/math_phys_methods.cpython-39.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.9, timestamp-based, .py timestamp: Fri Dec  9 13:27:20 2022 UTC, .py size: 1914 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 610d 0d0a 0000 0000 b837 9363 7a07 0000  a........7.cz...
+00000000: 610d 0d0a 0000 0000 f461 8764 7a07 0000  a........a.dz...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0002 0000 0040 0000 0073 2c00 0000 6400  .....@...s,...d.
 00000030: 5a00 6401 6402 6c01 6d02 5a02 0100 6401  Z.d.d.l.m.Z...d.
 00000040: 6403 6c03 5a04 6404 6405 8400 5a05 6406  d.l.Z.d.d...Z.d.
 00000050: 6407 8400 5a06 6403 5300 2908 7ae1 0a4e  d...Z.d.S.).z..N
 00000060: 756d 6572 6963 616c 204d 6574 686f 6473  umerical Methods
 00000070: 2066 6f72 204d 6174 6873 2061 6e64 2050   for Maths and P
@@ -61,65 +61,66 @@
 000003c0: 696f 6e20 6e75 6d62 6572 2e0a 0a20 2020  ion number...   
 000003d0: 2072 0100 0000 7a26 6572 7265 7572 203a   r....z&erreur :
 000003e0: 2069 6c20 6661 7574 2061 6772 616e 6469   il faut agrandi
 000003f0: 7220 6c27 696e 7465 7276 616c 6c65 e964  r l'intervalle.d
 00000400: 0000 00e9 0200 0000 e901 0000 0029 02da  .............)..
 00000410: 0570 7269 6e74 da03 6162 7329 06da 0146  .print..abs)...F
 00000420: da01 61da 0162 da03 746f 6cda 0169 da01  ..a..b..tol..i..
-00000430: 78a9 0072 0e00 0000 fa56 443a 5c74 6f6f  x..r.....VD:\too
-00000440: 6c73 5c67 6974 5f72 6570 6f5c 5375 704f  ls\git_repo\SupO
-00000450: 7054 6f6f 6c62 6f78 5c73 7263 5c53 7570  pToolbox\src\Sup
-00000460: 4f70 546f 6f6c 626f 785c 6d61 7468 5f70  OpToolbox\math_p
-00000470: 6879 735f 6d65 7468 6f64 735c 6d61 7468  hys_methods\math
-00000480: 5f70 6879 735f 6d65 7468 6f64 732e 7079  _phys_methods.py
-00000490: da09 6269 7365 6374 696f 6e10 0000 0073  ..bisection....s
-000004a0: 1600 0000 0018 1401 0802 0401 0401 1801  ................
-000004b0: 0c01 1401 0602 0401 0a01 7210 0000 0063  ..........r....c
-000004c0: 0400 0000 0000 0000 0000 0000 0900 0000  ................
-000004d0: 0300 0000 4300 0000 7356 0000 0064 017d  ....C...sV...d.}
-000004e0: 047c 027d 0574 007c 007c 0583 0183 017c  .|.}.t.|.|.....|
-000004f0: 036b 0472 4e7c 0464 026b 0072 4e7c 007c  .k.rN|.d.k.rN|.|
-00000500: 0583 017c 017c 0583 0102 007d 067d 077c  ...|.|.....}.}.|
-00000510: 060b 007c 071b 007d 087c 057c 0817 007d  ...|...}.|.|...}
-00000520: 057c 0464 0337 007d 0471 087c 057c 0466  .|.d.7.}.q.|.|.f
-00000530: 0253 0029 0461 b601 0000 0a20 2020 2043  .S.).a.....    C
-00000540: 616c 6375 6c61 7465 7320 7468 6520 6170  alculates the ap
-00000550: 7072 6f78 696d 6174 6976 6520 7661 6c75  proximative valu
-00000560: 6520 6f66 2061 2072 6f6f 7420 6f66 2061  e of a root of a
-00000570: 2066 756e 6374 696f 6e20 0a20 2020 2062   function .    b
-00000580: 7920 7468 6520 4e65 7774 6f6e 206d 6574  y the Newton met
-00000590: 686f 640a 0a20 2020 2050 6172 616d 6574  hod..    Paramet
-000005a0: 6572 730a 2020 2020 2d2d 2d2d 2d2d 2d2d  ers.    --------
-000005b0: 2d2d 0a20 2020 2046 203a 2066 756e 6374  --.    F : funct
-000005c0: 696f 6e0a 2020 2020 2020 2020 6d61 7468  ion.        math
-000005d0: 656d 6174 6963 616c 2066 756e 6374 696f  ematical functio
-000005e0: 6e2e 0a20 2020 2064 4620 3a20 6675 6e63  n..    dF : func
-000005f0: 7469 6f6e 0a20 2020 2020 2020 2064 6572  tion.        der
-00000600: 6976 6174 6520 6f66 2074 6865 2066 756e  ivate of the fun
-00000610: 6374 696f 6e20 462e 0a20 2020 2078 3020  ction F..    x0 
-00000620: 3a20 646f 7562 6c65 0a20 2020 2020 2020  : double.       
-00000630: 2069 6e69 7469 616c 2076 616c 7565 2e0a   initial value..
-00000640: 2020 2020 746f 6c20 3a20 646f 7562 6c65      tol : double
-00000650: 0a20 2020 2020 2020 2063 616c 6375 6c61  .        calcula
-00000660: 7469 6f6e 2074 6f6c 6572 616e 6365 2e0a  tion tolerance..
-00000670: 0a20 2020 2052 6574 7572 6e73 0a20 2020  .    Returns.   
-00000680: 202d 2d2d 2d2d 2d2d 0a20 2020 2078 203a   -------.    x :
-00000690: 2064 6f75 626c 650a 2020 2020 2020 2020   double.        
-000006a0: 6170 7072 6f78 696d 6174 6976 6520 7661  approximative va
-000006b0: 6c75 6520 6f66 2074 6865 2072 6f6f 742e  lue of the root.
-000006c0: 0a20 2020 2069 203a 2069 6e74 6567 6572  .    i : integer
-000006d0: 0a20 2020 2020 2020 2069 7465 7261 7469  .        iterati
-000006e0: 6f6e 206e 756d 6265 722e 0a0a 2020 2020  on number...    
-000006f0: 7201 0000 0072 0300 0000 7205 0000 0029  r....r....r....)
-00000700: 0172 0700 0000 2909 7208 0000 005a 0264  .r....).r....Z.d
-00000710: 46da 0278 3072 0b00 0000 720c 0000 0072  F..x0r....r....r
-00000720: 0d00 0000 da01 79da 0264 79da 0264 7872  ......y..dy..dxr
-00000730: 0e00 0000 720e 0000 0072 0f00 0000 da10  ....r....r......
-00000740: 6e65 7774 6f6e 5f66 696e 645f 726f 6f74  newton_find_root
-00000750: 3700 0000 7310 0000 0000 1804 0104 0118  7...s...........
-00000760: 0112 010a 0108 010a 0172 1500 0000 2907  .........r....).
-00000770: da07 5f5f 646f 635f 5f5a 0573 6369 7079  ..__doc__Z.scipy
-00000780: 7202 0000 00da 056e 756d 7079 da02 6e70  r......numpy..np
-00000790: 7210 0000 0072 1500 0000 720e 0000 0072  r....r....r....r
-000007a0: 0e00 0000 720e 0000 0072 0f00 0000 da08  ....r....r......
-000007b0: 3c6d 6f64 756c 653e 0200 0000 7308 0000  <module>....s...
-000007c0: 0004 0a0c 0108 0308 27                   ........'
+00000430: 78a9 0072 0e00 0000 fa65 443a 5c74 6f6f  x..r.....eD:\too
+00000440: 6c73 5c67 6974 5f72 6570 6f5c 6a76 696c  ls\git_repo\jvil
+00000450: 6c65 6d65 6a61 6e65 5c74 6573 7453 7570  lemejane\testSup
+00000460: 4f70 4e75 6d54 6f6f 6c73 5c53 7570 4f70  OpNumTools\SupOp
+00000470: 4e75 6d54 6f6f 6c73 5c6d 6174 685f 7068  NumTools\math_ph
+00000480: 7973 5f6d 6574 686f 6473 5c6d 6174 685f  ys_methods\math_
+00000490: 7068 7973 5f6d 6574 686f 6473 2e70 79da  phys_methods.py.
+000004a0: 0962 6973 6563 7469 6f6e 1000 0000 7316  .bisection....s.
+000004b0: 0000 0000 1814 0108 0204 0104 0118 010c  ................
+000004c0: 0114 0106 0204 010a 0172 1000 0000 6304  .........r....c.
+000004d0: 0000 0000 0000 0000 0000 0009 0000 0003  ................
+000004e0: 0000 0043 0000 0073 5600 0000 6401 7d04  ...C...sV...d.}.
+000004f0: 7c02 7d05 7400 7c00 7c05 8301 8301 7c03  |.}.t.|.|.....|.
+00000500: 6b04 724e 7c04 6402 6b00 724e 7c00 7c05  k.rN|.d.k.rN|.|.
+00000510: 8301 7c01 7c05 8301 0200 7d06 7d07 7c06  ..|.|.....}.}.|.
+00000520: 0b00 7c07 1b00 7d08 7c05 7c08 1700 7d05  ..|...}.|.|...}.
+00000530: 7c04 6403 3700 7d04 7108 7c05 7c04 6602  |.d.7.}.q.|.|.f.
+00000540: 5300 2904 61b6 0100 000a 2020 2020 4361  S.).a.....    Ca
+00000550: 6c63 756c 6174 6573 2074 6865 2061 7070  lculates the app
+00000560: 726f 7869 6d61 7469 7665 2076 616c 7565  roximative value
+00000570: 206f 6620 6120 726f 6f74 206f 6620 6120   of a root of a 
+00000580: 6675 6e63 7469 6f6e 200a 2020 2020 6279  function .    by
+00000590: 2074 6865 204e 6577 746f 6e20 6d65 7468   the Newton meth
+000005a0: 6f64 0a0a 2020 2020 5061 7261 6d65 7465  od..    Paramete
+000005b0: 7273 0a20 2020 202d 2d2d 2d2d 2d2d 2d2d  rs.    ---------
+000005c0: 2d0a 2020 2020 4620 3a20 6675 6e63 7469  -.    F : functi
+000005d0: 6f6e 0a20 2020 2020 2020 206d 6174 6865  on.        mathe
+000005e0: 6d61 7469 6361 6c20 6675 6e63 7469 6f6e  matical function
+000005f0: 2e0a 2020 2020 6446 203a 2066 756e 6374  ..    dF : funct
+00000600: 696f 6e0a 2020 2020 2020 2020 6465 7269  ion.        deri
+00000610: 7661 7465 206f 6620 7468 6520 6675 6e63  vate of the func
+00000620: 7469 6f6e 2046 2e0a 2020 2020 7830 203a  tion F..    x0 :
+00000630: 2064 6f75 626c 650a 2020 2020 2020 2020   double.        
+00000640: 696e 6974 6961 6c20 7661 6c75 652e 0a20  initial value.. 
+00000650: 2020 2074 6f6c 203a 2064 6f75 626c 650a     tol : double.
+00000660: 2020 2020 2020 2020 6361 6c63 756c 6174          calculat
+00000670: 696f 6e20 746f 6c65 7261 6e63 652e 0a0a  ion tolerance...
+00000680: 2020 2020 5265 7475 726e 730a 2020 2020      Returns.    
+00000690: 2d2d 2d2d 2d2d 2d0a 2020 2020 7820 3a20  -------.    x : 
+000006a0: 646f 7562 6c65 0a20 2020 2020 2020 2061  double.        a
+000006b0: 7070 726f 7869 6d61 7469 7665 2076 616c  pproximative val
+000006c0: 7565 206f 6620 7468 6520 726f 6f74 2e0a  ue of the root..
+000006d0: 2020 2020 6920 3a20 696e 7465 6765 720a      i : integer.
+000006e0: 2020 2020 2020 2020 6974 6572 6174 696f          iteratio
+000006f0: 6e20 6e75 6d62 6572 2e0a 0a20 2020 2072  n number...    r
+00000700: 0100 0000 7203 0000 0072 0500 0000 2901  ....r....r....).
+00000710: 7207 0000 0029 0972 0800 0000 5a02 6446  r....).r....Z.dF
+00000720: da02 7830 720b 0000 0072 0c00 0000 720d  ..x0r....r....r.
+00000730: 0000 00da 0179 da02 6479 da02 6478 720e  .....y..dy..dxr.
+00000740: 0000 0072 0e00 0000 720f 0000 00da 106e  ...r....r......n
+00000750: 6577 746f 6e5f 6669 6e64 5f72 6f6f 7437  ewton_find_root7
+00000760: 0000 0073 1000 0000 0018 0401 0401 1801  ...s............
+00000770: 1201 0a01 0801 0a01 7215 0000 0029 07da  ........r....)..
+00000780: 075f 5f64 6f63 5f5f da05 7363 6970 7972  .__doc__..scipyr
+00000790: 0200 0000 da05 6e75 6d70 79da 026e 7072  ......numpy..npr
+000007a0: 1000 0000 7215 0000 0072 0e00 0000 720e  ....r....r....r.
+000007b0: 0000 0072 0e00 0000 720f 0000 00da 083c  ...r....r......<
+000007c0: 6d6f 6475 6c65 3e02 0000 0073 0800 0000  module>....s....
+000007d0: 040a 0c01 0803 0827                      .......'
```

### Comparing `SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/__pycache__/signal_processing.cpython-39.pyc` & `SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/__pycache__/signal_processing.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `SupOpNumTools-0.1.1/src/SupOpNumTools/math_phys_methods/math_phys_methods.py` & `SupOpNumTools-1.0.0/src/SupOpNumTools/math_phys_methods/math_phys_methods.py`

 * *Files identical despite different names*

### Comparing `SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/__pycache__/M2DFilesDatabase.cpython-37.pyc` & `SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/M2DFilesDatabase.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/__pycache__/M2DFilesDatabase.cpython-38.pyc` & `SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/M2DFilesDatabase.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/__pycache__/signal_processing.cpython-37.pyc` & `SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/signal_processing.cpython-37.pyc`

 * *Files identical despite different names*

### Comparing `SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/__pycache__/signal_processing.cpython-39.pyc` & `SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/__pycache__/signal_processing.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `SupOpNumTools-0.1.1/src/SupOpNumTools/signal_processing/signal_processing.py` & `SupOpNumTools-1.0.0/src/SupOpNumTools/sig1D/sig1D.py`

 * *Files identical despite different names*

